# Comparing `tmp/django-pandas-0.6.6.tar.gz` & `tmp/django-pandas-0.6.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-pandas-0.6.6.tar", last modified: Fri Oct 29 14:27:52 2021, max compression
+gzip compressed data, was "django-pandas-0.6.7.tar", last modified: Wed Apr  3 20:51:05 2024, max compression
```

## Comparing `django-pandas-0.6.6.tar` & `django-pandas-0.6.7.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-29 14:27:52.078688 django-pandas-0.6.6/
--rw-r--r--   0 runner    (1001) docker     (121)     1207 2021-10-29 14:27:38.000000 django-pandas-0.6.6/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (121)     4573 2021-10-29 14:27:38.000000 django-pandas-0.6.6/CHANGES.rst
--rw-r--r--   0 runner    (1001) docker     (121)      889 2021-10-29 14:27:38.000000 django-pandas-0.6.6/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1540 2021-10-29 14:27:38.000000 django-pandas-0.6.6/LICENSE.rst
--rw-r--r--   0 runner    (1001) docker     (121)      210 2021-10-29 14:27:38.000000 django-pandas-0.6.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)    18299 2021-10-29 14:27:52.078688 django-pandas-0.6.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)    12628 2021-10-29 14:27:38.000000 django-pandas-0.6.6/README.rst
--rw-r--r--   0 runner    (1001) docker     (121)     3209 2021-10-29 14:27:38.000000 django-pandas-0.6.6/TODO.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-29 14:27:52.074688 django-pandas-0.6.6/django_pandas/
--rw-r--r--   0 runner    (1001) docker     (121)       22 2021-10-29 14:27:38.000000 django-pandas-0.6.6/django_pandas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     5096 2021-10-29 14:27:38.000000 django-pandas-0.6.6/django_pandas/io.py
--rw-r--r--   0 runner    (1001) docker     (121)    11673 2021-10-29 14:27:38.000000 django-pandas-0.6.6/django_pandas/managers.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-10-29 14:27:38.000000 django-pandas-0.6.6/django_pandas/models.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-29 14:27:52.074688 django-pandas-0.6.6/django_pandas/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-10-29 14:27:38.000000 django-pandas-0.6.6/django_pandas/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     6360 2021-10-29 14:27:38.000000 django-pandas-0.6.6/django_pandas/tests/models.py
--rw-r--r--   0 runner    (1001) docker     (121)     9409 2021-10-29 14:27:38.000000 django-pandas-0.6.6/django_pandas/tests/test_io.py
--rw-r--r--   0 runner    (1001) docker     (121)    14285 2021-10-29 14:27:38.000000 django-pandas-0.6.6/django_pandas/tests/test_manager.py
--rw-r--r--   0 runner    (1001) docker     (121)       51 2021-10-29 14:27:38.000000 django-pandas-0.6.6/django_pandas/tests/tests.py
--rw-r--r--   0 runner    (1001) docker     (121)     2988 2021-10-29 14:27:38.000000 django-pandas-0.6.6/django_pandas/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-29 14:27:52.074688 django-pandas-0.6.6/django_pandas.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)    18299 2021-10-29 14:27:52.000000 django-pandas-0.6.6/django_pandas.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      681 2021-10-29 14:27:52.000000 django-pandas-0.6.6/django_pandas.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-10-29 14:27:52.000000 django-pandas-0.6.6/django_pandas.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-10-29 14:27:51.000000 django-pandas-0.6.6/django_pandas.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)       79 2021-10-29 14:27:52.000000 django-pandas-0.6.6/django_pandas.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       14 2021-10-29 14:27:52.000000 django-pandas-0.6.6/django_pandas.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-29 14:27:52.078688 django-pandas-0.6.6/docs/
--rw-r--r--   0 runner    (1001) docker     (121)     5592 2021-10-29 14:27:38.000000 django-pandas-0.6.6/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (121)     7996 2021-10-29 14:27:38.000000 django-pandas-0.6.6/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (121)       53 2021-10-29 14:27:38.000000 django-pandas-0.6.6/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)     5110 2021-10-29 14:27:38.000000 django-pandas-0.6.6/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-10-29 14:27:38.000000 django-pandas-0.6.6/pyproject.toml
--rwxr-xr-x   0 runner    (1001) docker     (121)     1430 2021-10-29 14:27:38.000000 django-pandas-0.6.6/runtests.py
--rw-r--r--   0 runner    (1001) docker     (121)       38 2021-10-29 14:27:52.078688 django-pandas-0.6.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1613 2021-10-29 14:27:38.000000 django-pandas-0.6.6/setup.py
--rw-r--r--   0 runner    (1001) docker     (121)      810 2021-10-29 14:27:38.000000 django-pandas-0.6.6/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 20:51:05.111927 django-pandas-0.6.7/
+-rw-r--r--   0 runner    (1001) docker     (127)     1252 2024-04-03 20:51:01.000000 django-pandas-0.6.7/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     4794 2024-04-03 20:51:01.000000 django-pandas-0.6.7/CHANGES.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      889 2024-04-03 20:51:01.000000 django-pandas-0.6.7/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1540 2024-04-03 20:51:01.000000 django-pandas-0.6.7/LICENSE.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      210 2024-04-03 20:51:01.000000 django-pandas-0.6.7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    19070 2024-04-03 20:51:05.111927 django-pandas-0.6.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    13018 2024-04-03 20:51:01.000000 django-pandas-0.6.7/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3210 2024-04-03 20:51:01.000000 django-pandas-0.6.7/TODO.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 20:51:05.107927 django-pandas-0.6.7/django_pandas/
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-03 20:51:01.000000 django-pandas-0.6.7/django_pandas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5791 2024-04-03 20:51:01.000000 django-pandas-0.6.7/django_pandas/io.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11677 2024-04-03 20:51:01.000000 django-pandas-0.6.7/django_pandas/managers.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 20:51:01.000000 django-pandas-0.6.7/django_pandas/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 20:51:05.111927 django-pandas-0.6.7/django_pandas/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 20:51:01.000000 django-pandas-0.6.7/django_pandas/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6360 2024-04-03 20:51:01.000000 django-pandas-0.6.7/django_pandas/tests/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9908 2024-04-03 20:51:01.000000 django-pandas-0.6.7/django_pandas/tests/test_io.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15349 2024-04-03 20:51:01.000000 django-pandas-0.6.7/django_pandas/tests/test_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-03 20:51:01.000000 django-pandas-0.6.7/django_pandas/tests/tests.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2954 2024-04-03 20:51:01.000000 django-pandas-0.6.7/django_pandas/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 20:51:05.111927 django-pandas-0.6.7/django_pandas.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    19070 2024-04-03 20:51:05.000000 django-pandas-0.6.7/django_pandas.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      681 2024-04-03 20:51:05.000000 django-pandas-0.6.7/django_pandas.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 20:51:05.000000 django-pandas-0.6.7/django_pandas.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 20:51:04.000000 django-pandas-0.6.7/django_pandas.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-04-03 20:51:05.000000 django-pandas-0.6.7/django_pandas.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-03 20:51:05.000000 django-pandas-0.6.7/django_pandas.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 20:51:05.111927 django-pandas-0.6.7/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     5592 2024-04-03 20:51:01.000000 django-pandas-0.6.7/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)     7996 2024-04-03 20:51:01.000000 django-pandas-0.6.7/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-03 20:51:01.000000 django-pandas-0.6.7/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     5110 2024-04-03 20:51:01.000000 django-pandas-0.6.7/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 20:51:01.000000 django-pandas-0.6.7/pyproject.toml
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1430 2024-04-03 20:51:01.000000 django-pandas-0.6.7/runtests.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-03 20:51:05.111927 django-pandas-0.6.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1614 2024-04-03 20:51:01.000000 django-pandas-0.6.7/setup.py
+-rw-r--r--   0 runner    (1001) docker     (127)      591 2024-04-03 20:51:01.000000 django-pandas-0.6.7/tox.ini
```

### Comparing `django-pandas-0.6.6/AUTHORS.rst` & `django-pandas-0.6.7/AUTHORS.rst`

 * *Files 8% similar despite different names*

```diff
@@ -25,7 +25,8 @@
 - `Hélio Meira Lins <https://github.com/meiralins>`_
 - `@utpyngo <https://github.com/utpyngo>`_
 - `Anthony Monthe <https://github.com/ZuluPro>`_
 - `Vincent Toupet <https://github.com/vtoupet>`_
 - `Anton Ian Sipos <https://github.com/aisipos>`_
 - `Chuan-Jhe Hwong <https://github.com/CJHwong>`_
 - `Thomas Grainger <https://github.com/graingert/>`_
+- `Ryan Smith <https://github.com/bixbyr/>`_
```

### Comparing `django-pandas-0.6.6/CHANGES.rst` & `django-pandas-0.6.7/CHANGES.rst`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,18 @@
 CHANGES
 ========
-0.6.6 (2012-10-27)
+0.6.7 (2024-03-27)
+------------------
+
+Fix several deprecation warnings in pandas 2.1 which became actual errors in 2.2 
+as per `#158`_ (thanks to @bixbyr)
+
+.. _`#158`: https://github.com/chrisdev/django-pandas/pull/158
+
+0.6.6 (2021-10-27)
 ------------------
 The main feature of this is release in the use of a GHA to
 automate the publishing of the package to PYPI as per PR `#146`_
 (again much thanks @graingert). Several other minor issues have also
 been addressed.
 
 .. _`#146`: https://github.com/chrisdev/django-pandas/pull/146
```

### Comparing `django-pandas-0.6.6/CONTRIBUTING.rst` & `django-pandas-0.6.7/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `django-pandas-0.6.6/LICENSE.rst` & `django-pandas-0.6.7/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `django-pandas-0.6.6/PKG-INFO` & `django-pandas-0.6.7/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 Metadata-Version: 2.1
 Name: django-pandas
-Version: 0.6.6
+Version: 0.6.7
 Summary: Tools for working with pydata.pandas in your Django projects
 Home-page: https://github.com/chrisdev/django-pandas/
 Author: Christopher Clarke
 Author-email: cclarke@chrisdev.com
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 2.7
@@ -19,22 +17,27 @@
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Framework :: Django
 Description-Content-Type: text/x-rst
-Provides-Extra: test
 License-File: LICENSE.rst
 License-File: AUTHORS.rst
+Requires-Dist: pandas>=0.14.1
+Requires-Dist: six>=1.15.0
+Provides-Extra: test
+Requires-Dist: pandas>=0.20.1; extra == "test"
+Requires-Dist: coverage==5.4; extra == "test"
+Requires-Dist: semver==2.10.1; extra == "test"
 
 ==============
 Django Pandas
 ==============
-   
+
 .. image:: https://github.com/chrisdev/django-pandas/actions/workflows/test.yml/badge.svg
    :target: https://github.com/chrisdev/django-pandas/actions/workflows/test.yml
 
 .. image:: https://coveralls.io/repos/chrisdev/django-pandas/badge.png?branch=master
    :target: https://coveralls.io/r/chrisdev/django-pandas
 
 Tools for working with `pandas <http://pandas.pydata.org>`_ in your Django
@@ -56,19 +59,25 @@
 * `@henhuy <https://github.com/henhuy>`_
 * `Hélio Meira Lins <https://github.com/meiralins>`_
 * `@utpyngo <https://github.com/utpyngo>`_
 * `Anthony Monthe <https://github.com/ZuluPro>`_
 * `Vincent Toupet <https://github.com/vtoupet>`_
 * `Anton Ian Sipos <https://github.com/aisipos>`_
 * `Thomas Grainger <https://github.com/graingert/>`_
+* `Ryan Smith <https://github.com/bixbyr/>`_
 
 What's New
 ===========
-Version 0.6.5 added support for Pandas >= 1.3
-and fixes a number of other issues.
+This is release facilitates running of test with Python 3.10 and automates
+the publishing of the package to PYPI as per PR `#146`_
+(again much thanks @graingert). As usual we have attempted support legacy
+versions of Python/Django/Pandas and this sometimes results in deperation errors
+being displayed in when test are run. To avoid use `python -Werror runtests.py`
+
+.. _`#146`: https://github.com/chrisdev/django-pandas/pull/146
 
 Dependencies
 =============
 ``django-pandas`` supports `Django`_ (>=1.4.5) or later
 and requires `django-model-utils`_ (>= 1.4.0) and `Pandas`_ (>= 0.12.0).
 **Note** because of problems with the ``requires`` directive of setuptools
 you probably need to install ``numpy`` in your virtualenv  before you install
@@ -434,15 +443,23 @@
 
 
 .. end-here
 
 
 CHANGES
 ========
-0.6.6 (2012-10-27)
+0.6.7 (2024-03-27)
+------------------
+
+Fix several deprecation warnings in pandas 2.1 which became actual errors in 2.2 
+as per `#158`_ (thanks to @bixbyr)
+
+.. _`#158`: https://github.com/chrisdev/django-pandas/pull/158
+
+0.6.6 (2021-10-27)
 ------------------
 The main feature of this is release in the use of a GHA to
 automate the publishing of the package to PYPI as per PR `#146`_
 (again much thanks @graingert). Several other minor issues have also
 been addressed.
 
 .. _`#146`: https://github.com/chrisdev/django-pandas/pull/146
@@ -566,9 +583,7 @@
 - added a Boolean ``verbose`` argument to all methods (which defaults to ``True``)
   This populate the DataFrame columns with the human readable versions of
   foreign key or choice fields.
 - Improved the performance DataFrame creation by removing dependency on
   ``np.core.records.fromrecords``
 - Loads of bug fixes, more tests and improved coverage and better
   documentation
-
-
```

### Comparing `django-pandas-0.6.6/README.rst` & `django-pandas-0.6.7/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ==============
 Django Pandas
 ==============
-   
+
 .. image:: https://github.com/chrisdev/django-pandas/actions/workflows/test.yml/badge.svg
    :target: https://github.com/chrisdev/django-pandas/actions/workflows/test.yml
 
 .. image:: https://coveralls.io/repos/chrisdev/django-pandas/badge.png?branch=master
    :target: https://coveralls.io/r/chrisdev/django-pandas
 
 Tools for working with `pandas <http://pandas.pydata.org>`_ in your Django
@@ -27,19 +27,25 @@
 * `@henhuy <https://github.com/henhuy>`_
 * `Hélio Meira Lins <https://github.com/meiralins>`_
 * `@utpyngo <https://github.com/utpyngo>`_
 * `Anthony Monthe <https://github.com/ZuluPro>`_
 * `Vincent Toupet <https://github.com/vtoupet>`_
 * `Anton Ian Sipos <https://github.com/aisipos>`_
 * `Thomas Grainger <https://github.com/graingert/>`_
+* `Ryan Smith <https://github.com/bixbyr/>`_
 
 What's New
 ===========
-Version 0.6.5 added support for Pandas >= 1.3
-and fixes a number of other issues.
+This is release facilitates running of test with Python 3.10 and automates
+the publishing of the package to PYPI as per PR `#146`_
+(again much thanks @graingert). As usual we have attempted support legacy
+versions of Python/Django/Pandas and this sometimes results in deperation errors
+being displayed in when test are run. To avoid use `python -Werror runtests.py`
+
+.. _`#146`: https://github.com/chrisdev/django-pandas/pull/146
 
 Dependencies
 =============
 ``django-pandas`` supports `Django`_ (>=1.4.5) or later
 and requires `django-model-utils`_ (>= 1.4.0) and `Pandas`_ (>= 0.12.0).
 **Note** because of problems with the ``requires`` directive of setuptools
 you probably need to install ``numpy`` in your virtualenv  before you install
```

### Comparing `django-pandas-0.6.6/TODO.rst` & `django-pandas-0.6.7/TODO.rst`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 ====
 TODO
 ====
 
 - Add coverage and tox and integrate with travis-CL
 - Add to pivot_table method
+
 2013-07-24
 -----------
 - We need to implement the pivot table method
 
 - Can we bypass the ValuesListQuerySet and numpy_fromrecords and just use the
   DatatFrame.from_records with the tuple of sql records
```

### Comparing `django-pandas-0.6.6/django_pandas/io.py` & `django-pandas-0.6.7/django_pandas/io.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-import pandas as pd
-from .utils import update_with_verbose, get_related_model
 import django
+import pandas as pd
 
+from .utils import update_with_verbose, get_related_model
 
 FieldDoesNotExist = (
     django.db.models.fields.FieldDoesNotExist
     if django.VERSION < (1, 8)
     else django.core.exceptions.FieldDoesNotExist
 )
 
@@ -32,15 +32,18 @@
         yield field
 
 
 def is_values_queryset(qs):
     if django.VERSION < (1, 9):  # pragma: no cover
         return isinstance(qs, django.db.models.query.ValuesQuerySet)
     else:
-        return qs._iterable_class == django.db.models.query.ValuesIterable
+        try:
+            return qs._iterable_class == django.db.models.query.ValuesIterable
+        except:
+            return False
 
 
 def read_frame(qs, fieldnames=(), index_col=None, coerce_float=False,
                verbose=True, datetime_index=False, column_names=None):
     """
     Returns a dataframe from a QuerySet
 
@@ -77,15 +80,15 @@
                     DateTimeIndex.
 
     column_names: If not None, use to override the column names in the
                   DateFrame
     """
 
     if fieldnames:
-        fieldnames = pd.unique(fieldnames)
+        fieldnames = pd.unique(pd.Series(fieldnames))
         if index_col is not None and index_col not in fieldnames:
             # Add it to the field names if not already there
             fieldnames = tuple(fieldnames) + (index_col,)
             if column_names:
                 column_names = tuple(column_names) + (index_col,)
         fields = to_fields(qs, fieldnames)
     elif is_values_queryset(qs):
@@ -113,31 +116,56 @@
             [None] * (len(annotation_field_names) + len(extra_field_names))
 
         uniq_fields = set()
         fieldnames, fields = zip(
             *(f for f in zip(fieldnames, fields)
               if f[0] not in uniq_fields and not uniq_fields.add(f[0])))
     else:
-        fields = qs.model._meta.fields
-        fieldnames = [f.name for f in fields]
-        fieldnames += list(qs.query.annotation_select.keys())
+        try:
+            fields = qs.model._meta.fields
+            fieldnames = [f.name for f in fields]
+            fieldnames += list(qs.query.annotation_select.keys())
+        except:
+            pass
 
     if is_values_queryset(qs):
         recs = list(qs)
     else:
-        recs = list(qs.values_list(*fieldnames))
+        try:
+            recs = list(qs.values_list(*fieldnames))
+        except:
+            if fieldnames:
+                recs = [object_to_dict(q, fieldnames) for q in qs]
+            else:
+                recs = [object_to_dict(q) for q in qs]
 
     df = pd.DataFrame.from_records(
         recs,
         columns=column_names if column_names else fieldnames,
         coerce_float=coerce_float
     )
 
     if verbose:
         update_with_verbose(df, fieldnames, fields)
 
     if index_col is not None:
         df.set_index(index_col, inplace=True)
 
     if datetime_index:
-        df.index = pd.to_datetime(df.index, errors="ignore")
+        df.index = pd.to_datetime(df.index)
     return df
+
+
+def object_to_dict(obj, fields: list = None):
+    """
+        Convert obj to a dictionary
+
+        Parameters
+        ----------
+
+        obj: obj to an item of QuerySet
+        fieldnames: reserved fields, default to all fields
+    """
+    if not fields:
+        obj.__dict__.pop('_state')
+        return obj.__dict__
+    return {field: obj.__dict__.get(field) for field in fields}
```

### Comparing `django-pandas-0.6.6/django_pandas/managers.py` & `django-pandas-0.6.7/django_pandas/managers.py`

 * *Files 1% similar despite different names*

```diff
@@ -237,27 +237,27 @@
             else:
                 df = df.pivot(index=index,
                               columns=pivot_columns,
                               values=values)
 
         if freq is not None:
             if agg_kwargs is None:
-                agg_kwargs=dict()
+                agg_kwargs = dict()
             if agg_args is None:
-                agg_args=[]
+                agg_args = []
             df = df.resample(freq, **rs_kwargs).agg(*agg_args, **agg_kwargs)
 
         return df
 
     def to_dataframe(self, fieldnames=(), verbose=True, index=None,
                      coerce_float=False, datetime_index=False):
         """
         Returns a DataFrame from the queryset
 
-        Paramaters
+        Parameters
         -----------
 
         fieldnames:  The model field names(columns) to utilise in creating
                      the DataFrame. You can span a relationships in the usual
                      Django ORM way by using the foreign key field name
                      separated by double underscores and refer to a field
                      in a related model.
```

### Comparing `django-pandas-0.6.6/django_pandas/tests/models.py` & `django-pandas-0.6.7/django_pandas/tests/models.py`

 * *Files identical despite different names*

### Comparing `django-pandas-0.6.6/django_pandas/tests/test_io.py` & `django-pandas-0.6.7/django_pandas/tests/test_io.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from django.core.paginator import Paginator
 from django.test import TestCase
 import django
 from django.db.models import Sum
 import pandas as pd
 import numpy as np
 from .models import (MyModel, Trader, Security, TradeLog, TradeLogNote,
                      MyModelChoice, Portfolio)
@@ -43,14 +44,25 @@
                 for field in MyModel._meta.get_fields()
                 if not (field.many_to_one and field.related_model is None)
             )))
         self.assertEqual(c, len(fields))
         df1 = read_frame(qs, ['col1', 'col2'])
         self.assertEqual(df1.shape, (qs.count(), 2))
 
+    def test_page(self):
+        qs = MyModel.objects.all()
+        qs_list: list = Paginator(qs, 3).page(1).object_list
+        df = read_frame(qs_list, verbose=False)
+        self.assertEqual(list(df.columns),
+                         ['id', 'index_col', 'col1', 'col2', 'col3', 'col4'])
+
+        df = read_frame(qs_list, verbose=False, fieldnames=['col1', 'col2'])
+        self.assertEqual(list(df.columns),
+                         ['col1', 'col2'])
+
     def test_values(self):
         qs = MyModel.objects.all()
         qs = qs.extra(select={"ecol1": "col1+1"})
         qs = qs.values("index_col", "ecol1", "col1")
         qs = qs.annotate(scol1=Sum("col1"))
         df = read_frame(qs)
         self.assertEqual(list(df.columns),
```

### Comparing `django-pandas-0.6.6/django_pandas/tests/test_manager.py` & `django-pandas-0.6.7/django_pandas/tests/test_manager.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,12 +1,16 @@
+from datetime import datetime
+
 from django.test import TestCase
 import pandas as pd
 import numpy as np
 import pickle
 import django
+from pandas.core.indexes.datetimes import bdate_range
+
 from .models import (
     DataFrame, WideTimeSeries, WideTimeSeriesDateField,
     LongTimeSeries, PivotData, Dude, Car, Spot
 )
 try:
     import pandas._testing as tm
 except ImportError:
@@ -64,16 +68,36 @@
     def unpivot(self, frame):
         N, K = frame.shape
         data = {'value': frame.values.ravel('F'),
                 'variable': np.array(frame.columns).repeat(N),
                 'date': np.tile(np.array(frame.index), K)}
         return pd.DataFrame(data, columns=['date', 'variable', 'value'])
 
+    def _makeTimeDataFrame(self, n_rows: int) -> pd.DataFrame:
+        # Beginning in 2.2 pandas._testing.makeTimeDataFrame was removed, however all that is required for the tests
+        # in this module is a dataframe with columns A, B, C, D of random values indexed by a DatetimeIndex.
+        data = {}
+        for c in ['A', 'B', 'C', 'D']:
+            dt = datetime(2000, 1, 1)
+            dr = bdate_range(dt, periods=n_rows, freq='B', name=c)
+            pd.DatetimeIndex(dr, name=c)
+
+            data[c] = pd.Series(
+                np.random.default_rng(2).standard_normal(n_rows),
+                index=pd.DatetimeIndex(dr, name=c),
+                name=c,
+            )
+        return pd.DataFrame(data)
+
     def setUp(self):
-        self.ts = tm.makeTimeDataFrame(100)
+        if PANDAS_VERSIONINFO >= '2.2.0':
+            self.ts = self._makeTimeDataFrame(100)
+        else:
+            self.ts = tm.makeTimeDataFrame(100)
+
         self.ts2 = self.unpivot(self.ts).set_index('date')
         self.ts.columns = ['col1', 'col2', 'col3', 'col4']
         create_list = []
         for ix, cols in self.ts.iterrows():
             create_list.append(WideTimeSeries(date_ix=ix, col1=cols['col1'],
                                               col2=cols['col2'],
                                               col3=cols['col3'],
@@ -83,17 +107,17 @@
         for ix, cols in self.ts.iterrows():
             create_list.append(WideTimeSeriesDateField(date_ix=ix, col1=cols['col1'],
                                                        col2=cols['col2'],
                                                        col3=cols['col3'],
                                                        col4=cols['col4']))
         WideTimeSeriesDateField.objects.bulk_create(create_list)
 
-        create_list = [LongTimeSeries(date_ix=r[0], series_name=r[1][0],
-                                      value=r[1][1])
-                       for r in self.ts2.iterrows()]
+        create_list = [LongTimeSeries(date_ix=timestamp, series_name=s.iloc[0],
+                                      value=s.iloc[1])
+                       for timestamp, s in self.ts2.iterrows()]
 
         LongTimeSeries.objects.bulk_create(create_list)
 
     def test_widestorage(self):
 
         qs = WideTimeSeries.objects.all()
 
@@ -121,39 +145,46 @@
 
         self.assertEqual(qs.filter(series_name='A').count(), len(df['A']))
         self.assertIsInstance(df.index, pd.DatetimeIndex)
         self.assertIsNone(df.index.freq)
 
     def test_resampling(self):
         qs = LongTimeSeries.objects.all()
-        rs_kwargs = {'kind': 'period'}
         agg_args = None
         agg_kwargs = None
         if PANDAS_VERSIONINFO >= '0.25.0':
             agg_kwargs = {'func': 'sum'}
         else:
-            agg_args= ['sum']
+            agg_args = ['sum']
+
+        if PANDAS_VERSIONINFO >= '2.2.0':
+            freq = 'ME'
+        else:
+            freq = 'M'
+
         df = qs.to_timeseries(index='date_ix', pivot_columns='series_name',
                               values='value', storage='long',
-                              freq='M', rs_kwargs=rs_kwargs,
+                              freq=freq,
                               agg_args=agg_args,
                               agg_kwargs=agg_kwargs)
+        df.index = pd.PeriodIndex(df.index)
 
         self.assertEqual([d.month for d in qs.dates('date_ix', 'month')],
                          df.index.month.tolist())
 
         self.assertIsInstance(df.index, pd.PeriodIndex)
         #try on a  wide time seriesd
 
         qs2 = WideTimeSeries.objects.all()
 
         df1 = qs2.to_timeseries(index='date_ix', storage='wide',
-                                freq='M', rs_kwargs=rs_kwargs,
+                                freq=freq,
                                 agg_args=agg_args,
-                                agg_kwargs = agg_kwargs)
+                                agg_kwargs=agg_kwargs)
+        df1.index = pd.PeriodIndex(df1.index)
 
         self.assertEqual([d.month for d in qs.dates('date_ix', 'month')],
                          df1.index.month.tolist())
 
         self.assertIsInstance(df1.index, pd.PeriodIndex)
 
     def test_bad_args_wide_ts(self):
@@ -218,19 +249,18 @@
                                                 'shiny', 'dull',
                                                 'dull', 'shiny',
                                                 'shiny', 'dull',
                                                 'shiny', 'shiny', 'shiny'],
                                   'value_col_d': np.random.randn(11),
                                   'value_col_e': np.random.randn(11),
                                   'value_col_f': np.random.randn(11)})
-
-        create_list = [PivotData(row_col_a=r[1][0], row_col_b=r[1][1],
-                                 row_col_c=r[1][2], value_col_d=r[1][3],
-                                 value_col_e=r[1][4], value_col_f=r[1][5])
-                       for r in self.data.iterrows()]
+        create_list = [PivotData(row_col_a=r.iloc[0], row_col_b=r.iloc[1],
+                                 row_col_c=r.iloc[2], value_col_d=r.iloc[3],
+                                 value_col_e=r.iloc[4], value_col_f=r.iloc[5])
+                       for _, r in self.data.iterrows()]
 
         PivotData.objects.bulk_create(create_list)
 
     def test_pivot(self):
         qs = PivotData.objects.all()
         rows = ['row_col_a', 'row_col_b']
         cols = ['row_col_c']
```

### Comparing `django-pandas-0.6.6/django_pandas/utils.py` & `django-pandas-0.6.7/django_pandas/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -44,16 +44,15 @@
     base_cache_key = get_base_cache_key(model)
 
     def get_cache_key_from_pk(pk):
         return None if pk is None else base_cache_key % str(pk)
 
     def inner(pk_series):
         pk_series = pk_series.astype(object).where(pk_series.notnull(), None)
-        cache_keys = pk_series.apply(
-            get_cache_key_from_pk, convert_dtype=False)
+        cache_keys = pk_series.apply(get_cache_key_from_pk)
         unique_cache_keys = list(filter(None, cache_keys.unique()))
 
         if not unique_cache_keys:
             return pk_series
 
         out_dict = cache.get_many(unique_cache_keys)
```

### Comparing `django-pandas-0.6.6/django_pandas.egg-info/PKG-INFO` & `django-pandas-0.6.7/django_pandas.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 Metadata-Version: 2.1
 Name: django-pandas
-Version: 0.6.6
+Version: 0.6.7
 Summary: Tools for working with pydata.pandas in your Django projects
 Home-page: https://github.com/chrisdev/django-pandas/
 Author: Christopher Clarke
 Author-email: cclarke@chrisdev.com
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 2.7
@@ -19,22 +17,27 @@
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Framework :: Django
 Description-Content-Type: text/x-rst
-Provides-Extra: test
 License-File: LICENSE.rst
 License-File: AUTHORS.rst
+Requires-Dist: pandas>=0.14.1
+Requires-Dist: six>=1.15.0
+Provides-Extra: test
+Requires-Dist: pandas>=0.20.1; extra == "test"
+Requires-Dist: coverage==5.4; extra == "test"
+Requires-Dist: semver==2.10.1; extra == "test"
 
 ==============
 Django Pandas
 ==============
-   
+
 .. image:: https://github.com/chrisdev/django-pandas/actions/workflows/test.yml/badge.svg
    :target: https://github.com/chrisdev/django-pandas/actions/workflows/test.yml
 
 .. image:: https://coveralls.io/repos/chrisdev/django-pandas/badge.png?branch=master
    :target: https://coveralls.io/r/chrisdev/django-pandas
 
 Tools for working with `pandas <http://pandas.pydata.org>`_ in your Django
@@ -56,19 +59,25 @@
 * `@henhuy <https://github.com/henhuy>`_
 * `Hélio Meira Lins <https://github.com/meiralins>`_
 * `@utpyngo <https://github.com/utpyngo>`_
 * `Anthony Monthe <https://github.com/ZuluPro>`_
 * `Vincent Toupet <https://github.com/vtoupet>`_
 * `Anton Ian Sipos <https://github.com/aisipos>`_
 * `Thomas Grainger <https://github.com/graingert/>`_
+* `Ryan Smith <https://github.com/bixbyr/>`_
 
 What's New
 ===========
-Version 0.6.5 added support for Pandas >= 1.3
-and fixes a number of other issues.
+This is release facilitates running of test with Python 3.10 and automates
+the publishing of the package to PYPI as per PR `#146`_
+(again much thanks @graingert). As usual we have attempted support legacy
+versions of Python/Django/Pandas and this sometimes results in deperation errors
+being displayed in when test are run. To avoid use `python -Werror runtests.py`
+
+.. _`#146`: https://github.com/chrisdev/django-pandas/pull/146
 
 Dependencies
 =============
 ``django-pandas`` supports `Django`_ (>=1.4.5) or later
 and requires `django-model-utils`_ (>= 1.4.0) and `Pandas`_ (>= 0.12.0).
 **Note** because of problems with the ``requires`` directive of setuptools
 you probably need to install ``numpy`` in your virtualenv  before you install
@@ -434,15 +443,23 @@
 
 
 .. end-here
 
 
 CHANGES
 ========
-0.6.6 (2012-10-27)
+0.6.7 (2024-03-27)
+------------------
+
+Fix several deprecation warnings in pandas 2.1 which became actual errors in 2.2 
+as per `#158`_ (thanks to @bixbyr)
+
+.. _`#158`: https://github.com/chrisdev/django-pandas/pull/158
+
+0.6.6 (2021-10-27)
 ------------------
 The main feature of this is release in the use of a GHA to
 automate the publishing of the package to PYPI as per PR `#146`_
 (again much thanks @graingert). Several other minor issues have also
 been addressed.
 
 .. _`#146`: https://github.com/chrisdev/django-pandas/pull/146
@@ -566,9 +583,7 @@
 - added a Boolean ``verbose`` argument to all methods (which defaults to ``True``)
   This populate the DataFrame columns with the human readable versions of
   foreign key or choice fields.
 - Improved the performance DataFrame creation by removing dependency on
   ``np.core.records.fromrecords``
 - Loads of bug fixes, more tests and improved coverage and better
   documentation
-
-
```

### Comparing `django-pandas-0.6.6/django_pandas.egg-info/SOURCES.txt` & `django-pandas-0.6.7/django_pandas.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-pandas-0.6.6/docs/Makefile` & `django-pandas-0.6.7/docs/Makefile`

 * *Files identical despite different names*

### Comparing `django-pandas-0.6.6/docs/conf.py` & `django-pandas-0.6.7/docs/conf.py`

 * *Files identical despite different names*

### Comparing `django-pandas-0.6.6/docs/make.bat` & `django-pandas-0.6.7/docs/make.bat`

 * *Files identical despite different names*

### Comparing `django-pandas-0.6.6/runtests.py` & `django-pandas-0.6.7/runtests.py`

 * *Files identical despite different names*

### Comparing `django-pandas-0.6.6/setup.py` & `django-pandas-0.6.7/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 long_description = (
     codecs.open('README.rst', 'r', 'utf-8').read() + '\n\n' +
     codecs.open('CHANGES.rst', 'r', 'utf-8').read()
 )
 MAJOR = 0
 MINOR = 6
-MICRO = 6
+MICRO = 7 
 
 VERSION = '%d.%d.%d' % (MAJOR, MINOR, MICRO)
 
 setup(
     name='django-pandas',
     version=VERSION,
     description='Tools for working with pydata.pandas in your Django projects',
```

