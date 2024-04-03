# Comparing `tmp/tinta-0.1.7b2.tar.gz` & `tmp/tinta-0.1.7b3.tar.gz`

## Comparing `tinta-0.1.7b2.tar` & `tinta-0.1.7b3.tar`

### file list

```diff
@@ -1,44 +1,43 @@
--rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 tinta-0.1.7b2/.gitattributes
--rw-r--r--   0        0        0      145 2020-02-02 00:00:00.000000 tinta-0.1.7b2/.pylintrc
--rw-r--r--   0        0        0     3353 2020-02-02 00:00:00.000000 tinta-0.1.7b2/CODE_OF_CONDUCT.md
--rw-r--r--   0        0        0      245 2020-02-02 00:00:00.000000 tinta-0.1.7b2/DESCRIPTION.rst
--rw-r--r--   0        0        0     8392 2020-02-02 00:00:00.000000 tinta-0.1.7b2/HIPPOCRATIC_LICENSE.md
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 tinta-0.1.7b2/MANIFEST.in
--rw-r--r--   0        0        0      530 2020-02-02 00:00:00.000000 tinta-0.1.7b2/Pipfile
--rw-r--r--   0        0        0    45957 2020-02-02 00:00:00.000000 tinta-0.1.7b2/Pipfile.lock
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tinta-0.1.7b2/__init__.py
--rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 tinta-0.1.7b2/requirements-dev.txt
--rw-r--r--   0        0        0       10 2020-02-02 00:00:00.000000 tinta-0.1.7b2/requirements.txt
--rw-r--r--   0        0        0     2180 2020-02-02 00:00:00.000000 tinta-0.1.7b2/setup.py
--rw-r--r--   0        0        0     1355 2020-02-02 00:00:00.000000 tinta-0.1.7b2/.github/workflows/publish-test.yml
--rw-r--r--   0        0        0     1322 2020-02-02 00:00:00.000000 tinta-0.1.7b2/.github/workflows/publish.yml
--rw-r--r--   0        0        0     1474 2020-02-02 00:00:00.000000 tinta-0.1.7b2/.github/workflows/run-tests.yml
--rw-r--r--   0        0        0     1126 2020-02-02 00:00:00.000000 tinta-0.1.7b2/.vscode/launch.json
--rw-r--r--   0        0        0     2651 2020-02-02 00:00:00.000000 tinta-0.1.7b2/.vscode/settings.json
--rw-r--r--   0        0        0     5355 2020-02-02 00:00:00.000000 tinta-0.1.7b2/.vscode/tasks.json
--rw-r--r--   0        0        0     4696 2020-02-02 00:00:00.000000 tinta-0.1.7b2/examples/basic_example.py
--rw-r--r--   0        0        0      362 2020-02-02 00:00:00.000000 tinta-0.1.7b2/examples/colors.ini
--rw-r--r--   0        0        0     3106 2020-02-02 00:00:00.000000 tinta-0.1.7b2/examples/complete_example.py
--rw-r--r--   0        0        0   190743 2020-02-02 00:00:00.000000 tinta-0.1.7b2/examples/tinta-discover.png
--rw-r--r--   0        0        0     3056 2020-02-02 00:00:00.000000 tinta-0.1.7b2/junit/test-results.xml
--rw-r--r--   0        0        0     1149 2020-02-02 00:00:00.000000 tinta-0.1.7b2/tests/conftest.py
--rw-r--r--   0        0        0      585 2020-02-02 00:00:00.000000 tinta-0.1.7b2/tests/launch.json
--rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 tinta-0.1.7b2/tests/test_colors_invalid.ini
--rw-r--r--   0        0        0     1093 2020-02-02 00:00:00.000000 tinta-0.1.7b2/tests/test_discover.py
--rw-r--r--   0        0        0    16103 2020-02-02 00:00:00.000000 tinta-0.1.7b2/tests/test_tinta.py
--rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 tinta-0.1.7b2/tinta/__init__.py
--rw-r--r--   0        0        0      864 2020-02-02 00:00:00.000000 tinta-0.1.7b2/tinta/__main__.py
--rw-r--r--   0        0        0     4160 2020-02-02 00:00:00.000000 tinta-0.1.7b2/tinta/ansi.py
--rw-r--r--   0        0        0     6999 2020-02-02 00:00:00.000000 tinta-0.1.7b2/tinta/colorize.py
--rw-r--r--   0        0        0      329 2020-02-02 00:00:00.000000 tinta-0.1.7b2/tinta/colors.ini
--rw-r--r--   0        0        0     1877 2020-02-02 00:00:00.000000 tinta-0.1.7b2/tinta/constants.py
--rw-r--r--   0        0        0     7327 2020-02-02 00:00:00.000000 tinta-0.1.7b2/tinta/discover.py
--rw-r--r--   0        0        0      753 2020-02-02 00:00:00.000000 tinta-0.1.7b2/tinta/multi_version_imports.py
--rw-r--r--   0        0        0    25079 2020-02-02 00:00:00.000000 tinta-0.1.7b2/tinta/tinta.py
--rw-r--r--   0        0        0     2420 2020-02-02 00:00:00.000000 tinta-0.1.7b2/tinta/typ.py
--rw-r--r--   0        0        0      470 2020-02-02 00:00:00.000000 tinta-0.1.7b2/tinta/utils.py
--rw-r--r--   0        0        0     1334 2020-02-02 00:00:00.000000 tinta-0.1.7b2/.gitignore
--rw-r--r--   0        0        0     1081 2020-02-02 00:00:00.000000 tinta-0.1.7b2/LICENSE
--rw-r--r--   0        0        0    13520 2020-02-02 00:00:00.000000 tinta-0.1.7b2/README.md
--rw-r--r--   0        0        0     4112 2020-02-02 00:00:00.000000 tinta-0.1.7b2/pyproject.toml
--rw-r--r--   0        0        0    14576 2020-02-02 00:00:00.000000 tinta-0.1.7b2/PKG-INFO
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 tinta-0.1.7b3/.gitattributes
+-rw-r--r--   0        0        0      145 2020-02-02 00:00:00.000000 tinta-0.1.7b3/.pylintrc
+-rw-r--r--   0        0        0     3353 2020-02-02 00:00:00.000000 tinta-0.1.7b3/CODE_OF_CONDUCT.md
+-rw-r--r--   0        0        0      245 2020-02-02 00:00:00.000000 tinta-0.1.7b3/DESCRIPTION.rst
+-rw-r--r--   0        0        0     8392 2020-02-02 00:00:00.000000 tinta-0.1.7b3/HIPPOCRATIC_LICENSE.md
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 tinta-0.1.7b3/MANIFEST.in
+-rw-r--r--   0        0        0      530 2020-02-02 00:00:00.000000 tinta-0.1.7b3/Pipfile
+-rw-r--r--   0        0        0    45957 2020-02-02 00:00:00.000000 tinta-0.1.7b3/Pipfile.lock
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tinta-0.1.7b3/__init__.py
+-rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 tinta-0.1.7b3/requirements-dev.txt
+-rw-r--r--   0        0        0       10 2020-02-02 00:00:00.000000 tinta-0.1.7b3/requirements.txt
+-rw-r--r--   0        0        0     2180 2020-02-02 00:00:00.000000 tinta-0.1.7b3/setup.py
+-rw-r--r--   0        0        0     1355 2020-02-02 00:00:00.000000 tinta-0.1.7b3/.github/workflows/publish-test.yml
+-rw-r--r--   0        0        0     1322 2020-02-02 00:00:00.000000 tinta-0.1.7b3/.github/workflows/publish.yml
+-rw-r--r--   0        0        0     1474 2020-02-02 00:00:00.000000 tinta-0.1.7b3/.github/workflows/run-tests.yml
+-rw-r--r--   0        0        0     1310 2020-02-02 00:00:00.000000 tinta-0.1.7b3/.vscode/launch.json
+-rw-r--r--   0        0        0     2586 2020-02-02 00:00:00.000000 tinta-0.1.7b3/.vscode/settings.json
+-rw-r--r--   0        0        0     5355 2020-02-02 00:00:00.000000 tinta-0.1.7b3/.vscode/tasks.json
+-rw-r--r--   0        0        0     5612 2020-02-02 00:00:00.000000 tinta-0.1.7b3/examples/basic_example.py
+-rw-r--r--   0        0        0      362 2020-02-02 00:00:00.000000 tinta-0.1.7b3/examples/colors.ini
+-rw-r--r--   0        0        0     4678 2020-02-02 00:00:00.000000 tinta-0.1.7b3/examples/complete_example.py
+-rw-r--r--   0        0        0   190743 2020-02-02 00:00:00.000000 tinta-0.1.7b3/examples/tinta-discover.png
+-rw-r--r--   0        0        0     3056 2020-02-02 00:00:00.000000 tinta-0.1.7b3/junit/test-results.xml
+-rw-r--r--   0        0        0     1149 2020-02-02 00:00:00.000000 tinta-0.1.7b3/tests/conftest.py
+-rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 tinta-0.1.7b3/tests/test_colors_invalid.ini
+-rw-r--r--   0        0        0     1093 2020-02-02 00:00:00.000000 tinta-0.1.7b3/tests/test_discover.py
+-rw-r--r--   0        0        0    24079 2020-02-02 00:00:00.000000 tinta-0.1.7b3/tests/test_tinta.py
+-rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 tinta-0.1.7b3/tinta/__init__.py
+-rw-r--r--   0        0        0      864 2020-02-02 00:00:00.000000 tinta-0.1.7b3/tinta/__main__.py
+-rw-r--r--   0        0        0     4856 2020-02-02 00:00:00.000000 tinta-0.1.7b3/tinta/ansi.py
+-rw-r--r--   0        0        0     7263 2020-02-02 00:00:00.000000 tinta-0.1.7b3/tinta/colorize.py
+-rw-r--r--   0        0        0      329 2020-02-02 00:00:00.000000 tinta-0.1.7b3/tinta/colors.ini
+-rw-r--r--   0        0        0     1931 2020-02-02 00:00:00.000000 tinta-0.1.7b3/tinta/constants.py
+-rw-r--r--   0        0        0     7327 2020-02-02 00:00:00.000000 tinta-0.1.7b3/tinta/discover.py
+-rw-r--r--   0        0        0      753 2020-02-02 00:00:00.000000 tinta-0.1.7b3/tinta/multi_version_imports.py
+-rw-r--r--   0        0        0    25608 2020-02-02 00:00:00.000000 tinta-0.1.7b3/tinta/tinta.py
+-rw-r--r--   0        0        0     2420 2020-02-02 00:00:00.000000 tinta-0.1.7b3/tinta/typ.py
+-rw-r--r--   0        0        0      470 2020-02-02 00:00:00.000000 tinta-0.1.7b3/tinta/utils.py
+-rw-r--r--   0        0        0     1334 2020-02-02 00:00:00.000000 tinta-0.1.7b3/.gitignore
+-rw-r--r--   0        0        0     1081 2020-02-02 00:00:00.000000 tinta-0.1.7b3/LICENSE
+-rw-r--r--   0        0        0    13520 2020-02-02 00:00:00.000000 tinta-0.1.7b3/README.md
+-rw-r--r--   0        0        0     4124 2020-02-02 00:00:00.000000 tinta-0.1.7b3/pyproject.toml
+-rw-r--r--   0        0        0    14576 2020-02-02 00:00:00.000000 tinta-0.1.7b3/PKG-INFO
```

### Comparing `tinta-0.1.7b2/CODE_OF_CONDUCT.md` & `tinta-0.1.7b3/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `tinta-0.1.7b2/HIPPOCRATIC_LICENSE.md` & `tinta-0.1.7b3/HIPPOCRATIC_LICENSE.md`

 * *Files identical despite different names*

### Comparing `tinta-0.1.7b2/Pipfile` & `tinta-0.1.7b3/Pipfile`

 * *Files identical despite different names*

### Comparing `tinta-0.1.7b2/Pipfile.lock` & `tinta-0.1.7b3/Pipfile.lock`

 * *Files identical despite different names*

### Comparing `tinta-0.1.7b2/setup.py` & `tinta-0.1.7b3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 from setuptools import setup
 
 with Path("README.md").open(encoding="utf-8") as f:
     long_description = f.read()
 
 setup(
     name="tinta",
-    version="0.1.7b2",
+    version="0.1.7b3",
     description="Tinta, a magical console output tool.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="http://github.com/brandonscript/tinta",
     author="Brandon Shelley",
     author_email="brandon@pacificaviator.co",
     install_requires=[],
```

### Comparing `tinta-0.1.7b2/.github/workflows/publish-test.yml` & `tinta-0.1.7b3/.github/workflows/publish-test.yml`

 * *Files identical despite different names*

### Comparing `tinta-0.1.7b2/.github/workflows/publish.yml` & `tinta-0.1.7b3/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `tinta-0.1.7b2/.github/workflows/run-tests.yml` & `tinta-0.1.7b3/.github/workflows/run-tests.yml`

 * *Files identical despite different names*

### Comparing `tinta-0.1.7b2/.vscode/launch.json` & `tinta-0.1.7b3/.vscode/launch.json`

 * *Files 16% similar despite different names*

```diff
@@ -2,42 +2,48 @@
   // Use IntelliSense to learn about possible attributes.
   // Hover to view descriptions of existing attributes.
   // For more information, visit: https://go.microsoft.com/fwlink/?linkid=830387
   "version": "0.2.0",
   "configurations": [
     {
       "name": "Basic examples",
-      "type": "python",
+      "type": "debugpy",
       "request": "launch",
       "program": "examples/basic_example.py",
       "cwd": "${workspaceFolder}",
       "console": "integratedTerminal",
       "env": {
         // "PYTHONPATH": "${workspaceFolder}/tinta"
       },
       "justMyCode": true
     },
     {
       "name": "Complete example set",
-      "type": "python",
+      "type": "debugpy",
       "request": "launch",
       "program": "examples/complete_example.py",
       "cwd": "${workspaceFolder}",
       "console": "integratedTerminal",
       "env": {
         // "PYTHONPATH": "${workspaceFolder}/tinta"
       },
       "justMyCode": true
     },
     {
-      "name": "Run Tinta tests",
-      "type": "python",
+      "name": "Run Tinta tests (workspace python)",
+      "type": "debugpy",
       "request": "launch",
       "console": "integratedTerminal",
       "module": "pytest",
       "env": {
         "_PYTEST_RAISE": "1"
       },
       "args": ["-xv"]
+    },
+    {
+      "name": "Run Tinta tests (all versions)",
+      "type": "debugpy",
+      "preLaunchTask": "Run All Pytest Versions",
+      "request": "launch"
     }
   ]
 }
```

### Comparing `tinta-0.1.7b2/.vscode/settings.json` & `tinta-0.1.7b3/.vscode/settings.json`

 * *Files 8% similar despite different names*

```diff
@@ -57,110 +57,106 @@
 00000380: 0a20 2020 2022 7469 746c 6542 6172 2e69  .    "titleBar.i
 00000390: 6e61 6374 6976 6546 6f72 6567 726f 756e  nactiveForegroun
 000003a0: 6422 3a20 2223 3135 3230 3262 3939 222c  d": "#15202b99",
 000003b0: 0a20 2020 2022 636f 6d6d 616e 6443 656e  .    "commandCen
 000003c0: 7465 722e 626f 7264 6572 223a 2022 2331  ter.border": "#1
 000003d0: 3532 3032 6239 3922 0a20 207d 2c0a 2020  5202b99".  },.  
 000003e0: 2270 6561 636f 636b 2e63 6f6c 6f72 223a  "peacock.color":
-000003f0: 2022 2336 3164 6166 6222 2c0a 2020 2f2f   "#61dafb",.  //
-00000400: 2022 7079 7468 6f6e 2e74 6573 7469 6e67   "python.testing
-00000410: 2e70 7974 6573 7441 7267 7322 3a20 5b22  .pytestArgs": ["
-00000420: 2d72 5020 2d76 7620 2d2d 636f 6c6f 723d  -rP -vv --color=
-00000430: 7965 7320 7465 7374 7322 5d2c 0a20 2022  yes tests"],.  "
-00000440: 7079 7468 6f6e 2e74 6573 7469 6e67 2e75  python.testing.u
-00000450: 6e69 7474 6573 7445 6e61 626c 6564 223a  nittestEnabled":
-00000460: 2066 616c 7365 2c0a 2020 2270 7974 686f   false,.  "pytho
-00000470: 6e2e 7465 7374 696e 672e 7079 7465 7374  n.testing.pytest
-00000480: 456e 6162 6c65 6422 3a20 7472 7565 2c0a  Enabled": true,.
-00000490: 2020 2270 7974 686f 6e2e 7465 7374 696e    "python.testin
-000004a0: 672e 6377 6422 3a20 2224 7b77 6f72 6b73  g.cwd": "${works
-000004b0: 7061 6365 466f 6c64 6572 7d22 2c0a 2020  paceFolder}",.  
-000004c0: 2270 7974 686f 6e2e 7465 726d 696e 616c  "python.terminal
-000004d0: 2e61 6374 6976 6174 6545 6e76 6972 6f6e  .activateEnviron
-000004e0: 6d65 6e74 223a 2074 7275 652c 0a20 2022  ment": true,.  "
-000004f0: 7079 7468 6f6e 2e74 6572 6d69 6e61 6c2e  python.terminal.
-00000500: 6163 7469 7661 7465 456e 7649 6e43 7572  activateEnvInCur
-00000510: 7265 6e74 5465 726d 696e 616c 223a 2074  rentTerminal": t
-00000520: 7275 652c 0a20 2022 7079 7468 6f6e 2e74  rue,.  "python.t
-00000530: 6573 7469 6e67 2e61 7574 6f54 6573 7444  esting.autoTestD
-00000540: 6973 636f 7665 724f 6e53 6176 6545 6e61  iscoverOnSaveEna
-00000550: 626c 6564 223a 2074 7275 652c 0a20 2022  bled": true,.  "
-00000560: 7079 7468 6f6e 2e61 6e61 6c79 7369 732e  python.analysis.
-00000570: 6578 7472 6150 6174 6873 223a 205b 2224  extraPaths": ["$
-00000580: 7b77 6f72 6b73 7061 6365 466f 6c64 6572  {workspaceFolder
-00000590: 7d2f 2a2a 2f73 6974 652d 7061 636b 6167  }/**/site-packag
-000005a0: 6573 225d 2c0a 2020 2270 7974 686f 6e2e  es"],.  "python.
-000005b0: 6175 746f 436f 6d70 6c65 7465 2e65 7874  autoComplete.ext
-000005c0: 7261 5061 7468 7322 3a20 5b22 247b 776f  raPaths": ["${wo
-000005d0: 726b 7370 6163 6546 6f6c 6465 727d 2f2a  rkspaceFolder}/*
-000005e0: 2a2f 7369 7465 2d70 6163 6b61 6765 7322  */site-packages"
-000005f0: 5d2c 0a20 2022 7079 7468 6f6e 2e6c 696e  ],.  "python.lin
-00000600: 7469 6e67 2e65 6e61 626c 6564 223a 2074  ting.enabled": t
-00000610: 7275 652c 0a20 2022 5b70 7974 686f 6e5d  rue,.  "[python]
-00000620: 223a 207b 0a20 2020 2022 6564 6974 6f72  ": {.    "editor
-00000630: 2e74 6162 5369 7a65 223a 2034 2c0a 2020  .tabSize": 4,.  
-00000640: 2020 2265 6469 746f 722e 696e 7365 7274    "editor.insert
-00000650: 5370 6163 6573 223a 2074 7275 652c 0a20  Spaces": true,. 
-00000660: 2020 2022 6564 6974 6f72 2e66 6f72 6d61     "editor.forma
-00000670: 744f 6e53 6176 6522 3a20 7472 7565 2c0a  tOnSave": true,.
-00000680: 2020 2020 2265 6469 746f 722e 666f 726d      "editor.form
-00000690: 6174 4f6e 5061 7374 6522 3a20 6661 6c73  atOnPaste": fals
-000006a0: 652c 0a20 2020 2022 6564 6974 6f72 2e66  e,.    "editor.f
-000006b0: 6f72 6d61 744f 6e53 6176 654d 6f64 6522  ormatOnSaveMode"
-000006c0: 3a20 2266 696c 6522 2c0a 2020 2020 2265  : "file",.    "e
-000006d0: 7869 746f 722e 666f 726d 6174 4f6e 5479  xitor.formatOnTy
-000006e0: 7065 223a 2066 616c 7365 2c0a 2020 2020  pe": false,.    
-000006f0: 2265 6469 746f 722e 636f 6465 4163 7469  "editor.codeActi
-00000700: 6f6e 734f 6e53 6176 6522 3a20 7b0a 2020  onsOnSave": {.  
-00000710: 2020 2020 2273 6f75 7263 652e 6669 7841      "source.fixA
-00000720: 6c6c 223a 2022 6578 706c 6963 6974 222c  ll": "explicit",
-00000730: 0a20 2020 2020 2022 736f 7572 6365 2e6f  .      "source.o
-00000740: 7267 616e 697a 6549 6d70 6f72 7473 223a  rganizeImports":
-00000750: 2022 6578 706c 6963 6974 222c 0a20 2020   "explicit",.   
-00000760: 2020 2022 736f 7572 6365 2e75 6e75 7365     "source.unuse
-00000770: 6449 6d70 6f72 7473 223a 2022 6578 706c  dImports": "expl
-00000780: 6963 6974 220a 2020 2020 7d2c 0a20 2020  icit".    },.   
-00000790: 2022 6564 6974 6f72 2e64 6566 6175 6c74   "editor.default
-000007a0: 466f 726d 6174 7465 7222 3a20 226d 732d  Formatter": "ms-
-000007b0: 7079 7468 6f6e 2e62 6c61 636b 2d66 6f72  python.black-for
-000007c0: 6d61 7474 6572 220a 2020 7d2c 0a20 2022  matter".  },.  "
-000007d0: 6564 6974 6f72 2e69 6e73 6572 7453 7061  editor.insertSpa
-000007e0: 6365 7322 3a20 7472 7565 2c0a 2020 2265  ces": true,.  "e
-000007f0: 6469 746f 722e 7461 6253 697a 6522 3a20  ditor.tabSize": 
-00000800: 342c 0a20 2022 7079 7468 6f6e 2e64 6566  4,.  "python.def
-00000810: 6175 6c74 496e 7465 7270 7265 7465 7250  aultInterpreterP
-00000820: 6174 6822 3a20 2224 7b77 6f72 6b73 7061  ath": "${workspa
-00000830: 6365 466f 6c64 6572 7d2f 2e76 656e 762f  ceFolder}/.venv/
-00000840: 6269 6e2f 7079 7468 6f6e 222c 0a0a 2020  bin/python",..  
-00000850: 2270 7974 686f 6e2e 616e 616c 7973 6973  "python.analysis
-00000860: 2e74 7970 6543 6865 636b 696e 674d 6f64  .typeCheckingMod
-00000870: 6522 3a20 2262 6173 6963 222c 0a20 2022  e": "basic",.  "
-00000880: 7079 7468 6f6e 2e61 6e61 6c79 7369 732e  python.analysis.
-00000890: 6175 746f 496d 706f 7274 5573 6572 5379  autoImportUserSy
-000008a0: 6d62 6f6c 7322 3a20 7472 7565 2c0a 2020  mbols": true,.  
-000008b0: 2270 7974 686f 6e2e 616e 616c 7973 6973  "python.analysis
-000008c0: 2e61 7574 6f49 6d70 6f72 7443 6f6d 706c  .autoImportCompl
-000008d0: 6574 696f 6e73 223a 2074 7275 652c 0a20  etions": true,. 
-000008e0: 2022 7079 7468 6f6e 2e61 6e61 6c79 7369   "python.analysi
-000008f0: 732e 636f 6d70 6c65 7465 4675 6e63 7469  s.completeFuncti
-00000900: 6f6e 5061 7265 6e73 223a 2066 616c 7365  onParens": false
-00000910: 2c0a 2020 2270 7974 686f 6e2e 6175 746f  ,.  "python.auto
-00000920: 436f 6d70 6c65 7465 2e61 6464 4272 6163  Complete.addBrac
-00000930: 6b65 7473 223a 2066 616c 7365 2c0a 2020  kets": false,.  
-00000940: 2270 7974 686f 6e2e 616e 616c 7973 6973  "python.analysis
-00000950: 2e69 6e64 6578 696e 6722 3a20 7472 7565  .indexing": true
-00000960: 2c0a 2020 2270 7974 686f 6e2e 616e 616c  ,.  "python.anal
-00000970: 7973 6973 2e70 6163 6b61 6765 496e 6465  ysis.packageInde
-00000980: 7844 6570 7468 7322 3a20 5b0a 2020 2020  xDepths": [.    
-00000990: 7b0a 2020 2020 2020 226e 616d 6522 3a20  {.      "name": 
-000009a0: 2222 2c0a 2020 2020 2020 2264 6570 7468  "",.      "depth
-000009b0: 223a 2033 2c0a 2020 2020 2020 2269 6e63  ": 3,.      "inc
-000009c0: 6c75 6465 416c 6c53 796d 626f 6c73 223a  ludeAllSymbols":
-000009d0: 2074 7275 650a 2020 2020 7d0a 2020 5d2c   true.    }.  ],
-000009e0: 0a20 2022 7079 7468 6f6e 2e61 6e61 6c79  .  "python.analy
-000009f0: 7369 732e 6175 746f 5365 6172 6368 5061  sis.autoSearchPa
-00000a00: 7468 7322 3a20 7472 7565 2c0a 2020 2270  ths": true,.  "p
-00000a10: 7974 686f 6e2e 6c61 6e67 7561 6765 5365  ython.languageSe
-00000a20: 7276 6572 223a 2022 5079 6c61 6e63 6522  rver": "Pylance"
-00000a30: 2c0a 2020 2270 7974 686f 6e2e 666f 726d  ,.  "python.form
-00000a40: 6174 7469 6e67 2e70 726f 7669 6465 7222  atting.provider"
-00000a50: 3a20 2272 7566 6622 0a7d 0a              : "ruff".}.
+000003f0: 2022 2336 3164 6166 6222 2c0a 2020 2270   "#61dafb",.  "p
+00000400: 7974 686f 6e2e 7465 7374 696e 672e 756e  ython.testing.un
+00000410: 6974 7465 7374 456e 6162 6c65 6422 3a20  ittestEnabled": 
+00000420: 6661 6c73 652c 0a20 2022 7079 7468 6f6e  false,.  "python
+00000430: 2e74 6573 7469 6e67 2e70 7974 6573 7445  .testing.pytestE
+00000440: 6e61 626c 6564 223a 2074 7275 652c 0a20  nabled": true,. 
+00000450: 2022 7079 7468 6f6e 2e74 6573 7469 6e67   "python.testing
+00000460: 2e63 7764 223a 2022 247b 776f 726b 7370  .cwd": "${worksp
+00000470: 6163 6546 6f6c 6465 727d 222c 0a20 2022  aceFolder}",.  "
+00000480: 7079 7468 6f6e 2e74 6572 6d69 6e61 6c2e  python.terminal.
+00000490: 6163 7469 7661 7465 456e 7669 726f 6e6d  activateEnvironm
+000004a0: 656e 7422 3a20 7472 7565 2c0a 2020 2270  ent": true,.  "p
+000004b0: 7974 686f 6e2e 7465 726d 696e 616c 2e61  ython.terminal.a
+000004c0: 6374 6976 6174 6545 6e76 496e 4375 7272  ctivateEnvInCurr
+000004d0: 656e 7454 6572 6d69 6e61 6c22 3a20 7472  entTerminal": tr
+000004e0: 7565 2c0a 2020 2270 7974 686f 6e2e 7465  ue,.  "python.te
+000004f0: 7374 696e 672e 6175 746f 5465 7374 4469  sting.autoTestDi
+00000500: 7363 6f76 6572 4f6e 5361 7665 456e 6162  scoverOnSaveEnab
+00000510: 6c65 6422 3a20 7472 7565 2c0a 2020 2270  led": true,.  "p
+00000520: 7974 686f 6e2e 616e 616c 7973 6973 2e65  ython.analysis.e
+00000530: 7874 7261 5061 7468 7322 3a20 5b22 247b  xtraPaths": ["${
+00000540: 776f 726b 7370 6163 6546 6f6c 6465 727d  workspaceFolder}
+00000550: 2f2a 2a2f 7369 7465 2d70 6163 6b61 6765  /**/site-package
+00000560: 7322 5d2c 0a20 2022 7079 7468 6f6e 2e61  s"],.  "python.a
+00000570: 7574 6f43 6f6d 706c 6574 652e 6578 7472  utoComplete.extr
+00000580: 6150 6174 6873 223a 205b 2224 7b77 6f72  aPaths": ["${wor
+00000590: 6b73 7061 6365 466f 6c64 6572 7d2f 2a2a  kspaceFolder}/**
+000005a0: 2f73 6974 652d 7061 636b 6167 6573 225d  /site-packages"]
+000005b0: 2c0a 2020 2270 7974 686f 6e2e 6c69 6e74  ,.  "python.lint
+000005c0: 696e 672e 656e 6162 6c65 6422 3a20 7472  ing.enabled": tr
+000005d0: 7565 2c0a 2020 225b 7079 7468 6f6e 5d22  ue,.  "[python]"
+000005e0: 3a20 7b0a 2020 2020 2265 6469 746f 722e  : {.    "editor.
+000005f0: 7461 6253 697a 6522 3a20 342c 0a20 2020  tabSize": 4,.   
+00000600: 2022 6564 6974 6f72 2e69 6e73 6572 7453   "editor.insertS
+00000610: 7061 6365 7322 3a20 7472 7565 2c0a 2020  paces": true,.  
+00000620: 2020 2265 6469 746f 722e 666f 726d 6174    "editor.format
+00000630: 4f6e 5361 7665 223a 2074 7275 652c 0a20  OnSave": true,. 
+00000640: 2020 2022 6564 6974 6f72 2e66 6f72 6d61     "editor.forma
+00000650: 744f 6e50 6173 7465 223a 2066 616c 7365  tOnPaste": false
+00000660: 2c0a 2020 2020 2265 6469 746f 722e 666f  ,.    "editor.fo
+00000670: 726d 6174 4f6e 5361 7665 4d6f 6465 223a  rmatOnSaveMode":
+00000680: 2022 6669 6c65 222c 0a20 2020 2022 6578   "file",.    "ex
+00000690: 6974 6f72 2e66 6f72 6d61 744f 6e54 7970  itor.formatOnTyp
+000006a0: 6522 3a20 6661 6c73 652c 0a20 2020 2022  e": false,.    "
+000006b0: 6564 6974 6f72 2e63 6f64 6541 6374 696f  editor.codeActio
+000006c0: 6e73 4f6e 5361 7665 223a 207b 0a20 2020  nsOnSave": {.   
+000006d0: 2020 2022 736f 7572 6365 2e66 6978 416c     "source.fixAl
+000006e0: 6c22 3a20 2265 7870 6c69 6369 7422 2c0a  l": "explicit",.
+000006f0: 2020 2020 2020 2273 6f75 7263 652e 6f72        "source.or
+00000700: 6761 6e69 7a65 496d 706f 7274 7322 3a20  ganizeImports": 
+00000710: 2265 7870 6c69 6369 7422 2c0a 2020 2020  "explicit",.    
+00000720: 2020 2273 6f75 7263 652e 756e 7573 6564    "source.unused
+00000730: 496d 706f 7274 7322 3a20 2265 7870 6c69  Imports": "expli
+00000740: 6369 7422 0a20 2020 207d 2c0a 2020 2020  cit".    },.    
+00000750: 2265 6469 746f 722e 6465 6661 756c 7446  "editor.defaultF
+00000760: 6f72 6d61 7474 6572 223a 2022 6d73 2d70  ormatter": "ms-p
+00000770: 7974 686f 6e2e 626c 6163 6b2d 666f 726d  ython.black-form
+00000780: 6174 7465 7222 0a20 207d 2c0a 2020 2265  atter".  },.  "e
+00000790: 6469 746f 722e 696e 7365 7274 5370 6163  ditor.insertSpac
+000007a0: 6573 223a 2074 7275 652c 0a20 2022 6564  es": true,.  "ed
+000007b0: 6974 6f72 2e74 6162 5369 7a65 223a 2034  itor.tabSize": 4
+000007c0: 2c0a 2020 2270 7974 686f 6e2e 6465 6661  ,.  "python.defa
+000007d0: 756c 7449 6e74 6572 7072 6574 6572 5061  ultInterpreterPa
+000007e0: 7468 223a 2022 247b 776f 726b 7370 6163  th": "${workspac
+000007f0: 6546 6f6c 6465 727d 2f2e 7665 6e76 2f62  eFolder}/.venv/b
+00000800: 696e 2f70 7974 686f 6e22 2c0a 0a20 2022  in/python",..  "
+00000810: 7079 7468 6f6e 2e61 6e61 6c79 7369 732e  python.analysis.
+00000820: 7479 7065 4368 6563 6b69 6e67 4d6f 6465  typeCheckingMode
+00000830: 223a 2022 6261 7369 6322 2c0a 2020 2270  ": "basic",.  "p
+00000840: 7974 686f 6e2e 616e 616c 7973 6973 2e61  ython.analysis.a
+00000850: 7574 6f49 6d70 6f72 7455 7365 7253 796d  utoImportUserSym
+00000860: 626f 6c73 223a 2074 7275 652c 0a20 2022  bols": true,.  "
+00000870: 7079 7468 6f6e 2e61 6e61 6c79 7369 732e  python.analysis.
+00000880: 6175 746f 496d 706f 7274 436f 6d70 6c65  autoImportComple
+00000890: 7469 6f6e 7322 3a20 7472 7565 2c0a 2020  tions": true,.  
+000008a0: 2270 7974 686f 6e2e 616e 616c 7973 6973  "python.analysis
+000008b0: 2e63 6f6d 706c 6574 6546 756e 6374 696f  .completeFunctio
+000008c0: 6e50 6172 656e 7322 3a20 6661 6c73 652c  nParens": false,
+000008d0: 0a20 2022 7079 7468 6f6e 2e61 7574 6f43  .  "python.autoC
+000008e0: 6f6d 706c 6574 652e 6164 6442 7261 636b  omplete.addBrack
+000008f0: 6574 7322 3a20 6661 6c73 652c 0a20 2022  ets": false,.  "
+00000900: 7079 7468 6f6e 2e61 6e61 6c79 7369 732e  python.analysis.
+00000910: 696e 6465 7869 6e67 223a 2074 7275 652c  indexing": true,
+00000920: 0a20 2022 7079 7468 6f6e 2e61 6e61 6c79  .  "python.analy
+00000930: 7369 732e 7061 636b 6167 6549 6e64 6578  sis.packageIndex
+00000940: 4465 7074 6873 223a 205b 0a20 2020 207b  Depths": [.    {
+00000950: 0a20 2020 2020 2022 6e61 6d65 223a 2022  .      "name": "
+00000960: 222c 0a20 2020 2020 2022 6465 7074 6822  ",.      "depth"
+00000970: 3a20 332c 0a20 2020 2020 2022 696e 636c  : 3,.      "incl
+00000980: 7564 6541 6c6c 5379 6d62 6f6c 7322 3a20  udeAllSymbols": 
+00000990: 7472 7565 0a20 2020 207d 0a20 205d 2c0a  true.    }.  ],.
+000009a0: 2020 2270 7974 686f 6e2e 616e 616c 7973    "python.analys
+000009b0: 6973 2e61 7574 6f53 6561 7263 6850 6174  is.autoSearchPat
+000009c0: 6873 223a 2074 7275 652c 0a20 2022 7079  hs": true,.  "py
+000009d0: 7468 6f6e 2e6c 616e 6775 6167 6553 6572  thon.languageSer
+000009e0: 7665 7222 3a20 2250 796c 616e 6365 222c  ver": "Pylance",
+000009f0: 0a20 2022 7079 7468 6f6e 2e66 6f72 6d61  .  "python.forma
+00000a00: 7474 696e 672e 7072 6f76 6964 6572 223a  tting.provider":
+00000a10: 2022 7275 6666 220a 7d0a                  "ruff".}.
```

### Comparing `tinta-0.1.7b2/.vscode/tasks.json` & `tinta-0.1.7b3/.vscode/tasks.json`

 * *Files identical despite different names*

### Comparing `tinta-0.1.7b2/examples/tinta-discover.png` & `tinta-0.1.7b3/examples/tinta-discover.png`

 * *Files identical despite different names*

### Comparing `tinta-0.1.7b2/junit/test-results.xml` & `tinta-0.1.7b3/junit/test-results.xml`

 * *Files identical despite different names*

### Comparing `tinta-0.1.7b2/tests/conftest.py` & `tinta-0.1.7b3/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `tinta-0.1.7b2/tests/test_discover.py` & `tinta-0.1.7b3/tests/test_discover.py`

 * *Files identical despite different names*

### Comparing `tinta-0.1.7b2/tinta/__init__.py` & `tinta-0.1.7b3/tinta/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 # out in the MIT License.
 
 # Where a conflict or dispute would arise between these two licenses, HLv2.1
 # shall take precedence.
 
 from logging import getLogger
 
-__version__ = "0.1.7b2"
+__version__ = "0.1.7b3"
 
 logger = getLogger(__name__)
 
 try:
     from .tinta import Tinta
 
     assert bool(Tinta)
```

### Comparing `tinta-0.1.7b2/tinta/__main__.py` & `tinta-0.1.7b3/tinta/__main__.py`

 * *Files identical despite different names*

### Comparing `tinta-0.1.7b2/tinta/ansi.py` & `tinta-0.1.7b3/tinta/ansi.py`

 * *Files 14% similar despite different names*

```diff
@@ -19,14 +19,25 @@
 from typing import List, Optional, Union
 
 from .typ import MissingColorError
 
 config = configparser.ConfigParser()
 
 
+def _alias_key(colors: "AnsiColors", k: str, search: str, repl: str):
+    """Sets up an alias key for a color."""
+    if k not in config["colors"] and k not in colors.__dict__:
+        raise MissingColorError(f"Color '{k}' not found in colors.ini.")
+    if search.lower() in k.lower():
+        alias_key = k.replace(search.lower(), repl.lower())
+        if alias_key not in config["colors"] and alias_key not in colors.__dict__:
+            colors.__setattr__(alias_key, int(config["colors"][k]))
+            config["colors"][alias_key] = config["colors"][k]
+
+
 class AnsiColors:
     """Color builder for Tinta's console output.
 
     ANSI color map for console output. Get a list of colors here =
     http://www.lihaoyi.com/post/BuildyourownCommandLinewithANSIescapecodes.html#256-colors
 
     Or run Tinta.discover() to see all 256 colors on your system.
@@ -60,14 +71,19 @@
                 f"Tinta failed to load colors, could not find 'colors.ini' in cwd or in PYTHONPATH. Please provide a valid path to a colors.ini file."
             )
 
         config.read(path)
         for k, v in config["colors"].items():
             self.__setattr__(k, int(v))
 
+            _alias_key(self, k, "gray", "grey")
+            _alias_key(self, k, "grey", "gray")
+
+        self._colors_ini_path = path
+
     def get(self, color: str) -> int:
         """Returns the ANSI code for a color.
 
         Args:
             color (str): A color name.
 
         Returns:
```

### Comparing `tinta-0.1.7b2/tinta/colorize.py` & `tinta-0.1.7b3/tinta/colorize.py`

 * *Files 3% similar despite different names*

```diff
@@ -17,37 +17,45 @@
 # modified by github.com/brandoncript to be used in the Tinta project. It is
 # distributed under the same license as the original module, as well as the
 # MIT License.
 
 import re
 from typing import Any, List, Optional, overload, Tuple, TYPE_CHECKING, Union
 
-from .constants import SEP
+from .constants import ANSI_RESET_HEX, ANSI_RESET_OCT, SEP
 from .typ import MissingColorError
 
 if TYPE_CHECKING:
     from .tinta import Tinta
 
-ANSI_RESET_HEX = "\x1b[0m"
-ANSI_RESET_OCT = "\033[0m"
-
 STYLES = (
     "none",
     "bold",
     "faint",
     "italic",
     "underline",
     "blink",
     "blink2",
     "negative",
     "concealed",
     "crossed",
 )
 
 
+def was_reset(s: str) -> bool:
+    return s.strip().endswith(ANSI_RESET_HEX) or s.endswith(ANSI_RESET_OCT)
+
+
+def ensure_reset(s: str) -> str:
+    if was_reset(s):
+        return s
+    last_char_idx = len(s.rstrip())
+    return f"{s[:last_char_idx]}{ANSI_RESET_HEX}{s[last_char_idx:]}"
+
+
 def _parse_rgb(s: str) -> Tuple[int, ...]:
     if not isinstance(s, str):
         raise ValueError(f"Could not parse color '{s}'")
     s = s.strip().replace(" ", "").lower()
 
     # 6-digit hex
     match = re.match("#([a-f0-9]{6})$", s)
```

### Comparing `tinta-0.1.7b2/tinta/constants.py` & `tinta-0.1.7b3/tinta/constants.py`

 * *Files 6% similar despite different names*

```diff
@@ -18,11 +18,13 @@
 
 import os
 
 from .typ import parse_bool
 
 CURSOR_UP_ONE = "\x1b[1A"
 ERASE_LINE = "\x1b[2K"
+ANSI_RESET_HEX = "\x1b[0m"
+ANSI_RESET_OCT = "\033[0m"
 SEP = os.getenv("TINTA_SEPARATOR", " ")
 STEALTH = parse_bool(os.getenv("TINTA_STEALTH", False))
 PREFER_PLAINTEXT = parse_bool(os.getenv("TINTA_PLAINTEXT", False))
 SMART_FIX_PUNCTUATION = parse_bool(os.getenv("TINTA_SMART_FIX_PUNCTUATION", True))
```

### Comparing `tinta-0.1.7b2/tinta/discover.py` & `tinta-0.1.7b3/tinta/discover.py`

 * *Files identical despite different names*

### Comparing `tinta-0.1.7b2/tinta/multi_version_imports.py` & `tinta-0.1.7b3/tinta/multi_version_imports.py`

 * *Files identical despite different names*

### Comparing `tinta-0.1.7b2/tinta/tinta.py` & `tinta-0.1.7b3/tinta/tinta.py`

 * *Files 3% similar despite different names*

```diff
@@ -19,21 +19,28 @@
 import configparser
 import functools
 import os
 import re
 import sys
 from itertools import zip_longest
 from pathlib import Path
-from typing import Any, cast, List, Optional, overload, Union
+from typing import Any, cast, Dict, List, Optional, overload, Union
 
 from deprecated import deprecated
 
 from .ansi import AnsiColors
-from .colorize import ANSI_RESET_HEX, colorize, tint
-from .constants import PREFER_PLAINTEXT, SEP, SMART_FIX_PUNCTUATION, STEALTH
+from .colorize import colorize, ensure_reset, tint, was_reset
+from .constants import (
+    CURSOR_UP_ONE,
+    ERASE_LINE,
+    PREFER_PLAINTEXT,
+    SEP,
+    SMART_FIX_PUNCTUATION,
+    STEALTH,
+)
 from .discover import discover as _discover
 from .typ import copy_kwargs, MissingColorError, StringType
 
 config = configparser.ConfigParser()
 
 
 class _MetaTinta(type):
@@ -98,15 +105,15 @@
         normal() -> self:           Removes all styles.
         clear() -> self:            Removes all styles and colors.
         line() -> self:             Adds segments on a new line.
         print():                    Prints the output of a Tinta instance, then clears.
     """
 
     _initialized = False
-    _known_colors: dict[str, Any] = {}
+    _known_colors: Dict[str, Any] = {}
     color: Union[int, str]
     colors: AnsiColors
 
     def __init__(
         self, *s: Any, color: Optional[Union[str, int]] = None, sep: str = SEP
     ):
         """Main intializer for Tinta
@@ -122,15 +129,15 @@
         self._prefixes: List[str] = []
 
         # Inject ANSI helper functions
         if not Tinta._initialized:
             Tinta._known_colors = vars(self.colors)
             Tinta._initialized = True
         for c in Tinta._known_colors:
-            self.__setattr__(c, functools.partial(self.tint, c))
+            self.__setattr__(c, functools.partial(self.tint, color=c))
 
         if s:
             self.push(*s, sep=sep)
 
     def __call__(self, *s: Any, sep: str = SEP) -> "Tinta":
         return self.push(*s, sep=sep)
 
@@ -139,14 +146,23 @@
         Tinta instance.
 
         Returns:
             str: Plaintext string
         """
         return str(self.to_str(plaintext=True))
 
+    def __str__(self) -> str:
+        """Generates a string representation of the current
+        Tinta instance, colorized.
+
+        Returns:
+            str: Colorized string"""
+
+        return self.to_str()
+
     def _get_sep(
         self,
         p: "Tinta.Part",
         next_p: Optional["Tinta.Part"],
         sep: Optional[str],
     ) -> str:
         if not next_p:
@@ -186,32 +202,32 @@
                     (len(next_p.pln) > 1 and next_p.pln[1] == " "),
                 ]
             )
             if next_p and next_p.pln
             else False
         )
 
-        next_char_is_newline = next_p and next_p.pln.startswith(os.linesep)
+        next_char_is_newline = bool(next_p and next_p.pln.startswith(os.linesep))
         last_char_is_newline = p.pln.endswith(os.linesep)
         newline_affects_punc = last_char_is_newline or next_char_is_newline
 
         should_ignore_sep = punc_affects_sep or newline_affects_punc
 
         if not should_ignore_sep:
             s = f"{s}{self._get_sep(p, next_p, sep)}"
 
         # TODO: Not certain we ever want to do this, it has too many false negatives
         # if fix_punc:
         #     s = re.sub(r"(\w)\s+([.,;:!?])", r"\1\2", s)
 
         if next_p is None and p.has_formatting:
             if attr == "fmt":
-                s += ANSI_RESET_HEX
+                s = ensure_reset(s)
             elif attr == "esc":
-                s += esc(ANSI_RESET_HEX)
+                s = esc(ensure_reset(s))
 
         return s
 
     def to_str(
         self,
         sep: Optional[str] = None,
         plaintext: bool = False,
@@ -624,24 +640,27 @@
             force (bool, option): Forces printing, overriding TINTA_STEALTH.
         """
         # We don't print if the TINTA_STEALTH env is set
         if STEALTH and not force:
             return
 
         use_plaintext = True if plaintext or PREFER_PLAINTEXT else False
+        s = self.to_str(sep=sep, plaintext=use_plaintext)
+        # if s.strip() does not end with reset, add it after the last non-whitespace character
+        if not use_plaintext and not was_reset(s):
+            s = ensure_reset(s)
         print(
             self.to_str(sep=sep, plaintext=use_plaintext),
             end=end,
             file=file,
             flush=flush,
         )
 
         self.clear()
         self._parts = []
-        print("\033[0m", end="", file=file, flush=flush)
 
     def __getattr__(self, name: str) -> "Tinta":
         """Returns a tinted segment of text.
 
         Args:
             name (str): Name of the color.
 
@@ -728,22 +747,22 @@
         return re.sub(
             r"\x1B(?:[@-Z\\-_]|\[[0-?]*[ -/]*[@-~])", "", s, re.I | re.M | re.U
         )
 
     @classmethod
     def ljust(cls, s: str, width: int, fillchar: str = " ") -> str:
         """Returns a string left justified in a field of a specified width, accounting for ansi formatting."""
-        p = cls.strip_ansi(s)
-        return s.replace(p, p.ljust(width, fillchar))
+        chars_to_add = width - len(cls.strip_ansi(s))
+        return f"{s}{str(fillchar or '') * chars_to_add}"
 
     @classmethod
     def rjust(cls, s: str, width: int, fillchar: str = " ") -> str:
         """Returns a string right justified in a field of a specified width, accounting for ansi formatting."""
-        p = cls.strip_ansi(s)
-        return s.replace(p, p.rjust(width, fillchar))
+        chars_to_add = width - len(cls.strip_ansi(s))
+        return f"{str(fillchar or '') * chars_to_add}{s}"
 
 
 def esc(string: str, replace: bool = False) -> str:
     """Returns the raw representation of a string. If replace is true,
     replace a double backslash with a single backslash."""
     r = repr(string)[1:-1]  # Strip the quotes from representation
     if replace:
```

### Comparing `tinta-0.1.7b2/tinta/typ.py` & `tinta-0.1.7b3/tinta/typ.py`

 * *Files identical despite different names*

### Comparing `tinta-0.1.7b2/.gitignore` & `tinta-0.1.7b3/.gitignore`

 * *Files identical despite different names*

### Comparing `tinta-0.1.7b2/LICENSE` & `tinta-0.1.7b3/LICENSE`

 * *Files identical despite different names*

### Comparing `tinta-0.1.7b2/README.md` & `tinta-0.1.7b3/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 ## Tinta
 
 <img width="200" alt="Tinta Logo" src="https://user-images.githubusercontent.com/1480253/118584629-38023b80-b74c-11eb-8511-05258af553fb.png" />
 
 Tinta is a magical console output tool with support for printing in beautiful colors and with rich formatting, like bold and underline, using static, chain-able methods. It's so pretty, it's almost like a unicorn!
 
-![version](https://img.shields.io/badge/version-0.1.7b2-green.svg) [_![GitHub Actions Badge](https://img.shields.io/github/actions/workflow/status/brandonscript/tinta/run-tests.yml)_](https://github.com/brandonscript/tinta/actions) [_![Codacy Badge](https://app.codacy.com/project/badge/Grade/32bf3e3172cf434b914647f06569a836)_](https://www.codacy.com/gh/brandonscript/tinta/dashboard?utm_source=github.com&utm_medium=referral&utm_content=brandonscript/tinta&utm_campaign=Badge_Grade) ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/tinta) ![MIT License](https://img.shields.io/github/license/brandonscript/tinta) [_![](https://img.shields.io/badge/ethical-source-%23bb8c3c?labelColor=393162)_](https://img.shields.io/badge/ethical-source-%23bb8c3c?labelColor=393162) [_![Contributor Covenant](https://img.shields.io/badge/Contributor%20Covenant-2.0-4baaaa.svg)_](code_of_conduct.md)
+![version](https://img.shields.io/badge/version-0.1.7b3-green.svg) [_![GitHub Actions Badge](https://img.shields.io/github/actions/workflow/status/brandonscript/tinta/run-tests.yml)_](https://github.com/brandonscript/tinta/actions) [_![Codacy Badge](https://app.codacy.com/project/badge/Grade/32bf3e3172cf434b914647f06569a836)_](https://www.codacy.com/gh/brandonscript/tinta/dashboard?utm_source=github.com&utm_medium=referral&utm_content=brandonscript/tinta&utm_campaign=Badge_Grade) ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/tinta) ![MIT License](https://img.shields.io/github/license/brandonscript/tinta) [_![](https://img.shields.io/badge/ethical-source-%23bb8c3c?labelColor=393162)_](https://img.shields.io/badge/ethical-source-%23bb8c3c?labelColor=393162) [_![Contributor Covenant](https://img.shields.io/badge/Contributor%20Covenant-2.0-4baaaa.svg)_](code_of_conduct.md)
 
 ## Features and Tinta Basics
 
 `Tinta` takes a statically typed approach to handling rich-color console output.
 
 In the past you might have fiddled with ANSI colors codes, or passed strings to a generic class, only to discover you typo'd one of them! (Yes, we've all been there).
 
@@ -189,15 +189,15 @@
 
 ### Common Args
 
 All "add" methods (each color and style method, `Tinta()`, `push()`, and `tint`) take the following common args:
 
 - `s (str)` – A sequence of one or more text strings, to be joined together.
 - `sep (str)` – Used to join segment strings. Defaults to `' '`.
-  > _Note: `sep` behavior has been changed in v0.1.7b2 - if passing a `sep` argument in `print()`, it will overwrite any segment's individual `sep` argument._
+  > _Note: `sep` behavior has been changed in v0.1.7b3 - if passing a `sep` argument in `print()`, it will overwrite any segment's individual `sep` argument._
 
 For example:
 
 ```python
 Tinta('A set', 'of strings', 'joined', 'with', 'semicolons', sep=';').print()
 ```
 
@@ -224,15 +224,15 @@
 - `parts (list)` — A list of `Tinta.Part` segments, which each have a `fmt`, `pln`, and `esc` attribute.
 - ~~`parts_plaintext (list)` — A list of unstyled text segments.~~
 
 ### Built-in Methods
 
 _See below for detailed usage and arguments._
 
-> (Note: breaking changes in v0.1.7b2 - several methods have been renamed for better semantics).
+> (Note: breaking changes in v0.1.7b3 - several methods have been renamed for better semantics).
 
 - `print()` – Prints to the console.
 - `to_str() -> str` – Returns a joined text string.
 - `discover()` – Prints a list of available colors to the console.
 
 Remember, all of the following methods return the current `Tinta` instance `-> self` so you can chain styles together:
```

### Comparing `tinta-0.1.7b2/pyproject.toml` & `tinta-0.1.7b3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 # out in the MIT License.
 
 # Where a conflict or dispute would arise between these two licenses, HLv2.1
 # shall take precedence.
 
 [project]
 name = "tinta"
-version = "0.1.7b2"
+version = "0.1.7b3"
 description = "Tinta, a magical console output tool."
 authors = [{ name = "Brandon Shelley", email = "brandon@pacificaviator.co" }]
 license = "MIT"
 readme = "README.md"
 keywords = [
   "console",
   "colors",
@@ -151,12 +151,12 @@
 line-ending = "auto"
 skip-magic-trailing-comma = false
 quote-style = "double"
 
 [tool.pytest.ini_options]
 pythonpath = ["."]
 minversion = "7.0"
-addopts = "-s -rP -x -vv --color=yes"
+addopts = "-rP -vv --color=yes --capture=tee-sys"
 testpaths = ["tests"]
 python_files = ["*_test.py", "test_*.py"]
 python_classes = ["test_", "_test", "Test*"]
 python_functions = ["test_", "_test"]
```

### Comparing `tinta-0.1.7b2/PKG-INFO` & `tinta-0.1.7b3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: tinta
-Version: 0.1.7b2
+Version: 0.1.7b3
 Summary: Tinta, a magical console output tool.
 Project-URL: homepage, https://github.com/brandonscript/tinta
 Project-URL: repository, https://github.com/brandonscript/tinta
 Author-email: Brandon Shelley <brandon@pacificaviator.co>
 License-Expression: MIT
 License-File: LICENSE
 Keywords: ansi,cli,colors,console,development,print,term,terminal
@@ -25,15 +25,15 @@
 
 ## Tinta
 
 <img width="200" alt="Tinta Logo" src="https://user-images.githubusercontent.com/1480253/118584629-38023b80-b74c-11eb-8511-05258af553fb.png" />
 
 Tinta is a magical console output tool with support for printing in beautiful colors and with rich formatting, like bold and underline, using static, chain-able methods. It's so pretty, it's almost like a unicorn!
 
-![version](https://img.shields.io/badge/version-0.1.7b2-green.svg) [_![GitHub Actions Badge](https://img.shields.io/github/actions/workflow/status/brandonscript/tinta/run-tests.yml)_](https://github.com/brandonscript/tinta/actions) [_![Codacy Badge](https://app.codacy.com/project/badge/Grade/32bf3e3172cf434b914647f06569a836)_](https://www.codacy.com/gh/brandonscript/tinta/dashboard?utm_source=github.com&utm_medium=referral&utm_content=brandonscript/tinta&utm_campaign=Badge_Grade) ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/tinta) ![MIT License](https://img.shields.io/github/license/brandonscript/tinta) [_![](https://img.shields.io/badge/ethical-source-%23bb8c3c?labelColor=393162)_](https://img.shields.io/badge/ethical-source-%23bb8c3c?labelColor=393162) [_![Contributor Covenant](https://img.shields.io/badge/Contributor%20Covenant-2.0-4baaaa.svg)_](code_of_conduct.md)
+![version](https://img.shields.io/badge/version-0.1.7b3-green.svg) [_![GitHub Actions Badge](https://img.shields.io/github/actions/workflow/status/brandonscript/tinta/run-tests.yml)_](https://github.com/brandonscript/tinta/actions) [_![Codacy Badge](https://app.codacy.com/project/badge/Grade/32bf3e3172cf434b914647f06569a836)_](https://www.codacy.com/gh/brandonscript/tinta/dashboard?utm_source=github.com&utm_medium=referral&utm_content=brandonscript/tinta&utm_campaign=Badge_Grade) ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/tinta) ![MIT License](https://img.shields.io/github/license/brandonscript/tinta) [_![](https://img.shields.io/badge/ethical-source-%23bb8c3c?labelColor=393162)_](https://img.shields.io/badge/ethical-source-%23bb8c3c?labelColor=393162) [_![Contributor Covenant](https://img.shields.io/badge/Contributor%20Covenant-2.0-4baaaa.svg)_](code_of_conduct.md)
 
 ## Features and Tinta Basics
 
 `Tinta` takes a statically typed approach to handling rich-color console output.
 
 In the past you might have fiddled with ANSI colors codes, or passed strings to a generic class, only to discover you typo'd one of them! (Yes, we've all been there).
 
@@ -214,15 +214,15 @@
 
 ### Common Args
 
 All "add" methods (each color and style method, `Tinta()`, `push()`, and `tint`) take the following common args:
 
 - `s (str)` – A sequence of one or more text strings, to be joined together.
 - `sep (str)` – Used to join segment strings. Defaults to `' '`.
-  > _Note: `sep` behavior has been changed in v0.1.7b2 - if passing a `sep` argument in `print()`, it will overwrite any segment's individual `sep` argument._
+  > _Note: `sep` behavior has been changed in v0.1.7b3 - if passing a `sep` argument in `print()`, it will overwrite any segment's individual `sep` argument._
 
 For example:
 
 ```python
 Tinta('A set', 'of strings', 'joined', 'with', 'semicolons', sep=';').print()
 ```
 
@@ -249,15 +249,15 @@
 - `parts (list)` — A list of `Tinta.Part` segments, which each have a `fmt`, `pln`, and `esc` attribute.
 - ~~`parts_plaintext (list)` — A list of unstyled text segments.~~
 
 ### Built-in Methods
 
 _See below for detailed usage and arguments._
 
-> (Note: breaking changes in v0.1.7b2 - several methods have been renamed for better semantics).
+> (Note: breaking changes in v0.1.7b3 - several methods have been renamed for better semantics).
 
 - `print()` – Prints to the console.
 - `to_str() -> str` – Returns a joined text string.
 - `discover()` – Prints a list of available colors to the console.
 
 Remember, all of the following methods return the current `Tinta` instance `-> self` so you can chain styles together:
```

