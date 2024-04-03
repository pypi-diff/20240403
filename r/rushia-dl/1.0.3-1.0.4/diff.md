# Comparing `tmp/rushia_dl-1.0.3-py3-none-any.whl.zip` & `tmp/rushia_dl-1.0.4-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 4558 bytes, number of entries: 8
--rw-r--r--  2.0 unx        0 b- defN 24-Jan-16 07:43 rushia_dl/__init__.py
--rw-r--r--  2.0 unx     2346 b- defN 24-Jan-16 07:53 rushia_dl/cli.py
--rw-r--r--  2.0 unx     1063 b- defN 24-Jan-16 08:12 rushia_dl-1.0.3.dist-info/LICENSE
--rw-r--r--  2.0 unx     2805 b- defN 24-Jan-16 08:12 rushia_dl-1.0.3.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-Jan-16 08:12 rushia_dl-1.0.3.dist-info/WHEEL
--rw-r--r--  2.0 unx       49 b- defN 24-Jan-16 08:12 rushia_dl-1.0.3.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       10 b- defN 24-Jan-16 08:12 rushia_dl-1.0.3.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      641 b- defN 24-Jan-16 08:12 rushia_dl-1.0.3.dist-info/RECORD
-8 files, 7006 bytes uncompressed, 3432 bytes compressed:  51.0%
+Zip file size: 4697 bytes, number of entries: 8
+-rw-r--r--  2.0 unx        0 b- defN 24-Apr-03 11:13 rushia_dl/__init__.py
+-rw-r--r--  2.0 unx     3631 b- defN 24-Apr-03 13:03 rushia_dl/cli.py
+-rw-r--r--  2.0 unx     1063 b- defN 24-Apr-03 13:10 rushia_dl-1.0.4.dist-info/LICENSE
+-rw-r--r--  2.0 unx     2805 b- defN 24-Apr-03 13:10 rushia_dl-1.0.4.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-Apr-03 13:10 rushia_dl-1.0.4.dist-info/WHEEL
+-rw-r--r--  2.0 unx       49 b- defN 24-Apr-03 13:10 rushia_dl-1.0.4.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       10 b- defN 24-Apr-03 13:10 rushia_dl-1.0.4.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      641 b- defN 24-Apr-03 13:10 rushia_dl-1.0.4.dist-info/RECORD
+8 files, 8291 bytes uncompressed, 3571 bytes compressed:  56.9%
```

## zipnote {}

```diff
@@ -1,25 +1,25 @@
 Filename: rushia_dl/__init__.py
 Comment: 
 
 Filename: rushia_dl/cli.py
 Comment: 
 
-Filename: rushia_dl-1.0.3.dist-info/LICENSE
+Filename: rushia_dl-1.0.4.dist-info/LICENSE
 Comment: 
 
-Filename: rushia_dl-1.0.3.dist-info/METADATA
+Filename: rushia_dl-1.0.4.dist-info/METADATA
 Comment: 
 
-Filename: rushia_dl-1.0.3.dist-info/WHEEL
+Filename: rushia_dl-1.0.4.dist-info/WHEEL
 Comment: 
 
-Filename: rushia_dl-1.0.3.dist-info/entry_points.txt
+Filename: rushia_dl-1.0.4.dist-info/entry_points.txt
 Comment: 
 
-Filename: rushia_dl-1.0.3.dist-info/top_level.txt
+Filename: rushia_dl-1.0.4.dist-info/top_level.txt
 Comment: 
 
-Filename: rushia_dl-1.0.3.dist-info/RECORD
+Filename: rushia_dl-1.0.4.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## rushia_dl/cli.py

```diff
@@ -22,37 +22,63 @@
                         help="""
                         [REQUIRE] Please enter the video URL.
                         """)
     parser.add_argument("-f","--format", dest="format", required=True, choices=["mp3", "mp4"],
                         help="""
                         [REQUIRE] Please input format that mp3 or mp4.
                         """)
+    parser.add_argument("-m","--membership", dest="is_membership", required=False, action='store_true',
+                        help="""
+                        [OPTION] Please input -m option if you to do download file is membership only content.
+                        """)
     args = parser.parse_args()
     return args
 
 def main():
     args = parser()
-    if args.format == 'mp3':
-        ydl_opts = {
-            'format': 'bestaudio/best', # choice of quality
-            'extractaudio' : True,      # only keep the audio
-            'audioformat' : 'mp3',      # convert to mp3
-            'noplaylist' : True,        # only download single song, not playlist
-            'postprocessors': [{
-              'key': 'FFmpegExtractAudio',
-              'preferredcodec': 'mp3',
-              'preferredquality': '192',
-              }],
-             }
-    elif args.format == 'mp4':
-        ydl_opts = {
-            'format': 'bestvideo[ext=mp4]+bestaudio[ext=m4a]/bestvideo+bestaudio/best',
-            'download-archive': './download_cache.log',
-            'retries': 3,
-            }
+    if is_membership:
+        if args.format == 'mp3':
+            ydl_opts = {
+                'format': 'bestaudio/best', # choice of quality
+                'extractaudio' : True,      # only keep the audio
+                'audioformat' : 'mp3',      # convert to mp3
+                'noplaylist' : True,        # only download single song, not playlist
+                'cookiesfrombrowser': 'chrome',
+                'postprocessors': [{
+                  'key': 'FFmpegExtractAudio',
+                  'preferredcodec': 'mp3',
+                  'preferredquality': '192',
+                  }],
+                 }
+        elif args.format == 'mp4':
+            ydl_opts = {
+                'cookiesfrombrowser': 'chrome',
+                'format': 'bestvideo[ext=mp4]+bestaudio[ext=m4a]/bestvideo+bestaudio/best',
+                'download-archive': './download_cache.log',
+                'retries': 3,
+                }
+    else:
+        if args.format == 'mp3':
+            ydl_opts = {
+                'format': 'bestaudio/best', # choice of quality
+                'extractaudio' : True,      # only keep the audio
+                'audioformat' : 'mp3',      # convert to mp3
+                'noplaylist' : True,        # only download single song, not playlist
+                'postprocessors': [{
+                  'key': 'FFmpegExtractAudio',
+                  'preferredcodec': 'mp3',
+                  'preferredquality': '192',
+                  }],
+                 }
+        elif args.format == 'mp4':
+            ydl_opts = {
+                'format': 'bestvideo[ext=mp4]+bestaudio[ext=m4a]/bestvideo+bestaudio/best',
+                'download-archive': './download_cache.log',
+                'retries': 3,
+                }
 
     if args.path:
         if not Path(args.path).exists():
             print(f'{args.path} does not found.')
             exit(1)
         with open(args.path) as f:
             for video_url in f:
```

## Comparing `rushia_dl-1.0.3.dist-info/LICENSE` & `rushia_dl-1.0.4.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `rushia_dl-1.0.3.dist-info/METADATA` & `rushia_dl-1.0.4.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rushia-dl
-Version: 1.0.3
+Version: 1.0.4
 Summary: Youtube video & audio download wrapper
 Home-page: https://github.com/konono/rushia_dl
 Author: konono
 Author-email: kono@ms1.kononet.jp
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
```

