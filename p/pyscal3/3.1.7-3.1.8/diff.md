# Comparing `tmp/pyscal3-3.1.7.tar.gz` & `tmp/pyscal3-3.1.8-pp39-pypy39_pp73-manylinux_2_17_i686.manylinux2014_i686.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyscal3-3.1.7.tar", last modified: Fri Feb  2 21:27:34 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=store
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

