# Comparing `tmp/ollama_downloads-0.1.1.tar.gz` & `tmp/ollama_downloads-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ollama_downloads-0.1.1.tar", max compression
+gzip compressed data, was "ollama_downloads-0.1.2.tar", max compression
```

## Comparing `ollama_downloads-0.1.1.tar` & `ollama_downloads-0.1.2.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1069 2024-03-27 21:11:16.291574 ollama_downloads-0.1.1/LICENSE
--rw-r--r--   0        0        0      716 2024-03-30 16:37:59.617465 ollama_downloads-0.1.1/README.md
--rw-r--r--   0        0        0      981 2024-04-01 21:48:44.255748 ollama_downloads-0.1.1/pyproject.toml
--rw-r--r--   0        0        0        0 2024-03-27 19:16:18.538261 ollama_downloads-0.1.1/src/ollama_downloads/__init__.py
--rwxr-xr-x   0        0        0     9763 2024-04-01 21:41:13.183990 ollama_downloads-0.1.1/src/ollama_downloads/ollama_downloads_process.py
--rw-r--r--   0        0        0     1285 1970-01-01 00:00:00.000000 ollama_downloads-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1069 2024-03-27 21:11:16.291574 ollama_downloads-0.1.2/LICENSE
+-rw-r--r--   0        0        0      716 2024-03-30 16:37:59.617465 ollama_downloads-0.1.2/README.md
+-rw-r--r--   0        0        0      981 2024-04-03 01:20:40.178525 ollama_downloads-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-03-27 19:16:18.538261 ollama_downloads-0.1.2/src/ollama_downloads/__init__.py
+-rwxr-xr-x   0        0        0     9660 2024-04-03 02:14:56.786327 ollama_downloads-0.1.2/src/ollama_downloads/ollama_downloads_process.py
+-rw-r--r--   0        0        0     1285 1970-01-01 00:00:00.000000 ollama_downloads-0.1.2/PKG-INFO
```

### Comparing `ollama_downloads-0.1.1/LICENSE` & `ollama_downloads-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ollama_downloads-0.1.1/README.md` & `ollama_downloads-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `ollama_downloads-0.1.1/pyproject.toml` & `ollama_downloads-0.1.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ollama-downloads"
-version = "0.1.1"
+version = "0.1.2"
 description = ""
 authors = ["Kenneth Wong <kennethwork101@gmail.com>"]
 readme = "README.md"
 packages = [{include = "ollama_downloads", from = "src"}]
 
 [tool.poetry.dependencies]
 python = "^3.10"
```

### Comparing `ollama_downloads-0.1.1/src/ollama_downloads/ollama_downloads_process.py` & `ollama_downloads-0.1.2/src/ollama_downloads/ollama_downloads_process.py`

 * *Files 13% similar despite different names*

```diff
@@ -23,27 +23,32 @@
     name_ = f"{inspect.currentframe().f_code.co_name}"
     cmd = "ollama pull"
     command = f"{cmd} {model}"
     print(command)
     result = subprocess.check_output([command], shell=True)
     print(f"{name_} result: {result}")
 
+
 @clock
 class OllamaModels:
     @clock
     def __init__(self, options):
         self.name_ = self.__class__.__name__
         name_ = f"{self.name_}: {inspect.currentframe().f_code.co_name}"
         self.options = options
         self.url = options["url"]
         self.driver = webdriver.Chrome()
         self.driver.get(self.url)
         print(f"{name_} url {self.driver.current_url}")
         print(f"{name_} title {self.driver.title}")
         assert self.driver.title == "library", f"-error: {name_} bad title {self.driver.title}"
+        home_dir = os.path.expanduser("~")
+        self.models_dir = os.path.join(home_dir, options["models_dir"])
+        if not os.path.exists(self.models_dir):
+            os.makedirs(folder_path)
 
     @clock
     def __del__(self):
         name_ = f"{self.name_}: {inspect.currentframe().f_code.co_name}"
         print(f"{name_} exiting")
         self.close_browser()
 
@@ -175,46 +180,40 @@
             self._save_file(fname, data)
         for fname in ["models_all_downloaded.txt", "models_big.txt", "models_all.txt", "models_codes.txt", "models_sql.txt", "models_math.txt",]:
             self._load_file(fname)
 
     @clock
     def _save_file(self, fname, fdata):
         name_ = f"{self.name_}: {inspect.currentframe().f_code.co_name}"
-        dirpath = os.path.dirname(os.path.abspath(__file__))
-        # Package root is located at 2 levels up
-        dirpath = os.path.join(dirpath, "../..")
-        fname = os.path.join(dirpath, self.options["models_dir"], fname)
         print(f"{name_} fname {fname}")
+        print(f"{name_} self.models_dir {self.models_dir}")
+        fname = os.path.join(self.models_dir, fname)
         print(f"{name_} fname {fname}")
         with open(fname, "w") as fp:
             json.dump(fdata, fp, indent=4)
 
     @clock
     def _load_file(self, fname):
         name_ = f"{self.name_}: {inspect.currentframe().f_code.co_name}"
         print(f"{name_} fname {fname}")
-        dirpath = os.path.dirname(os.path.abspath(__file__))
-        # Package root is located at 2 levels up
-        dirpath = os.path.join(dirpath, "../..")
-        print(f"{name_} dirpath {dirpath}")
-        fname = os.path.join(dirpath, self.options["models_dir"], fname)
-        print(f"{name_} fname {fname}")
+        print(f"{name_} self.models_dir {self.models_dir}")
+        fname = os.path.join(self.models_dir, fname)
         print(f"{name_} fname {fname}")
         with open(fname, "r") as fp:
             data = json.load(fp)
             printit(f"{fname} data", data)
             printit(f"{fname} data type", type(data))
 
 
 def Options():
     parser = argparse.ArgumentParser()
     parser.add_argument('--default_concur_req', type=int, help='default_concur_req', default=10)
     parser.add_argument('--max_concur_req', type=int, help='max_concur_req', default=10)
     parser.add_argument('--url', type=str, help='url', default='https://ollama.com/library')
-    parser.add_argument('--models_dir', type=str, help='models_dir', default='models')
+    parser.add_argument('--models_dir', type=str, help='models_dir', default='.ollama_downloads/models')
     parser.add_argument('--models', type=str, help='models: A comma seperated list of models to download')
     args = vars(parser.parse_args())
     return args
 
 
 if __name__ == "__main__":
     options = Options()
```

### Comparing `ollama_downloads-0.1.1/PKG-INFO` & `ollama_downloads-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ollama-downloads
-Version: 0.1.1
+Version: 0.1.2
 Summary: 
 Author: Kenneth Wong
 Author-email: kennethwork101@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

