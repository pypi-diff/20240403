# Comparing `tmp/conformal_eval-1.0.0b2.tar.gz` & `tmp/conformal_eval-1.0.0b3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "conformal_eval-1.0.0b2.tar", max compression
+gzip compressed data, was "conformal_eval-1.0.0b3.tar", max compression
```

## Comparing `conformal_eval-1.0.0b2.tar` & `conformal_eval-1.0.0b3.tar`

### file list

```diff
@@ -1,26 +1,26 @@
--rw-r--r--   0        0        0     1059 2024-02-17 06:44:10.566376 conformal_eval-1.0.0b2/LICENSE.txt
--rw-r--r--   0        0        0     7059 2024-02-17 06:44:10.566376 conformal_eval-1.0.0b2/README.md
--rw-r--r--   0        0        0     1308 2024-02-17 06:44:10.590376 conformal_eval-1.0.0b2/pyproject.toml
--rw-r--r--   0        0        0       24 2024-02-17 06:44:10.590376 conformal_eval-1.0.0b2/src/conf_eval/__init__.py
--rw-r--r--   0        0        0     8368 2024-02-17 06:44:10.590376 conformal_eval-1.0.0b2/src/conf_eval/_utils.py
--rw-r--r--   0        0        0       21 2024-02-17 06:44:10.590376 conformal_eval-1.0.0b2/src/conf_eval/cpsign/__init__.py
--rw-r--r--   0        0        0    20207 2024-02-17 06:44:10.594376 conformal_eval-1.0.0b2/src/conf_eval/cpsign/_load.py
--rw-r--r--   0        0        0       20 2024-02-17 06:44:10.594376 conformal_eval-1.0.0b2/src/conf_eval/cpsign/report/__init__.py
--rw-r--r--   0        0        0    12796 2024-02-17 06:44:10.594376 conformal_eval-1.0.0b2/src/conf_eval/cpsign/report/_html.py
--rw-r--r--   0        0        0    24517 2024-02-17 06:44:10.594376 conformal_eval-1.0.0b2/src/conf_eval/cpsign/report/_static/UU_logo.svg
--rw-r--r--   0        0        0     9101 2024-02-17 06:44:10.594376 conformal_eval-1.0.0b2/src/conf_eval/cpsign/report/_static/arosbio-logo.png
--rw-r--r--   0        0        0    49936 2024-02-17 06:44:10.594376 conformal_eval-1.0.0b2/src/conf_eval/cpsign/report/_static/pharmbio-logo-new.png
--rw-r--r--   0        0        0     3378 2024-02-17 06:44:10.594376 conformal_eval-1.0.0b2/src/conf_eval/cpsign/report/_static/style.css
--rw-r--r--   0        0        0     1069 2024-02-17 06:44:10.594376 conformal_eval-1.0.0b2/src/conf_eval/cpsign/report/_templates/cp_metrics_template.html
--rw-r--r--   0        0        0     2530 2024-02-17 06:44:10.594376 conformal_eval-1.0.0b2/src/conf_eval/cpsign/report/_templates/template.html
--rw-r--r--   0        0        0      436 2024-02-17 06:44:10.594376 conformal_eval-1.0.0b2/src/conf_eval/cpsign/report/_templates/vap_metrics_template.html
--rw-r--r--   0        0        0     2085 2024-02-17 06:44:10.594376 conformal_eval-1.0.0b2/src/conf_eval/cpsign/report/html.py
--rw-r--r--   0        0        0      243 2024-02-17 06:44:10.594376 conformal_eval-1.0.0b2/src/conf_eval/metrics/__init__.py
--rw-r--r--   0        0        0    20880 2024-02-17 06:44:10.594376 conformal_eval-1.0.0b2/src/conf_eval/metrics/_classification.py
--rw-r--r--   0        0        0     2943 2024-02-17 06:44:10.594376 conformal_eval-1.0.0b2/src/conf_eval/metrics/_regression.py
--rw-r--r--   0        0        0      326 2024-02-17 06:44:10.594376 conformal_eval-1.0.0b2/src/conf_eval/plot/__init__.py
--rw-r--r--   0        0        0    40801 2024-02-17 06:44:10.594376 conformal_eval-1.0.0b2/src/conf_eval/plot/_classification.py
--rw-r--r--   0        0        0    12690 2024-02-17 06:44:10.594376 conformal_eval-1.0.0b2/src/conf_eval/plot/_common.py
--rw-r--r--   0        0        0     9295 2024-02-17 06:44:10.594376 conformal_eval-1.0.0b2/src/conf_eval/plot/_regression.py
--rw-r--r--   0        0        0     5946 2024-02-17 06:44:10.594376 conformal_eval-1.0.0b2/src/conf_eval/plot/_utils.py
--rw-r--r--   0        0        0     8147 1970-01-01 00:00:00.000000 conformal_eval-1.0.0b2/PKG-INFO
+-rw-r--r--   0        0        0     1059 2024-04-03 07:35:35.102782 conformal_eval-1.0.0b3/LICENSE.txt
+-rw-r--r--   0        0        0     7434 2024-04-03 07:35:35.102782 conformal_eval-1.0.0b3/README.md
+-rw-r--r--   0        0        0     1308 2024-04-03 07:35:35.126782 conformal_eval-1.0.0b3/pyproject.toml
+-rw-r--r--   0        0        0       24 2024-04-03 07:35:35.126782 conformal_eval-1.0.0b3/src/conf_eval/__init__.py
+-rw-r--r--   0        0        0     8368 2024-04-03 07:35:35.126782 conformal_eval-1.0.0b3/src/conf_eval/_utils.py
+-rw-r--r--   0        0        0       21 2024-04-03 07:35:35.126782 conformal_eval-1.0.0b3/src/conf_eval/cpsign/__init__.py
+-rw-r--r--   0        0        0    20207 2024-04-03 07:35:35.126782 conformal_eval-1.0.0b3/src/conf_eval/cpsign/_load.py
+-rw-r--r--   0        0        0       20 2024-04-03 07:35:35.126782 conformal_eval-1.0.0b3/src/conf_eval/cpsign/report/__init__.py
+-rw-r--r--   0        0        0    12926 2024-04-03 07:35:35.126782 conformal_eval-1.0.0b3/src/conf_eval/cpsign/report/_html.py
+-rw-r--r--   0        0        0    24517 2024-04-03 07:35:35.130782 conformal_eval-1.0.0b3/src/conf_eval/cpsign/report/_static/UU_logo.svg
+-rw-r--r--   0        0        0     9101 2024-04-03 07:35:35.130782 conformal_eval-1.0.0b3/src/conf_eval/cpsign/report/_static/arosbio-logo.png
+-rw-r--r--   0        0        0    49936 2024-04-03 07:35:35.130782 conformal_eval-1.0.0b3/src/conf_eval/cpsign/report/_static/pharmbio-logo-new.png
+-rw-r--r--   0        0        0     3378 2024-04-03 07:35:35.130782 conformal_eval-1.0.0b3/src/conf_eval/cpsign/report/_static/style.css
+-rw-r--r--   0        0        0     1069 2024-04-03 07:35:35.130782 conformal_eval-1.0.0b3/src/conf_eval/cpsign/report/_templates/cp_metrics_template.html
+-rw-r--r--   0        0        0     2560 2024-04-03 07:35:35.130782 conformal_eval-1.0.0b3/src/conf_eval/cpsign/report/_templates/template.html
+-rw-r--r--   0        0        0      436 2024-04-03 07:35:35.130782 conformal_eval-1.0.0b3/src/conf_eval/cpsign/report/_templates/vap_metrics_template.html
+-rw-r--r--   0        0        0     2085 2024-04-03 07:35:35.130782 conformal_eval-1.0.0b3/src/conf_eval/cpsign/report/html.py
+-rw-r--r--   0        0        0      243 2024-04-03 07:35:35.130782 conformal_eval-1.0.0b3/src/conf_eval/metrics/__init__.py
+-rw-r--r--   0        0        0    20880 2024-04-03 07:35:35.130782 conformal_eval-1.0.0b3/src/conf_eval/metrics/_classification.py
+-rw-r--r--   0        0        0     2943 2024-04-03 07:35:35.130782 conformal_eval-1.0.0b3/src/conf_eval/metrics/_regression.py
+-rw-r--r--   0        0        0      326 2024-04-03 07:35:35.130782 conformal_eval-1.0.0b3/src/conf_eval/plot/__init__.py
+-rw-r--r--   0        0        0    40801 2024-04-03 07:35:35.130782 conformal_eval-1.0.0b3/src/conf_eval/plot/_classification.py
+-rw-r--r--   0        0        0    12690 2024-04-03 07:35:35.130782 conformal_eval-1.0.0b3/src/conf_eval/plot/_common.py
+-rw-r--r--   0        0        0     9295 2024-04-03 07:35:35.130782 conformal_eval-1.0.0b3/src/conf_eval/plot/_regression.py
+-rw-r--r--   0        0        0     5946 2024-04-03 07:35:35.130782 conformal_eval-1.0.0b3/src/conf_eval/plot/_utils.py
+-rw-r--r--   0        0        0     8522 1970-01-01 00:00:00.000000 conformal_eval-1.0.0b3/PKG-INFO
```

### Comparing `conformal_eval-1.0.0b2/LICENSE.txt` & `conformal_eval-1.0.0b3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `conformal_eval-1.0.0b2/README.md` & `conformal_eval-1.0.0b3/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -12,17 +12,17 @@
 # or, depending on your shell you might need:
 pip install "conformal-eval[report]"
 ```
 
 
 ## Examples
 Examples of using the package can be seen in our examples notebooks: 
-- [Conformal Classification](examples/User_guide_classification.ipynb)
-- [Conformal Regression](examples/User_guide_regression.ipynb)
-- [Using Nonconformist and conf-eval](examples/Nonconformist_and_conformal-eval.ipynb)
+- [Conformal Classification](https://github.com/pharmbio/conformal-eval/tree/master/examples/User_guide_classification.ipynb)
+- [Conformal Regression](https://github.com/pharmbio/conformal-eval/tree/master/examples/User_guide_regression.ipynb)
+- [Using Nonconformist and conf-eval](https://github.com/pharmbio/conformal-eval/tree/master/examples/Nonconformist_and_conformal-eval.ipynb)
 
 ## Package dependencies
 Package dependencies can be found in the [pyproject.toml](pyproject.toml) under `[tool.poetry.dependencies]`, noting that the `Jinja2` package is only required for for the `report` extras (installing `conformal-eval[report]`).
 
 ## API
 
 ### Data format
@@ -85,14 +85,17 @@
  - [x] heatmap - Staffan
  - [x] p0-p1 plot - Staffan
  - [x] Add regression metrics
  - [x] Add plots regression
 
 
 ### Change log:
+- **1.0.0b3**:
+    * Allow to configure the 'static' output directory, to e.g. avoid path clashes with other files. 
+    * Change links in README to absolute urls to github, so they work at PyPI when deployed.
 - **1.0.0b2**:
     * Added the png-logo files for the `cpsign-report` utility (gitignore had removed them before). 
 - **1.0.0b1**:
     * Forked the [plot_utils](https://github.com/pharmbio/plot_utils) library to make an extensive refactor of module names.
     * Added `conf_eval.cpsign.report` module for generating model-reports in HTML format. The extras `report` is needed to run this code.
     * Fixed bugs when loading data from CPSign, e.g. missing standard-deviation columns in validation metrics.
     * Added new flag (`skip_inf`) when loading regression predictions and results, where a too high confidence level leads to infinitely large prediction intervals. This simply filters out the rows that have infinitely large outputs.
```

### Comparing `conformal_eval-1.0.0b2/pyproject.toml` & `conformal_eval-1.0.0b3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "conformal-eval"
-version = "1.0.0b2"
+version = "1.0.0b3"
 description = "A package with utility functions for evaluating conformal predictors"
 authors = ["Staffan Arvidsson McShane <staffan.arvidsson@gmail.com>"]
 license = "MIT"
 
 # URL metadata
 homepage = "https://github.com/pharmbio/conformal-eval"
 repository = "https://github.com/pharmbio/conformal-eval"
```

### Comparing `conformal_eval-1.0.0b2/src/conf_eval/_utils.py` & `conformal_eval-1.0.0b3/src/conf_eval/_utils.py`

 * *Files identical despite different names*

### Comparing `conformal_eval-1.0.0b2/src/conf_eval/cpsign/_load.py` & `conformal_eval-1.0.0b3/src/conf_eval/cpsign/_load.py`

 * *Files identical despite different names*

### Comparing `conformal_eval-1.0.0b2/src/conf_eval/cpsign/report/_html.py` & `conformal_eval-1.0.0b3/src/conf_eval/cpsign/report/_html.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     from jinja2 import Environment, FileSystemLoader
 except ImportError:
     raise ImportError("The 'report' extras are required to generate a report. Install them with 'pip install conformal-eval[report]'.")
     
 
 
 _static_sub_dir_name = "_static"
-_static_output_dir_name = "static"
+_static_output_dir_name = "_static"
 
 _default_page_name = "model-report.html"
 _package_dir = Path(__file__).absolute().parent
 _template_dir = _package_dir /"_templates"
 _figsize = (6,4)
 
 def generate_html(model_file: Union[str, Path],
@@ -66,15 +66,16 @@
     data = {
         'title': 'Model report',
         'heading': 'Model report: {}'.format(param_section['modelName']),
         'cpsign_build_version': cpsign_version,
         'pt_type' : __get_pt_type(param_section['predictor']['mlPredictorType']),
         'n_observations': param_section['data']['nrObservations'],
         'n_features': param_section['data']['nrFeatures'],
-        'if_clf': __get_clf_extra_info(param_section['data'])
+        'if_clf': __get_clf_extra_info(param_section['data']),
+        'static_dir': _static_output_dir_name
     }
     # Add hyper-parameter table
     ml_settings_matrix = []
     for key,val in param_section['predictor'].items():
         if key.endswith('Name') and "mlImplementationName" not in key:
             ml_settings_matrix.append([key,val])
     data['ml_settings_table'] = ml_settings_matrix
@@ -275,15 +276,16 @@
     # Generate a table of the other metrics
     metric_dict = cpsign.load_conf_independent_metrics(validation_file,sep=dialect.delimiter)
     metric_table = [[key, value] for key, value in metric_dict.items()]
     
     val_html = validation_template.render({'calib_src' : _static_output_dir_name+'/calibration_fig.svg',
                                            'eff_src' : _static_output_dir_name+'/efficiency_fig.svg',
                                            'eff_caption' : eff_caption,
-                                           'metric_table' : metric_table})
+                                           'metric_table' : metric_table,
+                                           'static_dir': _static_output_dir_name})
     
     return val_html
     
 def __generate_cvap_validation_section(validation_file,validation_template,output_dir: str):
     if validation_file is None:
         return None
```

### Comparing `conformal_eval-1.0.0b2/src/conf_eval/cpsign/report/_static/UU_logo.svg` & `conformal_eval-1.0.0b3/src/conf_eval/cpsign/report/_static/UU_logo.svg`

 * *Files identical despite different names*

### Comparing `conformal_eval-1.0.0b2/src/conf_eval/cpsign/report/_static/arosbio-logo.png` & `conformal_eval-1.0.0b3/src/conf_eval/cpsign/report/_static/arosbio-logo.png`

 * *Files identical despite different names*

### Comparing `conformal_eval-1.0.0b2/src/conf_eval/cpsign/report/_static/pharmbio-logo-new.png` & `conformal_eval-1.0.0b3/src/conf_eval/cpsign/report/_static/pharmbio-logo-new.png`

 * *Files identical despite different names*

### Comparing `conformal_eval-1.0.0b2/src/conf_eval/cpsign/report/_static/style.css` & `conformal_eval-1.0.0b3/src/conf_eval/cpsign/report/_static/style.css`

 * *Files identical despite different names*

### Comparing `conformal_eval-1.0.0b2/src/conf_eval/cpsign/report/_templates/cp_metrics_template.html` & `conformal_eval-1.0.0b3/src/conf_eval/cpsign/report/_templates/cp_metrics_template.html`

 * *Files identical despite different names*

### Comparing `conformal_eval-1.0.0b2/src/conf_eval/cpsign/report/_templates/template.html` & `conformal_eval-1.0.0b3/src/conf_eval/cpsign/report/_templates/template.html`

 * *Files 21% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 <!DOCTYPE html>
 <html lang="en">
     <head>
         <meta charset="UTF-8">
         <title>{% if title %}{{ title }}{% else %}Model report{% endif %}</title>
-        <link rel="stylesheet" href="static/style.css">
+        <link rel="stylesheet" href="{{ static_dir }}/style.css">
     </head>
     <body>
         <h1>{%if heading %}{{ heading }} {% else %}Model report{% endif %}</h1>
         <p>
         {% if intro %}
             {{intro}}
         {% else %}
@@ -45,18 +45,18 @@
         <!-- Add a section with validation metrics produced for this model (if present) -->
         {% if validation_section %}{{validation_section}}{% endif %}
         
         <footer>
             <div class="container">
 
                 <div class="pharmbio">
-                    <a href="https://pharmb.io/"><img src="static/pharmbio-logo-new.png" alt="Pharmbio logo"></a>
+                    <a href="https://pharmb.io/"><img src="{{ static_dir }}/pharmbio-logo-new.png" alt="Pharmbio logo"></a>
                 </div>
 
                 <div class="arosbio">
-                    <a href="https://arosbio.com"><img src="static/arosbio-logo.png" alt="Aros Bio"></a> 
+                    <a href="https://arosbio.com"><img src="{{ static_dir }}/arosbio-logo.png" alt="Aros Bio"></a> 
                 </div>
 
             </div>
         </footer>
     </body>
 </html>
```

### Comparing `conformal_eval-1.0.0b2/src/conf_eval/cpsign/report/html.py` & `conformal_eval-1.0.0b3/src/conf_eval/cpsign/report/html.py`

 * *Files identical despite different names*

### Comparing `conformal_eval-1.0.0b2/src/conf_eval/metrics/_classification.py` & `conformal_eval-1.0.0b3/src/conf_eval/metrics/_classification.py`

 * *Files identical despite different names*

### Comparing `conformal_eval-1.0.0b2/src/conf_eval/metrics/_regression.py` & `conformal_eval-1.0.0b3/src/conf_eval/metrics/_regression.py`

 * *Files identical despite different names*

### Comparing `conformal_eval-1.0.0b2/src/conf_eval/plot/_classification.py` & `conformal_eval-1.0.0b3/src/conf_eval/plot/_classification.py`

 * *Files identical despite different names*

### Comparing `conformal_eval-1.0.0b2/src/conf_eval/plot/_common.py` & `conformal_eval-1.0.0b3/src/conf_eval/plot/_common.py`

 * *Files identical despite different names*

### Comparing `conformal_eval-1.0.0b2/src/conf_eval/plot/_regression.py` & `conformal_eval-1.0.0b3/src/conf_eval/plot/_regression.py`

 * *Files identical despite different names*

### Comparing `conformal_eval-1.0.0b2/src/conf_eval/plot/_utils.py` & `conformal_eval-1.0.0b3/src/conf_eval/plot/_utils.py`

 * *Files identical despite different names*

### Comparing `conformal_eval-1.0.0b2/PKG-INFO` & `conformal_eval-1.0.0b3/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: conformal-eval
-Version: 1.0.0b2
+Version: 1.0.0b3
 Summary: A package with utility functions for evaluating conformal predictors
 Home-page: https://github.com/pharmbio/conformal-eval
 License: MIT
 Author: Staffan Arvidsson McShane
 Author-email: staffan.arvidsson@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
@@ -39,17 +39,17 @@
 # or, depending on your shell you might need:
 pip install "conformal-eval[report]"
 ```
 
 
 ## Examples
 Examples of using the package can be seen in our examples notebooks: 
-- [Conformal Classification](examples/User_guide_classification.ipynb)
-- [Conformal Regression](examples/User_guide_regression.ipynb)
-- [Using Nonconformist and conf-eval](examples/Nonconformist_and_conformal-eval.ipynb)
+- [Conformal Classification](https://github.com/pharmbio/conformal-eval/tree/master/examples/User_guide_classification.ipynb)
+- [Conformal Regression](https://github.com/pharmbio/conformal-eval/tree/master/examples/User_guide_regression.ipynb)
+- [Using Nonconformist and conf-eval](https://github.com/pharmbio/conformal-eval/tree/master/examples/Nonconformist_and_conformal-eval.ipynb)
 
 ## Package dependencies
 Package dependencies can be found in the [pyproject.toml](pyproject.toml) under `[tool.poetry.dependencies]`, noting that the `Jinja2` package is only required for for the `report` extras (installing `conformal-eval[report]`).
 
 ## API
 
 ### Data format
@@ -112,14 +112,17 @@
  - [x] heatmap - Staffan
  - [x] p0-p1 plot - Staffan
  - [x] Add regression metrics
  - [x] Add plots regression
 
 
 ### Change log:
+- **1.0.0b3**:
+    * Allow to configure the 'static' output directory, to e.g. avoid path clashes with other files. 
+    * Change links in README to absolute urls to github, so they work at PyPI when deployed.
 - **1.0.0b2**:
     * Added the png-logo files for the `cpsign-report` utility (gitignore had removed them before). 
 - **1.0.0b1**:
     * Forked the [plot_utils](https://github.com/pharmbio/plot_utils) library to make an extensive refactor of module names.
     * Added `conf_eval.cpsign.report` module for generating model-reports in HTML format. The extras `report` is needed to run this code.
     * Fixed bugs when loading data from CPSign, e.g. missing standard-deviation columns in validation metrics.
     * Added new flag (`skip_inf`) when loading regression predictions and results, where a too high confidence level leads to infinitely large prediction intervals. This simply filters out the rows that have infinitely large outputs.
```

