# Comparing `tmp/selestium-0.2.7.tar.gz` & `tmp/selestium-0.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "selestium-0.2.7.tar", last modified: Tue Apr  2 10:15:38 2024, max compression
+gzip compressed data, was "selestium-0.2.8.tar", last modified: Wed Apr  3 10:58:00 2024, max compression
```

## Comparing `selestium-0.2.7.tar` & `selestium-0.2.8.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 oguz      (1000) oguz      (1000)        0 2024-04-02 10:15:38.226698 selestium-0.2.7/
--rw-r--r--   0 oguz      (1000) oguz      (1000)    35149 2024-03-30 07:47:50.000000 selestium-0.2.7/LICENSE
--rw-r--r--   0 oguz      (1000) oguz      (1000)     3592 2024-04-02 10:15:38.226698 selestium-0.2.7/PKG-INFO
--rw-r--r--   0 oguz      (1000) oguz      (1000)     3269 2024-04-02 07:56:04.000000 selestium-0.2.7/README.md
-drwxr-xr-x   0 oguz      (1000) oguz      (1000)        0 2024-04-02 10:15:38.226698 selestium-0.2.7/Selestium/
--rw-r--r--   0 oguz      (1000) oguz      (1000)      757 2024-03-30 09:49:54.000000 selestium-0.2.7/Selestium/ChromeHandler.py
--rw-r--r--   0 oguz      (1000) oguz      (1000)     2107 2024-03-30 09:56:22.000000 selestium-0.2.7/Selestium/FirefoxHandler.py
--rw-r--r--   0 oguz      (1000) oguz      (1000)      199 2024-04-02 07:54:21.000000 selestium-0.2.7/Selestium/__init__.py
--rw-r--r--   0 oguz      (1000) oguz      (1000)     4695 2024-04-02 10:13:57.000000 selestium-0.2.7/Selestium/selestium.py
-drwxr-xr-x   0 oguz      (1000) oguz      (1000)        0 2024-04-02 10:15:38.226698 selestium-0.2.7/selestium.egg-info/
--rw-r--r--   0 oguz      (1000) oguz      (1000)     3592 2024-04-02 10:15:38.000000 selestium-0.2.7/selestium.egg-info/PKG-INFO
--rw-r--r--   0 oguz      (1000) oguz      (1000)      290 2024-04-02 10:15:38.000000 selestium-0.2.7/selestium.egg-info/SOURCES.txt
--rw-r--r--   0 oguz      (1000) oguz      (1000)        1 2024-04-02 10:15:38.000000 selestium-0.2.7/selestium.egg-info/dependency_links.txt
--rw-r--r--   0 oguz      (1000) oguz      (1000)       33 2024-04-02 10:15:38.000000 selestium-0.2.7/selestium.egg-info/requires.txt
--rw-r--r--   0 oguz      (1000) oguz      (1000)       10 2024-04-02 10:15:38.000000 selestium-0.2.7/selestium.egg-info/top_level.txt
--rw-r--r--   0 oguz      (1000) oguz      (1000)       38 2024-04-02 10:15:38.226698 selestium-0.2.7/setup.cfg
--rw-r--r--   0 oguz      (1000) oguz      (1000)      628 2024-04-02 09:21:08.000000 selestium-0.2.7/setup.py
+drwxr-xr-x   0 oguz      (1000) oguz      (1000)        0 2024-04-03 10:58:00.518317 selestium-0.2.8/
+-rw-r--r--   0 oguz      (1000) oguz      (1000)    35149 2024-03-30 07:47:50.000000 selestium-0.2.8/LICENSE
+-rw-r--r--   0 oguz      (1000) oguz      (1000)     3592 2024-04-03 10:58:00.518317 selestium-0.2.8/PKG-INFO
+-rw-r--r--   0 oguz      (1000) oguz      (1000)     3269 2024-04-02 07:56:04.000000 selestium-0.2.8/README.md
+drwxr-xr-x   0 oguz      (1000) oguz      (1000)        0 2024-04-03 10:58:00.508317 selestium-0.2.8/Selestium/
+-rw-r--r--   0 oguz      (1000) oguz      (1000)      853 2024-04-03 10:10:50.000000 selestium-0.2.8/Selestium/ChromeHandler.py
+-rw-r--r--   0 oguz      (1000) oguz      (1000)     2207 2024-04-03 10:09:54.000000 selestium-0.2.8/Selestium/FirefoxHandler.py
+-rw-r--r--   0 oguz      (1000) oguz      (1000)      199 2024-04-02 07:54:21.000000 selestium-0.2.8/Selestium/__init__.py
+-rw-r--r--   0 oguz      (1000) oguz      (1000)     4727 2024-04-03 10:08:28.000000 selestium-0.2.8/Selestium/selestium.py
+drwxr-xr-x   0 oguz      (1000) oguz      (1000)        0 2024-04-03 10:58:00.518317 selestium-0.2.8/selestium.egg-info/
+-rw-r--r--   0 oguz      (1000) oguz      (1000)     3592 2024-04-03 10:58:00.000000 selestium-0.2.8/selestium.egg-info/PKG-INFO
+-rw-r--r--   0 oguz      (1000) oguz      (1000)      290 2024-04-03 10:58:00.000000 selestium-0.2.8/selestium.egg-info/SOURCES.txt
+-rw-r--r--   0 oguz      (1000) oguz      (1000)        1 2024-04-03 10:58:00.000000 selestium-0.2.8/selestium.egg-info/dependency_links.txt
+-rw-r--r--   0 oguz      (1000) oguz      (1000)       33 2024-04-03 10:58:00.000000 selestium-0.2.8/selestium.egg-info/requires.txt
+-rw-r--r--   0 oguz      (1000) oguz      (1000)       10 2024-04-03 10:58:00.000000 selestium-0.2.8/selestium.egg-info/top_level.txt
+-rw-r--r--   0 oguz      (1000) oguz      (1000)       38 2024-04-03 10:58:00.518317 selestium-0.2.8/setup.cfg
+-rw-r--r--   0 oguz      (1000) oguz      (1000)      628 2024-04-03 10:56:46.000000 selestium-0.2.8/setup.py
```

### Comparing `selestium-0.2.7/LICENSE` & `selestium-0.2.8/LICENSE`

 * *Files identical despite different names*

### Comparing `selestium-0.2.7/PKG-INFO` & `selestium-0.2.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: selestium
-Version: 0.2.7
+Version: 0.2.8
 Summary: A Python module for web scraping with Selenium and BeautifulSoup
 Home-page: https://github.com/09u2h4n/selestium
 Author: Oğuzhan Yılmaz
 License: UNKNOWN
 Platform: UNKNOWN
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `selestium-0.2.7/README.md` & `selestium-0.2.8/README.md`

 * *Files identical despite different names*

### Comparing `selestium-0.2.7/Selestium/ChromeHandler.py` & `selestium-0.2.8/Selestium/ChromeHandler.py`

 * *Files 10% similar despite different names*

```diff
@@ -10,19 +10,21 @@
     Attributes:
         None
     """
 
     def __init__(self) -> None:
         pass
 
-    def initialize_driver(self):
+    def initialize_driver(self, headless=True, disable_gpu=True, **kwargs):
         """
         Initializes a WebDriver instance for Chrome with headless mode enabled.
 
         Returns:
             WebDriver: The initialized WebDriver instance.
         """
         options = ChromeOptions()
-        options.add_argument("--headless")
-        options.add_argument("--disable-gpu")
+        if headless:
+            options.add_argument("--headless")
+        if disable_gpu:
+            options.add_argument("--disable-gpu")
         driver = webdriver.Chrome(options=options)
         return driver
```

### Comparing `selestium-0.2.7/Selestium/FirefoxHandler.py` & `selestium-0.2.8/Selestium/FirefoxHandler.py`

 * *Files 3% similar despite different names*

```diff
@@ -41,25 +41,27 @@
         paths = os.environ.get('PATH', '').split(os.pathsep)
         for path in paths:
             full_path = os.path.join(path, "geckodriver")
             if os.path.exists(full_path) and os.access(full_path, os.X_OK):
                 return full_path
         return None
             
-    def initialize_driver(self):
+    def initialize_driver(self, headless=True, disable_gpu=True, **kwargs):
         """
         Initializes a WebDriver instance for Firefox with headless mode enabled.
 
         Returns:
             WebDriver: The initialized WebDriver instance.
         """
         options = FirefoxOptions()
-        options.add_argument("--headless")
-        options.add_argument("--disable-gpu")
+        if headless:
+            options.add_argument("--headless")
+        if disable_gpu:
+            options.add_argument("--disable-gpu")
         detected_os = self.detect_os()
-        geckodriver_path = self.detect_geckodriver()
         if detected_os == "Android":
+            geckodriver_path = self.detect_geckodriver()
             service = FirefoxService(executable_path=geckodriver_path)
             driver = webdriver.Firefox(options=options, service=service)
         else:
             driver = webdriver.Firefox(options=options)
         return driver
```

### Comparing `selestium-0.2.7/Selestium/selestium.py` & `selestium-0.2.8/Selestium/selestium.py`

 * *Files 2% similar despite different names*

```diff
@@ -71,23 +71,23 @@
         self.driver.get(url)
         html_content = self.driver.page_source
         response = HTMLResponse(html_content)
         # Close the WebDriver after rendering
         self.driver.quit()
         return response
 
-    def browser_controller(self):
+    def browser_controller(self, headless=True):
         """
         Returns the browser controller (WebDriver) instance.
 
         Returns:
             WebDriver: The browser controller instance.
         """
         if not self.driver:
-            self.driver = self.handler.initialize_driver()
+            self.driver = self.handler.initialize_driver(headless=headless)
         return self.driver
 
 class HTMLResponse:
     """
     A class representing an HTML response.
 
     Args:
```

### Comparing `selestium-0.2.7/selestium.egg-info/PKG-INFO` & `selestium-0.2.8/selestium.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: selestium
-Version: 0.2.7
+Version: 0.2.8
 Summary: A Python module for web scraping with Selenium and BeautifulSoup
 Home-page: https://github.com/09u2h4n/selestium
 Author: Oğuzhan Yılmaz
 License: UNKNOWN
 Platform: UNKNOWN
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `selestium-0.2.7/setup.py` & `selestium-0.2.8/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 # Read the contents of the README file
 with open('README.md', 'r', encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='selestium',
-    version='0.2.7',
+    version='0.2.8',
     description='A Python module for web scraping with Selenium and BeautifulSoup',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author='Oğuzhan Yılmaz',
     url='https://github.com/09u2h4n/selestium',
     packages=find_packages(),
     install_requires=[
```

