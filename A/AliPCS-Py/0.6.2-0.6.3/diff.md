# Comparing `tmp/alipcs_py-0.6.2.tar.gz` & `tmp/alipcs_py-0.6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "alipcs_py-0.6.2.tar", max compression
+gzip compressed data, was "alipcs_py-0.6.3.tar", max compression
```

## Comparing `alipcs_py-0.6.2.tar` & `alipcs_py-0.6.3.tar`

### file list

```diff
@@ -1,62 +1,62 @@
--rw-r--r--   0        0        0     1054 2021-08-22 03:34:43.538852 alipcs_py-0.6.2/LICENSE
--rw-r--r--   0        0        0    43879 2023-04-24 09:44:53.678600 alipcs_py-0.6.2/README.md
--rw-r--r--   0        0        0      106 2023-05-09 14:44:32.236305 alipcs_py-0.6.2/alipcs_py/__init__.py
--rw-r--r--   0        0        0      240 2023-04-24 04:55:07.710097 alipcs_py-0.6.2/alipcs_py/alipcs/__init__.py
--rw-r--r--   0        0        0    39076 2023-07-28 10:23:53.101308 alipcs_py-0.6.2/alipcs_py/alipcs/api.py
--rw-r--r--   0        0        0     2053 2023-06-30 06:02:57.163863 alipcs_py-0.6.2/alipcs_py/alipcs/errors.py
--rw-r--r--   0        0        0    19020 2023-07-28 10:56:37.768379 alipcs_py-0.6.2/alipcs_py/alipcs/inner.py
--rw-r--r--   0        0        0    44264 2023-09-10 09:39:59.259564 alipcs_py-0.6.2/alipcs_py/alipcs/pcs.py
--rw-r--r--   0        0        0    12095 2021-08-22 03:34:43.604109 alipcs_py-0.6.2/alipcs_py/alipcs/phone.py
--rw-r--r--   0        0        0     1446 2023-04-24 04:55:07.713710 alipcs_py-0.6.2/alipcs_py/alipcs/tree.py
--rw-r--r--   0        0        0      122 2021-09-18 06:46:25.830052 alipcs_py-0.6.2/alipcs_py/app/__init__.py
--rw-r--r--   0        0        0     8026 2023-04-24 04:55:07.714364 alipcs_py-0.6.2/alipcs_py/app/account.py
--rw-r--r--   0        0        0    50217 2023-09-25 15:48:47.875775 alipcs_py-0.6.2/alipcs_py/app/app.py
--rw-r--r--   0        0        0      825 2022-03-01 05:54:20.767866 alipcs_py-0.6.2/alipcs_py/app/config.py
--rw-r--r--   0        0        0        0 2021-08-22 03:34:43.630951 alipcs_py-0.6.2/alipcs_py/commands/__init__.py
--rw-r--r--   0        0        0      788 2022-12-04 09:09:43.288098 alipcs_py-0.6.2/alipcs_py/commands/cat.py
--rw-r--r--   0        0        0      653 2023-04-24 04:55:07.715731 alipcs_py-0.6.2/alipcs_py/commands/crypto.py
--rw-r--r--   0        0        0    14746 2023-04-24 04:55:07.716544 alipcs_py-0.6.2/alipcs_py/commands/display.py
--rw-r--r--   0        0        0    13914 2023-12-04 11:53:45.142762 alipcs_py-0.6.2/alipcs_py/commands/download.py
--rw-r--r--   0        0        0      494 2022-08-15 03:16:20.571025 alipcs_py-0.6.2/alipcs_py/commands/env.py
--rw-r--r--   0        0        0       40 2021-08-22 03:34:43.661676 alipcs_py-0.6.2/alipcs_py/commands/errors.py
--rw-r--r--   0        0        0     2557 2023-02-15 16:28:39.324554 alipcs_py-0.6.2/alipcs_py/commands/file_operators.py
--rw-r--r--   0        0        0    20271 2023-03-03 16:42:13.787873 alipcs_py-0.6.2/alipcs_py/commands/index.html
--rw-r--r--   0        0        0     5938 2023-04-24 04:55:07.718624 alipcs_py-0.6.2/alipcs_py/commands/list_files.py
--rw-r--r--   0        0        0      508 2022-12-04 07:57:21.765695 alipcs_py-0.6.2/alipcs_py/commands/log.py
--rw-r--r--   0        0        0     1250 2023-04-24 04:55:07.719052 alipcs_py-0.6.2/alipcs_py/commands/login.py
--rw-r--r--   0        0        0     8868 2023-12-04 11:55:57.794558 alipcs_py-0.6.2/alipcs_py/commands/play.py
--rw-r--r--   0        0        0      805 2021-09-20 14:44:04.367772 alipcs_py-0.6.2/alipcs_py/commands/search.py
--rw-r--r--   0        0        0     7029 2023-12-04 12:14:55.431425 alipcs_py-0.6.2/alipcs_py/commands/server.py
--rw-r--r--   0        0        0     9314 2023-09-25 15:50:16.051880 alipcs_py-0.6.2/alipcs_py/commands/share.py
--rw-r--r--   0        0        0     2670 2023-04-24 04:55:07.722333 alipcs_py-0.6.2/alipcs_py/commands/sifter.py
--rw-r--r--   0        0        0     2900 2023-04-24 04:55:07.723021 alipcs_py-0.6.2/alipcs_py/commands/sync.py
--rw-r--r--   0        0        0    22738 2023-07-28 11:05:10.789920 alipcs_py-0.6.2/alipcs_py/commands/upload.py
--rw-r--r--   0        0        0      199 2022-08-15 05:04:44.362792 alipcs_py-0.6.2/alipcs_py/commands/user.py
--rw-r--r--   0        0        0     1317 2021-08-22 03:34:43.572027 alipcs_py-0.6.2/alipcs_py/common/cache.py
--rw-r--r--   0        0        0      941 2021-08-22 03:34:43.565972 alipcs_py-0.6.2/alipcs_py/common/concurrent.py
--rw-r--r--   0        0        0      188 2021-08-22 03:34:43.600492 alipcs_py-0.6.2/alipcs_py/common/constant.py
--rw-r--r--   0        0        0     8745 2023-04-24 04:55:07.724749 alipcs_py-0.6.2/alipcs_py/common/crypto.py
--rw-r--r--   0        0        0      751 2023-04-24 04:55:07.725914 alipcs_py-0.6.2/alipcs_py/common/date.py
--rw-r--r--   0        0        0     3328 2022-12-04 08:32:10.634459 alipcs_py-0.6.2/alipcs_py/common/downloader.py
--rw-r--r--   0        0        0     1160 2021-09-18 06:46:25.816885 alipcs_py-0.6.2/alipcs_py/common/event.py
--rw-r--r--   0        0        0     3179 2021-08-22 03:34:43.569872 alipcs_py-0.6.2/alipcs_py/common/file_type.py
--rw-r--r--   0        0        0    33598 2023-08-05 12:18:49.044331 alipcs_py-0.6.2/alipcs_py/common/io.py
--rw-r--r--   0        0        0     2810 2021-08-22 03:34:43.602159 alipcs_py-0.6.2/alipcs_py/common/keyboard.py
--rw-r--r--   0        0        0     1087 2022-12-04 07:54:57.943327 alipcs_py-0.6.2/alipcs_py/common/log.py
--rw-r--r--   0        0        0      700 2022-03-20 08:23:18.211962 alipcs_py-0.6.2/alipcs_py/common/net.py
--rw-r--r--   0        0        0      165 2021-08-22 03:34:43.568880 alipcs_py-0.6.2/alipcs_py/common/number.py
--rw-r--r--   0        0        0     1554 2022-12-04 07:52:11.933700 alipcs_py-0.6.2/alipcs_py/common/path.py
--rw-r--r--   0        0        0      143 2021-08-22 03:34:43.595732 alipcs_py-0.6.2/alipcs_py/common/platform.py
--rw-r--r--   0        0        0     1222 2023-05-09 14:38:28.798699 alipcs_py-0.6.2/alipcs_py/common/progress_bar.py
--rw-r--r--   0        0        0     1322 2021-08-22 03:34:43.598103 alipcs_py-0.6.2/alipcs_py/common/simple_cipher.pyx
--rw-r--r--   0        0        0       73 2021-08-22 03:34:43.596516 alipcs_py-0.6.2/alipcs_py/common/url.py
--rw-r--r--   0        0        0      451 2022-03-02 13:55:46.279575 alipcs_py-0.6.2/alipcs_py/common/util.py
--rw-r--r--   0        0        0     1208 2022-03-01 06:20:58.123489 alipcs_py-0.6.2/alipcs_py/config/__init__.py
--rw-r--r--   0        0        0        0 2022-03-06 15:08:01.483390 alipcs_py-0.6.2/alipcs_py/storage/__init__.py
--rw-r--r--   0        0        0     6121 2023-04-24 04:55:07.728382 alipcs_py-0.6.2/alipcs_py/storage/store.py
--rw-r--r--   0        0        0     5188 2023-04-24 04:55:07.729402 alipcs_py-0.6.2/alipcs_py/storage/tables.py
--rw-r--r--   0        0        0     1424 2021-08-22 03:34:43.602731 alipcs_py-0.6.2/alipcs_py/utils.py
--rw-r--r--   0        0        0      735 2021-09-18 06:47:25.953980 alipcs_py-0.6.2/build.py
--rw-r--r--   0        0        0     1494 2023-12-04 12:32:06.531701 alipcs_py-0.6.2/pyproject.toml
--rw-r--r--   0        0        0    46242 1970-01-01 00:00:00.000000 alipcs_py-0.6.2/setup.py
--rw-r--r--   0        0        0    45539 1970-01-01 00:00:00.000000 alipcs_py-0.6.2/PKG-INFO
+-rw-r--r--   0        0        0     1054 2021-08-22 03:34:43.538852 alipcs_py-0.6.3/LICENSE
+-rw-r--r--   0        0        0    43879 2023-04-24 09:44:53.678600 alipcs_py-0.6.3/README.md
+-rw-r--r--   0        0        0      106 2024-02-04 07:45:30.265992 alipcs_py-0.6.3/alipcs_py/__init__.py
+-rw-r--r--   0        0        0      240 2023-04-24 04:55:07.710097 alipcs_py-0.6.3/alipcs_py/alipcs/__init__.py
+-rw-r--r--   0        0        0    39076 2024-02-03 16:41:15.701600 alipcs_py-0.6.3/alipcs_py/alipcs/api.py
+-rw-r--r--   0        0        0     2053 2023-06-30 06:02:57.163863 alipcs_py-0.6.3/alipcs_py/alipcs/errors.py
+-rw-r--r--   0        0        0    19020 2023-07-28 10:56:37.768379 alipcs_py-0.6.3/alipcs_py/alipcs/inner.py
+-rw-r--r--   0        0        0    44313 2024-02-04 06:49:57.573145 alipcs_py-0.6.3/alipcs_py/alipcs/pcs.py
+-rw-r--r--   0        0        0    12095 2021-08-22 03:34:43.604109 alipcs_py-0.6.3/alipcs_py/alipcs/phone.py
+-rw-r--r--   0        0        0     1446 2023-04-24 04:55:07.713710 alipcs_py-0.6.3/alipcs_py/alipcs/tree.py
+-rw-r--r--   0        0        0      122 2021-09-18 06:46:25.830052 alipcs_py-0.6.3/alipcs_py/app/__init__.py
+-rw-r--r--   0        0        0     8026 2023-04-24 04:55:07.714364 alipcs_py-0.6.3/alipcs_py/app/account.py
+-rw-r--r--   0        0        0    50253 2024-01-23 08:34:17.316145 alipcs_py-0.6.3/alipcs_py/app/app.py
+-rw-r--r--   0        0        0      825 2022-03-01 05:54:20.767866 alipcs_py-0.6.3/alipcs_py/app/config.py
+-rw-r--r--   0        0        0        0 2021-08-22 03:34:43.630951 alipcs_py-0.6.3/alipcs_py/commands/__init__.py
+-rw-r--r--   0        0        0      788 2022-12-04 09:09:43.288098 alipcs_py-0.6.3/alipcs_py/commands/cat.py
+-rw-r--r--   0        0        0      653 2023-04-24 04:55:07.715731 alipcs_py-0.6.3/alipcs_py/commands/crypto.py
+-rw-r--r--   0        0        0    14746 2023-04-24 04:55:07.716544 alipcs_py-0.6.3/alipcs_py/commands/display.py
+-rw-r--r--   0        0        0    13914 2023-12-04 11:53:45.142762 alipcs_py-0.6.3/alipcs_py/commands/download.py
+-rw-r--r--   0        0        0      494 2022-08-15 03:16:20.571025 alipcs_py-0.6.3/alipcs_py/commands/env.py
+-rw-r--r--   0        0        0       40 2021-08-22 03:34:43.661676 alipcs_py-0.6.3/alipcs_py/commands/errors.py
+-rw-r--r--   0        0        0     2557 2023-02-15 16:28:39.324554 alipcs_py-0.6.3/alipcs_py/commands/file_operators.py
+-rw-r--r--   0        0        0    20271 2023-03-03 16:42:13.787873 alipcs_py-0.6.3/alipcs_py/commands/index.html
+-rw-r--r--   0        0        0     5938 2023-04-24 04:55:07.718624 alipcs_py-0.6.3/alipcs_py/commands/list_files.py
+-rw-r--r--   0        0        0      508 2022-12-04 07:57:21.765695 alipcs_py-0.6.3/alipcs_py/commands/log.py
+-rw-r--r--   0        0        0     1250 2023-04-24 04:55:07.719052 alipcs_py-0.6.3/alipcs_py/commands/login.py
+-rw-r--r--   0        0        0     8868 2023-12-04 11:55:57.794558 alipcs_py-0.6.3/alipcs_py/commands/play.py
+-rw-r--r--   0        0        0      805 2021-09-20 14:44:04.367772 alipcs_py-0.6.3/alipcs_py/commands/search.py
+-rw-r--r--   0        0        0     7029 2023-12-04 12:14:55.431425 alipcs_py-0.6.3/alipcs_py/commands/server.py
+-rw-r--r--   0        0        0     9314 2023-09-25 15:50:16.051880 alipcs_py-0.6.3/alipcs_py/commands/share.py
+-rw-r--r--   0        0        0     2670 2023-04-24 04:55:07.722333 alipcs_py-0.6.3/alipcs_py/commands/sifter.py
+-rw-r--r--   0        0        0     2900 2023-04-24 04:55:07.723021 alipcs_py-0.6.3/alipcs_py/commands/sync.py
+-rw-r--r--   0        0        0    22802 2023-12-21 09:23:20.784192 alipcs_py-0.6.3/alipcs_py/commands/upload.py
+-rw-r--r--   0        0        0      199 2022-08-15 05:04:44.362792 alipcs_py-0.6.3/alipcs_py/commands/user.py
+-rw-r--r--   0        0        0     1317 2021-08-22 03:34:43.572027 alipcs_py-0.6.3/alipcs_py/common/cache.py
+-rw-r--r--   0        0        0      941 2021-08-22 03:34:43.565972 alipcs_py-0.6.3/alipcs_py/common/concurrent.py
+-rw-r--r--   0        0        0      188 2021-08-22 03:34:43.600492 alipcs_py-0.6.3/alipcs_py/common/constant.py
+-rw-r--r--   0        0        0     8745 2023-04-24 04:55:07.724749 alipcs_py-0.6.3/alipcs_py/common/crypto.py
+-rw-r--r--   0        0        0      751 2023-04-24 04:55:07.725914 alipcs_py-0.6.3/alipcs_py/common/date.py
+-rw-r--r--   0        0        0     3328 2022-12-04 08:32:10.634459 alipcs_py-0.6.3/alipcs_py/common/downloader.py
+-rw-r--r--   0        0        0     1160 2021-09-18 06:46:25.816885 alipcs_py-0.6.3/alipcs_py/common/event.py
+-rw-r--r--   0        0        0     3179 2021-08-22 03:34:43.569872 alipcs_py-0.6.3/alipcs_py/common/file_type.py
+-rw-r--r--   0        0        0    33598 2023-08-05 12:18:49.044331 alipcs_py-0.6.3/alipcs_py/common/io.py
+-rw-r--r--   0        0        0     2810 2021-08-22 03:34:43.602159 alipcs_py-0.6.3/alipcs_py/common/keyboard.py
+-rw-r--r--   0        0        0     1087 2022-12-04 07:54:57.943327 alipcs_py-0.6.3/alipcs_py/common/log.py
+-rw-r--r--   0        0        0      700 2022-03-20 08:23:18.211962 alipcs_py-0.6.3/alipcs_py/common/net.py
+-rw-r--r--   0        0        0      165 2021-08-22 03:34:43.568880 alipcs_py-0.6.3/alipcs_py/common/number.py
+-rw-r--r--   0        0        0     1554 2022-12-04 07:52:11.933700 alipcs_py-0.6.3/alipcs_py/common/path.py
+-rw-r--r--   0        0        0      143 2021-08-22 03:34:43.595732 alipcs_py-0.6.3/alipcs_py/common/platform.py
+-rw-r--r--   0        0        0     1222 2023-05-09 14:38:28.798699 alipcs_py-0.6.3/alipcs_py/common/progress_bar.py
+-rw-r--r--   0        0        0     1322 2021-08-22 03:34:43.598103 alipcs_py-0.6.3/alipcs_py/common/simple_cipher.pyx
+-rw-r--r--   0        0        0       73 2021-08-22 03:34:43.596516 alipcs_py-0.6.3/alipcs_py/common/url.py
+-rw-r--r--   0        0        0      451 2022-03-02 13:55:46.279575 alipcs_py-0.6.3/alipcs_py/common/util.py
+-rw-r--r--   0        0        0     1208 2022-03-01 06:20:58.123489 alipcs_py-0.6.3/alipcs_py/config/__init__.py
+-rw-r--r--   0        0        0        0 2022-03-06 15:08:01.483390 alipcs_py-0.6.3/alipcs_py/storage/__init__.py
+-rw-r--r--   0        0        0     6121 2023-04-24 04:55:07.728382 alipcs_py-0.6.3/alipcs_py/storage/store.py
+-rw-r--r--   0        0        0     5188 2024-02-03 08:30:27.813935 alipcs_py-0.6.3/alipcs_py/storage/tables.py
+-rw-r--r--   0        0        0     1424 2021-08-22 03:34:43.602731 alipcs_py-0.6.3/alipcs_py/utils.py
+-rw-r--r--   0        0        0      735 2021-09-18 06:47:25.953980 alipcs_py-0.6.3/build.py
+-rw-r--r--   0        0        0     1556 2024-02-04 07:43:29.489216 alipcs_py-0.6.3/pyproject.toml
+-rw-r--r--   0        0        0    46242 1970-01-01 00:00:00.000000 alipcs_py-0.6.3/setup.py
+-rw-r--r--   0        0        0    45289 1970-01-01 00:00:00.000000 alipcs_py-0.6.3/PKG-INFO
```

### Comparing `alipcs_py-0.6.2/LICENSE` & `alipcs_py-0.6.3/LICENSE`

 * *Files identical despite different names*

### Comparing `alipcs_py-0.6.2/README.md` & `alipcs_py-0.6.3/README.md`

 * *Files identical despite different names*

### Comparing `alipcs_py-0.6.2/alipcs_py/alipcs/api.py` & `alipcs_py-0.6.3/alipcs_py/alipcs/api.py`

 * *Files identical despite different names*

### Comparing `alipcs_py-0.6.2/alipcs_py/alipcs/errors.py` & `alipcs_py-0.6.3/alipcs_py/alipcs/errors.py`

 * *Files identical despite different names*

### Comparing `alipcs_py-0.6.2/alipcs_py/alipcs/inner.py` & `alipcs_py-0.6.3/alipcs_py/alipcs/inner.py`

 * *Files identical despite different names*

### Comparing `alipcs_py-0.6.2/alipcs_py/alipcs/pcs.py` & `alipcs_py-0.6.3/alipcs_py/alipcs/pcs.py`

 * *Files 0% similar despite different names*

```diff
@@ -650,15 +650,18 @@
     @assert_ok
     @handle_error
     def rename(self, file_id: str, name: str):
         """Rename the file to `name`"""
 
         url = PcsNode.Update.url()
         data = dict(
-            check_name_mode="refuse", drive_id=self.default_drive_id, file_id=file_id, name=name  # or "auto_rename"
+            check_name_mode="refuse",
+            drive_id=self.default_drive_id,
+            file_id=file_id,
+            name=name,  # or "auto_rename"
         )
         resp = self._request(Method.Post, url, json=data)
         return resp.json()
 
     def copy(self, *file_ids: str):
         assert len(file_ids) > 1
 
@@ -1189,17 +1192,17 @@
             err = parse_error(info["code"], info=info)
             raise err
 
         self._user_id = info["user_id"]
         self._user_name = info["user_name"]
         self._nick_name = info["nick_name"]
         self._default_drive_id = info["default_drive_id"]
-        self._domain_id = info["domain_id"]
-        self._role = info["role"]
-        self._status = info["status"]
+        self._domain_id = info.get("domain_id")
+        self._role = info.get("role")
+        self._status = info.get("status")
 
         return info
 
     def meta(self, *file_ids: str, share_id: str = None):
         assert "root" not in file_ids, '"root" has NOT meta info'
 
         responses = []
```

### Comparing `alipcs_py-0.6.2/alipcs_py/alipcs/phone.py` & `alipcs_py-0.6.3/alipcs_py/alipcs/phone.py`

 * *Files identical despite different names*

### Comparing `alipcs_py-0.6.2/alipcs_py/alipcs/tree.py` & `alipcs_py-0.6.3/alipcs_py/alipcs/tree.py`

 * *Files identical despite different names*

### Comparing `alipcs_py-0.6.2/alipcs_py/app/account.py` & `alipcs_py-0.6.3/alipcs_py/app/account.py`

 * *Files identical despite different names*

### Comparing `alipcs_py-0.6.2/alipcs_py/app/app.py` & `alipcs_py-0.6.3/alipcs_py/app/app.py`

 * *Files 0% similar despite different names*

```diff
@@ -1218,15 +1218,19 @@
 @click.argument("localpaths", nargs=-1, type=str)
 @click.argument("remotedir", nargs=1, type=str)
 @click.option(
     "--upload-type",
     "-t",
     type=click.Choice([t.name for t in UploadType]),
     default=UploadType.Many.name,
-    help=("上传方式，Many: 同时上传多个文件，" "One: 一次只上传一个文件，但同时上传文件的多个分片 " "(阿里网盘不支持单文件并发上传。`upload --upload-type One` 失效)"),
+    help=(
+        "上传方式，Many: 同时上传多个文件，"
+        "One: 一次只上传一个文件，但同时上传文件的多个分片 "
+        "(阿里网盘不支持单文件并发上传。`upload --upload-type One` 失效)"
+    ),
 )
 @click.option("--encrypt-password", "--ep", type=str, default=None, help="加密密码，默认使用用户设置的")
 @click.option(
     "--encrypt-type",
     "-e",
     type=click.Choice([t.name for t in EncryptType]),
     default=EncryptType.No.name,
@@ -1571,15 +1575,17 @@
     _find_shared_links(keywords)
     print()
     _find_shared_files(keywords, verbose=verbose)
 
 
 @app.command()
 @click.argument("share_ids", nargs=-1, type=str)
-@click.option("--keyword", "-k", multiple=True, type=str, help="要删除文件名的关键字，如果为空则删除share_id下的所有文件")
+@click.option(
+    "--keyword", "-k", multiple=True, type=str, help="要删除文件名的关键字，如果为空则删除share_id下的所有文件"
+)
 @click.pass_context
 @handle_error
 @save_modified_user_data
 def deletestoredshared(ctx, share_ids, keyword):
     """删除本地保存的分享连接或文件
 
     注意: 使用这个命令必须将配置文件 ~/.alipcs-py/config.toml 中的 [share] store 设为 true
```

### Comparing `alipcs_py-0.6.2/alipcs_py/app/config.py` & `alipcs_py-0.6.3/alipcs_py/app/config.py`

 * *Files identical despite different names*

### Comparing `alipcs_py-0.6.2/alipcs_py/commands/cat.py` & `alipcs_py-0.6.3/alipcs_py/commands/cat.py`

 * *Files identical despite different names*

### Comparing `alipcs_py-0.6.2/alipcs_py/commands/crypto.py` & `alipcs_py-0.6.3/alipcs_py/commands/crypto.py`

 * *Files identical despite different names*

### Comparing `alipcs_py-0.6.2/alipcs_py/commands/display.py` & `alipcs_py-0.6.3/alipcs_py/commands/display.py`

 * *Files identical despite different names*

### Comparing `alipcs_py-0.6.2/alipcs_py/commands/download.py` & `alipcs_py-0.6.3/alipcs_py/commands/download.py`

 * *Files identical despite different names*

### Comparing `alipcs_py-0.6.2/alipcs_py/commands/file_operators.py` & `alipcs_py-0.6.3/alipcs_py/commands/file_operators.py`

 * *Files identical despite different names*

### Comparing `alipcs_py-0.6.2/alipcs_py/commands/index.html` & `alipcs_py-0.6.3/alipcs_py/commands/index.html`

 * *Files identical despite different names*

### Comparing `alipcs_py-0.6.2/alipcs_py/commands/list_files.py` & `alipcs_py-0.6.3/alipcs_py/commands/list_files.py`

 * *Files identical despite different names*

### Comparing `alipcs_py-0.6.2/alipcs_py/commands/login.py` & `alipcs_py-0.6.3/alipcs_py/commands/login.py`

 * *Files identical despite different names*

### Comparing `alipcs_py-0.6.2/alipcs_py/commands/play.py` & `alipcs_py-0.6.3/alipcs_py/commands/play.py`

 * *Files identical despite different names*

### Comparing `alipcs_py-0.6.2/alipcs_py/commands/search.py` & `alipcs_py-0.6.3/alipcs_py/commands/search.py`

 * *Files identical despite different names*

### Comparing `alipcs_py-0.6.2/alipcs_py/commands/server.py` & `alipcs_py-0.6.3/alipcs_py/commands/server.py`

 * *Files identical despite different names*

### Comparing `alipcs_py-0.6.2/alipcs_py/commands/share.py` & `alipcs_py-0.6.3/alipcs_py/commands/share.py`

 * *Files identical despite different names*

### Comparing `alipcs_py-0.6.2/alipcs_py/commands/sifter.py` & `alipcs_py-0.6.3/alipcs_py/commands/sifter.py`

 * *Files identical despite different names*

### Comparing `alipcs_py-0.6.2/alipcs_py/commands/sync.py` & `alipcs_py-0.6.3/alipcs_py/commands/sync.py`

 * *Files identical despite different names*

### Comparing `alipcs_py-0.6.2/alipcs_py/commands/upload.py` & `alipcs_py-0.6.3/alipcs_py/commands/upload.py`

 * *Files 1% similar despite different names*

```diff
@@ -569,15 +569,17 @@
     """Upload one file with one connection"""
 
     _wait_start()
 
     localpath, remotepath = from_to
 
     remotedir = posix_path_dirname(remotepath)
-    dest_dir = api.makedir_path(remotedir)
+    dest_dir = api.path(remotedir)
+    if dest_dir is None:
+        dest_dir = api.makedir_path(remotedir)
     dest_file_id = dest_dir.file_id
 
     filename = posix_path_basename(remotepath)
 
     if not _need_to_upload(api, remotepath, check_name_mode):
         remove_progress_task(task_id)
         return
```

### Comparing `alipcs_py-0.6.2/alipcs_py/common/cache.py` & `alipcs_py-0.6.3/alipcs_py/common/cache.py`

 * *Files identical despite different names*

### Comparing `alipcs_py-0.6.2/alipcs_py/common/concurrent.py` & `alipcs_py-0.6.3/alipcs_py/common/concurrent.py`

 * *Files identical despite different names*

### Comparing `alipcs_py-0.6.2/alipcs_py/common/crypto.py` & `alipcs_py-0.6.3/alipcs_py/common/crypto.py`

 * *Files identical despite different names*

### Comparing `alipcs_py-0.6.2/alipcs_py/common/date.py` & `alipcs_py-0.6.3/alipcs_py/common/date.py`

 * *Files identical despite different names*

### Comparing `alipcs_py-0.6.2/alipcs_py/common/downloader.py` & `alipcs_py-0.6.3/alipcs_py/common/downloader.py`

 * *Files identical despite different names*

### Comparing `alipcs_py-0.6.2/alipcs_py/common/event.py` & `alipcs_py-0.6.3/alipcs_py/common/event.py`

 * *Files identical despite different names*

### Comparing `alipcs_py-0.6.2/alipcs_py/common/file_type.py` & `alipcs_py-0.6.3/alipcs_py/common/file_type.py`

 * *Files identical despite different names*

### Comparing `alipcs_py-0.6.2/alipcs_py/common/io.py` & `alipcs_py-0.6.3/alipcs_py/common/io.py`

 * *Files identical despite different names*

### Comparing `alipcs_py-0.6.2/alipcs_py/common/keyboard.py` & `alipcs_py-0.6.3/alipcs_py/common/keyboard.py`

 * *Files identical despite different names*

### Comparing `alipcs_py-0.6.2/alipcs_py/common/log.py` & `alipcs_py-0.6.3/alipcs_py/common/log.py`

 * *Files identical despite different names*

### Comparing `alipcs_py-0.6.2/alipcs_py/common/net.py` & `alipcs_py-0.6.3/alipcs_py/common/net.py`

 * *Files identical despite different names*

### Comparing `alipcs_py-0.6.2/alipcs_py/common/path.py` & `alipcs_py-0.6.3/alipcs_py/common/path.py`

 * *Files identical despite different names*

### Comparing `alipcs_py-0.6.2/alipcs_py/common/progress_bar.py` & `alipcs_py-0.6.3/alipcs_py/common/progress_bar.py`

 * *Files identical despite different names*

### Comparing `alipcs_py-0.6.2/alipcs_py/common/simple_cipher.pyx` & `alipcs_py-0.6.3/alipcs_py/common/simple_cipher.pyx`

 * *Files identical despite different names*

### Comparing `alipcs_py-0.6.2/alipcs_py/config/__init__.py` & `alipcs_py-0.6.3/alipcs_py/config/__init__.py`

 * *Files identical despite different names*

### Comparing `alipcs_py-0.6.2/alipcs_py/storage/store.py` & `alipcs_py-0.6.3/alipcs_py/storage/store.py`

 * *Files identical despite different names*

### Comparing `alipcs_py-0.6.2/alipcs_py/storage/tables.py` & `alipcs_py-0.6.3/alipcs_py/storage/tables.py`

 * *Files 0% similar despite different names*

```diff
@@ -26,15 +26,15 @@
         data: Dict[str, Any] = {}
         columns = self.__class__._meta.columns  # type: ignore
         pcs_fields = pcs_item.__dataclass_fields__
         for col in columns.keys():
             if col in pcs_fields:
                 val = getattr(self, col)
                 if pcs_fields[col].type == typing.Optional[bool] or pcs_fields[col].type == bool:
-                    if val == None:
+                    if val is None:
                         data[col] = None
                     else:
                         data[col] = bool(val)
                 else:
                     data[col] = val
         return pcs_item(**data)
```

### Comparing `alipcs_py-0.6.2/alipcs_py/utils.py` & `alipcs_py-0.6.3/alipcs_py/utils.py`

 * *Files identical despite different names*

### Comparing `alipcs_py-0.6.2/build.py` & `alipcs_py-0.6.3/build.py`

 * *Files identical despite different names*

### Comparing `alipcs_py-0.6.2/pyproject.toml` & `alipcs_py-0.6.3/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 name = "AliPCS-Py"
 homepage = "https://github.com/PeterDing/AliPCS-Py"
-version = "0.6.2"
+version = "0.6.3"
 description = "Ali Pcs Api and App"
 authors = ["PeterDing <dfhayst@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 classifiers = [
     "Environment :: Console",
     "Intended Audience :: Developers",
@@ -15,21 +15,20 @@
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: 3.12",
 ]
-build = "build.py"
 
 [tool.black]
 line-length = 119
 
 [tool.ruff]
-ignore = ["E501", "F401", "F841"]
+ignore = ["E501", "E402", "F401", "F403", "F841"]
 line-length = 119
 
 [tool.poetry.dependencies]
 python = "^3.8"
 requests = ">=2.31"
 requests-toolbelt = ">=1.0"
 peewee = ">=3.17"
@@ -47,20 +46,23 @@
 cryptography = ">=41.0"
 ecdsa = ">=0.18"
 cython = ">=3.0"
 passlib = ">=1.7"
 
 [tool.poetry.group.dev.dependencies]
 pytest = ">=7.4"
-mypy = ">=1.7"
-black = ">=23.11"
+ruff = ">=0.2"
 setuptools = ">=69.0"
 cython = ">=3.0"
 
+[tool.poetry.build]
+script = "build.py"
+generate-setup-file = true
+
 [tool.poetry.scripts]
 AliPCS-Py = 'alipcs_py.app:main'
 
 [tool.pyright]
 reportGeneralTypeIssues = true
 
 [build-system]
-requires = ["cython", "wheel", "setuptools"]
+requires = ["poetry-core", "cython", "wheel", "setuptools"]
```

### Comparing `alipcs_py-0.6.2/setup.py` & `alipcs_py-0.6.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -33,16 +33,16 @@
  'typing-extensions>=4.8',
  'uvicorn>=0.24']
 
 entry_points = \
 {'console_scripts': ['AliPCS-Py = alipcs_py.app:main']}
 
 setup_kwargs = {
-    'name': 'alipcs-py',
-    'version': '0.6.2',
+    'name': 'AliPCS-Py',
+    'version': '0.6.3',
     'description': 'Ali Pcs Api and App',
     'long_description': '# AliPCS-Py\n\n**2023-04-24 支持 阿里云盘开放平台 api。**\n\n**2023-02-15 使用临时 API 接口，让下载可用。**\n\n**2023-02-14 阿里网盘 API 下载接口不再提供第三方应用使用。需要申请使用官方 API 接口。目前官方 API 接口在内测中。本项目已提交内测申请，等待回复中。在此期间下载功能不能使用。**\n\n[![PyPI version](https://badge.fury.io/py/alipcs-py.svg)](https://badge.fury.io/py/alipcs-py)\n![Build](https://github.com/PeterDing/AliPCS-Py/workflows/AliPCS-Py%20Build%20&%20Test/badge.svg)\n\nAn AliPCS API and An App\n\nAliPCS-Py 是阿里云盘的非官方 api 和一个命令行运用程序。\n\n---\n\n## 百度云盘 api 和 命令行客户端在 https://github.com/PeterDing/BaiduPCS-Py\n\n---\n\n- [安装](#安装)\n- [更新](#更新)\n- [API](#API)\n- [用法](#用法)\n- [命令别名](#命令别名)\n- [对多个帐号进行相同操作](#对多个帐号进行相同操作)\n\n#### 用户相关命令\n\n- [添加用户](#添加用户)\n- [显示当前用户的信息](#显示当前用户的信息)\n- [更新用户信息](#更新用户信息)\n- [显示所有用户](#显示所有用户)\n- [切换当前用户](#切换当前用户)\n- [删除一个用户](#删除一个用户)\n- [显示当前工作目录](#显示当前工作目录)\n- [切换当前工作目录](#切换当前工作目录)\n\n#### 无感加密解密文件\n\n- [设置文件加密密码](#设置文件加密密码)\n\n#### 文件操作相关命令\n\n- [文件操作](#文件操作)\n- [列出网盘路径下的文件](#列出网盘路径下的文件)\n- [搜索文件](#搜索文件)\n- [显示文件内容](#显示文件内容)\n- [创建目录](#创建目录)\n- [移动文件](#移动文件)\n- [文件重命名](#文件重命名)\n- [拷贝文件](#拷贝文件)\n- [删除文件](#删除文件)\n- [下载文件或目录](#下载文件或目录)\n- [播放媒体文件](#播放媒体文件)\n- [上传文件](#上传文件)\n- [同步本地目录到远端](#同步本地目录到远端)\n\n#### 秒传\n\n- [关于秒传连接](#关于秒传连接)\n\n#### 分享相关命令\n\n- [分享文件](#分享文件)\n- [列出分享链接](#列出分享链接)\n- [取消分享链接](#取消分享链接)\n- [列出其他用户分享链接中的文件](#列出其他用户分享链接中的文件)\n- [下载他人分享的文件](#下载他人分享的文件)\n- [播放他人分享的文件](#播放他人分享的文件)\n- [保存其他用户分享的链接](#保存其他用户分享的链接)\n\n#### 本地保存分享连接\n\n- [保存分享连接至本地](#保存分享连接至本地)\n- [显示本地保存的分享连接](#显示本地保存的分享连接)\n- [显示本地保存的分享文件](#显示本地保存的分享文件)\n- [查找本地保存的分享连接](#查找本地保存的分享连接)\n- [查找本地保存的分享文件](#查找本地保存的分享文件)\n- [查找本地保存的分享连接和文件](#查找本地保存的分享连接和文件)\n- [删除本地保存的分享连接或文件](#删除本地保存的分享连接或文件)\n- [清理本地保存的无效分享连接](#清理本地保存的无效分享连接)\n\n#### HTTP 服务\n\n- [开启 HTTP 服务](#开启-HTTP-服务)\n\n## 安装\n\n需要 Python 版本大于或等于 3.8\n\n```\npip3 install Cython\npip3 install AliPCS-Py\n```\n\n### Windows 依赖\n\n在 Windows 上，AliPCS-Py 依赖 [Microsoft C++ Build Tools](https://visualstudio.microsoft.com/visual-cpp-build-tools/)。\n\n在安装 AliPCS-Py 前，请先安装 [Microsoft C++ Build Tools](https://visualstudio.microsoft.com/visual-cpp-build-tools/)，再在其中勾选 `C++ 生成工具` 并安装。完成后即可安装 AliPCS-Py。\n\n## 更新\n\n```\npip3 install AliPCS-Py --upgrade\n```\n\n## API\n\nAliPCS-Py 的阿里云盘 API 只依赖 requests，方便用户开发自己的运用。\n\n```python\nfrom alipcs_py.alipcs import AliPCSApi\n\napi = AliPCSApi(refresh_token)\n```\n\n## 用法\n\n```\nAliPCS-Py --help\n```\n\n## 命令别名\n\n可以用下面的命令别名代替原来的命令名。\n\n| 别名 | 原名         |\n| ---- | ------------ |\n| w    | who          |\n| uu   | updateuser   |\n| su   | su           |\n| ul   | userlist     |\n| ua   | useradd      |\n| ep   | encryptpwd   |\n| ud   | userdel      |\n| l    | ls           |\n| f    | search       |\n| md   | mkdir        |\n| mv   | move         |\n| rn   | rename       |\n| cp   | copy         |\n| rm   | remove       |\n| d    | download     |\n| p    | play         |\n| u    | upload       |\n| sn   | sync         |\n| S    | share        |\n| sl   | shared       |\n| cs   | cancelshared |\n| s    | save         |\n| sv   | server       |\n\n## 对多个帐号进行相同操作\n\nAliPCS-Py 支持对多个帐号进行相同操作。比如，用相同关键字搜索多个帐号，上传相同的文件/目录到多个帐号，等等。\n\n使用者只需用 `--users` 选项来指定要操作的帐号名即可。\n\n`--users` 接受一个参数，这个参数是用“,”连接的要进行操作帐号名的部分字符。假设我们现在有 3 个帐号，帐号名分别是 `Tom`，`Peter`，`Joy`。\n现在我要同时对`Tom`和`Joy`进行关键字搜索。我们可以用下面的命令进行：\n\n```\nAliPCS-Py --users \'Tom,Joy\' search \'keyword\' / -R\n```\n\n或者给出帐号名的部分片段：\n\n```\nAliPCS-Py --users \'om,oy\' search \'keyword\' / -R\n```\n\n更简单可以用：\n\n```\n# Tom, Joy 都包含字符 "o"\nAliPCS-Py --users \'o\' search \'keyword\' / -R\n```\n\n如果要对所有帐号进行操作用 `--users \'\'`。\n\n如果不使用 `--users` 选项，默认只对当前帐号进行操作。\n\n以下命令支持对多个帐号进行操作：\n\n- pwd\n- ls\n- search\n- cat\n- mkdir\n- move\n- rename\n- copy\n- remove\n- download\n- play\n- upload\n- sync\n- share\n- shared\n- cancelshared\n- save\n- server\n\n**注意**: `--users` 一定要跟在 `AliPCS-Py` 后，命令前。\n\n## 添加用户\n\n**从 2023-02-14 开始，阿里云盘官方限制了 web 端 api 的调用。从 web 端 api 获取到的下载连接是限速的。但如果调用[阿里云盘开放平台](https://survey.alibaba.com/apps/zhiliao/I9Dd1Nl89)的 api 获取到的下载连接是不限速的。**\n\nAliPCS-Py (>= v0.6.0) 支持调用阿里云盘开放平台 api。但是由于一直没有拿到内测，没法提供默认登录操作。需要用户自己找其他应用提供的登录方式登录。\n\n### 使用 web `refresh_token` 和 第三方认证地址 登录\n\n第三方认证地址提供阿里云盘开放平台的认证服务。由于一直没有拿到内测，本项目目前没法提供。需要使用者自行寻找。\n\n交互添加：\n\n```\nAliPCS-Py useradd\n```\n\n或者直接添加：\n\n```\nAliPCS-Py useradd --web-refresh-token "..." --client-server "..."\n# 其他选项留空\n```\n\n之后用阿里云盘 APP 扫码登录。\n\n### 使用 web `refresh_token` 和 阿里云盘开放平台认证凭证 登录\n\n如果使用者拿到了阿里云盘开放平台认证，会获得 `client-id` 和 `client-secret`。使用这两个值可以直接登录。\n\n交互添加：\n\n```\nAliPCS-Py useradd\n```\n\n或者直接添加：\n\n```\nAliPCS-Py useradd --web-refresh-token "..." --client-id "..." --client-secret "..."\n# 其他选项留空\n```\n\n之后用阿里云盘 APP 扫码登录。\n\n### 使用 web `refresh_token` 登录\n\n使用者需要在 https://www.aliyundrive.com/drive/ 登录后获取 `refresh_token` 值，并用命令 `useradd` 为 AliPCS-Py 添加一个用户。`useradd` 其他参数留空就好。\n\n使用者可以用下面的方式获取用户的 `refresh_token` 值。\n\n1. 登录 https://www.aliyundrive.com/drive/\n2. 打开浏览器的开发者工具(如 Chrome DevTools)。\n3. 然后选择开发者工具的 Console 面板。输入 `JSON.parse(localStorage.token).refresh_token`，再回车，获取 `refresh_token`。\n\n![refresh_token](./imgs/refresh_token.png)\n\n现在找到了 `refresh_token` 值，我们可以用下面的命令添加一个用户。\n\n交互添加：\n\n```\nAliPCS-Py useradd\n```\n\n或者直接添加：\n\n```\nAliPCS-Py useradd --web-refresh-token "..."\n```\n\nAliPCS-Py 支持多用户，你只需一直用 `useradd` 来添加用户即可。\n\n**注意：如果只用 `--web-refresh-token` 登录，下载文件时，服务器端会限速。**\n\n## 显示当前用户的信息\n\n```\nAliPCS-Py who\n```\n\n或者：\n\n```\nAliPCS-Py who user_id\n```\n\n指明显示用户 id 为 `user_id` 的用户信息。\n\n### 选项\n\n| Option                       | Description                |\n| ---------------------------- | -------------------------- |\n| -K, --show-encrypt-password  | 显示加密密码               |\n| --account-name TEXT          | 账号名 [默认为 user id]    |\n| --web-refresh-token TEXT     | 用户 web_refresh_token     |\n| --openapi-refresh-token TEXT | 用户 openapi_refresh_token |\n| --client-id TEXT             | openapi client id          |\n| --client-secret TEXT         | openapi client secret      |\n| --client-server TEXT         | openapi client server      |\n\n## 更新用户信息\n\n默认更新当前用户信息。\n\n```\nAliPCS-Py updateuser\n```\n\n也可指定多个 `user_id`\n\n```\nAliPCS-Py updateuser user_id\n```\n\n## 显示所有用户\n\n```\nAliPCS-Py userlist\n```\n\n## 切换当前用户\n\n```\nAliPCS-Py su\n```\n\n或者指定用户列表中用户所在的位置：\n\n```\nAliPCS-Py su 2\n```\n\n## 删除一个用户\n\n```\nAliPCS-Py userdel\n```\n\n## 设置文件加密密码\n\nAliPCS-Py 支持“无感的”文件加密。\n\nAliPCS-Py 可以加密上传文件，在下载的时候自动解密，让使用者感觉不到加密解密的过程。\n\n如果使用者需要将保密文件上传至阿里云盘保存，可以使用这个方法。即使帐号被盗，攻击者也无法还原文件内容。\n\nAliPCS-Py 支持以下加密方法：\n\n- **Simple** 一种简单的加密算法。根据密钥生成一个字节对照表来加密解密文件。\n  速度快，但**不安全**，不建议加密重要文件。\n  因为这种算法加解密不需要知道上下文信息，所以，下载时支持分段下载，如果是媒体文件则支持拖动播放。\n  推荐用于加密不重要的媒体文件。\n- **ChaCha20** 工业级加密算法，速度快，推荐用于加密重要文件。不支持分段下载。\n- **AES256CBC** 工业级加密算法，推荐用于加密重要文件。不支持分段下载。\n\n**注意**：用命令 `encryptpwd` 设置的密码**只是为当前用户**的。\n\n为当前用户设置加密密码:\n\n交互添加：\n\n```\nAliPCS-Py encryptpwd\n```\n\n或者直接添加：\n\n```\nAliPCS-Py encryptpwd --encrypt-password \'my-encrypt-password\'\n```\n\n上传并加密文件：\n\n上传和同步文件时只需要指定加密算法就可。如果不指定就不加密。\n\n```\n# 默认使用上面设置的 `encrypt-password`\nAliPCS-Py upload some-file.mp4 some-dir/ /to/here --encrypt-type AES256CBC\n```\n\n下载并用上面设置的 `encrypt-password` 自动解密文件：\n\n```\nAliPCS-Py download /to/here/some-file.mp4 /to/here/some-dir/\n```\n\n也可以使用临时的 `encrypt-password`：\n\n```\nAliPCS-Py upload some-file.mp4 some-dir/ /to/here --encrypt-type Simple --encrypt-password \'onlyyou\'\n```\n\n但在使用临时的 `encrypt-password` 后，`cat`、下载和播放这些文件时需要指定 `encrypt-password`，但不需要指定加密算法，程序会自动检查加密算法：\n\n```\n# 下载\nAliPCS-Py download /to/here/some-file.mp4 /to/here/some-dir/  --encrypt-password \'onlyyou\'\n\n# 开启本地服务并播放\nAliPCS-Py play /to/here/some-file.mp4 --encrypt-password \'onlyyou\' --use-local-server\n```\n\n显示当前用户的密钥：\n\n```\nAliPCS-Py who --show-encrypt-password\n```\n\nAliPCS-Py 下载时默认会解密文件，如果想要下载但不解密文件，需要加 `--no-decrypt`\n\n```\nAliPCS-Py download some-file --no-decrypt\n```\n\n## 文件操作\n\nAliPCS-Py 操作网盘中的文件可以使用文件的绝对路径或相对路径（相对与当前目录 pwd）。\n\n每一个用户都有自己的当前工作目录（pwd），默认为 `/` 根目录。\n\n使用者可以用 `cd` 命令来切换当前的工作目录（pwd）。\n\n下面所有涉及网盘路径的命令，其中如果网盘路径用的是相对路径，那么是相对于当前工作目录（pwd）的。\n如果是网盘路径用的是绝对路径，那么就是这个绝对路径。\n\n## 显示当前工作目录\n\n```\nAliPCS-Py pwd\n```\n\n## 切换当前工作目录\n\n切换到绝对路径：\n\n```\nAliPCS-Py cd /to/some/path\n```\n\n切换到相对路径：\n\n```\n# 切换到 (pwd)/../path\nAliPCS-Py cd ../path\n```\n\n## 列出网盘路径下的文件\n\n使用文件路径：\n\n```\nAliPCS-Py ls [OPTIONS] [REMOTEPATHS]...\n\nAliPCS-Py ls /absolute/path\n\n# or\nAliPCS-Py ls relative/path\n```\n\n使用文件 ID：\n\n```\nAliPCS-Py ls -i file_id1 -i file_id2 -i ...\n```\n\n### 选项\n\n| Option                     | Description                                           |\n| -------------------------- | ----------------------------------------------------- |\n| -i, --file-id TEXT         | 文件 ID                                               |\n| --share-id, --si TEXT      | 列出这个分享 ID 下的文件                              |\n| --share-url, --su TEXT     | 列出这个分享 url 下的文件                             |\n| -p, --password TEXT        | 分享链接密码，如果没有不用设置                        |\n| -r, --desc                 | 逆序排列文件                                          |\n| -n, --name                 | 依名字排序                                            |\n| -t, --time                 | 依时间排序                                            |\n| -s, --size                 | 依文件大小排序                                        |\n| -R, --recursive            | 递归列出文件                                          |\n| -I, --include TEXT         | 筛选包含这个字符串的文件                              |\n| --include-regex, --IR TEXT | 筛选包含这个正则表达式的文件                          |\n| -E, --exclude TEXT         | 筛选 **不** 包含这个字符串的文件                      |\n| --exclude-regex, --ER TEXT | 筛选 **不** 包含这个正则表达式的文件                  |\n| -f, --is-file              | 筛选 **非** 目录文件                                  |\n| -d, --is-dir               | 筛选目录文件                                          |\n| --no-highlight, --NH       | 取消匹配高亮                                          |\n| -S, --show-size            | 显示文件大小                                          |\n| -D, --show-date            | 显示文件创建时间                                      |\n| --show-file-id, --ID       | 显示文件 ID                                           |\n| -M, --show-hash            | 显示文件 sha1                                         |\n| -A, --show-absolute-path   | 显示文件绝对路径                                      |\n| --show-dl-link, --DL       | 显示文件下载连接                                      |\n| --csv                      | 用 csv 格式显示，单行显示，推荐和 --DL 或 --HL 一起用 |\n| --only-dl-link, --ODL      | 只显示文件下载连接                                    |\n\n## 搜索文件\n\n搜索包含 `keyword` 的文件\n\n```\nAliPCS-Py search [OPTIONS] KEYWORD [REMOTEDIR]\n\n# 在当前工作目录中搜索\nAliPCS-Py search keyword\n\n# or\nAliPCS-Py search keyword /absolute/path\n\n# or\nAliPCS-Py search keyword relative/path\n```\n\n### 选项\n\n| Option                     | Description                          |\n| -------------------------- | ------------------------------------ |\n| -R, --recursive            | 递归搜索文件                         |\n| -I, --include TEXT         | 筛选包含这个字符串的文件             |\n| --include-regex, --IR TEXT | 筛选包含这个正则表达式的文件         |\n| -E, --exclude TEXT         | 筛选 **不** 包含这个字符串的文件     |\n| --exclude-regex, --ER TEXT | 筛选 **不** 包含这个正则表达式的文件 |\n| -f, --is-file              | 筛选 **非** 目录文件                 |\n| -d, --is-dir               | 筛选目录文件                         |\n| --no-highlight, --NH       | 取消匹配高亮                         |\n| -S, --show-size            | 显示文件大小                         |\n| -D, --show-date            | 显示文件创建时间                     |\n| -M, --show-hash            | 显示文件 sha1                        |\n| --csv                      | 用 csv 格式显示                      |\n\n## 显示文件内容\n\n```\nAliPCS-Py cat [OPTIONS] REMOTEPATH\n```\n\n### 选项\n\n| Option                        | Description                  |\n| ----------------------------- | ---------------------------- |\n| -e, --encoding TEXT           | 文件编码，默认自动解码       |\n| --no-decrypt, --ND            | 不解密                       |\n| --encrypt-password, --ep TEXT | 加密密码，默认使用用户设置的 |\n\n## 创建目录\n\n```\nAliPCS-Py mkdir [OPTIONS] [REMOTEDIRS]...\n```\n\n### 选项\n\n| Option     | Description |\n| ---------- | ----------- |\n| -S, --show | 显示目录    |\n\n## 移动文件\n\n移动一些文件到一个目录中。\n\n```\nAliPCS-Py move [OPTIONS] [REMOTEPATHS]... REMOTEDIR\n```\n\n### 选项\n\n| Option     | Description |\n| ---------- | ----------- |\n| -S, --show | 显示结果    |\n\n## 文件重命名\n\n```\nAliPCS-Py rename [OPTIONS] REMOTEPATH NEW_NAME\n```\n\ne.g.\n\n重命名 `/path/to/far` to `/path/to/foo`\n\n```\nAliPCS-Py rename /path/to/far foo\n```\n\n### 选项\n\n| Option     | Description |\n| ---------- | ----------- |\n| -S, --show | 显示结果    |\n\n## 拷贝文件\n\n拷贝一些文件到一个目录中。\n\n```\nAliPCS-Py move [OPTIONS] [REMOTEPATHS]... REMOTEDIR\n```\n\n### 选项\n\n| Option     | Description |\n| ---------- | ----------- |\n| -S, --show | 显示结果    |\n\n## 删除文件\n\n```\nAliPCS-Py remove [OPTIONS] [REMOTEPATHS]...\n\n# 指定 路径\nAliPCS-Py remove /some/path\n# 指定 file-id\nAliPCS-Py remove --file-id ...\n```\n\n### 选项\n\n| Option        | Description  |\n| ------------- | ------------ |\n| -i, --file-id | TEXT 文件 ID |\n\n## 下载文件或目录\n\n> 在使用了阿里云盘开放平台 api 时，如果下载他人分享的文件，文件会先保存到 `/__alipcs_py_temp__`，在从其中下载。\n> 下载结束后，会删除 `__alipcs_py_temp__` 中下载的文件。\n\n使用文件路径：\n\n```\nAliPCS-Py download [OPTIONS] [REMOTEPATHS]...\n```\n\n使用文件 ID：\n\n```\nAliPCS-Py download -i file_id1 -i file_id2 -i ...\n```\n\n### 选项\n\n| Option                                                 | Description                                                                                                                                                                                                                                                                                                                                                                                                                                                    |\n| ------------------------------------------------------ | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |\n| -i, --file-id TEXT                                     | 文件 ID                                                                                                                                                                                                                                                                                                                                                                                                                                                        |\n| --share-id, --si TEXT                                  | 下载这个分享 ID 下的文件                                                                                                                                                                                                                                                                                                                                                                                                                                       |\n| --share-url, --su TEXT                                 | 下载这个分享 url 下的文件                                                                                                                                                                                                                                                                                                                                                                                                                                      |\n| -p, --password TEXT                                    | 分享链接密码，如果没有不用设置                                                                                                                                                                                                                                                                                                                                                                                                                                 |\n| -o, --outdir TEXT                                      | 指定下载本地目录，默认为当前目录                                                                                                                                                                                                                                                                                                                                                                                                                               |\n| -R, --recursive                                        | 递归下载                                                                                                                                                                                                                                                                                                                                                                                                                                                       |\n| -f, --from-index INTEGER                               | 从所有目录中的第几个文件开始下载，默认为 0（第一个）                                                                                                                                                                                                                                                                                                                                                                                                           |\n| -I, --include TEXT                                     | 筛选包含这个字符串的文件                                                                                                                                                                                                                                                                                                                                                                                                                                       |\n| --include-regex, --IR TEXT                             | 筛选包含这个正则表达式的文件                                                                                                                                                                                                                                                                                                                                                                                                                                   |\n| -E, --exclude TEXT                                     | 筛选 不 包含这个字符串的文件                                                                                                                                                                                                                                                                                                                                                                                                                                   |\n| --exclude-regex, --ER TEXT                             | 筛选 不 包含这个正则表达式的文件                                                                                                                                                                                                                                                                                                                                                                                                                               |\n| -s, --concurrency INTEGER                              | 下载同步链接数，默认为 5。建议小于 10。                                                                                                                                                                                                                                                                                                                                                                                                                        |\n| -k, --chunk-size TEXT                                  | 同步链接分块大小，默认为 50MB                                                                                                                                                                                                                                                                                                                                                                                                                                  |\n| -q, --quiet                                            | 取消第三方下载应用输出                                                                                                                                                                                                                                                                                                                                                                                                                                         |\n| --out-cmd, --OC                                        | 输出第三方下载应用命令                                                                                                                                                                                                                                                                                                                                                                                                                                         |\n| -d, --downloader [ me \\| aget_py \\| aget_rs \\| aria2 ] | 指定下载应用<br> <br> 默认为 me (AliPCS-Py 自己的下载器，支持断续下载)<br> me 使用多文件并发下载。<br> <br> 除 me 外，其他下载器，不使用多文件并发下载，使用一个文件多链接下载。<br> 如果需要下载多个小文件推荐使用 me，如果需要下载少量大文件推荐使用其他下载器。<br> <br> aget_py (https://github.com/PeterDing/aget) 默认安装<br> aget_rs (下载 https://github.com/PeterDing/aget-rs/releases)<br> aria2 (下载 https://github.com/aria2/aria2/releases)<br> |\n| --encrypt-password, --ep TEXT                          | 加密密码，默认使用用户设置的                                                                                                                                                                                                                                                                                                                                                                                                                                   |\n\n## 播放媒体文件\n\n> 在使用了阿里云盘开放平台 api 时，如果播放他人分享的文件，文件会先保存到 `/__alipcs_py_temp__`，在从其中播放。\n> 播放结束后，会删除 `__alipcs_py_temp__` 中播放的文件。\n\n使用文件路径：\n\n```\nAliPCS-Py play [OPTIONS] [REMOTEPATHS]...\n```\n\n使用文件 ID：\n\n**注意：目前，使用 `--share-id` 或 `--file-id` 时，无法使用 `--use-local-server`**\n\n```\nAliPCS-Py play -i file_id1 -i file_id2 -i ...\n```\n\n`play` 命令默认播放带有媒体后缀的文件，如 `abc.mp4`, `abc.mp3`。如果需要播放的媒体文件没有用常规的媒体文件后缀，则需要加选项 `--ignore-ext`。\n\n### 选项\n\n| Option                        | Description                                          |\n| ----------------------------- | ---------------------------------------------------- |\n| -i, --file-id TEXT            | 文件 ID                                              |\n| --share-id, --si TEXT         | 播放这个分享 ID 下的文件                             |\n| --share-url, --su TEXT        | 播放这个分享 url 下的文件                            |\n| -p, --password TEXT           | 链接密码，如果没有不用设置                           |\n| -R, --recursive               | 递归播放                                             |\n| -f, --from-index INTEGER      | 从所有目录中的第几个文件开始播放，默认为 0（第一个） |\n| -I, --include TEXT            | 筛选包含这个字符串的文件                             |\n| --include-regex, --IR TEXT    | 筛选包含这个正则表达式的文件                         |\n| -E, --exclude TEXT            | 筛选 不 包含这个字符串的文件                         |\n| --exclude-regex, --ER TEXT    | 筛选 不 包含这个正则表达式的文件                     |\n| --player-params, --PP TEXT    | 第三方播放器参数                                     |\n| -q, --quiet                   | 取消第三方播放器输出                                 |\n| --shuffle, --sf               | 随机播放                                             |\n| --ignore-ext, --IE            | 不用文件名后缀名来判断媒体文件                       |\n| --out-cmd, --OC               | 输出第三方播放器命令                                 |\n| --pl, --player [mpv]          | 指定第三方播放器<br><br>默认为 mpv (https://mpv.io)  |\n| -s, --use-local-server        | 使用本地服务器播放。                                 |\n| --encrypt-password, --ep TEXT | 加密密码，默认使用用户设置的                         |\n\n## 上传文件\n\n上传一些本地文件或目录到网盘目录。\n\nAliPCS-Py 首先会尝试秒传。如果秒传失败，会使用分片上传上传文件。\n\n上传过程中，按 “p” 可以暂停或继续上传。\n\n```\nAliPCS-Py upload [OPTIONS] [LOCALPATHS]... REMOTEDIR\n```\n\n指定上传方式：\n\n`--upload-type Many`: 同时上传多个文件。\n\n适合大多数文件长度小于 100M 以下的情况。\n\n```\nAliPCS-Py upload --upload-type Many [OPTIONS] [LOCALPATHS]... REMOTEDIR\n```\n\n<del>`--upload-type One`: 一次只上传一个文件，但同时上传文件的多个分片。</del>\n\n<del>适合大多数文件长度大于 1G 以上的情况。</del>\n\n**阿里网盘不支持单文件并发上传。`upload --upload-type One` 失效**\n\n```\nAliPCS-Py upload --upload-type One [OPTIONS] [LOCALPATHS]... REMOTEDIR\n```\n\n指定同时上传连接数量:\n\n`--max-workers` 默认为 CPU 核数。\n\n```\nAliPCS-Py upload --max-workers 4 [OPTIONS] [LOCALPATHS]... REMOTEDIR\n```\n\n如果上传本地目录 `localdir` 到远端目录 `remotedir`，AliPCS-Py 是将 `localdir` 这个目录上传到远端目录 `remotedir` 下。\n\n比如，`localdir` 下有 2 个文件 `a`，`b` 和一个下级目录 `sub/`，如果运行 `AliPCS-Py upload localdir remotedir`，结果是远端目录 `remotedir` 下增加了 1 个下级目录和它的所有文件 `localdir/a`，`localdir/b` 和一个下级目录 `localdir/sub/`。\n\n如果要将 `localdir` 下的所有文件（包括下级目录）上传到远端目录 `remotedir`，用 `AliPCS-Py upload localdir/* remotedir`\n\n### 选项\n\n| Option                                                     | Description                             |\n| ---------------------------------------------------------- | --------------------------------------- |\n| -t, --upload-type [One \\| Many]                            | 上传方式，Many (默认): 同时上传多个文件 |\n| --encrypt-password, --ep TEXT                              | 加密密码，默认使用用户设置的            |\n| -e, --encrypt-type [No \\| Simple \\| ChaCha20 \\| AES256CBC] | 文件加密方法，默认为 No 不加密          |\n| -w, --max-workers INTEGER                                  | 同时上传文件连接数量，默认为 CPU 核数   |\n| --no-ignore-existing, --NI                                 | 上传已经存在的文件                      |\n| --no-show-progress, --NP                                   | 不显示上传进度                          |\n\n## 同步本地目录到远端\n\n同步本地目录到远端。\n\n如果本地文件最后修改时间或大小和远端不同则上传文件。对于本地不存在的文件但远端存在则删除远端文件。\n\n```\nAliPCS-Py sync [OPTIONS] LOCALDIR REMOTEDIR\n```\n\n### 选项\n\n| Option                                                     | Description                    |\n| ---------------------------------------------------------- | ------------------------------ |\n| --encrypt-password, --ep TEXT                              | 加密密码，默认使用用户设置的   |\n| -e, --encrypt-type [No \\| Simple \\| ChaCha20 \\| AES256CBC] | 文件加密方法，默认为 No 不加密 |\n| -w, --max-workers INTEGER                                  | 同时上传文件数                 |\n| --no-show-progress, --NP                                   | 不显示上传进度                 |\n\n## 关于秒传连接\n\n**阿里云盘已经不能实现用秒传连接上传。**\n\n## 分享文件\n\n```\nAliPCS-Py share [OPTIONS] [REMOTEPATHS]...\n```\n\n### 选项\n\n| Option                      | Description                      |\n| --------------------------- | -------------------------------- |\n| -p, --password TEXT         | 设置秘密，4 个字符。默认没有秘密 |\n| --period-time, --pt INTEGER | 设置分享有效期，单位为天         |\n\n## 列出分享链接\n\n```\nAliPCS-Py shared\n```\n\n### 选项\n\n| Option         | Description                                  |\n| -------------- | -------------------------------------------- |\n| -A, --show-all | 显示所有分享的链接，默认只显示有效的分享链接 |\n\n## 取消分享链接\n\n```\nAliPCS-Py cancelshared [OPTIONS] [SHARE_IDS]...\n```\n\n## 列出其他用户分享链接中的文件\n\n给 `ls` 命令加参数，我们可以列出其他用户分享链接中的文件。\n\n**注意: 这里 `remotepaths` 只能是绝对路径。**\n\n如果有分享密码，加上 `--password PASSWORD`。\n\n- 使用分享连接\n\n  ```\n  AliPCS-Py ls --share-url SHARE_URL\n\n  # e.g.\n\n  # 列出这个分享url的根目录\n  AliPCS-Py ls --share-url https://www.aliyundrive.com/s/DaNNsdvi9bi\n\n  # 递归列出这个分享url的文件\n  AliPCS-Py ls --share-url https://www.aliyundrive.com/s/DaNNsdvi9bi -R\n\n  # 列出这个分享url的指定目录\n  AliPCS-Py ls --share-url https://www.aliyundrive.com/s/DaNNsdvi9bi/folder/613397974b634251e0554d7cb56df3e46d473239\n  ```\n\n- 使用分享 ID\n\n  分享 ID 是 https://www.aliyundrive.com/s/DaNNsdvi9bi 中的 `DaNNsdvi9bi`\n\n  ```\n  AliPCS-Py ls /path --share-id SHARE_ID\n\n  # e.g.\n\n  # 列出这个分享ID的根目录\n  AliPCS-Py ls / --share-id DaNNsdvi9bi\n\n  # 列出这个分享ID下，文件名为 "613397974b634251e0554d7cb56df3e46d473239" 的文件\n  AliPCS-Py ls --file-id 613397974b634251e0554d7cb56df3e46d473239 --share-id DaNNsdvi9bi\n  ```\n\n### 选项\n\n见 `ls` 命令。\n\n## 下载他人分享的文件\n\n使用 `--share-id` 或 `--share-url` 选项，`download` 命令可以直接下载他人分享的文件。\n\n**注意: 这里必须指定下载绝对路径或 file id**\n\n```\nAliPCS-Py download /path --share-url SHARED_URL\n\n# or\n\nAliPCS-Py download /path --share-id SHARED_URL\n\n# or\n\nAliPCS-Py download --file-id FILE_ID --share-id SHARED_URL\n```\n\n- 使用分享连接\n\n  ```\n  # 下载这个分享url下的根目录中的文件\n  AliPCS-Py download / --share-url https://www.aliyundrive.com/s/DaNNsdvi9bi\n\n  # 递归下载这个分享url下的所有的文件\n  AliPCS-Py download / --share-url https://www.aliyundrive.com/s/DaNNsdvi9bi -R\n\n  # 下载这个分享url的指定目录\n  AliPCS-Py download --share-url https://www.aliyundrive.com/s/DaNNsdvi9bi/folder/613397974b634251e0554d7cb56df3e46d473239\n  ```\n\n- 使用分享 ID\n\n  ```\n  # 下载这个分享url下的根目录中的文件\n  AliPCS-Py download / --share-id DaNNsdvi9bi\n\n  # 递归下载这个分享url下的所有的文件\n  AliPCS-Py download / --share-id DaNNsdvi9bi -R\n\n  # 下载这个分享ID下，文件名为 "613397974b634251e0554d7cb56df3e46d473239" 的文件\n  AliPCS-Py download --file-id 613397974b634251e0554d7cb56df3e46d473239 --share-id DaNNsdvi9bi\n  ```\n\n### 选项\n\n见 `download` 命令。\n\n## 播放他人分享的文件\n\n使用 `--share-id` 或 `--share-url` 选项，`play` 命令可以直接播放他人分享的媒体文件。\n\n**注意: 这里必须指定下载绝对路径或 file id**\n\n```\nAliPCS-Py play /path --share-url SHARED_URL\n\n# or\n\nAliPCS-Py play /path --share-id SHARED_URL\n\n# or\n\nAliPCS-Py play --file-id FILE_ID --share-id SHARED_URL\n```\n\n- 使用分享连接\n\n  ```\n  # 播放这个分享url下的根目录中的文件\n  AliPCS-Py play / --share-url https://www.aliyundrive.com/s/DaNNsdvi9bi\n\n  # 递归播放这个分享url下的所有的文件\n  AliPCS-Py play / --share-url https://www.aliyundrive.com/s/DaNNsdvi9bi -R\n\n  # 播放这个分享url的指定目录\n  AliPCS-Py play --share-url https://www.aliyundrive.com/s/DaNNsdvi9bi/folder/613397974b634251e0554d7cb56df3e46d473239\n  ```\n\n- 使用分享 ID\n\n  ```\n  # 播放这个分享url下的根目录中的文件\n  AliPCS-Py play --share-id DaNNsdvi9bi\n\n  # 递归播放这个分享url下的所有的文件\n  AliPCS-Py play --share-id DaNNsdvi9bi -R\n\n  # 播放这个分享ID下，文件名为 "613397974b634251e0554d7cb56df3e46d473239" 的文件\n  AliPCS-Py play --file-id 613397974b634251e0554d7cb56df3e46d473239 --share-id DaNNsdvi9bi\n  ```\n\n### 选项\n\n见 `play` 命令。\n\n## 保存其他用户分享的链接\n\n保存其他用户分享的链接到远端目录。\n\n```\nAliPCS-Py save [OPTIONS] SHARE_URL_OR_ID REMOTEDIR\n```\n\n指定 `--file-id` 可以保存指定的文件。\n\n### 选项\n\n| Option              | Description                    |\n| ------------------- | ------------------------------ |\n| -i, --file-id TEXT  | 文件 ID                        |\n| -p, --password TEXT | 分享链接密码，如果没有不用设置 |\n\n## 本地保存分享连接\n\n可以将他人分享了连接保存至本地，而不需要保存在网盘。这只作为一个记录。在需要是提供查看搜索功能。\n\n使用这个功能，需要使用者在本地配置文件(`~/.alipcs-py/config.toml`)中配置:\n\n```toml\n[share]\nstore = true\n```\n\n这个功能开启后，所有与他人分享连接的操作，都会将连接和其中访问过的文件信息保存在本地文件 `~/.alipcs-py/shared-store.sqlite3` 中。\n\n使用者可以用下面的命令来查看或搜索保存的分享连接。\n\n## 保存分享连接至本地\n\n```\nAliPCS-Py storesharedlinks [OPTIONS] [SHARE_URLS_OR_IDS]...\n```\n\n**注意**: 使用这个命令必须将配置文件 ~/.alipcs-py/config.toml 中的 [share] store 设为 true\n\n| Option              | Description                    |\n| ------------------- | ------------------------------ |\n| -p, --password TEXT | 分享链接密码，如果没有不用设置 |\n\n## 显示本地保存的分享连接\n\n```\nAliPCS-Py listsharedlinks\n```\n\n**注意**: 使用这个命令必须将配置文件 ~/.alipcs-py/config.toml 中的 [share] store 设为 true\n\n## 显示本地保存的分享文件\n\n```\nAliPCS-Py listsharedfiles [OPTIONS]\n```\n\n**注意**: 使用这个命令必须将配置文件 ~/.alipcs-py/config.toml 中的 [share] store 设为 true\n\n| Option                | Description                |\n| --------------------- | -------------------------- |\n| --share-id, --si TEXT | 指定显示 share id 下的文件 |\n\n## 查找本地保存的分享连接\n\n```\nAliPCS-Py findsharedlinks [KEYWORDS]...\n```\n\n**注意**: 使用这个命令必须将配置文件 ~/.alipcs-py/config.toml 中的 [share] store 设为 true\n\n## 查找本地保存的分享文件\n\n```\nAliPCS-Py findsharedfiles [KEYWORDS]...\n```\n\n**注意**: 使用这个命令必须将配置文件 ~/.alipcs-py/config.toml 中的 [share] store 设为 true\n\n| Option                | Description       |\n| --------------------- | ----------------- |\n| --share-id, --si TEXT | 要搜索的 share id |\n| -v, --verbose         | 显示细节          |\n\n## 查找本地保存的分享连接和文件\n\n```\nAliPCS-Py findshared [OPTIONS] [KEYWORDS]...\n```\n\n**注意**: 使用这个命令必须将配置文件 ~/.alipcs-py/config.toml 中的 [share] store 设为 true\n\n| Option        | Description |\n| ------------- | ----------- |\n| -v, --verbose | 显示细节    |\n\n## 删除本地保存的分享连接或文件\n\n```\nAliPCS-Py deletestoredshared [OPTIONS] [SHARE_IDS]...\n```\n\n**注意**: 使用这个命令必须将配置文件 ~/.alipcs-py/config.toml 中的 [share] store 设为 true\n\n| Option             | Description                                                |\n| ------------------ | ---------------------------------------------------------- |\n| -k, --keyword TEXT | 要删除文件名的关键字，如果为空则删除 share_id 下的所有文件 |\n\n## 清理本地保存的无效分享连接\n\n```\nAliPCS-Py cleanstore\n```\n\n**注意**: 使用这个命令必须将配置文件 ~/.alipcs-py/config.toml 中的 [share] store 设为 true\n\n## 开启 HTTP 服务\n\n在远端 `ROOT_DIR` 目录下开启 HTTP 服务。\n\n`ROOT_DIR` 默认为 `/`\n\n```\nAliPCS-Py AliPCS-Py server [OPTIONS] [ROOT_DIR]\n```\n\n如果需要设置认证，使用下面的选项设置用户名和密钥：\n\n```\nAliPCS-Py AliPCS-Py server [ROOT_DIR] --username \'foo\' --password \'bar\'\n```\n\n也可以指定服务路径：\n\n```\nAliPCS-Py AliPCS-Py server [ROOT_DIR] --path \'/my/pan\'\n\n# 访问 http://localhost:8000/my/pan/\n```\n\n### 选项\n\n| Option                        | Description                  |\n| ----------------------------- | ---------------------------- |\n| --path TEXT                   | 服务路径，默认为 “/”         |\n| -h, --host TEXT               | 监听 host                    |\n| -p, --port INTEGER            | 监听 port                    |\n| -w, --workers INTEGER         | 进程数                       |\n| --encrypt-password, --ep TEXT | 加密密码，默认使用用户设置的 |\n| --username TEXT               | HTTP Basic Auth 用户名       |\n| --password TEXT               | HTTP Basic Auth 密钥         |\n',
     'author': 'PeterDing',
     'author_email': 'dfhayst@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/PeterDing/AliPCS-Py',
```

### Comparing `alipcs_py-0.6.2/PKG-INFO` & `alipcs_py-0.6.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: alipcs-py
-Version: 0.6.2
+Name: AliPCS-Py
+Version: 0.6.3
 Summary: Ali Pcs Api and App
 Home-page: https://github.com/PeterDing/AliPCS-Py
 License: MIT
 Author: PeterDing
 Author-email: dfhayst@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Environment :: Console
@@ -14,20 +14,15 @@
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
 Requires-Dist: aget (>=0.2)
 Requires-Dist: chardet (>=5.2)
 Requires-Dist: click (>=8.1)
 Requires-Dist: cryptography (>=41.0)
 Requires-Dist: cython (>=3.0)
 Requires-Dist: ecdsa (>=0.18)
 Requires-Dist: fastapi (>=0.104)
```

