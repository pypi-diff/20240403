# Comparing `tmp/cam_utils-0.2.3.tar.gz` & `tmp/cam_utils-0.2.4.tar.gz`

## Comparing `cam_utils-0.2.3.tar` & `cam_utils-0.2.4.tar`

### file list

```diff
@@ -1,29 +1,29 @@
--rw-r--r--   0        0        0      742 2020-02-02 00:00:00.000000 cam_utils-0.2.3/.gitlab-ci.yml
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 cam_utils-0.2.3/CHANGELOG
--rw-r--r--   0        0        0      537 2020-02-02 00:00:00.000000 cam_utils-0.2.3/Makefile
--rw-r--r--   0        0        0     2452 2020-02-02 00:00:00.000000 cam_utils-0.2.3/cam_examples/exemplo_elastic.py
--rw-r--r--   0        0        0     2742 2020-02-02 00:00:00.000000 cam_utils-0.2.3/cam_examples/exemplo_rabbitmq.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cam_utils-0.2.3/cam_utils/__init__.py
--rw-r--r--   0        0        0     2308 2020-02-02 00:00:00.000000 cam_utils-0.2.3/cam_utils/api_request.py
--rw-r--r--   0        0        0     9986 2020-02-02 00:00:00.000000 cam_utils-0.2.3/cam_utils/db_elasticsearch.py
--rw-r--r--   0        0        0     3289 2020-02-02 00:00:00.000000 cam_utils-0.2.3/cam_utils/db_ldap.py
--rw-r--r--   0        0        0    10183 2020-02-02 00:00:00.000000 cam_utils-0.2.3/cam_utils/db_rabbitmq.py
--rw-r--r--   0        0        0     5017 2020-02-02 00:00:00.000000 cam_utils-0.2.3/cam_utils/valida_info.py
--rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 cam_utils-0.2.3/cam_utils/acsclient/__init__.py
--rw-r--r--   0        0        0     9757 2020-02-02 00:00:00.000000 cam_utils-0.2.3/cam_utils/acsclient/acsclient.py
--rw-r--r--   0        0        0      721 2020-02-02 00:00:00.000000 cam_utils-0.2.3/cam_utils/acsclient/templates/device.j2
--rw-r--r--   0        0        0      238 2020-02-02 00:00:00.000000 cam_utils-0.2.3/cam_utils/acsclient/templates/devicegroup.j2
--rw-r--r--   0        0        0      692 2020-02-02 00:00:00.000000 cam_utils-0.2.3/cam_utils/acsclient/templates/radius_device.j2
--rw-r--r--   0        0        0      581 2020-02-02 00:00:00.000000 cam_utils-0.2.3/cam_utils/acsclient/templates/search.j2
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 cam_utils-0.2.3/cam_utils/asterisk/__init__.py
--rw-r--r--   0        0        0     7620 2020-02-02 00:00:00.000000 cam_utils-0.2.3/cam_utils/asterisk/_actions.py
--rw-r--r--   0        0        0     9491 2020-02-02 00:00:00.000000 cam_utils-0.2.3/cam_utils/asterisk/ami13.py
--rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 cam_utils-0.2.3/cam_utils/asterisk/exceptions.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cam_utils-0.2.3/tests/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cam_utils-0.2.3/tests/asterisk/__init__.py
--rw-r--r--   0        0        0     7215 2020-02-02 00:00:00.000000 cam_utils-0.2.3/tests/asterisk/test_ami13.py
--rw-r--r--   0        0        0     3090 2020-02-02 00:00:00.000000 cam_utils-0.2.3/.gitignore
--rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 cam_utils-0.2.3/LICENSE
--rw-r--r--   0        0        0     2198 2020-02-02 00:00:00.000000 cam_utils-0.2.3/README.md
--rw-r--r--   0        0        0      664 2020-02-02 00:00:00.000000 cam_utils-0.2.3/pyproject.toml
--rw-r--r--   0        0        0     2799 2020-02-02 00:00:00.000000 cam_utils-0.2.3/PKG-INFO
+-rw-r--r--   0        0        0      742 2020-02-02 00:00:00.000000 cam_utils-0.2.4/.gitlab-ci.yml
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 cam_utils-0.2.4/CHANGELOG
+-rw-r--r--   0        0        0      537 2020-02-02 00:00:00.000000 cam_utils-0.2.4/Makefile
+-rw-r--r--   0        0        0     2452 2020-02-02 00:00:00.000000 cam_utils-0.2.4/cam_examples/exemplo_elastic.py
+-rw-r--r--   0        0        0     2742 2020-02-02 00:00:00.000000 cam_utils-0.2.4/cam_examples/exemplo_rabbitmq.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cam_utils-0.2.4/cam_utils/__init__.py
+-rw-r--r--   0        0        0     2308 2020-02-02 00:00:00.000000 cam_utils-0.2.4/cam_utils/api_request.py
+-rw-r--r--   0        0        0     9986 2020-02-02 00:00:00.000000 cam_utils-0.2.4/cam_utils/db_elasticsearch.py
+-rw-r--r--   0        0        0     3289 2020-02-02 00:00:00.000000 cam_utils-0.2.4/cam_utils/db_ldap.py
+-rw-r--r--   0        0        0    10183 2020-02-02 00:00:00.000000 cam_utils-0.2.4/cam_utils/db_rabbitmq.py
+-rw-r--r--   0        0        0     5017 2020-02-02 00:00:00.000000 cam_utils-0.2.4/cam_utils/valida_info.py
+-rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 cam_utils-0.2.4/cam_utils/acsclient/__init__.py
+-rw-r--r--   0        0        0     9757 2020-02-02 00:00:00.000000 cam_utils-0.2.4/cam_utils/acsclient/acsclient.py
+-rw-r--r--   0        0        0      721 2020-02-02 00:00:00.000000 cam_utils-0.2.4/cam_utils/acsclient/templates/device.j2
+-rw-r--r--   0        0        0      238 2020-02-02 00:00:00.000000 cam_utils-0.2.4/cam_utils/acsclient/templates/devicegroup.j2
+-rw-r--r--   0        0        0      692 2020-02-02 00:00:00.000000 cam_utils-0.2.4/cam_utils/acsclient/templates/radius_device.j2
+-rw-r--r--   0        0        0      581 2020-02-02 00:00:00.000000 cam_utils-0.2.4/cam_utils/acsclient/templates/search.j2
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 cam_utils-0.2.4/cam_utils/asterisk/__init__.py
+-rw-r--r--   0        0        0     7620 2020-02-02 00:00:00.000000 cam_utils-0.2.4/cam_utils/asterisk/_actions.py
+-rw-r--r--   0        0        0     9491 2020-02-02 00:00:00.000000 cam_utils-0.2.4/cam_utils/asterisk/ami13.py
+-rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 cam_utils-0.2.4/cam_utils/asterisk/exceptions.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cam_utils-0.2.4/tests/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cam_utils-0.2.4/tests/asterisk/__init__.py
+-rw-r--r--   0        0        0     7215 2020-02-02 00:00:00.000000 cam_utils-0.2.4/tests/asterisk/test_ami13.py
+-rw-r--r--   0        0        0     3090 2020-02-02 00:00:00.000000 cam_utils-0.2.4/.gitignore
+-rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 cam_utils-0.2.4/LICENSE
+-rw-r--r--   0        0        0     2198 2020-02-02 00:00:00.000000 cam_utils-0.2.4/README.md
+-rw-r--r--   0        0        0      663 2020-02-02 00:00:00.000000 cam_utils-0.2.4/pyproject.toml
+-rw-r--r--   0        0        0     2798 2020-02-02 00:00:00.000000 cam_utils-0.2.4/PKG-INFO
```

### Comparing `cam_utils-0.2.3/.gitlab-ci.yml` & `cam_utils-0.2.4/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `cam_utils-0.2.3/Makefile` & `cam_utils-0.2.4/Makefile`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 
 NAME=cam_utils
-VERSION=0.2.3
+VERSION=0.2.4
 PYTHON = python3
 
 
 
 # Define targets and their dependencies
 all: build upload
```

### Comparing `cam_utils-0.2.3/cam_examples/exemplo_elastic.py` & `cam_utils-0.2.4/cam_examples/exemplo_elastic.py`

 * *Files identical despite different names*

### Comparing `cam_utils-0.2.3/cam_examples/exemplo_rabbitmq.py` & `cam_utils-0.2.4/cam_examples/exemplo_rabbitmq.py`

 * *Files identical despite different names*

### Comparing `cam_utils-0.2.3/cam_utils/api_request.py` & `cam_utils-0.2.4/cam_utils/api_request.py`

 * *Files identical despite different names*

### Comparing `cam_utils-0.2.3/cam_utils/db_elasticsearch.py` & `cam_utils-0.2.4/cam_utils/db_elasticsearch.py`

 * *Files identical despite different names*

### Comparing `cam_utils-0.2.3/cam_utils/db_ldap.py` & `cam_utils-0.2.4/cam_utils/db_ldap.py`

 * *Files identical despite different names*

### Comparing `cam_utils-0.2.3/cam_utils/db_rabbitmq.py` & `cam_utils-0.2.4/cam_utils/db_rabbitmq.py`

 * *Files identical despite different names*

### Comparing `cam_utils-0.2.3/cam_utils/valida_info.py` & `cam_utils-0.2.4/cam_utils/valida_info.py`

 * *Files identical despite different names*

### Comparing `cam_utils-0.2.3/cam_utils/acsclient/acsclient.py` & `cam_utils-0.2.4/cam_utils/acsclient/acsclient.py`

 * *Files identical despite different names*

### Comparing `cam_utils-0.2.3/cam_utils/acsclient/templates/device.j2` & `cam_utils-0.2.4/cam_utils/acsclient/templates/device.j2`

 * *Files identical despite different names*

### Comparing `cam_utils-0.2.3/cam_utils/acsclient/templates/radius_device.j2` & `cam_utils-0.2.4/cam_utils/acsclient/templates/radius_device.j2`

 * *Files identical despite different names*

### Comparing `cam_utils-0.2.3/cam_utils/acsclient/templates/search.j2` & `cam_utils-0.2.4/cam_utils/acsclient/templates/search.j2`

 * *Files identical despite different names*

### Comparing `cam_utils-0.2.3/cam_utils/asterisk/_actions.py` & `cam_utils-0.2.4/cam_utils/asterisk/_actions.py`

 * *Files identical despite different names*

### Comparing `cam_utils-0.2.3/cam_utils/asterisk/ami13.py` & `cam_utils-0.2.4/cam_utils/asterisk/ami13.py`

 * *Files identical despite different names*

### Comparing `cam_utils-0.2.3/tests/asterisk/test_ami13.py` & `cam_utils-0.2.4/tests/asterisk/test_ami13.py`

 * *Files identical despite different names*

### Comparing `cam_utils-0.2.3/.gitignore` & `cam_utils-0.2.4/.gitignore`

 * *Files identical despite different names*

### Comparing `cam_utils-0.2.3/README.md` & `cam_utils-0.2.4/README.md`

 * *Files identical despite different names*

### Comparing `cam_utils-0.2.3/pyproject.toml` & `cam_utils-0.2.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "cam_utils"
-version = "0.2.3"
+version = "0.2.4"
 authors = [
     { name = "CAM TECNOLOGIA LTDA ME", email = "atendimento@camtecnologia.com.br" },
 ]
 description = "CAM UTILS LIBRARY TO PYTHON PROJECTS"
 readme = "README.md"
-requires-python = ">=3.12"
+requires-python = ">=3.8"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: POSIX :: Linux",
 ]
 
 [project.urls]
```

### Comparing `cam_utils-0.2.3/PKG-INFO` & `cam_utils-0.2.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.3
 Name: cam_utils
-Version: 0.2.3
+Version: 0.2.4
 Summary: CAM UTILS LIBRARY TO PYTHON PROJECTS
 Project-URL: Homepage, https://repo.camvoip.com.br/engenharia/bibliotecas-cam/python/cam_utils
 Project-URL: Issues, https://repo.camvoip.com.br/engenharia/bibliotecas-cam/python/cam_utils/-/issues
 Author-email: CAM TECNOLOGIA LTDA ME <atendimento@camtecnologia.com.br>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.12
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 
 # biblioteca cam_utils
 
 Bem vindo a 1a biblioteca Python3 da CAM Tecnologia para ser incorporada e reutilizada nos projetos de desenvolvimento Pyhton. 
 A biblioteca `cam_utils` na versão atual foi desenvolvida para Python 3 e armazenada livremente no PyPI:
```

