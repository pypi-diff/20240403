# Comparing `tmp/undertext-0.1.0.tar.gz` & `tmp/undertext-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "undertext-0.1.0.tar", last modified: Tue Apr  2 13:45:02 2024, max compression
+gzip compressed data, was "undertext-0.2.0.tar", last modified: Wed Apr  3 13:17:31 2024, max compression
```

## Comparing `undertext-0.1.0.tar` & `undertext-0.2.0.tar`

### file list

```diff
@@ -1,33 +1,38 @@
-drwxrwxr-x   0 playerg9  (1000) playerg9  (1000)        0 2024-04-02 13:45:02.865226 undertext-0.1.0/
--rw-rw-r--   0 playerg9  (1000) playerg9  (1000)     1074 2024-04-01 10:58:40.000000 undertext-0.1.0/LICENSE
--rw-r--r--   0 playerg9  (1000) playerg9  (1000)     3682 2024-04-02 13:45:02.865226 undertext-0.1.0/PKG-INFO
--rw-rw-r--   0 playerg9  (1000) playerg9  (1000)     2334 2024-04-02 12:06:09.000000 undertext-0.1.0/README.md
--rw-rw-r--   0 playerg9  (1000) playerg9  (1000)       87 2024-04-01 11:00:16.000000 undertext-0.1.0/pyproject.toml
--rw-rw-r--   0 playerg9  (1000) playerg9  (1000)       38 2024-04-02 13:45:02.865226 undertext-0.1.0/setup.cfg
--rw-rw-r--   0 playerg9  (1000) playerg9  (1000)     1917 2024-04-01 14:33:10.000000 undertext-0.1.0/setup.py
-drwxrwxr-x   0 playerg9  (1000) playerg9  (1000)        0 2024-04-02 13:45:02.861226 undertext-0.1.0/src/
-drwxrwxr-x   0 playerg9  (1000) playerg9  (1000)        0 2024-04-02 13:45:02.861226 undertext-0.1.0/src/undertext/
--rw-rw-r--   0 playerg9  (1000) playerg9  (1000)     1031 2024-04-02 13:05:36.000000 undertext-0.1.0/src/undertext/__cli__.py
--rw-rw-r--   0 playerg9  (1000) playerg9  (1000)     1663 2024-04-02 13:32:00.000000 undertext-0.1.0/src/undertext/__init__.py
--rw-rw-r--   0 playerg9  (1000) playerg9  (1000)     2280 2024-04-02 11:53:18.000000 undertext-0.1.0/src/undertext/__main__.py
--rw-rw-r--   0 playerg9  (1000) playerg9  (1000)      189 2024-04-01 12:30:46.000000 undertext-0.1.0/src/undertext/exceptions.py
-drwxrwxr-x   0 playerg9  (1000) playerg9  (1000)        0 2024-04-02 13:45:02.861226 undertext-0.1.0/src/undertext/readers/
--rw-rw-r--   0 playerg9  (1000) playerg9  (1000)      985 2024-04-02 13:20:03.000000 undertext-0.1.0/src/undertext/readers/__init__.py
--rw-rw-r--   0 playerg9  (1000) playerg9  (1000)     1262 2024-04-02 11:35:50.000000 undertext-0.1.0/src/undertext/readers/microdvd.py
--rw-rw-r--   0 playerg9  (1000) playerg9  (1000)     1699 2024-04-02 12:35:19.000000 undertext-0.1.0/src/undertext/readers/subrip.py
--rw-rw-r--   0 playerg9  (1000) playerg9  (1000)     3073 2024-04-02 11:04:28.000000 undertext-0.1.0/src/undertext/readers/webvtt.py
-drwxrwxr-x   0 playerg9  (1000) playerg9  (1000)        0 2024-04-02 13:45:02.861226 undertext-0.1.0/src/undertext/structures/
--rw-rw-r--   0 playerg9  (1000) playerg9  (1000)       86 2024-04-01 15:03:12.000000 undertext-0.1.0/src/undertext/structures/__init__.py
--rw-rw-r--   0 playerg9  (1000) playerg9  (1000)     2497 2024-04-02 12:35:19.000000 undertext-0.1.0/src/undertext/structures/caption.py
-drwxrwxr-x   0 playerg9  (1000) playerg9  (1000)        0 2024-04-02 13:45:02.865226 undertext-0.1.0/src/undertext/writers/
--rw-rw-r--   0 playerg9  (1000) playerg9  (1000)     1042 2024-04-02 13:20:10.000000 undertext-0.1.0/src/undertext/writers/__init__.py
--rw-rw-r--   0 playerg9  (1000) playerg9  (1000)      942 2024-04-02 11:35:50.000000 undertext-0.1.0/src/undertext/writers/microdvd.py
--rw-rw-r--   0 playerg9  (1000) playerg9  (1000)      926 2024-04-01 20:59:43.000000 undertext-0.1.0/src/undertext/writers/subrip.py
--rw-rw-r--   0 playerg9  (1000) playerg9  (1000)     1597 2024-04-02 11:01:15.000000 undertext-0.1.0/src/undertext/writers/webvtt.py
-drwxrwxr-x   0 playerg9  (1000) playerg9  (1000)        0 2024-04-02 13:45:02.865226 undertext-0.1.0/src/undertext.egg-info/
--rw-r--r--   0 playerg9  (1000) playerg9  (1000)     3682 2024-04-02 13:45:02.000000 undertext-0.1.0/src/undertext.egg-info/PKG-INFO
--rw-rw-r--   0 playerg9  (1000) playerg9  (1000)      707 2024-04-02 13:45:02.000000 undertext-0.1.0/src/undertext.egg-info/SOURCES.txt
--rw-rw-r--   0 playerg9  (1000) playerg9  (1000)        1 2024-04-02 13:45:02.000000 undertext-0.1.0/src/undertext.egg-info/dependency_links.txt
--rw-rw-r--   0 playerg9  (1000) playerg9  (1000)       54 2024-04-02 13:45:02.000000 undertext-0.1.0/src/undertext.egg-info/entry_points.txt
--rw-rw-r--   0 playerg9  (1000) playerg9  (1000)        7 2024-04-02 13:45:02.000000 undertext-0.1.0/src/undertext.egg-info/requires.txt
--rw-rw-r--   0 playerg9  (1000) playerg9  (1000)       10 2024-04-02 13:45:02.000000 undertext-0.1.0/src/undertext.egg-info/top_level.txt
+drwxrwxr-x   0 playerg9  (1000) playerg9  (1000)        0 2024-04-03 13:17:31.422301 undertext-0.2.0/
+-rw-rw-r--   0 playerg9  (1000) playerg9  (1000)     1074 2024-04-03 12:04:43.000000 undertext-0.2.0/LICENSE
+-rw-r--r--   0 playerg9  (1000) playerg9  (1000)     3741 2024-04-03 13:17:31.422301 undertext-0.2.0/PKG-INFO
+-rw-rw-r--   0 playerg9  (1000) playerg9  (1000)     2393 2024-04-03 12:04:43.000000 undertext-0.2.0/README.md
+-rw-rw-r--   0 playerg9  (1000) playerg9  (1000)       87 2024-04-03 12:04:43.000000 undertext-0.2.0/pyproject.toml
+-rw-rw-r--   0 playerg9  (1000) playerg9  (1000)       38 2024-04-03 13:17:31.422301 undertext-0.2.0/setup.cfg
+-rw-rw-r--   0 playerg9  (1000) playerg9  (1000)     1917 2024-04-03 12:04:43.000000 undertext-0.2.0/setup.py
+drwxrwxr-x   0 playerg9  (1000) playerg9  (1000)        0 2024-04-03 13:17:31.410301 undertext-0.2.0/src/
+drwxrwxr-x   0 playerg9  (1000) playerg9  (1000)        0 2024-04-03 13:17:31.414301 undertext-0.2.0/src/undertext/
+-rw-rw-r--   0 playerg9  (1000) playerg9  (1000)     1216 2024-04-03 12:04:43.000000 undertext-0.2.0/src/undertext/__cli__.py
+-rw-rw-r--   0 playerg9  (1000) playerg9  (1000)     1663 2024-04-03 13:17:26.000000 undertext-0.2.0/src/undertext/__init__.py
+-rw-rw-r--   0 playerg9  (1000) playerg9  (1000)     2538 2024-04-03 12:04:43.000000 undertext-0.2.0/src/undertext/__main__.py
+-rw-rw-r--   0 playerg9  (1000) playerg9  (1000)      189 2024-04-03 12:04:43.000000 undertext-0.2.0/src/undertext/exceptions.py
+drwxrwxr-x   0 playerg9  (1000) playerg9  (1000)        0 2024-04-03 13:17:31.418301 undertext-0.2.0/src/undertext/readers/
+-rw-rw-r--   0 playerg9  (1000) playerg9  (1000)     1105 2024-04-03 12:12:36.000000 undertext-0.2.0/src/undertext/readers/__init__.py
+-rw-rw-r--   0 playerg9  (1000) playerg9  (1000)     1262 2024-04-03 12:04:43.000000 undertext-0.2.0/src/undertext/readers/microdvd.py
+-rw-rw-r--   0 playerg9  (1000) playerg9  (1000)     1295 2024-04-03 12:04:43.000000 undertext-0.2.0/src/undertext/readers/subrip.py
+-rw-rw-r--   0 playerg9  (1000) playerg9  (1000)     1003 2024-04-03 12:23:11.000000 undertext-0.2.0/src/undertext/readers/subviewer.py
+-rw-rw-r--   0 playerg9  (1000) playerg9  (1000)     2684 2024-04-03 12:04:43.000000 undertext-0.2.0/src/undertext/readers/webvtt.py
+drwxrwxr-x   0 playerg9  (1000) playerg9  (1000)        0 2024-04-03 13:17:31.418301 undertext-0.2.0/src/undertext/structures/
+-rw-rw-r--   0 playerg9  (1000) playerg9  (1000)       86 2024-04-03 12:04:43.000000 undertext-0.2.0/src/undertext/structures/__init__.py
+-rw-rw-r--   0 playerg9  (1000) playerg9  (1000)     2497 2024-04-03 12:04:43.000000 undertext-0.2.0/src/undertext/structures/caption.py
+drwxrwxr-x   0 playerg9  (1000) playerg9  (1000)        0 2024-04-03 13:17:31.418301 undertext-0.2.0/src/undertext/util/
+-rw-rw-r--   0 playerg9  (1000) playerg9  (1000)       53 2024-04-03 12:04:43.000000 undertext-0.2.0/src/undertext/util/__init__.py
+-rw-rw-r--   0 playerg9  (1000) playerg9  (1000)     2396 2024-04-03 12:04:43.000000 undertext-0.2.0/src/undertext/util/time.py
+drwxrwxr-x   0 playerg9  (1000) playerg9  (1000)        0 2024-04-03 13:17:31.422301 undertext-0.2.0/src/undertext/writers/
+-rw-rw-r--   0 playerg9  (1000) playerg9  (1000)     1165 2024-04-03 12:04:43.000000 undertext-0.2.0/src/undertext/writers/__init__.py
+-rw-rw-r--   0 playerg9  (1000) playerg9  (1000)      942 2024-04-03 12:04:43.000000 undertext-0.2.0/src/undertext/writers/microdvd.py
+-rw-rw-r--   0 playerg9  (1000) playerg9  (1000)      768 2024-04-03 12:04:43.000000 undertext-0.2.0/src/undertext/writers/subrip.py
+-rw-rw-r--   0 playerg9  (1000) playerg9  (1000)      827 2024-04-03 12:23:11.000000 undertext-0.2.0/src/undertext/writers/subviewer.py
+-rw-rw-r--   0 playerg9  (1000) playerg9  (1000)     1455 2024-04-03 12:04:43.000000 undertext-0.2.0/src/undertext/writers/webvtt.py
+drwxrwxr-x   0 playerg9  (1000) playerg9  (1000)        0 2024-04-03 13:17:31.422301 undertext-0.2.0/src/undertext.egg-info/
+-rw-r--r--   0 playerg9  (1000) playerg9  (1000)     3741 2024-04-03 13:17:31.000000 undertext-0.2.0/src/undertext.egg-info/PKG-INFO
+-rw-rw-r--   0 playerg9  (1000) playerg9  (1000)      835 2024-04-03 13:17:31.000000 undertext-0.2.0/src/undertext.egg-info/SOURCES.txt
+-rw-rw-r--   0 playerg9  (1000) playerg9  (1000)        1 2024-04-03 13:17:31.000000 undertext-0.2.0/src/undertext.egg-info/dependency_links.txt
+-rw-rw-r--   0 playerg9  (1000) playerg9  (1000)       54 2024-04-03 13:17:31.000000 undertext-0.2.0/src/undertext.egg-info/entry_points.txt
+-rw-rw-r--   0 playerg9  (1000) playerg9  (1000)        7 2024-04-03 13:17:31.000000 undertext-0.2.0/src/undertext.egg-info/requires.txt
+-rw-rw-r--   0 playerg9  (1000) playerg9  (1000)       10 2024-04-03 13:17:31.000000 undertext-0.2.0/src/undertext.egg-info/top_level.txt
```

### Comparing `undertext-0.1.0/LICENSE` & `undertext-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `undertext-0.1.0/PKG-INFO` & `undertext-0.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: undertext
-Version: 0.1.0
+Version: 0.2.0
 Summary: library to load, edit and save different formats of subtitles
 Home-page: https://github.com/utility-libraries/undertext-py
 Author: PlayerG9
 License: MIT
 Project-URL: Organisation Github, https://github.com/utility-libraries
 Project-URL: Homepage, https://github.com/utility-libraries/undertext-py/
 Project-URL: Documentation, https://utility-libraries.github.io/undertext-py/
@@ -53,14 +53,15 @@
 ```
 
 ## File Formats
 
 | ext    | name                      | read  | write |
 |--------|---------------------------|-------|-------|
 | `.ass` | Advanced SubStation Alpha | ❌     | ❌     |
+| `.sbv` | SubViewer                 | ❌     | ✅     |
 | `.srt` | SubRip                    | ✅     | ✅     |
 | `.ssa` | Sub Station Alpha         | ❌     | ❌     |
 | `.sub` | MicroDVD                  | ✅     | ✅     |
 | `.vtt` | WebVTT                    | ✅     | ✅     |
 
 <small>Listed formats that are currently unsupported may be added at a later version</small>
```

### Comparing `undertext-0.1.0/README.md` & `undertext-0.2.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -22,14 +22,15 @@
 ```
 
 ## File Formats
 
 | ext    | name                      | read  | write |
 |--------|---------------------------|-------|-------|
 | `.ass` | Advanced SubStation Alpha | ❌     | ❌     |
+| `.sbv` | SubViewer                 | ❌     | ✅     |
 | `.srt` | SubRip                    | ✅     | ✅     |
 | `.ssa` | Sub Station Alpha         | ❌     | ❌     |
 | `.sub` | MicroDVD                  | ✅     | ✅     |
 | `.vtt` | WebVTT                    | ✅     | ✅     |
 
 <small>Listed formats that are currently unsupported may be added at a later version</small>
```

### Comparing `undertext-0.1.0/setup.py` & `undertext-0.2.0/setup.py`

 * *Files identical despite different names*

### Comparing `undertext-0.1.0/src/undertext/__cli__.py` & `undertext-0.2.0/src/undertext/__cli__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,21 +1,26 @@
 # -*- coding=utf-8 -*-
 r"""
 
 """
+import re
 from pathlib import Path
 from . import loads, dumps
 
 
-def cmd_read(input_fp, **kwargs) -> None:
+def cmd_read(input_fp, after: float = None, before: float = None, **kwargs) -> None:
     input_fp = Path(input_fp)
     if not input_fp.is_file():
         raise FileNotFoundError(str(input_fp))
 
     for caption in loads(input_fp, **kwargs):
+        if after and caption.start <= after:
+            continue
+        if before and caption.end >= before:
+            continue
         print(f"{caption!r}")
 
 
 def cmd_convert(input_fp: str, output_fp: str, overwrite: bool = False, **kwargs):
     input_fp = Path(input_fp)
     if not input_fp.is_file():
         raise FileNotFoundError(str(input_fp))
```

### Comparing `undertext-0.1.0/src/undertext/__init__.py` & `undertext-0.2.0/src/undertext/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 __copyright__ = "Copyright 2024, utility-libraries"
 __credits__ = ["PlayerG9"]
 __license__ = "MIT"
 __maintainer__ = "PlayerG9"
 __email__ = None
 __status__ = "Prototype"  # Prototype, Development, Production
 __description__ = "library to load, edit and save different formats of subtitles"
-__version_info__ = (0, 1, 0)
+__version_info__ = (0, 2, 0)
 __version__ = '.'.join(str(_) for _ in __version_info__)
 
 from .exceptions import *
 from .structures import *
 from . import readers, writers
 from .readers import loads
 from .writers import dumps
```

### Comparing `undertext-0.1.0/src/undertext/__main__.py` & `undertext-0.2.0/src/undertext/__main__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,26 +1,30 @@
 # -*- coding=utf-8 -*-
 r"""
 
 """
 import argparse as ap
-from . import __cli__ as cli
+from . import __cli__ as cli, util
 
 
 parser = ap.ArgumentParser(prog="undertext", formatter_class=ap.ArgumentDefaultsHelpFormatter)
 parser.set_defaults(fn=parser.print_help)
 subparsers = parser.add_subparsers()
 
 read_parser = subparsers.add_parser("read",
                                     epilog="Note: Some optional arguments are hidden")
 read_parser.set_defaults(fn=cli.cmd_read)
 read_parser.add_argument("input_fp", metavar="input",
                          help="input file")
 read_parser.add_argument("--fmt", type=str, default=ap.SUPPRESS,
                          help="specify the format if it can't be guessed from the file extension")
+read_parser.add_argument('--after', type=cli.parse_time,
+                         help="show only captions that start after")
+read_parser.add_argument('--before', type=cli.parse_time,
+                         help="show only captions that end before")
 read_parser.add_argument("--fps", type=float, default=ap.SUPPRESS,
                          help=ap.SUPPRESS)
 
 convert_parser = subparsers.add_parser("convert",
                                        epilog="Note: Some optional arguments are hidden and need to be prefixed"
                                               " with '--input-' or '--output-'")
 convert_parser.set_defaults(fn=cli.cmd_convert)
```

### Comparing `undertext-0.1.0/src/undertext/readers/__init__.py` & `undertext-0.2.0/src/undertext/readers/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -4,25 +4,28 @@
 """
 import typing as t
 from os import PathLike
 from pathlib import Path
 from ..structures import Caption
 from .microdvd import read_microdvd
 from .subrip import read_subrip
+from .subviewer import read_subviewer
 from .webvtt import read_webvtt
 
 
 EXT_MAP = dict(
+    sbv=read_subviewer,
     srt=read_subrip,
     sub=read_microdvd,
     vtt=read_webvtt,
 )
 ALIAS_MAP = dict(
     microdvd=read_microdvd,
     subrip=read_subrip,
+    subviewer=read_subviewer,
     webvtt=read_webvtt,
 )
 
 
 def loads(fp: t.Union[str, PathLike], fmt: str = None, **kwargs) -> t.List[Caption]:
     r"""
     load the captions from a file
@@ -34,13 +37,13 @@
     """
     fp = Path(fp)
 
     if fmt is None:
         fmt = fp.suffix[1:]
         reader = EXT_MAP.get(fmt.lower())
     else:
-        reader = ALIAS_MAP.get(fmt.lower())
+        reader = ALIAS_MAP.get(fmt.lower()) or EXT_MAP.get(fmt.lower())
 
     if reader is None:
         raise ValueError(f"Unknown format ({fmt!s})")
 
     return reader(fp, **kwargs)
```

### Comparing `undertext-0.1.0/src/undertext/readers/microdvd.py` & `undertext-0.2.0/src/undertext/readers/microdvd.py`

 * *Files identical despite different names*

### Comparing `undertext-0.1.0/src/undertext/readers/subrip.py` & `undertext-0.2.0/src/undertext/readers/subviewer.py`

 * *Files 26% similar despite different names*

```diff
@@ -3,58 +3,37 @@
 
 """
 import re
 import typing as t
 from pathlib import Path
 from ..structures import Caption
 from ..exceptions import *
+from ..util import parse_time_dot as parse_time
 
 
-TIME_RE = re.compile(r"(?:(?P<h>\d{2,}):)?(?P<m>\d{2}):(?P<s>\d{2},\d{3})")
-RANGE_RE = re.compile(r"^(?P<start>(\d{2,}:)?\d{2}:\d{2},\d{3}) --> (?P<end>(\d{2,}:)?\d{2}:\d{2},\d{3})"
-                      r"(?P<style> .*)?$")
+RANGE_RE = re.compile(r"^(?P<start>(\d{2,}:)?\d{2}:\d{2}.\d{3}),(?P<end>(\d{2,}:)?\d{2}:\d{2}.\d{3})$")
 
 
-def read_subrip(fp: Path) -> t.List[Caption]:
+def read_subviewer(fp: Path) -> t.List[Caption]:
     captions: t.List[Caption] = []
 
     with open(fp, 'r') as file:
         lines = (_.rstrip() for _ in iter(file))
 
-        i = 0
-
         for line in lines:
-            i += 1
-            if line != f"{i}":  # identifier is a numeric counter
-                raise FormatException("Bad numeric counter")
-
-            line = next(lines, "")
             match = RANGE_RE.fullmatch(line)
             if match is None:
                 raise FormatException(f"Missing or invalid time range ({line})")
 
             start = parse_time(match.group("start"))
             end = parse_time(match.group("end"))
 
-            text_lines = []
-            for text_line in lines:
-                if not text_line:
-                    break
-                text_lines.append(text_line)
+            text_line = next(lines, "")
+            text_lines = text_line.split("[br]")
 
             captions.append(
                 Caption(start=start, end=end, text=text_lines)
             )
 
-    return captions
+            next(lines, "")
 
-
-def parse_time(text: str) -> float:
-    match = TIME_RE.fullmatch(text)
-    if match is None:
-        raise FormatException(f"Bad time format: {text!r}")
-
-    hours = match.group("h")
-    hours = 0 if hours is None else int(hours)
-    minutes = int(match.group("m"))
-    seconds = float(match.group("s").replace(",", "."))
-    return (hours * 3600) + (minutes * 60) + seconds
+    return captions
```

### Comparing `undertext-0.1.0/src/undertext/readers/webvtt.py` & `undertext-0.2.0/src/undertext/readers/webvtt.py`

 * *Files 7% similar despite different names*

```diff
@@ -3,18 +3,18 @@
 
 """
 import re
 import typing as t
 from pathlib import Path
 from ..structures import Caption
 from ..exceptions import *
+from ..util import parse_time_dot as parse_time
 
 
 HEAD_RE = re.compile(r"^WEBVTT ?")
-TIME_RE = re.compile(r"(?:(?P<h>\d{2,}):)?(?P<m>\d{2}):(?P<s>\d{2}\.\d{3})")
 RANGE_RE = re.compile(r"^(?P<start>(\d{2,}:)?\d{2}:\d{2}\.\d{3}) --> (?P<end>(\d{2,}:)?\d{2}:\d{2}\.\d{3})"
                       r"(?P<style> .*)?$")
 
 
 def read_webvtt(fp: Path) -> t.List[Caption]:
     captions: t.List[Caption] = []
 
@@ -70,19 +70,7 @@
                         text_lines.append(text_line)
 
                 captions.append(
                     Caption(start=start, end=end, text=text_lines, id=id_, styles=styles)
                 )
 
     return captions
-
-
-def parse_time(text: str) -> float:
-    match = TIME_RE.fullmatch(text)
-    if match is None:
-        raise FormatException(f"Bad time format: {text!r}")
-
-    hours = match.group("h")
-    hours = 0 if hours is None else int(hours)
-    minutes = int(match.group("m"))
-    seconds = float(match.group("s"))
-    return (hours * 3600) + (minutes * 60) + seconds
```

### Comparing `undertext-0.1.0/src/undertext/structures/caption.py` & `undertext-0.2.0/src/undertext/structures/caption.py`

 * *Files identical despite different names*

### Comparing `undertext-0.1.0/src/undertext/writers/__init__.py` & `undertext-0.2.0/src/undertext/writers/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,25 +4,28 @@
 """
 import typing as t
 from os import PathLike
 from pathlib import Path
 from ..structures import Caption
 from .microdvd import write_microdvd
 from .subrip import write_subrip
+from .subviewer import write_subviewer
 from .webvtt import write_webvtt
 
 
 EXT_MAP = dict(
+    sbv=write_subviewer,
     srt=write_subrip,
     sub=write_microdvd,
     vtt=write_webvtt,
 )
 ALIAS_MAP = dict(
     microdvd=write_microdvd,
     subrip=write_subrip,
+    subviewer=write_subviewer,
     webvtt=write_webvtt,
 )
 
 
 def dumps(captions: t.List[Caption], fp: t.Union[str, PathLike], fmt: str = None, **kwargs) -> None:
     r"""
     dumps some captions into a file
@@ -34,13 +37,13 @@
     """
     fp = Path(fp)
 
     if fmt is None:
         fmt = fp.suffix[1:]
         writer = EXT_MAP.get(fmt.lower())
     else:
-        writer = ALIAS_MAP.get(fmt.lower())
+        writer = ALIAS_MAP.get(fmt.lower()) or EXT_MAP.get(fmt.lower())
 
     if writer is None:
         raise ValueError(f"Unknown format ({fmt!s})")
 
     return writer(captions, fp, **kwargs)
```

### Comparing `undertext-0.1.0/src/undertext/writers/microdvd.py` & `undertext-0.2.0/src/undertext/writers/microdvd.py`

 * *Files identical despite different names*

### Comparing `undertext-0.1.0/src/undertext/writers/subrip.py` & `undertext-0.2.0/src/undertext/writers/subrip.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 r"""
 
 """
 import io
 import typing as t
 from os import PathLike
 from ..structures import Caption
+from ..util import format_ts_comma as format_ts
 
 
 def write_subrip(captions: t.List[Caption], filename: t.Union[str, PathLike, t.TextIO]) -> None:
     stream = io.StringIO()
 
     for i, caption in enumerate(captions):
         if i != 0:
@@ -21,15 +22,7 @@
             stream.write(f"{line}\r\n")
 
     if isinstance(filename, (str, PathLike)):
         with open(filename, 'w') as file:
             file.write(stream.getvalue())
     else:
         filename.write(stream.getvalue())
-
-
-def format_ts(ts: float) -> str:
-    seconds = ts % 60
-    minutes = int((ts / 60) % 60)
-    hours = int(ts / 3600)
-
-    return f"{hours:0>2}:{minutes:0>2}:{format(seconds, '.3f').replace('.', ','):0>6}"
```

### Comparing `undertext-0.1.0/src/undertext/writers/webvtt.py` & `undertext-0.2.0/src/undertext/writers/webvtt.py`

 * *Files 18% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 r"""
 
 """
 import io
 import typing as t
 from os import PathLike
 from ..structures import Caption
+from ..util import format_ts_dot as format_ts
 
 
 def write_webvtt(captions: t.List[Caption], filename: t.Union[str, PathLike, t.TextIO],
                  header: str = None) -> None:
     stream = io.StringIO()
 
     stream.write("WEBVTT")
@@ -37,15 +38,7 @@
                 stream.write(f"- {line}\r\n")
 
     if isinstance(filename, (str, PathLike)):
         with open(filename, 'w') as file:
             file.write(stream.getvalue())
     else:
         filename.write(stream.getvalue())
-
-
-def format_ts(ts: float) -> str:
-    seconds = ts % 60
-    minutes = int((ts / 60) % 60)
-    hours = int(ts / 3600)
-
-    return f"{hours:0>2}:{minutes:0>2}:{format(seconds, '.3f'):0>6}"
```

### Comparing `undertext-0.1.0/src/undertext.egg-info/PKG-INFO` & `undertext-0.2.0/src/undertext.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: undertext
-Version: 0.1.0
+Version: 0.2.0
 Summary: library to load, edit and save different formats of subtitles
 Home-page: https://github.com/utility-libraries/undertext-py
 Author: PlayerG9
 License: MIT
 Project-URL: Organisation Github, https://github.com/utility-libraries
 Project-URL: Homepage, https://github.com/utility-libraries/undertext-py/
 Project-URL: Documentation, https://utility-libraries.github.io/undertext-py/
@@ -53,14 +53,15 @@
 ```
 
 ## File Formats
 
 | ext    | name                      | read  | write |
 |--------|---------------------------|-------|-------|
 | `.ass` | Advanced SubStation Alpha | ❌     | ❌     |
+| `.sbv` | SubViewer                 | ❌     | ✅     |
 | `.srt` | SubRip                    | ✅     | ✅     |
 | `.ssa` | Sub Station Alpha         | ❌     | ❌     |
 | `.sub` | MicroDVD                  | ✅     | ✅     |
 | `.vtt` | WebVTT                    | ✅     | ✅     |
 
 <small>Listed formats that are currently unsupported may be added at a later version</small>
```

### Comparing `undertext-0.1.0/src/undertext.egg-info/SOURCES.txt` & `undertext-0.2.0/src/undertext.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -11,14 +11,18 @@
 src/undertext.egg-info/dependency_links.txt
 src/undertext.egg-info/entry_points.txt
 src/undertext.egg-info/requires.txt
 src/undertext.egg-info/top_level.txt
 src/undertext/readers/__init__.py
 src/undertext/readers/microdvd.py
 src/undertext/readers/subrip.py
+src/undertext/readers/subviewer.py
 src/undertext/readers/webvtt.py
 src/undertext/structures/__init__.py
 src/undertext/structures/caption.py
+src/undertext/util/__init__.py
+src/undertext/util/time.py
 src/undertext/writers/__init__.py
 src/undertext/writers/microdvd.py
 src/undertext/writers/subrip.py
+src/undertext/writers/subviewer.py
 src/undertext/writers/webvtt.py
```

