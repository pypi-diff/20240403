# Comparing `tmp/repo-ast-builder-0.0.6.tar.gz` & `tmp/repo-ast-builder-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "repo-ast-builder-0.0.6.tar", last modified: Sat Mar 30 11:25:33 2024, max compression
+gzip compressed data, was "repo-ast-builder-0.0.7.tar", last modified: Wed Apr  3 15:30:39 2024, max compression
```

## Comparing `repo-ast-builder-0.0.6.tar` & `repo-ast-builder-0.0.7.tar`

### file list

```diff
@@ -1,21 +1,16 @@
-drwxr-xr-x   0 manuel     (501) staff       (20)        0 2024-03-30 11:25:33.883143 repo-ast-builder-0.0.6/
--rw-r--r--   0 manuel     (501) staff       (20)      816 2024-03-30 11:25:33.882836 repo-ast-builder-0.0.6/PKG-INFO
--rw-r--r--   0 manuel     (501) staff       (20)      264 2024-03-28 20:01:53.000000 repo-ast-builder-0.0.6/README.md
--rw-r--r--   0 manuel     (501) staff       (20)      649 2024-03-30 11:24:07.000000 repo-ast-builder-0.0.6/pyproject.toml
--rw-r--r--   0 manuel     (501) staff       (20)       38 2024-03-30 11:25:33.883196 repo-ast-builder-0.0.6/setup.cfg
-drwxr-xr-x   0 manuel     (501) staff       (20)        0 2024-03-30 11:25:33.875967 repo-ast-builder-0.0.6/src/
-drwxr-xr-x   0 manuel     (501) staff       (20)        0 2024-03-30 11:25:33.879627 repo-ast-builder-0.0.6/src/repo_ast_builder/
--rw-r--r--   0 manuel     (501) staff       (20)      181 2024-03-29 13:39:27.000000 repo-ast-builder-0.0.6/src/repo_ast_builder/__init__.py
--rw-r--r--   0 manuel     (501) staff       (20)      850 2024-03-29 15:48:50.000000 repo-ast-builder-0.0.6/src/repo_ast_builder/file_walking.py
--rw-r--r--   0 manuel     (501) staff       (20)     6020 2024-03-29 16:46:29.000000 repo-ast-builder-0.0.6/src/repo_ast_builder/general_node_walking.py
--rw-r--r--   0 manuel     (501) staff       (20)      650 2024-03-29 13:39:27.000000 repo-ast-builder-0.0.6/src/repo_ast_builder/main.py
--rw-r--r--   0 manuel     (501) staff       (20)      692 2024-03-29 13:39:27.000000 repo-ast-builder-0.0.6/src/repo_ast_builder/name_resolver.py
--rw-r--r--   0 manuel     (501) staff       (20)     3702 2024-03-30 11:24:40.000000 repo-ast-builder-0.0.6/src/repo_ast_builder/node_walking.py
--rw-r--r--   0 manuel     (501) staff       (20)       25 2024-03-28 13:53:49.000000 repo-ast-builder-0.0.6/src/repo_ast_builder/options.py
-drwxr-xr-x   0 manuel     (501) staff       (20)        0 2024-03-30 11:25:33.882105 repo-ast-builder-0.0.6/src/repo_ast_builder.egg-info/
--rw-r--r--   0 manuel     (501) staff       (20)      816 2024-03-30 11:25:33.000000 repo-ast-builder-0.0.6/src/repo_ast_builder.egg-info/PKG-INFO
--rw-r--r--   0 manuel     (501) staff       (20)      541 2024-03-30 11:25:33.000000 repo-ast-builder-0.0.6/src/repo_ast_builder.egg-info/SOURCES.txt
--rw-r--r--   0 manuel     (501) staff       (20)        1 2024-03-30 11:25:33.000000 repo-ast-builder-0.0.6/src/repo_ast_builder.egg-info/dependency_links.txt
--rw-r--r--   0 manuel     (501) staff       (20)       64 2024-03-30 11:25:33.000000 repo-ast-builder-0.0.6/src/repo_ast_builder.egg-info/entry_points.txt
--rw-r--r--   0 manuel     (501) staff       (20)       44 2024-03-30 11:25:33.000000 repo-ast-builder-0.0.6/src/repo_ast_builder.egg-info/requires.txt
--rw-r--r--   0 manuel     (501) staff       (20)       17 2024-03-30 11:25:33.000000 repo-ast-builder-0.0.6/src/repo_ast_builder.egg-info/top_level.txt
+drwxr-xr-x   0 manuel     (501) staff       (20)        0 2024-04-03 15:30:39.934899 repo-ast-builder-0.0.7/
+-rw-r--r--   0 manuel     (501) staff       (20)      846 2024-04-03 15:30:39.934513 repo-ast-builder-0.0.7/PKG-INFO
+-rw-r--r--   0 manuel     (501) staff       (20)      264 2024-03-28 20:01:53.000000 repo-ast-builder-0.0.7/README.md
+-rw-r--r--   0 manuel     (501) staff       (20)      670 2024-04-03 15:29:25.000000 repo-ast-builder-0.0.7/pyproject.toml
+-rw-r--r--   0 manuel     (501) staff       (20)       38 2024-04-03 15:30:39.934974 repo-ast-builder-0.0.7/setup.cfg
+drwxr-xr-x   0 manuel     (501) staff       (20)        0 2024-04-03 15:30:39.928579 repo-ast-builder-0.0.7/src/
+drwxr-xr-x   0 manuel     (501) staff       (20)        0 2024-04-03 15:30:39.929669 repo-ast-builder-0.0.7/src/repo_ast_builder/
+-rw-r--r--   0 manuel     (501) staff       (20)        0 2024-04-03 07:39:04.000000 repo-ast-builder-0.0.7/src/repo_ast_builder/__init__.py
+-rw-r--r--   0 manuel     (501) staff       (20)     2705 2024-04-03 15:26:48.000000 repo-ast-builder-0.0.7/src/repo_ast_builder/main.py
+drwxr-xr-x   0 manuel     (501) staff       (20)        0 2024-04-03 15:30:39.933625 repo-ast-builder-0.0.7/src/repo_ast_builder.egg-info/
+-rw-r--r--   0 manuel     (501) staff       (20)      846 2024-04-03 15:30:39.000000 repo-ast-builder-0.0.7/src/repo_ast_builder.egg-info/PKG-INFO
+-rw-r--r--   0 manuel     (501) staff       (20)      352 2024-04-03 15:30:39.000000 repo-ast-builder-0.0.7/src/repo_ast_builder.egg-info/SOURCES.txt
+-rw-r--r--   0 manuel     (501) staff       (20)        1 2024-04-03 15:30:39.000000 repo-ast-builder-0.0.7/src/repo_ast_builder.egg-info/dependency_links.txt
+-rw-r--r--   0 manuel     (501) staff       (20)       64 2024-04-03 15:30:39.000000 repo-ast-builder-0.0.7/src/repo_ast_builder.egg-info/entry_points.txt
+-rw-r--r--   0 manuel     (501) staff       (20)       59 2024-04-03 15:30:39.000000 repo-ast-builder-0.0.7/src/repo_ast_builder.egg-info/requires.txt
+-rw-r--r--   0 manuel     (501) staff       (20)       17 2024-04-03 15:30:39.000000 repo-ast-builder-0.0.7/src/repo_ast_builder.egg-info/top_level.txt
```

### Comparing `repo-ast-builder-0.0.6/PKG-INFO` & `repo-ast-builder-0.0.7/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 Metadata-Version: 2.1
 Name: repo-ast-builder
-Version: 0.0.6
+Version: 0.0.7
 Summary: Creates an AST of a Python project
 Keywords: ast,python,builder
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
+Requires-Dist: python-scalpel
 Provides-Extra: dev
 Requires-Dist: black; extra == "dev"
 Requires-Dist: bumpver; extra == "dev"
 Requires-Dist: isort; extra == "dev"
 Requires-Dist: pip-tools; extra == "dev"
 Requires-Dist: pytest; extra == "dev"
```

### Comparing `repo-ast-builder-0.0.6/src/repo_ast_builder.egg-info/PKG-INFO` & `repo-ast-builder-0.0.7/src/repo_ast_builder.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 Metadata-Version: 2.1
 Name: repo-ast-builder
-Version: 0.0.6
+Version: 0.0.7
 Summary: Creates an AST of a Python project
 Keywords: ast,python,builder
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
+Requires-Dist: python-scalpel
 Provides-Extra: dev
 Requires-Dist: black; extra == "dev"
 Requires-Dist: bumpver; extra == "dev"
 Requires-Dist: isort; extra == "dev"
 Requires-Dist: pip-tools; extra == "dev"
 Requires-Dist: pytest; extra == "dev"
```

