# Comparing `tmp/cipherspy-0.2.0.tar.gz` & `tmp/cipherspy-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cipherspy-0.2.0.tar", last modified: Mon Jan  1 00:36:12 2024, max compression
+gzip compressed data, was "cipherspy-0.3.1.tar", last modified: Wed Apr  3 03:40:00 2024, max compression
```

## Comparing `cipherspy-0.2.0.tar` & `cipherspy-0.3.1.tar`

### file list

```diff
@@ -1,18 +1,20 @@
-drwxr-xr-x   0 fathi     (1000) fathi     (1000)        0 2024-01-01 00:36:12.873061 cipherspy-0.2.0/
--rw-r--r--   0 fathi     (1000) fathi     (1000)     1073 2023-09-09 20:47:12.000000 cipherspy-0.2.0/LICENSE
--rw-r--r--   0 fathi     (1000) fathi     (1000)      784 2024-01-01 00:36:12.873061 cipherspy-0.2.0/PKG-INFO
--rw-r--r--   0 fathi     (1000) fathi     (1000)       11 2023-09-09 20:16:15.000000 cipherspy-0.2.0/README.md
-drwxr-xr-x   0 fathi     (1000) fathi     (1000)        0 2024-01-01 00:36:12.869061 cipherspy-0.2.0/cipherspy/
--rw-r--r--   0 fathi     (1000) fathi     (1000)        0 2023-09-09 20:13:32.000000 cipherspy-0.2.0/cipherspy/__init__.py
-drwxr-xr-x   0 fathi     (1000) fathi     (1000)        0 2024-01-01 00:36:12.873061 cipherspy-0.2.0/cipherspy/cipher/
--rw-r--r--   0 fathi     (1000) fathi     (1000)      213 2023-12-31 21:41:08.000000 cipherspy-0.2.0/cipherspy/cipher/__init__.py
--rw-r--r--   0 fathi     (1000) fathi     (1000)     1547 2024-01-01 00:32:54.000000 cipherspy-0.2.0/cipherspy/cipher/affine.py
--rw-r--r--   0 fathi     (1000) fathi     (1000)     1307 2024-01-01 00:32:54.000000 cipherspy-0.2.0/cipherspy/cipher/caesar.py
--rw-r--r--   0 fathi     (1000) fathi     (1000)     3970 2024-01-01 00:32:54.000000 cipherspy-0.2.0/cipherspy/cipher/playfair.py
-drwxr-xr-x   0 fathi     (1000) fathi     (1000)        0 2024-01-01 00:36:12.870061 cipherspy-0.2.0/cipherspy.egg-info/
--rw-r--r--   0 fathi     (1000) fathi     (1000)      784 2024-01-01 00:36:12.000000 cipherspy-0.2.0/cipherspy.egg-info/PKG-INFO
--rw-r--r--   0 fathi     (1000) fathi     (1000)      292 2024-01-01 00:36:12.000000 cipherspy-0.2.0/cipherspy.egg-info/SOURCES.txt
--rw-r--r--   0 fathi     (1000) fathi     (1000)        1 2024-01-01 00:36:12.000000 cipherspy-0.2.0/cipherspy.egg-info/dependency_links.txt
--rw-r--r--   0 fathi     (1000) fathi     (1000)       10 2024-01-01 00:36:12.000000 cipherspy-0.2.0/cipherspy.egg-info/top_level.txt
--rw-r--r--   0 fathi     (1000) fathi     (1000)       38 2024-01-01 00:36:12.873061 cipherspy-0.2.0/setup.cfg
--rw-r--r--   0 fathi     (1000) fathi     (1000)     1002 2024-01-01 00:32:54.000000 cipherspy-0.2.0/setup.py
+drwxr-xr-x   0 fathi     (1000) fathi     (1000)        0 2024-04-03 03:40:00.340365 cipherspy-0.3.1/
+-rw-r--r--   0 fathi     (1000) fathi     (1000)     1073 2024-02-28 20:35:30.000000 cipherspy-0.3.1/LICENSE
+-rw-r--r--   0 fathi     (1000) fathi     (1000)      782 2024-04-03 03:40:00.339365 cipherspy-0.3.1/PKG-INFO
+-rw-r--r--   0 fathi     (1000) fathi     (1000)       11 2024-02-28 20:35:30.000000 cipherspy-0.3.1/README.md
+drwxr-xr-x   0 fathi     (1000) fathi     (1000)        0 2024-04-03 03:40:00.336365 cipherspy-0.3.1/cipherspy/
+-rw-r--r--   0 fathi     (1000) fathi     (1000)        0 2024-02-28 20:35:30.000000 cipherspy-0.3.1/cipherspy/__init__.py
+drwxr-xr-x   0 fathi     (1000) fathi     (1000)        0 2024-04-03 03:40:00.339365 cipherspy-0.3.1/cipherspy/cipher/
+-rw-r--r--   0 fathi     (1000) fathi     (1000)      272 2024-04-03 03:05:33.000000 cipherspy-0.3.1/cipherspy/cipher/__init__.py
+-rw-r--r--   0 fathi     (1000) fathi     (1000)     2233 2024-04-03 03:33:54.000000 cipherspy-0.3.1/cipherspy/cipher/affine.py
+-rw-r--r--   0 fathi     (1000) fathi     (1000)     1537 2024-04-03 03:33:05.000000 cipherspy-0.3.1/cipherspy/cipher/caesar.py
+-rw-r--r--   0 fathi     (1000) fathi     (1000)     3473 2024-04-03 03:36:31.000000 cipherspy-0.3.1/cipherspy/cipher/hill.py
+-rw-r--r--   0 fathi     (1000) fathi     (1000)     4059 2024-04-03 03:34:15.000000 cipherspy-0.3.1/cipherspy/cipher/playfair.py
+-rw-r--r--   0 fathi     (1000) fathi     (1000)      164 2024-04-03 02:39:53.000000 cipherspy-0.3.1/cipherspy/exceptions.py
+drwxr-xr-x   0 fathi     (1000) fathi     (1000)        0 2024-04-03 03:40:00.337365 cipherspy-0.3.1/cipherspy.egg-info/
+-rw-r--r--   0 fathi     (1000) fathi     (1000)      782 2024-04-03 03:40:00.000000 cipherspy-0.3.1/cipherspy.egg-info/PKG-INFO
+-rw-r--r--   0 fathi     (1000) fathi     (1000)      341 2024-04-03 03:40:00.000000 cipherspy-0.3.1/cipherspy.egg-info/SOURCES.txt
+-rw-r--r--   0 fathi     (1000) fathi     (1000)        1 2024-04-03 03:40:00.000000 cipherspy-0.3.1/cipherspy.egg-info/dependency_links.txt
+-rw-r--r--   0 fathi     (1000) fathi     (1000)       10 2024-04-03 03:40:00.000000 cipherspy-0.3.1/cipherspy.egg-info/top_level.txt
+-rw-r--r--   0 fathi     (1000) fathi     (1000)       38 2024-04-03 03:40:00.340365 cipherspy-0.3.1/setup.cfg
+-rw-r--r--   0 fathi     (1000) fathi     (1000)     1000 2024-04-03 03:39:48.000000 cipherspy-0.3.1/setup.py
```

### Comparing `cipherspy-0.2.0/LICENSE` & `cipherspy-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `cipherspy-0.2.0/PKG-INFO` & `cipherspy-0.3.1/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: cipherspy
-Version: 0.2.0
+Version: 0.3.1
 Summary: Strong Passwords Generator made with python.
 Home-page: https://github.com/fathiabdelmalek/cipherspy.git
 Author: Fathi AbdelMalek
 Author-email: abdelmalek.fathi.2001@gmail.com
 License: OSI Approved :: MIT License
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: System Administrators
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Security
 Classifier: Topic :: Security :: Cryptography
-Requires-Python: >=3.6
+Requires-Python: >=3
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # cipher-py
```

### Comparing `cipherspy-0.2.0/cipherspy/cipher/affine.py` & `cipherspy-0.3.1/cipherspy/cipher/affine.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,52 +1,73 @@
-class AffineCipher:
-    def __init__(self, multiplier: int, shift: int):
-        self._multiplier = multiplier
-        self._shift = shift % 26
+from cipherspy.exceptions import NegativeNumberException
 
-    @property
-    def multiplier(self):
-        return self._multiplier
 
-    @multiplier.setter
-    def multiplier(self, multiplier: int):
-        self._multiplier = multiplier
+class AffineCipher:
+    def __init__(self, shift: int, multiplier: int):
+        super().__init__()
+        if shift <= 0:
+            raise NegativeNumberException(shift)
+        if multiplier <= 0:
+            raise NegativeNumberException(multiplier)
+        self._shift: int = shift % 26
+        self._multiplier: int = multiplier
 
     @property
-    def shift(self):
+    def shift(self) -> int:
         return self._shift
 
     @shift.setter
-    def shift(self, shift: int):
+    def shift(self, shift: int) -> None:
+        if shift <= 0:
+            raise NegativeNumberException(shift)
         self._shift = shift % 26
 
+    @property
+    def multiplier(self) -> int:
+        return self._multiplier
+
+    @multiplier.setter
+    def multiplier(self, multiplier: int) -> None:
+        if multiplier <= 0:
+            raise NegativeNumberException(multiplier)
+        self._multiplier = multiplier
+
     def _shift_char(self, char: chr):
         if char.isalpha():
             shifted = (self._multiplier * (ord(char) - ord('a')) + self._shift) % 26 + ord('a')
             if shifted > ord('z'):
                 shifted -= 26
             return chr(shifted)
         return char
 
     def encrypt(self, plaintext: str) -> str:
         encrypted_text = ''.join([self._shift_char(char) for char in plaintext.lower()])
         return encrypted_text
 
     def decrypt(self, ciphertext: str) -> str:
+        ciphertext = ciphertext.lower()
         self._shift = -self._shift
         decrypted_text = ''.join([self._shift_char(char) for char in ciphertext.lower()])
         self._shift = -self._shift
         return decrypted_text
 
 
 # Example usage:
 if __name__ == "__main__":
     base = 1
     shift = 2
-    message = "HELLO world 2024"
     cipher = AffineCipher(base, shift)
+
+    message = "HELLO world 2024"
+    print("Original message:", message)
+
     encrypted_message = cipher.encrypt(message)
+    print("Encrypted message:", encrypted_message)
+
     decrypted_message = cipher.decrypt(encrypted_message)
+    print("Decrypted message:", decrypted_message)
 
-    print("Original message:", message)
+    encrypted_message = cipher.encrypt(message)
     print("Encrypted message:", encrypted_message)
+
+    decrypted_message = cipher.decrypt(encrypted_message)
     print("Decrypted message:", decrypted_message)
```

### Comparing `cipherspy-0.2.0/cipherspy/cipher/caesar.py` & `cipherspy-0.3.1/cipherspy/cipher/caesar.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,44 +1,53 @@
+from cipherspy.exceptions import NegativeNumberException
+
+
 class CaesarCipher:
     def __init__(self, shift: int):
-        self._shift = shift % 26
+        super().__init__()
+        if shift <= 0:
+            raise NegativeNumberException(shift)
+        self._shift: int = shift % 26
 
     @property
-    def shift(self):
+    def shift(self) -> int:
         return self._shift
 
     @shift.setter
-    def shift(self, shift: int):
+    def shift(self, shift: int) -> None:
+        if shift <= 0:
+            raise NegativeNumberException(shift)
         self._shift = shift % 26
 
     def _shift_char(self, char: chr):
         if char.isalpha():
             shifted = ord(char) + self._shift
             if shifted > ord('z'):
                 shifted -= 26
             return chr(shifted)
         return char
 
     def encrypt(self, plaintext: str) -> str:
-        plaintext = plaintext.lower()
-        encrypted_text = ''.join([self._shift_char(char) for char in plaintext])
+        encrypted_text = ''.join([self._shift_char(char) for char in plaintext.lower()])
         return encrypted_text
 
     def decrypt(self, ciphertext: str) -> str:
         ciphertext = ciphertext.lower()
         self._shift = -self._shift
-        decrypted_text = ''.join([self._shift_char(char) for char in ciphertext])
+        decrypted_text = ''.join([self._shift_char(char) for char in ciphertext.lower()])
         self._shift = -self._shift
         return decrypted_text
 
 
 # Example usage:
 if __name__ == "__main__":
     shift = 3
-    message = "HELLO world 2023"
     cipher = CaesarCipher(shift)
-    encrypted_message = cipher.encrypt(message)
-    decrypted_message = cipher.decrypt(encrypted_message)
 
+    message = "HELLO world 2024"
     print("Original message:", message)
+
+    encrypted_message = cipher.encrypt(message)
     print("Encrypted message:", encrypted_message)
+
+    decrypted_message = cipher.decrypt(encrypted_message)
     print("Decrypted message:", decrypted_message)
```

### Comparing `cipherspy-0.2.0/cipherspy/cipher/playfair.py` & `cipherspy-0.3.1/cipherspy/cipher/playfair.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,42 +1,43 @@
 class PlayfairCipher:
-    def __init__(self, key: str):
-        self._key = self._prepare_key(key)
+
+    def __init__(self, key_str: str):
+        super().__init__()
+        self._key_str = self._prepare_key(key_str)
         self._matrix = self._generate_matrix()
 
     @property
-    def key(self):
-        return self._key
+    def key_str(self) -> str:
+        return self._key_str
 
-    @key.setter
-    def key(self, key: str):
-        self._key = self._prepare_key(key)
+    @key_str.setter
+    def key_str(self, key_str: str) -> None:
+        self._key_str = self._prepare_key(key_str)
         self._matrix = self._generate_matrix()
 
     @property
     def matrix(self):
         return self._matrix
 
-    def _prepare_key(self, key):
-        key = key.lower().replace("j", "i")
+    def _prepare_key(self, key_str: str) -> str:
         unique_chars = []
-        for char in key:
+        for char in key_str.lower().replace("j", "i"):
             if char not in unique_chars:
                 unique_chars.append(char)
         for char in "abcdefghiklmnopqrstuvwxyz":
             if char not in unique_chars:
                 unique_chars.append(char)
         return "".join(unique_chars)
 
     def _generate_matrix(self):
         matrix = [['' for _ in range(5)] for _ in range(5)]
         k = 0
         for i in range(5):
             for j in range(5):
-                matrix[i][j] = self._key[k]
+                matrix[i][j] = self._key_str[k]
                 k += 1
         return matrix
 
     def _get_coordinates(self, char: chr):
         for i, row in enumerate(self._matrix):
             if char in row:
                 return i, row.index(char)
@@ -62,15 +63,15 @@
         else:
             return self._matrix[row1][col2] + self._matrix[row2][col1]
 
     def encrypt(self, plaintext: str) -> str:
         plaintext = plaintext.lower().replace("j", "i")
         plaintext = ''.join(filter(str.isalnum, plaintext))
         for i in range(1, len(plaintext)):
-            if plaintext[i] == plaintext[i - 1] and plaintext[i].isalpha() and plaintext[i] != 'x':
+            if plaintext[i] == plaintext[i-1] and plaintext[i].isalpha() and plaintext[i] != 'x':
                 plaintext = plaintext[:i] + 'x' + plaintext[i:]
         ciphertext = ''
         i = 0
         while i < len(plaintext):
             if not plaintext[i].isalpha():
                 ciphertext += plaintext[i]
                 i += 1
@@ -102,15 +103,17 @@
                 i += 2
         return plaintext
 
 
 # Example usage:
 if __name__ == "__main__":
     key = "secret"
-    message = "HELLO world 2023"
     cipher = PlayfairCipher(key)
-    encrypted_message = cipher.encrypt(message)
-    decrypted_message = cipher.decrypt(encrypted_message)
 
+    message = "HELLO world 2024"
     print("Original message:", message)
+
+    encrypted_message = cipher.encrypt(message)
     print("Encrypted message:", encrypted_message)
+
+    decrypted_message = cipher.decrypt(encrypted_message)
     print("Decrypted message:", decrypted_message)
```

### Comparing `cipherspy-0.2.0/cipherspy.egg-info/PKG-INFO` & `cipherspy-0.3.1/cipherspy.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: cipherspy
-Version: 0.2.0
+Version: 0.3.1
 Summary: Strong Passwords Generator made with python.
 Home-page: https://github.com/fathiabdelmalek/cipherspy.git
 Author: Fathi AbdelMalek
 Author-email: abdelmalek.fathi.2001@gmail.com
 License: OSI Approved :: MIT License
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: System Administrators
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Security
 Classifier: Topic :: Security :: Cryptography
-Requires-Python: >=3.6
+Requires-Python: >=3
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # cipher-py
```

### Comparing `cipherspy-0.2.0/setup.py` & `cipherspy-0.3.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,24 @@
-import setuptools
+from setuptools import setup
 
 with open("README.md", "r") as readme:
     long_description = readme.read()
 
-setuptools.setup(
+setup(
     name="cipherspy",
-    version="0.2.0",
+    version="0.3.1",
     author="Fathi AbdelMalek",
     author_email="abdelmalek.fathi.2001@gmail.com",
     url="https://github.com/fathiabdelmalek/cipherspy.git",
     description="Strong Passwords Generator made with python.",
     license="OSI Approved :: MIT License",
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=['cipherspy', 'cipherspy.cipher'],
-    python_requires=">=3.6",
+    python_requires=">=3",
     classifiers=[
         "Development Status :: 1 - Planning",
         "Intended Audience :: Developers",
         "Intended Audience :: System Administrators",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
         "Programming Language :: Python",
```

