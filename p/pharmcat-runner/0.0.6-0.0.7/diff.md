# Comparing `tmp/pharmcat_runner-0.0.6.tar.gz` & `tmp/pharmcat_runner-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pharmcat_runner-0.0.6.tar", last modified: Sat Mar 30 16:03:29 2024, max compression
+gzip compressed data, was "pharmcat_runner-0.0.7.tar", last modified: Wed Apr  3 14:55:38 2024, max compression
```

## Comparing `pharmcat_runner-0.0.6.tar` & `pharmcat_runner-0.0.7.tar`

### file list

```diff
@@ -1,26 +1,27 @@
-drwxr-xr-x   0 andrew     (501) staff       (20)        0 2024-03-30 16:03:29.824222 pharmcat_runner-0.0.6/
--rw-r--r--   0 andrew     (501) staff       (20)     1069 2024-03-13 18:49:35.000000 pharmcat_runner-0.0.6/LICENSE
--rw-r--r--   0 andrew     (501) staff       (20)      324 2024-03-30 16:03:29.824297 pharmcat_runner-0.0.6/PKG-INFO
--rw-r--r--   0 andrew     (501) staff       (20)        0 2024-03-12 20:07:23.000000 pharmcat_runner-0.0.6/README.md
-drwxr-xr-x   0 andrew     (501) staff       (20)        0 2024-03-30 16:03:29.822678 pharmcat_runner-0.0.6/pharmcat_runner/
--rw-r--r--   0 andrew     (501) staff       (20)        0 2024-03-30 14:33:33.000000 pharmcat_runner-0.0.6/pharmcat_runner/__init__.py
--rw-r--r--   0 andrew     (501) staff       (20)     3924 2024-03-30 14:38:15.000000 pharmcat_runner-0.0.6/pharmcat_runner/__main__.py
--rw-r--r--   0 andrew     (501) staff       (20)     2062 2024-03-27 16:23:40.000000 pharmcat_runner-0.0.6/pharmcat_runner/common.py
--rw-r--r--   0 andrew     (501) staff       (20)    14719 2024-03-30 15:48:55.000000 pharmcat_runner-0.0.6/pharmcat_runner/haplotype.py
--rw-r--r--   0 andrew     (501) staff       (20)     4722 2024-03-30 15:11:33.000000 pharmcat_runner-0.0.6/pharmcat_runner/install.py
--rw-r--r--   0 andrew     (501) staff       (20)    20214 2024-03-30 16:03:11.000000 pharmcat_runner-0.0.6/pharmcat_runner/parser.py
--rw-r--r--   0 andrew     (501) staff       (20)     6352 2024-03-27 17:27:52.000000 pharmcat_runner-0.0.6/pharmcat_runner/qc_metrics.py
-drwxr-xr-x   0 andrew     (501) staff       (20)        0 2024-03-30 16:03:29.824068 pharmcat_runner-0.0.6/pharmcat_runner/tests/
--rw-r--r--   0 andrew     (501) staff       (20)        0 2024-03-14 15:27:15.000000 pharmcat_runner-0.0.6/pharmcat_runner/tests/__init__.py
--rw-r--r--   0 andrew     (501) staff       (20)     1039 2024-03-15 14:45:11.000000 pharmcat_runner-0.0.6/pharmcat_runner/tests/test_haplotype.py
--rw-r--r--   0 andrew     (501) staff       (20)      950 2024-03-15 01:59:43.000000 pharmcat_runner-0.0.6/pharmcat_runner/tests/test_parser.py
--rw-r--r--   0 andrew     (501) staff       (20)     3870 2024-03-30 15:54:26.000000 pharmcat_runner-0.0.6/pharmcat_runner/utils.py
-drwxr-xr-x   0 andrew     (501) staff       (20)        0 2024-03-30 16:03:29.823675 pharmcat_runner-0.0.6/pharmcat_runner.egg-info/
--rw-r--r--   0 andrew     (501) staff       (20)      324 2024-03-30 16:03:29.000000 pharmcat_runner-0.0.6/pharmcat_runner.egg-info/PKG-INFO
--rw-r--r--   0 andrew     (501) staff       (20)      602 2024-03-30 16:03:29.000000 pharmcat_runner-0.0.6/pharmcat_runner.egg-info/SOURCES.txt
--rw-r--r--   0 andrew     (501) staff       (20)        1 2024-03-30 16:03:29.000000 pharmcat_runner-0.0.6/pharmcat_runner.egg-info/dependency_links.txt
--rw-r--r--   0 andrew     (501) staff       (20)       67 2024-03-30 16:03:29.000000 pharmcat_runner-0.0.6/pharmcat_runner.egg-info/entry_points.txt
--rw-r--r--   0 andrew     (501) staff       (20)        7 2024-03-30 16:03:29.000000 pharmcat_runner-0.0.6/pharmcat_runner.egg-info/requires.txt
--rw-r--r--   0 andrew     (501) staff       (20)       16 2024-03-30 16:03:29.000000 pharmcat_runner-0.0.6/pharmcat_runner.egg-info/top_level.txt
--rw-r--r--   0 andrew     (501) staff       (20)      100 2024-03-30 16:03:29.824506 pharmcat_runner-0.0.6/setup.cfg
--rw-r--r--   0 andrew     (501) staff       (20)      647 2024-03-30 16:03:26.000000 pharmcat_runner-0.0.6/setup.py
+drwxr-xr-x   0 andrew     (501) staff       (20)        0 2024-04-03 14:55:38.736823 pharmcat_runner-0.0.7/
+-rw-r--r--   0 andrew     (501) staff       (20)     1069 2024-03-13 18:49:35.000000 pharmcat_runner-0.0.7/LICENSE
+-rw-r--r--   0 andrew     (501) staff       (20)     2066 2024-04-03 14:55:38.736909 pharmcat_runner-0.0.7/PKG-INFO
+-rw-r--r--   0 andrew     (501) staff       (20)     1749 2024-04-03 14:38:19.000000 pharmcat_runner-0.0.7/README.md
+drwxr-xr-x   0 andrew     (501) staff       (20)        0 2024-04-03 14:55:38.735511 pharmcat_runner-0.0.7/pharmcat_runner/
+-rw-r--r--   0 andrew     (501) staff       (20)        0 2024-03-30 14:33:33.000000 pharmcat_runner-0.0.7/pharmcat_runner/__init__.py
+-rw-r--r--   0 andrew     (501) staff       (20)     3924 2024-04-03 14:29:46.000000 pharmcat_runner-0.0.7/pharmcat_runner/__main__.py
+-rw-r--r--   0 andrew     (501) staff       (20)     2062 2024-03-27 16:23:40.000000 pharmcat_runner-0.0.7/pharmcat_runner/common.py
+-rw-r--r--   0 andrew     (501) staff       (20)     7718 2024-04-03 14:32:50.000000 pharmcat_runner-0.0.7/pharmcat_runner/haplotype.py
+-rw-r--r--   0 andrew     (501) staff       (20)     4941 2024-04-02 15:47:59.000000 pharmcat_runner-0.0.7/pharmcat_runner/install.py
+-rw-r--r--   0 andrew     (501) staff       (20)    20896 2024-04-03 14:52:59.000000 pharmcat_runner-0.0.7/pharmcat_runner/parser.py
+-rw-r--r--   0 andrew     (501) staff       (20)     6316 2024-04-03 13:55:28.000000 pharmcat_runner-0.0.7/pharmcat_runner/qc_metrics.py
+drwxr-xr-x   0 andrew     (501) staff       (20)        0 2024-04-03 14:55:38.736706 pharmcat_runner-0.0.7/pharmcat_runner/tests/
+-rw-r--r--   0 andrew     (501) staff       (20)        0 2024-03-14 15:27:15.000000 pharmcat_runner-0.0.7/pharmcat_runner/tests/__init__.py
+-rw-r--r--   0 andrew     (501) staff       (20)     1039 2024-03-15 14:45:11.000000 pharmcat_runner-0.0.7/pharmcat_runner/tests/test_haplotype.py
+-rw-r--r--   0 andrew     (501) staff       (20)      950 2024-03-15 01:59:43.000000 pharmcat_runner-0.0.7/pharmcat_runner/tests/test_parser.py
+-rw-r--r--   0 andrew     (501) staff       (20)     3843 2024-04-03 13:34:55.000000 pharmcat_runner-0.0.7/pharmcat_runner/utils.py
+-rw-r--r--   0 andrew     (501) staff       (20)     5914 2024-04-03 14:35:07.000000 pharmcat_runner-0.0.7/pharmcat_runner/vcf.py
+drwxr-xr-x   0 andrew     (501) staff       (20)        0 2024-04-03 14:55:38.736312 pharmcat_runner-0.0.7/pharmcat_runner.egg-info/
+-rw-r--r--   0 andrew     (501) staff       (20)     2066 2024-04-03 14:55:38.000000 pharmcat_runner-0.0.7/pharmcat_runner.egg-info/PKG-INFO
+-rw-r--r--   0 andrew     (501) staff       (20)      625 2024-04-03 14:55:38.000000 pharmcat_runner-0.0.7/pharmcat_runner.egg-info/SOURCES.txt
+-rw-r--r--   0 andrew     (501) staff       (20)        1 2024-04-03 14:55:38.000000 pharmcat_runner-0.0.7/pharmcat_runner.egg-info/dependency_links.txt
+-rw-r--r--   0 andrew     (501) staff       (20)       67 2024-04-03 14:55:38.000000 pharmcat_runner-0.0.7/pharmcat_runner.egg-info/entry_points.txt
+-rw-r--r--   0 andrew     (501) staff       (20)        7 2024-04-03 14:55:38.000000 pharmcat_runner-0.0.7/pharmcat_runner.egg-info/requires.txt
+-rw-r--r--   0 andrew     (501) staff       (20)       16 2024-04-03 14:55:38.000000 pharmcat_runner-0.0.7/pharmcat_runner.egg-info/top_level.txt
+-rw-r--r--   0 andrew     (501) staff       (20)      100 2024-04-03 14:55:38.737134 pharmcat_runner-0.0.7/setup.cfg
+-rw-r--r--   0 andrew     (501) staff       (20)      647 2024-04-03 14:55:33.000000 pharmcat_runner-0.0.7/setup.py
```

### Comparing `pharmcat_runner-0.0.6/LICENSE` & `pharmcat_runner-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `pharmcat_runner-0.0.6/pharmcat_runner/__main__.py` & `pharmcat_runner-0.0.7/pharmcat_runner/__main__.py`

 * *Files identical despite different names*

### Comparing `pharmcat_runner-0.0.6/pharmcat_runner/common.py` & `pharmcat_runner-0.0.7/pharmcat_runner/common.py`

 * *Files identical despite different names*

### Comparing `pharmcat_runner-0.0.6/pharmcat_runner/install.py` & `pharmcat_runner-0.0.7/pharmcat_runner/install.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import os
 import shutil
 import sys
 import traceback
 from tempfile import TemporaryDirectory
 
 from .common import *
-from .utils import curl, run_command, unpack_tar
+from .utils import curl, run_command, unpack_tar, check_python_verison
 
 
 def install_java(tempdir):
     curl(tempdir, JAVA_URL)
     unpack_tar(file=os.path.join(tempdir, os.path.basename(JAVA_URL)), dir_=BIN_DIR)
 
 
@@ -71,18 +71,28 @@
             for file in os.listdir(BIN_DIR):
                 if "jdk" in file:
                     f_out.write(f'export JAVA_HOME="{os.path.join(BIN_DIR, file)}"\n')
     shutil.copy2(bash_profile_temp, bash_profile)
     os.remove(bash_profile_temp)
 
 
-def validate_python_version():
-    version_data = sys.version
-    if int(version_data.split()[0].split(".")[1]) != 9:
-        raise RuntimeError(f"Requires Python v3.9+, found v{version_data.split()[0]}")
+def validate_python_version(tempdir):
+    if not check_python_verison():
+        try:
+            install_python(tempdir)
+        except Exception:
+            try:
+                shutil.rmtree(os.path.join(BIN_DIR, "python"))
+            except FileNotFoundError:
+                pass
+            raise RuntimeError(
+                f"Requires Python v3.9+, found v{sys.version.split()[0]}. Attempt to install new version of Python was unsuccesful"
+            )
+        else:
+            print("Successfully installed Python.")
 
 
 def install(overwrite=False):
     try:
         os.mkdir(BIN_DIR)
     except FileExistsError:
         if overwrite:
@@ -99,18 +109,15 @@
             print("***Installing PharmCAT and all required dependencies***")
             print("Please wait. This can take several minutes...")
 
             print("Installing java...")
             install_java(tempdir)
             print("Successfully installed java.")
 
-            # print("Installing Python...")
-            # install_python(tempdir)
-            # print("Successfully installed Python.")
-            validate_python_version()
+            validate_python_version(tempdir)
 
             print("Installing Preprocessor and PharmCAT pipeline...")
             install_preprocessor(tempdir)
             print("Successfully installed preprocessor and PharmCAT pipeline.")
 
             print("Downloading reference genome...")
             download_reference_genome(tempdir)
```

### Comparing `pharmcat_runner-0.0.6/pharmcat_runner/parser.py` & `pharmcat_runner-0.0.7/pharmcat_runner/parser.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,20 +1,19 @@
-import glob
 import json
 import os
 import re
 import warnings
 from functools import lru_cache
 from io import StringIO
 
 import numpy as np
 import pandas as pd
 
 from .common import *
-from .utils import run_command, validate_file, get_files, blockgz_compress
+from .utils import blockgz_compress, get_files, run_command
 
 GENES_WITH_AS = {"CYP2C9", "DPYD", "CYP2D6"}
 
 
 def get_cpic_dip_to_phen():
     dip_to_phen_data = pd.read_table(DIP_TO_PHEN_PATH, comment="#")
     dip_to_phen_data_raw = dip_to_phen_data.drop(columns="activity_score")
@@ -422,15 +421,15 @@
                 if gene == "CYP4F2":
                     phenotype = assign_cyp4f2_phenotype(genotype)
                 if gene == "CYP2D6":
                     if vcf_dir is None:
                         cyp2d6_cnv = 2
                     else:
                         cyp2d6_file = os.path.join(
-                            os.path.dirname(file), f"No_SULT1A1_{sample_id}.CEL.vcf"
+                            vcf_dir.replace("*", ""), f"No_SULT1A1_{sample_id}.CEL.vcf"
                         )
 
                         cyp2d6_cnv = determine_cyp2d6_cnv(file=cyp2d6_file)
                     if (
                         cyp2d6_cnv not in {0, 1, 2}
                         and genotype != "Indeterminate/Indeterminate"
                     ):
@@ -494,34 +493,53 @@
         if "*" in dir_:
             output_path = os.path.join(os.path.dirname(dir_), fname)
         else:
             output_path = os.path.join(".", fname)
     call_data_pharmcat.to_csv(output_path, index=False)
 
 
+def check_sex_ids(json_files, sex_data):
+    if len(json_files) != sex_data.shape[0]:
+        raise ValueError(
+            f"The number of json files {len(json_files)} does not match the number of samples in the sex ids file {sex_data.shape[0]}"
+        )
+    json_sample_ids = set()
+    for json_file in json_files:
+        sample_id = json_file.split(".")[1]
+        json_sample_ids.add(sample_id)
+
+    sex_ids = set(sex_data[0])
+
+    diff = json_sample_ids.difference(sex_ids)
+    if len(diff) != 0:
+        raise ValueError(f"Found {diff} sample ids in JSONs not in sex_ids file")
+    diff = sex_ids.difference(json_sample_ids)
+    if len(diff) != 0:
+        raise ValueError(
+            f"Found {diff} sample ids in sex_ids with no matching JSON file"
+        )
+
+
 def parse_pharmcat_output(
     pharmcat_dir=None, vcf_dir=None, sex_ids=None, output_dir=None
 ):
     if sex_ids is None:
         warnings.warn(
             "No sex info was provided. Without this, G6PD genotypes and phenotypes can be innacurate."
         )
         xy_ids = None
     else:
-        validate_file(sex_ids)
-        xy_ids = (
-            pd.read_table(sex_ids, header=None)
-            .loc[lambda x: x[1] == "M", [0]]
-            .to_list()
-        )
+        sex_data = pd.read_table(sex_ids, header=None)
     if vcf_dir is None:
         warnings.warn(
             "No VCF directory was provided. Without this, CYP2D6 copy number cannot be determined including *5."
         )
     files = [file for file in get_files(dir_=pharmcat_dir) if ".json" in file]
+    check_sex_ids(json_files=files, sex_data=sex_data)
+
     dip_to_phen, dip_to_activity_score = get_cpic_dip_to_phen()
     dpyd_allele_function = get_allele_function(gene="DPYD")
     cyp2d6_allele_function = get_allele_function(gene="CYP2D6")
     parsed_results = []
     for file in files:
         result = _parse_pharmcat_output(
             file=file,
```

### Comparing `pharmcat_runner-0.0.6/pharmcat_runner/qc_metrics.py` & `pharmcat_runner-0.0.7/pharmcat_runner/qc_metrics.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 import pandas as pd
 
 from .utils import index_file, run_command
 
 
 class QCMetrics:
-    # Order marders in the QC metric operations
+    # Order matters in the QC metric operations
     # Genotype metrics -> variant metrics -> sample metrics
     # Therefore they cannot all be computed at the same time
 
     # Metrics are first computed using PLINK to generate the required metrics files
     # Then the data is filtered using either bcftools or PLINK
     plink_vcf_flags = [
         "--recode",
@@ -21,18 +21,18 @@
         "chrMT",
         "--real-ref-alleles",  # Needed to code the correct allele as reference
     ]
 
     attrs_created = ["sc_file", "hwe_file", "vc_file"]
 
     def __init__(
-        self, file, tempdir, hwe=None, variant_call_rate=None, sample_call_rate=None
+        self, file, dir_, hwe=None, variant_call_rate=None, sample_call_rate=None
     ):
         self.file = file
-        self.tempdir = tempdir
+        self.dir_ = dir_
 
         self.variant_call_rate = variant_call_rate
         self.hwe = hwe
         self.sample_call_rate = sample_call_rate
 
     @staticmethod
     def _parse_metrics_file(file):
@@ -83,67 +83,67 @@
                 "--missing",
                 "--out",
                 output_prefix,
             ]
         )
 
     def _compute_variant_call_rate(self, file_input):
-        output_prefix = os.path.join(self.tempdir, "vcr")
+        output_prefix = os.path.join(self.dir_, "vcr")
         self._compute_base_qc(file=file_input, output_prefix=output_prefix)
         vcr = (
             self._parse_metrics_file(f"{output_prefix}.lmiss")
             .assign(VARIANT_CALL_RATE=lambda x: 1 - x["F_MISS"])
             .drop(columns="F_MISS")
         )
         vcr.to_csv(
-            os.path.join(self.tempdir, "variant_call_rate.tsv"), sep="\t", index=False
+            os.path.join(self.dir_, "variant_call_rate.tsv"), sep="\t", index=False
         )
 
     def _compute_hwe(self, file_input):
-        output_prefix = os.path.join(self.tempdir, "hwe")
+        output_prefix = os.path.join(self.dir_, "hwe")
         self._compute_base_qc(file=file_input, output_prefix=output_prefix)
         hwe = self._parse_metrics_file(f"{output_prefix}.hwe").drop(
             columns=["TEST", "A1", "A2"]
         )
-        hwe.to_csv(os.path.join(self.tempdir, "hwe.tsv"), sep="\t", index=False)
+        hwe.to_csv(os.path.join(self.dir_, "hwe.tsv"), sep="\t", index=False)
 
     def _compute_sample_call_rate(self, file_input):
-        output_prefix = os.path.join(self.tempdir, "scr")
+        output_prefix = os.path.join(self.dir_, "scr")
         self._compute_base_qc(file=file_input, output_prefix=output_prefix)
         scr = (
             self._parse_metrics_file(f"{output_prefix}.imiss")
             .assign(SAMPLE_CALL_RATE=lambda x: 1 - x["F_MISS"])
             .drop(columns="F_MISS")
         )
         scr.to_csv(
-            os.path.join(self.tempdir, "sample_call_rate.tsv"), sep="\t", index=False
+            os.path.join(self.dir_, "sample_call_rate.tsv"), sep="\t", index=False
         )
 
     @index_file
     def filter_on_variant_call_rate(self):
         file_input = self.output_file
         # Compute metrics file
         self._compute_variant_call_rate(file_input=file_input)
 
         # Filter on variant call rate
-        vc_qc_file = os.path.join(self.tempdir, "vc_qced.vcf.gz")
+        vc_qc_file = os.path.join(self.dir_, "vc_qced.vcf.gz")
         run_command(
             f"bcftools view --include 'F_MISSING < {1-self.variant_call_rate}' -Oz -o {vc_qc_file} {self.file}",
             shell=True,
         )
         return vc_qc_file
 
     @index_file
     def filter_on_hwe(self):
         # Computes HWE using mid p-value correction
         file_input = self.output_file
 
         # Compute metrics file
         self._compute_hwe(file_input=file_input)
-        hwe_qc_file = os.path.join(self.tempdir, "hwe_qced")
+        hwe_qc_file = os.path.join(self.dir_, "hwe_qced")
         run_command(
             [
                 "plink",
                 "--vcf",
                 file_input,
                 "--hwe",
                 str(self.hwe),
@@ -156,15 +156,15 @@
         return f"{hwe_qc_file}.vcf.gz"
 
     @index_file
     def filter_on_sample_call_rate(self):
         file_input = self.output_file
         self._compute_sample_call_rate(file_input=file_input)
 
-        sc_qc_file = os.path.join(self.tempdir, "sc_qced")
+        sc_qc_file = os.path.join(self.dir_, "sc_qced")
         run_command(
             [
                 "plink",
                 "--vcf",
                 file_input,
                 "--mind",
                 str(1 - self.sample_call_rate),
```

### Comparing `pharmcat_runner-0.0.6/pharmcat_runner/tests/test_haplotype.py` & `pharmcat_runner-0.0.7/pharmcat_runner/tests/test_haplotype.py`

 * *Files identical despite different names*

### Comparing `pharmcat_runner-0.0.6/pharmcat_runner/tests/test_parser.py` & `pharmcat_runner-0.0.7/pharmcat_runner/tests/test_parser.py`

 * *Files identical despite different names*

### Comparing `pharmcat_runner-0.0.6/pharmcat_runner/utils.py` & `pharmcat_runner-0.0.7/pharmcat_runner/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,23 +3,14 @@
 import shutil
 import subprocess
 import tarfile
 
 from .common import *
 
 
-def index_file(func):
-    def inner(*args, **kwargs):
-        file = func(*args, **kwargs)
-        run_command(["tabix", "-p", "vcf", file])
-        return file
-
-    return inner
-
-
 def blockgz_compress(input_file, output_file):
     run_command(f"bgzip -ck {input_file} > {output_file}", shell=True)
     return output_file
 
 
 def get_files(dir_):
     try:
@@ -112,14 +103,21 @@
         globbing = False
     if not globbing and len(os.listdir(dir_)) == 0:
         raise ValueError(
             f"Provided directory '{dir_}' does not exist or does not contain any files"
         )
 
 
+def check_python_verison():
+    version_data = sys.version
+    if int(version_data.split()[0].split(".")[1]) >= 9:
+        return False
+    return True
+
+
 def validate_plink():
     try:
         run_command(["plink", "-h"])
     except RuntimeError:
         raise RuntimeError(
             "PLINK was not found. Must install PLINK to run sample call rate or Hardy-Weinburg QC steps."
         )
```

### Comparing `pharmcat_runner-0.0.6/pharmcat_runner.egg-info/SOURCES.txt` & `pharmcat_runner-0.0.7/pharmcat_runner.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 pharmcat_runner/__main__.py
 pharmcat_runner/common.py
 pharmcat_runner/haplotype.py
 pharmcat_runner/install.py
 pharmcat_runner/parser.py
 pharmcat_runner/qc_metrics.py
 pharmcat_runner/utils.py
+pharmcat_runner/vcf.py
 pharmcat_runner.egg-info/PKG-INFO
 pharmcat_runner.egg-info/SOURCES.txt
 pharmcat_runner.egg-info/dependency_links.txt
 pharmcat_runner.egg-info/entry_points.txt
 pharmcat_runner.egg-info/requires.txt
 pharmcat_runner.egg-info/top_level.txt
 pharmcat_runner/tests/__init__.py
```

### Comparing `pharmcat_runner-0.0.6/setup.py` & `pharmcat_runner-0.0.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup, find_packages
 
 long_description = open("README.md").read()
 
 setup(
     name="pharmcat_runner",
-    version="0.0.6",
+    version="0.0.7",
     description="Installs, runs, and parsers PharmCAT using Pharmacoscan input.",
     author="Andrew Haddad, PharmD",
     author_email="andrew.haddad@pitt.edu",
     packages=find_packages(),
     long_description=long_description,
     long_description_content_type="text/markdown",
     entry_points={
```

