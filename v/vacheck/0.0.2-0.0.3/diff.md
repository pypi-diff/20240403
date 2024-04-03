# Comparing `tmp/vacheck-0.0.2.tar.gz` & `tmp/vacheck-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/Users/thomas.3912/GitHub/vacheck/dist/tmp1bwof211/vacheck-0.0.2.tar", last modified: Mon Nov 14 21:42:40 2022, max compression
+gzip compressed data, was "vacheck-0.0.3.tar", last modified: Wed Apr  3 16:34:45 2024, max compression
```

## Comparing `vacheck-0.0.2.tar` & `vacheck-0.0.3.tar`

### file list

```diff
@@ -1,42 +1,25 @@
-drwxr-xr-x   0 thomas.3912 (1583608718) 444659088        0 2022-11-14 21:42:40.882305 vacheck-0.0.2/
--rw-r--r--   0 thomas.3912 (1583608718) 444659088    35149 2022-06-16 14:06:08.000000 vacheck-0.0.2/LICENSE
--rw-r--r--   0 thomas.3912 (1583608718) 444659088       61 2022-07-25 15:38:35.000000 vacheck-0.0.2/MANIFEST.in
--rw-r--r--   0 thomas.3912 (1583608718) 444659088    11284 2022-11-14 21:42:40.881698 vacheck-0.0.2/PKG-INFO
--rw-r--r--   0 thomas.3912 (1583608718) 444659088    10539 2022-11-14 21:39:32.000000 vacheck-0.0.2/README.md
--rw-r--r--   0 thomas.3912 (1583608718) 444659088       87 2022-07-25 17:47:40.000000 vacheck-0.0.2/pyproject.toml
--rw-r--r--   0 thomas.3912 (1583608718) 444659088       38 2022-11-14 21:42:40.882483 vacheck-0.0.2/setup.cfg
--rw-r--r--   0 thomas.3912 (1583608718) 444659088     1323 2022-11-14 21:39:32.000000 vacheck-0.0.2/setup.py
-drwxr-xr-x   0 thomas.3912 (1583608718) 444659088        0 2022-11-14 21:42:40.851268 vacheck-0.0.2/tests/
--rw-r--r--   0 thomas.3912 (1583608718) 444659088        0 2022-07-22 23:54:37.000000 vacheck-0.0.2/tests/__init__.py
--rw-r--r--   0 thomas.3912 (1583608718) 444659088     2244 2022-06-17 02:31:31.000000 vacheck-0.0.2/tests/interva5_compare.py
--rw-r--r--   0 thomas.3912 (1583608718) 444659088     1696 2022-11-14 21:39:32.000000 vacheck-0.0.2/tests/test_compare_r.py
--rw-r--r--   0 thomas.3912 (1583608718) 444659088     2024 2022-11-14 21:39:32.000000 vacheck-0.0.2/tests/test_datacheck5.py
-drwxr-xr-x   0 thomas.3912 (1583608718) 444659088        0 2022-11-14 21:42:40.853946 vacheck-0.0.2/vacheck/
--rw-r--r--   0 thomas.3912 (1583608718) 444659088        0 2022-06-16 14:06:08.000000 vacheck-0.0.2/vacheck/__init__.py
--rw-r--r--   0 thomas.3912 (1583608718) 444659088      284 2022-11-14 21:39:32.000000 vacheck-0.0.2/vacheck/__version__.py
-drwxr-xr-x   0 thomas.3912 (1583608718) 444659088        0 2022-11-14 21:42:40.857631 vacheck-0.0.2/vacheck/data/
--rw-r--r--   0 thomas.3912 (1583608718) 444659088   125249 2022-06-16 14:06:08.000000 vacheck-0.0.2/vacheck/data/example_input.csv
--rw-r--r--   0 thomas.3912 (1583608718) 444659088   104949 2022-06-16 14:06:08.000000 vacheck-0.0.2/vacheck/data/probbaseV5.csv
--rw-r--r--   0 thomas.3912 (1583608718) 444659088     7526 2022-11-14 21:39:32.000000 vacheck-0.0.2/vacheck/datacheck5.py
--rw-r--r--   0 thomas.3912 (1583608718) 444659088      386 2022-06-16 14:06:08.000000 vacheck-0.0.2/vacheck/exceptions.py
-drwxr-xr-x   0 thomas.3912 (1583608718) 444659088        0 2022-11-14 21:42:40.880426 vacheck-0.0.2/vacheck.egg-info/
--rw-r--r--   0 thomas.3912 (1583608718) 444659088    11284 2022-11-14 21:42:40.000000 vacheck-0.0.2/vacheck.egg-info/PKG-INFO
--rw-r--r--   0 thomas.3912 (1583608718) 444659088     1026 2022-11-14 21:42:40.000000 vacheck-0.0.2/vacheck.egg-info/SOURCES.txt
--rw-r--r--   0 thomas.3912 (1583608718) 444659088        1 2022-11-14 21:42:40.000000 vacheck-0.0.2/vacheck.egg-info/dependency_links.txt
--rw-r--r--   0 thomas.3912 (1583608718) 444659088       13 2022-11-14 21:42:40.000000 vacheck-0.0.2/vacheck.egg-info/requires.txt
--rw-r--r--   0 thomas.3912 (1583608718) 444659088       24 2022-11-14 21:42:40.000000 vacheck-0.0.2/vacheck.egg-info/top_level.txt
-drwxr-xr-x   0 thomas.3912 (1583608718) 444659088        0 2022-11-14 21:42:40.845497 vacheck-0.0.2/venv/
-drwxr-xr-x   0 thomas.3912 (1583608718) 444659088        0 2022-11-14 21:42:40.875083 vacheck-0.0.2/venv/bin/
--rw-r--r--   0 thomas.3912 (1583608718) 444659088     1199 2022-06-16 14:07:32.000000 vacheck-0.0.2/venv/bin/activate_this.py
--rwxr-xr-x   0 thomas.3912 (1583608718) 444659088      626 2022-07-25 18:38:27.000000 vacheck-0.0.2/venv/bin/rst2html.py
--rwxr-xr-x   0 thomas.3912 (1583608718) 444659088      748 2022-07-25 18:38:27.000000 vacheck-0.0.2/venv/bin/rst2html4.py
--rwxr-xr-x   0 thomas.3912 (1583608718) 444659088     1093 2022-07-25 18:38:27.000000 vacheck-0.0.2/venv/bin/rst2html5.py
--rwxr-xr-x   0 thomas.3912 (1583608718) 444659088      825 2022-07-25 18:38:27.000000 vacheck-0.0.2/venv/bin/rst2latex.py
--rwxr-xr-x   0 thomas.3912 (1583608718) 444659088      648 2022-07-25 18:38:27.000000 vacheck-0.0.2/venv/bin/rst2man.py
--rwxr-xr-x   0 thomas.3912 (1583608718) 444659088      814 2022-07-25 18:38:27.000000 vacheck-0.0.2/venv/bin/rst2odt.py
--rwxr-xr-x   0 thomas.3912 (1583608718) 444659088     1752 2022-07-25 18:38:27.000000 vacheck-0.0.2/venv/bin/rst2odt_prepstyles.py
--rwxr-xr-x   0 thomas.3912 (1583608718) 444659088      633 2022-07-25 18:38:27.000000 vacheck-0.0.2/venv/bin/rst2pseudoxml.py
--rwxr-xr-x   0 thomas.3912 (1583608718) 444659088      669 2022-07-25 18:38:27.000000 vacheck-0.0.2/venv/bin/rst2s5.py
--rwxr-xr-x   0 thomas.3912 (1583608718) 444659088      905 2022-07-25 18:38:27.000000 vacheck-0.0.2/venv/bin/rst2xetex.py
--rwxr-xr-x   0 thomas.3912 (1583608718) 444659088      634 2022-07-25 18:38:27.000000 vacheck-0.0.2/venv/bin/rst2xml.py
--rwxr-xr-x   0 thomas.3912 (1583608718) 444659088      702 2022-07-25 18:38:27.000000 vacheck-0.0.2/venv/bin/rstpep2html.py
+drwxr-xr-x   0 thomas.3912 (1583608718) ASC\Domain Users (444659088)        0 2024-04-03 16:34:45.053529 vacheck-0.0.3/
+-rw-r--r--   0 thomas.3912 (1583608718) ASC\Domain Users (444659088)    35149 2022-06-16 14:06:08.000000 vacheck-0.0.3/LICENSE
+-rw-r--r--   0 thomas.3912 (1583608718) ASC\Domain Users (444659088)       61 2022-07-25 15:38:35.000000 vacheck-0.0.3/MANIFEST.in
+-rw-r--r--   0 thomas.3912 (1583608718) ASC\Domain Users (444659088)    11528 2024-04-03 16:34:45.052771 vacheck-0.0.3/PKG-INFO
+-rw-r--r--   0 thomas.3912 (1583608718) ASC\Domain Users (444659088)    10547 2022-11-22 19:28:24.000000 vacheck-0.0.3/README.md
+-rw-r--r--   0 thomas.3912 (1583608718) ASC\Domain Users (444659088)     1302 2024-04-03 16:24:27.000000 vacheck-0.0.3/pyproject.toml
+-rw-r--r--   0 thomas.3912 (1583608718) ASC\Domain Users (444659088)       38 2024-04-03 16:34:45.053631 vacheck-0.0.3/setup.cfg
+-rw-r--r--   0 thomas.3912 (1583608718) ASC\Domain Users (444659088)       38 2024-04-03 16:24:27.000000 vacheck-0.0.3/setup.py
+drwxr-xr-x   0 thomas.3912 (1583608718) ASC\Domain Users (444659088)        0 2024-04-03 16:34:45.040276 vacheck-0.0.3/src/
+drwxr-xr-x   0 thomas.3912 (1583608718) ASC\Domain Users (444659088)        0 2024-04-03 16:34:45.045634 vacheck-0.0.3/src/vacheck/
+-rw-r--r--   0 thomas.3912 (1583608718) ASC\Domain Users (444659088)        0 2024-04-03 16:24:27.000000 vacheck-0.0.3/src/vacheck/__init__.py
+drwxr-xr-x   0 thomas.3912 (1583608718) ASC\Domain Users (444659088)        0 2024-04-03 16:34:45.049810 vacheck-0.0.3/src/vacheck/data/
+-rw-r--r--   0 thomas.3912 (1583608718) ASC\Domain Users (444659088)   125249 2024-04-03 16:24:27.000000 vacheck-0.0.3/src/vacheck/data/example_input.csv
+-rw-r--r--   0 thomas.3912 (1583608718) ASC\Domain Users (444659088)   104949 2024-04-03 16:24:27.000000 vacheck-0.0.3/src/vacheck/data/probbaseV5.csv
+-rw-r--r--   0 thomas.3912 (1583608718) ASC\Domain Users (444659088)     7682 2024-04-03 16:24:27.000000 vacheck-0.0.3/src/vacheck/datacheck5.py
+-rw-r--r--   0 thomas.3912 (1583608718) ASC\Domain Users (444659088)      386 2024-04-03 16:24:27.000000 vacheck-0.0.3/src/vacheck/exceptions.py
+drwxr-xr-x   0 thomas.3912 (1583608718) ASC\Domain Users (444659088)        0 2024-04-03 16:34:45.052067 vacheck-0.0.3/src/vacheck.egg-info/
+-rw-r--r--   0 thomas.3912 (1583608718) ASC\Domain Users (444659088)    11528 2024-04-03 16:34:45.000000 vacheck-0.0.3/src/vacheck.egg-info/PKG-INFO
+-rw-r--r--   0 thomas.3912 (1583608718) ASC\Domain Users (444659088)      419 2024-04-03 16:34:45.000000 vacheck-0.0.3/src/vacheck.egg-info/SOURCES.txt
+-rw-r--r--   0 thomas.3912 (1583608718) ASC\Domain Users (444659088)        1 2024-04-03 16:34:45.000000 vacheck-0.0.3/src/vacheck.egg-info/dependency_links.txt
+-rw-r--r--   0 thomas.3912 (1583608718) ASC\Domain Users (444659088)       13 2024-04-03 16:34:45.000000 vacheck-0.0.3/src/vacheck.egg-info/requires.txt
+-rw-r--r--   0 thomas.3912 (1583608718) ASC\Domain Users (444659088)        8 2024-04-03 16:34:45.000000 vacheck-0.0.3/src/vacheck.egg-info/top_level.txt
+drwxr-xr-x   0 thomas.3912 (1583608718) ASC\Domain Users (444659088)        0 2024-04-03 16:34:45.051127 vacheck-0.0.3/tests/
+-rw-r--r--   0 thomas.3912 (1583608718) ASC\Domain Users (444659088)     1866 2024-04-03 16:24:27.000000 vacheck-0.0.3/tests/test_compare_r.py
+-rw-r--r--   0 thomas.3912 (1583608718) ASC\Domain Users (444659088)     2044 2024-04-03 16:24:27.000000 vacheck-0.0.3/tests/test_datacheck5.py
```

### Comparing `vacheck-0.0.2/LICENSE` & `vacheck-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `vacheck-0.0.2/PKG-INFO` & `vacheck-0.0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,30 @@
 Metadata-Version: 2.1
 Name: vacheck
-Version: 0.0.2
+Version: 0.0.3
 Summary: Verbal autopsy data consistency checks (from InterVA algorithm).
-Home-page: https://github.com/verbal-autopsy-software/vacheck
-Author: Jason Thomas
-Author-email: jarathomas@gmail.com
+Author-email: Jason Thomas <jarathomas@gmail.com>
+Maintainer-email: Jason Thomas <jarathomas@gmail.com>
 License: GPLv3
+Project-URL: Homepage, https://github.com/verbal-autopsy-software/vacheck
+Project-URL: Bug Tracker, https://github.com/verbal-autopsy-software/vacheck/issues
+Keywords: verbal autopsy
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: pandas
+Requires-Dist: numpy
 
 # vacheck
 
 [![image](https://img.shields.io/pypi/pyversions/vacheck)](https://pypi.org/project/vacheck/)
 [![pytest](https://github.com/verbal-autopsy-software/vacheck/actions/workflows/python-package.yml/badge.svg)](https://github.com/verbal-autopsy-software/vacheck/actions)
 
 Data consistency checks for verbal autopsy (VA) data collected using the WHO 
@@ -146,15 +151,15 @@
 * **subst** (column F)
 * **dontask1 - dontask8** (columns H - O)
 * **doaskif** (column P)
 * **nnonly** (column Q)
 
 ```python
 >>> from vacheck.datacheck5 import get_probbase
->>> probbase = get_probbase(keep_nan=True, keep_qdesc=True)
+>>> probbase = get_probbase(replace_nan=False, replace_qdesc=False)
 >>> probbase.iat[0, 2]
 'probbase v18 20200403 '
 >>> probbase.columns
 Index(['indic', 'qdesc', 'sdesc', 'who_2016', 'ilab', 'subst', 'samb',
        'dontask1', 'dontask2', 'dontask3', 'dontask4', 'dontask5', 'dontask6',
        'dontask7', 'dontask8', 'doaskif', 'nnonly', 'a_nrp', 'a_pend_6w',
        'a_preg', 'b_0101', 'b_0102', 'b_0103', 'b_0104', 'b_0105', 'b_0106',
```

### Comparing `vacheck-0.0.2/README.md` & `vacheck-0.0.3/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -127,15 +127,15 @@
 * **subst** (column F)
 * **dontask1 - dontask8** (columns H - O)
 * **doaskif** (column P)
 * **nnonly** (column Q)
 
 ```python
 >>> from vacheck.datacheck5 import get_probbase
->>> probbase = get_probbase(keep_nan=True, keep_qdesc=True)
+>>> probbase = get_probbase(replace_nan=False, replace_qdesc=False)
 >>> probbase.iat[0, 2]
 'probbase v18 20200403 '
 >>> probbase.columns
 Index(['indic', 'qdesc', 'sdesc', 'who_2016', 'ilab', 'subst', 'samb',
        'dontask1', 'dontask2', 'dontask3', 'dontask4', 'dontask5', 'dontask6',
        'dontask7', 'dontask8', 'doaskif', 'nnonly', 'a_nrp', 'a_pend_6w',
        'a_preg', 'b_0101', 'b_0102', 'b_0103', 'b_0104', 'b_0105', 'b_0106',
```

### Comparing `vacheck-0.0.2/tests/test_compare_r.py` & `vacheck-0.0.3/tests/test_compare_r.py`

 * *Files 8% similar despite different names*

```diff
@@ -31,19 +31,25 @@
 ''')
 r_df = robjects.globalenv["r_df"]
 
 with localconverter(robjects.default_converter + pandas2ri.converter):
     r_check = get_conversion().rpy2py(r_df)
     r_data = get_conversion().rpy2py(randomva5)
 
-r_data.replace({"y": 1, "n": 0, ".": nan}, inplace=True)
+for col in r_data:
+    if not (col == "ID"):
+        r_data[col] = r_data[col].cat.rename_categories({"y": 1, "n": 0, ".": 3})
+        r_data[col] = r_data[col].astype("float64")
+        r_data[col] = r_data[col].replace(3, nan)
+
+
 pb = get_probbase()
 py_check = r_data.replace(".", nan).apply(
     lambda x: datacheck5(x, x.ID, probbase=pb)['output'],
     axis=1)
 py_check
-r_check.set_axis(list(py_check), axis=1, inplace=True)
+r_check = r_check.set_axis(list(py_check), axis=1)
 r_check["ID"] = py_check["ID"].copy()
 
 
 def test_r_comparison():
     assert(all(r_check.replace(nan, 2).eq(py_check.replace(nan, 2))))
```

### Comparing `vacheck-0.0.2/tests/test_datacheck5.py` & `vacheck-0.0.3/tests/test_datacheck5.py`

 * *Files 15% similar despite different names*

```diff
@@ -41,25 +41,25 @@
         assert all(self.output_2.isin([self.va_id, 0, 1, 2]))
 
 
 def test_invalid_arg_type(single_record):
     with pytest.raises(exceptions.VAInputException):
         datacheck5(single_record.to_list(), probbase=pb, va_id="d1")
     with pytest.raises(exceptions.VAIDException):
-        single_record[0] = ""
+        single_record.iloc[0] = ""
         datacheck5(single_record, probbase=pb, va_id="")
     with pytest.raises(exceptions.VAInputException):
-        single_record[0] = 3
-        single_record[2] = 3
+        single_record.iloc[0] = 3
+        single_record.iloc[2] = 3
         datacheck5(single_record, probbase=pb, va_id=3)
 
 
 def test_invalid_va_input_data_value(single_record):
     bad_record = single_record
-    bad_record[2] = 33
+    bad_record.iloc[2] = 33
     with pytest.raises(exceptions.VAInputException):
         datacheck5(bad_record, probbase=pb, va_id="d1")
 
 
 def test_invalid_va_input_n_elements(single_record):
     bad_record = single_record
     bad_record.pop("i004a")
```

### Comparing `vacheck-0.0.2/vacheck/data/example_input.csv` & `vacheck-0.0.3/src/vacheck/data/example_input.csv`

 * *Files identical despite different names*

### Comparing `vacheck-0.0.2/vacheck/data/probbaseV5.csv` & `vacheck-0.0.3/src/vacheck/data/probbaseV5.csv`

 * *Files identical despite different names*

### Comparing `vacheck-0.0.2/vacheck/datacheck5.py` & `vacheck-0.0.3/src/vacheck/datacheck5.py`

 * *Files 3% similar despite different names*

```diff
@@ -165,32 +165,36 @@
     """
 
     example_input_bytes = get_data(__name__, "data/example_input.csv")
     example_input = read_csv(BytesIO(example_input_bytes))
     return example_input
 
 
-def get_probbase(keep_nan: bool = False,
-                 keep_qdesc: bool = False) -> numpy.ndarray:
+def get_probbase(drop_prior: bool = True,
+                 replace_nan: bool = True,
+                 replace_qdesc: bool = True) -> numpy.ndarray:
     """
     Get the probbase (the source of the data consistency checks).
 
-    :param keep_nan: Indicator for retaining NaN values (otherwise they
-    are filled in with '.'
-    :type keep_nan: bool
-    :param keep_qdesc: Indicator for retaining the values in the probbase
-    column 'qdesc' be
-    :type keep_qdesc: bool
+    :param drop_prior: Indicator for retaining row with
+    unconditional prior
+    :type drop_prior: bool
+    :param replace_nan: Indicator for replacing NaN values with "."
+    :type replace_nan: bool
+    :param replace_qdesc: Indicator for replacing values in column 'qdesc'
+    with "" (empty strings)
+    :type replace_qdesc: bool
     :return: symptom-cause-information matrix for InterVA5
     :rtype: numpy.array
     """
 
     probbase_bytes = get_data(__name__, "data/probbaseV5.csv")
     probbase = read_csv(BytesIO(probbase_bytes))
     # note: drop first row so it matches the input
-    probbase.drop(index=0, inplace=True)
-    if not keep_nan:
+    if drop_prior:
+        probbase.drop(index=0, inplace=True)
+    if replace_nan:
         probbase.fillna(".", inplace=True)
-    if not keep_qdesc:
+    if replace_qdesc:
         probbase["qdesc"] = ""
     probbase_array = probbase.to_numpy(dtype=str)
     return probbase_array
```

### Comparing `vacheck-0.0.2/vacheck.egg-info/PKG-INFO` & `vacheck-0.0.3/src/vacheck.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,30 @@
 Metadata-Version: 2.1
 Name: vacheck
-Version: 0.0.2
+Version: 0.0.3
 Summary: Verbal autopsy data consistency checks (from InterVA algorithm).
-Home-page: https://github.com/verbal-autopsy-software/vacheck
-Author: Jason Thomas
-Author-email: jarathomas@gmail.com
+Author-email: Jason Thomas <jarathomas@gmail.com>
+Maintainer-email: Jason Thomas <jarathomas@gmail.com>
 License: GPLv3
+Project-URL: Homepage, https://github.com/verbal-autopsy-software/vacheck
+Project-URL: Bug Tracker, https://github.com/verbal-autopsy-software/vacheck/issues
+Keywords: verbal autopsy
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: pandas
+Requires-Dist: numpy
 
 # vacheck
 
 [![image](https://img.shields.io/pypi/pyversions/vacheck)](https://pypi.org/project/vacheck/)
 [![pytest](https://github.com/verbal-autopsy-software/vacheck/actions/workflows/python-package.yml/badge.svg)](https://github.com/verbal-autopsy-software/vacheck/actions)
 
 Data consistency checks for verbal autopsy (VA) data collected using the WHO 
@@ -146,15 +151,15 @@
 * **subst** (column F)
 * **dontask1 - dontask8** (columns H - O)
 * **doaskif** (column P)
 * **nnonly** (column Q)
 
 ```python
 >>> from vacheck.datacheck5 import get_probbase
->>> probbase = get_probbase(keep_nan=True, keep_qdesc=True)
+>>> probbase = get_probbase(replace_nan=False, replace_qdesc=False)
 >>> probbase.iat[0, 2]
 'probbase v18 20200403 '
 >>> probbase.columns
 Index(['indic', 'qdesc', 'sdesc', 'who_2016', 'ilab', 'subst', 'samb',
        'dontask1', 'dontask2', 'dontask3', 'dontask4', 'dontask5', 'dontask6',
        'dontask7', 'dontask8', 'doaskif', 'nnonly', 'a_nrp', 'a_pend_6w',
        'a_preg', 'b_0101', 'b_0102', 'b_0103', 'b_0104', 'b_0105', 'b_0106',
```

