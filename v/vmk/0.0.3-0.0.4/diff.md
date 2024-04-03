# Comparing `tmp/vmk-0.0.3.tar.gz` & `tmp/vmk-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vmk-0.0.3.tar", last modified: Wed Apr  3 20:01:01 2024, max compression
+gzip compressed data, was "vmk-0.0.4.tar", last modified: Wed Apr  3 20:16:29 2024, max compression
```

## Comparing `vmk-0.0.3.tar` & `vmk-0.0.4.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 gabriel    (501) staff       (20)        0 2024-04-03 20:01:01.920856 vmk-0.0.3/
--rw-r--r--   0 gabriel    (501) staff       (20)     1068 2024-04-03 18:00:39.000000 vmk-0.0.3/LICENSE
--rw-r--r--   0 gabriel    (501) staff       (20)      576 2024-04-03 20:01:01.920512 vmk-0.0.3/PKG-INFO
--rw-r--r--   0 gabriel    (501) staff       (20)       41 2024-04-03 17:58:32.000000 vmk-0.0.3/README.md
--rw-r--r--   0 gabriel    (501) staff       (20)      682 2024-04-03 20:00:42.000000 vmk-0.0.3/pyproject.toml
--rw-r--r--   0 gabriel    (501) staff       (20)       38 2024-04-03 20:01:01.920901 vmk-0.0.3/setup.cfg
-drwxr-xr-x   0 gabriel    (501) staff       (20)        0 2024-04-03 20:01:01.911164 vmk-0.0.3/src/
-drwxr-xr-x   0 gabriel    (501) staff       (20)        0 2024-04-03 20:01:01.915238 vmk-0.0.3/src/vmk/
--rw-r--r--   0 gabriel    (501) staff       (20)      909 2024-04-03 19:59:55.000000 vmk-0.0.3/src/vmk/__init__.py
--rw-r--r--   0 gabriel    (501) staff       (20)     1234 2024-04-03 19:33:48.000000 vmk-0.0.3/src/vmk/combiner.py
-drwxr-xr-x   0 gabriel    (501) staff       (20)        0 2024-04-03 20:01:01.920126 vmk-0.0.3/src/vmk.egg-info/
--rw-r--r--   0 gabriel    (501) staff       (20)      576 2024-04-03 20:01:01.000000 vmk-0.0.3/src/vmk.egg-info/PKG-INFO
--rw-r--r--   0 gabriel    (501) staff       (20)      260 2024-04-03 20:01:01.000000 vmk-0.0.3/src/vmk.egg-info/SOURCES.txt
--rw-r--r--   0 gabriel    (501) staff       (20)        1 2024-04-03 20:01:01.000000 vmk-0.0.3/src/vmk.egg-info/dependency_links.txt
--rw-r--r--   0 gabriel    (501) staff       (20)       33 2024-04-03 20:01:01.000000 vmk-0.0.3/src/vmk.egg-info/entry_points.txt
--rw-r--r--   0 gabriel    (501) staff       (20)       14 2024-04-03 20:01:01.000000 vmk-0.0.3/src/vmk.egg-info/requires.txt
--rw-r--r--   0 gabriel    (501) staff       (20)        4 2024-04-03 20:01:01.000000 vmk-0.0.3/src/vmk.egg-info/top_level.txt
+drwxr-xr-x   0 gabriel    (501) staff       (20)        0 2024-04-03 20:16:29.650854 vmk-0.0.4/
+-rw-r--r--   0 gabriel    (501) staff       (20)     1068 2024-04-03 18:00:39.000000 vmk-0.0.4/LICENSE
+-rw-r--r--   0 gabriel    (501) staff       (20)     1391 2024-04-03 20:16:29.650445 vmk-0.0.4/PKG-INFO
+-rw-r--r--   0 gabriel    (501) staff       (20)      856 2024-04-03 20:08:09.000000 vmk-0.0.4/README.md
+-rw-r--r--   0 gabriel    (501) staff       (20)      682 2024-04-03 20:16:10.000000 vmk-0.0.4/pyproject.toml
+-rw-r--r--   0 gabriel    (501) staff       (20)       38 2024-04-03 20:16:29.650910 vmk-0.0.4/setup.cfg
+drwxr-xr-x   0 gabriel    (501) staff       (20)        0 2024-04-03 20:16:29.645076 vmk-0.0.4/src/
+drwxr-xr-x   0 gabriel    (501) staff       (20)        0 2024-04-03 20:16:29.647206 vmk-0.0.4/src/vmk/
+-rw-r--r--   0 gabriel    (501) staff       (20)      898 2024-04-03 20:15:49.000000 vmk-0.0.4/src/vmk/__init__.py
+-rw-r--r--   0 gabriel    (501) staff       (20)     1234 2024-04-03 20:03:49.000000 vmk-0.0.4/src/vmk/combiner.py
+drwxr-xr-x   0 gabriel    (501) staff       (20)        0 2024-04-03 20:16:29.649963 vmk-0.0.4/src/vmk.egg-info/
+-rw-r--r--   0 gabriel    (501) staff       (20)     1391 2024-04-03 20:16:29.000000 vmk-0.0.4/src/vmk.egg-info/PKG-INFO
+-rw-r--r--   0 gabriel    (501) staff       (20)      260 2024-04-03 20:16:29.000000 vmk-0.0.4/src/vmk.egg-info/SOURCES.txt
+-rw-r--r--   0 gabriel    (501) staff       (20)        1 2024-04-03 20:16:29.000000 vmk-0.0.4/src/vmk.egg-info/dependency_links.txt
+-rw-r--r--   0 gabriel    (501) staff       (20)       33 2024-04-03 20:16:29.000000 vmk-0.0.4/src/vmk.egg-info/entry_points.txt
+-rw-r--r--   0 gabriel    (501) staff       (20)       14 2024-04-03 20:16:29.000000 vmk-0.0.4/src/vmk.egg-info/requires.txt
+-rw-r--r--   0 gabriel    (501) staff       (20)        4 2024-04-03 20:16:29.000000 vmk-0.0.4/src/vmk.egg-info/top_level.txt
```

### Comparing `vmk-0.0.3/LICENSE` & `vmk-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `vmk-0.0.3/pyproject.toml` & `vmk-0.0.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "vmk"
-version = "0.0.3"
+version = "0.0.4"
 authors = [
   { name="disk" },
   { name="Vormak" },
 ]
 maintainers = [
   { name="chikorito", email="webmaster@chikorito.land" },
 ]
```

### Comparing `vmk-0.0.3/src/vmk/__init__.py` & `vmk-0.0.4/src/vmk/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 
 parser = argparse.ArgumentParser()
 parser.add_argument('-o', '--out', help="Output file")
 
 input_type = parser.add_mutually_exclusive_group()
 input_type.add_argument('-f', '--files', help="Input files", nargs='+')
-input_type.add_argument('-d', '--dir', help="Input directory", nargs='+')
+input_type.add_argument('-d', '--dir', help="Input directory")
 
 
 def main():
     args = parser.parse_args()
     combiner = Combiner()
     out = args.out or DEFAULT_OUT_FILE
```

### Comparing `vmk-0.0.3/src/vmk/combiner.py` & `vmk-0.0.4/src/vmk/combiner.py`

 * *Files identical despite different names*

