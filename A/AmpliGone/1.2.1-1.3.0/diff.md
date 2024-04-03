# Comparing `tmp/AmpliGone-1.2.1.tar.gz` & `tmp/AmpliGone-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "AmpliGone-1.2.1.tar", last modified: Tue Feb 28 11:22:21 2023, max compression
+gzip compressed data, was "AmpliGone-1.3.0.tar", last modified: Tue Aug  8 13:00:50 2023, max compression
```

## Comparing `AmpliGone-1.2.1.tar` & `AmpliGone-1.3.0.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 11:22:21.874104 AmpliGone-1.2.1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 11:22:21.874104 AmpliGone-1.2.1/AmpliGone/
--rw-r--r--   0 runner    (1001) docker     (123)    12463 2023-02-28 11:22:13.000000 AmpliGone-1.2.1/AmpliGone/AmpliGone.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-28 11:22:13.000000 AmpliGone-1.2.1/AmpliGone/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6268 2023-02-28 11:22:13.000000 AmpliGone-1.2.1/AmpliGone/cut_reads.py
--rw-r--r--   0 runner    (1001) docker     (123)     2562 2023-02-28 11:22:13.000000 AmpliGone-1.2.1/AmpliGone/cutlery.py
--rw-r--r--   0 runner    (1001) docker     (123)     6512 2023-02-28 11:22:13.000000 AmpliGone-1.2.1/AmpliGone/fasta2bed.py
--rw-r--r--   0 runner    (1001) docker     (123)     5517 2023-02-28 11:22:13.000000 AmpliGone-1.2.1/AmpliGone/func.py
--rw-r--r--   0 runner    (1001) docker     (123)     6447 2023-02-28 11:22:13.000000 AmpliGone-1.2.1/AmpliGone/io_ops.py
--rw-r--r--   0 runner    (1001) docker     (123)     5545 2023-02-28 11:22:13.000000 AmpliGone-1.2.1/AmpliGone/mappreset.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-02-28 11:22:13.000000 AmpliGone-1.2.1/AmpliGone/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 11:22:21.874104 AmpliGone-1.2.1/AmpliGone.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3618 2023-02-28 11:22:21.000000 AmpliGone-1.2.1/AmpliGone.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      452 2023-02-28 11:22:21.000000 AmpliGone-1.2.1/AmpliGone.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-28 11:22:21.000000 AmpliGone-1.2.1/AmpliGone.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-02-28 11:22:21.000000 AmpliGone-1.2.1/AmpliGone.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-28 11:22:21.000000 AmpliGone-1.2.1/AmpliGone.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-02-28 11:22:21.000000 AmpliGone-1.2.1/AmpliGone.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-02-28 11:22:21.000000 AmpliGone-1.2.1/AmpliGone.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-02-28 11:22:13.000000 AmpliGone-1.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3618 2023-02-28 11:22:21.874104 AmpliGone-1.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2531 2023-02-28 11:22:13.000000 AmpliGone-1.2.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-28 11:22:21.874104 AmpliGone-1.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1645 2023-02-28 11:22:13.000000 AmpliGone-1.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 13:00:50.950655 AmpliGone-1.3.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 13:00:50.950655 AmpliGone-1.3.0/AmpliGone/
+-rw-r--r--   0 runner    (1001) docker     (123)    12496 2023-08-08 13:00:47.000000 AmpliGone-1.3.0/AmpliGone/AmpliGone.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 13:00:47.000000 AmpliGone-1.3.0/AmpliGone/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6811 2023-08-08 13:00:47.000000 AmpliGone-1.3.0/AmpliGone/cut_reads.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2584 2023-08-08 13:00:47.000000 AmpliGone-1.3.0/AmpliGone/cutlery.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7420 2023-08-08 13:00:47.000000 AmpliGone-1.3.0/AmpliGone/fasta2bed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5517 2023-08-08 13:00:47.000000 AmpliGone-1.3.0/AmpliGone/func.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6447 2023-08-08 13:00:47.000000 AmpliGone-1.3.0/AmpliGone/io_ops.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5545 2023-08-08 13:00:47.000000 AmpliGone-1.3.0/AmpliGone/mappreset.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-08-08 13:00:47.000000 AmpliGone-1.3.0/AmpliGone/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 13:00:50.950655 AmpliGone-1.3.0/AmpliGone.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3618 2023-08-08 13:00:50.000000 AmpliGone-1.3.0/AmpliGone.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      452 2023-08-08 13:00:50.000000 AmpliGone-1.3.0/AmpliGone.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 13:00:50.000000 AmpliGone-1.3.0/AmpliGone.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-08-08 13:00:50.000000 AmpliGone-1.3.0/AmpliGone.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 13:00:50.000000 AmpliGone-1.3.0/AmpliGone.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-08-08 13:00:50.000000 AmpliGone-1.3.0/AmpliGone.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-08-08 13:00:50.000000 AmpliGone-1.3.0/AmpliGone.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-08-08 13:00:47.000000 AmpliGone-1.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3618 2023-08-08 13:00:50.950655 AmpliGone-1.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2531 2023-08-08 13:00:47.000000 AmpliGone-1.3.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-08 13:00:50.950655 AmpliGone-1.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1645 2023-08-08 13:00:47.000000 AmpliGone-1.3.0/setup.py
```

### Comparing `AmpliGone-1.2.1/AmpliGone/AmpliGone.py` & `AmpliGone-1.3.0/AmpliGone/AmpliGone.py`

 * *Files 1% similar despite different names*

```diff
@@ -343,15 +343,18 @@
         ProcessedReads.reset_index(drop=True)
     log.info("Done removing primer sequences")
 
     total_nuc_preprocessing = sum(tuple(chain(IndexedReads["Sequence"].str.len())))
     removed_coordinates = tuple(chain(*ProcessedReads["Removed_coordinates"]))
 
     log.info(
-        f"\tRemoved a total of [bold cyan]{len(removed_coordinates)}[/bold cyan] nucleotides. This is [bold cyan]{round((len(removed_coordinates)/total_nuc_preprocessing)*100, 2)}%[/bold cyan] of the total amount of nucleotides present in the original reads."
+        f"\tRemoved a total of [bold cyan]{len(removed_coordinates)}[/bold cyan] nucleotides."
+    )
+    log.info(
+        f"\tThis is [bold cyan]{round((len(removed_coordinates)/total_nuc_preprocessing)*100, 2)}%[/bold cyan] of the total amount of nucleotides present in the original reads."
     )
     log.info(
         f"\tThese nucleotides were removed from [bold cyan]{len(set(removed_coordinates))}[/bold cyan] unique nucleotide-coordinates."
     )
     log.info(
         f"\tThese nucleotide-coordinates correspond to the coordinates of [bold cyan]{len(primer_df)}[/bold cyan] (found) primers."
     )
```

### Comparing `AmpliGone-1.2.1/AmpliGone/cut_reads.py` & `AmpliGone-1.3.0/AmpliGone/cut_reads.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from collections import defaultdict
+
 import mappy as mp
 import pandas as pd
 
 from .cutlery import PositionInOrAfterPrimer, PositionInOrBeforePrimer
 
 
 def cut_read(
@@ -66,24 +68,32 @@
     preset,
     scoring,
     fragment_lookaround_size,
     amplicon_type,
     workers,
 ):
     Frame, _threadnumber = data
-    RVSet = set()
-    FWSet = set()
-    for _, start, end, strand in primer_df[["start", "end", "strand"]].itertuples():
+
+    RVDict = defaultdict(set)
+    FWDict = defaultdict(set)
+
+    reference_ids = set(primer_df["ref"].unique())
+    for refid in reference_ids:
+        RVDict[refid] = set()
+        FWDict[refid] = set()
+
+    for _, refid, start, end, strand in primer_df[
+        ["ref", "start", "end", "strand"]
+    ].itertuples():
+
         for coord in range(start + 1, end):  # +1 because reference is 1-based
             if strand == "+":
-                FWSet.add(coord)
+                FWDict[refid].add(coord)
             elif strand == "-":
-                RVSet.add(coord)
-    FWList = tuple(FWSet)  # Since tuples are hashable
-    RVList = tuple(RVSet)
+                RVDict[refid].add(coord)
 
     Aln = mp.Aligner(
         reference,
         preset=preset,
         best_n=1,
         scoring=scoring,
         extra_flags=0x4000000,  # Distinguish between match and mismatch: MM_F_EQX flag in minimap2
@@ -123,27 +133,35 @@
                         removed_coords_fw + removed_coords_rv
                     )
                     cutting_is_done = True
                     break
 
                 previous_seq = seq
 
+                # Fetch the primer coordinates that correspond to the reference that the read maps to
+                # we're using tuples here because they are hashable
+                FWTuple = tuple(FWDict[hit.ctg])
+                RVTuple = tuple(RVDict[hit.ctg])
+
+                if not FWTuple or not RVTuple:
+                    print(FWTuple, RVTuple, hit.ctg)
+
                 qstart = hit.q_st
                 qend = hit.q_en
 
                 if (
                     amplicon_type == "end-to-end"
                     or (amplicon_type == "end-to-mid" and hit.strand == 1)
                     or amplicon_type == "fragmented"
                 ):
                     seq, qual, removed_fw, qstart, qend = cut_read(
                         seq,
                         qual,
                         PositionNeedsCutting=PositionInOrBeforePrimer,
-                        primer_list=FWList,
+                        primer_list=FWTuple,
                         position_on_reference=hit.r_st,
                         cut_direction=1,
                         read_direction=hit.strand,
                         cigar=hit.cigar,
                         query_start=qstart,
                         query_end=qend,
                         fragment_lookaround_size=fragment_lookaround_size,
@@ -155,15 +173,15 @@
                     or (amplicon_type == "end-to-mid" and hit.strand == -1)
                     or amplicon_type == "fragmented"
                 ):
                     seq, qual, removed_rv, qstart, qend = cut_read(
                         seq,
                         qual,
                         PositionNeedsCutting=PositionInOrAfterPrimer,
-                        primer_list=RVList,
+                        primer_list=RVTuple,
                         position_on_reference=hit.r_en,
                         cut_direction=-1,
                         read_direction=hit.strand,
                         cigar=list(reversed(hit.cigar)),
                         query_start=qstart,
                         query_end=qend,
                         fragment_lookaround_size=fragment_lookaround_size,
```

### Comparing `AmpliGone-1.2.1/AmpliGone/cutlery.py` & `AmpliGone-1.3.0/AmpliGone/cutlery.py`

 * *Files 3% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 
     Returns
     -------
         A boolean value.
 
     """
     d = lambda x: abs(x - pos)
-    near = min(clist, key=d)
+    near = min(clist, key=d, default=0)
     return abs(pos - near) < max_lookaround and pos <= near
 
 
 @lru_cache(maxsize=2000000)
 def PositionInOrAfterPrimer(pos, clist, max_lookaround):
     """Given a position, a list of positions, and a maximum distance, return True if the position is
     within the maximum distance of the closest position in the list AND the position is greater than or equal
@@ -43,15 +43,15 @@
 
     Returns
     -------
         A boolean value.
 
     """
     d = lambda x: abs(x - pos)
-    near = min(clist, key=d)
+    near = min(clist, key=d, default=0)
     return abs(pos - near) < max_lookaround and pos >= near
 
 
 @lru_cache(maxsize=2000000)
 def ReadBeforePrimer(pos, clist):
     if pos in clist:
         return False
```

### Comparing `AmpliGone-1.2.1/AmpliGone/fasta2bed.py` & `AmpliGone-1.3.0/AmpliGone/fasta2bed.py`

 * *Files 11% similar despite different names*

```diff
@@ -87,60 +87,67 @@
 
     """
     keyl = ("LEFT", "PLUS", "POSITIVE", "FORWARD")
     keyr = ("RIGHT", "MINUS", "NEGATIVE", "REVERSE")
 
     primers = list(SeqIO.parse(primerfile, "fasta"))
 
-    ref_file = SeqIO.read(referencefile, "fasta")
-    ref_seq = str(ref_file.seq)
-
-    for primer in primers:
-        seq = str(primer.seq)
-        revcomp = Seq.reverse_complement(seq)
-
-        coords = get_coords(seq, ref_seq, err_rate)
-        rev_coords = get_coords(revcomp, ref_seq, err_rate)
-        if coords and rev_coords:
-            log.warning(
-                f"Primer [yellow underline]{primer.id}[/yellow underline] found on both forward and reverse strand of '[yellow]{ref_file.name}[/yellow]'.\n[yellow bold]Check to see if this is intended.[/yellow bold]"
-            )
-        if not coords and not rev_coords:
-            log.warning(
-                f"Skipping [yellow underline]{primer.id}[/yellow underline] as it is found on neither forward or reverse strand of [yellow underline]{ref_file.name}[/yellow underline].\n[yellow bold]Check to see if this is intended.[/yellow bold]"
-            )
-            continue
-        if coords and len(coords) > 1:
-            log.warning(
-                f"Primer [yellow underline]{primer.id}[/yellow underline] found on multiple locations on [underline]forward strand[/underline]: \n\t[yellow]{coords}\n[bold]Check to see if this is intended.[/yellow][/bold]"
-            )
-        if rev_coords and len(rev_coords) > 1:
-            log.warning(
-                f"Primer [yellow underline]{primer.id}[/yellow underline] found on multiple locations on [underline]reverse strand[/underline]: {rev_coords}.\nCheck to see if this is intended."
-            )
-        for start, end in coords.union(rev_coords):
-            if any(o in primer.id for o in keyl):
-                strand = "+"
-            elif any(o in primer.id for o in keyr):
-                strand = "-"
-            else:
-                log.error(
-                    f"Primer name {primer.id} does not contain orientation (e.g. {primer.id}_RIGHT). Consider suffixing with {keyl + keyr}"
+    ref_file = list(SeqIO.parse(referencefile, "fasta"))
+    ref_seq = [str(ref.seq) for ref in ref_file]
+    ref_id = [ref.id for ref in ref_file]
+
+    # The loop in a loop here is not a particularly efficient way of doing this.
+    # But this is the easiest implementation for now, and it's not like this is a particularly
+    # cpu or time intensive process anyway.
+    # Might come back to this when there's more time to create a better solution.
+    for ref_seq, ref_id in zip(ref_seq, ref_id):
+        log.info(f"Searching for primers in reference-id: [yellow]{ref_id}[/yellow]")
+        for primer in primers:
+            seq = str(primer.seq)
+            revcomp = Seq.reverse_complement(seq)
+
+            coords = get_coords(seq, ref_seq, err_rate)
+            rev_coords = get_coords(revcomp, ref_seq, err_rate)
+            if coords and rev_coords:
+                log.warning(
+                    f"\tPrimer [yellow underline]{primer.id}[/yellow underline] found on both [underline]forward[/underline] and [underline]reverse strand[/underline] of [yellow underline]{ref_id}[/yellow underline].\n\t[yellow bold]Check to see if this is intended.[/yellow bold]"
+                )
+            if not coords and not rev_coords:
+                log.warning(
+                    f"\tSkipping [yellow underline]{primer.id}[/yellow underline] as it is found on neither [underline]forward[/underline] or [underline]reverse strand[/underline] of [yellow underline]{ref_id}[/yellow underline].\n\t[yellow bold]Check to see if this is intended.[/yellow bold]"
+                )
+                continue
+            if coords and len(coords) > 1:
+                log.warning(
+                    f"\tPrimer [yellow underline]{primer.id}[/yellow underline] found on multiple locations on [underline]forward strand[/underline] of [yellow underline]{ref_id}[/yellow underline]: \n\t[yellow]{coords}\n\t[bold]Check to see if this is intended.[/yellow][/bold]"
+                )
+            if rev_coords and len(rev_coords) > 1:
+                log.warning(
+                    f"\tPrimer [yellow underline]{primer.id}[/yellow underline] found on multiple locations on [underline]reverse strand[/underline] of [yellow underline]{ref_id}[/yellow underline]: \n\t[yellow]{rev_coords}\n\t[bold]Check to see if this is intended.[/yellow][/bold]"
+                )
+            for start, end in coords.union(rev_coords):
+                if any(o in primer.id for o in keyl):
+                    strand = "+"
+                elif any(o in primer.id for o in keyr):
+                    strand = "-"
+                else:
+                    log.error(
+                        f"Primer name {primer.id} does not contain orientation (e.g. {primer.id}_RIGHT). Consider suffixing with {keyl + keyr}"
+                    )
+                    continue
+                yield dict(
+                    ref=ref_id,
+                    start=start,
+                    end=end,
+                    name=primer.id,
+                    score=".",
+                    strand=strand,
+                    seq=seq,
+                    revcomp=revcomp,
                 )
-                exit(1)
-            yield dict(
-                ref=ref_file.name,
-                start=start,
-                end=end,
-                name=primer.id,
-                score=".",
-                strand=strand,
-                seq=seq,
-                revcomp=revcomp,
-            )
 
 
 def CoordinateListsToBed(df, outfile):
     """It takes a dataframe with columns named "ref", "start", "end", "name", "score", and "strand" and
     writes them to a file in BED (headerless tsv) format
 
     Parameters
```

### Comparing `AmpliGone-1.2.1/AmpliGone/func.py` & `AmpliGone-1.3.0/AmpliGone/func.py`

 * *Files identical despite different names*

### Comparing `AmpliGone-1.2.1/AmpliGone/io_ops.py` & `AmpliGone-1.3.0/AmpliGone/io_ops.py`

 * *Files identical despite different names*

### Comparing `AmpliGone-1.2.1/AmpliGone/mappreset.py` & `AmpliGone-1.3.0/AmpliGone/mappreset.py`

 * *Files identical despite different names*

### Comparing `AmpliGone-1.2.1/AmpliGone.egg-info/PKG-INFO` & `AmpliGone-1.3.0/AmpliGone.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: AmpliGone
-Version: 1.2.1
+Version: 1.3.0
 Summary: Ampligone is a tool which accurately removes primer sequences from FastQ NGS reads in an amplicon sequencing experiment
 Home-page: https://rivm-bioinformatics.github.io/AmpliGone/
 Author: Florian Zwagemaker
 Author-email: ids-bioinformatics@rivm.nl
 License: AGPLv3
 Project-URL: Source Code, https://github.com/RIVM-bioinformatics/AmpliGone
 Description: [![CodeFactor](https://www.codefactor.io/repository/github/rivm-bioinformatics/ampligone/badge)](https://www.codefactor.io/repository/github/rivm-bioinformatics/ampligone)
```

### Comparing `AmpliGone-1.2.1/LICENSE` & `AmpliGone-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `AmpliGone-1.2.1/PKG-INFO` & `AmpliGone-1.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: AmpliGone
-Version: 1.2.1
+Version: 1.3.0
 Summary: Ampligone is a tool which accurately removes primer sequences from FastQ NGS reads in an amplicon sequencing experiment
 Home-page: https://rivm-bioinformatics.github.io/AmpliGone/
 Author: Florian Zwagemaker
 Author-email: ids-bioinformatics@rivm.nl
 License: AGPLv3
 Project-URL: Source Code, https://github.com/RIVM-bioinformatics/AmpliGone
 Description: [![CodeFactor](https://www.codefactor.io/repository/github/rivm-bioinformatics/ampligone/badge)](https://www.codefactor.io/repository/github/rivm-bioinformatics/ampligone)
```

### Comparing `AmpliGone-1.2.1/README.md` & `AmpliGone-1.3.0/README.md`

 * *Files identical despite different names*

### Comparing `AmpliGone-1.2.1/setup.py` & `AmpliGone-1.3.0/setup.py`

 * *Files identical despite different names*

