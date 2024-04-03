# Comparing `tmp/xia-module-gcp-bigquery-0.0.1.tar.gz` & `tmp/xia-module-gcp-bigquery-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xia-module-gcp-bigquery-0.0.1.tar", last modified: Sun Mar 31 18:28:46 2024, max compression
+gzip compressed data, was "xia-module-gcp-bigquery-0.0.2.tar", last modified: Wed Apr  3 07:08:55 2024, max compression
```

## Comparing `xia-module-gcp-bigquery-0.0.1.tar` & `xia-module-gcp-bigquery-0.0.2.tar`

### file list

```diff
@@ -1,38 +1,44 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 18:28:46.783166 xia-module-gcp-bigquery-0.0.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-03-31 18:28:17.000000 xia-module-gcp-bigquery-0.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-03-31 18:28:46.000000 xia-module-gcp-bigquery-0.0.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)      223 2024-03-31 18:28:46.783166 xia-module-gcp-bigquery-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       72 2024-03-31 18:28:17.000000 xia-module-gcp-bigquery-0.0.1/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-31 18:28:46.783166 xia-module-gcp-bigquery-0.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2247 2024-03-31 18:28:17.000000 xia-module-gcp-bigquery-0.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 18:28:46.779166 xia-module-gcp-bigquery-0.0.1/xia_module_gcp_bigquery/
--rw-r--r--   0 runner    (1001) docker     (127)      165 2024-03-31 18:28:17.000000 xia-module-gcp-bigquery-0.0.1/xia_module_gcp_bigquery/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      140 2024-03-31 18:28:17.000000 xia-module-gcp-bigquery-0.0.1/xia_module_gcp_bigquery/dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)      136 2024-03-31 18:28:17.000000 xia-module-gcp-bigquery-0.0.1/xia_module_gcp_bigquery/table.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 18:28:46.779166 xia-module-gcp-bigquery-0.0.1/xia_module_gcp_bigquery/templates/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 18:28:46.779166 xia-module-gcp-bigquery-0.0.1/xia_module_gcp_bigquery/templates/gcp-module-dataset/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 18:28:46.779166 xia-module-gcp-bigquery-0.0.1/xia_module_gcp_bigquery/templates/gcp-module-dataset/activate/
--rw-r--r--   0 runner    (1001) docker     (127)     1767 2024-03-31 18:28:17.000000 xia-module-gcp-bigquery-0.0.1/xia_module_gcp_bigquery/templates/gcp-module-dataset/activate/main.tf
--rw-r--r--   0 runner    (1001) docker     (127)      519 2024-03-31 18:28:17.000000 xia-module-gcp-bigquery-0.0.1/xia_module_gcp_bigquery/templates/gcp-module-dataset/activate/variables.tf
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 18:28:46.783166 xia-module-gcp-bigquery-0.0.1/xia_module_gcp_bigquery/templates/gcp-module-dataset/base/
--rw-r--r--   0 runner    (1001) docker     (127)      258 2024-03-31 18:28:17.000000 xia-module-gcp-bigquery-0.0.1/xia_module_gcp_bigquery/templates/gcp-module-dataset/base/activate.tf
--rw-r--r--   0 runner    (1001) docker     (127)      112 2024-03-31 18:28:17.000000 xia-module-gcp-bigquery-0.0.1/xia_module_gcp_bigquery/templates/gcp-module-dataset/base/main.tf
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 18:28:46.783166 xia-module-gcp-bigquery-0.0.1/xia_module_gcp_bigquery/templates/gcp-module-dataset/module/
--rw-r--r--   0 runner    (1001) docker     (127)      100 2024-03-31 18:28:17.000000 xia-module-gcp-bigquery-0.0.1/xia_module_gcp_bigquery/templates/gcp-module-dataset/module/main.tf
--rw-r--r--   0 runner    (1001) docker     (127)      171 2024-03-31 18:28:17.000000 xia-module-gcp-bigquery-0.0.1/xia_module_gcp_bigquery/templates/gcp-module-dataset/module/variables.tf
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 18:28:46.779166 xia-module-gcp-bigquery-0.0.1/xia_module_gcp_bigquery/templates/gcp-module-table/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 18:28:46.783166 xia-module-gcp-bigquery-0.0.1/xia_module_gcp_bigquery/templates/gcp-module-table/activate/
--rw-r--r--   0 runner    (1001) docker     (127)     1808 2024-03-31 18:28:17.000000 xia-module-gcp-bigquery-0.0.1/xia_module_gcp_bigquery/templates/gcp-module-table/activate/main.tf
--rw-r--r--   0 runner    (1001) docker     (127)      519 2024-03-31 18:28:17.000000 xia-module-gcp-bigquery-0.0.1/xia_module_gcp_bigquery/templates/gcp-module-table/activate/variables.tf
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 18:28:46.783166 xia-module-gcp-bigquery-0.0.1/xia_module_gcp_bigquery/templates/gcp-module-table/base/
--rw-r--r--   0 runner    (1001) docker     (127)      254 2024-03-31 18:28:17.000000 xia-module-gcp-bigquery-0.0.1/xia_module_gcp_bigquery/templates/gcp-module-table/base/activate.tf
--rw-r--r--   0 runner    (1001) docker     (127)      229 2024-03-31 18:28:17.000000 xia-module-gcp-bigquery-0.0.1/xia_module_gcp_bigquery/templates/gcp-module-table/base/main.tf
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 18:28:46.783166 xia-module-gcp-bigquery-0.0.1/xia_module_gcp_bigquery/templates/gcp-module-table/module/
--rw-r--r--   0 runner    (1001) docker     (127)      100 2024-03-31 18:28:17.000000 xia-module-gcp-bigquery-0.0.1/xia_module_gcp_bigquery/templates/gcp-module-table/module/main.tf
--rw-r--r--   0 runner    (1001) docker     (127)      171 2024-03-31 18:28:17.000000 xia-module-gcp-bigquery-0.0.1/xia_module_gcp_bigquery/templates/gcp-module-table/module/variables.tf
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-31 18:28:46.779166 xia-module-gcp-bigquery-0.0.1/xia_module_gcp_bigquery.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      223 2024-03-31 18:28:46.000000 xia-module-gcp-bigquery-0.0.1/xia_module_gcp_bigquery.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1209 2024-03-31 18:28:46.000000 xia-module-gcp-bigquery-0.0.1/xia_module_gcp_bigquery.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-31 18:28:46.000000 xia-module-gcp-bigquery-0.0.1/xia_module_gcp_bigquery.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-03-31 18:28:46.000000 xia-module-gcp-bigquery-0.0.1/xia_module_gcp_bigquery.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-03-31 18:28:46.000000 xia-module-gcp-bigquery-0.0.1/xia_module_gcp_bigquery.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 07:08:55.230963 xia-module-gcp-bigquery-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-04-03 07:08:28.000000 xia-module-gcp-bigquery-0.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-03 07:08:54.000000 xia-module-gcp-bigquery-0.0.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)      223 2024-04-03 07:08:55.230963 xia-module-gcp-bigquery-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-04-03 07:08:28.000000 xia-module-gcp-bigquery-0.0.2/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-03 07:08:55.230963 xia-module-gcp-bigquery-0.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2247 2024-04-03 07:08:28.000000 xia-module-gcp-bigquery-0.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 07:08:55.226963 xia-module-gcp-bigquery-0.0.2/xia_module_gcp_bigquery/
+-rw-r--r--   0 runner    (1001) docker     (127)      165 2024-04-03 07:08:28.000000 xia-module-gcp-bigquery-0.0.2/xia_module_gcp_bigquery/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      140 2024-04-03 07:08:28.000000 xia-module-gcp-bigquery-0.0.2/xia_module_gcp_bigquery/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)      136 2024-04-03 07:08:28.000000 xia-module-gcp-bigquery-0.0.2/xia_module_gcp_bigquery/table.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 07:08:55.226963 xia-module-gcp-bigquery-0.0.2/xia_module_gcp_bigquery/templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 07:08:55.226963 xia-module-gcp-bigquery-0.0.2/xia_module_gcp_bigquery/templates/gcp-module-dataset/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 07:08:55.230963 xia-module-gcp-bigquery-0.0.2/xia_module_gcp_bigquery/templates/gcp-module-dataset/activate/
+-rw-r--r--   0 runner    (1001) docker     (127)     1884 2024-04-03 07:08:28.000000 xia-module-gcp-bigquery-0.0.2/xia_module_gcp_bigquery/templates/gcp-module-dataset/activate/main.tf
+-rw-r--r--   0 runner    (1001) docker     (127)      519 2024-04-03 07:08:28.000000 xia-module-gcp-bigquery-0.0.2/xia_module_gcp_bigquery/templates/gcp-module-dataset/activate/variables.tf
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 07:08:55.230963 xia-module-gcp-bigquery-0.0.2/xia_module_gcp_bigquery/templates/gcp-module-dataset/base/
+-rw-r--r--   0 runner    (1001) docker     (127)      258 2024-04-03 07:08:28.000000 xia-module-gcp-bigquery-0.0.2/xia_module_gcp_bigquery/templates/gcp-module-dataset/base/activate.tf
+-rw-r--r--   0 runner    (1001) docker     (127)      112 2024-04-03 07:08:28.000000 xia-module-gcp-bigquery-0.0.2/xia_module_gcp_bigquery/templates/gcp-module-dataset/base/main.tf
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 07:08:55.226963 xia-module-gcp-bigquery-0.0.2/xia_module_gcp_bigquery/templates/gcp-module-dataset/cicd/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 07:08:55.230963 xia-module-gcp-bigquery-0.0.2/xia_module_gcp_bigquery/templates/gcp-module-dataset/cicd/github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 07:08:55.226963 xia-module-gcp-bigquery-0.0.2/xia_module_gcp_bigquery/templates/gcp-module-dataset/cicd/github/actions/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 07:08:55.230963 xia-module-gcp-bigquery-0.0.2/xia_module_gcp_bigquery/templates/gcp-module-dataset/cicd/github/actions/gcs-terraform-apply/
+-rw-r--r--   0 runner    (1001) docker     (127)      976 2024-04-03 07:08:28.000000 xia-module-gcp-bigquery-0.0.2/xia_module_gcp_bigquery/templates/gcp-module-dataset/cicd/github/actions/gcs-terraform-apply/action.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      922 2024-04-03 07:08:28.000000 xia-module-gcp-bigquery-0.0.2/xia_module_gcp_bigquery/templates/gcp-module-dataset/cicd/github/workflow.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 07:08:55.230963 xia-module-gcp-bigquery-0.0.2/xia_module_gcp_bigquery/templates/gcp-module-dataset/module/
+-rw-r--r--   0 runner    (1001) docker     (127)      100 2024-04-03 07:08:28.000000 xia-module-gcp-bigquery-0.0.2/xia_module_gcp_bigquery/templates/gcp-module-dataset/module/main.tf
+-rw-r--r--   0 runner    (1001) docker     (127)      171 2024-04-03 07:08:28.000000 xia-module-gcp-bigquery-0.0.2/xia_module_gcp_bigquery/templates/gcp-module-dataset/module/variables.tf
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 07:08:55.226963 xia-module-gcp-bigquery-0.0.2/xia_module_gcp_bigquery/templates/gcp-module-table/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 07:08:55.230963 xia-module-gcp-bigquery-0.0.2/xia_module_gcp_bigquery/templates/gcp-module-table/activate/
+-rw-r--r--   0 runner    (1001) docker     (127)     1925 2024-04-03 07:08:28.000000 xia-module-gcp-bigquery-0.0.2/xia_module_gcp_bigquery/templates/gcp-module-table/activate/main.tf
+-rw-r--r--   0 runner    (1001) docker     (127)      519 2024-04-03 07:08:28.000000 xia-module-gcp-bigquery-0.0.2/xia_module_gcp_bigquery/templates/gcp-module-table/activate/variables.tf
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 07:08:55.230963 xia-module-gcp-bigquery-0.0.2/xia_module_gcp_bigquery/templates/gcp-module-table/base/
+-rw-r--r--   0 runner    (1001) docker     (127)      254 2024-04-03 07:08:28.000000 xia-module-gcp-bigquery-0.0.2/xia_module_gcp_bigquery/templates/gcp-module-table/base/activate.tf
+-rw-r--r--   0 runner    (1001) docker     (127)      229 2024-04-03 07:08:28.000000 xia-module-gcp-bigquery-0.0.2/xia_module_gcp_bigquery/templates/gcp-module-table/base/main.tf
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 07:08:55.230963 xia-module-gcp-bigquery-0.0.2/xia_module_gcp_bigquery/templates/gcp-module-table/module/
+-rw-r--r--   0 runner    (1001) docker     (127)      100 2024-04-03 07:08:28.000000 xia-module-gcp-bigquery-0.0.2/xia_module_gcp_bigquery/templates/gcp-module-table/module/main.tf
+-rw-r--r--   0 runner    (1001) docker     (127)      171 2024-04-03 07:08:28.000000 xia-module-gcp-bigquery-0.0.2/xia_module_gcp_bigquery/templates/gcp-module-table/module/variables.tf
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 07:08:55.230963 xia-module-gcp-bigquery-0.0.2/xia_module_gcp_bigquery.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      223 2024-04-03 07:08:55.000000 xia-module-gcp-bigquery-0.0.2/xia_module_gcp_bigquery.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1391 2024-04-03 07:08:55.000000 xia-module-gcp-bigquery-0.0.2/xia_module_gcp_bigquery.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 07:08:55.000000 xia-module-gcp-bigquery-0.0.2/xia_module_gcp_bigquery.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-03 07:08:55.000000 xia-module-gcp-bigquery-0.0.2/xia_module_gcp_bigquery.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-03 07:08:55.000000 xia-module-gcp-bigquery-0.0.2/xia_module_gcp_bigquery.egg-info/top_level.txt
```

### Comparing `xia-module-gcp-bigquery-0.0.1/LICENSE` & `xia-module-gcp-bigquery-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `xia-module-gcp-bigquery-0.0.1/setup.py` & `xia-module-gcp-bigquery-0.0.2/setup.py`

 * *Files identical despite different names*

### Comparing `xia-module-gcp-bigquery-0.0.1/xia_module_gcp_bigquery/templates/gcp-module-dataset/activate/main.tf` & `xia-module-gcp-bigquery-0.0.2/xia_module_gcp_bigquery/templates/gcp-module-dataset/activate/main.tf`

 * *Files 12% similar despite different names*

```diff
@@ -16,14 +16,19 @@
         env_name          = env_name
         project_id        = "${local.project_prefix}${env_name}"
       }
     ]
   ]))
 }
 
+resource "google_project_service" "bigquery" {
+  service = "bigquery.googleapis.com"
+  disable_on_destroy = false
+}
+
 resource "google_project_iam_custom_role" "gcp_module_dataset_deployer_role" {
   for_each = local.environment_dict
 
   project     = "${local.project_prefix}${each.key}"
   role_id     = "gcpModuleDatasetDeployer"
   title       = "GCP Bigquery Dataset Deployer Role"
   description = "GCP Bigquery Dataset Deployer Role"
```

### Comparing `xia-module-gcp-bigquery-0.0.1/xia_module_gcp_bigquery/templates/gcp-module-dataset/activate/variables.tf` & `xia-module-gcp-bigquery-0.0.2/xia_module_gcp_bigquery/templates/gcp-module-dataset/activate/variables.tf`

 * *Files identical despite different names*

### Comparing `xia-module-gcp-bigquery-0.0.1/xia_module_gcp_bigquery/templates/gcp-module-table/activate/main.tf` & `xia-module-gcp-bigquery-0.0.2/xia_module_gcp_bigquery/templates/gcp-module-table/activate/main.tf`

 * *Files 5% similar despite different names*

```diff
@@ -33,14 +33,19 @@
     "bigquery.tables.list",
     "bigquery.tables.update",
     "bigquery.tables.delete",
     "bigquery.datasets.update"
   ]
 }
 
+resource "google_project_service" "bigquery" {
+  service = "bigquery.googleapis.com"
+  disable_on_destroy = false
+}
+
 resource "google_project_iam_member" "gcp_module_table_deployer_role_member" {
   for_each = { for s in local.all_role_attribution : "${s.app_name}-${s.env_name}" => s }
 
   project = each.value["project_id"]
   role    = google_project_iam_custom_role.gcp_module_table_deployer_role[each.value["env_name"]].id
   member  = "serviceAccount:wip-${each.value["app_name"]}-sa@${each.value["project_id"]}.iam.gserviceaccount.com"
```

### Comparing `xia-module-gcp-bigquery-0.0.1/xia_module_gcp_bigquery/templates/gcp-module-table/activate/variables.tf` & `xia-module-gcp-bigquery-0.0.2/xia_module_gcp_bigquery/templates/gcp-module-table/activate/variables.tf`

 * *Files identical despite different names*

### Comparing `xia-module-gcp-bigquery-0.0.1/xia_module_gcp_bigquery.egg-info/SOURCES.txt` & `xia-module-gcp-bigquery-0.0.2/xia_module_gcp_bigquery.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -10,14 +10,16 @@
 xia_module_gcp_bigquery.egg-info/dependency_links.txt
 xia_module_gcp_bigquery.egg-info/requires.txt
 xia_module_gcp_bigquery.egg-info/top_level.txt
 xia_module_gcp_bigquery/templates/gcp-module-dataset/activate/main.tf
 xia_module_gcp_bigquery/templates/gcp-module-dataset/activate/variables.tf
 xia_module_gcp_bigquery/templates/gcp-module-dataset/base/activate.tf
 xia_module_gcp_bigquery/templates/gcp-module-dataset/base/main.tf
+xia_module_gcp_bigquery/templates/gcp-module-dataset/cicd/github/workflow.yml
+xia_module_gcp_bigquery/templates/gcp-module-dataset/cicd/github/actions/gcs-terraform-apply/action.yml
 xia_module_gcp_bigquery/templates/gcp-module-dataset/module/main.tf
 xia_module_gcp_bigquery/templates/gcp-module-dataset/module/variables.tf
 xia_module_gcp_bigquery/templates/gcp-module-table/activate/main.tf
 xia_module_gcp_bigquery/templates/gcp-module-table/activate/variables.tf
 xia_module_gcp_bigquery/templates/gcp-module-table/base/activate.tf
 xia_module_gcp_bigquery/templates/gcp-module-table/base/main.tf
 xia_module_gcp_bigquery/templates/gcp-module-table/module/main.tf
```

