# Comparing `tmp/protkit-0.2.1.tar.gz` & `tmp/protkit-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "protkit-0.2.1.tar", last modified: Fri Mar  8 07:10:54 2024, max compression
+gzip compressed data, was "protkit-0.2.2.tar", last modified: Wed Apr  3 08:16:43 2024, max compression
```

## Comparing `protkit-0.2.1.tar` & `protkit-0.2.2.tar`

### file list

```diff
@@ -1,81 +1,84 @@
-drwxrwxr-x   0 fred      (1000) fred      (1000)        0 2024-03-08 07:10:54.295503 protkit-0.2.1/
--rw-rw-r--   0 fred      (1000) fred      (1000)    35149 2024-02-20 10:58:14.000000 protkit-0.2.1/LICENSE
--rw-r--r--   0 fred      (1000) fred      (1000)    18905 2024-03-08 07:10:54.295503 protkit-0.2.1/PKG-INFO
--rw-rw-r--   0 fred      (1000) fred      (1000)    17718 2024-03-06 07:08:30.000000 protkit-0.2.1/README.md
-drwxrwxr-x   0 fred      (1000) fred      (1000)        0 2024-03-08 07:10:54.291503 protkit-0.2.1/protkit/
--rw-rw-r--   0 fred      (1000) fred      (1000)     5279 2024-03-08 06:45:24.000000 protkit-0.2.1/protkit/__init__.py
-drwxrwxr-x   0 fred      (1000) fred      (1000)        0 2024-03-08 07:10:54.291503 protkit-0.2.1/protkit/core/
--rw-rw-r--   0 fred      (1000) fred      (1000)      135 2024-02-20 13:59:59.000000 protkit-0.2.1/protkit/core/__init__.py
--rw-rw-r--   0 fred      (1000) fred      (1000)     2609 2024-01-30 10:27:10.000000 protkit-0.2.1/protkit/core/extend_attributes.py
-drwxrwxr-x   0 fred      (1000) fred      (1000)        0 2024-03-08 07:10:54.291503 protkit-0.2.1/protkit/download/
--rw-rw-r--   0 fred      (1000) fred      (1000)      395 2024-02-20 11:32:28.000000 protkit-0.2.1/protkit/download/__init__.py
--rw-rw-r--   0 fred      (1000) fred      (1000)    12999 2024-02-28 11:30:48.000000 protkit-0.2.1/protkit/download/download.py
-drwxrwxr-x   0 fred      (1000) fred      (1000)        0 2024-03-08 07:10:54.291503 protkit-0.2.1/protkit/file_io/
--rw-rw-r--   0 fred      (1000) fred      (1000)      786 2024-02-20 11:40:22.000000 protkit-0.2.1/protkit/file_io/__init__.py
--rw-rw-r--   0 fred      (1000) fred      (1000)     3860 2024-02-20 11:40:22.000000 protkit-0.2.1/protkit/file_io/fasta_io.py
--rw-rw-r--   0 fred      (1000) fred      (1000)     3532 2024-02-20 11:40:22.000000 protkit-0.2.1/protkit/file_io/mmcif_io.py
--rw-rw-r--   0 fred      (1000) fred      (1000)     3405 2024-02-20 11:40:22.000000 protkit-0.2.1/protkit/file_io/mmtf_io.py
--rw-rw-r--   0 fred      (1000) fred      (1000)    42078 2024-02-20 11:40:22.000000 protkit-0.2.1/protkit/file_io/pdb_io.py
--rw-rw-r--   0 fred      (1000) fred      (1000)     1134 2024-02-20 11:40:22.000000 protkit-0.2.1/protkit/file_io/pqr_io.py
--rw-rw-r--   0 fred      (1000) fred      (1000)     9969 2024-02-20 11:40:22.000000 protkit-0.2.1/protkit/file_io/prot_io.py
-drwxrwxr-x   0 fred      (1000) fred      (1000)        0 2024-03-08 07:10:54.291503 protkit-0.2.1/protkit/geometry/
--rw-rw-r--   0 fred      (1000) fred      (1000)      147 2024-02-23 12:55:57.000000 protkit-0.2.1/protkit/geometry/__init__.py
--rw-rw-r--   0 fred      (1000) fred      (1000)     7717 2024-02-15 08:53:21.000000 protkit-0.2.1/protkit/geometry/math.py
--rw-rw-r--   0 fred      (1000) fred      (1000)     5103 2024-02-15 12:04:44.000000 protkit-0.2.1/protkit/geometry/space_query.py
-drwxrwxr-x   0 fred      (1000) fred      (1000)        0 2024-03-08 07:10:54.291503 protkit-0.2.1/protkit/metrics/
--rw-rw-r--   0 fred      (1000) fred      (1000)     1160 2024-02-23 12:57:26.000000 protkit-0.2.1/protkit/metrics/__init__.py
--rw-rw-r--   0 fred      (1000) fred      (1000)      272 2024-01-24 11:20:02.000000 protkit-0.2.1/protkit/metrics/classification_eval.py
--rw-rw-r--   0 fred      (1000) fred      (1000)      259 2024-01-24 11:20:02.000000 protkit-0.2.1/protkit/metrics/regression_eval.py
--rw-rw-r--   0 fred      (1000) fred      (1000)     5566 2024-02-23 12:57:27.000000 protkit-0.2.1/protkit/metrics/scoring_matrix.py
--rw-rw-r--   0 fred      (1000) fred      (1000)     6063 2024-02-02 14:13:32.000000 protkit-0.2.1/protkit/metrics/sequence_eval.py
--rw-rw-r--   0 fred      (1000) fred      (1000)     3172 2024-01-31 09:20:40.000000 protkit-0.2.1/protkit/metrics/structure_eval.py
--rw-rw-r--   0 fred      (1000) fred      (1000)      339 2024-01-24 11:18:08.000000 protkit-0.2.1/protkit/metrics/utility_eval.py
-drwxrwxr-x   0 fred      (1000) fred      (1000)        0 2024-03-08 07:10:54.295503 protkit-0.2.1/protkit/properties/
--rw-rw-r--   0 fred      (1000) fred      (1000)     1076 2024-03-08 07:01:09.000000 protkit-0.2.1/protkit/properties/__init__.py
--rw-rw-r--   0 fred      (1000) fred      (1000)     9887 2024-02-14 09:21:12.000000 protkit-0.2.1/protkit/properties/bond_angles.py
--rw-rw-r--   0 fred      (1000) fred      (1000)    10870 2024-02-14 09:21:12.000000 protkit-0.2.1/protkit/properties/bond_lengths.py
--rw-rw-r--   0 fred      (1000) fred      (1000)    10763 2024-03-07 14:33:32.000000 protkit-0.2.1/protkit/properties/bounds.py
--rw-rw-r--   0 fred      (1000) fred      (1000)     4785 2024-02-06 10:51:06.000000 protkit-0.2.1/protkit/properties/charge.py
--rw-rw-r--   0 fred      (1000) fred      (1000)     4652 2024-03-06 08:28:16.000000 protkit-0.2.1/protkit/properties/chemical_class.py
--rw-rw-r--   0 fred      (1000) fred      (1000)     4661 2024-03-06 15:04:02.000000 protkit-0.2.1/protkit/properties/circular_variance.py
--rw-rw-r--   0 fred      (1000) fred      (1000)     8207 2024-02-15 09:39:07.000000 protkit-0.2.1/protkit/properties/dihedral_angles.py
--rw-rw-r--   0 fred      (1000) fred      (1000)    18567 2024-03-06 09:40:04.000000 protkit-0.2.1/protkit/properties/donors_acceptors.py
--rw-rw-r--   0 fred      (1000) fred      (1000)    11621 2024-03-06 08:07:46.000000 protkit-0.2.1/protkit/properties/hydrophobicity.py
--rw-rw-r--   0 fred      (1000) fred      (1000)     6987 2024-02-15 13:14:20.000000 protkit-0.2.1/protkit/properties/interface.py
--rw-rw-r--   0 fred      (1000) fred      (1000)    12504 2024-03-06 08:11:59.000000 protkit-0.2.1/protkit/properties/mass.py
--rw-rw-r--   0 fred      (1000) fred      (1000)     5162 2024-03-06 08:38:24.000000 protkit-0.2.1/protkit/properties/polarity.py
--rw-rw-r--   0 fred      (1000) fred      (1000)     4202 2024-02-28 11:35:22.000000 protkit-0.2.1/protkit/properties/surface_area.py
--rw-rw-r--   0 fred      (1000) fred      (1000)     3595 2024-02-23 13:15:30.000000 protkit-0.2.1/protkit/properties/vdw_radius.py
--rw-rw-r--   0 fred      (1000) fred      (1000)     9901 2024-03-06 11:18:19.000000 protkit-0.2.1/protkit/properties/volume.py
-drwxrwxr-x   0 fred      (1000) fred      (1000)        0 2024-03-08 07:10:54.295503 protkit-0.2.1/protkit/seq/
--rw-rw-r--   0 fred      (1000) fred      (1000)      682 2024-02-20 13:57:49.000000 protkit-0.2.1/protkit/seq/__init__.py
--rw-rw-r--   0 fred      (1000) fred      (1000)      952 2024-02-20 11:40:22.000000 protkit-0.2.1/protkit/seq/antibody_sequence.py
--rw-rw-r--   0 fred      (1000) fred      (1000)     1220 2024-02-20 11:40:22.000000 protkit-0.2.1/protkit/seq/nucleotide_sequence.py
--rw-rw-r--   0 fred      (1000) fred      (1000)     3624 2024-02-20 11:40:22.000000 protkit-0.2.1/protkit/seq/protein_sequence.py
--rw-rw-r--   0 fred      (1000) fred      (1000)     5007 2024-01-30 10:27:58.000000 protkit-0.2.1/protkit/seq/sequence.py
--rw-rw-r--   0 fred      (1000) fred      (1000)     5473 2024-02-20 11:40:22.000000 protkit-0.2.1/protkit/seq/sequence_alignment.py
-drwxrwxr-x   0 fred      (1000) fred      (1000)        0 2024-03-08 07:10:54.295503 protkit-0.2.1/protkit/structure/
--rw-rw-r--   0 fred      (1000) fred      (1000)      516 2024-01-22 13:13:22.000000 protkit-0.2.1/protkit/structure/__init__.py
--rw-rw-r--   0 fred      (1000) fred      (1000)    11726 2024-02-20 11:51:26.000000 protkit-0.2.1/protkit/structure/atom.py
--rw-rw-r--   0 fred      (1000) fred      (1000)    19490 2024-03-06 15:18:38.000000 protkit-0.2.1/protkit/structure/chain.py
--rw-rw-r--   0 fred      (1000) fred      (1000)    24100 2024-03-06 12:09:29.000000 protkit-0.2.1/protkit/structure/protein.py
--rw-rw-r--   0 fred      (1000) fred      (1000)    20645 2024-03-06 15:24:06.000000 protkit-0.2.1/protkit/structure/residue.py
-drwxrwxr-x   0 fred      (1000) fred      (1000)        0 2024-03-08 07:10:54.295503 protkit-0.2.1/protkit/tasks/
--rw-rw-r--   0 fred      (1000) fred      (1000)      139 2024-02-23 13:58:02.000000 protkit-0.2.1/protkit/tasks/__init__.py
--rw-rw-r--   0 fred      (1000) fred      (1000)     1619 2024-02-23 13:58:40.000000 protkit-0.2.1/protkit/tasks/surface_area_calculator.py
-drwxrwxr-x   0 fred      (1000) fred      (1000)        0 2024-03-08 07:10:54.295503 protkit-0.2.1/protkit/tools/
--rw-rw-r--   0 fred      (1000) fred      (1000)      218 2024-03-08 06:50:53.000000 protkit-0.2.1/protkit/tools/__init__.py
--rw-rw-r--   0 fred      (1000) fred      (1000)     3946 2024-03-08 06:54:34.000000 protkit-0.2.1/protkit/tools/freesasa_adaptor.py
-drwxrwxr-x   0 fred      (1000) fred      (1000)        0 2024-03-08 07:10:54.295503 protkit-0.2.1/protkit.egg-info/
--rw-r--r--   0 fred      (1000) fred      (1000)    18905 2024-03-08 07:10:54.000000 protkit-0.2.1/protkit.egg-info/PKG-INFO
--rw-rw-r--   0 fred      (1000) fred      (1000)     1873 2024-03-08 07:10:54.000000 protkit-0.2.1/protkit.egg-info/SOURCES.txt
--rw-rw-r--   0 fred      (1000) fred      (1000)        1 2024-03-08 07:10:54.000000 protkit-0.2.1/protkit.egg-info/dependency_links.txt
--rw-rw-r--   0 fred      (1000) fred      (1000)      160 2024-03-08 07:10:54.000000 protkit-0.2.1/protkit.egg-info/requires.txt
--rw-rw-r--   0 fred      (1000) fred      (1000)       40 2024-03-08 07:10:54.000000 protkit-0.2.1/protkit.egg-info/top_level.txt
--rw-rw-r--   0 fred      (1000) fred      (1000)     1334 2024-03-08 07:10:49.000000 protkit-0.2.1/pyproject.toml
--rw-rw-r--   0 fred      (1000) fred      (1000)       38 2024-03-08 07:10:54.295503 protkit-0.2.1/setup.cfg
-drwxrwxr-x   0 fred      (1000) fred      (1000)        0 2024-03-08 07:10:54.295503 protkit-0.2.1/tests/
--rw-rw-r--   0 fred      (1000) fred      (1000)    13883 2024-03-08 06:56:19.000000 protkit-0.2.1/tests/quick_start_guide.py
-drwxrwxr-x   0 fred      (1000) fred      (1000)        0 2024-03-08 07:10:54.291503 protkit-0.2.1/venv/
-drwxrwxr-x   0 fred      (1000) fred      (1000)        0 2024-03-08 07:10:54.295503 protkit-0.2.1/venv/bin/
--rw-rw-r--   0 fred      (1000) fred      (1000)     1336 2024-02-20 10:55:31.000000 protkit-0.2.1/venv/bin/activate_this.py
+drwxrwxr-x   0 fred      (1000) fred      (1000)        0 2024-04-03 08:16:43.289593 protkit-0.2.2/
+-rw-rw-r--   0 fred      (1000) fred      (1000)    35149 2024-02-20 10:58:14.000000 protkit-0.2.2/LICENSE
+-rw-r--r--   0 fred      (1000) fred      (1000)    18905 2024-04-03 08:16:43.289593 protkit-0.2.2/PKG-INFO
+-rw-rw-r--   0 fred      (1000) fred      (1000)    17718 2024-03-06 07:08:30.000000 protkit-0.2.2/README.md
+drwxrwxr-x   0 fred      (1000) fred      (1000)        0 2024-04-03 08:16:43.285593 protkit-0.2.2/protkit/
+-rw-rw-r--   0 fred      (1000) fred      (1000)     5279 2024-03-08 06:45:24.000000 protkit-0.2.2/protkit/__init__.py
+drwxrwxr-x   0 fred      (1000) fred      (1000)        0 2024-04-03 08:16:43.285593 protkit-0.2.2/protkit/core/
+-rw-rw-r--   0 fred      (1000) fred      (1000)      135 2024-02-20 13:59:59.000000 protkit-0.2.2/protkit/core/__init__.py
+-rw-rw-r--   0 fred      (1000) fred      (1000)     2609 2024-01-30 10:27:10.000000 protkit-0.2.2/protkit/core/extend_attributes.py
+drwxrwxr-x   0 fred      (1000) fred      (1000)        0 2024-04-03 08:16:43.285593 protkit-0.2.2/protkit/download/
+-rw-rw-r--   0 fred      (1000) fred      (1000)      395 2024-02-20 11:32:28.000000 protkit-0.2.2/protkit/download/__init__.py
+-rw-rw-r--   0 fred      (1000) fred      (1000)    12986 2024-03-11 08:37:40.000000 protkit-0.2.2/protkit/download/download.py
+drwxrwxr-x   0 fred      (1000) fred      (1000)        0 2024-04-03 08:16:43.285593 protkit-0.2.2/protkit/file_io/
+-rw-rw-r--   0 fred      (1000) fred      (1000)      786 2024-02-20 11:40:22.000000 protkit-0.2.2/protkit/file_io/__init__.py
+-rw-rw-r--   0 fred      (1000) fred      (1000)     3870 2024-03-11 10:09:24.000000 protkit-0.2.2/protkit/file_io/fasta_io.py
+-rw-rw-r--   0 fred      (1000) fred      (1000)     3532 2024-02-20 11:40:22.000000 protkit-0.2.2/protkit/file_io/mmcif_io.py
+-rw-rw-r--   0 fred      (1000) fred      (1000)     3405 2024-02-20 11:40:22.000000 protkit-0.2.2/protkit/file_io/mmtf_io.py
+-rw-rw-r--   0 fred      (1000) fred      (1000)    44013 2024-04-02 14:47:49.000000 protkit-0.2.2/protkit/file_io/pdb_io.py
+-rw-rw-r--   0 fred      (1000) fred      (1000)     1134 2024-02-20 11:40:22.000000 protkit-0.2.2/protkit/file_io/pqr_io.py
+-rw-rw-r--   0 fred      (1000) fred      (1000)     9969 2024-02-20 11:40:22.000000 protkit-0.2.2/protkit/file_io/prot_io.py
+drwxrwxr-x   0 fred      (1000) fred      (1000)        0 2024-04-03 08:16:43.285593 protkit-0.2.2/protkit/geometry/
+-rw-rw-r--   0 fred      (1000) fred      (1000)      147 2024-02-23 12:55:57.000000 protkit-0.2.2/protkit/geometry/__init__.py
+-rw-rw-r--   0 fred      (1000) fred      (1000)     7717 2024-02-15 08:53:21.000000 protkit-0.2.2/protkit/geometry/math.py
+-rw-rw-r--   0 fred      (1000) fred      (1000)     5103 2024-02-15 12:04:44.000000 protkit-0.2.2/protkit/geometry/space_query.py
+drwxrwxr-x   0 fred      (1000) fred      (1000)        0 2024-04-03 08:16:43.289593 protkit-0.2.2/protkit/metrics/
+-rw-rw-r--   0 fred      (1000) fred      (1000)     1160 2024-02-23 12:57:26.000000 protkit-0.2.2/protkit/metrics/__init__.py
+-rw-rw-r--   0 fred      (1000) fred      (1000)      272 2024-01-24 11:20:02.000000 protkit-0.2.2/protkit/metrics/classification_eval.py
+-rw-rw-r--   0 fred      (1000) fred      (1000)      259 2024-01-24 11:20:02.000000 protkit-0.2.2/protkit/metrics/regression_eval.py
+-rw-rw-r--   0 fred      (1000) fred      (1000)     5566 2024-02-23 12:57:27.000000 protkit-0.2.2/protkit/metrics/scoring_matrix.py
+-rw-rw-r--   0 fred      (1000) fred      (1000)     6063 2024-02-02 14:13:32.000000 protkit-0.2.2/protkit/metrics/sequence_eval.py
+-rw-rw-r--   0 fred      (1000) fred      (1000)     3172 2024-01-31 09:20:40.000000 protkit-0.2.2/protkit/metrics/structure_eval.py
+-rw-rw-r--   0 fred      (1000) fred      (1000)      339 2024-01-24 11:18:08.000000 protkit-0.2.2/protkit/metrics/utility_eval.py
+drwxrwxr-x   0 fred      (1000) fred      (1000)        0 2024-04-03 08:16:43.289593 protkit-0.2.2/protkit/properties/
+-rw-rw-r--   0 fred      (1000) fred      (1000)     1076 2024-04-03 08:07:25.000000 protkit-0.2.2/protkit/properties/__init__.py
+-rw-rw-r--   0 fred      (1000) fred      (1000)     9887 2024-02-14 09:21:12.000000 protkit-0.2.2/protkit/properties/bond_angles.py
+-rw-rw-r--   0 fred      (1000) fred      (1000)    10870 2024-02-14 09:21:12.000000 protkit-0.2.2/protkit/properties/bond_lengths.py
+-rw-rw-r--   0 fred      (1000) fred      (1000)    10763 2024-03-07 14:33:32.000000 protkit-0.2.2/protkit/properties/bounds.py
+-rw-rw-r--   0 fred      (1000) fred      (1000)     4785 2024-02-06 10:51:06.000000 protkit-0.2.2/protkit/properties/charge.py
+-rw-rw-r--   0 fred      (1000) fred      (1000)     4652 2024-03-06 08:28:16.000000 protkit-0.2.2/protkit/properties/chemical_class.py
+-rw-rw-r--   0 fred      (1000) fred      (1000)     4661 2024-03-06 15:04:02.000000 protkit-0.2.2/protkit/properties/circular_variance.py
+-rw-rw-r--   0 fred      (1000) fred      (1000)     8207 2024-02-15 09:39:07.000000 protkit-0.2.2/protkit/properties/dihedral_angles.py
+-rw-rw-r--   0 fred      (1000) fred      (1000)    18567 2024-03-06 09:40:04.000000 protkit-0.2.2/protkit/properties/donors_acceptors.py
+-rw-rw-r--   0 fred      (1000) fred      (1000)    11621 2024-03-06 08:07:46.000000 protkit-0.2.2/protkit/properties/hydrophobicity.py
+-rw-rw-r--   0 fred      (1000) fred      (1000)     6987 2024-02-15 13:14:20.000000 protkit-0.2.2/protkit/properties/interface.py
+-rw-rw-r--   0 fred      (1000) fred      (1000)    12504 2024-03-06 08:11:59.000000 protkit-0.2.2/protkit/properties/mass.py
+-rw-rw-r--   0 fred      (1000) fred      (1000)     5162 2024-03-06 08:38:24.000000 protkit-0.2.2/protkit/properties/polarity.py
+-rw-rw-r--   0 fred      (1000) fred      (1000)     4202 2024-02-28 11:35:22.000000 protkit-0.2.2/protkit/properties/surface_area.py
+-rw-rw-r--   0 fred      (1000) fred      (1000)     3595 2024-02-23 13:15:30.000000 protkit-0.2.2/protkit/properties/vdw_radius.py
+-rw-rw-r--   0 fred      (1000) fred      (1000)     9901 2024-03-06 11:18:19.000000 protkit-0.2.2/protkit/properties/volume.py
+drwxrwxr-x   0 fred      (1000) fred      (1000)        0 2024-04-03 08:16:43.289593 protkit-0.2.2/protkit/seq/
+-rw-rw-r--   0 fred      (1000) fred      (1000)      682 2024-02-20 13:57:49.000000 protkit-0.2.2/protkit/seq/__init__.py
+-rw-rw-r--   0 fred      (1000) fred      (1000)      952 2024-02-20 11:40:22.000000 protkit-0.2.2/protkit/seq/antibody_sequence.py
+-rw-rw-r--   0 fred      (1000) fred      (1000)     1220 2024-02-20 11:40:22.000000 protkit-0.2.2/protkit/seq/nucleotide_sequence.py
+-rw-rw-r--   0 fred      (1000) fred      (1000)     3624 2024-02-20 11:40:22.000000 protkit-0.2.2/protkit/seq/protein_sequence.py
+-rw-rw-r--   0 fred      (1000) fred      (1000)     5710 2024-03-11 10:00:59.000000 protkit-0.2.2/protkit/seq/sequence.py
+-rw-rw-r--   0 fred      (1000) fred      (1000)     5473 2024-02-20 11:40:22.000000 protkit-0.2.2/protkit/seq/sequence_alignment.py
+drwxrwxr-x   0 fred      (1000) fred      (1000)        0 2024-04-03 08:16:43.289593 protkit-0.2.2/protkit/structure/
+-rw-rw-r--   0 fred      (1000) fred      (1000)      516 2024-01-22 13:13:22.000000 protkit-0.2.2/protkit/structure/__init__.py
+-rw-rw-r--   0 fred      (1000) fred      (1000)    11726 2024-02-20 11:51:26.000000 protkit-0.2.2/protkit/structure/atom.py
+-rw-rw-r--   0 fred      (1000) fred      (1000)    19490 2024-03-06 15:18:38.000000 protkit-0.2.2/protkit/structure/chain.py
+-rw-rw-r--   0 fred      (1000) fred      (1000)    24100 2024-03-06 12:09:29.000000 protkit-0.2.2/protkit/structure/protein.py
+-rw-rw-r--   0 fred      (1000) fred      (1000)    20645 2024-03-06 15:24:06.000000 protkit-0.2.2/protkit/structure/residue.py
+drwxrwxr-x   0 fred      (1000) fred      (1000)        0 2024-04-03 08:16:43.289593 protkit-0.2.2/protkit/tasks/
+-rw-rw-r--   0 fred      (1000) fred      (1000)      139 2024-04-03 08:07:09.000000 protkit-0.2.2/protkit/tasks/__init__.py
+-rw-rw-r--   0 fred      (1000) fred      (1000)     1369 2024-03-08 13:46:26.000000 protkit-0.2.2/protkit/tasks/protonator.py
+-rw-rw-r--   0 fred      (1000) fred      (1000)     1619 2024-02-23 13:58:40.000000 protkit-0.2.2/protkit/tasks/surface_area_calculator.py
+drwxrwxr-x   0 fred      (1000) fred      (1000)        0 2024-04-03 08:16:43.289593 protkit-0.2.2/protkit/tools/
+-rw-rw-r--   0 fred      (1000) fred      (1000)      218 2024-03-08 06:50:53.000000 protkit-0.2.2/protkit/tools/__init__.py
+-rw-rw-r--   0 fred      (1000) fred      (1000)     3946 2024-03-08 06:54:34.000000 protkit-0.2.2/protkit/tools/freesasa_adaptor.py
+-rw-rw-r--   0 fred      (1000) fred      (1000)     8569 2024-04-03 07:58:04.000000 protkit-0.2.2/protkit/tools/reduce_adaptor.py
+drwxrwxr-x   0 fred      (1000) fred      (1000)        0 2024-04-03 08:16:43.289593 protkit-0.2.2/protkit.egg-info/
+-rw-r--r--   0 fred      (1000) fred      (1000)    18905 2024-04-03 08:16:43.000000 protkit-0.2.2/protkit.egg-info/PKG-INFO
+-rw-rw-r--   0 fred      (1000) fred      (1000)     1954 2024-04-03 08:16:43.000000 protkit-0.2.2/protkit.egg-info/SOURCES.txt
+-rw-rw-r--   0 fred      (1000) fred      (1000)        1 2024-04-03 08:16:43.000000 protkit-0.2.2/protkit.egg-info/dependency_links.txt
+-rw-rw-r--   0 fred      (1000) fred      (1000)      160 2024-04-03 08:16:43.000000 protkit-0.2.2/protkit.egg-info/requires.txt
+-rw-rw-r--   0 fred      (1000) fred      (1000)       40 2024-04-03 08:16:43.000000 protkit-0.2.2/protkit.egg-info/top_level.txt
+-rw-rw-r--   0 fred      (1000) fred      (1000)     1334 2024-04-03 08:16:03.000000 protkit-0.2.2/pyproject.toml
+-rw-rw-r--   0 fred      (1000) fred      (1000)       38 2024-04-03 08:16:43.289593 protkit-0.2.2/setup.cfg
+drwxrwxr-x   0 fred      (1000) fred      (1000)        0 2024-04-03 08:16:43.289593 protkit-0.2.2/tests/
+-rw-rw-r--   0 fred      (1000) fred      (1000)    22661 2024-03-11 14:12:17.000000 protkit-0.2.2/tests/quick_start_guide.py
+-rw-rw-r--   0 fred      (1000) fred      (1000)      564 2024-03-26 13:48:46.000000 protkit-0.2.2/tests/test_reduce.py
+drwxrwxr-x   0 fred      (1000) fred      (1000)        0 2024-04-03 08:16:43.281593 protkit-0.2.2/venv/
+drwxrwxr-x   0 fred      (1000) fred      (1000)        0 2024-04-03 08:16:43.289593 protkit-0.2.2/venv/bin/
+-rw-rw-r--   0 fred      (1000) fred      (1000)     1336 2024-02-20 10:55:31.000000 protkit-0.2.2/venv/bin/activate_this.py
```

### Comparing `protkit-0.2.1/LICENSE` & `protkit-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `protkit-0.2.1/PKG-INFO` & `protkit-0.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: protkit
-Version: 0.2.1
+Version: 0.2.2
 Summary: A unified toolkit for structural protein engineering.
 Author-email: Fred Senekal <fred@silicogenesis.com>
 Maintainer-email: Fred Senekal <fred@silicogenesis.com>
 Project-URL: Homepage, https://protkit.silicogenesis.com
 Project-URL: Repository, https://github.com/silicogenesis/protkit
 Project-URL: Documentation, https://silicogenesis.github.io/protkit
 Keywords: protein,protein engineering,structural biology,computational biology,biology,bioinformatics,sequence,amino acid,residue,dataset,PDB,antibody,antibody engineering,cdr
```

### Comparing `protkit-0.2.1/README.md` & `protkit-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `protkit-0.2.1/protkit/__init__.py` & `protkit-0.2.2/protkit/__init__.py`

 * *Files identical despite different names*

### Comparing `protkit-0.2.1/protkit/core/extend_attributes.py` & `protkit-0.2.2/protkit/core/extend_attributes.py`

 * *Files identical despite different names*

### Comparing `protkit-0.2.1/protkit/download/download.py` & `protkit-0.2.2/protkit/download/download.py`

 * *Files 0% similar despite different names*

```diff
@@ -55,16 +55,16 @@
         Raises:
             Exception: If the file could not be downloaded or saved.
         """
         try:
             response = requests.get(url)
             if response.status_code == 200:
                 # Create the directory if it does not exist.
-                if os.path.isdir(file_path):
-                    directory = os.path.dirname(file_path)
+                directory = os.path.dirname(file_path)
+                if directory != "":
                     if not os.path.exists(directory):
                         os.makedirs(directory)
 
                 # Write the file to disk.
                 with open(file_path, "wb") as file:
                     file.write(response.content)
         except Exception as e:
```

### Comparing `protkit-0.2.1/protkit/file_io/__init__.py` & `protkit-0.2.2/protkit/file_io/__init__.py`

 * *Files identical despite different names*

### Comparing `protkit-0.2.1/protkit/file_io/fasta_io.py` & `protkit-0.2.2/protkit/file_io/fasta_io.py`

 * *Files 5% similar despite different names*

```diff
@@ -12,16 +12,16 @@
 
 See https://en.wikipedia.org/wiki/FASTA_format for more information.
 See https://www.rcsb.org/ for examples of FASTA files.
 
 Methods are static and can be called without instantiating the class.
 The main functions exposed by the class are:
 
-- `load()` to load a protein from a PDB file.
-- `save()` to save a protein to a PDB file.
+- `load()` to load a protein from a Fasta file.
+- `save()` to save a protein to a Fasta file.
 """
 
 from typing import List
 from protkit.seq.sequence import Sequence
 
 
 class FastaIO:
@@ -74,21 +74,21 @@
             # The last sequence is added assuming there is no empty line at the end.
             if description is not None or seq != "":
                 sequences.append(Sequence(seq, description))
 
         return sequences
 
     @staticmethod
-    def save(file_path: str, sequence: [Sequence, List[Sequence]], line_length: [int, None] = 80) -> None:
+    def save(sequence: [Sequence, List[Sequence]], file_path: str, line_length: [int, None] = 80) -> None:
         """
         Saves a FASTA file.
 
         Args:
-            file_path (str): The path to the FASTA file.
             sequence (Union[Sequence, List[Sequence]]): The sequence(s) to save.
+            file_path (str): The path to the FASTA file.
             line_length (int): The length of the lines in the FASTA file.
                 If None, the sequence will be saved on one line.
 
         Returns:
             None
         """
         if type(sequence) is Sequence:
@@ -101,9 +101,9 @@
                 else:
                     file.write(">\n")
 
                 if line_length is None:
                     file.write(seq.sequence + "\n")
                 else:
                     for i in range((len(seq.sequence) - 1) // line_length + 1):
-                        file.write(seq.sequence[i * line_length:(i + 1) * line_length] + "\n")
+                        file.write(seq.to_string(i * line_length, (i + 1) * line_length - 1) + "\n")
                 file.write("\n")
```

### Comparing `protkit-0.2.1/protkit/file_io/mmcif_io.py` & `protkit-0.2.2/protkit/file_io/mmcif_io.py`

 * *Files identical despite different names*

### Comparing `protkit-0.2.1/protkit/file_io/mmtf_io.py` & `protkit-0.2.2/protkit/file_io/mmtf_io.py`

 * *Files identical despite different names*

### Comparing `protkit-0.2.1/protkit/file_io/pdb_io.py` & `protkit-0.2.2/protkit/file_io/pdb_io.py`

 * *Files 3% similar despite different names*

```diff
@@ -369,22 +369,28 @@
         return text
 
     # --------------------------------------------------------------------------------
     # Main parsing and saving functions
     # --------------------------------------------------------------------------------
 
     @staticmethod
-    def parse_pdb_entries(file_path: str, is_pqr_format: bool = False):
+    def parse_pdb_entries_from_string(pdb_string: str, is_pqr_format: bool = False):
         """
-        Parse PDB file according to the spec provided at:
-        https://www.wwpdb.org/documentation/file-format-content/format33/sect9.html#ATOM
+        Parse a PDB file in string format into a list of entries.
+
+        Args:
+            pdb_string (str): The PDB file as a string.
+            is_pqr_format (bool): If the file is in PQR format.
+
+        Returns:
+            List[Dict]: A list of parsed entries.
         """
-        # Open the file and extract the individual lines.
-        with open(file_path) as file:
-            lines = file.read().split("\n")
+
+        # Split the string into lines
+        lines = pdb_string.split("\n")
 
         # Parse every line into dictionary information
         entries = []
         for line in lines:
             record_name = line[0:6].strip().upper()
             if record_name == "ATOM":
                 pdb_atom_dict = PDBIO.parse_pdb_atom_line(line)
@@ -402,28 +408,41 @@
                 pdb_end_model_dict = PDBIO.parse_pdb_end_model_line(line)
                 entries.append(pdb_end_model_dict)
             elif record_name == "SEQRES":
                 pdb_seqres_dict = PDBIO.parse_pdb_seqres_line(line)
                 entries.append(pdb_seqres_dict)
         return entries
 
+
     @staticmethod
-    def load(file_path: str,
-             is_pqr_format: bool = False,
-             pdb_id: Optional[str] = None) -> List[Protein]:
+    def parse_pdb_entries(file_path: str, is_pqr_format: bool = False):
+        """
+        Parse PDB file according to the spec provided at:
+        https://www.wwpdb.org/documentation/file-format-content/format33/sect9.html#ATOM
+        """
+        # Open the file and extract the individual lines.
+        with open(file_path) as file:
+            pdb_string = file.read()
+
+        return PDBIO.parse_pdb_entries_from_string(pdb_string, is_pqr_format=is_pqr_format)
 
+    @staticmethod
+    def load_from_string(pdb_string: str,
+                         is_pqr_format: bool = False,
+                         pdb_id: Optional[str] = None) -> List[Protein]:
         protein = Protein(pdb_id=pdb_id)
         models = []
         seqres = {}
         current_model = None
         current_chain: Optional[Chain] = None
         current_chain_id = None
         current_residue: Optional[Residue] = None
         current_residue_id = None
-        entries = PDBIO.parse_pdb_entries(file_path, is_pqr_format=is_pqr_format)
+
+        entries = PDBIO.parse_pdb_entries_from_string(pdb_string, is_pqr_format=is_pqr_format)
 
         for entry in entries:
             record_name = entry["record_name"]
             if record_name == "SEQRES":
                 chain_id = entry["chain_id"]
                 if chain_id not in seqres:
                     seqres[chain_id] = []
@@ -528,18 +547,40 @@
                     protein.get_chain(chain_id).set_attribute("seqres", seqres[chain_id])
 
         # Housekeeping
         # protein.set_residue_indexing()
 
         return [protein]
 
+
     @staticmethod
-    def save(protein: Protein,
-             file_path: str,
-             is_pqr_format=False) -> None:
+    def load(file_path: str,
+             is_pqr_format: bool = False,
+             pdb_id: Optional[str] = None) -> List[Protein]:
+        """
+        Load a protein from a PDB file.
+
+        Args:
+            file_path (str): The path to the PDB file.
+            is_pqr_format (bool): If the file is in PQR format.
+            pdb_id (str): The PDB ID of the protein.
+
+        Returns:
+            List[Protein]: A list of proteins.
+        """
+
+        # Open the file and extract the individual lines.
+        with open(file_path) as file:
+            pdb_string = file.read()
+
+        return PDBIO.load_from_string(pdb_string, is_pqr_format=is_pqr_format, pdb_id=pdb_id)
+
+    @staticmethod
+    def save_to_string(protein: Protein,
+                       is_pqr_format=False) -> str:
         text_entries = []
         num_seqres = 0
         num_atoms = 0
         num_hetatoms = 0
         num_ter = 0
         serial = 1
 
@@ -567,205 +608,213 @@
                         serial += 1
                         num_atoms += 1
 
         # Bookkeeping records
         text_entries.append(PDBIO.create_pdb_master_line(num_atoms, num_hetatoms, num_ter, num_seqres=num_seqres))
         text_entries.append("END".ljust(80))
 
+        return "\n".join(text_entries)
+
+    @staticmethod
+    def save(protein: Protein,
+             file_path: str,
+             is_pqr_format=False) -> None:
+
+        pdb_string = PDBIO.save_to_string(protein, is_pqr_format=is_pqr_format)
+
         with open(file_path, "w") as file:
-            file.write("\n".join(text_entries))
+            file.write(pdb_string)
 
     # TODO: from_pdb_text and to_pdb_text was added by Claudio
     # The intent is that one should parse proteins from text
     # without working with files. However, a lot of code copying
     # was made and it need to be reworked significantly.
 
-    @staticmethod
-    def from_pdb_text(lines) -> List[Protein]:
-        lines = lines.split("\n")
-
-        entries = []
-        for line in lines:
-            record_name = line[0:6].strip().upper()
-            if record_name == "ATOM":
-                pdb_atom_dict = PDBIO.parse_pdb_atom_line(line)
-                entries.append(pdb_atom_dict)
-            elif record_name == "HETATM":
-                pdb_atom_dict = PDBIO.parse_pdb_atom_line(line)
-                entries.append(pdb_atom_dict)
-            elif record_name == "TER":
-                pdb_ter_dict = PDBIO.parse_pdb_ter_line(line)
-                entries.append(pdb_ter_dict)
-            elif record_name == "MODEL":
-                pdb_model_dict = PDBIO.parse_pdb_model_line(line)
-                entries.append(pdb_model_dict)
-            elif record_name == "ENDMDL":
-                pdb_end_model_dict = PDBIO.parse_pdb_end_model_line(line)
-                entries.append(pdb_end_model_dict)
-            elif record_name == "SEQRES":
-                pdb_seqres_dict = PDBIO.parse_pdb_seqres_line(line)
-                entries.append(pdb_seqres_dict)
-
-        protein = Protein()
-        models = []
-        seqres = {}
-        current_model = None
-        current_chain: Optional[Chain] = None
-        current_chain_id = None
-        current_residue: Optional[Residue] = None
-        current_residue_id = None
-
-        for entry in entries:
-            record_name = entry["record_name"]
-            if record_name == "SEQRES":
-                chain_id = entry["chain_id"]
-                if chain_id not in seqres:
-                    seqres[chain_id] = []
-                seqres[chain_id].extend(entry["residues"])
-            elif record_name == "MODEL":
-                # Usually, the MODEL field will only be found in structures based on NMR.
-                # We only use the first model in a file if provided.
-                # There is nothing to do, so we
-                pass
-            elif record_name == "ENDMDL":
-                # Usually, the ENDMDL field will only be found in structures based on NMR.
-                # it closes a corresponding MODEL field.
-                # Since the end of the model is reached, no more entries should be parsed.
-                break
-            elif record_name == "TER":
-                # The TER field terminates the current chain.
-                current_chain = None
-                current_chain_id = None
-            elif record_name == "ATOM" or record_name == "HETATM":
-                # If we switched chains, set the chain.
-                if entry["chain_id"] != current_chain_id:
-                    current_chain_id = entry["chain_id"]
-                    if protein.has_chain(current_chain_id):
-                        current_chain = protein.get_chain(current_chain_id)
-                    else:
-                        current_chain = protein.create_chain(current_chain_id)
-
-                # Check if the residue exists
-                residue_id = current_chain_id + entry["res_seq"] + entry["icode"]
-                if residue_id != current_residue_id:
-                    current_residue_id = residue_id
-                    if record_name == "ATOM":
-                        # if entry["res_name"] in ResidueTemplate.VALID_DNA_RESIDUES:
-                        #     current_residue = current_chain.add_dna_residue(
-                        #         residue_type=entry["res_name"],
-                        #         sequence_no=int(entry["res_seq"]),
-                        #         insertion_code=entry["icode"]
-                        #     )
-                        # else:
-                        current_residue = Residue(
-                            residue_type=entry["res_name"],
-                            sequence_no=int(entry["res_seq"]),
-                            insertion_code=entry["icode"],
-                            chain=current_chain)
-                        current_chain.add_residue(current_residue)
-                    elif record_name == "HETATM":
-                        current_residue = Residue(
-                            residue_type=entry["res_name"],
-                            sequence_no=int(entry["res_seq"]),
-                            insertion_code=entry["icode"],
-                            chain=current_chain)
-                        current_chain.add_residue(current_residue)
-
-                        # current_residue = current_chain.add_het_residue(
-                        #     residue_type=entry["res_name"],
-                        #     sequence_no=int(entry["res_seq"]),
-                        #     insertion_code=entry["icode"]
-                        # )
-
-                # Temporary fix need to see if anything breaks (For Evo eg. 2HH1 -> HH12)
-                # Fix atom naming
-                if entry["atom_name"][0].isnumeric():
-                    entry["atom_name"] = entry["atom_name"][1:] + entry["atom_name"][0]
-                    if entry["element"] != "H":
-                        print(0)
-                    if entry["atom_name"][0] == "H":
-                        entry["element"] = "H"
-
-                # Add the atom to the residue
-                if entry["alt_loc"] == "":
-                    atom_id = entry["atom_name"]
-                else:
-                    atom_id = entry["atom_name"] + "_" + entry["alt_loc"]
-                atom = Atom(
-                    element=entry["element"],
-                    atom_type=entry["atom_name"],
-                    x=entry["x"],
-                    y=entry["y"],
-                    z=entry["z"],
-
-                    # pdb_serial=entry["serial"],
-                    # pdb_alt_loc=entry["alt_loc"],
-                    # pdb_occupancy=entry["occupancy"],
-                    # pdb_temp_factor=entry["temp_factor"],
-                    # pdb_assigned_charge=entry["assigned_charge"],
-                    # pqr_calculated_charge=entry["calculated_charge"],
-                    # pqr_radius=entry["radius"],
-                    #
-                    is_hetero=(record_name == "HETATM"),
-
-                    residue=current_residue
-                )
-                current_residue.add_atom(atom_id, atom)
-
-        # if seqres:
-        #     for chain_id in seqres:
-        #         if seqres[chain_id]:
-        #             protein.chains[chain_id].sequence = seqres[chain_id]
-
-        # Housekeeping
-        # protein.set_residue_indexing()
-
-        return [protein]
-
-    @staticmethod
-    def to_pdb_text(protein: Protein):
-        text_entries = ""
-        num_seqres = 0
-        num_atoms = 0
-        num_hetatoms = 0
-        num_ter = 0
-        serial = 1
-
-        for chain in protein.chains:
-            for residue in chain.residues:
-                for atom in residue.atoms:
-                    if not atom.is_hetero:
-                        atom_entry = {
-                            "element": atom.element,
-                            "atom_name": atom.atom_type,
-                            "alt_loc": atom.get_attribute("pdb_alt_loc"),
-                            "res_name": residue.residue_type,
-                            "chain_id": chain.chain_id,
-                            "res_seq": str(residue.sequence_no),
-                            "icode": residue.insertion_code,
-                            "x": atom.x,
-                            "y": atom.y,
-                            "z": atom.z,
-                            "occupancy": atom.get_attribute("occupancy"),
-                            # "temp_factor": atom._pdb_temp_factor if atom._pdb_temp_factor is not None else 0.0,
-                            "temp_factor": atom.get_attribute("temp_factor"),
-                            "charge": atom.get_attribute("assigned_charge")
-                        }
-                        text_entries += PDBIO.create_pdb_atom_line(atom_entry, serial)
-                        text_entries += "\n"
-                        serial += 1
-                        num_atoms += 1
-
-        # Bookkeeping records
-        text_entries += PDBIO.create_pdb_master_line(num_atoms, num_hetatoms, num_ter, num_seqres=num_seqres)
-        text_entries += "END".ljust(80)
-        text_entries += "\n"
-
-        return text_entries
+    # @staticmethod
+    # def from_pdb_text(lines) -> List[Protein]:
+    #     lines = lines.split("\n")
+    #
+    #     entries = []
+    #     for line in lines:
+    #         record_name = line[0:6].strip().upper()
+    #         if record_name == "ATOM":
+    #             pdb_atom_dict = PDBIO.parse_pdb_atom_line(line)
+    #             entries.append(pdb_atom_dict)
+    #         elif record_name == "HETATM":
+    #             pdb_atom_dict = PDBIO.parse_pdb_atom_line(line)
+    #             entries.append(pdb_atom_dict)
+    #         elif record_name == "TER":
+    #             pdb_ter_dict = PDBIO.parse_pdb_ter_line(line)
+    #             entries.append(pdb_ter_dict)
+    #         elif record_name == "MODEL":
+    #             pdb_model_dict = PDBIO.parse_pdb_model_line(line)
+    #             entries.append(pdb_model_dict)
+    #         elif record_name == "ENDMDL":
+    #             pdb_end_model_dict = PDBIO.parse_pdb_end_model_line(line)
+    #             entries.append(pdb_end_model_dict)
+    #         elif record_name == "SEQRES":
+    #             pdb_seqres_dict = PDBIO.parse_pdb_seqres_line(line)
+    #             entries.append(pdb_seqres_dict)
+    #
+    #     protein = Protein()
+    #     models = []
+    #     seqres = {}
+    #     current_model = None
+    #     current_chain: Optional[Chain] = None
+    #     current_chain_id = None
+    #     current_residue: Optional[Residue] = None
+    #     current_residue_id = None
+    #
+    #     for entry in entries:
+    #         record_name = entry["record_name"]
+    #         if record_name == "SEQRES":
+    #             chain_id = entry["chain_id"]
+    #             if chain_id not in seqres:
+    #                 seqres[chain_id] = []
+    #             seqres[chain_id].extend(entry["residues"])
+    #         elif record_name == "MODEL":
+    #             # Usually, the MODEL field will only be found in structures based on NMR.
+    #             # We only use the first model in a file if provided.
+    #             # There is nothing to do, so we
+    #             pass
+    #         elif record_name == "ENDMDL":
+    #             # Usually, the ENDMDL field will only be found in structures based on NMR.
+    #             # it closes a corresponding MODEL field.
+    #             # Since the end of the model is reached, no more entries should be parsed.
+    #             break
+    #         elif record_name == "TER":
+    #             # The TER field terminates the current chain.
+    #             current_chain = None
+    #             current_chain_id = None
+    #         elif record_name == "ATOM" or record_name == "HETATM":
+    #             # If we switched chains, set the chain.
+    #             if entry["chain_id"] != current_chain_id:
+    #                 current_chain_id = entry["chain_id"]
+    #                 if protein.has_chain(current_chain_id):
+    #                     current_chain = protein.get_chain(current_chain_id)
+    #                 else:
+    #                     current_chain = protein.create_chain(current_chain_id)
+    #
+    #             # Check if the residue exists
+    #             residue_id = current_chain_id + entry["res_seq"] + entry["icode"]
+    #             if residue_id != current_residue_id:
+    #                 current_residue_id = residue_id
+    #                 if record_name == "ATOM":
+    #                     # if entry["res_name"] in ResidueTemplate.VALID_DNA_RESIDUES:
+    #                     #     current_residue = current_chain.add_dna_residue(
+    #                     #         residue_type=entry["res_name"],
+    #                     #         sequence_no=int(entry["res_seq"]),
+    #                     #         insertion_code=entry["icode"]
+    #                     #     )
+    #                     # else:
+    #                     current_residue = Residue(
+    #                         residue_type=entry["res_name"],
+    #                         sequence_no=int(entry["res_seq"]),
+    #                         insertion_code=entry["icode"],
+    #                         chain=current_chain)
+    #                     current_chain.add_residue(current_residue)
+    #                 elif record_name == "HETATM":
+    #                     current_residue = Residue(
+    #                         residue_type=entry["res_name"],
+    #                         sequence_no=int(entry["res_seq"]),
+    #                         insertion_code=entry["icode"],
+    #                         chain=current_chain)
+    #                     current_chain.add_residue(current_residue)
+    #
+    #                     # current_residue = current_chain.add_het_residue(
+    #                     #     residue_type=entry["res_name"],
+    #                     #     sequence_no=int(entry["res_seq"]),
+    #                     #     insertion_code=entry["icode"]
+    #                     # )
+    #
+    #             # Temporary fix need to see if anything breaks (For Evo eg. 2HH1 -> HH12)
+    #             # Fix atom naming
+    #             if entry["atom_name"][0].isnumeric():
+    #                 entry["atom_name"] = entry["atom_name"][1:] + entry["atom_name"][0]
+    #                 if entry["element"] != "H":
+    #                     print(0)
+    #                 if entry["atom_name"][0] == "H":
+    #                     entry["element"] = "H"
+    #
+    #             # Add the atom to the residue
+    #             if entry["alt_loc"] == "":
+    #                 atom_id = entry["atom_name"]
+    #             else:
+    #                 atom_id = entry["atom_name"] + "_" + entry["alt_loc"]
+    #             atom = Atom(
+    #                 element=entry["element"],
+    #                 atom_type=entry["atom_name"],
+    #                 x=entry["x"],
+    #                 y=entry["y"],
+    #                 z=entry["z"],
+    #
+    #                 # pdb_serial=entry["serial"],
+    #                 # pdb_alt_loc=entry["alt_loc"],
+    #                 # pdb_occupancy=entry["occupancy"],
+    #                 # pdb_temp_factor=entry["temp_factor"],
+    #                 # pdb_assigned_charge=entry["assigned_charge"],
+    #                 # pqr_calculated_charge=entry["calculated_charge"],
+    #                 # pqr_radius=entry["radius"],
+    #                 #
+    #                 is_hetero=(record_name == "HETATM"),
+    #
+    #                 residue=current_residue
+    #             )
+    #             current_residue.add_atom(atom_id, atom)
+    #
+    #     # if seqres:
+    #     #     for chain_id in seqres:
+    #     #         if seqres[chain_id]:
+    #     #             protein.chains[chain_id].sequence = seqres[chain_id]
+    #
+    #     # Housekeeping
+    #     # protein.set_residue_indexing()
+    #
+    #     return [protein]
 
+    # @staticmethod
+    # def to_pdb_text(protein: Protein):
+    #     text_entries = ""
+    #     num_seqres = 0
+    #     num_atoms = 0
+    #     num_hetatoms = 0
+    #     num_ter = 0
+    #     serial = 1
+    #
+    #     for chain in protein.chains:
+    #         for residue in chain.residues:
+    #             for atom in residue.atoms:
+    #                 if not atom.is_hetero:
+    #                     atom_entry = {
+    #                         "element": atom.element,
+    #                         "atom_name": atom.atom_type,
+    #                         "alt_loc": atom.get_attribute("pdb_alt_loc"),
+    #                         "res_name": residue.residue_type,
+    #                         "chain_id": chain.chain_id,
+    #                         "res_seq": str(residue.sequence_no),
+    #                         "icode": residue.insertion_code,
+    #                         "x": atom.x,
+    #                         "y": atom.y,
+    #                         "z": atom.z,
+    #                         "occupancy": atom.get_attribute("occupancy"),
+    #                         # "temp_factor": atom._pdb_temp_factor if atom._pdb_temp_factor is not None else 0.0,
+    #                         "temp_factor": atom.get_attribute("temp_factor"),
+    #                         "charge": atom.get_attribute("assigned_charge")
+    #                     }
+    #                     text_entries += PDBIO.create_pdb_atom_line(atom_entry, serial)
+    #                     text_entries += "\n"
+    #                     serial += 1
+    #                     num_atoms += 1
+    #
+    #     # Bookkeeping records
+    #     text_entries += PDBIO.create_pdb_master_line(num_atoms, num_hetatoms, num_ter, num_seqres=num_seqres)
+    #     text_entries += "END".ljust(80)
+    #     text_entries += "\n"
+    #
+    #     return text_entries
 
     # @staticmethod
     # def save_to_pdb(file_path: str, protein):
     #     entries = []
     #
     #     num_seqres = 0
     #     num_atoms = 0
```

### Comparing `protkit-0.2.1/protkit/file_io/pqr_io.py` & `protkit-0.2.2/protkit/file_io/pqr_io.py`

 * *Files identical despite different names*

### Comparing `protkit-0.2.1/protkit/file_io/prot_io.py` & `protkit-0.2.2/protkit/file_io/prot_io.py`

 * *Files identical despite different names*

### Comparing `protkit-0.2.1/protkit/geometry/math.py` & `protkit-0.2.2/protkit/geometry/math.py`

 * *Files identical despite different names*

### Comparing `protkit-0.2.1/protkit/geometry/space_query.py` & `protkit-0.2.2/protkit/geometry/space_query.py`

 * *Files identical despite different names*

### Comparing `protkit-0.2.1/protkit/metrics/__init__.py` & `protkit-0.2.2/protkit/metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `protkit-0.2.1/protkit/metrics/scoring_matrix.py` & `protkit-0.2.2/protkit/metrics/scoring_matrix.py`

 * *Files identical despite different names*

### Comparing `protkit-0.2.1/protkit/metrics/sequence_eval.py` & `protkit-0.2.2/protkit/metrics/sequence_eval.py`

 * *Files identical despite different names*

### Comparing `protkit-0.2.1/protkit/metrics/structure_eval.py` & `protkit-0.2.2/protkit/metrics/structure_eval.py`

 * *Files identical despite different names*

### Comparing `protkit-0.2.1/protkit/properties/__init__.py` & `protkit-0.2.2/protkit/properties/__init__.py`

 * *Files identical despite different names*

### Comparing `protkit-0.2.1/protkit/properties/bond_angles.py` & `protkit-0.2.2/protkit/properties/bond_angles.py`

 * *Files identical despite different names*

### Comparing `protkit-0.2.1/protkit/properties/bond_lengths.py` & `protkit-0.2.2/protkit/properties/bond_lengths.py`

 * *Files identical despite different names*

### Comparing `protkit-0.2.1/protkit/properties/bounds.py` & `protkit-0.2.2/protkit/properties/bounds.py`

 * *Files identical despite different names*

### Comparing `protkit-0.2.1/protkit/properties/charge.py` & `protkit-0.2.2/protkit/properties/charge.py`

 * *Files identical despite different names*

### Comparing `protkit-0.2.1/protkit/properties/chemical_class.py` & `protkit-0.2.2/protkit/properties/chemical_class.py`

 * *Files identical despite different names*

### Comparing `protkit-0.2.1/protkit/properties/circular_variance.py` & `protkit-0.2.2/protkit/properties/circular_variance.py`

 * *Files identical despite different names*

### Comparing `protkit-0.2.1/protkit/properties/dihedral_angles.py` & `protkit-0.2.2/protkit/properties/dihedral_angles.py`

 * *Files identical despite different names*

### Comparing `protkit-0.2.1/protkit/properties/donors_acceptors.py` & `protkit-0.2.2/protkit/properties/donors_acceptors.py`

 * *Files identical despite different names*

### Comparing `protkit-0.2.1/protkit/properties/hydrophobicity.py` & `protkit-0.2.2/protkit/properties/hydrophobicity.py`

 * *Files identical despite different names*

### Comparing `protkit-0.2.1/protkit/properties/interface.py` & `protkit-0.2.2/protkit/properties/interface.py`

 * *Files identical despite different names*

### Comparing `protkit-0.2.1/protkit/properties/mass.py` & `protkit-0.2.2/protkit/properties/mass.py`

 * *Files identical despite different names*

### Comparing `protkit-0.2.1/protkit/properties/polarity.py` & `protkit-0.2.2/protkit/properties/polarity.py`

 * *Files identical despite different names*

### Comparing `protkit-0.2.1/protkit/properties/surface_area.py` & `protkit-0.2.2/protkit/properties/surface_area.py`

 * *Files identical despite different names*

### Comparing `protkit-0.2.1/protkit/properties/vdw_radius.py` & `protkit-0.2.2/protkit/properties/vdw_radius.py`

 * *Files identical despite different names*

### Comparing `protkit-0.2.1/protkit/properties/volume.py` & `protkit-0.2.2/protkit/properties/volume.py`

 * *Files identical despite different names*

### Comparing `protkit-0.2.1/protkit/seq/__init__.py` & `protkit-0.2.2/protkit/seq/__init__.py`

 * *Files identical despite different names*

### Comparing `protkit-0.2.1/protkit/seq/antibody_sequence.py` & `protkit-0.2.2/protkit/seq/antibody_sequence.py`

 * *Files identical despite different names*

### Comparing `protkit-0.2.1/protkit/seq/nucleotide_sequence.py` & `protkit-0.2.2/protkit/seq/nucleotide_sequence.py`

 * *Files identical despite different names*

### Comparing `protkit-0.2.1/protkit/seq/protein_sequence.py` & `protkit-0.2.2/protkit/seq/protein_sequence.py`

 * *Files identical despite different names*

### Comparing `protkit-0.2.1/protkit/seq/sequence.py` & `protkit-0.2.2/protkit/seq/sequence.py`

 * *Files 12% similar despite different names*

```diff
@@ -70,14 +70,36 @@
             return ""
         if len(self._sequence[0]) == 1:
             spacer = ""
         else:
             spacer = " "
         return spacer.join(self._sequence)
 
+    def to_string(self, start_index: int, end_index: int) -> str:
+        """
+        Returns a string representation of a subsequence.
+
+        Args:
+            start_index (int): The start index of the subsequence.
+            end_index (int): The end index of the subsequence.
+
+        Returns:
+            str: The string representation of the subsequence.
+        """
+        if self._sequence is None or len(self.sequence) == 0:
+            return ""
+
+        sub_sequence = [self._sequence[i] for i in range(start_index, min(end_index + 1, self.length))]
+
+        if len(self._sequence[0]) == 1:
+            return "".join(sub_sequence)
+        else:
+            return " ".join(sub_sequence)
+
+
     def __len__(self):
         """
         Returns the length of the sequence.
 
         Returns:
             int: The length of the sequence.
         """
```

### Comparing `protkit-0.2.1/protkit/seq/sequence_alignment.py` & `protkit-0.2.2/protkit/seq/sequence_alignment.py`

 * *Files identical despite different names*

### Comparing `protkit-0.2.1/protkit/structure/__init__.py` & `protkit-0.2.2/protkit/structure/__init__.py`

 * *Files identical despite different names*

### Comparing `protkit-0.2.1/protkit/structure/atom.py` & `protkit-0.2.2/protkit/structure/atom.py`

 * *Files identical despite different names*

### Comparing `protkit-0.2.1/protkit/structure/chain.py` & `protkit-0.2.2/protkit/structure/chain.py`

 * *Files identical despite different names*

### Comparing `protkit-0.2.1/protkit/structure/protein.py` & `protkit-0.2.2/protkit/structure/protein.py`

 * *Files identical despite different names*

### Comparing `protkit-0.2.1/protkit/structure/residue.py` & `protkit-0.2.2/protkit/structure/residue.py`

 * *Files identical despite different names*

### Comparing `protkit-0.2.1/protkit/tasks/surface_area_calculator.py` & `protkit-0.2.2/protkit/tasks/surface_area_calculator.py`

 * *Files identical despite different names*

### Comparing `protkit-0.2.1/protkit/tools/freesasa_adaptor.py` & `protkit-0.2.2/protkit/tools/freesasa_adaptor.py`

 * *Files identical despite different names*

### Comparing `protkit-0.2.1/protkit.egg-info/PKG-INFO` & `protkit-0.2.2/protkit.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: protkit
-Version: 0.2.1
+Version: 0.2.2
 Summary: A unified toolkit for structural protein engineering.
 Author-email: Fred Senekal <fred@silicogenesis.com>
 Maintainer-email: Fred Senekal <fred@silicogenesis.com>
 Project-URL: Homepage, https://protkit.silicogenesis.com
 Project-URL: Repository, https://github.com/silicogenesis/protkit
 Project-URL: Documentation, https://silicogenesis.github.io/protkit
 Keywords: protein,protein engineering,structural biology,computational biology,biology,bioinformatics,sequence,amino acid,residue,dataset,PDB,antibody,antibody engineering,cdr
```

### Comparing `protkit-0.2.1/protkit.egg-info/SOURCES.txt` & `protkit-0.2.2/protkit.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -52,12 +52,15 @@
 protkit/seq/sequence_alignment.py
 protkit/structure/__init__.py
 protkit/structure/atom.py
 protkit/structure/chain.py
 protkit/structure/protein.py
 protkit/structure/residue.py
 protkit/tasks/__init__.py
+protkit/tasks/protonator.py
 protkit/tasks/surface_area_calculator.py
 protkit/tools/__init__.py
 protkit/tools/freesasa_adaptor.py
+protkit/tools/reduce_adaptor.py
 tests/quick_start_guide.py
+tests/test_reduce.py
 venv/bin/activate_this.py
```

### Comparing `protkit-0.2.1/pyproject.toml` & `protkit-0.2.2/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 package-dir = "protkit"
 
 [tool.setuptools.packages]
 find = {}
 
 [project]
 name = "protkit"
-version = "0.2.1"
+version = "0.2.2"
 requires-python = ">=3.6"
 authors = [
     { name="Fred Senekal", email="fred@silicogenesis.com"},
 ]
 maintainers = [
     { name="Fred Senekal", email="fred@silicogenesis.com"},
 ]
```

### Comparing `protkit-0.2.1/tests/quick_start_guide.py` & `protkit-0.2.2/tests/quick_start_guide.py`

 * *Files 27% similar despite different names*

```diff
@@ -34,66 +34,390 @@
     # is available for later retrieval!
     protein.set_attribute("note", "Experimenting with Protkit")
     ProtIO.save(protein, "1ahw.prot")
     protein2 = ProtIO.load("1ahw.prot")[0]
     print(protein2.get_attribute('surface_area'))
     print(protein2.get_attribute('note'))
 
+
+def prep_data():
+    from protkit.download import Download
+    from protkit.file_io import ProtIO
+
+    # Download a PDB file from the RCSB PDB database and save it to a file.
+    Download.download_pdb_file_from_rcsb("1ahw", "1ahw.pdb")
+    Download.download_pdb_file_from_rcsb("3i40", "3i40.pdb")
+    Download.download_pdb_file_from_rcsb("4nkq", "4nkq.pdb")
+    Download.download_pdb_file_from_rcsb("6bom", "6bom.pdb")
+
+    # Load a PDB file into a Protein object.
+    ProtIO.convert("1ahw.pdb", "1ahw.prot")
+    ProtIO.convert("3i40.pdb", "3i40.prot")
+    ProtIO.convert("4nkq.pdb", "4nkq.prot")
+    ProtIO.convert("6bom.pdb", "6bom.prot")
+
+    # Download a FASTA file from RCSB PDB and save it to file.
+    Download.download_fasta_file_from_rcsb("1ahw", "1ahw.fasta")
+    Download.download_fasta_file_from_rcsb("3i40", "1ahw.3i40")
+    Download.download_fasta_file_from_rcsb("4nkq", "4nkq.fasta")
+    Download.download_fasta_file_from_rcsb("6bom", "6bom.fasta")
+
+
 def download_pdb_example():
     from protkit.download import Download
 
     # Download a PDB file from the RCSB PDB database and save it to a file.
-    Download.download_pdb_file_from_rcsb("1ahw", "data/pdb_files/rcsb/1ahw.pdb")
+    Download.download_pdb_file_from_rcsb("1ahw", "data/pdb/rcsb/1ahw.pdb")
 
     # Download a PDB file from the SAbDab database and save it to a file.
-    Download.download_pdb_file_from_sabdab("1ahw", "data/pdb_files/sabdab/1ahw.pdb")
+    Download.download_pdb_file_from_sabdab("1ahw", "data/pdb/sabdab/1ahw.pdb")
 
     # Download multiple PDB files from the RCSB PDB in parallel and save them to a directory.
-    Download.download_pdb_files_from_rcsb(["1ahw", "1a4y", "1a6m"], "data/pdb_files/rcsb/", n_jobs=3)
+    Download.download_pdb_files_from_rcsb(["1ahw", "1a4y", "1a6m"], "data/pdb/rcsb/", n_jobs=3)
+
 
 def download_fasta_example():
     from protkit.download import Download
 
     # Download a Fasta file from the Uniprot database and save it to a file.
-    Download.download_fasta_file_from_uniprot("P12345", "data/fasta_files/uniprot/P12345.xml")
-
-    # Download multiple Fasta files from the RCSB database in parallel and save them to a directory.
-    Download.download_fasta_files_from_rcsb(["P12345", "P12346", "P12347"], "data/fasta_files/rcsb/")
+    Download.download_fasta_file_from_uniprot("P01308", "data/fasta/uniprot/P01308.fasta")
 
     # Download multiple Fasta files from the Uniprot database in parallel and save them to a directory.
-    Download.download_fasta_files_from_uniprot(["P12345", "P12346", "P12347"], "data/fasta_files/rcsb/")
+    Download.download_fasta_files_from_uniprot(["P01308", "P68871", "P00533"], "data/fasta/uniprot", n_jobs=3)
+
+    # Download a Fasta file from the RCSB PDB database and save it to a file.
+    Download.download_fasta_file_from_rcsb("1ahw", "data/fasta/rcsb/1ahw.fasta")
+
+    # Download multiple Fasta files from the RCSB PDB database in parallel and save them to a directory.
+    Download.download_fasta_files_from_rcsb(["1ahw", "1a4y", "1a6m"], "data/fasta/rcsb/", n_jobs=3)
 
 
 def download_cif_example():
     from protkit.download import Download
 
     # Download a CIF file from the RCSB PDB database and save it to a file.
-    Download.download_cif_file_from_rcsb("1ahw", "data/cif_files/rcsb/1ahw.cif")
+    Download.download_cif_file_from_rcsb("1ahw", "data/cif/rcsb/1ahw.cif")
 
     # Download multiple CIF files from the RCSB PDB database in parallel and save them to a directory.
-    Download.download_cif_files_from_rcsb(["1ahw", "1a4y", "1a6m"], "data/cif_files/rcsb/")
+    Download.download_cif_files_from_rcsb(["1ahw", "1a4y", "1a6m"], "data/cif/rcsb/")
 
     # Download a binary CIF file from the RCSB PDB database and save it to a file.
-    Download.download_binary_cif_file_from_rcsb("1ahw", "data/cif_files/rcsb/1ahw.bcif")
+    Download.download_binary_cif_file_from_rcsb("1ahw", "data/cif/rcsb/1ahw.bcif")
 
     # Download multiple binary CIF files from the RCSB PDB database in parallel and save them to a directory.
-    Download.download_binary_cif_files_from_rcsb(["1ahw", "1a4y", "1a6m"], "data/cif_files/rcsb/")
+    Download.download_binary_cif_files_from_rcsb(["1ahw", "1a4y", "1a6m"], "data/cif/rcsb/")
 
-def prep_data():
-    from protkit.download import Download
+
+def file_io_pdb():
+    from protkit.file_io import PDBIO
+
+    protein = PDBIO.load("1ahw.pdb")[0]
+
+    protein.keep_chains(["A", "B"])
+
+    PDBIO.save(protein, "1ahw_AB.pdb")
+
+
+def file_io_prot():
     from protkit.file_io import ProtIO
 
-    # Download a PDB file from the RCSB PDB database and save it to a file.
-    Download.download_pdb_file_from_rcsb("1ahw", "1ahw.pdb")
+    protein = ProtIO.convert("1ahw.pdb", "1ahw.prot")
 
-    # Load a PDB file into a Protein object.
-    ProtIO.convert("1ahw.pdb", "1ahw.prot")
+    protein = ProtIO.load("1ahw.prot")[0]
+
+    ProtIO.save(protein, "1ahw.prot")
+
+
+def file_io_prot_multisave():
+    from protkit.file_io import ProtIO, PDBIO
+
+    protein1 = PDBIO.load("1ahw.pdb")[0]
+    protein2 = PDBIO.load("4nkq.pdb")[0]
+
+    ProtIO.save([protein1, protein2], "database.prot")
+
+
+def file_io_prot_compression():
+    from protkit.file_io import ProtIO
+
+    protein = ProtIO.load("1ahw.prot", decompress=True)[0]
+    ProtIO.save(protein, "1ahw.prot.json", compress=False)
+
+
+def file_io_fasta_load():
+    from protkit.file_io import FastaIO
+
+    sequences = FastaIO.load("1ahw.fasta")
+    for sequence in sequences:
+        print(f"{sequence.chain_id}: {sequence}")
+
+
+def file_io_fasta_save():
+    from protkit.file_io import FastaIO
+
+    sequences = FastaIO.load("1ahw.fasta")
+    FastaIO.save(sequences, "1ahw_copy.fasta")
+    FastaIO.save(sequences[0], "1ahw_A.fasta")
+
+
+def file_io_pqr():
+    from protkit.file_io import PQRIO
+
+    protein = PQRIO.load("1ahw.pqr")[0]
+
+    PQRIO.save(protein, "1ahw_copy.pqr")
+
+
+def file_io_cif():
+    from protkit.file_io import MMTFIO
+
+    protein = MMTFIO.load("1ahw.cif")[0]
+
+    MMTFIO.save(protein, "1ahw_copy.cif")
+
+
+def file_io_mmtf():
+    from protkit.file_io import MMTFIO
+
+    protein = MMTFIO.load("1ahw.mmtf")[0]
+
+
+def representation_protein():
+    # Loading a Protein
+    from protkit.file_io import ProtIO
+
+    protein = ProtIO.load("1ahw.prot")[0]
+
+    # Accessing Chains in a Protein
+    for chain in protein.chains:
+        print(f"{chain.chain_id}: {chain.num_residues} residues")
+        print(chain.sequence)
+
+    chain_a = protein.get_chain("A")
+    print(chain_a.sequence)
+
+    protein2 = protein.copy()
+    protein2.keep_chains(["A", "B"])
+    print(protein.num_chains)
+    print(protein2.num_chains)
+
+    protein3 = protein.copy()
+    protein3.remove_chains(["C", "D"])
+    print(protein3.num_chains)
+
+    # Isolating Chains
+    protein2 = protein.copy()
+    protein2.keep_chains(["A", "B"])
+    print(protein.num_chains)
+    print(protein2.num_chains)
+
+    # Renaming Chains
+    protein.rename_chain("A", "Z")
+
+
+def representation_protein_access():
+    from protkit.file_io import ProtIO
+
+    protein = ProtIO.load("1ahw.prot")[0]
+
+    # Accessing Residues in a Protein
+    for residue in protein.residues:
+        print(f"{residue.id}: {residue.residue_type}")
+
+    # Accessing Atoms in a Protein
+    coordinates = [(atom.x, atom.y, atom.z) for atom in protein.atoms]
+    print(coordinates)
+
+    # Powerful filters
+    atoms = protein.filter_atoms(
+        chain_criteria=[("chain_id", "A")],
+        residue_criteria=[("residue_type", "PRO")],
+        atom_criteria=[("atom_type", ["C", "CA", "N"])])
+    for atom in atoms:
+        print(f"{atom.residue.residue_code}, {atom.atom_type}, {atom.x}, {atom.y}, {atom.z}")
+
+    # Protein statistics
+    print(protein.num_chains)
+
+    print(protein.num_residues)
+    print(protein.num_disordered_residues)
+    print(protein.num_hetero_residues)
+    print(protein.num_water_residues)
+
+    print(protein.num_atoms)
+    print(protein.num_disordered_atoms)
+    print(protein.num_hetero_atoms)
+    print(protein.num_heavy_atoms)
+    print(protein.num_hydrogen_atoms)
+
+
+def representation_chain():
+    from protkit.file_io import ProtIO
+
+    # Identifying a Chain
+    protein = ProtIO.load("1ahw.prot")[0]
+    chain = protein.get_chain("A")
+    print(chain.chain_id)
+
+    protein.rename_chain("A", "Z")
+    print(chain.chain_id)
+    chain.chain_id = "X"
+
+    # Chain Sequence
+    print(chain.sequence)
+
+    # Accessing Residues in a Chain
+    for residue in chain.residues:
+        print(f"{residue.id}: {residue.residue_type}")
+
+    residue = chain.get_residue(0)
+    print(residue.id)
+
+    # Accessing Atoms in a Chain
+    for atom in chain.atoms:
+        print(f"{atom.id}")
+
+
+def representation_residue():
+    # Identifying a Residue
+    from protkit.file_io import ProtIO
+
+    protein = ProtIO.load("1ahw.prot")[0]
+    chain = protein.get_chain("A")
+    residue = chain.get_residue(0)
+
+    # Core Residue Properties
+    print(residue.residue_type)  # eg. GLY
+    print(residue.short_code)  # eg. G
+    print(residue.sequence_no)  # eg. 100
+    print(residue.insertion_code)  # eg. A
+    print(residue.is_disordered)  # eg. True
+    print(residue.is_hetero)  # eg. False
+
+    print(residue.sequence_code)  # eg. 100A
+    print(residue.residue_code)  # eg. GLY100A
+    print(residue.id)  # eg. A:GLY100A
+
+    # Accessing Atoms in a Residue
+    for atom in residue.atoms:
+        print(f"{atom.id}")
+
+    # Modifying the Atoms in a Residue
+    residue.keep_backbone_atoms()
+
+    residue.keep_atoms(["N", "CA", "C"])
+
+    residue.remove_atoms(["OXT"])
+
+    residue.remove_hydrogen_atoms()
+
+
+def representation_atom():
+    # Identifying an Atom
+    from protkit.file_io import ProtIO
+
+    protein = ProtIO.load("1ahw.prot")[0]
+    residue = protein.get_chain("A").get_residue(0)
+    atom = residue.get_atom("CA")
+
+    print(atom.id)
+    print(atom.atom_type)
+
+    print(atom.element)  # eg. C
+    print(atom.x, atom.y, atom.z)  # eg. 12.446, 8.496, 43.176
+    print(atom.is_disordered)  # eg. False
+    print(atom.is_hetero)  # eg. False
+
+def representation_atom_fix_disordered():
+    from protkit.file_io import ProtIO
+
+    protein = ProtIO.load("1ahw.prot")[0]
+    protein.fix_disordered_atoms()
+
+
+def representation_attributes():
+    from protkit.file_io import ProtIO
+
+    protein = ProtIO.load("3i40.prot")[0]
+
+    protein.set_attribute("note", "The file describes Human Insulin")
+    protein.set_attribute("organism", "Homo Sapiens")
+    protein.set_attribute("resolution", 1.85)
+    protein.get_chain("A").set_attribute("name", "Insulin A chain")
+    protein.get_chain("A").get_residue(0).set_attribute('first', True)
+
+    print(protein.get_attribute("note"))
+    print(protein.get_attribute("organism"))
+    print(protein.get_attribute("resolution"))
+    print(protein.get_chain("A").has_attribute("name"))
+    print(protein.get_chain("A").get_attribute("name"))
+    print(protein.get_chain("B").has_attribute("name"))
+    print(protein.get_chain("A").get_residue(0).get_attribute('first'))
+
+
+def quality_create_copy():
+    from protkit.file_io import ProtIO
+
+    protein = ProtIO.load("3i40.prot")[0]
+    protein2 = protein.copy()
+
+
+def quality_remove_water_molecules():
+    from protkit.file_io import ProtIO
+
+    protein = ProtIO.load("6bom.prot")[0]
+    print(f"{protein.num_water_residues}")
+    protein.remove_water_residues()
+    print(f"{protein.num_water_residues}")
+
+    protein.get_chain("A").remove_water_residues()
+
+
+def quality_remove_hetero_residues():
+    from protkit.file_io import ProtIO
+
+    protein = ProtIO.load("6bom.prot")[0]
+    print(f"{protein.num_hetero_residues}")
+    protein.remove_hetero_residues("TRS")
+    print(f"{protein.num_hetero_residues}")
+
+    protein.remove_hetero_residues(["TRS", "SO4"])
+
+
+def quality_fixing_disordered_atoms():
+    from protkit.file_io import ProtIO
+
+    protein = ProtIO.load("3i40.prot")[0]
+    print(f"{protein.num_disordered_atoms}")
+    print(protein.get_chain("A").get_residue(13).is_disordered)
+    print(protein.get_chain("A").get_residue(13).get_atom("CA").is_disordered)
+    print(protein.get_chain("A").get_residue(13).get_atom("CB").is_disordered)
+
+    protein.fix_disordered_atoms()
+    print(protein.get_chain("A").get_residue(13).get_atom("CB").is_disordered)
+    print(f"{protein.num_disordered_atoms}")
+
+
+def quality_removing_hydrogen_atoms():
+    from protkit.file_io import ProtIO
+
+    protein = ProtIO.load("1a4y_A_B.prot")[0]
+
+    print(f"{protein.num_atoms} atoms")
+    print(f"{protein.num_heavy_atoms} heavy atoms")
+    print(f"{protein.num_hydrogen_atoms} hydrogen atoms")
+
+    protein.remove_hydrogen_atoms()
+
+    print(f"{protein.num_hydrogen_atoms} hydrogen atoms after removal")
+
+
+# prep_data()
+quality_removing_hydrogen_atoms()
 
-    # Download a FASTA file from RCSB PDB and save it to file.
-    Download.download_fasta_file_from_rcsb("1ahw", "1ahw.fasta")
 
 def properties_hydrophobicity():
     from protkit.file_io import ProtIO
     from protkit.properties import Hydrophobicity
 
     protein = ProtIO.load("1ahw.prot")[0]
     Hydrophobicity.hydrophobicity_of_protein(protein, assign_attribute=True)
@@ -341,14 +665,15 @@
     for residue in residues1:
         if residue.get_attribute("ca_in_interface"):
             print(residue.id)
 
 # prep_data()
 
 # quick_start_example()
+
 # download_pdb_example()
 # download_fasta_example()
 # download_cif_example()
 
 # properties_hydrophobicity()
 # properties_hydrophobicity_class()
 # properties_mass()
```

### Comparing `protkit-0.2.1/venv/bin/activate_this.py` & `protkit-0.2.2/venv/bin/activate_this.py`

 * *Files identical despite different names*

