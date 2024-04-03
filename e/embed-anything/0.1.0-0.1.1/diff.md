# Comparing `tmp/embed_anything-0.1.0.tar.gz` & `tmp/embed_anything-0.1.1.tar.gz`

## Comparing `embed_anything-0.1.0.tar` & `embed_anything-0.1.1.tar`

### file list

```diff
@@ -1,12 +1,13 @@
--rw-r--r--   0        0        0      555 1970-01-01 00:00:00.000000 embed_anything-0.1.0/Cargo.toml
--rw-r--r--   0        0        0     3526 2024-03-31 23:05:19.000000 embed_anything-0.1.0/.github/workflows/CI.yml
--rw-r--r--   0        0        0      758 2024-03-31 23:05:19.000000 embed_anything-0.1.0/.gitignore
--rw-r--r--   0        0        0      346 2024-03-31 23:05:19.000000 embed_anything-0.1.0/embed_anything.pyi
--rw-r--r--   0        0        0     2850 2024-03-31 23:05:19.000000 embed_anything-0.1.0/src/embed.rs
--rw-r--r--   0        0        0     1527 2024-03-31 23:05:19.000000 embed_anything-0.1.0/src/file_embed.rs
--rw-r--r--   0        0        0      924 2024-03-31 23:05:19.000000 embed_anything-0.1.0/src/lib.rs
--rw-r--r--   0        0        0      296 2024-03-31 23:05:19.000000 embed_anything-0.1.0/src/pdf_processor.rs
--rw-r--r--   0        0        0      127 2024-03-31 23:05:19.000000 embed_anything-0.1.0/test.py
--rw-r--r--   0        0        0    42778 2024-03-31 23:05:19.000000 embed_anything-0.1.0/Cargo.lock
--rw-r--r--   0        0        0      409 2024-03-31 23:05:19.000000 embed_anything-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      263 1970-01-01 00:00:00.000000 embed_anything-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      555 1970-01-01 00:00:00.000000 embed_anything-0.1.1/Cargo.toml
+-rw-r--r--   0        0        0     3526 2024-03-31 23:05:19.000000 embed_anything-0.1.1/.github/workflows/CI.yml
+-rw-r--r--   0        0        0      758 2024-03-31 23:05:19.000000 embed_anything-0.1.1/.gitignore
+-rw-r--r--   0        0        0     1411 2024-04-03 17:03:00.000000 embed_anything-0.1.1/README.md
+-rw-r--r--   0        0        0      346 2024-03-31 23:05:19.000000 embed_anything-0.1.1/embed_anything.pyi
+-rw-r--r--   0        0        0     2850 2024-03-31 23:05:19.000000 embed_anything-0.1.1/src/embed.rs
+-rw-r--r--   0        0        0     1527 2024-03-31 23:05:19.000000 embed_anything-0.1.1/src/file_embed.rs
+-rw-r--r--   0        0        0      924 2024-03-31 23:05:19.000000 embed_anything-0.1.1/src/lib.rs
+-rw-r--r--   0        0        0      296 2024-03-31 23:05:19.000000 embed_anything-0.1.1/src/pdf_processor.rs
+-rw-r--r--   0        0        0      129 2024-04-01 21:49:59.000000 embed_anything-0.1.1/test.py
+-rw-r--r--   0        0        0    42778 2024-04-03 17:41:01.000000 embed_anything-0.1.1/Cargo.lock
+-rw-r--r--   0        0        0      571 2024-04-03 17:31:33.000000 embed_anything-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     1869 1970-01-01 00:00:00.000000 embed_anything-0.1.1/PKG-INFO
```

### Comparing `embed_anything-0.1.0/Cargo.toml` & `embed_anything-0.1.1/Cargo.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "embed_anything"
-version = "0.1.0"
+version = "0.1.1"
 edition = "2021"
 
 # See more keys and their definitions at https://doc.rust-lang.org/cargo/reference/manifest.html
 [lib]
 name = "embed_anything"
 crate-type = ["cdylib"]
```

### Comparing `embed_anything-0.1.0/.github/workflows/CI.yml` & `embed_anything-0.1.1/.github/workflows/CI.yml`

 * *Files identical despite different names*

### Comparing `embed_anything-0.1.0/.gitignore` & `embed_anything-0.1.1/.gitignore`

 * *Files identical despite different names*

### Comparing `embed_anything-0.1.0/src/embed.rs` & `embed_anything-0.1.1/src/embed.rs`

 * *Files identical despite different names*

### Comparing `embed_anything-0.1.0/src/file_embed.rs` & `embed_anything-0.1.1/src/file_embed.rs`

 * *Files identical despite different names*

### Comparing `embed_anything-0.1.0/src/lib.rs` & `embed_anything-0.1.1/src/lib.rs`

 * *Files identical despite different names*

### Comparing `embed_anything-0.1.0/Cargo.lock` & `embed_anything-0.1.1/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -121,15 +121,15 @@
 checksum = "b42b6fa04a440b495c8b04d0e71b707c585f83cb9cb28cf8cd0d976c315e31b4"
 dependencies = [
  "powerfmt",
 ]
 
 [[package]]
 name = "embed_anything"
-version = "0.1.0"
+version = "0.1.1"
 dependencies = [
  "futures",
  "pdf-extract",
  "pyo3",
  "pyo3-asyncio",
  "reqwest",
  "serde",
```

