# Comparing `tmp/bricka-0.3.3.tar.gz` & `tmp/bricka-0.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bricka-0.3.3.tar", max compression
+gzip compressed data, was "bricka-0.3.4.tar", max compression
```

## Comparing `bricka-0.3.3.tar` & `bricka-0.3.4.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1066 2024-03-27 17:34:43.752567 bricka-0.3.3/LICENSE
--rw-r--r--   0        0        0     7442 2024-03-27 17:34:43.752567 bricka-0.3.3/README.md
--rw-r--r--   0        0        0      681 2024-03-27 17:34:53.836496 bricka-0.3.3/pyproject.toml
--rw-r--r--   0        0        0        0 2024-03-27 17:34:43.756567 bricka-0.3.3/src/bricka/__init__.py
--rw-r--r--   0        0        0    18014 2024-03-27 17:34:43.756567 bricka-0.3.3/src/bricka/attrs.py
--rw-r--r--   0        0        0    16537 2024-03-27 17:34:43.756567 bricka-0.3.3/src/bricka/conflicts.py
--rw-r--r--   0        0        0    37850 2024-03-27 17:34:43.756567 bricka-0.3.3/src/bricka/elements.py
--rw-r--r--   0        0        0    22477 2024-03-27 17:34:43.756567 bricka-0.3.3/src/bricka/node.py
--rw-r--r--   0        0        0    35497 2024-03-27 17:34:43.756567 bricka-0.3.3/src/bricka/style.py
--rw-r--r--   0        0        0     6161 2024-03-27 17:34:43.756567 bricka-0.3.3/src/bricka/stylesheet.py
--rw-r--r--   0        0        0     7885 1970-01-01 00:00:00.000000 bricka-0.3.3/PKG-INFO
+-rw-r--r--   0        0        0     1066 2024-04-03 16:54:48.277924 bricka-0.3.4/LICENSE
+-rw-r--r--   0        0        0     7442 2024-04-03 16:54:48.281924 bricka-0.3.4/README.md
+-rw-r--r--   0        0        0      681 2024-04-03 16:54:58.973934 bricka-0.3.4/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-03 16:54:48.281924 bricka-0.3.4/src/bricka/__init__.py
+-rw-r--r--   0        0        0    18014 2024-04-03 16:54:48.281924 bricka-0.3.4/src/bricka/attrs.py
+-rw-r--r--   0        0        0    16537 2024-04-03 16:54:48.281924 bricka-0.3.4/src/bricka/conflicts.py
+-rw-r--r--   0        0        0    37850 2024-04-03 16:54:48.281924 bricka-0.3.4/src/bricka/elements.py
+-rw-r--r--   0        0        0    22481 2024-04-03 16:54:48.281924 bricka-0.3.4/src/bricka/node.py
+-rw-r--r--   0        0        0    35497 2024-04-03 16:54:48.281924 bricka-0.3.4/src/bricka/style.py
+-rw-r--r--   0        0        0     6161 2024-04-03 16:54:48.281924 bricka-0.3.4/src/bricka/stylesheet.py
+-rw-r--r--   0        0        0     7885 1970-01-01 00:00:00.000000 bricka-0.3.4/PKG-INFO
```

### Comparing `bricka-0.3.3/LICENSE` & `bricka-0.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `bricka-0.3.3/README.md` & `bricka-0.3.4/README.md`

 * *Files identical despite different names*

### Comparing `bricka-0.3.3/pyproject.toml` & `bricka-0.3.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "bricka"
-version = "0.3.3"
+version = "0.3.4"
 description = "Build reusable styled HTML components with python."
 authors = ["Said Atta <saidattaenp@yahoo.fr>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.11"
```

### Comparing `bricka-0.3.3/src/bricka/attrs.py` & `bricka-0.3.4/src/bricka/attrs.py`

 * *Files identical despite different names*

### Comparing `bricka-0.3.3/src/bricka/conflicts.py` & `bricka-0.3.4/src/bricka/conflicts.py`

 * *Files identical despite different names*

### Comparing `bricka-0.3.3/src/bricka/elements.py` & `bricka-0.3.4/src/bricka/elements.py`

 * *Files identical despite different names*

### Comparing `bricka-0.3.3/src/bricka/node.py` & `bricka-0.3.4/src/bricka/node.py`

 * *Files 0% similar despite different names*

```diff
@@ -267,18 +267,18 @@
         return name
       else:
         return ""
 
     if value is None:
       return ""
 
-    if self.attr_type(self.tag_name, name) == AttrType.URL:
-      return f'{name}="{urllib.parse.quote(value)}"' # type: ignore
-    else:  
-      return f'{name}="{html.escape(str(value), quote=True)}"'
+    # if self.attr_type(self.tag_name, name) == AttrType.URL:
+    #   return f'{name}="{urllib.parse.quote(value)}"' # type: ignore
+    # else:  
+    return f'{name}="{html.escape(str(value), quote=True)}"'
 
   def render_attrs(self) -> str:
     attrs: list[str] = []
     output = ""
     for key, value in self._attrs.items():
       if type(value) == dict:
         if key in PREFIXED_ATTRS:
```

### Comparing `bricka-0.3.3/src/bricka/style.py` & `bricka-0.3.4/src/bricka/style.py`

 * *Files identical despite different names*

### Comparing `bricka-0.3.3/src/bricka/stylesheet.py` & `bricka-0.3.4/src/bricka/stylesheet.py`

 * *Files identical despite different names*

### Comparing `bricka-0.3.3/PKG-INFO` & `bricka-0.3.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bricka
-Version: 0.3.3
+Version: 0.3.4
 Summary: Build reusable styled HTML components with python.
 License: MIT
 Author: Said Atta
 Author-email: saidattaenp@yahoo.fr
 Requires-Python: >=3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

