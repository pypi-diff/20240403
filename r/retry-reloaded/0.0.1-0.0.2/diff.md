# Comparing `tmp/retry-reloaded-0.0.1.tar.gz` & `tmp/retry-reloaded-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "retry-reloaded-0.0.1.tar", last modified: Mon Apr  1 12:18:15 2024, max compression
+gzip compressed data, was "retry-reloaded-0.0.2.tar", last modified: Wed Apr  3 16:43:01 2024, max compression
```

## Comparing `retry-reloaded-0.0.1.tar` & `retry-reloaded-0.0.2.tar`

### file list

```diff
@@ -1,26 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 12:18:15.282163 retry-reloaded-0.0.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1075 2024-04-01 12:18:05.000000 retry-reloaded-0.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     5490 2024-04-01 12:18:15.282163 retry-reloaded-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4967 2024-04-01 12:18:05.000000 retry-reloaded-0.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 12:18:15.278163 retry-reloaded-0.0.1/retry/
--rw-r--r--   0 runner    (1001) docker     (127)      583 2024-04-01 12:18:05.000000 retry-reloaded-0.0.1/retry/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5916 2024-04-01 12:18:05.000000 retry-reloaded-0.0.1/retry/retry.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 12:18:15.282163 retry-reloaded-0.0.1/retry/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 12:18:05.000000 retry-reloaded-0.0.1/retry/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3717 2024-04-01 12:18:05.000000 retry-reloaded-0.0.1/retry/utils/_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2465 2024-04-01 12:18:05.000000 retry-reloaded-0.0.1/retry/utils/_logging.py
--rw-r--r--   0 runner    (1001) docker     (127)     1991 2024-04-01 12:18:05.000000 retry-reloaded-0.0.1/retry/utils/_validate.py
--rw-r--r--   0 runner    (1001) docker     (127)     6892 2024-04-01 12:18:05.000000 retry-reloaded-0.0.1/retry/utils/backoff.py
--rw-r--r--   0 runner    (1001) docker     (127)     2253 2024-04-01 12:18:05.000000 retry-reloaded-0.0.1/retry/utils/callback.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 12:18:15.282163 retry-reloaded-0.0.1/retry_reloaded.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5490 2024-04-01 12:18:15.000000 retry-reloaded-0.0.1/retry_reloaded.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      448 2024-04-01 12:18:15.000000 retry-reloaded-0.0.1/retry_reloaded.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-01 12:18:15.000000 retry-reloaded-0.0.1/retry_reloaded.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-01 12:18:15.000000 retry-reloaded-0.0.1/retry_reloaded.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-01 12:18:15.282163 retry-reloaded-0.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      756 2024-04-01 12:18:05.000000 retry-reloaded-0.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 12:18:15.282163 retry-reloaded-0.0.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     4573 2024-04-01 12:18:05.000000 retry-reloaded-0.0.1/tests/test_backoff.py
--rw-r--r--   0 runner    (1001) docker     (127)     2186 2024-04-01 12:18:05.000000 retry-reloaded-0.0.1/tests/test_callback.py
--rw-r--r--   0 runner    (1001) docker     (127)     2770 2024-04-01 12:18:05.000000 retry-reloaded-0.0.1/tests/test_retry.py
--rw-r--r--   0 runner    (1001) docker     (127)     2004 2024-04-01 12:18:05.000000 retry-reloaded-0.0.1/tests/test_retry_args.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 16:43:01.418314 retry-reloaded-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1075 2024-04-03 16:42:55.000000 retry-reloaded-0.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     5531 2024-04-03 16:43:01.418314 retry-reloaded-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5008 2024-04-03 16:42:55.000000 retry-reloaded-0.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 16:43:01.414313 retry-reloaded-0.0.2/retry/
+-rw-r--r--   0 runner    (1001) docker     (127)      565 2024-04-03 16:42:55.000000 retry-reloaded-0.0.2/retry/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3717 2024-04-03 16:42:55.000000 retry-reloaded-0.0.2/retry/_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2465 2024-04-03 16:42:55.000000 retry-reloaded-0.0.2/retry/_logging.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1991 2024-04-03 16:42:55.000000 retry-reloaded-0.0.2/retry/_validate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6892 2024-04-03 16:42:55.000000 retry-reloaded-0.0.2/retry/backoff.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2253 2024-04-03 16:42:55.000000 retry-reloaded-0.0.2/retry/callback.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5892 2024-04-03 16:42:55.000000 retry-reloaded-0.0.2/retry/retry.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 16:43:01.418314 retry-reloaded-0.0.2/retry_reloaded.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5531 2024-04-03 16:43:01.000000 retry-reloaded-0.0.2/retry_reloaded.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      394 2024-04-03 16:43:01.000000 retry-reloaded-0.0.2/retry_reloaded.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 16:43:01.000000 retry-reloaded-0.0.2/retry_reloaded.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-03 16:43:01.000000 retry-reloaded-0.0.2/retry_reloaded.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-03 16:43:01.418314 retry-reloaded-0.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      756 2024-04-03 16:42:55.000000 retry-reloaded-0.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 16:43:01.418314 retry-reloaded-0.0.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     4567 2024-04-03 16:42:55.000000 retry-reloaded-0.0.2/tests/test_backoff.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2180 2024-04-03 16:42:55.000000 retry-reloaded-0.0.2/tests/test_callback.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2758 2024-04-03 16:42:55.000000 retry-reloaded-0.0.2/tests/test_retry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2004 2024-04-03 16:42:55.000000 retry-reloaded-0.0.2/tests/test_retry_args.py
```

### Comparing `retry-reloaded-0.0.1/LICENSE` & `retry-reloaded-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `retry-reloaded-0.0.1/PKG-INFO` & `retry-reloaded-0.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: retry-reloaded
-Version: 0.0.1
+Version: 0.0.2
 Summary: A simple Python library for retrying functions         with various backoff and callback strategies.
 Home-page: https://github.com/chrisK824/retry
 Author: Chris Karvouniaris
 Author-email: christos.karvouniaris247@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -12,14 +12,17 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # retry
 A simple, yet powerful, generic retry decorator in Python for retrying functions with various backoff and callback strategies.
 
 
+## Install
+`pip install retry-reloaded`
+
 ## Features:
 
 - **Exception Handling**: Retry based on specific exceptions.
 - **Maximum Retries**: Set the maximum number of retry attempts.
 - **Timeout**: Specify the maximum time to spend on retries. Timeout check happens right before retry execution of the wrapped function.
 - **Deadline**: Define a deadline for retries to complete. Deadline check happens right after the retry execution of the wrapped function.
 - **Backoff Strategies**: Choose from various backoff strategies: fixed, exponential, linear, random
```

### Comparing `retry-reloaded-0.0.1/README.md` & `retry-reloaded-0.0.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,14 @@
 # retry
 A simple, yet powerful, generic retry decorator in Python for retrying functions with various backoff and callback strategies.
 
 
+## Install
+`pip install retry-reloaded`
+
 ## Features:
 
 - **Exception Handling**: Retry based on specific exceptions.
 - **Maximum Retries**: Set the maximum number of retry attempts.
 - **Timeout**: Specify the maximum time to spend on retries. Timeout check happens right before retry execution of the wrapped function.
 - **Deadline**: Define a deadline for retries to complete. Deadline check happens right after the retry execution of the wrapped function.
 - **Backoff Strategies**: Choose from various backoff strategies: fixed, exponential, linear, random
```

### Comparing `retry-reloaded-0.0.1/retry/__init__.py` & `retry-reloaded-0.0.2/retry/__init__.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from .retry import retry
-from .utils.callback import CallbackFactory, callback_factory
-from .utils.backoff import (
+from .callback import CallbackFactory, callback_factory
+from .backoff import (
     FixedBackOff,
     LinearBackOff,
     ExponentialBackOff,
     RandomUniformBackOff,
 )
-from .utils._exceptions import (
+from ._exceptions import (
     MaxRetriesException,
     RetriesTimeoutException,
     RetriesDeadlineException
 )
 
 __all__ = [
     "retry",
```

### Comparing `retry-reloaded-0.0.1/retry/retry.py` & `retry-reloaded-0.0.2/retry/retry.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 import logging
 from time import sleep
 from functools import wraps
 from typing import Union, Callable, Tuple, Type
 from time import time
-from .utils._validate import _validate_args
-from .utils._logging import _init_logger, _log_retry
-from .utils._exceptions import (
+from ._validate import _validate_args
+from ._logging import _init_logger, _log_retry
+from ._exceptions import (
     MaxRetriesException,
     RetriesTimeoutException,
     RetriesDeadlineException,
 )
-from .utils.backoff import BackOff, FixedBackOff
+from .backoff import BackOff, FixedBackOff
 
 
 retry_logger = _init_logger(__package__)
 
 
 def retry(
     exceptions: Tuple[Type[Exception]] = (Exception,),
```

### Comparing `retry-reloaded-0.0.1/retry/utils/_exceptions.py` & `retry-reloaded-0.0.2/retry/_exceptions.py`

 * *Files identical despite different names*

### Comparing `retry-reloaded-0.0.1/retry/utils/_logging.py` & `retry-reloaded-0.0.2/retry/_logging.py`

 * *Files identical despite different names*

### Comparing `retry-reloaded-0.0.1/retry/utils/_validate.py` & `retry-reloaded-0.0.2/retry/_validate.py`

 * *Files identical despite different names*

### Comparing `retry-reloaded-0.0.1/retry/utils/backoff.py` & `retry-reloaded-0.0.2/retry/backoff.py`

 * *Files identical despite different names*

### Comparing `retry-reloaded-0.0.1/retry/utils/callback.py` & `retry-reloaded-0.0.2/retry/callback.py`

 * *Files identical despite different names*

### Comparing `retry-reloaded-0.0.1/retry_reloaded.egg-info/PKG-INFO` & `retry-reloaded-0.0.2/retry_reloaded.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: retry-reloaded
-Version: 0.0.1
+Version: 0.0.2
 Summary: A simple Python library for retrying functions         with various backoff and callback strategies.
 Home-page: https://github.com/chrisK824/retry
 Author: Chris Karvouniaris
 Author-email: christos.karvouniaris247@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -12,14 +12,17 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # retry
 A simple, yet powerful, generic retry decorator in Python for retrying functions with various backoff and callback strategies.
 
 
+## Install
+`pip install retry-reloaded`
+
 ## Features:
 
 - **Exception Handling**: Retry based on specific exceptions.
 - **Maximum Retries**: Set the maximum number of retry attempts.
 - **Timeout**: Specify the maximum time to spend on retries. Timeout check happens right before retry execution of the wrapped function.
 - **Deadline**: Define a deadline for retries to complete. Deadline check happens right after the retry execution of the wrapped function.
 - **Backoff Strategies**: Choose from various backoff strategies: fixed, exponential, linear, random
```

### Comparing `retry-reloaded-0.0.1/setup.py` & `retry-reloaded-0.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="retry-reloaded",
-    version="0.0.1",
+    version="0.0.2",
     description="A simple Python library for retrying functions \
         with various backoff and callback strategies.",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     url="https://github.com/chrisK824/retry",
     author="Chris Karvouniaris",
     author_email="christos.karvouniaris247@gmail.com",
```

### Comparing `retry-reloaded-0.0.1/tests/test_backoff.py` & `retry-reloaded-0.0.2/tests/test_backoff.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from retry.utils.backoff import (
+from retry.backoff import (
     FixedBackOff,
     LinearBackOff,
     RandomUniformBackOff,
     ExponentialBackOff,
 )
 import pytest
```

### Comparing `retry-reloaded-0.0.1/tests/test_callback.py` & `retry-reloaded-0.0.2/tests/test_callback.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from retry.utils.callback import CallbackFactory, callback_factory
+from retry.callback import CallbackFactory, callback_factory
 import pytest
 
 
 def test_CallbackFactory_callable_function():
     def dummy_func():
         pass
```

### Comparing `retry-reloaded-0.0.1/tests/test_retry.py` & `retry-reloaded-0.0.2/tests/test_retry.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import pytest
 from time import sleep
 from retry.retry import retry
-from retry.utils._exceptions import (
+from retry._exceptions import (
     MaxRetriesException,
     RetriesTimeoutException,
     RetriesDeadlineException
 )
-from retry.utils.backoff import FixedBackOff
+from retry.backoff import FixedBackOff
 
 
 def test_successful_execution():
     retries = 0
 
     @retry(max_retries=3)
     def successful_function():
```

### Comparing `retry-reloaded-0.0.1/tests/test_retry_args.py` & `retry-reloaded-0.0.2/tests/test_retry_args.py`

 * *Files identical despite different names*

