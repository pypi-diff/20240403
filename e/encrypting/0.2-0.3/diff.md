# Comparing `tmp/encrypting-0.2-py3-none-any.whl.zip` & `tmp/encrypting-0.3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,7 +1,7 @@
-Zip file size: 2653 bytes, number of entries: 5
--rw-rw-rw-  2.0 fat     2254 b- defN 24-Apr-01 14:10 encrypting/__init__.py
--rw-rw-rw-  2.0 fat     1922 b- defN 24-Apr-02 09:09 encrypting-0.2.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 24-Apr-02 09:09 encrypting-0.2.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       11 b- defN 24-Apr-02 09:09 encrypting-0.2.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      381 b- defN 24-Apr-02 09:09 encrypting-0.2.dist-info/RECORD
-5 files, 4660 bytes uncompressed, 1943 bytes compressed:  58.3%
+Zip file size: 2641 bytes, number of entries: 5
+-rw-rw-rw-  2.0 fat     2226 b- defN 24-Apr-03 13:44 encrypting/__init__.py
+-rw-rw-rw-  2.0 fat     1922 b- defN 24-Apr-03 13:46 encrypting-0.3.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 24-Apr-03 13:46 encrypting-0.3.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       11 b- defN 24-Apr-03 13:46 encrypting-0.3.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      381 b- defN 24-Apr-03 13:46 encrypting-0.3.dist-info/RECORD
+5 files, 4632 bytes uncompressed, 1931 bytes compressed:  58.3%
```

## zipnote {}

```diff
@@ -1,16 +1,16 @@
 Filename: encrypting/__init__.py
 Comment: 
 
-Filename: encrypting-0.2.dist-info/METADATA
+Filename: encrypting-0.3.dist-info/METADATA
 Comment: 
 
-Filename: encrypting-0.2.dist-info/WHEEL
+Filename: encrypting-0.3.dist-info/WHEEL
 Comment: 
 
-Filename: encrypting-0.2.dist-info/top_level.txt
+Filename: encrypting-0.3.dist-info/top_level.txt
 Comment: 
 
-Filename: encrypting-0.2.dist-info/RECORD
+Filename: encrypting-0.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## encrypting/__init__.py

```diff
@@ -1,9 +1,8 @@
 from random import getrandbits
-from math import gcd, fmod
 from hashlib import sha256
 
 def generate_pair(root_len=16, prime_len=1024):
 	return getrandbits(root_len), getrandbits(prime_len)
 
 class Encrypt:
 	def __init__(self, pair, secret_len=256):
```

## Comparing `encrypting-0.2.dist-info/METADATA` & `encrypting-0.3.dist-info/METADATA`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: encrypting
-Version: 0.2
+Version: 0.3
 Summary: Simple XOR Encryptor
 Author: MichaKrutoy
 Description-Content-Type: text/markdown
 
 # Encrypting library for python
 
 **This library provides a socket encryption method based on XOR and Diffie-Hellman algorithm**
```

