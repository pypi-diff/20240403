# Comparing `tmp/crawler_analytics-0.1.8.tar.gz` & `tmp/crawler_analytics-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "crawler_analytics-0.1.8.tar", max compression
+gzip compressed data, was "crawler_analytics-0.1.9.tar", max compression
```

## Comparing `crawler_analytics-0.1.8.tar` & `crawler_analytics-0.1.9.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0        0 2024-03-12 13:13:27.582306 crawler_analytics-0.1.8/README.md
--rw-r--r--   0        0        0       45 2024-03-13 01:56:07.452611 crawler_analytics-0.1.8/crawler_analytics/__init__.py
--rw-r--r--   0        0        0     2943 2024-03-14 01:19:00.109407 crawler_analytics-0.1.8/crawler_analytics/main.py
--rw-r--r--   0        0        0      759 2024-03-14 01:37:50.044047 crawler_analytics-0.1.8/crawler_analytics/server.py
--rw-r--r--   0        0        0      587 2024-03-14 01:38:24.031935 crawler_analytics-0.1.8/pyproject.toml
--rw-r--r--   0        0        0      554 1970-01-01 00:00:00.000000 crawler_analytics-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0        0 2024-03-12 13:13:27.582306 crawler_analytics-0.1.9/README.md
+-rw-r--r--   0        0        0       45 2024-03-13 01:56:07.452611 crawler_analytics-0.1.9/crawler_analytics/__init__.py
+-rw-r--r--   0        0        0     2955 2024-03-14 01:40:19.063442 crawler_analytics-0.1.9/crawler_analytics/main.py
+-rw-r--r--   0        0        0      759 2024-03-14 01:37:50.044047 crawler_analytics-0.1.9/crawler_analytics/server.py
+-rw-r--r--   0        0        0      587 2024-03-14 01:40:27.452159 crawler_analytics-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0      554 1970-01-01 00:00:00.000000 crawler_analytics-0.1.9/PKG-INFO
```

### Comparing `crawler_analytics-0.1.8/crawler_analytics/main.py` & `crawler_analytics-0.1.9/crawler_analytics/main.py`

 * *Files 0% similar despite different names*

```diff
@@ -53,18 +53,18 @@
         }
 
     async def set_target(self, n: int):
         target_key = self._key(KEYS["count"]["target"])
         await self.r.set(target_key, n)
 
     async def _get_today(self):
-        return self._get_image_count(start_time=int(time.time()) - 86400)
+        return await self._get_image_count(start_time=int(time.time()) - 86400)
 
     async def _get_yesterday(self):
-        return self._get_image_count(start_time=int(time.time()) - 172800)
+        return await self._get_image_count(start_time=int(time.time()) - 172800)
 
     async def _get_image_count(self, start_time: int = None):
         """先删除超过保留期限的数据，再查询"""
         current_time = time.time()
         end_time = current_time - 259200  # 三天
         await self.r.zremrangebyscore(self._key(KEYS["images"]), min=0, max=end_time)
```

### Comparing `crawler_analytics-0.1.8/crawler_analytics/server.py` & `crawler_analytics-0.1.9/crawler_analytics/server.py`

 * *Files identical despite different names*

### Comparing `crawler_analytics-0.1.8/pyproject.toml` & `crawler_analytics-0.1.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "crawler-analytics"
-version = "0.1.8"
+version = "0.1.9"
 description = ""
 authors = ["AprilNEA <github@sku.moe>"]
 readme = "README.md"
 packages = [{ include = "crawler_analytics" }]
 
 [tool.poetry.dependencies]
 python = "^3.8"
```

### Comparing `crawler_analytics-0.1.8/PKG-INFO` & `crawler_analytics-0.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: crawler-analytics
-Version: 0.1.8
+Version: 0.1.9
 Summary: 
 Author: AprilNEA
 Author-email: github@sku.moe
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

