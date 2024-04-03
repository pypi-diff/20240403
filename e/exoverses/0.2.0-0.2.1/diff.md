# Comparing `tmp/exoverses-0.2.0.tar.gz` & `tmp/exoverses-0.2.1.tar.gz`

## Comparing `exoverses-0.2.0.tar` & `exoverses-0.2.1.tar`

### file list

```diff
@@ -1,34 +1,34 @@
--rw-r--r--   0        0        0      554 2020-02-02 00:00:00.000000 exoverses-0.2.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0      949 2020-02-02 00:00:00.000000 exoverses-0.2.0/CHANGELOG.md
--rw-r--r--   0        0        0     4290 2020-02-02 00:00:00.000000 exoverses-0.2.0/README.md
--rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 exoverses-0.2.0/.github/dependabot.yml
--rw-r--r--   0        0        0     1143 2020-02-02 00:00:00.000000 exoverses-0.2.0/.github/workflows/publish-to-pypi.yml
--rw-r--r--   0        0        0      663 2020-02-02 00:00:00.000000 exoverses-0.2.0/.github/workflows/release-please.yml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 exoverses-0.2.0/src/exoverses/__init__.py
--rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 exoverses-0.2.0/src/exoverses/base/__init__.py
--rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 exoverses-0.2.0/src/exoverses/base/disk.py
--rw-r--r--   0        0        0     9844 2020-02-02 00:00:00.000000 exoverses-0.2.0/src/exoverses/base/planet.py
--rw-r--r--   0        0        0     1266 2020-02-02 00:00:00.000000 exoverses-0.2.0/src/exoverses/base/star.py
--rw-r--r--   0        0        0    15238 2020-02-02 00:00:00.000000 exoverses-0.2.0/src/exoverses/base/system.py
--rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 exoverses-0.2.0/src/exoverses/base/universe.py
--rw-r--r--   0        0        0     7395 2020-02-02 00:00:00.000000 exoverses-0.2.0/src/exoverses/data/mamajek_rhk.csv
--rw-r--r--   0        0        0      275 2020-02-02 00:00:00.000000 exoverses-0.2.0/src/exoverses/exosims/__init__.py
--rw-r--r--   0        0        0     1910 2020-02-02 00:00:00.000000 exoverses-0.2.0/src/exoverses/exosims/planet.py
--rw-r--r--   0        0        0     2554 2020-02-02 00:00:00.000000 exoverses-0.2.0/src/exoverses/exosims/star.py
--rw-r--r--   0        0        0     1625 2020-02-02 00:00:00.000000 exoverses-0.2.0/src/exoverses/exosims/system.py
--rw-r--r--   0        0        0     2029 2020-02-02 00:00:00.000000 exoverses-0.2.0/src/exoverses/exosims/universe.py
--rw-r--r--   0        0        0      334 2020-02-02 00:00:00.000000 exoverses-0.2.0/src/exoverses/exovista/__init__.py
--rw-r--r--   0        0        0     3577 2020-02-02 00:00:00.000000 exoverses-0.2.0/src/exoverses/exovista/disk.py
--rw-r--r--   0        0        0     4868 2020-02-02 00:00:00.000000 exoverses-0.2.0/src/exoverses/exovista/planet.py
--rw-r--r--   0        0        0     4462 2020-02-02 00:00:00.000000 exoverses-0.2.0/src/exoverses/exovista/star.py
--rw-r--r--   0        0        0     7603 2020-02-02 00:00:00.000000 exoverses-0.2.0/src/exoverses/exovista/system.py
--rw-r--r--   0        0        0     7554 2020-02-02 00:00:00.000000 exoverses-0.2.0/src/exoverses/exovista/universe.py
--rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 exoverses-0.2.0/src/exoverses/fit/__init__.py
--rw-r--r--   0        0        0     2644 2020-02-02 00:00:00.000000 exoverses-0.2.0/src/exoverses/fit/planet.py
--rw-r--r--   0        0        0     1942 2020-02-02 00:00:00.000000 exoverses-0.2.0/src/exoverses/fit/system.py
--rw-r--r--   0        0        0      449 2020-02-02 00:00:00.000000 exoverses-0.2.0/src/exoverses/util/__init__.py
--rw-r--r--   0        0        0    11910 2020-02-02 00:00:00.000000 exoverses-0.2.0/src/exoverses/util/misc.py
--rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 exoverses-0.2.0/.gitignore
--rw-r--r--   0        0        0     1067 2020-02-02 00:00:00.000000 exoverses-0.2.0/LICENSE
--rw-r--r--   0        0        0     1006 2020-02-02 00:00:00.000000 exoverses-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     6309 2020-02-02 00:00:00.000000 exoverses-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0      554 2020-02-02 00:00:00.000000 exoverses-0.2.1/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     1233 2020-02-02 00:00:00.000000 exoverses-0.2.1/CHANGELOG.md
+-rw-r--r--   0        0        0     4290 2020-02-02 00:00:00.000000 exoverses-0.2.1/README.md
+-rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 exoverses-0.2.1/.github/dependabot.yml
+-rw-r--r--   0        0        0     1143 2020-02-02 00:00:00.000000 exoverses-0.2.1/.github/workflows/publish-to-pypi.yml
+-rw-r--r--   0        0        0      663 2020-02-02 00:00:00.000000 exoverses-0.2.1/.github/workflows/release-please.yml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 exoverses-0.2.1/src/exoverses/__init__.py
+-rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 exoverses-0.2.1/src/exoverses/base/__init__.py
+-rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 exoverses-0.2.1/src/exoverses/base/disk.py
+-rw-r--r--   0        0        0     9844 2020-02-02 00:00:00.000000 exoverses-0.2.1/src/exoverses/base/planet.py
+-rw-r--r--   0        0        0     1347 2020-02-02 00:00:00.000000 exoverses-0.2.1/src/exoverses/base/star.py
+-rw-r--r--   0        0        0    15238 2020-02-02 00:00:00.000000 exoverses-0.2.1/src/exoverses/base/system.py
+-rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 exoverses-0.2.1/src/exoverses/base/universe.py
+-rw-r--r--   0        0        0     7395 2020-02-02 00:00:00.000000 exoverses-0.2.1/src/exoverses/data/mamajek_rhk.csv
+-rw-r--r--   0        0        0      275 2020-02-02 00:00:00.000000 exoverses-0.2.1/src/exoverses/exosims/__init__.py
+-rw-r--r--   0        0        0     1910 2020-02-02 00:00:00.000000 exoverses-0.2.1/src/exoverses/exosims/planet.py
+-rw-r--r--   0        0        0     2554 2020-02-02 00:00:00.000000 exoverses-0.2.1/src/exoverses/exosims/star.py
+-rw-r--r--   0        0        0     1625 2020-02-02 00:00:00.000000 exoverses-0.2.1/src/exoverses/exosims/system.py
+-rw-r--r--   0        0        0     2029 2020-02-02 00:00:00.000000 exoverses-0.2.1/src/exoverses/exosims/universe.py
+-rw-r--r--   0        0        0      334 2020-02-02 00:00:00.000000 exoverses-0.2.1/src/exoverses/exovista/__init__.py
+-rw-r--r--   0        0        0     3577 2020-02-02 00:00:00.000000 exoverses-0.2.1/src/exoverses/exovista/disk.py
+-rw-r--r--   0        0        0     4868 2020-02-02 00:00:00.000000 exoverses-0.2.1/src/exoverses/exovista/planet.py
+-rw-r--r--   0        0        0     4462 2020-02-02 00:00:00.000000 exoverses-0.2.1/src/exoverses/exovista/star.py
+-rw-r--r--   0        0        0     7603 2020-02-02 00:00:00.000000 exoverses-0.2.1/src/exoverses/exovista/system.py
+-rw-r--r--   0        0        0     7554 2020-02-02 00:00:00.000000 exoverses-0.2.1/src/exoverses/exovista/universe.py
+-rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 exoverses-0.2.1/src/exoverses/fit/__init__.py
+-rw-r--r--   0        0        0     2644 2020-02-02 00:00:00.000000 exoverses-0.2.1/src/exoverses/fit/planet.py
+-rw-r--r--   0        0        0     1942 2020-02-02 00:00:00.000000 exoverses-0.2.1/src/exoverses/fit/system.py
+-rw-r--r--   0        0        0      449 2020-02-02 00:00:00.000000 exoverses-0.2.1/src/exoverses/util/__init__.py
+-rw-r--r--   0        0        0    11910 2020-02-02 00:00:00.000000 exoverses-0.2.1/src/exoverses/util/misc.py
+-rw-r--r--   0        0        0     3089 2020-02-02 00:00:00.000000 exoverses-0.2.1/.gitignore
+-rw-r--r--   0        0        0     1067 2020-02-02 00:00:00.000000 exoverses-0.2.1/LICENSE
+-rw-r--r--   0        0        0     1006 2020-02-02 00:00:00.000000 exoverses-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0     6309 2020-02-02 00:00:00.000000 exoverses-0.2.1/PKG-INFO
```

### Comparing `exoverses-0.2.0/.pre-commit-config.yaml` & `exoverses-0.2.1/.pre-commit-config.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -2,20 +2,20 @@
   - repo: https://github.com/pre-commit/pre-commit-hooks
     rev: "v4.5.0"
     hooks:
       - id: trailing-whitespace
       - id: name-tests-test
       - id: end-of-file-fixer
   - repo: https://github.com/astral-sh/ruff-pre-commit
-    rev: v0.3.0
+    rev: v0.3.5
     hooks:
       # Run the linter.
       - id: ruff
         args: [ --fix ]
       # Run the formatter.
       - id: ruff-format
   - repo: https://github.com/compilerla/conventional-pre-commit
-    rev: v3.1.0
+    rev: v3.2.0
     hooks:
       - id: conventional-pre-commit
         stages: [commit-msg]
         args: []
```

### Comparing `exoverses-0.2.0/CHANGELOG.md` & `exoverses-0.2.1/CHANGELOG.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,16 @@
 # Changelog
 
+## [0.2.1](https://github.com/CoreySpohn/exoverses/compare/v0.2.0...v0.2.1) (2024-04-03)
+
+
+### Bug Fixes
+
+* **main:** Remove usage of deprecated open_text importlib.resources method ([4e77086](https://github.com/CoreySpohn/exoverses/commit/4e77086b372a0a02d4ce9608b8e0b151aa7fa86c))
+
 ## [0.2.0](https://github.com/CoreySpohn/exoverses/compare/v0.1.1...v0.2.0) (2024-04-03)
 
 
 ### Features
 
 * **main:** Add Kopparapu bins based on EXOSIMS implementation ([d49dd76](https://github.com/CoreySpohn/exoverses/commit/d49dd763af9c73d13e1dd7387a0940abc9976f15))
```

### Comparing `exoverses-0.2.0/README.md` & `exoverses-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `exoverses-0.2.0/.github/workflows/publish-to-pypi.yml` & `exoverses-0.2.1/.github/workflows/publish-to-pypi.yml`

 * *Files identical despite different names*

### Comparing `exoverses-0.2.0/.github/workflows/release-please.yml` & `exoverses-0.2.1/.github/workflows/release-please.yml`

 * *Files identical despite different names*

### Comparing `exoverses-0.2.0/src/exoverses/base/planet.py` & `exoverses-0.2.1/src/exoverses/base/planet.py`

 * *Files identical despite different names*

### Comparing `exoverses-0.2.0/src/exoverses/base/star.py` & `exoverses-0.2.1/src/exoverses/base/star.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,11 +1,13 @@
+from importlib.resources import files
+from pathlib import Path
+
 import astropy.constants as const
 import astropy.units as u
 import pandas as pd
-from importlib import resources
 
 
 class Star:
     """
     The star of a system
     """
 
@@ -26,15 +28,17 @@
             / u.s
             * (self.luminosity / const.L_sun) ** 0.5
             * (self.mass / const.M_sun) ** -1
             * (self.effective_temperature / (5777 * u.K)) ** -0.5
         ).decompose()
 
         # Magnetic activity noise scaling relation from Gupta 2021
-        with resources.open_text("exoverses.data", "mamajek_rhk.csv") as f:
-            rhk_df = pd.read_csv(f)
+        # Load rhk values from ExEP target list
+        rhk_df = pd.read_csv(
+            files("exoverses").joinpath(Path("data", "mamajek_rhk.csv"))
+        )
         if self.name in rhk_df["HIP"].values:
             logrhk = rhk_df.loc[rhk_df["HIP"] == self.name]["logR'HK"].item()
             logsigma_mag = 1.66 * logrhk + 8.39
             self.sigma_mag = 10**logsigma_mag * u.m / u.s
         else:
             self.sigma_mag = None
```

### Comparing `exoverses-0.2.0/src/exoverses/base/system.py` & `exoverses-0.2.1/src/exoverses/base/system.py`

 * *Files identical despite different names*

### Comparing `exoverses-0.2.0/src/exoverses/data/mamajek_rhk.csv` & `exoverses-0.2.1/src/exoverses/data/mamajek_rhk.csv`

 * *Files identical despite different names*

### Comparing `exoverses-0.2.0/src/exoverses/exosims/planet.py` & `exoverses-0.2.1/src/exoverses/exosims/planet.py`

 * *Files identical despite different names*

### Comparing `exoverses-0.2.0/src/exoverses/exosims/star.py` & `exoverses-0.2.1/src/exoverses/exosims/star.py`

 * *Files identical despite different names*

### Comparing `exoverses-0.2.0/src/exoverses/exosims/system.py` & `exoverses-0.2.1/src/exoverses/exosims/system.py`

 * *Files identical despite different names*

### Comparing `exoverses-0.2.0/src/exoverses/exosims/universe.py` & `exoverses-0.2.1/src/exoverses/exosims/universe.py`

 * *Files identical despite different names*

### Comparing `exoverses-0.2.0/src/exoverses/exovista/disk.py` & `exoverses-0.2.1/src/exoverses/exovista/disk.py`

 * *Files identical despite different names*

### Comparing `exoverses-0.2.0/src/exoverses/exovista/planet.py` & `exoverses-0.2.1/src/exoverses/exovista/planet.py`

 * *Files identical despite different names*

### Comparing `exoverses-0.2.0/src/exoverses/exovista/star.py` & `exoverses-0.2.1/src/exoverses/exovista/star.py`

 * *Files identical despite different names*

### Comparing `exoverses-0.2.0/src/exoverses/exovista/system.py` & `exoverses-0.2.1/src/exoverses/exovista/system.py`

 * *Files identical despite different names*

### Comparing `exoverses-0.2.0/src/exoverses/exovista/universe.py` & `exoverses-0.2.1/src/exoverses/exovista/universe.py`

 * *Files identical despite different names*

### Comparing `exoverses-0.2.0/src/exoverses/fit/planet.py` & `exoverses-0.2.1/src/exoverses/fit/planet.py`

 * *Files identical despite different names*

### Comparing `exoverses-0.2.0/src/exoverses/fit/system.py` & `exoverses-0.2.1/src/exoverses/fit/system.py`

 * *Files identical despite different names*

### Comparing `exoverses-0.2.0/src/exoverses/util/misc.py` & `exoverses-0.2.1/src/exoverses/util/misc.py`

 * *Files identical despite different names*

### Comparing `exoverses-0.2.0/.gitignore` & `exoverses-0.2.1/.gitignore`

 * *Files 4% similar despite different names*

```diff
@@ -154,7 +154,9 @@
 
 # PyCharm
 #  JetBrains specific template is maintained in a separate JetBrains.gitignore that can
 #  be found at https://github.com/github/gitignore/blob/main/Global/JetBrains.gitignore
 #  and can be added to the global gitignore or merged into this file.  For a more nuclear
 #  option (not recommended) you can uncomment the following to ignore the entire idea folder.
 #.idea/
+
+.DS_Store
```

### Comparing `exoverses-0.2.0/LICENSE` & `exoverses-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `exoverses-0.2.0/pyproject.toml` & `exoverses-0.2.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `exoverses-0.2.0/PKG-INFO` & `exoverses-0.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: exoverses
-Version: 0.2.0
+Version: 0.2.1
 Summary: A unified interface for the various tools that create universes for exoplanet simulations
 Project-URL: Homepage, https://github.com/CoreySpohn/exoverses
 Project-URL: Issues, https://github.com/CoreySpohn/exoverses/issues
 Author-email: Corey Spohn <corey.a.spohn@nasa.gov>
 License: MIT License
         
         Copyright (c) 2023 CoreySpohn
```

