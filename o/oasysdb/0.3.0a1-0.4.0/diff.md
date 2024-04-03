# Comparing `tmp/oasysdb-0.3.0a1.tar.gz` & `tmp/oasysdb-0.4.0.tar.gz`

## Comparing `oasysdb-0.3.0a1.tar` & `oasysdb-0.4.0.tar`

### file list

```diff
@@ -1,50 +1,54 @@
--rw-r--r--   0        0        0     1244 1970-01-01 00:00:00.000000 oasysdb-0.3.0a1/Cargo.toml
--rw-r--r--   0     1001      127      161 2024-03-12 22:58:39.000000 oasysdb-0.3.0a1/.editorconfig
--rw-r--r--   0     1001      127      761 2024-03-12 22:58:39.000000 oasysdb-0.3.0a1/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0     1001      127      331 2024-03-12 22:58:39.000000 oasysdb-0.3.0a1/.github/ISSUE_TEMPLATE/config.yml
--rw-r--r--   0     1001      127      496 2024-03-12 22:58:39.000000 oasysdb-0.3.0a1/.github/ISSUE_TEMPLATE/do_chore.md
--rw-r--r--   0     1001      127      664 2024-03-12 22:58:39.000000 oasysdb-0.3.0a1/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0     1001      127     3048 2024-03-12 22:58:39.000000 oasysdb-0.3.0a1/.github/workflows/deploy-python.yml
--rw-r--r--   0     1001      127      477 2024-03-12 22:58:39.000000 oasysdb-0.3.0a1/.github/workflows/deploy-rust.yml
--rw-r--r--   0     1001      127     1739 2024-03-12 22:58:39.000000 oasysdb-0.3.0a1/.github/workflows/quality-check.yml
--rw-r--r--   0     1001      127      220 2024-03-12 22:58:39.000000 oasysdb-0.3.0a1/.gitignore
--rw-r--r--   0     1001      127       93 2024-03-12 22:58:39.000000 oasysdb-0.3.0a1/.prettierrc.yml
--rw-r--r--   0     1001      127    34291 2024-03-12 22:58:39.000000 oasysdb-0.3.0a1/Cargo.lock
--rw-r--r--   0     1001      127     1082 2024-03-12 22:58:39.000000 oasysdb-0.3.0a1/bench/main.rs
--rw-r--r--   0     1001      127     3167 2024-03-12 22:58:39.000000 oasysdb-0.3.0a1/bench/utils.rs
--rw-r--r--   0     1001      127     2072 2024-03-12 22:58:39.000000 oasysdb-0.3.0a1/docs/changelog.md
--rw-r--r--   0     1001      127     5481 2024-03-12 22:58:39.000000 oasysdb-0.3.0a1/docs/code_of_conduct.md
--rw-r--r--   0     1001      127     4741 2024-03-12 22:58:39.000000 oasysdb-0.3.0a1/docs/contributing.md
--rw-r--r--   0     1001      127      798 2024-03-12 22:58:39.000000 oasysdb-0.3.0a1/docs/pull_request_template.md
--rw-r--r--   0     1001      127      722 2024-03-12 22:58:39.000000 oasysdb-0.3.0a1/docs/security.md
--rw-r--r--   0     1001      127      451 2024-03-12 22:58:39.000000 oasysdb-0.3.0a1/examples/extract-metadata.rs
--rw-r--r--   0     1001      127      609 2024-03-12 22:58:39.000000 oasysdb-0.3.0a1/examples/measure-memory.rs
--rw-r--r--   0     1001      127    10173 2024-03-12 22:58:39.000000 oasysdb-0.3.0a1/license
--rw-r--r--   0     1001      127      778 2024-03-12 22:58:39.000000 oasysdb-0.3.0a1/py/example.py
--rw-r--r--   0     1001      127       43 2024-03-12 22:58:39.000000 oasysdb-0.3.0a1/py/oasysdb/__init__.py
--rw-r--r--   0     1001      127     4128 2024-03-12 22:58:39.000000 oasysdb-0.3.0a1/py/oasysdb/collection.pyi
--rw-r--r--   0     1001      127     1653 2024-03-12 22:58:39.000000 oasysdb-0.3.0a1/py/oasysdb/database.pyi
--rw-r--r--   0     1001      127        0 2024-03-12 22:58:39.000000 oasysdb-0.3.0a1/py/oasysdb/py.typed
--rw-r--r--   0     1001      127      757 2024-03-12 22:58:39.000000 oasysdb-0.3.0a1/py/oasysdb/vector.pyi
--rw-r--r--   0     1001      127     3886 2024-03-12 22:58:39.000000 oasysdb-0.3.0a1/py/tests/test_collection.py
--rw-r--r--   0     1001      127     1350 2024-03-12 22:58:39.000000 oasysdb-0.3.0a1/py/tests/test_database.py
--rw-r--r--   0     1001      127      389 2024-03-12 22:58:39.000000 oasysdb-0.3.0a1/py/tests/test_vector.py
--rw-r--r--   0     1001      127     8510 2024-03-12 22:58:39.000000 oasysdb-0.3.0a1/readme.md
--rw-r--r--   0     1001      127       14 2024-03-12 22:58:39.000000 oasysdb-0.3.0a1/requirements.txt
--rw-r--r--   0     1001      127      104 2024-03-12 22:58:39.000000 oasysdb-0.3.0a1/rustfmt.toml
--rw-r--r--   0     1001      127     3687 2024-03-12 22:58:39.000000 oasysdb-0.3.0a1/src/db/database.rs
--rw-r--r--   0     1001      127      205 2024-03-12 22:58:39.000000 oasysdb-0.3.0a1/src/db/mod.rs
--rw-r--r--   0     1001      127    21206 2024-03-12 22:58:39.000000 oasysdb-0.3.0a1/src/func/collection.rs
--rw-r--r--   0     1001      127     2534 2024-03-12 22:58:39.000000 oasysdb-0.3.0a1/src/func/err.rs
--rw-r--r--   0     1001      127     3980 2024-03-12 22:58:39.000000 oasysdb-0.3.0a1/src/func/metadata.rs
--rw-r--r--   0     1001      127      784 2024-03-12 22:58:39.000000 oasysdb-0.3.0a1/src/func/mod.rs
--rw-r--r--   0     1001      127     9509 2024-03-12 22:58:39.000000 oasysdb-0.3.0a1/src/func/utils.rs
--rw-r--r--   0     1001      127     2571 2024-03-12 22:58:39.000000 oasysdb-0.3.0a1/src/func/vector.rs
--rw-r--r--   0     1001      127     1651 2024-03-12 22:58:39.000000 oasysdb-0.3.0a1/src/lib.rs
--rw-r--r--   0     1001      127       13 2024-03-12 22:58:39.000000 oasysdb-0.3.0a1/src/main.rs
--rw-r--r--   0     1001      127      159 2024-03-12 22:58:39.000000 oasysdb-0.3.0a1/src/prelude/mod.rs
--rw-r--r--   0     1001      127      667 2024-03-12 22:58:39.000000 oasysdb-0.3.0a1/src/tests/mod.rs
--rw-r--r--   0     1001      127     3354 2024-03-12 22:58:39.000000 oasysdb-0.3.0a1/src/tests/test_collection.rs
--rw-r--r--   0     1001      127     1504 2024-03-12 22:58:39.000000 oasysdb-0.3.0a1/src/tests/test_database.rs
--rw-r--r--   0     1001      127      640 2024-03-12 22:58:39.000000 oasysdb-0.3.0a1/pyproject.toml
--rw-r--r--   0        0        0     9285 1970-01-01 00:00:00.000000 oasysdb-0.3.0a1/PKG-INFO
+-rw-r--r--   0        0        0     1236 1970-01-01 00:00:00.000000 oasysdb-0.4.0/Cargo.toml
+-rw-r--r--   0     1001      127      161 2024-04-03 17:29:18.000000 oasysdb-0.4.0/.editorconfig
+-rw-r--r--   0     1001      127      761 2024-04-03 17:29:18.000000 oasysdb-0.4.0/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0     1001      127      331 2024-04-03 17:29:18.000000 oasysdb-0.4.0/.github/ISSUE_TEMPLATE/config.yml
+-rw-r--r--   0     1001      127      496 2024-04-03 17:29:18.000000 oasysdb-0.4.0/.github/ISSUE_TEMPLATE/do_chore.md
+-rw-r--r--   0     1001      127      664 2024-04-03 17:29:18.000000 oasysdb-0.4.0/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0     1001      127     3048 2024-04-03 17:29:18.000000 oasysdb-0.4.0/.github/workflows/deploy-python.yml
+-rw-r--r--   0     1001      127      477 2024-04-03 17:29:18.000000 oasysdb-0.4.0/.github/workflows/deploy-rust.yml
+-rw-r--r--   0     1001      127     1739 2024-04-03 17:29:18.000000 oasysdb-0.4.0/.github/workflows/quality-check.yml
+-rw-r--r--   0     1001      127      220 2024-04-03 17:29:18.000000 oasysdb-0.4.0/.gitignore
+-rw-r--r--   0     1001      127       93 2024-04-03 17:29:18.000000 oasysdb-0.4.0/.prettierrc.yml
+-rw-r--r--   0     1001      127    34283 2024-04-03 17:29:18.000000 oasysdb-0.4.0/Cargo.lock
+-rw-r--r--   0     1001      127     1020 2024-04-03 17:29:18.000000 oasysdb-0.4.0/bench/main.rs
+-rw-r--r--   0     1001      127     3175 2024-04-03 17:29:18.000000 oasysdb-0.4.0/bench/utils.rs
+-rw-r--r--   0     1001      127     4768 2024-04-03 17:29:18.000000 oasysdb-0.4.0/docs/changelog.md
+-rw-r--r--   0     1001      127     5481 2024-04-03 17:29:18.000000 oasysdb-0.4.0/docs/code_of_conduct.md
+-rw-r--r--   0     1001      127     5222 2024-04-03 17:29:18.000000 oasysdb-0.4.0/docs/contributing.md
+-rw-r--r--   0     1001      127      798 2024-04-03 17:29:18.000000 oasysdb-0.4.0/docs/pull_request_template.md
+-rw-r--r--   0     1001      127      722 2024-04-03 17:29:18.000000 oasysdb-0.4.0/docs/security.md
+-rw-r--r--   0     1001      127      453 2024-04-03 17:29:18.000000 oasysdb-0.4.0/examples/extract-metadata.rs
+-rw-r--r--   0     1001      127      611 2024-04-03 17:29:18.000000 oasysdb-0.4.0/examples/measure-memory.rs
+-rw-r--r--   0     1001      127      802 2024-04-03 17:29:18.000000 oasysdb-0.4.0/examples/quickstart.rs
+-rw-r--r--   0     1001      127    10173 2024-04-03 17:29:18.000000 oasysdb-0.4.0/license
+-rw-r--r--   0     1001      127      710 2024-04-03 17:29:18.000000 oasysdb-0.4.0/py/example.py
+-rw-r--r--   0     1001      127       43 2024-04-03 17:29:18.000000 oasysdb-0.4.0/py/oasysdb/__init__.py
+-rw-r--r--   0     1001      127     4498 2024-04-03 17:29:18.000000 oasysdb-0.4.0/py/oasysdb/collection.pyi
+-rw-r--r--   0     1001      127     1227 2024-04-03 17:29:18.000000 oasysdb-0.4.0/py/oasysdb/database.pyi
+-rw-r--r--   0     1001      127      119 2024-04-03 17:29:18.000000 oasysdb-0.4.0/py/oasysdb/prelude.pyi
+-rw-r--r--   0     1001      127        0 2024-04-03 17:29:18.000000 oasysdb-0.4.0/py/oasysdb/py.typed
+-rw-r--r--   0     1001      127      757 2024-04-03 17:29:18.000000 oasysdb-0.4.0/py/oasysdb/vector.pyi
+-rw-r--r--   0     1001      127     4799 2024-04-03 17:29:18.000000 oasysdb-0.4.0/py/tests/test_collection.py
+-rw-r--r--   0     1001      127     1462 2024-04-03 17:29:18.000000 oasysdb-0.4.0/py/tests/test_database.py
+-rw-r--r--   0     1001      127      390 2024-04-03 17:29:18.000000 oasysdb-0.4.0/py/tests/test_vector.py
+-rw-r--r--   0     1001      127     8980 2024-04-03 17:29:18.000000 oasysdb-0.4.0/readme.md
+-rw-r--r--   0     1001      127       14 2024-04-03 17:29:18.000000 oasysdb-0.4.0/requirements.txt
+-rw-r--r--   0     1001      127      104 2024-04-03 17:29:18.000000 oasysdb-0.4.0/rustfmt.toml
+-rw-r--r--   0     1001      127     2765 2024-04-03 17:29:18.000000 oasysdb-0.4.0/src/db/database.rs
+-rw-r--r--   0     1001      127      205 2024-04-03 17:29:18.000000 oasysdb-0.4.0/src/db/mod.rs
+-rw-r--r--   0     1001      127    23799 2024-04-03 17:29:18.000000 oasysdb-0.4.0/src/func/collection.rs
+-rw-r--r--   0     1001      127     2313 2024-04-03 17:29:18.000000 oasysdb-0.4.0/src/func/distance.rs
+-rw-r--r--   0     1001      127     2534 2024-04-03 17:29:18.000000 oasysdb-0.4.0/src/func/err.rs
+-rw-r--r--   0     1001      127     3980 2024-04-03 17:29:18.000000 oasysdb-0.4.0/src/func/metadata.rs
+-rw-r--r--   0     1001      127      886 2024-04-03 17:29:18.000000 oasysdb-0.4.0/src/func/mod.rs
+-rw-r--r--   0     1001      127    12506 2024-04-03 17:29:18.000000 oasysdb-0.4.0/src/func/utils.rs
+-rw-r--r--   0     1001      127     2272 2024-04-03 17:29:18.000000 oasysdb-0.4.0/src/func/vector.rs
+-rw-r--r--   0     1001      127     2101 2024-04-03 17:29:18.000000 oasysdb-0.4.0/src/lib.rs
+-rw-r--r--   0     1001      127       13 2024-04-03 17:29:18.000000 oasysdb-0.4.0/src/main.rs
+-rw-r--r--   0     1001      127      193 2024-04-03 17:29:18.000000 oasysdb-0.4.0/src/prelude/mod.rs
+-rw-r--r--   0     1001      127      998 2024-04-03 17:29:18.000000 oasysdb-0.4.0/src/tests/mod.rs
+-rw-r--r--   0     1001      127     4641 2024-04-03 17:29:18.000000 oasysdb-0.4.0/src/tests/test_collection.rs
+-rw-r--r--   0     1001      127     1495 2024-04-03 17:29:18.000000 oasysdb-0.4.0/src/tests/test_database.rs
+-rw-r--r--   0     1001      127      409 2024-04-03 17:29:18.000000 oasysdb-0.4.0/src/tests/test_distance.rs
+-rw-r--r--   0     1001      127      640 2024-04-03 17:29:18.000000 oasysdb-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0     9753 1970-01-01 00:00:00.000000 oasysdb-0.4.0/PKG-INFO
```

### Comparing `oasysdb-0.3.0a1/Cargo.toml` & `oasysdb-0.4.0/Cargo.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "oasysdb"
-version = "0.3.0-alpha.1"
+version = "0.4.0"
 edition = "2021"
 license = "Apache-2.0"
 readme = "readme.md"
 
 # Information.
 authors = ["Edwin Kys", "Oasys"]
 description = "Fast embedded vector database with incremental HNSW indexing."
```

### Comparing `oasysdb-0.3.0a1/.github/ISSUE_TEMPLATE/bug_report.md` & `oasysdb-0.4.0/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `oasysdb-0.3.0a1/.github/ISSUE_TEMPLATE/feature_request.md` & `oasysdb-0.4.0/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `oasysdb-0.3.0a1/.github/workflows/deploy-python.yml` & `oasysdb-0.4.0/.github/workflows/deploy-python.yml`

 * *Files identical despite different names*

### Comparing `oasysdb-0.3.0a1/.github/workflows/quality-check.yml` & `oasysdb-0.4.0/.github/workflows/quality-check.yml`

 * *Files identical despite different names*

### Comparing `oasysdb-0.3.0a1/Cargo.lock` & `oasysdb-0.4.0/Cargo.lock`

 * *Files 1% similar despite different names*

```diff
@@ -529,15 +529,15 @@
 dependencies = [
  "hermit-abi",
  "libc",
 ]
 
 [[package]]
 name = "oasysdb"
-version = "0.3.0-alpha.1"
+version = "0.4.0"
 dependencies = [
  "bincode",
  "byteorder",
  "criterion",
  "curl",
  "flate2",
  "jemalloc-ctl",
```

### Comparing `oasysdb-0.3.0a1/bench/main.rs` & `oasysdb-0.4.0/bench/main.rs`

 * *Files 10% similar despite different names*

```diff
@@ -1,37 +1,37 @@
 mod utils;
 
-use criterion::{black_box, criterion_group, criterion_main, Criterion};
-use oasysdb::collection::{Collection, Config};
+use criterion::*;
+use oasysdb::prelude::*;
 use utils::*;
 
 fn build_collection(path: &str) -> Collection {
     let records = get_records(path).unwrap();
     let config = Config::default();
-    Collection::build(config, records).unwrap()
+    Collection::build(&config, &records).unwrap()
 }
 
 fn bench_search_collection(criterion: &mut Criterion) {
     let id = "Search collection";
 
     // Download the dataset.
     download_siftsmall().unwrap();
 
     // Load the query data.
     let query_path = "data/siftsmall/siftsmall_query.fvecs";
     let query_data = read_vectors(query_path).unwrap();
+    let vector: Vector = query_data[0].clone().into();
 
     // Create the collection.
     let base_path = "data/siftsmall/siftsmall_base.fvecs";
     let collection = build_collection(base_path);
 
     // Benchmark the search speed.
     let routine = || {
-        let vector = query_data[0].clone();
-        black_box(collection.search(vector, 10).unwrap());
+        black_box(collection.search(&vector, 10).unwrap());
     };
 
     criterion.bench_function(id, |bencher| bencher.iter(routine));
 }
 
 criterion_group!(bench, bench_search_collection);
 criterion_main!(bench);
```

### Comparing `oasysdb-0.3.0a1/bench/utils.rs` & `oasysdb-0.4.0/bench/utils.rs`

 * *Files 1% similar despite different names*

```diff
@@ -99,12 +99,12 @@
 /// Reads and converts the vectors from the dataset into records.
 /// * `path`: Path to the dataset file.
 pub fn get_records(path: &str) -> Result<Vec<Record>, Box<dyn Error>> {
     // Create records where the ID is the index.
     let records = read_vectors(path)?
         .par_iter()
         .enumerate()
-        .map(|(id, vec)| Record::new(vec.into(), id.into()))
+        .map(|(id, vector)| Record::new(&vector.into(), &id.into()))
         .collect();
 
     Ok(records)
 }
```

### Comparing `oasysdb-0.3.0a1/docs/code_of_conduct.md` & `oasysdb-0.4.0/docs/code_of_conduct.md`

 * *Files identical despite different names*

### Comparing `oasysdb-0.3.0a1/docs/contributing.md` & `oasysdb-0.4.0/docs/contributing.md`

 * *Files 4% similar despite different names*

```diff
@@ -33,21 +33,33 @@
 
 # Getting started
 
 Getting started with OasysDB development is easy.
 
 You will need to have Rust installed. We recommend using [rustup](https://www.rust-lang.org/tools/install) to install Rust. We also recommend having rust-analyzer installed for your code editor.
 
-Once you have Rust installed, you can clone the repository and run the following commands in the root directory of the repository:
+After that, you need to install Maturin, which is a Python library used by OasysDB for building and publishing its Python packages. You can install Maturin using the following command:
 
 ```bash
+pip install maturin
+```
+
+After setting up Maturin, fork the repository and clone it to your local machine. Then, in the root directory of the project, you need to set up and activate Python virtual environment for the project with `requirements.txt` as the dependency.
+
+Once everything is set, you can run the following commands in the root directory of the repository:
+
+```bash
+# Run Rust tests.
 cargo test
+
+# Run Python tests.
+pytest
 ```
 
-This command will run the tests to make sure that everything is working as expected before you start working on your changes.
+These commands will run the tests to make sure that everything is working as expected before you start working on your changes.
 
 ```bash
 cargo bench
 ```
 
 This command will run the benchmarks to measure the performance of the vector database. This is useful to make sure that your changes don't introduce any significant performance regressions.
```

### Comparing `oasysdb-0.3.0a1/docs/pull_request_template.md` & `oasysdb-0.4.0/docs/pull_request_template.md`

 * *Files identical despite different names*

### Comparing `oasysdb-0.3.0a1/docs/security.md` & `oasysdb-0.4.0/docs/security.md`

 * *Files identical despite different names*

### Comparing `oasysdb-0.3.0a1/examples/measure-memory.rs` & `oasysdb-0.4.0/examples/measure-memory.rs`

 * *Files 2% similar despite different names*

```diff
@@ -9,14 +9,14 @@
     // Modify as needed.
     let len = 10000;
     let dimension = 128;
 
     // Build the vector collection.
     let records = Record::many_random(dimension, len);
     let config = Config::default();
-    Collection::build(config, records).unwrap();
+    Collection::build(&config, &records).unwrap();
 
     // Measure the memory usage.
     let memory = allocated::read().unwrap();
     println!("For {} vector records of dimension {}", len, dimension);
     println!("Memory usage: {} bytes", memory);
 }
```

### Comparing `oasysdb-0.3.0a1/license` & `oasysdb-0.4.0/license`

 * *Files identical despite different names*

### Comparing `oasysdb-0.3.0a1/py/oasysdb/collection.pyi` & `oasysdb-0.4.0/py/oasysdb/collection.pyi`

 * *Files 11% similar despite different names*

```diff
@@ -1,165 +1,180 @@
 # flake8: noqa F821
 
-from typing import Any, List
-from oasysdb.vector import Vector
+from typing import Any, List, Dict
+from oasysdb.vector import Vector, VectorID
 
 
 class Config:
     """The configuration for the vector collection.
 
     Args:
-    - ef_construction (int): Nodes to consider during index construction.
-    - ef_search (int): Nodes to consider during the search.
-    - ml (float): Layer multiplier of the HNSW index.
+    - ef_construction: Nodes to consider during index construction.
+    - ef_search: Nodes to consider during the search.
+    - ml: Layer multiplier of the HNSW index.
+    - distance: Distance metric function.
     """
 
     ef_construction: int
     ef_search: int
     ml: float
+    distance: str
 
     def __init__(
         self,
         ef_construction: int,
         ef_search: int,
         ml: float,
+        distance: str
     ) -> None: ...
 
     @staticmethod
     def create_default() -> Config:
         """Returns a default configuration.
 
         Default values:
         - ef_construction: 40
         - ef_search: 15
         - ml: 0.3
+        - distance: euclidean
         """
 
 
 class Record:
     """The vector record to store in the collection.
 
     Args:
-    - vector (List[float]): Vector embedding of float values.
-    - data (Metadata): Metadata of the vector.
+    - vector: Vector embedding of float values.
+    - data: Metadata of the vector.
 
     Metadata types:
     - String
     - Number
     - List of metadata types
     - Dictionary of metadata types
     """
 
-    vector: List[float]
+    vector: Vector
     data: Any
 
     def __init__(self, vector: List[float], data: Any) -> None: ...
 
     @staticmethod
     def random(dimension: int) -> Record:
         """Generates a random record with the given dimension
         with a random integer metadata.
 
         Args:
-        - dimension (int): Vector dimension.
+        - dimension: Vector dimension.
         """
 
     @staticmethod
     def many_random(dimension: int, len: int) -> List[Record]:
         """Generates a list of random records.
 
         Args:
-        - dimension (int): Vector dimension.
-        - len (int): Number of records.
+        - dimension: Vector dimension.
+        - len: Number of records.
         """
 
 
 class Collection:
     """The collection of vectors and their metadata."""
 
     config: Config
+    dimension: int
+    relevancy: float
 
     def __init__(self, config: Config) -> None: ...
 
     @staticmethod
-    def build(
-        config: Config,
-        records: List[Record],
-    ) -> Collection:
+    def from_records(config: Config, records: List[Record]) -> Collection:
         """Build a collection from the given records.
 
         Args:
-        - config (Config): Collection configuration.
-        - records (List[Record]): Records used to build the collection.
+        - config: Collection configuration.
+        - records: Records used to build the collection.
+        """
+
+    @staticmethod
+    def build(config: Config, records: List[Record]) -> Collection:
+        """Build a collection from the records.
+        This is an alias of from_records method and shared
+        the same implementation.
+
+        Args:
+        - config: Collection configuration.
+        - records: Records used to build the collection.
         """
 
     def insert(self, record: Record) -> None:
         """Inserts a record into the collection.
 
         Args:
-        - record (Record): Record to insert.
+        - record: Record to insert.
+        """
+
+    def insert_many(self, records: List[Record]) -> List[VectorID]:
+        """Inserts multiple records into the collection.
+
+        Args:
+        - records: Records to insert.
         """
 
-    def delete(self, id: int) -> None:
+    def delete(self, id: VectorID) -> None:
         """Deletes a record from the collection.
 
         Args:
-        - id (int): Vector ID to delete.
+        - id: Vector ID to delete.
         """
 
-    def get(self, id: int) -> Record:
+    def get(self, id: VectorID) -> Record:
         """Returns a record from the collection.
 
         Args:
-        - id (int): Vector ID to fetch.
+        - id: Vector ID to fetch.
+        """
+
+    def list(self) -> Dict[VectorID, Record]:
+        """Returns a dictionary of records in the collection
+        in the format of { VectorID: Record }.
         """
 
-    def update(self, id: int, record: Record) -> None:
+    def update(self, id: VectorID, record: Record) -> None:
         """Updates a record in the collection.
 
         Args:
-        - id (int): Vector ID to update.
-        - record (Record): New record.
+        - id: Vector ID to update.
+        - record: New record.
         """
 
-    def search(self, vector: List[float], n: int) -> List[SearchResult]:
+    def search(self, vector: Vector, n: int) -> List[SearchResult]:
         """Searches for the nearest neighbors to
         the given vector using HNSW indexing algorithm
 
         Args:
-        - vector (List[float]): Vector to search.
-        - n (int): Number of neighbors to return.
+        - vector: Vector to search.
+        - n: Number of neighbors to return.
         """
 
-    def true_search(self, vector: List[float], n: int) -> List[SearchResult]:
+    def true_search(self, vector: Vector, n: int) -> List[SearchResult]:
         """Searches for the nearest neighbors using brute force.
 
         Args:
-        - vector (List[float]): Vector to search.
-        - n (int): Number of neighbors to return.
-        """
-
-    def dimension(self) -> int:
-        """Returns the configured vector dimension in the collection."""
-
-    def set_dimension(self, dimension: int) -> None:
-        """Sets the vector dimension of the collection.
-        The collection must be empty to do this.
-
-        Args:
-        - dimension (int): Vector dimension.
+        - vector: Vector to search.
+        - n: Number of neighbors to return.
         """
 
     def len(self) -> int:
         """Returns the number of records in the collection."""
 
     def is_empty(self) -> bool:
         """Returns True if the collection is empty."""
 
-    def contains(self, id: int) -> bool:
+    def contains(self, id: VectorID) -> bool:
         """Returns True if the vector ID is in the collection."""
 
 
 class SearchResult:
     """The result of a search operation on the collection."""
 
     id: int
```

### Comparing `oasysdb-0.3.0a1/py/oasysdb/database.pyi` & `oasysdb-0.4.0/py/oasysdb/database.pyi`

 * *Files 22% similar despite different names*

```diff
@@ -3,61 +3,47 @@
 from oasysdb.collection import Collection, Record, Config
 
 
 class Database:
     """The persistent storage of vector collections.
 
     Args:
-    - path (str): Path to the database file.
+    - path: Path to the database file.
     """
 
     def __init__(self, path: str,) -> None: ...
 
     def new(path: str) -> Database:
         """Creates a new database at the given path.
         This will reset the database if it exists.
 
         Args:
-        - path (str): Path to the database file.
-        """
-
-    def create_collection(
-        self,
-        name: str,
-        config: Config = None,
-        records: List[Record] = None
-    ) -> None:
-        """Creates a new collection in the database.
-
-        Args:
-        - name (str): Collection name.
-        - config (Config): Collection configuration.
-        - records (List[Record]): Records to build the collection.
+        - path: Path to the database file.
         """
 
     def get_collection(self, name: str) -> Collection:
         """Returns the collection with the given name.
 
         Args:
-        - name (str): Collection name.
+        - name: Collection name.
         """
 
     def save_collection(self, name: str, collection: Collection) -> None:
         """Saves new or update existing collection to the database.
 
         Args:
-        - name (str): Collection name.
-        - collection (Collection): Vector collection.
+        - name: Collection name.
+        - collection: Vector collection.
         """
 
     def delete_collection(self, name: str) -> None:
         """Deletes the collection from the database.
 
         Args:
-        - name (str): Collection name.
+        - name: Collection name.
         """
 
     def len(self) -> int:
         """Returns the number of collections in the database."""
 
     def is_empty(self) -> bool:
         """Returns True if the database is empty."""
```

### Comparing `oasysdb-0.3.0a1/py/oasysdb/vector.pyi` & `oasysdb-0.4.0/py/oasysdb/vector.pyi`

 * *Files identical despite different names*

### Comparing `oasysdb-0.3.0a1/py/tests/test_collection.py` & `oasysdb-0.4.0/py/tests/test_collection.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,31 +1,38 @@
-from oasysdb.collection import Config, Record, Collection
-from oasysdb.vector import Vector
+from oasysdb.prelude import Config, Record, Collection, Vector, VectorID
 
 DIMENSION = 128
 LEN = 100
 
 
 def create_test_collection() -> Collection:
     """Creates a collection with random records for testing."""
     records = Record.many_random(dimension=DIMENSION, len=LEN)
     config = Config.create_default()
-    collection = Collection.build(config=config, records=records)
+    collection = Collection.from_records(config=config, records=records)
 
     assert collection.len() == len(records)
     return collection
 
 
 def test_create_config():
-    config = Config(ef_construction=40, ef_search=15, ml=0.3)
     default = Config.create_default()
 
+    # Create config based on the default.
+    config = Config(
+        ef_construction=40,
+        ef_search=15,
+        ml=0.3,
+        distance="euclidean"
+    )
+
     assert config.ef_construction == default.ef_construction
     assert config.ef_search == default.ef_search
     assert config.ml == default.ml
+    assert config.distance == default.distance
 
 
 def test_create_record():
     vector = [0.1, 0.2, 0.3]
     data = {"text": "This is an example."}
     record = Record(vector=vector, data=data)
 
@@ -50,25 +57,25 @@
 
     assert collection.config.ml == config.ml
     assert collection.is_empty()
 
 
 def test_build_collection():
     collection = create_test_collection()
-    assert collection.contains(0)
+    assert collection.contains(VectorID(0))
     assert not collection.is_empty()
 
 
 def test_insert_record():
     collection = create_test_collection()
     record = Record.random(dimension=128)
     collection.insert(record)
 
     assert collection.len() == LEN + 1
-    assert collection.contains(LEN)
+    assert collection.contains(VectorID(LEN))
 
 
 def test_insert_record_invalid_dimension():
     collection = create_test_collection()
     record = Record.random(dimension=100)
 
     # Insert should raise an exception because the
@@ -78,71 +85,94 @@
         assert False
     except Exception as e:
         assert "invalid vector dimension" in str(e).lower()
 
     assert collection.len() == LEN
 
 
+def test_insert_many_records():
+    collection = create_test_collection()
+    records = Record.many_random(dimension=DIMENSION, len=LEN)
+    collection.insert_many(records)
+
+    assert collection.len() == 2 * LEN
+    assert all(collection.contains(VectorID(i)) for i in range(LEN, 2 * LEN))
+
+
 def test_delete_record():
     collection = create_test_collection()
 
-    id = 0
+    id = VectorID(0)
     collection.delete(id)
 
     assert not collection.contains(id)
     assert collection.len() == LEN - 1
 
 
 def test_get_record():
     collection = create_test_collection()
 
-    id = 0
+    id = VectorID(0)
     record = collection.get(id)
 
     assert record is not None
     assert record.data is not None
 
 
 def test_update_record():
     collection = create_test_collection()
 
-    id = 0
+    id = VectorID(0)
     record = Record.random(dimension=128)
     collection.update(id, record)
 
     assert collection.contains(id)
     assert collection.get(id).data == record.data
 
 
 def test_search_record():
     collection = create_test_collection()
-    vector = Vector.random(dimension=DIMENSION).to_list()
+    collection.relevancy = 4.5
+
+    vector = Vector.random(dimension=DIMENSION)
     n = 10
 
     # Search for approximate neighbors and true neighbors.
     results = collection.search(vector, n=n)
     true_results = collection.true_search(vector, n=n)
 
     assert len(results) == n
     assert len(true_results) == n
 
     # Make sure the first result of the approximate search
     # is somewhere in the true results.
     assert results[0].id in [true.id for true in true_results]
 
+    # Check if the result distances are within the relevancy.
+    assert results[-1].distance <= collection.relevancy
+    assert true_results[-1].distance <= collection.relevancy
+
 
 def test_set_dimension():
     config = Config.create_default()
     collection = Collection(config=config)
 
     # Set the collection dimension to 100.
-    collection.set_dimension(100)
-    assert collection.dimension() == 100
+    collection.dimension = 100
 
     # When inserting a record with a different dimension,
     # the collection should raise an exception.
     try:
         record = Record.random(dimension=128)
         collection.insert(record)
         assert False
     except Exception as e:
         assert "invalid vector dimension" in str(e).lower()
+
+
+def test_list_records():
+    collection = create_test_collection()
+    records = collection.list()
+
+    assert len(records) == collection.len()
+    assert all(isinstance(k, VectorID) for k in records.keys())
+    assert all(isinstance(v, Record) for v in records.values())
```

### Comparing `oasysdb-0.3.0a1/py/tests/test_database.py` & `oasysdb-0.4.0/py/tests/test_database.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,9 +1,8 @@
-from oasysdb.database import Database
-from oasysdb.collection import Record, Collection, Config
+from oasysdb.prelude import Record, Collection, Config, Database
 
 
 NAME = "vectors"  # Initial collection name.
 DIMENSION = 128
 LEN = 100
 
 
@@ -11,15 +10,19 @@
     """Creates a new test database with an initial collection."""
 
     db = Database.new(path)
     assert db.is_empty()
 
     # Create a test collection with random records.
     records = Record.many_random(dimension=DIMENSION, len=LEN)
-    db.create_collection(name=NAME, records=records)
+    config = Config.create_default()
+    collection = Collection.from_records(config, records)
+
+    # Save the collection to the database.
+    db.save_collection(name=NAME, collection=collection)
     assert not db.is_empty()
 
     return db
 
 
 def test_open():
     db = Database(path="data/101")
```

### Comparing `oasysdb-0.3.0a1/readme.md` & `oasysdb-0.4.0/readme.md`

 * *Files 4% similar despite different names*

```diff
@@ -37,23 +37,31 @@
 use oasysdb::prelude::*;
 
 fn main() {
     // Vector dimension must be uniform.
     let dimension = 128;
 
     // Replace with your own data.
-    let records = Some(Record::many_random(dimension, 100));
-    let query = Vector::random(dimension);
+    let records = Record::many_random(dimension, 100);
+
+    let mut config = Config::default();
+
+    // Optionally set the distance function. Default to Euclidean.
+    config.distance = Distance::Cosine;
+
+    // Create a vector collection.
+    let collection = Collection::build(&config, &records).unwrap();
 
-    // Open the database and create a collection.
-    let mut db = Database::open("data/test").unwrap();
-    let collection = db.create_collection("vectors", None, records).unwrap();
+    // Optionally save the collection to persist it.
+    let mut db = Database::new("data/test").unwrap();
+    db.save_collection("vectors", &collection).unwrap();
 
     // Search for the nearest neighbors.
-    let result = collection.search(query.into(), 5).unwrap();
+    let query = Vector::random(dimension);
+    let result = collection.search(&query, 5).unwrap();
     println!("Nearest ID: {}", result[0].id);
 }
 ```
 
 ## Dealing with Metadata
 
 In OasysDB, you can store additional metadata for each vector which is useful to associate the vectors with other data. The code snippet below shows how to insert the `Metadata` to the `Record` or extract it.
@@ -61,15 +69,15 @@
 ```rust
 use oasysdb::prelude::*;
 
 fn main() {
     // Inserting a metadata value into a record.
     let data: &str = "This is an example.";
     let vector = Vector::random(128);
-    let record = Record::new(vector, data.into());
+    let record = Record::new(&vector, &data.into());
 
     // Extracting the metadata value.
     let metadata = record.data.clone();
     let data = match metadata {
         Metadata::Text(value) => value,
         _ => panic!("Data is not a text."),
     };
@@ -85,44 +93,43 @@
 ```bash
 pip install oasysdb
 ```
 
 This command will install the latest version of OasysDB to your Python environment. After you're all set with the installation, you can use the code snippet below as a reference to get started with OasysDB in Python.
 
 ```python
-from oasysdb.collection import Collection, Config, Record
-from oasysdb.database import Database
-from oasysdb.vector import Vector
+from oasysdb.prelude import *
 
 
-def main():
+if __name__ == "__main__":
     # Open the database.
     db = Database("data/example")
 
+    # Replace with your own records.
+    records = Record.many_random(dimension=128, len=100)
+
     # Create a vector collection.
     config = Config.create_default()
-    records = Record.many_random(dimension=128, len=100)
-    collection = Collection.build(config, records)
+    collection = Collection.from_records(config, records)
 
     # Optionally, persist the collection to the database.
     db.save_collection("my_collection", collection)
 
-    # Search for the nearest neighbors.
     # Replace with your own query.
-    query = Vector.random(128).to_list()
+    query = Vector.random(128)
+
+    # Search for the nearest neighbors.
     result = collection.search(query, n=5)
 
     # Print the result.
     print("Nearest neighbors ID: {}".format(result[0].id))
-
-
-if __name__ == "__main__":
-    main()
 ```
 
+If you want to learn more about using OasysDB for real-world applications, you can check out the this Google Colab notebook which demonstrates how to use OasysDB to build a simple image similarity search engine: [Image Search Engine with OasysDB](https://colab.research.google.com/drive/15_1hH7jGKzMeQ6IfnScjsc-iJRL5XyL7?usp=sharing)
+
 # 🎯 Benchmarks
 
 OasysDB uses a built-in benchmarking suite using Rust's [Criterion](https://docs.rs/criterion) crate which we use to measure the performance of the vector database.
 
 Currently, the benchmarks are focused on the performance of the collection's vector search functionality. We are working on adding more benchmarks to measure the performance of other operations.
 
 If you are curious and want to run the benchmarks, you can use the following command which will download the benchmarking dataset and run the benchmarks:
```

### Comparing `oasysdb-0.3.0a1/src/db/database.rs` & `oasysdb-0.4.0/src/db/database.rs`

 * *Files 14% similar despite different names*

```diff
@@ -32,42 +32,14 @@
     #[new]
     pub fn open(path: &str) -> Result<Self, Error> {
         let collections = sled::open(path)?;
         let count = collections.len();
         Ok(Self { collections, count })
     }
 
-    /// Creates a new collection in the database.
-    /// * `name` - Name of the collection.
-    /// * `config` - Collection configuration. Uses default if none.
-    /// * `records` - Vector records to insert into the collection.
-    pub fn create_collection(
-        &mut self,
-        name: &str,
-        config: Option<Config>,
-        records: Option<Vec<Record>>,
-    ) -> Result<Collection, Error> {
-        // This prevents the variable from being dropped.
-        let default_config = Config::default();
-
-        let config = match config {
-            Some(config) => config,
-            None => default_config,
-        };
-
-        // Create new or build a collection.
-        let collection = match records {
-            Some(records) => Collection::build(config, records)?,
-            None => Collection::new(config),
-        };
-
-        self.save_collection(name, &collection)?;
-        Ok(collection)
-    }
-
     /// Gets a collection from the database.
     /// * `name` - Name of the collection.
     pub fn get_collection(&self, name: &str) -> Result<Collection, Error> {
         let value = self.collections.get(name)?;
         match value {
             Some(value) => Ok(bincode::deserialize(&value)?),
             None => Err(Error::collection_not_found()),
```

### Comparing `oasysdb-0.3.0a1/src/func/collection.rs` & `oasysdb-0.4.0/src/func/collection.rs`

 * *Files 12% similar despite different names*

```diff
@@ -1,33 +1,50 @@
 use super::*;
 
 /// The collection HNSW index configuration.
 #[pyclass(module = "oasysdb.collection")]
-#[derive(Debug, Serialize, Deserialize, Clone, Copy)]
+#[derive(Debug, Serialize, Deserialize, Clone)]
 pub struct Config {
     /// Nodes to consider during construction.
     #[pyo3(get, set)]
     pub ef_construction: usize,
     /// Nodes to consider during search.
     #[pyo3(get, set)]
     pub ef_search: usize,
     /// Layer multiplier. The optimal value is `1/ln(M)`.
     #[pyo3(get, set)]
     pub ml: f32,
+    /// Distance calculation function.
+    #[pyo3(get)]
+    pub distance: Distance,
 }
 
 // Any modifications to this methods should be reflected in:
 // - py/tests/test_collection.py
 // - py/oasysdb/collection.pyi
 #[pymethods]
 impl Config {
     /// Creates a new collection config with the given parameters.
     #[new]
-    pub fn new(ef_construction: usize, ef_search: usize, ml: f32) -> Self {
-        Self { ef_construction, ef_search, ml }
+    pub fn new(
+        ef_construction: usize,
+        ef_search: usize,
+        ml: f32,
+        distance: &str,
+    ) -> Result<Self, Error> {
+        let distance = Distance::from(distance)?;
+        Ok(Self { ef_construction, ef_search, ml, distance })
+    }
+
+    /// Sets the distance calculation function.
+    /// * `distance`: Distance function, e.g. euclidean or dot.
+    #[setter]
+    pub fn set_distance(&mut self, distance: &str) -> Result<(), Error> {
+        self.distance = Distance::from(distance)?;
+        Ok(())
     }
 
     #[staticmethod]
     fn create_default() -> Self {
         Self::default()
     }
 
@@ -37,111 +54,35 @@
 }
 
 impl Default for Config {
     /// Default configuration for the collection index.
     /// * `ef_construction`: 40
     /// * `ef_search`: 15
     /// * `ml`: 0.3
+    /// * `distance`: euclidean
     fn default() -> Self {
-        Self { ef_construction: 40, ef_search: 15, ml: 0.3 }
-    }
-}
-
-struct IndexConstruction<'a> {
-    search_pool: SearchPool,
-    top_layer: LayerID,
-    base_layer: &'a [RwLock<BaseNode>],
-    vectors: &'a HashMap<VectorID, Vector>,
-    config: &'a Config,
-}
-
-impl<'a> IndexConstruction<'a> {
-    /// Inserts a vector ID into a layer.
-    /// * `vector_id`: Vector ID to insert.
-    /// * `layer`: Layer to insert into.
-    /// * `layers`: Upper layers.
-    fn insert(
-        &self,
-        vector_id: &VectorID,
-        layer: &LayerID,
-        layers: &[Vec<UpperNode>],
-    ) {
-        let vector = &self.vectors[vector_id];
-
-        let (mut search, mut insertion) = self.search_pool.pop();
-        insertion.ef = self.config.ef_construction;
-
-        // Find the first valid vector ID to push.
-        let validator = |i: usize| self.vectors.get(&i.into()).is_some();
-        let valid_id = (0..self.vectors.len())
-            .into_par_iter()
-            .find_first(|i| validator(*i))
-            .unwrap();
-
-        search.reset();
-        search.push(&valid_id.into(), vector, self.vectors);
-
-        for current_layer in self.top_layer.descend() {
-            if current_layer <= *layer {
-                search.ef = self.config.ef_construction;
-            }
-
-            // Find the nearest neighbor candidates.
-            if current_layer > *layer {
-                let layer = layers[current_layer.0 - 1].as_slice();
-                search.search(layer, vector, self.vectors, M);
-                search.cull();
-            } else {
-                search.search(self.base_layer, vector, self.vectors, M * 2);
-                break;
-            }
-        }
-
-        // Select the neighbors.
-        let candidates = {
-            let candidates = search.select_simple();
-            &candidates[..Ord::min(candidates.len(), M)]
-        };
-
-        for (i, candidate) in candidates.iter().enumerate() {
-            let vid = candidate.vector_id;
-            let old = &self.vectors[&vid];
-            let distance = candidate.distance;
-
-            // Function to sort the vectors by distance.
-            let ordering = |id: &VectorID| {
-                if !id.is_valid() {
-                    Ordering::Greater
-                } else {
-                    let other = &self.vectors[id];
-                    distance.cmp(&old.distance(other).into())
-                }
-            };
-
-            // Find the correct index to insert at to keep the order.
-            let index = self.base_layer[&vid]
-                .read()
-                .binary_search_by(ordering)
-                .unwrap_or_else(|error| error);
-
-            self.base_layer[&vid].write().insert(index, vector_id);
-            self.base_layer[vector_id].write().set(i, vector_id);
+        Self {
+            ef_construction: 40,
+            ef_search: 15,
+            ml: 0.3,
+            distance: Distance::Euclidean,
         }
-
-        self.search_pool.push(&(search, insertion));
     }
 }
 
 /// The collection of vector records with HNSW indexing.
 #[pyclass(module = "oasysdb.collection")]
 #[derive(Debug, Serialize, Deserialize, Clone)]
 pub struct Collection {
     /// The collection configuration object.
     #[pyo3(get)]
     pub config: Config,
+    /// The min/max distance to consider a neighbor.
+    #[pyo3(get)]
+    pub relevancy: f32,
     // Private fields below.
     data: HashMap<VectorID, Metadata>,
     vectors: HashMap<VectorID, Vector>,
     slots: Vec<VectorID>,
     base_layer: Vec<BaseNode>,
     upper_layers: Vec<Vec<UpperNode>>,
     // Utility fields.
@@ -160,169 +101,48 @@
 // Any modifications to these methods should be reflected in:
 // - py/tests/test_collection.py
 // - py/oasysdb/collection.pyi
 #[pymethods]
 impl Collection {
     /// Creates an empty collection with the given configuration.
     #[new]
-    pub fn new(config: Config) -> Self {
+    pub fn new(config: &Config) -> Self {
         Self {
-            config,
             count: 0,
             dimension: 0,
+            relevancy: -1.0,
+            config: config.clone(),
             data: HashMap::new(),
             vectors: HashMap::new(),
             slots: vec![],
             base_layer: vec![],
             upper_layers: vec![],
         }
     }
 
     #[staticmethod]
-    /// Builds the collection index from vector records.
-    /// * `config`: Collection configuration.
-    /// * `records`: List of vectors to build the index from.
-    pub fn build(config: Config, records: Vec<Record>) -> Result<Self, Error> {
-        if records.is_empty() {
-            return Ok(Self::new(config));
-        }
-
-        // Ensure the number of records is within the limit.
-        if records.len() >= u32::MAX as usize {
-            let message = format!(
-                "The collection record limit is {}. Given: {}",
-                u32::MAX,
-                records.len()
-            );
-
-            return Err(message.into());
-        }
-
-        // Ensure that the vector dimension is consistent.
-        let dimension = records[0].vector.len();
-        if records.par_iter().any(|i| i.vector.len() != dimension) {
-            let message = format!(
-                "The vector dimension is inconsistent. Expected: {}.",
-                dimension
-            );
-
-            return Err(message.into());
-        }
-
-        // Find the number of layers.
-
-        let mut len = records.len();
-        let mut layers = Vec::new();
-
-        loop {
-            let next = (len as f32 * config.ml) as usize;
-
-            if next < M {
-                break;
-            }
-
-            layers.push((len - next, len));
-            len = next;
-        }
-
-        layers.push((len, len));
-        layers.reverse();
-
-        let num_layers = layers.len();
-        let top_layer = LayerID(num_layers - 1);
-
-        // Give all vectors a random layer and sort the list of nodes
-        // by descending order for construction.
-
-        // This allows us to copy higher layers to lower layers as
-        // construction progresses, while preserving randomness in
-        // each point's layer and insertion order.
-
-        let vectors = records
-            .par_iter()
-            .enumerate()
-            .map(|(i, item)| (i.into(), item.vector.clone()))
-            .collect::<HashMap<VectorID, Vector>>();
-
-        // Figure out how many nodes will go on each layer.
-        // This helps us allocate memory capacity for each
-        // layer in advance, and also helps enable batch
-        // insertion of points.
-
-        let mut ranges = Vec::with_capacity(top_layer.0);
-        for (i, (size, cumulative)) in layers.into_iter().enumerate() {
-            let start = cumulative - size;
-            let layer_id = LayerID(num_layers - i - 1);
-            let value = max(start, 1)..cumulative;
-            ranges.push((layer_id, value));
-        }
-
-        // Create index constructor.
-
-        let search_pool = SearchPool::new(vectors.len());
-        let mut upper_layers = vec![vec![]; top_layer.0];
-        let base_layer = vectors
-            .par_iter()
-            .map(|_| RwLock::new(BaseNode::default()))
-            .collect::<Vec<_>>();
-
-        let state = IndexConstruction {
-            base_layer: &base_layer,
-            search_pool,
-            top_layer,
-            vectors: &vectors,
-            config: &config,
-        };
-
-        // Initialize data for layers.
-
-        for (layer, range) in ranges {
-            let end = range.end;
-
-            range.into_par_iter().for_each(|i: usize| {
-                state.insert(&i.into(), &layer, &upper_layers)
-            });
-
-            // Copy the base layer state to the upper layer.
-            if !layer.is_zero() {
-                (&state.base_layer[..end])
-                    .into_par_iter()
-                    .map(|zero| UpperNode::from_zero(&zero.read()))
-                    .collect_into_vec(&mut upper_layers[layer.0 - 1]);
-            }
-        }
-
-        let data = records
-            .iter()
-            .enumerate()
-            .map(|(i, item)| (i.into(), item.data.clone()))
-            .collect();
-
-        // Unwrap the base nodes for the base layer.
-        let base_iter = base_layer.into_par_iter();
-        let base_layer = base_iter.map(|node| node.into_inner()).collect();
-
-        // Add IDs to the slots.
-        let slots = (0..vectors.len()).map(|i| i.into()).collect();
+    fn from_records(
+        config: &Config,
+        records: Vec<Record>,
+    ) -> Result<Self, Error> {
+        Self::build(config, &records)
+    }
 
-        Ok(Self {
-            data,
-            vectors,
-            base_layer,
-            upper_layers,
-            slots,
-            dimension,
-            config,
-            count: records.len(),
-        })
+    #[staticmethod]
+    #[pyo3(name = "build")]
+    fn py_build(
+        config: &Config,
+        records: Vec<Record>,
+    ) -> Result<Collection, Error> {
+        Self::build(config, &records)
     }
 
     /// Inserts a vector record into the collection.
     /// * `record`: Vector record to insert.
-    pub fn insert(&mut self, record: Record) -> Result<(), Error> {
+    pub fn insert(&mut self, record: &Record) -> Result<(), Error> {
         // Ensure the number of records is within the limit.
         if self.slots.len() == u32::MAX as usize {
             return Err(Error::collection_limit());
         }
 
         // Ensure the vector dimension matches the collection config.
         // If it's the first record, set the dimension.
@@ -345,271 +165,536 @@
         self.slots.push(id);
 
         // Update the collection count.
         self.count += 1;
 
         // This operation is last because it depends on
         // the updated vectors data.
-        self.insert_to_layers(id.0 as usize);
+        self.insert_to_layers(&[id]);
 
         Ok(())
     }
 
+    #[pyo3(name = "insert_many")]
+    fn py_insert_many(
+        &mut self,
+        records: Vec<Record>,
+    ) -> Result<Vec<VectorID>, Error> {
+        let ids = self.insert_many(&records)?;
+        Ok(ids)
+    }
+
     /// Deletes a vector record from the collection.
     /// * `id`: Vector ID to delete.
-    pub fn delete(&mut self, id: usize) -> Result<(), Error> {
+    pub fn delete(&mut self, id: &VectorID) -> Result<(), Error> {
         // Ensure the vector ID exists in the collection.
         if !self.contains(id) {
             return Err(Error::record_not_found());
         }
 
-        self.delete_from_layers(id);
+        self.delete_from_layers(&[*id]);
 
         // Update the collection data.
-        let vector_id = VectorID(id as u32);
-        self.vectors.remove(&vector_id);
-        self.data.remove(&vector_id);
+        self.vectors.remove(id);
+        self.data.remove(id);
 
         // Make the slot invalid so it won't be used again.
-        self.slots[id] = INVALID;
+        self.slots[id.0 as usize] = INVALID;
 
         // Update the collection count.
         self.count -= 1;
 
         Ok(())
     }
 
+    /// Returns vector records in the collection as a HashMap.
+    pub fn list(&self) -> Result<HashMap<VectorID, Record>, Error> {
+        // Early return if the collection is empty.
+        if self.vectors.is_empty() {
+            return Ok(HashMap::new());
+        }
+
+        // Map the vectors to a hashmap of records.
+        let mapper = |(id, vector): (&VectorID, &Vector)| {
+            let data = self.data[id].clone();
+            let record = Record::new(vector, &data);
+            (*id, record)
+        };
+
+        let records = self.vectors.par_iter().map(mapper).collect();
+        Ok(records)
+    }
+
     /// Returns the vector record associated with the ID.
     /// * `id`: Vector ID to retrieve.
-    pub fn get(&self, id: usize) -> Result<Record, Error> {
+    pub fn get(&self, id: &VectorID) -> Result<Record, Error> {
         if !self.contains(id) {
             return Err(Error::record_not_found());
         }
 
-        let vector_id = VectorID(id as u32);
-        let vector = self.vectors[&vector_id].clone();
-        let data = self.data[&vector_id].clone();
-        Ok(Record::new(vector, data))
+        let vector = self.vectors[id].clone();
+        let data = self.data[id].clone();
+        Ok(Record::new(&vector, &data))
     }
 
     /// Updates a vector record in the collection.
     /// * `id`: Vector ID to update.
     /// * `record`: New vector record.
-    pub fn update(&mut self, id: usize, record: Record) -> Result<(), Error> {
+    pub fn update(
+        &mut self,
+        id: &VectorID,
+        record: &Record,
+    ) -> Result<(), Error> {
         if !self.contains(id) {
             return Err(Error::record_not_found());
         }
 
         // Validate the new vector dimension.
         self.validate_dimension(&record.vector)?;
 
         // Remove the old vector from the index layers.
-        self.delete_from_layers(id);
+        self.delete_from_layers(&[*id]);
 
         // Insert the updated vector and data.
-        let vector_id = VectorID(id as u32);
-        self.vectors.insert(vector_id, record.vector.clone());
-        self.data.insert(vector_id, record.data.clone());
-        self.insert_to_layers(id);
+        self.vectors.insert(*id, record.vector.clone());
+        self.data.insert(*id, record.data.clone());
+        self.insert_to_layers(&[*id]);
 
         Ok(())
     }
 
     /// Searches the collection for the nearest neighbors.
     /// * `vector`: Vector to search.
     /// * `n`: Number of neighbors to return.
     pub fn search(
         &self,
-        vector: Vec<f32>,
+        vector: &Vector,
         n: usize,
     ) -> Result<Vec<SearchResult>, Error> {
-        let vector = Vector(vector);
         let mut search = Search::default();
 
         // Early return if the collection is empty.
         if self.vectors.is_empty() {
             return Ok(vec![]);
         }
 
         // Ensure the vector dimension matches the collection dimension.
-        self.validate_dimension(&vector)?;
+        self.validate_dimension(vector)?;
 
         // Find the first valid vector ID from the slots.
         let slots_iter = self.slots.as_slice().into_par_iter();
         let vector_id = match slots_iter.find_first(|id| id.is_valid()) {
             Some(id) => id,
             None => return Err("Unable to initiate search.".into()),
         };
 
         search.visited.resize_capacity(self.vectors.len());
-        search.push(vector_id, &vector, &self.vectors);
+        search.push(vector_id, vector, &self.vectors);
 
         for layer in LayerID(self.upper_layers.len()).descend() {
             search.ef = if layer.is_zero() { self.config.ef_search } else { 5 };
 
             if layer.0 == 0 {
                 let layer = self.base_layer.as_slice();
-                search.search(layer, &vector, &self.vectors, M * 2);
+                search.search(layer, vector, &self.vectors, M * 2);
             } else {
                 let layer = self.upper_layers[layer.0 - 1].as_slice();
-                search.search(layer, &vector, &self.vectors, M);
+                search.search(layer, vector, &self.vectors, M);
             }
 
             if !layer.is_zero() {
                 search.cull();
             }
         }
 
         let map_result = |candidate: Candidate| {
             let id = candidate.vector_id.0;
             let distance = candidate.distance.0;
             let data = self.data[&candidate.vector_id].clone();
             SearchResult { id, distance, data }
         };
 
-        Ok(search.iter().map(map_result).take(n).collect())
+        // Get relevant results and truncate the list.
+        let res = search.iter().map(map_result).collect();
+        let mut relevant = self.truncate_irrelevant_result(res);
+        relevant.truncate(n);
+        Ok(relevant)
     }
 
     /// Searches the collection for the true nearest neighbors.
     /// * `vector`: Vector to search.
     /// * `n`: Number of neighbors to return.
     pub fn true_search(
         &self,
-        vector: Vec<f32>,
+        vector: &Vector,
         n: usize,
     ) -> Result<Vec<SearchResult>, Error> {
-        let vector = Vector(vector);
         let mut nearest = Vec::with_capacity(self.vectors.len());
 
         // Ensure the vector dimension matches the collection dimension.
-        self.validate_dimension(&vector)?;
+        self.validate_dimension(vector)?;
 
         // Calculate the distance between the query and each record.
         // Then, create a search result for each record.
         for (id, vec) in self.vectors.iter() {
-            let distance = vector.distance(vec);
+            let distance = self.config.distance.calculate(vector, vec);
             let data = self.data[id].clone();
             let res = SearchResult { id: id.0, distance, data };
             nearest.push(res);
         }
 
         // Sort the nearest neighbors by distance.
         nearest.sort_by(|a, b| a.distance.partial_cmp(&b.distance).unwrap());
-        nearest.truncate(n);
-        Ok(nearest)
+
+        // Remove irrelevant results and truncate the list.
+        let mut res = self.truncate_irrelevant_result(nearest);
+        res.truncate(n);
+        Ok(res)
     }
 
     /// Returns the configured vector dimension of the collection.
+    #[getter]
     pub fn dimension(&self) -> usize {
         self.dimension
     }
 
     /// Sets the vector dimension of the collection.
     /// * `dimension`: New vector dimension.
+    #[setter]
     pub fn set_dimension(&mut self, dimension: usize) -> Result<(), Error> {
         // This can only be set if the collection is empty.
         if !self.vectors.is_empty() {
             return Err("The collection must be empty.".into());
         }
 
         self.dimension = dimension;
         Ok(())
     }
 
+    /// Sets the min/max relevancy for the search results.
+    /// * `relevancy`: Relevancy score.
+    #[setter]
+    pub fn set_relevancy(&mut self, relevancy: f32) {
+        self.relevancy = relevancy;
+    }
+
     /// Returns the number of vector records in the collection.
     pub fn len(&self) -> usize {
         self.count
     }
 
     /// Returns true if the collection is empty.
     pub fn is_empty(&self) -> bool {
         self.count == 0
     }
 
     /// Checks if the collection contains a vector ID.
     /// * `id`: Vector ID to check.
-    pub fn contains(&self, id: usize) -> bool {
-        self.vectors.contains_key(&id.into())
+    pub fn contains(&self, id: &VectorID) -> bool {
+        self.vectors.contains_key(id)
     }
 
     fn __len__(&self) -> usize {
         self.len()
     }
 }
 
 impl Collection {
+    /// Builds the collection index from vector records.
+    /// * `config`: Collection configuration.
+    /// * `records`: List of vectors to build the index from.
+    pub fn build(config: &Config, records: &[Record]) -> Result<Self, Error> {
+        if records.is_empty() {
+            return Ok(Self::new(config));
+        }
+
+        // Ensure the number of records is within the limit.
+        if records.len() >= u32::MAX as usize {
+            let message = format!(
+                "The collection record limit is {}. Given: {}",
+                u32::MAX,
+                records.len()
+            );
+
+            return Err(message.into());
+        }
+
+        // Ensure that the vector dimension is consistent.
+        let dimension = records[0].vector.len();
+        if records.par_iter().any(|i| i.vector.len() != dimension) {
+            let message = format!(
+                "The vector dimension is inconsistent. Expected: {}.",
+                dimension
+            );
+
+            return Err(message.into());
+        }
+
+        // Find the number of layers.
+
+        let mut len = records.len();
+        let mut layers = Vec::new();
+
+        loop {
+            let next = (len as f32 * config.ml) as usize;
+
+            if next < M {
+                break;
+            }
+
+            layers.push((len - next, len));
+            len = next;
+        }
+
+        layers.push((len, len));
+        layers.reverse();
+
+        let num_layers = layers.len();
+        let top_layer = LayerID(num_layers - 1);
+
+        // Give all vectors a random layer and sort the list of nodes
+        // by descending order for construction.
+
+        // This allows us to copy higher layers to lower layers as
+        // construction progresses, while preserving randomness in
+        // each point's layer and insertion order.
+
+        let vectors = records
+            .par_iter()
+            .enumerate()
+            .map(|(i, item)| (i.into(), item.vector.clone()))
+            .collect::<HashMap<VectorID, Vector>>();
+
+        // Figure out how many nodes will go on each layer.
+        // This helps us allocate memory capacity for each
+        // layer in advance, and also helps enable batch
+        // insertion of points.
+
+        let mut ranges = Vec::with_capacity(top_layer.0);
+        for (i, (size, cumulative)) in layers.into_iter().enumerate() {
+            let start = cumulative - size;
+            let layer_id = LayerID(num_layers - i - 1);
+            let value = max(start, 1)..cumulative;
+            ranges.push((layer_id, value));
+        }
+
+        // Create index constructor.
+
+        let search_pool = SearchPool::new(vectors.len());
+        let mut upper_layers = vec![vec![]; top_layer.0];
+        let base_layer = vectors
+            .par_iter()
+            .map(|_| RwLock::new(BaseNode::default()))
+            .collect::<Vec<_>>();
+
+        let state = IndexConstruction {
+            base_layer: &base_layer,
+            search_pool,
+            top_layer,
+            vectors: &vectors,
+            config,
+        };
+
+        // Initialize data for layers.
+
+        for (layer, range) in ranges {
+            let end = range.end;
+
+            range.into_par_iter().for_each(|i: usize| {
+                state.insert(&i.into(), &layer, &upper_layers)
+            });
+
+            // Copy the base layer state to the upper layer.
+            if !layer.is_zero() {
+                (&state.base_layer[..end])
+                    .into_par_iter()
+                    .map(|zero| UpperNode::from_zero(&zero.read()))
+                    .collect_into_vec(&mut upper_layers[layer.0 - 1]);
+            }
+        }
+
+        let data = records
+            .iter()
+            .enumerate()
+            .map(|(i, item)| (i.into(), item.data.clone()))
+            .collect();
+
+        // Unwrap the base nodes for the base layer.
+        let base_iter = base_layer.into_par_iter();
+        let base_layer = base_iter.map(|node| node.into_inner()).collect();
+
+        // Add IDs to the slots.
+        let slots = (0..vectors.len()).map(|i| i.into()).collect();
+
+        Ok(Self {
+            data,
+            vectors,
+            base_layer,
+            upper_layers,
+            slots,
+            dimension,
+            config: config.clone(),
+            count: records.len(),
+            relevancy: -1.0,
+        })
+    }
+
+    /// Inserts multiple vector records into the collection.
+    /// * `records`: List of vector records to insert.
+    pub fn insert_many(
+        &mut self,
+        records: &[Record],
+    ) -> Result<Vec<VectorID>, Error> {
+        // Make sure the collection is not full after inserting.
+        if self.slots.len() + records.len() >= u32::MAX as usize {
+            return Err(Error::collection_limit());
+        }
+
+        // Sets the collection dimension if it's the first record.
+        if self.vectors.is_empty() && self.dimension == 0 {
+            self.dimension = records[0].vector.len();
+        }
+
+        // Validate the vector dimension against the collection.
+        if records.par_iter().any(|i| i.vector.len() != self.dimension) {
+            let message = format!(
+                "The vector dimension is inconsistent. Expected: {}.",
+                self.dimension
+            );
+
+            return Err(message.into());
+        }
+
+        // Create new vector IDs for the records.
+        let ids: Vec<VectorID> = {
+            let first_id = self.slots.len();
+            let final_id = self.slots.len() + records.len();
+            (first_id..final_id).map(|i| i.into()).collect()
+        };
+
+        // Store the new records vector and data.
+        for (id, record) in ids.iter().zip(records.iter()) {
+            self.vectors.insert(*id, record.vector.clone());
+            self.data.insert(*id, record.data.clone());
+        }
+
+        // Add new vector IDs to the slots.
+        self.slots.extend(ids.clone());
+
+        // Update the collection count.
+        self.count += records.len();
+
+        self.insert_to_layers(&ids);
+        Ok(ids)
+    }
+
     /// Validates a vector dimension against the collection's.
     fn validate_dimension(&self, vector: &Vector) -> Result<(), Error> {
         let found = vector.len();
         let expected = self.dimension;
 
         if found != expected {
             Err(Error::invalid_dimension(found, expected))
         } else {
             Ok(())
         }
     }
 
-    /// Inserts a vector ID into the index layers.
-    fn insert_to_layers(&mut self, id: usize) {
-        self.base_layer.push(BaseNode::default());
+    /// Inserts vector IDs into the index layers.
+    fn insert_to_layers(&mut self, ids: &[VectorID]) {
+        // Add new nodes to the base layer.
+        for _ in 0..ids.len() {
+            self.base_layer.push(BaseNode::default());
+        }
 
         let base_layer = self
             .base_layer
             .par_iter()
             .map(|node| RwLock::new(*node))
             .collect::<Vec<_>>();
 
         let top_layer = match self.upper_layers.is_empty() {
             true => LayerID(0),
             false => LayerID(self.upper_layers.len()),
         };
 
+        // Create a new index construction state.
         let state = IndexConstruction {
             base_layer: base_layer.as_slice(),
             search_pool: SearchPool::new(self.vectors.len()),
             top_layer,
             vectors: &self.vectors,
             config: &self.config,
         };
 
-        // Insert new vector into the contructor.
-        state.insert(&id.into(), &top_layer, &self.upper_layers);
+        // Insert all vectors into the state.
+        for id in ids {
+            state.insert(id, &top_layer, &self.upper_layers);
+        }
 
-        // Update the base layer with the new state.
+        // Update base layer using the new state.
         let iter = state.base_layer.into_par_iter();
         self.base_layer = iter.map(|node| *node.read()).collect();
     }
 
-    /// Removes a vector ID from all index layers.
-    fn delete_from_layers(&mut self, id: usize) {
-        let vector_id = VectorID(id as u32);
-
-        // Remove the vector from the base layer.
-        let base_node = &mut self.base_layer[id];
-        let index = base_node.par_iter().position_first(|x| *x == vector_id);
-        if let Some(index) = index {
-            base_node.set(index, &INVALID);
+    /// Removes vector IDs from all index layers.
+    fn delete_from_layers(&mut self, ids: &[VectorID]) {
+        // Remove the vectors from the base layer.
+        for id in ids {
+            let base_node = &mut self.base_layer[id.0 as usize];
+            let index = base_node.par_iter().position_first(|x| *x == *id);
+            if let Some(index) = index {
+                base_node.set(index, &INVALID);
+            }
         }
 
         // Remove the vector from the upper layers.
         for layer in LayerID(self.upper_layers.len()).descend() {
             let upper_layer = match layer.0 > 0 {
                 true => &mut self.upper_layers[layer.0 - 1],
                 false => break,
             };
 
-            let node = &mut upper_layer[id];
-            let index = node.0.par_iter().position_first(|x| *x == vector_id);
-
-            if let Some(index) = index {
-                node.set(index, &INVALID);
+            for id in ids {
+                let node = &mut upper_layer[id.0 as usize];
+                let index = node.0.par_iter().position_first(|x| *x == *id);
+                if let Some(index) = index {
+                    node.set(index, &INVALID);
+                }
             }
         }
     }
+
+    /// Truncates the search result based on the relevancy score.
+    fn truncate_irrelevant_result(
+        &self,
+        result: Vec<SearchResult>,
+    ) -> Vec<SearchResult> {
+        // Early return if the relevancy score is not set.
+        if self.relevancy == -1.0 {
+            return result;
+        }
+
+        // For Euclidean distance, relevant results are those
+        // smaller than the relevancy score with best distance of 0.0.
+        if self.config.distance == Distance::Euclidean {
+            return result
+                .into_par_iter()
+                .filter(|r| r.distance <= self.relevancy)
+                .collect();
+        }
+
+        // For other distance metrics, like cosine similarity
+        // and dot product, the relevant results are above
+        // the relevancy score.
+        result
+            .into_par_iter()
+            .filter(|r| r.distance >= self.relevancy)
+            .collect()
+    }
 }
 
 /// A record containing a vector and its associated data.
 #[pyclass(module = "oasysdb.collection")]
 #[derive(Serialize, Deserialize, Clone, Debug)]
 pub struct Record {
     /// The vector embedding.
@@ -625,24 +710,30 @@
 // - py/oasysdb/collection.pyi
 #[pymethods]
 impl Record {
     #[new]
     fn py_new(vector: Vec<f32>, data: &PyAny) -> Self {
         let vector = Vector::from(vector);
         let data = Metadata::from(data);
-        Self::new(vector, data)
+        Self::new(&vector, &data)
+    }
+
+    #[setter]
+    fn set_data(&mut self, data: &PyAny) -> Result<(), Error> {
+        self.data = Metadata::from(data);
+        Ok(())
     }
 
     /// Generates a random record for testing.
     /// * `dimension`: Vector dimension.
     #[staticmethod]
     pub fn random(dimension: usize) -> Self {
         let vector = Vector::random(dimension);
         let data = random::<usize>().into();
-        Self::new(vector, data)
+        Self::new(&vector, &data)
     }
 
     /// Generates many random records for testing.
     /// * `dimension`: Vector dimension.
     /// * `len`: Number of records to generate.
     #[staticmethod]
     pub fn many_random(dimension: usize, len: usize) -> Vec<Self> {
@@ -652,16 +743,16 @@
     fn __repr__(&self) -> String {
         format!("{:?}", self)
     }
 }
 
 impl Record {
     /// Creates a new record with a vector and data.
-    pub fn new(vector: Vector, data: Metadata) -> Self {
-        Self { vector, data }
+    pub fn new(vector: &Vector, data: &Metadata) -> Self {
+        Self { vector: vector.clone(), data: data.clone() }
     }
 }
 
 /// The collection nearest neighbor search result.
 #[pyclass(module = "oasysdb.collection")]
 #[derive(Serialize, Deserialize, Debug)]
 pub struct SearchResult {
```

### Comparing `oasysdb-0.3.0a1/src/func/err.rs` & `oasysdb-0.4.0/src/func/err.rs`

 * *Files identical despite different names*

### Comparing `oasysdb-0.3.0a1/src/func/metadata.rs` & `oasysdb-0.4.0/src/func/metadata.rs`

 * *Files identical despite different names*

### Comparing `oasysdb-0.3.0a1/src/func/mod.rs` & `oasysdb-0.4.0/src/func/mod.rs`

 * *Files 14% similar despite different names*

```diff
@@ -1,19 +1,23 @@
 /// The collection of vectors and their data.
 pub mod collection;
+/// Enum for the collection distance functions.
+pub mod distance;
 /// Error types for the database.
 pub mod err;
 /// Types for the metadata.
 pub mod metadata;
 /// Types for the vectors.
 pub mod vector;
 
 // Internal modules.
 mod utils;
 
+use collection::*;
+use distance::*;
 use err::*;
 use metadata::*;
 use utils::*;
 use vector::*;
 
 // External dependencies.
 use ordered_float::OrderedFloat;
```

### Comparing `oasysdb-0.3.0a1/src/func/utils.rs` & `oasysdb-0.4.0/src/func/utils.rs`

 * *Files 18% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+use self::distance::Distance;
+
 use super::*;
 
 pub const INVALID: VectorID = VectorID(u32::MAX);
 
 /// The M value for the HNSW algorithm.
 pub const M: usize = 32;
 
@@ -234,14 +236,15 @@
 pub struct Search {
     pub ef: usize,
     pub visited: Visited,
     candidates: BinaryHeap<Reverse<Candidate>>,
     nearest: Vec<Candidate>,
     working: Vec<Candidate>,
     discarded: Vec<Candidate>,
+    distance: Distance,
 }
 
 impl Search {
     pub fn new(capacity: usize) -> Self {
         let visited = Visited::with_capacity(capacity);
         Self { visited, ..Default::default() }
     }
@@ -280,15 +283,16 @@
     ) {
         if !self.visited.insert(vector_id) {
             return;
         }
 
         // Create a new candidate.
         let other = &vectors[vector_id];
-        let distance = OrderedFloat::from(vector.distance(other));
+        let distance = self.distance.calculate(vector, other);
+        let distance = OrderedFloat::from(distance);
         let new = Candidate { distance, vector_id: *vector_id };
 
         // Make sure the index to insert to is within the EF scope.
         let index = match self.nearest.binary_search(&new) {
             Err(index) if index < self.ef => index,
             Err(_) => return,
             Ok(_) => unreachable!(),
@@ -335,14 +339,15 @@
         Self {
             visited: Visited::with_capacity(0),
             candidates: BinaryHeap::new(),
             nearest: Vec::new(),
             working: Vec::new(),
             discarded: Vec::new(),
             ef: 5,
+            distance: Distance::Euclidean,
         }
     }
 }
 
 pub struct SearchPool {
     pool: Mutex<Vec<(Search, Search)>>,
     len: usize,
@@ -363,7 +368,93 @@
     }
 
     /// Pushes the searches to the pool.
     pub fn push(&self, item: &(Search, Search)) {
         self.pool.lock().push(item.clone());
     }
 }
+
+pub struct IndexConstruction<'a> {
+    pub search_pool: SearchPool,
+    pub top_layer: LayerID,
+    pub base_layer: &'a [RwLock<BaseNode>],
+    pub vectors: &'a HashMap<VectorID, Vector>,
+    pub config: &'a Config,
+}
+
+impl<'a> IndexConstruction<'a> {
+    /// Inserts a vector ID into a layer.
+    /// * `vector_id`: Vector ID to insert.
+    /// * `layer`: Layer to insert into.
+    /// * `layers`: Upper layers.
+    pub fn insert(
+        &self,
+        vector_id: &VectorID,
+        layer: &LayerID,
+        layers: &[Vec<UpperNode>],
+    ) {
+        let vector = &self.vectors[vector_id];
+        let dist = self.config.distance;
+
+        let (mut search, mut insertion) = self.search_pool.pop();
+        insertion.ef = self.config.ef_construction;
+
+        // Find the first valid vector ID to push.
+        let validator = |i: usize| self.vectors.get(&i.into()).is_some();
+        let valid_id = (0..self.vectors.len())
+            .into_par_iter()
+            .find_first(|i| validator(*i))
+            .unwrap();
+
+        search.reset();
+        search.push(&valid_id.into(), vector, self.vectors);
+
+        for current_layer in self.top_layer.descend() {
+            if current_layer <= *layer {
+                search.ef = self.config.ef_construction;
+            }
+
+            // Find the nearest neighbor candidates.
+            if current_layer > *layer {
+                let layer = layers[current_layer.0 - 1].as_slice();
+                search.search(layer, vector, self.vectors, M);
+                search.cull();
+            } else {
+                search.search(self.base_layer, vector, self.vectors, M * 2);
+                break;
+            }
+        }
+
+        // Select the neighbors.
+        let candidates = {
+            let candidates = search.select_simple();
+            &candidates[..Ord::min(candidates.len(), M)]
+        };
+
+        for (i, candidate) in candidates.iter().enumerate() {
+            let vid = candidate.vector_id;
+            let old = &self.vectors[&vid];
+            let distance = candidate.distance;
+
+            // Function to sort the vectors by distance.
+            let ordering = |id: &VectorID| {
+                if !id.is_valid() {
+                    Ordering::Greater
+                } else {
+                    let other = &self.vectors[id];
+                    distance.cmp(&dist.calculate(old, other).into())
+                }
+            };
+
+            // Find the correct index to insert at to keep the order.
+            let index = self.base_layer[&vid]
+                .read()
+                .binary_search_by(ordering)
+                .unwrap_or_else(|error| error);
+
+            self.base_layer[&vid].write().insert(index, vector_id);
+            self.base_layer[vector_id].write().set(i, vector_id);
+        }
+
+        self.search_pool.push(&(search, insertion));
+    }
+}
```

### Comparing `oasysdb-0.3.0a1/src/func/vector.rs` & `oasysdb-0.4.0/src/func/vector.rs`

 * *Files 22% similar despite different names*

```diff
@@ -80,23 +80,14 @@
     }
 
     fn __len__(&self) -> usize {
         self.len()
     }
 }
 
-impl Vector {
-    /// Returns the Euclidean distance between two vectors.
-    pub fn distance(&self, other: &Self) -> f32 {
-        assert_eq!(self.0.len(), other.0.len());
-        let iter = self.0.iter().zip(other.0.iter());
-        iter.map(|(a, b)| (a - b).powi(2)).sum::<f32>().sqrt()
-    }
-}
-
 impl Index<&VectorID> for [Vector] {
     type Output = Vector;
     fn index(&self, index: &VectorID) -> &Self::Output {
         &self[index.0 as usize]
     }
 }
```

### Comparing `oasysdb-0.3.0a1/src/lib.rs` & `oasysdb-0.4.0/src/lib.rs`

 * *Files 20% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 mod func;
 
 /// Convenience re-exports for the public APIs.
 pub mod prelude;
 
 pub use db::database;
 pub use func::collection;
+pub use func::distance;
 pub use func::err;
 pub use func::metadata;
 pub use func::vector;
 
 use pyo3::prelude::*;
 
 type Module = fn(Python<'_>, &PyModule) -> PyResult<()>;
@@ -27,14 +28,15 @@
     let sys = py.import("sys")?;
     let modules = sys.getattr("modules")?;
 
     let mods: Vec<(&str, Module)> = vec![
         ("collection", collection_modules),
         ("vector", vector_modules),
         ("database", database_modules),
+        ("prelude", prelude_modules),
     ];
 
     for (name, module) in mods {
         let full_name = format!("oasysdb.{}", name);
         let pymod = PyModule::new(py, &full_name)?;
         module(py, pymod)?;
         m.add(name, pymod)?;
@@ -61,7 +63,19 @@
 }
 
 #[pymodule]
 fn database_modules(_py: Python, m: &PyModule) -> PyResult<()> {
     m.add_class::<database::Database>()?;
     Ok(())
 }
+
+#[pymodule]
+fn prelude_modules(_py: Python, m: &PyModule) -> PyResult<()> {
+    m.add_class::<collection::Config>()?;
+    m.add_class::<collection::Record>()?;
+    m.add_class::<collection::Collection>()?;
+    m.add_class::<collection::SearchResult>()?;
+    m.add_class::<vector::Vector>()?;
+    m.add_class::<vector::VectorID>()?;
+    m.add_class::<database::Database>()?;
+    Ok(())
+}
```

### Comparing `oasysdb-0.3.0a1/src/tests/mod.rs` & `oasysdb-0.4.0/src/tests/mod.rs`

 * *Files 18% similar despite different names*

```diff
@@ -1,26 +1,37 @@
 mod test_collection;
 mod test_database;
+mod test_distance;
 
-use crate::collection::*;
-use crate::database::*;
-use crate::vector::*;
+use crate::prelude::*;
 use rayon::iter::*;
 use std::collections::HashMap;
 
 const DIMENSION: usize = 128;
 const LEN: usize = 100;
 
 /// The test database initial collection name.
 const NAME: &str = "vectors";
 
 fn create_test_database(path: &str) -> Database {
     let mut db = Database::new(path).unwrap();
-    let records = Record::many_random(DIMENSION, LEN);
-    db.create_collection(NAME, None, Some(records)).unwrap();
+    let collection = create_collection();
+    db.save_collection(NAME, &collection).unwrap();
     db
 }
 
-fn create_collection(records: Vec<Record>) -> Collection {
+fn create_collection() -> Collection {
+    let all_records = Record::many_random(DIMENSION, LEN);
+
+    // Split the records into two halves.
+    // The first half is used to build the collection.
+    // The second half is used to insert.
+    let mid = LEN / 2;
+    let first_half = &all_records[0..mid];
+    let second_half = &all_records[mid..LEN];
+
     let config = Config::default();
-    Collection::build(config, records).unwrap()
+    let mut collection = Collection::build(&config, first_half).unwrap();
+
+    collection.insert_many(second_half).unwrap();
+    collection
 }
```

### Comparing `oasysdb-0.3.0a1/src/tests/test_database.rs` & `oasysdb-0.4.0/src/tests/test_database.rs`

 * *Files 11% similar despite different names*

```diff
@@ -1,59 +1,58 @@
 use super::*;
 
 #[test]
 fn new() {
     let db = Database::new("data/001").unwrap();
     assert_eq!(db.len(), 0);
 }
-
 #[test]
-fn create_collection() {
-    let mut db = Database::new("data/002").unwrap();
-
-    let records = Some(Record::many_random(DIMENSION, LEN));
-    let collection = db.create_collection("test", None, records).unwrap();
-
-    assert_eq!(collection.len(), LEN);
-    assert_eq!(db.len(), 1);
+fn new_with_distance() {
+    let mut config = Config::default();
+    config.distance = Distance::Cosine;
+    let mut collection = Collection::new(&config);
+    collection.insert(&Record::random(DIMENSION)).unwrap();
 }
 
 #[test]
 fn get_collection() {
-    let db = create_test_database("data/003");
+    let db = create_test_database("data/002");
     let collection = db.get_collection(NAME).unwrap();
     assert_eq!(collection.len(), LEN);
 }
 
 #[test]
 fn save_collection_new() {
-    let mut db = Database::new("data/004").unwrap();
+    let mut db = Database::new("data/003").unwrap();
 
     // Create a collection from scratch.
     let config = Config::default();
-    let mut collection = Collection::new(config);
-    collection.insert(Record::random(DIMENSION)).unwrap();
+    let mut collection = Collection::new(&config);
+
+    // Insert a random record.
+    let record = Record::random(DIMENSION);
+    collection.insert(&record).unwrap();
 
     db.save_collection("new", &collection).unwrap();
     assert_eq!(collection.len(), 1);
     assert_eq!(db.len(), 1);
 }
 
 #[test]
 fn save_collection_update() {
-    let mut db = create_test_database("data/005");
+    let mut db = create_test_database("data/004");
 
     // Update the collection.
     let mut collection = db.get_collection(NAME).unwrap();
-    collection.insert(Record::random(DIMENSION)).unwrap();
+    collection.insert(&Record::random(DIMENSION)).unwrap();
 
     db.save_collection(NAME, &collection).unwrap();
     assert_eq!(collection.len(), LEN + 1);
     assert_eq!(db.len(), 1);
 }
 
 #[test]
 fn delete_collection() {
-    let mut db = create_test_database("data/006");
+    let mut db = create_test_database("data/005");
     db.delete_collection(NAME).unwrap();
     assert_eq!(db.len(), 0);
 }
```

### Comparing `oasysdb-0.3.0a1/pyproject.toml` & `oasysdb-0.4.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `oasysdb-0.3.0a1/PKG-INFO` & `oasysdb-0.4.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: oasysdb
-Version: 0.3.0a1
+Version: 0.4.0
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Rust
 Classifier: Topic :: Database
 Classifier: Topic :: Text Processing :: Indexing
 Summary: Fast embedded vector database with incremental HNSW indexing.
 Keywords: embedded,vector,database,hnsw,ann
@@ -56,23 +56,31 @@
 use oasysdb::prelude::*;
 
 fn main() {
     // Vector dimension must be uniform.
     let dimension = 128;
 
     // Replace with your own data.
-    let records = Some(Record::many_random(dimension, 100));
-    let query = Vector::random(dimension);
+    let records = Record::many_random(dimension, 100);
+
+    let mut config = Config::default();
+
+    // Optionally set the distance function. Default to Euclidean.
+    config.distance = Distance::Cosine;
+
+    // Create a vector collection.
+    let collection = Collection::build(&config, &records).unwrap();
 
-    // Open the database and create a collection.
-    let mut db = Database::open("data/test").unwrap();
-    let collection = db.create_collection("vectors", None, records).unwrap();
+    // Optionally save the collection to persist it.
+    let mut db = Database::new("data/test").unwrap();
+    db.save_collection("vectors", &collection).unwrap();
 
     // Search for the nearest neighbors.
-    let result = collection.search(query.into(), 5).unwrap();
+    let query = Vector::random(dimension);
+    let result = collection.search(&query, 5).unwrap();
     println!("Nearest ID: {}", result[0].id);
 }
 ```
 
 ## Dealing with Metadata
 
 In OasysDB, you can store additional metadata for each vector which is useful to associate the vectors with other data. The code snippet below shows how to insert the `Metadata` to the `Record` or extract it.
@@ -80,15 +88,15 @@
 ```rust
 use oasysdb::prelude::*;
 
 fn main() {
     // Inserting a metadata value into a record.
     let data: &str = "This is an example.";
     let vector = Vector::random(128);
-    let record = Record::new(vector, data.into());
+    let record = Record::new(&vector, &data.into());
 
     // Extracting the metadata value.
     let metadata = record.data.clone();
     let data = match metadata {
         Metadata::Text(value) => value,
         _ => panic!("Data is not a text."),
     };
@@ -104,44 +112,43 @@
 ```bash
 pip install oasysdb
 ```
 
 This command will install the latest version of OasysDB to your Python environment. After you're all set with the installation, you can use the code snippet below as a reference to get started with OasysDB in Python.
 
 ```python
-from oasysdb.collection import Collection, Config, Record
-from oasysdb.database import Database
-from oasysdb.vector import Vector
+from oasysdb.prelude import *
 
 
-def main():
+if __name__ == "__main__":
     # Open the database.
     db = Database("data/example")
 
+    # Replace with your own records.
+    records = Record.many_random(dimension=128, len=100)
+
     # Create a vector collection.
     config = Config.create_default()
-    records = Record.many_random(dimension=128, len=100)
-    collection = Collection.build(config, records)
+    collection = Collection.from_records(config, records)
 
     # Optionally, persist the collection to the database.
     db.save_collection("my_collection", collection)
 
-    # Search for the nearest neighbors.
     # Replace with your own query.
-    query = Vector.random(128).to_list()
+    query = Vector.random(128)
+
+    # Search for the nearest neighbors.
     result = collection.search(query, n=5)
 
     # Print the result.
     print("Nearest neighbors ID: {}".format(result[0].id))
-
-
-if __name__ == "__main__":
-    main()
 ```
 
+If you want to learn more about using OasysDB for real-world applications, you can check out the this Google Colab notebook which demonstrates how to use OasysDB to build a simple image similarity search engine: [Image Search Engine with OasysDB](https://colab.research.google.com/drive/15_1hH7jGKzMeQ6IfnScjsc-iJRL5XyL7?usp=sharing)
+
 # 🎯 Benchmarks
 
 OasysDB uses a built-in benchmarking suite using Rust's [Criterion](https://docs.rs/criterion) crate which we use to measure the performance of the vector database.
 
 Currently, the benchmarks are focused on the performance of the collection's vector search functionality. We are working on adding more benchmarks to measure the performance of other operations.
 
 If you are curious and want to run the benchmarks, you can use the following command which will download the benchmarking dataset and run the benchmarks:
```

