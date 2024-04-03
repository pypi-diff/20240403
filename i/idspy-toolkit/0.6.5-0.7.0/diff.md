# Comparing `tmp/idspy_toolkit-0.6.5.tar.gz` & `tmp/idspy_toolkit-0.7.0-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "idspy_toolkit-0.6.5.tar", last modified: Mon Mar 18 15:50:03 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

