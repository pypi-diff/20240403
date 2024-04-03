# Comparing `tmp/feno-0.0.6.tar.gz` & `tmp/feno-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "feno-0.0.6.tar", last modified: Tue Apr  2 01:52:54 2024, max compression
+gzip compressed data, was "feno-0.0.7.tar", last modified: Wed Apr  3 01:45:43 2024, max compression
```

## Comparing `feno-0.0.6.tar` & `feno-0.0.7.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 lion      (1000) lion      (1000)        0 2024-04-02 01:52:54.536522 feno-0.0.6/
--rw-r--r--   0 lion      (1000) lion      (1000)     1043 2024-03-26 18:23:42.000000 feno-0.0.6/LICENSE
--rw-r--r--   0 lion      (1000) lion      (1000)      191 2024-03-26 18:23:42.000000 feno-0.0.6/MANIFEST.in
--rw-r--r--   0 lion      (1000) lion      (1000)      918 2024-04-02 01:52:54.536522 feno-0.0.6/PKG-INFO
--rw-r--r--   0 lion      (1000) lion      (1000)       46 2024-03-27 17:52:43.000000 feno-0.0.6/README.md
--rw-r--r--   0 lion      (1000) lion      (1000)      244 2024-03-26 18:23:42.000000 feno-0.0.6/changelog.md
--rw-r--r--   0 lion      (1000) lion      (1000)      310 2024-03-27 17:54:40.000000 feno-0.0.6/requirements.txt
--rw-r--r--   0 lion      (1000) lion      (1000)       74 2024-04-02 01:52:54.539856 feno-0.0.6/setup.cfg
--rw-r--r--   0 lion      (1000) lion      (1000)     3107 2024-04-01 17:24:14.000000 feno-0.0.6/setup.py
-drwxr-xr-x   0 lion      (1000) lion      (1000)        0 2024-04-02 01:52:54.523189 feno-0.0.6/src/
-drwxr-xr-x   0 lion      (1000) lion      (1000)        0 2024-04-02 01:52:54.533189 feno-0.0.6/src/feno/
--rw-r--r--   0 lion      (1000) lion      (1000)       22 2024-04-01 17:41:26.000000 feno-0.0.6/src/feno/__init__.py
--rw-r--r--   0 lion      (1000) lion      (1000)     1851 2024-04-02 01:38:15.000000 feno-0.0.6/src/feno/__main__.py
--rw-r--r--   0 lion      (1000) lion      (1000)     5019 2024-04-02 01:38:03.000000 feno-0.0.6/src/feno/actions.py
--rw-r--r--   0 lion      (1000) lion      (1000)      550 2024-03-26 19:17:45.000000 feno-0.0.6/src/feno/cases.py
--rw-r--r--   0 lion      (1000) lion      (1000)     1699 2024-04-01 17:39:49.000000 feno-0.0.6/src/feno/check.py
--rw-r--r--   0 lion      (1000) lion      (1000)      938 2024-03-26 19:19:40.000000 feno-0.0.6/src/feno/css_style.py
--rw-r--r--   0 lion      (1000) lion      (1000)     3821 2024-03-27 17:09:25.000000 feno-0.0.6/src/feno/filter.py
--rw-r--r--   0 lion      (1000) lion      (1000)     6915 2024-04-02 01:52:43.000000 feno-0.0.6/src/feno/html.py
--rw-r--r--   0 lion      (1000) lion      (1000)     2494 2024-03-27 13:44:12.000000 feno-0.0.6/src/feno/indexer.py
--rw-r--r--   0 lion      (1000) lion      (1000)     3326 2024-03-27 13:09:44.000000 feno-0.0.6/src/feno/jsontools.py
--rw-r--r--   0 lion      (1000) lion      (1000)      393 2024-04-01 23:10:29.000000 feno-0.0.6/src/feno/log.py
--rw-r--r--   0 lion      (1000) lion      (1000)    10327 2024-03-27 17:02:47.000000 feno-0.0.6/src/feno/mdpp.py
--rw-r--r--   0 lion      (1000) lion      (1000)     4989 2024-04-01 23:31:38.000000 feno-0.0.6/src/feno/remote_md.py
--rw-r--r--   0 lion      (1000) lion      (1000)     1559 2024-04-02 00:04:11.000000 feno-0.0.6/src/feno/tree.py
-drwxr-xr-x   0 lion      (1000) lion      (1000)        0 2024-04-02 01:52:54.536522 feno-0.0.6/src/feno.egg-info/
--rw-r--r--   0 lion      (1000) lion      (1000)      918 2024-04-02 01:52:54.000000 feno-0.0.6/src/feno.egg-info/PKG-INFO
--rw-r--r--   0 lion      (1000) lion      (1000)      542 2024-04-02 01:52:54.000000 feno-0.0.6/src/feno.egg-info/SOURCES.txt
--rw-r--r--   0 lion      (1000) lion      (1000)        1 2024-04-02 01:52:54.000000 feno-0.0.6/src/feno.egg-info/dependency_links.txt
--rw-r--r--   0 lion      (1000) lion      (1000)      144 2024-04-02 01:52:54.000000 feno-0.0.6/src/feno.egg-info/entry_points.txt
--rw-r--r--   0 lion      (1000) lion      (1000)       55 2024-04-02 01:52:54.000000 feno-0.0.6/src/feno.egg-info/requires.txt
--rw-r--r--   0 lion      (1000) lion      (1000)        5 2024-04-02 01:52:54.000000 feno-0.0.6/src/feno.egg-info/top_level.txt
+drwxr-xr-x   0 lion      (1000) lion      (1000)        0 2024-04-03 01:45:43.279912 feno-0.0.7/
+-rw-r--r--   0 lion      (1000) lion      (1000)     1043 2024-03-26 18:23:42.000000 feno-0.0.7/LICENSE
+-rw-r--r--   0 lion      (1000) lion      (1000)      191 2024-03-26 18:23:42.000000 feno-0.0.7/MANIFEST.in
+-rw-r--r--   0 lion      (1000) lion      (1000)      918 2024-04-03 01:45:43.279912 feno-0.0.7/PKG-INFO
+-rw-r--r--   0 lion      (1000) lion      (1000)       46 2024-03-27 17:52:43.000000 feno-0.0.7/README.md
+-rw-r--r--   0 lion      (1000) lion      (1000)      319 2024-04-02 11:56:24.000000 feno-0.0.7/changelog.md
+-rw-r--r--   0 lion      (1000) lion      (1000)      310 2024-03-27 17:54:40.000000 feno-0.0.7/requirements.txt
+-rw-r--r--   0 lion      (1000) lion      (1000)       74 2024-04-03 01:45:43.279912 feno-0.0.7/setup.cfg
+-rw-r--r--   0 lion      (1000) lion      (1000)     3107 2024-04-01 17:24:14.000000 feno-0.0.7/setup.py
+drwxr-xr-x   0 lion      (1000) lion      (1000)        0 2024-04-03 01:45:43.266579 feno-0.0.7/src/
+drwxr-xr-x   0 lion      (1000) lion      (1000)        0 2024-04-03 01:45:43.276579 feno-0.0.7/src/feno/
+-rw-r--r--   0 lion      (1000) lion      (1000)       22 2024-04-03 01:45:25.000000 feno-0.0.7/src/feno/__init__.py
+-rw-r--r--   0 lion      (1000) lion      (1000)     1861 2024-04-02 01:57:25.000000 feno-0.0.7/src/feno/__main__.py
+-rw-r--r--   0 lion      (1000) lion      (1000)     5130 2024-04-02 12:05:39.000000 feno-0.0.7/src/feno/actions.py
+-rw-r--r--   0 lion      (1000) lion      (1000)      550 2024-03-26 19:17:45.000000 feno-0.0.7/src/feno/cases.py
+-rw-r--r--   0 lion      (1000) lion      (1000)     1699 2024-04-01 17:39:49.000000 feno-0.0.7/src/feno/check.py
+-rw-r--r--   0 lion      (1000) lion      (1000)      938 2024-03-26 19:19:40.000000 feno-0.0.7/src/feno/css_style.py
+-rw-r--r--   0 lion      (1000) lion      (1000)     4997 2024-04-03 01:36:37.000000 feno-0.0.7/src/feno/filter.py
+-rw-r--r--   0 lion      (1000) lion      (1000)     6915 2024-04-02 01:52:43.000000 feno-0.0.7/src/feno/html.py
+-rw-r--r--   0 lion      (1000) lion      (1000)     2494 2024-03-27 13:44:12.000000 feno-0.0.7/src/feno/indexer.py
+-rw-r--r--   0 lion      (1000) lion      (1000)     3326 2024-03-27 13:09:44.000000 feno-0.0.7/src/feno/jsontools.py
+-rw-r--r--   0 lion      (1000) lion      (1000)      393 2024-04-01 23:10:29.000000 feno-0.0.7/src/feno/log.py
+-rw-r--r--   0 lion      (1000) lion      (1000)    10371 2024-04-02 12:07:04.000000 feno-0.0.7/src/feno/mdpp.py
+-rw-r--r--   0 lion      (1000) lion      (1000)     4989 2024-04-01 23:31:38.000000 feno-0.0.7/src/feno/remote_md.py
+-rw-r--r--   0 lion      (1000) lion      (1000)     1846 2024-04-03 01:37:08.000000 feno-0.0.7/src/feno/tree.py
+drwxr-xr-x   0 lion      (1000) lion      (1000)        0 2024-04-03 01:45:43.279912 feno-0.0.7/src/feno.egg-info/
+-rw-r--r--   0 lion      (1000) lion      (1000)      918 2024-04-03 01:45:43.000000 feno-0.0.7/src/feno.egg-info/PKG-INFO
+-rw-r--r--   0 lion      (1000) lion      (1000)      542 2024-04-03 01:45:43.000000 feno-0.0.7/src/feno.egg-info/SOURCES.txt
+-rw-r--r--   0 lion      (1000) lion      (1000)        1 2024-04-03 01:45:43.000000 feno-0.0.7/src/feno.egg-info/dependency_links.txt
+-rw-r--r--   0 lion      (1000) lion      (1000)      144 2024-04-03 01:45:43.000000 feno-0.0.7/src/feno.egg-info/entry_points.txt
+-rw-r--r--   0 lion      (1000) lion      (1000)       55 2024-04-03 01:45:43.000000 feno-0.0.7/src/feno.egg-info/requires.txt
+-rw-r--r--   0 lion      (1000) lion      (1000)        5 2024-04-03 01:45:43.000000 feno-0.0.7/src/feno.egg-info/top_level.txt
```

### Comparing `feno-0.0.6/LICENSE` & `feno-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `feno-0.0.6/PKG-INFO` & `feno-0.0.7/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: feno
-Version: 0.0.6
+Version: 0.0.7
 Summary: feno: Flexible Exercise Notation Organizer
 Home-page: https://github.com/senapk/feno
 Author: David Sena Oliveira
 Author-email: sena@ufc.br
 Project-URL: Bug Reports, https://github.com/senapk/feno/issues
 Project-URL: Source, https://github.com/senapk/feno/
 Keywords: programming,learning
```

### Comparing `feno-0.0.6/setup.py` & `feno-0.0.7/setup.py`

 * *Files identical despite different names*

### Comparing `feno-0.0.6/src/feno/__main__.py` & `feno-0.0.7/src/feno/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,15 +29,15 @@
         exit(1)
 
     for target in args.targets:
         hook = os.path.basename(os.path.abspath(target))
 
         actions = Actions(target, args.remote)
         Log.resume(hook, end=": [ ")
-        Log.verbose(hook)
+        Log.verbose(hook, end=": ")
 
         if not actions.validate():
             continue
 
         actions.load_title()
         actions.create_cache()
         actions.update_markdown()
```

### Comparing `feno-0.0.6/src/feno/actions.py` & `feno-0.0.7/src/feno/actions.py`

 * *Files 2% similar despite different names*

```diff
@@ -54,17 +54,18 @@
         shutil.rmtree(self.cache)
         os.makedirs(self.cache)
         return self
     
     def need_rebuild(self):
         if Check.need_rebuild(self.source_dir, self.target):
             Log.resume("Changes ", end="")
+            Log.verbose(f"changes in {self.source_dir}")
             return True
             
-        Log.verbose(f"    no changes in {self.source_dir}")
+        Log.verbose("")
         return False
     
     def remote_md(self, disable_preamble=False):
         cfg = RemoteCfg()
         if self.remote_config is not None:
             cfg.read(self.remote_config)
         else:
@@ -127,8 +128,10 @@
             Log.resume("Cleaning ", end="")
             Log.verbose("    Cleaning  : html and cases files")
             os.remove(self.cases)
             os.remove(self.target_html)
 
     # run mdpp script on source readme
     def update_markdown(self):
-        Mdpp.update_file(self.source_readme)
+        if Mdpp.update_file(self.source_readme):
+            Log.resume("Mdpp ", end="")
+            Log.verbose(f"    Mdpp updading")
```

### Comparing `feno-0.0.6/src/feno/cases.py` & `feno-0.0.7/src/feno/cases.py`

 * *Files identical despite different names*

### Comparing `feno-0.0.6/src/feno/check.py` & `feno-0.0.7/src/feno/check.py`

 * *Files identical despite different names*

### Comparing `feno-0.0.6/src/feno/css_style.py` & `feno-0.0.7/src/feno/css_style.py`

 * *Files identical despite different names*

### Comparing `feno-0.0.6/src/feno/html.py` & `feno-0.0.7/src/feno/html.py`

 * *Files identical despite different names*

### Comparing `feno-0.0.6/src/feno/indexer.py` & `feno-0.0.7/src/feno/indexer.py`

 * *Files identical despite different names*

### Comparing `feno-0.0.6/src/feno/jsontools.py` & `feno-0.0.7/src/feno/jsontools.py`

 * *Files identical despite different names*

### Comparing `feno-0.0.6/src/feno/mdpp.py` & `feno-0.0.7/src/feno/mdpp.py`

 * *Files 2% similar despite different names*

```diff
@@ -246,35 +246,37 @@
                 file_content = f.read()
                 return True, file_content
         print("Warning: File", path, "not found")
         return False, "" 
 
 class Mdpp:
     @staticmethod
-    def update_file(target, action: Action = Action.RUN):
+    def update_file(target, action: Action = Action.RUN, quiet: bool = False) -> bool:
         path = Main.fix_path(target)
         target_dir = os.path.dirname(path)
         found, original = Main.open_file(path)
         if not found:
-            return
+            return False
         updated = original
         updated_toc = Toc.execute(updated, action)
         updated_toc = Toch.execute(updated_toc, action)
         if updated != updated_toc:
             updated = updated_toc
         updated = Load.execute(updated, target_dir, action)
         updated = Drafts.execute(target, updated, action)
         Save.execute(updated)
         
         if updated != original:
             with open(path, "w") as f:
                 f.write(updated)
                 hook = os.path.abspath(path).split(os.sep)[-2]
-                print(hook + " : mdpp updading")
-    
+                return True
+
+        return False
+
 def main():
     parser = argparse.ArgumentParser()
     parser.add_argument('targets', metavar='T', type=str, nargs='*', help='Readmes or folders')
     parser.add_argument('--quiet', '-q', action="store_true", help='quiet mode')
     parser.add_argument('--clean', '-c', action="store_true", help='clean mode')
     parser.add_argument('--version', '-v', action="store_true", help='version')
     args = parser.parse_args()
@@ -286,12 +288,12 @@
     if len(args.targets) == 0:
         print("No targets selected")
         exit()
     
     action = Action.RUN if not args.clean else Action.CLEAN
 
     for target in args.targets:
-        Mdpp.update_file(target, action)
+        Mdpp.update_file(target, action, args.quiet)
         
 
 if __name__ == '__main__':
     main()
```

### Comparing `feno-0.0.6/src/feno/remote_md.py` & `feno-0.0.7/src/feno/remote_md.py`

 * *Files identical despite different names*

### Comparing `feno-0.0.6/src/feno/tree.py` & `feno-0.0.7/src/feno/tree.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,23 @@
 import os
 
 from .log import Log
 from .filter import Filter
 
 class Tree:
+
+    @staticmethod
+    def add_file_to_tree(source, dict_tree):
+        pieces = source.split(os.sep)
+        if len(pieces) >= 3:
+            if pieces[-3] == "src":
+                if pieces[-2] not in dict_tree: # new language
+                    dict_tree[pieces[-2]] = []
+                dict_tree[pieces[-2]].append(pieces[-1])
+
     @staticmethod
     def deep_filter_copy(source, destiny, dict_tree, deep: int):
         if deep == 0:
             return
         if os.path.isdir(source):
             chain = source.split(os.sep)
             if len(chain) > 1 and chain[-1].startswith("."):
@@ -15,26 +25,23 @@
             if not os.path.isdir(destiny):
                 os.makedirs(destiny)
             for file in sorted(os.listdir(source)):
                 Tree.deep_filter_copy(os.path.join(source, file), os.path.join(destiny, file), dict_tree, deep - 1)
         else:
             filename = os.path.basename(source)
             text_extensions = [".md", ".c", ".cpp", ".h", ".hpp", ".py", ".java", ".js", ".ts", ".hs", ".txt"]
-            pieces = source.split(os.sep)
-            if len(pieces) >= 3:
-                if pieces[-3] == "src":
-                    if pieces[-2] not in dict_tree:
-                        dict_tree[pieces[-2]] = []
-                    dict_tree[pieces[-2]].append(pieces[-1])
-
             if not any([filename.endswith(ext) for ext in text_extensions]):
                 return
             content = open(source, "r").read()
             processed = Filter(filename).process(content)
-            with open(destiny, "w") as f:
-                if processed != content:
-                    Log.verbose("         draft: ", end="")
-                else:
-                    Log.verbose("         =====: ", end="")
-                f.write(processed)
-                Log.verbose(destiny)
+            if processed == content:
+                Log.verbose("         =====: ", end="")
+                open(destiny, "w").write(processed)
+                Tree.add_file_to_tree(source, dict_tree)
+            elif processed == "" or processed == "\n":
+                Log.verbose("         empty: ", end="")
+            else:
+                Log.verbose("         draft: ", end="")
+                open(destiny, "w").write(processed)
+                Tree.add_file_to_tree(source, dict_tree)
+            Log.verbose(destiny)
```

### Comparing `feno-0.0.6/src/feno.egg-info/PKG-INFO` & `feno-0.0.7/src/feno.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: feno
-Version: 0.0.6
+Version: 0.0.7
 Summary: feno: Flexible Exercise Notation Organizer
 Home-page: https://github.com/senapk/feno
 Author: David Sena Oliveira
 Author-email: sena@ufc.br
 Project-URL: Bug Reports, https://github.com/senapk/feno/issues
 Project-URL: Source, https://github.com/senapk/feno/
 Keywords: programming,learning
```

### Comparing `feno-0.0.6/src/feno.egg-info/SOURCES.txt` & `feno-0.0.7/src/feno.egg-info/SOURCES.txt`

 * *Files identical despite different names*

