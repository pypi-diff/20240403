# Comparing `tmp/gtimelog-0.9.2.tar.gz` & `tmp/gtimelog-0.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/gtimelog-0.9.2.tar", last modified: Sun Sep 28 18:47:38 2014, max compression
+gzip compressed data, was "dist/gtimelog-0.9.3.tar", last modified: Tue Sep 29 07:53:13 2015, max compression
```

## Comparing `gtimelog-0.9.2.tar` & `gtimelog-0.9.3.tar`

### file list

```diff
@@ -1,54 +1,55 @@
-drwxrwxr-x   0 mg        (1000) mg        (1000)        0 2014-09-28 18:47:38.000000 gtimelog-0.9.2/
--rw-r--r--   0 mg        (1000) mg        (1000)      624 2013-12-04 08:55:21.000000 gtimelog-0.9.2/TODO.rst
--rw-r--r--   0 mg        (1000) mg        (1000)      885 2013-12-04 11:11:59.000000 gtimelog-0.9.2/CONTRIBUTORS.rst
--rw-r--r--   0 mg        (1000) mg        (1000)    18026 2013-12-04 10:48:02.000000 gtimelog-0.9.2/COPYING
--rwxr-xr-x   0 mg        (1000) mg        (1000)      237 2013-12-04 09:23:05.000000 gtimelog-0.9.2/gtimelog
--rw-r--r--   0 mg        (1000) mg        (1000)      122 2013-12-04 06:57:08.000000 gtimelog-0.9.2/.coveragerc
--rwxr-xr-x   0 mg        (1000) mg        (1000)      231 2014-02-01 12:21:41.000000 gtimelog-0.9.2/runtests
--rw-r--r--   0 mg        (1000) mg        (1000)      313 2013-12-04 11:14:38.000000 gtimelog-0.9.2/MANIFEST.in
--rw-rw-r--   0 mg        (1000) mg        (1000)     2119 2014-09-28 18:46:17.000000 gtimelog-0.9.2/README.rst
--rw-r--r--   0 mg        (1000) mg        (1000)     9601 2013-12-23 13:32:43.000000 gtimelog-0.9.2/gtimelogrc.rst
--rw-rw-r--   0 mg        (1000) mg        (1000)      213 2014-09-28 18:46:17.000000 gtimelog-0.9.2/tox.ini
--rwxrwxr-x   0 mg        (1000) mg        (1000)     2007 2014-09-28 18:46:17.000000 gtimelog-0.9.2/setup.py
--rw-rw-r--   0 mg        (1000) mg        (1000)       59 2014-09-28 18:47:38.000000 gtimelog-0.9.2/setup.cfg
--rw-rw-r--   0 mg        (1000) mg        (1000)     4625 2014-09-28 18:47:38.000000 gtimelog-0.9.2/PKG-INFO
-drwxrwxr-x   0 mg        (1000) mg        (1000)        0 2014-09-28 18:47:38.000000 gtimelog-0.9.2/scripts/
--rwxr-xr-x   0 mg        (1000) mg        (1000)     4221 2013-11-27 08:21:52.000000 gtimelog-0.9.2/scripts/today.py
--rwxr-xr-x   0 mg        (1000) mg        (1000)      825 2013-11-27 08:21:52.000000 gtimelog-0.9.2/scripts/sum.py
--rw-r--r--   0 mg        (1000) mg        (1000)     1343 2013-12-04 09:58:41.000000 gtimelog-0.9.2/scripts/README.rst
--rwxr-xr-x   0 mg        (1000) mg        (1000)      720 2013-11-27 08:21:52.000000 gtimelog-0.9.2/scripts/difftime.py
--rwxr-xr-x   0 mg        (1000) mg        (1000)      411 2013-11-27 08:21:52.000000 gtimelog-0.9.2/scripts/timelog.py
--rwxr-xr-x   0 mg        (1000) mg        (1000)     1460 2013-11-27 08:21:52.000000 gtimelog-0.9.2/scripts/workdays.py
--rw-r--r--   0 mg        (1000) mg        (1000)      666 2013-11-27 08:21:52.000000 gtimelog-0.9.2/scripts/export-my-calendar.py
--rw-rw-r--   0 mg        (1000) mg        (1000)     4992 2014-09-28 18:46:17.000000 gtimelog-0.9.2/gtimelog.rst
-drwxrwxr-x   0 mg        (1000) mg        (1000)        0 2014-09-28 18:47:38.000000 gtimelog-0.9.2/docs/
--rw-r--r--   0 mg        (1000) mg        (1000)     2692 2013-12-07 09:01:14.000000 gtimelog-0.9.2/docs/formats.rst
--rw-rw-r--   0 mg        (1000) mg        (1000)     6153 2014-09-28 18:46:17.000000 gtimelog-0.9.2/docs/index.rst
--rw-r--r--   0 mg        (1000) mg        (1000)    48950 2013-12-04 09:27:58.000000 gtimelog-0.9.2/docs/gtimelog.png
-drwxrwxr-x   0 mg        (1000) mg        (1000)        0 2014-09-28 18:47:38.000000 gtimelog-0.9.2/src/
-drwxrwxr-x   0 mg        (1000) mg        (1000)        0 2014-09-28 18:47:38.000000 gtimelog-0.9.2/src/gtimelog/
--rw-rw-r--   0 mg        (1000) mg        (1000)     6011 2014-09-28 10:53:55.000000 gtimelog-0.9.2/src/gtimelog/settings.py
--rw-rw-r--   0 mg        (1000) mg        (1000)    54303 2014-09-28 18:46:17.000000 gtimelog-0.9.2/src/gtimelog/main.py
--rw-r--r--   0 mg        (1000) mg        (1000)     1239 2013-11-27 08:21:52.000000 gtimelog-0.9.2/src/gtimelog/gtimelog-small-bright.png
--rw-rw-r--   0 mg        (1000) mg        (1000)    34215 2014-09-28 18:46:17.000000 gtimelog-0.9.2/src/gtimelog/tests.py
--rw-rw-r--   0 mg        (1000) mg        (1000)       47 2014-09-28 18:46:32.000000 gtimelog-0.9.2/src/gtimelog/__init__.py
--rw-r--r--   0 mg        (1000) mg        (1000)   134918 2013-11-27 08:21:52.000000 gtimelog-0.9.2/src/gtimelog/gtimelog-large.png
--rw-rw-r--   0 mg        (1000) mg        (1000)    49038 2014-09-28 10:46:40.000000 gtimelog-0.9.2/src/gtimelog/gtimelog.ui
--rw-rw-r--   0 mg        (1000) mg        (1000)    34528 2014-09-28 18:46:17.000000 gtimelog-0.9.2/src/gtimelog/timelog.py
--rw-r--r--   0 mg        (1000) mg        (1000)     1919 2013-11-27 08:21:52.000000 gtimelog-0.9.2/src/gtimelog/gtimelog-small.png
--rw-r--r--   0 mg        (1000) mg        (1000)     7527 2013-11-27 08:21:52.000000 gtimelog-0.9.2/src/gtimelog/gtimelog.png
--rw-r--r--   0 mg        (1000) mg        (1000)     2448 2013-12-23 13:35:22.000000 gtimelog-0.9.2/Makefile
--rw-rw-r--   0 mg        (1000) mg        (1000)     1128 2014-09-28 18:46:17.000000 gtimelog-0.9.2/gtimelogrc.example
--rw-r--r--   0 mg        (1000) mg        (1000)      348 2013-11-28 09:11:38.000000 gtimelog-0.9.2/NOTES.rst
--rw-rw-r--   0 mg        (1000) mg        (1000)      119 2014-09-28 18:46:17.000000 gtimelog-0.9.2/.gitignore
-drwxrwxr-x   0 mg        (1000) mg        (1000)        0 2014-09-28 18:47:38.000000 gtimelog-0.9.2/gtimelog.egg-info/
--rw-r--r--   0 mg        (1000) mg        (1000)        1 2014-09-28 18:47:38.000000 gtimelog-0.9.2/gtimelog.egg-info/dependency_links.txt
--rw-r--r--   0 mg        (1000) mg        (1000)       57 2014-09-28 18:47:38.000000 gtimelog-0.9.2/gtimelog.egg-info/entry_points.txt
--rw-r--r--   0 mg        (1000) mg        (1000)     4625 2014-09-28 18:47:38.000000 gtimelog-0.9.2/gtimelog.egg-info/PKG-INFO
--rw-r--r--   0 mg        (1000) mg        (1000)        1 2013-12-07 14:54:26.000000 gtimelog-0.9.2/gtimelog.egg-info/not-zip-safe
--rw-r--r--   0 mg        (1000) mg        (1000)      890 2014-09-28 18:47:38.000000 gtimelog-0.9.2/gtimelog.egg-info/SOURCES.txt
--rw-r--r--   0 mg        (1000) mg        (1000)        9 2014-09-28 18:47:38.000000 gtimelog-0.9.2/gtimelog.egg-info/top_level.txt
--rw-r--r--   0 mg        (1000) mg        (1000)      194 2013-12-04 11:25:28.000000 gtimelog-0.9.2/gtimelog.desktop
--rw-rw-r--   0 mg        (1000) mg        (1000)      957 2014-09-28 18:46:17.000000 gtimelog-0.9.2/CONTRIBUTING.rst
--rw-rw-r--   0 mg        (1000) mg        (1000)      167 2014-09-28 18:46:17.000000 gtimelog-0.9.2/.travis.yml
--rw-rw-r--   0 mg        (1000) mg        (1000)    10786 2014-09-28 18:46:39.000000 gtimelog-0.9.2/NEWS.rst
+drwxrwxr-x   0 mg        (1000) mg        (1000)        0 2015-09-29 07:53:13.000000 gtimelog-0.9.3/
+-rw-r--r--   0 mg        (1000) mg        (1000)      624 2013-12-04 08:55:21.000000 gtimelog-0.9.3/TODO.rst
+-rw-rw-r--   0 mg        (1000) mg        (1000)      885 2015-09-29 07:49:42.000000 gtimelog-0.9.3/CONTRIBUTORS.rst
+-rw-r--r--   0 mg        (1000) mg        (1000)    18026 2013-12-04 10:48:02.000000 gtimelog-0.9.3/COPYING
+-rwxrwxr-x   0 mg        (1000) mg        (1000)      237 2015-09-18 06:50:52.000000 gtimelog-0.9.3/gtimelog
+-rw-rw-r--   0 mg        (1000) mg        (1000)      122 2015-09-29 07:50:14.000000 gtimelog-0.9.3/.coveragerc
+-rwxr-xr-x   0 mg        (1000) mg        (1000)      231 2014-02-01 12:21:41.000000 gtimelog-0.9.3/runtests
+-rw-rw-r--   0 mg        (1000) mg        (1000)      313 2015-09-29 07:49:42.000000 gtimelog-0.9.3/MANIFEST.in
+-rw-rw-r--   0 mg        (1000) mg        (1000)     2119 2015-09-29 07:50:14.000000 gtimelog-0.9.3/README.rst
+-rw-rw-r--   0 mg        (1000) mg        (1000)     9601 2015-09-29 07:50:14.000000 gtimelog-0.9.3/gtimelogrc.rst
+-rw-rw-r--   0 mg        (1000) mg        (1000)      223 2015-09-29 07:51:48.000000 gtimelog-0.9.3/tox.ini
+-rwxrwxr-x   0 mg        (1000) mg        (1000)     2105 2015-09-29 07:51:35.000000 gtimelog-0.9.3/setup.py
+-rw-rw-r--   0 mg        (1000) mg        (1000)       59 2015-09-29 07:53:13.000000 gtimelog-0.9.3/setup.cfg
+-rw-rw-r--   0 mg        (1000) mg        (1000)     4751 2015-09-29 07:53:13.000000 gtimelog-0.9.3/PKG-INFO
+drwxrwxr-x   0 mg        (1000) mg        (1000)        0 2015-09-29 07:53:13.000000 gtimelog-0.9.3/scripts/
+-rwxr-xr-x   0 mg        (1000) mg        (1000)     4221 2013-11-27 08:21:52.000000 gtimelog-0.9.3/scripts/today.py
+-rwxr-xr-x   0 mg        (1000) mg        (1000)      825 2013-11-27 08:21:52.000000 gtimelog-0.9.3/scripts/sum.py
+-rw-r--r--   0 mg        (1000) mg        (1000)     1343 2013-12-04 09:58:41.000000 gtimelog-0.9.3/scripts/README.rst
+-rwxr-xr-x   0 mg        (1000) mg        (1000)      720 2013-11-27 08:21:52.000000 gtimelog-0.9.3/scripts/difftime.py
+-rwxr-xr-x   0 mg        (1000) mg        (1000)      411 2013-11-27 08:21:52.000000 gtimelog-0.9.3/scripts/timelog.py
+-rwxr-xr-x   0 mg        (1000) mg        (1000)     1460 2013-11-27 08:21:52.000000 gtimelog-0.9.3/scripts/workdays.py
+-rw-r--r--   0 mg        (1000) mg        (1000)      666 2013-11-27 08:21:52.000000 gtimelog-0.9.3/scripts/export-my-calendar.py
+-rw-rw-r--   0 mg        (1000) mg        (1000)     4992 2015-09-29 07:50:14.000000 gtimelog-0.9.3/gtimelog.rst
+drwxrwxr-x   0 mg        (1000) mg        (1000)        0 2015-09-29 07:53:13.000000 gtimelog-0.9.3/docs/
+-rw-rw-r--   0 mg        (1000) mg        (1000)     2692 2015-09-29 07:49:42.000000 gtimelog-0.9.3/docs/formats.rst
+-rw-rw-r--   0 mg        (1000) mg        (1000)     6153 2015-09-29 07:50:14.000000 gtimelog-0.9.3/docs/index.rst
+-rw-rw-r--   0 mg        (1000) mg        (1000)    48950 2015-09-29 07:49:42.000000 gtimelog-0.9.3/docs/gtimelog.png
+drwxrwxr-x   0 mg        (1000) mg        (1000)        0 2015-09-29 07:53:13.000000 gtimelog-0.9.3/src/
+drwxrwxr-x   0 mg        (1000) mg        (1000)        0 2015-09-29 07:53:13.000000 gtimelog-0.9.3/src/gtimelog/
+-rw-rw-r--   0 mg        (1000) mg        (1000)     6011 2015-09-29 07:50:14.000000 gtimelog-0.9.3/src/gtimelog/settings.py
+-rw-rw-r--   0 mg        (1000) mg        (1000)    54303 2015-09-29 07:50:14.000000 gtimelog-0.9.3/src/gtimelog/main.py
+-rw-rw-r--   0 mg        (1000) mg        (1000)     1239 2015-09-29 07:49:42.000000 gtimelog-0.9.3/src/gtimelog/gtimelog-small-bright.png
+-rw-rw-r--   0 mg        (1000) mg        (1000)    34231 2015-09-29 07:50:14.000000 gtimelog-0.9.3/src/gtimelog/tests.py
+-rw-rw-r--   0 mg        (1000) mg        (1000)       47 2015-09-29 07:52:38.000000 gtimelog-0.9.3/src/gtimelog/__init__.py
+-rw-r--r--   0 mg        (1000) mg        (1000)   134918 2013-11-27 08:21:52.000000 gtimelog-0.9.3/src/gtimelog/gtimelog-large.png
+-rw-rw-r--   0 mg        (1000) mg        (1000)    49038 2015-09-29 07:50:14.000000 gtimelog-0.9.3/src/gtimelog/gtimelog.ui
+-rw-rw-r--   0 mg        (1000) mg        (1000)    34696 2015-09-29 07:50:14.000000 gtimelog-0.9.3/src/gtimelog/timelog.py
+-rw-rw-r--   0 mg        (1000) mg        (1000)     1919 2015-09-29 07:49:42.000000 gtimelog-0.9.3/src/gtimelog/gtimelog-small.png
+-rw-r--r--   0 mg        (1000) mg        (1000)     7527 2013-11-27 08:21:52.000000 gtimelog-0.9.3/src/gtimelog/gtimelog.png
+-rw-rw-r--   0 mg        (1000) mg        (1000)     2448 2015-09-29 07:50:14.000000 gtimelog-0.9.3/Makefile
+-rw-rw-r--   0 mg        (1000) mg        (1000)     1128 2015-09-29 07:50:14.000000 gtimelog-0.9.3/gtimelogrc.example
+-rw-rw-r--   0 mg        (1000) mg        (1000)      348 2015-09-29 07:49:42.000000 gtimelog-0.9.3/NOTES.rst
+-rw-rw-r--   0 mg        (1000) mg        (1000)      119 2015-09-29 07:50:14.000000 gtimelog-0.9.3/.gitignore
+drwxrwxr-x   0 mg        (1000) mg        (1000)        0 2015-09-29 07:53:13.000000 gtimelog-0.9.3/gtimelog.egg-info/
+-rw-rw-r--   0 mg        (1000) mg        (1000)        1 2015-09-29 07:53:13.000000 gtimelog-0.9.3/gtimelog.egg-info/dependency_links.txt
+-rw-rw-r--   0 mg        (1000) mg        (1000)       57 2015-09-29 07:53:13.000000 gtimelog-0.9.3/gtimelog.egg-info/entry_points.txt
+-rw-rw-r--   0 mg        (1000) mg        (1000)     4751 2015-09-29 07:53:13.000000 gtimelog-0.9.3/gtimelog.egg-info/PKG-INFO
+-rw-rw-r--   0 mg        (1000) mg        (1000)        1 2015-09-29 07:51:53.000000 gtimelog-0.9.3/gtimelog.egg-info/not-zip-safe
+-rw-rw-r--   0 mg        (1000) mg        (1000)      917 2015-09-29 07:53:13.000000 gtimelog-0.9.3/gtimelog.egg-info/SOURCES.txt
+-rw-rw-r--   0 mg        (1000) mg        (1000)       47 2015-09-29 07:53:13.000000 gtimelog-0.9.3/gtimelog.egg-info/pbr.json
+-rw-rw-r--   0 mg        (1000) mg        (1000)        9 2015-09-29 07:53:13.000000 gtimelog-0.9.3/gtimelog.egg-info/top_level.txt
+-rw-rw-r--   0 mg        (1000) mg        (1000)      194 2015-09-29 07:49:42.000000 gtimelog-0.9.3/gtimelog.desktop
+-rw-rw-r--   0 mg        (1000) mg        (1000)      957 2015-09-29 07:50:14.000000 gtimelog-0.9.3/CONTRIBUTING.rst
+-rw-rw-r--   0 mg        (1000) mg        (1000)      242 2015-09-29 07:50:14.000000 gtimelog-0.9.3/.travis.yml
+-rw-rw-r--   0 mg        (1000) mg        (1000)    10894 2015-09-29 07:50:34.000000 gtimelog-0.9.3/NEWS.rst
```

### Comparing `gtimelog-0.9.2/TODO.rst` & `gtimelog-0.9.3/TODO.rst`

 * *Files identical despite different names*

### Comparing `gtimelog-0.9.2/CONTRIBUTORS.rst` & `gtimelog-0.9.3/CONTRIBUTORS.rst`

 * *Files identical despite different names*

### Comparing `gtimelog-0.9.2/COPYING` & `gtimelog-0.9.3/COPYING`

 * *Files identical despite different names*

### Comparing `gtimelog-0.9.2/README.rst` & `gtimelog-0.9.3/README.rst`

 * *Files identical despite different names*

### Comparing `gtimelog-0.9.2/gtimelogrc.rst` & `gtimelog-0.9.3/gtimelogrc.rst`

 * *Files identical despite different names*

### Comparing `gtimelog-0.9.2/setup.py` & `gtimelog-0.9.3/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -51,14 +51,16 @@
     license='GPL',
     classifiers=[
         'Development Status :: 4 - Beta',
         'Environment :: X11 Applications :: GTK',
         'License :: OSI Approved :: GNU General Public License (GPL)',
         'Programming Language :: Python :: 2.7',
         'Programming Language :: Python :: 3.3',
+        'Programming Language :: Python :: 3.4',
+        'Programming Language :: Python :: 3.5',
         # 2.6 might work, but I can't test it myself -- recent
         # python-gobject versions dropped support for Python 2.6
         'Topic :: Office/Business',
     ],
 
     packages=['gtimelog'],
     package_dir={'gtimelog': 'src/gtimelog'},
```

### Comparing `gtimelog-0.9.2/PKG-INFO` & `gtimelog-0.9.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: gtimelog
-Version: 0.9.2
+Version: 0.9.3
 Summary: A Gtk+ time tracking application
 Home-page: http://mg.pov.lt/gtimelog/
 Author: Marius Gedminas
 Author-email: marius@gedmin.as
 License: GPL
 Description: GTimeLog
         ========
@@ -97,14 +97,20 @@
         .. _CONTRIBUTORS.rst: https://github.com/gtimelog/gtimelog/blob/master/CONTRIBUTORS.rst
         
         
         Changelog
         ---------
         
         
+        0.9.3 (2015-09-29)
+        ~~~~~~~~~~~~~~~~~~
+        
+        * Adding new entries didn't update total weekly numbers (GH: #28).
+        
+        
         0.9.2 (2014-09-28)
         ~~~~~~~~~~~~~~~~~~
         * Fix setup.py to work on Python 3 when your locale is not UTF-8
           (LP: #1263772).
         * Note that Gtk+ 2.x is no longer supported (this regressed somewhere between
           0.9.0 and 0.9.1, but I didn't notice because I have no access to a system
           that has Gtk+ 2.x).
@@ -114,26 +120,23 @@
         * Fix Unicode error when navigating history with PageUp/PageDown (GH: #22).
         * Update current task time when autoreloading (GH: #23).
         * Fix 'LocaleError: unknown encoding:' on Mac OS X (GH: #25).
         * Fix 'TypeError: unorderable types: NoneType() < str()' in summary view
           on Python 3 (GH: #26).
         
         
-        0.9.1 (2013-12-23)
-        ~~~~~~~~~~~~~~~~~~
-        * Manual pages for gtimelog(1) and gtimelogrc(5).
-        
-        
         Older versions
         ~~~~~~~~~~~~~~
         
         See the `full changelog`_.
         
         .. _full changelog: https://github.com/gtimelog/gtimelog/blob/master/NEWS.rst
         
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: X11 Applications :: GTK
 Classifier: License :: OSI Approved :: GNU General Public License (GPL)
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3.3
+Classifier: Programming Language :: Python :: 3.4
+Classifier: Programming Language :: Python :: 3.5
 Classifier: Topic :: Office/Business
```

### Comparing `gtimelog-0.9.2/scripts/today.py` & `gtimelog-0.9.3/scripts/today.py`

 * *Files identical despite different names*

### Comparing `gtimelog-0.9.2/scripts/sum.py` & `gtimelog-0.9.3/scripts/sum.py`

 * *Files identical despite different names*

### Comparing `gtimelog-0.9.2/scripts/README.rst` & `gtimelog-0.9.3/scripts/README.rst`

 * *Files identical despite different names*

### Comparing `gtimelog-0.9.2/scripts/difftime.py` & `gtimelog-0.9.3/scripts/difftime.py`

 * *Files identical despite different names*

### Comparing `gtimelog-0.9.2/scripts/workdays.py` & `gtimelog-0.9.3/scripts/workdays.py`

 * *Files identical despite different names*

### Comparing `gtimelog-0.9.2/scripts/export-my-calendar.py` & `gtimelog-0.9.3/scripts/export-my-calendar.py`

 * *Files identical despite different names*

### Comparing `gtimelog-0.9.2/gtimelog.rst` & `gtimelog-0.9.3/gtimelog.rst`

 * *Files identical despite different names*

### Comparing `gtimelog-0.9.2/docs/formats.rst` & `gtimelog-0.9.3/docs/formats.rst`

 * *Files identical despite different names*

### Comparing `gtimelog-0.9.2/docs/index.rst` & `gtimelog-0.9.3/docs/index.rst`

 * *Files identical despite different names*

### Comparing `gtimelog-0.9.2/docs/gtimelog.png` & `gtimelog-0.9.3/docs/gtimelog.png`

 * *Files identical despite different names*

### Comparing `gtimelog-0.9.2/src/gtimelog/settings.py` & `gtimelog-0.9.3/src/gtimelog/settings.py`

 * *Files identical despite different names*

### Comparing `gtimelog-0.9.2/src/gtimelog/main.py` & `gtimelog-0.9.3/src/gtimelog/main.py`

 * *Files identical despite different names*

### Comparing `gtimelog-0.9.2/src/gtimelog/gtimelog-small-bright.png` & `gtimelog-0.9.3/src/gtimelog/gtimelog-small-bright.png`

 * *Files identical despite different names*

### Comparing `gtimelog-0.9.2/src/gtimelog/tests.py` & `gtimelog-0.9.3/src/gtimelog/tests.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 """Tests for gtimelog"""
 
+import datetime
 import doctest
 import unittest
 import os
 import tempfile
 import shutil
 from pprint import pprint
```

### Comparing `gtimelog-0.9.2/src/gtimelog/gtimelog-large.png` & `gtimelog-0.9.3/src/gtimelog/gtimelog-large.png`

 * *Files identical despite different names*

### Comparing `gtimelog-0.9.2/src/gtimelog/gtimelog.ui` & `gtimelog-0.9.3/src/gtimelog/gtimelog.ui`

 * *Files identical despite different names*

### Comparing `gtimelog-0.9.2/src/gtimelog/timelog.py` & `gtimelog-0.9.3/src/gtimelog/timelog.py`

 * *Files 1% similar despite different names*

```diff
@@ -805,14 +805,17 @@
         last = self.window.last_time()
         if last and different_days(now, last, self.virtual_midnight):
             # next day: reset self.window
             self.reread()
         self.window.items.append((now, entry))
         line = '%s: %s' % (now.strftime("%Y-%m-%d %H:%M"), entry)
         self.raw_append(line)
+        for (min, max), cached in self._cache.items():
+            if cached is not self.window and min <= now < max:
+                cached.items.append((now, entry))
 
     def valid_time(self, time):
         if time > datetime.datetime.now():
             return False
         last = self.window.last_time()
         if last and time < last:
             return False
```

### Comparing `gtimelog-0.9.2/src/gtimelog/gtimelog-small.png` & `gtimelog-0.9.3/src/gtimelog/gtimelog-small.png`

 * *Files identical despite different names*

### Comparing `gtimelog-0.9.2/src/gtimelog/gtimelog.png` & `gtimelog-0.9.3/src/gtimelog/gtimelog.png`

 * *Files identical despite different names*

### Comparing `gtimelog-0.9.2/Makefile` & `gtimelog-0.9.3/Makefile`

 * *Files identical despite different names*

### Comparing `gtimelog-0.9.2/gtimelogrc.example` & `gtimelog-0.9.3/gtimelogrc.example`

 * *Files identical despite different names*

### Comparing `gtimelog-0.9.2/gtimelog.egg-info/PKG-INFO` & `gtimelog-0.9.3/gtimelog.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: gtimelog
-Version: 0.9.2
+Version: 0.9.3
 Summary: A Gtk+ time tracking application
 Home-page: http://mg.pov.lt/gtimelog/
 Author: Marius Gedminas
 Author-email: marius@gedmin.as
 License: GPL
 Description: GTimeLog
         ========
@@ -97,14 +97,20 @@
         .. _CONTRIBUTORS.rst: https://github.com/gtimelog/gtimelog/blob/master/CONTRIBUTORS.rst
         
         
         Changelog
         ---------
         
         
+        0.9.3 (2015-09-29)
+        ~~~~~~~~~~~~~~~~~~
+        
+        * Adding new entries didn't update total weekly numbers (GH: #28).
+        
+        
         0.9.2 (2014-09-28)
         ~~~~~~~~~~~~~~~~~~
         * Fix setup.py to work on Python 3 when your locale is not UTF-8
           (LP: #1263772).
         * Note that Gtk+ 2.x is no longer supported (this regressed somewhere between
           0.9.0 and 0.9.1, but I didn't notice because I have no access to a system
           that has Gtk+ 2.x).
@@ -114,26 +120,23 @@
         * Fix Unicode error when navigating history with PageUp/PageDown (GH: #22).
         * Update current task time when autoreloading (GH: #23).
         * Fix 'LocaleError: unknown encoding:' on Mac OS X (GH: #25).
         * Fix 'TypeError: unorderable types: NoneType() < str()' in summary view
           on Python 3 (GH: #26).
         
         
-        0.9.1 (2013-12-23)
-        ~~~~~~~~~~~~~~~~~~
-        * Manual pages for gtimelog(1) and gtimelogrc(5).
-        
-        
         Older versions
         ~~~~~~~~~~~~~~
         
         See the `full changelog`_.
         
         .. _full changelog: https://github.com/gtimelog/gtimelog/blob/master/NEWS.rst
         
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: X11 Applications :: GTK
 Classifier: License :: OSI Approved :: GNU General Public License (GPL)
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3.3
+Classifier: Programming Language :: Python :: 3.4
+Classifier: Programming Language :: Python :: 3.5
 Classifier: Topic :: Office/Business
```

### Comparing `gtimelog-0.9.2/gtimelog.egg-info/SOURCES.txt` & `gtimelog-0.9.3/gtimelog.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -22,14 +22,15 @@
 docs/gtimelog.png
 docs/index.rst
 gtimelog.egg-info/PKG-INFO
 gtimelog.egg-info/SOURCES.txt
 gtimelog.egg-info/dependency_links.txt
 gtimelog.egg-info/entry_points.txt
 gtimelog.egg-info/not-zip-safe
+gtimelog.egg-info/pbr.json
 gtimelog.egg-info/top_level.txt
 scripts/README.rst
 scripts/difftime.py
 scripts/export-my-calendar.py
 scripts/sum.py
 scripts/timelog.py
 scripts/today.py
```

### Comparing `gtimelog-0.9.2/CONTRIBUTING.rst` & `gtimelog-0.9.3/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `gtimelog-0.9.2/NEWS.rst` & `gtimelog-0.9.3/NEWS.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,17 @@
 Changelog
 ---------
 
 
+0.9.3 (2015-09-29)
+~~~~~~~~~~~~~~~~~~
+
+* Adding new entries didn't update total weekly numbers (GH: #28).
+
+
 0.9.2 (2014-09-28)
 ~~~~~~~~~~~~~~~~~~
 * Fix setup.py to work on Python 3 when your locale is not UTF-8
   (LP: #1263772).
 * Note that Gtk+ 2.x is no longer supported (this regressed somewhere between
   0.9.0 and 0.9.1, but I didn't notice because I have no access to a system
   that has Gtk+ 2.x).
```

