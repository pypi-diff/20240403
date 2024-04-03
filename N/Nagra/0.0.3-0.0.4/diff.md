# Comparing `tmp/Nagra-0.0.3.tar.gz` & `tmp/Nagra-0.0.4.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Nagra-0.0.3.tar", last modified: Thu Feb 29 13:21:29 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=store
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

