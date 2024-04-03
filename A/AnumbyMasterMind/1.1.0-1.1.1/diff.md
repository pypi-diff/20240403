# Comparing `tmp/AnumbyMasterMind-1.1.0.tar.gz` & `tmp/AnumbyMasterMind-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\AnumbyMasterMind-1.1.0.tar", last modified: Wed Apr  3 12:06:17 2024, max compression
+gzip compressed data, was "dist\AnumbyMasterMind-1.1.1.tar", last modified: Wed Apr  3 12:41:44 2024, max compression
```

## Comparing `AnumbyMasterMind-1.1.0.tar` & `AnumbyMasterMind-1.1.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2024-04-03 12:06:17.086041 AnumbyMasterMind-1.1.0/
-drwxrwxrwx   0        0        0        0 2024-04-03 12:06:17.055515 AnumbyMasterMind-1.1.0/AnumbyMasterMind/
--rw-rw-rw-   0        0        0       25 2024-03-28 20:30:04.000000 AnumbyMasterMind-1.1.0/AnumbyMasterMind/__init__.py
--rw-rw-rw-   0        0        0    11471 2024-04-02 15:28:57.000000 AnumbyMasterMind-1.1.0/AnumbyMasterMind/__main__.py
-drwxrwxrwx   0        0        0        0 2024-04-03 12:06:17.085032 AnumbyMasterMind-1.1.0/AnumbyMasterMind.egg-info/
--rw-rw-rw-   0        0        0     1878 2024-04-03 12:06:16.000000 AnumbyMasterMind-1.1.0/AnumbyMasterMind.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      348 2024-04-03 12:06:16.000000 AnumbyMasterMind-1.1.0/AnumbyMasterMind.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-03 12:06:16.000000 AnumbyMasterMind-1.1.0/AnumbyMasterMind.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       68 2024-04-03 12:06:16.000000 AnumbyMasterMind-1.1.0/AnumbyMasterMind.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       39 2024-04-03 12:06:16.000000 AnumbyMasterMind-1.1.0/AnumbyMasterMind.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2024-04-03 12:06:16.000000 AnumbyMasterMind-1.1.0/AnumbyMasterMind.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       85 2024-03-28 20:15:18.000000 AnumbyMasterMind-1.1.0/LICENSE
--rw-rw-rw-   0        0        0        0 2024-03-28 20:16:04.000000 AnumbyMasterMind-1.1.0/MANIFEST.in
--rw-rw-rw-   0        0        0     1878 2024-04-03 12:06:17.086041 AnumbyMasterMind-1.1.0/PKG-INFO
--rw-rw-rw-   0        0        0     1342 2024-03-28 20:37:03.000000 AnumbyMasterMind-1.1.0/README.md
--rw-rw-rw-   0        0        0       42 2024-04-03 12:06:17.087040 AnumbyMasterMind-1.1.0/setup.cfg
--rw-rw-rw-   0        0        0     1088 2024-03-28 21:49:23.000000 AnumbyMasterMind-1.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-03 12:41:44.383134 AnumbyMasterMind-1.1.1/
+drwxrwxrwx   0        0        0        0 2024-04-03 12:41:44.356025 AnumbyMasterMind-1.1.1/AnumbyMasterMind/
+-rw-rw-rw-   0        0        0       25 2024-03-28 20:30:04.000000 AnumbyMasterMind-1.1.1/AnumbyMasterMind/__init__.py
+-rw-rw-rw-   0        0        0    11799 2024-04-03 12:39:39.000000 AnumbyMasterMind-1.1.1/AnumbyMasterMind/__main__.py
+drwxrwxrwx   0        0        0        0 2024-04-03 12:41:44.381047 AnumbyMasterMind-1.1.1/AnumbyMasterMind.egg-info/
+-rw-rw-rw-   0        0        0     1878 2024-04-03 12:41:44.000000 AnumbyMasterMind-1.1.1/AnumbyMasterMind.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      348 2024-04-03 12:41:44.000000 AnumbyMasterMind-1.1.1/AnumbyMasterMind.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-03 12:41:44.000000 AnumbyMasterMind-1.1.1/AnumbyMasterMind.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       68 2024-04-03 12:41:44.000000 AnumbyMasterMind-1.1.1/AnumbyMasterMind.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       39 2024-04-03 12:41:44.000000 AnumbyMasterMind-1.1.1/AnumbyMasterMind.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2024-04-03 12:41:44.000000 AnumbyMasterMind-1.1.1/AnumbyMasterMind.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       85 2024-03-28 20:15:18.000000 AnumbyMasterMind-1.1.1/LICENSE
+-rw-rw-rw-   0        0        0        0 2024-03-28 20:16:04.000000 AnumbyMasterMind-1.1.1/MANIFEST.in
+-rw-rw-rw-   0        0        0     1878 2024-04-03 12:41:44.383134 AnumbyMasterMind-1.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0     1342 2024-03-28 20:37:03.000000 AnumbyMasterMind-1.1.1/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-03 12:41:44.384059 AnumbyMasterMind-1.1.1/setup.cfg
+-rw-rw-rw-   0        0        0     1088 2024-03-28 21:49:23.000000 AnumbyMasterMind-1.1.1/setup.py
```

### Comparing `AnumbyMasterMind-1.1.0/AnumbyMasterMind/__main__.py` & `AnumbyMasterMind-1.1.1/AnumbyMasterMind/__main__.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,14 +23,15 @@
     """
     Interface pour la reconnaissance de caractères.
     Première implémentation avec la caméra intégrée au PC
     """
 
     def __init__(self):
         self.reader = easyocr.Reader(['fr'])  # Utiliser EasyOCR avec la langue anglaise
+        self.count = 0
         if mode_camera == internal_mode:
             self.width = 640
             self.height = 480
         else:
             #  initialisation socket udp
             self.s = socket.socket(socket.AF_INET, socket.SOCK_DGRAM)
             self.addr_port = ('192.168.4.1', 10086)  # ESP32-CAM address
@@ -50,32 +51,36 @@
     def esp32cam(self):
         try:
             self.s.sendto(self.color, self.addr_port)
             buf = self.s.recvfrom(50000)
             raw_img = np.asarray(bytearray(buf[0]), dtype=np.uint8)
             return raw_img
         except:          # timeout de réception de l'image
-            print('no image ', self.count)
+            # print('no image ', self.count)
             self.count += 1
             return None
 
         """
         r = requests.get("http://192.168.4.1:80/capture")
         image = np.asarray(bytearray(r.content), dtype=np.uint8)
         return cv2.imdecode(image, cv2.IMREAD_COLOR)
         """
 
     def read(self):
         if mode_camera == internal_mode:
             frame = self.internal_camera()
         else:
             frame = self.esp32cam()
+            # print("OCR::read>", frame)
 
-        frame = cv2.cvtColor(frame, cv2.COLOR_BGR2RGB)
-        return self.reader.readtext(frame), frame
+        if not frame is None:
+            frame = cv2.cvtColor(frame, cv2.COLOR_BGR2RGB)
+            return self.reader.readtext(frame), frame
+        else:
+            return None, None
 
 
 class Jeu:
     info_start = "Choisis une position"
 
     def __init__(self):
         self.info = Jeu.info_start
@@ -291,27 +296,31 @@
         self.draw_ihm(jeu.position)
 
         if jeu.position == -1:
             jeu.info = f"choisis une position"
         else:
             jeu.info = f"choisis un chiffre"
 
-        for (bbox, text, prob) in result:
-            if prob > 0.5 and contains_integer(text):
-                t = int(text)
-                if t > 0 and t <= N:
-                    # print("t=", t, "position=", jeu.position, "jeu=", jeu)
-                    if jeu.position >= 0:
-                        if self.valid(t):
-                            jeu.jeu[jeu.position] = t
-                            # print("process_frame. position=", self.position, "jeu=", jeu)
-                            jeu.info = f"chiffre {t} choisi"
-                        else:
-                            jeu.info = f"doublons interdits ({t})"
-                    self.draw_ihm(jeu.position)
+        if result is None:
+            jeu.info = f"pas d'image"
+            self.draw_ihm(jeu.position)
+        else:
+            for (bbox, text, prob) in result:
+                if prob > 0.5 and contains_integer(text):
+                    t = int(text)
+                    if t > 0 and t <= N:
+                        # print("t=", t, "position=", jeu.position, "jeu=", jeu)
+                        if jeu.position >= 0:
+                            if self.valid(t):
+                                jeu.jeu[jeu.position] = t
+                                # print("process_frame. position=", self.position, "jeu=", jeu)
+                                jeu.info = f"chiffre {t} choisi"
+                            else:
+                                jeu.info = f"doublons interdits ({t})"
+                        self.draw_ihm(jeu.position)
 
                     break
 
     def run(self):
         global mode_camera
 
         while True:
```

### Comparing `AnumbyMasterMind-1.1.0/AnumbyMasterMind.egg-info/PKG-INFO` & `AnumbyMasterMind-1.1.1/AnumbyMasterMind.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: AnumbyMasterMind
-Version: 1.1.0
+Version: 1.1.1
 Summary: Implémentation du jeu MasterMind pour être associé avec un Robot et une logique neuronale
 Home-page: https://github.com/anumby-source/AnumbyMasterMind
 Author: Chris Arnault
 Author-email: chris.arnault.1@gmail.com
 License: CeCILL-B
 Classifier: License :: CeCILL-B Free Software License Agreement (CECILL-B)
 Classifier: Programming Language :: Python :: 3
```

### Comparing `AnumbyMasterMind-1.1.0/PKG-INFO` & `AnumbyMasterMind-1.1.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: AnumbyMasterMind
-Version: 1.1.0
+Version: 1.1.1
 Summary: Implémentation du jeu MasterMind pour être associé avec un Robot et une logique neuronale
 Home-page: https://github.com/anumby-source/AnumbyMasterMind
 Author: Chris Arnault
 Author-email: chris.arnault.1@gmail.com
 License: CeCILL-B
 Classifier: License :: CeCILL-B Free Software License Agreement (CECILL-B)
 Classifier: Programming Language :: Python :: 3
```

### Comparing `AnumbyMasterMind-1.1.0/README.md` & `AnumbyMasterMind-1.1.1/README.md`

 * *Files identical despite different names*

### Comparing `AnumbyMasterMind-1.1.0/setup.py` & `AnumbyMasterMind-1.1.1/setup.py`

 * *Files identical despite different names*

