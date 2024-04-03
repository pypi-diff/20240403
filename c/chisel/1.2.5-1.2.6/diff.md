# Comparing `tmp/chisel-1.2.5.tar.gz` & `tmp/chisel-1.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chisel-1.2.5.tar", last modified: Sat Feb 10 19:06:28 2024, max compression
+gzip compressed data, was "chisel-1.2.6.tar", last modified: Wed Apr  3 20:48:15 2024, max compression
```

## Comparing `chisel-1.2.5.tar` & `chisel-1.2.6.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 craighobbs   (501) staff       (20)        0 2024-02-10 19:06:28.669068 chisel-1.2.5/
--rw-r--r--   0 craighobbs   (501) staff       (20)     1081 2024-02-10 00:56:44.000000 chisel-1.2.5/LICENSE
--rw-r--r--   0 craighobbs   (501) staff       (20)     4540 2024-02-10 19:06:28.669010 chisel-1.2.5/PKG-INFO
--rw-r--r--   0 craighobbs   (501) staff       (20)     3484 2024-02-10 00:56:44.000000 chisel-1.2.5/README.rst
--rw-r--r--   0 craighobbs   (501) staff       (20)       50 2024-02-10 00:56:44.000000 chisel-1.2.5/pyproject.toml
--rw-r--r--   0 craighobbs   (501) staff       (20)     1054 2024-02-10 19:06:28.669297 chisel-1.2.5/setup.cfg
-drwxr-xr-x   0 craighobbs   (501) staff       (20)        0 2024-02-10 19:06:28.666807 chisel-1.2.5/src/
-drwxr-xr-x   0 craighobbs   (501) staff       (20)        0 2024-02-10 19:06:28.667929 chisel-1.2.5/src/chisel/
--rw-r--r--   0 craighobbs   (501) staff       (20)      502 2024-02-10 00:56:44.000000 chisel-1.2.5/src/chisel/__init__.py
--rw-r--r--   0 craighobbs   (501) staff       (20)    13926 2024-02-10 00:56:44.000000 chisel-1.2.5/src/chisel/action.py
--rw-r--r--   0 craighobbs   (501) staff       (20)    22354 2024-02-10 19:03:50.000000 chisel-1.2.5/src/chisel/app.py
--rw-r--r--   0 craighobbs   (501) staff       (20)     9936 2024-02-10 00:56:44.000000 chisel-1.2.5/src/chisel/doc.py
--rw-r--r--   0 craighobbs   (501) staff       (20)     8147 2024-02-10 00:56:44.000000 chisel-1.2.5/src/chisel/request.py
-drwxr-xr-x   0 craighobbs   (501) staff       (20)        0 2024-02-10 19:06:28.668643 chisel-1.2.5/src/chisel.egg-info/
--rw-r--r--   0 craighobbs   (501) staff       (20)     4540 2024-02-10 19:06:28.000000 chisel-1.2.5/src/chisel.egg-info/PKG-INFO
--rw-r--r--   0 craighobbs   (501) staff       (20)      314 2024-02-10 19:06:28.000000 chisel-1.2.5/src/chisel.egg-info/SOURCES.txt
--rw-r--r--   0 craighobbs   (501) staff       (20)        1 2024-02-10 19:06:28.000000 chisel-1.2.5/src/chisel.egg-info/dependency_links.txt
--rw-r--r--   0 craighobbs   (501) staff       (20)       23 2024-02-10 19:06:28.000000 chisel-1.2.5/src/chisel.egg-info/requires.txt
--rw-r--r--   0 craighobbs   (501) staff       (20)        7 2024-02-10 19:06:28.000000 chisel-1.2.5/src/chisel.egg-info/top_level.txt
+drwxr-xr-x   0 craighobbs   (501) staff       (20)        0 2024-04-03 20:48:15.674208 chisel-1.2.6/
+-rw-r--r--   0 craighobbs   (501) staff       (20)     1081 2024-04-02 16:27:20.000000 chisel-1.2.6/LICENSE
+-rw-r--r--   0 craighobbs   (501) staff       (20)     4155 2024-04-03 20:48:15.674147 chisel-1.2.6/PKG-INFO
+-rw-r--r--   0 craighobbs   (501) staff       (20)     3096 2024-04-03 20:25:13.000000 chisel-1.2.6/README.md
+-rw-r--r--   0 craighobbs   (501) staff       (20)       50 2024-04-02 16:27:20.000000 chisel-1.2.6/pyproject.toml
+-rw-r--r--   0 craighobbs   (501) staff       (20)     1056 2024-04-03 20:48:15.674508 chisel-1.2.6/setup.cfg
+drwxr-xr-x   0 craighobbs   (501) staff       (20)        0 2024-04-03 20:48:15.671950 chisel-1.2.6/src/
+drwxr-xr-x   0 craighobbs   (501) staff       (20)        0 2024-04-03 20:48:15.673120 chisel-1.2.6/src/chisel/
+-rw-r--r--   0 craighobbs   (501) staff       (20)      502 2024-04-02 16:27:20.000000 chisel-1.2.6/src/chisel/__init__.py
+-rw-r--r--   0 craighobbs   (501) staff       (20)    13926 2024-04-02 16:27:20.000000 chisel-1.2.6/src/chisel/action.py
+-rw-r--r--   0 craighobbs   (501) staff       (20)    22354 2024-04-02 16:27:20.000000 chisel-1.2.6/src/chisel/app.py
+-rw-r--r--   0 craighobbs   (501) staff       (20)     9936 2024-04-02 16:27:20.000000 chisel-1.2.6/src/chisel/doc.py
+-rw-r--r--   0 craighobbs   (501) staff       (20)     8147 2024-04-02 16:27:20.000000 chisel-1.2.6/src/chisel/request.py
+drwxr-xr-x   0 craighobbs   (501) staff       (20)        0 2024-04-03 20:48:15.673912 chisel-1.2.6/src/chisel.egg-info/
+-rw-r--r--   0 craighobbs   (501) staff       (20)     4155 2024-04-03 20:48:15.000000 chisel-1.2.6/src/chisel.egg-info/PKG-INFO
+-rw-r--r--   0 craighobbs   (501) staff       (20)      313 2024-04-03 20:48:15.000000 chisel-1.2.6/src/chisel.egg-info/SOURCES.txt
+-rw-r--r--   0 craighobbs   (501) staff       (20)        1 2024-04-03 20:48:15.000000 chisel-1.2.6/src/chisel.egg-info/dependency_links.txt
+-rw-r--r--   0 craighobbs   (501) staff       (20)       23 2024-04-03 20:48:15.000000 chisel-1.2.6/src/chisel.egg-info/requires.txt
+-rw-r--r--   0 craighobbs   (501) staff       (20)        7 2024-04-03 20:48:15.000000 chisel-1.2.6/src/chisel.egg-info/top_level.txt
```

### Comparing `chisel-1.2.5/LICENSE` & `chisel-1.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `chisel-1.2.5/PKG-INFO` & `chisel-1.2.6/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chisel
-Version: 1.2.5
+Version: 1.2.6
 Summary: Lightweight WSGI application framework, schema-validated JSON APIs, and API documentation
 Home-page: https://github.com/craigahobbs/chisel
 Author: Craig A. Hobbs
 Author-email: craigahobbs@gmail.com
 License: MIT
 Keywords: api,json,framework,schema,wsgi
 Classifier: Development Status :: 5 - Production/Stable
@@ -15,112 +15,99 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Internet :: WWW/HTTP :: WSGI
 Classifier: Topic :: Internet :: WWW/HTTP :: WSGI :: Application
 Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
-Description-Content-Type: text/x-rst
+Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: schema-markdown>=1.2.0
 
-chisel
-======
+# chisel
 
-.. |badge-status| image:: https://img.shields.io/pypi/status/chisel
-   :alt: PyPI - Status
-   :target: https://pypi.python.org/pypi/chisel/
-
-.. |badge-version| image:: https://img.shields.io/pypi/v/chisel
-   :alt: PyPI
-   :target: https://pypi.python.org/pypi/chisel/
-
-.. |badge-license| image:: https://img.shields.io/github/license/craigahobbs/chisel
-   :alt: GitHub
-   :target: https://github.com/craigahobbs/chisel/blob/main/LICENSE
-
-.. |badge-python| image:: https://img.shields.io/pypi/pyversions/chisel
-   :alt: PyPI - Python Version
-   :target: https://www.python.org/downloads/
-
-|badge-status| |badge-version| |badge-license| |badge-python|
+[![PyPI - Status](https://img.shields.io/pypi/status/chisel)](https://pypi.org/project/chisel/)
+[![PyPI](https://img.shields.io/pypi/v/chisel)](https://pypi.org/project/chisel/)
+[![GitHub](https://img.shields.io/github/license/craigahobbs/chisel)](https://github.com/craigahobbs/chisel/blob/main/LICENSE)
+[![PyPI - Python Version](https://img.shields.io/pypi/pyversions/chisel)](https://pypi.org/project/chisel/)
 
 Chisel is a light-weight Python WSGI application framework built for creating well-documented,
 schema-validated JSON web APIs.
 
 
-Links
------
+## Links
 
-- `API Documentation <https://craigahobbs.github.io/chisel/>`__
-- `Source code <https://github.com/craigahobbs/chisel>`__
+- [API Documentation](https://craigahobbs.github.io/chisel/)
+- [Source code](https://github.com/craigahobbs/chisel)
 
 
-JSON APIs
----------
+## JSON APIs
 
-Chisel provides the `action <https://craigahobbs.github.io/chisel/action.html#chisel.action>`__
+Chisel provides the [action](https://craigahobbs.github.io/chisel/action.html#chisel.action)
 decorator for easily implementing schema-validated JSON APIs.
 
->>> @chisel.action(spec='''
-... # Sum a list of numbers
-... action sum_numbers
-...     urls
-...        GET
-...
-...     query
-...         # The list of numbers
-...         float[len > 0] numbers
-...
-...     output
-...         # The sum of the numbers
-...         float sum
-... ''')
-... def sum_numbers(ctx, req):
-...     return {'sum': sum(req['numbers'])}
-...
->>> application = chisel.Application()
->>> application.add_request(sum_numbers)
->>> application.request('GET', '/sum_numbers', query_string='numbers.0=1&numbers.1=2&numbers.2=4')
+~~~ python
+@chisel.action(spec='''
+# Sum a list of numbers
+action sum_numbers
+    urls
+       GET
+
+    query
+        # The list of numbers
+        float[len > 0] numbers
+
+    output
+        # The sum of the numbers
+        float sum
+''')
+def sum_numbers(ctx, req):
+    return {'sum': sum(req['numbers'])}
+
+application = chisel.Application()
+application.add_request(sum_numbers)
+application.request('GET', '/sum_numbers', query_string='numbers.0=1&numbers.1=2&numbers.2=4')
+
 ('200 OK', [('Content-Type', 'application/json')], b'{"sum":7.0}')
+~~~
 
 Each action defines an ``action`` definition using
-`Schema Markdown <https://craigahobbs.github.io/schema-markdown-js/language/>`__.
+[Schema Markdown](https://craigahobbs.github.io/schema-markdown-js/language/).
 The action callback is passed two arguments, a request
-`Context <https://craigahobbs.github.io/chisel/app.html#chisel.Context>`__
+[Context](https://craigahobbs.github.io/chisel/app.html#chisel.Context)
 and the schema-validated request input dictionary. The input request dictionary is created by
 combining the request's URL path parameters, query string parameters, and input JSON content
 parameters.
 
 If there is a schema validation error the appropriate error code is automatically returned.
 
->>> status, _, content_bytes = application.request('GET', '/sum_numbers')
->>> status
-'400 Bad Request'
+~~~ python
+status, _, content_bytes = application.request('GET', '/sum_numbers')
 
->>> content_bytes
+'400 Bad Request'
 b'{"error":"InvalidInput","message":"Required member \'numbers\' missing (query string)"}'
+~~~
 
 
-API Documentation
------------------
+## API Documentation
 
 You can add API documentation to your application by adding the Chisel documentation application
 requests from
-`create_doc_requests <https://craigahobbs.github.io/chisel/request.html#chisel.create_doc_requests>`__.
+[create_doc_requests](https://craigahobbs.github.io/chisel/request.html#chisel.create_doc_requests).
 
->>> application = chisel.Application()
->>> application.add_requests(chisel.create_doc_requests())
+~~~ python
+application = chisel.Application()
+application.add_requests(chisel.create_doc_requests())
+~~~
 
 By default the documentation application is hosted at "/doc/". An example of of Chisel's documentation output is
-available `here <https://craigahobbs.github.io/chisel/example/#var.vName='chisel_doc_request'>`__.
-
+available [here](https://craigahobbs.github.io/chisel/example/#var.vName='chisel_doc_request').
 
-Development
------------
 
-This package is developed using `python-build <https://github.com/craigahobbs/python-build#readme>`__.
-It was started using `python-template <https://github.com/craigahobbs/python-template#readme>`__ as follows:
+## Development
 
-.. code-block:: sh
+This package is developed using [python-build](https://github.com/craigahobbs/python-build#readme).
+It was started using [python-template](https://github.com/craigahobbs/python-template#readme) as follows:
 
-    template-specialize python-template/template/ chisel/ -k package chisel -k name 'Craig A. Hobbs' -k email 'craigahobbs@gmail.com' -k github 'craigahobbs' -k nomain 1
+~~~ sh
+template-specialize python-template/template/ chisel/ -k package chisel -k name 'Craig A. Hobbs' -k email 'craigahobbs@gmail.com' -k github 'craigahobbs' -k nomain 1
+~~~
```

### Comparing `chisel-1.2.5/setup.cfg` & `chisel-1.2.6/setup.cfg`

 * *Files 14% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 [metadata]
 name = chisel
-version = 1.2.5
+version = 1.2.6
 url = https://github.com/craigahobbs/chisel
 author = Craig A. Hobbs
 author_email = craigahobbs@gmail.com
 license = MIT
 description = Lightweight WSGI application framework, schema-validated JSON APIs, and API documentation
-long_description = file:README.rst
-long_description_content_type = text/x-rst
+long_description = file:README.md
+long_description_content_type = text/markdown
 keywords = api, json, framework, schema, wsgi
 classifiers = 
 	Development Status :: 5 - Production/Stable
 	Intended Audience :: Developers
 	License :: OSI Approved :: MIT License
 	Operating System :: OS Independent
 	Programming Language :: Python :: 3.8
```

### Comparing `chisel-1.2.5/src/chisel/action.py` & `chisel-1.2.6/src/chisel/action.py`

 * *Files identical despite different names*

### Comparing `chisel-1.2.5/src/chisel/app.py` & `chisel-1.2.6/src/chisel/app.py`

 * *Files identical despite different names*

### Comparing `chisel-1.2.5/src/chisel/doc.py` & `chisel-1.2.6/src/chisel/doc.py`

 * *Files identical despite different names*

### Comparing `chisel-1.2.5/src/chisel/request.py` & `chisel-1.2.6/src/chisel/request.py`

 * *Files identical despite different names*

### Comparing `chisel-1.2.5/src/chisel.egg-info/PKG-INFO` & `chisel-1.2.6/src/chisel.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chisel
-Version: 1.2.5
+Version: 1.2.6
 Summary: Lightweight WSGI application framework, schema-validated JSON APIs, and API documentation
 Home-page: https://github.com/craigahobbs/chisel
 Author: Craig A. Hobbs
 Author-email: craigahobbs@gmail.com
 License: MIT
 Keywords: api,json,framework,schema,wsgi
 Classifier: Development Status :: 5 - Production/Stable
@@ -15,112 +15,99 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Internet :: WWW/HTTP :: WSGI
 Classifier: Topic :: Internet :: WWW/HTTP :: WSGI :: Application
 Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
-Description-Content-Type: text/x-rst
+Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: schema-markdown>=1.2.0
 
-chisel
-======
+# chisel
 
-.. |badge-status| image:: https://img.shields.io/pypi/status/chisel
-   :alt: PyPI - Status
-   :target: https://pypi.python.org/pypi/chisel/
-
-.. |badge-version| image:: https://img.shields.io/pypi/v/chisel
-   :alt: PyPI
-   :target: https://pypi.python.org/pypi/chisel/
-
-.. |badge-license| image:: https://img.shields.io/github/license/craigahobbs/chisel
-   :alt: GitHub
-   :target: https://github.com/craigahobbs/chisel/blob/main/LICENSE
-
-.. |badge-python| image:: https://img.shields.io/pypi/pyversions/chisel
-   :alt: PyPI - Python Version
-   :target: https://www.python.org/downloads/
-
-|badge-status| |badge-version| |badge-license| |badge-python|
+[![PyPI - Status](https://img.shields.io/pypi/status/chisel)](https://pypi.org/project/chisel/)
+[![PyPI](https://img.shields.io/pypi/v/chisel)](https://pypi.org/project/chisel/)
+[![GitHub](https://img.shields.io/github/license/craigahobbs/chisel)](https://github.com/craigahobbs/chisel/blob/main/LICENSE)
+[![PyPI - Python Version](https://img.shields.io/pypi/pyversions/chisel)](https://pypi.org/project/chisel/)
 
 Chisel is a light-weight Python WSGI application framework built for creating well-documented,
 schema-validated JSON web APIs.
 
 
-Links
------
+## Links
 
-- `API Documentation <https://craigahobbs.github.io/chisel/>`__
-- `Source code <https://github.com/craigahobbs/chisel>`__
+- [API Documentation](https://craigahobbs.github.io/chisel/)
+- [Source code](https://github.com/craigahobbs/chisel)
 
 
-JSON APIs
----------
+## JSON APIs
 
-Chisel provides the `action <https://craigahobbs.github.io/chisel/action.html#chisel.action>`__
+Chisel provides the [action](https://craigahobbs.github.io/chisel/action.html#chisel.action)
 decorator for easily implementing schema-validated JSON APIs.
 
->>> @chisel.action(spec='''
-... # Sum a list of numbers
-... action sum_numbers
-...     urls
-...        GET
-...
-...     query
-...         # The list of numbers
-...         float[len > 0] numbers
-...
-...     output
-...         # The sum of the numbers
-...         float sum
-... ''')
-... def sum_numbers(ctx, req):
-...     return {'sum': sum(req['numbers'])}
-...
->>> application = chisel.Application()
->>> application.add_request(sum_numbers)
->>> application.request('GET', '/sum_numbers', query_string='numbers.0=1&numbers.1=2&numbers.2=4')
+~~~ python
+@chisel.action(spec='''
+# Sum a list of numbers
+action sum_numbers
+    urls
+       GET
+
+    query
+        # The list of numbers
+        float[len > 0] numbers
+
+    output
+        # The sum of the numbers
+        float sum
+''')
+def sum_numbers(ctx, req):
+    return {'sum': sum(req['numbers'])}
+
+application = chisel.Application()
+application.add_request(sum_numbers)
+application.request('GET', '/sum_numbers', query_string='numbers.0=1&numbers.1=2&numbers.2=4')
+
 ('200 OK', [('Content-Type', 'application/json')], b'{"sum":7.0}')
+~~~
 
 Each action defines an ``action`` definition using
-`Schema Markdown <https://craigahobbs.github.io/schema-markdown-js/language/>`__.
+[Schema Markdown](https://craigahobbs.github.io/schema-markdown-js/language/).
 The action callback is passed two arguments, a request
-`Context <https://craigahobbs.github.io/chisel/app.html#chisel.Context>`__
+[Context](https://craigahobbs.github.io/chisel/app.html#chisel.Context)
 and the schema-validated request input dictionary. The input request dictionary is created by
 combining the request's URL path parameters, query string parameters, and input JSON content
 parameters.
 
 If there is a schema validation error the appropriate error code is automatically returned.
 
->>> status, _, content_bytes = application.request('GET', '/sum_numbers')
->>> status
-'400 Bad Request'
+~~~ python
+status, _, content_bytes = application.request('GET', '/sum_numbers')
 
->>> content_bytes
+'400 Bad Request'
 b'{"error":"InvalidInput","message":"Required member \'numbers\' missing (query string)"}'
+~~~
 
 
-API Documentation
------------------
+## API Documentation
 
 You can add API documentation to your application by adding the Chisel documentation application
 requests from
-`create_doc_requests <https://craigahobbs.github.io/chisel/request.html#chisel.create_doc_requests>`__.
+[create_doc_requests](https://craigahobbs.github.io/chisel/request.html#chisel.create_doc_requests).
 
->>> application = chisel.Application()
->>> application.add_requests(chisel.create_doc_requests())
+~~~ python
+application = chisel.Application()
+application.add_requests(chisel.create_doc_requests())
+~~~
 
 By default the documentation application is hosted at "/doc/". An example of of Chisel's documentation output is
-available `here <https://craigahobbs.github.io/chisel/example/#var.vName='chisel_doc_request'>`__.
-
+available [here](https://craigahobbs.github.io/chisel/example/#var.vName='chisel_doc_request').
 
-Development
------------
 
-This package is developed using `python-build <https://github.com/craigahobbs/python-build#readme>`__.
-It was started using `python-template <https://github.com/craigahobbs/python-template#readme>`__ as follows:
+## Development
 
-.. code-block:: sh
+This package is developed using [python-build](https://github.com/craigahobbs/python-build#readme).
+It was started using [python-template](https://github.com/craigahobbs/python-template#readme) as follows:
 
-    template-specialize python-template/template/ chisel/ -k package chisel -k name 'Craig A. Hobbs' -k email 'craigahobbs@gmail.com' -k github 'craigahobbs' -k nomain 1
+~~~ sh
+template-specialize python-template/template/ chisel/ -k package chisel -k name 'Craig A. Hobbs' -k email 'craigahobbs@gmail.com' -k github 'craigahobbs' -k nomain 1
+~~~
```

