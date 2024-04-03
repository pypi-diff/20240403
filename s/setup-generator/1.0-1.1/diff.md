# Comparing `tmp/setup-generator-1.0.tar.gz` & `tmp/setup-generator-1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "setup-generator-1.0.tar", last modified: Wed Jan 10 03:55:10 2024, max compression
+gzip compressed data, was "setup-generator-1.1.tar", last modified: Wed Apr  3 05:26:12 2024, max compression
```

## Comparing `setup-generator-1.0.tar` & `setup-generator-1.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2024-01-10 03:55:10.768833 setup-generator-1.0/
--rw-rw-rw-   0        0        0    35145 2024-01-03 04:45:08.000000 setup-generator-1.0/LICENSE
--rw-rw-rw-   0        0        0     1193 2024-01-10 03:55:10.768833 setup-generator-1.0/PKG-INFO
--rw-rw-rw-   0        0        0      628 2024-01-10 03:29:11.000000 setup-generator-1.0/README.md
--rw-rw-rw-   0        0        0       42 2024-01-10 03:55:10.768833 setup-generator-1.0/setup.cfg
--rw-rw-rw-   0        0        0      963 2024-01-10 03:51:05.000000 setup-generator-1.0/setup.py
-drwxrwxrwx   0        0        0        0 2024-01-10 03:55:10.751551 setup-generator-1.0/setupGenerator/
--rw-rw-rw-   0        0        0      694 2024-01-10 03:50:53.000000 setup-generator-1.0/setupGenerator/.template
--rw-rw-rw-   0        0        0       42 2024-01-10 03:38:58.000000 setup-generator-1.0/setupGenerator/__init__.py
-drwxrwxrwx   0        0        0        0 2024-01-10 03:55:10.751551 setup-generator-1.0/setupGenerator/scripts/
--rw-rw-rw-   0        0        0       38 2024-01-10 03:45:11.000000 setup-generator-1.0/setupGenerator/scripts/__init__.py
--rw-rw-rw-   0        0        0      999 2024-01-10 03:02:50.000000 setup-generator-1.0/setupGenerator/scripts/getPipFreeze.py
--rw-rw-rw-   0        0        0     2372 2024-01-10 03:45:24.000000 setup-generator-1.0/setupGenerator/setupGenerator.py
-drwxrwxrwx   0        0        0        0 2024-01-10 03:55:10.768833 setup-generator-1.0/setup_generator.egg-info/
--rw-rw-rw-   0        0        0     1193 2024-01-10 03:55:10.000000 setup-generator-1.0/setup_generator.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      421 2024-01-10 03:55:10.000000 setup-generator-1.0/setup_generator.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-01-10 03:55:10.000000 setup-generator-1.0/setup_generator.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       81 2024-01-10 03:55:10.000000 setup-generator-1.0/setup_generator.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      127 2024-01-10 03:55:10.000000 setup-generator-1.0/setup_generator.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2024-01-10 03:55:10.000000 setup-generator-1.0/setup_generator.egg-info/top_level.txt
+drwxrwxr-x   0 hoy       (1000) hoy       (1000)        0 2024-04-03 05:26:12.927520 setup-generator-1.1/
+-rw-rw-r--   0 hoy       (1000) hoy       (1000)    35145 2024-01-03 04:45:08.000000 setup-generator-1.1/LICENSE
+-rw-r--r--   0 hoy       (1000) hoy       (1000)     1159 2024-04-03 05:26:12.927520 setup-generator-1.1/PKG-INFO
+-rw-rw-r--   0 hoy       (1000) hoy       (1000)      628 2024-01-10 03:29:11.000000 setup-generator-1.1/README.md
+-rw-rw-r--   0 hoy       (1000) hoy       (1000)       38 2024-04-03 05:26:12.927520 setup-generator-1.1/setup.cfg
+-rw-rw-r--   0 hoy       (1000) hoy       (1000)      963 2024-04-03 05:24:25.000000 setup-generator-1.1/setup.py
+drwxrwxr-x   0 hoy       (1000) hoy       (1000)        0 2024-04-03 05:26:12.927520 setup-generator-1.1/setupGenerator/
+-rw-rw-r--   0 hoy       (1000) hoy       (1000)      694 2024-01-10 03:50:53.000000 setup-generator-1.1/setupGenerator/.template
+-rw-rw-r--   0 hoy       (1000) hoy       (1000)       42 2024-01-10 03:38:58.000000 setup-generator-1.1/setupGenerator/__init__.py
+drwxrwxr-x   0 hoy       (1000) hoy       (1000)        0 2024-04-03 05:26:12.927520 setup-generator-1.1/setupGenerator/scripts/
+-rw-rw-r--   0 hoy       (1000) hoy       (1000)       38 2024-01-10 03:45:11.000000 setup-generator-1.1/setupGenerator/scripts/__init__.py
+-rw-rw-r--   0 hoy       (1000) hoy       (1000)     1037 2024-04-03 05:20:05.000000 setup-generator-1.1/setupGenerator/scripts/getPipFreeze.py
+-rw-rw-r--   0 hoy       (1000) hoy       (1000)     2464 2024-04-03 05:22:39.000000 setup-generator-1.1/setupGenerator/setupGenerator.py
+drwxrwxr-x   0 hoy       (1000) hoy       (1000)        0 2024-04-03 05:26:12.927520 setup-generator-1.1/setup_generator.egg-info/
+-rw-r--r--   0 hoy       (1000) hoy       (1000)     1159 2024-04-03 05:26:12.000000 setup-generator-1.1/setup_generator.egg-info/PKG-INFO
+-rw-rw-r--   0 hoy       (1000) hoy       (1000)      421 2024-04-03 05:26:12.000000 setup-generator-1.1/setup_generator.egg-info/SOURCES.txt
+-rw-rw-r--   0 hoy       (1000) hoy       (1000)        1 2024-04-03 05:26:12.000000 setup-generator-1.1/setup_generator.egg-info/dependency_links.txt
+-rw-rw-r--   0 hoy       (1000) hoy       (1000)       81 2024-04-03 05:26:12.000000 setup-generator-1.1/setup_generator.egg-info/entry_points.txt
+-rw-rw-r--   0 hoy       (1000) hoy       (1000)      127 2024-04-03 05:26:12.000000 setup-generator-1.1/setup_generator.egg-info/requires.txt
+-rw-rw-r--   0 hoy       (1000) hoy       (1000)       15 2024-04-03 05:26:12.000000 setup-generator-1.1/setup_generator.egg-info/top_level.txt
```

### Comparing `setup-generator-1.0/LICENSE` & `setup-generator-1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `setup-generator-1.0/PKG-INFO` & `setup-generator-1.1/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,34 +1,34 @@
-Metadata-Version: 2.1
-Name: setup-generator
-Version: 1.0
-Summary: Pequena biblioteca para criar um setup.py rápido.
-Home-page: https://github.com/Hoyasumii/SetupGenerator
-Author: Alan Reis Anjos
-Author-email: alanreisanjo@gmail.com
-License: GPL-3.0
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: Jinja2==3.1.2
-Requires-Dist: keyboard==0.13.5
-Requires-Dist: MarkupSafe==2.1.3
-Requires-Dist: python-slugify==8.0.1
-Requires-Dist: setuptools==69.0.3
-Requires-Dist: simple-form==1.0
-Requires-Dist: text-unidecode==1.3
-
-## [SetupGenerator](https://pypi.org/project/setup-generator/)
-- Pequena biblioteca para criar um setup.py rápido.
-- Clique [**aqui**](https://github.com/Hoyasumii/SetupGenerator) para acessar o repositório.
----
-## Instalação
-- Você pode baixar pelo pip:
-```
-pip install setup-generator
-```
----
-## Como usar?
-- Abra o terminal e digite:
-```
-setup-generator 
-```
-- Depois disso, você será solicitado a digitar o nome do seu projeto, o nome do autor, a versão do projeto, a descrição do projeto, o nome do arquivo principal e o nome do arquivo de instalação. Após isso, o arquivo setup.py será criado.
+Metadata-Version: 2.1
+Name: setup-generator
+Version: 1.1
+Summary: Pequena biblioteca para criar um setup.py rápido.
+Home-page: https://github.com/Hoyasumii/SetupGenerator
+Author: Alan Reis Anjos
+Author-email: alanreisanjo@gmail.com
+License: GPL-3.0
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: Jinja2==3.1.2
+Requires-Dist: keyboard==0.13.5
+Requires-Dist: MarkupSafe==2.1.3
+Requires-Dist: python-slugify==8.0.1
+Requires-Dist: setuptools==69.0.3
+Requires-Dist: simple-form==1.4
+Requires-Dist: text-unidecode==1.3
+
+## [SetupGenerator](https://pypi.org/project/setup-generator/)
+- Pequena biblioteca para criar um setup.py rápido.
+- Clique [**aqui**](https://github.com/Hoyasumii/SetupGenerator) para acessar o repositório.
+---
+## Instalação
+- Você pode baixar pelo pip:
+```
+pip install setup-generator
+```
+---
+## Como usar?
+- Abra o terminal e digite:
+```
+setup-generator 
+```
+- Depois disso, você será solicitado a digitar o nome do seu projeto, o nome do autor, a versão do projeto, a descrição do projeto, o nome do arquivo principal e o nome do arquivo de instalação. Após isso, o arquivo setup.py será criado.
```

### Comparing `setup-generator-1.0/README.md` & `setup-generator-1.1/README.md`

 * *Files identical despite different names*

### Comparing `setup-generator-1.0/setup.py` & `setup-generator-1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,22 +3,22 @@
 
 if os.path.isfile("README.md"):
     with open("README.md", "r", encoding="utf-8") as readme:
         long_description = readme.read()
 
 setup(
     name="setup-generator",
-    version=1.0,
+    version=1.1,
     description="Pequena biblioteca para criar um setup.py rápido.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="Alan Reis Anjos",
     author_email="alanreisanjo@gmail.com",
     url="https://github.com/Hoyasumii/SetupGenerator",
     packages=['setupGenerator', 'setupGenerator.scripts'],
     package_data={'setupGenerator': ['.template']},
-    install_requires=['Jinja2==3.1.2', 'keyboard==0.13.5', 'MarkupSafe==2.1.3', 'python-slugify==8.0.1', 'setuptools==69.0.3', 'simple-form==1.0', 'text-unidecode==1.3'],
+    install_requires=['Jinja2==3.1.2', 'keyboard==0.13.5', 'MarkupSafe==2.1.3', 'python-slugify==8.0.1', 'setuptools==69.0.3', 'simple-form==1.4', 'text-unidecode==1.3'],
     license="GPL-3.0",
     entry_points={'console_scripts': [
         "setup-generator = setupGenerator.setupGenerator:setupGenerator"
     ]}
 )
```

### Comparing `setup-generator-1.0/setupGenerator/.template` & `setup-generator-1.1/setupGenerator/.template`

 * *Files identical despite different names*

### Comparing `setup-generator-1.0/setupGenerator/scripts/getPipFreeze.py` & `setup-generator-1.1/setupGenerator/scripts/getPipFreeze.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 import subprocess, os
 
 def getPipFreeze():
 
     # Get Virtual Enviroment name
     venv = os.environ.get("VIRTUAL_ENV")
 
+
     if venv is not None:
-        venv = venv.split("\\")[-1]
+        venv = venv.split("\\")[-1] if os.name == "nt" else venv.split("/")[-1]
 
         install_requires = None
         
         if os.name == "nt":
             install_requires = subprocess.run([f".\\{ venv }\\Scripts\\python", "-m", "pip", "freeze"], capture_output=True)
         else:
-            install_requires = subprocess.run(["source", f"./{ venv }/bin/python", "-m", "pip", "freeze"], capture_output=True)
+            install_requires = subprocess.run([f"./{ venv }/bin/python", "-m", "pip", "freeze"], capture_output=True)
     
     else:
         if os.name == "nt":
             install_requires = subprocess.run(["python", "-m", "pip", "freeze"], capture_output=True)
         else:
             install_requires = subprocess.run(["python3", "-m", "pip", "freeze"], capture_output=True)
 
     install_requires = install_requires.stdout.decode("utf-8").split("\n")
     install_requires = [ package[:-1] for package in install_requires if package != "" ]
 
-    return install_requires
+    return install_requires
```

### Comparing `setup-generator-1.0/setupGenerator/setupGenerator.py` & `setup-generator-1.1/setupGenerator/setupGenerator.py`

 * *Files 16% similar despite different names*

```diff
@@ -58,15 +58,17 @@
 
     data['packages'] = find_packages()
     data['package_data'] = { key: [ item for item in os.listdir(key.replace('.', '/')) if not item.endswith(".py") and os.path.isfile(f"{os.getcwd()}\\{ key }\\{ item }") ] for key in data['packages'] }
 
     data['install_requires'] = getPipFreeze()
     data['entry_points'] = { 'console_scripts': [ ] }
 
-    with open(f"{ libPath }\\.template", "r", encoding="utf-8") as templateFile:
+    templateFileName = f"{ libPath }\\.template" if os.name == "nt" else f"{ libPath }/.template"
+
+    with open(templateFileName, "r", encoding="utf-8") as templateFile:
         template = Template(templateFile.read())
 
     output = template.render(data)
 
     with open("setup.py", "w", encoding="utf-8") as setupFile:
         setupFile.write(output)
```

### Comparing `setup-generator-1.0/setup_generator.egg-info/PKG-INFO` & `setup-generator-1.1/setup_generator.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,34 +1,34 @@
-Metadata-Version: 2.1
-Name: setup-generator
-Version: 1.0
-Summary: Pequena biblioteca para criar um setup.py rápido.
-Home-page: https://github.com/Hoyasumii/SetupGenerator
-Author: Alan Reis Anjos
-Author-email: alanreisanjo@gmail.com
-License: GPL-3.0
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: Jinja2==3.1.2
-Requires-Dist: keyboard==0.13.5
-Requires-Dist: MarkupSafe==2.1.3
-Requires-Dist: python-slugify==8.0.1
-Requires-Dist: setuptools==69.0.3
-Requires-Dist: simple-form==1.0
-Requires-Dist: text-unidecode==1.3
-
-## [SetupGenerator](https://pypi.org/project/setup-generator/)
-- Pequena biblioteca para criar um setup.py rápido.
-- Clique [**aqui**](https://github.com/Hoyasumii/SetupGenerator) para acessar o repositório.
----
-## Instalação
-- Você pode baixar pelo pip:
-```
-pip install setup-generator
-```
----
-## Como usar?
-- Abra o terminal e digite:
-```
-setup-generator 
-```
-- Depois disso, você será solicitado a digitar o nome do seu projeto, o nome do autor, a versão do projeto, a descrição do projeto, o nome do arquivo principal e o nome do arquivo de instalação. Após isso, o arquivo setup.py será criado.
+Metadata-Version: 2.1
+Name: setup-generator
+Version: 1.1
+Summary: Pequena biblioteca para criar um setup.py rápido.
+Home-page: https://github.com/Hoyasumii/SetupGenerator
+Author: Alan Reis Anjos
+Author-email: alanreisanjo@gmail.com
+License: GPL-3.0
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: Jinja2==3.1.2
+Requires-Dist: keyboard==0.13.5
+Requires-Dist: MarkupSafe==2.1.3
+Requires-Dist: python-slugify==8.0.1
+Requires-Dist: setuptools==69.0.3
+Requires-Dist: simple-form==1.4
+Requires-Dist: text-unidecode==1.3
+
+## [SetupGenerator](https://pypi.org/project/setup-generator/)
+- Pequena biblioteca para criar um setup.py rápido.
+- Clique [**aqui**](https://github.com/Hoyasumii/SetupGenerator) para acessar o repositório.
+---
+## Instalação
+- Você pode baixar pelo pip:
+```
+pip install setup-generator
+```
+---
+## Como usar?
+- Abra o terminal e digite:
+```
+setup-generator 
+```
+- Depois disso, você será solicitado a digitar o nome do seu projeto, o nome do autor, a versão do projeto, a descrição do projeto, o nome do arquivo principal e o nome do arquivo de instalação. Após isso, o arquivo setup.py será criado.
```

