# Comparing `tmp/symlib-1.4.8.tar.gz` & `tmp/symlib-1.4.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "symlib-1.4.8.tar", last modified: Thu Feb 22 20:47:25 2024, max compression
+gzip compressed data, was "symlib-1.4.9.tar", last modified: Fri Feb 23 19:58:41 2024, max compression
```

## Comparing `symlib-1.4.8.tar` & `symlib-1.4.9.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2024-02-22 20:47:25.329473 symlib-1.4.8/
--rw-r--r--   0 phil       (501) staff       (20)     1071 2022-07-08 18:08:58.000000 symlib-1.4.8/LICENSE
--rw-r--r--   0 phil       (501) staff       (20)      762 2024-02-22 20:47:25.329322 symlib-1.4.8/PKG-INFO
--rw-r--r--   0 phil       (501) staff       (20)      260 2022-08-19 20:35:54.000000 symlib-1.4.8/README.md
--rw-r--r--   0 phil       (501) staff       (20)       84 2022-07-08 18:08:58.000000 symlib-1.4.8/pyproject.toml
--rw-r--r--   0 phil       (501) staff       (20)       38 2024-02-22 20:47:25.329508 symlib-1.4.8/setup.cfg
--rw-r--r--   0 phil       (501) staff       (20)      885 2024-02-22 20:47:05.000000 symlib-1.4.8/setup.py
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2024-02-22 20:47:25.328286 symlib-1.4.8/symlib/
--rw-r--r--   0 phil       (501) staff       (20)     2327 2024-01-25 02:25:02.000000 symlib-1.4.8/symlib/__init__.py
--rw-r--r--   0 phil       (501) staff       (20)     7006 2023-07-17 18:12:25.000000 symlib-1.4.8/symlib/file_management.py
--rw-r--r--   0 phil       (501) staff       (20)    63458 2024-02-14 01:50:22.000000 symlib-1.4.8/symlib/lib.py
--rw-r--r--   0 phil       (501) staff       (20)     9008 2023-06-16 17:53:43.000000 symlib-1.4.8/symlib/match.py
--rw-r--r--   0 phil       (501) staff       (20)     2000 2024-02-14 01:50:22.000000 symlib-1.4.8/symlib/sampling.py
--rw-r--r--   0 phil       (501) staff       (20)    45604 2024-02-22 20:46:32.000000 symlib-1.4.8/symlib/star_tagging.py
--rw-r--r--   0 phil       (501) staff       (20)    11570 2024-02-22 04:03:35.000000 symlib-1.4.8/symlib/util.py
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2024-02-22 20:47:25.329146 symlib-1.4.8/symlib.egg-info/
--rw-r--r--   0 phil       (501) staff       (20)      762 2024-02-22 20:47:25.000000 symlib-1.4.8/symlib.egg-info/PKG-INFO
--rw-r--r--   0 phil       (501) staff       (20)      322 2024-02-22 20:47:25.000000 symlib-1.4.8/symlib.egg-info/SOURCES.txt
--rw-r--r--   0 phil       (501) staff       (20)        1 2024-02-22 20:47:25.000000 symlib-1.4.8/symlib.egg-info/dependency_links.txt
--rw-r--r--   0 phil       (501) staff       (20)       41 2024-02-22 20:47:25.000000 symlib-1.4.8/symlib.egg-info/requires.txt
--rw-r--r--   0 phil       (501) staff       (20)        7 2024-02-22 20:47:25.000000 symlib-1.4.8/symlib.egg-info/top_level.txt
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2024-02-23 19:58:41.051522 symlib-1.4.9/
+-rw-r--r--   0 phil       (501) staff       (20)     1071 2022-07-08 18:08:58.000000 symlib-1.4.9/LICENSE
+-rw-r--r--   0 phil       (501) staff       (20)      762 2024-02-23 19:58:41.051281 symlib-1.4.9/PKG-INFO
+-rw-r--r--   0 phil       (501) staff       (20)      260 2022-08-19 20:35:54.000000 symlib-1.4.9/README.md
+-rw-r--r--   0 phil       (501) staff       (20)       84 2022-07-08 18:08:58.000000 symlib-1.4.9/pyproject.toml
+-rw-r--r--   0 phil       (501) staff       (20)       38 2024-02-23 19:58:41.051649 symlib-1.4.9/setup.cfg
+-rw-r--r--   0 phil       (501) staff       (20)      885 2024-02-23 19:58:35.000000 symlib-1.4.9/setup.py
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2024-02-23 19:58:41.042641 symlib-1.4.9/symlib/
+-rw-r--r--   0 phil       (501) staff       (20)     2327 2024-01-25 02:25:02.000000 symlib-1.4.9/symlib/__init__.py
+-rw-r--r--   0 phil       (501) staff       (20)     7006 2023-07-17 18:12:25.000000 symlib-1.4.9/symlib/file_management.py
+-rw-r--r--   0 phil       (501) staff       (20)    63556 2024-02-23 19:58:08.000000 symlib-1.4.9/symlib/lib.py
+-rw-r--r--   0 phil       (501) staff       (20)     9008 2023-06-16 17:53:43.000000 symlib-1.4.9/symlib/match.py
+-rw-r--r--   0 phil       (501) staff       (20)     1956 2024-02-23 19:58:08.000000 symlib-1.4.9/symlib/sampling.py
+-rw-r--r--   0 phil       (501) staff       (20)    45604 2024-02-22 20:46:32.000000 symlib-1.4.9/symlib/star_tagging.py
+-rw-r--r--   0 phil       (501) staff       (20)    11570 2024-02-22 04:03:35.000000 symlib-1.4.9/symlib/util.py
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2024-02-23 19:58:41.050918 symlib-1.4.9/symlib.egg-info/
+-rw-r--r--   0 phil       (501) staff       (20)      762 2024-02-23 19:58:41.000000 symlib-1.4.9/symlib.egg-info/PKG-INFO
+-rw-r--r--   0 phil       (501) staff       (20)      322 2024-02-23 19:58:41.000000 symlib-1.4.9/symlib.egg-info/SOURCES.txt
+-rw-r--r--   0 phil       (501) staff       (20)        1 2024-02-23 19:58:41.000000 symlib-1.4.9/symlib.egg-info/dependency_links.txt
+-rw-r--r--   0 phil       (501) staff       (20)       41 2024-02-23 19:58:41.000000 symlib-1.4.9/symlib.egg-info/requires.txt
+-rw-r--r--   0 phil       (501) staff       (20)        7 2024-02-23 19:58:41.000000 symlib-1.4.9/symlib.egg-info/top_level.txt
```

### Comparing `symlib-1.4.8/LICENSE` & `symlib-1.4.9/LICENSE`

 * *Files identical despite different names*

### Comparing `symlib-1.4.8/PKG-INFO` & `symlib-1.4.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: symlib
-Version: 1.4.8
+Version: 1.4.9
 Summary: A library for working with data from the Symphony and MW-est zoom-in suites.
 Home-page: https://github.com/phil-mansfield/symlib
 Author: Philip Mansfield
 Author-email: mansfield.astro@gmail.com
 Keywords: python
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `symlib-1.4.8/setup.py` & `symlib-1.4.9/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import setuptools
-version = "1.4.8"
+version = "1.4.9"
 
 with open("README.md", "r", encoding="utf-8") as f:
     long_description = f.read()
 
 setuptools.setup(
     name="symlib",
     version=version,
```

### Comparing `symlib-1.4.8/symlib/__init__.py` & `symlib-1.4.9/symlib/__init__.py`

 * *Files identical despite different names*

### Comparing `symlib-1.4.8/symlib/file_management.py` & `symlib-1.4.9/symlib/file_management.py`

 * *Files identical despite different names*

### Comparing `symlib-1.4.8/symlib/lib.py` & `symlib-1.4.9/symlib/lib.py`

 * *Files 1% similar despite different names*

```diff
@@ -635,16 +635,18 @@
         if i == 0: continue
 
         m_snap = merger_snap(central, x[ok], snap[ok])
         m_ratio = mvir[m_snap] / central["mvir"][m_snap]
 
         target = (snap >= m_snap) & s["ok"][i]
 
-        if h["first_infall_snap"][i] == -1: h["first_infall_snap"][i] = m_snap
         h[i]["merger_snap"], h[i]["merger_ratio"] = m_snap, m_ratio
+        if h["merger_snap"][i] == -1:
+            h["merger_snap"][i] = h["first_infall_snap"][i]
+        if h["first_infall_snap"][i] == -1: h["first_infall_snap"][i] = m_snap
         h["first_infall_snap"][i] = min(h["merger_snap"][i],
                                         h["first_infall_snap"][i])
 
         infall_snap = h["first_infall_snap"][i]
         mpeak_infall = np.max(s[i,:infall_snap+1]["mvir"])
         h["mpeak_pre"][i] = mpeak_infall
         h["false_selection"][i] = mpeak_infall < 300*param["mp"]
```

### Comparing `symlib-1.4.8/symlib/match.py` & `symlib-1.4.9/symlib/match.py`

 * *Files identical despite different names*

### Comparing `symlib-1.4.8/symlib/sampling.py` & `symlib-1.4.9/symlib/sampling.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,20 +6,19 @@
 
 class PDF(object):
     def __init__(self, pdf, low, high):
         self.pdf = pdf
 
         x = np.linspace(low, high, 150)
 
-        y_pdf = interpolate.UnivariateSpline(x, pdf(x))
+        y_pdf = interpolate.UnivariateSpline(x, pdf(x), k=1, s=0)
         
         y = np.zeros(len(x))
 
         for i in range(1, len(y)):
-            #y[i] = integrate.quad(pdf, low, x[i])[0]
             y[i] = y_pdf.integral(low, x[i])
             y[i] = max(y[i], y[i-1])
         y /= y[-1]
         
         self.low, self.high = low, high
         self.cdf = interpolate.interp1d(x, y, "linear")
         ok = np.ones(len(x))
```

### Comparing `symlib-1.4.8/symlib/star_tagging.py` & `symlib-1.4.9/symlib/star_tagging.py`

 * *Files identical despite different names*

### Comparing `symlib-1.4.8/symlib/util.py` & `symlib-1.4.9/symlib/util.py`

 * *Files identical despite different names*

### Comparing `symlib-1.4.8/symlib.egg-info/PKG-INFO` & `symlib-1.4.9/symlib.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: symlib
-Version: 1.4.8
+Version: 1.4.9
 Summary: A library for working with data from the Symphony and MW-est zoom-in suites.
 Home-page: https://github.com/phil-mansfield/symlib
 Author: Philip Mansfield
 Author-email: mansfield.astro@gmail.com
 Keywords: python
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

