# Comparing `tmp/e3-core-22.4.0.tar.gz` & `tmp/e3_core-22.5.0-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "e3-core-22.4.0.tar", last modified: Thu Jan 18 16:22:52 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

