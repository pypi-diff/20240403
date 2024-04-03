# Comparing `tmp/spotify_web_downloader-1.6.2.tar.gz` & `tmp/spotify_web_downloader-1.6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spotify_web_downloader-1.6.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "spotify_web_downloader-1.6.3.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `spotify_web_downloader-1.6.2.tar` & `spotify_web_downloader-1.6.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0     1137 2024-04-03 00:09:23.060490 spotify_web_downloader-1.6.2/.github/workflows/main.yml
--rw-r--r--   0        0        0       96 2024-04-03 00:09:23.060490 spotify_web_downloader-1.6.2/.gitignore
--rw-r--r--   0        0        0     8437 2024-04-03 00:09:23.060490 spotify_web_downloader-1.6.2/README.md
--rw-r--r--   0        0        0      533 2024-04-03 00:09:23.060490 spotify_web_downloader-1.6.2/pyproject.toml
--rw-r--r--   0        0        0       40 2024-04-03 00:09:23.060490 spotify_web_downloader-1.6.2/requirements.txt
--rw-r--r--   0        0        0       22 2024-04-03 00:09:23.060490 spotify_web_downloader-1.6.2/spotify_web_downloader/__init__.py
--rw-r--r--   0        0        0       30 2024-04-03 00:09:23.060490 spotify_web_downloader-1.6.2/spotify_web_downloader/__main__.py
--rw-r--r--   0        0        0    21310 2024-04-03 00:09:23.060490 spotify_web_downloader-1.6.2/spotify_web_downloader/cli.py
--rw-r--r--   0        0        0      511 2024-04-03 00:09:23.060490 spotify_web_downloader-1.6.2/spotify_web_downloader/constants.py
--rw-r--r--   0        0        0     8546 2024-04-03 00:09:23.060490 spotify_web_downloader-1.6.2/spotify_web_downloader/downloader.py
--rw-r--r--   0        0        0    11132 2024-04-03 00:09:23.060490 spotify_web_downloader-1.6.2/spotify_web_downloader/downloader_music_video.py
--rw-r--r--   0        0        0     9258 2024-04-03 00:09:23.060490 spotify_web_downloader-1.6.2/spotify_web_downloader/downloader_song.py
--rw-r--r--   0        0        0      177 2024-04-03 00:09:23.060490 spotify_web_downloader-1.6.2/spotify_web_downloader/enums.py
--rw-r--r--   0        0        0     4015 2024-04-03 00:09:23.060490 spotify_web_downloader-1.6.2/spotify_web_downloader/hardcoded_wvd.py
--rw-r--r--   0        0        0      707 2024-04-03 00:09:23.060490 spotify_web_downloader-1.6.2/spotify_web_downloader/models.py
--rw-r--r--   0        0        0     7738 2024-04-03 00:09:23.060490 spotify_web_downloader-1.6.2/spotify_web_downloader/spotify_api.py
--rw-r--r--   0        0        0     8848 1970-01-01 00:00:00.000000 spotify_web_downloader-1.6.2/PKG-INFO
+-rw-r--r--   0        0        0     1137 2024-04-03 13:01:18.141462 spotify_web_downloader-1.6.3/.github/workflows/main.yml
+-rw-r--r--   0        0        0       96 2024-04-03 13:01:18.141462 spotify_web_downloader-1.6.3/.gitignore
+-rw-r--r--   0        0        0     8437 2024-04-03 13:01:18.141462 spotify_web_downloader-1.6.3/README.md
+-rw-r--r--   0        0        0      533 2024-04-03 13:01:18.145462 spotify_web_downloader-1.6.3/pyproject.toml
+-rw-r--r--   0        0        0       40 2024-04-03 13:01:18.145462 spotify_web_downloader-1.6.3/requirements.txt
+-rw-r--r--   0        0        0       22 2024-04-03 13:01:18.145462 spotify_web_downloader-1.6.3/spotify_web_downloader/__init__.py
+-rw-r--r--   0        0        0       30 2024-04-03 13:01:18.145462 spotify_web_downloader-1.6.3/spotify_web_downloader/__main__.py
+-rw-r--r--   0        0        0    21483 2024-04-03 13:01:18.145462 spotify_web_downloader-1.6.3/spotify_web_downloader/cli.py
+-rw-r--r--   0        0        0      507 2024-04-03 13:01:18.145462 spotify_web_downloader-1.6.3/spotify_web_downloader/constants.py
+-rw-r--r--   0        0        0     8546 2024-04-03 13:01:18.145462 spotify_web_downloader-1.6.3/spotify_web_downloader/downloader.py
+-rw-r--r--   0        0        0    11657 2024-04-03 13:01:18.145462 spotify_web_downloader-1.6.3/spotify_web_downloader/downloader_music_video.py
+-rw-r--r--   0        0        0     9254 2024-04-03 13:01:18.145462 spotify_web_downloader-1.6.3/spotify_web_downloader/downloader_song.py
+-rw-r--r--   0        0        0      177 2024-04-03 13:01:18.145462 spotify_web_downloader-1.6.3/spotify_web_downloader/enums.py
+-rw-r--r--   0        0        0     4015 2024-04-03 13:01:18.145462 spotify_web_downloader-1.6.3/spotify_web_downloader/hardcoded_wvd.py
+-rw-r--r--   0        0        0      707 2024-04-03 13:01:18.145462 spotify_web_downloader-1.6.3/spotify_web_downloader/models.py
+-rw-r--r--   0        0        0     7738 2024-04-03 13:01:18.145462 spotify_web_downloader-1.6.3/spotify_web_downloader/spotify_api.py
+-rw-r--r--   0        0        0     8848 1970-01-01 00:00:00.000000 spotify_web_downloader-1.6.3/PKG-INFO
```

### Comparing `spotify_web_downloader-1.6.2/.github/workflows/main.yml` & `spotify_web_downloader-1.6.3/.github/workflows/main.yml`

 * *Files identical despite different names*

### Comparing `spotify_web_downloader-1.6.2/README.md` & `spotify_web_downloader-1.6.3/README.md`

 * *Files identical despite different names*

### Comparing `spotify_web_downloader-1.6.2/pyproject.toml` & `spotify_web_downloader-1.6.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `spotify_web_downloader-1.6.2/spotify_web_downloader/cli.py` & `spotify_web_downloader-1.6.3/spotify_web_downloader/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -467,17 +467,20 @@
                     )
                 else:
                     cover_url = downloader.get_cover_url(metadata_gid, "XXLARGE")
                     logger.debug("Getting album metadata")
                     album_metadata = spotify_api.get_album(
                         spotify_api.gid_to_track_id(metadata_gid["album"]["gid"])
                     )
+                    logger.debug("Getting track credits")
+                    track_credits = spotify_api.get_track_credits(track_id)
                     tags = downloader_music_video.get_tags(
                         metadata_gid,
                         album_metadata,
+                        track_credits,
                     )
                     final_path = downloader_music_video.get_final_path(tags)
                     cover_path = downloader_music_video.get_cover_path(final_path)
                     if final_path.exists() and not overwrite:
                         logger.warning(
                             f'({queue_progress}) Music video already exists at "{final_path}", skipping'
                         )
```

### Comparing `spotify_web_downloader-1.6.2/spotify_web_downloader/downloader.py` & `spotify_web_downloader-1.6.3/spotify_web_downloader/downloader.py`

 * *Files identical despite different names*

### Comparing `spotify_web_downloader-1.6.2/spotify_web_downloader/downloader_music_video.py` & `spotify_web_downloader-1.6.3/spotify_web_downloader/downloader_music_video.py`

 * *Files 3% similar despite different names*

```diff
@@ -199,38 +199,51 @@
         m3u8_path.parent.mkdir(parents=True, exist_ok=True)
         m3u8_path.write_text(m3u8_str)
 
     def get_tags(
         self,
         metadata_gid: dict,
         album_metadata: dict,
+        track_credits: dict,
     ) -> dict:
         isrc = None
         if metadata_gid.get("external_id"):
             isrc = next(
                 (i for i in metadata_gid["external_id"] if i["type"] == "isrc"), None
             )
         release_date_datetime_obj = self.downloader.get_release_date_datetime_obj(
             metadata_gid
         )
+        producers = next(
+            role
+            for role in track_credits["roleCredits"]
+            if role["roleTitle"] == "Producers"
+        )["artists"]
+        composers = next(
+            role
+            for role in track_credits["roleCredits"]
+            if role["roleTitle"] == "Writers"
+        )["artists"]
         tags = {
             "artist": self.downloader.get_artist(metadata_gid["artist"]),
-            "comment": f'https://open.spotify.com/track/{metadata_gid["canonical_uri"].split(":")[-1]}',
+            "composer": self.downloader.get_artist(composers) if composers else None,
             "copyright": next(
                 (i["text"] for i in album_metadata["copyrights"] if i["type"] == "P"),
                 None,
             ),
             "isrc": isrc.get("id") if isrc is not None else None,
             "label": metadata_gid["album"].get("label"),
             "media_type": 6,
+            "producer": self.downloader.get_artist(producers) if producers else None,
             "rating": 1 if metadata_gid.get("explicit") else 0,
             "title": album_metadata["name"],
             "release_date": self.downloader.get_release_date_tag(
                 release_date_datetime_obj
             ),
+            "url": f'https://open.spotify.com/track/{metadata_gid["canonical_uri"].split(":")[-1]}',
         }
         tags["release_year"] = str(release_date_datetime_obj.year)
         return tags
 
     def download(self, m3u8_path: Path, encrypted_path: str):
         if self.download_mode == DownloadModeVideo.YTDLP:
             self.download_ytdlp(m3u8_path, encrypted_path)
```

### Comparing `spotify_web_downloader-1.6.2/spotify_web_downloader/downloader_song.py` & `spotify_web_downloader-1.6.3/spotify_web_downloader/downloader_song.py`

 * *Files 1% similar despite different names*

```diff
@@ -108,15 +108,14 @@
             for role in track_credits["roleCredits"]
             if role["roleTitle"] == "Writers"
         )["artists"]
         tags = {
             "album": album_metadata["name"],
             "album_artist": self.downloader.get_artist(album_metadata["artists"]),
             "artist": self.downloader.get_artist(metadata_gid["artist"]),
-            "comment": f'https://open.spotify.com/track/{metadata_gid["canonical_uri"].split(":")[-1]}',
             "compilation": (
                 True if album_metadata["album_type"] == "compilation" else False
             ),
             "composer": self.downloader.get_artist(composers) if composers else None,
             "copyright": next(
                 (i["text"] for i in album_metadata["copyrights"] if i["type"] == "P"),
                 None,
@@ -136,14 +135,15 @@
             "title": metadata_gid["name"],
             "track": metadata_gid["number"],
             "track_total": max(
                 i["track_number"]
                 for i in album_metadata["tracks"]["items"]
                 if i["disc_number"] == metadata_gid["disc_number"]
             ),
+            "url": f'https://open.spotify.com/track/{metadata_gid["canonical_uri"].split(":")[-1]}',
         }
         return tags
 
     def download(self, encrypted_path: Path, stream_url: str):
         if self.download_mode == DownloadModeSong.YTDLP:
             self.download_ytdlp(encrypted_path, stream_url)
         elif self.download_mode == DownloadModeSong.ARIA2C:
```

### Comparing `spotify_web_downloader-1.6.2/spotify_web_downloader/hardcoded_wvd.py` & `spotify_web_downloader-1.6.3/spotify_web_downloader/hardcoded_wvd.py`

 * *Files identical despite different names*

### Comparing `spotify_web_downloader-1.6.2/spotify_web_downloader/models.py` & `spotify_web_downloader-1.6.3/spotify_web_downloader/models.py`

 * *Files identical despite different names*

### Comparing `spotify_web_downloader-1.6.2/spotify_web_downloader/spotify_api.py` & `spotify_web_downloader-1.6.3/spotify_web_downloader/spotify_api.py`

 * *Files identical despite different names*

### Comparing `spotify_web_downloader-1.6.2/PKG-INFO` & `spotify_web_downloader-1.6.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spotify-web-downloader
-Version: 1.6.2
+Version: 1.6.3
 Summary: Download songs/albums/playlists directly from Spotify in AAC
 Author: glomatico
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Requires-Dist: click
 Requires-Dist: pybase62
 Requires-Dist: pywidevine
```

