# Comparing `tmp/xontrib-pipeliner-0.4.2.tar.gz` & `tmp/xontrib-pipeliner-0.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xontrib-pipeliner-0.4.2.tar", last modified: Wed Feb 21 08:54:17 2024, max compression
+gzip compressed data, was "xontrib-pipeliner-0.4.3.tar", last modified: Wed Apr  3 11:30:04 2024, max compression
```

## Comparing `xontrib-pipeliner-0.4.2.tar` & `xontrib-pipeliner-0.4.3.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 08:54:17.414336 xontrib-pipeliner-0.4.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1319 2024-02-21 08:54:05.000000 xontrib-pipeliner-0.4.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-02-21 08:54:05.000000 xontrib-pipeliner-0.4.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     8093 2024-02-21 08:54:17.414336 xontrib-pipeliner-0.4.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     7044 2024-02-21 08:54:05.000000 xontrib-pipeliner-0.4.2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-21 08:54:17.414336 xontrib-pipeliner-0.4.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1506 2024-02-21 08:54:05.000000 xontrib-pipeliner-0.4.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 08:54:17.410336 xontrib-pipeliner-0.4.2/xontrib/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 08:54:17.414336 xontrib-pipeliner-0.4.2/xontrib/pipeliner/
--rw-r--r--   0 runner    (1001) docker     (127)     3961 2024-02-21 08:54:05.000000 xontrib-pipeliner-0.4.2/xontrib/pipeliner/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1296 2024-02-21 08:54:05.000000 xontrib-pipeliner-0.4.2/xontrib/pipeliner/parallel.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 08:54:17.414336 xontrib-pipeliner-0.4.2/xontrib_pipeliner.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     8093 2024-02-21 08:54:17.000000 xontrib-pipeliner-0.4.2/xontrib_pipeliner.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      545 2024-02-21 08:54:17.000000 xontrib-pipeliner-0.4.2/xontrib_pipeliner.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-21 08:54:17.000000 xontrib-pipeliner-0.4.2/xontrib_pipeliner.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-02-21 08:54:17.000000 xontrib-pipeliner-0.4.2/xontrib_pipeliner.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-02-21 08:54:17.000000 xontrib-pipeliner-0.4.2/xontrib_pipeliner.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 08:54:17.414336 xontrib-pipeliner-0.4.2/xontrib_pipeliner_asttokens/
--rw-r--r--   0 runner    (1001) docker     (127)      860 2024-02-21 08:54:05.000000 xontrib-pipeliner-0.4.2/xontrib_pipeliner_asttokens/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8547 2024-02-21 08:54:05.000000 xontrib-pipeliner-0.4.2/xontrib_pipeliner_asttokens/asttokens.py
--rw-r--r--   0 runner    (1001) docker     (127)     2656 2024-02-21 08:54:05.000000 xontrib-pipeliner-0.4.2/xontrib_pipeliner_asttokens/line_numbers.py
--rw-r--r--   0 runner    (1001) docker     (127)    16255 2024-02-21 08:54:05.000000 xontrib-pipeliner-0.4.2/xontrib_pipeliner_asttokens/mark_tokens.py
--rw-r--r--   0 runner    (1001) docker     (127)     9901 2024-02-21 08:54:05.000000 xontrib-pipeliner-0.4.2/xontrib_pipeliner_asttokens/util.py
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-02-21 08:54:05.000000 xontrib-pipeliner-0.4.2/xontrib_pipeliner_asttokens/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 11:30:04.260156 xontrib-pipeliner-0.4.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1319 2024-04-03 11:29:52.000000 xontrib-pipeliner-0.4.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-03 11:29:52.000000 xontrib-pipeliner-0.4.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     8093 2024-04-03 11:30:04.260156 xontrib-pipeliner-0.4.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7044 2024-04-03 11:29:52.000000 xontrib-pipeliner-0.4.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-03 11:30:04.260156 xontrib-pipeliner-0.4.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1506 2024-04-03 11:29:52.000000 xontrib-pipeliner-0.4.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 11:30:04.256156 xontrib-pipeliner-0.4.3/xontrib/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 11:30:04.260156 xontrib-pipeliner-0.4.3/xontrib/pipeliner/
+-rw-r--r--   0 runner    (1001) docker     (127)     4140 2024-04-03 11:29:52.000000 xontrib-pipeliner-0.4.3/xontrib/pipeliner/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1296 2024-04-03 11:29:52.000000 xontrib-pipeliner-0.4.3/xontrib/pipeliner/parallel.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 11:30:04.260156 xontrib-pipeliner-0.4.3/xontrib_pipeliner.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     8093 2024-04-03 11:30:04.000000 xontrib-pipeliner-0.4.3/xontrib_pipeliner.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      545 2024-04-03 11:30:04.000000 xontrib-pipeliner-0.4.3/xontrib_pipeliner.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 11:30:04.000000 xontrib-pipeliner-0.4.3/xontrib_pipeliner.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-03 11:30:04.000000 xontrib-pipeliner-0.4.3/xontrib_pipeliner.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-03 11:30:04.000000 xontrib-pipeliner-0.4.3/xontrib_pipeliner.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 11:30:04.260156 xontrib-pipeliner-0.4.3/xontrib_pipeliner_asttokens/
+-rw-r--r--   0 runner    (1001) docker     (127)      860 2024-04-03 11:29:52.000000 xontrib-pipeliner-0.4.3/xontrib_pipeliner_asttokens/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8547 2024-04-03 11:29:52.000000 xontrib-pipeliner-0.4.3/xontrib_pipeliner_asttokens/asttokens.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2656 2024-04-03 11:29:52.000000 xontrib-pipeliner-0.4.3/xontrib_pipeliner_asttokens/line_numbers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16255 2024-04-03 11:29:52.000000 xontrib-pipeliner-0.4.3/xontrib_pipeliner_asttokens/mark_tokens.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9901 2024-04-03 11:29:52.000000 xontrib-pipeliner-0.4.3/xontrib_pipeliner_asttokens/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-03 11:29:52.000000 xontrib-pipeliner-0.4.3/xontrib_pipeliner_asttokens/version.py
```

### Comparing `xontrib-pipeliner-0.4.2/LICENSE` & `xontrib-pipeliner-0.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `xontrib-pipeliner-0.4.2/PKG-INFO` & `xontrib-pipeliner-0.4.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xontrib-pipeliner
-Version: 0.4.2
+Version: 0.4.3
 Summary: Easily process the lines using pipes in xonsh.
 Home-page: https://github.com/anki-code/xontrib-pipeliner
 Author: anki
 Author-email: author@example.com
 License: BSD
 Project-URL: Documentation, https://github.com/anki-code/xontrib-pipeliner/blob/master/README.md
 Project-URL: Code, https://github.com/anki-code/xontrib-pipeliner
```

### Comparing `xontrib-pipeliner-0.4.2/README.md` & `xontrib-pipeliner-0.4.3/README.md`

 * *Files identical despite different names*

### Comparing `xontrib-pipeliner-0.4.2/setup.py` & `xontrib-pipeliner-0.4.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
     with open('README.md', 'r', encoding='utf-8') as fh:
         long_description = fh.read()
 except (IOError, OSError):
     long_description = ''
 
 setup(
     name='xontrib-pipeliner',
-    version='0.4.2',
+    version='0.4.3',
     license='BSD',
     author='anki',
     author_email='author@example.com',
     description="Easily process the lines using pipes in xonsh.",
     long_description=long_description,
     long_description_content_type='text/markdown',
     python_requires='>=3.6',
```

### Comparing `xontrib-pipeliner-0.4.2/xontrib/pipeliner/__init__.py` & `xontrib-pipeliner-0.4.3/xontrib/pipeliner/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -23,20 +23,24 @@
 }
 
 def _pl(args, stdin, stdout):
     err = False
     if len(args) == 0:
         print('Error: Python code not found', file=sys.stderr)
         err = True
+
+    presets = {**_default_presets, **__xonsh__.env.get('XONTRIB_PIPELINER_PRESETS', {})}
     if err:
-        print('Usage: <command> | <command> | ... | pl "<Python code>"', file=sys.stderr)
-        print('Example: echo "123" | pl "line[::-1]"', file=sys.stderr)
+        print('Usage: <command> | <command> | ... | pl "<Python code or preset name>"\n'
+            + 'Example: echo "123" | pl "line[::-1]"\n'
+            + 'Example: echo " 123 " | pl strip\n'
+            + 'Presets:\n' + '\n'.join(f"  {p}: {repr(v) if type(v) is str else 'func'}" for p,v in presets.items())
+        , file=sys.stderr)
         return
 
-    presets = {**_default_presets, **__xonsh__.env.get('XONTRIB_PIPELINER_PRESETS', {})}
     if args[0] in presets:
         preset = presets[args[0]]
         args = [preset(args[1:])] if callable(preset) else [preset]
     
     fn = eval('lambda line, num:'+args[0], __xonsh__.ctx)
 
     if stdin is None:
```

### Comparing `xontrib-pipeliner-0.4.2/xontrib/pipeliner/parallel.py` & `xontrib-pipeliner-0.4.3/xontrib/pipeliner/parallel.py`

 * *Files identical despite different names*

### Comparing `xontrib-pipeliner-0.4.2/xontrib_pipeliner.egg-info/PKG-INFO` & `xontrib-pipeliner-0.4.3/xontrib_pipeliner.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xontrib-pipeliner
-Version: 0.4.2
+Version: 0.4.3
 Summary: Easily process the lines using pipes in xonsh.
 Home-page: https://github.com/anki-code/xontrib-pipeliner
 Author: anki
 Author-email: author@example.com
 License: BSD
 Project-URL: Documentation, https://github.com/anki-code/xontrib-pipeliner/blob/master/README.md
 Project-URL: Code, https://github.com/anki-code/xontrib-pipeliner
```

### Comparing `xontrib-pipeliner-0.4.2/xontrib_pipeliner.egg-info/SOURCES.txt` & `xontrib-pipeliner-0.4.3/xontrib_pipeliner.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `xontrib-pipeliner-0.4.2/xontrib_pipeliner_asttokens/__init__.py` & `xontrib-pipeliner-0.4.3/xontrib_pipeliner_asttokens/__init__.py`

 * *Files identical despite different names*

### Comparing `xontrib-pipeliner-0.4.2/xontrib_pipeliner_asttokens/asttokens.py` & `xontrib-pipeliner-0.4.3/xontrib_pipeliner_asttokens/asttokens.py`

 * *Files identical despite different names*

### Comparing `xontrib-pipeliner-0.4.2/xontrib_pipeliner_asttokens/line_numbers.py` & `xontrib-pipeliner-0.4.3/xontrib_pipeliner_asttokens/line_numbers.py`

 * *Files identical despite different names*

### Comparing `xontrib-pipeliner-0.4.2/xontrib_pipeliner_asttokens/mark_tokens.py` & `xontrib-pipeliner-0.4.3/xontrib_pipeliner_asttokens/mark_tokens.py`

 * *Files identical despite different names*

### Comparing `xontrib-pipeliner-0.4.2/xontrib_pipeliner_asttokens/util.py` & `xontrib-pipeliner-0.4.3/xontrib_pipeliner_asttokens/util.py`

 * *Files identical despite different names*

