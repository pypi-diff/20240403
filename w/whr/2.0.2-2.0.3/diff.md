# Comparing `tmp/whr-2.0.2.tar.gz` & `tmp/whr-2.0.3-cp36-cp36m-win32.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "whr-2.0.2.tar", last modified: Tue Apr  2 15:09:56 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

