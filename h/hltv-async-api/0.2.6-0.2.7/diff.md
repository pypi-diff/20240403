# Comparing `tmp/hltv_async_api-0.2.6.tar.gz` & `tmp/hltv_async_api-0.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hltv_async_api-0.2.6.tar", last modified: Tue Apr  2 17:26:40 2024, max compression
+gzip compressed data, was "hltv_async_api-0.2.7.tar", last modified: Tue Apr  2 21:03:23 2024, max compression
```

## Comparing `hltv_async_api-0.2.6.tar` & `hltv_async_api-0.2.7.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-04-02 17:26:40.955364 hltv_async_api-0.2.6/
--rw-rw-rw-   0        0        0     1091 2024-04-02 00:22:12.000000 hltv_async_api-0.2.6/LICENSE
--rw-rw-rw-   0        0        0     2449 2024-04-02 17:26:40.953362 hltv_async_api-0.2.6/PKG-INFO
--rw-rw-rw-   0        0        0     1826 2024-04-02 15:07:09.000000 hltv_async_api-0.2.6/README.md
-drwxrwxrwx   0        0        0        0 2024-04-02 17:26:40.834812 hltv_async_api-0.2.6/hltv_async_api/
--rw-rw-rw-   0        0        0      124 2024-04-02 16:33:09.000000 hltv_async_api-0.2.6/hltv_async_api/__init__.py
--rw-rw-rw-   0        0        0    26016 2024-04-02 17:25:02.000000 hltv_async_api-0.2.6/hltv_async_api/aiohltv.py
-drwxrwxrwx   0        0        0        0 2024-04-02 17:26:40.951363 hltv_async_api-0.2.6/hltv_async_api.egg-info/
--rw-rw-rw-   0        0        0     2449 2024-04-02 17:26:40.000000 hltv_async_api-0.2.6/hltv_async_api.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      246 2024-04-02 17:26:40.000000 hltv_async_api-0.2.6/hltv_async_api.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-02 17:26:40.000000 hltv_async_api-0.2.6/hltv_async_api.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       15 2024-04-02 17:26:40.000000 hltv_async_api-0.2.6/hltv_async_api.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      537 2024-04-02 16:33:09.000000 hltv_async_api-0.2.6/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-02 17:26:40.955364 hltv_async_api-0.2.6/setup.cfg
--rw-rw-rw-   0        0        0      922 2024-04-02 16:33:09.000000 hltv_async_api-0.2.6/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-02 21:03:23.127077 hltv_async_api-0.2.7/
+-rw-rw-rw-   0        0        0     1091 2024-04-02 00:22:12.000000 hltv_async_api-0.2.7/LICENSE
+-rw-rw-rw-   0        0        0     4887 2024-04-02 21:03:23.125095 hltv_async_api-0.2.7/PKG-INFO
+-rw-rw-rw-   0        0        0     4264 2024-04-02 21:01:52.000000 hltv_async_api-0.2.7/README.md
+drwxrwxrwx   0        0        0        0 2024-04-02 21:03:23.080078 hltv_async_api-0.2.7/hltv_async_api/
+-rw-rw-rw-   0        0        0      124 2024-04-02 16:33:09.000000 hltv_async_api-0.2.7/hltv_async_api/__init__.py
+-rw-rw-rw-   0        0        0    28348 2024-04-02 21:00:56.000000 hltv_async_api-0.2.7/hltv_async_api/aiohltv.py
+drwxrwxrwx   0        0        0        0 2024-04-02 21:03:23.124075 hltv_async_api-0.2.7/hltv_async_api.egg-info/
+-rw-rw-rw-   0        0        0     4887 2024-04-02 21:03:22.000000 hltv_async_api-0.2.7/hltv_async_api.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      246 2024-04-02 21:03:22.000000 hltv_async_api-0.2.7/hltv_async_api.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-02 21:03:22.000000 hltv_async_api-0.2.7/hltv_async_api.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       15 2024-04-02 21:03:22.000000 hltv_async_api-0.2.7/hltv_async_api.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      537 2024-04-02 21:03:16.000000 hltv_async_api-0.2.7/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-02 21:03:23.128086 hltv_async_api-0.2.7/setup.cfg
+-rw-rw-rw-   0        0        0      922 2024-04-02 21:03:16.000000 hltv_async_api-0.2.7/setup.py
```

### Comparing `hltv_async_api-0.2.6/LICENSE` & `hltv_async_api-0.2.7/LICENSE`

 * *Files identical despite different names*

### Comparing `hltv_async_api-0.2.6/hltv_async_api/aiohltv.py` & `hltv_async_api-0.2.7/hltv_async_api/aiohltv.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from typing import Any, List
 from datetime import date, datetime, timedelta
+import pytz
 
 from bs4 import BeautifulSoup
 import asyncio
 from asyncio import get_running_loop
 from functools import partial
 
 from aiohttp import ClientSession, ClientTimeout
@@ -217,15 +218,15 @@
         """returns a list of all upcoming matches on HLTV"""
         r = await self.fetch("https://www.hltv.org/matches")
         if not r:return
 
         matches = []
         try:
 
-            days = 7
+
             for i, date_div in enumerate(r.find_all('div', {'class': 'upcomingMatchesSection'}), start=1):
                 if i > days:
                     break
                 date_ = date_div.find('span', {'class': 'matchDayHeadline'}).text.split()[-1]
                 matches_today = []
 
                 for match in date_div.find_all('div', {'class': 'upcomingMatch'}):
@@ -574,15 +575,15 @@
             total_trophys = None
             try:
                 last_trophy = r.find('div', {'class': 'trophyHolder'}).find('span')['title']
                 total_trophys = len(r.find_all('div', {'class': 'trophyHolder'}))
             except AttributeError:
                 pass
 
-            return (team_id, title, rank, players, coach, age, weeks, last_trophy, total_trophys)
+            return team_id, title, rank, players, coach, age, weeks, last_trophy, total_trophys
         except AttributeError:
             raise AttributeError("Parsing error, probably page not fully loaded")
 
     async def get_best_players(self, top=40):
         """
         returns a list of the top (1-40) players in top 20 at the year
         :params:
@@ -624,23 +625,74 @@
                     'maps': maps,
                     'rating': rating,
                 })
                 rank += 1
                 if rank > top:
                     break
         except AttributeError:
-            raise AttributeError("Parsing error, probably page not fully loaded")
+            raise AttributeError("Top players parsing error, probably page not fully loaded")
 
         return players
 
     # TODO WRITE
-    async def get_last_news(self):
-        return []
+    async def get_last_news(self, max_reg_news=2, only_today=True, only_featured=False):
+        r = await self.fetch('https://www.hltv.org/')
+
+        today = datetime.now(tz=pytz.timezone('Europe/Copenhagen'))
+        article_days = {
+            1: today.strftime('%d-%m'),
+            2: (today - timedelta(days=1)).strftime('%d-%m'),
+            3: 'old'
+        }
+
+        news = []
+        reg_news_num = 0
+        for i, news_date_div in enumerate(r.find_all('div', {'class', 'standard-box standard-list'}), start=1):
+            date_ = article_days[i]
+            f_news = []
+            reg_news = []
+            for featured_news_div in news_date_div.find_all('a', {'class': 'newsline article featured breaking-featured'}):
+                featured_id = featured_news_div['href'].split('/')[2]
+                featured_title = featured_news_div.find('div', {'class': 'featured-newstext'}).text
+                featured_description = featured_news_div.find('div', {'class': 'featured-small-newstext'}).text
+                f_news.append({
+                    'f_id': featured_id,
+                    'f_title': featured_title,
+                    'f_desc': featured_description,
+                })
+
+            if not only_featured and reg_news_num < max_reg_news:
+                for news_div in news_date_div.find_all('a',
+                                                           {'class': 'newsline article'}):
+                    if reg_news_num > max_reg_news:
+                        break
+                    if news_div['class'] != 'newsline article featured breaking-featured':
+                        news_id = news_div['href'].split('/')[2]
+                        news_title = news_div.find('div', {'class': 'newstext'}).text
+                        news_posted = news_div.find('div', {'class': 'newsrecent'}).text
+
+                        reg_news.append({
+                            'id': news_id,
+                            'title': news_title,
+                            'posted': news_posted,
+                        })
+                        reg_news_num += 1
+
+            news.append({
+                'date': date_,
+                'f_news': f_news,
+                'news': reg_news,
+            })
+
+            if only_today:
+                break
+
+        return news
 
 
 async def test():
     hltv = Hltv()
-    print(await hltv.get_upcoming_matches())
+    print(await hltv.get_last_news(only_today=True, max_reg_news=1))
 
 
 if __name__ == "__main__":
     asyncio.run(test())
```

### Comparing `hltv_async_api-0.2.6/pyproject.toml` & `hltv_async_api-0.2.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "hltv_async_api"
-version = "0.2.6"
+version = "0.2.7"
 authors = [
   { name="Akim Slys", email="akimslys2003@gmail.com" },
 ]
 description = "Hltv-aio An unofficial asynchronous HLTV API Wrapper for Python"
 readme = "README.md"
 requires-python = ">=3.9"
 classifiers = [
```

### Comparing `hltv_async_api-0.2.6/setup.py` & `hltv_async_api-0.2.7/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='hltv_async_api',
-    version='0.2.6',
+    version='0.2.7',
     author='akimerslys',
     author_email='akimslys2003@gmail.com',
     description='Hltv-aio: An unofficial asynchronous HLTV API Wrapper for Python',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/akimerslys/aiohltv',
     packages=find_packages(),
```

