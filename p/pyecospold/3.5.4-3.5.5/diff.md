# Comparing `tmp/pyecospold-3.5.4.tar.gz` & `tmp/pyecospold-3.5.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyecospold-3.5.4.tar", last modified: Thu Mar 28 13:52:38 2024, max compression
+gzip compressed data, was "pyecospold-3.5.5.tar", last modified: Wed Apr  3 13:49:14 2024, max compression
```

## Comparing `pyecospold-3.5.4.tar` & `pyecospold-3.5.5.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:52:38.203174 pyecospold-3.5.4/
--rw-r--r--   0 runner    (1001) docker     (127)     1454 2024-03-28 13:52:34.000000 pyecospold-3.5.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-03-28 13:52:34.000000 pyecospold-3.5.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     5918 2024-03-28 13:52:38.203174 pyecospold-3.5.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4174 2024-03-28 13:52:34.000000 pyecospold-3.5.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:52:38.195174 pyecospold-3.5.4/pyecospold/
--rw-r--r--   0 runner    (1001) docker     (127)      791 2024-03-28 13:52:34.000000 pyecospold-3.5.4/pyecospold/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2797 2024-03-28 13:52:34.000000 pyecospold-3.5.4/pyecospold/config.py
--rw-r--r--   0 runner    (1001) docker     (127)    14498 2024-03-28 13:52:34.000000 pyecospold-3.5.4/pyecospold/core.py
--rw-r--r--   0 runner    (1001) docker     (127)     1692 2024-03-28 13:52:34.000000 pyecospold-3.5.4/pyecospold/helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)    58148 2024-03-28 13:52:34.000000 pyecospold-3.5.4/pyecospold/model_v1.py
--rw-r--r--   0 runner    (1001) docker     (127)    99315 2024-03-28 13:52:34.000000 pyecospold-3.5.4/pyecospold/model_v2.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:52:38.191174 pyecospold-3.5.4/pyecospold/schemas/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:52:38.199174 pyecospold-3.5.4/pyecospold/schemas/v1/
--rw-r--r--   0 runner    (1001) docker     (127)     5486 2024-03-28 13:52:34.000000 pyecospold-3.5.4/pyecospold/schemas/v1/EcoInventCategories.xsd
--rw-r--r--   0 runner    (1001) docker     (127)     3387 2024-03-28 13:52:34.000000 pyecospold-3.5.4/pyecospold/schemas/v1/EcoInventCompanyCodes.xsd
--rw-r--r--   0 runner    (1001) docker     (127)     2568 2024-03-28 13:52:34.000000 pyecospold-3.5.4/pyecospold/schemas/v1/EcoInventRegionalCodes.xsd
--rw-r--r--   0 runner    (1001) docker     (127)     2215 2024-03-28 13:52:34.000000 pyecospold-3.5.4/pyecospold/schemas/v1/EcoInventUnits.xsd
--rw-r--r--   0 runner    (1001) docker     (127)    23151 2024-03-28 13:52:34.000000 pyecospold-3.5.4/pyecospold/schemas/v1/EcoSpold01DataTypes.xsd
--rw-r--r--   0 runner    (1001) docker     (127)    16759 2024-03-28 13:52:34.000000 pyecospold-3.5.4/pyecospold/schemas/v1/EcoSpold01Dataset.xsd
--rw-r--r--   0 runner    (1001) docker     (127)    11858 2024-03-28 13:52:34.000000 pyecospold-3.5.4/pyecospold/schemas/v1/EcoSpold01ElementaryDataset.xsd
--rw-r--r--   0 runner    (1001) docker     (127)    23965 2024-03-28 13:52:34.000000 pyecospold-3.5.4/pyecospold/schemas/v1/EcoSpold01FlowData.xsd
--rw-r--r--   0 runner    (1001) docker     (127)    15813 2024-03-28 13:52:34.000000 pyecospold-3.5.4/pyecospold/schemas/v1/EcoSpold01ImpactDataset.xsd
--rw-r--r--   0 runner    (1001) docker     (127)    59212 2024-03-28 13:52:34.000000 pyecospold-3.5.4/pyecospold/schemas/v1/EcoSpold01MetaInformation.xsd
--rw-r--r--   0 runner    (1001) docker     (127)     4015 2024-03-28 13:52:34.000000 pyecospold-3.5.4/pyecospold/schemas/v1/XmlNamespace.xsd
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:52:38.199174 pyecospold-3.5.4/pyecospold/schemas/v2/
--rw-r--r--   0 runner    (1001) docker     (127)     2227 2024-03-28 13:52:34.000000 pyecospold-3.5.4/pyecospold/schemas/v2/EcoSpold02.xsd
--rw-r--r--   0 runner    (1001) docker     (127)    19919 2024-03-28 13:52:34.000000 pyecospold-3.5.4/pyecospold/schemas/v2/EcoSpold02Activity.xsd
--rw-r--r--   0 runner    (1001) docker     (127)    20082 2024-03-28 13:52:34.000000 pyecospold-3.5.4/pyecospold/schemas/v2/EcoSpold02ChildActivity.xsd
--rw-r--r--   0 runner    (1001) docker     (127)    50218 2024-03-28 13:52:34.000000 pyecospold-3.5.4/pyecospold/schemas/v2/EcoSpold02ChildDataTypes.xsd
--rw-r--r--   0 runner    (1001) docker     (127)    52466 2024-03-28 13:52:34.000000 pyecospold-3.5.4/pyecospold/schemas/v2/EcoSpold02ChildFlowData.xsd
--rw-r--r--   0 runner    (1001) docker     (127)    70861 2024-03-28 13:52:34.000000 pyecospold-3.5.4/pyecospold/schemas/v2/EcoSpold02ChildMetaInformation.xsd
--rw-r--r--   0 runner    (1001) docker     (127)    49965 2024-03-28 13:52:34.000000 pyecospold-3.5.4/pyecospold/schemas/v2/EcoSpold02DataTypes.xsd
--rw-r--r--   0 runner    (1001) docker     (127)    52230 2024-03-28 13:52:34.000000 pyecospold-3.5.4/pyecospold/schemas/v2/EcoSpold02FlowData.xsd
--rw-r--r--   0 runner    (1001) docker     (127)    70813 2024-03-28 13:52:34.000000 pyecospold-3.5.4/pyecospold/schemas/v2/EcoSpold02MetaInformation.xsd
--rw-r--r--   0 runner    (1001) docker     (127)     4736 2024-03-28 13:52:34.000000 pyecospold-3.5.4/pyecospold/schemas/v2/XmlNamespace.xsd
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-03-28 13:52:34.000000 pyecospold-3.5.4/pyecospold/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:52:38.199174 pyecospold-3.5.4/pyecospold.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5918 2024-03-28 13:52:38.000000 pyecospold-3.5.4/pyecospold.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1460 2024-03-28 13:52:38.000000 pyecospold-3.5.4/pyecospold.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-28 13:52:38.000000 pyecospold-3.5.4/pyecospold.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      212 2024-03-28 13:52:38.000000 pyecospold-3.5.4/pyecospold.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-03-28 13:52:38.000000 pyecospold-3.5.4/pyecospold.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2502 2024-03-28 13:52:34.000000 pyecospold-3.5.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-28 13:52:38.203174 pyecospold-3.5.4/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 13:52:38.199174 pyecospold-3.5.4/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1167 2024-03-28 13:52:34.000000 pyecospold-3.5.4/tests/test_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     6597 2024-03-28 13:52:34.000000 pyecospold-3.5.4/tests/test_core.py
--rw-r--r--   0 runner    (1001) docker     (127)     1890 2024-03-28 13:52:34.000000 pyecospold-3.5.4/tests/test_helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)    18100 2024-03-28 13:52:34.000000 pyecospold-3.5.4/tests/test_model_v1.py
--rw-r--r--   0 runner    (1001) docker     (127)    29326 2024-03-28 13:52:34.000000 pyecospold-3.5.4/tests/test_model_v2.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 13:49:14.227437 pyecospold-3.5.5/
+-rw-r--r--   0 runner    (1001) docker     (127)     1454 2024-04-03 13:49:10.000000 pyecospold-3.5.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-04-03 13:49:10.000000 pyecospold-3.5.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     5918 2024-04-03 13:49:14.227437 pyecospold-3.5.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4174 2024-04-03 13:49:10.000000 pyecospold-3.5.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 13:49:14.219437 pyecospold-3.5.5/pyecospold/
+-rw-r--r--   0 runner    (1001) docker     (127)      791 2024-04-03 13:49:10.000000 pyecospold-3.5.5/pyecospold/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2797 2024-04-03 13:49:10.000000 pyecospold-3.5.5/pyecospold/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14498 2024-04-03 13:49:10.000000 pyecospold-3.5.5/pyecospold/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1692 2024-04-03 13:49:10.000000 pyecospold-3.5.5/pyecospold/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    58148 2024-04-03 13:49:10.000000 pyecospold-3.5.5/pyecospold/model_v1.py
+-rw-r--r--   0 runner    (1001) docker     (127)    99315 2024-04-03 13:49:10.000000 pyecospold-3.5.5/pyecospold/model_v2.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 13:49:14.215437 pyecospold-3.5.5/pyecospold/schemas/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 13:49:14.223437 pyecospold-3.5.5/pyecospold/schemas/v1/
+-rw-r--r--   0 runner    (1001) docker     (127)     5486 2024-04-03 13:49:10.000000 pyecospold-3.5.5/pyecospold/schemas/v1/EcoInventCategories.xsd
+-rw-r--r--   0 runner    (1001) docker     (127)     3387 2024-04-03 13:49:10.000000 pyecospold-3.5.5/pyecospold/schemas/v1/EcoInventCompanyCodes.xsd
+-rw-r--r--   0 runner    (1001) docker     (127)     2568 2024-04-03 13:49:10.000000 pyecospold-3.5.5/pyecospold/schemas/v1/EcoInventRegionalCodes.xsd
+-rw-r--r--   0 runner    (1001) docker     (127)     2215 2024-04-03 13:49:10.000000 pyecospold-3.5.5/pyecospold/schemas/v1/EcoInventUnits.xsd
+-rw-r--r--   0 runner    (1001) docker     (127)    23151 2024-04-03 13:49:10.000000 pyecospold-3.5.5/pyecospold/schemas/v1/EcoSpold01DataTypes.xsd
+-rw-r--r--   0 runner    (1001) docker     (127)    16759 2024-04-03 13:49:10.000000 pyecospold-3.5.5/pyecospold/schemas/v1/EcoSpold01Dataset.xsd
+-rw-r--r--   0 runner    (1001) docker     (127)    11858 2024-04-03 13:49:10.000000 pyecospold-3.5.5/pyecospold/schemas/v1/EcoSpold01ElementaryDataset.xsd
+-rw-r--r--   0 runner    (1001) docker     (127)    23965 2024-04-03 13:49:10.000000 pyecospold-3.5.5/pyecospold/schemas/v1/EcoSpold01FlowData.xsd
+-rw-r--r--   0 runner    (1001) docker     (127)    15813 2024-04-03 13:49:10.000000 pyecospold-3.5.5/pyecospold/schemas/v1/EcoSpold01ImpactDataset.xsd
+-rw-r--r--   0 runner    (1001) docker     (127)    59212 2024-04-03 13:49:10.000000 pyecospold-3.5.5/pyecospold/schemas/v1/EcoSpold01MetaInformation.xsd
+-rw-r--r--   0 runner    (1001) docker     (127)     4015 2024-04-03 13:49:10.000000 pyecospold-3.5.5/pyecospold/schemas/v1/XmlNamespace.xsd
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 13:49:14.223437 pyecospold-3.5.5/pyecospold/schemas/v2/
+-rw-r--r--   0 runner    (1001) docker     (127)     2227 2024-04-03 13:49:10.000000 pyecospold-3.5.5/pyecospold/schemas/v2/EcoSpold02.xsd
+-rw-r--r--   0 runner    (1001) docker     (127)    19919 2024-04-03 13:49:10.000000 pyecospold-3.5.5/pyecospold/schemas/v2/EcoSpold02Activity.xsd
+-rw-r--r--   0 runner    (1001) docker     (127)    20082 2024-04-03 13:49:10.000000 pyecospold-3.5.5/pyecospold/schemas/v2/EcoSpold02ChildActivity.xsd
+-rw-r--r--   0 runner    (1001) docker     (127)    50218 2024-04-03 13:49:10.000000 pyecospold-3.5.5/pyecospold/schemas/v2/EcoSpold02ChildDataTypes.xsd
+-rw-r--r--   0 runner    (1001) docker     (127)    52466 2024-04-03 13:49:10.000000 pyecospold-3.5.5/pyecospold/schemas/v2/EcoSpold02ChildFlowData.xsd
+-rw-r--r--   0 runner    (1001) docker     (127)    70861 2024-04-03 13:49:10.000000 pyecospold-3.5.5/pyecospold/schemas/v2/EcoSpold02ChildMetaInformation.xsd
+-rw-r--r--   0 runner    (1001) docker     (127)    49965 2024-04-03 13:49:10.000000 pyecospold-3.5.5/pyecospold/schemas/v2/EcoSpold02DataTypes.xsd
+-rw-r--r--   0 runner    (1001) docker     (127)    52230 2024-04-03 13:49:10.000000 pyecospold-3.5.5/pyecospold/schemas/v2/EcoSpold02FlowData.xsd
+-rw-r--r--   0 runner    (1001) docker     (127)    70813 2024-04-03 13:49:10.000000 pyecospold-3.5.5/pyecospold/schemas/v2/EcoSpold02MetaInformation.xsd
+-rw-r--r--   0 runner    (1001) docker     (127)     4736 2024-04-03 13:49:10.000000 pyecospold-3.5.5/pyecospold/schemas/v2/XmlNamespace.xsd
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-04-03 13:49:10.000000 pyecospold-3.5.5/pyecospold/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 13:49:14.227437 pyecospold-3.5.5/pyecospold.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5918 2024-04-03 13:49:14.000000 pyecospold-3.5.5/pyecospold.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1460 2024-04-03 13:49:14.000000 pyecospold-3.5.5/pyecospold.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 13:49:14.000000 pyecospold-3.5.5/pyecospold.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      212 2024-04-03 13:49:14.000000 pyecospold-3.5.5/pyecospold.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-03 13:49:14.000000 pyecospold-3.5.5/pyecospold.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2502 2024-04-03 13:49:10.000000 pyecospold-3.5.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-03 13:49:14.227437 pyecospold-3.5.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 13:49:14.227437 pyecospold-3.5.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1167 2024-04-03 13:49:10.000000 pyecospold-3.5.5/tests/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6597 2024-04-03 13:49:10.000000 pyecospold-3.5.5/tests/test_core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1890 2024-04-03 13:49:10.000000 pyecospold-3.5.5/tests/test_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18100 2024-04-03 13:49:10.000000 pyecospold-3.5.5/tests/test_model_v1.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29326 2024-04-03 13:49:10.000000 pyecospold-3.5.5/tests/test_model_v2.py
```

### Comparing `pyecospold-3.5.4/LICENSE` & `pyecospold-3.5.5/LICENSE`

 * *Files identical despite different names*

### Comparing `pyecospold-3.5.4/PKG-INFO` & `pyecospold-3.5.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyecospold
-Version: 3.5.4
+Version: 3.5.5
 Summary: A Python package that converts ecospold XML formats to their Python equivalents and export the same data back to XML.
 Author-email: Mina Sami <sami.mg@outlook.com>
 Maintainer-email: Mina Sami <sami.mg@outlook.com>
 Project-URL: source, https://github.com/sami-m-g/pyecospold
 Project-URL: homepage, https://github.com/sami-m-g/pyecospold
 Project-URL: tracker, https://github.com/sami-m-g/pyecospold/issues
 Classifier: Development Status :: 4 - Beta
```

### Comparing `pyecospold-3.5.4/README.md` & `pyecospold-3.5.5/README.md`

 * *Files identical despite different names*

### Comparing `pyecospold-3.5.4/pyecospold/__init__.py` & `pyecospold-3.5.5/pyecospold/__init__.py`

 * *Files identical despite different names*

### Comparing `pyecospold-3.5.4/pyecospold/config.py` & `pyecospold-3.5.5/pyecospold/config.py`

 * *Files identical despite different names*

### Comparing `pyecospold-3.5.4/pyecospold/core.py` & `pyecospold-3.5.5/pyecospold/core.py`

 * *Files identical despite different names*

### Comparing `pyecospold-3.5.4/pyecospold/helpers.py` & `pyecospold-3.5.5/pyecospold/helpers.py`

 * *Files identical despite different names*

### Comparing `pyecospold-3.5.4/pyecospold/model_v1.py` & `pyecospold-3.5.5/pyecospold/model_v1.py`

 * *Files identical despite different names*

### Comparing `pyecospold-3.5.4/pyecospold/model_v2.py` & `pyecospold-3.5.5/pyecospold/model_v2.py`

 * *Files identical despite different names*

### Comparing `pyecospold-3.5.4/pyecospold/schemas/v1/EcoInventCategories.xsd` & `pyecospold-3.5.5/pyecospold/schemas/v1/EcoInventCategories.xsd`

 * *Files identical despite different names*

### Comparing `pyecospold-3.5.4/pyecospold/schemas/v1/EcoInventCompanyCodes.xsd` & `pyecospold-3.5.5/pyecospold/schemas/v1/EcoInventCompanyCodes.xsd`

 * *Files identical despite different names*

### Comparing `pyecospold-3.5.4/pyecospold/schemas/v1/EcoInventRegionalCodes.xsd` & `pyecospold-3.5.5/pyecospold/schemas/v1/EcoInventRegionalCodes.xsd`

 * *Files identical despite different names*

### Comparing `pyecospold-3.5.4/pyecospold/schemas/v1/EcoInventUnits.xsd` & `pyecospold-3.5.5/pyecospold/schemas/v1/EcoInventUnits.xsd`

 * *Files identical despite different names*

### Comparing `pyecospold-3.5.4/pyecospold/schemas/v1/EcoSpold01DataTypes.xsd` & `pyecospold-3.5.5/pyecospold/schemas/v1/EcoSpold01DataTypes.xsd`

 * *Files identical despite different names*

### Comparing `pyecospold-3.5.4/pyecospold/schemas/v1/EcoSpold01Dataset.xsd` & `pyecospold-3.5.5/pyecospold/schemas/v1/EcoSpold01Dataset.xsd`

 * *Files identical despite different names*

### Comparing `pyecospold-3.5.4/pyecospold/schemas/v1/EcoSpold01ElementaryDataset.xsd` & `pyecospold-3.5.5/pyecospold/schemas/v1/EcoSpold01ElementaryDataset.xsd`

 * *Files identical despite different names*

### Comparing `pyecospold-3.5.4/pyecospold/schemas/v1/EcoSpold01FlowData.xsd` & `pyecospold-3.5.5/pyecospold/schemas/v1/EcoSpold01FlowData.xsd`

 * *Files identical despite different names*

### Comparing `pyecospold-3.5.4/pyecospold/schemas/v1/EcoSpold01ImpactDataset.xsd` & `pyecospold-3.5.5/pyecospold/schemas/v1/EcoSpold01ImpactDataset.xsd`

 * *Files identical despite different names*

### Comparing `pyecospold-3.5.4/pyecospold/schemas/v1/EcoSpold01MetaInformation.xsd` & `pyecospold-3.5.5/pyecospold/schemas/v1/EcoSpold01MetaInformation.xsd`

 * *Files identical despite different names*

### Comparing `pyecospold-3.5.4/pyecospold/schemas/v1/XmlNamespace.xsd` & `pyecospold-3.5.5/pyecospold/schemas/v1/XmlNamespace.xsd`

 * *Files identical despite different names*

### Comparing `pyecospold-3.5.4/pyecospold/schemas/v2/EcoSpold02.xsd` & `pyecospold-3.5.5/pyecospold/schemas/v2/EcoSpold02.xsd`

 * *Files identical despite different names*

### Comparing `pyecospold-3.5.4/pyecospold/schemas/v2/EcoSpold02Activity.xsd` & `pyecospold-3.5.5/pyecospold/schemas/v2/EcoSpold02Activity.xsd`

 * *Files identical despite different names*

### Comparing `pyecospold-3.5.4/pyecospold/schemas/v2/EcoSpold02ChildActivity.xsd` & `pyecospold-3.5.5/pyecospold/schemas/v2/EcoSpold02ChildActivity.xsd`

 * *Files identical despite different names*

### Comparing `pyecospold-3.5.4/pyecospold/schemas/v2/EcoSpold02ChildDataTypes.xsd` & `pyecospold-3.5.5/pyecospold/schemas/v2/EcoSpold02ChildDataTypes.xsd`

 * *Files identical despite different names*

### Comparing `pyecospold-3.5.4/pyecospold/schemas/v2/EcoSpold02ChildFlowData.xsd` & `pyecospold-3.5.5/pyecospold/schemas/v2/EcoSpold02ChildFlowData.xsd`

 * *Files identical despite different names*

### Comparing `pyecospold-3.5.4/pyecospold/schemas/v2/EcoSpold02ChildMetaInformation.xsd` & `pyecospold-3.5.5/pyecospold/schemas/v2/EcoSpold02ChildMetaInformation.xsd`

 * *Files identical despite different names*

### Comparing `pyecospold-3.5.4/pyecospold/schemas/v2/EcoSpold02DataTypes.xsd` & `pyecospold-3.5.5/pyecospold/schemas/v2/EcoSpold02DataTypes.xsd`

 * *Files identical despite different names*

### Comparing `pyecospold-3.5.4/pyecospold/schemas/v2/EcoSpold02FlowData.xsd` & `pyecospold-3.5.5/pyecospold/schemas/v2/EcoSpold02FlowData.xsd`

 * *Files identical despite different names*

### Comparing `pyecospold-3.5.4/pyecospold/schemas/v2/EcoSpold02MetaInformation.xsd` & `pyecospold-3.5.5/pyecospold/schemas/v2/EcoSpold02MetaInformation.xsd`

 * *Files identical despite different names*

### Comparing `pyecospold-3.5.4/pyecospold/schemas/v2/XmlNamespace.xsd` & `pyecospold-3.5.5/pyecospold/schemas/v2/XmlNamespace.xsd`

 * *Files identical despite different names*

### Comparing `pyecospold-3.5.4/pyecospold.egg-info/PKG-INFO` & `pyecospold-3.5.5/pyecospold.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyecospold
-Version: 3.5.4
+Version: 3.5.5
 Summary: A Python package that converts ecospold XML formats to their Python equivalents and export the same data back to XML.
 Author-email: Mina Sami <sami.mg@outlook.com>
 Maintainer-email: Mina Sami <sami.mg@outlook.com>
 Project-URL: source, https://github.com/sami-m-g/pyecospold
 Project-URL: homepage, https://github.com/sami-m-g/pyecospold
 Project-URL: tracker, https://github.com/sami-m-g/pyecospold/issues
 Classifier: Development Status :: 4 - Beta
```

### Comparing `pyecospold-3.5.4/pyecospold.egg-info/SOURCES.txt` & `pyecospold-3.5.5/pyecospold.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyecospold-3.5.4/pyproject.toml` & `pyecospold-3.5.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pyecospold-3.5.4/tests/test_config.py` & `pyecospold-3.5.5/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `pyecospold-3.5.4/tests/test_core.py` & `pyecospold-3.5.5/tests/test_core.py`

 * *Files identical despite different names*

### Comparing `pyecospold-3.5.4/tests/test_helpers.py` & `pyecospold-3.5.5/tests/test_helpers.py`

 * *Files identical despite different names*

### Comparing `pyecospold-3.5.4/tests/test_model_v1.py` & `pyecospold-3.5.5/tests/test_model_v1.py`

 * *Files identical despite different names*

### Comparing `pyecospold-3.5.4/tests/test_model_v2.py` & `pyecospold-3.5.5/tests/test_model_v2.py`

 * *Files identical despite different names*

