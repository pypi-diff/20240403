# Comparing `tmp/prospector_profile_duplicated-1.2.0.tar.gz` & `tmp/prospector_profile_duplicated-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prospector_profile_duplicated-1.2.0.tar", max compression
+gzip compressed data, was "prospector_profile_duplicated-1.3.0.tar", max compression
```

## Comparing `prospector_profile_duplicated-1.2.0.tar` & `prospector_profile_duplicated-1.3.0.tar`

### file list

```diff
@@ -1,12 +1,13 @@
--rw-r--r--   0        0        0     1303 2024-03-20 15:11:40.773536 prospector_profile_duplicated-1.2.0/LICENSE
--rw-r--r--   0        0        0      693 2024-03-20 15:11:40.773536 prospector_profile_duplicated-1.2.0/README.md
--rw-r--r--   0        0        0        0 2024-03-20 15:11:40.773536 prospector_profile_duplicated-1.2.0/prospector_profile_duplicated/__init__.py
--rw-r--r--   0        0        0       55 2024-03-20 15:11:40.773536 prospector_profile_duplicated-1.2.0/prospector_profile_duplicated/autoflake.yaml
--rw-r--r--   0        0        0     1794 2024-03-20 15:11:40.773536 prospector_profile_duplicated-1.2.0/prospector_profile_duplicated/black.yaml
--rw-r--r--   0        0        0      186 2024-03-20 15:11:40.773536 prospector_profile_duplicated-1.2.0/prospector_profile_duplicated/docformatter.yaml
--rw-r--r--   0        0        0      173 2024-03-20 15:11:40.773536 prospector_profile_duplicated-1.2.0/prospector_profile_duplicated/isort.yaml
--rw-r--r--   0        0        0      152 2024-03-20 15:11:40.773536 prospector_profile_duplicated-1.2.0/prospector_profile_duplicated/prospector.yaml
--rw-r--r--   0        0        0      917 2024-03-20 15:11:40.773536 prospector_profile_duplicated-1.2.0/prospector_profile_duplicated/pylint.yaml
--rw-r--r--   0        0        0      776 2024-03-20 15:11:40.773536 prospector_profile_duplicated-1.2.0/prospector_profile_duplicated/pyupgrade.yaml
--rw-r--r--   0        0        0     1778 2024-03-20 15:12:55.201506 prospector_profile_duplicated-1.2.0/pyproject.toml
--rw-r--r--   0        0        0     2002 1970-01-01 00:00:00.000000 prospector_profile_duplicated-1.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1303 2024-04-03 16:15:07.576513 prospector_profile_duplicated-1.3.0/LICENSE
+-rw-r--r--   0        0        0      693 2024-04-03 16:15:07.576513 prospector_profile_duplicated-1.3.0/README.md
+-rw-r--r--   0        0        0        0 2024-04-03 16:15:07.576513 prospector_profile_duplicated-1.3.0/prospector_profile_duplicated/__init__.py
+-rw-r--r--   0        0        0       55 2024-04-03 16:15:07.576513 prospector_profile_duplicated-1.3.0/prospector_profile_duplicated/autoflake.yaml
+-rw-r--r--   0        0        0     1794 2024-04-03 16:15:07.576513 prospector_profile_duplicated-1.3.0/prospector_profile_duplicated/black.yaml
+-rw-r--r--   0        0        0      186 2024-04-03 16:15:07.576513 prospector_profile_duplicated-1.3.0/prospector_profile_duplicated/docformatter.yaml
+-rw-r--r--   0        0        0      173 2024-04-03 16:15:07.576513 prospector_profile_duplicated-1.3.0/prospector_profile_duplicated/isort.yaml
+-rw-r--r--   0        0        0      178 2024-04-03 16:15:07.576513 prospector_profile_duplicated-1.3.0/prospector_profile_duplicated/prospector.yaml
+-rw-r--r--   0        0        0      119 2024-04-03 16:15:07.576513 prospector_profile_duplicated-1.3.0/prospector_profile_duplicated/pydocstyle.yaml
+-rw-r--r--   0        0        0      917 2024-04-03 16:15:07.576513 prospector_profile_duplicated-1.3.0/prospector_profile_duplicated/pylint.yaml
+-rw-r--r--   0        0        0      776 2024-04-03 16:15:07.576513 prospector_profile_duplicated-1.3.0/prospector_profile_duplicated/pyupgrade.yaml
+-rw-r--r--   0        0        0     1778 2024-04-03 16:15:55.148842 prospector_profile_duplicated-1.3.0/pyproject.toml
+-rw-r--r--   0        0        0     2002 1970-01-01 00:00:00.000000 prospector_profile_duplicated-1.3.0/PKG-INFO
```

### Comparing `prospector_profile_duplicated-1.2.0/LICENSE` & `prospector_profile_duplicated-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `prospector_profile_duplicated-1.2.0/README.md` & `prospector_profile_duplicated-1.3.0/README.md`

 * *Files identical despite different names*

### Comparing `prospector_profile_duplicated-1.2.0/prospector_profile_duplicated/black.yaml` & `prospector_profile_duplicated-1.3.0/prospector_profile_duplicated/black.yaml`

 * *Files identical despite different names*

### Comparing `prospector_profile_duplicated-1.2.0/prospector_profile_duplicated/pylint.yaml` & `prospector_profile_duplicated-1.3.0/prospector_profile_duplicated/pylint.yaml`

 * *Files identical despite different names*

### Comparing `prospector_profile_duplicated-1.2.0/prospector_profile_duplicated/pyupgrade.yaml` & `prospector_profile_duplicated-1.3.0/prospector_profile_duplicated/pyupgrade.yaml`

 * *Files identical despite different names*

### Comparing `prospector_profile_duplicated-1.2.0/pyproject.toml` & `prospector_profile_duplicated-1.3.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 strict = true
 
 [tool.pytest.ini_options]
 pytest_plugins = ["pytest_profiling"]
 
 [tool.poetry]
 name = "prospector-profile-duplicated"
-version = "1.2.0"
+version = "1.3.0"
 description = "Profile that can be used to disable the duplicated or conflict rules between Prospector and other tools"
 readme = "README.md"
 authors = ["Stéphane Brunner <stephane.brunner@gmail.com>"]
 homepage = "https://github.com/sbrunner/prospector-profile-duplicated"
 repository = "https://github.com/sbrunner/prospector-profile-duplicated"
 license = "BSD-2-Clause"
 classifiers = [
```

### Comparing `prospector_profile_duplicated-1.2.0/PKG-INFO` & `prospector_profile_duplicated-1.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prospector-profile-duplicated
-Version: 1.2.0
+Version: 1.3.0
 Summary: Profile that can be used to disable the duplicated or conflict rules between Prospector and other tools
 Home-page: https://github.com/sbrunner/prospector-profile-duplicated
 License: BSD-2-Clause
 Author: Stéphane Brunner
 Author-email: stephane.brunner@gmail.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

