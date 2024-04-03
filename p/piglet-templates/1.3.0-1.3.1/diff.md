# Comparing `tmp/piglet-templates-1.3.0.tar.gz` & `tmp/piglet-templates-1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "piglet-templates-1.3.0.tar", last modified: Fri Jun 10 12:16:15 2022, max compression
+gzip compressed data, was "piglet-templates-1.3.1.tar", last modified: Wed Apr  3 18:42:50 2024, max compression
```

## Comparing `piglet-templates-1.3.0.tar` & `piglet-templates-1.3.1.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 oliver    (1001) wheel        (0)        0 2022-06-10 12:16:15.327068 piglet-templates-1.3.0/
--rw-r--r--   0 oliver    (1001) wheel        (0)    10175 2022-06-10 12:14:42.000000 piglet-templates-1.3.0/LICENSE.txt
--rw-r--r--   0 oliver    (1001) wheel        (0)     2364 2022-06-10 12:16:15.327168 piglet-templates-1.3.0/PKG-INFO
--rw-r--r--   0 oliver    (1001) wheel        (0)     1475 2022-06-10 12:14:42.000000 piglet-templates-1.3.0/README.rst
-drwxr-xr-x   0 oliver    (1001) wheel        (0)        0 2022-06-10 12:16:15.324639 piglet-templates-1.3.0/piglet/
--rw-r--r--   0 oliver    (1001) wheel        (0)      931 2022-06-10 12:16:00.000000 piglet-templates-1.3.0/piglet/__init__.py
--rw-r--r--   0 oliver    (1001) wheel        (0)     7954 2022-06-10 12:14:42.000000 piglet-templates-1.3.0/piglet/astutil.py
--rw-r--r--   0 oliver    (1001) wheel        (0)    38786 2022-06-10 12:14:42.000000 piglet-templates-1.3.0/piglet/compile.py
--rw-r--r--   0 oliver    (1001) wheel        (0)     8808 2022-06-10 12:14:42.000000 piglet-templates-1.3.0/piglet/compilett.py
--rw-r--r--   0 oliver    (1001) wheel        (0)    30279 2022-06-10 12:14:42.000000 piglet-templates-1.3.0/piglet/compilexml.py
--rw-r--r--   0 oliver    (1001) wheel        (0)     1746 2022-06-10 12:14:42.000000 piglet-templates-1.3.0/piglet/exceptions.py
--rw-r--r--   0 oliver    (1001) wheel        (0)     3198 2022-06-10 12:14:42.000000 piglet-templates-1.3.0/piglet/i18n.py
--rw-r--r--   0 oliver    (1001) wheel        (0)    10706 2022-06-10 12:14:42.000000 piglet-templates-1.3.0/piglet/intermediate.py
--rw-r--r--   0 oliver    (1001) wheel        (0)     1132 2022-06-10 12:14:42.000000 piglet-templates-1.3.0/piglet/interpolate.py
--rw-r--r--   0 oliver    (1001) wheel        (0)    10679 2022-06-10 12:14:42.000000 piglet-templates-1.3.0/piglet/loader.py
--rw-r--r--   0 oliver    (1001) wheel        (0)     4966 2022-06-10 12:14:42.000000 piglet-templates-1.3.0/piglet/parse.py
-drwxr-xr-x   0 oliver    (1001) wheel        (0)        0 2022-06-10 12:16:15.325670 piglet-templates-1.3.0/piglet/parsers/
--rw-r--r--   0 oliver    (1001) wheel        (0)      339 2022-06-10 12:14:42.000000 piglet-templates-1.3.0/piglet/parsers/__init__.py
--rw-r--r--   0 oliver    (1001) wheel        (0)     5960 2022-06-10 12:14:42.000000 piglet-templates-1.3.0/piglet/parsers/html.py
--rw-r--r--   0 oliver    (1001) wheel        (0)     2913 2022-06-10 12:14:42.000000 piglet-templates-1.3.0/piglet/parsers/interpolation.py
--rw-r--r--   0 oliver    (1001) wheel        (0)     1482 2022-06-10 12:14:42.000000 piglet-templates-1.3.0/piglet/parsers/semicolonseparated.py
--rw-r--r--   0 oliver    (1001) wheel        (0)     3260 2022-06-10 12:14:42.000000 piglet-templates-1.3.0/piglet/parsers/text.py
--rw-r--r--   0 oliver    (1001) wheel        (0)     1102 2022-06-10 12:14:42.000000 piglet-templates-1.3.0/piglet/position.py
--rw-r--r--   0 oliver    (1001) wheel        (0)     7375 2022-06-10 12:14:42.000000 piglet-templates-1.3.0/piglet/runtime.py
--rw-r--r--   0 oliver    (1001) wheel        (0)     4960 2022-06-10 12:14:42.000000 piglet-templates-1.3.0/piglet/template.py
--rw-r--r--   0 oliver    (1001) wheel        (0)     4927 2022-06-10 12:14:42.000000 piglet-templates-1.3.0/piglet/test_compilett.py
--rw-r--r--   0 oliver    (1001) wheel        (0)     9977 2022-06-10 12:14:42.000000 piglet-templates-1.3.0/piglet/test_compilexml.py
--rw-r--r--   0 oliver    (1001) wheel        (0)     9000 2022-06-10 12:14:42.000000 piglet-templates-1.3.0/piglet/test_i18n.py
--rw-r--r--   0 oliver    (1001) wheel        (0)     2304 2022-06-10 12:14:42.000000 piglet-templates-1.3.0/piglet/test_interpolate.py
--rw-r--r--   0 oliver    (1001) wheel        (0)     9059 2022-06-10 12:14:42.000000 piglet-templates-1.3.0/piglet/test_loader.py
--rw-r--r--   0 oliver    (1001) wheel        (0)     5163 2022-06-10 12:14:42.000000 piglet-templates-1.3.0/piglet/test_parse.py
--rw-r--r--   0 oliver    (1001) wheel        (0)    25670 2022-06-10 12:14:42.000000 piglet-templates-1.3.0/piglet/test_piglet.py
--rw-r--r--   0 oliver    (1001) wheel        (0)      868 2022-06-10 12:14:42.000000 piglet-templates-1.3.0/piglet/test_position.py
-drwxr-xr-x   0 oliver    (1001) wheel        (0)        0 2022-06-10 12:16:15.326890 piglet-templates-1.3.0/piglet_templates.egg-info/
--rw-r--r--   0 oliver    (1001) wheel        (0)     2364 2022-06-10 12:16:15.000000 piglet-templates-1.3.0/piglet_templates.egg-info/PKG-INFO
--rw-r--r--   0 oliver    (1001) wheel        (0)      878 2022-06-10 12:16:15.000000 piglet-templates-1.3.0/piglet_templates.egg-info/SOURCES.txt
--rw-r--r--   0 oliver    (1001) wheel        (0)        1 2022-06-10 12:16:15.000000 piglet-templates-1.3.0/piglet_templates.egg-info/dependency_links.txt
--rw-r--r--   0 oliver    (1001) wheel        (0)      127 2022-06-10 12:16:15.000000 piglet-templates-1.3.0/piglet_templates.egg-info/entry_points.txt
--rw-r--r--   0 oliver    (1001) wheel        (0)       38 2022-06-10 12:16:15.000000 piglet-templates-1.3.0/piglet_templates.egg-info/requires.txt
--rw-r--r--   0 oliver    (1001) wheel        (0)        7 2022-06-10 12:16:15.000000 piglet-templates-1.3.0/piglet_templates.egg-info/top_level.txt
--rw-r--r--   0 oliver    (1001) wheel        (0)     1151 2022-06-10 12:16:15.327861 piglet-templates-1.3.0/setup.cfg
--rw-r--r--   0 oliver    (1001) wheel        (0)       33 2022-06-10 12:14:42.000000 piglet-templates-1.3.0/setup.py
+drwxr-xr-x   0 oliver    (1001) wheel        (0)        0 2024-04-03 18:42:50.747472 piglet-templates-1.3.1/
+-rw-r--r--   0 oliver    (1001) wheel        (0)    10175 2024-04-03 18:41:39.000000 piglet-templates-1.3.1/LICENSE.txt
+-rw-r--r--   0 oliver    (1001) wheel        (0)     2344 2024-04-03 18:42:50.747596 piglet-templates-1.3.1/PKG-INFO
+-rw-r--r--   0 oliver    (1001) wheel        (0)     1475 2024-04-03 18:41:39.000000 piglet-templates-1.3.1/README.rst
+drwxr-xr-x   0 oliver    (1001) wheel        (0)        0 2024-04-03 18:42:50.745903 piglet-templates-1.3.1/piglet/
+-rw-r--r--   0 oliver    (1001) wheel        (0)      931 2024-04-03 18:42:49.000000 piglet-templates-1.3.1/piglet/__init__.py
+-rw-r--r--   0 oliver    (1001) wheel        (0)     7954 2024-04-03 18:41:39.000000 piglet-templates-1.3.1/piglet/astutil.py
+-rw-r--r--   0 oliver    (1001) wheel        (0)    38786 2024-04-03 18:41:39.000000 piglet-templates-1.3.1/piglet/compile.py
+-rw-r--r--   0 oliver    (1001) wheel        (0)     8808 2024-04-03 18:41:39.000000 piglet-templates-1.3.1/piglet/compilett.py
+-rw-r--r--   0 oliver    (1001) wheel        (0)    30279 2024-04-03 18:41:39.000000 piglet-templates-1.3.1/piglet/compilexml.py
+-rw-r--r--   0 oliver    (1001) wheel        (0)     1746 2024-04-03 18:41:39.000000 piglet-templates-1.3.1/piglet/exceptions.py
+-rw-r--r--   0 oliver    (1001) wheel        (0)     3198 2024-04-03 18:41:39.000000 piglet-templates-1.3.1/piglet/i18n.py
+-rw-r--r--   0 oliver    (1001) wheel        (0)    10706 2024-04-03 18:41:39.000000 piglet-templates-1.3.1/piglet/intermediate.py
+-rw-r--r--   0 oliver    (1001) wheel        (0)     1132 2024-04-03 18:41:39.000000 piglet-templates-1.3.1/piglet/interpolate.py
+-rw-r--r--   0 oliver    (1001) wheel        (0)    10679 2024-04-03 18:41:39.000000 piglet-templates-1.3.1/piglet/loader.py
+-rw-r--r--   0 oliver    (1001) wheel        (0)     4966 2024-04-03 18:41:39.000000 piglet-templates-1.3.1/piglet/parse.py
+drwxr-xr-x   0 oliver    (1001) wheel        (0)        0 2024-04-03 18:42:50.746572 piglet-templates-1.3.1/piglet/parsers/
+-rw-r--r--   0 oliver    (1001) wheel        (0)      399 2024-04-03 18:41:39.000000 piglet-templates-1.3.1/piglet/parsers/__init__.py
+-rw-r--r--   0 oliver    (1001) wheel        (0)     5923 2024-04-03 18:41:39.000000 piglet-templates-1.3.1/piglet/parsers/html.py
+-rw-r--r--   0 oliver    (1001) wheel        (0)     2876 2024-04-03 18:41:39.000000 piglet-templates-1.3.1/piglet/parsers/interpolation.py
+-rw-r--r--   0 oliver    (1001) wheel        (0)     1482 2024-04-03 18:41:39.000000 piglet-templates-1.3.1/piglet/parsers/semicolonseparated.py
+-rw-r--r--   0 oliver    (1001) wheel        (0)     3223 2024-04-03 18:41:39.000000 piglet-templates-1.3.1/piglet/parsers/text.py
+-rw-r--r--   0 oliver    (1001) wheel        (0)     1102 2024-04-03 18:41:39.000000 piglet-templates-1.3.1/piglet/position.py
+-rw-r--r--   0 oliver    (1001) wheel        (0)     7375 2024-04-03 18:41:39.000000 piglet-templates-1.3.1/piglet/runtime.py
+-rw-r--r--   0 oliver    (1001) wheel        (0)     4960 2024-04-03 18:41:39.000000 piglet-templates-1.3.1/piglet/template.py
+-rw-r--r--   0 oliver    (1001) wheel        (0)     4927 2024-04-03 18:41:39.000000 piglet-templates-1.3.1/piglet/test_compilett.py
+-rw-r--r--   0 oliver    (1001) wheel        (0)     9977 2024-04-03 18:41:39.000000 piglet-templates-1.3.1/piglet/test_compilexml.py
+-rw-r--r--   0 oliver    (1001) wheel        (0)     9000 2024-04-03 18:41:39.000000 piglet-templates-1.3.1/piglet/test_i18n.py
+-rw-r--r--   0 oliver    (1001) wheel        (0)     2304 2024-04-03 18:41:39.000000 piglet-templates-1.3.1/piglet/test_interpolate.py
+-rw-r--r--   0 oliver    (1001) wheel        (0)     9059 2024-04-03 18:41:39.000000 piglet-templates-1.3.1/piglet/test_loader.py
+-rw-r--r--   0 oliver    (1001) wheel        (0)     5163 2024-04-03 18:41:39.000000 piglet-templates-1.3.1/piglet/test_parse.py
+-rw-r--r--   0 oliver    (1001) wheel        (0)    25670 2024-04-03 18:41:39.000000 piglet-templates-1.3.1/piglet/test_piglet.py
+-rw-r--r--   0 oliver    (1001) wheel        (0)      868 2024-04-03 18:41:39.000000 piglet-templates-1.3.1/piglet/test_position.py
+drwxr-xr-x   0 oliver    (1001) wheel        (0)        0 2024-04-03 18:42:50.747359 piglet-templates-1.3.1/piglet_templates.egg-info/
+-rw-r--r--   0 oliver    (1001) wheel        (0)     2344 2024-04-03 18:42:50.000000 piglet-templates-1.3.1/piglet_templates.egg-info/PKG-INFO
+-rw-r--r--   0 oliver    (1001) wheel        (0)      878 2024-04-03 18:42:50.000000 piglet-templates-1.3.1/piglet_templates.egg-info/SOURCES.txt
+-rw-r--r--   0 oliver    (1001) wheel        (0)        1 2024-04-03 18:42:50.000000 piglet-templates-1.3.1/piglet_templates.egg-info/dependency_links.txt
+-rw-r--r--   0 oliver    (1001) wheel        (0)      126 2024-04-03 18:42:50.000000 piglet-templates-1.3.1/piglet_templates.egg-info/entry_points.txt
+-rw-r--r--   0 oliver    (1001) wheel        (0)       38 2024-04-03 18:42:50.000000 piglet-templates-1.3.1/piglet_templates.egg-info/requires.txt
+-rw-r--r--   0 oliver    (1001) wheel        (0)        7 2024-04-03 18:42:50.000000 piglet-templates-1.3.1/piglet_templates.egg-info/top_level.txt
+-rw-r--r--   0 oliver    (1001) wheel        (0)     1151 2024-04-03 18:42:50.748296 piglet-templates-1.3.1/setup.cfg
+-rw-r--r--   0 oliver    (1001) wheel        (0)       33 2024-04-03 18:41:39.000000 piglet-templates-1.3.1/setup.py
```

### Comparing `piglet-templates-1.3.0/LICENSE.txt` & `piglet-templates-1.3.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `piglet-templates-1.3.0/PKG-INFO` & `piglet-templates-1.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: piglet-templates
-Version: 1.3.0
+Version: 1.3.1
 Summary: Fast, robust HTML templating engine
 Home-page: https://ollycope.com/software/piglet/latest/
 Author: Oliver Cope
 Author-email: oliver@redgecko.org
 License: Apache
 Keywords: jinja2 jinja genshi kajiki mako kid html templating template engine chameleon
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: Implementation :: PyPy
@@ -72,9 +71,7 @@
 -------
 
 Piglet-templates is licensed under the Apache license version 2.0.
 
 Piglet-templates is developed by
 `Olly Cope <https://ollycope.com/>`_
 and was created for `skot.be <https://skot.be/>`_
-
-
```

### Comparing `piglet-templates-1.3.0/README.rst` & `piglet-templates-1.3.1/README.rst`

 * *Files identical despite different names*

### Comparing `piglet-templates-1.3.0/piglet/__init__.py` & `piglet-templates-1.3.1/piglet/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-__version__ = "1.3.0"
+__version__ = "1.3.1"
 __all__ = [
     "__version__",
     "TemplateLoader",
     "HTMLTemplate",
     "TextTemplate",
     "PigletError",
     "PigletParseError",
```

### Comparing `piglet-templates-1.3.0/piglet/astutil.py` & `piglet-templates-1.3.1/piglet/astutil.py`

 * *Files identical despite different names*

### Comparing `piglet-templates-1.3.0/piglet/compile.py` & `piglet-templates-1.3.1/piglet/compile.py`

 * *Files identical despite different names*

### Comparing `piglet-templates-1.3.0/piglet/compilett.py` & `piglet-templates-1.3.1/piglet/compilett.py`

 * *Files identical despite different names*

### Comparing `piglet-templates-1.3.0/piglet/compilexml.py` & `piglet-templates-1.3.1/piglet/compilexml.py`

 * *Files identical despite different names*

### Comparing `piglet-templates-1.3.0/piglet/exceptions.py` & `piglet-templates-1.3.1/piglet/exceptions.py`

 * *Files identical despite different names*

### Comparing `piglet-templates-1.3.0/piglet/i18n.py` & `piglet-templates-1.3.1/piglet/i18n.py`

 * *Files identical despite different names*

### Comparing `piglet-templates-1.3.0/piglet/intermediate.py` & `piglet-templates-1.3.1/piglet/intermediate.py`

 * *Files identical despite different names*

### Comparing `piglet-templates-1.3.0/piglet/interpolate.py` & `piglet-templates-1.3.1/piglet/interpolate.py`

 * *Files identical despite different names*

### Comparing `piglet-templates-1.3.0/piglet/loader.py` & `piglet-templates-1.3.1/piglet/loader.py`

 * *Files identical despite different names*

### Comparing `piglet-templates-1.3.0/piglet/parse.py` & `piglet-templates-1.3.1/piglet/parse.py`

 * *Files identical despite different names*

### Comparing `piglet-templates-1.3.0/piglet/parsers/html.py` & `piglet-templates-1.3.1/piglet/parsers/html.py`

 * *Files 0% similar despite different names*

```diff
@@ -207,8 +207,7 @@
     | cdata
     | declaration
     | processing_instruction
 )
 html_template_parser = html()
 html_template_parser.leaveWhitespace()
 html_template_parser.parseWithTabs()
-html_template_parser.enablePackrat()
```

### Comparing `piglet-templates-1.3.0/piglet/parsers/interpolation.py` & `piglet-templates-1.3.1/piglet/parsers/interpolation.py`

 * *Files 3% similar despite different names*

```diff
@@ -92,8 +92,7 @@
     | escaped_dollar
     | lone_dollar
 ).setParseAction(lambda ts: list(group_strings(ts)))
 
 interpolation_parser = text_with_interpolations()
 interpolation_parser.leaveWhitespace()
 interpolation_parser.parseWithTabs()
-interpolation_parser.enablePackrat()
```

### Comparing `piglet-templates-1.3.0/piglet/parsers/semicolonseparated.py` & `piglet-templates-1.3.1/piglet/parsers/semicolonseparated.py`

 * *Files identical despite different names*

### Comparing `piglet-templates-1.3.0/piglet/parsers/text.py` & `piglet-templates-1.3.1/piglet/parsers/text.py`

 * *Files 2% similar despite different names*

```diff
@@ -108,8 +108,7 @@
 )
 
 text_template = ZeroOrMore(text | directive)
 
 text_template_parser = text_template()
 text_template_parser.leaveWhitespace()
 text_template_parser.parseWithTabs()
-text_template_parser.enablePackrat()
```

### Comparing `piglet-templates-1.3.0/piglet/position.py` & `piglet-templates-1.3.1/piglet/position.py`

 * *Files identical despite different names*

### Comparing `piglet-templates-1.3.0/piglet/runtime.py` & `piglet-templates-1.3.1/piglet/runtime.py`

 * *Files identical despite different names*

### Comparing `piglet-templates-1.3.0/piglet/template.py` & `piglet-templates-1.3.1/piglet/template.py`

 * *Files identical despite different names*

### Comparing `piglet-templates-1.3.0/piglet/test_compilett.py` & `piglet-templates-1.3.1/piglet/test_compilett.py`

 * *Files identical despite different names*

### Comparing `piglet-templates-1.3.0/piglet/test_compilexml.py` & `piglet-templates-1.3.1/piglet/test_compilexml.py`

 * *Files identical despite different names*

### Comparing `piglet-templates-1.3.0/piglet/test_i18n.py` & `piglet-templates-1.3.1/piglet/test_i18n.py`

 * *Files identical despite different names*

### Comparing `piglet-templates-1.3.0/piglet/test_interpolate.py` & `piglet-templates-1.3.1/piglet/test_interpolate.py`

 * *Files identical despite different names*

### Comparing `piglet-templates-1.3.0/piglet/test_loader.py` & `piglet-templates-1.3.1/piglet/test_loader.py`

 * *Files identical despite different names*

### Comparing `piglet-templates-1.3.0/piglet/test_parse.py` & `piglet-templates-1.3.1/piglet/test_parse.py`

 * *Files identical despite different names*

### Comparing `piglet-templates-1.3.0/piglet/test_piglet.py` & `piglet-templates-1.3.1/piglet/test_piglet.py`

 * *Files identical despite different names*

### Comparing `piglet-templates-1.3.0/piglet/test_position.py` & `piglet-templates-1.3.1/piglet/test_position.py`

 * *Files identical despite different names*

### Comparing `piglet-templates-1.3.0/piglet_templates.egg-info/PKG-INFO` & `piglet-templates-1.3.1/piglet_templates.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: piglet-templates
-Version: 1.3.0
+Version: 1.3.1
 Summary: Fast, robust HTML templating engine
 Home-page: https://ollycope.com/software/piglet/latest/
 Author: Oliver Cope
 Author-email: oliver@redgecko.org
 License: Apache
 Keywords: jinja2 jinja genshi kajiki mako kid html templating template engine chameleon
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: Implementation :: PyPy
@@ -72,9 +71,7 @@
 -------
 
 Piglet-templates is licensed under the Apache license version 2.0.
 
 Piglet-templates is developed by
 `Olly Cope <https://ollycope.com/>`_
 and was created for `skot.be <https://skot.be/>`_
-
-
```

### Comparing `piglet-templates-1.3.0/piglet_templates.egg-info/SOURCES.txt` & `piglet-templates-1.3.1/piglet_templates.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `piglet-templates-1.3.0/setup.cfg` & `piglet-templates-1.3.1/setup.cfg`

 * *Files identical despite different names*

