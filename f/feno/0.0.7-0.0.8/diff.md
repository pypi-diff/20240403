# Comparing `tmp/feno-0.0.7.tar.gz` & `tmp/feno-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "feno-0.0.7.tar", last modified: Wed Apr  3 01:45:43 2024, max compression
+gzip compressed data, was "feno-0.0.8.tar", last modified: Wed Apr  3 16:47:46 2024, max compression
```

## Comparing `feno-0.0.7.tar` & `feno-0.0.8.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 lion      (1000) lion      (1000)        0 2024-04-03 01:45:43.279912 feno-0.0.7/
--rw-r--r--   0 lion      (1000) lion      (1000)     1043 2024-03-26 18:23:42.000000 feno-0.0.7/LICENSE
--rw-r--r--   0 lion      (1000) lion      (1000)      191 2024-03-26 18:23:42.000000 feno-0.0.7/MANIFEST.in
--rw-r--r--   0 lion      (1000) lion      (1000)      918 2024-04-03 01:45:43.279912 feno-0.0.7/PKG-INFO
--rw-r--r--   0 lion      (1000) lion      (1000)       46 2024-03-27 17:52:43.000000 feno-0.0.7/README.md
--rw-r--r--   0 lion      (1000) lion      (1000)      319 2024-04-02 11:56:24.000000 feno-0.0.7/changelog.md
--rw-r--r--   0 lion      (1000) lion      (1000)      310 2024-03-27 17:54:40.000000 feno-0.0.7/requirements.txt
--rw-r--r--   0 lion      (1000) lion      (1000)       74 2024-04-03 01:45:43.279912 feno-0.0.7/setup.cfg
--rw-r--r--   0 lion      (1000) lion      (1000)     3107 2024-04-01 17:24:14.000000 feno-0.0.7/setup.py
-drwxr-xr-x   0 lion      (1000) lion      (1000)        0 2024-04-03 01:45:43.266579 feno-0.0.7/src/
-drwxr-xr-x   0 lion      (1000) lion      (1000)        0 2024-04-03 01:45:43.276579 feno-0.0.7/src/feno/
--rw-r--r--   0 lion      (1000) lion      (1000)       22 2024-04-03 01:45:25.000000 feno-0.0.7/src/feno/__init__.py
--rw-r--r--   0 lion      (1000) lion      (1000)     1861 2024-04-02 01:57:25.000000 feno-0.0.7/src/feno/__main__.py
--rw-r--r--   0 lion      (1000) lion      (1000)     5130 2024-04-02 12:05:39.000000 feno-0.0.7/src/feno/actions.py
--rw-r--r--   0 lion      (1000) lion      (1000)      550 2024-03-26 19:17:45.000000 feno-0.0.7/src/feno/cases.py
--rw-r--r--   0 lion      (1000) lion      (1000)     1699 2024-04-01 17:39:49.000000 feno-0.0.7/src/feno/check.py
--rw-r--r--   0 lion      (1000) lion      (1000)      938 2024-03-26 19:19:40.000000 feno-0.0.7/src/feno/css_style.py
--rw-r--r--   0 lion      (1000) lion      (1000)     4997 2024-04-03 01:36:37.000000 feno-0.0.7/src/feno/filter.py
--rw-r--r--   0 lion      (1000) lion      (1000)     6915 2024-04-02 01:52:43.000000 feno-0.0.7/src/feno/html.py
--rw-r--r--   0 lion      (1000) lion      (1000)     2494 2024-03-27 13:44:12.000000 feno-0.0.7/src/feno/indexer.py
--rw-r--r--   0 lion      (1000) lion      (1000)     3326 2024-03-27 13:09:44.000000 feno-0.0.7/src/feno/jsontools.py
--rw-r--r--   0 lion      (1000) lion      (1000)      393 2024-04-01 23:10:29.000000 feno-0.0.7/src/feno/log.py
--rw-r--r--   0 lion      (1000) lion      (1000)    10371 2024-04-02 12:07:04.000000 feno-0.0.7/src/feno/mdpp.py
--rw-r--r--   0 lion      (1000) lion      (1000)     4989 2024-04-01 23:31:38.000000 feno-0.0.7/src/feno/remote_md.py
--rw-r--r--   0 lion      (1000) lion      (1000)     1846 2024-04-03 01:37:08.000000 feno-0.0.7/src/feno/tree.py
-drwxr-xr-x   0 lion      (1000) lion      (1000)        0 2024-04-03 01:45:43.279912 feno-0.0.7/src/feno.egg-info/
--rw-r--r--   0 lion      (1000) lion      (1000)      918 2024-04-03 01:45:43.000000 feno-0.0.7/src/feno.egg-info/PKG-INFO
--rw-r--r--   0 lion      (1000) lion      (1000)      542 2024-04-03 01:45:43.000000 feno-0.0.7/src/feno.egg-info/SOURCES.txt
--rw-r--r--   0 lion      (1000) lion      (1000)        1 2024-04-03 01:45:43.000000 feno-0.0.7/src/feno.egg-info/dependency_links.txt
--rw-r--r--   0 lion      (1000) lion      (1000)      144 2024-04-03 01:45:43.000000 feno-0.0.7/src/feno.egg-info/entry_points.txt
--rw-r--r--   0 lion      (1000) lion      (1000)       55 2024-04-03 01:45:43.000000 feno-0.0.7/src/feno.egg-info/requires.txt
--rw-r--r--   0 lion      (1000) lion      (1000)        5 2024-04-03 01:45:43.000000 feno-0.0.7/src/feno.egg-info/top_level.txt
+drwxr-xr-x   0 lion      (1000) lion      (1000)        0 2024-04-03 16:47:46.179971 feno-0.0.8/
+-rw-r--r--   0 lion      (1000) lion      (1000)     1043 2024-03-26 18:23:42.000000 feno-0.0.8/LICENSE
+-rw-r--r--   0 lion      (1000) lion      (1000)      191 2024-03-26 18:23:42.000000 feno-0.0.8/MANIFEST.in
+-rw-r--r--   0 lion      (1000) lion      (1000)      918 2024-04-03 16:47:46.179971 feno-0.0.8/PKG-INFO
+-rw-r--r--   0 lion      (1000) lion      (1000)       46 2024-03-27 17:52:43.000000 feno-0.0.8/README.md
+-rw-r--r--   0 lion      (1000) lion      (1000)      374 2024-04-03 15:54:08.000000 feno-0.0.8/changelog.md
+-rw-r--r--   0 lion      (1000) lion      (1000)      310 2024-03-27 17:54:40.000000 feno-0.0.8/requirements.txt
+-rw-r--r--   0 lion      (1000) lion      (1000)       74 2024-04-03 16:47:46.179971 feno-0.0.8/setup.cfg
+-rw-r--r--   0 lion      (1000) lion      (1000)     3107 2024-04-01 17:24:14.000000 feno-0.0.8/setup.py
+drwxr-xr-x   0 lion      (1000) lion      (1000)        0 2024-04-03 16:47:46.166638 feno-0.0.8/src/
+drwxr-xr-x   0 lion      (1000) lion      (1000)        0 2024-04-03 16:47:46.173304 feno-0.0.8/src/feno/
+-rw-r--r--   0 lion      (1000) lion      (1000)       22 2024-04-03 16:47:40.000000 feno-0.0.8/src/feno/__init__.py
+-rw-r--r--   0 lion      (1000) lion      (1000)     1861 2024-04-02 01:57:25.000000 feno-0.0.8/src/feno/__main__.py
+-rw-r--r--   0 lion      (1000) lion      (1000)     5130 2024-04-02 12:05:39.000000 feno-0.0.8/src/feno/actions.py
+-rw-r--r--   0 lion      (1000) lion      (1000)      550 2024-03-26 19:17:45.000000 feno-0.0.8/src/feno/cases.py
+-rw-r--r--   0 lion      (1000) lion      (1000)     1699 2024-04-01 17:39:49.000000 feno-0.0.8/src/feno/check.py
+-rw-r--r--   0 lion      (1000) lion      (1000)      938 2024-03-26 19:19:40.000000 feno-0.0.8/src/feno/css_style.py
+-rw-r--r--   0 lion      (1000) lion      (1000)     4997 2024-04-03 01:36:37.000000 feno-0.0.8/src/feno/filter.py
+-rw-r--r--   0 lion      (1000) lion      (1000)     6915 2024-04-02 01:52:43.000000 feno-0.0.8/src/feno/html.py
+-rw-r--r--   0 lion      (1000) lion      (1000)     2494 2024-03-27 13:44:12.000000 feno-0.0.8/src/feno/indexer.py
+-rw-r--r--   0 lion      (1000) lion      (1000)     3326 2024-03-27 13:09:44.000000 feno-0.0.8/src/feno/jsontools.py
+-rw-r--r--   0 lion      (1000) lion      (1000)      393 2024-04-01 23:10:29.000000 feno-0.0.8/src/feno/log.py
+-rw-r--r--   0 lion      (1000) lion      (1000)    11193 2024-04-03 15:47:37.000000 feno-0.0.8/src/feno/mdpp.py
+-rw-r--r--   0 lion      (1000) lion      (1000)     4989 2024-04-01 23:31:38.000000 feno-0.0.8/src/feno/remote_md.py
+-rw-r--r--   0 lion      (1000) lion      (1000)     1846 2024-04-03 01:37:08.000000 feno-0.0.8/src/feno/tree.py
+drwxr-xr-x   0 lion      (1000) lion      (1000)        0 2024-04-03 16:47:46.176638 feno-0.0.8/src/feno.egg-info/
+-rw-r--r--   0 lion      (1000) lion      (1000)      918 2024-04-03 16:47:46.000000 feno-0.0.8/src/feno.egg-info/PKG-INFO
+-rw-r--r--   0 lion      (1000) lion      (1000)      542 2024-04-03 16:47:46.000000 feno-0.0.8/src/feno.egg-info/SOURCES.txt
+-rw-r--r--   0 lion      (1000) lion      (1000)        1 2024-04-03 16:47:46.000000 feno-0.0.8/src/feno.egg-info/dependency_links.txt
+-rw-r--r--   0 lion      (1000) lion      (1000)      144 2024-04-03 16:47:46.000000 feno-0.0.8/src/feno.egg-info/entry_points.txt
+-rw-r--r--   0 lion      (1000) lion      (1000)       55 2024-04-03 16:47:46.000000 feno-0.0.8/src/feno.egg-info/requires.txt
+-rw-r--r--   0 lion      (1000) lion      (1000)        5 2024-04-03 16:47:46.000000 feno-0.0.8/src/feno.egg-info/top_level.txt
```

### Comparing `feno-0.0.7/LICENSE` & `feno-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `feno-0.0.7/PKG-INFO` & `feno-0.0.8/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: feno
-Version: 0.0.7
+Version: 0.0.8
 Summary: feno: Flexible Exercise Notation Organizer
 Home-page: https://github.com/senapk/feno
 Author: David Sena Oliveira
 Author-email: sena@ufc.br
 Project-URL: Bug Reports, https://github.com/senapk/feno/issues
 Project-URL: Source, https://github.com/senapk/feno/
 Keywords: programming,learning
```

### Comparing `feno-0.0.7/setup.py` & `feno-0.0.8/setup.py`

 * *Files identical despite different names*

### Comparing `feno-0.0.7/src/feno/__main__.py` & `feno-0.0.8/src/feno/__main__.py`

 * *Files identical despite different names*

### Comparing `feno-0.0.7/src/feno/actions.py` & `feno-0.0.8/src/feno/actions.py`

 * *Files identical despite different names*

### Comparing `feno-0.0.7/src/feno/cases.py` & `feno-0.0.8/src/feno/cases.py`

 * *Files identical despite different names*

### Comparing `feno-0.0.7/src/feno/check.py` & `feno-0.0.8/src/feno/check.py`

 * *Files identical despite different names*

### Comparing `feno-0.0.7/src/feno/css_style.py` & `feno-0.0.8/src/feno/css_style.py`

 * *Files identical despite different names*

### Comparing `feno-0.0.7/src/feno/filter.py` & `feno-0.0.8/src/feno/filter.py`

 * *Files identical despite different names*

### Comparing `feno-0.0.7/src/feno/html.py` & `feno-0.0.8/src/feno/html.py`

 * *Files identical despite different names*

### Comparing `feno-0.0.7/src/feno/indexer.py` & `feno-0.0.8/src/feno/indexer.py`

 * *Files identical despite different names*

### Comparing `feno-0.0.7/src/feno/jsontools.py` & `feno-0.0.8/src/feno/jsontools.py`

 * *Files identical despite different names*

### Comparing `feno-0.0.7/src/feno/mdpp.py` & `feno-0.0.8/src/feno/mdpp.py`

 * *Files 7% similar despite different names*

```diff
@@ -139,14 +139,29 @@
         regex = r"\[\[" + tag + r"\]\].*?^(.*)^[\S ]*\[\[" + tag + r"\]\]"
         matches = re.finditer(regex, content, re.MULTILINE | re.DOTALL)
         for match in matches:
             return match.group(1)
         return ""
 
     @staticmethod
+    def rmcom(target: str, content: str) -> str:
+        com = "//"
+        if target.endswith(".py"):
+            com = "#"
+        if target.endswith(".puml"):
+            com = "'"
+        lines = content.split("\n")
+        output = []
+        for line in lines:
+            if not line.lstrip().startswith(com):
+                output.append(line)
+        return "\n".join(output)
+
+
+    @staticmethod
     def execute(content: str, target_dir, action: Action = Action.RUN) -> str:
         new_content = ""
         last = 0
 
         regex = r"<!-- load (\S*?) (\S*?) -->\n(.*?)<!-- load -->"
         matches = re.finditer(regex, content, re.MULTILINE | re.DOTALL)
         
@@ -158,14 +173,18 @@
 
             fenced: List[str] = [tag for tag in words if tag.startswith("fenced")]
             words = [tag for tag in words if not tag.startswith("fenced")]
 
             filter: List[str] = [tag for tag in words if tag.startswith("filter")]
             words = [tag for tag in words if not tag.startswith("filter")]
 
+            rmcom: List[str] = [tag for tag in words if tag.startswith("rmcom")]
+            words = [tag for tag in words if not tag.startswith("rmcom")]
+
+
             extract: List[str] = [tag for tag in words if tag.startswith("extract")]
             words = [tag for tag in words if not tag.startswith("extract")]
 
 
             ext = os.path.splitext(path)[1][1:]
             if len(words) > 0:
                 ext = words[0]
@@ -186,14 +205,19 @@
                     new_content += "\n```" + ext + "\n"
                 if os.path.isfile(abspath):
                     if len(filter) > 0:
                         data = Filter(path).process(open(abspath).read()) + "\n"
                         new_content += data
                         if data[-1] != "\n":
                             new_content += "\n"
+                    elif len(rmcom) > 0:
+                        data =  Load.rmcom(abspath, open(abspath).read()) + "\n"
+                        new_content += data
+                        if data[-1] != "\n":
+                            new_content += "\n"
                     elif len(extract) > 0:
                         tag = extract[0].split("=")[1]
                         data = Load.extract_between_tags(open(abspath).read(), tag)
                         new_content += data
                         if len(data) == 0 or data[-1] != "\n":
                             new_content += "\n"
                     else:
```

### Comparing `feno-0.0.7/src/feno/remote_md.py` & `feno-0.0.8/src/feno/remote_md.py`

 * *Files identical despite different names*

### Comparing `feno-0.0.7/src/feno/tree.py` & `feno-0.0.8/src/feno/tree.py`

 * *Files identical despite different names*

### Comparing `feno-0.0.7/src/feno.egg-info/PKG-INFO` & `feno-0.0.8/src/feno.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: feno
-Version: 0.0.7
+Version: 0.0.8
 Summary: feno: Flexible Exercise Notation Organizer
 Home-page: https://github.com/senapk/feno
 Author: David Sena Oliveira
 Author-email: sena@ufc.br
 Project-URL: Bug Reports, https://github.com/senapk/feno/issues
 Project-URL: Source, https://github.com/senapk/feno/
 Keywords: programming,learning
```

### Comparing `feno-0.0.7/src/feno.egg-info/SOURCES.txt` & `feno-0.0.8/src/feno.egg-info/SOURCES.txt`

 * *Files identical despite different names*

