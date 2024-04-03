# Comparing `tmp/home-assistant-intents-2024.3.6.tar.gz` & `tmp/home_assistant_intents-2024.4.3-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "home-assistant-intents-2024.3.6.tar", last modified: Wed Mar  6 17:25:48 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

