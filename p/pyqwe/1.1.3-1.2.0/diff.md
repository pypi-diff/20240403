# Comparing `tmp/pyqwe-1.1.3.tar.gz` & `tmp/pyqwe-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyqwe-1.1.3.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "pyqwe-1.2.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `pyqwe-1.1.3.tar` & `pyqwe-1.2.0.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0       28 2024-03-30 13:38:11.669595 pyqwe-1.1.3/.env.example
--rw-r--r--   0        0        0     1160 2024-03-30 13:38:11.669728 pyqwe-1.1.3/.gitignore
--rw-r--r--   0        0        0     1083 2024-03-29 08:24:35.046180 pyqwe-1.1.3/LICENSE
--rw-r--r--   0        0        0     2897 2024-04-02 10:17:48.240855 pyqwe-1.1.3/README.md
--rw-r--r--   0        0        0      204 2024-03-29 08:35:21.325325 pyqwe-1.1.3/flask_example/module.py
--rw-r--r--   0        0        0      204 2024-03-29 08:42:03.877337 pyqwe-1.1.3/flask_example/package/__init__.py
--rw-r--r--   0        0        0      936 2024-03-30 13:38:11.669969 pyqwe-1.1.3/pyproject.toml
--rw-r--r--   0        0        0     1111 2024-04-02 10:19:09.776543 pyqwe-1.1.3/pyqwe/__init__.py
--rw-r--r--   0        0        0      179 2024-03-30 13:38:11.670188 pyqwe-1.1.3/pyqwe/exceptions.py
--rw-r--r--   0        0        0     3876 2024-04-02 10:10:43.435476 pyqwe-1.1.3/pyqwe/helpers.py
--rw-r--r--   0        0        0      963 2024-04-01 15:43:06.466385 pyqwe-1.1.3/pyqwe/parser.py
--rw-r--r--   0        0        0     3301 1970-01-01 00:00:00.000000 pyqwe-1.1.3/PKG-INFO
+-rw-r--r--   0        0        0       28 2024-03-30 13:38:11.669595 pyqwe-1.2.0/.env.example
+-rw-r--r--   0        0        0     1160 2024-03-30 13:38:11.669728 pyqwe-1.2.0/.gitignore
+-rw-r--r--   0        0        0     1083 2024-03-29 08:24:35.046180 pyqwe-1.2.0/LICENSE
+-rw-r--r--   0        0        0     3010 2024-04-03 09:00:07.846648 pyqwe-1.2.0/README.md
+-rw-r--r--   0        0        0      204 2024-03-29 08:35:21.325325 pyqwe-1.2.0/flask_example/module.py
+-rw-r--r--   0        0        0      204 2024-03-29 08:42:03.877337 pyqwe-1.2.0/flask_example/package/__init__.py
+-rw-r--r--   0        0        0      936 2024-03-30 13:38:11.669969 pyqwe-1.2.0/pyproject.toml
+-rw-r--r--   0        0        0     1672 2024-04-03 09:00:25.131631 pyqwe-1.2.0/pyqwe/__init__.py
+-rw-r--r--   0        0        0      179 2024-03-30 13:38:11.670188 pyqwe-1.2.0/pyqwe/exceptions.py
+-rw-r--r--   0        0        0     3876 2024-04-02 10:10:43.435476 pyqwe-1.2.0/pyqwe/helpers.py
+-rw-r--r--   0        0        0      746 2024-04-03 08:55:46.563722 pyqwe-1.2.0/pyqwe/parser.py
+-rw-r--r--   0        0        0     3414 1970-01-01 00:00:00.000000 pyqwe-1.2.0/PKG-INFO
```

### Comparing `pyqwe-1.1.3/.gitignore` & `pyqwe-1.2.0/.gitignore`

 * *Files identical despite different names*

### Comparing `pyqwe-1.1.3/LICENSE` & `pyqwe-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pyqwe-1.1.3/README.md` & `pyqwe-1.2.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -24,14 +24,20 @@
 
 ```toml
 [tool.pyqwe]
 flask = "flask_app:run"
 say_hello = "*:echo Hello World"
 ```
 
+You will be able to see what commands you have set in the pyproject.toml file by running:
+
+```bash
+pyqwe list
+```
+
 ### Python commands:
 
 For Python, the commands are structured like (package:module):function
 
 #### Package example:
 
 ```text
@@ -97,18 +103,18 @@
 ```toml
 [tool.pyqwe]
 say_hello = "*shell:echo Hello World"
 ```
 
 ### Change the working directory
 
-You can change the working directory of a subprocess by adding the folder 
+You can change the working directory of a subprocess by adding the folder
 within parentheses to the command, `(node_app)` for example.
 
-**The folder must be relative** to the pyproject.toml file. 
+**The folder must be relative** to the pyproject.toml file.
 
 **Absolute paths are not supported**.
 
 **Moving up directories is not supported**, `../node_app` for example.
 
 ```toml
 [tool.pyqwe]
```

### Comparing `pyqwe-1.1.3/pyproject.toml` & `pyqwe-1.2.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pyqwe-1.1.3/pyqwe/helpers.py` & `pyqwe-1.2.0/pyqwe/helpers.py`

 * *Files identical despite different names*

### Comparing `pyqwe-1.1.3/PKG-INFO` & `pyqwe-1.2.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyqwe
-Version: 1.1.3
+Version: 1.2.0
 Summary: Run commands set in the pyproject.toml file
 Author-email: David Carmichael <david@uilix.com>
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: MIT License
 Requires-Dist: pyqwe-extra-dotenv ; extra == "dotenv"
 Project-URL: Source, https://github.com/CheeseCake87/pyqwe
@@ -36,14 +36,20 @@
 
 ```toml
 [tool.pyqwe]
 flask = "flask_app:run"
 say_hello = "*:echo Hello World"
 ```
 
+You will be able to see what commands you have set in the pyproject.toml file by running:
+
+```bash
+pyqwe list
+```
+
 ### Python commands:
 
 For Python, the commands are structured like (package:module):function
 
 #### Package example:
 
 ```text
@@ -109,18 +115,18 @@
 ```toml
 [tool.pyqwe]
 say_hello = "*shell:echo Hello World"
 ```
 
 ### Change the working directory
 
-You can change the working directory of a subprocess by adding the folder 
+You can change the working directory of a subprocess by adding the folder
 within parentheses to the command, `(node_app)` for example.
 
-**The folder must be relative** to the pyproject.toml file. 
+**The folder must be relative** to the pyproject.toml file.
 
 **Absolute paths are not supported**.
 
 **Moving up directories is not supported**, `../node_app` for example.
 
 ```toml
 [tool.pyqwe]
```

