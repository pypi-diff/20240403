# Comparing `tmp/automython-1.1.2.tar.gz` & `tmp/automython-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "automython-1.1.2.tar", last modified: Tue Apr  2 02:29:53 2024, max compression
+gzip compressed data, was "automython-1.2.0.tar", last modified: Wed Apr  3 19:20:06 2024, max compression
```

## Comparing `automython-1.1.2.tar` & `automython-1.2.0.tar`

### file list

```diff
@@ -1,26 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 02:29:53.604455 automython-1.1.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1080 2024-04-02 02:28:41.000000 automython-1.1.2/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)    12876 2024-04-02 02:29:53.604455 automython-1.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    10725 2024-04-02 02:28:41.000000 automython-1.1.2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1011 2024-04-02 02:28:41.000000 automython-1.1.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      234 2024-04-02 02:29:53.604455 automython-1.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1294 2024-04-02 02:28:41.000000 automython-1.1.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 02:29:53.600455 automython-1.1.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 02:29:53.600455 automython-1.1.2/src/automython.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    12876 2024-04-02 02:29:53.000000 automython-1.1.2/src/automython.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      537 2024-04-02 02:29:53.000000 automython-1.1.2/src/automython.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-02 02:29:53.000000 automython-1.1.2/src/automython.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-04-02 02:29:53.000000 automython-1.1.2/src/automython.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       80 2024-04-02 02:29:53.000000 automython-1.1.2/src/automython.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-02 02:29:53.000000 automython-1.1.2/src/automython.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 02:29:53.600455 automython-1.1.2/src/interpret/
--rw-r--r--   0 runner    (1001) docker     (127)     1699 2024-04-02 02:28:41.000000 automython-1.1.2/src/interpret/Buffer.py
--rw-r--r--   0 runner    (1001) docker     (127)     8780 2024-04-02 02:28:41.000000 automython-1.1.2/src/interpret/Lexer.py
--rw-r--r--   0 runner    (1001) docker     (127)    17278 2024-04-02 02:28:41.000000 automython-1.1.2/src/interpret/Parser.py
--rw-r--r--   0 runner    (1001) docker     (127)      725 2024-04-02 02:28:41.000000 automython-1.1.2/src/interpret/Token.py
--rw-r--r--   0 runner    (1001) docker     (127)     7123 2024-04-02 02:28:41.000000 automython-1.1.2/src/interpret/Visitor.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 02:28:41.000000 automython-1.1.2/src/interpret/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2297 2024-04-02 02:28:41.000000 automython-1.1.2/src/interpret/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     2008 2024-04-02 02:28:41.000000 automython-1.1.2/src/interpret/file_interface.py
--rw-r--r--   0 runner    (1001) docker     (127)    18876 2024-04-02 02:28:41.000000 automython-1.1.2/src/interpret/helpers.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      791 2024-04-02 02:28:41.000000 automython-1.1.2/src/interpret/interpreter.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 19:20:06.101591 automython-1.2.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1080 2024-04-03 19:19:02.000000 automython-1.2.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    14924 2024-04-03 19:20:06.101591 automython-1.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    12773 2024-04-03 19:19:02.000000 automython-1.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 19:20:06.093591 automython-1.2.0/automython/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 19:20:06.101591 automython-1.2.0/automython/automython.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    14924 2024-04-03 19:20:06.000000 automython-1.2.0/automython/automython.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      714 2024-04-03 19:20:06.000000 automython-1.2.0/automython/automython.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 19:20:06.000000 automython-1.2.0/automython/automython.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-04-03 19:20:06.000000 automython-1.2.0/automython/automython.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2024-04-03 19:20:06.000000 automython-1.2.0/automython/automython.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-03 19:20:06.000000 automython-1.2.0/automython/automython.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 19:20:06.097591 automython-1.2.0/automython/interpret/
+-rw-r--r--   0 runner    (1001) docker     (127)     1699 2024-04-03 19:19:02.000000 automython-1.2.0/automython/interpret/Buffer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9231 2024-04-03 19:19:02.000000 automython-1.2.0/automython/interpret/Lexer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19716 2024-04-03 19:19:02.000000 automython-1.2.0/automython/interpret/Parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)      725 2024-04-03 19:19:02.000000 automython-1.2.0/automython/interpret/Token.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8377 2024-04-03 19:19:02.000000 automython-1.2.0/automython/interpret/Visitor.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 19:19:02.000000 automython-1.2.0/automython/interpret/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2371 2024-04-03 19:19:02.000000 automython-1.2.0/automython/interpret/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2065 2024-04-03 19:19:02.000000 automython-1.2.0/automython/interpret/file_interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26425 2024-04-03 19:19:02.000000 automython-1.2.0/automython/interpret/helpers.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      791 2024-04-03 19:19:02.000000 automython-1.2.0/automython/interpret/interpreter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12283 2024-04-03 19:19:02.000000 automython-1.2.0/automython/interpret/tm_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2766 2024-04-03 19:19:02.000000 automython-1.2.0/automython/interpret/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1011 2024-04-03 19:19:02.000000 automython-1.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      241 2024-04-03 19:20:06.101591 automython-1.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1308 2024-04-03 19:19:02.000000 automython-1.2.0/setup.py
```

### Comparing `automython-1.1.2/LICENSE.txt` & `automython-1.2.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `automython-1.1.2/PKG-INFO` & `automython-1.2.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,49 +1,8 @@
-Metadata-Version: 2.1
-Name: automython
-Version: 1.1.2
-Summary: A simplistic programming language interpreter to Python to help students grasp finite automata theory programmatically and with a computed graph through visualization libraries.
-Home-page: https://github.com/mkantrr/automython
-Author: Matthew Kanter
-Author-email: Matthew Kanter <matt@matutu.dev>
-Maintainer-email: Matthew Kanter <matt@matutu.dev>
-License: The MIT License (MIT)
-        
-        Copyright (c) 2024 Matthew Kanter
-        
-        Permission is hereby granted, free of charge, to any person obtaining a copy
-        of this software and associated documentation files (the "Software"), to deal
-        in the Software without restriction, including without limitation the rights
-        to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-        copies of the Software, and to permit persons to whom the Software is
-        furnished to do so, subject to the following conditions:
-        
-        The above copyright notice and this permission notice shall be included in
-        all copies or substantial portions of the Software.
-        
-        THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-        IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-        FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-        AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-        LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-        OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
-        THE SOFTWARE.
-Keywords: automata,finite,compiler,interpreter,theory,computational theory,non-deterministic,turing,machine,state
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE.txt
-Requires-Dist: automata-lib[visual]>=8.2.0
-Requires-Dist: pandas>=2.2.0
-Requires-Dist: ipython>=8.22.2
-Requires-Dist: forbiddenfruit>=0.1.4
-
-# Automython
+# Automython (v1.2.0)
 
 *Copyright 2024 Matthew Kanter*  
 *Released under the MIT license*
 
 [![build](https://github.com/mkantrr/automython/actions/workflows/build.yml/badge.svg)](https://github.com/mkantrr/automythonactions/workflows/build.yml)
 
 ## [`https://pypi.org/project/automython`](https://pypi.org/project/automython)
@@ -135,14 +94,18 @@
 
 Dictioniaries in Automython act the same as `dict`s in Python. The only difference in the more limited support types for what you can assign to keys to only Automython's "native" types, and no other Python types that are not included.
 
 #### Set
 
 Sets in Automython act the same as `set`s in Python. The only difference in the more limited support types for what you can assign to keys to only Automython's "native" types, and no other Python types that are not included.
 
+#### Tuple
+
+Tuples in Automython act the same as `tuple`s in Python. The only difference is the more limited support, as you cannot perform most of the Python tuple functions and slick scripting you can here. They are built for a specific purpose, and it is moreso to be integrated with the computational theory concepts below.
+
 #### DFA
 **Deterministic Finite Automaton**:
 
 The DFA object in Automython must resemble this syntax:
 ```python
 DFA(states, input_symbols, transitions, initial_state, final_states, allow_partial[optional]: bool)
 ```
@@ -172,14 +135,34 @@
 
 - The `states` argument is a Set. This can be either a Set in the argument, or a variable that stores a Set.
 - The `input_symbols` argument is a Set. This can be either a Set in the argument, or a variable that stores a Set.
 - The `transitions` argument is a Dictionary. This can be either a Dictionary in the argument, or a variable that stores a Dictionary. The values of each key maps to an input symbol as a key to a Set of states.
 - The `initial_state` argument is a String. This can be either a String in the argument, or a variable that stores a String.
 - The `final_states` argument is a Set. This can be either a Set in the argument, or a variable that stores a Set.
 
+#### DTM
+**Deterministic Turing Machine**:
+
+The DFA object in Automython must resemble this syntax:
+```python
+DTM(states, input_symbols, tape_symbols, transitions, initial_state, blank_symbol, final_states)
+```
+It must **also** be assigned to a variable; it cannot be treated as an expression, i.e.:
+```python
+dtm = DTM(states, input_symbols, tape_symbols, transitions, initial_state, blank_symbol, final_states)
+```
+
+- The `states` argument is a Set. This can be either a Set in the argument, or a variable that stores a Set.
+- The `input_symbols` argument is a Set. This can be either a Set in the argument, or a variable that stores a Set. These symbols are all Strings, and are the only symbols that can exist on the tape before the Turing machine begins its run.
+- The `tape_symbols` argument is a Set. This can be either a Set in the argument, or a variable that stores a Set. These symbols are all Strings that are able to be read and written on the tape.
+- The `transitions` argument is a Dictionary. This can be either a Dictionary in the argument, or a variable that stores a Dictionary. The values of each key maps to an input symbol as a key to a Tuple of strings denoting the new state, write symbol, and direction to move on the tape.
+- The `initial_state` argument is a String. This can be either a String in the argument, or a variable that stores a String.
+- The `blank_symbol` argument is a String. This can be either a String in the argument, or a variable that stores a String. This is the symbol on the tape that fills theoretical space on the tape where the input is not.
+- The `final_states` argument is a Set. This can be either a Set in the argument, or a variable that stores a Set.
+
 ### Functions
 
 #### `save(path[optional], input_string[optional], horizontal[optional])`
 
 The `save()` function can only be used when calling it on an automata variable already assigned, i.e. `fa.save()`.
 
 When executed, this function will, by default, save the automata object's graph to a file named after the variable name, i.e. `fa.png`.
```

### Comparing `automython-1.1.2/README.md` & `automython-1.2.0/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,8 +1,49 @@
-# Automython
+Metadata-Version: 2.1
+Name: automython
+Version: 1.2.0
+Summary: A simplistic programming language interpreter to Python to help students grasp finite automata theory programmatically and with a computed graph through visualization libraries.
+Home-page: https://github.com/mkantrr/automython
+Author: Matthew Kanter
+Author-email: Matthew Kanter <matt@matutu.dev>
+Maintainer-email: Matthew Kanter <matt@matutu.dev>
+License: The MIT License (MIT)
+        
+        Copyright (c) 2024 Matthew Kanter
+        
+        Permission is hereby granted, free of charge, to any person obtaining a copy
+        of this software and associated documentation files (the "Software"), to deal
+        in the Software without restriction, including without limitation the rights
+        to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+        copies of the Software, and to permit persons to whom the Software is
+        furnished to do so, subject to the following conditions:
+        
+        The above copyright notice and this permission notice shall be included in
+        all copies or substantial portions of the Software.
+        
+        THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+        IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+        FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+        AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+        LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+        OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
+        THE SOFTWARE.
+Keywords: automata,finite,compiler,interpreter,theory,computational theory,non-deterministic,turing,machine,state
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+License-File: LICENSE.txt
+Requires-Dist: automata-lib[visual]>=8.2.0
+Requires-Dist: pandas>=2.2.0
+Requires-Dist: ipython>=8.22.2
+Requires-Dist: forbiddenfruit>=0.1.4
+
+# Automython (v1.2.0)
 
 *Copyright 2024 Matthew Kanter*  
 *Released under the MIT license*
 
 [![build](https://github.com/mkantrr/automython/actions/workflows/build.yml/badge.svg)](https://github.com/mkantrr/automythonactions/workflows/build.yml)
 
 ## [`https://pypi.org/project/automython`](https://pypi.org/project/automython)
@@ -94,14 +135,18 @@
 
 Dictioniaries in Automython act the same as `dict`s in Python. The only difference in the more limited support types for what you can assign to keys to only Automython's "native" types, and no other Python types that are not included.
 
 #### Set
 
 Sets in Automython act the same as `set`s in Python. The only difference in the more limited support types for what you can assign to keys to only Automython's "native" types, and no other Python types that are not included.
 
+#### Tuple
+
+Tuples in Automython act the same as `tuple`s in Python. The only difference is the more limited support, as you cannot perform most of the Python tuple functions and slick scripting you can here. They are built for a specific purpose, and it is moreso to be integrated with the computational theory concepts below.
+
 #### DFA
 **Deterministic Finite Automaton**:
 
 The DFA object in Automython must resemble this syntax:
 ```python
 DFA(states, input_symbols, transitions, initial_state, final_states, allow_partial[optional]: bool)
 ```
@@ -131,14 +176,34 @@
 
 - The `states` argument is a Set. This can be either a Set in the argument, or a variable that stores a Set.
 - The `input_symbols` argument is a Set. This can be either a Set in the argument, or a variable that stores a Set.
 - The `transitions` argument is a Dictionary. This can be either a Dictionary in the argument, or a variable that stores a Dictionary. The values of each key maps to an input symbol as a key to a Set of states.
 - The `initial_state` argument is a String. This can be either a String in the argument, or a variable that stores a String.
 - The `final_states` argument is a Set. This can be either a Set in the argument, or a variable that stores a Set.
 
+#### DTM
+**Deterministic Turing Machine**:
+
+The DFA object in Automython must resemble this syntax:
+```python
+DTM(states, input_symbols, tape_symbols, transitions, initial_state, blank_symbol, final_states)
+```
+It must **also** be assigned to a variable; it cannot be treated as an expression, i.e.:
+```python
+dtm = DTM(states, input_symbols, tape_symbols, transitions, initial_state, blank_symbol, final_states)
+```
+
+- The `states` argument is a Set. This can be either a Set in the argument, or a variable that stores a Set.
+- The `input_symbols` argument is a Set. This can be either a Set in the argument, or a variable that stores a Set. These symbols are all Strings, and are the only symbols that can exist on the tape before the Turing machine begins its run.
+- The `tape_symbols` argument is a Set. This can be either a Set in the argument, or a variable that stores a Set. These symbols are all Strings that are able to be read and written on the tape.
+- The `transitions` argument is a Dictionary. This can be either a Dictionary in the argument, or a variable that stores a Dictionary. The values of each key maps to an input symbol as a key to a Tuple of strings denoting the new state, write symbol, and direction to move on the tape.
+- The `initial_state` argument is a String. This can be either a String in the argument, or a variable that stores a String.
+- The `blank_symbol` argument is a String. This can be either a String in the argument, or a variable that stores a String. This is the symbol on the tape that fills theoretical space on the tape where the input is not.
+- The `final_states` argument is a Set. This can be either a Set in the argument, or a variable that stores a Set.
+
 ### Functions
 
 #### `save(path[optional], input_string[optional], horizontal[optional])`
 
 The `save()` function can only be used when calling it on an automata variable already assigned, i.e. `fa.save()`.
 
 When executed, this function will, by default, save the automata object's graph to a file named after the variable name, i.e. `fa.png`.
```

### Comparing `automython-1.1.2/pyproject.toml` & `automython-1.2.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "automython"
-version = "1.1.2"
+version = "1.2.0"
 description = "A simplistic programming language interpreter to Python to help students grasp finite automata theory programmatically and with a computed graph through visualization libraries."
 readme = "README.md"
 requires-python = ">=3.8"
 keywords = ['automata', "finite", 'compiler', 'interpreter', 'theory', 'computational theory', "non-deterministic", "turing", "machine", "state"]
 license = {file = 'LICENSE.txt'}
 authors = [
     {name = 'Matthew Kanter', email = 'matt@matutu.dev'}
```

### Comparing `automython-1.1.2/setup.py` & `automython-1.2.0/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,30 +5,30 @@
 HERE = pathlib.Path(__file__).parent
 
 # The text of the README file
 README = (HERE / "README.md").read_text()
 
 setup(
     name='automython',
-    version='1.1.2',
+    version='1.2.0',
     description='A simplistic programming language interpreter to Python to help students grasp finite automata theory programmatically and with a computed graph through visualization libraries.',
     long_description=README,
     long_description_content_type='text/markdown',
     url='https://github.com/mkantrr/automython',
     author='Matthew Kanter',
     author_email='matt@matutu.dev',
     license='MIT',
     keywords=['automata', "finite", 'compiler', 'interpreter', 'theory', 'computational theory', "non-deterministic", "turing", "machine", "state"],
     classifiers=[
         "License :: OSI Approved :: MIT License",
         "Programming Language :: Python :: 3",
         "Operating System :: OS Independent"
     ],
-    package_dir={'':'src'},
-    packages=find_packages('src'),
+    package_dir={'':'automython'},
+    packages=find_packages('automython'),
     install_requires=[
         "automata-lib[visual]",
         "pandas",
         "ipython",
         "forbiddenfruit"
     ],
     entry_points={
```

### Comparing `automython-1.1.2/src/automython.egg-info/PKG-INFO` & `automython-1.2.0/automython/automython.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: automython
-Version: 1.1.2
+Version: 1.2.0
 Summary: A simplistic programming language interpreter to Python to help students grasp finite automata theory programmatically and with a computed graph through visualization libraries.
 Home-page: https://github.com/mkantrr/automython
 Author: Matthew Kanter
 Author-email: Matthew Kanter <matt@matutu.dev>
 Maintainer-email: Matthew Kanter <matt@matutu.dev>
 License: The MIT License (MIT)
         
@@ -35,15 +35,15 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 Requires-Dist: automata-lib[visual]>=8.2.0
 Requires-Dist: pandas>=2.2.0
 Requires-Dist: ipython>=8.22.2
 Requires-Dist: forbiddenfruit>=0.1.4
 
-# Automython
+# Automython (v1.2.0)
 
 *Copyright 2024 Matthew Kanter*  
 *Released under the MIT license*
 
 [![build](https://github.com/mkantrr/automython/actions/workflows/build.yml/badge.svg)](https://github.com/mkantrr/automythonactions/workflows/build.yml)
 
 ## [`https://pypi.org/project/automython`](https://pypi.org/project/automython)
@@ -135,14 +135,18 @@
 
 Dictioniaries in Automython act the same as `dict`s in Python. The only difference in the more limited support types for what you can assign to keys to only Automython's "native" types, and no other Python types that are not included.
 
 #### Set
 
 Sets in Automython act the same as `set`s in Python. The only difference in the more limited support types for what you can assign to keys to only Automython's "native" types, and no other Python types that are not included.
 
+#### Tuple
+
+Tuples in Automython act the same as `tuple`s in Python. The only difference is the more limited support, as you cannot perform most of the Python tuple functions and slick scripting you can here. They are built for a specific purpose, and it is moreso to be integrated with the computational theory concepts below.
+
 #### DFA
 **Deterministic Finite Automaton**:
 
 The DFA object in Automython must resemble this syntax:
 ```python
 DFA(states, input_symbols, transitions, initial_state, final_states, allow_partial[optional]: bool)
 ```
@@ -172,14 +176,34 @@
 
 - The `states` argument is a Set. This can be either a Set in the argument, or a variable that stores a Set.
 - The `input_symbols` argument is a Set. This can be either a Set in the argument, or a variable that stores a Set.
 - The `transitions` argument is a Dictionary. This can be either a Dictionary in the argument, or a variable that stores a Dictionary. The values of each key maps to an input symbol as a key to a Set of states.
 - The `initial_state` argument is a String. This can be either a String in the argument, or a variable that stores a String.
 - The `final_states` argument is a Set. This can be either a Set in the argument, or a variable that stores a Set.
 
+#### DTM
+**Deterministic Turing Machine**:
+
+The DFA object in Automython must resemble this syntax:
+```python
+DTM(states, input_symbols, tape_symbols, transitions, initial_state, blank_symbol, final_states)
+```
+It must **also** be assigned to a variable; it cannot be treated as an expression, i.e.:
+```python
+dtm = DTM(states, input_symbols, tape_symbols, transitions, initial_state, blank_symbol, final_states)
+```
+
+- The `states` argument is a Set. This can be either a Set in the argument, or a variable that stores a Set.
+- The `input_symbols` argument is a Set. This can be either a Set in the argument, or a variable that stores a Set. These symbols are all Strings, and are the only symbols that can exist on the tape before the Turing machine begins its run.
+- The `tape_symbols` argument is a Set. This can be either a Set in the argument, or a variable that stores a Set. These symbols are all Strings that are able to be read and written on the tape.
+- The `transitions` argument is a Dictionary. This can be either a Dictionary in the argument, or a variable that stores a Dictionary. The values of each key maps to an input symbol as a key to a Tuple of strings denoting the new state, write symbol, and direction to move on the tape.
+- The `initial_state` argument is a String. This can be either a String in the argument, or a variable that stores a String.
+- The `blank_symbol` argument is a String. This can be either a String in the argument, or a variable that stores a String. This is the symbol on the tape that fills theoretical space on the tape where the input is not.
+- The `final_states` argument is a Set. This can be either a Set in the argument, or a variable that stores a Set.
+
 ### Functions
 
 #### `save(path[optional], input_string[optional], horizontal[optional])`
 
 The `save()` function can only be used when calling it on an automata variable already assigned, i.e. `fa.save()`.
 
 When executed, this function will, by default, save the automata object's graph to a file named after the variable name, i.e. `fa.png`.
```

### Comparing `automython-1.1.2/src/interpret/Buffer.py` & `automython-1.2.0/automython/interpret/Buffer.py`

 * *Files identical despite different names*

### Comparing `automython-1.1.2/src/interpret/Lexer.py` & `automython-1.2.0/automython/interpret/Lexer.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 VAR = 'VARIABLE'
 LITERAL = 'LITERAL'
 INTEGER = 'INTEGER'
 BOOLEAN = 'BOOLEAN'
 PRINT = 'PRINT'
 DFA = 'DFA'
 NFA = 'NFA'
+DTM = 'DTM'
 FUNCTION_CALL = 'FUNCTION_CALL'
 
 class TokenError(ValueError):
     """ The expected token cannot be found """
     def __init__(self, msg=""):
         self.msg = msg
         super().__init__(self.msg)
@@ -70,14 +71,18 @@
         if dfa:
             return dfa
         
         nfa = self._process_nfa()
         if nfa:
             return nfa
         
+        dtm = self._process_dtm()
+        if dtm:
+            return dtm
+        
         func_name = self._process_func_name()
         if func_name:
             return func_name
 
         boolean = self._process_boolean()
         if boolean:
             return boolean
@@ -231,14 +236,30 @@
 
         token_string = match.group()[:-1]
 
         return self._set_current_token_and_skip(
             token.Token(NFA, token_string)
         )
         
+    def _process_dtm(self):
+        regexp = re.compile(r"\b(DTM\()")
+        
+        match = regexp.match(
+            self._text_storage.tail
+        )
+
+        if not match:
+            return None
+
+        token_string = match.group()[:-1]
+
+        return self._set_current_token_and_skip(
+            token.Token(DTM, token_string)
+        )
+        
     def _process_func_name(self):
         matches = self.func_names() 
 
         for i in matches:
             if i:         
                 token_string = i.group()[:-1]
```

### Comparing `automython-1.1.2/src/interpret/Parser.py` & `automython-1.2.0/automython/interpret/Parser.py`

 * *Files 9% similar despite different names*

```diff
@@ -113,18 +113,16 @@
     def __init__(self, value):
         self.value = str(value)
     
 class DictionaryNode(ValueNode):
     node_type = 'dictionary'
     
     def __init__(self, dict):
-        self.elements = dict
-        for key, value in self.elements.items():
-            self.key = key
-            self.value = value
+        self.key = dict[0]
+        self.value = dict[1]
     def asdict(self):
         return {
             'type': self.node_type,
             'key':  self.key.asdict(), 
             'value': self.value.asdict()
         }
         
@@ -138,14 +136,29 @@
             self.elements.append(element.asdict())
         
     def asdict(self):
         return {
             'type': self.node_type,
             'value': self.elements
         }
+        
+class TupleNode(ValueNode):
+    node_type = 'tuple'
+    
+    def __init__(self, list):
+        self.value = list
+        self.elements = []
+        for element in self.value:
+            self.elements.append(element.asdict())
+        
+    def asdict(self):
+        return {
+            'type': self.node_type,
+            'value': tuple(self.elements)
+        }
 
 class ParametersNode(ValueNode):
     node_type = 'parameters'
     
     def __init__(self, list):
         self.value = list
         self.elements = []
@@ -184,14 +197,29 @@
         
     def asdict(self):
         return {
             'type': self.node_type,
             'value': self.elements
         }
         
+class DTMNode(ValueNode):
+    node_type = 'dtm'
+    
+    def __init__(self, list):
+        self.value = list
+        self.elements = []
+        for element in self.value:
+            self.elements.append(element.asdict())
+        
+    def asdict(self):
+        return {
+            'type': self.node_type,
+            'value': self.elements
+        }
+        
 class Parser:
 
     def __init__(self):
         self.lexer = fa_lex.Lexer()
         
     def _allow_whitespace(self):
         t = self.lexer.peek_token()
@@ -307,15 +335,17 @@
        
         t = self.lexer.peek_token()
         func_t = self.lexer.peek_token(2)
         if func_t.type == fa_lex.LITERAL and func_t.value == '.':
             value = self.parse_function()
         elif t.type == fa_lex.DFA or t.type == fa_lex.NFA:
             value = self.parse_fa()
-        elif t.type == fa_lex.LITERAL and t.value == '{':
+        elif t.type == fa_lex.DTM:
+            value = self.parse_tm()
+        elif t.type == fa_lex.LITERAL and (t.value == '{' or t.value == '('):
             value = self.parse_collection()
         else:
             value = self.parse_expression()
             
         if not value or t == token.Token(fa_lex.EOL) or t == token.Token(fa_lex.EOF):
             raise fa_lex.SyntaxError(
                 'Assignment has undefined value at line {}'.format(
@@ -453,26 +483,45 @@
                 'Unexpected value \'{}\' at line {}'.format(
                     t.value, self.lexer.line
                 )
             )
                 
         return left 
     
+    def parse_tuple(self, collection=None):
+        with self.lexer:
+            self._parse_literal(['('])
+            left = self.parse_expression()
+            if collection == None:
+                collection = []
+            collection.append(left)
+            self._parse_literal([','])
+            self._allow_whitespace()
+            collection = self.parse_tuple(collection)
+            self._parse_literal([')'])
+            return collection
+        
+        left = self.parse_expression() 
+        return left
+    
     def parse_dictionary(self):
-        key = self.parse_expression()
+        key = self.parse_tuple()
         
         with self.lexer:
             self.lexer.discard(token.Token(fa_lex.LITERAL, ':'))
             t = self._allow_whitespace() 
-            if t.type == fa_lex.LITERAL and t.value == '{':
+            if t.type == fa_lex.LITERAL and (t.value == '{' or t.value == '('):
                 value = self.parse_collection()
             else:
                 value = self.parse_expression() 
                 
-            key = DictionaryNode({key: value})
+            if type(key) == list:
+                key = DictionaryNode((TupleNode(key), value)) 
+            else:
+                key = DictionaryNode((key, value))
             
         return key
          
     def parse_elements(self, collection=None):
         left = self.parse_dictionary() 
         if collection == None:
             collection = []     
@@ -492,24 +541,32 @@
             with self.lexer:
                 self._parse_literal(['{'])
                 self._allow_whitespace()
                 collection = self.parse_elements()
                 self._allow_whitespace()
                 self._parse_literal(['}'])
                 return CollectionNode(collection)
+        elif t.type == fa_lex.LITERAL and t.value == '(':
+            with self.lexer:
+                self._parse_literal(['('])
+                self._allow_whitespace()
+                collection = self.parse_elements()
+                self._allow_whitespace()
+                self._parse_literal([')'])
+                return TupleNode(collection)
         else:
             raise fa_lex.SyntaxError(
                 'Unexpected value \'{}\' at line {}'.format(
                     t.value, self.lexer.line
                 )
             )
        
     def parse_parameters(self, parameters=None):
         t = self.lexer.peek_token()
-        if t.type == fa_lex.LITERAL and t.value == '{':
+        if t.type == fa_lex.LITERAL and (t.value == '{' or t.value == '('):
             left = self.parse_collection()
         else:
             left = self.parse_expression()
         if parameters == None:
             parameters = []     
         parameters.append(left)
         
@@ -543,14 +600,33 @@
                 self._parse_literal(['('])
                 self._allow_whitespace()
                 parameters = self.parse_parameters()
                 self._allow_whitespace()
                 self._parse_literal([')'])
                 return NFANode(parameters) 
             
+    def parse_tm(self):
+        t = self.lexer.get_token() 
+        
+        if t.type not in [fa_lex.DTM]:
+            raise fa_lex.SyntaxError(
+                'Unexpected value \'{}\', not a supported Automython TM at line {}'.format(
+                    t.value, self.lexer.line
+                )
+            )
+        
+        if t.type == fa_lex.DTM:
+            with self.lexer:
+                self._parse_literal(['('])
+                self._allow_whitespace()
+                parameters = self.parse_parameters()
+                self._allow_whitespace()
+                self._parse_literal([')'])
+                return DTMNode(parameters) 
+            
     def parse_line(self):
         node = None
         
         with self.lexer:
             node = self.parse_standalone_func()
             
         with self.lexer:
```

### Comparing `automython-1.1.2/src/interpret/Token.py` & `automython-1.2.0/automython/interpret/Token.py`

 * *Files identical despite different names*

### Comparing `automython-1.1.2/src/interpret/Visitor.py` & `automython-1.2.0/automython/interpret/Visitor.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import interpret.helpers as helpers
+import pandas as pd
 
 class Visitor:
   def __init__(self):
       self.variables = {}
       self.printables = []
       self.DFAs = {}
       self.NFAs = {}
@@ -77,14 +78,22 @@
             return collection, 'dictionary'
         else:
             collection = set()
             for element in node['value']:
                 right_value, right_type = self.visit_helper(element)
                 collection.add(right_value)
             return collection, node['type']
+        
+    if node['type'] == 'tuple':
+        collection = list()
+        for element in node['value']:
+           right_value, right_type = self.visit_helper(element) 
+           collection.append(right_value)
+        collection = tuple(collection)
+        return collection, node['type']
     
     if node['type'] == 'parameters':
         collection = list()
         for element in node['value']:
             right_value, right_type = self.visit_helper(element)
             collection.append(right_value)
         return collection, node['type']
@@ -179,27 +188,56 @@
             )
         except Exception as e:
             print()
             print(str(e))
             return None, None
         
         return parameters, node['type']
+    
+    if node['type'] == 'dtm':
+        parameters = list()
+        for element in node['value']:
+            right_value, right_type = self.visit_helper(element)
+            parameters.append(right_value)
+           
+        try: 
+            parameters = helpers.make_DTM(
+                parameters[0],
+                parameters[1],
+                parameters[2],
+                parameters[3],
+                parameters[4],
+                parameters[5],
+                parameters[6]
+            )
+        except Exception as e:
+            print()
+            print(str(e))
+            return None, None
+        
+        return parameters, node['type']
         
     if node['type'] == 'assignment':
         right_value, right_type = self.visit_helper(node['value'])
-        if right_value != None and right_type != None:
-            if right_type == 'dfa':
-                self.DFAs[node['variable']] = {
-                    'value': right_value,
-                    'type': right_type
-                }
-            if right_type == 'nfa':
-                self.NFAs[node['variable']] = {
-                    'value': right_value,
-                    'type': right_type
-                } 
-            self.variables[node['variable']] = {
-                'value': right_value,
-                'type': right_type
-            }
+        if type(right_value) != pd.DataFrame:
+            if right_value != None and right_type != None:
+                if right_type == 'dfa':
+                    self.DFAs[node['variable']] = {
+                        'value': right_value,
+                        'type': right_type
+                    }
+                if right_type == 'nfa':
+                    self.NFAs[node['variable']] = {
+                        'value': right_value,
+                        'type': right_type
+                    } 
+                if right_type == 'dtm':
+                    self.DTMs[node['variable']] = {
+                        'value': right_value,
+                        'type': right_type
+                    }
+        self.variables[node['variable']] = {
+            'value': right_value,
+            'type': right_type
+        }
 
         return None, None
```

### Comparing `automython-1.1.2/src/interpret/cli.py` & `automython-1.2.0/automython/interpret/cli.py`

 * *Files 11% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 from IPython.display import display
 
 def cli():
     parser = fa_parse.Parser()
     visitor = fa_visitor.Visitor()
    
-    print('Automython 1.1.2 on ' + str(helpers.system_type())) 
+    print('Automython 1.2.0 on ' + str(helpers.system_type())) 
     print('Enter/Paste your content. Ctrl-D (i.e. EOF) to end input block.')
     while True:
         text = ''
         while True:
             try:
                 line = input('>>> ')
                 if (line in ['exit', 'quit']):
@@ -58,13 +58,15 @@
                         t = parser.lexer.get_token()
                     t = parser.lexer.peek_token()
                 
         for i in visitor.printables:
             if type(i['print_func']['value']) == tuple:
                 if i['print_func']['value'][1] == 'ipython_display':
                     display(i['print_func']['value'][0])
+                else:
+                    print(i['print_func']['value'])
             else:
                 print(i['print_func']['value'])
         visitor.printables = []
         
 if __name__ == '__main__':
     cli()
```

### Comparing `automython-1.1.2/src/interpret/file_interface.py` & `automython-1.2.0/automython/interpret/file_interface.py`

 * *Files 8% similar despite different names*

```diff
@@ -41,25 +41,27 @@
             t = parser.lexer.get_token()
           t = parser.lexer.peek_token()
         
     for i in visitor.printables:
       if type(i['print_func']['value']) == tuple:
         if i['print_func']['value'][1] == 'ipython_display':
           display(i['print_func']['value'][0])
+        else:
+          print(i['print_func']['value'])
       else:
         print(i['print_func']['value'])
     visitor.printables = []
           
     error_flag = False
     
   except EOFError:
     sys.exit(0)
   
   except Exception as ex:
-    print()
+    raise ex
     template = "An exception of type {0} occurred:\n{1!r}"
     message = template.format(type(ex).__name__, ex.args[0])
     print(message)
     
   if error_flag:
     sys.exit(1)
```

### Comparing `automython-1.1.2/src/interpret/helpers.py` & `automython-1.2.0/automython/interpret/helpers.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from automata.fa.dfa import DFA
 from automata.fa.nfa import NFA
 from automata.tm.dtm import DTM
 from automata.tm.ntm import NTM
 from automata.tm.mntm import MNTM
+import interpret.tm_helpers as tm_helpers
 
 import random
 import copy
 from forbiddenfruit import curse
 from typing import Union
 import pandas as pd
 import subprocess, os, platform
@@ -18,18 +19,21 @@
 
 
 def system_type():
     return platform.system()
   
 def definition(*args):
     target_fa = args[0]
+    table = None
     if isinstance(target_fa, DFA):
         table = make_dfa_table(target_fa)
     elif isinstance(target_fa, NFA):
         table = make_nfa_table(target_fa)
+    elif isinstance(target_fa, tm_helpers.VisualDTM):
+        table = make_dtm_table(target_fa)
     return table
 
 #https://github.com/lewiuberg/visual-automata/blob/master/visual_automata/fa/nfa.py
 def make_dfa_table(target_fa) -> pd.DataFrame:
     initial_state = target_fa.initial_state
     final_states = target_fa.final_states
 
@@ -111,14 +115,59 @@
                     cell = "{" + ",".join(cell) + "}"
                 row[input_symbol] = cell
             table[state] = row
 
         table = pd.DataFrame.from_dict(table).fillna("∅").T
         table = table.reindex(sorted(table.columns), axis=1)
         return table
+    
+def make_dtm_table(target_fa) -> pd.DataFrame:
+    initial_state = target_fa.dtm.initial_state
+    final_states = target_fa.dtm.final_states
+
+    table = {}
+
+    for from_state, (to_state, write_symbol, direction), read_symbol in target_fa.iter_transitions():
+        # Prepare nice string for from_state
+        if isinstance(from_state, frozenset):
+            from_state_str = str(set(from_state))
+        else:
+            from_state_str = str(from_state)
+
+        if from_state in final_states:
+            from_state_str = "*" + from_state_str
+        if from_state == initial_state:
+            from_state_str = "→" + from_state_str
+
+        # Prepare nice string for to_state
+        if isinstance(to_state, frozenset):
+            to_state_str = str(set(to_state))
+        else:
+            to_state_str = str(to_state)
+
+        if to_state in final_states:
+            to_state_str = "*" + to_state_str
+
+        # Prepare nice symbol
+        if read_symbol == "":
+            read_symbol = "λ"
+        if write_symbol == "":
+            write_symbol = "λ"
+
+        from_state_dict = table.setdefault(from_state_str, dict())
+        from_state_dict.setdefault(to_state_str, set()).add(read_symbol + "/" + write_symbol + "," + direction)
+
+    # Reformat table for singleton sets
+    for symbol_dict in table.values():
+        for symbol in symbol_dict:
+            if len(symbol_dict[symbol]) == 1:
+                symbol_dict[symbol] = symbol_dict[symbol].pop()
+
+    df = pd.DataFrame.from_dict(table).fillna("∅").T
+    return df.reindex(sorted(df.columns), axis=1)
 
 #https://github.com/lewiuberg/visual-automata/blob/master/visual_automata/fa/nfa.py
 def _nfa_add_lambda(all_transitions: dict) -> dict:
         """
         Replacing '' key name for empty string (lambda/epsilon) transitions.
 
         Args:
@@ -153,14 +202,27 @@
        states=states,
        input_symbols=input_symbols,
        transitions=transitions,
        initial_state=initial_state,
        final_states=final_states 
     )
     
+def make_DTM(states, input_symbols, tape_symbols, transitions, initial_state, blank_symbol, final_states):
+    dtm = DTM(
+        states=states,
+        input_symbols=input_symbols,
+        tape_symbols=tape_symbols,
+        transitions=transitions,
+        initial_state=initial_state,
+        blank_symbol=blank_symbol,
+        final_states=final_states 
+    )
+    dtm = tm_helpers.VisualDTM(dtm)
+    return dtm
+    
 def open(filename): 
     if str(filename).lower().endswith(('.png', '.jpg', '.jpeg', '.svg', '.pdf')):
         try:
             if platform.system() == 'Darwin':       # macOS
                 subprocess.check_call(('open', filename), stdout=subprocess.DEVNULL, stderr=subprocess.STDOUT)
             elif platform.system() == 'Windows':    # Windows
                 os.startfile(os.path.normpath(filename))
@@ -168,39 +230,45 @@
                 subprocess.check_call(('xdg-open', filename), stdout=subprocess.DEVNULL, stderr=subprocess.STDOUT) 
             return ("Opening " + str(filename) + "...")
         except Exception as ex:
             message = 'The file ' + os.path.normpath(filename) + ' does not exist.'
             return message
     else:
         return 'The file ' + os.path.normpath(filename) + ' is not an accepted file type to open.'
+   
 def save(*args):
   target_fa = args[0]
   path = args[1]
   if len(args) > 2:
     input_string = args[2]
     if len(args) > 3:
       horizontal = args[3]
       return target_fa.show_diagram(input_str=input_string, path=path, horizontal=horizontal)
     else:
       return target_fa.show_diagram(input_str=input_string, path=path)
   else:
       return target_fa.show_diagram(path=path)
-          
+  
 def test(*args):
     target_fa = args[0]
     input_string = args[1]
     #(transition_steps, accepted) = target_fa._get_input_path(input_string)
     if isinstance(target_fa, DFA):
         taken_steps = \
             _make_dfa_transition_walkthrough(target_fa, input_string)
         return (taken_steps, 'ipython_display')
     elif isinstance(target_fa, NFA):
         taken_steps = \
             _make_nfa_transition_walkthrough(target_fa, input_string)
         return (taken_steps, 'ipython_display')
+    elif isinstance(target_fa, tm_helpers.VisualDTM):
+        taken_steps = \
+            _make_dtm_transition_walkthrough(target_fa, input_string)
+        return (taken_steps, 'ipython_display')
+        
     #return_string = 'Steps taken:'
     #for i in transition_steps:
     #  return_string += "\n->" + " From " + str(i[0]) + " to " + str(i[1]) + " on " + str(i[2])
     #return_string += '\n'
     #if (accepted):
     #    return_string += '\nAccepted word!'
     #else:
@@ -494,7 +562,137 @@
             return path
         # No path obtained. Try again.
         else:
             if counter <= recursion_limit:
                 return _nfa_pathsearcher(nfa, input_str, status, counter)
             else:
                 return False
+            
+def _make_dtm_transition_walkthrough(target_fa, input_str: str, return_result=False) -> Union[bool, list, list]:
+        """
+        Checks if string of input symbols results in final state.
+
+        Args:
+            input_str (str): The input string to run on the DFA.
+            return_result (bool, optional): Returns results to the show_diagram method. Defaults to False.
+
+        Raises:
+            TypeError: To let the user know a string has to be entered.
+
+        Returns:
+            Union[bool, list, list]: If the last state is the final state, transition pairs, and steps taken.
+        """
+        if not isinstance(input_str, str):
+            raise TypeError(f"input_str should be a string. {input_str} is {type(input_str)}, not a string.")
+
+        current_state = target_fa.dtm.initial_state
+        transitions_taken = []
+        symbol_sequence: list = []
+        status: bool = True
+
+        transitions_path, status = target_fa.get_input_path(input_str=input_str)
+        
+        for transition_index, configuration_pair in enumerate(
+                transitions_path, start=1
+            ):
+            
+            prev_configuration = configuration_pair[0]
+            configuration = configuration_pair[1]
+            
+            from_state = prev_configuration.state
+            to_state = configuration.state
+            
+            if configuration.tape.current_position > prev_configuration.tape.current_position:
+                direction = 'R'
+            elif configuration.tape.current_position < prev_configuration.tape.current_position:
+                direction = 'L'
+            else:
+                direction = 'N'
+                
+            if direction == 'R':
+                write_symbol = configuration.tape.tape[configuration.tape.current_position - 1]
+                read_symbol = prev_configuration.tape.tape[configuration.tape.current_position - 1]
+            elif direction == 'L':
+                write_symbol = configuration.tape.tape[configuration.tape.current_position + 1]
+                read_symbol = prev_configuration.tape.tape[configuration.tape.current_position + 1]
+            else: 
+                write_symbol = configuration.tape.tape[configuration.tape.current_position]
+                read_symbol = prev_configuration.tape.tape[configuration.tape.current_position]
+            
+            transition = target_fa.get_edge_name(read_symbol) + "/" + target_fa.get_edge_name(write_symbol) + "," + direction
+            transitions_taken.append((from_state, to_state, transition))
+
+        taken_steps = _get_dtm_transition_steps(
+            target_fa=target_fa.dtm,
+            initial_state=target_fa.dtm.initial_state,
+            final_states=target_fa.dtm.final_states,
+            input_str=input_str,
+            transitions_taken=transitions_taken,
+            status=status,
+        )
+        if return_result:
+            return status, taken_steps
+        else:
+            return taken_steps  # .to_string(index=False)
+        
+def _get_dtm_transition_steps(target_fa, initial_state, final_states, input_str: str, transitions_taken: list, status: bool) -> pd.DataFrame:
+    initial_state = target_fa.initial_state
+    final_states = target_fa.final_states
+    
+    current_states = transitions_taken.copy()
+    for i, state in enumerate(current_states):
+        if (
+            state[0] == initial_state and state[0] in
+            final_states
+        ):
+            current_states[i] = "→*" + state[0]
+        elif state[0] == initial_state:
+            current_states[i] = "→" + state[0]
+        elif state[0] in final_states:
+            current_states[i] = "*" + state[0]
+        else:
+            current_states[i] = state[0]
+    current_states.insert(0, "")
+
+    new_states = transitions_taken.copy()
+    for i, state in enumerate(new_states):
+        if (
+            state[1] == initial_state and state[1] in
+            final_states
+        ):
+            new_states[i] = "→*" + state[1]
+        elif state[1] == initial_state:
+            new_states[i] = "→" + state[1]
+        elif state[1] in final_states:
+            new_states[i] = "*" + state[1]
+        else:
+            new_states[i] = state[1]
+    new_states.insert(0, current_states[1])
+            
+    #del current_states[-1]
+    #del new_states[0]
+    actions = [str(x[2]) for x in transitions_taken]
+    actions.insert(0,"$/$/R")
+
+    transition_steps: dict = {
+        "Current state:": current_states,
+        "Read/Write/Move:": actions,
+        "New state:": new_states,
+    }
+
+    transition_steps = pd.DataFrame.from_dict(
+        transition_steps
+    )
+    transition_steps.index += 1
+    transition_steps = pd.DataFrame.from_dict(
+        transition_steps
+    ).rename_axis("Step:", axis=1)
+    if status:
+        transition_steps.columns = pd.MultiIndex.from_product(
+            [[f'[DTM on \"{input_str}\" is Accepted!]'], transition_steps.columns]
+        )
+        return transition_steps
+    else:
+        transition_steps.columns = pd.MultiIndex.from_product(
+            [[f'[DTM on \"{input_str}\" is Rejected...]'], transition_steps.columns]
+        )
+        return transition_steps
```

### Comparing `automython-1.1.2/src/interpret/interpreter.py` & `automython-1.2.0/automython/interpret/interpreter.py`

 * *Files identical despite different names*

