# Comparing `tmp/fits2rgb-0.1.1.tar.gz` & `tmp/fits2rgb-0.2.1-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fits2rgb-0.1.1.tar", last modified: Wed Apr  3 11:28:59 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

