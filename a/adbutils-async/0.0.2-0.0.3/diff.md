# Comparing `tmp/adbutils_async-0.0.2.tar.gz` & `tmp/adbutils_async-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adbutils_async-0.0.2.tar", last modified: Tue Apr  2 15:12:56 2024, max compression
+gzip compressed data, was "adbutils_async-0.0.3.tar", last modified: Wed Apr  3 03:18:52 2024, max compression
```

## Comparing `adbutils_async-0.0.2.tar` & `adbutils_async-0.0.3.tar`

### file list

```diff
@@ -1,36 +1,50 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 15:12:56.514719 adbutils_async-0.0.2/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 15:12:56.510719 adbutils_async-0.0.2/.github/
--rw-r--r--   0 runner    (1001) docker     (127)      126 2024-04-02 15:12:51.000000 adbutils_async-0.0.2/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 15:12:56.510719 adbutils_async-0.0.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1306 2024-04-02 15:12:51.000000 adbutils_async-0.0.2/.github/workflows/main.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1471 2024-04-02 15:12:51.000000 adbutils_async-0.0.2/.github/workflows/publish-to-pypi.yml
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-02 15:12:56.000000 adbutils_async-0.0.2/AUTHORS
--rw-r--r--   0 runner    (1001) docker     (127)      242 2024-04-02 15:12:56.000000 adbutils_async-0.0.2/ChangeLog
--rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-04-02 15:12:51.000000 adbutils_async-0.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    17142 2024-04-02 15:12:56.514719 adbutils_async-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    15377 2024-04-02 15:12:51.000000 adbutils_async-0.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 15:12:56.510719 adbutils_async-0.0.2/adbutils_async/
--rw-r--r--   0 runner    (1001) docker     (127)     3000 2024-04-02 15:12:51.000000 adbutils_async-0.0.2/adbutils_async/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11467 2024-04-02 15:12:51.000000 adbutils_async-0.0.2/adbutils_async/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9029 2024-04-02 15:12:51.000000 adbutils_async-0.0.2/adbutils_async/_adb.py
--rw-r--r--   0 runner    (1001) docker     (127)    42361 2024-04-02 15:12:51.000000 adbutils_async-0.0.2/adbutils_async/_device.py
--rw-r--r--   0 runner    (1001) docker     (127)     2054 2024-04-02 15:12:51.000000 adbutils_async-0.0.2/adbutils_async/_proto.py
--rw-r--r--   0 runner    (1001) docker     (127)     7260 2024-04-02 15:12:51.000000 adbutils_async-0.0.2/adbutils_async/_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      280 2024-04-02 15:12:51.000000 adbutils_async-0.0.2/adbutils_async/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 15:12:56.514719 adbutils_async-0.0.2/adbutils_async/binaries/
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-02 15:12:51.000000 adbutils_async-0.0.2/adbutils_async/binaries/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-02 15:12:51.000000 adbutils_async-0.0.2/adbutils_async/binaries/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      936 2024-04-02 15:12:51.000000 adbutils_async-0.0.2/adbutils_async/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)    12653 2024-04-02 15:12:51.000000 adbutils_async-0.0.2/adbutils_async/pidcat.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 15:12:56.514719 adbutils_async-0.0.2/adbutils_async.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    17142 2024-04-02 15:12:56.000000 adbutils_async-0.0.2/adbutils_async.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      711 2024-04-02 15:12:56.000000 adbutils_async-0.0.2/adbutils_async.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-02 15:12:56.000000 adbutils_async-0.0.2/adbutils_async.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-02 15:12:56.000000 adbutils_async-0.0.2/adbutils_async.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-02 15:12:56.000000 adbutils_async-0.0.2/adbutils_async.egg-info/pbr.json
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-02 15:12:56.000000 adbutils_async-0.0.2/adbutils_async.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     6050 2024-04-02 15:12:51.000000 adbutils_async-0.0.2/build_wheel.py
--rw-r--r--   0 runner    (1001) docker     (127)      934 2024-04-02 15:12:51.000000 adbutils_async-0.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-04-02 15:12:51.000000 adbutils_async-0.0.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)      653 2024-04-02 15:12:56.514719 adbutils_async-0.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      419 2024-04-02 15:12:51.000000 adbutils_async-0.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 03:18:52.254029 adbutils_async-0.0.3/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 03:18:52.250029 adbutils_async-0.0.3/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)      126 2024-04-03 03:18:44.000000 adbutils_async-0.0.3/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 03:18:52.250029 adbutils_async-0.0.3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1306 2024-04-03 03:18:44.000000 adbutils_async-0.0.3/.github/workflows/main.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1471 2024-04-03 03:18:44.000000 adbutils_async-0.0.3/.github/workflows/publish-to-pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-03 03:18:52.000000 adbutils_async-0.0.3/AUTHORS
+-rw-r--r--   0 runner    (1001) docker     (127)      216 2024-04-03 03:18:52.000000 adbutils_async-0.0.3/ChangeLog
+-rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-04-03 03:18:44.000000 adbutils_async-0.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    17254 2024-04-03 03:18:52.254029 adbutils_async-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    15377 2024-04-03 03:18:44.000000 adbutils_async-0.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 03:18:52.250029 adbutils_async-0.0.3/adbutils_async/
+-rw-r--r--   0 runner    (1001) docker     (127)     2897 2024-04-03 03:18:44.000000 adbutils_async-0.0.3/adbutils_async/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11467 2024-04-03 03:18:44.000000 adbutils_async-0.0.3/adbutils_async/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9015 2024-04-03 03:18:44.000000 adbutils_async-0.0.3/adbutils_async/_adb.py
+-rw-r--r--   0 runner    (1001) docker     (127)    42508 2024-04-03 03:18:44.000000 adbutils_async-0.0.3/adbutils_async/_device.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2069 2024-04-03 03:18:44.000000 adbutils_async-0.0.3/adbutils_async/_proto.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7657 2024-04-03 03:18:44.000000 adbutils_async-0.0.3/adbutils_async/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      274 2024-04-03 03:18:44.000000 adbutils_async-0.0.3/adbutils_async/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 03:18:52.254029 adbutils_async-0.0.3/adbutils_async/binaries/
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-03 03:18:44.000000 adbutils_async-0.0.3/adbutils_async/binaries/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-03 03:18:44.000000 adbutils_async-0.0.3/adbutils_async/binaries/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1001 2024-04-03 03:18:44.000000 adbutils_async-0.0.3/adbutils_async/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12635 2024-04-03 03:18:44.000000 adbutils_async-0.0.3/adbutils_async/pidcat.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 03:18:52.254029 adbutils_async-0.0.3/adbutils_async.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    17254 2024-04-03 03:18:52.000000 adbutils_async-0.0.3/adbutils_async.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-04-03 03:18:52.000000 adbutils_async-0.0.3/adbutils_async.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 03:18:52.000000 adbutils_async-0.0.3/adbutils_async.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 03:18:52.000000 adbutils_async-0.0.3/adbutils_async.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-03 03:18:52.000000 adbutils_async-0.0.3/adbutils_async.egg-info/pbr.json
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-03 03:18:52.000000 adbutils_async-0.0.3/adbutils_async.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-03 03:18:52.000000 adbutils_async-0.0.3/adbutils_async.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     6050 2024-04-03 03:18:44.000000 adbutils_async-0.0.3/build_wheel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1052 2024-04-03 03:18:44.000000 adbutils_async-0.0.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-04-03 03:18:44.000000 adbutils_async-0.0.3/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      653 2024-04-03 03:18:52.254029 adbutils_async-0.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      380 2024-04-03 03:18:44.000000 adbutils_async-0.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 03:18:52.254029 adbutils_async-0.0.3/test_real_device/
+-rw-r--r--   0 runner    (1001) docker     (127)     1089 2024-04-03 03:18:44.000000 adbutils_async-0.0.3/test_real_device/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      749 2024-04-03 03:18:44.000000 adbutils_async-0.0.3/test_real_device/test_adb.py
+-rw-r--r--   0 runner    (1001) docker     (127)      575 2024-04-03 03:18:44.000000 adbutils_async-0.0.3/test_real_device/test_deprecated.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8362 2024-04-03 03:18:44.000000 adbutils_async-0.0.3/test_real_device/test_device.py
+-rw-r--r--   0 runner    (1001) docker     (127)      952 2024-04-03 03:18:44.000000 adbutils_async-0.0.3/test_real_device/test_forward_reverse.py
+-rw-r--r--   0 runner    (1001) docker     (127)      299 2024-04-03 03:18:44.000000 adbutils_async-0.0.3/test_real_device/test_import.py
+-rw-r--r--   0 runner    (1001) docker     (127)      276 2024-04-03 03:18:44.000000 adbutils_async-0.0.3/test_real_device/test_record.py
+-rw-r--r--   0 runner    (1001) docker     (127)      858 2024-04-03 03:18:44.000000 adbutils_async-0.0.3/test_real_device/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 03:18:52.254029 adbutils_async-0.0.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     3772 2024-04-03 03:18:44.000000 adbutils_async-0.0.3/tests/adb_server.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1204 2024-04-03 03:18:44.000000 adbutils_async-0.0.3/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      291 2024-04-03 03:18:44.000000 adbutils_async-0.0.3/tests/test_adb_server.py
```

### Comparing `adbutils_async-0.0.2/.github/workflows/main.yml` & `adbutils_async-0.0.3/.github/workflows/main.yml`

 * *Files identical despite different names*

### Comparing `adbutils_async-0.0.2/.github/workflows/publish-to-pypi.yml` & `adbutils_async-0.0.3/.github/workflows/publish-to-pypi.yml`

 * *Files identical despite different names*

### Comparing `adbutils_async-0.0.2/LICENSE` & `adbutils_async-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `adbutils_async-0.0.2/PKG-INFO` & `adbutils_async-0.0.3/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: adbutils_async
-Version: 0.0.2
-Summary: A sample Python project
+Version: 0.0.3
+Summary: Python adb async library for adb service.
 Home-page: https://github.com/touxiaoling/adbutils_async
 Author: tomin
 Author-email: tomin <tomin@tomin.com>
 License: MIT License
         
         Copyright (c) 2019 openatx
         
@@ -29,15 +29,19 @@
         
 Project-URL: homepage, https://github.com/touxiaoling/adbutils_async
 Project-URL: repository, https://github.com/touxiaoling/adbutils_async
 Project-URL: documentation, https://github.com/touxiaoling/adbutils_async
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
-License-File: AUTHORS
+Requires-Dist: httpx
+Requires-Dist: Pillow
+Requires-Dist: deprecation
+Requires-Dist: retry
+Requires-Dist: apkutils2
 
 # adbutils_async
 [![PyPI](https://img.shields.io/pypi/v/adbutils_async.svg?color=blue)](https://pypi.org/project/adbutils_async/#history)
 
 Python adb async library for adb service (Only support Python3.10+)
 
 fork from [adbutils](https://github.com/openatx/adbutils)
```

### Comparing `adbutils_async-0.0.2/README.md` & `adbutils_async-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `adbutils_async-0.0.2/adbutils_async/__init__.py` & `adbutils_async-0.0.3/adbutils_async/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -48,57 +48,54 @@
             if info.state != "device":
                 continue
             yield AdbDevice(self, serial=info.serial)
 
     async def device_list(self) -> typing.List[AdbDevice]:
         return list(await self.iter_device())
 
-    async def device(self,
-               serial: str = None,
-               transport_id: int = None) -> AdbDevice:
+    async def device(self, serial: str = None, transport_id: int = None) -> AdbDevice:
         if serial:
             return AdbDevice(self, serial=serial)
-        
+
         if transport_id:
             return AdbDevice(self, transport_id=transport_id)
 
         serial = os.environ.get("ANDROID_SERIAL")
         if not serial:
             ds = await self.device_list()
             if len(ds) == 0:
-                raise RuntimeError("Can't find any android device/emulator")
+                raise AdbError("Can't find any android device/emulator")
             if len(ds) > 1:
-                raise RuntimeError(
-                    "more than one device/emulator, please specify the serial number"
-                )
+                raise AdbError("more than one device/emulator, please specify the serial number")
             return ds[0]
         return AdbDevice(self, serial)
 
 
-
 adb = AdbClient()
 device = adb.device
 
+
 async def _main():
     print("server version:", await adb.server_version())
     print("devices:", await adb.device_list())
     d = (await adb.device_list())[0]
 
     print(d.serial)
     async for f in adb.sync(d.serial).iter_directory("/data/local/tmp"):
         print(f)
 
     finfo = await adb.sync(d.serial).stat("/data/local/tmp")
     print(finfo)
     import io
+
     sync = adb.sync(d.serial)
     filepath = "/data/local/tmp/hi.txt"
-    await sync.push(io.BytesIO(b"hi5a4de5f4qa6we541fq6w1ef5a61f65ew1rf6we"),
-              filepath, 0o644)
+    await sync.push(io.BytesIO(b"hi5a4de5f4qa6we541fq6w1ef5a61f65ew1rf6we"), filepath, 0o644)
 
     print("FileInfo", await sync.stat(filepath))
     async for chunk in sync.iter_content(filepath):
         print(chunk)
     # sync.pull(filepath)
-        
+
+
 if __name__ == "__main__":
-    asyncio.run(_main())
+    asyncio.run(_main())
```

### Comparing `adbutils_async-0.0.2/adbutils_async/__main__.py` & `adbutils_async-0.0.3/adbutils_async/__main__.py`

 * *Files identical despite different names*

### Comparing `adbutils_async-0.0.2/adbutils_async/_adb.py` & `adbutils_async-0.0.3/adbutils_async/_adb.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 import asyncio
 import os
 import typing
 from typing import Union
 import weakref
-import struct
 
 from ._utils import adb_path, async_run
 from ._proto import DeviceEvent, AdbCmd
 from .errors import AdbError, AdbTimeout
 
 
 async def _check_server(host: str, port: int) -> bool:
```

### Comparing `adbutils_async-0.0.2/adbutils_async/_device.py` & `adbutils_async-0.0.3/adbutils_async/_device.py`

 * *Files 0% similar despite different names*

```diff
@@ -683,30 +683,30 @@
     async def keyevent(self, key_code: typing.Union[int, str]) -> str:
         """adb _run input keyevent KEY_CODE"""
         return await self.shell(["input", "keyevent", str(key_code)])
 
     def __is_percent(self, v):
         return isinstance(v, float) and v <= 1.0
 
-    async def click(self, x, y):
+    async def click(self, x, y) -> None:
         """
         simulate android tap
 
         Args:
             x, y: int
         """
         is_percent = self.__is_percent
         if any(map(is_percent, [x, y])):
             w, h = await self.window_size()
             x = int(x * w) if is_percent(x) else x
             y = int(y * h) if is_percent(y) else y
         x, y = map(str, [x, y])
-        return await self.shell(["input", "tap", x, y])
+        await self.shell(["input", "tap", x, y])
 
-    async def swipe(self, sx, sy, ex, ey, duration: float = 1.0):
+    async def swipe(self, sx, sy, ex, ey, duration: float = 1.0) -> None:
         """
         swipe from start point to end point
 
         Args:
             sx, sy: start point(x, y)
             ex, ey: end point(x, y)
         """
@@ -714,15 +714,15 @@
         if any(map(is_percent, [sx, sy, ex, ey])):
             w, h = await self.window_size()
             sx = int(sx * w) if is_percent(sx) else sx
             sy = int(sy * h) if is_percent(sy) else sy
             ex = int(ex * w) if is_percent(ex) else ex
             ey = int(ey * h) if is_percent(ey) else ey
         x1, y1, x2, y2 = map(str, [sx, sy, ex, ey])
-        return await self.shell(["input", "swipe", x1, y1, x2, y2, str(int(duration * 1000))])
+        await self.shell(["input", "swipe", x1, y1, x2, y2, str(int(duration * 1000))])
 
     async def send_keys(self, text: str):
         """
         Type a given text
 
         Args:
             text: text to be type
@@ -1097,22 +1097,25 @@
 
         Returns:
             content of xml
 
         Raises:
             AdbError
         """
-        output = await self.shell("uiautomator dump /data/local/tmp/uidump.xml && echo success")
-        if "Success" not in output:
+        target = '/data/local/tmp/uidump.xml'
+        output = await self.shell(
+            f'rm -f {target}; uiautomator dump {target} && echo success')
+        if 'ERROR' in output or 'success' not in output:
             raise AdbError("uiautomator dump failed", output)
 
-        buf = b""
-        for chunk in self.sync.iter_content("/data/local/tmp/uidump.xml"):
-            buf += chunk
-        return buf.decode("utf-8")
+        buf= await self.sync.read_bytes(target)
+        xml_data = buf.decode("utf-8")
+        if not xml_data.startswith('<?xml'):
+            raise AdbError("dump output is not xml", xml_data)
+        return xml_data
 
     @retry(AdbError, delay=0.5, tries=3, jitter=0.1)
     async def app_current(self) -> RunningAppInfo:
         """
         Returns:
             RunningAppInfo(package, activity, pid?)  pid can be 0
```

### Comparing `adbutils_async-0.0.2/adbutils_async/_proto.py` & `adbutils_async-0.0.3/adbutils_async/_proto.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,14 +11,15 @@
     "ForwardItem",
     "ReverseItem",
     "FileInfo",
     "WindowSize",
     "RunningAppInfo",
     "ShellReturn",
     "AdbDeviceInfo",
+    "AppInfo",
 ]
 
 import enum
 import datetime
 import pathlib
 import typing
 from dataclasses import dataclass
```

### Comparing `adbutils_async-0.0.2/adbutils_async/_utils.py` & `adbutils_async-0.0.3/adbutils_async/_utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import hashlib
+import importlib.resources
 import os
 import random
 import shlex
 import socket
 import subprocess
 import sys
 import tempfile
@@ -10,18 +11,19 @@
 import time
 import typing
 import zipfile
 import pathlib
 import asyncio
 import logging
 
-import whichcraft
+from shutil import which
 from apkutils2.axml.axmlparser import AXML
 from apkutils2.manifest import Manifest
-from pkg_resources import resource_filename
+
+from .errors import AdbError
 
 MB = 1024 * 1024
 _logger = logging.getLogger(__name__)
 
 
 def append_path(base: typing.Union[str, pathlib.Path], addition: str) -> str:
     if isinstance(base, pathlib.Path):
@@ -50,15 +52,15 @@
     except OSError:
         # bind 0 will fail on Manjaro, fallback to random port
         # https://github.com/openatx/adbutils/issues/85
         for _ in range(20):
             port = random.randint(10000, 20000)
             if not is_port_in_use(port):
                 return port
-        raise RuntimeError("No free port found")
+        raise AdbError("No free port found")
 
 
 def list2cmdline(args: typing.Union[list, tuple]):
     """do not use subprocess.list2cmdline, use this instead
 
     Reason:
         subprocess.list2cmdline(['echo', '&']) --> "a &", but what I expect should be "a '&'"
@@ -74,31 +76,43 @@
         return ip
     except OSError:
         return "127.0.0.1"
     finally:
         s.close()
 
 
+def _get_bin_dir():
+    if sys.version_info < (3, 9):
+        context = importlib.resources.path("adbutils.binaries", "__init__.py")
+    else:
+        ref = importlib.resources.files("adbutils.binaries") / "__init__.py"
+        context = importlib.resources.as_file(ref)
+    with context as path:
+        pass
+    # Return the dir. We assume that the data files are on a normal dir on the fs.
+    return str(path.parent)
+
+
 def adb_path():
     # 0. check env: ADBUTILS_ADB_PATH
     if os.getenv("ADBUTILS_ADB_PATH"):
         return os.getenv("ADBUTILS_ADB_PATH")
 
     # 1. find in $PATH
-    exe = whichcraft.which("adb")
+    exe = which("adb")
     if exe and _is_valid_exe(exe):
         return exe
 
     # 2. use buildin adb
-    bin_dir = resource_filename("adbutils", "binaries")
+    bin_dir = _get_bin_dir()
     exe = os.path.join(bin_dir, "adb.exe" if os.name == "nt" else "adb")
     if os.path.isfile(exe) and _is_valid_exe(exe):
         return exe
 
-    raise RuntimeError("No adb exe could be found. Install adb on your system")
+    raise AdbError("No adb exe could be found. Install adb on your system")
 
 
 def _popen_kwargs(prevent_sigint=False):
     startupinfo = None
     preexec_fn = None
     creationflags = 0
     if sys.platform.startswith("win"):
```

### Comparing `adbutils_async-0.0.2/adbutils_async/errors.py` & `adbutils_async-0.0.3/adbutils_async/errors.py`

 * *Files 13% similar despite different names*

```diff
@@ -12,14 +12,18 @@
     """adb error"""
 
 
 class AdbTimeout(AdbError):
     """timeout when communicate to adb-server"""
 
 
+class AdbConnectionError(AdbError):
+    """connection error"""
+
+
 class AdbInstallError(AdbError):
     def __init__(self, output: str):
         """
         Errors examples:
         Failure [INSTALL_FAILED_ALREADY_EXISTS: Attempt to re-install io.appium.android.apis without first uninstalling.]
         Error: Failed to parse APK file: android.content.pm.PackageParser$PackageParserException: Failed to parse /data/local/tmp/tmp-29649242.apk
```

### Comparing `adbutils_async-0.0.2/adbutils_async/pidcat.py` & `adbutils_async-0.0.3/adbutils_async/pidcat.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,14 @@
 # Originally written by Jeff Sharkey, http://jsharkey.org/
 # Piping detection and popen() added by other Android team members
 # Package filtering and output improvements by Jake Wharton, http://jakewharton.com
 
 import argparse
 import sys
 import re
-import subprocess
 from subprocess import PIPE
 
 import adbutils
 
 __version__ = "2.1.0"
 
 # yapf: disable
```

### Comparing `adbutils_async-0.0.2/adbutils_async.egg-info/PKG-INFO` & `adbutils_async-0.0.3/adbutils_async.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: adbutils_async
-Version: 0.0.2
-Summary: A sample Python project
+Version: 0.0.3
+Summary: Python adb async library for adb service.
 Home-page: https://github.com/touxiaoling/adbutils_async
 Author: tomin
 Author-email: tomin <tomin@tomin.com>
 License: MIT License
         
         Copyright (c) 2019 openatx
         
@@ -29,15 +29,19 @@
         
 Project-URL: homepage, https://github.com/touxiaoling/adbutils_async
 Project-URL: repository, https://github.com/touxiaoling/adbutils_async
 Project-URL: documentation, https://github.com/touxiaoling/adbutils_async
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
-License-File: AUTHORS
+Requires-Dist: httpx
+Requires-Dist: Pillow
+Requires-Dist: deprecation
+Requires-Dist: retry
+Requires-Dist: apkutils2
 
 # adbutils_async
 [![PyPI](https://img.shields.io/pypi/v/adbutils_async.svg?color=blue)](https://pypi.org/project/adbutils_async/#history)
 
 Python adb async library for adb service (Only support Python3.10+)
 
 fork from [adbutils](https://github.com/openatx/adbutils)
```

### Comparing `adbutils_async-0.0.2/build_wheel.py` & `adbutils_async-0.0.3/build_wheel.py`

 * *Files identical despite different names*

### Comparing `adbutils_async-0.0.2/setup.cfg` & `adbutils_async-0.0.3/setup.cfg`

 * *Files identical despite different names*

