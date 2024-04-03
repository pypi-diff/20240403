# Comparing `tmp/panpiper-1.0.0.tar.gz` & `tmp/panpiper-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "panpiper-1.0.0.tar", last modified: Thu Mar 30 16:55:22 2023, max compression
+gzip compressed data, was "panpiper-1.0.1.tar", last modified: Wed Apr  3 01:45:45 2024, max compression
```

## Comparing `panpiper-1.0.0.tar` & `panpiper-1.0.1.tar`

### file list

```diff
@@ -1,34 +1,81 @@
-drwxr-xr-x   0 reneeoles   (501) staff       (20)        0 2023-03-30 16:55:22.691640 panpiper-1.0.0/
--rw-r--r--   0 reneeoles   (501) staff       (20)     1509 2023-01-23 16:00:15.000000 panpiper-1.0.0/LICENSE
--rw-r--r--   0 reneeoles   (501) staff       (20)       37 2023-01-21 00:39:08.000000 panpiper-1.0.0/MANIFEST.in
--rw-r--r--   0 reneeoles   (501) staff       (20)     9324 2023-03-30 16:55:22.691265 panpiper-1.0.0/PKG-INFO
--rw-r--r--   0 reneeoles   (501) staff       (20)     8728 2023-03-30 16:43:34.000000 panpiper-1.0.0/README.md
-drwxr-xr-x   0 reneeoles   (501) staff       (20)        0 2023-03-30 16:55:22.683112 panpiper-1.0.0/panpiper/
--rw-r--r--   0 reneeoles   (501) staff       (20)      415 2023-01-23 16:01:59.000000 panpiper-1.0.0/panpiper/__init__.py
--rwxr-xr-x   0 reneeoles   (501) staff       (20)     6888 2023-03-30 16:43:34.000000 panpiper-1.0.0/panpiper/main.py
--rw-r--r--   0 reneeoles   (501) staff       (20)     5638 2023-03-30 16:43:34.000000 panpiper-1.0.0/panpiper/test.py
-drwxr-xr-x   0 reneeoles   (501) staff       (20)        0 2023-03-30 16:55:22.686933 panpiper-1.0.0/panpiper/tests/
--rw-r--r--   0 reneeoles   (501) staff       (20)        0 2023-01-26 16:07:32.000000 panpiper-1.0.0/panpiper/tests/__init__.py
-drwxr-xr-x   0 reneeoles   (501) staff       (20)        0 2023-03-30 16:55:22.687348 panpiper-1.0.0/panpiper/tests/test_data/
--rw-r--r--   0 reneeoles   (501) staff       (20)        0 2023-01-26 16:07:32.000000 panpiper-1.0.0/panpiper/tests/test_data/__init__.py
--rw-r--r--   0 reneeoles   (501) staff       (20)     3918 2023-03-30 16:43:34.000000 panpiper-1.0.0/panpiper/tests/test_main.py
-drwxr-xr-x   0 reneeoles   (501) staff       (20)        0 2023-03-30 16:55:22.689027 panpiper-1.0.0/panpiper/tests/test_scripts/
--rw-r--r--   0 reneeoles   (501) staff       (20)      361 2023-01-26 16:07:32.000000 panpiper-1.0.0/panpiper/tests/test_scripts/__init__.py
--rw-r--r--   0 reneeoles   (501) staff       (20)    14686 2023-01-26 16:07:32.000000 panpiper-1.0.0/panpiper/tests/test_scripts/filter_isolates.py
--rwxr-xr-x   0 reneeoles   (501) staff       (20)     1493 2023-01-26 16:07:32.000000 panpiper-1.0.0/panpiper/tests/test_scripts/test_concat_amrfinder.py
-drwxr-xr-x   0 reneeoles   (501) staff       (20)        0 2023-03-30 16:55:22.690783 panpiper-1.0.0/panpiper/workflow/
--rw-r--r--   0 reneeoles   (501) staff       (20)     1706 2023-03-30 16:43:34.000000 panpiper-1.0.0/panpiper/workflow/assembly.smk
--rw-r--r--   0 reneeoles   (501) staff       (20)    14894 2023-03-30 16:43:34.000000 panpiper-1.0.0/panpiper/workflow/pangenome.smk
--rw-r--r--   0 reneeoles   (501) staff       (20)     7287 2023-03-30 16:43:34.000000 panpiper-1.0.0/panpiper/workflow/pyseer.smk
--rw-r--r--   0 reneeoles   (501) staff       (20)     5565 2023-03-30 16:43:34.000000 panpiper-1.0.0/panpiper/workflow/quality.smk
--rw-r--r--   0 reneeoles   (501) staff       (20)     3234 2023-03-30 16:43:34.000000 panpiper-1.0.0/panpiper/workflow.py
-drwxr-xr-x   0 reneeoles   (501) staff       (20)        0 2023-03-30 16:55:22.686066 panpiper-1.0.0/panpiper.egg-info/
--rw-r--r--   0 reneeoles   (501) staff       (20)     9324 2023-03-30 16:55:22.000000 panpiper-1.0.0/panpiper.egg-info/PKG-INFO
--rw-r--r--   0 reneeoles   (501) staff       (20)      693 2023-03-30 16:55:22.000000 panpiper-1.0.0/panpiper.egg-info/SOURCES.txt
--rw-r--r--   0 reneeoles   (501) staff       (20)        1 2023-03-30 16:55:22.000000 panpiper-1.0.0/panpiper.egg-info/dependency_links.txt
--rw-r--r--   0 reneeoles   (501) staff       (20)       47 2023-03-30 16:55:22.000000 panpiper-1.0.0/panpiper.egg-info/entry_points.txt
--rw-r--r--   0 reneeoles   (501) staff       (20)        1 2023-03-30 16:55:22.000000 panpiper-1.0.0/panpiper.egg-info/not-zip-safe
--rw-r--r--   0 reneeoles   (501) staff       (20)       11 2023-03-30 16:55:22.000000 panpiper-1.0.0/panpiper.egg-info/requires.txt
--rw-r--r--   0 reneeoles   (501) staff       (20)        9 2023-03-30 16:55:22.000000 panpiper-1.0.0/panpiper.egg-info/top_level.txt
--rw-r--r--   0 reneeoles   (501) staff       (20)       38 2023-03-30 16:55:22.691691 panpiper-1.0.0/setup.cfg
--rw-r--r--   0 reneeoles   (501) staff       (20)     1419 2023-03-30 16:54:51.000000 panpiper-1.0.0/setup.py
+drwxr-xr-x   0 reneeoles   (501) staff       (20)        0 2024-04-03 01:45:45.673124 panpiper-1.0.1/
+-rw-r--r--   0 reneeoles   (501) staff       (20)     1509 2023-01-23 16:00:15.000000 panpiper-1.0.1/LICENSE
+-rw-r--r--   0 reneeoles   (501) staff       (20)       37 2023-01-21 00:39:08.000000 panpiper-1.0.1/MANIFEST.in
+-rw-r--r--   0 reneeoles   (501) staff       (20)     9698 2024-04-03 01:45:45.672949 panpiper-1.0.1/PKG-INFO
+-rw-r--r--   0 reneeoles   (501) staff       (20)     8735 2024-04-03 00:21:18.000000 panpiper-1.0.1/README.md
+drwxr-xr-x   0 reneeoles   (501) staff       (20)        0 2024-04-03 01:45:45.636859 panpiper-1.0.1/panpiper/
+-rw-r--r--   0 reneeoles   (501) staff       (20)      415 2023-01-23 16:01:59.000000 panpiper-1.0.1/panpiper/__init__.py
+-rwxr-xr-x   0 reneeoles   (501) staff       (20)     7451 2024-04-03 01:12:25.000000 panpiper-1.0.1/panpiper/main.py
+-rw-r--r--   0 reneeoles   (501) staff       (20)     5638 2023-03-30 16:43:34.000000 panpiper-1.0.1/panpiper/test.py
+drwxr-xr-x   0 reneeoles   (501) staff       (20)        0 2024-04-03 01:45:45.639690 panpiper-1.0.1/panpiper/tests/
+-rw-r--r--   0 reneeoles   (501) staff       (20)        0 2023-01-26 16:07:32.000000 panpiper-1.0.1/panpiper/tests/__init__.py
+drwxr-xr-x   0 reneeoles   (501) staff       (20)        0 2024-04-03 01:45:45.640218 panpiper-1.0.1/panpiper/tests/test_data/
+-rw-r--r--   0 reneeoles   (501) staff       (20)        0 2023-01-26 16:07:32.000000 panpiper-1.0.1/panpiper/tests/test_data/__init__.py
+-rw-r--r--   0 reneeoles   (501) staff       (20)     3918 2023-03-30 16:43:34.000000 panpiper-1.0.1/panpiper/tests/test_main.py
+drwxr-xr-x   0 reneeoles   (501) staff       (20)        0 2024-04-03 01:45:45.641922 panpiper-1.0.1/panpiper/tests/test_scripts/
+-rw-r--r--   0 reneeoles   (501) staff       (20)      361 2023-01-26 16:07:32.000000 panpiper-1.0.1/panpiper/tests/test_scripts/__init__.py
+-rw-r--r--   0 reneeoles   (501) staff       (20)    14686 2023-01-26 16:07:32.000000 panpiper-1.0.1/panpiper/tests/test_scripts/filter_isolates.py
+-rwxr-xr-x   0 reneeoles   (501) staff       (20)     1493 2023-01-26 16:07:32.000000 panpiper-1.0.1/panpiper/tests/test_scripts/test_concat_amrfinder.py
+drwxr-xr-x   0 reneeoles   (501) staff       (20)        0 2024-04-03 01:45:45.644948 panpiper-1.0.1/panpiper/workflow/
+-rw-r--r--   0 reneeoles   (501) staff       (20)     1706 2023-03-30 16:43:34.000000 panpiper-1.0.1/panpiper/workflow/assembly.smk
+drwxr-xr-x   0 reneeoles   (501) staff       (20)        0 2024-04-03 01:45:45.654017 panpiper-1.0.1/panpiper/workflow/envs/
+-rw-r--r--   0 reneeoles   (501) staff       (20)      149 2024-01-24 00:50:52.000000 panpiper-1.0.1/panpiper/workflow/envs/amrfinder.yml
+-rw-r--r--   0 reneeoles   (501) staff       (20)       93 2024-01-24 00:50:52.000000 panpiper-1.0.1/panpiper/workflow/envs/bakta.yml
+-rw-r--r--   0 reneeoles   (501) staff       (20)       65 2024-01-24 00:50:52.000000 panpiper-1.0.1/panpiper/workflow/envs/bbmap.yml
+-rw-r--r--   0 reneeoles   (501) staff       (20)      106 2024-01-24 00:50:52.000000 panpiper-1.0.1/panpiper/workflow/envs/bwa.yml
+-rw-r--r--   0 reneeoles   (501) staff       (20)      102 2024-01-24 00:50:52.000000 panpiper-1.0.1/panpiper/workflow/envs/checkm.yml
+-rw-r--r--   0 reneeoles   (501) staff       (20)      330 2024-04-03 01:37:37.000000 panpiper-1.0.1/panpiper/workflow/envs/checkm2.yml
+-rw-r--r--   0 reneeoles   (501) staff       (20)      110 2024-01-24 00:50:52.000000 panpiper-1.0.1/panpiper/workflow/envs/eggnog.yml
+-rw-r--r--   0 reneeoles   (501) staff       (20)      114 2024-01-24 00:50:52.000000 panpiper-1.0.1/panpiper/workflow/envs/fastani.yml
+-rw-r--r--   0 reneeoles   (501) staff       (20)      100 2024-01-24 00:50:52.000000 panpiper-1.0.1/panpiper/workflow/envs/fasttree.yml
+-rw-r--r--   0 reneeoles   (501) staff       (20)       97 2024-01-24 00:50:52.000000 panpiper-1.0.1/panpiper/workflow/envs/iqtree.yml
+-rw-r--r--   0 reneeoles   (501) staff       (20)       96 2024-01-24 00:50:52.000000 panpiper-1.0.1/panpiper/workflow/envs/kraken.yml
+-rw-r--r--   0 reneeoles   (501) staff       (20)       89 2024-01-24 00:50:52.000000 panpiper-1.0.1/panpiper/workflow/envs/mash.yml
+-rw-r--r--   0 reneeoles   (501) staff       (20)       97 2024-01-24 00:50:52.000000 panpiper-1.0.1/panpiper/workflow/envs/panaroo.yml
+-rw-r--r--   0 reneeoles   (501) staff       (20)       68 2024-01-24 00:50:52.000000 panpiper-1.0.1/panpiper/workflow/envs/poppunk.yml
+-rw-r--r--   0 reneeoles   (501) staff       (20)      172 2024-01-24 00:50:52.000000 panpiper-1.0.1/panpiper/workflow/envs/prokka.yml
+-rw-r--r--   0 reneeoles   (501) staff       (20)       95 2024-01-24 00:50:52.000000 panpiper-1.0.1/panpiper/workflow/envs/pyseer.yml
+-rw-r--r--   0 reneeoles   (501) staff       (20)      201 2024-01-24 00:50:52.000000 panpiper-1.0.1/panpiper/workflow/envs/r.yml
+-rw-r--r--   0 reneeoles   (501) staff       (20)       68 2024-01-24 00:50:52.000000 panpiper-1.0.1/panpiper/workflow/envs/raxml.yml
+-rw-r--r--   0 reneeoles   (501) staff       (20)      112 2024-01-24 00:50:52.000000 panpiper-1.0.1/panpiper/workflow/envs/shovill.yml
+-rw-r--r--   0 reneeoles   (501) staff       (20)      102 2024-01-24 00:50:52.000000 panpiper-1.0.1/panpiper/workflow/envs/unitig.yml
+-rw-r--r--   0 reneeoles   (501) staff       (20)      104 2024-01-24 00:50:52.000000 panpiper-1.0.1/panpiper/workflow/envs/virsorter.yml
+-rw-r--r--   0 reneeoles   (501) staff       (20)    13100 2024-04-03 01:09:15.000000 panpiper-1.0.1/panpiper/workflow/pangenome.smk
+-rw-r--r--   0 reneeoles   (501) staff       (20)     7287 2023-03-30 16:43:34.000000 panpiper-1.0.1/panpiper/workflow/pyseer.smk
+-rw-r--r--   0 reneeoles   (501) staff       (20)     5918 2024-04-03 01:19:50.000000 panpiper-1.0.1/panpiper/workflow/quality.smk
+drwxr-xr-x   0 reneeoles   (501) staff       (20)        0 2024-04-03 01:45:45.672102 panpiper-1.0.1/panpiper/workflow/scripts/
+-rw-r--r--   0 reneeoles   (501) staff       (20)     1813 2024-01-24 00:50:52.000000 panpiper-1.0.1/panpiper/workflow/scripts/AMR_heatmap.R
+-rw-r--r--   0 reneeoles   (501) staff       (20)     4329 2024-01-24 18:23:49.000000 panpiper-1.0.1/panpiper/workflow/scripts/checkm-log.py
+-rw-r--r--   0 reneeoles   (501) staff       (20)     1696 2024-01-24 00:59:58.000000 panpiper-1.0.1/panpiper/workflow/scripts/checkm_bin-stats.py
+-rw-r--r--   0 reneeoles   (501) staff       (20)     1559 2024-01-24 01:00:41.000000 panpiper-1.0.1/panpiper/workflow/scripts/checkm_cat.py
+-rw-r--r--   0 reneeoles   (501) staff       (20)     1711 2024-01-24 00:50:52.000000 panpiper-1.0.1/panpiper/workflow/scripts/concat_amrfinder.py
+-rw-r--r--   0 reneeoles   (501) staff       (20)     1603 2024-01-24 00:50:52.000000 panpiper-1.0.1/panpiper/workflow/scripts/count_patterns.py
+-rwxr-xr-x   0 reneeoles   (501) staff       (20)      201 2024-01-24 00:50:52.000000 panpiper-1.0.1/panpiper/workflow/scripts/create_list.sh
+-rw-r--r--   0 reneeoles   (501) staff       (20)      946 2024-01-24 00:50:52.000000 panpiper-1.0.1/panpiper/workflow/scripts/filter_genes.R
+-rw-r--r--   0 reneeoles   (501) staff       (20)     6219 2024-01-24 00:50:52.000000 panpiper-1.0.1/panpiper/workflow/scripts/filter_isolates.py
+-rw-r--r--   0 reneeoles   (501) staff       (20)     1033 2024-01-24 00:50:52.000000 panpiper-1.0.1/panpiper/workflow/scripts/filter_kmers.R
+-rw-r--r--   0 reneeoles   (501) staff       (20)      962 2024-01-24 00:50:52.000000 panpiper-1.0.1/panpiper/workflow/scripts/filter_kmers_enet.R
+-rw-r--r--   0 reneeoles   (501) staff       (20)     1948 2024-01-24 00:50:52.000000 panpiper-1.0.1/panpiper/workflow/scripts/kraken_reformat.py
+-rw-r--r--   0 reneeoles   (501) staff       (20)     2039 2024-01-24 00:50:52.000000 panpiper-1.0.1/panpiper/workflow/scripts/long_to_wide.py
+-rw-r--r--   0 reneeoles   (501) staff       (20)      749 2024-01-24 00:50:52.000000 panpiper-1.0.1/panpiper/workflow/scripts/mash.smk
+-rwxr-xr-x   0 reneeoles   (501) staff       (20)      561 2024-01-24 00:50:52.000000 panpiper-1.0.1/panpiper/workflow/scripts/move_files.sh
+-rw-r--r--   0 reneeoles   (501) staff       (20)     1098 2024-01-24 00:50:52.000000 panpiper-1.0.1/panpiper/workflow/scripts/nc_aa_translate.py
+-rw-r--r--   0 reneeoles   (501) staff       (20)     2513 2024-01-24 00:50:52.000000 panpiper-1.0.1/panpiper/workflow/scripts/phylogeny_distance.py
+-rw-r--r--   0 reneeoles   (501) staff       (20)     5633 2024-01-24 00:50:52.000000 panpiper-1.0.1/panpiper/workflow/scripts/phylogroup_cluster.py
+-rw-r--r--   0 reneeoles   (501) staff       (20)     4055 2024-01-24 00:50:52.000000 panpiper-1.0.1/panpiper/workflow/scripts/quality_report.Rmd
+-rw-r--r--   0 reneeoles   (501) staff       (20)  8290584 2024-01-24 00:50:52.000000 panpiper-1.0.1/panpiper/workflow/scripts/quality_report.html
+-rwxr-xr-x   0 reneeoles   (501) staff       (20)      190 2024-01-24 00:50:52.000000 panpiper-1.0.1/panpiper/workflow/scripts/setup.sh
+-rw-r--r--   0 reneeoles   (501) staff       (20)     3628 2024-01-24 00:50:52.000000 panpiper-1.0.1/panpiper/workflow/scripts/summarise_annotations.py
+-rw-r--r--   0 reneeoles   (501) staff       (20)     3338 2024-01-24 00:50:52.000000 panpiper-1.0.1/panpiper/workflow/scripts/summarise_annotations_enet.py
+-rw-r--r--   0 reneeoles   (501) staff       (20)     4461 2024-01-24 00:50:52.000000 panpiper-1.0.1/panpiper/workflow/scripts/wrangle_output.py
+-rw-r--r--   0 reneeoles   (501) staff       (20)     3278 2024-04-03 01:11:13.000000 panpiper-1.0.1/panpiper/workflow.py
+drwxr-xr-x   0 reneeoles   (501) staff       (20)        0 2024-04-03 01:45:45.672453 panpiper-1.0.1/panpiper.egg-info/
+-rw-r--r--   0 reneeoles   (501) staff       (20)     9698 2024-04-03 01:45:45.000000 panpiper-1.0.1/panpiper.egg-info/PKG-INFO
+-rw-r--r--   0 reneeoles   (501) staff       (20)     2467 2024-04-03 01:45:45.000000 panpiper-1.0.1/panpiper.egg-info/SOURCES.txt
+-rw-r--r--   0 reneeoles   (501) staff       (20)        1 2024-04-03 01:45:45.000000 panpiper-1.0.1/panpiper.egg-info/dependency_links.txt
+-rw-r--r--   0 reneeoles   (501) staff       (20)       47 2024-04-03 01:45:45.000000 panpiper-1.0.1/panpiper.egg-info/entry_points.txt
+-rw-r--r--   0 reneeoles   (501) staff       (20)        1 2023-03-30 16:55:22.000000 panpiper-1.0.1/panpiper.egg-info/not-zip-safe
+-rw-r--r--   0 reneeoles   (501) staff       (20)      187 2024-04-03 01:45:45.000000 panpiper-1.0.1/panpiper.egg-info/requires.txt
+-rw-r--r--   0 reneeoles   (501) staff       (20)        9 2024-04-03 01:45:45.000000 panpiper-1.0.1/panpiper.egg-info/top_level.txt
+-rw-r--r--   0 reneeoles   (501) staff       (20)       38 2024-04-03 01:45:45.673500 panpiper-1.0.1/setup.cfg
+-rw-r--r--   0 reneeoles   (501) staff       (20)     2026 2024-04-03 01:41:52.000000 panpiper-1.0.1/setup.py
```

### Comparing `panpiper-1.0.0/LICENSE` & `panpiper-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `panpiper-1.0.0/PKG-INFO` & `panpiper-1.0.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,23 +1,35 @@
 Metadata-Version: 2.1
 Name: panpiper
-Version: 1.0.0
+Version: 1.0.1
 Summary: Panpiper: snakemake workflow for bacterial isolate analysis
 Home-page: https://github.com/rolesucsd/Panpiper
 Author: Renee Oles
 Author-email: roles@health.ucsd.edu
 License: BSD-3-Clause
 Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
+Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Development Status :: 3 - Alpha
 Requires-Python: >=3.5
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: setuptools
+Requires-Dist: biopython>=1.78
+Requires-Dist: pandas>=1.0.0
+Requires-Dist: numpy>=1.19.2
+Requires-Dist: matplotlib>=3.1.0
+Requires-Dist: seaborn>=0.10.0
+Requires-Dist: scikit-learn>=0.22.0
+Requires-Dist: scipy>=1.4.0
+Requires-Dist: scikit-bio>=0.5.6
+Requires-Dist: umap-learn>=0.4.0
+Requires-Dist: dendropy>=4.5.0
+Requires-Dist: PyYAML>=5.3
 
 [![Project Status: Active - The project has reached a stable, usable state and is being actively developed.](http://www.repostatus.org/badges/latest/active.svg)](http://www.repostatus.org/#active)
 
 # Panpiper
 
 This package conducts bacterial isolate analysis for one species.  
 
@@ -73,15 +85,15 @@
 * Assembly/  
     * incomplete_assembly_files.txt - samples for which assembly failed
     *  complete_assembly_files.txt - samples for which assemblies passed 
     * {sample}/  
         * contigs.fa - edited assembly 
 
 ### Quality control: 
-The fasta file directory should contain a subdirectory for each sample where the subdirectory name is the sample of the sample. The fasta file within these directories should be formatted as contigs.fa. This is the standard output from Shovill. The sample list should have one sample name per line which corresponds to the directory names. The reference fasta file should be the representative strain of the species which the samples will be compared to using average nucleotide identity.
+The fasta file directory should contain a subdirectory for each sample where the subdirectory name is the sample of the sample. The fasta file within these directories should be formatted as contigs.fa. This is the standard output from Shovill. The sample list should have one sample name per line which corresponds to the name of the fasta file. The reference fasta file should be the representative strain of the species which the samples will be compared to using average nucleotide identity.
 
 Additional parameters that may be included:
 * --ani_cutoff : percent identity to reference cutoff (default 95)
 * --n50 : N50 cutoff (default 5000)
 * --contig_number : number of contigs cutoff (default 1000)
 
 ```sh
```

### Comparing `panpiper-1.0.0/README.md` & `panpiper-1.0.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -56,15 +56,15 @@
 * Assembly/  
     * incomplete_assembly_files.txt - samples for which assembly failed
     *  complete_assembly_files.txt - samples for which assemblies passed 
     * {sample}/  
         * contigs.fa - edited assembly 
 
 ### Quality control: 
-The fasta file directory should contain a subdirectory for each sample where the subdirectory name is the sample of the sample. The fasta file within these directories should be formatted as contigs.fa. This is the standard output from Shovill. The sample list should have one sample name per line which corresponds to the directory names. The reference fasta file should be the representative strain of the species which the samples will be compared to using average nucleotide identity.
+The fasta file directory should contain a subdirectory for each sample where the subdirectory name is the sample of the sample. The fasta file within these directories should be formatted as contigs.fa. This is the standard output from Shovill. The sample list should have one sample name per line which corresponds to the name of the fasta file. The reference fasta file should be the representative strain of the species which the samples will be compared to using average nucleotide identity.
 
 Additional parameters that may be included:
 * --ani_cutoff : percent identity to reference cutoff (default 95)
 * --n50 : N50 cutoff (default 5000)
 * --contig_number : number of contigs cutoff (default 1000)
 
 ```sh
```

### Comparing `panpiper-1.0.0/panpiper/main.py` & `panpiper-1.0.1/panpiper/main.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,41 +1,44 @@
 #!/usr/bin/env python
+# -*- coding: utf-8 -*-
+# File: main.py
+
 # ----------------------------------------------------------------------------
+# Panpiper: Pan-genome analysis pipeline
+#
+# Authors: Renee Oles
+#
 # Copyright (c) 2022--, Panpiper development team.
 #
 # Distributed under the terms of the Modified BSD License.
 #
 # The full license is in the file COPYING.txt, distributed with this software.
 # ----------------------------------------------------------------------------
 
 import argparse
 import logging
 import os
 import sys
 import pkg_resources
-# Delete after package creation
 import importlib
-
 from os.path import join, dirname, basename
 from shutil import copyfile
 from argparse import RawTextHelpFormatter
-
 from panpiper.test import Test
 from panpiper.workflow import Workflow
 
 # Snakefiles
 _ROOT = os.path.abspath(os.path.dirname(__file__))
 WORKFLOW_ASSEMBLY = os.path.join(_ROOT, 'workflow', 'assembly.smk')
 WORKFLOW_QUALITY = os.path.join(_ROOT, 'workflow', 'quality.smk')
 WORKFLOW_PANGENOME = os.path.join(_ROOT, 'workflow', 'pangenome.smk')
 WORKFLOW_PYSEER = os.path.join(_ROOT, 'workflow', 'pyseer.smk')
-
+WORKFLOW_SCRIPTS = os.path.join(_ROOT, 'workflow', 'scripts')
 
 def cli():
-
     ########## Arguments ##########
     ap = argparse.ArgumentParser(description='Package version ', add_help=False,
                                  allow_abbrev=False, formatter_class=RawTextHelpFormatter)
 
     # Required
     apr = ap.add_argument_group('main arguments')
     apr.add_argument('-q', '--fastq', help='Path to fastq file directory',
@@ -84,27 +87,37 @@
     app = ap.add_argument_group('parameters')
     app.add_argument(
         '--ani_cutoff', help='Average percent identity to reference cutoff', default=95, type=float)
     app.add_argument('--contig_number',
                      help='Max number of contigs', default=1000, type=int)
     app.add_argument('--n50', help='N50 cutoff', default=5000, type=int)
     app.add_argument('--eggnog_dir', help='Path to the eggnog database directory',
-                     default="panpiper/databases/eggnog", type=str)
-    app.add_argument('--kraken_dir', help='Path to the kraken2 database directory',
-                     default="panpiper/databases/kraken", type=str)
+                     default=os.path.join(_ROOT, "databases", "eggnog"), type=str)
     app.add_argument('--bakta_dir', help='Path to the bakta database directory',
-                     default="panpiper/databases/bakta", type=str)
+                     default=os.path.join(_ROOT, "databases", "bakta"), type=str)
+    app.add_argument('--checkm_dir', help='Path to the checkm database directory',
+                     default=os.path.join(_ROOT, "databases", "checkm2"), type=str)
     app.add_argument(
         '--pheno_column', help='The column in the phenotype file to use for the association study', type=str)
     app.add_argument(
         '--max_jobs', help='Maximum number of cluster jobs [%(default)s]', default=40, type=int)
+    app.add_argument('--scripts_dir', help='Directory of scripts in package, do not change unless you have modified the scripts',
+        type=str, default=WORKFLOW_SCRIPTS)
 
     ########## Workflow ##########
     master = Test(ap)
 
+    # Create the directory if it doesn't exist
+    if not os.path.exists(master.eggnog_dir):
+        os.makedirs(master.eggnog_dir)
+
+    # Create the directory if it doesn't exist
+    if not os.path.exists(master.bakta_dir):
+        os.makedirs(master.bakta_dir)
+
     wf = Workflow(master)
 
     # If only 1 snakemake command should be run
     if master.snake:
         logging.info('Only running '+master.snake+' snakefile')
         wf.run(snakefile=globals()['WORKFLOW_'+master.snake])
 
@@ -123,15 +136,15 @@
                      ', ANI Cutoff: ' + str(master.ani_cutoff) + ', Contig Number: ' + str(master.contig_number) + ', N50: ' + str(master.n50))
         wf.run(snakefile=WORKFLOW_QUALITY)
 
     # If workflow is set to Pangenome
     elif (master.workflow == "pangenome"):
         logging.info('Run pangenome creation and analysis')
         logging.info('The parameters used in this study are- Eggnog Database Directory: ' + master.eggnog_dir +
-                     ', Kraken Database Directory: ' + master.kraken_dir + ', Bakta Database Directory: ' + master.bakta_dir)
+                     ', Bakta Database Directory: ' + master.bakta_dir)
         wf.run(snakefile=WORKFLOW_PANGENOME)
 
     # If workflow is set to Pyseer
     elif (master.workflow == "pyseer"):
         logging.info('Run genome-wide association study')
         logging.info(
             'The parameters used in this study are- Phenotype column: ' + str(master.pheno_column))
```

### Comparing `panpiper-1.0.0/panpiper/test.py` & `panpiper-1.0.1/panpiper/test.py`

 * *Files identical despite different names*

### Comparing `panpiper-1.0.0/panpiper/tests/test_main.py` & `panpiper-1.0.1/panpiper/tests/test_main.py`

 * *Files identical despite different names*

### Comparing `panpiper-1.0.0/panpiper/tests/test_scripts/filter_isolates.py` & `panpiper-1.0.1/panpiper/tests/test_scripts/filter_isolates.py`

 * *Files identical despite different names*

### Comparing `panpiper-1.0.0/panpiper/tests/test_scripts/test_concat_amrfinder.py` & `panpiper-1.0.1/panpiper/tests/test_scripts/test_concat_amrfinder.py`

 * *Files identical despite different names*

### Comparing `panpiper-1.0.0/panpiper/workflow/assembly.smk` & `panpiper-1.0.1/panpiper/workflow/assembly.smk`

 * *Files identical despite different names*

### Comparing `panpiper-1.0.0/panpiper/workflow/pyseer.smk` & `panpiper-1.0.1/panpiper/workflow/pyseer.smk`

 * *Files identical despite different names*

### Comparing `panpiper-1.0.0/panpiper/workflow/quality.smk` & `panpiper-1.0.1/panpiper/workflow/quality.smk`

 * *Files 13% similar despite different names*

```diff
@@ -1,127 +1,137 @@
+# ----------------------------------------------------------------------------
+# Copyright (c) 2022--, Panpiper development team.
+#
+# Distributed under the terms of the Modified BSD License.
+#
+# The full license is in the file COPYING.txt, distributed with this software.
+# ----------------------------------------------------------------------------
 """
 Authors: Renee Oles
 Date Updated: 1/4/2022
-Purpose: Quality control
+Purpose: Quality Control
 """
+
 import os
 import subprocess
 import math
 import distutils.util
 
-
 OUT = config['out']
 FASTA = config['fasta']
 REFERENCE = config['ref']
 PARAMS = config['params']
 SAMPLE_LIST = config['list']
+PATH = config['scripts']
 SAMPLES_OUT = os.path.join(OUT, 'Quality/quality_report.html')
 
 with open(PARAMS, 'r') as fh:   
     fl = [x.strip().split() for x in fh.readlines()]
 param_dict = {x[0]: x[1] for x in fl}
 
 PARAMS_REF = param_dict["ref"]
 ANI_CUTOFF = param_dict["ani_cutoff"]
 CONTIG_NUMBER = param_dict["contig_number"]
 N50 = param_dict["n50"]
+CHECKM = param_dict['checkm_dir']
 
 def read_complete_files():
     with open(SAMPLE_LIST) as f:
         raw_reads = [sample for sample in f.read().split('\n') if len(sample) > 0]
         return(raw_reads)
 READS = read_complete_files()
 
 # Output
 rule all:
     input:
         SAMPLES_OUT,
 
-
 # Remove contigs smaller than 500 bp
 # 30 sec per file
+# Define a function to dynamically find the input file based on available extensions
+def find_assembly(wildcards):
+    for ext in ['fa', 'fna', 'fasta']:
+        path = os.path.join(FASTA, f"{wildcards.file}.{ext}")
+        if os.path.isfile(path):
+            return path
+    raise ValueError(f"No assembly file found for {wildcards.file} with extensions .fa, .fna, or .fasta")
+
 rule contig_filter:
     input:
-        assembly=os.path.join(FASTA,"{file}/contigs.fa"),
+        assembly=find_assembly,
     params:
         contig=500,
     conda:
         "envs/bbmap.yml"
     log:
-        os.path.join(OUT,"report/prokka_filter_{file}.log"),
+        os.path.join(OUT, "report/prokka_filter_{file}.log"),
     resources:
         mem="1G"
     threads: 1
     benchmark:
-        os.path.join(OUT,"benchmark/prokka_filter_{file}.benchmark"),    
+        os.path.join(OUT, "benchmark/prokka_filter_{file}.benchmark"),    
     output:
-        fna=os.path.join(OUT,"Quality/Assembly_filter/{file}/{file}.fna"),
+        fna=os.path.join(OUT, "Quality/Samples/{file}/{file}.fna"),
     shell:
-        "reformat.sh in={input.assembly} out={output} minlength={params.contig} &> {log}"
-
+        "reformat.sh in={input.assembly} out={output.fna} minlength={params.contig} &> {log}"
 
-# 5 minutes per sample
-rule run_checkm:
+rule run_checkm2:
     input:
-        file=os.path.join(OUT,"Quality/Assembly_filter/{file}/{file}.fna"),
+        file=os.path.join(OUT,"Quality/Samples/{file}/{file}.fna"),
     params:
-        binset=os.path.join(OUT,"Quality/Assembly_filter/{file}"),
+        binset=os.path.join(OUT,"Quality/checkm"),
+        checkmdb=os.path.join(CHECKM,"Quality/uniref100.KO.1.dmnd"),
     conda:
-        "envs/checkm.yml"
+        "envs/checkm2.yml"
     log:
-        log=os.path.join(OUT,"Quality/Assembly_filter/{file}/lineage.log"),
+        log=os.path.join(OUT,"report/checkm2_{file}.log"),
     benchmark:
-        os.path.join(OUT,"benchmark/checkm_{file}.benchmark"),
+        os.path.join(OUT,"benchmark/checkm2_{file}.benchmark"),
     output:
-        stats=os.path.join(OUT,"Quality/Assembly_filter/{file}/storage/bin_stats.analyze.tsv"),
+        stats=os.path.join(OUT,"Quality/Samples/{file}/checkm/quality_report.tsv"),
     shell:
         """
-        checkm lineage_wf -t 20 -x fna {params.binset} {params.binset} &> {log}
+        checkm2 predict --threads 20 --input {input} --database_path {params.checkmdb} --output-directory {params.binset} --force &> {log}
         """
 
-
 rule checkm_to_graph:
     input:
-        stats=expand(os.path.join(OUT,"Quality/Assembly_filter/{file}/storage/bin_stats.analyze.tsv"), file=READS),
+        stats=expand(os.path.join(OUT,"Quality/Samples/{file}/checkm/quality_report.tsv"), file=READS),
     params:
-        log=expand(os.path.join(OUT,"Quality/Assembly_filter/{file}/lineage.log"), file=READS),
-    conda:
-        "envs/r.yml"
+        outpref=OUT,
+        path=PATH,
     log:
-        os.path.join(OUT,"report/checkm_graph.log"),
+        os.path.join(OUT,"report/checkm_cat.log"),
     benchmark:
         os.path.join(OUT,"benchmark/checkm_graph.benchmark"),
     resources:
         mem="1G"
     threads: 1        
     output:
-        png=os.path.join(OUT,"Quality/CheckM/checkm_log.txt"),
-        stats=os.path.join(OUT,"Quality/CheckM/checkm_stats.txt"),
+        stats=os.path.join(OUT,"Quality/CheckM/checkm_cat.txt"),
     shell:
         """
-        Rscript panpiper/workflow/scripts/checkm-log.R {params.log}  &> {log}
-        Rscript panpiper/workflow/scripts/checkm_bin-stats.R {input.stats}  &> {log}
+        python {params.path}/checkm_cat.py {params.outpref} {input.stats} &> {log}
         """
 
-
 rule fastani:
     input:
         ref=REFERENCE,
-        file=os.path.join(OUT,"Quality/Assembly_filter/{file}/{file}.fna"),
+        file=os.path.join(OUT,"Quality/Samples/{file}/{file}.fna"),
     conda:
         "envs/fastani.yml"
     log:
         os.path.join(OUT,"report/fastani_{file}.log"),
     resources:
         mem="1G"
     threads: 1
     benchmark:
         os.path.join(OUT,"benchmark/fastani_{file}.benchmark"),    
     output:
-        temp(os.path.join(OUT,"Quality/FastANI/{file}.txt")),
+        os.path.join(OUT,"Quality/FastANI/{file}.txt"),
     shell:
         "fastANI -q {input.file} -r {input.ref} -o {output} &> {log}"
 
 
 rule fastani_concat:
     input:
         expand(os.path.join(OUT,"Quality/FastANI/{file}.txt"), file=READS),
@@ -135,41 +145,39 @@
 
 
 # Filter files based off user-defined rules
 # Need to edit this python file bc it's messy rn
 rule filter_files:
     input:
         ani=os.path.join(OUT,"Quality/FastANI/fastani_summary.txt"),
-        stat=os.path.join(OUT,"Quality/CheckM/checkm_stats.txt"),
+        checkm=os.path.join(OUT,"Quality/CheckM/checkm_cat.txt"),
     params:
-        checkm=os.path.join(OUT,"Quality/CheckM/checkm_log.txt"),
         outpath=os.path.join(OUT,"Quality"),
         ref=PARAMS_REF,
         ac=ANI_CUTOFF,
-        cn=CONTIG_NUMBER,
         n=N50,
+        path=PATH,
     log:
         os.path.join(OUT,"report/filter_files.log"),
     benchmark:
         os.path.join(OUT,"benchmark/filter_files.benchmark"),    
     resources:
         mem="1G"
     threads: 1
     output:
         os.path.join(OUT,"Quality/sample_list.txt"),
     shell:
         """
-        python panpiper/workflow/scripts/filter_isolates.py -o {params.outpath} -a {input.ani} -l {params.checkm} -s {input.stat} -r {params.ref} -ac {params.ac} -cn {params.cn} -n {params.n} &> {log}
+        python {params.path}/filter_isolates.py -o {params.outpath} -a {input.ani} -k {input.checkm} -r {params.ref} -ac {params.ac} -n {params.n} &> {log}
         """
 
 rule print_results:
     input:
         ani=os.path.join(OUT,"Quality/FastANI/fastani_summary.txt"),
-        stat=os.path.join(OUT,"Quality/CheckM/checkm_stats.txt"),
-        log=os.path.join(OUT,"Quality/CheckM/checkm_log.txt"),
+        checkm=os.path.join(OUT,"Quality/CheckM/checkm_cat.txt"),
         passed=os.path.join(OUT,"Quality/sample_list.txt"),
     params:
         ref=PARAMS_REF,
         outdir=os.path.join(OUT, 'Quality')
     conda:
         "envs/r.yml"
     log:
@@ -178,10 +186,10 @@
         os.path.join(OUT,"benchmark/print_results.benchmark"),    
     resources:
         mem="5G"
     threads: 1
     output:
         SAMPLES_OUT,
     shell:
-        "Rscript -e \"rmarkdown::render('panpiper/workflow/scripts/quality_report.Rmd', output_dir = '{params.outdir}', params=list(checkm = '{input.stat}', log = '{input.log}', ani = '{input.ani}', passed = '{input.passed}', ref = '{params.ref}'))\" &> {log}"
+        "Rscript -e \"rmarkdown::render('panpiper/workflow/scripts/quality_report.Rmd', output_dir = '{params.outdir}', params=list(checkm = '{input.checkm}', ani = '{input.ani}', passed = '{input.passed}', ref = '{params.ref}'))\" &> {log}"
```

### Comparing `panpiper-1.0.0/panpiper/workflow.py` & `panpiper-1.0.1/panpiper/workflow.py`

 * *Files 2% similar despite different names*

```diff
@@ -51,14 +51,15 @@
                'list='+self.sample_list,
                'ref='+self.reference,
                'structure='+self.structure,
                'unitig='+self.unitig,
                'tree='+self.tree,
                'genes='+self.genes,
                'pheno='+self.pheno,
+               'scripts='+self.scripts_dir,
                'params='+self.params]
 
         # If run on cluster
         if self.cluster:
             cmd += ['--profile', self.profile]
 
         # Only install conda envs if only_conda
```

### Comparing `panpiper-1.0.0/panpiper.egg-info/PKG-INFO` & `panpiper-1.0.1/panpiper.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,23 +1,35 @@
 Metadata-Version: 2.1
 Name: panpiper
-Version: 1.0.0
+Version: 1.0.1
 Summary: Panpiper: snakemake workflow for bacterial isolate analysis
 Home-page: https://github.com/rolesucsd/Panpiper
 Author: Renee Oles
 Author-email: roles@health.ucsd.edu
 License: BSD-3-Clause
 Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
+Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Development Status :: 3 - Alpha
 Requires-Python: >=3.5
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: setuptools
+Requires-Dist: biopython>=1.78
+Requires-Dist: pandas>=1.0.0
+Requires-Dist: numpy>=1.19.2
+Requires-Dist: matplotlib>=3.1.0
+Requires-Dist: seaborn>=0.10.0
+Requires-Dist: scikit-learn>=0.22.0
+Requires-Dist: scipy>=1.4.0
+Requires-Dist: scikit-bio>=0.5.6
+Requires-Dist: umap-learn>=0.4.0
+Requires-Dist: dendropy>=4.5.0
+Requires-Dist: PyYAML>=5.3
 
 [![Project Status: Active - The project has reached a stable, usable state and is being actively developed.](http://www.repostatus.org/badges/latest/active.svg)](http://www.repostatus.org/#active)
 
 # Panpiper
 
 This package conducts bacterial isolate analysis for one species.  
 
@@ -73,15 +85,15 @@
 * Assembly/  
     * incomplete_assembly_files.txt - samples for which assembly failed
     *  complete_assembly_files.txt - samples for which assemblies passed 
     * {sample}/  
         * contigs.fa - edited assembly 
 
 ### Quality control: 
-The fasta file directory should contain a subdirectory for each sample where the subdirectory name is the sample of the sample. The fasta file within these directories should be formatted as contigs.fa. This is the standard output from Shovill. The sample list should have one sample name per line which corresponds to the directory names. The reference fasta file should be the representative strain of the species which the samples will be compared to using average nucleotide identity.
+The fasta file directory should contain a subdirectory for each sample where the subdirectory name is the sample of the sample. The fasta file within these directories should be formatted as contigs.fa. This is the standard output from Shovill. The sample list should have one sample name per line which corresponds to the name of the fasta file. The reference fasta file should be the representative strain of the species which the samples will be compared to using average nucleotide identity.
 
 Additional parameters that may be included:
 * --ani_cutoff : percent identity to reference cutoff (default 95)
 * --n50 : N50 cutoff (default 5000)
 * --contig_number : number of contigs cutoff (default 1000)
 
 ```sh
```

