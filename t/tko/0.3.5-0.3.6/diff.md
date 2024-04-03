# Comparing `tmp/tko-0.3.5.tar.gz` & `tmp/tko-0.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tko-0.3.5.tar", last modified: Wed Apr  3 02:00:45 2024, max compression
+gzip compressed data, was "tko-0.3.6.tar", last modified: Wed Apr  3 16:44:33 2024, max compression
```

## Comparing `tko-0.3.5.tar` & `tko-0.3.6.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 lion      (1000) lion      (1000)        0 2024-04-03 02:00:45.566548 tko-0.3.5/
--rw-r--r--   0 lion      (1000) lion      (1000)     1043 2023-08-02 17:52:17.000000 tko-0.3.5/LICENSE
--rw-r--r--   0 lion      (1000) lion      (1000)      191 2023-08-02 17:33:10.000000 tko-0.3.5/MANIFEST.in
--rw-r--r--   0 lion      (1000) lion      (1000)     6765 2024-04-03 02:00:45.566548 tko-0.3.5/PKG-INFO
--rw-r--r--   0 lion      (1000) lion      (1000)     5911 2024-04-02 11:33:20.000000 tko-0.3.5/Readme.md
--rw-r--r--   0 lion      (1000) lion      (1000)     2982 2024-04-03 01:58:38.000000 tko-0.3.5/changelog.md
--rw-r--r--   0 lion      (1000) lion      (1000)      298 2023-08-02 17:36:39.000000 tko-0.3.5/requirements.txt
--rw-r--r--   0 lion      (1000) lion      (1000)       74 2024-04-03 02:00:45.566548 tko-0.3.5/setup.cfg
--rw-r--r--   0 lion      (1000) lion      (1000)     3969 2024-04-02 11:33:20.000000 tko-0.3.5/setup.py
-drwxr-xr-x   0 lion      (1000) lion      (1000)        0 2024-04-03 02:00:45.553215 tko-0.3.5/src/
-drwxr-xr-x   0 lion      (1000) lion      (1000)        0 2024-04-03 02:00:45.559882 tko-0.3.5/src/tko/
--rw-r--r--   0 lion      (1000) lion      (1000)       22 2024-04-03 02:00:39.000000 tko-0.3.5/src/tko/__init__.py
--rw-r--r--   0 lion      (1000) lion      (1000)     9191 2024-03-20 21:10:58.000000 tko-0.3.5/src/tko/__main__.py
--rw-r--r--   0 lion      (1000) lion      (1000)     6633 2024-04-03 01:50:04.000000 tko-0.3.5/src/tko/actions.py
--rw-r--r--   0 lion      (1000) lion      (1000)     4367 2024-03-20 21:10:58.000000 tko-0.3.5/src/tko/basic.py
--rw-r--r--   0 lion      (1000) lion      (1000)    10034 2023-10-19 13:10:37.000000 tko-0.3.5/src/tko/diff.py
--rw-r--r--   0 lion      (1000) lion      (1000)     7521 2024-03-21 14:49:39.000000 tko-0.3.5/src/tko/down.py
--rw-r--r--   0 lion      (1000) lion      (1000)     4997 2024-04-03 01:50:45.000000 tko-0.3.5/src/tko/filter.py
--rw-r--r--   0 lion      (1000) lion      (1000)     5747 2023-10-07 23:37:00.000000 tko-0.3.5/src/tko/format.py
--rw-r--r--   0 lion      (1000) lion      (1000)     2727 2024-03-13 17:39:00.000000 tko-0.3.5/src/tko/guide.py
--rw-r--r--   0 lion      (1000) lion      (1000)     8104 2024-04-02 18:12:46.000000 tko-0.3.5/src/tko/loader.py
--rw-r--r--   0 lion      (1000) lion      (1000)     2567 2023-08-03 03:39:13.000000 tko-0.3.5/src/tko/pattern.py
--rw-r--r--   0 lion      (1000) lion      (1000)     1803 2023-10-19 18:36:35.000000 tko-0.3.5/src/tko/runner.py
--rw-r--r--   0 lion      (1000) lion      (1000)     5609 2024-03-20 21:47:04.000000 tko-0.3.5/src/tko/settings.py
--rw-r--r--   0 lion      (1000) lion      (1000)     4426 2024-03-22 11:32:02.000000 tko-0.3.5/src/tko/solver.py
--rw-r--r--   0 lion      (1000) lion      (1000)     7124 2024-04-02 11:33:20.000000 tko-0.3.5/src/tko/wdir.py
--rw-r--r--   0 lion      (1000) lion      (1000)     3177 2024-04-02 11:33:20.000000 tko-0.3.5/src/tko/writer.py
-drwxr-xr-x   0 lion      (1000) lion      (1000)        0 2024-04-03 02:00:45.563215 tko-0.3.5/src/tko.egg-info/
--rw-r--r--   0 lion      (1000) lion      (1000)     6765 2024-04-03 02:00:45.000000 tko-0.3.5/src/tko.egg-info/PKG-INFO
--rw-r--r--   0 lion      (1000) lion      (1000)      554 2024-04-03 02:00:45.000000 tko-0.3.5/src/tko.egg-info/SOURCES.txt
--rw-r--r--   0 lion      (1000) lion      (1000)        1 2024-04-03 02:00:45.000000 tko-0.3.5/src/tko.egg-info/dependency_links.txt
--rw-r--r--   0 lion      (1000) lion      (1000)       47 2024-04-03 02:00:45.000000 tko-0.3.5/src/tko.egg-info/entry_points.txt
--rw-r--r--   0 lion      (1000) lion      (1000)       59 2024-04-03 02:00:45.000000 tko-0.3.5/src/tko.egg-info/requires.txt
--rw-r--r--   0 lion      (1000) lion      (1000)        4 2024-04-03 02:00:45.000000 tko-0.3.5/src/tko.egg-info/top_level.txt
+drwxr-xr-x   0 lion      (1000) lion      (1000)        0 2024-04-03 16:44:33.336644 tko-0.3.6/
+-rw-r--r--   0 lion      (1000) lion      (1000)     1043 2023-08-02 17:52:17.000000 tko-0.3.6/LICENSE
+-rw-r--r--   0 lion      (1000) lion      (1000)      191 2023-08-02 17:33:10.000000 tko-0.3.6/MANIFEST.in
+-rw-r--r--   0 lion      (1000) lion      (1000)     6765 2024-04-03 16:44:33.336644 tko-0.3.6/PKG-INFO
+-rw-r--r--   0 lion      (1000) lion      (1000)     5911 2024-04-02 11:33:20.000000 tko-0.3.6/Readme.md
+-rw-r--r--   0 lion      (1000) lion      (1000)     2991 2024-04-03 02:01:18.000000 tko-0.3.6/changelog.md
+-rw-r--r--   0 lion      (1000) lion      (1000)      298 2023-08-02 17:36:39.000000 tko-0.3.6/requirements.txt
+-rw-r--r--   0 lion      (1000) lion      (1000)       74 2024-04-03 16:44:33.336644 tko-0.3.6/setup.cfg
+-rw-r--r--   0 lion      (1000) lion      (1000)     3969 2024-04-02 11:33:20.000000 tko-0.3.6/setup.py
+drwxr-xr-x   0 lion      (1000) lion      (1000)        0 2024-04-03 16:44:33.323311 tko-0.3.6/src/
+drwxr-xr-x   0 lion      (1000) lion      (1000)        0 2024-04-03 16:44:33.329978 tko-0.3.6/src/tko/
+-rw-r--r--   0 lion      (1000) lion      (1000)       22 2024-04-03 12:38:49.000000 tko-0.3.6/src/tko/__init__.py
+-rw-r--r--   0 lion      (1000) lion      (1000)     9370 2024-04-03 12:42:46.000000 tko-0.3.6/src/tko/__main__.py
+-rw-r--r--   0 lion      (1000) lion      (1000)     6667 2024-04-03 12:43:36.000000 tko-0.3.6/src/tko/actions.py
+-rw-r--r--   0 lion      (1000) lion      (1000)     4516 2024-04-03 12:42:24.000000 tko-0.3.6/src/tko/basic.py
+-rw-r--r--   0 lion      (1000) lion      (1000)    10034 2023-10-19 13:10:37.000000 tko-0.3.6/src/tko/diff.py
+-rw-r--r--   0 lion      (1000) lion      (1000)     7521 2024-03-21 14:49:39.000000 tko-0.3.6/src/tko/down.py
+-rw-r--r--   0 lion      (1000) lion      (1000)     4997 2024-04-03 01:50:45.000000 tko-0.3.6/src/tko/filter.py
+-rw-r--r--   0 lion      (1000) lion      (1000)     5747 2023-10-07 23:37:00.000000 tko-0.3.6/src/tko/format.py
+-rw-r--r--   0 lion      (1000) lion      (1000)     2727 2024-03-13 17:39:00.000000 tko-0.3.6/src/tko/guide.py
+-rw-r--r--   0 lion      (1000) lion      (1000)     8104 2024-04-02 18:12:46.000000 tko-0.3.6/src/tko/loader.py
+-rw-r--r--   0 lion      (1000) lion      (1000)     2567 2023-08-03 03:39:13.000000 tko-0.3.6/src/tko/pattern.py
+-rw-r--r--   0 lion      (1000) lion      (1000)     1803 2023-10-19 18:36:35.000000 tko-0.3.6/src/tko/runner.py
+-rw-r--r--   0 lion      (1000) lion      (1000)     5609 2024-03-20 21:47:04.000000 tko-0.3.6/src/tko/settings.py
+-rw-r--r--   0 lion      (1000) lion      (1000)     4426 2024-03-22 11:32:02.000000 tko-0.3.6/src/tko/solver.py
+-rw-r--r--   0 lion      (1000) lion      (1000)     7124 2024-04-02 11:33:20.000000 tko-0.3.6/src/tko/wdir.py
+-rw-r--r--   0 lion      (1000) lion      (1000)     3177 2024-04-02 11:33:20.000000 tko-0.3.6/src/tko/writer.py
+drwxr-xr-x   0 lion      (1000) lion      (1000)        0 2024-04-03 16:44:33.333311 tko-0.3.6/src/tko.egg-info/
+-rw-r--r--   0 lion      (1000) lion      (1000)     6765 2024-04-03 16:44:33.000000 tko-0.3.6/src/tko.egg-info/PKG-INFO
+-rw-r--r--   0 lion      (1000) lion      (1000)      554 2024-04-03 16:44:33.000000 tko-0.3.6/src/tko.egg-info/SOURCES.txt
+-rw-r--r--   0 lion      (1000) lion      (1000)        1 2024-04-03 16:44:33.000000 tko-0.3.6/src/tko.egg-info/dependency_links.txt
+-rw-r--r--   0 lion      (1000) lion      (1000)       47 2024-04-03 16:44:33.000000 tko-0.3.6/src/tko.egg-info/entry_points.txt
+-rw-r--r--   0 lion      (1000) lion      (1000)       59 2024-04-03 16:44:33.000000 tko-0.3.6/src/tko.egg-info/requires.txt
+-rw-r--r--   0 lion      (1000) lion      (1000)        4 2024-04-03 16:44:33.000000 tko-0.3.6/src/tko.egg-info/top_level.txt
```

### Comparing `tko-0.3.5/LICENSE` & `tko-0.3.6/LICENSE`

 * *Files identical despite different names*

### Comparing `tko-0.3.5/PKG-INFO` & `tko-0.3.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tko
-Version: 0.3.5
+Version: 0.3.6
 Summary: tko: Test Kit Operations
 Home-page: https://github.com/senapk/tko
 Author: David Sena Oliveira
 Author-email: sena@ufc.br
 Project-URL: Bug Reports, https://github.com/senapk/tko/issues
 Project-URL: Source, https://github.com/senapk/tko/
 Keywords: programming,learning
```

### Comparing `tko-0.3.5/Readme.md` & `tko-0.3.6/Readme.md`

 * *Files identical despite different names*

### Comparing `tko-0.3.5/changelog.md` & `tko-0.3.6/changelog.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 # Changelog
 
+- 0.3.5:
+  - update filter mode
 - 0.3.4:
   - cio mode update parser
-  - update filter mode
 - 0.3.3:
   - improved filter mode for fun
   - fixed bud in grade reduction show for build a .tio file
 - 0.3.2:
   - search for "public static void main" in multi file java solvers
   - search for file without "export" in multi file typescript solvers
 - 0.3.1:
```

### Comparing `tko-0.3.5/setup.py` & `tko-0.3.6/setup.py`

 * *Files identical despite different names*

### Comparing `tko-0.3.5/src/tko/__main__.py` & `tko-0.3.6/src/tko/__main__.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,14 +27,16 @@
         elif args.all:
             param.set_diff_mode(DiffMode.ALL)
         else:
             param.set_diff_mode(DiffMode.FIRST)
 
         if args.filter:
             param.set_filter(True)
+        if args.compact:
+            param.set_compact(True)
 
         # load default diff from settings if not specified
         if not args.sideby and not args.updown:
             updown = not SettingsParser().get_hdiff()
             size_too_short = Report.get_terminal_size() < SettingsParser().get_hdiffmin()
             param.set_up_down(updown or size_too_short)
         elif args.sideby:
@@ -122,14 +124,15 @@
         
         subparsers = parser.add_subparsers(title='subcommands', help='help for subcommand.')
 
         # run
         parser_r = subparsers.add_parser('run', parents=[parent_basic], help='run with test cases.')
         parser_r.add_argument('target_list', metavar='T', type=str, nargs='*', help='solvers, test cases or folders.')
         parser_r.add_argument('--filter', '-f', action='store_true', help='filter solver in temp dir before run')
+        parser_r.add_argument('--compact', '-c', action='store_true', help='Dont show case descriptions in failures')
         parser_r.add_argument("--cmd", type=str, help="bash command to run code")
 
         group_n = parser_r.add_mutually_exclusive_group()
         group_n.add_argument('--quiet', '-q', action='store_true', help='quiet mode, do not show any failure.')
         group_n.add_argument('--all', '-a', action='store_true', help='show all failures.')
 
         # add a exclusive group for diff mode
```

### Comparing `tko-0.3.5/src/tko/actions.py` & `tko-0.3.6/src/tko/actions.py`

 * *Files 1% similar despite different names*

```diff
@@ -150,15 +150,16 @@
         if param.diff_mode == DiffMode.QUIET:
             return
         
         results = [unit.result for unit in wdir.unit_list]
         if not ExecutionResult.EXECUTION_ERROR in results and not ExecutionResult.WRONG_OUTPUT in results:
             return
         
-        print(wdir.unit_list_resume())
+        if not param.compact:
+            print(wdir.unit_list_resume())
         
         if param.diff_mode == DiffMode.FIRST:
         # printing only the first wrong case
             wrong = [unit for unit in wdir.unit_list if unit.result != ExecutionResult.SUCCESS][0]
             if param.is_up_down:
                 print(Diff.mount_up_down_diff(wrong))
             else:
```

### Comparing `tko-0.3.5/src/tko/basic.py` & `tko-0.3.6/src/tko/basic.py`

 * *Files 2% similar despite different names*

```diff
@@ -96,22 +96,27 @@
     class Basic:
         def __init__(self):
             self.index: Optional[int] = None
             self.label_pattern: Optional[str] = None
             self.is_up_down: bool = False
             self.diff_mode = DiffMode.FIRST
             self.filter: bool = False
+            self.compact: bool = False
 
         def set_index(self, value: Optional[int]):
             self.index: Optional[int] = value
             return self
 
         def set_label_pattern(self, label_pattern: Optional[str]):
             self.label_pattern: Optional[str] = label_pattern
             return self
+        
+        def set_compact(self, value: bool):
+            self.compact = value
+            return self
 
         def set_up_down(self, value: bool):
             self.is_up_down = value
             return self
     
         def set_filter(self, value: bool):
             self.filter = value
```

### Comparing `tko-0.3.5/src/tko/diff.py` & `tko-0.3.6/src/tko/diff.py`

 * *Files identical despite different names*

### Comparing `tko-0.3.5/src/tko/down.py` & `tko-0.3.6/src/tko/down.py`

 * *Files identical despite different names*

### Comparing `tko-0.3.5/src/tko/filter.py` & `tko-0.3.6/src/tko/filter.py`

 * *Files identical despite different names*

### Comparing `tko-0.3.5/src/tko/format.py` & `tko-0.3.6/src/tko/format.py`

 * *Files identical despite different names*

### Comparing `tko-0.3.5/src/tko/guide.py` & `tko-0.3.6/src/tko/guide.py`

 * *Files identical despite different names*

### Comparing `tko-0.3.5/src/tko/loader.py` & `tko-0.3.6/src/tko/loader.py`

 * *Files identical despite different names*

### Comparing `tko-0.3.5/src/tko/pattern.py` & `tko-0.3.6/src/tko/pattern.py`

 * *Files identical despite different names*

### Comparing `tko-0.3.5/src/tko/runner.py` & `tko-0.3.6/src/tko/runner.py`

 * *Files identical despite different names*

### Comparing `tko-0.3.5/src/tko/settings.py` & `tko-0.3.6/src/tko/settings.py`

 * *Files identical despite different names*

### Comparing `tko-0.3.5/src/tko/solver.py` & `tko-0.3.6/src/tko/solver.py`

 * *Files identical despite different names*

### Comparing `tko-0.3.5/src/tko/wdir.py` & `tko-0.3.6/src/tko/wdir.py`

 * *Files identical despite different names*

### Comparing `tko-0.3.5/src/tko/writer.py` & `tko-0.3.6/src/tko/writer.py`

 * *Files identical despite different names*

### Comparing `tko-0.3.5/src/tko.egg-info/PKG-INFO` & `tko-0.3.6/src/tko.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tko
-Version: 0.3.5
+Version: 0.3.6
 Summary: tko: Test Kit Operations
 Home-page: https://github.com/senapk/tko
 Author: David Sena Oliveira
 Author-email: sena@ufc.br
 Project-URL: Bug Reports, https://github.com/senapk/tko/issues
 Project-URL: Source, https://github.com/senapk/tko/
 Keywords: programming,learning
```

### Comparing `tko-0.3.5/src/tko.egg-info/SOURCES.txt` & `tko-0.3.6/src/tko.egg-info/SOURCES.txt`

 * *Files identical despite different names*

