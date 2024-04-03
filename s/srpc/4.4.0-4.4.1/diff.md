# Comparing `tmp/srpc-4.4.0-cp312-none-win_amd64.whl.zip` & `tmp/srpc-4.4.1-cp312-none-macosx_10_9_universal2.whl.zip`

## zipinfo {}

```diff
@@ -1,13 +1,13 @@
-Zip file size: 278455 bytes, number of entries: 11
--rw-rw-rw-  2.0 fat     1085 b- defN 24-Mar-29 12:39 srpc-4.4.0.dist-info/LICENSE
--rw-rw-rw-  2.0 fat     2216 b- defN 24-Mar-29 12:39 srpc-4.4.0.dist-info/METADATA
--rw-rw-rw-  2.0 fat      100 b- defN 24-Mar-29 12:39 srpc-4.4.0.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        1 b- defN 24-Mar-29 12:39 srpc-4.4.0.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      371 b- defN 24-Mar-29 12:39 srpc-4.4.0.dist-info/RECORD
--rw-rw-rw-  2.0 fat    23040 b- defN 24-Mar-29 12:39 srpc/__init__.pyd
--rw-rw-rw-  2.0 fat   122880 b- defN 24-Mar-29 12:39 srpc/client.pyd
--rw-rw-rw-  2.0 fat   119808 b- defN 24-Mar-29 12:39 srpc/protocol.pyd
--rw-rw-rw-  2.0 fat    83968 b- defN 24-Mar-29 12:39 srpc/ring.pyd
--rw-rw-rw-  2.0 fat   129024 b- defN 24-Mar-29 12:39 srpc/server.pyd
--rw-rw-rw-  2.0 fat   143872 b- defN 24-Mar-29 12:39 srpc/ulog.pyd
-11 files, 626365 bytes uncompressed, 277129 bytes compressed:  55.8%
+Zip file size: 618877 bytes, number of entries: 11
+-rw-r--r--  2.0 unx     1064 b- defN 24-Apr-03 15:27 srpc-4.4.1.dist-info/LICENSE
+-rw-r--r--  2.0 unx     2169 b- defN 24-Apr-03 15:27 srpc-4.4.1.dist-info/METADATA
+-rw-r--r--  2.0 unx      113 b- defN 24-Apr-03 15:27 srpc-4.4.1.dist-info/WHEEL
+-rw-r--r--  2.0 unx        1 b- defN 24-Apr-03 15:27 srpc-4.4.1.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      371 b- defN 24-Apr-03 15:27 srpc-4.4.1.dist-info/RECORD
+-rwxr-xr-x  2.0 unx   122272 b- defN 24-Apr-03 15:26 srpc/__init__.so
+-rwxr-xr-x  2.0 unx   407310 b- defN 24-Apr-03 15:26 srpc/client.so
+-rwxr-xr-x  2.0 unx   393344 b- defN 24-Apr-03 15:26 srpc/protocol.so
+-rwxr-xr-x  2.0 unx   287020 b- defN 24-Apr-03 15:27 srpc/ring.so
+-rwxr-xr-x  2.0 unx   426974 b- defN 24-Apr-03 15:26 srpc/server.so
+-rwxr-xr-x  2.0 unx   463004 b- defN 24-Apr-03 15:26 srpc/ulog.so
+11 files, 2103642 bytes uncompressed, 617563 bytes compressed:  70.7%
```

## zipnote {}

```diff
@@ -1,34 +1,34 @@
-Filename: srpc-4.4.0.dist-info/LICENSE
+Filename: srpc-4.4.1.dist-info/LICENSE
 Comment: 
 
-Filename: srpc-4.4.0.dist-info/METADATA
+Filename: srpc-4.4.1.dist-info/METADATA
 Comment: 
 
-Filename: srpc-4.4.0.dist-info/WHEEL
+Filename: srpc-4.4.1.dist-info/WHEEL
 Comment: 
 
-Filename: srpc-4.4.0.dist-info/top_level.txt
+Filename: srpc-4.4.1.dist-info/top_level.txt
 Comment: 
 
-Filename: srpc-4.4.0.dist-info/RECORD
+Filename: srpc-4.4.1.dist-info/RECORD
 Comment: 
 
-Filename: srpc/__init__.pyd
+Filename: srpc/__init__.so
 Comment: 
 
-Filename: srpc/client.pyd
+Filename: srpc/client.so
 Comment: 
 
-Filename: srpc/protocol.pyd
+Filename: srpc/protocol.so
 Comment: 
 
-Filename: srpc/ring.pyd
+Filename: srpc/ring.so
 Comment: 
 
-Filename: srpc/server.pyd
+Filename: srpc/server.so
 Comment: 
 
-Filename: srpc/ulog.pyd
+Filename: srpc/ulog.so
 Comment: 
 
 Zip file comment:
```

## Comparing `srpc-4.4.0.dist-info/LICENSE` & `srpc-4.4.1.dist-info/LICENSE`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-MIT License
-
-Copyright (c) 2021 YL Feng
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
+MIT License
+
+Copyright (c) 2021 YL Feng
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+SOFTWARE.
```

## Comparing `srpc-4.4.0.dist-info/METADATA` & `srpc-4.4.1.dist-info/METADATA`

 * *Files 17% similar despite different names*

```diff
@@ -1,47 +1,47 @@
-Metadata-Version: 2.1
-Name: srpc
-Version: 4.4.0
-Summary: description
-Author-email: YL <fengyl@pku.edu.cn>
-License: MIT License
-        
-        Copyright (c) 2021 YL Feng
-        
-        Permission is hereby granted, free of charge, to any person obtaining a copy
-        of this software and associated documentation files (the "Software"), to deal
-        in the Software without restriction, including without limitation the rights
-        to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-        copies of the Software, and to permit persons to whom the Software is
-        furnished to do so, subject to the following conditions:
-        
-        The above copyright notice and this permission notice shall be included in all
-        copies or substantial portions of the Software.
-        
-        THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-        IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-        FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-        AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-        LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-        OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-        SOFTWARE.
-        
-Project-URL: homepage, https://gitee.com
-Project-URL: documentation, https://gitee.com
-Project-URL: bugs, https://gitee.com
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Intended Audience :: Developers
-Classifier: Intended Audience :: Science/Research
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Natural Language :: Chinese (Simplified)
-Classifier: Natural Language :: English
-Classifier: Operating System :: Microsoft :: Windows
-Classifier: Operating System :: POSIX :: Linux
-Classifier: Operating System :: MacOS :: MacOS X
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Topic :: Scientific/Engineering :: Physics
-Requires-Python: >=3.10
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: msgpack >=1.0.0
-Requires-Dist: numpy >=1.20.0
-
+Metadata-Version: 2.1
+Name: srpc
+Version: 4.4.1
+Summary: description
+Author-email: YL <fengyl@pku.edu.cn>
+License: MIT License
+        
+        Copyright (c) 2021 YL Feng
+        
+        Permission is hereby granted, free of charge, to any person obtaining a copy
+        of this software and associated documentation files (the "Software"), to deal
+        in the Software without restriction, including without limitation the rights
+        to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+        copies of the Software, and to permit persons to whom the Software is
+        furnished to do so, subject to the following conditions:
+        
+        The above copyright notice and this permission notice shall be included in all
+        copies or substantial portions of the Software.
+        
+        THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+        IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+        FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+        AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+        LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+        OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+        SOFTWARE.
+        
+Project-URL: homepage, https://gitee.com
+Project-URL: documentation, https://gitee.com
+Project-URL: bugs, https://gitee.com
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Intended Audience :: Developers
+Classifier: Intended Audience :: Science/Research
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Natural Language :: Chinese (Simplified)
+Classifier: Natural Language :: English
+Classifier: Operating System :: Microsoft :: Windows
+Classifier: Operating System :: POSIX :: Linux
+Classifier: Operating System :: MacOS :: MacOS X
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Topic :: Scientific/Engineering :: Physics
+Requires-Python: >=3.10
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: msgpack >=1.0.0
+Requires-Dist: numpy >=1.20.0
+
```

