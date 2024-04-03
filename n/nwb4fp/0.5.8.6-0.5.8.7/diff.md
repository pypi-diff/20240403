# Comparing `tmp/nwb4fp-0.5.8.6.tar.gz` & `tmp/nwb4fp-0.5.8.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nwb4fp-0.5.8.6.tar", last modified: Wed Apr  3 10:02:12 2024, max compression
+gzip compressed data, was "nwb4fp-0.5.8.7.tar", last modified: Wed Apr  3 10:24:53 2024, max compression
```

## Comparing `nwb4fp-0.5.8.6.tar` & `nwb4fp-0.5.8.7.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxrwxrwx   0        0        0        0 2024-04-03 10:02:12.920225 nwb4fp-0.5.8.6/
--rw-rw-rw-   0        0        0     1089 2024-02-24 13:06:48.000000 nwb4fp-0.5.8.6/LICENSE
--rw-rw-rw-   0        0        0     5786 2024-04-03 10:02:12.914224 nwb4fp-0.5.8.6/PKG-INFO
--rw-rw-rw-   0        0        0     6901 2024-03-27 14:22:15.000000 nwb4fp-0.5.8.6/README.md
--rw-rw-rw-   0        0        0       42 2024-04-03 10:02:12.935225 nwb4fp-0.5.8.6/setup.cfg
--rw-rw-rw-   0        0        0      881 2024-04-03 10:02:09.000000 nwb4fp-0.5.8.6/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-03 10:02:12.392225 nwb4fp-0.5.8.6/src/
-drwxrwxrwx   0        0        0        0 2024-04-03 10:02:12.529227 nwb4fp-0.5.8.6/src/nwb4fp/
--rw-rw-rw-   0        0        0        0 2024-03-03 17:04:21.000000 nwb4fp-0.5.8.6/src/nwb4fp/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-03 10:02:12.626228 nwb4fp-0.5.8.6/src/nwb4fp/main/
--rw-rw-rw-   0        0        0        0 2024-03-08 16:12:29.000000 nwb4fp-0.5.8.6/src/nwb4fp/main/__init__.py
--rw-rw-rw-   0        0        0     3593 2024-03-29 11:35:18.000000 nwb4fp-0.5.8.6/src/nwb4fp/main/main_create_nwb.py
-drwxrwxrwx   0        0        0        0 2024-04-03 10:02:12.672226 nwb4fp-0.5.8.6/src/nwb4fp/postprocess/
--rw-rw-rw-   0        0        0    15551 2024-03-27 11:37:25.000000 nwb4fp-0.5.8.6/src/nwb4fp/postprocess/Get_positions.py
--rw-rw-rw-   0        0        0        0 2024-02-15 18:06:22.000000 nwb4fp-0.5.8.6/src/nwb4fp/postprocess/__init__.py
--rw-rw-rw-   0        0        0     1614 2024-02-21 21:21:29.000000 nwb4fp-0.5.8.6/src/nwb4fp/postprocess/add_wfcor.py
--rw-rw-rw-   0        0        0      470 2024-03-24 12:00:57.000000 nwb4fp-0.5.8.6/src/nwb4fp/postprocess/dlc_kinematic.py
--rw-rw-rw-   0        0        0     2485 2024-03-29 14:47:19.000000 nwb4fp-0.5.8.6/src/nwb4fp/postprocess/extract_wf.py
--rw-rw-rw-   0        0        0     1445 2024-03-03 15:56:30.000000 nwb4fp-0.5.8.6/src/nwb4fp/postprocess/get_potential_merge.py
--rw-rw-rw-   0        0        0     9965 2024-04-03 10:01:49.000000 nwb4fp-0.5.8.6/src/nwb4fp/postprocess/nwbPHYnOPHYS.py
--rw-rw-rw-   0        0        0    11891 2024-04-01 17:16:46.000000 nwb4fp-0.5.8.6/src/nwb4fp/postprocess/quality_metrix.py
-drwxrwxrwx   0        0        0        0 2024-04-03 10:02:12.418237 nwb4fp-0.5.8.6/src/nwb4fp/preprocess/
--rw-rw-rw-   0        0        0        0 2024-02-27 13:40:23.000000 nwb4fp-0.5.8.6/src/nwb4fp/preprocess/__init__.py
--rw-rw-rw-   0        0        0      459 2024-02-27 13:40:23.000000 nwb4fp-0.5.8.6/src/nwb4fp/preprocess/copy_file.py
--rw-rw-rw-   0        0        0      620 2024-02-27 13:40:23.000000 nwb4fp-0.5.8.6/src/nwb4fp/preprocess/down_sample.py
--rw-rw-rw-   0        0        0     6762 2024-03-05 12:39:24.000000 nwb4fp-0.5.8.6/src/nwb4fp/preprocess/down_sample_lfp.py
--rw-rw-rw-   0        0        0     3712 2024-02-27 13:40:23.000000 nwb4fp-0.5.8.6/src/nwb4fp/preprocess/extract_lfp.py
--rw-rw-rw-   0        0        0      148 2024-02-27 13:40:23.000000 nwb4fp-0.5.8.6/src/nwb4fp/preprocess/get_path.py
--rw-rw-rw-   0        0        0     1203 2024-02-27 13:40:23.000000 nwb4fp-0.5.8.6/src/nwb4fp/preprocess/load_data.py
--rw-rw-rw-   0        0        0      244 2024-02-27 13:40:23.000000 nwb4fp-0.5.8.6/src/nwb4fp/preprocess/run_phy.py
-drwxrwxrwx   0        0        0        0 2024-04-03 10:02:12.423227 nwb4fp-0.5.8.6/src/nwb4fp/test/
-drwxrwxrwx   0        0        0        0 2024-04-03 10:02:12.427231 nwb4fp-0.5.8.6/src/nwb4fp/test/run_scripts/
--rw-rw-rw-   0        0        0     1552 2024-04-03 09:55:04.000000 nwb4fp-0.5.8.6/src/nwb4fp/test/run_scripts/readnwb.py
--rw-rw-rw-   0        0        0     1454 2024-04-03 09:24:14.000000 nwb4fp-0.5.8.6/src/nwb4fp/test/run_scripts/readnwb_09PC.py
--rw-rw-rw-   0        0        0        0 2024-03-13 14:23:55.000000 nwb4fp-0.5.8.6/src/nwb4fp/test/run_scripts/test.py
-drwxrwxrwx   0        0        0        0 2024-04-03 10:02:12.392225 nwb4fp-0.5.8.6/src/nwb4fp.egg-info/
--rw-rw-rw-   0        0        0     5786 2024-04-03 10:02:12.000000 nwb4fp-0.5.8.6/src/nwb4fp.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1000 2024-04-03 10:02:12.000000 nwb4fp-0.5.8.6/src/nwb4fp.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-03 10:02:12.000000 nwb4fp-0.5.8.6/src/nwb4fp.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0     2916 2024-04-03 10:02:12.000000 nwb4fp-0.5.8.6/src/nwb4fp.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2024-04-03 10:02:12.000000 nwb4fp-0.5.8.6/src/nwb4fp.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-03 10:24:53.539119 nwb4fp-0.5.8.7/
+-rw-rw-rw-   0        0        0     1089 2024-02-24 13:06:48.000000 nwb4fp-0.5.8.7/LICENSE
+-rw-rw-rw-   0        0        0     5786 2024-04-03 10:24:53.531122 nwb4fp-0.5.8.7/PKG-INFO
+-rw-rw-rw-   0        0        0     6901 2024-03-27 14:22:15.000000 nwb4fp-0.5.8.7/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-03 10:24:53.555112 nwb4fp-0.5.8.7/setup.cfg
+-rw-rw-rw-   0        0        0      881 2024-04-03 10:24:32.000000 nwb4fp-0.5.8.7/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-03 10:24:52.683118 nwb4fp-0.5.8.7/src/
+drwxrwxrwx   0        0        0        0 2024-04-03 10:24:52.810119 nwb4fp-0.5.8.7/src/nwb4fp/
+-rw-rw-rw-   0        0        0        0 2024-03-03 17:04:21.000000 nwb4fp-0.5.8.7/src/nwb4fp/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-03 10:24:52.916113 nwb4fp-0.5.8.7/src/nwb4fp/main/
+-rw-rw-rw-   0        0        0        0 2024-03-08 16:12:29.000000 nwb4fp-0.5.8.7/src/nwb4fp/main/__init__.py
+-rw-rw-rw-   0        0        0     3593 2024-03-29 11:35:18.000000 nwb4fp-0.5.8.7/src/nwb4fp/main/main_create_nwb.py
+drwxrwxrwx   0        0        0        0 2024-04-03 10:24:53.144114 nwb4fp-0.5.8.7/src/nwb4fp/postprocess/
+-rw-rw-rw-   0        0        0    15551 2024-03-27 11:37:25.000000 nwb4fp-0.5.8.7/src/nwb4fp/postprocess/Get_positions.py
+-rw-rw-rw-   0        0        0        0 2024-02-15 18:06:22.000000 nwb4fp-0.5.8.7/src/nwb4fp/postprocess/__init__.py
+-rw-rw-rw-   0        0        0     1614 2024-02-21 21:21:29.000000 nwb4fp-0.5.8.7/src/nwb4fp/postprocess/add_wfcor.py
+-rw-rw-rw-   0        0        0      470 2024-03-24 12:00:57.000000 nwb4fp-0.5.8.7/src/nwb4fp/postprocess/dlc_kinematic.py
+-rw-rw-rw-   0        0        0     2485 2024-03-29 14:47:19.000000 nwb4fp-0.5.8.7/src/nwb4fp/postprocess/extract_wf.py
+-rw-rw-rw-   0        0        0     1445 2024-03-03 15:56:30.000000 nwb4fp-0.5.8.7/src/nwb4fp/postprocess/get_potential_merge.py
+-rw-rw-rw-   0        0        0    10141 2024-04-03 10:24:11.000000 nwb4fp-0.5.8.7/src/nwb4fp/postprocess/nwbPHYnOPHYS.py
+-rw-rw-rw-   0        0        0    11891 2024-04-01 17:16:46.000000 nwb4fp-0.5.8.7/src/nwb4fp/postprocess/quality_metrix.py
+drwxrwxrwx   0        0        0        0 2024-04-03 10:24:53.375111 nwb4fp-0.5.8.7/src/nwb4fp/preprocess/
+-rw-rw-rw-   0        0        0        0 2024-02-27 13:40:23.000000 nwb4fp-0.5.8.7/src/nwb4fp/preprocess/__init__.py
+-rw-rw-rw-   0        0        0      459 2024-02-27 13:40:23.000000 nwb4fp-0.5.8.7/src/nwb4fp/preprocess/copy_file.py
+-rw-rw-rw-   0        0        0      620 2024-02-27 13:40:23.000000 nwb4fp-0.5.8.7/src/nwb4fp/preprocess/down_sample.py
+-rw-rw-rw-   0        0        0     6762 2024-03-05 12:39:24.000000 nwb4fp-0.5.8.7/src/nwb4fp/preprocess/down_sample_lfp.py
+-rw-rw-rw-   0        0        0     3712 2024-02-27 13:40:23.000000 nwb4fp-0.5.8.7/src/nwb4fp/preprocess/extract_lfp.py
+-rw-rw-rw-   0        0        0      148 2024-02-27 13:40:23.000000 nwb4fp-0.5.8.7/src/nwb4fp/preprocess/get_path.py
+-rw-rw-rw-   0        0        0     1203 2024-02-27 13:40:23.000000 nwb4fp-0.5.8.7/src/nwb4fp/preprocess/load_data.py
+-rw-rw-rw-   0        0        0      244 2024-02-27 13:40:23.000000 nwb4fp-0.5.8.7/src/nwb4fp/preprocess/run_phy.py
+drwxrwxrwx   0        0        0        0 2024-04-03 10:24:52.705121 nwb4fp-0.5.8.7/src/nwb4fp/test/
+drwxrwxrwx   0        0        0        0 2024-04-03 10:24:53.444116 nwb4fp-0.5.8.7/src/nwb4fp/test/run_scripts/
+-rw-rw-rw-   0        0        0     1552 2024-04-03 09:55:04.000000 nwb4fp-0.5.8.7/src/nwb4fp/test/run_scripts/readnwb.py
+-rw-rw-rw-   0        0        0     1454 2024-04-03 09:24:14.000000 nwb4fp-0.5.8.7/src/nwb4fp/test/run_scripts/readnwb_09PC.py
+-rw-rw-rw-   0        0        0        0 2024-03-13 14:23:55.000000 nwb4fp-0.5.8.7/src/nwb4fp/test/run_scripts/test.py
+drwxrwxrwx   0        0        0        0 2024-04-03 10:24:52.880120 nwb4fp-0.5.8.7/src/nwb4fp.egg-info/
+-rw-rw-rw-   0        0        0     5786 2024-04-03 10:24:52.000000 nwb4fp-0.5.8.7/src/nwb4fp.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1000 2024-04-03 10:24:52.000000 nwb4fp-0.5.8.7/src/nwb4fp.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-03 10:24:52.000000 nwb4fp-0.5.8.7/src/nwb4fp.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0     2916 2024-04-03 10:24:52.000000 nwb4fp-0.5.8.7/src/nwb4fp.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2024-04-03 10:24:52.000000 nwb4fp-0.5.8.7/src/nwb4fp.egg-info/top_level.txt
```

### Comparing `nwb4fp-0.5.8.6/LICENSE` & `nwb4fp-0.5.8.7/LICENSE`

 * *Files identical despite different names*

### Comparing `nwb4fp-0.5.8.6/PKG-INFO` & `nwb4fp-0.5.8.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nwb4fp
-Version: 0.5.8.6
+Version: 0.5.8.7
 Summary: Description of my package
 Home-page: https://github.com/sachuriga283/nwb4fp
 Author: sachuriga283
 Author-email: sachuriga.sachuriga@ntnu.no
 License-File: LICENSE
 Requires-Dist: aiobotocore==2.11.2
 Requires-Dist: aiohttp==3.9.3
```

### Comparing `nwb4fp-0.5.8.6/README.md` & `nwb4fp-0.5.8.7/README.md`

 * *Files identical despite different names*

### Comparing `nwb4fp-0.5.8.6/setup.py` & `nwb4fp-0.5.8.7/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -7,15 +7,15 @@
             return [line.strip() for line in req if line.strip() and not line.startswith('#')]
     except UnicodeDecodeError:
         with open('requirements.txt', encoding='utf-16') as req:
             return [line.strip() for line in req if line.strip() and not line.startswith('#')]
 
 setup(
     name='nwb4fp',
-    version='0.5.8.6',
+    version='0.5.8.7',
     url='https://github.com/sachuriga283/nwb4fp',
     author='sachuriga283',
     author_email='sachuriga.sachuriga@ntnu.no',
     description='Description of my package',
     #packages=find_packages(./src/),    
     install_requires=read_requirements(),
 )
```

### Comparing `nwb4fp-0.5.8.6/src/nwb4fp/main/main_create_nwb.py` & `nwb4fp-0.5.8.7/src/nwb4fp/main/main_create_nwb.py`

 * *Files identical despite different names*

### Comparing `nwb4fp-0.5.8.6/src/nwb4fp/postprocess/Get_positions.py` & `nwb4fp-0.5.8.7/src/nwb4fp/postprocess/Get_positions.py`

 * *Files identical despite different names*

### Comparing `nwb4fp-0.5.8.6/src/nwb4fp/postprocess/add_wfcor.py` & `nwb4fp-0.5.8.7/src/nwb4fp/postprocess/add_wfcor.py`

 * *Files identical despite different names*

### Comparing `nwb4fp-0.5.8.6/src/nwb4fp/postprocess/extract_wf.py` & `nwb4fp-0.5.8.7/src/nwb4fp/postprocess/extract_wf.py`

 * *Files identical despite different names*

### Comparing `nwb4fp-0.5.8.6/src/nwb4fp/postprocess/get_potential_merge.py` & `nwb4fp-0.5.8.7/src/nwb4fp/postprocess/get_potential_merge.py`

 * *Files identical despite different names*

### Comparing `nwb4fp-0.5.8.6/src/nwb4fp/postprocess/nwbPHYnOPHYS.py` & `nwb4fp-0.5.8.7/src/nwb4fp/postprocess/nwbPHYnOPHYS.py`

 * *Files 2% similar despite different names*

```diff
@@ -58,18 +58,20 @@
             print("tried" + fr"{stream_name}")
             stream_name = 'Record Node 102#OE_FPGA_Acquisition_Board-101.Rhythm Data'
             interface_ophys = OpenEphysRecordingInterface(folder_path=folder_path,stream_name=stream_name)
         except AssertionError:
             try:
                 folder_path = fr"{ECEPHY_DATA_PATH}/Record Node 101"
                 print("tried" + fr"{stream_name}")
-                stream_name = 'Record Node 101#OE_FPGA_Acquisition_Board-101.Rhythm Data'
+                stream_name = 'Record Node 101#Acquisition_Board-100.Rhythm Data'
+                #stream_name = 'Record Node 101#OE_FPGA_Acquisition_Board-101.Rhythm Data'
                 interface_ophys = OpenEphysRecordingInterface(folder_path=folder_path,stream_name=stream_name)
             except AssertionError:
-                stream_name = 'Record Node 101#Acquisition_Board-100.Rhythm Data'
+                #stream_name = 'Record Node 101#Acquisition_Board-100.Rhythm Data'
+                stream_name = 'Record Node 101#OE_FPGA_Acquisition_Board-101.Rhythm Data'
                 print("tried" + fr"{stream_name}")
                 interface_ophys = OpenEphysRecordingInterface(folder_path=folder_path,stream_name=stream_name)
 
     # Extract what metadata we can from the source files
     folder1_path = f"{path}"  # Change the folder_path to the location of the data in your system
     print(fr"Animal number is {UD[0]}")
     # if UD[0] == "65410":
```

### Comparing `nwb4fp-0.5.8.6/src/nwb4fp/postprocess/quality_metrix.py` & `nwb4fp-0.5.8.7/src/nwb4fp/postprocess/quality_metrix.py`

 * *Files identical despite different names*

### Comparing `nwb4fp-0.5.8.6/src/nwb4fp/preprocess/down_sample.py` & `nwb4fp-0.5.8.7/src/nwb4fp/preprocess/down_sample.py`

 * *Files identical despite different names*

### Comparing `nwb4fp-0.5.8.6/src/nwb4fp/preprocess/down_sample_lfp.py` & `nwb4fp-0.5.8.7/src/nwb4fp/preprocess/down_sample_lfp.py`

 * *Files identical despite different names*

### Comparing `nwb4fp-0.5.8.6/src/nwb4fp/preprocess/extract_lfp.py` & `nwb4fp-0.5.8.7/src/nwb4fp/preprocess/extract_lfp.py`

 * *Files identical despite different names*

### Comparing `nwb4fp-0.5.8.6/src/nwb4fp/preprocess/load_data.py` & `nwb4fp-0.5.8.7/src/nwb4fp/preprocess/load_data.py`

 * *Files identical despite different names*

### Comparing `nwb4fp-0.5.8.6/src/nwb4fp/test/run_scripts/readnwb.py` & `nwb4fp-0.5.8.7/src/nwb4fp/test/run_scripts/readnwb.py`

 * *Files identical despite different names*

### Comparing `nwb4fp-0.5.8.6/src/nwb4fp/test/run_scripts/readnwb_09PC.py` & `nwb4fp-0.5.8.7/src/nwb4fp/test/run_scripts/readnwb_09PC.py`

 * *Files identical despite different names*

### Comparing `nwb4fp-0.5.8.6/src/nwb4fp.egg-info/PKG-INFO` & `nwb4fp-0.5.8.7/src/nwb4fp.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nwb4fp
-Version: 0.5.8.6
+Version: 0.5.8.7
 Summary: Description of my package
 Home-page: https://github.com/sachuriga283/nwb4fp
 Author: sachuriga283
 Author-email: sachuriga.sachuriga@ntnu.no
 License-File: LICENSE
 Requires-Dist: aiobotocore==2.11.2
 Requires-Dist: aiohttp==3.9.3
```

### Comparing `nwb4fp-0.5.8.6/src/nwb4fp.egg-info/SOURCES.txt` & `nwb4fp-0.5.8.7/src/nwb4fp.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nwb4fp-0.5.8.6/src/nwb4fp.egg-info/requires.txt` & `nwb4fp-0.5.8.7/src/nwb4fp.egg-info/requires.txt`

 * *Files identical despite different names*
