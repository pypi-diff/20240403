# Comparing `tmp/mov-cli-films-1.3.2.tar.gz` & `tmp/mov-cli-films-1.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mov-cli-films-1.3.2.tar", last modified: Wed Mar 27 22:34:04 2024, max compression
+gzip compressed data, was "mov-cli-films-1.3.3.tar", last modified: Wed Apr  3 18:26:32 2024, max compression
```

## Comparing `mov-cli-films-1.3.2.tar` & `mov-cli-films-1.3.3.tar`

### file list

```diff
@@ -1,26 +1,23 @@
-drwxr-xr-x   0 goldy     (1000) goldy     (1000)        0 2024-03-27 22:34:04.323585 mov-cli-films-1.3.2/
--rw-r--r--   0 goldy     (1000) goldy     (1000)     1064 2024-03-04 22:34:31.000000 mov-cli-films-1.3.2/LICENSE
--rw-r--r--   0 goldy     (1000) goldy     (1000)     2923 2024-03-27 22:34:04.323585 mov-cli-films-1.3.2/PKG-INFO
--rw-r--r--   0 goldy     (1000) goldy     (1000)      575 2024-03-09 16:43:29.000000 mov-cli-films-1.3.2/README.md
-drwxr-xr-x   0 goldy     (1000) goldy     (1000)        0 2024-03-27 22:34:04.320252 mov-cli-films-1.3.2/mov_cli_films/
--rw-r--r--   0 goldy     (1000) goldy     (1000)      446 2024-03-27 22:30:56.000000 mov-cli-films-1.3.2/mov_cli_films/__init__.py
-drwxr-xr-x   0 goldy     (1000) goldy     (1000)        0 2024-03-27 22:34:04.320252 mov-cli-films-1.3.2/mov_cli_films/vadapav/
--rw-r--r--   0 goldy     (1000) goldy     (1000)       23 2024-03-09 16:43:29.000000 mov-cli-films-1.3.2/mov_cli_films/vadapav/__init__.py
--rw-r--r--   0 goldy     (1000) goldy     (1000)     3913 2024-03-27 22:14:25.000000 mov-cli-films-1.3.2/mov_cli_films/vadapav/scraper.py
-drwxr-xr-x   0 goldy     (1000) goldy     (1000)        0 2024-03-27 22:34:04.320252 mov-cli-films-1.3.2/mov_cli_films/vidsrcme/
--rw-r--r--   0 goldy     (1000) goldy     (1000)       22 2024-03-14 20:16:52.000000 mov-cli-films-1.3.2/mov_cli_films/vidsrcme/__init__.py
--rw-r--r--   0 goldy     (1000) goldy     (1000)     3207 2024-03-27 22:13:56.000000 mov-cli-films-1.3.2/mov_cli_films/vidsrcme/scraper.py
-drwxr-xr-x   0 goldy     (1000) goldy     (1000)        0 2024-03-27 22:34:04.323585 mov-cli-films-1.3.2/mov_cli_films/vidsrcto/
--rw-r--r--   0 goldy     (1000) goldy     (1000)       22 2024-03-09 16:43:29.000000 mov-cli-films-1.3.2/mov_cli_films/vidsrcto/__init__.py
-drwxr-xr-x   0 goldy     (1000) goldy     (1000)        0 2024-03-27 22:34:04.323585 mov-cli-films-1.3.2/mov_cli_films/vidsrcto/ext/
--rw-r--r--   0 goldy     (1000) goldy     (1000)       22 2024-03-27 21:59:37.000000 mov-cli-films-1.3.2/mov_cli_films/vidsrcto/ext/__init__.py
--rw-r--r--   0 goldy     (1000) goldy     (1000)     4019 2024-03-27 21:59:49.000000 mov-cli-films-1.3.2/mov_cli_films/vidsrcto/ext/vidplay.py
--rw-r--r--   0 goldy     (1000) goldy     (1000)     4261 2024-03-27 22:31:01.000000 mov-cli-films-1.3.2/mov_cli_films/vidsrcto/scraper.py
-drwxr-xr-x   0 goldy     (1000) goldy     (1000)        0 2024-03-27 22:34:04.323585 mov-cli-films-1.3.2/mov_cli_films.egg-info/
--rw-r--r--   0 goldy     (1000) goldy     (1000)     2923 2024-03-27 22:34:04.000000 mov-cli-films-1.3.2/mov_cli_films.egg-info/PKG-INFO
--rw-r--r--   0 goldy     (1000) goldy     (1000)      524 2024-03-27 22:34:04.000000 mov-cli-films-1.3.2/mov_cli_films.egg-info/SOURCES.txt
--rw-r--r--   0 goldy     (1000) goldy     (1000)        1 2024-03-27 22:34:04.000000 mov-cli-films-1.3.2/mov_cli_films.egg-info/dependency_links.txt
--rw-r--r--   0 goldy     (1000) goldy     (1000)       88 2024-03-27 22:34:04.000000 mov-cli-films-1.3.2/mov_cli_films.egg-info/requires.txt
--rw-r--r--   0 goldy     (1000) goldy     (1000)       14 2024-03-27 22:34:04.000000 mov-cli-films-1.3.2/mov_cli_films.egg-info/top_level.txt
--rw-r--r--   0 goldy     (1000) goldy     (1000)     1328 2024-03-14 20:30:31.000000 mov-cli-films-1.3.2/pyproject.toml
--rw-r--r--   0 goldy     (1000) goldy     (1000)       38 2024-03-27 22:34:04.323585 mov-cli-films-1.3.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-03 18:26:32.271755 mov-cli-films-1.3.3/
+-rw-rw-rw-   0        0        0     1085 2024-04-03 14:45:08.000000 mov-cli-films-1.3.3/LICENSE
+-rw-rw-rw-   0        0        0     3004 2024-04-03 18:26:32.269758 mov-cli-films-1.3.3/PKG-INFO
+-rw-rw-rw-   0        0        0      607 2024-04-03 14:45:08.000000 mov-cli-films-1.3.3/README.md
+drwxrwxrwx   0        0        0        0 2024-04-03 18:26:32.226746 mov-cli-films-1.3.3/mov_cli_films/
+-rw-rw-rw-   0        0        0      406 2024-04-03 17:37:24.000000 mov-cli-films-1.3.3/mov_cli_films/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-03 18:26:32.249749 mov-cli-films-1.3.3/mov_cli_films/vidsrcme/
+-rw-rw-rw-   0        0        0       22 2024-04-03 14:45:08.000000 mov-cli-films-1.3.3/mov_cli_films/vidsrcme/__init__.py
+-rw-rw-rw-   0        0        0     3307 2024-04-03 14:45:08.000000 mov-cli-films-1.3.3/mov_cli_films/vidsrcme/scraper.py
+drwxrwxrwx   0        0        0        0 2024-04-03 18:26:32.263752 mov-cli-films-1.3.3/mov_cli_films/vidsrcto/
+-rw-rw-rw-   0        0        0       22 2024-04-03 14:45:08.000000 mov-cli-films-1.3.3/mov_cli_films/vidsrcto/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-03 18:26:32.266754 mov-cli-films-1.3.3/mov_cli_films/vidsrcto/ext/
+-rw-rw-rw-   0        0        0       22 2024-04-03 14:45:08.000000 mov-cli-films-1.3.3/mov_cli_films/vidsrcto/ext/__init__.py
+-rw-rw-rw-   0        0        0     4140 2024-04-03 14:45:08.000000 mov-cli-films-1.3.3/mov_cli_films/vidsrcto/ext/vidplay.py
+-rw-rw-rw-   0        0        0     4531 2024-04-03 18:25:52.000000 mov-cli-films-1.3.3/mov_cli_films/vidsrcto/scraper.py
+drwxrwxrwx   0        0        0        0 2024-04-03 18:26:32.268756 mov-cli-films-1.3.3/mov_cli_films.egg-info/
+-rw-rw-rw-   0        0        0     3004 2024-04-03 18:26:32.000000 mov-cli-films-1.3.3/mov_cli_films.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      457 2024-04-03 18:26:32.000000 mov-cli-films-1.3.3/mov_cli_films.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-03 18:26:32.000000 mov-cli-films-1.3.3/mov_cli_films.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       88 2024-04-03 18:26:32.000000 mov-cli-films-1.3.3/mov_cli_films.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2024-04-03 18:26:32.000000 mov-cli-films-1.3.3/mov_cli_films.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1378 2024-04-03 14:45:08.000000 mov-cli-films-1.3.3/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-03 18:26:32.271755 mov-cli-films-1.3.3/setup.cfg
```

### Comparing `mov-cli-films-1.3.2/PKG-INFO` & `mov-cli-films-1.3.3/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,81 +1,81 @@
-Metadata-Version: 2.1
-Name: mov-cli-films
-Version: 1.3.2
-Summary: A mov-cli v4 plugin for watching Films and Shows.
-Author-email: Ananas <ananas@r3tr0ananas.lol>
-License: MIT License
-        
-        Copyright (c) 2024 mov-cli
-        
-        Permission is hereby granted, free of charge, to any person obtaining a copy
-        of this software and associated documentation files (the "Software"), to deal
-        in the Software without restriction, including without limitation the rights
-        to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-        copies of the Software, and to permit persons to whom the Software is
-        furnished to do so, subject to the following conditions:
-        
-        The above copyright notice and this permission notice shall be included in all
-        copies or substantial portions of the Software.
-        
-        THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-        IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-        FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-        AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-        LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-        OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-        SOFTWARE.
-        
-Project-URL: GitHub, https://github.com/mov-cli/mov-cli-films
-Project-URL: BugTracker, https://github.com/mov-cli/mov-cli-films/issues
-Keywords: amazing mov-cli plugin
-Classifier: Operating System :: Microsoft :: Windows :: Windows 11
-Classifier: Operating System :: Microsoft :: Windows :: Windows 10
-Classifier: Operating System :: POSIX :: Linux
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: requests
-Requires-Dist: importlib-metadata; python_version < "3.8"
-Requires-Dist: mov-cli>=4.0.3
-Provides-Extra: dev
-Requires-Dist: ruff; extra == "dev"
-Requires-Dist: build; extra == "dev"
-
-<div align="center">
-
-  # mov-cli-films 
-  <sub>A mov-cli v4 plugin for watching Films and Shows.</sub>
-
-  <img src="https://github.com/mov-cli/mov-cli-vadapav/assets/132799819/6406133d-f840-424b-a1c9-04599fadb0a7">
-
-</div>
-
-> [!Warning]
-> WIP and written at 3 am 💀
-
-## Installation
-Here's how to install and add the plugin to mov-cli.
-
-1. Install the pip package.
-```sh
-pip install mov-cli-films 
-```
-2. Then add the plugin to your mov-cli config.
-```sh
-mov-cli -e
-```
-```toml
-[mov-cli.plugins]
-films = "mov-cli-films"
-```
-
-## Usage
-```sh
-mov-cli -s films the rookie
-```
+Metadata-Version: 2.1
+Name: mov-cli-films
+Version: 1.3.3
+Summary: A mov-cli v4 plugin for watching Films and Shows.
+Author-email: Ananas <ananas@r3tr0ananas.lol>
+License: MIT License
+        
+        Copyright (c) 2024 mov-cli
+        
+        Permission is hereby granted, free of charge, to any person obtaining a copy
+        of this software and associated documentation files (the "Software"), to deal
+        in the Software without restriction, including without limitation the rights
+        to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+        copies of the Software, and to permit persons to whom the Software is
+        furnished to do so, subject to the following conditions:
+        
+        The above copyright notice and this permission notice shall be included in all
+        copies or substantial portions of the Software.
+        
+        THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+        IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+        FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+        AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+        LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+        OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+        SOFTWARE.
+        
+Project-URL: GitHub, https://github.com/mov-cli/mov-cli-films
+Project-URL: BugTracker, https://github.com/mov-cli/mov-cli-films/issues
+Keywords: amazing mov-cli plugin
+Classifier: Operating System :: Microsoft :: Windows :: Windows 11
+Classifier: Operating System :: Microsoft :: Windows :: Windows 10
+Classifier: Operating System :: POSIX :: Linux
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: requests
+Requires-Dist: importlib-metadata; python_version < "3.8"
+Requires-Dist: mov-cli>=4.0.3
+Provides-Extra: dev
+Requires-Dist: ruff; extra == "dev"
+Requires-Dist: build; extra == "dev"
+
+<div align="center">
+
+  # mov-cli-films 
+  <sub>A mov-cli v4 plugin for watching Films and Shows.</sub>
+
+  <img src="https://github.com/mov-cli/mov-cli-vadapav/assets/132799819/6406133d-f840-424b-a1c9-04599fadb0a7">
+
+</div>
+
+> [!Warning]
+> WIP and written at 3 am 💀
+
+## Installation
+Here's how to install and add the plugin to mov-cli.
+
+1. Install the pip package.
+```sh
+pip install mov-cli-films 
+```
+2. Then add the plugin to your mov-cli config.
+```sh
+mov-cli -e
+```
+```toml
+[mov-cli.plugins]
+films = "mov-cli-films"
+```
+
+## Usage
+```sh
+mov-cli -s films the rookie
+```
```

### Comparing `mov-cli-films-1.3.2/mov_cli_films/vidsrcme/scraper.py` & `mov-cli-films-1.3.3/mov_cli_films/vidsrcme/scraper.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,101 +1,101 @@
-from __future__ import annotations
-from typing import TYPE_CHECKING, Dict, Iterable
-
-if TYPE_CHECKING:
-    from typing import Dict, Literal, Optional
-
-    from mov_cli import Config
-    from mov_cli.http_client import HTTPClient
-
-import re
-
-from mov_cli import utils
-from mov_cli.scraper import Scraper
-from mov_cli import Series, Movie, Metadata, MetadataType
-from mov_cli.utils.scraper import TheMovieDB
-import base64
-
-
-__all__ = ("VidSrcMeScraper",)
-
-class VidSrcMeScraper(Scraper):
-    def __init__(self, config: Config, http_client: HTTPClient) -> None:
-        self.base_url = "https://vidsrc.net"
-        self.tmdb = TheMovieDB(http_client)
-        super().__init__(config, http_client)
-
-    def search(self, query: str, limit: int = 10) -> Iterable[Metadata]:
-        return self.tmdb.search(query, limit)
-
-    def scrape_episodes(self, metadata: Metadata) -> Dict[int, int] | Dict[None, Literal[1]]:
-        return self.tmdb.scrape_episodes(metadata)
-
-    def __deobfstr(self, hash, index):
-        result = ""
-        for i in range(0, len(hash), 2):
-            j = hash[i:i+2]
-            result += chr(int(j, 16) ^ ord(index[i // 2 % len(index)]))
-        return result
-
-    def __extraction(self, script):
-        file_section = re.findall(r"file:\"#9(.*?)\"", script)[0]
-
-        based64 = re.sub('/@#@\\S+?=?=', '', file_section)
-
-        decoded_video = base64.b64decode(based64)
-
-        return decoded_video.decode()
-
-    def scrape(self, metadata: Metadata, episode: Optional[utils.EpisodeSelector] | None = None) -> Series | Movie:
-        if episode is None:
-            episode = utils.EpisodeSelector()
-
-        type = "movie" if metadata.type == MetadataType.MOVIE else "tv"
-
-        url_const = f"{self.base_url}/embed/{type}/{metadata.id}"
-
-        if metadata.type == MetadataType.SERIES:
-            url_const += f"/{episode.season}-{episode.episode}" 
-
-        vidsrc = self.http_client.get(url_const)
-
-        iframeurl = "https:" + self.soup(vidsrc).select("iframe#player_iframe")[0]["src"]
-
-        doc = self.http_client.get(iframeurl, headers={"Referer": vidsrc})
-
-        doc = self.soup(doc)
-
-        index = doc.select("body")[0]["data-i"]
-        hash = doc.select("div#hidden")[0]["data-h"]
-
-        srcrcp = "https:" + self.__deobfstr(hash, index).replace("vidsrc.stream", "vidsrc.net")
-
-        prourl = self.http_client.get(srcrcp, headers={"Referer": "https://vidsrc.stream/"}).headers["Location"]
-
-        prorcp = self.http_client.get(prourl, headers={"Referer": "https://vidsrc.stream/"})
-
-        prorcp = self.soup(prorcp)
-
-        scripts = prorcp.findAll("script")
-
-        for script in scripts:
-            if "Playerjs" in script.text:
-                player = script.text
-                break
-
-        url = self.__extraction(player)
-
-        if metadata.type == MetadataType.MOVIE:
-            return Movie(
-                url = url,
-                title = metadata.title,
-                referrer = "https://vidsrc.stream/",
-                year = metadata.year
-            )
-
-        return Series(
-            url = url,
-            title = metadata.title,
-            referrer = "https://vidsrc.stream/",
-            episode = episode
+from __future__ import annotations
+from typing import TYPE_CHECKING, Dict, Iterable
+
+if TYPE_CHECKING:
+    from typing import Dict, Literal, Optional
+
+    from mov_cli import Config
+    from mov_cli.http_client import HTTPClient
+
+import re
+
+from mov_cli import utils
+from mov_cli.scraper import Scraper
+from mov_cli import Series, Movie, Metadata, MetadataType
+from mov_cli.utils.scraper import TheMovieDB
+import base64
+
+
+__all__ = ("VidSrcMeScraper",)
+
+class VidSrcMeScraper(Scraper):
+    def __init__(self, config: Config, http_client: HTTPClient) -> None:
+        self.base_url = "https://vidsrc.net"
+        self.tmdb = TheMovieDB(http_client)
+        super().__init__(config, http_client)
+
+    def search(self, query: str, limit: int = 10) -> Iterable[Metadata]:
+        return self.tmdb.search(query, limit)
+
+    def scrape_episodes(self, metadata: Metadata) -> Dict[int, int] | Dict[None, Literal[1]]:
+        return self.tmdb.scrape_episodes(metadata)
+
+    def __deobfstr(self, hash, index):
+        result = ""
+        for i in range(0, len(hash), 2):
+            j = hash[i:i+2]
+            result += chr(int(j, 16) ^ ord(index[i // 2 % len(index)]))
+        return result
+
+    def __extraction(self, script):
+        file_section = re.findall(r"file:\"#9(.*?)\"", script)[0]
+
+        based64 = re.sub('/@#@\\S+?=?=', '', file_section)
+
+        decoded_video = base64.b64decode(based64)
+
+        return decoded_video.decode()
+
+    def scrape(self, metadata: Metadata, episode: Optional[utils.EpisodeSelector] | None = None) -> Series | Movie:
+        if episode is None:
+            episode = utils.EpisodeSelector()
+
+        type = "movie" if metadata.type == MetadataType.MOVIE else "tv"
+
+        url_const = f"{self.base_url}/embed/{type}/{metadata.id}"
+
+        if metadata.type == MetadataType.SERIES:
+            url_const += f"/{episode.season}-{episode.episode}" 
+
+        vidsrc = self.http_client.get(url_const)
+
+        iframeurl = "https:" + self.soup(vidsrc).select("iframe#player_iframe")[0]["src"]
+
+        doc = self.http_client.get(iframeurl, headers={"Referer": vidsrc})
+
+        doc = self.soup(doc)
+
+        index = doc.select("body")[0]["data-i"]
+        hash = doc.select("div#hidden")[0]["data-h"]
+
+        srcrcp = "https:" + self.__deobfstr(hash, index).replace("vidsrc.stream", "vidsrc.net")
+
+        prourl = self.http_client.get(srcrcp, headers={"Referer": "https://vidsrc.stream/"}).headers["Location"]
+
+        prorcp = self.http_client.get(prourl, headers={"Referer": "https://vidsrc.stream/"})
+
+        prorcp = self.soup(prorcp)
+
+        scripts = prorcp.findAll("script")
+
+        for script in scripts:
+            if "Playerjs" in script.text:
+                player = script.text
+                break
+
+        url = self.__extraction(player)
+
+        if metadata.type == MetadataType.MOVIE:
+            return Movie(
+                url = url,
+                title = metadata.title,
+                referrer = "https://vidsrc.stream/",
+                year = metadata.year
+            )
+
+        return Series(
+            url = url,
+            title = metadata.title,
+            referrer = "https://vidsrc.stream/",
+            episode = episode
         )
```

### Comparing `mov-cli-films-1.3.2/mov_cli_films/vidsrcto/ext/vidplay.py` & `mov-cli-films-1.3.3/mov_cli_films/vidsrcto/ext/vidplay.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,122 +1,122 @@
-"""Code from: https://github.com/Ciarands/vidsrc-to-resolver"""
-from __future__ import annotations
-from typing import TYPE_CHECKING, Dict
-
-if TYPE_CHECKING:
-    from typing import Dict, Optional, Union, Tuple, List
-
-    from mov_cli.http_client import HTTPClient
-
-import re
-import base64
-import json
-from mov_cli.errors import MovCliException
-
-__all__ = (
-    "VidPlay",
-)
-
-class VidPlay():
-    def __init__(self, http_client: HTTPClient) -> None:
-        self.KEY_URL : str = "https://github.com/Ciarands/vidsrc-keys/blob/main/keys.json"
-        self.http_client = http_client
-    
-    def decode_data(self, key: str, data: Union[bytearray, str]) -> bytearray:
-        key_bytes = bytes(key, 'utf-8')
-        s = bytearray(range(256))
-        j = 0
-
-        for i in range(256):
-            j = (j + s[i] + key_bytes[i % len(key_bytes)]) & 0xff
-            s[i], s[j] = s[j], s[i]
-
-        decoded = bytearray(len(data))
-        i = 0
-        k = 0
-
-        for index in range(len(data)):
-            i = (i + 1) & 0xff
-            k = (k + s[i]) & 0xff
-            s[i], s[k] = s[k], s[i]
-            t = (s[i] + s[k]) & 0xff
-
-            if isinstance(data[index], str):
-                decoded[index] = ord(data[index]) ^ s[t]
-            elif isinstance(data[index], int):
-                decoded[index] = data[index] ^ s[t]
-            else:
-                raise RC4DecodeFailure("Unsupported data type in the input")
-
-        return decoded
-    
-    def int_2_base(self, x: int, base: int) -> str:
-        charset = "0123456789abcdefghijklmnopqrstuvwxyzABCDEFGHIJKLMNOPQRSTUVWXYZ+/"
-
-        if x < 0:
-            sign = -1
-        elif x == 0:
-            return 0
-        else:
-            sign = 1
-
-        x *= sign
-        digits = []
-
-        while x:
-            digits.append(charset[int(x % base)])
-            x = int(x / base)
-        
-        if sign < 0:
-            digits.append('-')
-        digits.reverse()
-
-        return ''.join(digits)
-    
-    def decode_base64_url_safe(s: str) -> bytearray:
-        standardized_input = s.replace('_', '/').replace('-', '+')
-        binary_data = base64.b64decode(standardized_input)
-        return bytearray(binary_data)
-
-    def get_futoken(self, key: str, url: str, provider_url: str) -> str:
-        req = self.http_client.get(f"{provider_url}/futoken", {"Referer": url})
-        fu_key = re.search(r"var\s+k\s*=\s*'([^']+)'", req.text).group(1)
-        
-        return f"{fu_key},{','.join([str(ord(fu_key[i % len(fu_key)]) + ord(key[i])) for i in range(len(key))])}"
-
-    def encode_id(self, v_id: str) -> str:
-        req = self.http_client.get(self.KEY_URL)
-        
-        matches = re.search(r"\"rawLines\":\s*\[\"(.+)\"\]", req.text)
-
-        key1, key2 = json.loads(matches.group(1).replace("\\", ""))
-        decoded_id = self.decode_data(key1, v_id)
-        encoded_result = self.decode_data(key2, decoded_id)
-        
-        encoded_base64 = base64.b64encode(encoded_result)
-        decoded_result = encoded_base64.decode("utf-8")
-
-        return decoded_result.replace("/", "_")
-    
-    def resolve_source(self, url: str, provider_url: str = "https://vidplay.online") -> Tuple[Optional[List], Optional[Dict]]:
-        url_data = url.split("?")
-
-        key = self.encode_id(url_data[0].split("/e/")[-1])
-        futoken = self.get_futoken(key, url, provider_url)
-        
-        req = self.http_client.get(f"{provider_url}/mediainfo/{futoken}?{url_data[1]}&autostart=true", headers={"Referer": url})
-        if req.status_code != 200:
-            return None, None
-
-        req_data = req.json()
-        if (req_data.get("result")) and isinstance(req_data.get("result"), dict):
-            sources = req_data.get("result").get("sources")
-            return [value.get("file") for value in sources]
-        
-        return None, None
-
-class RC4DecodeFailure(MovCliException):
-    """Raised when failure on decoding RC4 data."""
-    def __init__(self) -> None:
-        super().__init__(
-            "Failed to decode RC4 Data."
+"""Code from: https://github.com/Ciarands/vidsrc-to-resolver"""
+from __future__ import annotations
+from typing import TYPE_CHECKING, Dict
+
+if TYPE_CHECKING:
+    from typing import Dict, Optional, Union, Tuple, List
+
+    from mov_cli.http_client import HTTPClient
+
+import re
+import base64
+import json
+from mov_cli.errors import MovCliException
+
+__all__ = (
+    "VidPlay",
+)
+
+class VidPlay():
+    def __init__(self, http_client: HTTPClient) -> None:
+        self.KEY_URL : str = "https://github.com/Ciarands/vidsrc-keys/blob/main/keys.json"
+        self.http_client = http_client
+    
+    def decode_data(self, key: str, data: Union[bytearray, str]) -> bytearray:
+        key_bytes = bytes(key, 'utf-8')
+        s = bytearray(range(256))
+        j = 0
+
+        for i in range(256):
+            j = (j + s[i] + key_bytes[i % len(key_bytes)]) & 0xff
+            s[i], s[j] = s[j], s[i]
+
+        decoded = bytearray(len(data))
+        i = 0
+        k = 0
+
+        for index in range(len(data)):
+            i = (i + 1) & 0xff
+            k = (k + s[i]) & 0xff
+            s[i], s[k] = s[k], s[i]
+            t = (s[i] + s[k]) & 0xff
+
+            if isinstance(data[index], str):
+                decoded[index] = ord(data[index]) ^ s[t]
+            elif isinstance(data[index], int):
+                decoded[index] = data[index] ^ s[t]
+            else:
+                raise RC4DecodeFailure("Unsupported data type in the input")
+
+        return decoded
+    
+    def int_2_base(self, x: int, base: int) -> str:
+        charset = "0123456789abcdefghijklmnopqrstuvwxyzABCDEFGHIJKLMNOPQRSTUVWXYZ+/"
+
+        if x < 0:
+            sign = -1
+        elif x == 0:
+            return 0
+        else:
+            sign = 1
+
+        x *= sign
+        digits = []
+
+        while x:
+            digits.append(charset[int(x % base)])
+            x = int(x / base)
+        
+        if sign < 0:
+            digits.append('-')
+        digits.reverse()
+
+        return ''.join(digits)
+    
+    def decode_base64_url_safe(s: str) -> bytearray:
+        standardized_input = s.replace('_', '/').replace('-', '+')
+        binary_data = base64.b64decode(standardized_input)
+        return bytearray(binary_data)
+
+    def get_futoken(self, key: str, url: str, provider_url: str) -> str:
+        req = self.http_client.get(f"{provider_url}/futoken", {"Referer": url})
+        fu_key = re.search(r"var\s+k\s*=\s*'([^']+)'", req.text).group(1)
+        
+        return f"{fu_key},{','.join([str(ord(fu_key[i % len(fu_key)]) + ord(key[i])) for i in range(len(key))])}"
+
+    def encode_id(self, v_id: str) -> str:
+        req = self.http_client.get(self.KEY_URL)
+        
+        matches = re.search(r"\"rawLines\":\s*\[\"(.+)\"\]", req.text)
+
+        key1, key2 = json.loads(matches.group(1).replace("\\", ""))
+        decoded_id = self.decode_data(key1, v_id)
+        encoded_result = self.decode_data(key2, decoded_id)
+        
+        encoded_base64 = base64.b64encode(encoded_result)
+        decoded_result = encoded_base64.decode("utf-8")
+
+        return decoded_result.replace("/", "_")
+    
+    def resolve_source(self, url: str, provider_url: str = "https://vidplay.online") -> Tuple[Optional[List], Optional[Dict]]:
+        url_data = url.split("?")
+
+        key = self.encode_id(url_data[0].split("/e/")[-1])
+        futoken = self.get_futoken(key, url, provider_url)
+        
+        req = self.http_client.get(f"{provider_url}/mediainfo/{futoken}?{url_data[1]}&autostart=true", headers={"Referer": url})
+        if req.status_code != 200:
+            return None, None
+
+        req_data = req.json()
+        if (req_data.get("result")) and isinstance(req_data.get("result"), dict):
+            sources = req_data.get("result").get("sources")
+            return [value.get("file") for value in sources]
+        
+        return None, None
+
+class RC4DecodeFailure(MovCliException):
+    """Raised when failure on decoding RC4 data."""
+    def __init__(self) -> None:
+        super().__init__(
+            "Failed to decode RC4 Data."
         )
```

### Comparing `mov-cli-films-1.3.2/mov_cli_films.egg-info/PKG-INFO` & `mov-cli-films-1.3.3/mov_cli_films.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,81 +1,81 @@
-Metadata-Version: 2.1
-Name: mov-cli-films
-Version: 1.3.2
-Summary: A mov-cli v4 plugin for watching Films and Shows.
-Author-email: Ananas <ananas@r3tr0ananas.lol>
-License: MIT License
-        
-        Copyright (c) 2024 mov-cli
-        
-        Permission is hereby granted, free of charge, to any person obtaining a copy
-        of this software and associated documentation files (the "Software"), to deal
-        in the Software without restriction, including without limitation the rights
-        to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-        copies of the Software, and to permit persons to whom the Software is
-        furnished to do so, subject to the following conditions:
-        
-        The above copyright notice and this permission notice shall be included in all
-        copies or substantial portions of the Software.
-        
-        THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-        IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-        FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-        AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-        LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-        OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-        SOFTWARE.
-        
-Project-URL: GitHub, https://github.com/mov-cli/mov-cli-films
-Project-URL: BugTracker, https://github.com/mov-cli/mov-cli-films/issues
-Keywords: amazing mov-cli plugin
-Classifier: Operating System :: Microsoft :: Windows :: Windows 11
-Classifier: Operating System :: Microsoft :: Windows :: Windows 10
-Classifier: Operating System :: POSIX :: Linux
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: requests
-Requires-Dist: importlib-metadata; python_version < "3.8"
-Requires-Dist: mov-cli>=4.0.3
-Provides-Extra: dev
-Requires-Dist: ruff; extra == "dev"
-Requires-Dist: build; extra == "dev"
-
-<div align="center">
-
-  # mov-cli-films 
-  <sub>A mov-cli v4 plugin for watching Films and Shows.</sub>
-
-  <img src="https://github.com/mov-cli/mov-cli-vadapav/assets/132799819/6406133d-f840-424b-a1c9-04599fadb0a7">
-
-</div>
-
-> [!Warning]
-> WIP and written at 3 am 💀
-
-## Installation
-Here's how to install and add the plugin to mov-cli.
-
-1. Install the pip package.
-```sh
-pip install mov-cli-films 
-```
-2. Then add the plugin to your mov-cli config.
-```sh
-mov-cli -e
-```
-```toml
-[mov-cli.plugins]
-films = "mov-cli-films"
-```
-
-## Usage
-```sh
-mov-cli -s films the rookie
-```
+Metadata-Version: 2.1
+Name: mov-cli-films
+Version: 1.3.3
+Summary: A mov-cli v4 plugin for watching Films and Shows.
+Author-email: Ananas <ananas@r3tr0ananas.lol>
+License: MIT License
+        
+        Copyright (c) 2024 mov-cli
+        
+        Permission is hereby granted, free of charge, to any person obtaining a copy
+        of this software and associated documentation files (the "Software"), to deal
+        in the Software without restriction, including without limitation the rights
+        to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+        copies of the Software, and to permit persons to whom the Software is
+        furnished to do so, subject to the following conditions:
+        
+        The above copyright notice and this permission notice shall be included in all
+        copies or substantial portions of the Software.
+        
+        THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+        IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+        FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+        AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+        LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+        OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+        SOFTWARE.
+        
+Project-URL: GitHub, https://github.com/mov-cli/mov-cli-films
+Project-URL: BugTracker, https://github.com/mov-cli/mov-cli-films/issues
+Keywords: amazing mov-cli plugin
+Classifier: Operating System :: Microsoft :: Windows :: Windows 11
+Classifier: Operating System :: Microsoft :: Windows :: Windows 10
+Classifier: Operating System :: POSIX :: Linux
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: requests
+Requires-Dist: importlib-metadata; python_version < "3.8"
+Requires-Dist: mov-cli>=4.0.3
+Provides-Extra: dev
+Requires-Dist: ruff; extra == "dev"
+Requires-Dist: build; extra == "dev"
+
+<div align="center">
+
+  # mov-cli-films 
+  <sub>A mov-cli v4 plugin for watching Films and Shows.</sub>
+
+  <img src="https://github.com/mov-cli/mov-cli-vadapav/assets/132799819/6406133d-f840-424b-a1c9-04599fadb0a7">
+
+</div>
+
+> [!Warning]
+> WIP and written at 3 am 💀
+
+## Installation
+Here's how to install and add the plugin to mov-cli.
+
+1. Install the pip package.
+```sh
+pip install mov-cli-films 
+```
+2. Then add the plugin to your mov-cli config.
+```sh
+mov-cli -e
+```
+```toml
+[mov-cli.plugins]
+films = "mov-cli-films"
+```
+
+## Usage
+```sh
+mov-cli -s films the rookie
+```
```

