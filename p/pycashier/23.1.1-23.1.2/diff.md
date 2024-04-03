# Comparing `tmp/pycashier-23.1.1.tar.gz` & `tmp/pycashier-23.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pycashier-23.1.1.tar", last modified: Thu Jan  5 18:28:05 2023, max compression
+gzip compressed data, was "pycashier-23.1.2.tar", last modified: Sat Jan  7 17:00:31 2023, max compression
```

## Comparing `pycashier-23.1.1.tar` & `pycashier-23.1.2.tar`

### file list

```diff
@@ -1,28 +1,28 @@
--rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-01-05 18:27:55.324644 pycashier-23.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     9691 2023-01-05 18:27:55.324644 pycashier-23.1.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-05 18:27:55.336644 pycashier-23.1.1/pycashier/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2235 2023-01-05 18:27:55.336644 pycashier-23.1.1/pycashier/_checks.py
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-01-05 18:27:55.336644 pycashier-23.1.1/pycashier/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     4299 2023-01-05 18:27:55.336644 pycashier-23.1.1/pycashier/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     1563 2023-01-05 18:27:55.336644 pycashier-23.1.1/pycashier/cluster.py
--rw-r--r--   0 runner    (1001) docker     (123)     3022 2023-01-05 18:27:55.336644 pycashier-23.1.1/pycashier/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     2935 2023-01-05 18:27:55.336644 pycashier-23.1.1/pycashier/extract.py
--rw-r--r--   0 runner    (1001) docker     (123)     4273 2023-01-05 18:27:55.336644 pycashier-23.1.1/pycashier/merge.py
--rw-r--r--   0 runner    (1001) docker     (123)    11212 2023-01-05 18:27:55.336644 pycashier-23.1.1/pycashier/options.py
--rw-r--r--   0 runner    (1001) docker     (123)     4943 2023-01-05 18:27:55.336644 pycashier-23.1.1/pycashier/pycashier.py
--rw-r--r--   0 runner    (1001) docker     (123)     3128 2023-01-05 18:27:55.336644 pycashier-23.1.1/pycashier/read_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     7553 2023-01-05 18:27:55.336644 pycashier-23.1.1/pycashier/single_cell.py
--rw-r--r--   0 runner    (1001) docker     (123)     2925 2023-01-05 18:27:55.336644 pycashier-23.1.1/pycashier/term.py
--rw-r--r--   0 runner    (1001) docker     (123)     7897 2023-01-05 18:27:55.336644 pycashier-23.1.1/pycashier/termui.py
--rw-r--r--   0 runner    (1001) docker     (123)     3302 2023-01-05 18:27:55.336644 pycashier-23.1.1/pycashier/trim.py
--rw-r--r--   0 runner    (1001) docker     (123)     8826 2023-01-05 18:27:55.336644 pycashier-23.1.1/pycashier/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-01-05 18:27:55.336644 pycashier-23.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)    62389 2023-01-05 18:27:55.336644 pycashier-23.1.1/tests/data/reference/mergedfastqs/test.merged.raw.fastq
--rw-r--r--   0 runner    (1001) docker     (123)     1960 2023-01-05 18:27:55.336644 pycashier-23.1.1/tests/data/reference/outs/test.q30.barcodes.r3d1.min0_off1.tsv
--rw-r--r--   0 runner    (1001) docker     (123)      445 2023-01-05 18:27:55.336644 pycashier-23.1.1/tests/data/reference/outs-scrna/test.cell_record_labeled.barcode.tsv
--rw-r--r--   0 runner    (1001) docker     (123)     5660 2023-01-05 18:27:55.340644 pycashier-23.1.1/tests/data/reference/rawfastqgzs/test.fastq.gz
--rw-r--r--   0 runner    (1001) docker     (123)   427534 2023-01-05 18:27:55.340644 pycashier-23.1.1/tests/data/reference/sams/test.sam
--rw-r--r--   0 runner    (1001) docker     (123)     7121 2023-01-05 18:27:55.340644 pycashier-23.1.1/tests/data/reference/unmergedfastqgzs/test.R1.raw.fastq.gz
--rw-r--r--   0 runner    (1001) docker     (123)     8577 2023-01-05 18:27:55.340644 pycashier-23.1.1/tests/data/reference/unmergedfastqgzs/test.R2.raw.fastq.gz
--rw-r--r--   0 runner    (1001) docker     (123)     2310 2023-01-05 18:27:55.340644 pycashier-23.1.1/tests/test_pycashier.py
--rw-------   0 runner    (1001) docker     (123)     9989 2023-01-05 18:28:05.988706 pycashier-23.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-01-07 17:00:21.395537 pycashier-23.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     9697 2023-01-07 17:00:21.395537 pycashier-23.1.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-07 17:00:21.403538 pycashier-23.1.2/pycashier/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2235 2023-01-07 17:00:21.403538 pycashier-23.1.2/pycashier/_checks.py
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-01-07 17:00:21.403538 pycashier-23.1.2/pycashier/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4299 2023-01-07 17:00:21.407538 pycashier-23.1.2/pycashier/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1563 2023-01-07 17:00:21.407538 pycashier-23.1.2/pycashier/cluster.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3022 2023-01-07 17:00:21.407538 pycashier-23.1.2/pycashier/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2935 2023-01-07 17:00:21.407538 pycashier-23.1.2/pycashier/extract.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4273 2023-01-07 17:00:21.407538 pycashier-23.1.2/pycashier/merge.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11234 2023-01-07 17:00:21.407538 pycashier-23.1.2/pycashier/options.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4943 2023-01-07 17:00:21.407538 pycashier-23.1.2/pycashier/pycashier.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3128 2023-01-07 17:00:21.407538 pycashier-23.1.2/pycashier/read_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7566 2023-01-07 17:00:21.407538 pycashier-23.1.2/pycashier/single_cell.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2925 2023-01-07 17:00:21.407538 pycashier-23.1.2/pycashier/term.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7897 2023-01-07 17:00:21.407538 pycashier-23.1.2/pycashier/termui.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3302 2023-01-07 17:00:21.407538 pycashier-23.1.2/pycashier/trim.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8842 2023-01-07 17:00:21.407538 pycashier-23.1.2/pycashier/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-01-07 17:00:21.407538 pycashier-23.1.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)    62389 2023-01-07 17:00:21.407538 pycashier-23.1.2/tests/data/reference/mergedfastqs/test.merged.raw.fastq
+-rw-r--r--   0 runner    (1001) docker     (123)     1960 2023-01-07 17:00:21.407538 pycashier-23.1.2/tests/data/reference/outs/test.q30.barcodes.r3d1.min0_off1.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)      445 2023-01-07 17:00:21.407538 pycashier-23.1.2/tests/data/reference/outs-scrna/test.cell_record_labeled.barcode.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)     5660 2023-01-07 17:00:21.407538 pycashier-23.1.2/tests/data/reference/rawfastqgzs/test.fastq.gz
+-rw-r--r--   0 runner    (1001) docker     (123)   427534 2023-01-07 17:00:21.411538 pycashier-23.1.2/tests/data/reference/sams/test.sam
+-rw-r--r--   0 runner    (1001) docker     (123)     7121 2023-01-07 17:00:21.411538 pycashier-23.1.2/tests/data/reference/unmergedfastqgzs/test.R1.raw.fastq.gz
+-rw-r--r--   0 runner    (1001) docker     (123)     8577 2023-01-07 17:00:21.411538 pycashier-23.1.2/tests/data/reference/unmergedfastqgzs/test.R2.raw.fastq.gz
+-rw-r--r--   0 runner    (1001) docker     (123)     2323 2023-01-07 17:00:21.411538 pycashier-23.1.2/tests/test_pycashier.py
+-rw-------   0 runner    (1001) docker     (123)     9995 2023-01-07 17:00:31.891631 pycashier-23.1.2/PKG-INFO
```

### Comparing `pycashier-23.1.1/LICENSE` & `pycashier-23.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pycashier-23.1.1/README.md` & `pycashier-23.1.2/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -37,15 +37,15 @@
 ```bash
 conda install -c conda-forge -c bioconda cutadapt fastp pysam starcode pycashier
 ```
 
 You can also use the included `env.yml` to create your environment and install everything you need.
 
 ```bash
-conda env create -f https://raw.githubusercontent.com/brocklab/pycashier/main/env.yml
+conda env create -f https://raw.githubusercontent.com/brocklab/pycashier/main/conda/env.yml
 conda activate cashierenv
 ```
 
 ### Docker
 
 If you prefer to use use `docker` you can use the below command.
```

### Comparing `pycashier-23.1.1/pycashier/_checks.py` & `pycashier-23.1.2/pycashier/_checks.py`

 * *Files identical despite different names*

### Comparing `pycashier-23.1.1/pycashier/cli.py` & `pycashier-23.1.2/pycashier/cli.py`

 * *Files identical despite different names*

### Comparing `pycashier-23.1.1/pycashier/cluster.py` & `pycashier-23.1.2/pycashier/cluster.py`

 * *Files identical despite different names*

### Comparing `pycashier-23.1.1/pycashier/config.py` & `pycashier-23.1.2/pycashier/config.py`

 * *Files identical despite different names*

### Comparing `pycashier-23.1.1/pycashier/extract.py` & `pycashier-23.1.2/pycashier/extract.py`

 * *Files identical despite different names*

### Comparing `pycashier-23.1.1/pycashier/merge.py` & `pycashier-23.1.2/pycashier/merge.py`

 * *Files identical despite different names*

### Comparing `pycashier-23.1.1/pycashier/options.py` & `pycashier-23.1.2/pycashier/options.py`

 * *Files 0% similar despite different names*

```diff
@@ -43,15 +43,15 @@
     default: Optional[Union[str, int, float, Path]] = None
     show_default: bool = False
     is_flag: bool = False
     type: Any = None
     required: bool = False
     params: Dict[str, Any] = field(default_factory=dict)
     name: str = ""
-    category: str | None = None
+    category: Optional[str] = None
 
     def __post_init__(self) -> None:
         if not self.name:
             self.name = max(self.param_decls, key=len).lstrip("-")
 
     def get_click_option(self) -> Callable[[click.decorators.FC], click.decorators.FC]:
         return click.option(
@@ -70,15 +70,15 @@
     #     return func
 
     def long(self) -> str:
         """return longest param declaration"""
         return max(self.param_decls, key=len)
 
 
-general_opts = ("verbose", "config", "save-config")
+general_opts = ("verbose", "config", "save-config", "skip-init-check")
 
 
 class OptionMap:
     def __init__(
         self, options: Tuple[Option, ...], subcmd_ref: Dict[str, Tuple[str, ...]]
     ) -> None:
         self.opts = {opt.name: opt for opt in options}
```

### Comparing `pycashier-23.1.1/pycashier/pycashier.py` & `pycashier-23.1.2/pycashier/pycashier.py`

 * *Files identical despite different names*

### Comparing `pycashier-23.1.1/pycashier/read_filter.py` & `pycashier-23.1.2/pycashier/read_filter.py`

 * *Files identical despite different names*

### Comparing `pycashier-23.1.1/pycashier/single_cell.py` & `pycashier-23.1.2/pycashier/single_cell.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import sys
 from pathlib import Path
-from typing import List
+from typing import List, Optional
 
 from rich.status import Status
 
 try:
     import pysam
 except ImportError:
     pass
@@ -162,15 +162,15 @@
 
     if check_output(tsv_out, "converting labeled fastq to tsv"):
         labeled_fastq_to_tsv(barcode_fastq, tsv_out)
 
 
 def single_cell(
     input_: Path,
-    samples: List[str] | None,
+    samples: Optional[List[str]],
     pipeline: Path,
     output: Path,
     error: float,
     minimum_length: int,
     length: int,
     upstream_adapter: str,
     downstream_adapter: str,
```

### Comparing `pycashier-23.1.1/pycashier/term.py` & `pycashier-23.1.2/pycashier/term.py`

 * *Files identical despite different names*

### Comparing `pycashier-23.1.1/pycashier/termui.py` & `pycashier-23.1.2/pycashier/termui.py`

 * *Files identical despite different names*

### Comparing `pycashier-23.1.1/pycashier/trim.py` & `pycashier-23.1.2/pycashier/trim.py`

 * *Files identical despite different names*

### Comparing `pycashier-23.1.1/pycashier/utils.py` & `pycashier-23.1.2/pycashier/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import csv
 import shlex
 import subprocess
 import sys
 from collections.abc import Iterable
 from itertools import zip_longest
 from pathlib import Path
-from typing import Any, Dict, List
+from typing import Any, Dict, List, Optional
 
 import click
 from rich.status import Status
 
 from .term import term
 
 
@@ -42,15 +42,15 @@
         term.print(f"[dim]ignoring {len(set(ignored))} samples")
 
     return files
 
 
 def get_input_files(
     src: Path,
-    samples: List[str] | None,
+    samples: Optional[List[str]],
     exts: List[str],
 ) -> List[Path]:
     """determine input files
     Args:
         src: Input directory that contains fastq/sam files.
         samples: List of allowed samples.
         exts: Acceptable file extensions.
@@ -158,15 +158,15 @@
         for row in spamreader:
             total_reads += float(row[1])
 
     return int(round(total_reads * filter_percent / 100, 0))
 
 
 def combine_outs(
-    input_dir: Path, samples: List[str] | None, output: Path, columns: List[str]
+    input_dir: Path, samples: Optional[List[str]], output: Path, columns: List[str]
 ) -> None:
     """combine output tsvs into one file
 
     Args:
         input_dir: Directory containing csv files to combine.
         samples: list of sample names to use
         output: TSV to save all data to.
```

### Comparing `pycashier-23.1.1/pyproject.toml` & `pycashier-23.1.2/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     "tomlkit>=0.10.1",
     "click-rich-help>=22.1.0",
     "click>=8.1.0",
 ]
 requires-python = ">=3.8,<3.11"
 readme = "README.md"
 dynamic = []
-version = "23.1.1"
+version = "23.1.2"
 
 [project.license]
 text = "MIT"
 
 [project.urls]
 repository = "https://github.com/brocklab/pycashier/"
```

### Comparing `pycashier-23.1.1/tests/data/reference/mergedfastqs/test.merged.raw.fastq` & `pycashier-23.1.2/tests/data/reference/mergedfastqs/test.merged.raw.fastq`

 * *Files identical despite different names*

### Comparing `pycashier-23.1.1/tests/data/reference/outs/test.q30.barcodes.r3d1.min0_off1.tsv` & `pycashier-23.1.2/tests/data/reference/outs/test.q30.barcodes.r3d1.min0_off1.tsv`

 * *Files identical despite different names*

### Comparing `pycashier-23.1.1/tests/data/reference/rawfastqgzs/test.fastq.gz` & `pycashier-23.1.2/tests/data/reference/rawfastqgzs/test.fastq.gz`

 * *Files identical despite different names*

### Comparing `pycashier-23.1.1/tests/data/reference/sams/test.sam` & `pycashier-23.1.2/tests/data/reference/sams/test.sam`

 * *Files identical despite different names*

### Comparing `pycashier-23.1.1/tests/data/reference/unmergedfastqgzs/test.R1.raw.fastq.gz` & `pycashier-23.1.2/tests/data/reference/unmergedfastqgzs/test.R1.raw.fastq.gz`

 * *Files identical despite different names*

### Comparing `pycashier-23.1.1/tests/data/reference/unmergedfastqgzs/test.R2.raw.fastq.gz` & `pycashier-23.1.2/tests/data/reference/unmergedfastqgzs/test.R2.raw.fastq.gz`

 * *Files identical despite different names*

### Comparing `pycashier-23.1.1/tests/test_pycashier.py` & `pycashier-23.1.2/tests/test_pycashier.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import filecmp
 import shutil
 import subprocess
 from pathlib import Path
-from typing import List, Tuple
+from typing import List, Tuple, Union
 
 TEST_DIR = Path(__file__).parent
 OUTS_DIR, REF_DIR, MERGED_DIR, PIPELINE_DIR = (
     TEST_DIR / "data" / name
     for name in ("outs", "reference", "mergedfastqs", "pipeline")
 )
 
@@ -18,15 +18,15 @@
 
 
 def cmp_outs(filename: str, paths: Tuple[Path, Path]) -> bool:
     file_one, file_two = (filepath / filename for filepath in paths)
     return filecmp.cmp(file_one, file_two)
 
 
-def pycashier_run(cmd: List[str | Path]) -> subprocess.CompletedProcess:
+def pycashier_run(cmd: List[Union[str, Path]]) -> subprocess.CompletedProcess:
     p = subprocess.run(
         ["pycashier", *cmd],
         capture_output=True,
         universal_newlines=True,
     )
     return p
```

### Comparing `pycashier-23.1.1/PKG-INFO` & `pycashier-23.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pycashier
-Version: 23.1.1
+Version: 23.1.2
 Summary: cash in on expressed barcode tags
 License: MIT
 Author-email: Daylin Morgan <daylinmorgan@gmail.com>
 Requires-Python: >=3.8,<3.11
 Project-URL: repository, https://github.com/brocklab/pycashier/
 Description-Content-Type: text/markdown
 
@@ -47,15 +47,15 @@
 ```bash
 conda install -c conda-forge -c bioconda cutadapt fastp pysam starcode pycashier
 ```
 
 You can also use the included `env.yml` to create your environment and install everything you need.
 
 ```bash
-conda env create -f https://raw.githubusercontent.com/brocklab/pycashier/main/env.yml
+conda env create -f https://raw.githubusercontent.com/brocklab/pycashier/main/conda/env.yml
 conda activate cashierenv
 ```
 
 ### Docker
 
 If you prefer to use use `docker` you can use the below command.
```

