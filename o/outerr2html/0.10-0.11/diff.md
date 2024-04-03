# Comparing `tmp/outerr2html-0.10.tar.gz` & `tmp/outerr2html-0.11.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "outerr2html-0.10.tar", last modified: Wed Apr  3 03:12:13 2024, max compression
+gzip compressed data, was "outerr2html-0.11.tar", last modified: Wed Apr  3 03:16:10 2024, max compression
```

## Comparing `outerr2html-0.10.tar` & `outerr2html-0.11.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2024-04-03 03:12:13.616545 outerr2html-0.10/
--rw-rw-rw-   0        0        0     1148 2024-04-03 03:12:05.000000 outerr2html-0.10/LICENSE.rst
--rw-rw-rw-   0        0        0      104 2024-04-03 03:12:04.000000 outerr2html-0.10/MANIFEST.in
--rw-rw-rw-   0        0        0     2630 2024-04-03 03:12:13.615792 outerr2html-0.10/PKG-INFO
--rw-rw-rw-   0        0        0     1881 2024-04-03 03:08:26.000000 outerr2html-0.10/README.md
-drwxrwxrwx   0        0        0        0 2024-04-03 03:12:13.609792 outerr2html-0.10/outerr2html/
--rw-rw-rw-   0        0        0     1881 2024-04-03 03:08:26.000000 outerr2html-0.10/outerr2html/README.MD
--rw-rw-rw-   0        0        0    17355 2024-04-03 02:54:25.000000 outerr2html-0.10/outerr2html/__init__.py
--rw-rw-rw-   0        0        0       27 2024-04-03 03:12:12.000000 outerr2html-0.10/outerr2html/requirements.txt
--rw-rw-rw-   0        0        0    12923 2024-04-03 03:12:12.000000 outerr2html-0.10/outerr2html/thirdparty.json
-drwxrwxrwx   0        0        0        0 2024-04-03 03:12:13.615043 outerr2html-0.10/outerr2html.egg-info/
--rw-rw-rw-   0        0        0     2630 2024-04-03 03:12:13.000000 outerr2html-0.10/outerr2html.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      329 2024-04-03 03:12:13.000000 outerr2html-0.10/outerr2html.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-03 03:12:13.000000 outerr2html-0.10/outerr2html.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       27 2024-04-03 03:12:13.000000 outerr2html-0.10/outerr2html.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2024-04-03 03:12:13.000000 outerr2html-0.10/outerr2html.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       85 2024-04-03 03:12:13.617322 outerr2html-0.10/setup.cfg
--rw-rw-rw-   0        0        0     1321 2024-04-03 03:12:12.000000 outerr2html-0.10/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-03 03:16:10.801173 outerr2html-0.11/
+-rw-rw-rw-   0        0        0     1148 2024-04-03 03:16:02.000000 outerr2html-0.11/LICENSE.rst
+-rw-rw-rw-   0        0        0      104 2024-04-03 03:16:01.000000 outerr2html-0.11/MANIFEST.in
+-rw-rw-rw-   0        0        0     2630 2024-04-03 03:16:10.800426 outerr2html-0.11/PKG-INFO
+-rw-rw-rw-   0        0        0     1881 2024-04-03 03:08:26.000000 outerr2html-0.11/README.md
+drwxrwxrwx   0        0        0        0 2024-04-03 03:16:10.792929 outerr2html-0.11/outerr2html/
+-rw-rw-rw-   0        0        0     1881 2024-04-03 03:08:26.000000 outerr2html-0.11/outerr2html/README.MD
+-rw-rw-rw-   0        0        0    17583 2024-04-03 03:15:47.000000 outerr2html-0.11/outerr2html/__init__.py
+-rw-rw-rw-   0        0        0       27 2024-04-03 03:16:09.000000 outerr2html-0.11/outerr2html/requirements.txt
+-rw-rw-rw-   0        0        0    12923 2024-04-03 03:16:09.000000 outerr2html-0.11/outerr2html/thirdparty.json
+drwxrwxrwx   0        0        0        0 2024-04-03 03:16:10.799672 outerr2html-0.11/outerr2html.egg-info/
+-rw-rw-rw-   0        0        0     2630 2024-04-03 03:16:10.000000 outerr2html-0.11/outerr2html.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      329 2024-04-03 03:16:10.000000 outerr2html-0.11/outerr2html.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-03 03:16:10.000000 outerr2html-0.11/outerr2html.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       27 2024-04-03 03:16:10.000000 outerr2html-0.11/outerr2html.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2024-04-03 03:16:10.000000 outerr2html-0.11/outerr2html.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       85 2024-04-03 03:16:10.801957 outerr2html-0.11/setup.cfg
+-rw-rw-rw-   0        0        0     1321 2024-04-03 03:16:09.000000 outerr2html-0.11/setup.py
```

### Comparing `outerr2html-0.10/LICENSE.rst` & `outerr2html-0.11/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `outerr2html-0.10/PKG-INFO` & `outerr2html-0.11/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: outerr2html
-Version: 0.10
+Version: 0.11
 Summary: Pipe stdout/stderr to TXT/HTML (Windows only)
 Home-page: https://github.com/hansalemaos/outerr2html
 Author: Johannes Fischer
 Author-email: aulasparticularesdealemaosp@gmail.com
 License: MIT
 Keywords: requests,ip,v4
 Classifier: Development Status :: 4 - Beta
```

### Comparing `outerr2html-0.10/README.md` & `outerr2html-0.11/README.md`

 * *Files identical despite different names*

### Comparing `outerr2html-0.10/outerr2html/README.MD` & `outerr2html-0.11/outerr2html/README.MD`

 * *Files identical despite different names*

### Comparing `outerr2html-0.10/outerr2html/__init__.py` & `outerr2html-0.11/outerr2html/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -220,14 +220,15 @@
     if res == 0:
         return False
     elif res != 1:
         ctypes.pythonapi.PyThreadState_SetAsyncExc(tid, 0)
         return False
     return True
 
+
 # C and console output crashes on ipython terminal
 if sys.modules.get("IPython.terminal.prompts", None):
 
     @contextmanager
     def stdout_redirector(
         outfolder,
         print_stdout=True,
@@ -338,14 +339,15 @@
                 tfileerr.close()
             except Exception as e:
                 pass
             thread_being_executed.killthread()
             time.sleep(sleep_at_end)
 
 else:
+
     @contextmanager
     def stdout_redirector(
         outfolder,
         print_stdout=True,
         print_stderr=True,
         line_limit_out=1000,
         line_limit_err=1000,
@@ -411,32 +413,34 @@
                 "so_stoptrigger": stdout_stoptrigger,
                 "se_stoptrigger": stderr_stoptrigger,
                 "so_print": stdout_print,
                 "se_print": stderr_print,
             },
         )
         thread_being_executed()
+
         # based on https://gist.github.com/natedileas/8eb31dc03b76183c0211cdde57791005
         def _redirect_stdout(to_fd):
             """Redirect stdout to the given file descriptor."""
             # Flush the C-level buffer stdout
             sys.stdout.flush()
-            libc.fflush(None) 
+            libc.fflush(None)
             # Flush and close sys.stdout - also closes the file descriptor (fd)
             sys.stdout.close()  # works with python.exe, but crashes ipython
             # Make original_stdout_fd point to the same file as to_fd
             os.dup2(to_fd, original_stdout_fd)
             # Create a new sys.stdout that points to the redirected fd
             sys.stdout = io.TextIOWrapper(
                 os.fdopen(original_stdout_fd, "wb"),
                 encoding=config.enco,
                 errors="backslashreplace",
                 line_buffering=True,
                 write_through=True,
             )
+
         def _redirect_stderr(to_fd):
             """Redirect stdout to the given file descriptor."""
             # Flush the C-level buffer stdout
             sys.stderr.flush()
             libc.fflush(None)  #### CHANGED THIS ARG TO NONE #############
             # Flush and close sys.stdout - also closes the file descriptor (fd)
             sys.stderr.close()
@@ -481,17 +485,22 @@
                     sys.stderr.write(
                         "Ansi2HTML not installed. No HTML conversion done.\n"
                     )
                     sys.stderr.flush()
                 else:
                     for filelists in [stdout_list, stderr_list]:
                         for fi in filelists:
-                            with open(fi, "r", encoding=config.enco) as f:
+                            with open(
+                                fi, "r", encoding=config.enco, errors="backslashreplace"
+                            ) as f:
                                 with open(
-                                    fi[:-4] + ".html", "w", encoding=config.enco
+                                    fi[:-4] + ".html",
+                                    "w",
+                                    encoding=config.enco,
+                                    errors="backslashreplace",
                                 ) as f2:
                                     f2.write(conv.convert(f.read()))
 
                     if delete_txt_files:
                         for filelists in [stdout_list, stderr_list]:
                             for fi in filelists:
                                 try:
```

### Comparing `outerr2html-0.10/outerr2html/thirdparty.json` & `outerr2html-0.11/outerr2html/thirdparty.json`

 * *Files identical despite different names*

### Comparing `outerr2html-0.10/outerr2html.egg-info/PKG-INFO` & `outerr2html-0.11/outerr2html.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: outerr2html
-Version: 0.10
+Version: 0.11
 Summary: Pipe stdout/stderr to TXT/HTML (Windows only)
 Home-page: https://github.com/hansalemaos/outerr2html
 Author: Johannes Fischer
 Author-email: aulasparticularesdealemaosp@gmail.com
 License: MIT
 Keywords: requests,ip,v4
 Classifier: Development Status :: 4 - Beta
```

### Comparing `outerr2html-0.10/setup.py` & `outerr2html-0.11/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 with open(os.path.join(os.path.abspath(os.path.dirname(__file__)),'README.md'), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()\
 
 from pathlib import Path
 this_directory = Path(__file__).parent
 #long_description = (this_directory / "README.md").read_text()
 
-VERSION = '''0.10'''
+VERSION = '''0.11'''
 DESCRIPTION = '''Pipe stdout/stderr to TXT/HTML (Windows only)'''
 
 # Setting up
 setup(
     name="outerr2html",
     version=VERSION,
     license='MIT',
```

