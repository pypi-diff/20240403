# Comparing `tmp/guia_cli-0.0.6.tar.gz` & `tmp/guia_cli-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "guia_cli-0.0.6.tar", last modified: Wed Apr  3 20:34:01 2024, max compression
+gzip compressed data, was "guia_cli-0.0.7.tar", last modified: Wed Apr  3 20:47:04 2024, max compression
```

## Comparing `guia_cli-0.0.6.tar` & `guia_cli-0.0.7.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 20:34:01.363012 guia_cli-0.0.6/
--rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-04-03 20:33:30.000000 guia_cli-0.0.6/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)     6059 2024-04-03 20:34:01.363012 guia_cli-0.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2626 2024-04-03 20:33:30.000000 guia_cli-0.0.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 20:34:01.363012 guia_cli-0.0.6/guia_cli.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6059 2024-04-03 20:34:01.000000 guia_cli-0.0.6/guia_cli.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      238 2024-04-03 20:34:01.000000 guia_cli-0.0.6/guia_cli.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 20:34:01.000000 guia_cli-0.0.6/guia_cli.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       95 2024-04-03 20:34:01.000000 guia_cli-0.0.6/guia_cli.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1553 2024-04-03 20:34:01.000000 guia_cli-0.0.6/guia_cli.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 20:34:01.000000 guia_cli-0.0.6/guia_cli.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       81 2024-04-03 20:33:30.000000 guia_cli-0.0.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-03 20:34:01.363012 guia_cli-0.0.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1681 2024-04-03 20:33:30.000000 guia_cli-0.0.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 20:47:04.837173 guia_cli-0.0.7/
+-rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-04-03 20:46:32.000000 guia_cli-0.0.7/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3440 2024-04-03 20:47:04.837173 guia_cli-0.0.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2626 2024-04-03 20:46:32.000000 guia_cli-0.0.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 20:47:04.837173 guia_cli-0.0.7/guia_cli.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3440 2024-04-03 20:47:04.000000 guia_cli-0.0.7/guia_cli.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      238 2024-04-03 20:47:04.000000 guia_cli-0.0.7/guia_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 20:47:04.000000 guia_cli-0.0.7/guia_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       95 2024-04-03 20:47:04.000000 guia_cli-0.0.7/guia_cli.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-04-03 20:47:04.000000 guia_cli-0.0.7/guia_cli.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 20:47:04.000000 guia_cli-0.0.7/guia_cli.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-04-03 20:46:32.000000 guia_cli-0.0.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-03 20:47:04.837173 guia_cli-0.0.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1700 2024-04-03 20:46:32.000000 guia_cli-0.0.7/setup.py
```

### Comparing `guia_cli-0.0.6/LICENSE.md` & `guia_cli-0.0.7/LICENSE.md`

 * *Files identical despite different names*

### Comparing `guia_cli-0.0.6/README.md` & `guia_cli-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `guia_cli-0.0.6/setup.py` & `guia_cli-0.0.7/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,16 +6,15 @@
     setuppy_dir = os.path.dirname(os.path.abspath(__file__))
     absolute_path_relative_to_setuppy = os.path.join(setuppy_dir, filepath)
     with open(absolute_path_relative_to_setuppy) as f:
         file_content = f.read()
     return file_content
 
 
-__VERSION__ = "0.0.6"
-REQUIREMENTS_LIST = read_file("requirements.txt").splitlines()
+__VERSION__ = "0.0.7"
 README_TEXT = read_file("README.md")
 
 
 # https://packaging.python.org/en/latest/key_projects/#setuptools
 setup(
     name="guia_cli",
     version=__VERSION__,
@@ -35,15 +34,19 @@
         "Intended Audience :: End Users/Desktop",
         "Operating System :: OS Independent",
         "Programming Language :: Python",
         "Topic :: Scientific/Engineering :: Artificial Intelligence",
     ],
     packages=find_packages(),
     include_package_data=True,
-    install_requires=REQUIREMENTS_LIST,
+    install_requires=[
+        "crewai>=0.19.0",
+        "langchain_google_genai",
+        "python-dotenv>=1.0.1",
+    ],
     entry_points={
         "console_scripts": [
             "gu = guia_cli.main:main",
             "guia = guia_cli.main:main",
             "gucli = guia_cli.main:main",
         ],
     },
```

