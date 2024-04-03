# Comparing `tmp/pytest_check_links-0.9.3.tar.gz` & `tmp/pytest_check_links-4.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
+gzip compressed data, was "dist/pytest_check_links-4.3.3.tar", last modified: Wed Jul 29 20:46:32 2020, max compression
```

## Comparing `pytest_check_links-0.9.3.tar` & `pytest_check_links-4.3.3.tar`

### file list

```diff
@@ -1,37 +1,41 @@
--rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 pytest_check_links-0.9.3/.git-blame-ignore-revs
--rw-r--r--   0        0        0     2268 2020-02-02 00:00:00.000000 pytest_check_links-0.9.3/.pre-commit-config.yaml
--rw-r--r--   0        0        0    11889 2020-02-02 00:00:00.000000 pytest_check_links-0.9.3/CHANGELOG.md
--rw-r--r--   0        0        0      857 2020-02-02 00:00:00.000000 pytest_check_links-0.9.3/RELEASE.md
--rw-r--r--   0        0        0      327 2020-02-02 00:00:00.000000 pytest_check_links-0.9.3/.github/dependabot.yml
--rw-r--r--   0        0        0      320 2020-02-02 00:00:00.000000 pytest_check_links-0.9.3/.github/workflows/enforce-label.yml
--rw-r--r--   0        0        0     1689 2020-02-02 00:00:00.000000 pytest_check_links-0.9.3/.github/workflows/prep-release.yml
--rw-r--r--   0        0        0      928 2020-02-02 00:00:00.000000 pytest_check_links-0.9.3/.github/workflows/publish-changelog.yml
--rw-r--r--   0        0        0     1798 2020-02-02 00:00:00.000000 pytest_check_links-0.9.3/.github/workflows/publish-release.yml
--rw-r--r--   0        0        0     4643 2020-02-02 00:00:00.000000 pytest_check_links-0.9.3/.github/workflows/tests.yml
--rw-r--r--   0        0        0      236 2020-02-02 00:00:00.000000 pytest_check_links-0.9.3/examples/anchors_other.html
--rw-r--r--   0        0        0      280 2020-02-02 00:00:00.000000 pytest_check_links-0.9.3/examples/anchors_remote.html
--rw-r--r--   0        0        0      403 2020-02-02 00:00:00.000000 pytest_check_links-0.9.3/examples/anchors_self.html
--rw-r--r--   0        0        0      256 2020-02-02 00:00:00.000000 pytest_check_links-0.9.3/examples/httpbin.md
--rw-r--r--   0        0        0     1494 2020-02-02 00:00:00.000000 pytest_check_links-0.9.3/examples/linkcheck.ipynb
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 pytest_check_links-0.9.3/examples/markdown.md
--rw-r--r--   0        0        0      684 2020-02-02 00:00:00.000000 pytest_check_links-0.9.3/examples/rst.rst
--rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 pytest_check_links-0.9.3/examples/setup.cfg
--rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 pytest_check_links-0.9.3/examples/nested/nested.md
--rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 pytest_check_links-0.9.3/examples/nested/nested.rst
--rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 pytest_check_links-0.9.3/pytest_check_links/__init__.py
--rw-r--r--   0        0        0      723 2020-02-02 00:00:00.000000 pytest_check_links-0.9.3/pytest_check_links/__main__.py
--rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 pytest_check_links-0.9.3/pytest_check_links/_version.py
--rw-r--r--   0        0        0     2017 2020-02-02 00:00:00.000000 pytest_check_links-0.9.3/pytest_check_links/args.py
--rw-r--r--   0        0        0    16317 2020-02-02 00:00:00.000000 pytest_check_links-0.9.3/pytest_check_links/plugin.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pytest_check_links-0.9.3/pytest_check_links/py.typed
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pytest_check_links-0.9.3/test/__init__.py
--rw-r--r--   0        0        0      444 2020-02-02 00:00:00.000000 pytest_check_links-0.9.3/test/conftest.py
--rw-r--r--   0        0        0      670 2020-02-02 00:00:00.000000 pytest_check_links-0.9.3/test/test_anchors.py
--rw-r--r--   0        0        0     3589 2020-02-02 00:00:00.000000 pytest_check_links-0.9.3/test/test_cache.py
--rw-r--r--   0        0        0     2167 2020-02-02 00:00:00.000000 pytest_check_links-0.9.3/test/test_check_links.py
--rw-r--r--   0        0        0     1163 2020-02-02 00:00:00.000000 pytest_check_links-0.9.3/test/test_cli.py
--rw-r--r--   0        0        0     1125 2020-02-02 00:00:00.000000 pytest_check_links-0.9.3/.gitignore
--rw-r--r--   0        0        0     1562 2020-02-02 00:00:00.000000 pytest_check_links-0.9.3/LICENSE
--rw-r--r--   0        0        0     3957 2020-02-02 00:00:00.000000 pytest_check_links-0.9.3/README.md
--rw-r--r--   0        0        0     5101 2020-02-02 00:00:00.000000 pytest_check_links-0.9.3/pyproject.toml
--rw-r--r--   0        0        0     7033 2020-02-02 00:00:00.000000 pytest_check_links-0.9.3/PKG-INFO
+drwxr-xr-x   0 stslve   (1919889055) ANT\Domain Users (1896053708)        0 2020-07-29 20:46:32.000000 pytest_check_links-4.3.3/
+-rw-r--r--   0 stslve   (1919889055) ANT\Domain Users (1896053708)      366 2020-05-02 09:02:00.000000 pytest_check_links-4.3.3/.travis.yml
+-rw-r--r--   0 stslve   (1919889055) ANT\Domain Users (1896053708)      226 2020-07-29 20:46:32.000000 pytest_check_links-4.3.3/AUTHORS
+-rw-r--r--   0 stslve   (1919889055) ANT\Domain Users (1896053708)     1068 2020-07-29 20:21:45.000000 pytest_check_links-4.3.3/CHANGELOG.md
+-rw-r--r--   0 stslve   (1919889055) ANT\Domain Users (1896053708)     2295 2020-07-29 20:46:32.000000 pytest_check_links-4.3.3/ChangeLog
+-rw-r--r--   0 stslve   (1919889055) ANT\Domain Users (1896053708)     1562 2020-04-11 21:53:26.000000 pytest_check_links-4.3.3/LICENSE
+-rw-r--r--   0 stslve   (1919889055) ANT\Domain Users (1896053708)     3991 2020-07-29 20:46:32.000000 pytest_check_links-4.3.3/PKG-INFO
+-rw-r--r--   0 stslve   (1919889055) ANT\Domain Users (1896053708)     2555 2020-05-04 10:58:32.000000 pytest_check_links-4.3.3/README.md
+-rw-r--r--   0 stslve   (1919889055) ANT\Domain Users (1896053708)      168 2020-04-21 15:12:53.000000 pytest_check_links-4.3.3/RELEASE.md
+drwxr-xr-x   0 stslve   (1919889055) ANT\Domain Users (1896053708)        0 2020-07-29 20:46:32.000000 pytest_check_links-4.3.3/examples/
+-rw-r--r--   0 stslve   (1919889055) ANT\Domain Users (1896053708)      236 2020-04-21 15:04:48.000000 pytest_check_links-4.3.3/examples/anchors_other.html
+-rw-r--r--   0 stslve   (1919889055) ANT\Domain Users (1896053708)      256 2020-05-02 09:02:00.000000 pytest_check_links-4.3.3/examples/anchors_remote.html
+-rw-r--r--   0 stslve   (1919889055) ANT\Domain Users (1896053708)      383 2020-07-29 20:20:27.000000 pytest_check_links-4.3.3/examples/anchors_self.html
+-rw-r--r--   0 stslve   (1919889055) ANT\Domain Users (1896053708)      256 2020-05-02 09:02:00.000000 pytest_check_links-4.3.3/examples/httpbin.md
+-rw-r--r--   0 stslve   (1919889055) ANT\Domain Users (1896053708)     1353 2020-03-30 09:40:43.000000 pytest_check_links-4.3.3/examples/linkcheck.ipynb
+-rw-r--r--   0 stslve   (1919889055) ANT\Domain Users (1896053708)      974 2020-03-30 09:40:43.000000 pytest_check_links-4.3.3/examples/markdown.md
+-rw-r--r--   0 stslve   (1919889055) ANT\Domain Users (1896053708)      687 2020-03-30 09:40:43.000000 pytest_check_links-4.3.3/examples/rst.rst
+-rw-r--r--   0 stslve   (1919889055) ANT\Domain Users (1896053708)       41 2020-03-30 09:40:43.000000 pytest_check_links-4.3.3/pytest.ini
+drwxr-xr-x   0 stslve   (1919889055) ANT\Domain Users (1896053708)        0 2020-07-29 20:46:32.000000 pytest_check_links-4.3.3/pytest_check_links/
+-rw-r--r--   0 stslve   (1919889055) ANT\Domain Users (1896053708)        0 2020-03-30 09:40:43.000000 pytest_check_links-4.3.3/pytest_check_links/__init__.py
+-rw-r--r--   0 stslve   (1919889055) ANT\Domain Users (1896053708)      579 2020-03-30 09:40:43.000000 pytest_check_links-4.3.3/pytest_check_links/__main__.py
+-rw-r--r--   0 stslve   (1919889055) ANT\Domain Users (1896053708)     1395 2020-05-02 09:02:00.000000 pytest_check_links-4.3.3/pytest_check_links/args.py
+-rw-r--r--   0 stslve   (1919889055) ANT\Domain Users (1896053708)    12742 2020-07-29 20:20:27.000000 pytest_check_links-4.3.3/pytest_check_links/plugin.py
+drwxr-xr-x   0 stslve   (1919889055) ANT\Domain Users (1896053708)        0 2020-07-29 20:46:32.000000 pytest_check_links-4.3.3/pytest_check_links.egg-info/
+-rw-r--r--   0 stslve   (1919889055) ANT\Domain Users (1896053708)     3991 2020-07-29 20:46:32.000000 pytest_check_links-4.3.3/pytest_check_links.egg-info/PKG-INFO
+-rw-r--r--   0 stslve   (1919889055) ANT\Domain Users (1896053708)      834 2020-07-29 20:46:32.000000 pytest_check_links-4.3.3/pytest_check_links.egg-info/SOURCES.txt
+-rw-r--r--   0 stslve   (1919889055) ANT\Domain Users (1896053708)        1 2020-07-29 20:46:32.000000 pytest_check_links-4.3.3/pytest_check_links.egg-info/dependency_links.txt
+-rw-r--r--   0 stslve   (1919889055) ANT\Domain Users (1896053708)      125 2020-07-29 20:46:32.000000 pytest_check_links-4.3.3/pytest_check_links.egg-info/entry_points.txt
+-rw-r--r--   0 stslve   (1919889055) ANT\Domain Users (1896053708)        1 2020-03-30 09:50:04.000000 pytest_check_links-4.3.3/pytest_check_links.egg-info/not-zip-safe
+-rw-r--r--   0 stslve   (1919889055) ANT\Domain Users (1896053708)       47 2020-07-29 20:46:32.000000 pytest_check_links-4.3.3/pytest_check_links.egg-info/pbr.json
+-rw-r--r--   0 stslve   (1919889055) ANT\Domain Users (1896053708)       82 2020-07-29 20:46:32.000000 pytest_check_links-4.3.3/pytest_check_links.egg-info/requires.txt
+-rw-r--r--   0 stslve   (1919889055) ANT\Domain Users (1896053708)       19 2020-07-29 20:46:32.000000 pytest_check_links-4.3.3/pytest_check_links.egg-info/top_level.txt
+-rw-r--r--   0 stslve   (1919889055) ANT\Domain Users (1896053708)       60 2020-07-29 20:20:27.000000 pytest_check_links-4.3.3/requirements.txt
+-rw-r--r--   0 stslve   (1919889055) ANT\Domain Users (1896053708)      909 2020-07-29 20:46:32.000000 pytest_check_links-4.3.3/setup.cfg
+-rw-r--r--   0 stslve   (1919889055) ANT\Domain Users (1896053708)      336 2020-04-11 21:53:26.000000 pytest_check_links-4.3.3/setup.py
+drwxr-xr-x   0 stslve   (1919889055) ANT\Domain Users (1896053708)        0 2020-07-29 20:46:32.000000 pytest_check_links-4.3.3/test/
+-rw-r--r--   0 stslve   (1919889055) ANT\Domain Users (1896053708)      120 2020-05-02 09:02:00.000000 pytest_check_links-4.3.3/test/__init__.py
+-rw-r--r--   0 stslve   (1919889055) ANT\Domain Users (1896053708)       30 2020-03-30 09:40:43.000000 pytest_check_links-4.3.3/test/conftest.py
+-rw-r--r--   0 stslve   (1919889055) ANT\Domain Users (1896053708)      791 2020-07-29 20:20:27.000000 pytest_check_links-4.3.3/test/test_anchors.py
+-rw-r--r--   0 stslve   (1919889055) ANT\Domain Users (1896053708)     3661 2020-05-02 09:02:00.000000 pytest_check_links-4.3.3/test/test_cache.py
+-rw-r--r--   0 stslve   (1919889055) ANT\Domain Users (1896053708)      800 2020-05-02 09:02:00.000000 pytest_check_links-4.3.3/test/test_check_links.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `pytest_check_links-0.9.3/examples/linkcheck.ipynb` & `pytest_check_links-4.3.3/examples/linkcheck.ipynb`

 * *Files 23% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9675925925925926%*

 * *Differences: {"'cells'": "{2: {'source': {insert: [(14, '[markdown absolute](/tmp)')], delete: [16, 14, 13]}}, "*

 * *            'delete: [3]}'}*

```diff
@@ -42,23 +42,16 @@
                 "\n",
                 "[markdown internal](#hash)\n",
                 "\n",
                 "[markdown local good](./linkcheck.ipynb)\n",
                 "\n",
                 "[markdown local bad](doesntexist.html)\n",
                 "\n",
-                "[markdown absolute](/tmp)\n",
-                "\n",
-                "[markdown link to ignore](http://example.com/404)"
+                "[markdown absolute](/tmp)"
             ]
-        },
-        {
-            "cell_type": "markdown",
-            "metadata": {},
-            "source": []
         }
     ],
     "metadata": {
         "kernelspec": {
             "display_name": "Python 3",
             "language": "python",
             "name": "python3"
```

### Comparing `pytest_check_links-0.9.3/examples/markdown.md` & `pytest_check_links-4.3.3/examples/markdown.md`

 * *Files 24% similar despite different names*

```diff
@@ -2,26 +2,26 @@
 
 [I'm an inline-style link](https://www.google.com)
 
 [I'm an inline-style link that 404s](http://example.com/404)
 
 [I'm an inline-style link with title](https://www.google.com "Google's Homepage")
 
-[I'm a reference-style link][arbitrary case-insensitive reference text]
+[I'm a reference-style link][Arbitrary case-insensitive reference text]
 
 [I'm a relative reference to a repository file](./markdown.md)
 
 [I'm a relative reference to a missing file](./missing)
 
 [You can use numbers for reference-style link definitions][1]
 
 Or leave it empty and use the [link text itself].
 
-URLs in angle brackets will automatically get turned into links.
-<http://www.example.com> and sometimes
-example.com (but not on GitHub, for example). This will 404: <http://www.example.com/404>
+URLs and URLs in angle brackets will automatically get turned into links.
+http://www.example.com or <http://www.example.com> and sometimes
+example.com (but not on GitHub, for example). These will 404: http://example.com/404 <http://www.example.com/404>
 
 Some text to show that the reference links can follow later.
 
-[1]: http://slashdot.org
 [arbitrary case-insensitive reference text]: https://www.mozilla.org
-[link text itself]: https://www.w3.org
+[1]: http://slashdot.org
+[link text itself]: http://www.reddit.com
```

### Comparing `pytest_check_links-0.9.3/examples/rst.rst` & `pytest_check_links-4.3.3/examples/rst.rst`

 * *Files 2% similar despite different names*

```diff
@@ -11,13 +11,13 @@
 
 `I’m a relative reference to a repository file <./rst.rst>`__
 
 `You can use numbers for reference-style link
 definitions <http://slashdot.org>`__
 
 Or leave it empty and use the `link text
-itself <https://www.w3.org>`__.
+itself <http://www.reddit.com>`__.
 
 URLs will automatically get turned into
 links. http://www.example.com or http://www.example.com/404.
 
 Some text to show that the reference links can follow later.
```

### Comparing `pytest_check_links-0.9.3/pytest_check_links/plugin.py` & `pytest_check_links-4.3.3/pytest_check_links/plugin.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,469 +1,365 @@
-"""pytest-check-links plugin."""
-from __future__ import annotations
-
+from docutils.core import publish_parts
+import io
 import os
-import re
 import time
 import warnings
-from pathlib import Path
-from typing import Any, Generator, cast
-from xml.etree.ElementTree import Element
 
 import html5lib
 import pytest
-from docutils.core import publish_parts
-from requests import Request, Response, Session
-from requests.utils import unquote  # type:ignore[attr-defined]
+from requests import Session, Request
+from requests.compat import unquote
 
-from .args import StoreCacheAction, StoreExtensionsAction
+from .args import StoreExtensionsAction, StoreCacheAction
 
-_ENC = "utf8"
+_ENC = 'utf8'
 
-default_extensions = {".md", ".rst", ".html", ".ipynb"}
-supported_extensions = {".md", ".rst", ".html", ".ipynb"}
+default_extensions = {'.md', '.rst', '.html', '.ipynb'}
+supported_extensions = {'.md', '.rst', '.html', '.ipynb'}
 
-default_cache = {
-    "cache_name": ".pytest-check-links-cache",
-    "backend": None,
-    "expire_after": None,
-    "allowable_codes": list(range(200, 512)),
-}
+default_cache = dict(
+    cache_name='.pytest-check-links-cache',
+    backend=None,
+    expire_after=None,
+    allowable_codes=list(range(200, 512)),
+)
 
 
-def pytest_addoption(parser: pytest.Parser) -> None:
-    """Add options to pytest."""
+def pytest_addoption(parser):
     group = parser.getgroup("general")
-    group.addoption("--check-links", action="store_true", help="Check links for validity")
-    group.addoption("--check-anchors", action="store_true", help="Check link anchors for validity")
-    group.addoption(
-        "--links-ext",
-        action=StoreExtensionsAction,
+    group.addoption('--check-links', action='store_true',
+        help="Check links for validity")
+    group.addoption('--check-anchors', action='store_true',
+        help="Check link anchors for validity")
+    group.addoption('--links-ext', action=StoreExtensionsAction,
         default=default_extensions,
         help="Which file extensions to check links for, "
-        "as a comma-separated list of values. Supported "
-        "extensions are: %s." % extensions_str(supported_extensions),
-    )
-    group.addoption(
-        "--check-links-ignore",
-        action="append",
-        help="A list of regular expressions that match URIs that should not be checked.",
-    )
-    group.addoption(
-        "--check-links-cache", action="store_true", help="Cache requests when checking links"
-    )
-    group.addoption("--check-links-cache-name", action=StoreCacheAction, help="Name of link cache")
-    group.addoption(
-        "--check-links-cache-backend", action=StoreCacheAction, help="Cache persistence backend"
-    )
-    group.addoption(
-        "--check-links-cache-expire-after",
-        action=StoreCacheAction,
-        help="Time to cache link responses (seconds)",
-    )
-    group.addoption(
-        "--check-links-cache-allowable-codes",
-        action=StoreCacheAction,
-        help="HTTP response codes to cache",
-    )
-    group.addoption(
-        "--check-links-cache-backend-opt",
-        action=StoreCacheAction,
-        help="Backend-specific options for link cache, specified as `opt:value`",
-    )
+             "as a comma-separated list of values. Supported "
+             "extensions are: %s." %
+                extensions_str(supported_extensions))
+
+    group.addoption('--check-links-cache', action='store_true',
+        help="Cache requests when checking links")
+    group.addoption('--check-links-cache-name', action=StoreCacheAction,
+        help="Name of link cache")
+    group.addoption('--check-links-cache-backend', action=StoreCacheAction,
+        help="Cache persistence backend")
+    group.addoption('--check-links-cache-expire-after', action=StoreCacheAction,
+        help="Time to cache link responses (seconds)")
+    group.addoption('--check-links-cache-allowable-codes', action=StoreCacheAction,
+        help="HTTP response codes to cache")
+    group.addoption('--check-links-cache-backend-opt', action=StoreCacheAction,
+        help="Backend-specific options for link cache, specfied as `opt:value`")
 
 
-def pytest_configure(config: pytest.Config) -> None:
-    """Configure pytest."""
+def pytest_configure(config):
     if config.option.links_ext:
         validate_extensions(config.option.links_ext)
 
 
-def pytest_collect_file(path: Any, parent: pytest.Collector) -> CheckLinks | None:
-    """Add pytest file collection filter."""
+def pytest_collect_file(path, parent):
     config = parent.config
-    ignore_links = config.option.check_links_ignore
-
     if config.option.check_links:
         requests_session = ensure_requests_session(config)
         if path.ext.lower() in config.option.links_ext:
-            path_obj = Path(path)
             check_anchors = config.option.check_anchors
             if hasattr(CheckLinks, "from_parent"):
-                return cast(
-                    CheckLinks,
-                    CheckLinks.from_parent(
-                        parent,
-                        path=path_obj,
-                        requests_session=requests_session,
-                        check_anchors=check_anchors,
-                        ignore_links=ignore_links,
-                    ),
-                )
-            return CheckLinks(
-                path=path_obj,
-                parent=parent,
-                requests_session=requests_session,
-                check_anchors=check_anchors,
-                ignore_links=ignore_links,
-            )
-    return None
+                return CheckLinks.from_parent(parent, fspath=path, requests_session=requests_session, check_anchors=check_anchors)
+            return CheckLinks(fspath=path, parent=parent, requests_session=requests_session, check_anchors=check_anchors)
 
-
-def ensure_requests_session(config: pytest.Config) -> Session:
-    """Build the singleton requests.Session (or subclass)"""
+def ensure_requests_session(config):
+    """Build the singleton requests.Session (or subclass)
+    """
     session_attr = "check_links_requests_session"
+
     if not hasattr(config.option, session_attr):
         if config.option.check_links_cache:
             from requests_cache import CachedSession
-
             conf_kwargs = getattr(config.option, "check_links_cache_kwargs", {})
             kwargs = dict(default_cache)
             kwargs.update(conf_kwargs)
-            requests_session = CachedSession(**kwargs)  # type:ignore[arg-type]
+            requests_session = CachedSession(**kwargs)
             if kwargs.get("expire_after"):
-                requests_session.cache.delete(expired=True)
+                requests_session.remove_expired_responses()
         else:
-            requests_session = Session()  # type:ignore[assignment]
+            requests_session = Session()
 
-        requests_session.headers["User-Agent"] = "pytest-check-links"
+        requests_session.headers['User-Agent'] = 'pytest-check-links'
 
         setattr(config.option, session_attr, requests_session)
 
-    return cast(Session, getattr(config.option, session_attr))
+    return getattr(config.option, session_attr)
 
 
 class CheckLinks(pytest.File):
     """Check the links in a file"""
-
-    def __init__(
-        self,
-        *,
-        requests_session: Session | None = None,
-        check_anchors: bool = False,
-        ignore_links: list[str] | None = None,
-        **kwargs: Any,
-    ) -> None:
-        """Initialize."""
-        super().__init__(**kwargs)
+    def __init__(self, parent=None, fspath=None, requests_session=None, check_anchors=False):
+        super(CheckLinks, self).__init__(fspath, parent)
         self.check_anchors = check_anchors
         self.requests_session = requests_session
-        self.ignore_links = ignore_links or []
-
-    def teardown(self) -> None:
-        """Teardown the handler."""
-        if self.requests_session:
-            self.requests_session.close()
 
-    def _html_from_html(self) -> str:
+    def _html_from_html(self):
         """Return HTML from an HTML file"""
-        with Path(self.path).open(encoding=_ENC) as f:
+        with io.open(str(self.fspath), encoding=_ENC) as f:
             return f.read()
 
-    def _html_from_markdown(self) -> str:
+    def _html_from_markdown(self):
         """Return HTML from a markdown file"""
         # FIXME: use commonmark or a pluggable engine
         from nbconvert.filters import markdown2html
-
-        with Path(self.path).open(encoding=_ENC) as f:
+        with io.open(str(self.fspath), encoding=_ENC) as f:
             markdown = f.read()
         return markdown2html(markdown)
 
-    def _html_from_rst(self) -> str:
+    def _html_from_rst(self):
         """Return HTML from an rst file"""
-        with Path(self.path).open(encoding=_ENC) as f:
+        with io.open(str(self.fspath), encoding=_ENC) as f:
             rst = f.read()
-        return cast(
-            str, publish_parts(rst, source_path=str(self.path), writer_name="html")["html_body"]
-        )
+        return publish_parts(rst, writer_name='html')['html_body']
 
-    def _items_from_notebook(self) -> Generator[LinkItem, None, None]:
+    def _items_from_notebook(self):
         """Yield LinkItems from a notebook"""
         import nbformat
-        from nbconvert.filters.markdown_mistune import IPythonRenderer, MarkdownWithMath
+        from nbconvert.filters import markdown2html
 
-        nb = nbformat.read(str(self.path), as_version=4)  # type:ignore[no-untyped-call]
+        nb = nbformat.read(str(self.fspath), as_version=4)
         for cell_num, cell in enumerate(nb.cells):
-            if cell.cell_type != "markdown":
+            if cell.cell_type != 'markdown':
                 continue
 
-            attachments = cell.get("attachments", {})
-            renderer = IPythonRenderer(escape=False, attachments=attachments)
-            html = MarkdownWithMath(renderer=renderer).render(cell.source)
-            basename = "Cell %i" % cell_num
+            html = markdown2html(cell.source)
+            basename = 'Cell %i' % cell_num
             for item in links_in_html(basename, self, html):
-                if not item.target:
-                    continue
-                ignore = False
-                for pattern in self.ignore_links:
-                    if re.match(pattern, item.target):
-                        ignore = True
-                if not ignore:
-                    yield item
-
-    def collect(self) -> Generator[LinkItem, None, None]:
-        """Collect the test."""
-        path = self.path
-        if path.suffix == ".ipynb":
+                yield item
+
+    def collect(self):
+        path = self.fspath
+        if path.ext == '.ipynb':
             for item in self._items_from_notebook():
                 yield item
             return
 
-        if path.suffix == ".html":
+        if path.ext == '.html':
             html = self._html_from_html()
-        elif path.suffix == ".md":
+        elif path.ext == '.md':
             html = self._html_from_markdown()
-        elif path.suffix == ".rst":
+        elif path.ext == '.rst':
             html = self._html_from_rst()
 
-        for item in links_in_html(str(path), self, html):
-            if not item.target:
-                continue
-            ignore = False
-            for pattern in self.ignore_links:
-                if re.match(pattern, item.target):
-                    ignore = True
-            if not ignore:
-                yield item
+        for item in links_in_html(path, self, html):
+            yield item
 
 
 class BrokenLinkError(Exception):
-    """A broken link error."""
-
-    def __init__(self, url: str, error: Exception | str) -> None:
-        """Initialize the error."""
+    def __init__(self, url, error):
         self.url = url
         self.error = error
 
-    def __repr__(self) -> str:
-        """The repr for the error."""
-        return f"<{self.__class__.__name__} url={self.url}, error={self.error}>"
+    def __repr__(self):
+        return "<%s url=%s, error=%s>" % (
+            self.__class__.__name__, self.url, self.error
+        )
 
 
-def links_in_html(base_name: str, parent: CheckLinks, html: str) -> Generator[LinkItem, None, None]:
+def links_in_html(base_name, parent, html):
     """Yield LinkItems from a markdown cell
 
     Parsed HTML with html5lib, yielding LinkItems for testing.
     """
     parsed = html5lib.parse(html, namespaceHTMLElements=False)
 
-    for element in parsed.iter():
+    for element in parsed.getiterator():
         url = None
         tag = element.tag
-        if tag == "a":
-            attr = "href"
-            url = element.get("href", "")
-            if url.startswith("#") and not parent.check_anchors:
+        if tag == 'a':
+            attr = 'href'
+            url = element.get('href', '')
+            if url.startswith('#') and not parent.check_anchors:
                 # skip internal links
                 continue
 
-        elif tag in {"img", "iframe"}:
-            attr = "src"
+        elif tag in {'img', 'iframe'}:
+            attr = 'src'
         else:
             continue
 
         url = element.get(attr)
-        name = f"{base_name} <{tag} {attr}={url}>"
+        name = '{} <{} {}={}>'.format(base_name, tag, attr, url)
 
         if url:
-            if ":" in url:
-                proto = url.split(":", 1)[0]
-                if proto.lower() not in {"http", "https"}:
+            if ':' in url:
+                proto = url.split(':', 1)[0]
+                if proto.lower() not in {'http', 'https'}:
                     # ignore non-http links (mailto:, data:, etc.)
                     continue
             if hasattr(LinkItem, "from_parent"):
                 yield LinkItem.from_parent(parent, name=name, target=url, parsed=parsed)
             else:
                 yield LinkItem(name=name, parent=parent, target=url, parsed=parsed)
 
 
 class LinkItem(pytest.Item):
-
     """Test item for an HTML link
 
     Args:
 
         name, parent: inherited from pytest.Item
         target (str): The URL or path target for the link
         parsed (xml.etree.ElementTree.Element): The parsed HTML
         description (str, optional): The description to be used in the report header
     """
-
-    parent: CheckLinks
-
-    def __init__(
-        self,
-        name: str | None = None,
-        parent: CheckLinks | None = None,
-        target: str | None = None,
-        parsed: Element | None = None,
-        description: str = "",
-        **kwargs: Any,
-    ):
-        """Initialize the item."""
-        super().__init__(name, parent, **kwargs)
+    def __init__(self, name=None, parent=None, target=None, parsed=None, description=''):
+        super(LinkItem, self).__init__(name, parent)
         self.target = target
         self.parsed = parsed
-        self.description = description or f"{self.path}: {target}"
+        self.description = description or '{}: {}'.format(self.fspath, target)
 
-    def repr_failure(self, excinfo: Any) -> str:  # type:ignore[override]
-        """Repr for a failure."""
+    def repr_failure(self, excinfo):
         exc = excinfo.value
         if isinstance(exc, BrokenLinkError):
-            return f"{exc.url}: {exc.error}"
-        return str(super().repr_failure(excinfo))
+            return '{}: {}'.format(exc.url, exc.error)
+        else:
+            return super(LinkItem, self).repr_failure(excinfo)
 
-    def reportinfo(self) -> tuple[Path, int, str]:
-        """Get the report information."""
-        return self.path, 0, self.description
+    def reportinfo(self):
+        return self.fspath, 0, self.description
 
-    def sleep(self, headers: dict[str, Any] | None) -> bool:
+    def sleep(self, headers):
         """Handle responses or errors with a Retry-After header.
 
         https://www.w3.org/Protocols/rfc2616/rfc2616-sec14.html#sec14.37
         """
         if headers is None:
             return False
 
-        header = headers.get("Retry-After")
+        header = headers.get('Retry-After')
 
         if header is None:
             return False
 
-        if header == "1m0s":
+        if header == '1m0s':
             sleep_time = 60
         else:
             try:
                 sleep_time = int(header)
             except ValueError:
                 sleep_time = 10
 
         time.sleep(sleep_time)
 
         return True
 
-    def handle_anchor(self, parsed: Element, anchor: str) -> None:
-        """Verify an anchor exists in the parsed HTML"""
-        anchors = set(parsed.findall(f'*//a[@name="{anchor}"]'))
-        anchors |= set(parsed.findall(f'*//*[@id="{anchor}"]'))
-        if not self.target:
-            return
+    def handle_anchor(self, parsed, anchor):
+        """Verify an anchor exists in the parsed HTML
+        """
+        anchors = set(parsed.findall('*//a[@name="{}"]'.format(anchor)))
+        anchors |= set(parsed.findall('*//*[@id="{}"]'.format(anchor)))
 
         if not anchors:
             raise BrokenLinkError(self.target, "Missing anchor: %s" % anchor)
 
         if len(anchors) > 1:
             raise BrokenLinkError(
-                self.target, "Ambiguous anchor: %d (found %s)" % (len(anchors), anchor)
+                self.target,
+                "Ambiguous anchor: %d (found %s)" % (
+                    len(anchors), anchor
+                )
             )
 
-    def fetch_with_retries(self, url: str, retries: int = 3) -> Response:
-        """Fetch a URL, optionally retrying after a delay (by header)"""
+    def fetch_with_retries(self, url, retries=3):
+        """Fetch a URL, optionally retrying after a delay (by header)
+        """
 
         url_no_anchor = url.split("#")[0]
         session = self.parent.requests_session
-        if session is None:
-            msg = "No session!"
-            raise RuntimeError(msg)
 
         try:
             response = session.get(url_no_anchor)
         except Exception as err:
-            if hasattr(err, "headers") and retries and self.sleep(err.headers):
+            if hasattr(err, 'headers') and retries and self.sleep(err.headers):
                 self.uncache_url(url_no_anchor)
                 return self.fetch_with_retries(url, retries=retries - 1)
 
-            raise BrokenLinkError(url, "%s" % err) from err
+            raise BrokenLinkError(url, "%s" % err)
 
         if response.status_code >= 400:
-            if retries and self.sleep(response.headers):  # type:ignore[arg-type]
+            if retries and self.sleep(response.headers):
                 self.uncache_url(url_no_anchor)
                 return self.fetch_with_retries(url, retries=retries - 1)
 
-            raise BrokenLinkError(url, "%d: %s" % (response.status_code, response.reason))
+            raise BrokenLinkError(url, "%d: %s" % (
+                response.status_code,
+                response.reason
+            ))
 
         return response
 
-    def uncache_url(self, url: str) -> bool:
-        """Uncache a url."""
-        from requests_cache import BaseCache  # type:ignore[attr-defined]
-
+    def uncache_url(self, url):
         uncached = False
         session = self.parent.requests_session
-        if session is None:
-            msg = "No current session"
-            raise ValueError(msg)
         if hasattr(session, "cache"):
-            request = Request("GET", url, headers=session.headers).prepare()
-            if session.cache is None:
-                msg = "No session cache found"
-                raise ValueError(msg)
-            cache: BaseCache = session.cache
-            key = cache.create_key(request)
-            if cache.contains(key):
+            request = Request('GET', url, headers=session.headers).prepare()
+            key = session.cache.create_key(request)
+            if session.cache.has_key(key):
                 session.cache.delete(key)
                 uncached = True
         return uncached
 
-    def runtest(self) -> None:
-        """Run the test."""
-        url = self.target or ""
+    def runtest(self):
+        url = self.target
 
-        if ":" in url:
+        if ':' in url:
             response = self.fetch_with_retries(url)
-            if self.parent.check_anchors and "#" in url:
-                anchor = url.split("#")[1]
-                if anchor and "html" in response.headers.get("Content-Type", ""):
+            if self.parent.check_anchors and '#' in url:
+                anchor = url.split('#')[1]
+                if anchor and "html" in response.headers.get("Content-Type"):
                     parsed = html5lib.parse(response.content, namespaceHTMLElements=False)
                     return self.handle_anchor(parsed, anchor)
         else:
-            if url.startswith("/"):
+            if url.startswith('/'):
                 raise BrokenLinkError(url, "absolute path link")
             # relative URL
             anchor = None
-            if "?" in url:
-                url = url.split("?")[0]
-            if "#" in url:
-                url, anchor = url.split("#")
+            if '?' in url:
+                url = url.split('?')[0]
+            if '#' in url:
+                url, anchor = url.split('#')
 
             if not url and anchor:
-                if self.parent.check_anchors and self.parsed:
+                if self.parent.check_anchors:
                     self.handle_anchor(self.parsed, anchor)
-                return None
+                return
 
-            url_path = unquote(url).replace("/", os.path.sep)
-            dirpath = self.path.parent
+            url_path = unquote(url).replace('/', os.path.sep)
+            dirpath = self.fspath.dirpath()
             exists = False
             for ext in supported_extensions:
-                rel_path = url_path.replace(".html", ext)
-                target_path = dirpath.joinpath(rel_path)
+                rel_path = url_path.replace('.html', ext)
+                target_path = dirpath.join(rel_path)
                 if target_path.exists():
                     exists = True
                     # only check anchors in html for now
                     if ext == ".html" and anchor and self.parent.check_anchors:
-                        with target_path.open() as fd:
-                            parsed = html5lib.parse(fd, namespaceHTMLElements=False)
+                        with target_path.open() as fpt:
+                            parsed = html5lib.parse(fpt, namespaceHTMLElements=False)
                             return self.handle_anchor(parsed, anchor)
                     break
             if not exists:
-                target_path = dirpath.joinpath(url_path)
+                target_path = dirpath.join(url_path)
                 raise BrokenLinkError(url, "No such file: %s" % target_path)
-            return None
 
 
-def extensions_str(extensions: set[str]) -> str:
-    """Get the extensions as a string."""
+def extensions_str(extensions):
     if not extensions:
-        return ""
-    exts = ['"%s"' % e.lstrip(".") for e in extensions if e]
-    if len(exts) == 1:
-        return exts[0]
-    return ", ".join(exts[:-1]) + " and %s" % exts[-1]
+        return ''
+    extensions = ['"%s"' % e.lstrip('.') for e in extensions if e]
+    if len(extensions) == 1:
+        return extensions[0]
+    return (", ".join(extensions[:-1]) +
+            " and %s" % extensions[-1])
 
 
-def validate_extensions(extensions: set[str]) -> None:
-    """Validate the extensions."""
+def validate_extensions(extensions):
     invalid = set(extensions) - supported_extensions
     if invalid:
-        warnings.warn(
-            "Unsupported extensions for check-links: %s" % extensions_str(invalid), stacklevel=2
-        )
+        warnings.warn("C1", "Unsupported extensions for check-links: %s" %
+            extensions_str(invalid))
```

### Comparing `pytest_check_links-0.9.3/test/test_cache.py` & `pytest_check_links-4.3.3/test/test_cache.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,135 +1,141 @@
 import os
-import shutil
-import sys
 import time
+import shutil
+
 from glob import glob
 
 import pytest
+
 import requests_cache
-from flaky import flaky
 
+from . import examples
+
+
+@pytest.fixture
+def base_args():
+    return ["-v", "--check-links", "--check-links-cache"]
 
-def assert_sqlite(pytester, name=None, tmpdir=None, exists=True):
+
+@pytest.fixture
+def memory_args(base_args):
+    return base_args + ["--check-links-cache-backend", "memory"]
+
+
+def assert_sqlite(testdir, name=None, tmpdir=None, exists=True):
     name = name or ".pytest-check-links-cache.sqlite"
-    tmpdir = str(tmpdir or pytester.path)
+    tmpdir = str(tmpdir or testdir.tmpdir)
     caches = list(glob(os.path.join(tmpdir, name)))
     if exists:
         assert caches
     else:
         assert not caches
 
 
-@flaky
-@pytest.mark.skipif(sys.implementation.name.lower() == "pypy", reason="Does not work on pypy")
-@pytest.mark.parametrize("cache_name", [None, "custom-cache"])
-def test_cache_expiry(pytester, base_args, cache_name, tmpdir):
-    """will the default sqlite3 backend persist and then expire?"""
-    pytester.copy_example("linkcheck.ipynb")
+@pytest.mark.parametrize("cache_name", [
+    None,
+    "custom-cache"
+])
+def test_cache_expiry(testdir, base_args, cache_name, tmpdir):
+    """will the default sqlite3 backend persist and then expire?
+    """
+    testdir.copy_example('linkcheck.ipynb')
 
-    args = [*base_args, "--check-links-cache-expire-after", "2"]
+    args = base_args + ["--check-links-cache-expire-after", "2"]
     if cache_name:
         args += ["--check-links-cache-name", os.path.join(str(tmpdir), cache_name)]
-    expected = {"passed": 3, "failed": 4}
+    expected = dict(passed=3, failed=3)
     t0 = time.time()
-    result = pytester.runpytest_subprocess(*args)
+    result = testdir.runpytest(*args)
     t1 = time.time()
     result.assert_outcomes(**expected)
 
     if cache_name:
-        assert_sqlite(pytester, name=f"{cache_name}.sqlite", tmpdir=tmpdir)
+        assert_sqlite(testdir, name="{}.sqlite".format(cache_name), tmpdir=tmpdir)
     else:
-        assert_sqlite(pytester)
+        assert_sqlite(testdir)
 
     t2 = time.time()
-    result = pytester.runpytest_subprocess(*args)
+    result = testdir.runpytest(*args)
     t3 = time.time()
     result.assert_outcomes(**expected)
 
-    d0 = t1 - t0
-    d1 = t3 - t2
-
-    assert d0 > d1, "cache did not make second run faster"
+    assert t1 - t0 > t3 - t2, "cache did not make second run faster"
 
     time.sleep(2)
 
     t4 = time.time()
-    result = pytester.runpytest_subprocess(*args)
+    result = testdir.runpytest(*args)
     t5 = time.time()
     result.assert_outcomes(**expected)
 
-    d2 = t5 - t4
-    d3 = t3 - t2
-
-    assert d2 > d3, "cache did not expire"
+    assert t5 - t4 > t3 - t2, "cache did not expire"
 
 
-@flaky
-def test_cache_memory(pytester, memory_args):
-    """will the memory backend cache links inside a run?"""
+def test_cache_memory(testdir, memory_args):
+    """will the memory backend cache links inside a run?
+    """
     expected = dict(passed=3, failed=0)
 
-    pytester.copy_example("httpbin.md")
+    testdir.copy_example('httpbin.md')
 
     def run(passed):
         t0 = time.time()
-        result = pytester.runpytest_subprocess(*memory_args)
+        result = testdir.runpytest(*memory_args)
         t1 = time.time()
         result.assert_outcomes(passed=passed, failed=0)
-        assert_sqlite(pytester, exists=False)
+        assert_sqlite(testdir, exists=False)
         return t1 - t0
 
     d0 = run(6)
 
     for i in range(5):
         shutil.copy(
-            os.path.join(str(pytester.path), "httpbin.md"),
-            os.path.join(str(pytester.path), f"httpbin{i}.md"),
+            os.path.join(str(testdir.tmpdir), "httpbin.md"),
+            os.path.join(str(testdir.tmpdir), "httpbin{}.md".format(i))
         )
 
     d1 = run(36)
     # allow a healthy savings margin for network flake
     assert d1 < d0 * 4
 
 
-@flaky
-def test_cache_retry(pytester, memory_args):
-    """will a Retry-After header work with cache?"""
+def test_cache_retry(testdir, memory_args):
+    """will a Retry-After header work with cache?
+    """
 
-    pytester.copy_example("httpbin.md")
+    testdir.copy_example('httpbin.md')
 
-    attempts: list = []
+    attempts = []
 
     _get = requests_cache.CachedSession.get
 
     def mock_get(*args, **kwargs):
         response = _get(*args, **kwargs)
         if len(attempts) < 5:
             response.status_code = 502
-            response.headers["Retry-After"] = "0"
+            response.headers['Retry-After'] = '0'
         attempts.append([args, kwargs])
         return response
 
     requests_cache.CachedSession.get = mock_get
 
-    result = pytester.runpytest_inprocess(*memory_args)
+    result = testdir.runpytest(*memory_args)
 
     try:
         result.assert_outcomes(passed=5, failed=1)
         assert len(attempts) == 10
     finally:
         requests_cache.CachedSession.get = _get
 
 
-@flaky
-def test_cache_backend_opts(pytester, base_args):
-    pytester.copy_example("httpbin.md")
-    args = [
-        *base_args,
-        "--check-links-cache-backend-opt",
-        "fast_save:true",
-        "--check-links-cache-name",
-        "foo",
+def test_cache_backend_opts(testdir, base_args):
+    testdir.copy_example('httpbin.md')
+    args = base_args + [
+        "--check-links-cache-backend-opt", "fast_save:true",
+        "--check-links-cache-name", "foo",
+        "--check-links-cache-backend-opt", "extension:.db",
+        "--check-links-cache-backend-opt", "allowable_codes:[200]"
     ]
-    result = pytester.runpytest_subprocess(*args)
+    result = testdir.runpytest(*args)
     result.assert_outcomes(passed=6, failed=0)
-    assert_sqlite(pytester, name="foo.sqlite")
+    assert_sqlite(testdir, name="foo.db")
```

### Comparing `pytest_check_links-0.9.3/LICENSE` & `pytest_check_links-4.3.3/LICENSE`

 * *Files identical despite different names*

