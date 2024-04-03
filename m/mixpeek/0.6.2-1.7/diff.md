# Comparing `tmp/mixpeek-0.6.2.tar.gz` & `tmp/mixpeek-1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mixpeek-0.6.2.tar", max compression
+gzip compressed data, was "mixpeek-1.7.tar", last modified: Mon Jan  2 17:08:37 2023, max compression
```

## Comparing `mixpeek-0.6.2.tar` & `mixpeek-1.7.tar`

### file list

```diff
@@ -1,78 +1,15 @@
--rw-r--r--   0        0        0     1064 2024-04-03 15:17:17.536929 mixpeek-0.6.2/LICENSE
--rw-r--r--   0        0        0     3495 2024-04-03 15:17:17.536929 mixpeek-0.6.2/README.md
--rw-r--r--   0        0        0      592 2024-04-03 15:17:17.536929 mixpeek-0.6.2/pyproject.toml
--rw-r--r--   0        0        0     2000 2024-04-03 15:17:17.536929 mixpeek-0.6.2/src/mixpeek/__init__.py
--rw-r--r--   0        0        0     7338 2024-04-03 15:17:17.536929 mixpeek-0.6.2/src/mixpeek/base_client.py
--rw-r--r--   0        0        0     2064 2024-04-03 15:17:17.536929 mixpeek-0.6.2/src/mixpeek/client.py
--rw-r--r--   0        0        0      790 2024-04-03 15:17:17.536929 mixpeek-0.6.2/src/mixpeek/core/__init__.py
--rw-r--r--   0        0        0      426 2024-04-03 15:17:17.536929 mixpeek-0.6.2/src/mixpeek/core/api_error.py
--rw-r--r--   0        0        0     2622 2024-04-03 15:17:17.536929 mixpeek-0.6.2/src/mixpeek/core/client_wrapper.py
--rw-r--r--   0        0        0     1047 2024-04-03 15:17:17.536929 mixpeek-0.6.2/src/mixpeek/core/datetime_utils.py
--rw-r--r--   0        0        0     1480 2024-04-03 15:17:17.536929 mixpeek-0.6.2/src/mixpeek/core/file.py
--rw-r--r--   0        0        0     5059 2024-04-03 15:17:17.536929 mixpeek-0.6.2/src/mixpeek/core/http_client.py
--rw-r--r--   0        0        0     3799 2024-04-03 15:17:17.536929 mixpeek-0.6.2/src/mixpeek/core/jsonable_encoder.py
--rw-r--r--   0        0        0      330 2024-04-03 15:17:17.540930 mixpeek-0.6.2/src/mixpeek/core/remove_none_from_dict.py
--rw-r--r--   0        0        0     1420 2024-04-03 15:17:17.540930 mixpeek-0.6.2/src/mixpeek/core/request_options.py
--rw-r--r--   0        0        0       65 2024-04-03 15:17:17.540930 mixpeek-0.6.2/src/mixpeek/embed/__init__.py
--rw-r--r--   0        0        0    16086 2024-04-03 15:17:17.540930 mixpeek-0.6.2/src/mixpeek/embed/client.py
--rw-r--r--   0        0        0      156 2024-04-03 15:17:17.540930 mixpeek-0.6.2/src/mixpeek/environment.py
--rw-r--r--   0        0        0      534 2024-04-03 15:17:17.540930 mixpeek-0.6.2/src/mixpeek/errors/__init__.py
--rw-r--r--   0        0        0      285 2024-04-03 15:17:17.540930 mixpeek-0.6.2/src/mixpeek/errors/bad_request_error.py
--rw-r--r--   0        0        0      284 2024-04-03 15:17:17.540930 mixpeek-0.6.2/src/mixpeek/errors/forbidden_error.py
--rw-r--r--   0        0        0      289 2024-04-03 15:17:17.540930 mixpeek-0.6.2/src/mixpeek/errors/internal_server_error.py
--rw-r--r--   0        0        0      283 2024-04-03 15:17:17.540930 mixpeek-0.6.2/src/mixpeek/errors/not_found_error.py
--rw-r--r--   0        0        0      287 2024-04-03 15:17:17.540930 mixpeek-0.6.2/src/mixpeek/errors/unauthorized_error.py
--rw-r--r--   0        0        0      313 2024-04-03 15:17:17.540930 mixpeek-0.6.2/src/mixpeek/errors/unprocessable_entity_error.py
--rw-r--r--   0        0        0       65 2024-04-03 15:17:17.540930 mixpeek-0.6.2/src/mixpeek/extract/__init__.py
--rw-r--r--   0        0        0    15158 2024-04-03 15:17:17.540930 mixpeek-0.6.2/src/mixpeek/extract/client.py
--rw-r--r--   0        0        0       65 2024-04-03 15:17:17.540930 mixpeek-0.6.2/src/mixpeek/generators/__init__.py
--rw-r--r--   0        0        0    10251 2024-04-03 15:17:17.540930 mixpeek-0.6.2/src/mixpeek/generators/client.py
--rw-r--r--   0        0        0       65 2024-04-03 15:17:17.540930 mixpeek-0.6.2/src/mixpeek/parse/__init__.py
--rw-r--r--   0        0        0     4717 2024-04-03 15:17:17.540930 mixpeek-0.6.2/src/mixpeek/parse/client.py
--rw-r--r--   0        0        0      279 2024-04-03 15:17:17.540930 mixpeek-0.6.2/src/mixpeek/parse_client.py
--rw-r--r--   0        0        0       65 2024-04-03 15:17:17.540930 mixpeek-0.6.2/src/mixpeek/pipelines/__init__.py
--rw-r--r--   0        0        0    22360 2024-04-03 15:17:17.540930 mixpeek-0.6.2/src/mixpeek/pipelines/client.py
--rw-r--r--   0        0        0        0 2024-04-03 15:17:17.540930 mixpeek-0.6.2/src/mixpeek/py.typed
--rw-r--r--   0        0        0       65 2024-04-03 15:17:17.540930 mixpeek-0.6.2/src/mixpeek/storage/__init__.py
--rw-r--r--   0        0        0    12609 2024-04-03 15:17:17.540930 mixpeek-0.6.2/src/mixpeek/storage/client.py
--rw-r--r--   0        0        0     2060 2024-04-03 15:17:17.540930 mixpeek-0.6.2/src/mixpeek/types/__init__.py
--rw-r--r--   0        0        0     1013 2024-04-03 15:17:17.540930 mixpeek-0.6.2/src/mixpeek/types/api_key.py
--rw-r--r--   0        0        0      939 2024-04-03 15:17:17.540930 mixpeek-0.6.2/src/mixpeek/types/audio_params.py
--rw-r--r--   0        0        0      959 2024-04-03 15:17:17.540930 mixpeek-0.6.2/src/mixpeek/types/configs_response.py
--rw-r--r--   0        0        0     1144 2024-04-03 15:17:17.540930 mixpeek-0.6.2/src/mixpeek/types/connection.py
--rw-r--r--   0        0        0      168 2024-04-03 15:17:17.540930 mixpeek-0.6.2/src/mixpeek/types/connection_engine.py
--rw-r--r--   0        0        0      938 2024-04-03 15:17:17.540930 mixpeek-0.6.2/src/mixpeek/types/csv_params.py
--rw-r--r--   0        0        0      945 2024-04-03 15:17:17.540930 mixpeek-0.6.2/src/mixpeek/types/destination.py
--rw-r--r--   0        0        0      955 2024-04-03 15:17:17.540930 mixpeek-0.6.2/src/mixpeek/types/embedding_response.py
--rw-r--r--   0        0        0      905 2024-04-03 15:17:17.540930 mixpeek-0.6.2/src/mixpeek/types/error_message.py
--rw-r--r--   0        0        0      995 2024-04-03 15:17:17.540930 mixpeek-0.6.2/src/mixpeek/types/error_response.py
--rw-r--r--   0        0        0      160 2024-04-03 15:17:17.540930 mixpeek-0.6.2/src/mixpeek/types/field_type.py
--rw-r--r--   0        0        0     1117 2024-04-03 15:17:17.540930 mixpeek-0.6.2/src/mixpeek/types/generation_response.py
--rw-r--r--   0        0        0      949 2024-04-03 15:17:17.540930 mixpeek-0.6.2/src/mixpeek/types/html_params.py
--rw-r--r--   0        0        0     1010 2024-04-03 15:17:17.540930 mixpeek-0.6.2/src/mixpeek/types/http_validation_error.py
--rw-r--r--   0        0        0     1070 2024-04-03 15:17:17.540930 mixpeek-0.6.2/src/mixpeek/types/image_params.py
--rw-r--r--   0        0        0      918 2024-04-03 15:17:17.540930 mixpeek-0.6.2/src/mixpeek/types/message.py
--rw-r--r--   0        0        0     1147 2024-04-03 15:17:17.540930 mixpeek-0.6.2/src/mixpeek/types/metadata.py
--rw-r--r--   0        0        0      170 2024-04-03 15:17:17.540930 mixpeek-0.6.2/src/mixpeek/types/modality.py
--rw-r--r--   0        0        0      948 2024-04-03 15:17:17.540930 mixpeek-0.6.2/src/mixpeek/types/model.py
--rw-r--r--   0        0        0      173 2024-04-03 15:17:17.540930 mixpeek-0.6.2/src/mixpeek/types/models.py
--rw-r--r--   0        0        0     1646 2024-04-03 15:17:17.540930 mixpeek-0.6.2/src/mixpeek/types/pdf_params.py
--rw-r--r--   0        0        0      888 2024-04-03 15:17:17.540930 mixpeek-0.6.2/src/mixpeek/types/ppt_params.py
--rw-r--r--   0        0        0      889 2024-04-03 15:17:17.540930 mixpeek-0.6.2/src/mixpeek/types/pptx_params.py
--rw-r--r--   0        0        0     1223 2024-04-03 15:17:17.540930 mixpeek-0.6.2/src/mixpeek/types/settings.py
--rw-r--r--   0        0        0      998 2024-04-03 15:17:17.540930 mixpeek-0.6.2/src/mixpeek/types/source.py
--rw-r--r--   0        0        0     1041 2024-04-03 15:17:17.540930 mixpeek-0.6.2/src/mixpeek/types/source_destination_mapping.py
--rw-r--r--   0        0        0      888 2024-04-03 15:17:17.540930 mixpeek-0.6.2/src/mixpeek/types/txt_params.py
--rw-r--r--   0        0        0     1249 2024-04-03 15:17:17.540930 mixpeek-0.6.2/src/mixpeek/types/user.py
--rw-r--r--   0        0        0     1029 2024-04-03 15:17:17.540930 mixpeek-0.6.2/src/mixpeek/types/validation_error.py
--rw-r--r--   0        0        0      128 2024-04-03 15:17:17.540930 mixpeek-0.6.2/src/mixpeek/types/validation_error_loc_item.py
--rw-r--r--   0        0        0      890 2024-04-03 15:17:17.540930 mixpeek-0.6.2/src/mixpeek/types/video_params.py
--rw-r--r--   0        0        0     1059 2024-04-03 15:17:17.540930 mixpeek-0.6.2/src/mixpeek/types/workflow_response.py
--rw-r--r--   0        0        0     1003 2024-04-03 15:17:17.540930 mixpeek-0.6.2/src/mixpeek/types/workflow_settings.py
--rw-r--r--   0        0        0      939 2024-04-03 15:17:17.540930 mixpeek-0.6.2/src/mixpeek/types/xlsx_params.py
--rw-r--r--   0        0        0       65 2024-04-03 15:17:17.540930 mixpeek-0.6.2/src/mixpeek/users/__init__.py
--rw-r--r--   0        0        0    14911 2024-04-03 15:17:17.540930 mixpeek-0.6.2/src/mixpeek/users/client.py
--rw-r--r--   0        0        0       75 2024-04-03 15:17:17.540930 mixpeek-0.6.2/src/mixpeek/version.py
--rw-r--r--   0        0        0       65 2024-04-03 15:17:17.540930 mixpeek-0.6.2/src/mixpeek/workflows/__init__.py
--rw-r--r--   0        0        0    24370 2024-04-03 15:17:17.540930 mixpeek-0.6.2/src/mixpeek/workflows/client.py
--rw-r--r--   0        0        0     3985 1970-01-01 00:00:00.000000 mixpeek-0.6.2/PKG-INFO
+drwxr-xr-x   0 ethan      (501) staff       (20)        0 2023-01-02 17:08:37.484937 mixpeek-1.7/
+-rw-r--r--   0 ethan      (501) staff       (20)     1072 2021-09-16 16:21:14.000000 mixpeek-1.7/LICENSE.rst
+-rw-r--r--   0 ethan      (501) staff       (20)       34 2021-10-14 01:21:10.000000 mixpeek-1.7/MANIFEST.in
+-rw-r--r--   0 ethan      (501) staff       (20)      254 2023-01-02 17:08:37.485030 mixpeek-1.7/PKG-INFO
+-rw-r--r--   0 ethan      (501) staff       (20)     5027 2022-12-22 16:06:52.000000 mixpeek-1.7/README.md
+drwxr-xr-x   0 ethan      (501) staff       (20)        0 2023-01-02 17:08:37.483629 mixpeek-1.7/mixpeek/
+-rw-r--r--   0 ethan      (501) staff       (20)     2740 2023-01-02 17:04:38.000000 mixpeek-1.7/mixpeek/__init__.py
+drwxr-xr-x   0 ethan      (501) staff       (20)        0 2023-01-02 17:08:37.484767 mixpeek-1.7/mixpeek.egg-info/
+-rw-r--r--   0 ethan      (501) staff       (20)      254 2023-01-02 17:08:37.000000 mixpeek-1.7/mixpeek.egg-info/PKG-INFO
+-rw-r--r--   0 ethan      (501) staff       (20)      226 2023-01-02 17:08:37.000000 mixpeek-1.7/mixpeek.egg-info/SOURCES.txt
+-rw-r--r--   0 ethan      (501) staff       (20)        1 2023-01-02 17:08:37.000000 mixpeek-1.7/mixpeek.egg-info/dependency_links.txt
+-rw-r--r--   0 ethan      (501) staff       (20)        9 2023-01-02 17:08:37.000000 mixpeek-1.7/mixpeek.egg-info/requires.txt
+-rw-r--r--   0 ethan      (501) staff       (20)        8 2023-01-02 17:08:37.000000 mixpeek-1.7/mixpeek.egg-info/top_level.txt
+-rw-r--r--   0 ethan      (501) staff       (20)      107 2023-01-02 17:08:37.485362 mixpeek-1.7/setup.cfg
+-rw-r--r--   0 ethan      (501) staff       (20)      368 2023-01-02 17:08:31.000000 mixpeek-1.7/setup.py
```

### Comparing `mixpeek-0.6.2/LICENSE` & `mixpeek-1.7/LICENSE.rst`

 * *Files 26% similar despite different names*

```diff
@@ -1,21 +1,20 @@
-MIT License
-
-Copyright (c) 2024 Mixpeek.
+The MIT License (MIT)
+Copyright (c) 2021 mixpeek
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
 
 The above copyright notice and this permission notice shall be included in all
 copies or substantial portions of the Software.
 
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND,
+EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF
+MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT.
+IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM,
+DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR
+OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE
+OR OTHER DEALINGS IN THE SOFTWARE.
```

