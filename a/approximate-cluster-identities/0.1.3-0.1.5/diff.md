# Comparing `tmp/approximate_cluster_identities-0.1.3.tar.gz` & `tmp/approximate_cluster_identities-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "approximate_cluster_identities-0.1.3.tar", last modified: Mon May  8 11:19:26 2023, max compression
+gzip compressed data, was "approximate_cluster_identities-0.1.5.tar", last modified: Wed Apr  3 12:51:49 2024, max compression
```

## Comparing `approximate_cluster_identities-0.1.3.tar` & `approximate_cluster_identities-0.1.5.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 11:19:26.556341 approximate_cluster_identities-0.1.3/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-08 11:19:14.000000 approximate_cluster_identities-0.1.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3523 2023-05-08 11:19:26.556341 approximate_cluster_identities-0.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2920 2023-05-08 11:19:14.000000 approximate_cluster_identities-0.1.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 11:19:26.552341 approximate_cluster_identities-0.1.3/approximate_cluster_identities/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 11:19:14.000000 approximate_cluster_identities-0.1.3/approximate_cluster_identities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10978 2023-05-08 11:19:14.000000 approximate_cluster_identities-0.1.3/approximate_cluster_identities/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 11:19:26.556341 approximate_cluster_identities-0.1.3/approximate_cluster_identities.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3523 2023-05-08 11:19:26.000000 approximate_cluster_identities-0.1.3/approximate_cluster_identities.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      438 2023-05-08 11:19:26.000000 approximate_cluster_identities-0.1.3/approximate_cluster_identities.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 11:19:26.000000 approximate_cluster_identities-0.1.3/approximate_cluster_identities.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-05-08 11:19:26.000000 approximate_cluster_identities-0.1.3/approximate_cluster_identities.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-05-08 11:19:26.000000 approximate_cluster_identities-0.1.3/approximate_cluster_identities.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-05-08 11:19:26.000000 approximate_cluster_identities-0.1.3/approximate_cluster_identities.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-08 11:19:26.556341 approximate_cluster_identities-0.1.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1180 2023-05-08 11:19:14.000000 approximate_cluster_identities-0.1.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 12:51:49.496138 approximate_cluster_identities-0.1.5/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-03 12:51:41.000000 approximate_cluster_identities-0.1.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3549 2024-04-03 12:51:49.496138 approximate_cluster_identities-0.1.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2946 2024-04-03 12:51:41.000000 approximate_cluster_identities-0.1.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 12:51:49.496138 approximate_cluster_identities-0.1.5/approximate_cluster_identities/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 12:51:41.000000 approximate_cluster_identities-0.1.5/approximate_cluster_identities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10021 2024-04-03 12:51:41.000000 approximate_cluster_identities-0.1.5/approximate_cluster_identities/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 12:51:49.496138 approximate_cluster_identities-0.1.5/approximate_cluster_identities.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3549 2024-04-03 12:51:49.000000 approximate_cluster_identities-0.1.5/approximate_cluster_identities.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      438 2024-04-03 12:51:49.000000 approximate_cluster_identities-0.1.5/approximate_cluster_identities.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 12:51:49.000000 approximate_cluster_identities-0.1.5/approximate_cluster_identities.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-03 12:51:49.000000 approximate_cluster_identities-0.1.5/approximate_cluster_identities.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-04-03 12:51:49.000000 approximate_cluster_identities-0.1.5/approximate_cluster_identities.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-04-03 12:51:49.000000 approximate_cluster_identities-0.1.5/approximate_cluster_identities.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-03 12:51:49.496138 approximate_cluster_identities-0.1.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1200 2024-04-03 12:51:41.000000 approximate_cluster_identities-0.1.5/setup.py
```

### Comparing `approximate_cluster_identities-0.1.3/LICENSE` & `approximate_cluster_identities-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `approximate_cluster_identities-0.1.3/PKG-INFO` & `approximate_cluster_identities-0.1.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: approximate_cluster_identities
-Version: 0.1.3
-Summary: A package to calculate and visualise approximate cluster identities for a large number of short nucleotide sequences using minimisers.
+Version: 0.1.5
+Summary: A package to calculate and visualise approximate cluster identities for a large number of short nucleotide sequences using minimizers.
 Author: Daniel Anderson
 Author-email: danp.anderson@outlook.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Approximate Cluster Identities (ACI)
 
-A python package to visualise the approximate within and between cluster identities of short sequences as assigned by e.g. mmseqs2, cd-hit or panaroo.
+A python package to visualise the approximate within and between cluster identities of a large number of short sequences as assigned by e.g. mmseqs2, cd-hit or panaroo.
 
 # Installation
 ```
 pip install approximate-cluster-identities
 ```
 
 # Usage
@@ -47,15 +47,15 @@
                         Jaccard similarity threshold (default: 0.9).
   --threads THREADS     Threads for sketching and jaccard distance calculations (default: 1).
   --shorter             Assess identity relative to the shorter sequence.
 ```
 
 # Methods
 
-We calculate sequence identities by pairwise calculation of jaccard distances using minimizers of size ```--kmerSize``` where 1 *k*-mer is sampled from a window of a total of ```--windowSize``` *k*-mers that slides across the input sequences. Increasing ```--windowSize``` will decrease the number of minimizers per sequence, decreasing the sensitivity of the identity calculations but increasing the speed of the programme. This tool is designed to give you an idea of how variable a large number of short sequences are within and between clusters to choose an appropriate sequencing clustering tool and its parameters.
+We calculate sequence identities by pairwise calculation of jaccard distances using minimizers of size ```--kmerSize``` where 1 *k*-mer is sampled from a window that slides across each sequence, each containing a total of ```--windowSize``` *k*-mers. Increasing ```--windowSize``` will decrease the number of minimizers per sequence, decreasing the sensitivity of the identity calculations but increasing the speed of the programme. This tool is designed to give you an idea of how variable a large number of short sequences are within and between clusters to choose an appropriate sequencing clustering tool and its parameters.
 
 # Example output
 
 Example cluster plots for data in ```test/``` using ```--windowSize 1``` and ```--windowSize 100```.
 
 ### Window size = 1
```

### Comparing `approximate_cluster_identities-0.1.3/README.md` & `approximate_cluster_identities-0.1.5/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # Approximate Cluster Identities (ACI)
 
-A python package to visualise the approximate within and between cluster identities of short sequences as assigned by e.g. mmseqs2, cd-hit or panaroo.
+A python package to visualise the approximate within and between cluster identities of a large number of short sequences as assigned by e.g. mmseqs2, cd-hit or panaroo.
 
 # Installation
 ```
 pip install approximate-cluster-identities
 ```
 
 # Usage
@@ -33,15 +33,15 @@
                         Jaccard similarity threshold (default: 0.9).
   --threads THREADS     Threads for sketching and jaccard distance calculations (default: 1).
   --shorter             Assess identity relative to the shorter sequence.
 ```
 
 # Methods
 
-We calculate sequence identities by pairwise calculation of jaccard distances using minimizers of size ```--kmerSize``` where 1 *k*-mer is sampled from a window of a total of ```--windowSize``` *k*-mers that slides across the input sequences. Increasing ```--windowSize``` will decrease the number of minimizers per sequence, decreasing the sensitivity of the identity calculations but increasing the speed of the programme. This tool is designed to give you an idea of how variable a large number of short sequences are within and between clusters to choose an appropriate sequencing clustering tool and its parameters.
+We calculate sequence identities by pairwise calculation of jaccard distances using minimizers of size ```--kmerSize``` where 1 *k*-mer is sampled from a window that slides across each sequence, each containing a total of ```--windowSize``` *k*-mers. Increasing ```--windowSize``` will decrease the number of minimizers per sequence, decreasing the sensitivity of the identity calculations but increasing the speed of the programme. This tool is designed to give you an idea of how variable a large number of short sequences are within and between clusters to choose an appropriate sequencing clustering tool and its parameters.
 
 # Example output
 
 Example cluster plots for data in ```test/``` using ```--windowSize 1``` and ```--windowSize 100```.
 
 ### Window size = 1
```

### Comparing `approximate_cluster_identities-0.1.3/approximate_cluster_identities/__main__.py` & `approximate_cluster_identities-0.1.5/approximate_cluster_identities/__main__.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,83 +2,66 @@
 from Bio import SeqIO
 from itertools import combinations
 from joblib import Parallel, delayed
 import json
 import networkx as nx
 import numpy as np
 import pandas as pd
+import sourmash
 import seaborn as sns
 import statistics
 import sys
 from tqdm import tqdm
 
 def read_metadata(input_json):
     with open(input_json, 'r') as f:
         metadata = json.load(f)
     return metadata
 
-def rolling_hash(seq, k, base=4):
-    hash_value = 0
-    for i in range(k):
-        hash_value = hash_value * base + ord(seq[i])
-    return hash_value
-
-def update_rolling_hash(prev_hash, prev_kmer, next_kmer, k, base=4):
-    return (prev_hash - ord(prev_kmer[0]) * (base ** (k - 1))) * base + ord(next_kmer[-1])
+def get_minhash(sequence, k, w):
+    assert not len(sequence) < w + k, f"The value of k or w is too large. Their sum should be no less than {len(sequence)}."
+    minhash = sourmash.MinHash(n=0, ksize=k, scaled=w)
+    minhash.add_sequence(sequence, force=True)
+    return minhash
 
 def calculate_minimizers(seqRecord, k, w):
-    rev_comp_sequence = str(seqRecord.reverse_complement().seq)
     sequence = str(seqRecord.seq)
+    return (seqRecord.id, get_minhash(sequence, k, w))
 
-    # Initialize hashes for the first k-mer in both strands
-    hash_forward = rolling_hash(sequence[:k], k)
-    hash_rev_comp = rolling_hash(rev_comp_sequence[:k], k)
-
-    hashes_forward = [hash_forward]
-    hashes_rev_comp = [hash_rev_comp]
-
-    # Calculate rolling hashes for the rest of the k-mers in both strands
-    for i in range(1, len(sequence) - k + 1):
-        hash_forward = update_rolling_hash(hash_forward, sequence[i-1:i-1+k], sequence[i:i+k], k)
-        hash_rev_comp = update_rolling_hash(hash_rev_comp, rev_comp_sequence[i-1:i-1+k], rev_comp_sequence[i:i+k], k)
-        hashes_forward.append(hash_forward)
-        hashes_rev_comp.append(hash_rev_comp)
-
-    # Find minimizers in windows of w consecutive k-mers
-    minimizers = set([min(min(hashes_forward[i:i+w]), min(hashes_rev_comp[i:i+w])) for i in range(len(hashes_forward) - w + 1)])
-    assert not len(minimizers) == 0, "Your chosen windowSize is larger than your shortest sequence. Reduce the windowSize and rerun the tool."
-    return (seqRecord.id, minimizers)
-
-def calculate_jaccard_distance(chunk,
-                            shorter):
+def calculate_distance(chunk,
+                shorter):
     distances = []
     for c in tqdm(chunk):
         seq1 = c[0]
         seq2 = c[1]
-        len_intersection = len(seq1[1].intersection(seq2[1]))
         if not shorter:
-            dist = float(len_intersection / (len(seq1[1]) + len(seq2[1]) - len_intersection))
+            dist = seq1[1].jaccard(seq2[1])
         else:
-            shorter = seq1[1] if len(seq1[1]) < len(seq2[1]) else seq2[1]
-            dist = float(len_intersection / len(shorter))
+            seq1_hashes = set(seq1[1].hashes)
+            seq2_hashes = set(seq2[1].hashes)
+            intersection_length = len(seq1_hashes & seq2_hashes)
+            dist = float(max([intersection_length / len(seq1_hashes), intersection_length / len(seq2_hashes)]))
         distances.append((seq1[0], seq2[0], dist))
     return distances
 
 def write_distance_gml(sequence_records,
-                    mash_df,
+                    distance_df,
                     metadata,
                     output_gml):
     G = nx.Graph()
     sys.stderr.write("\t\tWriting nodes...\n")
     for seq in tqdm(sequence_records):
         G.add_node(seq.id, cluster=metadata[seq.id])
     sys.stderr.write("\t\tWriting edges...\n")
-    for idx, row in tqdm(mash_df.iterrows()):
-        G.add_edge(row['seq1'], row['seq2'], weight=row['identity'])
-    nx.write_gml(G, output_gml)
+    seq1 = list(distance_df["seq1"])
+    seq2 = list(distance_df["seq2"])
+    identity = list(distance_df["identity"])
+    for i in tqdm(range(len(seq1))):
+        G.add_edge(seq1[i], seq2[i], weight=identity[i])
+    nx.write_gml(G, output_gml + ".gml")
 
 def calculate_cluster_stats(cluster_df, metadata):
     seq1 = [metadata[s] for s in list(cluster_df["seq1"])]
     seq2 = [metadata[s] for s in list(cluster_df["seq2"])]
     cluster_df["seq1_cluster"] = seq1
     cluster_df["seq2_cluster"] = seq2
     cluster_df["Same cluster"] = cluster_df["seq1"] == cluster_df["seq2"]
@@ -185,15 +168,15 @@
     sys.stderr.write(f"Calculating approximate jaccard distances using {str(args.threads)} threads...\n")
     distances = []
     # Get all unique pairs of sequences
     all_comparisons = [c for c in combinations(kmer_sets, 2)]
     # Split pairs into chunks based on the number of threads
     chunks = np.array_split(all_comparisons, args.threads)
     # Calculate approximate jaccard distances
-    chunk_distances = Parallel(n_jobs=args.threads)(delayed(calculate_jaccard_distance)(c, args.shorter) for c in chunks)
+    chunk_distances = Parallel(n_jobs=args.threads)(delayed(calculate_distance)(c, args.shorter) for c in chunks)
     for thread_distances in chunk_distances:
         distances += thread_distances
     # convert pairwise distances to dataframe
     cluster_df = pd.DataFrame(distances, columns=['seq1', 'seq2', 'identity'])
     if args.clusterPlot:
         # separate between cluster and within cluster distances
         sys.stderr.write("Making jointplot of all pairwise identities...\n")
```

### Comparing `approximate_cluster_identities-0.1.3/approximate_cluster_identities.egg-info/PKG-INFO` & `approximate_cluster_identities-0.1.5/approximate_cluster_identities.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: approximate-cluster-identities
-Version: 0.1.3
-Summary: A package to calculate and visualise approximate cluster identities for a large number of short nucleotide sequences using minimisers.
+Version: 0.1.5
+Summary: A package to calculate and visualise approximate cluster identities for a large number of short nucleotide sequences using minimizers.
 Author: Daniel Anderson
 Author-email: danp.anderson@outlook.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Approximate Cluster Identities (ACI)
 
-A python package to visualise the approximate within and between cluster identities of short sequences as assigned by e.g. mmseqs2, cd-hit or panaroo.
+A python package to visualise the approximate within and between cluster identities of a large number of short sequences as assigned by e.g. mmseqs2, cd-hit or panaroo.
 
 # Installation
 ```
 pip install approximate-cluster-identities
 ```
 
 # Usage
@@ -47,15 +47,15 @@
                         Jaccard similarity threshold (default: 0.9).
   --threads THREADS     Threads for sketching and jaccard distance calculations (default: 1).
   --shorter             Assess identity relative to the shorter sequence.
 ```
 
 # Methods
 
-We calculate sequence identities by pairwise calculation of jaccard distances using minimizers of size ```--kmerSize``` where 1 *k*-mer is sampled from a window of a total of ```--windowSize``` *k*-mers that slides across the input sequences. Increasing ```--windowSize``` will decrease the number of minimizers per sequence, decreasing the sensitivity of the identity calculations but increasing the speed of the programme. This tool is designed to give you an idea of how variable a large number of short sequences are within and between clusters to choose an appropriate sequencing clustering tool and its parameters.
+We calculate sequence identities by pairwise calculation of jaccard distances using minimizers of size ```--kmerSize``` where 1 *k*-mer is sampled from a window that slides across each sequence, each containing a total of ```--windowSize``` *k*-mers. Increasing ```--windowSize``` will decrease the number of minimizers per sequence, decreasing the sensitivity of the identity calculations but increasing the speed of the programme. This tool is designed to give you an idea of how variable a large number of short sequences are within and between clusters to choose an appropriate sequencing clustering tool and its parameters.
 
 # Example output
 
 Example cluster plots for data in ```test/``` using ```--windowSize 1``` and ```--windowSize 100```.
 
 ### Window size = 1
```

### Comparing `approximate_cluster_identities-0.1.3/setup.py` & `approximate_cluster_identities-0.1.5/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,28 +2,29 @@
 
 # Read the contents of your README file
 with open('README.md', 'r', encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='approximate_cluster_identities',
-    version='0.1.3',
-    description='A package to calculate and visualise approximate cluster identities for a large number of short nucleotide sequences using minimisers.',
+    version='0.1.5',
+    description='A package to calculate and visualise approximate cluster identities for a large number of short nucleotide sequences using minimizers.',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author='Daniel Anderson',
     author_email='danp.anderson@outlook.com',
     packages=find_packages(),
     install_requires=[
         'biopython',
         'pandas',
         'matplotlib',
         'networkx',
         'numpy',
         'seaborn',
+        'sourmash',
         'tqdm',
         'joblib'
     ],
     entry_points={
         'console_scripts': [
             'aci=approximate_cluster_identities.__main__:main',
         ],
```

