# Comparing `tmp/openfoodfacts-0.2.0.tar.gz` & `tmp/openfoodfacts-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openfoodfacts-0.2.0.tar", max compression
+gzip compressed data, was "openfoodfacts-0.2.1.tar", max compression
```

## Comparing `openfoodfacts-0.2.0.tar` & `openfoodfacts-0.2.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     1182 2024-03-01 13:44:17.138200 openfoodfacts-0.2.0/LICENSE
--rw-r--r--   0        0        0     4138 2024-03-01 13:44:17.138200 openfoodfacts-0.2.0/README.md
--rw-r--r--   0        0        0      465 2024-03-01 13:44:17.138200 openfoodfacts-0.2.0/openfoodfacts/__init__.py
--rw-r--r--   0        0        0    14488 2024-03-01 13:44:17.138200 openfoodfacts-0.2.0/openfoodfacts/api.py
--rw-r--r--   0        0        0     2891 2024-03-01 13:44:17.138200 openfoodfacts-0.2.0/openfoodfacts/dataset.py
--rw-r--r--   0        0        0     4937 2024-03-01 13:44:17.138200 openfoodfacts-0.2.0/openfoodfacts/images.py
--rw-r--r--   0        0        0     1482 2024-03-01 13:44:17.138200 openfoodfacts-0.2.0/openfoodfacts/ingredients.py
--rw-r--r--   0        0        0    39496 2024-03-01 13:44:17.138200 openfoodfacts-0.2.0/openfoodfacts/ocr.py
--rw-r--r--   0        0        0        0 2024-03-01 13:44:17.138200 openfoodfacts-0.2.0/openfoodfacts/py.typed
--rw-r--r--   0        0        0    14036 2024-03-01 13:44:17.138200 openfoodfacts-0.2.0/openfoodfacts/taxonomy.py
--rw-r--r--   0        0        0    24498 2024-03-01 13:44:17.138200 openfoodfacts-0.2.0/openfoodfacts/types.py
--rw-r--r--   0        0        0     7455 2024-03-01 13:44:17.142200 openfoodfacts-0.2.0/openfoodfacts/utils.py
--rw-r--r--   0        0        0      935 2024-03-01 13:44:17.142200 openfoodfacts-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     4730 1970-01-01 00:00:00.000000 openfoodfacts-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1182 2024-04-03 08:34:20.142831 openfoodfacts-0.2.1/LICENSE
+-rw-r--r--   0        0        0     4138 2024-04-03 08:34:20.142831 openfoodfacts-0.2.1/README.md
+-rw-r--r--   0        0        0      465 2024-04-03 08:34:20.142831 openfoodfacts-0.2.1/openfoodfacts/__init__.py
+-rw-r--r--   0        0        0    14488 2024-04-03 08:34:20.142831 openfoodfacts-0.2.1/openfoodfacts/api.py
+-rw-r--r--   0        0        0     3577 2024-04-03 08:34:20.142831 openfoodfacts-0.2.1/openfoodfacts/dataset.py
+-rw-r--r--   0        0        0     4937 2024-04-03 08:34:20.142831 openfoodfacts-0.2.1/openfoodfacts/images.py
+-rw-r--r--   0        0        0     1482 2024-04-03 08:34:20.142831 openfoodfacts-0.2.1/openfoodfacts/ingredients.py
+-rw-r--r--   0        0        0    39496 2024-04-03 08:34:20.142831 openfoodfacts-0.2.1/openfoodfacts/ocr.py
+-rw-r--r--   0        0        0        0 2024-04-03 08:34:20.142831 openfoodfacts-0.2.1/openfoodfacts/py.typed
+-rw-r--r--   0        0        0    14036 2024-04-03 08:34:20.142831 openfoodfacts-0.2.1/openfoodfacts/taxonomy.py
+-rw-r--r--   0        0        0    24499 2024-04-03 08:34:20.142831 openfoodfacts-0.2.1/openfoodfacts/types.py
+-rw-r--r--   0        0        0     7455 2024-04-03 08:34:20.142831 openfoodfacts-0.2.1/openfoodfacts/utils.py
+-rw-r--r--   0        0        0      935 2024-04-03 08:34:20.142831 openfoodfacts-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0     4730 1970-01-01 00:00:00.000000 openfoodfacts-0.2.1/PKG-INFO
```

### Comparing `openfoodfacts-0.2.0/LICENSE` & `openfoodfacts-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `openfoodfacts-0.2.0/README.md` & `openfoodfacts-0.2.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -106,10 +106,10 @@
 - [Pablo Hinojosa](https://github.com/Pablohn26)
 - [Andrea Stagi](https://github.com/astagi)
 - [Benoît Prieur](https://github.com/benprieur)
 - [Aadarsh A](https://github.com/aadarsh-ram)
 
 ## Copyright and License
 
-    Copyright 2016-2022 Open Food Facts
+    Copyright 2016-2024 Open Food Facts
 
 The Open Food Facts Python SDK is licensed under the [MIT License](https://github.com/openfoodfacts/openfoodfacts-python/blob/develop/LICENSE).
```

### Comparing `openfoodfacts-0.2.0/openfoodfacts/api.py` & `openfoodfacts-0.2.1/openfoodfacts/api.py`

 * *Files identical despite different names*

### Comparing `openfoodfacts-0.2.0/openfoodfacts/dataset.py` & `openfoodfacts-0.2.1/openfoodfacts/dataset.py`

 * *Files 14% similar despite different names*

```diff
@@ -13,64 +13,85 @@
 )
 
 logger = get_logger(__name__)
 
 
 DEFAULT_CACHE_DIR = Path("~/.cache/openfoodfacts/datasets").expanduser()
 DATASET_FILE_NAMES = {
-    DatasetType.jsonl: "openfoodfacts-products.jsonl.gz",
-    DatasetType.csv: "en.openfoodfacts.org.products.csv.gz",
+    Flavor.off: {
+        DatasetType.jsonl: "openfoodfacts-products.jsonl.gz",
+        DatasetType.csv: "en.openfoodfacts.org.products.csv.gz",
+    },
+    Flavor.obf: {
+        DatasetType.jsonl: "openbeautyfacts-products.jsonl.gz",
+        DatasetType.csv: "en.openbeautyfacts.org.products.csv",
+    },
+    Flavor.opff: {
+        DatasetType.jsonl: "openpetfoodfacts-products.jsonl.gz",
+        DatasetType.csv: "en.openpetfoodfacts.org.products.csv",
+    },
+    Flavor.opf: {
+        DatasetType.jsonl: "openproductsfacts-products.jsonl.gz",
+        DatasetType.csv: "en.openproductsfacts.org.products.csv",
+    },
 }
 
 
 def get_dataset(
+    flavor: Flavor = Flavor.off,
     dataset_type: DatasetType = DatasetType.jsonl,
     force_download: bool = False,
     download_newer: bool = False,
     cache_dir: Optional[Path] = None,
 ) -> Path:
     """Download (and cache) Open Food Facts dataset.
 
     The dataset is downloaded the first time and subsequently cached in
     `~/.cache/openfoodfacts/datasets`.
 
-    :param dataset_type: The, defaults to DatasetType.jsonl
+    :param flavor: The data source, defaults to Flavor.off
+    :param dataset_type: The returned format, defaults to DatasetType.jsonl
     :param force_download: if True, (re)download the dataset even if it was
         cached, defaults to False
     :param download_newer: if True, download the dataset if a more recent
         version is available (based on file Etag)
     :param cache_dir: the cache directory to use, defaults to
         ~/.cache/openfoodfacts/taxonomy
     :return: the path of the dataset
     """
     cache_dir = DEFAULT_CACHE_DIR if cache_dir is None else cache_dir
-    file_name = DATASET_FILE_NAMES[dataset_type]
+    file_name = DATASET_FILE_NAMES[flavor][dataset_type]
     dataset_path = cache_dir / file_name
-    url = f"{URLBuilder.static(Flavor.off, Environment.org)}/data/{file_name}"
+    url = f"{URLBuilder.static(flavor, Environment.org)}/data/{file_name}"
     cache_dir.mkdir(parents=True, exist_ok=True)
 
     if not should_download_file(url, dataset_path, force_download, download_newer):
         return dataset_path
 
     logger.info("Downloading dataset, saving it in %s", dataset_path)
     download_file(url, dataset_path)
     return dataset_path
 
 
 class ProductDataset:
-    def __init__(self, dataset_type: DatasetType = DatasetType.jsonl, **kwargs):
+    def __init__(
+        self,
+        flavor: Flavor = Flavor.off,
+        dataset_type: DatasetType = DatasetType.jsonl,
+        **kwargs,
+    ):
         """A product dataset.
 
         This class is used to iterate over the Open Food Facts dataset.
 
         :param dataset_type: the dataset type to use (csv or jsonl), defaults
             to DatasetType.jsonl
         """
         self.dataset_type = dataset_type
-        self.dataset_path = get_dataset(dataset_type, **kwargs)
+        self.dataset_path = get_dataset(flavor, dataset_type, **kwargs)
 
     def __iter__(self):
         if self.dataset_type is DatasetType.jsonl:
             return jsonl_iter(self.dataset_path)
         else:
             return self._csv_iterator()
 
@@ -82,9 +103,8 @@
                 yield dict(row)
 
     def count(self) -> int:
         """Return the number of products in the dataset."""
         count = 0
         for _ in self:
             count += 1
-
         return count
```

### Comparing `openfoodfacts-0.2.0/openfoodfacts/images.py` & `openfoodfacts-0.2.1/openfoodfacts/images.py`

 * *Files identical despite different names*

### Comparing `openfoodfacts-0.2.0/openfoodfacts/ingredients.py` & `openfoodfacts-0.2.1/openfoodfacts/ingredients.py`

 * *Files identical despite different names*

### Comparing `openfoodfacts-0.2.0/openfoodfacts/ocr.py` & `openfoodfacts-0.2.1/openfoodfacts/ocr.py`

 * *Files identical despite different names*

### Comparing `openfoodfacts-0.2.0/openfoodfacts/taxonomy.py` & `openfoodfacts-0.2.1/openfoodfacts/taxonomy.py`

 * *Files identical despite different names*

### Comparing `openfoodfacts-0.2.0/openfoodfacts/types.py` & `openfoodfacts-0.2.1/openfoodfacts/types.py`

 * *Files 0% similar despite different names*

```diff
@@ -36,15 +36,15 @@
         if self == self.off:
             return "openfoodfacts"
         elif self == self.obf:
             return "openbeautyfacts"
         elif self == self.opff:
             return "openpetfoodfacts"
         elif self == self.opf:
-            return "openproductfacts"
+            return "openproductsfacts"
         else:
             # Open Food Facts Pro
             return "pro.openfoodfacts"
 
     @classmethod
     def get_from_server_domain(cls, server_domain: str) -> "Flavor":
         """Get the `Flavor` associated with a `server_domain`."""
```

### Comparing `openfoodfacts-0.2.0/openfoodfacts/utils.py` & `openfoodfacts-0.2.1/openfoodfacts/utils.py`

 * *Files identical despite different names*

### Comparing `openfoodfacts-0.2.0/pyproject.toml` & `openfoodfacts-0.2.1/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "openfoodfacts"
-version = "0.2.0"
+version = "0.2.1"
 description = "Official Python SDK of Open Food Facts"
 authors = ["The Open Food Facts team"]
 license = "Apache 2.0"
 readme = "README.md"
 
 [tool.mypy]
 ignore_missing_imports = true
@@ -22,15 +22,15 @@
 requests = ">=2.20.0"
 pydantic = ">=2.0.0,<3.0.0"
 tqdm = ">=4.0.0,<5.0.0"
 
 [tool.poetry.group.dev.dependencies]
 requests-mock = "1.11.0"
 flake8 = "6.0.0"
-black = "24.1.0"
+black = "24.3.0"
 mypy = "1.3.0"
 isort = "5.12.0"
 coverage = {version = "7.2.7", extras = ["toml"]}
 pytest = "7.4.2"
 types-requests = "2.31.0.2"
 types-tqdm = "4.65.0.1"
```

### Comparing `openfoodfacts-0.2.0/PKG-INFO` & `openfoodfacts-0.2.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openfoodfacts
-Version: 0.2.0
+Version: 0.2.1
 Summary: Official Python SDK of Open Food Facts
 License: Apache 2.0
 Author: The Open Food Facts team
 Requires-Python: >=3.8.1,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
@@ -123,11 +123,11 @@
 - [Pablo Hinojosa](https://github.com/Pablohn26)
 - [Andrea Stagi](https://github.com/astagi)
 - [Benoît Prieur](https://github.com/benprieur)
 - [Aadarsh A](https://github.com/aadarsh-ram)
 
 ## Copyright and License
 
-    Copyright 2016-2022 Open Food Facts
+    Copyright 2016-2024 Open Food Facts
 
 The Open Food Facts Python SDK is licensed under the [MIT License](https://github.com/openfoodfacts/openfoodfacts-python/blob/develop/LICENSE).
```

