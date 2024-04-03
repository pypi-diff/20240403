# Comparing `tmp/squad-linaro-plugins-1.8.tar.gz` & `tmp/squad-linaro-plugins-1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/squad-linaro-plugins-1.8.tar", last modified: Fri Jun 14 11:05:59 2019, max compression
+gzip compressed data, was "dist/squad-linaro-plugins-1.9.tar", last modified: Tue Jul 16 11:04:25 2019, max compression
```

## Comparing `squad-linaro-plugins-1.8.tar` & `squad-linaro-plugins-1.9.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 milosz    (1000) milosz    (1000)        0 2019-06-14 11:05:59.000000 squad-linaro-plugins-1.8/
--rw-r--r--   0 milosz    (1000) milosz    (1000)      731 2019-06-14 10:14:57.000000 squad-linaro-plugins-1.8/setup.py
-drwxr-xr-x   0 milosz    (1000) milosz    (1000)        0 2019-06-14 11:05:59.000000 squad-linaro-plugins-1.8/test/
--rw-r--r--   0 milosz    (1000) milosz    (1000)     1799 2018-12-12 12:08:16.000000 squad-linaro-plugins-1.8/test/test_ltp.py
--rw-r--r--   0 milosz    (1000) milosz    (1000)    26173 2019-06-14 10:14:54.000000 squad-linaro-plugins-1.8/test/test_tradefed.py
-drwxr-xr-x   0 milosz    (1000) milosz    (1000)        0 2019-06-14 11:05:59.000000 squad-linaro-plugins-1.8/squad_linaro_plugins.egg-info/
--rw-rw-r--   0 milosz    (1000) milosz    (1000)        1 2019-06-14 11:05:59.000000 squad-linaro-plugins-1.8/squad_linaro_plugins.egg-info/dependency_links.txt
--rw-rw-r--   0 milosz    (1000) milosz    (1000)      373 2019-06-14 11:05:59.000000 squad-linaro-plugins-1.8/squad_linaro_plugins.egg-info/SOURCES.txt
--rw-rw-r--   0 milosz    (1000) milosz    (1000)       13 2019-06-14 11:05:59.000000 squad-linaro-plugins-1.8/squad_linaro_plugins.egg-info/top_level.txt
--rw-rw-r--   0 milosz    (1000) milosz    (1000)      499 2019-06-14 11:05:59.000000 squad-linaro-plugins-1.8/squad_linaro_plugins.egg-info/PKG-INFO
--rw-rw-r--   0 milosz    (1000) milosz    (1000)       64 2019-06-14 11:05:59.000000 squad-linaro-plugins-1.8/squad_linaro_plugins.egg-info/entry_points.txt
--rw-rw-r--   0 milosz    (1000) milosz    (1000)       21 2019-06-14 11:05:59.000000 squad-linaro-plugins-1.8/squad_linaro_plugins.egg-info/requires.txt
--rw-r--r--   0 milosz    (1000) milosz    (1000)      499 2019-06-14 11:05:59.000000 squad-linaro-plugins-1.8/PKG-INFO
--rw-r--r--   0 milosz    (1000) milosz    (1000)       38 2019-06-14 11:05:59.000000 squad-linaro-plugins-1.8/setup.cfg
--rw-rw-r--   0 milosz    (1000) milosz    (1000)       50 2018-01-26 14:45:00.000000 squad-linaro-plugins-1.8/MANIFEST.in
-drwxr-xr-x   0 milosz    (1000) milosz    (1000)        0 2019-06-14 11:05:59.000000 squad-linaro-plugins-1.8/tradefed/
--rw-r--r--   0 milosz    (1000) milosz    (1000)    11149 2019-06-14 10:14:54.000000 squad-linaro-plugins-1.8/tradefed/__init__.py
--rw-r--r--   0 milosz    (1000) milosz    (1000)     1321 2018-12-12 12:08:16.000000 squad-linaro-plugins-1.8/README.rst
-drwxr-xr-x   0 milosz    (1000) milosz    (1000)        0 2019-06-14 11:05:59.000000 squad-linaro-plugins-1.8/ltp/
--rw-rw-r--   0 milosz    (1000) milosz    (1000)      771 2018-11-07 11:20:40.000000 squad-linaro-plugins-1.8/ltp/__init__.py
+drwxr-xr-x   0 milosz    (1000) milosz    (1000)        0 2019-07-16 11:04:25.000000 squad-linaro-plugins-1.9/
+-rw-r--r--   0 milosz    (1000) milosz    (1000)      731 2019-07-16 11:03:12.000000 squad-linaro-plugins-1.9/setup.py
+drwxr-xr-x   0 milosz    (1000) milosz    (1000)        0 2019-07-16 11:04:25.000000 squad-linaro-plugins-1.9/test/
+-rw-r--r--   0 milosz    (1000) milosz    (1000)     1799 2018-12-12 12:08:16.000000 squad-linaro-plugins-1.9/test/test_ltp.py
+-rw-r--r--   0 milosz    (1000) milosz    (1000)    26597 2019-07-16 11:02:33.000000 squad-linaro-plugins-1.9/test/test_tradefed.py
+drwxr-xr-x   0 milosz    (1000) milosz    (1000)        0 2019-07-16 11:04:25.000000 squad-linaro-plugins-1.9/squad_linaro_plugins.egg-info/
+-rw-rw-r--   0 milosz    (1000) milosz    (1000)        1 2019-07-16 11:04:25.000000 squad-linaro-plugins-1.9/squad_linaro_plugins.egg-info/dependency_links.txt
+-rw-rw-r--   0 milosz    (1000) milosz    (1000)      373 2019-07-16 11:04:25.000000 squad-linaro-plugins-1.9/squad_linaro_plugins.egg-info/SOURCES.txt
+-rw-rw-r--   0 milosz    (1000) milosz    (1000)       13 2019-07-16 11:04:25.000000 squad-linaro-plugins-1.9/squad_linaro_plugins.egg-info/top_level.txt
+-rw-rw-r--   0 milosz    (1000) milosz    (1000)      465 2019-07-16 11:04:25.000000 squad-linaro-plugins-1.9/squad_linaro_plugins.egg-info/PKG-INFO
+-rw-rw-r--   0 milosz    (1000) milosz    (1000)       64 2019-07-16 11:04:25.000000 squad-linaro-plugins-1.9/squad_linaro_plugins.egg-info/entry_points.txt
+-rw-rw-r--   0 milosz    (1000) milosz    (1000)       21 2019-07-16 11:04:25.000000 squad-linaro-plugins-1.9/squad_linaro_plugins.egg-info/requires.txt
+-rw-r--r--   0 milosz    (1000) milosz    (1000)      465 2019-07-16 11:04:25.000000 squad-linaro-plugins-1.9/PKG-INFO
+-rw-r--r--   0 milosz    (1000) milosz    (1000)       38 2019-07-16 11:04:25.000000 squad-linaro-plugins-1.9/setup.cfg
+-rw-rw-r--   0 milosz    (1000) milosz    (1000)       50 2018-01-26 14:45:00.000000 squad-linaro-plugins-1.9/MANIFEST.in
+drwxr-xr-x   0 milosz    (1000) milosz    (1000)        0 2019-07-16 11:04:25.000000 squad-linaro-plugins-1.9/tradefed/
+-rw-r--r--   0 milosz    (1000) milosz    (1000)    11352 2019-07-16 11:02:33.000000 squad-linaro-plugins-1.9/tradefed/__init__.py
+-rw-r--r--   0 milosz    (1000) milosz    (1000)     1321 2018-12-12 12:08:16.000000 squad-linaro-plugins-1.9/README.rst
+drwxr-xr-x   0 milosz    (1000) milosz    (1000)        0 2019-07-16 11:04:25.000000 squad-linaro-plugins-1.9/ltp/
+-rw-rw-r--   0 milosz    (1000) milosz    (1000)      771 2018-11-07 11:20:40.000000 squad-linaro-plugins-1.9/ltp/__init__.py
```

### Comparing `squad-linaro-plugins-1.8/setup.py` & `squad-linaro-plugins-1.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name='squad-linaro-plugins',
-    version='1.8',
+    version='1.9',
     author='Milosz Wasilewski',
     author_email='milosz.wasilewski@linaro.org',
     url='https://github.com/linaro/squadplugins',
     packages=['tradefed', 'ltp'],
     entry_points={
         'squad_plugins': [
             'tradefed=tradefed:Tradefed',
```

### Comparing `squad-linaro-plugins-1.8/test/test_ltp.py` & `squad-linaro-plugins-1.9/test/test_ltp.py`

 * *Files identical despite different names*

### Comparing `squad-linaro-plugins-1.8/test/test_tradefed.py` & `squad-linaro-plugins-1.9/test/test_tradefed.py`

 * *Files 1% similar despite different names*

```diff
@@ -672,14 +672,23 @@
         type(test_mock).suite = suite_mock
         name_mock = PropertyMock(return_value="TestCaseBar.test_bar4")
         type(test_mock).name = name_mock
         self.plugin._assign_test_log(StringIO(XML_RESULTS), [test_mock])
         self.assertIn("java.lang.Error", test_mock.log)
         test_mock.save.assert_called_once()
 
+    def test_assign_test_log_no_slash(self):
+        test_mock = Mock()
+        suite_mock = PropertyMock(return_value="cts-lkft.arm64-v8a.module_foo")
+        type(test_mock).suite = suite_mock
+        name_mock = PropertyMock(return_value="TestCaseBar.test_bar4")
+        type(test_mock).name = name_mock
+        self.plugin._assign_test_log(StringIO(XML_RESULTS), [test_mock])
+        test_mock.save.assert_not_called()
+
     def test_assign_test_log_complex_name(self):
         test_mock = Mock()
         suite_mock = PropertyMock(return_value="cts-lkft/arm64-v8a.module_foo/TestCaseBar.first_subname/second_subname.third_subname")
         type(test_mock).suite = suite_mock
         name_mock = PropertyMock(return_value="test_bar5_64bit")
         type(test_mock).name = name_mock
         self.plugin._assign_test_log(StringIO(XML_RESULTS), [test_mock])
```

### Comparing `squad-linaro-plugins-1.8/tradefed/__init__.py` & `squad-linaro-plugins-1.9/tradefed/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -50,14 +50,18 @@
         if tradefed_tree is None:
             return
         buf.seek(0)
         for test in test_list:
             # search in etree for relevant test
             logger.debug("processing %s/%s" % (test.suite, test.name))
             test_suite_name_list = str(test.suite).split("/")
+            if len(test_suite_name_list) <= 1:
+                # assume that test results produced by LAVA
+                # and test-definitions always contain at least one "/"
+                continue
             test_suite_name = test_suite_name_list[1]
             test_suite_abi = None
             if "." in test_suite_name:
                 test_suite_abi, test_suite_name = test_suite_name.split(".")
             test_name_list = test.name.rsplit(".")
             test_name = test_name_list[-1]
             logger.debug("searching for %s log" % test_name)
```

### Comparing `squad-linaro-plugins-1.8/README.rst` & `squad-linaro-plugins-1.9/README.rst`

 * *Files identical despite different names*

### Comparing `squad-linaro-plugins-1.8/ltp/__init__.py` & `squad-linaro-plugins-1.9/ltp/__init__.py`

 * *Files identical despite different names*

