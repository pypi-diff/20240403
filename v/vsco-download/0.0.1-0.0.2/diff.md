# Comparing `tmp/vsco_download-0.0.1.tar.gz` & `tmp/vsco_download-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vsco_download-0.0.1.tar", last modified: Fri Mar  8 08:18:08 2024, max compression
+gzip compressed data, was "vsco_download-0.0.2.tar", last modified: Wed Apr  3 06:20:29 2024, max compression
```

## Comparing `vsco_download-0.0.1.tar` & `vsco_download-0.0.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-03-08 08:18:08.902481 vsco_download-0.0.1/
--rw-rw-rw-   0        0        0    11524 2024-03-08 02:28:31.000000 vsco_download-0.0.1/LICENSE
--rw-rw-rw-   0        0        0      407 2024-03-08 08:18:08.902481 vsco_download-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0       27 2024-03-08 02:28:31.000000 vsco_download-0.0.1/README.md
--rw-rw-rw-   0        0        0       86 2024-03-08 08:18:08.904802 vsco_download-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      519 2024-03-08 08:17:36.000000 vsco_download-0.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2024-03-08 08:18:08.893836 vsco_download-0.0.1/vsco_download/
--rw-rw-rw-   0        0        0        0 2024-03-08 07:29:08.000000 vsco_download-0.0.1/vsco_download/__init__.py
--rw-rw-rw-   0        0        0     5867 2024-03-08 08:08:46.000000 vsco_download-0.0.1/vsco_download/api.py
-drwxrwxrwx   0        0        0        0 2024-03-08 08:18:08.902481 vsco_download-0.0.1/vsco_download.egg-info/
--rw-rw-rw-   0        0        0      407 2024-03-08 08:18:08.000000 vsco_download-0.0.1/vsco_download.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      267 2024-03-08 08:18:08.000000 vsco_download-0.0.1/vsco_download.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-08 08:18:08.000000 vsco_download-0.0.1/vsco_download.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2024-03-08 08:18:08.000000 vsco_download-0.0.1/vsco_download.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2024-03-08 08:18:08.000000 vsco_download-0.0.1/vsco_download.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-03 06:20:29.732775 vsco_download-0.0.2/
+-rw-rw-rw-   0        0        0    11524 2024-03-08 02:28:31.000000 vsco_download-0.0.2/LICENSE
+-rw-rw-rw-   0        0        0      407 2024-04-03 06:20:29.732775 vsco_download-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0      873 2024-04-03 06:16:03.000000 vsco_download-0.0.2/README.md
+-rw-rw-rw-   0        0        0       86 2024-04-03 06:20:29.736354 vsco_download-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      519 2024-04-03 06:20:19.000000 vsco_download-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-03 06:20:29.700887 vsco_download-0.0.2/vsco_download/
+-rw-rw-rw-   0        0        0        0 2024-03-08 07:29:08.000000 vsco_download-0.0.2/vsco_download/__init__.py
+-rw-rw-rw-   0        0        0     5868 2024-04-03 06:15:32.000000 vsco_download-0.0.2/vsco_download/api.py
+drwxrwxrwx   0        0        0        0 2024-04-03 06:20:29.729308 vsco_download-0.0.2/vsco_download.egg-info/
+-rw-rw-rw-   0        0        0      407 2024-04-03 06:20:29.000000 vsco_download-0.0.2/vsco_download.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      267 2024-04-03 06:20:29.000000 vsco_download-0.0.2/vsco_download.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-03 06:20:29.000000 vsco_download-0.0.2/vsco_download.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2024-04-03 06:20:29.000000 vsco_download-0.0.2/vsco_download.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2024-04-03 06:20:29.000000 vsco_download-0.0.2/vsco_download.egg-info/top_level.txt
```

### Comparing `vsco_download-0.0.1/LICENSE` & `vsco_download-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `vsco_download-0.0.1/setup.py` & `vsco_download-0.0.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup, find_packages
 setup(
     name='vsco_download',
-    version='0.0.1',
+    version='0.0.2',
     author='Lockermanwxlf',
     author_email='sexyandhandsome12@gmail.com',
     description='A wrapper for VSCO download endpoints',
     packages=find_packages(),
     classifiers=[
         'Programming Language :: Python :: 3',
         'License :: OSI Approved :: Apache Software License',
```

### Comparing `vsco_download-0.0.1/vsco_download/api.py` & `vsco_download-0.0.2/vsco_download/api.py`

 * *Files 0% similar despite different names*

```diff
@@ -137,15 +137,15 @@
 
             VscoMedia(
                 self.session, f'https://{info['responsive_url']}', info['upload_date'], True)
 
             if not info['is_video'] else
 
             VscoMedia(
-                self.session, f'https//{info['video_url']}', info['upload_date'], False)
+                self.session, f'https://{info['video_url']}', info['upload_date'], False)
 
             for info in map(lambda x: x[x['type']], json['media'])
 
         ]
         return (medias, json.get('next_cursor'))
  
     def get_media_cursor(self, site_id: str):
```

