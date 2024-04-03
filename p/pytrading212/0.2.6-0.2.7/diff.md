# Comparing `tmp/pytrading212-0.2.6.tar.gz` & `tmp/pytrading212-0.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytrading212-0.2.6.tar", last modified: Wed Nov 15 21:27:31 2023, max compression
+gzip compressed data, was "pytrading212-0.2.7.tar", max compression
```

## Comparing `pytrading212-0.2.6.tar` & `pytrading212-0.2.7.tar`

### file list

```diff
@@ -1,24 +1,12 @@
-drwxrwxrwx   0        0        0        0 2023-11-15 21:27:31.091785 pytrading212-0.2.6/
--rw-rw-rw-   0        0        0     1087 2023-11-15 20:45:10.000000 pytrading212-0.2.6/LICENSE
--rw-rw-rw-   0        0        0    12623 2023-11-15 21:27:31.085041 pytrading212-0.2.6/PKG-INFO
--rw-rw-rw-   0        0        0    12224 2023-11-15 21:19:09.000000 pytrading212-0.2.6/README.md
--rw-rw-rw-   0        0        0      429 2023-11-15 21:27:28.000000 pytrading212-0.2.6/pyproject.toml
-drwxrwxrwx   0        0        0        0 2023-11-15 21:27:31.032413 pytrading212-0.2.6/pytrading212/
--rw-rw-rw-   0        0        0      339 2023-11-15 20:45:10.000000 pytrading212-0.2.6/pytrading212/__init__.py
--rw-rw-rw-   0        0        0      226 2023-11-15 20:45:10.000000 pytrading212-0.2.6/pytrading212/console.py
--rw-rw-rw-   0        0        0     1016 2023-11-15 20:45:10.000000 pytrading212-0.2.6/pytrading212/constants.py
--rw-rw-rw-   0        0        0      419 2023-11-15 20:45:10.000000 pytrading212-0.2.6/pytrading212/instrument.py
--rw-rw-rw-   0        0        0     5663 2023-11-15 20:45:10.000000 pytrading212-0.2.6/pytrading212/order.py
--rw-rw-rw-   0        0        0      242 2023-11-15 20:45:10.000000 pytrading212-0.2.6/pytrading212/position.py
--rw-rw-rw-   0        0        0    15091 2023-11-15 21:14:42.000000 pytrading212-0.2.6/pytrading212/trading212.py
--rw-rw-rw-   0        0        0      540 2023-11-15 20:45:10.000000 pytrading212-0.2.6/pytrading212/utils.py
-drwxrwxrwx   0        0        0        0 2023-11-15 21:27:31.060681 pytrading212-0.2.6/pytrading212.egg-info/
--rw-rw-rw-   0        0        0    12623 2023-11-15 21:27:30.000000 pytrading212-0.2.6/pytrading212.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      421 2023-11-15 21:27:30.000000 pytrading212-0.2.6/pytrading212.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-11-15 21:27:30.000000 pytrading212-0.2.6/pytrading212.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       19 2023-11-15 21:27:30.000000 pytrading212-0.2.6/pytrading212.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-11-15 21:27:31.092909 pytrading212-0.2.6/setup.cfg
--rw-rw-rw-   0        0        0      711 2023-11-15 21:20:15.000000 pytrading212-0.2.6/setup.py
-drwxrwxrwx   0        0        0        0 2023-11-15 21:27:31.075338 pytrading212-0.2.6/tests/
--rw-rw-rw-   0        0        0        0 2023-11-15 20:45:10.000000 pytrading212-0.2.6/tests/__init__.py
--rw-rw-rw-   0        0        0     2417 2023-11-15 20:45:10.000000 pytrading212-0.2.6/tests/test_order.py
+-rw-r--r--   0        0        0     1066 2024-04-03 11:11:26.032599 pytrading212-0.2.7/LICENSE
+-rw-r--r--   0        0        0    11829 2024-04-03 11:11:26.032599 pytrading212-0.2.7/README.md
+-rw-r--r--   0        0        0      410 2024-04-03 11:11:26.036599 pytrading212-0.2.7/pyproject.toml
+-rw-r--r--   0        0        0      377 2024-04-03 11:11:26.036599 pytrading212-0.2.7/pytrading212/__init__.py
+-rw-r--r--   0        0        0      214 2024-04-03 11:11:26.036599 pytrading212-0.2.7/pytrading212/console.py
+-rw-r--r--   0        0        0     5691 2024-04-03 11:11:26.036599 pytrading212-0.2.7/pytrading212/constants.py
+-rw-r--r--   0        0        0     2473 2024-04-03 11:11:26.036599 pytrading212-0.2.7/pytrading212/instrument.py
+-rw-r--r--   0        0        0     5487 2024-04-03 11:11:26.036599 pytrading212-0.2.7/pytrading212/order.py
+-rw-r--r--   0        0        0      236 2024-04-03 11:11:26.036599 pytrading212-0.2.7/pytrading212/position.py
+-rw-r--r--   0        0        0    14171 2024-04-03 11:11:26.036599 pytrading212-0.2.7/pytrading212/trading212.py
+-rw-r--r--   0        0        0      520 2024-04-03 11:11:26.036599 pytrading212-0.2.7/pytrading212/utils.py
+-rw-r--r--   0        0        0    12635 1970-01-01 00:00:00.000000 pytrading212-0.2.7/PKG-INFO
```

### Comparing `pytrading212-0.2.6/PKG-INFO` & `pytrading212-0.2.7/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,408 +1,395 @@
-Metadata-Version: 2.1
-Name: pytrading212
-Version: 0.2.6
-Summary: Unofficial Trading212 API
-Home-page: https://github.com/HellAmbro/Trading212API
-Author: HellAmbro
-Author-email: frambrosini1998@gmail.com
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.9
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-<div align="center">
-
-# PyTrading212 API
-
-## Unofficial API for Trading212
-### Unofficial API for Trading212 broker.
-
-
-
-### [Documentation](https://hellambro.github.io/Trading212API/)
-
-### Support the Project
-
-#### With a :star:
-
-[![Star History Chart](https://api.star-history.com/svg?repos=HellAmbro/Trading212API&type=Date)](https://star-history.com/#HellAmbro/Trading212API&Date)
-
-#### With a donation
-
-<a href="https://www.buymeacoffee.com/hellambro" target="_blank"><img src="https://cdn.buymeacoffee.com/buttons/v2/default-blue.png" alt="Buy Me A Coffee" height="50" ></a>
-
-**LTC** LbAzhtHBvQ2JCGhrcefUuvwNrv9VrQJoyJ
-
-**BTC** 1JWhMC3tiSjyR6t7BJuM7YRDg3xvPM2MDk
-
-**ETH** 0x51f1f0061eadc024ab4bd1f3658d249044160006
-
-</div>
-
-<div align="left">
-
-### Discord Channel for support
-[Discord](https://discord.gg/PmWemEUA)
-
-  ## Installation
-
-```bash
-pip install pytrading212
-```
-
-### Warning :warning:
-
-When you are using the API you cannot access Trading212 from other devices and browsers, except for the webdriver.New
-access from another browser may disconnect the current session, invalidating the _cookie_ and making the API not work.
-
-## PyTrading212 Usage
-
-For a full reference please look inside **examples** folder
-
-### Equity Example
-
-```python
-from selenium import webdriver
-from selenium.webdriver.chrome.service import Service
-
-from pytrading212 import Equity
-from pytrading212 import Mode, EquityOrder, OrderType
-
-driver = webdriver.Chrome(service=Service())
-equity = Equity(email='your_email', password='your_password', driver=driver, mode=Mode.DEMO)
-
-# Invalid order: voluntary typo-error in instrument code
-order = EquityOrder(instrument_code="AAAAPL_US_EQ", order_type=OrderType.MARKET, quantity=2)
-is_valid, reason = equity.check_order(order)
-if is_valid:
-    print("Your order is valid, can be executed.")
-else:
-    print("Your order is not valid. The reason is: ", reason)
-# Valid order
-order = EquityOrder(instrument_code="AAPL_US_EQ", order_type=OrderType.MARKET, quantity=2)
-
-# Check order validity (recommended)
-if equity.check_order(order)[0]:
-    # Review order (recommended)
-    print(equity.review_order(order))
-    # Execute order
-    print(equity.execute_order(order))
-
-equity.finish()
-```
-
-### CFD Example
-
-```python
-from selenium import webdriver
-from selenium.webdriver.chrome.service import Service
-
-from pytrading212 import CFD, CFDOrder
-from pytrading212 import Mode
-
-driver = webdriver.Chrome(service=Service())
-cfd = CFD(email='your_email', password='your_password', driver=driver, mode=Mode.DEMO)
-
-instrument_code = "AAPL"
-
-cfd_order = CFDOrder(instrument_code=instrument_code,
-                     quantity=-0.1,  # Sell (quantity is negative)
-                     target_price=cfd.get_current_price(instrument_code=instrument_code)
-                     )
-
-print(cfd.execute_order(order=cfd_order))
-```
-
-### PyTrading212 initialization
-
-:warning: As now March 2023 only one instance at time is supported. :warning:
-
-:x: This means that you cannot initialize both **Equity** and **CFD** :x:
-
-PyTrading212 **Equity** instance
-
-```python
-driver = webdriver.Chrome(service=Service())
-equity = Equity(email='your_email', password='your_password', driver=driver, mode=Mode.DEMO)
-```
-
-PyTrading212 **CFD** instance
-
-```python
-driver = webdriver.Chrome(service=Service())
-cfd = CFD(email='your_email', password='your_password', driver=driver, mode=Mode.DEMO)
-```
-
-### PyTrading212 close session
-
-Close the session, also the webdriver is closed.
-
-```python
-equity.finish()
-```
-
-or
-
-```python
-cfd.finish()
-```
-
-### Getting Instrument Code
-
-```python
-print(equity.get_companies())
-```
-
-or
-
-```python
-print(cfd.get_companies())
-```
-
-Returns a JSON with all Instrument code that you can trade, both CFD and Equity.
-
-**Note**: Instrument code is different for _CFD_ and _Equity_ even for the same Stock.
-For example **Apple** Instrument Code is:
-
-```
-CFD: AAPL
-EQUITY: AAPL_US_EQ
-```
-
-### Order Structure
-
-![order](docs/imgs/order_structure.png)
-
-### [Equity Order](https://hellambro.github.io/Trading212API/order.html#pytrading212.order.EquityOrder)
-
-It's possible to create **equity orders** directly from `EquityOrder` class
-
-```python
-# Buy
-order = EquityOrder(instrument_code="AAPL_US_EQ", order_type=OrderType.MARKET, quantity=1)
-equity.execute_order(order=order)
-```
-
-or
-
-```python
-# Buy
-market_order = MarketOrder(instrument_code="AAPL_US_EQ", quantity=1)
-equity.execute_order(order=market_order)
-```
-
-These two orders are equivalent, you can use both ways indifferently.
-
-For selling stocks (**that you own**, for short-selling see CFD section below) you just need to change the sign of
-_quantity_ or _value_ property
-
-```python
-# Sell
-order = EquityOrder(instrument_code="AAPL_US_EQ", order_type=OrderType.MARKET, quantity=-1)
-equity.execute_order(order=order)
-```
-
-or
-
-```python
-# Sell
-market_order = MarketOrder(instrument_code="AAPL_US_EQ", quantity=-1)
-equity.execute_order(order=market_order)
-```
-
-All other **equity order classes** are wrappers of the `EquityOrder`
-
-#### Wrappers for Equity Orders
-
-- MarketOrder
-
-```python
-market_order = MarketOrder(instrument_code="AAPL_US_EQ", quantity=1)
-```
-
-- LimitOrder
-
-```python
-limit_order = LimitOrder(instrument_code="AAPL_US_EQ",
-                         quantity=2,
-                         limit_price=150.0,
-                         time_validity=constants.TimeValidity.DAY)
-```
-
-- StopOrder
-
-```python
-stop_order = StopOrder(instrument_code="AAPL_US_EQ",
-                       quantity=-3,  # Sell
-                       stop_price=180.0,
-                       time_validity=constants.TimeValidity.GOOD_TILL_CANCEL)
-```
-
-- StopLimitOrder
-
-```python
-stop_limit_order = StopLimitOrder(instrument_code="AAPL_US_EQ",
-                                  quantity=1,
-                                  limit_price=150,
-                                  stop_price=180,
-                                  time_validity=constants.TimeValidity.DAY)
-```
-
-- ValueOrder
-
-```python
-value_order = ValueOrder(instrument_code="AAPL_US_EQ", value=2500.0)
-```
-
-These classes allow to simplify the creation of orders, avoiding errors for omitted parameters,
-improving code readability.
-
-### [CFD Order](https://hellambro.github.io/Trading212API/order.html#pytrading212.order.CFDOrder)
-
-You can use 3 types of CFD Orders: `Market`, `Limit/Stop`, `OCO` (Order Cancel Order)
-
-#### Market Order
-
-- Market Order without Take Profit and Stop Loss
-
-```python
-instrument_code = "AAPL"
-cfd_order = CFDMarketOrder(instrument_code=instrument_code,
-                           quantity=0.1,  # Buy (quantity is positive)
-                           target_price=cfd.get_current_price(instrument_code=instrument_code))
-```
-
-- MarketOrder with Take Profit (_limit_distance_)
-
-```python
-instrument_code = "AAPL"
-current_price = cfd.get_current_price(instrument_code=instrument_code)
-cfd_order = CFDMarketOrder(instrument_code=instrument_code,
-                           quantity=0.5,
-                           target_price=current_price,
-                           limit_distance=5.0)
-```
-
-- MarketOrder with Stop Loss (_stop_distance_)
-
-```python
-instrument_code = "AAPL"
-current_price = cfd.get_current_price(instrument_code=instrument_code)
-cfd_order = CFDMarketOrder(instrument_code=instrument_code,
-                           quantity=0.5,
-                           target_price=current_price,
-                           stop_distance=2.0)
-```
-
-- MarketOrder with Stop Loss and Take Profit
-
-```python
-instrument_code = "AAPL"
-current_price = cfd.get_current_price(instrument_code=instrument_code)
-cfd_order = CFDMarketOrder(instrument_code=instrument_code,
-                           quantity=0.5,
-                           target_price=current_price,
-                           limit_distance=4.0,
-                           stop_distance=2.0,
-                           )
-```
-
-- CFD Stop Limit Order
-
-#### Note about stop and limit distance
-
-`stop_distance` and `limit_distance` are the _distance_ between the **current price** and SL/TP price.
-You should add/subtract these quantities to the current price in order to get TP/SL price.
-
-```                                                   
-current_price = 150.0
-limit_distance = 10.0   -> TP price = 150.0 + 10.0 = 160.0
-stop_distance = 5.0     -> SL price = 150.0 - 5.0 =  145.0
-```
-
-#### Limit/Stop Order (Pending Order with specified price)
-
-- Limit/Stop Order with Take Profit and Stop Loss
-
-```python
-instrument_code = "AAPL"
-# Target price of Apple Stock, the current price - 20.0$ 
-target_price = cfd.get_current_price(instrument_code=instrument_code) - 20.0
-# Put a pending Buy Order when the price triggers target_price
-cfd_order = CFDLimitStopOrder(instrument_code=instrument_code,
-                              target_price=target_price,
-                              quantity=1,
-                              take_profit=target_price + 10,
-                              # TP when Apple's stock price is  10.0$ above the target_price
-                              stop_loss=target_price - 5)  # TP when Apple's stock price is  5.0$ below the target_price
-```
-
-- Limit/Stop Order without Take Profit
-
-```python
-instrument_code = "AAPL"
-target_price = cfd.get_current_price(instrument_code=instrument_code) - 10.0
-cfd_order = CFDLimitStopOrder(instrument_code=instrument_code,
-                              target_price=target_price,
-                              quantity=1,
-                              stop_loss=target_price - 3.0)
-```
-
-- Limit/Stop Order without Stop Loss
-
-```python
-instrument_code = "AAPL"
-target_price = cfd.get_current_price(instrument_code=instrument_code) - 30.0
-cfd_order = CFDLimitStopOrder(instrument_code=instrument_code,
-                              target_price=target_price,
-                              quantity=1,
-                              take_profit=target_price + 20)
-```
-
-- Limit/Stop Order without Take Profit and Stop Loss
-
-```python
-instrument_code = "AAPL"
-target_price = cfd.get_current_price(instrument_code=instrument_code) + 30.0
-cfd_order = CFDLimitStopOrder(instrument_code=instrument_code,
-                              target_price=target_price,
-                              quantity=-1) # Sell 
-```
-
-**Note about stop_loss and take_profit**
-
-`stop_loss` and `take_profit` indicates the price of the stock when we want to make the TP or SL trades.
-
-#### OCO Order (Order Cancel Order)
-
-**Buy** 1 Apple's Stock when the price drops below 150.0$ (now ~162.0$): execute `order1`, cancel `order2`
-
-or
-
-**Sell** 1 Apple's Stock when the price rise above 180.0$ (now ~162.0$): execute `order2`, cancel `order1`
-```python
-instrument_code = "AAPL"
-cfd_oco_order = CFDOCOOrder(instrument_code=instrument_code,
-                            order1=CFDOCOOrder.OCOSubOrder(price=150, quantity=1),
-                            order2=CFDOCOOrder.OCOSubOrder(price=180.0, quantity=-1))
-```
-
-### Useful resources
-
-- [Use Trading212 for Automatic Trading: an introduction to pytrading212 (Depreacted since v0.2.5)](https://medium.com/@francescoelambroambrosini/use-trading212-for-automatic-trading-an-introduction-to-pytrading212-367449b40a6)
-- [Driver requirements](https://www.selenium.dev/documentation/en/webdriver/driver_requirements)
-- [Getting started with WebDriver](https://www.selenium.dev/documentation/en/getting_started_with_webdriver/)
-
-### Disclaimer
-
-Nor me or Trading212 are responsible for the use of this API, first make sure that everything works well through the use
-of a **DEMO** account, then switch to **REAL** mode.
-
-In addition, I don't take responsibility for the accuracy of the information reported here and the proper functioning of
-the API
-
-All trademarks, logos and brand names are the property of their respective owners. All company, product and service
-names used in this website are for identification purposes only.
-
-</div>
+<div align="center">
+
+# PyTrading212 API
+
+## Unofficial API for Trading212
+### Unofficial API for Trading212 broker.
+
+
+
+### [Documentation](https://hellambro.github.io/Trading212API/)
+
+### Support the Project
+
+#### With a :star:
+
+[![Star History Chart](https://api.star-history.com/svg?repos=HellAmbro/Trading212API&type=Date)](https://star-history.com/#HellAmbro/Trading212API&Date)
+
+#### With a donation
+
+<a href="https://www.buymeacoffee.com/hellambro" target="_blank"><img src="https://cdn.buymeacoffee.com/buttons/v2/default-blue.png" alt="Buy Me A Coffee" height="50" ></a>
+
+**LTC** LbAzhtHBvQ2JCGhrcefUuvwNrv9VrQJoyJ
+
+**BTC** 1JWhMC3tiSjyR6t7BJuM7YRDg3xvPM2MDk
+
+**ETH** 0x51f1f0061eadc024ab4bd1f3658d249044160006
+
+</div>
+
+<div align="left">
+
+### Discord Channel for support
+[Discord](https://discord.gg/PmWemEUA)
+
+  ## Installation
+
+```bash
+pip install pytrading212
+```
+
+### Warning :warning:
+
+When you are using the API you cannot access Trading212 from other devices and browsers, except for the webdriver.New
+access from another browser may disconnect the current session, invalidating the _cookie_ and making the API not work.
+
+## PyTrading212 Usage
+
+For a full reference please look inside **examples** folder
+
+### Equity Example
+
+```python
+from selenium import webdriver
+from selenium.webdriver.chrome.service import Service
+
+from pytrading212 import Equity
+from pytrading212 import Mode, EquityOrder, OrderType
+
+driver = webdriver.Chrome(service=Service())
+equity = Equity(email='your_email', password='your_password', driver=driver, mode=Mode.DEMO)
+
+# Invalid order: voluntary typo-error in instrument code
+order = EquityOrder(instrument_code="AAAAPL_US_EQ", order_type=OrderType.MARKET, quantity=2)
+is_valid, reason = equity.check_order(order)
+if is_valid:
+    print("Your order is valid, can be executed.")
+else:
+    print("Your order is not valid. The reason is: ", reason)
+# Valid order
+order = EquityOrder(instrument_code="AAPL_US_EQ", order_type=OrderType.MARKET, quantity=2)
+
+# Check order validity (recommended)
+if equity.check_order(order)[0]:
+    # Review order (recommended)
+    print(equity.review_order(order))
+    # Execute order
+    print(equity.execute_order(order))
+
+equity.finish()
+```
+
+### CFD Example
+
+```python
+from selenium import webdriver
+from selenium.webdriver.chrome.service import Service
+
+from pytrading212 import CFD, CFDOrder
+from pytrading212 import Mode
+
+driver = webdriver.Chrome(service=Service())
+cfd = CFD(email='your_email', password='your_password', driver=driver, mode=Mode.DEMO)
+
+instrument_code = "AAPL"
+
+cfd_order = CFDOrder(instrument_code=instrument_code,
+                     quantity=-0.1,  # Sell (quantity is negative)
+                     target_price=cfd.get_current_price(instrument_code=instrument_code)
+                     )
+
+print(cfd.execute_order(order=cfd_order))
+```
+
+### PyTrading212 initialization
+
+:warning: As now March 2023 only one instance at time is supported. :warning:
+
+:x: This means that you cannot initialize both **Equity** and **CFD** :x:
+
+PyTrading212 **Equity** instance
+
+```python
+driver = webdriver.Chrome(service=Service())
+equity = Equity(email='your_email', password='your_password', driver=driver, mode=Mode.DEMO)
+```
+
+PyTrading212 **CFD** instance
+
+```python
+driver = webdriver.Chrome(service=Service())
+cfd = CFD(email='your_email', password='your_password', driver=driver, mode=Mode.DEMO)
+```
+
+### PyTrading212 close session
+
+Close the session, also the webdriver is closed.
+
+```python
+equity.finish()
+```
+
+or
+
+```python
+cfd.finish()
+```
+
+### Getting Instrument Code
+
+```python
+print(equity.get_companies())
+```
+
+or
+
+```python
+print(cfd.get_companies())
+```
+
+Returns a JSON with all Instrument code that you can trade, both CFD and Equity.
+
+**Note**: Instrument code is different for _CFD_ and _Equity_ even for the same Stock.
+For example **Apple** Instrument Code is:
+
+```
+CFD: AAPL
+EQUITY: AAPL_US_EQ
+```
+
+### Order Structure
+
+![order](docs/imgs/order_structure.png)
+
+### [Equity Order](https://hellambro.github.io/Trading212API/order.html#pytrading212.order.EquityOrder)
+
+It's possible to create **equity orders** directly from `EquityOrder` class
+
+```python
+# Buy
+order = EquityOrder(instrument_code="AAPL_US_EQ", order_type=OrderType.MARKET, quantity=1)
+equity.execute_order(order=order)
+```
+
+or
+
+```python
+# Buy
+market_order = MarketOrder(instrument_code="AAPL_US_EQ", quantity=1)
+equity.execute_order(order=market_order)
+```
+
+These two orders are equivalent, you can use both ways indifferently.
+
+For selling stocks (**that you own**, for short-selling see CFD section below) you just need to change the sign of
+_quantity_ or _value_ property
+
+```python
+# Sell
+order = EquityOrder(instrument_code="AAPL_US_EQ", order_type=OrderType.MARKET, quantity=-1)
+equity.execute_order(order=order)
+```
+
+or
+
+```python
+# Sell
+market_order = MarketOrder(instrument_code="AAPL_US_EQ", quantity=-1)
+equity.execute_order(order=market_order)
+```
+
+All other **equity order classes** are wrappers of the `EquityOrder`
+
+#### Wrappers for Equity Orders
+
+- MarketOrder
+
+```python
+market_order = MarketOrder(instrument_code="AAPL_US_EQ", quantity=1)
+```
+
+- LimitOrder
+
+```python
+limit_order = LimitOrder(instrument_code="AAPL_US_EQ",
+                         quantity=2,
+                         limit_price=150.0,
+                         time_validity=constants.TimeValidity.DAY)
+```
+
+- StopOrder
+
+```python
+stop_order = StopOrder(instrument_code="AAPL_US_EQ",
+                       quantity=-3,  # Sell
+                       stop_price=180.0,
+                       time_validity=constants.TimeValidity.GOOD_TILL_CANCEL)
+```
+
+- StopLimitOrder
+
+```python
+stop_limit_order = StopLimitOrder(instrument_code="AAPL_US_EQ",
+                                  quantity=1,
+                                  limit_price=150,
+                                  stop_price=180,
+                                  time_validity=constants.TimeValidity.DAY)
+```
+
+- ValueOrder
+
+```python
+value_order = ValueOrder(instrument_code="AAPL_US_EQ", value=2500.0)
+```
+
+These classes allow to simplify the creation of orders, avoiding errors for omitted parameters,
+improving code readability.
+
+### [CFD Order](https://hellambro.github.io/Trading212API/order.html#pytrading212.order.CFDOrder)
+
+You can use 3 types of CFD Orders: `Market`, `Limit/Stop`, `OCO` (Order Cancel Order)
+
+#### Market Order
+
+- Market Order without Take Profit and Stop Loss
+
+```python
+instrument_code = "AAPL"
+cfd_order = CFDMarketOrder(instrument_code=instrument_code,
+                           quantity=0.1,  # Buy (quantity is positive)
+                           target_price=cfd.get_current_price(instrument_code=instrument_code))
+```
+
+- MarketOrder with Take Profit (_limit_distance_)
+
+```python
+instrument_code = "AAPL"
+current_price = cfd.get_current_price(instrument_code=instrument_code)
+cfd_order = CFDMarketOrder(instrument_code=instrument_code,
+                           quantity=0.5,
+                           target_price=current_price,
+                           limit_distance=5.0)
+```
+
+- MarketOrder with Stop Loss (_stop_distance_)
+
+```python
+instrument_code = "AAPL"
+current_price = cfd.get_current_price(instrument_code=instrument_code)
+cfd_order = CFDMarketOrder(instrument_code=instrument_code,
+                           quantity=0.5,
+                           target_price=current_price,
+                           stop_distance=2.0)
+```
+
+- MarketOrder with Stop Loss and Take Profit
+
+```python
+instrument_code = "AAPL"
+current_price = cfd.get_current_price(instrument_code=instrument_code)
+cfd_order = CFDMarketOrder(instrument_code=instrument_code,
+                           quantity=0.5,
+                           target_price=current_price,
+                           limit_distance=4.0,
+                           stop_distance=2.0,
+                           )
+```
+
+- CFD Stop Limit Order
+
+#### Note about stop and limit distance
+
+`stop_distance` and `limit_distance` are the _distance_ between the **current price** and SL/TP price.
+You should add/subtract these quantities to the current price in order to get TP/SL price.
+
+```                                                   
+current_price = 150.0
+limit_distance = 10.0   -> TP price = 150.0 + 10.0 = 160.0
+stop_distance = 5.0     -> SL price = 150.0 - 5.0 =  145.0
+```
+
+#### Limit/Stop Order (Pending Order with specified price)
+
+- Limit/Stop Order with Take Profit and Stop Loss
+
+```python
+instrument_code = "AAPL"
+# Target price of Apple Stock, the current price - 20.0$ 
+target_price = cfd.get_current_price(instrument_code=instrument_code) - 20.0
+# Put a pending Buy Order when the price triggers target_price
+cfd_order = CFDLimitStopOrder(instrument_code=instrument_code,
+                              target_price=target_price,
+                              quantity=1,
+                              take_profit=target_price + 10,
+                              # TP when Apple's stock price is  10.0$ above the target_price
+                              stop_loss=target_price - 5)  # TP when Apple's stock price is  5.0$ below the target_price
+```
+
+- Limit/Stop Order without Take Profit
+
+```python
+instrument_code = "AAPL"
+target_price = cfd.get_current_price(instrument_code=instrument_code) - 10.0
+cfd_order = CFDLimitStopOrder(instrument_code=instrument_code,
+                              target_price=target_price,
+                              quantity=1,
+                              stop_loss=target_price - 3.0)
+```
+
+- Limit/Stop Order without Stop Loss
+
+```python
+instrument_code = "AAPL"
+target_price = cfd.get_current_price(instrument_code=instrument_code) - 30.0
+cfd_order = CFDLimitStopOrder(instrument_code=instrument_code,
+                              target_price=target_price,
+                              quantity=1,
+                              take_profit=target_price + 20)
+```
+
+- Limit/Stop Order without Take Profit and Stop Loss
+
+```python
+instrument_code = "AAPL"
+target_price = cfd.get_current_price(instrument_code=instrument_code) + 30.0
+cfd_order = CFDLimitStopOrder(instrument_code=instrument_code,
+                              target_price=target_price,
+                              quantity=-1) # Sell 
+```
+
+**Note about stop_loss and take_profit**
+
+`stop_loss` and `take_profit` indicates the price of the stock when we want to make the TP or SL trades.
+
+#### OCO Order (Order Cancel Order)
+
+**Buy** 1 Apple's Stock when the price drops below 150.0$ (now ~162.0$): execute `order1`, cancel `order2`
+
+or
+
+**Sell** 1 Apple's Stock when the price rise above 180.0$ (now ~162.0$): execute `order2`, cancel `order1`
+```python
+instrument_code = "AAPL"
+cfd_oco_order = CFDOCOOrder(instrument_code=instrument_code,
+                            order1=CFDOCOOrder.OCOSubOrder(price=150, quantity=1),
+                            order2=CFDOCOOrder.OCOSubOrder(price=180.0, quantity=-1))
+```
+
+### Useful resources
+
+- [Use Trading212 for Automatic Trading: an introduction to pytrading212 (Depreacted since v0.2.5)](https://medium.com/@francescoelambroambrosini/use-trading212-for-automatic-trading-an-introduction-to-pytrading212-367449b40a6)
+- [Driver requirements](https://www.selenium.dev/documentation/en/webdriver/driver_requirements)
+- [Getting started with WebDriver](https://www.selenium.dev/documentation/en/getting_started_with_webdriver/)
+
+### Disclaimer
+
+Nor me or Trading212 are responsible for the use of this API, first make sure that everything works well through the use
+of a **DEMO** account, then switch to **REAL** mode.
+
+In addition, I don't take responsibility for the accuracy of the information reported here and the proper functioning of
+the API
+
+All trademarks, logos and brand names are the property of their respective owners. All company, product and service
+names used in this website are for identification purposes only.
+
+</div>
```

#### html2text {}

```diff
@@ -1,13 +1,7 @@
-Metadata-Version: 2.1 Name: pytrading212 Version: 0.2.6 Summary: Unofficial
-Trading212 API Home-page: https://github.com/HellAmbro/Trading212API Author:
-HellAmbro Author-email: frambrosini1998@gmail.com Classifier: Programming
-Language :: Python :: 3.9 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.9 Description-Content-Type: text/markdown License-File:
-LICENSE
   # PyTrading212 API ## Unofficial API for Trading212 ### Unofficial API for
       Trading212 broker. ### [Documentation](https://hellambro.github.io/
   Trading212API/) ### Support the Project #### With a :star: [![Star History
            Chart](https://api.star-history.com/svg?repos=HellAmbro/
         Trading212API&type=Date)](https://star-history.com/#HellAmbro/
        Trading212API&Date) #### With a donation _[_B_u_y_ _M_e_ _A_ _C_o_f_f_e_e_]**LTC**
  LbAzhtHBvQ2JCGhrcefUuvwNrv9VrQJoyJ **BTC** 1JWhMC3tiSjyR6t7BJuM7YRDg3xvPM2MDk
```

### Comparing `pytrading212-0.2.6/README.md` & `pytrading212-0.2.7/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,395 +1,418 @@
-<div align="center">
-
-# PyTrading212 API
-
-## Unofficial API for Trading212
-### Unofficial API for Trading212 broker.
-
-
-
-### [Documentation](https://hellambro.github.io/Trading212API/)
-
-### Support the Project
-
-#### With a :star:
-
-[![Star History Chart](https://api.star-history.com/svg?repos=HellAmbro/Trading212API&type=Date)](https://star-history.com/#HellAmbro/Trading212API&Date)
-
-#### With a donation
-
-<a href="https://www.buymeacoffee.com/hellambro" target="_blank"><img src="https://cdn.buymeacoffee.com/buttons/v2/default-blue.png" alt="Buy Me A Coffee" height="50" ></a>
-
-**LTC** LbAzhtHBvQ2JCGhrcefUuvwNrv9VrQJoyJ
-
-**BTC** 1JWhMC3tiSjyR6t7BJuM7YRDg3xvPM2MDk
-
-**ETH** 0x51f1f0061eadc024ab4bd1f3658d249044160006
-
-</div>
-
-<div align="left">
-
-### Discord Channel for support
-[Discord](https://discord.gg/PmWemEUA)
-
-  ## Installation
-
-```bash
-pip install pytrading212
-```
-
-### Warning :warning:
-
-When you are using the API you cannot access Trading212 from other devices and browsers, except for the webdriver.New
-access from another browser may disconnect the current session, invalidating the _cookie_ and making the API not work.
-
-## PyTrading212 Usage
-
-For a full reference please look inside **examples** folder
-
-### Equity Example
-
-```python
-from selenium import webdriver
-from selenium.webdriver.chrome.service import Service
-
-from pytrading212 import Equity
-from pytrading212 import Mode, EquityOrder, OrderType
-
-driver = webdriver.Chrome(service=Service())
-equity = Equity(email='your_email', password='your_password', driver=driver, mode=Mode.DEMO)
-
-# Invalid order: voluntary typo-error in instrument code
-order = EquityOrder(instrument_code="AAAAPL_US_EQ", order_type=OrderType.MARKET, quantity=2)
-is_valid, reason = equity.check_order(order)
-if is_valid:
-    print("Your order is valid, can be executed.")
-else:
-    print("Your order is not valid. The reason is: ", reason)
-# Valid order
-order = EquityOrder(instrument_code="AAPL_US_EQ", order_type=OrderType.MARKET, quantity=2)
-
-# Check order validity (recommended)
-if equity.check_order(order)[0]:
-    # Review order (recommended)
-    print(equity.review_order(order))
-    # Execute order
-    print(equity.execute_order(order))
-
-equity.finish()
-```
-
-### CFD Example
-
-```python
-from selenium import webdriver
-from selenium.webdriver.chrome.service import Service
-
-from pytrading212 import CFD, CFDOrder
-from pytrading212 import Mode
-
-driver = webdriver.Chrome(service=Service())
-cfd = CFD(email='your_email', password='your_password', driver=driver, mode=Mode.DEMO)
-
-instrument_code = "AAPL"
-
-cfd_order = CFDOrder(instrument_code=instrument_code,
-                     quantity=-0.1,  # Sell (quantity is negative)
-                     target_price=cfd.get_current_price(instrument_code=instrument_code)
-                     )
-
-print(cfd.execute_order(order=cfd_order))
-```
-
-### PyTrading212 initialization
-
-:warning: As now March 2023 only one instance at time is supported. :warning:
-
-:x: This means that you cannot initialize both **Equity** and **CFD** :x:
-
-PyTrading212 **Equity** instance
-
-```python
-driver = webdriver.Chrome(service=Service())
-equity = Equity(email='your_email', password='your_password', driver=driver, mode=Mode.DEMO)
-```
-
-PyTrading212 **CFD** instance
-
-```python
-driver = webdriver.Chrome(service=Service())
-cfd = CFD(email='your_email', password='your_password', driver=driver, mode=Mode.DEMO)
-```
-
-### PyTrading212 close session
-
-Close the session, also the webdriver is closed.
-
-```python
-equity.finish()
-```
-
-or
-
-```python
-cfd.finish()
-```
-
-### Getting Instrument Code
-
-```python
-print(equity.get_companies())
-```
-
-or
-
-```python
-print(cfd.get_companies())
-```
-
-Returns a JSON with all Instrument code that you can trade, both CFD and Equity.
-
-**Note**: Instrument code is different for _CFD_ and _Equity_ even for the same Stock.
-For example **Apple** Instrument Code is:
-
-```
-CFD: AAPL
-EQUITY: AAPL_US_EQ
-```
-
-### Order Structure
-
-![order](docs/imgs/order_structure.png)
-
-### [Equity Order](https://hellambro.github.io/Trading212API/order.html#pytrading212.order.EquityOrder)
-
-It's possible to create **equity orders** directly from `EquityOrder` class
-
-```python
-# Buy
-order = EquityOrder(instrument_code="AAPL_US_EQ", order_type=OrderType.MARKET, quantity=1)
-equity.execute_order(order=order)
-```
-
-or
-
-```python
-# Buy
-market_order = MarketOrder(instrument_code="AAPL_US_EQ", quantity=1)
-equity.execute_order(order=market_order)
-```
-
-These two orders are equivalent, you can use both ways indifferently.
-
-For selling stocks (**that you own**, for short-selling see CFD section below) you just need to change the sign of
-_quantity_ or _value_ property
-
-```python
-# Sell
-order = EquityOrder(instrument_code="AAPL_US_EQ", order_type=OrderType.MARKET, quantity=-1)
-equity.execute_order(order=order)
-```
-
-or
-
-```python
-# Sell
-market_order = MarketOrder(instrument_code="AAPL_US_EQ", quantity=-1)
-equity.execute_order(order=market_order)
-```
-
-All other **equity order classes** are wrappers of the `EquityOrder`
-
-#### Wrappers for Equity Orders
-
-- MarketOrder
-
-```python
-market_order = MarketOrder(instrument_code="AAPL_US_EQ", quantity=1)
-```
-
-- LimitOrder
-
-```python
-limit_order = LimitOrder(instrument_code="AAPL_US_EQ",
-                         quantity=2,
-                         limit_price=150.0,
-                         time_validity=constants.TimeValidity.DAY)
-```
-
-- StopOrder
-
-```python
-stop_order = StopOrder(instrument_code="AAPL_US_EQ",
-                       quantity=-3,  # Sell
-                       stop_price=180.0,
-                       time_validity=constants.TimeValidity.GOOD_TILL_CANCEL)
-```
-
-- StopLimitOrder
-
-```python
-stop_limit_order = StopLimitOrder(instrument_code="AAPL_US_EQ",
-                                  quantity=1,
-                                  limit_price=150,
-                                  stop_price=180,
-                                  time_validity=constants.TimeValidity.DAY)
-```
-
-- ValueOrder
-
-```python
-value_order = ValueOrder(instrument_code="AAPL_US_EQ", value=2500.0)
-```
-
-These classes allow to simplify the creation of orders, avoiding errors for omitted parameters,
-improving code readability.
-
-### [CFD Order](https://hellambro.github.io/Trading212API/order.html#pytrading212.order.CFDOrder)
-
-You can use 3 types of CFD Orders: `Market`, `Limit/Stop`, `OCO` (Order Cancel Order)
-
-#### Market Order
-
-- Market Order without Take Profit and Stop Loss
-
-```python
-instrument_code = "AAPL"
-cfd_order = CFDMarketOrder(instrument_code=instrument_code,
-                           quantity=0.1,  # Buy (quantity is positive)
-                           target_price=cfd.get_current_price(instrument_code=instrument_code))
-```
-
-- MarketOrder with Take Profit (_limit_distance_)
-
-```python
-instrument_code = "AAPL"
-current_price = cfd.get_current_price(instrument_code=instrument_code)
-cfd_order = CFDMarketOrder(instrument_code=instrument_code,
-                           quantity=0.5,
-                           target_price=current_price,
-                           limit_distance=5.0)
-```
-
-- MarketOrder with Stop Loss (_stop_distance_)
-
-```python
-instrument_code = "AAPL"
-current_price = cfd.get_current_price(instrument_code=instrument_code)
-cfd_order = CFDMarketOrder(instrument_code=instrument_code,
-                           quantity=0.5,
-                           target_price=current_price,
-                           stop_distance=2.0)
-```
-
-- MarketOrder with Stop Loss and Take Profit
-
-```python
-instrument_code = "AAPL"
-current_price = cfd.get_current_price(instrument_code=instrument_code)
-cfd_order = CFDMarketOrder(instrument_code=instrument_code,
-                           quantity=0.5,
-                           target_price=current_price,
-                           limit_distance=4.0,
-                           stop_distance=2.0,
-                           )
-```
-
-- CFD Stop Limit Order
-
-#### Note about stop and limit distance
-
-`stop_distance` and `limit_distance` are the _distance_ between the **current price** and SL/TP price.
-You should add/subtract these quantities to the current price in order to get TP/SL price.
-
-```                                                   
-current_price = 150.0
-limit_distance = 10.0   -> TP price = 150.0 + 10.0 = 160.0
-stop_distance = 5.0     -> SL price = 150.0 - 5.0 =  145.0
-```
-
-#### Limit/Stop Order (Pending Order with specified price)
-
-- Limit/Stop Order with Take Profit and Stop Loss
-
-```python
-instrument_code = "AAPL"
-# Target price of Apple Stock, the current price - 20.0$ 
-target_price = cfd.get_current_price(instrument_code=instrument_code) - 20.0
-# Put a pending Buy Order when the price triggers target_price
-cfd_order = CFDLimitStopOrder(instrument_code=instrument_code,
-                              target_price=target_price,
-                              quantity=1,
-                              take_profit=target_price + 10,
-                              # TP when Apple's stock price is  10.0$ above the target_price
-                              stop_loss=target_price - 5)  # TP when Apple's stock price is  5.0$ below the target_price
-```
-
-- Limit/Stop Order without Take Profit
-
-```python
-instrument_code = "AAPL"
-target_price = cfd.get_current_price(instrument_code=instrument_code) - 10.0
-cfd_order = CFDLimitStopOrder(instrument_code=instrument_code,
-                              target_price=target_price,
-                              quantity=1,
-                              stop_loss=target_price - 3.0)
-```
-
-- Limit/Stop Order without Stop Loss
-
-```python
-instrument_code = "AAPL"
-target_price = cfd.get_current_price(instrument_code=instrument_code) - 30.0
-cfd_order = CFDLimitStopOrder(instrument_code=instrument_code,
-                              target_price=target_price,
-                              quantity=1,
-                              take_profit=target_price + 20)
-```
-
-- Limit/Stop Order without Take Profit and Stop Loss
-
-```python
-instrument_code = "AAPL"
-target_price = cfd.get_current_price(instrument_code=instrument_code) + 30.0
-cfd_order = CFDLimitStopOrder(instrument_code=instrument_code,
-                              target_price=target_price,
-                              quantity=-1) # Sell 
-```
-
-**Note about stop_loss and take_profit**
-
-`stop_loss` and `take_profit` indicates the price of the stock when we want to make the TP or SL trades.
-
-#### OCO Order (Order Cancel Order)
-
-**Buy** 1 Apple's Stock when the price drops below 150.0$ (now ~162.0$): execute `order1`, cancel `order2`
-
-or
-
-**Sell** 1 Apple's Stock when the price rise above 180.0$ (now ~162.0$): execute `order2`, cancel `order1`
-```python
-instrument_code = "AAPL"
-cfd_oco_order = CFDOCOOrder(instrument_code=instrument_code,
-                            order1=CFDOCOOrder.OCOSubOrder(price=150, quantity=1),
-                            order2=CFDOCOOrder.OCOSubOrder(price=180.0, quantity=-1))
-```
-
-### Useful resources
-
-- [Use Trading212 for Automatic Trading: an introduction to pytrading212 (Depreacted since v0.2.5)](https://medium.com/@francescoelambroambrosini/use-trading212-for-automatic-trading-an-introduction-to-pytrading212-367449b40a6)
-- [Driver requirements](https://www.selenium.dev/documentation/en/webdriver/driver_requirements)
-- [Getting started with WebDriver](https://www.selenium.dev/documentation/en/getting_started_with_webdriver/)
-
-### Disclaimer
-
-Nor me or Trading212 are responsible for the use of this API, first make sure that everything works well through the use
-of a **DEMO** account, then switch to **REAL** mode.
-
-In addition, I don't take responsibility for the accuracy of the information reported here and the proper functioning of
-the API
-
-All trademarks, logos and brand names are the property of their respective owners. All company, product and service
-names used in this website are for identification purposes only.
-
-</div>
+Metadata-Version: 2.1
+Name: pytrading212
+Version: 0.2.7
+Summary: Unofficial Trading212 API
+License: MIT
+Author: HellAmbro
+Author-email: frambrosini1998@gmail.com
+Requires-Python: >=3.7,<4.0
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Requires-Dist: requests (>=2.28.2,<3.0.0)
+Requires-Dist: rich (>=13.3.2,<14.0.0)
+Requires-Dist: selenium (>=4.8.2,<5.0.0)
+Requires-Dist: webdriver-manager (>=3.8.5,<4.0.0)
+Description-Content-Type: text/markdown
+
+<div align="center">
+
+# PyTrading212 API
+
+## Unofficial API for Trading212
+### Unofficial API for Trading212 broker.
+
+
+
+### [Documentation](https://hellambro.github.io/Trading212API/)
+
+### Support the Project
+
+#### With a :star:
+
+[![Star History Chart](https://api.star-history.com/svg?repos=HellAmbro/Trading212API&type=Date)](https://star-history.com/#HellAmbro/Trading212API&Date)
+
+#### With a donation
+
+<a href="https://www.buymeacoffee.com/hellambro" target="_blank"><img src="https://cdn.buymeacoffee.com/buttons/v2/default-blue.png" alt="Buy Me A Coffee" height="50" ></a>
+
+**LTC** LbAzhtHBvQ2JCGhrcefUuvwNrv9VrQJoyJ
+
+**BTC** 1JWhMC3tiSjyR6t7BJuM7YRDg3xvPM2MDk
+
+**ETH** 0x51f1f0061eadc024ab4bd1f3658d249044160006
+
+</div>
+
+<div align="left">
+
+### Discord Channel for support
+[Discord](https://discord.gg/PmWemEUA)
+
+  ## Installation
+
+```bash
+pip install pytrading212
+```
+
+### Warning :warning:
+
+When you are using the API you cannot access Trading212 from other devices and browsers, except for the webdriver.New
+access from another browser may disconnect the current session, invalidating the _cookie_ and making the API not work.
+
+## PyTrading212 Usage
+
+For a full reference please look inside **examples** folder
+
+### Equity Example
+
+```python
+from selenium import webdriver
+from selenium.webdriver.chrome.service import Service
+
+from pytrading212 import Equity
+from pytrading212 import Mode, EquityOrder, OrderType
+
+driver = webdriver.Chrome(service=Service())
+equity = Equity(email='your_email', password='your_password', driver=driver, mode=Mode.DEMO)
+
+# Invalid order: voluntary typo-error in instrument code
+order = EquityOrder(instrument_code="AAAAPL_US_EQ", order_type=OrderType.MARKET, quantity=2)
+is_valid, reason = equity.check_order(order)
+if is_valid:
+    print("Your order is valid, can be executed.")
+else:
+    print("Your order is not valid. The reason is: ", reason)
+# Valid order
+order = EquityOrder(instrument_code="AAPL_US_EQ", order_type=OrderType.MARKET, quantity=2)
+
+# Check order validity (recommended)
+if equity.check_order(order)[0]:
+    # Review order (recommended)
+    print(equity.review_order(order))
+    # Execute order
+    print(equity.execute_order(order))
+
+equity.finish()
+```
+
+### CFD Example
+
+```python
+from selenium import webdriver
+from selenium.webdriver.chrome.service import Service
+
+from pytrading212 import CFD, CFDOrder
+from pytrading212 import Mode
+
+driver = webdriver.Chrome(service=Service())
+cfd = CFD(email='your_email', password='your_password', driver=driver, mode=Mode.DEMO)
+
+instrument_code = "AAPL"
+
+cfd_order = CFDOrder(instrument_code=instrument_code,
+                     quantity=-0.1,  # Sell (quantity is negative)
+                     target_price=cfd.get_current_price(instrument_code=instrument_code)
+                     )
+
+print(cfd.execute_order(order=cfd_order))
+```
+
+### PyTrading212 initialization
+
+:warning: As now March 2023 only one instance at time is supported. :warning:
+
+:x: This means that you cannot initialize both **Equity** and **CFD** :x:
+
+PyTrading212 **Equity** instance
+
+```python
+driver = webdriver.Chrome(service=Service())
+equity = Equity(email='your_email', password='your_password', driver=driver, mode=Mode.DEMO)
+```
+
+PyTrading212 **CFD** instance
+
+```python
+driver = webdriver.Chrome(service=Service())
+cfd = CFD(email='your_email', password='your_password', driver=driver, mode=Mode.DEMO)
+```
+
+### PyTrading212 close session
+
+Close the session, also the webdriver is closed.
+
+```python
+equity.finish()
+```
+
+or
+
+```python
+cfd.finish()
+```
+
+### Getting Instrument Code
+
+```python
+print(equity.get_companies())
+```
+
+or
+
+```python
+print(cfd.get_companies())
+```
+
+Returns a JSON with all Instrument code that you can trade, both CFD and Equity.
+
+**Note**: Instrument code is different for _CFD_ and _Equity_ even for the same Stock.
+For example **Apple** Instrument Code is:
+
+```
+CFD: AAPL
+EQUITY: AAPL_US_EQ
+```
+
+### Order Structure
+
+![order](docs/imgs/order_structure.png)
+
+### [Equity Order](https://hellambro.github.io/Trading212API/order.html#pytrading212.order.EquityOrder)
+
+It's possible to create **equity orders** directly from `EquityOrder` class
+
+```python
+# Buy
+order = EquityOrder(instrument_code="AAPL_US_EQ", order_type=OrderType.MARKET, quantity=1)
+equity.execute_order(order=order)
+```
+
+or
+
+```python
+# Buy
+market_order = MarketOrder(instrument_code="AAPL_US_EQ", quantity=1)
+equity.execute_order(order=market_order)
+```
+
+These two orders are equivalent, you can use both ways indifferently.
+
+For selling stocks (**that you own**, for short-selling see CFD section below) you just need to change the sign of
+_quantity_ or _value_ property
+
+```python
+# Sell
+order = EquityOrder(instrument_code="AAPL_US_EQ", order_type=OrderType.MARKET, quantity=-1)
+equity.execute_order(order=order)
+```
+
+or
+
+```python
+# Sell
+market_order = MarketOrder(instrument_code="AAPL_US_EQ", quantity=-1)
+equity.execute_order(order=market_order)
+```
+
+All other **equity order classes** are wrappers of the `EquityOrder`
+
+#### Wrappers for Equity Orders
+
+- MarketOrder
+
+```python
+market_order = MarketOrder(instrument_code="AAPL_US_EQ", quantity=1)
+```
+
+- LimitOrder
+
+```python
+limit_order = LimitOrder(instrument_code="AAPL_US_EQ",
+                         quantity=2,
+                         limit_price=150.0,
+                         time_validity=constants.TimeValidity.DAY)
+```
+
+- StopOrder
+
+```python
+stop_order = StopOrder(instrument_code="AAPL_US_EQ",
+                       quantity=-3,  # Sell
+                       stop_price=180.0,
+                       time_validity=constants.TimeValidity.GOOD_TILL_CANCEL)
+```
+
+- StopLimitOrder
+
+```python
+stop_limit_order = StopLimitOrder(instrument_code="AAPL_US_EQ",
+                                  quantity=1,
+                                  limit_price=150,
+                                  stop_price=180,
+                                  time_validity=constants.TimeValidity.DAY)
+```
+
+- ValueOrder
+
+```python
+value_order = ValueOrder(instrument_code="AAPL_US_EQ", value=2500.0)
+```
+
+These classes allow to simplify the creation of orders, avoiding errors for omitted parameters,
+improving code readability.
+
+### [CFD Order](https://hellambro.github.io/Trading212API/order.html#pytrading212.order.CFDOrder)
+
+You can use 3 types of CFD Orders: `Market`, `Limit/Stop`, `OCO` (Order Cancel Order)
+
+#### Market Order
+
+- Market Order without Take Profit and Stop Loss
+
+```python
+instrument_code = "AAPL"
+cfd_order = CFDMarketOrder(instrument_code=instrument_code,
+                           quantity=0.1,  # Buy (quantity is positive)
+                           target_price=cfd.get_current_price(instrument_code=instrument_code))
+```
+
+- MarketOrder with Take Profit (_limit_distance_)
+
+```python
+instrument_code = "AAPL"
+current_price = cfd.get_current_price(instrument_code=instrument_code)
+cfd_order = CFDMarketOrder(instrument_code=instrument_code,
+                           quantity=0.5,
+                           target_price=current_price,
+                           limit_distance=5.0)
+```
+
+- MarketOrder with Stop Loss (_stop_distance_)
+
+```python
+instrument_code = "AAPL"
+current_price = cfd.get_current_price(instrument_code=instrument_code)
+cfd_order = CFDMarketOrder(instrument_code=instrument_code,
+                           quantity=0.5,
+                           target_price=current_price,
+                           stop_distance=2.0)
+```
+
+- MarketOrder with Stop Loss and Take Profit
+
+```python
+instrument_code = "AAPL"
+current_price = cfd.get_current_price(instrument_code=instrument_code)
+cfd_order = CFDMarketOrder(instrument_code=instrument_code,
+                           quantity=0.5,
+                           target_price=current_price,
+                           limit_distance=4.0,
+                           stop_distance=2.0,
+                           )
+```
+
+- CFD Stop Limit Order
+
+#### Note about stop and limit distance
+
+`stop_distance` and `limit_distance` are the _distance_ between the **current price** and SL/TP price.
+You should add/subtract these quantities to the current price in order to get TP/SL price.
+
+```                                                   
+current_price = 150.0
+limit_distance = 10.0   -> TP price = 150.0 + 10.0 = 160.0
+stop_distance = 5.0     -> SL price = 150.0 - 5.0 =  145.0
+```
+
+#### Limit/Stop Order (Pending Order with specified price)
+
+- Limit/Stop Order with Take Profit and Stop Loss
+
+```python
+instrument_code = "AAPL"
+# Target price of Apple Stock, the current price - 20.0$ 
+target_price = cfd.get_current_price(instrument_code=instrument_code) - 20.0
+# Put a pending Buy Order when the price triggers target_price
+cfd_order = CFDLimitStopOrder(instrument_code=instrument_code,
+                              target_price=target_price,
+                              quantity=1,
+                              take_profit=target_price + 10,
+                              # TP when Apple's stock price is  10.0$ above the target_price
+                              stop_loss=target_price - 5)  # TP when Apple's stock price is  5.0$ below the target_price
+```
+
+- Limit/Stop Order without Take Profit
+
+```python
+instrument_code = "AAPL"
+target_price = cfd.get_current_price(instrument_code=instrument_code) - 10.0
+cfd_order = CFDLimitStopOrder(instrument_code=instrument_code,
+                              target_price=target_price,
+                              quantity=1,
+                              stop_loss=target_price - 3.0)
+```
+
+- Limit/Stop Order without Stop Loss
+
+```python
+instrument_code = "AAPL"
+target_price = cfd.get_current_price(instrument_code=instrument_code) - 30.0
+cfd_order = CFDLimitStopOrder(instrument_code=instrument_code,
+                              target_price=target_price,
+                              quantity=1,
+                              take_profit=target_price + 20)
+```
+
+- Limit/Stop Order without Take Profit and Stop Loss
+
+```python
+instrument_code = "AAPL"
+target_price = cfd.get_current_price(instrument_code=instrument_code) + 30.0
+cfd_order = CFDLimitStopOrder(instrument_code=instrument_code,
+                              target_price=target_price,
+                              quantity=-1) # Sell 
+```
+
+**Note about stop_loss and take_profit**
+
+`stop_loss` and `take_profit` indicates the price of the stock when we want to make the TP or SL trades.
+
+#### OCO Order (Order Cancel Order)
+
+**Buy** 1 Apple's Stock when the price drops below 150.0$ (now ~162.0$): execute `order1`, cancel `order2`
+
+or
+
+**Sell** 1 Apple's Stock when the price rise above 180.0$ (now ~162.0$): execute `order2`, cancel `order1`
+```python
+instrument_code = "AAPL"
+cfd_oco_order = CFDOCOOrder(instrument_code=instrument_code,
+                            order1=CFDOCOOrder.OCOSubOrder(price=150, quantity=1),
+                            order2=CFDOCOOrder.OCOSubOrder(price=180.0, quantity=-1))
+```
+
+### Useful resources
+
+- [Use Trading212 for Automatic Trading: an introduction to pytrading212 (Depreacted since v0.2.5)](https://medium.com/@francescoelambroambrosini/use-trading212-for-automatic-trading-an-introduction-to-pytrading212-367449b40a6)
+- [Driver requirements](https://www.selenium.dev/documentation/en/webdriver/driver_requirements)
+- [Getting started with WebDriver](https://www.selenium.dev/documentation/en/getting_started_with_webdriver/)
+
+### Disclaimer
+
+Nor me or Trading212 are responsible for the use of this API, first make sure that everything works well through the use
+of a **DEMO** account, then switch to **REAL** mode.
+
+In addition, I don't take responsibility for the accuracy of the information reported here and the proper functioning of
+the API
+
+All trademarks, logos and brand names are the property of their respective owners. All company, product and service
+names used in this website are for identification purposes only.
+
+</div>
+
```

#### html2text {}

```diff
@@ -1,7 +1,18 @@
+Metadata-Version: 2.1 Name: pytrading212 Version: 0.2.7 Summary: Unofficial
+Trading212 API License: MIT Author: HellAmbro Author-email:
+frambrosini1998@gmail.com Requires-Python: >=3.7,<4.0 Classifier: License ::
+OSI Approved :: MIT License Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7 Classifier: Programming
+Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
+Language :: Python :: 3.11 Classifier: Programming Language :: Python :: 3.12
+Requires-Dist: requests (>=2.28.2,<3.0.0) Requires-Dist: rich
+(>=13.3.2,<14.0.0) Requires-Dist: selenium (>=4.8.2,<5.0.0) Requires-Dist:
+webdriver-manager (>=3.8.5,<4.0.0) Description-Content-Type: text/markdown
   # PyTrading212 API ## Unofficial API for Trading212 ### Unofficial API for
       Trading212 broker. ### [Documentation](https://hellambro.github.io/
   Trading212API/) ### Support the Project #### With a :star: [![Star History
            Chart](https://api.star-history.com/svg?repos=HellAmbro/
         Trading212API&type=Date)](https://star-history.com/#HellAmbro/
        Trading212API&Date) #### With a donation _[_B_u_y_ _M_e_ _A_ _C_o_f_f_e_e_]**LTC**
  LbAzhtHBvQ2JCGhrcefUuvwNrv9VrQJoyJ **BTC** 1JWhMC3tiSjyR6t7BJuM7YRDg3xvPM2MDk
```

### Comparing `pytrading212-0.2.6/pytrading212/trading212.py` & `pytrading212-0.2.7/pytrading212/trading212.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,358 +1,352 @@
-"""API for Trading212 Platform"""
-
-import json
-import logging
-import re
-import time
-from datetime import datetime
-from time import strftime
-from urllib.parse import urlencode
-
-import requests
-from selenium import webdriver
-from selenium.common.exceptions import NoSuchElementException
-from selenium.webdriver.common.by import By
-from selenium.webdriver.support import expected_conditions
-from selenium.webdriver.support.ui import WebDriverWait
-
-from pytrading212 import constants, console
-from pytrading212.instrument import CFDInstrument
-from pytrading212.order import CFDOrder, EquityOrder
-from pytrading212.position import Position
-
-
-class Trading212:
-    def __init__(
-            self,
-            email: str,
-            password: str,
-            driver: webdriver,
-            mode: constants.Mode = constants.Mode.DEMO,
-            trading: constants.Trading = constants.Trading.EQUITY,
-    ):
-        self.session = f"TRADING212_SESSION_{mode.name}"
-        self.base_url = f"https://{mode.name.lower()}.trading212.com"
-
-        console.log(f"Starting PyTrading212 v{constants.PYTRADING212_VERSION}\n"
-                    f"Trading: [green]{trading.name}[/green] \n"
-                    f"Mode: [green]{mode.name}[/green]")
-
-        self.driver = driver
-        self.driver.get(constants.URL_LOGIN)
-
-        # Click Accept all cookies if it appears
-        try:
-            console.log("Closing 'Cookies Popup'")
-            self.driver.find_element(By.CLASS_NAME, constants.CLASS_COOKIES_NOTICE_BUTTON).click()
-        except NoSuchElementException:
-            pass  # ignore
-
-        console.log("Authenticating")
-
-        WebDriverWait(self.driver, 120).until(expected_conditions.visibility_of_element_located((By.NAME, "email")))
-
-        # Authenticate
-        self.driver.find_element(By.NAME, "email").send_keys(email)
-        self.driver.find_element(By.NAME, "password").send_keys(password)
-
-        # Click login button
-        self.driver.find_element(By.CLASS_NAME, constants.CLASS_LOGIN_BUTTON).click()
-
-        # Wait until the site is fully loaded, 120 seconds is a lot, but the site sometimes is very slow
-        WebDriverWait(self.driver, 120).until(expected_conditions.
-                                              visibility_of_element_located((By.CLASS_NAME, "company-logo")))
-
-        self.user_agent = self.driver.execute_script("return navigator.userAgent;")
-
-        # Redirect to correct mode, DEMO or LIVE
-        if mode.name not in self.driver.current_url:
-            self.driver.get(self.base_url)
-            WebDriverWait(self.driver, 120).until(expected_conditions.
-                                                  visibility_of_element_located((By.CLASS_NAME, "company-logo")))
-
-        # Switch to right trading session: CFD or EQUITY
-        self.switch_to(trading=trading)
-
-        # Get session cookie
-        cookies = self.driver.get_cookies()
-        if cookies is not None:
-            for cookie in cookies:
-                # Get appropriate cookie for this session, live or demo
-                if self.session in cookie['name']:
-                    self.cookie = f"{self.session}={cookie['value']};"
-        else:
-            raise Exception("Unable to get cookies, aborting.")
-
-        # Necessary headers for requests
-        self.headers = {
-            "Accept": "application/json",
-            "Content-Type": "application/json",
-            "User-Agent": self.user_agent,
-            "Cookie": self.cookie,
-        }
-
-        self.companies = self.get_companies()
-
-    def __enter__(self):
-        return self
-
-    def __exit__(self, exc_type, exc_val, exc_tb):
-        self.finish()
-
-    def finish(self):
-        console.log("Closing session.")
-        self.driver.close()
-
-    def switch_to(self, trading: constants.Trading):
-        if not self.driver.find_elements(By.ID, "platform-loader"):
-            self.driver.find_element(By.CLASS_NAME, "account-menu-info").click()
-            WebDriverWait(self.driver, 10).until(expected_conditions.
-                                                 visibility_of_element_located((By.CLASS_NAME, "account-types")))
-            element_account_types = self.driver.find_element(By.CLASS_NAME, "account-types")
-            if trading == constants.Trading.CFD:
-                element_account_types.find_element(By.CLASS_NAME, "cfd").click()
-                WebDriverWait(self.driver, 60).until(expected_conditions.
-                                                     visibility_of_element_located((By.CLASS_NAME, "cfd-icon")))
-            elif trading == constants.Trading.EQUITY:
-                element_account_types.find_element(By.CLASS_NAME, "equity").click()
-                WebDriverWait(self.driver, 60).until(expected_conditions.
-                                                     visibility_of_element_located((By.CLASS_NAME, "equity-icon")))
-        else:
-            self.switch_to(trading)
-
-    def get_funds(self):
-        """Get your funds, free, available."""
-        response = requests.get(
-            f"{self.base_url}/rest/v2/customer/accounts/funds", headers=self.headers
-        )
-        return json.loads(response.content.decode("utf-8"))
-
-    def last_hour_hotlist(self):
-        """Trading 212 last hour hotlist"""
-        response = requests.get(
-            f"{self.base_url}/trading212.com/rest/positions-tracker/deltas/hourly/1"
-        )
-        return json.loads(response.content.decode("utf-8"))
-
-    def get_orders(self, older_than: datetime, newer_than: datetime):
-        """Get orders within a range of dates"""
-        params = {
-            'olderThan': strftime(older_than.isoformat()),
-            'newerThan': strftime(newer_than.isoformat())
-        }
-
-        response = requests.get(
-            f"{self.base_url}/rest/history/orders", headers=self.headers, params=urlencode(params)
-        )
-        return json.loads(response.content.decode("utf-8"))
-
-    def get_transactions(self, older_than: datetime, newer_than: datetime):
-        """Get transactions within a range of dates"""
-        params = {
-            'olderThan': strftime(older_than.isoformat()),
-            'newerThan': strftime(newer_than.isoformat())
-        }
-        response = requests.get(
-            f"{self.base_url}/rest/history/transactions", headers=self.headers, params=urlencode(params)
-        )
-        return json.loads(response.content.decode("utf-8"))
-
-    def get_order_details(self, details_path):
-        """Get Order Details"""
-        response = requests.get(f"{self.base_url}/rest/history{details_path}", headers=self.headers)
-        return json.loads(response.content.decode("utf-8"))
-
-    def get_dividends(self, older_than: datetime, newer_than: datetime):
-        """Get dividends within a range of dates"""
-        params = {'olderThan': strftime(older_than.isoformat()),
-                  'newerThan': strftime(newer_than.isoformat())
-                  }
-
-        response = requests.get(
-            f"{self.base_url}/rest/history/dividends", headers=self.headers, params=urlencode(params)
-        )
-        return json.loads(response.content.decode("utf-8"))
-
-    def get_fundamentals(self, ticker, language_code: str = "en"):
-        """Get fundamentals of a company by its isin"""
-        params = {'ticker': ticker,
-                  'languageCode': language_code
-                  }
-
-        response = requests.get(f"{self.base_url}/rest/companies/v2/fundamentals",
-                                params=params)
-        return json.loads(response.content.decode("utf-8"))
-
-    def get_portfolio_performance(self, time_period: constants.Period):
-        """Get Portfolio Performance"""
-        response = requests.get(
-            url=f"{self.base_url}/rest/v2/portfolio?period={time_period}",
-            headers=self.headers,
-        )
-        return json.loads(response.content.decode("utf-8"))
-
-    def get_portfolio_composition(self):
-        """Get Portfolio Composition"""
-        # click portfolio section on right-sidepanel
-        right_sidepanel_portfolio_class = 'portfolio-icon'
-        condition = expected_conditions.visibility_of_element_located(
-            (By.CLASS_NAME, right_sidepanel_portfolio_class)
-        )
-        WebDriverWait(self.driver, 30).until(condition)
-        self.driver.find_element(By.CLASS_NAME, right_sidepanel_portfolio_class).click()
-
-        positions = []
-        try:
-            # click on investments
-            self.driver.find_element(By.CLASS_NAME, 'investment-tab').click()
-            for item in self.driver.find_elements(By.CLASS_NAME, "investment-item"):
-                ticker = item.get_attribute("data-qa-item")
-                value = item.find_element(By.CLASS_NAME, "total-value").text
-                quantity = item.find_element(By.CLASS_NAME, "quantity").text
-                total_return = item.find_element(By.CLASS_NAME, "return").text
-                position = Position(ticker, value, quantity, total_return)
-                positions.append(position.__dict__)
-        except Exception as e:
-            logging.error(e)  # portfolio is empty
-        return positions
-
-    def get_companies(self):
-        """Get Ticker of all Trading212 tradable companies"""
-        response = requests.get(
-            url=f"{self.base_url}/rest/companies",
-            headers=self.headers
-        )
-        return json.loads(response.content.decode("utf-8"))
-
-    def search(self, query):
-        """Search a company"""
-        found = []
-        companies = self.get_companies()
-        for company in companies:
-            if query in company["ticker"]:
-                found.append(company["ticker"])
-
-        response = requests.post(
-            f"{self.base_url}/charting/prices?withFakes=false",
-            headers=self.headers,
-            data=found.__str__().replace("'", '"'),
-        )  # ' with " for Trading212 compatibility
-        return json.loads(response.content.decode("utf-8"))
-
-
-class Equity(Trading212):
-    """Trading 212 Equity"""
-
-    def __init__(self, email: str, password: str, driver: webdriver, mode: constants.Mode = constants.Mode.DEMO):
-        super().__init__(email, password, driver, mode, constants.Trading.EQUITY)
-
-    def review_order(self, order: EquityOrder):
-        """Preview of the order, with added costs and other useful data"""
-        # Check if it is a 'value' order or a 'quantity' order
-        if hasattr(order, 'value'):
-            url = f"{self.base_url}/rest/v1/equity/value-order/review"
-        else:
-            url = f"{self.base_url}/rest/public/added-costs"
-        response = requests.post(
-            url=url,
-            headers=self.headers,
-            data=order.to_json(),
-        )
-        return json.loads(response.content.decode("utf-8"))
-
-    def execute_order(self, order: EquityOrder):
-        """Execute equity order"""
-        # Check if it is a 'value' order or a 'quantity' order
-        if hasattr(order, 'value'):
-            url = f"{self.base_url}/rest/v1/equity/value-order"
-        else:
-            url = f"{self.base_url}/rest/public/v2/equity/order"
-        response = requests.post(
-            url=url,
-            headers=self.headers,
-            data=order.to_json(),
-        )
-        return json.loads(response.content.decode("utf-8"))
-
-    def cancel_order(self, order_id):
-        """Cancel a pending order"""
-        response = requests.delete(
-            url=f"{self.base_url}/rest/public/v2/equity/order/{order_id}",
-            headers=self.headers,
-        )
-        return json.loads(response.content.decode("utf-8"))
-
-    def check_order(self, equity_order: EquityOrder) -> [bool, str]:
-        """Check if Order is valid."""
-        is_valid_ticker = False, f"Instrument Code {equity_order.instrument_code} is not a valid Trading212 Ticker"
-        for company in self.get_companies():
-            if company['ticker'] == equity_order.instrument_code:
-                is_valid_ticker = True, f"Instrument Code {equity_order.instrument_code} is valid Trading212 Ticker"
-
-        return is_valid_ticker
-
-    def min_max_sell_buy(self, instrument_code: str):
-        params = {'instrumentCode': instrument_code}
-        response = requests.get(
-            f"{self.base_url}/rest/v1/equity/value-order/min-max",
-            headers=self.headers,
-            params=params
-        )
-        return json.loads(response.content.decode("utf-8"))
-
-
-class CFD(Trading212):
-    """ Trading 212 CFD """
-
-    def __init__(self, email: str, password: str, driver: webdriver, mode: constants.Mode = constants.Mode.DEMO):
-        super().__init__(email, password, driver, mode, constants.Trading.CFD)
-
-    def execute_order(self, order: CFDOrder):
-        """Execute CFD order"""
-
-        # Check if it is Limit Stop Order
-        if hasattr(order, 'is_limit_stop') and order.is_limit_stop == True:
-            url = f"{self.base_url}/rest/v2/pending-orders/entry-dep-limit-stop/{order.instrument_code}"
-        # Check if it is OCO Order
-        elif hasattr(order, 'is_oco') and order.is_oco == True:
-            url = f"{self.base_url}/rest/v2/pending-orders/entry-oco/{order.instrument_code}"
-        # Market Order
-        else:
-            url = f"{self.base_url}/rest/v2/trading/open-positions"
-
-        response = requests.post(
-            url=url,
-            headers=self.headers,
-            data=order.to_json(),
-        )
-        return json.loads(response.content.decode("utf-8"))
-
-    def trading_additional_info(self, order: CFDOrder):
-        """Get additional trading info before executing order."""
-        params = {'instrumentCode': order.instrument_code,
-                  'quantity': order.quantity,
-                  'positionId': 'null'}
-        response = requests.get(
-            f"{self.base_url}/rest/v1/tradingAdditionalInfo",
-            headers=self.headers,
-            params=params
-        )
-        return json.loads(response.content.decode("utf-8"))
-
-    def close_position(self, position_id):
-        """Close an open position."""
-        response = requests.delete(
-            url=f"{self.base_url}/rest/v2/trading/open-positions/close/{position_id}",
-            headers=self.headers,
-        )
-        return json.loads(response.content.decode("utf-8"))
-
-    def get_current_price(self, instrument_code):
-        """Workaround to get the current price of a CFD."""
-        # Simulate an order with target price 0, T212 will respond with a business exception so we can get the
-        # current price
-        cfd_order = CFDOrder(instrument_code=instrument_code,
-                             target_price=0.0,
-                             quantity=0.1)
-        # Return only the current price
-        return float(self.execute_order(cfd_order)['context']['current'])
+"""API for Trading212 Platform"""
+
+import json
+import logging
+import re
+import time
+from datetime import datetime
+from time import strftime
+from urllib.parse import urlencode
+
+import requests
+from selenium import webdriver
+from selenium.common.exceptions import NoSuchElementException
+from selenium.webdriver.common.by import By
+from selenium.webdriver.support import expected_conditions
+from selenium.webdriver.support.ui import WebDriverWait
+
+from pytrading212 import constants, console
+from pytrading212.instrument import CFDInstrument
+from pytrading212.order import CFDOrder, EquityOrder
+from pytrading212.position import Position
+
+
+class Trading212:
+    def __init__(
+            self,
+            email: str,
+            password: str,
+            driver: webdriver,
+            mode: constants.Mode = constants.Mode.DEMO,
+            trading: constants.Trading = constants.Trading.EQUITY,
+    ):
+        self.session = f"TRADING212_SESSION_{mode.name}"
+        self.base_url = f"https://{mode.name.lower()}.trading212.com"
+
+        console.log(f"Starting PyTrading212 v{constants.PYTRADING212_VERSION}\n"
+                    f"Trading: [green]{trading.name}[/green] \n"
+                    f"Mode: [green]{mode.name}[/green]")
+
+        self.driver = driver
+        self.driver.get(constants.URL_LOGIN)
+
+        # Click Accept all cookies if it appears
+        try:
+            console.log("Closing 'Cookies Popup'")
+            self.driver.find_element(By.CLASS_NAME, constants.CLASS_COOKIES_NOTICE_BUTTON).click()
+        except NoSuchElementException:
+            pass  # ignore
+
+        console.log("Authenticating")
+
+        WebDriverWait(self.driver, 120).until(expected_conditions.visibility_of_element_located((By.NAME, "email")))
+
+        # Authenticate
+        self.driver.find_element(By.NAME, "email").send_keys(email)
+        self.driver.find_element(By.NAME, "password").send_keys(password)
+
+        # Click login button
+        self.driver.find_element(By.CLASS_NAME, constants.CLASS_LOGIN_BUTTON).click()
+
+        # Close new app button, should be removed later
+        try:
+            WebDriverWait(self.driver, 30).until(expected_conditions.visibility_of_element_located(
+                (By.CSS_SELECTOR, constants.SELECTOR_NEW_APP)))
+            self.driver.find_element(By.CSS_SELECTOR, constants.SELECTOR_NEW_APP).click()
+        except NoSuchElementException:
+            pass
+
+        self.user_agent = self.driver.execute_script("return navigator.userAgent;")
+
+        # Switch to get also DEMO token
+        self.switch()
+        # Get session cookie
+        cookies = self.driver.get_cookies()
+        if cookies is not None:
+            for cookie in cookies:
+                # Get appropriate cookie for this session, live or demo
+                if self.session in cookie['name']:
+                    self.cookie = f"{self.session}={cookie['value']};"
+        else:
+            raise Exception("Unable to get cookies, aborting.")
+
+        # Necessary headers for requests
+        self.headers = {
+            "Accept": "application/json",
+            "Content-Type": "application/json",
+            "User-Agent": self.user_agent,
+            "Cookie": self.cookie,
+        }
+
+        self.companies = self.get_companies()
+
+    def __enter__(self):
+        return self
+
+    def __exit__(self, exc_type, exc_val, exc_tb):
+        self.finish()
+
+    def finish(self):
+        console.log("Closing session.")
+        self.driver.close()
+
+    def switch(self):
+        WebDriverWait(self.driver, 30).until(expected_conditions.visibility_of_element_located(
+            (By.CSS_SELECTOR, constants.SELECTOR_MENU_BUTTON)))
+        self.driver.find_element(By.CSS_SELECTOR, constants.SELECTOR_MENU_BUTTON).click()
+
+        self.driver.execute_script("arguments[0].scroll(0, arguments[0].scrollHeight);",
+                                   self.driver.find_element(By.CSS_SELECTOR, constants.SELECTOR_MENU_LIST))
+        self.driver.find_element(By.CSS_SELECTOR, constants.SELECTOR_SWITCH_DEMO).click()
+        WebDriverWait(self.driver, 30).until(expected_conditions.visibility_of_element_located(
+            (By.CSS_SELECTOR, constants.SELECTOR_DEMO_EQUITY)))
+        self.driver.find_element(By.CSS_SELECTOR, constants.SELECTOR_DEMO_EQUITY).click()
+        # Wait some seconds to initialize cookies
+        time.sleep(5)
+
+    def get_funds(self):
+        """Get your funds, free, available."""
+        response = requests.get(
+            f"{self.base_url}/rest/v2/customer/accounts/funds", headers=self.headers
+        )
+        return json.loads(response.content.decode("utf-8"))
+
+    def last_hour_hotlist(self):
+        """Trading 212 last hour hotlist"""
+        response = requests.get(
+            f"{self.base_url}/trading212.com/rest/positions-tracker/deltas/hourly/1"
+        )
+        return json.loads(response.content.decode("utf-8"))
+
+    def get_orders(self, older_than: datetime, newer_than: datetime):
+        """Get orders within a range of dates"""
+        params = {
+            'olderThan': strftime(older_than.isoformat()),
+            'newerThan': strftime(newer_than.isoformat())
+        }
+
+        response = requests.get(
+            f"{self.base_url}/rest/history/orders", headers=self.headers, params=urlencode(params)
+        )
+        return json.loads(response.content.decode("utf-8"))
+
+    def get_transactions(self, older_than: datetime, newer_than: datetime):
+        """Get transactions within a range of dates"""
+        params = {
+            'olderThan': strftime(older_than.isoformat()),
+            'newerThan': strftime(newer_than.isoformat())
+        }
+        response = requests.get(
+            f"{self.base_url}/rest/history/transactions", headers=self.headers, params=urlencode(params)
+        )
+        return json.loads(response.content.decode("utf-8"))
+
+    def get_order_details(self, details_path):
+        """Get Order Details"""
+        response = requests.get(f"{self.base_url}/rest/history{details_path}", headers=self.headers)
+        return json.loads(response.content.decode("utf-8"))
+
+    def get_dividends(self, older_than: datetime, newer_than: datetime):
+        """Get dividends within a range of dates"""
+        params = {'olderThan': strftime(older_than.isoformat()),
+                  'newerThan': strftime(newer_than.isoformat())
+                  }
+
+        response = requests.get(
+            f"{self.base_url}/rest/history/dividends", headers=self.headers, params=urlencode(params)
+        )
+        return json.loads(response.content.decode("utf-8"))
+
+    def get_fundamentals(self, ticker, language_code: str = "en"):
+        """Get fundamentals of a company by its isin"""
+        params = {'ticker': ticker,
+                  'languageCode': language_code
+                  }
+
+        response = requests.get(f"{self.base_url}/rest/companies/v2/fundamentals",
+                                params=params)
+        return json.loads(response.content.decode("utf-8"))
+
+    def get_portfolio_performance(self, time_period: constants.Period):
+        """Get Portfolio Performance"""
+        response = requests.get(
+            url=f"{self.base_url}/rest/v2/portfolio?period={time_period}",
+            headers=self.headers,
+        )
+        return json.loads(response.content.decode("utf-8"))
+
+    def get_portfolio_composition(self):
+        """Get Portfolio Composition"""
+        # click portfolio section on right-sidepanel
+        right_sidepanel_portfolio_class = 'portfolio-icon'
+        condition = expected_conditions.visibility_of_element_located(
+            (By.CLASS_NAME, right_sidepanel_portfolio_class)
+        )
+        WebDriverWait(self.driver, 30).until(condition)
+        self.driver.find_element(By.CLASS_NAME, right_sidepanel_portfolio_class).click()
+
+        positions = []
+        try:
+            # click on investments
+            self.driver.find_element(By.CLASS_NAME, 'investment-tab').click()
+            for item in self.driver.find_elements(By.CLASS_NAME, "investment-item"):
+                ticker = item.get_attribute("data-qa-item")
+                value = item.find_element(By.CLASS_NAME, "total-value").text
+                quantity = item.find_element(By.CLASS_NAME, "quantity").text
+                total_return = item.find_element(By.CLASS_NAME, "return").text
+                position = Position(ticker, value, quantity, total_return)
+                positions.append(position.__dict__)
+        except Exception as e:
+            logging.error(e)  # portfolio is empty
+        return positions
+
+    def get_companies(self):
+        """Get Ticker of all Trading212 tradable companies"""
+        response = requests.get(
+            url=f"{self.base_url}/rest/companies",
+            headers=self.headers
+        )
+        return json.loads(response.content.decode("utf-8"))
+
+    def search(self, query):
+        """Search a company"""
+        found = []
+        companies = self.get_companies()
+        for company in companies:
+            if query in company["ticker"]:
+                found.append(company["ticker"])
+
+        response = requests.post(
+            f"{self.base_url}/charting/prices?withFakes=false",
+            headers=self.headers,
+            data=found.__str__().replace("'", '"'),
+        )  # ' with " for Trading212 compatibility
+        return json.loads(response.content.decode("utf-8"))
+
+
+class Equity(Trading212):
+    """Trading 212 Equity"""
+
+    def __init__(self, email: str, password: str, driver: webdriver, mode: constants.Mode = constants.Mode.DEMO):
+        super().__init__(email, password, driver, mode, constants.Trading.EQUITY)
+
+    def review_order(self, order: EquityOrder):
+        """Preview of the order, with added costs and other useful data"""
+        # Check if it is a 'value' order or a 'quantity' order
+        if hasattr(order, 'value'):
+            url = f"{self.base_url}/rest/v1/equity/value-order/review"
+        else:
+            url = f"{self.base_url}/rest/public/added-costs"
+        response = requests.post(
+            url=url,
+            headers=self.headers,
+            data=order.to_json(),
+        )
+        return json.loads(response.content.decode("utf-8"))
+
+    def execute_order(self, order: EquityOrder):
+        """Execute equity order"""
+        # Check if it is a 'value' order or a 'quantity' order
+        if hasattr(order, 'value'):
+            url = f"{self.base_url}/rest/v1/equity/value-order"
+        else:
+            url = f"{self.base_url}/rest/public/v2/equity/order"
+        response = requests.post(
+            url=url,
+            headers=self.headers,
+            data=order.to_json(),
+        )
+        return json.loads(response.content.decode("utf-8"))
+
+    def cancel_order(self, order_id):
+        """Cancel a pending order"""
+        response = requests.delete(
+            url=f"{self.base_url}/rest/public/v2/equity/order/{order_id}",
+            headers=self.headers,
+        )
+        return json.loads(response.content.decode("utf-8"))
+
+    def check_order(self, equity_order: EquityOrder) -> [bool, str]:
+        """Check if Order is valid."""
+        is_valid_ticker = False, f"Instrument Code {equity_order.instrument_code} is not a valid Trading212 Ticker"
+        for company in self.get_companies():
+            if company['ticker'] == equity_order.instrument_code:
+                is_valid_ticker = True, f"Instrument Code {equity_order.instrument_code} is valid Trading212 Ticker"
+
+        return is_valid_ticker
+
+    def min_max_sell_buy(self, instrument_code: str):
+        params = {'instrumentCode': instrument_code}
+        response = requests.get(
+            f"{self.base_url}/rest/v1/equity/value-order/min-max",
+            headers=self.headers,
+            params=params
+        )
+        return json.loads(response.content.decode("utf-8"))
+
+
+class CFD(Trading212):
+    """ Trading 212 CFD """
+
+    def __init__(self, email: str, password: str, driver: webdriver, mode: constants.Mode = constants.Mode.DEMO):
+        super().__init__(email, password, driver, mode, constants.Trading.CFD)
+
+    def execute_order(self, order: CFDOrder):
+        """Execute CFD order"""
+
+        # Check if it is Limit Stop Order
+        if hasattr(order, 'is_limit_stop') and order.is_limit_stop == True:
+            url = f"{self.base_url}/rest/v2/pending-orders/entry-dep-limit-stop/{order.instrument_code}"
+        # Check if it is OCO Order
+        elif hasattr(order, 'is_oco') and order.is_oco == True:
+            url = f"{self.base_url}/rest/v2/pending-orders/entry-oco/{order.instrument_code}"
+        # Market Order
+        else:
+            url = f"{self.base_url}/rest/v2/trading/open-positions"
+
+        response = requests.post(
+            url=url,
+            headers=self.headers,
+            data=order.to_json(),
+        )
+        return json.loads(response.content.decode("utf-8"))
+
+    def trading_additional_info(self, order: CFDOrder):
+        """Get additional trading info before executing order."""
+        params = {'instrumentCode': order.instrument_code,
+                  'quantity': order.quantity,
+                  'positionId': 'null'}
+        response = requests.get(
+            f"{self.base_url}/rest/v1/tradingAdditionalInfo",
+            headers=self.headers,
+            params=params
+        )
+        return json.loads(response.content.decode("utf-8"))
+
+    def close_position(self, position_id):
+        """Close an open position."""
+        response = requests.delete(
+            url=f"{self.base_url}/rest/v2/trading/open-positions/close/{position_id}",
+            headers=self.headers,
+        )
+        return json.loads(response.content.decode("utf-8"))
+
+    def get_current_price(self, instrument_code):
+        """Workaround to get the current price of a CFD."""
+        # Simulate an order with target price 0, T212 will respond with a business exception so we can get the
+        # current price
+        cfd_order = CFDOrder(instrument_code=instrument_code,
+                             target_price=0.0,
+                             quantity=0.1)
+        # Return only the current price
+        return float(self.execute_order(cfd_order)['context']['current'])
```

