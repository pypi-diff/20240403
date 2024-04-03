# Comparing `tmp/pmxbot.webhooks-1.4.0.tar.gz` & `tmp/pmxbot.webhooks-1.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/tmp/tmpb6ktbgn3/tmpbkwatc0b/pmxbot.webhooks-1.4.0.tar", last modified: Sat Nov 14 22:13:24 2020, max compression
+gzip compressed data, was "pmxbot.webhooks-1.5.0.tar", last modified: Wed Apr  3 00:50:39 2024, max compression
```

## Comparing `pmxbot.webhooks-1.4.0.tar` & `pmxbot.webhooks-1.5.0.tar`

### file list

```diff
@@ -1,39 +1,40 @@
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-11-14 22:13:24.969806 pmxbot.webhooks-1.4.0/
--rw-r--r--   0 runner    (1001) docker     (116)       50 2020-11-14 22:13:03.000000 pmxbot.webhooks-1.4.0/.coveragerc
--rw-r--r--   0 runner    (1001) docker     (116)      246 2020-11-14 22:13:03.000000 pmxbot.webhooks-1.4.0/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-11-14 22:13:24.965806 pmxbot.webhooks-1.4.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-11-14 22:13:24.965806 pmxbot.webhooks-1.4.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (116)     1040 2020-11-14 22:13:03.000000 pmxbot.webhooks-1.4.0/.github/workflows/main.yml
--rw-r--r--   0 runner    (1001) docker     (116)      175 2020-11-14 22:13:03.000000 pmxbot.webhooks-1.4.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (116)       79 2020-11-14 22:13:03.000000 pmxbot.webhooks-1.4.0/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (116)      506 2020-11-14 22:13:03.000000 pmxbot.webhooks-1.4.0/CHANGES.rst
--rw-r--r--   0 runner    (1001) docker     (116)     1050 2020-11-14 22:13:03.000000 pmxbot.webhooks-1.4.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (116)     2277 2020-11-14 22:13:24.969806 pmxbot.webhooks-1.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)     1407 2020-11-14 22:13:03.000000 pmxbot.webhooks-1.4.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-11-14 22:13:24.969806 pmxbot.webhooks-1.4.0/docs/
--rw-r--r--   0 runner    (1001) docker     (116)      756 2020-11-14 22:13:03.000000 pmxbot.webhooks-1.4.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (116)       81 2020-11-14 22:13:03.000000 pmxbot.webhooks-1.4.0/docs/history.rst
--rw-r--r--   0 runner    (1001) docker     (116)      309 2020-11-14 22:13:03.000000 pmxbot.webhooks-1.4.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (116)       37 2020-11-14 22:13:03.000000 pmxbot.webhooks-1.4.0/mypy.ini
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-11-14 22:13:24.969806 pmxbot.webhooks-1.4.0/pmxbot/
--rw-r--r--   0 runner    (1001) docker     (116)       56 2020-11-14 22:13:03.000000 pmxbot.webhooks-1.4.0/pmxbot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     2990 2020-11-14 22:13:03.000000 pmxbot.webhooks-1.4.0/pmxbot/bookmarklet-min.js
--rw-r--r--   0 runner    (1001) docker     (116)     4773 2020-11-14 22:13:03.000000 pmxbot.webhooks-1.4.0/pmxbot/bookmarklet.js
--rw-r--r--   0 runner    (1001) docker     (116)    11688 2020-11-14 22:13:03.000000 pmxbot.webhooks-1.4.0/pmxbot/webhooks.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-11-14 22:13:24.969806 pmxbot.webhooks-1.4.0/pmxbot.webhooks.egg-info/
--rw-r--r--   0 runner    (1001) docker     (116)     2277 2020-11-14 22:13:24.000000 pmxbot.webhooks-1.4.0/pmxbot.webhooks.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)      644 2020-11-14 22:13:24.000000 pmxbot.webhooks-1.4.0/pmxbot.webhooks.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2020-11-14 22:13:24.000000 pmxbot.webhooks-1.4.0/pmxbot.webhooks.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (116)       46 2020-11-14 22:13:24.000000 pmxbot.webhooks-1.4.0/pmxbot.webhooks.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (116)        7 2020-11-14 22:13:24.000000 pmxbot.webhooks-1.4.0/pmxbot.webhooks.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (116)      300 2020-11-14 22:13:24.000000 pmxbot.webhooks-1.4.0/pmxbot.webhooks.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (116)       13 2020-11-14 22:13:24.000000 pmxbot.webhooks-1.4.0/pmxbot.webhooks.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (116)      457 2020-11-14 22:13:03.000000 pmxbot.webhooks-1.4.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (116)      333 2020-11-14 22:13:03.000000 pmxbot.webhooks-1.4.0/pytest.ini
--rw-r--r--   0 runner    (1001) docker     (116)     1123 2020-11-14 22:13:24.969806 pmxbot.webhooks-1.4.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (116)       92 2020-11-14 22:13:03.000000 pmxbot.webhooks-1.4.0/setup.py
--rw-r--r--   0 runner    (1001) docker     (116)     8511 2020-11-14 22:13:03.000000 pmxbot.webhooks-1.4.0/skeleton.md
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-11-14 22:13:24.969806 pmxbot.webhooks-1.4.0/tests/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2020-11-14 22:13:03.000000 pmxbot.webhooks-1.4.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     5416 2020-11-14 22:13:03.000000 pmxbot.webhooks-1.4.0/tests/test_http.py
--rw-r--r--   0 runner    (1001) docker     (116)      699 2020-11-14 22:13:03.000000 pmxbot.webhooks-1.4.0/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 00:50:39.579632 pmxbot.webhooks-1.5.0/
+-rw-r--r--   0 runner    (1001) docker     (127)      200 2024-04-03 00:50:21.000000 pmxbot.webhooks-1.5.0/.coveragerc
+-rw-r--r--   0 runner    (1001) docker     (127)      246 2024-04-03 00:50:21.000000 pmxbot.webhooks-1.5.0/.editorconfig
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 00:50:39.571632 pmxbot.webhooks-1.5.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)      148 2024-04-03 00:50:21.000000 pmxbot.webhooks-1.5.0/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 00:50:39.571632 pmxbot.webhooks-1.5.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     2855 2024-04-03 00:50:21.000000 pmxbot.webhooks-1.5.0/.github/workflows/main.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      116 2024-04-03 00:50:21.000000 pmxbot.webhooks-1.5.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      335 2024-04-03 00:50:21.000000 pmxbot.webhooks-1.5.0/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1023 2024-04-03 00:50:21.000000 pmxbot.webhooks-1.5.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      666 2024-04-03 00:50:21.000000 pmxbot.webhooks-1.5.0/NEWS.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2793 2024-04-03 00:50:39.579632 pmxbot.webhooks-1.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1504 2024-04-03 00:50:21.000000 pmxbot.webhooks-1.5.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 00:50:39.575632 pmxbot.webhooks-1.5.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     1188 2024-04-03 00:50:21.000000 pmxbot.webhooks-1.5.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-03 00:50:21.000000 pmxbot.webhooks-1.5.0/docs/history.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      339 2024-04-03 00:50:21.000000 pmxbot.webhooks-1.5.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2024-04-03 00:50:21.000000 pmxbot.webhooks-1.5.0/mypy.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 00:50:39.575632 pmxbot.webhooks-1.5.0/pmxbot/
+-rw-r--r--   0 runner    (1001) docker     (127)     2990 2024-04-03 00:50:21.000000 pmxbot.webhooks-1.5.0/pmxbot/bookmarklet-min.js
+-rw-r--r--   0 runner    (1001) docker     (127)     4773 2024-04-03 00:50:21.000000 pmxbot.webhooks-1.5.0/pmxbot/bookmarklet.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 00:50:39.575632 pmxbot.webhooks-1.5.0/pmxbot/compat/
+-rw-r--r--   0 runner    (1001) docker     (127)      155 2024-04-03 00:50:21.000000 pmxbot.webhooks-1.5.0/pmxbot/compat/py311.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11741 2024-04-03 00:50:21.000000 pmxbot.webhooks-1.5.0/pmxbot/webhooks.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 00:50:39.575632 pmxbot.webhooks-1.5.0/pmxbot.webhooks.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2793 2024-04-03 00:50:39.000000 pmxbot.webhooks-1.5.0/pmxbot.webhooks.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      631 2024-04-03 00:50:39.000000 pmxbot.webhooks-1.5.0/pmxbot.webhooks.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 00:50:39.000000 pmxbot.webhooks-1.5.0/pmxbot.webhooks.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-03 00:50:39.000000 pmxbot.webhooks-1.5.0/pmxbot.webhooks.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      282 2024-04-03 00:50:39.000000 pmxbot.webhooks-1.5.0/pmxbot.webhooks.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-03 00:50:39.000000 pmxbot.webhooks-1.5.0/pmxbot.webhooks.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      139 2024-04-03 00:50:21.000000 pmxbot.webhooks-1.5.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      584 2024-04-03 00:50:21.000000 pmxbot.webhooks-1.5.0/pytest.ini
+-rw-r--r--   0 runner    (1001) docker     (127)      419 2024-04-03 00:50:21.000000 pmxbot.webhooks-1.5.0/ruff.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      977 2024-04-03 00:50:39.579632 pmxbot.webhooks-1.5.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 00:50:39.575632 pmxbot.webhooks-1.5.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 00:50:21.000000 pmxbot.webhooks-1.5.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5347 2024-04-03 00:50:21.000000 pmxbot.webhooks-1.5.0/tests/test_http.py
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-03 00:50:21.000000 pmxbot.webhooks-1.5.0/towncrier.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1364 2024-04-03 00:50:21.000000 pmxbot.webhooks-1.5.0/tox.ini
```

### Comparing `pmxbot.webhooks-1.4.0/LICENSE` & `pmxbot.webhooks-1.5.0/LICENSE`

 * *Files 16% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-Copyright Jason R. Coombs
-
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to
 deal in the Software without restriction, including without limitation the
 rights to use, copy, modify, merge, publish, distribute, sublicense, and/or
 sell copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `pmxbot.webhooks-1.4.0/README.rst` & `pmxbot.webhooks-1.5.0/README.rst`

 * *Files 18% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 .. image:: https://img.shields.io/pypi/v/pmxbot.webhooks.svg
-   :target: `PyPI link`_
+   :target: https://pypi.org/project/pmxbot.webhooks
 
 .. image:: https://img.shields.io/pypi/pyversions/pmxbot.webhooks.svg
-   :target: `PyPI link`_
 
-.. _PyPI link: https://pypi.org/project/pmxbot.webhooks
+.. image:: https://github.com/jaraco/pmxbot.webhooks/actions/workflows/main.yml/badge.svg
+   :target: https://github.com/jaraco/pmxbot.webhooks/actions?query=workflow%3A%22tests%22
+   :alt: tests
+
+.. image:: https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/charliermarsh/ruff/main/assets/badge/v2.json
+    :target: https://github.com/astral-sh/ruff
+    :alt: Ruff
 
-.. image:: https://github.com/jaraco/skeleton/workflows/Automated%20Tests/badge.svg
-   :target: https://github.com/jaraco/skeleton/actions?query=workflow%3A%22Automated+Tests%22
-   :alt: Automated Tests
+.. .. image:: https://readthedocs.org/projects/PROJECT_RTD/badge/?version=latest
+..    :target: https://PROJECT_RTD.readthedocs.io/en/latest/?badge=latest
 
-.. image:: https://img.shields.io/badge/code%20style-black-000000.svg
-   :target: https://github.com/psf/black
-   :alt: Code style: Black
-
-.. .. image:: https://readthedocs.org/projects/pmxbotwebhooks/badge/?version=latest
-..    :target: https://pmxbotwebhooks.readthedocs.io/en/latest/?badge=latest
+.. image:: https://img.shields.io/badge/skeleton-2024-informational
+   :target: https://blog.jaraco.com/skeleton
 
 Webhooks for `pmxbot <https://pypi.org/project/pmxbot>`_. Read the source
 for details.
 
 Bookmarklet
 ===========
```

### Comparing `pmxbot.webhooks-1.4.0/docs/conf.py` & `pmxbot.webhooks-1.5.0/docs/conf.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,26 +1,43 @@
-#!/usr/bin/env python3
-# -*- coding: utf-8 -*-
-
-extensions = ['sphinx.ext.autodoc', 'jaraco.packaging.sphinx', 'rst.linker']
+extensions = [
+    'sphinx.ext.autodoc',
+    'jaraco.packaging.sphinx',
+]
 
 master_doc = "index"
+html_theme = "furo"
 
+# Link dates and other references in the changelog
+extensions += ['rst.linker']
 link_files = {
-    '../CHANGES.rst': dict(
+    '../NEWS.rst': dict(
         using=dict(GH='https://github.com'),
         replace=[
             dict(
                 pattern=r'(Issue #|\B#)(?P<issue>\d+)',
                 url='{package_url}/issues/{issue}',
             ),
             dict(
                 pattern=r'(?m:^((?P<scm_version>v?\d+(\.\d+){1,2}))\n[-=]+\n)',
                 with_scm='{text}\n{rev[timestamp]:%d %b %Y}\n',
             ),
             dict(
                 pattern=r'PEP[- ](?P<pep_number>\d+)',
-                url='https://www.python.org/dev/peps/pep-{pep_number:0>4}/',
+                url='https://peps.python.org/pep-{pep_number:0>4}/',
             ),
         ],
     )
 }
+
+# Be strict about any broken references
+nitpicky = True
+
+# Include Python intersphinx mapping to prevent failures
+# jaraco/skeleton#51
+extensions += ['sphinx.ext.intersphinx']
+intersphinx_mapping = {
+    'python': ('https://docs.python.org/3', None),
+    'pmxbot': ('https://pmxbot.readthedocs.io/en/latest/', None),
+}
+
+# Preserve authored syntax for defaults
+autodoc_preserve_defaults = True
```

### Comparing `pmxbot.webhooks-1.4.0/pmxbot/bookmarklet-min.js` & `pmxbot.webhooks-1.5.0/pmxbot/bookmarklet-min.js`

 * *Files identical despite different names*

### Comparing `pmxbot.webhooks-1.4.0/pmxbot/bookmarklet.js` & `pmxbot.webhooks-1.5.0/pmxbot/bookmarklet.js`

 * *Files identical despite different names*

### Comparing `pmxbot.webhooks-1.4.0/pmxbot/webhooks.py` & `pmxbot.webhooks-1.5.0/pmxbot/webhooks.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,16 @@
 import logging
 import codecs
 import textwrap
 import urllib.parse
 from itertools import chain
 from typing import List, Union
 
-import pkg_resources
+from .compat.py311 import resources
+
 from more_itertools import always_iterable
 import cherrypy
 import pmxbot.core
 import cherrypy_cors
 
 
 log = logging.getLogger(__name__)
@@ -132,15 +133,14 @@
         )
         proj = event['ProjectName']
         for channel in self.get_channels(proj):
             Server.send_to(channel, message.format(base=base, **event))
 
 
 class Velociraptor(ChannelSelector):
-
     SWARM_DEPLOY_DONE_RE = re.compile(r'Swarm (.+) finished')
 
     @cherrypy.expose
     @cherrypy.tools.allow(methods=['POST'])
     @cherrypy.tools.json_in()
     def default(self):
         event = cherrypy.request.json
@@ -307,16 +307,20 @@
         >>> 'pmxbot.example.com' in bm
         True
         >>> '%20' in bm
         True
         >>> 'href="javascript:' in bm
         True
         """
-        script = pkg_resources.resource_string(__name__, 'bookmarklet-min.js')
-        script = script.decode('utf-8').strip()
+        script = (
+            resources.files()
+            .joinpath('bookmarklet-min.js')
+            .read_text(encoding='utf-8')
+            .strip()
+        )
         hostname = cherrypy.request.headers['Host']
         script = script.replace('ircbot.example.com', hostname)
         script_href = 'javascript:' + urllib.parse.quote(script)
         tmpl = textwrap.dedent(
             """
             <html>
             <head></head>
```

### Comparing `pmxbot.webhooks-1.4.0/setup.cfg` & `pmxbot.webhooks-1.5.0/setup.cfg`

 * *Files 16% similar despite different names*

```diff
@@ -1,49 +1,46 @@
 [metadata]
-license_file = LICENSE
 name = pmxbot.webhooks
 author = Jason R. Coombs
 author_email = jaraco@jaraco.com
 description = An HTTP-based webhook service for pmxbot
 long_description = file:README.rst
 url = https://github.com/jaraco/pmxbot.webhooks
 classifiers = 
 	Development Status :: 5 - Production/Stable
 	Intended Audience :: Developers
 	License :: OSI Approved :: MIT License
 	Programming Language :: Python :: 3
 	Programming Language :: Python :: 3 :: Only
 
 [options]
-packages = find:
-namespace_packages = pmxbot
 include_package_data = true
-python_requires = >=3.6
+python_requires = >=3.8
 install_requires = 
 	twilio>=6
 	cherrypy_cors
 	more_itertools
-setup_requires = setuptools_scm[toml] >= 3.4.1
+	importlib_resources; python_version < "3.12"
 
 [options.extras_require]
 testing = 
-	pytest >= 3.5, !=3.7.3
-	pytest-checkdocs >= 1.2.3
-	pytest-flake8
-	pytest-black >= 0.3.7; python_implementation != "PyPy"
+	pytest >= 6, != 8.1.1
+	pytest-checkdocs >= 2.4
 	pytest-cov
-	pytest-mypy; python_implementation != "PyPy"
-	jaraco.test >= 3.2.0
+	pytest-mypy
+	pytest-enabler >= 2.2
+	pytest-ruff >= 0.2.1
 	
 	pmxbot
-	cherrypy[testing]
 docs = 
-	sphinx
-	jaraco.packaging >= 3.2
+	sphinx >= 3.5
+	jaraco.packaging >= 9.3
 	rst.linker >= 1.9
+	furo
+	sphinx-lint
 
 [options.entry_points]
 pmxbot_handlers = 
 	webhooks = pmxbot.webhooks
 
 [egg_info]
 tag_build =
```

### Comparing `pmxbot.webhooks-1.4.0/tests/test_http.py` & `pmxbot.webhooks-1.5.0/tests/test_http.py`

 * *Files 2% similar despite different names*

```diff
@@ -47,15 +47,14 @@
     def server(self):
         return cherrypy.tree.apps[''].root
 
     def _get(self, **kwargs):
         return self.getPage("/velociraptor", **kwargs)
 
     def _post_json(self, data):
-
         body = json.dumps(data)
         kwargs = {
             'method': 'POST',
             'headers': [
                 ('Content-Type', 'application/json'),
                 ('Content-Length', str(len(body))),
             ],
@@ -92,39 +91,35 @@
         payload = {
             'tags': ['route'],
             'title': 'My Swarm',
         }
         self._post_json(payload)
         self.assertStatus('200 OK')
         self.assertBody('OK')
-        mock_send_to.assert_has_calls(
-            [
-                mock.call('chan1', 'VR: Routed My Swarm'),
-                mock.call('chan2', 'VR: Routed My Swarm'),
-            ]
-        )
+        mock_send_to.assert_has_calls([
+            mock.call('chan1', 'VR: Routed My Swarm'),
+            mock.call('chan2', 'VR: Routed My Swarm'),
+        ])
 
     @mock.patch('pmxbot.webhooks.Server.send_to')
     @mock.patch('pmxbot.webhooks.ChannelSelector.get_channels')
     def test_event_swarm_deploy_done(self, mock_get_channels, mock_send_to):
         mock_get_channels.return_value = ['chan1', 'chan2']
         payload = {
             'tags': ['swarm', 'deploy', 'done'],
             'title': 'Swarm MySwarm finished',
             'message': 'Swarm MySwarm finished',
         }
         self._post_json(payload)
         self.assertStatus('200 OK')
         self.assertBody('OK')
-        mock_send_to.assert_has_calls(
-            [
-                mock.call('chan1', 'VR: Swarm MySwarm finished'),
-                mock.call('chan2', 'VR: Swarm MySwarm finished'),
-            ]
-        )
+        mock_send_to.assert_has_calls([
+            mock.call('chan1', 'VR: Swarm MySwarm finished'),
+            mock.call('chan2', 'VR: Swarm MySwarm finished'),
+        ])
 
     @mock.patch('pmxbot.webhooks.Server.send_to')
     @mock.patch('pmxbot.webhooks.ChannelSelector.get_channels')
     def test_event_scheduled_failed(self, mock_get_channels, mock_send_to):
         mock_get_channels.return_value = ['chan1']
         message = textwrap.dedent(
             """
```

