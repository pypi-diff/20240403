# Comparing `tmp/rpapy-1.1.2.tar.gz` & `tmp/rpapy-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rpapy-1.1.2.tar", max compression
+gzip compressed data, was "rpapy-1.1.3.tar", max compression
```

## Comparing `rpapy-1.1.2.tar` & `rpapy-1.1.3.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rw-r--r--   0        0        0     1100 2024-02-24 15:05:07.143850 rpapy-1.1.2/LICENSE
--rw-r--r--   0        0        0     1881 2024-04-03 13:55:57.715491 rpapy-1.1.2/pyproject.toml
--rw-r--r--   0        0        0     3759 2024-04-03 12:46:39.139719 rpapy-1.1.2/README.md
--rw-r--r--   0        0        0       53 2024-04-03 13:55:57.757467 rpapy-1.1.2/rpapy/__init__.py
--rw-r--r--   0        0        0     7606 2024-04-03 13:55:57.760460 rpapy-1.1.2/rpapy/__main__.py
--rw-r--r--   0        0        0    16039 2024-04-03 12:46:20.286610 rpapy-1.1.2/rpapy/activities.py
--rw-r--r--   0        0        0        0 2024-03-11 23:33:14.532292 rpapy-1.1.2/rpapy/core/__init__.py
--rw-r--r--   0        0        0     1890 2024-04-03 12:46:20.288639 rpapy-1.1.2/rpapy/core/config.py
--rw-r--r--   0        0        0     1944 2024-04-03 12:46:20.289639 rpapy-1.1.2/rpapy/core/image_mapper.py
--rw-r--r--   0        0        0    15288 2024-04-03 12:46:20.291650 rpapy-1.1.2/rpapy/core/locator.py
--rw-r--r--   0        0        0     1030 2024-04-03 12:46:20.292639 rpapy-1.1.2/rpapy/core/prepare_text.py
--rw-r--r--   0        0        0     4847 2024-04-03 12:46:20.296253 rpapy-1.1.2/rpapy/core/snipps/__init__.py
--rw-r--r--   0        0        0    10433 2024-04-03 12:46:20.299191 rpapy-1.1.2/rpapy/core/snipps/codesnippets.py
--rw-r--r--   0        0        0     5670 2024-04-03 12:46:20.300199 rpapy-1.1.2/rpapy/core/snipps/loads.py
--rw-r--r--   0        0        0    11236 2024-03-31 01:57:48.660663 rpapy-1.1.2/rpapy/core/snipps/snippingtools.py
--rw-r--r--   0        0        0    13102 2024-04-03 12:46:20.301190 rpapy-1.1.2/rpapy/core/snipps/templates.py
--rw-r--r--   0        0        0      257 2024-03-23 01:44:02.673566 rpapy-1.1.2/rpapy/core/utils/__init__.py
--rw-r--r--   0        0        0        0 2024-02-24 15:05:07.224251 rpapy-1.1.2/rpapy/core/utils/example/__init__.py
--rw-r--r--   0        0        0    89781 2024-03-22 18:35:46.875840 rpapy-1.1.2/rpapy/core/utils/example/paint_robot.py
--rw-r--r--   0        0        0    31581 2024-02-24 15:05:07.236199 rpapy-1.1.2/rpapy/core/utils/imagens/IMAGEM_NAO_ENCONTRADA.png
--rw-r--r--   0        0        0  2623476 2024-03-22 18:17:08.029741 rpapy-1.1.2/rpapy/core/utils/imagens/template_win11_screen_1920x1080.svg
--rw-r--r--   0        0        0     6920 2024-04-03 13:33:10.772736 rpapy-1.1.2/rpapy/core/utils/messages.py
--rw-r--r--   0        0        0     4995 1970-01-01 00:00:00.000000 rpapy-1.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1100 2024-02-24 15:05:07.143850 rpapy-1.1.3/LICENSE
+-rw-r--r--   0        0        0     1945 2024-04-03 19:07:10.838717 rpapy-1.1.3/pyproject.toml
+-rw-r--r--   0        0        0     3759 2024-04-03 12:46:39.139719 rpapy-1.1.3/README.md
+-rw-r--r--   0        0        0       53 2024-04-03 19:07:10.896450 rpapy-1.1.3/rpapy/__init__.py
+-rw-r--r--   0        0        0     7606 2024-04-03 19:07:12.659236 rpapy-1.1.3/rpapy/__main__.py
+-rw-r--r--   0        0        0    16039 2024-04-03 12:46:20.286610 rpapy-1.1.3/rpapy/activities.py
+-rw-r--r--   0        0        0        0 2024-03-11 23:33:14.532292 rpapy-1.1.3/rpapy/core/__init__.py
+-rw-r--r--   0        0        0     1890 2024-04-03 17:16:54.286915 rpapy-1.1.3/rpapy/core/config.py
+-rw-r--r--   0        0        0     1944 2024-04-03 12:46:20.289639 rpapy-1.1.3/rpapy/core/image_mapper.py
+-rw-r--r--   0        0        0    15243 2024-04-03 15:01:43.798119 rpapy-1.1.3/rpapy/core/locator.py
+-rw-r--r--   0        0        0     1030 2024-04-03 12:46:20.292639 rpapy-1.1.3/rpapy/core/prepare_text.py
+-rw-r--r--   0        0        0     4847 2024-04-03 12:46:20.296253 rpapy-1.1.3/rpapy/core/snipps/__init__.py
+-rw-r--r--   0        0        0    10433 2024-04-03 12:46:20.299191 rpapy-1.1.3/rpapy/core/snipps/codesnippets.py
+-rw-r--r--   0        0        0     5670 2024-04-03 12:46:20.300199 rpapy-1.1.3/rpapy/core/snipps/loads.py
+-rw-r--r--   0        0        0    11236 2024-03-31 01:57:48.660663 rpapy-1.1.3/rpapy/core/snipps/snippingtools.py
+-rw-r--r--   0        0        0    13099 2024-04-03 17:19:19.336645 rpapy-1.1.3/rpapy/core/snipps/templates.py
+-rw-r--r--   0        0        0      257 2024-04-03 15:02:48.012653 rpapy-1.1.3/rpapy/core/utils/__init__.py
+-rw-r--r--   0        0        0        0 2024-02-24 15:05:07.224251 rpapy-1.1.3/rpapy/core/utils/example/__init__.py
+-rw-r--r--   0        0        0    89689 2024-04-03 17:12:30.066746 rpapy-1.1.3/rpapy/core/utils/example/paint_robot.py
+-rw-r--r--   0        0        0    31581 2024-02-24 15:05:07.236199 rpapy-1.1.3/rpapy/core/utils/imagens/IMAGEM_NAO_ENCONTRADA.png
+-rw-r--r--   0        0        0  2623476 2024-03-22 18:17:08.029741 rpapy-1.1.3/rpapy/core/utils/imagens/template_win11_screen_1920x1080.svg
+-rw-r--r--   0        0        0     6920 2024-04-03 17:13:54.801542 rpapy-1.1.3/rpapy/core/utils/messages.py
+-rw-r--r--   0        0        0     4995 1970-01-01 00:00:00.000000 rpapy-1.1.3/PKG-INFO
```

### Comparing `rpapy-1.1.2/LICENSE` & `rpapy-1.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `rpapy-1.1.2/pyproject.toml` & `rpapy-1.1.3/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "rpapy"
-version = "1.1.2"
+version = "1.1.3"
 description = "RPAPY is a open source easy tool for automating boring stuffs on any screen with robotframework, pyautogui, pywinauto and others."
 authors = ["Codigo Sem Cera <codigo100cera@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/codigo100cera/rpapy"
 include = ["LICENSE", "README.md", "*.cfg", "rpapy/core/utils/imagens/*.png", "rpapy/core/utils/imagens/*.svg"]
 keywords = ["rpa", "robotframework", "automations", "tools"]
@@ -52,14 +52,17 @@
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.pytest.ini_options]
 pythonpath = "."
 addopts = "--doctest-modules"
 
+[tool.taskipy.tasks]
+draw = 'robot -d log tasks/main.robot'
+
 [tool.poetry_bumpversion.file."rpapy/__main__.py"]
 search = '- rpapy v{current_version}'
 replace = '- rpapy v{new_version}'
 
 [[tool.poetry_bumpversion.replacements]]
 files = ["rpapy/__init__.py",]
 search = '__version__ = "{current_version}"'
```

### Comparing `rpapy-1.1.2/README.md` & `rpapy-1.1.3/README.md`

 * *Files identical despite different names*

### Comparing `rpapy-1.1.2/rpapy/__main__.py` & `rpapy-1.1.3/rpapy/__main__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """RPAPY is a open source easy tool for automating boring stuffs on any screen with robotframework, pyautogui, pywinauto and others.
 --------
 
-- rpapy v1.1.2
+- rpapy v1.1.3
 """
 import sys
 from pathlib import Path
 from unittest.mock import patch
 
 import pyperclip
 from pynput import keyboard, mouse
```

### Comparing `rpapy-1.1.2/rpapy/activities.py` & `rpapy-1.1.3/rpapy/activities.py`

 * *Files identical despite different names*

### Comparing `rpapy-1.1.2/rpapy/core/config.py` & `rpapy-1.1.3/rpapy/core/config.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 class Config:
 
     BASE_DIR = os.environ.get('BASE_DIR_RPAPY') or basedir
 
     RESOURCES_DIR_NAME = os.environ.get('RESOURCES_DIR_NAME') or 'resources'
     RESOURCES_KEYWORDS_FILE_NAME = os.environ.get('RESOURCES_KEYWORDS_FILE_NAME') or 'keywords.robot'
     IMAGES_DIR_NAME = os.environ.get('IMAGES_DIR_NAME') or 'images'
-    IMAGES_ERROR_DIR_NAME = os.environ.get('IMAGES_ERROR_DIR_NAME') or 'images_error'
+    IMAGES_ERROR_DIR_NAME = os.environ.get('IMAGES_ERROR_DIR_NAME') or 'error_images'
     TASKS_DIR_NAME = os.environ.get('TASKS_DIR_NAME') or 'tasks'
     MAX_WAIT_MAINTENANCE = int(os.environ.get('MAX_WAIT_MAINTENANCE') or 5)
     CHECK_MODE = os.environ.get('CHECK_MODE') or False
     FAILSAFE_OFF = os.environ.get('FAILSAFE_OFF') or False
     ACTIVE_TEMPORARY_ARCHIVE = os.environ.get('ACTIVE_TEMPORARY_ARCHIVE') or False
     TEMPORALY_FILE_NAME = os.environ.get('TEMPORALY_FILE_NAME') or 'temp.txt'
```

### Comparing `rpapy-1.1.2/rpapy/core/image_mapper.py` & `rpapy-1.1.3/rpapy/core/image_mapper.py`

 * *Files identical despite different names*

### Comparing `rpapy-1.1.2/rpapy/core/locator.py` & `rpapy-1.1.3/rpapy/core/locator.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 import datetime
 import os
 import time
 import warnings
-from pathlib import Path
 from typing import Dict, Tuple
 
 import cv2
 import numpy as np
 import pyautogui
 from PIL import Image
 
-from rpapy.core.utils.messages import confirm_ok_cancel, confirm_yes_no_cancel
+from rpapy.core.utils.messages import confirm_yes_no_cancel
 
 with warnings.catch_warnings():
         warnings.simplefilter("ignore")
         from pywinauto import Desktop
 
 from rpapy.core.image_mapper import map_images
 from rpapy.core.snipps.loads import create_python_default_dirs
```

### Comparing `rpapy-1.1.2/rpapy/core/prepare_text.py` & `rpapy-1.1.3/rpapy/core/prepare_text.py`

 * *Files identical despite different names*

### Comparing `rpapy-1.1.2/rpapy/core/snipps/__init__.py` & `rpapy-1.1.3/rpapy/core/snipps/__init__.py`

 * *Files identical despite different names*

### Comparing `rpapy-1.1.2/rpapy/core/snipps/codesnippets.py` & `rpapy-1.1.3/rpapy/core/snipps/codesnippets.py`

 * *Files identical despite different names*

### Comparing `rpapy-1.1.2/rpapy/core/snipps/loads.py` & `rpapy-1.1.3/rpapy/core/snipps/loads.py`

 * *Files identical despite different names*

### Comparing `rpapy-1.1.2/rpapy/core/snipps/snippingtools.py` & `rpapy-1.1.3/rpapy/core/snipps/snippingtools.py`

 * *Files identical despite different names*

### Comparing `rpapy-1.1.2/rpapy/core/snipps/templates.py` & `rpapy-1.1.3/rpapy/core/snipps/templates.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,21 +3,21 @@
 ##########################################################################################
 
 VARIAVEIS_AMBIENTE = """###VARIAVEIS DE AMBIENTE PYTHON-DOTENV
 
 #RESOURCES_DIR_NAME=resources
 #RESOURCES_KEYWORDS_FILE_NAME=keywords.robot
 #IMAGES_DIR_NAME=images
-#IMAGES_ERROR_DIR_NAME=images_error
+#IMAGES_ERROR_DIR_NAME=error_images
 #TASKS_DIR_NAME=tasks
 #MAX_WAIT_MAINTENANCE=3
 #CHECK_MODE=True
 #FAILSAFE_OFF=True
 #ACTIVE_TEMPORARY_ARCHIVE=se
-#TEMPORALY_FILE_NAME=temp.Faltxt
+#TEMPORALY_FILE_NAME=temp.txt
 #ONLY_IMAGE_PATH=False
 
 """
 
 ##########################################################################################
 MODULES_IMPORT_PY = '''"""[summary]
 """
@@ -58,28 +58,28 @@
 
 *** Keywords ***
 Keyword principal
     Primeira Keyword        ${VAR}
 '''
 
 ##########################################################################################
-MODULES_IMPORT_RESOURCE = '''*** Settings ***
+MODULES_IMPORT_RESOURCE = """*** Settings ***
 Documentation    Documentacao das Keywords da Suite de Tasks
 Library     rpapy.activities
   
 
 *** Variables ***
 ${VAR}=      variables
 
 
 *** Keywords ***
 Primeira Keyword
     [Arguments]         ${arg}
     Log To Console      Hello ${arg}!
-'''
+"""
 
 ##########################################################################################
 MSG_OPCOES_IMG = """
 ***ATENÇÃO***
 Insira os parâmetros na sequência de 1 a 5, conforme o necessário, 
 deixando-os separados apenas por espaço.
```

### Comparing `rpapy-1.1.2/rpapy/core/utils/example/paint_robot.py` & `rpapy-1.1.3/rpapy/core/utils/example/paint_robot.py`

 * *Files 0% similar despite different names*

```diff
@@ -60,30 +60,30 @@
 
     Click Vision    btn_editar_cores    backend=uia
 
     Wait Element Vision    titulo_editar_cores
     Sleep    .5
 
     Write Text Vision    campo_red    backend=uia    after=.2
-    ...    text=${LIMPAR}${r}      move_x=-40
+    ...    text=${LIMPAR}${r}
 
     Write Text Vision    campo_green    backend=uia    after=.2
-    ...    text=${LIMPAR}${g}      move_x=-35
+    ...    text=${LIMPAR}${g}
 
     Write Text Vision    campo_blue    backend=uia    after=.2
-    ...    text=${LIMPAR}${b}      move_x=-35
+    ...    text=${LIMPAR}${b}
 
     # Write Text Vision    campo_matiz      backend=uia
-    # ...    text=${LIMPAR}${matiz}    move_x=-30
+    # ...    text=${LIMPAR}${matiz}
 
     # Write Text Vision    campo_sat      backend=uia
-    # ...    text=${LIMPAR}${sat}    move_x=-30
+    # ...    text=${LIMPAR}${sat}
 
     # Write Text Vision    campo_lum    backend=uia
-    # ...    text=${LIMPAR}${lum}    move_x=-30
+    # ...    text=${LIMPAR}${lum}
 
     Click Vision    btn_ok_cor_definida    backend=uia
 
 
 Reduzir zoom
     Wait Element Vision    icone_paint
     Click Vision    btn_reduzir_zoom    backend=uia     after=0.5
@@ -144,15 +144,14 @@
         Click Coord     ${coord}[0]     ${coord}[1]
     END
 
 """
 
 
 CUSTOM_KEYWORDS = """
-
 import os
 from pathlib import Path
 
 import mouse
 import pyautogui
 
 
@@ -184,15 +183,15 @@
             if flag_levantado:
                 pyautogui.moveTo(x, y, .2)
                 pyautogui.sleep(0.01)
                 flag_levantado = False
             
             start_x, start_y = mouse.get_position()
 
-            pyautogui.sleep(0.01)
+            pyautogui.sleep(0.03)
             mouse.drag(start_x, start_y, x, y, absolute=True, duration=float(0.00003))
             pyautogui.sleep(0.01)
 
 
 def apagar_desenho():
     pyautogui.sleep(3)
     pyautogui.hotkey('ctrl', 'a')
```

### Comparing `rpapy-1.1.2/rpapy/core/utils/imagens/IMAGEM_NAO_ENCONTRADA.png` & `rpapy-1.1.3/rpapy/core/utils/imagens/IMAGEM_NAO_ENCONTRADA.png`

 * *Files identical despite different names*

### Comparing `rpapy-1.1.2/rpapy/core/utils/imagens/template_win11_screen_1920x1080.svg` & `rpapy-1.1.3/rpapy/core/utils/imagens/template_win11_screen_1920x1080.svg`

 * *Files identical despite different names*

### Comparing `rpapy-1.1.2/rpapy/core/utils/messages.py` & `rpapy-1.1.3/rpapy/core/utils/messages.py`

 * *Files identical despite different names*

### Comparing `rpapy-1.1.2/PKG-INFO` & `rpapy-1.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rpapy
-Version: 1.1.2
+Version: 1.1.3
 Summary: RPAPY is a open source easy tool for automating boring stuffs on any screen with robotframework, pyautogui, pywinauto and others.
 Home-page: https://github.com/codigo100cera/rpapy
 License: MIT
 Keywords: rpa,robotframework,automations,tools
 Author: Codigo Sem Cera
 Author-email: codigo100cera@gmail.com
 Requires-Python: >=3.10,<3.13
```

