# Comparing `tmp/reasoner_validator-3.9.5.tar.gz` & `tmp/reasoner_validator-4.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "reasoner_validator-3.9.5.tar", max compression
+gzip compressed data, was "reasoner_validator-4.0.0.tar", max compression
```

## Comparing `reasoner_validator-3.9.5.tar` & `reasoner_validator-4.0.0.tar`

### file list

```diff
@@ -1,41 +1,41 @@
--rw-r--r--   0        0        0     1153 2024-01-10 03:36:02.754353 reasoner_validator-3.9.5/LICENSE
--rw-r--r--   0        0        0    13732 2024-01-10 03:36:02.754353 reasoner_validator-3.9.5/README.md
--rw-r--r--   0        0        0      131 2024-01-10 03:36:02.754353 reasoner_validator-3.9.5/docs/.nojekyll
--rw-r--r--   0        0        0      634 2024-01-10 03:36:02.754353 reasoner_validator-3.9.5/docs/Makefile
--rw-r--r--   0        0        0     2291 2024-01-10 03:36:02.758353 reasoner_validator-3.9.5/docs/conf.py
--rw-r--r--   0        0        0    20365 2024-01-10 03:36:02.758353 reasoner_validator-3.9.5/docs/index.rst
--rw-r--r--   0        0        0      795 2024-01-10 03:36:02.758353 reasoner_validator-3.9.5/docs/make.bat
--rw-r--r--   0        0        0      136 2024-01-10 03:36:02.758353 reasoner_validator-3.9.5/docs/reasoner_validator.biolink.rst
--rw-r--r--   0        0        0      135 2024-01-10 03:36:02.758353 reasoner_validator-3.9.5/docs/reasoner_validator.report.rst
--rw-r--r--   0        0        0      152 2024-01-10 03:36:02.758353 reasoner_validator-3.9.5/docs/reasoner_validator.rst
--rw-r--r--   0        0        0      146 2024-01-10 03:36:02.758353 reasoner_validator-3.9.5/docs/reasoner_validator.trapi.mapping.rst
--rw-r--r--   0        0        0      144 2024-01-10 03:36:02.758353 reasoner_validator-3.9.5/docs/reasoner_validator.trapi.rst
--rw-r--r--   0        0        0      163 2024-01-10 03:36:02.758353 reasoner_validator-3.9.5/docs/reasoner_validator.validation_codes.rst
--rw-r--r--   0        0        0      157 2024-01-10 03:36:02.758353 reasoner_validator-3.9.5/docs/reasoner_validator.versioning.rst
--rw-r--r--   0        0        0    39260 2024-01-10 03:36:02.758353 reasoner_validator-3.9.5/docs/validation_codes_dictionary.md
--rw-r--r--   0        0        0     2888 2024-01-10 03:36:02.758353 reasoner_validator-3.9.5/pyproject.toml
--rw-r--r--   0        0        0        0 2024-01-10 03:36:02.758353 reasoner_validator-3.9.5/reasoner_validator/__init__.py
--rw-r--r--   0        0        0    85545 2024-01-10 03:36:02.758353 reasoner_validator-3.9.5/reasoner_validator/biolink/__init__.py
--rw-r--r--   0        0        0    42793 2024-01-10 03:36:02.758353 reasoner_validator-3.9.5/reasoner_validator/codes.yaml
--rw-r--r--   0        0        0     1761 2024-01-10 03:36:02.758353 reasoner_validator-3.9.5/reasoner_validator/github.py
--rw-r--r--   0        0        0     3382 2024-01-10 03:36:02.758353 reasoner_validator-3.9.5/reasoner_validator/message.py
--rw-r--r--   0        0        0    27692 2024-01-10 03:36:02.758353 reasoner_validator-3.9.5/reasoner_validator/report.py
--rw-r--r--   0        0        0        0 2024-01-10 03:36:02.758353 reasoner_validator-3.9.5/reasoner_validator/sri/__init__.py
--rw-r--r--   0        0        0     4754 2024-01-10 03:36:02.758353 reasoner_validator-3.9.5/reasoner_validator/sri/util.py
--rw-r--r--   0        0        0    13890 2024-01-10 03:36:02.758353 reasoner_validator-3.9.5/reasoner_validator/trapi/__init__.py
--rw-r--r--   0        0        0     1112 2024-01-10 03:36:02.758353 reasoner_validator-3.9.5/reasoner_validator/trapi/mapping.py
--rw-r--r--   0        0        0    14636 2024-01-10 03:36:02.758353 reasoner_validator-3.9.5/reasoner_validator/validation_codes.py
--rw-r--r--   0        0        0    35157 2024-01-10 03:36:02.758353 reasoner_validator-3.9.5/reasoner_validator/validator.py
--rw-r--r--   0        0        0    11943 2024-01-10 03:36:02.758353 reasoner_validator-3.9.5/reasoner_validator/versioning.py
--rw-r--r--   0        0        0      501 2024-01-10 03:36:02.758353 reasoner_validator-3.9.5/reasoner_validator/versions.yaml
--rw-r--r--   0        0        0     2407 2024-01-10 03:36:02.762353 reasoner_validator-3.9.5/tests/__init__.py
--rw-r--r--   0        0        0        0 2024-01-10 03:36:02.762353 reasoner_validator-3.9.5/tests/conftest.py
--rw-r--r--   0        0        0   137871 2024-01-10 03:36:02.762353 reasoner_validator-3.9.5/tests/test_biolink_compliance_validation.py
--rw-r--r--   0        0        0    62107 2024-01-10 03:36:02.762353 reasoner_validator-3.9.5/tests/test_data/patched_trapi_schema_v1.4.0-beta5.yaml
--rw-r--r--   0        0        0    38215 2024-01-10 03:36:02.762353 reasoner_validator-3.9.5/tests/test_response_validator.py
--rw-r--r--   0        0        0     6157 2024-01-10 03:36:02.762353 reasoner_validator-3.9.5/tests/test_semver.py
--rw-r--r--   0        0        0     2248 2024-01-10 03:36:02.762353 reasoner_validator-3.9.5/tests/test_trapi_versioning.py
--rw-r--r--   0        0        0    27128 2024-01-10 03:36:02.762353 reasoner_validator-3.9.5/tests/test_validate.py
--rw-r--r--   0        0        0    21977 2024-01-10 03:36:02.762353 reasoner_validator-3.9.5/tests/test_validation_report.py
--rw-r--r--   0        0        0     2734 2024-01-10 03:36:02.762353 reasoner_validator-3.9.5/tests/test_workflows.py
--rw-r--r--   0        0        0    16067 1970-01-01 00:00:00.000000 reasoner_validator-3.9.5/PKG-INFO
+-rw-r--r--   0        0        0     1153 2024-04-03 01:08:55.981091 reasoner_validator-4.0.0/LICENSE
+-rw-r--r--   0        0        0    13503 2024-04-03 01:08:55.981091 reasoner_validator-4.0.0/README.md
+-rw-r--r--   0        0        0      131 2024-04-03 01:08:55.981091 reasoner_validator-4.0.0/docs/.nojekyll
+-rw-r--r--   0        0        0      634 2024-04-03 01:08:55.981091 reasoner_validator-4.0.0/docs/Makefile
+-rw-r--r--   0        0        0     2291 2024-04-03 01:08:55.981091 reasoner_validator-4.0.0/docs/conf.py
+-rw-r--r--   0        0        0    20365 2024-04-03 01:08:55.981091 reasoner_validator-4.0.0/docs/index.rst
+-rw-r--r--   0        0        0      795 2024-04-03 01:08:55.981091 reasoner_validator-4.0.0/docs/make.bat
+-rw-r--r--   0        0        0      136 2024-04-03 01:08:55.981091 reasoner_validator-4.0.0/docs/reasoner_validator.biolink.rst
+-rw-r--r--   0        0        0      135 2024-04-03 01:08:55.981091 reasoner_validator-4.0.0/docs/reasoner_validator.report.rst
+-rw-r--r--   0        0        0      152 2024-04-03 01:08:55.981091 reasoner_validator-4.0.0/docs/reasoner_validator.rst
+-rw-r--r--   0        0        0      146 2024-04-03 01:08:55.981091 reasoner_validator-4.0.0/docs/reasoner_validator.trapi.mapping.rst
+-rw-r--r--   0        0        0      144 2024-04-03 01:08:55.981091 reasoner_validator-4.0.0/docs/reasoner_validator.trapi.rst
+-rw-r--r--   0        0        0      163 2024-04-03 01:08:55.981091 reasoner_validator-4.0.0/docs/reasoner_validator.validation_codes.rst
+-rw-r--r--   0        0        0      157 2024-04-03 01:08:55.981091 reasoner_validator-4.0.0/docs/reasoner_validator.versioning.rst
+-rw-r--r--   0        0        0    39468 2024-04-03 01:08:55.981091 reasoner_validator-4.0.0/docs/validation_codes_dictionary.md
+-rw-r--r--   0        0        0     2888 2024-04-03 01:08:55.981091 reasoner_validator-4.0.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-03 01:08:55.981091 reasoner_validator-4.0.0/reasoner_validator/__init__.py
+-rw-r--r--   0        0        0    85875 2024-04-03 01:08:55.985091 reasoner_validator-4.0.0/reasoner_validator/biolink/__init__.py
+-rw-r--r--   0        0        0    43025 2024-04-03 01:08:55.985091 reasoner_validator-4.0.0/reasoner_validator/codes.yaml
+-rw-r--r--   0        0        0     1761 2024-04-03 01:08:55.985091 reasoner_validator-4.0.0/reasoner_validator/github.py
+-rw-r--r--   0        0        0     3973 2024-04-03 01:08:55.985091 reasoner_validator-4.0.0/reasoner_validator/message.py
+-rw-r--r--   0        0        0    46755 2024-04-03 01:08:55.985091 reasoner_validator-4.0.0/reasoner_validator/report.py
+-rw-r--r--   0        0        0        0 2024-04-03 01:08:55.985091 reasoner_validator-4.0.0/reasoner_validator/sri/__init__.py
+-rw-r--r--   0        0        0     4754 2024-04-03 01:08:55.985091 reasoner_validator-4.0.0/reasoner_validator/sri/util.py
+-rw-r--r--   0        0        0    14288 2024-04-03 01:08:55.985091 reasoner_validator-4.0.0/reasoner_validator/trapi/__init__.py
+-rw-r--r--   0        0        0     1120 2024-04-03 01:08:55.985091 reasoner_validator-4.0.0/reasoner_validator/trapi/mapping.py
+-rw-r--r--   0        0        0    14745 2024-04-03 01:08:55.985091 reasoner_validator-4.0.0/reasoner_validator/validation_codes.py
+-rw-r--r--   0        0        0    35564 2024-04-03 01:08:55.985091 reasoner_validator-4.0.0/reasoner_validator/validator.py
+-rw-r--r--   0        0        0    11943 2024-04-03 01:08:55.985091 reasoner_validator-4.0.0/reasoner_validator/versioning.py
+-rw-r--r--   0        0        0      838 2024-04-03 01:08:55.985091 reasoner_validator-4.0.0/reasoner_validator/versions.yaml
+-rw-r--r--   0        0        0     2407 2024-04-03 01:08:55.985091 reasoner_validator-4.0.0/tests/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-03 01:08:55.985091 reasoner_validator-4.0.0/tests/conftest.py
+-rw-r--r--   0        0        0   138310 2024-04-03 01:08:55.985091 reasoner_validator-4.0.0/tests/test_biolink_compliance_validation.py
+-rw-r--r--   0        0        0    62107 2024-04-03 01:08:55.985091 reasoner_validator-4.0.0/tests/test_data/patched_trapi_schema_v1.4.0-beta5.yaml
+-rw-r--r--   0        0        0    41247 2024-04-03 01:08:55.985091 reasoner_validator-4.0.0/tests/test_response_validator.py
+-rw-r--r--   0        0        0     6157 2024-04-03 01:08:55.985091 reasoner_validator-4.0.0/tests/test_semver.py
+-rw-r--r--   0        0        0     2248 2024-04-03 01:08:55.985091 reasoner_validator-4.0.0/tests/test_trapi_versioning.py
+-rw-r--r--   0        0        0    27195 2024-04-03 01:08:55.985091 reasoner_validator-4.0.0/tests/test_validate.py
+-rw-r--r--   0        0        0    30223 2024-04-03 01:08:55.985091 reasoner_validator-4.0.0/tests/test_validation_report.py
+-rw-r--r--   0        0        0     2734 2024-04-03 01:08:55.989091 reasoner_validator-4.0.0/tests/test_workflows.py
+-rw-r--r--   0        0        0    15838 1970-01-01 00:00:00.000000 reasoner_validator-4.0.0/PKG-INFO
```

### Comparing `reasoner_validator-3.9.5/LICENSE` & `reasoner_validator-4.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `reasoner_validator-3.9.5/README.md` & `reasoner_validator-4.0.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -49,15 +49,15 @@
 poetry install --all-extras
 ```
 
 ## Running Validation against an ARS UUID Result(*) or using a Local TRAPI Request Query
 
 A local script **`trapi_validator.py`** is available to run TRAPI Response validation against either a PK (UUID)
 indexed query result of the Biomedical Knowledge Translator "Autonomous Relay System" (ARS), a local JSON Response
-text file or a locally triggered _ad hoc_ query Request against an directly specified TRAPI endpoint.
+text file or a locally triggered _ad hoc_ query Request against a directly specified TRAPI endpoint.
 
 Note that it is best run within a **`poetry shell`** created by **`poetry install`**.
 
 For script usage, type:
 
 ```bash
 ./trapi_validator.py --help
@@ -180,16 +180,16 @@
 
 ### Typical Output
 
 As an example of the kind of output to expect, if one posts the following TRAPI Response JSON data structure to the **/validate** endpoint:
 
 ```json
 {
-  "trapi_version": "1.4.1",
-  "biolink_version": "3.5.0",
+  "trapi_version": "1.4.2",
+  "biolink_version": "4.1.5",
   "response": {
       "message": {
         "query_graph": {
             "nodes": {
                 "type-2 diabetes": {"ids": ["MONDO:0005148"]},
                 "drug": {"categories": ["biolink:Drug"]}
             },
@@ -223,55 +223,59 @@
 }
 ```
 
 one should typically get a response body something like the following JSON validation result back:
 
 ```json
 {
-  "trapi_version": "1.4.1",
-  "biolink_version": "3.2.1",
   "messages": {
-    "_comment": "some categories of messages may be absent, hence, empty dictionaries",
-    "critical": {},
-    "errors": {
-      "error.knowledge_graph.node.category.missing": {
-          "_comment": "source scope of the validation error ('global' or some knowledge source path string)",
-          "global": {
-              "_comment": "this message template does not have any additional parameters other than identifier hence it just has the unique identifier  value as a dictionary key, with associated value None",
-               "MONDO:0005148": null            
+    "Validate TRAPI Response": {
+      "Standards Test": {
+        "info": {
+          "info.query_graph.edge.predicate.mixin": {
+            "global": {
+              "biolink:treats": [
+                {
+                  "edge_id": "drug[biolink:Drug]--['biolink:treats']->type-2 diabetes[None]"
+                }
+              ]
+            }
           }
-        }
-    },
-    "warnings": {
-      "_comment": "validation code",
-      "warning.knowledge_graph.node.unmapped_prefix": {
-          "global": {
-              "_comment": "template identifier field value",
-              "CHEBI:6801": [  
-                  {
-                    "_comment": "additional message template field values, if applicable",
-                    "categories": "['biolink:Drug']"  
-                  }
-              ]       
+        },
+        "skipped": {},
+        "warning": {},
+        "error": {
+          "error.query_graph.edge.predicate.invalid": {
+            "global": {
+              "biolink:treats": [
+                {
+                  "edge_id": "drug[biolink:Drug]--['biolink:treats']->type-2 diabetes[None]"
+                }
+              ]
+            }
           }
-
-        }
-    },
-    "information": {},
-  }
+        },
+        "critical": {}
+      }
+    }
+  },
+  "trapi_version": "v1.4.2",
+  "biolink_version": "4.1.5"
 }
 ```
 
 To minimize redundancy in validation messages, messages are uniquely indexed in dictionaries at two levels:
 
 1. the (codes.yaml recorded) dot-delimited validation code path string
 2. for messages with templated parameters, by a mandatory 'identifier' field (which is expected to exist as a field in a template if such template has one or more parameterized fields)
 
 ### OpenTelemetry and Jaeger
 
+NOTE: OpenTelemetry is temporarily disabled in this code release (to be updated later)
+
 The web service may be monitored for OpenTelemetry by setting an environment variable **TELEMETRY_ENDPOINT**  to a suitable trace collecting endpoint in an application like [Jaeger](https://www.jaegertracing.io/) (see also the [Translator SRI Jaeger-Demo](https://github.com/TranslatorSRI/Jaeger-demo)).
 
 **Note:** the current system Docker (Compose) design only supports OpenTemplate tracing using the internal Jaeger container and may require further refinements to enable use of an external telemetry collector.
 
 ### Running the Web Service within Docker
 
 The Reasoner Validator web service may be run inside a docker container, using Docker Compose.
```

### Comparing `reasoner_validator-3.9.5/docs/Makefile` & `reasoner_validator-4.0.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `reasoner_validator-3.9.5/docs/conf.py` & `reasoner_validator-4.0.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `reasoner_validator-3.9.5/docs/index.rst` & `reasoner_validator-4.0.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `reasoner_validator-3.9.5/docs/make.bat` & `reasoner_validator-4.0.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `reasoner_validator-3.9.5/docs/validation_codes_dictionary.md` & `reasoner_validator-4.0.0/docs/validation_codes_dictionary.md`

 * *Files 2% similar despite different names*

```diff
@@ -1142,7 +1142,17 @@
 
 **Message:** Edge has an 'mixin' attribute_type_id
 
 **Context:** edge_id, identifier
 
 **Description:** TRAPI Messages in Knowledge Graphs can have 'mixin' attribute type identifiers, when the mode of validation is 'non-strict'.
 
+## Skipped Test
+
+### skipped.test
+
+**Message:** For reason indicated in the identifier
+
+**Context:** identifier
+
+**Description:** Test was skipped for the reason documented in the 'identifier' string value.
+
```

### Comparing `reasoner_validator-3.9.5/pyproject.toml` & `reasoner_validator-4.0.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "reasoner-validator"
-version = "3.9.5"
+version = "4.0.0"
 description = "Validation tools for Reasoner API"
 authors = [
     "Richard Bruskiewich <richard.bruskiewich@delphinai.com>",
     "Patrick Wang <patrickelvin@gmail.com>"
 ]
 maintainers = [
     "Richard Bruskiewich <richard.bruskiewich@delphinai.com>",
```

### Comparing `reasoner_validator-3.9.5/reasoner_validator/biolink/__init__.py` & `reasoner_validator-4.0.0/reasoner_validator/biolink/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -87,15 +87,15 @@
             if biolink_version is None:
                 self.default_biolink = True
             self.bmt = get_biolink_model_toolkit(biolink_version=biolink_version)
             self.biolink_version = self.bmt.get_model_version()
         else:
             self.biolink_version = "suppress"
 
-        logger.info(f"Resolved Biolink Model Version: '{self.biolink_version}'")
+        logger.debug(f"Resolved Biolink Model Version: '{self.biolink_version}'")
 
     def get_biolink_version(self) -> str:
         """
         :return: Biolink Model version currently targeted by the ValidationReporter.
         :rtype biolink_version: str
         """
         return self.biolink_version
@@ -150,37 +150,40 @@
 
 class BiolinkValidator(TRAPISchemaValidator, BMTWrapper):
     """
     Wrapper class for Biolink Model validation of a TRAPI message.
     """
     def __init__(
         self,
-        prefix: Optional[str] = None,
+        default_test: Optional[str] = None,
+        default_target: Optional[str] = None,
         trapi_version: Optional[str] = None,
         biolink_version: Optional[str] = None,
         target_provenance: Optional[Dict[str, str]] = None,
         strict_validation: Optional[bool] = None
     ):
         """
         Biolink Validator constructor.
-
-        :param prefix: named context of the BiolinkValidator, used as a prefix in validation messages.
+        :param default_test: Optional[str] =  None, initial default test context of the BiolinkValidator messages
+        :param default_target: Optional[str] =  None, initial default target context of the BiolinkValidator,
+                                                also used as a prefix in validation messages.
         :param trapi_version:  Optional[str], caller specified Biolink Model version (default: None, use TRAPI 'latest')
         :param biolink_version: Optional[str], caller specified Biolink Model version (default: None, use BMT 'latest')
                                 Note that a special biolink_version value string "suppress" disables full Biolink Model
                                 validation by the validator (i.e. limits validation to superficial validation).
         :param target_provenance: Optional[Dict[str,str]], Dictionary of context ARA and KP for provenance validation
         :param strict_validation: Optional[bool] = None, if True, some tests validate as 'error';  False, simply issues
                                   'info' message; A value of 'None' uses the default value for specific graph contexts.
 
         """
         BMTWrapper.__init__(self, biolink_version=biolink_version)
         TRAPISchemaValidator.__init__(
             self,
-            prefix=prefix if prefix else f"Biolink Validation",
+            default_test=default_test,
+            default_target=default_target if default_target else f"Biolink Validation",
             trapi_version=trapi_version,
             strict_validation=strict_validation
         )
         self.target_provenance: Optional[Dict] = target_provenance
 
         # the internal 'nodes' dictionary, indexed by 'node_id' key, tracks
         # the associated Biolink Model node categories, plus a usage count for the node_id key
```

### Comparing `reasoner_validator-3.9.5/reasoner_validator/codes.yaml` & `reasoner_validator-4.0.0/reasoner_validator/codes.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 #############################
 # Reasoner Validator        #
 # Message Codes             #
 #   - critical (errors)     #
 #   - error(s)              #
 #   - warning(s)            #
+#   - skipped (tests)       #
 #   - info(rmation)         #
 #############################
 critical:
   trapi:
     validation:
       $message: "Schema validation error"
       $context:
@@ -904,7 +905,13 @@
             $description: "TRAPI Messages in Knowledge Graphs can have 'abstract' attribute type identifiers, when the mode of validation is 'non-strict'."
           mixin:
             $message: "Edge has an 'mixin' attribute_type_id"
             $context:
               - edge_id
               - identifier
             $description: "TRAPI Messages in Knowledge Graphs can have 'mixin' attribute type identifiers, when the mode of validation is 'non-strict'."
+skipped:
+  test:
+    $message: "For reason indicated in the identifier"
+    $context:
+      - identifier
+    $description: "Test was skipped for the reason documented in the 'identifier' string value."
```

### Comparing `reasoner_validator-3.9.5/reasoner_validator/github.py` & `reasoner_validator-4.0.0/reasoner_validator/github.py`

 * *Files identical despite different names*

### Comparing `reasoner_validator-3.9.5/reasoner_validator/message.py` & `reasoner_validator-4.0.0/reasoner_validator/message.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """
 This module provides standalone global reasoner-validator validation Message types
 to avoid load order conflicts for other modules using these data types.
 """
+from enum import Enum
 from typing import Optional, List, Dict
 #
 # The MESSAGE_CATALOG data structure is something like the following:
 #
 #  {
 #    # message 'type'
 #     "information": {
@@ -38,15 +39,14 @@
 #     },
 #     "critical": {
 #       ...<similar to information data structure above>
 #     }
 # }
 #
 
-
 # One instance of 'MESSAGE_PARAMETERS' is a dictionary of string
 # parameters associated with a  given message code, as documented
 # within the global 'codes.yaml' validation message catalog
 MESSAGE_PARAMETERS = Dict[str, str]
 
 # An 'IDENTIFIED_MESSAGES' data structure is a dictionary of Lists
 # parameterized messages, indexed by a unique 'identifier' discriminator
@@ -63,27 +63,53 @@
 # particular coded message and resolved as to knowledge source. The scope may be 'global' or
 # defined by a 'source trail' of knowledge source specified by infores,
 # from a biolink:primary_knowledge_source up to a topmost biolink:aggregator_knowledge_source
 # retrieving the given knowledge assertion (Subject-Predicate-Object statement with evidence).
 SCOPED_MESSAGES = Dict[
     str,  # 'source trail' origin of affected edge or 'global' validation error
 
-    # (A given message code may have no IDENTIFIED_MESSAGES with discriminating identifier
-    #  and parameters hence,it may have a scoped value of 'None')
+    # (A given message code may have
+    # no IDENTIFIED_MESSAGES with discriminating identifier
+    #  and parameters hence, it may have a scoped value of 'None')
     Optional[IDENTIFIED_MESSAGES]
 ]
 
 # A 'MESSAGE_PARTITION' is a dictionary of coded messages,
 # indexed by validation code and corresponding to one of the
 # four major categories of validation messages:
 # critical/errors/warnings/information
 MESSAGE_PARTITION = Dict[
     str,  # message 'code' as indexing key
     SCOPED_MESSAGES
 ]
 
-# A MESSAGE_CATALOG contains the validation messages from all four
-# major categories of validation: critical/errors/warnings/information
+
+class MessageType(Enum):
+    info = "information"
+    skipped = "skipped tests"
+    warning = "warnings"
+    error = "errors"
+    critical = "critical errors"
+
+
+# A individual MESSAGE_CATALOG contains
+# the validation messages from
+# all four major categories of validation:
+# critical/errors/warnings/information
 MESSAGE_CATALOG = Dict[
-    str,  # message type (critical/errors/warnings/information)
+    str,  # message type (info/skipped/warning/error/critical)
     MESSAGE_PARTITION
 ]
+
+# MESSAGES_BY_TEST contains MESSAGE_CATALOG
+# entries indexed by individual tests
+MESSAGES_BY_TEST = Dict[
+    str,  # unique identifiers for each test
+    MESSAGE_CATALOG
+]
+
+# MESSAGES_BY_TARGET contains MESSAGES_BY_TEST entries
+# indexed by target: endpoint URL, URI or CURIE
+MESSAGES_BY_TARGET = Dict[
+    str,  # target identifier: endpoint URL, URI or CURIE
+    MESSAGES_BY_TEST
+]
```

### Comparing `reasoner_validator-3.9.5/reasoner_validator/report.py` & `reasoner_validator-4.0.0/tests/test_validation_report.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,616 +1,855 @@
-"""Error and Warning Reporting Module"""
-from enum import Enum
-from typing import Optional, Dict, List
-from sys import stdout
-from importlib import metadata
-from io import StringIO
+"""Testing Validation Report methods"""
 import copy
+import sys
+from typing import Optional, Dict, List
+from sys import stderr
 
-from json import dumps, JSONEncoder
+import pytest
 
 from reasoner_validator.message import (
-    MESSAGE_CATALOG,
-    MESSAGE_PARTITION,
-    SCOPED_MESSAGES,
+    MessageType,
     IDENTIFIED_MESSAGES,
-    MESSAGE_PARAMETERS
+    SCOPED_MESSAGES,
+    MESSAGE_PARTITION,
+    MESSAGE_CATALOG,
+    MESSAGES_BY_TEST,
+    MESSAGES_BY_TARGET
 )
+from reasoner_validator.report import ValidationReporter, TRAPIGraphType
 from reasoner_validator.validation_codes import CodeDictionary
+from reasoner_validator.versioning import get_latest_version
 
-import logging
-logger = logging.getLogger(__name__)
+TEST_TRAPI_VERSION = get_latest_version(ValidationReporter.DEFAULT_TRAPI_VERSION)
 
 
-class ReportJsonEncoder(JSONEncoder):
-    def default(self, o):
-        try:
-            iterable = iter(o)
-        except TypeError:
-            pass
+def check_messages(
+        validator: ValidationReporter,
+        code: str,
+        no_errors: bool = False,
+        source_trail: Optional[str] = None
+):
+    # TODO: only assume 'default' test and target for now (fix later if problematic)
+    messages: MESSAGES_BY_TARGET = validator.get_all_messages()
+    if code:
+        assert CodeDictionary.get_code_entry(code) is not None, f"check_messages() unknown code: '{code}'"
+        message_type: MessageType = validator.get_message_type(code)
+        coded_messages: MESSAGE_PARTITION = validator.get_messages_of_type(message_type)
+        assert any([message_code == code for message_code in coded_messages.keys()])
+        if source_trail:
+            source_trail_tags = coded_messages[code].keys()
+            assert source_trail in source_trail_tags
+            if source_trail != "global":
+                assert "global" not in source_trail_tags
+    else:
+        if no_errors:
+            # just don't want any error (including 'critical'); 'info', 'skipped' and 'warning' are ok?
+            assert not validator.has_critical(), f"Unexpected critical error messages seen {messages}"
+            assert not validator.has_errors(), f"Unexpected error messages seen {messages}"
         else:
-            return list(iterable)
-        # Let the base class default method raise the TypeError
-        return JSONEncoder.default(self, o)
+            # no expected at all? Assert the absence of such messages?
+            assert not validator.has_messages(), f"Unexpected messages seen {messages}"
 
 
-def _output(json, flat=False):
-    return dumps(json, cls=ReportJsonEncoder, sort_keys=False, indent=None if flat else 4)
+def test_graph_type_label():
+    assert TRAPIGraphType.Input_Edge.label() == "input_edge"
+    assert TRAPIGraphType.Query_Graph.label() == "query_graph"
+    assert TRAPIGraphType.Knowledge_Graph.label() == "knowledge_graph"
+
+
+def test_check_basic_get_code_subtree():
+    assert CodeDictionary.get_code_subtree("") is None
+    assert CodeDictionary.get_code_subtree("info") is not None
+    assert CodeDictionary.get_code_subtree("skipped") is not None
+    assert CodeDictionary.get_code_subtree("warning") is not None
+    assert CodeDictionary.get_code_subtree("error") is not None
+    assert CodeDictionary.get_code_subtree("critical") is not None
+    assert CodeDictionary.get_code_subtree("foo.bar") is None
+
+
+def test_get_code_subtree_is_leaf():
+
+    result = CodeDictionary.get_code_subtree("info.compliant", is_leaf=True)
+    assert result is not None
+    message_type, leaf = result
+    assert leaf is not None
+    assert isinstance(leaf, Dict)
+    assert all([key in [CodeDictionary.MESSAGE, CodeDictionary.DESCRIPTION] for key in leaf])
+    assert leaf[CodeDictionary.MESSAGE] == "Biolink Model-compliant TRAPI Message"
+    assert leaf[CodeDictionary.DESCRIPTION].startswith("Specified TRAPI message completely satisfies")
+
+    assert CodeDictionary.get_code_subtree("info.compliant", is_leaf=False) is None
+
+
+def test_get_code_subtree_facet_message():
+
+    result = CodeDictionary.get_code_subtree("info.compliant", facet="message", is_leaf=True)
+    assert result is not None
+    message_type, leaf = result
+    assert leaf is not None
+    assert isinstance(leaf, Dict)
+    assert CodeDictionary.MESSAGE in leaf
+    assert leaf[CodeDictionary.MESSAGE] == "Biolink Model-compliant TRAPI Message"
+    assert CodeDictionary.DESCRIPTION not in leaf
+
+    result = CodeDictionary.get_code_subtree("info.input_edge.predicate", facet="message")
+    assert result is not None
+    message_type, subtree = result
+    assert subtree is not None
+    assert isinstance(subtree, Dict)
+    assert all([key in ["abstract", "mixin"] for key in subtree])
+    assert CodeDictionary.MESSAGE in subtree["abstract"]
+    assert subtree["abstract"][CodeDictionary.MESSAGE] == "Edge has an 'abstract' predicate"
+    assert CodeDictionary.DESCRIPTION not in subtree["abstract"]
+
+
+def test_get_code_subtree_facet_description():
+
+    result = CodeDictionary.get_code_subtree("info.compliant", facet="description", is_leaf=True)
+    assert result is not None
+    message_type, leaf = result
+    assert leaf is not None
+    assert isinstance(leaf, Dict)
+    assert CodeDictionary.DESCRIPTION in leaf
+    assert leaf[CodeDictionary.DESCRIPTION].startswith("Specified TRAPI message completely satisfies")
+    assert CodeDictionary.MESSAGE not in leaf
+
+    result = CodeDictionary.get_code_subtree("info.input_edge.predicate", facet="description")
+    assert result is not None
+    message_type, subtree = result
+    assert subtree is not None
+    assert isinstance(subtree, Dict)
+    assert all([key in ["abstract", "mixin"] for key in subtree])
+    assert CodeDictionary.DESCRIPTION in subtree["mixin"]
+    assert subtree["mixin"][CodeDictionary.DESCRIPTION] == \
+           "Input edge data can have 'mixin' predicates, when the mode of validation is 'non-strict'."
+    assert CodeDictionary.MESSAGE not in subtree["mixin"]
+
+
+def test_get_code_subtree_internal_subtree():
+    assert CodeDictionary.get_code_subtree("warning") is not None
+
+    result = CodeDictionary.get_code_subtree("warning.knowledge_graph")
+    assert result is not None
+    message_type, subtree = result
+    assert isinstance(subtree, Dict)
+    assert message_type == "warning"
+    assert subtree is not None
+    assert all([key in ["nodes", "node", "predicate", "edge"] for key in subtree])
+
+
+def test_get_entry():
+    assert CodeDictionary.get_code_entry("") is None
+
+    code_entry: Optional[Dict] = CodeDictionary.get_code_entry("info.compliant")
+    assert code_entry is not None
+    assert CodeDictionary.MESSAGE in code_entry
+    assert code_entry[CodeDictionary.MESSAGE] == "Biolink Model-compliant TRAPI Message"
+
+    # Higher level subtrees, not terminal leaf entries?
+    assert CodeDictionary.get_code_entry("info") is None
+    assert CodeDictionary.get_code_entry("skipped") is None
+    assert CodeDictionary.get_code_entry("info.query_graph") is None
+    assert CodeDictionary.get_code_entry("info.query_graph.node") is None
+    assert CodeDictionary.get_code_entry("warning") is None
+    assert CodeDictionary.get_code_entry("error") is None
+    assert CodeDictionary.get_code_entry("critical") is None
+
+    # Unknown code?
+    assert CodeDictionary.get_code_entry("foo.bar") is None
+
+
+def test_get_message_template():
+    assert CodeDictionary.get_message_template("") is None
+    assert CodeDictionary.get_message_template("info.compliant") == "Biolink Model-compliant TRAPI Message"
+    assert CodeDictionary.get_message_template("critical.trapi.request.invalid") == \
+           "Test could not generate a valid TRAPI query request object using identified element"
+    assert CodeDictionary.get_message_template("foo.bar") is None
+
+
+def test_get_description():
+    assert CodeDictionary.get_description("") is None
+    info_compliant = CodeDictionary.get_description("info.compliant")
+    assert info_compliant is not None
+    assert info_compliant.startswith("Specified TRAPI message completely satisfies")
+    info_attribute = CodeDictionary.get_description("warning.knowledge_graph.edge.attribute.type_id.non_biolink_prefix")
+    assert info_attribute is not None
+    assert info_attribute.startswith("Non-Biolink CURIEs are tolerated")
+    assert CodeDictionary.get_description("foo.bar") is None
+
+
+def test_message_display():
+    scoped_messages = CodeDictionary.display(code="info.compliant", add_prefix=True)
+    assert "INFO - Compliant: Biolink Model-compliant TRAPI Message" in scoped_messages["global"]
+
+    scoped_messages = CodeDictionary.display("error.knowledge_graph.nodes.empty", add_prefix=True)
+    assert "ERROR - Knowledge Graph Nodes: No nodes found" in scoped_messages["global"]
+
+    scoped_messages = CodeDictionary.display(
+        code="info.excluded",
+
+        # this code has "global" scope plus
+        # an "identifier" context, but no other parameters
+        messages={
+            "global": {"a->biolink:related_to->b": None}
+        },
+        add_prefix=True
+    )
+    assert "INFO - Excluded: All test case S-P-O triples from " + \
+           "resource test location, or specific user excluded S-P-O triples" in scoped_messages["global"]
+
+    scoped_messages = CodeDictionary.display(
+        code="info.input_edge.predicate.abstract",
+
+        # this code has "global" scope, an "identifier" context
+        # plus one other parameter named 'edge_id'
+        messages={
+            "infores:chebi->infores:molepro->infores:arax": {
+                "biolink:contributor": [
+                    {
+                        "edge_id": "a->biolink:related_to->b"
+                    }
+                ]
+            }
+        },
+        add_prefix=True
+    )
+    assert "INFO - Input Edge Predicate: Edge has an 'abstract' predicate" \
+           in scoped_messages["infores:chebi->infores:molepro->infores:arax"]
+
+
+def test_unknown_message_code():
+    with pytest.raises(AssertionError):
+        CodeDictionary.display(code="foo.bar")
+
+
+im_test_aggregated: IDENTIFIED_MESSAGES = {
+    "Fe": None,
+    "Fo": None,
+    "Fum": [
+        {
+            "I": "smell",
+            "the": "blood"
+        }
+    ]
+}
+
+im_test_additions: IDENTIFIED_MESSAGES = {
+    "Fi": None,
+    "Fum": [
+        {
+            "of": "an",
+            "English": "man"
+        }
+    ]
+}
 
 
-class TRAPIGraphType(Enum):
-    """ Enum type of Biolink Model compliant graph data being validated."""
-    Input_Edge = "Input Edge"
-    Query_Graph = "Query Graph"
-    Knowledge_Graph = "Knowledge Graph"
+# IDENTIFIED_MESSAGES = Dict[
+#     str,  # key is the message-unique template 'identifier' value of parameterized messages
+#
+#     # Note: some message codes may not have any associated
+#     # parameters beyond their discriminating identifier
+#     Optional[List[MESSAGE_PARAMETERS]]
+# ]
+def test_merge_identified_messages():
+    reporter = ValidationReporter()
+    aggregated: IDENTIFIED_MESSAGES = copy.deepcopy(im_test_aggregated)
+    additions: IDENTIFIED_MESSAGES = copy.deepcopy(im_test_additions)
+    reporter.merge_identified_messages(
+        aggregated=aggregated,
+        additions=additions
+    )
+    assert "Fi" in aggregated.keys()
+    assert any(
+        [
+            "man" in parameters.values()
+            for parameters in aggregated["Fum"]
+            if "Fum" in aggregated.keys() and aggregated["Fum"]
+        ],
+    )
+
+
+im_another_test_addition: IDENTIFIED_MESSAGES = {
+    "Humpty": None,
+    "Dumpty": [
+        {
+            "On": "a",
+            "big": "wall"
+        }
+    ]
+}
+
+
+im_yetanother_test_addition: IDENTIFIED_MESSAGES = {
+    "Dumpty": [
+        {
+            "Had": "a",
+            "big": "fall"
+        }
+    ]
+}
+
+scope_test_tag = "infores:tweedle_dee -> infores:tweedle_dum"
+sm_test_aggregated: SCOPED_MESSAGES = {
+    "global": im_test_aggregated,
+    "infores:foo -> infores:bar": None,
+    scope_test_tag: im_another_test_addition
+}
+
+
+sm_test_additions: SCOPED_MESSAGES = {
+    "global": im_test_additions,
+    scope_test_tag: im_yetanother_test_addition
+}
+
+
+def _check_coded_messages(
+        coded_messages: SCOPED_MESSAGES,
+        target_scope: str,
+        target_identifier: str,
+        target_parameter_values: List[str]
+):
+    assert coded_messages is not None and target_scope in coded_messages.keys()
+    scoped_messages: Optional[IDENTIFIED_MESSAGES] = coded_messages[target_scope]
+    assert all(
+        [
+            any([p in parameters.values() for p in target_parameter_values])
+            for parameters in scoped_messages[target_identifier]
+            if target_identifier in scoped_messages.keys() and scoped_messages[target_identifier]
+        ]
+    )
+
+
+def _check_unfriendly_giant(coded_messages: SCOPED_MESSAGES):
+    _check_coded_messages(
+        coded_messages,
+        target_scope="global",
+        target_identifier="Fum",
+        target_parameter_values=["blood", "man"]
+    )
+
+
+def _check_humpty_dumpty(coded_messages: SCOPED_MESSAGES):
+    _check_coded_messages(
+        coded_messages,
+        target_scope=scope_test_tag,
+        target_identifier="Dumpty",
+        target_parameter_values=["wall", "fall"]
+    )
+
+
+# SCOPED_MESSAGES = Dict[
+#     str,  # 'source trail' origin of affected edge or 'global' validation error
+#
+#     # (A given message code may have
+#     # no IDENTIFIED_MESSAGES with discriminating identifier
+#     #  and parameters hence, it may have a scoped value of 'None')
+#     Optional[IDENTIFIED_MESSAGES]
+# ]
+def test_merge_scoped_messages():
+    reporter = ValidationReporter()
+    aggregated: SCOPED_MESSAGES = copy.deepcopy(sm_test_aggregated)
+    additions: SCOPED_MESSAGES = copy.deepcopy(sm_test_additions)
+    reporter.merge_scoped_messages(
+        aggregated=aggregated,
+        additions=additions
+    )
+    global_scoped_message: Optional[IDENTIFIED_MESSAGES] = aggregated["global"]
+    assert global_scoped_message is not None and "Fi" in global_scoped_message.keys()
+
+    # Now check for Humpty Dumpty message
+    # in the 'aggregated' SCOPED_MESSAGES
+    _check_humpty_dumpty(aggregated)
+
+
+code_for_testing = "info.input_edge.predicate.abstract"
+pm_test_aggregated: MESSAGE_PARTITION = {
+    "info.excluded": {
+        "global": {
+            "Horace van der Gelder": None
+        }
+    },
+    code_for_testing: {
+        "global": im_test_aggregated,
+        scope_test_tag: im_another_test_addition
+    }
+}
+
+pm_test_additions: MESSAGE_PARTITION = {
+    "info.excluded": {
+        "global": {
+            "Dolly Gallagher Levi": None
+        }
+    },
+    "info.compliant": {
+        "global": None
+    },
+    code_for_testing: {
+        "global": im_test_additions,
+        scope_test_tag: im_yetanother_test_addition
+    }
+}
+
 
-    def label(self) -> str:
-        return self.value.lower().replace(" ", "_")
+# MESSAGE_PARTITION = Dict[
+#     str,  # message 'code' as indexing key
+#     SCOPED_MESSAGES
+# ]
+def test_merge_coded_messages():
+    reporter = ValidationReporter()
+    aggregated: MESSAGE_PARTITION = copy.deepcopy(pm_test_aggregated)
+    additions: MESSAGE_PARTITION = copy.deepcopy(pm_test_additions)
+    reporter.merge_coded_messages(
+        aggregated=aggregated,
+        additions=additions
+    )
+    assert "info.compliant" in aggregated.keys()
+
+
+##########################
+# Full message test data #
+##########################
+full_test_messages_catalog_1: MESSAGE_CATALOG = {
+    "info": {
+        "info.excluded": {
+            "global": {
+                "Dolly Gallagher Levi": None
+            }
+        },
+        "info.compliant": {
+            "global": None
+        },
+        code_for_testing: {
+            "global": copy.deepcopy(im_test_aggregated)
+        }
+    },
+    "skipped": {
+        "skipped.test": {
+            "global": {
+                "Catastrophe": None
+            }
+        }
 
+    },
+    "warning": {
+        "warning.knowledge_graph.node.id.unmapped_prefix": {
+            "infores:earth -> infores:spaceship": {
+                "Will Robinson": [
+                    {
+                        "categories": "Lost in Space"
+                    }
+                ]
+            }
+        }
+    }
+}
 
-class ValidationReporter:
-    """
-    General wrapper for managing validation status messages: information, warnings, errors and 'critical' (errors).
-    The TRAPI version and Biolink Model versions are also tracked for convenience at this abstract level
-    although their application is within specific pertinent subclasses.
-    """
+full_test_messages_catalog_2: MESSAGE_CATALOG = {
+    "info": {
+        "info.excluded": {
+            "global": {
+                "Horace van der Gelder": None
+            }
+        },
+        code_for_testing: {
+            "global": copy.deepcopy(im_test_additions),
+            scope_test_tag: copy.deepcopy(im_another_test_addition)
+        }
+    },
+    "error": {
+        "error.biolink.model.noncompliance": {
+            "global": {
+                "6.6.6": [
+                    {
+                        'reason': "Dave, this can only be due to human error..."
+                    }
+                ]
+            }
+        }
+    },
+    "critical": {
+        "critical.trapi.validation": {
+            "global": {
+                "9.1.1": [
+                    {
+                        'component': 'Query',
+                        'reason': "Fire, Ambulance or Police?"
+                    }
+                ]
+            }
+        }
+    }
+}
 
-    # Default major version resolves to latest TRAPI OpenAPI release,
-    # specifically 1.3.0, as of September 1st, 2022
-    DEFAULT_TRAPI_VERSION = "1"
 
-    _message_type_tag: Dict[str, str] = {
-        "info": "information",
-        "warning": "warnings",
-        "error": "errors",
-        "critical": "critical"
+full_test_messages_catalog_3: MESSAGE_CATALOG = {
+    "info": {
+        code_for_testing: {
+            scope_test_tag: copy.deepcopy(im_yetanother_test_addition)
+        }
     }
+}
 
-    @classmethod
-    def get_message_type_tag(cls, message_type: str):
-        return cls._message_type_tag[message_type]
-
-    def __init__(
-            self,
-            prefix: Optional[str] = None,
-            strict_validation: Optional[bool] = None
+critical_test = "new_test_2"
+full_test_messages_by_test_1: MESSAGES_BY_TEST = {
+    "new_test_1": copy.deepcopy(full_test_messages_catalog_1),
+    critical_test: copy.deepcopy(full_test_messages_catalog_2)
+}
+
+full_test_messages_by_test_2: MESSAGES_BY_TEST = {
+    "new_test_3": copy.deepcopy(full_test_messages_catalog_3)
+}
+
+critical_target = "new_target_1"
+full_test_messages_by_target: MESSAGES_BY_TARGET = {
+    critical_target: copy.deepcopy(full_test_messages_by_test_1),
+    "new_target_2": copy.deepcopy(full_test_messages_by_test_2)
+}
+
+
+def test_get_all_messages_of_type():
+    reporter = ValidationReporter()
+    # Load the reporter with several messages
+    # across multiple test and target contexts
+    reporter.add_messages(new_messages=full_test_messages_by_target)
+    messages: MESSAGE_PARTITION = reporter.get_all_messages_of_type(MessageType.info)
+    print(messages, file=sys.stderr, flush=True)
+    assert all([code in ["info.excluded", "info.compliant", code_for_testing] for code in messages])
+    info_excluded_scoped_messages: SCOPED_MESSAGES = messages["info.excluded"]
+    assert "global" in info_excluded_scoped_messages and info_excluded_scoped_messages["global"] is not None
+    assert all(
+        [
+            identifier in ["Dolly Gallagher Levi", "Horace van der Gelder"]
+            for identifier in info_excluded_scoped_messages["global"].keys()
+        ]
+    )
+    info_compliant_messages: SCOPED_MESSAGES = messages["info.compliant"]
+    assert "global" in info_compliant_messages and info_compliant_messages["global"] is None
+
+    # In the SCOPED_MESSAGES associated with 'code_for_testing',
+    # Check for Jack in the Beanstalk Giant messages...
+    _check_unfriendly_giant(messages[code_for_testing])
+    # ...then, for Humpty Dumpty messages...
+    _check_humpty_dumpty(messages[code_for_testing])
+
+
+def test_prefix_accessors():
+    reporter = ValidationReporter()
+    assert reporter.report_header().startswith("Validation Report\n")
+    assert reporter.get_default_target() == "Target"
+    reporter.reset_default_target("test_prefix_accessors")
+    assert reporter.get_default_target() == "test_prefix_accessors"
+
+
+def test_get_message_type():
+    reporter = ValidationReporter()
+    assert reporter.get_message_type("info.compliant") == MessageType.info
+    assert reporter.get_message_type("skipped.test") == MessageType.skipped
+    assert reporter.get_message_type("warning.graph.empty") == MessageType.warning
+    assert reporter.get_message_type("error.trapi.response.empty") == MessageType.error
+    assert reporter.get_message_type("critical.trapi.validation") == MessageType.critical
+    with pytest.raises(NotImplementedError):
+        # unknown message type
+        reporter.get_message_type(code="foo.bar")
+
+
+def test_global_sourced_validation_message_report():
+    reporter1 = ValidationReporter(
+        default_test="test_global_sourced_validation_message_report",
+        default_target="First Validation Report"
+    )
+    reporter1.report(code="info.compliant")
+    reporter1.report(
+        code="info.input_edge.predicate.abstract",
+        identifier="biolink:contributor",
+        edge_id="a->biolink:contributor->b"
+    )
+    messages_by_code: MESSAGE_PARTITION = reporter1.get_messages_of_type(MessageType.info)
+    assert len(messages_by_code) > 0
+
+    displayed: List[str] = list()
+    for code, messages in messages_by_code.items():
+        scoped_messages = CodeDictionary.display(code, messages, add_prefix=True)
+        displayed.extend(scoped_messages["global"])
+    assert "INFO - Compliant: Biolink Model-compliant TRAPI Message" in displayed
+    assert "INFO - Input Edge Predicate: Edge has an 'abstract' predicate" in displayed
+
+
+def test_source_trail_scoped_validation_message_report():
+    reporter2 = ValidationReporter(
+        default_test="test_source_trail_scoped_validation_message_report",
+        default_target="Second Validation Report"
+    )
+    reporter2.report(
+        code="error.knowledge_graph.edge.predicate.abstract",
+        identifier="biolink:contributor",
+        edge_id="Richard->biolink:contributor->Translator",
+        source_trail="infores:sri"
+    )
+    reporter2.report(
+        code="error.knowledge_graph.edge.predicate.abstract",
+        identifier="biolink:contributor",
+        edge_id="Tim->biolink:contributor->Translator",
+        source_trail="infores:sri"
+    )
+    messages_by_code: MESSAGE_PARTITION = reporter2.get_messages_of_type(MessageType.error)
+    assert len(messages_by_code) > 0
+    assert "error.knowledge_graph.edge.predicate.abstract" in messages_by_code
+    assert "infores:sri" in messages_by_code['error.knowledge_graph.edge.predicate.abstract']
+    assert "global" not in messages_by_code['error.knowledge_graph.edge.predicate.abstract']
+
+
+def _validate_full_messages(
+        reporter: ValidationReporter,
+        message_type: MessageType,
+        full_message: str
+) -> None:
+    # DRY helper function for validating fully annotated messages
+    messages_by_code: MESSAGE_PARTITION = reporter.get_all_messages_of_type(message_type)
+    assert len(messages_by_code) > 0
+    full_messages_list: List[str] = list()
+    for code, messages in messages_by_code.items():
+        scoped_messages: Dict = CodeDictionary.display(code, messages, add_prefix=True)
+        scope, value = scoped_messages.popitem()
+        full_messages_list.append(value[0])
+    assert full_message in full_messages_list
+
+
+def test_messages():
+    # Loading and checking a first reporter
+    tm_default_test = "test_messages"
+    tm_default_target = "1st Test Message Set"
+    reporter1 = ValidationReporter(
+        default_test=tm_default_test,
+        default_target=tm_default_target
+    )
+    assert not reporter1.has_messages()
+    reporter1.report("info.compliant")
+    assert reporter1.has_messages()
+    assert reporter1.has_information()
+    assert not reporter1.has_warnings()
+    assert not reporter1.has_skipped()
+    assert not reporter1.has_errors()
+    assert not reporter1.has_critical()
+
+    reporter1.report("warning.graph.empty", identifier="Reporter1 Unit Test")
+    assert reporter1.has_warnings()
+    reporter1.report("error.knowledge_graph.nodes.empty")
+    assert reporter1.has_errors()
+
+    # Testing merging of messages from a second reporter
+    reporter2 = ValidationReporter(
+        default_test="test_messages",
+        default_target="2nd Test Message Set"
+    )
+    reporter2.report(
+        code="info.query_graph.edge.predicate.mixin",
+        identifier="biolink:this_is_a_mixin",
+        edge_id="a-biolink:this_is_a_mixin->b"
+    )
+    reporter2.report("warning.trapi.response.results.empty")
+    reporter2.report("error.knowledge_graph.edges.empty")
+    reporter1.merge(reporter2)
+
+    # No prefix...
+    reporter3 = ValidationReporter()
+    reporter3.report("error.trapi.response.query_graph.missing")
+    reporter1.merge(reporter3)
+
+    # testing addition a few raw batch messages
+    reporter1.add_messages(full_test_messages_by_target)
+
+    # Verify what we have
+    test_message_type: MessageType
+    full_message: str
+    for test_message_type, full_message in (
+        (
+            MessageType.info,
+            "INFO - Excluded: All test case S-P-O triples from resource test location, " +
+            "or specific user excluded S-P-O triples"
+        ),
+        (
+            MessageType.skipped,
+            "SKIPPED - Test: For reason indicated in the identifier"
+        ),
+        (
+            MessageType.warning,
+            "WARNING - Knowledge Graph Node Id Unmapped: Node identifier found unmapped to target categories for node"
+        ),
+        (
+            MessageType.error,
+            "ERROR - Biolink Model: S-P-O statement is not compliant to Biolink Model release"
+        ),
+        (
+            MessageType.critical,
+            "CRITICAL - Trapi: Schema validation error"
+        ),
     ):
-        """
-        :param prefix: Optional[str] =  None, named context of the Validator, used as a prefix in validation messages.
-        :param strict_validation: Optional[bool] = None, if True, some tests validate as 'error';  False, simply issues
-                                  'info' message; A value of 'None' uses the default value for specific graph contexts.
-        """
-        self.prefix: str = prefix if prefix else ""
-        self.strict_validation: Optional[bool] = strict_validation
-        self.messages: MESSAGE_CATALOG = {
-            "critical": dict(),
-            "errors": dict(),
-            "warnings": dict(),
-            "information": dict()
-        }
-
-    def is_strict_validation(self, graph_type: TRAPIGraphType) -> bool:
-        """
-        Predicate to test if strict validation is to be applied. If the internal
-        'strict_validation' flag is not set (i.e. None), then graph_type is
-        to resolve strictness based on TRAPI graph type context.
-
-        :param graph_type: TRAPIGraphType, type of TRAPI graph component being validated
-        :return: bool, value of validation strictness set in the ValidationReporter.
-        """
-        if self.strict_validation is None:
-            if graph_type == TRAPIGraphType.Knowledge_Graph:
-                return True
-            else:
-                return False
-        else:
-            return self.strict_validation
+        _validate_full_messages(reporter1, test_message_type, full_message)
 
-    def has_messages(self) -> bool:
-        """Predicate to detect any recorded validation messages.
-        :return: bool, True if ValidationReporter has any non-empty messages.
-        """
-        return self.has_information() or self.has_warnings() or self.has_errors() or self.has_critical()
-
-    def has_information(self) -> bool:
-        """Predicate to detect any recorded information messages.
-        :return: bool, True if ValidationReporter has any information messages.
-        """
-        return bool(self.messages["information"])
-
-    def has_warnings(self) -> bool:
-        """Predicate to detect any recorded warning messages.
-        :return: bool, True if ValidationReporter has any warning messages.
-        """
-        return bool(self.messages["warnings"])
-
-    def has_errors(self) -> bool:
-        """Predicate to detect any recorded error messages.
-        :return: bool, True if ValidationReporter has any error messages.
-        """
-        return bool(self.messages["errors"])
-
-    def has_critical(self) -> bool:
-        """Predicate to detect any recorded critical error messages.
-        :return: bool, True if ValidationReporter has any critical error messages.
-        """
-        return bool(self.messages["critical"])
-
-    def dump_info(self, flat=False) -> str:
-        """Dump information messages as JSON.
-        :param flat: render output as 'flat' JSON (default: False)
-        :return: str, JSON formatted string of information messages.
-        """
-        return _output(self.messages["information"], flat)
-
-    def dump_warnings(self, flat=False) -> str:
-        """Dump warning messages as JSON.
-        :param flat: render output as 'flat' JSON (default: False)
-        :return: str, JSON formatted string of warning messages.
-        """
-        return _output(self.messages["warnings"], flat)
-
-    def dump_errors(self, flat=False) -> str:
-        """Dump error messages as JSON.
-        :param flat: render output as 'flat' JSON (default: False)
-        :return: str, JSON formatted string of error messages.
-        """
-        return _output(self.messages["errors"], flat)
-
-    def dump_critical(self, flat=False) -> str:
-        """Dump critical error messages as JSON.
-        :param flat: render output as 'flat' JSON (default: False)
-        :return: str, JSON formatted string of critical error messages.
-        """
-        return _output(self.messages["critical"], flat)
-
-    def dump_messages(self, flat=False) -> str:
-        """Dump all messages as JSON.
-        :param flat: render output as 'flat' JSON (default: False)
-        :return: str, JSON formatted string of all messages.
-        """
-        return _output(self.messages, flat)
-
-    @staticmethod
-    def get_message_type(code: str) -> str:
-        """Get type of message code.
-        :param code: message code
-        :return: message type, one of 'info', 'warning', 'error' or 'critical'
-        """
-        code_id_parts: List[str] = code.split('.')
-        message_type: str = code_id_parts[0]
-        if message_type in ['info', 'warning', 'error', 'critical']:
-            return message_type
-        else:
-            raise NotImplementedError(
-                f"ValidationReport.get_message_type(): {code} is unknown code type: {message_type}"
+    obj = reporter1.to_dict()
+    assert "messages" in obj
+    assert critical_target in obj["messages"]
+    assert critical_test in obj["messages"][critical_target]
+    assert "critical" in obj["messages"][critical_target][critical_test]
+    assert "critical.trapi.validation" in obj["messages"][critical_target][critical_test]["critical"]
+
+    messages_by_target: SCOPED_MESSAGES = \
+        obj["messages"][critical_target][critical_test]["critical"]["critical.trapi.validation"]
+    assert messages_by_target, "Empty 'critical.trapi.validation' messages set?"
+    assert "9.1.1" in messages_by_target["global"]
+    message_subset: List = messages_by_target["global"]["9.1.1"]
+    assert "Fire, Ambulance or Police?" \
+           in [message['reason'] for message in message_subset if 'reason' in message]
+
+    for n in range(0, 10):
+        reporter1.report(code="error.input_edge.node.category.missing", identifier=f"biolink:not_a_category_{n}")
+
+    for c in range(0, 5):
+        for n in range(0, 10):
+            reporter1.report(
+                code="error.input_edge.node.category.unknown",
+                identifier=f"biolink:not_a_category_{c}",
+                node_id=f"n{n}"
             )
 
-    def report(self, code: str, source_trail: Optional[str] = None, **message):
-        """
-        Capture a single validation message, as per specified 'code' (with any code-specific contextural parameters).
-
-        :param code: str, dot delimited validation path code
-        :param source_trail, Optional[str], audit trail of knowledge source provenance for a given Edge, as a string.
-                             Defaults to "global" if not specified.
-        :param message: **Dict, named parameters representing extra (str-formatted) context for the given code message
-        :return: None (internally record the validation message)
-        """
-        # Sanity check: that the given code has been registered in the codes.yaml file
-        assert CodeDictionary.get_code_entry(code) is not None, f"ValidationReporter.report: unknown code '{code}'"
-
-        message_type_id = self.get_message_type(code)
-        message_type_tag = self.get_message_type_tag(message_type_id)
-        if code not in self.messages[message_type_tag]:
-            self.messages[message_type_tag][code] = dict()
-
-        # Set current scope of validation message
-        if source_trail is None:
-            source_trail = "global"
-
-        if source_trail not in self.messages[message_type_tag][code]:
-            self.messages[message_type_tag][code][source_trail] = dict()
-
-        scope = self.messages[message_type_tag][code][source_trail]
-
-        if message:
-            # If a message has any parameters, then one of them is
-            # expected to be a message indexing identifier
-            if "identifier" in message:
-                message_identifier = message.pop("identifier")
-                if not message:
-                    # the message_identifier was the only parameter to keep track of...
-                    scope[message_identifier] = None
-                else:
-                    # keep track of additional parameters in a list of dictionaries
-                    # (may have additional, currently unavoidable, content duplication?)
-                    if message_identifier not in scope or scope[message_identifier] is None:
-                        scope[message_identifier] = list()
-
-                    scope[message_identifier].append(message)
-
-        # else: additional parameters are None
-
-    def add_messages(self, new_messages: MESSAGE_CATALOG):
-        """
-        Batch addition of a dictionary of messages to a ValidationReporter instance.
-        :param new_messages: Dict[str, Dict], with key one of "information", "warnings", "errors" or "critical",
-                              with 'code' keyed dictionaries of (structured) message parameters.
-        """
-        for message_type in self.messages:   # 'info', 'warning', 'error', 'critical'
-            if message_type in new_messages:
-                message_type_contents = new_messages[message_type]
-                for code, details in message_type_contents.items():   # codes.yaml message codes
-                    if code not in self.messages[message_type]:
-                        self.messages[message_type][code] = dict()
-
-                    # 'source' scope is 'global' or a source trail path string, from primary to topmost aggregator
-                    for source, content in details.items():
-                        scope = self.messages[message_type][code][source] = dict()
-                        if content:
-                            # content is of type Dict[str, Optional[List[Dict[str, str]]]]
-                            # where dictionary keys are a set of message discriminating 'identifier'
-                            identifier: str
-                            parameters: Optional[List[Dict[str, str]]]
-                            for identifier, parameters in content.items():
-                                if self.messages[message_type][code] is None:
-                                    self.messages[message_type][code] = dict()
-                                if parameters:
-                                    # additional parameters seen?
-                                    if identifier not in self.messages[message_type][code] or \
-                                            scope[identifier] is None:
-                                        scope[identifier] = list()
-
-                                    scope[identifier].extend(parameters)
-                                else:
-                                    # the message 'identifier' is the only parameter
-                                    scope[identifier] = None
-
-    def get_messages(self) -> MESSAGE_CATALOG:
-        """
-        Get copy of all messages as a Python data structure.
-        :return: Dict (copy) of all validation messages in the ValidationReporter.
-        """
-        return copy.deepcopy(self.messages)
-
-    def get_info(self) -> MESSAGE_PARTITION:
-        """
-        Get copy of all recorded 'information' messages.
-        :return: List, copy of all information messages.
-        """
-        return copy.deepcopy(self.messages["information"])
-
-    def get_warnings(self) -> MESSAGE_PARTITION:
-        """
-        Get copy of all recorded 'warning' messages.
-        :return: List, copy of all warning messages.
-        """
-        return copy.deepcopy(self.messages["warnings"])
-
-    def get_errors(self) -> MESSAGE_PARTITION:
-        """
-        Get copy of all recorded 'error' messages.
-        :return: List, copy of all error messages.
-        """
-        return copy.deepcopy(self.messages["errors"])
-
-    def get_critical(self) -> MESSAGE_PARTITION:
-        """
-        Get copy of all recorded 'critical' error messages.
-        :return: List, copy of all critical error messages.
-        """
-        return copy.deepcopy(self.messages["critical"])
-
-    ############################
-    # General Instance methods #
-    ############################
-    def merge(self, reporter):
-        """
-        Merge all messages and metadata from a second ValidationReporter,
-        into the calling ValidationReporter instance.
-
-        :param reporter: second ValidationReporter
-        """
-        assert isinstance(reporter, ValidationReporter)
-
-        # new coded messages also need to be merged!
-        self.add_messages(reporter.get_messages())
-
-    def to_dict(self) -> Dict:
-        """
-        Export ValidationReporter message contents as a Python dictionary.
-        :return: Dict
-        """
-        return {"messages": self.get_messages()}
-
-    def apply_validation(self, validation_method, *args, **kwargs) -> bool:
-        """
-        Wrapper to allow validation_methods direct access to the ValidationReporter.
-
-        :param validation_method: function which accepts this instance of the
-               ValidationReporter as its first argument, for use in reporting validation errors.
-        :param args: any positional arguments to the validation_method, after the initial ValidationReporter argument
-        :param kwargs: any (optional, additional) keyword arguments to the validation_method, after positional arguments
-        :return: bool, returns 'False' if validation method documented (critical) errors; True otherwise
-        """
-        validation_method(self, *args, **kwargs)
-        # TODO: not sure if we should detect both 'errors' and 'critical' here or just 'critical'
-        if self.has_critical() or self.has_errors():
-            return False
-        else:
-            return True
+    # Informal test of a text 'dump' of all the messages as a
+    # text blob, using the 'display_all' method to format them
+    print(
+        "\n\nThis is an indirect 'test' of the ValidationReporter.dump() method\n"
+        "which simply executes the function and look at the results here on the console:",
+        file=stderr
+    )
+    reporter1.dump(file=stderr)
+
+    print(
+        f"\n{'-'*80}\n" +
+        "ValidatorReporter.dump() with title suppressed using 'title=None'\n" +
+        "and compressed using 'id_rows=2', 'msg_rows=3', 'compress=True':\n",
+        file=stderr
+    )
+    reporter1.dump(title=None, id_rows=2, msg_rows=3, compact_format=True, file=stderr)
+
+    print(
+        f"\n{'-'*80}\n" +
+        "ValidatorReporter.dump() resetting the title to a user string\n" +
+        "and compressed using 'id_rows=1', 'msg_rows=1', 'compress=True':\n",
+        file=stderr
+    )
+    reporter1.dump(title="My KP Validation Report", id_rows=1, msg_rows=1, compact_format=True, file=stderr)
+
+    validation_report: str = reporter1.dumps(id_rows=2, msg_rows=3)
+    assert validation_report.startswith("Reasoner Validator")
+
+
+def test_validator_method():
+
+    reporter = ValidationReporter(
+        default_test="test_validator_method",
+        default_target="Test Validator Method"
+    )
 
-    @staticmethod
-    def test_case_has_validation_errors(tag: str, case: Dict) -> bool:
-        """Check if test case has validation errors.
-
-        :param tag: str, top level string key in the 'case' whose value is the validation messages 'dictionary'
-        :param case: Dict, containing error messages in a structurally similar
-                     format to what is returned by the to_dict() method in this class.
-        :return: True if the case contains validation messages
-        """
-        # TODO: not sure if we should detect both 'errors' and 'critical' here or just 'critical'
-        #
-        # The 'case' dictionary object could have a format something like this:
-        #
-        #     tag: {
-        #         ...
-        #         "messages": {
-        #             "information": [],
-        #             "warnings": [
-        #                 {
-        #                     "warning.predicate.non_canonical": {
-        #                         "infores:molepro -> infores:arax": {  # local source scope of error
-        #                             "biolink:participates_in": {
-        #                                   "edge_id": "a--['biolink:participates_in']->b"
-        #                             }
-        #                         }
-        #                     }
-        #                 }
-        #             ],
-        #             "errors": [
-        #                 {
-        #                     "error.knowledge_graph.empty_nodes": {
-        #                         "global": None  # scope of error
-        #                     }
-        #                 }
-        #             ],
-        #             "critical": [
-        #                 {
-        #                     "critical.trapi.validation": {
-        #                         "global": None   # scope of critical error
-        #                     }
-        #                 }
-        #             ]
-        #         }
-        #     }
-        #
-        # where 'tag' == 'messages' and we have a non-empty "errors" set of messages
-        #
-        if case is not None and tag in case and \
-                'messages' in case[tag] and \
-                (
-                    'errors' in case[tag]['messages'] and case[tag]['messages']['errors'] or
-                    'critical' in case[tag]['messages'] and case[tag]['messages']['critical']
-                ):
-            return True
-        else:
-            return False
+    test_data: Dict = {
+        "some key": "some value"
+    }
+    test_parameters: Dict = {
+        "some parameter": "some parameter value",
+        "another parameter": "some other parameter value"
+    }
 
-    def report_header(self, title: Optional[str], compact_format: bool) -> str:
-        header: str = ""
-        if title is not None:
-
-            if not compact_format:
-                header += "\n"
-
-            if not title:
-                title = f"Validation Report"
-                title += f" for '{self.prefix}'" if self.prefix else ""
-
-            if not compact_format:
-                header += f"\n\033[4m{title}\033[0m\n"
-            else:
-                # compact also ignores underlining
-                header += f"{title}\n"
-
-        if not compact_format:
-            header += "\n"
-
-        header += f"Reasoner Validator version '{metadata.version('reasoner-validator')}'"
-        return header
-
-    def dump(
-            self,
-            title: Optional[str] = "",
-            id_rows: int = 0,
-            msg_rows: int = 0,
-            compact_format: bool = False,
-            file=stdout
+    def validator_method(validator: ValidationReporter, arg, **case):
+        assert isinstance(arg, Dict)
+        assert arg['some key'] == "some value"
+        validator.report(
+            "error.knowledge_graph.edge.provenance.infores.missing",
+            identifier="fake-edge-id",
+            infores="foo:bar"
+        )
+        assert len(case) == 2
+        assert case['some parameter'] == "some parameter value"
+        assert case['another parameter'] == "some other parameter value"
+        validator.report("warning.graph.empty", identifier="Fake")
+
+    reporter.apply_validation(validator_method, test_data, **test_parameters)
+
+    test_message_type: MessageType
+    full_message: str
+    for test_message_type, full_message in (
+        (
+            MessageType.warning,
+            "WARNING - Graph: Empty graph"
+        ),
+        (
+            MessageType.error,
+            "ERROR - Knowledge Graph Edge Provenance Infores: " +
+            "Edge has provenance value which is not a well-formed InfoRes CURIE"
+        )
     ):
-        """
-        Dump all available messages captured by the ValidationReporter,
-        printed as formatted human-readable text, on a specified file device.
-
-        :param title: Optional[str], user supplied report title (default: autogenerated if not set or empty string;
-                                     suppressed if an explicit argument of None is given); default: "" -> default title
-        :param id_rows: int >= 0, if set, maximum number of code-related identifiers to
-                             print per code (value of 0 means print all; default: 0)
-        :param msg_rows: int >= 0, if set, maximum number of parameterized code-related messages to
-                                  print per identifier row (value of 0 means print all; default: 0)
-        :param compact_format: bool, if True, omit blank lines inserted by default for human readability;
-                               also, suppress character escapes (i.e. underlining of titles) (default: False)
-        :param file: target file device for output
-        :return: n/a
-        """
-        assert id_rows >= 0, "dump(): 'id_rows' argument must be positive or equal to zero"
-        assert msg_rows >= 0, "dump(): 'pm_rows' argument must be positive or equal to zero"
-
-        print(f"{self.report_header(title, compact_format)}.\n", file=file)
-
-        if self.has_messages():
-
-            # self.messages is a MESSAGE_CATALOG where MESSAGE_CATALOG is Dict[<message type>, MESSAGE_PARTITION]
-            # <message type> is the top level partition of messages into 'critical', 'error', 'warning' or 'info'
-            message_type: str
-            coded_messages: MESSAGE_PARTITION
-            for message_type, coded_messages in self.messages.items():
-
-                # if there are coded validation messages for a
-                # given message type: 'critical', 'error', 'warning' or 'info' ...
-                if coded_messages:
-
-                    # ... then iterate through them and print them out
-
-                    if not compact_format:
-                        print(f"\033[4m{message_type.capitalize()}\033[0m", file=file)
-                        print(file=file)
-                    else:
-                        # compact also ignores underlining
-                        print(f"\n{message_type.capitalize()}:", file=file)
-
-                    # 'coded_messages' is a MESSAGE_PARTITION where
-                    # MESSAGE_PARTITION is Dict[<validation code>, SCOPED_MESSAGES]
-
-                    # 'validation code' is the dot-delimited string
-                    # representation of the YAML path of the message codes.yaml
-                    code: str
-                    messages_by_code:  SCOPED_MESSAGES
-
-                    # Grouping message outputs by validation codes
-                    for code, messages_by_code in coded_messages.items():
-
-                        code_label: str = CodeDictionary.validation_code_tag(code)
-                        print(
-                            f"* {code_label}:\n"
-                            f"=> {CodeDictionary.get_message_template(code)}",
-                            file=file
-                        )
-                        if not compact_format:
-                            print(file=file)
-
-                        # 'messages_by_code' is a SCOPED_MESSAGES where
-                        # SCOPED_MESSAGES is Dict[<scope>, Optional[IDENTIFIED_MESSAGES]]
-
-                        # <scope> is "global" or source trail path string
-                        scope: str
-                        messages_by_scope: Optional[IDENTIFIED_MESSAGES]
-                        for scope, messages_by_scope in messages_by_code.items():
-
-                            print(f"\t$ {scope}", file=file)
-
-                            # Codes with associated parameters should have
-                            # an embedded dictionary with 'identifier' keys
-
-                            ids_per_row: int = 0
-                            num_ids: int = len(messages_by_scope.keys())
-                            more_ids: int = num_ids - id_rows if num_ids > id_rows else 0
-
-                            # 'messages_by_scope' is Optional[IDENTIFIED_MESSAGES] where
-                            # 'IDENTIFIED_MESSAGES' is Dict[<identifier>, Optional[List[MESSAGE_PARAMETERS]]]
-
-                            # An entry of 'messages_by_scope' may be None if the given message code
-                            # has no additional parameters that distinguish instances of context (e.g. edge id?)
-                            # where the validation message occurs for the given identifier.
-
-                            # unique 'identifier' discriminator of the
-                            # (TRAPI or Biolink) token target of the validation
-                            identifier: str
-                            messages: Optional[List[MESSAGE_PARAMETERS]]
-                            for identifier, messages in messages_by_scope.items():
-
-                                if messages is None:
-
-                                    # For codes whose context of validation is solely discerned
-                                    # with their identifier, just print out the identifier
-
-                                    print(f"\t\t# {identifier}", file=file)
-
-                                    if not compact_format:
-                                        print(file=file)
-
-                                else:
-                                    # Since we have already checked if messages is None above, then we assume here that
-                                    # 'messages' is a List[MESSAGE_PARAMETERS] which records distinct additional context
-                                    # for a list of messages associated with a given code.
-                                    print(f"\t\t# {identifier}:", file=file)
-
-                                    first_message: bool = True
-                                    messages_per_row: int = 0
-                                    num_messages: int = len(messages)
-                                    more_msgs: int = num_messages - msg_rows if num_messages > msg_rows else 0
-
-                                    # 'messages' is an instance List[MESSAGE_PARAMETERS] where every entry of
-                                    # 'MESSAGE_PARAMETERS' is a dictionary of additional parameters documenting
-                                    # one specific instance of validation message related to the given identifier,
-                                    # where the keys are validation code specific (documented in codes.yaml)
-                                    parameters: MESSAGE_PARAMETERS
-                                    for parameters in messages:
-
-                                        if first_message:
-                                            tags = tuple(parameters.keys())
-                                            print(f"\t\t- {' | '.join(tags)}: ", file=file)
-                                            first_message = False
-
-                                        print(f"\t\t\t{' | '.join(parameters.values())}", file=file)
-
-                                        messages_per_row += 1
-                                        if msg_rows and messages_per_row >= msg_rows:
-                                            if more_msgs:
-                                                print(
-                                                    f"\t\t{str(more_msgs)} more messages " +
-                                                    f"for identifier '{identifier}'...",
-                                                    file=file
-                                                )
-                                            break
-
-                                    if not compact_format:
-                                        print(file=file)
-
-                                ids_per_row += 1
-                                if id_rows and ids_per_row >= id_rows:
-                                    if more_ids:
-                                        print(
-                                            f"{str(more_ids)} more identifiers for code '{code_label}'...",
-                                            file=file
-                                        )
-                                    break
-
-                            if not compact_format:
-                                print(file=file)
-
-                        # else:
-                        #     For codes with associated non-parametric templates,
-                        #     just printing the template (done above) suffices
+        _validate_full_messages(reporter, test_message_type, full_message)
 
-                # else: print nothing if a given message_type has no messages
-        else:
-            print(f"Hurray! No validation messages reported!", file=file)
 
-    def dumps(
-            self,
-            id_rows: int = 0,
-            msg_rows: int = 0,
-            compact_format: bool = True
-    ) -> str:
-        """
-        Text string version of dump(): returns all available messages captured by the
-        ValidationReporter, as a formatted human-readable text blob.
-
-        :param id_rows: int >= 0, if set, maximum number of code-related identifiers to
-                             print per code (value of 0 means print all; default: 0)
-        :param msg_rows: int >= 0, if set, maximum number of parameterized code-related messages to
-                                  print per identifier row (value of 0 means print all; default: 0)
-        :param compact_format: bool, if True, omit blank lines inserted by default for human readability (default: True)
-        :return: n/a
-        """
-        output_buffer: StringIO = StringIO()
-        self.dump(
-            title=None,  # title suppressed in dumps() string output
-            id_rows=id_rows,
-            msg_rows=msg_rows,
-            compact_format=compact_format,
-            file=output_buffer
-        )
-        text_output: str = output_buffer.getvalue()
-        output_buffer.close()
-        return text_output.strip()
+@pytest.mark.parametrize(
+    "tag,case,result",
+    [
+        (
+            'validation',
+            {
+                "validation": {
+                    "messages": {
+                        "information": {},
+                        "skipped tests": {},
+                        "warnings": {},
+                        "errors": {},
+                        "critical": {""}
+                    }
+                }
+            },
+            True
+        ),
+        (
+            'validation',
+            {
+                "validation": {
+                    "messages": {
+                        "information": {},
+                        "skipped tests": {},
+                        "warnings": {},
+                        "errors": {""},
+                        "critical": {}
+                    }
+                }
+            },
+            True
+        ),
+        (
+            "validation",
+            {
+                "validation": {
+                    "messages": {
+                        "information": {},
+                        "skipped tests": {},
+                        "warnings": {
+                            "warning.input_edge.node.category.deprecated": [
+                                {
+                                    "identifier": "biolink:ChemicalSubstance"
+                                }
+                            ],
+                            "warning.knowledge_graph.edge.predicate.non_canonical": [
+                                {
+                                    "identifier": "ABC1--biolink:participates_in->Glycolysis",
+                                    "predicate": "biolink:participates_in"
+                                }
+                            ]
+                        },
+                        "errors": {},
+                        "critical": {}
+                    }
+                }
+            },
+            False
+        ),
+    ]
+)
+def test_has_validation_errors(tag: str, case: Dict, result: bool):
+    reporter = ValidationReporter()
+    assert reporter.test_case_has_validation_errors(tag=tag, case=case) == result
```

### Comparing `reasoner_validator-3.9.5/reasoner_validator/sri/util.py` & `reasoner_validator-4.0.0/reasoner_validator/sri/util.py`

 * *Files identical despite different names*

### Comparing `reasoner_validator-3.9.5/reasoner_validator/trapi/__init__.py` & `reasoner_validator-4.0.0/reasoner_validator/trapi/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -226,38 +226,41 @@
 class TRAPISchemaValidator(ValidationReporter):
     """
     TRAPI Validator is a wrapper class for validating
     conformance of JSON messages to the Translator Reasoner API.
     """
     def __init__(
             self,
-            prefix: Optional[str] = None,
+            default_test: Optional[str] = None,
+            default_target: Optional[str] = None,
             trapi_version: Optional[str] = None,
             strict_validation: Optional[bool] = None
     ):
         """
         TRAPI Validator constructor.
-
-        :param prefix: str named context of the TRAPISchemaValidator, used as a prefix in validation messages.
+        :param default_test: Optional[str] =  None, initial default test context of the TRAPISchemaValidator messages
+        :param default_target: Optional[str] =  None, initial default target context of the TRAPISchemaValidator,
+                                                also used as a prefix in validation messages.
         :param trapi_version: str, version of component to validate against
         :param strict_validation: Optional[bool] = None, if True, some tests validate as 'error';  False, simply issues
                                   'info' message; A value of 'None' uses the default value for specific graph contexts.
 
         """
         self.default_trapi: bool = False
         if trapi_version is None:
             self.default_trapi = True
         self.trapi_version = get_latest_version(trapi_version) \
             if trapi_version else get_latest_version(self.DEFAULT_TRAPI_VERSION)
 
-        logger.info(f"TRAPISchemaValidator set to TRAPI Version: '{self.trapi_version}'")
+        logger.debug(f"TRAPISchemaValidator set to TRAPI Version: '{self.trapi_version}'")
 
         ValidationReporter.__init__(
             self,
-            prefix=prefix if prefix is not None else "TRAPI Validation",
+            default_test=default_test if default_test is not None else "Standards Test",
+            default_target=default_target if default_target is not None else "TRAPI Validation",
             strict_validation=strict_validation
         )
 
     def get_trapi_version(self) -> str:
         """
         :return: str, TRAPI (SemVer) version currently targeted by the TRAPISchemaValidator.
         """
@@ -365,12 +368,12 @@
         (including TRAPI version and parent class dictionary content)
         :return: Dict
         """
         dictionary = ValidationReporter.to_dict(self)
         dictionary["trapi_version"] = self.get_trapi_version()
         return dictionary
 
-    def report_header(self, title: Optional[str], compact_format: bool) -> str:
+    def report_header(self, title: Optional[str] = None, compact_format: bool = True) -> str:
         header: str = ValidationReporter.report_header(self, title, compact_format)
         header += f" validating against TRAPI version " \
                   f"'{str(self.get_trapi_version() if self.get_trapi_version() is not None else 'Default')}'"
         return header
```

### Comparing `reasoner_validator-3.9.5/reasoner_validator/trapi/mapping.py` & `reasoner_validator-4.0.0/reasoner_validator/trapi/mapping.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     """
     def __init__(self):
         """
         Mapping Validator constructor.
         """
         ValidationReporter.__init__(
             self,
-            prefix="Validating Knowledge Graph Node and Edge Mappings"
+            default_target="Validating Knowledge Graph Node and Edge Mappings"
         )
 
     def check_dangling_references(self, graph: Dict):
         if not ('nodes' in graph and graph['nodes'] and 'edges' in graph and graph['edges']):
             self.report(code="warning.graph.empty", identifier="MappingValidator")
         else:
             pass
```

### Comparing `reasoner_validator-3.9.5/reasoner_validator/validation_codes.py` & `reasoner_validator-4.0.0/reasoner_validator/validation_codes.py`

 * *Files 1% similar despite different names*

```diff
@@ -289,14 +289,16 @@
                 print("# Validation Codes Dictionary\n", file=markdown_file)
                 top_level_tag: str
 
                 for top_level_tag in code_dictionary.keys():
 
                     if top_level_tag == "info":
                         top_level_name = "Information"
+                    elif top_level_tag == "skipped":
+                        top_level_name = "Skipped Test"
                     elif top_level_tag == "critical":
                         top_level_name = "Critical Error"
                     else:
                         top_level_name = top_level_tag.capitalize()
 
                     print(f"## {top_level_name}\n", file=markdown_file)
                     cls._dump_code_markdown_entries(
```

### Comparing `reasoner_validator-3.9.5/reasoner_validator/validator.py` & `reasoner_validator-4.0.0/reasoner_validator/validator.py`

 * *Files 3% similar despite different names*

```diff
@@ -21,40 +21,44 @@
 # Unspoken assumption here is that validation of results returned for
 # Biolink Model release compliance only needs to be superficial
 RESULT_TEST_DATA_SAMPLE_SIZE = 10
 
 
 class TRAPIResponseValidator(BiolinkValidator):
     """
-    TRAPI Validator is an overall wrapper class for validating
-    conformance of TRAPI Responses to TRAPI and the Biolink Model.
+    TRAPIResponseValidator is an overall wrapper class for validating
+    conformance of full TRAPI Responses to TRAPI and the Biolink Model.
     """
     def __init__(
             self,
-            prefix: Optional[str] = None,
+            default_test: Optional[str] = None,
+            default_target: Optional[str] = None,
             trapi_version: Optional[str] = None,
             biolink_version: Optional[str] = None,
             target_provenance: Optional[Dict[str, str]] = None,
             strict_validation: Optional[bool] = None,
             suppress_empty_data_warnings: bool = False
     ):
         """
-        :param prefix: named context of the BiolinkValidator, used as a prefix in validation messages.
+        :param default_test: Optional[str] =  None, initial default test context of the TRAPIResponseValidator messages
+        :param default_target: Optional[str] =  None, initial default target context of the TRAPIResponseValidator,
+                                                also used as a prefix in validation messages.
         :param trapi_version: str, version of component against which to validate the message (mandatory, no default)
         :param biolink_version: Optional[str] = None, Biolink Model (SemVer) release against which the knowledge graph
                                 is to be validated (Default: if None, use the Biolink Model Toolkit default version).
         :param strict_validation: Optional[bool] = None, if True, some tests validate as 'error';  False, simply issues
                                   'info' message; A value of 'None' uses the default value for specific graph contexts.
         :param suppress_empty_data_warnings: bool = False, validation normally reports empty Message query graph,
                                 knowledge graph and results as warnings. This flag suppresses the reporting
                                 of such warnings (default: False).
         """
         BiolinkValidator.__init__(
             self,
-            prefix=prefix if prefix else "Validate TRAPI Response",
+            default_test=default_test,
+            default_target=default_target if default_target else "Validate TRAPI Response",
             trapi_version=trapi_version,
             biolink_version=biolink_version,
             target_provenance=target_provenance,
             strict_validation=strict_validation
         )
         self._is_trapi_1_4: Optional[bool] = None
         self.suppress_empty_data_warnings: bool = suppress_empty_data_warnings
@@ -702,15 +706,15 @@
         #
         # Check in the edges catalog for an edge containing
         # the case 'subject_id', 'predicate' and 'object_id'
         edges: Dict = knowledge_graph["edges"]
 
         bmtw = BMTWrapper(biolink_version=self.biolink_version)
 
-        predicate = case["predicate"]
+        predicate = case["predicate"] if "predicate" in case else case["predicate_id"]
 
         bmt: Optional[Toolkit] = bmtw.get_bmt()
         predicate_descendants: List[str]
         inverse_predicate_descendants: List[str] = list()  # may sometimes remain empty...
         if bmt is not None:
             predicate_descendants = bmt.get_descendants(predicate, formatted=True)
             inverse_predicate = bmtw.get_inverse_predicate(predicate)
```

### Comparing `reasoner_validator-3.9.5/reasoner_validator/versioning.py` & `reasoner_validator-4.0.0/reasoner_validator/versioning.py`

 * *Files identical despite different names*

### Comparing `reasoner_validator-3.9.5/tests/__init__.py` & `reasoner_validator-4.0.0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `reasoner_validator-3.9.5/tests/test_biolink_compliance_validation.py` & `reasoner_validator-4.0.0/tests/test_biolink_compliance_validation.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 
 pp = PrettyPrinter(indent=4)
 
 # January 25, 2023 - as of reasoner-validator 3.1.0,
 # we don't pretend to totally support Biolink Models any earlier than 3.1.1.
 # If earlier biolink model compliance testing is desired,
 # then perhaps reasoner-validator version 3.0.5 or earlier can be used.
-LATEST_BIOLINK_MODEL_VERSION = "3.5.4"
+LATEST_BIOLINK_MODEL_VERSION = Toolkit().get_model_version()
 
 # special case of signalling suppression of validation
 SUPPRESS_BIOLINK_MODEL_VALIDATION = "suppress"
 
 
 def test_set_default_biolink_versioned_global_environment():
     validator = BiolinkValidator()
@@ -66,15 +66,16 @@
     assert validator.minimum_required_biolink_version("2.2.0")
     # 2.2.0 >= 2.4.8 - False!
     assert not validator.minimum_required_biolink_version("2.4.8")
 
 
 def test_message():
     reporter = BiolinkValidator(
-        prefix="Test Message",
+        default_test="Test Message",
+        default_target="Test Reporter",
         trapi_version="v1.3",
         biolink_version=f"v{LATEST_BIOLINK_MODEL_VERSION}"
     )
     assert reporter.get_trapi_version() == "v1.3.0"
 
     # Note: BMT is a bit tricky in resolving Biolink Model versions:
     # the version is reported without the 'v' prefix of the GitHub release!
@@ -90,15 +91,15 @@
     tk: Toolkit = get_biolink_model_toolkit("2.2.0")
     predicate = tk.get_element("biolink:related_to")
     assert predicate['symmetric']
     predicate = tk.get_element("biolink:active_in")
     assert not predicate['symmetric']
     assert isinstance(predicate, SlotDefinition)
     assert not tk.get_inverse(predicate.name)
-    tk: Toolkit = get_biolink_model_toolkit("v2.4.8")
+    tk: Toolkit = get_biolink_model_toolkit("v4.1.4")
     predicate = tk.get_element("biolink:active_in")
     assert not predicate['symmetric']
     assert isinstance(predicate, SlotDefinition)
     assert tk.get_inverse(predicate.name) == "has active component"
 
 
 BLM_VERSION_PREFIX = f"Biolink Validation of"
@@ -400,15 +401,17 @@
                 'object_id': 'GO:0006094'  # Gluconeogenesis
             },
             # f"{INPUT_EDGE_PREFIX}: INFO - Predicate element 'biolink:decreases_amount_or_activity_of' is a mixin."
             "info.input_edge.predicate.mixin"
         )
     ]
 )
-def test_check_biolink_model_non_strict_compliance_of_input_edge(biolink_version: str, edge: Dict, validation_code: str):
+def test_check_biolink_model_non_strict_compliance_of_input_edge(
+        biolink_version: str, edge: Dict, validation_code: str
+):
     validator: BiolinkValidator = BiolinkValidator(biolink_version=biolink_version, strict_validation=False)
     validator.check_biolink_model_compliance_of_input_edge(edge=edge)
     check_messages(validator, validation_code)
 
 
 @pytest.mark.parametrize(
     "biolink_version,graph",
@@ -421,15 +424,15 @@
                     "t_edge": {
                         "attribute_constraints": [],
                         "exclude": None,
                         "knowledge_type": "inferred",
                         "object": "on",
                         "option_group_id": None,
                         "predicates": [
-                            "biolink:treats"
+                            "biolink:ameliorates_condition"
                         ],
                         "qualifier_constraints": [],
                         "subject": "sn"
                     }
                 },
                 "nodes": {
                     "on": {
@@ -464,15 +467,15 @@
                     "drug": {
                         "categories": ["biolink:Drug"]
                     }
                 },
                 "edges": {
                     "treats": {
                         "subject": "drug",
-                        "predicates": ["biolink:treats"],
+                        "predicates": ["biolink:ameliorates_condition"],
                         "object": "type-2 diabetes"
                     }
                 }
             }
         )
     ]
 )
@@ -498,15 +501,15 @@
                     "drug": {
                         "categories": ["biolink:Drug"]
                     }
                 },
                 "edges": {
                     "treats": {
                         "subject": "drug",
-                        "predicates": ["biolink:treats"],
+                        "predicates": ["biolink:ameliorates_condition"],
                         "object": "type-2 diabetes"
                     }
                 }
             },
             ""  # This should pass without errors
         ),
         (
@@ -535,15 +538,15 @@
                     "drug": {},
                     "type-2 diabetes": {}
 
                 },
                 "edges": {
                     "treats": {
                         "subject": "drug",
-                        "predicates": ["biolink:treats"],
+                        "predicates": ["biolink:ameliorates_condition"],
                         "object": "type-2 diabetes"
                     }
                 }
             },
             # At least one QNode needs to be informative
             "error.query_graph.nodes.uninformative"
         ),
@@ -600,15 +603,15 @@
             {
                 "nodes": {
                     "type-2 diabetes": {"ids": []}
                 },
                 "edges":  {
                     "treats": {
                         "subject": "drug",
-                        "predicates": ["biolink:treats"],
+                        "predicates": ["biolink:ameliorates_condition"],
                         "object": "type-2 diabetes"
                     }
                 }
             },
             # although permitted, with the presence of only
             # one node with empty ids, the nodes are uninformative
             "error.query_graph.nodes.uninformative"
@@ -622,15 +625,15 @@
                     "drug": {
                         "categories": ["biolink:Drug"]
                     }
                 },
                 "edges": {
                     "treats": {
                         "subject": "drug",
-                        "predicates": ["biolink:treats"],
+                        "predicates": ["biolink:ameliorates_condition"],
                         "object": "type-2 diabetes"
                     }
                 }
             },
             ""   # this should pass since at least one query node is adequately constrained
         ),
         (
@@ -649,15 +652,15 @@
                            "biolink:OrganismTaxon"
                         ]
                     }
                 },
                 "edges": {
                     "treats": {
                         "subject": "drug",
-                        "predicates": ["biolink:treats"],
+                        "predicates": ["biolink:ameliorates_condition"],
                         "object": "type-2 diabetes"
                     }
                 }
             },
             "warning.query_graph.nodes.dangling"
         ),
         (
@@ -668,15 +671,15 @@
                     "NCBIGene:29974": {
                        "categories": "biolink:Gene"
                     }
                 },
                 "edges": {
                     "treats": {
                         "subject": "drug",
-                        "predicates": ["biolink:treats"],
+                        "predicates": ["biolink:ameliorates_condition"],
                         "object": "type-2 diabetes"
                     }
                 }
             },
             # f"{QUERY_GRAPH_PREFIX}: ERROR - Node 'NCBIGene:29974.categories' slot value is not an array!"
             "error.query_graph.node.categories.not_array"
         ),
@@ -688,15 +691,15 @@
                     "NCBIGene:29974": {
                        "categories": ["biolink:InvalidCategory"]
                     }
                 },
                 "edges": {
                     "treats": {
                         "subject": "drug",
-                        "predicates": ["biolink:treats"],
+                        "predicates": ["biolink:ameliorates_condition"],
                         "object": "type-2 diabetes"
                     }
                 }
             },
             "error.query_graph.node.category.unknown"
         ),
         (
@@ -708,15 +711,15 @@
                     "drug": {
                         "categories": ["biolink:Drug"]
                     }
                 },
                 "edges": {
                     "treats": {
                         "subject": "drug",
-                        # "predicates": ["biolink:treats"],
+                        # "predicates": ["biolink:ameliorates_condition"],
                         "object": "type-2 diabetes"
                     }
                 }
             },
             ""  # Predicates slot can be null... This should pass without errors?
         ),
         (
@@ -728,20 +731,20 @@
                     "drug": {
                         "categories": ["biolink:Drug"]
                     }
                 },
                 "edges": {
                     "treats": {
                         "subject": "drug",
-                        "predicates": "biolink:treats",
+                        "predicates": "biolink:ameliorates_condition",
                         "object": "type-2 diabetes"
                     }
                 }
             },
-            # f"{QUERY_GRAPH_PREFIX}: ERROR - Edge 'drug--biolink:treats->type-2 diabetes' " +
+            # f"{QUERY_GRAPH_PREFIX}: ERROR - Edge 'drug--biolink:ameliorates_condition->type-2 diabetes' " +
             # f"predicate slot value is not an array!"
             "error.query_graph.edge.predicate.not_array"
         ),
         (
             LATEST_BIOLINK_MODEL_VERSION,
             # Query 14: ... but if present, predicates must have at least one predicate in the array
             {
@@ -833,34 +836,34 @@
                     "drug": {
                         "categories": ["biolink:Drug"]
                     },
                     "type-2 diabetes": {"ids": ["MONDO:0005148"]}
                 },
                 "edges": {
                     "treats": {
-                        "predicates": ["biolink:treats"],
+                        "predicates": ["biolink:ameliorates_condition"],
                         "object": "type-2 diabetes"
                     }
                 }
             },
-            # f"{QUERY_GRAPH_PREFIX}: ERROR - Edge 'None--['biolink:treats']->type-2 diabetes' " +
+            # f"{QUERY_GRAPH_PREFIX}: ERROR - Edge 'None--['biolink:ameliorates_condition']->type-2 diabetes' " +
             # "has a missing or empty 'subject' slot value!"
             "error.query_graph.edge.subject.missing"
         ),
         (
             LATEST_BIOLINK_MODEL_VERSION,
             # Query 19: 'Subject' id used in edge is missing from the nodes catalog?
             {
                 "nodes": {
                     "type-2 diabetes": {"ids": ["MONDO:0005148"]}
                 },
                 "edges": {
                     "treats": {
                         "subject": "drug",
-                        "predicates": ["biolink:treats"],
+                        "predicates": ["biolink:ameliorates_condition"],
                         "object": "type-2 diabetes"
                     }
                 }
             },
             # f"{QUERY_GRAPH_PREFIX}: ERROR - Edge 'subject' id 'drug' is missing from the nodes catalog!"
             "error.query_graph.edge.subject.missing_from_nodes"
         ),
@@ -873,19 +876,19 @@
                         "categories": ["biolink:Drug"]
                     },
                     "type-2 diabetes": {"ids": ["MONDO:0005148"]}
                 },
                 "edges": {
                     "treats": {
                         "subject": "drug",
-                        "predicates": ["biolink:treats"]
+                        "predicates": ["biolink:ameliorates_condition"]
                     }
                 }
             },
-            # f"{QUERY_GRAPH_PREFIX}: ERROR - Edge 'drug--['biolink:treats']->None' " +
+            # f"{QUERY_GRAPH_PREFIX}: ERROR - Edge 'drug--['biolink:ameliorates_condition']->None' " +
             # f"has a missing or empty 'object' slot value!"
             "error.query_graph.edge.object.missing"
         ),
         (
             LATEST_BIOLINK_MODEL_VERSION,
             # Query 21: 'Object' id used in edge is missing from the nodes catalog?
             {
@@ -893,15 +896,15 @@
                     "drug": {
                         "categories": ["biolink:Drug"]
                     }
                 },
                 "edges": {
                     "treats": {
                         "subject": "drug",
-                        "predicates": ["biolink:treats"],
+                        "predicates": ["biolink:ameliorates_condition"],
                         "object": "type-2 diabetes"
                     }
                 }
             },
             # f"{QUERY_GRAPH_PREFIX}: ERROR - Edge 'object' id 'type-2 diabetes' is missing from the nodes catalog!"
             "error.query_graph.edge.object.missing_from_nodes"
         ),
@@ -915,15 +918,15 @@
                         "categories": ["biolink:Drug"],
                         "is_set": "should-be-a-boolean"
                     }
                 },
                 "edges": {
                     "treats": {
                         "subject": "drug",
-                        "predicates": ["biolink:treats"],
+                        "predicates": ["biolink:ameliorates_condition"],
                         "object": "type-2 diabetes"
                     }
                 }
             },
             # f"{QUERY_GRAPH_PREFIX}: ERROR - Node 'drug.is_set' slot is not a boolean value!"
             "error.query_graph.node.is_set.not_boolean"
         ),
@@ -939,15 +942,15 @@
                     "drug": {
                         "categories": ["biolink:Drug"]
                     }
                 },
                 "edges": {
                     "treats": {
                         "subject": "drug",
-                        "predicates": ["biolink:treats"],
+                        "predicates": ["biolink:ameliorates_condition"],
                         "object": "type-2 diabetes"
                     }
                 }
             },
             # f"{QUERY_GRAPH_PREFIX}: WARNING - Node 'type-2 diabetes' has identifiers ['FOO:12345', 'BAR:67890'] " +
             # "unmapped to the target categories: ['biolink:Disease', 'biolink:Gene']?"
             "warning.query_graph.node.ids.unmapped_prefix"
@@ -961,15 +964,15 @@
                     "drug": {
                         "categories": ["biolink:BiologicalEntity"]
                     }
                 },
                 "edges": {
                     "treats": {
                         "subject": "drug",
-                        "predicates": ["biolink:treats"],
+                        "predicates": ["biolink:ameliorates_condition"],
                         "object": "type-2 diabetes"
                     }
                 }
             },
             ""
         ),
         (
@@ -981,15 +984,15 @@
                     "drug": {
                         "categories": ["biolink:ChemicalOrDrugOrTreatment"]
                     }
                 },
                 "edges": {
                     "treats": {
                         "subject": "drug",
-                        "predicates": ["biolink:treats"],
+                        "predicates": ["biolink:ameliorates_condition"],
                         "object": "type-2 diabetes"
                     }
                 }
             },
             ""
         ),
         (
@@ -3449,15 +3452,15 @@
     "resource_id": "infores:chebi",
 
     # required, string drawn from the TRAPI ResourceRoleEnum
     # values that were formerly recorded as TRAPI attributes
     # are now presented as first class edge annotation
     "resource_role": "primary_knowledge_source",
 
-    # nothing upstream... it' primary!
+    # nothing upstream... it's primary!
     "upstream_resource_ids": []
 }
 
 SAMPLE_KP_RETRIEVAL_SOURCE = {
     # required, infores CURIE to an Information Resource
     "resource_id": "infores:molepro",
 
@@ -3582,22 +3585,22 @@
         # TODO: need method to determine if an infores is known with recent changes to BMT
         # (
         #     [SAMPLE_RETRIEVAL_SOURCE_RESOURCE_ID_INFORES_UNKNOWN],
         #     "error.knowledge_graph.edge.sources.retrieval_source.resource_id.infores.unknown"
         # )
     ]
 )
-def test_latest_trapi_validate_sources(sources: bool, validation_code: str):
+def test_latest_trapi_validate_sources(sources: List[Dict], validation_code: str):
     # no attributes are strictly needed in 1.4.0-beta now that (mandatory)
     # Edge provenance is recorded in the Edge.sources list of RetrievalSource
     # message edges must have at least some 'provenance' attributes
-    sample_message = deepcopy(MESSAGE_EDGE_WITHOUT_ATTRIBUTES)
+    sample_message: Dict = deepcopy(MESSAGE_EDGE_WITHOUT_ATTRIBUTES)
     if sources is not None:
-        edge = sample_message["edges"]["edge_1"]
-        edge["sources"] = sources
+        edge: Dict = sample_message["edges"]["edge_1"]
+        edge["sources"]: List[Dict] = sources
     validator = BiolinkValidator(biolink_version=LATEST_BIOLINK_MODEL_VERSION)
     validator.check_biolink_model_compliance(graph=sample_message, graph_type=TRAPIGraphType.Knowledge_Graph)
     check_messages(validator, validation_code)
 
 
 @pytest.mark.parametrize(
     "predicate,result",
```

### Comparing `reasoner_validator-3.9.5/tests/test_data/patched_trapi_schema_v1.4.0-beta5.yaml` & `reasoner_validator-4.0.0/tests/test_data/patched_trapi_schema_v1.4.0-beta5.yaml`

 * *Files identical despite different names*

### Comparing `reasoner_validator-3.9.5/tests/test_response_validator.py` & `reasoner_validator-4.0.0/tests/test_response_validator.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 """
 Unit tests for the generic (shared) components of the SRI Testing Framework
 """
-from typing import  Dict
+from typing import Dict
 from sys import stderr
 
 import logging
 
-from json import dump
-
 from copy import deepcopy
 
 import pytest
 
 from dictdiffer import diff
 
 from reasoner_validator.trapi import TRAPI_1_3_0, TRAPI_1_4_2
@@ -31,15 +29,15 @@
         "drug": {
             "categories": ["biolink:Drug"]
         }
     },
     "edges": {
         "treats": {
             "subject": "drug",
-            "predicates": ["biolink:treats"],
+            "predicates": ["biolink:ameliorates_condition"],
             "object": "type-2 diabetes"
         }
     }
 }
 
 # Sample edge 1
 _TEST_EDGES_1 = {
@@ -212,27 +210,27 @@
     "message": {
         "query_graph": {
             "nodes": {
                 "type-2 diabetes": {"ids": ["MONDO:0005148"]},
                 "drug": {"categories": ["biolink:Drug"]}
             },
             "edges": {
-                "treats": {"subject": "drug", "predicates": ["biolink:treats"],
+                "treats": {"subject": "drug", "predicates": ["biolink:ameliorates_condition"],
                            "object": "type-2 diabetes"}
             }
         },
         "knowledge_graph": {
             "nodes": {
                 "MONDO:0005148": {"name": "type-2 diabetes", "categories": ["biolink:Disease"]},
                 "ncats.drug:9100L32L2N": {"name": "metformin", "categories": ["biolink:Drug"]}
             },
             "edges": {
                 "df87ff82": {
                     "subject": "ncats.drug:9100L32L2N",
-                    "predicate": "biolink:treats",
+                    "predicate": "biolink:ameliorates_condition",
                     "object": "MONDO:0005148",
                     "sources": [
                         {
                             "resource_id": "infores:chebi",
                             "resource_role": "primary_knowledge_source",
                             "upstream_resource_ids": []
                         },
@@ -297,21 +295,110 @@
         ]
     }
 }
 
 _TEST_TRAPI_1_4_2_FULL_SAMPLE_WITHOUT_AUX_GRAPH = deepcopy(_TEST_TRAPI_1_4_2_FULL_SAMPLE)
 _TEST_TRAPI_1_4_2_FULL_SAMPLE_WITHOUT_AUX_GRAPH["message"].pop("auxiliary_graphs")
 
-# original TRAPI schema.. changing the 'schema_version' may generate errors
 _TEST_TRAPI_1_4_2_FULL_SAMPLE_WITH_SCHEMA_VERSION = deepcopy(_TEST_TRAPI_1_4_2_FULL_SAMPLE)
 _TEST_TRAPI_1_4_2_FULL_SAMPLE_WITH_SCHEMA_VERSION["schema_version"] = "1.3.0"
 
-# original TRAPI schema.. changing the 'biolink_version' may generate errors
-_TEST_TRAPI_1_4_2_FULL_SAMPLE_WITH_BIOLINK_VERSION = deepcopy(_TEST_TRAPI_1_4_2_FULL_SAMPLE)
-_TEST_TRAPI_1_4_2_FULL_SAMPLE_WITH_BIOLINK_VERSION["biolink_version"] = "2.4.8"
+_TEST_TRAPI_1_4_2_FULL_SAMPLE_WITH_BIOLINK_VERSION = {
+    "biolink_version": "2.2.0",
+    "message": {
+        "query_graph": {
+            "nodes": {
+                "type-2 diabetes": {"ids": ["MONDO:0005148"]},
+                "drug": {"categories": ["biolink:Drug"]}
+            },
+            "edges": {
+                "treats": {
+                    "subject": "type-2 diabetes",
+                    "predicates": ["biolink:treated_by"],
+                    "object": "drug"
+                }
+            }
+        },
+        "knowledge_graph": {
+            "nodes": {
+                "MONDO:0005148": {"name": "type-2 diabetes", "categories": ["biolink:Disease"]},
+                "ncats.drug:9100L32L2N": {"name": "metformin", "categories": ["biolink:Drug"]}
+            },
+            "edges": {
+                "df87ff82": {
+                    "subject": "MONDO:0005148",
+                    "predicate": "biolink:treated_by",
+                    "object": "ncats.drug:9100L32L2N",
+                    "sources": [
+                        {
+                            "resource_id": "infores:chebi",
+                            "resource_role": "primary_knowledge_source",
+                            "upstream_resource_ids": []
+                        },
+                        {
+                            "resource_id": "infores:biothings-explorer",
+                            "resource_role": "aggregator_knowledge_source",
+                            "upstream_resource_ids": [
+                                "infores:chebi"
+                            ]
+                        },
+                        {
+                            "resource_id": "infores:molepro",
+                            "resource_role": "aggregator_knowledge_source",
+                            "upstream_resource_ids": [
+                                "infores:biothings-explorer"
+                            ]
+                        },
+                        {
+                            "resource_id": "infores:arax",
+                            "resource_role": "aggregator_knowledge_source",
+                            "upstream_resource_ids": [
+                                "infores:molepro"
+                            ]
+                        }
+                    ]
+                }
+            }
+        },
+        "auxiliary_graphs": {
+            "a0": {
+                "edges": [
+                    "e02",
+                    "e12"
+                ]
+            },
+            "a1": {
+                "edges": [
+                    "extra_edge0"
+                ]
+            },
+            "a2": {
+                "edges": [
+                    "extra_edge1"
+                ]
+            }
+        },
+        "results": [
+            {
+                "node_bindings": {
+                    "type-2 diabetes": [{"id": "MONDO:0005148"}],
+                    "drug": [{"id": "ncats.drug:9100L32L2N"}]
+                },
+                "analyses": [
+                    {
+                        "resource_id": "infores:ara0",
+                        "edge_bindings": {"treats": [{"id": "df87ff82"}]},
+                        "support_graphs": [],
+                        "score": 0.7
+                    }
+                ]
+            }
+        ]
+    }
+}
 
 NUM_SAMPLE_NODES = 5
 
 SAMPLE_NODES: Dict = dict()
 for node_id in range(1, NUM_SAMPLE_NODES):
     SAMPLE_NODES[f"n{node_id}"] = dict()
 
@@ -892,15 +979,15 @@
             True,
             ""   # this filtered workflow spec should pass
         ),
         (   # Query 27 - We throw a full TRAPI JSON example here (taken directly from the TRAPI implementation
             #            guidelines...) but add the 'schema_version' just for fun and profit
             _TEST_TRAPI_1_4_2_FULL_SAMPLE_WITH_SCHEMA_VERSION,
             None,
-            "3.0.0",
+            "4.1.4",
             None,
             True,
             "critical.trapi.validation"   # trying to validate a 1.4.2 schema against 1.3.0 will fail!
         ),
         (   # Query 28 - We throw a full TRAPI JSON example here (taken directly from the TRAPI implementation
             #            guidelines...) but explicitly specify the 'biolink_version == 2.5.8' just for fun and profit
             _TEST_TRAPI_1_4_2_FULL_SAMPLE_WITH_BIOLINK_VERSION,
@@ -1113,8 +1200,9 @@
         _TEST_TRAPI_1_4_2_FULL_SAMPLE,
         _TEST_TRAPI_1_4_2_FULL_SAMPLE_WITH_REPORTABLE_ERRORS
     ]
 )
 def test_dump_report_of_biolink_model_compliance_of_trapi_response_with_errors(response: Dict):
     validator: TRAPIResponseValidator = TRAPIResponseValidator()
     validator.check_compliance_of_trapi_response(response=response)
-    validator.dump()
+    validator.dump(file=stderr)
+    print("\n"+"="*80+"\n", file=stderr)
```

### Comparing `reasoner_validator-3.9.5/tests/test_semver.py` & `reasoner_validator-4.0.0/tests/test_semver.py`

 * *Files identical despite different names*

### Comparing `reasoner_validator-3.9.5/tests/test_trapi_versioning.py` & `reasoner_validator-4.0.0/tests/test_trapi_versioning.py`

 * *Files identical despite different names*

### Comparing `reasoner_validator-3.9.5/tests/test_validate.py` & `reasoner_validator-4.0.0/tests/test_validate.py`

 * *Files 1% similar despite different names*

```diff
@@ -87,15 +87,19 @@
 def test_load_master_schema():
     """Test load_schema('master')."""
     schema = load_schema("master")
     assert schema, "TRAPI Schema for ('master') branch is not available?"
 
 
 def test_message():
-    reporter = TRAPISchemaValidator(prefix="Test Message", trapi_version="v1.4")
+    reporter = TRAPISchemaValidator(
+        default_test="test_message",
+        default_target="Test Message",
+        trapi_version="v1.4"
+    )
     assert reporter.get_trapi_version() == LATEST_TRAPI_RELEASE
     assert not reporter.has_messages()
     reporter.report("info.compliant")
     assert reporter.has_messages()
     reporter.dump()
```

### Comparing `reasoner_validator-3.9.5/tests/test_workflows.py` & `reasoner_validator-4.0.0/tests/test_workflows.py`

 * *Files identical despite different names*

### Comparing `reasoner_validator-3.9.5/PKG-INFO` & `reasoner_validator-4.0.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: reasoner-validator
-Version: 3.9.5
+Version: 4.0.0
 Summary: Validation tools for Reasoner API
 Home-page: https://github.com/NCATSTranslator
 License: MIT
 Keywords: NCATS,Biomedical Data Translator,Translator,ReasonerAPI,TRAPI,validation,Biolink Model
 Author: Richard Bruskiewich
 Author-email: richard.bruskiewich@delphinai.com
 Maintainer: Richard Bruskiewich
@@ -97,15 +97,15 @@
 poetry install --all-extras
 ```
 
 ## Running Validation against an ARS UUID Result(*) or using a Local TRAPI Request Query
 
 A local script **`trapi_validator.py`** is available to run TRAPI Response validation against either a PK (UUID)
 indexed query result of the Biomedical Knowledge Translator "Autonomous Relay System" (ARS), a local JSON Response
-text file or a locally triggered _ad hoc_ query Request against an directly specified TRAPI endpoint.
+text file or a locally triggered _ad hoc_ query Request against a directly specified TRAPI endpoint.
 
 Note that it is best run within a **`poetry shell`** created by **`poetry install`**.
 
 For script usage, type:
 
 ```bash
 ./trapi_validator.py --help
@@ -228,16 +228,16 @@
 
 ### Typical Output
 
 As an example of the kind of output to expect, if one posts the following TRAPI Response JSON data structure to the **/validate** endpoint:
 
 ```json
 {
-  "trapi_version": "1.4.1",
-  "biolink_version": "3.5.0",
+  "trapi_version": "1.4.2",
+  "biolink_version": "4.1.5",
   "response": {
       "message": {
         "query_graph": {
             "nodes": {
                 "type-2 diabetes": {"ids": ["MONDO:0005148"]},
                 "drug": {"categories": ["biolink:Drug"]}
             },
@@ -271,55 +271,59 @@
 }
 ```
 
 one should typically get a response body something like the following JSON validation result back:
 
 ```json
 {
-  "trapi_version": "1.4.1",
-  "biolink_version": "3.2.1",
   "messages": {
-    "_comment": "some categories of messages may be absent, hence, empty dictionaries",
-    "critical": {},
-    "errors": {
-      "error.knowledge_graph.node.category.missing": {
-          "_comment": "source scope of the validation error ('global' or some knowledge source path string)",
-          "global": {
-              "_comment": "this message template does not have any additional parameters other than identifier hence it just has the unique identifier  value as a dictionary key, with associated value None",
-               "MONDO:0005148": null            
+    "Validate TRAPI Response": {
+      "Standards Test": {
+        "info": {
+          "info.query_graph.edge.predicate.mixin": {
+            "global": {
+              "biolink:treats": [
+                {
+                  "edge_id": "drug[biolink:Drug]--['biolink:treats']->type-2 diabetes[None]"
+                }
+              ]
+            }
           }
-        }
-    },
-    "warnings": {
-      "_comment": "validation code",
-      "warning.knowledge_graph.node.unmapped_prefix": {
-          "global": {
-              "_comment": "template identifier field value",
-              "CHEBI:6801": [  
-                  {
-                    "_comment": "additional message template field values, if applicable",
-                    "categories": "['biolink:Drug']"  
-                  }
-              ]       
+        },
+        "skipped": {},
+        "warning": {},
+        "error": {
+          "error.query_graph.edge.predicate.invalid": {
+            "global": {
+              "biolink:treats": [
+                {
+                  "edge_id": "drug[biolink:Drug]--['biolink:treats']->type-2 diabetes[None]"
+                }
+              ]
+            }
           }
-
-        }
-    },
-    "information": {},
-  }
+        },
+        "critical": {}
+      }
+    }
+  },
+  "trapi_version": "v1.4.2",
+  "biolink_version": "4.1.5"
 }
 ```
 
 To minimize redundancy in validation messages, messages are uniquely indexed in dictionaries at two levels:
 
 1. the (codes.yaml recorded) dot-delimited validation code path string
 2. for messages with templated parameters, by a mandatory 'identifier' field (which is expected to exist as a field in a template if such template has one or more parameterized fields)
 
 ### OpenTelemetry and Jaeger
 
+NOTE: OpenTelemetry is temporarily disabled in this code release (to be updated later)
+
 The web service may be monitored for OpenTelemetry by setting an environment variable **TELEMETRY_ENDPOINT**  to a suitable trace collecting endpoint in an application like [Jaeger](https://www.jaegertracing.io/) (see also the [Translator SRI Jaeger-Demo](https://github.com/TranslatorSRI/Jaeger-demo)).
 
 **Note:** the current system Docker (Compose) design only supports OpenTemplate tracing using the internal Jaeger container and may require further refinements to enable use of an external telemetry collector.
 
 ### Running the Web Service within Docker
 
 The Reasoner Validator web service may be run inside a docker container, using Docker Compose.
```

