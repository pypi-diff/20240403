# Comparing `tmp/requirements_parser-0.8.0.tar.gz` & `tmp/requirements_parser-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "requirements_parser-0.8.0.tar", max compression
+gzip compressed data, was "requirements_parser-0.9.0.tar", max compression
```

## Comparing `requirements_parser-0.8.0.tar` & `requirements_parser-0.9.0.tar`

### file list

```diff
@@ -1,66 +1,70 @@
--rw-r--r--   0        0        0      251 2024-04-03 10:02:11.404471 requirements_parser-0.8.0/AUTHORS.rst
--rw-r--r--   0        0        0    11356 2024-04-03 10:02:11.404471 requirements_parser-0.8.0/LICENSE
--rw-r--r--   0        0        0     1785 2024-04-03 10:02:11.404471 requirements_parser-0.8.0/README.md
--rw-r--r--   0        0        0     3793 2024-04-03 10:02:29.248442 requirements_parser-0.8.0/pyproject.toml
--rw-r--r--   0        0        0      883 2024-04-03 10:02:29.248442 requirements_parser-0.8.0/requirements/__init__.py
--rw-r--r--   0        0        0     2057 2024-04-03 10:02:11.408471 requirements_parser-0.8.0/requirements/fragment.py
--rw-r--r--   0        0        0     3372 2024-04-03 10:02:11.408471 requirements_parser-0.8.0/requirements/parser.py
--rw-r--r--   0        0        0      810 2024-04-03 10:02:11.408471 requirements_parser-0.8.0/requirements/py.typed
--rw-r--r--   0        0        0    10225 2024-04-03 10:02:11.408471 requirements_parser-0.8.0/requirements/requirement.py
--rw-r--r--   0        0        0     1063 2024-04-03 10:02:11.408471 requirements_parser-0.8.0/requirements/vcs.py
--rw-r--r--   0        0        0      657 2024-04-03 10:02:11.408471 requirements_parser-0.8.0/tests/__init__.py
--rw-r--r--   0        0        0        2 2024-04-03 10:02:11.408471 requirements_parser-0.8.0/tests/reqfiles/blank_1.expected
--rw-r--r--   0        0        0        3 2024-04-03 10:02:11.408471 requirements_parser-0.8.0/tests/reqfiles/blank_1.txt
--rw-r--r--   0        0        0        2 2024-04-03 10:02:11.408471 requirements_parser-0.8.0/tests/reqfiles/comment_1.expected
--rw-r--r--   0        0        0       20 2024-04-03 10:02:11.408471 requirements_parser-0.8.0/tests/reqfiles/comment_1.txt
--rw-r--r--   0        0        0      318 2024-04-03 10:02:11.408471 requirements_parser-0.8.0/tests/reqfiles/comment_2.expected
--rw-r--r--   0        0        0       22 2024-04-03 10:02:11.408471 requirements_parser-0.8.0/tests/reqfiles/comment_2.txt
--rw-r--r--   0        0        0    20562 2024-04-03 10:02:11.408471 requirements_parser-0.8.0/tests/reqfiles/crateio_requirements.expected
--rw-r--r--   0        0        0     2885 2024-04-03 10:02:11.408471 requirements_parser-0.8.0/tests/reqfiles/crateio_requirements.txt
--rw-r--r--   0        0        0     1818 2024-04-03 10:02:11.408471 requirements_parser-0.8.0/tests/reqfiles/editable_1.expected
--rw-r--r--   0        0        0      308 2024-04-03 10:02:11.408471 requirements_parser-0.8.0/tests/reqfiles/editable_1.txt
--rw-r--r--   0        0        0     1564 2024-04-03 10:02:11.408471 requirements_parser-0.8.0/tests/reqfiles/editable_2.expected
--rw-r--r--   0        0        0      338 2024-04-03 10:02:11.408471 requirements_parser-0.8.0/tests/reqfiles/editable_2.txt
--rw-r--r--   0        0        0      635 2024-04-03 10:02:11.408471 requirements_parser-0.8.0/tests/reqfiles/extras_1.expected
--rw-r--r--   0        0        0       37 2024-04-03 10:02:11.408471 requirements_parser-0.8.0/tests/reqfiles/extras_1.txt
--rw-r--r--   0        0        0       24 2024-04-03 10:02:11.408471 requirements_parser-0.8.0/tests/reqfiles/fail_1.txt
--rw-r--r--   0        0        0       58 2024-04-03 10:02:11.408471 requirements_parser-0.8.0/tests/reqfiles/fail_2.txt
--rw-r--r--   0        0        0     1339 2024-04-03 10:02:11.408471 requirements_parser-0.8.0/tests/reqfiles/file_1.expected
--rw-r--r--   0        0        0      172 2024-04-03 10:02:11.408471 requirements_parser-0.8.0/tests/reqfiles/file_1.txt
--rw-r--r--   0        0        0      311 2024-04-03 10:02:11.408471 requirements_parser-0.8.0/tests/reqfiles/global_options_requirements.expected
--rw-r--r--   0        0        0      168 2024-04-03 10:02:11.408471 requirements_parser-0.8.0/tests/reqfiles/global_options_requirements.txt
--rw-r--r--   0        0        0     1317 2024-04-03 10:02:11.408471 requirements_parser-0.8.0/tests/reqfiles/illustrative_requirements.expected
--rw-r--r--   0        0        0      121 2024-04-03 10:02:11.408471 requirements_parser-0.8.0/tests/reqfiles/illustrative_requirements.txt
--rw-r--r--   0        0        0      948 2024-04-03 10:02:11.408471 requirements_parser-0.8.0/tests/reqfiles/recursive_1.expected
--rw-r--r--   0        0        0       30 2024-04-03 10:02:11.408471 requirements_parser-0.8.0/tests/reqfiles/recursive_1.txt
--rw-r--r--   0        0        0      595 2024-04-03 10:02:11.408471 requirements_parser-0.8.0/tests/reqfiles/recursive_2.expected
--rw-r--r--   0        0        0       24 2024-04-03 10:02:11.408471 requirements_parser-0.8.0/tests/reqfiles/recursive_2.txt
--rw-r--r--   0        0        0      359 2024-04-03 10:02:11.408471 requirements_parser-0.8.0/tests/reqfiles/recursive_3.expected
--rw-r--r--   0        0        0        4 2024-04-03 10:02:11.408471 requirements_parser-0.8.0/tests/reqfiles/recursive_3.txt
--rw-r--r--   0        0        0     1387 2024-04-03 10:02:11.408471 requirements_parser-0.8.0/tests/reqfiles/rtfd_deploy_requirements.expected
--rw-r--r--   0        0        0     1184 2024-04-03 10:02:11.408471 requirements_parser-0.8.0/tests/reqfiles/rtfd_deploy_requirements.txt
--rw-r--r--   0        0        0    10893 2024-04-03 10:02:11.408471 requirements_parser-0.8.0/tests/reqfiles/rtfd_requirements.expected
--rw-r--r--   0        0        0     2341 2024-04-03 10:02:11.408471 requirements_parser-0.8.0/tests/reqfiles/rtfd_requirements.txt
--rw-r--r--   0        0        0     1242 2024-04-03 10:02:11.408471 requirements_parser-0.8.0/tests/reqfiles/simple_1.expected
--rw-r--r--   0        0        0       65 2024-04-03 10:02:11.408471 requirements_parser-0.8.0/tests/reqfiles/simple_1.txt
--rw-r--r--   0        0        0      408 2024-04-03 10:02:11.408471 requirements_parser-0.8.0/tests/reqfiles/specs_1.expected
--rw-r--r--   0        0        0       43 2024-04-03 10:02:11.408471 requirements_parser-0.8.0/tests/reqfiles/specs_1.txt
--rw-r--r--   0        0        0      759 2024-04-03 10:02:11.408471 requirements_parser-0.8.0/tests/reqfiles/subdirectory.expected
--rw-r--r--   0        0        0      145 2024-04-03 10:02:11.408471 requirements_parser-0.8.0/tests/reqfiles/subdirectory.txt
--rw-r--r--   0        0        0      305 2024-04-03 10:02:11.408471 requirements_parser-0.8.0/tests/reqfiles/underscores.expected
--rw-r--r--   0        0        0        9 2024-04-03 10:02:11.408471 requirements_parser-0.8.0/tests/reqfiles/underscores.txt
--rw-r--r--   0        0        0      926 2024-04-03 10:02:11.408471 requirements_parser-0.8.0/tests/reqfiles/uri.expected
--rw-r--r--   0        0        0      214 2024-04-03 10:02:11.408471 requirements_parser-0.8.0/tests/reqfiles/uri.txt
--rw-r--r--   0        0        0     4479 2024-04-03 10:02:11.408471 requirements_parser-0.8.0/tests/reqfiles/vcs_bzr.expected
--rw-r--r--   0        0        0      751 2024-04-03 10:02:11.408471 requirements_parser-0.8.0/tests/reqfiles/vcs_bzr.txt
--rw-r--r--   0        0        0     4842 2024-04-03 10:02:11.408471 requirements_parser-0.8.0/tests/reqfiles/vcs_git.expected
--rw-r--r--   0        0        0      812 2024-04-03 10:02:11.408471 requirements_parser-0.8.0/tests/reqfiles/vcs_git.txt
--rw-r--r--   0        0        0      397 2024-04-03 10:02:11.408471 requirements_parser-0.8.0/tests/reqfiles/vcs_git_extras_require.expected
--rw-r--r--   0        0        0       73 2024-04-03 10:02:11.408471 requirements_parser-0.8.0/tests/reqfiles/vcs_git_extras_require.txt
--rw-r--r--   0        0        0     5078 2024-04-03 10:02:11.408471 requirements_parser-0.8.0/tests/reqfiles/vcs_hg.expected
--rw-r--r--   0        0        0      814 2024-04-03 10:02:11.408471 requirements_parser-0.8.0/tests/reqfiles/vcs_hg.txt
--rw-r--r--   0        0        0     1502 2024-04-03 10:02:11.408471 requirements_parser-0.8.0/tests/reqfiles/vcs_svn.expected
--rw-r--r--   0        0        0      255 2024-04-03 10:02:11.408471 requirements_parser-0.8.0/tests/reqfiles/vcs_svn.txt
--rw-r--r--   0        0        0     2703 2024-04-03 10:02:11.408471 requirements_parser-0.8.0/tests/test_parser.py
--rw-r--r--   0        0        0     2145 2024-04-03 10:02:11.408471 requirements_parser-0.8.0/tests/test_requirement.py
--rw-r--r--   0        0        0     3245 1970-01-01 00:00:00.000000 requirements_parser-0.8.0/PKG-INFO
+-rw-r--r--   0        0        0      251 2024-04-03 10:27:16.691336 requirements_parser-0.9.0/AUTHORS.rst
+-rw-r--r--   0        0        0    11356 2024-04-03 10:27:16.691336 requirements_parser-0.9.0/LICENSE
+-rw-r--r--   0        0        0     1785 2024-04-03 10:27:16.691336 requirements_parser-0.9.0/README.md
+-rw-r--r--   0        0        0     3793 2024-04-03 10:27:36.383397 requirements_parser-0.9.0/pyproject.toml
+-rw-r--r--   0        0        0      883 2024-04-03 10:27:36.383397 requirements_parser-0.9.0/requirements/__init__.py
+-rw-r--r--   0        0        0     2057 2024-04-03 10:27:16.691336 requirements_parser-0.9.0/requirements/fragment.py
+-rw-r--r--   0        0        0     3484 2024-04-03 10:27:16.691336 requirements_parser-0.9.0/requirements/parser.py
+-rw-r--r--   0        0        0      810 2024-04-03 10:27:16.695336 requirements_parser-0.9.0/requirements/py.typed
+-rw-r--r--   0        0        0    10374 2024-04-03 10:27:16.695336 requirements_parser-0.9.0/requirements/requirement.py
+-rw-r--r--   0        0        0     1063 2024-04-03 10:27:16.695336 requirements_parser-0.9.0/requirements/vcs.py
+-rw-r--r--   0        0        0      657 2024-04-03 10:27:16.695336 requirements_parser-0.9.0/tests/__init__.py
+-rw-r--r--   0        0        0        2 2024-04-03 10:27:16.695336 requirements_parser-0.9.0/tests/reqfiles/blank_1.expected
+-rw-r--r--   0        0        0        3 2024-04-03 10:27:16.695336 requirements_parser-0.9.0/tests/reqfiles/blank_1.txt
+-rw-r--r--   0        0        0        2 2024-04-03 10:27:16.695336 requirements_parser-0.9.0/tests/reqfiles/comment_1.expected
+-rw-r--r--   0        0        0       20 2024-04-03 10:27:16.695336 requirements_parser-0.9.0/tests/reqfiles/comment_1.txt
+-rw-r--r--   0        0        0      318 2024-04-03 10:27:16.695336 requirements_parser-0.9.0/tests/reqfiles/comment_2.expected
+-rw-r--r--   0        0        0       22 2024-04-03 10:27:16.695336 requirements_parser-0.9.0/tests/reqfiles/comment_2.txt
+-rw-r--r--   0        0        0    20562 2024-04-03 10:27:16.695336 requirements_parser-0.9.0/tests/reqfiles/crateio_requirements.expected
+-rw-r--r--   0        0        0     2885 2024-04-03 10:27:16.695336 requirements_parser-0.9.0/tests/reqfiles/crateio_requirements.txt
+-rw-r--r--   0        0        0     1818 2024-04-03 10:27:16.695336 requirements_parser-0.9.0/tests/reqfiles/editable_1.expected
+-rw-r--r--   0        0        0      308 2024-04-03 10:27:16.695336 requirements_parser-0.9.0/tests/reqfiles/editable_1.txt
+-rw-r--r--   0        0        0     1564 2024-04-03 10:27:16.695336 requirements_parser-0.9.0/tests/reqfiles/editable_2.expected
+-rw-r--r--   0        0        0      338 2024-04-03 10:27:16.695336 requirements_parser-0.9.0/tests/reqfiles/editable_2.txt
+-rw-r--r--   0        0        0      635 2024-04-03 10:27:16.695336 requirements_parser-0.9.0/tests/reqfiles/extras_1.expected
+-rw-r--r--   0        0        0       37 2024-04-03 10:27:16.695336 requirements_parser-0.9.0/tests/reqfiles/extras_1.txt
+-rw-r--r--   0        0        0       24 2024-04-03 10:27:16.695336 requirements_parser-0.9.0/tests/reqfiles/fail_1.txt
+-rw-r--r--   0        0        0       58 2024-04-03 10:27:16.695336 requirements_parser-0.9.0/tests/reqfiles/fail_2.txt
+-rw-r--r--   0        0        0     1339 2024-04-03 10:27:16.695336 requirements_parser-0.9.0/tests/reqfiles/file_1.expected
+-rw-r--r--   0        0        0      172 2024-04-03 10:27:16.695336 requirements_parser-0.9.0/tests/reqfiles/file_1.txt
+-rw-r--r--   0        0        0      311 2024-04-03 10:27:16.695336 requirements_parser-0.9.0/tests/reqfiles/global_options_requirements.expected
+-rw-r--r--   0        0        0      168 2024-04-03 10:27:16.695336 requirements_parser-0.9.0/tests/reqfiles/global_options_requirements.txt
+-rw-r--r--   0        0        0      635 2024-04-03 10:27:16.695336 requirements_parser-0.9.0/tests/reqfiles/hash_1.expected
+-rw-r--r--   0        0        0      386 2024-04-03 10:27:16.695336 requirements_parser-0.9.0/tests/reqfiles/hash_1.txt
+-rw-r--r--   0        0        0      319 2024-04-03 10:27:16.695336 requirements_parser-0.9.0/tests/reqfiles/hash_2.expected
+-rw-r--r--   0        0        0       95 2024-04-03 10:27:16.695336 requirements_parser-0.9.0/tests/reqfiles/hash_2.txt
+-rw-r--r--   0        0        0     1317 2024-04-03 10:27:16.695336 requirements_parser-0.9.0/tests/reqfiles/illustrative_requirements.expected
+-rw-r--r--   0        0        0      121 2024-04-03 10:27:16.695336 requirements_parser-0.9.0/tests/reqfiles/illustrative_requirements.txt
+-rw-r--r--   0        0        0      948 2024-04-03 10:27:16.695336 requirements_parser-0.9.0/tests/reqfiles/recursive_1.expected
+-rw-r--r--   0        0        0       30 2024-04-03 10:27:16.695336 requirements_parser-0.9.0/tests/reqfiles/recursive_1.txt
+-rw-r--r--   0        0        0      595 2024-04-03 10:27:16.695336 requirements_parser-0.9.0/tests/reqfiles/recursive_2.expected
+-rw-r--r--   0        0        0       24 2024-04-03 10:27:16.695336 requirements_parser-0.9.0/tests/reqfiles/recursive_2.txt
+-rw-r--r--   0        0        0      359 2024-04-03 10:27:16.695336 requirements_parser-0.9.0/tests/reqfiles/recursive_3.expected
+-rw-r--r--   0        0        0        4 2024-04-03 10:27:16.695336 requirements_parser-0.9.0/tests/reqfiles/recursive_3.txt
+-rw-r--r--   0        0        0     1387 2024-04-03 10:27:16.695336 requirements_parser-0.9.0/tests/reqfiles/rtfd_deploy_requirements.expected
+-rw-r--r--   0        0        0     1184 2024-04-03 10:27:16.695336 requirements_parser-0.9.0/tests/reqfiles/rtfd_deploy_requirements.txt
+-rw-r--r--   0        0        0    10893 2024-04-03 10:27:16.695336 requirements_parser-0.9.0/tests/reqfiles/rtfd_requirements.expected
+-rw-r--r--   0        0        0     2341 2024-04-03 10:27:16.695336 requirements_parser-0.9.0/tests/reqfiles/rtfd_requirements.txt
+-rw-r--r--   0        0        0     1242 2024-04-03 10:27:16.695336 requirements_parser-0.9.0/tests/reqfiles/simple_1.expected
+-rw-r--r--   0        0        0       65 2024-04-03 10:27:16.695336 requirements_parser-0.9.0/tests/reqfiles/simple_1.txt
+-rw-r--r--   0        0        0      408 2024-04-03 10:27:16.695336 requirements_parser-0.9.0/tests/reqfiles/specs_1.expected
+-rw-r--r--   0        0        0       43 2024-04-03 10:27:16.695336 requirements_parser-0.9.0/tests/reqfiles/specs_1.txt
+-rw-r--r--   0        0        0      759 2024-04-03 10:27:16.695336 requirements_parser-0.9.0/tests/reqfiles/subdirectory.expected
+-rw-r--r--   0        0        0      145 2024-04-03 10:27:16.695336 requirements_parser-0.9.0/tests/reqfiles/subdirectory.txt
+-rw-r--r--   0        0        0      305 2024-04-03 10:27:16.695336 requirements_parser-0.9.0/tests/reqfiles/underscores.expected
+-rw-r--r--   0        0        0        9 2024-04-03 10:27:16.695336 requirements_parser-0.9.0/tests/reqfiles/underscores.txt
+-rw-r--r--   0        0        0      926 2024-04-03 10:27:16.695336 requirements_parser-0.9.0/tests/reqfiles/uri.expected
+-rw-r--r--   0        0        0      214 2024-04-03 10:27:16.695336 requirements_parser-0.9.0/tests/reqfiles/uri.txt
+-rw-r--r--   0        0        0     4479 2024-04-03 10:27:16.695336 requirements_parser-0.9.0/tests/reqfiles/vcs_bzr.expected
+-rw-r--r--   0        0        0      751 2024-04-03 10:27:16.695336 requirements_parser-0.9.0/tests/reqfiles/vcs_bzr.txt
+-rw-r--r--   0        0        0     4842 2024-04-03 10:27:16.695336 requirements_parser-0.9.0/tests/reqfiles/vcs_git.expected
+-rw-r--r--   0        0        0      812 2024-04-03 10:27:16.695336 requirements_parser-0.9.0/tests/reqfiles/vcs_git.txt
+-rw-r--r--   0        0        0      397 2024-04-03 10:27:16.695336 requirements_parser-0.9.0/tests/reqfiles/vcs_git_extras_require.expected
+-rw-r--r--   0        0        0       73 2024-04-03 10:27:16.695336 requirements_parser-0.9.0/tests/reqfiles/vcs_git_extras_require.txt
+-rw-r--r--   0        0        0     5078 2024-04-03 10:27:16.695336 requirements_parser-0.9.0/tests/reqfiles/vcs_hg.expected
+-rw-r--r--   0        0        0      814 2024-04-03 10:27:16.695336 requirements_parser-0.9.0/tests/reqfiles/vcs_hg.txt
+-rw-r--r--   0        0        0     1502 2024-04-03 10:27:16.695336 requirements_parser-0.9.0/tests/reqfiles/vcs_svn.expected
+-rw-r--r--   0        0        0      255 2024-04-03 10:27:16.695336 requirements_parser-0.9.0/tests/reqfiles/vcs_svn.txt
+-rw-r--r--   0        0        0     2703 2024-04-03 10:27:16.695336 requirements_parser-0.9.0/tests/test_parser.py
+-rw-r--r--   0        0        0     2145 2024-04-03 10:27:16.695336 requirements_parser-0.9.0/tests/test_requirement.py
+-rw-r--r--   0        0        0     3245 1970-01-01 00:00:00.000000 requirements_parser-0.9.0/PKG-INFO
```

### Comparing `requirements_parser-0.8.0/LICENSE` & `requirements_parser-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `requirements_parser-0.8.0/README.md` & `requirements_parser-0.9.0/README.md`

 * *Files identical despite different names*

### Comparing `requirements_parser-0.8.0/pyproject.toml` & `requirements_parser-0.9.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "requirements-parser"
 # !! version is managed by semantic_release
-version = "0.8.0"
+version = "0.9.0"
 description = "This is a small Python module for parsing Pip requirement files."
 authors = [
     "Paul Horton <paul@hogr.dev>",
     "David Fischer (@davidfischer)",
     "Trey Hunner (@treyhunner)",
     "Dima Veselov (@dveselov)",
     "Sascha Peilicke (@saschpe)",
```

### Comparing `requirements_parser-0.8.0/requirements/__init__.py` & `requirements_parser-0.9.0/requirements/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,8 +20,8 @@
 
 __all__ = [
     'parse'
 ]
 
 # !! version is managed by semantic_release
 # do not use typing here, or else `semantic_release` might have issues finding the variable
-__version__ = "0.8.0"  # noqa:Q000
+__version__ = "0.9.0"  # noqa:Q000
```

### Comparing `requirements_parser-0.8.0/requirements/fragment.py` & `requirements_parser-0.9.0/requirements/fragment.py`

 * *Files identical despite different names*

### Comparing `requirements_parser-0.8.0/requirements/parser.py` & `requirements_parser-0.9.0/requirements/parser.py`

 * *Files 6% similar despite different names*

```diff
@@ -58,15 +58,18 @@
         line = line.strip()
 
         if line == '':
             continue
         elif not line or line.startswith('#'):
             # comments are lines that start with # only
             continue
-        elif line.startswith('-r') or line.startswith('--requirement'):
+        elif not line or line.startswith('--hash='):
+            # hashes are lines that start with --hash=
+            continue
+        elif line.startswith(('-r', '--requirement')):
             _, new_filename = line.split()
             new_file_path = os.path.join(os.path.dirname(filename or '.'),
                                          new_filename)
             with open(new_file_path) as f:
                 for requirement in parse(f):
                     yield requirement
         elif line.startswith('-f') or line.startswith('--find-links') or \
```

### Comparing `requirements_parser-0.8.0/requirements/py.typed` & `requirements_parser-0.9.0/requirements/py.typed`

 * *Files identical despite different names*

### Comparing `requirements_parser-0.8.0/requirements/requirement.py` & `requirements_parser-0.9.0/requirements/requirement.py`

 * *Files 2% similar despite different names*

```diff
@@ -249,8 +249,13 @@
 
         if line.startswith('-e') or line.startswith('--editable'):
             # Editable installs are either a local project path
             # or a VCS project URI
             return cls.parse_editable(
                 re.sub(r'^(-e|--editable=?)\s*', '', line))
 
+        if ' --hash=' in line:
+            line = line[:line.find(' --hash=')]
+        if ' \\' in line:
+            line = line[:line.find(' \\')]
+
         return cls.parse_line(line)
```

### Comparing `requirements_parser-0.8.0/requirements/vcs.py` & `requirements_parser-0.9.0/requirements/vcs.py`

 * *Files identical despite different names*

### Comparing `requirements_parser-0.8.0/tests/__init__.py` & `requirements_parser-0.9.0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `requirements_parser-0.8.0/tests/reqfiles/crateio_requirements.expected` & `requirements_parser-0.9.0/tests/reqfiles/crateio_requirements.expected`

 * *Files identical despite different names*

### Comparing `requirements_parser-0.8.0/tests/reqfiles/crateio_requirements.txt` & `requirements_parser-0.9.0/tests/reqfiles/crateio_requirements.txt`

 * *Files identical despite different names*

### Comparing `requirements_parser-0.8.0/tests/reqfiles/editable_1.expected` & `requirements_parser-0.9.0/tests/reqfiles/editable_1.expected`

 * *Files identical despite different names*

### Comparing `requirements_parser-0.8.0/tests/reqfiles/editable_2.expected` & `requirements_parser-0.9.0/tests/reqfiles/editable_2.expected`

 * *Files identical despite different names*

### Comparing `requirements_parser-0.8.0/tests/reqfiles/extras_1.expected` & `requirements_parser-0.9.0/tests/reqfiles/extras_1.expected`

 * *Files identical despite different names*

### Comparing `requirements_parser-0.8.0/tests/reqfiles/file_1.expected` & `requirements_parser-0.9.0/tests/reqfiles/file_1.expected`

 * *Files identical despite different names*

### Comparing `requirements_parser-0.8.0/tests/reqfiles/illustrative_requirements.expected` & `requirements_parser-0.9.0/tests/reqfiles/illustrative_requirements.expected`

 * *Files identical despite different names*

### Comparing `requirements_parser-0.8.0/tests/reqfiles/recursive_1.expected` & `requirements_parser-0.9.0/tests/reqfiles/recursive_1.expected`

 * *Files identical despite different names*

### Comparing `requirements_parser-0.8.0/tests/reqfiles/recursive_2.expected` & `requirements_parser-0.9.0/tests/reqfiles/recursive_2.expected`

 * *Files identical despite different names*

### Comparing `requirements_parser-0.8.0/tests/reqfiles/rtfd_deploy_requirements.expected` & `requirements_parser-0.9.0/tests/reqfiles/rtfd_deploy_requirements.expected`

 * *Files identical despite different names*

### Comparing `requirements_parser-0.8.0/tests/reqfiles/rtfd_deploy_requirements.txt` & `requirements_parser-0.9.0/tests/reqfiles/rtfd_deploy_requirements.txt`

 * *Files identical despite different names*

### Comparing `requirements_parser-0.8.0/tests/reqfiles/rtfd_requirements.expected` & `requirements_parser-0.9.0/tests/reqfiles/rtfd_requirements.expected`

 * *Files identical despite different names*

### Comparing `requirements_parser-0.8.0/tests/reqfiles/rtfd_requirements.txt` & `requirements_parser-0.9.0/tests/reqfiles/rtfd_requirements.txt`

 * *Files identical despite different names*

### Comparing `requirements_parser-0.8.0/tests/reqfiles/simple_1.expected` & `requirements_parser-0.9.0/tests/reqfiles/simple_1.expected`

 * *Files identical despite different names*

### Comparing `requirements_parser-0.8.0/tests/reqfiles/subdirectory.expected` & `requirements_parser-0.9.0/tests/reqfiles/subdirectory.expected`

 * *Files identical despite different names*

### Comparing `requirements_parser-0.8.0/tests/reqfiles/uri.expected` & `requirements_parser-0.9.0/tests/reqfiles/uri.expected`

 * *Files identical despite different names*

### Comparing `requirements_parser-0.8.0/tests/reqfiles/vcs_bzr.expected` & `requirements_parser-0.9.0/tests/reqfiles/vcs_bzr.expected`

 * *Files identical despite different names*

### Comparing `requirements_parser-0.8.0/tests/reqfiles/vcs_bzr.txt` & `requirements_parser-0.9.0/tests/reqfiles/vcs_bzr.txt`

 * *Files identical despite different names*

### Comparing `requirements_parser-0.8.0/tests/reqfiles/vcs_git.expected` & `requirements_parser-0.9.0/tests/reqfiles/vcs_git.expected`

 * *Files identical despite different names*

### Comparing `requirements_parser-0.8.0/tests/reqfiles/vcs_git.txt` & `requirements_parser-0.9.0/tests/reqfiles/vcs_git.txt`

 * *Files identical despite different names*

### Comparing `requirements_parser-0.8.0/tests/reqfiles/vcs_hg.expected` & `requirements_parser-0.9.0/tests/reqfiles/vcs_hg.expected`

 * *Files identical despite different names*

### Comparing `requirements_parser-0.8.0/tests/reqfiles/vcs_hg.txt` & `requirements_parser-0.9.0/tests/reqfiles/vcs_hg.txt`

 * *Files identical despite different names*

### Comparing `requirements_parser-0.8.0/tests/reqfiles/vcs_svn.expected` & `requirements_parser-0.9.0/tests/reqfiles/vcs_svn.expected`

 * *Files identical despite different names*

### Comparing `requirements_parser-0.8.0/tests/test_parser.py` & `requirements_parser-0.9.0/tests/test_parser.py`

 * *Files identical despite different names*

### Comparing `requirements_parser-0.8.0/tests/test_requirement.py` & `requirements_parser-0.9.0/tests/test_requirement.py`

 * *Files identical despite different names*

### Comparing `requirements_parser-0.8.0/PKG-INFO` & `requirements_parser-0.9.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: requirements-parser
-Version: 0.8.0
+Version: 0.9.0
 Summary: This is a small Python module for parsing Pip requirement files.
 Home-page: https://github.com/madpah/requirements-parser/#readme
 License: Apache-2.0
 Keywords: Pip,requirements,parse
 Author: Paul Horton
 Author-email: paul@hogr.dev
 Maintainer: Paul Horton
```

