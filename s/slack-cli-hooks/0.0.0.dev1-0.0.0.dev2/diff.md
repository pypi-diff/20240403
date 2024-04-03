# Comparing `tmp/slack_cli_hooks-0.0.0.dev1.tar.gz` & `tmp/slack_cli_hooks-0.0.0.dev2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "slack_cli_hooks-0.0.0.dev1.tar", last modified: Mon Jan 22 19:57:47 2024, max compression
+gzip compressed data, was "slack_cli_hooks-0.0.0.dev2.tar", last modified: Wed Jan 24 20:11:03 2024, max compression
```

## Comparing `slack_cli_hooks-0.0.0.dev1.tar` & `slack_cli_hooks-0.0.0.dev2.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 wbergamin   (502) staff       (20)        0 2024-01-22 19:57:47.283065 slack_cli_hooks-0.0.0.dev1/
--rw-r--r--   0 wbergamin   (502) staff       (20)     1081 2023-12-04 16:07:50.000000 slack_cli_hooks-0.0.0.dev1/LICENSE
--rw-r--r--   0 wbergamin   (502) staff       (20)       51 2023-12-04 16:10:47.000000 slack_cli_hooks-0.0.0.dev1/MANIFEST.in
--rw-r--r--   0 wbergamin   (502) staff       (20)     4144 2024-01-22 19:57:47.282711 slack_cli_hooks-0.0.0.dev1/PKG-INFO
--rw-r--r--   0 wbergamin   (502) staff       (20)     2894 2024-01-22 19:33:53.000000 slack_cli_hooks-0.0.0.dev1/README.md
--rw-r--r--   0 wbergamin   (502) staff       (20)     1690 2023-12-20 17:57:50.000000 slack_cli_hooks-0.0.0.dev1/pyproject.toml
--rw-r--r--   0 wbergamin   (502) staff       (20)       22 2023-12-04 16:07:50.000000 slack_cli_hooks-0.0.0.dev1/requirements.txt
--rw-r--r--   0 wbergamin   (502) staff       (20)       38 2024-01-22 19:57:47.283130 slack_cli_hooks-0.0.0.dev1/setup.cfg
-drwxr-xr-x   0 wbergamin   (502) staff       (20)        0 2024-01-22 19:57:47.271953 slack_cli_hooks-0.0.0.dev1/slack_cli_hooks/
--rw-r--r--   0 wbergamin   (502) staff       (20)      508 2023-12-13 15:31:21.000000 slack_cli_hooks-0.0.0.dev1/slack_cli_hooks/__init__.py
-drwxr-xr-x   0 wbergamin   (502) staff       (20)        0 2024-01-22 19:57:47.274976 slack_cli_hooks-0.0.0.dev1/slack_cli_hooks/error/
--rw-r--r--   0 wbergamin   (502) staff       (20)      157 2024-01-05 17:06:46.000000 slack_cli_hooks-0.0.0.dev1/slack_cli_hooks/error/__init__.py
-drwxr-xr-x   0 wbergamin   (502) staff       (20)        0 2024-01-22 19:57:47.278062 slack_cli_hooks-0.0.0.dev1/slack_cli_hooks/hooks/
--rw-r--r--   0 wbergamin   (502) staff       (20)       51 2023-12-13 15:31:21.000000 slack_cli_hooks-0.0.0.dev1/slack_cli_hooks/hooks/__init__.py
--rw-r--r--   0 wbergamin   (502) staff       (20)     3911 2024-01-05 17:06:46.000000 slack_cli_hooks-0.0.0.dev1/slack_cli_hooks/hooks/check_update.py
--rw-r--r--   0 wbergamin   (502) staff       (20)      787 2024-01-05 17:06:46.000000 slack_cli_hooks-0.0.0.dev1/slack_cli_hooks/hooks/get_hooks.py
--rw-r--r--   0 wbergamin   (502) staff       (20)     1273 2023-12-20 17:57:58.000000 slack_cli_hooks-0.0.0.dev1/slack_cli_hooks/hooks/get_manifest.py
--rw-r--r--   0 wbergamin   (502) staff       (20)     1824 2024-01-04 16:43:48.000000 slack_cli_hooks-0.0.0.dev1/slack_cli_hooks/hooks/start.py
-drwxr-xr-x   0 wbergamin   (502) staff       (20)        0 2024-01-22 19:57:47.278997 slack_cli_hooks-0.0.0.dev1/slack_cli_hooks/hooks/utils/
--rw-r--r--   0 wbergamin   (502) staff       (20)       89 2023-12-19 20:50:29.000000 slack_cli_hooks-0.0.0.dev1/slack_cli_hooks/hooks/utils/__init__.py
--rw-r--r--   0 wbergamin   (502) staff       (20)      684 2024-01-05 17:06:46.000000 slack_cli_hooks-0.0.0.dev1/slack_cli_hooks/hooks/utils/managed_os_env_vars.py
-drwxr-xr-x   0 wbergamin   (502) staff       (20)        0 2024-01-22 19:57:47.280691 slack_cli_hooks-0.0.0.dev1/slack_cli_hooks/protocol/
--rw-r--r--   0 wbergamin   (502) staff       (20)      712 2023-12-13 15:31:21.000000 slack_cli_hooks-0.0.0.dev1/slack_cli_hooks/protocol/__init__.py
--rw-r--r--   0 wbergamin   (502) staff       (20)      564 2023-12-13 15:31:21.000000 slack_cli_hooks-0.0.0.dev1/slack_cli_hooks/protocol/default_protocol.py
--rw-r--r--   0 wbergamin   (502) staff       (20)      655 2023-12-13 15:31:21.000000 slack_cli_hooks-0.0.0.dev1/slack_cli_hooks/protocol/message_boundary_protocol.py
--rw-r--r--   0 wbergamin   (502) staff       (20)     1395 2023-12-13 15:31:21.000000 slack_cli_hooks-0.0.0.dev1/slack_cli_hooks/protocol/protocol.py
--rw-r--r--   0 wbergamin   (502) staff       (20)        0 2023-12-13 15:31:21.000000 slack_cli_hooks-0.0.0.dev1/slack_cli_hooks/py.typed
--rw-r--r--   0 wbergamin   (502) staff       (20)      103 2024-01-05 17:13:04.000000 slack_cli_hooks-0.0.0.dev1/slack_cli_hooks/version.py
-drwxr-xr-x   0 wbergamin   (502) staff       (20)        0 2024-01-22 19:57:47.282141 slack_cli_hooks-0.0.0.dev1/slack_cli_hooks.egg-info/
--rw-r--r--   0 wbergamin   (502) staff       (20)     4144 2024-01-22 19:57:47.000000 slack_cli_hooks-0.0.0.dev1/slack_cli_hooks.egg-info/PKG-INFO
--rw-r--r--   0 wbergamin   (502) staff       (20)      809 2024-01-22 19:57:47.000000 slack_cli_hooks-0.0.0.dev1/slack_cli_hooks.egg-info/SOURCES.txt
--rw-r--r--   0 wbergamin   (502) staff       (20)        1 2024-01-22 19:57:47.000000 slack_cli_hooks-0.0.0.dev1/slack_cli_hooks.egg-info/dependency_links.txt
--rw-r--r--   0 wbergamin   (502) staff       (20)       22 2024-01-22 19:57:47.000000 slack_cli_hooks-0.0.0.dev1/slack_cli_hooks.egg-info/requires.txt
--rw-r--r--   0 wbergamin   (502) staff       (20)       16 2024-01-22 19:57:47.000000 slack_cli_hooks-0.0.0.dev1/slack_cli_hooks.egg-info/top_level.txt
+drwxr-xr-x   0 wbergamin   (502) staff       (20)        0 2024-01-24 20:11:03.959276 slack_cli_hooks-0.0.0.dev2/
+-rw-r--r--   0 wbergamin   (502) staff       (20)     1081 2023-12-04 16:07:50.000000 slack_cli_hooks-0.0.0.dev2/LICENSE
+-rw-r--r--   0 wbergamin   (502) staff       (20)       51 2023-12-04 16:10:47.000000 slack_cli_hooks-0.0.0.dev2/MANIFEST.in
+-rw-r--r--   0 wbergamin   (502) staff       (20)     4391 2024-01-24 20:11:03.958908 slack_cli_hooks-0.0.0.dev2/PKG-INFO
+-rw-r--r--   0 wbergamin   (502) staff       (20)     3292 2024-01-23 18:33:05.000000 slack_cli_hooks-0.0.0.dev2/README.md
+-rw-r--r--   0 wbergamin   (502) staff       (20)     1547 2024-01-24 20:00:46.000000 slack_cli_hooks-0.0.0.dev2/pyproject.toml
+-rw-r--r--   0 wbergamin   (502) staff       (20)       22 2023-12-04 16:07:50.000000 slack_cli_hooks-0.0.0.dev2/requirements.txt
+-rw-r--r--   0 wbergamin   (502) staff       (20)       38 2024-01-24 20:11:03.959355 slack_cli_hooks-0.0.0.dev2/setup.cfg
+drwxr-xr-x   0 wbergamin   (502) staff       (20)        0 2024-01-24 20:11:03.947576 slack_cli_hooks-0.0.0.dev2/slack_cli_hooks/
+-rw-r--r--   0 wbergamin   (502) staff       (20)      508 2023-12-13 15:31:21.000000 slack_cli_hooks-0.0.0.dev2/slack_cli_hooks/__init__.py
+drwxr-xr-x   0 wbergamin   (502) staff       (20)        0 2024-01-24 20:11:03.949409 slack_cli_hooks-0.0.0.dev2/slack_cli_hooks/error/
+-rw-r--r--   0 wbergamin   (502) staff       (20)      157 2024-01-05 17:06:46.000000 slack_cli_hooks-0.0.0.dev2/slack_cli_hooks/error/__init__.py
+drwxr-xr-x   0 wbergamin   (502) staff       (20)        0 2024-01-24 20:11:03.953720 slack_cli_hooks-0.0.0.dev2/slack_cli_hooks/hooks/
+-rw-r--r--   0 wbergamin   (502) staff       (20)       51 2023-12-13 15:31:21.000000 slack_cli_hooks-0.0.0.dev2/slack_cli_hooks/hooks/__init__.py
+-rw-r--r--   0 wbergamin   (502) staff       (20)     3458 2024-01-23 21:23:25.000000 slack_cli_hooks-0.0.0.dev2/slack_cli_hooks/hooks/check_update.py
+-rw-r--r--   0 wbergamin   (502) staff       (20)      787 2024-01-05 17:06:46.000000 slack_cli_hooks-0.0.0.dev2/slack_cli_hooks/hooks/get_hooks.py
+-rw-r--r--   0 wbergamin   (502) staff       (20)     1273 2023-12-20 17:57:58.000000 slack_cli_hooks-0.0.0.dev2/slack_cli_hooks/hooks/get_manifest.py
+-rw-r--r--   0 wbergamin   (502) staff       (20)     1824 2024-01-24 19:56:56.000000 slack_cli_hooks-0.0.0.dev2/slack_cli_hooks/hooks/start.py
+drwxr-xr-x   0 wbergamin   (502) staff       (20)        0 2024-01-24 20:11:03.954770 slack_cli_hooks-0.0.0.dev2/slack_cli_hooks/hooks/utils/
+-rw-r--r--   0 wbergamin   (502) staff       (20)       89 2023-12-19 20:50:29.000000 slack_cli_hooks-0.0.0.dev2/slack_cli_hooks/hooks/utils/__init__.py
+-rw-r--r--   0 wbergamin   (502) staff       (20)      684 2024-01-05 17:06:46.000000 slack_cli_hooks-0.0.0.dev2/slack_cli_hooks/hooks/utils/managed_os_env_vars.py
+drwxr-xr-x   0 wbergamin   (502) staff       (20)        0 2024-01-24 20:11:03.957748 slack_cli_hooks-0.0.0.dev2/slack_cli_hooks/protocol/
+-rw-r--r--   0 wbergamin   (502) staff       (20)      712 2023-12-13 15:31:21.000000 slack_cli_hooks-0.0.0.dev2/slack_cli_hooks/protocol/__init__.py
+-rw-r--r--   0 wbergamin   (502) staff       (20)      564 2023-12-13 15:31:21.000000 slack_cli_hooks-0.0.0.dev2/slack_cli_hooks/protocol/default_protocol.py
+-rw-r--r--   0 wbergamin   (502) staff       (20)      655 2023-12-13 15:31:21.000000 slack_cli_hooks-0.0.0.dev2/slack_cli_hooks/protocol/message_boundary_protocol.py
+-rw-r--r--   0 wbergamin   (502) staff       (20)     1395 2023-12-13 15:31:21.000000 slack_cli_hooks-0.0.0.dev2/slack_cli_hooks/protocol/protocol.py
+-rw-r--r--   0 wbergamin   (502) staff       (20)        0 2023-12-13 15:31:21.000000 slack_cli_hooks-0.0.0.dev2/slack_cli_hooks/py.typed
+-rw-r--r--   0 wbergamin   (502) staff       (20)      103 2024-01-24 20:01:31.000000 slack_cli_hooks-0.0.0.dev2/slack_cli_hooks/version.py
+drwxr-xr-x   0 wbergamin   (502) staff       (20)        0 2024-01-24 20:11:03.958418 slack_cli_hooks-0.0.0.dev2/slack_cli_hooks.egg-info/
+-rw-r--r--   0 wbergamin   (502) staff       (20)     4391 2024-01-24 20:11:03.000000 slack_cli_hooks-0.0.0.dev2/slack_cli_hooks.egg-info/PKG-INFO
+-rw-r--r--   0 wbergamin   (502) staff       (20)      809 2024-01-24 20:11:03.000000 slack_cli_hooks-0.0.0.dev2/slack_cli_hooks.egg-info/SOURCES.txt
+-rw-r--r--   0 wbergamin   (502) staff       (20)        1 2024-01-24 20:11:03.000000 slack_cli_hooks-0.0.0.dev2/slack_cli_hooks.egg-info/dependency_links.txt
+-rw-r--r--   0 wbergamin   (502) staff       (20)       22 2024-01-24 20:11:03.000000 slack_cli_hooks-0.0.0.dev2/slack_cli_hooks.egg-info/requires.txt
+-rw-r--r--   0 wbergamin   (502) staff       (20)       16 2024-01-24 20:11:03.000000 slack_cli_hooks-0.0.0.dev2/slack_cli_hooks.egg-info/top_level.txt
```

### Comparing `slack_cli_hooks-0.0.0.dev1/LICENSE` & `slack_cli_hooks-0.0.0.dev2/LICENSE`

 * *Files identical despite different names*

### Comparing `slack_cli_hooks-0.0.0.dev1/README.md` & `slack_cli_hooks-0.0.0.dev2/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,181 +1,206 @@
-00000000: 2320 5079 7468 6f6e 2053 6c61 636b 2048  # Python Slack H
-00000010: 6f6f 6b73 0a0a 5468 6973 206c 6962 7261  ooks..This libra
-00000020: 7279 2064 6566 696e 6573 2074 6865 2063  ry defines the c
-00000030: 6f6e 7472 6163 7420 6265 7477 6565 6e20  ontract between 
-00000040: 7468 650a 5b53 6c61 636b 2043 4c49 5d28  the.[Slack CLI](
-00000050: 6874 7470 733a 2f2f 6170 692e 736c 6163  https://api.slac
-00000060: 6b2e 636f 6d2f 6175 746f 6d61 7469 6f6e  k.com/automation
-00000070: 2f63 6c69 2f69 6e73 7461 6c6c 2920 616e  /cli/install) an
-00000080: 640a 5b42 6f6c 7420 666f 7220 5079 7468  d.[Bolt for Pyth
-00000090: 6f6e 5d28 6874 7470 733a 2f2f 736c 6163  on](https://slac
-000000a0: 6b2e 6465 762f 626f 6c74 2d70 7974 686f  k.dev/bolt-pytho
-000000b0: 6e2f 292e 0a0a 2323 204f 7665 7276 6965  n/)...## Overvie
-000000c0: 770a 5468 6973 206c 6962 7261 7279 2065  w.This library e
-000000d0: 6e61 626c 6573 2069 6e74 6572 2d70 726f  nables inter-pro
-000000e0: 6365 7373 2063 6f6d 6d75 6e69 6361 7469  cess communicati
-000000f0: 6f6e 2062 6574 7765 656e 2074 6865 205b  on between the [
-00000100: 536c 6163 6b20 434c 495d 2868 7474 7073  Slack CLI](https
-00000110: 3a2f 2f61 7069 2e73 6c61 636b 2e63 6f6d  ://api.slack.com
-00000120: 2f61 7574 6f6d 6174 696f 6e2f 636c 692f  /automation/cli/
-00000130: 696e 7374 616c 6c29 2061 6e64 2061 7070  install) and app
-00000140: 6c69 6361 7469 6f6e 7320 6275 696c 7420  lications built 
-00000150: 7769 7468 2042 6f6c 7420 666f 7220 5079  with Bolt for Py
-00000160: 7468 6f6e 2e20 0a0a 5768 656e 2075 7365  thon. ..When use
-00000170: 6420 746f 6765 7468 6572 2c20 7468 6520  d together, the 
-00000180: 434c 4920 6465 6c65 6761 7465 7320 7661  CLI delegates va
-00000190: 7269 6f75 7320 7461 736b 7320 746f 2074  rious tasks to t
-000001a0: 6865 2042 6f6c 7420 6170 706c 6963 6174  he Bolt applicat
-000001b0: 696f 6e20 6279 2069 6e76 6f6b 696e 6720  ion by invoking 
-000001c0: 7072 6f63 6573 7365 7320 2822 686f 6f6b  processes ("hook
-000001d0: 7322 2920 616e 6420 7468 656e 206d 616b  s") and then mak
-000001e0: 696e 6720 7573 6520 6f66 2074 6865 2072  ing use of the r
-000001f0: 6573 706f 6e73 6573 2070 726f 7669 6465  esponses provide
-00000200: 6420 6279 2065 6163 6820 686f 6f6b 2773  d by each hook's
-00000210: 2060 7374 646f 7574 602e 200a 0a46 6f72   `stdout`. ..For
-00000220: 2061 2063 6f6d 706c 6574 6520 6c69 7374   a complete list
-00000230: 206f 6620 6176 6169 6c61 626c 6520 686f   of available ho
-00000240: 6f6b 732c 2072 6561 6420 7468 6520 5b53  oks, read the [S
-00000250: 7570 706f 7274 6564 2048 6f6f 6b73 5d28  upported Hooks](
-00000260: 2373 7570 706f 7274 6564 2d68 6f6f 6b73  #supported-hooks
-00000270: 2920 7365 6374 696f 6e2e 0a0a 2323 2052  ) section...## R
-00000280: 6571 7569 7265 6d65 6e74 730a 5468 6520  equirements.The 
-00000290: 6c61 7465 7374 206d 696e 6f72 2076 6572  latest minor ver
-000002a0: 7369 6f6e 206f 6620 5b42 6f6c 7420 7631  sion of [Bolt v1
-000002b0: 5d28 6874 7470 733a 2f2f 7079 7069 2e6f  ](https://pypi.o
-000002c0: 7267 2f70 726f 6a65 6374 2f73 6c61 636b  rg/project/slack
-000002d0: 2d62 6f6c 742f 2920 6973 2072 6563 6f6d  -bolt/) is recom
-000002e0: 6d65 6e64 6564 2e0a 0a23 2320 5573 6167  mended...## Usag
-000002f0: 650a 4120 536c 6163 6b20 434c 492d 636f  e.A Slack CLI-co
-00000300: 6d70 6174 6962 6c65 2053 6c61 636b 2061  mpatible Slack a
-00000310: 7070 6c69 6361 7469 6f6e 2069 6e63 6c75  pplication inclu
-00000320: 6465 7320 6120 602e 2f73 6c61 636b 2e6a  des a `./slack.j
-00000330: 736f 6e60 2066 696c 6520 7468 6174 2063  son` file that c
-00000340: 6f6e 7461 696e 7320 686f 6f6b 7320 7370  ontains hooks sp
-00000350: 6563 6966 6963 2074 6f20 7468 6174 2070  ecific to that p
-00000360: 726f 6a65 6374 2e20 4561 6368 2068 6f6f  roject. Each hoo
-00000370: 6b20 6973 2061 7373 6f63 6961 7465 6420  k is associated 
-00000380: 7769 7468 2063 6f6d 6d61 6e64 7320 7468  with commands th
-00000390: 6174 2061 7265 2061 7661 696c 6162 6c65  at are available
-000003a0: 2069 6e20 7468 6520 536c 6163 6b20 434c   in the Slack CL
-000003b0: 492e 2042 7920 6465 6661 756c 742c 2060  I. By default, `
-000003c0: 6765 742d 686f 6f6b 7360 2072 6574 7269  get-hooks` retri
-000003d0: 6576 6573 2061 6c6c 206f 6620 7468 6520  eves all of the 
-000003e0: 5b73 7570 706f 7274 6564 2068 6f6f 6b73  [supported hooks
-000003f0: 5d28 2373 7570 706f 7274 6564 2d68 6f6f  ](#supported-hoo
-00000400: 6b73 2920 616e 6420 7468 6569 7220 636f  ks) and their co
-00000410: 7272 6573 706f 6e64 696e 6720 7363 7269  rresponding scri
-00000420: 7074 7320 6173 2064 6566 696e 6564 2069  pts as defined i
-00000430: 6e20 7468 6973 206c 6962 7261 7279 2e0a  n this library..
-00000440: 0a54 6865 2043 4c49 2077 696c 6c20 616c  .The CLI will al
-00000450: 7761 7973 2075 7365 2074 6865 2076 6572  ways use the ver
-00000460: 7369 6f6e 206f 6620 7468 6520 6070 7974  sion of the `pyt
-00000470: 686f 6e2d 736c 6163 6b2d 686f 6f6b 7360  hon-slack-hooks`
-00000480: 2074 6861 7420 6973 2073 7065 6369 6669   that is specifi
-00000490: 6564 2069 6e20 7468 6520 7072 6f6a 6563  ed in the projec
-000004a0: 7427 7320 6072 6571 7569 7265 6d65 6e74  t's `requirement
-000004b0: 732e 7478 7460 2e0a 0a23 2323 2053 7570  s.txt`...### Sup
-000004c0: 706f 7274 6564 2048 6f6f 6b73 0a0a 5468  ported Hooks..Th
-000004d0: 6520 686f 6f6b 7320 6375 7272 656e 746c  e hooks currentl
-000004e0: 7920 7375 7070 6f72 7465 6420 666f 7220  y supported for 
-000004f0: 7573 6520 7769 7468 696e 2074 6865 2053  use within the S
-00000500: 6c61 636b 2043 4c49 2069 6e63 6c75 6465  lack CLI include
-00000510: 2060 6368 6563 6b2d 7570 6461 7465 602c   `check-update`,
-00000520: 2060 6765 742d 686f 6f6b 7360 2c20 6067   `get-hooks`, `g
-00000530: 6574 2d6d 616e 6966 6573 7460 2c20 616e  et-manifest`, an
-00000540: 6420 6073 7461 7274 603a 0a0a 7c20 486f  d `start`:..| Ho
-00000550: 6f6b 204e 616d 6520 207c 2043 4c49 2043  ok Name  | CLI C
-00000560: 6f6d 6d61 6e64 2020 7c20 4669 6c65 2020  ommand  | File  
-00000570: 7c20 2044 6573 6372 6970 7469 6f6e 2020  |  Description  
-00000580: 7c0a 7c20 2d2d 2d20 7c20 2d2d 2d20 7c20  |.| --- | --- | 
-00000590: 2d2d 2d20 7c20 2d2d 2d20 7c0a 7c20 6063  --- | --- |.| `c
-000005a0: 6865 636b 2d75 7064 6174 6560 207c 2060  heck-update` | `
-000005b0: 736c 6163 6b20 7570 6461 7465 6020 7c20  slack update` | 
-000005c0: 5b63 6865 636b 5f75 7064 6174 652e 7079  [check_update.py
-000005d0: 5d28 2e2f 736c 6163 6b5f 636c 695f 686f  ](./slack_cli_ho
-000005e0: 6f6b 732f 686f 6f6b 732f 6368 6563 6b5f  oks/hooks/check_
-000005f0: 7570 6461 7465 2e70 7929 207c 2043 6865  update.py) | Che
-00000600: 636b 7320 7468 6520 7072 6f6a 6563 7427  cks the project'
-00000610: 7320 536c 6163 6b20 6465 7065 6e64 656e  s Slack dependen
-00000620: 6369 6573 2074 6f20 6465 7465 726d 696e  cies to determin
-00000630: 6520 7768 6574 6865 7220 6f72 206e 6f74  e whether or not
-00000640: 2061 6e79 206c 6962 7261 7269 6573 206e   any libraries n
-00000650: 6565 6420 746f 2062 6520 7570 6461 7465  eed to be update
-00000660: 642e 207c 0a7c 2060 6765 742d 686f 6f6b  d. |.| `get-hook
-00000670: 7360 207c 2041 6c6c 207c 205b 6765 745f  s` | All | [get_
-00000680: 686f 6f6b 732e 7079 5d28 2e2f 736c 6163  hooks.py](./slac
-00000690: 6b5f 636c 695f 686f 6f6b 732f 686f 6f6b  k_cli_hooks/hook
-000006a0: 732f 6765 745f 686f 6f6b 732e 7079 2920  s/get_hooks.py) 
-000006b0: 7c20 4665 7463 6865 7320 7468 6520 6c69  | Fetches the li
-000006c0: 7374 206f 6620 6176 6169 6c61 626c 6520  st of available 
-000006d0: 686f 6f6b 7320 666f 7220 7468 6520 434c  hooks for the CL
-000006e0: 4920 6672 6f6d 2074 6869 7320 7265 706f  I from this repo
-000006f0: 7369 746f 7279 2e20 7c0a 7c20 6067 6574  sitory. |.| `get
-00000700: 2d6d 616e 6966 6573 7460 207c 2060 736c  -manifest` | `sl
-00000710: 6163 6b20 6d61 6e69 6665 7374 6020 7c20  ack manifest` | 
-00000720: 5b67 6574 5f6d 616e 6966 6573 742e 7079  [get_manifest.py
-00000730: 5d28 2e2f 736c 6163 6b5f 636c 695f 686f  ](./slack_cli_ho
-00000740: 6f6b 732f 686f 6f6b 732f 6765 745f 6d61  oks/hooks/get_ma
-00000750: 6e69 6665 7374 2e70 7929 207c 2043 6f6e  nifest.py) | Con
-00000760: 7665 7274 7320 6120 606d 616e 6966 6573  verts a `manifes
-00000770: 742e 6a73 6f6e 6020 6669 6c65 2069 6e74  t.json` file int
-00000780: 6f20 6120 7661 6c69 6420 6d61 6e69 6665  o a valid manife
-00000790: 7374 204a 534f 4e20 7061 796c 6f61 642e  st JSON payload.
-000007a0: 207c 0a7c 2060 7374 6172 7460 207c 2060   |.| `start` | `
-000007b0: 736c 6163 6b20 7275 6e60 207c 205b 7374  slack run` | [st
-000007c0: 6172 742e 7079 5d28 2e2f 736c 6163 6b5f  art.py](./slack_
-000007d0: 636c 695f 686f 6f6b 732f 686f 6f6b 732f  cli_hooks/hooks/
-000007e0: 7374 6172 742e 7079 2920 7c20 5768 696c  start.py) | Whil
-000007f0: 6520 6465 7665 6c6f 7069 6e67 206c 6f63  e developing loc
-00000800: 616c 6c79 2c20 7468 6520 434c 4920 6d61  ally, the CLI ma
-00000810: 6e61 6765 7320 6120 736f 636b 6574 2063  nages a socket c
-00000820: 6f6e 6e65 6374 696f 6e20 7769 7468 2053  onnection with S
-00000830: 6c61 636b 2773 2062 6163 6b65 6e64 2061  lack's backend a
-00000840: 6e64 2075 7469 6c69 7a65 7320 7468 6973  nd utilizes this
-00000850: 2068 6f6f 6b20 666f 7220 6576 656e 7473   hook for events
-00000860: 2072 6563 6569 7665 6420 7669 6120 7468   received via th
-00000870: 6973 2063 6f6e 6e65 6374 696f 6e2e 207c  is connection. |
-00000880: 0a0a 0a23 2323 204f 7665 7272 6964 696e  ...### Overridin
-00000890: 6720 486f 6f6b 730a 546f 2063 7573 746f  g Hooks.To custo
-000008a0: 6d69 7a65 2074 6865 2062 6568 6176 696f  mize the behavio
-000008b0: 7220 6f66 2061 2068 6f6f 6b2c 2061 6464  r of a hook, add
-000008c0: 2074 6865 2068 6f6f 6b20 746f 2079 6f75   the hook to you
-000008d0: 7220 6170 706c 6963 6174 696f 6e27 7320  r application's 
-000008e0: 602f 736c 6163 6b2e 6a73 6f6e 6020 6669  `/slack.json` fi
-000008f0: 6c65 2c20 616e 6420 7072 6f76 6964 6520  le, and provide 
-00000900: 6120 636f 7272 6573 706f 6e64 696e 6720  a corresponding 
-00000910: 7363 7269 7074 2074 6f20 6265 2065 7865  script to be exe
-00000920: 6375 7465 642e 200a 0a57 6865 6e20 636f  cuted. ..When co
-00000930: 6d6d 616e 6473 2061 7265 2072 756e 2c20  mmands are run, 
-00000940: 7468 6520 536c 6163 6b20 434c 4920 7769  the Slack CLI wi
-00000950: 6c6c 206c 6f6f 6b20 746f 2074 6865 2070  ll look to the p
-00000960: 726f 6a65 6374 2773 2068 6f6f 6b20 6465  roject's hook de
-00000970: 6669 6e69 7469 6f6e 7320 616e 6420 7573  finitions and us
-00000980: 6520 7468 6f73 6520 696e 7374 6561 6420  e those instead 
-00000990: 6f66 2077 6861 7427 7320 6465 6669 6e65  of what's define
-000009a0: 6420 696e 2074 6869 7320 6c69 6272 6172  d in this librar
-000009b0: 792c 2069 6620 7072 6f76 6964 6564 2e0a  y, if provided..
-000009c0: 0a42 656c 6f77 2069 7320 616e 2065 7861  .Below is an exa
-000009d0: 6d70 6c65 2060 2f73 6c61 636b 2e6a 736f  mple `/slack.jso
-000009e0: 6e60 2066 696c 6520 7468 6174 206f 7665  n` file that ove
-000009f0: 7272 6964 6573 2074 6865 2064 6566 6175  rrides the defau
-00000a00: 6c74 2060 7374 6172 7460 3a0a 0a60 6060  lt `start`:..```
-00000a10: 0a7b 0a20 2022 686f 6f6b 7322 3a20 7b0a  .{.  "hooks": {.
-00000a20: 2020 2020 2267 6574 2d68 6f6f 6b73 223a      "get-hooks":
-00000a30: 2022 7079 7468 6f6e 3320 2d6d 2073 6c61   "python3 -m sla
-00000a40: 636b 5f63 6c69 5f68 6f6f 6b73 2e68 6f6f  ck_cli_hooks.hoo
-00000a50: 6b73 2e67 6574 5f68 6f6f 6b73 222c 0a20  ks.get_hooks",. 
-00000a60: 2020 2022 7374 6172 7422 3a20 2270 7974     "start": "pyt
-00000a70: 686f 6e33 2061 7070 2e70 7922 0a20 207d  hon3 app.py".  }
-00000a80: 0a7d 0a60 6060 0a0a 2323 2043 6f6e 7472  .}.```..## Contr
-00000a90: 6962 7574 696e 670a 0a43 6f6e 7472 6962  ibuting..Contrib
-00000aa0: 7574 696f 6e73 2061 7265 2061 6c77 6179  utions are alway
-00000ab0: 7320 7765 6c63 6f6d 6521 2050 6c65 6173  s welcome! Pleas
-00000ac0: 6520 7265 7669 6577 2074 6865 0a5b 636f  e review the.[co
-00000ad0: 6e74 7269 6275 7469 6e67 2067 7569 6465  ntributing guide
-00000ae0: 6c69 6e65 735d 2868 7474 7073 3a2f 2f67  lines](https://g
-00000af0: 6974 6875 622e 636f 6d2f 736c 6163 6b61  ithub.com/slacka
-00000b00: 7069 2f70 7974 686f 6e2d 736c 6163 6b2d  pi/python-slack-
-00000b10: 686f 6f6b 732f 626c 6f62 2f6d 6169 6e2f  hooks/blob/main/
-00000b20: 2e67 6974 6875 622f 434f 4e54 5249 4255  .github/CONTRIBU
-00000b30: 5449 4e47 2e6d 6429 0a66 6f72 206d 6f72  TING.md).for mor
-00000b40: 6520 696e 666f 726d 6174 696f 6e2e       e information.
+00000000: 3c68 3120 616c 6967 6e3d 2263 656e 7465  <h1 align="cente
+00000010: 7222 3e50 7974 686f 6e20 536c 6163 6b20  r">Python Slack 
+00000020: 486f 6f6b 733c 2f68 313e 0a0a 3c70 2061  Hooks</h1>..<p a
+00000030: 6c69 676e 3d22 6365 6e74 6572 223e 0a20  lign="center">. 
+00000040: 2020 203c 6120 6872 6566 3d22 6874 7470     <a href="http
+00000050: 733a 2f2f 7079 7069 2e6f 7267 2f70 726f  s://pypi.org/pro
+00000060: 6a65 6374 2f73 6c61 636b 2d63 6c69 2d68  ject/slack-cli-h
+00000070: 6f6f 6b73 2f22 3e0a 2020 2020 2020 2020  ooks/">.        
+00000080: 3c69 6d67 2061 6c74 3d22 5079 5049 202d  <img alt="PyPI -
+00000090: 2056 6572 7369 6f6e 2220 7372 633d 2268   Version" src="h
+000000a0: 7474 7073 3a2f 2f69 6d67 2e73 6869 656c  ttps://img.shiel
+000000b0: 6473 2e69 6f2f 7079 7069 2f76 2f73 6c61  ds.io/pypi/v/sla
+000000c0: 636b 2d63 6c69 2d68 6f6f 6b73 3f73 7479  ck-cli-hooks?sty
+000000d0: 6c65 3d66 6c61 742d 7371 7561 7265 223e  le=flat-square">
+000000e0: 3c2f 613e 0a20 2020 203c 6120 6872 6566  </a>.    <a href
+000000f0: 3d22 6874 7470 733a 2f2f 7079 7069 2e6f  ="https://pypi.o
+00000100: 7267 2f70 726f 6a65 6374 2f73 6c61 636b  rg/project/slack
+00000110: 2d63 6c69 2d68 6f6f 6b73 2f22 3e0a 2020  -cli-hooks/">.  
+00000120: 2020 2020 2020 3c69 6d67 2061 6c74 3d22        <img alt="
+00000130: 5079 7468 6f6e 2056 6572 7369 6f6e 7322  Python Versions"
+00000140: 2073 7263 3d22 6874 7470 733a 2f2f 696d   src="https://im
+00000150: 672e 7368 6965 6c64 732e 696f 2f70 7970  g.shields.io/pyp
+00000160: 692f 7079 7665 7273 696f 6e73 2f73 6c61  i/pyversions/sla
+00000170: 636b 2d63 6c69 2d68 6f6f 6b73 2e73 7667  ck-cli-hooks.svg
+00000180: 3f73 7479 6c65 3d66 6c61 742d 7371 7561  ?style=flat-squa
+00000190: 7265 223e 3c2f 613e 0a3c 2f70 3e0a 0a54  re"></a>.</p>..T
+000001a0: 6869 7320 6c69 6272 6172 7920 6465 6669  his library defi
+000001b0: 6e65 7320 7468 6520 636f 6e74 7261 6374  nes the contract
+000001c0: 2062 6574 7765 656e 2074 6865 0a5b 536c   between the.[Sl
+000001d0: 6163 6b20 434c 495d 2868 7474 7073 3a2f  ack CLI](https:/
+000001e0: 2f61 7069 2e73 6c61 636b 2e63 6f6d 2f61  /api.slack.com/a
+000001f0: 7574 6f6d 6174 696f 6e2f 636c 692f 696e  utomation/cli/in
+00000200: 7374 616c 6c29 2061 6e64 0a5b 426f 6c74  stall) and.[Bolt
+00000210: 2066 6f72 2050 7974 686f 6e5d 2868 7474   for Python](htt
+00000220: 7073 3a2f 2f73 6c61 636b 2e64 6576 2f62  ps://slack.dev/b
+00000230: 6f6c 742d 7079 7468 6f6e 2f29 2e0a 0a23  olt-python/)...#
+00000240: 2320 4f76 6572 7669 6577 0a0a 5468 6973  # Overview..This
+00000250: 206c 6962 7261 7279 2065 6e61 626c 6573   library enables
+00000260: 2069 6e74 6572 2d70 726f 6365 7373 2063   inter-process c
+00000270: 6f6d 6d75 6e69 6361 7469 6f6e 2062 6574  ommunication bet
+00000280: 7765 656e 2074 6865 205b 536c 6163 6b20  ween the [Slack 
+00000290: 434c 495d 2868 7474 7073 3a2f 2f61 7069  CLI](https://api
+000002a0: 2e73 6c61 636b 2e63 6f6d 2f61 7574 6f6d  .slack.com/autom
+000002b0: 6174 696f 6e2f 636c 692f 696e 7374 616c  ation/cli/instal
+000002c0: 6c29 2061 6e64 2061 7070 6c69 6361 7469  l) and applicati
+000002d0: 6f6e 7320 6275 696c 7420 7769 7468 2042  ons built with B
+000002e0: 6f6c 7420 666f 7220 5079 7468 6f6e 2e0a  olt for Python..
+000002f0: 0a57 6865 6e20 7573 6564 2074 6f67 6574  .When used toget
+00000300: 6865 722c 2074 6865 2043 4c49 2064 656c  her, the CLI del
+00000310: 6567 6174 6573 2076 6172 696f 7573 2074  egates various t
+00000320: 6173 6b73 2074 6f20 7468 6520 426f 6c74  asks to the Bolt
+00000330: 2061 7070 6c69 6361 7469 6f6e 2062 7920   application by 
+00000340: 696e 766f 6b69 6e67 2070 726f 6365 7373  invoking process
+00000350: 6573 2028 2268 6f6f 6b73 2229 2061 6e64  es ("hooks") and
+00000360: 2074 6865 6e20 6d61 6b69 6e67 2075 7365   then making use
+00000370: 206f 6620 7468 6520 7265 7370 6f6e 7365   of the response
+00000380: 7320 7072 6f76 6964 6564 2062 7920 6561  s provided by ea
+00000390: 6368 2068 6f6f 6b27 7320 6073 7464 6f75  ch hook's `stdou
+000003a0: 7460 2e0a 0a46 6f72 2061 2063 6f6d 706c  t`...For a compl
+000003b0: 6574 6520 6c69 7374 206f 6620 6176 6169  ete list of avai
+000003c0: 6c61 626c 6520 686f 6f6b 732c 2072 6561  lable hooks, rea
+000003d0: 6420 7468 6520 5b53 7570 706f 7274 6564  d the [Supported
+000003e0: 2048 6f6f 6b73 5d28 2373 7570 706f 7274   Hooks](#support
+000003f0: 6564 2d68 6f6f 6b73 2920 7365 6374 696f  ed-hooks) sectio
+00000400: 6e2e 0a0a 2323 2052 6571 7569 7265 6d65  n...## Requireme
+00000410: 6e74 730a 0a54 6865 206c 6174 6573 7420  nts..The latest 
+00000420: 6d69 6e6f 7220 7665 7273 696f 6e20 6f66  minor version of
+00000430: 205b 426f 6c74 2076 315d 2868 7474 7073   [Bolt v1](https
+00000440: 3a2f 2f70 7970 692e 6f72 672f 7072 6f6a  ://pypi.org/proj
+00000450: 6563 742f 736c 6163 6b2d 626f 6c74 2f29  ect/slack-bolt/)
+00000460: 2069 7320 7265 636f 6d6d 656e 6465 642e   is recommended.
+00000470: 0a0a 2323 2055 7361 6765 0a0a 4120 536c  ..## Usage..A Sl
+00000480: 6163 6b20 434c 492d 636f 6d70 6174 6962  ack CLI-compatib
+00000490: 6c65 2053 6c61 636b 2061 7070 6c69 6361  le Slack applica
+000004a0: 7469 6f6e 2069 6e63 6c75 6465 7320 6120  tion includes a 
+000004b0: 602e 2f73 6c61 636b 2e6a 736f 6e60 2066  `./slack.json` f
+000004c0: 696c 6520 7468 6174 2063 6f6e 7461 696e  ile that contain
+000004d0: 7320 686f 6f6b 7320 7370 6563 6966 6963  s hooks specific
+000004e0: 2074 6f20 7468 6174 2070 726f 6a65 6374   to that project
+000004f0: 2e20 4561 6368 2068 6f6f 6b20 6973 2061  . Each hook is a
+00000500: 7373 6f63 6961 7465 6420 7769 7468 2063  ssociated with c
+00000510: 6f6d 6d61 6e64 7320 7468 6174 2061 7265  ommands that are
+00000520: 2061 7661 696c 6162 6c65 2069 6e20 7468   available in th
+00000530: 6520 536c 6163 6b20 434c 492e 2042 7920  e Slack CLI. By 
+00000540: 6465 6661 756c 742c 2060 6765 742d 686f  default, `get-ho
+00000550: 6f6b 7360 2072 6574 7269 6576 6573 2061  oks` retrieves a
+00000560: 6c6c 206f 6620 7468 6520 5b73 7570 706f  ll of the [suppo
+00000570: 7274 6564 2068 6f6f 6b73 5d28 2373 7570  rted hooks](#sup
+00000580: 706f 7274 6564 2d68 6f6f 6b73 2920 616e  ported-hooks) an
+00000590: 6420 7468 6569 7220 636f 7272 6573 706f  d their correspo
+000005a0: 6e64 696e 6720 7363 7269 7074 7320 6173  nding scripts as
+000005b0: 2064 6566 696e 6564 2069 6e20 7468 6973   defined in this
+000005c0: 206c 6962 7261 7279 2e0a 0a54 6865 2043   library...The C
+000005d0: 4c49 2077 696c 6c20 616c 7761 7973 2075  LI will always u
+000005e0: 7365 2074 6865 2076 6572 7369 6f6e 206f  se the version o
+000005f0: 6620 7468 6520 6070 7974 686f 6e2d 736c  f the `python-sl
+00000600: 6163 6b2d 686f 6f6b 7360 2074 6861 7420  ack-hooks` that 
+00000610: 6973 2073 7065 6369 6669 6564 2069 6e20  is specified in 
+00000620: 7468 6520 7072 6f6a 6563 7427 7320 6072  the project's `r
+00000630: 6571 7569 7265 6d65 6e74 732e 7478 7460  equirements.txt`
+00000640: 2e0a 0a23 2323 2053 7570 706f 7274 6564  ...### Supported
+00000650: 2048 6f6f 6b73 0a0a 5468 6520 686f 6f6b   Hooks..The hook
+00000660: 7320 6375 7272 656e 746c 7920 7375 7070  s currently supp
+00000670: 6f72 7465 6420 666f 7220 7573 6520 7769  orted for use wi
+00000680: 7468 696e 2074 6865 2053 6c61 636b 2043  thin the Slack C
+00000690: 4c49 2069 6e63 6c75 6465 2060 6368 6563  LI include `chec
+000006a0: 6b2d 7570 6461 7465 602c 2060 6765 742d  k-update`, `get-
+000006b0: 686f 6f6b 7360 2c20 6067 6574 2d6d 616e  hooks`, `get-man
+000006c0: 6966 6573 7460 2c20 616e 6420 6073 7461  ifest`, and `sta
+000006d0: 7274 603a 0a0a 7c20 486f 6f6b 204e 616d  rt`:..| Hook Nam
+000006e0: 6520 207c 2043 4c49 2043 6f6d 6d61 6e64  e  | CLI Command
+000006f0: 2020 7c20 4669 6c65 2020 7c20 2044 6573    | File  |  Des
+00000700: 6372 6970 7469 6f6e 2020 7c0a 7c20 2d2d  cription  |.| --
+00000710: 2d20 7c20 2d2d 2d20 7c20 2d2d 2d20 7c20  - | --- | --- | 
+00000720: 2d2d 2d20 7c0a 7c20 6063 6865 636b 2d75  --- |.| `check-u
+00000730: 7064 6174 6560 207c 2060 736c 6163 6b20  pdate` | `slack 
+00000740: 7570 6461 7465 6020 7c20 5b63 6865 636b  update` | [check
+00000750: 5f75 7064 6174 652e 7079 5d28 2e2f 736c  _update.py](./sl
+00000760: 6163 6b5f 636c 695f 686f 6f6b 732f 686f  ack_cli_hooks/ho
+00000770: 6f6b 732f 6368 6563 6b5f 7570 6461 7465  oks/check_update
+00000780: 2e70 7929 207c 2043 6865 636b 7320 7468  .py) | Checks th
+00000790: 6520 7072 6f6a 6563 7427 7320 536c 6163  e project's Slac
+000007a0: 6b20 6465 7065 6e64 656e 6369 6573 2074  k dependencies t
+000007b0: 6f20 6465 7465 726d 696e 6520 7768 6574  o determine whet
+000007c0: 6865 7220 6f72 206e 6f74 2061 6e79 206c  her or not any l
+000007d0: 6962 7261 7269 6573 206e 6565 6420 746f  ibraries need to
+000007e0: 2062 6520 7570 6461 7465 642e 207c 0a7c   be updated. |.|
+000007f0: 2060 6765 742d 686f 6f6b 7360 207c 2041   `get-hooks` | A
+00000800: 6c6c 207c 205b 6765 745f 686f 6f6b 732e  ll | [get_hooks.
+00000810: 7079 5d28 2e2f 736c 6163 6b5f 636c 695f  py](./slack_cli_
+00000820: 686f 6f6b 732f 686f 6f6b 732f 6765 745f  hooks/hooks/get_
+00000830: 686f 6f6b 732e 7079 2920 7c20 4665 7463  hooks.py) | Fetc
+00000840: 6865 7320 7468 6520 6c69 7374 206f 6620  hes the list of 
+00000850: 6176 6169 6c61 626c 6520 686f 6f6b 7320  available hooks 
+00000860: 666f 7220 7468 6520 434c 4920 6672 6f6d  for the CLI from
+00000870: 2074 6869 7320 7265 706f 7369 746f 7279   this repository
+00000880: 2e20 7c0a 7c20 6067 6574 2d6d 616e 6966  . |.| `get-manif
+00000890: 6573 7460 207c 2060 736c 6163 6b20 6d61  est` | `slack ma
+000008a0: 6e69 6665 7374 6020 7c20 5b67 6574 5f6d  nifest` | [get_m
+000008b0: 616e 6966 6573 742e 7079 5d28 2e2f 736c  anifest.py](./sl
+000008c0: 6163 6b5f 636c 695f 686f 6f6b 732f 686f  ack_cli_hooks/ho
+000008d0: 6f6b 732f 6765 745f 6d61 6e69 6665 7374  oks/get_manifest
+000008e0: 2e70 7929 207c 2043 6f6e 7665 7274 7320  .py) | Converts 
+000008f0: 6120 606d 616e 6966 6573 742e 6a73 6f6e  a `manifest.json
+00000900: 6020 6669 6c65 2069 6e74 6f20 6120 7661  ` file into a va
+00000910: 6c69 6420 6d61 6e69 6665 7374 204a 534f  lid manifest JSO
+00000920: 4e20 7061 796c 6f61 642e 207c 0a7c 2060  N payload. |.| `
+00000930: 7374 6172 7460 207c 2060 736c 6163 6b20  start` | `slack 
+00000940: 7275 6e60 207c 205b 7374 6172 742e 7079  run` | [start.py
+00000950: 5d28 2e2f 736c 6163 6b5f 636c 695f 686f  ](./slack_cli_ho
+00000960: 6f6b 732f 686f 6f6b 732f 7374 6172 742e  oks/hooks/start.
+00000970: 7079 2920 7c20 5768 696c 6520 6465 7665  py) | While deve
+00000980: 6c6f 7069 6e67 206c 6f63 616c 6c79 2c20  loping locally, 
+00000990: 7468 6520 434c 4920 6d61 6e61 6765 7320  the CLI manages 
+000009a0: 6120 736f 636b 6574 2063 6f6e 6e65 6374  a socket connect
+000009b0: 696f 6e20 7769 7468 2053 6c61 636b 2773  ion with Slack's
+000009c0: 2062 6163 6b65 6e64 2061 6e64 2075 7469   backend and uti
+000009d0: 6c69 7a65 7320 7468 6973 2068 6f6f 6b20  lizes this hook 
+000009e0: 666f 7220 6576 656e 7473 2072 6563 6569  for events recei
+000009f0: 7665 6420 7669 6120 7468 6973 2063 6f6e  ved via this con
+00000a00: 6e65 6374 696f 6e2e 207c 0a0a 2323 2320  nection. |..### 
+00000a10: 4f76 6572 7269 6469 6e67 2048 6f6f 6b73  Overriding Hooks
+00000a20: 0a0a 546f 2063 7573 746f 6d69 7a65 2074  ..To customize t
+00000a30: 6865 2062 6568 6176 696f 7220 6f66 2061  he behavior of a
+00000a40: 2068 6f6f 6b2c 2061 6464 2074 6865 2068   hook, add the h
+00000a50: 6f6f 6b20 746f 2079 6f75 7220 6170 706c  ook to your appl
+00000a60: 6963 6174 696f 6e27 7320 602f 736c 6163  ication's `/slac
+00000a70: 6b2e 6a73 6f6e 6020 6669 6c65 2c20 616e  k.json` file, an
+00000a80: 6420 7072 6f76 6964 6520 6120 636f 7272  d provide a corr
+00000a90: 6573 706f 6e64 696e 6720 7363 7269 7074  esponding script
+00000aa0: 2074 6f20 6265 2065 7865 6375 7465 642e   to be executed.
+00000ab0: 0a0a 5768 656e 2063 6f6d 6d61 6e64 7320  ..When commands 
+00000ac0: 6172 6520 7275 6e2c 2074 6865 2053 6c61  are run, the Sla
+00000ad0: 636b 2043 4c49 2077 696c 6c20 6c6f 6f6b  ck CLI will look
+00000ae0: 2074 6f20 7468 6520 7072 6f6a 6563 7427   to the project'
+00000af0: 7320 686f 6f6b 2064 6566 696e 6974 696f  s hook definitio
+00000b00: 6e73 2061 6e64 2075 7365 2074 686f 7365  ns and use those
+00000b10: 2069 6e73 7465 6164 206f 6620 7768 6174   instead of what
+00000b20: 2773 2064 6566 696e 6564 2069 6e20 7468  's defined in th
+00000b30: 6973 206c 6962 7261 7279 2c20 6966 2070  is library, if p
+00000b40: 726f 7669 6465 642e 0a0a 4265 6c6f 7720  rovided...Below 
+00000b50: 6973 2061 6e20 6578 616d 706c 6520 602f  is an example `/
+00000b60: 736c 6163 6b2e 6a73 6f6e 6020 6669 6c65  slack.json` file
+00000b70: 2074 6861 7420 6f76 6572 7269 6465 7320   that overrides 
+00000b80: 7468 6520 6465 6661 756c 7420 6073 7461  the default `sta
+00000b90: 7274 603a 0a0a 6060 606a 736f 6e0a 7b0a  rt`:..```json.{.
+00000ba0: 2020 2268 6f6f 6b73 223a 207b 0a20 2020    "hooks": {.   
+00000bb0: 2022 6765 742d 686f 6f6b 7322 3a20 2270   "get-hooks": "p
+00000bc0: 7974 686f 6e33 202d 6d20 736c 6163 6b5f  ython3 -m slack_
+00000bd0: 636c 695f 686f 6f6b 732e 686f 6f6b 732e  cli_hooks.hooks.
+00000be0: 6765 745f 686f 6f6b 7322 2c0a 2020 2020  get_hooks",.    
+00000bf0: 2273 7461 7274 223a 2022 7079 7468 6f6e  "start": "python
+00000c00: 3320 6170 702e 7079 220a 2020 7d0a 7d0a  3 app.py".  }.}.
+00000c10: 6060 600a 0a23 2320 436f 6e74 7269 6275  ```..## Contribu
+00000c20: 7469 6e67 0a0a 436f 6e74 7269 6275 7469  ting..Contributi
+00000c30: 6f6e 7320 6172 6520 616c 7761 7973 2077  ons are always w
+00000c40: 656c 636f 6d65 2120 506c 6561 7365 2072  elcome! Please r
+00000c50: 6576 6965 7720 7468 650a 5b63 6f6e 7472  eview the.[contr
+00000c60: 6962 7574 696e 6720 6775 6964 656c 696e  ibuting guidelin
+00000c70: 6573 5d28 6874 7470 733a 2f2f 6769 7468  es](https://gith
+00000c80: 7562 2e63 6f6d 2f73 6c61 636b 6170 692f  ub.com/slackapi/
+00000c90: 7079 7468 6f6e 2d73 6c61 636b 2d68 6f6f  python-slack-hoo
+00000ca0: 6b73 2f62 6c6f 622f 6d61 696e 2f2e 6769  ks/blob/main/.gi
+00000cb0: 7468 7562 2f43 4f4e 5452 4942 5554 494e  thub/CONTRIBUTIN
+00000cc0: 472e 6d64 290a 666f 7220 6d6f 7265 2069  G.md).for more i
+00000cd0: 6e66 6f72 6d61 7469 6f6e 2e0a            nformation..
```

### Comparing `slack_cli_hooks-0.0.0.dev1/pyproject.toml` & `slack_cli_hooks-0.0.0.dev2/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,30 +1,27 @@
 [build-system]
-requires = ["setuptools", "pytest-runner"]
+requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "slack_cli_hooks"
 dynamic = ["version", "readme", "dependencies"]
 description = "The Slack CLI contract implementation for Bolt Python"
 license = { text = "MIT" }
 authors = [{ name = "Slack Technologies, LLC", email = "opensource@slack.com" }]
-requires-python = ">=3.6"
+requires-python = ">=3.9"
 classifiers = [
 	"Development Status :: 2 - Pre-Alpha",
 	"Environment :: Console",
 	"Intended Audience :: Developers",
 	"Topic :: Office/Business",
 	"Topic :: Software Development",
 	"License :: OSI Approved :: MIT License",
 	"Programming Language :: Python",
 	"Programming Language :: Python :: 3 :: Only",
-	"Programming Language :: Python :: 3.6",
-	"Programming Language :: Python :: 3.7",
-	"Programming Language :: Python :: 3.8",
 	"Programming Language :: Python :: 3.9",
 	"Programming Language :: Python :: 3.10",
 	"Programming Language :: Python :: 3.11",
 	"Programming Language :: Python :: 3.12",
 	"Programming Language :: Python :: Implementation :: CPython",
 	"Programming Language :: Python :: Implementation :: PyPy",
 ]
```

### Comparing `slack_cli_hooks-0.0.0.dev1/slack_cli_hooks/hooks/check_update.py` & `slack_cli_hooks-0.0.0.dev2/slack_cli_hooks/hooks/check_update.py`

 * *Files 15% similar despite different names*

```diff
@@ -3,36 +3,25 @@
 from http.client import HTTPResponse
 from types import ModuleType
 from typing import Any, Dict, List, Optional
 from urllib import request
 
 import slack_bolt
 import slack_sdk
-from pkg_resources import parse_version as Version
+from packaging.version import Version
 
 import slack_cli_hooks.version
 from slack_cli_hooks.error import PypiError
 from slack_cli_hooks.protocol import Protocol, build_protocol
 
 PROTOCOL: Protocol
 
 DEPENDENCIES: List[ModuleType] = [slack_cli_hooks, slack_bolt, slack_sdk]
 
 
-def parse_major(v: Version) -> int:
-    """The first item of :attr:`release` or ``0`` if unavailable.
-
-    >>> parse_major(Version("1.2.3"))
-    1
-    """
-    # This implementation comes directly from the Version implementation since it is not supported in 3.6
-    # source: https://github.com/pypa/packaging/blob/main/src/packaging/version.py
-    return v._version.release[0] if len(v._version) >= 1 else 0  # type: ignore
-
-
 class Release:
     def __init__(
         self,
         name: str,
         current: Optional[Version] = None,
         latest: Optional[Version] = None,
         message: Optional[str] = None,
@@ -40,15 +29,15 @@
         error: Optional[Dict[str, str]] = None,
     ):
         self.name = name
         if current and latest:
             self.current = current.base_version
             self.latest = latest.base_version
             self.update = current < latest
-            self.breaking = (parse_major(current) - parse_major(latest)) != 0
+            self.breaking = (current.major - latest.major) != 0
         if error:
             self.error = error
         if message:
             self.message = message
         if url:
             self.url = url
```

### Comparing `slack_cli_hooks-0.0.0.dev1/slack_cli_hooks/hooks/get_hooks.py` & `slack_cli_hooks-0.0.0.dev2/slack_cli_hooks/hooks/get_hooks.py`

 * *Files identical despite different names*

### Comparing `slack_cli_hooks-0.0.0.dev1/slack_cli_hooks/hooks/get_manifest.py` & `slack_cli_hooks-0.0.0.dev2/slack_cli_hooks/hooks/get_manifest.py`

 * *Files identical despite different names*

### Comparing `slack_cli_hooks-0.0.0.dev1/slack_cli_hooks/hooks/start.py` & `slack_cli_hooks-0.0.0.dev2/slack_cli_hooks/hooks/start.py`

 * *Files identical despite different names*

### Comparing `slack_cli_hooks-0.0.0.dev1/slack_cli_hooks/hooks/utils/managed_os_env_vars.py` & `slack_cli_hooks-0.0.0.dev2/slack_cli_hooks/hooks/utils/managed_os_env_vars.py`

 * *Files identical despite different names*

### Comparing `slack_cli_hooks-0.0.0.dev1/slack_cli_hooks/protocol/__init__.py` & `slack_cli_hooks-0.0.0.dev2/slack_cli_hooks/protocol/__init__.py`

 * *Files identical despite different names*

### Comparing `slack_cli_hooks-0.0.0.dev1/slack_cli_hooks/protocol/default_protocol.py` & `slack_cli_hooks-0.0.0.dev2/slack_cli_hooks/protocol/default_protocol.py`

 * *Files identical despite different names*

### Comparing `slack_cli_hooks-0.0.0.dev1/slack_cli_hooks/protocol/message_boundary_protocol.py` & `slack_cli_hooks-0.0.0.dev2/slack_cli_hooks/protocol/message_boundary_protocol.py`

 * *Files identical despite different names*

### Comparing `slack_cli_hooks-0.0.0.dev1/slack_cli_hooks/protocol/protocol.py` & `slack_cli_hooks-0.0.0.dev2/slack_cli_hooks/protocol/protocol.py`

 * *Files identical despite different names*

### Comparing `slack_cli_hooks-0.0.0.dev1/slack_cli_hooks.egg-info/SOURCES.txt` & `slack_cli_hooks-0.0.0.dev2/slack_cli_hooks.egg-info/SOURCES.txt`

 * *Files identical despite different names*

