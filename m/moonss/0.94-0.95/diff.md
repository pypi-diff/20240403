# Comparing `tmp/moonss-0.94.tar.gz` & `tmp/moonss-0.95.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "moonss-0.94.tar", last modified: Wed Dec 20 09:26:05 2023, max compression
+gzip compressed data, was "moonss-0.95.tar", last modified: Wed Apr  3 05:20:29 2024, max compression
```

## Comparing `moonss-0.94.tar` & `moonss-0.95.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-20 09:26:05.610345 moonss-0.94/
--rw-r--r--   0 runner    (1001) docker     (127)     1889 2023-12-20 09:25:50.000000 moonss-0.94/DownloadHelper.py
--rw-r--r--   0 runner    (1001) docker     (127)      521 2023-12-20 09:26:05.610345 moonss-0.94/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       22 2023-12-20 09:25:50.000000 moonss-0.94/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     3282 2023-12-20 09:25:50.000000 moonss-0.94/SourceDataHelper.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-20 09:26:05.610345 moonss-0.94/moonss.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      521 2023-12-20 09:26:05.000000 moonss-0.94/moonss.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      215 2023-12-20 09:26:05.000000 moonss-0.94/moonss.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-20 09:26:05.000000 moonss-0.94/moonss.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       65 2023-12-20 09:26:05.000000 moonss-0.94/moonss.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       39 2023-12-20 09:26:05.000000 moonss-0.94/moonss.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1683 2023-12-20 09:25:50.000000 moonss-0.94/moonss.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-20 09:26:05.610345 moonss-0.94/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      697 2023-12-20 09:25:50.000000 moonss-0.94/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 05:20:29.576264 moonss-0.95/
+-rw-r--r--   0 runner    (1001) docker     (127)     2834 2024-04-03 05:20:20.000000 moonss-0.95/DownloadHelper.py
+-rw-r--r--   0 runner    (1001) docker     (127)      521 2024-04-03 05:20:29.576264 moonss-0.95/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-03 05:20:20.000000 moonss-0.95/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3282 2024-04-03 05:20:20.000000 moonss-0.95/SourceDataHelper.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 05:20:29.572264 moonss-0.95/moonss.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      521 2024-04-03 05:20:29.000000 moonss-0.95/moonss.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      215 2024-04-03 05:20:29.000000 moonss-0.95/moonss.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 05:20:29.000000 moonss-0.95/moonss.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-04-03 05:20:29.000000 moonss-0.95/moonss.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-04-03 05:20:29.000000 moonss-0.95/moonss.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1683 2024-04-03 05:20:20.000000 moonss-0.95/moonss.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-03 05:20:29.576264 moonss-0.95/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      697 2024-04-03 05:20:20.000000 moonss-0.95/setup.py
```

### Comparing `moonss-0.94/DownloadHelper.py` & `moonss-0.95/DownloadHelper.py`

 * *Files 19% similar despite different names*

```diff
@@ -9,25 +9,40 @@
     proxy_tmp = f"http://victor69:dota2hoabt2@geo.iproyal.com:12321"
     proxies = {"http": proxy_tmp, "https": proxy_tmp}
     return proxies
 
 def get_download_nwm_tiktok(url, retries=3):
     try:
         video_id=url.split('/')[-1]
+        urld = f"https://api22-normal-c-alisg.tiktokv.com/aweme/v1/feed/?aweme_id={video_id}&iid=7329834909681551122&device_id=7325735055111128585&channel=googleplay&app_name=musical_ly&version_code=330205&device_platform=android&device_type=SM-N950F&version=9"
+        proxies=get_proxy_iproyal()
+        headers={'user-agent':'com.zhiliaoapp.musically/2023302050 (Linux; U; Android 9; en; SM-N950F; Build/PPR1.180610.011; Cronet/TTNetVersion:996128d2 2024-01-12 QuicVersion:ce58f68a 2024-01-12)'}
+        res=requests.get(urld,headers=headers,proxies=proxies).json()
+        data=res['aweme_list'][0]
+        nwm_video_url_HQ= data['video']['bit_rate'][0]['play_addr']['url_list'][0]
+        return nwm_video_url_HQ
+    except:
+        if retries > 1:
+            return get_download_nwm_tiktok(url,retries-1)
+        pass
+    return None
+def get_download_nwm_tiktok_old(url, retries=3):
+    try:
+        video_id=url.split('/')[-1]
         urld = f"https://api16-normal-c-useast1a.tiktokv.com/aweme/v1/feed/?aweme_id={video_id}"
         proxies=get_proxy_iproyal()
         headers={'user-agent':'com.ss.android.ugc.trill/494+Mozilla/5.0+(Linux;+Android+12;+2112123G+Build/SKQ1.211006.001;+wv)+AppleWebKit/537.36+(KHTML,+like+Gecko)+Version/4.0+Chrome/107.0.5304.105+Mobile+Safari/537.36'}
         res=requests.get(urld, headers=headers, proxies=proxies).json()
         # print(res)
         data=res['aweme_list'][0]
         nwm_video_url_HQ= data['video']['bit_rate'][0]['play_addr']['url_list'][0]
         return nwm_video_url_HQ
     except:
         if retries > 1:
-            return get_download_nwm_tiktok(url,retries-1)
+            return get_download_nwm_tiktok_old(url,retries-1)
         pass
     return None
 
 def download_ytdlp(videoId):
     videoId = videoId.strip()
     result = os.path.join(get_dir("download"), f"{videoId}.webm")
     cmd = f"yt-dlp -f bv+ba/b -o {result} {videoId}"
@@ -42,8 +57,9 @@
 def download_douyin_video(video_id):
     return download_file(f"https://aweme.snssdk.com/aweme/v1/play/?video_id={video_id}&ratio=1080p&line=0",None, "mp4")
 def donwload_instagram_video(crawl_data_txt):
     crawl_data = json.loads(crawl_data_txt)
     if "video_url" in crawl_data:
         return download_file(crawl_data['video_url'],None, "mp4")
     else:
-        return None
+        return None
+
```

### Comparing `moonss-0.94/PKG-INFO` & `moonss-0.95/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: moonss
-Version: 0.94
+Version: 0.95
 Summary: A Des of moonss
 Home-page: https://github.com/vtandroid/dokr
 Author: Thanh Hoa
 Author-email: thanhhoakhmt1@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `moonss-0.94/SourceDataHelper.py` & `moonss-0.95/SourceDataHelper.py`

 * *Files identical despite different names*

### Comparing `moonss-0.94/moonss.egg-info/PKG-INFO` & `moonss-0.95/moonss.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: moonss
-Version: 0.94
+Version: 0.95
 Summary: A Des of moonss
 Home-page: https://github.com/vtandroid/dokr
 Author: Thanh Hoa
 Author-email: thanhhoakhmt1@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `moonss-0.94/moonss.py` & `moonss-0.95/moonss.py`

 * *Files identical despite different names*

### Comparing `moonss-0.94/setup.py` & `moonss-0.95/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import setuptools
 
 setuptools.setup(
     name='moonss',
-    version='0.94',
+    version='0.95',
     author="Thanh Hoa",
     author_email="thanhhoakhmt1@gmail.com",
     description="A Des of moonss",
     long_description="Des",
     long_description_content_type="text/markdown",
     url="https://github.com/vtandroid/dokr",
     packages=setuptools.find_packages(),
```

