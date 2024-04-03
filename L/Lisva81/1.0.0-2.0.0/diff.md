# Comparing `tmp/Lisva81-1.0.0.tar.gz` & `tmp/Lisva81-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Lisva81-1.0.0.tar", last modified: Sat Feb 24 05:12:50 2024, max compression
+gzip compressed data, was "Lisva81-2.0.0.tar", last modified: Mon Apr  1 05:43:39 2024, max compression
```

## Comparing `Lisva81-1.0.0.tar` & `Lisva81-2.0.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-02-24 05:12:50.421805 Lisva81-1.0.0/
--rw-rw-rw-   0        0        0     1235 2023-04-13 20:26:37.000000 Lisva81-1.0.0/LICENSE
-drwxrwxrwx   0        0        0        0 2024-02-24 05:12:50.368802 Lisva81-1.0.0/Lisva81/
--rw-rw-rw-   0        0        0     5016 2024-02-24 05:11:52.000000 Lisva81-1.0.0/Lisva81/__init__.py
--rw-rw-rw-   0        0        0       75 2024-02-24 05:09:43.000000 Lisva81-1.0.0/Lisva81/version.py
-drwxrwxrwx   0        0        0        0 2024-02-24 05:12:50.410804 Lisva81-1.0.0/Lisva81.egg-info/
--rw-rw-rw-   0        0        0      992 2024-02-24 05:12:47.000000 Lisva81-1.0.0/Lisva81.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      245 2024-02-24 05:12:48.000000 Lisva81-1.0.0/Lisva81.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-02-24 05:12:47.000000 Lisva81-1.0.0/Lisva81.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       22 2024-02-24 05:12:47.000000 Lisva81-1.0.0/Lisva81.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-02-24 05:12:47.000000 Lisva81-1.0.0/Lisva81.egg-info/top_level.txt
--rw-rw-rw-   0        0        0        2 2024-02-24 05:12:47.000000 Lisva81-1.0.0/Lisva81.egg-info/zip-safe
--rw-rw-rw-   0        0        0      992 2024-02-24 05:12:50.418805 Lisva81-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0      638 2023-04-25 04:32:36.000000 Lisva81-1.0.0/README.md
--rw-rw-rw-   0        0        0       42 2024-02-24 05:12:50.423805 Lisva81-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0     1605 2024-02-24 05:09:28.000000 Lisva81-1.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-01 05:43:39.742524 Lisva81-2.0.0/
+-rw-rw-rw-   0        0        0     1235 2023-04-13 20:26:37.000000 Lisva81-2.0.0/LICENSE
+drwxrwxrwx   0        0        0        0 2024-04-01 05:43:39.676520 Lisva81-2.0.0/Lisva81/
+-rw-rw-rw-   0        0        0     5654 2024-04-01 05:42:26.000000 Lisva81-2.0.0/Lisva81/__init__.py
+-rw-rw-rw-   0        0        0       75 2024-04-01 05:42:42.000000 Lisva81-2.0.0/Lisva81/version.py
+drwxrwxrwx   0        0        0        0 2024-04-01 05:43:39.732523 Lisva81-2.0.0/Lisva81.egg-info/
+-rw-rw-rw-   0        0        0      992 2024-04-01 05:43:37.000000 Lisva81-2.0.0/Lisva81.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      245 2024-04-01 05:43:38.000000 Lisva81-2.0.0/Lisva81.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-01 05:43:37.000000 Lisva81-2.0.0/Lisva81.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       22 2024-04-01 05:43:37.000000 Lisva81-2.0.0/Lisva81.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-04-01 05:43:37.000000 Lisva81-2.0.0/Lisva81.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0        2 2024-04-01 05:43:37.000000 Lisva81-2.0.0/Lisva81.egg-info/zip-safe
+-rw-rw-rw-   0        0        0      992 2024-04-01 05:43:39.739523 Lisva81-2.0.0/PKG-INFO
+-rw-rw-rw-   0        0        0      638 2023-04-25 04:32:36.000000 Lisva81-2.0.0/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-01 05:43:39.743523 Lisva81-2.0.0/setup.cfg
+-rw-rw-rw-   0        0        0     1605 2024-02-24 05:09:28.000000 Lisva81-2.0.0/setup.py
```

### Comparing `Lisva81-1.0.0/LICENSE` & `Lisva81-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `Lisva81-1.0.0/Lisva81/__init__.py` & `Lisva81-2.0.0/Lisva81/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -44,14 +44,16 @@
 
 def printl(text):
     init()
     print(Fore.GREEN + text,end='\r')
 
 def make_session(type,id):
     session = requests.Session()
+    if type=="rv":
+        return session
     resp = requests.post("http://apiserver.alwaysdata.net/session",json={"type":type,"id":id},headers={'Content-Type':'application/json'})
     data = json.loads(resp.text)
     session.cookies.update(data)
     return session
 
 def wait_download(url,ichunk=0,index=0,file=None,session=None):
     init()
@@ -62,14 +64,20 @@
         total_size = int(data[0])
         ids = data[1]
         filename = data[2].split("?")[-1]
         values = data[2].split("?"+filename)[0].split("?")
         type = "r"
         id = ""
         host = f"https://cujae.edu.cu/index.php/r/$$$call$$$/api/file/file-api/download-file?submissionFileId=*&submissionId={ids}&stageId=1"
+    elif "revgacetaestudiantil.sld" in dl:
+        filename = dl.split("/")[-1]
+        total_size = int(dl.split("/"+filename)[0].split("/")[-1])
+        url = dl.split("/"+size)[0]
+        type = "rv"
+        id = 0
     else:
         url = dl.split("{")[0]+".file"
         filename = dl.split("/")[-1]
         id = dl.split("{")[1].split("}")[0]
         total_size = int(dl.split("}/")[1].split("/")[0])
         type = "uo"
 
@@ -117,15 +125,18 @@
             i+=1
             if parte==totals:
                 total_size = chunk_por
     f.close()
     if os.path.exists('Lisva81/' + filename):
         os.unlink('Lisva81/' + filename)
     shutil.move(filename,'Lisva81/'+filename)
-        
+    if "revgacetaestudiantil.sld" in dl:
+        with open('Lisva81/dwnl' + filename, "wb") as filet:
+            filet.write(open(f, "rb").read().replace(b"\x89PNG\r\n\x1a\n\x00\x00\x00\rIHDR\x00\x00\x00\x01\x00\x00\x00\x01\x08\x02\x00\x00\x00\x90wS\xde\x00\x00\x00\x0cIDATx\x9cc```\x00\x00\x00\x04\x00\x01\xf6\x178U\x00\x00\x00\x00IEND\xaeB`\x82",b''))
+        os.unlink(f)
     os.system(cmd)
     printl('Descarga Finalizada !!! Archivos Guardados en ./Downloads. Envie 0 y luego Enter para salir o pulse solo Enter para continuar')
     state = 'finish'
     a = input()
     if a == '0':
         if state == 'finish':
             return False,i,chunk_por,file,session
```

### Comparing `Lisva81-1.0.0/Lisva81.egg-info/PKG-INFO` & `Lisva81-2.0.0/Lisva81.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Lisva81
-Version: 1.0.0
+Version: 2.0.0
 Summary: Python 3 library for short text
 Home-page: https://github.com/fenixinvitado2021/downfree
 Author: RayServer
 Author-email: susej.mabel2009@gmail.com
 License: The Unlicense (Unlicense)
 Keywords: telegram,download,stream,bots
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `Lisva81-1.0.0/PKG-INFO` & `Lisva81-2.0.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Lisva81
-Version: 1.0.0
+Version: 2.0.0
 Summary: Python 3 library for short text
 Home-page: https://github.com/fenixinvitado2021/downfree
 Author: RayServer
 Author-email: susej.mabel2009@gmail.com
 License: The Unlicense (Unlicense)
 Keywords: telegram,download,stream,bots
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `Lisva81-1.0.0/README.md` & `Lisva81-2.0.0/README.md`

 * *Files identical despite different names*

### Comparing `Lisva81-1.0.0/setup.py` & `Lisva81-2.0.0/setup.py`

 * *Files identical despite different names*

