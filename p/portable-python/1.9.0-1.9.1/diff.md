# Comparing `tmp/portable-python-1.9.0.tar.gz` & `tmp/portable-python-1.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "portable-python-1.9.0.tar", last modified: Wed Feb 14 21:57:24 2024, max compression
+gzip compressed data, was "portable-python-1.9.1.tar", last modified: Wed Apr  3 19:52:17 2024, max compression
```

## Comparing `portable-python-1.9.0.tar` & `portable-python-1.9.1.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 21:57:24.028467 portable-python-1.9.0/
--rw-r--r--   0 runner    (1001) docker     (127)     2167 2024-02-14 21:56:46.000000 portable-python-1.9.0/DEVELOP.md
--rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-02-14 21:56:46.000000 portable-python-1.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       99 2024-02-14 21:56:46.000000 portable-python-1.9.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     8583 2024-02-14 21:57:24.028467 portable-python-1.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6912 2024-02-14 21:56:46.000000 portable-python-1.9.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)      289 2024-02-14 21:56:46.000000 portable-python-1.9.0/SECURITY.md
--rw-r--r--   0 runner    (1001) docker     (127)     2098 2024-02-14 21:56:46.000000 portable-python-1.9.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-02-14 21:56:46.000000 portable-python-1.9.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-14 21:57:24.028467 portable-python-1.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1654 2024-02-14 21:56:46.000000 portable-python-1.9.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 21:57:24.024467 portable-python-1.9.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 21:57:24.028467 portable-python-1.9.0/src/portable_python/
--rw-r--r--   0 runner    (1001) docker     (127)    27235 2024-02-14 21:56:46.000000 portable-python-1.9.0/src/portable_python/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      149 2024-02-14 21:56:46.000000 portable-python-1.9.0/src/portable_python/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7488 2024-02-14 21:56:46.000000 portable-python-1.9.0/src/portable_python/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)    13714 2024-02-14 21:56:46.000000 portable-python-1.9.0/src/portable_python/config.py
--rw-r--r--   0 runner    (1001) docker     (127)    16567 2024-02-14 21:56:46.000000 portable-python-1.9.0/src/portable_python/cpython.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 21:57:24.028467 portable-python-1.9.0/src/portable_python/external/
--rw-r--r--   0 runner    (1001) docker     (127)      725 2024-02-14 21:56:46.000000 portable-python-1.9.0/src/portable_python/external/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3715 2024-02-14 21:56:46.000000 portable-python-1.9.0/src/portable_python/external/_inspect.py
--rw-r--r--   0 runner    (1001) docker     (127)     3490 2024-02-14 21:56:46.000000 portable-python-1.9.0/src/portable_python/external/tkinter.py
--rw-r--r--   0 runner    (1001) docker     (127)    10339 2024-02-14 21:56:46.000000 portable-python-1.9.0/src/portable_python/external/xcpython.py
--rw-r--r--   0 runner    (1001) docker     (127)    21349 2024-02-14 21:56:46.000000 portable-python-1.9.0/src/portable_python/inspector.py
--rw-r--r--   0 runner    (1001) docker     (127)     1978 2024-02-14 21:56:46.000000 portable-python-1.9.0/src/portable_python/tracking.py
--rw-r--r--   0 runner    (1001) docker     (127)     7085 2024-02-14 21:56:46.000000 portable-python-1.9.0/src/portable_python/versions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 21:57:24.028467 portable-python-1.9.0/src/portable_python.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     8583 2024-02-14 21:57:23.000000 portable-python-1.9.0/src/portable_python.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      981 2024-02-14 21:57:24.000000 portable-python-1.9.0/src/portable_python.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-14 21:57:23.000000 portable-python-1.9.0/src/portable_python.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-02-14 21:57:23.000000 portable-python-1.9.0/src/portable_python.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-02-14 21:57:23.000000 portable-python-1.9.0/src/portable_python.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-02-14 21:57:23.000000 portable-python-1.9.0/src/portable_python.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 21:57:24.028467 portable-python-1.9.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     4579 2024-02-14 21:56:46.000000 portable-python-1.9.0/tests/test_build.py
--rw-r--r--   0 runner    (1001) docker     (127)     3305 2024-02-14 21:56:46.000000 portable-python-1.9.0/tests/test_cleanup.py
--rw-r--r--   0 runner    (1001) docker     (127)      919 2024-02-14 21:56:46.000000 portable-python-1.9.0/tests/test_failed.py
--rw-r--r--   0 runner    (1001) docker     (127)     8366 2024-02-14 21:56:46.000000 portable-python-1.9.0/tests/test_inspector.py
--rw-r--r--   0 runner    (1001) docker     (127)      625 2024-02-14 21:56:46.000000 portable-python-1.9.0/tests/test_invoker.py
--rw-r--r--   0 runner    (1001) docker     (127)     1573 2024-02-14 21:56:46.000000 portable-python-1.9.0/tests/test_list.py
--rw-r--r--   0 runner    (1001) docker     (127)      711 2024-02-14 21:56:46.000000 portable-python-1.9.0/tests/test_prefix.py
--rw-r--r--   0 runner    (1001) docker     (127)      763 2024-02-14 21:56:46.000000 portable-python-1.9.0/tests/test_recompress.py
--rw-r--r--   0 runner    (1001) docker     (127)      408 2024-02-14 21:56:46.000000 portable-python-1.9.0/tests/test_report.py
--rw-r--r--   0 runner    (1001) docker     (127)     2877 2024-02-14 21:56:46.000000 portable-python-1.9.0/tests/test_setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 19:52:17.250450 portable-python-1.9.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     2167 2024-04-03 19:51:46.000000 portable-python-1.9.1/DEVELOP.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-04-03 19:51:46.000000 portable-python-1.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       99 2024-04-03 19:51:46.000000 portable-python-1.9.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     8583 2024-04-03 19:52:17.250450 portable-python-1.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6912 2024-04-03 19:51:46.000000 portable-python-1.9.1/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      289 2024-04-03 19:51:46.000000 portable-python-1.9.1/SECURITY.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2098 2024-04-03 19:51:46.000000 portable-python-1.9.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-04-03 19:51:46.000000 portable-python-1.9.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-03 19:52:17.250450 portable-python-1.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1654 2024-04-03 19:51:46.000000 portable-python-1.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 19:52:17.242450 portable-python-1.9.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 19:52:17.246450 portable-python-1.9.1/src/portable_python/
+-rw-r--r--   0 runner    (1001) docker     (127)    27235 2024-04-03 19:51:46.000000 portable-python-1.9.1/src/portable_python/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      149 2024-04-03 19:51:46.000000 portable-python-1.9.1/src/portable_python/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7488 2024-04-03 19:51:46.000000 portable-python-1.9.1/src/portable_python/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13714 2024-04-03 19:51:46.000000 portable-python-1.9.1/src/portable_python/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16567 2024-04-03 19:51:46.000000 portable-python-1.9.1/src/portable_python/cpython.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 19:52:17.246450 portable-python-1.9.1/src/portable_python/external/
+-rw-r--r--   0 runner    (1001) docker     (127)      725 2024-04-03 19:51:46.000000 portable-python-1.9.1/src/portable_python/external/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3715 2024-04-03 19:51:46.000000 portable-python-1.9.1/src/portable_python/external/_inspect.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3490 2024-04-03 19:51:46.000000 portable-python-1.9.1/src/portable_python/external/tkinter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10319 2024-04-03 19:51:46.000000 portable-python-1.9.1/src/portable_python/external/xcpython.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21349 2024-04-03 19:51:46.000000 portable-python-1.9.1/src/portable_python/inspector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1978 2024-04-03 19:51:46.000000 portable-python-1.9.1/src/portable_python/tracking.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7085 2024-04-03 19:51:46.000000 portable-python-1.9.1/src/portable_python/versions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 19:52:17.250450 portable-python-1.9.1/src/portable_python.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     8583 2024-04-03 19:52:17.000000 portable-python-1.9.1/src/portable_python.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      981 2024-04-03 19:52:17.000000 portable-python-1.9.1/src/portable_python.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 19:52:17.000000 portable-python-1.9.1/src/portable_python.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-04-03 19:52:17.000000 portable-python-1.9.1/src/portable_python.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-04-03 19:52:17.000000 portable-python-1.9.1/src/portable_python.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-03 19:52:17.000000 portable-python-1.9.1/src/portable_python.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 19:52:17.250450 portable-python-1.9.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     4579 2024-04-03 19:51:46.000000 portable-python-1.9.1/tests/test_build.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3305 2024-04-03 19:51:46.000000 portable-python-1.9.1/tests/test_cleanup.py
+-rw-r--r--   0 runner    (1001) docker     (127)      919 2024-04-03 19:51:46.000000 portable-python-1.9.1/tests/test_failed.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8366 2024-04-03 19:51:46.000000 portable-python-1.9.1/tests/test_inspector.py
+-rw-r--r--   0 runner    (1001) docker     (127)      625 2024-04-03 19:51:46.000000 portable-python-1.9.1/tests/test_invoker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1573 2024-04-03 19:51:46.000000 portable-python-1.9.1/tests/test_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)      711 2024-04-03 19:51:46.000000 portable-python-1.9.1/tests/test_prefix.py
+-rw-r--r--   0 runner    (1001) docker     (127)      763 2024-04-03 19:51:46.000000 portable-python-1.9.1/tests/test_recompress.py
+-rw-r--r--   0 runner    (1001) docker     (127)      408 2024-04-03 19:51:46.000000 portable-python-1.9.1/tests/test_report.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2877 2024-04-03 19:51:46.000000 portable-python-1.9.1/tests/test_setup.py
```

### Comparing `portable-python-1.9.0/DEVELOP.md` & `portable-python-1.9.1/DEVELOP.md`

 * *Files identical despite different names*

### Comparing `portable-python-1.9.0/LICENSE` & `portable-python-1.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `portable-python-1.9.0/PKG-INFO` & `portable-python-1.9.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: portable-python
-Version: 1.9.0
+Version: 1.9.1
 Summary: Portable python binaries
 Home-page: https://github.com/codrsquad/portable-python
 Author: Zoran Simic
 Author-email: zoran@simicweb.com
 License: MIT
 Project-URL: Documentation, https://github.com/codrsquad/portable-python/wiki
 Project-URL: Release notes, https://github.com/codrsquad/portable-python/wiki/Release-notes
```

### Comparing `portable-python-1.9.0/README.rst` & `portable-python-1.9.1/README.rst`

 * *Files identical despite different names*

### Comparing `portable-python-1.9.0/pyproject.toml` & `portable-python-1.9.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `portable-python-1.9.0/setup.py` & `portable-python-1.9.1/setup.py`

 * *Files identical despite different names*

### Comparing `portable-python-1.9.0/src/portable_python/__init__.py` & `portable-python-1.9.1/src/portable_python/__init__.py`

 * *Files identical despite different names*

### Comparing `portable-python-1.9.0/src/portable_python/cli.py` & `portable-python-1.9.1/src/portable_python/cli.py`

 * *Files identical despite different names*

### Comparing `portable-python-1.9.0/src/portable_python/config.py` & `portable-python-1.9.1/src/portable_python/config.py`

 * *Files identical despite different names*

### Comparing `portable-python-1.9.0/src/portable_python/cpython.py` & `portable-python-1.9.1/src/portable_python/cpython.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -207,20 +207,14 @@
 
     def _finalize(self):
         is_shared = self.setup.prefix or self.has_configure_opt("--enable-shared", "yes")
         if is_shared:
             lib_auto_correct = LibAutoCorrect(self.c_configure_prefix, self.install_folder, ppp_marker=self.setup.folders.ppp_marker)
             lib_auto_correct.run()
 
-        runez.abort_if(not runez.DRYRUN and not self.bin_python, f"Can't find bin/python in {self.bin_folder}")
-        PPG.config.ensure_main_file_symlinks(self)
-        if not self.setup.prefix:
-            self._relativize_sysconfig()
-            self._relativize_shebangs()
-
         PPG.config.cleanup_configured_globs("Pass 1", self, "cpython-clean-1st-pass")
         PPG.config.symlink_duplicates(self.install_folder)
         validation_script = PPG.config.resolved_path("cpython-validate-script")
         if validation_script:
             LOG.info("Exercising configured validation script: %s" % runez.short(validation_script))
             self.run_python(validation_script)
 
@@ -232,14 +226,20 @@
                 if "--with-ensurepip=install" not in self.c_configure_args_from_config:
                     cmd.append("--upgrade")
 
                 self.run_python(cmd)
 
             self.run_python("-mpip", "install", *runez.flattened(additional))
 
+        runez.abort_if(not runez.DRYRUN and not self.bin_python, f"Can't find bin/python in {self.bin_folder}")
+        PPG.config.ensure_main_file_symlinks(self)
+        if not self.setup.prefix:
+            self._relativize_sysconfig()
+            self._relativize_shebangs()
+
         self._validate_venv_module()
         if PPG.config.get_value("cpython-compile-all"):
             self.run_python("-mcompileall", "-q", self.install_folder / "lib")
 
         if self.prefix_config_folder:
             # When --enable-shared is specified, cpython build does not produce 'lib/libpython*.a'
             # Add it if build was not configured to clean up 'self.prefix_config_folder'
```

### Comparing `portable-python-1.9.0/src/portable_python/external/__init__.py` & `portable-python-1.9.1/src/portable_python/external/__init__.py`

 * *Files identical despite different names*

### Comparing `portable-python-1.9.0/src/portable_python/external/_inspect.py` & `portable-python-1.9.1/src/portable_python/external/_inspect.py`

 * *Files identical despite different names*

### Comparing `portable-python-1.9.0/src/portable_python/external/tkinter.py` & `portable-python-1.9.1/src/portable_python/external/tkinter.py`

 * *Files identical despite different names*

### Comparing `portable-python-1.9.0/src/portable_python/external/xcpython.py` & `portable-python-1.9.1/src/portable_python/external/xcpython.py`

 * *Files 1% similar despite different names*

```diff
@@ -312,15 +312,15 @@
 
     def auto_select_reason(self):
         if not self.resolved_telltale:
             return "Required when lzma.h is not available"
 
     @property
     def url(self):
-        return f"https://github.com/tukaani-project/xz/releases/download/v{self.version}/xz-{self.version}.tar.gz"
+        return f"https://downloads.sourceforge.net/project/lzmautils/xz-{self.version}.tar.gz"
 
     @property
     def version(self):
         return self.cfg_version("5.4.6")
 
     def _do_linux_compile(self):
         self.run_configure(
```

### Comparing `portable-python-1.9.0/src/portable_python/inspector.py` & `portable-python-1.9.1/src/portable_python/inspector.py`

 * *Files identical despite different names*

### Comparing `portable-python-1.9.0/src/portable_python/tracking.py` & `portable-python-1.9.1/src/portable_python/tracking.py`

 * *Files identical despite different names*

### Comparing `portable-python-1.9.0/src/portable_python/versions.py` & `portable-python-1.9.1/src/portable_python/versions.py`

 * *Files identical despite different names*

### Comparing `portable-python-1.9.0/src/portable_python.egg-info/PKG-INFO` & `portable-python-1.9.1/src/portable_python.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: portable-python
-Version: 1.9.0
+Version: 1.9.1
 Summary: Portable python binaries
 Home-page: https://github.com/codrsquad/portable-python
 Author: Zoran Simic
 Author-email: zoran@simicweb.com
 License: MIT
 Project-URL: Documentation, https://github.com/codrsquad/portable-python/wiki
 Project-URL: Release notes, https://github.com/codrsquad/portable-python/wiki/Release-notes
```

### Comparing `portable-python-1.9.0/src/portable_python.egg-info/SOURCES.txt` & `portable-python-1.9.1/src/portable_python.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `portable-python-1.9.0/tests/test_build.py` & `portable-python-1.9.1/tests/test_build.py`

 * *Files identical despite different names*

### Comparing `portable-python-1.9.0/tests/test_cleanup.py` & `portable-python-1.9.1/tests/test_cleanup.py`

 * *Files identical despite different names*

### Comparing `portable-python-1.9.0/tests/test_failed.py` & `portable-python-1.9.1/tests/test_failed.py`

 * *Files identical despite different names*

### Comparing `portable-python-1.9.0/tests/test_inspector.py` & `portable-python-1.9.1/tests/test_inspector.py`

 * *Files identical despite different names*

### Comparing `portable-python-1.9.0/tests/test_invoker.py` & `portable-python-1.9.1/tests/test_invoker.py`

 * *Files identical despite different names*

### Comparing `portable-python-1.9.0/tests/test_list.py` & `portable-python-1.9.1/tests/test_list.py`

 * *Files identical despite different names*

### Comparing `portable-python-1.9.0/tests/test_prefix.py` & `portable-python-1.9.1/tests/test_prefix.py`

 * *Files identical despite different names*

### Comparing `portable-python-1.9.0/tests/test_recompress.py` & `portable-python-1.9.1/tests/test_recompress.py`

 * *Files identical despite different names*

### Comparing `portable-python-1.9.0/tests/test_setup.py` & `portable-python-1.9.1/tests/test_setup.py`

 * *Files identical despite different names*

