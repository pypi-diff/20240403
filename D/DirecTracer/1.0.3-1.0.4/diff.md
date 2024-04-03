# Comparing `tmp/DirecTracer-1.0.3.tar.gz` & `tmp/DirecTracer-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "DirecTracer-1.0.3.tar", last modified: Sat Feb 17 13:16:40 2024, max compression
+gzip compressed data, was "DirecTracer-1.0.4.tar", last modified: Wed Apr  3 13:50:30 2024, max compression
```

## Comparing `DirecTracer-1.0.3.tar` & `DirecTracer-1.0.4.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2024-02-17 13:16:40.357302 DirecTracer-1.0.3/
--rw-rw-rw-   0        0        0     1085 2024-02-16 10:31:49.000000 DirecTracer-1.0.3/LICENSE.txt
--rw-rw-rw-   0        0        0     2695 2024-02-17 13:16:40.356301 DirecTracer-1.0.3/PKG-INFO
--rw-rw-rw-   0        0        0     2956 2024-02-17 13:16:31.000000 DirecTracer-1.0.3/README.md
-drwxrwxrwx   0        0        0        0 2024-02-17 13:16:40.341302 DirecTracer-1.0.3/app/
-drwxrwxrwx   0        0        0        0 2024-02-17 13:16:40.347302 DirecTracer-1.0.3/app/DirecTracer/
--rw-rw-rw-   0        0        0       56 2024-02-16 10:31:00.000000 DirecTracer-1.0.3/app/DirecTracer/__init__.py
-drwxrwxrwx   0        0        0        0 2024-02-17 13:16:40.353301 DirecTracer-1.0.3/app/DirecTracer/src/
--rw-rw-rw-   0        0        0     5531 2024-02-17 13:09:48.000000 DirecTracer-1.0.3/app/DirecTracer/src/DirectTracer.py
--rw-rw-rw-   0        0        0        0 2024-02-16 10:27:37.000000 DirecTracer-1.0.3/app/DirecTracer/src/__init__.py
-drwxrwxrwx   0        0        0        0 2024-02-17 13:16:40.355302 DirecTracer-1.0.3/app/DirecTracer/test/
--rw-rw-rw-   0        0        0        0 2024-02-16 10:27:37.000000 DirecTracer-1.0.3/app/DirecTracer/test/__init__.py
--rw-rw-rw-   0        0        0      908 2024-02-16 10:44:24.000000 DirecTracer-1.0.3/app/DirecTracer/test/generate_sample_structure.py
--rw-rw-rw-   0        0        0     1005 2024-02-16 11:48:04.000000 DirecTracer-1.0.3/app/DirecTracer/test/test_DirecTracer.py
-drwxrwxrwx   0        0        0        0 2024-02-17 13:16:40.351305 DirecTracer-1.0.3/app/DirecTracer.egg-info/
--rw-rw-rw-   0        0        0     2695 2024-02-17 13:16:40.000000 DirecTracer-1.0.3/app/DirecTracer.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      406 2024-02-17 13:16:40.000000 DirecTracer-1.0.3/app/DirecTracer.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-02-17 13:16:40.000000 DirecTracer-1.0.3/app/DirecTracer.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2024-02-17 13:16:40.000000 DirecTracer-1.0.3/app/DirecTracer.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-02-17 13:16:40.357302 DirecTracer-1.0.3/setup.cfg
--rw-rw-rw-   0        0        0     1048 2024-02-17 13:16:17.000000 DirecTracer-1.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-03 13:50:30.587767 DirecTracer-1.0.4/
+-rw-rw-rw-   0        0        0     1085 2024-02-16 10:31:49.000000 DirecTracer-1.0.4/LICENSE.txt
+-rw-rw-rw-   0        0        0     3923 2024-04-03 13:50:30.586771 DirecTracer-1.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0     3734 2024-04-03 13:48:34.000000 DirecTracer-1.0.4/README.md
+drwxrwxrwx   0        0        0        0 2024-04-03 13:50:30.574746 DirecTracer-1.0.4/app/
+drwxrwxrwx   0        0        0        0 2024-04-03 13:50:30.578746 DirecTracer-1.0.4/app/DirecTracer/
+-rw-rw-rw-   0        0        0       56 2024-02-16 10:31:00.000000 DirecTracer-1.0.4/app/DirecTracer/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-03 13:50:30.583767 DirecTracer-1.0.4/app/DirecTracer/src/
+-rw-rw-rw-   0        0        0     9485 2024-04-03 13:45:28.000000 DirecTracer-1.0.4/app/DirecTracer/src/DirectTracer.py
+-rw-rw-rw-   0        0        0        0 2024-02-16 10:27:37.000000 DirecTracer-1.0.4/app/DirecTracer/src/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-03 13:50:30.585771 DirecTracer-1.0.4/app/DirecTracer/test/
+-rw-rw-rw-   0        0        0        0 2024-02-16 10:27:37.000000 DirecTracer-1.0.4/app/DirecTracer/test/__init__.py
+-rw-rw-rw-   0        0        0      908 2024-02-16 10:44:24.000000 DirecTracer-1.0.4/app/DirecTracer/test/generate_sample_structure.py
+-rw-rw-rw-   0        0        0     1005 2024-02-16 11:48:04.000000 DirecTracer-1.0.4/app/DirecTracer/test/test_DirecTracer.py
+drwxrwxrwx   0        0        0        0 2024-04-03 13:50:30.582246 DirecTracer-1.0.4/app/DirecTracer.egg-info/
+-rw-rw-rw-   0        0        0     3923 2024-04-03 13:50:30.000000 DirecTracer-1.0.4/app/DirecTracer.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      406 2024-04-03 13:50:30.000000 DirecTracer-1.0.4/app/DirecTracer.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-03 13:50:30.000000 DirecTracer-1.0.4/app/DirecTracer.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       12 2024-04-03 13:50:30.000000 DirecTracer-1.0.4/app/DirecTracer.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-03 13:50:30.587767 DirecTracer-1.0.4/setup.cfg
+-rw-rw-rw-   0        0        0     1048 2024-04-03 13:26:14.000000 DirecTracer-1.0.4/setup.py
```

### Comparing `DirecTracer-1.0.3/LICENSE.txt` & `DirecTracer-1.0.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `DirecTracer-1.0.3/PKG-INFO` & `DirecTracer-1.0.4/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: DirecTracer
-Version: 1.0.3
+Version: 1.0.4
 Summary: DirecTracer is a Python script that generates a directory structure in both text and Markdown formats. It can be used to visualize the hierarchy of folders and files in a given directory, while also excluding specific folders and file extensions.
 Home-page: https://github.com/Hardvan/DirecTracer
 Author: Hardik Pawar
 Author-email: hardikpawarh@gmail.com
 License: UNKNOWN
 Keywords: directory structure,visualization,folder hierarchy,file organization
 Platform: UNKNOWN
@@ -15,19 +15,37 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 # DirecTracer
 
 DirecTracer is a Python script that generates a directory structure in both text and Markdown formats. It can be used to visualize the hierarchy of folders and files in a given directory, while also excluding specific folders and file extensions.
 
+## DirecTracer on PyPI
+
+View the DirecTracer package on PyPI by clicking [here](https://pypi.org/project/DirecTracer/).
+
 ## Features
 
-- Generates a directory structure in text and Markdown formats.
-- Supports ignoring specific directories and file extensions.
-- Outputs clickable links in the Markdown file for easy navigation.
+- `save_directory_structure()` function:
+
+  - Generates a directory structure in text and Markdown formats.
+  - Supports ignoring specific directories and file extensions.
+  - Outputs clickable links in the Markdown file for easy navigation.
+  - Text & loading animations while generating the directory structure.
+
+- `generate_markdown_table()` function:
+
+  - Generates a Markdown table from the given directory structure.
+  - Includes columns of Serial Number and clickable links to the files through the file names.
+
+## Demonstration Video
+
+Click on the thumbnail below to watch the demonstration video on YouTube.
+
+[![DirecTracer](./demo/thumbnail2.png)](https://youtu.be/FqMauKiTvVs?si=FJlBiQBwpZb7_IPm)
 
 ## Usage
 
 Install the DirecTracer package using the following command:
 
 ```bash
 pip install DirecTracer
@@ -55,19 +73,26 @@
    root_dir=os.getcwd(),
    text_output_file="directory_structure.txt",
    markdown_output_file="directory_structure.md",
    animation=True
 )
 ```
 
-The function accepts the following parameters:
+View the [`run.py`](./run.py) file for a complete example.
+
+The `save_directory_structure()` function accepts the following parameters:
 
 - **root_dir (str):** The root directory to start scanning from. Defaults to the current working directory.
 - **text_output_file (str):** The name of the text output file. Defaults to "directory_structure.txt".
 - **markdown_output_file (str):** The name of the Markdown output file. Defaults to "directory_structure.md".
 - **ignored_directories (list, optional):** List of directories to ignore. Defaults to [".git", ".vscode", "venv", ".venv", ".idea", "out"].
 - **ignored_extensions (list, optional):** List of file extensions to ignore. Defaults to [".exe"].
 - **animation (bool, optional):** Enable/Disable the loading animation. Defaults to False.
 
+The `generate_markdown_table()` function accepts the following parameters:
 
+- **root_dir (str)**: The root directory to start scanning from. Defaults to the current working directory.
+- **markdown_output_file (str)**: The name of the Markdown output file. Defaults to "markdown_table.md".
+- **animation (bool, optional)**: Enable/Disable the loading animation. Defaults to False.
+- **ignored_extensions (list, optional)**: List of file extensions to ignore. Defaults to [".exe"].
```

### Comparing `DirecTracer-1.0.3/app/DirecTracer/test/generate_sample_structure.py` & `DirecTracer-1.0.4/app/DirecTracer/test/generate_sample_structure.py`

 * *Files identical despite different names*

### Comparing `DirecTracer-1.0.3/app/DirecTracer/test/test_DirecTracer.py` & `DirecTracer-1.0.4/app/DirecTracer/test/test_DirecTracer.py`

 * *Files identical despite different names*

### Comparing `DirecTracer-1.0.3/app/DirecTracer.egg-info/PKG-INFO` & `DirecTracer-1.0.4/app/DirecTracer.egg-info/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: DirecTracer
-Version: 1.0.3
+Version: 1.0.4
 Summary: DirecTracer is a Python script that generates a directory structure in both text and Markdown formats. It can be used to visualize the hierarchy of folders and files in a given directory, while also excluding specific folders and file extensions.
 Home-page: https://github.com/Hardvan/DirecTracer
 Author: Hardik Pawar
 Author-email: hardikpawarh@gmail.com
 License: UNKNOWN
 Keywords: directory structure,visualization,folder hierarchy,file organization
 Platform: UNKNOWN
@@ -15,19 +15,37 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 # DirecTracer
 
 DirecTracer is a Python script that generates a directory structure in both text and Markdown formats. It can be used to visualize the hierarchy of folders and files in a given directory, while also excluding specific folders and file extensions.
 
+## DirecTracer on PyPI
+
+View the DirecTracer package on PyPI by clicking [here](https://pypi.org/project/DirecTracer/).
+
 ## Features
 
-- Generates a directory structure in text and Markdown formats.
-- Supports ignoring specific directories and file extensions.
-- Outputs clickable links in the Markdown file for easy navigation.
+- `save_directory_structure()` function:
+
+  - Generates a directory structure in text and Markdown formats.
+  - Supports ignoring specific directories and file extensions.
+  - Outputs clickable links in the Markdown file for easy navigation.
+  - Text & loading animations while generating the directory structure.
+
+- `generate_markdown_table()` function:
+
+  - Generates a Markdown table from the given directory structure.
+  - Includes columns of Serial Number and clickable links to the files through the file names.
+
+## Demonstration Video
+
+Click on the thumbnail below to watch the demonstration video on YouTube.
+
+[![DirecTracer](./demo/thumbnail2.png)](https://youtu.be/FqMauKiTvVs?si=FJlBiQBwpZb7_IPm)
 
 ## Usage
 
 Install the DirecTracer package using the following command:
 
 ```bash
 pip install DirecTracer
@@ -55,19 +73,26 @@
    root_dir=os.getcwd(),
    text_output_file="directory_structure.txt",
    markdown_output_file="directory_structure.md",
    animation=True
 )
 ```
 
-The function accepts the following parameters:
+View the [`run.py`](./run.py) file for a complete example.
+
+The `save_directory_structure()` function accepts the following parameters:
 
 - **root_dir (str):** The root directory to start scanning from. Defaults to the current working directory.
 - **text_output_file (str):** The name of the text output file. Defaults to "directory_structure.txt".
 - **markdown_output_file (str):** The name of the Markdown output file. Defaults to "directory_structure.md".
 - **ignored_directories (list, optional):** List of directories to ignore. Defaults to [".git", ".vscode", "venv", ".venv", ".idea", "out"].
 - **ignored_extensions (list, optional):** List of file extensions to ignore. Defaults to [".exe"].
 - **animation (bool, optional):** Enable/Disable the loading animation. Defaults to False.
 
+The `generate_markdown_table()` function accepts the following parameters:
 
+- **root_dir (str)**: The root directory to start scanning from. Defaults to the current working directory.
+- **markdown_output_file (str)**: The name of the Markdown output file. Defaults to "markdown_table.md".
+- **animation (bool, optional)**: Enable/Disable the loading animation. Defaults to False.
+- **ignored_extensions (list, optional)**: List of file extensions to ignore. Defaults to [".exe"].
```

### Comparing `DirecTracer-1.0.3/setup.py` & `DirecTracer-1.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("app/README.md", "r") as f:
     long_description = f.read()
 
 setup(
     name="DirecTracer",
-    version="1.0.3",
+    version="1.0.4",
     author="Hardik Pawar",
     author_email="hardikpawarh@gmail.com",
     description="DirecTracer is a Python script that generates a directory structure in both text and Markdown formats. It can be used to visualize the hierarchy of folders and files in a given directory, while also excluding specific folders and file extensions.",
     package_dir={"": "app"},
     packages=find_packages(where="app"),
     long_description=long_description,
     long_description_content_type="text/markdown",
```

