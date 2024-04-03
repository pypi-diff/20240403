# Comparing `tmp/sqooler-0.6.0.tar.gz` & `tmp/sqooler-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sqooler-0.6.0.tar", max compression
+gzip compressed data, was "sqooler-0.6.1.tar", max compression
```

## Comparing `sqooler-0.6.0.tar` & `sqooler-0.6.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     1211 2024-03-18 17:38:21.370303 sqooler-0.6.0/LICENSE
--rw-r--r--   0        0        0     3928 2024-03-21 16:38:07.651464 sqooler-0.6.0/README.md
--rw-r--r--   0        0        0     1035 2024-03-29 20:59:57.388780 sqooler-0.6.0/pyproject.toml
--rw-r--r--   0        0        0        0 2024-03-18 17:38:21.374962 sqooler-0.6.0/src/sqooler/__init__.py
--rw-r--r--   0        0        0    11986 2024-03-25 19:22:27.714545 sqooler-0.6.0/src/sqooler/schemes.py
--rw-r--r--   0        0        0     8775 2024-03-29 14:08:39.014572 sqooler-0.6.0/src/sqooler/security.py
--rw-r--r--   0        0        0    26841 2024-03-29 13:47:27.129262 sqooler-0.6.0/src/sqooler/spoolers.py
--rw-r--r--   0        0        0        0 2024-03-21 16:38:07.659018 sqooler-0.6.0/src/sqooler/storage_providers/__init__.py
--rw-r--r--   0        0        0    21471 2024-03-29 14:08:39.015790 sqooler-0.6.0/src/sqooler/storage_providers/base.py
--rw-r--r--   0        0        0    26457 2024-03-29 14:08:39.017351 sqooler-0.6.0/src/sqooler/storage_providers/dropbox.py
--rw-r--r--   0        0        0    22695 2024-03-29 14:08:39.018459 sqooler-0.6.0/src/sqooler/storage_providers/local.py
--rw-r--r--   0        0        0    27073 2024-03-29 14:08:39.019764 sqooler-0.6.0/src/sqooler/storage_providers/mongodb.py
--rw-r--r--   0        0        0     5718 2024-03-29 19:21:38.051011 sqooler-0.6.0/src/sqooler/utils.py
--rw-r--r--   0        0        0     4927 1970-01-01 00:00:00.000000 sqooler-0.6.0/PKG-INFO
+-rw-r--r--   0        0        0     1211 2024-03-18 17:38:21.370303 sqooler-0.6.1/LICENSE
+-rw-r--r--   0        0        0     3928 2024-03-21 16:38:07.651464 sqooler-0.6.1/README.md
+-rw-r--r--   0        0        0     1035 2024-04-03 17:36:13.735396 sqooler-0.6.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-03-18 17:38:21.374962 sqooler-0.6.1/src/sqooler/__init__.py
+-rw-r--r--   0        0        0    12140 2024-04-03 16:25:44.628605 sqooler-0.6.1/src/sqooler/schemes.py
+-rw-r--r--   0        0        0     8775 2024-03-29 14:08:39.014572 sqooler-0.6.1/src/sqooler/security.py
+-rw-r--r--   0        0        0    27142 2024-04-03 16:25:44.628916 sqooler-0.6.1/src/sqooler/spoolers.py
+-rw-r--r--   0        0        0        0 2024-03-21 16:38:07.659018 sqooler-0.6.1/src/sqooler/storage_providers/__init__.py
+-rw-r--r--   0        0        0    21471 2024-03-29 14:08:39.015790 sqooler-0.6.1/src/sqooler/storage_providers/base.py
+-rw-r--r--   0        0        0    26457 2024-03-29 14:08:39.017351 sqooler-0.6.1/src/sqooler/storage_providers/dropbox.py
+-rw-r--r--   0        0        0    22695 2024-03-29 14:08:39.018459 sqooler-0.6.1/src/sqooler/storage_providers/local.py
+-rw-r--r--   0        0        0    27073 2024-03-29 14:08:39.019764 sqooler-0.6.1/src/sqooler/storage_providers/mongodb.py
+-rw-r--r--   0        0        0     5718 2024-03-29 19:21:38.051011 sqooler-0.6.1/src/sqooler/utils.py
+-rw-r--r--   0        0        0     4927 1970-01-01 00:00:00.000000 sqooler-0.6.1/PKG-INFO
```

### Comparing `sqooler-0.6.0/LICENSE` & `sqooler-0.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `sqooler-0.6.0/README.md` & `sqooler-0.6.1/README.md`

 * *Files identical despite different names*

### Comparing `sqooler-0.6.0/pyproject.toml` & `sqooler-0.6.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "sqooler"
-version = "0.6.0"
+version = "0.6.1"
 description = "Code that enables validated cloud access to quantum hardware (simulators)"
 authors = ["fretchen <fred.jendrzejewski@gmail.com>"]
 repository = "https://github.com/Alqor-UG/sqooler"
 documentation = "https://alqor-ug.github.io/sqooler"
 license = "Unlicense"
 readme = "README.md"
 packages = [{include = "sqooler", from = "src"}]
```

### Comparing `sqooler-0.6.0/src/sqooler/schemes.py` & `sqooler-0.6.1/src/sqooler/schemes.py`

 * *Files 1% similar despite different names*

```diff
@@ -39,17 +39,17 @@
         description="The full name of the backend including the storage provider.",
         pattern=r"^$|^[a-z0-9]+_[a-z0-9]+_[a-z0-9]+$",
     ),
 ]
 
 # the strings that are allowed for the wire_order
 WireOrderStr = Annotated[
-    Literal["linear", "interleaved"],
+    Literal["sequential", "interleaved"],
     Field(
-        description="The wire order of the backend. Either linear or interleaved."
+        description="The wire order of the backend. Either sequential or interleaved."
         " Non standard qiskit field."
     ),
 ]
 
 
 class StatusMsgDict(BaseModel):
     """
@@ -226,14 +226,18 @@
     The input for the experimental job.
     """
 
     instructions: list[GateDict] = Field(description="The instructions for the job")
     num_wires: int = Field(description="The number of wires for the job")
     shots: int = Field(description="The number of shots for the job")
     wire_order: WireOrderStr
+    seed: Optional[int] = Field(
+        default=None,
+        description="The seed for the random number generator if one might be used",
+    )
 
 
 class DataDict(BaseModel):
     """
     A class that defines the structure of the data within the ExperimentDict.
     """
```

### Comparing `sqooler-0.6.0/src/sqooler/security.py` & `sqooler-0.6.1/src/sqooler/security.py`

 * *Files identical despite different names*

### Comparing `sqooler-0.6.0/src/sqooler/spoolers.py` & `sqooler-0.6.1/src/sqooler/spoolers.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,14 +27,15 @@
     BackendConfigSchemaIn,
     ExperimentDict,
     ExperimentalInputDict,
     ResultDict,
     StatusMsgDict,
     GateDict,
     LabscriptParams,
+    WireOrderStr,
     ColdAtomStr,
     get_init_status,
 )
 
 
 class BaseSpooler(ABC):
     """
@@ -60,15 +61,15 @@
         device_config: Type[BaseModel],
         n_wires: int,
         description: str = "",
         n_max_shots: int = 1000,
         version: str = "0.0.1",
         cold_atom_type: ColdAtomStr = "spin",
         n_max_experiments: int = 15,
-        wire_order: str = "interleaved",
+        wire_order: WireOrderStr = "interleaved",
         num_species: int = 1,
         operational: bool = True,
         sign: bool = False,
     ):
         """
         The constructor of the class.
         """
@@ -331,14 +332,21 @@
         ins_list = [gate_dict_from_list(instr) for instr in raw_ins_list]
         exp_info = ExperimentalInputDict(
             instructions=ins_list,
             shots=json_dict["shots"],
             wire_order=json_dict["wire_order"],
             num_wires=json_dict["num_wires"],
         )
+        exp_info = ExperimentalInputDict(
+            instructions=ins_list,
+            shots=json_dict["shots"],
+            wire_order=json_dict["wire_order"],
+            num_wires=json_dict["num_wires"],
+            seed=json_dict.get("seed", None),
+        )
         return exp_info
 
     def get_private_jwk(self) -> JWK:
         """
         Get the private JWK for the spooler.
 
         Returns:
@@ -447,15 +455,15 @@
         labscript_params: LabscriptParams,
         run: Any,  # it would be really nice to fix this type
         description: str = "",
         n_max_shots: int = 1000,
         version: str = "0.0.1",
         cold_atom_type: ColdAtomStr = "spin",
         n_max_experiments: int = 15,
-        wire_order: str = "interleaved",
+        wire_order: WireOrderStr = "interleaved",
         num_species: int = 1,
         operational: bool = True,
     ):
         """
         The constructor of the class. The  arguments are the same as for the Spooler
         class with two additions.
```

### Comparing `sqooler-0.6.0/src/sqooler/storage_providers/base.py` & `sqooler-0.6.1/src/sqooler/storage_providers/base.py`

 * *Files identical despite different names*

### Comparing `sqooler-0.6.0/src/sqooler/storage_providers/dropbox.py` & `sqooler-0.6.1/src/sqooler/storage_providers/dropbox.py`

 * *Files identical despite different names*

### Comparing `sqooler-0.6.0/src/sqooler/storage_providers/local.py` & `sqooler-0.6.1/src/sqooler/storage_providers/local.py`

 * *Files identical despite different names*

### Comparing `sqooler-0.6.0/src/sqooler/storage_providers/mongodb.py` & `sqooler-0.6.1/src/sqooler/storage_providers/mongodb.py`

 * *Files identical despite different names*

### Comparing `sqooler-0.6.0/src/sqooler/utils.py` & `sqooler-0.6.1/src/sqooler/utils.py`

 * *Files identical despite different names*

### Comparing `sqooler-0.6.0/PKG-INFO` & `sqooler-0.6.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sqooler
-Version: 0.6.0
+Version: 0.6.1
 Summary: Code that enables validated cloud access to quantum hardware (simulators)
 Home-page: https://github.com/Alqor-UG/sqooler
 License: Unlicense
 Keywords: pydantic,quantum-hardware,sdk-python
 Author: fretchen
 Author-email: fred.jendrzejewski@gmail.com
 Requires-Python: >=3.10,<4.0
```

