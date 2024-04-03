# Comparing `tmp/commonmeta_py-0.9.3.tar.gz` & `tmp/commonmeta_py-0.9.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "commonmeta_py-0.9.3.tar", max compression
+gzip compressed data, was "commonmeta_py-0.9.4.tar", max compression
```

## Comparing `commonmeta_py-0.9.3.tar` & `commonmeta_py-0.9.4.tar`

### file list

```diff
@@ -1,44 +1,44 @@
--rw-r--r--   0        0        0     1074 2023-02-21 06:38:55.700800 commonmeta_py-0.9.3/LICENSE
--rw-r--r--   0        0        0     6008 2023-09-14 14:09:22.921689 commonmeta_py-0.9.3/README.md
--rw-r--r--   0        0        0     1658 2023-09-14 17:49:33.421252 commonmeta_py-0.9.3/commonmeta/__init__.py
--rw-r--r--   0        0        0     9054 2024-01-13 23:45:30.203394 commonmeta_py-0.9.3/commonmeta/author_utils.py
--rw-r--r--   0        0        0     3323 2023-03-09 16:29:03.609320 commonmeta_py-0.9.3/commonmeta/base_utils.py
--rw-r--r--   0        0        0    14627 2023-09-12 13:01:04.530045 commonmeta_py-0.9.3/commonmeta/constants.py
--rw-r--r--   0        0        0     5452 2024-01-14 14:15:37.527705 commonmeta_py-0.9.3/commonmeta/date_utils.py
--rw-r--r--   0        0        0     3576 2023-03-06 11:26:51.937608 commonmeta_py-0.9.3/commonmeta/doi_utils.py
--rw-r--r--   0        0        0       56 2023-02-14 15:23:28.688206 commonmeta_py-0.9.3/commonmeta/metadata/__init__.py
--rw-r--r--   0        0        0     6899 2024-01-13 21:29:54.586698 commonmeta_py-0.9.3/commonmeta/metadata/metadata.py
--rw-r--r--   0        0        0      709 2024-01-13 14:11:52.569516 commonmeta_py-0.9.3/commonmeta/readers/__init__.py
--rw-r--r--   0        0        0        0 2023-02-19 09:38:13.587826 commonmeta_py-0.9.3/commonmeta/readers/bibtex_reader.py
--rw-r--r--   0        0        0     6053 2023-09-09 09:47:03.762792 commonmeta_py-0.9.3/commonmeta/readers/cff_reader.py
--rw-r--r--   0        0        0     3656 2023-09-10 10:19:10.546283 commonmeta_py-0.9.3/commonmeta/readers/codemeta_reader.py
--rw-r--r--   0        0        0      302 2024-01-13 14:13:06.635867 commonmeta_py-0.9.3/commonmeta/readers/commonmeta_reader.py
--rw-r--r--   0        0        0     9871 2023-09-11 10:08:16.995435 commonmeta_py-0.9.3/commonmeta/readers/crossref_reader.py
--rw-r--r--   0        0        0    20462 2023-09-11 09:32:48.588180 commonmeta_py-0.9.3/commonmeta/readers/crossref_xml_reader.py
--rw-r--r--   0        0        0     2584 2023-09-09 11:07:35.317858 commonmeta_py-0.9.3/commonmeta/readers/csl_reader.py
--rw-r--r--   0        0        0     5126 2024-01-14 14:38:04.826859 commonmeta_py-0.9.3/commonmeta/readers/datacite_reader.py
--rw-r--r--   0        0        0    11367 2024-01-14 14:37:56.867392 commonmeta_py-0.9.3/commonmeta/readers/datacite_xml_reader.py
--rw-r--r--   0        0        0     6773 2024-01-14 13:24:11.794486 commonmeta_py-0.9.3/commonmeta/readers/inveniordm_reader.py
--rw-r--r--   0        0        0     4501 2023-09-11 12:02:15.815494 commonmeta_py-0.9.3/commonmeta/readers/json_feed_reader.py
--rw-r--r--   0        0        0     7173 2023-09-12 12:07:23.937528 commonmeta_py-0.9.3/commonmeta/readers/kbase_reader.py
--rw-r--r--   0        0        0     4029 2023-02-26 13:06:27.824291 commonmeta_py-0.9.3/commonmeta/readers/ris_reader.py
--rw-r--r--   0        0        0    12685 2024-01-14 14:41:57.216355 commonmeta_py-0.9.3/commonmeta/readers/schema_org_reader.py
--rw-r--r--   0        0        0   855312 2023-03-03 21:07:36.789294 commonmeta_py-0.9.3/commonmeta/resources/cff_v1.2.0.json
--rw-r--r--   0        0        0    15070 2024-01-13 12:57:44.454997 commonmeta_py-0.9.3/commonmeta/resources/commonmeta_v0.10.5.json
--rw-r--r--   0        0        0    12166 2023-03-03 21:30:37.485484 commonmeta_py-0.9.3/commonmeta/resources/csl-data.json
--rw-r--r--   0        0        0    16650 2023-02-28 03:11:41.977630 commonmeta_py-0.9.3/commonmeta/resources/datacite-v4.json
--rw-r--r--   0        0        0   228225 2023-03-03 21:24:04.613058 commonmeta_py-0.9.3/commonmeta/resources/ietf-bcp-47.json
--rw-r--r--   0        0        0   246361 2023-03-03 21:23:26.505900 commonmeta_py-0.9.3/commonmeta/resources/iso-8601.json
--rw-r--r--   0        0        0   172114 2022-11-28 11:27:39.856874 commonmeta_py-0.9.3/commonmeta/resources/spdx/licenses.json
--rw-r--r--   0        0        0    47334 2023-03-06 10:56:11.260953 commonmeta_py-0.9.3/commonmeta/resources/spdx-schema..json
--rw-r--r--   0        0        0    33187 2024-01-13 14:09:14.257188 commonmeta_py-0.9.3/commonmeta/utils.py
--rw-r--r--   0        0        0      337 2023-09-11 15:38:29.982546 commonmeta_py-0.9.3/commonmeta/writers/__init__.py
--rw-r--r--   0        0        0     3910 2024-01-13 13:55:47.406590 commonmeta_py-0.9.3/commonmeta/writers/bibtex_writer.py
--rw-r--r--   0        0        0     1140 2023-03-09 13:32:48.697716 commonmeta_py-0.9.3/commonmeta/writers/citation_writer.py
--rw-r--r--   0        0        0     1248 2023-09-11 18:27:59.201624 commonmeta_py-0.9.3/commonmeta/writers/commonmeta_writer.py
--rw-r--r--   0        0        0     2125 2024-01-14 15:05:14.031100 commonmeta_py-0.9.3/commonmeta/writers/csl_writer.py
--rw-r--r--   0        0        0     4651 2023-09-11 07:40:10.354531 commonmeta_py-0.9.3/commonmeta/writers/datacite_writer.py
--rw-r--r--   0        0        0     1849 2023-09-11 07:41:07.721309 commonmeta_py-0.9.3/commonmeta/writers/ris_writer.py
--rw-r--r--   0        0        0     5659 2023-09-11 13:45:11.754575 commonmeta_py-0.9.3/commonmeta/writers/schema_org_writer.py
--rw-r--r--   0        0        0     1638 2024-01-14 15:02:18.769081 commonmeta_py-0.9.3/pyproject.toml
--rw-r--r--   0        0        0     7835 1970-01-01 00:00:00.000000 commonmeta_py-0.9.3/PKG-INFO
+-rw-r--r--   0        0        0     1074 2023-02-21 06:38:55.700800 commonmeta_py-0.9.4/LICENSE
+-rw-r--r--   0        0        0     6008 2024-01-14 22:22:01.942132 commonmeta_py-0.9.4/README.md
+-rw-r--r--   0        0        0     1658 2023-09-14 17:49:33.421252 commonmeta_py-0.9.4/commonmeta/__init__.py
+-rw-r--r--   0        0        0     9054 2024-01-13 23:45:30.203394 commonmeta_py-0.9.4/commonmeta/author_utils.py
+-rw-r--r--   0        0        0     3323 2023-03-09 16:29:03.609320 commonmeta_py-0.9.4/commonmeta/base_utils.py
+-rw-r--r--   0        0        0    14627 2023-09-12 13:01:04.530045 commonmeta_py-0.9.4/commonmeta/constants.py
+-rw-r--r--   0        0        0     5452 2024-01-14 14:15:37.527705 commonmeta_py-0.9.4/commonmeta/date_utils.py
+-rw-r--r--   0        0        0     3576 2024-01-14 22:11:17.226408 commonmeta_py-0.9.4/commonmeta/doi_utils.py
+-rw-r--r--   0        0        0       56 2023-02-14 15:23:28.688206 commonmeta_py-0.9.4/commonmeta/metadata/__init__.py
+-rw-r--r--   0        0        0     6984 2024-01-14 19:12:19.732665 commonmeta_py-0.9.4/commonmeta/metadata/metadata.py
+-rw-r--r--   0        0        0      742 2024-01-14 19:13:51.649297 commonmeta_py-0.9.4/commonmeta/readers/__init__.py
+-rw-r--r--   0        0        0        0 2023-02-19 09:38:13.587826 commonmeta_py-0.9.4/commonmeta/readers/bibtex_reader.py
+-rw-r--r--   0        0        0     6053 2023-09-09 09:47:03.762792 commonmeta_py-0.9.4/commonmeta/readers/cff_reader.py
+-rw-r--r--   0        0        0     3656 2023-09-10 10:19:10.546283 commonmeta_py-0.9.4/commonmeta/readers/codemeta_reader.py
+-rw-r--r--   0        0        0      302 2024-01-13 14:13:06.635867 commonmeta_py-0.9.4/commonmeta/readers/commonmeta_reader.py
+-rw-r--r--   0        0        0     9871 2023-09-11 10:08:16.995435 commonmeta_py-0.9.4/commonmeta/readers/crossref_reader.py
+-rw-r--r--   0        0        0    20462 2023-09-11 09:32:48.588180 commonmeta_py-0.9.4/commonmeta/readers/crossref_xml_reader.py
+-rw-r--r--   0        0        0     2584 2023-09-09 11:07:35.317858 commonmeta_py-0.9.4/commonmeta/readers/csl_reader.py
+-rw-r--r--   0        0        0     5126 2024-01-14 14:38:04.826859 commonmeta_py-0.9.4/commonmeta/readers/datacite_reader.py
+-rw-r--r--   0        0        0    11367 2024-01-14 14:37:56.867392 commonmeta_py-0.9.4/commonmeta/readers/datacite_xml_reader.py
+-rw-r--r--   0        0        0     6773 2024-01-14 13:24:11.794486 commonmeta_py-0.9.4/commonmeta/readers/inveniordm_reader.py
+-rw-r--r--   0        0        0     4501 2023-09-11 12:02:15.815494 commonmeta_py-0.9.4/commonmeta/readers/json_feed_reader.py
+-rw-r--r--   0        0        0     7173 2023-09-12 12:07:23.937528 commonmeta_py-0.9.4/commonmeta/readers/kbase_reader.py
+-rw-r--r--   0        0        0     3529 2024-01-14 22:19:07.325013 commonmeta_py-0.9.4/commonmeta/readers/ris_reader.py
+-rw-r--r--   0        0        0    12685 2024-01-14 14:41:57.216355 commonmeta_py-0.9.4/commonmeta/readers/schema_org_reader.py
+-rw-r--r--   0        0        0   855312 2023-03-03 21:07:36.789294 commonmeta_py-0.9.4/commonmeta/resources/cff_v1.2.0.json
+-rw-r--r--   0        0        0    15070 2024-01-13 12:57:44.454997 commonmeta_py-0.9.4/commonmeta/resources/commonmeta_v0.10.5.json
+-rw-r--r--   0        0        0    12166 2023-03-03 21:30:37.485484 commonmeta_py-0.9.4/commonmeta/resources/csl-data.json
+-rw-r--r--   0        0        0    16650 2023-02-28 03:11:41.977630 commonmeta_py-0.9.4/commonmeta/resources/datacite-v4.json
+-rw-r--r--   0        0        0   228225 2023-03-03 21:24:04.613058 commonmeta_py-0.9.4/commonmeta/resources/ietf-bcp-47.json
+-rw-r--r--   0        0        0   246361 2023-03-03 21:23:26.505900 commonmeta_py-0.9.4/commonmeta/resources/iso-8601.json
+-rw-r--r--   0        0        0   172114 2022-11-28 11:27:39.856874 commonmeta_py-0.9.4/commonmeta/resources/spdx/licenses.json
+-rw-r--r--   0        0        0    47334 2023-03-06 10:56:11.260953 commonmeta_py-0.9.4/commonmeta/resources/spdx-schema..json
+-rw-r--r--   0        0        0    33187 2024-01-13 14:09:14.257188 commonmeta_py-0.9.4/commonmeta/utils.py
+-rw-r--r--   0        0        0      337 2023-09-11 15:38:29.982546 commonmeta_py-0.9.4/commonmeta/writers/__init__.py
+-rw-r--r--   0        0        0     3916 2024-01-14 18:47:17.162087 commonmeta_py-0.9.4/commonmeta/writers/bibtex_writer.py
+-rw-r--r--   0        0        0     1140 2023-03-09 13:32:48.697716 commonmeta_py-0.9.4/commonmeta/writers/citation_writer.py
+-rw-r--r--   0        0        0     1248 2023-09-11 18:27:59.201624 commonmeta_py-0.9.4/commonmeta/writers/commonmeta_writer.py
+-rw-r--r--   0        0        0     2125 2024-01-14 15:05:14.031100 commonmeta_py-0.9.4/commonmeta/writers/csl_writer.py
+-rw-r--r--   0        0        0     4651 2023-09-11 07:40:10.354531 commonmeta_py-0.9.4/commonmeta/writers/datacite_writer.py
+-rw-r--r--   0        0        0     1849 2023-09-11 07:41:07.721309 commonmeta_py-0.9.4/commonmeta/writers/ris_writer.py
+-rw-r--r--   0        0        0     5659 2023-09-11 13:45:11.754575 commonmeta_py-0.9.4/commonmeta/writers/schema_org_writer.py
+-rw-r--r--   0        0        0     1638 2024-01-14 20:56:40.100063 commonmeta_py-0.9.4/pyproject.toml
+-rw-r--r--   0        0        0     7835 1970-01-01 00:00:00.000000 commonmeta_py-0.9.4/PKG-INFO
```

### Comparing `commonmeta_py-0.9.3/LICENSE` & `commonmeta_py-0.9.4/LICENSE`

 * *Files identical despite different names*

### Comparing `commonmeta_py-0.9.3/README.md` & `commonmeta_py-0.9.4/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -38,15 +38,15 @@
 | [CSL-JSON](https://citationstyles.org/)                                                     | csl      | pplication/vnd.citationstyles.csl+json | yes | yes     |
 | [Formatted text citation](https://citationstyles.org/)                                           | citation      | text/x-bibliography                    | no      | yes     |
 | [Codemeta](https://codemeta.github.io/)                                                          | codemeta      | application/vnd.codemeta.ld+json       | yes | later |
 | [Citation File Format (CFF)](https://citation-file-format.github.io/)                            | cff           | application/vnd.cff+yaml               | yes | later |
 | [JATS](https://jats.nlm.nih.gov/)                                                                | jats          | application/vnd.jats+xml               | later   | later   |
 | [CSV](ttps://en.wikipedia.org/wiki/Comma-separated_values)                                       | csv           | text/csv                               | no      | later   |
 | [BibTex](http://en.wikipedia.org/wiki/BibTeX)                                                    | bibtex        | application/x-bibtex                   | later | yes     |
-| [RIS](http://en.wikipedia.org/wiki/RIS_(file_format))                                            | ris           | application/x-research-info-systems    | later | yes     |
+| [RIS](http://en.wikipedia.org/wiki/RIS_(file_format))                                            | ris           | application/x-research-info-systems    | yes   | yes     |
 | [InvenioRDM](https://inveniordm.docs.cern.ch/reference/metadata/)                                | inveniordm    | application/vnd.inveniordm.v1+json     | later | yes     |
 | [JSON Feed](https://www.jsonfeed.org/)                                                           | json_feed_item     | application/feed+json    | yes | later     |
 
 _commonmeta_: the Commonmeta format is the native format for the library and used internally.
 _Planned_: we plan to implement this format for the v1.0 public release.  
 _Later_: we plan to implement this format in a later release.
```

### Comparing `commonmeta_py-0.9.3/commonmeta/__init__.py` & `commonmeta_py-0.9.4/commonmeta/__init__.py`

 * *Files identical despite different names*

### Comparing `commonmeta_py-0.9.3/commonmeta/author_utils.py` & `commonmeta_py-0.9.4/commonmeta/author_utils.py`

 * *Files identical despite different names*

### Comparing `commonmeta_py-0.9.3/commonmeta/base_utils.py` & `commonmeta_py-0.9.4/commonmeta/base_utils.py`

 * *Files identical despite different names*

### Comparing `commonmeta_py-0.9.3/commonmeta/constants.py` & `commonmeta_py-0.9.4/commonmeta/constants.py`

 * *Files identical despite different names*

### Comparing `commonmeta_py-0.9.3/commonmeta/date_utils.py` & `commonmeta_py-0.9.4/commonmeta/date_utils.py`

 * *Files identical despite different names*

### Comparing `commonmeta_py-0.9.3/commonmeta/doi_utils.py` & `commonmeta_py-0.9.4/commonmeta/doi_utils.py`

 * *Files identical despite different names*

### Comparing `commonmeta_py-0.9.3/commonmeta/metadata/metadata.py` & `commonmeta_py-0.9.4/commonmeta/metadata/metadata.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,14 +24,15 @@
     read_cff,
     get_json_feed_item,
     read_json_feed_item,
     get_inveniordm,
     read_inveniordm,
     read_kbase,
     read_commonmeta,
+    read_ris,
 )
 from ..writers import (
     write_datacite,
     write_bibtex,
     write_citation,
     write_csl,
     write_ris,
@@ -112,14 +113,16 @@
                 meta = read_cff(data)
             elif via == "inveniordm":
                 data = json.loads(string)
                 meta = read_inveniordm(data)
             elif via == "kbase":
                 data = json.loads(string)
                 meta = read_kbase(data)
+            elif via == "ris":
+                meta = read_ris(string)
             # elif via == "bibtex":
             #     data = yaml.safe_load(string)
             #     meta = read_bibtex(data)
             else:
                 raise ValueError("No input format found")
         else:
             raise ValueError("No metadata found")
```

### Comparing `commonmeta_py-0.9.3/commonmeta/readers/__init__.py` & `commonmeta_py-0.9.4/commonmeta/readers/__init__.py`

 * *Files 26% similar despite different names*

```diff
@@ -7,7 +7,8 @@
 from .cff_reader import get_cff, read_cff
 from .crossref_xml_reader import get_crossref_xml, read_crossref_xml
 from .datacite_xml_reader import get_datacite_xml, read_datacite_xml
 from .json_feed_reader import get_json_feed_item, read_json_feed_item
 from .inveniordm_reader import get_inveniordm, read_inveniordm
 from .kbase_reader import read_kbase
 from .commonmeta_reader import read_commonmeta
+from .ris_reader import read_ris
```

### Comparing `commonmeta_py-0.9.3/commonmeta/readers/cff_reader.py` & `commonmeta_py-0.9.4/commonmeta/readers/cff_reader.py`

 * *Files identical despite different names*

### Comparing `commonmeta_py-0.9.3/commonmeta/readers/codemeta_reader.py` & `commonmeta_py-0.9.4/commonmeta/readers/codemeta_reader.py`

 * *Files identical despite different names*

### Comparing `commonmeta_py-0.9.3/commonmeta/readers/crossref_reader.py` & `commonmeta_py-0.9.4/commonmeta/readers/crossref_reader.py`

 * *Files identical despite different names*

### Comparing `commonmeta_py-0.9.3/commonmeta/readers/crossref_xml_reader.py` & `commonmeta_py-0.9.4/commonmeta/readers/crossref_xml_reader.py`

 * *Files identical despite different names*

### Comparing `commonmeta_py-0.9.3/commonmeta/readers/csl_reader.py` & `commonmeta_py-0.9.4/commonmeta/readers/csl_reader.py`

 * *Files identical despite different names*

### Comparing `commonmeta_py-0.9.3/commonmeta/readers/datacite_reader.py` & `commonmeta_py-0.9.4/commonmeta/readers/datacite_reader.py`

 * *Files identical despite different names*

### Comparing `commonmeta_py-0.9.3/commonmeta/readers/datacite_xml_reader.py` & `commonmeta_py-0.9.4/commonmeta/readers/datacite_xml_reader.py`

 * *Files identical despite different names*

### Comparing `commonmeta_py-0.9.3/commonmeta/readers/inveniordm_reader.py` & `commonmeta_py-0.9.4/commonmeta/readers/inveniordm_reader.py`

 * *Files identical despite different names*

### Comparing `commonmeta_py-0.9.3/commonmeta/readers/json_feed_reader.py` & `commonmeta_py-0.9.4/commonmeta/readers/json_feed_reader.py`

 * *Files identical despite different names*

### Comparing `commonmeta_py-0.9.3/commonmeta/readers/kbase_reader.py` & `commonmeta_py-0.9.4/commonmeta/readers/kbase_reader.py`

 * *Files identical despite different names*

### Comparing `commonmeta_py-0.9.3/commonmeta/readers/schema_org_reader.py` & `commonmeta_py-0.9.4/commonmeta/readers/schema_org_reader.py`

 * *Files identical despite different names*

### Comparing `commonmeta_py-0.9.3/commonmeta/resources/cff_v1.2.0.json` & `commonmeta_py-0.9.4/commonmeta/resources/cff_v1.2.0.json`

 * *Files identical despite different names*

### Comparing `commonmeta_py-0.9.3/commonmeta/resources/commonmeta_v0.10.5.json` & `commonmeta_py-0.9.4/commonmeta/resources/commonmeta_v0.10.5.json`

 * *Files identical despite different names*

### Comparing `commonmeta_py-0.9.3/commonmeta/resources/csl-data.json` & `commonmeta_py-0.9.4/commonmeta/resources/csl-data.json`

 * *Files identical despite different names*

### Comparing `commonmeta_py-0.9.3/commonmeta/resources/datacite-v4.json` & `commonmeta_py-0.9.4/commonmeta/resources/datacite-v4.json`

 * *Files identical despite different names*

### Comparing `commonmeta_py-0.9.3/commonmeta/resources/ietf-bcp-47.json` & `commonmeta_py-0.9.4/commonmeta/resources/ietf-bcp-47.json`

 * *Files identical despite different names*

### Comparing `commonmeta_py-0.9.3/commonmeta/resources/iso-8601.json` & `commonmeta_py-0.9.4/commonmeta/resources/iso-8601.json`

 * *Files identical despite different names*

### Comparing `commonmeta_py-0.9.3/commonmeta/resources/spdx/licenses.json` & `commonmeta_py-0.9.4/commonmeta/resources/spdx/licenses.json`

 * *Files identical despite different names*

### Comparing `commonmeta_py-0.9.3/commonmeta/resources/spdx-schema..json` & `commonmeta_py-0.9.4/commonmeta/resources/spdx-schema..json`

 * *Files identical despite different names*

### Comparing `commonmeta_py-0.9.3/commonmeta/utils.py` & `commonmeta_py-0.9.4/commonmeta/utils.py`

 * *Files identical despite different names*

### Comparing `commonmeta_py-0.9.3/commonmeta/writers/bibtex_writer.py` & `commonmeta_py-0.9.4/commonmeta/writers/bibtex_writer.py`

 * *Files 0% similar despite different names*

```diff
@@ -48,15 +48,15 @@
         if container.get("identifierType", None) == "ISBN"
         else None
     )
     issue = container.get("issue", None)
     journal = (
         container.get("title", None)
         if type_ not in ["inbook", "inproceedings"]
-        and container.get("type") in ["Journal", "Blog"]
+        and container.get("type") in ["Journal", "Periodical"]
         else None
     )
     booktitle = (
         container.get("title", None) if type_ in ["inbook", "inproceedings"] else None
     )
     language = metadata.language
     location = (
```

### Comparing `commonmeta_py-0.9.3/commonmeta/writers/citation_writer.py` & `commonmeta_py-0.9.4/commonmeta/writers/citation_writer.py`

 * *Files identical despite different names*

### Comparing `commonmeta_py-0.9.3/commonmeta/writers/commonmeta_writer.py` & `commonmeta_py-0.9.4/commonmeta/writers/commonmeta_writer.py`

 * *Files identical despite different names*

### Comparing `commonmeta_py-0.9.3/commonmeta/writers/csl_writer.py` & `commonmeta_py-0.9.4/commonmeta/writers/csl_writer.py`

 * *Files identical despite different names*

### Comparing `commonmeta_py-0.9.3/commonmeta/writers/datacite_writer.py` & `commonmeta_py-0.9.4/commonmeta/writers/datacite_writer.py`

 * *Files identical despite different names*

### Comparing `commonmeta_py-0.9.3/commonmeta/writers/ris_writer.py` & `commonmeta_py-0.9.4/commonmeta/writers/ris_writer.py`

 * *Files identical despite different names*

### Comparing `commonmeta_py-0.9.3/commonmeta/writers/schema_org_writer.py` & `commonmeta_py-0.9.4/commonmeta/writers/schema_org_writer.py`

 * *Files identical despite different names*

### Comparing `commonmeta_py-0.9.3/pyproject.toml` & `commonmeta_py-0.9.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name="commonmeta-py"
-version="0.9.3"
+version="0.9.4"
 description="Library for conversions to/from the Commonmeta scholarly metadata format"
 authors=["Martin Fenner <martin@front-matter.io>"]
 readme = "README.md"
 packages = [{include = "commonmeta"}]
 
 [tool.poetry.dependencies]
 python = ">=3.9,<4.0.0"
```

### Comparing `commonmeta_py-0.9.3/PKG-INFO` & `commonmeta_py-0.9.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: commonmeta-py
-Version: 0.9.3
+Version: 0.9.4
 Summary: Library for conversions to/from the Commonmeta scholarly metadata format
 Author: Martin Fenner
 Author-email: martin@front-matter.io
 Requires-Python: >=3.9,<4.0.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -83,15 +83,15 @@
 | [CSL-JSON](https://citationstyles.org/)                                                     | csl      | pplication/vnd.citationstyles.csl+json | yes | yes     |
 | [Formatted text citation](https://citationstyles.org/)                                           | citation      | text/x-bibliography                    | no      | yes     |
 | [Codemeta](https://codemeta.github.io/)                                                          | codemeta      | application/vnd.codemeta.ld+json       | yes | later |
 | [Citation File Format (CFF)](https://citation-file-format.github.io/)                            | cff           | application/vnd.cff+yaml               | yes | later |
 | [JATS](https://jats.nlm.nih.gov/)                                                                | jats          | application/vnd.jats+xml               | later   | later   |
 | [CSV](ttps://en.wikipedia.org/wiki/Comma-separated_values)                                       | csv           | text/csv                               | no      | later   |
 | [BibTex](http://en.wikipedia.org/wiki/BibTeX)                                                    | bibtex        | application/x-bibtex                   | later | yes     |
-| [RIS](http://en.wikipedia.org/wiki/RIS_(file_format))                                            | ris           | application/x-research-info-systems    | later | yes     |
+| [RIS](http://en.wikipedia.org/wiki/RIS_(file_format))                                            | ris           | application/x-research-info-systems    | yes   | yes     |
 | [InvenioRDM](https://inveniordm.docs.cern.ch/reference/metadata/)                                | inveniordm    | application/vnd.inveniordm.v1+json     | later | yes     |
 | [JSON Feed](https://www.jsonfeed.org/)                                                           | json_feed_item     | application/feed+json    | yes | later     |
 
 _commonmeta_: the Commonmeta format is the native format for the library and used internally.
 _Planned_: we plan to implement this format for the v1.0 public release.  
 _Later_: we plan to implement this format in a later release.
```

