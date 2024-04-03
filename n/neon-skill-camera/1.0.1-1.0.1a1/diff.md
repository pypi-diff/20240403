# Comparing `tmp/neon-skill-camera-1.0.1.tar.gz` & `tmp/neon-skill-camera-1.0.1a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neon-skill-camera-1.0.1.tar", last modified: Wed Apr  3 20:13:35 2024, max compression
+gzip compressed data, was "neon-skill-camera-1.0.1a1.tar", last modified: Tue Feb  6 01:09:33 2024, max compression
```

## Comparing `neon-skill-camera-1.0.1.tar` & `neon-skill-camera-1.0.1a1.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 20:13:35.573769 neon-skill-camera-1.0.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1635 2024-04-03 20:13:33.000000 neon-skill-camera-1.0.1/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)     1085 2024-04-03 20:13:35.573769 neon-skill-camera-1.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      829 2024-04-03 20:13:33.000000 neon-skill-camera-1.0.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)    17038 2024-04-03 20:13:33.000000 neon-skill-camera-1.0.1/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 20:13:35.565769 neon-skill-camera-1.0.1/dialog/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 20:13:35.569769 neon-skill-camera-1.0.1/dialog/en-us/
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-03 20:13:33.000000 neon-skill-camera-1.0.1/dialog/en-us/DefaultDuration.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-03 20:13:33.000000 neon-skill-camera-1.0.1/dialog/en-us/LaunchCamera.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-03 20:13:33.000000 neon-skill-camera-1.0.1/dialog/en-us/NoCamera.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-04-03 20:13:33.000000 neon-skill-camera-1.0.1/dialog/en-us/NothingToShow.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-03 20:13:33.000000 neon-skill-camera-1.0.1/dialog/en-us/PictureInsteadOfVideo.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-03 20:13:33.000000 neon-skill-camera-1.0.1/dialog/en-us/ServerNotSupported.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-03 20:13:33.000000 neon-skill-camera-1.0.1/dialog/en-us/ShowLatest.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-03 20:13:33.000000 neon-skill-camera-1.0.1/dialog/en-us/StartRecording.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-03 20:13:33.000000 neon-skill-camera-1.0.1/dialog/en-us/hour.list
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-03 20:13:33.000000 neon-skill-camera-1.0.1/dialog/en-us/minute.list
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-03 20:13:33.000000 neon-skill-camera-1.0.1/dialog/en-us/second.list
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 20:13:35.573769 neon-skill-camera-1.0.1/neon_skill_camera.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1085 2024-04-03 20:13:35.000000 neon-skill-camera-1.0.1/neon_skill_camera.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      917 2024-04-03 20:13:35.000000 neon-skill-camera-1.0.1/neon_skill_camera.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 20:13:35.000000 neon-skill-camera-1.0.1/neon_skill_camera.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       73 2024-04-03 20:13:35.000000 neon-skill-camera-1.0.1/neon_skill_camera.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-03 20:13:35.000000 neon-skill-camera-1.0.1/neon_skill_camera.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-03 20:13:35.000000 neon-skill-camera-1.0.1/neon_skill_camera.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-03 20:13:35.573769 neon-skill-camera-1.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     4434 2024-04-03 20:13:33.000000 neon-skill-camera-1.0.1/setup.py
--rw-r--r--   0 runner    (1001) docker     (127)     1302 2024-04-03 20:13:33.000000 neon-skill-camera-1.0.1/skill.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 20:13:35.573769 neon-skill-camera-1.0.1/ui/
--rw-r--r--   0 runner    (1001) docker     (127)     7174 2024-04-03 20:13:33.000000 neon-skill-camera-1.0.1/ui/Camera.qml
--rw-r--r--   0 runner    (1001) docker     (127)     3850 2024-04-03 20:13:33.000000 neon-skill-camera-1.0.1/ui/ControlBar.qml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 20:13:35.573769 neon-skill-camera-1.0.1/ui/images/
--rw-r--r--   0 runner    (1001) docker     (127)     3050 2024-04-03 20:13:33.000000 neon-skill-camera-1.0.1/ui/images/back.svg
--rw-r--r--   0 runner    (1001) docker     (127)     4479 2024-04-03 20:13:33.000000 neon-skill-camera-1.0.1/ui/images/capture.svg
--rw-r--r--   0 runner    (1001) docker     (127)     2748 2024-04-03 20:13:33.000000 neon-skill-camera-1.0.1/ui/images/close.svg
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-03 20:13:33.000000 neon-skill-camera-1.0.1/ui/qmldir
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 20:13:35.573769 neon-skill-camera-1.0.1/ui/sounds/
--rw-r--r--   0 runner    (1001) docker     (127)   341166 2024-04-03 20:13:33.000000 neon-skill-camera-1.0.1/ui/sounds/clicking.wav
--rw-r--r--   0 runner    (1001) docker     (127)     1854 2024-04-03 20:13:33.000000 neon-skill-camera-1.0.1/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 20:13:35.569769 neon-skill-camera-1.0.1/vocab/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 20:13:35.573769 neon-skill-camera-1.0.1/vocab/en-us/
--rw-r--r--   0 runner    (1001) docker     (127)      747 2024-04-03 20:13:33.000000 neon-skill-camera-1.0.1/vocab/en-us/ShowLastIntent.intent
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-04-03 20:13:33.000000 neon-skill-camera-1.0.1/vocab/en-us/TakePicIntent.intent
--rw-r--r--   0 runner    (1001) docker     (127)      253 2024-04-03 20:13:33.000000 neon-skill-camera-1.0.1/vocab/en-us/TakeVidIntent.intent
--rw-r--r--   0 runner    (1001) docker     (127)       80 2024-04-03 20:13:33.000000 neon-skill-camera-1.0.1/vocab/en-us/duration.entity
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 01:09:33.571944 neon-skill-camera-1.0.1a1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1635 2024-02-06 01:09:30.000000 neon-skill-camera-1.0.1a1/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1087 2024-02-06 01:09:33.571944 neon-skill-camera-1.0.1a1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      829 2024-02-06 01:09:30.000000 neon-skill-camera-1.0.1a1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)    17038 2024-02-06 01:09:30.000000 neon-skill-camera-1.0.1a1/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 01:09:33.563944 neon-skill-camera-1.0.1a1/dialog/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 01:09:33.567944 neon-skill-camera-1.0.1a1/dialog/en-us/
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-02-06 01:09:30.000000 neon-skill-camera-1.0.1a1/dialog/en-us/DefaultDuration.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-02-06 01:09:30.000000 neon-skill-camera-1.0.1a1/dialog/en-us/LaunchCamera.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-02-06 01:09:30.000000 neon-skill-camera-1.0.1a1/dialog/en-us/NoCamera.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-02-06 01:09:30.000000 neon-skill-camera-1.0.1a1/dialog/en-us/NothingToShow.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-02-06 01:09:30.000000 neon-skill-camera-1.0.1a1/dialog/en-us/PictureInsteadOfVideo.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-02-06 01:09:30.000000 neon-skill-camera-1.0.1a1/dialog/en-us/ServerNotSupported.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-02-06 01:09:30.000000 neon-skill-camera-1.0.1a1/dialog/en-us/ShowLatest.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-02-06 01:09:30.000000 neon-skill-camera-1.0.1a1/dialog/en-us/StartRecording.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-02-06 01:09:30.000000 neon-skill-camera-1.0.1a1/dialog/en-us/hour.list
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-02-06 01:09:30.000000 neon-skill-camera-1.0.1a1/dialog/en-us/minute.list
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-02-06 01:09:30.000000 neon-skill-camera-1.0.1a1/dialog/en-us/second.list
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 01:09:33.567944 neon-skill-camera-1.0.1a1/neon_skill_camera.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1087 2024-02-06 01:09:33.000000 neon-skill-camera-1.0.1a1/neon_skill_camera.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      917 2024-02-06 01:09:33.000000 neon-skill-camera-1.0.1a1/neon_skill_camera.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-06 01:09:33.000000 neon-skill-camera-1.0.1a1/neon_skill_camera.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-02-06 01:09:33.000000 neon-skill-camera-1.0.1a1/neon_skill_camera.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-02-06 01:09:33.000000 neon-skill-camera-1.0.1a1/neon_skill_camera.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-02-06 01:09:33.000000 neon-skill-camera-1.0.1a1/neon_skill_camera.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-06 01:09:33.571944 neon-skill-camera-1.0.1a1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     4434 2024-02-06 01:09:30.000000 neon-skill-camera-1.0.1a1/setup.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1302 2024-02-06 01:09:30.000000 neon-skill-camera-1.0.1a1/skill.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 01:09:33.567944 neon-skill-camera-1.0.1a1/ui/
+-rw-r--r--   0 runner    (1001) docker     (127)     7174 2024-02-06 01:09:30.000000 neon-skill-camera-1.0.1a1/ui/Camera.qml
+-rw-r--r--   0 runner    (1001) docker     (127)     3850 2024-02-06 01:09:30.000000 neon-skill-camera-1.0.1a1/ui/ControlBar.qml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 01:09:33.567944 neon-skill-camera-1.0.1a1/ui/images/
+-rw-r--r--   0 runner    (1001) docker     (127)     3050 2024-02-06 01:09:30.000000 neon-skill-camera-1.0.1a1/ui/images/back.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     4479 2024-02-06 01:09:30.000000 neon-skill-camera-1.0.1a1/ui/images/capture.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     2748 2024-02-06 01:09:30.000000 neon-skill-camera-1.0.1a1/ui/images/close.svg
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-02-06 01:09:30.000000 neon-skill-camera-1.0.1a1/ui/qmldir
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 01:09:33.567944 neon-skill-camera-1.0.1a1/ui/sounds/
+-rw-r--r--   0 runner    (1001) docker     (127)   341166 2024-02-06 01:09:30.000000 neon-skill-camera-1.0.1a1/ui/sounds/clicking.wav
+-rw-r--r--   0 runner    (1001) docker     (127)     1856 2024-02-06 01:09:30.000000 neon-skill-camera-1.0.1a1/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 01:09:33.563944 neon-skill-camera-1.0.1a1/vocab/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 01:09:33.571944 neon-skill-camera-1.0.1a1/vocab/en-us/
+-rw-r--r--   0 runner    (1001) docker     (127)      747 2024-02-06 01:09:30.000000 neon-skill-camera-1.0.1a1/vocab/en-us/ShowLastIntent.intent
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-02-06 01:09:30.000000 neon-skill-camera-1.0.1a1/vocab/en-us/TakePicIntent.intent
+-rw-r--r--   0 runner    (1001) docker     (127)      253 2024-02-06 01:09:30.000000 neon-skill-camera-1.0.1a1/vocab/en-us/TakeVidIntent.intent
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2024-02-06 01:09:30.000000 neon-skill-camera-1.0.1a1/vocab/en-us/duration.entity
```

### Comparing `neon-skill-camera-1.0.1/LICENSE.md` & `neon-skill-camera-1.0.1a1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `neon-skill-camera-1.0.1/PKG-INFO` & `neon-skill-camera-1.0.1a1/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neon-skill-camera
-Version: 1.0.1
+Version: 1.0.1a1
 Home-page: https://github.com/NeonGeckoCom/skill-camera
 Author: Neongecko
 Author-email: developers@neon.ai
 License: BSD-3-Clause
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
```

### Comparing `neon-skill-camera-1.0.1/README.md` & `neon-skill-camera-1.0.1a1/README.md`

 * *Files identical despite different names*

### Comparing `neon-skill-camera-1.0.1/__init__.py` & `neon-skill-camera-1.0.1a1/__init__.py`

 * *Files identical despite different names*

### Comparing `neon-skill-camera-1.0.1/neon_skill_camera.egg-info/PKG-INFO` & `neon-skill-camera-1.0.1a1/neon_skill_camera.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neon-skill-camera
-Version: 1.0.1
+Version: 1.0.1a1
 Home-page: https://github.com/NeonGeckoCom/skill-camera
 Author: Neongecko
 Author-email: developers@neon.ai
 License: BSD-3-Clause
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
```

### Comparing `neon-skill-camera-1.0.1/neon_skill_camera.egg-info/SOURCES.txt` & `neon-skill-camera-1.0.1a1/neon_skill_camera.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `neon-skill-camera-1.0.1/setup.py` & `neon-skill-camera-1.0.1a1/setup.py`

 * *Files identical despite different names*

### Comparing `neon-skill-camera-1.0.1/skill.json` & `neon-skill-camera-1.0.1a1/skill.json`

 * *Files identical despite different names*

### Comparing `neon-skill-camera-1.0.1/ui/Camera.qml` & `neon-skill-camera-1.0.1a1/ui/Camera.qml`

 * *Files identical despite different names*

### Comparing `neon-skill-camera-1.0.1/ui/ControlBar.qml` & `neon-skill-camera-1.0.1a1/ui/ControlBar.qml`

 * *Files identical despite different names*

### Comparing `neon-skill-camera-1.0.1/ui/images/back.svg` & `neon-skill-camera-1.0.1a1/ui/images/back.svg`

 * *Files identical despite different names*

### Comparing `neon-skill-camera-1.0.1/ui/images/capture.svg` & `neon-skill-camera-1.0.1a1/ui/images/capture.svg`

 * *Files identical despite different names*

### Comparing `neon-skill-camera-1.0.1/ui/images/close.svg` & `neon-skill-camera-1.0.1a1/ui/images/close.svg`

 * *Files identical despite different names*

### Comparing `neon-skill-camera-1.0.1/ui/sounds/clicking.wav` & `neon-skill-camera-1.0.1a1/ui/sounds/clicking.wav`

 * *Files identical despite different names*

### Comparing `neon-skill-camera-1.0.1/version.py` & `neon-skill-camera-1.0.1a1/version.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,8 +22,8 @@
 # EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO,
 # PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA,
 # OR PROFITS;  OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF
 # LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING
 # NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS
 # SOFTWARE,  EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
-__version__ = "1.0.1"
+__version__ = "1.0.1a1"
```

### Comparing `neon-skill-camera-1.0.1/vocab/en-us/ShowLastIntent.intent` & `neon-skill-camera-1.0.1a1/vocab/en-us/ShowLastIntent.intent`

 * *Files identical despite different names*

