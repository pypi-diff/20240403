# Comparing `tmp/willse_backgammon-0.0.1.tar.gz` & `tmp/willse_backgammon-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "willse_backgammon-0.0.1.tar", last modified: Sun Mar 24 03:30:16 2024, max compression
+gzip compressed data, was "willse_backgammon-0.0.2.tar", last modified: Wed Apr  3 18:34:07 2024, max compression
```

## Comparing `willse_backgammon-0.0.1.tar` & `willse_backgammon-0.0.2.tar`

### file list

```diff
@@ -1,64 +1,64 @@
-drwxrwxrwx   0        0        0        0 2024-03-24 03:30:16.593618 willse_backgammon-0.0.1/
--rw-rw-rw-   0        0        0      175 2024-03-24 02:12:02.000000 willse_backgammon-0.0.1/MANIFEST.in
--rw-rw-rw-   0        0        0     1178 2024-03-24 03:30:16.593618 willse_backgammon-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0      588 2024-03-24 03:29:55.000000 willse_backgammon-0.0.1/README.md
--rw-rw-rw-   0        0        0      774 2024-03-24 03:29:50.000000 willse_backgammon-0.0.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-03-24 03:30:16.593618 willse_backgammon-0.0.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-03-24 03:30:16.532686 willse_backgammon-0.0.1/src/
-drwxrwxrwx   0        0        0        0 2024-03-24 03:30:16.537643 willse_backgammon-0.0.1/src/willse_backgammon/
-drwxrwxrwx   0        0        0        0 2024-03-24 03:30:16.562804 willse_backgammon-0.0.1/src/willse_backgammon/AI_Agents/
-drwxrwxrwx   0        0        0        0 2024-03-24 03:30:16.562804 willse_backgammon-0.0.1/src/willse_backgammon/AI_Agents/Data_Sets/
--rw-rw-rw-   0        0        0  2134016 2024-03-05 21:41:44.000000 willse_backgammon-0.0.1/src/willse_backgammon/AI_Agents/Data_Sets/Network_Type1_Data.db
--rw-rw-rw-   0        0        0     8192 2024-03-24 03:14:18.000000 willse_backgammon-0.0.1/src/willse_backgammon/AI_Agents/Data_Sets/Network_Type2_Data.db
--rw-rw-rw-   0        0        0    98700 2024-03-24 02:50:39.000000 willse_backgammon-0.0.1/src/willse_backgammon/AI_Agents/Data_Sets/data_set_1.csv
--rw-rw-rw-   0        0        0     5930 2024-03-24 03:12:57.000000 willse_backgammon-0.0.1/src/willse_backgammon/AI_Agents/Network_Type1.py
--rw-rw-rw-   0        0        0     2676 2024-03-24 03:14:15.000000 willse_backgammon-0.0.1/src/willse_backgammon/AI_Agents/Network_Type2.py
--rw-rw-rw-   0        0        0      858 2024-03-23 17:15:51.000000 willse_backgammon-0.0.1/src/willse_backgammon/AI_Agents/Pick_Best_Pip.py
--rw-rw-rw-   0        0        0     6249 2024-03-23 17:16:28.000000 willse_backgammon-0.0.1/src/willse_backgammon/AI_Agents/TreeSearchI.py
--rw-rw-rw-   0        0        0        0 2024-03-05 21:41:44.000000 willse_backgammon-0.0.1/src/willse_backgammon/AI_Agents/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-24 03:30:16.568264 willse_backgammon-0.0.1/src/willse_backgammon/AI_Agents/__pycache__/
--rw-rw-rw-   0        0        0     5569 2024-03-24 02:49:01.000000 willse_backgammon-0.0.1/src/willse_backgammon/AI_Agents/__pycache__/Network_Type1.cpython-310.pyc
--rw-rw-rw-   0        0        0      900 2024-03-24 02:22:09.000000 willse_backgammon-0.0.1/src/willse_backgammon/AI_Agents/__pycache__/Pick_Best_Pip.cpython-310.pyc
--rw-rw-rw-   0        0        0     4583 2024-03-24 02:22:09.000000 willse_backgammon-0.0.1/src/willse_backgammon/AI_Agents/__pycache__/TreeSearchI.cpython-310.pyc
--rw-rw-rw-   0        0        0      179 2024-03-24 02:22:08.000000 willse_backgammon-0.0.1/src/willse_backgammon/AI_Agents/__pycache__/__init__.cpython-310.pyc
-drwxrwxrwx   0        0        0        0 2024-03-24 03:30:16.585469 willse_backgammon-0.0.1/src/willse_backgammon/Images/
--rw-rw-rw-   0        0        0    54072 2024-03-05 21:41:44.000000 willse_backgammon-0.0.1/src/willse_backgammon/Images/Move.png
--rw-rw-rw-   0        0        0    56088 2024-03-05 21:41:44.000000 willse_backgammon-0.0.1/src/willse_backgammon/Images/Submove.png
--rw-rw-rw-   0        0        0    22157 2024-03-05 21:41:44.000000 willse_backgammon-0.0.1/src/willse_backgammon/Images/darkPiece.png
--rw-rw-rw-   0        0        0    23107 2024-03-05 21:41:44.000000 willse_backgammon-0.0.1/src/willse_backgammon/Images/darkPiece2.png
--rw-rw-rw-   0        0        0    22226 2024-03-05 21:41:44.000000 willse_backgammon-0.0.1/src/willse_backgammon/Images/darkPiece3.png
--rw-rw-rw-   0        0        0    18382 2024-03-05 21:41:44.000000 willse_backgammon-0.0.1/src/willse_backgammon/Images/delete_icon.png
--rw-rw-rw-   0        0        0    20857 2024-03-05 21:41:44.000000 willse_backgammon-0.0.1/src/willse_backgammon/Images/delete_icon2.png
--rw-rw-rw-   0        0        0    16892 2024-03-05 21:41:44.000000 willse_backgammon-0.0.1/src/willse_backgammon/Images/delete_icon3.png
--rw-rw-rw-   0        0        0     4133 2024-03-05 21:41:44.000000 willse_backgammon-0.0.1/src/willse_backgammon/Images/exit_icon.png
--rw-rw-rw-   0        0        0     7613 2024-03-05 21:41:44.000000 willse_backgammon-0.0.1/src/willse_backgammon/Images/gear_icon.png
--rw-rw-rw-   0        0        0    22231 2024-03-05 21:41:44.000000 willse_backgammon-0.0.1/src/willse_backgammon/Images/lightPiece.png
--rw-rw-rw-   0        0        0    22657 2024-03-05 21:41:44.000000 willse_backgammon-0.0.1/src/willse_backgammon/Images/lightPiece2.png
--rw-rw-rw-   0        0        0    22096 2024-03-05 21:41:44.000000 willse_backgammon-0.0.1/src/willse_backgammon/Images/lightPiece3.png
--rw-rw-rw-   0        0        0     5576 2024-03-05 21:41:44.000000 willse_backgammon-0.0.1/src/willse_backgammon/Images/quit_icon.png
--rw-rw-rw-   0        0        0    16049 2024-03-05 21:41:44.000000 willse_backgammon-0.0.1/src/willse_backgammon/Images/restart_icon.png
--rw-rw-rw-   0        0        0    15746 2024-03-05 21:41:44.000000 willse_backgammon-0.0.1/src/willse_backgammon/Images/restart_icon2.png
--rw-rw-rw-   0        0        0    16632 2024-03-05 21:41:44.000000 willse_backgammon-0.0.1/src/willse_backgammon/Images/restart_icon3.png
--rw-rw-rw-   0        0        0     1431 2024-03-24 02:11:25.000000 willse_backgammon-0.0.1/src/willse_backgammon/Main.py
-drwxrwxrwx   0        0        0        0 2024-03-24 03:30:16.590165 willse_backgammon-0.0.1/src/willse_backgammon/Main_Files/
--rw-rw-rw-   0        0        0     3766 2024-03-23 17:10:54.000000 willse_backgammon-0.0.1/src/willse_backgammon/Main_Files/AI.py
--rw-rw-rw-   0        0        0    16291 2024-03-23 19:03:29.000000 willse_backgammon-0.0.1/src/willse_backgammon/Main_Files/Graphics.py
--rw-rw-rw-   0        0        0    17746 2024-03-23 17:12:01.000000 willse_backgammon-0.0.1/src/willse_backgammon/Main_Files/Logic.py
--rw-rw-rw-   0        0        0    48714 2024-03-23 17:14:23.000000 willse_backgammon-0.0.1/src/willse_backgammon/Main_Files/Views.py
--rw-rw-rw-   0        0        0        0 2024-03-05 21:41:44.000000 willse_backgammon-0.0.1/src/willse_backgammon/Main_Files/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-24 03:30:16.593618 willse_backgammon-0.0.1/src/willse_backgammon/Main_Files/__pycache__/
--rw-rw-rw-   0        0        0     2679 2024-03-24 02:22:08.000000 willse_backgammon-0.0.1/src/willse_backgammon/Main_Files/__pycache__/AI.cpython-310.pyc
--rw-rw-rw-   0        0        0    11041 2024-03-24 02:22:08.000000 willse_backgammon-0.0.1/src/willse_backgammon/Main_Files/__pycache__/Graphics.cpython-310.pyc
--rw-rw-rw-   0        0        0     9242 2024-03-24 02:22:08.000000 willse_backgammon-0.0.1/src/willse_backgammon/Main_Files/__pycache__/Logic.cpython-310.pyc
--rw-rw-rw-   0        0        0    33317 2024-03-24 02:22:08.000000 willse_backgammon-0.0.1/src/willse_backgammon/Main_Files/__pycache__/Views.cpython-310.pyc
--rw-rw-rw-   0        0        0      180 2024-03-24 02:22:08.000000 willse_backgammon-0.0.1/src/willse_backgammon/Main_Files/__pycache__/__init__.cpython-310.pyc
--rw-rw-rw-   0        0        0     5083 2024-03-23 17:09:36.000000 willse_backgammon-0.0.1/src/willse_backgammon/Manual.py
--rw-rw-rw-   0        0        0    11375 2024-03-24 03:07:51.000000 willse_backgammon-0.0.1/src/willse_backgammon/Network.py
--rw-rw-rw-   0        0        0        0 2024-03-05 21:41:44.000000 willse_backgammon-0.0.1/src/willse_backgammon/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-24 03:30:16.593618 willse_backgammon-0.0.1/src/willse_backgammon.egg-info/
--rw-rw-rw-   0        0        0     1178 2024-03-24 03:30:16.000000 willse_backgammon-0.0.1/src/willse_backgammon.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2450 2024-03-24 03:30:16.000000 willse_backgammon-0.0.1/src/willse_backgammon.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-24 03:30:16.000000 willse_backgammon-0.0.1/src/willse_backgammon.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       70 2024-03-24 03:30:16.000000 willse_backgammon-0.0.1/src/willse_backgammon.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       13 2024-03-24 03:30:16.000000 willse_backgammon-0.0.1/src/willse_backgammon.egg-info/requires.txt
--rw-rw-rw-   0        0        0       18 2024-03-24 03:30:16.000000 willse_backgammon-0.0.1/src/willse_backgammon.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-03 18:34:07.888026 willse_backgammon-0.0.2/
+-rw-rw-rw-   0        0        0      175 2024-03-24 02:12:02.000000 willse_backgammon-0.0.2/MANIFEST.in
+-rw-rw-rw-   0        0        0     1201 2024-04-03 18:34:07.888026 willse_backgammon-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0      588 2024-04-03 18:33:25.000000 willse_backgammon-0.0.2/README.md
+-rw-rw-rw-   0        0        0      789 2024-04-03 18:28:18.000000 willse_backgammon-0.0.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-03 18:34:07.888026 willse_backgammon-0.0.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-03 18:34:07.660981 willse_backgammon-0.0.2/src/
+drwxrwxrwx   0        0        0        0 2024-04-03 18:34:07.682295 willse_backgammon-0.0.2/src/willse_backgammon/
+drwxrwxrwx   0        0        0        0 2024-04-03 18:34:07.734420 willse_backgammon-0.0.2/src/willse_backgammon/AI_Agents/
+drwxrwxrwx   0        0        0        0 2024-04-03 18:34:07.751575 willse_backgammon-0.0.2/src/willse_backgammon/AI_Agents/Data_Sets/
+-rw-rw-rw-   0        0        0  2134016 2024-03-05 21:41:44.000000 willse_backgammon-0.0.2/src/willse_backgammon/AI_Agents/Data_Sets/Network_Type1_Data.db
+-rw-rw-rw-   0        0        0     8192 2024-03-24 03:14:18.000000 willse_backgammon-0.0.2/src/willse_backgammon/AI_Agents/Data_Sets/Network_Type2_Data.db
+-rw-rw-rw-   0        0        0  5918748 2024-04-03 18:28:06.000000 willse_backgammon-0.0.2/src/willse_backgammon/AI_Agents/Data_Sets/data_set_1.csv
+-rw-rw-rw-   0        0        0     5930 2024-03-24 03:12:57.000000 willse_backgammon-0.0.2/src/willse_backgammon/AI_Agents/Network_Type1.py
+-rw-rw-rw-   0        0        0     2676 2024-03-24 03:14:15.000000 willse_backgammon-0.0.2/src/willse_backgammon/AI_Agents/Network_Type2.py
+-rw-rw-rw-   0        0        0      858 2024-03-23 17:15:51.000000 willse_backgammon-0.0.2/src/willse_backgammon/AI_Agents/Pick_Best_Pip.py
+-rw-rw-rw-   0        0        0     6249 2024-03-25 21:02:29.000000 willse_backgammon-0.0.2/src/willse_backgammon/AI_Agents/TreeSearchI.py
+-rw-rw-rw-   0        0        0        0 2024-03-05 21:41:44.000000 willse_backgammon-0.0.2/src/willse_backgammon/AI_Agents/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-03 18:34:07.759371 willse_backgammon-0.0.2/src/willse_backgammon/AI_Agents/__pycache__/
+-rw-rw-rw-   0        0        0     5660 2024-03-24 17:31:15.000000 willse_backgammon-0.0.2/src/willse_backgammon/AI_Agents/__pycache__/Network_Type1.cpython-310.pyc
+-rw-rw-rw-   0        0        0      900 2024-03-24 02:22:09.000000 willse_backgammon-0.0.2/src/willse_backgammon/AI_Agents/__pycache__/Pick_Best_Pip.cpython-310.pyc
+-rw-rw-rw-   0        0        0     4583 2024-03-25 21:03:36.000000 willse_backgammon-0.0.2/src/willse_backgammon/AI_Agents/__pycache__/TreeSearchI.cpython-310.pyc
+-rw-rw-rw-   0        0        0      179 2024-03-24 02:22:08.000000 willse_backgammon-0.0.2/src/willse_backgammon/AI_Agents/__pycache__/__init__.cpython-310.pyc
+drwxrwxrwx   0        0        0        0 2024-04-03 18:34:07.850522 willse_backgammon-0.0.2/src/willse_backgammon/Images/
+-rw-rw-rw-   0        0        0    54072 2024-03-05 21:41:44.000000 willse_backgammon-0.0.2/src/willse_backgammon/Images/Move.png
+-rw-rw-rw-   0        0        0    56088 2024-03-05 21:41:44.000000 willse_backgammon-0.0.2/src/willse_backgammon/Images/Submove.png
+-rw-rw-rw-   0        0        0    22157 2024-03-05 21:41:44.000000 willse_backgammon-0.0.2/src/willse_backgammon/Images/darkPiece.png
+-rw-rw-rw-   0        0        0    23107 2024-03-05 21:41:44.000000 willse_backgammon-0.0.2/src/willse_backgammon/Images/darkPiece2.png
+-rw-rw-rw-   0        0        0    22226 2024-03-05 21:41:44.000000 willse_backgammon-0.0.2/src/willse_backgammon/Images/darkPiece3.png
+-rw-rw-rw-   0        0        0    18382 2024-03-05 21:41:44.000000 willse_backgammon-0.0.2/src/willse_backgammon/Images/delete_icon.png
+-rw-rw-rw-   0        0        0    20857 2024-03-05 21:41:44.000000 willse_backgammon-0.0.2/src/willse_backgammon/Images/delete_icon2.png
+-rw-rw-rw-   0        0        0    16892 2024-03-05 21:41:44.000000 willse_backgammon-0.0.2/src/willse_backgammon/Images/delete_icon3.png
+-rw-rw-rw-   0        0        0     4133 2024-03-05 21:41:44.000000 willse_backgammon-0.0.2/src/willse_backgammon/Images/exit_icon.png
+-rw-rw-rw-   0        0        0     7613 2024-03-05 21:41:44.000000 willse_backgammon-0.0.2/src/willse_backgammon/Images/gear_icon.png
+-rw-rw-rw-   0        0        0    22231 2024-03-05 21:41:44.000000 willse_backgammon-0.0.2/src/willse_backgammon/Images/lightPiece.png
+-rw-rw-rw-   0        0        0    22657 2024-03-05 21:41:44.000000 willse_backgammon-0.0.2/src/willse_backgammon/Images/lightPiece2.png
+-rw-rw-rw-   0        0        0    22096 2024-03-05 21:41:44.000000 willse_backgammon-0.0.2/src/willse_backgammon/Images/lightPiece3.png
+-rw-rw-rw-   0        0        0     5576 2024-03-05 21:41:44.000000 willse_backgammon-0.0.2/src/willse_backgammon/Images/quit_icon.png
+-rw-rw-rw-   0        0        0    16049 2024-03-05 21:41:44.000000 willse_backgammon-0.0.2/src/willse_backgammon/Images/restart_icon.png
+-rw-rw-rw-   0        0        0    15746 2024-03-05 21:41:44.000000 willse_backgammon-0.0.2/src/willse_backgammon/Images/restart_icon2.png
+-rw-rw-rw-   0        0        0    16632 2024-03-05 21:41:44.000000 willse_backgammon-0.0.2/src/willse_backgammon/Images/restart_icon3.png
+-rw-rw-rw-   0        0        0     1431 2024-03-24 02:11:25.000000 willse_backgammon-0.0.2/src/willse_backgammon/Main.py
+drwxrwxrwx   0        0        0        0 2024-04-03 18:34:07.881204 willse_backgammon-0.0.2/src/willse_backgammon/Main_Files/
+-rw-rw-rw-   0        0        0     3766 2024-03-25 21:03:10.000000 willse_backgammon-0.0.2/src/willse_backgammon/Main_Files/AI.py
+-rw-rw-rw-   0        0        0    16288 2024-04-03 18:28:52.000000 willse_backgammon-0.0.2/src/willse_backgammon/Main_Files/Graphics.py
+-rw-rw-rw-   0        0        0    17634 2024-04-03 18:28:06.000000 willse_backgammon-0.0.2/src/willse_backgammon/Main_Files/Logic.py
+-rw-rw-rw-   0        0        0    59110 2024-03-26 21:12:53.000000 willse_backgammon-0.0.2/src/willse_backgammon/Main_Files/Views.py
+-rw-rw-rw-   0        0        0        0 2024-03-05 21:41:44.000000 willse_backgammon-0.0.2/src/willse_backgammon/Main_Files/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-03 18:34:07.888026 willse_backgammon-0.0.2/src/willse_backgammon/Main_Files/__pycache__/
+-rw-rw-rw-   0        0        0     2679 2024-03-25 21:03:36.000000 willse_backgammon-0.0.2/src/willse_backgammon/Main_Files/__pycache__/AI.cpython-310.pyc
+-rw-rw-rw-   0        0        0    11041 2024-03-24 02:22:08.000000 willse_backgammon-0.0.2/src/willse_backgammon/Main_Files/__pycache__/Graphics.cpython-310.pyc
+-rw-rw-rw-   0        0        0     9228 2024-03-26 21:16:46.000000 willse_backgammon-0.0.2/src/willse_backgammon/Main_Files/__pycache__/Logic.cpython-310.pyc
+-rw-rw-rw-   0        0        0    39258 2024-03-26 21:12:58.000000 willse_backgammon-0.0.2/src/willse_backgammon/Main_Files/__pycache__/Views.cpython-310.pyc
+-rw-rw-rw-   0        0        0      180 2024-03-24 02:22:08.000000 willse_backgammon-0.0.2/src/willse_backgammon/Main_Files/__pycache__/__init__.cpython-310.pyc
+-rw-rw-rw-   0        0        0     5697 2024-04-03 18:28:06.000000 willse_backgammon-0.0.2/src/willse_backgammon/Manual.py
+-rw-rw-rw-   0        0        0    11375 2024-03-24 03:07:51.000000 willse_backgammon-0.0.2/src/willse_backgammon/Network.py
+-rw-rw-rw-   0        0        0        0 2024-03-05 21:41:44.000000 willse_backgammon-0.0.2/src/willse_backgammon/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-03 18:34:07.888026 willse_backgammon-0.0.2/src/willse_backgammon.egg-info/
+-rw-rw-rw-   0        0        0     1201 2024-04-03 18:34:07.000000 willse_backgammon-0.0.2/src/willse_backgammon.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2450 2024-04-03 18:34:07.000000 willse_backgammon-0.0.2/src/willse_backgammon.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-03 18:34:07.000000 willse_backgammon-0.0.2/src/willse_backgammon.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       70 2024-04-03 18:34:07.000000 willse_backgammon-0.0.2/src/willse_backgammon.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       20 2024-04-03 18:34:07.000000 willse_backgammon-0.0.2/src/willse_backgammon.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       18 2024-04-03 18:34:07.000000 willse_backgammon-0.0.2/src/willse_backgammon.egg-info/top_level.txt
```

### Comparing `willse_backgammon-0.0.1/PKG-INFO` & `willse_backgammon-0.0.2/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 Metadata-Version: 2.1
 Name: willse_backgammon
-Version: 0.0.1
+Version: 0.0.2
 Summary: This package is a project I have created to learn python as well as the basics of Artificial Intelligence. It is still a Work in Progress.
 Author-email: Wills Erda <willse06@gmail.com>
 Project-URL: Homepage, https://github.com/GillsSpace/Backgammon_AI
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Requires-Dist: arcade
 Requires-Dist: numpy
+Requires-Dist: pandas
 
 
 # willse_backgammon
 
 This project was created my me to practice and improve my python skils and to learn about nureal networks and machine learning. It is very much still a work in progress.
 
 
@@ -24,21 +25,21 @@
 
 ```bash
   pip install willse_backgammon
 ```
     
 ## Run Locally
 
-After Intsallation, you can run the main application with the following command from terminal:
+After Installation, you can run the main application with the following command from terminal:
 
 ```bash
   > willse_backgammon_run
 ```
 
 
 ## Features
 
 - Two Player, Single Player, and Simulation Modes
-- Multiple AI modles
-- Currently v0.0.1
+- Multiple AI models
+- Currently v0.0.2
```

### Comparing `willse_backgammon-0.0.1/README.md` & `willse_backgammon-0.0.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -10,21 +10,21 @@
 
 ```bash
   pip install willse_backgammon
 ```
     
 ## Run Locally
 
-After Intsallation, you can run the main application with the following command from terminal:
+After Installation, you can run the main application with the following command from terminal:
 
 ```bash
   > willse_backgammon_run
 ```
 
 
 ## Features
 
 - Two Player, Single Player, and Simulation Modes
-- Multiple AI modles
-- Currently v0.0.1
+- Multiple AI models
+- Currently v0.0.2
```

### Comparing `willse_backgammon-0.0.1/pyproject.toml` & `willse_backgammon-0.0.2/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,28 +1,29 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "willse_backgammon"
-version = "0.0.1"
+version = "0.0.2"
 authors = [
   { name="Wills Erda", email="willse06@gmail.com" },
 ]
 description = "This package is a project I have created to learn python as well as the basics of Artificial Intelligence. It is still a Work in Progress."
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 dependencies = [
     "arcade",
     "numpy",
+    "pandas",
 ]
 
 [project.urls]
 Homepage = "https://github.com/GillsSpace/Backgammon_AI"
 
 [project.scripts]
 willse_backgammon_run = "willse_backgammon.Main:main"
```

### Comparing `willse_backgammon-0.0.1/src/willse_backgammon/AI_Agents/Data_Sets/Network_Type1_Data.db` & `willse_backgammon-0.0.2/src/willse_backgammon/AI_Agents/Data_Sets/Network_Type1_Data.db`

 * *Files identical despite different names*

### Comparing `willse_backgammon-0.0.1/src/willse_backgammon/AI_Agents/Data_Sets/Network_Type2_Data.db` & `willse_backgammon-0.0.2/src/willse_backgammon/AI_Agents/Data_Sets/Network_Type2_Data.db`

 * *Files identical despite different names*

### Comparing `willse_backgammon-0.0.1/src/willse_backgammon/AI_Agents/Network_Type1.py` & `willse_backgammon-0.0.2/src/willse_backgammon/AI_Agents/Network_Type1.py`

 * *Files identical despite different names*

### Comparing `willse_backgammon-0.0.1/src/willse_backgammon/AI_Agents/Network_Type2.py` & `willse_backgammon-0.0.2/src/willse_backgammon/AI_Agents/Network_Type2.py`

 * *Files identical despite different names*

### Comparing `willse_backgammon-0.0.1/src/willse_backgammon/AI_Agents/Pick_Best_Pip.py` & `willse_backgammon-0.0.2/src/willse_backgammon/AI_Agents/Pick_Best_Pip.py`

 * *Files identical despite different names*

### Comparing `willse_backgammon-0.0.1/src/willse_backgammon/AI_Agents/TreeSearchI.py` & `willse_backgammon-0.0.2/src/willse_backgammon/AI_Agents/TreeSearchI.py`

 * *Files 0% similar despite different names*

```diff
@@ -111,15 +111,15 @@
 # Running:
 def Full_Run(inputBoard: Board, inputTurn: Turn, suppressMultiProcessing=False):
     fastTurn = FastTurn(inputTurn.player, inputTurn.roll)
     # Takes a input of a FastBoard and a FastTurn and returns the optimal move for the current player to make.
     initialTurnSolutions = ReturnTurnSolutions(inputBoard, fastTurn)
     possiblePipDiffs = []
 
-    if len(initialTurnSolutions) < 32 or suppressMultiProcessing == True:
+    if len(initialTurnSolutions) < 48 or suppressMultiProcessing == True:
         for turnSolution in initialTurnSolutions:
             subTurnsList = []
             for roll in Data_rollOptions:
                 instanceSubTurn = SubTurn(turnSolution.Board, turnSolution.MoveSequence, roll,
                                           (1 if fastTurn.player == 2 else 2))
                 subTurnsList.append(instanceSubTurn)
             MaxPipDiffs = []
```

### Comparing `willse_backgammon-0.0.1/src/willse_backgammon/AI_Agents/__pycache__/Network_Type1.cpython-310.pyc` & `willse_backgammon-0.0.2/src/willse_backgammon/AI_Agents/__pycache__/Network_Type1.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Sun Mar 24 02:48:41 2024 UTC, .py size: 5859 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 5% similar despite different names*

```diff
@@ -1,349 +1,354 @@
-00000000: 6f0d 0d0a 0000 0000 8994 ff65 e316 0000  o..........e....
+00000000: 6f0d 0d0a 0000 0000 399a ff65 2a17 0000  o.......9..e*...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 0006 0000 0040 0000 0073 8800 0000 6400  .....@...s....d.
+00000020: 0006 0000 0040 0000 0073 b200 0000 6400  .....@...s....d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a01 6400  d.l.Z.d.d.l.Z.d.
-00000040: 6401 6c02 5a02 6400 6401 6c03 5a04 7a08  d.l.Z.d.d.l.Z.z.
-00000050: 6400 6402 6c05 6d06 5a06 0100 5700 6e0a  d.d.l.m.Z...W.n.
-00000060: 0100 0100 0100 6400 6402 6c07 6d06 5a06  ......d.d.l.m.Z.
-00000070: 0100 5900 4700 6403 6404 8400 6404 8302  ..Y.G.d.d...d...
-00000080: 5a08 4700 6405 6406 8400 6406 8302 5a09  Z.G.d.d...d...Z.
-00000090: 6407 6408 8400 5a0a 6409 6506 640a 6508  d.d...Z.d.e.d.e.
-000000a0: 6604 640b 640c 8404 5a0b 640d 640e 8400  f.d.d...Z.d.d...
-000000b0: 5a0c 6401 5300 290f e900 0000 004e 2901  Z.d.S.)......N).
-000000c0: da05 426f 6172 6463 0000 0000 0000 0000  ..Boardc........
-000000d0: 0000 0000 0000 0000 0300 0000 4000 0000  ............@...
-000000e0: 7316 0000 0065 005a 0164 005a 0264 0564  s....e.Z.d.Z.d.d
-000000f0: 0364 0484 045a 0364 0253 0029 06da 0846  .d...Z.d.S.)...F
-00000100: 6173 7454 7572 6eda 0672 6574 7572 6e4e  astTurn..returnN
-00000110: 6303 0000 0000 0000 0000 0000 0003 0000  c...............
-00000120: 0002 0000 0043 0000 0073 1000 0000 7c01  .....C...s....|.
-00000130: 7c00 5f00 7c02 7c00 5f01 6400 5300 a901  |._.|.|._.d.S...
-00000140: 4e29 02da 0670 6c61 7965 72da 0472 6f6c  N)...player..rol
-00000150: 6c29 03da 0473 656c 6672 0600 0000 7207  l)...selfr....r.
-00000160: 0000 00a9 0072 0900 0000 fa5b 643a 5c28  .....r.....[d:\(
-00000170: 5729 202d 2043 6f64 655c 2857 2920 4261  W) - Code\(W) Ba
-00000180: 636b 6761 6d6d 6f6e 2050 726f 6a65 6374  ckgammon Project
-00000190: 2046 696c 6573 5c73 7263 5c77 696c 6c73   Files\src\wills
-000001a0: 655f 6261 636b 6761 6d6d 6f6e 5c41 495f  e_backgammon\AI_
-000001b0: 4167 656e 7473 5c4e 6574 776f 726b 5f54  Agents\Network_T
-000001c0: 7970 6531 2e70 79da 085f 5f69 6e69 745f  ype1.py..__init_
-000001d0: 5f0c 0000 0073 0400 0000 0601 0a01 7a11  _....s........z.
-000001e0: 4661 7374 5475 726e 2e5f 5f69 6e69 745f  FastTurn.__init_
-000001f0: 5f29 0272 0400 0000 4e29 04da 085f 5f6e  _).r....N)...__n
-00000200: 616d 655f 5fda 0a5f 5f6d 6f64 756c 655f  ame__..__module_
-00000210: 5fda 0c5f 5f71 7561 6c6e 616d 655f 5f72  _..__qualname__r
-00000220: 0b00 0000 7209 0000 0072 0900 0000 7209  ....r....r....r.
-00000230: 0000 0072 0a00 0000 7203 0000 000b 0000  ...r....r.......
-00000240: 0073 0400 0000 0800 0e01 7203 0000 0063  .s........r....c
-00000250: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000260: 0200 0000 4000 0000 7344 0000 0065 005a  ....@...sD...e.Z
-00000270: 0164 005a 0264 0164 0284 005a 0364 0364  .d.Z.d.d...Z.d.d
-00000280: 0484 005a 0464 0564 0684 005a 0564 0764  ...Z.d.d...Z.d.d
-00000290: 0884 005a 0664 0964 0a84 005a 0764 0b64  ...Z.d.d...Z.d.d
-000002a0: 0c84 005a 0864 0d64 0e84 005a 0964 0f53  ...Z.d.d...Z.d.S
-000002b0: 0029 10da 1742 6163 6b67 616d 6d6f 6e4e  .)...BackgammonN
-000002c0: 6575 7261 6c4e 6574 776f 726b 6302 0000  euralNetworkc...
-000002d0: 0000 0000 0000 0000 0002 0000 0005 0000  ................
-000002e0: 0043 0000 0073 9000 0000 7400 a001 7c01  .C...s....t...|.
-000002f0: 6400 6401 8502 1900 a101 a002 6402 6403  d.d.........d.d.
-00000300: a102 7c00 5f03 7400 a001 7c01 6401 6404  ..|._.t...|.d.d.
-00000310: 8502 1900 a101 7c00 5f04 7400 a001 7c01  ......|._.t...|.
-00000320: 6404 6405 8502 1900 a101 a002 6402 6402  d.d.........d.d.
-00000330: a102 7c00 5f05 7400 a001 7c01 6405 6406  ..|._.t...|.d.d.
-00000340: 8502 1900 a101 7c00 5f06 7400 a001 7c01  ......|._.t...|.
-00000350: 6406 6407 8502 1900 a101 a002 6408 6402  d.d.........d.d.
-00000360: a102 7c00 5f07 7400 a001 7c01 6407 1900  ..|._.t...|.d...
-00000370: a101 7c00 5f08 6400 5300 2909 4e69 8003  ..|._.d.S.).Ni..
-00000380: 0000 e920 0000 00e9 1c00 0000 69a0 0300  ... ........i...
-00000390: 0069 a007 0000 69c0 0700 0069 e007 0000  .i....i....i....
-000003a0: e901 0000 0029 09da 026e 70da 0561 7272  .....)...np..arr
-000003b0: 6179 5a07 7265 7368 6170 65da 0877 6569  ayZ.reshape..wei
-000003c0: 6768 7473 31da 0562 6961 7331 da08 7765  ghts1..bias1..we
-000003d0: 6967 6874 7332 da05 6269 6173 32da 0877  ights2..bias2..w
-000003e0: 6569 6768 7473 33da 0562 6961 7333 2902  eights3..bias3).
-000003f0: 7208 0000 005a 0c77 6569 6768 7473 5f62  r....Z.weights_b
-00000400: 6961 7372 0900 0000 7209 0000 0072 0a00  iasr....r....r..
-00000410: 0000 720b 0000 0012 0000 0073 0c00 0000  ..r........s....
-00000420: 1c02 1401 1c01 1401 1c01 1401 7a20 4261  ............z Ba
-00000430: 636b 6761 6d6d 6f6e 4e65 7572 616c 4e65  ckgammonNeuralNe
-00000440: 7477 6f72 6b2e 5f5f 696e 6974 5f5f 6302  twork.__init__c.
-00000450: 0000 0000 0000 0000 0000 0002 0000 0004  ................
-00000460: 0000 0043 0000 0073 0c00 0000 7400 a001  ...C...s....t...
-00000470: 6401 7c01 a102 5300 2902 4e72 0100 0000  d.|...S.).Nr....
-00000480: 2902 7213 0000 00da 076d 6178 696d 756d  ).r......maximum
-00000490: a902 7208 0000 00da 0178 7209 0000 0072  ..r......xr....r
-000004a0: 0900 0000 720a 0000 00da 0472 656c 751b  ....r......relu.
-000004b0: 0000 0073 0200 0000 0c01 7a1c 4261 636b  ...s......z.Back
-000004c0: 6761 6d6d 6f6e 4e65 7572 616c 4e65 7477  gammonNeuralNetw
-000004d0: 6f72 6b2e 7265 6c75 6302 0000 0000 0000  ork.reluc.......
-000004e0: 0000 0000 0002 0000 0005 0000 0043 0000  .............C..
-000004f0: 0073 1200 0000 7400 a001 7c01 6401 6b04  .s....t...|.d.k.
-00000500: 6402 6401 a103 5300 2903 4e72 0100 0000  d.d...S.).Nr....
-00000510: 7212 0000 0029 0272 1300 0000 da05 7768  r....).r......wh
-00000520: 6572 6572 1c00 0000 7209 0000 0072 0900  erer....r....r..
-00000530: 0000 720a 0000 00da 0664 5f72 656c 751e  ..r......d_relu.
-00000540: 0000 0073 0200 0000 1201 7a1e 4261 636b  ...s......z.Back
-00000550: 6761 6d6d 6f6e 4e65 7572 616c 4e65 7477  gammonNeuralNetw
-00000560: 6f72 6b2e 645f 7265 6c75 6302 0000 0000  ork.d_reluc.....
-00000570: 0000 0000 0000 0002 0000 0006 0000 0043  ...............C
-00000580: 0000 0073 1600 0000 6401 6401 7400 a001  ...s....d.d.t...
-00000590: 7c01 6402 1b00 a101 1700 1b00 5300 2903  |.d.........S.).
-000005a0: 4e72 1200 0000 69f6 ffff ff29 0272 1300  Nr....i....).r..
-000005b0: 0000 da03 6578 7072 1c00 0000 7209 0000  ....expr....r...
-000005c0: 0072 0900 0000 720a 0000 00da 0773 6967  .r....r......sig
-000005d0: 6d6f 6964 2100 0000 7302 0000 0016 017a  moid!...s......z
-000005e0: 1f42 6163 6b67 616d 6d6f 6e4e 6575 7261  .BackgammonNeura
-000005f0: 6c4e 6574 776f 726b 2e73 6967 6d6f 6964  lNetwork.sigmoid
-00000600: 6302 0000 0000 0000 0000 0000 0002 0000  c...............
-00000610: 0005 0000 0043 0000 0073 1800 0000 7c00  .....C...s....|.
-00000620: a000 7c01 a101 6401 7c00 a000 7c01 a101  ..|...d.|...|...
-00000630: 1800 1400 5300 2902 4e72 1200 0000 2901  ....S.).Nr....).
-00000640: 7222 0000 0072 1c00 0000 7209 0000 0072  r"...r....r....r
-00000650: 0900 0000 720a 0000 00da 0964 5f73 6967  ....r......d_sig
-00000660: 6d6f 6964 2400 0000 7302 0000 0018 017a  moid$...s......z
-00000670: 2142 6163 6b67 616d 6d6f 6e4e 6575 7261  !BackgammonNeura
-00000680: 6c4e 6574 776f 726b 2e64 5f73 6967 6d6f  lNetwork.d_sigmo
-00000690: 6964 6303 0000 0000 0000 0000 0000 0007  idc.............
-000006a0: 0000 0006 0000 0003 0000 0073 b600 0000  ...........s....
-000006b0: 7c02 6401 6b02 722e 8700 6601 6402 6403  |.d.k.r...f.d.d.
-000006c0: 8408 7400 6404 6405 6405 8303 4400 8301  ..t.d.d.d...D...
-000006d0: 7d03 7c03 a001 8800 6406 1900 a101 0100  }.|.....d.......
-000006e0: 7c03 a001 8800 6407 1900 a101 0100 7c03  |.....d.......|.
-000006f0: a001 8800 6408 1900 a101 0100 7c03 a001  ....d.......|...
-00000700: 8800 6409 1900 a101 0100 6e02 8800 7d03  ..d.......n...}.
-00000710: 7c00 a002 7403 a004 7c00 6a05 7c03 a102  |...t...|.j.|...
-00000720: 7c00 6a06 1700 a101 7d04 7c00 a002 7403  |.j.....}.|...t.
-00000730: a004 7c00 6a07 7c04 a102 7c00 6a08 1700  ..|.j.|...|.j...
-00000740: a101 7d05 7c00 a009 7403 a004 7c00 6a0a  ..}.|...t...|.j.
-00000750: 7c05 a102 7c00 6a0b 1700 a101 7d06 7c06  |...|.j.....}.|.
-00000760: 640a 1900 5300 290c 7a54 7265 7475 726e  d...S.).zTreturn
-00000770: 7320 7468 6520 6573 7469 6d61 7465 6420  s the estimated 
-00000780: 7661 6c75 6520 6f66 2061 2070 6f73 6974  value of a posit
-00000790: 696f 6e20 666f 7220 706c 6179 6572 2066  ion for player f
-000007a0: 6f6c 6c6f 7769 6e67 2061 206d 6f76 6520  ollowing a move 
-000007b0: 6279 2074 6861 7420 706c 6179 6572 e902  by that player..
-000007c0: 0000 0063 0100 0000 0000 0000 0000 0000  ...c............
-000007d0: 0200 0000 0400 0000 1300 0000 7316 0000  ............s...
-000007e0: 0067 007c 005d 077d 0188 007c 0119 000b  .g.|.].}...|....
-000007f0: 0091 0271 0253 0072 0900 0000 7209 0000  ...q.S.r....r...
-00000800: 0029 02da 022e 30da 0169 a901 da09 706f  .)....0..i....po
-00000810: 7369 7469 6f6e 7372 0900 0000 720a 0000  sitionsr....r...
-00000820: 00da 0a3c 6c69 7374 636f 6d70 3e2d 0000  ...<listcomp>-..
-00000830: 0073 0200 0000 1600 7a33 4261 636b 6761  .s......z3Backga
-00000840: 6d6d 6f6e 4e65 7572 616c 4e65 7477 6f72  mmonNeuralNetwor
-00000850: 6b2e 666f 7277 6172 642e 3c6c 6f63 616c  k.forward.<local
-00000860: 733e 2e3c 6c69 7374 636f 6d70 3ee9 1700  s>.<listcomp>...
-00000870: 0000 e9ff ffff ffe9 1900 0000 e918 0000  ................
-00000880: 00e9 1b00 0000 e91a 0000 0072 0100 0000  ...........r....
-00000890: 4e29 0cda 0572 616e 6765 da06 6170 7065  N)...range..appe
-000008a0: 6e64 721e 0000 0072 1300 0000 da03 646f  ndr....r......do
-000008b0: 7472 1500 0000 7216 0000 0072 1700 0000  tr....r....r....
-000008c0: 7218 0000 0072 2200 0000 7219 0000 0072  r....r"...r....r
-000008d0: 1a00 0000 2907 7208 0000 0072 2800 0000  ....).r....r(...
-000008e0: 7206 0000 00da 0669 6e70 7574 73da 1468  r......inputs..h
-000008f0: 6964 6465 6e5f 6c61 7965 7231 5f6f 7574  idden_layer1_out
-00000900: 7075 74da 1468 6964 6465 6e5f 6c61 7965  put..hidden_laye
-00000910: 7232 5f6f 7574 7075 74da 066f 7574 7075  r2_output..outpu
-00000920: 7472 0900 0000 7227 0000 0072 0a00 0000  tr....r'...r....
-00000930: da07 666f 7277 6172 6427 0000 0073 1600  ..forward'...s..
-00000940: 0000 0805 1a01 0e01 0e01 0e01 1001 0402  ................
-00000950: 1a02 1a01 1a01 0801 7a1f 4261 636b 6761  ........z.Backga
-00000960: 6d6d 6f6e 4e65 7572 616c 4e65 7477 6f72  mmonNeuralNetwor
-00000970: 6b2e 666f 7277 6172 6463 0400 0000 0000  k.forwardc......
-00000980: 0000 0000 0000 0d00 0000 0700 0000 4300  ..............C.
-00000990: 0000 734c 0100 007c 00a0 0074 01a0 027c  ..sL...|...t...|
-000009a0: 017c 006a 03a1 027c 006a 0417 00a1 017d  .|.j...|.j.....}
-000009b0: 047c 00a0 0074 01a0 027c 047c 006a 05a1  .|...t...|.|.j..
-000009c0: 027c 006a 0617 00a1 017d 057c 00a0 0774  .|.j.....}.|...t
-000009d0: 01a0 027c 057c 006a 08a1 027c 006a 0917  ...|.|.j...|.j..
-000009e0: 00a1 017d 067c 067c 0218 007d 077c 077c  ...}.|.|...}.|.|
-000009f0: 00a0 0a7c 06a1 0114 007d 0874 01a0 027c  ...|.....}.t...|
-00000a00: 087c 006a 086a 0ba1 027d 097c 097c 00a0  .|.j.j...}.|.|..
-00000a10: 0c7c 05a1 0114 007d 0a74 01a0 027c 0a7c  .|.....}.t...|.|
-00000a20: 006a 056a 0ba1 027d 0b7c 0b7c 00a0 0c7c  .j.j...}.|.|...|
-00000a30: 04a1 0114 007d 0c7c 0004 006a 087c 0374  .....}.|...j.|.t
-00000a40: 01a0 027c 056a 0b7c 08a1 0214 0038 0002  ...|.j.|.....8..
-00000a50: 005f 087c 0004 006a 097c 0374 016a 0d7c  ._.|...j.|.t.j.|
-00000a60: 0864 0164 028d 0214 0038 0002 005f 097c  .d.d.....8..._.|
-00000a70: 0004 006a 057c 0374 01a0 027c 046a 0b7c  ...j.|.t...|.j.|
-00000a80: 0aa1 0214 0038 0002 005f 057c 0004 006a  .....8..._.|...j
-00000a90: 067c 0374 016a 0d7c 0a64 0164 028d 0214  .|.t.j.|.d.d....
-00000aa0: 0038 0002 005f 067c 0004 006a 037c 0374  .8..._.|...j.|.t
-00000ab0: 01a0 027c 016a 0b7c 0ca1 0214 0038 0002  ...|.j.|.....8..
-00000ac0: 005f 037c 0004 006a 047c 0374 016a 0d7c  ._.|...j.|.t.j.|
-00000ad0: 0c64 0164 028d 0214 0038 0002 005f 0464  .d.d.....8..._.d
-00000ae0: 0053 0029 034e 7201 0000 0029 01da 0461  .S.).Nr....)...a
-00000af0: 7869 7329 0e72 1e00 0000 7213 0000 0072  xis).r....r....r
-00000b00: 3200 0000 7215 0000 0072 1600 0000 7217  2...r....r....r.
-00000b10: 0000 0072 1800 0000 7222 0000 0072 1900  ...r....r"...r..
-00000b20: 0000 721a 0000 0072 2300 0000 da01 5472  ..r....r#.....Tr
-00000b30: 2000 0000 da03 7375 6d29 0d72 0800 0000   .....sum).r....
-00000b40: 7233 0000 00da 0774 6172 6765 7473 5a0d  r3.....targetsZ.
-00000b50: 6c65 6172 6e69 6e67 5f72 6174 6572 3400  learning_rater4.
-00000b60: 0000 7235 0000 0072 3600 0000 5a0c 6f75  ..r5...r6...Z.ou
-00000b70: 7470 7574 5f65 7272 6f72 5a0c 6f75 7470  tput_errorZ.outp
-00000b80: 7574 5f64 656c 7461 5a13 6869 6464 656e  ut_deltaZ.hidden
-00000b90: 5f6c 6179 6572 325f 6572 726f 725a 1368  _layer2_errorZ.h
-00000ba0: 6964 6465 6e5f 6c61 7965 7232 5f64 656c  idden_layer2_del
+00000040: 6401 6c02 5a02 6400 6401 6c03 5a03 6400  d.l.Z.d.d.l.Z.d.
+00000050: 6401 6c04 5a04 6400 6401 6c05 5a06 7a08  d.l.Z.d.d.l.Z.z.
+00000060: 6400 6402 6c07 6d08 5a08 0100 5700 6e0a  d.d.l.m.Z...W.n.
+00000070: 0100 0100 0100 6400 6402 6c09 6d08 5a08  ......d.d.l.m.Z.
+00000080: 0100 5900 6503 a00a 650b a101 6a0c 6a0c  ..Y.e...e...j.j.
+00000090: 6a0c 5a0d 6504 a00e 650d a101 0100 4700  j.Z.e...e.....G.
+000000a0: 6403 6404 8400 6404 8302 5a0f 4700 6405  d.d...d...Z.G.d.
+000000b0: 6406 8400 6406 8302 5a10 6407 6408 8400  d...d...Z.d.d...
+000000c0: 5a11 6409 6508 640a 650f 6604 640b 640c  Z.d.e.d.e.f.d.d.
+000000d0: 8404 5a12 640d 640e 8400 5a13 6401 5300  ..Z.d.d...Z.d.S.
+000000e0: 290f e900 0000 004e 2901 da05 426f 6172  )......N)...Boar
+000000f0: 6463 0000 0000 0000 0000 0000 0000 0000  dc..............
+00000100: 0000 0300 0000 4000 0000 7316 0000 0065  ......@...s....e
+00000110: 005a 0164 005a 0264 0564 0364 0484 045a  .Z.d.Z.d.d.d...Z
+00000120: 0364 0253 0029 06da 0846 6173 7454 7572  .d.S.)...FastTur
+00000130: 6eda 0672 6574 7572 6e4e 6303 0000 0000  n..returnNc.....
+00000140: 0000 0000 0000 0003 0000 0002 0000 0043  ...............C
+00000150: 0000 0073 1000 0000 7c01 7c00 5f00 7c02  ...s....|.|._.|.
+00000160: 7c00 5f01 6400 5300 a901 4e29 02da 0670  |._.d.S...N)...p
+00000170: 6c61 7965 72da 0472 6f6c 6c29 03da 0473  layer..roll)...s
+00000180: 656c 6672 0600 0000 7207 0000 00a9 0072  elfr....r......r
+00000190: 0900 0000 fa5b 643a 5c28 5729 202d 2043  .....[d:\(W) - C
+000001a0: 6f64 655c 2857 2920 4261 636b 6761 6d6d  ode\(W) Backgamm
+000001b0: 6f6e 2050 726f 6a65 6374 2046 696c 6573  on Project Files
+000001c0: 5c73 7263 5c77 696c 6c73 655f 6261 636b  \src\willse_back
+000001d0: 6761 6d6d 6f6e 5c41 495f 4167 656e 7473  gammon\AI_Agents
+000001e0: 5c4e 6574 776f 726b 5f54 7970 6531 2e70  \Network_Type1.p
+000001f0: 79da 085f 5f69 6e69 745f 5f0e 0000 0073  y..__init__....s
+00000200: 0400 0000 0601 0a01 7a11 4661 7374 5475  ........z.FastTu
+00000210: 726e 2e5f 5f69 6e69 745f 5f29 0272 0400  rn.__init__).r..
+00000220: 0000 4e29 04da 085f 5f6e 616d 655f 5fda  ..N)...__name__.
+00000230: 0a5f 5f6d 6f64 756c 655f 5fda 0c5f 5f71  .__module__..__q
+00000240: 7561 6c6e 616d 655f 5f72 0b00 0000 7209  ualname__r....r.
+00000250: 0000 0072 0900 0000 7209 0000 0072 0a00  ...r....r....r..
+00000260: 0000 7203 0000 000d 0000 0073 0400 0000  ..r........s....
+00000270: 0800 0e01 7203 0000 0063 0000 0000 0000  ....r....c......
+00000280: 0000 0000 0000 0000 0000 0200 0000 4000  ..............@.
+00000290: 0000 7344 0000 0065 005a 0164 005a 0264  ..sD...e.Z.d.Z.d
+000002a0: 0164 0284 005a 0364 0364 0484 005a 0464  .d...Z.d.d...Z.d
+000002b0: 0564 0684 005a 0564 0764 0884 005a 0664  .d...Z.d.d...Z.d
+000002c0: 0964 0a84 005a 0764 0b64 0c84 005a 0864  .d...Z.d.d...Z.d
+000002d0: 0d64 0e84 005a 0964 0f53 0029 10da 1742  .d...Z.d.S.)...B
+000002e0: 6163 6b67 616d 6d6f 6e4e 6575 7261 6c4e  ackgammonNeuralN
+000002f0: 6574 776f 726b 6302 0000 0000 0000 0000  etworkc.........
+00000300: 0000 0002 0000 0005 0000 0043 0000 0073  ...........C...s
+00000310: 9000 0000 7400 a001 7c01 6400 6401 8502  ....t...|.d.d...
+00000320: 1900 a101 a002 6402 6403 a102 7c00 5f03  ......d.d...|._.
+00000330: 7400 a001 7c01 6401 6404 8502 1900 a101  t...|.d.d.......
+00000340: 7c00 5f04 7400 a001 7c01 6404 6405 8502  |._.t...|.d.d...
+00000350: 1900 a101 a002 6402 6402 a102 7c00 5f05  ......d.d...|._.
+00000360: 7400 a001 7c01 6405 6406 8502 1900 a101  t...|.d.d.......
+00000370: 7c00 5f06 7400 a001 7c01 6406 6407 8502  |._.t...|.d.d...
+00000380: 1900 a101 a002 6408 6402 a102 7c00 5f07  ......d.d...|._.
+00000390: 7400 a001 7c01 6407 1900 a101 7c00 5f08  t...|.d.....|._.
+000003a0: 6400 5300 2909 4e69 8003 0000 e920 0000  d.S.).Ni..... ..
+000003b0: 00e9 1c00 0000 69a0 0300 0069 a007 0000  ......i....i....
+000003c0: 69c0 0700 0069 e007 0000 e901 0000 0029  i....i.........)
+000003d0: 09da 026e 70da 0561 7272 6179 da07 7265  ...np..array..re
+000003e0: 7368 6170 65da 0877 6569 6768 7473 31da  shape..weights1.
+000003f0: 0562 6961 7331 da08 7765 6967 6874 7332  .bias1..weights2
+00000400: da05 6269 6173 32da 0877 6569 6768 7473  ..bias2..weights
+00000410: 33da 0562 6961 7333 2902 7208 0000 005a  3..bias3).r....Z
+00000420: 0c77 6569 6768 7473 5f62 6961 7372 0900  .weights_biasr..
+00000430: 0000 7209 0000 0072 0a00 0000 720b 0000  ..r....r....r...
+00000440: 0014 0000 0073 0c00 0000 1c02 1401 1c01  .....s..........
+00000450: 1401 1c01 1401 7a20 4261 636b 6761 6d6d  ......z Backgamm
+00000460: 6f6e 4e65 7572 616c 4e65 7477 6f72 6b2e  onNeuralNetwork.
+00000470: 5f5f 696e 6974 5f5f 6302 0000 0000 0000  __init__c.......
+00000480: 0000 0000 0002 0000 0004 0000 0043 0000  .............C..
+00000490: 0073 0c00 0000 7400 a001 6401 7c01 a102  .s....t...d.|...
+000004a0: 5300 2902 4e72 0100 0000 2902 7213 0000  S.).Nr....).r...
+000004b0: 00da 076d 6178 696d 756d a902 7208 0000  ...maximum..r...
+000004c0: 00da 0178 7209 0000 0072 0900 0000 720a  ...xr....r....r.
+000004d0: 0000 00da 0472 656c 751d 0000 0073 0200  .....relu....s..
+000004e0: 0000 0c01 7a1c 4261 636b 6761 6d6d 6f6e  ....z.Backgammon
+000004f0: 4e65 7572 616c 4e65 7477 6f72 6b2e 7265  NeuralNetwork.re
+00000500: 6c75 6302 0000 0000 0000 0000 0000 0002  luc.............
+00000510: 0000 0005 0000 0043 0000 0073 1200 0000  .......C...s....
+00000520: 7400 a001 7c01 6401 6b04 6402 6401 a103  t...|.d.k.d.d...
+00000530: 5300 2903 4e72 0100 0000 7212 0000 0029  S.).Nr....r....)
+00000540: 0272 1300 0000 da05 7768 6572 6572 1d00  .r......wherer..
+00000550: 0000 7209 0000 0072 0900 0000 720a 0000  ..r....r....r...
+00000560: 00da 0664 5f72 656c 7520 0000 0073 0200  ...d_relu ...s..
+00000570: 0000 1201 7a1e 4261 636b 6761 6d6d 6f6e  ....z.Backgammon
+00000580: 4e65 7572 616c 4e65 7477 6f72 6b2e 645f  NeuralNetwork.d_
+00000590: 7265 6c75 6302 0000 0000 0000 0000 0000  reluc...........
+000005a0: 0002 0000 0006 0000 0043 0000 0073 1600  .........C...s..
+000005b0: 0000 6401 6401 7400 a001 7c01 6402 1b00  ..d.d.t...|.d...
+000005c0: a101 1700 1b00 5300 2903 4e72 1200 0000  ......S.).Nr....
+000005d0: 69f6 ffff ff29 0272 1300 0000 da03 6578  i....).r......ex
+000005e0: 7072 1d00 0000 7209 0000 0072 0900 0000  pr....r....r....
+000005f0: 720a 0000 00da 0773 6967 6d6f 6964 2300  r......sigmoid#.
+00000600: 0000 7302 0000 0016 017a 1f42 6163 6b67  ..s......z.Backg
+00000610: 616d 6d6f 6e4e 6575 7261 6c4e 6574 776f  ammonNeuralNetwo
+00000620: 726b 2e73 6967 6d6f 6964 6302 0000 0000  rk.sigmoidc.....
+00000630: 0000 0000 0000 0002 0000 0005 0000 0043  ...............C
+00000640: 0000 0073 1800 0000 7c00 a000 7c01 a101  ...s....|...|...
+00000650: 6401 7c00 a000 7c01 a101 1800 1400 5300  d.|...|.......S.
+00000660: 2902 4e72 1200 0000 2901 7223 0000 0072  ).Nr....).r#...r
+00000670: 1d00 0000 7209 0000 0072 0900 0000 720a  ....r....r....r.
+00000680: 0000 00da 0964 5f73 6967 6d6f 6964 2600  .....d_sigmoid&.
+00000690: 0000 7302 0000 0018 017a 2142 6163 6b67  ..s......z!Backg
+000006a0: 616d 6d6f 6e4e 6575 7261 6c4e 6574 776f  ammonNeuralNetwo
+000006b0: 726b 2e64 5f73 6967 6d6f 6964 6303 0000  rk.d_sigmoidc...
+000006c0: 0000 0000 0000 0000 0007 0000 0006 0000  ................
+000006d0: 0003 0000 0073 b600 0000 7c02 6401 6b02  .....s....|.d.k.
+000006e0: 722e 8700 6601 6402 6403 8408 7400 6404  r...f.d.d...t.d.
+000006f0: 6405 6405 8303 4400 8301 7d03 7c03 a001  d.d...D...}.|...
+00000700: 8800 6406 1900 a101 0100 7c03 a001 8800  ..d.......|.....
+00000710: 6407 1900 a101 0100 7c03 a001 8800 6408  d.......|.....d.
+00000720: 1900 a101 0100 7c03 a001 8800 6409 1900  ......|.....d...
+00000730: a101 0100 6e02 8800 7d03 7c00 a002 7403  ....n...}.|...t.
+00000740: a004 7c00 6a05 7c03 a102 7c00 6a06 1700  ..|.j.|...|.j...
+00000750: a101 7d04 7c00 a002 7403 a004 7c00 6a07  ..}.|...t...|.j.
+00000760: 7c04 a102 7c00 6a08 1700 a101 7d05 7c00  |...|.j.....}.|.
+00000770: a009 7403 a004 7c00 6a0a 7c05 a102 7c00  ..t...|.j.|...|.
+00000780: 6a0b 1700 a101 7d06 7c06 640a 1900 5300  j.....}.|.d...S.
+00000790: 290c 7a54 7265 7475 726e 7320 7468 6520  ).zTreturns the 
+000007a0: 6573 7469 6d61 7465 6420 7661 6c75 6520  estimated value 
+000007b0: 6f66 2061 2070 6f73 6974 696f 6e20 666f  of a position fo
+000007c0: 7220 706c 6179 6572 2066 6f6c 6c6f 7769  r player followi
+000007d0: 6e67 2061 206d 6f76 6520 6279 2074 6861  ng a move by tha
+000007e0: 7420 706c 6179 6572 e902 0000 0063 0100  t player.....c..
+000007f0: 0000 0000 0000 0000 0000 0200 0000 0400  ................
+00000800: 0000 1300 0000 7316 0000 0067 007c 005d  ......s....g.|.]
+00000810: 077d 0188 007c 0119 000b 0091 0271 0253  .}...|.......q.S
+00000820: 0072 0900 0000 7209 0000 0029 02da 022e  .r....r....)....
+00000830: 30da 0169 a901 da09 706f 7369 7469 6f6e  0..i....position
+00000840: 7372 0900 0000 720a 0000 00da 0a3c 6c69  sr....r......<li
+00000850: 7374 636f 6d70 3e2f 0000 0073 0200 0000  stcomp>/...s....
+00000860: 1600 7a33 4261 636b 6761 6d6d 6f6e 4e65  ..z3BackgammonNe
+00000870: 7572 616c 4e65 7477 6f72 6b2e 666f 7277  uralNetwork.forw
+00000880: 6172 642e 3c6c 6f63 616c 733e 2e3c 6c69  ard.<locals>.<li
+00000890: 7374 636f 6d70 3ee9 1700 0000 e9ff ffff  stcomp>.........
+000008a0: ffe9 1900 0000 e918 0000 00e9 1b00 0000  ................
+000008b0: e91a 0000 0072 0100 0000 4e29 0cda 0572  .....r....N)...r
+000008c0: 616e 6765 da06 6170 7065 6e64 721f 0000  ange..appendr...
+000008d0: 0072 1300 0000 da03 646f 7472 1600 0000  .r......dotr....
+000008e0: 7217 0000 0072 1800 0000 7219 0000 0072  r....r....r....r
+000008f0: 2300 0000 721a 0000 0072 1b00 0000 2907  #...r....r....).
+00000900: 7208 0000 0072 2900 0000 7206 0000 00da  r....r)...r.....
+00000910: 0669 6e70 7574 73da 1468 6964 6465 6e5f  .inputs..hidden_
+00000920: 6c61 7965 7231 5f6f 7574 7075 74da 1468  layer1_output..h
+00000930: 6964 6465 6e5f 6c61 7965 7232 5f6f 7574  idden_layer2_out
+00000940: 7075 74da 066f 7574 7075 7472 0900 0000  put..outputr....
+00000950: 7228 0000 0072 0a00 0000 da07 666f 7277  r(...r......forw
+00000960: 6172 6429 0000 0073 1600 0000 0805 1a01  ard)...s........
+00000970: 0e01 0e01 0e01 1001 0402 1a02 1a01 1a01  ................
+00000980: 0801 7a1f 4261 636b 6761 6d6d 6f6e 4e65  ..z.BackgammonNe
+00000990: 7572 616c 4e65 7477 6f72 6b2e 666f 7277  uralNetwork.forw
+000009a0: 6172 6463 0400 0000 0000 0000 0000 0000  ardc............
+000009b0: 0d00 0000 0700 0000 4300 0000 734c 0100  ........C...sL..
+000009c0: 007c 00a0 0074 01a0 027c 017c 006a 03a1  .|...t...|.|.j..
+000009d0: 027c 006a 0417 00a1 017d 047c 00a0 0074  .|.j.....}.|...t
+000009e0: 01a0 027c 047c 006a 05a1 027c 006a 0617  ...|.|.j...|.j..
+000009f0: 00a1 017d 057c 00a0 0774 01a0 027c 057c  ...}.|...t...|.|
+00000a00: 006a 08a1 027c 006a 0917 00a1 017d 067c  .j...|.j.....}.|
+00000a10: 067c 0218 007d 077c 077c 00a0 0a7c 06a1  .|...}.|.|...|..
+00000a20: 0114 007d 0874 01a0 027c 087c 006a 086a  ...}.t...|.|.j.j
+00000a30: 0ba1 027d 097c 097c 00a0 0c7c 05a1 0114  ...}.|.|...|....
+00000a40: 007d 0a74 01a0 027c 0a7c 006a 056a 0ba1  .}.t...|.|.j.j..
+00000a50: 027d 0b7c 0b7c 00a0 0c7c 04a1 0114 007d  .}.|.|...|.....}
+00000a60: 0c7c 0004 006a 087c 0374 01a0 027c 056a  .|...j.|.t...|.j
+00000a70: 0b7c 08a1 0214 0038 0002 005f 087c 0004  .|.....8..._.|..
+00000a80: 006a 097c 0374 016a 0d7c 0864 0164 028d  .j.|.t.j.|.d.d..
+00000a90: 0214 0038 0002 005f 097c 0004 006a 057c  ...8..._.|...j.|
+00000aa0: 0374 01a0 027c 046a 0b7c 0aa1 0214 0038  .t...|.j.|.....8
+00000ab0: 0002 005f 057c 0004 006a 067c 0374 016a  ..._.|...j.|.t.j
+00000ac0: 0d7c 0a64 0164 028d 0214 0038 0002 005f  .|.d.d.....8..._
+00000ad0: 067c 0004 006a 037c 0374 01a0 027c 016a  .|...j.|.t...|.j
+00000ae0: 0b7c 0ca1 0214 0038 0002 005f 037c 0004  .|.....8..._.|..
+00000af0: 006a 047c 0374 016a 0d7c 0c64 0164 028d  .j.|.t.j.|.d.d..
+00000b00: 0214 0038 0002 005f 0464 0053 0029 034e  ...8..._.d.S.).N
+00000b10: 7201 0000 0029 01da 0461 7869 7329 0e72  r....)...axis).r
+00000b20: 1f00 0000 7213 0000 0072 3300 0000 7216  ....r....r3...r.
+00000b30: 0000 0072 1700 0000 7218 0000 0072 1900  ...r....r....r..
+00000b40: 0000 7223 0000 0072 1a00 0000 721b 0000  ..r#...r....r...
+00000b50: 0072 2400 0000 da01 5472 2100 0000 da03  .r$.....Tr!.....
+00000b60: 7375 6d29 0d72 0800 0000 7234 0000 00da  sum).r....r4....
+00000b70: 0774 6172 6765 7473 5a0d 6c65 6172 6e69  .targetsZ.learni
+00000b80: 6e67 5f72 6174 6572 3500 0000 7236 0000  ng_rater5...r6..
+00000b90: 0072 3700 0000 5a0c 6f75 7470 7574 5f65  .r7...Z.output_e
+00000ba0: 7272 6f72 5a0c 6f75 7470 7574 5f64 656c  rrorZ.output_del
 00000bb0: 7461 5a13 6869 6464 656e 5f6c 6179 6572  taZ.hidden_layer
-00000bc0: 315f 6572 726f 725a 1368 6964 6465 6e5f  1_errorZ.hidden_
-00000bd0: 6c61 7965 7231 5f64 656c 7461 7209 0000  layer1_deltar...
-00000be0: 0072 0900 0000 720a 0000 00da 0f62 6163  .r....r......bac
-00000bf0: 6b70 726f 7061 6761 7469 6f6e 3a00 0000  kpropagation:...
-00000c00: 731e 0000 001a 021a 011a 0108 030e 0110  s...............
-00000c10: 020e 0110 020e 011c 031c 011c 021c 011c  ................
-00000c20: 0220 017a 2742 6163 6b67 616d 6d6f 6e4e  . .z'BackgammonN
-00000c30: 6575 7261 6c4e 6574 776f 726b 2e62 6163  euralNetwork.bac
-00000c40: 6b70 726f 7061 6761 7469 6f6e 4e29 0a72  kpropagationN).r
-00000c50: 0c00 0000 720d 0000 0072 0e00 0000 720b  ....r....r....r.
-00000c60: 0000 0072 1e00 0000 7220 0000 0072 2200  ...r....r ...r".
-00000c70: 0000 7223 0000 0072 3700 0000 723c 0000  ..r#...r7...r<..
-00000c80: 0072 0900 0000 7209 0000 0072 0900 0000  .r....r....r....
-00000c90: 720a 0000 0072 0f00 0000 1100 0000 7310  r....r........s.
-00000ca0: 0000 0008 0008 0108 0908 0308 0308 0308  ................
-00000cb0: 030c 1372 0f00 0000 6302 0000 0000 0000  ...r....c.......
-00000cc0: 0000 0000 0009 0000 0006 0000 0043 0000  .............C..
-00000cd0: 0073 9400 0000 6401 7d02 7400 a001 7c02  .s....d.}.t...|.
-00000ce0: a101 7d03 7c03 a002 a100 7d04 7c01 6402  ..}.|.....}.|.d.
-00000cf0: 6b02 7217 7c04 a003 6403 7c00 6601 a102  k.r.|...d.|.f...
-00000d00: 7d05 6e0b 7c01 6404 6b02 7222 7c04 a003  }.n.|.d.k.r"|...
-00000d10: 6405 7c00 6601 a102 7d05 7a10 7404 7c05  d.|.f...}.z.t.|.
-00000d20: a005 a100 6406 1900 6406 1900 8301 7d06  ....d...d.....}.
-00000d30: 7c06 a006 a100 7d06 5700 6e07 0100 0100  |.....}.W.n.....
-00000d40: 0100 6700 0600 5900 5300 6700 7d07 7c06  ..g...Y.S.g.}.|.
-00000d50: 4400 5d09 7d08 7c07 a007 7408 7c08 8301  D.].}.|...t.|...
-00000d60: a101 0100 713e 7c07 5300 2907 4e7a 3b77  ....q>|.S.).Nz;w
-00000d70: 696c 6c73 655f 6261 636b 6761 6d6d 6f6e  illse_backgammon
-00000d80: 2f41 495f 4167 656e 7473 2f44 6174 615f  /AI_Agents/Data_
-00000d90: 5365 7473 2f4e 6574 776f 726b 5f54 7970  Sets/Network_Typ
-00000da0: 6531 5f44 6174 612e 6462 da10 4e65 7477  e1_Data.db..Netw
-00000db0: 6f72 6b5f 5661 6c75 6573 5f31 7a2e 5345  ork_Values_1z.SE
-00000dc0: 4c45 4354 2064 6174 6120 4652 4f4d 204e  LECT data FROM N
-00000dd0: 6574 776f 726b 5f56 616c 7565 735f 3120  etwork_Values_1 
-00000de0: 5748 4552 4520 6964 203d 203f da19 4e65  WHERE id = ?..Ne
-00000df0: 7477 6f72 6b5f 5661 6c75 6573 5f54 6f75  twork_Values_Tou
-00000e00: 726e 616d 656e 747a 3753 454c 4543 5420  rnamentz7SELECT 
-00000e10: 6461 7461 2046 524f 4d20 4e65 7477 6f72  data FROM Networ
-00000e20: 6b5f 5661 6c75 6573 5f54 6f75 726e 616d  k_Values_Tournam
-00000e30: 656e 7420 5748 4552 4520 6964 203d 203f  ent WHERE id = ?
-00000e40: 7201 0000 0029 09da 0773 716c 6974 6533  r....)...sqlite3
-00000e50: da07 636f 6e6e 6563 74da 0663 7572 736f  ..connect..curso
-00000e60: 72da 0765 7865 6375 7465 da03 7374 725a  r..execute..strZ
-00000e70: 0866 6574 6368 616c 6cda 0672 7370 6c69  .fetchall..rspli
-00000e80: 7472 3100 0000 da05 666c 6f61 7429 09da  tr1.....float)..
-00000e90: 0269 64da 0974 6162 6c65 4e61 6d65 da04  .id..tableName..
-00000ea0: 5041 5448 da0a 636f 6e6e 6563 7469 6f6e  PATH..connection
-00000eb0: 7241 0000 00da 0672 6573 756c 74da 0464  rA.....result..d
-00000ec0: 6174 61da 046c 6973 74da 036e 756d 7209  ata..list..numr.
-00000ed0: 0000 0072 0900 0000 720a 0000 00da 0d66  ...r....r......f
-00000ee0: 726f 6d53 514c 746f 4c69 7374 5500 0000  romSQLtoListU...
-00000ef0: 7320 0000 0004 010a 0208 0108 0210 0108  s ..............
-00000f00: 010e 0102 0214 010c 0106 0108 0104 0208  ................
-00000f10: 0110 0104 0272 4e00 0000 da0a 696e 7075  .....rN.....inpu
-00000f20: 7442 6f61 7264 da09 696e 7075 7454 7572  tBoard..inputTur
-00000f30: 6e63 0300 0000 0000 0000 0000 0000 0e00  nc..............
-00000f40: 0000 0500 0000 4300 0000 73d0 0000 007c  ......C...s....|
-00000f50: 0264 0164 0285 0219 0064 036b 0272 0b64  .d.d.....d.k.r.d
-00000f60: 047d 036e 117c 0264 0164 0285 0219 0064  .}.n.|.d.d.....d
-00000f70: 056b 0272 1664 067d 036e 0674 0064 0783  .k.r.d.}.n.t.d..
-00000f80: 0101 0067 0053 0074 017c 0264 0264 0085  ...g.S.t.|.d.d..
-00000f90: 0219 007c 0383 027d 0474 027c 0483 017d  ...|...}.t.|...}
-00000fa0: 057c 00a0 037c 016a 047c 016a 05a1 027d  .|...|.j.|.j...}
-00000fb0: 0667 007d 077c 0644 005d 1b7d 0874 06a0  .g.}.|.D.].}.t..
-00000fc0: 077c 00a1 017d 097c 09a0 087c 087c 016a  .|...}.|...|.|.j
-00000fd0: 04a1 0201 007c 05a0 097c 096a 0a7c 016a  .....|...|.j.|.j
-00000fe0: 04a1 027d 0a7c 07a0 0b7c 0aa1 0101 0071  ...}.|...|.....q
-00000ff0: 3574 0c7c 0783 0164 086b 0272 5967 0053  5t.|...d.k.rYg.S
-00001000: 0074 0d7c 0783 017d 0b7c 07a0 0e7c 0ba1  .t.|...}.|...|..
-00001010: 017d 0c7c 067c 0c19 007d 0d7c 0d53 0029  .}.|.|...}.|.S.)
-00001020: 094e e905 0000 00e9 0900 0000 7a04 4e56  .N..........z.NV
-00001030: 312d 723d 0000 007a 044e 5654 2d72 3e00  1-r=...z.NVT-r>.
-00001040: 0000 7a26 4572 726f 723a 204e 6574 776f  ..z&Error: Netwo
-00001050: 726b 2049 6465 6e74 204e 6f74 2056 616c  rk Ident Not Val
-00001060: 6964 2028 5461 626c 6529 7201 0000 0029  id (Table)r....)
-00001070: 0fda 0570 7269 6e74 724e 0000 0072 0f00  ...printrN...r..
-00001080: 0000 da13 7265 7475 726e 4d6f 7665 5365  ....returnMoveSe
-00001090: 7175 656e 6365 7372 0600 0000 7207 0000  quencesr....r...
-000010a0: 00da 0463 6f70 79da 0864 6565 7063 6f70  ...copy..deepcop
-000010b0: 79da 096d 616b 654d 6f76 6573 7237 0000  y..makeMovesr7..
-000010c0: 0072 2800 0000 7231 0000 00da 036c 656e  .r(...r1.....len
-000010d0: da03 6d61 78da 0569 6e64 6578 290e 724f  ..max..index).rO
-000010e0: 0000 0072 5000 0000 da0c 6e65 7477 6f72  ...rP.....networ
-000010f0: 6b49 6465 6e74 7247 0000 00da 0277 625a  kIdentrG.....wbZ
-00001100: 076e 6574 776f 726b da05 6d6f 7665 735a  .network..movesZ
-00001110: 0a6d 6f76 6556 616c 7565 735a 076d 6f76  .moveValuesZ.mov
-00001120: 6553 6574 5a09 7465 7374 426f 6172 6472  eSetZ.testBoardr
-00001130: 3600 0000 5a08 6d61 7856 616c 7565 5a0b  6...Z.maxValueZ.
-00001140: 696e 6465 784f 664d 6f76 655a 1266 696e  indexOfMoveZ.fin
-00001150: 616c 4d6f 7665 5365 6c65 6374 696f 6e72  alMoveSelectionr
-00001160: 0900 0000 7209 0000 0072 0a00 0000 da08  ....r....r......
-00001170: 4675 6c6c 5f52 756e 6d00 0000 732a 0000  Full_Runm...s*..
-00001180: 0010 0206 0110 0106 0108 0204 0112 0208  ................
-00001190: 0210 0204 0208 010a 010e 0110 010c 010c  ................
-000011a0: 0204 0108 020a 0108 0104 0272 5e00 0000  ...........r^...
-000011b0: 6300 0000 0000 0000 0000 0000 0008 0000  c...............
-000011c0: 0006 0000 0043 0000 0073 d800 0000 6401  .....C...s....d.
-000011d0: 7d00 7400 a001 7c00 a101 7d01 7c01 a002  }.t...|...}.|...
-000011e0: a100 7d02 7a07 7c02 a003 6402 a101 0100  ..}.z.|...d.....
-000011f0: 5700 6e04 0100 0100 0100 5900 7c02 a003  W.n.......Y.|...
-00001200: 6403 a101 0100 7404 6404 8301 4400 5d41  d.....t.d...D.]A
-00001210: 7d03 6405 7c03 1700 6406 1b00 7d04 6700  }.d.|...d...}.g.
-00001220: 7d05 7404 6407 8301 4400 5d1c 7d03 7405  }.t.d...D.].}.t.
-00001230: 7406 a006 a100 6408 8302 7d06 7406 a007  t.....d...}.t...
-00001240: 6409 640a a102 6409 6b02 7243 640b 7c06  d.d...d.k.rCd.|.
-00001250: 1400 6e01 7c06 7d06 7c05 a008 7c06 a101  ..n.|.}.|...|...
-00001260: 0100 712e 640c a009 640d 640e 8400 7c05  ..q.d...d.d...|.
-00001270: 4400 8301 a101 7d07 7c02 a003 640f 7c04  D.....}.|...d.|.
-00001280: 7c07 6602 a102 0100 7c03 6409 1700 7d03  |.f.....|.d...}.
-00001290: 7120 7c01 a00a a100 0100 740b 6410 8301  q |.......t.d...
-000012a0: 0100 6400 5300 2911 4e7a 3677 696c 6c73  ..d.S.).Nz6wills
-000012b0: 655f 6261 636b 6761 6d6d 6f6e 5c41 495f  e_backgammon\AI_
-000012c0: 4167 656e 7473 5c4e 6574 776f 726b 5f54  Agents\Network_T
-000012d0: 7970 6531 5f44 6174 612e 7371 6c69 7465  ype1_Data.sqlite
-000012e0: 337a 1b44 524f 5020 5441 424c 4520 4e65  3z.DROP TABLE Ne
-000012f0: 7477 6f72 6b5f 5661 6c75 6573 5f31 7a32  twork_Values_1z2
-00001300: 4352 4541 5445 2054 4142 4c45 204e 6574  CREATE TABLE Net
-00001310: 776f 726b 5f56 616c 7565 735f 3120 2869  work_Values_1 (i
-00001320: 6420 5245 414c 2c20 6461 7461 2054 4558  d REAL, data TEX
-00001330: 5429 e940 0000 00e9 6500 0000 e964 0000  T).@....e....d..
-00001340: 0069 e107 0000 e903 0000 0072 1200 0000  .i.........r....
-00001350: 7224 0000 0072 2b00 0000 fa01 2063 0100  r$...r+..... c..
-00001360: 0000 0000 0000 0000 0000 0200 0000 0300  ................
-00001370: 0000 7300 0000 7318 0000 0081 007c 005d  ..s...s......|.]
-00001380: 077d 0174 007c 0183 0156 0001 0071 0264  .}.t.|...V...q.d
-00001390: 0053 0072 0500 0000 2901 7243 0000 0029  .S.r....).rC...)
-000013a0: 0272 2500 0000 724d 0000 0072 0900 0000  .r%...rM...r....
-000013b0: 7209 0000 0072 0a00 0000 da09 3c67 656e  r....r......<gen
-000013c0: 6578 7072 3ea3 0000 0073 0400 0000 0280  expr>....s......
-000013d0: 1600 7a24 496e 6974 6961 6c69 7a65 4461  ..z$InitializeDa
-000013e0: 7461 5365 742e 3c6c 6f63 616c 733e 2e3c  taSet.<locals>.<
-000013f0: 6765 6e65 7870 723e 7a2a 494e 5345 5254  genexpr>z*INSERT
-00001400: 2049 4e54 4f20 4e65 7477 6f72 6b5f 5661   INTO Network_Va
-00001410: 6c75 6573 5f31 2056 414c 5545 5320 283f  lues_1 VALUES (?
-00001420: 2c20 3f29 7a14 4461 7461 2053 6574 2049  , ?)z.Data Set I
-00001430: 6e69 7469 616c 697a 6564 290c 723f 0000  nitialized).r?..
-00001440: 0072 4000 0000 7241 0000 0072 4200 0000  .r@...rA...rB...
-00001450: 7230 0000 00da 0572 6f75 6e64 da06 7261  r0.....round..ra
-00001460: 6e64 6f6d da07 7261 6e64 696e 7472 3100  ndom..randintr1.
-00001470: 0000 da04 6a6f 696e 5a06 636f 6d6d 6974  ....joinZ.commit
-00001480: 7253 0000 0029 0872 4800 0000 7249 0000  rS...).rH...rI..
-00001490: 0072 4100 0000 7226 0000 0072 4600 0000  .rA...r&...rF...
-000014a0: 5a08 6461 7461 5365 7431 724d 0000 00da  Z.dataSet1rM....
-000014b0: 0676 616c 7565 7372 0900 0000 7209 0000  .valuesr....r...
-000014c0: 0072 0a00 0000 da11 496e 6974 6961 6c69  .r......Initiali
-000014d0: 7a65 4461 7461 5365 7490 0000 0073 2800  zeDataSet....s(.
-000014e0: 0000 0401 0a02 0801 0202 0e01 0601 0201  ................
-000014f0: 0a01 0c02 0c01 0401 0c01 0e01 1c01 0c01  ................
-00001500: 1401 1002 0a02 0802 0c01 726a 0000 0029  ..........rj...)
-00001510: 0d72 5500 0000 7266 0000 0072 3f00 0000  .rU...rf...r?...
-00001520: da05 6e75 6d70 7972 1300 0000 da10 4d61  ..numpyr......Ma
-00001530: 696e 5f46 696c 6573 2e4c 6f67 6963 7202  in_Files.Logicr.
-00001540: 0000 00da 2277 696c 6c73 655f 6261 636b  ...."willse_back
-00001550: 6761 6d6d 6f6e 2e4d 6169 6e5f 4669 6c65  gammon.Main_File
-00001560: 732e 4c6f 6769 6372 0300 0000 720f 0000  s.Logicr....r...
-00001570: 0072 4e00 0000 725e 0000 0072 6a00 0000  .rN...r^...rj...
-00001580: 7209 0000 0072 0900 0000 7209 0000 0072  r....r....r....r
-00001590: 0a00 0000 da08 3c6d 6f64 756c 653e 0100  ......<module>..
-000015a0: 0000 731a 0000 0008 0008 0108 0108 0102  ..s.............
-000015b0: 0210 0106 010e 010e 020e 0608 4412 180c  ............D...
-000015c0: 23                                       #
+00000bc0: 325f 6572 726f 725a 1368 6964 6465 6e5f  2_errorZ.hidden_
+00000bd0: 6c61 7965 7232 5f64 656c 7461 5a13 6869  layer2_deltaZ.hi
+00000be0: 6464 656e 5f6c 6179 6572 315f 6572 726f  dden_layer1_erro
+00000bf0: 725a 1368 6964 6465 6e5f 6c61 7965 7231  rZ.hidden_layer1
+00000c00: 5f64 656c 7461 7209 0000 0072 0900 0000  _deltar....r....
+00000c10: 720a 0000 00da 0f62 6163 6b70 726f 7061  r......backpropa
+00000c20: 6761 7469 6f6e 3c00 0000 731e 0000 001a  gation<...s.....
+00000c30: 021a 011a 0108 030e 0110 020e 0110 020e  ................
+00000c40: 011c 031c 011c 021c 011c 0220 017a 2742  ........... .z'B
+00000c50: 6163 6b67 616d 6d6f 6e4e 6575 7261 6c4e  ackgammonNeuralN
+00000c60: 6574 776f 726b 2e62 6163 6b70 726f 7061  etwork.backpropa
+00000c70: 6761 7469 6f6e 4e29 0a72 0c00 0000 720d  gationN).r....r.
+00000c80: 0000 0072 0e00 0000 720b 0000 0072 1f00  ...r....r....r..
+00000c90: 0000 7221 0000 0072 2300 0000 7224 0000  ..r!...r#...r$..
+00000ca0: 0072 3800 0000 723d 0000 0072 0900 0000  .r8...r=...r....
+00000cb0: 7209 0000 0072 0900 0000 720a 0000 0072  r....r....r....r
+00000cc0: 0f00 0000 1300 0000 7310 0000 0008 0008  ........s.......
+00000cd0: 0108 0908 0308 0308 0308 030c 1372 0f00  .............r..
+00000ce0: 0000 6302 0000 0000 0000 0000 0000 0009  ..c.............
+00000cf0: 0000 0006 0000 0043 0000 0073 9400 0000  .......C...s....
+00000d00: 6401 7d02 7400 a001 7c02 a101 7d03 7c03  d.}.t...|...}.|.
+00000d10: a002 a100 7d04 7c01 6402 6b02 7217 7c04  ....}.|.d.k.r.|.
+00000d20: a003 6403 7c00 6601 a102 7d05 6e0b 7c01  ..d.|.f...}.n.|.
+00000d30: 6404 6b02 7222 7c04 a003 6405 7c00 6601  d.k.r"|...d.|.f.
+00000d40: a102 7d05 7a10 7404 7c05 a005 a100 6406  ..}.z.t.|.....d.
+00000d50: 1900 6406 1900 8301 7d06 7c06 a006 a100  ..d.....}.|.....
+00000d60: 7d06 5700 6e07 0100 0100 0100 6700 0600  }.W.n.......g...
+00000d70: 5900 5300 6700 7d07 7c06 4400 5d09 7d08  Y.S.g.}.|.D.].}.
+00000d80: 7c07 a007 7408 7c08 8301 a101 0100 713e  |...t.|.......q>
+00000d90: 7c07 5300 2907 4e7a 3b77 696c 6c73 655f  |.S.).Nz;willse_
+00000da0: 6261 636b 6761 6d6d 6f6e 2f41 495f 4167  backgammon/AI_Ag
+00000db0: 656e 7473 2f44 6174 615f 5365 7473 2f4e  ents/Data_Sets/N
+00000dc0: 6574 776f 726b 5f54 7970 6531 5f44 6174  etwork_Type1_Dat
+00000dd0: 612e 6462 da10 4e65 7477 6f72 6b5f 5661  a.db..Network_Va
+00000de0: 6c75 6573 5f31 7a2e 5345 4c45 4354 2064  lues_1z.SELECT d
+00000df0: 6174 6120 4652 4f4d 204e 6574 776f 726b  ata FROM Network
+00000e00: 5f56 616c 7565 735f 3120 5748 4552 4520  _Values_1 WHERE 
+00000e10: 6964 203d 203f da19 4e65 7477 6f72 6b5f  id = ?..Network_
+00000e20: 5661 6c75 6573 5f54 6f75 726e 616d 656e  Values_Tournamen
+00000e30: 747a 3753 454c 4543 5420 6461 7461 2046  tz7SELECT data F
+00000e40: 524f 4d20 4e65 7477 6f72 6b5f 5661 6c75  ROM Network_Valu
+00000e50: 6573 5f54 6f75 726e 616d 656e 7420 5748  es_Tournament WH
+00000e60: 4552 4520 6964 203d 203f 7201 0000 0029  ERE id = ?r....)
+00000e70: 09da 0773 716c 6974 6533 da07 636f 6e6e  ...sqlite3..conn
+00000e80: 6563 74da 0663 7572 736f 72da 0765 7865  ect..cursor..exe
+00000e90: 6375 7465 da03 7374 72da 0866 6574 6368  cute..str..fetch
+00000ea0: 616c 6cda 0672 7370 6c69 7472 3200 0000  all..rsplitr2...
+00000eb0: da05 666c 6f61 7429 09da 0269 64da 0974  ..float)...id..t
+00000ec0: 6162 6c65 4e61 6d65 da04 5041 5448 da0a  ableName..PATH..
+00000ed0: 636f 6e6e 6563 7469 6f6e 7242 0000 00da  connectionrB....
+00000ee0: 0672 6573 756c 74da 0464 6174 61da 046c  .result..data..l
+00000ef0: 6973 74da 036e 756d 7209 0000 0072 0900  ist..numr....r..
+00000f00: 0000 720a 0000 00da 0d66 726f 6d53 514c  ..r......fromSQL
+00000f10: 746f 4c69 7374 5700 0000 7320 0000 0004  toListW...s ....
+00000f20: 010a 0208 0108 0210 0108 010e 0102 0214  ................
+00000f30: 010c 0106 0108 0104 0208 0110 0104 0272  ...............r
+00000f40: 5000 0000 da0a 696e 7075 7442 6f61 7264  P.....inputBoard
+00000f50: da09 696e 7075 7454 7572 6e63 0300 0000  ..inputTurnc....
+00000f60: 0000 0000 0000 0000 0e00 0000 0500 0000  ................
+00000f70: 4300 0000 73d0 0000 007c 0264 0164 0285  C...s....|.d.d..
+00000f80: 0219 0064 036b 0272 0b64 047d 036e 117c  ...d.k.r.d.}.n.|
+00000f90: 0264 0164 0285 0219 0064 056b 0272 1664  .d.d.....d.k.r.d
+00000fa0: 067d 036e 0674 0064 0783 0101 0067 0053  .}.n.t.d.....g.S
+00000fb0: 0074 017c 0264 0264 0085 0219 007c 0383  .t.|.d.d.....|..
+00000fc0: 027d 0474 027c 0483 017d 057c 00a0 037c  .}.t.|...}.|...|
+00000fd0: 016a 047c 016a 05a1 027d 0667 007d 077c  .j.|.j...}.g.}.|
+00000fe0: 0644 005d 1b7d 0874 06a0 077c 00a1 017d  .D.].}.t...|...}
+00000ff0: 097c 09a0 087c 087c 016a 04a1 0201 007c  .|...|.|.j.....|
+00001000: 05a0 097c 096a 0a7c 016a 04a1 027d 0a7c  ...|.j.|.j...}.|
+00001010: 07a0 0b7c 0aa1 0101 0071 3574 0c7c 0783  ...|.....q5t.|..
+00001020: 0164 086b 0272 5967 0053 0074 0d7c 0783  .d.k.rYg.S.t.|..
+00001030: 017d 0b7c 07a0 0e7c 0ba1 017d 0c7c 067c  .}.|...|...}.|.|
+00001040: 0c19 007d 0d7c 0d53 0029 094e e905 0000  ...}.|.S.).N....
+00001050: 00e9 0900 0000 7a04 4e56 312d 723e 0000  ......z.NV1-r>..
+00001060: 007a 044e 5654 2d72 3f00 0000 7a26 4572  .z.NVT-r?...z&Er
+00001070: 726f 723a 204e 6574 776f 726b 2049 6465  ror: Network Ide
+00001080: 6e74 204e 6f74 2056 616c 6964 2028 5461  nt Not Valid (Ta
+00001090: 626c 6529 7201 0000 0029 0fda 0570 7269  ble)r....)...pri
+000010a0: 6e74 7250 0000 0072 0f00 0000 5a13 7265  ntrP...r....Z.re
+000010b0: 7475 726e 4d6f 7665 5365 7175 656e 6365  turnMoveSequence
+000010c0: 7372 0600 0000 7207 0000 00da 0463 6f70  sr....r......cop
+000010d0: 79da 0864 6565 7063 6f70 79da 096d 616b  y..deepcopy..mak
+000010e0: 654d 6f76 6573 7238 0000 0072 2900 0000  eMovesr8...r)...
+000010f0: 7232 0000 00da 036c 656e da03 6d61 78da  r2.....len..max.
+00001100: 0569 6e64 6578 290e 7251 0000 0072 5200  .index).rQ...rR.
+00001110: 0000 da0c 6e65 7477 6f72 6b49 6465 6e74  ....networkIdent
+00001120: 7249 0000 00da 0277 62da 076e 6574 776f  rI.....wb..netwo
+00001130: 726b da05 6d6f 7665 735a 0a6d 6f76 6556  rk..movesZ.moveV
+00001140: 616c 7565 735a 076d 6f76 6553 6574 5a09  aluesZ.moveSetZ.
+00001150: 7465 7374 426f 6172 6472 3700 0000 5a08  testBoardr7...Z.
+00001160: 6d61 7856 616c 7565 5a0b 696e 6465 784f  maxValueZ.indexO
+00001170: 664d 6f76 655a 1266 696e 616c 4d6f 7665  fMoveZ.finalMove
+00001180: 5365 6c65 6374 696f 6e72 0900 0000 7209  Selectionr....r.
+00001190: 0000 0072 0a00 0000 da08 4675 6c6c 5f52  ...r......Full_R
+000011a0: 756e 6f00 0000 732a 0000 0010 0206 0110  uno...s*........
+000011b0: 0106 0108 0204 0112 0208 0210 0204 0208  ................
+000011c0: 010a 010e 0110 010c 010c 0204 0108 020a  ................
+000011d0: 0108 0104 0272 6000 0000 6300 0000 0000  .....r`...c.....
+000011e0: 0000 0000 0000 0008 0000 0006 0000 0043  ...............C
+000011f0: 0000 0073 d800 0000 6401 7d00 7400 a001  ...s....d.}.t...
+00001200: 7c00 a101 7d01 7c01 a002 a100 7d02 7a07  |...}.|.....}.z.
+00001210: 7c02 a003 6402 a101 0100 5700 6e04 0100  |...d.....W.n...
+00001220: 0100 0100 5900 7c02 a003 6403 a101 0100  ....Y.|...d.....
+00001230: 7404 6404 8301 4400 5d41 7d03 6405 7c03  t.d...D.]A}.d.|.
+00001240: 1700 6406 1b00 7d04 6700 7d05 7404 6407  ..d...}.g.}.t.d.
+00001250: 8301 4400 5d1c 7d03 7405 7406 a006 a100  ..D.].}.t.t.....
+00001260: 6408 8302 7d06 7406 a007 6409 640a a102  d...}.t...d.d...
+00001270: 6409 6b02 7243 640b 7c06 1400 6e01 7c06  d.k.rCd.|...n.|.
+00001280: 7d06 7c05 a008 7c06 a101 0100 712e 640c  }.|...|.....q.d.
+00001290: a009 640d 640e 8400 7c05 4400 8301 a101  ..d.d...|.D.....
+000012a0: 7d07 7c02 a003 640f 7c04 7c07 6602 a102  }.|...d.|.|.f...
+000012b0: 0100 7c03 6409 1700 7d03 7120 7c01 a00a  ..|.d...}.q |...
+000012c0: a100 0100 740b 6410 8301 0100 6400 5300  ....t.d.....d.S.
+000012d0: 2911 4e7a 3677 696c 6c73 655f 6261 636b  ).Nz6willse_back
+000012e0: 6761 6d6d 6f6e 5c41 495f 4167 656e 7473  gammon\AI_Agents
+000012f0: 5c4e 6574 776f 726b 5f54 7970 6531 5f44  \Network_Type1_D
+00001300: 6174 612e 7371 6c69 7465 337a 1b44 524f  ata.sqlite3z.DRO
+00001310: 5020 5441 424c 4520 4e65 7477 6f72 6b5f  P TABLE Network_
+00001320: 5661 6c75 6573 5f31 7a32 4352 4541 5445  Values_1z2CREATE
+00001330: 2054 4142 4c45 204e 6574 776f 726b 5f56   TABLE Network_V
+00001340: 616c 7565 735f 3120 2869 6420 5245 414c  alues_1 (id REAL
+00001350: 2c20 6461 7461 2054 4558 5429 e940 0000  , data TEXT).@..
+00001360: 00e9 6500 0000 e964 0000 0069 e107 0000  ..e....d...i....
+00001370: e903 0000 0072 1200 0000 7225 0000 0072  .....r....r%...r
+00001380: 2c00 0000 fa01 2063 0100 0000 0000 0000  ,..... c........
+00001390: 0000 0000 0200 0000 0300 0000 7300 0000  ............s...
+000013a0: 7318 0000 0081 007c 005d 077d 0174 007c  s......|.].}.t.|
+000013b0: 0183 0156 0001 0071 0264 0053 0072 0500  ...V...q.d.S.r..
+000013c0: 0000 2901 7244 0000 0029 0272 2600 0000  ..).rD...).r&...
+000013d0: 724f 0000 0072 0900 0000 7209 0000 0072  rO...r....r....r
+000013e0: 0a00 0000 da09 3c67 656e 6578 7072 3ea5  ......<genexpr>.
+000013f0: 0000 0073 0400 0000 0280 1600 7a24 496e  ...s........z$In
+00001400: 6974 6961 6c69 7a65 4461 7461 5365 742e  itializeDataSet.
+00001410: 3c6c 6f63 616c 733e 2e3c 6765 6e65 7870  <locals>.<genexp
+00001420: 723e 7a2a 494e 5345 5254 2049 4e54 4f20  r>z*INSERT INTO 
+00001430: 4e65 7477 6f72 6b5f 5661 6c75 6573 5f31  Network_Values_1
+00001440: 2056 414c 5545 5320 283f 2c20 3f29 7a14   VALUES (?, ?)z.
+00001450: 4461 7461 2053 6574 2049 6e69 7469 616c  Data Set Initial
+00001460: 697a 6564 290c 7240 0000 0072 4100 0000  ized).r@...rA...
+00001470: 7242 0000 0072 4300 0000 7231 0000 00da  rB...rC...r1....
+00001480: 0572 6f75 6e64 da06 7261 6e64 6f6d da07  .round..random..
+00001490: 7261 6e64 696e 7472 3200 0000 da04 6a6f  randintr2.....jo
+000014a0: 696e da06 636f 6d6d 6974 7255 0000 0029  in..commitrU...)
+000014b0: 0872 4a00 0000 724b 0000 0072 4200 0000  .rJ...rK...rB...
+000014c0: 7227 0000 0072 4800 0000 da08 6461 7461  r'...rH.....data
+000014d0: 5365 7431 724f 0000 00da 0676 616c 7565  Set1rO.....value
+000014e0: 7372 0900 0000 7209 0000 0072 0a00 0000  sr....r....r....
+000014f0: da11 496e 6974 6961 6c69 7a65 4461 7461  ..InitializeData
+00001500: 5365 7492 0000 0073 2800 0000 0401 0a02  Set....s(.......
+00001510: 0801 0202 0e01 0601 0201 0a01 0c02 0c01  ................
+00001520: 0401 0c01 0e01 1c01 0c01 1401 1002 0a02  ................
+00001530: 0802 0c01 726e 0000 0029 1472 5600 0000  ....rn...).rV...
+00001540: 7268 0000 0072 4000 0000 da07 7061 7468  rh...r@.....path
+00001550: 6c69 62da 026f 73da 056e 756d 7079 7213  lib..os..numpyr.
+00001560: 0000 00da 104d 6169 6e5f 4669 6c65 732e  .....Main_Files.
+00001570: 4c6f 6769 6372 0200 0000 da22 7769 6c6c  Logicr....."will
+00001580: 7365 5f62 6163 6b67 616d 6d6f 6e2e 4d61  se_backgammon.Ma
+00001590: 696e 5f46 696c 6573 2e4c 6f67 6963 da04  in_Files.Logic..
+000015a0: 5061 7468 da08 5f5f 6669 6c65 5f5f da06  Path..__file__..
+000015b0: 7061 7265 6e74 724a 0000 00da 0563 6864  parentrJ.....chd
+000015c0: 6972 7203 0000 0072 0f00 0000 7250 0000  irr....r....rP..
+000015d0: 0072 6000 0000 726e 0000 0072 0900 0000  .r`...rn...r....
+000015e0: 7209 0000 0072 0900 0000 720a 0000 00da  r....r....r.....
+000015f0: 083c 6d6f 6475 6c65 3e01 0000 0073 1a00  .<module>....s..
+00001600: 0000 2800 0801 0202 1001 0601 0e01 1003  ..(.............
+00001610: 0a01 0e02 0e06 0844 1218 0c23            .......D...#
```

### Comparing `willse_backgammon-0.0.1/src/willse_backgammon/AI_Agents/__pycache__/Pick_Best_Pip.cpython-310.pyc` & `willse_backgammon-0.0.2/src/willse_backgammon/AI_Agents/__pycache__/Pick_Best_Pip.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `willse_backgammon-0.0.1/src/willse_backgammon/AI_Agents/__pycache__/TreeSearchI.cpython-310.pyc` & `willse_backgammon-0.0.2/src/willse_backgammon/AI_Agents/__pycache__/TreeSearchI.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Sat Mar 23 17:16:28 2024 UTC, .py size: 6249 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 6c0e ff65 6918 0000  o.......l..ei...
+00000000: 6f0d 0d0a 0000 0000 65e6 0166 6918 0000  o.......e..fi...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0008 0000 0040 0000 0073 cc00 0000 6400  .....@...s....d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a01 7a0a  d.l.Z.d.d.l.Z.z.
 00000040: 6400 6402 6c02 6d03 5a03 6d04 5a04 0100  d.d.l.m.Z.m.Z...
 00000050: 5700 6e11 0400 6505 7923 0100 0100 0100  W.n...e.y#......
 00000060: 6400 6402 6c06 6d03 5a03 6d04 5a04 0100  d.d.l.m.Z.m.Z...
 00000070: 5900 6e01 7700 6700 6403 a201 5a07 6404  Y.n.w.g.d...Z.d.
@@ -226,15 +226,15 @@
 00000e10: 9077 0101 0001 0001 0059 0001 0074 047c  .w.......Y...t.|
 00000e20: 0483 0164 056b 0372 c488 006a 0164 046b  ...d.k.r...j.d.k
 00000e30: 0272 ae74 157c 0483 017d 0d7c 04a0 167c  .r.t.|...}.|...|
 00000e40: 0da1 017d 0e7c 037c 0e19 006a 0853 007c  ...}.|.|...j.S.|
 00000e50: 04a0 17a1 0001 007c 03a0 17a1 0001 0074  .......|.......t
 00000e60: 157c 0483 017d 0d7c 04a0 167c 0da1 017d  .|...}.|...|...}
 00000e70: 0e7c 037c 0e19 006a 0853 0067 0053 0029  .|.|...j.S.g.S.)
-00000e80: 0a4e e920 0000 0054 7205 0000 0072 0400  .N. ...Tr....r..
+00000e80: 0a4e e930 0000 0054 7205 0000 0072 0400  .N.0...Tr....r..
 00000e90: 0000 7201 0000 007a 2d49 6e69 7469 6174  ..r....z-Initiat
 00000ea0: 696e 6720 4d75 6c74 6970 726f 6365 7373  ing Multiprocess
 00000eb0: 696e 6720 666f 7220 5453 3120 7461 736b  ing for TS1 task
 00000ec0: 2077 6974 6820 7a11 2074 7572 6e20 656e   with z. turn en
 00000ed0: 6420 7374 6174 6573 2e63 0100 0000 0000  d states.c......
 00000ee0: 0000 0000 0000 0200 0000 0400 0000 1300  ................
 00000ef0: 0000 7316 0000 0067 007c 005d 077d 017c  ..s....g.|.].}.|
```

### Comparing `willse_backgammon-0.0.1/src/willse_backgammon/Images/Move.png` & `willse_backgammon-0.0.2/src/willse_backgammon/Images/Move.png`

 * *Files identical despite different names*

### Comparing `willse_backgammon-0.0.1/src/willse_backgammon/Images/Submove.png` & `willse_backgammon-0.0.2/src/willse_backgammon/Images/Submove.png`

 * *Files identical despite different names*

### Comparing `willse_backgammon-0.0.1/src/willse_backgammon/Images/darkPiece.png` & `willse_backgammon-0.0.2/src/willse_backgammon/Images/darkPiece.png`

 * *Files identical despite different names*

### Comparing `willse_backgammon-0.0.1/src/willse_backgammon/Images/darkPiece2.png` & `willse_backgammon-0.0.2/src/willse_backgammon/Images/darkPiece2.png`

 * *Files identical despite different names*

### Comparing `willse_backgammon-0.0.1/src/willse_backgammon/Images/darkPiece3.png` & `willse_backgammon-0.0.2/src/willse_backgammon/Images/darkPiece3.png`

 * *Files identical despite different names*

### Comparing `willse_backgammon-0.0.1/src/willse_backgammon/Images/delete_icon.png` & `willse_backgammon-0.0.2/src/willse_backgammon/Images/delete_icon.png`

 * *Files identical despite different names*

### Comparing `willse_backgammon-0.0.1/src/willse_backgammon/Images/delete_icon2.png` & `willse_backgammon-0.0.2/src/willse_backgammon/Images/delete_icon2.png`

 * *Files identical despite different names*

### Comparing `willse_backgammon-0.0.1/src/willse_backgammon/Images/delete_icon3.png` & `willse_backgammon-0.0.2/src/willse_backgammon/Images/delete_icon3.png`

 * *Files identical despite different names*

### Comparing `willse_backgammon-0.0.1/src/willse_backgammon/Images/exit_icon.png` & `willse_backgammon-0.0.2/src/willse_backgammon/Images/exit_icon.png`

 * *Files identical despite different names*

### Comparing `willse_backgammon-0.0.1/src/willse_backgammon/Images/gear_icon.png` & `willse_backgammon-0.0.2/src/willse_backgammon/Images/gear_icon.png`

 * *Files identical despite different names*

### Comparing `willse_backgammon-0.0.1/src/willse_backgammon/Images/lightPiece.png` & `willse_backgammon-0.0.2/src/willse_backgammon/Images/lightPiece.png`

 * *Files identical despite different names*

### Comparing `willse_backgammon-0.0.1/src/willse_backgammon/Images/lightPiece2.png` & `willse_backgammon-0.0.2/src/willse_backgammon/Images/lightPiece2.png`

 * *Files identical despite different names*

### Comparing `willse_backgammon-0.0.1/src/willse_backgammon/Images/lightPiece3.png` & `willse_backgammon-0.0.2/src/willse_backgammon/Images/lightPiece3.png`

 * *Files identical despite different names*

### Comparing `willse_backgammon-0.0.1/src/willse_backgammon/Images/quit_icon.png` & `willse_backgammon-0.0.2/src/willse_backgammon/Images/quit_icon.png`

 * *Files identical despite different names*

### Comparing `willse_backgammon-0.0.1/src/willse_backgammon/Images/restart_icon.png` & `willse_backgammon-0.0.2/src/willse_backgammon/Images/restart_icon.png`

 * *Files identical despite different names*

### Comparing `willse_backgammon-0.0.1/src/willse_backgammon/Images/restart_icon2.png` & `willse_backgammon-0.0.2/src/willse_backgammon/Images/restart_icon2.png`

 * *Files identical despite different names*

### Comparing `willse_backgammon-0.0.1/src/willse_backgammon/Images/restart_icon3.png` & `willse_backgammon-0.0.2/src/willse_backgammon/Images/restart_icon3.png`

 * *Files identical despite different names*

### Comparing `willse_backgammon-0.0.1/src/willse_backgammon/Main.py` & `willse_backgammon-0.0.2/src/willse_backgammon/Main.py`

 * *Files identical despite different names*

### Comparing `willse_backgammon-0.0.1/src/willse_backgammon/Main_Files/AI.py` & `willse_backgammon-0.0.2/src/willse_backgammon/Main_Files/AI.py`

 * *Files identical despite different names*

### Comparing `willse_backgammon-0.0.1/src/willse_backgammon/Main_Files/Graphics.py` & `willse_backgammon-0.0.2/src/willse_backgammon/Main_Files/Graphics.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,32 +6,32 @@
 import arcade
 import arcade.gui
 
 PATH = pathlib.Path(__file__).parent.parent.parent
 os.chdir(PATH)
 
 # Load images & sounds:
-gear_icon = arcade.load_texture("willse_backgammon\Images\gear_icon.png")
-exit_icon = arcade.load_texture("willse_backgammon\Images\exit_icon.png")
-quit_icon = arcade.load_texture("willse_backgammon\Images\quit_icon.png")
-
-delete_icon = arcade.load_texture("willse_backgammon\Images\delete_icon.png")
-darkPiece_icon = arcade.load_texture("willse_backgammon\Images\darkPiece.png")
-lightPiece_icon = arcade.load_texture("willse_backgammon\Images\lightPiece.png")
-restart_icon = arcade.load_texture("willse_backgammon\Images\\restart_icon.png")
-
-delete_icon2 = arcade.load_texture("willse_backgammon\Images\delete_icon2.png")
-darkPiece_icon2 = arcade.load_texture("willse_backgammon\Images\darkPiece2.png")
-lightPiece_icon2 = arcade.load_texture("willse_backgammon\Images\lightPiece2.png")
-restart_icon2 = arcade.load_texture("willse_backgammon\Images\\restart_icon2.png")
-
-delete_icon3 = arcade.load_texture("willse_backgammon\Images\delete_icon3.png")
-darkPiece_icon3 = arcade.load_texture("willse_backgammon\Images\darkPiece3.png")
-lightPiece_icon3 = arcade.load_texture("willse_backgammon\Images\lightPiece3.png")
-restart_icon3 = arcade.load_texture("willse_backgammon\Images\\restart_icon3.png")
+gear_icon = arcade.load_texture("willse_backgammon/Images/gear_icon.png")
+exit_icon = arcade.load_texture("willse_backgammon/Images/exit_icon.png")
+quit_icon = arcade.load_texture("willse_backgammon/Images/quit_icon.png")
+
+delete_icon = arcade.load_texture("willse_backgammon/Images/delete_icon.png")
+darkPiece_icon = arcade.load_texture("willse_backgammon/Images/darkPiece.png")
+lightPiece_icon = arcade.load_texture("willse_backgammon/Images/lightPiece.png")
+restart_icon = arcade.load_texture("willse_backgammon/Images/restart_icon.png")
+
+delete_icon2 = arcade.load_texture("willse_backgammon/Images/delete_icon2.png")
+darkPiece_icon2 = arcade.load_texture("willse_backgammon/Images/darkPiece2.png")
+lightPiece_icon2 = arcade.load_texture("willse_backgammon/Images/lightPiece2.png")
+restart_icon2 = arcade.load_texture("willse_backgammon/Images/restart_icon2.png")
+
+delete_icon3 = arcade.load_texture("willse_backgammon/Images/delete_icon3.png")
+darkPiece_icon3 = arcade.load_texture("willse_backgammon/Images/darkPiece3.png")
+lightPiece_icon3 = arcade.load_texture("willse_backgammon/Images/lightPiece3.png")
+restart_icon3 = arcade.load_texture("willse_backgammon/Images/restart_icon3.png")
 
 # Data:
 Master_Location_Dict = {1: (247, 755), 2: (307, 755), 3: (367, 755), 4: (427, 755), 5: (487, 755), 6: (547, 755),
                         7: (655, 755), 8: (715, 755), 9: (775, 755), 10: (835, 755), 11: (895, 755), 12: (955, 755),
                         13: (955, 47), 14: (895, 47), 15: (835, 47), 16: (775, 47), 17: (715, 47), 18: (655, 47),
                         19: (547, 47), 20: (487, 47), 21: (427, 47), 22: (367, 47), 23: (307, 47), 24: (247, 47)}
```

### Comparing `willse_backgammon-0.0.1/src/willse_backgammon/Main_Files/Logic.py` & `willse_backgammon-0.0.2/src/willse_backgammon/Main_Files/Logic.py`

 * *Files 2% similar despite different names*

```diff
@@ -99,16 +99,15 @@
                 p2_pip += (i + 1) * self.positions[i]
             elif self.positions[i] < 0:
                 p1_pip += (24 - i) * abs(self.positions[i])
         p1_pip += 25 * self.positions[24]
         p2_pip += 25 * self.positions[25]
         return (p1_pip, p2_pip)
 
-    def makeMove(self, move, player,
-                 fromMakeMoves=False):  # Updates the board with an inputted move: (start point,end point) // also updates pip, lastPoint, and BearOff
+    def makeMove(self, move, player, fromMakeMoves=False):  # Updates the board with an inputted move: (start point,end point) // also updates pip, lastPoint, and BearOff
         if move[0] == 1001:
             endPointIndex = move[1] - 1
             self.positions[23 + player] -= 1
             if player == 1:
                 if self.positions[endPointIndex] > 0:
                     self.positions[endPointIndex] = -1
                     self.positions[25] += 1
@@ -147,16 +146,15 @@
                 else:
                     self.positions[endPointIndex] += 1
         if fromMakeMoves == False:
             self.updatePip()
             self.updateLastOccupiedPoint(player)
             self.updateBearOffStatus()
 
-    def makeMoves(self, moves, player,
-                  updateLineData=False):  # Updates the board with a series of moves: ((move1),(move2),ect.) // also updates pip, lastPoint, and BearOff
+    def makeMoves(self, moves, player, updateLineData=False):  # Updates the board with a series of moves: ((move1),(move2),ect.) // also updates pip, lastPoint, and BearOff
         MoveLineData = []
         if len(moves) > 0 and type(moves[0]) == int:
             self.makeMove(moves, player, True)
             if updateLineData == True:
                 self.MoveLineData = GenerateMoveLineDataFast(moves, self)
         else:
             for move in moves:
@@ -177,19 +175,18 @@
         else:
             for index in range(23, -1, -1):
                 if self.positions[index] > 0:
                     self.lastPoints[1] = index + 1
                     break
 
     def updateBearOffStatus(self):  # Updates the self.bearOffStatus values based on current lastPoints
-        self.bearOffStatus[0] = True if (self.bearOffStatus[0]) or (self.lastPoints[0] > 18) else False
-        self.bearOffStatus[1] = True if (self.bearOffStatus[1]) or (self.lastPoints[1] < 7) else False
+        self.bearOffStatus[0] = True if (self.bearOffStatus[0]) or ((self.lastPoints[0] > 18) and (self.positions[24] == 0)) else False
+        self.bearOffStatus[1] = True if (self.bearOffStatus[1]) or ((self.lastPoints[1] < 7) and (self.positions[25] == 0)) else False
 
-    def returnMovesForDie(self, die, player,
-                          isBiggestDieOrSecondMove):  # returns all move options a die can be used for in the current board state: [(moveOption1),(moveOption2),ect.]
+    def returnMovesForDie(self, die, player, isBiggestDieOrSecondMove):  # returns all move options a die can be used for in the current board state: [(moveOption1),(moveOption2),ect.]
         moveList = []
 
         def canMoveTo(point, player):
             if point > 24 or point < 1:
                 return False
             oppValue = -1 if player == 2 else 1
             if self.positions[point - 1] == 0:
@@ -229,16 +226,15 @@
                     if self.positions[die - 1] > 0:
                         moveList.append((die, 2002))
                     if isBiggestDieOrSecondMove and self.lastPoints[1] < die:
                         moveList.append((self.lastPoints[1], 2002))
 
         return moveList
 
-    def returnMoveSequences(self, player,
-                            roll):  # for a given roll returns list of moves sequences that result in unique board States: [((move1),(move2)),((move1),(move2)), ect.]
+    def returnMoveSequences(self, player, roll):  # for a given roll returns list of moves sequences that result in unique board States: [((move1),(move2)),((move1),(move2)), ect.]
         Sequences = []
         EndBoards = []
         if roll[0] != roll[1]:
             biggerDie = roll[0] if roll[0] >= roll[1] else roll[1]
             FirstMoves = []
 
             # All Possible First Moves
@@ -331,16 +327,15 @@
 
         # Sets up unused_dice
         if self.doubles_turn == True:
             self.unused_dice = [self.roll[0]] * 4
         else:
             self.unused_dice = copy.deepcopy(self.roll)
 
-    def updatePossibleMovesHumanFormat(self,
-                                       Board: Board):  # updates self.currentPossibleMoves in Human playerType Format for use by Main Game Loop
+    def updatePossibleMovesHumanFormat(self, Board: Board):  # updates self.currentPossibleMoves in Human playerType Format for use by Main Game Loop
         # Human Format: [(startPoint,[possibleFirstEndPoint, possibleSecondEndPoint]), (1, [3, 5]), (12, [14]), (17, [19]), (19, [21, 23])]
         self.current_possible_moves = []
         if self.doubles_turn == True and len(self.unused_dice) > 0:
             self.current_possible_moves = Board.returnMovesForDie(self.roll[0], self.player, True)
             self.current_possible_moves = [(move[0], [move[1]]) for move in self.current_possible_moves]
         else:
             biggerDie = self.roll[0] if self.roll[0] > self.roll[1] else self.roll[1]
@@ -367,16 +362,15 @@
             else:
                 workingMovesList = []
                 for possibleMove in self.current_possible_moves[0]:
                     move = (possibleMove[0], [possibleMove[1]])
                     workingMovesList.append(move)
                 self.current_possible_moves = workingMovesList
 
-    def updatePossibleMovesStandardFormat(self,
-                                          Board: Board):  # updates self.currentPossibleMoves to full set of unique move sequences for use by AI programs
+    def updatePossibleMovesStandardFormat(self, Board: Board):  # updates self.currentPossibleMoves to full set of unique move sequences for use by AI programs
         self.current_possible_moves = Board.returnMoveSequences(self.player, self.roll)
 
     def formSpriteList(self, Board):  # creates and updates a sprit list for use by Main Game Loop
         # Needs Human Format for self.current_possible_moves
         self.sprites_move_start = createMoveStartSprites(self.current_possible_moves, Board, self.player)
 
 # Calculating Moves Logic
```

### Comparing `willse_backgammon-0.0.1/src/willse_backgammon/Main_Files/Views.py` & `willse_backgammon-0.0.2/src/willse_backgammon/Main_Files/Views.py`

 * *Files 9% similar despite different names*

```diff
@@ -50,15 +50,19 @@
             self.window.settings["Agent2"] = "TS 1" if self.window.settings["Agent2"] == "Human" else \
             self.window.settings["Agent2"]
             simView = MainSimView(self.backgroundColor)
             self.window.show_view(simView)
 
         @one_player_button.event("on_click")
         def on_click_OnePlayer(event):
-            pass
+            self.window.MainBoard.setStartPositions()
+            self.window.settings["Agent2"] = "TS 1" if self.window.settings["Agent2"] == "Human" else \
+            self.window.settings["Agent2"]
+            startView = Start_1P_View(self.backgroundColor)
+            self.window.show_view(startView)
 
         @two_player_button.event("on_click")
         def on_click_TwoPlayer(event):
             self.window.MainBoard.setStartPositions()
             startView = Start_2P_View(self.backgroundColor)
             self.window.show_view(startView)
 
@@ -90,15 +94,15 @@
         super().__init__()
         self.backgroundColor = backgroundColor
 
         self.manager = arcade.gui.UIManager()
         self.manager.enable()
 
         Settings_label = arcade.gui.UILabel(100, 625, 1100, 150, "Settings", font_size=30, align="center", bold=True)
-        Help_label = arcade.gui.UILabel(100, 0, 1100, 20, "*Agent 1 is used for single player games*", font_size=10, align="center", bold=True)
+        Help_label = arcade.gui.UILabel(100, 0, 1100, 20, "*Agent 2 is used for single player games*", font_size=10, align="center", bold=True)
 
         Back_button = arcade.gui.UIFlatButton(15, 745, 75, 40, "Back")
         Quit_button = arcade.gui.UIFlatButton(15, 695, 75, 40, "Quit")
 
         AIAgent1_label = arcade.gui.UILabel(165, 635, 100, 50, "Agent 1:", font_size=15, text_color=Graphics.black,
                                             bold=True)
         AIAgent2_label = arcade.gui.UILabel(165, 560, 100, 50, "Agent 2:", font_size=15, text_color=Graphics.black,
@@ -344,24 +348,20 @@
                                                              buttons=["Ok"])
                         self.manager.add(messageBox)
                     self.window.nextPlayer = 2
             else:
                 if self.window.settings["Agent2"] == "Human":
                     pass
                 else:
-                    self.window.MainTurn = Logic.Turn(player, self.window.settings["Agent2"],
-                                                      First=(self.window.nextPlayer == 0))
+                    self.window.MainTurn = Logic.Turn(player, self.window.settings["Agent2"], First=(self.window.nextPlayer == 0))
                     self.window.MainTurn.updatePossibleMovesStandardFormat(self.window.MainBoard)
-                    Moves = AI.Main(self.window.MainBoard, self.window.MainTurn, self.window.settings["Agent2"],
-                                    self.window.settings["Network2 ID"])
+                    Moves = AI.Main(self.window.MainBoard, self.window.MainTurn, self.window.settings["Agent2"], self.window.settings["Network2 ID"])
                     self.window.MainBoard.makeMoves(Moves, 2, True)
                     if self.window.MainBoard.pip[1] == 0:
-                        messageBox = arcade.gui.UIMessageBox(width=300, height=150, message_text=(
-                            "Game Over: \nPlayer 2 Wins! Please Select 'New Game' to start a new game."), callback=None,
-                                                             buttons=["Ok"])
+                        messageBox = arcade.gui.UIMessageBox(width=300, height=150, message_text=("Game Over: \nPlayer 2 Wins! Please Select 'New Game' to start a new game."), callback=None,buttons=["Ok"])
                         self.manager.add(messageBox)
                     self.window.nextPlayer = 1
 
             self.window.firstTurn = False
 
         @RunSetTurn_button.event("on_click")
         def on_click_run(event):
@@ -724,14 +724,252 @@
         arcade.draw_rectangle_filled(600, 400, 600, 50, Graphics.board_color)
         arcade.draw_rectangle_outline(600, 400, 600, 50, Graphics.board_color, 6)
 
         self.manager.draw()
 
 
 # 1P Views:
+class Start_1P_View(arcade.View):
+
+    def __init__(self, backgroundColor):
+        super().__init__()
+        self.backgroundColor = backgroundColor
+
+        self.manager = arcade.gui.UIManager()
+        self.manager.enable()
+
+        Back_button = arcade.gui.UIFlatButton(15, 745, 75, 40, "Back")
+        Quit_button = arcade.gui.UIFlatButton(15, 695, 75, 40, "Quit")
+        Roll_button = arcade.gui.UIFlatButton(400, 375, 125, 50, "Roll")
+        Settings_button = arcade.gui.UIFlatButton(700, 375, 125, 50, "Settings")
+
+        self.manager.add(Back_button)
+        self.manager.add(Quit_button)
+        self.manager.add(Roll_button)
+        self.manager.add(Settings_button)
+
+        @Back_button.event("on_click")
+        def on_click_back(event):
+            mainmenuView = MainMenuView(self.backgroundColor)
+            self.window.show_view(mainmenuView)
+
+        @Quit_button.event("on_click")
+        def on_click_Quit(event):
+            arcade.close_window()
+
+        @Roll_button.event("on_click")
+        def on_click_roll(event):
+            firstPlayer = random.randint(1, 2)
+
+            if firstPlayer == 1:    #Human
+                self.window.MainTurn = Logic.Turn(1, "Human", First=True)
+                self.window.MainTurn.updatePossibleMovesHumanFormat(self.window.MainBoard)
+                self.window.MainTurn.formSpriteList(self.window.MainBoard)
+                next_view = Human_1P_View(self.backgroundColor)
+                self.window.show_view(next_view)
+            else:                   #AI
+                self.window.MainTurn = Logic.Turn(2, self.window.settings["Agent2"], First=True)
+                roll = self.window.MainTurn.roll
+                self.window.MainTurn.updatePossibleMovesStandardFormat(self.window.MainBoard)
+                Moves = AI.Main(self.window.MainBoard, self.window.MainTurn, self.window.settings["Agent2"], self.window.settings["Network2 ID"])
+                self.window.MainBoard.makeMoves(Moves, 2, True)
+                next_view = Human_PreTurn_1P_View(self.backgroundColor,roll)
+                self.window.show_view(next_view)
+
+        @Settings_button.event("on_click")
+        def on_click_Settings(event):
+            self.window.lastPage = self
+            settingsView = SettingsView(self.backgroundColor)
+            self.window.show_view(settingsView)
+
+    def on_show_view(self):
+        self.manager.enable()
+        arcade.set_background_color(self.backgroundColor)
+
+    def on_hide_view(self):
+        self.manager.disable()
+
+    def on_draw(self):
+        self.clear()
+        Graphics.drawBoard()
+        Graphics.drawPieces(self.window.MainBoard.positions, self.window.MainBoard.pip)
+        self.manager.draw()
+
+
+class Human_1P_View(arcade.View):
+    
+    def __init__(self, backgroundColor):
+        super().__init__()
+        self.backgroundColor = backgroundColor
+
+        self.step = "Main"
+
+        self.manager = arcade.gui.UIManager()
+        self.manager.enable()
+
+        Exit_button = arcade.gui.UIFlatButton(15, 745, 75, 40, "Exit")
+        Quit_button = arcade.gui.UIFlatButton(15, 695, 75, 40, "Quit")
+        Settings_button = arcade.gui.UIFlatButton(1010, 15, 175, 40, "Settings")
+
+        Done_button = arcade.gui.UIFlatButton(1010, 510, 175, 40, "Done")
+
+        self.manager.add(Exit_button)
+        self.manager.add(Quit_button)
+        self.manager.add(Settings_button)
+        self.manager.add(Done_button)
+
+        @Exit_button.event("on_click")
+        def on_click_exit(event):
+            mainmenuView = MainMenuView(self.backgroundColor)
+            self.window.show_view(mainmenuView)
+
+        @Quit_button.event("on_click")
+        def on_click_Quit(event):
+            arcade.close_window()
+
+        @Settings_button.event("on_click")
+        def on_click_Settings(event):
+            self.window.lastPage = self
+            settingsView = SettingsView(self.backgroundColor)
+            self.window.show_view(settingsView)
+
+        @Done_button.event("on_click")
+        def on_click_done(event):
+
+            if self.window.MainBoard.pip[0] == 0:
+                messageBox = arcade.gui.UIMessageBox(width=300, height=150, message_text=("Game Over: \nYou Win! \n\n Exit to Main Menu For New Game"), callback=None, buttons=["Ok"])
+                self.manager.add(messageBox)
+
+                return
+
+            self.window.MainTurn = Logic.Turn(2, self.window.settings["Agent2"])
+            roll = self.window.MainTurn.roll
+            self.window.MainTurn.updatePossibleMovesStandardFormat(self.window.MainBoard)
+            Moves = AI.Main(self.window.MainBoard, self.window.MainTurn, self.window.settings["Agent2"], self.window.settings["Network2 ID"])
+            self.window.MainBoard.makeMoves(Moves, 2, True)
+            ai_win = True if self.window.MainBoard.pip[1] == 0 else False
+        
+            next_view = Human_PreTurn_1P_View(self.backgroundColor,roll,ai_win)
+            self.window.show_view(next_view)
+
+    def on_show_view(self):
+        self.manager.enable()
+        arcade.set_background_color(self.backgroundColor)
+
+    def on_hide_view(self):
+        self.manager.disable()
+
+    def on_draw(self):
+        self.clear()
+        Graphics.drawBoard()
+        arcade.draw_rectangle_filled(601, 401, 12, 762, Graphics.darkCheckerColor)
+        Graphics.drawPieces(self.window.MainBoard.positions, self.window.MainBoard.pip)
+        Graphics.drawDice(self.window.MainTurn.roll[0], self.window.MainTurn.roll[1], self.window.MainTurn.unused_dice)
+        Graphics.drawTurnMain(
+            self.window.MainTurn.sprites_move_start) if self.step == "Main" else Graphics.drawTurnBranch(
+            self.window.MainTurn.sprite_active, self.window.MainTurn.sprites_move_end)
+        self.manager.draw()
+
+    def on_mouse_press(self, x: int, y: int, button: int, modifiers: int):
+        if self.step == "Main":
+            clicked_sprite = arcade.get_sprites_at_point((x, y), self.window.MainTurn.sprites_move_start)
+            if clicked_sprite != []:
+                self.window.MainTurn.sprite_active = clicked_sprite[0]
+                self.window.MainTurn.sprites_move_end = Graphics.createMoveEndSprites(
+                    self.window.MainTurn.sprite_active, self.window.MainBoard)
+                self.step = "Branch"
+
+        elif self.step == "Branch":
+            self.step = "Main"
+            # When a possible sub-move sprite is clicked:
+            clicked_sprite = arcade.get_sprites_at_point((x, y), self.window.MainTurn.sprites_move_end)
+            if clicked_sprite != []:
+                self.window.MainBoard.makeMove((self.window.MainTurn.sprite_active.move[0], clicked_sprite[0].pos), 1)
+                if self.window.MainBoard.pip[0] == 0:
+                    pass
+                    # TO DO: add game over logic here
+                roll = Logic.fromMoveToDie(self.window.MainTurn.sprite_active.move[0], clicked_sprite[0].pos,
+                                           self.window.MainTurn.unused_dice, 1)
+                self.window.MainTurn.unused_dice.remove(roll)
+                if len(self.window.MainTurn.unused_dice) > 0:
+                    self.window.MainTurn.updatePossibleMovesHumanFormat(self.window.MainBoard)
+                    self.window.MainTurn.formSpriteList(self.window.MainBoard)
+                else:
+                    self.window.MainTurn.sprites_move_start = arcade.SpriteList()
+
+
+class Human_PreTurn_1P_View(arcade.View):
+    
+    def __init__(self, backgroundColor,last_roll,ai_win=False):
+        super().__init__()
+        self.backgroundColor = backgroundColor
+        self.ai_win = ai_win
+
+        self.manager = arcade.gui.UIManager()
+        self.manager.enable()
+
+        Exit_button = arcade.gui.UIFlatButton(15, 745, 75, 40, "Exit")
+        Quit_button = arcade.gui.UIFlatButton(15, 695, 75, 40, "Quit")
+        Settings_button = arcade.gui.UIFlatButton(1010, 15, 175, 40, "Settings")
+
+        Roll_button = arcade.gui.UIFlatButton(1010, 400, 175, 40, "Roll")
+
+        last_roll_label = arcade.gui.UILabel(1010, 450, 175, 40, f"AI Rolled {last_roll}", font_size=15, align="center", bold=True)
+
+        self.manager.add(Exit_button)
+        self.manager.add(Quit_button)
+        self.manager.add(Settings_button)
+        self.manager.add(Roll_button)
+        self.manager.add(last_roll_label)
+
+        @Exit_button.event("on_click")
+        def on_click_exit(event):
+            mainmenuView = MainMenuView(self.backgroundColor)
+            self.window.show_view(mainmenuView)
+
+        @Quit_button.event("on_click")
+        def on_click_Quit(event):
+            arcade.close_window()
+
+        @Settings_button.event("on_click")
+        def on_click_Settings(event):
+            self.window.lastPage = self
+            settingsView = SettingsView(self.backgroundColor)
+            self.window.show_view(settingsView)
+
+        @Roll_button.event("on_click")
+        def on_click_roll(event):
+            self.window.MainTurn = Logic.Turn(1, "Human")
+            self.window.MainTurn.updatePossibleMovesHumanFormat(self.window.MainBoard)
+            self.window.MainTurn.formSpriteList(self.window.MainBoard)
+
+            next_view = Human_1P_View(self.backgroundColor)
+            self.window.show_view(next_view)
+
+    def on_show_view(self):
+        self.manager.enable()
+
+        if self.ai_win:
+            messageBox = arcade.gui.UIMessageBox(width=300, height=150, message_text=(f"Game Over: \nAI Wins! \n \n Exit to Main Menu For New Game"), callback=None, buttons=["Ok"])
+            self.manager.add(messageBox)
+
+        arcade.set_background_color(self.backgroundColor)
+
+    def on_hide_view(self):
+        self.manager.disable()
+
+    def on_draw(self):
+        self.clear()
+        Graphics.drawBoard()
+        arcade.draw_rectangle_filled(601, 401, 12, 762, Graphics.darkCheckerColor)
+        Graphics.drawPieces(self.window.MainBoard.positions, self.window.MainBoard.pip)
+        if self.window.MainBoard.MoveLineData != None:
+            Graphics.DrawMoveLines(self.window.MainBoard.MoveLineData)
+        self.manager.draw()
+
 
 
 # 2P Views:
 class Start_2P_View(arcade.View):
 
     def __init__(self, backgroundColor):
         super().__init__()
```

### Comparing `willse_backgammon-0.0.1/src/willse_backgammon/Main_Files/__pycache__/AI.cpython-310.pyc` & `willse_backgammon-0.0.2/src/willse_backgammon/Main_Files/__pycache__/AI.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Sat Mar 23 17:10:54 2024 UTC, .py size: 3766 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 1e0d ff65 b60e 0000  o..........e....
+00000000: 6f0d 0d0a 0000 0000 8ee6 0166 b60e 0000  o..........f....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0008 0000 0040 0000 0073 f200 0000 6400  .....@...s....d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a01 7a1c  d.l.Z.d.d.l.Z.z.
 00000040: 6400 6402 6c02 6d03 5a04 0100 6400 6402  d.d.l.m.Z...d.d.
 00000050: 6c05 6d03 5a06 0100 6400 6402 6c07 6d03  l.m.Z...d.d.l.m.
 00000060: 5a08 0100 6400 6403 6c09 6d0a 5a0a 6d0b  Z...d.d.l.m.Z.m.
 00000070: 5a0b 0100 5700 6e23 0400 650c 7947 0100  Z...W.n#..e.yG..
```

### Comparing `willse_backgammon-0.0.1/src/willse_backgammon/Main_Files/__pycache__/Graphics.cpython-310.pyc` & `willse_backgammon-0.0.2/src/willse_backgammon/Main_Files/__pycache__/Graphics.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `willse_backgammon-0.0.1/src/willse_backgammon/Main_Files/__pycache__/Logic.cpython-310.pyc` & `willse_backgammon-0.0.2/src/willse_backgammon/Main_Files/__pycache__/Logic.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Sat Mar 23 17:12:01 2024 UTC, .py size: 17746 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 610d ff65 5245 0000  o.......a..eRE..
+00000000: 6f0d 0d0a 0000 0000 ef3a 0366 a244 0000  o........:.f.D..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0008 0000 0040 0000 0073 9000 0000 6400  .....@...s....d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a01 7a0a  d.l.Z.d.d.l.Z.z.
 00000040: 6400 6402 6c02 6d03 5a03 6d04 5a04 0100  d.d.l.m.Z.m.Z...
 00000050: 5700 6e11 0400 6505 7923 0100 0100 0100  W.n...e.y#......
 00000060: 6400 6402 6c06 6d03 5a03 6d04 5a04 0100  d.d.l.m.Z.m.Z...
 00000070: 5900 6e01 7700 6403 6404 8400 5a07 6405  Y.n.w.d.d...Z.d.
@@ -82,497 +82,496 @@
 00000510: 0383 0276 0072 1464 0453 0064 0553 0029  ...v.r.d.S.d.S.)
 00000520: 064e 7201 0000 0072 0500 0000 e907 0000  .Nr....r........
 00000530: 0054 4629 01da 0572 616e 6765 2901 720c  .TF)...range).r.
 00000540: 0000 0072 1000 0000 7210 0000 0072 1100  ...r....r....r..
 00000550: 0000 da0b 6973 4c65 6761 6c52 6f6c 6c36  ....isLegalRoll6
 00000560: 0000 0073 0600 0000 2401 0401 0402 7224  ...s....$.....r$
 00000570: 0000 0063 0000 0000 0000 0000 0000 0000  ...c............
-00000580: 0000 0000 0400 0000 4000 0000 7368 0000  ........@...sh..
+00000580: 0000 0000 0400 0000 4000 0000 7364 0000  ........@...sd..
 00000590: 0065 005a 0164 005a 0264 1864 1964 0364  .e.Z.d.Z.d.d.d.d
 000005a0: 0484 055a 0364 0564 0684 005a 0464 0764  ...Z.d.d...Z.d.d
-000005b0: 0884 005a 0564 0964 0a84 005a 0609 0b64  ...Z.d.d...Z...d
-000005c0: 1a64 0c64 0d84 015a 0709 0b64 1a64 0e64  .d.d...Z...d.d.d
-000005d0: 0f84 015a 0864 1064 1184 005a 0964 1264  ...Z.d.d...Z.d.d
-000005e0: 1384 005a 0a64 1464 1584 005a 0b64 1664  ...Z.d.d...Z.d.d
-000005f0: 1784 005a 0c64 0153 0029 1bda 0542 6f61  ...Z.d.S.)...Boa
-00000600: 7264 4eda 0672 6574 7572 6e63 0200 0000  rdN..returnc....
-00000610: 0000 0000 0000 0000 0200 0000 0200 0000  ................
-00000620: 4300 0000 733e 0000 007c 0164 0075 0072  C...s>...|.d.u.r
-00000630: 0867 0064 01a2 016e 017c 017c 005f 0064  .g.d...n.|.|._.d
-00000640: 0264 0267 027c 005f 0164 0364 0467 027c  .d.g.|._.d.d.g.|
-00000650: 005f 0264 0564 0567 027c 005f 0364 007c  ._.d.d.g.|._.d.|
-00000660: 005f 0464 0053 00a9 064e 291c e9fe ffff  ._.d.S...N).....
-00000670: ff72 0100 0000 7201 0000 0072 0100 0000  .r....r....r....
-00000680: 7201 0000 00e9 0500 0000 7201 0000 00e9  r.........r.....
-00000690: 0300 0000 7201 0000 0072 0100 0000 7201  ....r....r....r.
-000006a0: 0000 00e9 fbff ffff 7229 0000 0072 0100  ........r)...r..
-000006b0: 0000 7201 0000 0072 0100 0000 e9fd ffff  ..r....r........
-000006c0: ff72 0100 0000 722b 0000 0072 0100 0000  .r....r+...r....
-000006d0: 7201 0000 0072 0100 0000 7201 0000 00e9  r....r....r.....
-000006e0: 0200 0000 7201 0000 0072 0100 0000 7201  ....r....r....r.
-000006f0: 0000 0072 0100 0000 e9a7 0000 0072 0500  ...r.........r..
-00000700: 0000 721b 0000 0046 a905 721f 0000 00da  ..r....F..r.....
-00000710: 0370 6970 da0a 6c61 7374 506f 696e 7473  .pip..lastPoints
-00000720: da0d 6265 6172 4f66 6653 7461 7475 73da  ..bearOffStatus.
-00000730: 0c4d 6f76 654c 696e 6544 6174 6129 02da  .MoveLineData)..
-00000740: 0473 656c 665a 0d70 6f73 6974 696f 6e5f  .selfZ.position_
-00000750: 6c69 7374 7210 0000 0072 1000 0000 7211  listr....r....r.
-00000760: 0000 00da 085f 5f69 6e69 745f 5f3e 0000  .....__init__>..
-00000770: 0073 0a00 0000 1601 0a04 0a01 0a01 0a01  .s..............
-00000780: 7a0e 426f 6172 642e 5f5f 696e 6974 5f5f  z.Board.__init__
-00000790: 6301 0000 0000 0000 0000 0000 0001 0000  c...............
-000007a0: 0002 0000 0043 0000 0073 3200 0000 6700  .....C...s2...g.
-000007b0: 6401 a201 7c00 5f00 6402 6402 6702 7c00  d...|._.d.d.g.|.
-000007c0: 5f01 6403 6404 6702 7c00 5f02 6405 6405  _.d.d.g.|._.d.d.
-000007d0: 6702 7c00 5f03 6400 7c00 5f04 6400 5300  g.|._.d.|._.d.S.
-000007e0: 7227 0000 0072 2f00 0000 a901 7234 0000  r'...r/.....r4..
-000007f0: 0072 1000 0000 7210 0000 0072 1100 0000  .r....r....r....
-00000800: da11 7365 7453 7461 7274 506f 7369 7469  ..setStartPositi
-00000810: 6f6e 7348 0000 0073 0a00 0000 0a01 0a04  onsH...s........
-00000820: 0a01 0a01 0a01 7a17 426f 6172 642e 7365  ......z.Board.se
-00000830: 7453 7461 7274 506f 7369 7469 6f6e 7363  tStartPositionsc
-00000840: 0100 0000 0000 0000 0000 0000 0400 0000  ................
-00000850: 0600 0000 4300 0000 7396 0000 0064 017d  ....C...s....d.}
-00000860: 0164 017d 0274 0064 0283 0144 005d 297d  .d.}.t.d...D.])}
-00000870: 037c 006a 017c 0319 0064 016b 0472 1d7c  .|.j.|...d.k.r.|
-00000880: 027c 0364 0317 007c 006a 017c 0319 0014  .|.d...|.j.|....
-00000890: 0037 007d 0271 087c 006a 017c 0319 0064  .7.}.q.|.j.|...d
-000008a0: 016b 0072 317c 0164 027c 0318 0074 027c  .k.r1|.d.|...t.|
-000008b0: 006a 017c 0319 0083 0114 0037 007d 0171  .j.|.......7.}.q
-000008c0: 087c 0164 047c 006a 0164 0219 0014 0037  .|.d.|.j.d.....7
-000008d0: 007d 017c 0264 047c 006a 0164 0419 0014  .}.|.d.|.j.d....
-000008e0: 0037 007d 027c 017c 0266 027c 005f 0364  .7.}.|.|.f.|._.d
-000008f0: 0053 00a9 054e 7201 0000 0072 1b00 0000  .S...Nr....r....
-00000900: 7205 0000 0072 0600 0000 2904 7223 0000  r....r....).r#..
-00000910: 0072 1f00 0000 da03 6162 7372 3000 0000  .r......absr0...
-00000920: a904 7234 0000 005a 0670 315f 7069 705a  ..r4...Z.p1_pipZ
-00000930: 0670 325f 7069 70da 0169 7210 0000 0072  .p2_pip..ir....r
-00000940: 1000 0000 7211 0000 00da 0975 7064 6174  ....r......updat
-00000950: 6550 6970 5200 0000 7316 0000 0004 0104  ePipR...s.......
-00000960: 010c 010e 0118 010e 011a 0102 8012 0112  ................
-00000970: 010e 017a 0f42 6f61 7264 2e75 7064 6174  ...z.Board.updat
-00000980: 6550 6970 6301 0000 0000 0000 0000 0000  ePipc...........
-00000990: 0004 0000 0006 0000 0043 0000 0073 9000  .........C...s..
-000009a0: 0000 6401 7d01 6401 7d02 7400 6402 8301  ..d.}.d.}.t.d...
-000009b0: 4400 5d29 7d03 7c00 6a01 7c03 1900 6401  D.])}.|.j.|...d.
-000009c0: 6b04 721d 7c02 7c03 6403 1700 7c00 6a01  k.r.|.|.d...|.j.
-000009d0: 7c03 1900 1400 3700 7d02 7108 7c00 6a01  |.....7.}.q.|.j.
-000009e0: 7c03 1900 6401 6b00 7231 7c01 6402 7c03  |...d.k.r1|.d.|.
-000009f0: 1800 7402 7c00 6a01 7c03 1900 8301 1400  ..t.|.j.|.......
-00000a00: 3700 7d01 7108 7c01 6404 7c00 6a01 6402  7.}.q.|.d.|.j.d.
-00000a10: 1900 1400 3700 7d01 7c02 6404 7c00 6a01  ....7.}.|.d.|.j.
-00000a20: 6404 1900 1400 3700 7d02 7c01 7c02 6602  d.....7.}.|.|.f.
-00000a30: 5300 7238 0000 0029 0372 2300 0000 721f  S.r8...).r#...r.
-00000a40: 0000 0072 3900 0000 723a 0000 0072 1000  ...r9...r:...r..
-00000a50: 0000 7210 0000 0072 1100 0000 da09 7265  ..r....r......re
-00000a60: 7475 726e 5069 705e 0000 0073 1600 0000  turnPip^...s....
-00000a70: 0401 0401 0c01 0e01 1801 0e01 1a01 0280  ................
-00000a80: 1201 1201 0801 7a0f 426f 6172 642e 7265  ......z.Board.re
-00000a90: 7475 726e 5069 7046 6304 0000 0000 0000  turnPipFc.......
-00000aa0: 0000 0000 0006 0000 0004 0000 0043 0000  .............C..
-00000ab0: 0073 0c02 0000 7c01 6401 1900 6402 6b02  .s....|.d...d.k.
-00000ac0: 725b 7c01 6403 1900 6403 1800 7d04 7c00  r[|.d...d...}.|.
-00000ad0: 6a00 6404 7c02 1700 0500 1900 6403 3800  j.d.|.......d.8.
-00000ae0: 0300 3c00 7c02 6403 6b02 723b 7c00 6a00  ..<.|.d.k.r;|.j.
-00000af0: 7c04 1900 6401 6b04 7231 6405 7c00 6a00  |...d.k.r1d.|.j.
-00000b00: 7c04 3c00 7c00 6a00 6406 0500 1900 6403  |.<.|.j.d.....d.
-00000b10: 3700 0300 3c00 6ebf 7c00 6a00 7c04 0500  7...<.n.|.j.|...
-00000b20: 1900 6403 3800 0300 3c00 6eb5 7c00 6a00  ..d.8...<.n.|.j.
-00000b30: 7c04 1900 6401 6b00 7251 6403 7c00 6a00  |...d.k.rQd.|.j.
-00000b40: 7c04 3c00 7c00 6a00 6407 0500 1900 6403  |.<.|.j.d.....d.
-00000b50: 3700 0300 3c00 6e9f 7c00 6a00 7c04 0500  7...<.n.|.j.|...
-00000b60: 1900 6403 3700 0300 3c00 6e95 7c01 6403  ..d.7...<.n.|.d.
-00000b70: 1900 6408 6b02 728a 7c01 6401 1900 6403  ..d.k.r.|.d...d.
-00000b80: 1800 7d05 7c02 6403 6b02 7275 7c00 6a00  ..}.|.d.k.ru|.j.
-00000b90: 7c05 0500 1900 6403 3700 0300 3c00 6e09  |.....d.7...<.n.
-00000ba0: 7c00 6a00 7c05 0500 1900 6403 3800 0300  |.j.|.....d.8...
-00000bb0: 3c00 7c00 6a00 6406 7c02 1700 0500 1900  <.|.j.d.|.......
-00000bc0: 6403 3700 0300 3c00 6e66 7c01 6403 1900  d.7...<.nf|.d...
-00000bd0: 6403 1800 7d04 7c01 6401 1900 6403 1800  d...}.|.d...d...
-00000be0: 7d05 7c02 6403 6b02 72a4 7c00 6a00 7c05  }.|.d.k.r.|.j.|.
-00000bf0: 0500 1900 6403 3700 0300 3c00 6e09 7c00  ....d.7...<.n.|.
-00000c00: 6a00 7c05 0500 1900 6403 3800 0300 3c00  j.|.....d.8...<.
-00000c10: 7c02 6403 6b02 72d1 7c00 6a00 7c04 1900  |.d.k.r.|.j.|...
-00000c20: 6401 6b04 72c7 6405 7c00 6a00 7c04 3c00  d.k.r.d.|.j.|.<.
-00000c30: 7c00 6a00 6406 0500 1900 6403 3700 0300  |.j.d.....d.7...
-00000c40: 3c00 6e29 7c00 6a00 7c04 0500 1900 6403  <.n)|.j.|.....d.
-00000c50: 3800 0300 3c00 6e1f 7c00 6a00 7c04 1900  8...<.n.|.j.|...
-00000c60: 6401 6b00 72e7 6403 7c00 6a00 7c04 3c00  d.k.r.d.|.j.|.<.
-00000c70: 7c00 6a00 6407 0500 1900 6403 3700 0300  |.j.d.....d.7...
-00000c80: 3c00 6e09 7c00 6a00 7c04 0500 1900 6403  <.n.|.j.|.....d.
-00000c90: 3700 0300 3c00 7c03 6409 6b02 9001 7204  7...<.|.d.k...r.
-00000ca0: 7c00 a001 a100 0100 7c00 a002 7c02 a101  |.......|...|...
-00000cb0: 0100 7c00 a003 a100 0100 6400 5300 6400  ..|.......d.S.d.
-00000cc0: 5300 290a 4e72 0100 0000 7204 0000 0072  S.).Nr....r....r
-00000cd0: 0500 0000 e917 0000 0072 0800 0000 7206  .........r....r.
-00000ce0: 0000 0072 1b00 0000 7207 0000 0046 2904  ...r....r....F).
-00000cf0: 721f 0000 0072 3c00 0000 da17 7570 6461  r....r<.....upda
-00000d00: 7465 4c61 7374 4f63 6375 7069 6564 506f  teLastOccupiedPo
-00000d10: 696e 74da 1375 7064 6174 6542 6561 724f  int..updateBearO
-00000d20: 6666 5374 6174 7573 2906 7234 0000 00da  ffStatus).r4....
-00000d30: 046d 6f76 6572 0d00 0000 5a0d 6672 6f6d  .mover....Z.from
-00000d40: 4d61 6b65 4d6f 7665 735a 0d65 6e64 506f  MakeMovesZ.endPo
-00000d50: 696e 7449 6e64 6578 5a0f 7374 6172 7450  intIndexZ.startP
-00000d60: 6f69 6e74 496e 6465 7872 1000 0000 7210  ointIndexr....r.
-00000d70: 0000 0072 1100 0000 da08 6d61 6b65 4d6f  ...r......makeMo
-00000d80: 7665 6a00 0000 734a 0000 000c 020c 0116  vej...sJ........
-00000d90: 0108 010e 010a 0114 0114 020e 020a 0114  ................
-00000da0: 0114 020c 010c 0108 0114 0112 0218 010c  ................
-00000db0: 020c 0108 0114 0112 0208 010e 010a 0114  ................
-00000dc0: 0114 020e 020a 0114 0112 020a 0108 010a  ................
-00000dd0: 010c 0104 fd7a 0e42 6f61 7264 2e6d 616b  .....z.Board.mak
-00000de0: 654d 6f76 6563 0400 0000 0000 0000 0000  eMovec..........
-00000df0: 0000 0600 0000 0600 0000 4300 0000 7398  ..........C...s.
-00000e00: 0000 0067 007d 0474 007c 0183 0164 016b  ...g.}.t.|...d.k
-00000e10: 0472 2274 017c 0164 0119 0083 0174 026b  .r"t.|.d.....t.k
-00000e20: 0272 227c 00a0 037c 017c 0264 02a1 0301  .r"|...|.|.d....
-00000e30: 007c 0364 026b 0272 2174 047c 017c 0083  .|.d.k.r!t.|.|..
-00000e40: 027c 005f 056e 1b7c 0144 005d 157d 057c  .|._.n.|.D.].}.|
-00000e50: 00a0 037c 057c 0264 02a1 0301 007c 0364  ...|.|.d.....|.d
-00000e60: 026b 0272 397c 04a0 0674 047c 057c 0083  .k.r9|...t.|.|..
-00000e70: 02a1 0101 0071 247c 047c 005f 057c 00a0  .....q$|.|._.|..
-00000e80: 07a1 0001 007c 00a0 087c 02a1 0101 007c  .....|...|.....|
-00000e90: 00a0 09a1 0001 0064 0053 0029 034e 7201  .......d.S.).Nr.
-00000ea0: 0000 0054 290a 7215 0000 00da 0474 7970  ...T).r......typ
-00000eb0: 65da 0369 6e74 7242 0000 0072 0300 0000  e..intrB...r....
-00000ec0: 7233 0000 00da 0661 7070 656e 6472 3c00  r3.....appendr<.
-00000ed0: 0000 723f 0000 0072 4000 0000 2906 7234  ..r?...r@...).r4
-00000ee0: 0000 005a 056d 6f76 6573 720d 0000 005a  ...Z.movesr....Z
-00000ef0: 0e75 7064 6174 654c 696e 6544 6174 6172  .updateLineDatar
-00000f00: 3300 0000 7241 0000 0072 1000 0000 7210  3...rA...r....r.
-00000f10: 0000 0072 1100 0000 da09 6d61 6b65 4d6f  ...r......makeMo
-00000f20: 7665 739a 0000 0073 1e00 0000 0402 1c01  ves....s........
-00000f30: 0e01 0801 0c01 0280 0802 0e01 0801 1001  ................
-00000f40: 0280 0601 0801 0a01 0c01 7a0f 426f 6172  ..........z.Boar
-00000f50: 642e 6d61 6b65 4d6f 7665 7363 0200 0000  d.makeMovesc....
-00000f60: 0000 0000 0000 0000 0300 0000 0400 0000  ................
-00000f70: 4300 0000 7378 0000 007c 0164 016b 0272  C...sx...|.d.k.r
-00000f80: 2074 0064 0264 0364 0183 0344 005d 137d   t.d.d.d...D.].}
-00000f90: 027c 006a 017c 0219 0064 026b 0072 1d7c  .|.j.|...d.k.r.|
-00000fa0: 0264 0117 007c 006a 0264 023c 0001 0064  .d...|.j.d.<...d
-00000fb0: 0053 0071 0a64 0053 0074 0064 0464 0564  .S.q.d.S.t.d.d.d
-00000fc0: 0583 0344 005d 137d 027c 006a 017c 0219  ...D.].}.|.j.|..
-00000fd0: 0064 026b 0472 397c 0264 0117 007c 006a  .d.k.r9|.d...|.j
-00000fe0: 0264 013c 0001 0064 0053 0071 2664 0053  .d.<...d.S.q&d.S
-00000ff0: 0029 064e 7205 0000 0072 0100 0000 721b  .).Nr....r....r.
-00001000: 0000 0072 3e00 0000 7208 0000 0029 0372  ...r>...r....).r
-00001010: 2300 0000 721f 0000 0072 3100 0000 2903  #...r....r1...).
-00001020: 7234 0000 0072 0d00 0000 da05 696e 6465  r4...r......inde
-00001030: 7872 1000 0000 7210 0000 0072 1100 0000  xr....r....r....
-00001040: 723f 0000 00ab 0000 0073 1a00 0000 0801  r?.......s......
-00001050: 1001 0e01 0e01 0601 02fe 04ff 1005 0e01  ................
-00001060: 0e01 0601 02fe 04ff 7a1d 426f 6172 642e  ........z.Board.
-00001070: 7570 6461 7465 4c61 7374 4f63 6375 7069  updateLastOccupi
-00001080: 6564 506f 696e 7463 0100 0000 0000 0000  edPointc........
-00001090: 0000 0000 0100 0000 0300 0000 4300 0000  ............C...
-000010a0: 7350 0000 007c 006a 0064 0119 0073 0c7c  sP...|.j.d...s.|
-000010b0: 006a 0164 0119 0064 026b 0472 0e64 036e  .j.d...d.k.r.d.n
-000010c0: 0164 047c 006a 0064 013c 007c 006a 0064  .d.|.j.d.<.|.j.d
-000010d0: 0519 0073 1f7c 006a 0164 0519 0064 066b  ...s.|.j.d...d.k
-000010e0: 0072 2164 036e 0164 047c 006a 0064 053c  .r!d.n.d.|.j.d.<
-000010f0: 0064 0053 0029 074e 7201 0000 00e9 1200  .d.S.).Nr.......
-00001100: 0000 5446 7205 0000 0072 2200 0000 2902  ..TFr....r"...).
-00001110: 7232 0000 0072 3100 0000 7236 0000 0072  r2...r1...r6...r
-00001120: 1000 0000 7210 0000 0072 1100 0000 7240  ....r....r....r@
-00001130: 0000 00b7 0000 0073 0400 0000 2601 2a01  .......s....&.*.
-00001140: 7a19 426f 6172 642e 7570 6461 7465 4265  z.Board.updateBe
-00001150: 6172 4f66 6653 7461 7475 7363 0400 0000  arOffStatusc....
-00001160: 0000 0000 0000 0000 0700 0000 0600 0000  ................
-00001170: 0300 0000 73cc 0100 0067 007d 0487 0066  ....s....g.}...f
-00001180: 0164 0164 0284 087d 057c 0264 036b 0272  .d.d...}.|.d.k.r
-00001190: 7988 006a 0064 0419 0064 056b 0472 237c  y..j.d...d.k.r#|
-000011a0: 057c 0164 0383 0264 066b 0272 217c 04a0  .|.d...d.k.r!|..
-000011b0: 0164 077c 0166 02a1 0101 007c 0453 0074  .d.|.f.....|.S.t
-000011c0: 0264 0483 0144 005d 217d 0688 006a 007c  .d...D.]!}...j.|
-000011d0: 0619 0064 056b 0072 487c 057c 067c 0117  ...d.k.rH|.|.|..
-000011e0: 0064 0317 0064 0383 0264 066b 0272 487c  .d...d...d.k.rH|
-000011f0: 04a0 017c 0664 0317 007c 067c 0117 0064  ...|.d...|.|...d
-00001200: 0317 0066 02a1 0101 0071 2788 006a 0364  ...f.....q'..j.d
-00001210: 0519 0064 066b 0272 7788 006a 0064 047c  ...d.k.rw..j.d.|
-00001220: 0118 0019 0064 056b 0072 627c 04a0 0164  .....d.k.rb|...d
-00001230: 087c 0118 0064 0966 02a1 0101 007c 0372  .|...d.f.....|.r
-00001240: 7788 006a 0464 0519 0064 087c 0118 006b  w..j.d...d.|...k
-00001250: 0472 777c 04a0 0188 006a 0464 0519 0064  .rw|.....j.d...d
-00001260: 0966 02a1 0101 007c 0453 0088 006a 0064  .f.....|.S...j.d
-00001270: 0819 0064 056b 0472 947c 0564 087c 0118  ...d.k.r.|.d.|..
-00001280: 0064 0a83 0264 066b 0272 927c 04a0 0164  .d...d.k.r.|...d
-00001290: 0764 087c 0118 0066 02a1 0101 007c 0453  .d.|...f.....|.S
-000012a0: 0074 0264 0483 0144 005d 217d 0688 006a  .t.d...D.]!}...j
-000012b0: 007c 0619 0064 056b 0472 b97c 057c 067c  .|...d.k.r.|.|.|
-000012c0: 0118 0064 0317 0064 0a83 0264 066b 0272  ...d...d...d.k.r
-000012d0: b97c 04a0 017c 0664 0317 007c 067c 0118  .|...|.d...|.|..
-000012e0: 0064 0317 0066 02a1 0101 0071 9888 006a  .d...f.....q...j
-000012f0: 0364 0319 0064 066b 0272 e488 006a 007c  .d...d.k.r...j.|
-00001300: 0164 0318 0019 0064 056b 0472 d17c 04a0  .d.....d.k.r.|..
-00001310: 017c 0164 0966 02a1 0101 007c 0372 e488  .|.d.f.....|.r..
-00001320: 006a 0464 0319 007c 016b 0072 e47c 04a0  .j.d...|.k.r.|..
-00001330: 0188 006a 0464 0319 0064 0966 02a1 0101  ...j.d...d.f....
-00001340: 007c 0453 0029 0b4e 6302 0000 0000 0000  .|.S.).Nc.......
-00001350: 0000 0000 0003 0000 0003 0000 0013 0000  ................
-00001360: 0073 9000 0000 7c00 6401 6b04 7308 7c00  .s....|.d.k.s.|.
-00001370: 6402 6b00 720a 6403 5300 7c01 6404 6b02  d.k.r.d.S.|.d.k.
-00001380: 7210 6405 6e01 6402 7d02 8800 6a00 7c00  r.d.n.d.}...j.|.
-00001390: 6402 1800 1900 6406 6b02 721d 6407 5300  d.....d.k.r.d.S.
-000013a0: 8800 6a00 7c00 6402 1800 1900 6406 6b04  ..j.|.d.....d.k.
-000013b0: 722c 7c01 6404 6b02 722c 6407 5300 8800  r,|.d.k.r,d.S...
-000013c0: 6a00 7c00 6402 1800 1900 6406 6b00 723b  j.|.d.....d.k.r;
-000013d0: 7c01 6402 6b02 723b 6407 5300 8800 6a00  |.d.k.r;d.S...j.
-000013e0: 7c00 6402 1800 1900 7c02 6b02 7246 6407  |.d.....|.k.rFd.
-000013f0: 5300 6400 5300 2908 4e72 1b00 0000 7205  S.d.S.).Nr....r.
-00001400: 0000 0046 722d 0000 0072 0800 0000 7201  ...Fr-...r....r.
-00001410: 0000 0054 2901 721f 0000 0029 03da 0570  ...T).r....)...p
-00001420: 6f69 6e74 720d 0000 005a 086f 7070 5661  ointr....Z.oppVa
-00001430: 6c75 6572 3600 0000 7210 0000 0072 1100  luer6...r....r..
-00001440: 0000 da09 6361 6e4d 6f76 6554 6fbf 0000  ....canMoveTo...
-00001450: 0073 1800 0000 1001 0401 1001 1201 0401  .s..............
-00001460: 1a01 0401 1a01 0401 1201 0401 04ff 7a2a  ..............z*
-00001470: 426f 6172 642e 7265 7475 726e 4d6f 7665  Board.returnMove
-00001480: 7346 6f72 4469 652e 3c6c 6f63 616c 733e  sForDie.<locals>
-00001490: 2e63 616e 4d6f 7665 546f 7205 0000 0072  .canMoveTor....r
-000014a0: 1b00 0000 7201 0000 0054 7204 0000 0072  ....r....Tr....r
-000014b0: 0600 0000 7207 0000 0072 2d00 0000 2905  ....r....r-...).
-000014c0: 721f 0000 0072 4500 0000 7223 0000 0072  r....rE...r#...r
-000014d0: 3200 0000 7231 0000 0029 0772 3400 0000  2...r1...).r4...
-000014e0: 720e 0000 0072 0d00 0000 5a18 6973 4269  r....r....Z.isBi
-000014f0: 6767 6573 7444 6965 4f72 5365 636f 6e64  ggestDieOrSecond
-00001500: 4d6f 7665 5a08 6d6f 7665 4c69 7374 724a  MoveZ.moveListrJ
-00001510: 0000 005a 0a70 6f69 6e74 496e 6465 7872  ...Z.pointIndexr
-00001520: 1000 0000 7236 0000 0072 1100 0000 da11  ....r6...r......
-00001530: 7265 7475 726e 4d6f 7665 7346 6f72 4469  returnMovesForDi
-00001540: 65bb 0000 0073 4200 0000 0402 0c02 080d  e....sB.........
-00001550: 0e01 0e01 0e01 041b 0ce7 0e01 1601 1a01  ................
-00001560: 0280 0e01 1201 1201 1601 1401 0411 0ef2  ................
-00001570: 1201 1201 040c 0cf6 0e01 1601 1a01 0280  ................
-00001580: 0e01 1201 0e01 1201 1401 0402 7a17 426f  ............z.Bo
-00001590: 6172 642e 7265 7475 726e 4d6f 7665 7346  ard.returnMovesF
-000015a0: 6f72 4469 6563 0300 0000 0000 0000 0000  orDiec..........
-000015b0: 0000 1600 0000 0a00 0000 4300 0000 7320  ..........C...s 
-000015c0: 0300 0067 007d 0367 007d 047c 0264 0119  ...g.}.g.}.|.d..
-000015d0: 007c 0264 0219 006b 0372 a97c 0264 0119  .|.d...k.r.|.d..
-000015e0: 007c 0264 0219 006b 0572 187c 0264 0119  .|.d...k.r.|.d..
-000015f0: 006e 037c 0264 0219 007d 0567 007d 067c  .n.|.d...}.g.}.|
-00001600: 0244 005d 0e7d 077c 06a0 007c 00a0 017c  .D.].}.|...|...|
-00001610: 077c 017c 057c 076b 02a1 03a1 0101 0071  .|.|.|.k.......q
-00001620: 207c 0664 0119 007c 0664 0219 0017 007d   |.d...|.d.....}
-00001630: 067c 0644 005d 6d7d 0874 02a0 037c 00a1  .|.D.]m}.t...|..
-00001640: 017d 097c 09a0 047c 087c 01a1 0201 007c  .}.|...|.|.....|
-00001650: 096a 057c 0164 0218 0019 0064 016b 0272  .j.|.d.....d.k.r
-00001660: 567c 0867 017d 037c 0302 0001 0053 0074  V|.g.}.|.....S.t
-00001670: 067c 0864 0119 007c 0864 0219 007c 027c  .|.d...|.d...|.|
-00001680: 0183 047d 0a7c 0264 0219 007c 0a6b 0272  ...}.|.d...|.k.r
-00001690: 6b7c 0264 0119 006e 037c 0264 0219 007d  k|.d...n.|.d...}
-000016a0: 0b7c 09a0 017c 0b7c 0164 03a1 037d 0c74  .|...|.|.d...}.t
-000016b0: 077c 0c83 0164 016b 0272 827c 03a0 007c  .|...d.k.r.|...|
-000016c0: 08a1 0101 0071 397c 0c44 005d 217d 0d74  .....q9|.D.]!}.t
-000016d0: 02a0 037c 00a1 017d 0e7c 0ea0 087c 087c  ...|...}.|...|.|
-000016e0: 0d66 027c 01a1 0201 007c 0e6a 097c 0476  .f.|.....|.j.|.v
-000016f0: 0172 a57c 03a0 007c 087c 0d66 02a1 0101  .r.|...|.|.f....
-00001700: 007c 04a0 007c 0e6a 09a1 0101 0071 8471  .|...|.j.....q.q
-00001710: 397c 0353 007c 00a0 017c 0264 0119 007c  9|.S.|...|.d...|
-00001720: 0164 03a1 037d 067c 0644 005d d97d 0f74  .d...}.|.D.].}.t
-00001730: 02a0 037c 00a1 017d 097c 09a0 047c 0f7c  ...|...}.|...|.|
-00001740: 01a1 0201 007c 096a 057c 0164 0218 0019  .....|.j.|.d....
-00001750: 0064 016b 0272 d17c 0f67 017d 037c 0302  .d.k.r.|.g.}.|..
-00001760: 0001 0053 007c 09a0 017c 0264 0119 007c  ...S.|...|.d...|
-00001770: 0164 03a1 037d 0c74 077c 0c83 0164 016b  .d...}.t.|...d.k
-00001780: 0272 e67c 03a0 007c 0fa1 0101 0071 b47c  .r.|...|.....q.|
-00001790: 0c44 005d a47d 0d74 02a0 037c 09a1 017d  .D.].}.t...|...}
-000017a0: 0e7c 0ea0 047c 0d7c 01a1 0201 007c 0e6a  .|...|.|.....|.j
-000017b0: 057c 0164 0218 0019 0064 016b 0290 0172  .|.d.....d.k...r
-000017c0: 077c 03a0 007c 0f7c 0d66 02a1 0101 0071  .|...|.|.f.....q
-000017d0: e87c 0ea0 017c 0264 0119 007c 0164 03a1  .|...|.d...|.d..
-000017e0: 037d 1074 077c 1083 0164 016b 0290 0172  .}.t.|...d.k...r
-000017f0: 1f7c 03a0 007c 0f7c 0d67 02a1 0101 0071  .|...|.|.g.....q
-00001800: e87c 1044 005d 6a7d 1174 02a0 037c 0ea1  .|.D.]j}.t...|..
-00001810: 017d 127c 12a0 047c 117c 01a1 0201 007c  .}.|...|.|.....|
-00001820: 0e6a 057c 0164 0218 0019 0064 016b 0290  .j.|.d.....d.k..
-00001830: 0172 467c 0f7c 0d7c 1166 0367 017d 037c  .rF|.|.|.f.g.}.|
-00001840: 0302 0001 0002 0001 0002 0001 0053 007c  .............S.|
-00001850: 12a0 017c 0264 0119 007c 0164 03a1 037d  ...|.d...|.d...}
-00001860: 1374 077c 1383 0164 016b 0290 0172 607c  .t.|...d.k...r`|
-00001870: 03a0 007c 0f7c 0d7c 1167 03a1 0101 0090  ...|.|.|.g......
-00001880: 0171 217c 1344 005d 277d 1474 02a0 037c  .q!|.D.]'}.t...|
-00001890: 00a1 017d 157c 15a0 087c 0f7c 0d7c 117c  ...}.|...|.|.|.|
-000018a0: 1466 047c 01a1 0201 007c 156a 097c 0476  .f.|.....|.j.|.v
-000018b0: 0190 0172 887c 03a0 007c 0f7c 0d7c 117c  ...r.|...|.|.|.|
-000018c0: 1466 04a1 0101 007c 04a0 007c 156a 09a1  .f.....|...|.j..
-000018d0: 0101 0090 0171 6290 0171 2171 e871 b47c  .....qb..q!q.q.|
-000018e0: 0353 0029 044e 7201 0000 0072 0500 0000  .S.).Nr....r....
-000018f0: 5429 0a72 4500 0000 724b 0000 00da 0463  T).rE...rK.....c
-00001900: 6f70 79da 0864 6565 7063 6f70 7972 4200  opy..deepcopyrB.
-00001910: 0000 7230 0000 0072 1200 0000 7215 0000  ..r0...r....r...
-00001920: 0072 4600 0000 721f 0000 0029 1672 3400  .rF...r....).r4.
-00001930: 0000 720d 0000 0072 0c00 0000 5a09 5365  ..r....r....Z.Se
-00001940: 7175 656e 6365 735a 0945 6e64 426f 6172  quencesZ.EndBoar
-00001950: 6473 da09 6269 6767 6572 4469 655a 0a46  ds..biggerDieZ.F
-00001960: 6972 7374 4d6f 7665 7372 0e00 0000 7241  irstMovesr....rA
-00001970: 0000 005a 0a61 6c67 6f42 6f61 7264 315a  ...Z.algoBoard1Z
-00001980: 0775 7365 6444 6965 5a09 756e 7573 6564  .usedDieZ.unused
-00001990: 4469 655a 0b53 6563 6f6e 644d 6f76 6573  DieZ.SecondMoves
-000019a0: 5a0a 7365 636f 6e64 4d6f 7665 5a0a 616c  Z.secondMoveZ.al
-000019b0: 676f 426f 6172 6432 5a09 6669 7273 744d  goBoard2Z.firstM
-000019c0: 6f76 655a 0a54 6869 7264 4d6f 7665 735a  oveZ.ThirdMovesZ
-000019d0: 0974 6869 7264 4d6f 7665 5a0a 616c 676f  .thirdMoveZ.algo
-000019e0: 426f 6172 6433 5a0a 466f 7274 684d 6f76  Board3Z.ForthMov
-000019f0: 6573 5a09 666f 7274 684d 6f76 655a 0a61  esZ.forthMoveZ.a
-00001a00: 6c67 6f42 6f61 7264 3472 1000 0000 7210  lgoBoard4r....r.
-00001a10: 0000 0072 1100 0000 da13 7265 7475 726e  ...r......return
-00001a20: 4d6f 7665 5365 7175 656e 6365 73ec 0000  MoveSequences...
-00001a30: 0073 8e00 0000 0402 0401 1001 2001 0401  .s.......... ...
-00001a40: 0803 1a01 1001 0802 0a01 0c01 1201 0601  ................
-00001a50: 0801 1601 1c01 0e01 0c01 0a01 0201 0801  ................
-00001a60: 0a01 1001 0a01 0e01 0c01 0280 02fb 0406  ................
-00001a70: 1203 0801 0a01 0c01 1201 0601 0801 1201  ................
-00001a80: 0c01 0a01 0201 0801 0a01 0c01 1401 0e01  ................
-00001a90: 0201 1201 0e01 0e01 0201 0801 0a01 0c01  ................
-00001aa0: 1401 0c01 1001 1201 0e01 1001 0401 0801  ................
-00001ab0: 0a01 1401 0c01 1201 0c01 0480 04fb 02f6  ................
-00001ac0: 02f6 041a 7a19 426f 6172 642e 7265 7475  ....z.Board.retu
-00001ad0: 726e 4d6f 7665 5365 7175 656e 6365 7372  rnMoveSequencesr
-00001ae0: 1300 0000 2902 7226 0000 004e 2901 4629  ....).r&...N).F)
-00001af0: 0dda 085f 5f6e 616d 655f 5fda 0a5f 5f6d  ...__name__..__m
-00001b00: 6f64 756c 655f 5fda 0c5f 5f71 7561 6c6e  odule__..__qualn
-00001b10: 616d 655f 5f72 3500 0000 7237 0000 0072  ame__r5...r7...r
-00001b20: 3c00 0000 723d 0000 0072 4200 0000 7246  <...r=...rB...rF
-00001b30: 0000 0072 3f00 0000 7240 0000 0072 4b00  ...r?...r@...rK.
-00001b40: 0000 724f 0000 0072 1000 0000 7210 0000  ..rO...r....r...
-00001b50: 0072 1000 0000 7211 0000 0072 2500 0000  .r....r....r%...
-00001b60: 3d00 0000 731a 0000 0008 000c 0108 0a08  =...s...........
-00001b70: 0a08 0c02 0d0a ff02 310a ff08 1108 0c08  ........1.......
-00001b80: 040c 3172 2500 0000 6300 0000 0000 0000  ..1r%...c.......
-00001b90: 0000 0000 0000 0000 0003 0000 0040 0000  .............@..
-00001ba0: 0073 3a00 0000 6500 5a01 6400 5a02 640c  .s:...e.Z.d.Z.d.
-00001bb0: 6403 6404 8401 5a03 6405 6504 6602 6406  d.d...Z.d.e.f.d.
-00001bc0: 6407 8404 5a05 6405 6504 6602 6408 6409  d...Z.d.e.f.d.d.
-00001bd0: 8404 5a06 640a 640b 8400 5a07 6401 5300  ..Z.d.d...Z.d.S.
-00001be0: 290d da04 5475 726e 4e46 6305 0000 0000  )...TurnNFc.....
-00001bf0: 0000 0000 0000 0005 0000 0003 0000 0043  ...............C
-00001c00: 0000 0073 d800 0000 7c01 7c00 5f00 7c02  ...s....|.|._.|.
-00001c10: 7c00 5f01 7c03 6400 6b03 720c 7c03 6e02  |._.|.d.k.r.|.n.
-00001c20: 7402 8300 7c00 5f03 7c00 6a03 6401 1900  t...|._.|.j.d...
-00001c30: 7c00 6a03 6402 1900 6b02 721c 6403 6e01  |.j.d...k.r.d.n.
-00001c40: 6404 7c00 5f04 6700 7c00 5f05 6700 7c00  d.|._.g.|._.g.|.
-00001c50: 5f06 7c00 6a01 6405 6b02 7233 6700 7c00  _.|.j.d.k.r3g.|.
-00001c60: 5f07 6700 7c00 5f08 6700 7c00 5f09 7c04  _.g.|._.g.|._.|.
-00001c70: 7253 7c00 6a04 7253 7c00 6a03 6401 1900  rS|.j.rS|.j.d...
-00001c80: 7c00 6a03 6402 1900 6b02 7250 7402 8300  |.j.d...k.rPt...
-00001c90: 7c00 5f03 7c00 6a03 6401 1900 7c00 6a03  |._.|.j.d...|.j.
-00001ca0: 6402 1900 6b02 7342 6404 7c00 5f04 7c00  d...k.sBd.|._.|.
-00001cb0: 6a04 6403 6b02 7263 7c00 6a03 6401 1900  j.d.k.rc|.j.d...
-00001cc0: 6701 6406 1400 7c00 5f05 6400 5300 740a  g.d...|._.d.S.t.
-00001cd0: a00b 7c00 6a03 a101 7c00 5f05 6400 5300  ..|.j...|._.d.S.
-00001ce0: 2907 4e72 0100 0000 7205 0000 0054 46da  ).Nr....r....TF.
-00001cf0: 0548 756d 616e e904 0000 0029 0c72 0d00  .Human.....).r..
-00001d00: 0000 da0a 706c 6179 6572 5479 7065 721a  ....playerTyper.
-00001d10: 0000 0072 0c00 0000 da0c 646f 7562 6c65  ...r......double
-00001d20: 735f 7475 726e da0b 756e 7573 6564 5f64  s_turn..unused_d
-00001d30: 6963 65da 1663 7572 7265 6e74 5f70 6f73  ice..current_pos
-00001d40: 7369 626c 655f 6d6f 7665 73da 1273 7072  sible_moves..spr
-00001d50: 6974 6573 5f6d 6f76 655f 7374 6172 745a  ites_move_startZ
-00001d60: 1073 7072 6974 6573 5f6d 6f76 655f 656e  .sprites_move_en
-00001d70: 645a 0d73 7072 6974 655f 6163 7469 7665  dZ.sprite_active
-00001d80: 724c 0000 0072 4d00 0000 2905 7234 0000  rL...rM...).r4..
-00001d90: 0072 0d00 0000 7256 0000 0072 0c00 0000  .r....rV...r....
-00001da0: 5a05 4669 7273 7472 1000 0000 7210 0000  Z.Firstr....r...
-00001db0: 0072 1100 0000 7235 0000 0037 0100 0073  .r....r5...7...s
-00001dc0: 2400 0000 0601 0601 1402 1e01 0601 0602  $...............
-00001dd0: 0a02 0601 0601 0601 0a03 1401 0801 14ff  ................
-00001de0: 0602 0a03 1601 1202 7a0d 5475 726e 2e5f  ........z.Turn._
-00001df0: 5f69 6e69 745f 5f72 2500 0000 6302 0000  _init__r%...c...
-00001e00: 0000 0000 0000 0000 000b 0000 0009 0000  ................
-00001e10: 0043 0000 0073 8601 0000 6700 7c00 5f00  .C...s....g.|._.
-00001e20: 7c00 6a01 6401 6b02 7226 7402 7c00 6a03  |.j.d.k.r&t.|.j.
-00001e30: 8301 6402 6b04 7226 7c01 a004 7c00 6a05  ..d.k.r&|...|.j.
-00001e40: 6402 1900 7c00 6a06 6401 a103 7c00 5f00  d...|.j.d...|._.
-00001e50: 6403 6404 8400 7c00 6a00 4400 8301 7c00  d.d...|.j.D...|.
-00001e60: 5f00 6400 5300 7c00 6a05 6402 1900 7c00  _.d.S.|.j.d...|.
-00001e70: 6a05 6405 1900 6b04 7235 7c00 6a05 6402  j.d...k.r5|.j.d.
-00001e80: 1900 6e04 7c00 6a05 6405 1900 7d02 7c00  ..n.|.j.d...}.|.
-00001e90: 6a03 4400 5d17 7d03 7c00 6a00 a007 7c01  j.D.].}.|.j...|.
-00001ea0: a004 7c03 7c00 6a06 7c03 7c02 6b02 7051  ..|.|.j.|.|.k.pQ
-00001eb0: 7402 7c00 6a03 8301 6405 6b02 a103 a101  t.|.j...d.k.....
-00001ec0: 0100 713d 7402 7c00 6a03 8301 6405 6b04  ..q=t.|.j...d.k.
-00001ed0: 72a6 7c00 6a00 6402 1900 7c00 6a00 6405  r.|.j.d...|.j.d.
-00001ee0: 1900 1700 7c00 5f00 7c00 6a00 7d04 6700  ....|._.|.j.}.g.
-00001ef0: 7c00 5f00 6700 7d05 7c04 4400 5d09 7d06  |._.g.}.|.D.].}.
-00001f00: 7c05 a007 7c06 6402 1900 a101 0100 7171  |...|.d.......qq
-00001f10: 7c05 4400 5d26 7d07 6700 7d08 7c04 4400  |.D.]&}.g.}.|.D.
-00001f20: 5d0f 7d06 7c07 7c06 6402 1900 6b02 7292  ].}.|.|.d...k.r.
-00001f30: 7c08 a007 7c06 6405 1900 a101 0100 7183  |...|.d.......q.
-00001f40: 7c07 7c08 6602 7d09 7c09 7c00 6a00 7600  |.|.f.}.|.|.j.v.
-00001f50: 729d 717d 7c00 6a00 a007 7c09 a101 0100  r.q}|.j...|.....
-00001f60: 717d 6400 5300 6700 7d04 7c00 6a00 6402  q}d.S.g.}.|.j.d.
-00001f70: 1900 4400 5d10 7d0a 7c0a 6402 1900 7c0a  ..D.].}.|.d...|.
-00001f80: 6405 1900 6701 6602 7d06 7c04 a007 7c06  d...g.f.}.|...|.
-00001f90: a101 0100 71ad 7c04 7c00 5f00 6400 5300  ....q.|.|._.d.S.
-00001fa0: 2906 4e54 7201 0000 0063 0100 0000 0000  ).NTr....c......
-00001fb0: 0000 0000 0000 0200 0000 0500 0000 5300  ..............S.
-00001fc0: 0000 731e 0000 0067 007c 005d 0b7d 017c  ..s....g.|.].}.|
-00001fd0: 0164 0019 007c 0164 0119 0067 0166 0291  .d...|.d...g.f..
-00001fe0: 0271 0253 0029 0272 0100 0000 7205 0000  .q.S.).r....r...
-00001ff0: 0072 1000 0000 2902 da02 2e30 7241 0000  .r....)....0rA..
-00002000: 0072 1000 0000 7210 0000 0072 1100 0000  .r....r....r....
-00002010: da0a 3c6c 6973 7463 6f6d 703e 5801 0000  ..<listcomp>X...
-00002020: 7302 0000 001e 007a 3754 7572 6e2e 7570  s......z7Turn.up
-00002030: 6461 7465 506f 7373 6962 6c65 4d6f 7665  datePossibleMove
-00002040: 7348 756d 616e 466f 726d 6174 2e3c 6c6f  sHumanFormat.<lo
-00002050: 6361 6c73 3e2e 3c6c 6973 7463 6f6d 703e  cals>.<listcomp>
-00002060: 7205 0000 0029 0872 5900 0000 7257 0000  r....).rY...rW..
-00002070: 0072 1500 0000 7258 0000 0072 4b00 0000  .r....rX...rK...
-00002080: 720c 0000 0072 0d00 0000 7245 0000 0029  r....r....rE...)
-00002090: 0b72 3400 0000 7225 0000 0072 4e00 0000  .r4...r%...rN...
-000020a0: 720c 0000 005a 1077 6f72 6b69 6e67 4d6f  r....Z.workingMo
-000020b0: 7665 734c 6973 745a 0b73 7461 7274 506f  vesListZ.startPo
-000020c0: 696e 7473 7241 0000 005a 0a73 7461 7274  intsrA...Z.start
-000020d0: 506f 696e 745a 066e 756d 4669 6e5a 0966  PointZ.numFinZ.f
-000020e0: 696e 616c 4c69 7374 5a0c 706f 7373 6962  inalListZ.possib
-000020f0: 6c65 4d6f 7665 7210 0000 0072 1000 0000  leMover....r....
-00002100: 7211 0000 00da 1e75 7064 6174 6550 6f73  r......updatePos
-00002110: 7369 626c 654d 6f76 6573 4875 6d61 6e46  sibleMovesHumanF
-00002120: 6f72 6d61 7452 0100 0073 4000 0000 0603  ormatR...s@.....
-00002130: 1801 1801 1601 2802 0a01 0601 2001 06ff  ......(..... ...
-00002140: 0e02 1601 0601 0601 0401 0801 1001 0801  ................
-00002150: 0401 0801 0c01 0e01 0280 0801 0a01 0201  ................
-00002160: 0e02 04f7 040b 0e01 1201 0c01 0a01 7a23  ..............z#
-00002170: 5475 726e 2e75 7064 6174 6550 6f73 7369  Turn.updatePossi
-00002180: 626c 654d 6f76 6573 4875 6d61 6e46 6f72  bleMovesHumanFor
-00002190: 6d61 7463 0200 0000 0000 0000 0000 0000  matc............
-000021a0: 0200 0000 0400 0000 4300 0000 7316 0000  ........C...s...
-000021b0: 007c 01a0 007c 006a 017c 006a 02a1 027c  .|...|.j.|.j...|
-000021c0: 005f 0364 0053 0072 1300 0000 2904 724f  ._.d.S.r....).rO
-000021d0: 0000 0072 0d00 0000 720c 0000 0072 5900  ...r....r....rY.
-000021e0: 0000 a902 7234 0000 0072 2500 0000 7210  ....r4...r%...r.
-000021f0: 0000 0072 1000 0000 7211 0000 00da 2175  ...r....r.....!u
-00002200: 7064 6174 6550 6f73 7369 626c 654d 6f76  pdatePossibleMov
-00002210: 6573 5374 616e 6461 7264 466f 726d 6174  esStandardFormat
-00002220: 7601 0000 f302 0000 0016 027a 2654 7572  v..........z&Tur
-00002230: 6e2e 7570 6461 7465 506f 7373 6962 6c65  n.updatePossible
-00002240: 4d6f 7665 7353 7461 6e64 6172 6446 6f72  MovesStandardFor
-00002250: 6d61 7463 0200 0000 0000 0000 0000 0000  matc............
-00002260: 0200 0000 0400 0000 4300 0000 7316 0000  ........C...s...
-00002270: 0074 007c 006a 017c 017c 006a 0283 037c  .t.|.j.|.|.j...|
-00002280: 005f 0364 0053 0072 1300 0000 2904 7202  ._.d.S.r....).r.
-00002290: 0000 0072 5900 0000 720d 0000 0072 5a00  ...rY...r....rZ.
-000022a0: 0000 725e 0000 0072 1000 0000 7210 0000  ..r^...r....r...
-000022b0: 0072 1100 0000 da0e 666f 726d 5370 7269  .r......formSpri
-000022c0: 7465 4c69 7374 7a01 0000 7260 0000 007a  teListz...r`...z
-000022d0: 1354 7572 6e2e 666f 726d 5370 7269 7465  .Turn.formSprite
-000022e0: 4c69 7374 2902 4e46 2908 7250 0000 0072  List).NF).rP...r
-000022f0: 5100 0000 7252 0000 0072 3500 0000 7225  Q...rR...r5...r%
-00002300: 0000 0072 5d00 0000 725f 0000 0072 6100  ...r]...r_...ra.
-00002310: 0000 7210 0000 0072 1000 0000 7210 0000  ..r....r....r...
-00002320: 0072 1100 0000 7253 0000 0036 0100 0073  .r....rS...6...s
-00002330: 1200 0000 0800 0a01 021b 0201 0aff 0224  ...............$
-00002340: 0201 0aff 0c04 7253 0000 0029 0e72 4c00  ......rS...).rL.
-00002350: 0000 7218 0000 005a 134d 6169 6e5f 4669  ..r....Z.Main_Fi
-00002360: 6c65 732e 4772 6170 6869 6373 7202 0000  les.Graphicsr...
-00002370: 0072 0300 0000 da13 4d6f 6475 6c65 4e6f  .r......ModuleNo
-00002380: 7446 6f75 6e64 4572 726f 725a 2577 696c  tFoundErrorZ%wil
-00002390: 6c73 655f 6261 636b 6761 6d6d 6f6e 2e4d  lse_backgammon.M
-000023a0: 6169 6e5f 4669 6c65 732e 4772 6170 6869  ain_Files.Graphi
-000023b0: 6373 7212 0000 0072 1600 0000 721a 0000  csr....r....r...
-000023c0: 0072 2100 0000 7224 0000 0072 2500 0000  .r!...r$...r%...
-000023d0: 7253 0000 0072 1000 0000 7210 0000 0072  rS...r....r....r
-000023e0: 1000 0000 7211 0000 00da 083c 6d6f 6475  ....r......<modu
-000023f0: 6c65 3e01 0000 0073 1e00 0000 0800 0801  le>....s........
-00002400: 0202 1401 0c01 1401 02ff 0805 080d 0804  ................
-00002410: 0806 0814 0e07 007f 127a                 .........z
+000005b0: 0884 005a 0564 0964 0a84 005a 0664 1a64  ...Z.d.d...Z.d.d
+000005c0: 0c64 0d84 015a 0764 1a64 0e64 0f84 015a  .d...Z.d.d.d...Z
+000005d0: 0864 1064 1184 005a 0964 1264 1384 005a  .d.d...Z.d.d...Z
+000005e0: 0a64 1464 1584 005a 0b64 1664 1784 005a  .d.d...Z.d.d...Z
+000005f0: 0c64 0153 0029 1bda 0542 6f61 7264 4eda  .d.S.)...BoardN.
+00000600: 0672 6574 7572 6e63 0200 0000 0000 0000  .returnc........
+00000610: 0000 0000 0200 0000 0200 0000 4300 0000  ............C...
+00000620: 733e 0000 007c 0164 0075 0072 0867 0064  s>...|.d.u.r.g.d
+00000630: 01a2 016e 017c 017c 005f 0064 0264 0267  ...n.|.|._.d.d.g
+00000640: 027c 005f 0164 0364 0467 027c 005f 0264  .|._.d.d.g.|._.d
+00000650: 0564 0567 027c 005f 0364 007c 005f 0464  .d.g.|._.d.|._.d
+00000660: 0053 00a9 064e 291c e9fe ffff ff72 0100  .S...N)......r..
+00000670: 0000 7201 0000 0072 0100 0000 7201 0000  ..r....r....r...
+00000680: 00e9 0500 0000 7201 0000 00e9 0300 0000  ......r.........
+00000690: 7201 0000 0072 0100 0000 7201 0000 00e9  r....r....r.....
+000006a0: fbff ffff 7229 0000 0072 0100 0000 7201  ....r)...r....r.
+000006b0: 0000 0072 0100 0000 e9fd ffff ff72 0100  ...r.........r..
+000006c0: 0000 722b 0000 0072 0100 0000 7201 0000  ..r+...r....r...
+000006d0: 0072 0100 0000 7201 0000 00e9 0200 0000  .r....r.........
+000006e0: 7201 0000 0072 0100 0000 7201 0000 0072  r....r....r....r
+000006f0: 0100 0000 e9a7 0000 0072 0500 0000 721b  .........r....r.
+00000700: 0000 0046 a905 721f 0000 00da 0370 6970  ...F..r......pip
+00000710: da0a 6c61 7374 506f 696e 7473 da0d 6265  ..lastPoints..be
+00000720: 6172 4f66 6653 7461 7475 73da 0c4d 6f76  arOffStatus..Mov
+00000730: 654c 696e 6544 6174 6129 02da 0473 656c  eLineData)...sel
+00000740: 665a 0d70 6f73 6974 696f 6e5f 6c69 7374  fZ.position_list
+00000750: 7210 0000 0072 1000 0000 7211 0000 00da  r....r....r.....
+00000760: 085f 5f69 6e69 745f 5f3e 0000 0073 0a00  .__init__>...s..
+00000770: 0000 1601 0a04 0a01 0a01 0a01 7a0e 426f  ............z.Bo
+00000780: 6172 642e 5f5f 696e 6974 5f5f 6301 0000  ard.__init__c...
+00000790: 0000 0000 0000 0000 0001 0000 0002 0000  ................
+000007a0: 0043 0000 0073 3200 0000 6700 6401 a201  .C...s2...g.d...
+000007b0: 7c00 5f00 6402 6402 6702 7c00 5f01 6403  |._.d.d.g.|._.d.
+000007c0: 6404 6702 7c00 5f02 6405 6405 6702 7c00  d.g.|._.d.d.g.|.
+000007d0: 5f03 6400 7c00 5f04 6400 5300 7227 0000  _.d.|._.d.S.r'..
+000007e0: 0072 2f00 0000 a901 7234 0000 0072 1000  .r/.....r4...r..
+000007f0: 0000 7210 0000 0072 1100 0000 da11 7365  ..r....r......se
+00000800: 7453 7461 7274 506f 7369 7469 6f6e 7348  tStartPositionsH
+00000810: 0000 0073 0a00 0000 0a01 0a04 0a01 0a01  ...s............
+00000820: 0a01 7a17 426f 6172 642e 7365 7453 7461  ..z.Board.setSta
+00000830: 7274 506f 7369 7469 6f6e 7363 0100 0000  rtPositionsc....
+00000840: 0000 0000 0000 0000 0400 0000 0600 0000  ................
+00000850: 4300 0000 7396 0000 0064 017d 0164 017d  C...s....d.}.d.}
+00000860: 0274 0064 0283 0144 005d 297d 037c 006a  .t.d...D.])}.|.j
+00000870: 017c 0319 0064 016b 0472 1d7c 027c 0364  .|...d.k.r.|.|.d
+00000880: 0317 007c 006a 017c 0319 0014 0037 007d  ...|.j.|.....7.}
+00000890: 0271 087c 006a 017c 0319 0064 016b 0072  .q.|.j.|...d.k.r
+000008a0: 317c 0164 027c 0318 0074 027c 006a 017c  1|.d.|...t.|.j.|
+000008b0: 0319 0083 0114 0037 007d 0171 087c 0164  .......7.}.q.|.d
+000008c0: 047c 006a 0164 0219 0014 0037 007d 017c  .|.j.d.....7.}.|
+000008d0: 0264 047c 006a 0164 0419 0014 0037 007d  .d.|.j.d.....7.}
+000008e0: 027c 017c 0266 027c 005f 0364 0053 00a9  .|.|.f.|._.d.S..
+000008f0: 054e 7201 0000 0072 1b00 0000 7205 0000  .Nr....r....r...
+00000900: 0072 0600 0000 2904 7223 0000 0072 1f00  .r....).r#...r..
+00000910: 0000 da03 6162 7372 3000 0000 a904 7234  ....absr0.....r4
+00000920: 0000 005a 0670 315f 7069 705a 0670 325f  ...Z.p1_pipZ.p2_
+00000930: 7069 70da 0169 7210 0000 0072 1000 0000  pip..ir....r....
+00000940: 7211 0000 00da 0975 7064 6174 6550 6970  r......updatePip
+00000950: 5200 0000 7316 0000 0004 0104 010c 010e  R...s...........
+00000960: 0118 010e 011a 0102 8012 0112 010e 017a  ...............z
+00000970: 0f42 6f61 7264 2e75 7064 6174 6550 6970  .Board.updatePip
+00000980: 6301 0000 0000 0000 0000 0000 0004 0000  c...............
+00000990: 0006 0000 0043 0000 0073 9000 0000 6401  .....C...s....d.
+000009a0: 7d01 6401 7d02 7400 6402 8301 4400 5d29  }.d.}.t.d...D.])
+000009b0: 7d03 7c00 6a01 7c03 1900 6401 6b04 721d  }.|.j.|...d.k.r.
+000009c0: 7c02 7c03 6403 1700 7c00 6a01 7c03 1900  |.|.d...|.j.|...
+000009d0: 1400 3700 7d02 7108 7c00 6a01 7c03 1900  ..7.}.q.|.j.|...
+000009e0: 6401 6b00 7231 7c01 6402 7c03 1800 7402  d.k.r1|.d.|...t.
+000009f0: 7c00 6a01 7c03 1900 8301 1400 3700 7d01  |.j.|.......7.}.
+00000a00: 7108 7c01 6404 7c00 6a01 6402 1900 1400  q.|.d.|.j.d.....
+00000a10: 3700 7d01 7c02 6404 7c00 6a01 6404 1900  7.}.|.d.|.j.d...
+00000a20: 1400 3700 7d02 7c01 7c02 6602 5300 7238  ..7.}.|.|.f.S.r8
+00000a30: 0000 0029 0372 2300 0000 721f 0000 0072  ...).r#...r....r
+00000a40: 3900 0000 723a 0000 0072 1000 0000 7210  9...r:...r....r.
+00000a50: 0000 0072 1100 0000 da09 7265 7475 726e  ...r......return
+00000a60: 5069 705e 0000 0073 1600 0000 0401 0401  Pip^...s........
+00000a70: 0c01 0e01 1801 0e01 1a01 0280 1201 1201  ................
+00000a80: 0801 7a0f 426f 6172 642e 7265 7475 726e  ..z.Board.return
+00000a90: 5069 7046 6304 0000 0000 0000 0000 0000  PipFc...........
+00000aa0: 0006 0000 0004 0000 0043 0000 0073 0c02  .........C...s..
+00000ab0: 0000 7c01 6401 1900 6402 6b02 725b 7c01  ..|.d...d.k.r[|.
+00000ac0: 6403 1900 6403 1800 7d04 7c00 6a00 6404  d...d...}.|.j.d.
+00000ad0: 7c02 1700 0500 1900 6403 3800 0300 3c00  |.......d.8...<.
+00000ae0: 7c02 6403 6b02 723b 7c00 6a00 7c04 1900  |.d.k.r;|.j.|...
+00000af0: 6401 6b04 7231 6405 7c00 6a00 7c04 3c00  d.k.r1d.|.j.|.<.
+00000b00: 7c00 6a00 6406 0500 1900 6403 3700 0300  |.j.d.....d.7...
+00000b10: 3c00 6ebf 7c00 6a00 7c04 0500 1900 6403  <.n.|.j.|.....d.
+00000b20: 3800 0300 3c00 6eb5 7c00 6a00 7c04 1900  8...<.n.|.j.|...
+00000b30: 6401 6b00 7251 6403 7c00 6a00 7c04 3c00  d.k.rQd.|.j.|.<.
+00000b40: 7c00 6a00 6407 0500 1900 6403 3700 0300  |.j.d.....d.7...
+00000b50: 3c00 6e9f 7c00 6a00 7c04 0500 1900 6403  <.n.|.j.|.....d.
+00000b60: 3700 0300 3c00 6e95 7c01 6403 1900 6408  7...<.n.|.d...d.
+00000b70: 6b02 728a 7c01 6401 1900 6403 1800 7d05  k.r.|.d...d...}.
+00000b80: 7c02 6403 6b02 7275 7c00 6a00 7c05 0500  |.d.k.ru|.j.|...
+00000b90: 1900 6403 3700 0300 3c00 6e09 7c00 6a00  ..d.7...<.n.|.j.
+00000ba0: 7c05 0500 1900 6403 3800 0300 3c00 7c00  |.....d.8...<.|.
+00000bb0: 6a00 6406 7c02 1700 0500 1900 6403 3700  j.d.|.......d.7.
+00000bc0: 0300 3c00 6e66 7c01 6403 1900 6403 1800  ..<.nf|.d...d...
+00000bd0: 7d04 7c01 6401 1900 6403 1800 7d05 7c02  }.|.d...d...}.|.
+00000be0: 6403 6b02 72a4 7c00 6a00 7c05 0500 1900  d.k.r.|.j.|.....
+00000bf0: 6403 3700 0300 3c00 6e09 7c00 6a00 7c05  d.7...<.n.|.j.|.
+00000c00: 0500 1900 6403 3800 0300 3c00 7c02 6403  ....d.8...<.|.d.
+00000c10: 6b02 72d1 7c00 6a00 7c04 1900 6401 6b04  k.r.|.j.|...d.k.
+00000c20: 72c7 6405 7c00 6a00 7c04 3c00 7c00 6a00  r.d.|.j.|.<.|.j.
+00000c30: 6406 0500 1900 6403 3700 0300 3c00 6e29  d.....d.7...<.n)
+00000c40: 7c00 6a00 7c04 0500 1900 6403 3800 0300  |.j.|.....d.8...
+00000c50: 3c00 6e1f 7c00 6a00 7c04 1900 6401 6b00  <.n.|.j.|...d.k.
+00000c60: 72e7 6403 7c00 6a00 7c04 3c00 7c00 6a00  r.d.|.j.|.<.|.j.
+00000c70: 6407 0500 1900 6403 3700 0300 3c00 6e09  d.....d.7...<.n.
+00000c80: 7c00 6a00 7c04 0500 1900 6403 3700 0300  |.j.|.....d.7...
+00000c90: 3c00 7c03 6409 6b02 9001 7204 7c00 a001  <.|.d.k...r.|...
+00000ca0: a100 0100 7c00 a002 7c02 a101 0100 7c00  ....|...|.....|.
+00000cb0: a003 a100 0100 6400 5300 6400 5300 290a  ......d.S.d.S.).
+00000cc0: 4e72 0100 0000 7204 0000 0072 0500 0000  Nr....r....r....
+00000cd0: e917 0000 0072 0800 0000 7206 0000 0072  .....r....r....r
+00000ce0: 1b00 0000 7207 0000 0046 2904 721f 0000  ....r....F).r...
+00000cf0: 0072 3c00 0000 da17 7570 6461 7465 4c61  .r<.....updateLa
+00000d00: 7374 4f63 6375 7069 6564 506f 696e 74da  stOccupiedPoint.
+00000d10: 1375 7064 6174 6542 6561 724f 6666 5374  .updateBearOffSt
+00000d20: 6174 7573 2906 7234 0000 00da 046d 6f76  atus).r4.....mov
+00000d30: 6572 0d00 0000 5a0d 6672 6f6d 4d61 6b65  er....Z.fromMake
+00000d40: 4d6f 7665 735a 0d65 6e64 506f 696e 7449  MovesZ.endPointI
+00000d50: 6e64 6578 5a0f 7374 6172 7450 6f69 6e74  ndexZ.startPoint
+00000d60: 496e 6465 7872 1000 0000 7210 0000 0072  Indexr....r....r
+00000d70: 1100 0000 da08 6d61 6b65 4d6f 7665 6a00  ......makeMovej.
+00000d80: 0000 734a 0000 000c 010c 0116 0108 010e  ..sJ............
+00000d90: 010a 0114 0114 020e 020a 0114 0114 020c  ................
+00000da0: 010c 0108 0114 0112 0218 010c 020c 0108  ................
+00000db0: 0114 0112 0208 010e 010a 0114 0114 020e  ................
+00000dc0: 020a 0114 0112 020a 0108 010a 010c 0104  ................
+00000dd0: fd7a 0e42 6f61 7264 2e6d 616b 654d 6f76  .z.Board.makeMov
+00000de0: 6563 0400 0000 0000 0000 0000 0000 0600  ec..............
+00000df0: 0000 0600 0000 4300 0000 7398 0000 0067  ......C...s....g
+00000e00: 007d 0474 007c 0183 0164 016b 0472 2274  .}.t.|...d.k.r"t
+00000e10: 017c 0164 0119 0083 0174 026b 0272 227c  .|.d.....t.k.r"|
+00000e20: 00a0 037c 017c 0264 02a1 0301 007c 0364  ...|.|.d.....|.d
+00000e30: 026b 0272 2174 047c 017c 0083 027c 005f  .k.r!t.|.|...|._
+00000e40: 056e 1b7c 0144 005d 157d 057c 00a0 037c  .n.|.D.].}.|...|
+00000e50: 057c 0264 02a1 0301 007c 0364 026b 0272  .|.d.....|.d.k.r
+00000e60: 397c 04a0 0674 047c 057c 0083 02a1 0101  9|...t.|.|......
+00000e70: 0071 247c 047c 005f 057c 00a0 07a1 0001  .q$|.|._.|......
+00000e80: 007c 00a0 087c 02a1 0101 007c 00a0 09a1  .|...|.....|....
+00000e90: 0001 0064 0053 0029 034e 7201 0000 0054  ...d.S.).Nr....T
+00000ea0: 290a 7215 0000 00da 0474 7970 65da 0369  ).r......type..i
+00000eb0: 6e74 7242 0000 0072 0300 0000 7233 0000  ntrB...r....r3..
+00000ec0: 00da 0661 7070 656e 6472 3c00 0000 723f  ...appendr<...r?
+00000ed0: 0000 0072 4000 0000 2906 7234 0000 005a  ...r@...).r4...Z
+00000ee0: 056d 6f76 6573 720d 0000 005a 0e75 7064  .movesr....Z.upd
+00000ef0: 6174 654c 696e 6544 6174 6172 3300 0000  ateLineDatar3...
+00000f00: 7241 0000 0072 1000 0000 7210 0000 0072  rA...r....r....r
+00000f10: 1100 0000 da09 6d61 6b65 4d6f 7665 7399  ......makeMoves.
+00000f20: 0000 0073 1e00 0000 0401 1c01 0e01 0801  ...s............
+00000f30: 0c01 0280 0802 0e01 0801 1001 0280 0601  ................
+00000f40: 0801 0a01 0c01 7a0f 426f 6172 642e 6d61  ......z.Board.ma
+00000f50: 6b65 4d6f 7665 7363 0200 0000 0000 0000  keMovesc........
+00000f60: 0000 0000 0300 0000 0400 0000 4300 0000  ............C...
+00000f70: 7378 0000 007c 0164 016b 0272 2074 0064  sx...|.d.k.r t.d
+00000f80: 0264 0364 0183 0344 005d 137d 027c 006a  .d.d...D.].}.|.j
+00000f90: 017c 0219 0064 026b 0072 1d7c 0264 0117  .|...d.k.r.|.d..
+00000fa0: 007c 006a 0264 023c 0001 0064 0053 0071  .|.j.d.<...d.S.q
+00000fb0: 0a64 0053 0074 0064 0464 0564 0583 0344  .d.S.t.d.d.d...D
+00000fc0: 005d 137d 027c 006a 017c 0219 0064 026b  .].}.|.j.|...d.k
+00000fd0: 0472 397c 0264 0117 007c 006a 0264 013c  .r9|.d...|.j.d.<
+00000fe0: 0001 0064 0053 0071 2664 0053 0029 064e  ...d.S.q&d.S.).N
+00000ff0: 7205 0000 0072 0100 0000 721b 0000 0072  r....r....r....r
+00001000: 3e00 0000 7208 0000 0029 0372 2300 0000  >...r....).r#...
+00001010: 721f 0000 0072 3100 0000 2903 7234 0000  r....r1...).r4..
+00001020: 0072 0d00 0000 da05 696e 6465 7872 1000  .r......indexr..
+00001030: 0000 7210 0000 0072 1100 0000 723f 0000  ..r....r....r?..
+00001040: 00a9 0000 0073 1a00 0000 0801 1001 0e01  .....s..........
+00001050: 0e01 0601 02fe 04ff 1005 0e01 0e01 0601  ................
+00001060: 02fe 04ff 7a1d 426f 6172 642e 7570 6461  ....z.Board.upda
+00001070: 7465 4c61 7374 4f63 6375 7069 6564 506f  teLastOccupiedPo
+00001080: 696e 7463 0100 0000 0000 0000 0000 0000  intc............
+00001090: 0100 0000 0300 0000 4300 0000 7350 0000  ........C...sP..
+000010a0: 007c 006a 0064 0119 0073 0c7c 006a 0164  .|.j.d...s.|.j.d
+000010b0: 0119 0064 026b 0472 0e64 036e 0164 047c  ...d.k.r.d.n.d.|
+000010c0: 006a 0064 013c 007c 006a 0064 0519 0073  .j.d.<.|.j.d...s
+000010d0: 1f7c 006a 0164 0519 0064 066b 0072 2164  .|.j.d...d.k.r!d
+000010e0: 036e 0164 047c 006a 0064 053c 0064 0053  .n.d.|.j.d.<.d.S
+000010f0: 0029 074e 7201 0000 00e9 1200 0000 5446  .).Nr.........TF
+00001100: 7205 0000 0072 2200 0000 2902 7232 0000  r....r"...).r2..
+00001110: 0072 3100 0000 7236 0000 0072 1000 0000  .r1...r6...r....
+00001120: 7210 0000 0072 1100 0000 7240 0000 00b5  r....r....r@....
+00001130: 0000 0073 0400 0000 2601 2a01 7a19 426f  ...s....&.*.z.Bo
+00001140: 6172 642e 7570 6461 7465 4265 6172 4f66  ard.updateBearOf
+00001150: 6653 7461 7475 7363 0400 0000 0000 0000  fStatusc........
+00001160: 0000 0000 0700 0000 0600 0000 0300 0000  ................
+00001170: 73cc 0100 0067 007d 0487 0066 0164 0164  s....g.}...f.d.d
+00001180: 0284 087d 057c 0264 036b 0272 7988 006a  ...}.|.d.k.ry..j
+00001190: 0064 0419 0064 056b 0472 237c 057c 0164  .d...d.k.r#|.|.d
+000011a0: 0383 0264 066b 0272 217c 04a0 0164 077c  ...d.k.r!|...d.|
+000011b0: 0166 02a1 0101 007c 0453 0074 0264 0483  .f.....|.S.t.d..
+000011c0: 0144 005d 217d 0688 006a 007c 0619 0064  .D.]!}...j.|...d
+000011d0: 056b 0072 487c 057c 067c 0117 0064 0317  .k.rH|.|.|...d..
+000011e0: 0064 0383 0264 066b 0272 487c 04a0 017c  .d...d.k.rH|...|
+000011f0: 0664 0317 007c 067c 0117 0064 0317 0066  .d...|.|...d...f
+00001200: 02a1 0101 0071 2788 006a 0364 0519 0064  .....q'..j.d...d
+00001210: 066b 0272 7788 006a 0064 047c 0118 0019  .k.rw..j.d.|....
+00001220: 0064 056b 0072 627c 04a0 0164 087c 0118  .d.k.rb|...d.|..
+00001230: 0064 0966 02a1 0101 007c 0372 7788 006a  .d.f.....|.rw..j
+00001240: 0464 0519 0064 087c 0118 006b 0472 777c  .d...d.|...k.rw|
+00001250: 04a0 0188 006a 0464 0519 0064 0966 02a1  .....j.d...d.f..
+00001260: 0101 007c 0453 0088 006a 0064 0819 0064  ...|.S...j.d...d
+00001270: 056b 0472 947c 0564 087c 0118 0064 0a83  .k.r.|.d.|...d..
+00001280: 0264 066b 0272 927c 04a0 0164 0764 087c  .d.k.r.|...d.d.|
+00001290: 0118 0066 02a1 0101 007c 0453 0074 0264  ...f.....|.S.t.d
+000012a0: 0483 0144 005d 217d 0688 006a 007c 0619  ...D.]!}...j.|..
+000012b0: 0064 056b 0472 b97c 057c 067c 0118 0064  .d.k.r.|.|.|...d
+000012c0: 0317 0064 0a83 0264 066b 0272 b97c 04a0  ...d...d.k.r.|..
+000012d0: 017c 0664 0317 007c 067c 0118 0064 0317  .|.d...|.|...d..
+000012e0: 0066 02a1 0101 0071 9888 006a 0364 0319  .f.....q...j.d..
+000012f0: 0064 066b 0272 e488 006a 007c 0164 0318  .d.k.r...j.|.d..
+00001300: 0019 0064 056b 0472 d17c 04a0 017c 0164  ...d.k.r.|...|.d
+00001310: 0966 02a1 0101 007c 0372 e488 006a 0464  .f.....|.r...j.d
+00001320: 0319 007c 016b 0072 e47c 04a0 0188 006a  ...|.k.r.|.....j
+00001330: 0464 0319 0064 0966 02a1 0101 007c 0453  .d...d.f.....|.S
+00001340: 0029 0b4e 6302 0000 0000 0000 0000 0000  .).Nc...........
+00001350: 0003 0000 0003 0000 0013 0000 0073 9000  .............s..
+00001360: 0000 7c00 6401 6b04 7308 7c00 6402 6b00  ..|.d.k.s.|.d.k.
+00001370: 720a 6403 5300 7c01 6404 6b02 7210 6405  r.d.S.|.d.k.r.d.
+00001380: 6e01 6402 7d02 8800 6a00 7c00 6402 1800  n.d.}...j.|.d...
+00001390: 1900 6406 6b02 721d 6407 5300 8800 6a00  ..d.k.r.d.S...j.
+000013a0: 7c00 6402 1800 1900 6406 6b04 722c 7c01  |.d.....d.k.r,|.
+000013b0: 6404 6b02 722c 6407 5300 8800 6a00 7c00  d.k.r,d.S...j.|.
+000013c0: 6402 1800 1900 6406 6b00 723b 7c01 6402  d.....d.k.r;|.d.
+000013d0: 6b02 723b 6407 5300 8800 6a00 7c00 6402  k.r;d.S...j.|.d.
+000013e0: 1800 1900 7c02 6b02 7246 6407 5300 6400  ....|.k.rFd.S.d.
+000013f0: 5300 2908 4e72 1b00 0000 7205 0000 0046  S.).Nr....r....F
+00001400: 722d 0000 0072 0800 0000 7201 0000 0054  r-...r....r....T
+00001410: 2901 721f 0000 0029 03da 0570 6f69 6e74  ).r....)...point
+00001420: 720d 0000 005a 086f 7070 5661 6c75 6572  r....Z.oppValuer
+00001430: 3600 0000 7210 0000 0072 1100 0000 da09  6...r....r......
+00001440: 6361 6e4d 6f76 6554 6fbc 0000 0073 1800  canMoveTo....s..
+00001450: 0000 1001 0401 1001 1201 0401 1a01 0401  ................
+00001460: 1a01 0401 1201 0401 04ff 7a2a 426f 6172  ..........z*Boar
+00001470: 642e 7265 7475 726e 4d6f 7665 7346 6f72  d.returnMovesFor
+00001480: 4469 652e 3c6c 6f63 616c 733e 2e63 616e  Die.<locals>.can
+00001490: 4d6f 7665 546f 7205 0000 0072 1b00 0000  MoveTor....r....
+000014a0: 7201 0000 0054 7204 0000 0072 0600 0000  r....Tr....r....
+000014b0: 7207 0000 0072 2d00 0000 2905 721f 0000  r....r-...).r...
+000014c0: 0072 4500 0000 7223 0000 0072 3200 0000  .rE...r#...r2...
+000014d0: 7231 0000 0029 0772 3400 0000 720e 0000  r1...).r4...r...
+000014e0: 0072 0d00 0000 5a18 6973 4269 6767 6573  .r....Z.isBigges
+000014f0: 7444 6965 4f72 5365 636f 6e64 4d6f 7665  tDieOrSecondMove
+00001500: 5a08 6d6f 7665 4c69 7374 724a 0000 005a  Z.moveListrJ...Z
+00001510: 0a70 6f69 6e74 496e 6465 7872 1000 0000  .pointIndexr....
+00001520: 7236 0000 0072 1100 0000 da11 7265 7475  r6...r......retu
+00001530: 726e 4d6f 7665 7346 6f72 4469 65b9 0000  rnMovesForDie...
+00001540: 0073 4200 0000 0401 0c02 080d 0e01 0e01  .sB.............
+00001550: 0e01 041b 0ce7 0e01 1601 1a01 0280 0e01  ................
+00001560: 1201 1201 1601 1401 0411 0ef2 1201 1201  ................
+00001570: 040c 0cf6 0e01 1601 1a01 0280 0e01 1201  ................
+00001580: 0e01 1201 1401 0402 7a17 426f 6172 642e  ........z.Board.
+00001590: 7265 7475 726e 4d6f 7665 7346 6f72 4469  returnMovesForDi
+000015a0: 6563 0300 0000 0000 0000 0000 0000 1600  ec..............
+000015b0: 0000 0a00 0000 4300 0000 7320 0300 0067  ......C...s ...g
+000015c0: 007d 0367 007d 047c 0264 0119 007c 0264  .}.g.}.|.d...|.d
+000015d0: 0219 006b 0372 a97c 0264 0119 007c 0264  ...k.r.|.d...|.d
+000015e0: 0219 006b 0572 187c 0264 0119 006e 037c  ...k.r.|.d...n.|
+000015f0: 0264 0219 007d 0567 007d 067c 0244 005d  .d...}.g.}.|.D.]
+00001600: 0e7d 077c 06a0 007c 00a0 017c 077c 017c  .}.|...|...|.|.|
+00001610: 057c 076b 02a1 03a1 0101 0071 207c 0664  .|.k.......q |.d
+00001620: 0119 007c 0664 0219 0017 007d 067c 0644  ...|.d.....}.|.D
+00001630: 005d 6d7d 0874 02a0 037c 00a1 017d 097c  .]m}.t...|...}.|
+00001640: 09a0 047c 087c 01a1 0201 007c 096a 057c  ...|.|.....|.j.|
+00001650: 0164 0218 0019 0064 016b 0272 567c 0867  .d.....d.k.rV|.g
+00001660: 017d 037c 0302 0001 0053 0074 067c 0864  .}.|.....S.t.|.d
+00001670: 0119 007c 0864 0219 007c 027c 0183 047d  ...|.d...|.|...}
+00001680: 0a7c 0264 0219 007c 0a6b 0272 6b7c 0264  .|.d...|.k.rk|.d
+00001690: 0119 006e 037c 0264 0219 007d 0b7c 09a0  ...n.|.d...}.|..
+000016a0: 017c 0b7c 0164 03a1 037d 0c74 077c 0c83  .|.|.d...}.t.|..
+000016b0: 0164 016b 0272 827c 03a0 007c 08a1 0101  .d.k.r.|...|....
+000016c0: 0071 397c 0c44 005d 217d 0d74 02a0 037c  .q9|.D.]!}.t...|
+000016d0: 00a1 017d 0e7c 0ea0 087c 087c 0d66 027c  ...}.|...|.|.f.|
+000016e0: 01a1 0201 007c 0e6a 097c 0476 0172 a57c  .....|.j.|.v.r.|
+000016f0: 03a0 007c 087c 0d66 02a1 0101 007c 04a0  ...|.|.f.....|..
+00001700: 007c 0e6a 09a1 0101 0071 8471 397c 0353  .|.j.....q.q9|.S
+00001710: 007c 00a0 017c 0264 0119 007c 0164 03a1  .|...|.d...|.d..
+00001720: 037d 067c 0644 005d d97d 0f74 02a0 037c  .}.|.D.].}.t...|
+00001730: 00a1 017d 097c 09a0 047c 0f7c 01a1 0201  ...}.|...|.|....
+00001740: 007c 096a 057c 0164 0218 0019 0064 016b  .|.j.|.d.....d.k
+00001750: 0272 d17c 0f67 017d 037c 0302 0001 0053  .r.|.g.}.|.....S
+00001760: 007c 09a0 017c 0264 0119 007c 0164 03a1  .|...|.d...|.d..
+00001770: 037d 0c74 077c 0c83 0164 016b 0272 e67c  .}.t.|...d.k.r.|
+00001780: 03a0 007c 0fa1 0101 0071 b47c 0c44 005d  ...|.....q.|.D.]
+00001790: a47d 0d74 02a0 037c 09a1 017d 0e7c 0ea0  .}.t...|...}.|..
+000017a0: 047c 0d7c 01a1 0201 007c 0e6a 057c 0164  .|.|.....|.j.|.d
+000017b0: 0218 0019 0064 016b 0290 0172 077c 03a0  .....d.k...r.|..
+000017c0: 007c 0f7c 0d66 02a1 0101 0071 e87c 0ea0  .|.|.f.....q.|..
+000017d0: 017c 0264 0119 007c 0164 03a1 037d 1074  .|.d...|.d...}.t
+000017e0: 077c 1083 0164 016b 0290 0172 1f7c 03a0  .|...d.k...r.|..
+000017f0: 007c 0f7c 0d67 02a1 0101 0071 e87c 1044  .|.|.g.....q.|.D
+00001800: 005d 6a7d 1174 02a0 037c 0ea1 017d 127c  .]j}.t...|...}.|
+00001810: 12a0 047c 117c 01a1 0201 007c 0e6a 057c  ...|.|.....|.j.|
+00001820: 0164 0218 0019 0064 016b 0290 0172 467c  .d.....d.k...rF|
+00001830: 0f7c 0d7c 1166 0367 017d 037c 0302 0001  .|.|.f.g.}.|....
+00001840: 0002 0001 0002 0001 0053 007c 12a0 017c  .........S.|...|
+00001850: 0264 0119 007c 0164 03a1 037d 1374 077c  .d...|.d...}.t.|
+00001860: 1383 0164 016b 0290 0172 607c 03a0 007c  ...d.k...r`|...|
+00001870: 0f7c 0d7c 1167 03a1 0101 0090 0171 217c  .|.|.g.......q!|
+00001880: 1344 005d 277d 1474 02a0 037c 00a1 017d  .D.]'}.t...|...}
+00001890: 157c 15a0 087c 0f7c 0d7c 117c 1466 047c  .|...|.|.|.|.f.|
+000018a0: 01a1 0201 007c 156a 097c 0476 0190 0172  .....|.j.|.v...r
+000018b0: 887c 03a0 007c 0f7c 0d7c 117c 1466 04a1  .|...|.|.|.|.f..
+000018c0: 0101 007c 04a0 007c 156a 09a1 0101 0090  ...|...|.j......
+000018d0: 0171 6290 0171 2171 e871 b47c 0353 0029  .qb..q!q.q.|.S.)
+000018e0: 044e 7201 0000 0072 0500 0000 5429 0a72  .Nr....r....T).r
+000018f0: 4500 0000 724b 0000 00da 0463 6f70 79da  E...rK.....copy.
+00001900: 0864 6565 7063 6f70 7972 4200 0000 7230  .deepcopyrB...r0
+00001910: 0000 0072 1200 0000 7215 0000 0072 4600  ...r....r....rF.
+00001920: 0000 721f 0000 0029 1672 3400 0000 720d  ..r....).r4...r.
+00001930: 0000 0072 0c00 0000 5a09 5365 7175 656e  ...r....Z.Sequen
+00001940: 6365 735a 0945 6e64 426f 6172 6473 da09  cesZ.EndBoards..
+00001950: 6269 6767 6572 4469 655a 0a46 6972 7374  biggerDieZ.First
+00001960: 4d6f 7665 7372 0e00 0000 7241 0000 005a  Movesr....rA...Z
+00001970: 0a61 6c67 6f42 6f61 7264 315a 0775 7365  .algoBoard1Z.use
+00001980: 6444 6965 5a09 756e 7573 6564 4469 655a  dDieZ.unusedDieZ
+00001990: 0b53 6563 6f6e 644d 6f76 6573 5a0a 7365  .SecondMovesZ.se
+000019a0: 636f 6e64 4d6f 7665 5a0a 616c 676f 426f  condMoveZ.algoBo
+000019b0: 6172 6432 5a09 6669 7273 744d 6f76 655a  ard2Z.firstMoveZ
+000019c0: 0a54 6869 7264 4d6f 7665 735a 0974 6869  .ThirdMovesZ.thi
+000019d0: 7264 4d6f 7665 5a0a 616c 676f 426f 6172  rdMoveZ.algoBoar
+000019e0: 6433 5a0a 466f 7274 684d 6f76 6573 5a09  d3Z.ForthMovesZ.
+000019f0: 666f 7274 684d 6f76 655a 0a61 6c67 6f42  forthMoveZ.algoB
+00001a00: 6f61 7264 3472 1000 0000 7210 0000 0072  oard4r....r....r
+00001a10: 1100 0000 da13 7265 7475 726e 4d6f 7665  ......returnMove
+00001a20: 5365 7175 656e 6365 73e9 0000 0073 8e00  Sequences....s..
+00001a30: 0000 0401 0401 1001 2001 0401 0803 1a01  ........ .......
+00001a40: 1001 0802 0a01 0c01 1201 0601 0801 1601  ................
+00001a50: 1c01 0e01 0c01 0a01 0201 0801 0a01 1001  ................
+00001a60: 0a01 0e01 0c01 0280 02fb 0406 1203 0801  ................
+00001a70: 0a01 0c01 1201 0601 0801 1201 0c01 0a01  ................
+00001a80: 0201 0801 0a01 0c01 1401 0e01 0201 1201  ................
+00001a90: 0e01 0e01 0201 0801 0a01 0c01 1401 0c01  ................
+00001aa0: 1001 1201 0e01 1001 0401 0801 0a01 1401  ................
+00001ab0: 0c01 1201 0c01 0480 04fb 02f6 02f6 041a  ................
+00001ac0: 7a19 426f 6172 642e 7265 7475 726e 4d6f  z.Board.returnMo
+00001ad0: 7665 5365 7175 656e 6365 7372 1300 0000  veSequencesr....
+00001ae0: 2902 7226 0000 004e 2901 4629 0dda 085f  ).r&...N).F)..._
+00001af0: 5f6e 616d 655f 5fda 0a5f 5f6d 6f64 756c  _name__..__modul
+00001b00: 655f 5fda 0c5f 5f71 7561 6c6e 616d 655f  e__..__qualname_
+00001b10: 5f72 3500 0000 7237 0000 0072 3c00 0000  _r5...r7...r<...
+00001b20: 723d 0000 0072 4200 0000 7246 0000 0072  r=...rB...rF...r
+00001b30: 3f00 0000 7240 0000 0072 4b00 0000 724f  ?...r@...rK...rO
+00001b40: 0000 0072 1000 0000 7210 0000 0072 1000  ...r....r....r..
+00001b50: 0000 7211 0000 0072 2500 0000 3d00 0000  ..r....r%...=...
+00001b60: 7316 0000 0008 000c 0108 0a08 0a08 0c0a  s...............
+00001b70: 0c0a 2f08 1008 0c08 040c 3072 2500 0000  ../.......0r%...
+00001b80: 6300 0000 0000 0000 0000 0000 0000 0000  c...............
+00001b90: 0003 0000 0040 0000 0073 3a00 0000 6500  .....@...s:...e.
+00001ba0: 5a01 6400 5a02 640c 6403 6404 8401 5a03  Z.d.Z.d.d.d...Z.
+00001bb0: 6405 6504 6602 6406 6407 8404 5a05 6405  d.e.f.d.d...Z.d.
+00001bc0: 6504 6602 6408 6409 8404 5a06 640a 640b  e.f.d.d...Z.d.d.
+00001bd0: 8400 5a07 6401 5300 290d da04 5475 726e  ..Z.d.S.)...Turn
+00001be0: 4e46 6305 0000 0000 0000 0000 0000 0005  NFc.............
+00001bf0: 0000 0003 0000 0043 0000 0073 d800 0000  .......C...s....
+00001c00: 7c01 7c00 5f00 7c02 7c00 5f01 7c03 6400  |.|._.|.|._.|.d.
+00001c10: 6b03 720c 7c03 6e02 7402 8300 7c00 5f03  k.r.|.n.t...|._.
+00001c20: 7c00 6a03 6401 1900 7c00 6a03 6402 1900  |.j.d...|.j.d...
+00001c30: 6b02 721c 6403 6e01 6404 7c00 5f04 6700  k.r.d.n.d.|._.g.
+00001c40: 7c00 5f05 6700 7c00 5f06 7c00 6a01 6405  |._.g.|._.|.j.d.
+00001c50: 6b02 7233 6700 7c00 5f07 6700 7c00 5f08  k.r3g.|._.g.|._.
+00001c60: 6700 7c00 5f09 7c04 7253 7c00 6a04 7253  g.|._.|.rS|.j.rS
+00001c70: 7c00 6a03 6401 1900 7c00 6a03 6402 1900  |.j.d...|.j.d...
+00001c80: 6b02 7250 7402 8300 7c00 5f03 7c00 6a03  k.rPt...|._.|.j.
+00001c90: 6401 1900 7c00 6a03 6402 1900 6b02 7342  d...|.j.d...k.sB
+00001ca0: 6404 7c00 5f04 7c00 6a04 6403 6b02 7263  d.|._.|.j.d.k.rc
+00001cb0: 7c00 6a03 6401 1900 6701 6406 1400 7c00  |.j.d...g.d...|.
+00001cc0: 5f05 6400 5300 740a a00b 7c00 6a03 a101  _.d.S.t...|.j...
+00001cd0: 7c00 5f05 6400 5300 2907 4e72 0100 0000  |._.d.S.).Nr....
+00001ce0: 7205 0000 0054 46da 0548 756d 616e e904  r....TF..Human..
+00001cf0: 0000 0029 0c72 0d00 0000 da0a 706c 6179  ...).r......play
+00001d00: 6572 5479 7065 721a 0000 0072 0c00 0000  erTyper....r....
+00001d10: da0c 646f 7562 6c65 735f 7475 726e da0b  ..doubles_turn..
+00001d20: 756e 7573 6564 5f64 6963 65da 1663 7572  unused_dice..cur
+00001d30: 7265 6e74 5f70 6f73 7369 626c 655f 6d6f  rent_possible_mo
+00001d40: 7665 73da 1273 7072 6974 6573 5f6d 6f76  ves..sprites_mov
+00001d50: 655f 7374 6172 745a 1073 7072 6974 6573  e_startZ.sprites
+00001d60: 5f6d 6f76 655f 656e 645a 0d73 7072 6974  _move_endZ.sprit
+00001d70: 655f 6163 7469 7665 724c 0000 0072 4d00  e_activerL...rM.
+00001d80: 0000 2905 7234 0000 0072 0d00 0000 7256  ..).r4...r....rV
+00001d90: 0000 0072 0c00 0000 5a05 4669 7273 7472  ...r....Z.Firstr
+00001da0: 1000 0000 7210 0000 0072 1100 0000 7235  ....r....r....r5
+00001db0: 0000 0033 0100 0073 2400 0000 0601 0601  ...3...s$.......
+00001dc0: 1402 1e01 0601 0602 0a02 0601 0601 0601  ................
+00001dd0: 0a03 1401 0801 14ff 0602 0a03 1601 1202  ................
+00001de0: 7a0d 5475 726e 2e5f 5f69 6e69 745f 5f72  z.Turn.__init__r
+00001df0: 2500 0000 6302 0000 0000 0000 0000 0000  %...c...........
+00001e00: 000b 0000 0009 0000 0043 0000 0073 8601  .........C...s..
+00001e10: 0000 6700 7c00 5f00 7c00 6a01 6401 6b02  ..g.|._.|.j.d.k.
+00001e20: 7226 7402 7c00 6a03 8301 6402 6b04 7226  r&t.|.j...d.k.r&
+00001e30: 7c01 a004 7c00 6a05 6402 1900 7c00 6a06  |...|.j.d...|.j.
+00001e40: 6401 a103 7c00 5f00 6403 6404 8400 7c00  d...|._.d.d...|.
+00001e50: 6a00 4400 8301 7c00 5f00 6400 5300 7c00  j.D...|._.d.S.|.
+00001e60: 6a05 6402 1900 7c00 6a05 6405 1900 6b04  j.d...|.j.d...k.
+00001e70: 7235 7c00 6a05 6402 1900 6e04 7c00 6a05  r5|.j.d...n.|.j.
+00001e80: 6405 1900 7d02 7c00 6a03 4400 5d17 7d03  d...}.|.j.D.].}.
+00001e90: 7c00 6a00 a007 7c01 a004 7c03 7c00 6a06  |.j...|...|.|.j.
+00001ea0: 7c03 7c02 6b02 7051 7402 7c00 6a03 8301  |.|.k.pQt.|.j...
+00001eb0: 6405 6b02 a103 a101 0100 713d 7402 7c00  d.k.......q=t.|.
+00001ec0: 6a03 8301 6405 6b04 72a6 7c00 6a00 6402  j...d.k.r.|.j.d.
+00001ed0: 1900 7c00 6a00 6405 1900 1700 7c00 5f00  ..|.j.d.....|._.
+00001ee0: 7c00 6a00 7d04 6700 7c00 5f00 6700 7d05  |.j.}.g.|._.g.}.
+00001ef0: 7c04 4400 5d09 7d06 7c05 a007 7c06 6402  |.D.].}.|...|.d.
+00001f00: 1900 a101 0100 7171 7c05 4400 5d26 7d07  ......qq|.D.]&}.
+00001f10: 6700 7d08 7c04 4400 5d0f 7d06 7c07 7c06  g.}.|.D.].}.|.|.
+00001f20: 6402 1900 6b02 7292 7c08 a007 7c06 6405  d...k.r.|...|.d.
+00001f30: 1900 a101 0100 7183 7c07 7c08 6602 7d09  ......q.|.|.f.}.
+00001f40: 7c09 7c00 6a00 7600 729d 717d 7c00 6a00  |.|.j.v.r.q}|.j.
+00001f50: a007 7c09 a101 0100 717d 6400 5300 6700  ..|.....q}d.S.g.
+00001f60: 7d04 7c00 6a00 6402 1900 4400 5d10 7d0a  }.|.j.d...D.].}.
+00001f70: 7c0a 6402 1900 7c0a 6405 1900 6701 6602  |.d...|.d...g.f.
+00001f80: 7d06 7c04 a007 7c06 a101 0100 71ad 7c04  }.|...|.....q.|.
+00001f90: 7c00 5f00 6400 5300 2906 4e54 7201 0000  |._.d.S.).NTr...
+00001fa0: 0063 0100 0000 0000 0000 0000 0000 0200  .c..............
+00001fb0: 0000 0500 0000 5300 0000 731e 0000 0067  ......S...s....g
+00001fc0: 007c 005d 0b7d 017c 0164 0019 007c 0164  .|.].}.|.d...|.d
+00001fd0: 0119 0067 0166 0291 0271 0253 0029 0272  ...g.f...q.S.).r
+00001fe0: 0100 0000 7205 0000 0072 1000 0000 2902  ....r....r....).
+00001ff0: da02 2e30 7241 0000 0072 1000 0000 7210  ...0rA...r....r.
+00002000: 0000 0072 1100 0000 da0a 3c6c 6973 7463  ...r......<listc
+00002010: 6f6d 703e 5301 0000 7302 0000 001e 007a  omp>S...s......z
+00002020: 3754 7572 6e2e 7570 6461 7465 506f 7373  7Turn.updatePoss
+00002030: 6962 6c65 4d6f 7665 7348 756d 616e 466f  ibleMovesHumanFo
+00002040: 726d 6174 2e3c 6c6f 6361 6c73 3e2e 3c6c  rmat.<locals>.<l
+00002050: 6973 7463 6f6d 703e 7205 0000 0029 0872  istcomp>r....).r
+00002060: 5900 0000 7257 0000 0072 1500 0000 7258  Y...rW...r....rX
+00002070: 0000 0072 4b00 0000 720c 0000 0072 0d00  ...rK...r....r..
+00002080: 0000 7245 0000 0029 0b72 3400 0000 7225  ..rE...).r4...r%
+00002090: 0000 0072 4e00 0000 720c 0000 005a 1077  ...rN...r....Z.w
+000020a0: 6f72 6b69 6e67 4d6f 7665 734c 6973 745a  orkingMovesListZ
+000020b0: 0b73 7461 7274 506f 696e 7473 7241 0000  .startPointsrA..
+000020c0: 005a 0a73 7461 7274 506f 696e 745a 066e  .Z.startPointZ.n
+000020d0: 756d 4669 6e5a 0966 696e 616c 4c69 7374  umFinZ.finalList
+000020e0: 5a0c 706f 7373 6962 6c65 4d6f 7665 7210  Z.possibleMover.
+000020f0: 0000 0072 1000 0000 7211 0000 00da 1e75  ...r....r......u
+00002100: 7064 6174 6550 6f73 7369 626c 654d 6f76  pdatePossibleMov
+00002110: 6573 4875 6d61 6e46 6f72 6d61 744e 0100  esHumanFormatN..
+00002120: 0073 4000 0000 0602 1801 1801 1601 2802  .s@...........(.
+00002130: 0a01 0601 2001 06ff 0e02 1601 0601 0601  .... ...........
+00002140: 0401 0801 1001 0801 0401 0801 0c01 0e01  ................
+00002150: 0280 0801 0a01 0201 0e02 04f7 040b 0e01  ................
+00002160: 1201 0c01 0a01 7a23 5475 726e 2e75 7064  ......z#Turn.upd
+00002170: 6174 6550 6f73 7369 626c 654d 6f76 6573  atePossibleMoves
+00002180: 4875 6d61 6e46 6f72 6d61 7463 0200 0000  HumanFormatc....
+00002190: 0000 0000 0000 0000 0200 0000 0400 0000  ................
+000021a0: 4300 0000 7316 0000 007c 01a0 007c 006a  C...s....|...|.j
+000021b0: 017c 006a 02a1 027c 005f 0364 0053 0072  .|.j...|._.d.S.r
+000021c0: 1300 0000 2904 724f 0000 0072 0d00 0000  ....).rO...r....
+000021d0: 720c 0000 0072 5900 0000 a902 7234 0000  r....rY.....r4..
+000021e0: 0072 2500 0000 7210 0000 0072 1000 0000  .r%...r....r....
+000021f0: 7211 0000 00da 2175 7064 6174 6550 6f73  r.....!updatePos
+00002200: 7369 626c 654d 6f76 6573 5374 616e 6461  sibleMovesStanda
+00002210: 7264 466f 726d 6174 7101 0000 7302 0000  rdFormatq...s...
+00002220: 0016 017a 2654 7572 6e2e 7570 6461 7465  ...z&Turn.update
+00002230: 506f 7373 6962 6c65 4d6f 7665 7353 7461  PossibleMovesSta
+00002240: 6e64 6172 6446 6f72 6d61 7463 0200 0000  ndardFormatc....
+00002250: 0000 0000 0000 0000 0200 0000 0400 0000  ................
+00002260: 4300 0000 7316 0000 0074 007c 006a 017c  C...s....t.|.j.|
+00002270: 017c 006a 0283 037c 005f 0364 0053 0072  .|.j...|._.d.S.r
+00002280: 1300 0000 2904 7202 0000 0072 5900 0000  ....).r....rY...
+00002290: 720d 0000 0072 5a00 0000 725e 0000 0072  r....rZ...r^...r
+000022a0: 1000 0000 7210 0000 0072 1100 0000 da0e  ....r....r......
+000022b0: 666f 726d 5370 7269 7465 4c69 7374 7401  formSpriteListt.
+000022c0: 0000 7302 0000 0016 027a 1354 7572 6e2e  ..s......z.Turn.
+000022d0: 666f 726d 5370 7269 7465 4c69 7374 2902  formSpriteList).
+000022e0: 4e46 2908 7250 0000 0072 5100 0000 7252  NF).rP...rQ...rR
+000022f0: 0000 0072 3500 0000 7225 0000 0072 5d00  ...r5...r%...r].
+00002300: 0000 725f 0000 0072 6000 0000 7210 0000  ..r_...r`...r...
+00002310: 0072 1000 0000 7210 0000 0072 1100 0000  .r....r....r....
+00002320: 7253 0000 0032 0100 0073 0a00 0000 0800  rS...2...s......
+00002330: 0a01 0e1b 0e23 0c03 7253 0000 0029 0e72  .....#..rS...).r
+00002340: 4c00 0000 7218 0000 005a 134d 6169 6e5f  L...r....Z.Main_
+00002350: 4669 6c65 732e 4772 6170 6869 6373 7202  Files.Graphicsr.
+00002360: 0000 0072 0300 0000 da13 4d6f 6475 6c65  ...r......Module
+00002370: 4e6f 7446 6f75 6e64 4572 726f 725a 2577  NotFoundErrorZ%w
+00002380: 696c 6c73 655f 6261 636b 6761 6d6d 6f6e  illse_backgammon
+00002390: 2e4d 6169 6e5f 4669 6c65 732e 4772 6170  .Main_Files.Grap
+000023a0: 6869 6373 7212 0000 0072 1600 0000 721a  hicsr....r....r.
+000023b0: 0000 0072 2100 0000 7224 0000 0072 2500  ...r!...r$...r%.
+000023c0: 0000 7253 0000 0072 1000 0000 7210 0000  ..rS...r....r...
+000023d0: 0072 1000 0000 7211 0000 00da 083c 6d6f  .r....r......<mo
+000023e0: 6475 6c65 3e01 0000 0073 1e00 0000 0800  dule>....s......
+000023f0: 0801 0202 1401 0c01 1401 02ff 0805 080d  ................
+00002400: 0804 0806 0814 0e07 007f 1276            ...........v
```

### Comparing `willse_backgammon-0.0.1/src/willse_backgammon/Main_Files/__pycache__/Views.cpython-310.pyc` & `willse_backgammon-0.0.2/src/willse_backgammon/Main_Files/__pycache__/Views.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Sat Mar 23 17:14:23 2024 UTC, .py size: 48714 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-00000000: 6f0d 0d0a 0000 0000 ef0d ff65 4abe 0000  o..........eJ...
+00000000: 6f0d 0d0a 0000 0000 553a 0366 e6e6 0000  o.......U:.f....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 0008 0000 0040 0000 0073 4201 0000 6400  .....@...sB...d.
+00000020: 0008 0000 0040 0000 0073 7801 0000 6400  .....@...sx...d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a00 6400  d.l.Z.d.d.l.Z.d.
 00000040: 6401 6c02 5a02 7a14 6400 6402 6c03 6d04  d.l.Z.z.d.d.l.m.
 00000050: 5a04 0100 6400 6403 6c03 6d05 5a05 0100  Z...d.d.l.m.Z...
 00000060: 6400 6404 6c03 6d06 5a06 0100 5700 6e1b  d.d.l.m.Z...W.n.
 00000070: 0400 6507 793b 0100 0100 0100 6400 6402  ..e.y;......d.d.
 00000080: 6c08 6d04 5a04 0100 6400 6403 6c08 6d05  l.m.Z...d.d.l.m.
 00000090: 5a05 0100 6400 6404 6c08 6d06 5a06 0100  Z...d.d.l.m.Z...
@@ -16,2068 +16,2439 @@
 000000f0: 640d 640e 8400 640e 6500 6a09 8303 5a0e  d.d...d.e.j...Z.
 00000100: 4700 640f 6410 8400 6410 6500 6a09 8303  G.d.d...d.e.j...
 00000110: 5a0f 4700 6411 6412 8400 6412 6500 6a09  Z.G.d.d...d.e.j.
 00000120: 8303 5a10 4700 6413 6414 8400 6414 6500  ..Z.G.d.d...d.e.
 00000130: 6a09 8303 5a11 4700 6415 6416 8400 6416  j...Z.G.d.d...d.
 00000140: 6500 6a09 8303 5a12 4700 6417 6418 8400  e.j...Z.G.d.d...
 00000150: 6418 6500 6a09 8303 5a13 4700 6419 641a  d.e.j...Z.G.d.d.
-00000160: 8400 641a 6500 6a09 8303 5a14 6401 5300  ..d.e.j...Z.d.S.
-00000170: 291b e900 0000 004e 2901 da02 4149 2901  )......N)...AI).
-00000180: da05 4c6f 6769 6329 01da 0847 7261 7068  ..Logic)...Graph
-00000190: 6963 7363 0000 0000 0000 0000 0000 0000  icsc............
-000001a0: 0000 0000 0300 0000 0000 0000 f334 0000  .............4..
-000001b0: 0065 005a 0164 005a 0287 0066 0164 0164  .e.Z.d.Z...f.d.d
-000001c0: 0284 085a 0364 0364 0484 005a 0464 0564  ...Z.d.d...Z.d.d
-000001d0: 0684 005a 0564 0764 0884 005a 0687 0004  ...Z.d.d...Z....
-000001e0: 005a 0753 0029 09da 0c4d 6169 6e4d 656e  .Z.S.)...MainMen
-000001f0: 7556 6965 7763 0200 0000 0000 0000 0000  uViewc..........
-00000200: 0000 0e00 0000 0800 0000 0300 0000 73ba  ..............s.
-00000210: 0100 0074 0083 00a0 01a1 0001 007c 0188  ...t.........|..
-00000220: 005f 0274 036a 04a0 05a1 0088 005f 0688  ._.t.j......._..
-00000230: 006a 06a0 07a1 0001 0074 036a 04a0 08a1  .j.......t.j....
-00000240: 0088 005f 0974 036a 046a 0a64 0164 0264  ..._.t.j.j.d.d.d
-00000250: 0364 048d 037d 0288 006a 09a0 0b7c 026a  .d...}...j...|.j
-00000260: 0c64 0564 068d 01a1 0101 0074 036a 046a  .d.d.......t.j.j
-00000270: 0a64 0764 0864 0364 048d 037d 0388 006a  .d.d.d.d...}...j
-00000280: 09a0 0b7c 036a 0c64 0964 068d 01a1 0101  ...|.j.d.d......
-00000290: 0074 036a 046a 0d64 0a64 0b64 0c8d 027d  .t.j.j.d.d.d...}
-000002a0: 0474 036a 046a 0d64 0d64 0b64 0c8d 027d  .t.j.j.d.d.d...}
-000002b0: 0574 036a 046a 0d64 0e64 0b64 0c8d 027d  .t.j.j.d.d.d...}
-000002c0: 0674 036a 046a 0d64 0f64 0b64 0c8d 027d  .t.j.j.d.d.d...}
-000002d0: 0774 036a 046a 0d64 1064 0b64 0c8d 027d  .t.j.j.d.d.d...}
-000002e0: 0888 006a 09a0 0b7c 046a 0c64 0564 068d  ...j...|.j.d.d..
-000002f0: 01a1 0101 0088 006a 09a0 0b7c 056a 0c64  .......j...|.j.d
-00000300: 0564 068d 01a1 0101 0088 006a 09a0 0b7c  .d.........j...|
-00000310: 066a 0c64 0564 068d 01a1 0101 0088 006a  .j.d.d.........j
-00000320: 09a0 0b7c 076a 0c64 0564 068d 01a1 0101  ...|.j.d.d......
-00000330: 0088 006a 09a0 0b7c 086a 0c64 0564 068d  ...j...|.j.d.d..
-00000340: 01a1 0101 0088 006a 06a0 0b74 036a 046a  .......j...t.j.j
-00000350: 0e64 1164 1264 1388 006a 0964 148d 04a1  .d.d.d...j.d....
-00000360: 0101 007c 04a0 0f64 15a1 0187 0066 0164  ...|...d.....f.d
-00000370: 1664 1784 0883 017d 097c 05a0 0f64 15a1  .d.....}.|...d..
-00000380: 0164 1864 1984 0083 017d 0a7c 06a0 0f64  .d.d.....}.|...d
-00000390: 15a1 0187 0066 0164 1a64 1b84 0883 017d  .....f.d.d.....}
-000003a0: 0b7c 07a0 0f64 15a1 0187 0066 0164 1c64  .|...d.....f.d.d
-000003b0: 1d84 0883 017d 0c7c 08a0 0f64 15a1 0164  .....}.|...d...d
-000003c0: 1e64 1f84 0083 017d 0d64 0053 0029 204e  .d.....}.d.S.) N
-000003d0: da0a 4261 636b 6761 6d6d 6f6e e94b 0000  ..Backgammon.K..
-000003e0: 0029 03e9 ff00 0000 7209 0000 0072 0900  .)......r....r..
-000003f0: 0000 2903 da04 7465 7874 da09 666f 6e74  ..)...text..font
-00000400: 5f73 697a 65da 0a74 6578 745f 636f 6c6f  _size..text_colo
-00000410: 72e9 1400 0000 2901 da06 626f 7474 6f6d  r.....)...bottom
-00000420: 7a0d 6279 2057 696c 6c73 2045 7264 61e9  z.by Wills Erda.
-00000430: 1e00 0000 e928 0000 005a 0a53 696d 756c  .....(...Z.Simul
-00000440: 6174 696f 6ee9 2c01 0000 2902 720a 0000  ation.,...).r...
-00000450: 00da 0577 6964 7468 7a0a 4f6e 6520 506c  ...widthz.One Pl
-00000460: 6179 6572 7a0a 5477 6f20 506c 6179 6572  ayerz.Two Player
-00000470: da08 5365 7474 696e 6773 da04 5175 6974  ..Settings..Quit
-00000480: da08 6365 6e74 6572 5f78 da06 6365 6e74  ..center_x..cent
-00000490: 6572 7201 0000 0029 04da 0861 6e63 686f  err....)...ancho
-000004a0: 725f 78da 0861 6e63 686f 725f 79da 0761  r_x..anchor_y..a
-000004b0: 6c69 676e 5f79 da05 6368 696c 64da 086f  lign_y..child..o
-000004c0: 6e5f 636c 6963 6b63 0100 0000 0000 0000  n_clickc........
-000004d0: 0000 0000 0200 0000 0300 0000 1300 0000  ................
-000004e0: 7376 0000 0088 006a 006a 01a0 02a1 0001  sv.....j.j......
-000004f0: 0088 006a 006a 0364 0119 0064 026b 0272  ...j.j.d...d.k.r
-00000500: 1064 036e 0588 006a 006a 0364 0119 0088  .d.n...j.j.d....
-00000510: 006a 006a 0364 013c 0088 006a 006a 0364  .j.j.d.<...j.j.d
-00000520: 0419 0064 026b 0272 2464 036e 0588 006a  ...d.k.r$d.n...j
-00000530: 006a 0364 0419 0088 006a 006a 0364 043c  .j.d.....j.j.d.<
-00000540: 0074 0488 006a 0583 017d 0188 006a 00a0  .t...j...}...j..
-00000550: 067c 01a1 0101 0064 0053 0029 054e da06  .|.....d.S.).N..
-00000560: 4167 656e 7431 da05 4875 6d61 6efa 0454  Agent1..Human..T
-00000570: 5320 31da 0641 6765 6e74 3229 07da 0677  S 1..Agent2)...w
-00000580: 696e 646f 77da 094d 6169 6e42 6f61 7264  indow..MainBoard
-00000590: da11 7365 7453 7461 7274 506f 7369 7469  ..setStartPositi
-000005a0: 6f6e 73da 0873 6574 7469 6e67 73da 0b4d  ons..settings..M
-000005b0: 6169 6e53 696d 5669 6577 da0f 6261 636b  ainSimView..back
-000005c0: 6772 6f75 6e64 436f 6c6f 72da 0973 686f  groundColor..sho
-000005d0: 775f 7669 6577 2902 da05 6576 656e 74da  w_view)...event.
-000005e0: 0773 696d 5669 6577 a901 da04 7365 6c66  .simView....self
-000005f0: a900 fa54 643a 5c28 5729 202d 2043 6f64  ...Td:\(W) - Cod
-00000600: 655c 2857 2920 4261 636b 6761 6d6d 6f6e  e\(W) Backgammon
-00000610: 2050 726f 6a65 6374 2046 696c 6573 5c73   Project Files\s
-00000620: 7263 5c77 696c 6c73 655f 6261 636b 6761  rc\willse_backga
-00000630: 6d6d 6f6e 5c4d 6169 6e5f 4669 6c65 735c  mmon\Main_Files\
-00000640: 5669 6577 732e 7079 da0c 6f6e 5f63 6c69  Views.py..on_cli
-00000650: 636b 5f53 696d 2d00 0000 7312 0000 000c  ck_Sim-...s.....
-00000660: 0214 010a 010a ff14 020a 010a ff0a 0210  ................
-00000670: 017a 2b4d 6169 6e4d 656e 7556 6965 772e  .z+MainMenuView.
-00000680: 5f5f 696e 6974 5f5f 2e3c 6c6f 6361 6c73  __init__.<locals
-00000690: 3e2e 6f6e 5f63 6c69 636b 5f53 696d 6301  >.on_click_Simc.
-000006a0: 0000 0000 0000 0000 0000 0001 0000 0001  ................
-000006b0: 0000 0053 0000 0073 0400 0000 6400 5300  ...S...s....d.S.
-000006c0: a901 4e72 2b00 0000 a901 7227 0000 0072  ..Nr+.....r'...r
-000006d0: 2b00 0000 722b 0000 0072 2c00 0000 da12  +...r+...r,.....
-000006e0: 6f6e 5f63 6c69 636b 5f4f 6e65 506c 6179  on_click_OnePlay
-000006f0: 6572 3700 0000 7302 0000 0004 027a 314d  er7...s......z1M
-00000700: 6169 6e4d 656e 7556 6965 772e 5f5f 696e  ainMenuView.__in
-00000710: 6974 5f5f 2e3c 6c6f 6361 6c73 3e2e 6f6e  it__.<locals>.on
-00000720: 5f63 6c69 636b 5f4f 6e65 506c 6179 6572  _click_OnePlayer
-00000730: 6301 0000 0000 0000 0000 0000 0002 0000  c...............
-00000740: 0003 0000 0013 0000 0073 2600 0000 8800  .........s&.....
-00000750: 6a00 6a01 a002 a100 0100 7403 8800 6a04  j.j.......t...j.
-00000760: 8301 7d01 8800 6a00 a005 7c01 a101 0100  ..}...j...|.....
-00000770: 6400 5300 722e 0000 0029 0672 2000 0000  d.S.r....).r ...
-00000780: 7221 0000 0072 2200 0000 da0d 5374 6172  r!...r".....Star
-00000790: 745f 3250 5f56 6965 7772 2500 0000 7226  t_2P_Viewr%...r&
-000007a0: 0000 0029 0272 2700 0000 5a09 7374 6172  ...).r'...Z.star
-000007b0: 7456 6965 7772 2900 0000 722b 0000 0072  tViewr)...r+...r
-000007c0: 2c00 0000 da12 6f6e 5f63 6c69 636b 5f54  ,.....on_click_T
-000007d0: 776f 506c 6179 6572 3b00 0000 7306 0000  woPlayer;...s...
-000007e0: 000c 020a 0110 017a 314d 6169 6e4d 656e  .......z1MainMen
-000007f0: 7556 6965 772e 5f5f 696e 6974 5f5f 2e3c  uView.__init__.<
-00000800: 6c6f 6361 6c73 3e2e 6f6e 5f63 6c69 636b  locals>.on_click
-00000810: 5f54 776f 506c 6179 6572 6301 0000 0000  _TwoPlayerc.....
-00000820: 0000 0000 0000 0002 0000 0003 0000 0013  ................
-00000830: 0000 00f3 2200 0000 8800 8800 6a00 5f01  ....".......j._.
-00000840: 7402 8800 6a03 8301 7d01 8800 6a00 a004  t...j...}...j...
-00000850: 7c01 a101 0100 6400 5300 722e 0000 00a9  |.....d.S.r.....
-00000860: 0572 2000 0000 da08 6c61 7374 5061 6765  .r .....lastPage
-00000870: da0c 5365 7474 696e 6773 5669 6577 7225  ..SettingsViewr%
-00000880: 0000 0072 2600 0000 a902 7227 0000 005a  ...r&.....r'...Z
-00000890: 0c73 6574 7469 6e67 7356 6965 7772 2900  .settingsViewr).
-000008a0: 0000 722b 0000 0072 2c00 0000 da11 6f6e  ..r+...r,.....on
-000008b0: 5f63 6c69 636b 5f53 6574 7469 6e67 7341  _click_SettingsA
-000008c0: 0000 00f3 0600 0000 0802 0a01 1001 7a30  ..............z0
-000008d0: 4d61 696e 4d65 6e75 5669 6577 2e5f 5f69  MainMenuView.__i
-000008e0: 6e69 745f 5f2e 3c6c 6f63 616c 733e 2e6f  nit__.<locals>.o
-000008f0: 6e5f 636c 6963 6b5f 5365 7474 696e 6773  n_click_Settings
-00000900: 6301 0000 0000 0000 0000 0000 0001 0000  c...............
-00000910: 0002 0000 0053 0000 00f3 0c00 0000 7400  .....S........t.
-00000920: a001 a100 0100 6400 5300 722e 0000 00a9  ......d.S.r.....
-00000930: 02da 0661 7263 6164 65da 0c63 6c6f 7365  ...arcade..close
-00000940: 5f77 696e 646f 7772 2f00 0000 722b 0000  _windowr/...r+..
-00000950: 0072 2b00 0000 722c 0000 00da 0d6f 6e5f  .r+...r,.....on_
-00000960: 636c 6963 6b5f 5175 6974 4700 0000 f302  click_QuitG.....
-00000970: 0000 000c 027a 2c4d 6169 6e4d 656e 7556  .....z,MainMenuV
-00000980: 6965 772e 5f5f 696e 6974 5f5f 2e3c 6c6f  iew.__init__.<lo
-00000990: 6361 6c73 3e2e 6f6e 5f63 6c69 636b 5f51  cals>.on_click_Q
-000009a0: 7569 7429 10da 0573 7570 6572 da08 5f5f  uit)...super..__
-000009b0: 696e 6974 5f5f 7225 0000 0072 3c00 0000  init__r%...r<...
-000009c0: da03 6775 69da 0955 494d 616e 6167 6572  ..gui..UIManager
-000009d0: da07 6d61 6e61 6765 72da 0665 6e61 626c  ..manager..enabl
-000009e0: 65da 0b55 4942 6f78 4c61 796f 7574 5a05  e..UIBoxLayoutZ.
-000009f0: 765f 626f 78da 0755 494c 6162 656c da03  v_box..UILabel..
-00000a00: 6164 64da 1177 6974 685f 7370 6163 655f  add..with_space_
-00000a10: 6172 6f75 6e64 da0c 5549 466c 6174 4275  around..UIFlatBu
-00000a20: 7474 6f6e da0e 5549 416e 6368 6f72 5769  tton..UIAnchorWi
-00000a30: 6467 6574 7227 0000 0029 0e72 2a00 0000  dgetr'...).r*...
-00000a40: da10 6261 636b 6772 6f75 6e64 5f63 6f6c  ..background_col
-00000a50: 6f72 5a0a 7469 746c 655f 7465 7874 5a0d  orZ.title_textZ.
-00000a60: 7375 6274 6974 6c65 5f74 6578 745a 0a73  subtitle_textZ.s
-00000a70: 696d 5f62 7574 746f 6e5a 116f 6e65 5f70  im_buttonZ.one_p
-00000a80: 6c61 7965 725f 6275 7474 6f6e 5a11 7477  layer_buttonZ.tw
-00000a90: 6f5f 706c 6179 6572 5f62 7574 746f 6e5a  o_player_buttonZ
-00000aa0: 0f73 6574 7469 6e67 735f 6275 7474 6f6e  .settings_button
-00000ab0: 5a0b 7175 6974 5f62 7574 746f 6e72 2d00  Z.quit_buttonr-.
-00000ac0: 0000 7230 0000 0072 3200 0000 7238 0000  ..r0...r2...r8..
-00000ad0: 0072 3e00 0000 a901 da09 5f5f 636c 6173  .r>.......__clas
-00000ae0: 735f 5f72 2900 0000 722c 0000 0072 4100  s__r)...r,...rA.
-00000af0: 0000 1100 0000 733c 0000 000a 0106 010c  ......s<........
-00000b00: 020a 010c 0212 0214 0112 0114 0110 0210  ................
-00000b10: 0110 0110 0110 0114 0214 0114 0114 0114  ................
-00000b20: 011e 0208 020e 0108 090a 0108 030e 0108  ................
-00000b30: 050e 0108 050e 017a 154d 6169 6e4d 656e  .......z.MainMen
-00000b40: 7556 6965 772e 5f5f 696e 6974 5f5f 6301  uView.__init__c.
-00000b50: 0000 0000 0000 0000 0000 0001 0000 0003  ................
-00000b60: 0000 0043 0000 00f3 1a00 0000 7c00 6a00  ...C........|.j.
-00000b70: a001 a100 0100 7402 a003 7c00 6a04 a101  ......t...|.j...
-00000b80: 0100 6400 5300 722e 0000 00a9 0572 4400  ..d.S.r......rD.
-00000b90: 0000 7245 0000 0072 3c00 0000 da14 7365  ..rE...r<.....se
-00000ba0: 745f 6261 636b 6772 6f75 6e64 5f63 6f6c  t_background_col
-00000bb0: 6f72 7225 0000 0072 2900 0000 722b 0000  orr%...r)...r+..
-00000bc0: 0072 2b00 0000 722c 0000 00da 0c6f 6e5f  .r+...r,.....on_
-00000bd0: 7368 6f77 5f76 6965 774b 0000 00f3 0400  show_viewK......
-00000be0: 0000 0a01 1001 7a19 4d61 696e 4d65 6e75  ......z.MainMenu
-00000bf0: 5669 6577 2e6f 6e5f 7368 6f77 5f76 6965  View.on_show_vie
-00000c00: 7763 0100 0000 0000 0000 0000 0000 0100  wc..............
-00000c10: 0000 0200 0000 4300 0000 f30e 0000 007c  ......C........|
-00000c20: 006a 00a0 01a1 0001 0064 0053 0072 2e00  .j.......d.S.r..
-00000c30: 0000 a902 7244 0000 00da 0764 6973 6162  ....rD.....disab
-00000c40: 6c65 7229 0000 0072 2b00 0000 722b 0000  ler)...r+...r+..
-00000c50: 0072 2c00 0000 da0c 6f6e 5f68 6964 655f  .r,.....on_hide_
-00000c60: 7669 6577 4f00 0000 f302 0000 000e 017a  viewO..........z
-00000c70: 194d 6169 6e4d 656e 7556 6965 772e 6f6e  .MainMenuView.on
-00000c80: 5f68 6964 655f 7669 6577 6301 0000 0000  _hide_viewc.....
-00000c90: 0000 0000 0000 0001 0000 0002 0000 0043  ...............C
-00000ca0: 0000 00f3 1600 0000 7c00 a000 a100 0100  ........|.......
-00000cb0: 7c00 6a01 a002 a100 0100 6400 5300 722e  |.j.......d.S.r.
-00000cc0: 0000 00a9 03da 0563 6c65 6172 7244 0000  .......clearrD..
-00000cd0: 00da 0464 7261 7772 2900 0000 722b 0000  ...drawr)...r+..
-00000ce0: 0072 2b00 0000 722c 0000 00da 076f 6e5f  .r+...r,.....on_
-00000cf0: 6472 6177 5200 0000 f304 0000 0008 010e  drawR...........
-00000d00: 017a 144d 6169 6e4d 656e 7556 6965 772e  .z.MainMenuView.
-00000d10: 6f6e 5f64 7261 77a9 08da 085f 5f6e 616d  on_draw....__nam
-00000d20: 655f 5fda 0a5f 5f6d 6f64 756c 655f 5fda  e__..__module__.
-00000d30: 0c5f 5f71 7561 6c6e 616d 655f 5f72 4100  .__qualname__rA.
-00000d40: 0000 7252 0000 0072 5700 0000 725d 0000  ..rR...rW...r]..
-00000d50: 00da 0d5f 5f63 6c61 7373 6365 6c6c 5f5f  ...__classcell__
-00000d60: 722b 0000 0072 2b00 0000 724d 0000 0072  r+...r+...rM...r
-00000d70: 2c00 0000 7206 0000 000f 0000 0073 0a00  ,...r........s..
-00000d80: 0000 0800 0c02 083a 0804 1003 7206 0000  .......:....r...
-00000d90: 0063 0000 0000 0000 0000 0000 0000 0000  .c..............
-00000da0: 0000 0300 0000 0000 0000 7205 0000 0029  ..........r....)
-00000db0: 0972 3600 0000 6302 0000 0000 0000 0000  .r6...c.........
-00000dc0: 0000 001c 0000 000a 0000 0003 0000 0073  ...............s
-00000dd0: 1204 0000 7400 8300 a001 a100 0100 7c01  ....t.........|.
-00000de0: 8802 5f02 7403 6a04 a005 a100 8802 5f06  .._.t.j......._.
-00000df0: 8802 6a06 a007 a100 0100 7403 6a04 6a08  ..j.......t.j.j.
-00000e00: 6401 6402 6403 6404 6405 6406 6407 6408  d.d.d.d.d.d.d.d.
-00000e10: 6409 8d08 7d02 7403 6a04 6a08 6401 640a  d...}.t.j.j.d.d.
-00000e20: 6403 640b 640c 640d 6407 6408 6409 8d08  d.d.d.d.d.d.d...
-00000e30: 7d03 7403 6a04 a009 640e 640f 6410 6411  }.t.j...d.d.d.d.
-00000e40: 6412 a105 7d04 7403 6a04 a009 640e 6413  d...}.t.j...d.d.
-00000e50: 6410 6411 6414 a105 7d05 7403 6a04 6a08  d.d.d...}.t.j.j.
-00000e60: 6415 6416 6401 6417 6418 640e 740a 6a0b  d.d.d.d.d.d.t.j.
-00000e70: 6408 6419 8d08 7d06 7403 6a04 6a08 6415  d.d...}.t.j.j.d.
-00000e80: 641a 6401 6417 641b 640e 740a 6a0b 6408  d.d.d.d.d.t.j.d.
-00000e90: 6419 8d08 7d07 7403 6a04 a009 641c 641d  d...}.t.j...d.d.
-00000ea0: 6401 6411 641e a105 7d08 7403 6a04 a009  d.d.d...}.t.j...
-00000eb0: 641f 641d 6401 6411 6420 a105 7d09 7403  d.d.d.d.d ..}.t.
-00000ec0: 6a04 a009 6421 641d 6401 6411 6422 a105  j...d!d.d.d.d"..
-00000ed0: 7d0a 7403 6a04 a009 6423 641d 6401 6411  }.t.j...d#d.d.d.
-00000ee0: 6424 a105 7d0b 7403 6a04 a009 6425 641d  d$..}.t.j...d%d.
-00000ef0: 6401 6411 6426 a105 7d0c 7403 6a04 a009  d.d.d&..}.t.j...
-00000f00: 6427 641d 6401 6411 6428 a105 7d0d 7403  d'd.d.d.d(..}.t.
-00000f10: 6a04 a009 641f 6429 6401 6411 6420 a105  j...d.d)d.d.d ..
-00000f20: 7d0e 7403 6a04 a009 6421 6429 6401 6411  }.t.j...d!d)d.d.
-00000f30: 6422 a105 7d0f 7403 6a04 a009 641c 6429  d"..}.t.j...d.d)
-00000f40: 6401 6411 641e a105 7d10 7403 6a04 a009  d.d.d...}.t.j...
-00000f50: 6423 6429 6401 6411 6424 a105 7d11 7403  d#d)d.d.d$..}.t.
-00000f60: 6a04 a009 6425 6429 6401 6411 6426 a105  j...d%d)d.d.d&..
-00000f70: 7d12 7403 6a04 a009 6427 6429 6401 6411  }.t.j...d'd)d.d.
-00000f80: 6428 a105 7d13 7403 6a04 a00c 642a 642b  d(..}.t.j...d*d+
-00000f90: 6404 6411 8802 6a0d 6a0e 642c 1900 a105  d.d...j.j.d,....
-00000fa0: 8900 7403 6a04 a00c 642a 642d 6404 6411  ..t.j...d*d-d.d.
-00000fb0: 8802 6a0d 6a0e 642e 1900 a105 8901 8802  ..j.j.d.........
-00000fc0: 6a06 a00f 7c04 a101 0100 8802 6a06 a00f  j...|.......j...
-00000fd0: 7c05 a101 0100 8802 6a06 a00f 7c02 a101  |.......j...|...
-00000fe0: 0100 8802 6a06 a00f 7c03 a101 0100 8802  ....j...|.......
-00000ff0: 6a06 a00f 7c06 a101 0100 8802 6a06 a00f  j...|.......j...
-00001000: 7c07 a101 0100 8802 6a06 a00f 7c08 a101  |.......j...|...
-00001010: 0100 8802 6a06 a00f 7c09 a101 0100 8802  ....j...|.......
-00001020: 6a06 a00f 7c0a a101 0100 8802 6a06 a00f  j...|.......j...
-00001030: 7c0b a101 0100 8802 6a06 a00f 7c0c a101  |.......j...|...
-00001040: 0100 8802 6a06 a00f 7c0d a101 0100 8802  ....j...|.......
-00001050: 6a06 a00f 7c10 a101 0100 8802 6a06 a00f  j...|.......j...
-00001060: 7c0e a101 0100 8802 6a06 a00f 7c0f a101  |.......j...|...
-00001070: 0100 8802 6a06 a00f 7c11 a101 0100 8802  ....j...|.......
-00001080: 6a06 a00f 7c12 a101 0100 8802 6a06 a00f  j...|.......j...
-00001090: 7c13 a101 0100 8802 6a06 a00f 8800 a101  |.......j.......
-000010a0: 0100 8802 6a06 a00f 8801 a101 0100 7c04  ....j.........|.
-000010b0: a010 642f a101 8700 8701 8702 6603 6430  ..d/........f.d0
-000010c0: 6431 8408 8301 7d14 7c05 a010 642f a101  d1....}.|...d/..
-000010d0: 6432 6433 8400 8301 7d15 7c08 a010 642f  d2d3....}.|...d/
-000010e0: a101 8702 6601 6434 6435 8408 8301 7d16  ....f.d4d5....}.
-000010f0: 7c09 a010 642f a101 8702 6601 6436 6437  |...d/....f.d6d7
-00001100: 8408 8301 7d17 7c0a a010 642f a101 8702  ....}.|...d/....
-00001110: 6601 6438 6439 8408 8301 7d18 7c0b a010  f.d8d9....}.|...
-00001120: 642f a101 8702 6601 643a 643b 8408 8301  d/....f.d:d;....
-00001130: 7d19 7c0c a010 642f a101 8702 6601 643c  }.|...d/....f.d<
-00001140: 643d 8408 8301 7d1a 7c0d a010 642f a101  d=....}.|...d/..
-00001150: 8702 6601 643e 643f 8408 8301 7d1b 7c10  ..f.d>d?....}.|.
-00001160: a010 642f a101 8702 6601 6440 6435 8408  ..d/....f.d@d5..
-00001170: 8301 7d16 7c0e a010 642f a101 8702 6601  ..}.|...d/....f.
-00001180: 6441 6437 8408 8301 7d17 7c0f a010 642f  dAd7....}.|...d/
-00001190: a101 8702 6601 6442 6439 8408 8301 7d18  ....f.dBd9....}.
-000011a0: 7c11 a010 642f a101 8702 6601 6443 643b  |...d/....f.dCd;
-000011b0: 8408 8301 7d19 7c12 a010 642f a101 8702  ....}.|...d/....
-000011c0: 6601 6444 643d 8408 8301 7d1a 7c13 a010  f.dDd=....}.|...
-000011d0: 642f a101 8702 6601 6445 643f 8408 8301  d/....f.dEd?....
-000011e0: 7d1b 6400 5300 2946 4ee9 6400 0000 6971  }.d.S.)FN.d...iq
-000011f0: 0200 00e9 4c04 0000 e996 0000 0072 1300  ....L........r..
-00001200: 0000 720f 0000 0072 1600 0000 5429 0372  ..r....r....T).r
-00001210: 0b00 0000 da05 616c 6967 6eda 0462 6f6c  ......align..bol
-00001220: 6472 0100 0000 720d 0000 007a 292a 4167  dr....r....z)*Ag
-00001230: 656e 7420 3120 6973 2075 7365 6420 666f  ent 1 is used fo
-00001240: 7220 7369 6e67 6c65 2070 6c61 7965 7220  r single player 
-00001250: 6761 6d65 732a e90a 0000 00e9 0f00 0000  games*..........
-00001260: e9e9 0200 0072 0800 0000 7210 0000 00da  .....r....r.....
-00001270: 0442 6163 6be9 b702 0000 7214 0000 00e9  .Back.....r.....
-00001280: a500 0000 697b 0200 00e9 3200 0000 7a08  ....i{....2...z.
-00001290: 4167 656e 7420 313a 2903 720b 0000 0072  Agent 1:).r....r
-000012a0: 0c00 0000 7268 0000 0069 3002 0000 7a08  ....rh...i0...z.
-000012b0: 4167 656e 7420 323a 6909 0100 0069 8f02  Agent 2:i....i..
-000012c0: 0000 721d 0000 0069 7c01 0000 da06 5261  ..r....i|.....Ra
-000012d0: 6e64 6f6d 69ef 0100 00da 0350 4250 6962  ndomi......PBPib
-000012e0: 0200 0072 1e00 0000 e9d5 0200 00fa 0454  ...r...........T
-000012f0: 5320 3269 4803 0000 7a08 4e65 7477 6f72  S 2iH...z.Networ
-00001300: 6b3a 6944 0200 0069 bb03 0000 e985 0200  k:iD...i........
-00001310: 00fa 0b4e 6574 776f 726b 3120 4944 693a  ...Network1 IDi:
-00001320: 0200 00fa 0b4e 6574 776f 726b 3220 4944  .....Network2 ID
-00001330: 721b 0000 0063 0100 0000 0000 0000 0000  r....c..........
-00001340: 0000 0100 0000 0300 0000 1300 0000 7342  ..............sB
-00001350: 0000 0088 006a 0088 026a 016a 0264 013c  .....j...j.j.d.<
-00001360: 0088 016a 0088 026a 016a 0264 023c 0088  ...j...j.j.d.<..
-00001370: 026a 01a0 0388 026a 016a 04a1 0101 0074  .j.....j.j.....t
-00001380: 0564 0388 026a 016a 029b 009d 0283 0101  .d...j.j........
-00001390: 0064 0053 0029 044e 7275 0000 0072 7600  .d.S.).Nru...rv.
-000013a0: 0000 7a13 2043 7572 7265 6e74 2053 6574  ..z. Current Set
-000013b0: 7469 6e67 733a 2029 0672 0a00 0000 7220  tings: ).r....r 
-000013c0: 0000 0072 2300 0000 7226 0000 0072 3500  ...r#...r&...r5.
-000013d0: 0000 da05 7072 696e 7472 2f00 0000 a903  ....printr/.....
-000013e0: 5a0a 4e65 7477 6f72 6b49 4431 5a0a 4e65  Z.NetworkID1Z.Ne
-000013f0: 7477 6f72 6b49 4432 722a 0000 0072 2b00  tworkID2r*...r+.
-00001400: 0000 722c 0000 00da 0d6f 6e5f 636c 6963  ..r,.....on_clic
-00001410: 6b5f 4261 636b 9500 0000 7308 0000 000e  k_Back....s.....
-00001420: 020e 0110 0116 017a 2c53 6574 7469 6e67  .......z,Setting
-00001430: 7356 6965 772e 5f5f 696e 6974 5f5f 2e3c  sView.__init__.<
-00001440: 6c6f 6361 6c73 3e2e 6f6e 5f63 6c69 636b  locals>.on_click
-00001450: 5f42 6163 6b63 0100 0000 0000 0000 0000  _Backc..........
-00001460: 0000 0100 0000 0200 0000 5300 0000 723a  ..........S...r:
-00001470: 0000 0072 2e00 0000 723b 0000 0072 2f00  ...r....r;...r/.
-00001480: 0000 722b 0000 0072 2b00 0000 722c 0000  ..r+...r+...r,..
-00001490: 0072 3e00 0000 9c00 0000 723f 0000 007a  .r>.......r?...z
-000014a0: 2c53 6574 7469 6e67 7356 6965 772e 5f5f  ,SettingsView.__
-000014b0: 696e 6974 5f5f 2e3c 6c6f 6361 6c73 3e2e  init__.<locals>.
-000014c0: 6f6e 5f63 6c69 636b 5f51 7569 7463 0100  on_click_Quitc..
-000014d0: 0000 0000 0000 0000 0000 0100 0000 0300  ................
-000014e0: 0000 1300 0000 f310 0000 0064 0188 006a  ...........d...j
-000014f0: 006a 0164 023c 0064 0053 0029 034e 721d  .j.d.<.d.S.).Nr.
-00001500: 0000 0072 1c00 0000 a902 7220 0000 0072  ...r......r ...r
-00001510: 2300 0000 722f 0000 0072 2900 0000 722b  #...r/...r)...r+
-00001520: 0000 0072 2c00 0000 da10 6f6e 5f63 6c69  ...r,.....on_cli
-00001530: 636b 5f4f 7074 696f 6e31 a000 0000 f302  ck_Option1......
-00001540: 0000 0010 027a 2f53 6574 7469 6e67 7356  .....z/SettingsV
-00001550: 6965 772e 5f5f 696e 6974 5f5f 2e3c 6c6f  iew.__init__.<lo
-00001560: 6361 6c73 3e2e 6f6e 5f63 6c69 636b 5f4f  cals>.on_click_O
-00001570: 7074 696f 6e31 6301 0000 0000 0000 0000  ption1c.........
-00001580: 0000 0001 0000 0003 0000 0013 0000 0072  ...............r
-00001590: 7a00 0000 2903 4e72 7000 0000 721c 0000  z...).Nrp...r...
-000015a0: 0072 7b00 0000 722f 0000 0072 2900 0000  .r{...r/...r)...
-000015b0: 722b 0000 0072 2c00 0000 da10 6f6e 5f63  r+...r,.....on_c
-000015c0: 6c69 636b 5f4f 7074 696f 6e32 a400 0000  lick_Option2....
-000015d0: 727d 0000 007a 2f53 6574 7469 6e67 7356  r}...z/SettingsV
-000015e0: 6965 772e 5f5f 696e 6974 5f5f 2e3c 6c6f  iew.__init__.<lo
-000015f0: 6361 6c73 3e2e 6f6e 5f63 6c69 636b 5f4f  cals>.on_click_O
-00001600: 7074 696f 6e32 6301 0000 0000 0000 0000  ption2c.........
-00001610: 0000 0001 0000 0003 0000 0013 0000 0072  ...............r
-00001620: 7a00 0000 2903 4e72 7100 0000 721c 0000  z...).Nrq...r...
-00001630: 0072 7b00 0000 722f 0000 0072 2900 0000  .r{...r/...r)...
-00001640: 722b 0000 0072 2c00 0000 da10 6f6e 5f63  r+...r,.....on_c
-00001650: 6c69 636b 5f4f 7074 696f 6e33 a800 0000  lick_Option3....
-00001660: 727d 0000 007a 2f53 6574 7469 6e67 7356  r}...z/SettingsV
-00001670: 6965 772e 5f5f 696e 6974 5f5f 2e3c 6c6f  iew.__init__.<lo
-00001680: 6361 6c73 3e2e 6f6e 5f63 6c69 636b 5f4f  cals>.on_click_O
-00001690: 7074 696f 6e33 6301 0000 0000 0000 0000  ption3c.........
-000016a0: 0000 0001 0000 0003 0000 0013 0000 0072  ...............r
-000016b0: 7a00 0000 2903 4e72 1e00 0000 721c 0000  z...).Nr....r...
-000016c0: 0072 7b00 0000 722f 0000 0072 2900 0000  .r{...r/...r)...
-000016d0: 722b 0000 0072 2c00 0000 da10 6f6e 5f63  r+...r,.....on_c
-000016e0: 6c69 636b 5f4f 7074 696f 6e34 ac00 0000  lick_Option4....
-000016f0: 727d 0000 007a 2f53 6574 7469 6e67 7356  r}...z/SettingsV
-00001700: 6965 772e 5f5f 696e 6974 5f5f 2e3c 6c6f  iew.__init__.<lo
-00001710: 6361 6c73 3e2e 6f6e 5f63 6c69 636b 5f4f  cals>.on_click_O
-00001720: 7074 696f 6e34 6301 0000 0000 0000 0000  ption4c.........
-00001730: 0000 0001 0000 0003 0000 0013 0000 0072  ...............r
-00001740: 7a00 0000 2903 4e72 7300 0000 721c 0000  z...).Nrs...r...
-00001750: 0072 7b00 0000 722f 0000 0072 2900 0000  .r{...r/...r)...
-00001760: 722b 0000 0072 2c00 0000 da10 6f6e 5f63  r+...r,.....on_c
-00001770: 6c69 636b 5f4f 7074 696f 6e35 b000 0000  lick_Option5....
-00001780: 727d 0000 007a 2f53 6574 7469 6e67 7356  r}...z/SettingsV
-00001790: 6965 772e 5f5f 696e 6974 5f5f 2e3c 6c6f  iew.__init__.<lo
-000017a0: 6361 6c73 3e2e 6f6e 5f63 6c69 636b 5f4f  cals>.on_click_O
-000017b0: 7074 696f 6e35 6301 0000 0000 0000 0000  ption5c.........
-000017c0: 0000 0001 0000 0003 0000 0013 0000 0072  ...............r
-000017d0: 7a00 0000 2903 4eda 074e 6574 776f 726b  z...).N..Network
-000017e0: 721c 0000 0072 7b00 0000 722f 0000 0072  r....r{...r/...r
-000017f0: 2900 0000 722b 0000 0072 2c00 0000 da10  )...r+...r,.....
-00001800: 6f6e 5f63 6c69 636b 5f4f 7074 696f 6e36  on_click_Option6
-00001810: b400 0000 727d 0000 007a 2f53 6574 7469  ....r}...z/Setti
-00001820: 6e67 7356 6965 772e 5f5f 696e 6974 5f5f  ngsView.__init__
-00001830: 2e3c 6c6f 6361 6c73 3e2e 6f6e 5f63 6c69  .<locals>.on_cli
-00001840: 636b 5f4f 7074 696f 6e36 6301 0000 0000  ck_Option6c.....
-00001850: 0000 0000 0000 0001 0000 0003 0000 0013  ................
-00001860: 0000 0072 7a00 0000 2903 4e72 1d00 0000  ...rz...).Nr....
-00001870: 721f 0000 0072 7b00 0000 722f 0000 0072  r....r{...r/...r
-00001880: 2900 0000 722b 0000 0072 2c00 0000 727c  )...r+...r,...r|
-00001890: 0000 00b8 0000 0072 7d00 0000 6301 0000  .......r}...c...
-000018a0: 0000 0000 0000 0000 0001 0000 0003 0000  ................
-000018b0: 0013 0000 0072 7a00 0000 2903 4e72 7000  .....rz...).Nrp.
-000018c0: 0000 721f 0000 0072 7b00 0000 722f 0000  ..r....r{...r/..
-000018d0: 0072 2900 0000 722b 0000 0072 2c00 0000  .r)...r+...r,...
-000018e0: 727e 0000 00bc 0000 0072 7d00 0000 6301  r~.......r}...c.
-000018f0: 0000 0000 0000 0000 0000 0001 0000 0003  ................
-00001900: 0000 0013 0000 0072 7a00 0000 2903 4e72  .......rz...).Nr
-00001910: 7100 0000 721f 0000 0072 7b00 0000 722f  q...r....r{...r/
-00001920: 0000 0072 2900 0000 722b 0000 0072 2c00  ...r)...r+...r,.
-00001930: 0000 727f 0000 00c0 0000 0072 7d00 0000  ..r........r}...
-00001940: 6301 0000 0000 0000 0000 0000 0001 0000  c...............
-00001950: 0003 0000 0013 0000 0072 7a00 0000 2903  .........rz...).
-00001960: 4e72 1e00 0000 721f 0000 0072 7b00 0000  Nr....r....r{...
-00001970: 722f 0000 0072 2900 0000 722b 0000 0072  r/...r)...r+...r
-00001980: 2c00 0000 7280 0000 00c4 0000 0072 7d00  ,...r........r}.
-00001990: 0000 6301 0000 0000 0000 0000 0000 0001  ..c.............
-000019a0: 0000 0003 0000 0013 0000 0072 7a00 0000  ...........rz...
-000019b0: 2903 4e72 7300 0000 721f 0000 0072 7b00  ).Nrs...r....r{.
-000019c0: 0000 722f 0000 0072 2900 0000 722b 0000  ..r/...r)...r+..
-000019d0: 0072 2c00 0000 7281 0000 00c8 0000 0072  .r,...r........r
-000019e0: 7d00 0000 6301 0000 0000 0000 0000 0000  }...c...........
-000019f0: 0001 0000 0003 0000 0013 0000 0072 7a00  .............rz.
-00001a00: 0000 2903 4e72 8200 0000 721f 0000 0072  ..).Nr....r....r
-00001a10: 7b00 0000 722f 0000 0072 2900 0000 722b  {...r/...r)...r+
-00001a20: 0000 0072 2c00 0000 7283 0000 00cc 0000  ...r,...r.......
-00001a30: 0072 7d00 0000 2911 7240 0000 0072 4100  .r}...).r@...rA.
-00001a40: 0000 7225 0000 0072 3c00 0000 7242 0000  ..r%...r<...rB..
-00001a50: 0072 4300 0000 7244 0000 0072 4500 0000  .rC...rD...rE...
-00001a60: 7247 0000 0072 4a00 0000 7204 0000 00da  rG...rJ...r.....
-00001a70: 0562 6c61 636b da0b 5549 496e 7075 7454  .black..UIInputT
-00001a80: 6578 7472 2000 0000 7223 0000 0072 4800  extr ...r#...rH.
-00001a90: 0000 7227 0000 0029 1c72 2a00 0000 7225  ..r'...).r*...r%
-00001aa0: 0000 005a 0e53 6574 7469 6e67 735f 6c61  ...Z.Settings_la
-00001ab0: 6265 6c5a 0a48 656c 705f 6c61 6265 6cda  belZ.Help_label.
-00001ac0: 0b42 6163 6b5f 6275 7474 6f6e da0b 5175  .Back_button..Qu
-00001ad0: 6974 5f62 7574 746f 6e5a 0e41 4941 6765  it_buttonZ.AIAge
-00001ae0: 6e74 315f 6c61 6265 6c5a 0e41 4941 6765  nt1_labelZ.AIAge
-00001af0: 6e74 325f 6c61 6265 6c5a 1741 4941 6765  nt2_labelZ.AIAge
-00001b00: 6e74 315f 4f70 7469 6f6e 315f 6275 7474  nt1_Option1_butt
-00001b10: 6f6e 5a17 4149 4167 656e 7431 5f4f 7074  onZ.AIAgent1_Opt
-00001b20: 696f 6e32 5f62 7574 746f 6e5a 1741 4941  ion2_buttonZ.AIA
-00001b30: 6765 6e74 315f 4f70 7469 6f6e 335f 6275  gent1_Option3_bu
-00001b40: 7474 6f6e 5a17 4149 4167 656e 7431 5f4f  ttonZ.AIAgent1_O
-00001b50: 7074 696f 6e34 5f62 7574 746f 6e5a 1741  ption4_buttonZ.A
-00001b60: 4941 6765 6e74 315f 4f70 7469 6f6e 355f  IAgent1_Option5_
-00001b70: 6275 7474 6f6e 5a17 4149 4167 656e 7431  buttonZ.AIAgent1
-00001b80: 5f4f 7074 696f 6e36 5f62 7574 746f 6e5a  _Option6_buttonZ
-00001b90: 1741 4941 6765 6e74 325f 4f70 7469 6f6e  .AIAgent2_Option
-00001ba0: 325f 6275 7474 6f6e 5a17 4149 4167 656e  2_buttonZ.AIAgen
-00001bb0: 7432 5f4f 7074 696f 6e33 5f62 7574 746f  t2_Option3_butto
-00001bc0: 6e5a 1741 4941 6765 6e74 325f 4f70 7469  nZ.AIAgent2_Opti
-00001bd0: 6f6e 315f 6275 7474 6f6e 5a17 4149 4167  on1_buttonZ.AIAg
-00001be0: 656e 7432 5f4f 7074 696f 6e34 5f62 7574  ent2_Option4_but
-00001bf0: 746f 6e5a 1741 4941 6765 6e74 325f 4f70  tonZ.AIAgent2_Op
-00001c00: 7469 6f6e 355f 6275 7474 6f6e 5a17 4149  tion5_buttonZ.AI
-00001c10: 4167 656e 7432 5f4f 7074 696f 6e36 5f62  Agent2_Option6_b
-00001c20: 7574 746f 6e72 7900 0000 723e 0000 0072  uttonry...r>...r
-00001c30: 7c00 0000 727e 0000 0072 7f00 0000 7280  |...r~...r....r.
-00001c40: 0000 0072 8100 0000 7283 0000 0072 4d00  ...r....r....rM.
-00001c50: 0000 7278 0000 0072 2c00 0000 7241 0000  ..rx...r,...rA..
-00001c60: 0059 0000 0073 9800 0000 0a01 0601 0c02  .Y...s..........
-00001c70: 0a01 1c02 1c01 1402 1401 1602 0201 06ff  ................
-00001c80: 1602 0201 06ff 1403 1401 1401 1401 1401  ................
-00001c90: 1401 1402 1401 1401 1401 1401 1401 1c02  ................
-00001ca0: 1c01 0c02 0c01 0c02 0c01 0c01 0c01 0c02  ................
-00001cb0: 0c01 0c01 0c01 0c01 0c01 0c02 0c01 0c01  ................
-00001cc0: 0c01 0c01 0c01 0c02 0c01 0802 1201 0806  ................
-00001cd0: 0a01 0803 0e01 0803 0e01 0803 0e01 0803  ................
-00001ce0: 0e01 0803 0e01 0803 0e01 0803 0e01 0803  ................
-00001cf0: 0e01 0803 0e01 0803 0e01 0803 0e01 0803  ................
-00001d00: 1201 7a15 5365 7474 696e 6773 5669 6577  ..z.SettingsView
-00001d10: 2e5f 5f69 6e69 745f 5f63 0100 0000 0000  .__init__c......
-00001d20: 0000 0000 0000 0100 0000 0300 0000 4300  ..............C.
-00001d30: 0000 724f 0000 0072 2e00 0000 7250 0000  ..rO...r....rP..
-00001d40: 0072 2900 0000 722b 0000 0072 2b00 0000  .r)...r+...r+...
-00001d50: 722c 0000 0072 5200 0000 d000 0000 7253  r,...rR.......rS
-00001d60: 0000 007a 1953 6574 7469 6e67 7356 6965  ...z.SettingsVie
-00001d70: 772e 6f6e 5f73 686f 775f 7669 6577 6301  w.on_show_viewc.
-00001d80: 0000 0000 0000 0000 0000 0001 0000 0002  ................
-00001d90: 0000 0043 0000 0072 5400 0000 722e 0000  ...C...rT...r...
-00001da0: 0072 5500 0000 7229 0000 0072 2b00 0000  .rU...r)...r+...
-00001db0: 722b 0000 0072 2c00 0000 7257 0000 00d4  r+...r,...rW....
-00001dc0: 0000 0072 5800 0000 7a19 5365 7474 696e  ...rX...z.Settin
-00001dd0: 6773 5669 6577 2e6f 6e5f 6869 6465 5f76  gsView.on_hide_v
-00001de0: 6965 7763 0100 0000 0000 0000 0000 0000  iewc............
-00001df0: 0100 0000 0300 0000 4300 0000 7324 0000  ........C...s$..
-00001e00: 007c 00a0 00a1 0001 0074 01a0 027c 006a  .|.......t...|.j
-00001e10: 036a 04a1 0101 007c 006a 05a0 06a1 0001  .j.....|.j......
-00001e20: 0064 0053 0072 2e00 0000 2907 725b 0000  .d.S.r....).r[..
-00001e30: 0072 0400 0000 da0c 4472 6177 5365 7474  .r......DrawSett
-00001e40: 696e 6773 7220 0000 0072 2300 0000 7244  ingsr ...r#...rD
-00001e50: 0000 0072 5c00 0000 7229 0000 0072 2b00  ...r\...r)...r+.
-00001e60: 0000 722b 0000 0072 2c00 0000 725d 0000  ..r+...r,...r]..
-00001e70: 00d7 0000 0073 0600 0000 0801 0e02 0e02  .....s..........
-00001e80: 7a14 5365 7474 696e 6773 5669 6577 2e6f  z.SettingsView.o
-00001e90: 6e5f 6472 6177 725f 0000 0072 2b00 0000  n_drawr_...r+...
-00001ea0: 722b 0000 0072 4d00 0000 722c 0000 0072  r+...rM...r,...r
-00001eb0: 3600 0000 5700 0000 730a 0000 0008 000c  6...W...s.......
-00001ec0: 0208 7708 0410 0372 3600 0000 6300 0000  ..w....r6...c...
-00001ed0: 0000 0000 0000 0000 0000 0000 0003 0000  ................
-00001ee0: 0000 0000 0072 0500 0000 2909 7224 0000  .....r....).r$..
-00001ef0: 0063 0200 0000 0000 0000 0000 0000 1400  .c..............
-00001f00: 0000 0900 0000 0300 0000 73d4 0200 0074  ..........s....t
-00001f10: 0083 00a0 01a1 0001 007c 0188 005f 0274  .........|..._.t
-00001f20: 036a 04a0 05a1 0088 005f 0688 006a 06a0  .j......._...j..
-00001f30: 07a1 0001 0074 036a 04a0 0864 0164 0264  .....t.j...d.d.d
-00001f40: 0364 0464 05a1 057d 0274 036a 04a0 0864  .d.d...}.t.j...d
-00001f50: 0164 0664 0364 0464 07a1 057d 0374 036a  .d.d.d.d...}.t.j
-00001f60: 04a0 0864 0164 0164 0364 0864 09a1 057d  ...d.d.d.d.d...}
-00001f70: 0474 036a 04a0 0864 0a64 0164 0b64 0464  .t.j...d.d.d.d.d
-00001f80: 0ca1 057d 0574 036a 04a0 0864 0a64 0264  ...}.t.j...d.d.d
-00001f90: 0b64 0464 0da1 057d 0674 036a 04a0 0864  .d.d...}.t.j...d
-00001fa0: 0a64 0664 0b64 0464 0ea1 057d 0774 036a  .d.d.d.d...}.t.j
-00001fb0: 04a0 0864 0a64 0f64 0b64 0464 10a1 057d  ...d.d.d.d.d...}
-00001fc0: 0874 036a 04a0 0864 0a64 1164 0b64 0464  .t.j...d.d.d.d.d
-00001fd0: 12a1 057d 0974 036a 046a 0964 0a64 1364  ...}.t.j.j.d.d.d
-00001fe0: 0b64 0464 1464 1564 1664 178d 077d 0a74  .d.d.d.d.d...}.t
-00001ff0: 036a 04a0 0a64 1864 1964 0464 0474 0b6a  .j...d.d.d.d.t.j
-00002000: 0c74 0b6a 0d74 0b6a 0ea1 0788 005f 0f74  .t.j.t.j....._.t
-00002010: 036a 04a0 0a64 1a64 1964 0464 0474 0b6a  .j...d.d.d.d.t.j
-00002020: 1074 0b6a 1174 0b6a 12a1 0788 005f 1374  .t.j.t.j....._.t
-00002030: 036a 046a 0964 0a64 1b64 0b64 0464 1c64  .j.j.d.d.d.d.d.d
-00002040: 1564 1664 178d 077d 0b74 036a 046a 1464  .d.d...}.t.j.j.d
-00002050: 1d64 1e64 0b64 0464 1f64 1664 208d 0689  .d.d.d.d.d.d ...
-00002060: 0188 006a 06a0 157c 02a1 0101 0088 006a  ...j...|.......j
-00002070: 06a0 157c 03a1 0101 0088 006a 06a0 157c  ...|.......j...|
-00002080: 04a1 0101 0088 006a 06a0 157c 05a1 0101  .......j...|....
-00002090: 0088 006a 06a0 157c 06a1 0101 0088 006a  ...j...|.......j
-000020a0: 06a0 157c 07a1 0101 0088 006a 06a0 157c  ...|.......j...|
-000020b0: 08a1 0101 0088 006a 06a0 157c 09a1 0101  .......j...|....
-000020c0: 0088 006a 06a0 157c 0aa1 0101 0088 006a  ...j...|.......j
-000020d0: 06a0 1588 006a 0fa1 0101 0088 006a 06a0  .....j.......j..
-000020e0: 1588 006a 13a1 0101 0088 006a 06a0 157c  ...j.......j...|
-000020f0: 0ba1 0101 0088 006a 06a0 1588 01a1 0101  .......j........
-00002100: 007c 02a0 1664 21a1 0187 0066 0164 2264  .|...d!....f.d"d
-00002110: 2384 0883 017d 0c7c 03a0 1664 21a1 0164  #....}.|...d!..d
-00002120: 2464 2584 0083 017d 0d7c 04a0 1664 21a1  $d%....}.|...d!.
-00002130: 0187 0066 0164 2664 2784 0883 017d 0e7c  ...f.d&d'....}.|
-00002140: 05a0 1664 21a1 0187 0066 0164 2864 2984  ...d!....f.d(d).
-00002150: 0883 017d 0f7c 06a0 1664 21a1 0187 0066  ...}.|...d!....f
-00002160: 0164 2a64 2b84 0883 017d 107c 07a0 1664  .d*d+....}.|...d
-00002170: 21a1 0187 0066 0164 2c64 2b84 0883 017d  !....f.d,d+....}
-00002180: 107c 08a0 1664 21a1 0187 0087 0166 0264  .|...d!......f.d
-00002190: 2d64 2b84 0883 017d 107c 09a0 1664 21a1  -d+....}.|...d!.
-000021a0: 0187 0066 0164 2e64 2f84 0883 017d 1188  ...f.d.d/....}..
-000021b0: 006a 0fa0 1664 21a1 0187 0066 0164 3064  .j...d!....f.d0d
-000021c0: 3184 0883 017d 1288 006a 13a0 1664 21a1  1....}...j...d!.
-000021d0: 0187 0066 0164 3264 3384 0883 017d 1364  ...f.d2d3....}.d
-000021e0: 0053 0029 344e 726a 0000 0072 6b00 0000  .S.)4Nrj...rk...
-000021f0: 7208 0000 0072 1000 0000 da04 4578 6974  r....r......Exit
-00002200: 726d 0000 0072 1400 0000 e93c 0000 007a  rm...r.....<...z
-00002210: 084e 6577 2047 616d 65e9 f203 0000 e9af  .New Game.......
-00002220: 0000 0072 1300 0000 7a08 5275 6e20 4761  ...r....z.Run Ga
-00002230: 6d65 7a08 5275 6e20 5475 726e 7274 0000  mez.Run Turnrt..
-00002240: 007a 0c52 756e 2053 6574 2054 7572 6e69  .z.Run Set Turni
-00002250: 5302 0000 7a0a 4564 6974 2062 6f61 7264  S...z.Edit board
-00002260: 6921 0200 007a 0b4e 6578 7420 506c 6179  i!...z.Next Play
-00002270: 6572 7216 0000 00e9 1000 0000 2902 7267  err.........).rg
-00002280: 0000 0072 0b00 0000 691f 0400 0069 0302  ...r....i....i..
-00002290: 0000 6951 0400 0072 1100 0000 7a0d 4e65  ..iQ...r....z.Ne
-000022a0: 7874 2053 6574 2052 6f6c 6c69 3d04 0000  xt Set Rolli=...
-000022b0: 6904 0100 007a 0336 2c36 a901 720b 0000  i....z.6,6..r...
-000022c0: 0072 1b00 0000 6301 0000 0000 0000 0000  .r....c.........
-000022d0: 0000 0002 0000 0003 0000 0013 0000 00f3  ................
-000022e0: 1a00 0000 7400 8800 6a01 8301 7d01 8800  ....t...j...}...
-000022f0: 6a02 a003 7c01 a101 0100 6400 5300 722e  j...|.....d.S.r.
-00002300: 0000 00a9 0472 0600 0000 7225 0000 0072  .....r....r%...r
-00002310: 2000 0000 7226 0000 0029 0272 2700 0000   ...r&...).r'...
-00002320: 5a08 6d61 696e 5669 6577 7229 0000 0072  Z.mainViewr)...r
-00002330: 2b00 0000 722c 0000 0072 7900 0000 0c01  +...r,...ry.....
-00002340: 0000 f304 0000 000a 0210 017a 2b4d 6169  ...........z+Mai
-00002350: 6e53 696d 5669 6577 2e5f 5f69 6e69 745f  nSimView.__init_
-00002360: 5f2e 3c6c 6f63 616c 733e 2e6f 6e5f 636c  _.<locals>.on_cl
-00002370: 6963 6b5f 4261 636b 6301 0000 0000 0000  ick_Backc.......
-00002380: 0000 0000 0001 0000 0002 0000 0053 0000  .............S..
-00002390: 0072 3a00 0000 722e 0000 0072 3b00 0000  .r:...r....r;...
-000023a0: 722f 0000 0072 2b00 0000 722b 0000 0072  r/...r+...r+...r
-000023b0: 2c00 0000 723e 0000 0011 0100 0072 3f00  ,...r>.......r?.
-000023c0: 0000 7a2b 4d61 696e 5369 6d56 6965 772e  ..z+MainSimView.
-000023d0: 5f5f 696e 6974 5f5f 2e3c 6c6f 6361 6c73  __init__.<locals
-000023e0: 3e2e 6f6e 5f63 6c69 636b 5f51 7569 7463  >.on_click_Quitc
-000023f0: 0100 0000 0000 0000 0000 0000 0100 0000  ................
-00002400: 0200 0000 1300 0000 7318 0000 0088 006a  ........s......j
-00002410: 006a 01a0 02a1 0001 0064 0188 006a 005f  .j.......d...j._
-00002420: 0364 0053 0029 024e 5429 0472 2000 0000  .d.S.).NT).r ...
-00002430: 7221 0000 0072 2200 0000 da09 6669 7273  r!...r".....firs
-00002440: 7454 7572 6e72 2f00 0000 7229 0000 0072  tTurnr/...r)...r
-00002450: 2b00 0000 722c 0000 00da 0c6f 6e5f 636c  +...r,.....on_cl
-00002460: 6963 6b5f 4e65 7715 0100 0073 0400 0000  ick_New....s....
-00002470: 0c02 0c01 7a2a 4d61 696e 5369 6d56 6965  ....z*MainSimVie
-00002480: 772e 5f5f 696e 6974 5f5f 2e3c 6c6f 6361  w.__init__.<loca
-00002490: 6c73 3e2e 6f6e 5f63 6c69 636b 5f4e 6577  ls>.on_click_New
-000024a0: 6301 0000 0000 0000 0000 0000 0002 0000  c...............
-000024b0: 0003 0000 0013 0000 0072 3300 0000 722e  .........r3...r.
-000024c0: 0000 0072 3400 0000 7237 0000 0072 2900  ...r4...r7...r).
-000024d0: 0000 722b 0000 0072 2c00 0000 7238 0000  ..r+...r,...r8..
-000024e0: 001a 0100 0072 3900 0000 7a2f 4d61 696e  .....r9...z/Main
-000024f0: 5369 6d56 6965 772e 5f5f 696e 6974 5f5f  SimView.__init__
-00002500: 2e3c 6c6f 6361 6c73 3e2e 6f6e 5f63 6c69  .<locals>.on_cli
-00002510: 636b 5f53 6574 7469 6e67 7363 0100 0000  ck_Settingsc....
-00002520: 0000 0000 0000 0000 0400 0000 0700 0000  ................
-00002530: 1300 0000 73d6 0100 0088 006a 006a 0164  ....s......j.j.d
-00002540: 016b 0372 0a88 006a 006a 016e 0574 02a0  .k.r...j.j.n.t..
-00002550: 0364 0264 03a1 0288 006a 005f 0164 047d  .d.d.....j._.d.}
-00002560: 017c 0173 e988 006a 006a 0164 026b 0272  .|.s...j.j.d.k.r
-00002570: 8188 006a 006a 0464 0519 0064 066b 0272  ...j.j.d...d.k.r
-00002580: 256e c074 056a 0688 006a 006a 0188 006a  %n.t.j...j.j...j
-00002590: 006a 0464 0519 0088 006a 006a 0164 016b  .j.d.....j.j.d.k
-000025a0: 0264 078d 0388 006a 005f 0788 006a 006a  .d.....j._...j.j
-000025b0: 07a0 0888 006a 006a 09a1 0101 0074 0aa0  .....j.j.....t..
-000025c0: 0b88 006a 006a 0988 006a 006a 0788 006a  ...j.j...j.j...j
-000025d0: 006a 0464 0519 0088 006a 006a 0464 0819  .j.d.....j.j.d..
-000025e0: 00a1 047d 0288 006a 006a 09a0 0c7c 0264  ...}...j.j...|.d
-000025f0: 0264 09a1 0301 0088 006a 006a 096a 0d64  .d.......j.j.j.d
-00002600: 0119 0064 016b 0272 7c74 0e6a 0f6a 1064  ...d.k.r|t.j.j.d
-00002610: 0a64 0b64 0c64 0064 0d67 0164 0e8d 057d  .d.d.d.d.g.d...}
-00002620: 0388 006a 11a0 127c 03a1 0101 0064 097d  ...j...|.....d.}
-00002630: 0164 0388 006a 005f 016e 6488 006a 006a  .d...j._.nd..j.j
-00002640: 0464 0f19 0064 066b 0272 8a6e 5b74 056a  .d...d.k.r.n[t.j
-00002650: 0688 006a 006a 0188 006a 006a 0464 0f19  ...j.j...j.j.d..
-00002660: 0088 006a 006a 0164 016b 0264 078d 0388  ...j.j.d.k.d....
-00002670: 006a 005f 0788 006a 006a 07a0 0888 006a  .j._...j.j.....j
-00002680: 006a 09a1 0101 0074 0aa0 0b88 006a 006a  .j.....t.....j.j
-00002690: 0988 006a 006a 0788 006a 006a 0464 0f19  ...j.j...j.j.d..
-000026a0: 0088 006a 006a 0464 1019 00a1 047d 0288  ...j.j.d.....}..
-000026b0: 006a 006a 09a0 0c7c 0264 0364 09a1 0301  .j.j...|.d.d....
-000026c0: 0088 006a 006a 096a 0d64 0219 0064 016b  ...j.j.j.d...d.k
-000026d0: 0272 e174 0e6a 0f6a 1064 0a64 0b64 1164  .r.t.j.j.d.d.d.d
-000026e0: 0064 0d67 0164 0e8d 057d 0388 006a 11a0  .d.g.d...}...j..
-000026f0: 127c 03a1 0101 0064 097d 0164 0288 006a  .|.....d.}.d...j
-00002700: 005f 017c 0172 1664 0053 0064 0053 0029  ._.|.r.d.S.d.S.)
-00002710: 124e 7201 0000 00e9 0100 0000 e902 0000  .Nr.............
-00002720: 0046 721c 0000 0072 1d00 0000 a901 da05  .Fr....r........
-00002730: 4669 7273 7472 7500 0000 5472 1100 0000  Firstru...Tr....
-00002740: 7266 0000 00fa 4847 616d 6520 4f76 6572  rf....HGame Over
-00002750: 3a20 0a50 6c61 7965 7220 3120 5769 6e73  : .Player 1 Wins
-00002760: 2120 506c 6561 7365 2053 656c 6563 7420  ! Please Select 
-00002770: 274e 6577 2047 616d 6527 2074 6f20 7374  'New Game' to st
-00002780: 6172 7420 6120 6e65 7720 6761 6d65 2eda  art a new game..
-00002790: 024f 6ba9 0572 1200 0000 da06 6865 6967  .Ok..r......heig
-000027a0: 6874 da0c 6d65 7373 6167 655f 7465 7874  ht..message_text
-000027b0: da08 6361 6c6c 6261 636b da07 6275 7474  ..callback..butt
-000027c0: 6f6e 7372 1f00 0000 7276 0000 00fa 4847  onsr....rv....HG
-000027d0: 616d 6520 4f76 6572 3a20 0a50 6c61 7965  ame Over: .Playe
-000027e0: 7220 3220 5769 6e73 2120 506c 6561 7365  r 2 Wins! Please
-000027f0: 2053 656c 6563 7420 274e 6577 2047 616d   Select 'New Gam
-00002800: 6527 2074 6f20 7374 6172 7420 6120 6e65  e' to start a ne
-00002810: 7720 6761 6d65 2e29 1372 2000 0000 da0a  w game.).r .....
-00002820: 6e65 7874 506c 6179 6572 da06 7261 6e64  nextPlayer..rand
-00002830: 6f6d da07 7261 6e64 696e 7472 2300 0000  om..randintr#...
-00002840: 7203 0000 00da 0454 7572 6eda 084d 6169  r......Turn..Mai
-00002850: 6e54 7572 6eda 2175 7064 6174 6550 6f73  nTurn.!updatePos
-00002860: 7369 626c 654d 6f76 6573 5374 616e 6461  sibleMovesStanda
-00002870: 7264 466f 726d 6174 7221 0000 0072 0200  rdFormatr!...r..
-00002880: 0000 da04 4d61 696e da09 6d61 6b65 4d6f  ....Main..makeMo
-00002890: 7665 73da 0370 6970 723c 0000 0072 4200  ves..pipr<...rB.
-000028a0: 0000 da0c 5549 4d65 7373 6167 6542 6f78  ....UIMessageBox
-000028b0: 7244 0000 0072 4800 0000 2904 7227 0000  rD...rH...).r'..
-000028c0: 005a 0967 616d 655f 6f76 6572 da05 4d6f  .Z.game_over..Mo
-000028d0: 7665 73da 0a6d 6573 7361 6765 426f 7872  ves..messageBoxr
-000028e0: 2900 0000 722b 0000 0072 2c00 0000 da0c  )...r+...r,.....
-000028f0: 6f6e 5f63 6c69 636b 5f72 756e 2001 0000  on_click_run ...
-00002900: 7352 0000 0024 0204 0104 010c 0110 0102  sR...$..........
-00002910: 0114 020a 010a ff12 021a 010a 0104 ff12  ................
-00002920: 0212 010a 0102 0106 0106 fe0c 0304 010a  ................
-00002930: 0110 0202 0114 020a 010a ff12 021a 010a  ................
-00002940: 0104 ff12 0212 010a 0102 0106 0106 fe0c  ................
-00002950: 0304 0108 010c de7a 2a4d 6169 6e53 696d  .......z*MainSim
-00002960: 5669 6577 2e5f 5f69 6e69 745f 5f2e 3c6c  View.__init__.<l
-00002970: 6f63 616c 733e 2e6f 6e5f 636c 6963 6b5f  ocals>.on_click_
-00002980: 7275 6e63 0100 0000 0000 0000 0000 0000  runc............
-00002990: 0400 0000 0700 0000 1300 0000 73b6 0100  ............s...
-000029a0: 0088 006a 006a 0164 016b 0372 0a88 006a  ...j.j.d.k.r...j
-000029b0: 006a 016e 0574 02a0 0364 0264 03a1 027d  .j.n.t...d.d...}
-000029c0: 017c 0164 026b 0272 7588 006a 006a 0464  .|.d.k.ru..j.j.d
-000029d0: 0419 0064 056b 0272 1d6e b874 056a 067c  ...d.k.r.n.t.j.|
-000029e0: 0188 006a 006a 0464 0419 0088 006a 006a  ...j.j.d.....j.j
-000029f0: 0164 016b 0264 068d 0388 006a 005f 0788  .d.k.d.....j._..
-00002a00: 006a 006a 07a0 0888 006a 006a 09a1 0101  .j.j.....j.j....
-00002a10: 0074 0aa0 0b88 006a 006a 0988 006a 006a  .t.....j.j...j.j
-00002a20: 0788 006a 006a 0464 0419 0088 006a 006a  ...j.j.d.....j.j
-00002a30: 0464 0719 00a1 047d 0288 006a 006a 09a0  .d.....}...j.j..
-00002a40: 0c7c 0264 0264 08a1 0301 0088 006a 006a  .|.d.d.......j.j
-00002a50: 096a 0d64 0119 0064 016b 0272 7074 0e6a  .j.d...d.k.rpt.j
-00002a60: 0f6a 1064 0964 0a64 0b64 0064 0c67 0164  .j.d.d.d.d.d.g.d
-00002a70: 0d8d 057d 0388 006a 11a0 127c 03a1 0101  ...}...j...|....
-00002a80: 0064 0388 006a 005f 016e 6088 006a 006a  .d...j._.n`..j.j
-00002a90: 0464 0e19 0064 056b 0272 7e6e 5774 056a  .d...d.k.r~nWt.j
-00002aa0: 067c 0188 006a 006a 0464 0e19 0088 006a  .|...j.j.d.....j
-00002ab0: 006a 0164 016b 0264 068d 0388 006a 005f  .j.d.k.d.....j._
-00002ac0: 0788 006a 006a 07a0 0888 006a 006a 09a1  ...j.j.....j.j..
-00002ad0: 0101 0074 0aa0 0b88 006a 006a 0988 006a  ...t.....j.j...j
-00002ae0: 006a 0788 006a 006a 0464 0e19 0088 006a  .j...j.j.d.....j
-00002af0: 006a 0464 0f19 00a1 047d 0288 006a 006a  .j.d.....}...j.j
-00002b00: 09a0 0c7c 0264 0364 08a1 0301 0088 006a  ...|.d.d.......j
-00002b10: 006a 096a 0d64 0219 0064 016b 0272 d174  .j.j.d...d.k.r.t
-00002b20: 0e6a 0f6a 1064 0964 0a64 1064 0064 0c67  .j.j.d.d.d.d.d.g
-00002b30: 0164 0d8d 057d 0388 006a 11a0 127c 03a1  .d...}...j...|..
-00002b40: 0101 0064 0288 006a 005f 0164 1188 006a  ...d...j._.d...j
-00002b50: 005f 1364 0053 0029 124e 7201 0000 0072  ._.d.S.).Nr....r
-00002b60: 9400 0000 7295 0000 0072 1c00 0000 721d  ....r....r....r.
-00002b70: 0000 0072 9600 0000 7275 0000 0054 7211  ...r....ru...Tr.
-00002b80: 0000 0072 6600 0000 7298 0000 0072 9900  ...rf...r....r..
-00002b90: 0000 729a 0000 0072 1f00 0000 7276 0000  ..r....r....rv..
-00002ba0: 0072 9f00 0000 4629 1472 2000 0000 72a0  .r....F).r ...r.
-00002bb0: 0000 0072 a100 0000 72a2 0000 0072 2300  ...r....r....r#.
-00002bc0: 0000 7203 0000 0072 a300 0000 72a4 0000  ..r....r....r...
-00002bd0: 0072 a500 0000 7221 0000 0072 0200 0000  .r....r!...r....
-00002be0: 72a6 0000 0072 a700 0000 72a8 0000 0072  r....r....r....r
-00002bf0: 3c00 0000 7242 0000 0072 a900 0000 7244  <...rB...r....rD
-00002c00: 0000 0072 4800 0000 7292 0000 0029 0472  ...rH...r....).r
-00002c10: 2700 0000 da06 706c 6179 6572 72aa 0000  '.....playerr...
-00002c20: 0072 ab00 0000 7229 0000 0072 2b00 0000  .r....r)...r+...
-00002c30: 722c 0000 0072 ac00 0000 4801 0000 734a  r,...r....H...sJ
-00002c40: 0000 0020 0208 0110 0102 0110 020a 010a  ... ............
-00002c50: ff12 021a 010a 0104 ff12 0212 010a 0104  ................
-00002c60: 0104 0106 fe0c 030a 0110 0202 0110 020a  ................
-00002c70: 010a ff12 021a 010a 0104 ff12 0212 010a  ................
-00002c80: 0104 0104 0106 fe0c 0308 010c 0263 0100  .............c..
-00002c90: 0000 0000 0000 0000 0000 0600 0000 0700  ................
-00002ca0: 0000 1300 0000 7342 0200 0088 016a 006a  ......sB.....j.j
-00002cb0: 0164 0164 028d 017d 0164 0364 0484 007c  .d.d...}.d.d...|
-00002cc0: 0144 0083 017d 0274 02a0 037c 02a1 0173  .D...}.t...|...s
-00002cd0: 2774 046a 056a 0664 0564 0664 0764 0064  't.j.j.d.d.d.d.d
-00002ce0: 0867 0164 098d 057d 0388 006a 07a0 087c  .g.d...}...j...|
-00002cf0: 03a1 0101 0064 0053 007c 0264 0a19 007c  .....d.S.|.d...|
-00002d00: 0264 0b19 006b 0272 4788 006a 096a 0a72  .d...k.rG..j.j.r
-00002d10: 4774 046a 056a 0664 0564 0664 0c64 0064  Gt.j.j.d.d.d.d.d
-00002d20: 0867 0164 098d 057d 0388 006a 07a0 087c  .g.d...}...j...|
-00002d30: 03a1 0101 0064 0053 0088 006a 096a 0b64  .....d.S...j.j.d
-00002d40: 0a6b 0372 5188 006a 096a 0b6e 0574 0ca0  .k.rQ..j.j.n.t..
-00002d50: 0d64 0b64 0da1 027d 047c 0464 0b6b 0272  .d.d...}.|.d.k.r
-00002d60: bb88 006a 096a 0e64 0e19 0064 0f6b 0272  ...j.j.d...d.k.r
-00002d70: 646e b774 026a 0f7c 0488 006a 096a 0e64  dn.t.j.|...j.j.d
-00002d80: 0e19 0088 006a 096a 0a7c 0264 108d 0488  .....j.j.|.d....
-00002d90: 006a 095f 1088 006a 096a 10a0 1188 006a  .j._...j.j.....j
-00002da0: 096a 12a1 0101 0074 13a0 1488 006a 096a  .j.....t.....j.j
-00002db0: 1288 006a 096a 1088 006a 096a 0e64 0e19  ...j.j...j.j.d..
-00002dc0: 0088 006a 096a 0e64 1119 00a1 047d 0588  ...j.j.d.....}..
-00002dd0: 006a 096a 12a0 157c 0564 0b64 12a1 0301  .j.j...|.d.d....
-00002de0: 0088 006a 096a 126a 1664 0a19 0064 0a6b  ...j.j.j.d...d.k
-00002df0: 0272 b674 046a 056a 0664 0564 0664 1364  .r.t.j.j.d.d.d.d
-00002e00: 0064 0867 0164 098d 057d 0388 006a 07a0  .d.g.d...}...j..
-00002e10: 087c 03a1 0101 0064 0d88 006a 095f 0b6e  .|.....d...j._.n
-00002e20: 6088 006a 096a 0e64 1419 0064 0f6b 0272  `..j.j.d...d.k.r
-00002e30: c46e 5774 026a 0f7c 0488 006a 096a 0e64  .nWt.j.|...j.j.d
-00002e40: 1419 0088 006a 096a 0a7c 0264 108d 0488  .....j.j.|.d....
-00002e50: 006a 095f 1088 006a 096a 10a0 1188 006a  .j._...j.j.....j
-00002e60: 096a 12a1 0101 0074 13a0 1488 006a 096a  .j.....t.....j.j
-00002e70: 1288 006a 096a 1088 006a 096a 0e64 1419  ...j.j...j.j.d..
-00002e80: 0088 006a 096a 0e64 1519 00a1 047d 0588  ...j.j.d.....}..
-00002e90: 006a 096a 12a0 157c 0564 0d64 12a1 0301  .j.j...|.d.d....
-00002ea0: 0088 006a 096a 126a 1664 0b19 0064 0a6b  ...j.j.j.d...d.k
-00002eb0: 0290 0172 1774 046a 056a 0664 0564 0664  ...r.t.j.j.d.d.d
-00002ec0: 1664 0064 0867 0164 098d 057d 0388 006a  .d.d.g.d...}...j
-00002ed0: 07a0 087c 03a1 0101 0064 0b88 006a 095f  ...|.....d...j._
-00002ee0: 0b64 1788 006a 095f 0a64 0053 0029 184e  .d...j._.d.S.).N
-00002ef0: fa01 2ca9 01da 0373 6570 6301 0000 0000  ..,....sepc.....
-00002f00: 0000 0000 0000 0002 0000 0004 0000 0053  ...............S
-00002f10: 0000 00f3 1400 0000 6700 7c00 5d06 7d01  ........g.|.].}.
-00002f20: 7400 7c01 8301 9102 7102 5300 722b 0000  t.|.....q.S.r+..
-00002f30: 00a9 01da 0369 6e74 a902 da02 2e30 da03  .....int.....0..
-00002f40: 6e75 6d72 2b00 0000 722b 0000 0072 2c00  numr+...r+...r,.
-00002f50: 0000 da0a 3c6c 6973 7463 6f6d 703e 7201  ....<listcomp>r.
-00002f60: 0000 f302 0000 0014 007a 3e4d 6169 6e53  .........z>MainS
-00002f70: 696d 5669 6577 2e5f 5f69 6e69 745f 5f2e  imView.__init__.
-00002f80: 3c6c 6f63 616c 733e 2e6f 6e5f 636c 6963  <locals>.on_clic
-00002f90: 6b5f 7275 6e2e 3c6c 6f63 616c 733e 2e3c  k_run.<locals>.<
-00002fa0: 6c69 7374 636f 6d70 3e72 1100 0000 7266  listcomp>r....rf
-00002fb0: 0000 007a 4d49 6e70 7574 7465 6420 726f  ...zMInputted ro
-00002fc0: 6c6c 206e 6f74 206c 6567 616c 2e20 0a50  ll not legal. .P
-00002fd0: 6c65 6173 6520 696e 7075 7420 7661 6c69  lease input vali
-00002fe0: 6420 726f 6c6c 2069 6e20 666f 726d 206e  d roll in form n
-00002ff0: 756d 312c 6e75 6d32 200a 652e 672e 2034  um1,num2 .e.g. 4
-00003000: 2c35 7299 0000 0072 9a00 0000 7201 0000  ,5r....r....r...
-00003010: 0072 9400 0000 7a70 496e 7075 7474 6564  .r....zpInputted
-00003020: 2072 6f6c 6c20 6e6f 7420 6c65 6761 6c2e   roll not legal.
-00003030: 204e 6f20 446f 7562 6c65 7320 616c 6c6f   No Doubles allo
-00003040: 7765 6420 666f 7220 6669 7273 7420 6d6f  wed for first mo
-00003050: 7665 2e20 0a50 6c65 6173 6520 696e 7075  ve. .Please inpu
-00003060: 7420 7661 6c69 6420 726f 6c6c 2069 6e20  t valid roll in 
-00003070: 666f 726d 206e 756d 312c 6e75 6d32 200a  form num1,num2 .
-00003080: 652e 672e 2034 2c35 7295 0000 0072 1c00  e.g. 4,5r....r..
-00003090: 0000 721d 0000 0029 0272 9700 0000 da04  ..r....).r......
-000030a0: 726f 6c6c 7275 0000 0054 7298 0000 0072  rollru...Tr....r
-000030b0: 1f00 0000 7276 0000 0072 9f00 0000 4629  ....rv...r....F)
-000030c0: 1772 0a00 0000 da06 7273 706c 6974 7203  .r......rsplitr.
-000030d0: 0000 00da 0b69 734c 6567 616c 526f 6c6c  .....isLegalRoll
-000030e0: 723c 0000 0072 4200 0000 72a9 0000 0072  r<...rB...r....r
-000030f0: 4400 0000 7248 0000 0072 2000 0000 7292  D...rH...r ...r.
-00003100: 0000 0072 a000 0000 72a1 0000 0072 a200  ...r....r....r..
-00003110: 0000 7223 0000 0072 a300 0000 72a4 0000  ..r#...r....r...
-00003120: 0072 a500 0000 7221 0000 0072 0200 0000  .r....r!...r....
-00003130: 72a6 0000 0072 a700 0000 72a8 0000 0029  r....r....r....)
-00003140: 0672 2700 0000 5a0f 7365 745f 726f 6c6c  .r'...Z.set_roll
-00003150: 5f73 7472 696e 675a 0873 6574 5f72 6f6c  _stringZ.set_rol
-00003160: 6c72 ab00 0000 72ad 0000 0072 aa00 0000  lr....r....r....
-00003170: a902 722a 0000 005a 0d73 6574 526f 6c6c  ..r*...Z.setRoll
-00003180: 5f69 6e70 7574 722b 0000 0072 2c00 0000  _inputr+...r,...
-00003190: 72ac 0000 006e 0100 0073 6a00 0000 0e03  r....n...sj.....
-000031a0: 0e01 0a02 0a01 0401 0401 06fe 0c03 0401  ................
-000031b0: 1802 0a01 0201 0601 06fe 0c03 0401 2002  .............. .
-000031c0: 0801 1001 0201 1002 0801 0aff 1202 1a01  ................
-000031d0: 0a01 04ff 1202 1201 0a01 0401 0401 06fe  ................
-000031e0: 0c03 0a01 1002 0201 1002 0801 0aff 1202  ................
-000031f0: 1a01 0a01 04ff 1202 1401 0a01 0401 0401  ................
-00003200: 06fe 0c03 0801 0c02 6301 0000 0000 0000  ........c.......
-00003210: 0000 0000 0002 0000 0003 0000 0013 0000  ................
-00003220: 0072 8f00 0000 722e 0000 0029 04da 0d45  .r....r....)...E
-00003230: 6469 7442 6f61 7264 5669 6577 7225 0000  ditBoardViewr%..
-00003240: 0072 2000 0000 7226 0000 0029 0272 2700  .r ...r&...).r'.
-00003250: 0000 5a08 4564 6974 5669 6577 7229 0000  ..Z.EditViewr)..
-00003260: 0072 2b00 0000 722c 0000 00da 0d6f 6e5f  .r+...r,.....on_
-00003270: 636c 6963 6b5f 4564 6974 a601 0000 7291  click_Edit....r.
-00003280: 0000 007a 2b4d 6169 6e53 696d 5669 6577  ...z+MainSimView
-00003290: 2e5f 5f69 6e69 745f 5f2e 3c6c 6f63 616c  .__init__.<local
-000032a0: 733e 2e6f 6e5f 636c 6963 6b5f 4564 6974  s>.on_click_Edit
-000032b0: 6301 0000 0000 0000 0000 0000 0001 0000  c...............
-000032c0: 0002 0000 0013 0000 00f3 1c00 0000 8800  ................
-000032d0: 6a00 6a01 6401 6b03 7208 6401 6e01 6402  j.j.d.k.r.d.n.d.
-000032e0: 8800 6a00 5f01 6400 5300 2903 4e72 9400  ..j._.d.S.).Nr..
-000032f0: 0000 7201 0000 00a9 0272 2000 0000 72a0  ..r......r ...r.
-00003300: 0000 0072 2f00 0000 7229 0000 0072 2b00  ...r/...r)...r+.
-00003310: 0000 722c 0000 00da 0d6f 6e5f 636c 6963  ..r,.....on_clic
-00003320: 6b5f 4461 726b ab01 0000 f302 0000 001c  k_Dark..........
-00003330: 027a 2b4d 6169 6e53 696d 5669 6577 2e5f  .z+MainSimView._
-00003340: 5f69 6e69 745f 5f2e 3c6c 6f63 616c 733e  _init__.<locals>
-00003350: 2e6f 6e5f 636c 6963 6b5f 4461 726b 6301  .on_click_Darkc.
-00003360: 0000 0000 0000 0000 0000 0001 0000 0002  ................
-00003370: 0000 0013 0000 0072 bf00 0000 2903 4e72  .......r....).Nr
-00003380: 9500 0000 7201 0000 0072 c000 0000 722f  ....r....r....r/
-00003390: 0000 0072 2900 0000 722b 0000 0072 2c00  ...r)...r+...r,.
-000033a0: 0000 da0e 6f6e 5f63 6c69 636b 5f4c 6967  ....on_click_Lig
-000033b0: 6874 af01 0000 72c2 0000 007a 2c4d 6169  ht....r....z,Mai
-000033c0: 6e53 696d 5669 6577 2e5f 5f69 6e69 745f  nSimView.__init_
-000033d0: 5f2e 3c6c 6f63 616c 733e 2e6f 6e5f 636c  _.<locals>.on_cl
-000033e0: 6963 6b5f 4c69 6768 7429 1772 4000 0000  ick_Light).r@...
-000033f0: 7241 0000 0072 2500 0000 723c 0000 0072  rA...r%...r<...r
-00003400: 4200 0000 7243 0000 0072 4400 0000 7245  B...rC...rD...rE
-00003410: 0000 0072 4a00 0000 7247 0000 00da 0f55  ...rJ...rG.....U
-00003420: 4954 6578 7475 7265 4275 7474 6f6e 7204  ITextureButtonr.
-00003430: 0000 00da 0e64 6172 6b50 6965 6365 5f69  .....darkPiece_i
-00003440: 636f 6eda 0f64 6172 6b50 6965 6365 5f69  con..darkPiece_i
-00003450: 636f 6e32 da0f 6461 726b 5069 6563 655f  con2..darkPiece_
-00003460: 6963 6f6e 33da 156e 6578 7450 6c61 7965  icon3..nextPlaye
-00003470: 7244 6172 6b5f 6275 7474 6f6e da0f 6c69  rDark_button..li
-00003480: 6768 7450 6965 6365 5f69 636f 6eda 106c  ghtPiece_icon..l
-00003490: 6967 6874 5069 6563 655f 6963 6f6e 32da  ightPiece_icon2.
-000034a0: 106c 6967 6874 5069 6563 655f 6963 6f6e  .lightPiece_icon
-000034b0: 33da 166e 6578 7450 6c61 7965 724c 6967  3..nextPlayerLig
-000034c0: 6874 5f62 7574 746f 6e72 8500 0000 7248  ht_buttonr....rH
-000034d0: 0000 0072 2700 0000 2914 722a 0000 0072  ...r'...).r*...r
-000034e0: 2500 0000 7286 0000 0072 8700 0000 5a0a  %...r....r....Z.
-000034f0: 4e65 775f 6275 7474 6f6e 5a0e 5365 7474  New_buttonZ.Sett
-00003500: 696e 675f 6275 7474 6f6e 5a0e 5275 6e47  ing_buttonZ.RunG
-00003510: 616d 655f 6275 7474 6f6e 5a14 5275 6e52  ame_buttonZ.RunR
-00003520: 616e 646f 6d54 7572 6e5f 6275 7474 6f6e  andomTurn_button
-00003530: 5a11 5275 6e53 6574 5475 726e 5f62 7574  Z.RunSetTurn_but
-00003540: 746f 6e5a 1045 6469 7442 6f61 7264 5f62  tonZ.EditBoard_b
-00003550: 7574 746f 6e5a 106e 6578 7450 6c61 7965  uttonZ.nextPlaye
-00003560: 725f 6c61 6265 6c5a 0d73 6574 526f 6c6c  r_labelZ.setRoll
-00003570: 5f6c 6162 656c 7279 0000 0072 3e00 0000  _labelry...r>...
-00003580: 7293 0000 0072 3800 0000 72ac 0000 0072  r....r8...r....r
-00003590: be00 0000 72c1 0000 0072 c300 0000 724d  ....r....r....rM
-000035a0: 0000 0072 bc00 0000 722c 0000 0072 4100  ...r....r,...rA.
-000035b0: 0000 e100 0000 736c 0000 000a 0106 010c  ......sl........
-000035c0: 020a 0114 0214 0114 0114 0114 0214 0114  ................
-000035d0: 0114 011a 0212 0108 0106 ff12 0208 0106  ................
-000035e0: ff1a 0318 010c 020c 010c 010c 010c 020c  ................
-000035f0: 010c 010c 010c 020e 010e 010c 020c 0108  ................
-00003600: 020e 0108 040a 0108 030e 0108 040e 0108  ................
-00003610: 050e 0108 270e 0108 2510 0108 370e 010a  ....'...%...7...
-00003620: 040e 010a 0312 017a 144d 6169 6e53 696d  .......z.MainSim
-00003630: 5669 6577 2e5f 5f69 6e69 745f 5f63 0100  View.__init__c..
-00003640: 0000 0000 0000 0000 0000 0100 0000 0300  ................
-00003650: 0000 4300 0000 724f 0000 0072 2e00 0000  ..C...rO...r....
-00003660: 7250 0000 0072 2900 0000 722b 0000 0072  rP...r)...r+...r
-00003670: 2b00 0000 722c 0000 0072 5200 0000 b301  +...r,...rR.....
-00003680: 0000 7253 0000 007a 184d 6169 6e53 696d  ..rS...z.MainSim
-00003690: 5669 6577 2e6f 6e5f 7368 6f77 5f76 6965  View.on_show_vie
-000036a0: 7763 0100 0000 0000 0000 0000 0000 0100  wc..............
-000036b0: 0000 0200 0000 4300 0000 7254 0000 0072  ......C...rT...r
-000036c0: 2e00 0000 7255 0000 0072 2900 0000 722b  ....rU...r)...r+
-000036d0: 0000 0072 2b00 0000 722c 0000 0072 5700  ...r+...r,...rW.
-000036e0: 0000 b701 0000 7258 0000 007a 184d 6169  ......rX...z.Mai
-000036f0: 6e53 696d 5669 6577 2e6f 6e5f 6869 6465  nSimView.on_hide
-00003700: 5f76 6965 7763 0100 0000 0000 0000 0000  _viewc..........
-00003710: 0000 0100 0000 0500 0000 4300 0000 73e8  ..........C...s.
-00003720: 0000 007c 00a0 00a1 0001 007c 006a 016a  ...|.......|.j.j
-00003730: 0264 016b 0272 1574 036a 047c 006a 055f  .d.k.r.t.j.|.j._
-00003740: 0674 036a 077c 006a 085f 066e 1b7c 006a  .t.j.|.j._.n.|.j
-00003750: 016a 0264 026b 0272 2674 036a 097c 006a  .j.d.k.r&t.j.|.j
-00003760: 085f 0674 036a 0a7c 006a 055f 066e 0a74  ._.t.j.|.j._.n.t
-00003770: 036a 0a7c 006a 055f 0674 036a 077c 006a  .j.|.j._.t.j.|.j
-00003780: 085f 0674 03a0 0ba1 0001 0074 03a0 0c7c  ._.t.......t...|
-00003790: 006a 016a 0d6a 0e7c 006a 016a 0d6a 0fa1  .j.j.j.|.j.j.j..
-000037a0: 0201 0074 03a0 10a1 0001 007c 006a 016a  ...t.......|.j.j
-000037b0: 0d6a 1164 006b 0372 5374 03a0 127c 006a  .j.d.k.rSt...|.j
-000037c0: 016a 0d6a 11a1 0101 007c 006a 016a 1364  .j.j.....|.j.j.d
-000037d0: 006b 0372 6d74 03a0 147c 006a 016a 136a  .k.rmt...|.j.j.j
-000037e0: 1564 0319 007c 006a 016a 136a 1564 0119  .d...|.j.j.j.d..
-000037f0: 007c 006a 016a 136a 16a1 0301 007c 006a  .|.j.j.j.....|.j
-00003800: 17a0 18a1 0001 0064 0053 0029 044e 7294  .......d.S.).Nr.
-00003810: 0000 0072 9500 0000 7201 0000 0029 1972  ...r....r....).r
-00003820: 5b00 0000 7220 0000 0072 a000 0000 7204  [...r ...r....r.
-00003830: 0000 0072 c700 0000 72c8 0000 00da 0774  ...r....r......t
-00003840: 6578 7475 7265 72c9 0000 0072 cc00 0000  exturer....r....
-00003850: 72cb 0000 0072 c500 0000 da09 6472 6177  r....r......draw
-00003860: 426f 6172 64da 0a64 7261 7750 6965 6365  Board..drawPiece
-00003870: 7372 2100 0000 da09 706f 7369 7469 6f6e  sr!.....position
-00003880: 7372 a800 0000 da0b 4472 6177 5369 6d4d  sr......DrawSimM
-00003890: 6169 6eda 0c4d 6f76 654c 696e 6544 6174  ain..MoveLineDat
-000038a0: 61da 0d44 7261 774d 6f76 654c 696e 6573  a..DrawMoveLines
-000038b0: 72a4 0000 00da 0864 7261 7744 6963 6572  r......drawDicer
-000038c0: b900 0000 da0b 756e 7573 6564 5f64 6963  ......unused_dic
-000038d0: 6572 4400 0000 725c 0000 0072 2900 0000  erD...r\...r)...
-000038e0: 722b 0000 0072 2b00 0000 722c 0000 0072  r+...r+...r,...r
-000038f0: 5d00 0000 ba01 0000 7326 0000 0008 010c  ].......s&......
-00003900: 020a 010c 010c 010a 010c 010a 020a 0108  ................
-00003910: 0218 0108 020e 0210 010c 011c 0108 0104  ................
-00003920: ff0e 037a 134d 6169 6e53 696d 5669 6577  ...z.MainSimView
-00003930: 2e6f 6e5f 6472 6177 725f 0000 0072 2b00  .on_drawr_...r+.
-00003940: 0000 722b 0000 0072 4d00 0000 722c 0000  ..r+...rM...r,..
-00003950: 0072 2400 0000 e000 0000 730c 0000 0008  .r$.......s.....
-00003960: 000c 0100 7f08 5308 0410 0372 2400 0000  ......S....r$...
-00003970: 6300 0000 0000 0000 0000 0000 0000 0000  c...............
-00003980: 0008 0000 0000 0000 0073 4e00 0000 6500  .........sN...e.
-00003990: 5a01 6400 5a02 8700 6601 6401 6402 8408  Z.d.Z...f.d.d...
-000039a0: 5a03 6403 6404 8400 5a04 6405 6406 8400  Z.d.d...Z.d.d...
-000039b0: 5a05 6407 6506 6408 6506 6409 6506 640a  Z.d.e.d.e.d.e.d.
-000039c0: 6506 6608 640b 640c 8404 5a07 640d 640e  e.f.d.d...Z.d.d.
-000039d0: 8400 5a08 8700 0400 5a09 5300 290f 72bd  ..Z.....Z.S.).r.
-000039e0: 0000 0063 0200 0000 0000 0000 0000 0000  ...c............
-000039f0: 1000 0000 0900 0000 0300 0000 7370 0200  ............sp..
-00003a00: 0074 0083 00a0 01a1 0001 007c 0188 035f  .t.........|..._
-00003a10: 0264 0088 035f 0374 046a 05a0 06a1 0088  .d..._.t.j......
-00003a20: 035f 0788 036a 07a0 08a1 0001 0074 046a  ._...j.......t.j
-00003a30: 05a0 0964 0164 0264 0364 0464 05a1 057d  ...d.d.d.d.d...}
-00003a40: 0274 046a 05a0 0964 0164 0664 0364 0464  .t.j...d.d.d.d.d
-00003a50: 07a1 057d 0374 046a 05a0 0a64 0864 0964  ...}.t.j...d.d.d
-00003a60: 0364 0374 0b6a 0c74 0b6a 0d74 0b6a 0ea1  .d.t.j.t.j.t.j..
-00003a70: 0789 0274 046a 05a0 0a64 0864 0a64 0364  ...t.j...d.d.d.d
-00003a80: 0374 0b6a 0f74 0b6a 1074 0b6a 11a1 0789  .t.j.t.j.t.j....
-00003a90: 0074 046a 05a0 0a64 0864 0b64 0364 0374  .t.j...d.d.d.d.t
-00003aa0: 0b6a 1274 0b6a 1374 0b6a 14a1 0789 0174  .j.t.j.t.j.....t
-00003ab0: 046a 05a0 0a64 0864 0c64 0364 0374 0b6a  .j...d.d.d.d.t.j
-00003ac0: 1574 0b6a 1674 0b6a 17a1 077d 0474 046a  .t.j.t.j...}.t.j
-00003ad0: 05a0 0964 0864 0164 0d64 0464 0ea1 057d  ...d.d.d.d.d...}
-00003ae0: 0574 046a 056a 1864 0f64 1064 1164 1264  .t.j.j.d.d.d.d.d
-00003af0: 1364 0164 148d 067d 0674 046a 056a 1864  .d.d...}.t.j.j.d
-00003b00: 0f64 1564 1164 1264 1664 0164 148d 067d  .d.d.d.d.d.d...}
-00003b10: 0774 046a 056a 1864 0f64 1764 1164 1264  .t.j.j.d.d.d.d.d
-00003b20: 1864 0164 148d 067d 0874 046a 056a 1864  .d.d...}.t.j.j.d
-00003b30: 0f64 1964 1164 1264 1a64 0164 148d 067d  .d.d.d.d.d.d...}
-00003b40: 0988 036a 07a0 197c 02a1 0101 0088 036a  ...j...|.......j
-00003b50: 07a0 197c 03a1 0101 0088 036a 07a0 1988  ...|.......j....
-00003b60: 02a1 0101 0088 036a 07a0 1988 00a1 0101  .......j........
-00003b70: 0088 036a 07a0 1988 01a1 0101 0088 036a  ...j...........j
-00003b80: 07a0 197c 04a1 0101 0088 036a 07a0 197c  ...|.......j...|
-00003b90: 06a1 0101 0088 036a 07a0 197c 07a1 0101  .......j...|....
-00003ba0: 0088 036a 07a0 197c 08a1 0101 0088 036a  ...j...|.......j
-00003bb0: 07a0 197c 09a1 0101 0088 036a 07a0 197c  ...|.......j...|
-00003bc0: 05a1 0101 007c 02a0 1a64 1ba1 0187 0366  .....|...d.....f
-00003bd0: 0164 1c64 1d84 0883 017d 0a7c 03a0 1a64  .d.d.....}.|...d
-00003be0: 1ba1 0164 1e64 1f84 0083 017d 0b88 02a0  ...d.d.....}....
-00003bf0: 1a64 1ba1 0187 0087 0187 0287 0366 0464  .d...........f.d
-00003c00: 2064 2184 0883 017d 0c88 00a0 1a64 1ba1   d!....}.....d..
-00003c10: 0187 0087 0187 0287 0366 0464 2264 2384  .........f.d"d#.
-00003c20: 0883 017d 0d88 01a0 1a64 1ba1 0187 0087  ...}.....d......
-00003c30: 0187 0287 0366 0464 2464 2584 0883 017d  .....f.d$d%....}
-00003c40: 0e7c 04a0 1a64 1ba1 0187 0366 0164 2664  .|...d.....f.d&d
-00003c50: 2184 0883 017d 0c7c 05a0 1a64 1ba1 0187  !....}.|...d....
-00003c60: 0366 0164 2764 2884 0883 017d 0f64 0053  .f.d'd(....}.d.S
-00003c70: 0029 294e 726a 0000 0072 6b00 0000 7208  .))Nrj...rk...r.
-00003c80: 0000 0072 1000 0000 da04 446f 6e65 726d  ...r......Donerm
-00003c90: 0000 0072 1400 0000 728b 0000 00e9 fe01  ...r....r.......
-00003ca0: 0000 69a4 0100 0069 4a01 0000 e9f0 0000  ..i....iJ.......
-00003cb0: 0072 8c00 0000 7a0e 4564 6974 2061 7320  .r....z.Edit as 
-00003cc0: 5374 7269 6e67 7265 0000 0069 0d02 0000  Stringre...i....
-00003cd0: e95a 0000 00e9 2d00 0000 7a09 4164 6420  .Z....-...z.Add 
-00003ce0: 4c69 6768 7472 8e00 0000 69b3 0100 007a  Lightr....i....z
-00003cf0: 0b41 6464 2020 2020 4461 726b 6959 0100  .Add    DarkiY..
-00003d00: 007a 0c44 656c 6574 6520 5069 6563 6572  .z.Delete Piecer
-00003d10: 0900 0000 7a0a 4465 6c65 7465 2041 6c6c  ....z.Delete All
-00003d20: 721b 0000 0063 0100 0000 0000 0000 0000  r....c..........
-00003d30: 0000 0300 0000 0700 0000 1300 0000 735c  ..............s\
-00003d40: 0000 0074 00a0 0188 006a 026a 036a 04a1  ...t.....j.j.j..
-00003d50: 0172 1a74 0588 006a 0683 017d 0164 0088  .r.t...j...}.d..
-00003d60: 006a 026a 035f 0788 006a 02a0 087c 01a1  .j.j._...j...|..
-00003d70: 0101 0064 0053 0074 096a 0a6a 0b64 0164  ...d.S.t.j.j.d.d
-00003d80: 0264 0364 0064 0467 0164 058d 057d 0288  .d.d.d.g.d...}..
-00003d90: 006a 0ca0 0d7c 02a1 0101 0064 0053 0029  .j...|.....d.S.)
-00003da0: 064e 7211 0000 0072 6600 0000 7a4b 4572  .Nr....rf...zKEr
-00003db0: 726f 723a 200a 5468 6973 2069 6e20 6e6f  ror: .This in no
-00003dc0: 7420 6120 6c65 6761 6c20 4261 636b 6761  t a legal Backga
-00003dd0: 6d6d 6f6e 2062 6f61 7264 2e20 506c 6561  mmon board. Plea
-00003de0: 7365 2050 726f 7669 6465 2061 206c 6567  se Provide a leg
-00003df0: 616c 2062 6f61 7264 2e72 9900 0000 729a  al board.r....r.
-00003e00: 0000 0029 0e72 0300 0000 da0c 6973 4c65  ...).r......isLe
-00003e10: 6761 6c42 6f61 7264 7220 0000 0072 2100  galBoardr ...r!.
-00003e20: 0000 72d0 0000 0072 2400 0000 7225 0000  ..r....r$...r%..
-00003e30: 0072 d200 0000 7226 0000 0072 3c00 0000  .r....r&...r<...
-00003e40: 7242 0000 0072 a900 0000 7244 0000 0072  rB...r....rD...r
-00003e50: 4800 0000 2903 7227 0000 0072 2800 0000  H...).r'...r(...
-00003e60: 72ab 0000 0072 2900 0000 722b 0000 0072  r....r)...r+...r
-00003e70: 2c00 0000 da0d 6f6e 5f63 6c69 636b 5f44  ,.....on_click_D
-00003e80: 6f6e 6501 0200 0073 1200 0000 1002 0a01  one....s........
-00003e90: 0a01 1001 0a02 0401 0401 06fe 1003 7a2d  ..............z-
-00003ea0: 4564 6974 426f 6172 6456 6965 772e 5f5f  EditBoardView.__
-00003eb0: 696e 6974 5f5f 2e3c 6c6f 6361 6c73 3e2e  init__.<locals>.
-00003ec0: 6f6e 5f63 6c69 636b 5f44 6f6e 6563 0100  on_click_Donec..
-00003ed0: 0000 0000 0000 0000 0000 0100 0000 0200  ................
-00003ee0: 0000 5300 0000 723a 0000 0072 2e00 0000  ..S...r:...r....
-00003ef0: 723b 0000 0072 2f00 0000 722b 0000 0072  r;...r/...r+...r
-00003f00: 2b00 0000 722c 0000 0072 3e00 0000 0d02  +...r,...r>.....
-00003f10: 0000 723f 0000 007a 2d45 6469 7442 6f61  ..r?...z-EditBoa
-00003f20: 7264 5669 6577 2e5f 5f69 6e69 745f 5f2e  rdView.__init__.
-00003f30: 3c6c 6f63 616c 733e 2e6f 6e5f 636c 6963  <locals>.on_clic
-00003f40: 6b5f 5175 6974 6301 0000 0000 0000 0000  k_Quitc.........
-00003f50: 0000 0001 0000 0002 0000 0013 0000 00f3  ................
-00003f60: 2200 0000 6401 8803 5f00 7401 6a02 8802  "...d..._.t.j...
-00003f70: 5f03 7401 6a04 8800 5f03 7401 6a05 8801  _.t.j..._.t.j...
-00003f80: 5f03 6400 5300 2902 4eda 054c 6967 6874  _.d.S.).N..Light
-00003f90: 2906 da04 746f 6f6c 7204 0000 0072 cb00  )...toolr....r..
-00003fa0: 0000 72cd 0000 0072 c500 0000 da0b 6465  ..r....r......de
-00003fb0: 6c65 7465 5f69 636f 6e72 2f00 0000 a904  lete_iconr/.....
-00003fc0: 5a0b 6461 726b 5f62 7574 746f 6e5a 0d64  Z.dark_buttonZ.d
-00003fd0: 656c 6574 655f 6275 7474 6f6e 5a0c 6c69  elete_buttonZ.li
-00003fe0: 6768 745f 6275 7474 6f6e 722a 0000 0072  ght_buttonr*...r
-00003ff0: 2b00 0000 722c 0000 00da 0e6f 6e5f 636c  +...r,.....on_cl
-00004000: 6963 6b5f 6c69 6768 7411 0200 00f3 0800  ick_light.......
-00004010: 0000 0602 0801 0801 0c01 7a2e 4564 6974  ..........z.Edit
-00004020: 426f 6172 6456 6965 772e 5f5f 696e 6974  BoardView.__init
-00004030: 5f5f 2e3c 6c6f 6361 6c73 3e2e 6f6e 5f63  __.<locals>.on_c
-00004040: 6c69 636b 5f6c 6967 6874 6301 0000 0000  lick_lightc.....
-00004050: 0000 0000 0000 0001 0000 0002 0000 0013  ................
-00004060: 0000 0072 dd00 0000 2902 4eda 0444 6172  ...r....).N..Dar
-00004070: 6b29 0672 df00 0000 7204 0000 0072 c900  k).r....r....r..
-00004080: 0000 72cd 0000 0072 c700 0000 72e0 0000  ..r....r....r...
-00004090: 0072 2f00 0000 72e1 0000 0072 2b00 0000  .r/...r....r+...
-000040a0: 722c 0000 00da 0d6f 6e5f 636c 6963 6b5f  r,.....on_click_
-000040b0: 6461 726b 1802 0000 72e3 0000 007a 2d45  dark....r....z-E
-000040c0: 6469 7442 6f61 7264 5669 6577 2e5f 5f69  ditBoardView.__i
-000040d0: 6e69 745f 5f2e 3c6c 6f63 616c 733e 2e6f  nit__.<locals>.o
-000040e0: 6e5f 636c 6963 6b5f 6461 726b 6301 0000  n_click_darkc...
-000040f0: 0000 0000 0000 0000 0001 0000 0002 0000  ................
-00004100: 0013 0000 0072 dd00 0000 2902 4eda 0644  .....r....).N..D
-00004110: 656c 6574 6529 0672 df00 0000 7204 0000  elete).r....r...
-00004120: 0072 c900 0000 72cd 0000 0072 c500 0000  .r....r....r....
-00004130: da0c 6465 6c65 7465 5f69 636f 6e33 722f  ..delete_icon3r/
-00004140: 0000 0072 e100 0000 722b 0000 0072 2c00  ...r....r+...r,.
-00004150: 0000 da0f 6f6e 5f63 6c69 636b 5f64 656c  ....on_click_del
-00004160: 6574 651f 0200 0072 e300 0000 7a2f 4564  ete....r....z/Ed
-00004170: 6974 426f 6172 6456 6965 772e 5f5f 696e  itBoardView.__in
-00004180: 6974 5f5f 2e3c 6c6f 6361 6c73 3e2e 6f6e  it__.<locals>.on
-00004190: 5f63 6c69 636b 5f64 656c 6574 6563 0100  _click_deletec..
-000041a0: 0000 0000 0000 0000 0000 0100 0000 0200  ................
-000041b0: 0000 1300 0000 7314 0000 0064 0167 0164  ......s....d.g.d
-000041c0: 0214 0088 006a 006a 015f 0264 0053 0029  .....j.j._.d.S.)
-000041d0: 034e 7201 0000 00e9 1c00 0000 2903 7220  .Nr.........).r 
-000041e0: 0000 0072 2100 0000 72d0 0000 0072 2f00  ...r!...r....r/.
-000041f0: 0000 7229 0000 0072 2b00 0000 722c 0000  ..r)...r+...r,..
-00004200: 0072 e200 0000 2602 0000 7302 0000 0014  .r....&...s.....
-00004210: 0263 0100 0000 0000 0000 0000 0000 0200  .c..............
-00004220: 0000 0300 0000 1300 0000 728f 0000 0072  ..........r....r
-00004230: 2e00 0000 2904 da11 4564 6974 4173 5374  ....)...EditAsSt
-00004240: 7269 6e67 5f56 6965 7772 2500 0000 7220  ring_Viewr%...r 
-00004250: 0000 0072 2600 0000 2902 7227 0000 00da  ...r&...).r'....
-00004260: 0865 6469 7456 6965 7772 2900 0000 722b  .editViewr)...r+
-00004270: 0000 0072 2c00 0000 72be 0000 002a 0200  ...r,...r....*..
-00004280: 0072 9100 0000 7a2d 4564 6974 426f 6172  .r....z-EditBoar
-00004290: 6456 6965 772e 5f5f 696e 6974 5f5f 2e3c  dView.__init__.<
-000042a0: 6c6f 6361 6c73 3e2e 6f6e 5f63 6c69 636b  locals>.on_click
-000042b0: 5f45 6469 7429 1b72 4000 0000 7241 0000  _Edit).r@...rA..
-000042c0: 0072 2500 0000 72df 0000 0072 3c00 0000  .r%...r....r<...
-000042d0: 7242 0000 0072 4300 0000 7244 0000 0072  rB...rC...rD...r
-000042e0: 4500 0000 724a 0000 0072 c400 0000 7204  E...rJ...r....r.
-000042f0: 0000 0072 c900 0000 72ca 0000 0072 cb00  ...r....r....r..
-00004300: 0000 72c5 0000 0072 c600 0000 72c7 0000  ..r....r....r...
-00004310: 0072 e000 0000 da0c 6465 6c65 7465 5f69  .r......delete_i
-00004320: 636f 6e32 72e7 0000 00da 0c72 6573 7461  con2r......resta
-00004330: 7274 5f69 636f 6eda 0d72 6573 7461 7274  rt_icon..restart
-00004340: 5f69 636f 6e32 da0d 7265 7374 6172 745f  _icon2..restart_
-00004350: 6963 6f6e 33da 0a55 4954 6578 7441 7265  icon3..UITextAre
-00004360: 6172 4800 0000 7227 0000 0029 1072 2a00  arH...r'...).r*.
-00004370: 0000 7225 0000 00da 0b44 6f6e 655f 6275  ..r%.....Done_bu
-00004380: 7474 6f6e 7287 0000 005a 0e72 6573 7461  ttonr....Z.resta
-00004390: 7274 5f62 7574 746f 6e5a 0b45 6469 745f  rt_buttonZ.Edit_
-000043a0: 6275 7474 6f6e 5a0b 6c69 6768 745f 6c61  buttonZ.light_la
-000043b0: 6265 6c5a 0a64 6172 6b5f 6c61 6265 6c5a  belZ.dark_labelZ
-000043c0: 0c64 656c 6574 655f 6c61 6265 6c5a 0d72  .delete_labelZ.r
-000043d0: 6573 7461 7274 5f6c 6162 656c 72dc 0000  estart_labelr...
-000043e0: 0072 3e00 0000 72e2 0000 0072 e500 0000  .r>...r....r....
-000043f0: 72e8 0000 0072 be00 0000 724d 0000 0072  r....r....rM...r
-00004400: e100 0000 722c 0000 0072 4100 0000 d601  ....r,...rA.....
-00004410: 0000 7362 0000 000a 0106 0106 020c 020a  ..sb............
-00004420: 0114 0214 0112 0208 0104 ff16 0204 0104  ................
-00004430: ff16 0204 0104 ff16 0204 0104 ff14 0318  ................
-00004440: 0218 0118 0118 010c 020c 010c 020c 010c  ................
-00004450: 010c 010c 020c 010c 010c 010c 0208 020e  ................
-00004460: 0108 0b0a 0108 0314 0108 0614 0108 0614  ................
-00004470: 0108 060e 0108 0312 017a 1645 6469 7442  .........z.EditB
-00004480: 6f61 7264 5669 6577 2e5f 5f69 6e69 745f  oardView.__init_
-00004490: 5f63 0100 0000 0000 0000 0000 0000 0100  _c..............
-000044a0: 0000 0300 0000 4300 0000 724f 0000 0072  ......C...rO...r
-000044b0: 2e00 0000 7250 0000 0072 2900 0000 722b  ....rP...r)...r+
-000044c0: 0000 0072 2b00 0000 722c 0000 0072 5200  ...r+...r,...rR.
-000044d0: 0000 2f02 0000 7253 0000 007a 1a45 6469  ../...rS...z.Edi
-000044e0: 7442 6f61 7264 5669 6577 2e6f 6e5f 7368  tBoardView.on_sh
-000044f0: 6f77 5f76 6965 7763 0100 0000 0000 0000  ow_viewc........
-00004500: 0000 0000 0100 0000 0200 0000 4300 0000  ............C...
-00004510: 7254 0000 0072 2e00 0000 7255 0000 0072  rT...r....rU...r
-00004520: 2900 0000 722b 0000 0072 2b00 0000 722c  )...r+...r+...r,
-00004530: 0000 0072 5700 0000 3302 0000 7258 0000  ...rW...3...rX..
-00004540: 007a 1a45 6469 7442 6f61 7264 5669 6577  .z.EditBoardView
-00004550: 2e6f 6e5f 6869 6465 5f76 6965 77da 0178  .on_hide_view..x
-00004560: da01 79da 0662 7574 746f 6eda 096d 6f64  ..y..button..mod
-00004570: 6966 6965 7273 6305 0000 0000 0000 0000  ifiersc.........
-00004580: 0000 0006 0000 0004 0000 0043 0000 0073  ...........C...s
-00004590: 0609 0000 6400 7d05 6401 7c01 0400 0300  ....d.}.d.|.....
-000045a0: 6b00 720c 6402 6b00 721c 6e02 0100 6e0e  k.r.d.k.r.n...n.
-000045b0: 6403 7c02 0400 0300 6b00 7218 6404 6b00  d.|.....k.r.d.k.
-000045c0: 721c 6e02 0100 6e02 6405 7d05 6402 7c01  r.n...n.d.}.d.|.
-000045d0: 0400 0300 6b00 7226 6406 6b00 7236 6e02  ....k.r&d.k.r6n.
-000045e0: 0100 6e0e 6403 7c02 0400 0300 6b00 7232  ..n.d.|.....k.r2
-000045f0: 6404 6b00 7236 6e02 0100 6e02 6407 7d05  d.k.r6n...n.d.}.
-00004600: 6406 7c01 0400 0300 6b00 7240 6408 6b00  d.|.....k.r@d.k.
-00004610: 7250 6e02 0100 6e0e 6403 7c02 0400 0300  rPn...n.d.|.....
-00004620: 6b00 724c 6404 6b00 7250 6e02 0100 6e02  k.rLd.k.rPn...n.
-00004630: 6409 7d05 6408 7c01 0400 0300 6b00 725a  d.}.d.|.....k.rZ
-00004640: 640a 6b00 726a 6e02 0100 6e0e 6403 7c02  d.k.rjn...n.d.|.
-00004650: 0400 0300 6b00 7266 6404 6b00 726a 6e02  ....k.rfd.k.rjn.
-00004660: 0100 6e02 640b 7d05 640a 7c01 0400 0300  ..n.d.}.d.|.....
-00004670: 6b00 7274 640c 6b00 7284 6e02 0100 6e0e  k.rtd.k.r.n...n.
-00004680: 6403 7c02 0400 0300 6b00 7280 6404 6b00  d.|.....k.r.d.k.
-00004690: 7284 6e02 0100 6e02 640d 7d05 640c 7c01  r.n...n.d.}.d.|.
-000046a0: 0400 0300 6b00 728e 640e 6b00 729e 6e02  ....k.r.d.k.r.n.
-000046b0: 0100 6e0e 6403 7c02 0400 0300 6b00 729a  ..n.d.|.....k.r.
-000046c0: 6404 6b00 729e 6e02 0100 6e02 640f 7d05  d.k.r.n...n.d.}.
-000046d0: 6401 7c01 0400 0300 6b00 72a8 6402 6b00  d.|.....k.r.d.k.
-000046e0: 72b8 6e02 0100 6e0e 6410 7c02 0400 0300  r.n...n.d.|.....
-000046f0: 6b00 72b4 6411 6b00 72b8 6e02 0100 6e02  k.r.d.k.r.n...n.
-00004700: 6412 7d05 6402 7c01 0400 0300 6b00 72c2  d.}.d.|.....k.r.
-00004710: 6406 6b00 72d2 6e02 0100 6e0e 6410 7c02  d.k.r.n...n.d.|.
-00004720: 0400 0300 6b00 72ce 6411 6b00 72d2 6e02  ....k.r.d.k.r.n.
-00004730: 0100 6e02 6413 7d05 6406 7c01 0400 0300  ..n.d.}.d.|.....
-00004740: 6b00 72dc 6408 6b00 72ec 6e02 0100 6e0e  k.r.d.k.r.n...n.
-00004750: 6410 7c02 0400 0300 6b00 72e8 6411 6b00  d.|.....k.r.d.k.
-00004760: 72ec 6e02 0100 6e02 6414 7d05 6408 7c01  r.n...n.d.}.d.|.
-00004770: 0400 0300 6b00 72f7 640a 6b00 9001 7209  ....k.r.d.k...r.
-00004780: 6e02 0100 6e10 6410 7c02 0400 0300 6b00  n...n.d.|.....k.
-00004790: 9001 7205 6411 6b00 9001 7209 6e02 0100  ..r.d.k...r.n...
-000047a0: 6e02 6415 7d05 640a 7c01 0400 0300 6b00  n.d.}.d.|.....k.
-000047b0: 9001 7215 640c 6b00 9001 7227 6e02 0100  ..r.d.k...r'n...
-000047c0: 6e10 6410 7c02 0400 0300 6b00 9001 7223  n.d.|.....k...r#
-000047d0: 6411 6b00 9001 7227 6e02 0100 6e02 6416  d.k...r'n...n.d.
-000047e0: 7d05 640c 7c01 0400 0300 6b00 9001 7233  }.d.|.....k...r3
-000047f0: 640e 6b00 9001 7245 6e02 0100 6e10 6410  d.k...rEn...n.d.
-00004800: 7c02 0400 0300 6b00 9001 7241 6411 6b00  |.....k...rAd.k.
-00004810: 9001 7245 6e02 0100 6e02 6417 7d05 6418  ..rEn...n.d.}.d.
-00004820: 7c01 0400 0300 6b00 9001 7251 6419 6b00  |.....k...rQd.k.
-00004830: 9001 7263 6e02 0100 6e10 6403 7c02 0400  ..rcn...n.d.|...
-00004840: 0300 6b00 9001 725f 6404 6b00 9001 7263  ..k...r_d.k...rc
-00004850: 6e02 0100 6e02 641a 7d05 6419 7c01 0400  n...n.d.}.d.|...
-00004860: 0300 6b00 9001 726f 641b 6b00 9001 7281  ..k...rod.k...r.
-00004870: 6e02 0100 6e10 6403 7c02 0400 0300 6b00  n...n.d.|.....k.
-00004880: 9001 727d 6404 6b00 9001 7281 6e02 0100  ..r}d.k...r.n...
-00004890: 6e02 641c 7d05 641b 7c01 0400 0300 6b00  n.d.}.d.|.....k.
-000048a0: 9001 728d 641d 6b00 9001 729f 6e02 0100  ..r.d.k...r.n...
-000048b0: 6e10 6403 7c02 0400 0300 6b00 9001 729b  n.d.|.....k...r.
-000048c0: 6404 6b00 9001 729f 6e02 0100 6e02 641e  d.k...r.n...n.d.
-000048d0: 7d05 641d 7c01 0400 0300 6b00 9001 72ab  }.d.|.....k...r.
-000048e0: 641f 6b00 9001 72bd 6e02 0100 6e10 6403  d.k...r.n...n.d.
-000048f0: 7c02 0400 0300 6b00 9001 72b9 6404 6b00  |.....k...r.d.k.
-00004900: 9001 72bd 6e02 0100 6e02 6420 7d05 641f  ..r.n...n.d }.d.
-00004910: 7c01 0400 0300 6b00 9001 72c9 6421 6b00  |.....k...r.d!k.
-00004920: 9001 72db 6e02 0100 6e10 6403 7c02 0400  ..r.n...n.d.|...
-00004930: 0300 6b00 9001 72d7 6404 6b00 9001 72db  ..k...r.d.k...r.
-00004940: 6e02 0100 6e02 6422 7d05 6421 7c01 0400  n...n.d"}.d!|...
-00004950: 0300 6b00 9001 72e7 6423 6b00 9001 72f9  ..k...r.d#k...r.
-00004960: 6e02 0100 6e10 6403 7c02 0400 0300 6b00  n...n.d.|.....k.
-00004970: 9001 72f5 6404 6b00 9001 72f9 6e02 0100  ..r.d.k...r.n...
-00004980: 6e02 6424 7d05 6418 7c01 0400 0300 6b00  n.d$}.d.|.....k.
-00004990: 9002 7205 6419 6b00 9002 7217 6e02 0100  ..r.d.k...r.n...
-000049a0: 6e10 6410 7c02 0400 0300 6b00 9002 7213  n.d.|.....k...r.
-000049b0: 6411 6b00 9002 7217 6e02 0100 6e02 6425  d.k...r.n...n.d%
-000049c0: 7d05 6419 7c01 0400 0300 6b00 9002 7223  }.d.|.....k...r#
-000049d0: 641b 6b00 9002 7235 6e02 0100 6e10 6410  d.k...r5n...n.d.
-000049e0: 7c02 0400 0300 6b00 9002 7231 6411 6b00  |.....k...r1d.k.
-000049f0: 9002 7235 6e02 0100 6e02 6426 7d05 641b  ..r5n...n.d&}.d.
-00004a00: 7c01 0400 0300 6b00 9002 7241 641d 6b00  |.....k...rAd.k.
-00004a10: 9002 7253 6e02 0100 6e10 6410 7c02 0400  ..rSn...n.d.|...
-00004a20: 0300 6b00 9002 724f 6411 6b00 9002 7253  ..k...rOd.k...rS
-00004a30: 6e02 0100 6e02 6427 7d05 641d 7c01 0400  n...n.d'}.d.|...
-00004a40: 0300 6b00 9002 725f 641f 6b00 9002 7271  ..k...r_d.k...rq
-00004a50: 6e02 0100 6e10 6410 7c02 0400 0300 6b00  n...n.d.|.....k.
-00004a60: 9002 726d 6411 6b00 9002 7271 6e02 0100  ..rmd.k...rqn...
-00004a70: 6e02 6428 7d05 641f 7c01 0400 0300 6b00  n.d(}.d.|.....k.
-00004a80: 9002 727d 6421 6b00 9002 728f 6e02 0100  ..r}d!k...r.n...
-00004a90: 6e10 6410 7c02 0400 0300 6b00 9002 728b  n.d.|.....k...r.
-00004aa0: 6411 6b00 9002 728f 6e02 0100 6e02 6429  d.k...r.n...n.d)
-00004ab0: 7d05 6421 7c01 0400 0300 6b00 9002 729b  }.d!|.....k...r.
-00004ac0: 6423 6b00 9002 72ad 6e02 0100 6e10 6410  d#k...r.n...n.d.
-00004ad0: 7c02 0400 0300 6b00 9002 72a9 6411 6b00  |.....k...r.d.k.
-00004ae0: 9002 72ad 6e02 0100 6e02 642a 7d05 642b  ..r.n...n.d*}.d+
-00004af0: 7c01 0400 0300 6b00 9002 72b9 642c 6b00  |.....k...r.d,k.
-00004b00: 9002 72cb 6e02 0100 6e10 642d 7c02 0400  ..r.n...n.d-|...
-00004b10: 0300 6b00 9002 72c7 642e 6b00 9002 72cb  ..k...r.d.k...r.
-00004b20: 6e02 0100 6e02 642f 7d05 642b 7c01 0400  n...n.d/}.d+|...
-00004b30: 0300 6b00 9002 72d7 642c 6b00 9002 72e9  ..k...r.d,k...r.
-00004b40: 6e02 0100 6e10 6430 7c02 0400 0300 6b00  n...n.d0|.....k.
-00004b50: 9002 72e5 6431 6b00 9002 72e9 6e02 0100  ..r.d1k...r.n...
-00004b60: 6e02 6432 7d05 6433 7c01 0400 0300 6b00  n.d2}.d3|.....k.
-00004b70: 9002 72f5 6434 6b00 9003 7207 6e02 0100  ..r.d4k...r.n...
-00004b80: 6e10 6431 7c02 0400 0300 6b00 9003 7203  n.d1|.....k...r.
-00004b90: 642d 6b00 9003 7207 6e02 0100 6e02 6435  d-k...r.n...n.d5
-00004ba0: 7d05 6436 7c01 0400 0300 6b00 9003 7213  }.d6|.....k...r.
-00004bb0: 6437 6b00 9003 7225 6e02 0100 6e10 6431  d7k...r%n...n.d1
-00004bc0: 7c02 0400 0300 6b00 9003 7221 642d 6b00  |.....k...r!d-k.
-00004bd0: 9003 7225 6e02 0100 6e02 6438 7d05 7c05  ..r%n...n.d8}.|.
-00004be0: 6435 6b02 9003 726d 7c00 6a00 6439 6b02  d5k...rm|.j.d9k.
-00004bf0: 9003 7249 7c00 6a01 6a02 6a03 7c05 1900  ..rI|.j.j.j.|...
-00004c00: 6405 6b04 9003 7247 7c00 6a01 6a02 6a03  d.k...rG|.j.j.j.
-00004c10: 7c05 0500 1900 643a 3700 0300 3c00 6400  |.....d:7...<.d.
-00004c20: 5300 6400 5300 7c00 6a00 643b 6b02 9003  S.d.S.|.j.d;k...
-00004c30: 725c 7c00 6a01 6a02 6a03 7c05 0500 1900  r\|.j.j.j.|.....
-00004c40: 6407 3700 0300 3c00 6400 5300 7c00 6a00  d.7...<.d.S.|.j.
-00004c50: 643c 6b02 9003 726b 6405 7c00 6a01 6a02  d<k...rkd.|.j.j.
-00004c60: 6a03 7c05 3c00 6400 5300 6400 5300 7c05  j.|.<.d.S.d.S.|.
-00004c70: 6438 6b02 9003 72b5 7c00 6a00 6439 6b02  d8k...r.|.j.d9k.
-00004c80: 9003 7285 7c00 6a01 6a02 6a03 7c05 0500  ..r.|.j.j.j.|...
-00004c90: 1900 6407 3700 0300 3c00 6400 5300 7c00  ..d.7...<.d.S.|.
-00004ca0: 6a00 643b 6b02 9003 72a4 7c00 6a01 6a02  j.d;k...r.|.j.j.
-00004cb0: 6a03 7c05 1900 6405 6b04 9003 72a2 7c00  j.|...d.k...r.|.
-00004cc0: 6a01 6a02 6a03 7c05 0500 1900 643a 3700  j.j.j.|.....d:7.
-00004cd0: 0300 3c00 6400 5300 6400 5300 7c00 6a00  ..<.d.S.d.S.|.j.
-00004ce0: 643c 6b02 9003 72b3 6405 7c00 6a01 6a02  d<k...r.d.|.j.j.
-00004cf0: 6a03 7c05 3c00 6400 5300 6400 5300 7c05  j.|.<.d.S.d.S.|.
-00004d00: 642f 6b02 9003 72fd 7c00 6a00 6439 6b02  d/k...r.|.j.d9k.
-00004d10: 9003 72cd 7c00 6a01 6a02 6a03 7c05 0500  ..r.|.j.j.j.|...
-00004d20: 1900 6407 3700 0300 3c00 6400 5300 7c00  ..d.7...<.d.S.|.
-00004d30: 6a00 643b 6b02 9003 72ec 7c00 6a01 6a02  j.d;k...r.|.j.j.
-00004d40: 6a03 7c05 1900 6405 6b04 9003 72ea 7c00  j.|...d.k...r.|.
-00004d50: 6a01 6a02 6a03 7c05 0500 1900 643a 3700  j.j.j.|.....d:7.
-00004d60: 0300 3c00 6400 5300 6400 5300 7c00 6a00  ..<.d.S.d.S.|.j.
-00004d70: 643c 6b02 9003 72fb 6405 7c00 6a01 6a02  d<k...r.d.|.j.j.
-00004d80: 6a03 7c05 3c00 6400 5300 6400 5300 7c05  j.|.<.d.S.d.S.|.
-00004d90: 6432 6b02 9004 7245 7c00 6a00 6439 6b02  d2k...rE|.j.d9k.
-00004da0: 9004 7221 7c00 6a01 6a02 6a03 7c05 1900  ..r!|.j.j.j.|...
-00004db0: 6405 6b04 9004 721f 7c00 6a01 6a02 6a03  d.k...r.|.j.j.j.
-00004dc0: 7c05 0500 1900 643a 3700 0300 3c00 6400  |.....d:7...<.d.
-00004dd0: 5300 6400 5300 7c00 6a00 643b 6b02 9004  S.d.S.|.j.d;k...
-00004de0: 7234 7c00 6a01 6a02 6a03 7c05 0500 1900  r4|.j.j.j.|.....
-00004df0: 6407 3700 0300 3c00 6400 5300 7c00 6a00  d.7...<.d.S.|.j.
-00004e00: 643c 6b02 9004 7243 6405 7c00 6a01 6a02  d<k...rCd.|.j.j.
-00004e10: 6a03 7c05 3c00 6400 5300 6400 5300 7c05  j.|.<.d.S.d.S.|.
-00004e20: 6400 6b03 9004 727f 7c00 6a00 6439 6b02  d.k...r.|.j.d9k.
-00004e30: 9004 725d 7c00 6a01 6a02 6a03 7c05 0500  ..r]|.j.j.j.|...
-00004e40: 1900 6407 3700 0300 3c00 6400 5300 7c00  ..d.7...<.d.S.|.
-00004e50: 6a00 643b 6b02 9004 7270 7c00 6a01 6a02  j.d;k...rp|.j.j.
-00004e60: 6a03 7c05 0500 1900 643a 3700 0300 3c00  j.|.....d:7...<.
-00004e70: 6400 5300 7c00 6a00 643c 6b02 9004 7281  d.S.|.j.d<k...r.
-00004e80: 6405 7c00 6a01 6a02 6a03 7c05 3c00 6400  d.|.j.j.j.|.<.d.
-00004e90: 5300 6400 5300 6400 5300 293d 4ee9 d800  S.d.S.d.S.)=N...
-00004ea0: 0000 6914 0100 0069 e401 0000 69fe 0200  ..i....i....i...
-00004eb0: 0072 0100 0000 6950 0100 0072 9400 0000  .r....iP...r....
-00004ec0: 698c 0100 0072 9500 0000 69c8 0100 00e9  i....r....i.....
-00004ed0: 0300 0000 6904 0200 00e9 0400 0000 6940  ....i.........i@
-00004ee0: 0200 00e9 0500 0000 e92c 0000 0069 3c01  .........,...i<.
-00004ef0: 0000 e917 0000 00e9 1600 0000 e915 0000  ................
-00004f00: 0072 0d00 0000 e913 0000 00e9 1200 0000  .r..............
-00004f10: 6970 0200 0069 ac02 0000 e906 0000 0069  ip...i.........i
-00004f20: e802 0000 e907 0000 0069 2403 0000 e908  .........i$.....
-00004f30: 0000 0069 6003 0000 e909 0000 0069 9c03  ...i`........i..
-00004f40: 0000 7269 0000 0069 d803 0000 e90b 0000  ..ri...i........
-00004f50: 00e9 1100 0000 728d 0000 0072 6a00 0000  ......r....rj...
-00004f60: e90e 0000 00e9 0d00 0000 e90c 0000 00e9  ................
-00004f70: 7800 0000 e9b4 0000 0069 c201 0000 69ee  x........i....i.
-00004f80: 0200 00e9 1b00 0000 726f 0000 0069 5e01  ........ro...i^.
-00004f90: 0000 e91a 0000 0069 f901 0000 692b 0200  .......i....i+..
-00004fa0: 00e9 1800 0000 7274 0000 0072 6d00 0000  ......rt...rm...
-00004fb0: e919 0000 0072 de00 0000 e9ff ffff ff72  .....r.........r
-00004fc0: e400 0000 72e6 0000 0029 0472 df00 0000  ....r....).r....
-00004fd0: 7220 0000 0072 2100 0000 72d0 0000 0029  r ...r!...r....)
-00004fe0: 0672 2a00 0000 72f2 0000 0072 f300 0000  .r*...r....r....
-00004ff0: 72f4 0000 0072 f500 0000 da08 706f 7369  r....r......posi
-00005000: 7469 6f6e 722b 0000 0072 2b00 0000 722c  tionr+...r+...r,
-00005010: 0000 00da 0e6f 6e5f 6d6f 7573 655f 7072  .....on_mouse_pr
-00005020: 6573 7336 0200 0073 d400 0000 0401 3001  ess6...s......0.
-00005030: 0401 3001 0401 3001 0401 3001 0401 3001  ..0...0...0...0.
-00005040: 0401 3001 0401 3001 0401 3001 0401 3001  ..0...0...0...0.
-00005050: 0401 3601 0401 3801 0401 3801 0401 3801  ..6...8...8...8.
-00005060: 0401 3801 0401 3801 0401 3801 0401 3801  ..8...8...8...8.
-00005070: 0401 3801 0401 3801 0401 3801 0401 3801  ..8...8...8...8.
-00005080: 0401 3801 0401 3801 0401 3801 0401 3801  ..8...8...8...8.
-00005090: 0401 3801 0401 3801 0401 3801 0401 0a02  ..8...8...8.....
-000050a0: 0c01 1401 1a01 04ff 0c02 1a01 0c01 1201  ................
-000050b0: 04ff 0a02 0c01 1a01 0c01 1401 1a01 04ff  ................
-000050c0: 0c02 1201 04ff 0a02 0c01 1a01 0c01 1401  ................
-000050d0: 1a01 04ff 0c02 1201 04ff 0a02 0c01 1401  ................
-000050e0: 1a01 04ff 0c02 1a01 0c01 1201 04ff 0a02  ................
-000050f0: 0c01 1a01 0c01 1a01 0c01 1201 04fa 0405  ................
-00005100: 7a1c 4564 6974 426f 6172 6456 6965 772e  z.EditBoardView.
-00005110: 6f6e 5f6d 6f75 7365 5f70 7265 7373 6301  on_mouse_pressc.
-00005120: 0000 0000 0000 0000 0000 0001 0000 0004  ................
-00005130: 0000 0043 0000 0073 3e00 0000 7c00 a000  ...C...s>...|...
-00005140: a100 0100 7401 a002 a100 0100 7401 a003  ....t.......t...
-00005150: 7c00 6a04 6a05 6a06 7c00 6a04 6a05 6a07  |.j.j.j.|.j.j.j.
-00005160: a102 0100 7401 a008 a100 0100 7c00 6a09  ....t.......|.j.
-00005170: a00a a100 0100 6400 5300 722e 0000 0029  ......d.S.r....)
-00005180: 0b72 5b00 0000 7204 0000 0072 ce00 0000  .r[...r....r....
-00005190: 72cf 0000 0072 2000 0000 7221 0000 0072  r....r ...r!...r
-000051a0: d000 0000 72a8 0000 00da 0c44 7261 7742  ....r......DrawB
-000051b0: 6172 426f 7865 7372 4400 0000 725c 0000  arBoxesrD...r\..
-000051c0: 0072 2900 0000 722b 0000 0072 2b00 0000  .r)...r+...r+...
-000051d0: 722c 0000 0072 5d00 0000 9902 0000 730a  r,...r].......s.
-000051e0: 0000 0008 0108 0218 0108 010e 017a 1545  .............z.E
-000051f0: 6469 7442 6f61 7264 5669 6577 2e6f 6e5f  ditBoardView.on_
-00005200: 6472 6177 290a 7260 0000 0072 6100 0000  draw).r`...ra...
-00005210: 7262 0000 0072 4100 0000 7252 0000 0072  rb...rA...rR...r
-00005220: 5700 0000 72b3 0000 0072 1101 0000 725d  W...r....r....r]
-00005230: 0000 0072 6300 0000 722b 0000 0072 2b00  ...rc...r+...r+.
-00005240: 0000 724d 0000 0072 2c00 0000 72bd 0000  ..rM...r,...r...
-00005250: 00d5 0100 0073 0c00 0000 0800 0c01 0859  .....s.........Y
-00005260: 0804 1a03 1063 72bd 0000 0063 0000 0000  .....cr....c....
-00005270: 0000 0000 0000 0000 0000 0000 0300 0000  ................
-00005280: 0000 0000 7205 0000 0029 0972 ea00 0000  ....r....).r....
-00005290: 6302 0000 0000 0000 0000 0000 0006 0000  c...............
-000052a0: 0007 0000 0003 0000 0073 a000 0000 7400  .........s....t.
-000052b0: 8300 a001 a100 0100 7c01 8800 5f02 7403  ........|..._.t.
-000052c0: 6a04 a005 a100 8800 5f06 8800 6a06 a007  j......._...j...
-000052d0: a100 0100 6401 6402 8400 8800 6a08 6a09  ....d.d.....j.j.
-000052e0: 6a0a 4400 8301 7d02 6403 a00b 7c02 a101  j.D...}.d...|...
-000052f0: 7d03 7403 6a04 a00c 6404 6405 6406 6407  }.t.j...d.d.d.d.
-00005300: 6408 a105 7d04 7403 6a04 a00d 6409 640a  d...}.t.j...d.d.
-00005310: 640b 6407 7c03 a105 8901 8800 6a06 a00e  d.d.|.......j...
-00005320: 7c04 a101 0100 8800 6a06 a00e 8801 a101  |.......j.......
-00005330: 0100 7c04 a00f 640c a101 8700 8701 6602  ..|...d.......f.
-00005340: 640d 640e 8408 8301 7d05 6400 5300 290f  d.d.....}.d.S.).
-00005350: 4e63 0100 0000 0000 0000 0000 0000 0200  Nc..............
-00005360: 0000 0400 0000 5300 0000 72b1 0000 0072  ......S...r....r
-00005370: 2b00 0000 2901 da03 7374 7272 b400 0000  +...)...strr....
-00005380: 722b 0000 0072 2b00 0000 722c 0000 0072  r+...r+...r,...r
-00005390: b700 0000 ab02 0000 72b8 0000 007a 2e45  ........r....z.E
-000053a0: 6469 7441 7353 7472 696e 675f 5669 6577  ditAsString_View
-000053b0: 2e5f 5f69 6e69 745f 5f2e 3c6c 6f63 616c  .__init__.<local
-000053c0: 733e 2e3c 6c69 7374 636f 6d70 3efa 022c  s>.<listcomp>..,
-000053d0: 2069 2602 0000 7211 0000 0072 6400 0000   i&...r....rd...
-000053e0: 726f 0000 0072 d600 0000 6945 0100 00e9  ro...r....iE....
-000053f0: 7701 0000 e958 0200 0072 1b00 0000 6301  w....X...r....c.
-00005400: 0000 0000 0000 0000 0000 0005 0000 000a  ................
-00005410: 0000 0013 0000 0073 a400 0000 8801 6a00  .......s......j.
-00005420: 6a01 6401 6402 8d01 7d01 7a09 6403 6404  j.d.d...}.z.d.d.
-00005430: 8400 7c01 4400 8301 7d02 5700 6e16 0100  ..|.D...}.W.n...
-00005440: 0100 0100 7402 6a03 6a04 6405 6406 6407  ....t.j.j.d.d.d.
-00005450: 6400 6408 6701 6409 8d05 7d03 8800 6a05  d.d.g.d...}...j.
-00005460: a006 7c03 a101 0100 5900 7407 a008 7c02  ..|.....Y.t...|.
-00005470: a101 723e 7c02 8800 6a09 6a0a 5f0b 740c  ..r>|...j.j._.t.
-00005480: 8800 6a0d 8301 7d04 8800 6a09 a00e 7c04  ..j...}...j...|.
-00005490: a101 0100 6400 5300 7402 6a03 6a04 6405  ....d.S.t.j.j.d.
-000054a0: 6406 6407 6400 6408 6701 6409 8d05 7d03  d.d.d.d.g.d...}.
-000054b0: 8800 6a05 a006 7c03 a101 0100 6400 5300  ..j...|.....d.S.
-000054c0: 290a 4e72 1401 0000 72af 0000 0063 0100  ).Nr....r....c..
-000054d0: 0000 0000 0000 0000 0000 0200 0000 0400  ................
-000054e0: 0000 5300 0000 72b1 0000 0072 2b00 0000  ..S...r....r+...
-000054f0: 72b2 0000 0072 b400 0000 722b 0000 0072  r....r....r+...r
-00005500: 2b00 0000 722c 0000 0072 b700 0000 ba02  +...r,...r......
-00005510: 0000 72b8 0000 007a 4545 6469 7441 7353  ..r....zEEditAsS
-00005520: 7472 696e 675f 5669 6577 2e5f 5f69 6e69  tring_View.__ini
-00005530: 745f 5f2e 3c6c 6f63 616c 733e 2e6f 6e5f  t__.<locals>.on_
-00005540: 636c 6963 6b5f 446f 6e65 2e3c 6c6f 6361  click_Done.<loca
-00005550: 6c73 3e2e 3c6c 6973 7463 6f6d 703e 7211  ls>.<listcomp>r.
-00005560: 0000 0072 6600 0000 7a59 4572 726f 723a  ...rf...zYError:
-00005570: 200a 5468 6973 2069 6e20 6e6f 7420 6120   .This in not a 
-00005580: 6c65 6761 6c20 4261 636b 6761 6d6d 6f6e  legal Backgammon
-00005590: 2062 6f61 7264 2073 7472 696e 672e 2050   board string. P
-000055a0: 6c65 6173 6520 5072 6f76 6964 6520 6120  lease Provide a 
-000055b0: 6c65 6761 6c20 626f 6172 6420 7374 7269  legal board stri
-000055c0: 6e67 2e72 9900 0000 729a 0000 0029 0f72  ng.r....r....).r
-000055d0: 0a00 0000 72ba 0000 0072 3c00 0000 7242  ....r....r<...rB
-000055e0: 0000 0072 a900 0000 7244 0000 0072 4800  ...r....rD...rH.
-000055f0: 0000 7203 0000 0072 db00 0000 7220 0000  ..r....r....r ..
-00005600: 0072 2100 0000 72d0 0000 0072 bd00 0000  .r!...r....r....
-00005610: 7225 0000 0072 2600 0000 2905 7227 0000  r%...r&...).r'..
-00005620: 00da 0a73 7472 696e 674c 6973 745a 076e  ...stringListZ.n
-00005630: 756d 4c69 7374 72ab 0000 0072 eb00 0000  umListr....r....
-00005640: a902 722a 0000 005a 0a74 6578 745f 696e  ..r*...Z.text_in
-00005650: 7075 7472 2b00 0000 722c 0000 0072 dc00  putr+...r,...r..
-00005660: 0000 b402 0000 7324 0000 000e 0302 0212  ......s$........
-00005670: 0106 010a 0102 0106 0106 fe0e 030a 020a  ................
-00005680: 010a 0110 010a 0202 0106 0106 fe10 037a  ...............z
-00005690: 3145 6469 7441 7353 7472 696e 675f 5669  1EditAsString_Vi
-000056a0: 6577 2e5f 5f69 6e69 745f 5f2e 3c6c 6f63  ew.__init__.<loc
-000056b0: 616c 733e 2e6f 6e5f 636c 6963 6b5f 446f  als>.on_click_Do
-000056c0: 6e65 2910 7240 0000 0072 4100 0000 7225  ne).r@...rA...r%
-000056d0: 0000 0072 3c00 0000 7242 0000 0072 4300  ...r<...rB...rC.
-000056e0: 0000 7244 0000 0072 4500 0000 7220 0000  ..rD...rE...r ..
-000056f0: 0072 2100 0000 72d0 0000 00da 046a 6f69  .r!...r......joi
-00005700: 6e72 4a00 0000 7285 0000 0072 4800 0000  nrJ...r....rH...
-00005710: 7227 0000 0029 0672 2a00 0000 7225 0000  r'...).r*...r%..
-00005720: 0072 1701 0000 da06 7374 7269 6e67 72f1  .r......stringr.
-00005730: 0000 0072 dc00 0000 724d 0000 0072 1801  ...r....rM...r..
-00005740: 0000 722c 0000 0072 4100 0000 a402 0000  ..r,...rA.......
-00005750: 7318 0000 000a 0106 010c 020a 0114 020a  s...............
-00005760: 0114 0214 010c 020c 0108 0214 017a 1a45  .............z.E
-00005770: 6469 7441 7353 7472 696e 675f 5669 6577  ditAsString_View
-00005780: 2e5f 5f69 6e69 745f 5f63 0100 0000 0000  .__init__c......
-00005790: 0000 0000 0000 0100 0000 0300 0000 4300  ..............C.
-000057a0: 0000 724f 0000 0072 2e00 0000 7250 0000  ..rO...r....rP..
-000057b0: 0072 2900 0000 722b 0000 0072 2b00 0000  .r)...r+...r+...
-000057c0: 722c 0000 0072 5200 0000 cb02 0000 7253  r,...rR.......rS
-000057d0: 0000 007a 1e45 6469 7441 7353 7472 696e  ...z.EditAsStrin
-000057e0: 675f 5669 6577 2e6f 6e5f 7368 6f77 5f76  g_View.on_show_v
-000057f0: 6965 7763 0100 0000 0000 0000 0000 0000  iewc............
-00005800: 0100 0000 0200 0000 4300 0000 7254 0000  ........C...rT..
-00005810: 0072 2e00 0000 7255 0000 0072 2900 0000  .r....rU...r)...
-00005820: 722b 0000 0072 2b00 0000 722c 0000 0072  r+...r+...r,...r
-00005830: 5700 0000 cf02 0000 7258 0000 007a 1e45  W.......rX...z.E
-00005840: 6469 7441 7353 7472 696e 675f 5669 6577  ditAsString_View
-00005850: 2e6f 6e5f 6869 6465 5f76 6965 7763 0100  .on_hide_viewc..
-00005860: 0000 0000 0000 0000 0000 0100 0000 0800  ................
-00005870: 0000 4300 0000 7340 0000 007c 00a0 00a1  ..C...s@...|....
-00005880: 0001 0074 01a0 0264 0164 0264 0164 0374  ...t...d.d.d.d.t
-00005890: 036a 04a1 0501 0074 01a0 0564 0164 0264  .j.....t...d.d.d
-000058a0: 0164 0374 036a 0464 04a1 0601 007c 006a  .d.t.j.d.....|.j
-000058b0: 06a0 07a1 0001 0064 0053 0029 054e 7216  .......d.S.).Nr.
-000058c0: 0100 00e9 9001 0000 726f 0000 0072 0001  ........ro...r..
-000058d0: 0000 2908 725b 0000 0072 3c00 0000 da15  ..).r[...r<.....
-000058e0: 6472 6177 5f72 6563 7461 6e67 6c65 5f66  draw_rectangle_f
-000058f0: 696c 6c65 6472 0400 0000 da0b 626f 6172  illedr......boar
-00005900: 645f 636f 6c6f 72da 1664 7261 775f 7265  d_color..draw_re
-00005910: 6374 616e 676c 655f 6f75 746c 696e 6572  ctangle_outliner
-00005920: 4400 0000 725c 0000 0072 2900 0000 722b  D...r\...r)...r+
-00005930: 0000 0072 2b00 0000 722c 0000 0072 5d00  ...r+...r,...r].
-00005940: 0000 d202 0000 7308 0000 0008 0114 0116  ......s.........
-00005950: 010e 027a 1945 6469 7441 7353 7472 696e  ...z.EditAsStrin
-00005960: 675f 5669 6577 2e6f 6e5f 6472 6177 725f  g_View.on_drawr_
-00005970: 0000 0072 2b00 0000 722b 0000 0072 4d00  ...r+...r+...rM.
-00005980: 0000 722c 0000 0072 ea00 0000 a202 0000  ..r,...r........
-00005990: 730a 0000 0008 000c 0208 2708 0410 0372  s.........'....r
-000059a0: ea00 0000 6300 0000 0000 0000 0000 0000  ....c...........
-000059b0: 0000 0000 0003 0000 0000 0000 0072 0500  .............r..
-000059c0: 0000 2909 7231 0000 0063 0200 0000 0000  ..).r1...c......
-000059d0: 0000 0000 0000 0a00 0000 0700 0000 0300  ................
-000059e0: 0000 73fe 0000 0074 0083 00a0 01a1 0001  ..s....t........
-000059f0: 007c 0188 005f 0274 036a 04a0 05a1 0088  .|..._.t.j......
-00005a00: 005f 0688 006a 06a0 07a1 0001 0074 036a  ._...j.......t.j
-00005a10: 04a0 0864 0164 0264 0364 0464 05a1 057d  ...d.d.d.d.d...}
-00005a20: 0274 036a 04a0 0864 0164 0664 0364 0464  .t.j...d.d.d.d.d
-00005a30: 07a1 057d 0374 036a 04a0 0864 0864 0964  ...}.t.j...d.d.d
-00005a40: 0a64 0b64 0ca1 057d 0474 036a 04a0 0864  .d.d...}.t.j...d
-00005a50: 0d64 0964 0a64 0b64 0ea1 057d 0588 006a  .d.d.d.d...}...j
-00005a60: 06a0 097c 02a1 0101 0088 006a 06a0 097c  ...|.......j...|
-00005a70: 03a1 0101 0088 006a 06a0 097c 04a1 0101  .......j...|....
-00005a80: 0088 006a 06a0 097c 05a1 0101 007c 02a0  ...j...|.....|..
-00005a90: 0a64 0fa1 0187 0066 0164 1064 1184 0883  .d.....f.d.d....
-00005aa0: 017d 067c 03a0 0a64 0fa1 0164 1264 1384  .}.|...d...d.d..
-00005ab0: 0083 017d 077c 04a0 0a64 0fa1 0187 0066  ...}.|...d.....f
-00005ac0: 0164 1464 1584 0883 017d 087c 05a0 0a64  .d.d.....}.|...d
-00005ad0: 0fa1 0187 0066 0164 1664 1784 0883 017d  .....f.d.d.....}
-00005ae0: 0964 0053 0029 184e 726a 0000 0072 6b00  .d.S.).Nrj...rk.
-00005af0: 0000 7208 0000 0072 1000 0000 726c 0000  ..r....r....rl..
-00005b00: 0072 6d00 0000 7214 0000 0072 1b01 0000  .rm...r....r....
-00005b10: 7215 0100 00e9 7d00 0000 726f 0000 00da  r.....}...ro....
-00005b20: 0452 6f6c 6c69 bc02 0000 7213 0000 0072  .Rolli....r....r
-00005b30: 1b00 0000 6301 0000 0000 0000 0000 0000  ....c...........
-00005b40: 0002 0000 0003 0000 0013 0000 0072 8f00  .............r..
-00005b50: 0000 722e 0000 0072 9000 0000 a902 7227  ..r....r......r'
-00005b60: 0000 005a 0c6d 6169 6e6d 656e 7556 6965  ...Z.mainmenuVie
-00005b70: 7772 2900 0000 722b 0000 0072 2c00 0000  wr)...r+...r,...
-00005b80: da0d 6f6e 5f63 6c69 636b 5f62 6163 6bf1  ..on_click_back.
-00005b90: 0200 0072 9100 0000 7a2d 5374 6172 745f  ...r....z-Start_
-00005ba0: 3250 5f56 6965 772e 5f5f 696e 6974 5f5f  2P_View.__init__
-00005bb0: 2e3c 6c6f 6361 6c73 3e2e 6f6e 5f63 6c69  .<locals>.on_cli
-00005bc0: 636b 5f62 6163 6b63 0100 0000 0000 0000  ck_backc........
-00005bd0: 0000 0000 0100 0000 0200 0000 5300 0000  ............S...
-00005be0: 723a 0000 0072 2e00 0000 723b 0000 0072  r:...r....r;...r
-00005bf0: 2f00 0000 722b 0000 0072 2b00 0000 722c  /...r+...r+...r,
-00005c00: 0000 0072 3e00 0000 f602 0000 723f 0000  ...r>.......r?..
-00005c10: 007a 2d53 7461 7274 5f32 505f 5669 6577  .z-Start_2P_View
-00005c20: 2e5f 5f69 6e69 745f 5f2e 3c6c 6f63 616c  .__init__.<local
-00005c30: 733e 2e6f 6e5f 636c 6963 6b5f 5175 6974  s>.on_click_Quit
-00005c40: 6301 0000 0000 0000 0000 0000 0004 0000  c...............
-00005c50: 0005 0000 0013 0000 0073 8000 0000 7400  .........s....t.
-00005c60: a001 6401 6402 a102 7d01 7402 6a03 7c01  ..d.d...}.t.j.|.
-00005c70: 6403 6404 6405 8d03 8800 6a04 5f05 8800  d.d.d.....j._...
-00005c80: 6a04 6a05 a006 8800 6a04 6a07 a101 0100  j.j.....j.j.....
-00005c90: 8800 6a04 6a05 a008 8800 6a04 6a07 a101  ..j.j.....j.j...
-00005ca0: 0100 7c01 6401 6b02 7233 7409 8800 6a0a  ..|.d.k.r3t...j.
-00005cb0: 8301 7d02 8800 6a04 a00b 7c02 a101 0100  ..}...j...|.....
-00005cc0: 6400 5300 740c 8800 6a0a 8301 7d03 8800  d.S.t...j...}...
-00005cd0: 6a04 a00b 7c03 a101 0100 6400 5300 2906  j...|.....d.S.).
-00005ce0: 4e72 9400 0000 7295 0000 0072 1d00 0000  Nr....r....r....
-00005cf0: 5472 9600 0000 290d 72a1 0000 0072 a200  Tr....).r....r..
-00005d00: 0000 7203 0000 0072 a300 0000 7220 0000  ..r....r....r ..
-00005d10: 0072 a400 0000 da1e 7570 6461 7465 506f  .r......updatePo
-00005d20: 7373 6962 6c65 4d6f 7665 7348 756d 616e  ssibleMovesHuman
-00005d30: 466f 726d 6174 7221 0000 00da 0e66 6f72  Formatr!.....for
-00005d40: 6d53 7072 6974 654c 6973 74da 0f50 315f  mSpriteList..P1_
-00005d50: 5475 726e 5f32 505f 5669 6577 7225 0000  Turn_2P_Viewr%..
-00005d60: 0072 2600 0000 da0f 5032 5f54 7572 6e5f  .r&.....P2_Turn_
-00005d70: 3250 5f56 6965 7729 0472 2700 0000 5a0b  2P_View).r'...Z.
-00005d80: 6669 7273 7450 6c61 7965 725a 0b70 6c61  firstPlayerZ.pla
-00005d90: 7965 7231 7669 6577 5a0b 706c 6179 6572  yer1viewZ.player
-00005da0: 3276 6965 7772 2900 0000 722b 0000 0072  2viewr)...r+...r
-00005db0: 2c00 0000 da0d 6f6e 5f63 6c69 636b 5f72  ,.....on_click_r
-00005dc0: 6f6c 6cfa 0200 0073 1200 0000 0c02 1402  oll....s........
-00005dd0: 1201 1201 0802 0a01 1001 0a02 1001 7a2d  ..............z-
-00005de0: 5374 6172 745f 3250 5f56 6965 772e 5f5f  Start_2P_View.__
-00005df0: 696e 6974 5f5f 2e3c 6c6f 6361 6c73 3e2e  init__.<locals>.
-00005e00: 6f6e 5f63 6c69 636b 5f72 6f6c 6c63 0100  on_click_rollc..
-00005e10: 0000 0000 0000 0000 0000 0200 0000 0300  ................
-00005e20: 0000 1300 0000 7233 0000 0072 2e00 0000  ......r3...r....
-00005e30: 7234 0000 0072 3700 0000 7229 0000 0072  r4...r7...r)...r
-00005e40: 2b00 0000 722c 0000 0072 3800 0000 0903  +...r,...r8.....
-00005e50: 0000 7239 0000 007a 3153 7461 7274 5f32  ..r9...z1Start_2
-00005e60: 505f 5669 6577 2e5f 5f69 6e69 745f 5f2e  P_View.__init__.
-00005e70: 3c6c 6f63 616c 733e 2e6f 6e5f 636c 6963  <locals>.on_clic
-00005e80: 6b5f 5365 7474 696e 6773 a90b 7240 0000  k_Settings..r@..
-00005e90: 0072 4100 0000 7225 0000 0072 3c00 0000  .rA...r%...r<...
-00005ea0: 7242 0000 0072 4300 0000 7244 0000 0072  rB...rC...rD...r
-00005eb0: 4500 0000 724a 0000 0072 4800 0000 7227  E...rJ...rH...r'
-00005ec0: 0000 0029 0a72 2a00 0000 7225 0000 0072  ...).r*...r%...r
-00005ed0: 8600 0000 7287 0000 00da 0b52 6f6c 6c5f  ....r......Roll_
-00005ee0: 6275 7474 6f6e da0f 5365 7474 696e 6773  button..Settings
-00005ef0: 5f62 7574 746f 6e72 2201 0000 723e 0000  _buttonr"...r>..
-00005f00: 0072 2701 0000 7238 0000 0072 4d00 0000  .r'...r8...rM...
-00005f10: 7229 0000 0072 2c00 0000 7241 0000 00e0  r)...r,...rA....
-00005f20: 0200 0073 2800 0000 0a01 0601 0c02 0a01  ...s(...........
-00005f30: 1402 1401 1401 1401 0c02 0c01 0c01 0c01  ................
-00005f40: 0802 0e01 0804 0a01 0803 0e01 080e 1201  ................
-00005f50: 7a16 5374 6172 745f 3250 5f56 6965 772e  z.Start_2P_View.
-00005f60: 5f5f 696e 6974 5f5f 6301 0000 0000 0000  __init__c.......
-00005f70: 0000 0000 0001 0000 0003 0000 0043 0000  .............C..
-00005f80: 0072 4f00 0000 722e 0000 0072 5000 0000  .rO...r....rP...
-00005f90: 7229 0000 0072 2b00 0000 722b 0000 0072  r)...r+...r+...r
-00005fa0: 2c00 0000 7252 0000 000f 0300 0072 5300  ,...rR.......rS.
-00005fb0: 0000 7a1a 5374 6172 745f 3250 5f56 6965  ..z.Start_2P_Vie
-00005fc0: 772e 6f6e 5f73 686f 775f 7669 6577 6301  w.on_show_viewc.
-00005fd0: 0000 0000 0000 0000 0000 0001 0000 0002  ................
-00005fe0: 0000 0043 0000 0072 5400 0000 722e 0000  ...C...rT...r...
-00005ff0: 0072 5500 0000 7229 0000 0072 2b00 0000  .rU...r)...r+...
-00006000: 722b 0000 0072 2c00 0000 7257 0000 0013  r+...r,...rW....
-00006010: 0300 0072 5800 0000 7a1a 5374 6172 745f  ...rX...z.Start_
-00006020: 3250 5f56 6965 772e 6f6e 5f68 6964 655f  2P_View.on_hide_
-00006030: 7669 6577 6301 0000 0000 0000 0000 0000  viewc...........
-00006040: 0001 0000 0004 0000 0043 0000 0073 3600  .........C...s6.
-00006050: 0000 7c00 a000 a100 0100 7401 a002 a100  ..|.......t.....
-00006060: 0100 7401 a003 7c00 6a04 6a05 6a06 7c00  ..t...|.j.j.j.|.
-00006070: 6a04 6a05 6a07 a102 0100 7c00 6a08 a009  j.j.j.....|.j...
-00006080: a100 0100 6400 5300 722e 0000 0029 0a72  ....d.S.r....).r
-00006090: 5b00 0000 7204 0000 0072 ce00 0000 72cf  [...r....r....r.
-000060a0: 0000 0072 2000 0000 7221 0000 0072 d000  ...r ...r!...r..
-000060b0: 0000 72a8 0000 0072 4400 0000 725c 0000  ..r....rD...r\..
-000060c0: 0072 2900 0000 722b 0000 0072 2b00 0000  .r)...r+...r+...
-000060d0: 722c 0000 0072 5d00 0000 1603 0000 7308  r,...r].......s.
-000060e0: 0000 0008 0108 0118 010e 017a 1553 7461  ...........z.Sta
-000060f0: 7274 5f32 505f 5669 6577 2e6f 6e5f 6472  rt_2P_View.on_dr
-00006100: 6177 725f 0000 0072 2b00 0000 722b 0000  awr_...r+...r+..
-00006110: 0072 4d00 0000 722c 0000 0072 3100 0000  .rM...r,...r1...
-00006120: de02 0000 730a 0000 0008 000c 0208 2f08  ....s........./.
-00006130: 0410 0372 3100 0000 6300 0000 0000 0000  ...r1...c.......
-00006140: 0000 0000 0000 0000 0008 0000 0000 0000  ................
-00006150: 00f3 4e00 0000 6500 5a01 6400 5a02 8700  ..N...e.Z.d.Z...
-00006160: 6601 6401 6402 8408 5a03 6403 6404 8400  f.d.d...Z.d.d...
-00006170: 5a04 6405 6406 8400 5a05 6407 6408 8400  Z.d.d...Z.d.d...
-00006180: 5a06 6409 6507 640a 6507 640b 6507 640c  Z.d.e.d.e.d.e.d.
-00006190: 6507 6608 640d 640e 8404 5a08 8700 0400  e.f.d.d...Z.....
-000061a0: 5a09 5300 290f 7225 0100 0063 0200 0000  Z.S.).r%...c....
-000061b0: 0000 0000 0000 0000 0a00 0000 0700 0000  ................
-000061c0: 0300 0000 7304 0100 0074 0083 00a0 01a1  ....s....t......
-000061d0: 0001 007c 0188 005f 0264 0188 005f 0374  ...|..._.d..._.t
-000061e0: 046a 05a0 06a1 0088 005f 0788 006a 07a0  .j......._...j..
-000061f0: 08a1 0001 0074 046a 05a0 0964 0264 0364  .....t.j...d.d.d
-00006200: 0464 0564 06a1 057d 0274 046a 05a0 0964  .d.d...}.t.j...d
-00006210: 0264 0764 0464 0564 08a1 057d 0374 046a  .d.d.d.d...}.t.j
-00006220: 05a0 0964 0964 0264 0a64 0564 0ba1 057d  ...d.d.d.d.d...}
-00006230: 0474 046a 05a0 0964 0964 0c64 0a64 0564  .t.j...d.d.d.d.d
-00006240: 0da1 057d 0588 006a 07a0 0a7c 02a1 0101  ...}...j...|....
-00006250: 0088 006a 07a0 0a7c 03a1 0101 0088 006a  ...j...|.......j
-00006260: 07a0 0a7c 04a1 0101 0088 006a 07a0 0a7c  ...|.......j...|
-00006270: 05a1 0101 007c 02a0 0b64 0ea1 0187 0066  .....|...d.....f
-00006280: 0164 0f64 1084 0883 017d 067c 03a0 0b64  .d.d.....}.|...d
-00006290: 0ea1 0164 1164 1284 0083 017d 077c 04a0  ...d.d.....}.|..
-000062a0: 0b64 0ea1 0187 0066 0164 1364 1484 0883  .d.....f.d.d....
-000062b0: 017d 087c 05a0 0b64 0ea1 0187 0066 0164  .}.|...d.....f.d
-000062c0: 1564 1684 0883 017d 0964 0053 0029 174e  .d.....}.d.S.).N
-000062d0: 72a6 0000 0072 6a00 0000 726b 0000 0072  r....rj...rk...r
-000062e0: 0800 0000 7210 0000 0072 8900 0000 726d  ....r....r....rm
-000062f0: 0000 0072 1400 0000 728b 0000 0072 8c00  ...r....r....r..
-00006300: 0000 7213 0000 0072 d700 0000 72d6 0000  ..r....r....r...
-00006310: 0072 1b00 0000 6301 0000 0000 0000 0000  .r....c.........
-00006320: 0000 0002 0000 0003 0000 0013 0000 0072  ...............r
-00006330: 8f00 0000 722e 0000 0072 9000 0000 7221  ....r....r....r!
-00006340: 0100 0072 2900 0000 722b 0000 0072 2c00  ...r)...r+...r,.
-00006350: 0000 da0d 6f6e 5f63 6c69 636b 5f65 7869  ....on_click_exi
-00006360: 7433 0300 0072 9100 0000 7a2f 5031 5f54  t3...r....z/P1_T
-00006370: 7572 6e5f 3250 5f56 6965 772e 5f5f 696e  urn_2P_View.__in
-00006380: 6974 5f5f 2e3c 6c6f 6361 6c73 3e2e 6f6e  it__.<locals>.on
-00006390: 5f63 6c69 636b 5f65 7869 7463 0100 0000  _click_exitc....
-000063a0: 0000 0000 0000 0000 0100 0000 0200 0000  ................
-000063b0: 5300 0000 723a 0000 0072 2e00 0000 723b  S...r:...r....r;
-000063c0: 0000 0072 2f00 0000 722b 0000 0072 2b00  ...r/...r+...r+.
-000063d0: 0000 722c 0000 0072 3e00 0000 3803 0000  ..r,...r>...8...
-000063e0: 723f 0000 007a 2f50 315f 5475 726e 5f32  r?...z/P1_Turn_2
-000063f0: 505f 5669 6577 2e5f 5f69 6e69 745f 5f2e  P_View.__init__.
-00006400: 3c6c 6f63 616c 733e 2e6f 6e5f 636c 6963  <locals>.on_clic
-00006410: 6b5f 5175 6974 6301 0000 0000 0000 0000  k_Quitc.........
-00006420: 0000 0002 0000 0003 0000 0013 0000 0072  ...............r
-00006430: 3300 0000 722e 0000 0072 3400 0000 7237  3...r....r4...r7
-00006440: 0000 0072 2900 0000 722b 0000 0072 2c00  ...r)...r+...r,.
-00006450: 0000 7238 0000 003c 0300 0072 3900 0000  ..r8...<...r9...
-00006460: 7a33 5031 5f54 7572 6e5f 3250 5f56 6965  z3P1_Turn_2P_Vie
-00006470: 772e 5f5f 696e 6974 5f5f 2e3c 6c6f 6361  w.__init__.<loca
-00006480: 6c73 3e2e 6f6e 5f63 6c69 636b 5f53 6574  ls>.on_click_Set
-00006490: 7469 6e67 7363 0100 0000 0000 0000 0000  tingsc..........
-000064a0: 0000 0200 0000 0300 0000 1300 0000 728f  ..............r.
-000064b0: 0000 0072 2e00 0000 2904 da12 5032 5f50  ...r....)...P2_P
-000064c0: 7265 5475 726e 5f32 505f 5669 6577 7225  reTurn_2P_Viewr%
-000064d0: 0000 0072 2000 0000 7226 0000 00a9 0272  ...r ...r&.....r
-000064e0: 2700 0000 5a0e 6e65 7874 506c 6179 6572  '...Z.nextPlayer
-000064f0: 5669 6577 7229 0000 0072 2b00 0000 722c  Viewr)...r+...r,
-00006500: 0000 00da 0d6f 6e5f 636c 6963 6b5f 646f  .....on_click_do
-00006510: 6e65 4203 0000 7291 0000 007a 2f50 315f  neB...r....z/P1_
-00006520: 5475 726e 5f32 505f 5669 6577 2e5f 5f69  Turn_2P_View.__i
-00006530: 6e69 745f 5f2e 3c6c 6f63 616c 733e 2e6f  nit__.<locals>.o
-00006540: 6e5f 636c 6963 6b5f 646f 6e65 290c 7240  n_click_done).r@
-00006550: 0000 0072 4100 0000 7225 0000 00da 0473  ...rA...r%.....s
-00006560: 7465 7072 3c00 0000 7242 0000 0072 4300  tepr<...rB...rC.
-00006570: 0000 7244 0000 0072 4500 0000 724a 0000  ..rD...rE...rJ..
-00006580: 0072 4800 0000 7227 0000 00a9 0a72 2a00  .rH...r'.....r*.
-00006590: 0000 7225 0000 00da 0b45 7869 745f 6275  ..r%.....Exit_bu
-000065a0: 7474 6f6e 7287 0000 0072 2a01 0000 72f1  ttonr....r*...r.
-000065b0: 0000 0072 2c01 0000 723e 0000 0072 3800  ...r,...r>...r8.
-000065c0: 0000 722f 0100 0072 4d00 0000 7229 0000  ..r/...rM...r)..
-000065d0: 0072 2c00 0000 7241 0000 001f 0300 0073  .r,...rA.......s
-000065e0: 2a00 0000 0a01 0601 0602 0c02 0a01 1402  *...............
-000065f0: 1401 1401 1402 0c02 0c01 0c01 0c01 0802  ................
-00006600: 0e01 0804 0a01 0803 0e01 0805 1201 7a18  ..............z.
-00006610: 5031 5f54 7572 6e5f 3250 5f56 6965 772e  P1_Turn_2P_View.
-00006620: 5f5f 696e 6974 5f5f 6301 0000 0000 0000  __init__c.......
-00006630: 0000 0000 0001 0000 0003 0000 0043 0000  .............C..
-00006640: 0072 4f00 0000 722e 0000 0072 5000 0000  .rO...r....rP...
-00006650: 7229 0000 0072 2b00 0000 722b 0000 0072  r)...r+...r+...r
-00006660: 2c00 0000 7252 0000 0047 0300 0072 5300  ,...rR...G...rS.
-00006670: 0000 7a1c 5031 5f54 7572 6e5f 3250 5f56  ..z.P1_Turn_2P_V
-00006680: 6965 772e 6f6e 5f73 686f 775f 7669 6577  iew.on_show_view
-00006690: 6301 0000 0000 0000 0000 0000 0001 0000  c...............
-000066a0: 0002 0000 0043 0000 0072 5400 0000 722e  .....C...rT...r.
-000066b0: 0000 0072 5500 0000 7229 0000 0072 2b00  ...rU...r)...r+.
-000066c0: 0000 722b 0000 0072 2c00 0000 7257 0000  ..r+...r,...rW..
-000066d0: 004b 0300 0072 5800 0000 7a1c 5031 5f54  .K...rX...z.P1_T
-000066e0: 7572 6e5f 3250 5f56 6965 772e 6f6e 5f68  urn_2P_View.on_h
-000066f0: 6964 655f 7669 6577 6301 0000 0000 0000  ide_viewc.......
-00006700: 0000 0000 0001 0000 0007 0000 0043 0000  .............C..
-00006710: 00f3 a800 0000 7c00 a000 a100 0100 7c00  ......|.......|.
-00006720: 6a01 a002 a100 0100 7403 a004 a100 0100  j.......t.......
-00006730: 7405 a006 6401 6402 6403 6404 7403 6a07  t...d.d.d.d.t.j.
-00006740: a105 0100 7403 a008 7c00 6a09 6a0a 6a0b  ....t...|.j.j.j.
-00006750: 7c00 6a09 6a0a 6a0c a102 0100 7403 a00d  |.j.j.j.....t...
-00006760: 7c00 6a09 6a0e 6a0f 6405 1900 7c00 6a09  |.j.j.j.d...|.j.
-00006770: 6a0e 6a0f 6406 1900 7c00 6a09 6a0e 6a10  j.j.d...|.j.j.j.
-00006780: a103 0100 7c00 6a11 6407 6b02 7246 7403  ....|.j.d.k.rFt.
-00006790: a012 7c00 6a09 6a0e 6a13 a101 0100 6400  ..|.j.j.j.....d.
-000067a0: 5300 7403 a014 7c00 6a09 6a0e 6a15 7c00  S.t...|.j.j.j.|.
-000067b0: 6a09 6a0e 6a16 a102 0100 6400 5300 a908  j.j.j.....d.S...
-000067c0: 4ee9 5902 0000 e991 0100 0072 0801 0000  N.Y........r....
-000067d0: e9fa 0200 0072 0100 0000 7294 0000 0072  .....r....r....r
-000067e0: a600 0000 2917 725b 0000 0072 4400 0000  ....).r[...rD...
-000067f0: 725c 0000 0072 0400 0000 72ce 0000 0072  r\...r....r....r
-00006800: 3c00 0000 721c 0100 00da 1064 6172 6b43  <...r......darkC
-00006810: 6865 636b 6572 436f 6c6f 7272 cf00 0000  heckerColorr....
-00006820: 7220 0000 0072 2100 0000 72d0 0000 0072  r ...r!...r....r
-00006830: a800 0000 72d4 0000 0072 a400 0000 72b9  ....r....r....r.
-00006840: 0000 0072 d500 0000 7230 0100 00da 0c64  ...r....r0.....d
-00006850: 7261 7754 7572 6e4d 6169 6eda 1273 7072  rawTurnMain..spr
-00006860: 6974 6573 5f6d 6f76 655f 7374 6172 74da  ites_move_start.
-00006870: 0e64 7261 7754 7572 6e42 7261 6e63 68da  .drawTurnBranch.
-00006880: 0d73 7072 6974 655f 6163 7469 7665 da10  .sprite_active..
-00006890: 7370 7269 7465 735f 6d6f 7665 5f65 6e64  sprites_move_end
-000068a0: 7229 0000 0072 2b00 0000 722b 0000 0072  r)...r+...r+...r
-000068b0: 2c00 0000 725d 0000 004e 0300 00f3 1a00  ,...r]...N......
-000068c0: 0000 0801 0a01 0801 1401 1801 2801 0802  ............(...
-000068d0: 06ff 0801 08ff 0401 1001 08ff 7a17 5031  ............z.P1
-000068e0: 5f54 7572 6e5f 3250 5f56 6965 772e 6f6e  _Turn_2P_View.on
-000068f0: 5f64 7261 7772 f200 0000 72f3 0000 0072  _drawr....r....r
-00006900: f400 0000 72f5 0000 0063 0500 0000 0000  ....r....c......
-00006910: 0000 0000 0000 0700 0000 0600 0000 4300  ..............C.
-00006920: 0000 f354 0100 007c 006a 0064 016b 0272  ...T...|.j.d.k.r
-00006930: 3074 01a0 027c 017c 0266 027c 006a 036a  0t...|.|.f.|.j.j
-00006940: 046a 05a1 027d 057c 0567 006b 0372 2e7c  .j...}.|.g.k.r.|
-00006950: 0564 0219 007c 006a 036a 045f 0674 07a0  .d...|.j.j._.t..
-00006960: 087c 006a 036a 046a 067c 006a 036a 09a1  .|.j.j.j.|.j.j..
-00006970: 027c 006a 036a 045f 0a64 037c 005f 0064  .|.j.j._.d.|._.d
-00006980: 0053 0064 0053 007c 006a 0064 036b 0272  .S.d.S.|.j.d.k.r
-00006990: a664 017c 005f 0074 01a0 027c 017c 0266  .d.|._.t...|.|.f
-000069a0: 027c 006a 036a 046a 0aa1 027d 057c 0567  .|.j.j.j...}.|.g
-000069b0: 006b 0372 a87c 006a 036a 09a0 0b7c 006a  .k.r.|.j.j...|.j
-000069c0: 036a 046a 066a 0c64 0219 007c 0564 0219  .j.j.j.d...|.d..
-000069d0: 006a 0d66 0264 04a1 0201 007c 006a 036a  .j.f.d.....|.j.j
-000069e0: 096a 0e64 0219 0064 026b 0272 6409 0074  .j.d...d.k.rd..t
-000069f0: 0fa0 107c 006a 036a 046a 066a 0c64 0219  ...|.j.j.j.j.d..
-00006a00: 007c 0564 0219 006a 0d7c 006a 036a 046a  .|.d...j.|.j.j.j
-00006a10: 1164 04a1 047d 067c 006a 036a 046a 11a0  .d...}.|.j.j.j..
-00006a20: 127c 06a1 0101 0074 137c 006a 036a 046a  .|.....t.|.j.j.j
-00006a30: 1183 0164 026b 0472 9d7c 006a 036a 04a0  ...d.k.r.|.j.j..
-00006a40: 147c 006a 036a 09a1 0101 007c 006a 036a  .|.j.j.....|.j.j
-00006a50: 04a0 157c 006a 036a 09a1 0101 0064 0053  ...|.j.j.....d.S
-00006a60: 0074 01a0 16a1 007c 006a 036a 045f 0564  .t.....|.j.j._.d
-00006a70: 0053 0064 0053 0064 0053 0029 054e 72a6  .S.d.S.d.S.).Nr.
-00006a80: 0000 0072 0100 0000 da06 4272 616e 6368  ...r......Branch
-00006a90: 7294 0000 00a9 1772 3001 0000 723c 0000  r......r0...r<..
-00006aa0: 00da 1467 6574 5f73 7072 6974 6573 5f61  ...get_sprites_a
-00006ab0: 745f 706f 696e 7472 2000 0000 72a4 0000  t_pointr ...r...
-00006ac0: 0072 3a01 0000 723c 0100 0072 0400 0000  .r:...r<...r....
-00006ad0: da14 6372 6561 7465 4d6f 7665 456e 6453  ..createMoveEndS
-00006ae0: 7072 6974 6573 7221 0000 0072 3d01 0000  pritesr!...r=...
-00006af0: da08 6d61 6b65 4d6f 7665 da04 6d6f 7665  ..makeMove..move
-00006b00: da03 706f 7372 a800 0000 7203 0000 00da  ..posr....r.....
-00006b10: 0d66 726f 6d4d 6f76 6554 6f44 6965 72d5  .fromMoveToDier.
-00006b20: 0000 00da 0672 656d 6f76 65da 036c 656e  .....remove..len
-00006b30: 7223 0100 0072 2401 0000 da0a 5370 7269  r#...r$.....Spri
-00006b40: 7465 4c69 7374 a907 722a 0000 0072 f200  teList..r*...r..
-00006b50: 0000 72f3 0000 0072 f400 0000 72f5 0000  ..r....r....r...
-00006b60: 005a 0e63 6c69 636b 6564 5f73 7072 6974  .Z.clicked_sprit
-00006b70: 6572 b900 0000 722b 0000 0072 2b00 0000  er....r+...r+...
-00006b80: 722c 0000 0072 1101 0000 5903 0000 f334  r,...r....Y....4
-00006b90: 0000 000a 0116 0108 010e 0104 010e 010a  ................
-00006ba0: ff0a 0204 fc0a 0606 0116 0208 0126 0112  .............&..
-00006bb0: 0102 011a 020a 0104 ff10 0212 0112 0116  ................
-00006bc0: 0112 0204 f004 047a 1e50 315f 5475 726e  .......z.P1_Turn
-00006bd0: 5f32 505f 5669 6577 2e6f 6e5f 6d6f 7573  _2P_View.on_mous
-00006be0: 655f 7072 6573 73a9 0a72 6000 0000 7261  e_press..r`...ra
-00006bf0: 0000 0072 6200 0000 7241 0000 0072 5200  ...rb...rA...rR.
-00006c00: 0000 7257 0000 0072 5d00 0000 72b3 0000  ..rW...r]...r...
-00006c10: 0072 1101 0000 7263 0000 0072 2b00 0000  .r....rc...r+...
-00006c20: 722b 0000 0072 4d00 0000 722c 0000 0072  r+...rM...r,...r
-00006c30: 2501 0000 1d03 0000 f30c 0000 0008 000c  %...............
-00006c40: 0208 2808 0408 0322 0b72 2501 0000 6300  ..(....".r%...c.
-00006c50: 0000 0000 0000 0000 0000 0000 0000 0008  ................
-00006c60: 0000 0000 0000 0072 2b01 0000 290f 7226  .......r+...).r&
-00006c70: 0100 0063 0200 0000 0000 0000 0000 0000  ...c............
-00006c80: 0a00 0000 0700 0000 0300 0000 7304 0100  ............s...
-00006c90: 0074 0083 00a0 01a1 0001 007c 0188 005f  .t.........|..._
-00006ca0: 0274 036a 04a0 05a1 0088 005f 0688 006a  .t.j......._...j
-00006cb0: 06a0 07a1 0001 0064 0188 005f 0874 036a  .......d..._.t.j
-00006cc0: 04a0 0964 0264 0364 0464 0564 06a1 057d  ...d.d.d.d.d...}
-00006cd0: 0274 036a 04a0 0964 0264 0764 0464 0564  .t.j...d.d.d.d.d
-00006ce0: 08a1 057d 0374 036a 04a0 0964 0964 0264  ...}.t.j...d.d.d
-00006cf0: 0a64 0564 0ba1 057d 0474 036a 04a0 0964  .d.d...}.t.j...d
-00006d00: 0964 0c64 0a64 0564 0da1 057d 0588 006a  .d.d.d.d...}...j
-00006d10: 06a0 0a7c 02a1 0101 0088 006a 06a0 0a7c  ...|.......j...|
-00006d20: 03a1 0101 0088 006a 06a0 0a7c 04a1 0101  .......j...|....
-00006d30: 0088 006a 06a0 0a7c 05a1 0101 007c 02a0  ...j...|.....|..
-00006d40: 0b64 0ea1 0187 0066 0164 0f64 1084 0883  .d.....f.d.d....
-00006d50: 017d 067c 03a0 0b64 0ea1 0164 1164 1284  .}.|...d...d.d..
-00006d60: 0083 017d 077c 04a0 0b64 0ea1 0187 0066  ...}.|...d.....f
-00006d70: 0164 1364 1484 0883 017d 087c 05a0 0b64  .d.d.....}.|...d
-00006d80: 0ea1 0187 0066 0164 1564 1684 0883 017d  .....f.d.d.....}
-00006d90: 0964 0053 0029 174e 72a6 0000 0072 6a00  .d.S.).Nr....rj.
-00006da0: 0000 726b 0000 0072 0800 0000 7210 0000  ..rk...r....r...
-00006db0: 0072 8900 0000 726d 0000 0072 1400 0000  .r....rm...r....
-00006dc0: 728b 0000 0072 8c00 0000 7213 0000 0072  r....r....r....r
-00006dd0: d700 0000 72d6 0000 0072 1b00 0000 6301  ....r....r....c.
-00006de0: 0000 0000 0000 0000 0000 0002 0000 0003  ................
-00006df0: 0000 0013 0000 0072 8f00 0000 722e 0000  .......r....r...
-00006e00: 0072 9000 0000 7221 0100 0072 2900 0000  .r....r!...r)...
-00006e10: 722b 0000 0072 2c00 0000 722c 0100 008b  r+...r,...r,....
-00006e20: 0300 0072 9100 0000 7a2f 5032 5f54 7572  ...r....z/P2_Tur
-00006e30: 6e5f 3250 5f56 6965 772e 5f5f 696e 6974  n_2P_View.__init
-00006e40: 5f5f 2e3c 6c6f 6361 6c73 3e2e 6f6e 5f63  __.<locals>.on_c
-00006e50: 6c69 636b 5f65 7869 7463 0100 0000 0000  lick_exitc......
-00006e60: 0000 0000 0000 0100 0000 0200 0000 5300  ..............S.
-00006e70: 0000 723a 0000 0072 2e00 0000 723b 0000  ..r:...r....r;..
-00006e80: 0072 2f00 0000 722b 0000 0072 2b00 0000  .r/...r+...r+...
-00006e90: 722c 0000 0072 3e00 0000 9003 0000 723f  r,...r>.......r?
-00006ea0: 0000 007a 2f50 325f 5475 726e 5f32 505f  ...z/P2_Turn_2P_
-00006eb0: 5669 6577 2e5f 5f69 6e69 745f 5f2e 3c6c  View.__init__.<l
-00006ec0: 6f63 616c 733e 2e6f 6e5f 636c 6963 6b5f  ocals>.on_click_
-00006ed0: 5175 6974 6301 0000 0000 0000 0000 0000  Quitc...........
-00006ee0: 0002 0000 0003 0000 0013 0000 0072 3300  .............r3.
-00006ef0: 0000 722e 0000 0072 3400 0000 7237 0000  ..r....r4...r7..
-00006f00: 0072 2900 0000 722b 0000 0072 2c00 0000  .r)...r+...r,...
-00006f10: 7238 0000 0094 0300 0072 3900 0000 7a33  r8.......r9...z3
-00006f20: 5032 5f54 7572 6e5f 3250 5f56 6965 772e  P2_Turn_2P_View.
-00006f30: 5f5f 696e 6974 5f5f 2e3c 6c6f 6361 6c73  __init__.<locals
-00006f40: 3e2e 6f6e 5f63 6c69 636b 5f53 6574 7469  >.on_click_Setti
-00006f50: 6e67 7363 0100 0000 0000 0000 0000 0000  ngsc............
-00006f60: 0200 0000 0300 0000 1300 0000 728f 0000  ............r...
-00006f70: 0072 2e00 0000 2904 da12 5031 5f50 7265  .r....)...P1_Pre
-00006f80: 5475 726e 5f32 505f 5669 6577 7225 0000  Turn_2P_Viewr%..
-00006f90: 0072 2000 0000 7226 0000 0072 2e01 0000  .r ...r&...r....
-00006fa0: 7229 0000 0072 2b00 0000 722c 0000 0072  r)...r+...r,...r
-00006fb0: 2f01 0000 9a03 0000 7291 0000 007a 2f50  /.......r....z/P
-00006fc0: 325f 5475 726e 5f32 505f 5669 6577 2e5f  2_Turn_2P_View._
-00006fd0: 5f69 6e69 745f 5f2e 3c6c 6f63 616c 733e  _init__.<locals>
-00006fe0: 2e6f 6e5f 636c 6963 6b5f 646f 6e65 290c  .on_click_done).
-00006ff0: 7240 0000 0072 4100 0000 7225 0000 0072  r@...rA...r%...r
-00007000: 3c00 0000 7242 0000 0072 4300 0000 7244  <...rB...rC...rD
-00007010: 0000 0072 4500 0000 7230 0100 0072 4a00  ...rE...r0...rJ.
-00007020: 0000 7248 0000 0072 2700 0000 7231 0100  ..rH...r'...r1..
-00007030: 0072 4d00 0000 7229 0000 0072 2c00 0000  .rM...r)...r,...
-00007040: 7241 0000 0077 0300 0073 2a00 0000 0a01  rA...w...s*.....
-00007050: 0601 0c02 0a01 0602 1402 1401 1401 1402  ................
-00007060: 0c02 0c01 0c01 0c01 0802 0e01 0804 0a01  ................
-00007070: 0803 0e01 0805 1201 7a18 5032 5f54 7572  ........z.P2_Tur
-00007080: 6e5f 3250 5f56 6965 772e 5f5f 696e 6974  n_2P_View.__init
-00007090: 5f5f 6301 0000 0000 0000 0000 0000 0001  __c.............
-000070a0: 0000 0003 0000 0043 0000 0072 4f00 0000  .......C...rO...
-000070b0: 722e 0000 0072 5000 0000 7229 0000 0072  r....rP...r)...r
-000070c0: 2b00 0000 722b 0000 0072 2c00 0000 7252  +...r+...r,...rR
-000070d0: 0000 009f 0300 0072 5300 0000 7a1c 5032  .......rS...z.P2
-000070e0: 5f54 7572 6e5f 3250 5f56 6965 772e 6f6e  _Turn_2P_View.on
-000070f0: 5f73 686f 775f 7669 6577 6301 0000 0000  _show_viewc.....
-00007100: 0000 0000 0000 0001 0000 0002 0000 0043  ...............C
-00007110: 0000 0072 5400 0000 722e 0000 0072 5500  ...rT...r....rU.
-00007120: 0000 7229 0000 0072 2b00 0000 722b 0000  ..r)...r+...r+..
-00007130: 0072 2c00 0000 7257 0000 00a3 0300 0072  .r,...rW.......r
-00007140: 5800 0000 7a1c 5032 5f54 7572 6e5f 3250  X...z.P2_Turn_2P
-00007150: 5f56 6965 772e 6f6e 5f68 6964 655f 7669  _View.on_hide_vi
-00007160: 6577 6301 0000 0000 0000 0000 0000 0001  ewc.............
-00007170: 0000 0007 0000 0043 0000 0072 3301 0000  .......C...r3...
-00007180: 7234 0100 0029 1772 5b00 0000 7244 0000  r4...).r[...rD..
-00007190: 0072 5c00 0000 7204 0000 0072 ce00 0000  .r\...r....r....
-000071a0: 723c 0000 0072 1c01 0000 da11 6c69 6768  r<...r......ligh
-000071b0: 7443 6865 636b 6572 436f 6c6f 7272 cf00  tCheckerColorr..
-000071c0: 0000 7220 0000 0072 2100 0000 72d0 0000  ..r ...r!...r...
-000071d0: 0072 a800 0000 72d4 0000 0072 a400 0000  .r....r....r....
-000071e0: 72b9 0000 0072 d500 0000 7230 0100 0072  r....r....r0...r
-000071f0: 3901 0000 723a 0100 0072 3b01 0000 723c  9...r:...r;...r<
-00007200: 0100 0072 3d01 0000 7229 0000 0072 2b00  ...r=...r)...r+.
-00007210: 0000 722b 0000 0072 2c00 0000 725d 0000  ..r+...r,...r]..
-00007220: 00a6 0300 0072 3e01 0000 7a17 5032 5f54  .....r>...z.P2_T
-00007230: 7572 6e5f 3250 5f56 6965 772e 6f6e 5f64  urn_2P_View.on_d
-00007240: 7261 7772 f200 0000 72f3 0000 0072 f400  rawr....r....r..
-00007250: 0000 72f5 0000 0063 0500 0000 0000 0000  ..r....c........
-00007260: 0000 0000 0700 0000 0600 0000 4300 0000  ............C...
-00007270: 723f 0100 0029 054e 72a6 0000 0072 0100  r?...).Nr....r..
-00007280: 0000 7240 0100 0072 9500 0000 7241 0100  ..r@...r....rA..
-00007290: 0072 4b01 0000 722b 0000 0072 2b00 0000  .rK...r+...r+...
-000072a0: 722c 0000 0072 1101 0000 b103 0000 724c  r,...r........rL
-000072b0: 0100 007a 1e50 325f 5475 726e 5f32 505f  ...z.P2_Turn_2P_
-000072c0: 5669 6577 2e6f 6e5f 6d6f 7573 655f 7072  View.on_mouse_pr
-000072d0: 6573 7372 4d01 0000 722b 0000 0072 2b00  essrM...r+...r+.
-000072e0: 0000 724d 0000 0072 2c00 0000 7226 0100  ..rM...r,...r&..
-000072f0: 0075 0300 0072 4e01 0000 7226 0100 0063  .u...rN...r&...c
-00007300: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00007310: 0300 0000 0000 0000 7205 0000 0029 0972  ........r....).r
-00007320: 4f01 0000 6302 0000 0000 0000 0000 0000  O...c...........
-00007330: 000a 0000 0007 0000 0003 0000 00f3 fe00  ................
-00007340: 0000 7400 8300 a001 a100 0100 7c01 8800  ..t.........|...
-00007350: 5f02 7403 6a04 a005 a100 8800 5f06 8800  _.t.j......._...
-00007360: 6a06 a007 a100 0100 7403 6a04 a008 6401  j.......t.j...d.
-00007370: 6402 6403 6404 6405 a105 7d02 7403 6a04  d.d.d.d...}.t.j.
-00007380: a008 6401 6406 6403 6404 6407 a105 7d03  ..d.d.d.d.d...}.
-00007390: 7403 6a04 a008 6408 6401 6409 6404 640a  t.j...d.d.d.d.d.
-000073a0: a105 7d04 7403 6a04 a008 6408 640b 6409  ..}.t.j...d.d.d.
-000073b0: 6404 640c a105 7d05 8800 6a06 a009 7c02  d.d...}...j...|.
-000073c0: a101 0100 8800 6a06 a009 7c03 a101 0100  ......j...|.....
-000073d0: 8800 6a06 a009 7c04 a101 0100 8800 6a06  ..j...|.......j.
-000073e0: a009 7c05 a101 0100 7c02 a00a 640d a101  ..|.....|...d...
-000073f0: 8700 6601 640e 640f 8408 8301 7d06 7c03  ..f.d.d.....}.|.
-00007400: a00a 640d a101 6410 6411 8400 8301 7d07  ..d...d.d.....}.
-00007410: 7c04 a00a 640d a101 8700 6601 6412 6413  |...d.....f.d.d.
-00007420: 8408 8301 7d08 7c05 a00a 640d a101 8700  ....}.|...d.....
-00007430: 6601 6414 6415 8408 8301 7d09 6400 5300  f.d.d.....}.d.S.
-00007440: 2916 4e72 6a00 0000 726b 0000 0072 0800  ).Nrj...rk...r..
-00007450: 0000 7210 0000 0072 8900 0000 726d 0000  ..r....r....rm..
-00007460: 0072 1400 0000 728b 0000 0072 8c00 0000  .r....r....r....
-00007470: 7213 0000 0072 1b01 0000 7220 0100 0072  r....r....r ...r
-00007480: 1b00 0000 6301 0000 0000 0000 0000 0000  ....c...........
-00007490: 0002 0000 0003 0000 0013 0000 0072 8f00  .............r..
-000074a0: 0000 722e 0000 0072 9000 0000 7221 0100  ..r....r....r!..
-000074b0: 0072 2900 0000 722b 0000 0072 2c00 0000  .r)...r+...r,...
-000074c0: 722c 0100 00e1 0300 0072 9100 0000 7a32  r,.......r....z2
-000074d0: 5031 5f50 7265 5475 726e 5f32 505f 5669  P1_PreTurn_2P_Vi
-000074e0: 6577 2e5f 5f69 6e69 745f 5f2e 3c6c 6f63  ew.__init__.<loc
-000074f0: 616c 733e 2e6f 6e5f 636c 6963 6b5f 6578  als>.on_click_ex
-00007500: 6974 6301 0000 0000 0000 0000 0000 0001  itc.............
-00007510: 0000 0002 0000 0053 0000 0072 3a00 0000  .......S...r:...
-00007520: 722e 0000 0072 3b00 0000 722f 0000 0072  r....r;...r/...r
-00007530: 2b00 0000 722b 0000 0072 2c00 0000 723e  +...r+...r,...r>
-00007540: 0000 00e6 0300 0072 3f00 0000 7a32 5031  .......r?...z2P1
-00007550: 5f50 7265 5475 726e 5f32 505f 5669 6577  _PreTurn_2P_View
-00007560: 2e5f 5f69 6e69 745f 5f2e 3c6c 6f63 616c  .__init__.<local
-00007570: 733e 2e6f 6e5f 636c 6963 6b5f 5175 6974  s>.on_click_Quit
-00007580: 6301 0000 0000 0000 0000 0000 0002 0000  c...............
-00007590: 0003 0000 0013 0000 0072 3300 0000 722e  .........r3...r.
-000075a0: 0000 0072 3400 0000 7237 0000 0072 2900  ...r4...r7...r).
-000075b0: 0000 722b 0000 0072 2c00 0000 7238 0000  ..r+...r,...r8..
-000075c0: 00ea 0300 0072 3900 0000 7a36 5031 5f50  .....r9...z6P1_P
-000075d0: 7265 5475 726e 5f32 505f 5669 6577 2e5f  reTurn_2P_View._
-000075e0: 5f69 6e69 745f 5f2e 3c6c 6f63 616c 733e  _init__.<locals>
-000075f0: 2e6f 6e5f 636c 6963 6b5f 5365 7474 696e  .on_click_Settin
-00007600: 6773 6301 0000 0000 0000 0000 0000 0002  gsc.............
-00007610: 0000 0005 0000 0013 0000 00f3 5200 0000  ............R...
-00007620: 7400 6a01 6401 6402 6403 6404 8d03 8800  t.j.d.d.d.d.....
-00007630: 6a02 5f03 8800 6a02 6a03 a004 8800 6a02  j._...j.j.....j.
-00007640: 6a05 a101 0100 8800 6a02 6a03 a006 8800  j.......j.j.....
-00007650: 6a02 6a05 a101 0100 7407 8800 6a08 8301  j.j.....t...j...
-00007660: 7d01 8800 6a02 a009 7c01 a101 0100 6400  }...j...|.....d.
-00007670: 5300 2905 4e72 9400 0000 721d 0000 0046  S.).Nr....r....F
-00007680: 7296 0000 0029 0a72 0300 0000 72a3 0000  r....).r....r...
-00007690: 0072 2000 0000 72a4 0000 0072 2301 0000  .r ...r....r#...
-000076a0: 7221 0000 0072 2401 0000 7225 0100 0072  r!...r$...r%...r
-000076b0: 2500 0000 7226 0000 0072 2e01 0000 7229  %...r&...r....r)
-000076c0: 0000 0072 2b00 0000 722c 0000 0072 2701  ...r+...r,...r'.
-000076d0: 0000 f003 0000 f30a 0000 0014 0212 0112  ................
-000076e0: 010a 0210 017a 3250 315f 5072 6554 7572  .....z2P1_PreTur
-000076f0: 6e5f 3250 5f56 6965 772e 5f5f 696e 6974  n_2P_View.__init
-00007700: 5f5f 2e3c 6c6f 6361 6c73 3e2e 6f6e 5f63  __.<locals>.on_c
-00007710: 6c69 636b 5f72 6f6c 6c72 2801 0000 a90a  lick_rollr(.....
-00007720: 722a 0000 0072 2500 0000 7232 0100 0072  r*...r%...r2...r
-00007730: 8700 0000 722a 0100 0072 2901 0000 722c  ....r*...r)...r,
-00007740: 0100 0072 3e00 0000 7238 0000 0072 2701  ...r>...r8...r'.
-00007750: 0000 724d 0000 0072 2900 0000 722c 0000  ..rM...r)...r,..
-00007760: 0072 4100 0000 cf03 0000 f328 0000 000a  .rA........(....
-00007770: 0106 010c 020a 0114 0214 0114 0114 020c  ................
-00007780: 020c 010c 010c 0108 020e 0108 040a 0108  ................
-00007790: 030e 0108 0512 017a 1b50 315f 5072 6554  .......z.P1_PreT
-000077a0: 7572 6e5f 3250 5f56 6965 772e 5f5f 696e  urn_2P_View.__in
-000077b0: 6974 5f5f 6301 0000 0000 0000 0000 0000  it__c...........
-000077c0: 0001 0000 0003 0000 0043 0000 0072 4f00  .........C...rO.
-000077d0: 0000 722e 0000 0072 5000 0000 7229 0000  ..r....rP...r)..
-000077e0: 0072 2b00 0000 722b 0000 0072 2c00 0000  .r+...r+...r,...
-000077f0: 7252 0000 00f9 0300 0072 5300 0000 7a1f  rR.......rS...z.
-00007800: 5031 5f50 7265 5475 726e 5f32 505f 5669  P1_PreTurn_2P_Vi
-00007810: 6577 2e6f 6e5f 7368 6f77 5f76 6965 7763  ew.on_show_viewc
-00007820: 0100 0000 0000 0000 0000 0000 0100 0000  ................
-00007830: 0200 0000 4300 0000 7254 0000 0072 2e00  ....C...rT...r..
-00007840: 0000 7255 0000 0072 2900 0000 722b 0000  ..rU...r)...r+..
-00007850: 0072 2b00 0000 722c 0000 0072 5700 0000  .r+...r,...rW...
-00007860: fd03 0000 7258 0000 007a 1f50 315f 5072  ....rX...z.P1_Pr
-00007870: 6554 7572 6e5f 3250 5f56 6965 772e 6f6e  eTurn_2P_View.on
-00007880: 5f68 6964 655f 7669 6577 6301 0000 0000  _hide_viewc.....
-00007890: 0000 0000 0000 0001 0000 0007 0000 0043  ...............C
-000078a0: 0000 00f3 4a00 0000 7c00 a000 a100 0100  ....J...|.......
-000078b0: 7c00 6a01 a002 a100 0100 7403 a004 a100  |.j.......t.....
-000078c0: 0100 7405 a006 6401 6402 6403 6404 7403  ..t...d.d.d.d.t.
-000078d0: 6a07 a105 0100 7403 a008 7c00 6a09 6a0a  j.....t...|.j.j.
-000078e0: 6a0b 7c00 6a09 6a0a 6a0c a102 0100 6400  j.|.j.j.j.....d.
-000078f0: 5300 a905 4e72 3501 0000 7236 0100 0072  S...Nr5...r6...r
-00007900: 0801 0000 7237 0100 0029 0d72 5b00 0000  ....r7...).r[...
-00007910: 7244 0000 0072 5c00 0000 7204 0000 0072  rD...r\...r....r
-00007920: ce00 0000 723c 0000 0072 1c01 0000 7238  ....r<...r....r8
-00007930: 0100 0072 cf00 0000 7220 0000 0072 2100  ...r....r ...r!.
-00007940: 0000 72d0 0000 0072 a800 0000 7229 0000  ..r....r....r)..
-00007950: 0072 2b00 0000 722b 0000 0072 2c00 0000  .r+...r+...r,...
-00007960: 725d 0000 0000 0400 00f3 0a00 0000 0801  r]..............
-00007970: 0a01 0801 1401 1c01 7a1a 5031 5f50 7265  ........z.P1_Pre
-00007980: 5475 726e 5f32 505f 5669 6577 2e6f 6e5f  Turn_2P_View.on_
-00007990: 6472 6177 725f 0000 0072 2b00 0000 722b  drawr_...r+...r+
-000079a0: 0000 0072 4d00 0000 722c 0000 0072 4f01  ...rM...r,...rO.
-000079b0: 0000 cd03 0000 f30a 0000 0008 000c 0208  ................
-000079c0: 2a08 0410 0372 4f01 0000 6300 0000 0000  *....rO...c.....
-000079d0: 0000 0000 0000 0000 0000 0003 0000 0000  ................
-000079e0: 0000 0072 0500 0000 2909 722d 0100 0063  ...r....).r-...c
-000079f0: 0200 0000 0000 0000 0000 0000 0a00 0000  ................
-00007a00: 0700 0000 0300 0000 7251 0100 0029 164e  ........rQ...).N
-00007a10: 726a 0000 0072 6b00 0000 7208 0000 0072  rj...rk...r....r
-00007a20: 1000 0000 7289 0000 0072 6d00 0000 7214  ....r....rm...r.
-00007a30: 0000 0072 8b00 0000 728c 0000 0072 1300  ...r....r....r..
-00007a40: 0000 721b 0100 0072 2001 0000 721b 0000  ..r....r ...r...
-00007a50: 0063 0100 0000 0000 0000 0000 0000 0200  .c..............
-00007a60: 0000 0300 0000 1300 0000 728f 0000 0072  ..........r....r
-00007a70: 2e00 0000 7290 0000 0072 2101 0000 7229  ....r....r!...r)
-00007a80: 0000 0072 2b00 0000 722c 0000 0072 2c01  ...r+...r,...r,.
-00007a90: 0000 1c04 0000 7291 0000 007a 3250 325f  ......r....z2P2_
-00007aa0: 5072 6554 7572 6e5f 3250 5f56 6965 772e  PreTurn_2P_View.
-00007ab0: 5f5f 696e 6974 5f5f 2e3c 6c6f 6361 6c73  __init__.<locals
-00007ac0: 3e2e 6f6e 5f63 6c69 636b 5f65 7869 7463  >.on_click_exitc
-00007ad0: 0100 0000 0000 0000 0000 0000 0100 0000  ................
-00007ae0: 0200 0000 5300 0000 723a 0000 0072 2e00  ....S...r:...r..
-00007af0: 0000 723b 0000 0072 2f00 0000 722b 0000  ..r;...r/...r+..
-00007b00: 0072 2b00 0000 722c 0000 0072 3e00 0000  .r+...r,...r>...
-00007b10: 2104 0000 723f 0000 007a 3250 325f 5072  !...r?...z2P2_Pr
-00007b20: 6554 7572 6e5f 3250 5f56 6965 772e 5f5f  eTurn_2P_View.__
-00007b30: 696e 6974 5f5f 2e3c 6c6f 6361 6c73 3e2e  init__.<locals>.
-00007b40: 6f6e 5f63 6c69 636b 5f51 7569 7463 0100  on_click_Quitc..
-00007b50: 0000 0000 0000 0000 0000 0200 0000 0300  ................
-00007b60: 0000 1300 0000 7233 0000 0072 2e00 0000  ......r3...r....
-00007b70: 7234 0000 0072 3700 0000 7229 0000 0072  r4...r7...r)...r
-00007b80: 2b00 0000 722c 0000 0072 3800 0000 2504  +...r,...r8...%.
-00007b90: 0000 7239 0000 007a 3650 325f 5072 6554  ..r9...z6P2_PreT
-00007ba0: 7572 6e5f 3250 5f56 6965 772e 5f5f 696e  urn_2P_View.__in
-00007bb0: 6974 5f5f 2e3c 6c6f 6361 6c73 3e2e 6f6e  it__.<locals>.on
-00007bc0: 5f63 6c69 636b 5f53 6574 7469 6e67 7363  _click_Settingsc
-00007bd0: 0100 0000 0000 0000 0000 0000 0200 0000  ................
-00007be0: 0500 0000 1300 0000 7252 0100 0029 054e  ........rR...).N
-00007bf0: 7295 0000 0072 1d00 0000 4672 9600 0000  r....r....Fr....
-00007c00: 290a 7203 0000 0072 a300 0000 7220 0000  ).r....r....r ..
-00007c10: 0072 a400 0000 7223 0100 0072 2100 0000  .r....r#...r!...
-00007c20: 7224 0100 0072 2601 0000 7225 0000 0072  r$...r&...r%...r
-00007c30: 2600 0000 722e 0100 0072 2900 0000 722b  &...r....r)...r+
-00007c40: 0000 0072 2c00 0000 7227 0100 002b 0400  ...r,...r'...+..
-00007c50: 0072 5301 0000 7a32 5032 5f50 7265 5475  .rS...z2P2_PreTu
-00007c60: 726e 5f32 505f 5669 6577 2e5f 5f69 6e69  rn_2P_View.__ini
-00007c70: 745f 5f2e 3c6c 6f63 616c 733e 2e6f 6e5f  t__.<locals>.on_
-00007c80: 636c 6963 6b5f 726f 6c6c 7228 0100 0072  click_rollr(...r
-00007c90: 5401 0000 724d 0000 0072 2900 0000 722c  T...rM...r)...r,
-00007ca0: 0000 0072 4100 0000 0a04 0000 7255 0100  ...rA.......rU..
-00007cb0: 007a 1b50 325f 5072 6554 7572 6e5f 3250  .z.P2_PreTurn_2P
-00007cc0: 5f56 6965 772e 5f5f 696e 6974 5f5f 6301  _View.__init__c.
-00007cd0: 0000 0000 0000 0000 0000 0001 0000 0003  ................
-00007ce0: 0000 0043 0000 0072 4f00 0000 722e 0000  ...C...rO...r...
-00007cf0: 0072 5000 0000 7229 0000 0072 2b00 0000  .rP...r)...r+...
-00007d00: 722b 0000 0072 2c00 0000 7252 0000 0034  r+...r,...rR...4
-00007d10: 0400 0072 5300 0000 7a1f 5032 5f50 7265  ...rS...z.P2_Pre
-00007d20: 5475 726e 5f32 505f 5669 6577 2e6f 6e5f  Turn_2P_View.on_
-00007d30: 7368 6f77 5f76 6965 7763 0100 0000 0000  show_viewc......
-00007d40: 0000 0000 0000 0100 0000 0200 0000 4300  ..............C.
-00007d50: 0000 7254 0000 0072 2e00 0000 7255 0000  ..rT...r....rU..
-00007d60: 0072 2900 0000 722b 0000 0072 2b00 0000  .r)...r+...r+...
-00007d70: 722c 0000 0072 5700 0000 3804 0000 7258  r,...rW...8...rX
-00007d80: 0000 007a 1f50 325f 5072 6554 7572 6e5f  ...z.P2_PreTurn_
-00007d90: 3250 5f56 6965 772e 6f6e 5f68 6964 655f  2P_View.on_hide_
-00007da0: 7669 6577 6301 0000 0000 0000 0000 0000  viewc...........
-00007db0: 0001 0000 0007 0000 0043 0000 0072 5601  .........C...rV.
-00007dc0: 0000 7257 0100 0029 0d72 5b00 0000 7244  ..rW...).r[...rD
-00007dd0: 0000 0072 5c00 0000 7204 0000 0072 ce00  ...r\...r....r..
-00007de0: 0000 723c 0000 0072 1c01 0000 7250 0100  ..r<...r....rP..
-00007df0: 0072 cf00 0000 7220 0000 0072 2100 0000  .r....r ...r!...
-00007e00: 72d0 0000 0072 a800 0000 7229 0000 0072  r....r....r)...r
-00007e10: 2b00 0000 722b 0000 0072 2c00 0000 725d  +...r+...r,...r]
-00007e20: 0000 003b 0400 0072 5801 0000 7a1a 5032  ...;...rX...z.P2
-00007e30: 5f50 7265 5475 726e 5f32 505f 5669 6577  _PreTurn_2P_View
-00007e40: 2e6f 6e5f 6472 6177 725f 0000 0072 2b00  .on_drawr_...r+.
-00007e50: 0000 722b 0000 0072 4d00 0000 722c 0000  ..r+...rM...r,..
-00007e60: 0072 2d01 0000 0804 0000 7259 0100 0072  .r-.......rY...r
-00007e70: 2d01 0000 6300 0000 0000 0000 0000 0000  -...c...........
-00007e80: 0000 0000 0003 0000 0000 0000 0072 0500  .............r..
-00007e90: 0000 2909 da10 4761 6d65 4f76 6572 5f32  ..)...GameOver_2
-00007ea0: 505f 5669 6577 6302 0000 0000 0000 0000  P_Viewc.........
-00007eb0: 0000 0003 0000 0007 0000 0003 0000 0073  ...............s
-00007ec0: 4a00 0000 7400 8300 a001 a100 0100 7c01  J...t.........|.
-00007ed0: 7c00 5f02 7403 6a04 a005 a100 7c00 5f06  |._.t.j.....|._.
-00007ee0: 7c00 6a06 a007 a100 0100 7403 6a04 a008  |.j.......t.j...
-00007ef0: 6401 6402 6403 6404 6405 a105 7d02 7c00  d.d.d.d.d...}.|.
-00007f00: 6a06 a009 7c02 a101 0100 6400 5300 2906  j...|.....d.S.).
-00007f10: 4e72 0e01 0000 7272 0000 0072 6400 0000  Nr....rr...rd...
-00007f20: 726f 0000 0072 6c00 0000 290a 7240 0000  ro...rl...).r@..
-00007f30: 0072 4100 0000 7225 0000 0072 3c00 0000  .rA...r%...r<...
-00007f40: 7242 0000 0072 4300 0000 7244 0000 0072  rB...rC...rD...r
-00007f50: 4500 0000 724a 0000 0072 4800 0000 2903  E...rJ...rH...).
-00007f60: 722a 0000 0072 4c00 0000 5a0b 6261 636b  r*...rL...Z.back
-00007f70: 5f62 7574 746f 6e72 4d00 0000 722b 0000  _buttonrM...r+..
-00007f80: 0072 2c00 0000 7241 0000 0045 0400 0073  .r,...rA...E...s
-00007f90: 0c00 0000 0a01 0601 0c02 0a01 1402 1002  ................
-00007fa0: 7a19 4761 6d65 4f76 6572 5f32 505f 5669  z.GameOver_2P_Vi
-00007fb0: 6577 2e5f 5f69 6e69 745f 5f63 0100 0000  ew.__init__c....
-00007fc0: 0000 0000 0000 0000 0100 0000 0300 0000  ................
-00007fd0: 4300 0000 724f 0000 0072 2e00 0000 7250  C...rO...r....rP
-00007fe0: 0000 0072 2900 0000 722b 0000 0072 2b00  ...r)...r+...r+.
-00007ff0: 0000 722c 0000 0072 5200 0000 5004 0000  ..r,...rR...P...
-00008000: 7253 0000 007a 1d47 616d 654f 7665 725f  rS...z.GameOver_
-00008010: 3250 5f56 6965 772e 6f6e 5f73 686f 775f  2P_View.on_show_
-00008020: 7669 6577 6301 0000 0000 0000 0000 0000  viewc...........
-00008030: 0001 0000 0002 0000 0043 0000 0072 5400  .........C...rT.
-00008040: 0000 722e 0000 0072 5500 0000 7229 0000  ..r....rU...r)..
-00008050: 0072 2b00 0000 722b 0000 0072 2c00 0000  .r+...r+...r,...
-00008060: 7257 0000 0054 0400 0072 5800 0000 7a1d  rW...T...rX...z.
-00008070: 4761 6d65 4f76 6572 5f32 505f 5669 6577  GameOver_2P_View
-00008080: 2e6f 6e5f 6869 6465 5f76 6965 7763 0100  .on_hide_viewc..
-00008090: 0000 0000 0000 0000 0000 0100 0000 0200  ................
-000080a0: 0000 4300 0000 7259 0000 0072 2e00 0000  ..C...rY...r....
-000080b0: 725a 0000 0072 2900 0000 722b 0000 0072  rZ...r)...r+...r
-000080c0: 2b00 0000 722c 0000 0072 5d00 0000 5704  +...r,...r]...W.
-000080d0: 0000 725e 0000 007a 1847 616d 654f 7665  ..r^...z.GameOve
-000080e0: 725f 3250 5f56 6965 772e 6f6e 5f64 7261  r_2P_View.on_dra
-000080f0: 7772 5f00 0000 722b 0000 0072 2b00 0000  wr_...r+...r+...
-00008100: 724d 0000 0072 2c00 0000 725a 0100 0043  rM...r,...rZ...C
-00008110: 0400 0073 0a00 0000 0800 0c02 080b 0804  ...s............
-00008120: 1003 725a 0100 0029 1572 3c00 0000 da0a  ..rZ...).r<.....
-00008130: 6172 6361 6465 2e67 7569 72a1 0000 00da  arcade.guir.....
-00008140: 0a4d 6169 6e5f 4669 6c65 7372 0200 0000  .Main_Filesr....
-00008150: 7203 0000 0072 0400 0000 da13 4d6f 6475  r....r......Modu
-00008160: 6c65 4e6f 7446 6f75 6e64 4572 726f 72da  leNotFoundError.
-00008170: 1c77 696c 6c73 655f 6261 636b 6761 6d6d  .willse_backgamm
-00008180: 6f6e 2e4d 6169 6e5f 4669 6c65 73da 0456  on.Main_Files..V
-00008190: 6965 7772 0600 0000 7236 0000 0072 2400  iewr....r6...r$.
-000081a0: 0000 72bd 0000 0072 ea00 0000 7231 0000  ..r....r....r1..
-000081b0: 0072 2501 0000 7226 0100 0072 4f01 0000  .r%...r&...rO...
-000081c0: 722d 0100 0072 5a01 0000 722b 0000 0072  r-...rZ...r+...r
-000081d0: 2b00 0000 722b 0000 0072 2c00 0000 da08  +...r+...r,.....
-000081e0: 3c6d 6f64 756c 653e 0100 0000 7334 0000  <module>....s4..
-000081f0: 0008 0008 0108 0102 020c 010c 0110 010c  ................
-00008200: 010c 010c 0110 0102 fd12 0612 4800 7f12  ............H...
-00008210: 0a00 7f12 7600 7f12 4e12 3c12 3f12 5812  ....v...N.<.?.X.
-00008220: 5812 3b16 3b                             X.;.;
+00000160: 8400 641a 6500 6a09 8303 5a14 4700 641b  ..d.e.j...Z.G.d.
+00000170: 641c 8400 641c 6500 6a09 8303 5a15 4700  d...d.e.j...Z.G.
+00000180: 641d 641e 8400 641e 6500 6a09 8303 5a16  d.d...d.e.j...Z.
+00000190: 4700 641f 6420 8400 6420 6500 6a09 8303  G.d.d ..d e.j...
+000001a0: 5a17 6401 5300 2921 e900 0000 004e 2901  Z.d.S.)!.....N).
+000001b0: da02 4149 2901 da05 4c6f 6769 6329 01da  ..AI)...Logic)..
+000001c0: 0847 7261 7068 6963 7363 0000 0000 0000  .Graphicsc......
+000001d0: 0000 0000 0000 0000 0000 0300 0000 0000  ................
+000001e0: 0000 f334 0000 0065 005a 0164 005a 0287  ...4...e.Z.d.Z..
+000001f0: 0066 0164 0164 0284 085a 0364 0364 0484  .f.d.d...Z.d.d..
+00000200: 005a 0464 0564 0684 005a 0564 0764 0884  .Z.d.d...Z.d.d..
+00000210: 005a 0687 0004 005a 0753 0029 09da 0c4d  .Z.....Z.S.)...M
+00000220: 6169 6e4d 656e 7556 6965 7763 0200 0000  ainMenuViewc....
+00000230: 0000 0000 0000 0000 0e00 0000 0800 0000  ................
+00000240: 0300 0000 73be 0100 0074 0083 00a0 01a1  ....s....t......
+00000250: 0001 007c 0188 005f 0274 036a 04a0 05a1  ...|..._.t.j....
+00000260: 0088 005f 0688 006a 06a0 07a1 0001 0074  ..._...j.......t
+00000270: 036a 04a0 08a1 0088 005f 0974 036a 046a  .j......._.t.j.j
+00000280: 0a64 0164 0264 0364 048d 037d 0288 006a  .d.d.d.d...}...j
+00000290: 09a0 0b7c 026a 0c64 0564 068d 01a1 0101  ...|.j.d.d......
+000002a0: 0074 036a 046a 0a64 0764 0864 0364 048d  .t.j.j.d.d.d.d..
+000002b0: 037d 0388 006a 09a0 0b7c 036a 0c64 0964  .}...j...|.j.d.d
+000002c0: 068d 01a1 0101 0074 036a 046a 0d64 0a64  .......t.j.j.d.d
+000002d0: 0b64 0c8d 027d 0474 036a 046a 0d64 0d64  .d...}.t.j.j.d.d
+000002e0: 0b64 0c8d 027d 0574 036a 046a 0d64 0e64  .d...}.t.j.j.d.d
+000002f0: 0b64 0c8d 027d 0674 036a 046a 0d64 0f64  .d...}.t.j.j.d.d
+00000300: 0b64 0c8d 027d 0774 036a 046a 0d64 1064  .d...}.t.j.j.d.d
+00000310: 0b64 0c8d 027d 0888 006a 09a0 0b7c 046a  .d...}...j...|.j
+00000320: 0c64 0564 068d 01a1 0101 0088 006a 09a0  .d.d.........j..
+00000330: 0b7c 056a 0c64 0564 068d 01a1 0101 0088  .|.j.d.d........
+00000340: 006a 09a0 0b7c 066a 0c64 0564 068d 01a1  .j...|.j.d.d....
+00000350: 0101 0088 006a 09a0 0b7c 076a 0c64 0564  .....j...|.j.d.d
+00000360: 068d 01a1 0101 0088 006a 09a0 0b7c 086a  .........j...|.j
+00000370: 0c64 0564 068d 01a1 0101 0088 006a 06a0  .d.d.........j..
+00000380: 0b74 036a 046a 0e64 1164 1264 1388 006a  .t.j.j.d.d.d...j
+00000390: 0964 148d 04a1 0101 007c 04a0 0f64 15a1  .d.......|...d..
+000003a0: 0187 0066 0164 1664 1784 0883 017d 097c  ...f.d.d.....}.|
+000003b0: 05a0 0f64 15a1 0187 0066 0164 1864 1984  ...d.....f.d.d..
+000003c0: 0883 017d 0a7c 06a0 0f64 15a1 0187 0066  ...}.|...d.....f
+000003d0: 0164 1a64 1b84 0883 017d 0b7c 07a0 0f64  .d.d.....}.|...d
+000003e0: 15a1 0187 0066 0164 1c64 1d84 0883 017d  .....f.d.d.....}
+000003f0: 0c7c 08a0 0f64 15a1 0164 1e64 1f84 0083  .|...d...d.d....
+00000400: 017d 0d64 0053 0029 204e da0a 4261 636b  .}.d.S.) N..Back
+00000410: 6761 6d6d 6f6e e94b 0000 0029 03e9 ff00  gammon.K...)....
+00000420: 0000 7209 0000 0072 0900 0000 2903 da04  ..r....r....)...
+00000430: 7465 7874 da09 666f 6e74 5f73 697a 65da  text..font_size.
+00000440: 0a74 6578 745f 636f 6c6f 72e9 1400 0000  .text_color.....
+00000450: 2901 da06 626f 7474 6f6d 7a0d 6279 2057  )...bottomz.by W
+00000460: 696c 6c73 2045 7264 61e9 1e00 0000 e928  ills Erda......(
+00000470: 0000 005a 0a53 696d 756c 6174 696f 6ee9  ...Z.Simulation.
+00000480: 2c01 0000 2902 720a 0000 00da 0577 6964  ,...).r......wid
+00000490: 7468 7a0a 4f6e 6520 506c 6179 6572 7a0a  thz.One Playerz.
+000004a0: 5477 6f20 506c 6179 6572 da08 5365 7474  Two Player..Sett
+000004b0: 696e 6773 da04 5175 6974 da08 6365 6e74  ings..Quit..cent
+000004c0: 6572 5f78 da06 6365 6e74 6572 7201 0000  er_x..centerr...
+000004d0: 0029 04da 0861 6e63 686f 725f 78da 0861  .)...anchor_x..a
+000004e0: 6e63 686f 725f 79da 0761 6c69 676e 5f79  nchor_y..align_y
+000004f0: da05 6368 696c 64da 086f 6e5f 636c 6963  ..child..on_clic
+00000500: 6b63 0100 0000 0000 0000 0000 0000 0200  kc..............
+00000510: 0000 0300 0000 1300 0000 7376 0000 0088  ..........sv....
+00000520: 006a 006a 01a0 02a1 0001 0088 006a 006a  .j.j.........j.j
+00000530: 0364 0119 0064 026b 0272 1064 036e 0588  .d...d.k.r.d.n..
+00000540: 006a 006a 0364 0119 0088 006a 006a 0364  .j.j.d.....j.j.d
+00000550: 013c 0088 006a 006a 0364 0419 0064 026b  .<...j.j.d...d.k
+00000560: 0272 2464 036e 0588 006a 006a 0364 0419  .r$d.n...j.j.d..
+00000570: 0088 006a 006a 0364 043c 0074 0488 006a  ...j.j.d.<.t...j
+00000580: 0583 017d 0188 006a 00a0 067c 01a1 0101  ...}...j...|....
+00000590: 0064 0053 0029 054e da06 4167 656e 7431  .d.S.).N..Agent1
+000005a0: da05 4875 6d61 6efa 0454 5320 31da 0641  ..Human..TS 1..A
+000005b0: 6765 6e74 3229 07da 0677 696e 646f 77da  gent2)...window.
+000005c0: 094d 6169 6e42 6f61 7264 da11 7365 7453  .MainBoard..setS
+000005d0: 7461 7274 506f 7369 7469 6f6e 73da 0873  tartPositions..s
+000005e0: 6574 7469 6e67 73da 0b4d 6169 6e53 696d  ettings..MainSim
+000005f0: 5669 6577 da0f 6261 636b 6772 6f75 6e64  View..background
+00000600: 436f 6c6f 72da 0973 686f 775f 7669 6577  Color..show_view
+00000610: 2902 da05 6576 656e 74da 0773 696d 5669  )...event..simVi
+00000620: 6577 a901 da04 7365 6c66 a900 fa54 643a  ew....self...Td:
+00000630: 5c28 5729 202d 2043 6f64 655c 2857 2920  \(W) - Code\(W) 
+00000640: 4261 636b 6761 6d6d 6f6e 2050 726f 6a65  Backgammon Proje
+00000650: 6374 2046 696c 6573 5c73 7263 5c77 696c  ct Files\src\wil
+00000660: 6c73 655f 6261 636b 6761 6d6d 6f6e 5c4d  lse_backgammon\M
+00000670: 6169 6e5f 4669 6c65 735c 5669 6577 732e  ain_Files\Views.
+00000680: 7079 da0c 6f6e 5f63 6c69 636b 5f53 696d  py..on_click_Sim
+00000690: 2d00 0000 7312 0000 000c 0214 010a 010a  -...s...........
+000006a0: ff14 020a 010a ff0a 0210 017a 2b4d 6169  ...........z+Mai
+000006b0: 6e4d 656e 7556 6965 772e 5f5f 696e 6974  nMenuView.__init
+000006c0: 5f5f 2e3c 6c6f 6361 6c73 3e2e 6f6e 5f63  __.<locals>.on_c
+000006d0: 6c69 636b 5f53 696d 6301 0000 0000 0000  lick_Simc.......
+000006e0: 0000 0000 0002 0000 0003 0000 0013 0000  ................
+000006f0: 0073 4e00 0000 8800 6a00 6a01 a002 a100  .sN.....j.j.....
+00000700: 0100 8800 6a00 6a03 6401 1900 6402 6b02  ....j.j.d...d.k.
+00000710: 7210 6403 6e05 8800 6a00 6a03 6401 1900  r.d.n...j.j.d...
+00000720: 8800 6a00 6a03 6401 3c00 7404 8800 6a05  ..j.j.d.<.t...j.
+00000730: 8301 7d01 8800 6a00 a006 7c01 a101 0100  ..}...j...|.....
+00000740: 6400 5300 2904 4e72 1f00 0000 721d 0000  d.S.).Nr....r...
+00000750: 0072 1e00 0000 2907 7220 0000 0072 2100  .r....).r ...r!.
+00000760: 0000 7222 0000 0072 2300 0000 da0d 5374  ..r"...r#.....St
+00000770: 6172 745f 3150 5f56 6965 7772 2500 0000  art_1P_Viewr%...
+00000780: 7226 0000 00a9 0272 2700 0000 5a09 7374  r&.....r'...Z.st
+00000790: 6172 7456 6965 7772 2900 0000 722b 0000  artViewr)...r+..
+000007a0: 0072 2c00 0000 da12 6f6e 5f63 6c69 636b  .r,.....on_click
+000007b0: 5f4f 6e65 506c 6179 6572 3700 0000 730c  _OnePlayer7...s.
+000007c0: 0000 000c 0214 010a 010a ff0a 0210 017a  ...............z
+000007d0: 314d 6169 6e4d 656e 7556 6965 772e 5f5f  1MainMenuView.__
+000007e0: 696e 6974 5f5f 2e3c 6c6f 6361 6c73 3e2e  init__.<locals>.
+000007f0: 6f6e 5f63 6c69 636b 5f4f 6e65 506c 6179  on_click_OnePlay
+00000800: 6572 6301 0000 0000 0000 0000 0000 0002  erc.............
+00000810: 0000 0003 0000 0013 0000 0073 2600 0000  ...........s&...
+00000820: 8800 6a00 6a01 a002 a100 0100 7403 8800  ..j.j.......t...
+00000830: 6a04 8301 7d01 8800 6a00 a005 7c01 a101  j...}...j...|...
+00000840: 0100 6400 5300 a901 4e29 0672 2000 0000  ..d.S...N).r ...
+00000850: 7221 0000 0072 2200 0000 da0d 5374 6172  r!...r".....Star
+00000860: 745f 3250 5f56 6965 7772 2500 0000 7226  t_2P_Viewr%...r&
+00000870: 0000 0072 2f00 0000 7229 0000 0072 2b00  ...r/...r)...r+.
+00000880: 0000 722c 0000 00da 126f 6e5f 636c 6963  ..r,.....on_clic
+00000890: 6b5f 5477 6f50 6c61 7965 723f 0000 0073  k_TwoPlayer?...s
+000008a0: 0600 0000 0c02 0a01 1001 7a31 4d61 696e  ..........z1Main
+000008b0: 4d65 6e75 5669 6577 2e5f 5f69 6e69 745f  MenuView.__init_
+000008c0: 5f2e 3c6c 6f63 616c 733e 2e6f 6e5f 636c  _.<locals>.on_cl
+000008d0: 6963 6b5f 5477 6f50 6c61 7965 7263 0100  ick_TwoPlayerc..
+000008e0: 0000 0000 0000 0000 0000 0200 0000 0300  ................
+000008f0: 0000 1300 0000 f322 0000 0088 0088 006a  .......".......j
+00000900: 005f 0174 0288 006a 0383 017d 0188 006a  ._.t...j...}...j
+00000910: 00a0 047c 01a1 0101 0064 0053 0072 3100  ...|.....d.S.r1.
+00000920: 0000 a905 7220 0000 00da 086c 6173 7450  ....r .....lastP
+00000930: 6167 65da 0c53 6574 7469 6e67 7356 6965  age..SettingsVie
+00000940: 7772 2500 0000 7226 0000 00a9 0272 2700  wr%...r&.....r'.
+00000950: 0000 5a0c 7365 7474 696e 6773 5669 6577  ..Z.settingsView
+00000960: 7229 0000 0072 2b00 0000 722c 0000 00da  r)...r+...r,....
+00000970: 116f 6e5f 636c 6963 6b5f 5365 7474 696e  .on_click_Settin
+00000980: 6773 4500 0000 f306 0000 0008 020a 0110  gsE.............
+00000990: 017a 304d 6169 6e4d 656e 7556 6965 772e  .z0MainMenuView.
+000009a0: 5f5f 696e 6974 5f5f 2e3c 6c6f 6361 6c73  __init__.<locals
+000009b0: 3e2e 6f6e 5f63 6c69 636b 5f53 6574 7469  >.on_click_Setti
+000009c0: 6e67 7363 0100 0000 0000 0000 0000 0000  ngsc............
+000009d0: 0100 0000 0200 0000 5300 0000 f30c 0000  ........S.......
+000009e0: 0074 00a0 01a1 0001 0064 0053 0072 3100  .t.......d.S.r1.
+000009f0: 0000 a902 da06 6172 6361 6465 da0c 636c  ......arcade..cl
+00000a00: 6f73 655f 7769 6e64 6f77 a901 7227 0000  ose_window..r'..
+00000a10: 0072 2b00 0000 722b 0000 0072 2c00 0000  .r+...r+...r,...
+00000a20: da0d 6f6e 5f63 6c69 636b 5f51 7569 744b  ..on_click_QuitK
+00000a30: 0000 00f3 0200 0000 0c02 7a2c 4d61 696e  ..........z,Main
+00000a40: 4d65 6e75 5669 6577 2e5f 5f69 6e69 745f  MenuView.__init_
+00000a50: 5f2e 3c6c 6f63 616c 733e 2e6f 6e5f 636c  _.<locals>.on_cl
+00000a60: 6963 6b5f 5175 6974 2910 da05 7375 7065  ick_Quit)...supe
+00000a70: 72da 085f 5f69 6e69 745f 5f72 2500 0000  r..__init__r%...
+00000a80: 723d 0000 00da 0367 7569 da09 5549 4d61  r=.....gui..UIMa
+00000a90: 6e61 6765 72da 076d 616e 6167 6572 da06  nager..manager..
+00000aa0: 656e 6162 6c65 da0b 5549 426f 784c 6179  enable..UIBoxLay
+00000ab0: 6f75 745a 0576 5f62 6f78 da07 5549 4c61  outZ.v_box..UILa
+00000ac0: 6265 6cda 0361 6464 da11 7769 7468 5f73  bel..add..with_s
+00000ad0: 7061 6365 5f61 726f 756e 64da 0c55 4946  pace_around..UIF
+00000ae0: 6c61 7442 7574 746f 6eda 0e55 4941 6e63  latButton..UIAnc
+00000af0: 686f 7257 6964 6765 7472 2700 0000 290e  horWidgetr'...).
+00000b00: 722a 0000 00da 1062 6163 6b67 726f 756e  r*.....backgroun
+00000b10: 645f 636f 6c6f 725a 0a74 6974 6c65 5f74  d_colorZ.title_t
+00000b20: 6578 745a 0d73 7562 7469 746c 655f 7465  extZ.subtitle_te
+00000b30: 7874 5a0a 7369 6d5f 6275 7474 6f6e 5a11  xtZ.sim_buttonZ.
+00000b40: 6f6e 655f 706c 6179 6572 5f62 7574 746f  one_player_butto
+00000b50: 6e5a 1174 776f 5f70 6c61 7965 725f 6275  nZ.two_player_bu
+00000b60: 7474 6f6e 5a0f 7365 7474 696e 6773 5f62  ttonZ.settings_b
+00000b70: 7574 746f 6e5a 0b71 7569 745f 6275 7474  uttonZ.quit_butt
+00000b80: 6f6e 722d 0000 0072 3000 0000 7233 0000  onr-...r0...r3..
+00000b90: 0072 3900 0000 7240 0000 00a9 01da 095f  .r9...r@......._
+00000ba0: 5f63 6c61 7373 5f5f 7229 0000 0072 2c00  _class__r)...r,.
+00000bb0: 0000 7243 0000 0011 0000 0073 3c00 0000  ..rC.......s<...
+00000bc0: 0a01 0601 0c02 0a01 0c02 1202 1401 1201  ................
+00000bd0: 1401 1002 1001 1001 1001 1001 1402 1401  ................
+00000be0: 1401 1401 1401 1e02 0802 0e01 0809 0e01  ................
+00000bf0: 0807 0e01 0805 0e01 0805 0e01 7a15 4d61  ............z.Ma
+00000c00: 696e 4d65 6e75 5669 6577 2e5f 5f69 6e69  inMenuView.__ini
+00000c10: 745f 5f63 0100 0000 0000 0000 0000 0000  t__c............
+00000c20: 0100 0000 0300 0000 4300 0000 f31a 0000  ........C.......
+00000c30: 007c 006a 00a0 01a1 0001 0074 02a0 037c  .|.j.......t...|
+00000c40: 006a 04a1 0101 0064 0053 0072 3100 0000  .j.....d.S.r1...
+00000c50: a905 7246 0000 0072 4700 0000 723d 0000  ..rF...rG...r=..
+00000c60: 00da 1473 6574 5f62 6163 6b67 726f 756e  ...set_backgroun
+00000c70: 645f 636f 6c6f 7272 2500 0000 7229 0000  d_colorr%...r)..
+00000c80: 0072 2b00 0000 722b 0000 0072 2c00 0000  .r+...r+...r,...
+00000c90: da0c 6f6e 5f73 686f 775f 7669 6577 4f00  ..on_show_viewO.
+00000ca0: 0000 f304 0000 000a 0110 017a 194d 6169  ...........z.Mai
+00000cb0: 6e4d 656e 7556 6965 772e 6f6e 5f73 686f  nMenuView.on_sho
+00000cc0: 775f 7669 6577 6301 0000 0000 0000 0000  w_viewc.........
+00000cd0: 0000 0001 0000 0002 0000 0043 0000 00f3  ...........C....
+00000ce0: 0e00 0000 7c00 6a00 a001 a100 0100 6400  ....|.j.......d.
+00000cf0: 5300 7231 0000 00a9 0272 4600 0000 da07  S.r1.....rF.....
+00000d00: 6469 7361 626c 6572 2900 0000 722b 0000  disabler)...r+..
+00000d10: 0072 2b00 0000 722c 0000 00da 0c6f 6e5f  .r+...r,.....on_
+00000d20: 6869 6465 5f76 6965 7753 0000 00f3 0200  hide_viewS......
+00000d30: 0000 0e01 7a19 4d61 696e 4d65 6e75 5669  ....z.MainMenuVi
+00000d40: 6577 2e6f 6e5f 6869 6465 5f76 6965 7763  ew.on_hide_viewc
+00000d50: 0100 0000 0000 0000 0000 0000 0100 0000  ................
+00000d60: 0200 0000 4300 0000 f316 0000 007c 00a0  ....C........|..
+00000d70: 00a1 0001 007c 006a 01a0 02a1 0001 0064  .....|.j.......d
+00000d80: 0053 0072 3100 0000 a903 da05 636c 6561  .S.r1.......clea
+00000d90: 7272 4600 0000 da04 6472 6177 7229 0000  rrF.....drawr)..
+00000da0: 0072 2b00 0000 722b 0000 0072 2c00 0000  .r+...r+...r,...
+00000db0: da07 6f6e 5f64 7261 7756 0000 00f3 0400  ..on_drawV......
+00000dc0: 0000 0801 0e01 7a14 4d61 696e 4d65 6e75  ......z.MainMenu
+00000dd0: 5669 6577 2e6f 6e5f 6472 6177 a908 da08  View.on_draw....
+00000de0: 5f5f 6e61 6d65 5f5f da0a 5f5f 6d6f 6475  __name__..__modu
+00000df0: 6c65 5f5f da0c 5f5f 7175 616c 6e61 6d65  le__..__qualname
+00000e00: 5f5f 7243 0000 0072 5400 0000 7259 0000  __rC...rT...rY..
+00000e10: 0072 5f00 0000 da0d 5f5f 636c 6173 7363  .r_.....__classc
+00000e20: 656c 6c5f 5f72 2b00 0000 722b 0000 0072  ell__r+...r+...r
+00000e30: 4f00 0000 722c 0000 0072 0600 0000 0f00  O...r,...r......
+00000e40: 0000 730a 0000 0008 000c 0208 3e08 0410  ..s.........>...
+00000e50: 0372 0600 0000 6300 0000 0000 0000 0000  .r....c.........
+00000e60: 0000 0000 0000 0003 0000 0000 0000 0072  ...............r
+00000e70: 0500 0000 2909 7237 0000 0063 0200 0000  ....).r7...c....
+00000e80: 0000 0000 0000 0000 1c00 0000 0a00 0000  ................
+00000e90: 0300 0000 7312 0400 0074 0083 00a0 01a1  ....s....t......
+00000ea0: 0001 007c 0188 025f 0274 036a 04a0 05a1  ...|..._.t.j....
+00000eb0: 0088 025f 0688 026a 06a0 07a1 0001 0074  ..._...j.......t
+00000ec0: 036a 046a 0864 0164 0264 0364 0464 0564  .j.j.d.d.d.d.d.d
+00000ed0: 0664 0764 0864 098d 087d 0274 036a 046a  .d.d.d...}.t.j.j
+00000ee0: 0864 0164 0a64 0364 0b64 0c64 0d64 0764  .d.d.d.d.d.d.d.d
+00000ef0: 0864 098d 087d 0374 036a 04a0 0964 0e64  .d...}.t.j...d.d
+00000f00: 0f64 1064 1164 12a1 057d 0474 036a 04a0  .d.d.d...}.t.j..
+00000f10: 0964 0e64 1364 1064 1164 14a1 057d 0574  .d.d.d.d.d...}.t
+00000f20: 036a 046a 0864 1564 1664 0164 1764 1864  .j.j.d.d.d.d.d.d
+00000f30: 0e74 0a6a 0b64 0864 198d 087d 0674 036a  .t.j.d.d...}.t.j
+00000f40: 046a 0864 1564 1a64 0164 1764 1b64 0e74  .j.d.d.d.d.d.d.t
+00000f50: 0a6a 0b64 0864 198d 087d 0774 036a 04a0  .j.d.d...}.t.j..
+00000f60: 0964 1c64 1d64 0164 1164 1ea1 057d 0874  .d.d.d.d.d...}.t
+00000f70: 036a 04a0 0964 1f64 1d64 0164 1164 20a1  .j...d.d.d.d.d .
+00000f80: 057d 0974 036a 04a0 0964 2164 1d64 0164  .}.t.j...d!d.d.d
+00000f90: 1164 22a1 057d 0a74 036a 04a0 0964 2364  .d"..}.t.j...d#d
+00000fa0: 1d64 0164 1164 24a1 057d 0b74 036a 04a0  .d.d.d$..}.t.j..
+00000fb0: 0964 2564 1d64 0164 1164 26a1 057d 0c74  .d%d.d.d.d&..}.t
+00000fc0: 036a 04a0 0964 2764 1d64 0164 1164 28a1  .j...d'd.d.d.d(.
+00000fd0: 057d 0d74 036a 04a0 0964 1f64 2964 0164  .}.t.j...d.d)d.d
+00000fe0: 1164 20a1 057d 0e74 036a 04a0 0964 2164  .d ..}.t.j...d!d
+00000ff0: 2964 0164 1164 22a1 057d 0f74 036a 04a0  )d.d.d"..}.t.j..
+00001000: 0964 1c64 2964 0164 1164 1ea1 057d 1074  .d.d)d.d.d...}.t
+00001010: 036a 04a0 0964 2364 2964 0164 1164 24a1  .j...d#d)d.d.d$.
+00001020: 057d 1174 036a 04a0 0964 2564 2964 0164  .}.t.j...d%d)d.d
+00001030: 1164 26a1 057d 1274 036a 04a0 0964 2764  .d&..}.t.j...d'd
+00001040: 2964 0164 1164 28a1 057d 1374 036a 04a0  )d.d.d(..}.t.j..
+00001050: 0c64 2a64 2b64 0464 1188 026a 0d6a 0e64  .d*d+d.d...j.j.d
+00001060: 2c19 00a1 0589 0074 036a 04a0 0c64 2a64  ,......t.j...d*d
+00001070: 2d64 0464 1188 026a 0d6a 0e64 2e19 00a1  -d.d...j.j.d....
+00001080: 0589 0188 026a 06a0 0f7c 04a1 0101 0088  .....j...|......
+00001090: 026a 06a0 0f7c 05a1 0101 0088 026a 06a0  .j...|.......j..
+000010a0: 0f7c 02a1 0101 0088 026a 06a0 0f7c 03a1  .|.......j...|..
+000010b0: 0101 0088 026a 06a0 0f7c 06a1 0101 0088  .....j...|......
+000010c0: 026a 06a0 0f7c 07a1 0101 0088 026a 06a0  .j...|.......j..
+000010d0: 0f7c 08a1 0101 0088 026a 06a0 0f7c 09a1  .|.......j...|..
+000010e0: 0101 0088 026a 06a0 0f7c 0aa1 0101 0088  .....j...|......
+000010f0: 026a 06a0 0f7c 0ba1 0101 0088 026a 06a0  .j...|.......j..
+00001100: 0f7c 0ca1 0101 0088 026a 06a0 0f7c 0da1  .|.......j...|..
+00001110: 0101 0088 026a 06a0 0f7c 10a1 0101 0088  .....j...|......
+00001120: 026a 06a0 0f7c 0ea1 0101 0088 026a 06a0  .j...|.......j..
+00001130: 0f7c 0fa1 0101 0088 026a 06a0 0f7c 11a1  .|.......j...|..
+00001140: 0101 0088 026a 06a0 0f7c 12a1 0101 0088  .....j...|......
+00001150: 026a 06a0 0f7c 13a1 0101 0088 026a 06a0  .j...|.......j..
+00001160: 0f88 00a1 0101 0088 026a 06a0 0f88 01a1  .........j......
+00001170: 0101 007c 04a0 1064 2fa1 0187 0087 0187  ...|...d/.......
+00001180: 0266 0364 3064 3184 0883 017d 147c 05a0  .f.d0d1....}.|..
+00001190: 1064 2fa1 0164 3264 3384 0083 017d 157c  .d/..d2d3....}.|
+000011a0: 08a0 1064 2fa1 0187 0266 0164 3464 3584  ...d/....f.d4d5.
+000011b0: 0883 017d 167c 09a0 1064 2fa1 0187 0266  ...}.|...d/....f
+000011c0: 0164 3664 3784 0883 017d 177c 0aa0 1064  .d6d7....}.|...d
+000011d0: 2fa1 0187 0266 0164 3864 3984 0883 017d  /....f.d8d9....}
+000011e0: 187c 0ba0 1064 2fa1 0187 0266 0164 3a64  .|...d/....f.d:d
+000011f0: 3b84 0883 017d 197c 0ca0 1064 2fa1 0187  ;....}.|...d/...
+00001200: 0266 0164 3c64 3d84 0883 017d 1a7c 0da0  .f.d<d=....}.|..
+00001210: 1064 2fa1 0187 0266 0164 3e64 3f84 0883  .d/....f.d>d?...
+00001220: 017d 1b7c 10a0 1064 2fa1 0187 0266 0164  .}.|...d/....f.d
+00001230: 4064 3584 0883 017d 167c 0ea0 1064 2fa1  @d5....}.|...d/.
+00001240: 0187 0266 0164 4164 3784 0883 017d 177c  ...f.dAd7....}.|
+00001250: 0fa0 1064 2fa1 0187 0266 0164 4264 3984  ...d/....f.dBd9.
+00001260: 0883 017d 187c 11a0 1064 2fa1 0187 0266  ...}.|...d/....f
+00001270: 0164 4364 3b84 0883 017d 197c 12a0 1064  .dCd;....}.|...d
+00001280: 2fa1 0187 0266 0164 4464 3d84 0883 017d  /....f.dDd=....}
+00001290: 1a7c 13a0 1064 2fa1 0187 0266 0164 4564  .|...d/....f.dEd
+000012a0: 3f84 0883 017d 1b64 0053 0029 464e e964  ?....}.d.S.)FN.d
+000012b0: 0000 0069 7102 0000 e94c 0400 00e9 9600  ...iq....L......
+000012c0: 0000 7213 0000 0072 0f00 0000 7216 0000  ..r....r....r...
+000012d0: 0054 a903 720b 0000 00da 0561 6c69 676e  .T..r......align
+000012e0: da04 626f 6c64 7201 0000 0072 0d00 0000  ..boldr....r....
+000012f0: 7a29 2a41 6765 6e74 2032 2069 7320 7573  z)*Agent 2 is us
+00001300: 6564 2066 6f72 2073 696e 676c 6520 706c  ed for single pl
+00001310: 6179 6572 2067 616d 6573 2ae9 0a00 0000  ayer games*.....
+00001320: e90f 0000 00e9 e902 0000 7208 0000 0072  ..........r....r
+00001330: 1000 0000 da04 4261 636b e9b7 0200 0072  ......Back.....r
+00001340: 1400 0000 e9a5 0000 0069 7b02 0000 e932  .........i{....2
+00001350: 0000 007a 0841 6765 6e74 2031 3a29 0372  ...z.Agent 1:).r
+00001360: 0b00 0000 720c 0000 0072 6b00 0000 6930  ....r....rk...i0
+00001370: 0200 007a 0841 6765 6e74 2032 3a69 0901  ...z.Agent 2:i..
+00001380: 0000 698f 0200 0072 1d00 0000 697c 0100  ..i....r....i|..
+00001390: 00da 0652 616e 646f 6d69 ef01 0000 da03  ...Randomi......
+000013a0: 5042 5069 6202 0000 721e 0000 00e9 d502  PBPib...r.......
+000013b0: 0000 fa04 5453 2032 6948 0300 007a 084e  ....TS 2iH...z.N
+000013c0: 6574 776f 726b 3a69 4402 0000 69bb 0300  etwork:iD...i...
+000013d0: 00e9 8502 0000 fa0b 4e65 7477 6f72 6b31  ........Network1
+000013e0: 2049 4469 3a02 0000 fa0b 4e65 7477 6f72   IDi:.....Networ
+000013f0: 6b32 2049 4472 1b00 0000 6301 0000 0000  k2 IDr....c.....
+00001400: 0000 0000 0000 0001 0000 0003 0000 0013  ................
+00001410: 0000 0073 4200 0000 8800 6a00 8802 6a01  ...sB.....j...j.
+00001420: 6a02 6401 3c00 8801 6a00 8802 6a01 6a02  j.d.<...j...j.j.
+00001430: 6402 3c00 8802 6a01 a003 8802 6a01 6a04  d.<...j.....j.j.
+00001440: a101 0100 7405 6403 8802 6a01 6a02 9b00  ....t.d...j.j...
+00001450: 9d02 8301 0100 6400 5300 2904 4e72 7800  ......d.S.).Nrx.
+00001460: 0000 7279 0000 007a 1320 4375 7272 656e  ..ry...z. Curren
+00001470: 7420 5365 7474 696e 6773 3a20 2906 720a  t Settings: ).r.
+00001480: 0000 0072 2000 0000 7223 0000 0072 2600  ...r ...r#...r&.
+00001490: 0000 7236 0000 00da 0570 7269 6e74 723f  ..r6.....printr?
+000014a0: 0000 00a9 035a 0a4e 6574 776f 726b 4944  .....Z.NetworkID
+000014b0: 315a 0a4e 6574 776f 726b 4944 3272 2a00  1Z.NetworkID2r*.
+000014c0: 0000 722b 0000 0072 2c00 0000 da0d 6f6e  ..r+...r,.....on
+000014d0: 5f63 6c69 636b 5f42 6163 6b99 0000 0073  _click_Back....s
+000014e0: 0800 0000 0e02 0e01 1001 1601 7a2c 5365  ............z,Se
+000014f0: 7474 696e 6773 5669 6577 2e5f 5f69 6e69  ttingsView.__ini
+00001500: 745f 5f2e 3c6c 6f63 616c 733e 2e6f 6e5f  t__.<locals>.on_
+00001510: 636c 6963 6b5f 4261 636b 6301 0000 0000  click_Backc.....
+00001520: 0000 0000 0000 0001 0000 0002 0000 0053  ...............S
+00001530: 0000 0072 3b00 0000 7231 0000 0072 3c00  ...r;...r1...r<.
+00001540: 0000 723f 0000 0072 2b00 0000 722b 0000  ..r?...r+...r+..
+00001550: 0072 2c00 0000 7240 0000 00a0 0000 0072  .r,...r@.......r
+00001560: 4100 0000 7a2c 5365 7474 696e 6773 5669  A...z,SettingsVi
+00001570: 6577 2e5f 5f69 6e69 745f 5f2e 3c6c 6f63  ew.__init__.<loc
+00001580: 616c 733e 2e6f 6e5f 636c 6963 6b5f 5175  als>.on_click_Qu
+00001590: 6974 6301 0000 0000 0000 0000 0000 0001  itc.............
+000015a0: 0000 0003 0000 0013 0000 00f3 1000 0000  ................
+000015b0: 6401 8800 6a00 6a01 6402 3c00 6400 5300  d...j.j.d.<.d.S.
+000015c0: 2903 4e72 1d00 0000 721c 0000 00a9 0272  ).Nr....r......r
+000015d0: 2000 0000 7223 0000 0072 3f00 0000 7229   ...r#...r?...r)
+000015e0: 0000 0072 2b00 0000 722c 0000 00da 106f  ...r+...r,.....o
+000015f0: 6e5f 636c 6963 6b5f 4f70 7469 6f6e 31a4  n_click_Option1.
+00001600: 0000 00f3 0200 0000 1002 7a2f 5365 7474  ..........z/Sett
+00001610: 696e 6773 5669 6577 2e5f 5f69 6e69 745f  ingsView.__init_
+00001620: 5f2e 3c6c 6f63 616c 733e 2e6f 6e5f 636c  _.<locals>.on_cl
+00001630: 6963 6b5f 4f70 7469 6f6e 3163 0100 0000  ick_Option1c....
+00001640: 0000 0000 0000 0000 0100 0000 0300 0000  ................
+00001650: 1300 0000 727d 0000 0029 034e 7273 0000  ....r}...).Nrs..
+00001660: 0072 1c00 0000 727e 0000 0072 3f00 0000  .r....r~...r?...
+00001670: 7229 0000 0072 2b00 0000 722c 0000 00da  r)...r+...r,....
+00001680: 106f 6e5f 636c 6963 6b5f 4f70 7469 6f6e  .on_click_Option
+00001690: 32a8 0000 0072 8000 0000 7a2f 5365 7474  2....r....z/Sett
+000016a0: 696e 6773 5669 6577 2e5f 5f69 6e69 745f  ingsView.__init_
+000016b0: 5f2e 3c6c 6f63 616c 733e 2e6f 6e5f 636c  _.<locals>.on_cl
+000016c0: 6963 6b5f 4f70 7469 6f6e 3263 0100 0000  ick_Option2c....
+000016d0: 0000 0000 0000 0000 0100 0000 0300 0000  ................
+000016e0: 1300 0000 727d 0000 0029 034e 7274 0000  ....r}...).Nrt..
+000016f0: 0072 1c00 0000 727e 0000 0072 3f00 0000  .r....r~...r?...
+00001700: 7229 0000 0072 2b00 0000 722c 0000 00da  r)...r+...r,....
+00001710: 106f 6e5f 636c 6963 6b5f 4f70 7469 6f6e  .on_click_Option
+00001720: 33ac 0000 0072 8000 0000 7a2f 5365 7474  3....r....z/Sett
+00001730: 696e 6773 5669 6577 2e5f 5f69 6e69 745f  ingsView.__init_
+00001740: 5f2e 3c6c 6f63 616c 733e 2e6f 6e5f 636c  _.<locals>.on_cl
+00001750: 6963 6b5f 4f70 7469 6f6e 3363 0100 0000  ick_Option3c....
+00001760: 0000 0000 0000 0000 0100 0000 0300 0000  ................
+00001770: 1300 0000 727d 0000 0029 034e 721e 0000  ....r}...).Nr...
+00001780: 0072 1c00 0000 727e 0000 0072 3f00 0000  .r....r~...r?...
+00001790: 7229 0000 0072 2b00 0000 722c 0000 00da  r)...r+...r,....
+000017a0: 106f 6e5f 636c 6963 6b5f 4f70 7469 6f6e  .on_click_Option
+000017b0: 34b0 0000 0072 8000 0000 7a2f 5365 7474  4....r....z/Sett
+000017c0: 696e 6773 5669 6577 2e5f 5f69 6e69 745f  ingsView.__init_
+000017d0: 5f2e 3c6c 6f63 616c 733e 2e6f 6e5f 636c  _.<locals>.on_cl
+000017e0: 6963 6b5f 4f70 7469 6f6e 3463 0100 0000  ick_Option4c....
+000017f0: 0000 0000 0000 0000 0100 0000 0300 0000  ................
+00001800: 1300 0000 727d 0000 0029 034e 7276 0000  ....r}...).Nrv..
+00001810: 0072 1c00 0000 727e 0000 0072 3f00 0000  .r....r~...r?...
+00001820: 7229 0000 0072 2b00 0000 722c 0000 00da  r)...r+...r,....
+00001830: 106f 6e5f 636c 6963 6b5f 4f70 7469 6f6e  .on_click_Option
+00001840: 35b4 0000 0072 8000 0000 7a2f 5365 7474  5....r....z/Sett
+00001850: 696e 6773 5669 6577 2e5f 5f69 6e69 745f  ingsView.__init_
+00001860: 5f2e 3c6c 6f63 616c 733e 2e6f 6e5f 636c  _.<locals>.on_cl
+00001870: 6963 6b5f 4f70 7469 6f6e 3563 0100 0000  ick_Option5c....
+00001880: 0000 0000 0000 0000 0100 0000 0300 0000  ................
+00001890: 1300 0000 727d 0000 0029 034e da07 4e65  ....r}...).N..Ne
+000018a0: 7477 6f72 6b72 1c00 0000 727e 0000 0072  tworkr....r~...r
+000018b0: 3f00 0000 7229 0000 0072 2b00 0000 722c  ?...r)...r+...r,
+000018c0: 0000 00da 106f 6e5f 636c 6963 6b5f 4f70  .....on_click_Op
+000018d0: 7469 6f6e 36b8 0000 0072 8000 0000 7a2f  tion6....r....z/
+000018e0: 5365 7474 696e 6773 5669 6577 2e5f 5f69  SettingsView.__i
+000018f0: 6e69 745f 5f2e 3c6c 6f63 616c 733e 2e6f  nit__.<locals>.o
+00001900: 6e5f 636c 6963 6b5f 4f70 7469 6f6e 3663  n_click_Option6c
+00001910: 0100 0000 0000 0000 0000 0000 0100 0000  ................
+00001920: 0300 0000 1300 0000 727d 0000 0029 034e  ........r}...).N
+00001930: 721d 0000 0072 1f00 0000 727e 0000 0072  r....r....r~...r
+00001940: 3f00 0000 7229 0000 0072 2b00 0000 722c  ?...r)...r+...r,
+00001950: 0000 0072 7f00 0000 bc00 0000 7280 0000  ...r........r...
+00001960: 0063 0100 0000 0000 0000 0000 0000 0100  .c..............
+00001970: 0000 0300 0000 1300 0000 727d 0000 0029  ..........r}...)
+00001980: 034e 7273 0000 0072 1f00 0000 727e 0000  .Nrs...r....r~..
+00001990: 0072 3f00 0000 7229 0000 0072 2b00 0000  .r?...r)...r+...
+000019a0: 722c 0000 0072 8100 0000 c000 0000 7280  r,...r........r.
+000019b0: 0000 0063 0100 0000 0000 0000 0000 0000  ...c............
+000019c0: 0100 0000 0300 0000 1300 0000 727d 0000  ............r}..
+000019d0: 0029 034e 7274 0000 0072 1f00 0000 727e  .).Nrt...r....r~
+000019e0: 0000 0072 3f00 0000 7229 0000 0072 2b00  ...r?...r)...r+.
+000019f0: 0000 722c 0000 0072 8200 0000 c400 0000  ..r,...r........
+00001a00: 7280 0000 0063 0100 0000 0000 0000 0000  r....c..........
+00001a10: 0000 0100 0000 0300 0000 1300 0000 727d  ..............r}
+00001a20: 0000 0029 034e 721e 0000 0072 1f00 0000  ...).Nr....r....
+00001a30: 727e 0000 0072 3f00 0000 7229 0000 0072  r~...r?...r)...r
+00001a40: 2b00 0000 722c 0000 0072 8300 0000 c800  +...r,...r......
+00001a50: 0000 7280 0000 0063 0100 0000 0000 0000  ..r....c........
+00001a60: 0000 0000 0100 0000 0300 0000 1300 0000  ................
+00001a70: 727d 0000 0029 034e 7276 0000 0072 1f00  r}...).Nrv...r..
+00001a80: 0000 727e 0000 0072 3f00 0000 7229 0000  ..r~...r?...r)..
+00001a90: 0072 2b00 0000 722c 0000 0072 8400 0000  .r+...r,...r....
+00001aa0: cc00 0000 7280 0000 0063 0100 0000 0000  ....r....c......
+00001ab0: 0000 0000 0000 0100 0000 0300 0000 1300  ................
+00001ac0: 0000 727d 0000 0029 034e 7285 0000 0072  ..r}...).Nr....r
+00001ad0: 1f00 0000 727e 0000 0072 3f00 0000 7229  ....r~...r?...r)
+00001ae0: 0000 0072 2b00 0000 722c 0000 0072 8600  ...r+...r,...r..
+00001af0: 0000 d000 0000 7280 0000 0029 1172 4200  ......r....).rB.
+00001b00: 0000 7243 0000 0072 2500 0000 723d 0000  ..rC...r%...r=..
+00001b10: 0072 4400 0000 7245 0000 0072 4600 0000  .rD...rE...rF...
+00001b20: 7247 0000 0072 4900 0000 724c 0000 0072  rG...rI...rL...r
+00001b30: 0400 0000 da05 626c 6163 6bda 0b55 4949  ......black..UII
+00001b40: 6e70 7574 5465 7874 7220 0000 0072 2300  nputTextr ...r#.
+00001b50: 0000 724a 0000 0072 2700 0000 291c 722a  ..rJ...r'...).r*
+00001b60: 0000 0072 2500 0000 5a0e 5365 7474 696e  ...r%...Z.Settin
+00001b70: 6773 5f6c 6162 656c 5a0a 4865 6c70 5f6c  gs_labelZ.Help_l
+00001b80: 6162 656c da0b 4261 636b 5f62 7574 746f  abel..Back_butto
+00001b90: 6eda 0b51 7569 745f 6275 7474 6f6e 5a0e  n..Quit_buttonZ.
+00001ba0: 4149 4167 656e 7431 5f6c 6162 656c 5a0e  AIAgent1_labelZ.
+00001bb0: 4149 4167 656e 7432 5f6c 6162 656c 5a17  AIAgent2_labelZ.
+00001bc0: 4149 4167 656e 7431 5f4f 7074 696f 6e31  AIAgent1_Option1
+00001bd0: 5f62 7574 746f 6e5a 1741 4941 6765 6e74  _buttonZ.AIAgent
+00001be0: 315f 4f70 7469 6f6e 325f 6275 7474 6f6e  1_Option2_button
+00001bf0: 5a17 4149 4167 656e 7431 5f4f 7074 696f  Z.AIAgent1_Optio
+00001c00: 6e33 5f62 7574 746f 6e5a 1741 4941 6765  n3_buttonZ.AIAge
+00001c10: 6e74 315f 4f70 7469 6f6e 345f 6275 7474  nt1_Option4_butt
+00001c20: 6f6e 5a17 4149 4167 656e 7431 5f4f 7074  onZ.AIAgent1_Opt
+00001c30: 696f 6e35 5f62 7574 746f 6e5a 1741 4941  ion5_buttonZ.AIA
+00001c40: 6765 6e74 315f 4f70 7469 6f6e 365f 6275  gent1_Option6_bu
+00001c50: 7474 6f6e 5a17 4149 4167 656e 7432 5f4f  ttonZ.AIAgent2_O
+00001c60: 7074 696f 6e32 5f62 7574 746f 6e5a 1741  ption2_buttonZ.A
+00001c70: 4941 6765 6e74 325f 4f70 7469 6f6e 335f  IAgent2_Option3_
+00001c80: 6275 7474 6f6e 5a17 4149 4167 656e 7432  buttonZ.AIAgent2
+00001c90: 5f4f 7074 696f 6e31 5f62 7574 746f 6e5a  _Option1_buttonZ
+00001ca0: 1741 4941 6765 6e74 325f 4f70 7469 6f6e  .AIAgent2_Option
+00001cb0: 345f 6275 7474 6f6e 5a17 4149 4167 656e  4_buttonZ.AIAgen
+00001cc0: 7432 5f4f 7074 696f 6e35 5f62 7574 746f  t2_Option5_butto
+00001cd0: 6e5a 1741 4941 6765 6e74 325f 4f70 7469  nZ.AIAgent2_Opti
+00001ce0: 6f6e 365f 6275 7474 6f6e 727c 0000 0072  on6_buttonr|...r
+00001cf0: 4000 0000 727f 0000 0072 8100 0000 7282  @...r....r....r.
+00001d00: 0000 0072 8300 0000 7284 0000 0072 8600  ...r....r....r..
+00001d10: 0000 724f 0000 0072 7b00 0000 722c 0000  ..rO...r{...r,..
+00001d20: 0072 4300 0000 5d00 0000 7398 0000 000a  .rC...]...s.....
+00001d30: 0106 010c 020a 011c 021c 0114 0214 0116  ................
+00001d40: 0202 0106 ff16 0202 0106 ff14 0314 0114  ................
+00001d50: 0114 0114 0114 0114 0214 0114 0114 0114  ................
+00001d60: 0114 011c 021c 010c 020c 010c 020c 010c  ................
+00001d70: 010c 010c 020c 010c 010c 010c 010c 010c  ................
+00001d80: 020c 010c 010c 010c 010c 010c 020c 0108  ................
+00001d90: 0212 0108 060a 0108 030e 0108 030e 0108  ................
+00001da0: 030e 0108 030e 0108 030e 0108 030e 0108  ................
+00001db0: 030e 0108 030e 0108 030e 0108 030e 0108  ................
+00001dc0: 030e 0108 0312 017a 1553 6574 7469 6e67  .......z.Setting
+00001dd0: 7356 6965 772e 5f5f 696e 6974 5f5f 6301  sView.__init__c.
+00001de0: 0000 0000 0000 0000 0000 0001 0000 0003  ................
+00001df0: 0000 0043 0000 0072 5100 0000 7231 0000  ...C...rQ...r1..
+00001e00: 0072 5200 0000 7229 0000 0072 2b00 0000  .rR...r)...r+...
+00001e10: 722b 0000 0072 2c00 0000 7254 0000 00d4  r+...r,...rT....
+00001e20: 0000 0072 5500 0000 7a19 5365 7474 696e  ...rU...z.Settin
+00001e30: 6773 5669 6577 2e6f 6e5f 7368 6f77 5f76  gsView.on_show_v
+00001e40: 6965 7763 0100 0000 0000 0000 0000 0000  iewc............
+00001e50: 0100 0000 0200 0000 4300 0000 7256 0000  ........C...rV..
+00001e60: 0072 3100 0000 7257 0000 0072 2900 0000  .r1...rW...r)...
+00001e70: 722b 0000 0072 2b00 0000 722c 0000 0072  r+...r+...r,...r
+00001e80: 5900 0000 d800 0000 725a 0000 007a 1953  Y.......rZ...z.S
+00001e90: 6574 7469 6e67 7356 6965 772e 6f6e 5f68  ettingsView.on_h
+00001ea0: 6964 655f 7669 6577 6301 0000 0000 0000  ide_viewc.......
+00001eb0: 0000 0000 0001 0000 0003 0000 0043 0000  .............C..
+00001ec0: 0073 2400 0000 7c00 a000 a100 0100 7401  .s$...|.......t.
+00001ed0: a002 7c00 6a03 6a04 a101 0100 7c00 6a05  ..|.j.j.....|.j.
+00001ee0: a006 a100 0100 6400 5300 7231 0000 0029  ......d.S.r1...)
+00001ef0: 0772 5d00 0000 7204 0000 00da 0c44 7261  .r]...r......Dra
+00001f00: 7753 6574 7469 6e67 7372 2000 0000 7223  wSettingsr ...r#
+00001f10: 0000 0072 4600 0000 725e 0000 0072 2900  ...rF...r^...r).
+00001f20: 0000 722b 0000 0072 2b00 0000 722c 0000  ..r+...r+...r,..
+00001f30: 0072 5f00 0000 db00 0000 7306 0000 0008  .r_.......s.....
+00001f40: 010e 020e 027a 1453 6574 7469 6e67 7356  .....z.SettingsV
+00001f50: 6965 772e 6f6e 5f64 7261 7772 6100 0000  iew.on_drawra...
+00001f60: 722b 0000 0072 2b00 0000 724f 0000 0072  r+...r+...rO...r
+00001f70: 2c00 0000 7237 0000 005b 0000 0073 0a00  ,...r7...[...s..
+00001f80: 0000 0800 0c02 0877 0804 1003 7237 0000  .......w....r7..
+00001f90: 0063 0000 0000 0000 0000 0000 0000 0000  .c..............
+00001fa0: 0000 0300 0000 0000 0000 7205 0000 0029  ..........r....)
+00001fb0: 0972 2400 0000 6302 0000 0000 0000 0000  .r$...c.........
+00001fc0: 0000 0014 0000 0009 0000 0003 0000 0073  ...............s
+00001fd0: d402 0000 7400 8300 a001 a100 0100 7c01  ....t.........|.
+00001fe0: 8800 5f02 7403 6a04 a005 a100 8800 5f06  .._.t.j......._.
+00001ff0: 8800 6a06 a007 a100 0100 7403 6a04 a008  ..j.......t.j...
+00002000: 6401 6402 6403 6404 6405 a105 7d02 7403  d.d.d.d.d...}.t.
+00002010: 6a04 a008 6401 6406 6403 6404 6407 a105  j...d.d.d.d.d...
+00002020: 7d03 7403 6a04 a008 6401 6401 6403 6408  }.t.j...d.d.d.d.
+00002030: 6409 a105 7d04 7403 6a04 a008 640a 6401  d...}.t.j...d.d.
+00002040: 640b 6404 640c a105 7d05 7403 6a04 a008  d.d.d...}.t.j...
+00002050: 640a 6402 640b 6404 640d a105 7d06 7403  d.d.d.d.d...}.t.
+00002060: 6a04 a008 640a 6406 640b 6404 640e a105  j...d.d.d.d.d...
+00002070: 7d07 7403 6a04 a008 640a 640f 640b 6404  }.t.j...d.d.d.d.
+00002080: 6410 a105 7d08 7403 6a04 a008 640a 6411  d...}.t.j...d.d.
+00002090: 640b 6404 6412 a105 7d09 7403 6a04 6a09  d.d.d...}.t.j.j.
+000020a0: 640a 6413 640b 6404 6414 6415 6416 6417  d.d.d.d.d.d.d.d.
+000020b0: 8d07 7d0a 7403 6a04 a00a 6418 6419 6404  ..}.t.j...d.d.d.
+000020c0: 6404 740b 6a0c 740b 6a0d 740b 6a0e a107  d.t.j.t.j.t.j...
+000020d0: 8800 5f0f 7403 6a04 a00a 641a 6419 6404  .._.t.j...d.d.d.
+000020e0: 6404 740b 6a10 740b 6a11 740b 6a12 a107  d.t.j.t.j.t.j...
+000020f0: 8800 5f13 7403 6a04 6a09 640a 641b 640b  .._.t.j.j.d.d.d.
+00002100: 6404 641c 6415 6416 6417 8d07 7d0b 7403  d.d.d.d.d...}.t.
+00002110: 6a04 6a14 641d 641e 640b 6404 641f 6416  j.j.d.d.d.d.d.d.
+00002120: 6420 8d06 8901 8800 6a06 a015 7c02 a101  d ......j...|...
+00002130: 0100 8800 6a06 a015 7c03 a101 0100 8800  ....j...|.......
+00002140: 6a06 a015 7c04 a101 0100 8800 6a06 a015  j...|.......j...
+00002150: 7c05 a101 0100 8800 6a06 a015 7c06 a101  |.......j...|...
+00002160: 0100 8800 6a06 a015 7c07 a101 0100 8800  ....j...|.......
+00002170: 6a06 a015 7c08 a101 0100 8800 6a06 a015  j...|.......j...
+00002180: 7c09 a101 0100 8800 6a06 a015 7c0a a101  |.......j...|...
+00002190: 0100 8800 6a06 a015 8800 6a0f a101 0100  ....j.....j.....
+000021a0: 8800 6a06 a015 8800 6a13 a101 0100 8800  ..j.....j.......
+000021b0: 6a06 a015 7c0b a101 0100 8800 6a06 a015  j...|.......j...
+000021c0: 8801 a101 0100 7c02 a016 6421 a101 8700  ......|...d!....
+000021d0: 6601 6422 6423 8408 8301 7d0c 7c03 a016  f.d"d#....}.|...
+000021e0: 6421 a101 6424 6425 8400 8301 7d0d 7c04  d!..d$d%....}.|.
+000021f0: a016 6421 a101 8700 6601 6426 6427 8408  ..d!....f.d&d'..
+00002200: 8301 7d0e 7c05 a016 6421 a101 8700 6601  ..}.|...d!....f.
+00002210: 6428 6429 8408 8301 7d0f 7c06 a016 6421  d(d)....}.|...d!
+00002220: a101 8700 6601 642a 642b 8408 8301 7d10  ....f.d*d+....}.
+00002230: 7c07 a016 6421 a101 8700 6601 642c 642b  |...d!....f.d,d+
+00002240: 8408 8301 7d10 7c08 a016 6421 a101 8700  ....}.|...d!....
+00002250: 8701 6602 642d 642b 8408 8301 7d10 7c09  ..f.d-d+....}.|.
+00002260: a016 6421 a101 8700 6601 642e 642f 8408  ..d!....f.d.d/..
+00002270: 8301 7d11 8800 6a0f a016 6421 a101 8700  ..}...j...d!....
+00002280: 6601 6430 6431 8408 8301 7d12 8800 6a13  f.d0d1....}...j.
+00002290: a016 6421 a101 8700 6601 6432 6433 8408  ..d!....f.d2d3..
+000022a0: 8301 7d13 6400 5300 2934 4e72 6d00 0000  ..}.d.S.)4Nrm...
+000022b0: 726e 0000 0072 0800 0000 7210 0000 00da  rn...r....r.....
+000022c0: 0445 7869 7472 7000 0000 7214 0000 00e9  .Exitrp...r.....
+000022d0: 3c00 0000 7a08 4e65 7720 4761 6d65 e9f2  <...z.New Game..
+000022e0: 0300 00e9 af00 0000 7213 0000 007a 0852  ........r....z.R
+000022f0: 756e 2047 616d 657a 0852 756e 2054 7572  un Gamez.Run Tur
+00002300: 6e72 7700 0000 7a0c 5275 6e20 5365 7420  nrw...z.Run Set 
+00002310: 5475 726e 6953 0200 007a 0a45 6469 7420  TurniS...z.Edit 
+00002320: 626f 6172 6469 2102 0000 7a0b 4e65 7874  boardi!...z.Next
+00002330: 2050 6c61 7965 7272 1600 0000 e910 0000   Playerr........
+00002340: 0029 0272 6a00 0000 720b 0000 0069 1f04  .).rj...r....i..
+00002350: 0000 6903 0200 0069 5104 0000 7211 0000  ..i....iQ...r...
+00002360: 007a 0d4e 6578 7420 5365 7420 526f 6c6c  .z.Next Set Roll
+00002370: 693d 0400 0069 0401 0000 7a03 362c 36a9  i=...i....z.6,6.
+00002380: 0172 0b00 0000 721b 0000 0063 0100 0000  .r....r....c....
+00002390: 0000 0000 0000 0000 0200 0000 0300 0000  ................
+000023a0: 1300 0000 f31a 0000 0074 0088 006a 0183  .........t...j..
+000023b0: 017d 0188 006a 02a0 037c 01a1 0101 0064  .}...j...|.....d
+000023c0: 0053 0072 3100 0000 a904 7206 0000 0072  .S.r1.....r....r
+000023d0: 2500 0000 7220 0000 0072 2600 0000 2902  %...r ...r&...).
+000023e0: 7227 0000 005a 086d 6169 6e56 6965 7772  r'...Z.mainViewr
+000023f0: 2900 0000 722b 0000 0072 2c00 0000 727c  )...r+...r,...r|
+00002400: 0000 0010 0100 00f3 0400 0000 0a02 1001  ................
+00002410: 7a2b 4d61 696e 5369 6d56 6965 772e 5f5f  z+MainSimView.__
+00002420: 696e 6974 5f5f 2e3c 6c6f 6361 6c73 3e2e  init__.<locals>.
+00002430: 6f6e 5f63 6c69 636b 5f42 6163 6b63 0100  on_click_Backc..
+00002440: 0000 0000 0000 0000 0000 0100 0000 0200  ................
+00002450: 0000 5300 0000 723b 0000 0072 3100 0000  ..S...r;...r1...
+00002460: 723c 0000 0072 3f00 0000 722b 0000 0072  r<...r?...r+...r
+00002470: 2b00 0000 722c 0000 0072 4000 0000 1501  +...r,...r@.....
+00002480: 0000 7241 0000 007a 2b4d 6169 6e53 696d  ..rA...z+MainSim
+00002490: 5669 6577 2e5f 5f69 6e69 745f 5f2e 3c6c  View.__init__.<l
+000024a0: 6f63 616c 733e 2e6f 6e5f 636c 6963 6b5f  ocals>.on_click_
+000024b0: 5175 6974 6301 0000 0000 0000 0000 0000  Quitc...........
+000024c0: 0001 0000 0002 0000 0013 0000 0073 1800  .............s..
+000024d0: 0000 8800 6a00 6a01 a002 a100 0100 6401  ....j.j.......d.
+000024e0: 8800 6a00 5f03 6400 5300 2902 4e54 2904  ..j._.d.S.).NT).
+000024f0: 7220 0000 0072 2100 0000 7222 0000 00da  r ...r!...r"....
+00002500: 0966 6972 7374 5475 726e 723f 0000 0072  .firstTurnr?...r
+00002510: 2900 0000 722b 0000 0072 2c00 0000 da0c  )...r+...r,.....
+00002520: 6f6e 5f63 6c69 636b 5f4e 6577 1901 0000  on_click_New....
+00002530: 7304 0000 000c 020c 017a 2a4d 6169 6e53  s........z*MainS
+00002540: 696d 5669 6577 2e5f 5f69 6e69 745f 5f2e  imView.__init__.
+00002550: 3c6c 6f63 616c 733e 2e6f 6e5f 636c 6963  <locals>.on_clic
+00002560: 6b5f 4e65 7763 0100 0000 0000 0000 0000  k_Newc..........
+00002570: 0000 0200 0000 0300 0000 1300 0000 7234  ..............r4
+00002580: 0000 0072 3100 0000 7235 0000 0072 3800  ...r1...r5...r8.
+00002590: 0000 7229 0000 0072 2b00 0000 722c 0000  ..r)...r+...r,..
+000025a0: 0072 3900 0000 1e01 0000 723a 0000 007a  .r9.......r:...z
+000025b0: 2f4d 6169 6e53 696d 5669 6577 2e5f 5f69  /MainSimView.__i
+000025c0: 6e69 745f 5f2e 3c6c 6f63 616c 733e 2e6f  nit__.<locals>.o
+000025d0: 6e5f 636c 6963 6b5f 5365 7474 696e 6773  n_click_Settings
+000025e0: 6301 0000 0000 0000 0000 0000 0004 0000  c...............
+000025f0: 0007 0000 0013 0000 0073 d601 0000 8800  .........s......
+00002600: 6a00 6a01 6401 6b03 720a 8800 6a00 6a01  j.j.d.k.r...j.j.
+00002610: 6e05 7402 a003 6402 6403 a102 8800 6a00  n.t...d.d.....j.
+00002620: 5f01 6404 7d01 7c01 73e9 8800 6a00 6a01  _.d.}.|.s...j.j.
+00002630: 6402 6b02 7281 8800 6a00 6a04 6405 1900  d.k.r...j.j.d...
+00002640: 6406 6b02 7225 6ec0 7405 6a06 8800 6a00  d.k.r%n.t.j...j.
+00002650: 6a01 8800 6a00 6a04 6405 1900 8800 6a00  j...j.j.d.....j.
+00002660: 6a01 6401 6b02 6407 8d03 8800 6a00 5f07  j.d.k.d.....j._.
+00002670: 8800 6a00 6a07 a008 8800 6a00 6a09 a101  ..j.j.....j.j...
+00002680: 0100 740a a00b 8800 6a00 6a09 8800 6a00  ..t.....j.j...j.
+00002690: 6a07 8800 6a00 6a04 6405 1900 8800 6a00  j...j.j.d.....j.
+000026a0: 6a04 6408 1900 a104 7d02 8800 6a00 6a09  j.d.....}...j.j.
+000026b0: a00c 7c02 6402 6409 a103 0100 8800 6a00  ..|.d.d.......j.
+000026c0: 6a09 6a0d 6401 1900 6401 6b02 727c 740e  j.j.d...d.k.r|t.
+000026d0: 6a0f 6a10 640a 640b 640c 6400 640d 6701  j.j.d.d.d.d.d.g.
+000026e0: 640e 8d05 7d03 8800 6a11 a012 7c03 a101  d...}...j...|...
+000026f0: 0100 6409 7d01 6403 8800 6a00 5f01 6e64  ..d.}.d...j._.nd
+00002700: 8800 6a00 6a04 640f 1900 6406 6b02 728a  ..j.j.d...d.k.r.
+00002710: 6e5b 7405 6a06 8800 6a00 6a01 8800 6a00  n[t.j...j.j...j.
+00002720: 6a04 640f 1900 8800 6a00 6a01 6401 6b02  j.d.....j.j.d.k.
+00002730: 6407 8d03 8800 6a00 5f07 8800 6a00 6a07  d.....j._...j.j.
+00002740: a008 8800 6a00 6a09 a101 0100 740a a00b  ....j.j.....t...
+00002750: 8800 6a00 6a09 8800 6a00 6a07 8800 6a00  ..j.j...j.j...j.
+00002760: 6a04 640f 1900 8800 6a00 6a04 6410 1900  j.d.....j.j.d...
+00002770: a104 7d02 8800 6a00 6a09 a00c 7c02 6403  ..}...j.j...|.d.
+00002780: 6409 a103 0100 8800 6a00 6a09 6a0d 6402  d.......j.j.j.d.
+00002790: 1900 6401 6b02 72e1 740e 6a0f 6a10 640a  ..d.k.r.t.j.j.d.
+000027a0: 640b 6411 6400 640d 6701 640e 8d05 7d03  d.d.d.d.g.d...}.
+000027b0: 8800 6a11 a012 7c03 a101 0100 6409 7d01  ..j...|.....d.}.
+000027c0: 6402 8800 6a00 5f01 7c01 7216 6400 5300  d...j._.|.r.d.S.
+000027d0: 6400 5300 2912 4e72 0100 0000 e901 0000  d.S.).Nr........
+000027e0: 00e9 0200 0000 4672 1c00 0000 721d 0000  ......Fr....r...
+000027f0: 00a9 01da 0546 6972 7374 7278 0000 0054  .....Firstrx...T
+00002800: 7211 0000 0072 6800 0000 fa48 4761 6d65  r....rh....HGame
+00002810: 204f 7665 723a 200a 506c 6179 6572 2031   Over: .Player 1
+00002820: 2057 696e 7321 2050 6c65 6173 6520 5365   Wins! Please Se
+00002830: 6c65 6374 2027 4e65 7720 4761 6d65 2720  lect 'New Game' 
+00002840: 746f 2073 7461 7274 2061 206e 6577 2067  to start a new g
+00002850: 616d 652e da02 4f6b a905 7212 0000 00da  ame...Ok..r.....
+00002860: 0668 6569 6768 74da 0c6d 6573 7361 6765  .height..message
+00002870: 5f74 6578 74da 0863 616c 6c62 6163 6bda  _text..callback.
+00002880: 0762 7574 746f 6e73 721f 0000 0072 7900  .buttonsr....ry.
+00002890: 0000 fa48 4761 6d65 204f 7665 723a 200a  ...HGame Over: .
+000028a0: 506c 6179 6572 2032 2057 696e 7321 2050  Player 2 Wins! P
+000028b0: 6c65 6173 6520 5365 6c65 6374 2027 4e65  lease Select 'Ne
+000028c0: 7720 4761 6d65 2720 746f 2073 7461 7274  w Game' to start
+000028d0: 2061 206e 6577 2067 616d 652e 2913 7220   a new game.).r 
+000028e0: 0000 00da 0a6e 6578 7450 6c61 7965 72da  .....nextPlayer.
+000028f0: 0672 616e 646f 6dda 0772 616e 6469 6e74  .random..randint
+00002900: 7223 0000 0072 0300 0000 da04 5475 726e  r#...r......Turn
+00002910: da08 4d61 696e 5475 726e da21 7570 6461  ..MainTurn.!upda
+00002920: 7465 506f 7373 6962 6c65 4d6f 7665 7353  tePossibleMovesS
+00002930: 7461 6e64 6172 6446 6f72 6d61 7472 2100  tandardFormatr!.
+00002940: 0000 7202 0000 00da 044d 6169 6eda 096d  ..r......Main..m
+00002950: 616b 654d 6f76 6573 da03 7069 7072 3d00  akeMoves..pipr=.
+00002960: 0000 7244 0000 00da 0c55 494d 6573 7361  ..rD.....UIMessa
+00002970: 6765 426f 7872 4600 0000 724a 0000 0029  geBoxrF...rJ...)
+00002980: 0472 2700 0000 5a09 6761 6d65 5f6f 7665  .r'...Z.game_ove
+00002990: 72da 054d 6f76 6573 da0a 6d65 7373 6167  r..Moves..messag
+000029a0: 6542 6f78 7229 0000 0072 2b00 0000 722c  eBoxr)...r+...r,
+000029b0: 0000 00da 0c6f 6e5f 636c 6963 6b5f 7275  .....on_click_ru
+000029c0: 6e24 0100 0073 5200 0000 2402 0401 0401  n$...sR...$.....
+000029d0: 0c01 1001 0201 1402 0a01 0aff 1202 1a01  ................
+000029e0: 0a01 04ff 1202 1201 0a01 0201 0601 06fe  ................
+000029f0: 0c03 0401 0a01 1002 0201 1402 0a01 0aff  ................
+00002a00: 1202 1a01 0a01 04ff 1202 1201 0a01 0201  ................
+00002a10: 0601 06fe 0c03 0401 0801 0cde 7a2a 4d61  ............z*Ma
+00002a20: 696e 5369 6d56 6965 772e 5f5f 696e 6974  inSimView.__init
+00002a30: 5f5f 2e3c 6c6f 6361 6c73 3e2e 6f6e 5f63  __.<locals>.on_c
+00002a40: 6c69 636b 5f72 756e 6301 0000 0000 0000  lick_runc.......
+00002a50: 0000 0000 0004 0000 0007 0000 0013 0000  ................
+00002a60: 0073 b601 0000 8800 6a00 6a01 6401 6b03  .s......j.j.d.k.
+00002a70: 720a 8800 6a00 6a01 6e05 7402 a003 6402  r...j.j.n.t...d.
+00002a80: 6403 a102 7d01 7c01 6402 6b02 7275 8800  d...}.|.d.k.ru..
+00002a90: 6a00 6a04 6404 1900 6405 6b02 721d 6eb8  j.j.d...d.k.r.n.
+00002aa0: 7405 6a06 7c01 8800 6a00 6a04 6404 1900  t.j.|...j.j.d...
+00002ab0: 8800 6a00 6a01 6401 6b02 6406 8d03 8800  ..j.j.d.k.d.....
+00002ac0: 6a00 5f07 8800 6a00 6a07 a008 8800 6a00  j._...j.j.....j.
+00002ad0: 6a09 a101 0100 740a a00b 8800 6a00 6a09  j.....t.....j.j.
+00002ae0: 8800 6a00 6a07 8800 6a00 6a04 6404 1900  ..j.j...j.j.d...
+00002af0: 8800 6a00 6a04 6407 1900 a104 7d02 8800  ..j.j.d.....}...
+00002b00: 6a00 6a09 a00c 7c02 6402 6408 a103 0100  j.j...|.d.d.....
+00002b10: 8800 6a00 6a09 6a0d 6401 1900 6401 6b02  ..j.j.j.d...d.k.
+00002b20: 7270 740e 6a0f 6a10 6409 640a 640b 6400  rpt.j.j.d.d.d.d.
+00002b30: 640c 6701 640d 8d05 7d03 8800 6a11 a012  d.g.d...}...j...
+00002b40: 7c03 a101 0100 6403 8800 6a00 5f01 6e60  |.....d...j._.n`
+00002b50: 8800 6a00 6a04 640e 1900 6405 6b02 727e  ..j.j.d...d.k.r~
+00002b60: 6e57 7405 6a06 7c01 8800 6a00 6a04 640e  nWt.j.|...j.j.d.
+00002b70: 1900 8800 6a00 6a01 6401 6b02 6406 8d03  ....j.j.d.k.d...
+00002b80: 8800 6a00 5f07 8800 6a00 6a07 a008 8800  ..j._...j.j.....
+00002b90: 6a00 6a09 a101 0100 740a a00b 8800 6a00  j.j.....t.....j.
+00002ba0: 6a09 8800 6a00 6a07 8800 6a00 6a04 640e  j...j.j...j.j.d.
+00002bb0: 1900 8800 6a00 6a04 640f 1900 a104 7d02  ....j.j.d.....}.
+00002bc0: 8800 6a00 6a09 a00c 7c02 6403 6408 a103  ..j.j...|.d.d...
+00002bd0: 0100 8800 6a00 6a09 6a0d 6402 1900 6401  ....j.j.j.d...d.
+00002be0: 6b02 72d1 740e 6a0f 6a10 6409 640a 6410  k.r.t.j.j.d.d.d.
+00002bf0: 6400 640c 6701 640d 8d05 7d03 8800 6a11  d.d.g.d...}...j.
+00002c00: a012 7c03 a101 0100 6402 8800 6a00 5f01  ..|.....d...j._.
+00002c10: 6411 8800 6a00 5f13 6400 5300 2912 4e72  d...j._.d.S.).Nr
+00002c20: 0100 0000 7297 0000 0072 9800 0000 721c  ....r....r....r.
+00002c30: 0000 0072 1d00 0000 7299 0000 0072 7800  ...r....r....rx.
+00002c40: 0000 5472 1100 0000 7268 0000 0072 9b00  ..Tr....rh...r..
+00002c50: 0000 729c 0000 0072 9d00 0000 721f 0000  ..r....r....r...
+00002c60: 0072 7900 0000 72a2 0000 0046 2914 7220  .ry...r....F).r 
+00002c70: 0000 0072 a300 0000 72a4 0000 0072 a500  ...r....r....r..
+00002c80: 0000 7223 0000 0072 0300 0000 72a6 0000  ..r#...r....r...
+00002c90: 0072 a700 0000 72a8 0000 0072 2100 0000  .r....r....r!...
+00002ca0: 7202 0000 0072 a900 0000 72aa 0000 0072  r....r....r....r
+00002cb0: ab00 0000 723d 0000 0072 4400 0000 72ac  ....r=...rD...r.
+00002cc0: 0000 0072 4600 0000 724a 0000 0072 9500  ...rF...rJ...r..
+00002cd0: 0000 2904 7227 0000 00da 0670 6c61 7965  ..).r'.....playe
+00002ce0: 7272 ad00 0000 72ae 0000 0072 2900 0000  rr....r....r)...
+00002cf0: 722b 0000 0072 2c00 0000 72af 0000 004c  r+...r,...r....L
+00002d00: 0100 0073 3c00 0000 2002 0801 1001 0201  ...s<... .......
+00002d10: 1002 0a01 0aff 1202 1a01 0a01 04ff 1202  ................
+00002d20: 1201 0a01 0401 0401 06fe 0c03 0a01 1002  ................
+00002d30: 0201 2402 1201 2801 1201 1201 1801 0c01  ..$...(.........
+00002d40: 0801 0c02 6301 0000 0000 0000 0000 0000  ....c...........
+00002d50: 0006 0000 0007 0000 0013 0000 0073 4202  .............sB.
+00002d60: 0000 8801 6a00 6a01 6401 6402 8d01 7d01  ....j.j.d.d...}.
+00002d70: 6403 6404 8400 7c01 4400 8301 7d02 7402  d.d...|.D...}.t.
+00002d80: a003 7c02 a101 7327 7404 6a05 6a06 6405  ..|...s't.j.j.d.
+00002d90: 6406 6407 6400 6408 6701 6409 8d05 7d03  d.d.d.d.g.d...}.
+00002da0: 8800 6a07 a008 7c03 a101 0100 6400 5300  ..j...|.....d.S.
+00002db0: 7c02 640a 1900 7c02 640b 1900 6b02 7247  |.d...|.d...k.rG
+00002dc0: 8800 6a09 6a0a 7247 7404 6a05 6a06 6405  ..j.j.rGt.j.j.d.
+00002dd0: 6406 640c 6400 6408 6701 6409 8d05 7d03  d.d.d.d.g.d...}.
+00002de0: 8800 6a07 a008 7c03 a101 0100 6400 5300  ..j...|.....d.S.
+00002df0: 8800 6a09 6a0b 640a 6b03 7251 8800 6a09  ..j.j.d.k.rQ..j.
+00002e00: 6a0b 6e05 740c a00d 640b 640d a102 7d04  j.n.t...d.d...}.
+00002e10: 7c04 640b 6b02 72bb 8800 6a09 6a0e 640e  |.d.k.r...j.j.d.
+00002e20: 1900 640f 6b02 7264 6eb7 7402 6a0f 7c04  ..d.k.rdn.t.j.|.
+00002e30: 8800 6a09 6a0e 640e 1900 8800 6a09 6a0a  ..j.j.d.....j.j.
+00002e40: 7c02 6410 8d04 8800 6a09 5f10 8800 6a09  |.d.....j._...j.
+00002e50: 6a10 a011 8800 6a09 6a12 a101 0100 7413  j.....j.j.....t.
+00002e60: a014 8800 6a09 6a12 8800 6a09 6a10 8800  ....j.j...j.j...
+00002e70: 6a09 6a0e 640e 1900 8800 6a09 6a0e 6411  j.j.d.....j.j.d.
+00002e80: 1900 a104 7d05 8800 6a09 6a12 a015 7c05  ....}...j.j...|.
+00002e90: 640b 6412 a103 0100 8800 6a09 6a12 6a16  d.d.......j.j.j.
+00002ea0: 640a 1900 640a 6b02 72b6 7404 6a05 6a06  d...d.k.r.t.j.j.
+00002eb0: 6405 6406 6413 6400 6408 6701 6409 8d05  d.d.d.d.d.g.d...
+00002ec0: 7d03 8800 6a07 a008 7c03 a101 0100 640d  }...j...|.....d.
+00002ed0: 8800 6a09 5f0b 6e60 8800 6a09 6a0e 6414  ..j._.n`..j.j.d.
+00002ee0: 1900 640f 6b02 72c4 6e57 7402 6a0f 7c04  ..d.k.r.nWt.j.|.
+00002ef0: 8800 6a09 6a0e 6414 1900 8800 6a09 6a0a  ..j.j.d.....j.j.
+00002f00: 7c02 6410 8d04 8800 6a09 5f10 8800 6a09  |.d.....j._...j.
+00002f10: 6a10 a011 8800 6a09 6a12 a101 0100 7413  j.....j.j.....t.
+00002f20: a014 8800 6a09 6a12 8800 6a09 6a10 8800  ....j.j...j.j...
+00002f30: 6a09 6a0e 6414 1900 8800 6a09 6a0e 6415  j.j.d.....j.j.d.
+00002f40: 1900 a104 7d05 8800 6a09 6a12 a015 7c05  ....}...j.j...|.
+00002f50: 640d 6412 a103 0100 8800 6a09 6a12 6a16  d.d.......j.j.j.
+00002f60: 640b 1900 640a 6b02 9001 7217 7404 6a05  d...d.k...r.t.j.
+00002f70: 6a06 6405 6406 6416 6400 6408 6701 6409  j.d.d.d.d.d.g.d.
+00002f80: 8d05 7d03 8800 6a07 a008 7c03 a101 0100  ..}...j...|.....
+00002f90: 640b 8800 6a09 5f0b 6417 8800 6a09 5f0a  d...j._.d...j._.
+00002fa0: 6400 5300 2918 4efa 012c a901 da03 7365  d.S.).N..,....se
+00002fb0: 7063 0100 0000 0000 0000 0000 0000 0200  pc..............
+00002fc0: 0000 0400 0000 5300 0000 f314 0000 0067  ......S........g
+00002fd0: 007c 005d 067d 0174 007c 0183 0191 0271  .|.].}.t.|.....q
+00002fe0: 0253 0072 2b00 0000 a901 da03 696e 74a9  .S.r+.......int.
+00002ff0: 02da 022e 30da 036e 756d 722b 0000 0072  ....0..numr+...r
+00003000: 2b00 0000 722c 0000 00da 0a3c 6c69 7374  +...r,.....<list
+00003010: 636f 6d70 3e72 0100 00f3 0200 0000 1400  comp>r..........
+00003020: 7a3e 4d61 696e 5369 6d56 6965 772e 5f5f  z>MainSimView.__
+00003030: 696e 6974 5f5f 2e3c 6c6f 6361 6c73 3e2e  init__.<locals>.
+00003040: 6f6e 5f63 6c69 636b 5f72 756e 2e3c 6c6f  on_click_run.<lo
+00003050: 6361 6c73 3e2e 3c6c 6973 7463 6f6d 703e  cals>.<listcomp>
+00003060: 7211 0000 0072 6800 0000 7a4d 496e 7075  r....rh...zMInpu
+00003070: 7474 6564 2072 6f6c 6c20 6e6f 7420 6c65  tted roll not le
+00003080: 6761 6c2e 200a 506c 6561 7365 2069 6e70  gal. .Please inp
+00003090: 7574 2076 616c 6964 2072 6f6c 6c20 696e  ut valid roll in
+000030a0: 2066 6f72 6d20 6e75 6d31 2c6e 756d 3220   form num1,num2 
+000030b0: 0a65 2e67 2e20 342c 3572 9c00 0000 729d  .e.g. 4,5r....r.
+000030c0: 0000 0072 0100 0000 7297 0000 007a 7049  ...r....r....zpI
+000030d0: 6e70 7574 7465 6420 726f 6c6c 206e 6f74  nputted roll not
+000030e0: 206c 6567 616c 2e20 4e6f 2044 6f75 626c   legal. No Doubl
+000030f0: 6573 2061 6c6c 6f77 6564 2066 6f72 2066  es allowed for f
+00003100: 6972 7374 206d 6f76 652e 200a 506c 6561  irst move. .Plea
+00003110: 7365 2069 6e70 7574 2076 616c 6964 2072  se input valid r
+00003120: 6f6c 6c20 696e 2066 6f72 6d20 6e75 6d31  oll in form num1
+00003130: 2c6e 756d 3220 0a65 2e67 2e20 342c 3572  ,num2 .e.g. 4,5r
+00003140: 9800 0000 721c 0000 0072 1d00 0000 2902  ....r....r....).
+00003150: 729a 0000 00da 0472 6f6c 6c72 7800 0000  r......rollrx...
+00003160: 5472 9b00 0000 721f 0000 0072 7900 0000  Tr....r....ry...
+00003170: 72a2 0000 0046 2917 720a 0000 00da 0672  r....F).r......r
+00003180: 7370 6c69 7472 0300 0000 da0b 6973 4c65  splitr......isLe
+00003190: 6761 6c52 6f6c 6c72 3d00 0000 7244 0000  galRollr=...rD..
+000031a0: 0072 ac00 0000 7246 0000 0072 4a00 0000  .r....rF...rJ...
+000031b0: 7220 0000 0072 9500 0000 72a3 0000 0072  r ...r....r....r
+000031c0: a400 0000 72a5 0000 0072 2300 0000 72a6  ....r....r#...r.
+000031d0: 0000 0072 a700 0000 72a8 0000 0072 2100  ...r....r....r!.
+000031e0: 0000 7202 0000 0072 a900 0000 72aa 0000  ..r....r....r...
+000031f0: 0072 ab00 0000 2906 7227 0000 005a 0f73  .r....).r'...Z.s
+00003200: 6574 5f72 6f6c 6c5f 7374 7269 6e67 5a08  et_roll_stringZ.
+00003210: 7365 745f 726f 6c6c 72ae 0000 0072 b000  set_rollr....r..
+00003220: 0000 72ad 0000 00a9 0272 2a00 0000 5a0d  ..r......r*...Z.
+00003230: 7365 7452 6f6c 6c5f 696e 7075 7472 2b00  setRoll_inputr+.
+00003240: 0000 722c 0000 0072 af00 0000 6e01 0000  ..r,...r....n...
+00003250: 736a 0000 000e 030e 010a 020a 0104 0104  sj..............
+00003260: 0106 fe0c 0304 0118 020a 0102 0106 0106  ................
+00003270: fe0c 0304 0120 0208 0110 0102 0110 0208  ..... ..........
+00003280: 010a ff12 021a 010a 0104 ff12 0212 010a  ................
+00003290: 0104 0104 0106 fe0c 030a 0110 0202 0110  ................
+000032a0: 0208 010a ff12 021a 010a 0104 ff12 0214  ................
+000032b0: 010a 0104 0104 0106 fe0c 0308 010c 0263  ...............c
+000032c0: 0100 0000 0000 0000 0000 0000 0200 0000  ................
+000032d0: 0300 0000 1300 0000 7292 0000 0072 3100  ........r....r1.
+000032e0: 0000 2904 da0d 4564 6974 426f 6172 6456  ..)...EditBoardV
+000032f0: 6965 7772 2500 0000 7220 0000 0072 2600  iewr%...r ...r&.
+00003300: 0000 2902 7227 0000 005a 0845 6469 7456  ..).r'...Z.EditV
+00003310: 6965 7772 2900 0000 722b 0000 0072 2c00  iewr)...r+...r,.
+00003320: 0000 da0d 6f6e 5f63 6c69 636b 5f45 6469  ....on_click_Edi
+00003330: 74a6 0100 0072 9400 0000 7a2b 4d61 696e  t....r....z+Main
+00003340: 5369 6d56 6965 772e 5f5f 696e 6974 5f5f  SimView.__init__
+00003350: 2e3c 6c6f 6361 6c73 3e2e 6f6e 5f63 6c69  .<locals>.on_cli
+00003360: 636b 5f45 6469 7463 0100 0000 0000 0000  ck_Editc........
+00003370: 0000 0000 0100 0000 0200 0000 1300 0000  ................
+00003380: f31c 0000 0088 006a 006a 0164 016b 0372  .......j.j.d.k.r
+00003390: 0864 016e 0164 0288 006a 005f 0164 0053  .d.n.d...j._.d.S
+000033a0: 0029 034e 7297 0000 0072 0100 0000 a902  .).Nr....r......
+000033b0: 7220 0000 0072 a300 0000 723f 0000 0072  r ...r....r?...r
+000033c0: 2900 0000 722b 0000 0072 2c00 0000 da0d  )...r+...r,.....
+000033d0: 6f6e 5f63 6c69 636b 5f44 6172 6bab 0100  on_click_Dark...
+000033e0: 00f3 0200 0000 1c02 7a2b 4d61 696e 5369  ........z+MainSi
+000033f0: 6d56 6965 772e 5f5f 696e 6974 5f5f 2e3c  mView.__init__.<
+00003400: 6c6f 6361 6c73 3e2e 6f6e 5f63 6c69 636b  locals>.on_click
+00003410: 5f44 6172 6b63 0100 0000 0000 0000 0000  _Darkc..........
+00003420: 0000 0100 0000 0200 0000 1300 0000 72c2  ..............r.
+00003430: 0000 0029 034e 7298 0000 0072 0100 0000  ...).Nr....r....
+00003440: 72c3 0000 0072 3f00 0000 7229 0000 0072  r....r?...r)...r
+00003450: 2b00 0000 722c 0000 00da 0e6f 6e5f 636c  +...r,.....on_cl
+00003460: 6963 6b5f 4c69 6768 74af 0100 0072 c500  ick_Light....r..
+00003470: 0000 7a2c 4d61 696e 5369 6d56 6965 772e  ..z,MainSimView.
+00003480: 5f5f 696e 6974 5f5f 2e3c 6c6f 6361 6c73  __init__.<locals
+00003490: 3e2e 6f6e 5f63 6c69 636b 5f4c 6967 6874  >.on_click_Light
+000034a0: 2917 7242 0000 0072 4300 0000 7225 0000  ).rB...rC...r%..
+000034b0: 0072 3d00 0000 7244 0000 0072 4500 0000  .r=...rD...rE...
+000034c0: 7246 0000 0072 4700 0000 724c 0000 0072  rF...rG...rL...r
+000034d0: 4900 0000 da0f 5549 5465 7874 7572 6542  I.....UITextureB
+000034e0: 7574 746f 6e72 0400 0000 da0e 6461 726b  uttonr......dark
+000034f0: 5069 6563 655f 6963 6f6e da0f 6461 726b  Piece_icon..dark
+00003500: 5069 6563 655f 6963 6f6e 32da 0f64 6172  Piece_icon2..dar
+00003510: 6b50 6965 6365 5f69 636f 6e33 da15 6e65  kPiece_icon3..ne
+00003520: 7874 506c 6179 6572 4461 726b 5f62 7574  xtPlayerDark_but
+00003530: 746f 6eda 0f6c 6967 6874 5069 6563 655f  ton..lightPiece_
+00003540: 6963 6f6e da10 6c69 6768 7450 6965 6365  icon..lightPiece
+00003550: 5f69 636f 6e32 da10 6c69 6768 7450 6965  _icon2..lightPie
+00003560: 6365 5f69 636f 6e33 da16 6e65 7874 506c  ce_icon3..nextPl
+00003570: 6179 6572 4c69 6768 745f 6275 7474 6f6e  ayerLight_button
+00003580: 7288 0000 0072 4a00 0000 7227 0000 0029  r....rJ...r'...)
+00003590: 1472 2a00 0000 7225 0000 0072 8900 0000  .r*...r%...r....
+000035a0: 728a 0000 005a 0a4e 6577 5f62 7574 746f  r....Z.New_butto
+000035b0: 6e5a 0e53 6574 7469 6e67 5f62 7574 746f  nZ.Setting_butto
+000035c0: 6e5a 0e52 756e 4761 6d65 5f62 7574 746f  nZ.RunGame_butto
+000035d0: 6e5a 1452 756e 5261 6e64 6f6d 5475 726e  nZ.RunRandomTurn
+000035e0: 5f62 7574 746f 6e5a 1152 756e 5365 7454  _buttonZ.RunSetT
+000035f0: 7572 6e5f 6275 7474 6f6e 5a10 4564 6974  urn_buttonZ.Edit
+00003600: 426f 6172 645f 6275 7474 6f6e 5a10 6e65  Board_buttonZ.ne
+00003610: 7874 506c 6179 6572 5f6c 6162 656c 5a0d  xtPlayer_labelZ.
+00003620: 7365 7452 6f6c 6c5f 6c61 6265 6c72 7c00  setRoll_labelr|.
+00003630: 0000 7240 0000 0072 9600 0000 7239 0000  ..r@...r....r9..
+00003640: 0072 af00 0000 72c1 0000 0072 c400 0000  .r....r....r....
+00003650: 72c6 0000 0072 4f00 0000 72bf 0000 0072  r....rO...r....r
+00003660: 2c00 0000 7243 0000 00e5 0000 0073 6c00  ,...rC.......sl.
+00003670: 0000 0a01 0601 0c02 0a01 1402 1401 1401  ................
+00003680: 1401 1402 1401 1401 1401 1a02 1201 0801  ................
+00003690: 06ff 1202 0801 06ff 1a03 1801 0c02 0c01  ................
+000036a0: 0c01 0c01 0c02 0c01 0c01 0c01 0c02 0e01  ................
+000036b0: 0e01 0c02 0c01 0802 0e01 0804 0a01 0803  ................
+000036c0: 0e01 0804 0e01 0805 0e01 0827 0e01 0821  ...........'...!
+000036d0: 1001 0837 0e01 0a04 0e01 0a03 1201 7a14  ...7..........z.
+000036e0: 4d61 696e 5369 6d56 6965 772e 5f5f 696e  MainSimView.__in
+000036f0: 6974 5f5f 6301 0000 0000 0000 0000 0000  it__c...........
+00003700: 0001 0000 0003 0000 0043 0000 0072 5100  .........C...rQ.
+00003710: 0000 7231 0000 0072 5200 0000 7229 0000  ..r1...rR...r)..
+00003720: 0072 2b00 0000 722b 0000 0072 2c00 0000  .r+...r+...r,...
+00003730: 7254 0000 00b3 0100 0072 5500 0000 7a18  rT.......rU...z.
+00003740: 4d61 696e 5369 6d56 6965 772e 6f6e 5f73  MainSimView.on_s
+00003750: 686f 775f 7669 6577 6301 0000 0000 0000  how_viewc.......
+00003760: 0000 0000 0001 0000 0002 0000 0043 0000  .............C..
+00003770: 0072 5600 0000 7231 0000 0072 5700 0000  .rV...r1...rW...
+00003780: 7229 0000 0072 2b00 0000 722b 0000 0072  r)...r+...r+...r
+00003790: 2c00 0000 7259 0000 00b7 0100 0072 5a00  ,...rY.......rZ.
+000037a0: 0000 7a18 4d61 696e 5369 6d56 6965 772e  ..z.MainSimView.
+000037b0: 6f6e 5f68 6964 655f 7669 6577 6301 0000  on_hide_viewc...
+000037c0: 0000 0000 0000 0000 0001 0000 0005 0000  ................
+000037d0: 0043 0000 0073 e800 0000 7c00 a000 a100  .C...s....|.....
+000037e0: 0100 7c00 6a01 6a02 6401 6b02 7215 7403  ..|.j.j.d.k.r.t.
+000037f0: 6a04 7c00 6a05 5f06 7403 6a07 7c00 6a08  j.|.j._.t.j.|.j.
+00003800: 5f06 6e1b 7c00 6a01 6a02 6402 6b02 7226  _.n.|.j.j.d.k.r&
+00003810: 7403 6a09 7c00 6a08 5f06 7403 6a0a 7c00  t.j.|.j._.t.j.|.
+00003820: 6a05 5f06 6e0a 7403 6a0a 7c00 6a05 5f06  j._.n.t.j.|.j._.
+00003830: 7403 6a07 7c00 6a08 5f06 7403 a00b a100  t.j.|.j._.t.....
+00003840: 0100 7403 a00c 7c00 6a01 6a0d 6a0e 7c00  ..t...|.j.j.j.|.
+00003850: 6a01 6a0d 6a0f a102 0100 7403 a010 a100  j.j.j.....t.....
+00003860: 0100 7c00 6a01 6a0d 6a11 6400 6b03 7253  ..|.j.j.j.d.k.rS
+00003870: 7403 a012 7c00 6a01 6a0d 6a11 a101 0100  t...|.j.j.j.....
+00003880: 7c00 6a01 6a13 6400 6b03 726d 7403 a014  |.j.j.d.k.rmt...
+00003890: 7c00 6a01 6a13 6a15 6403 1900 7c00 6a01  |.j.j.j.d...|.j.
+000038a0: 6a13 6a15 6401 1900 7c00 6a01 6a13 6a16  j.j.d...|.j.j.j.
+000038b0: a103 0100 7c00 6a17 a018 a100 0100 6400  ....|.j.......d.
+000038c0: 5300 2904 4e72 9700 0000 7298 0000 0072  S.).Nr....r....r
+000038d0: 0100 0000 2919 725d 0000 0072 2000 0000  ....).r]...r ...
+000038e0: 72a3 0000 0072 0400 0000 72ca 0000 0072  r....r....r....r
+000038f0: cb00 0000 da07 7465 7874 7572 6572 cc00  ......texturer..
+00003900: 0000 72cf 0000 0072 ce00 0000 72c8 0000  ..r....r....r...
+00003910: 00da 0964 7261 7742 6f61 7264 da0a 6472  ...drawBoard..dr
+00003920: 6177 5069 6563 6573 7221 0000 00da 0970  awPiecesr!.....p
+00003930: 6f73 6974 696f 6e73 72ab 0000 00da 0b44  ositionsr......D
+00003940: 7261 7753 696d 4d61 696e da0c 4d6f 7665  rawSimMain..Move
+00003950: 4c69 6e65 4461 7461 da0d 4472 6177 4d6f  LineData..DrawMo
+00003960: 7665 4c69 6e65 7372 a700 0000 da08 6472  veLinesr......dr
+00003970: 6177 4469 6365 72bc 0000 00da 0b75 6e75  awDicer......unu
+00003980: 7365 645f 6469 6365 7246 0000 0072 5e00  sed_dicerF...r^.
+00003990: 0000 7229 0000 0072 2b00 0000 722b 0000  ..r)...r+...r+..
+000039a0: 0072 2c00 0000 725f 0000 00ba 0100 0073  .r,...r_.......s
+000039b0: 2600 0000 0801 0c02 0a01 0c01 0c01 0a01  &...............
+000039c0: 0c01 0a02 0a01 0802 1801 0802 0e02 1001  ................
+000039d0: 0c01 1c01 0801 04ff 0e03 7a13 4d61 696e  ..........z.Main
+000039e0: 5369 6d56 6965 772e 6f6e 5f64 7261 7772  SimView.on_drawr
+000039f0: 6100 0000 722b 0000 0072 2b00 0000 724f  a...r+...r+...rO
+00003a00: 0000 0072 2c00 0000 7224 0000 00e4 0000  ...r,...r$......
+00003a10: 0073 0c00 0000 0800 0c01 007f 084f 0804  .s...........O..
+00003a20: 1003 7224 0000 0063 0000 0000 0000 0000  ..r$...c........
+00003a30: 0000 0000 0000 0000 0800 0000 0000 0000  ................
+00003a40: 734e 0000 0065 005a 0164 005a 0287 0066  sN...e.Z.d.Z...f
+00003a50: 0164 0164 0284 085a 0364 0364 0484 005a  .d.d...Z.d.d...Z
+00003a60: 0464 0564 0684 005a 0564 0765 0664 0865  .d.d...Z.d.e.d.e
+00003a70: 0664 0965 0664 0a65 0666 0864 0b64 0c84  .d.e.d.e.f.d.d..
+00003a80: 045a 0764 0d64 0e84 005a 0887 0004 005a  .Z.d.d...Z.....Z
+00003a90: 0953 0029 0f72 c000 0000 6302 0000 0000  .S.).r....c.....
+00003aa0: 0000 0000 0000 0010 0000 0009 0000 0003  ................
+00003ab0: 0000 0073 7002 0000 7400 8300 a001 a100  ...sp...t.......
+00003ac0: 0100 7c01 8803 5f02 6400 8803 5f03 7404  ..|..._.d..._.t.
+00003ad0: 6a05 a006 a100 8803 5f07 8803 6a07 a008  j......._...j...
+00003ae0: a100 0100 7404 6a05 a009 6401 6402 6403  ....t.j...d.d.d.
+00003af0: 6404 6405 a105 7d02 7404 6a05 a009 6401  d.d...}.t.j...d.
+00003b00: 6406 6403 6404 6407 a105 7d03 7404 6a05  d.d.d.d...}.t.j.
+00003b10: a00a 6408 6409 6403 6403 740b 6a0c 740b  ..d.d.d.d.t.j.t.
+00003b20: 6a0d 740b 6a0e a107 8902 7404 6a05 a00a  j.t.j.....t.j...
+00003b30: 6408 640a 6403 6403 740b 6a0f 740b 6a10  d.d.d.d.t.j.t.j.
+00003b40: 740b 6a11 a107 8900 7404 6a05 a00a 6408  t.j.....t.j...d.
+00003b50: 640b 6403 6403 740b 6a12 740b 6a13 740b  d.d.d.t.j.t.j.t.
+00003b60: 6a14 a107 8901 7404 6a05 a00a 6408 640c  j.....t.j...d.d.
+00003b70: 6403 6403 740b 6a15 740b 6a16 740b 6a17  d.d.t.j.t.j.t.j.
+00003b80: a107 7d04 7404 6a05 a009 6408 6401 640d  ..}.t.j...d.d.d.
+00003b90: 6404 640e a105 7d05 7404 6a05 6a18 640f  d.d...}.t.j.j.d.
+00003ba0: 6410 6411 6412 6413 6401 6414 8d06 7d06  d.d.d.d.d.d...}.
+00003bb0: 7404 6a05 6a18 640f 6415 6411 6412 6416  t.j.j.d.d.d.d.d.
+00003bc0: 6401 6414 8d06 7d07 7404 6a05 6a18 640f  d.d...}.t.j.j.d.
+00003bd0: 6417 6411 6412 6418 6401 6414 8d06 7d08  d.d.d.d.d.d...}.
+00003be0: 7404 6a05 6a18 640f 6419 6411 6412 641a  t.j.j.d.d.d.d.d.
+00003bf0: 6401 6414 8d06 7d09 8803 6a07 a019 7c02  d.d...}...j...|.
+00003c00: a101 0100 8803 6a07 a019 7c03 a101 0100  ......j...|.....
+00003c10: 8803 6a07 a019 8802 a101 0100 8803 6a07  ..j...........j.
+00003c20: a019 8800 a101 0100 8803 6a07 a019 8801  ..........j.....
+00003c30: a101 0100 8803 6a07 a019 7c04 a101 0100  ......j...|.....
+00003c40: 8803 6a07 a019 7c06 a101 0100 8803 6a07  ..j...|.......j.
+00003c50: a019 7c07 a101 0100 8803 6a07 a019 7c08  ..|.......j...|.
+00003c60: a101 0100 8803 6a07 a019 7c09 a101 0100  ......j...|.....
+00003c70: 8803 6a07 a019 7c05 a101 0100 7c02 a01a  ..j...|.....|...
+00003c80: 641b a101 8703 6601 641c 641d 8408 8301  d.....f.d.d.....
+00003c90: 7d0a 7c03 a01a 641b a101 641e 641f 8400  }.|...d...d.d...
+00003ca0: 8301 7d0b 8802 a01a 641b a101 8700 8701  ..}.....d.......
+00003cb0: 8702 8703 6604 6420 6421 8408 8301 7d0c  ....f.d d!....}.
+00003cc0: 8800 a01a 641b a101 8700 8701 8702 8703  ....d...........
+00003cd0: 6604 6422 6423 8408 8301 7d0d 8801 a01a  f.d"d#....}.....
+00003ce0: 641b a101 8700 8701 8702 8703 6604 6424  d...........f.d$
+00003cf0: 6425 8408 8301 7d0e 7c04 a01a 641b a101  d%....}.|...d...
+00003d00: 8703 6601 6426 6421 8408 8301 7d0c 7c05  ..f.d&d!....}.|.
+00003d10: a01a 641b a101 8703 6601 6427 6428 8408  ..d.....f.d'd(..
+00003d20: 8301 7d0f 6400 5300 2929 4e72 6d00 0000  ..}.d.S.))Nrm...
+00003d30: 726e 0000 0072 0800 0000 7210 0000 00da  rn...r....r.....
+00003d40: 0444 6f6e 6572 7000 0000 7214 0000 0072  .Donerp...r....r
+00003d50: 8e00 0000 e9fe 0100 0069 a401 0000 694a  .........i....iJ
+00003d60: 0100 00e9 f000 0000 728f 0000 007a 0e45  ........r....z.E
+00003d70: 6469 7420 6173 2053 7472 696e 6772 6700  dit as Stringrg.
+00003d80: 0000 690d 0200 00e9 5a00 0000 e92d 0000  ..i.....Z....-..
+00003d90: 007a 0941 6464 204c 6967 6874 7291 0000  .z.Add Lightr...
+00003da0: 0069 b301 0000 7a0b 4164 6420 2020 2044  .i....z.Add    D
+00003db0: 6172 6b69 5901 0000 7a0c 4465 6c65 7465  arkiY...z.Delete
+00003dc0: 2050 6965 6365 7209 0000 007a 0a44 656c   Piecer....z.Del
+00003dd0: 6574 6520 416c 6c72 1b00 0000 6301 0000  ete Allr....c...
+00003de0: 0000 0000 0000 0000 0003 0000 0007 0000  ................
+00003df0: 0013 0000 0073 5c00 0000 7400 a001 8800  .....s\...t.....
+00003e00: 6a02 6a03 6a04 a101 721a 7405 8800 6a06  j.j.j...r.t...j.
+00003e10: 8301 7d01 6400 8800 6a02 6a03 5f07 8800  ..}.d...j.j._...
+00003e20: 6a02 a008 7c01 a101 0100 6400 5300 7409  j...|.....d.S.t.
+00003e30: 6a0a 6a0b 6401 6402 6403 6400 6404 6701  j.j.d.d.d.d.d.g.
+00003e40: 6405 8d05 7d02 8800 6a0c a00d 7c02 a101  d...}...j...|...
+00003e50: 0100 6400 5300 2906 4e72 1100 0000 7268  ..d.S.).Nr....rh
+00003e60: 0000 007a 4b45 7272 6f72 3a20 0a54 6869  ...zKError: .Thi
+00003e70: 7320 696e 206e 6f74 2061 206c 6567 616c  s in not a legal
+00003e80: 2042 6163 6b67 616d 6d6f 6e20 626f 6172   Backgammon boar
+00003e90: 642e 2050 6c65 6173 6520 5072 6f76 6964  d. Please Provid
+00003ea0: 6520 6120 6c65 6761 6c20 626f 6172 642e  e a legal board.
+00003eb0: 729c 0000 0072 9d00 0000 290e 7203 0000  r....r....).r...
+00003ec0: 00da 0c69 734c 6567 616c 426f 6172 6472  ...isLegalBoardr
+00003ed0: 2000 0000 7221 0000 0072 d300 0000 7224   ...r!...r....r$
+00003ee0: 0000 0072 2500 0000 72d5 0000 0072 2600  ...r%...r....r&.
+00003ef0: 0000 723d 0000 0072 4400 0000 72ac 0000  ..r=...rD...r...
+00003f00: 0072 4600 0000 724a 0000 0029 0372 2700  .rF...rJ...).r'.
+00003f10: 0000 7228 0000 0072 ae00 0000 7229 0000  ..r(...r....r)..
+00003f20: 0072 2b00 0000 722c 0000 00da 0d6f 6e5f  .r+...r,.....on_
+00003f30: 636c 6963 6b5f 446f 6e65 0102 0000 7312  click_Done....s.
+00003f40: 0000 0010 020a 010a 0110 010a 0204 0104  ................
+00003f50: 0106 fe10 037a 2d45 6469 7442 6f61 7264  .....z-EditBoard
+00003f60: 5669 6577 2e5f 5f69 6e69 745f 5f2e 3c6c  View.__init__.<l
+00003f70: 6f63 616c 733e 2e6f 6e5f 636c 6963 6b5f  ocals>.on_click_
+00003f80: 446f 6e65 6301 0000 0000 0000 0000 0000  Donec...........
+00003f90: 0001 0000 0002 0000 0053 0000 0072 3b00  .........S...r;.
+00003fa0: 0000 7231 0000 0072 3c00 0000 723f 0000  ..r1...r<...r?..
+00003fb0: 0072 2b00 0000 722b 0000 0072 2c00 0000  .r+...r+...r,...
+00003fc0: 7240 0000 000d 0200 0072 4100 0000 7a2d  r@.......rA...z-
+00003fd0: 4564 6974 426f 6172 6456 6965 772e 5f5f  EditBoardView.__
+00003fe0: 696e 6974 5f5f 2e3c 6c6f 6361 6c73 3e2e  init__.<locals>.
+00003ff0: 6f6e 5f63 6c69 636b 5f51 7569 7463 0100  on_click_Quitc..
+00004000: 0000 0000 0000 0000 0000 0100 0000 0200  ................
+00004010: 0000 1300 0000 f322 0000 0064 0188 035f  ......."...d..._
+00004020: 0074 016a 0288 025f 0374 016a 0488 005f  .t.j..._.t.j..._
+00004030: 0374 016a 0588 015f 0364 0053 0029 024e  .t.j..._.d.S.).N
+00004040: da05 4c69 6768 7429 06da 0474 6f6f 6c72  ..Light)...toolr
+00004050: 0400 0000 72ce 0000 0072 d000 0000 72c8  ....r....r....r.
+00004060: 0000 00da 0b64 656c 6574 655f 6963 6f6e  .....delete_icon
+00004070: 723f 0000 00a9 045a 0b64 6172 6b5f 6275  r?.....Z.dark_bu
+00004080: 7474 6f6e 5a0d 6465 6c65 7465 5f62 7574  ttonZ.delete_but
+00004090: 746f 6e5a 0c6c 6967 6874 5f62 7574 746f  tonZ.light_butto
+000040a0: 6e72 2a00 0000 722b 0000 0072 2c00 0000  nr*...r+...r,...
+000040b0: da0e 6f6e 5f63 6c69 636b 5f6c 6967 6874  ..on_click_light
+000040c0: 1102 0000 f308 0000 0006 0208 0108 010c  ................
+000040d0: 017a 2e45 6469 7442 6f61 7264 5669 6577  .z.EditBoardView
+000040e0: 2e5f 5f69 6e69 745f 5f2e 3c6c 6f63 616c  .__init__.<local
+000040f0: 733e 2e6f 6e5f 636c 6963 6b5f 6c69 6768  s>.on_click_ligh
+00004100: 7463 0100 0000 0000 0000 0000 0000 0100  tc..............
+00004110: 0000 0200 0000 1300 0000 72e0 0000 0029  ..........r....)
+00004120: 024e da04 4461 726b 2906 72e2 0000 0072  .N..Dark).r....r
+00004130: 0400 0000 72cc 0000 0072 d000 0000 72ca  ....r....r....r.
+00004140: 0000 0072 e300 0000 723f 0000 0072 e400  ...r....r?...r..
+00004150: 0000 722b 0000 0072 2c00 0000 da0d 6f6e  ..r+...r,.....on
+00004160: 5f63 6c69 636b 5f64 6172 6b18 0200 0072  _click_dark....r
+00004170: e600 0000 7a2d 4564 6974 426f 6172 6456  ....z-EditBoardV
+00004180: 6965 772e 5f5f 696e 6974 5f5f 2e3c 6c6f  iew.__init__.<lo
+00004190: 6361 6c73 3e2e 6f6e 5f63 6c69 636b 5f64  cals>.on_click_d
+000041a0: 6172 6b63 0100 0000 0000 0000 0000 0000  arkc............
+000041b0: 0100 0000 0200 0000 1300 0000 72e0 0000  ............r...
+000041c0: 0029 024e da06 4465 6c65 7465 2906 72e2  .).N..Delete).r.
+000041d0: 0000 0072 0400 0000 72cc 0000 0072 d000  ...r....r....r..
+000041e0: 0000 72c8 0000 00da 0c64 656c 6574 655f  ..r......delete_
+000041f0: 6963 6f6e 3372 3f00 0000 72e4 0000 0072  icon3r?...r....r
+00004200: 2b00 0000 722c 0000 00da 0f6f 6e5f 636c  +...r,.....on_cl
+00004210: 6963 6b5f 6465 6c65 7465 1f02 0000 72e6  ick_delete....r.
+00004220: 0000 007a 2f45 6469 7442 6f61 7264 5669  ...z/EditBoardVi
+00004230: 6577 2e5f 5f69 6e69 745f 5f2e 3c6c 6f63  ew.__init__.<loc
+00004240: 616c 733e 2e6f 6e5f 636c 6963 6b5f 6465  als>.on_click_de
+00004250: 6c65 7465 6301 0000 0000 0000 0000 0000  letec...........
+00004260: 0001 0000 0002 0000 0013 0000 0073 1400  .............s..
+00004270: 0000 6401 6701 6402 1400 8800 6a00 6a01  ..d.g.d.....j.j.
+00004280: 5f02 6400 5300 2903 4e72 0100 0000 e91c  _.d.S.).Nr......
+00004290: 0000 0029 0372 2000 0000 7221 0000 0072  ...).r ...r!...r
+000042a0: d300 0000 723f 0000 0072 2900 0000 722b  ....r?...r)...r+
+000042b0: 0000 0072 2c00 0000 72e5 0000 0026 0200  ...r,...r....&..
+000042c0: 0073 0200 0000 1402 6301 0000 0000 0000  .s......c.......
+000042d0: 0000 0000 0002 0000 0003 0000 0013 0000  ................
+000042e0: 0072 9200 0000 7231 0000 0029 04da 1145  .r....r1...)...E
+000042f0: 6469 7441 7353 7472 696e 675f 5669 6577  ditAsString_View
+00004300: 7225 0000 0072 2000 0000 7226 0000 0029  r%...r ...r&...)
+00004310: 0272 2700 0000 da08 6564 6974 5669 6577  .r'.....editView
+00004320: 7229 0000 0072 2b00 0000 722c 0000 0072  r)...r+...r,...r
+00004330: c100 0000 2a02 0000 7294 0000 007a 2d45  ....*...r....z-E
+00004340: 6469 7442 6f61 7264 5669 6577 2e5f 5f69  ditBoardView.__i
+00004350: 6e69 745f 5f2e 3c6c 6f63 616c 733e 2e6f  nit__.<locals>.o
+00004360: 6e5f 636c 6963 6b5f 4564 6974 291b 7242  n_click_Edit).rB
+00004370: 0000 0072 4300 0000 7225 0000 0072 e200  ...rC...r%...r..
+00004380: 0000 723d 0000 0072 4400 0000 7245 0000  ..r=...rD...rE..
+00004390: 0072 4600 0000 7247 0000 0072 4c00 0000  .rF...rG...rL...
+000043a0: 72c7 0000 0072 0400 0000 72cc 0000 0072  r....r....r....r
+000043b0: cd00 0000 72ce 0000 0072 c800 0000 72c9  ....r....r....r.
+000043c0: 0000 0072 ca00 0000 72e3 0000 00da 0c64  ...r....r......d
+000043d0: 656c 6574 655f 6963 6f6e 3272 ea00 0000  elete_icon2r....
+000043e0: da0c 7265 7374 6172 745f 6963 6f6e da0d  ..restart_icon..
+000043f0: 7265 7374 6172 745f 6963 6f6e 32da 0d72  restart_icon2..r
+00004400: 6573 7461 7274 5f69 636f 6e33 da0a 5549  estart_icon3..UI
+00004410: 5465 7874 4172 6561 724a 0000 0072 2700  TextArearJ...r'.
+00004420: 0000 2910 722a 0000 0072 2500 0000 da0b  ..).r*...r%.....
+00004430: 446f 6e65 5f62 7574 746f 6e72 8a00 0000  Done_buttonr....
+00004440: 5a0e 7265 7374 6172 745f 6275 7474 6f6e  Z.restart_button
+00004450: 5a0b 4564 6974 5f62 7574 746f 6e5a 0b6c  Z.Edit_buttonZ.l
+00004460: 6967 6874 5f6c 6162 656c 5a0a 6461 726b  ight_labelZ.dark
+00004470: 5f6c 6162 656c 5a0c 6465 6c65 7465 5f6c  _labelZ.delete_l
+00004480: 6162 656c 5a0d 7265 7374 6172 745f 6c61  abelZ.restart_la
+00004490: 6265 6c72 df00 0000 7240 0000 0072 e500  belr....r@...r..
+000044a0: 0000 72e8 0000 0072 eb00 0000 72c1 0000  ..r....r....r...
+000044b0: 0072 4f00 0000 72e4 0000 0072 2c00 0000  .rO...r....r,...
+000044c0: 7243 0000 00d6 0100 0073 6200 0000 0a01  rC.......sb.....
+000044d0: 0601 0602 0c02 0a01 1402 1401 1202 0801  ................
+000044e0: 04ff 1602 0401 04ff 1602 0401 04ff 1602  ................
+000044f0: 0401 04ff 1403 1802 1801 1801 1801 0c02  ................
+00004500: 0c01 0c02 0c01 0c01 0c01 0c02 0c01 0c01  ................
+00004510: 0c01 0c02 0802 0e01 080b 0a01 0803 1401  ................
+00004520: 0806 1401 0806 1401 0806 0e01 0803 1201  ................
+00004530: 7a16 4564 6974 426f 6172 6456 6965 772e  z.EditBoardView.
+00004540: 5f5f 696e 6974 5f5f 6301 0000 0000 0000  __init__c.......
+00004550: 0000 0000 0001 0000 0003 0000 0043 0000  .............C..
+00004560: 0072 5100 0000 7231 0000 0072 5200 0000  .rQ...r1...rR...
+00004570: 7229 0000 0072 2b00 0000 722b 0000 0072  r)...r+...r+...r
+00004580: 2c00 0000 7254 0000 002f 0200 0072 5500  ,...rT.../...rU.
+00004590: 0000 7a1a 4564 6974 426f 6172 6456 6965  ..z.EditBoardVie
+000045a0: 772e 6f6e 5f73 686f 775f 7669 6577 6301  w.on_show_viewc.
+000045b0: 0000 0000 0000 0000 0000 0001 0000 0002  ................
+000045c0: 0000 0043 0000 0072 5600 0000 7231 0000  ...C...rV...r1..
+000045d0: 0072 5700 0000 7229 0000 0072 2b00 0000  .rW...r)...r+...
+000045e0: 722b 0000 0072 2c00 0000 7259 0000 0033  r+...r,...rY...3
+000045f0: 0200 0072 5a00 0000 7a1a 4564 6974 426f  ...rZ...z.EditBo
+00004600: 6172 6456 6965 772e 6f6e 5f68 6964 655f  ardView.on_hide_
+00004610: 7669 6577 da01 78da 0179 da06 6275 7474  view..x..y..butt
+00004620: 6f6e da09 6d6f 6469 6669 6572 7363 0500  on..modifiersc..
+00004630: 0000 0000 0000 0000 0000 0600 0000 0400  ................
+00004640: 0000 4300 0000 7306 0900 0064 007d 0564  ..C...s....d.}.d
+00004650: 017c 0104 0003 006b 0072 0c64 026b 0072  .|.....k.r.d.k.r
+00004660: 1c6e 0201 006e 0e64 037c 0204 0003 006b  .n...n.d.|.....k
+00004670: 0072 1864 046b 0072 1c6e 0201 006e 0264  .r.d.k.r.n...n.d
+00004680: 057d 0564 027c 0104 0003 006b 0072 2664  .}.d.|.....k.r&d
+00004690: 066b 0072 366e 0201 006e 0e64 037c 0204  .k.r6n...n.d.|..
+000046a0: 0003 006b 0072 3264 046b 0072 366e 0201  ...k.r2d.k.r6n..
+000046b0: 006e 0264 077d 0564 067c 0104 0003 006b  .n.d.}.d.|.....k
+000046c0: 0072 4064 086b 0072 506e 0201 006e 0e64  .r@d.k.rPn...n.d
+000046d0: 037c 0204 0003 006b 0072 4c64 046b 0072  .|.....k.rLd.k.r
+000046e0: 506e 0201 006e 0264 097d 0564 087c 0104  Pn...n.d.}.d.|..
+000046f0: 0003 006b 0072 5a64 0a6b 0072 6a6e 0201  ...k.rZd.k.rjn..
+00004700: 006e 0e64 037c 0204 0003 006b 0072 6664  .n.d.|.....k.rfd
+00004710: 046b 0072 6a6e 0201 006e 0264 0b7d 0564  .k.rjn...n.d.}.d
+00004720: 0a7c 0104 0003 006b 0072 7464 0c6b 0072  .|.....k.rtd.k.r
+00004730: 846e 0201 006e 0e64 037c 0204 0003 006b  .n...n.d.|.....k
+00004740: 0072 8064 046b 0072 846e 0201 006e 0264  .r.d.k.r.n...n.d
+00004750: 0d7d 0564 0c7c 0104 0003 006b 0072 8e64  .}.d.|.....k.r.d
+00004760: 0e6b 0072 9e6e 0201 006e 0e64 037c 0204  .k.r.n...n.d.|..
+00004770: 0003 006b 0072 9a64 046b 0072 9e6e 0201  ...k.r.d.k.r.n..
+00004780: 006e 0264 0f7d 0564 017c 0104 0003 006b  .n.d.}.d.|.....k
+00004790: 0072 a864 026b 0072 b86e 0201 006e 0e64  .r.d.k.r.n...n.d
+000047a0: 107c 0204 0003 006b 0072 b464 116b 0072  .|.....k.r.d.k.r
+000047b0: b86e 0201 006e 0264 127d 0564 027c 0104  .n...n.d.}.d.|..
+000047c0: 0003 006b 0072 c264 066b 0072 d26e 0201  ...k.r.d.k.r.n..
+000047d0: 006e 0e64 107c 0204 0003 006b 0072 ce64  .n.d.|.....k.r.d
+000047e0: 116b 0072 d26e 0201 006e 0264 137d 0564  .k.r.n...n.d.}.d
+000047f0: 067c 0104 0003 006b 0072 dc64 086b 0072  .|.....k.r.d.k.r
+00004800: ec6e 0201 006e 0e64 107c 0204 0003 006b  .n...n.d.|.....k
+00004810: 0072 e864 116b 0072 ec6e 0201 006e 0264  .r.d.k.r.n...n.d
+00004820: 147d 0564 087c 0104 0003 006b 0072 f764  .}.d.|.....k.r.d
+00004830: 0a6b 0090 0172 096e 0201 006e 1064 107c  .k...r.n...n.d.|
+00004840: 0204 0003 006b 0090 0172 0564 116b 0090  .....k...r.d.k..
+00004850: 0172 096e 0201 006e 0264 157d 0564 0a7c  .r.n...n.d.}.d.|
+00004860: 0104 0003 006b 0090 0172 1564 0c6b 0090  .....k...r.d.k..
+00004870: 0172 276e 0201 006e 1064 107c 0204 0003  .r'n...n.d.|....
+00004880: 006b 0090 0172 2364 116b 0090 0172 276e  .k...r#d.k...r'n
+00004890: 0201 006e 0264 167d 0564 0c7c 0104 0003  ...n.d.}.d.|....
+000048a0: 006b 0090 0172 3364 0e6b 0090 0172 456e  .k...r3d.k...rEn
+000048b0: 0201 006e 1064 107c 0204 0003 006b 0090  ...n.d.|.....k..
+000048c0: 0172 4164 116b 0090 0172 456e 0201 006e  .rAd.k...rEn...n
+000048d0: 0264 177d 0564 187c 0104 0003 006b 0090  .d.}.d.|.....k..
+000048e0: 0172 5164 196b 0090 0172 636e 0201 006e  .rQd.k...rcn...n
+000048f0: 1064 037c 0204 0003 006b 0090 0172 5f64  .d.|.....k...r_d
+00004900: 046b 0090 0172 636e 0201 006e 0264 1a7d  .k...rcn...n.d.}
+00004910: 0564 197c 0104 0003 006b 0090 0172 6f64  .d.|.....k...rod
+00004920: 1b6b 0090 0172 816e 0201 006e 1064 037c  .k...r.n...n.d.|
+00004930: 0204 0003 006b 0090 0172 7d64 046b 0090  .....k...r}d.k..
+00004940: 0172 816e 0201 006e 0264 1c7d 0564 1b7c  .r.n...n.d.}.d.|
+00004950: 0104 0003 006b 0090 0172 8d64 1d6b 0090  .....k...r.d.k..
+00004960: 0172 9f6e 0201 006e 1064 037c 0204 0003  .r.n...n.d.|....
+00004970: 006b 0090 0172 9b64 046b 0090 0172 9f6e  .k...r.d.k...r.n
+00004980: 0201 006e 0264 1e7d 0564 1d7c 0104 0003  ...n.d.}.d.|....
+00004990: 006b 0090 0172 ab64 1f6b 0090 0172 bd6e  .k...r.d.k...r.n
+000049a0: 0201 006e 1064 037c 0204 0003 006b 0090  ...n.d.|.....k..
+000049b0: 0172 b964 046b 0090 0172 bd6e 0201 006e  .r.d.k...r.n...n
+000049c0: 0264 207d 0564 1f7c 0104 0003 006b 0090  .d }.d.|.....k..
+000049d0: 0172 c964 216b 0090 0172 db6e 0201 006e  .r.d!k...r.n...n
+000049e0: 1064 037c 0204 0003 006b 0090 0172 d764  .d.|.....k...r.d
+000049f0: 046b 0090 0172 db6e 0201 006e 0264 227d  .k...r.n...n.d"}
+00004a00: 0564 217c 0104 0003 006b 0090 0172 e764  .d!|.....k...r.d
+00004a10: 236b 0090 0172 f96e 0201 006e 1064 037c  #k...r.n...n.d.|
+00004a20: 0204 0003 006b 0090 0172 f564 046b 0090  .....k...r.d.k..
+00004a30: 0172 f96e 0201 006e 0264 247d 0564 187c  .r.n...n.d$}.d.|
+00004a40: 0104 0003 006b 0090 0272 0564 196b 0090  .....k...r.d.k..
+00004a50: 0272 176e 0201 006e 1064 107c 0204 0003  .r.n...n.d.|....
+00004a60: 006b 0090 0272 1364 116b 0090 0272 176e  .k...r.d.k...r.n
+00004a70: 0201 006e 0264 257d 0564 197c 0104 0003  ...n.d%}.d.|....
+00004a80: 006b 0090 0272 2364 1b6b 0090 0272 356e  .k...r#d.k...r5n
+00004a90: 0201 006e 1064 107c 0204 0003 006b 0090  ...n.d.|.....k..
+00004aa0: 0272 3164 116b 0090 0272 356e 0201 006e  .r1d.k...r5n...n
+00004ab0: 0264 267d 0564 1b7c 0104 0003 006b 0090  .d&}.d.|.....k..
+00004ac0: 0272 4164 1d6b 0090 0272 536e 0201 006e  .rAd.k...rSn...n
+00004ad0: 1064 107c 0204 0003 006b 0090 0272 4f64  .d.|.....k...rOd
+00004ae0: 116b 0090 0272 536e 0201 006e 0264 277d  .k...rSn...n.d'}
+00004af0: 0564 1d7c 0104 0003 006b 0090 0272 5f64  .d.|.....k...r_d
+00004b00: 1f6b 0090 0272 716e 0201 006e 1064 107c  .k...rqn...n.d.|
+00004b10: 0204 0003 006b 0090 0272 6d64 116b 0090  .....k...rmd.k..
+00004b20: 0272 716e 0201 006e 0264 287d 0564 1f7c  .rqn...n.d(}.d.|
+00004b30: 0104 0003 006b 0090 0272 7d64 216b 0090  .....k...r}d!k..
+00004b40: 0272 8f6e 0201 006e 1064 107c 0204 0003  .r.n...n.d.|....
+00004b50: 006b 0090 0272 8b64 116b 0090 0272 8f6e  .k...r.d.k...r.n
+00004b60: 0201 006e 0264 297d 0564 217c 0104 0003  ...n.d)}.d!|....
+00004b70: 006b 0090 0272 9b64 236b 0090 0272 ad6e  .k...r.d#k...r.n
+00004b80: 0201 006e 1064 107c 0204 0003 006b 0090  ...n.d.|.....k..
+00004b90: 0272 a964 116b 0090 0272 ad6e 0201 006e  .r.d.k...r.n...n
+00004ba0: 0264 2a7d 0564 2b7c 0104 0003 006b 0090  .d*}.d+|.....k..
+00004bb0: 0272 b964 2c6b 0090 0272 cb6e 0201 006e  .r.d,k...r.n...n
+00004bc0: 1064 2d7c 0204 0003 006b 0090 0272 c764  .d-|.....k...r.d
+00004bd0: 2e6b 0090 0272 cb6e 0201 006e 0264 2f7d  .k...r.n...n.d/}
+00004be0: 0564 2b7c 0104 0003 006b 0090 0272 d764  .d+|.....k...r.d
+00004bf0: 2c6b 0090 0272 e96e 0201 006e 1064 307c  ,k...r.n...n.d0|
+00004c00: 0204 0003 006b 0090 0272 e564 316b 0090  .....k...r.d1k..
+00004c10: 0272 e96e 0201 006e 0264 327d 0564 337c  .r.n...n.d2}.d3|
+00004c20: 0104 0003 006b 0090 0272 f564 346b 0090  .....k...r.d4k..
+00004c30: 0372 076e 0201 006e 1064 317c 0204 0003  .r.n...n.d1|....
+00004c40: 006b 0090 0372 0364 2d6b 0090 0372 076e  .k...r.d-k...r.n
+00004c50: 0201 006e 0264 357d 0564 367c 0104 0003  ...n.d5}.d6|....
+00004c60: 006b 0090 0372 1364 376b 0090 0372 256e  .k...r.d7k...r%n
+00004c70: 0201 006e 1064 317c 0204 0003 006b 0090  ...n.d1|.....k..
+00004c80: 0372 2164 2d6b 0090 0372 256e 0201 006e  .r!d-k...r%n...n
+00004c90: 0264 387d 057c 0564 356b 0290 0372 6d7c  .d8}.|.d5k...rm|
+00004ca0: 006a 0064 396b 0290 0372 497c 006a 016a  .j.d9k...rI|.j.j
+00004cb0: 026a 037c 0519 0064 056b 0490 0372 477c  .j.|...d.k...rG|
+00004cc0: 006a 016a 026a 037c 0505 0019 0064 3a37  .j.j.j.|.....d:7
+00004cd0: 0003 003c 0064 0053 0064 0053 007c 006a  ...<.d.S.d.S.|.j
+00004ce0: 0064 3b6b 0290 0372 5c7c 006a 016a 026a  .d;k...r\|.j.j.j
+00004cf0: 037c 0505 0019 0064 0737 0003 003c 0064  .|.....d.7...<.d
+00004d00: 0053 007c 006a 0064 3c6b 0290 0372 6b64  .S.|.j.d<k...rkd
+00004d10: 057c 006a 016a 026a 037c 053c 0064 0053  .|.j.j.j.|.<.d.S
+00004d20: 0064 0053 007c 0564 386b 0290 0372 b57c  .d.S.|.d8k...r.|
+00004d30: 006a 0064 396b 0290 0372 857c 006a 016a  .j.d9k...r.|.j.j
+00004d40: 026a 037c 0505 0019 0064 0737 0003 003c  .j.|.....d.7...<
+00004d50: 0064 0053 007c 006a 0064 3b6b 0290 0372  .d.S.|.j.d;k...r
+00004d60: a47c 006a 016a 026a 037c 0519 0064 056b  .|.j.j.j.|...d.k
+00004d70: 0490 0372 a27c 006a 016a 026a 037c 0505  ...r.|.j.j.j.|..
+00004d80: 0019 0064 3a37 0003 003c 0064 0053 0064  ...d:7...<.d.S.d
+00004d90: 0053 007c 006a 0064 3c6b 0290 0372 b364  .S.|.j.d<k...r.d
+00004da0: 057c 006a 016a 026a 037c 053c 0064 0053  .|.j.j.j.|.<.d.S
+00004db0: 0064 0053 007c 0564 2f6b 0290 0372 fd7c  .d.S.|.d/k...r.|
+00004dc0: 006a 0064 396b 0290 0372 cd7c 006a 016a  .j.d9k...r.|.j.j
+00004dd0: 026a 037c 0505 0019 0064 0737 0003 003c  .j.|.....d.7...<
+00004de0: 0064 0053 007c 006a 0064 3b6b 0290 0372  .d.S.|.j.d;k...r
+00004df0: ec7c 006a 016a 026a 037c 0519 0064 056b  .|.j.j.j.|...d.k
+00004e00: 0490 0372 ea7c 006a 016a 026a 037c 0505  ...r.|.j.j.j.|..
+00004e10: 0019 0064 3a37 0003 003c 0064 0053 0064  ...d:7...<.d.S.d
+00004e20: 0053 007c 006a 0064 3c6b 0290 0372 fb64  .S.|.j.d<k...r.d
+00004e30: 057c 006a 016a 026a 037c 053c 0064 0053  .|.j.j.j.|.<.d.S
+00004e40: 0064 0053 007c 0564 326b 0290 0472 457c  .d.S.|.d2k...rE|
+00004e50: 006a 0064 396b 0290 0472 217c 006a 016a  .j.d9k...r!|.j.j
+00004e60: 026a 037c 0519 0064 056b 0490 0472 1f7c  .j.|...d.k...r.|
+00004e70: 006a 016a 026a 037c 0505 0019 0064 3a37  .j.j.j.|.....d:7
+00004e80: 0003 003c 0064 0053 0064 0053 007c 006a  ...<.d.S.d.S.|.j
+00004e90: 0064 3b6b 0290 0472 347c 006a 016a 026a  .d;k...r4|.j.j.j
+00004ea0: 037c 0505 0019 0064 0737 0003 003c 0064  .|.....d.7...<.d
+00004eb0: 0053 007c 006a 0064 3c6b 0290 0472 4364  .S.|.j.d<k...rCd
+00004ec0: 057c 006a 016a 026a 037c 053c 0064 0053  .|.j.j.j.|.<.d.S
+00004ed0: 0064 0053 007c 0564 006b 0390 0472 7f7c  .d.S.|.d.k...r.|
+00004ee0: 006a 0064 396b 0290 0472 5d7c 006a 016a  .j.d9k...r]|.j.j
+00004ef0: 026a 037c 0505 0019 0064 0737 0003 003c  .j.|.....d.7...<
+00004f00: 0064 0053 007c 006a 0064 3b6b 0290 0472  .d.S.|.j.d;k...r
+00004f10: 707c 006a 016a 026a 037c 0505 0019 0064  p|.j.j.j.|.....d
+00004f20: 3a37 0003 003c 0064 0053 007c 006a 0064  :7...<.d.S.|.j.d
+00004f30: 3c6b 0290 0472 8164 057c 006a 016a 026a  <k...r.d.|.j.j.j
+00004f40: 037c 053c 0064 0053 0064 0053 0064 0053  .|.<.d.S.d.S.d.S
+00004f50: 0029 3d4e e9d8 0000 0069 1401 0000 69e4  .)=N.....i....i.
+00004f60: 0100 0069 fe02 0000 7201 0000 0069 5001  ...i....r....iP.
+00004f70: 0000 7297 0000 0069 8c01 0000 7298 0000  ..r....i....r...
+00004f80: 0069 c801 0000 e903 0000 0069 0402 0000  .i.........i....
+00004f90: e904 0000 0069 4002 0000 e905 0000 00e9  .....i@.........
+00004fa0: 2c00 0000 693c 0100 00e9 1700 0000 e916  ,...i<..........
+00004fb0: 0000 00e9 1500 0000 720d 0000 00e9 1300  ........r.......
+00004fc0: 0000 e912 0000 0069 7002 0000 69ac 0200  .......ip...i...
+00004fd0: 00e9 0600 0000 69e8 0200 00e9 0700 0000  ......i.........
+00004fe0: 6924 0300 00e9 0800 0000 6960 0300 00e9  i$........i`....
+00004ff0: 0900 0000 699c 0300 0072 6c00 0000 69d8  ....i....rl...i.
+00005000: 0300 00e9 0b00 0000 e911 0000 0072 9000  .............r..
+00005010: 0000 726d 0000 00e9 0e00 0000 e90d 0000  ..rm............
+00005020: 00e9 0c00 0000 e978 0000 00e9 b400 0000  .......x........
+00005030: e9c2 0100 0069 ee02 0000 e91b 0000 0072  .....i.........r
+00005040: 7200 0000 695e 0100 00e9 1a00 0000 69f9  r...i^........i.
+00005050: 0100 0069 2b02 0000 e918 0000 0072 7700  ...i+........rw.
+00005060: 0000 7270 0000 00e9 1900 0000 72e1 0000  ..rp........r...
+00005070: 00e9 ffff ffff 72e7 0000 0072 e900 0000  ......r....r....
+00005080: 2904 72e2 0000 0072 2000 0000 7221 0000  ).r....r ...r!..
+00005090: 0072 d300 0000 2906 722a 0000 0072 f500  .r....).r*...r..
+000050a0: 0000 72f6 0000 0072 f700 0000 72f8 0000  ..r....r....r...
+000050b0: 00da 0870 6f73 6974 696f 6e72 2b00 0000  ...positionr+...
+000050c0: 722b 0000 0072 2c00 0000 da0e 6f6e 5f6d  r+...r,.....on_m
+000050d0: 6f75 7365 5f70 7265 7373 3602 0000 73d4  ouse_press6...s.
+000050e0: 0000 0004 0130 0104 0130 0104 0130 0104  .....0...0...0..
+000050f0: 0130 0104 0130 0104 0130 0104 0130 0104  .0...0...0...0..
+00005100: 0130 0104 0130 0104 0136 0104 0138 0104  .0...0...6...8..
+00005110: 0138 0104 0138 0104 0138 0104 0138 0104  .8...8...8...8..
+00005120: 0138 0104 0138 0104 0138 0104 0138 0104  .8...8...8...8..
+00005130: 0138 0104 0138 0104 0138 0104 0138 0104  .8...8...8...8..
+00005140: 0138 0104 0138 0104 0138 0104 0138 0104  .8...8...8...8..
+00005150: 0138 0104 010a 020c 0114 011a 0104 ff0c  .8..............
+00005160: 021a 010c 0112 0104 ff0a 020c 011a 010c  ................
+00005170: 0114 011a 0104 ff0c 0212 0104 ff0a 020c  ................
+00005180: 011a 010c 0114 011a 0104 ff0c 0212 0104  ................
+00005190: ff0a 020c 0114 011a 0104 ff0c 021a 010c  ................
+000051a0: 0112 0104 ff0a 020c 011a 010c 011a 010c  ................
+000051b0: 0112 0104 fa04 057a 1c45 6469 7442 6f61  .......z.EditBoa
+000051c0: 7264 5669 6577 2e6f 6e5f 6d6f 7573 655f  rdView.on_mouse_
+000051d0: 7072 6573 7363 0100 0000 0000 0000 0000  pressc..........
+000051e0: 0000 0100 0000 0400 0000 4300 0000 733e  ..........C...s>
+000051f0: 0000 007c 00a0 00a1 0001 0074 01a0 02a1  ...|.......t....
+00005200: 0001 0074 01a0 037c 006a 046a 056a 067c  ...t...|.j.j.j.|
+00005210: 006a 046a 056a 07a1 0201 0074 01a0 08a1  .j.j.j.....t....
+00005220: 0001 007c 006a 09a0 0aa1 0001 0064 0053  ...|.j.......d.S
+00005230: 0072 3100 0000 290b 725d 0000 0072 0400  .r1...).r]...r..
+00005240: 0000 72d1 0000 0072 d200 0000 7220 0000  ..r....r....r ..
+00005250: 0072 2100 0000 72d3 0000 0072 ab00 0000  .r!...r....r....
+00005260: da0c 4472 6177 4261 7242 6f78 6573 7246  ..DrawBarBoxesrF
+00005270: 0000 0072 5e00 0000 7229 0000 0072 2b00  ...r^...r)...r+.
+00005280: 0000 722b 0000 0072 2c00 0000 725f 0000  ..r+...r,...r_..
+00005290: 0099 0200 0073 0a00 0000 0801 0802 1801  .....s..........
+000052a0: 0801 0e01 7a15 4564 6974 426f 6172 6456  ....z.EditBoardV
+000052b0: 6965 772e 6f6e 5f64 7261 7729 0a72 6200  iew.on_draw).rb.
+000052c0: 0000 7263 0000 0072 6400 0000 7243 0000  ..rc...rd...rC..
+000052d0: 0072 5400 0000 7259 0000 0072 b600 0000  .rT...rY...r....
+000052e0: 7215 0100 0072 5f00 0000 7265 0000 0072  r....r_...re...r
+000052f0: 2b00 0000 722b 0000 0072 4f00 0000 722c  +...r+...rO...r,
+00005300: 0000 0072 c000 0000 d501 0000 730c 0000  ...r........s...
+00005310: 0008 000c 0108 5908 041a 0310 6372 c000  ......Y.....cr..
+00005320: 0000 6300 0000 0000 0000 0000 0000 0000  ..c.............
+00005330: 0000 0003 0000 0000 0000 0072 0500 0000  ...........r....
+00005340: 2909 72ed 0000 0063 0200 0000 0000 0000  ).r....c........
+00005350: 0000 0000 0600 0000 0700 0000 0300 0000  ................
+00005360: 73a0 0000 0074 0083 00a0 01a1 0001 007c  s....t.........|
+00005370: 0188 005f 0274 036a 04a0 05a1 0088 005f  ..._.t.j......._
+00005380: 0688 006a 06a0 07a1 0001 0064 0164 0284  ...j.......d.d..
+00005390: 0088 006a 086a 096a 0a44 0083 017d 0264  ...j.j.j.D...}.d
+000053a0: 03a0 0b7c 02a1 017d 0374 036a 04a0 0c64  ...|...}.t.j...d
+000053b0: 0464 0564 0664 0764 08a1 057d 0474 036a  .d.d.d.d...}.t.j
+000053c0: 04a0 0d64 0964 0a64 0b64 077c 03a1 0589  ...d.d.d.d.|....
+000053d0: 0188 006a 06a0 0e7c 04a1 0101 0088 006a  ...j...|.......j
+000053e0: 06a0 0e88 01a1 0101 007c 04a0 0f64 0ca1  .........|...d..
+000053f0: 0187 0087 0166 0264 0d64 0e84 0883 017d  .....f.d.d.....}
+00005400: 0564 0053 0029 0f4e 6301 0000 0000 0000  .d.S.).Nc.......
+00005410: 0000 0000 0002 0000 0004 0000 0053 0000  .............S..
+00005420: 0072 b400 0000 722b 0000 0029 01da 0373  .r....r+...)...s
+00005430: 7472 72b7 0000 0072 2b00 0000 722b 0000  trr....r+...r+..
+00005440: 0072 2c00 0000 72ba 0000 00ab 0200 0072  .r,...r........r
+00005450: bb00 0000 7a2e 4564 6974 4173 5374 7269  ....z.EditAsStri
+00005460: 6e67 5f56 6965 772e 5f5f 696e 6974 5f5f  ng_View.__init__
+00005470: 2e3c 6c6f 6361 6c73 3e2e 3c6c 6973 7463  .<locals>.<listc
+00005480: 6f6d 703e fa02 2c20 6926 0200 0072 1100  omp>.., i&...r..
+00005490: 0000 7266 0000 0072 7200 0000 72d9 0000  ..rf...rr...r...
+000054a0: 0069 4501 0000 e977 0100 00e9 5802 0000  .iE....w....X...
+000054b0: 721b 0000 0063 0100 0000 0000 0000 0000  r....c..........
+000054c0: 0000 0500 0000 0a00 0000 1300 0000 73a4  ..............s.
+000054d0: 0000 0088 016a 006a 0164 0164 028d 017d  .....j.j.d.d...}
+000054e0: 017a 0964 0364 0484 007c 0144 0083 017d  .z.d.d...|.D...}
+000054f0: 0257 006e 1601 0001 0001 0074 026a 036a  .W.n.......t.j.j
+00005500: 0464 0564 0664 0764 0064 0867 0164 098d  .d.d.d.d.d.g.d..
+00005510: 057d 0388 006a 05a0 067c 03a1 0101 0059  .}...j...|.....Y
+00005520: 0074 07a0 087c 02a1 0172 3e7c 0288 006a  .t...|...r>|...j
+00005530: 096a 0a5f 0b74 0c88 006a 0d83 017d 0488  .j._.t...j...}..
+00005540: 006a 09a0 0e7c 04a1 0101 0064 0053 0074  .j...|.....d.S.t
+00005550: 026a 036a 0464 0564 0664 0764 0064 0867  .j.j.d.d.d.d.d.g
+00005560: 0164 098d 057d 0388 006a 05a0 067c 03a1  .d...}...j...|..
+00005570: 0101 0064 0053 0029 0a4e 7218 0100 0072  ...d.S.).Nr....r
+00005580: b200 0000 6301 0000 0000 0000 0000 0000  ....c...........
+00005590: 0002 0000 0004 0000 0053 0000 0072 b400  .........S...r..
+000055a0: 0000 722b 0000 0072 b500 0000 72b7 0000  ..r+...r....r...
+000055b0: 0072 2b00 0000 722b 0000 0072 2c00 0000  .r+...r+...r,...
+000055c0: 72ba 0000 00ba 0200 0072 bb00 0000 7a45  r........r....zE
+000055d0: 4564 6974 4173 5374 7269 6e67 5f56 6965  EditAsString_Vie
+000055e0: 772e 5f5f 696e 6974 5f5f 2e3c 6c6f 6361  w.__init__.<loca
+000055f0: 6c73 3e2e 6f6e 5f63 6c69 636b 5f44 6f6e  ls>.on_click_Don
+00005600: 652e 3c6c 6f63 616c 733e 2e3c 6c69 7374  e.<locals>.<list
+00005610: 636f 6d70 3e72 1100 0000 7268 0000 007a  comp>r....rh...z
+00005620: 5945 7272 6f72 3a20 0a54 6869 7320 696e  YError: .This in
+00005630: 206e 6f74 2061 206c 6567 616c 2042 6163   not a legal Bac
+00005640: 6b67 616d 6d6f 6e20 626f 6172 6420 7374  kgammon board st
+00005650: 7269 6e67 2e20 506c 6561 7365 2050 726f  ring. Please Pro
+00005660: 7669 6465 2061 206c 6567 616c 2062 6f61  vide a legal boa
+00005670: 7264 2073 7472 696e 672e 729c 0000 0072  rd string.r....r
+00005680: 9d00 0000 290f 720a 0000 0072 bd00 0000  ....).r....r....
+00005690: 723d 0000 0072 4400 0000 72ac 0000 0072  r=...rD...r....r
+000056a0: 4600 0000 724a 0000 0072 0300 0000 72de  F...rJ...r....r.
+000056b0: 0000 0072 2000 0000 7221 0000 0072 d300  ...r ...r!...r..
+000056c0: 0000 72c0 0000 0072 2500 0000 7226 0000  ..r....r%...r&..
+000056d0: 0029 0572 2700 0000 da0a 7374 7269 6e67  .).r'.....string
+000056e0: 4c69 7374 5a07 6e75 6d4c 6973 7472 ae00  ListZ.numListr..
+000056f0: 0000 72ee 0000 00a9 0272 2a00 0000 5a0a  ..r......r*...Z.
+00005700: 7465 7874 5f69 6e70 7574 722b 0000 0072  text_inputr+...r
+00005710: 2c00 0000 72df 0000 00b4 0200 0073 2400  ,...r........s$.
+00005720: 0000 0e03 0202 1201 0601 0a01 0201 0601  ................
+00005730: 06fe 0e03 0a02 0a01 0a01 1001 0a02 0201  ................
+00005740: 0601 06fe 1003 7a31 4564 6974 4173 5374  ......z1EditAsSt
+00005750: 7269 6e67 5f56 6965 772e 5f5f 696e 6974  ring_View.__init
+00005760: 5f5f 2e3c 6c6f 6361 6c73 3e2e 6f6e 5f63  __.<locals>.on_c
+00005770: 6c69 636b 5f44 6f6e 6529 1072 4200 0000  lick_Done).rB...
+00005780: 7243 0000 0072 2500 0000 723d 0000 0072  rC...r%...r=...r
+00005790: 4400 0000 7245 0000 0072 4600 0000 7247  D...rE...rF...rG
+000057a0: 0000 0072 2000 0000 7221 0000 0072 d300  ...r ...r!...r..
+000057b0: 0000 da04 6a6f 696e 724c 0000 0072 8800  ....joinrL...r..
+000057c0: 0000 724a 0000 0072 2700 0000 2906 722a  ..rJ...r'...).r*
+000057d0: 0000 0072 2500 0000 721b 0100 00da 0673  ...r%...r......s
+000057e0: 7472 696e 6772 f400 0000 72df 0000 0072  tringr....r....r
+000057f0: 4f00 0000 721c 0100 0072 2c00 0000 7243  O...r....r,...rC
+00005800: 0000 00a4 0200 0073 1800 0000 0a01 0601  .......s........
+00005810: 0c02 0a01 1402 0a01 1402 1401 0c02 0c01  ................
+00005820: 0802 1401 7a1a 4564 6974 4173 5374 7269  ....z.EditAsStri
+00005830: 6e67 5f56 6965 772e 5f5f 696e 6974 5f5f  ng_View.__init__
+00005840: 6301 0000 0000 0000 0000 0000 0001 0000  c...............
+00005850: 0003 0000 0043 0000 0072 5100 0000 7231  .....C...rQ...r1
+00005860: 0000 0072 5200 0000 7229 0000 0072 2b00  ...rR...r)...r+.
+00005870: 0000 722b 0000 0072 2c00 0000 7254 0000  ..r+...r,...rT..
+00005880: 00cb 0200 0072 5500 0000 7a1e 4564 6974  .....rU...z.Edit
+00005890: 4173 5374 7269 6e67 5f56 6965 772e 6f6e  AsString_View.on
+000058a0: 5f73 686f 775f 7669 6577 6301 0000 0000  _show_viewc.....
+000058b0: 0000 0000 0000 0001 0000 0002 0000 0043  ...............C
+000058c0: 0000 0072 5600 0000 7231 0000 0072 5700  ...rV...r1...rW.
+000058d0: 0000 7229 0000 0072 2b00 0000 722b 0000  ..r)...r+...r+..
+000058e0: 0072 2c00 0000 7259 0000 00cf 0200 0072  .r,...rY.......r
+000058f0: 5a00 0000 7a1e 4564 6974 4173 5374 7269  Z...z.EditAsStri
+00005900: 6e67 5f56 6965 772e 6f6e 5f68 6964 655f  ng_View.on_hide_
+00005910: 7669 6577 6301 0000 0000 0000 0000 0000  viewc...........
+00005920: 0001 0000 0008 0000 0043 0000 0073 4000  .........C...s@.
+00005930: 0000 7c00 a000 a100 0100 7401 a002 6401  ..|.......t...d.
+00005940: 6402 6401 6403 7403 6a04 a105 0100 7401  d.d.d.t.j.....t.
+00005950: a005 6401 6402 6401 6403 7403 6a04 6404  ..d.d.d.d.t.j.d.
+00005960: a106 0100 7c00 6a06 a007 a100 0100 6400  ....|.j.......d.
+00005970: 5300 2905 4e72 1a01 0000 e990 0100 0072  S.).Nr.........r
+00005980: 7200 0000 7203 0100 0029 0872 5d00 0000  r...r....).r]...
+00005990: 723d 0000 00da 1564 7261 775f 7265 6374  r=.....draw_rect
+000059a0: 616e 676c 655f 6669 6c6c 6564 7204 0000  angle_filledr...
+000059b0: 00da 0b62 6f61 7264 5f63 6f6c 6f72 da16  ...board_color..
+000059c0: 6472 6177 5f72 6563 7461 6e67 6c65 5f6f  draw_rectangle_o
+000059d0: 7574 6c69 6e65 7246 0000 0072 5e00 0000  utlinerF...r^...
+000059e0: 7229 0000 0072 2b00 0000 722b 0000 0072  r)...r+...r+...r
+000059f0: 2c00 0000 725f 0000 00d2 0200 0073 0800  ,...r_.......s..
+00005a00: 0000 0801 1401 1601 0e02 7a19 4564 6974  ..........z.Edit
+00005a10: 4173 5374 7269 6e67 5f56 6965 772e 6f6e  AsString_View.on
+00005a20: 5f64 7261 7772 6100 0000 722b 0000 0072  _drawra...r+...r
+00005a30: 2b00 0000 724f 0000 0072 2c00 0000 72ed  +...rO...r,...r.
+00005a40: 0000 00a2 0200 0073 0a00 0000 0800 0c02  .......s........
+00005a50: 0827 0804 1003 72ed 0000 0063 0000 0000  .'....r....c....
+00005a60: 0000 0000 0000 0000 0000 0000 0300 0000  ................
+00005a70: 0000 0000 7205 0000 0029 0972 2e00 0000  ....r....).r....
+00005a80: 6302 0000 0000 0000 0000 0000 000a 0000  c...............
+00005a90: 0007 0000 0003 0000 00f3 fe00 0000 7400  ..............t.
+00005aa0: 8300 a001 a100 0100 7c01 8800 5f02 7403  ........|..._.t.
+00005ab0: 6a04 a005 a100 8800 5f06 8800 6a06 a007  j......._...j...
+00005ac0: a100 0100 7403 6a04 a008 6401 6402 6403  ....t.j...d.d.d.
+00005ad0: 6404 6405 a105 7d02 7403 6a04 a008 6401  d.d...}.t.j...d.
+00005ae0: 6406 6403 6404 6407 a105 7d03 7403 6a04  d.d.d.d...}.t.j.
+00005af0: a008 6408 6409 640a 640b 640c a105 7d04  ..d.d.d.d.d...}.
+00005b00: 7403 6a04 a008 640d 6409 640a 640b 640e  t.j...d.d.d.d.d.
+00005b10: a105 7d05 8800 6a06 a009 7c02 a101 0100  ..}...j...|.....
+00005b20: 8800 6a06 a009 7c03 a101 0100 8800 6a06  ..j...|.......j.
+00005b30: a009 7c04 a101 0100 8800 6a06 a009 7c05  ..|.......j...|.
+00005b40: a101 0100 7c02 a00a 640f a101 8700 6601  ....|...d.....f.
+00005b50: 6410 6411 8408 8301 7d06 7c03 a00a 640f  d.d.....}.|...d.
+00005b60: a101 6412 6413 8400 8301 7d07 7c04 a00a  ..d.d.....}.|...
+00005b70: 640f a101 8700 6601 6414 6415 8408 8301  d.....f.d.d.....
+00005b80: 7d08 7c05 a00a 640f a101 8700 6601 6416  }.|...d.....f.d.
+00005b90: 6417 8408 8301 7d09 6400 5300 2918 4e72  d.....}.d.S.).Nr
+00005ba0: 6d00 0000 726e 0000 0072 0800 0000 7210  m...rn...r....r.
+00005bb0: 0000 0072 6f00 0000 7270 0000 0072 1400  ...ro...rp...r..
+00005bc0: 0000 721f 0100 0072 1901 0000 e97d 0000  ..r....r.....}..
+00005bd0: 0072 7200 0000 da04 526f 6c6c e9bc 0200  .rr.....Roll....
+00005be0: 0072 1300 0000 721b 0000 0063 0100 0000  .r....r....c....
+00005bf0: 0000 0000 0000 0000 0200 0000 0300 0000  ................
+00005c00: 1300 0000 7292 0000 0072 3100 0000 7293  ....r....r1...r.
+00005c10: 0000 00a9 0272 2700 0000 5a0c 6d61 696e  .....r'...Z.main
+00005c20: 6d65 6e75 5669 6577 7229 0000 0072 2b00  menuViewr)...r+.
+00005c30: 0000 722c 0000 00da 0d6f 6e5f 636c 6963  ..r,.....on_clic
+00005c40: 6b5f 6261 636b ee02 0000 7294 0000 007a  k_back....r....z
+00005c50: 2d53 7461 7274 5f31 505f 5669 6577 2e5f  -Start_1P_View._
+00005c60: 5f69 6e69 745f 5f2e 3c6c 6f63 616c 733e  _init__.<locals>
+00005c70: 2e6f 6e5f 636c 6963 6b5f 6261 636b 6301  .on_click_backc.
+00005c80: 0000 0000 0000 0000 0000 0001 0000 0002  ................
+00005c90: 0000 0053 0000 0072 3b00 0000 7231 0000  ...S...r;...r1..
+00005ca0: 0072 3c00 0000 723f 0000 0072 2b00 0000  .r<...r?...r+...
+00005cb0: 722b 0000 0072 2c00 0000 7240 0000 00f3  r+...r,...r@....
+00005cc0: 0200 0072 4100 0000 7a2d 5374 6172 745f  ...rA...z-Start_
+00005cd0: 3150 5f56 6965 772e 5f5f 696e 6974 5f5f  1P_View.__init__
+00005ce0: 2e3c 6c6f 6361 6c73 3e2e 6f6e 5f63 6c69  .<locals>.on_cli
+00005cf0: 636b 5f51 7569 7463 0100 0000 0000 0000  ck_Quitc........
+00005d00: 0000 0000 0500 0000 0700 0000 1300 0000  ................
+00005d10: 73f4 0000 0074 00a0 0164 0164 02a1 027d  s....t...d.d...}
+00005d20: 017c 0164 016b 0272 3374 026a 0364 0164  .|.d.k.r3t.j.d.d
+00005d30: 0364 0464 058d 0388 006a 045f 0588 006a  .d.d.....j._...j
+00005d40: 046a 05a0 0688 006a 046a 07a1 0101 0088  .j.....j.j......
+00005d50: 006a 046a 05a0 0888 006a 046a 07a1 0101  .j.j.....j.j....
+00005d60: 0074 0988 006a 0a83 017d 0288 006a 04a0  .t...j...}...j..
+00005d70: 0b7c 02a1 0101 0064 0053 0074 026a 0364  .|.....d.S.t.j.d
+00005d80: 0288 006a 046a 0c64 0619 0064 0464 058d  ...j.j.d...d.d..
+00005d90: 0388 006a 045f 0588 006a 046a 056a 0d7d  ...j._...j.j.j.}
+00005da0: 0388 006a 046a 05a0 0e88 006a 046a 07a1  ...j.j.....j.j..
+00005db0: 0101 0074 0fa0 1088 006a 046a 0788 006a  ...t.....j.j...j
+00005dc0: 046a 0588 006a 046a 0c64 0619 0088 006a  .j...j.j.d.....j
+00005dd0: 046a 0c64 0719 00a1 047d 0488 006a 046a  .j.d.....}...j.j
+00005de0: 07a0 117c 0464 0264 04a1 0301 0074 1288  ...|.d.d.....t..
+00005df0: 006a 0a7c 0383 027d 0288 006a 04a0 0b7c  .j.|...}...j...|
+00005e00: 02a1 0101 0064 0053 0029 084e 7297 0000  .....d.S.).Nr...
+00005e10: 0072 9800 0000 721d 0000 0054 7299 0000  .r....r....Tr...
+00005e20: 0072 1f00 0000 7279 0000 0029 1372 a400  .r....ry...).r..
+00005e30: 0000 72a5 0000 0072 0300 0000 72a6 0000  ..r....r....r...
+00005e40: 0072 2000 0000 72a7 0000 00da 1e75 7064  .r ...r......upd
+00005e50: 6174 6550 6f73 7369 626c 654d 6f76 6573  atePossibleMoves
+00005e60: 4875 6d61 6e46 6f72 6d61 7472 2100 0000  HumanFormatr!...
+00005e70: da0e 666f 726d 5370 7269 7465 4c69 7374  ..formSpriteList
+00005e80: da0d 4875 6d61 6e5f 3150 5f56 6965 7772  ..Human_1P_Viewr
+00005e90: 2500 0000 7226 0000 0072 2300 0000 72bc  %...r&...r#...r.
+00005ea0: 0000 0072 a800 0000 7202 0000 0072 a900  ...r....r....r..
+00005eb0: 0000 72aa 0000 00da 1548 756d 616e 5f50  ..r......Human_P
+00005ec0: 7265 5475 726e 5f31 505f 5669 6577 2905  reTurn_1P_View).
+00005ed0: 7227 0000 00da 0b66 6972 7374 506c 6179  r'.....firstPlay
+00005ee0: 6572 da09 6e65 7874 5f76 6965 7772 bc00  er..next_viewr..
+00005ef0: 0000 72ad 0000 0072 2900 0000 722b 0000  ..r....r)...r+..
+00005f00: 0072 2c00 0000 da0d 6f6e 5f63 6c69 636b  .r,.....on_click
+00005f10: 5f72 6f6c 6cf7 0200 0073 1c00 0000 0c02  _roll....s......
+00005f20: 0802 1401 1201 1201 0a01 1001 1c02 0a01  ................
+00005f30: 1201 2801 1201 0c01 1001 7a2d 5374 6172  ..(.......z-Star
+00005f40: 745f 3150 5f56 6965 772e 5f5f 696e 6974  t_1P_View.__init
+00005f50: 5f5f 2e3c 6c6f 6361 6c73 3e2e 6f6e 5f63  __.<locals>.on_c
+00005f60: 6c69 636b 5f72 6f6c 6c63 0100 0000 0000  lick_rollc......
+00005f70: 0000 0000 0000 0200 0000 0300 0000 1300  ................
+00005f80: 0000 7234 0000 0072 3100 0000 7235 0000  ..r4...r1...r5..
+00005f90: 0072 3800 0000 7229 0000 0072 2b00 0000  .r8...r)...r+...
+00005fa0: 722c 0000 0072 3900 0000 0a03 0000 723a  r,...r9.......r:
+00005fb0: 0000 007a 3153 7461 7274 5f31 505f 5669  ...z1Start_1P_Vi
+00005fc0: 6577 2e5f 5f69 6e69 745f 5f2e 3c6c 6f63  ew.__init__.<loc
+00005fd0: 616c 733e 2e6f 6e5f 636c 6963 6b5f 5365  als>.on_click_Se
+00005fe0: 7474 696e 6773 a90b 7242 0000 0072 4300  ttings..rB...rC.
+00005ff0: 0000 7225 0000 0072 3d00 0000 7244 0000  ..r%...r=...rD..
+00006000: 0072 4500 0000 7246 0000 0072 4700 0000  .rE...rF...rG...
+00006010: 724c 0000 0072 4a00 0000 7227 0000 00a9  rL...rJ...r'....
+00006020: 0a72 2a00 0000 7225 0000 0072 8900 0000  .r*...r%...r....
+00006030: 728a 0000 00da 0b52 6f6c 6c5f 6275 7474  r......Roll_butt
+00006040: 6f6e da0f 5365 7474 696e 6773 5f62 7574  on..Settings_but
+00006050: 746f 6e72 2801 0000 7240 0000 0072 2f01  tonr(...r@...r/.
+00006060: 0000 7239 0000 0072 4f00 0000 7229 0000  ..r9...rO...r)..
+00006070: 0072 2c00 0000 7243 0000 00dd 0200 0073  .r,...rC.......s
+00006080: 2800 0000 0a01 0601 0c02 0a01 1402 1401  (...............
+00006090: 1401 1401 0c02 0c01 0c01 0c01 0802 0e01  ................
+000060a0: 0804 0a01 0803 0e01 0812 1201 7a16 5374  ............z.St
+000060b0: 6172 745f 3150 5f56 6965 772e 5f5f 696e  art_1P_View.__in
+000060c0: 6974 5f5f 6301 0000 0000 0000 0000 0000  it__c...........
+000060d0: 0001 0000 0003 0000 0043 0000 0072 5100  .........C...rQ.
+000060e0: 0000 7231 0000 0072 5200 0000 7229 0000  ..r1...rR...r)..
+000060f0: 0072 2b00 0000 722b 0000 0072 2c00 0000  .r+...r+...r,...
+00006100: 7254 0000 0010 0300 0072 5500 0000 7a1a  rT.......rU...z.
+00006110: 5374 6172 745f 3150 5f56 6965 772e 6f6e  Start_1P_View.on
+00006120: 5f73 686f 775f 7669 6577 6301 0000 0000  _show_viewc.....
+00006130: 0000 0000 0000 0001 0000 0002 0000 0043  ...............C
+00006140: 0000 0072 5600 0000 7231 0000 0072 5700  ...rV...r1...rW.
+00006150: 0000 7229 0000 0072 2b00 0000 722b 0000  ..r)...r+...r+..
+00006160: 0072 2c00 0000 7259 0000 0014 0300 0072  .r,...rY.......r
+00006170: 5a00 0000 7a1a 5374 6172 745f 3150 5f56  Z...z.Start_1P_V
+00006180: 6965 772e 6f6e 5f68 6964 655f 7669 6577  iew.on_hide_view
+00006190: 6301 0000 0000 0000 0000 0000 0001 0000  c...............
+000061a0: 0004 0000 0043 0000 00f3 3600 0000 7c00  .....C....6...|.
+000061b0: a000 a100 0100 7401 a002 a100 0100 7401  ......t.......t.
+000061c0: a003 7c00 6a04 6a05 6a06 7c00 6a04 6a05  ..|.j.j.j.|.j.j.
+000061d0: 6a07 a102 0100 7c00 6a08 a009 a100 0100  j.....|.j.......
+000061e0: 6400 5300 7231 0000 00a9 0a72 5d00 0000  d.S.r1.....r]...
+000061f0: 7204 0000 0072 d100 0000 72d2 0000 0072  r....r....r....r
+00006200: 2000 0000 7221 0000 0072 d300 0000 72ab   ...r!...r....r.
+00006210: 0000 0072 4600 0000 725e 0000 0072 2900  ...rF...r^...r).
+00006220: 0000 722b 0000 0072 2b00 0000 722c 0000  ..r+...r+...r,..
+00006230: 0072 5f00 0000 1703 0000 f308 0000 0008  .r_.............
+00006240: 0108 0118 010e 017a 1553 7461 7274 5f31  .......z.Start_1
+00006250: 505f 5669 6577 2e6f 6e5f 6472 6177 7261  P_View.on_drawra
+00006260: 0000 0072 2b00 0000 722b 0000 0072 4f00  ...r+...r+...rO.
+00006270: 0000 722c 0000 0072 2e00 0000 db02 0000  ..r,...r........
+00006280: 730a 0000 0008 000c 0208 3308 0410 0372  s.........3....r
+00006290: 2e00 0000 6300 0000 0000 0000 0000 0000  ....c...........
+000062a0: 0000 0000 0008 0000 0000 0000 00f3 4e00  ..............N.
+000062b0: 0000 6500 5a01 6400 5a02 8700 6601 6401  ..e.Z.d.Z...f.d.
+000062c0: 6402 8408 5a03 6403 6404 8400 5a04 6405  d...Z.d.d...Z.d.
+000062d0: 6406 8400 5a05 6407 6408 8400 5a06 6409  d...Z.d.d...Z.d.
+000062e0: 6507 640a 6507 640b 6507 640c 6507 6608  e.d.e.d.e.d.e.f.
+000062f0: 640d 640e 8404 5a08 8700 0400 5a09 5300  d.d...Z.....Z.S.
+00006300: 290f 722b 0100 0063 0200 0000 0000 0000  ).r+...c........
+00006310: 0000 0000 0a00 0000 0700 0000 0300 0000  ................
+00006320: f304 0100 0074 0083 00a0 01a1 0001 007c  .....t.........|
+00006330: 0188 005f 0264 0188 005f 0374 046a 05a0  ..._.d..._.t.j..
+00006340: 06a1 0088 005f 0788 006a 07a0 08a1 0001  ....._...j......
+00006350: 0074 046a 05a0 0964 0264 0364 0464 0564  .t.j...d.d.d.d.d
+00006360: 06a1 057d 0274 046a 05a0 0964 0264 0764  ...}.t.j...d.d.d
+00006370: 0464 0564 08a1 057d 0374 046a 05a0 0964  .d.d...}.t.j...d
+00006380: 0964 0264 0a64 0564 0ba1 057d 0474 046a  .d.d.d.d...}.t.j
+00006390: 05a0 0964 0964 0c64 0a64 0564 0da1 057d  ...d.d.d.d.d...}
+000063a0: 0588 006a 07a0 0a7c 02a1 0101 0088 006a  ...j...|.......j
+000063b0: 07a0 0a7c 03a1 0101 0088 006a 07a0 0a7c  ...|.......j...|
+000063c0: 04a1 0101 0088 006a 07a0 0a7c 05a1 0101  .......j...|....
+000063d0: 007c 02a0 0b64 0ea1 0187 0066 0164 0f64  .|...d.....f.d.d
+000063e0: 1084 0883 017d 067c 03a0 0b64 0ea1 0164  .....}.|...d...d
+000063f0: 1164 1284 0083 017d 077c 04a0 0b64 0ea1  .d.....}.|...d..
+00006400: 0187 0066 0164 1364 1484 0883 017d 087c  ...f.d.d.....}.|
+00006410: 05a0 0b64 0ea1 0187 0066 0164 1564 1684  ...d.....f.d.d..
+00006420: 0883 017d 0964 0053 0029 174e 72a9 0000  ...}.d.S.).Nr...
+00006430: 0072 6d00 0000 726e 0000 0072 0800 0000  .rm...rn...r....
+00006440: 7210 0000 0072 8c00 0000 7270 0000 0072  r....r....rp...r
+00006450: 1400 0000 728e 0000 0072 8f00 0000 7213  ....r....r....r.
+00006460: 0000 0072 da00 0000 72d9 0000 0072 1b00  ...r....r....r..
+00006470: 0000 6301 0000 0000 0000 0000 0000 0002  ..c.............
+00006480: 0000 0003 0000 0013 0000 0072 9200 0000  ...........r....
+00006490: 7231 0000 0072 9300 0000 7227 0100 0072  r1...r....r'...r
+000064a0: 2900 0000 722b 0000 0072 2c00 0000 da0d  )...r+...r,.....
+000064b0: 6f6e 5f63 6c69 636b 5f65 7869 7434 0300  on_click_exit4..
+000064c0: 0072 9400 0000 7a2d 4875 6d61 6e5f 3150  .r....z-Human_1P
+000064d0: 5f56 6965 772e 5f5f 696e 6974 5f5f 2e3c  _View.__init__.<
+000064e0: 6c6f 6361 6c73 3e2e 6f6e 5f63 6c69 636b  locals>.on_click
+000064f0: 5f65 7869 7463 0100 0000 0000 0000 0000  _exitc..........
+00006500: 0000 0100 0000 0200 0000 5300 0000 723b  ..........S...r;
+00006510: 0000 0072 3100 0000 723c 0000 0072 3f00  ...r1...r<...r?.
+00006520: 0000 722b 0000 0072 2b00 0000 722c 0000  ..r+...r+...r,..
+00006530: 0072 4000 0000 3903 0000 7241 0000 007a  .r@...9...rA...z
+00006540: 2d48 756d 616e 5f31 505f 5669 6577 2e5f  -Human_1P_View._
+00006550: 5f69 6e69 745f 5f2e 3c6c 6f63 616c 733e  _init__.<locals>
+00006560: 2e6f 6e5f 636c 6963 6b5f 5175 6974 6301  .on_click_Quitc.
+00006570: 0000 0000 0000 0000 0000 0002 0000 0003  ................
+00006580: 0000 0013 0000 0072 3400 0000 7231 0000  .......r4...r1..
+00006590: 0072 3500 0000 7238 0000 0072 2900 0000  .r5...r8...r)...
+000065a0: 722b 0000 0072 2c00 0000 7239 0000 003d  r+...r,...r9...=
+000065b0: 0300 0072 3a00 0000 7a31 4875 6d61 6e5f  ...r:...z1Human_
+000065c0: 3150 5f56 6965 772e 5f5f 696e 6974 5f5f  1P_View.__init__
+000065d0: 2e3c 6c6f 6361 6c73 3e2e 6f6e 5f63 6c69  .<locals>.on_cli
+000065e0: 636b 5f53 6574 7469 6e67 7363 0100 0000  ck_Settingsc....
+000065f0: 0000 0000 0000 0000 0600 0000 0700 0000  ................
+00006600: 1300 0000 73e0 0000 0088 006a 006a 016a  ....s......j.j.j
+00006610: 0264 0119 0064 016b 0272 1d74 036a 046a  .d...d.k.r.t.j.j
+00006620: 0564 0264 0364 0464 0064 0567 0164 068d  .d.d.d.d.d.g.d..
+00006630: 057d 0188 006a 06a0 077c 01a1 0101 0064  .}...j...|.....d
+00006640: 0053 0074 08a0 0964 0788 006a 006a 0a64  .S.t...d...j.j.d
+00006650: 0819 00a1 0288 006a 005f 0b88 006a 006a  .......j._...j.j
+00006660: 0b6a 0c7d 0288 006a 006a 0ba0 0d88 006a  .j.}...j.j.....j
+00006670: 006a 01a1 0101 0074 0ea0 0f88 006a 006a  .j.....t.....j.j
+00006680: 0188 006a 006a 0b88 006a 006a 0a64 0819  ...j.j...j.j.d..
+00006690: 0088 006a 006a 0a64 0919 00a1 047d 0388  ...j.j.d.....}..
+000066a0: 006a 006a 01a0 107c 0364 0764 0aa1 0301  .j.j...|.d.d....
+000066b0: 0088 006a 006a 016a 0264 0b19 0064 016b  ...j.j.j.d...d.k
+000066c0: 0272 5f64 0a6e 0164 0c7d 0474 1188 006a  .r_d.n.d.}.t...j
+000066d0: 127c 027c 0483 037d 0588 006a 00a0 137c  .|.|...}...j...|
+000066e0: 05a1 0101 0064 0053 0029 0d4e 7201 0000  .....d.S.).Nr...
+000066f0: 0072 1100 0000 7268 0000 007a 3647 616d  .r....rh...z6Gam
+00006700: 6520 4f76 6572 3a20 0a59 6f75 2057 696e  e Over: .You Win
+00006710: 2120 0a0a 2045 7869 7420 746f 204d 6169  ! .. Exit to Mai
+00006720: 6e20 4d65 6e75 2046 6f72 204e 6577 2047  n Menu For New G
+00006730: 616d 6572 9c00 0000 729d 0000 0072 9800  amer....r....r..
+00006740: 0000 721f 0000 0072 7900 0000 5472 9700  ..r....ry...Tr..
+00006750: 0000 4629 1472 2000 0000 7221 0000 0072  ..F).r ...r!...r
+00006760: ab00 0000 723d 0000 0072 4400 0000 72ac  ....r=...rD...r.
+00006770: 0000 0072 4600 0000 724a 0000 0072 0300  ...rF...rJ...r..
+00006780: 0000 72a6 0000 0072 2300 0000 72a7 0000  ..r....r#...r...
+00006790: 0072 bc00 0000 72a8 0000 0072 0200 0000  .r....r....r....
+000067a0: 72a9 0000 0072 aa00 0000 722c 0100 0072  r....r....r,...r
+000067b0: 2500 0000 7226 0000 0029 0672 2700 0000  %...r&...).r'...
+000067c0: 72ae 0000 0072 bc00 0000 72ad 0000 00da  r....r....r.....
+000067d0: 0661 695f 7769 6e72 2e01 0000 7229 0000  .ai_winr....r)..
+000067e0: 0072 2b00 0000 722c 0000 00da 0d6f 6e5f  .r+...r,.....on_
+000067f0: 636c 6963 6b5f 646f 6e65 4303 0000 7318  click_doneC...s.
+00006800: 0000 0012 0318 010c 0104 0218 020a 0112  ................
+00006810: 0128 0112 011a 010e 0210 017a 2d48 756d  .(.........z-Hum
+00006820: 616e 5f31 505f 5669 6577 2e5f 5f69 6e69  an_1P_View.__ini
+00006830: 745f 5f2e 3c6c 6f63 616c 733e 2e6f 6e5f  t__.<locals>.on_
+00006840: 636c 6963 6b5f 646f 6e65 a90c 7242 0000  click_done..rB..
+00006850: 0072 4300 0000 7225 0000 00da 0473 7465  .rC...r%.....ste
+00006860: 7072 3d00 0000 7244 0000 0072 4500 0000  pr=...rD...rE...
+00006870: 7246 0000 0072 4700 0000 724c 0000 0072  rF...rG...rL...r
+00006880: 4a00 0000 7227 0000 00a9 0a72 2a00 0000  J...r'.....r*...
+00006890: 7225 0000 00da 0b45 7869 745f 6275 7474  r%.....Exit_butt
+000068a0: 6f6e 728a 0000 0072 3301 0000 72f4 0000  onr....r3...r...
+000068b0: 0072 3901 0000 7240 0000 0072 3900 0000  .r9...r@...r9...
+000068c0: 723b 0100 0072 4f00 0000 7229 0000 0072  r;...rO...r)...r
+000068d0: 2c00 0000 7243 0000 0020 0300 00f3 2a00  ,...rC... ....*.
+000068e0: 0000 0a01 0601 0602 0c02 0a01 1402 1401  ................
+000068f0: 1401 1402 0c02 0c01 0c01 0c01 0802 0e01  ................
+00006900: 0804 0a01 0803 0e01 0805 1201 7a16 4875  ............z.Hu
+00006910: 6d61 6e5f 3150 5f56 6965 772e 5f5f 696e  man_1P_View.__in
+00006920: 6974 5f5f 6301 0000 0000 0000 0000 0000  it__c...........
+00006930: 0001 0000 0003 0000 0043 0000 0072 5100  .........C...rQ.
+00006940: 0000 7231 0000 0072 5200 0000 7229 0000  ..r1...rR...r)..
+00006950: 0072 2b00 0000 722b 0000 0072 2c00 0000  .r+...r+...r,...
+00006960: 7254 0000 0056 0300 0072 5500 0000 7a1a  rT...V...rU...z.
+00006970: 4875 6d61 6e5f 3150 5f56 6965 772e 6f6e  Human_1P_View.on
+00006980: 5f73 686f 775f 7669 6577 6301 0000 0000  _show_viewc.....
+00006990: 0000 0000 0000 0001 0000 0002 0000 0043  ...............C
+000069a0: 0000 0072 5600 0000 7231 0000 0072 5700  ...rV...r1...rW.
+000069b0: 0000 7229 0000 0072 2b00 0000 722b 0000  ..r)...r+...r+..
+000069c0: 0072 2c00 0000 7259 0000 005a 0300 0072  .r,...rY...Z...r
+000069d0: 5a00 0000 7a1a 4875 6d61 6e5f 3150 5f56  Z...z.Human_1P_V
+000069e0: 6965 772e 6f6e 5f68 6964 655f 7669 6577  iew.on_hide_view
+000069f0: 6301 0000 0000 0000 0000 0000 0001 0000  c...............
+00006a00: 0007 0000 0043 0000 0073 b400 0000 7c00  .....C...s....|.
+00006a10: a000 a100 0100 7401 a002 a100 0100 7403  ......t.......t.
+00006a20: a004 6401 6402 6403 6404 7401 6a05 a105  ..d.d.d.d.t.j...
+00006a30: 0100 7401 a006 7c00 6a07 6a08 6a09 7c00  ..t...|.j.j.j.|.
+00006a40: 6a07 6a08 6a0a a102 0100 7401 a00b 7c00  j.j.j.....t...|.
+00006a50: 6a07 6a0c 6a0d 6405 1900 7c00 6a07 6a0c  j.j.j.d...|.j.j.
+00006a60: 6a0d 6406 1900 7c00 6a07 6a0c 6a0e a103  j.d...|.j.j.j...
+00006a70: 0100 7c00 6a0f 6407 6b02 723f 7401 a010  ..|.j.d.k.r?t...
+00006a80: 7c00 6a07 6a0c 6a11 a101 6e13 7401 a012  |.j.j.j...n.t...
+00006a90: 7c00 6a07 6a0c 6a13 7c00 6a07 6a0c 6a14  |.j.j.j.|.j.j.j.
+00006aa0: a102 0100 7c00 6a15 a016 a100 0100 6400  ....|.j.......d.
+00006ab0: 5300 0100 7c00 6a15 a016 a100 0100 6400  S...|.j.......d.
+00006ac0: 5300 a908 4ee9 5902 0000 e991 0100 0072  S...N.Y........r
+00006ad0: 0b01 0000 e9fa 0200 0072 0100 0000 7297  .........r....r.
+00006ae0: 0000 0072 a900 0000 2917 725d 0000 0072  ...r....).r]...r
+00006af0: 0400 0000 72d1 0000 0072 3d00 0000 7220  ....r....r=...r 
+00006b00: 0100 00da 1064 6172 6b43 6865 636b 6572  .....darkChecker
+00006b10: 436f 6c6f 7272 d200 0000 7220 0000 0072  Colorr....r ...r
+00006b20: 2100 0000 72d3 0000 0072 ab00 0000 72d7  !...r....r....r.
+00006b30: 0000 0072 a700 0000 72bc 0000 0072 d800  ...r....r....r..
+00006b40: 0000 723d 0100 00da 0c64 7261 7754 7572  ..r=.....drawTur
+00006b50: 6e4d 6169 6eda 1273 7072 6974 6573 5f6d  nMain..sprites_m
+00006b60: 6f76 655f 7374 6172 74da 0e64 7261 7754  ove_start..drawT
+00006b70: 7572 6e42 7261 6e63 68da 0d73 7072 6974  urnBranch..sprit
+00006b80: 655f 6163 7469 7665 da10 7370 7269 7465  e_active..sprite
+00006b90: 735f 6d6f 7665 5f65 6e64 7246 0000 0072  s_move_endrF...r
+00006ba0: 5e00 0000 7229 0000 0072 2b00 0000 722b  ^...r)...r+...r+
+00006bb0: 0000 0072 2c00 0000 725f 0000 005d 0300  ...r,...r_...]..
+00006bc0: 0073 1e00 0000 0801 0801 1401 1801 2801  .s............(.
+00006bd0: 0802 06ff 0801 04ff 0401 1001 04ff 0e02  ................
+00006be0: 02fd 0e03 7a15 4875 6d61 6e5f 3150 5f56  ....z.Human_1P_V
+00006bf0: 6965 772e 6f6e 5f64 7261 7772 f500 0000  iew.on_drawr....
+00006c00: 72f6 0000 0072 f700 0000 72f8 0000 0063  r....r....r....c
+00006c10: 0500 0000 0000 0000 0000 0000 0700 0000  ................
+00006c20: 0600 0000 4300 0000 f354 0100 007c 006a  ....C....T...|.j
+00006c30: 0064 016b 0272 3074 01a0 027c 017c 0266  .d.k.r0t...|.|.f
+00006c40: 027c 006a 036a 046a 05a1 027d 057c 0567  .|.j.j.j...}.|.g
+00006c50: 006b 0372 2e7c 0564 0219 007c 006a 036a  .k.r.|.d...|.j.j
+00006c60: 045f 0674 07a0 087c 006a 036a 046a 067c  ._.t...|.j.j.j.|
+00006c70: 006a 036a 09a1 027c 006a 036a 045f 0a64  .j.j...|.j.j._.d
+00006c80: 037c 005f 0064 0053 0064 0053 007c 006a  .|._.d.S.d.S.|.j
+00006c90: 0064 036b 0272 a664 017c 005f 0074 01a0  .d.k.r.d.|._.t..
+00006ca0: 027c 017c 0266 027c 006a 036a 046a 0aa1  .|.|.f.|.j.j.j..
+00006cb0: 027d 057c 0567 006b 0372 a87c 006a 036a  .}.|.g.k.r.|.j.j
+00006cc0: 09a0 0b7c 006a 036a 046a 066a 0c64 0219  ...|.j.j.j.j.d..
+00006cd0: 007c 0564 0219 006a 0d66 0264 04a1 0201  .|.d...j.f.d....
+00006ce0: 007c 006a 036a 096a 0e64 0219 0064 026b  .|.j.j.j.d...d.k
+00006cf0: 0272 6409 0074 0fa0 107c 006a 036a 046a  .rd..t...|.j.j.j
+00006d00: 066a 0c64 0219 007c 0564 0219 006a 0d7c  .j.d...|.d...j.|
+00006d10: 006a 036a 046a 1164 04a1 047d 067c 006a  .j.j.j.d...}.|.j
+00006d20: 036a 046a 11a0 127c 06a1 0101 0074 137c  .j.j...|.....t.|
+00006d30: 006a 036a 046a 1183 0164 026b 0472 9d7c  .j.j.j...d.k.r.|
+00006d40: 006a 036a 04a0 147c 006a 036a 09a1 0101  .j.j...|.j.j....
+00006d50: 007c 006a 036a 04a0 157c 006a 036a 09a1  .|.j.j...|.j.j..
+00006d60: 0101 0064 0053 0074 01a0 16a1 007c 006a  ...d.S.t.....|.j
+00006d70: 036a 045f 0564 0053 0064 0053 0064 0053  .j._.d.S.d.S.d.S
+00006d80: 00a9 054e 72a9 0000 0072 0100 0000 da06  ...Nr....r......
+00006d90: 4272 616e 6368 7297 0000 00a9 1772 3d01  Branchr......r=.
+00006da0: 0000 723d 0000 00da 1467 6574 5f73 7072  ..r=.....get_spr
+00006db0: 6974 6573 5f61 745f 706f 696e 7472 2000  ites_at_pointr .
+00006dc0: 0000 72a7 0000 0072 4701 0000 7249 0100  ..r....rG...rI..
+00006dd0: 0072 0400 0000 da14 6372 6561 7465 4d6f  .r......createMo
+00006de0: 7665 456e 6453 7072 6974 6573 7221 0000  veEndSpritesr!..
+00006df0: 0072 4a01 0000 da08 6d61 6b65 4d6f 7665  .rJ.....makeMove
+00006e00: da04 6d6f 7665 da03 706f 7372 ab00 0000  ..move..posr....
+00006e10: 7203 0000 00da 0d66 726f 6d4d 6f76 6554  r......fromMoveT
+00006e20: 6f44 6965 72d8 0000 00da 0672 656d 6f76  oDier......remov
+00006e30: 65da 036c 656e 7229 0100 0072 2a01 0000  e..lenr)...r*...
+00006e40: da0a 5370 7269 7465 4c69 7374 a907 722a  ..SpriteList..r*
+00006e50: 0000 0072 f500 0000 72f6 0000 0072 f700  ...r....r....r..
+00006e60: 0000 72f8 0000 005a 0e63 6c69 636b 6564  ..r....Z.clicked
+00006e70: 5f73 7072 6974 6572 bc00 0000 722b 0000  _spriter....r+..
+00006e80: 0072 2b00 0000 722c 0000 0072 1501 0000  .r+...r,...r....
+00006e90: 6803 0000 f334 0000 000a 0116 0108 010e  h....4..........
+00006ea0: 0104 010e 010a ff0a 0204 fc0a 0606 0116  ................
+00006eb0: 0208 0126 0112 0102 011a 020a 0104 ff10  ...&............
+00006ec0: 0212 0112 0116 0112 0204 f004 047a 1c48  .............z.H
+00006ed0: 756d 616e 5f31 505f 5669 6577 2e6f 6e5f  uman_1P_View.on_
+00006ee0: 6d6f 7573 655f 7072 6573 73a9 0a72 6200  mouse_press..rb.
+00006ef0: 0000 7263 0000 0072 6400 0000 7243 0000  ..rc...rd...rC..
+00006f00: 0072 5400 0000 7259 0000 0072 5f00 0000  .rT...rY...r_...
+00006f10: 72b6 0000 0072 1501 0000 7265 0000 0072  r....r....re...r
+00006f20: 2b00 0000 722b 0000 0072 4f00 0000 722c  +...r+...rO...r,
+00006f30: 0000 0072 2b01 0000 1e03 0000 730c 0000  ...r+.......s...
+00006f40: 0008 000c 0208 3608 0408 0322 0b72 2b01  ......6....".r+.
+00006f50: 0000 6300 0000 0000 0000 0000 0000 0000  ..c.............
+00006f60: 0000 0004 0000 0000 0000 0073 3600 0000  ...........s6...
+00006f70: 6500 5a01 6400 5a02 640a 8700 6601 6402  e.Z.d.Z.d...f.d.
+00006f80: 6403 8409 5a03 6404 6405 8400 5a04 6406  d...Z.d.d...Z.d.
+00006f90: 6407 8400 5a05 6408 6409 8400 5a06 8700  d...Z.d.d...Z...
+00006fa0: 0400 5a07 5300 290b 722c 0100 0046 6304  ..Z.S.).r,...Fc.
+00006fb0: 0000 0000 0000 0000 0000 000d 0000 000a  ................
+00006fc0: 0000 0003 0000 0073 3201 0000 7400 8300  .......s2...t...
+00006fd0: a001 a100 0100 7c01 8800 5f02 7c03 8800  ......|..._.|...
+00006fe0: 5f03 7404 6a05 a006 a100 8800 5f07 8800  _.t.j......._...
+00006ff0: 6a07 a008 a100 0100 7404 6a05 a009 6401  j.......t.j...d.
+00007000: 6402 6403 6404 6405 a105 7d04 7404 6a05  d.d.d.d...}.t.j.
+00007010: a009 6401 6406 6403 6404 6407 a105 7d05  ..d.d.d.d.d...}.
+00007020: 7404 6a05 a009 6408 6401 6409 6404 640a  t.j...d.d.d.d.d.
+00007030: a105 7d06 7404 6a05 a009 6408 640b 6409  ..}.t.j...d.d.d.
+00007040: 6404 640c a105 7d07 7404 6a05 6a0a 6408  d.d...}.t.j.j.d.
+00007050: 640d 6409 6404 640e 7c02 9b00 9d02 6401  d.d.d.d.|.....d.
+00007060: 640f 6410 6411 8d08 7d08 8800 6a07 a00b  d.d.d...}...j...
+00007070: 7c04 a101 0100 8800 6a07 a00b 7c05 a101  |.......j...|...
+00007080: 0100 8800 6a07 a00b 7c06 a101 0100 8800  ....j...|.......
+00007090: 6a07 a00b 7c07 a101 0100 8800 6a07 a00b  j...|.......j...
+000070a0: 7c08 a101 0100 7c04 a00c 6412 a101 8700  |.....|...d.....
+000070b0: 6601 6413 6414 8408 8301 7d09 7c05 a00c  f.d.d.....}.|...
+000070c0: 6412 a101 6415 6416 8400 8301 7d0a 7c06  d...d.d.....}.|.
+000070d0: a00c 6412 a101 8700 6601 6417 6418 8408  ..d.....f.d.d...
+000070e0: 8301 7d0b 7c07 a00c 6412 a101 8700 6601  ..}.|...d.....f.
+000070f0: 6419 641a 8408 8301 7d0c 6400 5300 291b  d.d.....}.d.S.).
+00007100: 4e72 6d00 0000 726e 0000 0072 0800 0000  Nrm...rn...r....
+00007110: 7210 0000 0072 8c00 0000 7270 0000 0072  r....r....rp...r
+00007120: 1400 0000 728e 0000 0072 8f00 0000 7213  ....r....r....r.
+00007130: 0000 0072 1f01 0000 7225 0100 0072 0e01  ...r....r%...r..
+00007140: 0000 7a0a 4149 2052 6f6c 6c65 6420 7216  ..z.AI Rolled r.
+00007150: 0000 0054 7269 0000 0072 1b00 0000 6301  ...Tri...r....c.
+00007160: 0000 0000 0000 0000 0000 0002 0000 0003  ................
+00007170: 0000 0013 0000 0072 9200 0000 7231 0000  .......r....r1..
+00007180: 0072 9300 0000 7227 0100 0072 2900 0000  .r....r'...r)...
+00007190: 722b 0000 0072 2c00 0000 7239 0100 009c  r+...r,...r9....
+000071a0: 0300 0072 9400 0000 7a35 4875 6d61 6e5f  ...r....z5Human_
+000071b0: 5072 6554 7572 6e5f 3150 5f56 6965 772e  PreTurn_1P_View.
+000071c0: 5f5f 696e 6974 5f5f 2e3c 6c6f 6361 6c73  __init__.<locals
+000071d0: 3e2e 6f6e 5f63 6c69 636b 5f65 7869 7463  >.on_click_exitc
+000071e0: 0100 0000 0000 0000 0000 0000 0100 0000  ................
+000071f0: 0200 0000 5300 0000 723b 0000 0072 3100  ....S...r;...r1.
+00007200: 0000 723c 0000 0072 3f00 0000 722b 0000  ..r<...r?...r+..
+00007210: 0072 2b00 0000 722c 0000 0072 4000 0000  .r+...r,...r@...
+00007220: a103 0000 7241 0000 007a 3548 756d 616e  ....rA...z5Human
+00007230: 5f50 7265 5475 726e 5f31 505f 5669 6577  _PreTurn_1P_View
+00007240: 2e5f 5f69 6e69 745f 5f2e 3c6c 6f63 616c  .__init__.<local
+00007250: 733e 2e6f 6e5f 636c 6963 6b5f 5175 6974  s>.on_click_Quit
+00007260: 6301 0000 0000 0000 0000 0000 0002 0000  c...............
+00007270: 0003 0000 0013 0000 0072 3400 0000 7231  .........r4...r1
+00007280: 0000 0072 3500 0000 7238 0000 0072 2900  ...r5...r8...r).
+00007290: 0000 722b 0000 0072 2c00 0000 7239 0000  ..r+...r,...r9..
+000072a0: 00a5 0300 0072 3a00 0000 7a39 4875 6d61  .....r:...z9Huma
+000072b0: 6e5f 5072 6554 7572 6e5f 3150 5f56 6965  n_PreTurn_1P_Vie
+000072c0: 772e 5f5f 696e 6974 5f5f 2e3c 6c6f 6361  w.__init__.<loca
+000072d0: 6c73 3e2e 6f6e 5f63 6c69 636b 5f53 6574  ls>.on_click_Set
+000072e0: 7469 6e67 7363 0100 0000 0000 0000 0000  tingsc..........
+000072f0: 0000 0200 0000 0400 0000 1300 0000 734e  ..............sN
+00007300: 0000 0074 00a0 0164 0164 02a1 0288 006a  ...t...d.d.....j
+00007310: 025f 0388 006a 026a 03a0 0488 006a 026a  ._...j.j.....j.j
+00007320: 05a1 0101 0088 006a 026a 03a0 0688 006a  .......j.j.....j
+00007330: 026a 05a1 0101 0074 0788 006a 0883 017d  .j.....t...j...}
+00007340: 0188 006a 02a0 097c 01a1 0101 0064 0053  ...j...|.....d.S
+00007350: 0029 034e 7297 0000 0072 1d00 0000 290a  .).Nr....r....).
+00007360: 7203 0000 0072 a600 0000 7220 0000 0072  r....r....r ...r
+00007370: a700 0000 7229 0100 0072 2100 0000 722a  ....r)...r!...r*
+00007380: 0100 0072 2b01 0000 7225 0000 0072 2600  ...r+...r%...r&.
+00007390: 0000 2902 7227 0000 0072 2e01 0000 7229  ..).r'...r....r)
+000073a0: 0000 0072 2b00 0000 722c 0000 0072 2f01  ...r+...r,...r/.
+000073b0: 0000 ab03 0000 730a 0000 0010 0212 0112  ......s.........
+000073c0: 010a 0210 017a 3548 756d 616e 5f50 7265  .....z5Human_Pre
+000073d0: 5475 726e 5f31 505f 5669 6577 2e5f 5f69  Turn_1P_View.__i
+000073e0: 6e69 745f 5f2e 3c6c 6f63 616c 733e 2e6f  nit__.<locals>.o
+000073f0: 6e5f 636c 6963 6b5f 726f 6c6c 290d 7242  n_click_roll).rB
+00007400: 0000 0072 4300 0000 7225 0000 0072 3a01  ...rC...r%...r:.
+00007410: 0000 723d 0000 0072 4400 0000 7245 0000  ..r=...rD...rE..
+00007420: 0072 4600 0000 7247 0000 0072 4c00 0000  .rF...rG...rL...
+00007430: 7249 0000 0072 4a00 0000 7227 0000 0029  rI...rJ...r'...)
+00007440: 0d72 2a00 0000 7225 0000 005a 096c 6173  .r*...r%...Z.las
+00007450: 745f 726f 6c6c 723a 0100 0072 3f01 0000  t_rollr:...r?...
+00007460: 728a 0000 0072 3301 0000 7232 0100 005a  r....r3...r2...Z
+00007470: 0f6c 6173 745f 726f 6c6c 5f6c 6162 656c  .last_roll_label
+00007480: 7239 0100 0072 4000 0000 7239 0000 0072  r9...r@...r9...r
+00007490: 2f01 0000 724f 0000 0072 2900 0000 722c  /...rO...r)...r,
+000074a0: 0000 0072 4300 0000 8603 0000 732e 0000  ...rC.......s...
+000074b0: 000a 0106 0106 010c 020a 0114 0214 0114  ................
+000074c0: 0114 0222 020c 020c 010c 010c 010c 0108  ..."............
+000074d0: 020e 0108 040a 0108 030e 0108 0512 017a  ...............z
+000074e0: 1e48 756d 616e 5f50 7265 5475 726e 5f31  .Human_PreTurn_1
+000074f0: 505f 5669 6577 2e5f 5f69 6e69 745f 5f63  P_View.__init__c
+00007500: 0100 0000 0000 0000 0000 0000 0200 0000  ................
+00007510: 0700 0000 4300 0000 7344 0000 007c 006a  ....C...sD...|.j
+00007520: 00a0 01a1 0001 007c 006a 0272 1a74 036a  .......|.j.r.t.j
+00007530: 046a 0564 0164 0264 0364 0064 0467 0164  .j.d.d.d.d.d.g.d
+00007540: 058d 057d 017c 006a 00a0 067c 01a1 0101  ...}.|.j...|....
+00007550: 0074 03a0 077c 006a 08a1 0101 0064 0053  .t...|.j.....d.S
+00007560: 0029 064e 7211 0000 0072 6800 0000 7a37  .).Nr....rh...z7
+00007570: 4761 6d65 204f 7665 723a 200a 4149 2057  Game Over: .AI W
+00007580: 696e 7321 200a 200a 2045 7869 7420 746f  ins! . . Exit to
+00007590: 204d 6169 6e20 4d65 6e75 2046 6f72 204e   Main Menu For N
+000075a0: 6577 2047 616d 6572 9c00 0000 729d 0000  ew Gamer....r...
+000075b0: 0029 0972 4600 0000 7247 0000 0072 3a01  .).rF...rG...r:.
+000075c0: 0000 723d 0000 0072 4400 0000 72ac 0000  ..r=...rD...r...
+000075d0: 0072 4a00 0000 7253 0000 0072 2500 0000  .rJ...rS...r%...
+000075e0: 2902 722a 0000 0072 ae00 0000 722b 0000  ).r*...r....r+..
+000075f0: 0072 2b00 0000 722c 0000 0072 5400 0000  .r+...r,...rT...
+00007600: b403 0000 730a 0000 000a 0106 0218 010c  ....s...........
+00007610: 0110 027a 2248 756d 616e 5f50 7265 5475  ...z"Human_PreTu
+00007620: 726e 5f31 505f 5669 6577 2e6f 6e5f 7368  rn_1P_View.on_sh
+00007630: 6f77 5f76 6965 7763 0100 0000 0000 0000  ow_viewc........
+00007640: 0000 0000 0100 0000 0200 0000 4300 0000  ............C...
+00007650: 7256 0000 0072 3100 0000 7257 0000 0072  rV...r1...rW...r
+00007660: 2900 0000 722b 0000 0072 2b00 0000 722c  )...r+...r+...r,
+00007670: 0000 0072 5900 0000 bd03 0000 725a 0000  ...rY.......rZ..
+00007680: 007a 2248 756d 616e 5f50 7265 5475 726e  .z"Human_PreTurn
+00007690: 5f31 505f 5669 6577 2e6f 6e5f 6869 6465  _1P_View.on_hide
+000076a0: 5f76 6965 7763 0100 0000 0000 0000 0000  _viewc..........
+000076b0: 0000 0100 0000 0700 0000 4300 0000 7368  ..........C...sh
+000076c0: 0000 007c 00a0 00a1 0001 0074 01a0 02a1  ...|.......t....
+000076d0: 0001 0074 03a0 0464 0164 0264 0364 0474  ...t...d.d.d.d.t
+000076e0: 016a 05a1 0501 0074 01a0 067c 006a 076a  .j.....t...|.j.j
+000076f0: 086a 097c 006a 076a 086a 0aa1 0201 007c  .j.|.j.j.j.....|
+00007700: 006a 076a 086a 0b64 006b 0372 2d74 01a0  .j.j.j.d.k.r-t..
+00007710: 0c7c 006a 076a 086a 0ba1 0101 007c 006a  .|.j.j.j.....|.j
+00007720: 0da0 0ea1 0001 0064 0053 00a9 054e 7242  .......d.S...NrB
+00007730: 0100 0072 4301 0000 720b 0100 0072 4401  ...rC...r....rD.
+00007740: 0000 290f 725d 0000 0072 0400 0000 72d1  ..).r]...r....r.
+00007750: 0000 0072 3d00 0000 7220 0100 0072 4501  ...r=...r ...rE.
+00007760: 0000 72d2 0000 0072 2000 0000 7221 0000  ..r....r ...r!..
+00007770: 0072 d300 0000 72ab 0000 0072 d500 0000  .r....r....r....
+00007780: 72d6 0000 0072 4600 0000 725e 0000 0072  r....rF...r^...r
+00007790: 2900 0000 722b 0000 0072 2b00 0000 722c  )...r+...r+...r,
+000077a0: 0000 0072 5f00 0000 c003 0000 730e 0000  ...r_.......s...
+000077b0: 0008 0108 0114 0118 010e 0110 010e 017a  ...............z
+000077c0: 1d48 756d 616e 5f50 7265 5475 726e 5f31  .Human_PreTurn_1
+000077d0: 505f 5669 6577 2e6f 6e5f 6472 6177 2901  P_View.on_draw).
+000077e0: 4672 6100 0000 722b 0000 0072 2b00 0000  Fra...r+...r+...
+000077f0: 724f 0000 0072 2c00 0000 722c 0100 0084  rO...r,...r,....
+00007800: 0300 0073 0a00 0000 0800 0e02 082e 0809  ...s............
+00007810: 1003 722c 0100 0063 0000 0000 0000 0000  ..r,...c........
+00007820: 0000 0000 0000 0000 0300 0000 0000 0000  ................
+00007830: 7205 0000 0029 0972 3200 0000 6302 0000  r....).r2...c...
+00007840: 0000 0000 0000 0000 000a 0000 0007 0000  ................
+00007850: 0003 0000 0072 2301 0000 2918 4e72 6d00  .....r#...).Nrm.
+00007860: 0000 726e 0000 0072 0800 0000 7210 0000  ..rn...r....r...
+00007870: 0072 6f00 0000 7270 0000 0072 1400 0000  .ro...rp...r....
+00007880: 721f 0100 0072 1901 0000 7224 0100 0072  r....r....r$...r
+00007890: 7200 0000 7225 0100 0072 2601 0000 7213  r...r%...r&...r.
+000078a0: 0000 0072 1b00 0000 6301 0000 0000 0000  ...r....c.......
+000078b0: 0000 0000 0002 0000 0003 0000 0013 0000  ................
+000078c0: 0072 9200 0000 7231 0000 0072 9300 0000  .r....r1...r....
+000078d0: 7227 0100 0072 2900 0000 722b 0000 0072  r'...r)...r+...r
+000078e0: 2c00 0000 7228 0100 00df 0300 0072 9400  ,...r(.......r..
+000078f0: 0000 7a2d 5374 6172 745f 3250 5f56 6965  ..z-Start_2P_Vie
+00007900: 772e 5f5f 696e 6974 5f5f 2e3c 6c6f 6361  w.__init__.<loca
+00007910: 6c73 3e2e 6f6e 5f63 6c69 636b 5f62 6163  ls>.on_click_bac
+00007920: 6b63 0100 0000 0000 0000 0000 0000 0100  kc..............
+00007930: 0000 0200 0000 5300 0000 723b 0000 0072  ......S...r;...r
+00007940: 3100 0000 723c 0000 0072 3f00 0000 722b  1...r<...r?...r+
+00007950: 0000 0072 2b00 0000 722c 0000 0072 4000  ...r+...r,...r@.
+00007960: 0000 e403 0000 7241 0000 007a 2d53 7461  ......rA...z-Sta
+00007970: 7274 5f32 505f 5669 6577 2e5f 5f69 6e69  rt_2P_View.__ini
+00007980: 745f 5f2e 3c6c 6f63 616c 733e 2e6f 6e5f  t__.<locals>.on_
+00007990: 636c 6963 6b5f 5175 6974 6301 0000 0000  click_Quitc.....
+000079a0: 0000 0000 0000 0004 0000 0005 0000 0013  ................
+000079b0: 0000 0073 8000 0000 7400 a001 6401 6402  ...s....t...d.d.
+000079c0: a102 7d01 7402 6a03 7c01 6403 6404 6405  ..}.t.j.|.d.d.d.
+000079d0: 8d03 8800 6a04 5f05 8800 6a04 6a05 a006  ....j._...j.j...
+000079e0: 8800 6a04 6a07 a101 0100 8800 6a04 6a05  ..j.j.......j.j.
+000079f0: a008 8800 6a04 6a07 a101 0100 7c01 6401  ....j.j.....|.d.
+00007a00: 6b02 7233 7409 8800 6a0a 8301 7d02 8800  k.r3t...j...}...
+00007a10: 6a04 a00b 7c02 a101 0100 6400 5300 740c  j...|.....d.S.t.
+00007a20: 8800 6a0a 8301 7d03 8800 6a04 a00b 7c03  ..j...}...j...|.
+00007a30: a101 0100 6400 5300 2906 4e72 9700 0000  ....d.S.).Nr....
+00007a40: 7298 0000 0072 1d00 0000 5472 9900 0000  r....r....Tr....
+00007a50: 290d 72a4 0000 0072 a500 0000 7203 0000  ).r....r....r...
+00007a60: 0072 a600 0000 7220 0000 0072 a700 0000  .r....r ...r....
+00007a70: 7229 0100 0072 2100 0000 722a 0100 00da  r)...r!...r*....
+00007a80: 0f50 315f 5475 726e 5f32 505f 5669 6577  .P1_Turn_2P_View
+00007a90: 7225 0000 0072 2600 0000 da0f 5032 5f54  r%...r&.....P2_T
+00007aa0: 7572 6e5f 3250 5f56 6965 7729 0472 2700  urn_2P_View).r'.
+00007ab0: 0000 722d 0100 005a 0b70 6c61 7965 7231  ..r-...Z.player1
+00007ac0: 7669 6577 5a0b 706c 6179 6572 3276 6965  viewZ.player2vie
+00007ad0: 7772 2900 0000 722b 0000 0072 2c00 0000  wr)...r+...r,...
+00007ae0: 722f 0100 00e8 0300 0073 1200 0000 0c02  r/.......s......
+00007af0: 1402 1201 1201 0802 0a01 1001 0a02 1001  ................
+00007b00: 7a2d 5374 6172 745f 3250 5f56 6965 772e  z-Start_2P_View.
+00007b10: 5f5f 696e 6974 5f5f 2e3c 6c6f 6361 6c73  __init__.<locals
+00007b20: 3e2e 6f6e 5f63 6c69 636b 5f72 6f6c 6c63  >.on_click_rollc
+00007b30: 0100 0000 0000 0000 0000 0000 0200 0000  ................
+00007b40: 0300 0000 1300 0000 7234 0000 0072 3100  ........r4...r1.
+00007b50: 0000 7235 0000 0072 3800 0000 7229 0000  ..r5...r8...r)..
+00007b60: 0072 2b00 0000 722c 0000 0072 3900 0000  .r+...r,...r9...
+00007b70: f703 0000 723a 0000 007a 3153 7461 7274  ....r:...z1Start
+00007b80: 5f32 505f 5669 6577 2e5f 5f69 6e69 745f  _2P_View.__init_
+00007b90: 5f2e 3c6c 6f63 616c 733e 2e6f 6e5f 636c  _.<locals>.on_cl
+00007ba0: 6963 6b5f 5365 7474 696e 6773 7230 0100  ick_Settingsr0..
+00007bb0: 0072 3101 0000 724f 0000 0072 2900 0000  .r1...rO...r)...
+00007bc0: 722c 0000 0072 4300 0000 ce03 0000 7328  r,...rC.......s(
+00007bd0: 0000 000a 0106 010c 020a 0114 0214 0114  ................
+00007be0: 0114 010c 020c 010c 010c 0108 020e 0108  ................
+00007bf0: 040a 0108 030e 0108 0e12 017a 1653 7461  ...........z.Sta
+00007c00: 7274 5f32 505f 5669 6577 2e5f 5f69 6e69  rt_2P_View.__ini
+00007c10: 745f 5f63 0100 0000 0000 0000 0000 0000  t__c............
+00007c20: 0100 0000 0300 0000 4300 0000 7251 0000  ........C...rQ..
+00007c30: 0072 3100 0000 7252 0000 0072 2900 0000  .r1...rR...r)...
+00007c40: 722b 0000 0072 2b00 0000 722c 0000 0072  r+...r+...r,...r
+00007c50: 5400 0000 fd03 0000 7255 0000 007a 1a53  T.......rU...z.S
+00007c60: 7461 7274 5f32 505f 5669 6577 2e6f 6e5f  tart_2P_View.on_
+00007c70: 7368 6f77 5f76 6965 7763 0100 0000 0000  show_viewc......
+00007c80: 0000 0000 0000 0100 0000 0200 0000 4300  ..............C.
+00007c90: 0000 7256 0000 0072 3100 0000 7257 0000  ..rV...r1...rW..
+00007ca0: 0072 2900 0000 722b 0000 0072 2b00 0000  .r)...r+...r+...
+00007cb0: 722c 0000 0072 5900 0000 0104 0000 725a  r,...rY.......rZ
+00007cc0: 0000 007a 1a53 7461 7274 5f32 505f 5669  ...z.Start_2P_Vi
+00007cd0: 6577 2e6f 6e5f 6869 6465 5f76 6965 7763  ew.on_hide_viewc
+00007ce0: 0100 0000 0000 0000 0000 0000 0100 0000  ................
+00007cf0: 0400 0000 4300 0000 7234 0100 0072 3100  ....C...r4...r1.
+00007d00: 0000 7235 0100 0072 2900 0000 722b 0000  ..r5...r)...r+..
+00007d10: 0072 2b00 0000 722c 0000 0072 5f00 0000  .r+...r,...r_...
+00007d20: 0404 0000 7236 0100 007a 1553 7461 7274  ....r6...z.Start
+00007d30: 5f32 505f 5669 6577 2e6f 6e5f 6472 6177  _2P_View.on_draw
+00007d40: 7261 0000 0072 2b00 0000 722b 0000 0072  ra...r+...r+...r
+00007d50: 4f00 0000 722c 0000 0072 3200 0000 cc03  O...r,...r2.....
+00007d60: 0000 730a 0000 0008 000c 0208 2f08 0410  ..s........./...
+00007d70: 0372 3200 0000 6300 0000 0000 0000 0000  .r2...c.........
+00007d80: 0000 0000 0000 0008 0000 0000 0000 0072  ...............r
+00007d90: 3701 0000 290f 725c 0100 0063 0200 0000  7...).r\...c....
+00007da0: 0000 0000 0000 0000 0a00 0000 0700 0000  ................
+00007db0: 0300 0000 7238 0100 0029 174e 72a9 0000  ....r8...).Nr...
+00007dc0: 0072 6d00 0000 726e 0000 0072 0800 0000  .rm...rn...r....
+00007dd0: 7210 0000 0072 8c00 0000 7270 0000 0072  r....r....rp...r
+00007de0: 1400 0000 728e 0000 0072 8f00 0000 7213  ....r....r....r.
+00007df0: 0000 0072 da00 0000 72d9 0000 0072 1b00  ...r....r....r..
+00007e00: 0000 6301 0000 0000 0000 0000 0000 0002  ..c.............
+00007e10: 0000 0003 0000 0013 0000 0072 9200 0000  ...........r....
+00007e20: 7231 0000 0072 9300 0000 7227 0100 0072  r1...r....r'...r
+00007e30: 2900 0000 722b 0000 0072 2c00 0000 7239  )...r+...r,...r9
+00007e40: 0100 0021 0400 0072 9400 0000 7a2f 5031  ...!...r....z/P1
+00007e50: 5f54 7572 6e5f 3250 5f56 6965 772e 5f5f  _Turn_2P_View.__
+00007e60: 696e 6974 5f5f 2e3c 6c6f 6361 6c73 3e2e  init__.<locals>.
+00007e70: 6f6e 5f63 6c69 636b 5f65 7869 7463 0100  on_click_exitc..
+00007e80: 0000 0000 0000 0000 0000 0100 0000 0200  ................
+00007e90: 0000 5300 0000 723b 0000 0072 3100 0000  ..S...r;...r1...
+00007ea0: 723c 0000 0072 3f00 0000 722b 0000 0072  r<...r?...r+...r
+00007eb0: 2b00 0000 722c 0000 0072 4000 0000 2604  +...r,...r@...&.
+00007ec0: 0000 7241 0000 007a 2f50 315f 5475 726e  ..rA...z/P1_Turn
+00007ed0: 5f32 505f 5669 6577 2e5f 5f69 6e69 745f  _2P_View.__init_
+00007ee0: 5f2e 3c6c 6f63 616c 733e 2e6f 6e5f 636c  _.<locals>.on_cl
+00007ef0: 6963 6b5f 5175 6974 6301 0000 0000 0000  ick_Quitc.......
+00007f00: 0000 0000 0002 0000 0003 0000 0013 0000  ................
+00007f10: 0072 3400 0000 7231 0000 0072 3500 0000  .r4...r1...r5...
+00007f20: 7238 0000 0072 2900 0000 722b 0000 0072  r8...r)...r+...r
+00007f30: 2c00 0000 7239 0000 002a 0400 0072 3a00  ,...r9...*...r:.
+00007f40: 0000 7a33 5031 5f54 7572 6e5f 3250 5f56  ..z3P1_Turn_2P_V
+00007f50: 6965 772e 5f5f 696e 6974 5f5f 2e3c 6c6f  iew.__init__.<lo
+00007f60: 6361 6c73 3e2e 6f6e 5f63 6c69 636b 5f53  cals>.on_click_S
+00007f70: 6574 7469 6e67 7363 0100 0000 0000 0000  ettingsc........
+00007f80: 0000 0000 0200 0000 0300 0000 1300 0000  ................
+00007f90: 7292 0000 0072 3100 0000 2904 da12 5032  r....r1...)...P2
+00007fa0: 5f50 7265 5475 726e 5f32 505f 5669 6577  _PreTurn_2P_View
+00007fb0: 7225 0000 0072 2000 0000 7226 0000 00a9  r%...r ...r&....
+00007fc0: 0272 2700 0000 5a0e 6e65 7874 506c 6179  .r'...Z.nextPlay
+00007fd0: 6572 5669 6577 7229 0000 0072 2b00 0000  erViewr)...r+...
+00007fe0: 722c 0000 0072 3b01 0000 3004 0000 7294  r,...r;...0...r.
+00007ff0: 0000 007a 2f50 315f 5475 726e 5f32 505f  ...z/P1_Turn_2P_
+00008000: 5669 6577 2e5f 5f69 6e69 745f 5f2e 3c6c  View.__init__.<l
+00008010: 6f63 616c 733e 2e6f 6e5f 636c 6963 6b5f  ocals>.on_click_
+00008020: 646f 6e65 723c 0100 0072 3e01 0000 724f  doner<...r>...rO
+00008030: 0000 0072 2900 0000 722c 0000 0072 4300  ...r)...r,...rC.
+00008040: 0000 0d04 0000 7240 0100 007a 1850 315f  ......r@...z.P1_
+00008050: 5475 726e 5f32 505f 5669 6577 2e5f 5f69  Turn_2P_View.__i
+00008060: 6e69 745f 5f63 0100 0000 0000 0000 0000  nit__c..........
+00008070: 0000 0100 0000 0300 0000 4300 0000 7251  ..........C...rQ
+00008080: 0000 0072 3100 0000 7252 0000 0072 2900  ...r1...rR...r).
+00008090: 0000 722b 0000 0072 2b00 0000 722c 0000  ..r+...r+...r,..
+000080a0: 0072 5400 0000 3504 0000 7255 0000 007a  .rT...5...rU...z
+000080b0: 1c50 315f 5475 726e 5f32 505f 5669 6577  .P1_Turn_2P_View
+000080c0: 2e6f 6e5f 7368 6f77 5f76 6965 7763 0100  .on_show_viewc..
+000080d0: 0000 0000 0000 0000 0000 0100 0000 0200  ................
+000080e0: 0000 4300 0000 7256 0000 0072 3100 0000  ..C...rV...r1...
+000080f0: 7257 0000 0072 2900 0000 722b 0000 0072  rW...r)...r+...r
+00008100: 2b00 0000 722c 0000 0072 5900 0000 3904  +...r,...rY...9.
+00008110: 0000 725a 0000 007a 1c50 315f 5475 726e  ..rZ...z.P1_Turn
+00008120: 5f32 505f 5669 6577 2e6f 6e5f 6869 6465  _2P_View.on_hide
+00008130: 5f76 6965 7763 0100 0000 0000 0000 0000  _viewc..........
+00008140: 0000 0100 0000 0700 0000 4300 0000 f3a8  ..........C.....
+00008150: 0000 007c 00a0 00a1 0001 007c 006a 01a0  ...|.......|.j..
+00008160: 02a1 0001 0074 03a0 04a1 0001 0074 05a0  .....t.......t..
+00008170: 0664 0164 0264 0364 0474 036a 07a1 0501  .d.d.d.d.t.j....
+00008180: 0074 03a0 087c 006a 096a 0a6a 0b7c 006a  .t...|.j.j.j.|.j
+00008190: 096a 0a6a 0ca1 0201 0074 03a0 0d7c 006a  .j.j.....t...|.j
+000081a0: 096a 0e6a 0f64 0519 007c 006a 096a 0e6a  .j.j.d...|.j.j.j
+000081b0: 0f64 0619 007c 006a 096a 0e6a 10a1 0301  .d...|.j.j.j....
+000081c0: 007c 006a 1164 076b 0272 4674 03a0 127c  .|.j.d.k.rFt...|
+000081d0: 006a 096a 0e6a 13a1 0101 0064 0053 0074  .j.j.j.....d.S.t
+000081e0: 03a0 147c 006a 096a 0e6a 157c 006a 096a  ...|.j.j.j.|.j.j
+000081f0: 0e6a 16a1 0201 0064 0053 0072 4101 0000  .j.....d.S.rA...
+00008200: 2917 725d 0000 0072 4600 0000 725e 0000  ).r]...rF...r^..
+00008210: 0072 0400 0000 72d1 0000 0072 3d00 0000  .r....r....r=...
+00008220: 7220 0100 0072 4501 0000 72d2 0000 0072  r ...rE...r....r
+00008230: 2000 0000 7221 0000 0072 d300 0000 72ab   ...r!...r....r.
+00008240: 0000 0072 d700 0000 72a7 0000 0072 bc00  ...r....r....r..
+00008250: 0000 72d8 0000 0072 3d01 0000 7246 0100  ..r....r=...rF..
+00008260: 0072 4701 0000 7248 0100 0072 4901 0000  .rG...rH...rI...
+00008270: 724a 0100 0072 2900 0000 722b 0000 0072  rJ...r)...r+...r
+00008280: 2b00 0000 722c 0000 0072 5f00 0000 3c04  +...r,...r_...<.
+00008290: 0000 f31a 0000 0008 010a 0108 0114 0118  ................
+000082a0: 0128 0108 0206 ff08 0108 ff04 0110 0108  .(..............
+000082b0: ff7a 1750 315f 5475 726e 5f32 505f 5669  .z.P1_Turn_2P_Vi
+000082c0: 6577 2e6f 6e5f 6472 6177 72f5 0000 0072  ew.on_drawr....r
+000082d0: f600 0000 72f7 0000 0072 f800 0000 6305  ....r....r....c.
+000082e0: 0000 0000 0000 0000 0000 0007 0000 0006  ................
+000082f0: 0000 0043 0000 0072 4b01 0000 724c 0100  ...C...rK...rL..
+00008300: 0072 4e01 0000 7258 0100 0072 2b00 0000  .rN...rX...r+...
+00008310: 722b 0000 0072 2c00 0000 7215 0100 0047  r+...r,...r....G
+00008320: 0400 0072 5901 0000 7a1e 5031 5f54 7572  ...rY...z.P1_Tur
+00008330: 6e5f 3250 5f56 6965 772e 6f6e 5f6d 6f75  n_2P_View.on_mou
+00008340: 7365 5f70 7265 7373 725a 0100 0072 2b00  se_pressrZ...r+.
+00008350: 0000 722b 0000 0072 4f00 0000 722c 0000  ..r+...rO...r,..
+00008360: 0072 5c01 0000 0b04 0000 f30c 0000 0008  .r\.............
+00008370: 000c 0208 2808 0408 0322 0b72 5c01 0000  ....(....".r\...
+00008380: 6300 0000 0000 0000 0000 0000 0000 0000  c...............
+00008390: 0008 0000 0000 0000 0072 3701 0000 290f  .........r7...).
+000083a0: 725d 0100 0063 0200 0000 0000 0000 0000  r]...c..........
+000083b0: 0000 0a00 0000 0700 0000 0300 0000 7304  ..............s.
+000083c0: 0100 0074 0083 00a0 01a1 0001 007c 0188  ...t.........|..
+000083d0: 005f 0274 036a 04a0 05a1 0088 005f 0688  ._.t.j......._..
+000083e0: 006a 06a0 07a1 0001 0064 0188 005f 0874  .j.......d..._.t
+000083f0: 036a 04a0 0964 0264 0364 0464 0564 06a1  .j...d.d.d.d.d..
+00008400: 057d 0274 036a 04a0 0964 0264 0764 0464  .}.t.j...d.d.d.d
+00008410: 0564 08a1 057d 0374 036a 04a0 0964 0964  .d...}.t.j...d.d
+00008420: 0264 0a64 0564 0ba1 057d 0474 036a 04a0  .d.d.d...}.t.j..
+00008430: 0964 0964 0c64 0a64 0564 0da1 057d 0588  .d.d.d.d.d...}..
+00008440: 006a 06a0 0a7c 02a1 0101 0088 006a 06a0  .j...|.......j..
+00008450: 0a7c 03a1 0101 0088 006a 06a0 0a7c 04a1  .|.......j...|..
+00008460: 0101 0088 006a 06a0 0a7c 05a1 0101 007c  .....j...|.....|
+00008470: 02a0 0b64 0ea1 0187 0066 0164 0f64 1084  ...d.....f.d.d..
+00008480: 0883 017d 067c 03a0 0b64 0ea1 0164 1164  ...}.|...d...d.d
+00008490: 1284 0083 017d 077c 04a0 0b64 0ea1 0187  .....}.|...d....
+000084a0: 0066 0164 1364 1484 0883 017d 087c 05a0  .f.d.d.....}.|..
+000084b0: 0b64 0ea1 0187 0066 0164 1564 1684 0883  .d.....f.d.d....
+000084c0: 017d 0964 0053 0029 174e 72a9 0000 0072  .}.d.S.).Nr....r
+000084d0: 6d00 0000 726e 0000 0072 0800 0000 7210  m...rn...r....r.
+000084e0: 0000 0072 8c00 0000 7270 0000 0072 1400  ...r....rp...r..
+000084f0: 0000 728e 0000 0072 8f00 0000 7213 0000  ..r....r....r...
+00008500: 0072 da00 0000 72d9 0000 0072 1b00 0000  .r....r....r....
+00008510: 6301 0000 0000 0000 0000 0000 0002 0000  c...............
+00008520: 0003 0000 0013 0000 0072 9200 0000 7231  .........r....r1
+00008530: 0000 0072 9300 0000 7227 0100 0072 2900  ...r....r'...r).
+00008540: 0000 722b 0000 0072 2c00 0000 7239 0100  ..r+...r,...r9..
+00008550: 0079 0400 0072 9400 0000 7a2f 5032 5f54  .y...r....z/P2_T
+00008560: 7572 6e5f 3250 5f56 6965 772e 5f5f 696e  urn_2P_View.__in
+00008570: 6974 5f5f 2e3c 6c6f 6361 6c73 3e2e 6f6e  it__.<locals>.on
+00008580: 5f63 6c69 636b 5f65 7869 7463 0100 0000  _click_exitc....
+00008590: 0000 0000 0000 0000 0100 0000 0200 0000  ................
+000085a0: 5300 0000 723b 0000 0072 3100 0000 723c  S...r;...r1...r<
+000085b0: 0000 0072 3f00 0000 722b 0000 0072 2b00  ...r?...r+...r+.
+000085c0: 0000 722c 0000 0072 4000 0000 7e04 0000  ..r,...r@...~...
+000085d0: 7241 0000 007a 2f50 325f 5475 726e 5f32  rA...z/P2_Turn_2
+000085e0: 505f 5669 6577 2e5f 5f69 6e69 745f 5f2e  P_View.__init__.
+000085f0: 3c6c 6f63 616c 733e 2e6f 6e5f 636c 6963  <locals>.on_clic
+00008600: 6b5f 5175 6974 6301 0000 0000 0000 0000  k_Quitc.........
+00008610: 0000 0002 0000 0003 0000 0013 0000 0072  ...............r
+00008620: 3400 0000 7231 0000 0072 3500 0000 7238  4...r1...r5...r8
+00008630: 0000 0072 2900 0000 722b 0000 0072 2c00  ...r)...r+...r,.
+00008640: 0000 7239 0000 0082 0400 0072 3a00 0000  ..r9.......r:...
+00008650: 7a33 5032 5f54 7572 6e5f 3250 5f56 6965  z3P2_Turn_2P_Vie
+00008660: 772e 5f5f 696e 6974 5f5f 2e3c 6c6f 6361  w.__init__.<loca
+00008670: 6c73 3e2e 6f6e 5f63 6c69 636b 5f53 6574  ls>.on_click_Set
+00008680: 7469 6e67 7363 0100 0000 0000 0000 0000  tingsc..........
+00008690: 0000 0200 0000 0300 0000 1300 0000 7292  ..............r.
+000086a0: 0000 0072 3100 0000 2904 da12 5031 5f50  ...r1...)...P1_P
+000086b0: 7265 5475 726e 5f32 505f 5669 6577 7225  reTurn_2P_Viewr%
+000086c0: 0000 0072 2000 0000 7226 0000 0072 5f01  ...r ...r&...r_.
+000086d0: 0000 7229 0000 0072 2b00 0000 722c 0000  ..r)...r+...r,..
+000086e0: 0072 3b01 0000 8804 0000 7294 0000 007a  .r;.......r....z
+000086f0: 2f50 325f 5475 726e 5f32 505f 5669 6577  /P2_Turn_2P_View
+00008700: 2e5f 5f69 6e69 745f 5f2e 3c6c 6f63 616c  .__init__.<local
+00008710: 733e 2e6f 6e5f 636c 6963 6b5f 646f 6e65  s>.on_click_done
+00008720: 290c 7242 0000 0072 4300 0000 7225 0000  ).rB...rC...r%..
+00008730: 0072 3d00 0000 7244 0000 0072 4500 0000  .r=...rD...rE...
+00008740: 7246 0000 0072 4700 0000 723d 0100 0072  rF...rG...r=...r
+00008750: 4c00 0000 724a 0000 0072 2700 0000 723e  L...rJ...r'...r>
+00008760: 0100 0072 4f00 0000 7229 0000 0072 2c00  ...rO...r)...r,.
+00008770: 0000 7243 0000 0065 0400 0073 2a00 0000  ..rC...e...s*...
+00008780: 0a01 0601 0c02 0a01 0602 1402 1401 1401  ................
+00008790: 1402 0c02 0c01 0c01 0c01 0802 0e01 0804  ................
+000087a0: 0a01 0803 0e01 0805 1201 7a18 5032 5f54  ..........z.P2_T
+000087b0: 7572 6e5f 3250 5f56 6965 772e 5f5f 696e  urn_2P_View.__in
+000087c0: 6974 5f5f 6301 0000 0000 0000 0000 0000  it__c...........
+000087d0: 0001 0000 0003 0000 0043 0000 0072 5100  .........C...rQ.
+000087e0: 0000 7231 0000 0072 5200 0000 7229 0000  ..r1...rR...r)..
+000087f0: 0072 2b00 0000 722b 0000 0072 2c00 0000  .r+...r+...r,...
+00008800: 7254 0000 008d 0400 0072 5500 0000 7a1c  rT.......rU...z.
+00008810: 5032 5f54 7572 6e5f 3250 5f56 6965 772e  P2_Turn_2P_View.
+00008820: 6f6e 5f73 686f 775f 7669 6577 6301 0000  on_show_viewc...
+00008830: 0000 0000 0000 0000 0001 0000 0002 0000  ................
+00008840: 0043 0000 0072 5600 0000 7231 0000 0072  .C...rV...r1...r
+00008850: 5700 0000 7229 0000 0072 2b00 0000 722b  W...r)...r+...r+
+00008860: 0000 0072 2c00 0000 7259 0000 0091 0400  ...r,...rY......
+00008870: 0072 5a00 0000 7a1c 5032 5f54 7572 6e5f  .rZ...z.P2_Turn_
+00008880: 3250 5f56 6965 772e 6f6e 5f68 6964 655f  2P_View.on_hide_
+00008890: 7669 6577 6301 0000 0000 0000 0000 0000  viewc...........
+000088a0: 0001 0000 0007 0000 0043 0000 0072 6001  .........C...r`.
+000088b0: 0000 7241 0100 0029 1772 5d00 0000 7246  ..rA...).r]...rF
+000088c0: 0000 0072 5e00 0000 7204 0000 0072 d100  ...r^...r....r..
+000088d0: 0000 723d 0000 0072 2001 0000 da11 6c69  ..r=...r .....li
+000088e0: 6768 7443 6865 636b 6572 436f 6c6f 7272  ghtCheckerColorr
+000088f0: d200 0000 7220 0000 0072 2100 0000 72d3  ....r ...r!...r.
+00008900: 0000 0072 ab00 0000 72d7 0000 0072 a700  ...r....r....r..
+00008910: 0000 72bc 0000 0072 d800 0000 723d 0100  ..r....r....r=..
+00008920: 0072 4601 0000 7247 0100 0072 4801 0000  .rF...rG...rH...
+00008930: 7249 0100 0072 4a01 0000 7229 0000 0072  rI...rJ...r)...r
+00008940: 2b00 0000 722b 0000 0072 2c00 0000 725f  +...r+...r,...r_
+00008950: 0000 0094 0400 0072 6101 0000 7a17 5032  .......ra...z.P2
+00008960: 5f54 7572 6e5f 3250 5f56 6965 772e 6f6e  _Turn_2P_View.on
+00008970: 5f64 7261 7772 f500 0000 72f6 0000 0072  _drawr....r....r
+00008980: f700 0000 72f8 0000 0063 0500 0000 0000  ....r....c......
+00008990: 0000 0000 0000 0700 0000 0600 0000 4300  ..............C.
+000089a0: 0000 724b 0100 0029 054e 72a9 0000 0072  ..rK...).Nr....r
+000089b0: 0100 0000 724d 0100 0072 9800 0000 724e  ....rM...r....rN
+000089c0: 0100 0072 5801 0000 722b 0000 0072 2b00  ...rX...r+...r+.
+000089d0: 0000 722c 0000 0072 1501 0000 9f04 0000  ..r,...r........
+000089e0: 7259 0100 007a 1e50 325f 5475 726e 5f32  rY...z.P2_Turn_2
+000089f0: 505f 5669 6577 2e6f 6e5f 6d6f 7573 655f  P_View.on_mouse_
+00008a00: 7072 6573 7372 5a01 0000 722b 0000 0072  pressrZ...r+...r
+00008a10: 2b00 0000 724f 0000 0072 2c00 0000 725d  +...rO...r,...r]
+00008a20: 0100 0063 0400 0072 6201 0000 725d 0100  ...c...rb...r]..
+00008a30: 0063 0000 0000 0000 0000 0000 0000 0000  .c..............
+00008a40: 0000 0300 0000 0000 0000 7205 0000 0029  ..........r....)
+00008a50: 0972 6301 0000 6302 0000 0000 0000 0000  .rc...c.........
+00008a60: 0000 000a 0000 0007 0000 0003 0000 00f3  ................
+00008a70: fe00 0000 7400 8300 a001 a100 0100 7c01  ....t.........|.
+00008a80: 8800 5f02 7403 6a04 a005 a100 8800 5f06  .._.t.j......._.
+00008a90: 8800 6a06 a007 a100 0100 7403 6a04 a008  ..j.......t.j...
+00008aa0: 6401 6402 6403 6404 6405 a105 7d02 7403  d.d.d.d.d...}.t.
+00008ab0: 6a04 a008 6401 6406 6403 6404 6407 a105  j...d.d.d.d.d...
+00008ac0: 7d03 7403 6a04 a008 6408 6401 6409 6404  }.t.j...d.d.d.d.
+00008ad0: 640a a105 7d04 7403 6a04 a008 6408 640b  d...}.t.j...d.d.
+00008ae0: 6409 6404 640c a105 7d05 8800 6a06 a009  d.d.d...}...j...
+00008af0: 7c02 a101 0100 8800 6a06 a009 7c03 a101  |.......j...|...
+00008b00: 0100 8800 6a06 a009 7c04 a101 0100 8800  ....j...|.......
+00008b10: 6a06 a009 7c05 a101 0100 7c02 a00a 640d  j...|.....|...d.
+00008b20: a101 8700 6601 640e 640f 8408 8301 7d06  ....f.d.d.....}.
+00008b30: 7c03 a00a 640d a101 6410 6411 8400 8301  |...d...d.d.....
+00008b40: 7d07 7c04 a00a 640d a101 8700 6601 6412  }.|...d.....f.d.
+00008b50: 6413 8408 8301 7d08 7c05 a00a 640d a101  d.....}.|...d...
+00008b60: 8700 6601 6414 6415 8408 8301 7d09 6400  ..f.d.d.....}.d.
+00008b70: 5300 2916 4e72 6d00 0000 726e 0000 0072  S.).Nrm...rn...r
+00008b80: 0800 0000 7210 0000 0072 8c00 0000 7270  ....r....r....rp
+00008b90: 0000 0072 1400 0000 728e 0000 0072 8f00  ...r....r....r..
+00008ba0: 0000 7213 0000 0072 1f01 0000 7225 0100  ..r....r....r%..
+00008bb0: 0072 1b00 0000 6301 0000 0000 0000 0000  .r....c.........
+00008bc0: 0000 0002 0000 0003 0000 0013 0000 0072  ...............r
+00008bd0: 9200 0000 7231 0000 0072 9300 0000 7227  ....r1...r....r'
+00008be0: 0100 0072 2900 0000 722b 0000 0072 2c00  ...r)...r+...r,.
+00008bf0: 0000 7239 0100 00cf 0400 0072 9400 0000  ..r9.......r....
+00008c00: 7a32 5031 5f50 7265 5475 726e 5f32 505f  z2P1_PreTurn_2P_
+00008c10: 5669 6577 2e5f 5f69 6e69 745f 5f2e 3c6c  View.__init__.<l
+00008c20: 6f63 616c 733e 2e6f 6e5f 636c 6963 6b5f  ocals>.on_click_
+00008c30: 6578 6974 6301 0000 0000 0000 0000 0000  exitc...........
+00008c40: 0001 0000 0002 0000 0053 0000 0072 3b00  .........S...r;.
+00008c50: 0000 7231 0000 0072 3c00 0000 723f 0000  ..r1...r<...r?..
+00008c60: 0072 2b00 0000 722b 0000 0072 2c00 0000  .r+...r+...r,...
+00008c70: 7240 0000 00d4 0400 0072 4100 0000 7a32  r@.......rA...z2
+00008c80: 5031 5f50 7265 5475 726e 5f32 505f 5669  P1_PreTurn_2P_Vi
+00008c90: 6577 2e5f 5f69 6e69 745f 5f2e 3c6c 6f63  ew.__init__.<loc
+00008ca0: 616c 733e 2e6f 6e5f 636c 6963 6b5f 5175  als>.on_click_Qu
+00008cb0: 6974 6301 0000 0000 0000 0000 0000 0002  itc.............
+00008cc0: 0000 0003 0000 0013 0000 0072 3400 0000  ...........r4...
+00008cd0: 7231 0000 0072 3500 0000 7238 0000 0072  r1...r5...r8...r
+00008ce0: 2900 0000 722b 0000 0072 2c00 0000 7239  )...r+...r,...r9
+00008cf0: 0000 00d8 0400 0072 3a00 0000 7a36 5031  .......r:...z6P1
+00008d00: 5f50 7265 5475 726e 5f32 505f 5669 6577  _PreTurn_2P_View
+00008d10: 2e5f 5f69 6e69 745f 5f2e 3c6c 6f63 616c  .__init__.<local
+00008d20: 733e 2e6f 6e5f 636c 6963 6b5f 5365 7474  s>.on_click_Sett
+00008d30: 696e 6773 6301 0000 0000 0000 0000 0000  ingsc...........
+00008d40: 0002 0000 0005 0000 0013 0000 00f3 5200  ..............R.
+00008d50: 0000 7400 6a01 6401 6402 6403 6404 8d03  ..t.j.d.d.d.d...
+00008d60: 8800 6a02 5f03 8800 6a02 6a03 a004 8800  ..j._...j.j.....
+00008d70: 6a02 6a05 a101 0100 8800 6a02 6a03 a006  j.j.......j.j...
+00008d80: 8800 6a02 6a05 a101 0100 7407 8800 6a08  ..j.j.....t...j.
+00008d90: 8301 7d01 8800 6a02 a009 7c01 a101 0100  ..}...j...|.....
+00008da0: 6400 5300 2905 4e72 9700 0000 721d 0000  d.S.).Nr....r...
+00008db0: 0046 7299 0000 0029 0a72 0300 0000 72a6  .Fr....).r....r.
+00008dc0: 0000 0072 2000 0000 72a7 0000 0072 2901  ...r ...r....r).
+00008dd0: 0000 7221 0000 0072 2a01 0000 725c 0100  ..r!...r*...r\..
+00008de0: 0072 2500 0000 7226 0000 0072 5f01 0000  .r%...r&...r_...
+00008df0: 7229 0000 0072 2b00 0000 722c 0000 0072  r)...r+...r,...r
+00008e00: 2f01 0000 de04 0000 f30a 0000 0014 0212  /...............
+00008e10: 0112 010a 0210 017a 3250 315f 5072 6554  .......z2P1_PreT
+00008e20: 7572 6e5f 3250 5f56 6965 772e 5f5f 696e  urn_2P_View.__in
+00008e30: 6974 5f5f 2e3c 6c6f 6361 6c73 3e2e 6f6e  it__.<locals>.on
+00008e40: 5f63 6c69 636b 5f72 6f6c 6c72 3001 0000  _click_rollr0...
+00008e50: a90a 722a 0000 0072 2500 0000 723f 0100  ..r*...r%...r?..
+00008e60: 0072 8a00 0000 7233 0100 0072 3201 0000  .r....r3...r2...
+00008e70: 7239 0100 0072 4000 0000 7239 0000 0072  r9...r@...r9...r
+00008e80: 2f01 0000 724f 0000 0072 2900 0000 722c  /...rO...r)...r,
+00008e90: 0000 0072 4300 0000 bd04 0000 f328 0000  ...rC........(..
+00008ea0: 000a 0106 010c 020a 0114 0214 0114 0114  ................
+00008eb0: 020c 020c 010c 010c 0108 020e 0108 040a  ................
+00008ec0: 0108 030e 0108 0512 017a 1b50 315f 5072  .........z.P1_Pr
+00008ed0: 6554 7572 6e5f 3250 5f56 6965 772e 5f5f  eTurn_2P_View.__
+00008ee0: 696e 6974 5f5f 6301 0000 0000 0000 0000  init__c.........
+00008ef0: 0000 0001 0000 0003 0000 0043 0000 0072  ...........C...r
+00008f00: 5100 0000 7231 0000 0072 5200 0000 7229  Q...r1...rR...r)
+00008f10: 0000 0072 2b00 0000 722b 0000 0072 2c00  ...r+...r+...r,.
+00008f20: 0000 7254 0000 00e7 0400 0072 5500 0000  ..rT.......rU...
+00008f30: 7a1f 5031 5f50 7265 5475 726e 5f32 505f  z.P1_PreTurn_2P_
+00008f40: 5669 6577 2e6f 6e5f 7368 6f77 5f76 6965  View.on_show_vie
+00008f50: 7763 0100 0000 0000 0000 0000 0000 0100  wc..............
+00008f60: 0000 0200 0000 4300 0000 7256 0000 0072  ......C...rV...r
+00008f70: 3100 0000 7257 0000 0072 2900 0000 722b  1...rW...r)...r+
+00008f80: 0000 0072 2b00 0000 722c 0000 0072 5900  ...r+...r,...rY.
+00008f90: 0000 eb04 0000 725a 0000 007a 1f50 315f  ......rZ...z.P1_
+00008fa0: 5072 6554 7572 6e5f 3250 5f56 6965 772e  PreTurn_2P_View.
+00008fb0: 6f6e 5f68 6964 655f 7669 6577 6301 0000  on_hide_viewc...
+00008fc0: 0000 0000 0000 0000 0001 0000 0007 0000  ................
+00008fd0: 0043 0000 00f3 4a00 0000 7c00 a000 a100  .C....J...|.....
+00008fe0: 0100 7c00 6a01 a002 a100 0100 7403 a004  ..|.j.......t...
+00008ff0: a100 0100 7405 a006 6401 6402 6403 6404  ....t...d.d.d.d.
+00009000: 7403 6a07 a105 0100 7403 a008 7c00 6a09  t.j.....t...|.j.
+00009010: 6a0a 6a0b 7c00 6a09 6a0a 6a0c a102 0100  j.j.|.j.j.j.....
+00009020: 6400 5300 725b 0100 0029 0d72 5d00 0000  d.S.r[...).r]...
+00009030: 7246 0000 0072 5e00 0000 7204 0000 0072  rF...r^...r....r
+00009040: d100 0000 723d 0000 0072 2001 0000 7245  ....r=...r ...rE
+00009050: 0100 0072 d200 0000 7220 0000 0072 2100  ...r....r ...r!.
+00009060: 0000 72d3 0000 0072 ab00 0000 7229 0000  ..r....r....r)..
+00009070: 0072 2b00 0000 722b 0000 0072 2c00 0000  .r+...r+...r,...
+00009080: 725f 0000 00ee 0400 00f3 0a00 0000 0801  r_..............
+00009090: 0a01 0801 1401 1c01 7a1a 5031 5f50 7265  ........z.P1_Pre
+000090a0: 5475 726e 5f32 505f 5669 6577 2e6f 6e5f  Turn_2P_View.on_
+000090b0: 6472 6177 7261 0000 0072 2b00 0000 722b  drawra...r+...r+
+000090c0: 0000 0072 4f00 0000 722c 0000 0072 6301  ...rO...r,...rc.
+000090d0: 0000 bb04 0000 f30a 0000 0008 000c 0208  ................
+000090e0: 2a08 0410 0372 6301 0000 6300 0000 0000  *....rc...c.....
+000090f0: 0000 0000 0000 0000 0000 0003 0000 0000  ................
+00009100: 0000 0072 0500 0000 2909 725e 0100 0063  ...r....).r^...c
+00009110: 0200 0000 0000 0000 0000 0000 0a00 0000  ................
+00009120: 0700 0000 0300 0000 7265 0100 0029 164e  ........re...).N
+00009130: 726d 0000 0072 6e00 0000 7208 0000 0072  rm...rn...r....r
+00009140: 1000 0000 728c 0000 0072 7000 0000 7214  ....r....rp...r.
+00009150: 0000 0072 8e00 0000 728f 0000 0072 1300  ...r....r....r..
+00009160: 0000 721f 0100 0072 2501 0000 721b 0000  ..r....r%...r...
+00009170: 0063 0100 0000 0000 0000 0000 0000 0200  .c..............
+00009180: 0000 0300 0000 1300 0000 7292 0000 0072  ..........r....r
+00009190: 3100 0000 7293 0000 0072 2701 0000 7229  1...r....r'...r)
+000091a0: 0000 0072 2b00 0000 722c 0000 0072 3901  ...r+...r,...r9.
+000091b0: 0000 0a05 0000 7294 0000 007a 3250 325f  ......r....z2P2_
+000091c0: 5072 6554 7572 6e5f 3250 5f56 6965 772e  PreTurn_2P_View.
+000091d0: 5f5f 696e 6974 5f5f 2e3c 6c6f 6361 6c73  __init__.<locals
+000091e0: 3e2e 6f6e 5f63 6c69 636b 5f65 7869 7463  >.on_click_exitc
+000091f0: 0100 0000 0000 0000 0000 0000 0100 0000  ................
+00009200: 0200 0000 5300 0000 723b 0000 0072 3100  ....S...r;...r1.
+00009210: 0000 723c 0000 0072 3f00 0000 722b 0000  ..r<...r?...r+..
+00009220: 0072 2b00 0000 722c 0000 0072 4000 0000  .r+...r,...r@...
+00009230: 0f05 0000 7241 0000 007a 3250 325f 5072  ....rA...z2P2_Pr
+00009240: 6554 7572 6e5f 3250 5f56 6965 772e 5f5f  eTurn_2P_View.__
+00009250: 696e 6974 5f5f 2e3c 6c6f 6361 6c73 3e2e  init__.<locals>.
+00009260: 6f6e 5f63 6c69 636b 5f51 7569 7463 0100  on_click_Quitc..
+00009270: 0000 0000 0000 0000 0000 0200 0000 0300  ................
+00009280: 0000 1300 0000 7234 0000 0072 3100 0000  ......r4...r1...
+00009290: 7235 0000 0072 3800 0000 7229 0000 0072  r5...r8...r)...r
+000092a0: 2b00 0000 722c 0000 0072 3900 0000 1305  +...r,...r9.....
+000092b0: 0000 723a 0000 007a 3650 325f 5072 6554  ..r:...z6P2_PreT
+000092c0: 7572 6e5f 3250 5f56 6965 772e 5f5f 696e  urn_2P_View.__in
+000092d0: 6974 5f5f 2e3c 6c6f 6361 6c73 3e2e 6f6e  it__.<locals>.on
+000092e0: 5f63 6c69 636b 5f53 6574 7469 6e67 7363  _click_Settingsc
+000092f0: 0100 0000 0000 0000 0000 0000 0200 0000  ................
+00009300: 0500 0000 1300 0000 7266 0100 0029 054e  ........rf...).N
+00009310: 7298 0000 0072 1d00 0000 4672 9900 0000  r....r....Fr....
+00009320: 290a 7203 0000 0072 a600 0000 7220 0000  ).r....r....r ..
+00009330: 0072 a700 0000 7229 0100 0072 2100 0000  .r....r)...r!...
+00009340: 722a 0100 0072 5d01 0000 7225 0000 0072  r*...r]...r%...r
+00009350: 2600 0000 725f 0100 0072 2900 0000 722b  &...r_...r)...r+
+00009360: 0000 0072 2c00 0000 722f 0100 0019 0500  ...r,...r/......
+00009370: 0072 6701 0000 7a32 5032 5f50 7265 5475  .rg...z2P2_PreTu
+00009380: 726e 5f32 505f 5669 6577 2e5f 5f69 6e69  rn_2P_View.__ini
+00009390: 745f 5f2e 3c6c 6f63 616c 733e 2e6f 6e5f  t__.<locals>.on_
+000093a0: 636c 6963 6b5f 726f 6c6c 7230 0100 0072  click_rollr0...r
+000093b0: 6801 0000 724f 0000 0072 2900 0000 722c  h...rO...r)...r,
+000093c0: 0000 0072 4300 0000 f804 0000 7269 0100  ...rC.......ri..
+000093d0: 007a 1b50 325f 5072 6554 7572 6e5f 3250  .z.P2_PreTurn_2P
+000093e0: 5f56 6965 772e 5f5f 696e 6974 5f5f 6301  _View.__init__c.
+000093f0: 0000 0000 0000 0000 0000 0001 0000 0003  ................
+00009400: 0000 0043 0000 0072 5100 0000 7231 0000  ...C...rQ...r1..
+00009410: 0072 5200 0000 7229 0000 0072 2b00 0000  .rR...r)...r+...
+00009420: 722b 0000 0072 2c00 0000 7254 0000 0022  r+...r,...rT..."
+00009430: 0500 0072 5500 0000 7a1f 5032 5f50 7265  ...rU...z.P2_Pre
+00009440: 5475 726e 5f32 505f 5669 6577 2e6f 6e5f  Turn_2P_View.on_
+00009450: 7368 6f77 5f76 6965 7763 0100 0000 0000  show_viewc......
+00009460: 0000 0000 0000 0100 0000 0200 0000 4300  ..............C.
+00009470: 0000 7256 0000 0072 3100 0000 7257 0000  ..rV...r1...rW..
+00009480: 0072 2900 0000 722b 0000 0072 2b00 0000  .r)...r+...r+...
+00009490: 722c 0000 0072 5900 0000 2605 0000 725a  r,...rY...&...rZ
+000094a0: 0000 007a 1f50 325f 5072 6554 7572 6e5f  ...z.P2_PreTurn_
+000094b0: 3250 5f56 6965 772e 6f6e 5f68 6964 655f  2P_View.on_hide_
+000094c0: 7669 6577 6301 0000 0000 0000 0000 0000  viewc...........
+000094d0: 0001 0000 0007 0000 0043 0000 0072 6a01  .........C...rj.
+000094e0: 0000 725b 0100 0029 0d72 5d00 0000 7246  ..r[...).r]...rF
+000094f0: 0000 0072 5e00 0000 7204 0000 0072 d100  ...r^...r....r..
+00009500: 0000 723d 0000 0072 2001 0000 7264 0100  ..r=...r ...rd..
+00009510: 0072 d200 0000 7220 0000 0072 2100 0000  .r....r ...r!...
+00009520: 72d3 0000 0072 ab00 0000 7229 0000 0072  r....r....r)...r
+00009530: 2b00 0000 722b 0000 0072 2c00 0000 725f  +...r+...r,...r_
+00009540: 0000 0029 0500 0072 6b01 0000 7a1a 5032  ...)...rk...z.P2
+00009550: 5f50 7265 5475 726e 5f32 505f 5669 6577  _PreTurn_2P_View
+00009560: 2e6f 6e5f 6472 6177 7261 0000 0072 2b00  .on_drawra...r+.
+00009570: 0000 722b 0000 0072 4f00 0000 722c 0000  ..r+...rO...r,..
+00009580: 0072 5e01 0000 f604 0000 726c 0100 0072  .r^.......rl...r
+00009590: 5e01 0000 6300 0000 0000 0000 0000 0000  ^...c...........
+000095a0: 0000 0000 0003 0000 0000 0000 0072 0500  .............r..
+000095b0: 0000 2909 da10 4761 6d65 4f76 6572 5f32  ..)...GameOver_2
+000095c0: 505f 5669 6577 6302 0000 0000 0000 0000  P_Viewc.........
+000095d0: 0000 0003 0000 0007 0000 0003 0000 0073  ...............s
+000095e0: 4a00 0000 7400 8300 a001 a100 0100 7c01  J...t.........|.
+000095f0: 7c00 5f02 7403 6a04 a005 a100 7c00 5f06  |._.t.j.....|._.
+00009600: 7c00 6a06 a007 a100 0100 7403 6a04 a008  |.j.......t.j...
+00009610: 6401 6402 6403 6404 6405 a105 7d02 7c00  d.d.d.d.d...}.|.
+00009620: 6a06 a009 7c02 a101 0100 6400 5300 2906  j...|.....d.S.).
+00009630: 4e72 1201 0000 7275 0000 0072 6600 0000  Nr....ru...rf...
+00009640: 7272 0000 0072 6f00 0000 290a 7242 0000  rr...ro...).rB..
+00009650: 0072 4300 0000 7225 0000 0072 3d00 0000  .rC...r%...r=...
+00009660: 7244 0000 0072 4500 0000 7246 0000 0072  rD...rE...rF...r
+00009670: 4700 0000 724c 0000 0072 4a00 0000 2903  G...rL...rJ...).
+00009680: 722a 0000 0072 4e00 0000 5a0b 6261 636b  r*...rN...Z.back
+00009690: 5f62 7574 746f 6e72 4f00 0000 722b 0000  _buttonrO...r+..
+000096a0: 0072 2c00 0000 7243 0000 0033 0500 0073  .r,...rC...3...s
+000096b0: 0c00 0000 0a01 0601 0c02 0a01 1402 1002  ................
+000096c0: 7a19 4761 6d65 4f76 6572 5f32 505f 5669  z.GameOver_2P_Vi
+000096d0: 6577 2e5f 5f69 6e69 745f 5f63 0100 0000  ew.__init__c....
+000096e0: 0000 0000 0000 0000 0100 0000 0300 0000  ................
+000096f0: 4300 0000 7251 0000 0072 3100 0000 7252  C...rQ...r1...rR
+00009700: 0000 0072 2900 0000 722b 0000 0072 2b00  ...r)...r+...r+.
+00009710: 0000 722c 0000 0072 5400 0000 3e05 0000  ..r,...rT...>...
+00009720: 7255 0000 007a 1d47 616d 654f 7665 725f  rU...z.GameOver_
+00009730: 3250 5f56 6965 772e 6f6e 5f73 686f 775f  2P_View.on_show_
+00009740: 7669 6577 6301 0000 0000 0000 0000 0000  viewc...........
+00009750: 0001 0000 0002 0000 0043 0000 0072 5600  .........C...rV.
+00009760: 0000 7231 0000 0072 5700 0000 7229 0000  ..r1...rW...r)..
+00009770: 0072 2b00 0000 722b 0000 0072 2c00 0000  .r+...r+...r,...
+00009780: 7259 0000 0042 0500 0072 5a00 0000 7a1d  rY...B...rZ...z.
+00009790: 4761 6d65 4f76 6572 5f32 505f 5669 6577  GameOver_2P_View
+000097a0: 2e6f 6e5f 6869 6465 5f76 6965 7763 0100  .on_hide_viewc..
+000097b0: 0000 0000 0000 0000 0000 0100 0000 0200  ................
+000097c0: 0000 4300 0000 725b 0000 0072 3100 0000  ..C...r[...r1...
+000097d0: 725c 0000 0072 2900 0000 722b 0000 0072  r\...r)...r+...r
+000097e0: 2b00 0000 722c 0000 0072 5f00 0000 4505  +...r,...r_...E.
+000097f0: 0000 7260 0000 007a 1847 616d 654f 7665  ..r`...z.GameOve
+00009800: 725f 3250 5f56 6965 772e 6f6e 5f64 7261  r_2P_View.on_dra
+00009810: 7772 6100 0000 722b 0000 0072 2b00 0000  wra...r+...r+...
+00009820: 724f 0000 0072 2c00 0000 726d 0100 0031  rO...r,...rm...1
+00009830: 0500 0073 0a00 0000 0800 0c02 080b 0804  ...s............
+00009840: 1003 726d 0100 0029 1872 3d00 0000 da0a  ..rm...).r=.....
+00009850: 6172 6361 6465 2e67 7569 72a4 0000 00da  arcade.guir.....
+00009860: 0a4d 6169 6e5f 4669 6c65 7372 0200 0000  .Main_Filesr....
+00009870: 7203 0000 0072 0400 0000 da13 4d6f 6475  r....r......Modu
+00009880: 6c65 4e6f 7446 6f75 6e64 4572 726f 72da  leNotFoundError.
+00009890: 1c77 696c 6c73 655f 6261 636b 6761 6d6d  .willse_backgamm
+000098a0: 6f6e 2e4d 6169 6e5f 4669 6c65 73da 0456  on.Main_Files..V
+000098b0: 6965 7772 0600 0000 7237 0000 0072 2400  iewr....r7...r$.
+000098c0: 0000 72c0 0000 0072 ed00 0000 722e 0000  ..r....r....r...
+000098d0: 0072 2b01 0000 722c 0100 0072 3200 0000  .r+...r,...r2...
+000098e0: 725c 0100 0072 5d01 0000 7263 0100 0072  r\...r]...rc...r
+000098f0: 5e01 0000 726d 0100 0072 2b00 0000 722b  ^...rm...r+...r+
+00009900: 0000 0072 2b00 0000 722c 0000 00da 083c  ...r+...r,.....<
+00009910: 6d6f 6475 6c65 3e01 0000 0073 3a00 0000  module>....s:...
+00009920: 0800 0801 0801 0202 0c01 0c01 1001 0c01  ................
+00009930: 0c01 0c01 1001 02fd 1206 124c 007f 120a  ...........L....
+00009940: 007f 1272 007f 124e 1239 1243 1266 1248  ...r...N.9.C.f.H
+00009950: 123f 1258 1258 123b 163b                 .?.X.X.;.;
```

### Comparing `willse_backgammon-0.0.1/src/willse_backgammon/Manual.py` & `willse_backgammon-0.0.2/src/willse_backgammon/Manual.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,13 @@
 import multiprocessing
 import random
 import time
+import numpy as np
+import pandas as pd
+import pathlib
 
 try:
     from Main_Files import AI as AI
     from Main_Files import Logic as Logic
 except ModuleNotFoundError:
     from willse_backgammon.Main_Files import Logic as Logic
     from willse_backgammon.Main_Files import AI as AI
@@ -133,15 +136,40 @@
 
 
 def TestAIMoveUpdates(Board: Logic.Board, player, roll):
     Turn = Logic.Turn(player, "AI", None, roll=roll)
     Turn.updatePossibleMovesAI(Board, player)
     print(f"PossibleMoves = {Turn.current_possible_moves}")
 
+def test():
+    df = pd.read_csv("willse_backgammon/AI_Agents/Data_Sets/data_set_1.csv")
+    data = np.array(df)
+
+    print(df.head()) 
+    print(data.shape)
+    
+    m, n = data.shape
+    np.random.shuffle(data)
+
+    data_dev = data[0:1000].T
+    Y_dev = data_dev[2]
+    Y_dev = Y_dev.strip("][").split(", ")
+    print(Y_dev.shape)
+    X_dev = data_dev[1]
+    print(X_dev.shape)
+    X_dev = X_dev / 255.0
+
+    data_train = data[1000:m].T
+    Y_train = data_train[0]
+    X_train = data_train[1:n]
+    X_train = X_train / 255.0
+
+
+
 
 Board = Logic.Board()
 
 ##### Current Test Code #####
 
 if __name__ == "__main__":
-    pass
+    test()
     # RunGamesMulti("Network", "TS1", 1000, netIdent1="V1.0-NVT-A1-100", netIdent2="V1.0-NVT-A600")
```

### Comparing `willse_backgammon-0.0.1/src/willse_backgammon/Network.py` & `willse_backgammon-0.0.2/src/willse_backgammon/Network.py`

 * *Files identical despite different names*

### Comparing `willse_backgammon-0.0.1/src/willse_backgammon.egg-info/PKG-INFO` & `willse_backgammon-0.0.2/src/willse_backgammon.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 Metadata-Version: 2.1
 Name: willse_backgammon
-Version: 0.0.1
+Version: 0.0.2
 Summary: This package is a project I have created to learn python as well as the basics of Artificial Intelligence. It is still a Work in Progress.
 Author-email: Wills Erda <willse06@gmail.com>
 Project-URL: Homepage, https://github.com/GillsSpace/Backgammon_AI
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Requires-Dist: arcade
 Requires-Dist: numpy
+Requires-Dist: pandas
 
 
 # willse_backgammon
 
 This project was created my me to practice and improve my python skils and to learn about nureal networks and machine learning. It is very much still a work in progress.
 
 
@@ -24,21 +25,21 @@
 
 ```bash
   pip install willse_backgammon
 ```
     
 ## Run Locally
 
-After Intsallation, you can run the main application with the following command from terminal:
+After Installation, you can run the main application with the following command from terminal:
 
 ```bash
   > willse_backgammon_run
 ```
 
 
 ## Features
 
 - Two Player, Single Player, and Simulation Modes
-- Multiple AI modles
-- Currently v0.0.1
+- Multiple AI models
+- Currently v0.0.2
```

### Comparing `willse_backgammon-0.0.1/src/willse_backgammon.egg-info/SOURCES.txt` & `willse_backgammon-0.0.2/src/willse_backgammon.egg-info/SOURCES.txt`

 * *Files identical despite different names*

