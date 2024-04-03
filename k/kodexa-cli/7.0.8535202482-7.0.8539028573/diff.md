# Comparing `tmp/kodexa_cli-7.0.8535202482.tar.gz` & `tmp/kodexa_cli-7.0.8539028573.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kodexa_cli-7.0.8535202482.tar", max compression
+gzip compressed data, was "kodexa_cli-7.0.8539028573.tar", max compression
```

## Comparing `kodexa_cli-7.0.8535202482.tar` & `kodexa_cli-7.0.8539028573.tar`

### file list

```diff
@@ -1,43 +1,43 @@
--rw-r--r--   0        0        0    11357 2024-04-03 08:04:51.604847 kodexa_cli-7.0.8535202482/LICENSE
--rw-r--r--   0        0        0     2157 2024-04-03 08:04:51.604847 kodexa_cli-7.0.8535202482/README.md
--rw-r--r--   0        0        0       64 2024-04-03 08:04:51.608847 kodexa_cli-7.0.8535202482/kodexa_cli/__init__.py
--rw-r--r--   0        0        0      349 2024-04-03 08:04:51.608847 kodexa_cli-7.0.8535202482/kodexa_cli/charts/extension-pack/.helmignore
--rw-r--r--   0        0        0      146 2024-04-03 08:04:51.608847 kodexa_cli-7.0.8535202482/kodexa_cli/charts/extension-pack/Chart.yaml
--rw-r--r--   0        0        0        0 2024-04-03 08:04:51.608847 kodexa_cli-7.0.8535202482/kodexa_cli/charts/extension-pack/resources/.gitkeep
--rw-r--r--   0        0        0       38 2024-04-03 08:04:51.608847 kodexa_cli-7.0.8535202482/kodexa_cli/charts/extension-pack/templates/NOTES.txt
--rw-r--r--   0        0        0     1852 2024-04-03 08:04:51.608847 kodexa_cli-7.0.8535202482/kodexa_cli/charts/extension-pack/templates/_helpers.tpl
--rw-r--r--   0        0        0      324 2024-04-03 08:04:51.608847 kodexa_cli-7.0.8535202482/kodexa_cli/charts/extension-pack/templates/configmap.yaml
--rw-r--r--   0        0        0      250 2024-04-03 08:04:51.608847 kodexa_cli-7.0.8535202482/kodexa_cli/charts/extension-pack/values.yaml
--rw-r--r--   0        0        0      402 2024-04-03 08:04:51.608847 kodexa_cli-7.0.8535202482/kodexa_cli/charts/resource-container/Dockerfile
--rw-r--r--   0        0        0      174 2024-04-03 08:04:51.608847 kodexa_cli-7.0.8535202482/kodexa_cli/charts/resource-container/health-check.conf
--rw-r--r--   0        0        0        0 2024-04-03 08:04:51.608847 kodexa_cli-7.0.8535202482/kodexa_cli/charts/resource-container/index.html
--rw-r--r--   0        0        0      349 2024-04-03 08:04:51.608847 kodexa_cli-7.0.8535202482/kodexa_cli/charts/resource-pack/.helmignore
--rw-r--r--   0        0        0      140 2024-04-03 08:04:51.608847 kodexa_cli-7.0.8535202482/kodexa_cli/charts/resource-pack/Chart.yaml
--rw-r--r--   0        0        0     1528 2024-04-03 08:04:51.608847 kodexa_cli-7.0.8535202482/kodexa_cli/charts/resource-pack/templates/_helpers.tpl
--rw-r--r--   0        0        0     1791 2024-04-03 08:04:51.608847 kodexa_cli-7.0.8535202482/kodexa_cli/charts/resource-pack/templates/deployment.yaml
--rw-r--r--   0        0        0      410 2024-04-03 08:04:51.608847 kodexa_cli-7.0.8535202482/kodexa_cli/charts/resource-pack/templates/service.yaml
--rw-r--r--   0        0        0      330 2024-04-03 08:04:51.608847 kodexa_cli-7.0.8535202482/kodexa_cli/charts/resource-pack/values.yaml
--rw-r--r--   0        0        0    48743 2024-04-03 08:04:51.608847 kodexa_cli-7.0.8535202482/kodexa_cli/cli.py
--rw-r--r--   0        0        0     7641 2024-04-03 08:04:51.608847 kodexa_cli-7.0.8535202482/kodexa_cli/documentation.py
--rw-r--r--   0        0        0      134 2024-04-03 08:04:51.608847 kodexa_cli-7.0.8535202482/kodexa_cli/templates/action.jinja2
--rw-r--r--   0        0        0     1356 2024-04-03 08:04:51.608847 kodexa_cli-7.0.8535202482/kodexa_cli/templates/assistant.jinja2
--rw-r--r--   0        0        0     1021 2024-04-03 08:04:51.608847 kodexa_cli-7.0.8535202482/kodexa_cli/templates/content-taxon.jinja2
--rw-r--r--   0        0        0      328 2024-04-03 08:04:51.608847 kodexa_cli-7.0.8535202482/kodexa_cli/templates/data-store.jinja2
--rw-r--r--   0        0        0      707 2024-04-03 08:04:51.608847 kodexa_cli-7.0.8535202482/kodexa_cli/templates/document-store.jinja2
--rw-r--r--   0        0        0       30 2024-04-03 08:04:51.608847 kodexa_cli-7.0.8535202482/kodexa_cli/templates/extension-pack.jinja2
--rw-r--r--   0        0        0      818 2024-04-03 08:04:51.608847 kodexa_cli-7.0.8535202482/kodexa_cli/templates/header.jinja2
--rw-r--r--   0        0        0      343 2024-04-03 08:04:51.608847 kodexa_cli-7.0.8535202482/kodexa_cli/templates/index.jinja2
--rw-r--r--   0        0        0       30 2024-04-03 08:04:51.608847 kodexa_cli-7.0.8535202482/kodexa_cli/templates/model-runtime.jinja2
--rw-r--r--   0        0        0     2999 2024-04-03 08:04:51.608847 kodexa_cli-7.0.8535202482/kodexa_cli/templates/model.jinja2
--rw-r--r--   0        0        0     1137 2024-04-03 08:04:51.612847 kodexa_cli-7.0.8535202482/kodexa_cli/templates/options.jinja2
--rw-r--r--   0        0        0        0 2024-04-03 08:04:51.612847 kodexa_cli-7.0.8535202482/kodexa_cli/templates/overview.jinja2
--rw-r--r--   0        0        0      722 2024-04-03 08:04:51.612847 kodexa_cli-7.0.8535202482/kodexa_cli/templates/processing-taxon.jinja2
--rw-r--r--   0        0        0       30 2024-04-03 08:04:51.612847 kodexa_cli-7.0.8535202482/kodexa_cli/templates/project-template.jinja2
--rw-r--r--   0        0        0       30 2024-04-03 08:04:51.612847 kodexa_cli-7.0.8535202482/kodexa_cli/templates/store.jinja2
--rw-r--r--   0        0        0      492 2024-04-03 08:04:51.612847 kodexa_cli-7.0.8535202482/kodexa_cli/templates/taxon.jinja2
--rw-r--r--   0        0        0      273 2024-04-03 08:04:51.612847 kodexa_cli-7.0.8535202482/kodexa_cli/templates/taxonomy-labels.jinja2
--rw-r--r--   0        0        0      534 2024-04-03 08:04:51.612847 kodexa_cli-7.0.8535202482/kodexa_cli/templates/taxonomy-structure.jinja2
--rw-r--r--   0        0        0      269 2024-04-03 08:04:51.612847 kodexa_cli-7.0.8535202482/kodexa_cli/templates/taxonomy.jinja2
--rw-r--r--   0        0        0      808 2024-04-03 08:05:08.481160 kodexa_cli-7.0.8535202482/pyproject.toml
--rw-r--r--   0        0        0     3404 1970-01-01 00:00:00.000000 kodexa_cli-7.0.8535202482/setup.py
--rw-r--r--   0        0        0     2767 1970-01-01 00:00:00.000000 kodexa_cli-7.0.8535202482/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-04-03 12:52:35.954015 kodexa_cli-7.0.8539028573/LICENSE
+-rw-r--r--   0        0        0     2157 2024-04-03 12:52:35.954015 kodexa_cli-7.0.8539028573/README.md
+-rw-r--r--   0        0        0       64 2024-04-03 12:52:35.958015 kodexa_cli-7.0.8539028573/kodexa_cli/__init__.py
+-rw-r--r--   0        0        0      349 2024-04-03 12:52:35.958015 kodexa_cli-7.0.8539028573/kodexa_cli/charts/extension-pack/.helmignore
+-rw-r--r--   0        0        0      146 2024-04-03 12:52:35.958015 kodexa_cli-7.0.8539028573/kodexa_cli/charts/extension-pack/Chart.yaml
+-rw-r--r--   0        0        0        0 2024-04-03 12:52:35.958015 kodexa_cli-7.0.8539028573/kodexa_cli/charts/extension-pack/resources/.gitkeep
+-rw-r--r--   0        0        0       38 2024-04-03 12:52:35.958015 kodexa_cli-7.0.8539028573/kodexa_cli/charts/extension-pack/templates/NOTES.txt
+-rw-r--r--   0        0        0     1852 2024-04-03 12:52:35.958015 kodexa_cli-7.0.8539028573/kodexa_cli/charts/extension-pack/templates/_helpers.tpl
+-rw-r--r--   0        0        0      324 2024-04-03 12:52:35.958015 kodexa_cli-7.0.8539028573/kodexa_cli/charts/extension-pack/templates/configmap.yaml
+-rw-r--r--   0        0        0      250 2024-04-03 12:52:35.958015 kodexa_cli-7.0.8539028573/kodexa_cli/charts/extension-pack/values.yaml
+-rw-r--r--   0        0        0      402 2024-04-03 12:52:35.962015 kodexa_cli-7.0.8539028573/kodexa_cli/charts/resource-container/Dockerfile
+-rw-r--r--   0        0        0      174 2024-04-03 12:52:35.962015 kodexa_cli-7.0.8539028573/kodexa_cli/charts/resource-container/health-check.conf
+-rw-r--r--   0        0        0        0 2024-04-03 12:52:35.962015 kodexa_cli-7.0.8539028573/kodexa_cli/charts/resource-container/index.html
+-rw-r--r--   0        0        0      349 2024-04-03 12:52:35.962015 kodexa_cli-7.0.8539028573/kodexa_cli/charts/resource-pack/.helmignore
+-rw-r--r--   0        0        0      140 2024-04-03 12:52:35.962015 kodexa_cli-7.0.8539028573/kodexa_cli/charts/resource-pack/Chart.yaml
+-rw-r--r--   0        0        0     1528 2024-04-03 12:52:35.962015 kodexa_cli-7.0.8539028573/kodexa_cli/charts/resource-pack/templates/_helpers.tpl
+-rw-r--r--   0        0        0     1791 2024-04-03 12:52:35.962015 kodexa_cli-7.0.8539028573/kodexa_cli/charts/resource-pack/templates/deployment.yaml
+-rw-r--r--   0        0        0      410 2024-04-03 12:52:35.962015 kodexa_cli-7.0.8539028573/kodexa_cli/charts/resource-pack/templates/service.yaml
+-rw-r--r--   0        0        0      330 2024-04-03 12:52:35.962015 kodexa_cli-7.0.8539028573/kodexa_cli/charts/resource-pack/values.yaml
+-rw-r--r--   0        0        0    48926 2024-04-03 12:52:35.962015 kodexa_cli-7.0.8539028573/kodexa_cli/cli.py
+-rw-r--r--   0        0        0     7641 2024-04-03 12:52:35.962015 kodexa_cli-7.0.8539028573/kodexa_cli/documentation.py
+-rw-r--r--   0        0        0      134 2024-04-03 12:52:35.962015 kodexa_cli-7.0.8539028573/kodexa_cli/templates/action.jinja2
+-rw-r--r--   0        0        0     1356 2024-04-03 12:52:35.962015 kodexa_cli-7.0.8539028573/kodexa_cli/templates/assistant.jinja2
+-rw-r--r--   0        0        0     1021 2024-04-03 12:52:35.962015 kodexa_cli-7.0.8539028573/kodexa_cli/templates/content-taxon.jinja2
+-rw-r--r--   0        0        0      328 2024-04-03 12:52:35.962015 kodexa_cli-7.0.8539028573/kodexa_cli/templates/data-store.jinja2
+-rw-r--r--   0        0        0      707 2024-04-03 12:52:35.962015 kodexa_cli-7.0.8539028573/kodexa_cli/templates/document-store.jinja2
+-rw-r--r--   0        0        0       30 2024-04-03 12:52:35.962015 kodexa_cli-7.0.8539028573/kodexa_cli/templates/extension-pack.jinja2
+-rw-r--r--   0        0        0      818 2024-04-03 12:52:35.962015 kodexa_cli-7.0.8539028573/kodexa_cli/templates/header.jinja2
+-rw-r--r--   0        0        0      343 2024-04-03 12:52:35.962015 kodexa_cli-7.0.8539028573/kodexa_cli/templates/index.jinja2
+-rw-r--r--   0        0        0       30 2024-04-03 12:52:35.962015 kodexa_cli-7.0.8539028573/kodexa_cli/templates/model-runtime.jinja2
+-rw-r--r--   0        0        0     2999 2024-04-03 12:52:35.962015 kodexa_cli-7.0.8539028573/kodexa_cli/templates/model.jinja2
+-rw-r--r--   0        0        0     1137 2024-04-03 12:52:35.962015 kodexa_cli-7.0.8539028573/kodexa_cli/templates/options.jinja2
+-rw-r--r--   0        0        0        0 2024-04-03 12:52:35.962015 kodexa_cli-7.0.8539028573/kodexa_cli/templates/overview.jinja2
+-rw-r--r--   0        0        0      722 2024-04-03 12:52:35.962015 kodexa_cli-7.0.8539028573/kodexa_cli/templates/processing-taxon.jinja2
+-rw-r--r--   0        0        0       30 2024-04-03 12:52:35.962015 kodexa_cli-7.0.8539028573/kodexa_cli/templates/project-template.jinja2
+-rw-r--r--   0        0        0       30 2024-04-03 12:52:35.962015 kodexa_cli-7.0.8539028573/kodexa_cli/templates/store.jinja2
+-rw-r--r--   0        0        0      492 2024-04-03 12:52:35.962015 kodexa_cli-7.0.8539028573/kodexa_cli/templates/taxon.jinja2
+-rw-r--r--   0        0        0      273 2024-04-03 12:52:35.962015 kodexa_cli-7.0.8539028573/kodexa_cli/templates/taxonomy-labels.jinja2
+-rw-r--r--   0        0        0      534 2024-04-03 12:52:35.962015 kodexa_cli-7.0.8539028573/kodexa_cli/templates/taxonomy-structure.jinja2
+-rw-r--r--   0        0        0      269 2024-04-03 12:52:35.962015 kodexa_cli-7.0.8539028573/kodexa_cli/templates/taxonomy.jinja2
+-rw-r--r--   0        0        0      808 2024-04-03 12:52:51.805993 kodexa_cli-7.0.8539028573/pyproject.toml
+-rw-r--r--   0        0        0     3404 1970-01-01 00:00:00.000000 kodexa_cli-7.0.8539028573/setup.py
+-rw-r--r--   0        0        0     2767 1970-01-01 00:00:00.000000 kodexa_cli-7.0.8539028573/PKG-INFO
```

### Comparing `kodexa_cli-7.0.8535202482/LICENSE` & `kodexa_cli-7.0.8539028573/LICENSE`

 * *Files identical despite different names*

### Comparing `kodexa_cli-7.0.8535202482/README.md` & `kodexa_cli-7.0.8539028573/README.md`

 * *Files identical despite different names*

### Comparing `kodexa_cli-7.0.8535202482/kodexa_cli/charts/extension-pack/templates/_helpers.tpl` & `kodexa_cli-7.0.8539028573/kodexa_cli/charts/extension-pack/templates/_helpers.tpl`

 * *Files identical despite different names*

### Comparing `kodexa_cli-7.0.8535202482/kodexa_cli/charts/resource-pack/templates/_helpers.tpl` & `kodexa_cli-7.0.8539028573/kodexa_cli/charts/resource-pack/templates/_helpers.tpl`

 * *Files identical despite different names*

### Comparing `kodexa_cli-7.0.8535202482/kodexa_cli/charts/resource-pack/templates/deployment.yaml` & `kodexa_cli-7.0.8539028573/kodexa_cli/charts/resource-pack/templates/deployment.yaml`

 * *Files identical despite different names*

### Comparing `kodexa_cli-7.0.8535202482/kodexa_cli/cli.py` & `kodexa_cli-7.0.8539028573/kodexa_cli/cli.py`

 * *Files 0% similar despite different names*

```diff
@@ -965,17 +965,23 @@
 
     if platform_url is not None:
         print(f"URL: {get_current_kodexa_url()}")
 
         if show_token:
             print(f"Access Token: {get_current_access_token()}")
         kodexa_version = KodexaPlatform.get_server_info()
-        print(f"Environment: {kodexa_version['environment']}")
-        print(f"Version: {kodexa_version['version']}")
-        print(f"Release: {kodexa_version['release']}")
+
+        try:
+            print(kodexa_version)
+            print(f"Environment: {kodexa_version['environment']}")
+            print(f"Version: {kodexa_version['version']}")
+            print(f"Release: {kodexa_version['release']}")
+        except:
+            print("Unable to get environment details. Does this environment require a Cloudflare token?")
+
         if python:
             print("\nPython example:\n\n")
             print(f"from kodexa import KodexaClient")
             print(
                 f"client = KodexaClient('{get_current_kodexa_url()}', '{get_current_access_token()}')"
             )
     else:
```

### Comparing `kodexa_cli-7.0.8535202482/kodexa_cli/documentation.py` & `kodexa_cli-7.0.8539028573/kodexa_cli/documentation.py`

 * *Files identical despite different names*

### Comparing `kodexa_cli-7.0.8535202482/kodexa_cli/templates/assistant.jinja2` & `kodexa_cli-7.0.8539028573/kodexa_cli/templates/assistant.jinja2`

 * *Files identical despite different names*

### Comparing `kodexa_cli-7.0.8535202482/kodexa_cli/templates/content-taxon.jinja2` & `kodexa_cli-7.0.8539028573/kodexa_cli/templates/content-taxon.jinja2`

 * *Files identical despite different names*

### Comparing `kodexa_cli-7.0.8535202482/kodexa_cli/templates/document-store.jinja2` & `kodexa_cli-7.0.8539028573/kodexa_cli/templates/document-store.jinja2`

 * *Files identical despite different names*

### Comparing `kodexa_cli-7.0.8535202482/kodexa_cli/templates/header.jinja2` & `kodexa_cli-7.0.8539028573/kodexa_cli/templates/header.jinja2`

 * *Files identical despite different names*

### Comparing `kodexa_cli-7.0.8535202482/kodexa_cli/templates/model.jinja2` & `kodexa_cli-7.0.8539028573/kodexa_cli/templates/model.jinja2`

 * *Files identical despite different names*

### Comparing `kodexa_cli-7.0.8535202482/kodexa_cli/templates/options.jinja2` & `kodexa_cli-7.0.8539028573/kodexa_cli/templates/options.jinja2`

 * *Files identical despite different names*

### Comparing `kodexa_cli-7.0.8535202482/kodexa_cli/templates/processing-taxon.jinja2` & `kodexa_cli-7.0.8539028573/kodexa_cli/templates/processing-taxon.jinja2`

 * *Files identical despite different names*

### Comparing `kodexa_cli-7.0.8535202482/kodexa_cli/templates/taxonomy-structure.jinja2` & `kodexa_cli-7.0.8539028573/kodexa_cli/templates/taxonomy-structure.jinja2`

 * *Files identical despite different names*

### Comparing `kodexa_cli-7.0.8535202482/pyproject.toml` & `kodexa_cli-7.0.8539028573/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "kodexa-cli"
-version = "7.0.08535202482"
+version = "7.0.08539028573"
 description = "Command Line Tools for Kodexa"
 authors = ["Austin Redenbaugh <austin@kodexa.com>", "Philip Dodds <philip@kodexa.com>", "Romar Cablao <rcablao@kodexa.com>", "Amadea Paula Dodds <amadeapaula@kodexa.com>", "John Patrick Sese <jp@kodexa.com>"]
 readme = "README.md"
 packages = [{include = "kodexa_cli"}]
 
 [tool.poetry.scripts]
 kodexa = 'kodexa_cli.cli:safe_entry_point'
```

### Comparing `kodexa_cli-7.0.8535202482/setup.py` & `kodexa_cli-7.0.8539028573/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,15 +23,15 @@
  'wrapt>=1.15.0,<2.0.0']
 
 entry_points = \
 {'console_scripts': ['kodexa = kodexa_cli.cli:safe_entry_point']}
 
 setup_kwargs = {
     'name': 'kodexa-cli',
-    'version': '7.0.8535202482',
+    'version': '7.0.8539028573',
     'description': 'Command Line Tools for Kodexa',
     'long_description': '# Kodexa Command Line Tools\n\n[![Kodexa CLI Python Package](https://github.com/kodexa-ai/kodexa-cli/actions/workflows/build-and-release.yml/badge.svg)](https://github.com/kodexa-ai/kodexa-cli/actions/workflows/build-and-release.yml)\n\n![img.png](https://docs.kodexa.com/img.png)\n\nKodexa is a platform for building intelligent document processing pipelines. It is a set of tools and services that\nallow you to build a pipeline that can take a document, extract the content, and then process it to extract the\ninformation you need.\n\nIt is built on a set of core principles:\n\n* **Document Centric** - Kodexa is built around the idea of a document. A document is a collection of content\n  nodes that are connected together. This is a powerful model that allows you to build pipelines that can\n  extract content from a wide range of sources.\n\n* **Pipeline Oriented** - Kodexa is built around the idea of a pipeline. A pipeline is a series of steps that\n  can be executed on a document. This allows you to build a pipeline that can extract content from a wide range\n  of sources.\n\n* **Extensible** - Kodexa is built around the idea of a pipeline. A pipeline is a series of steps that can be executed\n  on a document. This allows you to build a pipeline that can extract content from a wide range of sources.\n\n* **Label Driven** - Kodexa focuses on the idea of labels. Labels are a way to identify content within a document\n  and then use that content to drive the processing of the document.\n\n# Command Line Tools\n\nThis repository contains the command line tools for Kodexa. The tools are the primary way to interact with Kodexa. It\nallows you to configure components and manage aspects of your Kodexa Platform installation.\n\n## Documentation & Examples\n\nDocumentation is available at the [Kodexa Documentation Portal](https://docs.kodexa.com)\n\n## Set-up\n\nWe use poetry to manage our dependencies, so you can install them with:\n\n    poetry install\n\nYou can then run the tests with:\n\n    poetry run pytest\n\n# Contributing\n\nWe welcome contributions to the Kodexa platform. Please see our [contributing guide](CONTRIBUTING.md) for more details.\n\n# License\n\nApache 2.0\n',
     'author': 'Austin Redenbaugh',
     'author_email': 'austin@kodexa.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `kodexa_cli-7.0.8535202482/PKG-INFO` & `kodexa_cli-7.0.8539028573/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kodexa-cli
-Version: 7.0.8535202482
+Version: 7.0.8539028573
 Summary: Command Line Tools for Kodexa
 Author: Austin Redenbaugh
 Author-email: austin@kodexa.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

