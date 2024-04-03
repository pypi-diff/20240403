# Comparing `tmp/statecraft-0.1.0.tar.gz` & `tmp/statecraft-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "statecraft-0.1.0.tar", last modified: Wed Apr  3 11:03:47 2024, max compression
+gzip compressed data, was "statecraft-0.1.1.tar", last modified: Wed Apr  3 11:28:06 2024, max compression
```

## Comparing `statecraft-0.1.0.tar` & `statecraft-0.1.1.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 Kola       (501) staff       (20)        0 2024-04-03 11:03:47.857451 statecraft-0.1.0/
--rw-r--r--   0 Kola       (501) staff       (20)    11358 2024-04-03 11:02:42.000000 statecraft-0.1.0/LICENSE
--rw-r--r--   0 Kola       (501) staff       (20)       76 2024-04-03 11:03:47.857195 statecraft-0.1.0/PKG-INFO
--rw-r--r--   0 Kola       (501) staff       (20)     3207 2024-04-03 10:35:56.000000 statecraft-0.1.0/README.md
--rw-r--r--   0 Kola       (501) staff       (20)      900 2024-04-03 10:50:57.000000 statecraft-0.1.0/pyproject.toml
--rw-r--r--   0 Kola       (501) staff       (20)       38 2024-04-03 11:03:47.857540 statecraft-0.1.0/setup.cfg
--rw-r--r--   0 Kola       (501) staff       (20)      153 2024-04-03 10:56:40.000000 statecraft-0.1.0/setup.py
-drwxr-xr-x   0 Kola       (501) staff       (20)        0 2024-04-03 11:03:47.851081 statecraft-0.1.0/statecraft/
--rw-r--r--   0 Kola       (501) staff       (20)      236 2024-04-03 10:36:07.000000 statecraft-0.1.0/statecraft/__init__.py
--rw-r--r--   0 Kola       (501) staff       (20)      849 2024-03-27 00:09:23.000000 statecraft-0.1.0/statecraft/_setup.py
--rw-r--r--   0 Kola       (501) staff       (20)     4148 2024-04-03 10:38:43.000000 statecraft-0.1.0/statecraft/client.py
--rw-r--r--   0 Kola       (501) staff       (20)    10281 2024-04-03 10:43:20.000000 statecraft-0.1.0/statecraft/core.py
--rw-r--r--   0 Kola       (501) staff       (20)      287 2024-03-26 13:46:51.000000 statecraft-0.1.0/statecraft/metadata.py
--rw-r--r--   0 Kola       (501) staff       (20)      368 2024-03-26 15:52:01.000000 statecraft-0.1.0/statecraft/models.py
--rw-r--r--   0 Kola       (501) staff       (20)     1682 2024-04-03 10:35:22.000000 statecraft-0.1.0/statecraft/states_list.py
--rw-r--r--   0 Kola       (501) staff       (20)      195 2024-03-27 00:03:59.000000 statecraft-0.1.0/statecraft/user_attributes.py
--rw-r--r--   0 Kola       (501) staff       (20)      398 2024-03-26 15:06:22.000000 statecraft-0.1.0/statecraft/utils.py
-drwxr-xr-x   0 Kola       (501) staff       (20)        0 2024-04-03 11:03:47.856751 statecraft-0.1.0/statecraft.egg-info/
--rw-r--r--   0 Kola       (501) staff       (20)       76 2024-04-03 11:03:47.000000 statecraft-0.1.0/statecraft.egg-info/PKG-INFO
--rw-r--r--   0 Kola       (501) staff       (20)      381 2024-04-03 11:03:47.000000 statecraft-0.1.0/statecraft.egg-info/SOURCES.txt
--rw-r--r--   0 Kola       (501) staff       (20)        1 2024-04-03 11:03:47.000000 statecraft-0.1.0/statecraft.egg-info/dependency_links.txt
--rw-r--r--   0 Kola       (501) staff       (20)       11 2024-04-03 11:03:47.000000 statecraft-0.1.0/statecraft.egg-info/top_level.txt
+drwxr-xr-x   0 Kola       (501) staff       (20)        0 2024-04-03 11:28:06.848269 statecraft-0.1.1/
+-rw-r--r--   0 Kola       (501) staff       (20)    11358 2024-04-03 11:02:42.000000 statecraft-0.1.1/LICENSE
+-rw-r--r--   0 Kola       (501) staff       (20)     3324 2024-04-03 11:28:06.848023 statecraft-0.1.1/PKG-INFO
+-rw-r--r--   0 Kola       (501) staff       (20)     3207 2024-04-03 10:35:56.000000 statecraft-0.1.1/README.md
+-rw-r--r--   0 Kola       (501) staff       (20)      983 2024-04-03 11:21:45.000000 statecraft-0.1.1/pyproject.toml
+-rw-r--r--   0 Kola       (501) staff       (20)       38 2024-04-03 11:28:06.848354 statecraft-0.1.1/setup.cfg
+-rw-r--r--   0 Kola       (501) staff       (20)      371 2024-04-03 11:26:47.000000 statecraft-0.1.1/setup.py
+drwxr-xr-x   0 Kola       (501) staff       (20)        0 2024-04-03 11:28:06.846545 statecraft-0.1.1/statecraft/
+-rw-r--r--   0 Kola       (501) staff       (20)      236 2024-04-03 10:36:07.000000 statecraft-0.1.1/statecraft/__init__.py
+-rw-r--r--   0 Kola       (501) staff       (20)      849 2024-03-27 00:09:23.000000 statecraft-0.1.1/statecraft/_setup.py
+-rw-r--r--   0 Kola       (501) staff       (20)     4148 2024-04-03 10:38:43.000000 statecraft-0.1.1/statecraft/client.py
+-rw-r--r--   0 Kola       (501) staff       (20)    10281 2024-04-03 10:43:20.000000 statecraft-0.1.1/statecraft/core.py
+-rw-r--r--   0 Kola       (501) staff       (20)      287 2024-03-26 13:46:51.000000 statecraft-0.1.1/statecraft/metadata.py
+-rw-r--r--   0 Kola       (501) staff       (20)      368 2024-03-26 15:52:01.000000 statecraft-0.1.1/statecraft/models.py
+-rw-r--r--   0 Kola       (501) staff       (20)     1682 2024-04-03 10:35:22.000000 statecraft-0.1.1/statecraft/states_list.py
+-rw-r--r--   0 Kola       (501) staff       (20)      195 2024-03-27 00:03:59.000000 statecraft-0.1.1/statecraft/user_attributes.py
+-rw-r--r--   0 Kola       (501) staff       (20)      398 2024-03-26 15:06:22.000000 statecraft-0.1.1/statecraft/utils.py
+drwxr-xr-x   0 Kola       (501) staff       (20)        0 2024-04-03 11:28:06.847702 statecraft-0.1.1/statecraft.egg-info/
+-rw-r--r--   0 Kola       (501) staff       (20)     3324 2024-04-03 11:28:06.000000 statecraft-0.1.1/statecraft.egg-info/PKG-INFO
+-rw-r--r--   0 Kola       (501) staff       (20)      381 2024-04-03 11:28:06.000000 statecraft-0.1.1/statecraft.egg-info/SOURCES.txt
+-rw-r--r--   0 Kola       (501) staff       (20)        1 2024-04-03 11:28:06.000000 statecraft-0.1.1/statecraft.egg-info/dependency_links.txt
+-rw-r--r--   0 Kola       (501) staff       (20)       11 2024-04-03 11:28:06.000000 statecraft-0.1.1/statecraft.egg-info/top_level.txt
```

### Comparing `statecraft-0.1.0/LICENSE` & `statecraft-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `statecraft-0.1.0/README.md` & `statecraft-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `statecraft-0.1.0/pyproject.toml` & `statecraft-0.1.1/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -3,27 +3,30 @@
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "statecraft"
 version = "0.1.0"
 description = "Store, manage and remix states for SSMs and other Stateful models"
 authors = ["koayon <koayon@gmail.com>"]
-license = "MIT"
+license = "Apache-2.0"
 readme = "README.md"
 packages = [{include = "statecraft"}]
 requires-python = ">=3.8"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
     "Development Status :: 4 - Beta",
     "Intended Audience :: Developers",
     "Typing :: Typed",
 ]
 
+[tool.poetry.urls]
+Repository = "https://github.com/koayon/statecraft.git"
+
 [tool.poetry.dependencies]
 python = "^3.10"
 python-dotenv = "^0.19.1"
 responses = "^0.13.4"
 torch = "2.1.2"
 transformers = "4.40.0.dev0"
 pydantic = "2.5.3"
```

### Comparing `statecraft-0.1.0/statecraft/_setup.py` & `statecraft-0.1.1/statecraft/_setup.py`

 * *Files identical despite different names*

### Comparing `statecraft-0.1.0/statecraft/client.py` & `statecraft-0.1.1/statecraft/client.py`

 * *Files identical despite different names*

### Comparing `statecraft-0.1.0/statecraft/core.py` & `statecraft-0.1.1/statecraft/core.py`

 * *Files identical despite different names*

### Comparing `statecraft-0.1.0/statecraft/states_list.py` & `statecraft-0.1.1/statecraft/states_list.py`

 * *Files identical despite different names*

