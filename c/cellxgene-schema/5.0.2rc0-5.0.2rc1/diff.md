# Comparing `tmp/cellxgene-schema-5.0.2rc0.tar.gz` & `tmp/cellxgene-schema-5.0.2rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cellxgene-schema-5.0.2rc0.tar", last modified: Mon Apr  1 17:15:07 2024, max compression
+gzip compressed data, was "cellxgene-schema-5.0.2rc1.tar", last modified: Tue Apr  2 16:52:52 2024, max compression
```

## Comparing `cellxgene-schema-5.0.2rc0.tar` & `cellxgene-schema-5.0.2rc1.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 ngloria    (502) staff       (20)        0 2024-04-01 17:15:07.762824 cellxgene-schema-5.0.2rc0/
--rw-r--r--   0 ngloria    (502) staff       (20)     1098 2022-06-09 16:50:04.000000 cellxgene-schema-5.0.2rc0/LICENSE.txt
--rw-r--r--   0 ngloria    (502) staff       (20)      174 2022-09-27 19:46:36.000000 cellxgene-schema-5.0.2rc0/MANIFEST.in
--rw-r--r--   0 ngloria    (502) staff       (20)      723 2024-04-01 17:15:07.762894 cellxgene-schema-5.0.2rc0/PKG-INFO
-drwxr-xr-x   0 ngloria    (502) staff       (20)        0 2024-04-01 17:15:07.761082 cellxgene-schema-5.0.2rc0/cellxgene_schema/
--rw-r--r--   0 ngloria    (502) staff       (20)       27 2024-04-01 17:07:52.000000 cellxgene-schema-5.0.2rc0/cellxgene_schema/__init__.py
--rw-r--r--   0 ngloria    (502) staff       (20)     3902 2024-04-01 17:05:13.000000 cellxgene-schema-5.0.2rc0/cellxgene_schema/cli.py
--rw-r--r--   0 ngloria    (502) staff       (20)      493 2024-04-01 17:07:52.000000 cellxgene-schema-5.0.2rc0/cellxgene_schema/env.py
--rw-r--r--   0 ngloria    (502) staff       (20)     3304 2024-04-01 17:07:52.000000 cellxgene-schema-5.0.2rc0/cellxgene_schema/gencode.py
--rw-r--r--   0 ngloria    (502) staff       (20)    14201 2024-04-01 17:07:43.000000 cellxgene-schema-5.0.2rc0/cellxgene_schema/migrate.py
--rw-r--r--   0 ngloria    (502) staff       (20)     2774 2023-09-14 14:21:43.000000 cellxgene-schema-5.0.2rc0/cellxgene_schema/remove_labels.py
--rw-r--r--   0 ngloria    (502) staff       (20)      522 2023-09-14 14:21:43.000000 cellxgene-schema-5.0.2rc0/cellxgene_schema/schema.py
-drwxr-xr-x   0 ngloria    (502) staff       (20)        0 2024-04-01 17:15:07.762441 cellxgene-schema-5.0.2rc0/cellxgene_schema/schema_definitions/
--rw-r--r--   0 ngloria    (502) staff       (20)    28901 2024-02-08 20:49:38.000000 cellxgene-schema-5.0.2rc0/cellxgene_schema/schema_definitions/schema_definition.yaml
--rw-r--r--   0 ngloria    (502) staff       (20)     6738 2024-03-14 20:00:30.000000 cellxgene-schema-5.0.2rc0/cellxgene_schema/utils.py
--rw-r--r--   0 ngloria    (502) staff       (20)    63307 2024-04-01 17:07:52.000000 cellxgene-schema-5.0.2rc0/cellxgene_schema/validate.py
--rw-r--r--   0 ngloria    (502) staff       (20)    15528 2024-04-01 17:07:52.000000 cellxgene-schema-5.0.2rc0/cellxgene_schema/write_labels.py
-drwxr-xr-x   0 ngloria    (502) staff       (20)        0 2024-04-01 17:15:07.762296 cellxgene-schema-5.0.2rc0/cellxgene_schema.egg-info/
--rw-r--r--   0 ngloria    (502) staff       (20)      723 2024-04-01 17:15:07.000000 cellxgene-schema-5.0.2rc0/cellxgene_schema.egg-info/PKG-INFO
--rw-r--r--   0 ngloria    (502) staff       (20)      681 2024-04-01 17:15:07.000000 cellxgene-schema-5.0.2rc0/cellxgene_schema.egg-info/SOURCES.txt
--rw-r--r--   0 ngloria    (502) staff       (20)        1 2024-04-01 17:15:07.000000 cellxgene-schema-5.0.2rc0/cellxgene_schema.egg-info/dependency_links.txt
--rw-r--r--   0 ngloria    (502) staff       (20)       70 2024-04-01 17:15:07.000000 cellxgene-schema-5.0.2rc0/cellxgene_schema.egg-info/entry_points.txt
--rw-r--r--   0 ngloria    (502) staff       (20)        1 2023-12-13 19:01:56.000000 cellxgene-schema-5.0.2rc0/cellxgene_schema.egg-info/not-zip-safe
--rw-r--r--   0 ngloria    (502) staff       (20)      176 2024-04-01 17:15:07.000000 cellxgene-schema-5.0.2rc0/cellxgene_schema.egg-info/requires.txt
--rw-r--r--   0 ngloria    (502) staff       (20)       17 2024-04-01 17:15:07.000000 cellxgene-schema-5.0.2rc0/cellxgene_schema.egg-info/top_level.txt
--rw-r--r--   0 ngloria    (502) staff       (20)      176 2024-04-01 17:07:52.000000 cellxgene-schema-5.0.2rc0/requirements.txt
--rw-r--r--   0 ngloria    (502) staff       (20)       70 2024-04-01 17:15:07.763159 cellxgene-schema-5.0.2rc0/setup.cfg
--rw-r--r--   0 ngloria    (502) staff       (20)     1229 2024-04-01 17:07:52.000000 cellxgene-schema-5.0.2rc0/setup.py
+drwxr-xr-x   0 ngloria    (502) staff       (20)        0 2024-04-02 16:52:52.517512 cellxgene-schema-5.0.2rc1/
+-rw-r--r--   0 ngloria    (502) staff       (20)     1098 2022-06-09 16:50:04.000000 cellxgene-schema-5.0.2rc1/LICENSE.txt
+-rw-r--r--   0 ngloria    (502) staff       (20)      174 2022-09-27 19:46:36.000000 cellxgene-schema-5.0.2rc1/MANIFEST.in
+-rw-r--r--   0 ngloria    (502) staff       (20)      723 2024-04-02 16:52:52.517617 cellxgene-schema-5.0.2rc1/PKG-INFO
+drwxr-xr-x   0 ngloria    (502) staff       (20)        0 2024-04-02 16:52:52.515313 cellxgene-schema-5.0.2rc1/cellxgene_schema/
+-rw-r--r--   0 ngloria    (502) staff       (20)       27 2024-04-02 16:52:21.000000 cellxgene-schema-5.0.2rc1/cellxgene_schema/__init__.py
+-rw-r--r--   0 ngloria    (502) staff       (20)     3902 2024-04-02 16:42:30.000000 cellxgene-schema-5.0.2rc1/cellxgene_schema/cli.py
+-rw-r--r--   0 ngloria    (502) staff       (20)      493 2024-04-02 16:44:16.000000 cellxgene-schema-5.0.2rc1/cellxgene_schema/env.py
+-rw-r--r--   0 ngloria    (502) staff       (20)     3304 2024-04-02 16:44:16.000000 cellxgene-schema-5.0.2rc1/cellxgene_schema/gencode.py
+-rw-r--r--   0 ngloria    (502) staff       (20)    14201 2024-04-02 16:42:30.000000 cellxgene-schema-5.0.2rc1/cellxgene_schema/migrate.py
+-rw-r--r--   0 ngloria    (502) staff       (20)     2774 2023-09-14 14:21:43.000000 cellxgene-schema-5.0.2rc1/cellxgene_schema/remove_labels.py
+-rw-r--r--   0 ngloria    (502) staff       (20)      522 2023-09-14 14:21:43.000000 cellxgene-schema-5.0.2rc1/cellxgene_schema/schema.py
+drwxr-xr-x   0 ngloria    (502) staff       (20)        0 2024-04-02 16:52:52.516971 cellxgene-schema-5.0.2rc1/cellxgene_schema/schema_definitions/
+-rw-r--r--   0 ngloria    (502) staff       (20)    28970 2024-04-02 16:44:21.000000 cellxgene-schema-5.0.2rc1/cellxgene_schema/schema_definitions/schema_definition.yaml
+-rw-r--r--   0 ngloria    (502) staff       (20)     6738 2024-03-14 20:00:30.000000 cellxgene-schema-5.0.2rc1/cellxgene_schema/utils.py
+-rw-r--r--   0 ngloria    (502) staff       (20)    63353 2024-04-02 16:44:21.000000 cellxgene-schema-5.0.2rc1/cellxgene_schema/validate.py
+-rw-r--r--   0 ngloria    (502) staff       (20)    15528 2024-04-02 16:44:16.000000 cellxgene-schema-5.0.2rc1/cellxgene_schema/write_labels.py
+drwxr-xr-x   0 ngloria    (502) staff       (20)        0 2024-04-02 16:52:52.516772 cellxgene-schema-5.0.2rc1/cellxgene_schema.egg-info/
+-rw-r--r--   0 ngloria    (502) staff       (20)      723 2024-04-02 16:52:52.000000 cellxgene-schema-5.0.2rc1/cellxgene_schema.egg-info/PKG-INFO
+-rw-r--r--   0 ngloria    (502) staff       (20)      681 2024-04-02 16:52:52.000000 cellxgene-schema-5.0.2rc1/cellxgene_schema.egg-info/SOURCES.txt
+-rw-r--r--   0 ngloria    (502) staff       (20)        1 2024-04-02 16:52:52.000000 cellxgene-schema-5.0.2rc1/cellxgene_schema.egg-info/dependency_links.txt
+-rw-r--r--   0 ngloria    (502) staff       (20)       70 2024-04-02 16:52:52.000000 cellxgene-schema-5.0.2rc1/cellxgene_schema.egg-info/entry_points.txt
+-rw-r--r--   0 ngloria    (502) staff       (20)        1 2023-12-13 19:01:56.000000 cellxgene-schema-5.0.2rc1/cellxgene_schema.egg-info/not-zip-safe
+-rw-r--r--   0 ngloria    (502) staff       (20)      176 2024-04-02 16:52:52.000000 cellxgene-schema-5.0.2rc1/cellxgene_schema.egg-info/requires.txt
+-rw-r--r--   0 ngloria    (502) staff       (20)       17 2024-04-02 16:52:52.000000 cellxgene-schema-5.0.2rc1/cellxgene_schema.egg-info/top_level.txt
+-rw-r--r--   0 ngloria    (502) staff       (20)      176 2024-04-02 16:44:16.000000 cellxgene-schema-5.0.2rc1/requirements.txt
+-rw-r--r--   0 ngloria    (502) staff       (20)       70 2024-04-02 16:52:52.518251 cellxgene-schema-5.0.2rc1/setup.cfg
+-rw-r--r--   0 ngloria    (502) staff       (20)     1229 2024-04-02 16:52:21.000000 cellxgene-schema-5.0.2rc1/setup.py
```

### Comparing `cellxgene-schema-5.0.2rc0/LICENSE.txt` & `cellxgene-schema-5.0.2rc1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `cellxgene-schema-5.0.2rc0/PKG-INFO` & `cellxgene-schema-5.0.2rc1/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cellxgene-schema
-Version: 5.0.2rc0
+Version: 5.0.2rc1
 Summary: Tool for applying and validating cellxgene integration schema to single cell datasets
 Home-page: https://github.com/chanzuckerberg/single-cell-curation
 Author: Chan Zuckerberg Initiative
 Author-email: cellxgene@chanzuckerberg.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Intended Audience :: Science/Research
```

### Comparing `cellxgene-schema-5.0.2rc0/cellxgene_schema/cli.py` & `cellxgene-schema-5.0.2rc1/cellxgene_schema/cli.py`

 * *Files identical despite different names*

### Comparing `cellxgene-schema-5.0.2rc0/cellxgene_schema/gencode.py` & `cellxgene-schema-5.0.2rc1/cellxgene_schema/gencode.py`

 * *Files identical despite different names*

### Comparing `cellxgene-schema-5.0.2rc0/cellxgene_schema/migrate.py` & `cellxgene-schema-5.0.2rc1/cellxgene_schema/migrate.py`

 * *Files identical despite different names*

### Comparing `cellxgene-schema-5.0.2rc0/cellxgene_schema/remove_labels.py` & `cellxgene-schema-5.0.2rc1/cellxgene_schema/remove_labels.py`

 * *Files identical despite different names*

### Comparing `cellxgene-schema-5.0.2rc0/cellxgene_schema/schema.py` & `cellxgene-schema-5.0.2rc1/cellxgene_schema/schema.py`

 * *Files identical despite different names*

### Comparing `cellxgene-schema-5.0.2rc0/cellxgene_schema/schema_definitions/schema_definition.yaml` & `cellxgene-schema-5.0.2rc1/cellxgene_schema/schema_definitions/schema_definition.yaml`

 * *Files 3% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 sparsity: 0.5
 # If the R array will exceed this number in size, then Seurat conversion will fail
 max_size_for_seurat: 2147483647  # 2^31 - 1 (max value for 4-byte signed int)
 # Perform the checks for "raw" requirements IF:
 raw:
     obs:
         assay_ontology_term_id:
-                not_children_of:
+                not_descendants_of:
                     EFO:
                         - EFO:0007045 # ATAC-seq
                         - EFO:0008804 # Methyl-seq
                         - EFO:0000751 # methylation profiling
                         - EFO:0008939 # snmC-seq
 components:
     uns:
@@ -126,30 +126,30 @@
                             - CL:0000548
                 add_labels:
                     -
                         type: curie
                         to_column: cell_type
             assay_ontology_term_id:
                 error_message_suffix: >-
-                    Only children terms of either 'EFO:0002772' or 'EFO:0010183' are allowed for assay_ontology_term_id
+                    Only descendant terms of either 'EFO:0002772' or 'EFO:0010183' are allowed for assay_ontology_term_id
                 type: curie
                 curie_constraints:
                     ontologies:
                         - EFO
                     allowed:
                         ancestors:
                             EFO:
                                 - EFO:0002772
                                 - EFO:0010183
                 add_labels:
                     -
                         type: curie
                         to_column: assay
             disease_ontology_term_id:
-                error_message_suffix: "Only 'PATO:0000461' (normal), 'MONDO:0021178' (injury) or children terms thereof, or children terms of 'MONDO:0000001' (disease) are allowed"
+                error_message_suffix: "Only 'PATO:0000461' (normal), 'MONDO:0021178' (injury) or descendant terms thereof, or descendant terms of 'MONDO:0000001' (disease) are allowed"
                 type: curie
                 curie_constraints:
                     ontologies:
                         - MONDO
                         - PATO
                     allowed:
                         terms:
@@ -163,15 +163,15 @@
                                 - MONDO:0021178
                 add_labels:
                     -
                         type: curie
                         to_column: disease
             organism_ontology_term_id:
                 type: curie
-                error_message_suffix: "Only children term ids of 'NCBITaxon:33208' for metazoan are allowed."
+                error_message_suffix: "Only descendant term ids of 'NCBITaxon:33208' for metazoan are allowed."
                 curie_constraints:
                     ontologies:
                         - NCBITaxon
                 add_labels:
                     -
                         type: curie
                         to_column: organism
@@ -197,15 +197,15 @@
                 type: curie
                 dependencies:
                     -
                         # If tissue_type is tissue OR organoid
                         rule: "tissue_type == 'tissue' | tissue_type == 'organoid'"
                         error_message_suffix: >-
                             When 'tissue_type' is 'tissue' or 'organoid',
-                            'tissue_ontology_term_id' MUST be a child term id of 'UBERON:0001062' (anatomical entity).
+                            'tissue_ontology_term_id' MUST be a descendant term id of 'UBERON:0001062' (anatomical entity).
                         type: curie
                         curie_constraints:
                             ontologies:
                                 - UBERON
                             allowed:
                                 ancestors:
                                     UBERON:
@@ -323,15 +323,15 @@
                             ontologies:
                                 - MmusDv
                             exceptions:
                                 - unknown
                 # If organism is not humnan nor mouse
                 error_message_suffix: >-
                     When 'organism_ontology_term_id' is not 'NCBITaxon:10090' nor 'NCBITaxon:9606',
-                    'development_stage_ontology_term_id' MUST be a child term id of 'UBERON:0000105'
+                    'development_stage_ontology_term_id' MUST be a descendant term id of 'UBERON:0000105'
                     excluding 'UBERON:0000071', or unknown.
                 curie_constraints:
                     ontologies:
                         - UBERON
                     allowed:
                         ancestors:
                             UBERON:
@@ -361,125 +361,125 @@
                 # if no dependencies are matched
                 warning_message: >-
                     Data contains assay(s) that are not represented in the 'suspension_type' schema definition table. Ensure you have
                     selected the most appropriate value for the assay(s) between 'cell', 'nucleus', and 'na'. Please contact cellxgene@chanzuckerberg.com
                     during submission so that the assay(s) can be added to the schema definition document.
                 dependencies:
                     -
-                        # If assay_ontology_term_id is EFO:0030080 or its children, 'suspension_type' MUST be 'cell' or 'nucleus'
+                        # If assay_ontology_term_id is EFO:0030080 or its descendants, 'suspension_type' MUST be 'cell' or 'nucleus'
                         complex_rule:
                             match_ancestors:
                                 column: assay_ontology_term_id
                                 ancestors:
                                     EFO:
                                         - EFO:0030080
                                 inclusive: True
                         type: categorical
                         error_message_suffix: >- 
-                            when 'assay_ontology_term_id' is EFO:0030080 or its children
+                            when 'assay_ontology_term_id' is EFO:0030080 or its descendants
                         enum:
                             - "cell"
                             - "nucleus"
                     -
-                        # If assay_ontology_term_id is EFO:0007045 or its children, 'suspension_type' MUST be 'nucleus'
+                        # If assay_ontology_term_id is EFO:0007045 or its descendants, 'suspension_type' MUST be 'nucleus'
                         complex_rule:
                             match_ancestors:
                                 column: assay_ontology_term_id
                                 ancestors:
                                     EFO:
                                         - EFO:0007045
                                 inclusive: True
                         type: categorical
                         error_message_suffix: >- 
-                            when 'assay_ontology_term_id' is EFO:0007045 or its children
+                            when 'assay_ontology_term_id' is EFO:0007045 or its descendants
                         enum:
                             - "nucleus"
                     -
-                        # If assay_ontology_term_id is EFO:0009294 or its children, 'suspension_type' MUST be 'cell'
+                        # If assay_ontology_term_id is EFO:0009294 or its descendants, 'suspension_type' MUST be 'cell'
                         complex_rule:
                             match_ancestors:
                                 column: assay_ontology_term_id
                                 ancestors:
                                     EFO:
                                         - EFO:0009294
                                 inclusive: True
                         type: categorical
                         error_message_suffix: >- 
-                            when 'assay_ontology_term_id' is EFO:0009294 or its children
+                            when 'assay_ontology_term_id' is EFO:0009294 or its descendants
                         enum:
                             - "cell"
                     -
-                        # If assay_ontology_term_id is EFO:0010184 or its children, 'suspension_type' MUST be 'cell' or 'nucleus'
+                        # If assay_ontology_term_id is EFO:0010184 or its descendants, 'suspension_type' MUST be 'cell' or 'nucleus'
                         complex_rule:
                             match_ancestors:
                                 column: assay_ontology_term_id
                                 ancestors:
                                     EFO:
                                         - EFO:0010184
                                 inclusive: True
                         type: categorical
                         error_message_suffix: >- 
-                            when 'assay_ontology_term_id' is EFO:0010184 or its children
+                            when 'assay_ontology_term_id' is EFO:0010184 or its descendants
                         enum:
                             - "cell"
                             - "nucleus"
                     -
-                        # If assay_ontology_term_id is EFO:0009918 or its children, 'suspension_type' MUST be 'na'
+                        # If assay_ontology_term_id is EFO:0009918 or its descendants, 'suspension_type' MUST be 'na'
                         complex_rule:
                             match_ancestors:
                                 column: assay_ontology_term_id
                                 ancestors:
                                     EFO:
                                         - EFO:0009918
                                 inclusive: True
                         type: categorical
                         error_message_suffix: >- 
-                            when 'assay_ontology_term_id' is EFO:0009918 or its children
+                            when 'assay_ontology_term_id' is EFO:0009918 or its descendants
                         enum:
                             - "na"
                     -
-                        # If assay_ontology_term_id is EFO:0700000 or its children, 'suspension_type' MUST be 'na'
+                        # If assay_ontology_term_id is EFO:0700000 or its descendants, 'suspension_type' MUST be 'na'
                         complex_rule:
                             match_ancestors:
                                 column: assay_ontology_term_id
                                 ancestors:
                                     EFO:
                                         - EFO:0700000
                                 inclusive: True
                         type: categorical
                         error_message_suffix: >- 
-                            when 'assay_ontology_term_id' is EFO:0700000 or its children
+                            when 'assay_ontology_term_id' is EFO:0700000 or its descendants
                         enum:
                             - "na"
                     -
-                        # If assay_ontology_term_id is EFO:0008994 or its children, 'suspension_type' MUST be 'na'
+                        # If assay_ontology_term_id is EFO:0008994 or its descendants, 'suspension_type' MUST be 'na'
                         complex_rule:
                             match_ancestors:
                                 column: assay_ontology_term_id
                                 ancestors:
                                     EFO:
                                         - EFO:0008994
                                 inclusive: True
                         type: categorical
                         error_message_suffix: >- 
-                            when 'assay_ontology_term_id' is EFO:0008994 or its children
+                            when 'assay_ontology_term_id' is EFO:0008994 or its descendants
                         enum:
                             - "na"
                     -
-                        # If assay_ontology_term_id is EFO:0008919 or its children, 'suspension_type' MUST be 'cell'
+                        # If assay_ontology_term_id is EFO:0008919 or its descendants, 'suspension_type' MUST be 'cell'
                         complex_rule:
                             match_ancestors:
                                 column: assay_ontology_term_id
                                 ancestors:
                                     EFO:
                                         - EFO:0008919
                                 inclusive: True
                         type: categorical
                         error_message_suffix: >- 
-                            when 'assay_ontology_term_id' is EFO:0008919 or its children
+                            when 'assay_ontology_term_id' is EFO:0008919 or its descendants
                         enum:
                             - "cell"
                     -
                         # If assay_ontology_term_id is EFO:0010010, 'suspension_type' MUST be 'cell' or 'nucleus'
                         rule: "assay_ontology_term_id == 'EFO:0010010'"
                         type: categorical
                         error_message_suffix: >-
```

### Comparing `cellxgene-schema-5.0.2rc0/cellxgene_schema/utils.py` & `cellxgene-schema-5.0.2rc1/cellxgene_schema/utils.py`

 * *Files identical despite different names*

### Comparing `cellxgene-schema-5.0.2rc0/cellxgene_schema/validate.py` & `cellxgene-schema-5.0.2rc1/cellxgene_schema/validate.py`

 * *Files 0% similar despite different names*

```diff
@@ -102,41 +102,41 @@
         else:
             return self._get_component_def(component)["columns"][column_name]
 
     def _has_forbidden_curie_ancestor(
         self, term_id: str, column_name: str, forbidden_def: Dict[str, List[str]]
     ) -> bool:
         """
-        Validate if a single curie term id is a child term of any forbidden ancestors.
+        Validate if a single curie term id is a descendant term of any forbidden ancestors.
         If there is a forbidden ancestor detected, it adds it to self.errors.
 
         :param str term_id: the curie term id to validate
         :param str column_name: original column name in adata where the term_id comes from (used for error messages)
         :param Dict[str, List[str] forbidden_def: mapping of ontologies to list of ancestor terms to validate against
 
         :returns bool
         """
         for ontology_name in forbidden_def:
             for ancestor in forbidden_def[ontology_name]:
                 if ancestor in ONTOLOGY_PARSER.get_term_ancestors(term_id):
                     self.errors.append(
-                        f"'{term_id}' in '{column_name}' is not allowed. Child terms of "
+                        f"'{term_id}' in '{column_name}' is not allowed. Descendant terms of "
                         f"'{ancestor}' are not allowed."
                     )
                     return True
         return False
 
     def _validate_curie_ancestors(
         self,
         term_id: str,
         allowed_ancestors: Dict[str, List[str]],
         inclusive: bool = False,
     ) -> bool:
         """
-        Validate a single curie term id is a valid child of any allowed ancestors
+        Validate a single curie term id is a valid descendant of any allowed ancestors
 
         :param str term_id: the curie term id to validate
         :param dict{str: list[str]} allowed_ancestors: keys must be ontology names and values must lists of
         allowed ancestors
         :param bool inclusive:  if True then the ancestors themselves are allowed
 
         :rtype Bool
@@ -148,16 +148,16 @@
             for ancestor in ancestors:
                 if inclusive and term_id == ancestor:
                     checks.append(True)
 
                 is_valid_term_id = ONTOLOGY_PARSER.is_valid_term_id(term_id)
                 is_valid_ancestor_id = ONTOLOGY_PARSER.is_valid_term_id(ancestor)
                 if is_valid_term_id & is_valid_ancestor_id:
-                    is_child = ancestor in ONTOLOGY_PARSER.get_term_ancestors(term_id)
-                    checks.append(is_child)
+                    is_descendant = ancestor in ONTOLOGY_PARSER.get_term_ancestors(term_id)
+                    checks.append(is_descendant)
 
         if True not in checks:
             return False
         return True
 
     def _validate_curie_ontology(self, term_id: str, column_name: str, allowed_ontologies: List[str]) -> bool:
         """
@@ -516,15 +516,15 @@
         column = getattr(df.query("not (" + all_rules + " )", engine="python"), column_name)
 
         return column
 
     def _generate_match_ancestors_query_fn(self, rule_def: Dict):
         """
         Generates vectorized function and args to query a pandas dataframe. Function will determine whether values from
-        a specified column is a child term to a group of specified ancestors, returning a Bool.
+        a specified column is a descendant term to a group of specified ancestors, returning a Bool.
         :param rule_def: defines arguments to pass into vectorized ancestor match validation function
         :return: Tuple(function, Tuple(str, List[str], List[str]))
         """
         validate_curie_ancestors_vectorized = np.vectorize(self._validate_curie_ancestors)
         ancestor_map = rule_def["ancestors"]
         inclusive = rule_def["inclusive"]
 
@@ -990,28 +990,28 @@
         for key, value in component.items():
             # Check for empty ndarrays
             if isinstance(value, np.ndarray) and not value.size:
                 self.errors.append(
                     f"The size of the ndarray stored for a 'adata.{component_name}['{key}']' MUST NOT be zero."
                 )
 
-    def _are_children_of(self, component: str, column: str, ontology_name: str, ancestors: List[str]) -> bool:
+    def _are_descendants_of(self, component: str, column: str, ontology_name: str, ancestors: List[str]) -> bool:
         """
         Checks if elements in the specified column of the component (e.g. 'assay_ontology_term_id' of 'adata.obs') are
-        children of the given ancestors.
+        descendants of the given ancestors.
 
         Ancestors checks are inclusive, meaning that a value is its own ancestor as well.
 
         :param str component: the name of the component that's been checked.
         :param str column: Column in the component to check
         :param str ontology_name: Name of the ontology (e.g. "EFO")
         :param List[str] ancestors: List of ancestors
 
         :rtype bool
-        :return True if any value in column is children of any ancestor.
+        :return True if any value in column is a descendant of any ancestor.
         """
 
         curies = getattr(getattr(self.adata, component), column)
         curies = curies.drop_duplicates()
 
         for curie in curies:
             if ONTOLOGY_PARSER.is_valid_term_id(curie):
@@ -1139,17 +1139,17 @@
 
         # Asses if we actually need to perform validation of raw based on the rules in the schema
         # As of now, this means that we only do validation of raw if it's RNA data
         checks = []
         for component, component_rules in self.schema_def["raw"].items():
             for column, column_rules in component_rules.items():
                 for rule, rule_def in column_rules.items():
-                    if rule == "not_children_of":
+                    if rule == "not_descendants_of":
                         for ontology_name, ancestors in rule_def.items():
-                            checks.append(not self._are_children_of(component, column, ontology_name, ancestors))
+                            checks.append(not self._are_descendants_of(component, column, ontology_name, ancestors))
                     else:
                         raise ValueError(f"'{rule}' rule in raw definition of the schema is not implemented ")
 
         # If all checks passed then proceed with validation
         if all(checks):
             # If both "raw.X" and "X" exist but neither are raw
             # This is testing for when sometimes data contributors put a normalized matrix in both "X" and "raw.X".
```

### Comparing `cellxgene-schema-5.0.2rc0/cellxgene_schema/write_labels.py` & `cellxgene-schema-5.0.2rc1/cellxgene_schema/write_labels.py`

 * *Files identical despite different names*

### Comparing `cellxgene-schema-5.0.2rc0/cellxgene_schema.egg-info/PKG-INFO` & `cellxgene-schema-5.0.2rc1/cellxgene_schema.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cellxgene-schema
-Version: 5.0.2rc0
+Version: 5.0.2rc1
 Summary: Tool for applying and validating cellxgene integration schema to single cell datasets
 Home-page: https://github.com/chanzuckerberg/single-cell-curation
 Author: Chan Zuckerberg Initiative
 Author-email: cellxgene@chanzuckerberg.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Intended Audience :: Science/Research
```

### Comparing `cellxgene-schema-5.0.2rc0/cellxgene_schema.egg-info/SOURCES.txt` & `cellxgene-schema-5.0.2rc1/cellxgene_schema.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cellxgene-schema-5.0.2rc0/setup.py` & `cellxgene-schema-5.0.2rc1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 
 with open("requirements.txt") as fh:
     requirements = fh.read().splitlines()
 
 setup(
     name="cellxgene-schema",
-    version="5.0.2-rc.0",
+    version="5.0.2-rc.1",
     url="https://github.com/chanzuckerberg/single-cell-curation",
     license="MIT",
     author="Chan Zuckerberg Initiative",
     author_email="cellxgene@chanzuckerberg.com",
     description="Tool for applying and validating cellxgene integration schema to single cell datasets",
     long_description="Tool for applying and validating cellxgene integration schema to single cell datasets",
     install_requires=requirements,
```

