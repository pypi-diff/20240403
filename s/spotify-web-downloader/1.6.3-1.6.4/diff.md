# Comparing `tmp/spotify_web_downloader-1.6.3.tar.gz` & `tmp/spotify_web_downloader-1.6.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spotify_web_downloader-1.6.3.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "spotify_web_downloader-1.6.4.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `spotify_web_downloader-1.6.3.tar` & `spotify_web_downloader-1.6.4.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0     1137 2024-04-03 13:01:18.141462 spotify_web_downloader-1.6.3/.github/workflows/main.yml
--rw-r--r--   0        0        0       96 2024-04-03 13:01:18.141462 spotify_web_downloader-1.6.3/.gitignore
--rw-r--r--   0        0        0     8437 2024-04-03 13:01:18.141462 spotify_web_downloader-1.6.3/README.md
--rw-r--r--   0        0        0      533 2024-04-03 13:01:18.145462 spotify_web_downloader-1.6.3/pyproject.toml
--rw-r--r--   0        0        0       40 2024-04-03 13:01:18.145462 spotify_web_downloader-1.6.3/requirements.txt
--rw-r--r--   0        0        0       22 2024-04-03 13:01:18.145462 spotify_web_downloader-1.6.3/spotify_web_downloader/__init__.py
--rw-r--r--   0        0        0       30 2024-04-03 13:01:18.145462 spotify_web_downloader-1.6.3/spotify_web_downloader/__main__.py
--rw-r--r--   0        0        0    21483 2024-04-03 13:01:18.145462 spotify_web_downloader-1.6.3/spotify_web_downloader/cli.py
--rw-r--r--   0        0        0      507 2024-04-03 13:01:18.145462 spotify_web_downloader-1.6.3/spotify_web_downloader/constants.py
--rw-r--r--   0        0        0     8546 2024-04-03 13:01:18.145462 spotify_web_downloader-1.6.3/spotify_web_downloader/downloader.py
--rw-r--r--   0        0        0    11657 2024-04-03 13:01:18.145462 spotify_web_downloader-1.6.3/spotify_web_downloader/downloader_music_video.py
--rw-r--r--   0        0        0     9254 2024-04-03 13:01:18.145462 spotify_web_downloader-1.6.3/spotify_web_downloader/downloader_song.py
--rw-r--r--   0        0        0      177 2024-04-03 13:01:18.145462 spotify_web_downloader-1.6.3/spotify_web_downloader/enums.py
--rw-r--r--   0        0        0     4015 2024-04-03 13:01:18.145462 spotify_web_downloader-1.6.3/spotify_web_downloader/hardcoded_wvd.py
--rw-r--r--   0        0        0      707 2024-04-03 13:01:18.145462 spotify_web_downloader-1.6.3/spotify_web_downloader/models.py
--rw-r--r--   0        0        0     7738 2024-04-03 13:01:18.145462 spotify_web_downloader-1.6.3/spotify_web_downloader/spotify_api.py
--rw-r--r--   0        0        0     8848 1970-01-01 00:00:00.000000 spotify_web_downloader-1.6.3/PKG-INFO
+-rw-r--r--   0        0        0     1137 2024-04-03 16:20:28.923047 spotify_web_downloader-1.6.4/.github/workflows/main.yml
+-rw-r--r--   0        0        0       96 2024-04-03 16:20:28.923047 spotify_web_downloader-1.6.4/.gitignore
+-rw-r--r--   0        0        0     8433 2024-04-03 16:20:28.923047 spotify_web_downloader-1.6.4/README.md
+-rw-r--r--   0        0        0      533 2024-04-03 16:20:28.923047 spotify_web_downloader-1.6.4/pyproject.toml
+-rw-r--r--   0        0        0       40 2024-04-03 16:20:28.923047 spotify_web_downloader-1.6.4/requirements.txt
+-rw-r--r--   0        0        0       22 2024-04-03 16:20:28.923047 spotify_web_downloader-1.6.4/spotify_web_downloader/__init__.py
+-rw-r--r--   0        0        0       30 2024-04-03 16:20:28.923047 spotify_web_downloader-1.6.4/spotify_web_downloader/__main__.py
+-rw-r--r--   0        0        0    21551 2024-04-03 16:20:28.923047 spotify_web_downloader-1.6.4/spotify_web_downloader/cli.py
+-rw-r--r--   0        0        0      507 2024-04-03 16:20:28.923047 spotify_web_downloader-1.6.4/spotify_web_downloader/constants.py
+-rw-r--r--   0        0        0     8546 2024-04-03 16:20:28.927047 spotify_web_downloader-1.6.4/spotify_web_downloader/downloader.py
+-rw-r--r--   0        0        0    11644 2024-04-03 16:20:28.927047 spotify_web_downloader-1.6.4/spotify_web_downloader/downloader_music_video.py
+-rw-r--r--   0        0        0     9241 2024-04-03 16:20:28.927047 spotify_web_downloader-1.6.4/spotify_web_downloader/downloader_song.py
+-rw-r--r--   0        0        0      177 2024-04-03 16:20:28.927047 spotify_web_downloader-1.6.4/spotify_web_downloader/enums.py
+-rw-r--r--   0        0        0     4015 2024-04-03 16:20:28.927047 spotify_web_downloader-1.6.4/spotify_web_downloader/hardcoded_wvd.py
+-rw-r--r--   0        0        0      707 2024-04-03 16:20:28.927047 spotify_web_downloader-1.6.4/spotify_web_downloader/models.py
+-rw-r--r--   0        0        0     7738 2024-04-03 16:20:28.927047 spotify_web_downloader-1.6.4/spotify_web_downloader/spotify_api.py
+-rw-r--r--   0        0        0     8844 1970-01-01 00:00:00.000000 spotify_web_downloader-1.6.4/PKG-INFO
```

### Comparing `spotify_web_downloader-1.6.3/.github/workflows/main.yml` & `spotify_web_downloader-1.6.4/.github/workflows/main.yml`

 * *Files identical despite different names*

### Comparing `spotify_web_downloader-1.6.3/README.md` & `spotify_web_downloader-1.6.4/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -66,15 +66,14 @@
 | `--no-config-file`, `-n` / -                                    | Do not use a config file.                                                    | `false`                                      |
 
 ### Tag variables
 The following variables can be used in the template folder/file and/or in the `exclude_tags` list:
 - `album`
 - `album_artist`
 - `artist`
-- `comment`
 - `compilation`
 - `composer`
 - `copyright`
 - `cover`
 - `disc`
 - `disc_total`
 - `isrc`
@@ -84,14 +83,15 @@
 - `producer`
 - `rating`
 - `release_date`
 - `release_year`
 - `title`
 - `track`
 - `track_total`
+- `url`
 
 ### Music videos quality
 Music videos will be downloaded in the highest quality available in H.264/AAC, up to 1080p.
 
 ### Download mode
 The following modes are available for songs:
 * `ytdlp`
```

### Comparing `spotify_web_downloader-1.6.3/pyproject.toml` & `spotify_web_downloader-1.6.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `spotify_web_downloader-1.6.3/spotify_web_downloader/cli.py` & `spotify_web_downloader-1.6.4/spotify_web_downloader/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -394,14 +394,15 @@
                     logger.debug("Getting track credits")
                     track_credits = spotify_api.get_track_credits(track_id)
                     tags = downloader_song.get_tags(
                         metadata_gid,
                         album_metadata,
                         track_credits,
                         lyrics.unsynced,
+                        track_id,
                     )
                     final_path = downloader_song.get_final_path(tags)
                     lrc_path = downloader_song.get_lrc_path(final_path)
                     cover_path = downloader_song.get_cover_path(final_path)
                     cover_url = downloader.get_cover_url(metadata_gid, "LARGE")
                     if lrc_only:
                         pass
@@ -473,14 +474,15 @@
                     )
                     logger.debug("Getting track credits")
                     track_credits = spotify_api.get_track_credits(track_id)
                     tags = downloader_music_video.get_tags(
                         metadata_gid,
                         album_metadata,
                         track_credits,
+                        track_id,
                     )
                     final_path = downloader_music_video.get_final_path(tags)
                     cover_path = downloader_music_video.get_cover_path(final_path)
                     if final_path.exists() and not overwrite:
                         logger.warning(
                             f'({queue_progress}) Music video already exists at "{final_path}", skipping'
                         )
```

### Comparing `spotify_web_downloader-1.6.3/spotify_web_downloader/downloader.py` & `spotify_web_downloader-1.6.4/spotify_web_downloader/downloader.py`

 * *Files identical despite different names*

### Comparing `spotify_web_downloader-1.6.3/spotify_web_downloader/downloader_music_video.py` & `spotify_web_downloader-1.6.4/spotify_web_downloader/downloader_music_video.py`

 * *Files 2% similar despite different names*

```diff
@@ -200,14 +200,15 @@
         m3u8_path.write_text(m3u8_str)
 
     def get_tags(
         self,
         metadata_gid: dict,
         album_metadata: dict,
         track_credits: dict,
+        track_id: str,
     ) -> dict:
         isrc = None
         if metadata_gid.get("external_id"):
             isrc = next(
                 (i for i in metadata_gid["external_id"] if i["type"] == "isrc"), None
             )
         release_date_datetime_obj = self.downloader.get_release_date_datetime_obj(
@@ -235,15 +236,15 @@
             "media_type": 6,
             "producer": self.downloader.get_artist(producers) if producers else None,
             "rating": 1 if metadata_gid.get("explicit") else 0,
             "title": album_metadata["name"],
             "release_date": self.downloader.get_release_date_tag(
                 release_date_datetime_obj
             ),
-            "url": f'https://open.spotify.com/track/{metadata_gid["canonical_uri"].split(":")[-1]}',
+            "url": f"https://open.spotify.com/track/{track_id}",
         }
         tags["release_year"] = str(release_date_datetime_obj.year)
         return tags
 
     def download(self, m3u8_path: Path, encrypted_path: str):
         if self.download_mode == DownloadModeVideo.YTDLP:
             self.download_ytdlp(m3u8_path, encrypted_path)
```

### Comparing `spotify_web_downloader-1.6.3/spotify_web_downloader/downloader_song.py` & `spotify_web_downloader-1.6.4/spotify_web_downloader/downloader_song.py`

 * *Files 2% similar despite different names*

```diff
@@ -85,14 +85,15 @@
 
     def get_tags(
         self,
         metadata_gid: dict,
         album_metadata: dict,
         track_credits: dict,
         lyrics_unsynced: str,
+        track_id: str,
     ) -> dict:
         isrc = None
         if metadata_gid.get("external_id"):
             isrc = next(
                 (i for i in metadata_gid["external_id"] if i["type"] == "isrc"), None
             )
         release_date_datetime_obj = self.downloader.get_release_date_datetime_obj(
@@ -135,15 +136,15 @@
             "title": metadata_gid["name"],
             "track": metadata_gid["number"],
             "track_total": max(
                 i["track_number"]
                 for i in album_metadata["tracks"]["items"]
                 if i["disc_number"] == metadata_gid["disc_number"]
             ),
-            "url": f'https://open.spotify.com/track/{metadata_gid["canonical_uri"].split(":")[-1]}',
+            "url": f"https://open.spotify.com/track/{track_id}",
         }
         return tags
 
     def download(self, encrypted_path: Path, stream_url: str):
         if self.download_mode == DownloadModeSong.YTDLP:
             self.download_ytdlp(encrypted_path, stream_url)
         elif self.download_mode == DownloadModeSong.ARIA2C:
```

### Comparing `spotify_web_downloader-1.6.3/spotify_web_downloader/hardcoded_wvd.py` & `spotify_web_downloader-1.6.4/spotify_web_downloader/hardcoded_wvd.py`

 * *Files identical despite different names*

### Comparing `spotify_web_downloader-1.6.3/spotify_web_downloader/models.py` & `spotify_web_downloader-1.6.4/spotify_web_downloader/models.py`

 * *Files identical despite different names*

### Comparing `spotify_web_downloader-1.6.3/spotify_web_downloader/spotify_api.py` & `spotify_web_downloader-1.6.4/spotify_web_downloader/spotify_api.py`

 * *Files identical despite different names*

### Comparing `spotify_web_downloader-1.6.3/PKG-INFO` & `spotify_web_downloader-1.6.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spotify-web-downloader
-Version: 1.6.3
+Version: 1.6.4
 Summary: Download songs/albums/playlists directly from Spotify in AAC
 Author: glomatico
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Requires-Dist: click
 Requires-Dist: pybase62
 Requires-Dist: pywidevine
@@ -80,15 +80,14 @@
 | `--no-config-file`, `-n` / -                                    | Do not use a config file.                                                    | `false`                                      |
 
 ### Tag variables
 The following variables can be used in the template folder/file and/or in the `exclude_tags` list:
 - `album`
 - `album_artist`
 - `artist`
-- `comment`
 - `compilation`
 - `composer`
 - `copyright`
 - `cover`
 - `disc`
 - `disc_total`
 - `isrc`
@@ -98,14 +97,15 @@
 - `producer`
 - `rating`
 - `release_date`
 - `release_year`
 - `title`
 - `track`
 - `track_total`
+- `url`
 
 ### Music videos quality
 Music videos will be downloaded in the highest quality available in H.264/AAC, up to 1080p.
 
 ### Download mode
 The following modes are available for songs:
 * `ytdlp`
```

