# Comparing `tmp/almirah-0.1.0.tar.gz` & `tmp/almirah-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "almirah-0.1.0.tar", max compression
+gzip compressed data, was "almirah-0.2.0.tar", max compression
```

## Comparing `almirah-0.1.0.tar` & `almirah-0.2.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0     1072 2023-12-14 15:12:52.530529 almirah-0.1.0/LICENSE
--rw-r--r--   0        0        0      963 2023-12-14 15:12:52.530529 almirah-0.1.0/README.md
--rw-r--r--   0        0        0      225 2023-12-14 15:12:52.530529 almirah-0.1.0/almirah/__init__.py
--rw-r--r--   0        0        0      281 2023-12-14 15:12:52.530529 almirah-0.1.0/almirah/data/__init__.py
--rw-r--r--   0        0        0     5073 2023-12-14 15:12:52.530529 almirah-0.1.0/almirah/data/configs/bids.yaml
--rw-r--r--   0        0        0     8049 2023-12-14 15:12:52.530529 almirah-0.1.0/almirah/data/convert.py
--rw-r--r--   0        0        0     4646 2023-12-14 15:12:52.530529 almirah-0.1.0/almirah/data/dataset.py
--rw-r--r--   0        0        0     3784 2023-12-14 15:12:52.530529 almirah-0.1.0/almirah/data/indexer.py
--rw-r--r--   0        0        0     6793 2023-12-14 15:12:52.534529 almirah-0.1.0/almirah/data/layout.py
--rw-r--r--   0        0        0     1448 2023-12-14 15:12:52.534529 almirah-0.1.0/almirah/data/report.py
--rw-r--r--   0        0        0    11521 2023-12-14 15:12:52.534529 almirah-0.1.0/almirah/data/specification.py
--rw-r--r--   0        0        0    16444 2023-12-14 15:12:52.534529 almirah-0.1.0/almirah/db.py
--rw-r--r--   0        0        0     3285 2023-12-14 15:12:52.534529 almirah-0.1.0/almirah/utils.py
--rw-r--r--   0        0        0     1059 2023-12-14 15:12:52.538529 almirah-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     1646 1970-01-01 00:00:00.000000 almirah-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1072 2024-04-03 06:23:38.217076 almirah-0.2.0/LICENSE
+-rw-r--r--   0        0        0      963 2024-04-03 06:23:38.217076 almirah-0.2.0/README.md
+-rw-r--r--   0        0        0      225 2024-04-03 06:23:38.217076 almirah-0.2.0/almirah/__init__.py
+-rw-r--r--   0        0        0      281 2024-04-03 06:23:38.217076 almirah-0.2.0/almirah/data/__init__.py
+-rw-r--r--   0        0        0     5268 2024-04-03 06:23:38.221076 almirah-0.2.0/almirah/data/configs/bids.yaml
+-rw-r--r--   0        0        0     8102 2024-04-03 06:23:38.221076 almirah-0.2.0/almirah/data/convert.py
+-rw-r--r--   0        0        0     4646 2024-04-03 06:23:38.221076 almirah-0.2.0/almirah/data/dataset.py
+-rw-r--r--   0        0        0     3784 2024-04-03 06:23:38.221076 almirah-0.2.0/almirah/data/indexer.py
+-rw-r--r--   0        0        0     6854 2024-04-03 06:23:38.221076 almirah-0.2.0/almirah/data/layout.py
+-rw-r--r--   0        0        0     1448 2024-04-03 06:23:38.221076 almirah-0.2.0/almirah/data/report.py
+-rw-r--r--   0        0        0    12226 2024-04-03 06:23:38.221076 almirah-0.2.0/almirah/data/specification.py
+-rw-r--r--   0        0        0    18868 2024-04-03 06:23:38.221076 almirah-0.2.0/almirah/db.py
+-rw-r--r--   0        0        0     3830 2024-04-03 06:23:38.221076 almirah-0.2.0/almirah/utils.py
+-rw-r--r--   0        0        0     1120 2024-04-03 06:23:38.225076 almirah-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     1646 1970-01-01 00:00:00.000000 almirah-0.2.0/PKG-INFO
```

### Comparing `almirah-0.1.0/LICENSE` & `almirah-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `almirah-0.1.0/README.md` & `almirah-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `almirah-0.1.0/almirah/data/configs/bids.yaml` & `almirah-0.2.0/almirah/data/configs/bids.yaml`

 * *Files 8% similar despite different names*

```diff
@@ -21,32 +21,48 @@
   - name: datatype
     pattern: "(?:(?<!sourcedata))[/\\\\]+(anat|dwi|eeg|eyetrack|fmap|func|nirs|genome)[/\\\\]+"
   - name: sourcetype
     pattern: "sourcedata/(eeg|eyetrack|mri|nirs|genome)"
   - name: pipeline
     pattern: "derivatives/([a-zA-Z0-9]+)"
 path_patterns:
+
+# mri source data path patterns
   - "sourcedata/{sourcetype<mri>|mri}/sub-{subject}[/ses-{session}]/sub-{subject}[_ses-{session}][_task-{task}][_acq-{acquisition}][_run-{run}]_{suffix<mri>|mri}{extension<.dcm>}"
-  - "sourcedata/{sourcetype<eeg>|eeg}/sub-{subject}[/ses-{session}]/sub-{subject}[_ses-{session}]_task-{task}[_acq-{acquisition}][_run-{run}]_{suffix<eeg>|eeg}{extension<.bdf|.cnt|.data|.edf|.gdf|.mat|.mff|.nxe|.set|.vhdr|.vmrk>}"  
+
+# eeg source data path patterns
+  - "sourcedata/{sourcetype<eeg>|eeg}/sub-{subject}[/ses-{session}]/sub-{subject}[_ses-{session}]_task-{task}[_acq-{acquisition}][_run-{run}]_{suffix<eeg>|eeg}{extension<.bdf|.cnt|.data|.edf|.gdf|.mat|.mff|.nxe|.set|.vhdr|.vmrk>}"
+
+# nirs source data path patterns
   - "sourcedata/{sourcetype<nirs>|nirs}/sub-{subject}[/ses-{session}]/sub-{subject}[_ses-{session}]_task-{task}[_acq-{acquisition}][_run-{run}]_{suffix<nirs>|nirs}{extension<.nirx>}"
+
+# eye track source data path patterns
   - "sourcedata/{sourcetype<eyetrack>|eyetrack}/sub-{subject}[/ses-{session}]/sub-{subject}[_ses-{session}]_task-{task}[_acq-{acquisition}][_run-{run}]_{suffix<eyetrack>|eyetrack}{extension<.edf|.dat|.log>}"
+
+# mri path patterns
   - "sub-{subject}[/ses-{session}]/{datatype<anat>|anat}/sub-{subject}[_ses-{session}][_task-{task}][_acq-{acquisition}][_run-{run}]_{suffix<T1w|T2w|FLAIR>}{extension<.nii|.nii.gz|.json>|.nii.gz}"
   - "sub-{subject}[/ses-{session}]/{datatype<func>|func}/sub-{subject}[_ses-{session}]_task-{task}[_acq-{acquisition}][_dir-{direction}][_run-{run}]_{suffix<bold>}{extension<.nii|.nii.gz|.json>|.nii.gz}"
   - "sub-{subject}[/ses-{session}]/{datatype<dwi>|dwi}/sub-{subject}[_ses-{session}][_acq-{acquisition}]{suffix<dwi>}{extension<.bval|.bvec|.json|.nii.gz|.nii>|.nii.gz}"
   - "sub-{subject}[/ses-{session}]/{datatype<fmap>|fmap}/sub-{subject}[_ses-{session}][_acq-{acquisition}][_dir-{direction}][_run-{run}]_{suffix<phasediff|magnitude1|magnitude2|phase1|phase2|fieldmap>}{extension<.nii|.nii.gz|.json>|.nii.gz}"
   - "sub-{subject}[/ses-{session}]/{datatype<fmap>|fmap}/sub-{subject}[_ses-{session}][_acq-{acquisition}]_dir-{direction}[_run-{run}]_{suffix<epi>}{extension<.nii|.nii.gz|.json>|.nii.gz}"
+
+# eeg path patterns
   - "sub-{subject}[/ses-{session}]/{datatype<eeg>|eeg}/sub-{subject}[_ses-{session}]_task-{task}[_acq-{acquisition}][_run-{run}]_{suffix<eeg>}{extension<.edf|.vhdr|.vmrk|.eeg|.set|.fdt|.bdf|.json>}"
   - "sub-{subject}[/ses-{session}]/{datatype<eeg>}/sub-{subject}[_ses-{session}]_task-{task}[_acq-{acquisition}][_run-{run}]_{suffix<channels|events>}{extension<.tsv|.json>|.tsv}"
   - "sub-{subject}[/ses-{session}]/{datatype<eeg>}/sub-{subject}[_ses-{session}][_acq-{acquisition}][_space-{space}]_{suffix<coordsystem>}{extension<.json>|.json}"
   - "sub-{subject}[/ses-{session}]/{datatype<eeg>}/sub-{subject}[_ses-{session}][_acq-{acquisition}][_space-{space}]_{suffix<electrodes>}{extension<.tsv|.json>|.tsv}"
   - "sub-{subject}[/ses-{session}]/{datatype<eeg>}/sub-{subject}[_ses-{session}][_acq-{acquisition}]_{suffix<photo>|photo}{extension<.jpg>}"
-  - "sub-{subject}[/ses-{session}]/{datatype<eeg>|eeg}/sub-{subject}[_ses-{session}]_task-{task}[_acq-{acquisition}][_run-{run}]_{suffix<physio>}{extension<.tsv.gz|.json>}"  
+  - "sub-{subject}[/ses-{session}]/{datatype<eeg>|eeg}/sub-{subject}[_ses-{session}]_task-{task}[_acq-{acquisition}][_run-{run}]_{suffix<physio>}{extension<.tsv.gz|.json>}"
+
+# nirs path patterns
   - "sub-{subject}[/ses-{session}]/{datatype<nirs>|nirs}/sub-{subject}[_ses-{session}]_task-{task}[_acq-{acquisition}][_run-{run}]_{suffix<nirs>}{extension<.snirf|.json>}"
   - "sub-{subject}[/ses-{session}]/{datatype<nirs>|nirs}/sub-{subject}[_ses-{session}]_task-{task}[_acq-{acquisition}][_run-{run}]_{suffix<events|channels>}{extension<.tsv|.json>}"
   - "sub-{subject}[/ses-{session}]/{datatype<nirs>|nirs}/sub-{subject}[_ses-{session}][_acq-{acquisition}]_{suffix<optodes>}{extension<.tsv|.json>}"
   - "sub-{subject}[/ses-{session}]/{datatype<nirs>|nirs}/sub-{subject}[_ses-{session}][_acq-{acquisition}]_{suffix<coordsystem>}{extension<.json>}"
+
+# eye track path patterns
   - "sub-{subject}[/ses-{session}]/{datatype<eyetrack>|eyetrack}/sub-{subject}[_ses-{session}]_task-{task}[_acq-{acquisition}][_run-{run}]_{suffix<eyetrack>}{extension<.asc>}"
   - "sub-{subject}[/ses-{session}]/{datatype<eyetrack>|eyetrack}/sub-{subject}[_ses-{session}]_task-{task}[_acq-{acquisition}][_run-{run}]_{suffix<events>}{extension<.tsv|.json>}"
+
+# genome path patterns
   - "sub-{subject}[/ses-{session}]/{datatype<genome>|genome}/sub-{subject}[_ses-{session}]_sample-{sample}[_acq-{acquisition}]_{suffix<exome>|exome}{extension<.bam>}"
   - "sub-{subject}[/ses-{session}]/{datatype<genome>|genome}/sub-{subject}[_ses-{session}]_sample-{sample}[_acq-{acquisition}]_{suffix<annotated>|annotated}{extension<.vcf|.txt>}"
-  - "{suffix}{extension}"
-  - "derivatives/{pipeline}"
```

### Comparing `almirah-0.1.0/almirah/data/convert.py` & `almirah-0.2.0/almirah/data/convert.py`

 * *Files 6% similar despite different names*

```diff
@@ -122,14 +122,15 @@
 
 
 def nirs_conv(files, out, dst, **kwargs):
     """Convert NIRS data format and write to disk."""
 
     for file in files:
         raw = mne.io.read_raw_nirx(file.path)
+        raw.anonymize(**kwargs.get("anonymize", {}))
         new_path = os.path.join(
             dst,
             file.build_modified_path(
                 extension="snirf",
                 sourcetype=None,
             ),
         )
```

### Comparing `almirah-0.1.0/almirah/data/dataset.py` & `almirah-0.2.0/almirah/data/dataset.py`

 * *Files identical despite different names*

### Comparing `almirah-0.1.0/almirah/data/indexer.py` & `almirah-0.2.0/almirah/data/indexer.py`

 * *Files identical despite different names*

### Comparing `almirah-0.1.0/almirah/data/layout.py` & `almirah-0.2.0/almirah/data/layout.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,12 @@
 """Model classes to represent layouts and its components."""
 
 import os
 import logging
 
-from datalad import api
-
 from typing import List
 from typing import Dict
 
 from sqlalchemy import inspect
 from sqlalchemy import ForeignKey
 from sqlalchemy.orm import Mapped
 from sqlalchemy.orm import relationship
@@ -93,19 +91,22 @@
     def build_path(self):
         """Build path based on tags associated with file."""
         t = self.get_tags()
         return self.layout.spec.build_path(t)
 
     def build_modified_path(self, **changes):
         "Returns the path for file given changes to tags."
-        t = self.get_tags().update(changes)
-        return self.layout.spec.build_path(t)
+        tags = self.get_tags()
+        tags.update(changes)
+        return self.layout.spec.build_path(tags)
 
     def get(self):
         """Get file from remote dataset."""
+        from datalad import api
+
         api.get(self.path, dataset=self.root)
 
     def get_tags(self):
         """Returns tags associated with the file."""
         return {n: t.value for n, t in self.tags.items()}
 
     def __repr__(self):
@@ -214,16 +215,19 @@
         if reindex or not inspect(layout).persistent:
             layout.reindex(valid_only)
 
         return layout
 
     def clone_from_url(self):
         """Clone layout from a datalad url."""
-        logging.info(f"Cloning layout from {self.url}")
+
+        from datalad import api
+
         api.clone(source=self.url, path=self.root)
+        logging.info(f"Cloning layout from {self.url}")
 
     def get_files(self, **filters):
         """Return files that match criteria."""
         files_filter = self.indexer._files_filter(self.root, **filters)
         files = self.indexer.run_query(files_filter)
         return files
```

### Comparing `almirah-0.1.0/almirah/data/report.py` & `almirah-0.2.0/almirah/data/report.py`

 * *Files identical despite different names*

### Comparing `almirah-0.1.0/almirah/data/specification.py` & `almirah-0.2.0/almirah/data/specification.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,17 +7,15 @@
 
 import pandas as pd
 from string import Formatter
 
 from .. import utils
 
 
-_TAG_PATTERN = re.compile(
-    r"({([\w\d]*?)(?:<([^>]+)>)?(?:\|((?:\.?[\w])+))?\})",
-)
+_TAG_PATTERN = re.compile(r"({([\w\d]*?)(?:<([^>]+)>)?(?:\|((?:\.?[\w])+))?\})")
 
 __all__ = ["Specification"]
 
 
 class Specification:
     """Representation of the specification used.
 
@@ -59,26 +57,32 @@
     def validate(self, path):
         """Returns True if path is valid."""
         tags = self.extract_tags(path)
         if self.build_path(tags) == path:
             return True
         return False
 
-    def build_path(self, tags):
+    def build_path(self, tags, strict=False):
         """Construct path provided a set of tags.
 
         Parameters
         ----------
         tags : dict
             A dictionary with tag name, value pairs.
 
+        strict : bool
+            If True, the tags provided should exactly match the
+            requirements. If False, extra tags are ignored and the
+            first matching path is built.
+
         Returns
         -------
         path : str
             The constructed path if successful, else `None`.
+
         """
 
         path_patterns = self.spec.get("path_patterns")
         logging.debug(f"Building path with tags : {tags}")
 
         # Remove none values
         tags = {k: v for k, v in tags.items() if v or v == 0}
@@ -88,39 +92,34 @@
             ext = tags.get("extension")
             tags["extension"] = ext if ext.startswith(".") else "." + ext
 
         # Attempt to match pattern with tags and return first match
         for pattern in path_patterns:
             path = pattern
             matches = _TAG_PATTERN.findall(pattern)
-            tags_defined = [t[1] for t in matches]
 
             # Do not tamper with tags provided so that
             # it can be used for other patterns
             tags_copy = tags.copy()
 
-            # Skip if all tags not matched
-            if set(tags_copy.keys()) - set(tags_defined):
+            # Skip if strict set and all tags not matched
+            if strict and set(tags_copy.keys()) - set([t[1] for t in matches]):
                 continue
 
             # Validate and fill in missing tags with default
-            for subpattern, name, valid, default in matches:
-                valid_expanded = [v for v in valid.split("|")]
+            for subpattern, name, valid_vals, default in matches:
+                valid = [v for v in valid_vals.split("|")]
 
-                if (
-                    valid_expanded
-                    and name in tags_copy
-                    and tags_copy[name] not in valid_expanded
-                ):
+                if valid and name in tags_copy and tags_copy[name] not in valid:
                     continue
 
                 if name not in tags_copy and default:
                     tags_copy[name] = default
 
-                if valid_expanded and default and default not in valid_expanded:
+                if valid and default and default not in valid:
                     warnings.warn(
                         f"Pattern {subpattern} is inconsistent as it defines an invalid default value"
                     )
 
                 # Simplify path
                 path = path.replace(subpattern, "{%s}" % name)
 
@@ -165,28 +164,23 @@
         for mandatory_key in [
             "source",
             "destination",
             "pattern",
             "tag_rules",
         ]:
             if mandatory_key not in rules:
-                raise KeyError(f"Expected '{mandatory_key}' in rule.")
+                raise KeyError(f"Expected '{mandatory_key}' key in rule.")
 
         source = rules.get("source")
         destination = rules.get("destination")
         logging.info(f"Initiating organization of {source} -> {destination}")
 
-        map_ = rules.get("map")
-        if map_:
-            mapping = pd.read_csv(map_, dtype=str)
-            logging.info(f"File {map_} will be used for mapping tag values")
-
         overwrite = rules.get("overwrite", False)
         if overwrite:
-            logging.warning("If found, existing files will be overwritten")
+            logging.warning("Overwrite set: Existing files may be overwritten")
 
         add = rules.get("add", None)
         for a in add or []:
             logging.info(f"File {a['path']} will be added as {a['position']}.")
 
         logging.debug(f"Matching contents with pattern {rules.get('pattern')}")
 
@@ -206,15 +200,15 @@
                 if "value" in rule:
                     val = rule.get("value")
                     tags[tag_name] = val
                     logging.debug(f"Setting tag with {val}")
                 else:
                     match = re.findall(rule.get("pattern"), file)
                     if match and len(match) != 1:
-                        logging.error("Expected single match, more found.")
+                        logging.warning("Expected single match, found more.")
 
                     # Choose last match always
                     val = match[-1] if match else None
                     logging.debug(f"Matching with pattern yields {val}")
 
                     if "prepend" in rule and val:
                         val = "".join([str(rule.get("prepend")), val])
@@ -232,30 +226,49 @@
                     if c := rule.get("case") in ["lower", "upper"] and val:
                         val = val.lower() if c == "lower" else val.upper()
 
                     if "default" in rule and not val:
                         val = rule.get("default")
                         logging.debug(f"Using default value of {val} for tag")
 
-                    if "from" in rule and val:
-                        from_, to = rule.get("from"), rule.get("to")
+                    if "padding" in rule and val:
+                        pad = rule.get("padding")
 
-                        if not to or not map_:
-                            raise KeyError("Expected to and map if from found")
+                        # Set defaults
+                        direction = (pad.get("direction", "left"),)
+                        char = (pad.get("char", "0"),)
+                        length = pad["length"]
+
+                        if direction == "left":
+                            val.rjust(length, char)
+
+                        elif direction == "right":
+                            val.ljust(length, char)
+
+                    if "replace" in rule and val:
+                        rep = rule.get("replace")
+                        col, with_, from_ = [rep[x] for x in ["col", "with", "from"]]
+                        logging.info(f"File {from_} will be used to map tag values")
+                        mapping = pd.read_csv(from_, dtype=str)
 
-                        m = mapping.where(mapping[from_] == val).dropna()
+                        # TODO: Modularize below code snippet
+                        m = mapping.where(mapping[col] == val).dropna()
+
+                        if len(m) == 0:
+                            logging.error(f"No mapping found for {val}")
+                            continue
 
-                        if len(m) != 1:
-                            logging.error(f"Expected unique map for {val}")
+                        if len(m) > 1:
+                            logging.error(f"Expected unique map for {val}, found many")
                             continue
 
-                        val = m[to].values[0]
+                        val = m[with_].values[0]
 
                     if not val:
-                        logging.error(f"Value for tag {tag_name} not found.")
+                        logging.error(f"Value for {tag_name} tag not found in {file}.")
 
                 logging.info(f"File marked with {tag_name}:{val} tag")
                 tags.update({tag_name: val})
 
             # Warning, clunky code ahead. To be made better
             rel_path = self.build_path(tags)
             if not rel_path:
@@ -306,20 +319,19 @@
                         tag_val = rule.get("suffix")
                         tags_copy.update({"suffix": tag_val})
                         logging.info(f"File marked with suffix:{tag_val} tag")
 
                 # Copy fellow files
                 rel_path = self.build_path(tags_copy)
                 if not rel_path:
-                    logging.info("Unable to build destination path for file")
+                    logging.error(f"Unable to build destination path for file {file}")
                     continue
                 new_path = os.path.join(rules.get("destination"), rel_path)
                 logging.info(f"Target destination path is {new_path}")
                 utils.copy(fellow, new_path, overwrite)
-                logging.info("Moved file to target")
 
     def __repr__(self):
         return f"<Specification name={self.name}>"
 
 
 def get_spec(path=None, name=None):
     if not path:
```

### Comparing `almirah-0.1.0/almirah/db.py` & `almirah-0.2.0/almirah/db.py`

 * *Files 6% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 from sqlalchemy.types import Integer
 from sqlalchemy.types import String
 from sqlalchemy.types import DateTime
 
 from sqlalchemy import create_engine
 from sqlalchemy.orm import sessionmaker
 
-from . import utils
+from .utils import get_dtype, log_df, log_col
 
 __all__ = ["DBManager", "common_records", "migrate", "transform", "validate"]
 
 
 class DBManager:
     """Interface to connect with db and perform operations."""
 
@@ -86,15 +86,15 @@
             "boolean": Boolean,
             "datetime": DateTime,
             "float": Float,
             "integer": Integer,
             "str": String,
         }
 
-        dtype, length = utils.get_dtype(dtype, default_length)
+        dtype, length = get_dtype(dtype, default_length)
         stype = SQL_TYPE_EQUIVALENT[dtype]
 
         return stype(length) if length else stype()
 
     def get_table(self, table, cols=None):
         """
         Retrieve table records in db as a DataFrame.
@@ -256,15 +256,15 @@
         Raises
         ------
         ValueError
             When primary key duplicates are found and `resolve` is True.
 
         """
         dups = df.duplicated(self.get_primary(table), resolve)
-        utils.log_df(df[dups], "Found duplicate records: \n {df}")
+        log_df(df[dups], "Found duplicate records")
         return ~dups
 
     def resolve_fks(self, df, table, resolve=False):
         """
         Parameters
         ----------
         df : pandas.DataFrame
@@ -291,15 +291,15 @@
         mask = pd.Series(True, index=df.index)
 
         for fkc in self.meta.tables[table].foreign_key_constraints:
             p_cols = [fk.column.name for fk in fkc.elements]
             p_df = self.get_table(fkc.referred_table.name, p_cols)
             p_mask = common_records(df, p_df, fkc.column_keys, p_cols)
 
-            utils.log_df(df[~p_mask], "Missing parent records: \n {df}")
+            log_df(df[~p_mask], "Missing parent records")
 
             if not p_mask.all() and resolve:
                 logging.info("Resolving missing records by insert to parent")
                 self.to_table(
                     df[~p_mask][fkc.column_keys].set_axis(p_cols, axis=1),
                     fkc.referred_table.name,
                     check_dups=True,
@@ -339,14 +339,20 @@
         )
         .replace({"both": True, "left_only": False, "right_only": False})
         .set_index("index")["exists"]
         .astype("bool")
     )
 
 
+def check_for_key(key, mapping):
+    """Return columns in table mapping which contain the key provided."""
+
+    return [c["name"] for c in mapping["cols"] if key in c.keys()]
+
+
 def migrate(
     src,
     target,
     mapping,
     dry_run=False,
     na_vals=[],
     dtype_kws=None,
@@ -386,47 +392,35 @@
         Other keyword arguments are passed down to
         :meth:`napi.db.to_table`.
     """
 
     s = DBManager(src)
     t = DBManager(target)
 
-    na_vals = ["", "None", "NONE", "NA", "N/A", "<NA>", "Not applicable"] + na_vals
+    na = ["", "None", "NONE", "NA", "N/A", "<NA>", "Not applicable"] + na_vals
 
     for m in mapping:
         logging.info(f"Transferring table {m['maps']} -> {m['table']}")
 
         # Extract source records
-        src_df = s.get_table(m["maps"])
-        src_df = src_df.replace(na_vals, pd.NA)
-        tar_df = pd.DataFrame(index=src_df.index)
+        records = s.get_table(m["maps"]).replace(na, pd.NA)
 
         # Transform and validate
-        tr_error = pd.Series(False, index=src_df.index)
-        mask = pd.Series(True, index=src_df.index)
-
-        for col in m["cols"] + m.get("detach", []):
-            name, maps = col["name"], col["maps"]
-            logging.debug(f"Transforming and validating column {name}")
-            tar_df[name], err = transform(src_df[maps], dtype_kws, **col)
-            mask &= validate(tar_df[name], **col)
-            tr_error |= err
-
-        utils.log_df(src_df[tr_error], "Unable to transform records: \n {df}")
-        utils.log_df(src_df[~mask], "Found invalid records: \n {df}")
+        records = transform(records, dtype_kws, m)
+        mask = validate(records, m)
 
         # Reshape data records
-        tar_df = reshape(tar_df[mask & ~tr_error], m.get("reshape", dict()))
+        df = reshape(records[mask], m.get("reshape", dict()))
 
         if dry_run:
             continue
 
         # Load records into target
         t.create_table(m["table"], m["cols"] + m.get("attach", []), m.get("refs", []))
-        t.to_table(tar_df, m["table"], threshold=m.get("threshold"), **kwargs)
+        t.to_table(df, m["table"], threshold=m.get("threshold"), **kwargs)
 
 
 def set_dtype(series, dtype, **kwargs):
     """
     Set dtype of series.
 
     Parameters
@@ -438,25 +432,25 @@
         Supported dtype to which the series will be converted.
 
     kwargs: key, value mappings
         Other keyword arguments are passed down to `pandas.to_datetime()`_
         if the dtype is 'datetime'.
     """
 
-    dtype, _ = utils.get_dtype(dtype)
+    dtype, _ = get_dtype(dtype)
 
-    if dtype == "datetime":
+    if dtype == str:
+        series = series.astype(dtype)
+
+    elif dtype == "datetime":
         series = pd.to_datetime(series, errors="coerce", **kwargs)
 
     elif dtype in {"float", "integer"}:
         series = pd.to_numeric(series, errors="coerce", downcast=dtype)
 
-    elif dtype == str:
-        series = series.astype(dtype)
-
     elif dtype == "boolean":
         series = series.replace(
             {
                 "1": True,
                 "0": False,
                 "True": True,
                 "False": False,
@@ -465,72 +459,148 @@
             }
         )
         series = series.astype(dtype)
 
     return series.convert_dtypes()
 
 
-def reshape(df, steps):
-    """Reshape a dataframe into appropriate shape."""
+def reshape(records, steps):
+    """Reshape table records into appropriate shape."""
 
     for procedure in steps:
         [(p, k)] = procedure.items()
 
         if p == "add":
-            df[k["name"]] = k["value"]
+            records[k["name"]] = k["value"]
 
         if p == "split":
-            df[k["rename"]] = df[k["name"]].str.split(k["pat"], expand=True)
+            records[k["rename"]] = records[k["name"]].str.split(k["pat"], expand=True)
 
         if p == "melt":
-            df = df.melt(**k)
+            records = records.melt(**k)
 
         if p == "pivot":
-            df = df.pivot_table(**k).reset_index()
+            records = records.pivot_table(**k).reset_index()
+
+    return records
+
+
+def transform(records, dtype_kws, mapping):
+    """Transform table records into appropriate format."""
+
+    df = pd.DataFrame(index=records.index)
+    to_hide = check_for_key("hide", mapping)
+    error = pd.Series(False, index=records.index)
+
+    for col in mapping["cols"] + mapping.get("detach", []):
+        name, maps = col["name"], col["maps"]
+        logging.debug(f"Transforming column {name}")
+        df[name], col_error = transform_column(records[maps], dtype_kws, **col)
+        error |= col_error
+
+    log_df(records[error], "Error transforming records", hide=to_hide)
+    return df[~error]
+
+
+def replace_value(value, field, using, file):
+    # Get mapping
+    mapping = pd.read_csv(file, dtype=str)
 
-    return df
+    # Find value to replace
+    result = mapping.query("`%s` == @value" % field)
 
+    if len(result) == 0:
+        logging.error(f"Value '{value}' not found in field '{field}' of file '{file}'.")
+        return
 
-def transform(series, dtype_kws=None, **kwargs):
-    """Transform series and return with appropriate datatype."""
+    if len(result) > 1:
+        logging.error(f"Non-unique mappings for value '{value}' in file {file}")
+        return
 
-    s = series.copy(deep=True)
+    return result.at[0, using]
+
+
+def replace_column(series, field, using, file, strict=True):
+    # Load mapping from file
+    mapping = pd.read_csv(file, dtype=str)
+    logging.info(f"Replacing values in '{field}' with '{using}' from {file}")
+
+    # Stop if non-unique mappings
+    if mapping.duplicated([field]).any():
+        raise ValueError(f"Non-unique mappings found in file {file}")
+
+    mapping = pd.Series(mapping[using], index=mapping[field])
+    replaced = series.map(mapping)
+
+    # Retain original value if replacement not strict
+    if not strict:
+        replaced.fillna(series, inplace=True)
+
+    return replaced
+
+
+def transform_column(series, dtype_kws=dict(), **kwargs):
+    """Transform column to appropriate datatype."""
+
+    hide = kwargs.get("hide", False)
+    s, error = series.copy(deep=True), series.isna()
 
     if pat := kwargs.get("extract"):
         s = s.astype(str).str.extract(pat, expand=False)
+        logging.info(f"Extracting and replacing based on pattern {pat}")
 
     if rep := kwargs.get("replace"):
-        s = s.replace({k["value"]: k["with"] for k in rep})
+        if "field" in rep:
+            replace_column(s, **rep)
+            logging.info("Replacing values with mapping in external file")
+        else:
+            s = s.replace({k["value"]: k["with"] for k in rep})
+            logging.info("Replacing values with given in config")
 
     if ca := kwargs.get("case"):
         s = s.str.upper() if ca == "upper" else s.str.lower()
-
-    if not dtype_kws:
-        dtype_kws = dict()
+        logging.info(f"Changing case to {ca}")
 
     s = set_dtype(s, kwargs["dtype"], **dtype_kws)
-
     error = series.notna() & s.isna()
-    utils.log_df(series[error], "Bad transform: \n{df}", level=logging.DEBUG)
+    log_col(series[error], f"Error transforming values to {kwargs['dtype']}", hide=hide)
 
     return s, error
 
 
-def validate(series, **kwargs):
-    """Validate series and return mask."""
+def validate(records, mapping):
+    """Validate table records and return mask where True means valid."""
+
+    to_hide = check_for_key("hide", mapping)
+    mask = pd.Series(True, index=records.index)
+
+    for col in mapping["cols"] + mapping.get("detach", []):
+        logging.debug(f"Validating column {col['name']}")
+        mask &= validate_column(records[col["name"]], **col)
+
+    log_df(records[~mask], "Found invalid records", hide=to_hide)
+    return mask
+
+
+def validate_column(series, **kwargs):
+    """Validate column and return mask where True means valid."""
 
+    hide = kwargs.get("hide", False)
     mask = pd.Series(True, index=series.index)
 
     if kwargs.get("primary"):
-        mask &= series.notna()
+        mask &= (m := series.notna())
+        log_col(series[~m], "Primary column values cannot be NA", hide=hide)
 
     if pat := kwargs.get("like"):
-        mask &= series.astype(str).str.fullmatch(pat) | series.isna()
+        mask &= (m := series.astype(str).str.fullmatch(pat) | series.isna())
+        log_col(series[~m], f"Values do not match pattern {pat}", hide=hide)
 
     if bounds := kwargs.get("between"):
-        mask &= series.between(*bounds) | series.isna()
+        mask &= (m := series.between(*bounds) | series.isna())
+        log_col(series[~m], f"Values not between bounds {bounds}", hide=hide)
 
     if members := kwargs.get("in"):
-        mask &= series.isin(members) | series.isna()
+        mask &= (m := series.isin(members) | series.isna())
+        log_col(series[~m], f"Values not in {members}", hide=hide)
 
-    utils.log_df(series[~mask], "Bad validation: \n{df}", level=logging.DEBUG)
     return mask
```

### Comparing `almirah-0.1.0/almirah/utils.py` & `almirah-0.2.0/almirah/utils.py`

 * *Files 12% similar despite different names*

```diff
@@ -14,21 +14,22 @@
 def copy(src, dst, overwrite=False):
     """Copies from source to destination."""
     if not dst:
         raise TypeError("Expected destination path, received None")
 
     if os.path.exists(dst):
         if not overwrite:
-            logging.warning("Skipping copy as file exists")
+            logging.error(f"Skipping copy of {src} to {dst} as file exists")
             return
         if overwrite:
-            logging.warning("Overwriting existing file")
+            logging.warning(f"Overwriting and copying {src} to {dst}")
             remover = shutil.rmtree if os.path.isdir(dst) else os.remove
             remover(dst)
 
+    logging.debug(f"Initiating copy of {src} to {dst}")
     os.makedirs(os.path.dirname(dst), exist_ok=True)
     copier = shutil.copytree if os.path.isdir(src) else shutil.copy2
     copier(src, dst)
 
 
 def get_dir_contents(root, pattern, skip=None):
     """Return list of contents in a directory that match pattern."""
@@ -66,34 +67,49 @@
 
 def run_shell(cmd, suppress_output=True):
     """Execute shell command in background."""
     sp = subprocess.run(cmd, shell=True)
     return sp
 
 
-def log_df(df, msg, level=logging.ERROR, **kwargs):
+def log_df(df, msg, hide=list(), level=logging.ERROR, **kwargs):
     """
     Log df records with a message.
 
     Parameters
     ----------
     df: pandas.DataFrame
         DataFrame to be logged.
 
     msg: str
         Log message compatible with string formatting.
 
+    hide: list-like or scalar, optional
+        Sensitive column or columns to hide.
+
     level: int, optional
         Logging level to use. Accepts logging.LEVEL values.
 
     kwargs: key, value mappings
         Other keyword arguments are passed to `str.format()`.
     """
+
     if not df.empty:
-        logging.log(level, msg.format(df=df.to_string(), **kwargs))
+        logging.log(level, msg + "\n%s", df.drop(columns=hide).to_string(), **kwargs)
+
+
+def log_col(series, msg, hide=False, level=logging.ERROR, **kwargs):
+    """Log column values with a message."""
+
+    if hide:
+        series = series.index.to_series()
+        logging.info("Column values will not be displayed as hide set")
+
+    if not series.empty:
+        logging.log(level, msg + "\n%s", series.to_string(), **kwargs)
 
 
 def get_dtype(dtype, default_length=250):
     """Returns supported dtype and length from provided dtype string."""
 
     SUPPORTED_DTYPES = {"boolean", "datetime", "float", "integer", "str"}
```

### Comparing `almirah-0.1.0/pyproject.toml` & `almirah-0.2.0/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "almirah"
-version = "0.1.0"
+version = "0.2.0"
 description = "a wardrobe for datasets"
 authors = ["girish <girishmm@ncbs.res.in>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
@@ -31,14 +31,17 @@
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.4.0"
 furo = "^2023.9.10"
 towncrier = "^23.6.0"
 sphinx-copybutton = "^0.5.2"
 sphinx-autobuild = "^2021.3.14"
 
+[tool.poetry.group.mariadb.dependencies]
+pymysql = "^1.1.0"
+
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.towncrier]
 package = "almirah"
 package_dir = "almirah"
```

### Comparing `almirah-0.1.0/PKG-INFO` & `almirah-0.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: almirah
-Version: 0.1.0
+Version: 0.2.0
 Summary: a wardrobe for datasets
 License: MIT
 Author: girish
 Author-email: girishmm@ncbs.res.in
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: almirah Version: 0.1.0 Summary: a wardrobe for
+Metadata-Version: 2.1 Name: almirah Version: 0.2.0 Summary: a wardrobe for
 datasets License: MIT Author: girish Author-email: girishmm@ncbs.res.in
 Requires-Python: >=3.9,<4.0 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11 Classifier: Programming
 Language :: Python :: 3.12 Requires-Dist: datalad (>=0.19.3,<0.20.0) Requires-
 Dist: pandas (>=2.1.4,<3.0.0) Requires-Dist: pyyaml (>=6.0.1,<7.0.0) Requires-
```

