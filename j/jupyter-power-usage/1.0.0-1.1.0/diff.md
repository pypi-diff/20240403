# Comparing `tmp/jupyter_power_usage-1.0.0.tar.gz` & `tmp/jupyter_power_usage-1.1.0.tar.gz`

## Comparing `jupyter_power_usage-1.0.0.tar` & `jupyter_power_usage-1.1.0.tar`

### file list

```diff
@@ -1,49 +1,49 @@
--rw-r--r--   0        0        0      350 2020-02-02 00:00:00.000000 jupyter_power_usage-1.0.0/.flake8
--rw-r--r--   0        0        0     1275 2020-02-02 00:00:00.000000 jupyter_power_usage-1.0.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 jupyter_power_usage-1.0.0/.prettierignore
--rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 jupyter_power_usage-1.0.0/.yarnrc.yml
--rw-r--r--   0        0        0     1849 2020-02-02 00:00:00.000000 jupyter_power_usage-1.0.0/CHANGELOG.md
--rw-r--r--   0        0        0     4701 2020-02-02 00:00:00.000000 jupyter_power_usage-1.0.0/CONTRIBUTING.md
--rw-r--r--   0        0        0      221 2020-02-02 00:00:00.000000 jupyter_power_usage-1.0.0/RELEASE.md
--rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 jupyter_power_usage-1.0.0/install.json
--rw-r--r--   0        0        0     6288 2020-02-02 00:00:00.000000 jupyter_power_usage-1.0.0/package.json
--rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 jupyter_power_usage-1.0.0/setup.py
--rw-r--r--   0        0        0      566 2020-02-02 00:00:00.000000 jupyter_power_usage-1.0.0/tsconfig.json
--rw-r--r--   0        0        0   183801 2020-02-02 00:00:00.000000 jupyter_power_usage-1.0.0/yarn.lock
--rw-r--r--   0        0        0    68927 2020-02-02 00:00:00.000000 jupyter_power_usage-1.0.0/doc/frontend-settings.png
--rw-r--r--   0        0        0    12874 2020-02-02 00:00:00.000000 jupyter_power_usage-1.0.0/doc/power-usage.gif
--rw-r--r--   0        0        0     1743 2020-02-02 00:00:00.000000 jupyter_power_usage-1.0.0/jupyter_power_usage/__init__.py
--rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 jupyter_power_usage-1.0.0/jupyter_power_usage/_version.py
--rw-r--r--   0        0        0     3428 2020-02-02 00:00:00.000000 jupyter_power_usage-1.0.0/jupyter_power_usage/api.py
--rw-r--r--   0        0        0     1617 2020-02-02 00:00:00.000000 jupyter_power_usage-1.0.0/jupyter_power_usage/config.py
--rw-r--r--   0        0        0     8507 2020-02-02 00:00:00.000000 jupyter_power_usage-1.0.0/jupyter_power_usage/metrics.py
--rw-r--r--   0        0        0     7284 2020-02-02 00:00:00.000000 jupyter_power_usage-1.0.0/jupyter_power_usage/utils.py
--rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 jupyter_power_usage-1.0.0/jupyter_power_usage/etc/jupyter_server_config.d/jupyter-power-usage.json
--rw-r--r--   0        0        0     5624 2020-02-02 00:00:00.000000 jupyter_power_usage-1.0.0/jupyter_power_usage/labextension/package.json
--rw-r--r--   0        0        0     6288 2020-02-02 00:00:00.000000 jupyter_power_usage-1.0.0/jupyter_power_usage/labextension/schemas/@mahendrapaipuri/jupyter-power-usage/package.json.orig
--rw-r--r--   0        0        0     2607 2020-02-02 00:00:00.000000 jupyter_power_usage-1.0.0/jupyter_power_usage/labextension/schemas/@mahendrapaipuri/jupyter-power-usage/plugin.json
--rw-r--r--   0        0        0    14473 2020-02-02 00:00:00.000000 jupyter_power_usage-1.0.0/jupyter_power_usage/labextension/static/32.df2f2b30253633c749ea.js
--rw-r--r--   0        0        0    28319 2020-02-02 00:00:00.000000 jupyter_power_usage-1.0.0/jupyter_power_usage/labextension/static/646.92e3ed3d9aea0d36c6a9.js
--rw-r--r--   0        0        0     4628 2020-02-02 00:00:00.000000 jupyter_power_usage-1.0.0/jupyter_power_usage/labextension/static/747.19551df7a36576f1c11f.js
--rw-r--r--   0        0        0     7413 2020-02-02 00:00:00.000000 jupyter_power_usage-1.0.0/jupyter_power_usage/labextension/static/remoteEntry.8012d710f1db7c034cba.js
--rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 jupyter_power_usage-1.0.0/jupyter_power_usage/labextension/static/style.js
--rw-r--r--   0        0        0     3687 2020-02-02 00:00:00.000000 jupyter_power_usage-1.0.0/jupyter_power_usage/labextension/static/third-party-licenses.json
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jupyter_power_usage-1.0.0/jupyter_power_usage/tests/__init__.py
--rw-r--r--   0        0        0     1066 2020-02-02 00:00:00.000000 jupyter_power_usage-1.0.0/jupyter_power_usage/tests/test_basic.py
--rw-r--r--   0        0        0     2607 2020-02-02 00:00:00.000000 jupyter_power_usage-1.0.0/schema/plugin.json
--rw-r--r--   0        0        0     1521 2020-02-02 00:00:00.000000 jupyter_power_usage-1.0.0/src/cpuPowerView.tsx
--rw-r--r--   0        0        0     1877 2020-02-02 00:00:00.000000 jupyter_power_usage-1.0.0/src/emissionsHandler.ts
--rw-r--r--   0        0        0     1621 2020-02-02 00:00:00.000000 jupyter_power_usage-1.0.0/src/emissionsView.tsx
--rw-r--r--   0        0        0     1009 2020-02-02 00:00:00.000000 jupyter_power_usage-1.0.0/src/format.ts
--rw-r--r--   0        0        0     1506 2020-02-02 00:00:00.000000 jupyter_power_usage-1.0.0/src/gpuPowerView.tsx
--rw-r--r--   0        0        0     4710 2020-02-02 00:00:00.000000 jupyter_power_usage-1.0.0/src/index.ts
--rw-r--r--   0        0        0     2299 2020-02-02 00:00:00.000000 jupyter_power_usage-1.0.0/src/indicator.tsx
--rw-r--r--   0        0        0    13579 2020-02-02 00:00:00.000000 jupyter_power_usage-1.0.0/src/model.ts
--rw-r--r--   0        0        0      674 2020-02-02 00:00:00.000000 jupyter_power_usage-1.0.0/style/base.css
--rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 jupyter_power_usage-1.0.0/style/index.css
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 jupyter_power_usage-1.0.0/style/index.js
--rw-r--r--   0        0        0     1550 2020-02-02 00:00:00.000000 jupyter_power_usage-1.0.0/.gitignore
--rw-r--r--   0        0        0    11345 2020-02-02 00:00:00.000000 jupyter_power_usage-1.0.0/LICENSE
--rw-r--r--   0        0        0     5942 2020-02-02 00:00:00.000000 jupyter_power_usage-1.0.0/README.md
--rw-r--r--   0        0        0     3910 2020-02-02 00:00:00.000000 jupyter_power_usage-1.0.0/pyproject.toml
--rw-r--r--   0        0        0    20363 2020-02-02 00:00:00.000000 jupyter_power_usage-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0      350 2020-02-02 00:00:00.000000 jupyter_power_usage-1.1.0/.flake8
+-rw-r--r--   0        0        0     1290 2020-02-02 00:00:00.000000 jupyter_power_usage-1.1.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 jupyter_power_usage-1.1.0/.prettierignore
+-rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 jupyter_power_usage-1.1.0/.yarnrc.yml
+-rw-r--r--   0        0        0     2892 2020-02-02 00:00:00.000000 jupyter_power_usage-1.1.0/CHANGELOG.md
+-rw-r--r--   0        0        0     4710 2020-02-02 00:00:00.000000 jupyter_power_usage-1.1.0/CONTRIBUTING.md
+-rw-r--r--   0        0        0      221 2020-02-02 00:00:00.000000 jupyter_power_usage-1.1.0/RELEASE.md
+-rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 jupyter_power_usage-1.1.0/install.json
+-rw-r--r--   0        0        0     6288 2020-02-02 00:00:00.000000 jupyter_power_usage-1.1.0/package.json
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 jupyter_power_usage-1.1.0/setup.py
+-rw-r--r--   0        0        0      566 2020-02-02 00:00:00.000000 jupyter_power_usage-1.1.0/tsconfig.json
+-rw-r--r--   0        0        0   183801 2020-02-02 00:00:00.000000 jupyter_power_usage-1.1.0/yarn.lock
+-rw-r--r--   0        0        0    69248 2020-02-02 00:00:00.000000 jupyter_power_usage-1.1.0/doc/frontend-settings.png
+-rw-r--r--   0        0        0    12874 2020-02-02 00:00:00.000000 jupyter_power_usage-1.1.0/doc/power-usage.gif
+-rw-r--r--   0        0        0     1353 2020-02-02 00:00:00.000000 jupyter_power_usage-1.1.0/jupyter_power_usage/__init__.py
+-rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 jupyter_power_usage-1.1.0/jupyter_power_usage/_version.py
+-rw-r--r--   0        0        0     5422 2020-02-02 00:00:00.000000 jupyter_power_usage-1.1.0/jupyter_power_usage/api.py
+-rw-r--r--   0        0        0     1112 2020-02-02 00:00:00.000000 jupyter_power_usage-1.1.0/jupyter_power_usage/config.py
+-rw-r--r--   0        0        0    10065 2020-02-02 00:00:00.000000 jupyter_power_usage-1.1.0/jupyter_power_usage/metrics.py
+-rw-r--r--   0        0        0     6707 2020-02-02 00:00:00.000000 jupyter_power_usage-1.1.0/jupyter_power_usage/utils.py
+-rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 jupyter_power_usage-1.1.0/jupyter_power_usage/etc/jupyter_server_config.d/jupyter-power-usage.json
+-rw-r--r--   0        0        0     5624 2020-02-02 00:00:00.000000 jupyter_power_usage-1.1.0/jupyter_power_usage/labextension/package.json
+-rw-r--r--   0        0        0     6288 2020-02-02 00:00:00.000000 jupyter_power_usage-1.1.0/jupyter_power_usage/labextension/schemas/@mahendrapaipuri/jupyter-power-usage/package.json.orig
+-rw-r--r--   0        0        0     3266 2020-02-02 00:00:00.000000 jupyter_power_usage-1.1.0/jupyter_power_usage/labextension/schemas/@mahendrapaipuri/jupyter-power-usage/plugin.json
+-rw-r--r--   0        0        0    15861 2020-02-02 00:00:00.000000 jupyter_power_usage-1.1.0/jupyter_power_usage/labextension/static/32.d626a962b7bd9192a1da.js
+-rw-r--r--   0        0        0    28319 2020-02-02 00:00:00.000000 jupyter_power_usage-1.1.0/jupyter_power_usage/labextension/static/646.92e3ed3d9aea0d36c6a9.js
+-rw-r--r--   0        0        0     4628 2020-02-02 00:00:00.000000 jupyter_power_usage-1.1.0/jupyter_power_usage/labextension/static/747.19551df7a36576f1c11f.js
+-rw-r--r--   0        0        0     7409 2020-02-02 00:00:00.000000 jupyter_power_usage-1.1.0/jupyter_power_usage/labextension/static/remoteEntry.20fe913e7d7c5e7492d8.js
+-rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 jupyter_power_usage-1.1.0/jupyter_power_usage/labextension/static/style.js
+-rw-r--r--   0        0        0     3687 2020-02-02 00:00:00.000000 jupyter_power_usage-1.1.0/jupyter_power_usage/labextension/static/third-party-licenses.json
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jupyter_power_usage-1.1.0/jupyter_power_usage/tests/__init__.py
+-rw-r--r--   0        0        0     1066 2020-02-02 00:00:00.000000 jupyter_power_usage-1.1.0/jupyter_power_usage/tests/test_basic.py
+-rw-r--r--   0        0        0     3266 2020-02-02 00:00:00.000000 jupyter_power_usage-1.1.0/schema/plugin.json
+-rw-r--r--   0        0        0     1521 2020-02-02 00:00:00.000000 jupyter_power_usage-1.1.0/src/cpuPowerView.tsx
+-rw-r--r--   0        0        0     4189 2020-02-02 00:00:00.000000 jupyter_power_usage-1.1.0/src/emissionsHandler.ts
+-rw-r--r--   0        0        0     1621 2020-02-02 00:00:00.000000 jupyter_power_usage-1.1.0/src/emissionsView.tsx
+-rw-r--r--   0        0        0     1009 2020-02-02 00:00:00.000000 jupyter_power_usage-1.1.0/src/format.ts
+-rw-r--r--   0        0        0     1506 2020-02-02 00:00:00.000000 jupyter_power_usage-1.1.0/src/gpuPowerView.tsx
+-rw-r--r--   0        0        0     5173 2020-02-02 00:00:00.000000 jupyter_power_usage-1.1.0/src/index.ts
+-rw-r--r--   0        0        0     2299 2020-02-02 00:00:00.000000 jupyter_power_usage-1.1.0/src/indicator.tsx
+-rw-r--r--   0        0        0    15438 2020-02-02 00:00:00.000000 jupyter_power_usage-1.1.0/src/model.ts
+-rw-r--r--   0        0        0      674 2020-02-02 00:00:00.000000 jupyter_power_usage-1.1.0/style/base.css
+-rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 jupyter_power_usage-1.1.0/style/index.css
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 jupyter_power_usage-1.1.0/style/index.js
+-rw-r--r--   0        0        0     1550 2020-02-02 00:00:00.000000 jupyter_power_usage-1.1.0/.gitignore
+-rw-r--r--   0        0        0    11345 2020-02-02 00:00:00.000000 jupyter_power_usage-1.1.0/LICENSE
+-rw-r--r--   0        0        0     6638 2020-02-02 00:00:00.000000 jupyter_power_usage-1.1.0/README.md
+-rw-r--r--   0        0        0     3910 2020-02-02 00:00:00.000000 jupyter_power_usage-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0    21077 2020-02-02 00:00:00.000000 jupyter_power_usage-1.1.0/PKG-INFO
```

### Comparing `jupyter_power_usage-1.0.0/.pre-commit-config.yaml` & `jupyter_power_usage-1.1.0/.pre-commit-config.yaml`

 * *Files 8% similar despite different names*

```diff
@@ -1,42 +1,42 @@
 repos:
   - repo: https://github.com/asottile/reorder-python-imports
     rev: v3.12.0
     hooks:
       - id: reorder-python-imports
         language_version: python3
   - repo: https://github.com/psf/black
-    rev: 23.9.1
+    rev: 24.1.1
     hooks:
       - id: black
   - repo: https://github.com/PyCQA/flake8
-    rev: '6.1.0'
+    rev: '7.0.0'
     hooks:
       - id: flake8
   - repo: https://github.com/pre-commit/mirrors-prettier
-    rev: v3.0.0
+    rev: v4.0.0-alpha.8
     hooks:
       - id: prettier
         additional_dependencies:
           - prettier@2.8.4
   - repo: https://github.com/pre-commit/mirrors-eslint
-    rev: v8.43.0
+    rev: v9.0.0-alpha.2
     hooks:
       - id: eslint
         files: \.[jt]sx?$ # *.js, *.jsx, *.ts and *.tsx
         types: [file]
         additional_dependencies:
           - '@typescript-eslint/eslint-plugin@5.55.0'
           - '@typescript-eslint/parser@5.55.0'
           - eslint@^8.36.0
           - eslint-config-prettier@8.7.0
           - eslint-plugin-prettier@4.2.1
           - typescript@5.0.4
   - repo: https://github.com/pre-commit/pre-commit-hooks
-    rev: v4.4.0
+    rev: v4.5.0
     hooks:
       - id: end-of-file-fixer
       - id: check-json
       - id: check-yaml
         exclude: ^helm-chart/nbviewer/templates/
       - id: check-case-conflict
       - id: check-executables-have-shebangs
```

### Comparing `jupyter_power_usage-1.0.0/CHANGELOG.md` & `jupyter_power_usage-1.1.0/CHANGELOG.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,35 @@
 # Changelog
 
 <!-- <START NEW CHANGELOG ENTRY> -->
 
+## 1.1.0
+
+([Full Changelog](https://github.com/mahendrapaipuri/jupyter-power-usage/compare/v1.0.0...43f5a12b352e65bd810d75bb06608e605836ca4c))
+
+### Enhancements made
+
+- Electricity Maps Support [#9](https://github.com/mahendrapaipuri/jupyter-power-usage/pull/9) ([@mahendrapaipuri](https://github.com/mahendrapaipuri))
+
+### Bugs fixed
+
+- Fix CPU share estimation [#7](https://github.com/mahendrapaipuri/jupyter-power-usage/pull/7) ([@mahendrapaipuri](https://github.com/mahendrapaipuri))
+
+### Maintenance and upkeep improvements
+
+- Fix CPU share estimation [#7](https://github.com/mahendrapaipuri/jupyter-power-usage/pull/7) ([@mahendrapaipuri](https://github.com/mahendrapaipuri))
+
+### Contributors to this release
+
+([GitHub contributors page for this release](https://github.com/mahendrapaipuri/jupyter-power-usage/graphs/contributors?from=2023-10-12&to=2024-04-03&type=c))
+
+[@mahendrapaipuri](https://github.com/search?q=repo%3Amahendrapaipuri%2Fjupyter-power-usage+involves%3Amahendrapaipuri+updated%3A2023-10-12..2024-04-03&type=Issues)
+
+<!-- <END NEW CHANGELOG ENTRY> -->
+
 ## 1.0.0
 
 ([Full Changelog](https://github.com/mahendrapaipuri/jupyter-power-usage/compare/v0.1.1...62b1ee6d0ed0a662330c0156807b07e493eeb85a))
 
 ### Enhancements made
 
 - Upgrade to JupyterLab 4 [#4](https://github.com/mahendrapaipuri/jupyter-power-usage/pull/4) ([@mahendrapaipuri](https://github.com/mahendrapaipuri))
@@ -16,16 +40,14 @@
 
 ### Contributors to this release
 
 ([GitHub contributors page for this release](https://github.com/mahendrapaipuri/jupyter-power-usage/graphs/contributors?from=2023-10-12&to=2023-10-12&type=c))
 
 [@mahendrapaipuri](https://github.com/search?q=repo%3Amahendrapaipuri%2Fjupyter-power-usage+involves%3Amahendrapaipuri+updated%3A2023-10-12..2023-10-12&type=Issues)
 
-<!-- <END NEW CHANGELOG ENTRY> -->
-
 ## 0.1.1
 
 ([Full Changelog](https://github.com/mahendrapaipuri/jupyter-power-usage/compare/3b718a62b80160933904e991b2ebde25598434a5...d8fc444ef94e53dab89ce84192927d215558a82e))
 
 ### Maintenance and upkeep improvements
 
 - Update `package.json` config and README [#2](https://github.com/mahendrapaipuri/jupyter-power-usage/pull/2) ([@mahendrapaipuri](https://github.com/mahendrapaipuri))
```

### Comparing `jupyter_power_usage-1.0.0/CONTRIBUTING.md` & `jupyter_power_usage-1.1.0/CONTRIBUTING.md`

 * *Files 1% similar despite different names*

```diff
@@ -83,27 +83,27 @@
 
 ```bash
 JupyterLab v3.6.6
 /path/to/env/share/jupyter/labextensions
         @mahendrapaipuri/jupyter-power-usage v0.1.0 enabled OK
 ```
 
-## Estimating emission factor
+<!-- ## Estimating emission factor
 
 Currently only French real time emission factor is implemented in the extension to estimation eCO<sub>2</sub> emissions based on power usage. For the rest of the countries a constant emission factor that can be configurable is used.
 
 API requests for the emission factor is made from the frontend extension rather than backend server. The rationale is that the machine where backend server is running might not have internet connectivity. Also, these sort of API requests are rate limited and hence, making requests from individual user browser is more appropriate.
 
 In order to add support for other countries, users need to make changes in the file [emissionsHandler.ts](./src/emissionsHandler.ts) as follows:
 
 - Create a new namespace with name of the country.
 - Add all the necessary logic to get the emission factor in g/kWh for the country in its namespace.
 - Finally, modify `getEmissions` function in [emissionsHandler.ts](./src/emissionsHandler.ts) to get the emission factor of the country.
 
-We need to add the country code in the enum section of `countryCode` object in [plugin.json](./schema/plugin.json). This enables users to use this country specific emission factor to estimate emissions.
+We need to add the country code in the enum section of `countryCode` object in [plugin.json](./schema/plugin.json). This enables users to use this country specific emission factor to estimate emissions. -->
 
 ## pre-commit
 
 `jupyter-power-usage` has adopted automatic code formatting so you shouldn't need to worry too much about your code style.
 As long as your code is valid,
 the pre-commit hook should take care of how it should look. Here is how to set up pre-commit hooks for automatic code formatting, etc.
```

### Comparing `jupyter_power_usage-1.0.0/package.json` & `jupyter_power_usage-1.1.0/package.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9782608695652174%*

 * *Differences: {"'version'": "'1.1.0'"}*

```diff
@@ -170,9 +170,9 @@
             "property-no-vendor-prefix": null,
             "selector-class-pattern": null,
             "selector-no-vendor-prefix": null,
             "value-no-vendor-prefix": null
         }
     },
     "types": "lib/index.d.ts",
-    "version": "1.0.0"
+    "version": "1.1.0"
 }
```

### Comparing `jupyter_power_usage-1.0.0/tsconfig.json` & `jupyter_power_usage-1.1.0/tsconfig.json`

 * *Files identical despite different names*

### Comparing `jupyter_power_usage-1.0.0/yarn.lock` & `jupyter_power_usage-1.1.0/yarn.lock`

 * *Files identical despite different names*

### Comparing `jupyter_power_usage-1.0.0/doc/power-usage.gif` & `jupyter_power_usage-1.1.0/doc/power-usage.gif`

 * *Files identical despite different names*

### Comparing `jupyter_power_usage-1.0.0/jupyter_power_usage/metrics.py` & `jupyter_power_usage-1.1.0/jupyter_power_usage/metrics.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,20 +1,7 @@
-# Copyright 2023 IDRIS / jupyter
-#
-# Licensed under the Apache License, Version 2.0 (the "License");
-# you may not use this file except in compliance with the License.
-# You may obtain a copy of the License at
-#
-#     http://www.apache.org/licenses/LICENSE-2.0
-#
-# Unless required by applicable law or agreed to in writing, software
-# distributed under the License is distributed on an "AS IS" BASIS,
-# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-# See the License for the specific language governing permissions and
-# limitations under the License.
 import re
 import time
 
 import psutil
 from jupyter_server.serverapp import ServerApp
 from py3nvml.py3nvml import nvmlDeviceGetCount
 from py3nvml.py3nvml import nvmlDeviceGetEnforcedPowerLimit
@@ -26,14 +13,17 @@
 from .utils import filter_rapl_domains
 
 # Default power consumption for DRAM if counters are available
 # Units in W/GB RAM consumed
 # Source: https://arxiv.org/pdf/2306.08323.pdf
 DEFAULT_DRAM_CONSUMPTION = 0.375
 
+# Minimum share of procs in current scope
+CPU_SHARE_THRESHOLD = 0.001
+
 
 class CpuPowerUsage:
     """Extract CPU power usage using RAPL metrics"""
 
     def __init__(self, server_app: ServerApp):
         self.server_app = server_app
         self.config = server_app.web_app.settings['jupyter_power_usage_config']
@@ -57,25 +47,55 @@
         self._power_usage_available = False
         counters = self.get_rapl_counters()
         if sum(counters.values()) > 0:
             self._power_usage_available = True
 
             # Setup first readings
             self.rapl_readings_t = counters
+            self.total_cpu_time_t = self.get_total_cpu_time(psutil.cpu_times())
+            self.procs_cpu_time_t = self.total_cpu_time_t
             self.time_t = time.time()
 
     def power_usage_available(self):
         """Check if power metrics are available"""
         return self._power_usage_available
 
     def get_power_limit(self):
         """Get CPU power limit"""
         return self._power_limit
 
     @staticmethod
+    def get_total_cpu_time(cpu_times, proc=False):
+        """Get total CPU time at current time
+
+        Total cpu time excluding iowait, steal and idle. CPU is doing nothing in
+        these modes and so we exclude them.
+
+        If proc=True, sum only user and system cpu_times. Rest are not available
+        on cpu_times()
+
+        Example:
+        user=146611.61, nice=37933.89, system=74662.47, idle=3519011.28,
+        iowait=58120.7, irq=0.0, softirq=2281.55, steal=0.0, guest=0.0,
+        guest_nice=0.0
+        """
+        if proc:
+            return cpu_times.user + cpu_times.system
+        else:
+            return (
+                cpu_times.user
+                + cpu_times.nice
+                + cpu_times.system
+                + cpu_times.irq
+                + cpu_times.softirq
+                + cpu_times.guest
+                + cpu_times.guest_nice
+            )
+
+    @staticmethod
     def read_energy_counter(path):
         """Read energy counter file and return value"""
         try:
             content = open(path, 'r').read().rstrip()
             # Units are micro Joules
             return int(content)
         except (PermissionError, ValueError):
@@ -92,19 +112,40 @@
     def get_cpu_share(self, pids):
         """Get CPU share of processes based on defined scope"""
         # If system wide measurement is chosen we dont need to compute share
         # So return immediately with share as 1
         if self.config.measurement_scope == 'system':
             return 1, 1
 
-        # CPU share is sum of all process's cpu percents
-        cpu_share = sum(
-            [psutil.Process(pid=p).cpu_percent(interval=0.05) / 100 for p in pids]
+        # CPU share of current scope is rate(procs_cpu_time) / rate(total_cpu_time)
+        # This will give the share of cpu time of processes in current scope to TOTAL
+        # cpu time. We dont need to account for number of CPUs as it is a ratio
+        #
+        # Total CPU time of all processes in the current scope
+        procs_cpu_times = sum(
+            [
+                self.get_total_cpu_time(psutil.Process(pid=p).cpu_times(), proc=True)
+                for p in pids
+            ]
+        )
+        # Total CPU time of the host excluding times in IOwait, idle, steal
+        total_cpu_time = self.get_total_cpu_time(psutil.cpu_times())
+        cpu_share = (procs_cpu_times - self.procs_cpu_time_t) / (
+            total_cpu_time - self.total_cpu_time_t
         )
 
+        # cpu_share can be negative when there is a lot of CPU activity and if all
+        # activity disappears suddently, it tends to go negative. Use a threshold to
+        # avoid negative values
+        cpu_share = max(cpu_share, CPU_SHARE_THRESHOLD)
+
+        # Update the times at t which will be used in next cycle
+        self.procs_cpu_time_t = procs_cpu_times
+        self.total_cpu_time_t = total_cpu_time
+
         # Memory share if sum of all process's memory / total memory consumption
         # We choose RSS here to estimate the share. Sum of all RSS will be more than
         # the physical memory as we will add shared memory of all processes thus
         # deuplicating memory. But we are interested only in the fraction and it
         # seems to be a reasonable estimate
         mem_share = sum([psutil.Process(pid=p).memory_info().rss for p in pids]) / sum(
             [p.memory_info().rss for p in psutil.process_iter(['memory_info'])]
@@ -156,14 +197,15 @@
         cpu_power_usage, dram_power_usage = self.get_total_power_usage(
             current_time - self.time_t, (rapl_readings_dt, self.rapl_readings_t)
         )
         # # For local testing
         # import random
         # cpu_power_usage = random.uniform(20, 30)
         # dram_power_usage = random.uniform(5, 10)
+
         cpu_share, mem_share = self.get_cpu_share(pids)
 
         # Set current measurements as previous measurements for next reading
         self.rapl_readings_t = rapl_readings_dt
         self.time_t = current_time
 
         return cpu_power_usage * cpu_share + dram_power_usage * mem_share
```

### Comparing `jupyter_power_usage-1.0.0/jupyter_power_usage/utils.py` & `jupyter_power_usage-1.1.0/jupyter_power_usage/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,7 @@
-# Copyright 2023 IDRIS / jupyter
-#
-# Licensed under the Apache License, Version 2.0 (the "License");
-# you may not use this file except in compliance with the License.
-# You may obtain a copy of the License at
-#
-#     http://www.apache.org/licenses/LICENSE-2.0
-#
-# Unless required by applicable law or agreed to in writing, software
-# distributed under the License is distributed on an "AS IS" BASIS,
-# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-# See the License for the specific language governing permissions and
-# limitations under the License.
 import os
 import re
 import subprocess
 
 # RAPL powercap API directory
 RAPL_API_DIR = '/sys/class/powercap/intel-rapl'
 
@@ -175,17 +162,17 @@
                 continue
 
             unq_dom_name = f'{dom_name}-{pkg_name}'
             filtered_domains[unq_dom_name] = dom_dict['energy_uj']
             filtered_domains_power_limits[unq_dom_name] = read_power_limit_uw_counter(
                 dom_dict['energy_uj']
             )
-            filtered_domains_overflow_counters[
-                unq_dom_name
-            ] = read_max_energy_uj_counter(dom_dict['energy_uj'])
+            filtered_domains_overflow_counters[unq_dom_name] = (
+                read_max_energy_uj_counter(dom_dict['energy_uj'])
+            )
     return (
         filtered_domains,
         filtered_domains_power_limits,
         filtered_domains_overflow_counters,
     )
```

### Comparing `jupyter_power_usage-1.0.0/jupyter_power_usage/labextension/package.json` & `jupyter_power_usage-1.1.0/jupyter_power_usage/labextension/package.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9778079710144927%*

 * *Differences: {"'jupyterlab'": "{'_build': {'load': 'static/remoteEntry.20fe913e7d7c5e7492d8.js'}}",*

 * * "'version'": "'1.1.0'"}*

```diff
@@ -110,15 +110,15 @@
         "style/**/*.{css,eot,gif,html,jpg,json,png,svg,woff2,ttf}",
         "style/index.js"
     ],
     "homepage": "https://github.com/mahendrapaipuri/jupyter-power-usage",
     "jupyterlab": {
         "_build": {
             "extension": "./extension",
-            "load": "static/remoteEntry.8012d710f1db7c034cba.js",
+            "load": "static/remoteEntry.20fe913e7d7c5e7492d8.js",
             "style": "./style"
         },
         "extension": true,
         "outputDir": "jupyter_power_usage/labextension",
         "schemaDir": "schema"
     },
     "keywords": [
@@ -175,9 +175,9 @@
             "property-no-vendor-prefix": null,
             "selector-class-pattern": null,
             "selector-no-vendor-prefix": null,
             "value-no-vendor-prefix": null
         }
     },
     "types": "lib/index.d.ts",
-    "version": "1.0.0"
+    "version": "1.1.0"
 }
```

### Comparing `jupyter_power_usage-1.0.0/jupyter_power_usage/labextension/schemas/@mahendrapaipuri/jupyter-power-usage/package.json.orig` & `jupyter_power_usage-1.1.0/jupyter_power_usage/labextension/schemas/@mahendrapaipuri/jupyter-power-usage/package.json.orig`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9782608695652174%*

 * *Differences: {"'version'": "'1.1.0'"}*

```diff
@@ -170,9 +170,9 @@
             "property-no-vendor-prefix": null,
             "selector-class-pattern": null,
             "selector-no-vendor-prefix": null,
             "value-no-vendor-prefix": null
         }
     },
     "types": "lib/index.d.ts",
-    "version": "1.0.0"
+    "version": "1.1.0"
 }
```

### Comparing `jupyter_power_usage-1.0.0/jupyter_power_usage/labextension/schemas/@mahendrapaipuri/jupyter-power-usage/plugin.json` & `jupyter_power_usage-1.1.0/jupyter_power_usage/labextension/schemas/@mahendrapaipuri/jupyter-power-usage/plugin.json`

 * *Files 6% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9985942322530863%*

 * *Differences: {"'definitions'": "{'emissions': {'properties': {'countryCode': {'description': 'ISO code of the "*

 * *                  "country of which emission factor will be used.', delete: ['enum', 'default']}, "*

 * *                  "'refreshRate': {'description': 'eCO2 emission factor will be updated at this "*

 * *                  "interval. Do not use too small intervals as these APIs are rate limited.'}, "*

 * *                  "'source': OrderedDict([('title', 'Source of emission factor'), ('description', "*

 * *                   […]*

```diff
@@ -9,32 +9,48 @@
                 }
             },
             "type": "object"
         },
         "emissions": {
             "properties": {
                 "countryCode": {
-                    "default": "",
-                    "description": "ISO code of the country of which emission factor will be used",
-                    "enum": [
-                        "",
-                        "fr"
-                    ],
+                    "description": "ISO code of the country of which emission factor will be used.",
                     "title": "Country code",
                     "type": "string"
                 },
+                "emapsAccessToken": {
+                    "description": "API Access token for Electricity Maps.",
+                    "title": "Electricity Maps Access token",
+                    "type": "string"
+                },
                 "factor": {
                     "description": "eCO2 emission factor will be used if Emission data for the selected country is not available.",
                     "title": "Emission factor (g/kWh)",
                     "type": "number"
                 },
                 "refreshRate": {
-                    "description": "eCO2 emission factor will be updated at this interval. Do not use too small intervals as these sort of APIs are rate limited.",
+                    "description": "eCO2 emission factor will be updated at this interval. Do not use too small intervals as these APIs are rate limited.",
                     "title": "Refresh rate (ms)",
                     "type": "number"
+                },
+                "source": {
+                    "default": "rte",
+                    "description": "Emission factor fetched from this source will be used. RTE eCO2 mix source is only available for France.",
+                    "oneOf": [
+                        {
+                            "const": "emaps",
+                            "title": "Electricity Maps"
+                        },
+                        {
+                            "const": "rte",
+                            "title": "RTE eCO2 mix"
+                        }
+                    ],
+                    "title": "Source of emission factor",
+                    "type": "string"
                 }
             },
             "type": "object"
         },
         "gpu": {
             "properties": {
                 "label": {
@@ -72,15 +88,16 @@
             },
             "description": "Settings for the CPU Power indicator",
             "title": "CPU Power Settings"
         },
         "emissions": {
             "$ref": "#/definitions/emissions",
             "default": {
-                "countryCode": "",
+                "countryCode": "FR",
+                "emapsAccessToken": "",
                 "factor": 475,
                 "refreshRate": 1800000
             },
             "description": "Settings for the estimating eCO2 emissions",
             "title": "Emissions Estimation Settings"
         },
         "gpu": {
```

### Comparing `jupyter_power_usage-1.0.0/jupyter_power_usage/labextension/static/32.df2f2b30253633c749ea.js` & `jupyter_power_usage-1.1.0/jupyter_power_usage/labextension/static/32.d626a962b7bd9192a1da.js`

 * *Files 12% similar despite different names*

#### js-beautify {}

```diff
@@ -1,132 +1,132 @@
 "use strict";
 (self.webpackChunk_mahendrapaipuri_jupyter_power_usage = self.webpackChunk_mahendrapaipuri_jupyter_power_usage || []).push([
     [32], {
         32: (e, t, n) => {
             n.r(t), n.d(t, {
-                default: () => B
+                default: () => z
             });
-            var r = n(861),
-                i = n(684),
-                s = n(29),
-                a = n.n(s),
+            var s = n(510),
+                r = n(8),
+                i = n(29),
+                a = n.n(i),
                 o = n(496);
-            const l = ({
+            const c = ({
                     percentage: e,
                     color: t
                 }) => a().createElement("div", {
                     className: "jp-IndicatorFiller",
                     style: {
                         width: 100 * e + "%",
                         background: `${t}`
                     }
                 }),
-                c = ({
+                l = ({
                     values: e,
                     percentage: t,
                     baseColor: n
                 }) => {
-                    const [r, i] = (0, s.useState)(!1), c = t > .5 ? t > .8 ? "red" : "orange" : n;
+                    const [s, r] = (0, i.useState)(!1), l = t > .5 ? t > .8 ? "red" : "orange" : n;
                     return a().createElement("div", {
                         className: "jp-IndicatorBar",
                         onClick: () => {
-                            i(!r)
+                            r(!s)
                         }
-                    }, r && a().createElement(o.Sparklines, {
+                    }, s && a().createElement(o.Sparklines, {
                         data: e,
                         min: 0,
                         max: 1,
                         limit: e.length,
                         margin: 0
                     }, a().createElement(o.SparklinesLine, {
                         style: {
-                            stroke: c,
+                            stroke: l,
                             strokeWidth: 4,
-                            fill: c,
+                            fill: l,
                             fillOpacity: 1
                         }
-                    }), a().createElement(o.SparklinesSpots, null)), !r && a().createElement(l, {
+                    }), a().createElement(o.SparklinesSpots, null)), !s && a().createElement(c, {
                         percentage: t,
-                        color: c
+                        color: l
                     }))
                 },
                 u = ({
                     enabled: e,
                     values: t,
                     label: n,
-                    color: r,
-                    text: i
+                    color: s,
+                    text: r
                 }) => {
-                    const s = t[t.length - 1];
+                    const i = t[t.length - 1];
                     return e && a().createElement("div", {
                         className: "jp-IndicatorContainer"
                     }, a().createElement("div", {
                         className: "jp-IndicatorText"
-                    }, n), null !== s && a().createElement("div", {
+                    }, n), null !== i && a().createElement("div", {
                         className: "jp-IndicatorWrapper"
-                    }, a().createElement(c, {
+                    }, a().createElement(l, {
                         values: t,
-                        percentage: s,
-                        baseColor: r
+                        percentage: i,
+                        baseColor: s
                     })), a().createElement("div", {
                         className: "jp-IndicatorText"
-                    }, i))
+                    }, r))
                 },
                 p = ({
                     model: e,
                     label: t
                 }) => {
-                    const [n, r] = (0, s.useState)(""), [i, o] = (0, s.useState)([]), l = () => {
+                    const [n, s] = (0, i.useState)(""), [r, o] = (0, i.useState)([]), c = () => {
                         const {
                             currentCpuPower: t,
                             currentCpuPowerLimit: n
-                        } = e, i = `${t.toFixed(2)} ${n?"/ "+n.toFixed(0):""} W`, s = e.values.map((e => e.cpuPowerShare));
-                        r(i), o(s)
+                        } = e, r = `${t.toFixed(2)} ${n?"/ "+n.toFixed(0):""} W`, i = e.values.map((e => e.cpuPowerShare));
+                        s(r), o(i)
                     };
-                    return (0, s.useEffect)((() => (e.changed.connect(l), () => {
-                        e.changed.disconnect(l)
+                    return (0, i.useEffect)((() => (e.changed.connect(c), () => {
+                        e.changed.disconnect(c)
                     })), [e]), a().createElement(u, {
                         enabled: e.cpuPowerAvailable,
-                        values: i,
+                        values: r,
                         label: t,
                         color: "#1AB7AE",
                         text: n
                     })
                 };
             var d;
             ! function(e) {
-                e.createPowerView = (e, t) => r.ReactWidget.create(a().createElement(p, {
+                e.createPowerView = (e, t) => s.ReactWidget.create(a().createElement(p, {
                     model: e,
                     label: t
                 }))
             }(d || (d = {}));
             const h = ({
                 model: e,
                 label: t
             }) => {
-                const [n, r] = (0, s.useState)(""), [i, o] = (0, s.useState)([]), l = () => {
+                const [n, s] = (0, i.useState)(""), [r, o] = (0, i.useState)([]), c = () => {
                     const {
                         currentGpuPower: t,
                         currentGpuLimit: n
-                    } = e, i = `${t.toFixed(2)} ${n?"/ "+n.toFixed(0):""} W`, s = e.values.map((e => e.gpuPowerShare));
-                    r(i), o(s)
+                    } = e, r = `${t.toFixed(2)} ${n?"/ "+n.toFixed(0):""} W`, i = e.values.map((e => e.gpuPowerShare));
+                    s(r), o(i)
                 };
-                return (0, s.useEffect)((() => (e.changed.connect(l), () => {
-                    e.changed.disconnect(l)
+                return (0, i.useEffect)((() => (e.changed.connect(c), () => {
+                    e.changed.disconnect(c)
                 })), [e]), a().createElement(u, {
                     enabled: e.gpuPowerAvailable,
-                    values: i,
+                    values: r,
                     label: t,
                     color: "#76B900",
                     text: n
                 })
             };
             var m;
             ! function(e) {
-                e.createPowerView = (e, t) => r.ReactWidget.create(a().createElement(h, {
+                e.createPowerView = (e, t) => s.ReactWidget.create(a().createElement(h, {
                     model: e,
                     label: t
                 }))
             }(m || (m = {}));
             const g = ({
                     enabled: e,
                     text: t
@@ -136,79 +136,107 @@
                     className: "jp-IndicatorText"
                 }, a().createElement("span", null, "eCO", a().createElement("sub", null, "2"), ":")), a().createElement("div", {
                     className: "jp-IndicatorText"
                 }, t)),
                 f = ({
                     model: e
                 }) => {
-                    const [t, n] = (0, s.useState)(""), r = () => {
+                    const [t, n] = (0, i.useState)(""), s = () => {
                         const {
                             currentEmissions: t,
-                            emissionsUnits: r
-                        } = e, i = ["mg", "g", "kg"].indexOf(r) > 0 ? 0 : 2, s = `${t.toFixed(i)} ${e.emissionsUnits}`;
-                        n(s)
+                            emissionsUnits: s
+                        } = e, r = ["mg", "g", "kg"].indexOf(s) > 0 ? 0 : 2, i = `${t.toFixed(r)} ${e.emissionsUnits}`;
+                        n(i)
                     };
-                    return (0, s.useEffect)((() => (e.changed.connect(r), () => {
-                        e.changed.disconnect(r)
+                    return (0, i.useEffect)((() => (e.changed.connect(s), () => {
+                        e.changed.disconnect(s)
                     })), [e]), a().createElement(g, {
                         enabled: e.emissionsAvailable,
                         text: t
                     })
                 };
             var v;
             ! function(e) {
-                e.createEmissionsView = e => r.ReactWidget.create(a().createElement(f, {
+                e.createEmissionsView = e => s.ReactWidget.create(a().createElement(f, {
                     model: e
                 }))
             }(v || (v = {}));
-            var w = n(614),
-                _ = n(788),
+            var w = n(311),
+                _ = n(217),
                 b = n(797),
-                P = n(901);
-            const E = 1e3,
-                y = 1e6;
-            var x;
+                y = n(901);
+            const P = 1e3,
+                E = 1e6;
+            var x, A;
             ! function(e) {
-                e.getOpenDataSoftEmissions = async () => {
+                e.getOpenDataSoftEmissionFactor = async () => {
                     var e, t;
                     const n = {
                             dataset: "eco2mix-national-tr",
                             facet: "date_heure",
                             start: "0",
                             rows: "1",
                             sort: "date_heure",
                             timezone: "Europe/Paris",
                             q: `date_heure:[${(new Date).toISOString().split("T")[0]} TO #now()] AND NOT #null(taux_co2)`
                         },
-                        r = w.URLExt.objectToQueryString(n),
-                        i = w.URLExt.join("https://odre.opendatasoft.com", "/api/records/1.0/search/", r);
+                        s = w.URLExt.objectToQueryString(n),
+                        r = w.URLExt.join("https://odre.opendatasoft.com", "/api/records/1.0/search/", s);
                     try {
-                        const n = await fetch(i, {
+                        const n = await fetch(r, {
                             method: "GET"
                         });
                         if (!n.ok) return console.debug("Request to Opendatasoft API failed"), null;
-                        const r = await n.json();
-                        if (r && r.records && r.records.length > 0) return (null === (t = null === (e = r.records[0]) || void 0 === e ? void 0 : e.fields) || void 0 === t ? void 0 : t.taux_co2) || 0
+                        const s = await n.json();
+                        if (s && s.records && s.records.length > 0) return (null === (t = null === (e = s.records[0]) || void 0 === e ? void 0 : e.fields) || void 0 === t ? void 0 : t.taux_co2) || 0
                     } catch (e) {
                         return console.info(`Request to Opendatasoft API failed due to ${e}`), null
                     }
                     return null
                 }
-            }(x || (x = {}));
-            var A, C, U;
+            }(x || (x = {})),
+            function(e) {
+                const t = "/v3/carbon-intensity/latest",
+                    n = _.ServerConnection.makeSettings();
+                e.getElectricityMapsEmissionFactor = async (e, s, r) => {
+                    const i = {
+                            zone: r.toUpperCase()
+                        },
+                        a = w.URLExt.objectToQueryString(i);
+                    try {
+                        let r;
+                        const i = new Headers;
+                        s.length > 0 && i.set("auth-token", s), r = e ? w.URLExt.join(n.baseUrl, "api/metrics/v1/emission_factor/emaps", t, a) : w.URLExt.join("https://api.electricitymap.org", t, a);
+                        const o = await fetch(r, {
+                            method: "GET",
+                            headers: i
+                        });
+                        if (!o.ok) return console.debug("Request to Electricity Maps API failed"), null;
+                        const c = await o.json();
+                        if (c && c.carbonIntensity) return c.carbonIntensity || 0
+                    } catch (e) {
+                        return console.info(`Request to Electricity Maps failed due to ${e}`), null
+                    }
+                    return null
+                }
+            }(A || (A = {}));
+            const F = async function(e, t, n, s) {
+                return "rte" === e ? await x.getOpenDataSoftEmissionFactor() : "emaps" === e ? await A.getElectricityMapsEmissionFactor(t, n.emaps, s) : null
+            };
+            var U, C, S;
             ! function(e) {
-                class t extends r.VDomModel {
+                class t extends s.VDomModel {
                     constructor(e, t) {
                         super(), this._cpuPowerUsageAvailable = !1, this._gpuPowerUsageAvailable = !1, this._emissionsAvailable = !1, this._currentCpuPowerLimit = null, this._currentCpuPowerUsage = null, this._currentGpuPowerUsage = null, this._currentGpuPowerLimit = null, this._currentEmissions = null, this._lastEmissionReading = Date.now(), this._lastEmissionFactor = null, this._totalEmissions = 0, this._values = [], this._emissionModel = e;
                         for (let e = 0; e < 20; e++) this._values.push({
                             cpuPowerShare: 0,
                             gpuPowerShare: 0
                         });
                         this._poll = new b.Poll({
-                            factory: () => U.powerUsageFactory(),
+                            factory: () => S.powerUsageFactory(),
                             frequency: {
                                 interval: t.refreshRate,
                                 backoff: !0
                             },
                             name: "jupyter-power-usage:PowerUsage#metrics"
                         }), this._poll.ticked.connect((e => {
                             const {
@@ -266,46 +294,52 @@
                         this._poll.dispose()
                     }
                     _updateMetricsValues(e) {
                         if (null === e) return this._cpuPowerUsageAvailable = !1, this._gpuPowerUsageAvailable = !1, this._emissionsAvailable = !1, this._currentCpuPowerLimit = null, this._currentCpuPowerUsage = null, this._currentGpuPowerUsage = null, this._currentGpuPowerLimit = null, void(this._currentEmissions = null);
                         const t = e.cpu ? e.cpu.usage : null,
                             n = e.cpu ? e.cpu.limit : null;
                         this._cpuPowerUsageAvailable = !!t, this._currentCpuPowerUsage = t, this._currentCpuPowerLimit = n;
-                        const r = e.gpu ? e.gpu.usage : null,
-                            i = e.gpu ? e.gpu.limit : null;
-                        this._gpuPowerUsageAvailable = !!r, this._currentGpuPowerUsage = r, this._currentGpuPowerLimit = i;
+                        const s = e.gpu ? e.gpu.usage : null,
+                            r = e.gpu ? e.gpu.limit : null;
+                        this._gpuPowerUsageAvailable = !!s, this._currentGpuPowerUsage = s, this._currentGpuPowerLimit = r;
                         const {
-                            emissionFactorAvailable: s,
+                            emissionFactorAvailable: i,
                             currentEmissionFactor: a
                         } = this._emissionModel;
-                        if (this._lastEmissionFactor = s ? a : this._lastEmissionFactor, this._emissionsAvailable = null !== this._lastEmissionFactor, this._emissionsAvailable) {
+                        if (this._lastEmissionFactor = i ? a : this._lastEmissionFactor, this._emissionsAvailable = null !== this._lastEmissionFactor, this._emissionsAvailable) {
                             const e = Date.now() - this._lastEmissionReading,
-                                n = (t || 0) + (r || 0),
-                                i = this._lastEmissionFactor * n * e / 1e3;
+                                n = (t || 0) + (s || 0),
+                                r = this._lastEmissionFactor * n * e / 1e3;
                             this._lastEmissionReading = Date.now();
-                            const s = this._totalEmissions + i,
-                                [a, l] = (o = s) ? o < E ? [o, "mg"] : E === o || o < y ? [o / E, "g"] : [o / y, "kg"] : [0, "mg"];
-                            this._currentEmissions = a, this._emissionsUnits = l, this._totalEmissions = s
+                            const i = this._totalEmissions + r,
+                                [a, c] = (o = i) ? o < P ? [o, "mg"] : P === o || o < E ? [o / P, "g"] : [o / E, "kg"] : [0, "mg"];
+                            this._currentEmissions = a, this._emissionsUnits = c, this._totalEmissions = i
                         }
                         var o;
-                        const l = this._currentCpuPowerLimit ? Math.min(this._currentCpuPowerUsage / this._currentCpuPowerLimit, 1) : null,
-                            c = this._currentGpuPowerUsage && this._currentGpuPowerLimit ? Math.min(this._currentGpuPowerUsage / this._currentGpuPowerLimit, 1) : null;
+                        const c = this._currentCpuPowerLimit ? Math.min(this._currentCpuPowerUsage / this._currentCpuPowerLimit, 1) : null,
+                            l = this._currentGpuPowerUsage && this._currentGpuPowerLimit ? Math.min(this._currentGpuPowerUsage / this._currentGpuPowerLimit, 1) : null;
                         this._values.push({
-                            cpuPowerShare: l,
-                            gpuPowerShare: c
+                            cpuPowerShare: c,
+                            gpuPowerShare: l
                         }), this._values.shift(), this.stateChanged.emit(void 0)
                     }
                 }
                 e.Model = t
-            }(A || (A = {})),
+            }(U || (U = {})),
             function(e) {
                 e.Model = class {
                     constructor(e) {
-                        this._emissionFactorAvailable = !1, this._currentEmissionFactor = null, this._changed = new P.Signal(this), this._poll = new b.Poll({
-                            factory: () => U.emissionsFactory(e.countryCode, e.defaultEmissionFactor),
+                        this._emissionFactorAvailable = !1, this._useProxy = !1, this._currentEmissionFactor = null, this._changed = new y.Signal(this), "emaps" === e.emissionFactorSource && new Promise((() => {
+                            F(e.emissionFactorSource, !0, e.accessTokens, e.countryCode).then((e => {
+                                this._useProxy = !!e
+                            })).catch((() => {
+                                console.warn("Emission factor from Electricity maps will be fetched by making API requests directly from the browser. If a access token has been set, this can pose security risks. Please configure the access token on Jupyter server extension."), this._useProxy = !1
+                            }))
+                        })), this._poll = new b.Poll({
+                            factory: () => S.emissionsFactory(e.emissionFactorSource, this._useProxy, e.accessTokens, e.countryCode, e.defaultEmissionFactor),
                             frequency: {
                                 interval: e.refreshRate,
                                 backoff: !0
                             },
                             name: "jupyter-power-usage:EmissionFactor#metrics"
                         }), this._poll.ticked.connect((e => {
                             const {
@@ -340,215 +374,219 @@
                 }
             }(C || (C = {})),
             function(e) {
                 const t = _.ServerConnection.makeSettings(),
                     n = w.URLExt.join(t.baseUrl, "api/metrics/v1/power_usage");
                 e.powerUsageFactory = async () => {
                     const e = _.ServerConnection.makeRequest(n, {}, t),
-                        r = await e;
-                    return r.ok ? await r.json() : null
-                }, e.emissionsFactory = async (e, t) => {
-                    const n = await async function(e) {
-                        return "fr" === e ? await x.getOpenDataSoftEmissions() : null
-                    }(e);
-                    return n ? n / 3600 : t / 3600
+                        s = await e;
+                    return s.ok ? await s.json() : null
+                }, e.emissionsFactory = async (e, t, n, s, r) => {
+                    const i = await F(e, t, n, s);
+                    return i ? i / 3600 : r / 3600
                 }
-            }(U || (U = {}));
-            var F = n(379),
-                S = n.n(F),
-                j = n(795),
-                I = n.n(j),
-                k = n(569),
-                L = n.n(k),
-                T = n(565),
-                R = n.n(T),
-                G = n(216),
-                M = n.n(G),
-                N = n(589),
-                O = n.n(N),
-                V = n(760),
+            }(S || (S = {}));
+            var j = n(379),
+                k = n.n(j),
+                I = n(795),
+                T = n.n(I),
+                L = n(569),
+                R = n.n(L),
+                M = n(565),
+                G = n.n(M),
+                N = n(216),
+                q = n.n(N),
+                O = n(589),
+                V = n.n(O),
+                $ = n(760),
                 D = {};
-            D.styleTagTransform = O(), D.setAttributes = R(), D.insert = L().bind(null, "head"), D.domAPI = I(), D.insertStyleElement = M(), S()(V.Z, D), V.Z && V.Z.locals && V.Z.locals;
+            D.styleTagTransform = V(), D.setAttributes = G(), D.insert = R().bind(null, "head"), D.domAPI = T(), D.insertStyleElement = q(), k()($.Z, D), $.Z && $.Z.locals && $.Z.locals;
             const W = 5e3,
-                $ = 18e5,
-                q = {
+                B = 18e5,
+                Z = {
                     id: "@mahendrapaipuri/jupyter-power-usage:plugin",
                     autoStart: !0,
-                    requires: [r.IToolbarWidgetRegistry],
-                    optional: [i.ISettingRegistry],
+                    requires: [s.IToolbarWidgetRegistry],
+                    optional: [r.ISettingRegistry],
                     activate: async (e, t, n) => {
                         console.log("@mahendrapaipuri/jupyter-power-usage extension is activated");
-                        let r = W,
-                            i = "CPU Power: ",
-                            s = "GPU Power: ",
-                            a = $,
-                            o = "fr",
-                            l = 475;
+                        let s = W,
+                            r = "CPU Power: ",
+                            i = "GPU Power: ",
+                            a = B,
+                            o = "rte",
+                            c = "",
+                            l = "fr",
+                            u = 475;
                         if (n) {
-                            const e = await n.load(q.id);
-                            r = e.get("refreshRate").composite, r < W && (console.log("Refresh rate is floored at 5000 ms"), r = W);
+                            const e = await n.load(Z.id);
+                            s = e.get("refreshRate").composite, s < W && (console.log("Refresh rate is floored at 5000 ms"), s = W);
                             const t = e.get("emissions").composite;
-                            o = t.countryCode, a = t.refreshRate, l = t.factor, a < $ && (console.log("Emissions update interval is floored at 1800000 ms"), a = $);
-                            const c = e.get("cpu").composite;
-                            i = c.label;
-                            const u = e.get("gpu").composite;
-                            s = u.label
+                            o = t.source, c = t.emapsAccessToken, l = t.countryCode, a = t.refreshRate, u = t.factor, a < B && (console.log("Emissions update interval is floored at 1800000 ms"), a = B);
+                            const p = e.get("cpu").composite;
+                            r = p.label;
+                            const d = e.get("gpu").composite;
+                            i = d.label
                         }
-                        const c = new C.Model({
+                        const p = new C.Model({
                             refreshRate: a,
-                            countryCode: o,
-                            defaultEmissionFactor: l
+                            emissionFactorSource: o,
+                            accessTokens: {
+                                emaps: c
+                            },
+                            countryCode: l,
+                            defaultEmissionFactor: u
                         });
-                        await c.refresh();
-                        const u = new A.Model(c, {
-                            refreshRate: r
+                        await p.refresh();
+                        const h = new U.Model(p, {
+                            refreshRate: s
                         });
-                        await u.refresh(), u.cpuPowerAvailable || u.gpuPowerAvailable || (console.log("Power metrics are not available..."), u.dispose(), c.dispose()), u.cpuPowerAvailable && t.addFactory("TopBar", "cpu_power", (() => d.createPowerView(u, i))), u.gpuPowerAvailable && t.addFactory("TopBar", "gpu_power", (() => m.createPowerView(u, s))), u.emissionsAvailable && t.addFactory("TopBar", "emissions", (() => v.createEmissionsView(u)))
+                        await h.refresh(), h.cpuPowerAvailable || h.gpuPowerAvailable || (console.log("Power metrics are not available..."), h.dispose(), p.dispose()), h.cpuPowerAvailable && t.addFactory("TopBar", "cpu_power", (() => d.createPowerView(h, r))), h.gpuPowerAvailable && t.addFactory("TopBar", "gpu_power", (() => m.createPowerView(h, i))), h.emissionsAvailable && t.addFactory("TopBar", "emissions", (() => v.createEmissionsView(h)))
                     }
                 },
-                B = q
+                z = Z
         },
         150: (e, t, n) => {
             n.d(t, {
                 Z: () => o
             });
-            var r = n(81),
-                i = n.n(r),
-                s = n(645),
-                a = n.n(s)()(i());
+            var s = n(81),
+                r = n.n(s),
+                i = n(645),
+                a = n.n(i)()(r());
             a.push([e.id, ".jp-IndicatorContainer {\n  display: flex;\n  flex-direction: row;\n}\n\n.jp-IndicatorFiller {\n  height: 100%;\n}\n\n.jp-IndicatorText {\n  display: flex;\n  min-width: 35px;\n  flex-direction: column;\n  justify-content: center;\n  text-align: right;\n  white-space: nowrap;\n  overflow: hidden;\n}\n\n.jp-IndicatorWrapper {\n  display: flex;\n  flex-direction: column;\n  justify-content: center;\n  margin-left: 5px;\n  margin-right: 5px;\n  width: 75px;\n}\n\n.jp-IndicatorBar {\n  height: 75%;\n  outline: 1px solid black;\n}\n\n.jp-IndicatorBar svg {\n  max-width: 100%;\n  height: 100%;\n}\n\n/* To center the subscript in the text */\nsub {\n  top: 0;\n  bottom: 0;\n  line-height: 1;\n  font-size: 0.5em;\n}\n", ""]);
             const o = a
         },
         760: (e, t, n) => {
             n.d(t, {
-                Z: () => c
+                Z: () => l
             });
-            var r = n(81),
-                i = n.n(r),
-                s = n(645),
-                a = n.n(s),
+            var s = n(81),
+                r = n.n(s),
+                i = n(645),
+                a = n.n(i),
                 o = n(150),
-                l = a()(i());
-            l.i(o.Z), l.push([e.id, "\n", ""]);
-            const c = l
+                c = a()(r());
+            c.i(o.Z), c.push([e.id, "\n", ""]);
+            const l = c
         },
         645: e => {
             e.exports = function(e) {
                 var t = [];
                 return t.toString = function() {
                     return this.map((function(t) {
                         var n = "",
-                            r = void 0 !== t[5];
-                        return t[4] && (n += "@supports (".concat(t[4], ") {")), t[2] && (n += "@media ".concat(t[2], " {")), r && (n += "@layer".concat(t[5].length > 0 ? " ".concat(t[5]) : "", " {")), n += e(t), r && (n += "}"), t[2] && (n += "}"), t[4] && (n += "}"), n
+                            s = void 0 !== t[5];
+                        return t[4] && (n += "@supports (".concat(t[4], ") {")), t[2] && (n += "@media ".concat(t[2], " {")), s && (n += "@layer".concat(t[5].length > 0 ? " ".concat(t[5]) : "", " {")), n += e(t), s && (n += "}"), t[2] && (n += "}"), t[4] && (n += "}"), n
                     })).join("")
-                }, t.i = function(e, n, r, i, s) {
+                }, t.i = function(e, n, s, r, i) {
                     "string" == typeof e && (e = [
                         [null, e, void 0]
                     ]);
                     var a = {};
-                    if (r)
+                    if (s)
                         for (var o = 0; o < this.length; o++) {
-                            var l = this[o][0];
-                            null != l && (a[l] = !0)
+                            var c = this[o][0];
+                            null != c && (a[c] = !0)
                         }
-                    for (var c = 0; c < e.length; c++) {
-                        var u = [].concat(e[c]);
-                        r && a[u[0]] || (void 0 !== s && (void 0 === u[5] || (u[1] = "@layer".concat(u[5].length > 0 ? " ".concat(u[5]) : "", " {").concat(u[1], "}")), u[5] = s), n && (u[2] ? (u[1] = "@media ".concat(u[2], " {").concat(u[1], "}"), u[2] = n) : u[2] = n), i && (u[4] ? (u[1] = "@supports (".concat(u[4], ") {").concat(u[1], "}"), u[4] = i) : u[4] = "".concat(i)), t.push(u))
+                    for (var l = 0; l < e.length; l++) {
+                        var u = [].concat(e[l]);
+                        s && a[u[0]] || (void 0 !== i && (void 0 === u[5] || (u[1] = "@layer".concat(u[5].length > 0 ? " ".concat(u[5]) : "", " {").concat(u[1], "}")), u[5] = i), n && (u[2] ? (u[1] = "@media ".concat(u[2], " {").concat(u[1], "}"), u[2] = n) : u[2] = n), r && (u[4] ? (u[1] = "@supports (".concat(u[4], ") {").concat(u[1], "}"), u[4] = r) : u[4] = "".concat(r)), t.push(u))
                     }
                 }, t
             }
         },
         81: e => {
             e.exports = function(e) {
                 return e[1]
             }
         },
         379: e => {
             var t = [];
 
             function n(e) {
-                for (var n = -1, r = 0; r < t.length; r++)
-                    if (t[r].identifier === e) {
-                        n = r;
+                for (var n = -1, s = 0; s < t.length; s++)
+                    if (t[s].identifier === e) {
+                        n = s;
                         break
                     } return n
             }
 
-            function r(e, r) {
-                for (var s = {}, a = [], o = 0; o < e.length; o++) {
-                    var l = e[o],
-                        c = r.base ? l[0] + r.base : l[0],
-                        u = s[c] || 0,
-                        p = "".concat(c, " ").concat(u);
-                    s[c] = u + 1;
+            function s(e, s) {
+                for (var i = {}, a = [], o = 0; o < e.length; o++) {
+                    var c = e[o],
+                        l = s.base ? c[0] + s.base : c[0],
+                        u = i[l] || 0,
+                        p = "".concat(l, " ").concat(u);
+                    i[l] = u + 1;
                     var d = n(p),
                         h = {
-                            css: l[1],
-                            media: l[2],
-                            sourceMap: l[3],
-                            supports: l[4],
-                            layer: l[5]
+                            css: c[1],
+                            media: c[2],
+                            sourceMap: c[3],
+                            supports: c[4],
+                            layer: c[5]
                         };
                     if (-1 !== d) t[d].references++, t[d].updater(h);
                     else {
-                        var m = i(h, r);
-                        r.byIndex = o, t.splice(o, 0, {
+                        var m = r(h, s);
+                        s.byIndex = o, t.splice(o, 0, {
                             identifier: p,
                             updater: m,
                             references: 1
                         })
                     }
                     a.push(p)
                 }
                 return a
             }
 
-            function i(e, t) {
+            function r(e, t) {
                 var n = t.domAPI(t);
                 return n.update(e),
                     function(t) {
                         if (t) {
                             if (t.css === e.css && t.media === e.media && t.sourceMap === e.sourceMap && t.supports === e.supports && t.layer === e.layer) return;
                             n.update(e = t)
                         } else n.remove()
                     }
             }
-            e.exports = function(e, i) {
-                var s = r(e = e || [], i = i || {});
+            e.exports = function(e, r) {
+                var i = s(e = e || [], r = r || {});
                 return function(e) {
                     e = e || [];
-                    for (var a = 0; a < s.length; a++) {
-                        var o = n(s[a]);
+                    for (var a = 0; a < i.length; a++) {
+                        var o = n(i[a]);
                         t[o].references--
                     }
-                    for (var l = r(e, i), c = 0; c < s.length; c++) {
-                        var u = n(s[c]);
+                    for (var c = s(e, r), l = 0; l < i.length; l++) {
+                        var u = n(i[l]);
                         0 === t[u].references && (t[u].updater(), t.splice(u, 1))
                     }
-                    s = l
+                    i = c
                 }
             }
         },
         569: e => {
             var t = {};
             e.exports = function(e, n) {
-                var r = function(e) {
+                var s = function(e) {
                     if (void 0 === t[e]) {
                         var n = document.querySelector(e);
                         if (window.HTMLIFrameElement && n instanceof window.HTMLIFrameElement) try {
                             n = n.contentDocument.head
                         } catch (e) {
                             n = null
                         }
                         t[e] = n
                     }
                     return t[e]
                 }(e);
-                if (!r) throw new Error("Couldn't find a style target. This probably means that the value for the 'insert' parameter is invalid.");
-                r.appendChild(n)
+                if (!s) throw new Error("Couldn't find a style target. This probably means that the value for the 'insert' parameter is invalid.");
+                s.appendChild(n)
             }
         },
         216: e => {
             e.exports = function(e) {
                 var t = document.createElement("style");
                 return e.setAttributes(t, e.attributes), e.insert(t, e.options), t
             }
@@ -565,20 +603,20 @@
                     update: function() {},
                     remove: function() {}
                 };
                 var t = e.insertStyleElement(e);
                 return {
                     update: function(n) {
                         ! function(e, t, n) {
-                            var r = "";
-                            n.supports && (r += "@supports (".concat(n.supports, ") {")), n.media && (r += "@media ".concat(n.media, " {"));
-                            var i = void 0 !== n.layer;
-                            i && (r += "@layer".concat(n.layer.length > 0 ? " ".concat(n.layer) : "", " {")), r += n.css, i && (r += "}"), n.media && (r += "}"), n.supports && (r += "}");
-                            var s = n.sourceMap;
-                            s && "undefined" != typeof btoa && (r += "\n/*# sourceMappingURL=data:application/json;base64,".concat(btoa(unescape(encodeURIComponent(JSON.stringify(s)))), " */")), t.styleTagTransform(r, e, t.options)
+                            var s = "";
+                            n.supports && (s += "@supports (".concat(n.supports, ") {")), n.media && (s += "@media ".concat(n.media, " {"));
+                            var r = void 0 !== n.layer;
+                            r && (s += "@layer".concat(n.layer.length > 0 ? " ".concat(n.layer) : "", " {")), s += n.css, r && (s += "}"), n.media && (s += "}"), n.supports && (s += "}");
+                            var i = n.sourceMap;
+                            i && "undefined" != typeof btoa && (s += "\n/*# sourceMappingURL=data:application/json;base64,".concat(btoa(unescape(encodeURIComponent(JSON.stringify(i)))), " */")), t.styleTagTransform(s, e, t.options)
                         }(t, e, n)
                     },
                     remove: function() {
                         ! function(e) {
                             if (null === e.parentNode) return !1;
                             e.parentNode.removeChild(e)
                         }(t)
```

### Comparing `jupyter_power_usage-1.0.0/jupyter_power_usage/labextension/static/646.92e3ed3d9aea0d36c6a9.js` & `jupyter_power_usage-1.1.0/jupyter_power_usage/labextension/static/646.92e3ed3d9aea0d36c6a9.js`

 * *Files identical despite different names*

### Comparing `jupyter_power_usage-1.0.0/jupyter_power_usage/labextension/static/747.19551df7a36576f1c11f.js` & `jupyter_power_usage-1.1.0/jupyter_power_usage/labextension/static/747.19551df7a36576f1c11f.js`

 * *Files identical despite different names*

### Comparing `jupyter_power_usage-1.0.0/jupyter_power_usage/labextension/static/remoteEntry.8012d710f1db7c034cba.js` & `jupyter_power_usage-1.1.0/jupyter_power_usage/labextension/static/remoteEntry.20fe913e7d7c5e7492d8.js`

 * *Files 4% similar despite different names*

#### js-beautify {}

```diff
@@ -44,20 +44,20 @@
     }, j.d = (e, r) => {
         for (var t in r) j.o(r, t) && !j.o(e, t) && Object.defineProperty(e, t, {
             enumerable: !0,
             get: r[t]
         })
     }, j.f = {}, j.e = e => Promise.all(Object.keys(j.f).reduce(((r, t) => (j.f[t](e, r), r)), [])), j.u = e => e + "." + {
         29: "264e3efb1b2477b15441",
-        32: "df2f2b30253633c749ea",
+        32: "d626a962b7bd9192a1da",
         646: "92e3ed3d9aea0d36c6a9",
         747: "19551df7a36576f1c11f"
     } [e] + ".js?v=" + {
         29: "264e3efb1b2477b15441",
-        32: "df2f2b30253633c749ea",
+        32: "d626a962b7bd9192a1da",
         646: "92e3ed3d9aea0d36c6a9",
         747: "19551df7a36576f1c11f"
     } [e], j.g = function() {
         if ("object" == typeof globalThis) return globalThis;
         try {
             return this || new Function("return this")()
         } catch (e) {
@@ -111,15 +111,15 @@
                         (!u || !u.loaded && (!a != !u.eager ? a : i > u.from)) && (n[r] = {
                             get: t,
                             from: i,
                             eager: !!a
                         })
                     },
                     l = [];
-                return "default" === t && (u("@mahendrapaipuri/jupyter-power-usage", "1.0.0", (() => Promise.all([j.e(29), j.e(32)]).then((() => () => j(32))))), u("react-sparklines", "1.7.0", (() => Promise.all([j.e(646), j.e(29)]).then((() => () => j(646)))))), e[t] = l.length ? Promise.all(l).then((() => e[t] = 1)) : 1
+                return "default" === t && (u("@mahendrapaipuri/jupyter-power-usage", "1.1.0", (() => Promise.all([j.e(29), j.e(32)]).then((() => () => j(32))))), u("react-sparklines", "1.7.0", (() => Promise.all([j.e(646), j.e(29)]).then((() => () => j(646)))))), e[t] = l.length ? Promise.all(l).then((() => e[t] = 1)) : 1
             }
         }
     })(), (() => {
         var e;
         j.g.importScripts && (e = j.g.location + "");
         var r = j.g.document;
         if (!e && r && (r.currentScript && (e = r.currentScript.src), !e)) {
@@ -220,24 +220,24 @@
         var o = j.I(r);
         return o && o.then ? o.then(e.bind(e, r, j.S[r], t, a, n)) : e(r, j.S[r], t, a, n)
     })(((e, r, t, a) => (i(e, t), s(r, 0, t, a)))), v = c(((e, r, t, a, n) => {
         var o = r && j.o(r, t) && p(r, t, a);
         return o ? d(o) : n()
     })), g = {}, m = {
         29: () => h("default", "react", [1, 18, 2, 0]),
+        8: () => h("default", "@jupyterlab/settingregistry", [1, 4, 1, 5]),
+        217: () => h("default", "@jupyterlab/services", [1, 7, 1, 5]),
+        311: () => h("default", "@jupyterlab/coreutils", [1, 6, 1, 5]),
         496: () => v("default", "react-sparklines", [1, 1, 7, 0], (() => j.e(646).then((() => () => j(646))))),
-        614: () => h("default", "@jupyterlab/coreutils", [1, 6, 0, 7]),
-        684: () => h("default", "@jupyterlab/settingregistry", [1, 4, 0, 7]),
-        788: () => h("default", "@jupyterlab/services", [1, 7, 0, 7]),
+        510: () => h("default", "@jupyterlab/apputils", [1, 4, 2, 5]),
         797: () => h("default", "@lumino/polling", [1, 2, 0, 0]),
-        861: () => h("default", "@jupyterlab/apputils", [1, 4, 1, 7]),
         901: () => h("default", "@lumino/signaling", [1, 2, 0, 0])
     }, b = {
         29: [29],
-        32: [496, 614, 684, 788, 797, 861, 901]
+        32: [8, 217, 311, 496, 510, 797, 901]
     }, j.f.consumes = (e, r) => {
         j.o(b, e) && b[e].forEach((e => {
             if (j.o(g, e)) return r.push(g[e]);
             var t = r => {
                     g[e] = 0, j.m[e] = t => {
                         delete j.c[e], t.exports = r()
                     }
```

### Comparing `jupyter_power_usage-1.0.0/jupyter_power_usage/labextension/static/third-party-licenses.json` & `jupyter_power_usage-1.1.0/jupyter_power_usage/labextension/static/third-party-licenses.json`

 * *Files identical despite different names*

### Comparing `jupyter_power_usage-1.0.0/jupyter_power_usage/tests/test_basic.py` & `jupyter_power_usage-1.1.0/jupyter_power_usage/tests/test_basic.py`

 * *Files identical despite different names*

### Comparing `jupyter_power_usage-1.0.0/schema/plugin.json` & `jupyter_power_usage-1.1.0/schema/plugin.json`

 * *Files 6% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9985942322530863%*

 * *Differences: {"'definitions'": "{'emissions': {'properties': {'countryCode': {'description': 'ISO code of the "*

 * *                  "country of which emission factor will be used.', delete: ['enum', 'default']}, "*

 * *                  "'refreshRate': {'description': 'eCO2 emission factor will be updated at this "*

 * *                  "interval. Do not use too small intervals as these APIs are rate limited.'}, "*

 * *                  "'source': OrderedDict([('title', 'Source of emission factor'), ('description', "*

 * *                   […]*

```diff
@@ -9,32 +9,48 @@
                 }
             },
             "type": "object"
         },
         "emissions": {
             "properties": {
                 "countryCode": {
-                    "default": "",
-                    "description": "ISO code of the country of which emission factor will be used",
-                    "enum": [
-                        "",
-                        "fr"
-                    ],
+                    "description": "ISO code of the country of which emission factor will be used.",
                     "title": "Country code",
                     "type": "string"
                 },
+                "emapsAccessToken": {
+                    "description": "API Access token for Electricity Maps.",
+                    "title": "Electricity Maps Access token",
+                    "type": "string"
+                },
                 "factor": {
                     "description": "eCO2 emission factor will be used if Emission data for the selected country is not available.",
                     "title": "Emission factor (g/kWh)",
                     "type": "number"
                 },
                 "refreshRate": {
-                    "description": "eCO2 emission factor will be updated at this interval. Do not use too small intervals as these sort of APIs are rate limited.",
+                    "description": "eCO2 emission factor will be updated at this interval. Do not use too small intervals as these APIs are rate limited.",
                     "title": "Refresh rate (ms)",
                     "type": "number"
+                },
+                "source": {
+                    "default": "rte",
+                    "description": "Emission factor fetched from this source will be used. RTE eCO2 mix source is only available for France.",
+                    "oneOf": [
+                        {
+                            "const": "emaps",
+                            "title": "Electricity Maps"
+                        },
+                        {
+                            "const": "rte",
+                            "title": "RTE eCO2 mix"
+                        }
+                    ],
+                    "title": "Source of emission factor",
+                    "type": "string"
                 }
             },
             "type": "object"
         },
         "gpu": {
             "properties": {
                 "label": {
@@ -72,15 +88,16 @@
             },
             "description": "Settings for the CPU Power indicator",
             "title": "CPU Power Settings"
         },
         "emissions": {
             "$ref": "#/definitions/emissions",
             "default": {
-                "countryCode": "",
+                "countryCode": "FR",
+                "emapsAccessToken": "",
                 "factor": 475,
                 "refreshRate": 1800000
             },
             "description": "Settings for the estimating eCO2 emissions",
             "title": "Emissions Estimation Settings"
         },
         "gpu": {
```

### Comparing `jupyter_power_usage-1.0.0/src/cpuPowerView.tsx` & `jupyter_power_usage-1.1.0/src/cpuPowerView.tsx`

 * *Files identical despite different names*

### Comparing `jupyter_power_usage-1.0.0/src/emissionsHandler.ts` & `jupyter_power_usage-1.1.0/src/emissionsHandler.ts`

 * *Files 24% similar despite different names*

```diff
@@ -1,15 +1,19 @@
 import { URLExt } from '@jupyterlab/coreutils';
 
-namespace France {
+import { ServerConnection } from '@jupyterlab/services';
+
+import { EmissionFactor } from './model';
+
+namespace RTE {
   // Open Data Soft base and API URLs
   const OPENDATASOFT_API_BASEURL = 'https://odre.opendatasoft.com';
   const OPENDATASOFT_API_PATH = '/api/records/1.0/search/';
 
-  export const getOpenDataSoftEmissions = async (): Promise<number> => {
+  export const getOpenDataSoftEmissionFactor = async (): Promise<number> => {
     // Get current date in yyyy-mm-dd format
     const currentDate = new Date().toISOString().split('T')[0];
 
     // Make query params into a object
     const queryParams = {
       dataset: 'eco2mix-national-tr',
       facet: 'date_heure',
@@ -44,21 +48,100 @@
       console.info(`Request to Opendatasoft API failed due to ${error}`);
       return null;
     }
     return null;
   };
 }
 
+namespace ElectricityMaps {
+  // Open Data Soft base and API URLs
+  const EMAPS_API_BASEURL = 'https://api.electricitymap.org';
+  const EMAPS_API_PATH = '/v3/carbon-intensity/latest';
+
+  /**
+   * Settings for making requests to the server.
+   */
+  const SERVER_CONNECTION_SETTINGS = ServerConnection.makeSettings();
+
+  export const getElectricityMapsEmissionFactor = async (
+    proxy: boolean,
+    accessToken: string,
+    countryCode: string
+  ): Promise<number> => {
+    // Make query params into a object
+    const queryParams = {
+      zone: countryCode.toUpperCase(),
+    };
+
+    // Convert queryParams into encoded string
+    const queryString = URLExt.objectToQueryString(queryParams);
+
+    // Make request and get response data
+    try {
+      let apiUrl: string;
+
+      const requestHeaders: HeadersInit = new Headers();
+      // Set auth token if it is not empty
+      if (accessToken.length > 0) {
+        requestHeaders.set('auth-token', accessToken);
+      }
+
+      if (proxy) {
+        // Make a proxy request to electricty maps from jupyter server
+        apiUrl = URLExt.join(
+          SERVER_CONNECTION_SETTINGS.baseUrl,
+          'api/metrics/v1/emission_factor/emaps',
+          EMAPS_API_PATH,
+          queryString
+        );
+      } else {
+        // Make full API URL for making direct request from browser
+        apiUrl = URLExt.join(EMAPS_API_BASEURL, EMAPS_API_PATH, queryString);
+      }
+
+      // Make request
+      const response = await fetch(apiUrl, {
+        method: 'GET',
+        headers: requestHeaders,
+      });
+
+      if (!response.ok) {
+        console.debug('Request to Electricity Maps API failed');
+        return null;
+      }
+      const data = await response.json();
+      if (data && data.carbonIntensity) {
+        return data.carbonIntensity || 0;
+      }
+    } catch (error) {
+      console.info(`Request to Electricity Maps failed due to ${error}`);
+      return null;
+    }
+    return null;
+  };
+}
+
 /**
  * Get eCo2 Emissions coefficient in g/kWh for a given country
  *
- * @param countryCode ISO code of the country e.g. fr, uk, us, de.
+ * @param countryCode ISO code of the country e.g. FR, UK, US, DE.
  */
-async function getEmissions(countryCode: string): Promise<number> {
-  if (countryCode === 'fr') {
-    return await France.getOpenDataSoftEmissions();
+async function getEmissions(
+  source: string,
+  proxy: boolean,
+  accessTokens: EmissionFactor.Model.IAccessTokens,
+  countryCode: string
+): Promise<number> {
+  if (source === 'rte') {
+    return await RTE.getOpenDataSoftEmissionFactor();
+  } else if (source === 'emaps') {
+    return await ElectricityMaps.getElectricityMapsEmissionFactor(
+      proxy,
+      accessTokens.emaps,
+      countryCode
+    );
   } else {
     return null;
   }
 }
 
 export default getEmissions;
```

### Comparing `jupyter_power_usage-1.0.0/src/emissionsView.tsx` & `jupyter_power_usage-1.1.0/src/emissionsView.tsx`

 * *Files identical despite different names*

### Comparing `jupyter_power_usage-1.0.0/src/format.ts` & `jupyter_power_usage-1.1.0/src/format.ts`

 * *Files identical despite different names*

### Comparing `jupyter_power_usage-1.0.0/src/gpuPowerView.tsx` & `jupyter_power_usage-1.1.0/src/gpuPowerView.tsx`

 * *Files identical despite different names*

### Comparing `jupyter_power_usage-1.0.0/src/index.ts` & `jupyter_power_usage-1.1.0/src/index.ts`

 * *Files 14% similar despite different names*

```diff
@@ -46,24 +46,31 @@
 
 /**
  * The default emission factor to use in case on unavailable data
  */
 const DEFAULT_EMISSION_FACTOR = 475;
 
 /**
+ * The default emission factor source
+ */
+const DEFAULT_EMISSION_FACTOR_SOURCE = 'rte';
+
+/**
  * An interface for resource settings.
  */
 interface IResourceSettings extends JSONObject {
   label: string;
 }
 
 /**
  * An interface for emissions settings.
  */
 interface IEmissionsSettings extends JSONObject {
+  source: string;
+  emapsAccessToken: string;
   countryCode: string;
   refreshRate: number;
   factor: number;
 }
 
 /**
  * Initialization data for the jupyterlab-system-monitor extension.
@@ -80,28 +87,32 @@
   ) => {
     console.log('@mahendrapaipuri/jupyter-power-usage extension is activated');
 
     let refreshRate = DEFAULT_RAPL_REFRESH_RATE;
     let cpuPowerLabel = DEFAULT_CPU_POWER_LABEL;
     let gpuPowerLabel = DEFAULT_GPU_POWER_LABEL;
     let emissionsRefreshRate = DEFAULT_EMISSIONS_REFRESH_RATE;
+    let emissionFactorSource = DEFAULT_EMISSION_FACTOR_SOURCE;
+    let emapsAccessToken = '';
     let countryCode = DEFAULT_COUNTRY_CODE;
     let emissionFactor = DEFAULT_EMISSION_FACTOR;
 
     if (settingRegistry) {
       const settings = await settingRegistry.load(extension.id);
       refreshRate = settings.get('refreshRate').composite as number;
       if (refreshRate < DEFAULT_RAPL_REFRESH_RATE) {
         console.log(
           `Refresh rate is floored at ${DEFAULT_RAPL_REFRESH_RATE} ms`
         );
         refreshRate = DEFAULT_RAPL_REFRESH_RATE;
       }
       const emissionsSettings = settings.get('emissions')
         .composite as IEmissionsSettings;
+      emissionFactorSource = emissionsSettings.source;
+      emapsAccessToken = emissionsSettings.emapsAccessToken;
       countryCode = emissionsSettings.countryCode;
       emissionsRefreshRate = emissionsSettings.refreshRate;
       emissionFactor = emissionsSettings.factor;
       if (emissionsRefreshRate < DEFAULT_EMISSIONS_REFRESH_RATE) {
         console.log(
           `Emissions update interval is floored at ${DEFAULT_EMISSIONS_REFRESH_RATE} ms`
         );
@@ -111,14 +122,18 @@
       cpuPowerLabel = cpuSettings.label;
       const gpuSettings = settings.get('gpu').composite as IResourceSettings;
       gpuPowerLabel = gpuSettings.label;
     }
 
     const emissionsModel = new EmissionFactor.Model({
       refreshRate: emissionsRefreshRate,
+      emissionFactorSource: emissionFactorSource,
+      accessTokens: {
+        emaps: emapsAccessToken,
+      },
       countryCode: countryCode,
       defaultEmissionFactor: emissionFactor,
     });
     await emissionsModel.refresh();
 
     const model = new PowerUsage.Model(emissionsModel, { refreshRate });
     await model.refresh();
```

### Comparing `jupyter_power_usage-1.0.0/src/indicator.tsx` & `jupyter_power_usage-1.1.0/src/indicator.tsx`

 * *Files identical despite different names*

### Comparing `jupyter_power_usage-1.0.0/src/model.ts` & `jupyter_power_usage-1.1.0/src/model.ts`

 * *Files 3% similar despite different names*

```diff
@@ -309,17 +309,52 @@
   export class Model {
     /**
      * Construct a new eCo2 emissions model.
      *
      * @param options The options for creating the model.
      */
     constructor(options: Model.IOptions) {
+      // Test an api request to the jupyter server
+      // to see if the access token is set on server.
+      // If so, use that. If not, warn the user and
+      // use the client-side access token.
+      if (options.emissionFactorSource === 'emaps') {
+        new Promise<boolean>(() => {
+          getEmissions(
+            options.emissionFactorSource,
+            true,
+            options.accessTokens,
+            options.countryCode
+          )
+            .then((result) => {
+              if (!result) {
+                this._useProxy = false;
+              } else {
+                this._useProxy = true;
+              }
+            })
+            .catch(() => {
+              console.warn(
+                'Emission factor from Electricity maps will be fetched ' +
+                  'by making API requests directly from the browser. ' +
+                  'If a access token has been set, this can pose security risks. ' +
+                  'Please configure the access token on Jupyter server extension.'
+              );
+              this._useProxy = false;
+            });
+        });
+      }
+
+      // Set polling
       this._poll = new Poll<number | null>({
         factory: (): Promise<number> =>
           Private.emissionsFactory(
+            options.emissionFactorSource,
+            this._useProxy,
+            options.accessTokens,
             options.countryCode,
             options.defaultEmissionFactor
           ),
         frequency: {
           interval: options.refreshRate,
           backoff: true,
         },
@@ -389,33 +424,54 @@
       this._emissionFactorAvailable = emissionFactor !== null;
 
       this._currentEmissionFactor = emissionFactor;
       this._changed.emit(void 0);
     }
 
     private _emissionFactorAvailable = false;
+    private _useProxy = false;
     private _currentEmissionFactor: number | null = null;
     private _poll: Poll<number | null>;
     private _changed = new Signal<this, void>(this);
   }
 
   /**
    * A namespace for Model statics.
    */
   export namespace Model {
     /**
+     * Access tokens for emission sources.
+     */
+    export interface IAccessTokens {
+      /**
+       * The API access token for Electricity maps.
+       */
+      emaps: string;
+    }
+
+    /**
      * Options for creating a Emissions model.
      */
     export interface IOptions {
       /**
        * The refresh rate (in ms) for updating emissions (g/kWh) value.
        */
       refreshRate: number;
 
       /**
+       * The source of the emission factor.
+       */
+      emissionFactorSource: string;
+
+      /**
+       * The API access token for emission factor sources.
+       */
+      accessTokens: IAccessTokens;
+
+      /**
        * The country for which we are querying emissions API server.
        */
       countryCode: string;
 
       /**
        * Default emissions factor that will be used in case of unavailable data
        */
@@ -479,19 +535,27 @@
       return null;
     };
 
   /**
    * Make a request to the emissions backend.
    */
   export const emissionsFactory = async (
+    emissionFactorSource: string,
+    proxy: boolean,
+    accessTokens: EmissionFactor.Model.IAccessTokens,
     countryCode: string,
     defaultEmissionFactor: number
   ): Promise<number | null> => {
     // This is emission factor typically expressed in g/kWh
     // We convert it to mg/Ws here
-    const emissionFactor = await getEmissions(countryCode);
+    const emissionFactor = await getEmissions(
+      emissionFactorSource,
+      proxy,
+      accessTokens,
+      countryCode
+    );
     if (emissionFactor) {
       return emissionFactor / EF_UNIT_CONVERSION;
     }
     return defaultEmissionFactor / EF_UNIT_CONVERSION;
   };
 }
```

### Comparing `jupyter_power_usage-1.0.0/style/base.css` & `jupyter_power_usage-1.1.0/style/base.css`

 * *Files identical despite different names*

### Comparing `jupyter_power_usage-1.0.0/.gitignore` & `jupyter_power_usage-1.1.0/.gitignore`

 * *Files identical despite different names*

### Comparing `jupyter_power_usage-1.0.0/LICENSE` & `jupyter_power_usage-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `jupyter_power_usage-1.0.0/README.md` & `jupyter_power_usage-1.1.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -60,27 +60,35 @@
 
 - `process`: Power usage for current process and its children will be reported
 - `user`: Power usage for current user processes will be reported
 - `system`: Power usage for entire system will be reported.
 
 By default `process` scope is used. The user can change it by CLI flag `--PowerUsageDisplay.measurement_scope` to `jupyter lab` command. Alternatively, it can be configured in `jupyter_server_config.json` in [Jupyter config directory](https://docs.jupyter.org/en/latest/use/jupyter-directories.html#configuration-files).
 
+#### Electricity Maps API token
+
+An API token for electricity maps emission factor. By default API requests are made from jupyter server as they involve including authentication token. These are called proxied requests. If they fail, API requests directly from the browser will be made using the API token configured in the frontend extension. Users should configure the token on the server config as exposing API token in browsers can pose security issues. It can be set on CLI using `--PowerUsageDisplay.emaps_access_token=<token>`.
+
 ### Frontend extension config
 
 ![Frontend extension settings](https://raw.githubusercontent.com/mahendrapaipuri/jupyter-power-usage/main/doc/frontend-settings.png)
 
 The frontend extension settings can be accessed by `Settings -> Advanced Settings -> Power Usage Monitor` in JupyterLab. Important settings are:
 
 - `Refresh Rate`: Frequency at which power usage is updated in the JupyterLab. Do not use too small intervals as it will end up making too many API calls to update metrics.
 
 - `CPU label` and `GPU label` settings are self explanatory.
 
 **Emissions Estimation Settings**
 
-- `Country code`: Currently only data for France is supported. The realtime emission factor from [RTE eCO<sub>2</sub> mix](https://www.rte-france.com/en/eco2mix/co2-emissions). We encourage users to add support for other countries. Please check [`CONTRIBUTING.md`](CONTRIBUTING.md) on how to do it. If your country is not available in the list, leave it blank.
+- `Source of emission factor`: Currently [Electricity Maps](https://www.electricitymaps.com/) and [RTE eCO<sub>2</sub> mix](https://www.rte-france.com/en/eco2mix/co2-emissions) are supported. Note that RTE eCO<sub>2</sub> mix data is only available for France.
+
+- `Electricity Maps Access token`: An API access token for Electricity Maps (See [Server Config](#electricity-maps-api-token)).
+
+- `Country code`: ISO 3166-1 alpha-2 country code. This will be used only when `Electricity Maps` emission factor source is used.
 
 - `Refresh rate`: This defines how often the emission factor is updated in ms. For [RTE eCO<sub>2</sub> mix](https://www.rte-france.com/en/eco2mix/co2-emissions) data, it is updated every 30 min and has a rate limit of 50000 API requests per month.
 
 - `Emission factor`: This constant emission factor is used in the estimation of emissions when country specific data is unavailable.
 
 ## Contributing
```

### Comparing `jupyter_power_usage-1.0.0/pyproject.toml` & `jupyter_power_usage-1.1.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `jupyter_power_usage-1.0.0/PKG-INFO` & `jupyter_power_usage-1.1.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,11 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: jupyter_power_usage
-Version: 1.0.0
+Version: 1.1.0
+Dynamic: Keywords
 Summary: Extension that shows system power usage
 Project-URL: Homepage, https://github.com/mahendrapaipuri/jupyter-power-usage
 Project-URL: Bug Tracker, https://github.com/mahendrapaipuri/jupyter-power-usage/issues
 Project-URL: Repository, https://github.com/mahendrapaipuri/jupyter-power-usage.git
 Author-email: Mahendra Paipuri <mahendra.paipuri@cnrs.fr>
 License:                                  Apache License
                                    Version 2.0, January 2004
@@ -295,27 +296,35 @@
 
 - `process`: Power usage for current process and its children will be reported
 - `user`: Power usage for current user processes will be reported
 - `system`: Power usage for entire system will be reported.
 
 By default `process` scope is used. The user can change it by CLI flag `--PowerUsageDisplay.measurement_scope` to `jupyter lab` command. Alternatively, it can be configured in `jupyter_server_config.json` in [Jupyter config directory](https://docs.jupyter.org/en/latest/use/jupyter-directories.html#configuration-files).
 
+#### Electricity Maps API token
+
+An API token for electricity maps emission factor. By default API requests are made from jupyter server as they involve including authentication token. These are called proxied requests. If they fail, API requests directly from the browser will be made using the API token configured in the frontend extension. Users should configure the token on the server config as exposing API token in browsers can pose security issues. It can be set on CLI using `--PowerUsageDisplay.emaps_access_token=<token>`.
+
 ### Frontend extension config
 
 ![Frontend extension settings](https://raw.githubusercontent.com/mahendrapaipuri/jupyter-power-usage/main/doc/frontend-settings.png)
 
 The frontend extension settings can be accessed by `Settings -> Advanced Settings -> Power Usage Monitor` in JupyterLab. Important settings are:
 
 - `Refresh Rate`: Frequency at which power usage is updated in the JupyterLab. Do not use too small intervals as it will end up making too many API calls to update metrics.
 
 - `CPU label` and `GPU label` settings are self explanatory.
 
 **Emissions Estimation Settings**
 
-- `Country code`: Currently only data for France is supported. The realtime emission factor from [RTE eCO<sub>2</sub> mix](https://www.rte-france.com/en/eco2mix/co2-emissions). We encourage users to add support for other countries. Please check [`CONTRIBUTING.md`](CONTRIBUTING.md) on how to do it. If your country is not available in the list, leave it blank.
+- `Source of emission factor`: Currently [Electricity Maps](https://www.electricitymaps.com/) and [RTE eCO<sub>2</sub> mix](https://www.rte-france.com/en/eco2mix/co2-emissions) are supported. Note that RTE eCO<sub>2</sub> mix data is only available for France.
+
+- `Electricity Maps Access token`: An API access token for Electricity Maps (See [Server Config](#electricity-maps-api-token)).
+
+- `Country code`: ISO 3166-1 alpha-2 country code. This will be used only when `Electricity Maps` emission factor source is used.
 
 - `Refresh rate`: This defines how often the emission factor is updated in ms. For [RTE eCO<sub>2</sub> mix](https://www.rte-france.com/en/eco2mix/co2-emissions) data, it is updated every 30 min and has a rate limit of 50000 API requests per month.
 
 - `Emission factor`: This constant emission factor is used in the estimation of emissions when country specific data is unavailable.
 
 ## Contributing
```

