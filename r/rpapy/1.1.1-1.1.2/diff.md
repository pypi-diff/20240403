# Comparing `tmp/rpapy-1.1.1.tar.gz` & `tmp/rpapy-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rpapy-1.1.1.tar", max compression
+gzip compressed data, was "rpapy-1.1.2.tar", max compression
```

## Comparing `rpapy-1.1.1.tar` & `rpapy-1.1.2.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rw-r--r--   0        0        0     1100 2024-02-24 15:05:07.143850 rpapy-1.1.1/LICENSE
--rw-r--r--   0        0        0     1881 2024-04-03 12:49:20.475924 rpapy-1.1.1/pyproject.toml
--rw-r--r--   0        0        0     3759 2024-04-03 12:46:39.139719 rpapy-1.1.1/README.md
--rw-r--r--   0        0        0       53 2024-04-03 12:49:20.510862 rpapy-1.1.1/rpapy/__init__.py
--rw-r--r--   0        0        0     7610 2024-04-03 12:49:20.513398 rpapy-1.1.1/rpapy/__main__.py
--rw-r--r--   0        0        0    16039 2024-04-03 12:46:20.286610 rpapy-1.1.1/rpapy/activities.py
--rw-r--r--   0        0        0        0 2024-03-11 23:33:14.532292 rpapy-1.1.1/rpapy/core/__init__.py
--rw-r--r--   0        0        0     1890 2024-04-03 12:46:20.288639 rpapy-1.1.1/rpapy/core/config.py
--rw-r--r--   0        0        0     1944 2024-04-03 12:46:20.289639 rpapy-1.1.1/rpapy/core/image_mapper.py
--rw-r--r--   0        0        0    15288 2024-04-03 12:46:20.291650 rpapy-1.1.1/rpapy/core/locator.py
--rw-r--r--   0        0        0     1030 2024-04-03 12:46:20.292639 rpapy-1.1.1/rpapy/core/prepare_text.py
--rw-r--r--   0        0        0     4847 2024-04-03 12:46:20.296253 rpapy-1.1.1/rpapy/core/snipps/__init__.py
--rw-r--r--   0        0        0    10433 2024-04-03 12:46:20.299191 rpapy-1.1.1/rpapy/core/snipps/codesnippets.py
--rw-r--r--   0        0        0     5670 2024-04-03 12:46:20.300199 rpapy-1.1.1/rpapy/core/snipps/loads.py
--rw-r--r--   0        0        0    11236 2024-03-31 01:57:48.660663 rpapy-1.1.1/rpapy/core/snipps/snippingtools.py
--rw-r--r--   0        0        0    13102 2024-04-03 12:46:20.301190 rpapy-1.1.1/rpapy/core/snipps/templates.py
--rw-r--r--   0        0        0      257 2024-03-23 01:44:02.673566 rpapy-1.1.1/rpapy/core/utils/__init__.py
--rw-r--r--   0        0        0        0 2024-02-24 15:05:07.224251 rpapy-1.1.1/rpapy/core/utils/example/__init__.py
--rw-r--r--   0        0        0    89781 2024-03-22 18:35:46.875840 rpapy-1.1.1/rpapy/core/utils/example/paint_robot.py
--rw-r--r--   0        0        0    31581 2024-02-24 15:05:07.236199 rpapy-1.1.1/rpapy/core/utils/imagens/IMAGEM_NAO_ENCONTRADA.png
--rw-r--r--   0        0        0  2623476 2024-03-22 18:17:08.029741 rpapy-1.1.1/rpapy/core/utils/imagens/template_win11_screen_1920x1080.svg
--rw-r--r--   0        0        0     6959 2024-04-03 12:46:20.304187 rpapy-1.1.1/rpapy/core/utils/messages.py
--rw-r--r--   0        0        0     4995 1970-01-01 00:00:00.000000 rpapy-1.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1100 2024-02-24 15:05:07.143850 rpapy-1.1.2/LICENSE
+-rw-r--r--   0        0        0     1881 2024-04-03 13:55:57.715491 rpapy-1.1.2/pyproject.toml
+-rw-r--r--   0        0        0     3759 2024-04-03 12:46:39.139719 rpapy-1.1.2/README.md
+-rw-r--r--   0        0        0       53 2024-04-03 13:55:57.757467 rpapy-1.1.2/rpapy/__init__.py
+-rw-r--r--   0        0        0     7606 2024-04-03 13:55:57.760460 rpapy-1.1.2/rpapy/__main__.py
+-rw-r--r--   0        0        0    16039 2024-04-03 12:46:20.286610 rpapy-1.1.2/rpapy/activities.py
+-rw-r--r--   0        0        0        0 2024-03-11 23:33:14.532292 rpapy-1.1.2/rpapy/core/__init__.py
+-rw-r--r--   0        0        0     1890 2024-04-03 12:46:20.288639 rpapy-1.1.2/rpapy/core/config.py
+-rw-r--r--   0        0        0     1944 2024-04-03 12:46:20.289639 rpapy-1.1.2/rpapy/core/image_mapper.py
+-rw-r--r--   0        0        0    15288 2024-04-03 12:46:20.291650 rpapy-1.1.2/rpapy/core/locator.py
+-rw-r--r--   0        0        0     1030 2024-04-03 12:46:20.292639 rpapy-1.1.2/rpapy/core/prepare_text.py
+-rw-r--r--   0        0        0     4847 2024-04-03 12:46:20.296253 rpapy-1.1.2/rpapy/core/snipps/__init__.py
+-rw-r--r--   0        0        0    10433 2024-04-03 12:46:20.299191 rpapy-1.1.2/rpapy/core/snipps/codesnippets.py
+-rw-r--r--   0        0        0     5670 2024-04-03 12:46:20.300199 rpapy-1.1.2/rpapy/core/snipps/loads.py
+-rw-r--r--   0        0        0    11236 2024-03-31 01:57:48.660663 rpapy-1.1.2/rpapy/core/snipps/snippingtools.py
+-rw-r--r--   0        0        0    13102 2024-04-03 12:46:20.301190 rpapy-1.1.2/rpapy/core/snipps/templates.py
+-rw-r--r--   0        0        0      257 2024-03-23 01:44:02.673566 rpapy-1.1.2/rpapy/core/utils/__init__.py
+-rw-r--r--   0        0        0        0 2024-02-24 15:05:07.224251 rpapy-1.1.2/rpapy/core/utils/example/__init__.py
+-rw-r--r--   0        0        0    89781 2024-03-22 18:35:46.875840 rpapy-1.1.2/rpapy/core/utils/example/paint_robot.py
+-rw-r--r--   0        0        0    31581 2024-02-24 15:05:07.236199 rpapy-1.1.2/rpapy/core/utils/imagens/IMAGEM_NAO_ENCONTRADA.png
+-rw-r--r--   0        0        0  2623476 2024-03-22 18:17:08.029741 rpapy-1.1.2/rpapy/core/utils/imagens/template_win11_screen_1920x1080.svg
+-rw-r--r--   0        0        0     6920 2024-04-03 13:33:10.772736 rpapy-1.1.2/rpapy/core/utils/messages.py
+-rw-r--r--   0        0        0     4995 1970-01-01 00:00:00.000000 rpapy-1.1.2/PKG-INFO
```

### Comparing `rpapy-1.1.1/LICENSE` & `rpapy-1.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `rpapy-1.1.1/pyproject.toml` & `rpapy-1.1.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "rpapy"
-version = "1.1.1"
+version = "1.1.2"
 description = "RPAPY is a open source easy tool for automating boring stuffs on any screen with robotframework, pyautogui, pywinauto and others."
 authors = ["Codigo Sem Cera <codigo100cera@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/codigo100cera/rpapy"
 include = ["LICENSE", "README.md", "*.cfg", "rpapy/core/utils/imagens/*.png", "rpapy/core/utils/imagens/*.svg"]
 keywords = ["rpa", "robotframework", "automations", "tools"]
```

### Comparing `rpapy-1.1.1/README.md` & `rpapy-1.1.2/README.md`

 * *Files identical despite different names*

### Comparing `rpapy-1.1.1/rpapy/__main__.py` & `rpapy-1.1.2/rpapy/__main__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """RPAPY is a open source easy tool for automating boring stuffs on any screen with robotframework, pyautogui, pywinauto and others.
 --------
 
-- rpapy v1.1.1
+- rpapy v1.1.2
 """
 import sys
 from pathlib import Path
 from unittest.mock import patch
 
 import pyperclip
 from pynput import keyboard, mouse
@@ -119,15 +119,15 @@
         self.hotkeys_thread = HotkeysThread(self)
         self.hotkeys_thread.change_file.connect(self._change_file)
         self.hotkeys_thread.capture_image.connect(self._capture_imagem)
         self.hotkeys_thread.set_backend_uia.connect(self.set_backend_uia)
         self.hotkeys_thread.set_backend_win32.connect(self.set_backend_win32)
         self.hotkeys_thread.inspect_element.connect(self._backend_inspect)
         self.hotkeys_thread.show_config.connect(self._show_config)
-        self.hotkeys_thread.load_example.connect(self._upload_example)
+        self.hotkeys_thread.load_example.connect(self._load_example)
         self.hotkeys_thread.update_image.connect(self._update_image)
         self.hotkeys_thread.off.connect(self._turn_off)
         self.hotkeys_thread.start()
 
         self.mouse_thread = MouseThread(self)
         self.mouse_thread.start()
         
@@ -155,15 +155,15 @@
         self.mouse_thread.listener.stop()
         print('>>>> Agente RPA desligado.')
         exit(0)
 
     def _show_config(self):
         message_to_set_timeout(self.config.get_config(), timeout=False)
 
-    def _upload_example(self):
+    def _load_example(self):
         load_robot_example()
 
     def set_backend_uia(self, backend: str):
         self.backend = backend
         print('>>>> Backend changed to "UIA".')             
 
     def set_backend_win32(self, backend: str):
```

### Comparing `rpapy-1.1.1/rpapy/activities.py` & `rpapy-1.1.2/rpapy/activities.py`

 * *Files identical despite different names*

### Comparing `rpapy-1.1.1/rpapy/core/config.py` & `rpapy-1.1.2/rpapy/core/config.py`

 * *Files identical despite different names*

### Comparing `rpapy-1.1.1/rpapy/core/image_mapper.py` & `rpapy-1.1.2/rpapy/core/image_mapper.py`

 * *Files identical despite different names*

### Comparing `rpapy-1.1.1/rpapy/core/locator.py` & `rpapy-1.1.2/rpapy/core/locator.py`

 * *Files identical despite different names*

### Comparing `rpapy-1.1.1/rpapy/core/prepare_text.py` & `rpapy-1.1.2/rpapy/core/prepare_text.py`

 * *Files identical despite different names*

### Comparing `rpapy-1.1.1/rpapy/core/snipps/__init__.py` & `rpapy-1.1.2/rpapy/core/snipps/__init__.py`

 * *Files identical despite different names*

### Comparing `rpapy-1.1.1/rpapy/core/snipps/codesnippets.py` & `rpapy-1.1.2/rpapy/core/snipps/codesnippets.py`

 * *Files identical despite different names*

### Comparing `rpapy-1.1.1/rpapy/core/snipps/loads.py` & `rpapy-1.1.2/rpapy/core/snipps/loads.py`

 * *Files identical despite different names*

### Comparing `rpapy-1.1.1/rpapy/core/snipps/snippingtools.py` & `rpapy-1.1.2/rpapy/core/snipps/snippingtools.py`

 * *Files identical despite different names*

### Comparing `rpapy-1.1.1/rpapy/core/snipps/templates.py` & `rpapy-1.1.2/rpapy/core/snipps/templates.py`

 * *Files identical despite different names*

### Comparing `rpapy-1.1.1/rpapy/core/utils/example/paint_robot.py` & `rpapy-1.1.2/rpapy/core/utils/example/paint_robot.py`

 * *Files identical despite different names*

### Comparing `rpapy-1.1.1/rpapy/core/utils/imagens/IMAGEM_NAO_ENCONTRADA.png` & `rpapy-1.1.2/rpapy/core/utils/imagens/IMAGEM_NAO_ENCONTRADA.png`

 * *Files identical despite different names*

### Comparing `rpapy-1.1.1/rpapy/core/utils/imagens/template_win11_screen_1920x1080.svg` & `rpapy-1.1.2/rpapy/core/utils/imagens/template_win11_screen_1920x1080.svg`

 * *Files identical despite different names*

### Comparing `rpapy-1.1.1/rpapy/core/utils/messages.py` & `rpapy-1.1.2/rpapy/core/utils/messages.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,30 +12,30 @@
     choices = ['OK', 'CANCEL']
 
     buttons = [sg.Button(choice, button_color=("black", "#e3b200")) for choice in choices]
 
     layout = [[text], buttons]
 
     window = sg.Window(
-        "Select Anchor",
+        title,
         layout,
         # icon="icon.ico",
         no_titlebar=True,
         background_color="#ffde27",
         element_justification="center",
         use_default_focus=False,
         keep_on_top=True
     )
 
     choice, _ = window.Read()
     window.Close()
     del(window)
 
     if choice is None or choice.upper() == 'CANCEL':
-        sg.popup_annoying(f'O processo foi cancelado', 
+        sg.popup(f'O processo foi cancelado', 
                           keep_on_top=True)
         return False
     return True
 
 
 def confirm_yes_no_cancel(text:str, title:str = 'Janela de Confirmação')-> bool:
     sg.ChangeLookAndFeel("SystemDefault")
@@ -45,15 +45,15 @@
     choices = ['YES', 'NO', 'CANCEL']
 
     buttons = [sg.Button(choice, button_color=("black", "#e3b200")) for choice in choices]
 
     layout = [[text], buttons]
 
     window = sg.Window(
-        "Select Anchor",
+        title,
         layout,
         # icon="icon.ico",
         no_titlebar=True,
         background_color="#ffde27",
         element_justification="center",
         use_default_focus=False,
         keep_on_top=True
@@ -80,15 +80,15 @@
     choices = ['YES', 'NO']
 
     buttons = [sg.Button(choice, button_color=("black", "#e3b200")) for choice in choices]
 
     layout = [[text], buttons]
 
     window = sg.Window(
-        "Select Anchor",
+        title,
         layout,
         # icon="icon.ico",
         no_titlebar=True,
         background_color="#ffde27",
         element_justification="center",
         use_default_focus=False,
         keep_on_top=True
```

### Comparing `rpapy-1.1.1/PKG-INFO` & `rpapy-1.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rpapy
-Version: 1.1.1
+Version: 1.1.2
 Summary: RPAPY is a open source easy tool for automating boring stuffs on any screen with robotframework, pyautogui, pywinauto and others.
 Home-page: https://github.com/codigo100cera/rpapy
 License: MIT
 Keywords: rpa,robotframework,automations,tools
 Author: Codigo Sem Cera
 Author-email: codigo100cera@gmail.com
 Requires-Python: >=3.10,<3.13
```

