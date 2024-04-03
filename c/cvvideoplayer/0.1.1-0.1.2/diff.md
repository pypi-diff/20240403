# Comparing `tmp/cvvideoplayer-0.1.1.tar.gz` & `tmp/cvvideoplayer-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cvvideoplayer-0.1.1.tar", last modified: Tue Apr  2 10:33:38 2024, max compression
+gzip compressed data, was "cvvideoplayer-0.1.2.tar", last modified: Wed Apr  3 19:16:34 2024, max compression
```

## Comparing `cvvideoplayer-0.1.1.tar` & `cvvideoplayer-0.1.2.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxrwxrwx   0        0        0        0 2024-04-02 10:33:38.531571 cvvideoplayer-0.1.1/
--rw-rw-rw-   0        0        0     1067 2024-03-17 19:44:52.000000 cvvideoplayer-0.1.1/License.txt
--rw-rw-rw-   0        0        0      727 2024-04-02 10:33:38.530540 cvvideoplayer-0.1.1/PKG-INFO
--rw-rw-rw-   0        0        0     4313 2024-04-02 09:31:58.000000 cvvideoplayer-0.1.1/README.md
-drwxrwxrwx   0        0        0        0 2024-04-02 10:33:38.498985 cvvideoplayer-0.1.1/cvvideoplayer/
--rw-rw-rw-   0        0        0      136 2024-03-30 19:30:46.000000 cvvideoplayer-0.1.1/cvvideoplayer/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-02 10:33:38.515184 cvvideoplayer-0.1.1/cvvideoplayer/frame_editors/
--rw-rw-rw-   0        0        0      303 2024-04-02 06:16:09.000000 cvvideoplayer-0.1.1/cvvideoplayer/frame_editors/__init__.py
--rw-rw-rw-   0        0        0     4125 2024-04-02 09:54:25.000000 cvvideoplayer-0.1.1/cvvideoplayer/frame_editors/base_bbox_plotter.py
--rw-rw-rw-   0        0        0     2606 2024-04-02 09:54:25.000000 cvvideoplayer-0.1.1/cvvideoplayer/frame_editors/base_frame_editor.py
-drwxrwxrwx   0        0        0        0 2024-04-02 10:33:38.520528 cvvideoplayer-0.1.1/cvvideoplayer/frame_editors/basic_frame_editors/
--rw-rw-rw-   0        0        0        0 2024-03-22 18:47:56.000000 cvvideoplayer-0.1.1/cvvideoplayer/frame_editors/basic_frame_editors/__init__.py
--rw-rw-rw-   0        0        0     2373 2024-04-02 06:51:34.000000 cvvideoplayer-0.1.1/cvvideoplayer/frame_editors/basic_frame_editors/frame_normlizer.py
--rw-rw-rw-   0        0        0     1868 2024-04-02 06:51:34.000000 cvvideoplayer-0.1.1/cvvideoplayer/frame_editors/basic_frame_editors/frame_num_printer.py
--rw-rw-rw-   0        0        0     1108 2024-04-02 06:51:34.000000 cvvideoplayer-0.1.1/cvvideoplayer/frame_editors/basic_frame_editors/histogram_equalizer.py
--rw-rw-rw-   0        0        0     1387 2024-04-02 06:16:09.000000 cvvideoplayer-0.1.1/cvvideoplayer/frame_editors/detections_csv_plotter.py
--rw-rw-rw-   0        0        0     3359 2024-04-02 09:55:33.000000 cvvideoplayer-0.1.1/cvvideoplayer/frame_reader.py
--rw-rw-rw-   0        0        0     1402 2024-04-02 09:54:25.000000 cvvideoplayer-0.1.1/cvvideoplayer/recorder.py
-drwxrwxrwx   0        0        0        0 2024-04-02 10:33:38.527380 cvvideoplayer-0.1.1/cvvideoplayer/utils/
--rw-rw-rw-   0        0        0        0 2024-03-22 18:47:56.000000 cvvideoplayer-0.1.1/cvvideoplayer/utils/__init__.py
--rw-rw-rw-   0        0        0      863 2024-03-30 19:30:46.000000 cvvideoplayer-0.1.1/cvvideoplayer/utils/bbox_utils.py
--rw-rw-rw-   0        0        0     2233 2024-04-02 06:16:09.000000 cvvideoplayer-0.1.1/cvvideoplayer/utils/drawing_utils.py
--rw-rw-rw-   0        0        0     4350 2024-04-02 06:51:34.000000 cvvideoplayer-0.1.1/cvvideoplayer/utils/video_player_utils.py
--rw-rw-rw-   0        0        0     3012 2024-03-30 19:30:46.000000 cvvideoplayer-0.1.1/cvvideoplayer/utils/windows_vk_dict.py
--rw-rw-rw-   0        0        0    11899 2024-04-02 08:26:41.000000 cvvideoplayer-0.1.1/cvvideoplayer/video_player.py
-drwxrwxrwx   0        0        0        0 2024-04-02 10:33:38.508588 cvvideoplayer-0.1.1/cvvideoplayer.egg-info/
--rw-rw-rw-   0        0        0      727 2024-04-02 10:33:38.000000 cvvideoplayer-0.1.1/cvvideoplayer.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1016 2024-04-02 10:33:38.000000 cvvideoplayer-0.1.1/cvvideoplayer.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-02 10:33:38.000000 cvvideoplayer-0.1.1/cvvideoplayer.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       57 2024-04-02 10:33:38.000000 cvvideoplayer-0.1.1/cvvideoplayer.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2024-04-02 10:33:38.000000 cvvideoplayer-0.1.1/cvvideoplayer.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-02 10:33:38.531571 cvvideoplayer-0.1.1/setup.cfg
--rw-rw-rw-   0        0        0      940 2024-04-02 10:33:27.000000 cvvideoplayer-0.1.1/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-02 10:33:38.529520 cvvideoplayer-0.1.1/tests/
--rw-rw-rw-   0        0        0        0 2024-03-18 19:35:21.000000 cvvideoplayer-0.1.1/tests/test_video_player_basic_functionality.py
+drwxrwxrwx   0        0        0        0 2024-04-03 19:16:34.563959 cvvideoplayer-0.1.2/
+-rw-rw-rw-   0        0        0     1067 2024-03-17 19:44:52.000000 cvvideoplayer-0.1.2/License.txt
+-rw-rw-rw-   0        0        0      727 2024-04-03 19:16:34.562738 cvvideoplayer-0.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0     4900 2024-04-03 18:20:34.000000 cvvideoplayer-0.1.2/README.md
+drwxrwxrwx   0        0        0        0 2024-04-03 19:16:34.529934 cvvideoplayer-0.1.2/cvvideoplayer/
+-rw-rw-rw-   0        0        0      187 2024-04-02 17:56:54.000000 cvvideoplayer-0.1.2/cvvideoplayer/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-03 19:16:34.545668 cvvideoplayer-0.1.2/cvvideoplayer/frame_editors/
+-rw-rw-rw-   0        0        0      303 2024-04-02 06:16:09.000000 cvvideoplayer-0.1.2/cvvideoplayer/frame_editors/__init__.py
+-rw-rw-rw-   0        0        0     4127 2024-04-02 17:56:54.000000 cvvideoplayer-0.1.2/cvvideoplayer/frame_editors/base_bbox_plotter.py
+-rw-rw-rw-   0        0        0     2606 2024-04-02 09:54:25.000000 cvvideoplayer-0.1.2/cvvideoplayer/frame_editors/base_frame_editor.py
+drwxrwxrwx   0        0        0        0 2024-04-03 19:16:34.552248 cvvideoplayer-0.1.2/cvvideoplayer/frame_editors/basic_frame_editors/
+-rw-rw-rw-   0        0        0        0 2024-03-22 18:47:56.000000 cvvideoplayer-0.1.2/cvvideoplayer/frame_editors/basic_frame_editors/__init__.py
+-rw-rw-rw-   0        0        0     2373 2024-04-02 06:51:34.000000 cvvideoplayer-0.1.2/cvvideoplayer/frame_editors/basic_frame_editors/frame_normlizer.py
+-rw-rw-rw-   0        0        0     1868 2024-04-02 06:51:34.000000 cvvideoplayer-0.1.2/cvvideoplayer/frame_editors/basic_frame_editors/frame_num_printer.py
+-rw-rw-rw-   0        0        0     1108 2024-04-02 06:51:34.000000 cvvideoplayer-0.1.2/cvvideoplayer/frame_editors/basic_frame_editors/histogram_equalizer.py
+-rw-rw-rw-   0        0        0     1387 2024-04-02 06:16:09.000000 cvvideoplayer-0.1.2/cvvideoplayer/frame_editors/detections_csv_plotter.py
+-rw-rw-rw-   0        0        0     3363 2024-04-02 17:56:54.000000 cvvideoplayer-0.1.2/cvvideoplayer/frame_reader.py
+-rw-rw-rw-   0        0        0     1404 2024-04-02 17:56:54.000000 cvvideoplayer-0.1.2/cvvideoplayer/recorder.py
+drwxrwxrwx   0        0        0        0 2024-04-03 19:16:34.559695 cvvideoplayer-0.1.2/cvvideoplayer/utils/
+-rw-rw-rw-   0        0        0        0 2024-03-22 18:47:56.000000 cvvideoplayer-0.1.2/cvvideoplayer/utils/__init__.py
+-rw-rw-rw-   0        0        0      863 2024-03-30 19:30:46.000000 cvvideoplayer-0.1.2/cvvideoplayer/utils/bbox_utils.py
+-rw-rw-rw-   0        0        0     2233 2024-04-02 06:16:09.000000 cvvideoplayer-0.1.2/cvvideoplayer/utils/drawing_utils.py
+-rw-rw-rw-   0        0        0     3277 2024-04-02 17:56:54.000000 cvvideoplayer-0.1.2/cvvideoplayer/utils/video_player_utils.py
+-rw-rw-rw-   0        0        0     3012 2024-03-30 19:30:46.000000 cvvideoplayer-0.1.2/cvvideoplayer/utils/windows_vk_dict.py
+-rw-rw-rw-   0        0        0    12573 2024-04-03 19:08:49.000000 cvvideoplayer-0.1.2/cvvideoplayer/video_player.py
+drwxrwxrwx   0        0        0        0 2024-04-03 19:16:34.538570 cvvideoplayer-0.1.2/cvvideoplayer.egg-info/
+-rw-rw-rw-   0        0        0      727 2024-04-03 19:16:34.000000 cvvideoplayer-0.1.2/cvvideoplayer.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1016 2024-04-03 19:16:34.000000 cvvideoplayer-0.1.2/cvvideoplayer.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-03 19:16:34.000000 cvvideoplayer-0.1.2/cvvideoplayer.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       57 2024-04-03 19:16:34.000000 cvvideoplayer-0.1.2/cvvideoplayer.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2024-04-03 19:16:34.000000 cvvideoplayer-0.1.2/cvvideoplayer.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-03 19:16:34.563959 cvvideoplayer-0.1.2/setup.cfg
+-rw-rw-rw-   0        0        0      931 2024-04-03 19:16:26.000000 cvvideoplayer-0.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-03 19:16:34.561692 cvvideoplayer-0.1.2/tests/
+-rw-rw-rw-   0        0        0        0 2024-03-18 19:35:21.000000 cvvideoplayer-0.1.2/tests/test_video_player_basic_functionality.py
```

### Comparing `cvvideoplayer-0.1.1/License.txt` & `cvvideoplayer-0.1.2/License.txt`

 * *Files identical despite different names*

### Comparing `cvvideoplayer-0.1.1/PKG-INFO` & `cvvideoplayer-0.1.2/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cvvideoplayer
-Version: 0.1.1
+Version: 0.1.2
 Summary: moduler multi purpose video player for python
 Author: Daniel Tomer
 Author-email: danieltomer1@gmail.com
 Project-URL: Homepage, https://github.com/danieltomer1/CVVideoPlayer
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.8
```

### Comparing `cvvideoplayer-0.1.1/README.md` & `cvvideoplayer-0.1.2/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,51 +1,56 @@
 <div align="center"><img src="assets/logo.png" width="150"></div>
 
 ## Introduction
 CV video player is a Python-based customizable video player that helps computer vision practitioners
-to develop, analyze and debug their video related algorithms and model.
+to develop, analyze, and debug their video-related algorithms and models.
 
 
 ## Installation
 `pip install cvvideoplayer`
 
 ## Usage
-The player is interactive and operates only with keyboard presses (no buttons). The user can register new 
+The player is interactive and operates only with keyboard presses (no buttons). The user can register 
 shortcuts using the VideoPlayer class's API.
 
-### Design overview
-
+**Design overview**
 <div align="center"><img src="assets/video_player_design_chart.png" width="500"></div>
 
 The player receives an image from the FrameReader, the frame is then passed to a list of frame editors
-which alter it in any way desirable and return the frame. The frame editors also specify weather or not 
-to preform the edit after the frame has been resized to fit the screen.
+which alter it in any way desirable and return the frame. The frame editors also specify whether 
+to perform the edit after the frame has been resized to fit the screen or before.
+
+<details>
+<summary>FrameReader class</summary>
 
-### FrameReader class
 Implements the following protocol:
 ```python
 class FrameReader(abc.ABC):
     @abc.abstractmethod
     def get_frame(self, frame_num: int) -> Optional[np.ndarray]:
         pass
 
     @abc.abstractmethod
     def __len__(self) -> int:
         pass
 ```
 
-A ready to use LocalFrameReader is already implemented and can be used to read 
+A ready-to-use LocalFrameReader is already implemented and can be used to read 
 any local video file or folder containing the frames as images 
 (as long as there is a number in the name of the image files indicating their order).
 
-### FrameEditor class
+</details>
+
+
+<details>
+<summary>FrameEditor class</summary>
 
 You can add any number of FrameEditors for the player to apply using
 the VideoPlayer method "add_frame_editor". A FrameEditor is a class
-that needs to  inherit BaseFrameEditor and to implement 
+that needs to inherit BaseFrameEditor and implement 
 the following abstract methods:
 
 ```python
 class BaseFrameEditor(ABC):
     @property
     @abstractmethod
     def edit_after_resize(self) -> bool:
@@ -65,17 +70,23 @@
             frame (): the input frame
             frame_num ():
 
         Returns: the edited frame
         """
         pass
 ```
-### KeyFunction dataclass
-A KeyFunction defines a keypress:function mapping with an added description of the
-function's purpose. You can add a new KeyFunction in to ways:
+
+</details>
+
+
+<details>
+<summary>KeyFunction dataclass</summary>
+
+A KeyFunction defines a mapping between a key and a function with an added description of the
+function's purpose. You can add a new KeyFunction in two ways:
 - Using the video player's method "register_key_function"
 - Using a FrameEditors property "key_functions_to_register" which returns 
 a list of KeyFunctions that will be registered once the FrameEditor is added 
 to the player
 
 ### default key functions:
 These are used by the player and cannot be overwritten:
@@ -84,14 +95,35 @@
 - "left": Previous frame
 - "ctrl+right": 10 frames forward
 - "ctrl+left": 10 frames back
 - "ctrl+shift+right": 50 frames forward
 - "ctrl+shift+left": 50 frames back
 - "+": Increase frame size
 - "-": Decrease frame size
+
+</details>
+
+<details>
+<summary>Recorder class</summary>
+
+The recorder class is an object that can be used to record whatever is being
+played in the video player. By default, the video will be saved in an "outputs" folder
+which will be created in the CWD.
+
+To use the recorder:
+```python
+from cvvideoplayer import VideoPlayer, Recorder
+video_player = VideoPlayer(
+    recorder=Recorder(),
+    **other_video_player_kwargs
+)
+```
+
+</details>
+
 ## Quick Start
 ```python
 from cvvideoplayer import LocalFrameReader, Recorder, VideoPlayer
 
 
 def run_player():
     video_player = VideoPlayer(
@@ -105,15 +137,15 @@
         video_player.run()
 
 
 if __name__ == "__main__":
     run_player()
 ``` 
 
-In this example we initiate a very basic video player that will play "example_video.mp4" with added basic
+In this example, we initiate a very basic video player that will play "example_video.mp4" with added basic
 frame editors:
 - Frame number printer (disable/enable with **ctrl+f**): Prints the current frame number and original frame resolution in the top left corner
 - Histogram Equalizer (disable/enable with **ctrl+h**): Preforms histogram equalization on the image
 - Frame Normalizer: Allows the user to print the current frame's intensities histogram and also
 set a dynamic range for the image (see printed keymap at runtime for the used keyboard shortcuts).
 
-Check out the run_video_player.py which also uses the DetectionsCsvPlotter to plot precalculated detection
+Check out the run_video_player.py which also uses the DetectionsCsvPlotter to plot precalculated detection
```

### Comparing `cvvideoplayer-0.1.1/cvvideoplayer/frame_editors/base_bbox_plotter.py` & `cvvideoplayer-0.1.2/cvvideoplayer/frame_editors/base_bbox_plotter.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 
 
 class BaseBboxPlotter(BaseFrameEditor, ABC):
     """
     An abstract class that can be used a parent to any FrameEditor that needs to print bounding boxes on the frame.
     The self._edit_frame is already implemented and instead the derived class must implement the "get_bboxes" method.
     """
+
     def __init__(
         self,
         enable_by_default: bool = False,
         show_above_bbox_label: bool = True,
         show_below_bbox_label: bool = True,
         default_bbox_color: Tuple[int, int, int] = (255, 0, 0),
         text_color: Tuple[int, int, int] = (255, 255, 255),
```

### Comparing `cvvideoplayer-0.1.1/cvvideoplayer/frame_editors/base_frame_editor.py` & `cvvideoplayer-0.1.2/cvvideoplayer/frame_editors/base_frame_editor.py`

 * *Files identical despite different names*

### Comparing `cvvideoplayer-0.1.1/cvvideoplayer/frame_editors/basic_frame_editors/frame_normlizer.py` & `cvvideoplayer-0.1.2/cvvideoplayer/frame_editors/basic_frame_editors/frame_normlizer.py`

 * *Files identical despite different names*

### Comparing `cvvideoplayer-0.1.1/cvvideoplayer/frame_editors/basic_frame_editors/frame_num_printer.py` & `cvvideoplayer-0.1.2/cvvideoplayer/frame_editors/basic_frame_editors/frame_num_printer.py`

 * *Files identical despite different names*

### Comparing `cvvideoplayer-0.1.1/cvvideoplayer/frame_editors/basic_frame_editors/histogram_equalizer.py` & `cvvideoplayer-0.1.2/cvvideoplayer/frame_editors/basic_frame_editors/histogram_equalizer.py`

 * *Files identical despite different names*

### Comparing `cvvideoplayer-0.1.1/cvvideoplayer/frame_editors/detections_csv_plotter.py` & `cvvideoplayer-0.1.2/cvvideoplayer/frame_editors/detections_csv_plotter.py`

 * *Files identical despite different names*

### Comparing `cvvideoplayer-0.1.1/cvvideoplayer/frame_reader.py` & `cvvideoplayer-0.1.2/cvvideoplayer/frame_reader.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,28 +11,30 @@
 RANDOM_STATE = random.Random(42)
 
 
 class FrameReader(abc.ABC):
     """
     The frame reader is used in the video player to fetch frames according to a frame number
     """
+
     @abc.abstractmethod
     def get_frame(self, frame_num: int) -> Optional[np.ndarray]:
         pass
 
     @abc.abstractmethod
     def __len__(self) -> int:
         pass
 
 
 class LocalFrameReader(FrameReader):
     """
     A frame reader used to read any local video file or folder containing the frames as images
     (as long as there is a number in the name of the image files indicating their order).
     """
+
     def __init__(self, source_path):
         """
         Args:
             source_path: can be either a local video file path or a path to a directory containing frames as single
             images. the images need to contain a integer in their name specifying the frame order.
         """
         if Path(source_path).is_dir():
```

### Comparing `cvvideoplayer-0.1.1/cvvideoplayer/recorder.py` & `cvvideoplayer-0.1.2/cvvideoplayer/recorder.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 
 
 class Recorder:
     """
     In charge of recording what ever the video player is playing. The output video will be saved in
     output_video_path
     """
+
     def __init__(
         self,
         output_video_path: Path = Path("./outputs/recorded_video.mp4"),
         recorded_video_fps: int = 30,
         output_video_shape: Tuple[int, int] = (640, 512),
     ):
```

### Comparing `cvvideoplayer-0.1.1/cvvideoplayer/utils/bbox_utils.py` & `cvvideoplayer-0.1.2/cvvideoplayer/utils/bbox_utils.py`

 * *Files identical despite different names*

### Comparing `cvvideoplayer-0.1.1/cvvideoplayer/utils/drawing_utils.py` & `cvvideoplayer-0.1.2/cvvideoplayer/utils/drawing_utils.py`

 * *Files identical despite different names*

### Comparing `cvvideoplayer-0.1.1/cvvideoplayer/utils/windows_vk_dict.py` & `cvvideoplayer-0.1.2/cvvideoplayer/utils/windows_vk_dict.py`

 * *Files identical despite different names*

### Comparing `cvvideoplayer-0.1.1/cvvideoplayer/video_player.py` & `cvvideoplayer-0.1.2/cvvideoplayer/video_player.py`

 * *Files 5% similar despite different names*

```diff
@@ -10,17 +10,19 @@
 
 from .frame_editors import FrameNumPrinter, FrameNormalizer, HistogramEqualizer, BaseFrameEditor
 from .frame_reader import FrameReader
 from .recorder import Recorder
 from .utils.video_player_utils import (
     get_keyboard_layout,
     get_screen_adjusted_frame_size,
-    get_screen_size,
-    get_forground_window_pid,
-    KeyFunction, MODIFIERS,
+    get_foreground_window_pid,
+    KeyFunction,
+    MODIFIERS,
+    get_screen_size_linux,
+    get_screen_size_windows,
 )
 from .utils.windows_vk_dict import VK_CODE_MAP
 
 
 class VideoPlayer:
     def __init__(
         self,
@@ -37,25 +39,24 @@
 
         self._show_sidebar = False
         self._start_from_frame = start_from_frame
         self._last_frame = len(frame_reader) - 1
         self._frame_num = start_from_frame - 1
         self._modifiers = set()
         self._current_frame = None
-        self._frame_editors: list[BaseFrameEditor] = []
+        self._frame_editors: List[BaseFrameEditor] = []
 
         self._ui_queue = Queue()
         self._keyboard_layout = get_keyboard_layout()
-        self._number_action_registered = False
         self._play = False
 
-        self._screen_size = get_screen_size()
         self._resize_factor = 1.0
+        self._play_speed = 1
 
-        self._keymap: Dict[str: KeyFunction] = {}
+        self._keymap: Dict[str:KeyFunction] = {}
         self._add_default_key_functions()
         if add_basic_frame_editors:
             self._add_basic_frame_editors()
 
     def __enter__(self):
         return self
 
@@ -75,16 +76,16 @@
                     f" (key = {key_function.key}) which is not an instance of KeymapAction"
                 )
                 self.register_key_function(key_function)
 
     def register_key_function(self, key_function: KeyFunction) -> None:
         key = key_function.key
         if "+" in key:
-            modifiers = sorted(key.split("+")[:-1])
-            key_without_modifiers = key.split("+")[-1]
+            modifiers = sorted([modifier for modifier in key.split("+")[:-1] if modifier])
+            key_without_modifiers = key.split("+")[-1] or "+"
             key = "+".join(modifiers + [key_without_modifiers])
         else:
             key_without_modifiers = key
             modifiers = []
 
         if key_without_modifiers.isnumeric():
             general_num_key = "+".join(modifiers + ["num"])
@@ -112,17 +113,14 @@
             key = self._ui_queue.get()
             if key == keyboard.Key.esc or cv2.getWindowProperty(self._video_name, cv2.WND_PROP_VISIBLE) < 1:
                 cv2.destroyAllWindows()
                 break
 
             if key == "mouse_click":
                 cv2.waitKey(30)
-            elif key == keyboard.Key.space:
-                self._play = bool(1 - self._play)
-                self._play_continuously()
             else:
                 self._handle_keyboard_press(key)
 
     def _setup(self) -> None:
         if platform.system() == "Linux":
             self._linux_setup()
         elif platform.system() == "Windows":
@@ -139,18 +137,20 @@
         cv2.waitKey(50)
         time.sleep(0.5)
         self._window_pid = self._get_in_focus_window_name()
         self._print_keymap()
 
     def _windows_setup(self) -> None:
         self._map_vk_code = lambda x: VK_CODE_MAP[x]
-        self._get_in_focus_window_name = get_forground_window_pid
+        self._get_in_focus_window_name = get_foreground_window_pid
+        self._screen_size = get_screen_size_windows()
 
     def _linux_setup(self) -> None:
         self._map_vk_code = lambda x: chr(x)
+        self._screen_size = get_screen_size_linux()
 
         def _get_in_focus_window_name():
             window = Xlib.display.Display().get_input_focus().focus
             if isinstance(window, int):
                 return ""
             return window.get_wm_name()
 
@@ -186,17 +186,17 @@
 
     def _show_current_frame(self) -> None:
         frame = self._current_frame.copy()
 
         for frame_editor in self._frame_editors:
             if not frame_editor.edit_after_resize:
                 frame = frame_editor.edit_frame(frame, self._frame_num)
-                assert frame.shape[:2] == self._original_frame_size, (
-                    "frame editors with edit_after_resize==False can not alter the frame's shape"
-                )
+                assert (
+                    frame.shape[:2] == self._original_frame_size
+                ), "frame editors with edit_after_resize==False can not alter the frame's shape"
 
         frame = self._resize_frame(frame)
 
         for frame_editor in self._frame_editors:
             if frame_editor.edit_after_resize:
                 frame = frame_editor.edit_frame(frame, self._frame_num)
 
@@ -211,84 +211,104 @@
 
     def _add_basic_frame_editors(self) -> None:
         self.add_frame_editor(FrameNumPrinter(video_total_frame_num=len(self._frame_reader)))
         self.add_frame_editor(FrameNormalizer())
         self.add_frame_editor(HistogramEqualizer())
 
     def _print_keymap(self) -> None:
-        print("space bar: Play/Pause video")
-        for key, action in self._keymap.items():
-            print(f"{key}: {action.description}")
+        for key, key_function in self._keymap.items():
+            if key_function.description:
+                print(f"{key}: {key_function.description}")
         print("***********************************")
 
     def _play_continuously(self) -> None:
         while self._ui_queue.empty() and self._play:
-            self._next_frame(1)
+            self._next_frame(self._play_speed)
             self._show_current_frame()
 
     def _resize_frame(self, frame) -> np.ndarray:
         width, height = get_screen_adjusted_frame_size(
             screen_size=self._screen_size,
             frame_width=frame.shape[1],
             frame_height=frame.shape[0],
         )
         frame_size = int(self._resize_factor * width), int(self._resize_factor * height)
         return cv2.resize(frame, frame_size)
 
     def _next_frame(self, num_frames_to_skip=1) -> None:
         if self._frame_num == self._last_frame:
+            self._play = False
             return
 
-        self._frame_num = min(self._frame_num + num_frames_to_skip, len(self._frame_reader) - 1)
+        self._frame_num = min(self._frame_num + num_frames_to_skip, self._last_frame)
         self._current_frame = self._frame_reader.get_frame(self._frame_num)
 
     def _prev_frame(self, num_frames_to_skip=1) -> None:
         if self._frame_num == 0:
             return
 
         self._frame_num = max(self._frame_num - num_frames_to_skip, 0)
         self._current_frame = self._frame_reader.get_frame(self._frame_num)
 
     def _change_frame_resize_factor(self, change_by: float) -> None:
         self._resize_factor = max(0.1, min(1.0, self._resize_factor + change_by))
 
+    def _play_pause(self):
+        self._play = not self._play
+        self._play_continuously()
+
+    def _double_play_speed(self) -> None:
+        self._play_speed = min(16, self._play_speed * 2)
+        self._play = True
+        self._play_continuously()
+
+    def _half_play_speed(self) -> None:
+        self._play_speed = max(1, self._play_speed // 2)
+        self._play = True
+        self._play_continuously()
+
     def _add_default_key_functions(self) -> None:
         default_key_functions = [
-            KeyFunction(key="right", func=lambda: self._next_frame(1), description="Go to next frame"),
-            KeyFunction(key="left", func=lambda: self._prev_frame(1), description="Go to previous frame"),
-            KeyFunction(key="ctrl+right", func=lambda: self._next_frame(10), description="Go 10 frames forward"),
-            KeyFunction(key="ctrl+left", func=lambda: self._prev_frame(10), description="Go 10 frames back"),
-            KeyFunction(key="ctrl+shift+right", func=lambda: self._next_frame(50), description="Go 50 frames forward"),
-            KeyFunction(key="ctrl+shift+left", func=lambda: self._prev_frame(50), description="Go 50 frames back"),
-            KeyFunction(key="+", func=lambda: self._change_frame_resize_factor(0.1), description="Increase frame size"),
-            KeyFunction(key="shift++", func=lambda: self._change_frame_resize_factor(0.1), description="Increase frame size"),
-            KeyFunction(key="-", func=lambda: self._change_frame_resize_factor(-0.1), description="Decrease frame size"),
+            KeyFunction("space", func=lambda: self._play_pause(), description="Play/Pause video"),
+            KeyFunction("right", func=lambda: self._next_frame(1), description="Next frame"),
+            KeyFunction("left", func=lambda: self._prev_frame(1), description="Previous frame"),
+            KeyFunction("ctrl+right", func=lambda: self._next_frame(10), description="10 frames forward"),
+            KeyFunction("ctrl+left", func=lambda: self._prev_frame(10), description="10 frames back"),
+            KeyFunction("ctrl+shift+right", func=lambda: self._next_frame(50), description="50 frames forward"),
+            KeyFunction("ctrl+shift+left", func=lambda: self._prev_frame(50), description="50 frames back"),
+            KeyFunction("ctrl++", func=lambda: self._change_frame_resize_factor(0.1), description="Increase frame size"),
+            KeyFunction("ctrl+-", lambda: self._change_frame_resize_factor(-0.1), description="Decrease frame size"),
+            KeyFunction("+", lambda: self._double_play_speed(), description="Double play speed"),
+            KeyFunction("shift++", lambda: self._double_play_speed(), description=""),
+            KeyFunction("-", lambda: self._half_play_speed(), description="Half play speed"),
         ]
 
         for key_function in default_key_functions:
             self.register_key_function(key_function)
 
     def _handle_keyboard_press(self, key_without_modifiers) -> None:
         if (
             str(key_without_modifiers) == "<65437>"
         ):  # work around for a bug in pynput model that does not convert 5 for some reason
             key_without_modifiers = "5"
 
         if hasattr(key_without_modifiers, "vk") and key_without_modifiers.vk is not None:
             key_without_modifiers = self._map_vk_code(key_without_modifiers.vk).lower()
-            key = "+".join(sorted(self._modifiers) + [key_without_modifiers])
         else:
             key_without_modifiers = str(key_without_modifiers).replace("'", "").replace("Key.", "")
-            key = "+".join(sorted(self._modifiers) + [key_without_modifiers])
+
+        if not key_without_modifiers == "space":
+            self._play = False
 
         if str(key_without_modifiers).isnumeric():
             general_num_key = "+".join(sorted(self._modifiers) + ["num"])
         else:
             general_num_key = None
 
+        key = "+".join(sorted(self._modifiers) + [key_without_modifiers])
         if general_num_key in self._keymap:
             self._keymap[general_num_key].func(key_without_modifiers)
         elif key in self._keymap:
             self._keymap[key].func()
         else:
             print(f"{key} deos nothing")
```

### Comparing `cvvideoplayer-0.1.1/cvvideoplayer.egg-info/PKG-INFO` & `cvvideoplayer-0.1.2/cvvideoplayer.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cvvideoplayer
-Version: 0.1.1
+Version: 0.1.2
 Summary: moduler multi purpose video player for python
 Author: Daniel Tomer
 Author-email: danieltomer1@gmail.com
 Project-URL: Homepage, https://github.com/danieltomer1/CVVideoPlayer
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.8
```

### Comparing `cvvideoplayer-0.1.1/cvvideoplayer.egg-info/SOURCES.txt` & `cvvideoplayer-0.1.2/cvvideoplayer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cvvideoplayer-0.1.1/setup.py` & `cvvideoplayer-0.1.2/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 from setuptools import setup, find_packages
 
 setup(
     name="cvvideoplayer",
-    version="0.1.1",
+    version="0.1.2",
     author="Daniel Tomer",
     author_email="danieltomer1@gmail.com",
     description="moduler multi purpose video player for python",
-    long_description=("CV video player is a Python-based customizable video player that helps"
-                      " computer vision practitioners to develop, analyze and debug their video"
-                      " related algorithms and model."),
+    long_description=(
+        "CV video player is a Python-based customizable video player that helps"
+        " computer vision practitioners to develop, analyze and debug their video"
+        " related algorithms and model."
+    ),
     packages=find_packages(),
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
     ],
     install_requires=[
         "numpy",
@@ -20,10 +22,10 @@
         "pynput",
         "decord",
         "python-xlib",
         "matplotlib",
     ],
     python_requires=">=3.8",
     project_urls={
-      "Homepage": "https://github.com/danieltomer1/CVVideoPlayer",
-    }
+        "Homepage": "https://github.com/danieltomer1/CVVideoPlayer",
+    },
 )
```

