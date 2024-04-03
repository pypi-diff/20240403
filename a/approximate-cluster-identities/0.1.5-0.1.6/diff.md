# Comparing `tmp/approximate_cluster_identities-0.1.5.tar.gz` & `tmp/approximate_cluster_identities-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "approximate_cluster_identities-0.1.5.tar", last modified: Wed Apr  3 12:51:49 2024, max compression
+gzip compressed data, was "approximate_cluster_identities-0.1.6.tar", last modified: Wed Apr  3 14:52:27 2024, max compression
```

## Comparing `approximate_cluster_identities-0.1.5.tar` & `approximate_cluster_identities-0.1.6.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 12:51:49.496138 approximate_cluster_identities-0.1.5/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-03 12:51:41.000000 approximate_cluster_identities-0.1.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3549 2024-04-03 12:51:49.496138 approximate_cluster_identities-0.1.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2946 2024-04-03 12:51:41.000000 approximate_cluster_identities-0.1.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 12:51:49.496138 approximate_cluster_identities-0.1.5/approximate_cluster_identities/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 12:51:41.000000 approximate_cluster_identities-0.1.5/approximate_cluster_identities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10021 2024-04-03 12:51:41.000000 approximate_cluster_identities-0.1.5/approximate_cluster_identities/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 12:51:49.496138 approximate_cluster_identities-0.1.5/approximate_cluster_identities.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3549 2024-04-03 12:51:49.000000 approximate_cluster_identities-0.1.5/approximate_cluster_identities.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      438 2024-04-03 12:51:49.000000 approximate_cluster_identities-0.1.5/approximate_cluster_identities.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 12:51:49.000000 approximate_cluster_identities-0.1.5/approximate_cluster_identities.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-03 12:51:49.000000 approximate_cluster_identities-0.1.5/approximate_cluster_identities.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       72 2024-04-03 12:51:49.000000 approximate_cluster_identities-0.1.5/approximate_cluster_identities.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-04-03 12:51:49.000000 approximate_cluster_identities-0.1.5/approximate_cluster_identities.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-03 12:51:49.496138 approximate_cluster_identities-0.1.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1200 2024-04-03 12:51:41.000000 approximate_cluster_identities-0.1.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 14:52:27.680770 approximate_cluster_identities-0.1.6/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-03 14:52:19.000000 approximate_cluster_identities-0.1.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3549 2024-04-03 14:52:27.680770 approximate_cluster_identities-0.1.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2946 2024-04-03 14:52:19.000000 approximate_cluster_identities-0.1.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 14:52:27.680770 approximate_cluster_identities-0.1.6/approximate_cluster_identities/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 14:52:19.000000 approximate_cluster_identities-0.1.6/approximate_cluster_identities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10607 2024-04-03 14:52:19.000000 approximate_cluster_identities-0.1.6/approximate_cluster_identities/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 14:52:27.680770 approximate_cluster_identities-0.1.6/approximate_cluster_identities.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3549 2024-04-03 14:52:27.000000 approximate_cluster_identities-0.1.6/approximate_cluster_identities.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      438 2024-04-03 14:52:27.000000 approximate_cluster_identities-0.1.6/approximate_cluster_identities.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 14:52:27.000000 approximate_cluster_identities-0.1.6/approximate_cluster_identities.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-03 14:52:27.000000 approximate_cluster_identities-0.1.6/approximate_cluster_identities.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-04-03 14:52:27.000000 approximate_cluster_identities-0.1.6/approximate_cluster_identities.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-04-03 14:52:27.000000 approximate_cluster_identities-0.1.6/approximate_cluster_identities.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-03 14:52:27.680770 approximate_cluster_identities-0.1.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1200 2024-04-03 14:52:19.000000 approximate_cluster_identities-0.1.6/setup.py
```

### Comparing `approximate_cluster_identities-0.1.5/LICENSE` & `approximate_cluster_identities-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `approximate_cluster_identities-0.1.5/PKG-INFO` & `approximate_cluster_identities-0.1.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: approximate_cluster_identities
-Version: 0.1.5
+Version: 0.1.6
 Summary: A package to calculate and visualise approximate cluster identities for a large number of short nucleotide sequences using minimizers.
 Author: Daniel Anderson
 Author-email: danp.anderson@outlook.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `approximate_cluster_identities-0.1.5/README.md` & `approximate_cluster_identities-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `approximate_cluster_identities-0.1.5/approximate_cluster_identities/__main__.py` & `approximate_cluster_identities-0.1.6/approximate_cluster_identities/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 from Bio import SeqIO
 from itertools import combinations
 from joblib import Parallel, delayed
 import json
 import networkx as nx
 import numpy as np
 import pandas as pd
+import random
 import sourmash
 import seaborn as sns
 import statistics
 import sys
 from tqdm import tqdm
 
 def read_metadata(input_json):
@@ -24,27 +25,28 @@
     return minhash
 
 def calculate_minimizers(seqRecord, k, w):
     sequence = str(seqRecord.seq)
     return (seqRecord.id, get_minhash(sequence, k, w))
 
 def calculate_distance(chunk,
+                kmer_sets_dict,
                 shorter):
     distances = []
     for c in tqdm(chunk):
-        seq1 = c[0]
-        seq2 = c[1]
+        seq1 = kmer_sets_dict[c[0]]
+        seq2 = kmer_sets_dict[c[1]]
         if not shorter:
-            dist = seq1[1].jaccard(seq2[1])
+            dist = seq1.jaccard(seq2)
         else:
-            seq1_hashes = set(seq1[1].hashes)
-            seq2_hashes = set(seq2[1].hashes)
+            seq1_hashes = set(seq1.hashes)
+            seq2_hashes = set(seq2.hashes)
             intersection_length = len(seq1_hashes & seq2_hashes)
             dist = float(max([intersection_length / len(seq1_hashes), intersection_length / len(seq2_hashes)]))
-        distances.append((seq1[0], seq2[0], dist))
+        distances.append((c[0], c[1], dist))
     return distances
 
 def write_distance_gml(sequence_records,
                     distance_df,
                     metadata,
                     output_gml):
     G = nx.Graph()
@@ -155,28 +157,42 @@
     # parse command line arguements
     args = get_options()
     # read cluster assignment metadata
     metadata = read_metadata(args.input_json)
     # read fasta files
     sys.stderr.write("Reading sequences\n")
     sequence_records = list(SeqIO.parse(args.input_fasta, "fasta"))
+    # subsample the clusters
+    random.shuffle(sequence_records)
+    cluster_count = set()
+    subsampled_records = []
+    for record in sequence_records:
+        if len(cluster_count) < 2500:
+            subsampled_records.append(record)
+            cluster_count.add(metadata[record.id])
+        else:
+            break
     # extract minimisers from sequences
     sys.stderr.write(f"Extracting minimisers using {str(args.threads)} threads...\n")
     kmer_sets = Parallel(n_jobs=args.threads)(delayed(calculate_minimizers)(seq,
                                                                         args.kmerSize,
-                                                                        args.windowSize) for seq in tqdm(sequence_records))
+                                                                        args.windowSize) for seq in tqdm(subsampled_records))
+    kmer_sets_dict = {}
+    for pair in kmer_sets:
+        kmer_sets_dict[pair[0]] = pair[1]
+    # Get all unique pairs of sequences
+    sys.stderr.write(f"Enumerating all sequence combinations...\n")
+    all_comparisons = [c for c in tqdm(combinations(list(kmer_sets_dict.keys()), 2))]
     # Calculate distances
     sys.stderr.write(f"Calculating approximate jaccard distances using {str(args.threads)} threads...\n")
     distances = []
-    # Get all unique pairs of sequences
-    all_comparisons = [c for c in combinations(kmer_sets, 2)]
     # Split pairs into chunks based on the number of threads
     chunks = np.array_split(all_comparisons, args.threads)
     # Calculate approximate jaccard distances
-    chunk_distances = Parallel(n_jobs=args.threads)(delayed(calculate_distance)(c, args.shorter) for c in chunks)
+    chunk_distances = Parallel(n_jobs=args.threads)(delayed(calculate_distance)(c, kmer_sets_dict, args.shorter) for c in chunks)
     for thread_distances in chunk_distances:
         distances += thread_distances
     # convert pairwise distances to dataframe
     cluster_df = pd.DataFrame(distances, columns=['seq1', 'seq2', 'identity'])
     if args.clusterPlot:
         # separate between cluster and within cluster distances
         sys.stderr.write("Making jointplot of all pairwise identities...\n")
```

### Comparing `approximate_cluster_identities-0.1.5/approximate_cluster_identities.egg-info/PKG-INFO` & `approximate_cluster_identities-0.1.6/approximate_cluster_identities.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: approximate-cluster-identities
-Version: 0.1.5
+Version: 0.1.6
 Summary: A package to calculate and visualise approximate cluster identities for a large number of short nucleotide sequences using minimizers.
 Author: Daniel Anderson
 Author-email: danp.anderson@outlook.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `approximate_cluster_identities-0.1.5/setup.py` & `approximate_cluster_identities-0.1.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 # Read the contents of your README file
 with open('README.md', 'r', encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='approximate_cluster_identities',
-    version='0.1.5',
+    version='0.1.6',
     description='A package to calculate and visualise approximate cluster identities for a large number of short nucleotide sequences using minimizers.',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author='Daniel Anderson',
     author_email='danp.anderson@outlook.com',
     packages=find_packages(),
     install_requires=[
```

