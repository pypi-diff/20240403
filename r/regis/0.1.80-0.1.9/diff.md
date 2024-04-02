# Comparing `tmp/regis-0.1.80.tar.gz` & `tmp/regis-0.1.9.tar.gz`

## Comparing `regis-0.1.80.tar` & `regis-0.1.9.tar`

### file list

```diff
@@ -1,31 +1,26 @@
--rwxr-xr-x   0        0        0      185 2020-02-02 00:00:00.000000 regis-0.1.80/create_pip_package_test.bat
--rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 regis-0.1.80/install.py
--rwxr-xr-x   0        0        0      160 2020-02-02 00:00:00.000000 regis-0.1.80/install_local.bat
--rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 regis-0.1.80/.vscode/settings.json
--rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 regis-0.1.80/regis/__init__.py
--rw-r--r--   0        0        0    11361 2020-02-02 00:00:00.000000 regis-0.1.80/regis/build.py
--rw-r--r--   0        0        0    11352 2020-02-02 00:00:00.000000 regis-0.1.80/regis/code_coverage.py
--rw-r--r--   0        0        0      521 2020-02-02 00:00:00.000000 regis-0.1.80/regis/compiler_db.py
--rw-r--r--   0        0        0     2244 2020-02-02 00:00:00.000000 regis-0.1.80/regis/diagnostics.py
--rw-r--r--   0        0        0     3107 2020-02-02 00:00:00.000000 regis-0.1.80/regis/dir_watcher.py
--rw-r--r--   0        0        0     6947 2020-02-02 00:00:00.000000 regis-0.1.80/regis/generation.py
--rw-r--r--   0        0        0     3279 2020-02-02 00:00:00.000000 regis-0.1.80/regis/git.py
--rw-r--r--   0        0        0      630 2020-02-02 00:00:00.000000 regis-0.1.80/regis/git_hooks.py
--rw-r--r--   0        0        0     7577 2020-02-02 00:00:00.000000 regis-0.1.80/regis/required_externals.py
--rw-r--r--   0        0        0     8726 2020-02-02 00:00:00.000000 regis-0.1.80/regis/required_libs.py
--rw-r--r--   0        0        0    10561 2020-02-02 00:00:00.000000 regis-0.1.80/regis/required_tools.py
--rw-r--r--   0        0        0      355 2020-02-02 00:00:00.000000 regis-0.1.80/regis/rex_json.py
--rw-r--r--   0        0        0    12753 2020-02-02 00:00:00.000000 regis-0.1.80/regis/run_clang_format.py
--rw-r--r--   0        0        0    17817 2020-02-02 00:00:00.000000 regis-0.1.80/regis/run_clang_tidy.py
--rw-r--r--   0        0        0     4166 2020-02-02 00:00:00.000000 regis-0.1.80/regis/run_clang_tools.py
--rw-r--r--   0        0        0     1014 2020-02-02 00:00:00.000000 regis-0.1.80/regis/subproc.py
--rw-r--r--   0        0        0      581 2020-02-02 00:00:00.000000 regis-0.1.80/regis/task_raii_printing.py
--rw-r--r--   0        0        0    37964 2020-02-02 00:00:00.000000 regis-0.1.80/regis/test.py
--rw-r--r--   0        0        0     6423 2020-02-02 00:00:00.000000 regis-0.1.80/regis/util.py
--rw-r--r--   0        0        0     3729 2020-02-02 00:00:00.000000 regis-0.1.80/regis/vs.py
--rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 regis-0.1.80/regis/.vscode/settings.json
--rw-r--r--   0        0        0     1962 2020-02-02 00:00:00.000000 regis-0.1.80/.gitignore
--rw-r--r--   0        0        0     1092 2020-02-02 00:00:00.000000 regis-0.1.80/LICENSE
--rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 regis-0.1.80/README.md
--rw-r--r--   0        0        0      701 2020-02-02 00:00:00.000000 regis-0.1.80/pyproject.toml
--rw-r--r--   0        0        0      743 2020-02-02 00:00:00.000000 regis-0.1.80/PKG-INFO
+-rwxr-xr-x   0        0        0      163 2020-02-02 00:00:00.000000 regis-0.1.9/create_pip_package.bat
+-rwxr-xr-x   0        0        0      185 2020-02-02 00:00:00.000000 regis-0.1.9/create_pip_package_test.bat
+-rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 regis-0.1.9/install.py
+-rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 regis-0.1.9/regis/__init__.py
+-rw-r--r--   0        0        0     1838 2020-02-02 00:00:00.000000 regis-0.1.9/regis/build.py
+-rw-r--r--   0        0        0    10382 2020-02-02 00:00:00.000000 regis-0.1.9/regis/code_coverage.py
+-rw-r--r--   0        0        0     2232 2020-02-02 00:00:00.000000 regis-0.1.9/regis/diagnostics.py
+-rw-r--r--   0        0        0     3753 2020-02-02 00:00:00.000000 regis-0.1.9/regis/generation.py
+-rw-r--r--   0        0        0      531 2020-02-02 00:00:00.000000 regis-0.1.9/regis/git_hooks.py
+-rw-r--r--   0        0        0     6421 2020-02-02 00:00:00.000000 regis-0.1.9/regis/install_externals.py
+-rw-r--r--   0        0        0     8204 2020-02-02 00:00:00.000000 regis-0.1.9/regis/required_libs.py
+-rw-r--r--   0        0        0     8317 2020-02-02 00:00:00.000000 regis-0.1.9/regis/required_tools.py
+-rw-r--r--   0        0        0      355 2020-02-02 00:00:00.000000 regis-0.1.9/regis/rex_json.py
+-rw-r--r--   0        0        0    12753 2020-02-02 00:00:00.000000 regis-0.1.9/regis/run_clang_format.py
+-rw-r--r--   0        0        0    15236 2020-02-02 00:00:00.000000 regis-0.1.9/regis/run_clang_tidy.py
+-rw-r--r--   0        0        0     3395 2020-02-02 00:00:00.000000 regis-0.1.9/regis/run_clang_tools.py
+-rw-r--r--   0        0        0      932 2020-02-02 00:00:00.000000 regis-0.1.9/regis/setup.py
+-rw-r--r--   0        0        0     1014 2020-02-02 00:00:00.000000 regis-0.1.9/regis/subproc.py
+-rw-r--r--   0        0        0      493 2020-02-02 00:00:00.000000 regis-0.1.9/regis/task_raii_printing.py
+-rw-r--r--   0        0        0    26553 2020-02-02 00:00:00.000000 regis-0.1.9/regis/test.py
+-rw-r--r--   0        0        0     4879 2020-02-02 00:00:00.000000 regis-0.1.9/regis/util.py
+-rw-r--r--   0        0        0     1938 2020-02-02 00:00:00.000000 regis-0.1.9/.gitignore
+-rw-r--r--   0        0        0     1092 2020-02-02 00:00:00.000000 regis-0.1.9/LICENSE
+-rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 regis-0.1.9/README.md
+-rw-r--r--   0        0        0      681 2020-02-02 00:00:00.000000 regis-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0      711 2020-02-02 00:00:00.000000 regis-0.1.9/PKG-INFO
```

### Comparing `regis-0.1.80/install.py` & `regis-0.1.9/install.py`

 * *Files identical despite different names*

### Comparing `regis-0.1.80/regis/code_coverage.py` & `regis-0.1.9/regis/code_coverage.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,53 +2,36 @@
 from pathlib import Path
 import required_tools
 import util
 import subprocess
 import re
 import diagnostics
 import shutil
-import regis.util
-import regis.rex_json
 
-html_report_folder = "lcov"
-root_path = regis.util.find_root()
-settings = regis.rex_json.load_file(os.path.join(root_path, regis.util.settingsPathFromRoot))
+htlm_report_folder = "lcov"
 
 def create_index_rawdata(rawdataPath):
-  log_folder = os.path.join(root_path, settings["intermediate_folder"], settings["logs_folder"])
-  stem = Path(rawdataPath).stem
-  output_folder = os.path.join(log_folder, stem)
-  if not os.path.isdir(output_folder):
-    os.makedirs(output_folder)
-    
-  output_path = os.path.join(output_folder, f"{Path(rawdataPath).stem}.profdata")
+  folder = Path(rawdataPath).parent
+  output_path = os.path.join(folder, f"{Path(rawdataPath).stem}.profdata")
   llvm_profdata_path = required_tools.tool_paths_dict["llvm_profdata_path"]
   os.system(f"{llvm_profdata_path} merge -sparse {rawdataPath} -o {output_path}")
 
   return output_path
 
 def get_line_oriented_report_filename(profDataPath):
-  log_folder = os.path.join(root_path, settings["intermediate_folder"], settings["logs_folder"])
-  stem = Path(profDataPath).stem
-  return os.path.join(log_folder, stem, f"{Path(profDataPath).stem}_line.html")
+  return os.path.join(Path(profDataPath).parent, f"{Path(profDataPath).stem}_line.html")
 
 def get_file_level_summary_filename(profDataPath):
-  log_folder = os.path.join(root_path, settings["intermediate_folder"], settings["logs_folder"])
-  stem = Path(profDataPath).stem
-  return os.path.join(log_folder, stem, f"{Path(profDataPath).stem}_file.report")
+  return os.path.join(Path(profDataPath).parent, f"{Path(profDataPath).stem}_file.report")
 
 def get_lcov_filename(profDataPath):
-  log_folder = os.path.join(root_path, settings["intermediate_folder"], settings["logs_folder"])
-  stem = Path(profDataPath).stem
-  return os.path.join(log_folder, stem, f"{Path(profDataPath).stem}_lcov.info")
+  return os.path.join(Path(profDataPath).parent, f"{Path(profDataPath).stem}_lcov.info")
 
 def get_lcov_unmangled_filename(profDataPath):
-  log_folder = os.path.join(root_path, settings["intermediate_folder"], settings["logs_folder"])
-  stem = Path(profDataPath).stem
-  return os.path.join(log_folder, stem, f"{Path(profDataPath).stem}_lcov_unmangled.info")
+  return os.path.join(Path(profDataPath).parent, f"{Path(profDataPath).stem}_lcov_unmangled.info")
 
 def create_line_oriented_report(programPath, profDataPath):
   llvm_cov_path = required_tools.tool_paths_dict["llvm_cov_path"]
   log_file_path = get_line_oriented_report_filename(profDataPath)
   if os.path.exists(log_file_path):
     os.remove(log_file_path)
 
@@ -135,21 +118,20 @@
   f.truncate()
   f.close()
 
   return unmangled_log_file_path
 
 def __generate_html_reports(unmangledLogFilePath):
   lcov_path = required_tools.tool_paths_dict["lcov_path"]
-  perl_path = required_tools.tool_paths_dict['perl_path']
-  cmd = f"{perl_path} {lcov_path} {unmangledLogFilePath} -q -o {os.path.join(Path(unmangledLogFilePath).parent, html_report_folder)}"
+  cmd = f"perl {lcov_path} {unmangledLogFilePath} -q -o {os.path.join(Path(unmangledLogFilePath).parent, htlm_report_folder)}"
   os.system(cmd)
 
 def create_lcov_report(programPath, profDataPath):
-  if os.path.exists(html_report_folder):
-    shutil.rmtree(html_report_folder)
+  if os.path.exists(htlm_report_folder):
+    shutil.rmtree(htlm_report_folder)
   
   log_file_path = __create_mangled_lcov_info(programPath, profDataPath)
   unmangled_log_file_path = __unmangle_function_names(log_file_path, profDataPath)
   __generate_html_reports(unmangled_log_file_path)
 
 class CoverageCategory:
   def __init__(self, total, missed, cover):
@@ -269,11 +251,11 @@
     if file_summary.coverage() != 100:
       result = 1
       # diagnostics.log_err(f"File {file_summary.filename()} was not fully covered, please see below for more details")
       # diagnostics.log_err(f"Alternatively, investigate the line coverage report file for this file")    
       # diagnostics.log_err(f"This file is located at {Path(filepath).parent}")    
 
   if result != 0:
-    diagnostics.log_err(f"No full coverage. More info found: {filepath}")
+    diagnostics.log_err(f"Errors reported in file: {filepath}")
     diagnostics.log_err(f"Alternatively, investigate the line coverage file or html report located at {Path(filepath).parent}")    
 
   return result
```

### Comparing `regis-0.1.80/regis/diagnostics.py` & `regis-0.1.9/regis/diagnostics.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,21 +25,21 @@
   def no_color(self, msg):
     print(msg)
 
   def debug(self, msg):
     termcolor.cprint(f"{msg}", "magenta")
 
   def info(self, msg):
-    termcolor.cprint(f"{msg}", "light_green")
+    termcolor.cprint(f"{msg}", "green")
 
   def warning(self, msg):
     termcolor.cprint(f"{msg}", "yellow")
 
   def error(self, msg):
-    termcolor.cprint(f"{msg}", "light_red")
+    termcolor.cprint(f"{msg}", "red")
 
   def critical(self, msg):
     self.logger.error(f"-- Critical Error Occurred --")
     self.logger.error(msg)
     raise Exception(msg)
 
 class StreamLogger(Logger):
```

### Comparing `regis-0.1.80/regis/git_hooks.py` & `regis-0.1.9/regis/git_hooks.py`

 * *Files 13% similar despite different names*

```diff
@@ -5,21 +5,17 @@
 
 def __install(hooksPath):
     root_path = regis.util.find_root()
 
     if not os.path.exists(hooksPath):
         return
     
-    git_path = os.path.join(root_path, ".git")
-    if not os.path.exists(git_path):
-        return
-    
     hooks = os.listdir(hooksPath)
 
     for hook in hooks:
         src = os.path.join(hooksPath, hook)
-        dst = os.path.join(git_path, "hooks", hook)
+        dst = os.path.join(root_path, ".git", "hooks", hook)
         shutil.copy(src, dst)
 
 def run(hooksPath):
     task = regis.task_raii_printing.TaskRaiiPrint("Installing git hooks")
     __install(hooksPath)
```

### Comparing `regis-0.1.80/regis/required_externals.py` & `regis-0.1.9/regis/install_externals.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,27 +1,26 @@
 import os
+import json
 import requests
 import zipfile
 import shutil
 from enum import Enum
 
 import regis.diagnostics
 import regis.util
 import regis.rex_json
-import regis.task_raii_printing
-
-root = regis.util.find_root()
-settings = regis.rex_json.load_file(os.path.join(root, regis.util.settingsPathFromRoot))
-temp_dir = os.path.join(root, settings["intermediate_folder"], 'tmp')
 
 class Host(Enum):
     UNKNOWN = 0
     GITLAB = 1
     GITHUB = 2
 
+def __get_script_path():
+    return os.path.dirname(os.path.realpath(__file__))
+
 def __get_host(path):
     if "gitlab" in path:
         return Host.GITLAB
     elif "github" in path:
         return Host.GITHUB
     
     regis.diagnostics.log_info("Unknown host!")
@@ -48,156 +47,132 @@
     elif host == Host.GITLAB:
         return __build_gitlab_path(baseUrl, name, tag)
     else:
         regis.diagnostics.log_err(f"Unknown url host: {host} in url: {baseUrl}")
         return ""
 
 def __load_externals_required():
-    json_blob = regis.rex_json.load_file(os.path.join(root, "_build", "config", "required_externals.json"))
+    root = regis.util.find_root()
+
+    json_blob = regis.rex_json.load_file(os.path.join(root, "build", "config", "required_externals.json"))
     if json_blob == None:
         regis.diagnostics.log_err("Loaded json blob is None, stopping json parse")
         return []
 
     externals_required = []
     for object in json_blob:
         externals_required.append(json_blob[object])
 
     return externals_required
 
 def __download_external(url):
-    # create temporary directory to store cached files to
-    if not os.path.exists(temp_dir):
-        regis.diagnostics.log_info(f'creating: {temp_dir}')
-        os.mkdir(temp_dir)
-
     # get basename of the URL (a.k.a. the filename + extention we would like to download)
     url_basename = os.path.basename(url)
-    download_filepath = os.path.join(temp_dir, url_basename)
 
     # request a download of the given URL
-    if not os.path.exists(download_filepath):
+    if not os.path.exists(url_basename):
         response = requests.get(url)
         if response.status_code == requests.codes.ok:
             # write the downloaded file to disk
-            open(download_filepath, "wb").write(response.content)
+            open(url_basename, "wb").write(response.content)
         else:
             # bad request was made
             regis.diagnostics.log_err(f"Bad request [{str(response.status_code)}] for given url: {url}")
             return []
         
     # extract the zip file on disk
     # we cache the files within the directory before 
     # and after extraction, this gives us the ability
     # to examine the added files within the directory
     regis.diagnostics.log_info("Extracting: " + url)
     
     # pre list directories
     # cached directories before we downloaded anything
-    pre_list_dir = os.listdir(temp_dir)
-    with zipfile.ZipFile(download_filepath,"r") as zip_ref:
-        zip_ref.extractall(temp_dir)
+    pre_list_dir = os.listdir(__get_script_path())
+    with zipfile.ZipFile(url_basename,"r") as zip_ref:
+        zip_ref.extractall(__get_script_path())
 
     # post list directories
     # directories after we downloaded the repository
-    post_list_dir = os.listdir(temp_dir)
+    post_list_dir = os.listdir(__get_script_path())
 
     regis.diagnostics.log_info("Looking for added extracted directories ...")
     added_directory_names = []
     for post_dir in post_list_dir:
         count = pre_list_dir.count(post_dir)
         if count == 0:
             added_directory_names.append(post_dir)
     regis.diagnostics.log_info(f"Found ({str(len(added_directory_names))}): ".join(added_directory_names))
 
     # remove the created zip file
-    os.remove(download_filepath)
+    os.remove(url_basename)
 
     return added_directory_names
 
 def __verify_external(externalPath, requiredTag):
     external_name = os.path.basename(externalPath)
 
     if os.path.exists(externalPath):
         regis.diagnostics.log_no_color(f"External found: {external_name}")
         regis.diagnostics.log_no_color(f"validating version ...")
         version = regis.util.load_version_file(externalPath)
         if version != requiredTag:
             regis.diagnostics.log_err(f"Invalid version data found, redownloading external: {external_name}")
             return False
-        regis.diagnostics.log_info(f"correct version")
         return True
 
     else:
         return False
 
 def __install_external(external):
-    with regis.task_raii_printing.TaskRaiiPrint("Installing externals.."):
-        external_url = external["url"]
-        external_name = external["name"]
-        external_tag = external["tag"]
-        external_store = external["storage"]
-        external_store = external_store.replace("~", root)
-
-        externals_dir = os.path.join(external_store, external_name)
-
-        # if the external is already present we need to check if we need to redownload anything
-        valid_external = __verify_external(externals_dir, external_tag)
-        if not valid_external:    
-            # any data that was already available will be deleted 
-            # the data will be out of date anyway when a download is triggered
-            if os.path.exists(externals_dir):
-                shutil.rmtree(externals_dir)
-
-            url = __build_host_path(external_url, external_name, external_tag)
-            added_directories = __download_external(url)     
-
-            if len(added_directories) == 1:
-                # move to output directory
-                shutil.move(os.path.join(temp_dir, added_directories[0]), os.path.join(external_store, added_directories[0]))
-                # change directory name
-                cwd = os.getcwd()
-                os.chdir(external_store)
-                os.rename(added_directories[0], external_name)
-                os.chdir(cwd)
-            elif len(added_directories) > 1:
-                # create output directory
-                if not os.path.exists(externals_dir):
-                    os.makedirs(externals_dir)
-                # move to output directory
-                for added_directory in added_directories:
-                    shutil.move(os.path.join(temp_dir, added_directory), externals_dir)
-            else:
-                regis.diagnostics.log_err("No directories where extracted.")
-                return
-
-            regis.util.create_version_file(externals_dir, external_tag)   
-
-def __remove_tmp_dir():
-    if os.path.exists(temp_dir):
-        shutil.rmtree(temp_dir)
-
-def query():
-    externals_required = __load_externals_required()
-    if externals_required == None:
-        regis.diagnostics.log_err("Required externals is None, exiting ...")
-        return
-    
-    for external in externals_required:
+    root = regis.util.find_root()
 
-        external_tag = external["tag"]
-        external_name = external["name"]
-        external_store = external["storage"]
-        external_store = external_store.replace("~", root)
-        externals_dir = os.path.join(external_store, external_name)
+    external_url = external["url"]
+    external_name = external["name"]
+    external_tag = external["tag"]
+    external_store = external["storage"]
+    external_store = external_store.replace("~", root)
+
+    externals_dir = os.path.join(external_store, external_name)
+
+    # if the external is already present we need to check if we need to redownload anything
+    valid_external = __verify_external(externals_dir, external_tag)
+    if not valid_external:    
+        # any data that was already available will be deleted 
+        # the data will be out of date anyway when a download is triggered
+        if os.path.exists(externals_dir):
+            shutil.rmtree(externals_dir)
+
+        url = __build_host_path(external_url, external_name, external_tag)
+        added_directories = __download_external(url)     
+
+        if len(added_directories) == 1:
+            # move to output directory
+            shutil.move(os.path.join(__get_script_path(), added_directories[0]), os.path.join(external_store, added_directories[0]))
+            # change directory name
+            cwd = os.getcwd()
+            os.chdir(external_store)
+            os.rename(added_directories[0], external_name)
+            os.chdir(cwd)
+        elif len(added_directories) > 1:
+            # create output directory
+            if not os.path.exists(externals_dir):
+                os.makedirs(externals_dir)
+            # move to output directory
+            for added_directory in added_directories:
+                shutil.move(os.path.join(__get_script_path(), added_directory), externals_dir)
+        else:
+            regis.diagnostics.log_err("No directories where extracted.")
+            return
 
-        __verify_external(externals_dir, external_tag)
+        regis.util.create_version_file(externals_dir, external_tag)   
 
 def run():
+    regis.diagnostics.log_info("Start installing externals ...")
+
     externals_required = __load_externals_required()
     if externals_required == None:
         regis.diagnostics.log_err("Required externals is None, exiting ...")
         return
 
     for external in externals_required:
         __install_external(external)    
-
-    __remove_tmp_dir()
```

### Comparing `regis-0.1.80/regis/required_libs.py` & `regis-0.1.9/regis/required_libs.py`

 * *Files 4% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 import threading
 import requests
 import zipfile 
 import shutil
 from pathlib import Path
 
 root = regis.util.find_root()
-settings = regis.rex_json.load_file(os.path.join(root, regis.util.settingsPathFromRoot))
+settings = regis.rex_json.load_file(os.path.join(root, "build", "config", "settings.json"))
 build_dir = os.path.join(root, settings["build_folder"])
 temp_dir = os.path.join(root, settings["intermediate_folder"])
 tools_install_dir = os.path.join(temp_dir, settings["tools_folder"])
 libs_install_dir = os.path.join(temp_dir, settings["libs_folder"])
 lib_paths_filepath = os.path.join(libs_install_dir, "lib_paths.json")
 zip_downloads_path = os.path.join(libs_install_dir, "zips")
 
@@ -34,15 +34,15 @@
 if os.path.exists(lib_paths_filepath):
   lib_paths_dict = regis.rex_json.load_file(lib_paths_filepath)
 required_libs = []
 not_found_libs = []
 
 def __load_required_libs_dict():
   libs_required = []
-  json_blob = regis.rex_json.load_file(os.path.join(root, "_build", "config", "required_libs.json"))
+  json_blob = regis.rex_json.load_file(os.path.join(root, "build", "config", "required_libs.json"))
   for object in json_blob:
     libs_required.append(json_blob[object])
 
   return libs_required
 
 def __print_lib_found(lib_path, path : str):
   regis.diagnostics.log_no_color(f"{lib_path} found at {path}")
@@ -103,22 +103,22 @@
 
 def __launch_download_thread(url):
     thread = threading.Thread(target=__download_file, args=(url,))
     thread.start()
     return thread  
 
 def __download_lib(name, version, numZipFiles):
-  with regis.task_raii_printing.TaskRaiiPrint(f"Downloading lib {name} {version}"):
-    with regis.util.LoadingAnimation('Downloading'):
-      threads = []
-      for i in range(numZipFiles):
-        threads.append(__launch_download_thread((f"https://github.com/RisingLiberty/RegisZip/raw/{version}/data/{name}.zip.{(i + 1):03d}")))
+  task_print = regis.task_raii_printing.TaskRaiiPrint(f"Downloading lib {name} {version}")
 
-      for thread in threads:
-        thread.join()
+  threads = []
+  for i in range(numZipFiles):
+    threads.append(__launch_download_thread((f"https://github.com/RisingLiberty/RegisZip/raw/{version}/data/{name}.zip.{(i + 1):03d}")))
+
+  for thread in threads:
+    thread.join()
 
 def __enumerate_libs(zipsFolder):
   zips = os.listdir(zipsFolder)
   libs = []
   for zip in zips:
     stem = Path(zip).stem
     if stem not in libs:
@@ -132,31 +132,29 @@
   for zip in zips:
     if Path(zip).stem == stem:
       lib_zip_files.append(os.path.join(folder, zip))
 
   return lib_zip_files
 
 def __unzip_lib(name):
-  with regis.task_raii_printing.TaskRaiiPrint("Unzipping files"):
-    libs_to_unzip = __enumerate_libs(zip_downloads_path)
+  task_print = regis.task_raii_printing.TaskRaiiPrint("Unzipping files")
+  libs_to_unzip = __enumerate_libs(zip_downloads_path)
 
-    with regis.util.LoadingAnimation('Extracting zips'):
-      for lib in libs_to_unzip:
-        lib_zip_files = __enumerate_zip_files_for_lib(lib, zip_downloads_path)
-        lib_master_zip = os.path.join(zip_downloads_path, f"{lib}")
-        regis.diagnostics.log_info(f'extracting {lib} to {lib_master_zip}')
-        with open(lib_master_zip, "ab") as f:
-          for lib_zip in lib_zip_files:
-            with open(lib_zip, "rb") as z:
-                f.write(z.read())
+  for lib in libs_to_unzip:
+    lib_zip_files = __enumerate_zip_files_for_lib(lib, zip_downloads_path)
+    lib_master_zip = os.path.join(zip_downloads_path, f"{lib}.zip")
+    with open(lib_master_zip, "ab") as f:
+      for lib_zip in lib_zip_files:
+        with open(lib_zip, "rb") as z:
+            f.write(z.read())
 
-        with zipfile.ZipFile(lib_master_zip, "r") as zip_obj:
-            zip_obj.extractall(libs_install_dir)
+    with zipfile.ZipFile(lib_master_zip, "r") as zip_obj:
+        zip_obj.extractall(libs_install_dir)
 
-      regis.diagnostics.log_info(f"libs unzipped to {libs_install_dir}")
+  regis.diagnostics.log_info(f"libs unzipped to {libs_install_dir}")
 
 def __is_up_to_date(installPaths, lib):
   for install_path in installPaths:
     path = os.path.join(install_path, lib["archive_name"])
     version = regis.util.load_version_file(path)
     if version == lib["version"]:
       return True
@@ -186,32 +184,27 @@
       not_found_libs.append(required_lib)
             
   return not_found_libs
 
 # checks all paths of the required libs, making sure all of them are installed
 # if they're not installed, it'll flag a required_lib as not fully installed
 def __are_installed():
-  with regis.task_raii_printing.TaskRaiiPrint("Checking if libs are installed"):
+  task_print = regis.task_raii_printing.TaskRaiiPrint("Checking if libs are installed")
 
-    global required_libs
-    required_libs = __load_required_libs_dict()
-    
-    global lib_paths_dict
-    if lib_paths_dict == None:
-      lib_paths_dict = {}
-      
-    global not_found_libs
-    not_found_libs = __look_for_required_libs(required_libs)
+  global required_libs
+  required_libs = __load_required_libs_dict()
+  
+  global lib_paths_dict
+  if lib_paths_dict == None:
+    lib_paths_dict = {}
     
-    if len(not_found_libs) == 0:
-      regis.diagnostics.log_info(f'All libs found')
-    else:
-      regis.diagnostics.log_warn(f'Libs that weren\'t found or were out of date')
-      for lib in not_found_libs:
-        regis.diagnostics.log_warn(f"\t{lib['config_name']}")
+  global not_found_libs
+  not_found_libs = __look_for_required_libs(required_libs)
+  
+  return len(not_found_libs) == 0
 
 def __download():
   # create the temporary path for zips
   if not os.path.exists(zip_downloads_path):
       os.makedirs(zip_downloads_path)
 
   # filter duplicate tools
@@ -241,17 +234,14 @@
     if config_name in lib_paths_dict:
       lib_paths_dict[config_name].clear()
     paths_not_found = __look_for_paths(lib, lib["paths"], [libs_install_dir])
   
     if len(paths_not_found) > 0:
       regis.diagnostics.log_err(f"failed to install {config_name}")
   
-def query():
-  __are_installed()
-
 def run():
   if not __are_installed():
     __download()
     __install()
 
   regis.rex_json.save_file(lib_paths_filepath, lib_paths_dict)
```

### Comparing `regis-0.1.80/regis/required_tools.py` & `regis-0.1.9/regis/required_tools.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,40 +1,38 @@
 import os
 import copy
 import regis.rex_json
 import regis.util
 import regis.task_raii_printing
 import regis.diagnostics
-import regis.vs
 import requests
 import zipfile 
 import shutil
 import threading
 import argparse
 
 from pathlib import Path
 
 root = regis.util.find_root()
-settings = regis.rex_json.load_file(os.path.join(root, regis.util.settingsPathFromRoot))
+settings = regis.rex_json.load_file(os.path.join(root, "build", "config", "settings.json"))
 build_dir = os.path.join(root, settings["build_folder"])
 temp_dir = os.path.join(root, settings["intermediate_folder"])
 tools_install_dir = os.path.join(temp_dir, settings["tools_folder"])
 tool_paths_filepath = os.path.join(tools_install_dir, "tool_paths.json")
 zip_downloads_path = os.path.join(tools_install_dir, "zips")
 
 tool_paths_dict = {}
 if os.path.exists(tool_paths_filepath):
   tool_paths_dict = regis.rex_json.load_file(tool_paths_filepath)
 required_tools = []
 not_found_tools = []
-found_tools = []
 
 def __load_required_tools_dict():
   tools_required = []
-  json_blob = regis.rex_json.load_file(os.path.join(root, "_build", "config", "required_tools.json"))
+  json_blob = regis.rex_json.load_file(os.path.join(root, "build", "config", "required_tools.json"))
   for object in json_blob:
     tools_required.append(json_blob[object])
 
   return tools_required
 
 def __print_tool_found(tool, path : str):
   regis.diagnostics.log_no_color(f"{tool['config_name']} found at {path}")
@@ -44,71 +42,22 @@
   if "extension" in tool:
     extension = tool["extension"]
   elif regis.util.is_windows():
     extension = ".exe"
 
   return extension
 
-def __get_msvc_paths(msvcRelPath : str):
-  res = []
-
-  installed_vs_versions = regis.vs.installed_versions()
-  tool_path = msvcRelPath
-  for installed_vs in installed_vs_versions:
-    msvc_path = os.path.join(installed_vs.installation_path, 'VC', 'Tools', tool_path)
-    if os.path.exists(msvc_path):
-      res.append(msvc_path)
+def __look_for_tools(required_tools):
+  paths = []
     
-  return res
-
-def __get_possible_tool_install_dirs(requiredTool : dict):
-  res = []
-
-  # we purposely don't look in the PATH env variable
-  # as we cannot confidently check version of tools
-  # found in PATH.
-
-  # some tools have specific locations they can be installed at
-  if requiredTool['archive_name'] == 'MSVC':
-    res.extend(__get_msvc_paths(requiredTool['path']))
-
-  return res
-
-def __look_for_tool_on_system(requiredTool):
-    possible_paths = __get_possible_tool_install_dirs(requiredTool)
-
-    # look for the tool
-    exe_extension = __get_tool_extension(requiredTool)
-    tool_path = regis.util.find_file_in_paths(f"{requiredTool['stem']}{exe_extension}", possible_paths)
-
-    return tool_path
-
-def __look_for_tools(required_tools):   
   for required_tool in required_tools:
     stem = required_tool["stem"]
     path = os.path.join(tools_install_dir, required_tool["archive_name"])
     version = regis.util.load_version_file(path)
 
-    # If the version file is not found
-    # we look for the tool somewhere else on the system
-    if not version:
-      tool_path = __look_for_tool_on_system(required_tool)
-      # if the tool is found, we save this path instead
-      # we don't download the tool from the web
-      if tool_path != '':
-        __print_tool_found(required_tool, tool_path)
-        tool_config_name = required_tool["config_name"]
-        tool_paths_dict[tool_config_name] = tool_path
-        found_tools.append(required_tool)
-        continue
-
-      regis.diagnostics.log_err(f"{stem} not found")
-      not_found_tools.append(required_tool)
-      continue
-
     # check if our version is up to date
     if version != required_tool["version"]:
       regis.diagnostics.log_err(f"{stem} is out of date")
       not_found_tools.append(required_tool)
       continue
 
     config_name = required_tool["config_name"]
@@ -121,54 +70,53 @@
           continue
       else:
         regis.diagnostics.log_err(f"Error: tool path cached, but path doesn't exist: {tool_path}")
         not_found_tools.append(required_tool)
         continue
 
     # if not, add the path of the tool directory where it'd be downloaded to
-    paths_to_use = []
+    paths_to_use = copy.deepcopy(paths)
     paths_to_use.append(os.path.join(tools_install_dir, required_tool["path"]))
 
     # look for the tool
     exe_extension = __get_tool_extension(required_tool)
     tool_path = regis.util.find_file_in_paths(f"{stem}{exe_extension}", paths_to_use)
 
     # tool is found, add it to the cached paths
     if tool_path != '':
       __print_tool_found(required_tool, tool_path)
       tool_config_name = required_tool["config_name"]
       tool_paths_dict[tool_config_name] = tool_path
-      found_tools.append(required_tool)
     # tool is not found, add it to the list to be looked for later
     else:
       not_found_tools.append(required_tool)
 
   return not_found_tools
 
 def are_installed():
-  with regis.task_raii_printing.TaskRaiiPrint("Checking if tools are installed"):
+  task_print = regis.task_raii_printing.TaskRaiiPrint("Checking if tools are installed")
 
-    global required_tools
-    required_tools = __load_required_tools_dict()
+  global required_tools
+  required_tools = __load_required_tools_dict()
+  
+  global tool_paths_dict
+  if tool_paths_dict == None:
+    tool_paths_dict = {}
     
-    global tool_paths_dict
-    if tool_paths_dict == None:
-      tool_paths_dict = {}
-      
-    global not_found_tools
-    not_found_tools = __look_for_tools(required_tools)
-
-    if len(not_found_tools) == 0:
-      regis.diagnostics.log_info("All tools found")
-      regis.rex_json.save_file(tool_paths_filepath, tool_paths_dict)
-      return True
-    else:
-      regis.diagnostics.log_warn(f"Tools that weren't found or were out of date: ")
-      for tool in not_found_tools:
-        regis.diagnostics.log_warn(f"\t-{tool['stem']}")
+  global not_found_tools
+  not_found_tools = __look_for_tools(required_tools)
+
+  if len(not_found_tools) == 0:
+    regis.diagnostics.log_info("All tools found")
+    regis.rex_json.save_file(tool_paths_filepath, tool_paths_dict)
+    return True
+  else:
+    regis.diagnostics.log_warn(f"Tools that weren't found: ")
+    for tool in not_found_tools:
+      regis.diagnostics.log_warn(f"\t-{tool['stem']}")
 
   return False
 
 def __download_file(url):
   filename = os.path.basename(url)
   filePath = os.path.join(zip_downloads_path, filename)
   
@@ -177,48 +125,46 @@
     open(filePath, "wb").write(response.content)
   
 def __make_zip_download_path():
   if not os.path.exists(zip_downloads_path):
     os.makedirs(zip_downloads_path)
 
 def __download_tool(name, version, numZipFiles):
-  with regis.task_raii_printing.TaskRaiiPrint(f"Downloading tool {name} {version}"):
-
-    with regis.util.LoadingAnimation('Downloading'):
+  task_print = regis.task_raii_printing.TaskRaiiPrint(f"Downloading tool {name} {version}")
 
-      threads = []
-      for i in range(numZipFiles):
-        threads.append(__launch_download_thread((f"https://github.com/RisingLiberty/RegisZip/raw/{version}/data/{name}.zip.{(i + 1):03d}")))
+  threads = []
+  for i in range(numZipFiles):
+    threads.append(__launch_download_thread((f"https://github.com/RisingLiberty/RegisZip/raw/{version}/data/{name}.zip.{(i + 1):03d}")))
 
-      for thread in threads:
-        thread.join()
+  for thread in threads:
+    thread.join()
 
 def __download_tools_archive():
-  with regis.task_raii_printing.TaskRaiiPrint("Downloading tools"):
+  task_print = regis.task_raii_printing.TaskRaiiPrint("Downloading tools")
 
-    # filter duplicate tools
-    tools_to_download = []
-    for not_found_tool in not_found_tools:
-      archive_name = not_found_tool["archive_name"]
-      should_add = True
-      for tool_to_download in tools_to_download:
-        if archive_name == tool_to_download["archive_name"]:
-          should_add = False
-          break
-      
-      if should_add:
-        tools_to_download.append(not_found_tool)
-
-    for not_found_tool in tools_to_download:
-      arch_name = not_found_tool["archive_name"]
-      num_zip_files = not_found_tool["num_zip_files"]
-      version = not_found_tool["version"]
-      __download_tool(arch_name, version, num_zip_files)
+  # filter duplicate tools
+  tools_to_download = []
+  for not_found_tool in not_found_tools:
+    archive_name = not_found_tool["archive_name"]
+    should_add = True
+    for tool_to_download in tools_to_download:
+      if archive_name == tool_to_download["archive_name"]:
+        should_add = False
+        break
+    
+    if should_add:
+      tools_to_download.append(not_found_tool)
+
+  for not_found_tool in tools_to_download:
+    arch_name = not_found_tool["archive_name"]
+    num_zip_files = not_found_tool["num_zip_files"]
+    version = not_found_tool["version"]
+    __download_tool(arch_name, version, num_zip_files)
 
-    return tools_to_download
+  return tools_to_download
     
 def __enumerate_tools(zipsFolder):
   zips = os.listdir(zipsFolder)
   tools = []
   for zip in zips:
     stem = Path(zip).stem
     if stem not in tools:
@@ -232,83 +178,74 @@
   for zip in zips:
     if Path(zip).stem == stem:
       tool_zip_files.append(os.path.join(folder, zip))
 
   return tool_zip_files
 
 def __unzip_tools():
-  with regis.task_raii_printing.TaskRaiiPrint("Unzipping files"):
-    tools_to_unzip = __enumerate_tools(zip_downloads_path)
+  task_print = regis.task_raii_printing.TaskRaiiPrint("Unzipping files")
+  tools_to_unzip = __enumerate_tools(zip_downloads_path)
 
-    with regis.util.LoadingAnimation('Extracting zips'):
-      for tool in tools_to_unzip:
-        tool_zip_files = __zip_files_for_tool(tool, zip_downloads_path)
-        tool_master_zip = os.path.join(zip_downloads_path, f"{tool}")
-        regis.diagnostics.log_info(f'extracting {tool} to {tool_master_zip}')
-        with open(tool_master_zip, "ab") as f:
-          for tool_zip in tool_zip_files:
-            with open(tool_zip, "rb") as z:
-                f.write(z.read())
+  for tool in tools_to_unzip:
+    tool_zip_files = __zip_files_for_tool(tool, zip_downloads_path)
+    tool_master_zip = os.path.join(zip_downloads_path, f"{tool}")
+    with open(tool_master_zip, "ab") as f:
+      for tool_zip in tool_zip_files:
+        with open(tool_zip, "rb") as z:
+            f.write(z.read())
 
-        with zipfile.ZipFile(tool_master_zip, "r") as zip_obj:
-            zip_obj.extractall(tools_install_dir)
+    with zipfile.ZipFile(tool_master_zip, "r") as zip_obj:
+        zip_obj.extractall(tools_install_dir)
 
-      regis.diagnostics.log_info(f"tools unzipped to {tools_install_dir}")
+  regis.diagnostics.log_info(f"tools unzipped to {tools_install_dir}")
 
-def __create_version_files(foundTools : []):
-  for tool in foundTools:
+def __create_version_files(toolsToDownload : []):
+  for tool in toolsToDownload:
     path = os.path.join(tools_install_dir, tool["archive_name"])
     regis.util.create_version_file(path, tool["version"])
 
 def __delete_tmp_folders():
   shutil.rmtree(zip_downloads_path)
 
 def __launch_download_thread(url):
     thread = threading.Thread(target=__download_file, args=(url,))
     thread.start()
     return thread  
 
 def download():
-  with regis.task_raii_printing.TaskRaiiPrint("Downloading tools"):
-    __make_zip_download_path()
-    __download_tools_archive()
-    __unzip_tools()
-    __delete_tmp_folders()
+  task_print = regis.task_raii_printing.TaskRaiiPrint("Downloading tools")
+  __make_zip_download_path()
+  tools_to_download = __download_tools_archive()
+  __unzip_tools()
+  __create_version_files(tools_to_download)
+  __delete_tmp_folders()
 
 def install():
-  with regis.task_raii_printing.TaskRaiiPrint("installing tools"):
-
-    global tool_paths_dict
-    global not_found_tools
-    for tool in not_found_tools:
+  task_print = regis.task_raii_printing.TaskRaiiPrint("installing tools")
 
-      # look for tool in the folder where it'd be downloaded to
-      exe_extension = __get_tool_extension(tool)
-      path = regis.util.find_file_in_folder(f"{tool['stem']}{exe_extension}", os.path.join(tools_install_dir, tool["path"]))
-
-      # if not found, something is wrong and we have to investigate manually
-      if path == "":
-        tool_name = tool["stem"]
-        regis.diagnostics.log_err(f"failed to find {tool_name}")
-      else:
-        # if found, add it to the cached paths
-        __print_tool_found(tool, path)
-        tool_config_name = tool["config_name"]
-        tool_paths_dict[tool_config_name] = path
-    
-    found_tools.extend(not_found_tools)
-
-    __create_version_files(found_tools)
-
-    # save cached paths to disk
-    regis.rex_json.save_file(tool_paths_filepath, tool_paths_dict)
-
-def query():
-  """Query which required tools are still missing on the current machine."""
-  are_installed()
+  global tool_paths_dict
+  global not_found_tools
+  for tool in not_found_tools:
+
+    # look for tool in the folder where it'd be downloaded to
+    exe_extension = __get_tool_extension(tool)
+    path = regis.util.find_file_in_folder(f"{tool['stem']}{exe_extension}", os.path.join(tools_install_dir, tool["path"]))
+
+    # if not found, something is wrong and we have to investigate manually
+    if path == "":
+      tool_name = tool["stem"]
+      regis.diagnostics.log_err(f"failed to find {tool_name}")
+    else:
+      # if found, add it to the cached paths
+      __print_tool_found(tool, path)
+      tool_config_name = tool["config_name"]
+      tool_paths_dict[tool_config_name] = path
+  
+  # save cached paths to disk
+  regis.rex_json.save_file(tool_paths_filepath, tool_paths_dict)
 
 def run():
   if not are_installed():
     download()
     install()
 
 if __name__ == "__main__":
```

### Comparing `regis-0.1.80/regis/run_clang_format.py` & `regis-0.1.9/regis/run_clang_format.py`

 * *Files identical despite different names*

### Comparing `regis-0.1.80/regis/run_clang_tidy.py` & `regis-0.1.9/regis/run_clang_tidy.py`

 * *Files 14% similar despite different names*

```diff
@@ -45,27 +45,20 @@
 import re
 import shutil
 import subprocess
 import sys
 import tempfile
 import threading
 import traceback
-import time
-
-import regis.util
-import regis.diagnostics
-import regis.rex_json
 
 try:
   import yaml
 except ImportError:
   yaml = None
 
-processed_files : dict[str, float] = {}
-active_pids = []
 
 def strtobool(val):
   """Convert a string representation of truth to a bool following LLVM's CLI argument parsing."""
 
   val = val.lower()
   if val in ['', 'true', '1']:
     return True
@@ -179,84 +172,55 @@
   if binary:
     return binary
   else:
     raise SystemExit(
       "error: failed to find {} in $PATH or at {}"
       .format(name, built_path))
 
-def processed_filepath(build_path : str):
-  return os.path.join(build_path, 'processed.json')
 
-def should_process_file(file : str, build_path : str, config_path : str):
-  global processed_files
-  invocation_str = invocation_string(build_path, file, config_path)
-  if invocation_str in processed_files:
-    was_successful = processed_files[invocation_str]['successful']
-    file_process_time = float(processed_files[invocation_str]['timestamp'])
-    file_mod_time = os.path.getmtime(file)
-
-    return not was_successful or file_mod_time > file_process_time
-  
-  return True
-  
 def apply_fixes(args, clang_apply_replacements_binary, tmpdir):
   """Calls clang-apply-fixes on a given directory."""
   invocation = [clang_apply_replacements_binary]
-  invocation.append(' -ignore-insert-conflict')
+  invocation.append('-ignore-insert-conflict')
   if args.format:
-    invocation.append(' -format')
+    invocation.append('-format')
   if args.style:
-    invocation.append(' -style=' + args.style)
-  invocation.append(f' {tmpdir}')
-  
-  cmd = ''.join(invocation)
-  proc = regis.util.run_subprocess_from_command(''.join(cmd))
-  regis.util.wait_for_process(proc)
-  
-def invocation_string(build_path : str, file : str, config_path : str):
-  return build_path + ' - ' + config_path + ' - -' + (file)
+    invocation.append('-style=' + args.style)
+  invocation.append(tmpdir)
+  subprocess.call(invocation)
+
 
 def run_tidy(args, clang_tidy_binary, tmpdir, build_path, queue, lock,
              failed_files):
   """Takes filenames out of queue and runs clang-tidy on them."""
   while True:
     name = queue.get()
     invocation = get_tidy_invocation(name, clang_tidy_binary, args.checks,
                                      tmpdir, build_path, args.header_filter,
                                      args.allow_enabling_alpha_checkers,
                                      args.extra_arg, args.extra_arg_before,
                                      args.quiet, args.config_file, args.config,
                                      args.line_filter, args.use_color,
                                      args.plugins)
 
-    try:
-      proc = subprocess.Popen(invocation, stdout=subprocess.PIPE, stderr=subprocess.PIPE)
-      active_pids.append(proc.pid)
-      output, err = proc.communicate()
-      active_pids.remove(proc.pid)
-      if proc.returncode != 0:
-        if proc.returncode < 0:
-          msg = "%s: terminated by signal %d\n" % (name, -proc.returncode)
-          err += msg.encode('utf-8')
-        failed_files.append(name)
-      with lock:
-        sys.stdout.write(' '.join(invocation) + '\n' + output.decode('utf-8'))
-        if len(err) > 0:
-          sys.stdout.flush()
-          sys.stderr.write(err.decode('utf-8'))
-        invocation_str = invocation_string(build_path, name, args.config_file)
-        processed_files[invocation_str] = {}
-        processed_files[invocation_str]['timestamp'] = time.time()
-        processed_files[invocation_str]['successful'] = proc.returncode == 0 # warnings are > 0, errors are < 0
-    except Exception as Ex:
-      regis.diagnostics.log_err(f'exception occurred: {Ex}')
+    proc = subprocess.Popen(invocation, stdout=subprocess.PIPE, stderr=subprocess.PIPE)
+    output, err = proc.communicate()
+    if proc.returncode != 0:
+      if proc.returncode < 0:
+        msg = "%s: terminated by signal %d\n" % (name, -proc.returncode)
+        err += msg.encode('utf-8')
+      failed_files.append(name)
+    with lock:
+      sys.stdout.write(' '.join(invocation) + '\n' + output.decode('utf-8'))
+      if len(err) > 0:
+        sys.stdout.flush()
+        sys.stderr.write(err.decode('utf-8'))
     queue.task_done()
 
 
-
 def run():
   parser = argparse.ArgumentParser(description='Runs clang-tidy over all files '
                                    'in a compilation database. Requires '
                                    'clang-tidy and clang-apply-replacements in '
                                    '$PATH or in your build directory.')
   parser.add_argument('-allow-enabling-alpha-checkers',
                       action='store_true', help='allow alpha checkers from '
@@ -318,35 +282,24 @@
                       help='Additional argument to prepend to the compiler '
                       'command line.')
   parser.add_argument('-quiet', action='store_true',
                       help='Run clang-tidy in quiet mode')
   parser.add_argument('-load', dest='plugins',
                       action='append', default=[],
                       help='Load the specified plugin in clang-tidy.')
-  parser.add_argument('-incremental', action='store_true', default=False, help='run incrementally, skip files already processed run and haven\'t changed since last run')
-
   args = parser.parse_args()
 
   db_path = 'compile_commands.json'
 
   if args.build_path is not None:
     build_path = args.build_path
   else:
     # Find our database
     build_path = find_compilation_database(db_path)
 
-  if args.incremental:
-    regis.diagnostics.log_info(f'Running incremental mode')
-    global processed_files
-    processed_path = processed_filepath(build_path)
-    if os.path.exists(processed_path):
-      processed_files = regis.rex_json.load_file(processed_path)
-    else:
-      processed_files = {}
-
   clang_tidy_binary = find_binary(args.clang_tidy_binary, "clang-tidy",
                                   build_path)
 
   tmpdir = None
   if args.fix or (yaml and args.export_fixes):
     clang_apply_replacements_binary = find_binary(
       args.clang_apply_replacements_binary, "clang-apply-replacements",
@@ -396,46 +349,30 @@
       t = threading.Thread(target=run_tidy,
                            args=(args, clang_tidy_binary, tmpdir, build_path,
                                  task_queue, lock, failed_files))
       t.daemon = True
       t.start()
 
     # Fill the queue with files.
-    num_files_skipped = 0
     for name in files:
       if file_name_re.search(name):
-        if not args.incremental or should_process_file(name, build_path, args.config_file):
-          task_queue.put(name)
-        else:
-          num_files_skipped += 1
+        task_queue.put(name)
 
     # Wait for all threads to be done.
     task_queue.join()
-
-    regis.diagnostics.log_info(f'skipped {num_files_skipped} files')
-
     if len(failed_files):
       return_code = 1
 
   except KeyboardInterrupt:
     # This is a sad hack. Unfortunately subprocess goes
     # bonkers with ctrl-c and we start forking merrily.
     print('\nCtrl-C detected, goodbye.')
     if tmpdir:
       shutil.rmtree(tmpdir)
-
-    for pid in active_pids:
-      try:
-        os.kill(pid, 9)
-      except Exception as ex:
-        # this is a hack on Windows which can sometimes fail to kill a process
-        try:
-          subprocess.check_output("Taskkill /PID %d /F" % pid)
-        except Exception as ex:
-          pass
+    os.kill(0, 9)
 
   if yaml and args.export_fixes:
     print('Writing fixes to ' + args.export_fixes + ' ...')
     try:
       merge_replacement_files(tmpdir, args.export_fixes)
     except:
       print('Error exporting fixes.\n', file=sys.stderr)
@@ -450,14 +387,12 @@
       print('Error applying fixes.\n', file=sys.stderr)
       traceback.print_exc()
       return_code = 1
 
   if tmpdir:
     shutil.rmtree(tmpdir)
     
-  regis.rex_json.save_file(processed_filepath(build_path), processed_files)
-
   sys.exit(return_code)
 
 
 if __name__ == '__main__':
   run()
```

### Comparing `regis-0.1.80/regis/run_clang_tools.py` & `regis-0.1.9/regis/run_clang_tools.py`

 * *Files 16% similar despite different names*

```diff
@@ -17,30 +17,30 @@
 import regis.rex_json
 import shutil
 
 clang_tidy_first_pass_filename = ".clang-tidy_first_pass"
 clang_tidy_second_pass_filename = ".clang-tidy_second_pass"
 clang_tidy_format_filename = ".clang-format"
 root = regis.util.find_root()
-settings = regis.rex_json.load_file(os.path.join(root, regis.util.settingsPathFromRoot))
+settings = regis.rex_json.load_file(os.path.join(root, "build", "config", "settings.json"))
 intermediate_folder = settings["intermediate_folder"]
 build_folder = settings["build_folder"]
 processes_in_flight_filename = os.path.join(root, intermediate_folder, build_folder, "ninja", "post_builds_in_flight.tmp")
 project = ""
 
 def __quoted_path(path):
   quote = "\""
   return f"{quote}{path}{quote}"
 
 def __run_command(command):
   proc = regis.subproc.run(command)
   streamdata = proc.communicate()[0]
   return proc.returncode
 
-def run(projectName : str, compdb : str, srcRoot : str, bRunAllChecks : bool, regex : str, bRebuild : bool = False):
+def run(projectName, compdb, srcRoot):
   script_path = os.path.dirname(__file__)
   global project
   project = projectName
 
   headerFilters = regis.util.retrieve_header_filters(compdb, project)
   headerFiltersRegex = regis.util.create_header_filter_regex(headerFilters)
 
@@ -50,32 +50,18 @@
   clang_config_file = os.path.join(compdb, clang_tidy_first_pass_filename)
 
   compdb_path = os.path.join(compdb, "compile_commands.json")
   if os.path.exists(compdb_path):
     regis.diagnostics.log_info(f"Compiler db found at {compdb_path}")
 
     regis.diagnostics.log_info("Running clang-tidy - auto fixes")
-    cmd = f"py {__quoted_path(script_path)}/run_clang_tidy.py -clang-tidy-binary={__quoted_path(clang_tidy_path)} -clang-apply-replacements-binary={__quoted_path(clang_apply_replacements_path)} -config-file={__quoted_path(clang_config_file)} -p={__quoted_path(compdb)} -header-filter={headerFiltersRegex} -quiet -fix {regex}"
-    
-    if not bRebuild:
-      cmd += ' -incremental'
-    
-    proc = regis.util.run_subprocess_from_command(cmd)
-    rc = regis.util.wait_for_process(proc)
+    rc = __run_command(f"py {__quoted_path(script_path)}/run_clang_tidy.py -clang-tidy-binary={__quoted_path(clang_tidy_path)} -clang-apply-replacements-binary={__quoted_path(clang_apply_replacements_path)} -config-file={__quoted_path(clang_config_file)} -p={__quoted_path(compdb)} -header-filter={headerFiltersRegex} -quiet -fix") # force clang compiler, as clang-tools expect it
 
     if rc != 0:
       raise Exception("clang-tidy auto fixes failed")
-  
-    if bRunAllChecks:
-      clang_config_file = os.path.join(compdb, clang_tidy_second_pass_filename)
-      regis.diagnostics.log_info("Running clang-tidy - all checks")  
-      cmd = f"py {__quoted_path(script_path)}/run_clang_tidy.py -clang-tidy-binary={__quoted_path(clang_tidy_path)} -clang-apply-replacements-binary={__quoted_path(clang_apply_replacements_path)} -config-file={__quoted_path(clang_config_file)} -p={__quoted_path(compdb)} -header-filter={headerFiltersRegex} -quiet {regex}"
-      rc = __run_command(cmd) # force clang compiler, as clang-tools expect it
-
-
   else:
     regis.diagnostics.log_warn(f"No compiler db found at {compdb}")
 
   regis.diagnostics.log_info("Running clang-format")
   rc = __run_command(f"py {__quoted_path(script_path)}/run_clang_format.py --clang-format-executable={__quoted_path(clang_format_path)} -r -i {srcRoot}")
 
   if rc != 0:
```

### Comparing `regis-0.1.80/regis/subproc.py` & `regis-0.1.9/regis/subproc.py`

 * *Files identical despite different names*

### Comparing `regis-0.1.80/regis/util.py` & `regis-0.1.9/regis/util.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,39 +1,29 @@
 import os
 import subprocess
-import shutil
-import sys
-import time
-import itertools
-import threading
 from pathlib import Path
 import regis.diagnostics
 import regis.rex_json
 
-settingsPathFromRoot = os.path.join("_build", "config", "settings.json")
-
 def create_version_file(directory : str, tag : str):
     version = {
         "tag": tag
     }
 
-    if not os.path.exists(directory):
-      os.mkdir(directory)
-      
     path = os.path.join(directory, "version.json")
     regis.rex_json.save_file(path, version)
 
 def load_version_file(directory):
   version_file = os.path.join(directory, "version.json")
   if os.path.exists(version_file):
     version_data = regis.rex_json.load_file(version_file)           
     if version_data != None:
       return version_data["tag"]
 
-  return None
+  return ''
 
 def env_paths():
   envPath = os.environ["PATH"]
   paths = envPath.split(os.pathsep)
   return paths
 
 def retrieve_header_filters(targetDir, projectName):
@@ -108,24 +98,24 @@
       dir_idx -= 1
       path_idx -= 1
 
     if dir_idx == -1:
       if os.path.exists(path):
         return path
       else:
-        regis.diagnostics.log_err(f"matching directory found, but doesn't exist: {path}")
+        diagnostics.log_err(f"matching directory found, but doesn't exist: {path}")
 
   return None
 
 def find_in_parent(path, toFind):
   curr_path = path
 
   while toFind not in os.listdir(curr_path):
     if Path(curr_path).parent == curr_path:
-      regis.diagnostics.log_err(f"{toFind} not found in parents of {path}")
+      diagnostics.log_err(f"{toFind} not found in parents of {path}")
       return ''
 
     curr_path = Path(curr_path).parent
 
   return curr_path
 
 def find_root():
@@ -143,108 +133,51 @@
       files_with_extension.append(file)
 
   return files_with_extension
 
 def is_windows():
   return os.name == 'nt'
 
-def run_subprocess_from_command(command : str):
+def run_subprocess(command):
   proc = subprocess.Popen(command)
+  proc.communicate()
   return proc
 
-def run_subprocess(command : str, args = []):
-  proc = subprocess.Popen(executable=command, args=args)
-  return proc
-
-def run_and_get_output(command):
-  proc = subprocess.Popen(command, stdout=subprocess.PIPE, stderr=subprocess.PIPE)
-  output, errc = proc.communicate()
-
-  return output.decode('utf-8'), proc.returncode
-
 def run_subprocess_with_working_dir(command, workingDir):
   proc = subprocess.Popen(command, cwd=workingDir)
   return proc
 
-def run_subprocess_with_callback(command, callback, filterLines):
+def run_subprocess_with_callback(command, callback):
   proc = subprocess.Popen(command, stdout=subprocess.PIPE, stderr=subprocess.PIPE)
-  callback(proc.pid, proc.stdout, False, filterLines)
-  callback(proc.pid, proc.stderr, True, filterLines)
+  callback(proc.stdout)
+  callback(proc.stderr)
   return proc
 
 def wait_for_process(process):
-  process.wait()
-  return process.returncode
+  streamdata = process.communicate()[0]
+  return process.returncode  
 
 def is_executable(path):
   if is_windows():
     if Path(path).suffix == ".exe":
       return True
   else:
     return os.access(path, os.X_OK)
 
 def find_all_files_in_folder(dir, toFindRegex):
   return list(Path(dir).rglob(toFindRegex))
 
-def remove_folders_recursive(dir : str):
-  if os.path.exists(dir):
-    shutil.rmtree(dir)
-
-def temp_cwd(newdir : str):
-	"""Create a scoped working directory. 
-		
-		Example usage:
-
-		with R.temp_cwd('c:\\p4') as d:
-			# cwd is now set to c:\\p4
-			t = os.path.join('data.txt')
-			with open(t, 'wb') as f:
-				f.write(data)
-			shutil.move(t, somewhere)
-		--> cwd is reset to what it was before it entered scope
-	"""
-	class temp_cwd_(object):
-		def __init__(self, newdir):
-					self.ndir = newdir
-					self.odir = os.getcwd()
-
-		def __enter__(self):
-			os.chdir(self.ndir)
-			return self.ndir
-		
-		def __exit__(self, extype, exvalue, tb):
-			os.chdir(self.odir)
-
-	return temp_cwd_(newdir)
-
-class LoadingAnimation():
-    def __init__(self, msg = 'loading'):
-      self.done = False
-      self.msg = msg
-
-
-    def __enter__(self):
-      self.thread = threading.Thread(target=self.start)
-      self.thread.start()
-      return self
-
-    def __exit__(self, exc_type, exc_value, traceback):
-      self.stop()
-
-    def start(self):
-      for c in itertools.cycle(['|', '/', '-', '\\']):
-        if self.done:
-            break
-        sys.stdout.write(f'\r{self.msg} ' + c)
-        sys.stdout.flush()
-        time.sleep(0.1)
-      num_spaces = len(self.msg)
-      sys.stdout.write('\rDone!'.rjust(num_spaces, ' '))
-      sys.stdout.write('\n')
-      sys.stdout.flush()
-
-    def stop(self):
-       self.done = True
-       self.thread.join()
+def find_ninja_project(project):
+  root = find_root()
+  project_file_name = f"{project}.nproj"
+  settings = regis.rex_json.load_file(os.path.join(root, "build", "config", "settings.json"))
+  intermediate_folder = settings["intermediate_folder"]
+  build_folder = settings["build_folder"]
 
+  directory = os.path.join(root, intermediate_folder, build_folder, "ninja")
+  
+  for root_, dirs, files in os.walk(directory):
+    for file in files:
+      if Path(file).name.lower() == project_file_name.lower():
+        return os.path.join(root_, file)
 
-   
+  return ""
```

### Comparing `regis-0.1.80/.gitignore` & `regis-0.1.9/.gitignore`

 * *Files 3% similar despite different names*

```diff
@@ -124,8 +124,7 @@
 .mypy_cache/
 .dmypy.json
 dmypy.json
 
 # Pyre type checker
 .pyre/
 auth.txt
-create_pip_package.bat
```

### Comparing `regis-0.1.80/LICENSE` & `regis-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `regis-0.1.80/pyproject.toml` & `regis-0.1.9/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "regis"
-version = "0.1.80"
+version = "0.1.9"
 authors = [
   { name="Nick De Breuck", email="nick.debreuck@outlook.com" },
 ]
 description = "python framework used by Rex Engine"
 readme = "README.md"
 requires-python = ">=3.9"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 dependencies = [
-  "requests", "termcolor>=2.2.0", "psutil", "filelock", "gitpython", "watchdog"
+  "requests", "termcolor", "psutil", "filelock", "gitpython"
 ]
 
 [project.urls]
 "Homepage" = "https://github.com/RisingLiberty/RexPy"
 "Bug Tracker" = "https://github.com/RisingLiberty/RexPy/issues"
```

### Comparing `regis-0.1.80/PKG-INFO` & `regis-0.1.9/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,22 +1,21 @@
-Metadata-Version: 2.3
+Metadata-Version: 2.1
 Name: regis
-Version: 0.1.80
+Version: 0.1.9
 Summary: python framework used by Rex Engine
 Project-URL: Homepage, https://github.com/RisingLiberty/RexPy
 Project-URL: Bug Tracker, https://github.com/RisingLiberty/RexPy/issues
 Author-email: Nick De Breuck <nick.debreuck@outlook.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.9
 Requires-Dist: filelock
 Requires-Dist: gitpython
 Requires-Dist: psutil
 Requires-Dist: requests
-Requires-Dist: termcolor>=2.2.0
-Requires-Dist: watchdog
+Requires-Dist: termcolor
 Description-Content-Type: text/markdown
 
 # RexPy
 Python framework used in Rex Game Engine and Rex Standard Library
```

