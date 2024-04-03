# Comparing `tmp/rabbitizer-1.9.4.tar.gz` & `tmp/rabbitizer-1.9.5-cp38-cp38-musllinux_1_1_x86_64.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rabbitizer-1.9.4.tar", last modified: Mon Mar 18 19:42:16 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=store
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

