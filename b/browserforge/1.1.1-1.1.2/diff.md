# Comparing `tmp/browserforge-1.1.1.tar.gz` & `tmp/browserforge-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "browserforge-1.1.1.tar", max compression
+gzip compressed data, was "browserforge-1.1.2.tar", max compression
```

## Comparing `browserforge-1.1.1.tar` & `browserforge-1.1.2.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rw-r--r--   0        0        0     1097 2024-03-13 07:45:41.744935 browserforge-1.1.1/browserforge/__main__.py
--rw-r--r--   0        0        0    10067 2024-03-18 03:43:41.178037 browserforge-1.1.1/browserforge/bayesian_network.py
--rw-r--r--   0        0        0     7238 2024-03-18 03:43:45.511398 browserforge-1.1.1/browserforge/download.py
--rw-r--r--   0        0        0      280 2024-03-15 00:28:56.972014 browserforge-1.1.1/browserforge/fingerprints/__init__.py
--rw-r--r--   0        0        0        0 2024-03-13 07:45:41.746937 browserforge-1.1.1/browserforge/fingerprints/data/__init__.py
--rw-r--r--   0        0        0    12425 2024-03-18 03:43:31.901438 browserforge-1.1.1/browserforge/fingerprints/generator.py
--rw-r--r--   0        0        0      131 2024-03-13 07:45:41.747980 browserforge-1.1.1/browserforge/headers/__init__.py
--rw-r--r--   0        0        0        0 2024-03-13 07:45:41.748943 browserforge-1.1.1/browserforge/headers/data/__init__.py
--rw-r--r--   0        0        0    21339 2024-03-18 03:43:54.677570 browserforge-1.1.1/browserforge/headers/generator.py
--rw-r--r--   0        0        0     1218 2024-03-18 03:44:01.529593 browserforge-1.1.1/browserforge/headers/utils.py
--rw-r--r--   0        0        0       21 2024-03-18 03:16:48.230584 browserforge-1.1.1/browserforge/injectors/__init__.py
--rw-r--r--   0        0        0      325 2024-03-14 07:58:17.918717 browserforge-1.1.1/browserforge/injectors/data/__init__.py
--rw-r--r--   0        0        0     6512 2024-03-14 04:06:29.000000 browserforge-1.1.1/browserforge/injectors/data/utils.js.xz
--rw-r--r--   0        0        0      146 2024-03-18 03:15:53.345716 browserforge-1.1.1/browserforge/injectors/playwright/__init__.py
--rw-r--r--   0        0        0     3525 2024-03-18 03:38:43.618886 browserforge-1.1.1/browserforge/injectors/playwright/injector.py
--rw-r--r--   0        0        0      125 2024-03-18 03:02:16.660740 browserforge-1.1.1/browserforge/injectors/pyppeteer/__init__.py
--rw-r--r--   0        0        0     2454 2024-03-18 03:09:14.200001 browserforge-1.1.1/browserforge/injectors/pyppeteer/injector.py
--rw-r--r--   0        0        0      315 2024-03-18 03:47:07.934145 browserforge-1.1.1/browserforge/injectors/undetected_playwright/__init__.py
--rw-r--r--   0        0        0     3580 2024-03-18 03:39:13.178650 browserforge-1.1.1/browserforge/injectors/undetected_playwright/injector.py
--rw-r--r--   0        0        0     4245 2024-03-18 03:09:14.177479 browserforge-1.1.1/browserforge/injectors/utils.py
--rw-r--r--   0        0        0        0 2024-03-18 02:55:50.343869 browserforge-1.1.1/browserforge/py.typed
--rw-r--r--   0        0        0    11558 2024-03-13 07:45:41.743936 browserforge-1.1.1/LICENSE
--rw-r--r--   0        0        0      827 2024-03-18 03:19:08.667601 browserforge-1.1.1/pyproject.toml
--rw-r--r--   0        0        0    28273 2024-03-18 03:45:40.565667 browserforge-1.1.1/README.md
--rw-r--r--   0        0        0    28774 1970-01-01 00:00:00.000000 browserforge-1.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1097 2024-04-03 03:11:08.160280 browserforge-1.1.2/browserforge/__main__.py
+-rw-r--r--   0        0        0    10067 2024-04-03 03:11:08.161282 browserforge-1.1.2/browserforge/bayesian_network.py
+-rw-r--r--   0        0        0     7238 2024-04-03 03:11:08.161282 browserforge-1.1.2/browserforge/download.py
+-rw-r--r--   0        0        0      280 2024-04-03 03:11:08.162282 browserforge-1.1.2/browserforge/fingerprints/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-03 03:11:08.162282 browserforge-1.1.2/browserforge/fingerprints/data/__init__.py
+-rw-r--r--   0        0        0    12425 2024-04-03 03:11:08.163725 browserforge-1.1.2/browserforge/fingerprints/generator.py
+-rw-r--r--   0        0        0      131 2024-04-03 03:11:08.163725 browserforge-1.1.2/browserforge/headers/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-03 03:11:08.163725 browserforge-1.1.2/browserforge/headers/data/__init__.py
+-rw-r--r--   0        0        0    21446 2024-04-03 03:11:08.165113 browserforge-1.1.2/browserforge/headers/generator.py
+-rw-r--r--   0        0        0     1218 2024-04-03 03:11:08.165113 browserforge-1.1.2/browserforge/headers/utils.py
+-rw-r--r--   0        0        0       21 2024-04-03 03:11:08.165113 browserforge-1.1.2/browserforge/injectors/__init__.py
+-rw-r--r--   0        0        0      325 2024-04-03 03:11:08.165113 browserforge-1.1.2/browserforge/injectors/data/__init__.py
+-rw-r--r--   0        0        0     6512 2024-04-03 03:11:08.166381 browserforge-1.1.2/browserforge/injectors/data/utils.js.xz
+-rw-r--r--   0        0        0      146 2024-04-03 03:11:08.166381 browserforge-1.1.2/browserforge/injectors/playwright/__init__.py
+-rw-r--r--   0        0        0     3525 2024-04-03 03:11:08.166381 browserforge-1.1.2/browserforge/injectors/playwright/injector.py
+-rw-r--r--   0        0        0      125 2024-04-03 03:11:08.166381 browserforge-1.1.2/browserforge/injectors/pyppeteer/__init__.py
+-rw-r--r--   0        0        0     2454 2024-04-03 03:11:08.167667 browserforge-1.1.2/browserforge/injectors/pyppeteer/injector.py
+-rw-r--r--   0        0        0      315 2024-04-03 03:11:08.167667 browserforge-1.1.2/browserforge/injectors/undetected_playwright/__init__.py
+-rw-r--r--   0        0        0     3580 2024-04-03 03:11:08.167667 browserforge-1.1.2/browserforge/injectors/undetected_playwright/injector.py
+-rw-r--r--   0        0        0     4245 2024-04-03 03:11:08.167667 browserforge-1.1.2/browserforge/injectors/utils.py
+-rw-r--r--   0        0        0        0 2024-04-03 03:11:08.167667 browserforge-1.1.2/browserforge/py.typed
+-rw-r--r--   0        0        0    11558 2024-04-03 03:11:08.159282 browserforge-1.1.2/LICENSE
+-rw-r--r--   0        0        0      882 2024-04-03 03:11:08.169042 browserforge-1.1.2/pyproject.toml
+-rw-r--r--   0        0        0    28273 2024-04-03 03:11:08.160280 browserforge-1.1.2/README.md
+-rw-r--r--   0        0        0    28833 1970-01-01 00:00:00.000000 browserforge-1.1.2/PKG-INFO
```

### Comparing `browserforge-1.1.1/browserforge/__main__.py` & `browserforge-1.1.2/browserforge/__main__.py`

 * *Files identical despite different names*

### Comparing `browserforge-1.1.1/browserforge/bayesian_network.py` & `browserforge-1.1.2/browserforge/bayesian_network.py`

 * *Files identical despite different names*

### Comparing `browserforge-1.1.1/browserforge/download.py` & `browserforge-1.1.2/browserforge/download.py`

 * *Files identical despite different names*

### Comparing `browserforge-1.1.1/browserforge/fingerprints/generator.py` & `browserforge-1.1.2/browserforge/fingerprints/generator.py`

 * *Files identical despite different names*

### Comparing `browserforge-1.1.1/browserforge/headers/generator.py` & `browserforge-1.1.2/browserforge/headers/generator.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,22 @@
 from dataclasses import dataclass
 from pathlib import Path
-from typing import Any, Dict, Iterable, List, Literal, Optional, Tuple, TypeAlias, Union
+from typing import Any, Dict, Iterable, List, Literal, Optional, Tuple, Union
 
 import orjson
-
 from browserforge.bayesian_network import BayesianNetwork, get_possible_values
 
 from .utils import get_browser, get_user_agent, pascalize_headers, tuplify
 
+try:
+    from typing import TypeAlias
+except ImportError:
+    from typing_extensions import TypeAlias  # < 3.10
+
+
 """Constants"""
 SUPPORTED_BROWSERS = ('chrome', 'firefox', 'safari', 'edge')
 SUPPORTED_OPERATING_SYSTEMS = ('windows', 'macos', 'linux', 'android', 'ios')
 SUPPORTED_DEVICES = ('desktop', 'mobile')
 SUPPORTED_HTTP_VERSIONS = ('1', '2')
 MISSING_VALUE_DATASET_TOKEN = '*MISSING_VALUE*'
 HTTP1_SEC_FETCH_ATTRIBUTES = {
```

### Comparing `browserforge-1.1.1/browserforge/headers/utils.py` & `browserforge-1.1.2/browserforge/headers/utils.py`

 * *Files identical despite different names*

### Comparing `browserforge-1.1.1/browserforge/injectors/data/utils.js.xz` & `browserforge-1.1.2/browserforge/injectors/data/utils.js.xz`

 * *Files identical despite different names*

### Comparing `browserforge-1.1.1/browserforge/injectors/playwright/injector.py` & `browserforge-1.1.2/browserforge/injectors/playwright/injector.py`

 * *Files identical despite different names*

### Comparing `browserforge-1.1.1/browserforge/injectors/pyppeteer/injector.py` & `browserforge-1.1.2/browserforge/injectors/pyppeteer/injector.py`

 * *Files identical despite different names*

### Comparing `browserforge-1.1.1/browserforge/injectors/undetected_playwright/injector.py` & `browserforge-1.1.2/browserforge/injectors/undetected_playwright/injector.py`

 * *Files identical despite different names*

### Comparing `browserforge-1.1.1/browserforge/injectors/utils.py` & `browserforge-1.1.2/browserforge/injectors/utils.py`

 * *Files identical despite different names*

### Comparing `browserforge-1.1.1/LICENSE` & `browserforge-1.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `browserforge-1.1.1/pyproject.toml` & `browserforge-1.1.2/pyproject.toml`

 * *Files 27% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "browserforge"
-version = "1.1.1"
+version = "1.1.2"
 description = "Intelligent browser header & fingerprint generator"
 authors = ["daijro <daijro.dev@gmail.com>"]
 license = "Apache-2.0"
 readme = "README.md"
 repository = "https://github.com/daijro/browserforge"
 keywords = [
     "client",
@@ -30,7 +30,8 @@
 [tool.poetry.dependencies]
 python = "^3.8"
 click = "*"
 rich = "*"
 aiofiles = "*"
 httpx = "*"
 orjson = "*"
+typing_extensions = {version = "*", python = "<3.10"}
```

### Comparing `browserforge-1.1.1/README.md` & `browserforge-1.1.2/README.md`

 * *Files identical despite different names*

### Comparing `browserforge-1.1.1/PKG-INFO` & `browserforge-1.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: browserforge
-Version: 1.1.1
+Version: 1.1.2
 Summary: Intelligent browser header & fingerprint generator
 Home-page: https://github.com/daijro/browserforge
 License: Apache-2.0
 Keywords: client,headers,fingerprint,generator,browser,http,scraping,requests,playwright
 Author: daijro
 Author-email: daijro.dev@gmail.com
 Requires-Python: >=3.8,<4.0
@@ -19,14 +19,15 @@
 Classifier: Topic :: Internet :: WWW/HTTP :: Browsers
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Dist: aiofiles
 Requires-Dist: click
 Requires-Dist: httpx
 Requires-Dist: orjson
 Requires-Dist: rich
+Requires-Dist: typing_extensions ; python_version < "3.10"
 Project-URL: Repository, https://github.com/daijro/browserforge
 Description-Content-Type: text/markdown
 
 <h1 align="center">
     BrowserForge
 </h1>
```

#### html2text {}

```diff
@@ -1,22 +1,23 @@
-Metadata-Version: 2.1 Name: browserforge Version: 1.1.1 Summary: Intelligent
+Metadata-Version: 2.1 Name: browserforge Version: 1.1.2 Summary: Intelligent
 browser header & fingerprint generator Home-page: https://github.com/daijro/
 browserforge License: Apache-2.0 Keywords:
 client,headers,fingerprint,generator,browser,http,scraping,requests,playwright
 Author: daijro Author-email: daijro.dev@gmail.com Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: Apache Software License Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
 Programming Language :: Python :: 3.10 Classifier: Programming Language ::
 Python :: 3.11 Classifier: Programming Language :: Python :: 3.12 Classifier:
 Topic :: Internet :: WWW/HTTP Classifier: Topic :: Internet :: WWW/HTTP ::
 Browsers Classifier: Topic :: Software Development :: Libraries :: Python
 Modules Requires-Dist: aiofiles Requires-Dist: click Requires-Dist: httpx
-Requires-Dist: orjson Requires-Dist: rich Project-URL: Repository, https://
-github.com/daijro/browserforge Description-Content-Type: text/markdown
+Requires-Dist: orjson Requires-Dist: rich Requires-Dist: typing_extensions ;
+python_version < "3.10" Project-URL: Repository, https://github.com/daijro/
+browserforge Description-Content-Type: text/markdown
                           ************ BBrroowwsseerrFFoorrggee ************
  _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_g_i_t_h_u_b_/_l_i_c_e_n_s_e_/_d_a_i_j_r_o_/_b_r_o_w_s_e_r_f_o_r_g_e_._s_v_g_?_c_o_l_o_r_=_y_e_l_l_o_w_]
 _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_p_y_t_h_o_n_-_3_._8_&_#_8_2_0_8_;_3_._1_2_-_b_l_u_e_]_[_P_y_P_I_]_[_P_y_P_I_]_[_h_t_t_p_s_:_/_/
   _i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_c_o_d_e_%_2_0_s_t_y_l_e_-_b_l_a_c_k_-_b_l_a_c_k_._s_v_g_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/
 _b_a_d_g_e_/_i_m_p_o_r_t_s_-_i_s_o_r_t_-_y_e_l_l_o_w_._s_v_g_]_[_h_t_t_p_:_/_/_w_w_w_._m_y_p_y_-_l_a_n_g_._o_r_g_/_s_t_a_t_i_c_/_m_y_p_y___b_a_d_g_e_._s_v_g_]
         ****** ?ð???­ IInntteelllliiggeenntt bbrroowwsseerr hheeaaddeerr && ffiinnggeerrpprriinntt ggeenneerraattoorr ******
 --- ## What is it? BrowserForge is a browser header and fingerprint generator
```

