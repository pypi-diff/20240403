# Comparing `tmp/igor2-0.5.5.tar.gz` & `tmp/igor2-0.5.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "igor2-0.5.5.tar", last modified: Wed Mar 20 16:49:58 2024, max compression
+gzip compressed data, was "igor2-0.5.6.tar", last modified: Wed Apr  3 15:25:37 2024, max compression
```

## Comparing `igor2-0.5.5.tar` & `igor2-0.5.6.tar`

### file list

```diff
@@ -1,60 +1,61 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 16:49:58.578006 igor2-0.5.5/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 16:49:58.570006 igor2-0.5.5/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 16:49:58.574006 igor2-0.5.5/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      962 2024-03-20 16:49:52.000000 igor2-0.5.5/.github/workflows/check.yml
--rw-r--r--   0 runner    (1001) docker     (127)      693 2024-03-20 16:49:52.000000 igor2-0.5.5/.github/workflows/deploy_pypi.yml
--rw-r--r--   0 runner    (1001) docker     (127)      107 2024-03-20 16:49:52.000000 igor2-0.5.5/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      722 2024-03-20 16:49:52.000000 igor2-0.5.5/CHANGELOG
--rw-r--r--   0 runner    (1001) docker     (127)     7639 2024-03-20 16:49:52.000000 igor2-0.5.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-03-20 16:49:52.000000 igor2-0.5.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     2739 2024-03-20 16:49:58.578006 igor2-0.5.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1958 2024-03-20 16:49:52.000000 igor2-0.5.5/Readme.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 16:49:58.574006 igor2-0.5.5/igor2/
--rw-r--r--   0 runner    (1001) docker     (127)      147 2024-03-20 16:49:52.000000 igor2-0.5.5/igor2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-03-20 16:49:58.000000 igor2-0.5.5/igor2/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)    31678 2024-03-20 16:49:52.000000 igor2-0.5.5/igor2/binarywave.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 16:49:58.574006 igor2-0.5.5/igor2/cli/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-20 16:49:52.000000 igor2-0.5.5/igor2/cli/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      551 2024-03-20 16:49:52.000000 igor2-0.5.5/igor2/cli/igorbinarywave.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1784 2024-03-20 16:49:52.000000 igor2-0.5.5/igor2/cli/igorpackedexperiment.py
--rw-r--r--   0 runner    (1001) docker     (127)     2804 2024-03-20 16:49:52.000000 igor2-0.5.5/igor2/cli/script.py
--rw-r--r--   0 runner    (1001) docker     (127)     8098 2024-03-20 16:49:52.000000 igor2-0.5.5/igor2/packed.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 16:49:58.578006 igor2-0.5.5/igor2/record/
--rw-r--r--   0 runner    (1001) docker     (127)      703 2024-03-20 16:49:52.000000 igor2-0.5.5/igor2/record/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      813 2024-03-20 16:49:52.000000 igor2-0.5.5/igor2/record/base.py
--rw-r--r--   0 runner    (1001) docker     (127)      125 2024-03-20 16:49:52.000000 igor2-0.5.5/igor2/record/folder.py
--rw-r--r--   0 runner    (1001) docker     (127)      170 2024-03-20 16:49:52.000000 igor2-0.5.5/igor2/record/history.py
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-03-20 16:49:52.000000 igor2-0.5.5/igor2/record/packedfile.py
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-03-20 16:49:52.000000 igor2-0.5.5/igor2/record/procedure.py
--rw-r--r--   0 runner    (1001) docker     (127)    12380 2024-03-20 16:49:52.000000 igor2-0.5.5/igor2/record/variables.py
--rw-r--r--   0 runner    (1001) docker     (127)      338 2024-03-20 16:49:52.000000 igor2-0.5.5/igor2/record/wave.py
--rw-r--r--   0 runner    (1001) docker     (127)    28950 2024-03-20 16:49:52.000000 igor2-0.5.5/igor2/struct.py
--rw-r--r--   0 runner    (1001) docker     (127)     3931 2024-03-20 16:49:52.000000 igor2-0.5.5/igor2/util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 16:49:58.578006 igor2-0.5.5/igor2.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2739 2024-03-20 16:49:58.000000 igor2-0.5.5/igor2.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1147 2024-03-20 16:49:58.000000 igor2-0.5.5/igor2.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-20 16:49:58.000000 igor2-0.5.5/igor2.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      124 2024-03-20 16:49:58.000000 igor2-0.5.5/igor2.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-03-20 16:49:58.000000 igor2-0.5.5/igor2.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-03-20 16:49:58.000000 igor2-0.5.5/igor2.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1169 2024-03-20 16:49:52.000000 igor2-0.5.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-20 16:49:58.578006 igor2-0.5.5/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 16:49:58.578006 igor2-0.5.5/tests/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 16:49:58.578006 igor2-0.5.5/tests/data/
--rw-r--r--   0 runner    (1001) docker     (127)      156 2024-03-20 16:49:52.000000 igor2-0.5.5/tests/data/README
--rw-r--r--   0 runner    (1001) docker     (127)      182 2024-03-20 16:49:52.000000 igor2-0.5.5/tests/data/mac-double.ibw
--rw-r--r--   0 runner    (1001) docker     (127)      422 2024-03-20 16:49:52.000000 igor2-0.5.5/tests/data/mac-textWave.ibw
--rw-r--r--   0 runner    (1001) docker     (127)      177 2024-03-20 16:49:52.000000 igor2-0.5.5/tests/data/mac-version2.ibw
--rw-r--r--   0 runner    (1001) docker     (127)      150 2024-03-20 16:49:52.000000 igor2-0.5.5/tests/data/mac-version3Dependent.ibw
--rw-r--r--   0 runner    (1001) docker     (127)      483 2024-03-20 16:49:52.000000 igor2-0.5.5/tests/data/mac-version5.ibw
--rw-r--r--   0 runner    (1001) docker     (127)      384 2024-03-20 16:49:52.000000 igor2-0.5.5/tests/data/mac-zeroPointWave.ibw
--rw-r--r--   0 runner    (1001) docker     (127)    65987 2024-03-20 16:49:52.000000 igor2-0.5.5/tests/data/polar-graphs-demo.pxp
--rw-r--r--   0 runner    (1001) docker     (127)      182 2024-03-20 16:49:52.000000 igor2-0.5.5/tests/data/win-double.ibw
--rw-r--r--   0 runner    (1001) docker     (127)      422 2024-03-20 16:49:52.000000 igor2-0.5.5/tests/data/win-textWave.ibw
--rw-r--r--   0 runner    (1001) docker     (127)      177 2024-03-20 16:49:52.000000 igor2-0.5.5/tests/data/win-version2.ibw
--rw-r--r--   0 runner    (1001) docker     (127)      483 2024-03-20 16:49:52.000000 igor2-0.5.5/tests/data/win-version5.ibw
--rw-r--r--   0 runner    (1001) docker     (127)      384 2024-03-20 16:49:52.000000 igor2-0.5.5/tests/data/win-zeroPointWave.ibw
--rw-r--r--   0 runner    (1001) docker     (127)     1129 2024-03-20 16:49:52.000000 igor2-0.5.5/tests/helper.py
--rw-r--r--   0 runner    (1001) docker     (127)      305 2024-03-20 16:49:52.000000 igor2-0.5.5/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)    27639 2024-03-20 16:49:52.000000 igor2-0.5.5/tests/test_ibw.py
--rw-r--r--   0 runner    (1001) docker     (127)     7186 2024-03-20 16:49:52.000000 igor2-0.5.5/tests/test_pxp.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 15:25:37.358497 igor2-0.5.6/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 15:25:37.350497 igor2-0.5.6/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 15:25:37.350497 igor2-0.5.6/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      962 2024-04-03 15:25:33.000000 igor2-0.5.6/.github/workflows/check.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      693 2024-04-03 15:25:33.000000 igor2-0.5.6/.github/workflows/deploy_pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      107 2024-04-03 15:25:33.000000 igor2-0.5.6/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      786 2024-04-03 15:25:33.000000 igor2-0.5.6/CHANGELOG
+-rw-r--r--   0 runner    (1001) docker     (127)     7639 2024-04-03 15:25:33.000000 igor2-0.5.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-04-03 15:25:33.000000 igor2-0.5.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2739 2024-04-03 15:25:37.358497 igor2-0.5.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1958 2024-04-03 15:25:33.000000 igor2-0.5.6/Readme.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 15:25:37.350497 igor2-0.5.6/igor2/
+-rw-r--r--   0 runner    (1001) docker     (127)      147 2024-04-03 15:25:33.000000 igor2-0.5.6/igor2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-03 15:25:37.000000 igor2-0.5.6/igor2/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31678 2024-04-03 15:25:33.000000 igor2-0.5.6/igor2/binarywave.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 15:25:37.354497 igor2-0.5.6/igor2/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 15:25:33.000000 igor2-0.5.6/igor2/cli/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      551 2024-04-03 15:25:33.000000 igor2-0.5.6/igor2/cli/igorbinarywave.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1784 2024-04-03 15:25:33.000000 igor2-0.5.6/igor2/cli/igorpackedexperiment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2804 2024-04-03 15:25:33.000000 igor2-0.5.6/igor2/cli/script.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9001 2024-04-03 15:25:33.000000 igor2-0.5.6/igor2/packed.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 15:25:37.354497 igor2-0.5.6/igor2/record/
+-rw-r--r--   0 runner    (1001) docker     (127)      703 2024-04-03 15:25:33.000000 igor2-0.5.6/igor2/record/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      813 2024-04-03 15:25:33.000000 igor2-0.5.6/igor2/record/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      125 2024-04-03 15:25:33.000000 igor2-0.5.6/igor2/record/folder.py
+-rw-r--r--   0 runner    (1001) docker     (127)      170 2024-04-03 15:25:33.000000 igor2-0.5.6/igor2/record/history.py
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-03 15:25:33.000000 igor2-0.5.6/igor2/record/packedfile.py
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-04-03 15:25:33.000000 igor2-0.5.6/igor2/record/procedure.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12380 2024-04-03 15:25:33.000000 igor2-0.5.6/igor2/record/variables.py
+-rw-r--r--   0 runner    (1001) docker     (127)      338 2024-04-03 15:25:33.000000 igor2-0.5.6/igor2/record/wave.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28950 2024-04-03 15:25:33.000000 igor2-0.5.6/igor2/struct.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3931 2024-04-03 15:25:33.000000 igor2-0.5.6/igor2/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 15:25:37.358497 igor2-0.5.6/igor2.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2739 2024-04-03 15:25:37.000000 igor2-0.5.6/igor2.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1179 2024-04-03 15:25:37.000000 igor2-0.5.6/igor2.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 15:25:37.000000 igor2-0.5.6/igor2.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      124 2024-04-03 15:25:37.000000 igor2-0.5.6/igor2.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-04-03 15:25:37.000000 igor2-0.5.6/igor2.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-03 15:25:37.000000 igor2-0.5.6/igor2.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1169 2024-04-03 15:25:33.000000 igor2-0.5.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-03 15:25:37.358497 igor2-0.5.6/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 15:25:37.354497 igor2-0.5.6/tests/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 15:25:37.358497 igor2-0.5.6/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (127)      156 2024-04-03 15:25:33.000000 igor2-0.5.6/tests/data/README
+-rw-r--r--   0 runner    (1001) docker     (127)      182 2024-04-03 15:25:33.000000 igor2-0.5.6/tests/data/mac-double.ibw
+-rw-r--r--   0 runner    (1001) docker     (127)      422 2024-04-03 15:25:33.000000 igor2-0.5.6/tests/data/mac-textWave.ibw
+-rw-r--r--   0 runner    (1001) docker     (127)      177 2024-04-03 15:25:33.000000 igor2-0.5.6/tests/data/mac-version2.ibw
+-rw-r--r--   0 runner    (1001) docker     (127)      150 2024-04-03 15:25:33.000000 igor2-0.5.6/tests/data/mac-version3Dependent.ibw
+-rw-r--r--   0 runner    (1001) docker     (127)      483 2024-04-03 15:25:33.000000 igor2-0.5.6/tests/data/mac-version5.ibw
+-rw-r--r--   0 runner    (1001) docker     (127)      384 2024-04-03 15:25:33.000000 igor2-0.5.6/tests/data/mac-zeroPointWave.ibw
+-rwxr-xr-x   0 runner    (1001) docker     (127)    13138 2024-04-03 15:25:33.000000 igor2-0.5.6/tests/data/packed-byteorder.pxt
+-rw-r--r--   0 runner    (1001) docker     (127)    65987 2024-04-03 15:25:33.000000 igor2-0.5.6/tests/data/polar-graphs-demo.pxp
+-rw-r--r--   0 runner    (1001) docker     (127)      182 2024-04-03 15:25:33.000000 igor2-0.5.6/tests/data/win-double.ibw
+-rw-r--r--   0 runner    (1001) docker     (127)      422 2024-04-03 15:25:33.000000 igor2-0.5.6/tests/data/win-textWave.ibw
+-rw-r--r--   0 runner    (1001) docker     (127)      177 2024-04-03 15:25:33.000000 igor2-0.5.6/tests/data/win-version2.ibw
+-rw-r--r--   0 runner    (1001) docker     (127)      483 2024-04-03 15:25:33.000000 igor2-0.5.6/tests/data/win-version5.ibw
+-rw-r--r--   0 runner    (1001) docker     (127)      384 2024-04-03 15:25:33.000000 igor2-0.5.6/tests/data/win-zeroPointWave.ibw
+-rw-r--r--   0 runner    (1001) docker     (127)     1129 2024-04-03 15:25:33.000000 igor2-0.5.6/tests/helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)      305 2024-04-03 15:25:33.000000 igor2-0.5.6/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27639 2024-04-03 15:25:33.000000 igor2-0.5.6/tests/test_ibw.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8465 2024-04-03 15:25:33.000000 igor2-0.5.6/tests/test_pxp.py
```

### Comparing `igor2-0.5.5/.github/workflows/check.yml` & `igor2-0.5.6/.github/workflows/check.yml`

 * *Files identical despite different names*

### Comparing `igor2-0.5.5/.github/workflows/deploy_pypi.yml` & `igor2-0.5.6/.github/workflows/deploy_pypi.yml`

 * *Files identical despite different names*

### Comparing `igor2-0.5.5/CHANGELOG` & `igor2-0.5.6/CHANGELOG`

 * *Files 22% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+0.5.6
+ - enh: allow specifying the byte order when loading data
 0.5.5
  - docs: fix readme
 0.5.4
  - fix: entrypoints not working (#6, #10)
  - enh: make matplotlib optional for CLI
 0.5.3
  - setup: bump numpy to 1.25.1
```

### Comparing `igor2-0.5.5/LICENSE` & `igor2-0.5.6/LICENSE`

 * *Files identical despite different names*

### Comparing `igor2-0.5.5/PKG-INFO` & `igor2-0.5.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: igor2
-Version: 0.5.5
+Version: 0.5.6
 Summary: interface for reading binary IGOR files
 Author: Paul Kienzle, W. Trevor King, Aurelien Jaquier, Zbigniew Jędrzejewski-Szmek, Paul Müller
 License: GNU Lesser General Public License v3 or later (LGPLv3+)
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 or later (LGPLv3+)
```

### Comparing `igor2-0.5.5/Readme.rst` & `igor2-0.5.6/Readme.rst`

 * *Files identical despite different names*

### Comparing `igor2-0.5.5/igor2/binarywave.py` & `igor2-0.5.6/igor2/binarywave.py`

 * *Files identical despite different names*

### Comparing `igor2-0.5.5/igor2/cli/igorbinarywave.py` & `igor2-0.5.6/igor2/cli/igorbinarywave.py`

 * *Files identical despite different names*

### Comparing `igor2-0.5.5/igor2/cli/igorpackedexperiment.py` & `igor2-0.5.6/igor2/cli/igorpackedexperiment.py`

 * *Files identical despite different names*

### Comparing `igor2-0.5.5/igor2/cli/script.py` & `igor2-0.5.6/igor2/cli/script.py`

 * *Files identical despite different names*

### Comparing `igor2-0.5.5/igor2/packed.py` & `igor2-0.5.6/igor2/packed.py`

 * *Files 13% similar despite different names*

```diff
@@ -39,23 +39,46 @@
 # CR_STR = '\x15'  (\r)
 
 PACKEDRECTYPE_MASK = 0x7FFF  # Record type = (recordType & PACKEDREC_TYPE_MASK)
 SUPERCEDED_MASK = 0x8000  # Bit is set if the record is superceded by
 # a later record in the packed file.
 
 
-def load(filename, strict=True, ignore_unknown=True):
+def load(filename, strict=True, ignore_unknown=True, initial_byte_order=None):
+    """Load a packed experiment file.
+
+    Parameters
+    ----------
+    filename : str or file-like object
+        The path to the file or a file-like object representing the packed
+        experiment file.
+    strict : bool, optional
+        This parameter is ignored. Defaults to True.
+    ignore_unknown : bool, optional
+        If True, ignore unknown record types. Defaults to True.
+    initial_byte_order : str or None, optional
+        The initial byte order to use for unpacking. Must be one of '>', '=',
+        '<'. If None, '=' is used. Defaults to None.
+
+    Returns
+    -------
+    records : list of Record
+        The records in the packed experiment file.
+    filesystem : dict
+        The filesystem structure of the packed experiment file.
+    """
     logger.debug('loading a packed experiment file from {}'.format(filename))
     records = []
     if hasattr(filename, 'read'):
         f = filename  # filename is actually a stream object
     else:
         f = open(filename, 'rb')
     byte_order = None
-    initial_byte_order = '='
+    if initial_byte_order is None:
+        initial_byte_order = '='
     try:
         while True:
             PackedFileRecordHeader.byte_order = initial_byte_order
             PackedFileRecordHeader.setup()
             b = bytes(f.read(PackedFileRecordHeader.size))
             if not b:
                 break
@@ -76,15 +99,16 @@
                     PackedFileRecordHeader.setup()
                     header = PackedFileRecordHeader.unpack_from(b)
                     logger.debug(
                         'reordered version: {}'.format(header['version']))
             data = bytes(f.read(header['numDataBytes']))
             if len(data) < header['numDataBytes']:
                 raise ValueError(
-                    ('not enough data for the next record ({} < {})'
+                    ('not enough data for the next record ({} < {}), '
+                     'try loading with a different initial byte order'
                      ).format(len(b), header['numDataBytes']))
             record_type = _RECORD_TYPE.get(
                 header['recordType'] & PACKEDRECTYPE_MASK, _UnknownRecord)
             logger.debug('the new record has type {} ({}).'.format(
                 record_type, header['recordType']))
             if record_type in [_UnknownRecord, _UnusedRecord
                                ] and not ignore_unknown:
```

### Comparing `igor2-0.5.5/igor2/record/__init__.py` & `igor2-0.5.6/igor2/record/__init__.py`

 * *Files identical despite different names*

### Comparing `igor2-0.5.5/igor2/record/base.py` & `igor2-0.5.6/igor2/record/base.py`

 * *Files identical despite different names*

### Comparing `igor2-0.5.5/igor2/record/variables.py` & `igor2-0.5.6/igor2/record/variables.py`

 * *Files identical despite different names*

### Comparing `igor2-0.5.5/igor2/struct.py` & `igor2-0.5.6/igor2/struct.py`

 * *Files identical despite different names*

### Comparing `igor2-0.5.5/igor2/util.py` & `igor2-0.5.6/igor2/util.py`

 * *Files identical despite different names*

### Comparing `igor2-0.5.5/igor2.egg-info/PKG-INFO` & `igor2-0.5.6/igor2.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: igor2
-Version: 0.5.5
+Version: 0.5.6
 Summary: interface for reading binary IGOR files
 Author: Paul Kienzle, W. Trevor King, Aurelien Jaquier, Zbigniew Jędrzejewski-Szmek, Paul Müller
 License: GNU Lesser General Public License v3 or later (LGPLv3+)
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 or later (LGPLv3+)
```

### Comparing `igor2-0.5.5/igor2.egg-info/SOURCES.txt` & `igor2-0.5.6/igor2.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -37,13 +37,14 @@
 tests/data/README
 tests/data/mac-double.ibw
 tests/data/mac-textWave.ibw
 tests/data/mac-version2.ibw
 tests/data/mac-version3Dependent.ibw
 tests/data/mac-version5.ibw
 tests/data/mac-zeroPointWave.ibw
+tests/data/packed-byteorder.pxt
 tests/data/polar-graphs-demo.pxp
 tests/data/win-double.ibw
 tests/data/win-textWave.ibw
 tests/data/win-version2.ibw
 tests/data/win-version5.ibw
 tests/data/win-zeroPointWave.ibw
```

### Comparing `igor2-0.5.5/pyproject.toml` & `igor2-0.5.6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `igor2-0.5.5/tests/data/polar-graphs-demo.pxp` & `igor2-0.5.6/tests/data/polar-graphs-demo.pxp`

 * *Files identical despite different names*

### Comparing `igor2-0.5.5/tests/helper.py` & `igor2-0.5.6/tests/helper.py`

 * *Files identical despite different names*

### Comparing `igor2-0.5.5/tests/test_ibw.py` & `igor2-0.5.6/tests/test_ibw.py`

 * *Files identical despite different names*

### Comparing `igor2-0.5.5/tests/test_pxp.py` & `igor2-0.5.6/tests/test_pxp.py`

 * *Files 20% similar despite different names*

```diff
@@ -125,7 +125,30 @@
         28.70550728, 28.50283432, 27.68538666, 26.36607552,
         25.73583984, 26.78374672, 28.8236084, 30.36226463,
         30.91939545, 31.22146797, 31.97431755, 32.95656204,
         33.4611969, 33.23248672, 32.3250885, 30.64473915,
         28.72983551, 28.05199242, 29.29024887, 31.3501091,
         32.7331543, 32.87995529, 32.28799438, 31.99738503],
         dtype=np.float32))
+
+
+def test_pxt():
+    data = loadpxp(data_dir / 'packed-byteorder.pxt', initial_byte_order='>')
+    records = data[0]
+    assert len(records) == 2
+    assert records[0].variables == {'version': 2,
+                                    'variables': {
+                                        'var_header': {'numSysVars': 0,
+                                                       'numUserVars': 0,
+                                                       'numUserStrs': 0,
+                                                       'numDependentVars': 0,
+                                                       'numDependentStrs': 0},
+                                        'sysVars': {},
+                                        'userVars': {},
+                                        'userStrs': {},
+                                        'dependentVars': [],
+                                        'dependentStrs': []}}
+    assert np.allclose(records[1].wave['wave']["wData"][:30, 0], np.array(
+        [14603., 13701., 14907., 13795., 14339., 14942., 14984., 14261.,
+         12647., 14242., 14470., 13913., 14158., 14754., 14462., 14346.,
+         14219., 13467., 13595., 14331., 13960., 12934., 12897., 13557.,
+         13105., 12797., 13234., 13053., 13455., 12825.], dtype='>f8'))
```

