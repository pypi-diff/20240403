# Comparing `tmp/aioopenexchangerates-0.4.8.tar.gz` & `tmp/aioopenexchangerates-0.4.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aioopenexchangerates-0.4.8.tar", max compression
+gzip compressed data, was "aioopenexchangerates-0.4.9.tar", max compression
```

## Comparing `aioopenexchangerates-0.4.8.tar` & `aioopenexchangerates-0.4.9.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0    11346 2024-01-30 00:23:46.576482 aioopenexchangerates-0.4.8/LICENSE
--rw-r--r--   0        0        0     3568 2024-01-30 00:23:46.576482 aioopenexchangerates-0.4.8/README.md
--rw-r--r--   0        0        0     3938 2024-01-30 00:23:47.468494 aioopenexchangerates-0.4.8/pyproject.toml
--rw-r--r--   0        0        0      396 2024-01-30 00:23:47.468494 aioopenexchangerates-0.4.8/src/aioopenexchangerates/__init__.py
--rw-r--r--   0        0        0     2875 2024-01-30 00:23:46.576482 aioopenexchangerates-0.4.8/src/aioopenexchangerates/client.py
--rw-r--r--   0        0        0      483 2024-01-30 00:23:46.576482 aioopenexchangerates-0.4.8/src/aioopenexchangerates/exceptions.py
--rw-r--r--   0        0        0      146 2024-01-30 00:23:46.576482 aioopenexchangerates-0.4.8/src/aioopenexchangerates/main.py
--rw-r--r--   0        0        0      105 2024-01-30 00:23:46.576482 aioopenexchangerates-0.4.8/src/aioopenexchangerates/model/__init__.py
--rw-r--r--   0        0        0      180 2024-01-30 00:23:46.576482 aioopenexchangerates-0.4.8/src/aioopenexchangerates/model/latest.py
--rw-r--r--   0        0        0      323 2024-01-30 00:23:46.576482 aioopenexchangerates-0.4.8/src/aioopenexchangerates/model/response.py
--rw-r--r--   0        0        0        0 2024-01-30 00:23:46.576482 aioopenexchangerates-0.4.8/src/aioopenexchangerates/py.typed
--rw-r--r--   0        0        0     4873 1970-01-01 00:00:00.000000 aioopenexchangerates-0.4.8/PKG-INFO
+-rw-r--r--   0        0        0    11346 2024-04-03 18:42:19.463115 aioopenexchangerates-0.4.9/LICENSE
+-rw-r--r--   0        0        0     3568 2024-04-03 18:42:19.463115 aioopenexchangerates-0.4.9/README.md
+-rw-r--r--   0        0        0     3940 2024-04-03 18:42:21.127146 aioopenexchangerates-0.4.9/pyproject.toml
+-rw-r--r--   0        0        0      396 2024-04-03 18:42:21.127146 aioopenexchangerates-0.4.9/src/aioopenexchangerates/__init__.py
+-rw-r--r--   0        0        0     2875 2024-04-03 18:42:19.463115 aioopenexchangerates-0.4.9/src/aioopenexchangerates/client.py
+-rw-r--r--   0        0        0      483 2024-04-03 18:42:19.463115 aioopenexchangerates-0.4.9/src/aioopenexchangerates/exceptions.py
+-rw-r--r--   0        0        0      146 2024-04-03 18:42:19.463115 aioopenexchangerates-0.4.9/src/aioopenexchangerates/main.py
+-rw-r--r--   0        0        0      105 2024-04-03 18:42:19.467115 aioopenexchangerates-0.4.9/src/aioopenexchangerates/model/__init__.py
+-rw-r--r--   0        0        0      180 2024-04-03 18:42:19.467115 aioopenexchangerates-0.4.9/src/aioopenexchangerates/model/latest.py
+-rw-r--r--   0        0        0      323 2024-04-03 18:42:19.467115 aioopenexchangerates-0.4.9/src/aioopenexchangerates/model/response.py
+-rw-r--r--   0        0        0        0 2024-04-03 18:42:19.467115 aioopenexchangerates-0.4.9/src/aioopenexchangerates/py.typed
+-rw-r--r--   0        0        0     4873 1970-01-01 00:00:00.000000 aioopenexchangerates-0.4.9/PKG-INFO
```

### Comparing `aioopenexchangerates-0.4.8/LICENSE` & `aioopenexchangerates-0.4.9/LICENSE`

 * *Files identical despite different names*

### Comparing `aioopenexchangerates-0.4.8/README.md` & `aioopenexchangerates-0.4.9/README.md`

 * *Files identical despite different names*

### Comparing `aioopenexchangerates-0.4.8/pyproject.toml` & `aioopenexchangerates-0.4.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 license = "Apache Software License 2.0"
 name = "aioopenexchangerates"
 packages = [
   {include = "aioopenexchangerates", from = "src"},
 ]
 readme = "README.md"
 repository = "https://github.com/MartinHjelmare/aioopenexchangerates"
-version = "0.4.8"
+version = "0.4.9"
 
 [tool.poetry.urls]
 "Bug Tracker" = "https://github.com/MartinHjelmare/aioopenexchangerates/issues"
 "Changelog" = "https://github.com/MartinHjelmare/aioopenexchangerates/blob/main/CHANGELOG.md"
 
 [tool.poetry.dependencies]
 aiohttp = "^3.8.4"
@@ -40,15 +40,15 @@
 isort = "^5.10"
 mypy = "^1.0"
 pre-commit = "^3.0.0"
 pylint = "^3.0.0"
 pylint-strict-informational = "^0.1"
 pytest = "^8.0.0"
 pytest-aiohttp = "^1.0.4"
-pytest-cov = "^4.0"
+pytest-cov = "^5.0.0"
 python-semantic-release = "^8.0.0"
 pyupgrade = "^3.0"
 yarl = "^1.7.2"
 
 [tool.poetry.group.docs]
 optional = true
```

### Comparing `aioopenexchangerates-0.4.8/src/aioopenexchangerates/client.py` & `aioopenexchangerates-0.4.9/src/aioopenexchangerates/client.py`

 * *Files identical despite different names*

### Comparing `aioopenexchangerates-0.4.8/PKG-INFO` & `aioopenexchangerates-0.4.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aioopenexchangerates
-Version: 0.4.8
+Version: 0.4.9
 Summary: Fetch rates from openexchangerates with aiohttp.
 Home-page: https://github.com/MartinHjelmare/aioopenexchangerates
 License: Apache Software License 2.0
 Author: Martin Hjelmare
 Author-email: marhje52@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 2 - Pre-Alpha
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: aioopenexchangerates Version: 0.4.8 Summary: Fetch
+Metadata-Version: 2.1 Name: aioopenexchangerates Version: 0.4.9 Summary: Fetch
 rates from openexchangerates with aiohttp. Home-page: https://github.com/
 MartinHjelmare/aioopenexchangerates License: Apache Software License 2.0
 Author: Martin Hjelmare Author-email: marhje52@gmail.com Requires-Python:
 >=3.9,<4.0 Classifier: Development Status :: 2 - Pre-Alpha Classifier: Intended
 Audience :: Developers Classifier: License :: Other/Proprietary License
 Classifier: Natural Language :: English Classifier: Operating System :: OS
 Independent Classifier: Programming Language :: Python :: 3 Classifier:
```

