# Comparing `tmp/goodip-0.0.3.tar.gz` & `tmp/goodip-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "goodip-0.0.3.tar", last modified: Tue Apr  2 15:22:42 2024, max compression
+gzip compressed data, was "goodip-0.0.4.tar", last modified: Wed Apr  3 18:01:42 2024, max compression
```

## Comparing `goodip-0.0.3.tar` & `goodip-0.0.4.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-04-02 15:22:42.661876 goodip-0.0.3/
--rw-rw-rw-   0        0        0     1071 2024-02-01 09:40:20.000000 goodip-0.0.3/LICENSE
--rw-rw-rw-   0        0        0     1046 2024-04-02 15:22:42.657800 goodip-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0      199 2024-04-02 15:21:35.000000 goodip-0.0.3/README.md
-drwxrwxrwx   0        0        0        0 2024-04-02 15:22:42.578878 goodip-0.0.3/goodip/
--rw-rw-rw-   0        0        0      330 2024-04-02 14:25:53.000000 goodip-0.0.3/goodip/__init__.py
--rw-rw-rw-   0        0        0      298 2024-04-02 13:33:13.000000 goodip-0.0.3/goodip/connection_check.py
--rw-rw-rw-   0        0        0     1390 2024-04-02 14:55:21.000000 goodip-0.0.3/goodip/ip.py
-drwxrwxrwx   0        0        0        0 2024-04-02 15:22:42.649713 goodip-0.0.3/goodip.egg-info/
--rw-rw-rw-   0        0        0     1046 2024-04-02 15:22:41.000000 goodip-0.0.3/goodip.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      234 2024-04-02 15:22:42.000000 goodip-0.0.3/goodip.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-02 15:22:41.000000 goodip-0.0.3/goodip.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       33 2024-04-02 15:22:42.000000 goodip-0.0.3/goodip.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2024-04-02 15:22:42.000000 goodip-0.0.3/goodip.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-02 15:22:42.662404 goodip-0.0.3/setup.cfg
--rw-rw-rw-   0        0        0     1017 2024-04-02 15:22:17.000000 goodip-0.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-03 18:01:42.128471 goodip-0.0.4/
+-rw-rw-rw-   0        0        0     1071 2024-02-01 09:40:20.000000 goodip-0.0.4/LICENSE
+-rw-rw-rw-   0        0        0     1058 2024-04-03 18:01:42.118383 goodip-0.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0      211 2024-04-03 17:49:23.000000 goodip-0.0.4/README.md
+drwxrwxrwx   0        0        0        0 2024-04-03 18:01:41.944338 goodip-0.0.4/goodip/
+-rw-rw-rw-   0        0        0      330 2024-04-02 14:25:53.000000 goodip-0.0.4/goodip/__init__.py
+-rw-rw-rw-   0        0        0      298 2024-04-02 13:33:13.000000 goodip-0.0.4/goodip/connection_check.py
+-rw-rw-rw-   0        0        0     1486 2024-04-03 17:51:46.000000 goodip-0.0.4/goodip/ip.py
+drwxrwxrwx   0        0        0        0 2024-04-03 18:01:42.118383 goodip-0.0.4/goodip.egg-info/
+-rw-rw-rw-   0        0        0     1058 2024-04-03 18:01:41.000000 goodip-0.0.4/goodip.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      234 2024-04-03 18:01:41.000000 goodip-0.0.4/goodip.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-03 18:01:41.000000 goodip-0.0.4/goodip.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       33 2024-04-03 18:01:41.000000 goodip-0.0.4/goodip.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2024-04-03 18:01:41.000000 goodip-0.0.4/goodip.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-03 18:01:42.128471 goodip-0.0.4/setup.cfg
+-rw-rw-rw-   0        0        0     1017 2024-04-03 17:45:49.000000 goodip-0.0.4/setup.py
```

### Comparing `goodip-0.0.3/LICENSE` & `goodip-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `goodip-0.0.3/PKG-INFO` & `goodip-0.0.4/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: goodip
-Version: 0.0.3
+Version: 0.0.4
 Summary: you can get your ip address and get its information.
 Home-page: https://github.com/Erfan-Bafandeh/goodip
 Author: Erfan Bafandeh
 Author-email: user.enbh@gmail.com
 Keywords: ip,myip,goodip,checkip
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
@@ -25,14 +25,15 @@
 
 ```python
 from goodip import ip
 
 ip = ip()
 
 ip.ip
+ip.country
 ip.region
 ip.city
 ip.isp
 ip.organization
 ip.network
 ip.usage_type
 ip.timezone
```

### Comparing `goodip-0.0.3/goodip/ip.py` & `goodip-0.0.4/goodip/ip.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,14 +7,15 @@
     def __init__(self):
         if connection_check() == False:
             print("please turn on your internet :|")
             exit()
         response = get("https://browserleaks.com/ip").text
         html = BeautifulSoup(response, "html.parser")
         self.ip = html.find_all("span", {"class":"flag-text wball"})[0].text
+        self.country = html.find_all("tbody")[0].find_all("tr")[4].find_all("td")[1].span.text
         self.region = html.find_all("tbody")[0].find_all("tr")[5].find_all("td")[1].text
         self.city = html.find_all("tbody")[0].find_all("tr")[6].find_all("td")[1].text
         self.isp = html.find_all("tbody")[0].find_all("tr")[7].find_all("td")[1].text
         self.organization = html.find_all("tbody")[0].find_all("tr")[8].find_all("td")[1].text
         self.network = html.find_all("tbody")[0].find_all("tr")[9].find_all("td")[1].text
         self.usage_type = html.find_all("tbody")[0].find_all("tr")[10].find_all("td")[1].text
         self.timezone = html.find_all("tbody")[0].find_all("tr")[11].find_all("td")[1].text
```

### Comparing `goodip-0.0.3/goodip.egg-info/PKG-INFO` & `goodip-0.0.4/goodip.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: goodip
-Version: 0.0.3
+Version: 0.0.4
 Summary: you can get your ip address and get its information.
 Home-page: https://github.com/Erfan-Bafandeh/goodip
 Author: Erfan Bafandeh
 Author-email: user.enbh@gmail.com
 Keywords: ip,myip,goodip,checkip
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
@@ -25,14 +25,15 @@
 
 ```python
 from goodip import ip
 
 ip = ip()
 
 ip.ip
+ip.country
 ip.region
 ip.city
 ip.isp
 ip.organization
 ip.network
 ip.usage_type
 ip.timezone
```

### Comparing `goodip-0.0.3/setup.py` & `goodip-0.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name = 'goodip',
-    version = '0.0.3',
+    version = '0.0.4',
     author= 'Erfan Bafandeh',
     author_email = 'user.enbh@gmail.com',
     description = 'you can get your ip address and get its information.',
     keywords = ['ip', 'myip', 'goodip', 'checkip'],
     long_description = open("README.md", encoding="utf-8").read(),
     python_requires="~=3.6",
     long_description_content_type = 'text/markdown',
```

