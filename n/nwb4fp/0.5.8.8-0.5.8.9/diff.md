# Comparing `tmp/nwb4fp-0.5.8.8.tar.gz` & `tmp/nwb4fp-0.5.8.9-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nwb4fp-0.5.8.8.tar", last modified: Wed Apr  3 10:49:24 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

