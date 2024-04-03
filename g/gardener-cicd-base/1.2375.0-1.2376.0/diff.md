# Comparing `tmp/gardener-cicd-base-1.2375.0.tar.gz` & `tmp/gardener_cicd_base-1.2376.0-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gardener-cicd-base-1.2375.0.tar", last modified: Wed Apr  3 11:35:10 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

