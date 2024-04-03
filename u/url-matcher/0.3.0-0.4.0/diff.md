# Comparing `tmp/url-matcher-0.3.0.tar.gz` & `tmp/url-matcher-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "url-matcher-0.3.0.tar", last modified: Thu Sep 21 08:14:29 2023, max compression
+gzip compressed data, was "url-matcher-0.4.0.tar", last modified: Wed Apr  3 07:02:22 2024, max compression
```

## Comparing `url-matcher-0.3.0.tar` & `url-matcher-0.4.0.tar`

### file list

```diff
@@ -1,20 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-21 08:14:29.001555 url-matcher-0.3.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1509 2023-09-21 08:14:19.000000 url-matcher-0.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3773 2023-09-21 08:14:29.001555 url-matcher-0.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2990 2023-09-21 08:14:19.000000 url-matcher-0.3.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)       85 2023-09-21 08:14:19.000000 url-matcher-0.3.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-09-21 08:14:29.001555 url-matcher-0.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1312 2023-09-21 08:14:19.000000 url-matcher-0.3.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-21 08:14:29.001555 url-matcher-0.3.0/url_matcher/
--rw-r--r--   0 runner    (1001) docker     (127)       80 2023-09-21 08:14:19.000000 url-matcher-0.3.0/url_matcher/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       22 2023-09-21 08:14:19.000000 url-matcher-0.3.0/url_matcher/__version__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3386 2023-09-21 08:14:19.000000 url-matcher-0.3.0/url_matcher/example.py
--rw-r--r--   0 runner    (1001) docker     (127)     8205 2023-09-21 08:14:19.000000 url-matcher-0.3.0/url_matcher/matcher.py
--rw-r--r--   0 runner    (1001) docker     (127)     9465 2023-09-21 08:14:19.000000 url-matcher-0.3.0/url_matcher/patterns.py
--rw-r--r--   0 runner    (1001) docker     (127)      656 2023-09-21 08:14:19.000000 url-matcher-0.3.0/url_matcher/util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-21 08:14:29.001555 url-matcher-0.3.0/url_matcher.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3773 2023-09-21 08:14:28.000000 url-matcher-0.3.0/url_matcher.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      357 2023-09-21 08:14:28.000000 url-matcher-0.3.0/url_matcher.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-09-21 08:14:28.000000 url-matcher-0.3.0/url_matcher.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2023-09-21 08:14:28.000000 url-matcher-0.3.0/url_matcher.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2023-09-21 08:14:28.000000 url-matcher-0.3.0/url_matcher.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 07:02:22.372842 url-matcher-0.4.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1509 2024-04-03 07:02:14.000000 url-matcher-0.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3855 2024-04-03 07:02:22.372842 url-matcher-0.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2990 2024-04-03 07:02:14.000000 url-matcher-0.4.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-04-03 07:02:14.000000 url-matcher-0.4.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-03 07:02:22.372842 url-matcher-0.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1362 2024-04-03 07:02:14.000000 url-matcher-0.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 07:02:22.368842 url-matcher-0.4.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     5760 2024-04-03 07:02:14.000000 url-matcher-0.4.0/tests/test_matcher.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1339 2024-04-03 07:02:14.000000 url-matcher-0.4.0/tests/test_patterns.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 07:02:22.372842 url-matcher-0.4.0/url_matcher/
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2024-04-03 07:02:14.000000 url-matcher-0.4.0/url_matcher/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-03 07:02:14.000000 url-matcher-0.4.0/url_matcher/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3395 2024-04-03 07:02:14.000000 url-matcher-0.4.0/url_matcher/example.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8370 2024-04-03 07:02:14.000000 url-matcher-0.4.0/url_matcher/matcher.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9465 2024-04-03 07:02:14.000000 url-matcher-0.4.0/url_matcher/patterns.py
+-rw-r--r--   0 runner    (1001) docker     (127)      656 2024-04-03 07:02:14.000000 url-matcher-0.4.0/url_matcher/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 07:02:22.372842 url-matcher-0.4.0/url_matcher.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3855 2024-04-03 07:02:22.000000 url-matcher-0.4.0/url_matcher.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      402 2024-04-03 07:02:22.000000 url-matcher-0.4.0/url_matcher.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 07:02:22.000000 url-matcher-0.4.0/url_matcher.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-03 07:02:22.000000 url-matcher-0.4.0/url_matcher.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-03 07:02:22.000000 url-matcher-0.4.0/url_matcher.egg-info/top_level.txt
```

### Comparing `url-matcher-0.3.0/LICENSE` & `url-matcher-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `url-matcher-0.3.0/PKG-INFO` & `url-matcher-0.4.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,27 +1,29 @@
 Metadata-Version: 2.1
 Name: url-matcher
-Version: 0.3.0
+Version: 0.4.0
 Summary: URL matching rules library to connect URLs with resources
 Home-page: https://github.com/zytedata/url-matcher
 Author: Zyte Group Ltd
 Author-email: info@zyte.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 License-File: LICENSE
+Requires-Dist: tldextract>=1.2
 
 ===========
 url-matcher
 ===========
 
 .. image:: https://img.shields.io/pypi/v/url-matcher.svg
    :target: https://pypi.python.org/pypi/url-matcher
```

### Comparing `url-matcher-0.3.0/README.rst` & `url-matcher-0.4.0/README.rst`

 * *Files identical despite different names*

### Comparing `url-matcher-0.3.0/setup.py` & `url-matcher-0.4.0/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -38,9 +38,10 @@
         "Natural Language :: English",
         "Operating System :: OS Independent",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
+        "Programming Language :: Python :: 3.12",
     ],
 )
```

### Comparing `url-matcher-0.3.0/url_matcher/example.py` & `url-matcher-0.4.0/url_matcher/example.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 Example of usage of the URLMatcher library
 """
+
 import dataclasses
 import random
 import time
 from collections import Counter
 
 from url_matcher import Patterns, URLMatcher
 from url_matcher.matcher import IncludePatternsWithoutDomainError
@@ -96,10 +97,10 @@
 for domain, url in urls:
     match = matcher.match(url)
     counter[bool(match)] += 1
     assert match and f"{domain}" in match
 end = time.perf_counter()
 
 # It took in my machine ~ 0.04 millis per URL
-print(f"{((end-start)/N_URLS)*1000:.3f} milliseconds per URL. Total {end-start} seconds to match {N_URLS} URLs")
+print(f"{((end - start) / N_URLS) * 1000:.3f} milliseconds per URL. Total {end - start} seconds to match {N_URLS} URLs")
 
 print("Everything worked fine!")
```

### Comparing `url-matcher-0.3.0/url_matcher/matcher.py` & `url-matcher-0.4.0/url_matcher/matcher.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """
 The matcher module contains the UrlMatcher class.
 """
+
 from dataclasses import dataclass, field
 from itertools import chain
-from typing import Any, Dict, Iterable, List, Mapping, Optional, Tuple, Union
+from typing import Any, Dict, Iterable, Iterator, List, Mapping, Optional, Tuple, Union
 
 from url_matcher.patterns import PatternMatcher, get_pattern_domain, hierarchical_str
 from url_matcher.util import get_domain
 
 
 @dataclass(init=False, frozen=True)
 class Patterns:
@@ -30,15 +31,16 @@
         #     * https://github.com/python/cpython/blob/v3.10.2/Lib/dataclasses.py#L1117-L1120
         object.__setattr__(self, "include", tuple(include))
         object.__setattr__(self, "exclude", tuple(exclude or []))
         object.__setattr__(self, "priority", priority)
 
     def get_domains(self) -> List[str]:
         domains = [get_pattern_domain(pattern) for pattern in self.include]
-        return [domain for domain in domains if domain]
+        # remove duplicate domains preserving the order
+        return list(dict.fromkeys(domain for domain in domains if domain))
 
     def get_includes_without_domain(self) -> List[str]:
         return [pattern for pattern in self.include if get_pattern_domain(pattern) is None]
 
     def all_includes_have_domain(self) -> bool:
         """Return true if all the include patterns have a domain"""
         return not self.get_includes_without_domain()
@@ -146,19 +148,21 @@
         if patterns.is_universal_pattern():
             self._del_matcher("", identifier)
 
     def get(self, identifier: Any) -> Optional[Patterns]:
         return self.patterns.get(identifier)
 
     def match(self, url: str) -> Optional[Any]:
+        return next(self.match_all(url), None)
+
+    def match_all(self, url: str) -> Iterator[Any]:
         domain = get_domain(url)
         for matcher in chain(self.matchers_by_domain.get(domain) or [], self.matchers_by_domain.get("") or []):
             if matcher.match(url):
-                return matcher.identifier
-        return None
+                yield matcher.identifier
 
     def _sort_domain(self, domain: str):
         """
         Sort all the rules within a domain so that the matching can be done in sequence:
         the first rule matching wins.
 
         A total ordering is defined. This is ensured by using including
```

### Comparing `url-matcher-0.3.0/url_matcher/patterns.py` & `url-matcher-0.4.0/url_matcher/patterns.py`

 * *Files identical despite different names*

### Comparing `url-matcher-0.3.0/url_matcher/util.py` & `url-matcher-0.4.0/url_matcher/util.py`

 * *Files identical despite different names*

### Comparing `url-matcher-0.3.0/url_matcher.egg-info/PKG-INFO` & `url-matcher-0.4.0/url_matcher.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,27 +1,29 @@
 Metadata-Version: 2.1
 Name: url-matcher
-Version: 0.3.0
+Version: 0.4.0
 Summary: URL matching rules library to connect URLs with resources
 Home-page: https://github.com/zytedata/url-matcher
 Author: Zyte Group Ltd
 Author-email: info@zyte.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 License-File: LICENSE
+Requires-Dist: tldextract>=1.2
 
 ===========
 url-matcher
 ===========
 
 .. image:: https://img.shields.io/pypi/v/url-matcher.svg
    :target: https://pypi.python.org/pypi/url-matcher
```

