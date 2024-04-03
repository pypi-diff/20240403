# Comparing `tmp/dektools-0.1.72.tar.gz` & `tmp/dektools-0.1.9-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dektools-0.1.72.tar", last modified: Wed Apr  3 16:30:51 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

