# Comparing `tmp/spotify_web_downloader-1.6.tar.gz` & `tmp/spotify_web_downloader-1.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spotify_web_downloader-1.6.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "spotify_web_downloader-1.6.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `spotify_web_downloader-1.6.tar` & `spotify_web_downloader-1.6.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0     1137 2024-04-02 17:45:37.913384 spotify_web_downloader-1.6/.github/workflows/main.yml
--rw-r--r--   0        0        0       96 2024-04-02 17:45:37.913384 spotify_web_downloader-1.6/.gitignore
--rw-r--r--   0        0        0     8410 2024-04-02 17:45:37.913384 spotify_web_downloader-1.6/README.md
--rw-r--r--   0        0        0      533 2024-04-02 17:45:37.913384 spotify_web_downloader-1.6/pyproject.toml
--rw-r--r--   0        0        0       40 2024-04-02 17:45:37.913384 spotify_web_downloader-1.6/requirements.txt
--rw-r--r--   0        0        0       20 2024-04-02 17:45:37.913384 spotify_web_downloader-1.6/spotify_web_downloader/__init__.py
--rw-r--r--   0        0        0       30 2024-04-02 17:45:37.913384 spotify_web_downloader-1.6/spotify_web_downloader/__main__.py
--rw-r--r--   0        0        0    21135 2024-04-02 17:45:37.913384 spotify_web_downloader-1.6/spotify_web_downloader/cli.py
--rw-r--r--   0        0        0      457 2024-04-02 17:45:37.913384 spotify_web_downloader-1.6/spotify_web_downloader/constants.py
--rw-r--r--   0        0        0     8459 2024-04-02 17:45:37.913384 spotify_web_downloader-1.6/spotify_web_downloader/downloader.py
--rw-r--r--   0        0        0    11132 2024-04-02 17:45:37.913384 spotify_web_downloader-1.6/spotify_web_downloader/downloader_music_video.py
--rw-r--r--   0        0        0     8729 2024-04-02 17:45:37.913384 spotify_web_downloader-1.6/spotify_web_downloader/downloader_song.py
--rw-r--r--   0        0        0      175 2024-04-02 17:45:37.913384 spotify_web_downloader-1.6/spotify_web_downloader/enums.py
--rw-r--r--   0        0        0     4015 2024-04-02 17:45:37.913384 spotify_web_downloader-1.6/spotify_web_downloader/hardcoded_wvd.py
--rw-r--r--   0        0        0      707 2024-04-02 17:45:37.913384 spotify_web_downloader-1.6/spotify_web_downloader/models.py
--rw-r--r--   0        0        0     7367 2024-04-02 17:45:37.913384 spotify_web_downloader-1.6/spotify_web_downloader/spotify_api.py
--rw-r--r--   0        0        0     8819 1970-01-01 00:00:00.000000 spotify_web_downloader-1.6/PKG-INFO
+-rw-r--r--   0        0        0     1137 2024-04-02 23:27:23.064091 spotify_web_downloader-1.6.1/.github/workflows/main.yml
+-rw-r--r--   0        0        0       96 2024-04-02 23:27:23.064091 spotify_web_downloader-1.6.1/.gitignore
+-rw-r--r--   0        0        0     8411 2024-04-02 23:27:23.064091 spotify_web_downloader-1.6.1/README.md
+-rw-r--r--   0        0        0      533 2024-04-02 23:27:23.064091 spotify_web_downloader-1.6.1/pyproject.toml
+-rw-r--r--   0        0        0       40 2024-04-02 23:27:23.064091 spotify_web_downloader-1.6.1/requirements.txt
+-rw-r--r--   0        0        0       22 2024-04-02 23:27:23.064091 spotify_web_downloader-1.6.1/spotify_web_downloader/__init__.py
+-rw-r--r--   0        0        0       30 2024-04-02 23:27:23.064091 spotify_web_downloader-1.6.1/spotify_web_downloader/__main__.py
+-rw-r--r--   0        0        0    21137 2024-04-02 23:27:23.064091 spotify_web_downloader-1.6.1/spotify_web_downloader/cli.py
+-rw-r--r--   0        0        0      457 2024-04-02 23:27:23.064091 spotify_web_downloader-1.6.1/spotify_web_downloader/constants.py
+-rw-r--r--   0        0        0     8546 2024-04-02 23:27:23.064091 spotify_web_downloader-1.6.1/spotify_web_downloader/downloader.py
+-rw-r--r--   0        0        0    11132 2024-04-02 23:27:23.064091 spotify_web_downloader-1.6.1/spotify_web_downloader/downloader_music_video.py
+-rw-r--r--   0        0        0     8729 2024-04-02 23:27:23.064091 spotify_web_downloader-1.6.1/spotify_web_downloader/downloader_song.py
+-rw-r--r--   0        0        0      177 2024-04-02 23:27:23.064091 spotify_web_downloader-1.6.1/spotify_web_downloader/enums.py
+-rw-r--r--   0        0        0     4015 2024-04-02 23:27:23.064091 spotify_web_downloader-1.6.1/spotify_web_downloader/hardcoded_wvd.py
+-rw-r--r--   0        0        0      707 2024-04-02 23:27:23.064091 spotify_web_downloader-1.6.1/spotify_web_downloader/models.py
+-rw-r--r--   0        0        0     7367 2024-04-02 23:27:23.064091 spotify_web_downloader-1.6.1/spotify_web_downloader/spotify_api.py
+-rw-r--r--   0        0        0     8822 1970-01-01 00:00:00.000000 spotify_web_downloader-1.6.1/PKG-INFO
```

### Comparing `spotify_web_downloader-1.6/.github/workflows/main.yml` & `spotify_web_downloader-1.6.1/.github/workflows/main.yml`

 * *Files identical despite different names*

### Comparing `spotify_web_downloader-1.6/README.md` & `spotify_web_downloader-1.6.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -54,15 +54,15 @@
 | `--date-tag-template` / `date_tag_template`                     | Date tag template.                                                           | `%Y-%m-%dT%H:%M:%SZ`                         |
 | `--exclude-tags` / `exclude_tags`                               | Comma-separated tags to exclude.                                             | `null`                                       |
 | `--truncate` / `truncate`                                       | Maximum length of the file/folder names.                                     | `40`                                         |
 | `--template-folder-album` / `template_folder_album`             | Template of the album folders as a format string.                            | `{album_artist}/{album}`                     |
 | `--template-folder-compilation` / `template_folder_compilation` | Template of the compilation album folders as a format string.                | `Compilations/{album}`                       |
 | `--template-file-single-disc` / `template_file_single_disc`     | Template of the song files for single-disc albums as a format string.        | `{track:02d} {title}`                        |
 | `--template-file-multi-disc` / `template_file_multi_disc`       | Template of the song files for multi-disc albums as a format string.         | `{disc}-{track:02d} {title}`                 |
-| `--download-mode-song` / `download_mode_song`                   | Download mode for songs.                                                     | `ydlp`                                       |
+| `--download-mode-song` / `download_mode_song`                   | Download mode for songs.                                                     | `ytdlp`                                      |
 | `--premium-quality`, `-p` / `premium_quality`                   | Download songs in premium quality.                                           | `false`                                      |
 | `--template-folder-music-video` / `template_folder_music_video` | Template of the music video folders as a format string.                      | `{artist}/Unknown Album`                     |
 | `--template-file-music-video` / `template_file_music_video`     | Template of the music video files as a format string.                        | `{title}`                                    |
 | `--download-mode-video` / `download_mode_video`                 | Download mode for videos.                                                    | `ydlp`                                       |
 | `--no-config-file`, `-n` / -                                    | Do not use a config file.                                                    | `false`                                      |
 
 ### Tag variables
@@ -84,21 +84,21 @@
 - `release_date`
 - `release_year`
 - `title`
 - `track`
 - `track_total`
 
 ### Music videos quality
-Music videos will be downloaded in the highest quality available in H.254/AAC, up to 1080p.
+Music videos will be downloaded in the highest quality available in H.264/AAC, up to 1080p.
 
 ### Download mode
 The following modes are available for songs:
 * `ytdlp`
 * `aria2c`
     * Faster than `ytdlp`
     * Can be obtained from here: https://github.com/aria2/aria2/releases
 
 The following modes are available for videos:
 * `ytdlp`
-* `nm38dlre`
+* `nm3u8dlre`
     * Faster than `ytdlp`
     * Can be obtained from here: https://github.com/nilaoda/N_m3u8DL-RE/releases
```

### Comparing `spotify_web_downloader-1.6/pyproject.toml` & `spotify_web_downloader-1.6.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `spotify_web_downloader-1.6/spotify_web_downloader/cli.py` & `spotify_web_downloader-1.6.1/spotify_web_downloader/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -308,15 +308,15 @@
     )
     downloader_music_video = DownloaderMusicVideo(
         downloader,
         template_folder_music_video,
         template_file_music_video,
         download_mode_video,
     )
-    if not no_lrc:
+    if not lrc_only:
         if wvd_path and not wvd_path.exists():
             logger.critical(X_NOT_FOUND_STRING.format(".wvd file", wvd_path))
             return
         logger.debug("Setting up CDM")
         downloader.set_cdm()
         if not downloader.ffmpeg_path_full:
             logger.critical(X_NOT_FOUND_STRING.format("ffmpeg", ffmpeg_path))
```

### Comparing `spotify_web_downloader-1.6/spotify_web_downloader/downloader.py` & `spotify_web_downloader-1.6.1/spotify_web_downloader/downloader.py`

 * *Files 1% similar despite different names*

```diff
@@ -173,17 +173,21 @@
 
     def apply_tags(self, fixed_location: Path, tags: dict, cover_url: str):
         mp4_tags = {
             v: [tags[k]]
             for k, v in MP4_TAGS_MAP.items()
             if k not in self.exclude_tags_list and tags.get(k) is not None
         }
-        if not {"track", "track_total"} & set(self.exclude_tags_list):
+        if not {"track", "track_total"} & set(self.exclude_tags_list) and tags.get(
+            "track"
+        ):
             mp4_tags["trkn"] = [[0, 0]]
-        if not {"disc", "disc_total"} & set(self.exclude_tags_list):
+        if not {"disc", "disc_total"} & set(self.exclude_tags_list) and tags.get(
+            "disc"
+        ):
             mp4_tags["disk"] = [[0, 0]]
         if (
             "compilation" not in self.exclude_tags_list
             and tags.get("compilation") is not None
         ):
             mp4_tags["cpil"] = tags["compilation"]
         if "cover" not in self.exclude_tags_list:
```

### Comparing `spotify_web_downloader-1.6/spotify_web_downloader/downloader_music_video.py` & `spotify_web_downloader-1.6.1/spotify_web_downloader/downloader_music_video.py`

 * *Files identical despite different names*

### Comparing `spotify_web_downloader-1.6/spotify_web_downloader/downloader_song.py` & `spotify_web_downloader-1.6.1/spotify_web_downloader/downloader_song.py`

 * *Files identical despite different names*

### Comparing `spotify_web_downloader-1.6/spotify_web_downloader/hardcoded_wvd.py` & `spotify_web_downloader-1.6.1/spotify_web_downloader/hardcoded_wvd.py`

 * *Files identical despite different names*

### Comparing `spotify_web_downloader-1.6/spotify_web_downloader/models.py` & `spotify_web_downloader-1.6.1/spotify_web_downloader/models.py`

 * *Files identical despite different names*

### Comparing `spotify_web_downloader-1.6/spotify_web_downloader/spotify_api.py` & `spotify_web_downloader-1.6.1/spotify_web_downloader/spotify_api.py`

 * *Files identical despite different names*

### Comparing `spotify_web_downloader-1.6/PKG-INFO` & `spotify_web_downloader-1.6.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spotify-web-downloader
-Version: 1.6
+Version: 1.6.1
 Summary: Download songs/albums/playlists directly from Spotify in AAC
 Author: glomatico
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Requires-Dist: click
 Requires-Dist: pybase62
 Requires-Dist: pywidevine
@@ -68,15 +68,15 @@
 | `--date-tag-template` / `date_tag_template`                     | Date tag template.                                                           | `%Y-%m-%dT%H:%M:%SZ`                         |
 | `--exclude-tags` / `exclude_tags`                               | Comma-separated tags to exclude.                                             | `null`                                       |
 | `--truncate` / `truncate`                                       | Maximum length of the file/folder names.                                     | `40`                                         |
 | `--template-folder-album` / `template_folder_album`             | Template of the album folders as a format string.                            | `{album_artist}/{album}`                     |
 | `--template-folder-compilation` / `template_folder_compilation` | Template of the compilation album folders as a format string.                | `Compilations/{album}`                       |
 | `--template-file-single-disc` / `template_file_single_disc`     | Template of the song files for single-disc albums as a format string.        | `{track:02d} {title}`                        |
 | `--template-file-multi-disc` / `template_file_multi_disc`       | Template of the song files for multi-disc albums as a format string.         | `{disc}-{track:02d} {title}`                 |
-| `--download-mode-song` / `download_mode_song`                   | Download mode for songs.                                                     | `ydlp`                                       |
+| `--download-mode-song` / `download_mode_song`                   | Download mode for songs.                                                     | `ytdlp`                                      |
 | `--premium-quality`, `-p` / `premium_quality`                   | Download songs in premium quality.                                           | `false`                                      |
 | `--template-folder-music-video` / `template_folder_music_video` | Template of the music video folders as a format string.                      | `{artist}/Unknown Album`                     |
 | `--template-file-music-video` / `template_file_music_video`     | Template of the music video files as a format string.                        | `{title}`                                    |
 | `--download-mode-video` / `download_mode_video`                 | Download mode for videos.                                                    | `ydlp`                                       |
 | `--no-config-file`, `-n` / -                                    | Do not use a config file.                                                    | `false`                                      |
 
 ### Tag variables
@@ -98,22 +98,22 @@
 - `release_date`
 - `release_year`
 - `title`
 - `track`
 - `track_total`
 
 ### Music videos quality
-Music videos will be downloaded in the highest quality available in H.254/AAC, up to 1080p.
+Music videos will be downloaded in the highest quality available in H.264/AAC, up to 1080p.
 
 ### Download mode
 The following modes are available for songs:
 * `ytdlp`
 * `aria2c`
     * Faster than `ytdlp`
     * Can be obtained from here: https://github.com/aria2/aria2/releases
 
 The following modes are available for videos:
 * `ytdlp`
-* `nm38dlre`
+* `nm3u8dlre`
     * Faster than `ytdlp`
     * Can be obtained from here: https://github.com/nilaoda/N_m3u8DL-RE/releases
```

