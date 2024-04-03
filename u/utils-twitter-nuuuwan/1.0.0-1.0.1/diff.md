# Comparing `tmp/utils_twitter-nuuuwan-1.0.0.tar.gz` & `tmp/utils_twitter-nuuuwan-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "utils_twitter-nuuuwan-1.0.0.tar", last modified: Wed Sep 27 02:27:24 2023, max compression
+gzip compressed data, was "utils_twitter-nuuuwan-1.0.1.tar", last modified: Wed Apr  3 16:21:24 2024, max compression
```

## Comparing `utils_twitter-nuuuwan-1.0.0.tar` & `utils_twitter-nuuuwan-1.0.1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-27 02:27:24.375156 utils_twitter-nuuuwan-1.0.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1075 2023-09-27 02:26:45.000000 utils_twitter-nuuuwan-1.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      569 2023-09-27 02:27:24.375156 utils_twitter-nuuuwan-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      198 2023-09-27 02:26:45.000000 utils_twitter-nuuuwan-1.0.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-09-27 02:27:24.375156 utils_twitter-nuuuwan-1.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      942 2023-09-27 02:26:45.000000 utils_twitter-nuuuwan-1.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-27 02:27:24.371156 utils_twitter-nuuuwan-1.0.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-27 02:27:24.371156 utils_twitter-nuuuwan-1.0.0/src/utils_twitter/
--rw-r--r--   0 runner    (1001) docker     (127)      259 2023-09-27 02:26:45.000000 utils_twitter-nuuuwan-1.0.0/src/utils_twitter/Tweet.py
--rw-r--r--   0 runner    (1001) docker     (127)      263 2023-09-27 02:26:45.000000 utils_twitter-nuuuwan-1.0.0/src/utils_twitter/Twitter.py
--rw-r--r--   0 runner    (1001) docker     (127)      967 2023-09-27 02:26:45.000000 utils_twitter-nuuuwan-1.0.0/src/utils_twitter/TwitterActionerMixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1495 2023-09-27 02:26:45.000000 utils_twitter-nuuuwan-1.0.0/src/utils_twitter/TwitterActionerMixinHelpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     1116 2023-09-27 02:26:45.000000 utils_twitter-nuuuwan-1.0.0/src/utils_twitter/TwitterBase.py
--rw-r--r--   0 runner    (1001) docker     (127)      966 2023-09-27 02:26:45.000000 utils_twitter-nuuuwan-1.0.0/src/utils_twitter/TwitterLoaderMixin.py
--rw-r--r--   0 runner    (1001) docker     (127)       82 2023-09-27 02:26:45.000000 utils_twitter-nuuuwan-1.0.0/src/utils_twitter/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-27 02:27:24.375156 utils_twitter-nuuuwan-1.0.0/src/utils_twitter_nuuuwan.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      569 2023-09-27 02:27:24.000000 utils_twitter-nuuuwan-1.0.0/src/utils_twitter_nuuuwan.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      622 2023-09-27 02:27:24.000000 utils_twitter-nuuuwan-1.0.0/src/utils_twitter_nuuuwan.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-09-27 02:27:24.000000 utils_twitter-nuuuwan-1.0.0/src/utils_twitter_nuuuwan.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       26 2023-09-27 02:27:24.000000 utils_twitter-nuuuwan-1.0.0/src/utils_twitter_nuuuwan.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2023-09-27 02:27:24.000000 utils_twitter-nuuuwan-1.0.0/src/utils_twitter_nuuuwan.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-27 02:27:24.375156 utils_twitter-nuuuwan-1.0.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      161 2023-09-27 02:26:45.000000 utils_twitter-nuuuwan-1.0.0/tests/test_tweet.py
--rw-r--r--   0 runner    (1001) docker     (127)     2112 2023-09-27 02:26:45.000000 utils_twitter-nuuuwan-1.0.0/tests/test_twitter_actioner_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1053 2023-09-27 02:26:45.000000 utils_twitter-nuuuwan-1.0.0/tests/test_twitter_actioner_mixin_helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 16:21:24.902727 utils_twitter-nuuuwan-1.0.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1075 2024-04-03 16:20:55.000000 utils_twitter-nuuuwan-1.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      569 2024-04-03 16:21:24.898727 utils_twitter-nuuuwan-1.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      288 2024-04-03 16:20:55.000000 utils_twitter-nuuuwan-1.0.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-03 16:21:24.902727 utils_twitter-nuuuwan-1.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      942 2024-04-03 16:20:55.000000 utils_twitter-nuuuwan-1.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 16:21:24.898727 utils_twitter-nuuuwan-1.0.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 16:21:24.898727 utils_twitter-nuuuwan-1.0.1/src/utils_twitter/
+-rw-r--r--   0 runner    (1001) docker     (127)      259 2024-04-03 16:20:55.000000 utils_twitter-nuuuwan-1.0.1/src/utils_twitter/Tweet.py
+-rw-r--r--   0 runner    (1001) docker     (127)      263 2024-04-03 16:20:55.000000 utils_twitter-nuuuwan-1.0.1/src/utils_twitter/Twitter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      970 2024-04-03 16:20:55.000000 utils_twitter-nuuuwan-1.0.1/src/utils_twitter/TwitterActionerMixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1736 2024-04-03 16:20:55.000000 utils_twitter-nuuuwan-1.0.1/src/utils_twitter/TwitterActionerMixinHelpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1116 2024-04-03 16:20:55.000000 utils_twitter-nuuuwan-1.0.1/src/utils_twitter/TwitterBase.py
+-rw-r--r--   0 runner    (1001) docker     (127)      966 2024-04-03 16:20:55.000000 utils_twitter-nuuuwan-1.0.1/src/utils_twitter/TwitterLoaderMixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      410 2024-04-03 16:20:55.000000 utils_twitter-nuuuwan-1.0.1/src/utils_twitter/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 16:21:24.898727 utils_twitter-nuuuwan-1.0.1/src/utils_twitter_nuuuwan.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      569 2024-04-03 16:21:24.000000 utils_twitter-nuuuwan-1.0.1/src/utils_twitter_nuuuwan.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      622 2024-04-03 16:21:24.000000 utils_twitter-nuuuwan-1.0.1/src/utils_twitter_nuuuwan.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 16:21:24.000000 utils_twitter-nuuuwan-1.0.1/src/utils_twitter_nuuuwan.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-03 16:21:24.000000 utils_twitter-nuuuwan-1.0.1/src/utils_twitter_nuuuwan.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-03 16:21:24.000000 utils_twitter-nuuuwan-1.0.1/src/utils_twitter_nuuuwan.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 16:21:24.898727 utils_twitter-nuuuwan-1.0.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      161 2024-04-03 16:20:55.000000 utils_twitter-nuuuwan-1.0.1/tests/test_tweet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2112 2024-04-03 16:20:55.000000 utils_twitter-nuuuwan-1.0.1/tests/test_twitter_actioner_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1022 2024-04-03 16:20:55.000000 utils_twitter-nuuuwan-1.0.1/tests/test_twitter_actioner_mixin_helpers.py
```

### Comparing `utils_twitter-nuuuwan-1.0.0/LICENSE` & `utils_twitter-nuuuwan-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `utils_twitter-nuuuwan-1.0.0/PKG-INFO` & `utils_twitter-nuuuwan-1.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: utils_twitter-nuuuwan
-Version: 1.0.0
+Version: 1.0.1
 Summary: Utilities for Twitter
 Home-page: https://github.com/nuuuwan/utils_twitter
 Author: Nuwan I. Senaratna
 Author-email: nuuuwan@gmail.com
 Project-URL: Bug Tracker, https://github.com/nuuuwan/utils_twitter/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `utils_twitter-nuuuwan-1.0.0/setup.py` & `utils_twitter-nuuuwan-1.0.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """Setup."""
 
 import setuptools
 
 DIST_NAME = 'utils_twitter'
-VERSION = "1.0.0"
+VERSION = "1.0.1"
 DESCRIPTION = 'Utilities for Twitter'
 
 setuptools.setup(
     name="%s-nuuuwan" % DIST_NAME,
     version=VERSION,
     author="Nuwan I. Senaratna",
     author_email="nuuuwan@gmail.com",
```

### Comparing `utils_twitter-nuuuwan-1.0.0/src/utils_twitter/TwitterActionerMixin.py` & `utils_twitter-nuuuwan-1.0.1/src/utils_twitter/TwitterActionerMixin.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 """Implements twitter."""
 
 
 import logging
 
 from utils_twitter.Tweet import Tweet
-from utils_twitter.TwitterActionerMixinHelpers import (
-    _update_profile_description, _update_status, _upload_media)
+from utils_twitter.TwitterActionerMixinHelpers import \
+    TwitterActionerMixinHelpers as helpers
 
 log = logging.getLogger(__name__)
 
 
 class TwitterActionerMixin:
     def send(self, tweet: Tweet):
-        media_ids = _upload_media(
+        media_ids = helpers._upload_media(
             self.api,
             tweet.image_file_path_list,
         )
-        return _update_status(
+        return helpers._update_status(
             self.api, tweet.text, media_ids, tweet.in_reply_to_status_id
         )
 
     def update_profile_description(self):
-        _update_profile_description(self.api)
+        helpers._update_profile_description(self.api)
 
     def update_profile_image(self, profile_image_file):
         log.debug(f'update_profile_image: {profile_image_file}')
         self.api.update_profile_image(profile_image_file)
 
     def update_banner_image(self, banner_image_file):
         log.debug(f'update_banner_image: {banner_image_file}')
```

### Comparing `utils_twitter-nuuuwan-1.0.0/src/utils_twitter/TwitterActionerMixinHelpers.py` & `utils_twitter-nuuuwan-1.0.1/src/utils_twitter/TwitterActionerMixinHelpers.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,50 +1,52 @@
 """Implements twitter."""
 
-from utils_base import TIMEZONE_OFFSET, Log, Time, TimeFormat
+from utils_base import Log, Time, TimeFormat, TimeZoneOffset
 
 log = Log('Twitter')
 
 
-def _update_status(api, tweet_text, media_ids, in_reply_to_status_id):
-    if len(media_ids) > 0:
-        if in_reply_to_status_id:
-            response = api.update_status(
-                tweet_text,
-                media_ids=media_ids,
-                in_reply_to_status_id=in_reply_to_status_id,
-            )
+class TwitterActionerMixinHelpers:
+    @staticmethod
+    def _update_status(api, tweet_text, media_ids, in_reply_to_status_id):
+        if len(media_ids) > 0:
+            if in_reply_to_status_id:
+                response = api.update_status(
+                    tweet_text,
+                    media_ids=media_ids,
+                    in_reply_to_status_id=in_reply_to_status_id,
+                )
+            else:
+                response = api.update_status(
+                    tweet_text,
+                    media_ids=media_ids,
+                )
         else:
-            response = api.update_status(
-                tweet_text,
-                media_ids=media_ids,
-            )
-    else:
-        if in_reply_to_status_id:
-            response = api.update_status(
-                tweet_text, in_reply_to_status_id=in_reply_to_status_id
+            if in_reply_to_status_id:
+                response = api.update_status(
+                    tweet_text, in_reply_to_status_id=in_reply_to_status_id
+                )
+            else:
+                response = api.update_status(tweet_text)
+        return response
+
+    @staticmethod
+    def _upload_media(api, image_files):
+        media_ids = []
+        for image_file in image_files:
+            media_id = api.media_upload(image_file).media_id
+            media_ids.append(media_id)
+            log.info(
+                f'Uploaded status image {image_file} to twitter as {media_id}',
             )
-        else:
-            response = api.update_status(tweet_text)
-    return response
+        return media_ids
 
-
-def _upload_media(api, image_files):
-    media_ids = []
-    for image_file in image_files:
-        media_id = api.media_upload(image_file).media_id
-        media_ids.append(media_id)
-        log.info(
-            f'Uploaded status image {image_file} to twitter as {media_id}',
+    @staticmethod
+    def _update_profile_description(api):
+        date_with_timezone = TimeFormat(
+            '%Y-%m-%d %H:%M:%S', TimeZoneOffset.LK
+        ).stringify(Time.now())
+        description = (
+            f'Automatically updated at {date_with_timezone} (#SriLanka Time)'
         )
-    return media_ids
-
-
-def _update_profile_description(api):
-    date_with_timezone = TimeFormat(
-        '%Y-%m-%d %H:%M:%S', TIMEZONE_OFFSET.LK
-    ).stringify(Time.now())
-    description = (
-        f'Automatically updated at {date_with_timezone} (#SriLanka Time)'
-    )
-    api.update_profile(description=description)
-    log.info(f'Updated profile description to: {description}')
+        api.update_profile(description=description)
+        log.info(f'Updated profile description to: {description}')
```

### Comparing `utils_twitter-nuuuwan-1.0.0/src/utils_twitter/TwitterBase.py` & `utils_twitter-nuuuwan-1.0.1/src/utils_twitter/TwitterBase.py`

 * *Files identical despite different names*

### Comparing `utils_twitter-nuuuwan-1.0.0/src/utils_twitter/TwitterLoaderMixin.py` & `utils_twitter-nuuuwan-1.0.1/src/utils_twitter/TwitterLoaderMixin.py`

 * *Files identical despite different names*

### Comparing `utils_twitter-nuuuwan-1.0.0/src/utils_twitter_nuuuwan.egg-info/PKG-INFO` & `utils_twitter-nuuuwan-1.0.1/src/utils_twitter_nuuuwan.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: utils-twitter-nuuuwan
-Version: 1.0.0
+Name: utils_twitter-nuuuwan
+Version: 1.0.1
 Summary: Utilities for Twitter
 Home-page: https://github.com/nuuuwan/utils_twitter
 Author: Nuwan I. Senaratna
 Author-email: nuuuwan@gmail.com
 Project-URL: Bug Tracker, https://github.com/nuuuwan/utils_twitter/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `utils_twitter-nuuuwan-1.0.0/src/utils_twitter_nuuuwan.egg-info/SOURCES.txt` & `utils_twitter-nuuuwan-1.0.1/src/utils_twitter_nuuuwan.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `utils_twitter-nuuuwan-1.0.0/tests/test_twitter_actioner_mixin.py` & `utils_twitter-nuuuwan-1.0.1/tests/test_twitter_actioner_mixin.py`

 * *Files identical despite different names*

