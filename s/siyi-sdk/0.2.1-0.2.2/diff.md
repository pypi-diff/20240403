# Comparing `tmp/siyi_sdk-0.2.1.tar.gz` & `tmp/siyi_sdk-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "siyi_sdk-0.2.1.tar", max compression
+gzip compressed data, was "siyi_sdk-0.2.2.tar", max compression
```

## Comparing `siyi_sdk-0.2.1.tar` & `siyi_sdk-0.2.2.tar`

### file list

```diff
@@ -1,36 +1,36 @@
--rw-r--r--   0        0        0       51 2024-03-25 23:21:52.454164 siyi_sdk-0.2.1/README.md
--rw-r--r--   0        0        0      335 2024-03-28 23:40:28.395938 siyi_sdk-0.2.1/pyproject.toml
--rw-r--r--   0        0        0       33 2024-03-25 23:25:34.330901 siyi_sdk-0.2.1/siyi_sdk/.git
--rw-r--r--   0        0        0     3078 2024-03-25 23:25:34.334901 siyi_sdk-0.2.1/siyi_sdk/.gitignore
--rw-r--r--   0        0        0     1082 2024-03-25 23:25:34.334901 siyi_sdk-0.2.1/siyi_sdk/LICENSE
--rw-r--r--   0        0        0     4034 2024-03-25 23:25:44.550383 siyi_sdk-0.2.1/siyi_sdk/README.md
--rw-r--r--   0        0        0       58 2024-03-25 23:25:34.334901 siyi_sdk-0.2.1/siyi_sdk/__init__.py
--rw-r--r--   0        0        0     4353 2024-03-25 23:25:34.334901 siyi_sdk-0.2.1/siyi_sdk/crc16_python.py
--rw-r--r--   0        0        0  8385675 2024-03-25 23:25:44.562382 siyi_sdk-0.2.1/siyi_sdk/gui/demo.mp4
--rw-r--r--   0        0        0    16665 2024-03-25 23:25:44.562382 siyi_sdk-0.2.1/siyi_sdk/gui/gui_tkinter.png
--rw-r--r--   0        0        0     3994 2024-03-28 21:15:20.435565 siyi_sdk-0.2.1/siyi_sdk/gui/tkgui.py
--rw-r--r--   0        0        0    12921 2024-03-28 21:04:24.903711 siyi_sdk-0.2.1/siyi_sdk/siyi_message.py
--rw-r--r--   0        0        0    30315 2024-03-28 21:04:24.903711 siyi_sdk-0.2.1/siyi_sdk/siyi_sdk.py
--rw-r--r--   0        0        0     9360 2024-03-25 23:25:34.334901 siyi_sdk-0.2.1/siyi_sdk/stream.py
--rw-r--r--   0        0        0        0 2024-03-25 23:25:34.334901 siyi_sdk-0.2.1/siyi_sdk/tests/__init__.py
--rw-r--r--   0        0        0      878 2024-03-28 21:04:24.903711 siyi_sdk-0.2.1/siyi_sdk/tests/serial/test_center_gimbal.py
--rw-r--r--   0        0        0      787 2024-03-28 21:04:24.903711 siyi_sdk-0.2.1/siyi_sdk/tests/serial/test_get_fw_ver.py
--rw-r--r--   0        0        0      820 2024-03-28 21:04:24.903711 siyi_sdk-0.2.1/siyi_sdk/tests/serial/test_gimbal_position.py
--rw-r--r--   0        0        0      790 2024-03-28 21:04:24.903711 siyi_sdk-0.2.1/siyi_sdk/tests/serial/test_gimbal_rotation.py
--rw-r--r--   0        0        0      844 2024-03-25 23:25:34.334901 siyi_sdk-0.2.1/siyi_sdk/tests/test_center_gimbal.py
--rw-r--r--   0        0        0      746 2024-03-25 23:25:34.334901 siyi_sdk-0.2.1/siyi_sdk/tests/test_follow_mode.py
--rw-r--r--   0        0        0      737 2024-03-25 23:25:34.334901 siyi_sdk-0.2.1/siyi_sdk/tests/test_fpv_mode.py
--rw-r--r--   0        0        0      924 2024-03-25 23:25:34.334901 siyi_sdk-0.2.1/siyi_sdk/tests/test_from_rtsp_to_rtmp.py
--rw-r--r--   0        0        0      753 2024-03-25 23:25:34.334901 siyi_sdk-0.2.1/siyi_sdk/tests/test_get_fw_ver.py
--rw-r--r--   0        0        0      881 2024-03-25 23:25:34.334901 siyi_sdk-0.2.1/siyi_sdk/tests/test_get_gimbal_info.py
--rw-r--r--   0        0        0      734 2024-03-25 23:25:34.334901 siyi_sdk-0.2.1/siyi_sdk/tests/test_get_hw_id.py
--rw-r--r--   0        0        0      774 2024-03-28 21:14:01.390679 siyi_sdk-0.2.1/siyi_sdk/tests/test_gimbal_position.py
--rw-r--r--   0        0        0      756 2024-03-25 23:25:34.334901 siyi_sdk-0.2.1/siyi_sdk/tests/test_gimbal_rotation.py
--rw-r--r--   0        0        0      740 2024-03-25 23:25:34.334901 siyi_sdk-0.2.1/siyi_sdk/tests/test_lock_mode.py
--rw-r--r--   0        0        0     1088 2024-03-25 23:25:34.334901 siyi_sdk-0.2.1/siyi_sdk/tests/test_record_video.py
--rw-r--r--   0        0        0     1213 2024-03-25 23:25:34.334901 siyi_sdk-0.2.1/siyi_sdk/tests/test_rtmp_stream.py
--rw-r--r--   0        0        0      582 2024-03-25 23:25:34.334901 siyi_sdk-0.2.1/siyi_sdk/tests/test_rtsp.py
--rw-r--r--   0        0        0      918 2024-03-25 23:25:34.334901 siyi_sdk-0.2.1/siyi_sdk/tests/test_zoom.py
--rw-r--r--   0        0        0      541 2024-03-25 23:25:34.334901 siyi_sdk-0.2.1/siyi_sdk/tests/udp_server.py
--rw-r--r--   0        0        0     1209 2024-03-28 21:04:24.903711 siyi_sdk-0.2.1/siyi_sdk/utils.py
--rw-r--r--   0        0        0      608 1970-01-01 00:00:00.000000 siyi_sdk-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0       51 2024-03-25 23:21:52.454164 siyi_sdk-0.2.2/README.md
+-rw-r--r--   0        0        0      335 2024-04-03 21:55:12.144840 siyi_sdk-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0       33 2024-03-25 23:25:34.330901 siyi_sdk-0.2.2/siyi_sdk/.git
+-rw-r--r--   0        0        0     3078 2024-03-25 23:25:34.334901 siyi_sdk-0.2.2/siyi_sdk/.gitignore
+-rw-r--r--   0        0        0     1082 2024-03-25 23:25:34.334901 siyi_sdk-0.2.2/siyi_sdk/LICENSE
+-rw-r--r--   0        0        0     4034 2024-03-25 23:25:44.550383 siyi_sdk-0.2.2/siyi_sdk/README.md
+-rw-r--r--   0        0        0       58 2024-03-25 23:25:34.334901 siyi_sdk-0.2.2/siyi_sdk/__init__.py
+-rw-r--r--   0        0        0     4353 2024-03-25 23:25:34.334901 siyi_sdk-0.2.2/siyi_sdk/crc16_python.py
+-rw-r--r--   0        0        0  8385675 2024-03-25 23:25:44.562382 siyi_sdk-0.2.2/siyi_sdk/gui/demo.mp4
+-rw-r--r--   0        0        0    16665 2024-03-25 23:25:44.562382 siyi_sdk-0.2.2/siyi_sdk/gui/gui_tkinter.png
+-rw-r--r--   0        0        0     3994 2024-03-28 21:15:20.435565 siyi_sdk-0.2.2/siyi_sdk/gui/tkgui.py
+-rw-r--r--   0        0        0    12921 2024-03-28 21:04:24.903711 siyi_sdk-0.2.2/siyi_sdk/siyi_message.py
+-rw-r--r--   0        0        0    30319 2024-04-03 21:54:04.268109 siyi_sdk-0.2.2/siyi_sdk/siyi_sdk.py
+-rw-r--r--   0        0        0     9360 2024-03-25 23:25:34.334901 siyi_sdk-0.2.2/siyi_sdk/stream.py
+-rw-r--r--   0        0        0        0 2024-03-25 23:25:34.334901 siyi_sdk-0.2.2/siyi_sdk/tests/__init__.py
+-rw-r--r--   0        0        0      878 2024-03-28 21:04:24.903711 siyi_sdk-0.2.2/siyi_sdk/tests/serial/test_center_gimbal.py
+-rw-r--r--   0        0        0      787 2024-03-28 21:04:24.903711 siyi_sdk-0.2.2/siyi_sdk/tests/serial/test_get_fw_ver.py
+-rw-r--r--   0        0        0      820 2024-03-28 21:04:24.903711 siyi_sdk-0.2.2/siyi_sdk/tests/serial/test_gimbal_position.py
+-rw-r--r--   0        0        0      790 2024-03-28 21:04:24.903711 siyi_sdk-0.2.2/siyi_sdk/tests/serial/test_gimbal_rotation.py
+-rw-r--r--   0        0        0      844 2024-03-25 23:25:34.334901 siyi_sdk-0.2.2/siyi_sdk/tests/test_center_gimbal.py
+-rw-r--r--   0        0        0      746 2024-03-25 23:25:34.334901 siyi_sdk-0.2.2/siyi_sdk/tests/test_follow_mode.py
+-rw-r--r--   0        0        0      737 2024-03-25 23:25:34.334901 siyi_sdk-0.2.2/siyi_sdk/tests/test_fpv_mode.py
+-rw-r--r--   0        0        0      924 2024-03-25 23:25:34.334901 siyi_sdk-0.2.2/siyi_sdk/tests/test_from_rtsp_to_rtmp.py
+-rw-r--r--   0        0        0      753 2024-03-25 23:25:34.334901 siyi_sdk-0.2.2/siyi_sdk/tests/test_get_fw_ver.py
+-rw-r--r--   0        0        0      881 2024-03-25 23:25:34.334901 siyi_sdk-0.2.2/siyi_sdk/tests/test_get_gimbal_info.py
+-rw-r--r--   0        0        0      734 2024-03-25 23:25:34.334901 siyi_sdk-0.2.2/siyi_sdk/tests/test_get_hw_id.py
+-rw-r--r--   0        0        0      774 2024-03-28 21:14:01.390679 siyi_sdk-0.2.2/siyi_sdk/tests/test_gimbal_position.py
+-rw-r--r--   0        0        0      756 2024-03-25 23:25:34.334901 siyi_sdk-0.2.2/siyi_sdk/tests/test_gimbal_rotation.py
+-rw-r--r--   0        0        0      740 2024-03-25 23:25:34.334901 siyi_sdk-0.2.2/siyi_sdk/tests/test_lock_mode.py
+-rw-r--r--   0        0        0     1088 2024-03-25 23:25:34.334901 siyi_sdk-0.2.2/siyi_sdk/tests/test_record_video.py
+-rw-r--r--   0        0        0     1213 2024-03-25 23:25:34.334901 siyi_sdk-0.2.2/siyi_sdk/tests/test_rtmp_stream.py
+-rw-r--r--   0        0        0      582 2024-03-25 23:25:34.334901 siyi_sdk-0.2.2/siyi_sdk/tests/test_rtsp.py
+-rw-r--r--   0        0        0      918 2024-03-25 23:25:34.334901 siyi_sdk-0.2.2/siyi_sdk/tests/test_zoom.py
+-rw-r--r--   0        0        0      541 2024-03-25 23:25:34.334901 siyi_sdk-0.2.2/siyi_sdk/tests/udp_server.py
+-rw-r--r--   0        0        0     1209 2024-03-28 21:04:24.903711 siyi_sdk-0.2.2/siyi_sdk/utils.py
+-rw-r--r--   0        0        0      608 1970-01-01 00:00:00.000000 siyi_sdk-0.2.2/PKG-INFO
```

### Comparing `siyi_sdk-0.2.1/siyi_sdk/.gitignore` & `siyi_sdk-0.2.2/siyi_sdk/.gitignore`

 * *Files identical despite different names*

### Comparing `siyi_sdk-0.2.1/siyi_sdk/LICENSE` & `siyi_sdk-0.2.2/siyi_sdk/LICENSE`

 * *Files identical despite different names*

### Comparing `siyi_sdk-0.2.1/siyi_sdk/README.md` & `siyi_sdk-0.2.2/siyi_sdk/README.md`

 * *Files identical despite different names*

### Comparing `siyi_sdk-0.2.1/siyi_sdk/crc16_python.py` & `siyi_sdk-0.2.2/siyi_sdk/crc16_python.py`

 * *Files identical despite different names*

### Comparing `siyi_sdk-0.2.1/siyi_sdk/gui/demo.mp4` & `siyi_sdk-0.2.2/siyi_sdk/gui/demo.mp4`

 * *Files identical despite different names*

### Comparing `siyi_sdk-0.2.1/siyi_sdk/gui/gui_tkinter.png` & `siyi_sdk-0.2.2/siyi_sdk/gui/gui_tkinter.png`

 * *Files identical despite different names*

### Comparing `siyi_sdk-0.2.1/siyi_sdk/gui/tkgui.py` & `siyi_sdk-0.2.2/siyi_sdk/gui/tkgui.py`

 * *Files identical despite different names*

### Comparing `siyi_sdk-0.2.1/siyi_sdk/siyi_message.py` & `siyi_sdk-0.2.2/siyi_sdk/siyi_message.py`

 * *Files identical despite different names*

### Comparing `siyi_sdk-0.2.1/siyi_sdk/siyi_sdk.py` & `siyi_sdk-0.2.2/siyi_sdk/siyi_sdk.py`

 * *Files 0% similar despite different names*

```diff
@@ -833,16 +833,16 @@
         err_thresh: [float] acceptable error threshold, in degrees, to stop correction
         kp [float] proportional gain
         """
         if (pitch >25 or pitch <-90):
             self._logger.error("desired pitch is outside controllable range -90~25")
             return
 
-        if (yaw >45 or yaw <-45):
-            self._logger.error("Desired yaw is outside controllable range -45~45")
+        if (yaw >130 or yaw <-130):
+            self._logger.error("Desired yaw is outside controllable range -130~130")
             return
 
         th = err_thresh
         gain = kp
         while(True):
             self.requestGimbalAttitude()
             if self._att_msg.seq==self._last_att_seq:
```

### Comparing `siyi_sdk-0.2.1/siyi_sdk/stream.py` & `siyi_sdk-0.2.2/siyi_sdk/stream.py`

 * *Files identical despite different names*

### Comparing `siyi_sdk-0.2.1/siyi_sdk/tests/serial/test_center_gimbal.py` & `siyi_sdk-0.2.2/siyi_sdk/tests/serial/test_center_gimbal.py`

 * *Files identical despite different names*

### Comparing `siyi_sdk-0.2.1/siyi_sdk/tests/serial/test_get_fw_ver.py` & `siyi_sdk-0.2.2/siyi_sdk/tests/serial/test_get_fw_ver.py`

 * *Files identical despite different names*

### Comparing `siyi_sdk-0.2.1/siyi_sdk/tests/serial/test_gimbal_position.py` & `siyi_sdk-0.2.2/siyi_sdk/tests/serial/test_gimbal_position.py`

 * *Files identical despite different names*

### Comparing `siyi_sdk-0.2.1/siyi_sdk/tests/serial/test_gimbal_rotation.py` & `siyi_sdk-0.2.2/siyi_sdk/tests/serial/test_gimbal_rotation.py`

 * *Files identical despite different names*

### Comparing `siyi_sdk-0.2.1/siyi_sdk/tests/test_center_gimbal.py` & `siyi_sdk-0.2.2/siyi_sdk/tests/test_center_gimbal.py`

 * *Files identical despite different names*

### Comparing `siyi_sdk-0.2.1/siyi_sdk/tests/test_follow_mode.py` & `siyi_sdk-0.2.2/siyi_sdk/tests/test_follow_mode.py`

 * *Files identical despite different names*

### Comparing `siyi_sdk-0.2.1/siyi_sdk/tests/test_fpv_mode.py` & `siyi_sdk-0.2.2/siyi_sdk/tests/test_fpv_mode.py`

 * *Files identical despite different names*

### Comparing `siyi_sdk-0.2.1/siyi_sdk/tests/test_from_rtsp_to_rtmp.py` & `siyi_sdk-0.2.2/siyi_sdk/tests/test_from_rtsp_to_rtmp.py`

 * *Files identical despite different names*

### Comparing `siyi_sdk-0.2.1/siyi_sdk/tests/test_get_fw_ver.py` & `siyi_sdk-0.2.2/siyi_sdk/tests/test_get_fw_ver.py`

 * *Files identical despite different names*

### Comparing `siyi_sdk-0.2.1/siyi_sdk/tests/test_get_gimbal_info.py` & `siyi_sdk-0.2.2/siyi_sdk/tests/test_get_gimbal_info.py`

 * *Files identical despite different names*

### Comparing `siyi_sdk-0.2.1/siyi_sdk/tests/test_get_hw_id.py` & `siyi_sdk-0.2.2/siyi_sdk/tests/test_get_hw_id.py`

 * *Files identical despite different names*

### Comparing `siyi_sdk-0.2.1/siyi_sdk/tests/test_gimbal_position.py` & `siyi_sdk-0.2.2/siyi_sdk/tests/test_gimbal_position.py`

 * *Files identical despite different names*

### Comparing `siyi_sdk-0.2.1/siyi_sdk/tests/test_gimbal_rotation.py` & `siyi_sdk-0.2.2/siyi_sdk/tests/test_gimbal_rotation.py`

 * *Files identical despite different names*

### Comparing `siyi_sdk-0.2.1/siyi_sdk/tests/test_lock_mode.py` & `siyi_sdk-0.2.2/siyi_sdk/tests/test_lock_mode.py`

 * *Files identical despite different names*

### Comparing `siyi_sdk-0.2.1/siyi_sdk/tests/test_record_video.py` & `siyi_sdk-0.2.2/siyi_sdk/tests/test_record_video.py`

 * *Files identical despite different names*

### Comparing `siyi_sdk-0.2.1/siyi_sdk/tests/test_rtmp_stream.py` & `siyi_sdk-0.2.2/siyi_sdk/tests/test_rtmp_stream.py`

 * *Files identical despite different names*

### Comparing `siyi_sdk-0.2.1/siyi_sdk/tests/test_rtsp.py` & `siyi_sdk-0.2.2/siyi_sdk/tests/test_rtsp.py`

 * *Files identical despite different names*

### Comparing `siyi_sdk-0.2.1/siyi_sdk/tests/test_zoom.py` & `siyi_sdk-0.2.2/siyi_sdk/tests/test_zoom.py`

 * *Files identical despite different names*

### Comparing `siyi_sdk-0.2.1/siyi_sdk/tests/udp_server.py` & `siyi_sdk-0.2.2/siyi_sdk/tests/udp_server.py`

 * *Files identical despite different names*

### Comparing `siyi_sdk-0.2.1/siyi_sdk/utils.py` & `siyi_sdk-0.2.2/siyi_sdk/utils.py`

 * *Files identical despite different names*

### Comparing `siyi_sdk-0.2.1/PKG-INFO` & `siyi_sdk-0.2.2/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: siyi-sdk
-Version: 0.2.1
+Version: 0.2.2
 Summary: SIYI gimbal camera SDK
 Author: Soter Technology
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

