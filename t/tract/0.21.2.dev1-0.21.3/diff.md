# Comparing `tmp/tract-0.21.2.dev1.tar.gz` & `tmp/tract-0.21.3-cp311-cp311-macosx_11_0_arm64.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tract-0.21.2.dev1.tar", last modified: Mon Mar 25 17:37:59 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=store
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

