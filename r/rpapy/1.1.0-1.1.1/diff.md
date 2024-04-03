# Comparing `tmp/rpapy-1.1.0.tar.gz` & `tmp/rpapy-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rpapy-1.1.0.tar", max compression
+gzip compressed data, was "rpapy-1.1.1.tar", max compression
```

## Comparing `rpapy-1.1.0.tar` & `rpapy-1.1.1.tar`

### file list

```diff
@@ -1,24 +1,23 @@
--rw-r--r--   0        0        0     1100 2024-02-24 15:05:07.143850 rpapy-1.1.0/LICENSE
--rw-r--r--   0        0        0     1860 2024-03-31 02:00:44.231206 rpapy-1.1.0/pyproject.toml
--rw-r--r--   0        0        0     3745 2024-03-25 01:16:01.410262 rpapy-1.1.0/README.md
--rw-r--r--   0        0        0     3431 2024-03-11 23:33:14.514133 rpapy-1.1.0/rpapy/.UserSnippetsVsCode/python.json
--rw-r--r--   0        0        0     5270 2024-03-11 23:33:14.516752 rpapy-1.1.0/rpapy/.UserSnippetsVsCode/robot.json
--rw-r--r--   0        0        0       51 2024-03-31 02:00:44.267684 rpapy-1.1.0/rpapy/__init__.py
--rw-r--r--   0        0        0     7477 2024-03-31 02:00:44.269683 rpapy-1.1.0/rpapy/__main__.py
--rw-r--r--   0        0        0    16151 2024-03-31 01:57:48.652748 rpapy-1.1.0/rpapy/activities.py
--rw-r--r--   0        0        0        0 2024-03-11 23:33:14.532292 rpapy-1.1.0/rpapy/core/__init__.py
--rw-r--r--   0        0        0     1719 2024-03-25 02:28:25.326274 rpapy-1.1.0/rpapy/core/config.py
--rw-r--r--   0        0        0     5708 2024-03-22 19:43:14.396835 rpapy-1.1.0/rpapy/core/loads.py
--rw-r--r--   0        0        0    17290 2024-03-31 01:57:48.654748 rpapy-1.1.0/rpapy/core/localizador.py
--rw-r--r--   0        0        0     1028 2024-03-11 23:33:14.561544 rpapy-1.1.0/rpapy/core/prepare_text.py
--rw-r--r--   0        0        0     5074 2024-03-31 01:57:48.657871 rpapy-1.1.0/rpapy/core/snipps/__init__.py
--rw-r--r--   0        0        0    10387 2024-03-11 23:33:14.593462 rpapy-1.1.0/rpapy/core/snipps/codesnippets.py
--rw-r--r--   0        0        0    11236 2024-03-31 01:57:48.660663 rpapy-1.1.0/rpapy/core/snipps/snippingtools.py
--rw-r--r--   0        0        0      257 2024-03-23 01:44:02.673566 rpapy-1.1.0/rpapy/core/utils/__init__.py
--rw-r--r--   0        0        0        0 2024-02-24 15:05:07.224251 rpapy-1.1.0/rpapy/core/utils/example/__init__.py
--rw-r--r--   0        0        0    89781 2024-03-22 18:35:46.875840 rpapy-1.1.0/rpapy/core/utils/example/paint_robot.py
--rw-r--r--   0        0        0    31581 2024-02-24 15:05:07.236199 rpapy-1.1.0/rpapy/core/utils/imagens/IMAGEM_NAO_ENCONTRADA.png
--rw-r--r--   0        0        0  2623476 2024-03-22 18:17:08.029741 rpapy-1.1.0/rpapy/core/utils/imagens/template_win11_screen_1920x1080.svg
--rw-r--r--   0        0        0     1138 2024-03-11 23:33:14.600032 rpapy-1.1.0/rpapy/core/utils/messages.py
--rw-r--r--   0        0        0    13753 2024-03-22 20:57:59.758019 rpapy-1.1.0/rpapy/core/utils/templates.py
--rw-r--r--   0        0        0     4939 1970-01-01 00:00:00.000000 rpapy-1.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1100 2024-02-24 15:05:07.143850 rpapy-1.1.1/LICENSE
+-rw-r--r--   0        0        0     1881 2024-04-03 12:49:20.475924 rpapy-1.1.1/pyproject.toml
+-rw-r--r--   0        0        0     3759 2024-04-03 12:46:39.139719 rpapy-1.1.1/README.md
+-rw-r--r--   0        0        0       53 2024-04-03 12:49:20.510862 rpapy-1.1.1/rpapy/__init__.py
+-rw-r--r--   0        0        0     7610 2024-04-03 12:49:20.513398 rpapy-1.1.1/rpapy/__main__.py
+-rw-r--r--   0        0        0    16039 2024-04-03 12:46:20.286610 rpapy-1.1.1/rpapy/activities.py
+-rw-r--r--   0        0        0        0 2024-03-11 23:33:14.532292 rpapy-1.1.1/rpapy/core/__init__.py
+-rw-r--r--   0        0        0     1890 2024-04-03 12:46:20.288639 rpapy-1.1.1/rpapy/core/config.py
+-rw-r--r--   0        0        0     1944 2024-04-03 12:46:20.289639 rpapy-1.1.1/rpapy/core/image_mapper.py
+-rw-r--r--   0        0        0    15288 2024-04-03 12:46:20.291650 rpapy-1.1.1/rpapy/core/locator.py
+-rw-r--r--   0        0        0     1030 2024-04-03 12:46:20.292639 rpapy-1.1.1/rpapy/core/prepare_text.py
+-rw-r--r--   0        0        0     4847 2024-04-03 12:46:20.296253 rpapy-1.1.1/rpapy/core/snipps/__init__.py
+-rw-r--r--   0        0        0    10433 2024-04-03 12:46:20.299191 rpapy-1.1.1/rpapy/core/snipps/codesnippets.py
+-rw-r--r--   0        0        0     5670 2024-04-03 12:46:20.300199 rpapy-1.1.1/rpapy/core/snipps/loads.py
+-rw-r--r--   0        0        0    11236 2024-03-31 01:57:48.660663 rpapy-1.1.1/rpapy/core/snipps/snippingtools.py
+-rw-r--r--   0        0        0    13102 2024-04-03 12:46:20.301190 rpapy-1.1.1/rpapy/core/snipps/templates.py
+-rw-r--r--   0        0        0      257 2024-03-23 01:44:02.673566 rpapy-1.1.1/rpapy/core/utils/__init__.py
+-rw-r--r--   0        0        0        0 2024-02-24 15:05:07.224251 rpapy-1.1.1/rpapy/core/utils/example/__init__.py
+-rw-r--r--   0        0        0    89781 2024-03-22 18:35:46.875840 rpapy-1.1.1/rpapy/core/utils/example/paint_robot.py
+-rw-r--r--   0        0        0    31581 2024-02-24 15:05:07.236199 rpapy-1.1.1/rpapy/core/utils/imagens/IMAGEM_NAO_ENCONTRADA.png
+-rw-r--r--   0        0        0  2623476 2024-03-22 18:17:08.029741 rpapy-1.1.1/rpapy/core/utils/imagens/template_win11_screen_1920x1080.svg
+-rw-r--r--   0        0        0     6959 2024-04-03 12:46:20.304187 rpapy-1.1.1/rpapy/core/utils/messages.py
+-rw-r--r--   0        0        0     4995 1970-01-01 00:00:00.000000 rpapy-1.1.1/PKG-INFO
```

### Comparing `rpapy-1.1.0/LICENSE` & `rpapy-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `rpapy-1.1.0/pyproject.toml` & `rpapy-1.1.1/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "rpapy"
-version = "1.1.0"
+version = "1.1.1"
 description = "RPAPY is a open source easy tool for automating boring stuffs on any screen with robotframework, pyautogui, pywinauto and others."
 authors = ["Codigo Sem Cera <codigo100cera@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/codigo100cera/rpapy"
 include = ["LICENSE", "README.md", "*.cfg", "rpapy/core/utils/imagens/*.png", "rpapy/core/utils/imagens/*.svg"]
 keywords = ["rpa", "robotframework", "automations", "tools"]
@@ -26,14 +26,15 @@
 python-dotenv = "^1.0.1"
 rpaframework = "^28.3.0"
 pytesseract = "^0.3.10"
 mouse = "^0.7.1"
 numpy = "^1.26.4"
 opencv-python = "^4.9.0.80"
 pysimplegui = "<5.0,>=4.0"
+keyring = "^25.1.0"
 
 [tool.poetry.scripts]
 rpapy = 'rpapy.__main__:main'
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^8.0.1"
 pytest-cov = "^4.1.0"
```

### Comparing `rpapy-1.1.0/README.md` & `rpapy-1.1.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -12,28 +12,28 @@
 
 ## Get started
 
 ### Windows
 
 The easiest way to install RPAPY is by using __pip install__
 
-- Download and install [Python 3.7](https://www.python.org)
+- Download and install [Python >=3.10, <3.13 ](https://www.python.org)
 
 - Install the latest version RPAPY on your machine:
 ```
 pip install rpapy
 ```
 
 However, it is advisable to use a virtual environment for an isolated installation of all requirements, this avoids conflicts with the python interpreter installed on the host machine:
 ```
 pip install virtualenv
 mkdir <your-project-name>
 cd <your-project-name>
-virtualenv create rpapy-env
-activate rpapy-ev
+virtualenv create rpapy-venv
+activate rpapy-venv
 pip install rpapy
 ```
 
 The construction of the project structure is accomplished by executing the following command in the terminal:
 ```
 rpapy
 ```
```

### Comparing `rpapy-1.1.0/rpapy/__main__.py` & `rpapy-1.1.1/rpapy/__main__.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,76 +1,77 @@
 """RPAPY is a open source easy tool for automating boring stuffs on any screen with robotframework, pyautogui, pywinauto and others.
 --------
 
-- rpapy v1.1.0
+- rpapy v1.1.1
 """
 import sys
 from pathlib import Path
 from unittest.mock import patch
 
 import pyperclip
 from pynput import keyboard, mouse
 from PySide6.QtCore import QObject, QThread, Signal
 from PySide6.QtWidgets import QApplication
 
 with patch("ctypes.windll.user32.SetProcessDPIAware", autospec=True):
     import pyautogui  # noqa # pylint:disable=unused-import
 
-from rpapy.core.loads import (create_default_script_file,
-                              create_robot_default_dirs, load_robot_example)
+from rpapy.core.config import Config
 from rpapy.core.snipps import capture_image_crop, update_image
+from rpapy.core.snipps.loads import (create_default_script_file,
+                                     load_robot_example)
 from rpapy.core.utils import draw_outline
-from rpapy.core.utils.messages import message_to_set_timeout
+from rpapy.core.utils.messages import message_to_set_timeout, select_item_list
 
 
-def get_position_element(x, y):
+def get_element_position(x, y):
     print('{0} at {1}'.format('Pressed', (x, y)))
     pyperclip.copy('{0}, {1}'.format(x, y))
 
 
 class MouseThread(QThread):
-    controle_key = keyboard.Controller()
+    key_controll = keyboard.Controller()
 
     def run(self):
         
         def on_move(x, y):   
             positionStr = 'X: ' + str(x).rjust(4, ' ') + ' Y: ' + str(y).rjust(4, ' ')
             print(positionStr, end='')
             print('\b' * len(positionStr), end='', flush=True)            
             
         def on_click(x, y, button, pressed):
             if pressed:        
-                # get_position_element(x, y)
+                # get_element_position(x, y)
                 pass
 
         # ...or, in a non-blocking fashion:
         self.listener = mouse.Listener(
             on_move=on_move,
             on_click=on_click)
         self.listener.start()
 
 
 class HotkeysThread(QThread):
-    capiturar_imagem = Signal(object)
-    alterar_arquivo = Signal(bool)
+    capture_image = Signal(object)
+    change_file = Signal(bool)
     set_backend_uia = Signal(object)
     set_backend_win32 = Signal(object)
     show_config = Signal()
     load_example = Signal()
     inspect_element = Signal()
     update_image = Signal()
     off = Signal(object)
 
     def run(self):
         flag_backend = True
-        def capiturar_imagem():
-            self.capiturar_imagem.emit('Alterar imagem')
+        def capture_image():
+            self.capture_image.emit('Change image')
 
-        def alterar_arquivo():
-            self.alterar_arquivo.emit(True)
+        def change_file():
+            self.change_file.emit(True)
         
         def set_backend_uia_win32():
             nonlocal flag_backend
             flag_backend = not flag_backend
             if flag_backend:
                 self.set_backend_uia.emit('uia')
             else:
@@ -88,16 +89,16 @@
         def load_example():
             self.load_example.emit()
 
         def turn_off_agentpy():
             h.stop()
                 
         with keyboard.GlobalHotKeys({
-                '<ctrl>+<alt>+p': capiturar_imagem,
-                '<ctrl>+<alt>+r': alterar_arquivo,
+                '<ctrl>+<alt>+p': capture_image,
+                '<ctrl>+<alt>+r': change_file,
                 '<ctrl>+<alt>+b': set_backend_uia_win32,
                 '<ctrl>+<alt>+u': update_image,
                 '<ctrl>+i':       inspect_element,
                 '<ctrl>+<cmd>+c': show_config,
                 '<ctrl>+<cmd>+e': load_example,
                 '<ctrl>+<cmd>+x': turn_off_agentpy}) as h:
             h.join()
@@ -105,24 +106,23 @@
         self.off.emit('Global hotkey turned_off_agent.')
 
 
 class AgentPy(QObject):
     
     def __init__(self, config=None):
         super(AgentPy, self).__init__()
-        from rpapy.core.config import Config
-
-        self._config: Config = Config if config is None else config
+        
+        self.config: Config = Config if config is None else config
 
-        self._nome_arquivo = 'main.robot'
+        self._file_name = 'main.robot'
         self.backend = 'uia'
 
         self.hotkeys_thread = HotkeysThread(self)
-        self.hotkeys_thread.alterar_arquivo.connect(self._change_file)
-        self.hotkeys_thread.capiturar_imagem.connect(self._capiturar_imagem)
+        self.hotkeys_thread.change_file.connect(self._change_file)
+        self.hotkeys_thread.capture_image.connect(self._capture_imagem)
         self.hotkeys_thread.set_backend_uia.connect(self.set_backend_uia)
         self.hotkeys_thread.set_backend_win32.connect(self.set_backend_win32)
         self.hotkeys_thread.inspect_element.connect(self._backend_inspect)
         self.hotkeys_thread.show_config.connect(self._show_config)
         self.hotkeys_thread.load_example.connect(self._upload_example)
         self.hotkeys_thread.update_image.connect(self._update_image)
         self.hotkeys_thread.off.connect(self._turn_off)
@@ -153,60 +153,65 @@
     def _turn_off(self):
         print('\nTurn off')
         self.mouse_thread.listener.stop()
         print('>>>> Agente RPA desligado.')
         exit(0)
 
     def _show_config(self):
-        message_to_set_timeout(self._config.get_config(), timeout=False)
+        message_to_set_timeout(self.config.get_config(), timeout=False)
 
     def _upload_example(self):
         load_robot_example()
 
     def set_backend_uia(self, backend: str):
         self.backend = backend
-        print('>>>> Backend alterado para "UIA".')             
+        print('>>>> Backend changed to "UIA".')             
 
     def set_backend_win32(self, backend: str):
         self.backend = backend        
-        print('>>>> Backend alterado para "WIN32".')             
+        print('>>>> Backend changed to "WIN32".')             
     
     def _backend_inspect(self):
         x, y = pyautogui.position()
-        get_position_element(x, y)
+        get_element_position(x, y)
         draw_outline(x, y, backend=self.backend)
 
-    def _capiturar_imagem(self):
-        capture_image_crop(self._nome_arquivo)
+    def _capture_imagem(self):
+        capture_image_crop(self._file_name)
 
     def _change_file(self):        
-        file_name = create_default_script_file(default_name=self._nome_arquivo)
+        file_name = create_default_script_file(default_name=self._file_name)
         if file_name is None:
-            pyautogui.alert(title='RPAPY', text='O agente foi cancelado.')
+            pyautogui.alert(title='RPAPY', text='O agente será desligado.')
             pyautogui.hotkey('ctrl', 'win', 'x')
             return
-        self._nome_arquivo = file_name
+        self._file_name = file_name
     
     def _update_image(self):
-        from rpapy.core.config import Config
-        from rpapy.core.localizador import mapear_imagens
+        from rpapy.core.image_mapper import map_images
+
+        map_images_regions_anchors = map_images()        
+        image_name_list = list(map_images_regions_anchors)
+
+        image_name = select_item_list(text='Selecione o nome da imagem a ser atualizada',
+                                      title='Update Image',
+                                      item_type_name='Image',
+                                      item_list=image_name_list,
+                                      index=0)
         
-        default_name  = pyperclip.paste()
-        image_name = pyautogui.prompt(text='Insirá o nome da imagem a ser atualizada', 
-                                      title='Atualização de imagem', default=default_name)    
         if image_name is None or image_name.strip() == '':
             return
 
-        image_name_path = mapear_imagens().get(image_name, {}).get('image')
+        image_name_path = map_images_regions_anchors.get(image_name, {}).get('image')
 
         if image_name_path is not None:
             update_image(image_name_path)
         else:
             pyautogui.alert(title='RPAPY',
-                            text=f'A imagem "{image_name}" não foi encontrada no diretório {Config.IMAGES_DIR_NAME}.')
+                            text=f'A imagem "{image_name}" não foi encontrada no diretório {self.config.IMAGES_DIR_NAME}.')
 
 
 def main():
     app = QApplication.instance()
     if app is None:
         app = QApplication(sys.argv)
     agent = AgentPy()
```

### Comparing `rpapy-1.1.0/rpapy/activities.py` & `rpapy-1.1.1/rpapy/activities.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,38 +1,37 @@
 import contextlib
 from typing import Tuple
 
-from pywinauto import Desktop
-
-from rpapy.core.localizador import LocalizadorImagem, max_wait_attr
-from rpapy.core.prepare_text import prepare_text_to_pyautogui
-from rpapy.core.snipps.snippingtools import ImageNotFoundError
+from rpapy.core.locator import LocatorImage, max_wait_attr
+from rpapy.core.prepare_text import prepare_text_for_pyautogui
 
 ###########################################################
-_identifier_img = LocalizadorImagem()
+_identifier_img = LocatorImage()
 ###########################################################
 
+
 def toast_process_start_notifier():
     print('\n>>>> Robo.py iniciando processo...')
 
 
-def _get_ui_element(x: int, y: int,*,attr_name: str, backend: Desktop, wait_attr: float):
+def _get_ui_element(x: int, y: int,*,attr_name: str, backend: 'Desktop', wait_attr: float):
+    from pywinauto import Desktop
     UI_element = Desktop(backend=backend).from_point(x, y)
     max_wait_attr(UI_element, attr_name=attr_name, max_wait=wait_attr)
     return UI_element
 
 
 def wait_element_vision(*args, **kwargs):
     get_element_vision(*args, **kwargs)
 
 
 def get_element_vision(image_name: str, *args,        
         attr_name: str=None,
-        identifier_img: LocalizadorImagem=None,
-        backend: str=None,             # As opções são: 'uia' ou 'win32'
+        identifier_img: LocatorImage=None,
+        backend: str=None,             # Options: 'uia' ou 'win32'
         before: float=0.0,
         after: float=0.0,
         max_wait: float=None, 
         interval: float=None,
         confidence: float=None,
         wait_vanish: bool=False,
         execute: bool=False,
@@ -106,15 +105,15 @@
         return UI_element
     else:
         raise Exception(f'O backend "{backend}" não identificado.')
 
 
 def write_text_vision(image_name: str,*,
         text: str,
-        identifier_img: LocalizadorImagem=None,
+        identifier_img: LocatorImage=None,
         backend: str=None,             # As opções são: 'uia' ou 'win32'
         max_wait: float=None, 
         wait_vanish: bool=False,
         move_x: int=0,
         move_y: int=0,
         delay: float=0.0,
         before: float=0.0,
@@ -123,26 +122,26 @@
         confidence: float=None,
         wait_attr: float=5.0,
         ignore_error:bool=False,
         ignore_set_focus: bool=False):
 
     attr_name = 'type_keys' if backend is not None else 'press'
     if backend is None:
-        text = prepare_text_to_pyautogui(text)
+        text = prepare_text_for_pyautogui(text)
 
     execute = True
     
     return get_element_vision(image_name, text, identifier_img=identifier_img, backend=backend, max_wait=max_wait, 
                                 attr_name=attr_name, wait_vanish=wait_vanish, move_x=move_x, move_y=move_y, delay=delay, 
                                 before=before, after=after, interval=interval, confidence=confidence, wait_attr=wait_attr, 
                                 execute=execute, ignore_error=ignore_error, ignore_set_focus=ignore_set_focus)
 
 
 def click_vision(image_name: str,*,
-        identifier_img: LocalizadorImagem=None,
+        identifier_img: LocatorImage=None,
         backend: str=None,             # As opções são: 'uia' ou 'win32'
         button: str='left',
         max_wait: float=None, 
         move_x: int=0,
         move_y: int=0,
         delay: float=0.0,
         before: float=0.0,
@@ -159,15 +158,15 @@
     return get_element_vision(image_name,attr_name=attr_name, identifier_img=identifier_img, backend=backend, 
                                 button=button, delay=delay, before=before, after=after, max_wait=max_wait, 
                                 interval=interval, confidence=confidence, wait_vanish=wait_vanish, wait_attr=wait_attr, 
                                 move_x=move_x, move_y=move_y,ignore_error=ignore_error, execute=execute)
 
 
 def double_click_vision(image_name: str,*,
-        identifier_img: LocalizadorImagem=None,
+        identifier_img: LocatorImage=None,
         button: str='left',
         delay: float=0.0,
         before: float=0.0,
         after: float=0.0,
         max_wait: float=None, 
         interval: float=None,
         confidence: float=None,
@@ -185,15 +184,15 @@
     return get_element_vision(image_name,attr_name=attr_name, identifier_img=identifier_img, backend=backend, 
                                 button=button, delay=delay, before=before, after=after, max_wait=max_wait, interval=interval, 
                                 confidence=confidence, wait_vanish=wait_vanish, wait_attr=wait_attr, move_x=move_x, move_y=move_y,
                                 ignore_error=ignore_error, execute=execute, ignore_set_focus=ignore_set_focus)
 
 
 def triple_click_vision(image_name: str,*,
-        identifier_img: LocalizadorImagem=None,
+        identifier_img: LocatorImage=None,
         button: str='left',
         delay: float=0.1,
         before: float=0.0,
         after: float=0.0,
         max_wait: float=None, 
         interval: float=None,
         confidence: float=None,
@@ -273,15 +272,15 @@
         before: float=0.0,
         after: float=0.0,
         backend: str=None,             # As opções são: 'uia' ou 'win32'
         wait_attr: float=5.0):
 
     attr_name = 'type_keys' if backend is not None else 'press'
     if backend is None:
-        text = prepare_text_to_pyautogui(text)    
+        text = prepare_text_for_pyautogui(text)    
 
     return get_element_coord(x, y, text, attr_name=attr_name, backend=backend, before=before, after=after, delay=delay, wait_attr=wait_attr)
     
 
 def click_coord(x: int, y: int,
         button: str='left',
         delay: float=0.0,
@@ -317,15 +316,15 @@
         wait_attr: float=5.0):
 
     attr_name = 'triple_click_input' if backend is not None else 'doubleClick'
 
     return get_element_coord(x, y, button=button, attr_name=attr_name, backend=backend, before=before, after=after, delay=delay, wait_attr=wait_attr)
 
 
-def get_text_ocr_vision(image_name, region:Tuple[int], *args, identifier_img: LocalizadorImagem=None, lang: str='por', **kwargs) -> str:
+def get_text_ocr_vision(image_name, region:Tuple[int], *args, identifier_img: LocatorImage=None, lang: str='por', **kwargs) -> str:
     import pytesseract as ocr
     from pyautogui import screenshot
 
     coordinate = wait_element_vision(image_name,identifier_img=identifier_img, **kwargs)
     
     image_region = screenshot(region=region)
     ocr_text_result = ocr.image_to_string(image_region, lang=lang)
@@ -439,9 +438,9 @@
         sleep(1)
         if windows_list:
             break
     return windows_list
 
 
 def get_path_by_image_name(image_name: str)-> str:
-    from rpapy.core.localizador import get_absolute_path_by_image_name
+    from rpapy.core.locator import get_absolute_path_by_image_name
     return get_absolute_path_by_image_name(image_name)
```

### Comparing `rpapy-1.1.0/rpapy/core/loads.py` & `rpapy-1.1.1/rpapy/core/snipps/loads.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,25 +1,61 @@
 import contextlib
 import os
-from pathlib import Path
 import shutil
+from pathlib import Path
+from typing import Dict, Tuple
 
 import pyautogui
 
-from .config import Config
-from .utils import templates
+from rpapy.core.utils.messages import confirm_ok_cancel, prompt
+
+from ..config import Config
+
+
+def create_python_default_dirs():
+    path_dir_resources = Path(Config.BASE_DIR, Config.RESOURCES_DIR_NAME)
+    with contextlib.suppress(FileExistsError):
+        path_dir_resources.mkdir()
+
+    path_dir_images = Path(path_dir_resources, Config.IMAGES_DIR_NAME)
+    with contextlib.suppress(FileExistsError):
+        path_dir_images.mkdir()
+
+    error_images_dir_path = path_dir_resources / Config.IMAGES_ERROR_DIR_NAME
+    with contextlib.suppress(FileExistsError):
+        error_images_dir_path.mkdir()
+
+
+def replace_file_confirm(path_file: Path, content: str = None,* , origin_file: Path = None):
+    if path_file.exists():
+        text = f'O arquivo "{path_file.name}" será subistuido, para confirmar clique em OK.'
+        opcao = confirm_ok_cancel(text=text, title='RPA-PY')        
+        if opcao:
+            if '.py' in path_file.name:
+                path_file.write_text(content)
+            elif '.svg' in path_file.name:
+                shutil.copy(origin_file, path_file)
+            else:
+                path_file.write_text(content, encoding='utf-8')            
+    else:
+        if '.py' in path_file.name:
+                path_file.write_text(content)
+        elif '.svg' in path_file.name:
+            shutil.copy(origin_file, path_file)
+        else:
+            path_file.write_text(content, encoding='utf-8')
 
 
 def load_robot_example():
 
     from rpapy.core.utils.example import paint_robot
 
     text = f'***ATENÇÃO***\n\nAlguns arquivos poderão ser substituidos!\nVocê deseja carregar a implementação de exemplo do robo-rpapy?'
-    opcao = pyautogui.confirm(text=text, title='RPA-PY', buttons=['OK','CANCEL'])        
-    if opcao is None or opcao == 'CANCEL':
+    opcao = confirm_ok_cancel(text=text, title='RPA-PY')        
+    if not opcao:
         return
 
     pyautogui.alert(title='ATENÇÃO!', text='Após terminar de carregar os arquivos, execute\no seguinte comando no terminal:\n\nrobot -d log tasks')
 
     create_example_default_dirs()
     create_robot_default_dirs()
 
@@ -39,70 +75,35 @@
     replace_file_confirm(path_main_robot, paint_robot.MAIN_ROBOT)
 
     origin_file_svg = Path(HERE) / 'utils/imagens/template_win11_screen_1920x1080.svg'
     svg_template_path = Path(Config.BASE_DIR, 'resources/desenhos/template_win11_screen_1920x1080.svg')
     replace_file_confirm(svg_template_path, origin_file=origin_file_svg)
 
 
-def replace_file_confirm(path_file: Path, content: str = None,* , origin_file: Path = None):
-    if path_file.exists():
-        text = f'O arquivo "{path_file.name}" será subistuido, para confirmar clique em OK.'
-        opcao = pyautogui.confirm(text=text, title='RPA-PY', buttons=['OK','CANCEL'])        
-        if opcao is not None or opcao != 'CANCEL':
-            if '.py' in path_file.name:
-                path_file.write_text(content)
-            elif '.svg' in path_file.name:
-                shutil.copy(origin_file, path_file)
-            else:
-                path_file.write_text(content, encoding='utf-8')            
-    else:
-        if '.py' in path_file.name:
-                path_file.write_text(content)
-        elif '.svg' in path_file.name:
-            shutil.copy(origin_file, path_file)
-        else:
-            path_file.write_text(content, encoding='utf-8')
-
-
 def create_robot_default_dirs():
-
     path_dir_task = Path(Config.BASE_DIR, Config.TASKS_DIR_NAME)
     with contextlib.suppress(FileExistsError):
         path_dir_task.mkdir()
 
     create_python_default_dirs()  
 
 
-def create_python_default_dirs():
-
-    path_dir_resources = Path(Config.BASE_DIR, Config.RESOURCES_DIR_NAME)
-    with contextlib.suppress(FileExistsError):
-        path_dir_resources.mkdir()
-
-    path_dir_images = Path(path_dir_resources, Config.IMAGES_DIR_NAME)
-    with contextlib.suppress(FileExistsError):
-        path_dir_images.mkdir()
-
-    error_images_dir_path = path_dir_resources / Config.IMAGES_ERROR_DIR_NAME
-    with contextlib.suppress(FileExistsError):
-        error_images_dir_path.mkdir()
-
-
-def create_example_default_dirs():
-    
+def create_example_default_dirs():    
     create_python_default_dirs()
-    path_desenhos_dir = Path(Config.BASE_DIR, Config.RESOURCES_DIR_NAME, 'desenhos')
+    draw_dir_path = Path(Config.BASE_DIR, Config.RESOURCES_DIR_NAME, 'desenhos')
     with contextlib.suppress(FileExistsError):
-        path_desenhos_dir.mkdir()
+        draw_dir_path.mkdir()
+
 
+def create_default_script_file(*, file_name:str=None, default_name:str='main.robot'):
+    from . import templates
 
-def create_default_script_file(*, file_name:str=None, default_name:str='main.robot'):    
     if file_name is None:
-        file_name = pyautogui.prompt(text='Insirá o nome do arquivo com extensão .robot ou .py', title='Alteração de Arquivo', default=default_name)    
-        if file_name is None:
+        file_name = prompt(text='Insirá o nome do arquivo com extensão .robot ou .py', title='Alteração de Arquivo', default=default_name)
+        if file_name is False:
             return
 
     file_name = default_name if file_name is None or file_name.strip() == '' else file_name
 
     name, extention, *_ = file_name.lower().split('.')
 
     file_name = file_name if extention == 'py' or extention == 'robot' else f'{name}.robot'
```

### Comparing `rpapy-1.1.0/rpapy/core/localizador.py` & `rpapy-1.1.1/rpapy/core/locator.py`

 * *Files 22% similar despite different names*

```diff
@@ -6,71 +6,72 @@
 from typing import Dict, Tuple
 
 import cv2
 import numpy as np
 import pyautogui
 from PIL import Image
 
+from rpapy.core.utils.messages import confirm_ok_cancel, confirm_yes_no_cancel
+
 with warnings.catch_warnings():
         warnings.simplefilter("ignore")
         from pywinauto import Desktop
 
-from rpapy.core.loads import create_python_default_dirs
+from rpapy.core.image_mapper import map_images
+from rpapy.core.snipps.loads import create_python_default_dirs
 
 from .config import Config
 from .snipps import update_image
 from .snipps.snippingtools import (ImageNotDisappearError, ImageNotFoundError,
                                    close_window_with_title)
 
-MODO_MANUTENCAO = False
-if Config.VERIFICAR_MODO:
-    MODOS = {'SIM':True, 'NAO': False, None:'CANCEL'}
-    MODO_MANUTENCAO = MODOS[pyautogui.confirm(title='RPAPY',text='Ativar o modo de manutenção?', buttons=['SIM', 'NAO'])]
-
-if MODO_MANUTENCAO == 'CANCEL': 
-    pyautogui.alert(title='RPAPY', text='O processo foi cancelado!')
+MAINTENANCE_MODE = False
+if Config.CHECK_MODE:
+    MAINTENANCE_MODE = confirm_yes_no_cancel(title='RPAPY',text='Ativar o modo de manutenção?')
+
+if MAINTENANCE_MODE is None: 
+    pyautogui.hotkey('ctrl', 'win', 'x')
+    pyautogui.sleep(2)
     exit()
 
-if MODO_MANUTENCAO is False:
+if MAINTENANCE_MODE is False:
     pyautogui.FAILSAFE = False
 
 if Config.FAILSAFE_OFF:    
     pyautogui.FAILSAFE = False
 
-path_base_dir = Path(Config.BASE_DIR)
-path_dir_resources = Path(path_base_dir, Config.RESOURCES_DIR_NAME)
-path_dir_images =  Path(path_dir_resources, Config.IMAGES_DIR_NAME)
-path_dir_error_images = Path(path_dir_resources, Config.IMAGES_ERROR_DIR_NAME)
+images_dir_path =  Config.IMAGES_DIR_PATH
+error_images_dir_path = Config.ERROR_IMAGES_DIR_PATH
 
 
-def localizar_na_tela(image, *args, **kwargs):
+def locate_on_screen(image, *args, **kwargs):
     try:
         img = Image.open(image)
         return pyautogui.locateOnScreen(img, *args, **kwargs)
     except ValueError:
         pass
 
 
-class LocalizadorImagem():
+class LocatorImage():
 
     def __init__(self):
-        self._screenshots: Dict[str, Tuple[int]] = mapear_imagens()
+        self._screenshots: Dict[str, Dict[str, Tuple[int]]] = map_images()
         self.wait_before = 0.0
         self.debug = False
         self._interval = 0.2
-        self._max_wait = Config.MAX_WAIT_MANUTENCAO if MODO_MANUTENCAO else 30
-        self._modo_manutencao = MODO_MANUTENCAO
+        self._max_wait = Config.MAX_WAIT_MAINTENANCE if MAINTENANCE_MODE else 30
+        self._maintenance_mode = MAINTENANCE_MODE
 
-    def modo_manutencao(self, opcao: bool):
-        if isinstance(opcao, bool):
-            if opcao:
-                self._modo_manutencao = opcao
+    def modo_manutencao(self, option: bool):
+        if isinstance(option, bool):
+            if option:
+                self._maintenance_mode = option
                 self._max_wait = 10
             else:
-                self._modo_manutencao = opcao
+                self._maintenance_mode = option
                 self._max_wait = 30
 
     @property
     def max_wait(self):
         return self._max_wait
 
     @max_wait.setter
@@ -97,258 +98,212 @@
                  confidence: float=None, 
                  wait_vanish=False,
                  interval: float=None, 
                  deslocar_x:int=0, 
                  deslocar_y:int=0, 
                  ignore_error: bool=False) -> Tuple[int]:
         
-        """Busca a imagem na tela até o tempo máximo definido por parâmetro, e retorna 
-        a coordenada da imagem se encontrada, senão lança uma excessão personalizada ImageNotFoundError.
+        """Searches the image on the screen until the maximum time defined by parameter, and returns
+        the image coordinate if found, otherwise it throws the custom exception ImageNotFoundError.
         Arguments:
-            image {str} -- nome da imagem a ser recuperada no dicionário
+            image {str} -- name of the image to be retrieved from the dictionary
         Keyword Arguments:
-            max_wait {float} -- [tempo máximo de espera para encontra a imagem] (default: {None})
-            interval {float} -- [intervalo de parada para busca da imagem] (default: {None})
-            deslocar_x {int} -- [desloca o centro da localização da imagem no eixo x] (default: {0})
-            deslocar_y {int} -- [desloca o centro da localização da imagem no eixo] (default: {0})
+            max_wait {float} -- maximum waiting time to find the image (default: {None})
+            interval {float} -- stop interval for image search (default: {None})
+            deslocar_x {int} -- shifts the center of the image location on the x-axis (default: {0})
+            deslocar_y {int} -- shifts the center of the image location on the y-axis (default: {0})
         Raises:
-            ImageNotFoundError: [Excessão lançada quando a imagem não for encontrada dentro do prazo máximo]
+            ImageNotFoundError: Excess thrown when the image is not found within the maximum period
         Returns:
-            Tuple[int] -- [tupla contendo os valores (x, y) do centro da imagem identificada]
+            Tuple[int] -- tuple containing the values ​​(x, y) of the center of the identified image
         """
-        # Se True efetua uma parada a cada execução. Utilizado para reduzir a velocidade do bot.
+        # If True performs a stop at each execution. Used to reduce the speed of the bot.
         if self.debug:
             input(f'Localizar "{image_name}" - Pressione enter para continuar...')
 
-        # Atribui ao interval_local o intervalo passado por parâmetro, de diferente de None
+        # Assigns to interval_local the interval passed as a parameter, other than None.
         if interval is not None:
             if interval > 0:
                 interval_local = interval
             else:
                 interval_local = self._interval
         else:
             interval_local = self._interval
 
-        # Atribui ao max_wait_local o tempo máximo passado por parâmetro, se diferente de None
+        # Assigns to max_wait_local the maximum time passed per parameter, if different from None.
         if max_wait is not None:
             max_wait = float(max_wait)
             if max_wait > 0 and max_wait > interval_local:
                 max_wait_local = max_wait
             else:
                 max_wait_local = self._max_wait
         else:
             max_wait_local = self._max_wait
         
-        # Efetua uma pausa antes de tentar encontrar a localização da imagem
+        # Pauses before trying to find the image location.
         time.sleep(self.wait_before)
 
-        # Move o mouse para um ponto de descanso na tela para não interferir na busca da imagem
+        # Moves the mouse to a resting point on the screen so as not to interfere with the image search.
         pyautogui.moveTo(700,5,0)
 
-        # Inicia a coordenada com o padrão flag None
+        # Starts the coordinate with the default flag None.
         coordenada = None
 
-        # Armazena o início da execução do método para ser verificado com o max_wait
+        # Registers the start of method execution to be checked with max_wait.
         start_time = time.time()
 
         if not wait_vanish:
-            # Repete o bloco de codigo, enquanto variável coordenada for igual a None
+            # Repeat the code block as long as the coordinate variable is equal to None.
             while coordenada is None:
                 try:
-                    # recupera a imagem do mapa, passando o nome enviado por parâmetro
+                    # retrieves the map image, passing the name sent as a parameter.
                     image_region = {
                         'image': self._screenshots[image_name]['image'],
                         'region': self._screenshots[image_name]['region']
                     }
                 except KeyError:
-                    # Cria um arquivo com image_name no diretório images se não existir
+                    # Create a file with image_name in the images directory if it does not exist
                     im = Image.open(os.path.join(os.path.abspath(os.path.dirname(__file__)),'utils/imagens/IMAGEM_NAO_ENCONTRADA.png'))
-                    im.save(f'{path_dir_images}/{image_name}-(300, 50, 700, 200).png', 'PNG')
+                    im.save(f'{images_dir_path}/{image_name}-(300, 50, 700, 200).png', 'PNG')
                     time.sleep(1)
-                    # Atualiza o mapa com a imagem criada com o paramêtro image_name.
-                    self._screenshots = mapear_imagens()
+                    # Updates the map with the image created with the image_name parameter.
+                    self._screenshots = map_images()
                     continue
                 
                 try:
-                    # Executa o bloco else se a imagem for encontrada no mapa e efetua um continue para sair do loop
+                    # Executes the else block if the image is found on the map and continues to exit the loop.
                     if confidence is None:
-                        coordenada = localizar_na_tela(**image_region)
+                        coordenada = locate_on_screen(**image_region)
                     else:
-                        coordenada = localizar_na_tela(**image_region, confidence=confidence)
+                        coordenada = locate_on_screen(**image_region, confidence=confidence)
 
                     if coordenada is not None:
                         continue
                 except Exception:
                     coordenada = None
                     
-                # Entra no bloco se o tempo de execução do loop exceder o max_wait.
+                # Enter block if loop execution time exceeds max_wait.
                 if time.time() - start_time > max_wait_local:
-                    if self._modo_manutencao:
+                    if self._maintenance_mode:
                         atualizou = update_image(image_region.get('image'))
                         if atualizou:
-                            self._screenshots = mapear_imagens()
+                            self._screenshots = map_images()
                             image_region = {
                                 'image': self._screenshots[image_name]['image'],
                                 'region': self._screenshots[image_name]['region']
                             }
                         start_time = time.time()
                     elif not ignore_error:
-                        # Efetua um print da tela no momento em que ocorreu o erro
+                        # Take a screenshot of the screen at the time the error occurred.
                         image_not_found_error = pyautogui.screenshot()
-                        # Salva o print da tela com o nome da imagem que não foi encontrada, incluindo data e hora
+                        # Saves the screenshot with the name of the image that was not found, including date and time.
                         salvar_img_error(image_name, image_not_found_error)
-                        # Lança a exceção de imagem não encotrada.
+                        # Throws the image not found exception.
                         raise ImageNotFoundError(f'A imagem "{image_name}", não foi encontrada!')
 
-                # Efetua um intervalo de parada entre os loop de tentativa de encontrar a imagem
+                # Take a timeout between loops trying to find the image.
                 time.sleep(interval_local)
             else:
-                # Se o loop for encerrado na condicional do while, este bloco é executado.            
-                # Recupera a coordenada x,y do centro da imagem encontrada.
+                
+                # If the loop is terminated in the while conditional, this block is executed.
+                # Retrieves the x,y coordinate of the center of the found image.
                 resultado = pyautogui.center(coordenada)
 
-                # Recupera as coordenadas da ancora para aplicar o deslocamento
+                # Retrieves the anchor coordinates to apply the displacement
                 anchor_coord = self._screenshots[image_name]['anchor_coord']
                 if anchor_coord is not None and deslocar_x + deslocar_y == 0:
                     deslocar_x, deslocar_y = anchor_coord
 
-                # Retorna o resultado adionando os deslocamentos, se passados por parâmetro.
+                # Returns the result adding the displacements, if passed by parameter.
                 return resultado[0] + int(deslocar_x), resultado[-1] + int(deslocar_y)
         
         else:
-            # Armazena o início da execução do método para ser verificado com o max_wait
+            # Stores the start of method execution to be checked with max_wait.
             start_time = time.time()
 
-            # Define coordenada diferente de None para iniciar o loop while
+            # Sets a coordinate other than None to start the while loop.
             coordenada = True
 
-            # Verifica se a imagem buscada na tela desapareceu            
+            # Checks whether the image searched for on the screen has disappeared.            
             while coordenada is not None:
                 try:
-                    # recupera a imagem do mapa, passando o nome enviado por parâmetro
+                    # retrieves the map image, passing the name sent as a parameter.
                     image_region = {
                         'image': self._screenshots[image_name]['image'],
                         'region': self._screenshots[image_name]['region']
                     }                
                 except KeyError as e:
-                    # Se modo manutenção igual True, cria imagem provisória e atualiza a imagem recem criada no mapa
-                    if self._modo_manutencao:
-                        # Cria um arquivo com image_name no diretório images se não existir
+                    # If maintenance mode equals True, creates a provisional image and updates the newly created image on the map.
+                    if self._maintenance_mode:
+                        # Create a file with image_name in the images directory if it does not exist.
                         im = pyautogui.screenshot(region=(1, 1, 300, 150))
-                        im.save(f'{path_dir_images}/{image_name}-(300, 50, 350, 200).png', 'PNG')
+                        im.save(f'{images_dir_path}/{image_name}-(300, 50, 350, 200).png', 'PNG')
                         time.sleep(1)
-                        # Atualiza o mapa com a imagem criada com o paramêtro image_name.
-                        self._screenshots = mapear_imagens()
-                        # recupera a imagem do mapa, passando o nome enviado por parâmetro
+                        # Updates the map with the image created with the image_name parameter.
+                        self._screenshots = map_images()
+                        # Retrieves the map image, passing the name sent as a parameter.
                         image_region = {
                             'image': self._screenshots[image_name]['image'],
                             'region': self._screenshots[image_name]['region']
                         }             
                     
                         atualizou = update_image(image_region.get('image'))
                         if atualizou:
-                            self._screenshots = mapear_imagens()
+                            self._screenshots = map_images()
                             image_region = {
                                 'image': self._screenshots[image_name]['image'],
                                 'region': self._screenshots[image_name]['region']
                             }
                     else:
                         raise KeyError(e)     
                 else:
-                    # Executa o bloco else se a imagem for encontrada no mapa
-                    coordenada = localizar_na_tela(**image_region)
-                    # Efetua um break para sair do loop quando as coordenas da imagem não forem mais encontradas
+                    # Execute the else block if the image is found on the map.
+                    coordenada = locate_on_screen(**image_region)
+                    # Performs a break to exit the loop when the image coordinates are no longer found.
                     if coordenada is None:
                         continue             
                 
                 if time.time() - start_time > max_wait_local:
-                    if self._modo_manutencao:
-                        # Abre a imagem a que não desapareceu no tempo de espera máxima
+                    if self._maintenance_mode:
+                        # Open the image that did not disappear within the maximum waiting time.
                         im = Image.open(image_region['image'])
                         im.show()
                         pyautogui.alert(title='RPAPY', text='A imagen {} não desapareceu em {:.0f} minutos! Feche-a para continuar a manutenção.'.format(image_region['image'], time.time() - start_time))
-                        # Fecha janela do visualizador de imagem após confirmacao de troca
-                        fechar_visualizador_fotos('fotos')
+                        # Closes image viewer window after switching confirmation.
+                        close_image_viewer('fotos')
                         start_time = time.time()
                     else:
                         raise ImageNotDisappearError("A imagem não desapareceu em {} seconds".format(time.time() - start_time))
 
-                # Efetua um intervalo parada entre os loop de tentativa de encontrar a imagem
+                # Performs a pause between loops trying to find the image
                 time.sleep(interval_local)
 
 
-def fechar_visualizador_fotos(title: str):
-    """Fecha a janela do visualizador de imagem do windows
+def close_image_viewer(title: str):
+    """Closes the Windows Image Viewer window
     
     Arguments:
-        title {str} -- Nome ou parte do nome do titulo da janela do visualizador de imagens
+        title {str} -- Name or part of the name of the title of the image viewer window.
     """
-    visualizadores_fotos = pyautogui.getWindowsWithTitle(title)
-    for v in visualizadores_fotos:
+    image_viewer = pyautogui.getWindowsWithTitle(title)
+    for v in image_viewer:
         v.close()
     
 
 def salvar_img_error(image_name:str, im:Image) ->None:
-    """Salva um print da tela no momento em que ocorreu o erro com informações 
-    de data e hora e nome da imagem em que foi lançado o erro.
+    """Saves a screenshot of the moment the error occurred with information
+    date and time and name of the image where the error was thrown.
     
     Arguments:
-        image_name {str} -- nome da imagem que não foi encotrado pelo metodo de busca
-        im {Image} -- imagem que capiturada no momento do erro.
+        image_name {str} -- name of the image that was not found by the search method.
+        im {Image} -- image that was captured at the time of the error.
     """    
     create_python_default_dirs()    
     nome_arquivo = datetime.datetime.now().strftime('%Y.%m.%d-%Hh%Mm%Ss')+'_'+image_name
-    im.save(f'{path_dir_error_images}/{nome_arquivo}.png', 'PNG')
-
-
-def mapear_imagens():
-    """Efetua o mapeamento das imagens capituradas pelo agente.py
-    e salvas no diretorio images. Utiliza o nome da imagem para 
-    recuperar a região onde a imagem deverá ser procurada.
-    
-    Returns:
-        [dict] -- [dicionário contendo os dados da imagem]
-    """
-    create_python_default_dirs()
-
-    # recupera o diretório onde estão as imagens    
-    try: 
-        path_dir_images.mkdir()
-    except FileExistsError:
-        pass
-
-    resultado: Dict[str, Dict[str, Tuple[int]]] = {}
-
-    # Recupera todos os arquivos de imagem no formato nome+região
-    images_path = path_dir_images.glob('*).png')
-
-    # Itera por todas as imagens encontradas no diretório
-    # recupera do nome e a tupla que indica a região da imagem
-    # adiciona os dados em um dict litera e adiona ao dict resultado pelo método default.
-    for p in images_path:
-        p: Path = p
-
-        anchor_coord = None
-        nome, *_ = p.name.split('-')
-        
-        if '#' in p.name:
-            restante, anchor_coord = p.name.removeprefix(nome+'-').split('#')
-            region_tuple = tuple(int(i) for i in restante[1:-1].split(','))
-            anchor_coord = tuple(int(i) for i in anchor_coord.split('.')[0][1:-1].split(','))
-
-        else:
-            restante = p.name.removeprefix(nome+'-')
-            region_tuple = tuple(int(i) for i in restante.removesuffix('.png')[1:-1].split(','))
-        
-        resultado.setdefault(nome, {
-            'image': p.as_posix(), 
-            'region': region_tuple, 
-            'anchor_coord': anchor_coord,
-        })
-    return resultado
+    im.save(f'{error_images_dir_path}/{nome_arquivo}.png', 'PNG')
 
 
 def max_wait_attr(desktop: Desktop, attr_name: str, max_wait: float=5.0) -> AttributeError:
     start_time = time.time()
     while True:
         if hasattr(desktop, attr_name):
             break
@@ -359,40 +314,39 @@
 
 def image_optmization(im: Image) -> Image:
     """Fonte: https://blog.codeexpertslearning.com.br/lendo-imagens-uma-abordagem-%C3%A0-ocr-com-google-tesseract-e-python-ee8e8009f2ab
     Pesquisado em: 02/01/2020
     """
     from PIL import Image
 
-    # tipando a leitura para os canais de ordem RGB
+    # Typing the reading for RGB order channels.
     imagem = im.convert('RGB')
 
-    # convertendo em um array editável de numpy[x, y, CANALS]
+    # Converting to an editable array of numpy[x, y, CANALS]
     npimagem = np.asarray(imagem).astype(np.uint8)  
 
-    # diminuição dos ruidos antes da binarização
-    npimagem[:, :, 0] = 0 # zerando o canal R (RED)
-    npimagem[:, :, 2] = 0 # zerando o canal B (BLUE)
+    # Noise reduction before binarization.
+    npimagem[:, :, 0] = 0       # canal R (RED).
+    npimagem[:, :, 2] = 0       # canal B (BLUE).
 
-    # atribuição em escala de cinza
+    # Grayscale Attribution
     im = cv2.cvtColor(npimagem, cv2.COLOR_RGB2GRAY) 
 
-    # aplicação da truncagem binária para a intensidade
-    # pixels de intensidade de cor abaixo de 127 serão convertidos para 0 (PRETO)
-    # pixels de intensidade de cor acima de 127 serão convertidos para 255 (BRANCO)
-    # A atrubição do THRESH_OTSU incrementa uma análise inteligente dos nivels 
-    # de truncagem
+    # Application of binary truncation for intensity
+    # Color intensity pixels below 127 will be converted to 0 (BLACK).
+    # Color intensity pixels above 127 will be converted to 255 (WHITE).
+    # The THRESH_OTSU attribute increases intelligent level analysis truncation.
     ret, thresh = cv2.threshold(im, 127, 255, cv2.THRESH_BINARY | cv2.THRESH_OTSU) 
 
-    # reconvertendo o retorno do threshold em um objeto do tipo PIL.Image
+    # Reconverting the threshold return into an object of type PIL.Image
     binimagem = Image.fromarray(thresh) 
 
-    # # chamada ao tesseract OCR por meio de seu wrapper
+    # Call to tesseract OCR through its wrapper
     # phrase = ocr.image_to_string(binimagem, lang='por')
 
-    # # impressão do resultado
+    # printout of result
     # print(phrase)
 
     return binimagem
 
 if '__main__' == __name__:
-    mapear_imagens()
+    map_images()
```

### Comparing `rpapy-1.1.0/rpapy/core/prepare_text.py` & `rpapy-1.1.1/rpapy/core/prepare_text.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """Normaliza o texto para execucao de teclas especiais no pyautogui no mesmo padrão do pywinauto
 """
 
-def prepare_text_to_pyautogui(text):
+def prepare_text_for_pyautogui(text):
     result = []
     keys_press = ''
     flag_key = False
     for l in text:
 
         if l in '{[':
             flag_key = True
@@ -30,8 +30,8 @@
         if flag_key is False:
             result.append(l)
     
     return result
 
 
 if __name__ == "__main__":
-    print(prepare_text_to_pyautogui(r'{ESC 5}ocorrência{TAB 3}trabalhador{ENTER 2}'))
+    print(prepare_text_for_pyautogui(r'{ESC 5}ocorrência{TAB 3}trabalhador{ENTER 2}'))
```

### Comparing `rpapy-1.1.0/rpapy/core/snipps/__init__.py` & `rpapy-1.1.1/rpapy/core/snipps/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,31 +1,30 @@
 import time
 from pathlib import Path
 from typing import Optional
 
 from PIL import Image
+
 from rpapy.core.config import Config
-from rpapy.core.loads import create_python_default_dirs
 from rpapy.core.snipps.codesnippets import add_new_activity
-from rpapy.core.snipps.snippingtools import (ImageNotFoundError,
-                                             close_window_with_title,
+from rpapy.core.snipps.loads import create_python_default_dirs
+from rpapy.core.snipps.snippingtools import (close_window_with_title,
                                              record_image, record_region,
                                              remove_duplicate_images,
                                              show_image_crop)
 from rpapy.core.utils.messages import confirm_ok_cancel
 
 
 def capture_image_crop(file_name:str=None)-> Optional[bool]:    
     
     if file_name is not None and ('.py' not in file_name.lower() and '.robot' not in file_name.lower()):
         raise Exception('O nome do arquivo deve ter a extensão .py ou .robot')
 
     create_python_default_dirs()
-    resources_path = Path(Config.BASE_DIR, Config.RESOURCES_DIR_NAME)
-    images_dir_path = resources_path / Config.IMAGES_DIR_NAME
+    images_dir_path = Config.IMAGES_DIR_PATH
     
     msg = 'Clique em IMG, IMG_ANCHOR, IMG_OCR e selecione o retângulo do elemento de interface na tela ou OCR.'
     snippet_type = None
     im_crop, anchor_coord = record_image(msg)      # Funcao para capiturar o recorte da imagem no screenshot da tela principar
     if im_crop == 'CANCEL':
         return    
         
@@ -65,16 +64,16 @@
         ImageNotFoundError: [Exception lançada quando a troca da img for cancelada]
     
     Returns:
         [bool] -- [retorna True se a imagem foi trocada, senão False]
     """
     
     create_python_default_dirs()
-    resources_path = Path(Config.BASE_DIR, Config.RESOURCES_DIR_NAME)
-    images_dir_path = resources_path / Config.IMAGES_DIR_NAME
+    
+    images_dir_path = Config.IMAGES_DIR_PATH
 
     # Recupera apenas o nome da imagem sem dados da região para utilizar na capitura da nova imagem
     image_name = image_name_path.split('/')[-1].split('-')[0]
 
     # Abre a imagem a ser trocada para ser exibida pelo visualizador de imagens
     im_crop = Image.open(image_name_path)
     cv2 = show_image_crop(im_crop)
```

### Comparing `rpapy-1.1.0/rpapy/core/snipps/codesnippets.py` & `rpapy-1.1.1/rpapy/core/snipps/codesnippets.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 import contextlib
 from pathlib import Path
 from typing import Dict, List
 
 import pyautogui
 import pyperclip
+
 from rpapy.core.config import Config
+from rpapy.core.snipps import templates
+from rpapy.core.snipps.loads import (create_default_script_file,
+                                     create_robot_default_dirs)
 from rpapy.core.snipps.snippingtools import record_region
-from rpapy.core.loads import create_default_script_file, create_robot_default_dirs
-from rpapy.core.utils import templates
 
 
 class ParamNotFoundError(Exception):
     pass
 
 
 _templates = {
@@ -123,16 +125,16 @@
     code = complete_robot_syntax(code)
     code = complete_python_syntax(code)
     pyperclip.copy(code)
 
     create_default_script_file(file_name=nome_arquivo)
         
     # Decide qual arquivo será aberto para escrita do snippet de código
-    if Config.ARQUIVO_TEMPORARIO_ATIVO:
-        path_file = Path(Config.BASE_DIR, Config.NOME_ARQUIVO_TEMPORARIO)
+    if Config.ACTIVE_TEMPORARY_ARCHIVE:
+        path_file = Path(Config.BASE_DIR, Config.TEMPORALY_FILE_NAME)
         if not path_file.exists():
             path_file.touch()
     elif extensao == 'robot':
         create_robot_default_dirs()
         path_dir_task = Path(Config.BASE_DIR, Config.TASKS_DIR_NAME)        
         path_file = path_dir_task / nome_arquivo
     else:
```

### Comparing `rpapy-1.1.0/rpapy/core/snipps/snippingtools.py` & `rpapy-1.1.1/rpapy/core/snipps/snippingtools.py`

 * *Files identical despite different names*

### Comparing `rpapy-1.1.0/rpapy/core/utils/example/paint_robot.py` & `rpapy-1.1.1/rpapy/core/utils/example/paint_robot.py`

 * *Files identical despite different names*

### Comparing `rpapy-1.1.0/rpapy/core/utils/imagens/IMAGEM_NAO_ENCONTRADA.png` & `rpapy-1.1.1/rpapy/core/utils/imagens/IMAGEM_NAO_ENCONTRADA.png`

 * *Files identical despite different names*

### Comparing `rpapy-1.1.0/rpapy/core/utils/imagens/template_win11_screen_1920x1080.svg` & `rpapy-1.1.1/rpapy/core/utils/imagens/template_win11_screen_1920x1080.svg`

 * *Files identical despite different names*

### Comparing `rpapy-1.1.0/rpapy/core/utils/templates.py` & `rpapy-1.1.1/rpapy/core/snipps/templates.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,46 +5,40 @@
 VARIAVEIS_AMBIENTE = """###VARIAVEIS DE AMBIENTE PYTHON-DOTENV
 
 #RESOURCES_DIR_NAME=resources
 #RESOURCES_KEYWORDS_FILE_NAME=keywords.robot
 #IMAGES_DIR_NAME=images
 #IMAGES_ERROR_DIR_NAME=images_error
 #TASKS_DIR_NAME=tasks
-#MAX_WAIT_MANUTENCAO=3
-#VERIFICAR_MODO=True
+#MAX_WAIT_MAINTENANCE=3
+#CHECK_MODE=True
 #FAILSAFE_OFF=True
-#ARQUIVO_TEMPORARIO_ATIVO=se
-#NOME_ARQUIVO_TEMPORARIO=temp.Faltxt
+#ACTIVE_TEMPORARY_ARCHIVE=se
+#TEMPORALY_FILE_NAME=temp.Faltxt
 #ONLY_IMAGE_PATH=False
 
 """
 
 ##########################################################################################
 MODULES_IMPORT_PY = '''"""[summary]
 """
 
 import time
 from pathlib import Path
 
 import pyautogui
 import pytesseract as ocr
 from pywinauto import Desktop
-from rpapy.activities import (click_coord, click_vision, contextlib, double_click_coord, 
-                              double_click_vision, drag_to_vision, drag_vision, get_element_coord, 
-                              get_element_vision, get_path_by_image_name, get_text_ocr_region, 
-                              get_text_ocr_vision, get_windows_title, max_wait_attr, open_executable, 
-                              prepare_text_to_pyautogui, registrar_credencial, toast_process_start_notifier, 
-                              triple_click_coord, triple_click_vision, wait_element_vision, write_text_coord, 
-                              write_text_vision)
-from rpapy.core.localizador import (ImageNotFoundError, LocalizadorImagem,
+from rpapy.activities import *
+from rpapy.core.localizador import (ImageNotFoundError, LocatorImage,
                                     image_optmization, max_wait_attr)
 
 #######################DEFINE#######################
 toast_process_start_notifier()
-get_coordenadas = LocalizadorImagem()
+get_coordenadas = LocatorImage()
 #######################DEFINE#######################
 
 
 '''
 ##########################################################################################
 
 MODULES_IMPORT_ROBOT = '''*** Settings ***
```

### Comparing `rpapy-1.1.0/PKG-INFO` & `rpapy-1.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 Metadata-Version: 2.1
 Name: rpapy
-Version: 1.1.0
+Version: 1.1.1
 Summary: RPAPY is a open source easy tool for automating boring stuffs on any screen with robotframework, pyautogui, pywinauto and others.
 Home-page: https://github.com/codigo100cera/rpapy
 License: MIT
 Keywords: rpa,robotframework,automations,tools
 Author: Codigo Sem Cera
 Author-email: codigo100cera@gmail.com
 Requires-Python: >=3.10,<3.13
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
+Requires-Dist: keyring (>=25.1.0,<26.0.0)
 Requires-Dist: mouse (>=0.7.1,<0.8.0)
 Requires-Dist: numpy (>=1.26.4,<2.0.0)
 Requires-Dist: opencv-python (>=4.9.0.80,<5.0.0.0)
 Requires-Dist: pyautogui (>=0.9.54,<0.10.0)
 Requires-Dist: pynput (>=1.7.6,<2.0.0)
 Requires-Dist: pyperclip (>=1.8.2,<2.0.0)
 Requires-Dist: pyside6 (>=6.6.2,<7.0.0)
@@ -43,28 +44,28 @@
 
 ## Get started
 
 ### Windows
 
 The easiest way to install RPAPY is by using __pip install__
 
-- Download and install [Python 3.7](https://www.python.org)
+- Download and install [Python >=3.10, <3.13 ](https://www.python.org)
 
 - Install the latest version RPAPY on your machine:
 ```
 pip install rpapy
 ```
 
 However, it is advisable to use a virtual environment for an isolated installation of all requirements, this avoids conflicts with the python interpreter installed on the host machine:
 ```
 pip install virtualenv
 mkdir <your-project-name>
 cd <your-project-name>
-virtualenv create rpapy-env
-activate rpapy-ev
+virtualenv create rpapy-venv
+activate rpapy-venv
 pip install rpapy
 ```
 
 The construction of the project structure is accomplished by executing the following command in the terminal:
 ```
 rpapy
 ```
```

