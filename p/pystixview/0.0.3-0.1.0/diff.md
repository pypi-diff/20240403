# Comparing `tmp/pystixview-0.0.3.tar.gz` & `tmp/pystixview-0.1.0-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pystixview-0.0.3.tar", last modified: Sun Mar 10 21:34:15 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

