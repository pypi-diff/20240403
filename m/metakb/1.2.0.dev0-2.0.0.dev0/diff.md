# Comparing `tmp/metakb-1.2.0.dev0.tar.gz` & `tmp/metakb-2.0.0.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "metakb-1.2.0.dev0.tar", last modified: Fri May 12 17:55:44 2023, max compression
+gzip compressed data, was "metakb-2.0.0.dev0.tar", last modified: Wed Apr  3 14:37:24 2024, max compression
```

## Comparing `metakb-1.2.0.dev0.tar` & `metakb-2.0.0.dev0.tar`

### file list

```diff
@@ -1,36 +1,38 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 17:55:44.705232 metakb-1.2.0.dev0/
--rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-05-12 17:55:35.000000 metakb-1.2.0.dev0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    10533 2023-05-12 17:55:44.705232 metakb-1.2.0.dev0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     9698 2023-05-12 17:55:35.000000 metakb-1.2.0.dev0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 17:55:44.701232 metakb-1.2.0.dev0/metakb/
--rw-r--r--   0 runner    (1001) docker     (123)     1470 2023-05-12 17:55:35.000000 metakb-1.2.0.dev0/metakb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16703 2023-05-12 17:55:35.000000 metakb-1.2.0.dev0/metakb/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)    22378 2023-05-12 17:55:35.000000 metakb-1.2.0.dev0/metakb/database.py
--rw-r--r--   0 runner    (1001) docker     (123)     5690 2023-05-12 17:55:35.000000 metakb-1.2.0.dev0/metakb/delta.py
--rw-r--r--   0 runner    (1001) docker     (123)      124 2023-05-12 17:55:35.000000 metakb-1.2.0.dev0/metakb/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 17:55:44.701232 metakb-1.2.0.dev0/metakb/harvesters/
--rw-r--r--   0 runner    (1001) docker     (123)      175 2023-05-12 17:55:35.000000 metakb-1.2.0.dev0/metakb/harvesters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1934 2023-05-12 17:55:35.000000 metakb-1.2.0.dev0/metakb/harvesters/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     5034 2023-05-12 17:55:35.000000 metakb-1.2.0.dev0/metakb/harvesters/civic.py
--rw-r--r--   0 runner    (1001) docker     (123)    10059 2023-05-12 17:55:35.000000 metakb-1.2.0.dev0/metakb/harvesters/moa.py
--rw-r--r--   0 runner    (1001) docker     (123)     7326 2023-05-12 17:55:35.000000 metakb-1.2.0.dev0/metakb/harvesters/oncokb.py
--rw-r--r--   0 runner    (1001) docker     (123)     4546 2023-05-12 17:55:35.000000 metakb-1.2.0.dev0/metakb/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     8810 2023-05-12 17:55:35.000000 metakb-1.2.0.dev0/metakb/normalizers.py
--rw-r--r--   0 runner    (1001) docker     (123)    55043 2023-05-12 17:55:35.000000 metakb-1.2.0.dev0/metakb/query.py
--rw-r--r--   0 runner    (1001) docker     (123)    41922 2023-05-12 17:55:35.000000 metakb-1.2.0.dev0/metakb/schemas.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 17:55:44.705232 metakb-1.2.0.dev0/metakb/transform/
--rw-r--r--   0 runner    (1001) docker     (123)      219 2023-05-12 17:55:35.000000 metakb-1.2.0.dev0/metakb/transform/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8903 2023-05-12 17:55:35.000000 metakb-1.2.0.dev0/metakb/transform/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    32381 2023-05-12 17:55:35.000000 metakb-1.2.0.dev0/metakb/transform/civic.py
--rw-r--r--   0 runner    (1001) docker     (123)    16923 2023-05-12 17:55:35.000000 metakb-1.2.0.dev0/metakb/transform/moa.py
--rw-r--r--   0 runner    (1001) docker     (123)    20954 2023-05-12 17:55:35.000000 metakb-1.2.0.dev0/metakb/transform/oncokb.py
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-05-12 17:55:35.000000 metakb-1.2.0.dev0/metakb/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 17:55:44.701232 metakb-1.2.0.dev0/metakb.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    10533 2023-05-12 17:55:44.000000 metakb-1.2.0.dev0/metakb.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      659 2023-05-12 17:55:44.000000 metakb-1.2.0.dev0/metakb.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-12 17:55:44.000000 metakb-1.2.0.dev0/metakb.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-12 17:55:44.000000 metakb-1.2.0.dev0/metakb.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      365 2023-05-12 17:55:44.000000 metakb-1.2.0.dev0/metakb.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-12 17:55:44.000000 metakb-1.2.0.dev0/metakb.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1451 2023-05-12 17:55:44.705232 metakb-1.2.0.dev0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      153 2023-05-12 17:55:35.000000 metakb-1.2.0.dev0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 14:37:24.169038 metakb-2.0.0.dev0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1061 2024-04-03 14:37:20.000000 metakb-2.0.0.dev0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    11960 2024-04-03 14:37:24.169038 metakb-2.0.0.dev0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     8553 2024-04-03 14:37:20.000000 metakb-2.0.0.dev0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     5134 2024-04-03 14:37:20.000000 metakb-2.0.0.dev0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-03 14:37:24.169038 metakb-2.0.0.dev0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 14:37:24.165038 metakb-2.0.0.dev0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 14:37:24.165038 metakb-2.0.0.dev0/src/metakb/
+-rw-r--r--   0 runner    (1001) docker     (127)     1382 2024-04-03 14:37:20.000000 metakb-2.0.0.dev0/src/metakb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12392 2024-04-03 14:37:20.000000 metakb-2.0.0.dev0/src/metakb/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22594 2024-04-03 14:37:20.000000 metakb-2.0.0.dev0/src/metakb/database.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 14:37:24.169038 metakb-2.0.0.dev0/src/metakb/harvesters/
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-03 14:37:20.000000 metakb-2.0.0.dev0/src/metakb/harvesters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1925 2024-04-03 14:37:20.000000 metakb-2.0.0.dev0/src/metakb/harvesters/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5045 2024-04-03 14:37:20.000000 metakb-2.0.0.dev0/src/metakb/harvesters/civic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9560 2024-04-03 14:37:20.000000 metakb-2.0.0.dev0/src/metakb/harvesters/moa.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3039 2024-04-03 14:37:20.000000 metakb-2.0.0.dev0/src/metakb/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8584 2024-04-03 14:37:20.000000 metakb-2.0.0.dev0/src/metakb/normalizers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26027 2024-04-03 14:37:20.000000 metakb-2.0.0.dev0/src/metakb/query.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 14:37:24.169038 metakb-2.0.0.dev0/src/metakb/schemas/
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-04-03 14:37:20.000000 metakb-2.0.0.dev0/src/metakb/schemas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5989 2024-04-03 14:37:20.000000 metakb-2.0.0.dev0/src/metakb/schemas/annotation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1352 2024-04-03 14:37:20.000000 metakb-2.0.0.dev0/src/metakb/schemas/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)      189 2024-04-03 14:37:20.000000 metakb-2.0.0.dev0/src/metakb/schemas/app.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7026 2024-04-03 14:37:20.000000 metakb-2.0.0.dev0/src/metakb/schemas/categorical_variation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6472 2024-04-03 14:37:20.000000 metakb-2.0.0.dev0/src/metakb/schemas/variation_statement.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 14:37:24.169038 metakb-2.0.0.dev0/src/metakb/transform/
+-rw-r--r--   0 runner    (1001) docker     (127)      127 2024-04-03 14:37:20.000000 metakb-2.0.0.dev0/src/metakb/transform/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19542 2024-04-03 14:37:20.000000 metakb-2.0.0.dev0/src/metakb/transform/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34126 2024-04-03 14:37:20.000000 metakb-2.0.0.dev0/src/metakb/transform/civic.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22687 2024-04-03 14:37:20.000000 metakb-2.0.0.dev0/src/metakb/transform/moa.py
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-03 14:37:20.000000 metakb-2.0.0.dev0/src/metakb/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 14:37:24.169038 metakb-2.0.0.dev0/src/metakb.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    11960 2024-04-03 14:37:24.000000 metakb-2.0.0.dev0/src/metakb.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      798 2024-04-03 14:37:24.000000 metakb-2.0.0.dev0/src/metakb.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 14:37:24.000000 metakb-2.0.0.dev0/src/metakb.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      359 2024-04-03 14:37:24.000000 metakb-2.0.0.dev0/src/metakb.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-03 14:37:24.000000 metakb-2.0.0.dev0/src/metakb.egg-info/top_level.txt
```

### Comparing `metakb-1.2.0.dev0/LICENSE` & `metakb-2.0.0.dev0/LICENSE`

 * *Files identical despite different names*

### Comparing `metakb-1.2.0.dev0/PKG-INFO` & `metakb-2.0.0.dev0/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,29 +1,7 @@
-Metadata-Version: 2.1
-Name: metakb
-Version: 1.2.0.dev0
-Summary: A search interface for cancer variant interpretations assembled by aggregating and harmonizing across multiple cancer variant interpretation knowledgebases.
-Home-page: https://github.com/cancervariants/metakb
-Author: VICC
-Author-email: help@cancervariants.org
-License: MIT
-Platform: UNKNOWN
-Classifier: Development Status :: 3 - Alpha
-Classifier: Intended Audience :: Science/Research
-Classifier: Intended Audience :: Developers
-Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-Provides-Extra: dev
-Provides-Extra: tests
-License-File: LICENSE
-
 [![Documentation Status](https://readthedocs.org/projects/vicc-metakb/badge/?version=latest)](https://vicc-metakb.readthedocs.io/en/latest/?badge=latest) [![Build Status](https://travis-ci.org/cancervariants/metakb.svg?branch=main)](https://travis-ci.org/cancervariants/metakb) [![Coverage Status](https://coveralls.io/repos/github/cancervariants/metakb/badge.svg?branch=main)](https://coveralls.io/github/cancervariants/metakb?branch=main)
 
 # metakb
 
 The intent of the project is to leverage the collective knowledge of the disparate existing resources of the VICC to improve the comprehensiveness of clinical interpretation of genomic variation. An ongoing goal will be to provide and improve upon standards and guidelines by which other groups with clinical interpretation data may make it accessible and visible to the public. We have released a preprint discussing our initial harmonization effort and observed disparities in the structure and content of variant interpretations.
 
 ## Getting Started
@@ -63,15 +41,15 @@
 
 ### Setting up Neo4j
 
 The MetaKB uses [Neo4j](https://neo4j.com/) for its database backend. To run a local MetaKB instance, you'll need to run a Neo4j database instance as well. The easiest way to do this is from Neo4j Desktop.
 
 First, follow the [desktop setup instructions](https://neo4j.com/developer/neo4j-desktop) to download, install, and open Neo4j Desktop for the first time.
 
-Once you have opened Neo4j desktop, use the "New" button in the upper-left region of the window to create a new project. Within that project, click the "Add" button in the upper-right region of the window and select "Local DBMS". The name of the DBMS doesn't matter, but the password will be used later to connect the database to MetaKB (we have been using "admin" by default). Click "Create". Then, click the row within the project screen corresponding to your newly-created DBMS, and click the green "Start" button to start the database service.
+Once you have opened Neo4j desktop, use the `New` button in the upper-left region of the window to create a new project. Within that project, click the `Add` button in the upper-right region of the window and select `Local DBMS`. The name of the DBMS doesn't matter, but the password will be used later to connect the database to MetaKB (we have been using `password` by default). Select version `5.14.0` (other versions have not been tested). Click `Create`. Then, click the row within the project screen corresponding to your newly-created DBMS, and click the green `Start` button to start the database service.
 
 The graph will initially be empty, but once you have successfully loaded data, Neo4j Desktop provides an interface for exploring and visualizing relationships within the graph. To access it, click the blue "Open" button. The prompt at the top of this window processes [Cypher queries](https://neo4j.com/docs/cypher-refcard/current/); to start, try `MATCH (n:Statement {id:"civic.eid:1409"}) RETURN n`. Buttons on the left-hand edge of the results pane let you select graph, tabular, or textual output.
 
 
 ### Setting up normalizers
 
 The MetaKB calls a number of normalizer libraries to transform resource data and resolve incoming search queries. These will be installed as part of the package requirements, but require additional setup.
@@ -90,17 +68,15 @@
 
 Next, initialize the [Variation Normalizer](https://github.com/cancervariants/variation-normalization) by following the instructions in the [README](https://github.com/cancervariants/variation-normalization#installation). When setting up the UTA database, [these](https://github.com/ga4gh/vrs-python/tree/main/docs/setup_help) docs may be helpful.
 
 
 The MetaKB can acquire all other needed normalizer data, except for that of [OMIM](https://www.omim.org/downloads), which must be manually placed:
 
 ```sh
-cd disease/  # starting from the site-packages dir of your virtual environment's Python instance
-mkdir -p data/omim
-cp ~/YOUR/PATH/TO/mimTitles.txt data/omim/omim_<date>.tsv  # replace <date> with date of data acquisition formatted as YYYYMMDD
+cp ~/YOUR/PATH/TO/mimTitles.txt ~/.local/share/wags_tails/omim/omim_<date>.tsv  # replace <date> with date of data acquisition formatted as YYYYMMDD
 ```
 
 ### Environment Variables
 
 MetaKB relies on environment variables to set in order to work.
 
 * Always Required:
@@ -111,63 +87,35 @@
 
     Example:
 
     ```shell script
     export UTA_DB_URL=postgresql://uta_admin:password@localhost:5432/uta/uta_20210129
     ```
 
-  * `ONCOKB_API_TOKEN`
-    * Required to harvest OncoKB data. If you do not set this environment variable, you can set during the initialization of the OncoKBHarvester.
-    * Used to access OncoKB data via their REST API. See [here](https://www.oncokb.org/apiAccess) for more information on how to register an account and get an OncoKB API token.
-
-    Example for setting environment variable:
-    ```shell script
-    export ONCOKB_API_TOKEN={api_token}
-    ```
-
-    Example for setting during OncoKB Harvester initialization:
-    ```python
-    OncoKBHarvester(api_token={api_token})
-    ```
-
 * Required when using the `--load_normalizers_db` or `--force_load_normalizers_db` arguments in CLI commands
-  * `RXNORM_API_KEY`
+  * `UMLS_API_KEY`
     * Used in Therapy Normalizer to retrieve RxNorm data
-    * RxNorm requires a UMLS license, which you can register for one [here](https://www.nlm.nih.gov/research/umls/index.html). You must set the `RxNORM_API_KEY` environment variable to your API key. This can be found in the [UTS 'My Profile' area](https://uts.nlm.nih.gov/uts/profile) after singing in.
+    * RxNorm requires a UMLS license, which you can register for one [here](https://www.nlm.nih.gov/research/umls/index.html). You must set the `UMLS_API_KEY` environment variable to your API key. This can be found in the [UTS 'My Profile' area](https://uts.nlm.nih.gov/uts/profile) after singing in.
 
     Example:
 
     ```shell script
-    export RXNORM_API_KEY={rxnorm_api_key}
+    export UMLS_API_KEY={rxnorm_api_key}
     ```
 
-  * `DATAVERSE_API_KEY`
+  * `HARVARD_DATAVERSE_API_KEY`
     * Used in Therapy Normalizer to retrieve HemOnc data
-    * HemOnc.org data requires a Harvard Dataverse API key. After creating a user account on the Harvard Dataverse website, you can follow [these instructions](https://guides.dataverse.org/en/latest/user/account.html) to generate a key. You will create or login to your account at [this](https://dataverse.harvard.edu/) site. You must set the `DATAVERSE_API_KEY` environment variable to your API key.
+    * HemOnc.org data requires a Harvard Dataverse API key. After creating a user account on the Harvard Dataverse website, you can follow [these instructions](https://guides.dataverse.org/en/latest/user/account.html) to generate a key. You will create or login to your account at [this](https://dataverse.harvard.edu/) site. You must set the `HARVARD_DATAVERSE_API_KEY` environment variable to your API key.
 
     Example:
 
     ```shell script
-    export DATAVERSE_API_KEY={dataverse_api_key}
+    export HARVARD_DATAVERSE_API_KEY={dataverse_api_key}
     ```
 
-### Data files
-
-Some sources in MetaKB require user provided files to harvest data.
-
-* OncoKB
-  * In addition to setting the `ONCOKB_API_TOKEN` environment variable to harvest OncoKB data, you also need to provide a CSV file containing a header row with `hugo_symbol` and `protein_change`, associated rows containing protein variants you wish to harvest, and using a comma as the delimiter. The file will look something like:
-
-    ```csv
-    hugo_symbol,protein_change
-    BRAF,V600E
-    ...
-    ```
-  * This file will harvest OncoKB evidence based on the variants provided.
-
 ### Loading data
 
 Once Neo4j and DynamoDB instances are both running, and necessary normalizer data has been placed, run the MetaKB CLI with the `--initialize_normalizers` flag to acquire all other necessary normalizer source data, and execute harvest, transform, and load operations into the graph datastore.
 
 In the MetaKB project root, run the following:
 
 ```sh
@@ -198,18 +146,18 @@
 ```sh
 python3 -m pytest
 ```
 
 
 ### And coding style tests
 
-Code style is managed by [flake8](https://github.com/PyCQA/flake8) and checked prior to commit.
+Code style is managed by [ruff](https://astral.sh/ruff) and checked prior to commit.
 
 ```
-see .flake8
+python3 -m ruff check --fix . && python3 -m ruff format .
 
 ```
 
 ## Contributing
 
 Please read [CONTRIBUTING.md](CONTRIBUTING.md) for details on our code of conduct, and the process for submitting pull requests to us.
 
@@ -233,9 +181,7 @@
 ## Versioning
 
 We use [SemVer](http://semver.org/) for versioning. For the versions available, see the [tags on this repository](https://github.com/cancervariants/metakb/tags).
 
 ## License
 
 This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details
-
-
```

### Comparing `metakb-1.2.0.dev0/README.md` & `metakb-2.0.0.dev0/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,7 +1,80 @@
+Metadata-Version: 2.1
+Name: metakb
+Version: 2.0.0.dev0
+Summary: A search interface for cancer variant interpretations assembled by aggregating and harmonizing across multiple cancer variant interpretation knowledgebases.
+Author: Alex H Wagner, Kori Kuzma, James Stevenson, Brian Walsh, Jeff Liu
+License: MIT License
+        
+        Copyright (c) 2018 VICC
+        
+        Permission is hereby granted, free of charge, to any person obtaining a copy
+        of this software and associated documentation files (the "Software"), to deal
+        in the Software without restriction, including without limitation the rights
+        to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+        copies of the Software, and to permit persons to whom the Software is
+        furnished to do so, subject to the following conditions:
+        
+        The above copyright notice and this permission notice shall be included in all
+        copies or substantial portions of the Software.
+        
+        THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+        IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+        FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+        AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+        LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+        OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+        SOFTWARE.
+        
+Project-URL: Homepage, https://github.com/cancervariants/metakb
+Project-URL: Documentation, https://github.com/cancervariants/metakb
+Project-URL: Changelog, https://github.com/cancervariants/metakb/releases
+Project-URL: Source, https://github.com/cancervariants/metakb
+Project-URL: Bug Tracker, https://github.com/cancervariants/metakb/issues
+Classifier: Development Status :: 3 - Alpha
+Classifier: Intended Audience :: Science/Research
+Classifier: Intended Audience :: Developers
+Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: ga4gh.vrs~=2.0.0a5
+Requires-Dist: gene-normalizer[etl]~=0.3.0-dev1
+Requires-Dist: variation-normalizer~=0.8.2
+Requires-Dist: disease-normalizer[etl]~=0.4.0.dev3
+Requires-Dist: thera-py[etl]~=0.5.0.dev3
+Requires-Dist: civicpy~=3.0.0
+Requires-Dist: requests
+Requires-Dist: pydantic==2.*
+Requires-Dist: requests-cache
+Requires-Dist: neo4j==5.*
+Requires-Dist: uvicorn
+Requires-Dist: fastapi
+Requires-Dist: boto3
+Requires-Dist: botocore
+Requires-Dist: asyncclick
+Provides-Extra: tests
+Requires-Dist: pytest; extra == "tests"
+Requires-Dist: pytest-cov; extra == "tests"
+Requires-Dist: mock; extra == "tests"
+Requires-Dist: pytest-asyncio; extra == "tests"
+Provides-Extra: dev
+Requires-Dist: pre-commit; extra == "dev"
+Requires-Dist: ruff==0.2.0; extra == "dev"
+Provides-Extra: notebooks
+Requires-Dist: ipykernel; extra == "notebooks"
+Requires-Dist: jupyterlab; extra == "notebooks"
+
 [![Documentation Status](https://readthedocs.org/projects/vicc-metakb/badge/?version=latest)](https://vicc-metakb.readthedocs.io/en/latest/?badge=latest) [![Build Status](https://travis-ci.org/cancervariants/metakb.svg?branch=main)](https://travis-ci.org/cancervariants/metakb) [![Coverage Status](https://coveralls.io/repos/github/cancervariants/metakb/badge.svg?branch=main)](https://coveralls.io/github/cancervariants/metakb?branch=main)
 
 # metakb
 
 The intent of the project is to leverage the collective knowledge of the disparate existing resources of the VICC to improve the comprehensiveness of clinical interpretation of genomic variation. An ongoing goal will be to provide and improve upon standards and guidelines by which other groups with clinical interpretation data may make it accessible and visible to the public. We have released a preprint discussing our initial harmonization effort and observed disparities in the structure and content of variant interpretations.
 
 ## Getting Started
@@ -41,15 +114,15 @@
 
 ### Setting up Neo4j
 
 The MetaKB uses [Neo4j](https://neo4j.com/) for its database backend. To run a local MetaKB instance, you'll need to run a Neo4j database instance as well. The easiest way to do this is from Neo4j Desktop.
 
 First, follow the [desktop setup instructions](https://neo4j.com/developer/neo4j-desktop) to download, install, and open Neo4j Desktop for the first time.
 
-Once you have opened Neo4j desktop, use the "New" button in the upper-left region of the window to create a new project. Within that project, click the "Add" button in the upper-right region of the window and select "Local DBMS". The name of the DBMS doesn't matter, but the password will be used later to connect the database to MetaKB (we have been using "admin" by default). Click "Create". Then, click the row within the project screen corresponding to your newly-created DBMS, and click the green "Start" button to start the database service.
+Once you have opened Neo4j desktop, use the `New` button in the upper-left region of the window to create a new project. Within that project, click the `Add` button in the upper-right region of the window and select `Local DBMS`. The name of the DBMS doesn't matter, but the password will be used later to connect the database to MetaKB (we have been using `password` by default). Select version `5.14.0` (other versions have not been tested). Click `Create`. Then, click the row within the project screen corresponding to your newly-created DBMS, and click the green `Start` button to start the database service.
 
 The graph will initially be empty, but once you have successfully loaded data, Neo4j Desktop provides an interface for exploring and visualizing relationships within the graph. To access it, click the blue "Open" button. The prompt at the top of this window processes [Cypher queries](https://neo4j.com/docs/cypher-refcard/current/); to start, try `MATCH (n:Statement {id:"civic.eid:1409"}) RETURN n`. Buttons on the left-hand edge of the results pane let you select graph, tabular, or textual output.
 
 
 ### Setting up normalizers
 
 The MetaKB calls a number of normalizer libraries to transform resource data and resolve incoming search queries. These will be installed as part of the package requirements, but require additional setup.
@@ -68,17 +141,15 @@
 
 Next, initialize the [Variation Normalizer](https://github.com/cancervariants/variation-normalization) by following the instructions in the [README](https://github.com/cancervariants/variation-normalization#installation). When setting up the UTA database, [these](https://github.com/ga4gh/vrs-python/tree/main/docs/setup_help) docs may be helpful.
 
 
 The MetaKB can acquire all other needed normalizer data, except for that of [OMIM](https://www.omim.org/downloads), which must be manually placed:
 
 ```sh
-cd disease/  # starting from the site-packages dir of your virtual environment's Python instance
-mkdir -p data/omim
-cp ~/YOUR/PATH/TO/mimTitles.txt data/omim/omim_<date>.tsv  # replace <date> with date of data acquisition formatted as YYYYMMDD
+cp ~/YOUR/PATH/TO/mimTitles.txt ~/.local/share/wags_tails/omim/omim_<date>.tsv  # replace <date> with date of data acquisition formatted as YYYYMMDD
 ```
 
 ### Environment Variables
 
 MetaKB relies on environment variables to set in order to work.
 
 * Always Required:
@@ -89,62 +160,34 @@
 
     Example:
 
     ```shell script
     export UTA_DB_URL=postgresql://uta_admin:password@localhost:5432/uta/uta_20210129
     ```
 
-  * `ONCOKB_API_TOKEN`
-    * Required to harvest OncoKB data. If you do not set this environment variable, you can set during the initialization of the OncoKBHarvester.
-    * Used to access OncoKB data via their REST API. See [here](https://www.oncokb.org/apiAccess) for more information on how to register an account and get an OncoKB API token.
-
-    Example for setting environment variable:
-    ```shell script
-    export ONCOKB_API_TOKEN={api_token}
-    ```
-
-    Example for setting during OncoKB Harvester initialization:
-    ```python
-    OncoKBHarvester(api_token={api_token})
-    ```
-
 * Required when using the `--load_normalizers_db` or `--force_load_normalizers_db` arguments in CLI commands
-  * `RXNORM_API_KEY`
+  * `UMLS_API_KEY`
     * Used in Therapy Normalizer to retrieve RxNorm data
-    * RxNorm requires a UMLS license, which you can register for one [here](https://www.nlm.nih.gov/research/umls/index.html). You must set the `RxNORM_API_KEY` environment variable to your API key. This can be found in the [UTS 'My Profile' area](https://uts.nlm.nih.gov/uts/profile) after singing in.
+    * RxNorm requires a UMLS license, which you can register for one [here](https://www.nlm.nih.gov/research/umls/index.html). You must set the `UMLS_API_KEY` environment variable to your API key. This can be found in the [UTS 'My Profile' area](https://uts.nlm.nih.gov/uts/profile) after singing in.
 
     Example:
 
     ```shell script
-    export RXNORM_API_KEY={rxnorm_api_key}
+    export UMLS_API_KEY={rxnorm_api_key}
     ```
 
-  * `DATAVERSE_API_KEY`
+  * `HARVARD_DATAVERSE_API_KEY`
     * Used in Therapy Normalizer to retrieve HemOnc data
-    * HemOnc.org data requires a Harvard Dataverse API key. After creating a user account on the Harvard Dataverse website, you can follow [these instructions](https://guides.dataverse.org/en/latest/user/account.html) to generate a key. You will create or login to your account at [this](https://dataverse.harvard.edu/) site. You must set the `DATAVERSE_API_KEY` environment variable to your API key.
+    * HemOnc.org data requires a Harvard Dataverse API key. After creating a user account on the Harvard Dataverse website, you can follow [these instructions](https://guides.dataverse.org/en/latest/user/account.html) to generate a key. You will create or login to your account at [this](https://dataverse.harvard.edu/) site. You must set the `HARVARD_DATAVERSE_API_KEY` environment variable to your API key.
 
     Example:
 
     ```shell script
-    export DATAVERSE_API_KEY={dataverse_api_key}
-    ```
-
-### Data files
-
-Some sources in MetaKB require user provided files to harvest data.
-
-* OncoKB
-  * In addition to setting the `ONCOKB_API_TOKEN` environment variable to harvest OncoKB data, you also need to provide a CSV file containing a header row with `hugo_symbol` and `protein_change`, associated rows containing protein variants you wish to harvest, and using a comma as the delimiter. The file will look something like:
-
-    ```csv
-    hugo_symbol,protein_change
-    BRAF,V600E
-    ...
+    export HARVARD_DATAVERSE_API_KEY={dataverse_api_key}
     ```
-  * This file will harvest OncoKB evidence based on the variants provided.
 
 ### Loading data
 
 Once Neo4j and DynamoDB instances are both running, and necessary normalizer data has been placed, run the MetaKB CLI with the `--initialize_normalizers` flag to acquire all other necessary normalizer source data, and execute harvest, transform, and load operations into the graph datastore.
 
 In the MetaKB project root, run the following:
 
@@ -176,18 +219,18 @@
 ```sh
 python3 -m pytest
 ```
 
 
 ### And coding style tests
 
-Code style is managed by [flake8](https://github.com/PyCQA/flake8) and checked prior to commit.
+Code style is managed by [ruff](https://astral.sh/ruff) and checked prior to commit.
 
 ```
-see .flake8
+python3 -m ruff check --fix . && python3 -m ruff format .
 
 ```
 
 ## Contributing
 
 Please read [CONTRIBUTING.md](CONTRIBUTING.md) for details on our code of conduct, and the process for submitting pull requests to us.
```

### Comparing `metakb-1.2.0.dev0/metakb/__init__.py` & `metakb-2.0.0.dev0/src/metakb/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,40 +1,35 @@
 """The MetaKB package."""
-from pathlib import Path
 import logging
 from os import environ
+from pathlib import Path
 
 APP_ROOT = Path(__file__).resolve().parents[0]
-PROJECT_ROOT = Path(__file__).resolve().parents[1]
-
-if 'METAKB_NORM_EB_PROD' in environ:
-    LOG_FN = "/tmp/metakb.log"
-else:
-    LOG_FN = "metakb.log"
+LOG_FN = "/tmp/metakb.log" if "METAKB_NORM_EB_PROD" in environ else "metakb.log"  # noqa: S108
 
 logging.basicConfig(
-    filename=LOG_FN,
-    format='[%(asctime)s] - %(name)s - %(levelname)s : %(message)s')
-logger = logging.getLogger('metakb')
+    filename=LOG_FN, format="[%(asctime)s] - %(name)s - %(levelname)s : %(message)s"
+)
+logger = logging.getLogger("metakb")
 logger.setLevel(logging.DEBUG)
 logging.getLogger("boto3").setLevel(logging.INFO)
 logging.getLogger("botocore").setLevel(logging.INFO)
 logging.getLogger("urllib3").setLevel(logging.INFO)
 logging.getLogger("python_jsonschema_objects").setLevel(logging.INFO)
 logging.getLogger("hgvs.parser").setLevel(logging.INFO)
-logging.getLogger("biocommons.seqrepo.seqaliasdb.seqaliasdb").setLevel(logging.INFO)  # noqa: E501
-logging.getLogger("biocommons.seqrepo.fastadir.fastadir").setLevel(logging.INFO)  # noqa: E501
+logging.getLogger("biocommons.seqrepo.seqaliasdb.seqaliasdb").setLevel(logging.INFO)
+logging.getLogger("biocommons.seqrepo.fastadir.fastadir").setLevel(logging.INFO)
 logging.getLogger("requests_cache.patcher").setLevel(logging.INFO)
 logging.getLogger("bioregistry.resource_manager").setLevel(logging.INFO)
 logging.getLogger("blib2to3.pgen2.driver").setLevel(logging.INFO)
 logging.getLogger("neo4j").setLevel(logging.INFO)
 logging.getLogger("asyncio").setLevel(logging.INFO)
 logger.handlers = []
 
-if 'METAKB_NORM_EB_PROD' in environ:
+if "METAKB_NORM_EB_PROD" in environ:
     ch = logging.StreamHandler()
     ch.setLevel(logging.DEBUG)
     logger.addHandler(ch)
 
 
 # default date format for all saved data files
 DATE_FMT = "%Y%m%d"
```

### Comparing `metakb-1.2.0.dev0/metakb/cli.py` & `metakb-2.0.0.dev0/src/metakb/cli.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,435 +1,367 @@
-"""
-Provide CLI utility for performing data collection, transformation, and upload
+"""Provide CLI utility for performing data collection, transformation, and upload
 to graph datastore.
 """
-from timeit import default_timer as timer
-from os import environ
 import logging
-from typing import Optional
-from pathlib import Path
 import re
 import tempfile
+from os import environ
+from pathlib import Path
+from timeit import default_timer as timer
+from typing import Optional
 from zipfile import ZipFile
 
 import asyncclick as click
-from disease.database import Database as DiseaseDatabase
-from disease.schemas import SourceName as DiseaseSources
-from disease.cli import CLI as DiseaseCLI
-from therapy.database import Database as TherapyDatabase
-from therapy.schemas import SourceName as TherapySources
-from therapy.cli import CLI as TherapyCLI
-from gene.database.dynamodb import DynamoDbDatabase as GeneDatabase
-from gene.schemas import SourceName as GeneSources
-import gene.cli as GeneCLI
 import boto3
 from boto3.exceptions import ResourceLoadException
 from botocore.config import Config
+from disease.cli import update_db as update_normalizer_disease_db
+from gene.cli import update_normalizer_db as update_normalizer_gene_db
+from therapy.cli import update_normalizer_db as update_normalizer_therapy_db
 
 from metakb import APP_ROOT
 from metakb.database import Graph
-from metakb.schemas import SourceName
-from metakb.harvesters import Harvester, CIViCHarvester, MOAHarvester, OncoKBHarvester
-from metakb.transform import Transform, CIViCTransform, MOATransform, OncoKBTransform
-
+from metakb.harvesters.civic import CivicHarvester
+from metakb.harvesters.moa import MoaHarvester
+from metakb.schemas.app import SourceName
+from metakb.transform import CivicTransform, MoaTransform
 
-logger = logging.getLogger('metakb.cli')
-logger.setLevel(logging.DEBUG)
+logger = logging.getLogger(__name__)
 
 
-def echo_info(msg: str):
+def echo_info(msg: str) -> None:
     """Log (as INFO) and echo given message.
-    :param str msg: message to emit
+
+    :param msg: message to emit
     """
     click.echo(msg)
     logger.info(msg)
 
 
-class CLI:
-    """Update database."""
+@click.command()
+@click.option(
+    "--db_url",
+    default="bolt://localhost:7687",
+    help=(
+        "URL endpoint for the application Neo4j database. Can also be provided via environment variable METAKB_DB_URL, which takes priority."
+    ),
+)
+@click.option(
+    "--db_username",
+    default="neo4j",
+    help=(
+        "Username to provide to application Neo4j database. Can also be provided via environment variable METAKB_DB_USERNAME, which takes priority."
+    ),
+)
+@click.option(
+    "--db_password",
+    default="password",
+    help=(
+        "Password to provide to application Neo4j database. Can also be provided via environment variable METAKB_DB_PASSWORD, which takes priority."
+    ),
+)
+@click.option(
+    "--force_load_normalizers_db",
+    "-f",
+    is_flag=True,
+    default=False,
+    help=("Load all normalizers data into DynamoDB database."),
+)
+@click.option(
+    "--normalizers_db_url",
+    help=(
+        "URL endpoint of normalizers DynamoDB database. If not given, defaults to `http://localhost:8000` per the configuration rules of the individual normalizers."
+    ),
+)
+@click.option(
+    "--load_latest_cdms",
+    "-l",
+    is_flag=True,
+    default=False,
+    help=(
+        "Clear MetaKB Neo4j database and load most recent available source CDM files. Does not run harvest and transform methods to generate new CDM files. Exclusive with --load_target_cdm and --load_latest_s3_cdms."
+    ),
+)
+@click.option(
+    "--load_target_cdm",
+    "-t",
+    type=click.Path(exists=True, dir_okay=False, readable=True, path_type=Path),
+    required=False,
+    help=(
+        "Load transformed CDM file at specified path. Exclusive with --load_latest_cdms and --load_latest_s3_cdms."
+    ),
+)
+@click.option(
+    "--load_latest_s3_cdms",
+    "-s",
+    is_flag=True,
+    default=False,
+    required=False,
+    help=(
+        "Clear MetaKB database, retrieve most recent data available from public VICC S3 bucket, and load the database with retrieved data. Exclusive with --load_latest_cdms and load_target_cdm."
+    ),
+)
+@click.option(
+    "--update_cached",
+    "-u",
+    is_flag=True,
+    default=False,
+    required=False,
+    help=(
+        "`True` if civicpy cache should be updated. Note this will take several minutes. `False` if local cache should be used"
+    ),
+)
+async def update_metakb_db(
+    db_url: str,
+    db_username: str,
+    db_password: str,
+    force_load_normalizers_db: bool,
+    normalizers_db_url: str,
+    load_latest_cdms: bool,
+    load_target_cdm: Optional[Path],
+    load_latest_s3_cdms: bool,
+    update_cached: bool,
+) -> None:
+    """Execute data harvest and transformation from resources and upload to graph
+    datastore.
+
+    :param db_url: URL endpoint for the application Neo4j database. Can also be provided
+        via environment variable ``METAKB_DB_URL``, which takes priority.
+    :param db_username: Username to provide to application Neo4j database. Can also be
+        provided via environment variable ``METAKB_DB_USERNAME``, which takes priority.
+    :param db_password: Password to provide to application Neo4j database. Can also be
+        provided via environment variable ``METAKB_DB_PASSWORD``, which takes priority.
+    :param force_load_normalizers_db: Load all normalizers data into DynamoDB database.
+    :param normalizers_db_url: URL endpoint of normalizers DynamoDB database. If not
+        given, defaults to ``http://localhost:8000`` per the configuration rules of the
+        individual normalizers.
+    :param load_latest_cdms: Clear MetaKB Neo4j database and load most recent available
+        source CDM files. Does not run harvest and transform methods to generate new CDM
+        files. Exclusive with --load_target_cdm and --load_latest_s3_cdms.
+    :param load_target_cdm: Load transformed CDM file at specified path. Exclusive with
+        --load_latest_cdms and --load_latest_s3_cdms.
+    :param load_latest_s3_cdms: Clear MetaKB database, retrieve most recent data
+        available from public VICC S3 bucket, and load the database with retrieved data.
+        Exclusive with --load_latest_cdms and load_target_cdm.
+    :param update_cached: `True` if civicpy cache should be updated. Note this will take
+        several minutes. `False` if local cache should be used
+    """
+    if sum([load_latest_cdms, bool(load_target_cdm), load_latest_s3_cdms]) > 1:
+        _help_msg(
+            "Error: Can only use one of `--load_latest_cdms`, `--load_target_cdm`, `--load_latest_s3_cdms`."
+        )
+
+    if not any([load_latest_cdms, load_target_cdm, load_latest_s3_cdms]):
+        if force_load_normalizers_db:
+            if normalizers_db_url:
+                for env_var_name in [
+                    "GENE_NORM_DB_URL",
+                    "THERAPY_NORM_DB_URL",
+                    "DISEASE_NORM_DB_URL",
+                ]:
+                    environ[env_var_name] = normalizers_db_url
+
+            _load_normalizers_db()
+
+        _harvest_sources(update_cached)
+        await _transform_sources()
+
+    # Load neo4j database
+    start = timer()
+    echo_info("Loading neo4j database...")
+
+    g = Graph(uri=db_url, credentials=(db_username, db_password))
+
+    if load_target_cdm:
+        g.load_from_json(load_target_cdm)
+    else:
+        version = _retrieve_s3_cdms() if load_latest_s3_cdms else None
+        g.clear()
+
+        for src in sorted({v.value for v in SourceName.__members__.values()}):
+            pattern = (
+                f"{src}_cdm_{version}.json"
+                if version is not None
+                else f"{src}_cdm_*.json"
+            )
+            globbed = (APP_ROOT / "data" / src / "transform").glob(pattern)
+
+            try:
+                path = sorted(globbed)[-1]
+            except IndexError as e:
+                msg = f"No valid transform file found matching pattern: {pattern}"
+                raise FileNotFoundError(msg) from e
+
+            g.load_from_json(path)
+
+    g.close()
+    end = timer()
+    echo_info(f"Successfully loaded neo4j database in {(end - start):.5f} s\n")
+
+
+def _help_msg(msg: str = "") -> None:
+    """Handle invalid user input.
+
+    :param msg: Error message to display to user.
+    """
+    ctx = click.get_current_context()
+    logger.fatal(msg)
+
+    if msg:
+        click.echo(msg)
+    else:
+        click.echo(ctx.get_help())
+
+    ctx.exit()
 
-    @staticmethod
-    @click.command()
-    @click.option(
-        '--db_url',
-        help=('URL endpoint for the application Neo4j database. Can also be '
-              'provided via environment variable METAKB_DB_URL.')
-    )
-    @click.option(
-        '--db_username',
-        help=('Username to provide to application database. Can also be '
-              'provided via environment variable METAKB_DB_USERNAME.')
-    )
-    @click.option(
-        '--db_password',
-        help=('Password to provide to application database. Can also be '
-              'provided via environment variable METAKB_DB_PASSWORD.')
-    )
-    @click.option(
-        '--load_normalizers_db',
-        '-i',
-        is_flag=True,
-        default=False,
-        help='Check normalizers database and load data if necessary.'
-    )
-    @click.option(
-        '--force_load_normalizers_db',
-        '-f',
-        is_flag=True,
-        default=False,
-        help=('Load all normalizers data into database. Overrides '
-              '--load_normalizers_db if both are selected.')
-    )
-    @click.option(
-        '--normalizers_db_url',
-        default='http://localhost:8000',
-        help=('URL endpoint of normalizers DynamoDB database. Set to '
-              '`http://localhost:8000` by default.')
-    )
-    @click.option(
-        "--load_latest_cdms",
-        "-l",
-        is_flag=True,
-        default=False,
-        help=("Clear MetaKB database and load most recent available source "
-              "CDM files. Does not run harvest and transform methods to "
-              "generate new CDM files. Exclusive with --load_target_cdm and "
-              "--load_latest_s3_cdms.")
-    )
-    @click.option(
-        "--load_target_cdm",
-        "-t",
-        type=click.Path(exists=True, dir_okay=False, readable=True,
-                        path_type=Path),
-        required=False,
-        help=("Load transformed CDM file at specified path. Exclusive with "
-              "--load_latest_cdms and --load_latest_s3_cdms.")
-    )
-    @click.option(
-        "--load_latest_s3_cdms",
-        "-s",
-        is_flag=True,
-        default=False,
-        required=False,
-        help=("Clear MetaKB database, retrieve most recent data available "
-              "from VICC S3 bucket, and load the database with retrieved "
-              "data. Will not download OncoKB transformed data. Exclusive with"
-              " --load_latest_cdms and load_target_cdm.")
-    )
-    @click.option(
-        "--update_cached",
-        "-uc",
-        is_flag=True,
-        default=False,
-        required=False,
-        help=("`True` if civicpy cache should be updated. Note this will take serveral"
-              "minutes. `False` if local cache should be used")
-    )
-    @click.option(
-        "--update_from_remote",
-        "-ur",
-        is_flag=True,
-        default=False,
-        required=False,
-        help=("If set to `True`, civicpy.update_cache will first download the remote "
-              "cache designated by REMOTE_CACHE_URL, store it to LOCAL_CACHE_PATH, "
-              "and then load the downloaded cache into memory.")
-    )
-    @click.option(
-        "--oncokb_variants_by_protein_change_path",
-        "-k",
-        required=False,
-        type=click.Path(exists=True, dir_okay=False, readable=True, path_type=Path),
-        help=("Path to CSV file containing header row with `hugo_symbol` and "
-              "`protein_change` and associated rows containing protein variants you "
-              "wish to harvest using a comma as the delimiter. Not required if using "
-              "`--load_latest_cdms`, `--load_target_cdm`, or `--load_latest_s3_cdms`")
-    )
-    async def update_metakb_db(
-        db_url: str, db_username: str, db_password: str,
-        load_normalizers_db: bool, force_load_normalizers_db: bool,
-        normalizers_db_url: str, load_latest_cdms: bool,
-        load_target_cdm: Optional[Path], load_latest_s3_cdms: bool,
-        update_cached: bool, update_from_remote: bool,
-        oncokb_variants_by_protein_change_path: Optional[Path]
-    ):
-        """Execute data harvest and transformation from resources and upload
-        to graph datastore.
-        """
-        if sum([load_latest_cdms, bool(load_target_cdm),
-                load_latest_s3_cdms]) > 1:
-            CLI()._help_msg("Error: Can only use one of `--load_latest_cdms`, "
-                            "`--load_target_cdm`, `--load_latest_s3_cdms`.")
-
-        db_url = CLI()._check_db_param(db_url, 'URL')
-        db_username = CLI()._check_db_param(db_username, 'username')
-        db_password = CLI()._check_db_param(db_password, 'password')
-
-        if normalizers_db_url:
-            for env_var_name in ['GENE_NORM_DB_URL', 'THERAPY_NORM_DB_URL',
-                                 'DISEASE_NORM_DB_URL']:
-                environ[env_var_name] = normalizers_db_url
-
-        if not any([load_latest_cdms, load_target_cdm, load_latest_s3_cdms]):
-            if load_normalizers_db or force_load_normalizers_db:
-                CLI()._load_normalizers_db(force_load_normalizers_db)
-
-            if not oncokb_variants_by_protein_change_path:
-                CLI()._help_msg(
-                    "Error: Must provide `--oncokb_variants_by_protein_change_path`")
-
-            CLI()._harvest_sources(update_cached, update_from_remote,
-                                   oncokb_variants_by_protein_change_path)
-            await CLI()._transform_sources()
 
-        # Load neo4j database
+def _load_normalizers_db() -> None:
+    """Load normalizer DynamoDB database source data."""
+    for name, update_normalizer_db_fn in [
+        ("Disease", update_normalizer_disease_db),
+        ("Therapy", update_normalizer_therapy_db),
+        ("Gene", update_normalizer_gene_db),
+    ]:
+        _update_normalizer_db(name, update_normalizer_db_fn)
+
+    echo_info("Normalizers database loaded.\n")
+
+
+def _update_normalizer_db(
+    name: str,
+    update_normalizer_db_fn: callable,
+) -> None:
+    """Update Normalizer DynamoDB database.
+
+    :param name: Name of the normalizer
+    :param update_normalizer_db_fn: Function to update the normalizer DynamoDB database
+    """
+    try:
+        echo_info(f"\nLoading {name} Normalizer data...")
+        update_normalizer_db_fn(["--update_all", "--update_merged"])
+        echo_info(f"Successfully Loaded {name} Normalizer data.\n")
+    except SystemExit as e:
+        if e.code != 0:
+            raise e
+
+
+def _harvest_sources(update_cached: bool) -> None:
+    """Run harvesting procedure for all sources.
+
+    :param update_cached: `True` if civicpy cache should be updated. Note this will take
+        several minutes. `False` if local cache should be used
+    """
+    echo_info("Harvesting sources...")
+    harvester_sources = {
+        SourceName.CIVIC.value: CivicHarvester,
+        SourceName.MOA.value: MoaHarvester,
+    }
+    total_start = timer()
+
+    for source_str, source_class in harvester_sources.items():
+        echo_info(f"Harvesting {source_str}...")
         start = timer()
-        echo_info("Loading neo4j database...")
 
-        g = Graph(uri=db_url, credentials=(db_username, db_password))
-        if load_target_cdm:
-            g.load_from_json(load_target_cdm)
+        if source_str == SourceName.CIVIC.value and update_cached:
+            # Use latest civic data
+            echo_info("(civicpy cache is also being updated)")
+            source = source_class(update_cache=True, update_from_remote=False)
         else:
-            version = None
-            if load_latest_s3_cdms:
-                version = CLI()._retrieve_s3_cdms()
-            g.clear()
-            for src in sorted({v.value for v
-                               in SourceName.__members__.values()}):
-                if version is not None:
-                    pattern = f"{src}_cdm_{version}.json"
-                else:
-                    pattern = f"{src}_cdm_*.json"
-                globbed = (APP_ROOT / "data" / src / "transform").glob(pattern)
-                try:
-                    path = sorted(globbed)[-1]
-                except IndexError:
-                    raise FileNotFoundError(f"No valid transform file found "
-                                            f"matching pattern: {pattern}")
-                click.echo(f"\tLoading {src} CDM from path...: {path}")
-                g.load_from_json(path)
-        g.close()
+            source = source_class()
+
+        source_successful = source.harvest()
+
         end = timer()
-        echo_info(
-            f"Successfully loaded neo4j database in {(end-start):.5f} s\n"
-        )
 
-    s3_cdm_pattern = re.compile(
-        r"cdm/20[23]\d[01]\d[0123]\d/(.*)_cdm_(.*).json.zip")
+        if not source_successful:
+            echo_info(f"{source_str} harvest failed.")
+            click.get_current_context().exit()
 
-    def _retrieve_s3_cdms(self) -> str:
-        """Retrieve most recent CDM files from VICC S3 bucket. Expects to find
-        files in a path like the following:
-            s3://vicc-metakb/cdm/20220201/civic_cdm_20220201.json.zip
-        :return: date string from retrieved files to use when loading to DB.
-        :raise: ResourceLoadException if S3 initialization fails
-        :raise: FileNotFoundError if unable to find files matching expected
+        echo_info(f"{source_str} harvest finished in {(end - start):.5f} s")
+
+    total_end = timer()
+    echo_info(
+        f"Successfully harvested all sources in {(total_end - total_start):.5f} s\n"
+    )
+
+
+async def _transform_sources() -> None:
+    """Run transformation procedure for all sources."""
+    echo_info("Transforming harvested data to CDM...")
+    transform_sources = {
+        SourceName.CIVIC.value: CivicTransform,
+        SourceName.MOA.value: MoaTransform,
+    }
+    total_start = timer()
+
+    for src_str, src_name in transform_sources.items():
+        echo_info(f"Transforming {src_str}...")
+        start = timer()
+        source = src_name()
+        await source.transform()
+        end = timer()
+        echo_info(f"{src_str} transform finished in {(end - start):.5f} s.")
+        source.create_json()
+
+    total_end = timer()
+    echo_info(
+        f"Successfully transformed all sources to CDM in "
+        f"{(total_end - total_start):.5f} s\n"
+    )
+
+
+def _retrieve_s3_cdms() -> str:
+    """Retrieve most recent CDM files from VICC S3 bucket.
+    Expects to find files in a path like the following:
+        s3://vicc-metakb/cdm/20220201/civic_cdm_20220201.json.zip
+
+    :raise ResourceLoadException: if S3 initialization fails
+    :raise FileNotFoundError:  if unable to find files matching expected
         pattern in VICC MetaKB bucket.
-        """
-        echo_info("Attempting to fetch CDM files from S3 bucket")
-        s3 = boto3.resource("s3", config=Config(region_name="us-east-2"))
-        if not s3:
-            raise ResourceLoadException("Unable to initiate AWS S3 Resource")
-        bucket = sorted(
-            list(
-                s3.Bucket("vicc-metakb").objects.filter(Prefix="cdm").all()
-            ),
-            key=lambda f: f.key,
-            reverse=True
-        )
-        newest_version: Optional[str] = None
-        for file in bucket:
-            match = re.match(self.s3_cdm_pattern, file.key)
-            if match:
-                source = match.group(1)
-                if newest_version is None:
-                    newest_version = match.group(2)
-                elif match.group(2) != newest_version:
-                    continue
-            else:
-                continue
+    :return: date string from retrieved files to use when loading to DB.
+    """
+    echo_info("Attempting to fetch CDM files from S3 bucket")
+    s3 = boto3.resource("s3", config=Config(region_name="us-east-2"))
 
-            tmp_path = Path(tempfile.gettempdir()) / "metakb_dl_tmp"
-            with open(tmp_path, "wb") as f:
-                file.Object().download_fileobj(f)
-
-            cdm_dir = APP_ROOT / "data" / source / "transform"
-            cdm_zip = ZipFile(tmp_path, "r")
-            cdm_zip.extract(f"{source}_cdm_{newest_version}.json", cdm_dir)
-
-        if newest_version is None:
-            raise FileNotFoundError("Unable to locate files matching expected "
-                                    "resource pattern in VICC s3 bucket")
-        echo_info(f"Retrieved CDM files dated {newest_version}")
-        return newest_version
-
-    @staticmethod
-    def _harvest_sources(
-        update_cached, update_from_remote, oncokb_variants_by_protein_change_path
-    ) -> None:
-        """Run harvesting procedure for all sources."""
-        echo_info("Harvesting sources...")
-        # TODO: Switch to using constant
-        harvester_sources = {
-            SourceName.CIVIC.value: CIViCHarvester,
-            SourceName.MOA.value: MOAHarvester,
-            SourceName.ONCOKB.value: OncoKBHarvester
-        }
-        total_start = timer()
-        for source_str, source_class in harvester_sources.items():
-            echo_info(f"Harvesting {source_str}...")
-            start = timer()
-
-            if source_str == SourceName.CIVIC and update_cached:
-                echo_info("(civicpy cache is also being updated)")
-                source: Harvester = source_class(
-                    update_cache=update_cached, update_from_remote=update_from_remote
-                )
-                # Use latest civic data
-                source_successful = source.harvest()
-            else:
-                source: Harvester = source_class()
-                if source_str == SourceName.ONCOKB:
-                    source_successful = source.harvest(
-                        oncokb_variants_by_protein_change_path
-                    )
-                else:
-                    source_successful = source.harvest()
-
-            end = timer()
-            if not source_successful:
-                echo_info(f'{source_str} harvest failed.')
-                click.get_current_context().exit()
-            echo_info(
-                f"{source_str} harvest finished in {(end - start):.5f} s")
-        total_end = timer()
-        echo_info(
-            f"Successfully harvested all sources in "
-            f"{(total_end - total_start):.5f} s\n"
+    if not s3:
+        msg = "Unable to initiate AWS S3 Resource"
+        raise ResourceLoadException(msg)
+
+    bucket = sorted(  # noqa: C414
+        list(s3.Bucket("vicc-metakb").objects.filter(Prefix="cdm").all()),
+        key=lambda f: f.key,
+        reverse=True,
+    )
+    newest_version: Optional[str] = None
+
+    for file in bucket:
+        match = re.match(
+            re.compile(r"cdm/20[23]\d[01]\d[0123]\d/(.*)_cdm_(.*).json.zip"), file.key
         )
 
-    @staticmethod
-    async def _transform_sources() -> None:
-        """Run transformation procedure for all sources."""
-        echo_info("Transforming harvested data to CDM...")
-        # TODO: Switch to using constant
-        transform_sources = {
-            SourceName.CIVIC.value: CIViCTransform,
-            SourceName.MOA.value: MOATransform,
-            SourceName.ONCOKB.value: OncoKBTransform
-        }
-        total_start = timer()
-        for src_str, src_name in transform_sources.items():
-            echo_info(f"Transforming {src_str}...")
-            start = timer()
-            source: Transform = src_name()
-            await source.transform()
-            end = timer()
-            echo_info(
-                f"{src_str} transform finished in {(end - start):.5f} s.")
-            source.create_json()
-        total_end = timer()
-        echo_info(
-            f"Successfully transformed all sources to CDM in "
-            f"{(total_end-total_start):.5f} s\n"
-        )
+        if match:
+            source = match.group(1)
+            if newest_version is None:
+                newest_version = match.group(2)
+            elif match.group(2) != newest_version:
+                continue
+        else:
+            continue
 
-    def _load_normalizers_db(self, load_normalizer_db):
-        """Load normalizer database source data.
+        tmp_path = Path(tempfile.gettempdir()) / "metakb_dl_tmp"
+        with tmp_path.open("wb") as f:
+            file.Object().download_fileobj(f)
 
-        :param bool load_normalizer_db: Load normalizer database for each
-            normalizer
-        """
-        if load_normalizer_db:
-            load_disease = load_therapy = load_gene = True
-        else:
-            load_disease = self._check_normalizer(
-                DiseaseDatabase(), {src.value for src in DiseaseSources})
-            load_therapy = self._check_normalizer(
-                TherapyDatabase(), {src for src in TherapySources})
-            load_gene = self._check_normalizer(
-                GeneDatabase(), {src.value for src in GeneSources})
-
-        for load_source, normalizer_cli in [
-            (load_disease, DiseaseCLI), (load_therapy, TherapyCLI),
-            (load_gene, GeneCLI)
-        ]:
-            name = \
-                str(normalizer_cli).split()[1].split('.')[0][1:].capitalize()
-            self._update_normalizer_db(name, load_source, normalizer_cli)
-        echo_info("Normalizers database loaded.\n")
-
-    @staticmethod
-    def _check_normalizer(db, sources) -> bool:
-        """Check whether or not normalizer data needs to be loaded.
-
-        :param Database db: Normalizer database
-        :param set sources: Sources that are needed in the normalizer db
-        :return: `True` If normalizer needs to be loaded. `False` otherwise.
-        """
-        for src in sources:
-            response = db.metadata.get_item(
-                Key={'src_name': src}
-            )
-            if not response.get('Item'):
-                return True
-        return False
-
-    @staticmethod
-    def _update_normalizer_db(name, load_normalizer, source_cli) -> None:
-        """Update Normalizer database.
-
-        :param str name: Name of the normalizer
-        :param bool load_normalizer: Whether or not to load normalizer db
-        :param CLI source_cli: Normalizer CLI class for loading and
-            deleting source data
-        """
-        if load_normalizer:
-            try:
-                echo_info(f'\nLoading {name} Normalizer data...')
-                source_cli.update_normalizer_db(
-                    ['--update_all', '--update_merged'])
-                echo_info(f'Successfully Loaded {name} Normalizer data.\n')
-            except SystemExit as e:
-                if e.code != 0:
-                    raise e
-        else:
-            echo_info(f'{name} Normalizer is already loaded.\n')
+        cdm_dir = APP_ROOT / "data" / source / "transform"
+        cdm_zip = ZipFile(tmp_path, "r")
+        cdm_zip.extract(f"{source}_cdm_{newest_version}.json", cdm_dir)
 
-    @staticmethod
-    def _check_db_param(param: str, name: str) -> str:
-        """Check for MetaKB database parameter.
-        :param str param: value of parameter as received from command line
-        :param str name: name of parameter
-        :return: parameter value, or exit with error message if unavailable
-        """
-        if not param:
-            env_var_name = f'METAKB_DB_{name.upper()}'
-            if env_var_name in environ.keys():
-                return environ[env_var_name]
-            else:
-                # Default is local
-                if name == 'URL':
-                    return "bolt://localhost:7687"
-                elif name == 'username':
-                    return 'neo4j'
-                else:
-                    return 'admin'
-        else:
-            return param
+    if newest_version is None:
+        msg = "Unable to locate files matching expected resource pattern in VICC s3 bucket"
+        raise FileNotFoundError(msg)
 
-    @staticmethod
-    def _help_msg(msg: str = ""):
-        """Handle invalid user input.
-        :param str msg: Error message to display to user.
-        """
-        ctx = click.get_current_context()
-        logger.fatal(msg)
-        if msg:
-            click.echo(msg)
-        else:
-            click.echo(ctx.get_help())
-        ctx.exit()
+    echo_info(f"Retrieved CDM files dated {newest_version}")
+    return newest_version
 
 
-if __name__ == '__main__':
-    CLI().update_metakb_db(_anyio_backend="asyncio")
+if __name__ == "__main__":
+    update_metakb_db(_anyio_backend="asyncio")
```

### Comparing `metakb-1.2.0.dev0/metakb/harvesters/base.py` & `metakb-2.0.0.dev0/src/metakb/harvesters/base.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,52 +1,53 @@
 """A module for the Harvester base class"""
-from typing import List, Dict, Optional
+import datetime
 import json
 import logging
-from datetime import datetime as dt
+from typing import Dict, List, Optional
 
 from metakb import APP_ROOT, DATE_FMT
 
-logger = logging.getLogger("metakb.harvesters.base")
-logger.setLevel(logging.DEBUG)
+logger = logging.getLogger(__name__)
 
 
 class Harvester:
     """A base class for content harvesters."""
 
     def harvest(self) -> bool:
-        """
-        Retrieve and store records from a resource. Records may be stored in
+        """Retrieve and store records from a resource. Records may be stored in
         any manner, but must be retrievable by :method:`iterate_records`.
 
         :return: `True` if operation was successful, `False` otherwise.
         :rtype: bool
         """
         raise NotImplementedError
 
-    def create_json(self, items: Dict[str, List],
-                    filename: Optional[str] = None) -> bool:
+    def create_json(
+        self, items: Dict[str, List], filename: Optional[str] = None
+    ) -> bool:
         """Create composite and individual JSON for harvested data.
 
         :param Dict items: item types keyed to Lists of values
         :param Optional[str] filename: custom filename for composite document
         :return: `True` if JSON creation was successful. `False` otherwise.
         """
-        composite_dict = dict()
+        composite_dict = {}
         src = self.__class__.__name__.lower().split("harvest")[0]
         src_dir = APP_ROOT / "data" / src / "harvester"
         src_dir.mkdir(exist_ok=True, parents=True)
-        today = dt.strftime(dt.today(), DATE_FMT)
+        today = datetime.datetime.strftime(
+            datetime.datetime.now(tz=datetime.timezone.utc), DATE_FMT
+        )
         try:
             for item_type, item_list in items.items():
                 composite_dict[item_type] = item_list
 
-                with open(src_dir / f"{item_type}_{today}.json", "w+") as f:
+                with (src_dir / f"{item_type}_{today}.json").open("w+") as f:
                     f.write(json.dumps(item_list, indent=4))
             if not filename:
                 filename = f"{src}_harvester_{today}.json"
-            with open(src_dir / filename, "w+") as f:
+            with (src_dir / filename).open("w+") as f:
                 f.write(json.dumps(composite_dict, indent=4))
         except Exception as e:
-            logger.error(f"Unable to create json: {e}")
+            logger.error("Unable to create json: %s", e)
             return False
         return True
```

### Comparing `metakb-1.2.0.dev0/metakb/harvesters/civic.py` & `metakb-2.0.0.dev0/src/metakb/harvesters/civic.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,29 +1,30 @@
 """A module for the CIViC harvester."""
 import logging
-from typing import Dict, List, Optional
 from pathlib import Path
+from typing import Dict, List, Optional
 
-from civicpy import civic as civicpy, LOCAL_CACHE_PATH
+from civicpy import LOCAL_CACHE_PATH
+from civicpy import civic as civicpy
 
-from metakb.harvesters.base import Harvester  # noqa: I202
+from metakb.harvesters.base import Harvester
 
 logger = logging.getLogger(__name__)
 
 
-class CIViCHarvester(Harvester):
+class CivicHarvester(Harvester):
     """A class for the CIViC harvester."""
 
     def __init__(
         self,
         update_cache: bool = False,
         update_from_remote: bool = True,
-        local_cache_path: Optional[Path] = LOCAL_CACHE_PATH
+        local_cache_path: Optional[Path] = LOCAL_CACHE_PATH,
     ) -> None:
-        """Initialize CIViCHarvester class.
+        """Initialize CivicHarvester class.
 
         :param update_cache: `True` if civicpy cache should be updated. Note
             this will take several minutes. `False` if to use local cache.
         :param update_from_remote: If set to `True`, civicpy.update_cache will first
             download the remote cache designated by REMOTE_CACHE_URL, store it
             to LOCAL_CACHE_PATH, and then load the downloaded cache into memory.
             This parameter defaults to `True`.
@@ -58,25 +59,25 @@
 
             json_created = self.create_json(
                 {
                     "evidence": self.evidence,
                     "genes": self.genes,
                     "variants": self.variants,
                     "molecular_profiles": self.molecular_profiles,
-                    "assertions": self.assertions
+                    "assertions": self.assertions,
                 },
-                filename
+                filename,
             )
             if not json_created:
                 logger.error(
                     "CIViC Harvester was not successful: JSON files not created."
                 )
                 return False
-        except Exception as e:  # noqa: E722
-            logger.error(f"CIViC Harvester was not successful: {e}")
+        except Exception as e:
+            logger.error("CIViC Harvester was not successful: %s", e)
             return False
         else:
             logger.info("CIViC Harvester was successful.")
             return True
 
     def harvest_evidence(self) -> List[Dict]:
         """Harvest all CIViC evidence item records.
@@ -126,14 +127,15 @@
         """
         if obj is None:
             return None
 
         if isinstance(obj, civicpy.CivicRecord):
             return {
                 k: self._dictify(v)
-                for k, v in obj.__dict__.items() if not k.startswith(("_", "partial"))
+                for k, v in obj.__dict__.items()
+                if not k.startswith(("_", "partial"))
             }
 
         if isinstance(obj, list):
             return [self._dictify(item) for item in obj]
 
         return obj
```

### Comparing `metakb-1.2.0.dev0/metakb/harvesters/moa.py` & `metakb-2.0.0.dev0/src/metakb/harvesters/moa.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,74 +1,70 @@
 """A module for the Molecular Oncology Almanac harvester"""
 import logging
-from typing import Optional, List, Dict
+from typing import Dict, List, Optional
 
 import requests
 import requests_cache
 
-from metakb.harvesters.base import Harvester  # noqa: I202
+from metakb.harvesters.base import Harvester
 
+logger = logging.getLogger(__name__)
 
-logger = logging.getLogger("metakb.harvesters.moa")
-logger.setLevel(logging.DEBUG)
 
-
-class MOAHarvester(Harvester):
+class MoaHarvester(Harvester):
     """A class for the Molecular Oncology Almanac harvester."""
 
     def harvest(self, filename: Optional[str] = None) -> bool:
-        """
-        Retrieve and store sources, variants, and assertions
+        """Retrieve and store sources, variants, and assertions
         records from MOAlmanac in composite and individual JSON files.
 
         :param Optional[str] filename: File name for composite json
-        :return: True if successfully retreived, False otherwise
+        :return: True if successfully retrieved, False otherwise
         :rtype: bool
         """
         try:
             assertion_resp = self._get_all_assertions()
             sources = self._harvest_sources(assertion_resp)
             variants, variants_list = self.harvest_variants()
             assertions = self.harvest_assertions(assertion_resp, variants_list)
             genes = self._harvest_genes()
             json_created = self.create_json(
                 {
                     "assertions": assertions,
                     "sources": sources,
                     "variants": variants,
-                    "genes": genes
+                    "genes": genes,
                 },
-                filename
+                filename,
             )
             if not json_created:
                 logger.error("MOAlmanac Harvester was not successful.")
                 return False
-        except Exception as e:  # noqa: E722
-            logger.error(f"MOAlmanac Harvester was not successful: {e}")
+        except Exception as e:
+            logger.error("MOAlmanac Harvester was not successful: %s", e)
             return False
         else:
             logger.info("MOAlmanac Harvester was successful.")
             return True
 
     @staticmethod
     def _harvest_genes() -> List[Dict]:
-        """Harvest all genes from MOAlamanc
+        """Harvest all genes from MOAlmanac
 
         :return: List of MOA gene records
         """
-        genes = list()
+        genes = []
         with requests_cache.disabled():
-            r = requests.get("https://moalmanac.org/api/genes")
+            r = requests.get("https://moalmanac.org/api/genes", timeout=60)
             if r.status_code == 200:
                 genes = r.json()
         return genes
 
     def _harvest_sources(self, assertion_resp: List[Dict]) -> List[Dict]:
-        """
-        Harvest all MOA sources
+        """Harvest all MOA sources
 
         :param List[Dict] assertion_resp: A list of MOA assertion records
         :return: A list of sources
         :rtype: list
         """
         sources = []
 
@@ -77,201 +73,191 @@
             s = self._source_item(source)
             if s not in sources:
                 sources.append(s)
 
         return sources
 
     def harvest_variants(self) -> List[Dict]:
-        """
-        Harvest all MOA variants
+        """Harvest all MOA variants
 
         :return: A list of variants
         :rtype: list
         """
         variants_list = self._get_all_variants()
         variants = []
 
         for variant in variants_list:
             v = self._harvest_variant(variant)
             variants.append(v)
 
         return variants, variants_list
 
-    def harvest_assertions(self, assertion_resp: List[Dict],
-                           variants_list: List[Dict]) -> List[Dict]:
-        """
-        Harvest all MOA assertions
+    def harvest_assertions(
+        self, assertion_resp: List[Dict], variants_list: List[Dict]
+    ) -> List[Dict]:
+        """Harvest all MOA assertions
 
         :param List[Dict] assertion_resp: A list of MOA assertion records
         :param List[Dict] variants_list: A list of MOA variant records
         :return: A list of assertions
         :rtype: list
         """
         assertions = []
         for assertion in assertion_resp:
             a = self._harvest_assertion(assertion, variants_list)
             assertions.append(a)
 
         return assertions
 
     def _get_all_assertions(self) -> List[Dict]:
-        """
-        Return all assertion records.
+        """Return all assertion records.
 
         :return: All moa assertion records
         """
         with requests_cache.disabled():
-            r = requests.get("https://moalmanac.org/api/assertions")
-            assertions = r.json()
-
-        return assertions
+            r = requests.get("https://moalmanac.org/api/assertions", timeout=60)
+            return r.json()
 
     def _get_all_variants(self) -> List[Dict]:
-        """
-        Return all variant records
+        """Return all variant records
 
         :return: All moa variant records
         """
         with requests_cache.disabled():
-            r = requests.get("https://moalmanac.org/api/features")
-            variants = r.json()
-
-        return variants
+            r = requests.get("https://moalmanac.org/api/features", timeout=60)
+            return r.json()
 
     def _source_item(self, source: Dict) -> Dict:
-        """
-        Harvest an individual MOA source of evidence
+        """Harvest an individual MOA source of evidence
 
         :param Dict source: source record of each assertion record
         :return: a dictionary containing MOA source of evidence data
         :rtype: dict
         """
-        source_record = {
+        return {
             "id": source["source_id"],
             "type": source["source_type"],
             "doi": source["doi"],
             "nct": source["nct"],
             "pmid": source["pmid"],
             "url": source["url"],
-            "citation": source["citation"]
+            "citation": source["citation"],
         }
-        return source_record
 
     def _harvest_variant(self, variant: Dict) -> Dict:
         """Harvest an individual MOA variant record.
 
         :param Dict variant: A MOA variant record
         :return: A dictionary containing MOA variant data
         :rtype: dict
         """
-        variant_record = {
-            "id": variant["feature_id"]
-        }
+        variant_record = {"id": variant["feature_id"]}
 
-        variant_record.update({k: v for k, v in variant["attributes"][0].items()})  # noqa: E501
+        variant_record.update(dict(variant["attributes"][0].items()))
         variant_record.update(self._get_feature(variant_record))
 
         return variant_record
 
     def _harvest_assertion(self, assertion: Dict, variants_list: List[Dict]) -> Dict:
-        """
-        Harvest an individual MOA assertion record
+        """Harvest an individual MOA assertion record
 
         :param Dict assertion: a MOA assertion record
         :param List[Dict] variants_list: a list of MOA variant records
         :return: A dictionary containing MOA assertion data
         :rtype: dict
         """
         assertion_record = {
             "id": assertion["assertion_id"],
             "context": assertion["context"],
             "description": assertion["description"],
             "disease": {
                 "name": assertion["disease"],
                 "oncotree_code": assertion["oncotree_code"],
-                "oncotree_term": assertion["oncotree_term"]
+                "oncotree_term": assertion["oncotree_term"],
             },
             "therapy_name": assertion["therapy_name"],
             "therapy_type": assertion["therapy_type"],
             "clinical_significance": self._get_therapy(
-                assertion["therapy_resistance"],
-                assertion["therapy_sensitivity"]),
+                assertion["therapy_resistance"], assertion["therapy_sensitivity"]
+            ),
             "predictive_implication": assertion["predictive_implication"],
             "favorable_prognosis": assertion["favorable_prognosis"],
             "created_on": assertion["created_on"],
             "last_updated": assertion["last_updated"],
             "submitted_by": assertion["submitted_by"],
             "validated": assertion["validated"],
-            "source_ids": assertion["sources"][0]["source_id"]
+            "source_ids": assertion["sources"][0]["source_id"],
         }
 
         for v in variants_list:
             if v["attributes"][0] == assertion["features"][0]["attributes"][0]:
                 assertion_record.update({"variant": self._harvest_variant(v)})
 
         return assertion_record
 
     def _get_therapy(self, resistance: bool, sensitivity: bool) -> Optional[str]:
-        """
-        Get therapy response data.
+        """Get therapy response data.
 
         :param bool resistance: `True` if Therapy Resistance.
             `False` if not Therapy Resistance
         :param bool sensitivity: `True` if Therapy Sensitivity.
             `False` if not Therapy Sensitivity
         :return: whether the therapy response is resistance or sensitivity
         :rtype: str
         """
         if resistance:
             return "resistance"
-        elif sensitivity:
+        if sensitivity:
             return "sensitivity"
-        else:
-            return None
+        return None
 
     def _get_feature(self, v: Dict) -> Dict:
-        """
-        Get feature name from the harvested variants
+        """Get feature name from the harvested variants
 
         :param Dict v: harvested MOA variant
         :return: feature name same format as displayed in moalmanac.org
         :rtype: dict
         """
         feature_type = v["feature_type"]
         if feature_type == "rearrangement":
-            feature = "{}{}{}".format(v["gene1"],
-                                      f"--{v['gene2']}" if v["gene2"] else "",
-                                      f" {v['rearrangement_type']}"
-                                      if v["rearrangement_type"] else "")
+            feature = "{}{}{}".format(
+                v["gene1"],
+                f"--{v['gene2']}" if v["gene2"] else "",
+                f" {v['rearrangement_type']}" if v["rearrangement_type"] else "",
+            )
         elif feature_type == "somatic_variant":
-            feature = "{}{}{}".format(v["gene"],
-                                      f" {v['protein_change']}"
-                                      if v["protein_change"] else "",
-                                      f" ({v['variant_annotation']})"
-                                      if v["variant_annotation"] else "")
+            feature = "{}{}{}".format(
+                v["gene"],
+                f" {v['protein_change']}" if v["protein_change"] else "",
+                f" ({v['variant_annotation']})" if v["variant_annotation"] else "",
+            )
         elif feature_type == "germline_variant":
-            feature = "{}{}".format(v["gene"], " (Pathogenic)"
-                                    if v["pathogenic"] == "1.0" else "")
+            feature = "{}{}".format(
+                v["gene"], " (Pathogenic)" if v["pathogenic"] == "1.0" else ""
+            )
         elif feature_type == "copy_number":
             feature = "{} {}".format(v["gene"], v["direction"])
         elif feature_type == "microsatellite_stability":
             feature = "{}".format(v.get("status"))
         elif feature_type == "mutational_signature":
-            csn = v["cosmic_signature_number"]
-            feature = "COSMIC Signature {}".format(csn)
+            csn = v.get("cosmic_signature_number", "")
+            feature = f"COSMIC Signature {csn}"
         elif feature_type == "mutational_burden":
             clss = v["classification"]
             min_mut = v["minimum_mutations"]
             mut_per_mb = v["mutations_per_mb"]
-            feature = "{}{}".format(clss,
-                                    f" (>= {min_mut} mutations)" if min_mut
-                                    else (f" (>= {mut_per_mb} mutations/Mb)"
-                                          if mut_per_mb else ""))
+            feature = "{}{}".format(
+                clss,
+                f" (>= {min_mut} mutations)"
+                if min_mut
+                else (f" (>= {mut_per_mb} mutations/Mb)" if mut_per_mb else ""),
+            )
         elif feature_type == "neoantigen_burden":
             feature = "{}".format(v["classification"])
         elif feature_type == "knockdown" or feature_type == "silencing":
-            feature = "{}{}".format(v["gene"], f" ({v['technique']})"
-                                    if v["technique"] else "")
+            feature = "{}{}".format(
+                v["gene"], f" ({v['technique']})" if v["technique"] else ""
+            )
         else:
             feature = "{}".format(v["event"])
 
         return {"feature": feature.strip()}
```

### Comparing `metakb-1.2.0.dev0/metakb/normalizers.py` & `metakb-2.0.0.dev0/src/metakb/normalizers.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,98 +1,93 @@
 """Module for VICC normalizers."""
 import logging
 from typing import List, Optional, Tuple
 
-from ga4gh.vrsatile.pydantic.vrsatile_models import VariationDescriptor, Extension
-from variation.query import QueryHandler as VariationQueryHandler
-from therapy.query import QueryHandler as TherapyQueryHandler
-from therapy.schemas import NormalizationService as NormalizedTherapy, ApprovalRating
+from disease.database import create_db as create_disease_db
 from disease.query import QueryHandler as DiseaseQueryHandler
 from disease.schemas import NormalizationService as NormalizedDisease
-from gene.database.dynamodb import DynamoDbDatabase
+from ga4gh.core import core_models
+from ga4gh.vrs import models
+from gene.database import create_db as create_gene_db
 from gene.query import QueryHandler as GeneQueryHandler
 from gene.schemas import NormalizeService as NormalizedGene
-
+from therapy.database import create_db as create_therapy_db
+from therapy.query import QueryHandler as TherapyQueryHandler
+from therapy.schemas import ApprovalRating
+from therapy.schemas import NormalizationService as NormalizedTherapy
+from variation.query import QueryHandler as VariationQueryHandler
 
 logger = logging.getLogger(__name__)
 
 
-class VICCNormalizers:
+class ViccNormalizers:
     """A class for normalizing terms using VICC normalizers."""
 
-    def __init__(
-        self, gene_query_handler: Optional[GeneQueryHandler] = None,
-        variation_query_handler: Optional[VariationQueryHandler] = None,
-        disease_query_handler: Optional[DiseaseQueryHandler] = None,
-        therapy_query_handler: Optional[TherapyQueryHandler] = None
-    ) -> None:
-        """Initialize the VICC Normalizers.
-
-        :param gene_query_handler: Gene QueryHandler instance
-        :param variation_query_handler: Variation QueryHandler instance
-        :param disease_query_handler: Disease QueryHandler instance
-        :param therapy_query_handler: Therapy QueryHandler instance
-        """
-        self.disease_query_handler = disease_query_handler or DiseaseQueryHandler()
-        self.therapy_query_handler = therapy_query_handler or TherapyQueryHandler()
-        self.gene_query_handler = (gene_query_handler or GeneQueryHandler(DynamoDbDatabase()))  # noqa: E501
-
-        if variation_query_handler:
-            self.variation_query_handler = variation_query_handler
-        else:
-            self.variation_query_handler = VariationQueryHandler(
-                gene_query_handler=self.gene_query_handler
-            )
+    def __init__(self) -> None:
+        """Initialize the VICC normalizers query handler instances."""
+        self.gene_query_handler = GeneQueryHandler(create_gene_db())
+        self.variation_normalizer = VariationQueryHandler(
+            gene_query_handler=self.gene_query_handler
+        )
+        self.disease_query_handler = DiseaseQueryHandler(create_disease_db())
+        self.therapy_query_handler = TherapyQueryHandler(create_therapy_db())
 
     async def normalize_variation(
         self, queries: List[str]
-    ) -> Optional[VariationDescriptor]:
+    ) -> Optional[models.Variation]:
         """Normalize variation queries.
 
-        :param queries: Possible query strings to try to normalize
+        :param List[str] queries: Possible query strings to try to normalize
             which are used in the event that a MANE transcript cannot be found
         :return: A normalized variation
         """
         for query in queries:
             if not query:
                 continue
             try:
-                variation_norm_resp = await self.variation_query_handler.normalize_handler.normalize(query)  # noqa: E501
-                if variation_norm_resp and variation_norm_resp.variation_descriptor:
-                    return variation_norm_resp.variation_descriptor
-            except Exception as e:  # noqa: E722
-                logger.warning(f"Variation Normalizer raised an exception using query"
-                               f" {query}: {e}")
+                variation_norm_resp = (
+                    await self.variation_normalizer.normalize_handler.normalize(query)
+                )
+                if variation_norm_resp and variation_norm_resp.variation:
+                    return variation_norm_resp.variation
+            except Exception as e:
+                logger.warning(
+                    "Variation Normalizer raised an exception using query %s: %s",
+                    query,
+                    e,
+                )
         return None
 
     def normalize_gene(
         self, queries: List[str]
     ) -> Tuple[Optional[NormalizedGene], Optional[str]]:
         """Normalize gene queries
 
-        :param queries: Gene queries to normalize
-        :return: The highest matched gene's normalized response and ID, if successful
+        :param list queries: Gene queries to normalize
+        :return: The highest matched gene's normalized response and ID
         """
         gene_norm_resp = None
         normalized_gene_id = None
         highest_match = 0
         for query_str in queries:
             if not query_str:
                 continue
 
             try:
                 gene_norm_resp = self.gene_query_handler.normalize(query_str)
             except Exception as e:
-                logger.warning(f"Gene Normalizer raised an exception using query "
-                               f"{query_str}: {e}")
+                logger.warning(
+                    "Gene Normalizer raised an exception using query %s: %s",
+                    query_str,
+                    e,
+                )
             else:
                 if gene_norm_resp.match_type > highest_match:
                     highest_match = gene_norm_resp.match_type
-                    normalized_gene_id = \
-                        gene_norm_resp.gene_descriptor.gene_id
+                    normalized_gene_id = gene_norm_resp.normalized_id
                     if highest_match == 100:
                         break
         return gene_norm_resp, normalized_gene_id
 
     def normalize_disease(
         self, queries: List[str]
     ) -> Tuple[Optional[NormalizedDisease], Optional[str]]:
@@ -108,21 +103,23 @@
         for query in queries:
             if not query:
                 continue
 
             try:
                 disease_norm_resp = self.disease_query_handler.normalize(query)
             except Exception as e:
-                logger.warning(f"Disease Normalizer raised an exception using query "
-                               f"{query}: {e}")
+                logger.warning(
+                    "Disease Normalizer raised an exception using query %s: %s",
+                    query,
+                    e,
+                )
             else:
                 if disease_norm_resp.match_type > highest_match:
                     highest_match = disease_norm_resp.match_type
-                    normalized_disease_id = \
-                        disease_norm_resp.disease_descriptor.disease_id
+                    normalized_disease_id = disease_norm_resp.normalized_id
                     if highest_match == 100:
                         break
         return disease_norm_resp, normalized_disease_id
 
     def normalize_therapy(
         self, queries: List[str]
     ) -> Tuple[Optional[NormalizedTherapy], Optional[str]]:
@@ -138,68 +135,87 @@
         for query in queries:
             if not query:
                 continue
 
             try:
                 therapy_norm_resp = self.therapy_query_handler.normalize(query)
             except Exception as e:
-                logger.warning(f"Therapy Normalizer raised an exception using "
-                               f"query {query}: {e}")
+                logger.warning(
+                    "Therapy Normalizer raised an exception using query %s: %s",
+                    query,
+                    e,
+                )
             else:
                 if therapy_norm_resp.match_type > highest_match:
                     highest_match = therapy_norm_resp.match_type
-                    normalized_therapy_id = therapy_norm_resp.therapy_descriptor.therapy_id  # noqa: E501
+                    normalized_therapy_id = therapy_norm_resp.normalized_id
                     if highest_match == 100:
                         break
         return therapy_norm_resp, normalized_therapy_id
 
     @staticmethod
     def get_regulatory_approval_extension(
-        therapy_norm_resp: NormalizedTherapy
-    ) -> Optional[Extension]:
+        therapy_norm_resp: NormalizedTherapy,
+    ) -> Optional[core_models.Extension]:
         """Given therapy normalization service response, extract out the regulatory
         approval extension
 
         :param NormalizedTherapy therapy_norm_resp: Response from normalizing therapy
         :return: Extension containing transformed regulatory approval and indication
             data if it `regulatory_approval` extensions exists in therapy normalizer
         """
         regulatory_approval_extension = None
-        tn_resp_exts = therapy_norm_resp.dict().get("therapy_descriptor", {}).get("extensions") or []  # noqa: E501
+        tn_resp_exts = (
+            therapy_norm_resp.model_dump()
+            .get("therapeutic_agent", {})
+            .get("extensions")
+            or []
+        )
         tn_ext = [v for v in tn_resp_exts if v["name"] == "regulatory_approval"]
 
         if tn_ext:
             ext_value = tn_ext[0]["value"]
             approval_ratings = ext_value.get("approval_ratings", [])
             matched_ext_value = None
 
-            if any(ar in {ApprovalRating.FDA_PRESCRIPTION, ApprovalRating.FDA_OTC}
-                    for ar in approval_ratings):
-                if ApprovalRating.FDA_DISCONTINUED not in approval_ratings or \
-                    ApprovalRating.CHEMBL_4 in approval_ratings:  # noqa: E125
+            if any(
+                ar in {ApprovalRating.FDA_PRESCRIPTION, ApprovalRating.FDA_OTC}
+                for ar in approval_ratings
+            ):
+                if (
+                    ApprovalRating.FDA_DISCONTINUED not in approval_ratings
+                    or ApprovalRating.CHEMBL_4 in approval_ratings
+                ):
                     matched_ext_value = "FDA"
             elif ApprovalRating.CHEMBL_4 in approval_ratings:
                 matched_ext_value = "chembl_phase_4"
 
             if matched_ext_value:
                 has_indications = ext_value.get("has_indication", [])
-                matched_indications = list()
+                matched_indications = []
 
                 for indication in has_indications:
                     indication_exts = indication.get("extensions", [])
                     for indication_ext in indication_exts:
                         if indication_ext["value"] == matched_ext_value:
-                            matched_indications.append({
+                            matched_ind = {
                                 "id": indication["id"],
                                 "type": indication["type"],
                                 "label": indication["label"],
-                                "disease_id": indication["disease_id"]
-                            })
+                            }
+
+                            if indication.get("mappings"):
+                                matched_ind["mappings"] = indication["mappings"]
+
+                            matched_indications.append(matched_ind)
 
-                regulatory_approval_extension = Extension(
+                regulatory_approval_extension = core_models.Extension(
                     name="regulatory_approval",
                     value={
-                        "approval_rating": "FDA" if matched_ext_value == "FDA" else "ChEMBL",  # noqa: E501
-                        "has_indications": matched_indications
-                    })
+                        "approval_rating": "FDA"
+                        if matched_ext_value == "FDA"
+                        else "ChEMBL",
+                        "has_indications": matched_indications,
+                    },
+                )
 
         return regulatory_approval_extension
```

### Comparing `metakb-1.2.0.dev0/metakb/transform/civic.py` & `metakb-2.0.0.dev0/src/metakb/transform/civic.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,774 +1,912 @@
 """A module for to transform CIViC."""
-from typing import Optional, Dict, List, Set
-from pathlib import Path
 import logging
 import re
+from enum import Enum
+from pathlib import Path
+from typing import Dict, List, Optional, Tuple
 
-from ga4gh.vrsatile.pydantic.vrsatile_models import VariationDescriptor, \
-    Extension, Expression, GeneDescriptor, ValueObjectDescriptor
+from ga4gh.core import core_models
+from ga4gh.vrs import models
+from pydantic import BaseModel, ValidationError
 
 from metakb import APP_ROOT
-from metakb.normalizers import VICCNormalizers
-from metakb.transform.base import Transform
-import metakb.schemas as schemas
-
+from metakb.normalizers import ViccNormalizers
+from metakb.schemas.annotation import Direction, Document
+from metakb.schemas.categorical_variation import ProteinSequenceConsequence
+from metakb.schemas.variation_statement import (
+    AlleleOrigin,
+    VariantTherapeuticResponseStudy,
+    VariantTherapeuticResponseStudyPredicate,
+    _VariantOncogenicityStudyQualifier,
+)
+from metakb.transform.base import (
+    CivicEvidenceLevel,
+    MethodId,
+    TherapeuticProcedureType,
+    Transform,
+)
 
 logger = logging.getLogger(__name__)
 
+# SNP pattern
+SNP_RE = re.compile(r"RS\d+")
+
+# Variant names that are known to not be supported in the variation-normalizer
+UNABLE_TO_NORMALIZE_VAR_NAMES = {
+    "mutation",
+    "exon",
+    "overexpression",
+    "frameshift",
+    "promoter",
+    "deletion",
+    "type",
+    "insertion",
+    "expression",
+    "duplication",
+    "copy",
+    "underexpression",
+    "number",
+    "variation",
+    "repeat",
+    "rearrangement",
+    "activation",
+    "mislocalization",
+    "translocation",
+    "wild",
+    "polymorphism",
+    "frame",
+    "shift",
+    "loss",
+    "function",
+    "levels",
+    "inactivation",
+    "snp",
+    "fusion",
+    "dup",
+    "truncation",
+    "homozygosity",
+    "gain",
+    "phosphorylation",
+}
+
+
+class _VariationCache(BaseModel):
+    """Create model for caching CIViC Variation data that will be accessed when
+    transforming MP data
+    """
+
+    vrs_variation: Dict
+    civic_gene_id: str
+    variant_types: Optional[List[core_models.Coding]] = None
+    mappings: Optional[List[core_models.Mapping]] = None
+    aliases: Optional[List[str]] = None
+    coordinates: Optional[Dict]
+    members: Optional[List[models.Variation]] = None
+
+
+class SourcePrefix(str, Enum):
+    """Define constraints for source prefixes."""
+
+    PUBMED = "PUBMED"
+    ASCO = "ASCO"
+    ASH = "ASH"
+
 
-class CIViCTransform(Transform):
+class CivicTransform(Transform):
     """A class for transforming CIViC to the common data model."""
 
-    def __init__(self,
-                 data_dir: Path = APP_ROOT / "data",
-                 harvester_path: Optional[Path] = None,
-                 normalizers: Optional[VICCNormalizers] = None) -> None:
+    def __init__(
+        self,
+        data_dir: Path = APP_ROOT / "data",
+        harvester_path: Optional[Path] = None,
+        normalizers: Optional[ViccNormalizers] = None,
+    ) -> None:
         """Initialize CIViC Transform class.
-        :param Path data_dir: Path to source data directory
-        :param Optional[Path] harvester_path: Path to previously harvested data
-        :param VICCNormalizers normalizers: normalizer collection instance
-        """
-        super().__init__(data_dir=data_dir,
-                         harvester_path=harvester_path,
-                         normalizers=normalizers)
-        # Able to normalize these IDSs
-        self.valid_ids = {
-            'variation_descriptors': dict(),
-            'disease_descriptors': dict(),
-            'therapy_descriptors': dict()
-        }
-        # Unable to normalize these IDs
-        self.invalid_ids = {
-            'therapy_descriptors': list(),
-            'disease_descriptors': list()
+
+        :param data_dir: Path to source data directory
+        :param harvester_path: Path to previously harvested CIViC data
+        :param normalizers: normalizer collection instance
+        """
+        super().__init__(
+            data_dir=data_dir, harvester_path=harvester_path, normalizers=normalizers
+        )
+
+        # Method will always be the same
+        self.methods = [self.methods_mapping[MethodId.CIVIC_EID_SOP.value]]
+
+        # Cache for normalized concepts. The key is the concept type and value is a
+        # dictionary of mappings from CIViC concept (key) to transformed concept (value)
+        self.able_to_normalize = {
+            "variations": {},  # will store _VariationCache data
+            "molecular_profiles": {},
+            "diseases": {},
+            "therapeutics": {},
+            "genes": {},
         }
 
     @staticmethod
-    def _mp_to_variant_mapping(molecular_profiles: List[Dict]) -> Dict:
-        """Get mapping from Molecular Profile ID to Variant ID. We currently do not
-        handle complex molecular profiles (> 1 variant associated).
+    def _mp_to_variant_mapping(molecular_profiles: List[Dict]) -> Tuple[List, Dict]:
+        """Get mapping from Molecular Profile ID to Variant ID.
+        We currently do not handle complex molecular profiles (> 1 variant associated).
 
         :param molecular_profiles: List of civic molecular profiles represented as
             dictionaries
-        :return: Molecular Profile ID to Variant ID mapping {mp_id: v_id}
+        :return: Tuple containing list of supported molecular profiles and mapping from
+            Molecular Profile ID to Variant ID {mp_id: v_id}
         """
-        mapping: Dict = {}
-        not_supported_mps = set()
+        mp_id_to_v_id: Dict = {}
+        supported_mps = []
+        not_supported_mp_ids = set()
         for mp in molecular_profiles:
             mp_id = mp["id"]
             mp_variant_ids = mp["variant_ids"]
             if len(mp_variant_ids) != 1:
-                mapping[mp_id] = None
-                not_supported_mps.add(mp_id)
+                mp_id_to_v_id[mp_id] = None
+                not_supported_mp_ids.add(mp_id)
             else:
-                mapping[mp_id] = mp_variant_ids[0]
+                supported_mps.append(mp)
+                mp_id_to_v_id[mp_id] = mp_variant_ids[0]
 
-        logger.debug(f"{len(not_supported_mps)} Molecular Profiles not supported: "
-                     f"{not_supported_mps}")
-        return mapping
+        logger.debug(
+            "%s Molecular Profiles not supported: %s",
+            len(not_supported_mp_ids),
+            not_supported_mp_ids,
+        )
+        return supported_mps, mp_id_to_v_id
 
-    async def transform(self):
-        """Transform CIViC harvested json to common data model."""
+    async def transform(self) -> None:
+        """Transform CIViC harvested json to common data model. Will store transformed
+        results in instance variables.
+        """
         data = self.extract_harvester()
-        evidence_items = data['evidence']
-        assertions = data['assertions']
-        molecular_profiles = data["molecular_profiles"]
-        variants = data['variants']
-        genes = data['genes']
-        mp_id_to_v_id_mapping = self._mp_to_variant_mapping(molecular_profiles)
-
-        # Only want evidence with approved status
-        evidence_items = [e for e in evidence_items if e["status"] == "accepted"]
-
-        # Filter Variant IDs for Prognostic, Predictive, and Diagnostic evidence
-        supported_evidence_types = ['PROGNOSTIC', 'PREDICTIVE', 'DIAGNOSTIC']
-        evidence_items = [e for e in evidence_items
-                          if e["evidence_type"].upper() in supported_evidence_types]
-        assertions = [a for a in assertions
-                      if a["assertion_type"].upper() in supported_evidence_types]
-
-        vids = {mp_id_to_v_id_mapping[e["molecular_profile_id"]]
-                for e in evidence_items if e["molecular_profile_id"]}
-        vids |= {mp_id_to_v_id_mapping[a["molecular_profile_id"]]
-                 for a in assertions if a["molecular_profile_id"]}
-
-        await self._add_variation_descriptors(variants, vids)
-        self._add_gene_descriptors(genes)
-        self._add_methods()
-        self._transform_evidence_and_assertions(evidence_items, mp_id_to_v_id_mapping)
-        self._transform_evidence_and_assertions(
-            assertions, mp_id_to_v_id_mapping, is_evidence=False
+        evidence_items = data["evidence"]
+
+        # Get list of supported molecular profiles and mapping to variant id
+        molecular_profiles, mp_id_to_v_id_mapping = self._mp_to_variant_mapping(
+            data["molecular_profiles"]
         )
 
-    def _transform_evidence_and_assertions(
-        self, records: List[Dict], mp_id_to_v_id_mapping: Dict, is_evidence=True
+        # Only want evidence with approved status and predictive evidence type
+        evidence_items = [
+            e
+            for e in evidence_items
+            if e["status"] == "accepted" and e["evidence_type"].upper() == "PREDICTIVE"
+        ]
+
+        # Get all variant IDs from supported molecular profiles
+        vids = {
+            mp_id_to_v_id_mapping[e["molecular_profile_id"]]
+            for e in evidence_items
+            if e["molecular_profile_id"]
+        }
+
+        # Add variant (only supported) and gene (all) data
+        # (mutates `variations` and `genes`)
+        variants = data["variants"]
+        variants = [v for v in variants if v["id"] in vids]
+        await self._add_variations(variants)
+        self._add_genes(data["genes"])
+
+        # Only want to add MPs where variation-normalizer succeeded for the related
+        # variant. Will update `molecular_profiles`
+        able_to_normalize_vids = self.able_to_normalize["variations"].keys()
+        mps = [
+            mp
+            for mp in molecular_profiles
+            if f"civic.vid:{mp['variant_ids'][0]}" in able_to_normalize_vids
+        ]
+        self._add_protein_consequences(mps, mp_id_to_v_id_mapping)
+
+        # Add variant therapeutic response study data. Will update `studies`
+        self._add_variant_therapeutic_response_studies(
+            evidence_items, mp_id_to_v_id_mapping
+        )
+
+    def _add_variant_therapeutic_response_studies(
+        self, records: List[Dict], mp_id_to_v_id_mapping: Dict
     ) -> None:
-        """Transform statements, propositions, descriptors, and documents
-        from CIViC evidence items and assertions.
+        """Create Variant Therapeutic Response Studies from CIViC Evidence Items.
+        Will add associated values to instance variables (`therapeutics`, `diseases`,
+        and `documents`). `able_to_normalize` and `unable_to_normalize` will also be
+        mutated for associated therapeutics and diseases.
 
-        :param records: CIViC Evidence Items or Assertions
-        :param mp_id_to_v_id_mapping: Molecular Profile ID to Variant ID mappin
+        :param records: List of CIViC Evidence Items
+        :param mp_id_to_v_id_mapping: Molecular Profile ID to Variant ID mapping
             {mp_id: v_id}
-        :param is_evidence: `True` if records are evidence items.
-            `False` if records are assertions.
         """
         for r in records:
-            name_lower = r['name'].lower()
-            if name_lower.startswith('eid'):
-                civic_id = name_lower.replace('eid', 'civic.eid:')
-            else:
-                civic_id = name_lower.replace('aid', 'civic.aid:')
-
-            # Omit entries that are not in an accepted state
-            if r['status'] != 'accepted':
-                logger.warning(f"{civic_id} has status: {r['status']}")
+            # Check cache for molecular profile, variation and gene data
+            mp_id = f"civic.mpid:{r['molecular_profile_id']}"
+            mp = self.able_to_normalize["molecular_profiles"].get(mp_id)
+            if not mp:
+                logger.debug("mp_id not supported: %s", mp_id)
                 continue
 
-            record_type = r["evidence_type"] if is_evidence else r["assertion_type"]
-            if record_type not in ["PREDICTIVE", "PROGNOSTIC", "DIAGNOSTIC"]:
+            variant_id = f"civic.vid:{mp_id_to_v_id_mapping[r['molecular_profile_id']]}"
+            variation_gene_map = self.able_to_normalize["variations"].get(variant_id)
+            if not variation_gene_map:
+                logger.debug("variant_id not supported: %s", variant_id)
                 continue
-            else:
-                # Functional Evidence types do not have a disease
-                if not r['disease']:
-                    continue
-
-            if record_type == "PREDICTIVE":
-                if len(r["therapies"]) != 1:
-                    continue
-                else:
-                    therapy_id = f"civic.tid:{r['therapies'][0]['id']}"
-                    therapy_descriptor = \
-                        self._add_therapy_descriptor(therapy_id, r)
-                    if not therapy_descriptor:
-                        continue
 
-                    if therapy_descriptor not in self.therapy_descriptors:
-                        self.therapy_descriptors.append(therapy_descriptor)
-            else:
-                therapy_id = None
-                therapy_descriptor = None
+            # Get predicate
+            predicate = self._get_predicate(r["evidence_type"], r["significance"])
 
-            disease_id = f"civic.did:{r['disease']['id']}"
-            disease_descriptor = self._add_disease_descriptor(disease_id, r)
-            if not disease_descriptor:
+            # Don't support TR that has  `None`, "N/A", or "Unknown" predicate
+            if not predicate:
                 continue
 
-            if disease_descriptor not in self.disease_descriptors:
-                self.disease_descriptors.append(disease_descriptor)
-
-            variant_id = f"civic.vid:{mp_id_to_v_id_mapping[r['molecular_profile_id']]}"
-            variation_descriptor = \
-                self.valid_ids['variation_descriptors'].get(variant_id)
-            if not variation_descriptor:
+            # Add disease
+            if not r["disease"]:
                 continue
 
-            try:
-                proposition_type = self._get_proposition_type(record_type)
-            except KeyError:
+            civic_disease = self._add_disease(r["disease"])
+            if not civic_disease:
                 continue
 
-            predicate = self._get_predicate(proposition_type, r["significance"])
+            therapies = r["therapies"]
+            if len(therapies) == 1:
+                # Add TherapeuticAgent
+                therapeutic_procedure_id = f"civic.tid:{therapies[0]['id']}"
+                therapy_interaction_type = None
+                therapeutic_procedure_type = TherapeuticProcedureType.THERAPEUTIC_AGENT
+            else:
+                # Add TherapeuticSubstituteGroup
+                therapy_interaction_type = r["therapy_interaction_type"]
+                therapeutic_ids = [f"civic.tid:{t['id']}" for t in therapies]
+                therapeutic_digest = self._get_digest_for_str_lists(therapeutic_ids)
+
+                if therapy_interaction_type == "SUBSTITUTES":
+                    therapeutic_procedure_id = f"civic.tsgid:{therapeutic_digest}"
+                    therapeutic_procedure_type = (
+                        TherapeuticProcedureType.THERAPEUTIC_SUBSTITUTE_GROUP
+                    )
+                elif therapy_interaction_type == "COMBINATION":
+                    therapeutic_procedure_id = f"civic.ctid:{therapeutic_digest}"
+                    therapeutic_procedure_type = (
+                        TherapeuticProcedureType.COMBINATION_THERAPY
+                    )
+                else:
+                    logger.debug(
+                        "civic therapy_interaction_type not supported: %s",
+                        therapy_interaction_type,
+                    )
+                    continue
 
-            # Don't support TR that has  `None`, "N/A", or "Unknown" predicate
-            if not predicate:
+            civic_therapeutic = self._add_therapeutic_procedure(
+                therapeutic_procedure_id,
+                therapies,
+                therapeutic_procedure_type,
+                therapy_interaction_type,
+            )
+            if not civic_therapeutic:
                 continue
 
-            object = None
-            if therapy_descriptor:
-                object = therapy_descriptor["therapy_id"]
-
-            proposition = self._get_proposition(
-                proposition_type, predicate, variation_descriptor["variation_id"],
-                disease_descriptor["disease_id"], object)
-
-            # Only support Therapeutic Response and Prognostic
-            if not proposition:
+            # Add document
+            document = self._add_eid_document(r["source"])
+            if not document:
                 continue
 
-            if is_evidence:
-                # Evidence items's method and evidence level
-                method = f'method:{schemas.MethodID.CIVIC_EID_SOP}'
-                evidence_level = f"civic.evidence_level:{r['evidence_level']}"
-
-                # Supported by evidence for evidence item
-                document = self._get_eid_document(r['source'])
-                if document not in self.documents:
-                    self.documents.append(document)
-                supported_by = [document['id']]
-            else:
-                # Assertion's method
-                if r['amp_level'] and not r['acmg_codes']:
-                    method = \
-                        f'method:' \
-                        f'{schemas.MethodID.CIVIC_AID_AMP_ASCO_CAP}'
-                elif not r['amp_level'] and r['acmg_codes']:
-                    method = f'method:' \
-                             f'{schemas.MethodID.CIVIC_AID_ACMG}'
-                else:
-                    # Statements are required to have a method
-                    logger.warning(f"Unable to get method for {civic_id}")
-                    continue
+            # Get strength
+            direction = self._get_evidence_direction(r["evidence_direction"])
+            evidence_level = CivicEvidenceLevel[r["evidence_level"]]
+            strength = self.evidence_level_to_vicc_concept_mapping[evidence_level]
+
+            # Get qualifier
+            civic_gene = self.able_to_normalize["genes"].get(
+                variation_gene_map["civic_gene_id"]
+            )
+            qualifiers = self._get_variant_onco_study_qualifier(
+                r["variant_origin"], civic_gene
+            )
 
-                # assertion's evidence level
-                evidence_level = self._get_assertion_evidence_level(r)
+            statement = VariantTherapeuticResponseStudy(
+                id=r["name"].lower().replace("eid", "civic.eid:"),
+                description=r["description"] if r["description"] else None,
+                direction=direction,
+                strength=strength,
+                predicate=predicate,
+                variant=mp,
+                therapeutic=civic_therapeutic,
+                tumorType=civic_disease,
+                qualifiers=qualifiers,
+                specifiedBy=self.methods[0],
+                isReportedIn=[document],
+            ).model_dump(exclude_none=True)
+            self.studies.append(statement)
+
+    def _get_variant_onco_study_qualifier(
+        self, variant_origin: str, gene: Optional[core_models.Gene] = None
+    ) -> Optional[_VariantOncogenicityStudyQualifier]:
+        """Get Variant Oncogenicity Study Qualifier
+
+        :param variant_origin: CIViC evidence item's variant origin
+        :param gene: CIViC gene data
+        :return: Variant Oncogenicity Study Qualifier for a Variant Therapeutic Response
+            Study, if allele origin or gene exists
+        """
+        variant_origin = variant_origin.upper()
+        if variant_origin == "SOMATIC":
+            allele_origin = AlleleOrigin.SOMATIC
+        elif variant_origin in {"RARE_GERMLINE", "COMMON_GERMLINE"}:
+            allele_origin = AlleleOrigin.GERMLINE
+        else:
+            allele_origin = None
 
-                # Supported by evidence for assertion
-                supported_by = list()
-                documents = \
-                    self._get_aid_document(r)
-                for d in documents:
-                    if d not in self.documents:
-                        self.documents.append(d)
-                    supported_by.append(d['id'])
-
-                for ev_id in r["evidence_ids"]:
-                    supported_by.append(f"civic.eid:{ev_id}")
-
-            statement = schemas.Statement(
-                id=civic_id,
-                description=r['description'],
-                direction=self._get_evidence_direction(
-                    r["evidence_direction"] if is_evidence else r["assertion_direction"]
-                ),
-                evidence_level=evidence_level,
-                proposition=proposition['id'],
-                variation_origin=self._get_variation_origin(
-                    r['variant_origin']),
-                variation_descriptor=variant_id,
-                therapy_descriptor=therapy_id,
-                disease_descriptor=disease_id,
-                method=method,
-                supported_by=supported_by
-            ).dict(exclude_none=True)
-            self.statements.append(statement)
+        if allele_origin or gene:
+            qualifier = _VariantOncogenicityStudyQualifier(
+                alleleOrigin=allele_origin, geneContext=gene
+            )
+        else:
+            qualifier = None
+        return qualifier
 
-    def _get_evidence_direction(self, direction) -> Optional[str]:
-        """Return the evidence direction.
+    def _get_evidence_direction(self, direction: str) -> Optional[Direction]:
+        """Get the normalized evidence direction
 
-        :param str direction: The civic evidence_direction value
-        :return: `supports` or `does_not_support` or None
+        :param direction: CIViC evidence item's direction
+        :return: Normalized evidence direction
         """
         direction_upper = direction.upper()
         if direction_upper == "SUPPORTS":
-            return schemas.Direction.SUPPORTS.value
-        elif direction_upper == "DOES_NOT_SUPPORT":
-            return schemas.Direction.DOES_NOT_SUPPORT.value
-        else:
-            return None
-
-    def _get_assertion_evidence_level(self, assertion) -> Optional[str]:
-        """Return evidence_level for CIViC assertion.
+            return Direction.SUPPORTS
+        if direction_upper == "DOES_NOT_SUPPORT":
+            return Direction.REFUTES
+        return Direction.NONE
+
+    def _get_predicate(
+        self, record_type: str, clin_sig: str
+    ) -> Optional[VariantTherapeuticResponseStudyPredicate]:
+        """Return predicate for an evidence item.
 
-        :param dict assertion: CIViC Assertion
-        :return: CIViC assertion evidence_level
+        :param record_type: The evidence type
+        :param clin_sig: The evidence item's clinical significance
+        :return: Predicate for proposition
         """
-        evidence_level = None
-        # TODO: CHECK
-        if assertion['amp_level']:
-            if assertion['amp_level'] == 'Not Applicable':
-                evidence_level = None
-            else:
-                amp_level = assertion["amp_level"]
-                regex = re.compile(r"TIER_(?P<tier>\w+)_LEVEL_(?P<level>\w+)")
-                match = regex.match(amp_level)
-                if match:
-                    match = match.groupdict()
-                    tier = match["tier"]
-                    level = match["level"]
-
-                    if tier == 'I':
-                        tier = 1
-                    elif tier == 'II':
-                        tier = 2
-                    elif tier == 'III':
-                        tier = 3
-                    elif tier == 'IV':
-                        tier = 4
+        predicate = None
 
-                    evidence_level = f"amp_asco_cap_2017_level:" \
-                                     f"{tier}{level}"
-                else:
-                    raise Exception(f"{amp_level} not supported with regex")
-        return evidence_level
+        if record_type == "PREDICTIVE":
+            if clin_sig == "SENSITIVITYRESPONSE":
+                predicate = (
+                    VariantTherapeuticResponseStudyPredicate.PREDICTS_SENSITIVITY_TO
+                )
+            elif clin_sig == "RESISTANCE":
+                predicate = (
+                    VariantTherapeuticResponseStudyPredicate.PREDICTS_RESISTANCE_TO
+                )
+        return predicate
 
-    def _get_proposition_type(self,
-                              evidence_type,
-                              is_evidence=True) -> Optional[schemas.PropositionType]:  # noqa: E501
-        """Return proposition type for a given EID or AID.
-
-        :param str evidence_type: CIViC evidence type
-        :param bool is_evidence: `True` if EID. `False` if AID.
-        :return: Proposition's type
-        """
-        evidence_type = evidence_type.upper()
-        if evidence_type in schemas.PropositionType.__members__.keys():
-            if evidence_type == 'PREDISPOSING':
-                if is_evidence:
-                    proposition_type = schemas.PropositionType.PREDISPOSING
-                else:
-                    proposition_type = schemas.PropositionType.PATHOGENIC
-            else:
-                proposition_type = schemas.PropositionType[evidence_type]
-        else:
-            raise KeyError(f"Proposition Type {evidence_type} not found in "
-                           f"schemas.PropositionType")
-        return proposition_type
+    def _add_protein_consequences(
+        self, molecular_profiles: List[Dict], mp_id_to_v_id_mapping: Dict
+    ) -> None:
+        """Create Protein Sequence Consequence objects for all supported MP records.
+        Mutates instance variables `able_to_normalize['molecular_profiles']` and
+        `molecular_profiles`.
+
+        :param molecular_profiles: List of supported Molecular Profiles in CIViC.
+            The associated, single variant record for each MP was successfully
+            normalized
+        :param mp_id_to_v_id_mapping: Mapping from Molecular Profile ID to Variant ID
+            {mp_id: v_id}
+        """
+        for mp in molecular_profiles:
+            mp_id = f"civic.mpid:{mp['id']}"
+            vid = f"civic.vid:{mp_id_to_v_id_mapping[mp['id']]}"
+            civic_variation_data = self.able_to_normalize["variations"][vid]
 
-    def _get_variation_origin(self, variant_origin) -> Optional[str]:
-        """Return variant origin.
+            # Only support Alleles for now
+            if civic_variation_data["vrs_variation"]["type"] != "Allele":
+                continue
 
-        :param str variant_origin: CIViC variant origin
-        :return: Variation origin
-        """
-        variant_origin = variant_origin.upper()
-        if variant_origin == "SOMATIC":
-            origin = schemas.VariationOrigin.SOMATIC.value
-        elif variant_origin in ["RARE_GERMLINE", "COMMON_GERMLINE"]:
-            origin = schemas.VariationOrigin.GERMLINE.value
-        elif variant_origin == "NA":
-            origin = schemas.VariationOrigin.NOT_APPLICABLE.value
+            # Get aliases from MP and Variant record
+            aliases = civic_variation_data["aliases"] or []
+            for a in mp["aliases"] or []:
+                if not SNP_RE.match(a):
+                    aliases.append(a)
+
+            # Get molecular profile score data
+            mp_score = mp["molecular_profile_score"]
+            if mp_score:
+                extensions = [
+                    core_models.Extension(
+                        name="CIViC Molecular Profile Score", value=mp_score
+                    )
+                ]
+            else:
+                extensions = []
+
+            # Get CIViC representative coordinate and Variant types data
+            for ext_key, var_key in [
+                ("CIViC representative coordinate", "coordinates"),
+                ("Variant types", "variant_types"),
+            ]:
+                if civic_variation_data[var_key]:
+                    extensions.append(
+                        core_models.Extension(
+                            name=ext_key, value=civic_variation_data[var_key]
+                        )
+                    )
+
+            psc = ProteinSequenceConsequence(
+                id=mp_id,
+                description=mp["description"],
+                label=mp["name"],
+                definingContext=civic_variation_data["vrs_variation"],
+                aliases=list(set(aliases)) or None,
+                mappings=civic_variation_data["mappings"],
+                extensions=extensions or None,
+                members=civic_variation_data["members"],
+            ).model_dump(exclude_none=True)
+            self.molecular_profiles.append(psc)
+            self.able_to_normalize["molecular_profiles"][mp_id] = psc
+
+    @staticmethod
+    def _get_variant_name(variant: Dict) -> str:
+        """Get variant name from CIViC Variant record.
+        If 'c.' in name, use the cDNA name
+
+        :param variant: CIViC Variant record
+        :return: Variant name to use for query
+        """
+        if "c." in variant["name"]:
+            variant_name = variant["name"]
+            if "(" in variant_name:
+                variant_name = variant_name.replace("(", "").replace(")", "")
+            variant_name = variant_name.split()[-1]
         else:
-            origin = None
-        return origin
+            variant_name = variant["name"]
+        return variant_name
 
-    def _get_predicate(self, proposition_type,
-                       clin_sig) -> Optional[schemas.Predicate]:
-        """Return predicate for an evidence item.
+    @staticmethod
+    def _is_supported_variant_query(variant_name: str, variant_id: int) -> bool:
+        """Determine if a variant name is supported by the variation-normalizer.
+        This is used to skip normalization on variants that the variation-normalizer
+        is known not to support
+
+        :param variant_name: Variant name in CIViC
+        :param variant_id: CIViC Variant ID
+        :return: `True` if the variant_name is supported in the variation-normalizer.
+            `False` otherwise
+        """
+        # Will remove as more get implemented in variation normalizer
+        # Filtering to speed up transformation
+        vname_lower = variant_name.lower()
+
+        if vname_lower.endswith("fs") or "-" in vname_lower or "/" in vname_lower:
+            logger.debug(
+                "Variation Normalizer does not support %s: %s", variant_id, variant_name
+            )
+            return False
 
-        :param str proposition_type: The proposition type
-        :param str clin_sig: The evidence item's clinical significance
-        :return: Predicate for proposition if valid
-        """
-        if clin_sig is None or clin_sig.upper() in ['N/A', 'UNKNOWN']:
-            return None
+        if set(vname_lower.split()) & UNABLE_TO_NORMALIZE_VAR_NAMES:
+            logger.debug(
+                "Variation Normalizer does not support %s: %s", variant_id, variant_name
+            )
+            return False
 
-        clin_sig = '_'.join(clin_sig.upper().split())
-        if clin_sig == "NA":
-            logger.info("NA predicate not supported")
-            return None
-        predicate = None
+        return True
 
-        if proposition_type == schemas.PropositionType.PREDICTIVE:
-            if clin_sig == 'SENSITIVITYRESPONSE':
-                predicate = schemas.PredictivePredicate.SENSITIVITY
-            elif clin_sig == 'RESISTANCE':
-                predicate = schemas.PredictivePredicate.RESISTANCE
-        elif proposition_type == schemas.PropositionType.DIAGNOSTIC:
-            predicate = schemas.DiagnosticPredicate[clin_sig]
-        elif proposition_type == schemas.PropositionType.PROGNOSTIC:
-            if clin_sig == 'POSITIVE':
-                predicate = schemas.PrognosticPredicate.BETTER_OUTCOME
-            else:
-                predicate = schemas.PrognosticPredicate[clin_sig]
-        elif proposition_type == schemas.PropositionType.FUNCTIONAL:
-            predicate = schemas.FunctionalPredicate[clin_sig]
-        elif proposition_type == schemas.PropositionType.ONCOGENIC:
-            # TODO: There are currently no Oncogenic types in CIViC harvester
-            #  Look into why this is
-            pass
-        elif proposition_type == schemas.PropositionType.PATHOGENIC:
-            if clin_sig in ['PATHOGENIC', 'LIKELY_PATHOGENIC']:
-                predicate = schemas.PathogenicPredicate.PATHOGENIC
-        else:
-            logger.warning(f"CIViC proposition type: {proposition_type} "
-                           f"not supported in Predicate schemas")
-        return predicate
+    async def _get_variation_members(
+        self, variant: Dict
+    ) -> Optional[List[models.Variation]]:
+        """Get members field for variation object. This is the related variant concepts.
+        For now, we will only do genomic HGVS expressions
+
+        :param variant: CIViC Variant record
+        :return: List containing one VRS variation record for associated genomic HGVS
+            expression, if variation-normalizer was able to normalize
+        """
+        members = None
+        genomic_hgvs = (
+            [expr for expr in variant["hgvs_expressions"] if "g." in expr] or [None]
+        )[0]
+        if genomic_hgvs:
+            vrs_genomic_variation = await self.vicc_normalizers.normalize_variation(
+                [genomic_hgvs]
+            )
 
-    async def _add_variation_descriptors(self, variants: List, vids: Set) -> None:
-        """Add Variation Descriptors to dict of transformations.
+            if vrs_genomic_variation:
+                genomic_params = vrs_genomic_variation.model_dump(exclude_none=True)
+                genomic_params["label"] = genomic_hgvs
+                members = [models.Variation(**genomic_params)]
+        return members
+
+    async def _add_variations(self, variants: List[Dict]) -> None:
+        """Normalize supported CIViC variant records.
+        Mutates instance variables `able_to_normalize['variations']` and `variations`,
+        if the variation-normalizer can successfully normalize the variant
 
-        :param List variants: CIViC variants
-        :param set vids: Candidate CIViC Variant IDs
+        :param variants: List of all CIViC variant records
         """
         for variant in variants:
-            if variant["id"] not in vids:
-                continue
             variant_id = f"civic.vid:{variant['id']}"
-            if "c." in variant["name"]:
-                variant_name = variant["name"]
-                if "(" in variant_name:
-                    variant_name = \
-                        variant_name.replace("(", "").replace(")", "")
-                variant_name = variant_name.split()[-1]
-            else:
-                variant_name = variant["name"]
-
+            variant_name = self._get_variant_name(variant)
             variant_query = f"{variant['entrez_name']} {variant_name}"
-            hgvs_exprs = self._get_hgvs_expr(variant)
 
-            # TODO: Remove as more get implemented in variation normalizer
-            #  Filtering to speed up transformation
-            vname_lower = variant["name"].lower()
-
-            if vname_lower.endswith("fs") or "-" in vname_lower or "/" in vname_lower:  # noqa: E501
-                if not hgvs_exprs:
-                    logger.warning("Variation Normalizer does not support "
-                                   f"{variant_id}: {variant_query}")
-                    continue
-
-            unable_to_normalize = {
-                "mutation", "exon", "overexpression",
-                "frameshift", "promoter", "deletion", "type", "insertion",
-                "expression", "duplication", "copy", "underexpression",
-                "number", "variation", "repeat", "rearrangement", "activation",
-                "expression", "mislocalization", "translocation", "wild",
-                "polymorphism", "frame", "shift", "loss", "function", "levels",
-                "inactivation", "snp", "fusion", "dup", "truncation",
-                "homozygosity", "gain", "phosphorylation"
-            }
-
-            if set(vname_lower.split()) & unable_to_normalize:
-                logger.warning("Variation Normalizer does not support "
-                               f"{variant_id}: {variant_query}")
+            if not self._is_supported_variant_query(variant_name, variant_id):
                 continue
 
-            variation_descriptor = await self.vicc_normalizers.normalize_variation(
+            vrs_variation = await self.vicc_normalizers.normalize_variation(
                 [variant_query]
             )
 
             # Couldn't find normalized concept
-            if not variation_descriptor:
-                logger.warning("Variation Normalizer unable to normalize "
-                               f"civic.vid:{variant['id']} using query "
-                               f"{variant_query}")
+            if not vrs_variation:
+                logger.debug(
+                    "Variation Normalizer unable to normalize %s using query %s",
+                    variant_id,
+                    variant_query,
+                )
                 continue
 
-            if variant["variant_types"]:
-                structural_type = variant["variant_types"][0]["so_id"]
-            else:
-                structural_type = None
+            # Create VRS Variation object
+            params = vrs_variation.model_dump(exclude_none=True)
+            params["label"] = variant["name"]
+            civic_variation = models.Variation(**params)
+
+            # Get expressions
+            hgvs_exprs = self._get_expressions(variant)
+            if hgvs_exprs:
+                civic_variation.root.expressions = hgvs_exprs
+
+            # Get members
+            members = await self._get_variation_members(variant)
+
+            # Get variant types
+            variant_types_value = []
+            for vt in variant["variant_types"]:
+                variant_types_value.append(
+                    core_models.Coding(
+                        code=vt["so_id"],
+                        system=f"{vt['url'].rsplit('/', 1)[0]}/",
+                        label="_".join(vt["name"].lower().split()),
+                    )
+                )
 
-            variation_descriptor = VariationDescriptor(
-                id=variant_id,
-                label=variant["name"],
-                variation_id=variation_descriptor.variation_id,
-                variation=variation_descriptor.variation,
-                gene_context=f"civic.gid:{variant['gene_id']}",
-                structural_type=structural_type,
-                expressions=hgvs_exprs,
-                xrefs=self._get_variant_xrefs(variant),
-                alternate_labels=[v_alias for v_alias in
-                                  variant["variant_aliases"] if not
-                                  v_alias.startswith("RS")],
-                extensions=self._get_variant_extensions(variant)
-            ).dict(by_alias=True, exclude_none=True)
-            self.valid_ids["variation_descriptors"][variant_id] = \
-                variation_descriptor
-            self.variation_descriptors.append(
-                variation_descriptor
-            )
-
-    def _get_variant_extensions(self, variant) -> list:
-        """Return a list of extensions for a variant.
-
-        :param dict variant: A CIViC variant record
-        :return: A list of extensions
-        """
-        return [
-            Extension(
-                name='civic_representative_coordinate',
-                value={k: v for k, v in variant['coordinates'].items()
-                       if v is not None}
-            ).dict(exclude_none=True)
-        ]
+            # Get mappings
+            mappings = [
+                core_models.Mapping(
+                    coding=core_models.Coding(
+                        code=str(variant["id"]),
+                        system="https://civicdb.org/variants/",
+                    ),
+                    relation=core_models.Relation.EXACT_MATCH,
+                )
+            ]
 
-    def _get_variant_xrefs(self, v) -> Optional[List[str]]:
-        """Return a list of xrefs for a variant.
+            if variant["allele_registry_id"]:
+                mappings.append(
+                    core_models.Mapping(
+                        coding=core_models.Coding(
+                            code=variant["allele_registry_id"],
+                            system="https://reg.clinicalgenome.org/",
+                        ),
+                        relation=core_models.Relation.RELATED_MATCH,
+                    )
+                )
 
-        :param dict v: A CIViC variant record
-        :return: A dictionary of xrefs
-        """
-        xrefs = []
-        for xref in ['clinvar_entries', 'allele_registry_id',
-                     'variant_aliases']:
-            if xref == 'clinvar_entries':
-                for clinvar_entry in v['clinvar_entries']:
-                    if clinvar_entry and clinvar_entry not in ['N/A',
-                                                               "NONE FOUND"]:
-                        xrefs.append(f"{schemas.XrefSystem.CLINVAR.value}:"
-                                     f"{clinvar_entry}")
-            elif xref == 'allele_registry_id' and v['allele_registry_id']:
-                xrefs.append(f"{schemas.XrefSystem.CLINGEN.value}:"
-                             f"{v['allele_registry_id']}")
-            elif xref == 'variant_aliases':
-                dbsnp_xrefs = [item for item in v['variant_aliases']
-                               if item.startswith('RS')]
-                for dbsnp_xref in dbsnp_xrefs:
-                    xrefs.append(f"{schemas.XrefSystem.DB_SNP.value}:"
-                                 f"{dbsnp_xref.split('RS')[-1]}")
-        return xrefs
-
-    def _get_hgvs_expr(self, variant) -> Optional[List[Dict[str, str]]]:
-        """Return a list of hgvs expressions for a given variant.
-
-        :param dict variant: A CIViC variant record
-        :return: A list of hgvs expressions
-        """
-        hgvs_expressions = list()
-        for hgvs_expr in variant['hgvs_expressions']:
-            if ':g.' in hgvs_expr:
-                syntax = 'hgvs.g'
-            elif ':c.' in hgvs_expr:
-                syntax = 'hgvs.c'
-            else:
-                syntax = 'hgvs.p'
-            if hgvs_expr != 'N/A':
-                hgvs_expressions.append(
-                    Expression(syntax=syntax,
-                               value=hgvs_expr).dict(exclude_none=True)
+            for ce in variant["clinvar_entries"]:
+                mappings.append(
+                    core_models.Mapping(
+                        coding=core_models.Coding(
+                            code=ce,
+                            system="https://www.ncbi.nlm.nih.gov/clinvar/variation/",
+                        ),
+                        relation=core_models.Relation.RELATED_MATCH,
+                    )
                 )
-        return hgvs_expressions
 
-    def _add_gene_descriptors(self, genes) -> None:
-        """Add Gene Descriptors to dict of transformations.
+            aliases = []
+            for a in variant["variant_aliases"]:
+                if SNP_RE.match(a):
+                    a = a.lower()
+                    mappings.append(
+                        core_models.Mapping(
+                            coding=core_models.Coding(
+                                code=a,
+                                system="https://www.ncbi.nlm.nih.gov/snp/",
+                            ),
+                            relation=core_models.Relation.RELATED_MATCH,
+                        )
+                    )
+                else:
+                    aliases.append(a)
+
+            if variant["coordinates"]:
+                coordinates = {
+                    k: v for k, v in variant["coordinates"].items() if v is not None
+                }
+            else:
+                coordinates = None
+
+            civic_variation_dict = civic_variation.model_dump(exclude_none=True)
+            self.variations.append(civic_variation_dict)
+            self.able_to_normalize["variations"][variant_id] = _VariationCache(
+                vrs_variation=civic_variation_dict,
+                civic_gene_id=f"civic.gid:{variant['gene_id']}",
+                variant_types=variant_types_value or None,
+                mappings=mappings or None,
+                aliases=aliases or None,
+                coordinates=coordinates or None,
+                members=members,
+            ).model_dump()
+
+    def _get_expressions(self, variant: Dict) -> List[models.Expression]:
+        """Get expressions for a given variant
+
+        :param variant: A CIViC variant record
+        :return: A list of expressions
+        """
+        expressions = []
+        for hgvs_expr in variant["hgvs_expressions"]:
+            if ":g." in hgvs_expr:
+                syntax = models.Syntax.HGVS_G
+            elif ":c." in hgvs_expr:
+                syntax = models.Syntax.HGVS_C
+            else:
+                syntax = models.Syntax.HGVS_P
+
+            if hgvs_expr != "N/A":
+                expressions.append(models.Expression(syntax=syntax, value=hgvs_expr))
+        return expressions
+
+    def _add_genes(self, genes: List[Dict]) -> None:
+        """Create gene objects for all CIViC gene records.
+        Mutates instance variables `able_to_normalize['genes']` and `genes`, if the
+        gene-normalizer can successfully normalize the gene
 
-        :param list genes: CIViC genes
+        :param genes: All genes in CIViC
         """
         for gene in genes:
             gene_id = f"civic.gid:{gene['id']}"
             ncbigene = f"ncbigene:{gene['entrez_id']}"
-            queries = [ncbigene, gene['name']] + gene['aliases']
+            queries = [ncbigene, gene["name"]] + gene["aliases"]
 
-            _, normalized_gene_id = \
-                self.vicc_normalizers.normalize_gene(queries)
+            _, normalized_gene_id = self.vicc_normalizers.normalize_gene(queries)
 
             if normalized_gene_id:
-                gene_descriptor = GeneDescriptor(
+                civic_gene = core_models.Gene(
                     id=gene_id,
-                    label=gene['name'],
-                    description=gene['description'] if gene['description'] else None,  # noqa: E501
-                    gene_id=normalized_gene_id,
-                    alternate_labels=gene['aliases'],
-                    xrefs=[ncbigene]
-                ).dict(exclude_none=True)
-                self.gene_descriptors.append(gene_descriptor)
-            else:
-                logger.warning(f"Gene Normalizer unable to normalize {gene_id}"
-                               f"using queries: {queries}")
-
-    def _add_disease_descriptor(self, disease_id, record) \
-            -> Optional[ValueObjectDescriptor]:
-        """Add disease ID to list of valid or invalid transformations.
-
-        :param str disease_id: The CIViC ID for the disease
-        :param dict record: CIViC AID or EID
-        :return: A disease descriptor
-        """
-        disease_descriptor = \
-            self.valid_ids['disease_descriptors'].get(disease_id)
-        if disease_descriptor:
-            return disease_descriptor
-        else:
-            disease_descriptor = None
-            if disease_id not in self.invalid_ids['disease_descriptors']:
-                disease_descriptor = \
-                    self._get_disease_descriptors(record['disease'])
-                if disease_descriptor:
-                    self.valid_ids['disease_descriptors'][disease_id] = \
-                        disease_descriptor
-                else:
-                    self.invalid_ids['disease_descriptors'].append(disease_id)
-            return disease_descriptor
+                    label=gene["name"],
+                    description=gene["description"] if gene["description"] else None,
+                    mappings=[
+                        core_models.Mapping(
+                            coding=core_models.Coding(
+                                code=f"ncbigene:{gene['entrez_id']}",
+                                system="https://www.ncbi.nlm.nih.gov/gene/",
+                            ),
+                            relation=core_models.Relation.EXACT_MATCH,
+                        )
+                    ],
+                    aliases=gene["aliases"] if gene["aliases"] else None,
+                    extensions=[
+                        core_models.Extension(
+                            name="gene_normalizer_id", value=normalized_gene_id
+                        )
+                    ],
+                ).model_dump(exclude_none=True)
+                self.able_to_normalize["genes"][gene_id] = civic_gene
+                self.genes.append(civic_gene)
+            else:
+                logger.debug(
+                    "Gene Normalizer unable to normalize %s using queries: %s",
+                    gene_id,
+                    queries,
+                )
 
-    def _get_disease_descriptors(self, disease) \
-            -> Optional[ValueObjectDescriptor]:
-        """Get a disease descriptor.
+    def _add_disease(self, disease: Dict) -> Optional[core_models.Disease]:
+        """Create or get disease given CIViC disease.
+        First looks in cache for existing disease, if not found will attempt to
+        normalize. Will add CIViC disease ID to `diseases` and
+        `able_to_normalize['diseases']` if disease-normalizer is able to normalize. Else
+        will add the CIViC disease ID to `unable_to_normalize['disease']`
 
-        :param dict disease: A CIViC disease record
-        :return: A Disease Descriptor
+        :param disease: CIViC Disease object
+        :return: Disease object if disease-normalizer was able to normalize
+        """
+        disease_id = f"civic.did:{disease['id']}"
+        vrs_disease = self.able_to_normalize["diseases"].get(disease_id)
+        if vrs_disease:
+            return vrs_disease
+        vrs_disease = None
+        if disease_id not in self.unable_to_normalize["diseases"]:
+            vrs_disease = self._get_disease(disease)
+            if vrs_disease:
+                self.able_to_normalize["diseases"][disease_id] = vrs_disease
+                self.diseases.append(vrs_disease)
+            else:
+                self.unable_to_normalize["diseases"].add(disease_id)
+        return vrs_disease
+
+    def _get_disease(self, disease: Dict) -> Optional[Dict]:
+        """Get core_models.Disease object for a CIViC disease
+
+        :param disease: CIViC disease record
+        :return: If able to normalize, core_models.Disease represented as a dict.
+            Otherwise, `None`
         """
-        if not disease:
-            return None
-
         disease_id = f"civic.did:{disease['id']}"
-        display_name = disease['display_name']
-        doid = disease['doid']
+        display_name = disease["display_name"]
+        doid = disease["doid"]
+        mappings = []
 
         if not doid:
-            logger.debug(f"{disease_id} ({display_name}) has null DOID")
+            logger.debug("%s (%s) has null DOID", disease_id, display_name)
             queries = [display_name]
-            xrefs = []
         else:
             doid = f"DOID:{doid}"
             queries = [doid, display_name]
-            xrefs = [doid]
+            mappings.append(
+                core_models.Mapping(
+                    coding=core_models.Coding(
+                        code=doid,
+                        system="https://www.disease-ontology.org/",
+                    ),
+                    relation=core_models.Relation.EXACT_MATCH,
+                )
+            )
 
-        _, normalized_disease_id = \
-            self.vicc_normalizers.normalize_disease(queries)
+        (
+            disease_norm_resp,
+            normalized_disease_id,
+        ) = self.vicc_normalizers.normalize_disease(queries)
 
         if not normalized_disease_id:
-            logger.warning(f"Disease Normalizer unable to normalize: "
-                           f"{disease_id} using queries {queries}")
+            logger.debug(
+                "Disease Normalizer unable to normalize: %s using queries %s",
+                disease_id,
+                queries,
+            )
             return None
 
-        disease_descriptor = ValueObjectDescriptor(
+        return core_models.Disease(
             id=disease_id,
-            type="DiseaseDescriptor",
             label=display_name,
-            disease_id=normalized_disease_id,
-            xrefs=xrefs if xrefs else None
-        ).dict(exclude_none=True)
-        return disease_descriptor
-
-    def _add_therapy_descriptor(self, therapy_id, record)\
-            -> Optional[ValueObjectDescriptor]:
-        """Add therapy ID to list of valid or invalid transformations.
-
-        :param str therapy_id: The CIViC ID for the drug
-        :param dict record: CIViC AID or EID
-        :return: A therapy descriptor
-        """
-        therapy_descriptor = \
-            self.valid_ids['therapy_descriptors'].get(therapy_id)
-        if therapy_descriptor:
-            return therapy_descriptor
+            mappings=mappings if mappings else None,
+            extensions=[
+                self._get_disease_normalizer_ext_data(
+                    normalized_disease_id, disease_norm_resp
+                ),
+            ],
+        ).model_dump(exclude_none=True)
+
+    def _get_therapeutic_substitute_group(
+        self,
+        therapeutic_sub_group_id: str,
+        therapies: List[Dict],
+        therapy_interaction_type: str,
+    ) -> Optional[core_models.TherapeuticSubstituteGroup]:
+        """Get Therapeutic Substitute Group for CIViC therapies
+
+        :param therapeutic_sub_group_id: ID for Therapeutic Substitute Group
+        :param therapies: List of CIViC therapy objects
+        :param therapy_interaction_type: Therapy interaction type provided by CIViC
+        :return: If able to normalize all therapy objects in `therapies`, returns
+            Therapeutic Substitute Group represented as a dict
+        """
+        substitutes = []
+
+        for therapy in therapies:
+            therapeutic_procedure_id = f"civic.tid:{therapy['id']}"
+            ta = self._add_therapeutic_procedure(
+                therapeutic_procedure_id,
+                [therapy],
+                TherapeuticProcedureType.THERAPEUTIC_AGENT,
+            )
+            if not ta:
+                return None
+
+            substitutes.append(ta)
+
+        extensions = [
+            core_models.Extension(
+                name="civic_therapy_interaction_type", value=therapy_interaction_type
+            ).model_dump(exclude_none=True)
+        ]
+
+        try:
+            tsg = core_models.TherapeuticSubstituteGroup(
+                id=therapeutic_sub_group_id,
+                substitutes=substitutes,
+                extensions=extensions,
+            ).model_dump(exclude_none=True)
+        except ValidationError as e:
+            # If substitutes validation checks fail
+            logger.debug(
+                "ValidationError raised when attempting to create TherapeuticSubstituteGroup: %s",
+                {e},
+            )
+            tsg = None
+
+        return tsg
+
+    def _get_therapeutic_agent(
+        self, therapy: Dict
+    ) -> Optional[core_models.TherapeuticAgent]:
+        """Get Therapeutic Agent for CIViC therapy
+
+        :param therapy: CIViC therapy object
+        :return: If able to normalize therapy, returns therapeutic agent represented as
+            a dict
+        """
+        therapy_id = f"civic.tid:{therapy['id']}"
+        label = therapy["name"]
+        ncit_id = therapy["ncit_id"]
+        mappings = []
+        if ncit_id:
+            queries = [f"ncit:{ncit_id}", label]
+            mappings.append(
+                core_models.Mapping(
+                    coding=core_models.Coding(
+                        code=ncit_id,
+                        system="https://ncit.nci.nih.gov/ncitbrowser/ConceptReport.jsp?dictionary=NCI_Thesaurus&code=",
+                    ),
+                    relation=core_models.Relation.EXACT_MATCH,
+                )
+            )
         else:
-            therapy_descriptor = None
-            if therapy_id not in self.invalid_ids['therapy_descriptors']:
-                therapy_descriptor = \
-                    self._get_therapy_descriptor(record["therapies"][0])
-                if therapy_descriptor:
-                    self.valid_ids['therapy_descriptors'][therapy_id] = \
-                        therapy_descriptor
-                else:
-                    self.invalid_ids['therapy_descriptors'].append(therapy_id)
-            return therapy_descriptor
+            queries = [label]
 
-    def _get_therapy_descriptor(self, drug) \
-            -> Optional[ValueObjectDescriptor]:
-        """Get a therapy descriptor.
-
-        :param dict drug: A CIViC drug record
-        :return: A Therapy Descriptor
-        """
-        therapy_id = f"civic.tid:{drug['id']}"
-        label = drug['name']
-        ncit_id = f"ncit:{drug['ncit_id']}"
-        queries = [ncit_id, label]
-
-        therapy_norm_resp, normalized_therapy_id = \
-            self.vicc_normalizers.normalize_therapy(queries)
-
-        if not normalized_therapy_id:
-            logger.warning(f"Therapy Normalizer unable to normalize: "
-                           f"using queries {ncit_id} and {label}")
+        (
+            therapy_norm_resp,
+            normalized_therapeutic_id,
+        ) = self.vicc_normalizers.normalize_therapy(queries)
+
+        if not normalized_therapeutic_id:
+            logger.debug(
+                "Therapy Normalizer unable to normalize: using queries ncit:%s and %s",
+                ncit_id,
+                label,
+            )
             return None
 
-        regulatory_approval_extension = \
+        regulatory_approval_extension = (
             self.vicc_normalizers.get_regulatory_approval_extension(therapy_norm_resp)
+        )
 
-        therapy_descriptor = ValueObjectDescriptor(
-            id=therapy_id,
-            type="TherapyDescriptor",
-            label=label,
-            therapy_id=normalized_therapy_id,
-            alternate_labels=drug['aliases'],
-            xrefs=[ncit_id],
-            extensions=[regulatory_approval_extension] if regulatory_approval_extension else None  # noqa: E501
-        ).dict(exclude_none=True)
-        return therapy_descriptor
-
-    def _add_methods(self) -> None:
-        """Add methods to list of transformations."""
-        self.methods = [
-            schemas.Method(
-                id=f'method:'
-                   f'{schemas.MethodID.CIVIC_EID_SOP}',
-                label='Standard operating procedure for curation and clinical'
-                      ' interpretation of variants in cancer',
-                url='https://genomemedicine.biomedcentral.com/articles/'
-                    '10.1186/s13073-019-0687-x',
-                version=schemas.Date(year=2019, month=11, day=29).dict(),
-                authors='Danos, A.M., Krysiak, K., Barnell, E.K. et al.'
-            ).dict(exclude_none=True),
-            schemas.Method(
-                id=f'method:'
-                   f'{schemas.MethodID.CIVIC_AID_AMP_ASCO_CAP.value}',
-                label='Standards and Guidelines for the '
-                      'Interpretation and Reporting of Sequence '
-                      'Variants in Cancer: A Joint Consensus '
-                      'Recommendation of the Association '
-                      'for Molecular Pathology, American Society of '
-                      'Clinical Oncology, and College of American '
-                      'Pathologists',
-                url='https://pubmed.ncbi.nlm.nih.gov/27993330/',
-                version=schemas.Date(year=2017,
-                                     month=1).dict(exclude_none=True),
-                authors='Li MM, Datto M, Duncavage EJ, et al.'
-            ).dict(exclude_none=True),
-            schemas.Method(
-                id=f'method:'
-                   f'{schemas.MethodID.CIVIC_AID_ACMG.value}',
-                label='Standards and guidelines for the '
-                      'interpretation of sequence variants: a '
-                      'joint consensus recommendation of the '
-                      'American College of Medical Genetics and'
-                      ' Genomics and the Association for '
-                      'Molecular Pathology',
-                url='https://pubmed.ncbi.nlm.nih.gov/25741868/',
-                version=schemas.Date(year=2015,
-                                     month=5).dict(exclude_none=True),
-                authors='Richards S, Aziz N, Bale S, et al.'
-            ).dict(exclude_none=True)
+        extensions = [
+            self._get_therapy_normalizer_ext_data(
+                normalized_therapeutic_id, therapy_norm_resp
+            ),
         ]
 
-    def _get_eid_document(self, source) -> Optional[schemas.Document]:
-        """Get an EID's document.
+        if regulatory_approval_extension:
+            extensions.append(regulatory_approval_extension)
 
-        :param dict source: An evidence item's source
-        :return: Document for EID
-        """
-        source_type = source['source_type'].upper()
-        if source_type in schemas.SourcePrefix.__members__:
-            prefix = schemas.SourcePrefix[source_type].value
-            document_id = f"{prefix}:{source['citation_id']}"
-            xrefs = []
-            if source['asco_abstract_id']:
-                xrefs.append(f"asco.abstract:{source['asco_abstract_id']}")
-            if source['pmc_id']:
-                xrefs.append(f"pmc:{source['pmc_id']}")
-
-            document = schemas.Document(
-                id=document_id,
-                label=source['citation'],
-                description=source["title"],
-                xrefs=xrefs if xrefs else None
-            ).dict(exclude_none=True)
-            return document
-        else:
-            logger.warning(f"{source_type} not in schemas.SourcePrefix")
+        return core_models.TherapeuticAgent(
+            id=therapy_id,
+            label=label,
+            mappings=mappings if mappings else None,
+            aliases=therapy["aliases"] if therapy["aliases"] else None,
+            extensions=extensions,
+        ).model_dump(exclude_none=True)
+
+    def _add_eid_document(self, source: Dict) -> Optional[Document]:
+        """Create document object for CIViC source
+        Mutates instance variable `documents`
+
+        :param source: An evidence item's source
+        :return: Document for Evidence Item if source type is supported
+        """
+        source_type = source["source_type"].upper()
+        source_id = source["id"]
+        if source_type in SourcePrefix.__members__:
+            document = Document(
+                id=f"civic.source:{source_id}",
+                label=source["citation"],
+                title=source["title"],
+            ).model_dump(exclude_none=True)
 
-    def _get_aid_document(self, assertion: Dict) -> List[schemas.Document]:
-        """Get an AID's documents.
+            if source["source_type"] == SourcePrefix.PUBMED:
+                document["pmid"] = int(source["citation_id"])
 
-        :param dict assertion: A CIViC Assertion
-        :return: A list of AID documents
-        """
-        # NCCN Guidlines
-        documents = list()
-        nccn_guideline = assertion["nccn_guideline"] or dict()
-        label = nccn_guideline.get("name")
-        version = assertion["nccn_guideline_version"]
-        if label and version:
-            doc_id = "https://www.nccn.org/professionals/physician_gls/default.aspx"  # noqa: E501
-            doc_label = f"NCCN Guidelines: {label} version {version}"
-            db_id = self._get_document_id(document_id=doc_id, label=doc_label)
-            documents = list()
-            documents.append(schemas.Document(
-                id=db_id,
-                document_id=doc_id,
-                label=doc_label
-            ).dict(exclude_none=True))
-
-        # TODO: Check this after first pass
-        # ACMG Codes
-        if assertion['acmg_codes']:
-            for acmg_code in assertion['acmg_codes']:
-                document_id = f"acmg:{acmg_code['code']}"
-                documents.append(schemas.Document(
-                    id=document_id,
-                    label=acmg_code['code'],
-                    description=acmg_code['description']
-                ).dict(exclude_none=True))
+            if document not in self.documents:
+                self.documents.append(document)
+        else:
+            logger.warning(
+                "Document, %s, not supported. %s not in SourcePrefix",
+                source_id,
+                source_type,
+            )
+            document = None
 
-        return documents
+        return document
```

### Comparing `metakb-1.2.0.dev0/metakb/transform/oncokb.py` & `metakb-2.0.0.dev0/src/metakb/transform/moa.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,483 +1,590 @@
-"""A module for transforming OncoKB to common data model (CDM)"""
-from typing import Optional, Dict, List
+"""A module to convert MOA resources to common data model"""
+
+import json
+import logging
 from pathlib import Path
+from typing import Dict, List, Optional
 from urllib.parse import quote
-from copy import deepcopy
-import logging
 
-from ga4gh.vrsatile.pydantic.vrsatile_models import VariationDescriptor, \
-    Extension, GeneDescriptor, ValueObjectDescriptor
+from ga4gh.core import core_models, sha512t24u
+from ga4gh.vrs import models
 
 from metakb import APP_ROOT
-from metakb.normalizers import VICCNormalizers
-from metakb.transform.base import Transform
-from metakb.schemas import Date, DiagnosticPredicate, Document, Method, MethodID, \
-    Predicate, PredictivePredicate, PropositionType, Statement
-
-
-logger = logging.getLogger("metakb.transform.oncokb")
-logger.setLevel(logging.DEBUG)
-
-
-# OncoKB gene fields (oncokb_label, ext_label)
-GENE_EXT_CONVERSIONS = [
-    ("grch37Isoform", "ensembl_transcript_GRCh37"),
-    ("grch37RefSeq", "refseq_transcript_GRCh37"),
-    ("grch38Isoform", "ensembl_transcript_GRCh38"),
-    ("grch38RefSeq", "refseq_transcript_GRCh38"),
-    ("oncogene", "oncogene"),
-    ("highestSensitiveLevel", "oncokb_highest_sensitive_level"),
-    ("highestResistanceLevel", "oncokb_highest_resistance_level"),
-    ("background", "oncokb_background"),
-    ("tsg", "tumor_suppressor_gene")
-]
-
-
-# OncoKB variation fields (oncokb_label, ext_label)
-VARIATION_EXT_CONVERSIONS = [
-    ("oncogenic", "oncogenic"),
-    ("mutationEffect", "mutation_effect"),
-    ("hotspot", "hotspot"),
-    ("vus", "vus"),
-    ("highestSensitiveLevel", "oncokb_highest_sensitive_level"),
-    ("highestResistanceLevel", "oncokb_highest_resistance_level"),
-    ("highestDiagnosticImplicationLevel", "oncokb_highest_diagnostic_implication_level"),  # noqa: E501
-    ("highestPrognosticImplicationLevel", "oncokb_highest_prognostic_implication_level"),  # noqa: E501
-    ("highestFdaLevel", "oncokb_highest_fda_level"),
-    ("alleleExist", "allele_exist")
-]
-
-
-# OncoKB disease fields (oncokb_label, ext_label)
-DISEASE_EXT_CONVERSIONS = [
-    ("mainType", "oncotree_main_type"),
-    ("tissue", "tissue"),
-    ("children", "children"),
-    ("parent", "parent"),
-    ("level", "level"),
-    ("tumorForm", "tumor_form")
-]
+from metakb.normalizers import ViccNormalizers
+from metakb.schemas.annotation import Direction, Document
+from metakb.schemas.categorical_variation import ProteinSequenceConsequence
+from metakb.schemas.variation_statement import (
+    AlleleOrigin,
+    VariantTherapeuticResponseStudy,
+    VariantTherapeuticResponseStudyPredicate,
+    _VariantOncogenicityStudyQualifier,
+)
+from metakb.transform.base import (
+    MethodId,
+    MoaEvidenceLevel,
+    TherapeuticProcedureType,
+    Transform,
+)
 
+logger = logging.getLogger(__name__)
 
-class OncoKBTransform(Transform):
-    """A class for transforming OncoKB to the common data model."""
 
-    method = f"method:{MethodID.ONCOKB_SOP}"
+class MoaTransform(Transform):
+    """A class for transforming MOA resources to common data model."""
 
     def __init__(
-        self, data_dir: Path = APP_ROOT / "data", harvester_path: Optional[Path] = None,
-        normalizers: Optional[VICCNormalizers] = None
+        self,
+        data_dir: Path = APP_ROOT / "data",
+        harvester_path: Optional[Path] = None,
+        normalizers: Optional[ViccNormalizers] = None,
     ) -> None:
-        """Initialize OncoKB Transform class.
+        """Initialize MOAlmanac Transform class.
 
-        :param Path data_dir: Path to source data directory
-        :param Optional[Path] harvester_path: Path to previously harvested data
-        :param VICCNormalizers normalizers: normalizer collection instance
-        """
-        super().__init__(data_dir, harvester_path, normalizers)
-        # Able to normalize these IDSs
-        self.valid_ids = {
-            "disease_descriptors": dict(),
-            "therapy_descriptors": dict()
-        }
-        # Unable to normalize these IDs
-        self.invalid_ids = {
-            "therapy_descriptors": set(),
-            "disease_descriptors": set()
+        :param data_dir: Path to source data directory
+        :param harvester_path: Path to previously harvested MOA data
+        :param normalizers: normalizer collection instance
+        """
+        super().__init__(
+            data_dir=data_dir, harvester_path=harvester_path, normalizers=normalizers
+        )
+
+        # Method will always be the same
+        self.methods = [self.methods_mapping[MethodId.MOA_ASSERTION_BIORXIV.value]]
+
+        # Cache for normalized concepts. The key is the concept type and value is a
+        # dictionary of mappings from MOA concept (key) to transformed concept (value)
+        self.able_to_normalize = {
+            "variations": {},
+            "diseases": {},
+            "therapeutics": {},
+            "genes": {},
+            "documents": {},
         }
 
-        self.methods = [
-            Method(id=f"method:{MethodID.ONCOKB_SOP}",
-                   label="OncoKB Curation Standard Operating Procedure",
-                   url="https://sop.oncokb.org/",
-                   version=Date(year=2021, month=11).dict(),
-                   authors="OncoKB").dict(exclude_none=True)
-        ]
-
     async def transform(self) -> None:
-        """Transform OncoKB harvested JSON to common data model. Will update instance
-        variables (statements, propositions, variation_descriptors, gene_descriptors,
-        therapy_descriptors, disease_descriptors, documents) with transformed data from
-        OncoKB.
+        """Transform MOA harvested JSON to common data model. Will store transformed
+        results in instance variables.
         """
         data = self.extract_harvester()
-        variants_data = data["variants"]
-        genes_data = data["genes"]
-        levels = data["levels"]
-
-        self.sensitive_levels = levels["sensitive"]
-        self.resistance_levels = levels["resistance"]
-        self.fda_levels = levels["fda"]
-
-        self._add_gene_descriptors(genes_data)
-        await self._transform_evidence(variants_data)
-
-    async def _transform_evidence(self, variants_data: List[Dict]) -> None:
-        """Transform OncoKB evidence to common data model. Will update instance
-        variables (statements, propositions, variation_descriptors, gene_descriptors,
-        therapy_descriptors, disease_descriptors, documents) with transformed data from
-        OncoKB.
-
-        :param List[Dict] variants_data: Variants data from OncoKB. Contains variant
-            and associated evidence data.
-        """
-        for data in variants_data:
-            # Exclude trying on variants we know we can't normalize
-            unable_to_normalize_variant = {
-                "fusion", "fusions", "mutation", "mutations", "tandem", "domain",
-                "splice", "deletion", "hypermethylation", "silencing", "overexpression"
-            }
 
-            alt = data["query"]["alteration"]
-            if set(alt.lower().split()) & unable_to_normalize_variant:
-                logger.debug(f"Variation Normalizer does not support: {alt}")
+        # Add gene, variant, and source data to instance variables (`genes`,
+        # `variations`, and `documents`)
+        self._add_genes(data["genes"])
+        await self._add_protein_consequences(data["variants"])
+        self._add_documents(data["sources"])
+
+        # Add variant therapeutic response study data. Will update `studies`
+        await self._add_variant_therapeutic_response_studies(data["assertions"])
+
+    async def _add_variant_therapeutic_response_studies(
+        self, assertions: List[Dict]
+    ) -> None:
+        """Create Variant Therapeutic Response Studies from MOA assertions.
+        Will add associated values to instances variables (`therapeutics`, `diseases`,
+        and `studies`). `able_to_normalize` and `unable_to_normalize` will also be
+        mutated for associated therapeutics and diseases.
+
+        :param assertions: A list of MOA assertion records
+        """
+        for record in assertions:
+            assertion_id = f"moa.assertion:{record['id']}"
+            variant_id = record["variant"]["id"]
+
+            # Check cache for variation record (which contains gene information)
+            variation_gene_map = self.able_to_normalize["variations"].get(variant_id)
+            if not variation_gene_map:
+                logger.debug(
+                    "%s has no variation for variant_id %s", assertion_id, variant_id
+                )
                 continue
 
-            variation_descriptor = await self._add_variation_descriptor(data)
-            if not variation_descriptor:
+            # Get predicate. We only support therapeutic resistance/sensitivity
+            if record["clinical_significance"] == "resistance":
+                predicate = (
+                    VariantTherapeuticResponseStudyPredicate.PREDICTS_RESISTANCE_TO
+                )
+            elif record["clinical_significance"] == "sensitivity":
+                predicate = (
+                    VariantTherapeuticResponseStudyPredicate.PREDICTS_SENSITIVITY_TO
+                )
+            else:
+                logger.debug(
+                    "clinical_significance not supported: %s",
+                    record["clinical_significance"],
+                )
                 continue
 
-            # We skip prognostic evidence (prognosticImplications) since there is not
-            # enough information
+            # Get strength
+            predictive_implication = (
+                record["predictive_implication"]
+                .strip()
+                .replace(" ", "_")
+                .replace("-", "_")
+                .upper()
+            )
+            moa_evidence_level = MoaEvidenceLevel[predictive_implication]
+            strength = self.evidence_level_to_vicc_concept_mapping[moa_evidence_level]
+
+            # Add therapeutic agent. We only support one therapy, so we will skip others
+            therapy_name = record["therapy_name"]
+            if not therapy_name:
+                logger.debug("%s has no therapy_name", assertion_id)
+                continue
 
-            for diagnostic_imp in data["diagnosticImplications"]:
-                # Diagnostic evidence is all inclusive
-                self._add_diagnostic_evidence(diagnostic_imp, variation_descriptor)
-
-            for treatment in data["treatments"]:
-                # Therapeutic evidence
-                # Only support where only one drug
-                if len(treatment["drugs"]) != 1:
+            therapy_interaction_type = record["therapy_type"]
+
+            if "+" in therapy_name:
+                # Indicates multiple therapies
+                if therapy_interaction_type.upper() in {
+                    "COMBINATION THERAPY",
+                    "IMMUNOTHERAPY",
+                    "RADIATION THERAPY",
+                    "TARGETED THERAPY",
+                }:
+                    therapeutic_procedure_type = (
+                        TherapeuticProcedureType.COMBINATION_THERAPY
+                    )
+                else:
+                    # skipping HORMONE and CHEMOTHERAPY for now
                     continue
 
-                self._add_therapeutic_evidence(treatment, variation_descriptor)
+                therapies = [tn.strip() for tn in therapy_name.split("+")]
+                therapeutic_digest = self._get_digest_for_str_lists(
+                    [f"moa.therapy:{tn}" for tn in therapies]
+                )
+                therapeutic_procedure_id = f"moa.ctid:{therapeutic_digest}"
+            else:
+                therapeutic_procedure_id = f"moa.therapy:{therapy_name}"
+                therapies = [therapy_name]
+                therapeutic_procedure_type = TherapeuticProcedureType.THERAPEUTIC_AGENT
+
+            moa_therapeutic = self._add_therapeutic_procedure(
+                therapeutic_procedure_id,
+                therapies,
+                therapeutic_procedure_type,
+                therapy_interaction_type,
+            )
+
+            if not moa_therapeutic:
+                logger.debug(
+                    "%s has no therapeutic agent for therapy_name %s",
+                    assertion_id,
+                    therapy_name,
+                )
+                continue
 
-    def _add_evidence(
-        self, evidence_data: Dict, proposition_type: PropositionType, level: str,
-        predicate: Predicate, disease_data: Dict, variation_descriptor: Dict,
-        extensions: Optional[List] = None, therapy_descriptor: Optional[Dict] = None
-    ) -> None:
-        """Add transformed oncokb evidence as statements
-        Will update instance variables (disease_descriptors, proposition, documents,
-        statements)
-
-        :param Dict evidence_data: OncoKB evidence data
-        :param PropositionType proposition_type: Proposition type of `evidence_data`
-        :param str level: OncoKB level of `evidence_data`
-        :param Predicate predicate: Predicate of `evidence_data`
-        :param Dict disease_data: Disease data for `evidence_data`
-        :param Dict variation_descriptor: Variation descriptor associated to
-            `evidence_data`
-        :param Optional[List] extensions: List of extensions for `evidence_data`
-        :param Optional[Dict] therapy_descriptor: Therapy descriptor associated to
-            `evidence_data`. Only for therapeutic evidence.
-        """
-        disease_descriptor = self._add_disease_descriptor(disease_data)
-        if not disease_descriptor:
-            return None
+            # Add disease
+            moa_disease = self._add_disease(record["disease"])
+            if not moa_disease:
+                logger.debug(
+                    "%s has no disease for disease %s", assertion_id, record["disease"]
+                )
+                continue
 
-        proposition = self._get_proposition(
-            proposition_type, predicate, variation_descriptor["variation_id"],
-            disease_descriptor["disease_id"],
-            therapy_descriptor["therapy_id"] if therapy_descriptor else None)
-        if proposition:
-            documents = self._get_documents(evidence_data["pmids"])
-            description = evidence_data["description"]
-
-            statement_params = {
-                "description": description if description else None,
-                "evidence_level": f"oncokb.evidence_level:{level}",
-                "proposition": proposition["id"],
-                "variation_descriptor": variation_descriptor["id"],
-                "disease_descriptor": disease_descriptor["id"],
-                "therapy_descriptor": therapy_descriptor["id"] if therapy_descriptor else None,  # noqa: E501
-                "method": self.methods[0]["id"],
-                "supported_by": [d["id"] for d in documents],
-                "extensions": extensions
-            }
-            digest = self._generate_digest(statement_params)
-            statement_params["id"] = f"oncokb.evidence:{digest}"
-            statement = Statement(
-                **statement_params).dict(by_alias=True, exclude_none=True)
-            self.statements.append(statement)
-
-    def _add_diagnostic_evidence(self, diagnostic_implication: Dict,
-                                 variation_descriptor: Dict) -> None:
-        """Transform OncoKB Diagnostic Evidence to common data model. Will update
-        instance variables (statements, propositions, variation_descriptors,
-        gene_descriptors, therapy_descriptors, disease_descriptors, documents) with
-        transformed data from OncoKB.
-
-        :param Dict diagnostic_implication: Diagnostic evidence
-        :param Dict variation_descriptor: Variation Descriptor associated to diagnostic
-            evidence
-        """
-        predicate = DiagnosticPredicate.POSITIVE
-        proposition_type = PropositionType.DIAGNOSTIC
-        level = diagnostic_implication["levelOfEvidence"]
-        disease_data = diagnostic_implication["tumorType"]
-        self._add_evidence(diagnostic_implication, proposition_type, level, predicate,
-                           disease_data, variation_descriptor)
-
-    def _add_therapeutic_evidence(self, treatment: Dict,
-                                  variation_descriptor: Dict) -> None:
-        """Transform OncoKB Therapeutic Evidence to common data model. Will update
-        instance variables (statements, propositions, variation_descriptors,
-        gene_descriptors, therapy_descriptors, disease_descriptors, documents) with
-        transformed data from OncoKB.
-
-        :param Dict treatment: Therapeutic evidence
-        :param Dict variation_descriptor: Variation Descriptor associated to therapeutic
-            evidence
-        """
-        level = treatment["level"]
-        proposition_type = PropositionType.PREDICTIVE
-        predicate = None
-        if level in self.sensitive_levels:
-            predicate = PredictivePredicate.SENSITIVITY
-        elif level in self.resistance_levels:
-            predicate = PredictivePredicate.RESISTANCE
+            # Add document
+            document = self.able_to_normalize["documents"].get(record["source_ids"])
+
+            # Get qualifier
+            gene = variation_gene_map["moa_gene"]
+            qualifiers = self._get_variant_onco_study_qualifier(
+                record["variant"]["feature_type"], gene
+            )
+
+            statement = VariantTherapeuticResponseStudy(
+                direction=Direction.NONE,
+                id=assertion_id,
+                description=record["description"],
+                strength=strength,
+                predicate=predicate,
+                variant=variation_gene_map["psc"],
+                therapeutic=moa_therapeutic,
+                tumorType=moa_disease,
+                qualifiers=qualifiers,
+                specifiedBy=self.methods[0],
+                isReportedIn=[document],
+            ).model_dump(exclude_none=True)
+            self.studies.append(statement)
+
+    def _get_variant_onco_study_qualifier(
+        self, feature_type: str, gene: Optional[core_models.Gene] = None
+    ) -> Optional[_VariantOncogenicityStudyQualifier]:
+        """Get Variant Oncogenicity Study Qualifier
+
+        :param feature_type: MOA feature type
+        :param gene: MOA gene data
+        :return: Variant Oncogenicity Study Qualifier for a Variant Therapeutic Response
+            Study, if allele origin or gene exists
+        """
+        if feature_type == "somatic_variant":
+            allele_origin = AlleleOrigin.SOMATIC
+        elif feature_type == "germline_variant":
+            allele_origin = AlleleOrigin.GERMLINE
         else:
-            # This shouldn't happen, but adding a check just in case
-            logger.warning(f"Level {level} not in Sensitive or Resistance level")
-            return None
+            allele_origin = None
 
-        therapy_descriptor = self._add_therapy_descriptor(treatment["drugs"])
-        if not therapy_descriptor:
-            return None
+        if allele_origin or gene:
+            qualifier = _VariantOncogenicityStudyQualifier(
+                alleleOrigin=allele_origin, geneContext=gene
+            )
+        else:
+            qualifier = None
+        return qualifier
 
-        disease_data = treatment["levelAssociatedCancerType"]
+    async def _add_protein_consequences(self, variants: List[Dict]) -> None:
+        """Create Protein Sequence Consequence objects for all MOA variant records.
+        Mutates instance variables `able_to_normalize['variations']` and
+        `variations`, if the variation-normalizer can successfully normalize the variant
+
+        :param variants: All variants in MOAlmanac
+        """
+        for variant in variants:
+            variant_id = variant["id"]
+            moa_variant_id = f"moa.variant:{variant_id}"
+            feature = variant["feature"]
+            # Skipping Fusion + Translocation + rearrangements that variation normalizer
+            # does not support
+            if "rearrangement_type" in variant:
+                logger.debug(
+                    "Variation Normalizer does not support %s: %s",
+                    moa_variant_id,
+                    feature,
+                )
+                continue
 
-        extensions = list()
-        fda_level = treatment["fdaLevel"]
-        if fda_level:
-            ext_value = {
-                "level": fda_level,
-                "description": self.fda_levels[fda_level]
+            # Gene is required to form query
+            gene = variant.get("gene")
+            if not gene:
+                logger.debug(
+                    "Variation Normalizer does not support %s: %s (no gene provided)",
+                    moa_variant_id,
+                    feature,
+                )
+                continue
 
-            }
-            extensions.append(Extension(name="onckb_fda_level", value=ext_value).dict())
+            moa_gene = self.able_to_normalize["genes"].get(quote(gene))
+            if not moa_gene:
+                logger.debug(
+                    "moa.variant:%s has no gene for gene, %s", variant_id, gene
+                )
+                continue
+
+            # Form query and run through variation-normalizer
+            # For now, the normalizer only support amino acid substitution
+            vrs_variation = None
+            if variant.get("protein_change"):
+                gene = moa_gene["label"]
+                query = f"{gene} {variant['protein_change'][2:]}"
+                vrs_variation = await self.vicc_normalizers.normalize_variation([query])
+
+                if not vrs_variation:
+                    logger.debug(
+                        "Variation Normalizer unable to normalize: moa.variant: %s using query: %s",
+                        variant_id,
+                        query,
+                    )
+                    continue
+            else:
+                logger.debug(
+                    "Variation Normalizer does not support %s: %s",
+                    moa_variant_id,
+                    feature,
+                )
+                continue
 
-        self._add_evidence(treatment, proposition_type, level, predicate, disease_data,
-                           variation_descriptor, extensions, therapy_descriptor)
+            # Create VRS Variation object
+            params = vrs_variation.model_dump(exclude_none=True)
+            moa_variant_id = f"moa.variant:{variant_id}"
+            params["id"] = vrs_variation.id
+            moa_variation = models.Variation(**params)
+
+            # Add MOA representative coordinate data to extensions
+            coordinates_keys = [
+                "chromosome",
+                "start_position",
+                "end_position",
+                "reference_allele",
+                "alternate_allele",
+                "cdna_change",
+                "protein_change",
+                "exon",
+            ]
+            moa_rep_coord = {k: variant.get(k) for k in coordinates_keys}
+            extensions = [
+                core_models.Extension(
+                    name="MOA representative coordinate", value=moa_rep_coord
+                )
+            ]
+            members = await self._get_variation_members(moa_rep_coord)
+
+            # Add mappings data
+            mappings = [
+                core_models.Mapping(
+                    coding=core_models.Coding(
+                        code=str(variant_id),
+                        system="https://moalmanac.org/api/features/",
+                    ),
+                    relation=core_models.Relation.EXACT_MATCH,
+                )
+            ]
+
+            if variant["rsid"]:
+                mappings.append(
+                    core_models.Mapping(
+                        coding=core_models.Coding(
+                            code=variant["rsid"],
+                            system="https://www.ncbi.nlm.nih.gov/snp/",
+                        ),
+                        relation=core_models.Relation.RELATED_MATCH,
+                    )
+                )
+
+            psc = ProteinSequenceConsequence(
+                id=moa_variant_id,
+                label=feature,
+                definingContext=moa_variation.root,
+                mappings=mappings or None,
+                extensions=extensions,
+                members=members,
+            ).model_dump(exclude_none=True)
+
+            self.able_to_normalize["variations"][variant_id] = {
+                "psc": psc,
+                "moa_gene": moa_gene,
+            }
+            self.variations.append(psc)
 
-    def _add_therapy_descriptor(self, drugs_data: List[Dict]) -> Optional[Dict]:
-        """Get therapy descriptor
-        The `therapy_descriptor` instance variable will be updated if therapy normalizer
-        was able to normalize the drug and if the drug does not already have a therapy
-        descriptor.
-
-        :param List[Dict] drugs_data: List of drugs. For now, `drugs_data` will always
-            have a length of one.
-        :return: Therapy descriptor represented as a dictionary if therapy normalizer
-            was able to normalize the drug
-        """
-        # Since we only support 1 therapeutic we can get the first element
-        drug = drugs_data[0]
-        ncit_code = drug["ncitCode"]
-        if ncit_code in self.valid_ids["therapy_descriptors"]:
-            therapy_descriptor = self.valid_ids["therapy_descriptors"][ncit_code]
+    async def _get_variation_members(
+        self, moa_rep_coord: Dict
+    ) -> Optional[List[models.Variation]]:
+        """Get members field for variation object. This is the related variant concepts.
+        FOr now, only looks at genomic representative coordinate.
+
+        :param moa_rep_coord: MOA Representative Coordinate
+        :return: List containing one VRS variation record for associated genomic
+            representation, if variation-normalizer was able to successfully normalize
+        """
+        members = None
+        chromosome = moa_rep_coord.get("chromosome")
+        pos = moa_rep_coord.get("start_position")
+        ref = moa_rep_coord.get("reference_allele")
+        alt = moa_rep_coord.get("alternate_allele")
+
+        if all((chromosome, pos is not None, ref and ref != "-", alt and alt != "-")):
+            gnomad_vcf = f"{chromosome}-{pos}-{ref}-{alt}"
+
+            vrs_genomic_variation = await self.vicc_normalizers.normalize_variation(
+                [gnomad_vcf]
+            )
+
+            if vrs_genomic_variation:
+                genomic_params = vrs_genomic_variation.model_dump(exclude_none=True)
+                genomic_params["label"] = gnomad_vcf
+                members = [models.Variation(**genomic_params)]
+            else:
+                logger.debug(
+                    "Variation Normalizer unable to normalize genomic representation: %s",
+                    gnomad_vcf,
+                )
         else:
-            therapy_descriptor = None
-            if ncit_code not in self.invalid_ids["therapy_descriptors"]:
-                therapy_descriptor = self._get_therapy_descriptor(drugs_data)
-                if therapy_descriptor:
-                    self.valid_ids["therapy_descriptors"][ncit_code] = therapy_descriptor  # noqa: E501
-                    self.therapy_descriptors.append(therapy_descriptor)
-                else:
-                    self.invalid_ids["therapy_descriptors"].add(ncit_code)
-        return therapy_descriptor
+            logger.debug(
+                "Not enough enough information provided to create genomic representation: %s",
+                moa_rep_coord,
+            )
+
+        return members
+
+    def _add_genes(self, genes: List[str]) -> None:
+        """Create gene objects for all MOA gene records.
+        Mutates instance variables `able_to_normalize['genes']` and `genes`, if
+        the gene-normalizer can successfully normalize the gene
 
-    def _get_therapy_descriptor(self, drugs_data: List[Dict]) -> Optional[Dict]:
-        """Get therapy descriptor for drug
+        :param genes: All genes in MOAlmanac
+        """
+        for gene in genes:
+            _, normalized_gene_id = self.vicc_normalizers.normalize_gene([gene])
+            if normalized_gene_id:
+                moa_gene = core_models.Gene(
+                    id=f"moa.normalize.gene:{quote(gene)}",
+                    label=gene,
+                    extensions=[
+                        core_models.Extension(
+                            name="gene_normalizer_id", value=normalized_gene_id
+                        )
+                    ],
+                ).model_dump(exclude_none=True)
+                self.able_to_normalize["genes"][quote(gene)] = moa_gene
+                self.genes.append(moa_gene)
+            else:
+                logger.debug("Gene Normalizer unable to normalize: %s", gene)
 
-        :param List[Dict] drugs_data: List of drugs. For now, `drugs_data` will always
-            have a length of one.
-        :return: Therapy descriptor represented as a dictionary if therapy normalizer
-            was able to normalize the drug
-        """
-        # Since we only support 1 therapeutic we can get the first element
-        drug = drugs_data[0]
-        ncit_id = f"ncit:{drug['ncitCode']}"
-        label = drug["drugName"]
-
-        queries = [ncit_id, label]
-        therapy_norm_resp, normalized_therapy_id = \
-            self.vicc_normalizers.normalize_therapy(queries)
-        if not normalized_therapy_id:
-            logger.warning(f"Therapy Normalizer unable to normalize using queries: {queries}")  # noqa: E501
-            return None
+    def _add_documents(self, sources: List) -> None:
+        """Create document objects for all MOA sources.
+        Mutates instance variables `documents` and `self.able_to_normalize["documents"]`
+
+        :param sources: All sources in MOA
+        """
+        for source in sources:
+            source_id = source["id"]
+
+            if source["nct"]:
+                mappings = [
+                    core_models.Mapping(
+                        coding=core_models.Coding(
+                            code=source["nct"],
+                            system="https://clinicaltrials.gov/search?term=",
+                        ),
+                        relation=core_models.Relation.EXACT_MATCH,
+                    )
+                ]
+            else:
+                mappings = None
 
-        regulatory_approval_extension = \
-            self.vicc_normalizers.get_regulatory_approval_extension(therapy_norm_resp)
+            document = Document(
+                id=f"moa.source:{source_id}",
+                title=source["citation"],
+                url=source["url"] if source["url"] else None,
+                pmid=source["pmid"] if source["pmid"] else None,
+                doi=source["doi"] if source["doi"] else None,
+                mappings=mappings,
+                extensions=[
+                    core_models.Extension(name="source_type", value=source["type"])
+                ],
+            ).model_dump(exclude_none=True)
+            self.able_to_normalize["documents"][source_id] = document
+            self.documents.append(document)
+
+    def _get_therapeutic_substitute_group(
+        self,
+        therapeutic_sub_group_id: str,
+        therapies: List[Dict],
+        therapy_interaction_type: str,
+    ) -> None:
+        """MOA does not support therapeutic substitute group
 
-        return ValueObjectDescriptor(
-            type="TherapyDescriptor",
-            id=f"oncokb.normalize.therapy:{quote(label)}",
-            label=label,
-            therapy_id=normalized_therapy_id,
-            alternate_labels=drug["synonyms"] if drug["synonyms"] else None,
-            xrefs=[ncit_id],
-            extensions=[regulatory_approval_extension] if regulatory_approval_extension else None  # noqa: E501
-        ).dict(exclude_none=True)
-
-    def _add_disease_descriptor(self, disease_data: Dict) -> Optional[Dict]:
-        """Get disease descriptor
-        The `disease_descriptor` instance variable will be updated if disease normalizer
-        was able to normalize the disease and if the disease does not already have a
-        disease descriptor.
-
-        :param Dict disease_data: Disease data
-        :return: Disease descriptor represented as a dictionary if disease normalizer
-            was able to normalize the disease
-        """
-        disease_id = str(disease_data["id"])
-        if disease_id in self.valid_ids["disease_descriptors"]:
-            disease_descriptor = self.valid_ids["disease_descriptors"][disease_id]
-        else:
-            disease_descriptor = None
-            if disease_id not in self.invalid_ids["disease_descriptors"]:
-                disease_descriptor = self._get_disease_descriptor(disease_data)
-                if disease_descriptor:
-                    self.valid_ids["disease_descriptors"][disease_id] = \
-                        disease_descriptor
-                    self.disease_descriptors.append(disease_descriptor)
-                else:
-                    self.invalid_ids["disease_descriptors"].add(disease_id)
-        return disease_descriptor
+        :param therapeutic_sub_group_id: ID for Therapeutic Substitute Group
+        :param therapies: List of therapy objects
+        :param therapy_interaction_type: Therapy type provided by MOA
+        :return: None, since not supported by MOA
+        """
 
-    def _get_disease_descriptor(self, disease_data: Dict) -> Optional[Dict]:
-        """Get disease descriptor for disease
+    def _get_therapeutic_agent(self, label: str) -> Optional[Dict]:
+        """Get Therapeutic Agent for a MOA therapy name.
+        Will run `label` through therapy-normalizer.
 
-        :param Dict disease_data: Disease data
-        :return: Disease descriptor represented as a dictionary if disease normalizer
-            was able to normalize the disease
-        """
-        oncokb_disease_id = f"oncokb.disease:{disease_data['id']}"
-        oncotree_code = f"oncotree:{disease_data['code']}"
-        label = disease_data["name"]
-        queries = [oncotree_code, label]
-        _, normalized_disease_id = self.vicc_normalizers.normalize_disease(queries)
-        if not normalized_disease_id:
-            logger.warning(f"Disease Normalizer unable to normalize: "
-                           f"{oncokb_disease_id} using queries {queries}")
-            return None
+        :param label: MOA therapy name
+        :return: If able to normalize therapy, returns therapeutic agent represented as
+            a dict
+        """
+        (
+            therapy_norm_resp,
+            normalized_therapeutic_id,
+        ) = self.vicc_normalizers.normalize_therapy([label])
 
-        extensions = list()
-        for key, ext_label in DISEASE_EXT_CONVERSIONS:
-            if disease_data[key] or disease_data[key] is False:
-                if key == "mainType":
-                    value = deepcopy(disease_data[key])
-                    value["tumor_form"] = value.pop("tumorForm")
-                else:
-                    value = disease_data[key]
-                extensions.append(Extension(name=ext_label, value=value))
+        if not normalized_therapeutic_id:
+            logger.debug("Therapy Normalizer unable to normalize: %s", label)
+            return None
 
-        disease_descriptor = ValueObjectDescriptor(
-            id=oncokb_disease_id,
-            type="DiseaseDescriptor",
-            label=label,
-            disease_id=normalized_disease_id,
-            xrefs=[oncotree_code],
-            extensions=extensions if extensions else None
-        ).dict(exclude_none=True)
-        return disease_descriptor
-
-    def _add_gene_descriptors(self, genes: List[Dict]) -> None:
-        """Add gene descriptors represented as a dict to the `gene_descriptors` instance
-            variable
+        extensions = [
+            self._get_therapy_normalizer_ext_data(
+                normalized_therapeutic_id, therapy_norm_resp
+            ),
+        ]
 
-        :param List[Dict] genes: List of genes in OncoKB
-        """
-        for gene in genes:
-            gene_queries = list()
-            xrefs = list()
+        regulatory_approval_extension = (
+            self.vicc_normalizers.get_regulatory_approval_extension(therapy_norm_resp)
+        )
 
-            entrez_id = gene["entrezGeneId"]
-            if entrez_id:
-                entrez_id = f"ncbigene:{entrez_id}"
-                gene_queries.append(entrez_id)
-                xrefs.append(entrez_id)
-
-            symbol = gene["hugoSymbol"]
-            if symbol:
-                gene_queries.append(symbol)
+        if regulatory_approval_extension:
+            extensions.append(regulatory_approval_extension)
 
-            _, normalized_gene_id = self.vicc_normalizers.normalize_gene(gene_queries)
-            if normalized_gene_id:
-                extensions = list()
+        return core_models.TherapeuticAgent(
+            id=f"moa.{therapy_norm_resp.therapeutic_agent.id}",
+            label=label,
+            extensions=extensions,
+        ).model_dump(exclude_none=True)
 
-                for key, ext_label in GENE_EXT_CONVERSIONS:
-                    if gene[key] or gene[key] is False:
-                        extensions.append(Extension(name=ext_label, value=gene[key]))
-
-                gene_descriptor = GeneDescriptor(
-                    id=f"oncokb.normalize.gene:{symbol}",
-                    label=symbol,
-                    gene_id=normalized_gene_id,
-                    description=gene["summary"] if gene["summary"] else None,
-                    extensions=extensions if extensions else None,
-                    xrefs=xrefs if xrefs else None
-                ).dict(exclude_none=True)
-                self.gene_descriptors.append(gene_descriptor)
-            else:
-                logger.warning(f"Gene Normalizer unable to normalize: {gene_queries}")
+    def _add_disease(self, disease: Dict) -> Optional[Dict]:
+        """Create or get disease given MOA disease.
+        First looks in cache for existing disease, if not found will attempt to
+        normalize. Will generate a digest from the original MOA disease object. This
+        will be used as the key in the caches. Will add the generated digest to
+        `diseases` and `able_to_normalize['diseases']` if disease-normalizer is able to
+        normalize. Else will add the generated digest to
+        `unable_to_normalize['disease']`
 
-    async def _add_variation_descriptor(self, data: Dict) -> Optional[Dict]:
-        """Get variation descriptor
-        The `variation_descriptors` instance variable will be updated if variation
-        normalize was able to normalize the variant.
-
-        :param Dict data: OncoKB data
-        :return: Variation Descriptor represented as a dictionary if variation
-            normalizer was able to normalize the variant
-        """
-        query = data["query"]
-        gene = query["hugoSymbol"]
-        alteration = query["alteration"]
-        if not all((gene, alteration)):
+        :param disease: MOA disease object
+        :return: Disease object if disease-normalizer was able to normalize
+        """
+        if not all(value for value in disease.values()):
             return None
 
-        variant = f"{gene} {alteration}"
-        variation_descriptor = await self.vicc_normalizers.normalize_variation(
-            [variant])
-
-        if not variation_descriptor:
-            logger.warning(f"Variation Normalizer unable to normalize: {variant}")
-            return None
+        # Since MOA disease objects do not have an ID, we will create a digest from
+        # the original MOA disease object
+        disease_list = sorted([f"{k}:{v}" for k, v in disease.items() if v])
+        blob = json.dumps(disease_list, separators=(",", ":")).encode("ascii")
+        disease_id = sha512t24u(blob)
+
+        vrs_disease = self.able_to_normalize["diseases"].get(disease_id)
+        if vrs_disease:
+            return vrs_disease
+        vrs_disease = None
+        if disease_id not in self.unable_to_normalize["diseases"]:
+            vrs_disease = self._get_disease(disease)
+            if vrs_disease:
+                self.able_to_normalize["diseases"][disease_id] = vrs_disease
+                self.diseases.append(vrs_disease)
+            else:
+                self.unable_to_normalize["diseases"].add(disease_id)
+        return vrs_disease
 
-        extensions = list()
-        for key, ext_label in VARIATION_EXT_CONVERSIONS:
-            if data[key] or data[key] is False:
-                extensions.append(Extension(name=ext_label, value=data[key]).dict())
-
-        vd = VariationDescriptor(
-            id=f"oncokb.variant:{quote(variant)}",
-            label=variant,
-            description=data["variantSummary"] if data["variantSummary"] else None,
-            variation_id=variation_descriptor.variation_id,
-            variation=variation_descriptor.variation,
-            gene_context=f"oncokb.normalize.gene:{query['hugoSymbol']}",
-            extensions=extensions if extensions else None
-        ).dict(by_alias=True, exclude_none=True)
-        self.variation_descriptors.append(vd)
-        return vd
+    def _get_disease(self, disease: Dict) -> Optional[Dict]:
+        """Get core_models.Disease object for a MOA disease
 
-    def _get_documents(self, pmids: List[str]) -> List[dict]:
-        """Get documents from PMIDs.
+        :param disease: MOA disease record
+        :return: If able to normalize, core_models.Disease represented as a dict.
+            Otherwise, `None`
+        """
+        queries = []
+        mappings = []
+
+        ot_code = disease["oncotree_code"]
+        ot_term = disease["oncotree_term"]
+        if ot_code:
+            mappings.append(
+                core_models.Mapping(
+                    coding=core_models.Coding(
+                        code=ot_code,
+                        system="https://oncotree.mskcc.org/",
+                        label=ot_term,
+                    ),
+                    relation=core_models.Relation.EXACT_MATCH,
+                )
+            )
+            queries.append(f"oncotree:{disease['oncotree_code']}")
+
+        disease_name = disease["name"]
+        if ot_term:
+            queries.append(ot_term)
+
+        if disease_name:
+            queries.append(disease_name)
+
+        (
+            disease_norm_resp,
+            normalized_disease_id,
+        ) = self.vicc_normalizers.normalize_disease(queries)
 
-        :param List[str] pmids: List of PubMed IDs
-        :return: List of documents represented as dictionaries
-        """
-        documents = list()
-        for pmid in pmids:
-            document = Document(
-                id=f"pmid:{pmid}",
-                label=f"PubMed {pmid}"
-            ).dict(exclude_none=True)
-            documents.append(document)
-            if document not in self.documents:
-                self.documents.append(document)
+        if not normalized_disease_id:
+            logger.debug("Disease Normalizer unable to normalize: %s", queries)
+            return None
 
-        # TODO: Do abstracts in issue-204
-        return documents
+        return core_models.Disease(
+            id=f"moa.{disease_norm_resp.disease.id}",
+            label=disease_name,
+            mappings=mappings if mappings else None,
+            extensions=[
+                self._get_disease_normalizer_ext_data(
+                    normalized_disease_id, disease_norm_resp
+                ),
+            ],
+        ).model_dump(exclude_none=True)
```

### Comparing `metakb-1.2.0.dev0/metakb.egg-info/PKG-INFO` & `metakb-2.0.0.dev0/src/metakb.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,28 +1,79 @@
 Metadata-Version: 2.1
 Name: metakb
-Version: 1.2.0.dev0
+Version: 2.0.0.dev0
 Summary: A search interface for cancer variant interpretations assembled by aggregating and harmonizing across multiple cancer variant interpretation knowledgebases.
-Home-page: https://github.com/cancervariants/metakb
-Author: VICC
-Author-email: help@cancervariants.org
-License: MIT
-Platform: UNKNOWN
+Author: Alex H Wagner, Kori Kuzma, James Stevenson, Brian Walsh, Jeff Liu
+License: MIT License
+        
+        Copyright (c) 2018 VICC
+        
+        Permission is hereby granted, free of charge, to any person obtaining a copy
+        of this software and associated documentation files (the "Software"), to deal
+        in the Software without restriction, including without limitation the rights
+        to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+        copies of the Software, and to permit persons to whom the Software is
+        furnished to do so, subject to the following conditions:
+        
+        The above copyright notice and this permission notice shall be included in all
+        copies or substantial portions of the Software.
+        
+        THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+        IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+        FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+        AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+        LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+        OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+        SOFTWARE.
+        
+Project-URL: Homepage, https://github.com/cancervariants/metakb
+Project-URL: Documentation, https://github.com/cancervariants/metakb
+Project-URL: Changelog, https://github.com/cancervariants/metakb/releases
+Project-URL: Source, https://github.com/cancervariants/metakb
+Project-URL: Bug Tracker, https://github.com/cancervariants/metakb/issues
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
-Provides-Extra: dev
-Provides-Extra: tests
 License-File: LICENSE
+Requires-Dist: ga4gh.vrs~=2.0.0a5
+Requires-Dist: gene-normalizer[etl]~=0.3.0-dev1
+Requires-Dist: variation-normalizer~=0.8.2
+Requires-Dist: disease-normalizer[etl]~=0.4.0.dev3
+Requires-Dist: thera-py[etl]~=0.5.0.dev3
+Requires-Dist: civicpy~=3.0.0
+Requires-Dist: requests
+Requires-Dist: pydantic==2.*
+Requires-Dist: requests-cache
+Requires-Dist: neo4j==5.*
+Requires-Dist: uvicorn
+Requires-Dist: fastapi
+Requires-Dist: boto3
+Requires-Dist: botocore
+Requires-Dist: asyncclick
+Provides-Extra: tests
+Requires-Dist: pytest; extra == "tests"
+Requires-Dist: pytest-cov; extra == "tests"
+Requires-Dist: mock; extra == "tests"
+Requires-Dist: pytest-asyncio; extra == "tests"
+Provides-Extra: dev
+Requires-Dist: pre-commit; extra == "dev"
+Requires-Dist: ruff==0.2.0; extra == "dev"
+Provides-Extra: notebooks
+Requires-Dist: ipykernel; extra == "notebooks"
+Requires-Dist: jupyterlab; extra == "notebooks"
 
 [![Documentation Status](https://readthedocs.org/projects/vicc-metakb/badge/?version=latest)](https://vicc-metakb.readthedocs.io/en/latest/?badge=latest) [![Build Status](https://travis-ci.org/cancervariants/metakb.svg?branch=main)](https://travis-ci.org/cancervariants/metakb) [![Coverage Status](https://coveralls.io/repos/github/cancervariants/metakb/badge.svg?branch=main)](https://coveralls.io/github/cancervariants/metakb?branch=main)
 
 # metakb
 
 The intent of the project is to leverage the collective knowledge of the disparate existing resources of the VICC to improve the comprehensiveness of clinical interpretation of genomic variation. An ongoing goal will be to provide and improve upon standards and guidelines by which other groups with clinical interpretation data may make it accessible and visible to the public. We have released a preprint discussing our initial harmonization effort and observed disparities in the structure and content of variant interpretations.
 
@@ -63,15 +114,15 @@
 
 ### Setting up Neo4j
 
 The MetaKB uses [Neo4j](https://neo4j.com/) for its database backend. To run a local MetaKB instance, you'll need to run a Neo4j database instance as well. The easiest way to do this is from Neo4j Desktop.
 
 First, follow the [desktop setup instructions](https://neo4j.com/developer/neo4j-desktop) to download, install, and open Neo4j Desktop for the first time.
 
-Once you have opened Neo4j desktop, use the "New" button in the upper-left region of the window to create a new project. Within that project, click the "Add" button in the upper-right region of the window and select "Local DBMS". The name of the DBMS doesn't matter, but the password will be used later to connect the database to MetaKB (we have been using "admin" by default). Click "Create". Then, click the row within the project screen corresponding to your newly-created DBMS, and click the green "Start" button to start the database service.
+Once you have opened Neo4j desktop, use the `New` button in the upper-left region of the window to create a new project. Within that project, click the `Add` button in the upper-right region of the window and select `Local DBMS`. The name of the DBMS doesn't matter, but the password will be used later to connect the database to MetaKB (we have been using `password` by default). Select version `5.14.0` (other versions have not been tested). Click `Create`. Then, click the row within the project screen corresponding to your newly-created DBMS, and click the green `Start` button to start the database service.
 
 The graph will initially be empty, but once you have successfully loaded data, Neo4j Desktop provides an interface for exploring and visualizing relationships within the graph. To access it, click the blue "Open" button. The prompt at the top of this window processes [Cypher queries](https://neo4j.com/docs/cypher-refcard/current/); to start, try `MATCH (n:Statement {id:"civic.eid:1409"}) RETURN n`. Buttons on the left-hand edge of the results pane let you select graph, tabular, or textual output.
 
 
 ### Setting up normalizers
 
 The MetaKB calls a number of normalizer libraries to transform resource data and resolve incoming search queries. These will be installed as part of the package requirements, but require additional setup.
@@ -90,17 +141,15 @@
 
 Next, initialize the [Variation Normalizer](https://github.com/cancervariants/variation-normalization) by following the instructions in the [README](https://github.com/cancervariants/variation-normalization#installation). When setting up the UTA database, [these](https://github.com/ga4gh/vrs-python/tree/main/docs/setup_help) docs may be helpful.
 
 
 The MetaKB can acquire all other needed normalizer data, except for that of [OMIM](https://www.omim.org/downloads), which must be manually placed:
 
 ```sh
-cd disease/  # starting from the site-packages dir of your virtual environment's Python instance
-mkdir -p data/omim
-cp ~/YOUR/PATH/TO/mimTitles.txt data/omim/omim_<date>.tsv  # replace <date> with date of data acquisition formatted as YYYYMMDD
+cp ~/YOUR/PATH/TO/mimTitles.txt ~/.local/share/wags_tails/omim/omim_<date>.tsv  # replace <date> with date of data acquisition formatted as YYYYMMDD
 ```
 
 ### Environment Variables
 
 MetaKB relies on environment variables to set in order to work.
 
 * Always Required:
@@ -111,62 +160,34 @@
 
     Example:
 
     ```shell script
     export UTA_DB_URL=postgresql://uta_admin:password@localhost:5432/uta/uta_20210129
     ```
 
-  * `ONCOKB_API_TOKEN`
-    * Required to harvest OncoKB data. If you do not set this environment variable, you can set during the initialization of the OncoKBHarvester.
-    * Used to access OncoKB data via their REST API. See [here](https://www.oncokb.org/apiAccess) for more information on how to register an account and get an OncoKB API token.
-
-    Example for setting environment variable:
-    ```shell script
-    export ONCOKB_API_TOKEN={api_token}
-    ```
-
-    Example for setting during OncoKB Harvester initialization:
-    ```python
-    OncoKBHarvester(api_token={api_token})
-    ```
-
 * Required when using the `--load_normalizers_db` or `--force_load_normalizers_db` arguments in CLI commands
-  * `RXNORM_API_KEY`
+  * `UMLS_API_KEY`
     * Used in Therapy Normalizer to retrieve RxNorm data
-    * RxNorm requires a UMLS license, which you can register for one [here](https://www.nlm.nih.gov/research/umls/index.html). You must set the `RxNORM_API_KEY` environment variable to your API key. This can be found in the [UTS 'My Profile' area](https://uts.nlm.nih.gov/uts/profile) after singing in.
+    * RxNorm requires a UMLS license, which you can register for one [here](https://www.nlm.nih.gov/research/umls/index.html). You must set the `UMLS_API_KEY` environment variable to your API key. This can be found in the [UTS 'My Profile' area](https://uts.nlm.nih.gov/uts/profile) after singing in.
 
     Example:
 
     ```shell script
-    export RXNORM_API_KEY={rxnorm_api_key}
+    export UMLS_API_KEY={rxnorm_api_key}
     ```
 
-  * `DATAVERSE_API_KEY`
+  * `HARVARD_DATAVERSE_API_KEY`
     * Used in Therapy Normalizer to retrieve HemOnc data
-    * HemOnc.org data requires a Harvard Dataverse API key. After creating a user account on the Harvard Dataverse website, you can follow [these instructions](https://guides.dataverse.org/en/latest/user/account.html) to generate a key. You will create or login to your account at [this](https://dataverse.harvard.edu/) site. You must set the `DATAVERSE_API_KEY` environment variable to your API key.
+    * HemOnc.org data requires a Harvard Dataverse API key. After creating a user account on the Harvard Dataverse website, you can follow [these instructions](https://guides.dataverse.org/en/latest/user/account.html) to generate a key. You will create or login to your account at [this](https://dataverse.harvard.edu/) site. You must set the `HARVARD_DATAVERSE_API_KEY` environment variable to your API key.
 
     Example:
 
     ```shell script
-    export DATAVERSE_API_KEY={dataverse_api_key}
-    ```
-
-### Data files
-
-Some sources in MetaKB require user provided files to harvest data.
-
-* OncoKB
-  * In addition to setting the `ONCOKB_API_TOKEN` environment variable to harvest OncoKB data, you also need to provide a CSV file containing a header row with `hugo_symbol` and `protein_change`, associated rows containing protein variants you wish to harvest, and using a comma as the delimiter. The file will look something like:
-
-    ```csv
-    hugo_symbol,protein_change
-    BRAF,V600E
-    ...
+    export HARVARD_DATAVERSE_API_KEY={dataverse_api_key}
     ```
-  * This file will harvest OncoKB evidence based on the variants provided.
 
 ### Loading data
 
 Once Neo4j and DynamoDB instances are both running, and necessary normalizer data has been placed, run the MetaKB CLI with the `--initialize_normalizers` flag to acquire all other necessary normalizer source data, and execute harvest, transform, and load operations into the graph datastore.
 
 In the MetaKB project root, run the following:
 
@@ -198,18 +219,18 @@
 ```sh
 python3 -m pytest
 ```
 
 
 ### And coding style tests
 
-Code style is managed by [flake8](https://github.com/PyCQA/flake8) and checked prior to commit.
+Code style is managed by [ruff](https://astral.sh/ruff) and checked prior to commit.
 
 ```
-see .flake8
+python3 -m ruff check --fix . && python3 -m ruff format .
 
 ```
 
 ## Contributing
 
 Please read [CONTRIBUTING.md](CONTRIBUTING.md) for details on our code of conduct, and the process for submitting pull requests to us.
 
@@ -233,9 +254,7 @@
 ## Versioning
 
 We use [SemVer](http://semver.org/) for versioning. For the versions available, see the [tags on this repository](https://github.com/cancervariants/metakb/tags).
 
 ## License
 
 This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details
-
-
```

