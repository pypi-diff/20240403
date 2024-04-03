# Comparing `tmp/yayy-0.1.0.tar.gz` & `tmp/yayy-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yayy-0.1.0.tar", last modified: Wed Apr  3 14:34:11 2024, max compression
+gzip compressed data, was "yayy-0.1.1.tar", last modified: Wed Apr  3 14:56:01 2024, max compression
```

## Comparing `yayy-0.1.0.tar` & `yayy-0.1.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2024-04-03 14:34:11.875880 yayy-0.1.0/
--rw-rw-rw-   0        0        0     1058 2023-12-28 09:22:07.000000 yayy-0.1.0/LICENSE
--rw-rw-rw-   0        0        0     1640 2024-04-03 14:34:11.872828 yayy-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0     1245 2024-04-03 14:32:07.000000 yayy-0.1.0/README.md
--rw-rw-rw-   0        0        0       42 2024-04-03 14:34:11.876729 yayy-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0      867 2024-04-03 14:29:55.000000 yayy-0.1.0/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-03 14:34:11.838061 yayy-0.1.0/yayy/
--rw-rw-rw-   0        0        0       19 2024-03-23 13:35:28.000000 yayy-0.1.0/yayy/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-03 14:34:11.872828 yayy-0.1.0/yayy/assets/
--rw-rw-rw-   0        0        0       29 2024-03-25 17:52:46.000000 yayy-0.1.0/yayy/assets/data.json
--rw-rw-rw-   0        0        0      890 2024-04-03 14:32:19.000000 yayy-0.1.0/yayy/constants.py
--rw-rw-rw-   0        0        0     2552 2024-04-03 14:33:30.000000 yayy-0.1.0/yayy/main.py
--rw-rw-rw-   0        0        0     3019 2024-04-03 14:26:49.000000 yayy-0.1.0/yayy/utils.py
-drwxrwxrwx   0        0        0        0 2024-04-03 14:34:11.872828 yayy-0.1.0/yayy.egg-info/
--rw-rw-rw-   0        0        0     1640 2024-04-03 14:34:11.000000 yayy-0.1.0/yayy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      280 2024-04-03 14:34:11.000000 yayy-0.1.0/yayy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-03 14:34:11.000000 yayy-0.1.0/yayy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       39 2024-04-03 14:34:11.000000 yayy-0.1.0/yayy.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       40 2024-04-03 14:34:11.000000 yayy-0.1.0/yayy.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2024-04-03 14:34:11.000000 yayy-0.1.0/yayy.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-03 14:56:01.157930 yayy-0.1.1/
+-rw-rw-rw-   0        0        0     1058 2023-12-28 09:22:07.000000 yayy-0.1.1/LICENSE
+-rw-rw-rw-   0        0        0     1627 2024-04-03 14:56:01.157930 yayy-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0     1232 2024-04-03 14:55:36.000000 yayy-0.1.1/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-03 14:56:01.157930 yayy-0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0      867 2024-04-03 14:55:42.000000 yayy-0.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-03 14:56:01.117154 yayy-0.1.1/yayy/
+-rw-rw-rw-   0        0        0       19 2024-03-23 13:35:28.000000 yayy-0.1.1/yayy/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-03 14:56:01.156487 yayy-0.1.1/yayy/assets/
+-rw-rw-rw-   0        0        0       29 2024-03-25 17:52:46.000000 yayy-0.1.1/yayy/assets/data.json
+-rw-rw-rw-   0        0        0      890 2024-04-03 14:32:19.000000 yayy-0.1.1/yayy/constants.py
+-rw-rw-rw-   0        0        0     2552 2024-04-03 14:35:33.000000 yayy-0.1.1/yayy/main.py
+-rw-rw-rw-   0        0        0     3019 2024-04-03 14:26:49.000000 yayy-0.1.1/yayy/utils.py
+drwxrwxrwx   0        0        0        0 2024-04-03 14:56:01.155447 yayy-0.1.1/yayy.egg-info/
+-rw-rw-rw-   0        0        0     1627 2024-04-03 14:56:01.000000 yayy-0.1.1/yayy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      280 2024-04-03 14:56:01.000000 yayy-0.1.1/yayy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-03 14:56:01.000000 yayy-0.1.1/yayy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       39 2024-04-03 14:56:01.000000 yayy-0.1.1/yayy.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       40 2024-04-03 14:56:01.000000 yayy-0.1.1/yayy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2024-04-03 14:56:01.000000 yayy-0.1.1/yayy.egg-info/top_level.txt
```

### Comparing `yayy-0.1.0/LICENSE` & `yayy-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `yayy-0.1.0/PKG-INFO` & `yayy-0.1.1/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,25 +1,15 @@
-Metadata-Version: 2.1
-Name: yayy
-Version: 0.1.0
-Summary: Si Un Problema Puede Solucionarse, Entonces No Vale La Pena Preocuparse Por El.
-Author: Pablo Escobar
-License: MIT
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # yayy
 
-### Installation
-Copy and save the below file as `install.bat`
+## Scripts
 
-```
+These are batch files, save them in a .bat format.
+
+1. `install.bat`
+```bat
 @echo off
 echo Installing yayy Python package...
 
 REM Check if pip is installed
 python -m pip --version >nul 2>&1
 if %errorlevel% neq 0 (
     echo Error: Python pip is not installed or not in PATH.
@@ -33,31 +23,33 @@
 if %errorlevel% equ 0 (
     echo yayy installed successfully.
 ) else (
     echo Error: Failed to install yayy.
     exit /b 1
 )
 
-REM Install disdial package
-python -m pip install disdial
-
-REM Check if installation was successful
-if %errorlevel% equ 0 (
-    echo Disdial installed successfully.
-) else (
-    echo Error: Failed to install Disdial.
-    exit /b 1
-)
-
 exit /b 0
 ```
 
-<!-- 1. Run `install.bat` file  -->
+2. `run.bat`
+```bat
+@echo off
+echo Running yayy...
+
+REM
+yay
+
+echo yayy execution completed.
+
+pause
+```
 
-### Usage:
-1. Get your gemini api key from [here](https://aistudio.google.com/app/apikey).
-3. Type `yay` in the terminal or you can run the `run.bat` script, find it [here](misc/run.bat).
-4. Paste the gemini api key (only asked for the first time).
-5. Now copy your questions and paste them in the terminal window by just pressing the enter key.
-6. You should receive your answers.
+## Note:
+- Get your gemini api key from [here](https://aistudio.google.com/app/apikey).
+- You may use the execution Type `yay` in the terminal to run the script directly from the terminal.
+- Copy da MCQ and paste it in the terminal by simply pressing enter key.
+- Wait for the answers to arrive.
+- Supported OS: Windows 11
+- To reset terminal opacity back to 100%, rerun the tool and kill the process by pressing `ctrl+c`.
 
-### Demo Link
+# Lastly
+![image](https://github.com/arpy8/queky/assets/74809468/671d24e4-77a6-474b-a083-730b2874f15f)
```

### Comparing `yayy-0.1.0/setup.py` & `yayy-0.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as f:
     long_description = f.read()
 
 setup(
     name="yayy",
-    version="0.1.0",
+    version="0.1.1",
     author="Pablo Escobar",
     description="Si Un Problema Puede Solucionarse, Entonces No Vale La Pena Preocuparse Por El.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=find_packages(),
     install_requires=["pyperclip", "google-generativeai", "pyautogui"],
     entry_points={
```

### Comparing `yayy-0.1.0/yayy/constants.py` & `yayy-0.1.1/yayy/constants.py`

 * *Files identical despite different names*

### Comparing `yayy-0.1.0/yayy/main.py` & `yayy-0.1.1/yayy/main.py`

 * *Files identical despite different names*

### Comparing `yayy-0.1.0/yayy/utils.py` & `yayy-0.1.1/yayy/utils.py`

 * *Files identical despite different names*

### Comparing `yayy-0.1.0/yayy.egg-info/PKG-INFO` & `yayy-0.1.1/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,25 +1,27 @@
 Metadata-Version: 2.1
 Name: yayy
-Version: 0.1.0
+Version: 0.1.1
 Summary: Si Un Problema Puede Solucionarse, Entonces No Vale La Pena Preocuparse Por El.
 Author: Pablo Escobar
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # yayy
 
-### Installation
-Copy and save the below file as `install.bat`
+## Scripts
 
-```
+These are batch files, save them in a .bat format.
+
+1. `install.bat`
+```bat
 @echo off
 echo Installing yayy Python package...
 
 REM Check if pip is installed
 python -m pip --version >nul 2>&1
 if %errorlevel% neq 0 (
     echo Error: Python pip is not installed or not in PATH.
@@ -33,31 +35,33 @@
 if %errorlevel% equ 0 (
     echo yayy installed successfully.
 ) else (
     echo Error: Failed to install yayy.
     exit /b 1
 )
 
-REM Install disdial package
-python -m pip install disdial
-
-REM Check if installation was successful
-if %errorlevel% equ 0 (
-    echo Disdial installed successfully.
-) else (
-    echo Error: Failed to install Disdial.
-    exit /b 1
-)
-
 exit /b 0
 ```
 
-<!-- 1. Run `install.bat` file  -->
+2. `run.bat`
+```bat
+@echo off
+echo Running yayy...
+
+REM
+yay
+
+echo yayy execution completed.
+
+pause
+```
 
-### Usage:
-1. Get your gemini api key from [here](https://aistudio.google.com/app/apikey).
-3. Type `yay` in the terminal or you can run the `run.bat` script, find it [here](misc/run.bat).
-4. Paste the gemini api key (only asked for the first time).
-5. Now copy your questions and paste them in the terminal window by just pressing the enter key.
-6. You should receive your answers.
+## Note:
+- Get your gemini api key from [here](https://aistudio.google.com/app/apikey).
+- You may use the execution Type `yay` in the terminal to run the script directly from the terminal.
+- Copy da MCQ and paste it in the terminal by simply pressing enter key.
+- Wait for the answers to arrive.
+- Supported OS: Windows 11
+- To reset terminal opacity back to 100%, rerun the tool and kill the process by pressing `ctrl+c`.
 
-### Demo Link
+# Lastly
+![image](https://github.com/arpy8/queky/assets/74809468/671d24e4-77a6-474b-a083-730b2874f15f)
```

