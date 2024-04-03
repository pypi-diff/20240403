# Comparing `tmp/syndb_constants-0.9.3.tar.gz` & `tmp/syndb_constants-0.9.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "syndb_constants-0.9.3.tar", max compression
+gzip compressed data, was "syndb_constants-0.9.4.tar", max compression
```

## Comparing `syndb_constants-0.9.3.tar` & `syndb_constants-0.9.4.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0        0 2024-01-02 09:32:58.074130 syndb_constants-0.9.3/README.md
--rw-r--r--   0        0        0      527 2024-01-02 20:59:39.645825 syndb_constants-0.9.3/pyproject.toml
--rw-r--r--   0        0        0        0 2024-01-02 09:32:58.074130 syndb_constants-0.9.3/syndb_constants/__init__.py
--rw-r--r--   0        0        0       70 2024-01-02 09:32:58.690787 syndb_constants-0.9.3/syndb_constants/api.py
--rw-r--r--   0        0        0     2192 2024-01-02 20:59:34.662656 syndb_constants-0.9.3/syndb_constants/dataset.py
--rw-r--r--   0        0        0     2362 2024-01-02 09:32:58.697454 syndb_constants-0.9.3/syndb_constants/table.py
--rw-r--r--   0        0        0      476 1970-01-01 00:00:00.000000 syndb_constants-0.9.3/PKG-INFO
+-rw-r--r--   0        0        0        0 2024-01-02 09:32:58.074130 syndb_constants-0.9.4/README.md
+-rw-r--r--   0        0        0      527 2024-01-04 17:42:21.702320 syndb_constants-0.9.4/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-01-02 09:32:58.074130 syndb_constants-0.9.4/syndb_constants/__init__.py
+-rw-r--r--   0        0        0       70 2024-01-02 09:32:58.690787 syndb_constants-0.9.4/syndb_constants/api.py
+-rw-r--r--   0        0        0     2192 2024-01-02 20:59:34.662656 syndb_constants-0.9.4/syndb_constants/dataset.py
+-rw-r--r--   0        0        0     2359 2024-01-04 17:41:38.370048 syndb_constants-0.9.4/syndb_constants/table.py
+-rw-r--r--   0        0        0      476 1970-01-01 00:00:00.000000 syndb_constants-0.9.4/PKG-INFO
```

### Comparing `syndb_constants-0.9.3/pyproject.toml` & `syndb_constants-0.9.4/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "syndb-constants"
-version = "0.9.3"
+version = "0.9.4"
 description = "Constants used with SynDB in Python"
 authors = ["caniko <git@rotas.mozmail.com>"]
 readme = "README.md"
 packages = [{include = "syndb_constants"}]
 
 [tool.poetry.dependencies]
 python = ">=3.9,<4.0"
```

### Comparing `syndb_constants-0.9.3/syndb_constants/dataset.py` & `syndb_constants-0.9.4/syndb_constants/dataset.py`

 * *Files identical despite different names*

### Comparing `syndb_constants-0.9.3/syndb_constants/table.py` & `syndb_constants-0.9.4/syndb_constants/table.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 
 SyndbTableNames = Literal[
     "neuron",
     "dendrite",
     "axon",
     "pre_synaptic_terminal",
-    "terminal",
+    "synapse",
     "dendritic_spine",
     "endoplasmic_reticulum",
     "nucleus",
     "vesicle",
     "mitochondria",
 ]
 
@@ -25,15 +25,15 @@
     # Neuro data hierarchy ==================
     NEURON = auto()
 
     # Neurites
     DENDRITE = auto()
     AXON = auto()
     PRE_SYNAPTIC_TERMINAL = auto()
-    TERMINAL = auto()
+    SYNAPSE = auto()
     DENDRITIC_SPINE = auto()
 
     # Cellular structures
     ENDOPLASMIC_RETICULUM = auto()
     NUCLEUS = auto()
 
     # Smaller organelles
@@ -48,15 +48,15 @@
 
 table_name_to_syndb_table = {n: s for s, n in syndb_table_to_table_name.items()}
 
 
 COMPARTMENT_HIERARCHY: list[tuple[SyndbTable, ...]] = [
     (SyndbTable.NEURON,),
     (SyndbTable.DENDRITE, SyndbTable.AXON),
-    (SyndbTable.PRE_SYNAPTIC_TERMINAL, SyndbTable.TERMINAL, SyndbTable.DENDRITIC_SPINE),
+    (SyndbTable.PRE_SYNAPTIC_TERMINAL, SyndbTable.SYNAPSE, SyndbTable.DENDRITIC_SPINE),
     (
         SyndbTable.MITOCHONDRIA,
         SyndbTable.ENDOPLASMIC_RETICULUM,
         SyndbTable.NUCLEUS,
         SyndbTable.VESICLE,
     ),
 ]
```

