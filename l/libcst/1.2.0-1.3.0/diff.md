# Comparing `tmp/libcst-1.2.0.tar.gz` & `tmp/libcst-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "libcst-1.2.0.tar", last modified: Mon Feb 19 12:48:24 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=store
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

