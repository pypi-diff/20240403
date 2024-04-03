# Comparing `tmp/nonebot_plugin_ghtiles-0.1.1.tar.gz` & `tmp/nonebot_plugin_ghtiles-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_ghtiles-0.1.1.tar", last modified: Tue Apr  2 00:36:08 2024, max compression
+gzip compressed data, was "nonebot_plugin_ghtiles-0.1.2.tar", last modified: Wed Apr  3 11:09:55 2024, max compression
```

## Comparing `nonebot_plugin_ghtiles-0.1.1.tar` & `nonebot_plugin_ghtiles-0.1.2.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1064 2024-04-02 00:35:53.354958 nonebot_plugin_ghtiles-0.1.1/LICENSE
--rw-r--r--   0        0        0     3002 2024-04-02 00:35:53.354958 nonebot_plugin_ghtiles-0.1.1/README.md
--rw-r--r--   0        0        0     7242 2024-04-02 00:35:53.354958 nonebot_plugin_ghtiles-0.1.1/nonebot_plugin_ghtiles/__init__.py
--rw-r--r--   0        0        0      241 2024-04-02 00:35:53.354958 nonebot_plugin_ghtiles-0.1.1/nonebot_plugin_ghtiles/config.py
--rw-r--r--   0        0        0     1774 2024-04-02 00:35:53.354958 nonebot_plugin_ghtiles-0.1.1/nonebot_plugin_ghtiles/utils.py
--rw-r--r--   0        0        0     1142 2024-04-02 00:36:08.842974 nonebot_plugin_ghtiles-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     3714 1970-01-01 00:00:00.000000 nonebot_plugin_ghtiles-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1064 2024-04-03 11:09:42.331021 nonebot_plugin_ghtiles-0.1.2/LICENSE
+-rw-r--r--   0        0        0     3002 2024-04-03 11:09:42.331021 nonebot_plugin_ghtiles-0.1.2/README.md
+-rw-r--r--   0        0        0     7242 2024-04-03 11:09:42.331021 nonebot_plugin_ghtiles-0.1.2/nonebot_plugin_ghtiles/__init__.py
+-rw-r--r--   0        0        0      241 2024-04-03 11:09:42.331021 nonebot_plugin_ghtiles-0.1.2/nonebot_plugin_ghtiles/config.py
+-rw-r--r--   0        0        0     2211 2024-04-03 11:09:42.331021 nonebot_plugin_ghtiles-0.1.2/nonebot_plugin_ghtiles/utils.py
+-rw-r--r--   0        0        0     1172 2024-04-03 11:09:55.310957 nonebot_plugin_ghtiles-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     3752 1970-01-01 00:00:00.000000 nonebot_plugin_ghtiles-0.1.2/PKG-INFO
```

### Comparing `nonebot_plugin_ghtiles-0.1.1/LICENSE` & `nonebot_plugin_ghtiles-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_ghtiles-0.1.1/README.md` & `nonebot_plugin_ghtiles-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_ghtiles-0.1.1/nonebot_plugin_ghtiles/__init__.py` & `nonebot_plugin_ghtiles-0.1.2/nonebot_plugin_ghtiles/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_ghtiles-0.1.1/nonebot_plugin_ghtiles/utils.py` & `nonebot_plugin_ghtiles-0.1.2/nonebot_plugin_ghtiles/utils.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,46 +1,49 @@
 import json
 import re
 import httpx
 from datetime import datetime
 from pathlib import Path
+from bs4 import BeautifulSoup
 
 
 def get_today() -> str:
     return datetime.now().strftime("%Y-%m-%d")
 
-
+# only contributions html elements
 async def get_homepage_html(gh_name: str, proxy: str = "https://github.com") -> str:
-    url = f"{proxy}/{gh_name}"
+    url = f"{proxy}/{gh_name}?action=show&controller=profiles&tab=contributions&user_id={gh_name}"
+    headers = {
+        "X-Requested-With": "XMLHttpRequest"
+    }
     async with httpx.AsyncClient() as client:
-        response = await client.get(url)
+        response = await client.get(url, headers=headers)
         response.raise_for_status()
         return response.text
 
 
 async def check_contributions(gh_html: str) -> bool:
     return re.compile(r"\'s activity is private\<\/h2\>").search(gh_html) is None
 
 
 async def get_today_contributions(gh_html: str) -> int:
-    match = re.compile(
-        r'data-date="' + get_today() + r".*?(\d+|No) contributions"
-    ).search(gh_html)
-    if match:
-        contributions = match.group(1)
-        if contributions == "No":
-            return 0
-        else:
-            return int(contributions)
-    else:
-        return 0
-
+    soup = BeautifulSoup(gh_html, "html.parser")
+    contributions = 0
+    if soup.tbody is None:
+        return contributions
+    tt = soup.tbody("tool-tip")
+    today_index = next((index for index, td in enumerate(soup.tbody("td", class_="ContributionCalendar-day")) if td.get('data-date') == get_today()), None)
+    if today_index is not None:
+        search = re.search(r'\d+', tt[today_index].text)
+        if search is not None:
+            contributions = int(search.group())
+    return contributions
 
 class AutoSave:
-    def __init__(self, fileProxy: Path, proxy: dict = None, initial_data: dict = None):
+    def __init__(self, fileProxy: Path, proxy: dict = None, initial_data: dict = None): # type: ignore
         self._fileProxy = fileProxy
         if proxy is None:
             if fileProxy.exists():
                 load_by_file = json.loads(fileProxy.read_text())
                 self._proxy = load_by_file if load_by_file else initial_data or {}
             else:
                 self._proxy = initial_data or {}
```

### Comparing `nonebot_plugin_ghtiles-0.1.1/pyproject.toml` & `nonebot_plugin_ghtiles-0.1.2/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 [project]
 name = "nonebot-plugin-ghtiles"
-version = "0.1.1"
+version = "0.1.2"
 description = "A nonebot2 plugin for show GitHub contributions"
 readme = "README.md"
 requires-python = ">=3.9, <4.0"
 dependencies = [
     "nonebot2>=2.2.0",
     "httpx~=0.27",
     "nonebot-plugin-alconna>=0.38.1",
     "nonebot-plugin-apscheduler~=0.4",
     "nonebot-plugin-session~=0.3",
     "nonebot-plugin-localstore~=0.6",
+    "beautifulsoup4>=4.12.3",
 ]
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
```

### Comparing `nonebot_plugin_ghtiles-0.1.1/PKG-INFO` & `nonebot_plugin_ghtiles-0.1.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-ghtiles
-Version: 0.1.1
+Version: 0.1.2
 Summary: A nonebot2 plugin for show GitHub contributions
 Home-page: https://github.com/Lipraty/nonebot-plugin-ghtiles
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Project-URL: Homepage, https://github.com/Lipraty/nonebot-plugin-ghtiles
 Requires-Python: <4.0,>=3.9
 Requires-Dist: nonebot2>=2.2.0
 Requires-Dist: httpx~=0.27
 Requires-Dist: nonebot-plugin-alconna>=0.38.1
 Requires-Dist: nonebot-plugin-apscheduler~=0.4
 Requires-Dist: nonebot-plugin-session~=0.3
 Requires-Dist: nonebot-plugin-localstore~=0.6
+Requires-Dist: beautifulsoup4>=4.12.3
 Description-Content-Type: text/markdown
 
 <div align="center">
   <a href="https://v2.nonebot.dev/store">
     <img src="https://raw.githubusercontent.com/A-kirami/nonebot-plugin-template/resources/nbp_logo.png" width="180" height="180" alt="logo">
   </a>
   <br>
```

#### html2text {}

```diff
@@ -1,17 +1,17 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-ghtiles Version: 0.1.1 Summary: A
+Metadata-Version: 2.1 Name: nonebot-plugin-ghtiles Version: 0.1.2 Summary: A
 nonebot2 plugin for show GitHub contributions Home-page: https://github.com/
 Lipraty/nonebot-plugin-ghtiles Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License Classifier: Operating System
 :: OS Independent Project-URL: Homepage, https://github.com/Lipraty/nonebot-
 plugin-ghtiles Requires-Python: <4.0,>=3.9 Requires-Dist: nonebot2>=2.2.0
 Requires-Dist: httpx~=0.27 Requires-Dist: nonebot-plugin-alconna>=0.38.1
 Requires-Dist: nonebot-plugin-apscheduler~=0.4 Requires-Dist: nonebot-plugin-
-session~=0.3 Requires-Dist: nonebot-plugin-localstore~=0.6 Description-Content-
-Type: text/markdown
+session~=0.3 Requires-Dist: nonebot-plugin-localstore~=0.6 Requires-Dist:
+beautifulsoup4>=4.12.3 Description-Content-Type: text/markdown
                                     _[_l_o_g_o_]
                                     [logo]
   # NoneBot-Plugin-GHTiles _â¨ ççä½ ç GitHub ç·ç  for NoneBot2 â¨_
                              [python]_[_p_d_m_-_m_a_n_a_g_e_d_]
             _[_P_y_d_a_n_t_i_c_ _V_e_r_s_i_o_n_ _1_ _O_r_ _2_]_[_l_i_c_e_n_s_e_]_[_p_y_p_i_]_[_p_y_p_i_ _d_o_w_n_l_o_a_d_]
 ## ð ä»ç» NoneBot2 æä»¶ï¼ç¨äºæ¥çä½ ç GitHub ç·ç  ## ð¿
 å®è£ ä»¥ä¸æå°çæ¹æ³ ä»»é**å¶ä¸** å³å¯ [æ¨è] ä½¿ç¨ nb-cli
```

