# Comparing `tmp/spotGUI-0.4.8.tar.gz` & `tmp/spotGUI-0.4.9-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spotGUI-0.4.8.tar", last modified: Sun Mar 31 08:30:03 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

