# Comparing `tmp/pyscal_rdf-0.1.6.tar.gz` & `tmp/pyscal_rdf-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyscal_rdf-0.1.6.tar", last modified: Thu Feb 15 17:45:15 2024, max compression
+gzip compressed data, was "pyscal_rdf-0.1.7.tar", last modified: Wed Apr  3 08:59:32 2024, max compression
```

## Comparing `pyscal_rdf-0.1.6.tar` & `pyscal_rdf-0.1.7.tar`

### file list

```diff
@@ -1,24 +1,41 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 17:45:15.749330 pyscal_rdf-0.1.6/
--rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-02-15 17:44:45.000000 pyscal_rdf-0.1.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-02-15 17:44:45.000000 pyscal_rdf-0.1.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     2871 2024-02-15 17:45:15.749330 pyscal_rdf-0.1.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1957 2024-02-15 17:44:45.000000 pyscal_rdf-0.1.6/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1180 2024-02-15 17:44:45.000000 pyscal_rdf-0.1.6/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 17:45:15.745330 pyscal_rdf-0.1.6/pyscal_rdf/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 17:45:15.745330 pyscal_rdf-0.1.6/pyscal_rdf/data/
--rw-r--r--   0 runner    (1001) docker     (127)    52826 2024-02-15 17:44:45.000000 pyscal_rdf-0.1.6/pyscal_rdf/data/asmo.owl
--rw-r--r--   0 runner    (1001) docker     (127)    63736 2024-02-15 17:44:45.000000 pyscal_rdf-0.1.6/pyscal_rdf/data/cmso.owl
--rw-r--r--   0 runner    (1001) docker     (127)     3963 2024-02-15 17:44:45.000000 pyscal_rdf-0.1.6/pyscal_rdf/data/element.yml
--rw-r--r--   0 runner    (1001) docker     (127)    29789 2024-02-15 17:44:45.000000 pyscal_rdf-0.1.6/pyscal_rdf/data/pldo.owl
--rw-r--r--   0 runner    (1001) docker     (127)    23430 2024-02-15 17:44:45.000000 pyscal_rdf-0.1.6/pyscal_rdf/data/podo.owl
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 17:45:15.749330 pyscal_rdf-0.1.6/pyscal_rdf/data/pyscal_rdf.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2871 2024-02-15 17:45:15.000000 pyscal_rdf-0.1.6/pyscal_rdf/data/pyscal_rdf.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      502 2024-02-15 17:45:15.000000 pyscal_rdf-0.1.6/pyscal_rdf/data/pyscal_rdf.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-15 17:45:15.000000 pyscal_rdf-0.1.6/pyscal_rdf/data/pyscal_rdf.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       70 2024-02-15 17:45:15.000000 pyscal_rdf-0.1.6/pyscal_rdf/data/pyscal_rdf.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-15 17:45:15.000000 pyscal_rdf-0.1.6/pyscal_rdf/data/pyscal_rdf.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-15 17:45:15.749330 pyscal_rdf-0.1.6/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-15 17:45:15.749330 pyscal_rdf-0.1.6/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      533 2024-02-15 17:44:45.000000 pyscal_rdf-0.1.6/tests/test_encoder_and_write.py
--rw-r--r--   0 runner    (1001) docker     (127)      534 2024-02-15 17:44:45.000000 pyscal_rdf-0.1.6/tests/test_graph.py
--rw-r--r--   0 runner    (1001) docker     (127)      545 2024-02-15 17:44:45.000000 pyscal_rdf-0.1.6/tests/test_structuregraph.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 08:59:32.855282 pyscal_rdf-0.1.7/
+-rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-04-03 08:59:30.000000 pyscal_rdf-0.1.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-03 08:59:30.000000 pyscal_rdf-0.1.7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2767 2024-04-03 08:59:32.855282 pyscal_rdf-0.1.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2129 2024-04-03 08:59:30.000000 pyscal_rdf-0.1.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 08:59:32.851282 pyscal_rdf-0.1.7/pyscal_rdf/
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-03 08:59:30.000000 pyscal_rdf-0.1.7/pyscal_rdf/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 08:59:32.851282 pyscal_rdf-0.1.7/pyscal_rdf/data/
+-rw-r--r--   0 runner    (1001) docker     (127)    52826 2024-04-03 08:59:30.000000 pyscal_rdf-0.1.7/pyscal_rdf/data/asmo.owl
+-rw-r--r--   0 runner    (1001) docker     (127)    63736 2024-04-03 08:59:30.000000 pyscal_rdf-0.1.7/pyscal_rdf/data/cmso.owl
+-rw-r--r--   0 runner    (1001) docker     (127)     3963 2024-04-03 08:59:30.000000 pyscal_rdf-0.1.7/pyscal_rdf/data/element.yml
+-rw-r--r--   0 runner    (1001) docker     (127)    29789 2024-04-03 08:59:30.000000 pyscal_rdf-0.1.7/pyscal_rdf/data/pldo.owl
+-rw-r--r--   0 runner    (1001) docker     (127)    23430 2024-04-03 08:59:30.000000 pyscal_rdf-0.1.7/pyscal_rdf/data/podo.owl
+-rw-r--r--   0 runner    (1001) docker     (127)      455 2024-04-03 08:59:30.000000 pyscal_rdf-0.1.7/pyscal_rdf/encoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)    39539 2024-04-03 08:59:30.000000 pyscal_rdf-0.1.7/pyscal_rdf/graph.py
+-rw-r--r--   0 runner    (1001) docker     (127)      589 2024-04-03 08:59:30.000000 pyscal_rdf-0.1.7/pyscal_rdf/json_io.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 08:59:32.851282 pyscal_rdf-0.1.7/pyscal_rdf/network/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 08:59:30.000000 pyscal_rdf-0.1.7/pyscal_rdf/network/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9952 2024-04-03 08:59:30.000000 pyscal_rdf-0.1.7/pyscal_rdf/network/network.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2730 2024-04-03 08:59:30.000000 pyscal_rdf-0.1.7/pyscal_rdf/network/ontology.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8601 2024-04-03 08:59:30.000000 pyscal_rdf-0.1.7/pyscal_rdf/network/parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)      844 2024-04-03 08:59:30.000000 pyscal_rdf-0.1.7/pyscal_rdf/network/patch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6774 2024-04-03 08:59:30.000000 pyscal_rdf-0.1.7/pyscal_rdf/network/term.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4971 2024-04-03 08:59:30.000000 pyscal_rdf-0.1.7/pyscal_rdf/properties.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4623 2024-04-03 08:59:30.000000 pyscal_rdf-0.1.7/pyscal_rdf/rdfsystem.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9682 2024-04-03 08:59:30.000000 pyscal_rdf-0.1.7/pyscal_rdf/structure.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10210 2024-04-03 08:59:30.000000 pyscal_rdf-0.1.7/pyscal_rdf/visualize.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8065 2024-04-03 08:59:30.000000 pyscal_rdf-0.1.7/pyscal_rdf/workflow.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 08:59:32.855282 pyscal_rdf-0.1.7/pyscal_rdf.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2767 2024-04-03 08:59:32.000000 pyscal_rdf-0.1.7/pyscal_rdf.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      832 2024-04-03 08:59:32.000000 pyscal_rdf-0.1.7/pyscal_rdf.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 08:59:32.000000 pyscal_rdf-0.1.7/pyscal_rdf.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 08:59:32.000000 pyscal_rdf-0.1.7/pyscal_rdf.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-04-03 08:59:32.000000 pyscal_rdf-0.1.7/pyscal_rdf.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-03 08:59:32.000000 pyscal_rdf-0.1.7/pyscal_rdf.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-03 08:59:32.855282 pyscal_rdf-0.1.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      847 2024-04-03 08:59:32.000000 pyscal_rdf-0.1.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 08:59:32.855282 pyscal_rdf-0.1.7/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      533 2024-04-03 08:59:30.000000 pyscal_rdf-0.1.7/tests/test_encoder_and_write.py
+-rw-r--r--   0 runner    (1001) docker     (127)      534 2024-04-03 08:59:30.000000 pyscal_rdf-0.1.7/tests/test_graph.py
+-rw-r--r--   0 runner    (1001) docker     (127)      545 2024-04-03 08:59:30.000000 pyscal_rdf-0.1.7/tests/test_structuregraph.py
```

### Comparing `pyscal_rdf-0.1.6/LICENSE` & `pyscal_rdf-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `pyscal_rdf-0.1.6/PKG-INFO` & `pyscal_rdf-0.1.7/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,31 +1,29 @@
 Metadata-Version: 2.1
 Name: pyscal_rdf
-Version: 0.1.6
+Version: 0.1.7
 Summary: Ontology based structural manipulation and quering
-Author-email: Abril Azocar Guzman <a.azocar.guzman@fz-juelich.de>, Sarath Menon <sarath.menon@pyscal.org>
-Maintainer-email: Sarath Menon <sarath.menon@pyscal.org>
-License: MIT License
-Project-URL: Homepage, https://pyscal.org
-Project-URL: Documentation, https://rdf.pyscal.org
-Project-URL: Repository, https://github.com/pyscal/pyscal_rdf
-Keywords: ontology,research-data-management,rdm,computational-materials-science,atomic-simulation,atomic-structures
+Home-page: https://pyscal.org
+Download-URL: https://github.com/pyscal/pyscal_rdf
+Author: Abril Azocar Guzman, Sarath Menon
+Author-email: sarath.menon@pyscal.org
 Classifier: Programming Language :: Python :: 3
-Requires-Python: <3.12,>=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy
 Requires-Dist: ase
 Requires-Dist: rdflib
 Requires-Dist: pyyaml
 Requires-Dist: graphviz
 Requires-Dist: networkx
 Requires-Dist: ipycytoscape
 Requires-Dist: pyscal3
 Requires-Dist: spglib
+Requires-Dist: pandas
+Requires-Dist: owlready2
 
 # pyscal_rdf
 
 `pyscal_rdf` is a python tool for ontology-based creation, manipulation, and quering of structures. `pyscal_rdf` uses the [Computational Material Sample Ontology (CMSO)](https://github.com/Materials-Data-Science-and-Informatics/cmso-ontology). 
 
 The package is currently under activate development and could be  unstable .
 
@@ -84,9 +82,11 @@
 
 ## Using `pyscal_rdf`
 
 Coming soon..
 
 
 ## Acknowledgements
-
 This work is supported by the [NFDI-Matwerk](https://nfdi-matwerk.de/) consortia.
+
+Funded by the Deutsche Forschungsgemeinschaft (DFG, German Research Foundation) under the National Research Data Infrastructure – NFDI 38/1 – project number 460247524
+
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `pyscal_rdf-0.1.6/README.md` & `pyscal_rdf-0.1.7/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -59,9 +59,11 @@
 
 ## Using `pyscal_rdf`
 
 Coming soon..
 
 
 ## Acknowledgements
-
 This work is supported by the [NFDI-Matwerk](https://nfdi-matwerk.de/) consortia.
+
+Funded by the Deutsche Forschungsgemeinschaft (DFG, German Research Foundation) under the National Research Data Infrastructure – NFDI 38/1 – project number 460247524
+
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `pyscal_rdf-0.1.6/pyscal_rdf/data/asmo.owl` & `pyscal_rdf-0.1.7/pyscal_rdf/data/asmo.owl`

 * *Files identical despite different names*

### Comparing `pyscal_rdf-0.1.6/pyscal_rdf/data/cmso.owl` & `pyscal_rdf-0.1.7/pyscal_rdf/data/cmso.owl`

 * *Files identical despite different names*

### Comparing `pyscal_rdf-0.1.6/pyscal_rdf/data/element.yml` & `pyscal_rdf-0.1.7/pyscal_rdf/data/element.yml`

 * *Files identical despite different names*

### Comparing `pyscal_rdf-0.1.6/pyscal_rdf/data/pldo.owl` & `pyscal_rdf-0.1.7/pyscal_rdf/data/pldo.owl`

 * *Files identical despite different names*

### Comparing `pyscal_rdf-0.1.6/pyscal_rdf/data/podo.owl` & `pyscal_rdf-0.1.7/pyscal_rdf/data/podo.owl`

 * *Files identical despite different names*

### Comparing `pyscal_rdf-0.1.6/pyscal_rdf/data/pyscal_rdf.egg-info/PKG-INFO` & `pyscal_rdf-0.1.7/pyscal_rdf.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,31 +1,29 @@
 Metadata-Version: 2.1
 Name: pyscal_rdf
-Version: 0.1.6
+Version: 0.1.7
 Summary: Ontology based structural manipulation and quering
-Author-email: Abril Azocar Guzman <a.azocar.guzman@fz-juelich.de>, Sarath Menon <sarath.menon@pyscal.org>
-Maintainer-email: Sarath Menon <sarath.menon@pyscal.org>
-License: MIT License
-Project-URL: Homepage, https://pyscal.org
-Project-URL: Documentation, https://rdf.pyscal.org
-Project-URL: Repository, https://github.com/pyscal/pyscal_rdf
-Keywords: ontology,research-data-management,rdm,computational-materials-science,atomic-simulation,atomic-structures
+Home-page: https://pyscal.org
+Download-URL: https://github.com/pyscal/pyscal_rdf
+Author: Abril Azocar Guzman, Sarath Menon
+Author-email: sarath.menon@pyscal.org
 Classifier: Programming Language :: Python :: 3
-Requires-Python: <3.12,>=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy
 Requires-Dist: ase
 Requires-Dist: rdflib
 Requires-Dist: pyyaml
 Requires-Dist: graphviz
 Requires-Dist: networkx
 Requires-Dist: ipycytoscape
 Requires-Dist: pyscal3
 Requires-Dist: spglib
+Requires-Dist: pandas
+Requires-Dist: owlready2
 
 # pyscal_rdf
 
 `pyscal_rdf` is a python tool for ontology-based creation, manipulation, and quering of structures. `pyscal_rdf` uses the [Computational Material Sample Ontology (CMSO)](https://github.com/Materials-Data-Science-and-Informatics/cmso-ontology). 
 
 The package is currently under activate development and could be  unstable .
 
@@ -84,9 +82,11 @@
 
 ## Using `pyscal_rdf`
 
 Coming soon..
 
 
 ## Acknowledgements
-
 This work is supported by the [NFDI-Matwerk](https://nfdi-matwerk.de/) consortia.
+
+Funded by the Deutsche Forschungsgemeinschaft (DFG, German Research Foundation) under the National Research Data Infrastructure – NFDI 38/1 – project number 460247524
+
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `pyscal_rdf-0.1.6/tests/test_encoder_and_write.py` & `pyscal_rdf-0.1.7/tests/test_encoder_and_write.py`

 * *Files identical despite different names*

### Comparing `pyscal_rdf-0.1.6/tests/test_graph.py` & `pyscal_rdf-0.1.7/tests/test_graph.py`

 * *Files identical despite different names*

### Comparing `pyscal_rdf-0.1.6/tests/test_structuregraph.py` & `pyscal_rdf-0.1.7/tests/test_structuregraph.py`

 * *Files identical despite different names*

