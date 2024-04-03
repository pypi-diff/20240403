# Comparing `tmp/loggerjava-0.0.7.4.tar.gz` & `tmp/loggerjava-0.0.7.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "loggerjava-0.0.7.4.tar", last modified: Tue Apr  2 11:24:02 2024, max compression
+gzip compressed data, was "loggerjava-0.0.7.5.tar", last modified: Wed Apr  3 14:51:41 2024, max compression
```

## Comparing `loggerjava-0.0.7.4.tar` & `loggerjava-0.0.7.5.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 11:24:02.334785 loggerjava-0.0.7.4/
--rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-04-02 11:23:58.000000 loggerjava-0.0.7.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2676 2024-04-02 11:24:02.334785 loggerjava-0.0.7.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2153 2024-04-02 11:23:58.000000 loggerjava-0.0.7.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 11:24:02.334785 loggerjava-0.0.7.4/loggerjava/
--rw-r--r--   0 runner    (1001) docker     (127)    13411 2024-04-02 11:23:58.000000 loggerjava-0.0.7.4/loggerjava/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5152 2024-04-02 11:23:58.000000 loggerjava-0.0.7.4/loggerjava/loggerjava.py
--rw-r--r--   0 runner    (1001) docker     (127)     1614 2024-04-02 11:23:58.000000 loggerjava-0.0.7.4/loggerjava/test_loggerjava.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 11:24:02.334785 loggerjava-0.0.7.4/loggerjava.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2676 2024-04-02 11:24:02.000000 loggerjava-0.0.7.4/loggerjava.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      255 2024-04-02 11:24:02.000000 loggerjava-0.0.7.4/loggerjava.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-02 11:24:02.000000 loggerjava-0.0.7.4/loggerjava.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-02 11:24:02.000000 loggerjava-0.0.7.4/loggerjava.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      488 2024-04-02 11:23:58.000000 loggerjava-0.0.7.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-02 11:24:02.334785 loggerjava-0.0.7.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-04-02 11:23:58.000000 loggerjava-0.0.7.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 14:51:41.576277 loggerjava-0.0.7.5/
+-rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-04-03 14:51:31.000000 loggerjava-0.0.7.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2821 2024-04-03 14:51:41.576277 loggerjava-0.0.7.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2298 2024-04-03 14:51:31.000000 loggerjava-0.0.7.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 14:51:41.572276 loggerjava-0.0.7.5/loggerjava/
+-rw-r--r--   0 runner    (1001) docker     (127)    11694 2024-04-03 14:51:31.000000 loggerjava-0.0.7.5/loggerjava/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5198 2024-04-03 14:51:31.000000 loggerjava-0.0.7.5/loggerjava/loggerjava.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2571 2024-04-03 14:51:31.000000 loggerjava-0.0.7.5/loggerjava/test_loggerjava.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 14:51:41.576277 loggerjava-0.0.7.5/loggerjava.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2821 2024-04-03 14:51:41.000000 loggerjava-0.0.7.5/loggerjava.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      255 2024-04-03 14:51:41.000000 loggerjava-0.0.7.5/loggerjava.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 14:51:41.000000 loggerjava-0.0.7.5/loggerjava.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-03 14:51:41.000000 loggerjava-0.0.7.5/loggerjava.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      488 2024-04-03 14:51:31.000000 loggerjava-0.0.7.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-03 14:51:41.576277 loggerjava-0.0.7.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-04-03 14:51:31.000000 loggerjava-0.0.7.5/setup.py
```

### Comparing `loggerjava-0.0.7.4/LICENSE` & `loggerjava-0.0.7.5/LICENSE`

 * *Files identical despite different names*

### Comparing `loggerjava-0.0.7.4/PKG-INFO` & `loggerjava-0.0.7.5/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: loggerjava
-Version: 0.0.7.4
+Version: 0.0.7.5
 Summary: an easy logger outputs like java logs
 Author: HTony03
 Author-email: HTony03 <HTony03@foxmail.com>
 Project-URL: Homepage, https://github.com/HTony03/loggerjava
 Project-URL: Issues, https://github.com/HTony03/loggerjava/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -33,14 +33,16 @@
 [20:39:00] [main/ERROR]: test
 [20:39:00] [main/FATAL]: test
 ```
 
 ### Developing features
 - [ ] mutiple variable with different configs
 - [x] new config format
+- [ ] catch and format errors
+- [ ] override config once
 
 
 ### Config
 ```python
 import loggerjava
 loggerjava.config(**kwargs)
 """
@@ -71,14 +73,16 @@
 """
 ```
 using `logger.exportconfig()` to export your current config
 
 and using `logger.inportconfig(inputconfig)` to inport your config
 ### Versions
 
+`v0.0.7.5` edited the original log codes,adding "log" feature,add the fatalexit config
+
 `v0.0.7.2` adding the "fatalexit" feature,adding an easier log function(not completed)
 
 `v0.0.7.1` adding debug config,adding debug
 
 `v0.0.7` no actual updates, updating version num to ver x.x.x
 
 `0.0.6.1` update readme
```

### Comparing `loggerjava-0.0.7.4/README.md` & `loggerjava-0.0.7.5/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -18,14 +18,16 @@
 [20:39:00] [main/ERROR]: test
 [20:39:00] [main/FATAL]: test
 ```
 
 ### Developing features
 - [ ] mutiple variable with different configs
 - [x] new config format
+- [ ] catch and format errors
+- [ ] override config once
 
 
 ### Config
 ```python
 import loggerjava
 loggerjava.config(**kwargs)
 """
@@ -56,14 +58,16 @@
 """
 ```
 using `logger.exportconfig()` to export your current config
 
 and using `logger.inportconfig(inputconfig)` to inport your config
 ### Versions
 
+`v0.0.7.5` edited the original log codes,adding "log" feature,add the fatalexit config
+
 `v0.0.7.2` adding the "fatalexit" feature,adding an easier log function(not completed)
 
 `v0.0.7.1` adding debug config,adding debug
 
 `v0.0.7` no actual updates, updating version num to ver x.x.x
 
 `0.0.6.1` update readme
```

### Comparing `loggerjava-0.0.7.4/loggerjava/__init__.py` & `loggerjava-0.0.7.5/loggerjava/__init__.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,163 +1,116 @@
 import time
+import loggerjava
+
 if __name__ == '__main__':
     pass
 
-ver = "v0.0.7.4"
+ver = "v0.0.7.5"
 name = "log"
 absolutepath = False
 showdetailedtime = False
 showinconsole = True
 filetype = ".log"
 file_encoding = "utf-8"
 route = r"log.log"
 debugin = False
 fatalclose = False
 
 
 # noinspection PyTypeChecker
-def debug(txt, pos="main"):
+def log(txt, type="i", pos="main", **overrides):
     """
         :param txt: the detail description of this log
+        :param type: the type of the log,using:debug,info,warn,error,fatal
         :param pos: show where the log's actual called positon in the code
-        :return: debug log
+        :return: log
         """
-    level = 'debug'
+    for configname, configdata in overrides.items():
+        pass
+    level = _formats.typeformat(type)
     if absolutepath:
         f = open(route, mode="at+", encoding=file_encoding)
     else:
         f = open(name + filetype, mode="at+", encoding=file_encoding)
     if showdetailedtime and showinconsole:
-        f.write(_output.format(time.asctime(), pos, level, txt))
-        print(_output.format(time.asctime(), pos, level, txt))
+        # noinspection PyTypeChecker
+        f.write(_formats.format(time.asctime(), pos, level, txt))
+        print(_formats.format(time.asctime(), pos, level, txt))
     elif not showdetailedtime and showinconsole:
-        f.write(_output.format(_output.time1(), pos, level, txt))
-        print(_output.format(_output.time1(), pos, level, txt))
+        f.write(_formats.format(_formats.time1(), pos, level, txt))
+        print(_formats.format(_formats.time1(), pos, level, txt))
     elif showdetailedtime and not showinconsole:
-        f.write(_output.format(time.asctime(), pos, level, txt))
+        f.write(_formats.format(time.asctime(), pos, level, txt))
     else:
-        f.write(_output.format(_output.time1(), pos, level, txt))
+        f.write(_formats.format(_formats.time1(), pos, level, txt))
     if debugin and not showdetailedtime:
-        return _output.format(_output.time1(), pos, level, txt)
+        return _formats.format(_formats.time1(), pos, level, txt)
     elif debugin and showdetailedtime:
-        return _output.format(time.asctime(), pos, level, txt)
+        return _formats.format(time.asctime(), pos, level, txt)
     f.close()
 
 
+def debug(txt, pos="main"):
+    """
+        :param txt: the detail description of this log
+        :param pos: show where the log's actual called positon in the code
+        :return: debug log
+        """
+    if debugin:
+        return log(txt, type='debug', pos=pos)
+    else:
+        log(txt, type='debug', pos=pos)
+
+
 def info(txt, pos="main"):
     """
         :param txt: the detail description of this log
         :param pos: show where the log's actual called positon in the code
         :return: info log
         """
-    level = 'INFO'
-    if absolutepath:
-        f = open(route, mode="at+", encoding=file_encoding)
-    else:
-        f = open(name + filetype, mode="at+", encoding=file_encoding)
-    if showdetailedtime and showinconsole:
-        # noinspection PyTypeChecker
-        f.write(_output.format(time.asctime(), pos, level, txt))
-        print(_output.format(time.asctime(), pos, level, txt))
-    elif not showdetailedtime and showinconsole:
-        f.write(_output.format(_output.time1(), pos, level, txt))
-        print(_output.format(_output.time1(), pos, level, txt))
-    elif showdetailedtime and not showinconsole:
-        f.write(_output.format(time.asctime(), pos, level, txt))
+    if debugin:
+        return log(txt, type='INFO', pos=pos)
     else:
-        f.write(_output.format(_output.time1(), pos, level, txt))
-    if debugin and not showdetailedtime:
-        return _output.format(_output.time1(), pos, level, txt)
-    elif debugin and showdetailedtime:
-        return _output.format(time.asctime(), pos, level, txt)
-    f.close()
+        return log(txt, type='INFO', pos=pos)
 
 
 def warn(txt, pos="main"):
     """
         :param txt: the detail description of this log
         :param pos: show where the log's actual called positon in the code
         :return: warning log
         """
-    level = 'WARN'
-    if absolutepath:
-        f = open(route, mode="at+", encoding=file_encoding)
+    if debugin:
+        return log(txt, type='WARN', pos=pos)
     else:
-        f = open(name + filetype, mode="at+", encoding=file_encoding)
-    if showdetailedtime and showinconsole:
-        f.write(_output.format(time.asctime(), pos, level, txt))
-        print(_output.format(time.asctime(), pos, level, txt))
-    elif not showdetailedtime and showinconsole:
-        f.write(_output.format(_output.time1(), pos, level, txt))
-        print(_output.format(_output.time1(), pos, level, txt))
-    elif showdetailedtime and not showinconsole:
-        f.write(_output.format(time.asctime(), pos, level, txt))
-    else:
-        f.write(_output.format(_output.time1(), pos, level, txt))
-    if debugin and not showdetailedtime:
-        return _output.format(_output.time1(), pos, level, txt)
-    elif debugin and showdetailedtime:
-        return _output.format(time.asctime(), pos, level, txt)
-    f.close()
+        log(txt, type='WARN', pos=pos)
 
 
 def error(txt, pos="main"):
     """
         :param txt: the detail description of this log
         :param pos: show where the log's actual called positon in the code
         :return: error log
         """
-    level = 'ERROR'
-    if absolutepath:
-        f = open(route, mode="at+", encoding=file_encoding)
+    if debugin:
+        return log(txt, type='ERROR', pos=pos)
     else:
-        f = open(name + filetype, mode="at+", encoding=file_encoding)
-    if showdetailedtime and showinconsole:
-        f.write(_output.format(time.asctime(), pos, level, txt))
-        print(_output.format(time.asctime(), pos, level, txt))
-    elif not showdetailedtime and showinconsole:
-        f.write(_output.format(_output.time1(), pos, level, txt))
-        print(_output.format(_output.time1(), pos, level, txt))
-    elif showdetailedtime and not showinconsole:
-        f.write(_output.format(time.asctime(), pos, level, txt))
-    else:
-        f.write(_output.format(_output.time1(), pos, level, txt))
-    if debugin and not showdetailedtime:
-        return _output.format(_output.time1(), pos, level, txt)
-    elif debugin and showdetailedtime:
-        return _output.format(time.asctime(), pos, level, txt)
-    f.close()
+        log(txt, type='ERROR', pos=pos)
 
 
 def fatal(txt, pos="main"):
     """
     :param txt: the detail description of this log
     :param pos: show where the log's actual called positon in the code
     :return: fatal log
     """
-    level = 'FATAL'
-    if absolutepath:
-        f = open(route, mode="at+", encoding=file_encoding)
-    else:
-        f = open(name + filetype, mode="at+", encoding=file_encoding)
-    if showdetailedtime and showinconsole:
-        f.write(_output.format(time.asctime(), pos, level, txt))
-        print(_output.format(time.asctime(), pos, level, txt))
-    elif not showdetailedtime and showinconsole:
-        f.write(_output.format(_output.time1(), pos, level, txt))
-        print(_output.format(_output.time1(), pos, level, txt))
-    elif showdetailedtime and not showinconsole:
-        f.write(_output.format(time.asctime(), pos, level, txt))
+    if debugin:
+        return log(txt, type='FATAL', pos=pos)
     else:
-        f.write(_output.format(_output.time1(), pos, level, txt))
-    if debugin and not showdetailedtime:
-        return _output.format(_output.time1(), pos, level, txt)
-    elif debugin and showdetailedtime:
-        return _output.format(time.asctime(), pos, level, txt)
-    f.close()
+        log(txt, type='FATAL', pos=pos)
     if fatalclose:
         exit(10)
 
 
 def config(**kwargs):
     """
     :param kwargs:input config names and config data
@@ -181,15 +134,15 @@
 
     showinconsole : whether to show the log in the python console
 
     fatalexit : whether to exit the program after a fatal log
 
     :return:
     """
-    global showinconsole, showdetailedtime, absolutepath, name, filetype, file_encoding, route,debugin
+    global showinconsole, showdetailedtime, absolutepath, name, filetype, file_encoding, route, debugin, fatalclose
     for configname, configdata in kwargs.items():
 
         if configname == "name":
             name = configdata
             f = open(name + filetype, mode="w", encoding=file_encoding)
             f.close()
 
@@ -204,101 +157,105 @@
             f.close()
 
         elif configname == "file_encoding":
             try:
                 if absolutepath:
                     tmpf = open(route, mode="w", encoding=configname)
                 else:
-                    tmpf = open(name+filetype, mode="w", encoding=configname)
+                    tmpf = open(name + filetype, mode="w", encoding=configname)
                 tmpf.close()
                 file_encoding = configname
                 del tmpf
                 if absolutepath:
                     f = open(route, mode="w", encoding=file_encoding)
                 else:
-                    f = open(name+filetype, mode="w", encoding=file_encoding)
+                    f = open(name + filetype, mode="w", encoding=file_encoding)
                 f.close()
             except LookupError:
                 warn("wrong file encoding config.this config is set to normal", pos="main_loggerjava")
                 file_encoding = "utf-8"
 
         elif configname == "showdetailedtime":
-            if configdata or not configdata:
+            if _formats.testformat(configdata, 1):
                 showdetailedtime = configdata
             else:
                 tmpin = showinconsole
                 showinconsole = True
                 warn("wrong detailed time config.this config is set to normal", pos="main_loggerjava")
                 showinconsole = tmpin
                 showdetailedtime = False
                 del tmpin
 
         elif configname == "showinconsole":
-            if configdata or not configdata:
+            if _formats.testformat(configdata, 1):
                 showinconsole = configdata
             else:
                 showinconsole = True
                 warn("wrong show in console config.this config is set to normal", pos="main_loggerjava")
 
         elif configname == "absolutepath":
-            if configdata or not configdata:
+            if _formats.testformat(configdata, 1):
                 absolutepath = configdata
                 if absolutepath:
                     f = open(route, mode="w", encoding=file_encoding)
                 else:
-                    f = open(name+filetype, mode="w", encoding=file_encoding)
+                    f = open(name + filetype, mode="w", encoding=file_encoding)
                 f.close()
             else:
                 tmpin = showinconsole
                 showinconsole = True
                 warn("wrong absolute path config.this config is set to normal", pos="main_loggerjava")
                 showinconsole = tmpin
                 absolutepath = False
                 f = open(name + filetype, mode="w", encoding=file_encoding)
                 f.close()
                 del tmpin
         elif configname == "debuging":
             debugin = configdata
         elif configname == "fatalexit":
-            if configdata or not configdata:
+            if _formats.testformat(configdata, 1):
                 fatalclose = configdata
             else:
                 warn("wrong fatal exit config.this config is set to normal", pos="main_loggerjava")
-                fatalclose = False                
+                fatalclose = False
 
 
 def version():
     """
     show the current version of loggerjava
     :return:
     """
     print("Current loggerjava ver:%s" % ver)
 
 
+def test():
+    loggerjava.test_loggerjava.testin()
+
+
 def exportconfig():
     """
     export current config
     use loadconfig(config) to load this exported config
     returning as a lib
     :return:
     """
     i = {"name": name, "filetype": filetype, "absolutepath": absolutepath,
          "route": route, "showdetailedtime": showdetailedtime, "showinconsole": showinconsole,
-         "file_encoding": file_encoding}
+         "file_encoding": file_encoding, "fatalexit": fatalclose}
     return i
 
 
 def loadconfig(inputconfig):
     """
     :param inputconfig: the config lib exported from exportconfig()
     :return:
     """
-    global name, showdetailedtime, showinconsole, absolutepath, filetype, file_encoding, route
+    global name, showdetailedtime, showinconsole, absolutepath, filetype, file_encoding, route, fatalclose
 
-    if inputconfig["absolutepath"] or not inputconfig["absolutepath"]:
+    if _formats.testformat(inputconfig["absolutepath"], 1):
         absolutepath = inputconfig["absolutepath"]
     else:
         tmpin = showinconsole
         showinconsole = True
         warn("wrong absolute path config.this config is set to normal", pos="main_loggerjava")
         showinconsole = tmpin
         absolutepath = False
@@ -322,41 +279,74 @@
 
     if absolutepath:
         f = open(route, mode="at+", encoding=file_encoding)
     else:
         f = open(name + filetype, mode="at+", encoding=file_encoding)
     f.close()
 
-    if inputconfig["showdetailedtime"] or not inputconfig["showdetailedtime"]:
+    if _formats.testformat(inputconfig["showdetailedtime"], 1):
         showdetailedtime = inputconfig["showdetailedtime"]
     else:
         tmpin = showinconsole
         showinconsole = True
         warn("wrong detailed time config.this config is set to normal", pos="main_loggerjava")
         showinconsole = tmpin
         showdetailedtime = False
         del tmpin
 
-    if inputconfig["showinconsole"] or not inputconfig["showinconsole"]:
+    if _formats.testformat(inputconfig["showinconsole"], 1):
         showinconsole = inputconfig["showinconsole"]
     else:
         showinconsole = True
         warn("wrong show in console config.this config is set to normal", pos="main_loggerjava")
 
+    if _formats.testformat(inputconfig["fatalexit"], 1):
+        fatalclose = inputconfig["fatalexit"]
+    else:
+        fatalclose = False
+        tmpin = showinconsole
+        showinconsole = True
+        warn("wrong fatal close config.this config is set to normal", pos="main_loggerjava")
+        showinconsole = tmpin
+        del tmpin
+
+
 # noinspection PyMethodParameters
 
 
-class _output:
+class _formats:
     def typeformat(type):
-        debugformat = ["D","d","DEBUG","debug"]
-        infoformat = ["I","i","INFO","info"]
+        debugformat = ["D", "d", "DEBUG", "debug"]
+        infoformat = ["I", "i", "INFO", "info"]
+        warnformat = ["W", "w", "WARN", "warn"]
+        errorformat = ["E", "e", "ERROR", "error"]
+        fatalformat = ["F", "f", "FATAL", "fatal"]
+
         if type in debugformat:
-            return "DEBUG"
+            return "debug"
         elif type in infoformat:
             return "INFO"
+        elif type in warnformat:
+            return "WARN"
+        elif type in errorformat:
+            return "ERROR"
+        elif type in fatalformat:
+            return "FATAL"
+        else:
+            warn("unknown given format", pos="main_loggerjava")
+            return "WARN"
+
+    def testformat(name, type):
+        if type == 1:
+            if name or not name:
+                return True
+            else:
+                return False
+        elif type == 2:
+            pass
 
     def format(time1, place, level, txt):
         return "[%s] [%s/%s]: %s\n" % (time1, place, level, txt)
 
     def time1():
         return str(time.localtime().tm_hour).rjust(2, "0") + ":" + \
             str(time.localtime().tm_min).rjust(2, "0") + ":" + str(time.localtime().tm_sec).rjust(2, "0")
```

### Comparing `loggerjava-0.0.7.4/loggerjava/loggerjava.py` & `loggerjava-0.0.7.5/loggerjava/loggerjava.py`

 * *Files 22% similar despite different names*

```diff
@@ -12,83 +12,83 @@
         self.showdetailedtime = False
         self.showinconsole = True
 
     def debug(self, txt, pos="main"):
         level = 'debug'
         f = open(self.name + ".log", "at+")
         if self.showdetailedtime and self.showinconsole:
-            f.write(self._output.format(time.asctime(), pos, level, txt))
-            print(self._output.format(time.asctime(), pos, level, txt))
+            f.write(self._formats.format(time.asctime(), pos, level, txt))
+            print(self._formats.format(time.asctime(), pos, level, txt))
         elif not self.showdetailedtime and self.showinconsole:
-            f.write(self._output.format(self._output.time1(), pos, level, txt))
-            print(self._output.format(self._output.time1(), pos, level, txt))
+            f.write(self._formats.format(self._formats.time1(), pos, level, txt))
+            print(self._formats.format(self._formats.time1(), pos, level, txt))
         elif self.showdetailedtime and not self.showinconsole:
-            f.write(self._output.format(time.asctime(), pos, level, txt))
+            f.write(self._formats.format(time.asctime(), pos, level, txt))
         else:
-            f.write(self._output.format(self._output.time1(), pos, level, txt))
+            f.write(self._formats.format(self._formats.time1(), pos, level, txt))
         f.close()
 
     def info(self, txt, pos="main"):
         level = 'INFO'
         f = open(self.name+".log", "at+")
         if self.showdetailedtime and self.showinconsole:
-            f.write(self._output.format(time.asctime(), pos, level, txt))
-            print(self._output.format(time.asctime(), pos, level, txt))
+            f.write(self._formats.format(time.asctime(), pos, level, txt))
+            print(self._formats.format(time.asctime(), pos, level, txt))
         elif not self.showdetailedtime and self.showinconsole:
-            f.write(self._output.format(self._output.time1(), pos, level, txt))
-            print(self._output.format(self._output.time1(), pos, level, txt))
+            f.write(self._formats.format(self._formats.time1(), pos, level, txt))
+            print(self._formats.format(self._formats.time1(), pos, level, txt))
         elif self.showdetailedtime and not self.showinconsole:
-            f.write(self._output.format(time.asctime(), pos, level, txt))
+            f.write(self._formats.format(time.asctime(), pos, level, txt))
         else:
-            f.write(self._output.format(self._output.time1(), pos, level, txt))
+            f.write(self._formats.format(self._formats.time1(), pos, level, txt))
         f.close()
 
     def warn(self, txt, pos="main"):
         level = 'WARN'
         f = open(self.name + ".log", "at+")
         if self.showdetailedtime and self.showinconsole:
-            f.write(self._output.format(time.asctime(), pos, level, txt))
-            print(self._output.format(time.asctime(), pos, level, txt))
+            f.write(self._formats.format(time.asctime(), pos, level, txt))
+            print(self._formats.format(time.asctime(), pos, level, txt))
         elif not self.showdetailedtime and self.showinconsole:
-            f.write(self._output.format(self._output.time1(), pos, level, txt))
-            print(self._output.format(self._output.time1(), pos, level, txt))
+            f.write(self._formats.format(self._formats.time1(), pos, level, txt))
+            print(self._formats.format(self._formats.time1(), pos, level, txt))
         elif self.showdetailedtime and not self.showinconsole:
-            f.write(self._output.format(time.asctime(), pos, level, txt))
+            f.write(self._formats.format(time.asctime(), pos, level, txt))
         else:
-            f.write(self._output.format(self._output.time1(), pos, level, txt))
+            f.write(self._formats.format(self._formats.time1(), pos, level, txt))
         f.close()
 
     def Error(self, txt, pos="main"):
         level = 'ERROR'
         f = open(self.name + ".log", "at+")
         if self.showdetailedtime and self.showinconsole:
-            f.write(self._output.format(time.asctime(), pos, level, txt))
-            print(self._output.format(time.asctime(), pos, level, txt))
+            f.write(self._formats.format(time.asctime(), pos, level, txt))
+            print(self._formats.format(time.asctime(), pos, level, txt))
         elif not self.showdetailedtime and self.showinconsole:
-            f.write(self._output.format(self._output.time1(), pos, level, txt))
-            print(self._output.format(self._output.time1(), pos, level, txt))
+            f.write(self._formats.format(self._formats.time1(), pos, level, txt))
+            print(self._formats.format(self._formats.time1(), pos, level, txt))
         elif self.showdetailedtime and not self.showinconsole:
-            f.write(self._output.format(time.asctime(), pos, level, txt))
+            f.write(self._formats.format(time.asctime(), pos, level, txt))
         else:
-            f.write(self._output.format(self._output.time1(), pos, level, txt))
+            f.write(self._formats.format(self._formats.time1(), pos, level, txt))
         f.close()
 
     def FATAL(self, txt, pos="main"):
         level = 'FATAL'
         f = open(self.name + ".log", "at+")
         if self.showdetailedtime and self.showinconsole:
-            f.write(self._output.format(time.asctime(), pos, level, txt))
-            print(self._output.format(time.asctime(), pos, level, txt))
+            f.write(self._formats.format(time.asctime(), pos, level, txt))
+            print(self._formats.format(time.asctime(), pos, level, txt))
         elif not self.showdetailedtime and self.showinconsole:
-            f.write(self._output.format(self._output.time1(), pos, level, txt))
-            print(self._output.format(self._output.time1(), pos, level, txt))
+            f.write(self._formats.format(self._formats.time1(), pos, level, txt))
+            print(self._formats.format(self._formats.time1(), pos, level, txt))
         elif self.showdetailedtime and not self.showinconsole:
-            f.write(self._output.format(time.asctime(), pos, level, txt))
+            f.write(self._formats.format(time.asctime(), pos, level, txt))
         else:
-            f.write(self._output.format(self._output.time1(), pos, level, txt))
+            f.write(self._formats.format(self._formats.time1(), pos, level, txt))
         f.close()
 
     def config(self, name="log", showdetailedtime=False, showinconsole=False):
         self.name = name
         f = open(self.name + ".log", "w")
         f.close()
         if not showdetailedtime or showdetailedtime:
@@ -99,15 +99,15 @@
         if not showinconsole or showinconsole:
             self.showinconsole = showinconsole
         else:
             print("wrong detailed time config\nthis config is set to normal")
             self.showinconsole = False
 
     # noinspection PyMethodParameters
-    class _output:
+    class _formats:
         def format(time1, place, level, txt):
             return "[%s] [%s/%s]: %s\n" % (time1, place, level, txt)
 
         def time1():
             return str(time.localtime().tm_hour).rjust(2, "0")+":" +\
                 str(time.localtime().tm_min).rjust(2, "0")+":"+str(time.localtime().tm_sec).rjust(2, "0")
```

### Comparing `loggerjava-0.0.7.4/loggerjava.egg-info/PKG-INFO` & `loggerjava-0.0.7.5/loggerjava.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: loggerjava
-Version: 0.0.7.4
+Version: 0.0.7.5
 Summary: an easy logger outputs like java logs
 Author: HTony03
 Author-email: HTony03 <HTony03@foxmail.com>
 Project-URL: Homepage, https://github.com/HTony03/loggerjava
 Project-URL: Issues, https://github.com/HTony03/loggerjava/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -33,14 +33,16 @@
 [20:39:00] [main/ERROR]: test
 [20:39:00] [main/FATAL]: test
 ```
 
 ### Developing features
 - [ ] mutiple variable with different configs
 - [x] new config format
+- [ ] catch and format errors
+- [ ] override config once
 
 
 ### Config
 ```python
 import loggerjava
 loggerjava.config(**kwargs)
 """
@@ -71,14 +73,16 @@
 """
 ```
 using `logger.exportconfig()` to export your current config
 
 and using `logger.inportconfig(inputconfig)` to inport your config
 ### Versions
 
+`v0.0.7.5` edited the original log codes,adding "log" feature,add the fatalexit config
+
 `v0.0.7.2` adding the "fatalexit" feature,adding an easier log function(not completed)
 
 `v0.0.7.1` adding debug config,adding debug
 
 `v0.0.7` no actual updates, updating version num to ver x.x.x
 
 `0.0.6.1` update readme
```

### Comparing `loggerjava-0.0.7.4/setup.py` & `loggerjava-0.0.7.5/setup.py`

 * *Files identical despite different names*

