# Comparing `tmp/kisstdlib-0.0.2.tar.gz` & `tmp/kisstdlib-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kisstdlib-0.0.2.tar", last modified: Fri Mar  8 14:07:05 2024, max compression
+gzip compressed data, was "kisstdlib-0.0.3.tar", last modified: Wed Apr  3 14:20:08 2024, max compression
```

## Comparing `kisstdlib-0.0.2.tar` & `kisstdlib-0.0.3.tar`

### file list

```diff
@@ -1,28 +1,29 @@
-drwx------   0 oxij      (1000) oxij      (1000)        0 2024-03-08 14:07:05.151346 kisstdlib-0.0.2/
--rw-------   0 oxij      (1000) oxij      (1000)      568 2024-03-08 14:07:05.150346 kisstdlib-0.0.2/PKG-INFO
--rw-------   0 oxij      (1000) oxij      (1000)      109 2023-11-22 18:22:49.000000 kisstdlib-0.0.2/README.md
-drwx------   0 oxij      (1000) oxij      (1000)        0 2024-03-08 14:07:05.148346 kisstdlib-0.0.2/kisstdlib/
--rw-------   0 oxij      (1000) oxij      (1000)     1161 2024-02-21 14:49:16.000000 kisstdlib-0.0.2/kisstdlib/__init__.py
-drwx------   0 oxij      (1000) oxij      (1000)        0 2024-03-08 14:07:05.149346 kisstdlib-0.0.2/kisstdlib/argparse/
--rw-------   0 oxij      (1000) oxij      (1000)     1179 2024-02-21 14:49:16.000000 kisstdlib-0.0.2/kisstdlib/argparse/__init__.py
--rw-------   0 oxij      (1000) oxij      (1000)     8631 2024-02-21 14:49:16.000000 kisstdlib-0.0.2/kisstdlib/argparse/better.py
--rw-------   0 oxij      (1000) oxij      (1000)     1626 2024-02-21 14:49:16.000000 kisstdlib-0.0.2/kisstdlib/exceptions.py
-drwx------   0 oxij      (1000) oxij      (1000)        0 2024-03-08 14:07:05.150346 kisstdlib-0.0.2/kisstdlib/io/
--rw-------   0 oxij      (1000) oxij      (1000)     2263 2024-02-21 14:49:16.000000 kisstdlib-0.0.2/kisstdlib/io/__init__.py
--rw-------   0 oxij      (1000) oxij      (1000)     3555 2024-02-21 14:49:16.000000 kisstdlib-0.0.2/kisstdlib/io/base.py
-drwx------   0 oxij      (1000) oxij      (1000)        0 2024-03-08 14:07:05.150346 kisstdlib-0.0.2/kisstdlib/io/encoder/
--rw-------   0 oxij      (1000) oxij      (1000)     1199 2024-02-21 14:49:16.000000 kisstdlib-0.0.2/kisstdlib/io/encoder/__init__.py
--rw-------   0 oxij      (1000) oxij      (1000)     2994 2024-02-21 14:49:16.000000 kisstdlib-0.0.2/kisstdlib/io/encoder/base.py
--rw-------   0 oxij      (1000) oxij      (1000)     5221 2024-02-21 14:49:16.000000 kisstdlib-0.0.2/kisstdlib/io/encoder/pyrepr.py
--rw-------   0 oxij      (1000) oxij      (1000)     4250 2024-02-21 14:49:16.000000 kisstdlib-0.0.2/kisstdlib/io/wrapper.py
--rw-------   0 oxij      (1000) oxij      (1000)     1874 2024-02-21 14:49:16.000000 kisstdlib-0.0.2/kisstdlib/logging.py
--rw-------   0 oxij      (1000) oxij      (1000)     3680 2024-03-08 13:35:46.000000 kisstdlib-0.0.2/kisstdlib/path.py
--rw-------   0 oxij      (1000) oxij      (1000)        0 2023-11-22 18:22:49.000000 kisstdlib-0.0.2/kisstdlib/py.typed
-drwx------   0 oxij      (1000) oxij      (1000)        0 2024-03-08 14:07:05.149346 kisstdlib-0.0.2/kisstdlib.egg-info/
--rw-------   0 oxij      (1000) oxij      (1000)      568 2024-03-08 14:07:05.000000 kisstdlib-0.0.2/kisstdlib.egg-info/PKG-INFO
--rw-------   0 oxij      (1000) oxij      (1000)      492 2024-03-08 14:07:05.000000 kisstdlib-0.0.2/kisstdlib.egg-info/SOURCES.txt
--rw-------   0 oxij      (1000) oxij      (1000)        1 2024-03-08 14:07:05.000000 kisstdlib-0.0.2/kisstdlib.egg-info/dependency_links.txt
--rw-------   0 oxij      (1000) oxij      (1000)       10 2024-03-08 14:07:05.000000 kisstdlib-0.0.2/kisstdlib.egg-info/top_level.txt
--rw-------   0 oxij      (1000) oxij      (1000)      708 2024-03-08 14:02:54.000000 kisstdlib-0.0.2/pyproject.toml
--rw-------   0 oxij      (1000) oxij      (1000)       38 2024-03-08 14:07:05.151346 kisstdlib-0.0.2/setup.cfg
--rw-------   0 oxij      (1000) oxij      (1000)       60 2023-11-22 18:22:49.000000 kisstdlib-0.0.2/setup.py
+drwx------   0 oxij      (1000) oxij      (1000)        0 2024-04-03 14:20:08.923670 kisstdlib-0.0.3/
+-rw-r--r--   0 oxij      (1000) oxij      (1000)      568 2024-04-03 14:20:08.923670 kisstdlib-0.0.3/PKG-INFO
+-rw-------   0 oxij      (1000) oxij      (1000)      109 2023-11-22 18:22:49.000000 kisstdlib-0.0.3/README.md
+drwx------   0 oxij      (1000) oxij      (1000)        0 2024-04-03 14:20:08.919670 kisstdlib-0.0.3/kisstdlib/
+-rw-------   0 oxij      (1000) oxij      (1000)     1161 2024-04-03 10:07:26.000000 kisstdlib-0.0.3/kisstdlib/__init__.py
+drwx------   0 oxij      (1000) oxij      (1000)        0 2024-04-03 14:20:08.921670 kisstdlib-0.0.3/kisstdlib/argparse/
+-rw-------   0 oxij      (1000) oxij      (1000)     1179 2024-04-03 10:07:26.000000 kisstdlib-0.0.3/kisstdlib/argparse/__init__.py
+-rw-------   0 oxij      (1000) oxij      (1000)     8631 2024-04-03 10:07:26.000000 kisstdlib-0.0.3/kisstdlib/argparse/better.py
+-rw-------   0 oxij      (1000) oxij      (1000)     1626 2024-04-03 10:07:26.000000 kisstdlib-0.0.3/kisstdlib/exceptions.py
+drwx------   0 oxij      (1000) oxij      (1000)        0 2024-04-03 14:20:08.922670 kisstdlib-0.0.3/kisstdlib/io/
+-rw-------   0 oxij      (1000) oxij      (1000)     2263 2024-04-03 10:07:26.000000 kisstdlib-0.0.3/kisstdlib/io/__init__.py
+-rw-------   0 oxij      (1000) oxij      (1000)     3555 2024-04-03 10:07:26.000000 kisstdlib-0.0.3/kisstdlib/io/base.py
+drwx------   0 oxij      (1000) oxij      (1000)        0 2024-04-03 14:20:08.922670 kisstdlib-0.0.3/kisstdlib/io/encoder/
+-rw-------   0 oxij      (1000) oxij      (1000)     1199 2024-04-03 10:07:26.000000 kisstdlib-0.0.3/kisstdlib/io/encoder/__init__.py
+-rw-------   0 oxij      (1000) oxij      (1000)     2994 2024-04-03 10:07:26.000000 kisstdlib-0.0.3/kisstdlib/io/encoder/base.py
+-rw-------   0 oxij      (1000) oxij      (1000)     5221 2024-04-03 10:07:26.000000 kisstdlib-0.0.3/kisstdlib/io/encoder/pyrepr.py
+-rw-------   0 oxij      (1000) oxij      (1000)     1419 2024-04-03 10:07:26.000000 kisstdlib-0.0.3/kisstdlib/io/stdio.py
+-rw-------   0 oxij      (1000) oxij      (1000)     4433 2024-04-03 10:07:26.000000 kisstdlib-0.0.3/kisstdlib/io/wrapper.py
+-rw-------   0 oxij      (1000) oxij      (1000)     1874 2024-04-03 10:07:26.000000 kisstdlib-0.0.3/kisstdlib/logging.py
+-rw-------   0 oxij      (1000) oxij      (1000)     3902 2024-04-03 10:07:26.000000 kisstdlib-0.0.3/kisstdlib/path.py
+-rw-------   0 oxij      (1000) oxij      (1000)        0 2023-11-22 18:22:49.000000 kisstdlib-0.0.3/kisstdlib/py.typed
+drwx------   0 oxij      (1000) oxij      (1000)        0 2024-04-03 14:20:08.923670 kisstdlib-0.0.3/kisstdlib.egg-info/
+-rw-r--r--   0 oxij      (1000) oxij      (1000)      568 2024-04-03 14:20:08.000000 kisstdlib-0.0.3/kisstdlib.egg-info/PKG-INFO
+-rw-------   0 oxij      (1000) oxij      (1000)      514 2024-04-03 14:20:08.000000 kisstdlib-0.0.3/kisstdlib.egg-info/SOURCES.txt
+-rw-------   0 oxij      (1000) oxij      (1000)        1 2024-04-03 14:20:08.000000 kisstdlib-0.0.3/kisstdlib.egg-info/dependency_links.txt
+-rw-------   0 oxij      (1000) oxij      (1000)       10 2024-04-03 14:20:08.000000 kisstdlib-0.0.3/kisstdlib.egg-info/top_level.txt
+-rw-------   0 oxij      (1000) oxij      (1000)      708 2024-04-03 10:07:26.000000 kisstdlib-0.0.3/pyproject.toml
+-rw-------   0 oxij      (1000) oxij      (1000)       38 2024-04-03 14:20:08.923670 kisstdlib-0.0.3/setup.cfg
+-rw-------   0 oxij      (1000) oxij      (1000)       60 2023-11-22 18:22:49.000000 kisstdlib-0.0.3/setup.py
```

### Comparing `kisstdlib-0.0.2/PKG-INFO` & `kisstdlib-0.0.3/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kisstdlib
-Version: 0.0.2
+Version: 0.0.3
 Summary: Keep It Simple STandarD LIBraries set for Python
 Author-email: Jan Malakhovski <oxij@oxij.org>
 Keywords: sys,stdlib
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: License :: OSI Approved :: Python Software Foundation License
```

### Comparing `kisstdlib-0.0.2/kisstdlib/__init__.py` & `kisstdlib-0.0.3/kisstdlib/argparse/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-# This file is a part of kisstdlib project.
+# Copyright (c) 2023 Jan Malakhovski <oxij@oxij.org>
 #
-# Copyright (c) 2018-2023 Jan Malakhovski <oxij@oxij.org>
+# This file is a part of kisstdlib project.
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 # copies of the Software, and to permit persons to whom the Software is
 # furnished to do so, subject to the following conditions:
@@ -15,7 +15,9 @@
 # THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
 # IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
+
+from .better import *
```

### Comparing `kisstdlib-0.0.2/kisstdlib/argparse/__init__.py` & `kisstdlib-0.0.3/kisstdlib/io/encoder/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-# This file is a part of kisstdlib project.
-#
 # Copyright (c) 2023 Jan Malakhovski <oxij@oxij.org>
 #
+# This file is a part of kisstdlib project.
+#
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 # copies of the Software, and to permit persons to whom the Software is
 # furnished to do so, subject to the following conditions:
 #
@@ -16,8 +16,9 @@
 # IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 
-from .better import *
+from .base import *
+from .pyrepr import *
```

### Comparing `kisstdlib-0.0.2/kisstdlib/argparse/better.py` & `kisstdlib-0.0.3/kisstdlib/argparse/better.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
+# Copyright (c) 2022-2023 Jan Malakhovski <oxij@oxij.org>
+#
 # This file is a part of kisstdlib project.
 #
 # This file can be distributed under the terms of the MIT-style license given
 # below or Python Software Foundation License version 2 (PSF-2.0) as published
 # by Python Software Foundation.
 #
-# Copyright (c) 2022-2023 Jan Malakhovski <oxij@oxij.org>
-#
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 # copies of the Software, and to permit persons to whom the Software is
 # furnished to do so, subject to the following conditions:
 #
```

### Comparing `kisstdlib-0.0.2/kisstdlib/exceptions.py` & `kisstdlib-0.0.3/kisstdlib/exceptions.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-# This file is a part of kisstdlib project.
-#
 # Copyright (c) 2023 Jan Malakhovski <oxij@oxij.org>
 #
+# This file is a part of kisstdlib project.
+#
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 # copies of the Software, and to permit persons to whom the Software is
 # furnished to do so, subject to the following conditions:
 #
```

### Comparing `kisstdlib-0.0.2/kisstdlib/io/__init__.py` & `kisstdlib-0.0.3/kisstdlib/io/__init__.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-# This file is a part of kisstdlib project.
-#
 # Copyright (c) 2018-2023 Jan Malakhovski <oxij@oxij.org>
 #
+# This file is a part of kisstdlib project.
+#
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 # copies of the Software, and to permit persons to whom the Software is
 # furnished to do so, subject to the following conditions:
 #
```

### Comparing `kisstdlib-0.0.2/kisstdlib/io/base.py` & `kisstdlib-0.0.3/kisstdlib/io/base.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-# This file is a part of kisstdlib project.
-#
 # Copyright (c) 2018-2023 Jan Malakhovski <oxij@oxij.org>
 #
+# This file is a part of kisstdlib project.
+#
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 # copies of the Software, and to permit persons to whom the Software is
 # furnished to do so, subject to the following conditions:
 #
```

### Comparing `kisstdlib-0.0.2/kisstdlib/io/encoder/__init__.py` & `kisstdlib-0.0.3/kisstdlib/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-# This file is a part of kisstdlib project.
+# Copyright (c) 2018-2023 Jan Malakhovski <oxij@oxij.org>
 #
-# Copyright (c) 2023 Jan Malakhovski <oxij@oxij.org>
+# This file is a part of kisstdlib project.
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 # copies of the Software, and to permit persons to whom the Software is
 # furnished to do so, subject to the following conditions:
@@ -15,10 +15,7 @@
 # THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
 # IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
-
-from .base import *
-from .pyrepr import *
```

### Comparing `kisstdlib-0.0.2/kisstdlib/io/encoder/base.py` & `kisstdlib-0.0.3/kisstdlib/io/encoder/base.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-# This file is a part of kisstdlib project.
-#
 # Copyright (c) 2023 Jan Malakhovski <oxij@oxij.org>
 #
+# This file is a part of kisstdlib project.
+#
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 # copies of the Software, and to permit persons to whom the Software is
 # furnished to do so, subject to the following conditions:
 #
```

### Comparing `kisstdlib-0.0.2/kisstdlib/io/encoder/pyrepr.py` & `kisstdlib-0.0.3/kisstdlib/io/encoder/pyrepr.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-# This file is a part of kisstdlib project.
-#
 # Copyright (c) 2023 Jan Malakhovski <oxij@oxij.org>
 #
+# This file is a part of kisstdlib project.
+#
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 # copies of the Software, and to permit persons to whom the Software is
 # furnished to do so, subject to the following conditions:
 #
```

### Comparing `kisstdlib-0.0.2/kisstdlib/io/wrapper.py` & `kisstdlib-0.0.3/kisstdlib/io/wrapper.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-# This file is a part of kisstdlib project.
+# Copyright (c) 2018-2024 Jan Malakhovski <oxij@oxij.org>
 #
-# Copyright (c) 2018-2023 Jan Malakhovski <oxij@oxij.org>
+# This file is a part of kisstdlib project.
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 # copies of the Software, and to permit persons to whom the Software is
 # furnished to do so, subject to the following conditions:
@@ -23,36 +23,45 @@
 import logging as _logging
 import os as _os
 import sys as _sys
 import typing as _t
 
 from .base import *
 
+_logger = _logging.getLogger("kisstd")
+
 class MinimalIOWrapper(MinimalIO):
+    fobj : _t.Any
+    fileno : int | None
+
     def __init__(self, fobj : _t.Any) -> None:
         self.fobj = fobj
         # _socket.socket's fileno() will return -1 after
         # .close() and poll needs an actual value to unsubscribe
         # properly so we have to keep a copy here
         try:
-            self._fileno = fobj.fileno()
+            self.fileno = fobj.fileno()
         except OSError:
-            self._fileno = None
-        _logging.getLogger("kisstd").debug("init %s", self)
+            self.fileno = None
+        _logger.debug("init %s", self)
 
     def __del__(self) -> None:
-        _logging.getLogger("kisstd").debug("del %s", self)
+        _logger.debug("del %s", self)
 
     def __repr__(self) -> str:
-        if self._fileno is not None:
-            desc = "fd=" + str(self._fileno)
+        if self.fileno is not None:
+            desc = "fd=" + str(self.fileno)
         else:
             desc = "obj=" + str(id(self.fobj))
         return "<%s %s %s closed=%s>" % (self.__class__.__name__, hex(id(self)), desc, self.closed)
 
+    @property
+    def isatty(self) -> bool:
+        return self.fobj.isatty() # type: ignore
+
     def close(self) -> None:
         self.fobj.close()
 
     @property
     def closed(self) -> bool:
         return self.fobj.closed # type: ignore
 
@@ -110,10 +119,14 @@
 
     def write(self, data : str | ByteString) -> None:
         if isinstance(data, str):
             self.write_str(data)
         else:
             self.write_bytes(data)
 
-stdin = TIOWrappedReader(_os.fdopen(_sys.stdin.fileno(), "rb"))
-stdout = TIOWrappedWriter(_os.fdopen(_sys.stdout.fileno(), "wb"))
-stderr = TIOWrappedWriter(_os.fdopen(_sys.stderr.fileno(), "wb"))
+    def write_ln(self, data : str | ByteString) -> None:
+        self.write(data)
+        self.write_bytes(self.eol)
+
+    def __exit__(self, exc_type : _t.Any, exc_value : _t.Any, exc_tb : _t.Any) -> None:
+        self.flush()
+        self.close()
```

### Comparing `kisstdlib-0.0.2/kisstdlib/logging.py` & `kisstdlib-0.0.3/kisstdlib/logging.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-# This file is a part of kisstdlib project.
-#
 # Copyright (c) 2023 Jan Malakhovski <oxij@oxij.org>
 #
+# This file is a part of kisstdlib project.
+#
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 # copies of the Software, and to permit persons to whom the Software is
 # furnished to do so, subject to the following conditions:
 #
```

### Comparing `kisstdlib-0.0.2/kisstdlib/path.py` & `kisstdlib-0.0.3/kisstdlib/path.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-# This file is a part of kisstdlib project.
+# Copyright (c) 2018-2024 Jan Malakhovski <oxij@oxij.org>
 #
-# Copyright (c) 2018-2023 Jan Malakhovski <oxij@oxij.org>
+# This file is a part of kisstdlib project.
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 # copies of the Software, and to permit persons to whom the Software is
 # furnished to do so, subject to the following conditions:
@@ -22,21 +22,22 @@
 
 import logging as _logging
 import os as _os
 import stat as _stat
 import typing as _t
 
 def walk_orderly(path : _t.AnyStr,
+                 *,
                  include_directories : bool = True,
                  follow_symlinks : bool = True,
-                 order_by : bool | None = True,
+                 ordering : bool | None = True,
                  handle_error : _t.Callable[..., None] | None = _logging.error) -> _t.Iterable[_t.AnyStr]:
     """Similar to os.walk, but produces an iterator over plain file paths, allows
        non-directories as input (which will just output a single element), and
-       the output is guaranteed to be ordered if `order_by` is not `None`.
+       the output is guaranteed to be ordered if `ordering` is not `None`.
     """
 
     try:
         fstat = _os.stat(path, follow_symlinks = follow_symlinks)
     except OSError:
         if handle_error is not None:
             handle_error("failed to stat: %s", path)
@@ -81,18 +82,22 @@
                     if isinstance(entry.path, bytes):
                         elements.append(entry.path + b"/") # type: ignore
                     else:
                         elements.append(entry.path + "/")
                 else:
                     elements.append(entry.path)
 
-    if order_by is not None:
-        elements.sort(reverse=not order_by)
+    if ordering is not None:
+        elements.sort(reverse=not ordering)
 
     for path in elements:
         lchar : _t.AnyStr = path[-1:]
         if lchar == "/" or lchar == b"/":
             if include_directories:
                 yield path
-            yield from walk_orderly(path, include_directories, follow_symlinks, order_by, handle_error)
+            yield from walk_orderly(path,
+                                    include_directories=include_directories,
+                                    follow_symlinks=follow_symlinks,
+                                    ordering=ordering,
+                                    handle_error=handle_error)
         else:
             yield path
```

### Comparing `kisstdlib-0.0.2/kisstdlib.egg-info/PKG-INFO` & `kisstdlib-0.0.3/kisstdlib.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kisstdlib
-Version: 0.0.2
+Version: 0.0.3
 Summary: Keep It Simple STandarD LIBraries set for Python
 Author-email: Jan Malakhovski <oxij@oxij.org>
 Keywords: sys,stdlib
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: License :: OSI Approved :: Python Software Foundation License
```

### Comparing `kisstdlib-0.0.2/pyproject.toml` & `kisstdlib-0.0.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 [project]
 name = "kisstdlib"
-version = "0.0.2"
+version = "0.0.3"
 authors = [{ name = "Jan Malakhovski", email = "oxij@oxij.org" }]
 description = "Keep It Simple STandarD LIBraries set for Python"
 readme = "README.md"
 classifiers = [
     "Development Status :: 4 - Beta",
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
```

