# Comparing `tmp/litdata-0.2.2.tar.gz` & `tmp/litdata-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "litdata-0.2.2.tar", last modified: Fri Mar  8 15:18:25 2024, max compression
+gzip compressed data, was "litdata-0.2.3.tar", last modified: Wed Apr  3 09:19:15 2024, max compression
```

## Comparing `litdata-0.2.2.tar` & `litdata-0.2.3.tar`

### file list

```diff
@@ -1,51 +1,52 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 15:18:25.452941 litdata-0.2.2/
--rw-r--r--   0 runner    (1001) docker     (127)      348 2024-03-08 15:18:16.000000 litdata-0.2.2/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)    11352 2024-03-08 15:18:16.000000 litdata-0.2.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      802 2024-03-08 15:18:16.000000 litdata-0.2.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    20470 2024-03-08 15:18:25.452941 litdata-0.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    18837 2024-03-08 15:18:16.000000 litdata-0.2.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 15:18:25.444941 litdata-0.2.2/litdata/
--rw-r--r--   0 runner    (1001) docker     (127)      294 2024-03-08 15:18:16.000000 litdata-0.2.2/litdata/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)     1328 2024-03-08 15:18:16.000000 litdata-0.2.2/litdata/__about__.py
--rw-r--r--   0 runner    (1001) docker     (127)      604 2024-03-08 15:18:16.000000 litdata-0.2.2/litdata/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2144 2024-03-08 15:18:16.000000 litdata-0.2.2/litdata/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 15:18:25.448941 litdata-0.2.2/litdata/processing/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-08 15:18:16.000000 litdata-0.2.2/litdata/processing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    41437 2024-03-08 15:18:16.000000 litdata-0.2.2/litdata/processing/data_processor.py
--rw-r--r--   0 runner    (1001) docker     (127)    17119 2024-03-08 15:18:16.000000 litdata-0.2.2/litdata/processing/functions.py
--rw-r--r--   0 runner    (1001) docker     (127)     3626 2024-03-08 15:18:16.000000 litdata-0.2.2/litdata/processing/readers.py
--rw-r--r--   0 runner    (1001) docker     (127)     4994 2024-03-08 15:18:16.000000 litdata-0.2.2/litdata/processing/utilities.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 15:18:25.448941 litdata-0.2.2/litdata/streaming/
--rw-r--r--   0 runner    (1001) docker     (127)      988 2024-03-08 15:18:16.000000 litdata-0.2.2/litdata/streaming/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6150 2024-03-08 15:18:16.000000 litdata-0.2.2/litdata/streaming/cache.py
--rw-r--r--   0 runner    (1001) docker     (127)     1920 2024-03-08 15:18:16.000000 litdata-0.2.2/litdata/streaming/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     7028 2024-03-08 15:18:16.000000 litdata-0.2.2/litdata/streaming/combined.py
--rw-r--r--   0 runner    (1001) docker     (127)     2097 2024-03-08 15:18:16.000000 litdata-0.2.2/litdata/streaming/compression.py
--rw-r--r--   0 runner    (1001) docker     (127)     7735 2024-03-08 15:18:16.000000 litdata-0.2.2/litdata/streaming/config.py
--rw-r--r--   0 runner    (1001) docker     (127)    25854 2024-03-08 15:18:16.000000 litdata-0.2.2/litdata/streaming/dataloader.py
--rw-r--r--   0 runner    (1001) docker     (127)    19440 2024-03-08 15:18:16.000000 litdata-0.2.2/litdata/streaming/dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     4514 2024-03-08 15:18:16.000000 litdata-0.2.2/litdata/streaming/downloader.py
--rw-r--r--   0 runner    (1001) docker     (127)     8501 2024-03-08 15:18:16.000000 litdata-0.2.2/litdata/streaming/item_loader.py
--rw-r--r--   0 runner    (1001) docker     (127)    13091 2024-03-08 15:18:16.000000 litdata-0.2.2/litdata/streaming/reader.py
--rw-r--r--   0 runner    (1001) docker     (127)    11808 2024-03-08 15:18:16.000000 litdata-0.2.2/litdata/streaming/resolver.py
--rw-r--r--   0 runner    (1001) docker     (127)     9691 2024-03-08 15:18:16.000000 litdata-0.2.2/litdata/streaming/sampler.py
--rw-r--r--   0 runner    (1001) docker     (127)    14307 2024-03-08 15:18:16.000000 litdata-0.2.2/litdata/streaming/serializers.py
--rw-r--r--   0 runner    (1001) docker     (127)     6028 2024-03-08 15:18:16.000000 litdata-0.2.2/litdata/streaming/shuffle.py
--rw-r--r--   0 runner    (1001) docker     (127)    18061 2024-03-08 15:18:16.000000 litdata-0.2.2/litdata/streaming/writer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 15:18:25.452941 litdata-0.2.2/litdata/utilities/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-08 15:18:16.000000 litdata-0.2.2/litdata/utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5998 2024-03-08 15:18:16.000000 litdata-0.2.2/litdata/utilities/broadcast.py
--rw-r--r--   0 runner    (1001) docker     (127)     6903 2024-03-08 15:18:16.000000 litdata-0.2.2/litdata/utilities/env.py
--rw-r--r--   0 runner    (1001) docker     (127)      993 2024-03-08 15:18:16.000000 litdata-0.2.2/litdata/utilities/format.py
--rw-r--r--   0 runner    (1001) docker     (127)     1030 2024-03-08 15:18:16.000000 litdata-0.2.2/litdata/utilities/packing.py
--rw-r--r--   0 runner    (1001) docker     (127)     2956 2024-03-08 15:18:16.000000 litdata-0.2.2/litdata/utilities/shuffle.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 15:18:25.452941 litdata-0.2.2/litdata.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    20470 2024-03-08 15:18:25.000000 litdata-0.2.2/litdata.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1148 2024-03-08 15:18:25.000000 litdata-0.2.2/litdata.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-08 15:18:25.000000 litdata-0.2.2/litdata.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-08 15:18:25.000000 litdata-0.2.2/litdata.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      150 2024-03-08 15:18:25.000000 litdata-0.2.2/litdata.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-03-08 15:18:25.000000 litdata-0.2.2/litdata.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      187 2024-03-08 15:18:16.000000 litdata-0.2.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-08 15:18:25.452941 litdata-0.2.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     3949 2024-03-08 15:18:16.000000 litdata-0.2.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 09:19:15.409219 litdata-0.2.3/
+-rw-r--r--   0 runner    (1001) docker     (127)      348 2024-04-03 09:19:05.000000 litdata-0.2.3/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)    11352 2024-04-03 09:19:05.000000 litdata-0.2.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      802 2024-04-03 09:19:05.000000 litdata-0.2.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    20638 2024-04-03 09:19:15.409219 litdata-0.2.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    18917 2024-04-03 09:19:05.000000 litdata-0.2.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-03 09:19:05.000000 litdata-0.2.3/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-03 09:19:15.409219 litdata-0.2.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     4083 2024-04-03 09:19:05.000000 litdata-0.2.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 09:19:15.401219 litdata-0.2.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 09:19:15.401219 litdata-0.2.3/src/litdata/
+-rw-r--r--   0 runner    (1001) docker     (127)     1328 2024-04-03 09:19:05.000000 litdata-0.2.3/src/litdata/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1166 2024-04-03 09:19:05.000000 litdata-0.2.3/src/litdata/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2123 2024-04-03 09:19:05.000000 litdata-0.2.3/src/litdata/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3774 2024-04-03 09:19:05.000000 litdata-0.2.3/src/litdata/imports.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 09:19:15.405219 litdata-0.2.3/src/litdata/processing/
+-rw-r--r--   0 runner    (1001) docker     (127)      579 2024-04-03 09:19:05.000000 litdata-0.2.3/src/litdata/processing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    42556 2024-04-03 09:19:05.000000 litdata-0.2.3/src/litdata/processing/data_processor.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17136 2024-04-03 09:19:05.000000 litdata-0.2.3/src/litdata/processing/functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4343 2024-04-03 09:19:05.000000 litdata-0.2.3/src/litdata/processing/readers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6040 2024-04-03 09:19:05.000000 litdata-0.2.3/src/litdata/processing/utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 09:19:15.405219 litdata-0.2.3/src/litdata/streaming/
+-rw-r--r--   0 runner    (1001) docker     (127)      988 2024-04-03 09:19:05.000000 litdata-0.2.3/src/litdata/streaming/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5870 2024-04-03 09:19:05.000000 litdata-0.2.3/src/litdata/streaming/cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2500 2024-04-03 09:19:05.000000 litdata-0.2.3/src/litdata/streaming/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7028 2024-04-03 09:19:05.000000 litdata-0.2.3/src/litdata/streaming/combined.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2092 2024-04-03 09:19:05.000000 litdata-0.2.3/src/litdata/streaming/compression.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7735 2024-04-03 09:19:05.000000 litdata-0.2.3/src/litdata/streaming/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25854 2024-04-03 09:19:05.000000 litdata-0.2.3/src/litdata/streaming/dataloader.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19431 2024-04-03 09:19:05.000000 litdata-0.2.3/src/litdata/streaming/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4515 2024-04-03 09:19:05.000000 litdata-0.2.3/src/litdata/streaming/downloader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8501 2024-04-03 09:19:05.000000 litdata-0.2.3/src/litdata/streaming/item_loader.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13127 2024-04-03 09:19:05.000000 litdata-0.2.3/src/litdata/streaming/reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12365 2024-04-03 09:19:05.000000 litdata-0.2.3/src/litdata/streaming/resolver.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9749 2024-04-03 09:19:05.000000 litdata-0.2.3/src/litdata/streaming/sampler.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14520 2024-04-03 09:19:05.000000 litdata-0.2.3/src/litdata/streaming/serializers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6028 2024-04-03 09:19:05.000000 litdata-0.2.3/src/litdata/streaming/shuffle.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18051 2024-04-03 09:19:05.000000 litdata-0.2.3/src/litdata/streaming/writer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 09:19:15.409219 litdata-0.2.3/src/litdata/utilities/
+-rw-r--r--   0 runner    (1001) docker     (127)      579 2024-04-03 09:19:05.000000 litdata-0.2.3/src/litdata/utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6386 2024-04-03 09:19:05.000000 litdata-0.2.3/src/litdata/utilities/broadcast.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7483 2024-04-03 09:19:05.000000 litdata-0.2.3/src/litdata/utilities/env.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1573 2024-04-03 09:19:05.000000 litdata-0.2.3/src/litdata/utilities/format.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1610 2024-04-03 09:19:05.000000 litdata-0.2.3/src/litdata/utilities/packing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3536 2024-04-03 09:19:05.000000 litdata-0.2.3/src/litdata/utilities/shuffle.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 09:19:15.409219 litdata-0.2.3/src/litdata.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    20638 2024-04-03 09:19:15.000000 litdata-0.2.3/src/litdata.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1294 2024-04-03 09:19:15.000000 litdata-0.2.3/src/litdata.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 09:19:15.000000 litdata-0.2.3/src/litdata.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 09:19:15.000000 litdata-0.2.3/src/litdata.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      124 2024-04-03 09:19:15.000000 litdata-0.2.3/src/litdata.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-03 09:19:15.000000 litdata-0.2.3/src/litdata.egg-info/top_level.txt
```

### Comparing `litdata-0.2.2/LICENSE` & `litdata-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `litdata-0.2.2/MANIFEST.in` & `litdata-0.2.3/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `litdata-0.2.2/PKG-INFO` & `litdata-0.2.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: litdata
-Version: 0.2.2
+Version: 0.2.3
 Summary: The Deep Learning framework to train, deploy, and ship AI products Lightning fast.
 Home-page: https://github.com/Lightning-AI/lit-data
 Download-URL: https://github.com/Lightning-AI/litdata
 Author: Lightning AI et al.
 Author-email: pytorch@lightning.ai
 License: Apache-2.0
 Project-URL: Bug Tracker, https://github.com/Lightning-AI/litdata/issues
@@ -22,26 +22,26 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: lightning-cloud==0.5.64
-Requires-Dist: lightning-utilities<0.11.0,>=0.8.0
 Requires-Dist: torch>=2.1.0
 Requires-Dist: filelock
-Requires-Dist: tqdm
 Requires-Dist: numpy
-Requires-Dist: torchvision
-Requires-Dist: pillow
-Requires-Dist: viztracer
-Requires-Dist: pyarrow
 Requires-Dist: boto3[crt]
+Requires-Dist: requests
 Provides-Extra: extras
+Requires-Dist: lightning-cloud==0.5.65; extra == "extras"
+Requires-Dist: pillow; extra == "extras"
+Requires-Dist: pyarrow; extra == "extras"
+Requires-Dist: torchvision; extra == "extras"
+Requires-Dist: tqdm; extra == "extras"
+Requires-Dist: viztracer; extra == "extras"
 
 <div align="center">
 
 <img alt="Lightning" src="https://pl-flash-data.s3.amazonaws.com/lit_data_logo.webp" width="800px" style="max-width: 100%;">
 
 <br/>
 <br/>
@@ -80,14 +80,20 @@
 
 Install **LitData** with `pip`
 
 ```bash
 pip install litdata
 ```
 
+Install **LitData** with the extras
+
+```bash
+pip install 'litdata[extras]'
+```
+
 ## Quick Start
 
 ### 1. Prepare Your Data
 
 Convert your raw dataset into **LitData Optimized Streaming Format** using the `optimize` operator.
 
 Here is an example with some random images.
```

### Comparing `litdata-0.2.2/README.md` & `litdata-0.2.3/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -39,14 +39,20 @@
 
 Install **LitData** with `pip`
 
 ```bash
 pip install litdata
 ```
 
+Install **LitData** with the extras
+
+```bash
+pip install 'litdata[extras]'
+```
+
 ## Quick Start
 
 ### 1. Prepare Your Data
 
 Convert your raw dataset into **LitData Optimized Streaming Format** using the `optimize` operator.
 
 Here is an example with some random images.
```

### Comparing `litdata-0.2.2/litdata/__about__.py` & `litdata-0.2.3/src/litdata/__about__.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import time
 
-__version__ = "0.2.2"
+__version__ = "0.2.3"
 __author__ = "Lightning AI et al."
 __author_email__ = "pytorch@lightning.ai"
 __license__ = "Apache-2.0"
 __copyright__ = f"Copyright (c) 2023-{time.strftime('%Y')}, {__author__}."
 __homepage__ = "https://github.com/Lightning-AI/lit-data"
 __docs_url__ = "https://lightning.ai/docs/pytorch/stable/"
 # this has to be simple string, see: https://github.com/pypa/twine/issues/522
```

### Comparing `litdata-0.2.2/litdata/constants.py` & `litdata-0.2.3/src/litdata/constants.py`

 * *Files 7% similar despite different names*

```diff
@@ -12,25 +12,26 @@
 # limitations under the License.
 
 import os
 from pathlib import Path
 
 import numpy as np
 import torch
-from lightning_utilities.core.imports import RequirementCache
+
+from litdata.imports import RequirementCache
 
 _INDEX_FILENAME = "index.json"
 _DEFAULT_CHUNK_BYTES = 1 << 26  # 64M B
 _DEFAULT_FAST_DEV_RUN_ITEMS = 10
 _DEFAULT_CACHE_DIR = os.path.join(Path.home(), ".lightning", "chunks")
 
 # This is required for full pytree serialization / deserialization support
 _TORCH_GREATER_EQUAL_2_1_0 = RequirementCache("torch>=2.1.0")
 _VIZ_TRACKER_AVAILABLE = RequirementCache("viztracer")
-_LIGHTNING_CLOUD_LATEST = RequirementCache("lightning-cloud>=0.5.64")
+_LIGHTNING_CLOUD_AVAILABLE = RequirementCache("lightning-cloud")
 _BOTO3_AVAILABLE = RequirementCache("boto3")
 _TORCH_AUDIO_AVAILABLE = RequirementCache("torchaudio")
 _ZSTD_AVAILABLE = RequirementCache("zstd")
 
 # DON'T CHANGE ORDER
 _TORCH_DTYPES_MAPPING = {
     0: torch.float32,
```

### Comparing `litdata-0.2.2/litdata/processing/data_processor.py` & `litdata-0.2.3/src/litdata/processing/data_processor.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,20 @@
+# Copyright The Lightning AI team.
+# Licensed under the Apache License, Version 2.0 (the "License");
+# you may not use this file except in compliance with the License.
+# You may obtain a copy of the License at
+#
+#     http://www.apache.org/licenses/LICENSE-2.0
+#
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS,
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+# See the License for the specific language governing permissions and
+# limitations under the License.
+
 import concurrent
 import json
 import logging
 import os
 import random
 import shutil
 import signal
@@ -15,38 +28,43 @@
 from queue import Empty
 from time import sleep, time
 from typing import Any, Dict, List, Optional, Tuple, TypeVar, Union
 from urllib import parse
 
 import numpy as np
 import torch
-from tqdm.auto import tqdm as _tqdm
 
 from litdata.constants import (
     _BOTO3_AVAILABLE,
     _DEFAULT_FAST_DEV_RUN_ITEMS,
     _INDEX_FILENAME,
     _IS_IN_STUDIO,
-    _LIGHTNING_CLOUD_LATEST,
+    _LIGHTNING_CLOUD_AVAILABLE,
     _TORCH_GREATER_EQUAL_2_1_0,
 )
+from litdata.imports import RequirementCache
 from litdata.processing.readers import BaseReader, StreamingDataLoaderReader
 from litdata.processing.utilities import _create_dataset
 from litdata.streaming import Cache
 from litdata.streaming.cache import Dir
 from litdata.streaming.client import S3Client
 from litdata.streaming.dataloader import StreamingDataLoader
 from litdata.streaming.resolver import _resolve_dir
 from litdata.utilities.broadcast import broadcast_object
 from litdata.utilities.packing import _pack_greedily
 
+_TQDM_AVAILABLE = RequirementCache("tqdm")
+
+if _TQDM_AVAILABLE:
+    from tqdm.auto import tqdm as _tqdm
+
 if _TORCH_GREATER_EQUAL_2_1_0:
     from torch.utils._pytree import tree_flatten, tree_unflatten, treespec_loads
 
-if _LIGHTNING_CLOUD_LATEST:
+if _LIGHTNING_CLOUD_AVAILABLE:
     from lightning_cloud.openapi import V1DatasetType
 
 
 if _BOTO3_AVAILABLE:
     import botocore
 
 logger = logging.Logger(__name__)
@@ -847,14 +865,15 @@
             weights: Provide a list of weights associated to the inputs.
                 This is used to evenly split the work among the workers.
             reader: Map the inputs to worker inputs and provides a read method to read a slice of the data.
 
         """
         self.input_dir = _resolve_dir(input_dir)
         self.output_dir = _resolve_dir(output_dir)
+
         self.num_workers = num_workers or (1 if fast_dev_run else (os.cpu_count() or 1) * 4)
         self.num_downloaders = num_downloaders or 2
         self.num_uploaders = num_uploaders or 5
         self.delete_cached_files = delete_cached_files
         self.fast_dev_run = _get_fast_dev_run() if fast_dev_run is None else fast_dev_run
         self.workers: Any = []
         self.workers_tracker: Dict[int, int] = {}
@@ -869,16 +888,16 @@
             raise ValueError("Either the reader or the weights needs to be defined.")
 
         # Ensure the input dir is the same across all nodes
         self.input_dir = broadcast_object("input_dir", self.input_dir)
 
         if self.output_dir:
             # Ensure the output dir is the same across all nodes
-            self.output_dir = broadcast_object("output_dir", self.output_dir)
-            print(f"Storing the files under {self.output_dir.path}")
+            self.output_dir = broadcast_object("output_dir", self.output_dir, rank=_get_node_rank())
+            print(f"Storing the files under {self.output_dir.path if self.output_dir.path else self.output_dir.url}")
 
         self.random_seed = random_seed
 
     def run(self, data_recipe: DataRecipe) -> None:
         """The `DataProcessor.run(...)` method triggers the data recipe processing over your dataset."""
         if not isinstance(data_recipe, DataRecipe):
             raise ValueError("The provided value should be a data recipe.")
@@ -926,76 +945,85 @@
             workers_user_items = [w[:items_to_keep] for w in workers_user_items]
             print(f"Fast dev run is enabled. Limiting to {items_to_keep} items per process.")
 
         num_items = sum([len(items) for items in workers_user_items])
 
         self._cleanup_cache()
 
-        print(f"Starting {self.num_workers} workers with {num_items} items.")
+        print(
+            f"Starting {self.num_workers} workers with {num_items} items."
+            f" The progress bar is only updated when a worker finishes."
+        )
 
         if self.input_dir is None and self.src_resolver is not None and self.input_dir:
             self.input_dir = self.src_resolver(self.input_dir)
             print(f"The remote_dir is `{self.input_dir}`.")
 
         signal.signal(signal.SIGINT, self._signal_handler)
 
         self._create_process_workers(data_recipe, workers_user_items)
 
         print("Workers are ready ! Starting data processing...")
 
         current_total = 0
-        has_failed = False
-        pbar = _tqdm(
-            desc="Progress",
-            total=num_items,
-            smoothing=0,
-            position=-1,
-            mininterval=1,
-            leave=True,
-            dynamic_ncols=True,
-        )
+        if _TQDM_AVAILABLE:
+            pbar = _tqdm(
+                desc="Progress",
+                total=num_items,
+                smoothing=0,
+                position=-1,
+                mininterval=1,
+                leave=True,
+                dynamic_ncols=True,
+            )
+        num_nodes = _get_num_nodes()
+        node_rank = _get_node_rank()
+        total_num_items = len(user_items)
 
         while True:
             try:
                 error = self.error_queue.get(timeout=0.001)
                 self._exit_on_error(error)
             except Empty:
                 assert self.progress_queue
                 try:
                     index, counter = self.progress_queue.get(timeout=0.001)
                 except Empty:
                     continue
                 self.workers_tracker[index] = counter
                 new_total = sum(self.workers_tracker.values())
 
-            pbar.update(new_total - current_total)
+            if _TQDM_AVAILABLE:
+                pbar.update(new_total - current_total)
 
             current_total = new_total
             if current_total == num_items:
                 break
 
+            if _IS_IN_STUDIO and node_rank == 0:
+                with open("status.json", "w") as f:
+                    json.dump({"progress": str(100 * current_total * num_nodes / total_num_items) + "%"}, f)
+
             # Exit early if all the workers are done.
             # This means there were some kinda of errors.
             if all(not w.is_alive() for w in self.workers):
-                has_failed = True
-                break
+                raise RuntimeError("One of the worker has failed")
 
-        pbar.close()
+        if _TQDM_AVAILABLE:
+            pbar.close()
 
-        num_nodes = _get_num_nodes()
-        node_rank = _get_node_rank()
         # TODO: Understand why it hangs.
         if num_nodes == 1:
             for w in self.workers:
                 w.join(0)
 
         print("Workers are finished.")
         result = data_recipe._done(len(user_items), self.delete_cached_files, self.output_dir)
 
-        if num_nodes == node_rank + 1 and self.output_dir.url and _IS_IN_STUDIO:
+        if num_nodes == node_rank + 1 and self.output_dir.url and _IS_IN_STUDIO and self.input_dir.path:
             assert self.output_dir.path
             _create_dataset(
                 input_dir=self.input_dir.path,
                 storage_dir=self.output_dir.path,
                 dataset_type=V1DatasetType.CHUNKED
                 if isinstance(data_recipe, DataChunkRecipe)
                 else V1DatasetType.TRANSFORMED,
@@ -1006,18 +1034,14 @@
                 compression=result.compression,
                 num_chunks=result.num_chunks,
                 num_bytes_per_chunk=result.num_bytes_per_chunk,
             )
 
         print("Finished data processing!")
 
-        # TODO: Understand why it is required to avoid long shutdown.
-        if _get_num_nodes() > 1:
-            os._exit(int(has_failed))
-
     def _exit_on_error(self, error: str) -> None:
         for w in self.workers:
             w.join(0)
         raise RuntimeError(f"We found the following error {error}.")
 
     def _create_process_workers(self, data_recipe: DataRecipe, workers_user_items: List[List[Any]]) -> None:
         self.progress_queue = Queue()
```

### Comparing `litdata-0.2.2/litdata/processing/functions.py` & `litdata-0.2.3/src/litdata/processing/functions.py`

 * *Files 1% similar despite different names*

```diff
@@ -38,27 +38,27 @@
 if _TORCH_GREATER_EQUAL_2_1_0:
     from torch.utils._pytree import tree_flatten
 
 
 def _get_indexed_paths(data: Any) -> Dict[int, str]:
     flattened_item, _ = tree_flatten(data)
 
-    indexed_paths = {
+    return {
         index: element
         for index, element in enumerate(flattened_item)
         if isinstance(element, str) and os.path.exists(element)
     }
 
-    return indexed_paths
-
 
 def _get_input_dir(inputs: Sequence[Any]) -> Optional[str]:
     indexed_paths = _get_indexed_paths(inputs[0])
 
     if len(indexed_paths) == 0:
+        if len(inputs) < 2:
+            return None
         # Check whether the second element has any input_path
         indexed_paths = _get_indexed_paths(inputs[1])
         if len(indexed_paths) == 0:
             return None
 
         # Every element should have filepaths if any contains one.
         raise ValueError(f"The provided item {inputs[0]} didn't contain any filepaths.")
```

### Comparing `litdata-0.2.2/litdata/processing/readers.py` & `litdata-0.2.3/src/litdata/processing/readers.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,18 +1,37 @@
+# Copyright The Lightning AI team.
+# Licensed under the Apache License, Version 2.0 (the "License");
+# you may not use this file except in compliance with the License.
+# You may obtain a copy of the License at
+#
+#     http://www.apache.org/licenses/LICENSE-2.0
+#
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS,
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+# See the License for the specific language governing permissions and
+# limitations under the License.
+
 import contextlib
 import os
 from abc import ABC, abstractmethod
 from typing import Any, List
 
-from lightning_utilities.core.imports import RequirementCache
-from tqdm import tqdm
-
+from litdata.imports import RequirementCache
 from litdata.streaming.dataloader import StreamingDataLoader
 
 _PYARROW_AVAILABLE = RequirementCache("pyarrow")
+_TQDM_AVAILABLE = RequirementCache("tqdm")
+
+if _TQDM_AVAILABLE:
+    from tqdm.auto import tqdm as _tqdm
+else:
+
+    def _tqdm(iterator: Any) -> Any:
+        yield from iterator
 
 
 class BaseReader(ABC):
     def get_num_nodes(self) -> int:
         return int(os.getenv("DATA_OPTIMIZER_NUM_NODES", 1))
 
     def get_node_rank(self) -> int:
@@ -75,15 +94,15 @@
 
         for filepath in filepaths:
             num_rows = self._get_num_rows(filepath)
 
             table = None
             parquet_filename = os.path.basename(filepath)
 
-            for start in tqdm(range(0, num_rows, self.num_rows)):
+            for start in _tqdm(range(0, num_rows, self.num_rows)):
                 end = min(start + self.num_rows, num_rows)
                 chunk_filepath = os.path.join(cache_folder, f"{start}_{end}_{parquet_filename}")
                 new_items.append(chunk_filepath)
 
                 if os.path.exists(chunk_filepath):
                     continue
```

### Comparing `litdata-0.2.2/litdata/streaming/__init__.py` & `litdata-0.2.3/src/litdata/streaming/__init__.py`

 * *Files identical despite different names*

### Comparing `litdata-0.2.2/litdata/streaming/cache.py` & `litdata-0.2.3/src/litdata/streaming/cache.py`

 * *Files 6% similar despite different names*

```diff
@@ -13,15 +13,14 @@
 
 import logging
 import os
 from typing import Any, Dict, List, Optional, Tuple, Union
 
 from litdata.constants import (
     _INDEX_FILENAME,
-    _LIGHTNING_CLOUD_LATEST,
     _TORCH_GREATER_EQUAL_2_1_0,
 )
 from litdata.streaming.item_loader import BaseItemLoader
 from litdata.streaming.reader import BinaryReader
 from litdata.streaming.resolver import Dir, _resolve_dir
 from litdata.streaming.sampler import ChunkedIndex
 from litdata.streaming.serializers import Serializer
@@ -56,20 +55,14 @@
             serializers: Provide your own serializers.
 
         """
         super().__init__()
         if not _TORCH_GREATER_EQUAL_2_1_0:
             raise ModuleNotFoundError("PyTorch version 2.1 or higher is required to use the cache.")
 
-        if not _LIGHTNING_CLOUD_LATEST:
-            raise ModuleNotFoundError(
-                "The `lightning-cloud` package in your environement is out-dated."
-                " Run: `pip install -U lightning-cloud` to resolve this."
-            )
-
         input_dir = _resolve_dir(input_dir)
         self._cache_dir = input_dir.path
         assert self._cache_dir
         self._writer = BinaryWriter(
             self._cache_dir,
             chunk_size=chunk_size,
             chunk_bytes=chunk_bytes,
```

### Comparing `litdata-0.2.2/litdata/streaming/client.py` & `litdata-0.2.3/src/litdata/streaming/client.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,7 +1,20 @@
+# Copyright The Lightning AI team.
+# Licensed under the Apache License, Version 2.0 (the "License");
+# you may not use this file except in compliance with the License.
+# You may obtain a copy of the License at
+#
+#     http://www.apache.org/licenses/LICENSE-2.0
+#
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS,
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+# See the License for the specific language governing permissions and
+# limitations under the License.
+
 import os
 from time import time
 from typing import Any, Optional
 
 from litdata.constants import _BOTO3_AVAILABLE, _IS_IN_STUDIO
 
 if _BOTO3_AVAILABLE:
```

### Comparing `litdata-0.2.2/litdata/streaming/combined.py` & `litdata-0.2.3/src/litdata/streaming/combined.py`

 * *Files identical despite different names*

### Comparing `litdata-0.2.2/litdata/streaming/compression.py` & `litdata-0.2.3/src/litdata/streaming/compression.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,23 +10,21 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from abc import ABC, abstractmethod
 from typing import Dict, TypeVar
 
-from lightning_utilities.core.imports import requires
-
 from litdata.constants import _ZSTD_AVAILABLE
 
+TCompressor = TypeVar("TCompressor", bound="Compressor")
+
 if _ZSTD_AVAILABLE:
     import zstd
 
-TCompressor = TypeVar("TCompressor", bound="Compressor")
-
 
 class Compressor(ABC):
     """Base class for compression algorithm."""
 
     @abstractmethod
     def compress(self, data: bytes) -> bytes:
         pass
@@ -40,17 +38,18 @@
     def register(cls, compressors: Dict[str, "Compressor"]) -> None:
         pass
 
 
 class ZSTDCompressor(Compressor):
     """Compressor for the zstd package."""
 
-    @requires("zstd")
     def __init__(self, level: int) -> None:
         super().__init__()
+        if not _ZSTD_AVAILABLE:
+            raise ModuleNotFoundError()
         self.level = level
         self.extension = "zstd"
 
     @property
     def name(self) -> str:
         return f"{self.extension}:{self.level}"
```

### Comparing `litdata-0.2.2/litdata/streaming/config.py` & `litdata-0.2.3/src/litdata/streaming/config.py`

 * *Files identical despite different names*

### Comparing `litdata-0.2.2/litdata/streaming/dataloader.py` & `litdata-0.2.3/src/litdata/streaming/dataloader.py`

 * *Files identical despite different names*

### Comparing `litdata-0.2.2/litdata/streaming/dataset.py` & `litdata-0.2.3/src/litdata/streaming/dataset.py`

 * *Files 0% similar despite different names*

```diff
@@ -315,30 +315,28 @@
         if _is_in_dataloader_worker():
             raise RuntimeError("The method `state_dict` should only be called in the main process.")
 
         if self._state_dict is not None:
             self._state_dict["num_samples_yielded"] = num_samples_yielded
             return self._state_dict
 
-        state = {
+        return {
             "num_samples_yielded": num_samples_yielded,
             "num_workers": num_workers,
             "batch_size": batch_size,
             "current_epoch": self.current_epoch,
             "input_dir_path": self.input_dir.path,
             "input_dir_url": self.input_dir.url,
             "item_loader": self.item_loader.state_dict() if self.item_loader else None,
             "drop_last": self.drop_last,
             "seed": self.seed,
             "world_size": self.distributed_env.world_size,
             "shuffle": self.shuffle,
         }
 
-        return state
-
     def load_state_dict(self, state_dict: Dict[str, Any]) -> None:
         if state_dict:
             # the state is restored within the workers
             self._state_dict = state_dict
 
     def _validate_state_dict(self) -> None:
         assert self._state_dict
@@ -398,15 +396,15 @@
             raise ValueError(
                 "The provided `drop_last` state doesn't match the current one. "
                 f"Found `{self.drop_last}` instead of `{state['drop_last']}`."
             )
 
 
 def _try_create_cache_dir(input_dir: Optional[str]) -> Optional[str]:
-    hash_object = hashlib.md5((input_dir or "").encode())
+    hash_object = hashlib.md5((input_dir or "").encode())  # noqa: S324
     if "LIGHTNING_CLUSTER_ID" not in os.environ or "LIGHTNING_CLOUD_PROJECT_ID" not in os.environ:
         cache_dir = os.path.join(_DEFAULT_CACHE_DIR, hash_object.hexdigest())
         os.makedirs(cache_dir, exist_ok=True)
         return cache_dir
     cache_dir = os.path.join("/cache", "chunks", hash_object.hexdigest())
     os.makedirs(cache_dir, exist_ok=True)
     return cache_dir
```

### Comparing `litdata-0.2.2/litdata/streaming/downloader.py` & `litdata-0.2.3/src/litdata/streaming/downloader.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
+
 import os
 import shutil
 import subprocess
 from abc import ABC
 from typing import Any, Dict, List
 from urllib import parse
```

### Comparing `litdata-0.2.2/litdata/streaming/item_loader.py` & `litdata-0.2.3/src/litdata/streaming/item_loader.py`

 * *Files identical despite different names*

### Comparing `litdata-0.2.2/litdata/streaming/reader.py` & `litdata-0.2.3/src/litdata/streaming/reader.py`

 * *Files 0% similar despite different names*

```diff
@@ -32,15 +32,15 @@
 if _TORCH_GREATER_EQUAL_2_1_0:
     pass
 
 
 logger = Logger(__name__)
 
 
-_END_TOKEN = "END"
+_END_TOKEN = "END"  # noqa: S105
 
 # Note: The timeout here should not be too short. We need to prevent the caller from aggressively
 # querying the queue and consuming too many CPU cycles.
 _DEFAULT_TIMEOUT = 0.1
 _LONG_DEFAULT_TIMEOUT = 5
 
 
@@ -245,15 +245,17 @@
                 self._prepare_thread.download([index.chunk_index])
 
             if self._last_chunk_index is None:
                 self._last_chunk_index = index.chunk_index
 
         # Fetch the element
         chunk_filepath, begin, chunk_bytes = self.config[index]
-        item = self._item_loader.load_item_from_chunk(index.index, index.chunk_index, chunk_filepath, begin, chunk_bytes)
+        item = self._item_loader.load_item_from_chunk(
+            index.index, index.chunk_index, chunk_filepath, begin, chunk_bytes
+        )
 
         # We need to request deletion after the latest element has been loaded.
         # Otherwise, this could trigger segmentation fault error depending on the item loader used.
         if self._config and self._config._remote_dir and index.chunk_index != self._last_chunk_index:
             assert self._prepare_thread
             assert self._last_chunk_index is not None
```

### Comparing `litdata-0.2.2/litdata/streaming/resolver.py` & `litdata-0.2.3/src/litdata/streaming/resolver.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,35 @@
+# Copyright The Lightning AI team.
+# Licensed under the Apache License, Version 2.0 (the "License");
+# you may not use this file except in compliance with the License.
+# You may obtain a copy of the License at
+#
+#     http://www.apache.org/licenses/LICENSE-2.0
+#
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS,
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+# See the License for the specific language governing permissions and
+# limitations under the License.
+
 import datetime
 import os
 import re
 import sys
 from dataclasses import dataclass
 from pathlib import Path
 from time import sleep
-from typing import Optional, Union
+from typing import Any, Optional, Union
 from urllib import parse
 
-from lightning_cloud.openapi import V1CloudSpace
-from lightning_cloud.rest_client import LightningClient
+from litdata.constants import _LIGHTNING_CLOUD_AVAILABLE
+
+if _LIGHTNING_CLOUD_AVAILABLE:
+    from lightning_cloud.rest_client import LightningClient
 
-# To avoid adding lightning_utilities as a dependency for now.
 try:
     import boto3
     import botocore
 
     _BOTO3_AVAILABLE = True
 except Exception:
     _BOTO3_AVAILABLE = False
@@ -77,15 +91,15 @@
 
     if dir_path_absolute.startswith("/teamspace/datasets") and len(dir_path_absolute.split("/")) > 3:
         return _resolve_datasets(dir_path_absolute)
 
     return Dir(path=dir_path_absolute, url=None)
 
 
-def _match_studio(target_id: Optional[str], target_name: Optional[str], cloudspace: V1CloudSpace) -> bool:
+def _match_studio(target_id: Optional[str], target_name: Optional[str], cloudspace: Any) -> bool:
     if cloudspace.name is not None and target_name is not None and cloudspace.name.lower() == target_name.lower():
         return True
 
     if target_id is not None and cloudspace.id == target_id:
         return True
 
     if (
```

### Comparing `litdata-0.2.2/litdata/streaming/sampler.py` & `litdata-0.2.3/src/litdata/streaming/sampler.py`

 * *Files 0% similar despite different names*

```diff
@@ -176,22 +176,24 @@
         indices_per_workers: List[List[ChunkedIndex]] = [[] for _ in range(self._num_workers)]
 
         for i, (chunk_index, chunk_interval) in enumerate(zip(shuffled_indexes, shuffled_chunk_intervals)):
             worker_id = i % self._num_workers
             interval_indices = np.arange(chunk_interval[0], chunk_interval[1])
             shuffled_interval_indices = np.random.permutation(interval_indices).tolist()
             is_empty = len(indices_per_workers[worker_id]) == 0
-            indices_per_workers[worker_id].extend([
-                ChunkedIndex(
-                    index,
-                    chunk_index,
-                    chunk_indexes=chunks_per_workers[worker_id] if j == 0 and is_empty else None,
-                )
-                for j, index in enumerate(shuffled_interval_indices)
-            ])
+            indices_per_workers[worker_id].extend(
+                [
+                    ChunkedIndex(
+                        index,
+                        chunk_index,
+                        chunk_indexes=chunks_per_workers[worker_id] if j == 0 and is_empty else None,
+                    )
+                    for j, index in enumerate(shuffled_interval_indices)
+                ]
+            )
 
         indices_per_workers_splitted = [self._chunk_list(indices, self._batch_size) for indices in indices_per_workers]
 
         yield from self.__iter_indices_per_workers__(indices_per_workers_splitted)
 
     def __len__(self) -> int:
         return self._length
```

### Comparing `litdata-0.2.2/litdata/streaming/serializers.py` & `litdata-0.2.3/src/litdata/streaming/serializers.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,32 +17,42 @@
 import tempfile
 from abc import ABC, abstractmethod
 from collections import OrderedDict
 from typing import Any, Dict, Optional, Tuple, Union
 
 import numpy as np
 import torch
-from lightning_utilities.core.imports import RequirementCache
 
 from litdata.constants import _NUMPY_DTYPES_MAPPING, _TORCH_DTYPES_MAPPING
+from litdata.imports import RequirementCache
 
 _PIL_AVAILABLE = RequirementCache("PIL")
 _TORCH_VISION_AVAILABLE = RequirementCache("torchvision")
 _AV_AVAILABLE = RequirementCache("av")
 
 if _PIL_AVAILABLE:
     from PIL import Image
     from PIL.GifImagePlugin import GifImageFile
     from PIL.JpegImagePlugin import JpegImageFile
     from PIL.PngImagePlugin import PngImageFile
     from PIL.WebPImagePlugin import WebPImageFile
 else:
-    Image = None
-    JpegImageFile = None
-    PngImageFile = None
+
+    class Image:  # type: ignore
+        Image = None
+
+    class JpegImageFile:  # type: ignore
+        pass
+
+    class PngImageFile:  # type: ignore
+        pass
+
+    class WebPImageFile:  # type: ignore
+        pass
+
 
 if _TORCH_VISION_AVAILABLE:
     from torchvision.io import decode_jpeg
     from torchvision.transforms.functional import pil_to_tensor
 
 
 class Serializer(ABC):
@@ -67,15 +77,15 @@
     def setup(self, metadata: Any) -> None:
         pass
 
 
 class PILSerializer(Serializer):
     """The PILSerializer serialize and deserialize PIL Image to and from bytes."""
 
-    def serialize(self, item: Image) -> Tuple[bytes, Optional[str]]:
+    def serialize(self, item: Any) -> Tuple[bytes, Optional[str]]:
         mode = item.mode.encode("utf-8")
         width, height = item.size
         raw = item.tobytes()
         ints = np.array([width, height, len(mode)], np.uint32)
         return ints.tobytes() + mode + raw, None
 
     @classmethod
@@ -91,15 +101,15 @@
     def can_serialize(self, item: Any) -> bool:
         return bool(_PIL_AVAILABLE) and isinstance(item, Image.Image) and not isinstance(item, JpegImageFile)
 
 
 class JPEGSerializer(Serializer):
     """The JPEGSerializer serialize and deserialize JPEG image to and from bytes."""
 
-    def serialize(self, item: Image) -> Tuple[bytes, Optional[str]]:
+    def serialize(self, item: Any) -> Tuple[bytes, Optional[str]]:
         if isinstance(item, JpegImageFile):
             if not hasattr(item, "filename"):
                 raise ValueError(
                     "The JPEG Image's filename isn't defined. HINT: Open the image in your Dataset __getitem__ method."
                 )
             if item.filename and os.path.isfile(item.filename):
                 # read the content of the file directly
@@ -268,15 +278,15 @@
 class PickleSerializer(Serializer):
     """The PickleSerializer serialize and deserialize python objects to and from bytes."""
 
     def serialize(self, item: Any) -> Tuple[bytes, Optional[str]]:
         return pickle.dumps(item), None
 
     def deserialize(self, data: bytes) -> Any:
-        return pickle.loads(data)
+        return pickle.loads(data)  # noqa: S301
 
     def can_serialize(self, _: Any) -> bool:
         return True
 
 
 class FileSerializer(Serializer):
     def serialize(self, filepath: str) -> Tuple[bytes, Optional[str]]:
@@ -359,30 +369,32 @@
     def __init__(self) -> None:
         super().__init__(np.float64)
 
     def can_serialize(self, data: float) -> bool:
         return isinstance(data, float)
 
 
-_SERIALIZERS = OrderedDict(**{
-    "str": StringSerializer(),
-    "int": IntegerSerializer(),
-    "float": FloatSerializer(),
-    "video": VideoSerializer(),
-    "tif": FileSerializer(),
-    "file": FileSerializer(),
-    "pil": PILSerializer(),
-    "jpeg": JPEGSerializer(),
-    "bytes": BytesSerializer(),
-    "no_header_numpy": NoHeaderNumpySerializer(),
-    "numpy": NumpySerializer(),
-    "no_header_tensor": NoHeaderTensorSerializer(),
-    "tensor": TensorSerializer(),
-    "pickle": PickleSerializer(),
-})
+_SERIALIZERS = OrderedDict(
+    **{
+        "str": StringSerializer(),
+        "int": IntegerSerializer(),
+        "float": FloatSerializer(),
+        "video": VideoSerializer(),
+        "tif": FileSerializer(),
+        "file": FileSerializer(),
+        "pil": PILSerializer(),
+        "jpeg": JPEGSerializer(),
+        "bytes": BytesSerializer(),
+        "no_header_numpy": NoHeaderNumpySerializer(),
+        "numpy": NumpySerializer(),
+        "no_header_tensor": NoHeaderTensorSerializer(),
+        "tensor": TensorSerializer(),
+        "pickle": PickleSerializer(),
+    }
+)
 
 
 def _get_serializers(serializers: Optional[Dict[str, Serializer]]) -> Dict[str, Serializer]:
     if serializers:
         serializers = OrderedDict(**serializers)
         serializers.update(_SERIALIZERS)
     else:
```

### Comparing `litdata-0.2.2/litdata/streaming/shuffle.py` & `litdata-0.2.3/src/litdata/streaming/shuffle.py`

 * *Files identical despite different names*

### Comparing `litdata-0.2.2/litdata/streaming/writer.py` & `litdata-0.2.3/src/litdata/streaming/writer.py`

 * *Files 0% similar despite different names*

```diff
@@ -126,22 +126,21 @@
             else:
                 self._worker_env = _WorkerEnv.detect()
                 self._rank = self._distributed_env.global_rank * self._worker_env.world_size + self._worker_env.rank
         return self._rank
 
     def get_config(self) -> Dict[str, Any]:
         """Returns the config of the writer."""
-        out = {
+        return {
             "compression": self._compression,
             "chunk_size": self._chunk_size,
             "chunk_bytes": self._chunk_bytes,
             "data_format": self._data_format,
             "data_spec": treespec_dumps(self._data_spec) if self._data_spec else None,
         }
-        return out
 
     def serialize(self, items: Any) -> Tuple[bytes, Optional[int]]:
         """Serialize a dictionary into its binary format."""
 
         # Flatten the items provided by the users
         flattened, data_spec = tree_flatten(items)
 
@@ -287,20 +286,21 @@
         self._serialized_items[index] = Item(
             index=index,
             data=data,
             bytes=len(data),
             dim=dim,
         )
 
-        if self._should_write():
-            filepath = os.path.join(self._cache_dir, self.get_chunk_filename())
-            self.write_chunk()
-            self._min_index = None
-            self._max_index = None
-            return filepath
+        if not self._should_write():
+            return None
+        filepath = os.path.join(self._cache_dir, self.get_chunk_filename())
+        self.write_chunk()
+        self._min_index = None
+        self._max_index = None
+        return filepath
 
     def _should_write(self) -> bool:
         # TODO: Misleading method name, it modifies `self._min_index` and `self._max_index`!
         if not self._serialized_items:
             return False
         indexes = list(self._serialized_items.keys())
         self._min_index = index = indexes[0] if len(indexes) == 1 else min(*indexes)
```

### Comparing `litdata-0.2.2/litdata/utilities/broadcast.py` & `litdata-0.2.3/src/litdata/utilities/broadcast.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import json
 import os
 import pickle
 from logging import Logger
+from time import sleep
 from typing import Any, Callable, Dict, Optional
 from urllib.parse import urljoin
 
 import requests
 import urllib3
 
 # for backwards compatibility
@@ -118,42 +119,54 @@
 
         lightning_app_state_url = os.getenv("LIGHTNING_APP_STATE_URL")
         if lightning_app_state_url is None:
             raise RuntimeError("The `LIGHTNING_APP_STATE_URL` should be set.")
 
         self.private_client: _HTTPClient = _HTTPClient(lightning_app_state_url, auth_token=token, use_retry=False)
 
-    def set_and_get(self, key: str, value: Any) -> Any:
+    def set_and_get(self, key: str, value: Any, rank: Optional[int] = None) -> Any:
         payload = {"key": key, "value": pickle.dumps(value, 0).decode()}
 
+        if rank is not None:
+            payload["rank"] = str(rank)
+
         # Try the public address first
         try:
             resp = self.public_client.post("/broadcast", json=payload)
         except (requests.exceptions.ConnectionError, urllib3.exceptions.MaxRetryError):
             # fallback to the private one
             resp = self.private_client.post("/broadcast", json=payload)
 
         if resp.status_code != 200:
             raise RuntimeError(f"Failed to broadcast the following {key=} {value=}.")
-        return pickle.loads(bytes(resp.json()["value"], "utf-8"))
+
+        value = resp.json()["value"]
+        if value is None:
+            return value
+        return pickle.loads(bytes(value, "utf-8"))  # noqa: S301
 
 
-def broadcast_object(key: str, obj: Any) -> Any:
+def broadcast_object(key: str, obj: Any, rank: Optional[int] = None) -> Any:
     """This function enables to broadcast object across machines."""
     if os.getenv("LIGHTNING_APP_EXTERNAL_URL") is not None:
-        return _ImmutableDistributedMap().set_and_get(key, obj)
+        value = None
+        while value is None:
+            value = _ImmutableDistributedMap().set_and_get(key, obj, rank)
+            if value is None:
+                sleep(3)
+        return value
     return obj
 
 
 def _get_token() -> Optional[str]:
     """This function tries to retrieve a temporary token."""
     if os.getenv("LIGHTNING_CLOUD_URL") is None:
         return None
 
     payload = {"apiKey": os.getenv("LIGHTNING_API_KEY"), "username": os.getenv("LIGHTNING_USERNAME")}
     url_login = os.getenv("LIGHTNING_CLOUD_URL", "") + "/v1/auth/login"
-    res = requests.post(url_login, data=json.dumps(payload))
+    res = requests.post(url_login, data=json.dumps(payload))  # noqa: S113
     if "token" not in res.json():
         raise RuntimeError(
             f"You haven't properly setup your environment variables with {url_login} and data: \n{payload}"
         )
     return res.json()["token"]
```

### Comparing `litdata-0.2.2/litdata/utilities/env.py` & `litdata-0.2.3/src/litdata/utilities/env.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,7 +1,20 @@
+# Copyright The Lightning AI team.
+# Licensed under the Apache License, Version 2.0 (the "License");
+# you may not use this file except in compliance with the License.
+# You may obtain a copy of the License at
+#
+#     http://www.apache.org/licenses/LICENSE-2.0
+#
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS,
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+# See the License for the specific language governing permissions and
+# limitations under the License.
+
 import os
 from typing import Callable, Optional
 
 import torch
 from torch.utils.data import get_worker_info as torch_get_worker_info
```

### Comparing `litdata-0.2.2/litdata/utilities/shuffle.py` & `litdata-0.2.3/src/litdata/utilities/shuffle.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,7 +1,20 @@
+# Copyright The Lightning AI team.
+# Licensed under the Apache License, Version 2.0 (the "License");
+# you may not use this file except in compliance with the License.
+# You may obtain a copy of the License at
+#
+#     http://www.apache.org/licenses/LICENSE-2.0
+#
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS,
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+# See the License for the specific language governing permissions and
+# limitations under the License.
+
 from typing import Any, List, Tuple
 
 import numpy as np
 
 from litdata.utilities.env import _DistributedEnv
```

### Comparing `litdata-0.2.2/litdata.egg-info/PKG-INFO` & `litdata-0.2.3/src/litdata.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: litdata
-Version: 0.2.2
+Version: 0.2.3
 Summary: The Deep Learning framework to train, deploy, and ship AI products Lightning fast.
 Home-page: https://github.com/Lightning-AI/lit-data
 Download-URL: https://github.com/Lightning-AI/litdata
 Author: Lightning AI et al.
 Author-email: pytorch@lightning.ai
 License: Apache-2.0
 Project-URL: Bug Tracker, https://github.com/Lightning-AI/litdata/issues
@@ -22,26 +22,26 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: lightning-cloud==0.5.64
-Requires-Dist: lightning-utilities<0.11.0,>=0.8.0
 Requires-Dist: torch>=2.1.0
 Requires-Dist: filelock
-Requires-Dist: tqdm
 Requires-Dist: numpy
-Requires-Dist: torchvision
-Requires-Dist: pillow
-Requires-Dist: viztracer
-Requires-Dist: pyarrow
 Requires-Dist: boto3[crt]
+Requires-Dist: requests
 Provides-Extra: extras
+Requires-Dist: lightning-cloud==0.5.65; extra == "extras"
+Requires-Dist: pillow; extra == "extras"
+Requires-Dist: pyarrow; extra == "extras"
+Requires-Dist: torchvision; extra == "extras"
+Requires-Dist: tqdm; extra == "extras"
+Requires-Dist: viztracer; extra == "extras"
 
 <div align="center">
 
 <img alt="Lightning" src="https://pl-flash-data.s3.amazonaws.com/lit_data_logo.webp" width="800px" style="max-width: 100%;">
 
 <br/>
 <br/>
@@ -80,14 +80,20 @@
 
 Install **LitData** with `pip`
 
 ```bash
 pip install litdata
 ```
 
+Install **LitData** with the extras
+
+```bash
+pip install 'litdata[extras]'
+```
+
 ## Quick Start
 
 ### 1. Prepare Your Data
 
 Convert your raw dataset into **LitData Optimized Streaming Format** using the `optimize` operator.
 
 Here is an example with some random images.
```

### Comparing `litdata-0.2.2/litdata.egg-info/SOURCES.txt` & `litdata-0.2.3/src/litdata.egg-info/SOURCES.txt`

 * *Files 27% similar despite different names*

```diff
@@ -1,43 +1,43 @@
 CHANGELOG.md
 LICENSE
 MANIFEST.in
 README.md
 requirements.txt
 setup.py
-litdata/CHANGELOG.md
-litdata/__about__.py
-litdata/__init__.py
-litdata/constants.py
-litdata.egg-info/PKG-INFO
-litdata.egg-info/SOURCES.txt
-litdata.egg-info/dependency_links.txt
-litdata.egg-info/not-zip-safe
-litdata.egg-info/requires.txt
-litdata.egg-info/top_level.txt
-litdata/processing/__init__.py
-litdata/processing/data_processor.py
-litdata/processing/functions.py
-litdata/processing/readers.py
-litdata/processing/utilities.py
-litdata/streaming/__init__.py
-litdata/streaming/cache.py
-litdata/streaming/client.py
-litdata/streaming/combined.py
-litdata/streaming/compression.py
-litdata/streaming/config.py
-litdata/streaming/dataloader.py
-litdata/streaming/dataset.py
-litdata/streaming/downloader.py
-litdata/streaming/item_loader.py
-litdata/streaming/reader.py
-litdata/streaming/resolver.py
-litdata/streaming/sampler.py
-litdata/streaming/serializers.py
-litdata/streaming/shuffle.py
-litdata/streaming/writer.py
-litdata/utilities/__init__.py
-litdata/utilities/broadcast.py
-litdata/utilities/env.py
-litdata/utilities/format.py
-litdata/utilities/packing.py
-litdata/utilities/shuffle.py
+src/litdata/__about__.py
+src/litdata/__init__.py
+src/litdata/constants.py
+src/litdata/imports.py
+src/litdata.egg-info/PKG-INFO
+src/litdata.egg-info/SOURCES.txt
+src/litdata.egg-info/dependency_links.txt
+src/litdata.egg-info/not-zip-safe
+src/litdata.egg-info/requires.txt
+src/litdata.egg-info/top_level.txt
+src/litdata/processing/__init__.py
+src/litdata/processing/data_processor.py
+src/litdata/processing/functions.py
+src/litdata/processing/readers.py
+src/litdata/processing/utilities.py
+src/litdata/streaming/__init__.py
+src/litdata/streaming/cache.py
+src/litdata/streaming/client.py
+src/litdata/streaming/combined.py
+src/litdata/streaming/compression.py
+src/litdata/streaming/config.py
+src/litdata/streaming/dataloader.py
+src/litdata/streaming/dataset.py
+src/litdata/streaming/downloader.py
+src/litdata/streaming/item_loader.py
+src/litdata/streaming/reader.py
+src/litdata/streaming/resolver.py
+src/litdata/streaming/sampler.py
+src/litdata/streaming/serializers.py
+src/litdata/streaming/shuffle.py
+src/litdata/streaming/writer.py
+src/litdata/utilities/__init__.py
+src/litdata/utilities/broadcast.py
+src/litdata/utilities/env.py
+src/litdata/utilities/format.py
+src/litdata/utilities/packing.py
+src/litdata/utilities/shuffle.py
```

### Comparing `litdata-0.2.2/setup.py` & `litdata-0.2.3/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 #!/usr/bin/env python
 import glob
 import os
 from importlib.util import module_from_spec, spec_from_file_location
 from pathlib import Path
 
 from pkg_resources import parse_requirements
-from setuptools import setup
+from setuptools import find_packages, setup
 
 _PATH_ROOT = os.path.dirname(__file__)
+_PATH_SOURCE = os.path.join(_PATH_ROOT, "src")
 _PATH_REQUIRES = os.path.join(_PATH_ROOT, "requirements")
 
 
 def _load_py_module(fname, pkg="litdata"):
-    spec = spec_from_file_location(os.path.join(pkg, fname), os.path.join(_PATH_ROOT, pkg, fname))
+    spec = spec_from_file_location(os.path.join(pkg, fname), os.path.join(_PATH_SOURCE, pkg, fname))
     py = module_from_spec(spec)
     spec.loader.exec_module(py)
     return py
 
 
 def _load_requirements(path_dir: str = _PATH_ROOT, file_name: str = "requirements.txt") -> list:
     reqs = parse_requirements(open(os.path.join(path_dir, file_name)).readlines())
@@ -56,14 +57,16 @@
     description=about.__docs__,
     author=about.__author__,
     author_email=about.__author_email__,
     url=about.__homepage__,
     download_url="https://github.com/Lightning-AI/litdata",
     license=about.__license__,
     long_description=readme,
+    packages=find_packages(where="src"),
+    package_dir={"": "src"},
     long_description_content_type="text/markdown",
     include_package_data=True,
     zip_safe=False,
     keywords=["deep learning", "pytorch", "AI", "streaming", "cloud", "data processing"],
     python_requires=">=3.8",
     setup_requires=["wheel"],
     install_requires=_load_requirements(),
```

