# Comparing `tmp/pharmcat_runner-0.0.7.tar.gz` & `tmp/pharmcat_runner-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pharmcat_runner-0.0.7.tar", last modified: Wed Apr  3 14:55:38 2024, max compression
+gzip compressed data, was "pharmcat_runner-0.0.8.tar", last modified: Wed Apr  3 15:33:10 2024, max compression
```

## Comparing `pharmcat_runner-0.0.7.tar` & `pharmcat_runner-0.0.8.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 andrew     (501) staff       (20)        0 2024-04-03 14:55:38.736823 pharmcat_runner-0.0.7/
--rw-r--r--   0 andrew     (501) staff       (20)     1069 2024-03-13 18:49:35.000000 pharmcat_runner-0.0.7/LICENSE
--rw-r--r--   0 andrew     (501) staff       (20)     2066 2024-04-03 14:55:38.736909 pharmcat_runner-0.0.7/PKG-INFO
--rw-r--r--   0 andrew     (501) staff       (20)     1749 2024-04-03 14:38:19.000000 pharmcat_runner-0.0.7/README.md
-drwxr-xr-x   0 andrew     (501) staff       (20)        0 2024-04-03 14:55:38.735511 pharmcat_runner-0.0.7/pharmcat_runner/
--rw-r--r--   0 andrew     (501) staff       (20)        0 2024-03-30 14:33:33.000000 pharmcat_runner-0.0.7/pharmcat_runner/__init__.py
--rw-r--r--   0 andrew     (501) staff       (20)     3924 2024-04-03 14:29:46.000000 pharmcat_runner-0.0.7/pharmcat_runner/__main__.py
--rw-r--r--   0 andrew     (501) staff       (20)     2062 2024-03-27 16:23:40.000000 pharmcat_runner-0.0.7/pharmcat_runner/common.py
--rw-r--r--   0 andrew     (501) staff       (20)     7718 2024-04-03 14:32:50.000000 pharmcat_runner-0.0.7/pharmcat_runner/haplotype.py
--rw-r--r--   0 andrew     (501) staff       (20)     4941 2024-04-02 15:47:59.000000 pharmcat_runner-0.0.7/pharmcat_runner/install.py
--rw-r--r--   0 andrew     (501) staff       (20)    20896 2024-04-03 14:52:59.000000 pharmcat_runner-0.0.7/pharmcat_runner/parser.py
--rw-r--r--   0 andrew     (501) staff       (20)     6316 2024-04-03 13:55:28.000000 pharmcat_runner-0.0.7/pharmcat_runner/qc_metrics.py
-drwxr-xr-x   0 andrew     (501) staff       (20)        0 2024-04-03 14:55:38.736706 pharmcat_runner-0.0.7/pharmcat_runner/tests/
--rw-r--r--   0 andrew     (501) staff       (20)        0 2024-03-14 15:27:15.000000 pharmcat_runner-0.0.7/pharmcat_runner/tests/__init__.py
--rw-r--r--   0 andrew     (501) staff       (20)     1039 2024-03-15 14:45:11.000000 pharmcat_runner-0.0.7/pharmcat_runner/tests/test_haplotype.py
--rw-r--r--   0 andrew     (501) staff       (20)      950 2024-03-15 01:59:43.000000 pharmcat_runner-0.0.7/pharmcat_runner/tests/test_parser.py
--rw-r--r--   0 andrew     (501) staff       (20)     3843 2024-04-03 13:34:55.000000 pharmcat_runner-0.0.7/pharmcat_runner/utils.py
--rw-r--r--   0 andrew     (501) staff       (20)     5914 2024-04-03 14:35:07.000000 pharmcat_runner-0.0.7/pharmcat_runner/vcf.py
-drwxr-xr-x   0 andrew     (501) staff       (20)        0 2024-04-03 14:55:38.736312 pharmcat_runner-0.0.7/pharmcat_runner.egg-info/
--rw-r--r--   0 andrew     (501) staff       (20)     2066 2024-04-03 14:55:38.000000 pharmcat_runner-0.0.7/pharmcat_runner.egg-info/PKG-INFO
--rw-r--r--   0 andrew     (501) staff       (20)      625 2024-04-03 14:55:38.000000 pharmcat_runner-0.0.7/pharmcat_runner.egg-info/SOURCES.txt
--rw-r--r--   0 andrew     (501) staff       (20)        1 2024-04-03 14:55:38.000000 pharmcat_runner-0.0.7/pharmcat_runner.egg-info/dependency_links.txt
--rw-r--r--   0 andrew     (501) staff       (20)       67 2024-04-03 14:55:38.000000 pharmcat_runner-0.0.7/pharmcat_runner.egg-info/entry_points.txt
--rw-r--r--   0 andrew     (501) staff       (20)        7 2024-04-03 14:55:38.000000 pharmcat_runner-0.0.7/pharmcat_runner.egg-info/requires.txt
--rw-r--r--   0 andrew     (501) staff       (20)       16 2024-04-03 14:55:38.000000 pharmcat_runner-0.0.7/pharmcat_runner.egg-info/top_level.txt
--rw-r--r--   0 andrew     (501) staff       (20)      100 2024-04-03 14:55:38.737134 pharmcat_runner-0.0.7/setup.cfg
--rw-r--r--   0 andrew     (501) staff       (20)      647 2024-04-03 14:55:33.000000 pharmcat_runner-0.0.7/setup.py
+drwxr-xr-x   0 andrew     (501) staff       (20)        0 2024-04-03 15:33:10.695169 pharmcat_runner-0.0.8/
+-rw-r--r--   0 andrew     (501) staff       (20)     1069 2024-03-13 18:49:35.000000 pharmcat_runner-0.0.8/LICENSE
+-rw-r--r--   0 andrew     (501) staff       (20)     2051 2024-04-03 15:33:10.695259 pharmcat_runner-0.0.8/PKG-INFO
+-rw-r--r--   0 andrew     (501) staff       (20)     1734 2024-04-03 14:57:28.000000 pharmcat_runner-0.0.8/README.md
+drwxr-xr-x   0 andrew     (501) staff       (20)        0 2024-04-03 15:33:10.692052 pharmcat_runner-0.0.8/pharmcat_runner/
+-rw-r--r--   0 andrew     (501) staff       (20)        0 2024-03-30 14:33:33.000000 pharmcat_runner-0.0.8/pharmcat_runner/__init__.py
+-rw-r--r--   0 andrew     (501) staff       (20)     3916 2024-04-03 15:32:50.000000 pharmcat_runner-0.0.8/pharmcat_runner/__main__.py
+-rw-r--r--   0 andrew     (501) staff       (20)     2062 2024-03-27 16:23:40.000000 pharmcat_runner-0.0.8/pharmcat_runner/common.py
+-rw-r--r--   0 andrew     (501) staff       (20)     7737 2024-04-03 15:17:54.000000 pharmcat_runner-0.0.8/pharmcat_runner/haplotype.py
+-rw-r--r--   0 andrew     (501) staff       (20)     5096 2024-04-03 15:05:04.000000 pharmcat_runner-0.0.8/pharmcat_runner/install.py
+-rw-r--r--   0 andrew     (501) staff       (20)    20896 2024-04-03 14:52:59.000000 pharmcat_runner-0.0.8/pharmcat_runner/parser.py
+-rw-r--r--   0 andrew     (501) staff       (20)     6332 2024-04-03 14:59:55.000000 pharmcat_runner-0.0.8/pharmcat_runner/qc_metrics.py
+drwxr-xr-x   0 andrew     (501) staff       (20)        0 2024-04-03 15:33:10.694842 pharmcat_runner-0.0.8/pharmcat_runner/tests/
+-rw-r--r--   0 andrew     (501) staff       (20)        0 2024-03-14 15:27:15.000000 pharmcat_runner-0.0.8/pharmcat_runner/tests/__init__.py
+-rw-r--r--   0 andrew     (501) staff       (20)     1039 2024-03-15 14:45:11.000000 pharmcat_runner-0.0.8/pharmcat_runner/tests/test_haplotype.py
+-rw-r--r--   0 andrew     (501) staff       (20)      950 2024-03-15 01:59:43.000000 pharmcat_runner-0.0.8/pharmcat_runner/tests/test_parser.py
+-rw-r--r--   0 andrew     (501) staff       (20)     3860 2024-04-03 15:32:06.000000 pharmcat_runner-0.0.8/pharmcat_runner/utils.py
+-rw-r--r--   0 andrew     (501) staff       (20)     5987 2024-04-03 15:11:01.000000 pharmcat_runner-0.0.8/pharmcat_runner/vcf.py
+drwxr-xr-x   0 andrew     (501) staff       (20)        0 2024-04-03 15:33:10.694388 pharmcat_runner-0.0.8/pharmcat_runner.egg-info/
+-rw-r--r--   0 andrew     (501) staff       (20)     2051 2024-04-03 15:33:10.000000 pharmcat_runner-0.0.8/pharmcat_runner.egg-info/PKG-INFO
+-rw-r--r--   0 andrew     (501) staff       (20)      625 2024-04-03 15:33:10.000000 pharmcat_runner-0.0.8/pharmcat_runner.egg-info/SOURCES.txt
+-rw-r--r--   0 andrew     (501) staff       (20)        1 2024-04-03 15:33:10.000000 pharmcat_runner-0.0.8/pharmcat_runner.egg-info/dependency_links.txt
+-rw-r--r--   0 andrew     (501) staff       (20)       67 2024-04-03 15:33:10.000000 pharmcat_runner-0.0.8/pharmcat_runner.egg-info/entry_points.txt
+-rw-r--r--   0 andrew     (501) staff       (20)        7 2024-04-03 15:33:10.000000 pharmcat_runner-0.0.8/pharmcat_runner.egg-info/requires.txt
+-rw-r--r--   0 andrew     (501) staff       (20)       16 2024-04-03 15:33:10.000000 pharmcat_runner-0.0.8/pharmcat_runner.egg-info/top_level.txt
+-rw-r--r--   0 andrew     (501) staff       (20)      100 2024-04-03 15:33:10.695542 pharmcat_runner-0.0.8/setup.cfg
+-rw-r--r--   0 andrew     (501) staff       (20)      647 2024-04-03 15:33:07.000000 pharmcat_runner-0.0.8/setup.py
```

### Comparing `pharmcat_runner-0.0.7/LICENSE` & `pharmcat_runner-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `pharmcat_runner-0.0.7/PKG-INFO` & `pharmcat_runner-0.0.8/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pharmcat_runner
-Version: 0.0.7
+Version: 0.0.8
 Summary: Installs, runs, and parsers PharmCAT using Pharmacoscan input.
 Home-page: UNKNOWN
 Author: Andrew Haddad, PharmD
 Author-email: andrew.haddad@pitt.edu
 License: UNKNOWN
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
@@ -22,17 +22,15 @@
 ## Installation
 
 Installation can be acheived using pip or any other package manager of your choosing. It is highly recommended that installation is done with Python 3.9+. Some conda environments can conflict with installation of a new verison.
 ```sh
 pip install pharmcat_runner 
 ```
 
-## Parsing genotypes
-
-### CLI
+## Usage
 ```sh
 # Install PharmCAT and all required dependencies. If an installation already exists, must pass --overwrite to update
 python3 -m pharmcat_runner install
 
 # Run optional QC steps followed by PharmCAT
 python3 -m pharmcat_runner haplotype --files "data/*.vcf" --hwe 0.001 --variant_call_rate 0.95 --sample_call_rate 0.95
 
@@ -40,15 +38,15 @@
 # VCFs are required for accurate reporting of CYP2D6
 # Sex ids are required for accurate reporting of G6PD
 # Warnings are reported if either of these are not supplied
 python3 -m pharmcat_runner parser --files "results/pharmcat_output/*.json" --vcfs "data/*.vcf" --sex_ids sex_ids.txt
 ```
 
 ## sex_ids file
-This file is required for accurate reporting of G6PD genotypes and phenotypes. This should be a tab delimited file without a header. The two columns should be sample id and predicted sex (M-Male, F-Female, O-Other). The samples in this file must match the samples in the pharmcat output
+This file is required for accurate reporting of G6PD genotypes and phenotypes. This should be a tab delimited file without a header. The two columns should be sample id and predicted sex (M-Male, F-Female, O-Other). The sample ids in this file must match the sample ids in the pharmcat output
 |   |   |
 |---|---|
 |1234 | M |
 |5678 | F |
 |1357 | O |
 
 ## Bugs and desired features
```

### Comparing `pharmcat_runner-0.0.7/README.md` & `pharmcat_runner-0.0.8/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -10,17 +10,15 @@
 ## Installation
 
 Installation can be acheived using pip or any other package manager of your choosing. It is highly recommended that installation is done with Python 3.9+. Some conda environments can conflict with installation of a new verison.
 ```sh
 pip install pharmcat_runner 
 ```
 
-## Parsing genotypes
-
-### CLI
+## Usage
 ```sh
 # Install PharmCAT and all required dependencies. If an installation already exists, must pass --overwrite to update
 python3 -m pharmcat_runner install
 
 # Run optional QC steps followed by PharmCAT
 python3 -m pharmcat_runner haplotype --files "data/*.vcf" --hwe 0.001 --variant_call_rate 0.95 --sample_call_rate 0.95
 
@@ -28,15 +26,15 @@
 # VCFs are required for accurate reporting of CYP2D6
 # Sex ids are required for accurate reporting of G6PD
 # Warnings are reported if either of these are not supplied
 python3 -m pharmcat_runner parser --files "results/pharmcat_output/*.json" --vcfs "data/*.vcf" --sex_ids sex_ids.txt
 ```
 
 ## sex_ids file
-This file is required for accurate reporting of G6PD genotypes and phenotypes. This should be a tab delimited file without a header. The two columns should be sample id and predicted sex (M-Male, F-Female, O-Other). The samples in this file must match the samples in the pharmcat output
+This file is required for accurate reporting of G6PD genotypes and phenotypes. This should be a tab delimited file without a header. The two columns should be sample id and predicted sex (M-Male, F-Female, O-Other). The sample ids in this file must match the sample ids in the pharmcat output
 |   |   |
 |---|---|
 |1234 | M |
 |5678 | F |
 |1357 | O |
 
 ## Bugs and desired features
```

### Comparing `pharmcat_runner-0.0.7/pharmcat_runner/__main__.py` & `pharmcat_runner-0.0.8/pharmcat_runner/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,35 +17,33 @@
     if "linux" not in sys.platform.lower():
         raise OSError("Only linux systems are supported at this time.")
     install(overwrite=args.overwrite)
 
 
 def call_haplotype(args):
     validate_environment()
-    validate_directory(args.files)
+    validate_directory(args.files, file_ext=".vcf")
     if args.hwe or args.sample_call_rate:
         validate_plink()
     call_haplotypes(
         dir_=args.files,
         hwe=args.hwe,
         variant_call_rate=args.variant_call_rate,
         sample_call_rate=args.sample_call_rate,
         output_dir=args.output,
         debug=args.debug,
     )
 
 
 def call_parser(args):
-    validate_directory(args.files)
+    validate_directory(args.files, file_ext=".json")
     if args.sex_ids:
         validate_file(args.sex_ids)
     if args.vcfs:
-        validate_directory(args.vcfs)
-    if args.output:
-        validate_directory(args.output)
+        validate_directory(args.vcfs, file_ext=".vcf")
     parse_pharmcat_output(
         pharmcat_dir=args.files,
         vcf_dir=args.vcfs,
         sex_ids=args.sex_ids,
         output_dir=args.output,
     )
```

### Comparing `pharmcat_runner-0.0.7/pharmcat_runner/common.py` & `pharmcat_runner-0.0.8/pharmcat_runner/common.py`

 * *Files identical despite different names*

### Comparing `pharmcat_runner-0.0.7/pharmcat_runner/haplotype.py` & `pharmcat_runner-0.0.8/pharmcat_runner/haplotype.py`

 * *Files 1% similar despite different names*

```diff
@@ -167,22 +167,22 @@
             files = _get_files(dir_)
             print("Prepping files for PharmCAT...")
             vcf_standardized = standardize_vcfs(files=files, dir_=tempdir)
             pharmcat_variants_only_file = filter_vcf_for_variants(
                 file=vcf_standardized,
                 dir_=tempdir,
                 positions_file=pharmcat_positions_file,
-                exclusions='POS==42126599 || ID=="AX-165885131"',
+                exclusions='POS==42126599 || ID=="AX-165885131_chrX_154532990_CGGT_C"',
             )
 
             if any([hwe, variant_call_rate, sample_call_rate]):
                 print("Running pre-PharmCAT QC...")
                 qc_metrics = run_qc(
                     file=pharmcat_variants_only_file,
-                    tempdir=tempdir,
+                    dir_=tempdir,
                     hwe=hwe,
                     variant_call_rate=variant_call_rate,
                     sample_call_rate=sample_call_rate,
                 )
             try:
                 vcf_input = qc_metrics.output_file
             except NameError:
```

### Comparing `pharmcat_runner-0.0.7/pharmcat_runner/install.py` & `pharmcat_runner-0.0.8/pharmcat_runner/install.py`

 * *Files 3% similar despite different names*

```diff
@@ -74,23 +74,27 @@
     shutil.copy2(bash_profile_temp, bash_profile)
     os.remove(bash_profile_temp)
 
 
 def validate_python_version(tempdir):
     if not check_python_verison():
         try:
+            print(
+                "Incorrect version of Python was found. Attempting to install Python..."
+            )
             install_python(tempdir)
         except Exception:
             try:
                 shutil.rmtree(os.path.join(BIN_DIR, "python"))
             except FileNotFoundError:
                 pass
-            raise RuntimeError(
-                f"Requires Python v3.9+, found v{sys.version.split()[0]}. Attempt to install new version of Python was unsuccesful"
-            )
+            finally:
+                raise RuntimeError(
+                    f"Requires Python v3.9+, found v{sys.version.split()[0]}. Attempt to install new version of Python was unsuccesful"
+                )
         else:
             print("Successfully installed Python.")
 
 
 def install(overwrite=False):
     try:
         os.mkdir(BIN_DIR)
```

### Comparing `pharmcat_runner-0.0.7/pharmcat_runner/parser.py` & `pharmcat_runner-0.0.8/pharmcat_runner/parser.py`

 * *Files identical despite different names*

### Comparing `pharmcat_runner-0.0.7/pharmcat_runner/qc_metrics.py` & `pharmcat_runner-0.0.8/pharmcat_runner/qc_metrics.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import csv
 import os
 
 import pandas as pd
 
-from .utils import index_file, run_command
+from .utils import run_command
+from .vcf import index_file
 
 
 class QCMetrics:
     # Order matters in the QC metric operations
     # Genotype metrics -> variant metrics -> sample metrics
     # Therefore they cannot all be computed at the same time
```

### Comparing `pharmcat_runner-0.0.7/pharmcat_runner/tests/test_haplotype.py` & `pharmcat_runner-0.0.8/pharmcat_runner/tests/test_haplotype.py`

 * *Files identical despite different names*

### Comparing `pharmcat_runner-0.0.7/pharmcat_runner/tests/test_parser.py` & `pharmcat_runner-0.0.8/pharmcat_runner/tests/test_parser.py`

 * *Files identical despite different names*

### Comparing `pharmcat_runner-0.0.7/pharmcat_runner/utils.py` & `pharmcat_runner-0.0.8/pharmcat_runner/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -87,35 +87,35 @@
             shutil.rmtree(dir_)
         except FileNotFoundError:
             pass
     if not os.path.exists(dir_):
         os.mkdir(dir_)
 
 
-def validate_directory(dir_):
+def validate_directory(dir_, file_ext=None):
     if not isinstance(dir_, str):
         raise TypeError(f"Directory must be a string, got '{type(dir_)}'")
     glob_files = glob.glob(dir_)
     globbing = True
     for file in glob_files:
-        if ".vcf" in file:
+        if file_ext in file:
             break
     else:
         globbing = False
     if not globbing and len(os.listdir(dir_)) == 0:
         raise ValueError(
             f"Provided directory '{dir_}' does not exist or does not contain any files"
         )
 
 
 def check_python_verison():
     version_data = sys.version
     if int(version_data.split()[0].split(".")[1]) >= 9:
-        return False
-    return True
+        return True
+    return False
 
 
 def validate_plink():
     try:
         run_command(["plink", "-h"])
     except RuntimeError:
         raise RuntimeError(
```

### Comparing `pharmcat_runner-0.0.7/pharmcat_runner/vcf.py` & `pharmcat_runner-0.0.8/pharmcat_runner/vcf.py`

 * *Files 2% similar despite different names*

```diff
@@ -198,8 +198,10 @@
     )
     annotate_id_file = annotate_id(file=alignment_sorted)
 
     standardized_file = os.path.join(
         os.path.dirname(annotate_id_file), "standardized.vcf.gz"
     )
     shutil.copy2(annotate_id_file, standardized_file)
+    shutil.copy2(annotate_id_file + ".tbi", standardized_file + ".tbi")
+
     return standardized_file
```

### Comparing `pharmcat_runner-0.0.7/pharmcat_runner.egg-info/PKG-INFO` & `pharmcat_runner-0.0.8/pharmcat_runner.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pharmcat-runner
-Version: 0.0.7
+Version: 0.0.8
 Summary: Installs, runs, and parsers PharmCAT using Pharmacoscan input.
 Home-page: UNKNOWN
 Author: Andrew Haddad, PharmD
 Author-email: andrew.haddad@pitt.edu
 License: UNKNOWN
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
@@ -22,17 +22,15 @@
 ## Installation
 
 Installation can be acheived using pip or any other package manager of your choosing. It is highly recommended that installation is done with Python 3.9+. Some conda environments can conflict with installation of a new verison.
 ```sh
 pip install pharmcat_runner 
 ```
 
-## Parsing genotypes
-
-### CLI
+## Usage
 ```sh
 # Install PharmCAT and all required dependencies. If an installation already exists, must pass --overwrite to update
 python3 -m pharmcat_runner install
 
 # Run optional QC steps followed by PharmCAT
 python3 -m pharmcat_runner haplotype --files "data/*.vcf" --hwe 0.001 --variant_call_rate 0.95 --sample_call_rate 0.95
 
@@ -40,15 +38,15 @@
 # VCFs are required for accurate reporting of CYP2D6
 # Sex ids are required for accurate reporting of G6PD
 # Warnings are reported if either of these are not supplied
 python3 -m pharmcat_runner parser --files "results/pharmcat_output/*.json" --vcfs "data/*.vcf" --sex_ids sex_ids.txt
 ```
 
 ## sex_ids file
-This file is required for accurate reporting of G6PD genotypes and phenotypes. This should be a tab delimited file without a header. The two columns should be sample id and predicted sex (M-Male, F-Female, O-Other). The samples in this file must match the samples in the pharmcat output
+This file is required for accurate reporting of G6PD genotypes and phenotypes. This should be a tab delimited file without a header. The two columns should be sample id and predicted sex (M-Male, F-Female, O-Other). The sample ids in this file must match the sample ids in the pharmcat output
 |   |   |
 |---|---|
 |1234 | M |
 |5678 | F |
 |1357 | O |
 
 ## Bugs and desired features
```

### Comparing `pharmcat_runner-0.0.7/pharmcat_runner.egg-info/SOURCES.txt` & `pharmcat_runner-0.0.8/pharmcat_runner.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pharmcat_runner-0.0.7/setup.py` & `pharmcat_runner-0.0.8/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup, find_packages
 
 long_description = open("README.md").read()
 
 setup(
     name="pharmcat_runner",
-    version="0.0.7",
+    version="0.0.8",
     description="Installs, runs, and parsers PharmCAT using Pharmacoscan input.",
     author="Andrew Haddad, PharmD",
     author_email="andrew.haddad@pitt.edu",
     packages=find_packages(),
     long_description=long_description,
     long_description_content_type="text/markdown",
     entry_points={
```

