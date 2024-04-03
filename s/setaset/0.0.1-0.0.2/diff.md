# Comparing `tmp/setaset-0.0.1.tar.gz` & `tmp/setaset-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "setaset-0.0.1.tar", last modified: Sun Mar 10 13:52:29 2024, max compression
+gzip compressed data, was "setaset-0.0.2.tar", last modified: Wed Apr  3 13:10:02 2024, max compression
```

## Comparing `setaset-0.0.1.tar` & `setaset-0.0.2.tar`

### file list

```diff
@@ -1,14 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-03-10 13:52:29.122907 setaset-0.0.1/
--rw-rw-rw-   0        0        0     1070 2024-03-09 14:43:26.000000 setaset-0.0.1/LICENSE
--rw-rw-rw-   0        0        0      564 2024-03-10 13:52:29.121891 setaset-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0      157 2024-03-10 13:00:04.000000 setaset-0.0.1/README.md
--rw-rw-rw-   0        0        0      476 2024-03-10 13:52:11.000000 setaset-0.0.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-03-10 13:52:29.122907 setaset-0.0.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-03-10 13:52:29.114065 setaset-0.0.1/src/
--rw-rw-rw-   0        0        0      205 2024-03-03 14:02:25.000000 setaset-0.0.1/src/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-10 13:52:29.120900 setaset-0.0.1/src/setaset.egg-info/
--rw-rw-rw-   0        0        0      564 2024-03-10 13:52:29.000000 setaset-0.0.1/src/setaset.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      201 2024-03-10 13:52:29.000000 setaset-0.0.1/src/setaset.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-10 13:52:29.000000 setaset-0.0.1/src/setaset.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       15 2024-03-10 13:52:29.000000 setaset-0.0.1/src/setaset.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      252 2024-03-10 12:48:58.000000 setaset-0.0.1/src/setop.py
+drwxrwxrwx   0        0        0        0 2024-04-03 13:10:02.906088 setaset-0.0.2/
+-rw-rw-rw-   0        0        0     1070 2024-03-09 14:43:26.000000 setaset-0.0.2/LICENSE
+-rw-rw-rw-   0        0        0      607 2024-04-03 13:10:02.904973 setaset-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0      200 2024-04-03 13:07:58.000000 setaset-0.0.2/README.md
+-rw-rw-rw-   0        0        0      476 2024-04-03 13:04:50.000000 setaset-0.0.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-03 13:10:02.906088 setaset-0.0.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-03 13:10:02.891030 setaset-0.0.2/src/
+drwxrwxrwx   0        0        0        0 2024-04-03 13:10:02.896038 setaset-0.0.2/src/setaset/
+-rw-rw-rw-   0        0        0      205 2024-03-03 14:02:25.000000 setaset-0.0.2/src/setaset/__init__.py
+-rw-rw-rw-   0        0        0      252 2024-03-10 12:48:58.000000 setaset-0.0.2/src/setaset/setop.py
+drwxrwxrwx   0        0        0        0 2024-04-03 13:10:02.903779 setaset-0.0.2/src/setaset.egg-info/
+-rw-rw-rw-   0        0        0      607 2024-04-03 13:10:02.000000 setaset-0.0.2/src/setaset.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      217 2024-04-03 13:10:02.000000 setaset-0.0.2/src/setaset.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-03 13:10:02.000000 setaset-0.0.2/src/setaset.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2024-04-03 13:10:02.000000 setaset-0.0.2/src/setaset.egg-info/top_level.txt
```

### Comparing `setaset-0.0.1/LICENSE` & `setaset-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `setaset-0.0.1/PKG-INFO` & `setaset-0.0.2/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 Metadata-Version: 2.1
 Name: setaset
-Version: 0.0.1
+Version: 0.0.2
 Summary: A set theory package
 Author-email: richardguo <290413564@qq.com>
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Scientific/Engineering :: Mathematics
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 ## Background
 This project is used for testing and research on set theory.
 ## Install
 Simply use pip.
 `$ pip install setaset`
-## License
-[MIT](LICENSE)
+## Change Log
+0.0.1 add a subset function.
+0.0.2 fix a install-bug.
```

### Comparing `setaset-0.0.1/src/setaset.egg-info/PKG-INFO` & `setaset-0.0.2/src/setaset.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 Metadata-Version: 2.1
 Name: setaset
-Version: 0.0.1
+Version: 0.0.2
 Summary: A set theory package
 Author-email: richardguo <290413564@qq.com>
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Scientific/Engineering :: Mathematics
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 ## Background
 This project is used for testing and research on set theory.
 ## Install
 Simply use pip.
 `$ pip install setaset`
-## License
-[MIT](LICENSE)
+## Change Log
+0.0.1 add a subset function.
+0.0.2 fix a install-bug.
```

