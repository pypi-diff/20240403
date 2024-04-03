# Comparing `tmp/ssb_datadoc-0.8.2.tar.gz` & `tmp/ssb_datadoc-0.8.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ssb_datadoc-0.8.2.tar", max compression
+gzip compressed data, was "ssb_datadoc-0.8.3.tar", max compression
```

## Comparing `ssb_datadoc-0.8.2.tar` & `ssb_datadoc-0.8.3.tar`

### file list

```diff
@@ -1,51 +1,51 @@
--rw-r--r--   0        0        0     1073 2024-04-02 10:56:19.575211 ssb_datadoc-0.8.2/LICENSE
--rw-r--r--   0        0        0     3034 2024-04-02 10:56:19.575211 ssb_datadoc-0.8.2/README.md
--rw-r--r--   0        0        0     5188 2024-04-02 10:56:27.959211 ssb_datadoc-0.8.2/pyproject.toml
--rw-r--r--   0        0        0       85 2024-04-02 10:56:19.579211 ssb_datadoc-0.8.2/src/datadoc/__init__.py
--rw-r--r--   0        0        0     5885 2024-04-02 10:56:19.579211 ssb_datadoc-0.8.2/src/datadoc/app.py
--rw-r--r--   0        0        0      133 2024-04-02 10:56:19.579211 ssb_datadoc-0.8.2/src/datadoc/assets/app_style.css
--rw-r--r--   0        0        0    80523 2024-04-02 10:56:19.579211 ssb_datadoc-0.8.2/src/datadoc/assets/bootstrap-icons.css
--rw-r--r--   0        0        0   163874 2024-04-02 10:56:19.579211 ssb_datadoc-0.8.2/src/datadoc/assets/bootstrap.min.css
--rw-r--r--   0        0        0    52127 2024-04-02 10:56:19.579211 ssb_datadoc-0.8.2/src/datadoc/assets/bundle.css
--rw-r--r--   0        0        0      346 2024-04-02 10:56:19.579211 ssb_datadoc-0.8.2/src/datadoc/assets/controlbar_style.css
--rw-r--r--   0        0        0   137124 2024-04-02 10:56:19.579211 ssb_datadoc-0.8.2/src/datadoc/assets/fonts/bootstrap-icons.woff
--rw-r--r--   0        0        0   102536 2024-04-02 10:56:19.579211 ssb_datadoc-0.8.2/src/datadoc/assets/fonts/bootstrap-icons.woff2
--rw-r--r--   0        0        0      213 2024-04-02 10:56:19.579211 ssb_datadoc-0.8.2/src/datadoc/assets/header.css
--rw-r--r--   0        0        0     1405 2024-04-02 10:56:19.579211 ssb_datadoc-0.8.2/src/datadoc/assets/workspace_style.css
--rw-r--r--   0        0        0      131 2024-04-02 10:56:19.579211 ssb_datadoc-0.8.2/src/datadoc/assets/workspace_tab.css
--rw-r--r--   0        0        0       56 2024-04-02 10:56:19.579211 ssb_datadoc-0.8.2/src/datadoc/backend/__init__.py
--rw-r--r--   0        0        0     5635 2024-04-02 10:56:19.579211 ssb_datadoc-0.8.2/src/datadoc/backend/code_list.py
--rw-r--r--   0        0        0    13540 2024-04-02 10:56:19.579211 ssb_datadoc-0.8.2/src/datadoc/backend/dapla_dataset_path_info.py
--rw-r--r--   0        0        0    11054 2024-04-02 10:56:19.579211 ssb_datadoc-0.8.2/src/datadoc/backend/datadoc_metadata.py
--rw-r--r--   0        0        0     7491 2024-04-02 10:56:19.579211 ssb_datadoc-0.8.2/src/datadoc/backend/dataset_parser.py
--rw-r--r--   0        0        0       83 2024-04-02 10:56:19.579211 ssb_datadoc-0.8.2/src/datadoc/backend/external_sources/__init__.py
--rw-r--r--   0        0        0     1681 2024-04-02 10:56:19.579211 ssb_datadoc-0.8.2/src/datadoc/backend/external_sources/external_sources.py
--rw-r--r--   0        0        0     5321 2024-04-02 10:56:19.579211 ssb_datadoc-0.8.2/src/datadoc/backend/model_backwards_compatibility.py
--rw-r--r--   0        0        0     5828 2024-04-02 10:56:19.579211 ssb_datadoc-0.8.2/src/datadoc/backend/statistic_subject_mapping.py
--rw-r--r--   0        0        0     2500 2024-04-02 10:56:19.579211 ssb_datadoc-0.8.2/src/datadoc/backend/user_info.py
--rw-r--r--   0        0        0     3730 2024-04-02 10:56:19.579211 ssb_datadoc-0.8.2/src/datadoc/config.py
--rw-r--r--   0        0        0     6184 2024-04-02 10:56:19.579211 ssb_datadoc-0.8.2/src/datadoc/enums.py
--rw-r--r--   0        0        0       52 2024-04-02 10:56:19.579211 ssb_datadoc-0.8.2/src/datadoc/frontend/__init__.py
--rw-r--r--   0        0        0      310 2024-04-02 10:56:19.579211 ssb_datadoc-0.8.2/src/datadoc/frontend/callbacks/__init__.py
--rw-r--r--   0        0        0     7865 2024-04-02 10:56:19.579211 ssb_datadoc-0.8.2/src/datadoc/frontend/callbacks/dataset.py
--rw-r--r--   0        0        0    13456 2024-04-02 10:56:19.579211 ssb_datadoc-0.8.2/src/datadoc/frontend/callbacks/register_callbacks.py
--rw-r--r--   0        0        0     5623 2024-04-02 10:56:19.579211 ssb_datadoc-0.8.2/src/datadoc/frontend/callbacks/utils.py
--rw-r--r--   0        0        0     5466 2024-04-02 10:56:19.579211 ssb_datadoc-0.8.2/src/datadoc/frontend/callbacks/variables.py
--rw-r--r--   0        0        0      190 2024-04-02 10:56:19.579211 ssb_datadoc-0.8.2/src/datadoc/frontend/components/__init__.py
--rw-r--r--   0        0        0     1063 2024-04-02 10:56:19.579211 ssb_datadoc-0.8.2/src/datadoc/frontend/components/alerts.py
--rw-r--r--   0        0        0     5414 2024-04-02 10:56:19.579211 ssb_datadoc-0.8.2/src/datadoc/frontend/components/builders.py
--rw-r--r--   0        0        0     2502 2024-04-02 10:56:19.579211 ssb_datadoc-0.8.2/src/datadoc/frontend/components/control_bars.py
--rw-r--r--   0        0        0     1101 2024-04-02 10:56:19.579211 ssb_datadoc-0.8.2/src/datadoc/frontend/components/dataset_tab.py
--rw-r--r--   0        0        0     1734 2024-04-02 10:56:19.579211 ssb_datadoc-0.8.2/src/datadoc/frontend/components/variables_tab.py
--rw-r--r--   0        0        0       74 2024-04-02 10:56:19.579211 ssb_datadoc-0.8.2/src/datadoc/frontend/fields/__init__.py
--rw-r--r--   0        0        0     8725 2024-04-02 10:56:19.579211 ssb_datadoc-0.8.2/src/datadoc/frontend/fields/display_base.py
--rw-r--r--   0        0        0    13438 2024-04-02 10:56:19.579211 ssb_datadoc-0.8.2/src/datadoc/frontend/fields/display_dataset.py
--rw-r--r--   0        0        0     8336 2024-04-02 10:56:19.579211 ssb_datadoc-0.8.2/src/datadoc/frontend/fields/display_variables.py
--rw-r--r--   0        0        0       72 2024-04-02 10:56:19.579211 ssb_datadoc-0.8.2/src/datadoc/logging_configuration/__init__.py
--rw-r--r--   0        0        0     1586 2024-04-02 10:56:19.579211 ssb_datadoc-0.8.2/src/datadoc/logging_configuration/json_formatter.py
--rw-r--r--   0        0        0     1747 2024-04-02 10:56:19.579211 ssb_datadoc-0.8.2/src/datadoc/logging_configuration/logging_config.py
--rw-r--r--   0        0        0        0 2024-04-02 10:56:19.579211 ssb_datadoc-0.8.2/src/datadoc/py.typed
--rw-r--r--   0        0        0      898 2024-04-02 10:56:19.579211 ssb_datadoc-0.8.2/src/datadoc/state.py
--rw-r--r--   0        0        0     2153 2024-04-02 10:56:19.579211 ssb_datadoc-0.8.2/src/datadoc/utils.py
--rw-r--r--   0        0        0      220 2024-04-02 10:56:19.579211 ssb_datadoc-0.8.2/src/datadoc/wsgi.py
--rw-r--r--   0        0        0     4583 1970-01-01 00:00:00.000000 ssb_datadoc-0.8.2/PKG-INFO
+-rw-r--r--   0        0        0     1073 2024-04-03 12:53:52.041906 ssb_datadoc-0.8.3/LICENSE
+-rw-r--r--   0        0        0     3034 2024-04-03 12:53:52.041906 ssb_datadoc-0.8.3/README.md
+-rw-r--r--   0        0        0     5188 2024-04-03 12:54:04.289871 ssb_datadoc-0.8.3/pyproject.toml
+-rw-r--r--   0        0        0       85 2024-04-03 12:53:52.045906 ssb_datadoc-0.8.3/src/datadoc/__init__.py
+-rw-r--r--   0        0        0     6015 2024-04-03 12:53:52.045906 ssb_datadoc-0.8.3/src/datadoc/app.py
+-rw-r--r--   0        0        0      154 2024-04-03 12:53:52.045906 ssb_datadoc-0.8.3/src/datadoc/assets/app_style.css
+-rw-r--r--   0        0        0    80523 2024-04-03 12:53:52.045906 ssb_datadoc-0.8.3/src/datadoc/assets/bootstrap-icons.css
+-rw-r--r--   0        0        0   163874 2024-04-03 12:53:52.045906 ssb_datadoc-0.8.3/src/datadoc/assets/bootstrap.min.css
+-rw-r--r--   0        0        0    52127 2024-04-03 12:53:52.045906 ssb_datadoc-0.8.3/src/datadoc/assets/bundle.css
+-rw-r--r--   0        0        0      390 2024-04-03 12:53:52.045906 ssb_datadoc-0.8.3/src/datadoc/assets/controlbar_style.css
+-rw-r--r--   0        0        0   137124 2024-04-03 12:53:52.045906 ssb_datadoc-0.8.3/src/datadoc/assets/fonts/bootstrap-icons.woff
+-rw-r--r--   0        0        0   102536 2024-04-03 12:53:52.045906 ssb_datadoc-0.8.3/src/datadoc/assets/fonts/bootstrap-icons.woff2
+-rw-r--r--   0        0        0      218 2024-04-03 12:53:52.045906 ssb_datadoc-0.8.3/src/datadoc/assets/header.css
+-rw-r--r--   0        0        0     1296 2024-04-03 12:53:52.045906 ssb_datadoc-0.8.3/src/datadoc/assets/workspace_style.css
+-rw-r--r--   0        0        0      131 2024-04-03 12:53:52.045906 ssb_datadoc-0.8.3/src/datadoc/assets/workspace_tab.css
+-rw-r--r--   0        0        0       56 2024-04-03 12:53:52.045906 ssb_datadoc-0.8.3/src/datadoc/backend/__init__.py
+-rw-r--r--   0        0        0     5635 2024-04-03 12:53:52.045906 ssb_datadoc-0.8.3/src/datadoc/backend/code_list.py
+-rw-r--r--   0        0        0    13540 2024-04-03 12:53:52.045906 ssb_datadoc-0.8.3/src/datadoc/backend/dapla_dataset_path_info.py
+-rw-r--r--   0        0        0    11054 2024-04-03 12:53:52.045906 ssb_datadoc-0.8.3/src/datadoc/backend/datadoc_metadata.py
+-rw-r--r--   0        0        0     7491 2024-04-03 12:53:52.045906 ssb_datadoc-0.8.3/src/datadoc/backend/dataset_parser.py
+-rw-r--r--   0        0        0       83 2024-04-03 12:53:52.045906 ssb_datadoc-0.8.3/src/datadoc/backend/external_sources/__init__.py
+-rw-r--r--   0        0        0     1681 2024-04-03 12:53:52.045906 ssb_datadoc-0.8.3/src/datadoc/backend/external_sources/external_sources.py
+-rw-r--r--   0        0        0     5321 2024-04-03 12:53:52.045906 ssb_datadoc-0.8.3/src/datadoc/backend/model_backwards_compatibility.py
+-rw-r--r--   0        0        0     5828 2024-04-03 12:53:52.045906 ssb_datadoc-0.8.3/src/datadoc/backend/statistic_subject_mapping.py
+-rw-r--r--   0        0        0     2500 2024-04-03 12:53:52.045906 ssb_datadoc-0.8.3/src/datadoc/backend/user_info.py
+-rw-r--r--   0        0        0     3730 2024-04-03 12:53:52.045906 ssb_datadoc-0.8.3/src/datadoc/config.py
+-rw-r--r--   0        0        0     6184 2024-04-03 12:53:52.045906 ssb_datadoc-0.8.3/src/datadoc/enums.py
+-rw-r--r--   0        0        0       52 2024-04-03 12:53:52.045906 ssb_datadoc-0.8.3/src/datadoc/frontend/__init__.py
+-rw-r--r--   0        0        0      310 2024-04-03 12:53:52.045906 ssb_datadoc-0.8.3/src/datadoc/frontend/callbacks/__init__.py
+-rw-r--r--   0        0        0     7865 2024-04-03 12:53:52.045906 ssb_datadoc-0.8.3/src/datadoc/frontend/callbacks/dataset.py
+-rw-r--r--   0        0        0    13456 2024-04-03 12:53:52.045906 ssb_datadoc-0.8.3/src/datadoc/frontend/callbacks/register_callbacks.py
+-rw-r--r--   0        0        0     5623 2024-04-03 12:53:52.045906 ssb_datadoc-0.8.3/src/datadoc/frontend/callbacks/utils.py
+-rw-r--r--   0        0        0     5466 2024-04-03 12:53:52.045906 ssb_datadoc-0.8.3/src/datadoc/frontend/callbacks/variables.py
+-rw-r--r--   0        0        0      190 2024-04-03 12:53:52.045906 ssb_datadoc-0.8.3/src/datadoc/frontend/components/__init__.py
+-rw-r--r--   0        0        0     1063 2024-04-03 12:53:52.045906 ssb_datadoc-0.8.3/src/datadoc/frontend/components/alerts.py
+-rw-r--r--   0        0        0     5414 2024-04-03 12:53:52.045906 ssb_datadoc-0.8.3/src/datadoc/frontend/components/builders.py
+-rw-r--r--   0        0        0     2502 2024-04-03 12:53:52.045906 ssb_datadoc-0.8.3/src/datadoc/frontend/components/control_bars.py
+-rw-r--r--   0        0        0     1101 2024-04-03 12:53:52.045906 ssb_datadoc-0.8.3/src/datadoc/frontend/components/dataset_tab.py
+-rw-r--r--   0        0        0     1734 2024-04-03 12:53:52.045906 ssb_datadoc-0.8.3/src/datadoc/frontend/components/variables_tab.py
+-rw-r--r--   0        0        0       74 2024-04-03 12:53:52.049906 ssb_datadoc-0.8.3/src/datadoc/frontend/fields/__init__.py
+-rw-r--r--   0        0        0     8725 2024-04-03 12:53:52.049906 ssb_datadoc-0.8.3/src/datadoc/frontend/fields/display_base.py
+-rw-r--r--   0        0        0    13438 2024-04-03 12:53:52.049906 ssb_datadoc-0.8.3/src/datadoc/frontend/fields/display_dataset.py
+-rw-r--r--   0        0        0     8336 2024-04-03 12:53:52.049906 ssb_datadoc-0.8.3/src/datadoc/frontend/fields/display_variables.py
+-rw-r--r--   0        0        0       72 2024-04-03 12:53:52.049906 ssb_datadoc-0.8.3/src/datadoc/logging_configuration/__init__.py
+-rw-r--r--   0        0        0     1586 2024-04-03 12:53:52.049906 ssb_datadoc-0.8.3/src/datadoc/logging_configuration/json_formatter.py
+-rw-r--r--   0        0        0     1747 2024-04-03 12:53:52.049906 ssb_datadoc-0.8.3/src/datadoc/logging_configuration/logging_config.py
+-rw-r--r--   0        0        0        0 2024-04-03 12:53:52.049906 ssb_datadoc-0.8.3/src/datadoc/py.typed
+-rw-r--r--   0        0        0      898 2024-04-03 12:53:52.049906 ssb_datadoc-0.8.3/src/datadoc/state.py
+-rw-r--r--   0        0        0     2153 2024-04-03 12:53:52.049906 ssb_datadoc-0.8.3/src/datadoc/utils.py
+-rw-r--r--   0        0        0      220 2024-04-03 12:53:52.049906 ssb_datadoc-0.8.3/src/datadoc/wsgi.py
+-rw-r--r--   0        0        0     4583 1970-01-01 00:00:00.000000 ssb_datadoc-0.8.3/PKG-INFO
```

### Comparing `ssb_datadoc-0.8.2/LICENSE` & `ssb_datadoc-0.8.3/LICENSE`

 * *Files identical despite different names*

### Comparing `ssb_datadoc-0.8.2/README.md` & `ssb_datadoc-0.8.3/README.md`

 * *Files identical despite different names*

### Comparing `ssb_datadoc-0.8.2/pyproject.toml` & `ssb_datadoc-0.8.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ssb-datadoc"
-version = "0.8.2"
+version = "0.8.3"
 description = "Document dataset metadata. For use in Statistics Norway's metadata system."
 authors = ["Statistics Norway <stat-dev@ssb.no>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/statisticsnorway/datadoc"
 repository = "https://github.com/statisticsnorway/datadoc"
 documentation = "https://statisticsnorway.github.io/datadoc"
```

### Comparing `ssb_datadoc-0.8.2/src/datadoc/app.py` & `ssb_datadoc-0.8.3/src/datadoc/app.py`

 * *Files 2% similar despite different names*

```diff
@@ -69,15 +69,20 @@
                         id="tabs",
                         class_name="ssb-tabs",
                         children=tabs_children,
                     ),
                 ],
                 className="main-content-app",
             ),
-            build_language_dropdown(),
+            html.Footer(
+                [
+                    build_language_dropdown(),
+                ],
+                className="language-footer",
+            ),
         ],
         className="app-wrapper",
     )
 
     register_callbacks(app)
 
     return app
```

### Comparing `ssb_datadoc-0.8.2/src/datadoc/assets/bootstrap-icons.css` & `ssb_datadoc-0.8.3/src/datadoc/assets/bootstrap-icons.css`

 * *Files identical despite different names*

### Comparing `ssb_datadoc-0.8.2/src/datadoc/assets/bootstrap.min.css` & `ssb_datadoc-0.8.3/src/datadoc/assets/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `ssb_datadoc-0.8.2/src/datadoc/assets/bundle.css` & `ssb_datadoc-0.8.3/src/datadoc/assets/bundle.css`

 * *Files identical despite different names*

### Comparing `ssb_datadoc-0.8.2/src/datadoc/assets/fonts/bootstrap-icons.woff` & `ssb_datadoc-0.8.3/src/datadoc/assets/fonts/bootstrap-icons.woff`

 * *Files identical despite different names*

### Comparing `ssb_datadoc-0.8.2/src/datadoc/assets/fonts/bootstrap-icons.woff2` & `ssb_datadoc-0.8.3/src/datadoc/assets/fonts/bootstrap-icons.woff2`

 * *Files identical despite different names*

### Comparing `ssb_datadoc-0.8.2/src/datadoc/assets/workspace_style.css` & `ssb_datadoc-0.8.3/src/datadoc/assets/workspace_style.css`

 * *Files 19% similar despite different names*

```diff
@@ -42,14 +42,15 @@
 }
 
 .edit-section-form{
     display: flex;
     flex-wrap: wrap;
     gap: 2rem;
     padding-top: 1rem;
+    align-items: flex-end;
 }
 
 .alert-section{
     display: flex;
     flex-wrap: wrap;
     justify-content: space-around;
     gap: 1rem;
@@ -76,12 +77,7 @@
 .form-check.ssb-checkbox{
     align-self: center;
 }
 
 .form-check{
     padding-left: 0;
 }
-
-/*Target child selector (label) of variable-dropdown*/
-.ssb-dropdown.variable-dropdown > .dropdown-label{
-    margin-bottom: 0.6rem;
-}
```

### Comparing `ssb_datadoc-0.8.2/src/datadoc/backend/code_list.py` & `ssb_datadoc-0.8.3/src/datadoc/backend/code_list.py`

 * *Files identical despite different names*

### Comparing `ssb_datadoc-0.8.2/src/datadoc/backend/dapla_dataset_path_info.py` & `ssb_datadoc-0.8.3/src/datadoc/backend/dapla_dataset_path_info.py`

 * *Files identical despite different names*

### Comparing `ssb_datadoc-0.8.2/src/datadoc/backend/datadoc_metadata.py` & `ssb_datadoc-0.8.3/src/datadoc/backend/datadoc_metadata.py`

 * *Files identical despite different names*

### Comparing `ssb_datadoc-0.8.2/src/datadoc/backend/dataset_parser.py` & `ssb_datadoc-0.8.3/src/datadoc/backend/dataset_parser.py`

 * *Files identical despite different names*

### Comparing `ssb_datadoc-0.8.2/src/datadoc/backend/external_sources/external_sources.py` & `ssb_datadoc-0.8.3/src/datadoc/backend/external_sources/external_sources.py`

 * *Files identical despite different names*

### Comparing `ssb_datadoc-0.8.2/src/datadoc/backend/model_backwards_compatibility.py` & `ssb_datadoc-0.8.3/src/datadoc/backend/model_backwards_compatibility.py`

 * *Files identical despite different names*

### Comparing `ssb_datadoc-0.8.2/src/datadoc/backend/statistic_subject_mapping.py` & `ssb_datadoc-0.8.3/src/datadoc/backend/statistic_subject_mapping.py`

 * *Files identical despite different names*

### Comparing `ssb_datadoc-0.8.2/src/datadoc/backend/user_info.py` & `ssb_datadoc-0.8.3/src/datadoc/backend/user_info.py`

 * *Files identical despite different names*

### Comparing `ssb_datadoc-0.8.2/src/datadoc/config.py` & `ssb_datadoc-0.8.3/src/datadoc/config.py`

 * *Files identical despite different names*

### Comparing `ssb_datadoc-0.8.2/src/datadoc/enums.py` & `ssb_datadoc-0.8.3/src/datadoc/enums.py`

 * *Files identical despite different names*

### Comparing `ssb_datadoc-0.8.2/src/datadoc/frontend/callbacks/dataset.py` & `ssb_datadoc-0.8.3/src/datadoc/frontend/callbacks/dataset.py`

 * *Files identical despite different names*

### Comparing `ssb_datadoc-0.8.2/src/datadoc/frontend/callbacks/register_callbacks.py` & `ssb_datadoc-0.8.3/src/datadoc/frontend/callbacks/register_callbacks.py`

 * *Files identical despite different names*

### Comparing `ssb_datadoc-0.8.2/src/datadoc/frontend/callbacks/utils.py` & `ssb_datadoc-0.8.3/src/datadoc/frontend/callbacks/utils.py`

 * *Files identical despite different names*

### Comparing `ssb_datadoc-0.8.2/src/datadoc/frontend/callbacks/variables.py` & `ssb_datadoc-0.8.3/src/datadoc/frontend/callbacks/variables.py`

 * *Files identical despite different names*

### Comparing `ssb_datadoc-0.8.2/src/datadoc/frontend/components/alerts.py` & `ssb_datadoc-0.8.3/src/datadoc/frontend/components/alerts.py`

 * *Files identical despite different names*

### Comparing `ssb_datadoc-0.8.2/src/datadoc/frontend/components/builders.py` & `ssb_datadoc-0.8.3/src/datadoc/frontend/components/builders.py`

 * *Files identical despite different names*

### Comparing `ssb_datadoc-0.8.2/src/datadoc/frontend/components/control_bars.py` & `ssb_datadoc-0.8.3/src/datadoc/frontend/components/control_bars.py`

 * *Files identical despite different names*

### Comparing `ssb_datadoc-0.8.2/src/datadoc/frontend/components/dataset_tab.py` & `ssb_datadoc-0.8.3/src/datadoc/frontend/components/dataset_tab.py`

 * *Files identical despite different names*

### Comparing `ssb_datadoc-0.8.2/src/datadoc/frontend/components/variables_tab.py` & `ssb_datadoc-0.8.3/src/datadoc/frontend/components/variables_tab.py`

 * *Files identical despite different names*

### Comparing `ssb_datadoc-0.8.2/src/datadoc/frontend/fields/display_base.py` & `ssb_datadoc-0.8.3/src/datadoc/frontend/fields/display_base.py`

 * *Files identical despite different names*

### Comparing `ssb_datadoc-0.8.2/src/datadoc/frontend/fields/display_dataset.py` & `ssb_datadoc-0.8.3/src/datadoc/frontend/fields/display_dataset.py`

 * *Files identical despite different names*

### Comparing `ssb_datadoc-0.8.2/src/datadoc/frontend/fields/display_variables.py` & `ssb_datadoc-0.8.3/src/datadoc/frontend/fields/display_variables.py`

 * *Files identical despite different names*

### Comparing `ssb_datadoc-0.8.2/src/datadoc/logging_configuration/json_formatter.py` & `ssb_datadoc-0.8.3/src/datadoc/logging_configuration/json_formatter.py`

 * *Files identical despite different names*

### Comparing `ssb_datadoc-0.8.2/src/datadoc/logging_configuration/logging_config.py` & `ssb_datadoc-0.8.3/src/datadoc/logging_configuration/logging_config.py`

 * *Files identical despite different names*

### Comparing `ssb_datadoc-0.8.2/src/datadoc/state.py` & `ssb_datadoc-0.8.3/src/datadoc/state.py`

 * *Files identical despite different names*

### Comparing `ssb_datadoc-0.8.2/src/datadoc/utils.py` & `ssb_datadoc-0.8.3/src/datadoc/utils.py`

 * *Files identical despite different names*

### Comparing `ssb_datadoc-0.8.2/PKG-INFO` & `ssb_datadoc-0.8.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ssb-datadoc
-Version: 0.8.2
+Version: 0.8.3
 Summary: Document dataset metadata. For use in Statistics Norway's metadata system.
 Home-page: https://github.com/statisticsnorway/datadoc
 License: MIT
 Author: Statistics Norway
 Author-email: stat-dev@ssb.no
 Requires-Python: >=3.10,<4.0
 Classifier: Development Status :: 4 - Beta
```

