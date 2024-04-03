# Comparing `tmp/menu_cli_seb-0.1.5.tar.gz` & `tmp/menu_cli_seb-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "menu_cli_seb-0.1.5.tar", max compression
+gzip compressed data, was "menu_cli_seb-0.1.6.tar", max compression
```

## Comparing `menu_cli_seb-0.1.5.tar` & `menu_cli_seb-0.1.6.tar`

### file list

```diff
@@ -1,6 +1,7 @@
--rw-r--r--   0        0        0        0 2024-04-02 12:54:28.705738 menu_cli_seb-0.1.5/menu_cli_seb/__init__.py
--rw-r--r--   0        0        0       64 2024-04-02 14:40:11.254391 menu_cli_seb-0.1.5/menu_cli_seb/__main__.py
--rw-r--r--   0        0        0     2172 2024-04-02 14:37:59.417085 menu_cli_seb-0.1.5/menu_cli_seb/main.py
--rw-r--r--   0        0        0      426 2024-04-02 14:54:23.854316 menu_cli_seb-0.1.5/pyproject.toml
--rw-r--r--   0        0        0        0 2024-04-02 12:54:28.706738 menu_cli_seb-0.1.5/README.md
--rw-r--r--   0        0        0      425 1970-01-01 00:00:00.000000 menu_cli_seb-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0        0 2024-04-02 12:54:28.705738 menu_cli_seb-0.1.6/menu_cli_seb/__init__.py
+-rw-r--r--   0        0        0       64 2024-04-02 14:40:11.254391 menu_cli_seb-0.1.6/menu_cli_seb/__main__.py
+-rw-r--r--   0        0        0     2580 2024-04-03 13:45:56.018809 menu_cli_seb-0.1.6/menu_cli_seb/main.py
+-rw-r--r--   0        0        0      604 2024-04-03 13:36:56.774302 menu_cli_seb-0.1.6/menu_cli_seb/properties.py
+-rw-r--r--   0        0        0      426 2024-04-03 13:47:32.234971 menu_cli_seb-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-02 12:54:28.706738 menu_cli_seb-0.1.6/README.md
+-rw-r--r--   0        0        0      425 1970-01-01 00:00:00.000000 menu_cli_seb-0.1.6/PKG-INFO
```

### Comparing `menu_cli_seb-0.1.5/menu_cli_seb/main.py` & `menu_cli_seb-0.1.6/menu_cli_seb/main.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,28 +1,38 @@
 from bs4 import BeautifulSoup
 import requests
 import json
 import sys
 from datetime import datetime
+from .properties import set_environment_variable, set_environment_variables
+
+CONFIG_FILE = "config.json"
 
 def main():
     if len(sys.argv) < 2:
         print("Usage: python sebfood [day-week]")
         sys.exit(1)
 
-
+    set_environment_variables()
     argument = sys.argv[1]
 
     print("Argument received:", argument)
     if argument.lower() == 'day':
         print_day()
     elif argument.lower() == 'week':
         print_out_weeks()
-
-
+    elif argument.lower() == 'set':
+        if(len(sys.argv) > 2  ):
+            key = sys.argv[2]
+            value = sys.argv[3]
+            set_environment_variable(key,value)
+        else:
+            print("Use set http_proxy proxies")
+                
+         
 def print_day():
     current_date = datetime.now()
     formatted_date = current_date.strftime("%Y-%m-%d")
   
     bistro , salluhallen = f'https://www.foodandco.se/api/restaurant/menu/day?date={formatted_date}&language=sv&onlyPublishedMenu=true&restaurantPageId=166181' ,f'https://www.foodandco.se/api/restaurant/menu/day?date={formatted_date}&language=sv&onlyPublishedMenu=true&restaurantPageId=197239'
     print("BISTRO")
     bistro_response = requests.get(bistro)
@@ -56,8 +66,7 @@
         print(d.get('DayOfWeek'))
         soup = BeautifulSoup(d.get('Html'), 'html.parser')
         strong_tags = soup.find_all('strong')
         for tag in strong_tags:
             print(tag.get_text(strip=True))
         print("\n")
             
-
```

