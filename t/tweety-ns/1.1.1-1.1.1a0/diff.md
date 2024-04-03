# Comparing `tmp/tweety-ns-1.1.1.tar.gz` & `tmp/tweety-ns-1.1.1a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tweety-ns-1.1.1.tar", last modified: Mon Apr  1 07:46:03 2024, max compression
+gzip compressed data, was "tweety-ns-1.1.1a0.tar", last modified: Wed Apr  3 11:13:57 2024, max compression
```

## Comparing `tweety-ns-1.1.1.tar` & `tweety-ns-1.1.1a0.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxrwxr-x   0 kharltayyab  (1000) kharltayyab  (1000)        0 2024-04-01 07:46:03.635728 tweety-ns-1.1.1/
--rw-r--r--   0 kharltayyab  (1000) kharltayyab  (1000)     1891 2024-04-01 07:46:03.635728 tweety-ns-1.1.1/PKG-INFO
--rwxr-xr-x   0 kharltayyab  (1000) kharltayyab  (1000)     1142 2023-12-31 07:12:35.000000 tweety-ns-1.1.1/README.md
--rwxr-xr-x   0 kharltayyab  (1000) kharltayyab  (1000)      108 2021-11-15 09:32:36.000000 tweety-ns-1.1.1/pyproject.toml
--rwxr-xr-x   0 kharltayyab  (1000) kharltayyab  (1000)      671 2024-04-01 07:46:03.635728 tweety-ns-1.1.1/setup.cfg
--rwxr-xr-x   0 kharltayyab  (1000) kharltayyab  (1000)      785 2024-04-01 07:44:57.000000 tweety-ns-1.1.1/setup.py
-drwxrwxr-x   0 kharltayyab  (1000) kharltayyab  (1000)        0 2024-04-01 07:46:03.627728 tweety-ns-1.1.1/src/
-drwxrwxr-x   0 kharltayyab  (1000) kharltayyab  (1000)        0 2024-04-01 07:46:03.627728 tweety-ns-1.1.1/src/tweety/
--rwxr-xr-x   0 kharltayyab  (1000) kharltayyab  (1000)      276 2024-04-01 07:45:05.000000 tweety-ns-1.1.1/src/tweety/__init__.py
--rwxr-xr-x   0 kharltayyab  (1000) kharltayyab  (1000)     7504 2024-03-04 12:19:25.000000 tweety-ns-1.1.1/src/tweety/auth.py
--rwxr-xr-x   0 kharltayyab  (1000) kharltayyab  (1000)    31680 2024-03-20 05:30:39.000000 tweety-ns-1.1.1/src/tweety/bot.py
--rwxr-xr-x   0 kharltayyab  (1000) kharltayyab  (1000)    95767 2024-03-20 11:19:15.000000 tweety-ns-1.1.1/src/tweety/builder.py
-drwxrwxr-x   0 kharltayyab  (1000) kharltayyab  (1000)        0 2024-04-01 07:46:03.631728 tweety-ns-1.1.1/src/tweety/events/
--rwxr-xr-x   0 kharltayyab  (1000) kharltayyab  (1000)       42 2023-07-04 06:05:54.000000 tweety-ns-1.1.1/src/tweety/events/__init__.py
--rwxr-xr-x   0 kharltayyab  (1000) kharltayyab  (1000)     2119 2024-03-31 11:29:17.000000 tweety-ns-1.1.1/src/tweety/events/newmessage.py
--rwxr-xr-x   0 kharltayyab  (1000) kharltayyab  (1000)    21984 2024-03-19 11:58:49.000000 tweety-ns-1.1.1/src/tweety/exceptions_.py
--rwxr-xr-x   0 kharltayyab  (1000) kharltayyab  (1000)     2341 2024-03-03 15:25:23.000000 tweety-ns-1.1.1/src/tweety/filters.py
--rwxr-xr-x   0 kharltayyab  (1000) kharltayyab  (1000)    20098 2024-03-20 05:50:42.000000 tweety-ns-1.1.1/src/tweety/http.py
--rwxr-xr-x   0 kharltayyab  (1000) kharltayyab  (1000)     1844 2024-03-20 17:15:35.000000 tweety-ns-1.1.1/src/tweety/session.py
-drwxrwxr-x   0 kharltayyab  (1000) kharltayyab  (1000)        0 2024-04-01 07:46:03.631728 tweety-ns-1.1.1/src/tweety/types/
--rwxr-xr-x   0 kharltayyab  (1000) kharltayyab  (1000)     1249 2024-03-20 05:30:39.000000 tweety-ns-1.1.1/src/tweety/types/__init__.py
--rwxr-xr-x   0 kharltayyab  (1000) kharltayyab  (1000)     3039 2024-02-12 12:06:11.000000 tweety-ns-1.1.1/src/tweety/types/base.py
--rwxr-xr-x   0 kharltayyab  (1000) kharltayyab  (1000)     1172 2024-01-20 09:02:27.000000 tweety-ns-1.1.1/src/tweety/types/bookmarks.py
--rwxr-xr-x   0 kharltayyab  (1000) kharltayyab  (1000)     3256 2024-01-20 09:00:34.000000 tweety-ns-1.1.1/src/tweety/types/community.py
--rwxr-xr-x   0 kharltayyab  (1000) kharltayyab  (1000)     4054 2024-02-22 14:22:03.000000 tweety-ns-1.1.1/src/tweety/types/follow.py
--rwxr-xr-x   0 kharltayyab  (1000) kharltayyab  (1000)      987 2024-01-20 08:43:34.000000 tweety-ns-1.1.1/src/tweety/types/gifs.py
--rwxr-xr-x   0 kharltayyab  (1000) kharltayyab  (1000)    17219 2024-03-31 11:47:45.000000 tweety-ns-1.1.1/src/tweety/types/inbox.py
--rwxr-xr-x   0 kharltayyab  (1000) kharltayyab  (1000)     1444 2024-03-03 17:35:17.000000 tweety-ns-1.1.1/src/tweety/types/likes.py
--rwxr-xr-x   0 kharltayyab  (1000) kharltayyab  (1000)     4302 2024-01-20 08:28:50.000000 tweety-ns-1.1.1/src/tweety/types/lists.py
--rwxr-xr-x   0 kharltayyab  (1000) kharltayyab  (1000)     1511 2024-01-19 19:19:11.000000 tweety-ns-1.1.1/src/tweety/types/mentions.py
--rwxr-xr-x   0 kharltayyab  (1000) kharltayyab  (1000)     9019 2024-03-20 17:11:54.000000 tweety-ns-1.1.1/src/tweety/types/n_types.py
--rwxr-xr-x   0 kharltayyab  (1000) kharltayyab  (1000)     1351 2024-01-19 19:15:58.000000 tweety-ns-1.1.1/src/tweety/types/notification.py
--rw-rw-r--   0 kharltayyab  (1000) kharltayyab  (1000)     1103 2024-03-20 05:31:04.000000 tweety-ns-1.1.1/src/tweety/types/places.py
--rwxr-xr-x   0 kharltayyab  (1000) kharltayyab  (1000)     1184 2024-01-19 19:12:37.000000 tweety-ns-1.1.1/src/tweety/types/retweets.py
--rwxr-xr-x   0 kharltayyab  (1000) kharltayyab  (1000)     3806 2024-02-03 16:37:11.000000 tweety-ns-1.1.1/src/tweety/types/search.py
--rwxr-xr-x   0 kharltayyab  (1000) kharltayyab  (1000)     1216 2024-01-31 06:59:29.000000 tweety-ns-1.1.1/src/tweety/types/topic.py
--rwxr-xr-x   0 kharltayyab  (1000) kharltayyab  (1000)    58413 2024-03-27 06:41:42.000000 tweety-ns-1.1.1/src/tweety/types/twDataTypes.py
--rwxr-xr-x   0 kharltayyab  (1000) kharltayyab  (1000)    12236 2024-03-18 07:58:43.000000 tweety-ns-1.1.1/src/tweety/types/usertweet.py
--rwxr-xr-x   0 kharltayyab  (1000) kharltayyab  (1000)      475 2024-03-31 08:30:34.000000 tweety-ns-1.1.1/src/tweety/updates.py
--rwxr-xr-x   0 kharltayyab  (1000) kharltayyab  (1000)    36036 2024-03-20 05:54:31.000000 tweety-ns-1.1.1/src/tweety/user.py
--rwxr-xr-x   0 kharltayyab  (1000) kharltayyab  (1000)     6192 2024-03-04 11:48:15.000000 tweety-ns-1.1.1/src/tweety/utils.py
-drwxrwxr-x   0 kharltayyab  (1000) kharltayyab  (1000)        0 2024-04-01 07:46:03.631728 tweety-ns-1.1.1/src/tweety_ns.egg-info/
--rw-r--r--   0 kharltayyab  (1000) kharltayyab  (1000)     1891 2024-04-01 07:46:03.000000 tweety-ns-1.1.1/src/tweety_ns.egg-info/PKG-INFO
--rwxr-xr-x   0 kharltayyab  (1000) kharltayyab  (1000)     1026 2024-04-01 07:46:03.000000 tweety-ns-1.1.1/src/tweety_ns.egg-info/SOURCES.txt
--rwxr-xr-x   0 kharltayyab  (1000) kharltayyab  (1000)        1 2024-04-01 07:46:03.000000 tweety-ns-1.1.1/src/tweety_ns.egg-info/dependency_links.txt
--rwxr-xr-x   0 kharltayyab  (1000) kharltayyab  (1000)       40 2024-04-01 07:46:03.000000 tweety-ns-1.1.1/src/tweety_ns.egg-info/requires.txt
--rwxr-xr-x   0 kharltayyab  (1000) kharltayyab  (1000)        7 2024-04-01 07:46:03.000000 tweety-ns-1.1.1/src/tweety_ns.egg-info/top_level.txt
+drwxrwxr-x   0 kharltayyab  (1000) kharltayyab  (1000)        0 2024-04-03 11:13:57.066130 tweety-ns-1.1.1a0/
+-rw-r--r--   0 kharltayyab  (1000) kharltayyab  (1000)     1893 2024-04-03 11:13:57.066130 tweety-ns-1.1.1a0/PKG-INFO
+-rwxr-xr-x   0 kharltayyab  (1000) kharltayyab  (1000)     1142 2023-12-31 07:12:35.000000 tweety-ns-1.1.1a0/README.md
+-rwxr-xr-x   0 kharltayyab  (1000) kharltayyab  (1000)      108 2021-11-15 09:32:36.000000 tweety-ns-1.1.1a0/pyproject.toml
+-rwxr-xr-x   0 kharltayyab  (1000) kharltayyab  (1000)      673 2024-04-03 11:13:57.066130 tweety-ns-1.1.1a0/setup.cfg
+-rwxr-xr-x   0 kharltayyab  (1000) kharltayyab  (1000)      787 2024-04-03 11:13:32.000000 tweety-ns-1.1.1a0/setup.py
+drwxrwxr-x   0 kharltayyab  (1000) kharltayyab  (1000)        0 2024-04-03 11:13:57.062130 tweety-ns-1.1.1a0/src/
+drwxrwxr-x   0 kharltayyab  (1000) kharltayyab  (1000)        0 2024-04-03 11:13:57.066130 tweety-ns-1.1.1a0/src/tweety/
+-rwxr-xr-x   0 kharltayyab  (1000) kharltayyab  (1000)      278 2024-04-03 11:13:43.000000 tweety-ns-1.1.1a0/src/tweety/__init__.py
+-rwxr-xr-x   0 kharltayyab  (1000) kharltayyab  (1000)     7504 2024-03-04 12:19:25.000000 tweety-ns-1.1.1a0/src/tweety/auth.py
+-rwxr-xr-x   0 kharltayyab  (1000) kharltayyab  (1000)    31680 2024-03-20 05:30:39.000000 tweety-ns-1.1.1a0/src/tweety/bot.py
+-rwxr-xr-x   0 kharltayyab  (1000) kharltayyab  (1000)    95767 2024-03-20 11:19:15.000000 tweety-ns-1.1.1a0/src/tweety/builder.py
+drwxrwxr-x   0 kharltayyab  (1000) kharltayyab  (1000)        0 2024-04-03 11:13:57.066130 tweety-ns-1.1.1a0/src/tweety/events/
+-rwxr-xr-x   0 kharltayyab  (1000) kharltayyab  (1000)       42 2023-07-04 06:05:54.000000 tweety-ns-1.1.1a0/src/tweety/events/__init__.py
+-rwxr-xr-x   0 kharltayyab  (1000) kharltayyab  (1000)     2119 2024-03-31 11:29:17.000000 tweety-ns-1.1.1a0/src/tweety/events/newmessage.py
+-rwxr-xr-x   0 kharltayyab  (1000) kharltayyab  (1000)    21984 2024-03-19 11:58:49.000000 tweety-ns-1.1.1a0/src/tweety/exceptions_.py
+-rwxr-xr-x   0 kharltayyab  (1000) kharltayyab  (1000)     2341 2024-03-03 15:25:23.000000 tweety-ns-1.1.1a0/src/tweety/filters.py
+-rwxr-xr-x   0 kharltayyab  (1000) kharltayyab  (1000)    20098 2024-03-20 05:50:42.000000 tweety-ns-1.1.1a0/src/tweety/http.py
+-rwxr-xr-x   0 kharltayyab  (1000) kharltayyab  (1000)     1844 2024-03-20 17:15:35.000000 tweety-ns-1.1.1a0/src/tweety/session.py
+drwxrwxr-x   0 kharltayyab  (1000) kharltayyab  (1000)        0 2024-04-03 11:13:57.066130 tweety-ns-1.1.1a0/src/tweety/types/
+-rwxr-xr-x   0 kharltayyab  (1000) kharltayyab  (1000)     1249 2024-03-20 05:30:39.000000 tweety-ns-1.1.1a0/src/tweety/types/__init__.py
+-rwxr-xr-x   0 kharltayyab  (1000) kharltayyab  (1000)     3039 2024-02-12 12:06:11.000000 tweety-ns-1.1.1a0/src/tweety/types/base.py
+-rwxr-xr-x   0 kharltayyab  (1000) kharltayyab  (1000)     1172 2024-01-20 09:02:27.000000 tweety-ns-1.1.1a0/src/tweety/types/bookmarks.py
+-rwxr-xr-x   0 kharltayyab  (1000) kharltayyab  (1000)     3256 2024-01-20 09:00:34.000000 tweety-ns-1.1.1a0/src/tweety/types/community.py
+-rwxr-xr-x   0 kharltayyab  (1000) kharltayyab  (1000)     4054 2024-02-22 14:22:03.000000 tweety-ns-1.1.1a0/src/tweety/types/follow.py
+-rwxr-xr-x   0 kharltayyab  (1000) kharltayyab  (1000)      987 2024-01-20 08:43:34.000000 tweety-ns-1.1.1a0/src/tweety/types/gifs.py
+-rwxr-xr-x   0 kharltayyab  (1000) kharltayyab  (1000)    17406 2024-04-03 10:27:15.000000 tweety-ns-1.1.1a0/src/tweety/types/inbox.py
+-rwxr-xr-x   0 kharltayyab  (1000) kharltayyab  (1000)     1444 2024-03-03 17:35:17.000000 tweety-ns-1.1.1a0/src/tweety/types/likes.py
+-rwxr-xr-x   0 kharltayyab  (1000) kharltayyab  (1000)     4302 2024-01-20 08:28:50.000000 tweety-ns-1.1.1a0/src/tweety/types/lists.py
+-rwxr-xr-x   0 kharltayyab  (1000) kharltayyab  (1000)     1511 2024-01-19 19:19:11.000000 tweety-ns-1.1.1a0/src/tweety/types/mentions.py
+-rwxr-xr-x   0 kharltayyab  (1000) kharltayyab  (1000)     9019 2024-03-20 17:11:54.000000 tweety-ns-1.1.1a0/src/tweety/types/n_types.py
+-rwxr-xr-x   0 kharltayyab  (1000) kharltayyab  (1000)     1351 2024-01-19 19:15:58.000000 tweety-ns-1.1.1a0/src/tweety/types/notification.py
+-rw-rw-r--   0 kharltayyab  (1000) kharltayyab  (1000)     1103 2024-03-20 05:31:04.000000 tweety-ns-1.1.1a0/src/tweety/types/places.py
+-rwxr-xr-x   0 kharltayyab  (1000) kharltayyab  (1000)     1184 2024-01-19 19:12:37.000000 tweety-ns-1.1.1a0/src/tweety/types/retweets.py
+-rwxr-xr-x   0 kharltayyab  (1000) kharltayyab  (1000)     3806 2024-02-03 16:37:11.000000 tweety-ns-1.1.1a0/src/tweety/types/search.py
+-rwxr-xr-x   0 kharltayyab  (1000) kharltayyab  (1000)     1216 2024-01-31 06:59:29.000000 tweety-ns-1.1.1a0/src/tweety/types/topic.py
+-rwxr-xr-x   0 kharltayyab  (1000) kharltayyab  (1000)    58413 2024-03-27 06:41:42.000000 tweety-ns-1.1.1a0/src/tweety/types/twDataTypes.py
+-rwxr-xr-x   0 kharltayyab  (1000) kharltayyab  (1000)    12236 2024-03-18 07:58:43.000000 tweety-ns-1.1.1a0/src/tweety/types/usertweet.py
+-rwxr-xr-x   0 kharltayyab  (1000) kharltayyab  (1000)      475 2024-03-31 08:30:34.000000 tweety-ns-1.1.1a0/src/tweety/updates.py
+-rwxr-xr-x   0 kharltayyab  (1000) kharltayyab  (1000)    36036 2024-03-20 05:54:31.000000 tweety-ns-1.1.1a0/src/tweety/user.py
+-rwxr-xr-x   0 kharltayyab  (1000) kharltayyab  (1000)     6192 2024-03-04 11:48:15.000000 tweety-ns-1.1.1a0/src/tweety/utils.py
+drwxrwxr-x   0 kharltayyab  (1000) kharltayyab  (1000)        0 2024-04-03 11:13:57.066130 tweety-ns-1.1.1a0/src/tweety_ns.egg-info/
+-rw-r--r--   0 kharltayyab  (1000) kharltayyab  (1000)     1893 2024-04-03 11:13:57.000000 tweety-ns-1.1.1a0/src/tweety_ns.egg-info/PKG-INFO
+-rwxr-xr-x   0 kharltayyab  (1000) kharltayyab  (1000)     1026 2024-04-03 11:13:57.000000 tweety-ns-1.1.1a0/src/tweety_ns.egg-info/SOURCES.txt
+-rwxr-xr-x   0 kharltayyab  (1000) kharltayyab  (1000)        1 2024-04-03 11:13:57.000000 tweety-ns-1.1.1a0/src/tweety_ns.egg-info/dependency_links.txt
+-rwxr-xr-x   0 kharltayyab  (1000) kharltayyab  (1000)       40 2024-04-03 11:13:57.000000 tweety-ns-1.1.1a0/src/tweety_ns.egg-info/requires.txt
+-rwxr-xr-x   0 kharltayyab  (1000) kharltayyab  (1000)        7 2024-04-03 11:13:57.000000 tweety-ns-1.1.1a0/src/tweety_ns.egg-info/top_level.txt
```

### Comparing `tweety-ns-1.1.1/PKG-INFO` & `tweety-ns-1.1.1a0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tweety-ns
-Version: 1.1.1
+Version: 1.1.1a0
 Summary: An easy Twitter Scraper
 Home-page: https://github.com/mahrtayyab/tweety
 Author: Tayyab Kharl
 Author-email: tayyabmahr@gmail.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/mahrtayyab/tweety/issues
 Project-URL: Documentation, https://github.com/mahrtayyab/tweety
```

### Comparing `tweety-ns-1.1.1/README.md` & `tweety-ns-1.1.1a0/README.md`

 * *Files identical despite different names*

### Comparing `tweety-ns-1.1.1/setup.cfg` & `tweety-ns-1.1.1a0/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = tweety-ns
-version = 1.1.1
+version = 1.1.1a0
 author = Tayyab Kharl
 author_email = tayyabmahr@gmail.com
 description = An easy Twitter Scraper
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/mahrtayyab/tweety
 project_urls =
```

### Comparing `tweety-ns-1.1.1/src/tweety/auth.py` & `tweety-ns-1.1.1a0/src/tweety/auth.py`

 * *Files identical despite different names*

### Comparing `tweety-ns-1.1.1/src/tweety/bot.py` & `tweety-ns-1.1.1a0/src/tweety/bot.py`

 * *Files identical despite different names*

### Comparing `tweety-ns-1.1.1/src/tweety/builder.py` & `tweety-ns-1.1.1a0/src/tweety/builder.py`

 * *Files identical despite different names*

### Comparing `tweety-ns-1.1.1/src/tweety/events/newmessage.py` & `tweety-ns-1.1.1a0/src/tweety/events/newmessage.py`

 * *Files identical despite different names*

### Comparing `tweety-ns-1.1.1/src/tweety/exceptions_.py` & `tweety-ns-1.1.1a0/src/tweety/exceptions_.py`

 * *Files identical despite different names*

### Comparing `tweety-ns-1.1.1/src/tweety/filters.py` & `tweety-ns-1.1.1a0/src/tweety/filters.py`

 * *Files identical despite different names*

### Comparing `tweety-ns-1.1.1/src/tweety/http.py` & `tweety-ns-1.1.1a0/src/tweety/http.py`

 * *Files identical despite different names*

### Comparing `tweety-ns-1.1.1/src/tweety/session.py` & `tweety-ns-1.1.1a0/src/tweety/session.py`

 * *Files identical despite different names*

### Comparing `tweety-ns-1.1.1/src/tweety/types/__init__.py` & `tweety-ns-1.1.1a0/src/tweety/types/__init__.py`

 * *Files identical despite different names*

### Comparing `tweety-ns-1.1.1/src/tweety/types/base.py` & `tweety-ns-1.1.1a0/src/tweety/types/base.py`

 * *Files identical despite different names*

### Comparing `tweety-ns-1.1.1/src/tweety/types/bookmarks.py` & `tweety-ns-1.1.1a0/src/tweety/types/bookmarks.py`

 * *Files identical despite different names*

### Comparing `tweety-ns-1.1.1/src/tweety/types/community.py` & `tweety-ns-1.1.1a0/src/tweety/types/community.py`

 * *Files identical despite different names*

### Comparing `tweety-ns-1.1.1/src/tweety/types/follow.py` & `tweety-ns-1.1.1a0/src/tweety/types/follow.py`

 * *Files identical despite different names*

### Comparing `tweety-ns-1.1.1/src/tweety/types/gifs.py` & `tweety-ns-1.1.1a0/src/tweety/types/gifs.py`

 * *Files identical despite different names*

### Comparing `tweety-ns-1.1.1/src/tweety/types/inbox.py` & `tweety-ns-1.1.1a0/src/tweety/types/inbox.py`

 * *Files 2% similar despite different names*

```diff
@@ -107,14 +107,15 @@
 
     def __init__(self, conversation, inbox, client, get_all_messages=False):
         super().__init__()
         self._inbox = inbox
         self._client = client
         self._raw = conversation
         self._get_all_messages = get_all_messages
+        self.admin = None
         self.id = self['id'] = self._get_key("conversation_id")
         self.last_read_event_id = self['last_read_event_id'] = self._get_key("last_read_event_id")
         self.low_quality = self['low_quality'] = self._get_key("low_quality")
         self.max_entry_id = self['max_entry_id'] = self._get_key("max_entry_id")
         self.min_entry_id = self['min_entry_id'] = self._get_key("min_entry_id")
         self.muted = self['muted'] = self._get_key("muted")
         self.notifications_disabled = self['notifications_disabled'] = self._get_key("notifications_disabled")
@@ -136,21 +137,27 @@
                     return participant.name
         return ""
 
     def get_participants(self):
         users = []
         participants = self._raw['participants']
         for participant in participants:
+            this_user = None
             try:
                 user = self._inbox['users'].get(str(participant['user_id']))
                 if user:
                     user['__typename'] = "User"
-                    users.append(User(self._client, user))
+                    this_user = User(self._client, user)
             except Exception as e:
-                users.append(str(participant['user_id']))
+                this_user = str(participant["user_id"])
+
+            if participant.get("is_admin") is True:
+                self.admin = this_user
+
+            users.append(this_user)
 
         return users
 
     def _get_key(self, keyName, default=None):
         return self._raw.get(keyName, default)
 
     def _parse_message(self, entry):
```

### Comparing `tweety-ns-1.1.1/src/tweety/types/likes.py` & `tweety-ns-1.1.1a0/src/tweety/types/likes.py`

 * *Files identical despite different names*

### Comparing `tweety-ns-1.1.1/src/tweety/types/lists.py` & `tweety-ns-1.1.1a0/src/tweety/types/lists.py`

 * *Files identical despite different names*

### Comparing `tweety-ns-1.1.1/src/tweety/types/mentions.py` & `tweety-ns-1.1.1a0/src/tweety/types/mentions.py`

 * *Files identical despite different names*

### Comparing `tweety-ns-1.1.1/src/tweety/types/n_types.py` & `tweety-ns-1.1.1a0/src/tweety/types/n_types.py`

 * *Files identical despite different names*

### Comparing `tweety-ns-1.1.1/src/tweety/types/notification.py` & `tweety-ns-1.1.1a0/src/tweety/types/notification.py`

 * *Files identical despite different names*

### Comparing `tweety-ns-1.1.1/src/tweety/types/places.py` & `tweety-ns-1.1.1a0/src/tweety/types/places.py`

 * *Files identical despite different names*

### Comparing `tweety-ns-1.1.1/src/tweety/types/retweets.py` & `tweety-ns-1.1.1a0/src/tweety/types/retweets.py`

 * *Files identical despite different names*

### Comparing `tweety-ns-1.1.1/src/tweety/types/search.py` & `tweety-ns-1.1.1a0/src/tweety/types/search.py`

 * *Files identical despite different names*

### Comparing `tweety-ns-1.1.1/src/tweety/types/topic.py` & `tweety-ns-1.1.1a0/src/tweety/types/topic.py`

 * *Files identical despite different names*

### Comparing `tweety-ns-1.1.1/src/tweety/types/twDataTypes.py` & `tweety-ns-1.1.1a0/src/tweety/types/twDataTypes.py`

 * *Files identical despite different names*

### Comparing `tweety-ns-1.1.1/src/tweety/types/usertweet.py` & `tweety-ns-1.1.1a0/src/tweety/types/usertweet.py`

 * *Files identical despite different names*

### Comparing `tweety-ns-1.1.1/src/tweety/user.py` & `tweety-ns-1.1.1a0/src/tweety/user.py`

 * *Files identical despite different names*

### Comparing `tweety-ns-1.1.1/src/tweety/utils.py` & `tweety-ns-1.1.1a0/src/tweety/utils.py`

 * *Files identical despite different names*

### Comparing `tweety-ns-1.1.1/src/tweety_ns.egg-info/PKG-INFO` & `tweety-ns-1.1.1a0/src/tweety_ns.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tweety-ns
-Version: 1.1.1
+Version: 1.1.1a0
 Summary: An easy Twitter Scraper
 Home-page: https://github.com/mahrtayyab/tweety
 Author: Tayyab Kharl
 Author-email: tayyabmahr@gmail.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/mahrtayyab/tweety/issues
 Project-URL: Documentation, https://github.com/mahrtayyab/tweety
```

### Comparing `tweety-ns-1.1.1/src/tweety_ns.egg-info/SOURCES.txt` & `tweety-ns-1.1.1a0/src/tweety_ns.egg-info/SOURCES.txt`

 * *Files identical despite different names*

