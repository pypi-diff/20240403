# Comparing `tmp/yayy-0.1.1.tar.gz` & `tmp/yayy-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yayy-0.1.1.tar", last modified: Wed Apr  3 14:56:01 2024, max compression
+gzip compressed data, was "yayy-0.1.3.tar", last modified: Wed Apr  3 15:11:23 2024, max compression
```

## Comparing `yayy-0.1.1.tar` & `yayy-0.1.3.tar`

### file list

```diff
@@ -1,20 +1,19 @@
-drwxrwxrwx   0        0        0        0 2024-04-03 14:56:01.157930 yayy-0.1.1/
--rw-rw-rw-   0        0        0     1058 2023-12-28 09:22:07.000000 yayy-0.1.1/LICENSE
--rw-rw-rw-   0        0        0     1627 2024-04-03 14:56:01.157930 yayy-0.1.1/PKG-INFO
--rw-rw-rw-   0        0        0     1232 2024-04-03 14:55:36.000000 yayy-0.1.1/README.md
--rw-rw-rw-   0        0        0       42 2024-04-03 14:56:01.157930 yayy-0.1.1/setup.cfg
--rw-rw-rw-   0        0        0      867 2024-04-03 14:55:42.000000 yayy-0.1.1/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-03 14:56:01.117154 yayy-0.1.1/yayy/
--rw-rw-rw-   0        0        0       19 2024-03-23 13:35:28.000000 yayy-0.1.1/yayy/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-03 14:56:01.156487 yayy-0.1.1/yayy/assets/
--rw-rw-rw-   0        0        0       29 2024-03-25 17:52:46.000000 yayy-0.1.1/yayy/assets/data.json
--rw-rw-rw-   0        0        0      890 2024-04-03 14:32:19.000000 yayy-0.1.1/yayy/constants.py
--rw-rw-rw-   0        0        0     2552 2024-04-03 14:35:33.000000 yayy-0.1.1/yayy/main.py
--rw-rw-rw-   0        0        0     3019 2024-04-03 14:26:49.000000 yayy-0.1.1/yayy/utils.py
-drwxrwxrwx   0        0        0        0 2024-04-03 14:56:01.155447 yayy-0.1.1/yayy.egg-info/
--rw-rw-rw-   0        0        0     1627 2024-04-03 14:56:01.000000 yayy-0.1.1/yayy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      280 2024-04-03 14:56:01.000000 yayy-0.1.1/yayy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-03 14:56:01.000000 yayy-0.1.1/yayy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       39 2024-04-03 14:56:01.000000 yayy-0.1.1/yayy.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       40 2024-04-03 14:56:01.000000 yayy-0.1.1/yayy.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2024-04-03 14:56:01.000000 yayy-0.1.1/yayy.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-03 15:11:23.192826 yayy-0.1.3/
+-rw-rw-rw-   0        0        0     1589 2024-04-03 15:11:23.192826 yayy-0.1.3/PKG-INFO
+-rw-rw-rw-   0        0        0     1217 2024-04-03 15:06:38.000000 yayy-0.1.3/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-03 15:11:23.192826 yayy-0.1.3/setup.cfg
+-rw-rw-rw-   0        0        0      869 2024-04-03 15:11:13.000000 yayy-0.1.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-03 15:11:23.170227 yayy-0.1.3/yayy/
+-rw-rw-rw-   0        0        0       19 2024-03-23 13:35:28.000000 yayy-0.1.3/yayy/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-03 15:11:23.191295 yayy-0.1.3/yayy/assets/
+-rw-rw-rw-   0        0        0       22 2024-04-03 15:09:35.000000 yayy-0.1.3/yayy/assets/data.json
+-rw-rw-rw-   0        0        0      890 2024-04-03 15:07:09.000000 yayy-0.1.3/yayy/constants.py
+-rw-rw-rw-   0        0        0     2558 2024-04-03 15:07:20.000000 yayy-0.1.3/yayy/main.py
+-rw-rw-rw-   0        0        0     3019 2024-04-03 15:06:14.000000 yayy-0.1.3/yayy/utils.py
+drwxrwxrwx   0        0        0        0 2024-04-03 15:11:23.190256 yayy-0.1.3/yayy.egg-info/
+-rw-rw-rw-   0        0        0     1589 2024-04-03 15:11:23.000000 yayy-0.1.3/yayy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      272 2024-04-03 15:11:23.000000 yayy-0.1.3/yayy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-03 15:11:23.000000 yayy-0.1.3/yayy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       41 2024-04-03 15:11:23.000000 yayy-0.1.3/yayy.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       40 2024-04-03 15:11:23.000000 yayy-0.1.3/yayy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2024-04-03 15:11:23.000000 yayy-0.1.3/yayy.egg-info/top_level.txt
```

### Comparing `yayy-0.1.1/PKG-INFO` & `yayy-0.1.3/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 Metadata-Version: 2.1
 Name: yayy
-Version: 0.1.1
+Version: 0.1.3
 Summary: Si Un Problema Puede Solucionarse, Entonces No Vale La Pena Preocuparse Por El.
 Author: Pablo Escobar
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
-License-File: LICENSE
 
 # yayy
 
 ## Scripts
 
 These are batch files, save them in a .bat format.
 
@@ -44,24 +43,24 @@
 
 2. `run.bat`
 ```bat
 @echo off
 echo Running yayy...
 
 REM
-yay
+fkvit
 
 echo yayy execution completed.
 
 pause
 ```
+You may run the tool manually post installation by typing `fkvit` in your terminal.
 
 ## Note:
 - Get your gemini api key from [here](https://aistudio.google.com/app/apikey).
-- You may use the execution Type `yay` in the terminal to run the script directly from the terminal.
 - Copy da MCQ and paste it in the terminal by simply pressing enter key.
 - Wait for the answers to arrive.
 - Supported OS: Windows 11
 - To reset terminal opacity back to 100%, rerun the tool and kill the process by pressing `ctrl+c`.
 
 # Lastly
 ![image](https://github.com/arpy8/queky/assets/74809468/671d24e4-77a6-474b-a083-730b2874f15f)
```

### Comparing `yayy-0.1.1/README.md` & `yayy-0.1.3/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -32,24 +32,24 @@
 
 2. `run.bat`
 ```bat
 @echo off
 echo Running yayy...
 
 REM
-yay
+fkvit
 
 echo yayy execution completed.
 
 pause
 ```
+You may run the tool manually post installation by typing `fkvit` in your terminal.
 
 ## Note:
 - Get your gemini api key from [here](https://aistudio.google.com/app/apikey).
-- You may use the execution Type `yay` in the terminal to run the script directly from the terminal.
 - Copy da MCQ and paste it in the terminal by simply pressing enter key.
 - Wait for the answers to arrive.
 - Supported OS: Windows 11
 - To reset terminal opacity back to 100%, rerun the tool and kill the process by pressing `ctrl+c`.
 
 # Lastly
 ![image](https://github.com/arpy8/queky/assets/74809468/671d24e4-77a6-474b-a083-730b2874f15f)
```

### Comparing `yayy-0.1.1/setup.py` & `yayy-0.1.3/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as f:
     long_description = f.read()
 
 setup(
     name="yayy",
-    version="0.1.1",
+    version="0.1.3",
     author="Pablo Escobar",
     description="Si Un Problema Puede Solucionarse, Entonces No Vale La Pena Preocuparse Por El.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=find_packages(),
     install_requires=["pyperclip", "google-generativeai", "pyautogui"],
     entry_points={
         "console_scripts": [
-            "yay=yayy.main:main",
+            "fkvit=yayy.main:main",
         ],
     },
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
```

### Comparing `yayy-0.1.1/yayy/constants.py` & `yayy-0.1.3/yayy/constants.py`

 * *Files identical despite different names*

### Comparing `yayy-0.1.1/yayy/main.py` & `yayy-0.1.3/yayy/main.py`

 * *Files 3% similar despite different names*

```diff
@@ -28,15 +28,15 @@
                     
                 data["GOOGLE_API_KEY"] = api_key.strip()
                 
                 with open(JSON_FILE, "w") as file:
                     json.dump(data, file)
                     
                 print("API key saved successfully.")
-                subprocess.run(["qk"])
+                subprocess.run(["fkvit"])
                 
             else:
                 _ = modify_env(True)
 
                 while True:
                     user_input = input("\n<<< press enter to paste >>>\n")
                     print("\033[H\033[J")
@@ -66,12 +66,12 @@
             
     elif args.reset:
         with open(JSON_FILE, "r") as file: data = json.load(file)
         data["GOOGLE_API_KEY"] = ""
         with open(JSON_FILE, "w") as file: json.dump(data, file)
             
         print("API key reset successfully.")
-        subprocess.run(["qk"])
+        subprocess.run(["fkvit"])
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `yayy-0.1.1/yayy/utils.py` & `yayy-0.1.3/yayy/utils.py`

 * *Files identical despite different names*

### Comparing `yayy-0.1.1/yayy.egg-info/PKG-INFO` & `yayy-0.1.3/yayy.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 Metadata-Version: 2.1
 Name: yayy
-Version: 0.1.1
+Version: 0.1.3
 Summary: Si Un Problema Puede Solucionarse, Entonces No Vale La Pena Preocuparse Por El.
 Author: Pablo Escobar
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
-License-File: LICENSE
 
 # yayy
 
 ## Scripts
 
 These are batch files, save them in a .bat format.
 
@@ -44,24 +43,24 @@
 
 2. `run.bat`
 ```bat
 @echo off
 echo Running yayy...
 
 REM
-yay
+fkvit
 
 echo yayy execution completed.
 
 pause
 ```
+You may run the tool manually post installation by typing `fkvit` in your terminal.
 
 ## Note:
 - Get your gemini api key from [here](https://aistudio.google.com/app/apikey).
-- You may use the execution Type `yay` in the terminal to run the script directly from the terminal.
 - Copy da MCQ and paste it in the terminal by simply pressing enter key.
 - Wait for the answers to arrive.
 - Supported OS: Windows 11
 - To reset terminal opacity back to 100%, rerun the tool and kill the process by pressing `ctrl+c`.
 
 # Lastly
 ![image](https://github.com/arpy8/queky/assets/74809468/671d24e4-77a6-474b-a083-730b2874f15f)
```

