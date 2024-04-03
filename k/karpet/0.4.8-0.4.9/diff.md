# Comparing `tmp/karpet-0.4.8.tar.gz` & `tmp/karpet-0.4.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "karpet-0.4.8.tar", max compression
+gzip compressed data, was "karpet-0.4.9.tar", max compression
```

## Comparing `karpet-0.4.8.tar` & `karpet-0.4.9.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1059 2019-11-24 12:59:27.263983 karpet-0.4.8/LICENSE
--rw-r--r--   0        0        0     9055 2023-01-18 09:10:06.333998 karpet-0.4.8/README.rst
--rw-r--r--   0        0        0       33 2019-11-24 12:59:27.267983 karpet-0.4.8/karpet/__init__.py
--rw-r--r--   0        0        0    23195 2023-01-17 09:06:42.895428 karpet-0.4.8/karpet/core.py
--rw-r--r--   0        0        0       22 2022-11-27 20:42:12.519119 karpet-0.4.8/karpet/meta.py
--rw-r--r--   0        0        0      244 2022-11-27 20:42:22.195224 karpet-0.4.8/karpet/utils.py
--rw-r--r--   0        0        0      896 2023-01-18 09:10:14.082081 karpet-0.4.8/pyproject.toml
--rw-r--r--   0        0        0    10408 2023-01-18 09:13:37.388529 karpet-0.4.8/setup.py
--rw-r--r--   0        0        0    10124 2023-01-18 09:13:37.389214 karpet-0.4.8/PKG-INFO
+-rw-r--r--   0        0        0     1059 2019-11-24 12:59:27.263983 karpet-0.4.9/LICENSE
+-rw-r--r--   0        0        0     9087 2023-01-30 10:27:43.763136 karpet-0.4.9/README.rst
+-rw-r--r--   0        0        0       33 2019-11-24 12:59:27.267983 karpet-0.4.9/karpet/__init__.py
+-rw-r--r--   0        0        0    23787 2023-01-30 10:26:08.278092 karpet-0.4.9/karpet/core.py
+-rw-r--r--   0        0        0       22 2022-11-27 20:42:12.519119 karpet-0.4.9/karpet/meta.py
+-rw-r--r--   0        0        0      244 2022-11-27 20:42:22.195224 karpet-0.4.9/karpet/utils.py
+-rw-r--r--   0        0        0      896 2023-01-30 10:32:13.366082 karpet-0.4.9/pyproject.toml
+-rw-r--r--   0        0        0    10444 2023-01-30 10:32:17.170832 karpet-0.4.9/setup.py
+-rw-r--r--   0        0        0    10156 2023-01-30 10:32:17.171583 karpet-0.4.9/PKG-INFO
```

### Comparing `karpet-0.4.8/LICENSE` & `karpet-0.4.9/LICENSE`

 * *Files identical despite different names*

### Comparing `karpet-0.4.8/README.rst` & `karpet-0.4.9/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -236,14 +236,18 @@
     2023-01-16 21:00:00  1592.68  1593.66  1584.71  1587.87
     2023-01-16 21:30:00  1587.28  1587.28  1583.13  1583.13
     2023-01-16 22:00:00  1573.99  1580.11  1573.99  1579.97
 
 Changelog
 ---------
 
+0.4.9
+~~~~~
+- new retry policy
+
 0.4.8
 ~~~~~
 - new ``fetch_crypto_live_data()``
 
 0.4.7.
 ~~~~~~
 - dependencies updated
```

### Comparing `karpet-0.4.8/karpet/core.py` & `karpet-0.4.9/karpet/core.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,37 +1,62 @@
 try:
     from pytrends.request import TrendReq
 except:
     pass
 
 import asyncio
 import time
-from datetime import date, datetime, timedelta
+from datetime import datetime, timedelta
 
 import aiohttp
 import numpy as np
 import pandas as pd
 import requests
 from bs4 import BeautifulSoup
+from requests.adapters import HTTPAdapter, Retry
 
 
 class Karpet:
 
     quick_search_data = None
+    req_retries = 4
+    req_backoff_factor = 3
 
     def __init__(self, start=None, end=None):
         """
         Constructor.
 
         :param datetime.date start: History data begining.
         :param datetime.date end: History data end.
         """
 
         self.start = start
         self.end = end
+        self.req_ses = self.get_session()
+
+    def get_session(self):
+
+        # Waits for 1.5s, 3s, 6s, 12s, 24s between requests.
+        status_forcelist = (500, 502, 503, 504, 429)
+
+        retry = Retry(
+            total=self.req_retries,
+            read=self.req_retries,
+            connect=self.req_retries,
+            backoff_factor=self.req_backoff_factor,
+            status_forcelist=status_forcelist,
+            method_whitelist=False,
+        )
+        adapter = HTTPAdapter(max_retries=retry)
+
+        session = requests.Session()
+        # session.mount("http://", adapter)
+        session.mount("https://", adapter)
+
+        return session
 
     def get_quick_search_data(self):
         """
         Downloads JSON from coinmarketcap.com quick search
         widget. Data contains list of all cryptocurrencies
         where each item has following structure:
 
@@ -49,32 +74,20 @@
         }
 
         :raises Exception: In case of unreachable data or error during parsing.
         :return: Downloaded JSON data - for each item structure see above.
         :rtype: list
         """
 
-        if self.quick_search_data:
-            return self.quick_search_data
-
-        url = "https://s2.coinmarketcap.com/generated/search/quick_search.json"
-
-        # Download.
-        try:
-            response = requests.get(url)
-        except:
-            raise Exception("Couldn't download necessary data from the internet.")
-
-        # Parse.
-        try:
-            self.quick_search_data = response.json()
+        if not self.quick_search_data:
+            self.quick_search_data = self._get_json(
+                "https://s2.coinmarketcap.com/generated/search/quick_search.json"
+            )
 
-            return self.quick_search_data
-        except:
-            raise Exception("Couldn't parse downloaded data from the internet.")
+        return self.quick_search_data
 
     def fetch_crypto_historical_data(self, symbol=None, id=None):
         """
         Retrieve basic historical information (by days) for a specific
         cryptocurrency from coingecko.com.
         Coin ID can be retreived by get_coin_ids() method.
 
@@ -242,15 +255,20 @@
         if trdays > 270:
             raise ValueError("trdays must not exceed 270")
         if overlap >= trdays:
             raise ValueError("Overlap can't exceed search days")
 
         stich_overlap = trdays - overlap
         n_days = (self.end - self.start).days
-        pytrends = TrendReq(hl=hl, tz=tz)
+        pytrends = TrendReq(
+            hl=hl,
+            tz=tz,
+            retries=self.req_retries,
+            backoff_factor=self.req_backoff_factor,
+        )
 
         # Get the dates for each search.
         if n_days <= trdays:
             trend_dates = [
                 "{} {}".format(
                     self.start.strftime("%Y-%m-%d"), self.end.strftime("%Y-%m-%d")
                 )
@@ -398,15 +416,15 @@
             :return: Dict with ``editors_choice`` and ``hot_stories`` items.
             :rtype: dict
             """
 
             headers = {
                 "User-Agent": "Mozilla/5.0 (X11; Linux x86_64; rv:69.0) Gecko/20100101 Firefox/69.0"
             }
-            response = requests.get("https://cointelegraph.com/", headers=headers)
+            response = self.req_ses.get("https://cointelegraph.com/", headers=headers)
             dom = BeautifulSoup(response.text, "lxml")
 
             def parse_news(news_items):
                 """
                 Parse news URL from news LI HTML elements.
 
                 :param list news_items: List of LI HTML elements where A HTML elements sits.
@@ -669,18 +687,20 @@
         :param str url: URL to be scraped.
         :return: Parsed JSON data.
         :rtype: object or list
         """
 
         # Download.
         try:
-            response = requests.get(url)
+            response = self.req_ses.get(url)
         except:
             raise Exception("Couldn't download necessary data from the internet.")
 
+        response.raise_for_status()
+
         # Parse.
         try:
             return response.json()
         except:
             raise Exception("Couldn't parse downloaded data from the internet.")
 
     def _get_coin_id_from_params(self, symbol=None, id=None):
```

### Comparing `karpet-0.4.8/pyproject.toml` & `karpet-0.4.9/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "karpet"
-version = "0.4.8"
+version = "0.4.9"
 description = "Library for fetching coin/token historical data, trends and more."
 authors = ["n1 <hrdina.pavel@gmail.com>"]
 readme = "README.rst"
 homepage = "https://github.com/im-n1/karpet"
 classifiers = [
     "Programming Language :: Python :: 3.6",
     "License :: OSI Approved :: MIT License",
```

### Comparing `karpet-0.4.8/setup.py` & `karpet-0.4.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,17 +16,17 @@
  'requests>=2.22.0,<3.0.0']
 
 extras_require = \
 {'google': ['pytrends>=4.7.3,<5.0.0']}
 
 setup_kwargs = {
     'name': 'karpet',
-    'version': '0.4.8',
+    'version': '0.4.9',
     'description': 'Library for fetching coin/token historical data, trends and more.',
-    'long_description': '.. image:: https://raw.githubusercontent.com/im-n1/karpet/master/assets/logo.png\n   :align: center\n\n.. image:: https://img.shields.io/pypi/v/karpet.svg?color=0c7dbe\n   :alt: PyPI\n\n.. image:: https://img.shields.io/pypi/l/karpet.svg?color=0c7dbe\n   :alt: PyPI - License\n\n.. image:: https://img.shields.io/pypi/dm/karpet.svg?color=0c7dbe\n   :alt: PyPI - Downloads\n\n.. contents::\n\nKarpet\n======\nKarpet is a tiny library with just a few dependencies\nfor fetching coins/tokens metrics data from the internet.\n\nIt can provide following data:\n\n* coin/token historical price data (no limits)\n* google trends for the given list of keywords (longer period than official API)\n* twitter scraping for the given keywords (no limits)\n* much more info about crypto coins/tokens (no rate limits)\n\nWhat is upcoming?\n\n* Reddit metrics\n* Have a request? Open an issue ;)\n\nDependencies\n------------\nLibrary uses a few nifty dependencies and is Python 3.6+ only. There is no\nneed to install dependencies you don\'t need. Therefore this library utilizes\nextras which install optional dependencies:\n\n* for Google trends - google\n\nUsage\n-----\n1. Install the library via pip.\n\n.. code-block:: bash\n\n   pip install karpet  # Basics only\n   pip install karpet[google]  # For Google trends\n\n2. Import the library class first.\n\n.. code-block:: python\n\n    from karpet import Karpet\n\nfetch_crypto_historical_data()\n~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~\nRetrieves historical data.\n\n.. code-block:: python\n\n    k = Karpet(date(2019, 1, 1), date(2019, 5, 1))\n    df = k.fetch_crypto_historical_data(id="ethereum")  # Dataframe with historical data.\n    df.head()\n\n                     price   market_cap total_volume\n    2019-01-01  131.458725  1.36773e+10  1.36773e+10\n    2019-01-02  138.144802  1.43923e+10  1.43923e+10\n    2019-01-03  152.860453  1.59222e+10  1.59222e+10\n    2019-01-04  146.730599  1.52777e+10  1.52777e+10\n    2019-01-05  153.056567  1.59408e+10  1.59408e+10\n\n\nfetch_crypto_exchanges()\n~~~~~~~~~~~~~~~~~~~~~~~~\nRetrieves exchange list.\n\n.. code-block:: python\n\n    k = Karpet()\n    k.fetch_crypto_exchanges("nrg")\n    [\'DigiFinex\', \'KuCoin\', \'CryptoBridge\', \'Bitbns\', \'CoinExchange\']\n\nfetch_google_trends()\n~~~~~~~~~~~~~~~~~~~~~\nRetrieves Google Trends - in percents for the given date range.\n\n.. code-block:: python\n\n    k = Karpet(date(2019, 1, 1), date(2019, 5, 1))\n    df = k.fetch_google_trends(kw_list=["bitcoin"])  # Dataframe with trends.\n    df.head()\n\n.. image:: https://raw.githubusercontent.com/im-n1/karpet/master/assets/google_trends.png\n\nAnd with a few lines of code you can get a chart\n\n.. code-block:: python\n\n   df = df.set_index("date")\n   df.plot()\n\n.. image:: https://raw.githubusercontent.com/im-n1/karpet/master/assets/trends_chart.png\n\nfetch_news()\n~~~~~~~~~~~~\nRetrieves crypto news.\n\n.. code-block:: python\n\n   k = Karpet()\n   news = k.fetch_news("btc")  # Gets 10 news.\n   print(news[0])\n   {\n      \'url\': \'https://cointelegraph.com/ ....\',  # Truncated.\n      \'title\': \'Shell Invests in Blockchain-Based Energy Startup\',\n      \'description\': \'The world’s fifth top oil and gas firm, Shell, has...\',  # Truncated.\n      \'date\': datetime.datetime(2019, 7, 28, 9, 24, tzinfo=datetime.timezone(datetime.timedelta(seconds=3600)))\n      \'image\': \'https://images.cointelegraph.com/....jpg\'  # Truncated.\n   }\n   news = k.fetch_news("btc", limit=30)  # Gets 30 news.\n\nfetch_top_news()\n~~~~~~~~~~~~~~~~\nRetrieves top crypto news in 2 categories:\n\n* Editor\'s choices - articles picked by editors\n* Hot stories - articles with most views\n\n.. code-block:: python\n\n   k = Karpet()\n   editors_choices, top_stories = k.fetch_top_news()\n   print(len(editors_choices))\n   5\n   print(len(top_stories))\n   5\n   print(editors_choices[0])\n   {\n      \'url\': \'https://cointelegraph.com/...\',  # Truncated.\n      \'title\': \'Bank of China’s New Infographic Shows Why Bitcoin Price Is Going Up\',\n      \'date\': datetime.datetime(2019, 7, 27, 10, 7, tzinfo=datetime.timezone(datetime.timedelta(seconds=3600))),\n      \'image\': \'https://images.cointelegraph.com/images/740_aHR...\', # Truncated.\n      \'description\': \'The Chinese central bank released on its website an ...\'  # Truncated.\n   }\n   print(top_stories[0])\n   {\n      \'url\': \'https://cointelegraph.com/...\',  # Truncated.\n      \'title\': \'Bitcoin Price Shuns Volatility as Analysts Warn of Potential Drop to $7,000\',\n      \'date\': datetime.datetime(2019, 7, 27, 10, 7, tzinfo=datetime.timezone(datetime.timedelta(seconds=3600))),\n      \'image\': \'https://images.cointelegraph.com/images/740_aHR0c...\'  # Truncated.\n      \'description\': \'Stability around $10,600 for Bitcoin price is ...\'  # Truncated.\n   }\n\nget_coin_ids()\n~~~~~~~~~~~~~~\nResolves coin ID\'s based on the given symbol (there are coins out there with identical symbol).\n\nUse this to get distinctive coin ID which can be used as ``id`` param for\nmethod ``fetch_crypto_historical_data()``.\n\n.. code-block:: python\n\n    k = Karpet()\n    print(k.get_coin_ids("sta"))\n    [\'statera\']\n\n\nget_basic_data()\n~~~~~~~~~~~~~~~~\nFetches coin/token basic data like:\n\n``open_issues`` is only provided if ``total_issues`` and ``closed_issues`` are\navailable.\n\n.. code-block:: python\n\n    k = Karpet()\n    print(k.get_basic_data(id="ethereum"))\n    {\n        \'closed_issues\': 5530,\n        \'commit_count_4_weeks\': 40,\n        \'current_price\': 3167.67,\n        \'forks\': 11635,\n        \'market_cap\': 371964284548,\n        \'name\': \'Ethereum\',\n        \'open_issues\': 230,\n        \'pull_request_contributors\': 552,\n        \'rank\': 2,\n        \'reddit_accounts_active_48h\': 2881.0,\n        \'reddit_average_comments_48h\': 417.083,\n        \'reddit_average_posts_48h\': 417.083,\n        \'reddit_subscribers\': 1057875,\n        \'stars\': 31680,\n        \'total_issues\': 5760,\n        \'year_high\': 4182.790285752286,\n        \'year_low\': 321.0774351739628,\n        \'yoy_change\': 695.9225871929757,  # growth/drop in percents\n        \'price_change_24\': 120.1,\n        \'price_change_24_percents\': 1.23\n    }\n\nget_quick_search_data()\n~~~~~~~~~~~~~~~~~~~~~~~\nLists all coins/tokes with some basic info.\n\n.. code-block:: python\n\n    k = Karpet()\n    print(k.get_quick_search_data()[0])\n    {\n        "name": "Bitcoin",\n        "symbol": "BTC",\n        "rank": 1,\n        "slug": "bitcoin",\n        "tokens": [\n            "Bitcoin",\n            "bitcoin",\n            "BTC"\n        ],\n        "id": 1,\n    }\n\nfetch_crypto_live_data()\n~~~~~~~~~~~~~~~~~~~~~~~~\nRetrieves live market data.\n\n.. code-block:: python\n\n    k = Karpet()\n    df = k.fetch_crypto_live_data(id="ethereum")  # Dataframe with live data.\n    df.head()\n\n                            open     high      low    close\n    2023-01-16 20:00:00  1593.01  1595.05  1593.01  1594.28\n    2023-01-16 20:30:00  1593.37  1593.37  1589.03  1589.35\n    2023-01-16 21:00:00  1592.68  1593.66  1584.71  1587.87\n    2023-01-16 21:30:00  1587.28  1587.28  1583.13  1583.13\n    2023-01-16 22:00:00  1573.99  1580.11  1573.99  1579.97\n\nChangelog\n---------\n\n0.4.8\n~~~~~\n- new ``fetch_crypto_live_data()``\n\n0.4.7.\n~~~~~~\n- dependencies updated\n- news with non UTF-8 chars handled and dropped\n- fixed code formatting\n\n0.4.6\n~~~~~\n- new ``price_change_24`` and ``price_change_24_percents`` properties for ``get_basic_data()``\n- new ``get_quick_search_data()``\n\n0.4.5\n~~~~~\n- fixed dependencies\n\n0.4.4\n~~~~~\n- removed obsolete parts of the code and some dependencies\n\n0.4.3\n~~~~~\n- fixed ``get_basic_data()`` method (different data source)\n- new property in ``get_basic_data()`` return dict - ``rank``\n- tests enhanced\n\n0.4.2\n~~~~~\n- fixed minor bugs\n\n0.4.1\n~~~~~\n- new data in ``get_basic_data()`` method - ``year_low``, ``year_high``, ``yoy_change``\n\n0.4\n~~~\n- new method ``get_basic_data()``\n\n0.3.3\n~~~~~\n- removed twitter integration - twitterscraper library is not up to date\n- fixed news fetching\n\n\n0.3.2\n~~~~~\n- new method ``get_coin_ids()``\n- method ``fetch_crypto_historical_data()`` has ``id`` param now\n\n0.3.1\n~~~~~\n- migrated to coingecko.com API (no API key needed anymore)\n\n0.3\n~~~\n- migrated to cryptocompare.com API (you need an API key now)\n- requirements are now managed by Poetry\n\n0.2.5\n~~~~~\n- added ``fetch_top_news()`` method for top crypto news separated in 2 categories\n\n0.2.4\n~~~~~\n- ``fetch_news()`` adds new "description" item and renames "image_url" to "image"\n- all ``fetch_news()`` item properties are now presented even if they are ``None``\n\n0.2.3\n~~~~~\n- simplified import from ``from karpet.karpet import Karpet`` to ``from karpet import Karpet``\n\n0.2.2\n~~~~~\n- added ``fetch_news()`` method for retrieving crypto news\n\n0.2.1\n~~~~~\n- added ``fetch_exchanges()`` method for retrieving symbol exchange list\n- removed obsolete library dependency\n\n0.2\n~~~\n- twitter scraping added\n\n0.1\n~~~\n- initial release\n\nCredits\n-------\nThis is my personal library I use in my long-term project. I can pretty much guarantee it will\nlive for a long time then. I will add new features over time and I more than welcome any\nhelp or bug reports. Feel free to open an issue or merge request.\n\nThe code is is licensed under MIT license.\n',
+    'long_description': '.. image:: https://raw.githubusercontent.com/im-n1/karpet/master/assets/logo.png\n   :align: center\n\n.. image:: https://img.shields.io/pypi/v/karpet.svg?color=0c7dbe\n   :alt: PyPI\n\n.. image:: https://img.shields.io/pypi/l/karpet.svg?color=0c7dbe\n   :alt: PyPI - License\n\n.. image:: https://img.shields.io/pypi/dm/karpet.svg?color=0c7dbe\n   :alt: PyPI - Downloads\n\n.. contents::\n\nKarpet\n======\nKarpet is a tiny library with just a few dependencies\nfor fetching coins/tokens metrics data from the internet.\n\nIt can provide following data:\n\n* coin/token historical price data (no limits)\n* google trends for the given list of keywords (longer period than official API)\n* twitter scraping for the given keywords (no limits)\n* much more info about crypto coins/tokens (no rate limits)\n\nWhat is upcoming?\n\n* Reddit metrics\n* Have a request? Open an issue ;)\n\nDependencies\n------------\nLibrary uses a few nifty dependencies and is Python 3.6+ only. There is no\nneed to install dependencies you don\'t need. Therefore this library utilizes\nextras which install optional dependencies:\n\n* for Google trends - google\n\nUsage\n-----\n1. Install the library via pip.\n\n.. code-block:: bash\n\n   pip install karpet  # Basics only\n   pip install karpet[google]  # For Google trends\n\n2. Import the library class first.\n\n.. code-block:: python\n\n    from karpet import Karpet\n\nfetch_crypto_historical_data()\n~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~\nRetrieves historical data.\n\n.. code-block:: python\n\n    k = Karpet(date(2019, 1, 1), date(2019, 5, 1))\n    df = k.fetch_crypto_historical_data(id="ethereum")  # Dataframe with historical data.\n    df.head()\n\n                     price   market_cap total_volume\n    2019-01-01  131.458725  1.36773e+10  1.36773e+10\n    2019-01-02  138.144802  1.43923e+10  1.43923e+10\n    2019-01-03  152.860453  1.59222e+10  1.59222e+10\n    2019-01-04  146.730599  1.52777e+10  1.52777e+10\n    2019-01-05  153.056567  1.59408e+10  1.59408e+10\n\n\nfetch_crypto_exchanges()\n~~~~~~~~~~~~~~~~~~~~~~~~\nRetrieves exchange list.\n\n.. code-block:: python\n\n    k = Karpet()\n    k.fetch_crypto_exchanges("nrg")\n    [\'DigiFinex\', \'KuCoin\', \'CryptoBridge\', \'Bitbns\', \'CoinExchange\']\n\nfetch_google_trends()\n~~~~~~~~~~~~~~~~~~~~~\nRetrieves Google Trends - in percents for the given date range.\n\n.. code-block:: python\n\n    k = Karpet(date(2019, 1, 1), date(2019, 5, 1))\n    df = k.fetch_google_trends(kw_list=["bitcoin"])  # Dataframe with trends.\n    df.head()\n\n.. image:: https://raw.githubusercontent.com/im-n1/karpet/master/assets/google_trends.png\n\nAnd with a few lines of code you can get a chart\n\n.. code-block:: python\n\n   df = df.set_index("date")\n   df.plot()\n\n.. image:: https://raw.githubusercontent.com/im-n1/karpet/master/assets/trends_chart.png\n\nfetch_news()\n~~~~~~~~~~~~\nRetrieves crypto news.\n\n.. code-block:: python\n\n   k = Karpet()\n   news = k.fetch_news("btc")  # Gets 10 news.\n   print(news[0])\n   {\n      \'url\': \'https://cointelegraph.com/ ....\',  # Truncated.\n      \'title\': \'Shell Invests in Blockchain-Based Energy Startup\',\n      \'description\': \'The world’s fifth top oil and gas firm, Shell, has...\',  # Truncated.\n      \'date\': datetime.datetime(2019, 7, 28, 9, 24, tzinfo=datetime.timezone(datetime.timedelta(seconds=3600)))\n      \'image\': \'https://images.cointelegraph.com/....jpg\'  # Truncated.\n   }\n   news = k.fetch_news("btc", limit=30)  # Gets 30 news.\n\nfetch_top_news()\n~~~~~~~~~~~~~~~~\nRetrieves top crypto news in 2 categories:\n\n* Editor\'s choices - articles picked by editors\n* Hot stories - articles with most views\n\n.. code-block:: python\n\n   k = Karpet()\n   editors_choices, top_stories = k.fetch_top_news()\n   print(len(editors_choices))\n   5\n   print(len(top_stories))\n   5\n   print(editors_choices[0])\n   {\n      \'url\': \'https://cointelegraph.com/...\',  # Truncated.\n      \'title\': \'Bank of China’s New Infographic Shows Why Bitcoin Price Is Going Up\',\n      \'date\': datetime.datetime(2019, 7, 27, 10, 7, tzinfo=datetime.timezone(datetime.timedelta(seconds=3600))),\n      \'image\': \'https://images.cointelegraph.com/images/740_aHR...\', # Truncated.\n      \'description\': \'The Chinese central bank released on its website an ...\'  # Truncated.\n   }\n   print(top_stories[0])\n   {\n      \'url\': \'https://cointelegraph.com/...\',  # Truncated.\n      \'title\': \'Bitcoin Price Shuns Volatility as Analysts Warn of Potential Drop to $7,000\',\n      \'date\': datetime.datetime(2019, 7, 27, 10, 7, tzinfo=datetime.timezone(datetime.timedelta(seconds=3600))),\n      \'image\': \'https://images.cointelegraph.com/images/740_aHR0c...\'  # Truncated.\n      \'description\': \'Stability around $10,600 for Bitcoin price is ...\'  # Truncated.\n   }\n\nget_coin_ids()\n~~~~~~~~~~~~~~\nResolves coin ID\'s based on the given symbol (there are coins out there with identical symbol).\n\nUse this to get distinctive coin ID which can be used as ``id`` param for\nmethod ``fetch_crypto_historical_data()``.\n\n.. code-block:: python\n\n    k = Karpet()\n    print(k.get_coin_ids("sta"))\n    [\'statera\']\n\n\nget_basic_data()\n~~~~~~~~~~~~~~~~\nFetches coin/token basic data like:\n\n``open_issues`` is only provided if ``total_issues`` and ``closed_issues`` are\navailable.\n\n.. code-block:: python\n\n    k = Karpet()\n    print(k.get_basic_data(id="ethereum"))\n    {\n        \'closed_issues\': 5530,\n        \'commit_count_4_weeks\': 40,\n        \'current_price\': 3167.67,\n        \'forks\': 11635,\n        \'market_cap\': 371964284548,\n        \'name\': \'Ethereum\',\n        \'open_issues\': 230,\n        \'pull_request_contributors\': 552,\n        \'rank\': 2,\n        \'reddit_accounts_active_48h\': 2881.0,\n        \'reddit_average_comments_48h\': 417.083,\n        \'reddit_average_posts_48h\': 417.083,\n        \'reddit_subscribers\': 1057875,\n        \'stars\': 31680,\n        \'total_issues\': 5760,\n        \'year_high\': 4182.790285752286,\n        \'year_low\': 321.0774351739628,\n        \'yoy_change\': 695.9225871929757,  # growth/drop in percents\n        \'price_change_24\': 120.1,\n        \'price_change_24_percents\': 1.23\n    }\n\nget_quick_search_data()\n~~~~~~~~~~~~~~~~~~~~~~~\nLists all coins/tokes with some basic info.\n\n.. code-block:: python\n\n    k = Karpet()\n    print(k.get_quick_search_data()[0])\n    {\n        "name": "Bitcoin",\n        "symbol": "BTC",\n        "rank": 1,\n        "slug": "bitcoin",\n        "tokens": [\n            "Bitcoin",\n            "bitcoin",\n            "BTC"\n        ],\n        "id": 1,\n    }\n\nfetch_crypto_live_data()\n~~~~~~~~~~~~~~~~~~~~~~~~\nRetrieves live market data.\n\n.. code-block:: python\n\n    k = Karpet()\n    df = k.fetch_crypto_live_data(id="ethereum")  # Dataframe with live data.\n    df.head()\n\n                            open     high      low    close\n    2023-01-16 20:00:00  1593.01  1595.05  1593.01  1594.28\n    2023-01-16 20:30:00  1593.37  1593.37  1589.03  1589.35\n    2023-01-16 21:00:00  1592.68  1593.66  1584.71  1587.87\n    2023-01-16 21:30:00  1587.28  1587.28  1583.13  1583.13\n    2023-01-16 22:00:00  1573.99  1580.11  1573.99  1579.97\n\nChangelog\n---------\n\n0.4.9\n~~~~~\n- new retry policy\n\n0.4.8\n~~~~~\n- new ``fetch_crypto_live_data()``\n\n0.4.7.\n~~~~~~\n- dependencies updated\n- news with non UTF-8 chars handled and dropped\n- fixed code formatting\n\n0.4.6\n~~~~~\n- new ``price_change_24`` and ``price_change_24_percents`` properties for ``get_basic_data()``\n- new ``get_quick_search_data()``\n\n0.4.5\n~~~~~\n- fixed dependencies\n\n0.4.4\n~~~~~\n- removed obsolete parts of the code and some dependencies\n\n0.4.3\n~~~~~\n- fixed ``get_basic_data()`` method (different data source)\n- new property in ``get_basic_data()`` return dict - ``rank``\n- tests enhanced\n\n0.4.2\n~~~~~\n- fixed minor bugs\n\n0.4.1\n~~~~~\n- new data in ``get_basic_data()`` method - ``year_low``, ``year_high``, ``yoy_change``\n\n0.4\n~~~\n- new method ``get_basic_data()``\n\n0.3.3\n~~~~~\n- removed twitter integration - twitterscraper library is not up to date\n- fixed news fetching\n\n\n0.3.2\n~~~~~\n- new method ``get_coin_ids()``\n- method ``fetch_crypto_historical_data()`` has ``id`` param now\n\n0.3.1\n~~~~~\n- migrated to coingecko.com API (no API key needed anymore)\n\n0.3\n~~~\n- migrated to cryptocompare.com API (you need an API key now)\n- requirements are now managed by Poetry\n\n0.2.5\n~~~~~\n- added ``fetch_top_news()`` method for top crypto news separated in 2 categories\n\n0.2.4\n~~~~~\n- ``fetch_news()`` adds new "description" item and renames "image_url" to "image"\n- all ``fetch_news()`` item properties are now presented even if they are ``None``\n\n0.2.3\n~~~~~\n- simplified import from ``from karpet.karpet import Karpet`` to ``from karpet import Karpet``\n\n0.2.2\n~~~~~\n- added ``fetch_news()`` method for retrieving crypto news\n\n0.2.1\n~~~~~\n- added ``fetch_exchanges()`` method for retrieving symbol exchange list\n- removed obsolete library dependency\n\n0.2\n~~~\n- twitter scraping added\n\n0.1\n~~~\n- initial release\n\nCredits\n-------\nThis is my personal library I use in my long-term project. I can pretty much guarantee it will\nlive for a long time then. I will add new features over time and I more than welcome any\nhelp or bug reports. Feel free to open an issue or merge request.\n\nThe code is is licensed under MIT license.\n',
     'author': 'n1',
     'author_email': 'hrdina.pavel@gmail.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://github.com/im-n1/karpet',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `karpet-0.4.8/PKG-INFO` & `karpet-0.4.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: karpet
-Version: 0.4.8
+Version: 0.4.9
 Summary: Library for fetching coin/token historical data, trends and more.
 Home-page: https://github.com/im-n1/karpet
 Author: n1
 Author-email: hrdina.pavel@gmail.com
 Requires-Python: >=3.8.0,<4.0.0
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -263,14 +263,18 @@
     2023-01-16 21:00:00  1592.68  1593.66  1584.71  1587.87
     2023-01-16 21:30:00  1587.28  1587.28  1583.13  1583.13
     2023-01-16 22:00:00  1573.99  1580.11  1573.99  1579.97
 
 Changelog
 ---------
 
+0.4.9
+~~~~~
+- new retry policy
+
 0.4.8
 ~~~~~
 - new ``fetch_crypto_live_data()``
 
 0.4.7.
 ~~~~~~
 - dependencies updated
```

