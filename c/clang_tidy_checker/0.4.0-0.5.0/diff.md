# Comparing `tmp/clang_tidy_checker-0.4.0.tar.gz` & `tmp/clang_tidy_checker-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "clang_tidy_checker-0.4.0.tar", max compression
+gzip compressed data, was "clang_tidy_checker-0.5.0.tar", max compression
```

## Comparing `clang_tidy_checker-0.4.0.tar` & `clang_tidy_checker-0.5.0.tar`

### file list

```diff
@@ -1,13 +1,16 @@
--rw-r--r--   0        0        0      201 2024-01-23 15:11:15.485816 clang_tidy_checker-0.4.0/README.md
--rw-r--r--   0        0        0        0 2024-01-23 15:11:15.515817 clang_tidy_checker-0.4.0/clang_tidy_checker/__init__.py
--rw-r--r--   0        0        0       94 2024-01-23 15:11:15.485816 clang_tidy_checker-0.4.0/clang_tidy_checker/__main__.py
--rw-r--r--   0        0        0     1259 2024-01-23 15:11:15.485816 clang_tidy_checker-0.4.0/clang_tidy_checker/check_files.py
--rw-r--r--   0        0        0     5796 2024-01-23 15:11:15.485816 clang_tidy_checker-0.4.0/clang_tidy_checker/clang_tidy_executor.py
--rw-r--r--   0        0        0     2043 2024-01-23 15:11:15.485816 clang_tidy_checker-0.4.0/clang_tidy_checker/command_executor.py
--rw-r--r--   0        0        0     2266 2024-01-23 15:11:15.485816 clang_tidy_checker-0.4.0/clang_tidy_checker/config.py
--rw-r--r--   0        0        0     2707 2024-01-23 15:11:15.485816 clang_tidy_checker-0.4.0/clang_tidy_checker/main.py
--rw-r--r--   0        0        0      602 2024-01-23 15:11:15.485816 clang_tidy_checker-0.4.0/clang_tidy_checker/search_checked_files.py
--rw-r--r--   0        0        0      743 2024-01-23 15:11:15.486816 clang_tidy_checker-0.4.0/clang_tidy_checker/search_clang_tidy.py
--rw-r--r--   0        0        0     2734 2024-01-23 15:11:15.486816 clang_tidy_checker-0.4.0/clang_tidy_checker/source_hash_calculator.py
--rw-r--r--   0        0        0     1915 2024-01-23 15:11:15.487816 clang_tidy_checker-0.4.0/pyproject.toml
--rw-r--r--   0        0        0     1432 1970-01-01 00:00:00.000000 clang_tidy_checker-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0      201 2024-04-03 14:51:05.235818 clang_tidy_checker-0.5.0/README.md
+-rw-r--r--   0        0        0        0 2024-04-03 14:51:05.263818 clang_tidy_checker-0.5.0/clang_tidy_checker/__init__.py
+-rw-r--r--   0        0        0       94 2024-04-03 14:51:05.236818 clang_tidy_checker-0.5.0/clang_tidy_checker/__main__.py
+-rw-r--r--   0        0        0      575 2024-04-03 14:51:05.236818 clang_tidy_checker-0.5.0/clang_tidy_checker/cache_model.py
+-rw-r--r--   0        0        0     3338 2024-04-03 14:51:05.236818 clang_tidy_checker-0.5.0/clang_tidy_checker/cache_table.py
+-rw-r--r--   0        0        0     1259 2024-04-03 14:51:05.236818 clang_tidy_checker-0.5.0/clang_tidy_checker/check_files.py
+-rw-r--r--   0        0        0      200 2024-04-03 14:51:05.236818 clang_tidy_checker-0.5.0/clang_tidy_checker/check_result.py
+-rw-r--r--   0        0        0     4890 2024-04-03 14:51:05.236818 clang_tidy_checker-0.5.0/clang_tidy_checker/clang_tidy_executor.py
+-rw-r--r--   0        0        0     2043 2024-04-03 14:51:05.236818 clang_tidy_checker-0.5.0/clang_tidy_checker/command_executor.py
+-rw-r--r--   0        0        0     2646 2024-04-03 14:51:05.236818 clang_tidy_checker-0.5.0/clang_tidy_checker/config.py
+-rw-r--r--   0        0        0     2707 2024-04-03 14:51:05.236818 clang_tidy_checker-0.5.0/clang_tidy_checker/main.py
+-rw-r--r--   0        0        0      602 2024-04-03 14:51:05.236818 clang_tidy_checker-0.5.0/clang_tidy_checker/search_checked_files.py
+-rw-r--r--   0        0        0      743 2024-04-03 14:51:05.236818 clang_tidy_checker-0.5.0/clang_tidy_checker/search_clang_tidy.py
+-rw-r--r--   0        0        0     2803 2024-04-03 14:51:05.236818 clang_tidy_checker-0.5.0/clang_tidy_checker/source_hash_calculator.py
+-rw-r--r--   0        0        0     1965 2024-04-03 14:51:05.237818 clang_tidy_checker-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0     1487 1970-01-01 00:00:00.000000 clang_tidy_checker-0.5.0/PKG-INFO
```

### Comparing `clang_tidy_checker-0.4.0/clang_tidy_checker/check_files.py` & `clang_tidy_checker-0.5.0/clang_tidy_checker/check_files.py`

 * *Files identical despite different names*

### Comparing `clang_tidy_checker-0.4.0/clang_tidy_checker/clang_tidy_executor.py` & `clang_tidy_checker-0.5.0/clang_tidy_checker/clang_tidy_executor.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,38 +1,28 @@
 """Class to execute clang-tidy."""
 
 import abc
-import dataclasses
 import logging
 import os
 import typing
 
-import msgpack
-
+from clang_tidy_checker.cache_table import create_cache_table_at
+from clang_tidy_checker.check_result import CheckResult
 from clang_tidy_checker.command_executor import CommandExecutor
 from clang_tidy_checker.config import Config
 from clang_tidy_checker.source_hash_calculator import SourceHashCalculator
 
 try:
     from typing import Self
 except ImportError:
     Self = typing.TypeVar("Self", bound="IClangTidyExecutor")  # type: ignore
 
 LOGGER = logging.getLogger(__name__)
 
 
-@dataclasses.dataclass
-class CheckResult:
-    """Class of the result of a check."""
-
-    exit_code: int
-    stdout: str
-    stderr: str
-
-
 class IClangTidyExecutor(abc.ABC):
     """Interface for clang-tidy executor."""
 
     @abc.abstractmethod
     async def __aenter__(self) -> Self:
         pass
 
@@ -120,76 +110,49 @@
             stdout=stdout,
             stderr=stderr,
         )
 
         return CheckResult(exit_code=exit_code, stdout=stdout, stderr=stderr)
 
 
-def get_cache_file_path(cache_dir: str, source_hash: str) -> str:
-    """Get the file path of cache file.
-
-    Args:
-        cache_dir (str): Path to the cache directory.
-        source_hash (str): Hash of the source code.
-
-    Returns:
-        str: Path to the cache file.
-    """
-    return os.path.join(
-        cache_dir, source_hash[-1], source_hash[-2], source_hash[-20:-2]
-    )
-
-
 class CachedClangTidyExecutor(IClangTidyExecutor):
     """Class to execute clang-tidy but with caching of results."""
 
     def __init__(self, config: Config) -> None:
         self._clang_tidy_executor = ClangTidyExecutor(config=config)
         self._source_hash_calculator = SourceHashCalculator(config=config)
         if config.cache_dir is None:
             raise ValueError("Cache directory is required for CachedClangTidyExecutor.")
         self._cache_dir = config.cache_dir
+        os.makedirs(config.cache_dir, exist_ok=True)
+        self._cache_table = create_cache_table_at(
+            f"{config.cache_dir}/clang_tidy_cache_v2.db",
+            max_cache_entries=config.max_cache_entries,
+        )
 
     async def __aenter__(self) -> Self:
         await self._clang_tidy_executor.__aenter__()
         await self._source_hash_calculator.__aenter__()
         return self
 
     async def __aexit__(self, exc_type, exc_value, traceback) -> None:
         await self._clang_tidy_executor.__aexit__(exc_type, exc_value, traceback)
         await self._source_hash_calculator.__aexit__(exc_type, exc_value, traceback)
 
     async def execute(self, *, input_file: str) -> CheckResult:
         source_hash = await self._source_hash_calculator.calculate(
             input_file=input_file
         )
-        cache_file_path = get_cache_file_path(
-            cache_dir=self._cache_dir, source_hash=source_hash
+
+        result = self._cache_table.load(source_hash=source_hash)
+        if result is None:
+            result = await self._clang_tidy_executor.execute(input_file=input_file)
+            self._cache_table.save(source_hash=source_hash, result=result)
+
+        write_result_log(
+            exit_code=result.exit_code,
+            input_file=input_file,
+            stdout=result.stdout,
+            stderr=result.stderr,
         )
-        if os.path.exists(cache_file_path):
-            with open(cache_file_path, "rb") as file:
-                result_dict = msgpack.unpack(file)
-            exit_code = int(result_dict["error_code"])
-            stdout = str(result_dict["stdout"])
-            stderr = str(result_dict["stderr"])
-
-            write_result_log(
-                exit_code=exit_code,
-                input_file=input_file,
-                stdout=stdout,
-                stderr=stderr,
-            )
-
-            return CheckResult(exit_code=exit_code, stdout=stdout, stderr=stderr)
-
-        result = await self._clang_tidy_executor.execute(input_file=input_file)
-        os.makedirs(os.path.dirname(cache_file_path), exist_ok=True)
-        with open(cache_file_path, "wb") as file:
-            msgpack.pack(
-                {
-                    "error_code": result.exit_code,
-                    "stdout": result.stdout,
-                    "stderr": result.stderr,
-                },
-                file,
-            )
+
         return result
```

### Comparing `clang_tidy_checker-0.4.0/clang_tidy_checker/command_executor.py` & `clang_tidy_checker-0.5.0/clang_tidy_checker/command_executor.py`

 * *Files identical despite different names*

### Comparing `clang_tidy_checker-0.4.0/clang_tidy_checker/config.py` & `clang_tidy_checker-0.5.0/clang_tidy_checker/config.py`

 * *Files 12% similar despite different names*

```diff
@@ -37,25 +37,32 @@
 
 # Key of extra arguments.
 EXTRA_ARGS_KEY = "extra_args"
 
 # Key of cache directory.
 CACHE_DIR_KEY = "cache_dir"
 
+# Key of the maximum number of entries in the cache.
+MAX_CACHE_ENTRIES_KEY = "max_cache_entries"
+
+# Default value of the maximum number of entries in the cache.
+DEFAULT_MAX_CACHE_ENTRIES_KEY = 1000
+
 
 @dataclasses.dataclass
 class Config:
     """Class of configuration."""
 
     clang_tidy_path: str
     build_dir: str
     show_progress: bool
     checked_file_patterns: typing.List[str]
     extra_args: typing.List[str]
     cache_dir: typing.Optional[str]
+    max_cache_entries: int
 
 
 async def parse_config_from_dict(config: dict) -> Config:
     """Parse configuration from dictionaries.
 
     Args:
         config (dict): Input dictionary.
@@ -79,15 +86,20 @@
 
     extra_args = [str(elem) for elem in config.get(EXTRA_ARGS_KEY, [])]
 
     cache_dir = config.get(CACHE_DIR_KEY, None)
     if cache_dir is not None:
         cache_dir = str(cache_dir)
 
+    max_cache_entries = int(
+        config.get(MAX_CACHE_ENTRIES_KEY, DEFAULT_MAX_CACHE_ENTRIES_KEY)
+    )
+
     return Config(
         clang_tidy_path=clang_tidy_path,
         build_dir=build_dir,
         show_progress=show_progress,
         checked_file_patterns=checked_file_patterns,
         extra_args=extra_args,
         cache_dir=cache_dir,
+        max_cache_entries=max_cache_entries,
     )
```

### Comparing `clang_tidy_checker-0.4.0/clang_tidy_checker/main.py` & `clang_tidy_checker-0.5.0/clang_tidy_checker/main.py`

 * *Files identical despite different names*

### Comparing `clang_tidy_checker-0.4.0/clang_tidy_checker/search_checked_files.py` & `clang_tidy_checker-0.5.0/clang_tidy_checker/search_checked_files.py`

 * *Files identical despite different names*

### Comparing `clang_tidy_checker-0.4.0/clang_tidy_checker/search_clang_tidy.py` & `clang_tidy_checker-0.5.0/clang_tidy_checker/search_clang_tidy.py`

 * *Files identical despite different names*

### Comparing `clang_tidy_checker-0.4.0/clang_tidy_checker/source_hash_calculator.py` & `clang_tidy_checker-0.5.0/clang_tidy_checker/source_hash_calculator.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """Class to calculate hash of source codes."""
 
 import asyncio
+import base64
 import hashlib
 import json
 import logging
 import os
 import shlex
 import typing
 
@@ -89,8 +90,10 @@
 
         Args:
             string (str): Input.
 
         Returns:
             str: Hash.
         """
-        return hashlib.sha256(string.encode()).hexdigest()
+        return base64.b64encode(hashlib.sha3_512(string.encode()).digest()).decode(
+            "ascii"
+        )
```

### Comparing `clang_tidy_checker-0.4.0/pyproject.toml` & `clang_tidy_checker-0.5.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "clang_tidy_checker"
-version = "0.4.0"
+version = "0.5.0"
 description = "Tool to check C / C++ source codes using clang-tidy."
 authors = ["Kenta Kabashima <kenta_program37@hotmail.co.jp>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://gitlab.com/MusicScience37Projects/tools/clang-tidy-checker"
 repository = "https://gitlab.com/MusicScience37Projects/tools/clang-tidy-checker.git"
 documentation = "https://musicscience37projects.gitlab.io/tools/clang-tidy-checker/"
@@ -16,24 +16,25 @@
     "Intended Audience :: Developers",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
     "Programming Language :: C",
     "Programming Language :: C++",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
+    "Programming Language :: Python :: 3.12",
     "Topic :: Software Development :: Quality Assurance",
     "Typing :: Typed",
 ]
 
 [tool.poetry.dependencies]
-python = ">=3.10,<3.12"
+python = ">=3.10,<3.13"
 PyYAML = ">=6"
 click = ">=8.1.6"
 tqdm = ">=4.65.0"
-msgpack = ">=1.0.7"
+sqlalchemy = ">=2.0.29"
 
 [tool.poetry.group.dev.dependencies]
 pre-commit = "^3.6.0"
 Sphinx = "^7.2.6"
 black = "^23.12.1"
 doc8 = "^1.1.1"
 pylint = "^3.0.3"
```

### Comparing `clang_tidy_checker-0.4.0/PKG-INFO` & `clang_tidy_checker-0.5.0/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,32 +1,33 @@
 Metadata-Version: 2.1
 Name: clang_tidy_checker
-Version: 0.4.0
+Version: 0.5.0
 Summary: Tool to check C / C++ source codes using clang-tidy.
 Home-page: https://gitlab.com/MusicScience37Projects/tools/clang-tidy-checker
 License: MIT
 Keywords: clang-tidy,c++
 Author: Kenta Kabashima
 Author-email: kenta_program37@hotmail.co.jp
-Requires-Python: >=3.10,<3.12
+Requires-Python: >=3.10,<3.13
 Classifier: Development Status :: 4 - Beta
 Classifier: Framework :: AsyncIO
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: C
 Classifier: Programming Language :: C++
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Software Development :: Quality Assurance
 Classifier: Typing :: Typed
 Requires-Dist: PyYAML (>=6)
 Requires-Dist: click (>=8.1.6)
-Requires-Dist: msgpack (>=1.0.7)
+Requires-Dist: sqlalchemy (>=2.0.29)
 Requires-Dist: tqdm (>=4.65.0)
 Project-URL: Documentation, https://musicscience37projects.gitlab.io/tools/clang-tidy-checker/
 Project-URL: Repository, https://gitlab.com/MusicScience37Projects/tools/clang-tidy-checker.git
 Description-Content-Type: text/markdown
 
 # clang-tidy-checker
```

