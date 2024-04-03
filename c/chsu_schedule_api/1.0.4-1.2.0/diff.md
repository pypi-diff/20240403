# Comparing `tmp/chsu_schedule_api-1.0.4.tar.gz` & `tmp/chsu_schedule_api-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chsu_schedule_api-1.0.4.tar", max compression
+gzip compressed data, was "chsu_schedule_api-1.2.0.tar", max compression
```

## Comparing `chsu_schedule_api-1.0.4.tar` & `chsu_schedule_api-1.2.0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rw-r--r--   0        0        0      153 2024-03-28 22:56:25.487494 chsu_schedule_api-1.0.4/chsu_schedule_api/__init__.py
--rw-r--r--   0        0        0       86 2024-03-28 22:56:25.487494 chsu_schedule_api-1.0.4/chsu_schedule_api/api/__init__.py
--rw-r--r--   0        0        0     1108 2024-03-28 22:56:25.487494 chsu_schedule_api-1.0.4/chsu_schedule_api/api/abc.py
--rw-r--r--   0        0        0     4524 2024-03-28 22:56:25.487494 chsu_schedule_api-1.0.4/chsu_schedule_api/api/api.py
--rw-r--r--   0        0        0      116 2024-03-28 22:56:25.488497 chsu_schedule_api-1.0.4/chsu_schedule_api/client/__init__.py
--rw-r--r--   0        0        0     1071 2024-03-28 22:56:25.488497 chsu_schedule_api-1.0.4/chsu_schedule_api/client/abc.py
--rw-r--r--   0        0        0     2065 2024-03-28 22:56:25.488497 chsu_schedule_api-1.0.4/chsu_schedule_api/client/aiohttp.py
--rw-r--r--   0        0        0      298 2024-03-28 22:56:25.488497 chsu_schedule_api-1.0.4/chsu_schedule_api/constants.py
--rw-r--r--   0        0        0      116 2024-03-28 22:56:25.488497 chsu_schedule_api-1.0.4/chsu_schedule_api/enums.py
--rw-r--r--   0        0        0      232 2024-03-28 22:56:25.488497 chsu_schedule_api-1.0.4/chsu_schedule_api/errors.py
--rw-r--r--   0        0        0      764 2024-03-29 09:42:46.272712 chsu_schedule_api-1.0.4/chsu_schedule_api/models/__init__.py
--rw-r--r--   0        0        0      302 2024-03-28 22:56:25.490518 chsu_schedule_api-1.0.4/chsu_schedule_api/models/auditorium.py
--rw-r--r--   0        0        0      208 2024-03-29 08:16:57.081988 chsu_schedule_api-1.0.4/chsu_schedule_api/models/base.py
--rw-r--r--   0        0        0      106 2024-03-28 22:56:25.490997 chsu_schedule_api-1.0.4/chsu_schedule_api/models/building.py
--rw-r--r--   0        0        0      411 2024-03-28 22:56:25.490997 chsu_schedule_api-1.0.4/chsu_schedule_api/models/department.py
--rw-r--r--   0        0        0      108 2024-03-28 22:56:25.491524 chsu_schedule_api-1.0.4/chsu_schedule_api/models/discipline.py
--rw-r--r--   0        0        0      356 2024-03-28 22:56:25.491524 chsu_schedule_api-1.0.4/chsu_schedule_api/models/student_group.py
--rw-r--r--   0        0        0      332 2024-03-28 22:56:25.491524 chsu_schedule_api-1.0.4/chsu_schedule_api/models/teacher.py
--rw-r--r--   0        0        0     2449 2024-03-29 08:17:12.598060 chsu_schedule_api-1.0.4/chsu_schedule_api/models/timetable.py
--rw-r--r--   0        0        0     1093 2024-03-28 22:56:25.486469 chsu_schedule_api-1.0.4/LICENSE
--rw-r--r--   0        0        0     1378 2024-03-29 09:48:01.400559 chsu_schedule_api-1.0.4/pyproject.toml
--rw-r--r--   0        0        0     1572 2024-03-28 23:14:49.426570 chsu_schedule_api-1.0.4/README.md
--rw-r--r--   0        0        0     2157 1970-01-01 00:00:00.000000 chsu_schedule_api-1.0.4/PKG-INFO
+-rw-r--r--   0        0        0      153 2024-04-03 17:16:51.794488 chsu_schedule_api-1.2.0/chsu_schedule_api/__init__.py
+-rw-r--r--   0        0        0       86 2024-04-03 17:16:51.794488 chsu_schedule_api-1.2.0/chsu_schedule_api/api/__init__.py
+-rw-r--r--   0        0        0     1082 2024-04-03 17:31:25.471419 chsu_schedule_api-1.2.0/chsu_schedule_api/api/abc.py
+-rw-r--r--   0        0        0     5980 2024-04-03 19:13:25.257881 chsu_schedule_api-1.2.0/chsu_schedule_api/api/api.py
+-rw-r--r--   0        0        0      116 2024-04-03 17:16:51.794488 chsu_schedule_api-1.2.0/chsu_schedule_api/client/__init__.py
+-rw-r--r--   0        0        0     1071 2024-04-03 17:16:51.794488 chsu_schedule_api-1.2.0/chsu_schedule_api/client/abc.py
+-rw-r--r--   0        0        0     2065 2024-04-03 17:16:51.794488 chsu_schedule_api-1.2.0/chsu_schedule_api/client/aiohttp.py
+-rw-r--r--   0        0        0      298 2024-04-03 17:16:51.794488 chsu_schedule_api-1.2.0/chsu_schedule_api/constants.py
+-rw-r--r--   0        0        0      116 2024-04-03 17:16:51.794488 chsu_schedule_api-1.2.0/chsu_schedule_api/enums.py
+-rw-r--r--   0        0        0      326 2024-04-03 18:34:26.473939 chsu_schedule_api-1.2.0/chsu_schedule_api/errors.py
+-rw-r--r--   0        0        0      882 2024-04-03 17:42:51.378097 chsu_schedule_api-1.2.0/chsu_schedule_api/models/__init__.py
+-rw-r--r--   0        0        0      302 2024-04-03 17:16:51.794488 chsu_schedule_api-1.2.0/chsu_schedule_api/models/auditorium.py
+-rw-r--r--   0        0        0      208 2024-04-03 17:16:51.794488 chsu_schedule_api-1.2.0/chsu_schedule_api/models/base.py
+-rw-r--r--   0        0        0      106 2024-04-03 17:16:51.794488 chsu_schedule_api-1.2.0/chsu_schedule_api/models/building.py
+-rw-r--r--   0        0        0      411 2024-04-03 17:16:51.799035 chsu_schedule_api-1.2.0/chsu_schedule_api/models/department.py
+-rw-r--r--   0        0        0      108 2024-04-03 17:16:51.799035 chsu_schedule_api-1.2.0/chsu_schedule_api/models/discipline.py
+-rw-r--r--   0        0        0      356 2024-04-03 17:16:51.799035 chsu_schedule_api-1.2.0/chsu_schedule_api/models/student_group.py
+-rw-r--r--   0        0        0      332 2024-04-03 17:16:51.799035 chsu_schedule_api-1.2.0/chsu_schedule_api/models/teacher.py
+-rw-r--r--   0        0        0     2977 2024-04-03 19:04:29.238962 chsu_schedule_api-1.2.0/chsu_schedule_api/models/timetable.py
+-rw-r--r--   0        0        0     1093 2024-04-03 17:16:51.794488 chsu_schedule_api-1.2.0/LICENSE
+-rw-r--r--   0        0        0     1378 2024-04-03 19:27:47.899358 chsu_schedule_api-1.2.0/pyproject.toml
+-rw-r--r--   0        0        0     2293 2024-04-03 19:16:31.736270 chsu_schedule_api-1.2.0/README.md
+-rw-r--r--   0        0        0     2844 1970-01-01 00:00:00.000000 chsu_schedule_api-1.2.0/PKG-INFO
```

### Comparing `chsu_schedule_api-1.0.4/chsu_schedule_api/api/abc.py` & `chsu_schedule_api-1.2.0/chsu_schedule_api/api/abc.py`

 * *Files 8% similar despite different names*

```diff
@@ -12,17 +12,16 @@
     """Abstract API class"""
 
     _client: "ABCHttpClient"
     _auth_data: dict[str, str]
     _headers: dict[str, str]
 
     @abstractmethod
-    def __init__(
-        self, username: str, password: str, client: "ABCHttpClient | None"
-    ) -> None: ...
+    def __init__(self, client: "ABCHttpClient") -> None:
+        self._client = client
 
     async def request(
         self, method: "Methods", path: str, data: object = None, **kwargs
     ) -> str | None:
         """Make http request"""
         return await self._client.request(
             method, f"{BASE_URL}{path}", data=data, **kwargs
```

### Comparing `chsu_schedule_api-1.0.4/chsu_schedule_api/client/abc.py` & `chsu_schedule_api-1.2.0/chsu_schedule_api/client/abc.py`

 * *Files identical despite different names*

### Comparing `chsu_schedule_api-1.0.4/chsu_schedule_api/client/aiohttp.py` & `chsu_schedule_api-1.2.0/chsu_schedule_api/client/aiohttp.py`

 * *Files identical despite different names*

### Comparing `chsu_schedule_api-1.0.4/chsu_schedule_api/models/__init__.py` & `chsu_schedule_api-1.2.0/chsu_schedule_api/models/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -4,34 +4,40 @@
 from .department import Department, Node
 from .discipline import Discipline
 from .student_group import Chair, Faculty, StudentGroup
 from .teacher import Teacher
 from .timetable import (
     Full,
     Group,
+    GroupId,
     Lecturer,
+    LecturerId,
     TimeTable,
     TimeTableType,
+    TitleTimeTableType,
     TTAuditory,
     TTStudentGroup,
 )
 
 __all__ = (
     "Full",
+    "Group",
+    "GroupId",
+    "Lecturer",
     "Auditorium",
     "CHSUModel",
     "CHSUResponseModel",
     "Building",
     "Department",
     "Node",
     "Discipline",
     "Chair",
     "Faculty",
     "StudentGroup",
     "Teacher",
-    "Group",
-    "Lecturer",
+    "LecturerId",
     "TimeTable",
     "TimeTableType",
+    "TitleTimeTableType",
     "TTAuditory",
     "TTStudentGroup",
 )
```

### Comparing `chsu_schedule_api-1.0.4/LICENSE` & `chsu_schedule_api-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `chsu_schedule_api-1.0.4/pyproject.toml` & `chsu_schedule_api-1.2.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "chsu_schedule_api"
-version = "1.0.4"
+version = "1.2.0"
 description = "Asynchronous API wrapper for CHSU schedule API"
 authors = ["VoVcHiC <hello@chsutech.ru>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/vovchic17/CHSUScheduleAPI"
 repository = "https://github.com/vovchic17/CHSUScheduleAPI"
 keywords = ["chsu", "schedule", "api"]
```

### Comparing `chsu_schedule_api-1.0.4/README.md` & `chsu_schedule_api-1.2.0/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -24,14 +24,15 @@
 Install via pip
 
 ```shell
 pip install chsu_schedule_api
 ```
 
 ## Example
+Get building list
 ```python
 import asyncio
 
 from chsu_schedule_api import CHSUApi
 
 client = CHSUApi(username="USERNAME", password="PASSWORD")
 
@@ -42,9 +43,42 @@
     print(buildings)
 
 
 if __name__ == "__main__":
     asyncio.run(main())
 ```
 
+## Example
+Get your group schedule
+```python
+import asyncio
+
+from chsu_schedule_api import CHSUApi
+from chsu_schedule_api.models import Group
+
+client = CHSUApi(username="USERNAME", password="PASSWORD")
+
+async def main() -> None:
+    await client.auth_signin()
+    group_tt = await client.get_time_table(
+        Group(
+            title="1ИСб-01-1оп-22",
+            from_date="03.04.2024",
+            to_date="03.04.2024",
+        )
+    )
+
+    for tt in group_tt:
+        print(
+            tt.start_time,
+            tt.end_time,
+            tt.discipline.title,
+            tt.auditory.title
+        )
+
+
+if __name__ == "__main__":
+    asyncio.run(main())
+```
+
 ## License
 MIT
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `chsu_schedule_api-1.0.4/PKG-INFO` & `chsu_schedule_api-1.2.0/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chsu_schedule_api
-Version: 1.0.4
+Version: 1.2.0
 Summary: Asynchronous API wrapper for CHSU schedule API
 Home-page: https://github.com/vovchic17/CHSUScheduleAPI
 License: MIT
 Keywords: chsu,schedule,api
 Author: VoVcHiC
 Author-email: hello@chsutech.ru
 Requires-Python: >=3.12,<4.0
@@ -42,14 +42,15 @@
 Install via pip
 
 ```shell
 pip install chsu_schedule_api
 ```
 
 ## Example
+Get building list
 ```python
 import asyncio
 
 from chsu_schedule_api import CHSUApi
 
 client = CHSUApi(username="USERNAME", password="PASSWORD")
 
@@ -60,9 +61,42 @@
     print(buildings)
 
 
 if __name__ == "__main__":
     asyncio.run(main())
 ```
 
+## Example
+Get your group schedule
+```python
+import asyncio
+
+from chsu_schedule_api import CHSUApi
+from chsu_schedule_api.models import Group
+
+client = CHSUApi(username="USERNAME", password="PASSWORD")
+
+async def main() -> None:
+    await client.auth_signin()
+    group_tt = await client.get_time_table(
+        Group(
+            title="1ИСб-01-1оп-22",
+            from_date="03.04.2024",
+            to_date="03.04.2024",
+        )
+    )
+
+    for tt in group_tt:
+        print(
+            tt.start_time,
+            tt.end_time,
+            tt.discipline.title,
+            tt.auditory.title
+        )
+
+
+if __name__ == "__main__":
+    asyncio.run(main())
+```
+
 ## License
 MIT
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

