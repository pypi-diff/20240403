# Comparing `tmp/lmwrapper-0.8.7.2.tar.gz` & `tmp/lmwrapper-0.8.7.3-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lmwrapper-0.8.7.2.tar", last modified: Tue Apr  2 20:35:44 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

