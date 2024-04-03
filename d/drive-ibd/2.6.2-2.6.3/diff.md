# Comparing `tmp/drive_ibd-2.6.2.tar.gz` & `tmp/drive_ibd-2.6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "drive_ibd-2.6.2.tar", max compression
+gzip compressed data, was "drive_ibd-2.6.3.tar", max compression
```

## Comparing `drive_ibd-2.6.2.tar` & `drive_ibd-2.6.3.tar`

### file list

```diff
@@ -1,40 +1,40 @@
--rw-r--r--   0        0        0    11357 2023-10-09 16:10:09.111536 drive_ibd-2.6.2/LICENSE
--rw-r--r--   0        0        0     1614 2023-12-15 15:41:34.755994 drive_ibd-2.6.2/README.md
--rw-r--r--   0        0        0        0 2023-07-03 15:02:02.235740 drive_ibd-2.6.2/drive/__init__.py
--rwxr-xr-x   0        0        0    12233 2024-03-06 22:07:36.488162 drive_ibd-2.6.2/drive/__main__.py
--rw-r--r--   0        0        0       45 2023-08-03 19:43:34.428381 drive_ibd-2.6.2/drive/cluster/__init__.py
--rw-r--r--   0        0        0    20260 2024-03-06 22:07:36.488162 drive_ibd-2.6.2/drive/cluster/cluster.py
--rw-r--r--   0        0        0      205 2023-08-03 19:43:34.456380 drive_ibd-2.6.2/drive/config.json
--rwxr-xr-x   0        0        0    12387 2024-03-20 14:52:56.694514 drive_ibd-2.6.2/drive/drive.py
--rw-r--r--   0        0        0      129 2023-08-03 19:43:34.456380 drive_ibd-2.6.2/drive/factory/__init__.py
--rw-r--r--   0        0        0     1529 2023-08-03 19:43:34.524379 drive_ibd-2.6.2/drive/factory/factory.py
--rw-r--r--   0        0        0      784 2023-08-03 19:43:34.616376 drive_ibd-2.6.2/drive/factory/loader.py
--rw-r--r--   0        0        0       30 2023-08-03 19:43:34.664375 drive_ibd-2.6.2/drive/filters/__init__.py
--rw-r--r--   0        0        0    18392 2024-03-20 14:52:30.550275 drive_ibd-2.6.2/drive/filters/filter.py
--rw-r--r--   0        0        0       37 2023-04-03 17:12:25.006647 drive_ibd-2.6.2/drive/log/.git
--rw-r--r--   0        0        0       12 2023-04-03 17:12:25.030646 drive_ibd-2.6.2/drive/log/.gitignore
--rw-r--r--   0        0        0     4433 2023-04-03 17:12:25.050646 drive_ibd-2.6.2/drive/log/README.md
--rw-r--r--   0        0        0       33 2023-05-04 22:00:40.780404 drive_ibd-2.6.2/drive/log/__init__.py
--rw-r--r--   0        0        0      225 2023-05-04 22:01:13.999559 drive_ibd-2.6.2/drive/log/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0      303 2023-04-07 13:55:36.577011 drive_ibd-2.6.2/drive/log/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0     7199 2023-11-25 21:04:36.562604 drive_ibd-2.6.2/drive/log/__pycache__/logger.cpython-311.pyc
--rw-r--r--   0        0        0     2730 2023-04-14 16:19:44.018287 drive_ibd-2.6.2/drive/log/__pycache__/logger.cpython-39.pyc
--rw-r--r--   0        0        0     5031 2023-11-25 21:03:38.140112 drive_ibd-2.6.2/drive/log/logger.py
--rw-r--r--   0        0        0      189 2023-12-15 15:59:21.176736 drive_ibd-2.6.2/drive/models/__init__.py
--rw-r--r--   0        0        0      697 2024-03-19 14:02:55.531225 drive_ibd-2.6.2/drive/models/data_container.py
--rw-r--r--   0        0        0     4576 2024-03-06 22:07:36.492162 drive_ibd-2.6.2/drive/models/generate_indices.py
--rw-r--r--   0        0        0     2161 2023-08-03 19:43:34.884370 drive_ibd-2.6.2/drive/models/networks.py
--rw-r--r--   0        0        0      617 2023-08-03 19:43:34.908369 drive_ibd-2.6.2/drive/models/types.py
--rw-r--r--   0        0        0        0 2023-08-03 19:43:34.908369 drive_ibd-2.6.2/drive/plugins/__init__.py
--rw-r--r--   0        0        0     4435 2023-08-28 16:34:24.642658 drive_ibd-2.6.2/drive/plugins/network_writer.py
--rw-r--r--   0        0        0    11804 2024-03-20 14:04:52.564391 drive_ibd-2.6.2/drive/plugins/pvalues.py
--rw-r--r--   0        0        0        3 2024-03-06 22:07:36.516162 drive_ibd-2.6.2/drive/profile.json
--rw-r--r--   0        0        0       39 2023-12-15 15:59:21.224735 drive_ibd-2.6.2/drive/utilities/callbacks/__init__.py
--rw-r--r--   0        0        0     1821 2023-12-15 15:59:21.248734 drive_ibd-2.6.2/drive/utilities/callbacks/callbacks.py
--rw-r--r--   0        0        0     2263 2023-08-03 19:43:35.044366 drive_ibd-2.6.2/drive/utilities/load_phenotypes.py
--rw-r--r--   0        0        0      121 2023-08-03 19:43:35.076365 drive_ibd-2.6.2/drive/utilities/parser/__init__.py
--rw-r--r--   0        0        0     7531 2024-03-20 15:00:20.095218 drive_ibd-2.6.2/drive/utilities/parser/case_file_parser.py
--rw-r--r--   0        0        0      919 2023-08-03 19:43:35.156363 drive_ibd-2.6.2/drive/utilities/parser/phenotype_descriptions_parser.py
--rw-r--r--   0        0        0     2211 2024-03-20 15:03:35.825207 drive_ibd-2.6.2/pyproject.toml
--rw-r--r--   0        0        0     2868 1970-01-01 00:00:00.000000 drive_ibd-2.6.2/setup.py
--rw-r--r--   0        0        0     2828 1970-01-01 00:00:00.000000 drive_ibd-2.6.2/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-10-09 16:10:09.111536 drive_ibd-2.6.3/LICENSE
+-rw-r--r--   0        0        0     1614 2023-12-15 15:41:34.755994 drive_ibd-2.6.3/README.md
+-rw-r--r--   0        0        0        0 2023-07-03 15:02:02.235740 drive_ibd-2.6.3/drive/__init__.py
+-rwxr-xr-x   0        0        0    12233 2024-03-06 22:07:36.488162 drive_ibd-2.6.3/drive/__main__.py
+-rw-r--r--   0        0        0       45 2023-08-03 19:43:34.428381 drive_ibd-2.6.3/drive/cluster/__init__.py
+-rw-r--r--   0        0        0    20260 2024-03-06 22:07:36.488162 drive_ibd-2.6.3/drive/cluster/cluster.py
+-rw-r--r--   0        0        0      205 2023-08-03 19:43:34.456380 drive_ibd-2.6.3/drive/config.json
+-rwxr-xr-x   0        0        0    12405 2024-04-03 20:36:29.343561 drive_ibd-2.6.3/drive/drive.py
+-rw-r--r--   0        0        0      129 2023-08-03 19:43:34.456380 drive_ibd-2.6.3/drive/factory/__init__.py
+-rw-r--r--   0        0        0     1529 2023-08-03 19:43:34.524379 drive_ibd-2.6.3/drive/factory/factory.py
+-rw-r--r--   0        0        0      784 2023-08-03 19:43:34.616376 drive_ibd-2.6.3/drive/factory/loader.py
+-rw-r--r--   0        0        0       30 2023-08-03 19:43:34.664375 drive_ibd-2.6.3/drive/filters/__init__.py
+-rw-r--r--   0        0        0    18392 2024-03-20 14:52:30.550275 drive_ibd-2.6.3/drive/filters/filter.py
+-rw-r--r--   0        0        0       37 2023-04-03 17:12:25.006647 drive_ibd-2.6.3/drive/log/.git
+-rw-r--r--   0        0        0       12 2023-04-03 17:12:25.030646 drive_ibd-2.6.3/drive/log/.gitignore
+-rw-r--r--   0        0        0     4433 2023-04-03 17:12:25.050646 drive_ibd-2.6.3/drive/log/README.md
+-rw-r--r--   0        0        0       33 2023-05-04 22:00:40.780404 drive_ibd-2.6.3/drive/log/__init__.py
+-rw-r--r--   0        0        0      225 2023-05-04 22:01:13.999559 drive_ibd-2.6.3/drive/log/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0      303 2023-04-07 13:55:36.577011 drive_ibd-2.6.3/drive/log/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0     7199 2023-11-25 21:04:36.562604 drive_ibd-2.6.3/drive/log/__pycache__/logger.cpython-311.pyc
+-rw-r--r--   0        0        0     2730 2023-04-14 16:19:44.018287 drive_ibd-2.6.3/drive/log/__pycache__/logger.cpython-39.pyc
+-rw-r--r--   0        0        0     5031 2023-11-25 21:03:38.140112 drive_ibd-2.6.3/drive/log/logger.py
+-rw-r--r--   0        0        0      189 2023-12-15 15:59:21.176736 drive_ibd-2.6.3/drive/models/__init__.py
+-rw-r--r--   0        0        0      697 2024-03-19 14:02:55.531225 drive_ibd-2.6.3/drive/models/data_container.py
+-rw-r--r--   0        0        0     4576 2024-03-06 22:07:36.492162 drive_ibd-2.6.3/drive/models/generate_indices.py
+-rw-r--r--   0        0        0     2161 2023-08-03 19:43:34.884370 drive_ibd-2.6.3/drive/models/networks.py
+-rw-r--r--   0        0        0      617 2023-08-03 19:43:34.908369 drive_ibd-2.6.3/drive/models/types.py
+-rw-r--r--   0        0        0        0 2023-08-03 19:43:34.908369 drive_ibd-2.6.3/drive/plugins/__init__.py
+-rw-r--r--   0        0        0     4435 2023-08-28 16:34:24.642658 drive_ibd-2.6.3/drive/plugins/network_writer.py
+-rw-r--r--   0        0        0    11904 2024-04-03 20:36:18.799715 drive_ibd-2.6.3/drive/plugins/pvalues.py
+-rw-r--r--   0        0        0        3 2024-03-06 22:07:36.516162 drive_ibd-2.6.3/drive/profile.json
+-rw-r--r--   0        0        0       39 2023-12-15 15:59:21.224735 drive_ibd-2.6.3/drive/utilities/callbacks/__init__.py
+-rw-r--r--   0        0        0     1821 2023-12-15 15:59:21.248734 drive_ibd-2.6.3/drive/utilities/callbacks/callbacks.py
+-rw-r--r--   0        0        0     2263 2023-08-03 19:43:35.044366 drive_ibd-2.6.3/drive/utilities/load_phenotypes.py
+-rw-r--r--   0        0        0      121 2023-08-03 19:43:35.076365 drive_ibd-2.6.3/drive/utilities/parser/__init__.py
+-rw-r--r--   0        0        0     7763 2024-04-03 20:36:29.307561 drive_ibd-2.6.3/drive/utilities/parser/case_file_parser.py
+-rw-r--r--   0        0        0      919 2023-08-03 19:43:35.156363 drive_ibd-2.6.3/drive/utilities/parser/phenotype_descriptions_parser.py
+-rw-r--r--   0        0        0     2211 2024-04-03 20:05:55.639813 drive_ibd-2.6.3/pyproject.toml
+-rw-r--r--   0        0        0     2868 1970-01-01 00:00:00.000000 drive_ibd-2.6.3/setup.py
+-rw-r--r--   0        0        0     2828 1970-01-01 00:00:00.000000 drive_ibd-2.6.3/PKG-INFO
```

### Comparing `drive_ibd-2.6.2/LICENSE` & `drive_ibd-2.6.3/LICENSE`

 * *Files identical despite different names*

### Comparing `drive_ibd-2.6.2/README.md` & `drive_ibd-2.6.3/README.md`

 * *Files identical despite different names*

### Comparing `drive_ibd-2.6.2/drive/__main__.py` & `drive_ibd-2.6.3/drive/__main__.py`

 * *Files identical despite different names*

### Comparing `drive_ibd-2.6.2/drive/cluster/cluster.py` & `drive_ibd-2.6.3/drive/cluster/cluster.py`

 * *Files identical despite different names*

### Comparing `drive_ibd-2.6.2/drive/drive.py` & `drive_ibd-2.6.3/drive/drive.py`

 * *Files 0% similar despite different names*

```diff
@@ -254,14 +254,15 @@
 
     parser.add_argument(
         "--version", action="version", version=f"%(prog)s: {version('drive-ibd')}"
     )
 
     args = parser.parse_args()
 
+    print("test")
     # getting the programs start time
     start_time = datetime.now()
 
     # We need to make sure that there is a configuration file
     json_config = args.json_config if args.json_config else find_json_file()
 
     # creating and configuring the logger and then recording user inputs
```

### Comparing `drive_ibd-2.6.2/drive/factory/factory.py` & `drive_ibd-2.6.3/drive/factory/factory.py`

 * *Files identical despite different names*

### Comparing `drive_ibd-2.6.2/drive/factory/loader.py` & `drive_ibd-2.6.3/drive/factory/loader.py`

 * *Files identical despite different names*

### Comparing `drive_ibd-2.6.2/drive/filters/filter.py` & `drive_ibd-2.6.3/drive/filters/filter.py`

 * *Files identical despite different names*

### Comparing `drive_ibd-2.6.2/drive/log/README.md` & `drive_ibd-2.6.3/drive/log/README.md`

 * *Files identical despite different names*

### Comparing `drive_ibd-2.6.2/drive/log/__pycache__/logger.cpython-311.pyc` & `drive_ibd-2.6.3/drive/log/__pycache__/logger.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `drive_ibd-2.6.2/drive/log/__pycache__/logger.cpython-39.pyc` & `drive_ibd-2.6.3/drive/log/__pycache__/logger.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `drive_ibd-2.6.2/drive/log/logger.py` & `drive_ibd-2.6.3/drive/log/logger.py`

 * *Files identical despite different names*

### Comparing `drive_ibd-2.6.2/drive/models/data_container.py` & `drive_ibd-2.6.3/drive/models/data_container.py`

 * *Files identical despite different names*

### Comparing `drive_ibd-2.6.2/drive/models/generate_indices.py` & `drive_ibd-2.6.3/drive/models/generate_indices.py`

 * *Files identical despite different names*

### Comparing `drive_ibd-2.6.2/drive/models/networks.py` & `drive_ibd-2.6.3/drive/models/networks.py`

 * *Files identical despite different names*

### Comparing `drive_ibd-2.6.2/drive/models/types.py` & `drive_ibd-2.6.3/drive/models/types.py`

 * *Files identical despite different names*

### Comparing `drive_ibd-2.6.2/drive/plugins/network_writer.py` & `drive_ibd-2.6.3/drive/plugins/network_writer.py`

 * *Files identical despite different names*

### Comparing `drive_ibd-2.6.2/drive/plugins/pvalues.py` & `drive_ibd-2.6.3/drive/plugins/pvalues.py`

 * *Files 2% similar despite different names*

```diff
@@ -57,38 +57,41 @@
         pvalue = result.pvalue
 
         logger.debug(f"pvalue for {phenotype} = {pvalue}")
 
         return pvalue
 
     @staticmethod
-    def _determine_phenotype_frequency(phenotype_counts: Dict[str, List[str]]) -> float:
+    def _determine_phenotype_frequency(
+        phecode: str, phenotype_counts: Dict[str, List[str]]
+    ) -> float:
         """calculate the phenotype frequency in the cohort
 
         Parameters
         ----------
+        phecode : str
+            phecode id. This value will only be used for a logging statement
+
         phenotype_counts : Dict[str, List[str]]
             Dictionary that has list for individuals who are
             cases, controls, or exclusions.
 
         Returns
         -------
         float
             returns the phenotype frequency as a float
         """
 
         # We need to first check if there are even controls in the file
         phenotype_frequency = len(phenotype_counts.get("cases")) / (
-            len(phenotype_counts.get("controls"))
-            + len(phenotype_counts.get("cases"))
-            + len(phenotype_counts.get("excluded", []))
+            len(phenotype_counts.get("controls")) + len(phenotype_counts.get("cases"))
         )
 
         logger.verbose(
-            f"Identified {len(phenotype_counts.get('cases'))} cases and {len(phenotype_counts.get('controls'))} giving a phenotype frequency of {phenotype_frequency}"  # noqa: E501
+            f"For PheCode, {phecode}, {len(phenotype_counts.get('cases'))} cases and {len(phenotype_counts.get('controls'))} were identified giving a phenotype frequency of {phenotype_frequency}"  # noqa: E501
         )
 
         return phenotype_frequency
 
     @staticmethod
     def _get_carrier_count_in_network(
         phenotype_counts: Dict[str, List[str]], network: Network_Interface
@@ -215,15 +218,15 @@
         for phenotype, phenotype_counts in cohort_carriers.items():
             # if there are no controls then we can't do the
             # stats and should just return a string of N/A for all values
             if len(phenotype_counts.get("controls")) == 0:
                 phenotype_pvalues[phenotype] = "N/A\tN/A\tN/A\tN/A"
             else:
                 phenotype_freq = Pvalues._determine_phenotype_frequency(
-                    phenotype_counts
+                    phenotype, phenotype_counts
                 )
 
                 num_carriers_in_network = Pvalues._get_carrier_count_in_network(
                     phenotype_counts, network
                 )
 
                 carrier_set = Pvalues._get_carriers_in_network(
```

### Comparing `drive_ibd-2.6.2/drive/utilities/callbacks/callbacks.py` & `drive_ibd-2.6.3/drive/utilities/callbacks/callbacks.py`

 * *Files identical despite different names*

### Comparing `drive_ibd-2.6.2/drive/utilities/load_phenotypes.py` & `drive_ibd-2.6.3/drive/utilities/load_phenotypes.py`

 * *Files identical despite different names*

### Comparing `drive_ibd-2.6.2/drive/utilities/parser/case_file_parser.py` & `drive_ibd-2.6.3/drive/utilities/parser/case_file_parser.py`

 * *Files 4% similar despite different names*

```diff
@@ -61,15 +61,15 @@
             phenotype matrix using pd.read_csv
         """
         try:
             pheno_df = pd.read_csv(
                 self.file,
                 sep="\t",
                 na_values=["na", "n/a", "-1", "-1.0", " ", "", "NA", "N/A"],
-            ).fillna("-1")
+            ).fillna(-1)
 
         except pd.errors.ParserError as e:
             logger.critical(e)
             logger.critical(
                 f"Encountered the following error while trying to read in the phenotype matrix: {self.file}"  # noqa: E501
             )
             raise pd.errors.ParserError(
@@ -172,14 +172,17 @@
 
             phenotype_dict[phecode_name] = {
                 "cases": cases,
                 "controls": controls,
                 "excluded": exclusions,
             }
 
+        logger.info(
+            f"For PheCode, {phecode_name}, identified {len(phenotype_dict[phecode_name]['cases'])} cases, {len(phenotype_dict[phecode_name]['controls'])} controls, and {len(phenotype_dict[phecode_name]['excluded'])} exclusions"
+        )  # noqa: E501
         return phenotype_dict, grids.values.tolist()
 
     def parse_cases_and_controls(
         self,
     ) -> Tuple[Dict[str, Dict[str, Set[str]]], Dict[int, str]]:
         """Generate a list for cases, controls, and excluded individuals.
 
@@ -193,10 +196,8 @@
             cohort
         """
 
         cols_to_keep = self._generate_columns_to_keep()
 
         phenotyping_dictionary, cohort_ids = self._process_matrix(cols_to_keep)
 
-        print(phenotyping_dictionary)
-
         return phenotyping_dictionary, cohort_ids
```

### Comparing `drive_ibd-2.6.2/drive/utilities/parser/phenotype_descriptions_parser.py` & `drive_ibd-2.6.3/drive/utilities/parser/phenotype_descriptions_parser.py`

 * *Files identical despite different names*

### Comparing `drive_ibd-2.6.2/pyproject.toml` & `drive_ibd-2.6.3/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 name = "drive-ibd"
 
-version = "2.6.2"
+version = "2.6.3"
 description = "cli tool to identify networks of individuals who share IBD segments overlapping loci of interest"
 authors = ["James Baker <james.baker@vanderbilt.edu>", "Hung-Hsin Chen <hung-hsin.chen.1@vumc.org>", "Jennifer E. Below <jennifer.e.below@vumc.org>"]
 maintainers = ["James Baker <james.baker@vanderbilt.edu>", "Hung-Hsin Chen <hung-hsin.chen.1@vumc.org>"]
 repository = "https://github.com/belowlab/drive"
 homepage = "https://drive-ibd.readthedocs.io/en/latest/"
 readme = "README.md"
 keywords = ["python", "genetics", "identity by descent", "relatedness"]
```

### Comparing `drive_ibd-2.6.2/setup.py` & `drive_ibd-2.6.3/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -24,15 +24,15 @@
  'scipy>=1.10.1,<2.0.0']
 
 entry_points = \
 {'console_scripts': ['drive = drive.drive:main']}
 
 setup_kwargs = {
     'name': 'drive-ibd',
-    'version': '2.6.2',
+    'version': '2.6.3',
     'description': 'cli tool to identify networks of individuals who share IBD segments overlapping loci of interest',
     'long_description': '[![Documentation Status](https://readthedocs.org/projects/drive-ibd/badge/?version=latest)](https://drive-ibd.readthedocs.io/en/latest/?badge=latest)\n[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)\n[![PyPI version](https://badge.fury.io/py/drive-ibd.svg)](https://badge.fury.io/py/drive-ibd)\n\n# DRIVE:\n\nThis repository contains the source code for the tool DRIVE (Distant Relatedness for Identification and Variant Evaluation) is a novel approach to IBD-based genotype inference used to identify shared chromosomal segments in dense genetic arrays. DRIVE implements a random walk algorithm that identifies clusters of individuals who pairwise share an IBD segment overlapping a locus of interest. This tool was developed in python by the Below Lab at Vanderbilt University. The documentation for how to use this tool can be found here [DRIVE documentation](https://drive-ibd.readthedocs.io/en/latest/)\n\n## Installing DRIVE:\nDRIVE is available on PYPI and can easily be installed using the following command:\n\n```bash\npip install drive-ibd\n```\nIt is recommended to install DRIVE within a virtual environment such as venv, or conda. More information about this process can be found within the documentation.\n\nIf the user wishes to develop DRIVE or install the program from source then they can clone the repository. This process is described under the section called "Github Installation" in the documentation.\n\n### Reporting issues:\nIf you wish to report a bug or propose a feature you can find templates under the .github/ISSUE_TEMPLATE directory.\n\n',
     'author': 'James Baker',
     'author_email': 'james.baker@vanderbilt.edu',
     'maintainer': 'James Baker',
     'maintainer_email': 'james.baker@vanderbilt.edu',
     'url': 'https://drive-ibd.readthedocs.io/en/latest/',
```

### Comparing `drive_ibd-2.6.2/PKG-INFO` & `drive_ibd-2.6.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: drive-ibd
-Version: 2.6.2
+Version: 2.6.3
 Summary: cli tool to identify networks of individuals who share IBD segments overlapping loci of interest
 Home-page: https://drive-ibd.readthedocs.io/en/latest/
 Keywords: python,genetics,identity by descent,relatedness
 Author: James Baker
 Author-email: james.baker@vanderbilt.edu
 Maintainer: James Baker
 Maintainer-email: james.baker@vanderbilt.edu
```

