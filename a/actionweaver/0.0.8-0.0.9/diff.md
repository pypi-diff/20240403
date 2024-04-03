# Comparing `tmp/actionweaver-0.0.8.tar.gz` & `tmp/actionweaver-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "actionweaver-0.0.8.tar", max compression
+gzip compressed data, was "actionweaver-0.0.9.tar", max compression
```

## Comparing `actionweaver-0.0.8.tar` & `actionweaver-0.0.9.tar`

### file list

```diff
@@ -1,44 +1,44 @@
--rw-r--r--   0        0        0    11357 2023-08-18 00:58:34.007393 actionweaver-0.0.8/LICENSE
--rw-r--r--   0        0        0    10409 2023-09-07 03:13:17.779911 actionweaver-0.0.8/README.md
--rw-r--r--   0        0        0      116 2023-09-07 03:13:17.780127 actionweaver-0.0.8/actionweaver/__init__.py
--rw-r--r--   0        0        0      118 2023-09-07 03:13:17.780297 actionweaver-0.0.8/actionweaver/actions/__init__.py
--rw-r--r--   0        0        0      320 2023-09-07 03:24:43.230875 actionweaver-0.0.8/actionweaver/actions/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0    10662 2023-09-07 03:33:09.363816 actionweaver-0.0.8/actionweaver/actions/__pycache__/action.cpython-39.pyc
--rw-r--r--   0        0        0     2463 2023-09-07 03:24:43.235355 actionweaver-0.0.8/actionweaver/actions/__pycache__/orchestration.cpython-39.pyc
--rw-r--r--   0        0        0    12119 2023-09-07 03:29:30.173957 actionweaver-0.0.8/actionweaver/actions/action.py
--rw-r--r--   0        0        0     1946 2023-09-07 03:13:17.780722 actionweaver-0.0.8/actionweaver/actions/orchestration.py
--rw-r--r--   0        0        0        0 2023-09-07 03:13:17.780786 actionweaver-0.0.8/actionweaver/llms/openai/__init__.py
--rw-r--r--   0        0        0      158 2023-09-07 03:24:43.312626 actionweaver-0.0.8/actionweaver/llms/openai/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0     6024 2023-09-10 15:46:44.082903 actionweaver-0.0.8/actionweaver/llms/openai/__pycache__/chat.cpython-39.pyc
--rw-r--r--   0        0        0     1748 2023-09-07 03:24:43.315911 actionweaver-0.0.8/actionweaver/llms/openai/__pycache__/functions.cpython-39.pyc
--rw-r--r--   0        0        0     1541 2023-09-07 03:24:43.317972 actionweaver-0.0.8/actionweaver/llms/openai/__pycache__/tokens.cpython-39.pyc
--rw-r--r--   0        0        0    11501 2023-09-10 15:45:45.244909 actionweaver-0.0.8/actionweaver/llms/openai/chat.py
--rw-r--r--   0        0        0     2071 2023-09-07 03:13:17.781303 actionweaver-0.0.8/actionweaver/llms/openai/functions.py
--rw-r--r--   0        0        0     1378 2023-09-07 03:13:17.782027 actionweaver-0.0.8/actionweaver/llms/openai/tokens.py
--rw-r--r--   0        0        0       53 2023-09-07 03:13:17.782367 actionweaver-0.0.8/actionweaver/mixins/__init__.py
--rw-r--r--   0        0        0      216 2023-09-07 03:24:43.295503 actionweaver-0.0.8/actionweaver/mixins/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0     3749 2023-09-07 03:24:43.296777 actionweaver-0.0.8/actionweaver/mixins/__pycache__/action_handler_mixin.cpython-39.pyc
--rw-r--r--   0        0        0     4090 2023-09-07 03:13:17.782542 actionweaver-0.0.8/actionweaver/mixins/action_handler_mixin.py
--rw-r--r--   0        0        0      255 2023-09-07 03:13:17.782732 actionweaver-0.0.8/actionweaver/mixins/examples/__init__.py
--rw-r--r--   0        0        0      287 2023-09-07 03:24:43.322362 actionweaver-0.0.8/actionweaver/mixins/examples/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0     2045 2023-09-07 03:24:43.324639 actionweaver-0.0.8/actionweaver/mixins/examples/__pycache__/folium.cpython-39.pyc
--rw-r--r--   0        0        0     1340 2023-09-07 15:10:38.492798 actionweaver-0.0.8/actionweaver/mixins/examples/__pycache__/langchain.cpython-39.pyc
--rw-r--r--   0        0        0     1188 2023-09-07 03:24:43.355365 actionweaver-0.0.8/actionweaver/mixins/examples/__pycache__/openai.cpython-39.pyc
--rw-r--r--   0        0        0     1524 2023-09-07 03:13:17.782925 actionweaver-0.0.8/actionweaver/mixins/examples/folium.py
--rw-r--r--   0        0        0     1049 2023-09-07 15:09:12.800036 actionweaver-0.0.8/actionweaver/mixins/examples/langchain.py
--rw-r--r--   0        0        0        0 2023-09-02 23:11:10.084119 actionweaver-0.0.8/actionweaver/mixins/examples/llama_index.py
--rw-r--r--   0        0        0      784 2023-09-07 03:13:17.783409 actionweaver-0.0.8/actionweaver/mixins/examples/openai.py
--rw-r--r--   0        0        0      107 2023-09-07 03:13:17.783612 actionweaver-0.0.8/actionweaver/utils/__init__.py
--rw-r--r--   0        0        0      279 2023-09-07 03:24:43.236495 actionweaver-0.0.8/actionweaver/utils/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0      203 2023-09-07 03:24:43.238244 actionweaver-0.0.8/actionweaver/utils/__pycache__/action_scope.cpython-39.pyc
--rw-r--r--   0        0        0     1052 2023-09-07 03:28:22.467916 actionweaver-0.0.8/actionweaver/utils/__pycache__/cache.cpython-39.pyc
--rw-r--r--   0        0        0      556 2023-09-07 15:29:25.093771 actionweaver-0.0.8/actionweaver/utils/__pycache__/output.cpython-39.pyc
--rw-r--r--   0        0        0     1592 2023-09-07 03:24:43.239116 actionweaver-0.0.8/actionweaver/utils/__pycache__/pydantic_utils.cpython-39.pyc
--rw-r--r--   0        0        0     1022 2023-09-07 03:24:43.320143 actionweaver-0.0.8/actionweaver/utils/__pycache__/stream.cpython-39.pyc
--rw-r--r--   0        0        0       48 2023-09-07 03:13:17.783772 actionweaver-0.0.8/actionweaver/utils/action_scope.py
--rw-r--r--   0        0        0      748 2023-09-07 03:13:17.783951 actionweaver-0.0.8/actionweaver/utils/cache.py
--rw-r--r--   0        0        0      502 2023-09-07 15:09:43.623199 actionweaver-0.0.8/actionweaver/utils/output.py
--rw-r--r--   0        0        0     2802 2023-09-07 03:13:17.784132 actionweaver-0.0.8/actionweaver/utils/pydantic_utils.py
--rw-r--r--   0        0        0      942 2023-09-07 03:13:17.784316 actionweaver-0.0.8/actionweaver/utils/stream.py
--rw-r--r--   0        0        0      435 2023-09-10 15:45:49.922932 actionweaver-0.0.8/pyproject.toml
--rw-r--r--   0        0        0    10955 1970-01-01 00:00:00.000000 actionweaver-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-08-18 00:58:34.007393 actionweaver-0.0.9/LICENSE
+-rw-r--r--   0        0        0    10409 2023-09-07 03:13:17.779911 actionweaver-0.0.9/README.md
+-rw-r--r--   0        0        0      116 2023-09-07 03:13:17.780127 actionweaver-0.0.9/actionweaver/__init__.py
+-rw-r--r--   0        0        0      118 2023-09-07 03:13:17.780297 actionweaver-0.0.9/actionweaver/actions/__init__.py
+-rw-r--r--   0        0        0      320 2023-09-07 03:24:43.230875 actionweaver-0.0.9/actionweaver/actions/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0    10662 2023-09-07 03:33:09.363816 actionweaver-0.0.9/actionweaver/actions/__pycache__/action.cpython-39.pyc
+-rw-r--r--   0        0        0     2463 2023-09-07 03:24:43.235355 actionweaver-0.0.9/actionweaver/actions/__pycache__/orchestration.cpython-39.pyc
+-rw-r--r--   0        0        0    12119 2023-09-07 03:29:30.173957 actionweaver-0.0.9/actionweaver/actions/action.py
+-rw-r--r--   0        0        0     1946 2023-09-07 03:13:17.780722 actionweaver-0.0.9/actionweaver/actions/orchestration.py
+-rw-r--r--   0        0        0        0 2023-09-07 03:13:17.780786 actionweaver-0.0.9/actionweaver/llms/openai/__init__.py
+-rw-r--r--   0        0        0      158 2023-09-07 03:24:43.312626 actionweaver-0.0.9/actionweaver/llms/openai/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0     6078 2023-09-10 17:35:39.472542 actionweaver-0.0.9/actionweaver/llms/openai/__pycache__/chat.cpython-39.pyc
+-rw-r--r--   0        0        0     1748 2023-09-07 03:24:43.315911 actionweaver-0.0.9/actionweaver/llms/openai/__pycache__/functions.cpython-39.pyc
+-rw-r--r--   0        0        0     1541 2023-09-07 03:24:43.317972 actionweaver-0.0.9/actionweaver/llms/openai/__pycache__/tokens.cpython-39.pyc
+-rw-r--r--   0        0        0    11644 2023-09-10 17:34:34.218692 actionweaver-0.0.9/actionweaver/llms/openai/chat.py
+-rw-r--r--   0        0        0     2071 2023-09-07 03:13:17.781303 actionweaver-0.0.9/actionweaver/llms/openai/functions.py
+-rw-r--r--   0        0        0     1378 2023-09-07 03:13:17.782027 actionweaver-0.0.9/actionweaver/llms/openai/tokens.py
+-rw-r--r--   0        0        0       53 2023-09-07 03:13:17.782367 actionweaver-0.0.9/actionweaver/mixins/__init__.py
+-rw-r--r--   0        0        0      216 2023-09-07 03:24:43.295503 actionweaver-0.0.9/actionweaver/mixins/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0     3749 2023-09-07 03:24:43.296777 actionweaver-0.0.9/actionweaver/mixins/__pycache__/action_handler_mixin.cpython-39.pyc
+-rw-r--r--   0        0        0     4090 2023-09-07 03:13:17.782542 actionweaver-0.0.9/actionweaver/mixins/action_handler_mixin.py
+-rw-r--r--   0        0        0      255 2023-09-07 03:13:17.782732 actionweaver-0.0.9/actionweaver/mixins/examples/__init__.py
+-rw-r--r--   0        0        0      287 2023-09-07 03:24:43.322362 actionweaver-0.0.9/actionweaver/mixins/examples/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0     2045 2023-09-07 03:24:43.324639 actionweaver-0.0.9/actionweaver/mixins/examples/__pycache__/folium.cpython-39.pyc
+-rw-r--r--   0        0        0     1340 2023-09-07 15:10:38.492798 actionweaver-0.0.9/actionweaver/mixins/examples/__pycache__/langchain.cpython-39.pyc
+-rw-r--r--   0        0        0     1188 2023-09-07 03:24:43.355365 actionweaver-0.0.9/actionweaver/mixins/examples/__pycache__/openai.cpython-39.pyc
+-rw-r--r--   0        0        0     1524 2023-09-07 03:13:17.782925 actionweaver-0.0.9/actionweaver/mixins/examples/folium.py
+-rw-r--r--   0        0        0     1049 2023-09-07 15:09:12.800036 actionweaver-0.0.9/actionweaver/mixins/examples/langchain.py
+-rw-r--r--   0        0        0        0 2023-09-02 23:11:10.084119 actionweaver-0.0.9/actionweaver/mixins/examples/llama_index.py
+-rw-r--r--   0        0        0      784 2023-09-07 03:13:17.783409 actionweaver-0.0.9/actionweaver/mixins/examples/openai.py
+-rw-r--r--   0        0        0      107 2023-09-07 03:13:17.783612 actionweaver-0.0.9/actionweaver/utils/__init__.py
+-rw-r--r--   0        0        0      279 2023-09-07 03:24:43.236495 actionweaver-0.0.9/actionweaver/utils/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0      203 2023-09-07 03:24:43.238244 actionweaver-0.0.9/actionweaver/utils/__pycache__/action_scope.cpython-39.pyc
+-rw-r--r--   0        0        0     1052 2023-09-07 03:28:22.467916 actionweaver-0.0.9/actionweaver/utils/__pycache__/cache.cpython-39.pyc
+-rw-r--r--   0        0        0      556 2023-09-07 15:29:25.093771 actionweaver-0.0.9/actionweaver/utils/__pycache__/output.cpython-39.pyc
+-rw-r--r--   0        0        0     1592 2023-09-07 03:24:43.239116 actionweaver-0.0.9/actionweaver/utils/__pycache__/pydantic_utils.cpython-39.pyc
+-rw-r--r--   0        0        0     1022 2023-09-07 03:24:43.320143 actionweaver-0.0.9/actionweaver/utils/__pycache__/stream.cpython-39.pyc
+-rw-r--r--   0        0        0       48 2023-09-07 03:13:17.783772 actionweaver-0.0.9/actionweaver/utils/action_scope.py
+-rw-r--r--   0        0        0      748 2023-09-07 03:13:17.783951 actionweaver-0.0.9/actionweaver/utils/cache.py
+-rw-r--r--   0        0        0      502 2023-09-07 15:09:43.623199 actionweaver-0.0.9/actionweaver/utils/output.py
+-rw-r--r--   0        0        0     2802 2023-09-07 03:13:17.784132 actionweaver-0.0.9/actionweaver/utils/pydantic_utils.py
+-rw-r--r--   0        0        0      942 2023-09-07 03:13:17.784316 actionweaver-0.0.9/actionweaver/utils/stream.py
+-rw-r--r--   0        0        0      435 2023-09-10 17:34:36.778196 actionweaver-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0    10955 1970-01-01 00:00:00.000000 actionweaver-0.0.9/PKG-INFO
```

### Comparing `actionweaver-0.0.8/LICENSE` & `actionweaver-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `actionweaver-0.0.8/README.md` & `actionweaver-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `actionweaver-0.0.8/actionweaver/actions/__pycache__/action.cpython-39.pyc` & `actionweaver-0.0.9/actionweaver/actions/__pycache__/action.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `actionweaver-0.0.8/actionweaver/actions/__pycache__/orchestration.cpython-39.pyc` & `actionweaver-0.0.9/actionweaver/actions/__pycache__/orchestration.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `actionweaver-0.0.8/actionweaver/actions/action.py` & `actionweaver-0.0.9/actionweaver/actions/action.py`

 * *Files identical despite different names*

### Comparing `actionweaver-0.0.8/actionweaver/actions/orchestration.py` & `actionweaver-0.0.9/actionweaver/actions/orchestration.py`

 * *Files identical despite different names*

### Comparing `actionweaver-0.0.8/actionweaver/llms/openai/__pycache__/chat.cpython-39.pyc` & `actionweaver-0.0.9/actionweaver/llms/openai/__pycache__/chat.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Sun Sep 10 15:45:45 2023 UTC, .py size: 11501 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 a9e4 fd64 ed2c 0000  a..........d.,..
+00000000: 610d 0d0a 0000 0000 2afe fd64 7c2d 0000  a.......*..d|-..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 b200 0000 6400  .....@...s....d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a01 6400  d.l.Z.d.d.l.Z.d.
 00000040: 6401 6c02 5a02 6400 6401 6c03 5a03 6400  d.l.Z.d.d.l.Z.d.
 00000050: 6401 6c04 5a04 6400 6402 6c05 6d06 5a06  d.l.Z.d.d.l.m.Z.
 00000060: 0100 6400 6403 6c07 6d08 5a08 6d09 5a09  ..d.d.l.m.Z.m.Z.
 00000070: 6d0a 5a0a 0100 6400 6404 6c0b 6d0c 5a0c  m.Z...d.d.l.m.Z.
@@ -185,193 +185,196 @@
 00000b80: fb04 0820 0102 0202 0102 fe04 ff06 0606  ... ............
 00000b90: 0202 0102 0102 0102 0106 0102 fa04 ff04  ................
 00000ba0: 0a7a 254f 7065 6e41 4943 6861 7443 6f6d  .z%OpenAIChatCom
 00000bb0: 706c 6574 696f 6e2e 5f69 6e76 6f6b 655f  pletion._invoke_
 00000bc0: 6675 6e63 7469 6f6e 4629 03da 0573 636f  functionF)...sco
 00000bd0: 7065 da09 6f72 6368 5f65 7870 72da 0673  pe..orch_expr..s
 00000be0: 7472 6561 6d63 0200 0000 0000 0000 0300  treamc..........
-00000bf0: 0000 1a00 0000 0900 0000 4f00 0000 73c2  ..........O...s.
+00000bf0: 0000 1b00 0000 0900 0000 4f00 0000 73d2  ..........O...s.
 00000c00: 0200 0074 0074 01a0 02a1 0083 017d 077c  ...t.t.......}.|
-00000c10: 06a0 0364 017c 006a 04a1 027d 087c 006a  ...d.|.j...}.|.j
-00000c20: 05a0 06a1 0001 007c 0264 0275 0072 3074  .......|.d.u.r0t
-00000c30: 077d 0274 087c 0283 017d 097c 006a 096a  .}.t.|...}.|.j.j
-00000c40: 0a7d 0a7c 0364 0275 0172 827c 006a 096a  .}.|.d.u.r.|.j.j
-00000c50: 0ba0 0c7c 03a1 0101 0064 037d 0274 0d7c  ...|.....d.}.t.|
-00000c60: 0267 017c 0317 0083 017d 0b74 087c 0283  .g.|.....}.t.|..
-00000c70: 017d 097c 0ba0 0e7c 02a1 017c 0b7c 093c  .}.|...|...|.|.<
-00000c80: 007c 0b7d 0a7c 006a 0fa0 1064 047c 087c  .|.}.|.j...d.|.|
-00000c90: 027c 0174 11a0 11a1 007c 0764 059c 06a1  .|.t.....|.d....
-00000ca0: 0101 0064 027d 0c74 12a0 137c 0a7c 0919  ...d.}.t...|.|..
-00000cb0: 007c 006a 09a1 027d 0d7c 006a 0fa0 1064  .|.j...}.|.j...d
-00000cc0: 067c 077c 017c 087c 0274 11a0 11a1 0064  .|.|.|.|.t.....d
-00000cd0: 079c 067c 0da0 14a1 00a5 01a1 0101 007c  ...|...........|
-00000ce0: 0da0 14a1 007d 0e7c 0e64 0819 0090 0172  .....}.|.d.....r
-00000cf0: 0a74 156a 166a 1766 007c 087c 017c 0464  .t.j.j.f.|.|.|.d
-00000d00: 099c 037c 0ea4 018e 017d 0f6e 1274 156a  ...|.....}.n.t.j
-00000d10: 166a 177c 087c 017c 0464 098d 037d 0f74  .j.|.|.|.d...}.t
-00000d20: 187c 0f83 0190 0172 e874 197c 0f83 015c  .|.....r.t.|...\
-00000d30: 027d 107d 1164 0a7c 106a 1a64 0b19 0064  .}.}.d.|.j.d...d
-00000d40: 0c19 0076 0090 0172 6474 1b7c 106a 1a64  ...v...rdt.|.j.d
-00000d50: 0b19 0064 0c19 0064 0a19 0074 0083 0290  ...d...d...t....
-00000d60: 0172 647c 1153 0064 0d7c 106a 1a64 0b19  .rd|.S.d.|.j.d..
-00000d70: 0064 0c19 0076 0090 0172 d474 1c7c 1183  .d...v...r.t.|..
-00000d80: 017d 1269 007d 137c 1244 005d 247d 147c  .}.i.}.|.D.]$}.|
-00000d90: 1464 0e19 0064 0b19 0064 0c19 00a0 1da1  .d...d...d......
-00000da0: 007d 1574 1e7c 137c 1583 027d 1390 0171  .}.t.|.|...}...q
-00000db0: 887c 137c 1064 0e19 0064 0b19 0064 0f3c  .|.|.d...d...d.<
-00000dc0: 007c 137c 1064 0e19 0064 0b19 0064 0c3c  .|.|.d...d...d.<
-00000dd0: 007c 107d 0f6e 1274 1f64 1074 1c7c 1183  .|.}.n.t.d.t.|..
-00000de0: 019b 009d 0283 0182 016e 0e7c 006a 05a0  .........n.|.j..
-00000df0: 207c 0f6a 21a1 0101 007c 006a 0fa0 1064   |.j!....|.j...d
-00000e00: 117c 0f74 11a0 11a1 007c 0764 129c 04a1  .|.t.....|.d....
-00000e10: 0101 007c 0f6a 1a64 0b19 007d 167c 1664  ...|.j.d...}.|.d
-00000e20: 0f19 007d 1764 0d7c 1776 0090 0272 647c  ...}.d.|.v...rd|
-00000e30: 1764 0d19 0090 0272 647c 00a0 227c 077c  .d.....rd|.."|.|
-00000e40: 017c 087c 1764 0d19 007c 0a7c 097c 0da1  .|.|.d...|.|.|..
-00000e50: 075c 027d 0d5c 027d 187d 197c 1890 0272  .\.}.\.}.}.|...r
-00000e60: bc7c 1953 0071 b664 0a7c 1776 0090 0272  .|.S.q.d.|.v...r
-00000e70: ae7c 1764 0a19 0090 0272 ae7c 1764 0a19  .|.d.....r.|.d..
-00000e80: 007d 0c7c 1664 1319 0064 146b 0290 0272  .}.|.d...d.k...r
-00000e90: bc7c 006a 0fa0 1064 157c 0874 11a0 11a1  .|.j...d.|.t....
-00000ea0: 007c 0764 169c 04a1 0101 0090 0271 be71  .|.d.........q.q
-00000eb0: b674 1f64 177c 0f9b 009d 0283 0182 0171  .t.d.|.........q
-00000ec0: b67c 0c53 0029 1861 5702 0000 0a20 2020  .|.S.).aW....   
-00000ed0: 2020 2020 2049 6e76 6f6b 6520 7468 6520       Invoke the 
-00000ee0: 4f70 656e 4149 2041 5049 2077 6974 6820  OpenAI API with 
-00000ef0: 7468 6520 7072 6f76 6964 6564 206d 6573  the provided mes
-00000f00: 7361 6765 7320 616e 6420 6675 6e63 7469  sages and functi
-00000f10: 6f6e 732e 0a0a 2020 2020 2020 2020 4675  ons...        Fu
-00000f20: 6e63 7469 6f6e 7320 7375 7070 6c69 6564  nctions supplied
-00000f30: 2074 6f20 7468 6520 4150 4920 6172 6520   to the API are 
-00000f40: 6465 7465 726d 696e 6564 2062 7920 7468  determined by th
-00000f50: 6520 7370 6563 6966 6965 6420 7363 6f70  e specified scop
-00000f60: 6520 616e 6420 6f72 6368 6573 7472 6174  e and orchestrat
-00000f70: 696f 6e20 6578 7072 6573 7369 6f6e 2e0a  ion expression..
-00000f80: 0a20 2020 2020 2020 2041 7267 733a 0a20  .        Args:. 
-00000f90: 2020 2020 2020 2020 2020 206d 6573 7361             messa
-00000fa0: 6765 7320 286c 6973 7429 3a20 4c69 7374  ges (list): List
-00000fb0: 206f 6620 6d65 7373 6167 6520 6f62 6a65   of message obje
-00000fc0: 6374 7320 666f 7220 7468 6520 636f 6e76  cts for the conv
-00000fd0: 6572 7361 7469 6f6e 2e0a 2020 2020 2020  ersation..      
-00000fe0: 2020 2020 2020 7363 6f70 6520 2873 7472        scope (str
-00000ff0: 293a 2053 636f 7065 206f 6620 7468 6520  ): Scope of the 
-00001000: 6675 6e63 7469 6f6e 7320 746f 2062 6520  functions to be 
-00001010: 7573 6564 2e0a 2020 2020 2020 2020 2020  used..          
-00001020: 2020 6f72 6368 5f65 7870 723a 2049 6620    orch_expr: If 
-00001030: 7370 6563 6966 6965 642c 206f 7665 7272  specified, overr
-00001040: 6964 6573 2074 6865 206f 7263 6865 7374  ides the orchest
-00001050: 7261 7469 6f6e 2064 6963 7469 6f6e 6172  ration dictionar
-00001060: 792c 2064 6574 6572 6d69 6e69 6e67 2074  y, determining t
-00001070: 6865 2041 5049 2063 616c 6c20 666c 6f77  he API call flow
-00001080: 2e0a 2020 2020 2020 2020 2020 2020 7374  ..            st
-00001090: 7265 616d 2028 626f 6f6c 293a 2049 6620  ream (bool): If 
-000010a0: 5472 7565 2c20 7265 7475 726e 7320 6120  True, returns a 
-000010b0: 6765 6e65 7261 746f 7220 7468 6174 2079  generator that y
-000010c0: 6965 6c64 7320 7468 6520 4150 4920 7265  ields the API re
-000010d0: 7370 6f6e 7365 732e 0a0a 2020 2020 2020  sponses...      
-000010e0: 2020 5265 7475 726e 733a 0a20 2020 2020    Returns:.     
-000010f0: 2020 2020 2020 2041 5049 2072 6573 706f         API respo
-00001100: 6e73 6520 7769 7468 2067 656e 6572 6174  nse with generat
-00001110: 6564 206f 7574 7075 742e 0a20 2020 2020  ed output..     
-00001120: 2020 2072 1600 0000 4e5a 125f 6c6c 6d5f     r....NZ._llm_
-00001130: 6f72 6368 6573 7472 6174 696f 6e7a 1c43  orchestrationz.C
-00001140: 7265 6174 696e 6720 6e65 7720 6368 6174  reating new chat
-00001150: 2063 6f6d 706c 6574 696f 6e29 0672 2500   completion).r%.
-00001160: 0000 7216 0000 0072 4800 0000 da0e 696e  ..r....rH.....in
-00001170: 7075 745f 6d65 7373 6167 6573 7226 0000  put_messagesr&..
-00001180: 0072 2700 0000 7a12 4361 6c6c 696e 6720  .r'...z.Calling 
-00001190: 4f70 656e 4149 2041 5049 2906 7225 0000  OpenAI API).r%..
-000011a0: 0072 2700 0000 724b 0000 0072 1600 0000  .r'...rK...r....
-000011b0: 7248 0000 0072 2600 0000 7241 0000 0029  rH...r&...rA...)
-000011c0: 0372 1600 0000 7242 0000 0072 4a00 0000  .r....rB...rJ...
-000011d0: 7221 0000 0072 0100 0000 da05 6465 6c74  r!...r......delt
-000011e0: 6172 2200 0000 da07 6368 6f69 6365 7372  ar".....choicesr
-000011f0: 2500 0000 7a29 556e 7375 7070 6f72 7465  %...z)Unsupporte
-00001200: 6420 7265 7370 6f6e 7365 2066 726f 6d20  d response from 
-00001210: 7374 7265 616d 696e 6720 4150 493a 207a  streaming API: z
-00001220: 2152 6563 6569 7665 6420 7265 7370 6f6e  !Received respon
-00001230: 7365 2066 726f 6d20 4f70 656e 4149 2041  se from OpenAI A
-00001240: 5049 2904 7225 0000 00da 0872 6573 706f  PI).r%.....respo
-00001250: 6e73 6572 2600 0000 7227 0000 005a 0d66  nser&...r'...Z.f
-00001260: 696e 6973 685f 7265 6173 6f6e 722d 0000  inish_reasonr-..
-00001270: 007a 154d 6f64 656c 2064 6563 6964 6573  .z.Model decides
-00001280: 2074 6f20 7374 6f70 2904 7225 0000 0072   to stop).r%...r
-00001290: 1600 0000 7226 0000 0072 2700 0000 7a26  ....r&...r'...z&
-000012a0: 556e 7375 7070 6f72 7465 6420 7265 7370  Unsupported resp
-000012b0: 6f6e 7365 2066 726f 6d20 4f70 656e 4149  onse from OpenAI
-000012c0: 2061 7069 3a20 2923 723d 0000 00da 0475   api: )#r=.....u
-000012d0: 7569 64da 0575 7569 6434 da03 6765 7472  uid..uuid4..getr
-000012e0: 1600 0000 721b 0000 00da 0563 6c65 6172  ....r......clear
-000012f0: 720a 0000 0072 0700 0000 7218 0000 00da  r....r....r.....
-00001300: 096f 7263 685f 6469 6374 da0f 6163 7469  .orch_dict..acti
-00001310: 6f6e 5f68 616e 646c 6572 73da 2163 6865  on_handlers.!che
-00001320: 636b 5f6f 7263 6865 7374 7261 7469 6f6e  ck_orchestration
-00001330: 5f65 7870 725f 7661 6c69 6469 7479 7205  _expr_validityr.
-00001340: 0000 00da 0370 6f70 7215 0000 0072 3e00  .....popr....r>.
-00001350: 0000 723b 0000 0072 0800 0000 723f 0000  ..r;...r....r?..
-00001360: 005a 0c74 6f5f 6172 6775 6d65 6e74 73da  .Z.to_arguments.
-00001370: 066f 7065 6e61 69da 0e43 6861 7443 6f6d  .openai..ChatCom
-00001380: 706c 6574 696f 6eda 0663 7265 6174 6572  pletion..creater
-00001390: 0c00 0000 720b 0000 0072 4d00 0000 7233  ....r....rM...r3
-000013a0: 0000 00da 046c 6973 7472 3400 0000 720d  .....listr4...r.
-000013b0: 0000 0072 0e00 0000 5a0b 7472 6163 6b5f  ...r....Z.track_
-000013c0: 7573 6167 65da 0575 7361 6765 7247 0000  usage..usagerG..
-000013d0: 0029 1a72 1c00 0000 7242 0000 0072 4800  .).r....rB...rH.
-000013e0: 0000 7249 0000 0072 4a00 0000 da04 6172  ..rI...rJ.....ar
-000013f0: 6773 da06 6b77 6172 6773 7227 0000 0072  gs..kwargsr'...r
-00001400: 1600 0000 7244 0000 0072 4300 0000 5a16  ....rD...rC...Z.
-00001410: 6e65 775f 6f72 6368 6573 7472 6174 696f  new_orchestratio
-00001420: 6e5f 6469 6374 724e 0000 0072 4100 0000  n_dictrN...rA...
-00001430: 5a11 6675 6e63 7469 6f6e 5f61 7267 756d  Z.function_argum
-00001440: 656e 745a 0c61 7069 5f72 6573 706f 6e73  entZ.api_respons
-00001450: 655a 0d66 6972 7374 5f65 6c65 6d65 6e74  eZ.first_element
-00001460: da08 6974 6572 6174 6f72 da01 6c5a 0664  ..iterator..lZ.d
-00001470: 656c 7461 73da 0765 6c65 6d65 6e74 724c  eltas..elementrL
-00001480: 0000 00da 0663 686f 6963 6572 2500 0000  .....choicer%...
-00001490: 722d 0000 00da 0472 6573 7072 1200 0000  r-.....respr....
-000014a0: 7212 0000 0072 1300 0000 7259 0000 008e  r....r....rY....
-000014b0: 0000 0073 dc00 0000 0013 0c02 0e03 0a02  ...s............
-000014c0: 0801 0401 0802 0802 0801 0801 02ff 0404  ................
-000014d0: 0402 0e03 0801 0e03 0402 0602 0201 0201  ................
-000014e0: 0201 0201 0601 02fa 04ff 040b 0401 0401  ................
-000014f0: 0601 04fe 0406 0602 0201 0201 0201 0201  ................
-00001500: 0201 06fa 0407 06f9 02ff 040c 0801 0a01  ................
-00001510: 0801 0201 0201 02fd 0404 02fc 0807 0601  ................
-00001520: 0201 0201 02fd 0607 0a01 0c02 1601 12ff  ................
-00001530: 0604 0401 1402 0802 0401 0801 1401 0e02  ................
-00001540: 1001 1001 0602 0201 0cff 0605 0e02 0602  ................
-00001550: 0201 0201 0601 02fc 04ff 0409 0a01 0802  ................
-00001560: 1401 0401 0201 0201 0201 0601 0201 0201  ................
-00001570: 02f9 0c09 0601 0601 1401 0804 0e08 0602  ................
-00001580: 0201 0201 0601 02fc 04ff 0409 0602 0201  ................
-00001590: 08ff 0603 7a1b 4f70 656e 4149 4368 6174  ....z.OpenAIChat
-000015a0: 436f 6d70 6c65 7469 6f6e 2e63 7265 6174  Completion.creat
-000015b0: 6529 024e 4e29 0872 0f00 0000 7210 0000  e).NN).r....r...
-000015c0: 0072 1100 0000 721d 0000 0072 0400 0000  .r....r....r....
-000015d0: 721f 0000 0072 4700 0000 7259 0000 0072  r....rG...rY...r
-000015e0: 1200 0000 7212 0000 0072 1200 0000 7213  ....r....r....r.
-000015f0: 0000 0072 1400 0000 1d00 0000 730a 0000  ...r........s...
-00001600: 0008 010a 0a0e 0308 6406 ff72 1400 0000  ........d..r....
-00001610: 291b 7236 0000 0072 1900 0000 723b 0000  ).r6...r....r;..
-00001620: 0072 4f00 0000 7257 0000 00da 146f 7065  .rO...rW.....ope
-00001630: 6e61 692e 6f70 656e 6169 5f6f 626a 6563  nai.openai_objec
-00001640: 7472 0200 0000 da1b 6163 7469 6f6e 7765  tr......actionwe
-00001650: 6176 6572 2e61 6374 696f 6e73 2e61 6374  aver.actions.act
-00001660: 696f 6e72 0300 0000 7204 0000 0072 0500  ionr....r....r..
-00001670: 0000 da22 6163 7469 6f6e 7765 6176 6572  ..."actionweaver
-00001680: 2e61 6374 696f 6e73 2e6f 7263 6865 7374  .actions.orchest
-00001690: 7261 7469 6f6e 7206 0000 0072 0700 0000  rationr....r....
-000016a0: 5a22 6163 7469 6f6e 7765 6176 6572 2e6c  Z"actionweaver.l
-000016b0: 6c6d 732e 6f70 656e 6169 2e66 756e 6374  lms.openai.funct
-000016c0: 696f 6e73 7208 0000 00da 1f61 6374 696f  ionsr......actio
-000016d0: 6e77 6561 7665 722e 6c6c 6d73 2e6f 7065  nweaver.llms.ope
-000016e0: 6e61 692e 746f 6b65 6e73 7209 0000 00da  nai.tokensr.....
-000016f0: 1261 6374 696f 6e77 6561 7665 722e 7574  .actionweaver.ut
-00001700: 696c 7372 0a00 0000 5a19 6163 7469 6f6e  ilsr....Z.action
-00001710: 7765 6176 6572 2e75 7469 6c73 2e73 7472  weaver.utils.str
-00001720: 6561 6d72 0b00 0000 720c 0000 0072 0d00  eamr....r....r..
-00001730: 0000 da09 4578 6365 7074 696f 6e72 0e00  ....Exceptionr..
-00001740: 0000 7214 0000 0072 1200 0000 7212 0000  ..r....r....r...
-00001750: 0072 1200 0000 7213 0000 00da 083c 6d6f  .r....r......<mo
-00001760: 6475 6c65 3e01 0000 0073 1a00 0000 0801  dule>....s......
-00001770: 0801 0801 0802 0801 0c02 1405 1001 0c01  ................
-00001780: 0c01 0c01 1407 1004                      ........
+00000c10: 06a0 0364 017c 006a 04a1 027d 087c 06a0  ...d.|.j...}.|..
+00000c20: 0364 0264 03a1 027d 097c 006a 05a0 06a1  .d.d...}.|.j....
+00000c30: 0001 007c 0264 0475 0072 3c74 077d 0274  ...|.d.u.r<t.}.t
+00000c40: 087c 0283 017d 0a7c 006a 096a 0a7d 0b7c  .|...}.|.j.j.}.|
+00000c50: 0364 0475 0172 8e7c 006a 096a 0ba0 0c7c  .d.u.r.|.j.j...|
+00000c60: 03a1 0101 0064 057d 0274 0d7c 0267 017c  .....d.}.t.|.g.|
+00000c70: 0317 0083 017d 0c74 087c 0283 017d 0a7c  .....}.t.|...}.|
+00000c80: 0ca0 0e7c 02a1 017c 0c7c 0a3c 007c 0c7d  ...|...|.|.<.|.}
+00000c90: 0b7c 006a 0fa0 1064 067c 087c 027c 0174  .|.j...d.|.|.|.t
+00000ca0: 11a0 11a1 007c 0764 079c 06a1 0101 0064  .....|.d.......d
+00000cb0: 047d 0d74 12a0 137c 0b7c 0a19 007c 006a  .}.t...|.|...|.j
+00000cc0: 09a1 027d 0e7c 006a 0fa0 1064 087c 077c  ...}.|.j...d.|.|
+00000cd0: 017c 087c 0274 11a0 11a1 0064 099c 067c  .|.|.t.....d...|
+00000ce0: 0ea0 14a1 00a5 01a1 0101 007c 0ea0 14a1  ...........|....
+00000cf0: 007d 0f7c 0f64 0a19 0090 0172 1874 156a  .}.|.d.....r.t.j
+00000d00: 166a 1766 007c 087c 097c 017c 0464 0b9c  .j.f.|.|.|.|.d..
+00000d10: 047c 0fa4 018e 017d 106e 1474 156a 166a  .|.....}.n.t.j.j
+00000d20: 177c 087c 097c 017c 0464 0b8d 047d 1074  .|.|.|.|.d...}.t
+00000d30: 187c 1083 0190 0172 f874 197c 1083 015c  .|.....r.t.|...\
+00000d40: 027d 117d 1264 0c7c 116a 1a64 0d19 0064  .}.}.d.|.j.d...d
+00000d50: 0e19 0076 0090 0172 7474 1b7c 116a 1a64  ...v...rtt.|.j.d
+00000d60: 0d19 0064 0e19 0064 0c19 0074 0083 0290  ...d...d...t....
+00000d70: 0172 747c 1253 0064 0f7c 116a 1a64 0d19  .rt|.S.d.|.j.d..
+00000d80: 0064 0e19 0076 0090 0172 e474 1c7c 1283  .d...v...r.t.|..
+00000d90: 017d 1369 007d 147c 1344 005d 247d 157c  .}.i.}.|.D.]$}.|
+00000da0: 1564 1019 0064 0d19 0064 0e19 00a0 1da1  .d...d...d......
+00000db0: 007d 1674 1e7c 147c 1683 027d 1490 0171  .}.t.|.|...}...q
+00000dc0: 987c 147c 1164 1019 0064 0d19 0064 113c  .|.|.d...d...d.<
+00000dd0: 007c 147c 1164 1019 0064 0d19 0064 0e3c  .|.|.d...d...d.<
+00000de0: 007c 117d 106e 1274 1f64 1274 1c7c 1283  .|.}.n.t.d.t.|..
+00000df0: 019b 009d 0283 0182 016e 0e7c 006a 05a0  .........n.|.j..
+00000e00: 207c 106a 21a1 0101 007c 006a 0fa0 1064   |.j!....|.j...d
+00000e10: 137c 1074 11a0 11a1 007c 0764 149c 04a1  .|.t.....|.d....
+00000e20: 0101 007c 106a 1a64 0d19 007d 177c 1764  ...|.j.d...}.|.d
+00000e30: 1119 007d 1864 0f7c 1876 0090 0272 747c  ...}.d.|.v...rt|
+00000e40: 1864 0f19 0090 0272 747c 00a0 227c 077c  .d.....rt|.."|.|
+00000e50: 017c 087c 1864 0f19 007c 0b7c 0a7c 0ea1  .|.|.d...|.|.|..
+00000e60: 075c 027d 0e5c 027d 197d 1a7c 1990 0272  .\.}.\.}.}.|...r
+00000e70: cc7c 1a53 0071 c264 0c7c 1876 0090 0272  .|.S.q.d.|.v...r
+00000e80: be7c 1864 0c19 0090 0272 be7c 1864 0c19  .|.d.....r.|.d..
+00000e90: 007d 0d7c 1764 1519 0064 166b 0290 0272  .}.|.d...d.k...r
+00000ea0: cc7c 006a 0fa0 1064 177c 0874 11a0 11a1  .|.j...d.|.t....
+00000eb0: 007c 0764 189c 04a1 0101 0090 0271 ce71  .|.d.........q.q
+00000ec0: c274 1f64 197c 109b 009d 0283 0182 0171  .t.d.|.........q
+00000ed0: c27c 0d53 0029 1a61 5702 0000 0a20 2020  .|.S.).aW....   
+00000ee0: 2020 2020 2049 6e76 6f6b 6520 7468 6520       Invoke the 
+00000ef0: 4f70 656e 4149 2041 5049 2077 6974 6820  OpenAI API with 
+00000f00: 7468 6520 7072 6f76 6964 6564 206d 6573  the provided mes
+00000f10: 7361 6765 7320 616e 6420 6675 6e63 7469  sages and functi
+00000f20: 6f6e 732e 0a0a 2020 2020 2020 2020 4675  ons...        Fu
+00000f30: 6e63 7469 6f6e 7320 7375 7070 6c69 6564  nctions supplied
+00000f40: 2074 6f20 7468 6520 4150 4920 6172 6520   to the API are 
+00000f50: 6465 7465 726d 696e 6564 2062 7920 7468  determined by th
+00000f60: 6520 7370 6563 6966 6965 6420 7363 6f70  e specified scop
+00000f70: 6520 616e 6420 6f72 6368 6573 7472 6174  e and orchestrat
+00000f80: 696f 6e20 6578 7072 6573 7369 6f6e 2e0a  ion expression..
+00000f90: 0a20 2020 2020 2020 2041 7267 733a 0a20  .        Args:. 
+00000fa0: 2020 2020 2020 2020 2020 206d 6573 7361             messa
+00000fb0: 6765 7320 286c 6973 7429 3a20 4c69 7374  ges (list): List
+00000fc0: 206f 6620 6d65 7373 6167 6520 6f62 6a65   of message obje
+00000fd0: 6374 7320 666f 7220 7468 6520 636f 6e76  cts for the conv
+00000fe0: 6572 7361 7469 6f6e 2e0a 2020 2020 2020  ersation..      
+00000ff0: 2020 2020 2020 7363 6f70 6520 2873 7472        scope (str
+00001000: 293a 2053 636f 7065 206f 6620 7468 6520  ): Scope of the 
+00001010: 6675 6e63 7469 6f6e 7320 746f 2062 6520  functions to be 
+00001020: 7573 6564 2e0a 2020 2020 2020 2020 2020  used..          
+00001030: 2020 6f72 6368 5f65 7870 723a 2049 6620    orch_expr: If 
+00001040: 7370 6563 6966 6965 642c 206f 7665 7272  specified, overr
+00001050: 6964 6573 2074 6865 206f 7263 6865 7374  ides the orchest
+00001060: 7261 7469 6f6e 2064 6963 7469 6f6e 6172  ration dictionar
+00001070: 792c 2064 6574 6572 6d69 6e69 6e67 2074  y, determining t
+00001080: 6865 2041 5049 2063 616c 6c20 666c 6f77  he API call flow
+00001090: 2e0a 2020 2020 2020 2020 2020 2020 7374  ..            st
+000010a0: 7265 616d 2028 626f 6f6c 293a 2049 6620  ream (bool): If 
+000010b0: 5472 7565 2c20 7265 7475 726e 7320 6120  True, returns a 
+000010c0: 6765 6e65 7261 746f 7220 7468 6174 2079  generator that y
+000010d0: 6965 6c64 7320 7468 6520 4150 4920 7265  ields the API re
+000010e0: 7370 6f6e 7365 732e 0a0a 2020 2020 2020  sponses...      
+000010f0: 2020 5265 7475 726e 733a 0a20 2020 2020    Returns:.     
+00001100: 2020 2020 2020 2041 5049 2072 6573 706f         API respo
+00001110: 6e73 6520 7769 7468 2067 656e 6572 6174  nse with generat
+00001120: 6564 206f 7574 7075 742e 0a20 2020 2020  ed output..     
+00001130: 2020 2072 1600 0000 da0b 7465 6d70 6572     r......temper
+00001140: 6174 7572 6567 0000 0000 0000 0000 4e5a  atureg........NZ
+00001150: 125f 6c6c 6d5f 6f72 6368 6573 7472 6174  ._llm_orchestrat
+00001160: 696f 6e7a 1c43 7265 6174 696e 6720 6e65  ionz.Creating ne
+00001170: 7720 6368 6174 2063 6f6d 706c 6574 696f  w chat completio
+00001180: 6e29 0672 2500 0000 7216 0000 0072 4800  n).r%...r....rH.
+00001190: 0000 da0e 696e 7075 745f 6d65 7373 6167  ....input_messag
+000011a0: 6573 7226 0000 0072 2700 0000 7a12 4361  esr&...r'...z.Ca
+000011b0: 6c6c 696e 6720 4f70 656e 4149 2041 5049  lling OpenAI API
+000011c0: 2906 7225 0000 0072 2700 0000 724c 0000  ).r%...r'...rL..
+000011d0: 0072 1600 0000 7248 0000 0072 2600 0000  .r....rH...r&...
+000011e0: 7241 0000 0029 0472 1600 0000 724b 0000  rA...).r....rK..
+000011f0: 0072 4200 0000 724a 0000 0072 2100 0000  .rB...rJ...r!...
+00001200: 7201 0000 00da 0564 656c 7461 7222 0000  r......deltar"..
+00001210: 00da 0763 686f 6963 6573 7225 0000 007a  ...choicesr%...z
+00001220: 2955 6e73 7570 706f 7274 6564 2072 6573  )Unsupported res
+00001230: 706f 6e73 6520 6672 6f6d 2073 7472 6561  ponse from strea
+00001240: 6d69 6e67 2041 5049 3a20 7a21 5265 6365  ming API: z!Rece
+00001250: 6976 6564 2072 6573 706f 6e73 6520 6672  ived response fr
+00001260: 6f6d 204f 7065 6e41 4920 4150 4929 0472  om OpenAI API).r
+00001270: 2500 0000 da08 7265 7370 6f6e 7365 7226  %.....responser&
+00001280: 0000 0072 2700 0000 5a0d 6669 6e69 7368  ...r'...Z.finish
+00001290: 5f72 6561 736f 6e72 2d00 0000 7a15 4d6f  _reasonr-...z.Mo
+000012a0: 6465 6c20 6465 6369 6465 7320 746f 2073  del decides to s
+000012b0: 746f 7029 0472 2500 0000 7216 0000 0072  top).r%...r....r
+000012c0: 2600 0000 7227 0000 007a 2655 6e73 7570  &...r'...z&Unsup
+000012d0: 706f 7274 6564 2072 6573 706f 6e73 6520  ported response 
+000012e0: 6672 6f6d 204f 7065 6e41 4920 6170 693a  from OpenAI api:
+000012f0: 2029 2372 3d00 0000 da04 7575 6964 da05   )#r=.....uuid..
+00001300: 7575 6964 34da 0367 6574 7216 0000 0072  uuid4..getr....r
+00001310: 1b00 0000 da05 636c 6561 7272 0a00 0000  ......clearr....
+00001320: 7207 0000 0072 1800 0000 da09 6f72 6368  r....r......orch
+00001330: 5f64 6963 74da 0f61 6374 696f 6e5f 6861  _dict..action_ha
+00001340: 6e64 6c65 7273 da21 6368 6563 6b5f 6f72  ndlers.!check_or
+00001350: 6368 6573 7472 6174 696f 6e5f 6578 7072  chestration_expr
+00001360: 5f76 616c 6964 6974 7972 0500 0000 da03  _validityr......
+00001370: 706f 7072 1500 0000 723e 0000 0072 3b00  popr....r>...r;.
+00001380: 0000 7208 0000 0072 3f00 0000 5a0c 746f  ..r....r?...Z.to
+00001390: 5f61 7267 756d 656e 7473 da06 6f70 656e  _arguments..open
+000013a0: 6169 da0e 4368 6174 436f 6d70 6c65 7469  ai..ChatCompleti
+000013b0: 6f6e da06 6372 6561 7465 720c 0000 0072  on..creater....r
+000013c0: 0b00 0000 724e 0000 0072 3300 0000 da04  ....rN...r3.....
+000013d0: 6c69 7374 7234 0000 0072 0d00 0000 720e  listr4...r....r.
+000013e0: 0000 005a 0b74 7261 636b 5f75 7361 6765  ...Z.track_usage
+000013f0: da05 7573 6167 6572 4700 0000 291b 721c  ..usagerG...).r.
+00001400: 0000 0072 4200 0000 7248 0000 0072 4900  ...rB...rH...rI.
+00001410: 0000 724a 0000 00da 0461 7267 73da 066b  ..rJ.....args..k
+00001420: 7761 7267 7372 2700 0000 7216 0000 0072  wargsr'...r....r
+00001430: 4b00 0000 7244 0000 0072 4300 0000 5a16  K...rD...rC...Z.
+00001440: 6e65 775f 6f72 6368 6573 7472 6174 696f  new_orchestratio
+00001450: 6e5f 6469 6374 724f 0000 0072 4100 0000  n_dictrO...rA...
+00001460: 5a11 6675 6e63 7469 6f6e 5f61 7267 756d  Z.function_argum
+00001470: 656e 745a 0c61 7069 5f72 6573 706f 6e73  entZ.api_respons
+00001480: 655a 0d66 6972 7374 5f65 6c65 6d65 6e74  eZ.first_element
+00001490: da08 6974 6572 6174 6f72 da01 6c5a 0664  ..iterator..lZ.d
+000014a0: 656c 7461 73da 0765 6c65 6d65 6e74 724d  eltas..elementrM
+000014b0: 0000 00da 0663 686f 6963 6572 2500 0000  .....choicer%...
+000014c0: 722d 0000 00da 0472 6573 7072 1200 0000  r-.....respr....
+000014d0: 7212 0000 0072 1300 0000 725a 0000 008e  r....r....rZ....
+000014e0: 0000 0073 e200 0000 0013 0c02 0e01 0c03  ...s............
+000014f0: 0a02 0801 0401 0802 0802 0801 0801 02ff  ................
+00001500: 0404 0402 0e03 0801 0e03 0402 0602 0201  ................
+00001510: 0201 0201 0201 0601 02fa 04ff 040b 0401  ................
+00001520: 0401 0601 04fe 0406 0602 0201 0201 0201  ................
+00001530: 0201 0201 06fa 0407 06f9 02ff 040c 0801  ................
+00001540: 0a01 0801 0201 0201 0201 02fc 0405 02fb  ................
+00001550: 0808 0601 0201 0201 0201 02fc 0608 0a01  ................
+00001560: 0c02 1601 12ff 0604 0401 1402 0802 0401  ................
+00001570: 0801 1401 0e02 1001 1001 0602 0201 0cff  ................
+00001580: 0605 0e02 0602 0201 0201 0601 02fc 04ff  ................
+00001590: 0409 0a01 0802 1401 0401 0201 0201 0201  ................
+000015a0: 0601 0201 0201 02f9 0c09 0601 0601 1401  ................
+000015b0: 0804 0e08 0602 0201 0201 0601 02fc 04ff  ................
+000015c0: 0409 0602 0201 08ff 0603 7a1b 4f70 656e  ..........z.Open
+000015d0: 4149 4368 6174 436f 6d70 6c65 7469 6f6e  AIChatCompletion
+000015e0: 2e63 7265 6174 6529 024e 4e29 0872 0f00  .create).NN).r..
+000015f0: 0000 7210 0000 0072 1100 0000 721d 0000  ..r....r....r...
+00001600: 0072 0400 0000 721f 0000 0072 4700 0000  .r....r....rG...
+00001610: 725a 0000 0072 1200 0000 7212 0000 0072  rZ...r....r....r
+00001620: 1200 0000 7213 0000 0072 1400 0000 1d00  ....r....r......
+00001630: 0000 730a 0000 0008 010a 0a0e 0308 6406  ..s...........d.
+00001640: ff72 1400 0000 291b 7236 0000 0072 1900  .r....).r6...r..
+00001650: 0000 723b 0000 0072 5000 0000 7258 0000  ..r;...rP...rX..
+00001660: 00da 146f 7065 6e61 692e 6f70 656e 6169  ...openai.openai
+00001670: 5f6f 626a 6563 7472 0200 0000 da1b 6163  _objectr......ac
+00001680: 7469 6f6e 7765 6176 6572 2e61 6374 696f  tionweaver.actio
+00001690: 6e73 2e61 6374 696f 6e72 0300 0000 7204  ns.actionr....r.
+000016a0: 0000 0072 0500 0000 da22 6163 7469 6f6e  ...r....."action
+000016b0: 7765 6176 6572 2e61 6374 696f 6e73 2e6f  weaver.actions.o
+000016c0: 7263 6865 7374 7261 7469 6f6e 7206 0000  rchestrationr...
+000016d0: 0072 0700 0000 5a22 6163 7469 6f6e 7765  .r....Z"actionwe
+000016e0: 6176 6572 2e6c 6c6d 732e 6f70 656e 6169  aver.llms.openai
+000016f0: 2e66 756e 6374 696f 6e73 7208 0000 00da  .functionsr.....
+00001700: 1f61 6374 696f 6e77 6561 7665 722e 6c6c  .actionweaver.ll
+00001710: 6d73 2e6f 7065 6e61 692e 746f 6b65 6e73  ms.openai.tokens
+00001720: 7209 0000 00da 1261 6374 696f 6e77 6561  r......actionwea
+00001730: 7665 722e 7574 696c 7372 0a00 0000 5a19  ver.utilsr....Z.
+00001740: 6163 7469 6f6e 7765 6176 6572 2e75 7469  actionweaver.uti
+00001750: 6c73 2e73 7472 6561 6d72 0b00 0000 720c  ls.streamr....r.
+00001760: 0000 0072 0d00 0000 da09 4578 6365 7074  ...r......Except
+00001770: 696f 6e72 0e00 0000 7214 0000 0072 1200  ionr....r....r..
+00001780: 0000 7212 0000 0072 1200 0000 7213 0000  ..r....r....r...
+00001790: 00da 083c 6d6f 6475 6c65 3e01 0000 0073  ...<module>....s
+000017a0: 1a00 0000 0801 0801 0801 0802 0801 0c02  ................
+000017b0: 1405 1001 0c01 0c01 0c01 1407 1004       ..............
```

### Comparing `actionweaver-0.0.8/actionweaver/llms/openai/__pycache__/functions.cpython-39.pyc` & `actionweaver-0.0.9/actionweaver/llms/openai/__pycache__/functions.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `actionweaver-0.0.8/actionweaver/llms/openai/__pycache__/tokens.cpython-39.pyc` & `actionweaver-0.0.9/actionweaver/llms/openai/__pycache__/tokens.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `actionweaver-0.0.8/actionweaver/llms/openai/chat.py` & `actionweaver-0.0.9/actionweaver/llms/openai/chat.py`

 * *Files 2% similar despite different names*

```diff
@@ -157,14 +157,15 @@
             API response with generated output.
         """
 
         # Todo: pass call_id to the decorated method
         call_id = str(uuid.uuid4())
 
         model = kwargs.get("model", self.model)
+        temperature = kwargs.get("temperature", 0.0)
 
         # Restart token usage tracker
         self.token_usage_tracker.clear()
 
         if scope is None:
             scope = DEFAULT_ACTION_SCOPE
         default_expr = _ActionHandlerLLMInvoke(scope)
@@ -217,21 +218,23 @@
                 }
             )
 
             function_argument = functions.to_arguments()
             if function_argument["functions"]:
                 api_response = openai.ChatCompletion.create(
                     model=model,
+                    temperature=temperature,
                     messages=messages,
                     stream=stream,
                     **function_argument,
                 )
             else:
                 api_response = openai.ChatCompletion.create(
                     model=model,
+                    temperature=temperature,
                     messages=messages,
                     stream=stream,
                 )
 
             # logic to handle streaming API response
             if is_generator(api_response):
                 first_element, iterator = get_first_element_and_iterator(api_response)
```

### Comparing `actionweaver-0.0.8/actionweaver/llms/openai/functions.py` & `actionweaver-0.0.9/actionweaver/llms/openai/functions.py`

 * *Files identical despite different names*

### Comparing `actionweaver-0.0.8/actionweaver/llms/openai/tokens.py` & `actionweaver-0.0.9/actionweaver/llms/openai/tokens.py`

 * *Files identical despite different names*

### Comparing `actionweaver-0.0.8/actionweaver/mixins/__pycache__/action_handler_mixin.cpython-39.pyc` & `actionweaver-0.0.9/actionweaver/mixins/__pycache__/action_handler_mixin.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `actionweaver-0.0.8/actionweaver/mixins/action_handler_mixin.py` & `actionweaver-0.0.9/actionweaver/mixins/action_handler_mixin.py`

 * *Files identical despite different names*

### Comparing `actionweaver-0.0.8/actionweaver/mixins/examples/__pycache__/folium.cpython-39.pyc` & `actionweaver-0.0.9/actionweaver/mixins/examples/__pycache__/folium.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `actionweaver-0.0.8/actionweaver/mixins/examples/__pycache__/langchain.cpython-39.pyc` & `actionweaver-0.0.9/actionweaver/mixins/examples/__pycache__/langchain.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `actionweaver-0.0.8/actionweaver/mixins/examples/__pycache__/openai.cpython-39.pyc` & `actionweaver-0.0.9/actionweaver/mixins/examples/__pycache__/openai.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `actionweaver-0.0.8/actionweaver/mixins/examples/folium.py` & `actionweaver-0.0.9/actionweaver/mixins/examples/folium.py`

 * *Files identical despite different names*

### Comparing `actionweaver-0.0.8/actionweaver/mixins/examples/langchain.py` & `actionweaver-0.0.9/actionweaver/mixins/examples/langchain.py`

 * *Files identical despite different names*

### Comparing `actionweaver-0.0.8/actionweaver/mixins/examples/openai.py` & `actionweaver-0.0.9/actionweaver/mixins/examples/openai.py`

 * *Files identical despite different names*

### Comparing `actionweaver-0.0.8/actionweaver/utils/__pycache__/cache.cpython-39.pyc` & `actionweaver-0.0.9/actionweaver/utils/__pycache__/cache.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `actionweaver-0.0.8/actionweaver/utils/__pycache__/output.cpython-39.pyc` & `actionweaver-0.0.9/actionweaver/utils/__pycache__/output.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `actionweaver-0.0.8/actionweaver/utils/__pycache__/pydantic_utils.cpython-39.pyc` & `actionweaver-0.0.9/actionweaver/utils/__pycache__/pydantic_utils.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `actionweaver-0.0.8/actionweaver/utils/__pycache__/stream.cpython-39.pyc` & `actionweaver-0.0.9/actionweaver/utils/__pycache__/stream.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `actionweaver-0.0.8/actionweaver/utils/cache.py` & `actionweaver-0.0.9/actionweaver/utils/cache.py`

 * *Files identical despite different names*

### Comparing `actionweaver-0.0.8/actionweaver/utils/pydantic_utils.py` & `actionweaver-0.0.9/actionweaver/utils/pydantic_utils.py`

 * *Files identical despite different names*

### Comparing `actionweaver-0.0.8/actionweaver/utils/stream.py` & `actionweaver-0.0.9/actionweaver/utils/stream.py`

 * *Files identical despite different names*

### Comparing `actionweaver-0.0.8/PKG-INFO` & `actionweaver-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: actionweaver
-Version: 0.0.8
+Version: 0.0.9
 Summary: An Application Framework for Building LLM Agents
 Author: Teng "Niel" Hu
 Author-email: hu.niel92@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

