# Comparing `tmp/bia-ia-0.0.2.tar.gz` & `tmp/bia-ia-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, last modified: Tue Apr  2 21:47:59 2024, from Unix
+gzip compressed data, last modified: Tue Apr  2 21:57:37 2024, from Unix
```

## Comparing `bia-ia-0.0.2.tar` & `bia-ia-0.0.3.tar`

### file list

```diff
@@ -1,112 +1,134 @@
-drwxr-xr-x   0 tylerdddd   (501) staff       (20)        0 2024-04-02 21:45:04.000000 bia-ia-0.0.2/
--rw-r--r--   0 tylerdddd   (501) staff       (20)      692 2024-04-02 21:44:14.000000 bia-ia-0.0.2/PKG-INFO
-drwxr-xr-x   0 tylerdddd   (501) staff       (20)        0 2024-04-02 21:44:14.000000 bia-ia-0.0.2/bia_ia.egg-info/
-drwxr-xr-x   0 tylerdddd   (501) staff       (20)        0 2024-04-02 21:46:37.000000 bia-ia-0.0.2/bia-ia/
--rw-r--r--   0 tylerdddd   (501) staff       (20)     1391 2024-04-02 21:44:11.000000 bia-ia-0.0.2/setup.py
--rw-r--r--   0 tylerdddd   (501) staff       (20)       38 2024-04-02 21:44:14.000000 bia-ia-0.0.2/setup.cfg
--rw-r--r--   0 tylerdddd   (501) staff       (20)     1184 2024-04-02 21:16:33.000000 bia-ia-0.0.2/bia-ia/bia.py
--rw-r--r--   0 tylerdddd   (501) staff       (20)      122 2024-04-02 21:16:33.000000 bia-ia-0.0.2/bia-ia/__init__.py
-drwxr-xr-x   0 tylerdddd   (501) staff       (20)        0 2024-04-02 21:46:05.000000 bia-ia-0.0.2/bia-ia/utils/
-drwxr-xr-x   0 tylerdddd   (501) staff       (20)        0 2024-04-02 21:44:14.000000 bia-ia-0.0.2/bia-ia/models/
-drwxr-xr-x   0 tylerdddd   (501) staff       (20)        0 2024-04-02 21:44:14.000000 bia-ia-0.0.2/bia-ia/controllers/
-drwxr-xr-x   0 tylerdddd   (501) staff       (20)        0 2024-04-02 21:44:49.000000 bia-ia-0.0.2/bia-ia/data/
-drwxr-xr-x   0 tylerdddd   (501) staff       (20)        0 2024-04-02 21:44:14.000000 bia-ia-0.0.2/bia-ia/views/
--rw-r--r--   0 tylerdddd   (501) staff       (20)      373 2024-04-02 21:16:33.000000 bia-ia-0.0.2/bia-ia/views/ui.py
--rw-r--r--   0 tylerdddd   (501) staff       (20)     8738 2024-04-02 21:16:33.000000 bia-ia-0.0.2/bia-ia/views/app.py
--rw-r--r--   0 tylerdddd   (501) staff       (20)      120 2024-04-02 21:44:49.000000 bia-ia-0.0.2/bia-ia/data/._.DS_Store
--rw-r--r--   0 tylerdddd   (501) staff       (20)     6148 2024-04-02 21:44:49.770172 bia-ia-0.0.2/bia-ia/data/.DS_Store
-drwxr-xr-x   0 tylerdddd   (501) staff       (20)        0 2024-04-02 21:44:49.000000 bia-ia-0.0.2/bia-ia/data/python/
-drwxr-xr-x   0 tylerdddd   (501) staff       (20)        0 2024-04-02 21:44:49.000000 bia-ia-0.0.2/bia-ia/data/camera/
--rw-r--r--   0 tylerdddd   (501) staff       (20)      220 2024-04-02 21:44:49.000000 bia-ia-0.0.2/bia-ia/data/.__bia.db
--rw-r--r--   0 tylerdddd   (501) staff       (20)   147456 2024-04-02 21:44:49.773155 bia-ia-0.0.2/bia-ia/data/_bia.db
-drwxr-xr-x   0 tylerdddd   (501) staff       (20)        0 2024-04-02 21:44:49.000000 bia-ia-0.0.2/bia-ia/data/arduino/
-drwxr-xr-x   0 tylerdddd   (501) staff       (20)        0 2024-04-02 21:44:49.000000 bia-ia-0.0.2/bia-ia/data/logs/
--rw-r--r--   0 tylerdddd   (501) staff       (20)      276 2024-04-02 21:44:49.000000 bia-ia-0.0.2/bia-ia/data/._bia.db
--rw-r--r--   0 tylerdddd   (501) staff       (20)   147456 2024-04-02 21:44:49.784264 bia-ia-0.0.2/bia-ia/data/bia.db
--rw-r--r--   0 tylerdddd   (501) staff       (20)        0 2024-04-02 21:44:49.000000 bia-ia-0.0.2/bia-ia/data/logs/bia_2024_03_24_03_09_.log
--rw-r--r--   0 tylerdddd   (501) staff       (20)        0 2024-04-02 21:44:49.000000 bia-ia-0.0.2/bia-ia/data/logs/bia_2024_03_24_09_30_.log
--rw-r--r--   0 tylerdddd   (501) staff       (20)     2017 2024-04-02 21:44:49.000000 bia-ia-0.0.2/bia-ia/data/logs/bia_2024_03_24_10_51_.log
--rw-r--r--   0 tylerdddd   (501) staff       (20)      416 2024-04-02 21:44:49.000000 bia-ia-0.0.2/bia-ia/data/logs/bia_2024_03_24_09_10_.log
--rw-r--r--   0 tylerdddd   (501) staff       (20)      406 2024-04-02 21:44:49.000000 bia-ia-0.0.2/bia-ia/data/logs/bia_2024_03_25_09_04_.log
--rw-r--r--   0 tylerdddd   (501) staff       (20)      220 2024-04-02 21:44:49.000000 bia-ia-0.0.2/bia-ia/data/logs/._bia_2024_03_25_08_53_.log
--rw-r--r--   0 tylerdddd   (501) staff       (20)        0 2024-04-02 21:44:49.783509 bia-ia-0.0.2/bia-ia/data/logs/bia_2024_03_25_08_53_.log
--rw-r--r--   0 tylerdddd   (501) staff       (20)      441 2024-04-02 21:44:49.000000 bia-ia-0.0.2/bia-ia/data/logs/bia_2024_03_24_01_37_.log
--rw-r--r--   0 tylerdddd   (501) staff       (20)    19665 2024-04-02 21:44:49.000000 bia-ia-0.0.2/bia-ia/data/logs/bia_2024_03_24_03_06_.log
-drwxr-xr-x   0 tylerdddd   (501) staff       (20)        0 2024-04-02 21:44:49.000000 bia-ia-0.0.2/bia-ia/data/arduino/20240324_150726/
-drwxr-xr-x   0 tylerdddd   (501) staff       (20)        0 2024-04-02 21:44:49.000000 bia-ia-0.0.2/bia-ia/data/arduino/20240324_105329/
-drwxr-xr-x   0 tylerdddd   (501) staff       (20)        0 2024-04-02 21:44:49.000000 bia-ia-0.0.2/bia-ia/data/arduino/20240324_110209/
-drwxr-xr-x   0 tylerdddd   (501) staff       (20)        0 2024-04-02 21:44:49.000000 bia-ia-0.0.2/bia-ia/data/arduino/20240324_150807/
--rw-r--r--   0 tylerdddd   (501) staff       (20)      120 2024-04-02 21:44:49.000000 bia-ia-0.0.2/bia-ia/data/arduino/._.DS_Store
--rw-r--r--   0 tylerdddd   (501) staff       (20)     6148 2024-04-02 21:44:49.776050 bia-ia-0.0.2/bia-ia/data/arduino/.DS_Store
-drwxr-xr-x   0 tylerdddd   (501) staff       (20)        0 2024-04-02 21:44:49.000000 bia-ia-0.0.2/bia-ia/data/arduino/20240324_110918/
-drwxr-xr-x   0 tylerdddd   (501) staff       (20)        0 2024-04-02 21:44:49.000000 bia-ia-0.0.2/bia-ia/data/arduino/20240324_151148/
-drwxr-xr-x   0 tylerdddd   (501) staff       (20)        0 2024-04-02 21:44:49.000000 bia-ia-0.0.2/bia-ia/data/arduino/20240324_111016/
-drwxr-xr-x   0 tylerdddd   (501) staff       (20)        0 2024-04-02 21:44:49.000000 bia-ia-0.0.2/bia-ia/data/arduino/20240324_150841/
-drwxr-xr-x   0 tylerdddd   (501) staff       (20)        0 2024-04-02 21:44:49.000000 bia-ia-0.0.2/bia-ia/data/arduino/20240324_110240/
-drwxr-xr-x   0 tylerdddd   (501) staff       (20)        0 2024-04-02 21:44:49.000000 bia-ia-0.0.2/bia-ia/data/arduino/20240324_105359/
-drwxr-xr-x   0 tylerdddd   (501) staff       (20)        0 2024-04-02 21:44:49.000000 bia-ia-0.0.2/bia-ia/data/arduino/20240324_105203/
-drwxr-xr-x   0 tylerdddd   (501) staff       (20)        0 2024-04-02 21:44:49.000000 bia-ia-0.0.2/bia-ia/data/arduino/20240324_110952/
-drwxr-xr-x   0 tylerdddd   (501) staff       (20)        0 2024-04-02 21:44:49.000000 bia-ia-0.0.2/bia-ia/data/arduino/20240324_105738/
-drwxr-xr-x   0 tylerdddd   (501) staff       (20)        0 2024-04-02 21:44:49.000000 bia-ia-0.0.2/bia-ia/data/arduino/20240324_111301/
--rw-r--r--   0 tylerdddd   (501) staff       (20)      430 2024-04-02 21:44:49.000000 bia-ia-0.0.2/bia-ia/data/arduino/20240324_111301/20240324_111301.ino
--rw-r--r--   0 tylerdddd   (501) staff       (20)      176 2024-04-02 21:44:49.000000 bia-ia-0.0.2/bia-ia/data/arduino/20240324_105738/._20240324_105738.ino
--rw-r--r--   0 tylerdddd   (501) staff       (20)     1971 2024-04-02 21:44:49.781433 bia-ia-0.0.2/bia-ia/data/arduino/20240324_105738/20240324_105738.ino
--rw-r--r--   0 tylerdddd   (501) staff       (20)      376 2024-04-02 21:44:49.000000 bia-ia-0.0.2/bia-ia/data/arduino/20240324_110952/20240324_110952.ino
--rw-r--r--   0 tylerdddd   (501) staff       (20)      176 2024-04-02 21:44:49.000000 bia-ia-0.0.2/bia-ia/data/arduino/20240324_105203/._20240324_105203.ino
--rw-r--r--   0 tylerdddd   (501) staff       (20)      412 2024-04-02 21:44:49.780150 bia-ia-0.0.2/bia-ia/data/arduino/20240324_105203/20240324_105203.ino
--rw-r--r--   0 tylerdddd   (501) staff       (20)      176 2024-04-02 21:44:49.000000 bia-ia-0.0.2/bia-ia/data/arduino/20240324_105359/._20240324_105359.ino
--rw-r--r--   0 tylerdddd   (501) staff       (20)      429 2024-04-02 21:44:49.779479 bia-ia-0.0.2/bia-ia/data/arduino/20240324_105359/20240324_105359.ino
--rw-r--r--   0 tylerdddd   (501) staff       (20)      176 2024-04-02 21:44:49.000000 bia-ia-0.0.2/bia-ia/data/arduino/20240324_110240/._20240324_110240.ino
--rw-r--r--   0 tylerdddd   (501) staff       (20)      400 2024-04-02 21:44:49.778909 bia-ia-0.0.2/bia-ia/data/arduino/20240324_110240/20240324_110240.ino
--rw-r--r--   0 tylerdddd   (501) staff       (20)      404 2024-04-02 21:44:49.000000 bia-ia-0.0.2/bia-ia/data/arduino/20240324_150841/20240324_150841.ino
--rw-r--r--   0 tylerdddd   (501) staff       (20)      401 2024-04-02 21:44:49.000000 bia-ia-0.0.2/bia-ia/data/arduino/20240324_111016/20240324_111016.ino
--rw-r--r--   0 tylerdddd   (501) staff       (20)      537 2024-04-02 21:44:49.000000 bia-ia-0.0.2/bia-ia/data/arduino/20240324_151148/20240324_151148.ino
--rw-r--r--   0 tylerdddd   (501) staff       (20)      377 2024-04-02 21:44:49.000000 bia-ia-0.0.2/bia-ia/data/arduino/20240324_110918/20240324_110918.ino
--rw-r--r--   0 tylerdddd   (501) staff       (20)      398 2024-04-02 21:44:49.000000 bia-ia-0.0.2/bia-ia/data/arduino/20240324_150807/20240324_150807.ino
--rw-r--r--   0 tylerdddd   (501) staff       (20)      176 2024-04-02 21:44:49.000000 bia-ia-0.0.2/bia-ia/data/arduino/20240324_110209/._20240324_110209.ino
--rw-r--r--   0 tylerdddd   (501) staff       (20)      504 2024-04-02 21:44:49.775096 bia-ia-0.0.2/bia-ia/data/arduino/20240324_110209/20240324_110209.ino
--rw-r--r--   0 tylerdddd   (501) staff       (20)      376 2024-04-02 21:44:49.000000 bia-ia-0.0.2/bia-ia/data/arduino/20240324_105329/20240324_105329.ino
--rw-r--r--   0 tylerdddd   (501) staff       (20)     1730 2024-04-02 21:44:49.000000 bia-ia-0.0.2/bia-ia/data/arduino/20240324_150726/20240324_150726.ino
--rw-r--r--   0 tylerdddd   (501) staff       (20)   306118 2024-04-02 21:44:49.000000 bia-ia-0.0.2/bia-ia/data/camera/20240323_095157.jpg
--rw-r--r--   0 tylerdddd   (501) staff       (20)      120 2024-04-02 21:44:49.000000 bia-ia-0.0.2/bia-ia/data/python/._.DS_Store
--rw-r--r--   0 tylerdddd   (501) staff       (20)     6148 2024-04-02 21:44:49.771313 bia-ia-0.0.2/bia-ia/data/python/.DS_Store
--rw-r--r--   0 tylerdddd   (501) staff       (20)     2780 2024-04-02 21:16:33.000000 bia-ia-0.0.2/bia-ia/controllers/action.py
--rw-r--r--   0 tylerdddd   (501) staff       (20)     1332 2024-04-02 21:16:33.000000 bia-ia-0.0.2/bia-ia/controllers/asynch.py
--rw-r--r--   0 tylerdddd   (501) staff       (20)     2937 2024-04-02 21:16:33.000000 bia-ia-0.0.2/bia-ia/controllers/base.py
-drwxr-xr-x   0 tylerdddd   (501) staff       (20)        0 2024-04-02 21:44:14.000000 bia-ia-0.0.2/bia-ia/models/blocks/
-drwxr-xr-x   0 tylerdddd   (501) staff       (20)        0 2024-04-02 21:44:14.000000 bia-ia-0.0.2/bia-ia/models/database/
-drwxr-xr-x   0 tylerdddd   (501) staff       (20)        0 2024-04-02 21:44:14.000000 bia-ia-0.0.2/bia-ia/models/speech/
-drwxr-xr-x   0 tylerdddd   (501) staff       (20)        0 2024-04-02 21:44:14.000000 bia-ia-0.0.2/bia-ia/models/robot/
-drwxr-xr-x   0 tylerdddd   (501) staff       (20)        0 2024-04-02 21:44:14.000000 bia-ia-0.0.2/bia-ia/models/openAI/
--rw-r--r--   0 tylerdddd   (501) staff       (20)     1553 2024-04-02 21:16:33.000000 bia-ia-0.0.2/bia-ia/models/openAI/ai.py
--rw-r--r--   0 tylerdddd   (501) staff       (20)     4602 2024-04-02 21:16:33.000000 bia-ia-0.0.2/bia-ia/models/robot/robot.py
--rw-r--r--   0 tylerdddd   (501) staff       (20)     5890 2024-04-02 21:16:33.000000 bia-ia-0.0.2/bia-ia/models/speech/prompt.py
--rw-r--r--   0 tylerdddd   (501) staff       (20)     1583 2024-04-02 21:16:33.000000 bia-ia-0.0.2/bia-ia/models/database/grandma.py
--rw-r--r--   0 tylerdddd   (501) staff       (20)     1041 2024-04-02 21:16:33.000000 bia-ia-0.0.2/bia-ia/models/database/mia_utils.py
--rw-r--r--   0 tylerdddd   (501) staff       (20)     7012 2024-04-02 21:16:33.000000 bia-ia-0.0.2/bia-ia/models/database/mia.py
--rw-r--r--   0 tylerdddd   (501) staff       (20)     1169 2024-04-02 21:16:33.000000 bia-ia-0.0.2/bia-ia/models/blocks/netflix.py
--rw-r--r--   0 tylerdddd   (501) staff       (20)     1040 2024-04-02 21:16:33.000000 bia-ia-0.0.2/bia-ia/models/blocks/web.py
--rw-r--r--   0 tylerdddd   (501) staff       (20)     1181 2024-04-02 21:16:33.000000 bia-ia-0.0.2/bia-ia/models/blocks/youtube.py
--rw-r--r--   0 tylerdddd   (501) staff       (20)      867 2024-04-02 21:16:33.000000 bia-ia-0.0.2/bia-ia/models/blocks/display.py
--rw-r--r--   0 tylerdddd   (501) staff       (20)      923 2024-04-02 21:16:33.000000 bia-ia-0.0.2/bia-ia/models/blocks/default.py
--rw-r--r--   0 tylerdddd   (501) staff       (20)     1622 2024-04-02 21:16:33.000000 bia-ia-0.0.2/bia-ia/models/blocks/camera.py
--rw-r--r--   0 tylerdddd   (501) staff       (20)      860 2024-04-02 21:16:33.000000 bia-ia-0.0.2/bia-ia/models/blocks/alexa.py
--rw-r--r--   0 tylerdddd   (501) staff       (20)     2292 2024-04-02 21:16:33.000000 bia-ia-0.0.2/bia-ia/models/blocks/python.py
--rw-r--r--   0 tylerdddd   (501) staff       (20)     1141 2024-04-02 21:16:33.000000 bia-ia-0.0.2/bia-ia/models/blocks/tv.py
--rw-r--r--   0 tylerdddd   (501) staff       (20)     1158 2024-04-02 21:16:33.000000 bia-ia-0.0.2/bia-ia/models/blocks/radio.py
--rw-r--r--   0 tylerdddd   (501) staff       (20)      880 2024-04-02 21:16:33.000000 bia-ia-0.0.2/bia-ia/models/blocks/block.py
--rw-r--r--   0 tylerdddd   (501) staff       (20)      879 2024-04-02 21:16:33.000000 bia-ia-0.0.2/bia-ia/models/blocks/macro.py
--rw-r--r--   0 tylerdddd   (501) staff       (20)     2588 2024-04-02 21:16:33.000000 bia-ia-0.0.2/bia-ia/models/blocks/arduino.py
--rw-r--r--   0 tylerdddd   (501) staff       (20)     1299 2024-04-02 21:16:33.000000 bia-ia-0.0.2/bia-ia/utils/lang.py
--rw-r--r--   0 tylerdddd   (501) staff       (20)    10394 2024-04-02 21:16:33.000000 bia-ia-0.0.2/bia-ia/utils/config.py
--rw-r--r--   0 tylerdddd   (501) staff       (20)     2431 2024-04-02 21:46:05.000000 bia-ia-0.0.2/bia-ia/utils/_config.cfg
--rw-r--r--   0 tylerdddd   (501) staff       (20)     2424 2024-04-02 21:46:05.000000 bia-ia-0.0.2/bia-ia/utils/config.cfg
--rw-r--r--   0 tylerdddd   (501) staff       (20)     1783 2024-04-02 21:16:33.000000 bia-ia-0.0.2/bia-ia/utils/text2Speech.py
--rw-r--r--   0 tylerdddd   (501) staff       (20)     1817 2024-04-02 21:16:33.000000 bia-ia-0.0.2/bia-ia/utils/debug.py
--rw-r--r--   0 tylerdddd   (501) staff       (20)     2481 2024-04-02 21:16:33.000000 bia-ia-0.0.2/bia-ia/utils/speech2Text.py
--rw-r--r--   0 tylerdddd   (501) staff       (20)     1411 2024-04-02 21:16:33.000000 bia-ia-0.0.2/bia-ia/utils/paraphrase.py
--rw-r--r--   0 tylerdddd   (501) staff       (20)      692 2024-04-02 21:44:14.000000 bia-ia-0.0.2/bia_ia.egg-info/PKG-INFO
--rw-r--r--   0 tylerdddd   (501) staff       (20)     1047 2024-04-02 21:44:14.000000 bia-ia-0.0.2/bia_ia.egg-info/SOURCES.txt
--rw-r--r--   0 tylerdddd   (501) staff       (20)      149 2024-04-02 21:44:14.000000 bia-ia-0.0.2/bia_ia.egg-info/requires.txt
--rw-r--r--   0 tylerdddd   (501) staff       (20)        7 2024-04-02 21:44:14.000000 bia-ia-0.0.2/bia_ia.egg-info/top_level.txt
--rw-r--r--   0 tylerdddd   (501) staff       (20)        1 2024-04-02 21:44:14.000000 bia-ia-0.0.2/bia_ia.egg-info/dependency_links.txt
+drwxr-xr-x   0 tylerdddd   (501) staff       (20)        0 2024-04-02 21:56:22.000000 bia-ia-0.0.3/
+-rw-r--r--   0 tylerdddd   (501) staff       (20)      692 2024-04-02 21:56:22.000000 bia-ia-0.0.3/PKG-INFO
+drwxr-xr-x   0 tylerdddd   (501) staff       (20)        0 2024-04-02 21:52:29.000000 bia-ia-0.0.3/bia_ia.egg-info/
+drwxr-xr-x   0 tylerdddd   (501) staff       (20)        0 2024-04-02 21:54:25.000000 bia-ia-0.0.3/bia-ia/
+-rw-r--r--   0 tylerdddd   (501) staff       (20)     1391 2024-04-02 21:56:08.000000 bia-ia-0.0.3/setup.py
+-rw-r--r--   0 tylerdddd   (501) staff       (20)       38 2024-04-02 21:52:29.000000 bia-ia-0.0.3/setup.cfg
+-rw-r--r--   0 tylerdddd   (501) staff       (20)     1184 2024-04-02 21:16:33.000000 bia-ia-0.0.3/bia-ia/bia.py
+drwxr-xr-x   0 tylerdddd   (501) staff       (20)        0 2024-04-02 21:53:53.000000 bia-ia-0.0.3/bia-ia/deploy/
+-rw-r--r--   0 tylerdddd   (501) staff       (20)      122 2024-04-02 21:16:33.000000 bia-ia-0.0.3/bia-ia/__init__.py
+drwxr-xr-x   0 tylerdddd   (501) staff       (20)        0 2024-04-02 21:55:18.000000 bia-ia-0.0.3/bia-ia/utils/
+drwxr-xr-x   0 tylerdddd   (501) staff       (20)        0 2024-04-02 21:52:29.000000 bia-ia-0.0.3/bia-ia/models/
+drwxr-xr-x   0 tylerdddd   (501) staff       (20)        0 2024-04-02 21:52:29.000000 bia-ia-0.0.3/bia-ia/controllers/
+drwxr-xr-x   0 tylerdddd   (501) staff       (20)        0 2024-04-02 21:54:25.000000 bia-ia-0.0.3/bia-ia/data/
+drwxr-xr-x   0 tylerdddd   (501) staff       (20)        0 2024-04-02 21:52:29.000000 bia-ia-0.0.3/bia-ia/views/
+-rw-r--r--   0 tylerdddd   (501) staff       (20)      373 2024-04-02 21:16:33.000000 bia-ia-0.0.3/bia-ia/views/ui.py
+-rw-r--r--   0 tylerdddd   (501) staff       (20)     8738 2024-04-02 21:16:33.000000 bia-ia-0.0.3/bia-ia/views/app.py
+-rw-r--r--   0 tylerdddd   (501) staff       (20)      120 2024-04-02 21:54:25.000000 bia-ia-0.0.3/bia-ia/data/._.DS_Store
+-rw-r--r--   0 tylerdddd   (501) staff       (20)     6148 2024-04-02 21:54:25.238843 bia-ia-0.0.3/bia-ia/data/.DS_Store
+drwxr-xr-x   0 tylerdddd   (501) staff       (20)        0 2024-04-02 21:54:25.000000 bia-ia-0.0.3/bia-ia/data/python/
+drwxr-xr-x   0 tylerdddd   (501) staff       (20)        0 2024-04-02 21:54:25.000000 bia-ia-0.0.3/bia-ia/data/camera/
+-rw-r--r--   0 tylerdddd   (501) staff       (20)      220 2024-04-02 21:54:25.000000 bia-ia-0.0.3/bia-ia/data/.__bia.db
+-rw-r--r--   0 tylerdddd   (501) staff       (20)   147456 2024-04-02 21:54:25.242977 bia-ia-0.0.3/bia-ia/data/_bia.db
+drwxr-xr-x   0 tylerdddd   (501) staff       (20)        0 2024-04-02 21:54:25.000000 bia-ia-0.0.3/bia-ia/data/arduino/
+drwxr-xr-x   0 tylerdddd   (501) staff       (20)        0 2024-04-02 21:54:25.000000 bia-ia-0.0.3/bia-ia/data/logs/
+-rw-r--r--   0 tylerdddd   (501) staff       (20)      276 2024-04-02 21:54:25.000000 bia-ia-0.0.3/bia-ia/data/._bia.db
+-rw-r--r--   0 tylerdddd   (501) staff       (20)   147456 2024-04-02 21:54:25.261860 bia-ia-0.0.3/bia-ia/data/bia.db
+-rw-r--r--   0 tylerdddd   (501) staff       (20)        0 2024-04-02 21:54:25.000000 bia-ia-0.0.3/bia-ia/data/logs/bia_2024_03_24_03_09_.log
+-rw-r--r--   0 tylerdddd   (501) staff       (20)        0 2024-04-02 21:54:25.000000 bia-ia-0.0.3/bia-ia/data/logs/bia_2024_03_24_09_30_.log
+-rw-r--r--   0 tylerdddd   (501) staff       (20)     2017 2024-04-02 21:54:25.000000 bia-ia-0.0.3/bia-ia/data/logs/bia_2024_03_24_10_51_.log
+-rw-r--r--   0 tylerdddd   (501) staff       (20)      416 2024-04-02 21:54:25.000000 bia-ia-0.0.3/bia-ia/data/logs/bia_2024_03_24_09_10_.log
+-rw-r--r--   0 tylerdddd   (501) staff       (20)      406 2024-04-02 21:54:25.000000 bia-ia-0.0.3/bia-ia/data/logs/bia_2024_03_25_09_04_.log
+-rw-r--r--   0 tylerdddd   (501) staff       (20)      220 2024-04-02 21:54:25.000000 bia-ia-0.0.3/bia-ia/data/logs/._bia_2024_03_25_08_53_.log
+-rw-r--r--   0 tylerdddd   (501) staff       (20)        0 2024-04-02 21:54:25.260745 bia-ia-0.0.3/bia-ia/data/logs/bia_2024_03_25_08_53_.log
+-rw-r--r--   0 tylerdddd   (501) staff       (20)      441 2024-04-02 21:54:25.000000 bia-ia-0.0.3/bia-ia/data/logs/bia_2024_03_24_01_37_.log
+-rw-r--r--   0 tylerdddd   (501) staff       (20)    19665 2024-04-02 21:54:25.000000 bia-ia-0.0.3/bia-ia/data/logs/bia_2024_03_24_03_06_.log
+drwxr-xr-x   0 tylerdddd   (501) staff       (20)        0 2024-04-02 21:54:25.000000 bia-ia-0.0.3/bia-ia/data/arduino/20240324_150726/
+drwxr-xr-x   0 tylerdddd   (501) staff       (20)        0 2024-04-02 21:54:25.000000 bia-ia-0.0.3/bia-ia/data/arduino/20240324_105329/
+drwxr-xr-x   0 tylerdddd   (501) staff       (20)        0 2024-04-02 21:54:25.000000 bia-ia-0.0.3/bia-ia/data/arduino/20240324_110209/
+drwxr-xr-x   0 tylerdddd   (501) staff       (20)        0 2024-04-02 21:54:25.000000 bia-ia-0.0.3/bia-ia/data/arduino/20240324_150807/
+-rw-r--r--   0 tylerdddd   (501) staff       (20)      120 2024-04-02 21:54:25.000000 bia-ia-0.0.3/bia-ia/data/arduino/._.DS_Store
+-rw-r--r--   0 tylerdddd   (501) staff       (20)     6148 2024-04-02 21:54:25.248662 bia-ia-0.0.3/bia-ia/data/arduino/.DS_Store
+drwxr-xr-x   0 tylerdddd   (501) staff       (20)        0 2024-04-02 21:54:25.000000 bia-ia-0.0.3/bia-ia/data/arduino/20240324_110918/
+drwxr-xr-x   0 tylerdddd   (501) staff       (20)        0 2024-04-02 21:54:25.000000 bia-ia-0.0.3/bia-ia/data/arduino/20240324_151148/
+drwxr-xr-x   0 tylerdddd   (501) staff       (20)        0 2024-04-02 21:54:25.000000 bia-ia-0.0.3/bia-ia/data/arduino/20240324_111016/
+drwxr-xr-x   0 tylerdddd   (501) staff       (20)        0 2024-04-02 21:54:25.000000 bia-ia-0.0.3/bia-ia/data/arduino/20240324_150841/
+drwxr-xr-x   0 tylerdddd   (501) staff       (20)        0 2024-04-02 21:54:25.000000 bia-ia-0.0.3/bia-ia/data/arduino/20240324_110240/
+drwxr-xr-x   0 tylerdddd   (501) staff       (20)        0 2024-04-02 21:54:25.000000 bia-ia-0.0.3/bia-ia/data/arduino/20240324_105359/
+drwxr-xr-x   0 tylerdddd   (501) staff       (20)        0 2024-04-02 21:54:25.000000 bia-ia-0.0.3/bia-ia/data/arduino/20240324_105203/
+drwxr-xr-x   0 tylerdddd   (501) staff       (20)        0 2024-04-02 21:54:25.000000 bia-ia-0.0.3/bia-ia/data/arduino/20240324_110952/
+drwxr-xr-x   0 tylerdddd   (501) staff       (20)        0 2024-04-02 21:54:25.000000 bia-ia-0.0.3/bia-ia/data/arduino/20240324_105738/
+drwxr-xr-x   0 tylerdddd   (501) staff       (20)        0 2024-04-02 21:54:25.000000 bia-ia-0.0.3/bia-ia/data/arduino/20240324_111301/
+-rw-r--r--   0 tylerdddd   (501) staff       (20)      430 2024-04-02 21:54:25.000000 bia-ia-0.0.3/bia-ia/data/arduino/20240324_111301/20240324_111301.ino
+-rw-r--r--   0 tylerdddd   (501) staff       (20)      176 2024-04-02 21:54:25.000000 bia-ia-0.0.3/bia-ia/data/arduino/20240324_105738/._20240324_105738.ino
+-rw-r--r--   0 tylerdddd   (501) staff       (20)     1971 2024-04-02 21:54:25.256188 bia-ia-0.0.3/bia-ia/data/arduino/20240324_105738/20240324_105738.ino
+-rw-r--r--   0 tylerdddd   (501) staff       (20)      376 2024-04-02 21:54:25.000000 bia-ia-0.0.3/bia-ia/data/arduino/20240324_110952/20240324_110952.ino
+-rw-r--r--   0 tylerdddd   (501) staff       (20)      176 2024-04-02 21:54:25.000000 bia-ia-0.0.3/bia-ia/data/arduino/20240324_105203/._20240324_105203.ino
+-rw-r--r--   0 tylerdddd   (501) staff       (20)      412 2024-04-02 21:54:25.254871 bia-ia-0.0.3/bia-ia/data/arduino/20240324_105203/20240324_105203.ino
+-rw-r--r--   0 tylerdddd   (501) staff       (20)      176 2024-04-02 21:54:25.000000 bia-ia-0.0.3/bia-ia/data/arduino/20240324_105359/._20240324_105359.ino
+-rw-r--r--   0 tylerdddd   (501) staff       (20)      429 2024-04-02 21:54:25.254180 bia-ia-0.0.3/bia-ia/data/arduino/20240324_105359/20240324_105359.ino
+-rw-r--r--   0 tylerdddd   (501) staff       (20)      176 2024-04-02 21:54:25.000000 bia-ia-0.0.3/bia-ia/data/arduino/20240324_110240/._20240324_110240.ino
+-rw-r--r--   0 tylerdddd   (501) staff       (20)      400 2024-04-02 21:54:25.253583 bia-ia-0.0.3/bia-ia/data/arduino/20240324_110240/20240324_110240.ino
+-rw-r--r--   0 tylerdddd   (501) staff       (20)      404 2024-04-02 21:54:25.000000 bia-ia-0.0.3/bia-ia/data/arduino/20240324_150841/20240324_150841.ino
+-rw-r--r--   0 tylerdddd   (501) staff       (20)      401 2024-04-02 21:54:25.000000 bia-ia-0.0.3/bia-ia/data/arduino/20240324_111016/20240324_111016.ino
+-rw-r--r--   0 tylerdddd   (501) staff       (20)      537 2024-04-02 21:54:25.000000 bia-ia-0.0.3/bia-ia/data/arduino/20240324_151148/20240324_151148.ino
+-rw-r--r--   0 tylerdddd   (501) staff       (20)      377 2024-04-02 21:54:25.000000 bia-ia-0.0.3/bia-ia/data/arduino/20240324_110918/20240324_110918.ino
+-rw-r--r--   0 tylerdddd   (501) staff       (20)      398 2024-04-02 21:54:25.000000 bia-ia-0.0.3/bia-ia/data/arduino/20240324_150807/20240324_150807.ino
+-rw-r--r--   0 tylerdddd   (501) staff       (20)      176 2024-04-02 21:54:25.000000 bia-ia-0.0.3/bia-ia/data/arduino/20240324_110209/._20240324_110209.ino
+-rw-r--r--   0 tylerdddd   (501) staff       (20)      504 2024-04-02 21:54:25.247577 bia-ia-0.0.3/bia-ia/data/arduino/20240324_110209/20240324_110209.ino
+-rw-r--r--   0 tylerdddd   (501) staff       (20)      376 2024-04-02 21:54:25.000000 bia-ia-0.0.3/bia-ia/data/arduino/20240324_105329/20240324_105329.ino
+-rw-r--r--   0 tylerdddd   (501) staff       (20)     1730 2024-04-02 21:54:25.000000 bia-ia-0.0.3/bia-ia/data/arduino/20240324_150726/20240324_150726.ino
+-rw-r--r--   0 tylerdddd   (501) staff       (20)   306118 2024-04-02 21:54:25.000000 bia-ia-0.0.3/bia-ia/data/camera/20240323_095157.jpg
+-rw-r--r--   0 tylerdddd   (501) staff       (20)      120 2024-04-02 21:54:25.000000 bia-ia-0.0.3/bia-ia/data/python/._.DS_Store
+-rw-r--r--   0 tylerdddd   (501) staff       (20)     6148 2024-04-02 21:54:25.240595 bia-ia-0.0.3/bia-ia/data/python/.DS_Store
+-rw-r--r--   0 tylerdddd   (501) staff       (20)     2780 2024-04-02 21:16:33.000000 bia-ia-0.0.3/bia-ia/controllers/action.py
+-rw-r--r--   0 tylerdddd   (501) staff       (20)     1332 2024-04-02 21:16:33.000000 bia-ia-0.0.3/bia-ia/controllers/asynch.py
+-rw-r--r--   0 tylerdddd   (501) staff       (20)     2937 2024-04-02 21:16:33.000000 bia-ia-0.0.3/bia-ia/controllers/base.py
+drwxr-xr-x   0 tylerdddd   (501) staff       (20)        0 2024-04-02 21:52:29.000000 bia-ia-0.0.3/bia-ia/models/blocks/
+drwxr-xr-x   0 tylerdddd   (501) staff       (20)        0 2024-04-02 21:52:29.000000 bia-ia-0.0.3/bia-ia/models/database/
+drwxr-xr-x   0 tylerdddd   (501) staff       (20)        0 2024-04-02 21:52:29.000000 bia-ia-0.0.3/bia-ia/models/speech/
+drwxr-xr-x   0 tylerdddd   (501) staff       (20)        0 2024-04-02 21:52:29.000000 bia-ia-0.0.3/bia-ia/models/robot/
+drwxr-xr-x   0 tylerdddd   (501) staff       (20)        0 2024-04-02 21:52:29.000000 bia-ia-0.0.3/bia-ia/models/openAI/
+-rw-r--r--   0 tylerdddd   (501) staff       (20)     1553 2024-04-02 21:16:33.000000 bia-ia-0.0.3/bia-ia/models/openAI/ai.py
+-rw-r--r--   0 tylerdddd   (501) staff       (20)     4602 2024-04-02 21:16:33.000000 bia-ia-0.0.3/bia-ia/models/robot/robot.py
+-rw-r--r--   0 tylerdddd   (501) staff       (20)     5890 2024-04-02 21:16:33.000000 bia-ia-0.0.3/bia-ia/models/speech/prompt.py
+-rw-r--r--   0 tylerdddd   (501) staff       (20)     1583 2024-04-02 21:16:33.000000 bia-ia-0.0.3/bia-ia/models/database/grandma.py
+-rw-r--r--   0 tylerdddd   (501) staff       (20)     1041 2024-04-02 21:16:33.000000 bia-ia-0.0.3/bia-ia/models/database/mia_utils.py
+-rw-r--r--   0 tylerdddd   (501) staff       (20)     7012 2024-04-02 21:16:33.000000 bia-ia-0.0.3/bia-ia/models/database/mia.py
+-rw-r--r--   0 tylerdddd   (501) staff       (20)     1169 2024-04-02 21:16:33.000000 bia-ia-0.0.3/bia-ia/models/blocks/netflix.py
+-rw-r--r--   0 tylerdddd   (501) staff       (20)     1040 2024-04-02 21:16:33.000000 bia-ia-0.0.3/bia-ia/models/blocks/web.py
+-rw-r--r--   0 tylerdddd   (501) staff       (20)     1181 2024-04-02 21:16:33.000000 bia-ia-0.0.3/bia-ia/models/blocks/youtube.py
+-rw-r--r--   0 tylerdddd   (501) staff       (20)      867 2024-04-02 21:16:33.000000 bia-ia-0.0.3/bia-ia/models/blocks/display.py
+-rw-r--r--   0 tylerdddd   (501) staff       (20)      923 2024-04-02 21:16:33.000000 bia-ia-0.0.3/bia-ia/models/blocks/default.py
+-rw-r--r--   0 tylerdddd   (501) staff       (20)     1622 2024-04-02 21:16:33.000000 bia-ia-0.0.3/bia-ia/models/blocks/camera.py
+-rw-r--r--   0 tylerdddd   (501) staff       (20)      860 2024-04-02 21:16:33.000000 bia-ia-0.0.3/bia-ia/models/blocks/alexa.py
+-rw-r--r--   0 tylerdddd   (501) staff       (20)     2292 2024-04-02 21:16:33.000000 bia-ia-0.0.3/bia-ia/models/blocks/python.py
+-rw-r--r--   0 tylerdddd   (501) staff       (20)     1141 2024-04-02 21:16:33.000000 bia-ia-0.0.3/bia-ia/models/blocks/tv.py
+-rw-r--r--   0 tylerdddd   (501) staff       (20)     1158 2024-04-02 21:16:33.000000 bia-ia-0.0.3/bia-ia/models/blocks/radio.py
+-rw-r--r--   0 tylerdddd   (501) staff       (20)      880 2024-04-02 21:16:33.000000 bia-ia-0.0.3/bia-ia/models/blocks/block.py
+-rw-r--r--   0 tylerdddd   (501) staff       (20)      879 2024-04-02 21:16:33.000000 bia-ia-0.0.3/bia-ia/models/blocks/macro.py
+-rw-r--r--   0 tylerdddd   (501) staff       (20)     2588 2024-04-02 21:16:33.000000 bia-ia-0.0.3/bia-ia/models/blocks/arduino.py
+-rw-r--r--   0 tylerdddd   (501) staff       (20)     1299 2024-04-02 21:16:33.000000 bia-ia-0.0.3/bia-ia/utils/lang.py
+-rw-r--r--   0 tylerdddd   (501) staff       (20)    10394 2024-04-02 21:16:33.000000 bia-ia-0.0.3/bia-ia/utils/config.py
+-rw-r--r--   0 tylerdddd   (501) staff       (20)     2431 2024-04-02 21:55:18.000000 bia-ia-0.0.3/bia-ia/utils/_config.cfg
+-rw-r--r--   0 tylerdddd   (501) staff       (20)     2424 2024-04-02 21:55:18.000000 bia-ia-0.0.3/bia-ia/utils/config.cfg
+-rw-r--r--   0 tylerdddd   (501) staff       (20)     1783 2024-04-02 21:16:33.000000 bia-ia-0.0.3/bia-ia/utils/text2Speech.py
+-rw-r--r--   0 tylerdddd   (501) staff       (20)     1817 2024-04-02 21:16:33.000000 bia-ia-0.0.3/bia-ia/utils/debug.py
+-rw-r--r--   0 tylerdddd   (501) staff       (20)     2481 2024-04-02 21:16:33.000000 bia-ia-0.0.3/bia-ia/utils/speech2Text.py
+-rw-r--r--   0 tylerdddd   (501) staff       (20)     1411 2024-04-02 21:16:33.000000 bia-ia-0.0.3/bia-ia/utils/paraphrase.py
+-rwxr-xr-x   0 tylerdddd   (501) staff       (20)      327 2024-04-02 21:53:53.000000 bia-ia-0.0.3/bia-ia/deploy/._Bia.command
+-rwxr-xr-x   0 tylerdddd   (501) staff       (20)      278 2024-04-02 21:53:53.828253 bia-ia-0.0.3/bia-ia/deploy/Bia.command
+drwxr-xr-x   0 tylerdddd   (501) staff       (20)        0 2024-04-02 21:53:53.000000 bia-ia-0.0.3/bia-ia/deploy/Otto.egg-info/
+-rwxr-xr-x   0 tylerdddd   (501) staff       (20)      327 2024-04-02 21:53:53.000000 bia-ia-0.0.3/bia-ia/deploy/._run.sh
+-rwxr-xr-x   0 tylerdddd   (501) staff       (20)      259 2024-04-02 21:53:53.832494 bia-ia-0.0.3/bia-ia/deploy/run.sh
+-rwxr-xr-x   0 tylerdddd   (501) staff       (20)      327 2024-04-02 21:53:53.000000 bia-ia-0.0.3/bia-ia/deploy/._deploy.sh
+-rwxr-xr-x   0 tylerdddd   (501) staff       (20)      866 2024-04-02 21:53:53.833635 bia-ia-0.0.3/bia-ia/deploy/deploy.sh
+drwxr-xr-x   0 tylerdddd   (501) staff       (20)        0 2024-04-02 21:53:53.000000 bia-ia-0.0.3/bia-ia/deploy/Bia.egg-info/
+drwxr-xr-x   0 tylerdddd   (501) staff       (20)        0 2024-04-02 21:53:53.000000 bia-ia-0.0.3/bia-ia/deploy/biaa.egg-info/
+-rw-r--r--   0 tylerdddd   (501) staff       (20)       99 2024-04-02 21:53:53.000000 bia-ia-0.0.3/bia-ia/deploy/biaa.egg-info/PKG-INFO
+-rw-r--r--   0 tylerdddd   (501) staff       (20)        0 2024-04-02 21:53:53.000000 bia-ia-0.0.3/bia-ia/deploy/biaa.egg-info/SOURCES.txt
+-rw-r--r--   0 tylerdddd   (501) staff       (20)        4 2024-04-02 21:53:53.000000 bia-ia-0.0.3/bia-ia/deploy/biaa.egg-info/top_level.txt
+-rw-r--r--   0 tylerdddd   (501) staff       (20)        1 2024-04-02 21:53:53.000000 bia-ia-0.0.3/bia-ia/deploy/biaa.egg-info/dependency_links.txt
+-rw-r--r--   0 tylerdddd   (501) staff       (20)       98 2024-04-02 21:53:53.000000 bia-ia-0.0.3/bia-ia/deploy/Bia.egg-info/PKG-INFO
+-rw-r--r--   0 tylerdddd   (501) staff       (20)        0 2024-04-02 21:53:53.000000 bia-ia-0.0.3/bia-ia/deploy/Bia.egg-info/SOURCES.txt
+-rw-r--r--   0 tylerdddd   (501) staff       (20)        7 2024-04-02 21:53:53.000000 bia-ia-0.0.3/bia-ia/deploy/Bia.egg-info/top_level.txt
+-rw-r--r--   0 tylerdddd   (501) staff       (20)        1 2024-04-02 21:53:53.000000 bia-ia-0.0.3/bia-ia/deploy/Bia.egg-info/dependency_links.txt
+-rw-r--r--   0 tylerdddd   (501) staff       (20)       76 2024-04-02 21:53:53.000000 bia-ia-0.0.3/bia-ia/deploy/Otto.egg-info/PKG-INFO
+-rw-r--r--   0 tylerdddd   (501) staff       (20)        0 2024-04-02 21:53:53.000000 bia-ia-0.0.3/bia-ia/deploy/Otto.egg-info/SOURCES.txt
+-rw-r--r--   0 tylerdddd   (501) staff       (20)        4 2024-04-02 21:53:53.000000 bia-ia-0.0.3/bia-ia/deploy/Otto.egg-info/top_level.txt
+-rw-r--r--   0 tylerdddd   (501) staff       (20)        1 2024-04-02 21:53:53.000000 bia-ia-0.0.3/bia-ia/deploy/Otto.egg-info/dependency_links.txt
+-rw-r--r--   0 tylerdddd   (501) staff       (20)      692 2024-04-02 21:52:29.000000 bia-ia-0.0.3/bia_ia.egg-info/PKG-INFO
+-rw-r--r--   0 tylerdddd   (501) staff       (20)     1047 2024-04-02 21:52:29.000000 bia-ia-0.0.3/bia_ia.egg-info/SOURCES.txt
+-rw-r--r--   0 tylerdddd   (501) staff       (20)      149 2024-04-02 21:52:29.000000 bia-ia-0.0.3/bia_ia.egg-info/requires.txt
+-rw-r--r--   0 tylerdddd   (501) staff       (20)        7 2024-04-02 21:52:29.000000 bia-ia-0.0.3/bia_ia.egg-info/top_level.txt
+-rw-r--r--   0 tylerdddd   (501) staff       (20)        1 2024-04-02 21:52:29.000000 bia-ia-0.0.3/bia_ia.egg-info/dependency_links.txt
```

### Comparing `bia-ia-0.0.2/PKG-INFO` & `bia-ia-0.0.3/bia_ia.egg-info/PKG-INFO`

 * *Files identical despite different names*

### Comparing `bia-ia-0.0.2/setup.py` & `bia-ia-0.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 #
 # setup definition
 # --------------------------
 
 from setuptools import setup
 
 __project__ = "bia-ia"
-__version__ = "0.0.2"
+__version__ = "0.0.3"
 __description__ = "BIA (IA), your IA powered vocal assistant"
 __packages__ = ["bia-ia", "bia-ia.utils", "bia-ia.controllers", "bia-ia.models.blocks", "bia-ia.models.database", "bia-ia.models.openAI", "bia-ia.models.robot", "bia-ia.models.speech", "bia-ia.data", "bia-ia.deploy", "bia-ia.views", "bia-ia.bin"]
 __author__ = "TylerDDDD"
 __author_email__ = "makertylerdddd@gmail.com"
 __classifiers__ = [
 	"Development Status :: 3 - Alpha", 
 	"Intended Audience :: Education",
```

### Comparing `bia-ia-0.0.2/bia-ia/bia.py` & `bia-ia-0.0.3/bia-ia/bia.py`

 * *Files identical despite different names*

### Comparing `bia-ia-0.0.2/bia-ia/views/app.py` & `bia-ia-0.0.3/bia-ia/views/app.py`

 * *Files identical despite different names*

### Comparing `bia-ia-0.0.2/bia-ia/data/.DS_Store` & `bia-ia-0.0.3/bia-ia/data/.DS_Store`

 * *Files identical despite different names*

### Comparing `bia-ia-0.0.2/bia-ia/data/_bia.db` & `bia-ia-0.0.3/bia-ia/data/_bia.db`

 * *Files identical despite different names*

### Comparing `bia-ia-0.0.2/bia-ia/data/bia.db` & `bia-ia-0.0.3/bia-ia/data/bia.db`

 * *Files identical despite different names*

### Comparing `bia-ia-0.0.2/bia-ia/data/logs/bia_2024_03_24_10_51_.log` & `bia-ia-0.0.3/bia-ia/data/logs/bia_2024_03_24_10_51_.log`

 * *Files identical despite different names*

### Comparing `bia-ia-0.0.2/bia-ia/data/logs/bia_2024_03_24_03_06_.log` & `bia-ia-0.0.3/bia-ia/data/logs/bia_2024_03_24_03_06_.log`

 * *Files identical despite different names*

### Comparing `bia-ia-0.0.2/bia-ia/data/arduino/.DS_Store` & `bia-ia-0.0.3/bia-ia/data/arduino/.DS_Store`

 * *Files identical despite different names*

### Comparing `bia-ia-0.0.2/bia-ia/data/arduino/20240324_105738/20240324_105738.ino` & `bia-ia-0.0.3/bia-ia/data/arduino/20240324_105738/20240324_105738.ino`

 * *Files identical despite different names*

### Comparing `bia-ia-0.0.2/bia-ia/data/arduino/20240324_151148/20240324_151148.ino` & `bia-ia-0.0.3/bia-ia/data/arduino/20240324_151148/20240324_151148.ino`

 * *Files identical despite different names*

### Comparing `bia-ia-0.0.2/bia-ia/data/arduino/20240324_150726/20240324_150726.ino` & `bia-ia-0.0.3/bia-ia/data/arduino/20240324_150726/20240324_150726.ino`

 * *Files identical despite different names*

### Comparing `bia-ia-0.0.2/bia-ia/data/camera/20240323_095157.jpg` & `bia-ia-0.0.3/bia-ia/data/camera/20240323_095157.jpg`

 * *Files identical despite different names*

### Comparing `bia-ia-0.0.2/bia-ia/data/python/.DS_Store` & `bia-ia-0.0.3/bia-ia/data/python/.DS_Store`

 * *Files identical despite different names*

### Comparing `bia-ia-0.0.2/bia-ia/controllers/action.py` & `bia-ia-0.0.3/bia-ia/controllers/action.py`

 * *Files identical despite different names*

### Comparing `bia-ia-0.0.2/bia-ia/controllers/asynch.py` & `bia-ia-0.0.3/bia-ia/controllers/asynch.py`

 * *Files identical despite different names*

### Comparing `bia-ia-0.0.2/bia-ia/controllers/base.py` & `bia-ia-0.0.3/bia-ia/controllers/base.py`

 * *Files identical despite different names*

### Comparing `bia-ia-0.0.2/bia-ia/models/openAI/ai.py` & `bia-ia-0.0.3/bia-ia/models/openAI/ai.py`

 * *Files identical despite different names*

### Comparing `bia-ia-0.0.2/bia-ia/models/robot/robot.py` & `bia-ia-0.0.3/bia-ia/models/robot/robot.py`

 * *Files identical despite different names*

### Comparing `bia-ia-0.0.2/bia-ia/models/speech/prompt.py` & `bia-ia-0.0.3/bia-ia/models/speech/prompt.py`

 * *Files identical despite different names*

### Comparing `bia-ia-0.0.2/bia-ia/models/database/grandma.py` & `bia-ia-0.0.3/bia-ia/models/database/grandma.py`

 * *Files identical despite different names*

### Comparing `bia-ia-0.0.2/bia-ia/models/database/mia_utils.py` & `bia-ia-0.0.3/bia-ia/models/database/mia_utils.py`

 * *Files identical despite different names*

### Comparing `bia-ia-0.0.2/bia-ia/models/database/mia.py` & `bia-ia-0.0.3/bia-ia/models/database/mia.py`

 * *Files identical despite different names*

### Comparing `bia-ia-0.0.2/bia-ia/models/blocks/netflix.py` & `bia-ia-0.0.3/bia-ia/models/blocks/netflix.py`

 * *Files identical despite different names*

### Comparing `bia-ia-0.0.2/bia-ia/models/blocks/web.py` & `bia-ia-0.0.3/bia-ia/models/blocks/web.py`

 * *Files identical despite different names*

### Comparing `bia-ia-0.0.2/bia-ia/models/blocks/youtube.py` & `bia-ia-0.0.3/bia-ia/models/blocks/youtube.py`

 * *Files identical despite different names*

### Comparing `bia-ia-0.0.2/bia-ia/models/blocks/display.py` & `bia-ia-0.0.3/bia-ia/models/blocks/display.py`

 * *Files identical despite different names*

### Comparing `bia-ia-0.0.2/bia-ia/models/blocks/default.py` & `bia-ia-0.0.3/bia-ia/models/blocks/default.py`

 * *Files identical despite different names*

### Comparing `bia-ia-0.0.2/bia-ia/models/blocks/camera.py` & `bia-ia-0.0.3/bia-ia/models/blocks/camera.py`

 * *Files identical despite different names*

### Comparing `bia-ia-0.0.2/bia-ia/models/blocks/alexa.py` & `bia-ia-0.0.3/bia-ia/models/blocks/alexa.py`

 * *Files identical despite different names*

### Comparing `bia-ia-0.0.2/bia-ia/models/blocks/python.py` & `bia-ia-0.0.3/bia-ia/models/blocks/python.py`

 * *Files identical despite different names*

### Comparing `bia-ia-0.0.2/bia-ia/models/blocks/tv.py` & `bia-ia-0.0.3/bia-ia/models/blocks/tv.py`

 * *Files identical despite different names*

### Comparing `bia-ia-0.0.2/bia-ia/models/blocks/radio.py` & `bia-ia-0.0.3/bia-ia/models/blocks/radio.py`

 * *Files identical despite different names*

### Comparing `bia-ia-0.0.2/bia-ia/models/blocks/block.py` & `bia-ia-0.0.3/bia-ia/models/blocks/block.py`

 * *Files identical despite different names*

### Comparing `bia-ia-0.0.2/bia-ia/models/blocks/macro.py` & `bia-ia-0.0.3/bia-ia/models/blocks/macro.py`

 * *Files identical despite different names*

### Comparing `bia-ia-0.0.2/bia-ia/models/blocks/arduino.py` & `bia-ia-0.0.3/bia-ia/models/blocks/arduino.py`

 * *Files identical despite different names*

### Comparing `bia-ia-0.0.2/bia-ia/utils/lang.py` & `bia-ia-0.0.3/bia-ia/utils/lang.py`

 * *Files identical despite different names*

### Comparing `bia-ia-0.0.2/bia-ia/utils/config.py` & `bia-ia-0.0.3/bia-ia/utils/config.py`

 * *Files identical despite different names*

### Comparing `bia-ia-0.0.2/bia-ia/utils/_config.cfg` & `bia-ia-0.0.3/bia-ia/utils/_config.cfg`

 * *Files identical despite different names*

### Comparing `bia-ia-0.0.2/bia-ia/utils/config.cfg` & `bia-ia-0.0.3/bia-ia/utils/config.cfg`

 * *Files identical despite different names*

### Comparing `bia-ia-0.0.2/bia-ia/utils/text2Speech.py` & `bia-ia-0.0.3/bia-ia/utils/text2Speech.py`

 * *Files identical despite different names*

### Comparing `bia-ia-0.0.2/bia-ia/utils/debug.py` & `bia-ia-0.0.3/bia-ia/utils/debug.py`

 * *Files identical despite different names*

### Comparing `bia-ia-0.0.2/bia-ia/utils/speech2Text.py` & `bia-ia-0.0.3/bia-ia/utils/speech2Text.py`

 * *Files identical despite different names*

### Comparing `bia-ia-0.0.2/bia-ia/utils/paraphrase.py` & `bia-ia-0.0.3/bia-ia/utils/paraphrase.py`

 * *Files identical despite different names*

### Comparing `bia-ia-0.0.2/bia_ia.egg-info/PKG-INFO` & `bia-ia-0.0.3/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bia-ia
-Version: 0.0.2
+Version: 0.0.3
 Summary: BIA (IA), your IA powered vocal assistant
 Author: TylerDDDD
 Author-email: makertylerdddd@gmail.com
 Keywords: robot,otto,ai,vocal,assistant
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Education
 Classifier: Programming Language :: Python :: 3
```

### Comparing `bia-ia-0.0.2/bia_ia.egg-info/SOURCES.txt` & `bia-ia-0.0.3/bia_ia.egg-info/SOURCES.txt`

 * *Files identical despite different names*

