# Comparing `tmp/pytoolbox-14.8.1.tar.gz` & `tmp/pytoolbox-14.8.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytoolbox-14.8.1.tar", last modified: Tue Apr  2 11:25:01 2024, max compression
+gzip compressed data, was "pytoolbox-14.8.2.tar", last modified: Wed Apr  3 10:21:27 2024, max compression
```

## Comparing `pytoolbox-14.8.1.tar` & `pytoolbox-14.8.2.tar`

### file list

```diff
@@ -1,222 +1,222 @@
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2024-04-02 11:25:01.357379 pytoolbox-14.8.1/
--rw-rw-r--   0 david     (1000) david     (1000)      219 2024-03-25 15:44:57.000000 pytoolbox-14.8.1/AUTHORS.md
--rw-rw-r--   0 david     (1000) david     (1000)    35196 2024-04-02 11:17:18.000000 pytoolbox-14.8.1/CHANGELOG.md
--rw-rw-r--   0 david     (1000) david     (1000)     5747 2024-03-25 15:44:57.000000 pytoolbox-14.8.1/LICENSE.rst
--rw-rw-r--   0 david     (1000) david     (1000)       27 2024-03-25 15:44:57.000000 pytoolbox-14.8.1/MANIFEST.in
--rw-r--r--   0 david     (1000) david     (1000)    11167 2024-04-02 11:25:01.357379 pytoolbox-14.8.1/PKG-INFO
--rw-rw-r--   0 david     (1000) david     (1000)     6529 2024-03-26 07:35:12.000000 pytoolbox-14.8.1/README.rst
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2024-04-02 11:25:01.257378 pytoolbox-14.8.1/pytoolbox/
--rw-rw-r--   0 david     (1000) david     (1000)      467 2024-04-02 11:17:33.000000 pytoolbox-14.8.1/pytoolbox/__init__.py
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2024-04-02 11:25:01.257378 pytoolbox-14.8.1/pytoolbox/ai/
--rw-rw-r--   0 david     (1000) david     (1000)        0 2024-03-25 15:44:57.000000 pytoolbox-14.8.1/pytoolbox/ai/__init__.py
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2024-04-02 11:25:01.261378 pytoolbox-14.8.1/pytoolbox/ai/vision/
--rw-rw-r--   0 david     (1000) david     (1000)        0 2024-03-25 15:44:57.000000 pytoolbox-14.8.1/pytoolbox/ai/vision/__init__.py
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2024-04-02 11:25:01.261378 pytoolbox-14.8.1/pytoolbox/ai/vision/face/
--rw-rw-r--   0 david     (1000) david     (1000)        0 2024-03-25 15:44:57.000000 pytoolbox-14.8.1/pytoolbox/ai/vision/face/__init__.py
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2024-04-02 11:25:01.261378 pytoolbox-14.8.1/pytoolbox/ai/vision/face/detect/
--rw-rw-r--   0 david     (1000) david     (1000)       67 2024-03-25 15:44:57.000000 pytoolbox-14.8.1/pytoolbox/ai/vision/face/detect/__init__.py
--rw-rw-r--   0 david     (1000) david     (1000)     8925 2024-03-25 15:44:57.000000 pytoolbox-14.8.1/pytoolbox/ai/vision/face/detect/dlib.py
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2024-04-02 11:25:01.261378 pytoolbox-14.8.1/pytoolbox/ai/vision/face/recognize/
--rw-rw-r--   0 david     (1000) david     (1000)       97 2024-03-25 15:44:57.000000 pytoolbox-14.8.1/pytoolbox/ai/vision/face/recognize/__init__.py
--rw-rw-r--   0 david     (1000) david     (1000)    11412 2024-03-25 15:44:57.000000 pytoolbox-14.8.1/pytoolbox/ai/vision/face/recognize/nn4_small2.py
--rw-rw-r--   0 david     (1000) david     (1000)      651 2024-03-25 15:44:57.000000 pytoolbox-14.8.1/pytoolbox/ai/vision/utils.py
--rw-rw-r--   0 david     (1000) david     (1000)     7959 2024-04-02 11:17:02.000000 pytoolbox-14.8.1/pytoolbox/argparse.py
--rw-rw-r--   0 david     (1000) david     (1000)     1738 2024-03-25 15:44:57.000000 pytoolbox-14.8.1/pytoolbox/atlassian.py
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2024-04-02 11:25:01.261378 pytoolbox-14.8.1/pytoolbox/aws/
--rw-rw-r--   0 david     (1000) david     (1000)       71 2024-03-25 15:44:57.000000 pytoolbox-14.8.1/pytoolbox/aws/__init__.py
--rw-rw-r--   0 david     (1000) david     (1000)     2768 2024-03-25 15:44:57.000000 pytoolbox-14.8.1/pytoolbox/aws/s3.py
--rw-rw-r--   0 david     (1000) david     (1000)    10212 2024-03-25 15:44:57.000000 pytoolbox-14.8.1/pytoolbox/collections.py
--rw-rw-r--   0 david     (1000) david     (1000)     4223 2024-04-02 11:17:02.000000 pytoolbox-14.8.1/pytoolbox/comparison.py
--rw-rw-r--   0 david     (1000) david     (1000)     6412 2024-04-02 11:17:02.000000 pytoolbox-14.8.1/pytoolbox/console.py
--rw-rw-r--   0 david     (1000) david     (1000)     6587 2024-03-25 15:44:57.000000 pytoolbox-14.8.1/pytoolbox/crypto.py
--rw-rw-r--   0 david     (1000) david     (1000)    12567 2024-03-25 15:44:57.000000 pytoolbox-14.8.1/pytoolbox/datetime.py
--rw-rw-r--   0 david     (1000) david     (1000)     5427 2024-04-02 11:17:02.000000 pytoolbox-14.8.1/pytoolbox/decorators.py
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2024-04-02 11:25:01.265378 pytoolbox-14.8.1/pytoolbox/django/
--rw-rw-r--   0 david     (1000) david     (1000)        0 2024-03-25 15:44:57.000000 pytoolbox-14.8.1/pytoolbox/django/__init__.py
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2024-04-02 11:25:01.265378 pytoolbox-14.8.1/pytoolbox/django/core/
--rw-rw-r--   0 david     (1000) david     (1000)        0 2024-03-25 15:44:57.000000 pytoolbox-14.8.1/pytoolbox/django/core/__init__.py
--rw-rw-r--   0 david     (1000) david     (1000)      113 2024-03-25 15:44:57.000000 pytoolbox-14.8.1/pytoolbox/django/core/constants.py
--rw-rw-r--   0 david     (1000) david     (1000)     2628 2024-03-25 15:44:57.000000 pytoolbox-14.8.1/pytoolbox/django/core/exceptions.py
--rw-rw-r--   0 david     (1000) david     (1000)     2582 2024-04-02 11:17:02.000000 pytoolbox-14.8.1/pytoolbox/django/core/validators.py
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2024-04-02 11:25:01.269378 pytoolbox-14.8.1/pytoolbox/django/forms/
--rw-rw-r--   0 david     (1000) david     (1000)       28 2024-03-25 15:44:57.000000 pytoolbox-14.8.1/pytoolbox/django/forms/__init__.py
--rw-rw-r--   0 david     (1000) david     (1000)      728 2024-03-25 15:44:57.000000 pytoolbox-14.8.1/pytoolbox/django/forms/base.py
--rw-rw-r--   0 david     (1000) david     (1000)      563 2024-03-25 15:44:57.000000 pytoolbox-14.8.1/pytoolbox/django/forms/fields.py
--rw-rw-r--   0 david     (1000) david     (1000)     5345 2024-04-02 11:17:02.000000 pytoolbox-14.8.1/pytoolbox/django/forms/mixins.py
--rw-rw-r--   0 david     (1000) david     (1000)     3562 2024-03-25 15:44:57.000000 pytoolbox-14.8.1/pytoolbox/django/forms/utils.py
--rw-rw-r--   0 david     (1000) david     (1000)      787 2024-03-25 15:44:57.000000 pytoolbox-14.8.1/pytoolbox/django/forms/widgets.py
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2024-04-02 11:25:01.273378 pytoolbox-14.8.1/pytoolbox/django/models/
--rw-rw-r--   0 david     (1000) david     (1000)        0 2024-03-25 15:44:57.000000 pytoolbox-14.8.1/pytoolbox/django/models/__init__.py
--rw-rw-r--   0 david     (1000) david     (1000)      412 2024-03-25 15:44:57.000000 pytoolbox-14.8.1/pytoolbox/django/models/base.py
--rw-rw-r--   0 david     (1000) david     (1000)     1658 2024-03-25 15:44:57.000000 pytoolbox-14.8.1/pytoolbox/django/models/decorators.py
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2024-04-02 11:25:01.273378 pytoolbox-14.8.1/pytoolbox/django/models/fields/
--rw-rw-r--   0 david     (1000) david     (1000)       28 2024-03-25 15:44:57.000000 pytoolbox-14.8.1/pytoolbox/django/models/fields/__init__.py
--rw-rw-r--   0 david     (1000) david     (1000)     4157 2024-03-25 15:44:57.000000 pytoolbox-14.8.1/pytoolbox/django/models/fields/base.py
--rw-rw-r--   0 david     (1000) david     (1000)     1299 2024-03-25 15:44:57.000000 pytoolbox-14.8.1/pytoolbox/django/models/fields/mixins.py
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2024-04-02 11:25:01.273378 pytoolbox-14.8.1/pytoolbox/django/models/managers/
--rw-rw-r--   0 david     (1000) david     (1000)        0 2024-03-25 15:44:57.000000 pytoolbox-14.8.1/pytoolbox/django/models/managers/__init__.py
--rw-rw-r--   0 david     (1000) david     (1000)      773 2024-03-25 15:44:57.000000 pytoolbox-14.8.1/pytoolbox/django/models/managers/mixins.py
--rw-rw-r--   0 david     (1000) david     (1000)      468 2024-03-25 15:44:57.000000 pytoolbox-14.8.1/pytoolbox/django/models/metaclass.py
--rw-rw-r--   0 david     (1000) david     (1000)    15196 2024-04-02 11:17:02.000000 pytoolbox-14.8.1/pytoolbox/django/models/mixins.py
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2024-04-02 11:25:01.277378 pytoolbox-14.8.1/pytoolbox/django/models/query/
--rw-rw-r--   0 david     (1000) david     (1000)        0 2024-03-25 15:44:57.000000 pytoolbox-14.8.1/pytoolbox/django/models/query/__init__.py
--rw-rw-r--   0 david     (1000) david     (1000)     2555 2024-03-25 15:44:57.000000 pytoolbox-14.8.1/pytoolbox/django/models/query/mixins.py
--rw-rw-r--   0 david     (1000) david     (1000)     1511 2024-04-02 11:17:02.000000 pytoolbox-14.8.1/pytoolbox/django/models/utils.py
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2024-04-02 11:25:01.277378 pytoolbox-14.8.1/pytoolbox/django/signals/
--rw-rw-r--   0 david     (1000) david     (1000)       64 2024-03-25 15:44:57.000000 pytoolbox-14.8.1/pytoolbox/django/signals/__init__.py
--rw-rw-r--   0 david     (1000) david     (1000)      541 2024-03-25 15:44:57.000000 pytoolbox-14.8.1/pytoolbox/django/signals/dispatch.py
--rw-rw-r--   0 david     (1000) david     (1000)     3796 2024-04-02 11:17:02.000000 pytoolbox-14.8.1/pytoolbox/django/signals/handlers.py
--rw-rw-r--   0 david     (1000) david     (1000)     1426 2024-04-02 11:17:02.000000 pytoolbox-14.8.1/pytoolbox/django/storage.py
--rw-rw-r--   0 david     (1000) david     (1000)    10688 2024-04-02 11:17:02.000000 pytoolbox-14.8.1/pytoolbox/django/templatetags.py
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2024-04-02 11:25:01.277378 pytoolbox-14.8.1/pytoolbox/django/test/
--rw-rw-r--   0 david     (1000) david     (1000)        0 2024-03-25 15:44:57.000000 pytoolbox-14.8.1/pytoolbox/django/test/__init__.py
--rw-rw-r--   0 david     (1000) david     (1000)     4796 2024-03-25 15:44:57.000000 pytoolbox-14.8.1/pytoolbox/django/test/mixins.py
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2024-04-02 11:25:01.281378 pytoolbox-14.8.1/pytoolbox/django/test/runner/
--rw-rw-r--   0 david     (1000) david     (1000)        0 2024-03-25 15:44:57.000000 pytoolbox-14.8.1/pytoolbox/django/test/runner/__init__.py
--rw-rw-r--   0 david     (1000) david     (1000)      878 2024-03-25 15:44:57.000000 pytoolbox-14.8.1/pytoolbox/django/test/runner/mixins.py
--rw-rw-r--   0 david     (1000) david     (1000)      614 2024-03-25 15:44:57.000000 pytoolbox-14.8.1/pytoolbox/django/urls.py
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2024-04-02 11:25:01.281378 pytoolbox-14.8.1/pytoolbox/django/utils/
--rw-rw-r--   0 david     (1000) david     (1000)        0 2024-03-25 15:44:57.000000 pytoolbox-14.8.1/pytoolbox/django/utils/__init__.py
--rw-rw-r--   0 david     (1000) david     (1000)     2375 2024-03-25 15:44:57.000000 pytoolbox-14.8.1/pytoolbox/django/utils/collections.py
--rw-rw-r--   0 david     (1000) david     (1000)     1660 2024-03-25 15:44:57.000000 pytoolbox-14.8.1/pytoolbox/django/utils/logging.py
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2024-04-02 11:25:01.281378 pytoolbox-14.8.1/pytoolbox/django/views/
--rw-rw-r--   0 david     (1000) david     (1000)       28 2024-03-25 15:44:57.000000 pytoolbox-14.8.1/pytoolbox/django/views/__init__.py
--rw-rw-r--   0 david     (1000) david     (1000)      511 2024-03-25 15:44:57.000000 pytoolbox-14.8.1/pytoolbox/django/views/base.py
--rw-rw-r--   0 david     (1000) david     (1000)     4927 2024-03-25 15:44:57.000000 pytoolbox-14.8.1/pytoolbox/django/views/mixins.py
--rw-rw-r--   0 david     (1000) david     (1000)      317 2024-03-25 15:44:57.000000 pytoolbox-14.8.1/pytoolbox/django/views/utils.py
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2024-04-02 11:25:01.285378 pytoolbox-14.8.1/pytoolbox/django_datatable_view/
--rw-rw-r--   0 david     (1000) david     (1000)        0 2024-03-25 15:44:57.000000 pytoolbox-14.8.1/pytoolbox/django_datatable_view/__init__.py
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2024-04-02 11:25:01.285378 pytoolbox-14.8.1/pytoolbox/django_datatable_view/views/
--rw-rw-r--   0 david     (1000) david     (1000)        0 2024-03-25 15:44:57.000000 pytoolbox-14.8.1/pytoolbox/django_datatable_view/views/__init__.py
--rw-rw-r--   0 david     (1000) david     (1000)     1767 2024-03-25 15:44:57.000000 pytoolbox-14.8.1/pytoolbox/django_datatable_view/views/mixins.py
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2024-04-02 11:25:01.285378 pytoolbox-14.8.1/pytoolbox/django_filter/
--rw-rw-r--   0 david     (1000) david     (1000)        0 2024-03-25 15:44:57.000000 pytoolbox-14.8.1/pytoolbox/django_filter/__init__.py
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2024-04-02 11:25:01.285378 pytoolbox-14.8.1/pytoolbox/django_filter/filterset/
--rw-rw-r--   0 david     (1000) david     (1000)        0 2024-03-25 15:44:57.000000 pytoolbox-14.8.1/pytoolbox/django_filter/filterset/__init__.py
--rw-rw-r--   0 david     (1000) david     (1000)      752 2024-04-02 11:17:02.000000 pytoolbox-14.8.1/pytoolbox/django_filter/filterset/mixins.py
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2024-04-02 11:25:01.285378 pytoolbox-14.8.1/pytoolbox/django_formtools/
--rw-rw-r--   0 david     (1000) david     (1000)        0 2024-03-25 15:44:57.000000 pytoolbox-14.8.1/pytoolbox/django_formtools/__init__.py
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2024-04-02 11:25:01.289378 pytoolbox-14.8.1/pytoolbox/django_formtools/views/
--rw-rw-r--   0 david     (1000) david     (1000)        0 2024-03-25 15:44:57.000000 pytoolbox-14.8.1/pytoolbox/django_formtools/views/__init__.py
--rw-rw-r--   0 david     (1000) david     (1000)     3091 2024-03-25 15:44:57.000000 pytoolbox-14.8.1/pytoolbox/django_formtools/views/mixins.py
--rw-rw-r--   0 david     (1000) david     (1000)     1570 2024-04-02 11:17:02.000000 pytoolbox-14.8.1/pytoolbox/enum.py
--rw-rw-r--   0 david     (1000) david     (1000)     6445 2024-04-02 11:17:02.000000 pytoolbox-14.8.1/pytoolbox/exceptions.py
--rw-rw-r--   0 david     (1000) david     (1000)    25984 2024-04-02 11:17:02.000000 pytoolbox-14.8.1/pytoolbox/filesystem.py
--rw-rw-r--   0 david     (1000) david     (1000)     3134 2024-04-02 11:17:02.000000 pytoolbox-14.8.1/pytoolbox/flask.py
--rw-rw-r--   0 david     (1000) david     (1000)     4203 2024-04-02 11:17:02.000000 pytoolbox-14.8.1/pytoolbox/git.py
--rw-rw-r--   0 david     (1000) david     (1000)    11833 2024-04-02 11:17:02.000000 pytoolbox-14.8.1/pytoolbox/humanize.py
--rw-rw-r--   0 david     (1000) david     (1000)     2417 2024-03-25 15:44:57.000000 pytoolbox-14.8.1/pytoolbox/itertools.py
--rw-rw-r--   0 david     (1000) david     (1000)    49307 2024-04-02 11:17:02.000000 pytoolbox-14.8.1/pytoolbox/juju.py
--rw-rw-r--   0 david     (1000) david     (1000)     1120 2024-03-25 15:44:57.000000 pytoolbox-14.8.1/pytoolbox/linux.py
--rw-rw-r--   0 david     (1000) david     (1000)     5533 2024-04-02 11:17:02.000000 pytoolbox-14.8.1/pytoolbox/logging.py
--rw-rw-r--   0 david     (1000) david     (1000)      424 2024-03-25 15:44:57.000000 pytoolbox-14.8.1/pytoolbox/module.py
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2024-04-02 11:25:01.289378 pytoolbox-14.8.1/pytoolbox/multimedia/
--rw-rw-r--   0 david     (1000) david     (1000)        0 2024-03-25 15:44:57.000000 pytoolbox-14.8.1/pytoolbox/multimedia/__init__.py
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2024-04-02 11:25:01.293378 pytoolbox-14.8.1/pytoolbox/multimedia/exif/
--rw-rw-r--   0 david     (1000) david     (1000)      344 2024-03-25 15:44:57.000000 pytoolbox-14.8.1/pytoolbox/multimedia/exif/__init__.py
--rw-rw-r--   0 david     (1000) david     (1000)     1654 2024-03-25 15:44:57.000000 pytoolbox-14.8.1/pytoolbox/multimedia/exif/brand.py
--rw-rw-r--   0 david     (1000) david     (1000)      642 2024-03-25 15:44:57.000000 pytoolbox-14.8.1/pytoolbox/multimedia/exif/camera.py
--rw-rw-r--   0 david     (1000) david     (1000)     1145 2024-04-02 11:17:02.000000 pytoolbox-14.8.1/pytoolbox/multimedia/exif/equipment.py
--rw-rw-r--   0 david     (1000) david     (1000)     1914 2024-03-25 15:44:57.000000 pytoolbox-14.8.1/pytoolbox/multimedia/exif/image.py
--rw-rw-r--   0 david     (1000) david     (1000)      907 2024-03-25 15:44:57.000000 pytoolbox-14.8.1/pytoolbox/multimedia/exif/lens.py
--rw-rw-r--   0 david     (1000) david     (1000)     2579 2024-04-02 11:17:02.000000 pytoolbox-14.8.1/pytoolbox/multimedia/exif/metadata.py
--rw-rw-r--   0 david     (1000) david     (1000)     1847 2024-03-25 15:44:57.000000 pytoolbox-14.8.1/pytoolbox/multimedia/exif/photo.py
--rw-rw-r--   0 david     (1000) david     (1000)     3909 2024-04-02 11:17:02.000000 pytoolbox-14.8.1/pytoolbox/multimedia/exif/tag.py
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2024-04-02 11:25:01.301378 pytoolbox-14.8.1/pytoolbox/multimedia/ffmpeg/
--rw-rw-r--   0 david     (1000) david     (1000)      672 2024-03-25 15:44:57.000000 pytoolbox-14.8.1/pytoolbox/multimedia/ffmpeg/__init__.py
--rw-rw-r--   0 david     (1000) david     (1000)     7270 2024-03-25 15:44:57.000000 pytoolbox-14.8.1/pytoolbox/multimedia/ffmpeg/encode.py
--rw-rw-r--   0 david     (1000) david     (1000)     5898 2024-03-25 15:44:57.000000 pytoolbox-14.8.1/pytoolbox/multimedia/ffmpeg/ffmpeg.py
--rw-rw-r--   0 david     (1000) david     (1000)     8566 2024-03-25 15:44:57.000000 pytoolbox-14.8.1/pytoolbox/multimedia/ffmpeg/ffprobe.py
--rw-rw-r--   0 david     (1000) david     (1000)     9639 2024-03-25 15:44:57.000000 pytoolbox-14.8.1/pytoolbox/multimedia/ffmpeg/miscellaneous.py
--rw-rw-r--   0 david     (1000) david     (1000)     1809 2024-03-25 15:44:57.000000 pytoolbox-14.8.1/pytoolbox/multimedia/ffmpeg/utils.py
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2024-04-02 11:25:01.301378 pytoolbox-14.8.1/pytoolbox/multimedia/image/
--rw-rw-r--   0 david     (1000) david     (1000)     2302 2024-03-25 15:44:57.000000 pytoolbox-14.8.1/pytoolbox/multimedia/image/PIL.py
--rw-rw-r--   0 david     (1000) david     (1000)        0 2024-03-25 15:44:57.000000 pytoolbox-14.8.1/pytoolbox/multimedia/image/__init__.py
--rw-rw-r--   0 david     (1000) david     (1000)     1699 2024-03-25 15:44:57.000000 pytoolbox-14.8.1/pytoolbox/multimedia/x264.py
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2024-04-02 11:25:01.305378 pytoolbox-14.8.1/pytoolbox/network/
--rw-rw-r--   0 david     (1000) david     (1000)        0 2024-03-25 15:44:57.000000 pytoolbox-14.8.1/pytoolbox/network/__init__.py
--rw-rw-r--   0 david     (1000) david     (1000)    11608 2024-03-25 15:44:57.000000 pytoolbox-14.8.1/pytoolbox/network/http.py
--rw-rw-r--   0 david     (1000) david     (1000)     1151 2024-03-25 15:44:57.000000 pytoolbox-14.8.1/pytoolbox/network/ip.py
--rw-rw-r--   0 david     (1000) david     (1000)    15650 2024-04-02 11:17:02.000000 pytoolbox-14.8.1/pytoolbox/network/rtp.py
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2024-04-02 11:25:01.305378 pytoolbox-14.8.1/pytoolbox/network/smpte2022/
--rw-rw-r--   0 david     (1000) david     (1000)        0 2024-03-25 15:44:57.000000 pytoolbox-14.8.1/pytoolbox/network/smpte2022/__init__.py
--rw-rw-r--   0 david     (1000) david     (1000)    27733 2024-04-02 11:17:02.000000 pytoolbox-14.8.1/pytoolbox/network/smpte2022/base.py
--rw-rw-r--   0 david     (1000) david     (1000)    10420 2024-03-25 15:44:57.000000 pytoolbox-14.8.1/pytoolbox/network/smpte2022/generator.py
--rw-rw-r--   0 david     (1000) david     (1000)    27854 2024-03-25 15:44:57.000000 pytoolbox-14.8.1/pytoolbox/network/smpte2022/receiver.py
--rw-rw-r--   0 david     (1000) david     (1000)      916 2024-03-25 15:44:57.000000 pytoolbox-14.8.1/pytoolbox/network/url.py
--rw-rw-r--   0 david     (1000) david     (1000)      527 2024-03-25 15:44:57.000000 pytoolbox-14.8.1/pytoolbox/pandas.py
--rw-rw-r--   0 david     (1000) david     (1000)      466 2024-03-25 15:44:57.000000 pytoolbox-14.8.1/pytoolbox/private.py
--rw-rw-r--   0 david     (1000) david     (1000)     5330 2024-04-02 11:17:02.000000 pytoolbox-14.8.1/pytoolbox/regex.py
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2024-04-02 11:25:01.309378 pytoolbox-14.8.1/pytoolbox/rest_framework/
--rw-rw-r--   0 david     (1000) david     (1000)        0 2024-03-25 15:44:57.000000 pytoolbox-14.8.1/pytoolbox/rest_framework/__init__.py
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2024-04-02 11:25:01.309378 pytoolbox-14.8.1/pytoolbox/rest_framework/metadata/
--rw-rw-r--   0 david     (1000) david     (1000)        0 2024-03-25 15:44:57.000000 pytoolbox-14.8.1/pytoolbox/rest_framework/metadata/__init__.py
--rw-rw-r--   0 david     (1000) david     (1000)     1106 2024-04-02 11:17:02.000000 pytoolbox-14.8.1/pytoolbox/rest_framework/metadata/mixins.py
--rw-rw-r--   0 david     (1000) david     (1000)      717 2024-03-25 15:44:57.000000 pytoolbox-14.8.1/pytoolbox/rest_framework/permissions.py
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2024-04-02 11:25:01.309378 pytoolbox-14.8.1/pytoolbox/rest_framework/serializers/
--rw-rw-r--   0 david     (1000) david     (1000)        0 2024-03-25 15:44:57.000000 pytoolbox-14.8.1/pytoolbox/rest_framework/serializers/__init__.py
--rw-rw-r--   0 david     (1000) david     (1000)      777 2024-03-25 15:44:57.000000 pytoolbox-14.8.1/pytoolbox/rest_framework/serializers/fields.py
--rw-rw-r--   0 david     (1000) david     (1000)     2238 2024-03-25 15:44:57.000000 pytoolbox-14.8.1/pytoolbox/rest_framework/serializers/mixins.py
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2024-04-02 11:25:01.313378 pytoolbox-14.8.1/pytoolbox/rest_framework/views/
--rw-rw-r--   0 david     (1000) david     (1000)        0 2024-03-25 15:44:57.000000 pytoolbox-14.8.1/pytoolbox/rest_framework/views/__init__.py
--rw-rw-r--   0 david     (1000) david     (1000)     1571 2024-03-25 15:44:57.000000 pytoolbox-14.8.1/pytoolbox/rest_framework/views/mixins.py
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2024-04-02 11:25:01.317378 pytoolbox-14.8.1/pytoolbox/selenium/
--rw-rw-r--   0 david     (1000) david     (1000)      149 2024-03-25 15:44:57.000000 pytoolbox-14.8.1/pytoolbox/selenium/__init__.py
--rw-rw-r--   0 david     (1000) david     (1000)     3349 2024-03-25 15:44:57.000000 pytoolbox-14.8.1/pytoolbox/selenium/client.py
--rw-rw-r--   0 david     (1000) david     (1000)     1343 2024-03-25 15:44:57.000000 pytoolbox-14.8.1/pytoolbox/selenium/common.py
--rw-rw-r--   0 david     (1000) david     (1000)      464 2024-03-25 15:44:57.000000 pytoolbox-14.8.1/pytoolbox/selenium/exceptions.py
--rw-rw-r--   0 david     (1000) david     (1000)      266 2024-03-25 15:44:57.000000 pytoolbox-14.8.1/pytoolbox/selenium/select.py
--rw-rw-r--   0 david     (1000) david     (1000)     2631 2024-04-02 11:17:02.000000 pytoolbox-14.8.1/pytoolbox/selenium/test.py
--rw-rw-r--   0 david     (1000) david     (1000)      815 2024-03-25 15:44:57.000000 pytoolbox-14.8.1/pytoolbox/selenium/webdrivers.py
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2024-04-02 11:25:01.317378 pytoolbox-14.8.1/pytoolbox/selenium/webelements/
--rw-rw-r--   0 david     (1000) david     (1000)      186 2024-03-25 15:44:57.000000 pytoolbox-14.8.1/pytoolbox/selenium/webelements/__init__.py
--rw-rw-r--   0 david     (1000) david     (1000)     1109 2024-03-25 15:44:57.000000 pytoolbox-14.8.1/pytoolbox/selenium/webelements/base.py
--rw-rw-r--   0 david     (1000) david     (1000)     1030 2024-03-25 15:44:57.000000 pytoolbox-14.8.1/pytoolbox/selenium/webelements/bootstrap_slider.py
--rw-rw-r--   0 david     (1000) david     (1000)      473 2024-03-25 15:44:57.000000 pytoolbox-14.8.1/pytoolbox/selenium/webelements/bootstrap_switch.py
--rw-rw-r--   0 david     (1000) david     (1000)    21143 2024-04-02 11:17:02.000000 pytoolbox-14.8.1/pytoolbox/serialization.py
--rw-rw-r--   0 david     (1000) david     (1000)      452 2024-03-25 15:44:57.000000 pytoolbox-14.8.1/pytoolbox/setuptools.py
--rw-rw-r--   0 david     (1000) david     (1000)     1650 2024-03-25 15:44:57.000000 pytoolbox-14.8.1/pytoolbox/signals.py
--rw-rw-r--   0 david     (1000) david     (1000)     3402 2024-04-02 11:17:02.000000 pytoolbox-14.8.1/pytoolbox/ssh.py
--rw-rw-r--   0 david     (1000) david     (1000)     2875 2024-03-25 15:44:57.000000 pytoolbox-14.8.1/pytoolbox/states.py
--rw-rw-r--   0 david     (1000) david     (1000)     4864 2024-03-25 15:44:57.000000 pytoolbox-14.8.1/pytoolbox/string.py
--rw-rw-r--   0 david     (1000) david     (1000)    13522 2024-04-02 11:17:02.000000 pytoolbox-14.8.1/pytoolbox/subprocess.py
--rw-rw-r--   0 david     (1000) david     (1000)     3407 2024-03-25 15:44:57.000000 pytoolbox-14.8.1/pytoolbox/throttles.py
--rw-rw-r--   0 david     (1000) david     (1000)     8965 2024-04-02 11:17:02.000000 pytoolbox-14.8.1/pytoolbox/types.py
--rw-rw-r--   0 david     (1000) david     (1000)    10931 2024-03-25 15:44:57.000000 pytoolbox-14.8.1/pytoolbox/unittest.py
--rw-rw-r--   0 david     (1000) david     (1000)     9644 2024-04-02 11:17:02.000000 pytoolbox-14.8.1/pytoolbox/validation.py
--rw-rw-r--   0 david     (1000) david     (1000)     1164 2024-03-25 15:44:57.000000 pytoolbox-14.8.1/pytoolbox/virtualenv.py
--rw-rw-r--   0 david     (1000) david     (1000)     2160 2024-03-25 15:44:57.000000 pytoolbox-14.8.1/pytoolbox/voluptuous.py
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2024-04-02 11:25:01.333378 pytoolbox-14.8.1/pytoolbox.egg-info/
--rw-r--r--   0 david     (1000) david     (1000)    11167 2024-04-02 11:25:01.000000 pytoolbox-14.8.1/pytoolbox.egg-info/PKG-INFO
--rw-rw-r--   0 david     (1000) david     (1000)     5548 2024-04-02 11:25:01.000000 pytoolbox-14.8.1/pytoolbox.egg-info/SOURCES.txt
--rw-rw-r--   0 david     (1000) david     (1000)        1 2024-04-02 11:25:01.000000 pytoolbox-14.8.1/pytoolbox.egg-info/dependency_links.txt
--rw-rw-r--   0 david     (1000) david     (1000)     1042 2024-04-02 11:25:01.000000 pytoolbox-14.8.1/pytoolbox.egg-info/requires.txt
--rw-rw-r--   0 david     (1000) david     (1000)       10 2024-04-02 11:25:01.000000 pytoolbox-14.8.1/pytoolbox.egg-info/top_level.txt
--rw-rw-r--   0 david     (1000) david     (1000)      144 2024-04-02 11:25:01.357379 pytoolbox-14.8.1/setup.cfg
--rwxrwxr-x   0 david     (1000) david     (1000)     8796 2024-03-25 15:44:57.000000 pytoolbox-14.8.1/setup.py
-drwxrwxr-x   0 david     (1000) david     (1000)        0 2024-04-02 11:25:01.333378 pytoolbox-14.8.1/tests/
--rw-rw-r--   0 david     (1000) david     (1000)     2961 2024-04-02 11:17:02.000000 pytoolbox-14.8.1/tests/test_argparse.py
--rw-rw-r--   0 david     (1000) david     (1000)     1237 2024-03-25 15:44:57.000000 pytoolbox-14.8.1/tests/test_collections.py
--rw-rw-r--   0 david     (1000) david     (1000)     4691 2024-04-02 11:17:02.000000 pytoolbox-14.8.1/tests/test_comparison.py
--rw-rw-r--   0 david     (1000) david     (1000)      832 2024-03-25 15:44:57.000000 pytoolbox-14.8.1/tests/test_console.py
--rw-rw-r--   0 david     (1000) david     (1000)      514 2024-03-25 15:44:57.000000 pytoolbox-14.8.1/tests/test_decorators.py
--rw-rw-r--   0 david     (1000) david     (1000)      668 2024-03-25 15:44:57.000000 pytoolbox-14.8.1/tests/test_django_utils.py
--rw-rw-r--   0 david     (1000) david     (1000)     2185 2024-04-02 11:17:02.000000 pytoolbox-14.8.1/tests/test_exceptions.py
--rw-rw-r--   0 david     (1000) david     (1000)    16098 2024-03-25 15:44:57.000000 pytoolbox-14.8.1/tests/test_ffmpeg.py
--rw-rw-r--   0 david     (1000) david     (1000)     2555 2024-03-25 15:44:57.000000 pytoolbox-14.8.1/tests/test_filesystem.py
--rw-rw-r--   0 david     (1000) david     (1000)     5059 2024-04-02 11:17:02.000000 pytoolbox-14.8.1/tests/test_git.py
--rw-rw-r--   0 david     (1000) david     (1000)     2887 2024-03-25 15:44:57.000000 pytoolbox-14.8.1/tests/test_juju.py
--rw-rw-r--   0 david     (1000) david     (1000)      813 2024-04-02 11:17:02.000000 pytoolbox-14.8.1/tests/test_logging.py
--rw-rw-r--   0 david     (1000) david     (1000)      705 2024-03-25 15:44:57.000000 pytoolbox-14.8.1/tests/test_module.py
--rw-rw-r--   0 david     (1000) david     (1000)      692 2024-03-25 15:44:57.000000 pytoolbox-14.8.1/tests/test_private.py
--rw-rw-r--   0 david     (1000) david     (1000)     2068 2024-03-25 15:44:57.000000 pytoolbox-14.8.1/tests/test_regex.py
--rw-rw-r--   0 david     (1000) david     (1000)     1679 2024-03-25 15:44:57.000000 pytoolbox-14.8.1/tests/test_serialization.py
--rw-rw-r--   0 david     (1000) david     (1000)     2699 2024-03-25 15:44:57.000000 pytoolbox-14.8.1/tests/test_signals.py
--rw-rw-r--   0 david     (1000) david     (1000)     4525 2024-03-25 15:44:57.000000 pytoolbox-14.8.1/tests/test_ssh.py
--rw-rw-r--   0 david     (1000) david     (1000)     4125 2024-03-25 15:44:57.000000 pytoolbox-14.8.1/tests/test_states.py
--rw-rw-r--   0 david     (1000) david     (1000)     2873 2024-03-25 15:44:57.000000 pytoolbox-14.8.1/tests/test_string.py
--rw-rw-r--   0 david     (1000) david     (1000)     6002 2024-04-02 11:17:02.000000 pytoolbox-14.8.1/tests/test_subprocess.py
--rw-rw-r--   0 david     (1000) david     (1000)      338 2024-03-25 15:44:57.000000 pytoolbox-14.8.1/tests/test_types.py
--rw-rw-r--   0 david     (1000) david     (1000)     5981 2024-03-25 15:44:57.000000 pytoolbox-14.8.1/tests/test_unittest.py
--rw-rw-r--   0 david     (1000) david     (1000)      637 2024-03-25 15:44:57.000000 pytoolbox-14.8.1/tests/test_validation.py
--rw-rw-r--   0 david     (1000) david     (1000)      433 2024-03-25 15:44:57.000000 pytoolbox-14.8.1/tests/test_x264.py
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2024-04-03 10:21:27.105097 pytoolbox-14.8.2/
+-rw-rw-r--   0 david     (1000) david     (1000)      219 2024-03-25 15:44:57.000000 pytoolbox-14.8.2/AUTHORS.md
+-rw-rw-r--   0 david     (1000) david     (1000)    35535 2024-04-03 10:16:31.000000 pytoolbox-14.8.2/CHANGELOG.md
+-rw-rw-r--   0 david     (1000) david     (1000)     5747 2024-03-25 15:44:57.000000 pytoolbox-14.8.2/LICENSE.rst
+-rw-rw-r--   0 david     (1000) david     (1000)       27 2024-03-25 15:44:57.000000 pytoolbox-14.8.2/MANIFEST.in
+-rw-r--r--   0 david     (1000) david     (1000)    11167 2024-04-03 10:21:27.105097 pytoolbox-14.8.2/PKG-INFO
+-rw-rw-r--   0 david     (1000) david     (1000)     6529 2024-03-26 07:35:12.000000 pytoolbox-14.8.2/README.rst
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2024-04-03 10:21:27.005096 pytoolbox-14.8.2/pytoolbox/
+-rw-rw-r--   0 david     (1000) david     (1000)      467 2024-04-03 10:16:38.000000 pytoolbox-14.8.2/pytoolbox/__init__.py
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2024-04-03 10:21:27.009096 pytoolbox-14.8.2/pytoolbox/ai/
+-rw-rw-r--   0 david     (1000) david     (1000)        0 2024-03-25 15:44:57.000000 pytoolbox-14.8.2/pytoolbox/ai/__init__.py
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2024-04-03 10:21:27.009096 pytoolbox-14.8.2/pytoolbox/ai/vision/
+-rw-rw-r--   0 david     (1000) david     (1000)        0 2024-03-25 15:44:57.000000 pytoolbox-14.8.2/pytoolbox/ai/vision/__init__.py
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2024-04-03 10:21:27.009096 pytoolbox-14.8.2/pytoolbox/ai/vision/face/
+-rw-rw-r--   0 david     (1000) david     (1000)        0 2024-03-25 15:44:57.000000 pytoolbox-14.8.2/pytoolbox/ai/vision/face/__init__.py
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2024-04-03 10:21:27.009096 pytoolbox-14.8.2/pytoolbox/ai/vision/face/detect/
+-rw-rw-r--   0 david     (1000) david     (1000)       67 2024-03-25 15:44:57.000000 pytoolbox-14.8.2/pytoolbox/ai/vision/face/detect/__init__.py
+-rw-rw-r--   0 david     (1000) david     (1000)     8925 2024-03-25 15:44:57.000000 pytoolbox-14.8.2/pytoolbox/ai/vision/face/detect/dlib.py
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2024-04-03 10:21:27.013096 pytoolbox-14.8.2/pytoolbox/ai/vision/face/recognize/
+-rw-rw-r--   0 david     (1000) david     (1000)       97 2024-03-25 15:44:57.000000 pytoolbox-14.8.2/pytoolbox/ai/vision/face/recognize/__init__.py
+-rw-rw-r--   0 david     (1000) david     (1000)    11412 2024-03-25 15:44:57.000000 pytoolbox-14.8.2/pytoolbox/ai/vision/face/recognize/nn4_small2.py
+-rw-rw-r--   0 david     (1000) david     (1000)      651 2024-03-25 15:44:57.000000 pytoolbox-14.8.2/pytoolbox/ai/vision/utils.py
+-rw-rw-r--   0 david     (1000) david     (1000)     7959 2024-04-02 11:17:02.000000 pytoolbox-14.8.2/pytoolbox/argparse.py
+-rw-rw-r--   0 david     (1000) david     (1000)     1738 2024-03-25 15:44:57.000000 pytoolbox-14.8.2/pytoolbox/atlassian.py
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2024-04-03 10:21:27.013096 pytoolbox-14.8.2/pytoolbox/aws/
+-rw-rw-r--   0 david     (1000) david     (1000)       71 2024-03-25 15:44:57.000000 pytoolbox-14.8.2/pytoolbox/aws/__init__.py
+-rw-rw-r--   0 david     (1000) david     (1000)     2768 2024-03-25 15:44:57.000000 pytoolbox-14.8.2/pytoolbox/aws/s3.py
+-rw-rw-r--   0 david     (1000) david     (1000)    10212 2024-03-25 15:44:57.000000 pytoolbox-14.8.2/pytoolbox/collections.py
+-rw-rw-r--   0 david     (1000) david     (1000)     4223 2024-04-02 11:17:02.000000 pytoolbox-14.8.2/pytoolbox/comparison.py
+-rw-rw-r--   0 david     (1000) david     (1000)     6412 2024-04-02 11:17:02.000000 pytoolbox-14.8.2/pytoolbox/console.py
+-rw-rw-r--   0 david     (1000) david     (1000)     6587 2024-03-25 15:44:57.000000 pytoolbox-14.8.2/pytoolbox/crypto.py
+-rw-rw-r--   0 david     (1000) david     (1000)    12567 2024-03-25 15:44:57.000000 pytoolbox-14.8.2/pytoolbox/datetime.py
+-rw-rw-r--   0 david     (1000) david     (1000)     5427 2024-04-02 11:17:02.000000 pytoolbox-14.8.2/pytoolbox/decorators.py
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2024-04-03 10:21:27.013096 pytoolbox-14.8.2/pytoolbox/django/
+-rw-rw-r--   0 david     (1000) david     (1000)        0 2024-03-25 15:44:57.000000 pytoolbox-14.8.2/pytoolbox/django/__init__.py
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2024-04-03 10:21:27.017096 pytoolbox-14.8.2/pytoolbox/django/core/
+-rw-rw-r--   0 david     (1000) david     (1000)        0 2024-03-25 15:44:57.000000 pytoolbox-14.8.2/pytoolbox/django/core/__init__.py
+-rw-rw-r--   0 david     (1000) david     (1000)      113 2024-03-25 15:44:57.000000 pytoolbox-14.8.2/pytoolbox/django/core/constants.py
+-rw-rw-r--   0 david     (1000) david     (1000)     2628 2024-03-25 15:44:57.000000 pytoolbox-14.8.2/pytoolbox/django/core/exceptions.py
+-rw-rw-r--   0 david     (1000) david     (1000)     2582 2024-04-02 11:17:02.000000 pytoolbox-14.8.2/pytoolbox/django/core/validators.py
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2024-04-03 10:21:27.017096 pytoolbox-14.8.2/pytoolbox/django/forms/
+-rw-rw-r--   0 david     (1000) david     (1000)       28 2024-03-25 15:44:57.000000 pytoolbox-14.8.2/pytoolbox/django/forms/__init__.py
+-rw-rw-r--   0 david     (1000) david     (1000)      728 2024-03-25 15:44:57.000000 pytoolbox-14.8.2/pytoolbox/django/forms/base.py
+-rw-rw-r--   0 david     (1000) david     (1000)      563 2024-03-25 15:44:57.000000 pytoolbox-14.8.2/pytoolbox/django/forms/fields.py
+-rw-rw-r--   0 david     (1000) david     (1000)     5345 2024-04-02 11:17:02.000000 pytoolbox-14.8.2/pytoolbox/django/forms/mixins.py
+-rw-rw-r--   0 david     (1000) david     (1000)     3562 2024-03-25 15:44:57.000000 pytoolbox-14.8.2/pytoolbox/django/forms/utils.py
+-rw-rw-r--   0 david     (1000) david     (1000)      787 2024-03-25 15:44:57.000000 pytoolbox-14.8.2/pytoolbox/django/forms/widgets.py
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2024-04-03 10:21:27.021096 pytoolbox-14.8.2/pytoolbox/django/models/
+-rw-rw-r--   0 david     (1000) david     (1000)        0 2024-03-25 15:44:57.000000 pytoolbox-14.8.2/pytoolbox/django/models/__init__.py
+-rw-rw-r--   0 david     (1000) david     (1000)      412 2024-03-25 15:44:57.000000 pytoolbox-14.8.2/pytoolbox/django/models/base.py
+-rw-rw-r--   0 david     (1000) david     (1000)     1658 2024-03-25 15:44:57.000000 pytoolbox-14.8.2/pytoolbox/django/models/decorators.py
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2024-04-03 10:21:27.021096 pytoolbox-14.8.2/pytoolbox/django/models/fields/
+-rw-rw-r--   0 david     (1000) david     (1000)       28 2024-03-25 15:44:57.000000 pytoolbox-14.8.2/pytoolbox/django/models/fields/__init__.py
+-rw-rw-r--   0 david     (1000) david     (1000)     4157 2024-03-25 15:44:57.000000 pytoolbox-14.8.2/pytoolbox/django/models/fields/base.py
+-rw-rw-r--   0 david     (1000) david     (1000)     1299 2024-03-25 15:44:57.000000 pytoolbox-14.8.2/pytoolbox/django/models/fields/mixins.py
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2024-04-03 10:21:27.025096 pytoolbox-14.8.2/pytoolbox/django/models/managers/
+-rw-rw-r--   0 david     (1000) david     (1000)        0 2024-03-25 15:44:57.000000 pytoolbox-14.8.2/pytoolbox/django/models/managers/__init__.py
+-rw-rw-r--   0 david     (1000) david     (1000)      773 2024-03-25 15:44:57.000000 pytoolbox-14.8.2/pytoolbox/django/models/managers/mixins.py
+-rw-rw-r--   0 david     (1000) david     (1000)      468 2024-03-25 15:44:57.000000 pytoolbox-14.8.2/pytoolbox/django/models/metaclass.py
+-rw-rw-r--   0 david     (1000) david     (1000)    15196 2024-04-02 11:17:02.000000 pytoolbox-14.8.2/pytoolbox/django/models/mixins.py
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2024-04-03 10:21:27.025096 pytoolbox-14.8.2/pytoolbox/django/models/query/
+-rw-rw-r--   0 david     (1000) david     (1000)        0 2024-03-25 15:44:57.000000 pytoolbox-14.8.2/pytoolbox/django/models/query/__init__.py
+-rw-rw-r--   0 david     (1000) david     (1000)     2555 2024-03-25 15:44:57.000000 pytoolbox-14.8.2/pytoolbox/django/models/query/mixins.py
+-rw-rw-r--   0 david     (1000) david     (1000)     1511 2024-04-02 11:17:02.000000 pytoolbox-14.8.2/pytoolbox/django/models/utils.py
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2024-04-03 10:21:27.025096 pytoolbox-14.8.2/pytoolbox/django/signals/
+-rw-rw-r--   0 david     (1000) david     (1000)       64 2024-03-25 15:44:57.000000 pytoolbox-14.8.2/pytoolbox/django/signals/__init__.py
+-rw-rw-r--   0 david     (1000) david     (1000)      541 2024-03-25 15:44:57.000000 pytoolbox-14.8.2/pytoolbox/django/signals/dispatch.py
+-rw-rw-r--   0 david     (1000) david     (1000)     3796 2024-04-02 11:17:02.000000 pytoolbox-14.8.2/pytoolbox/django/signals/handlers.py
+-rw-rw-r--   0 david     (1000) david     (1000)     1426 2024-04-02 11:48:14.000000 pytoolbox-14.8.2/pytoolbox/django/storage.py
+-rw-rw-r--   0 david     (1000) david     (1000)    10688 2024-04-02 11:17:02.000000 pytoolbox-14.8.2/pytoolbox/django/templatetags.py
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2024-04-03 10:21:27.025096 pytoolbox-14.8.2/pytoolbox/django/test/
+-rw-rw-r--   0 david     (1000) david     (1000)        0 2024-03-25 15:44:57.000000 pytoolbox-14.8.2/pytoolbox/django/test/__init__.py
+-rw-rw-r--   0 david     (1000) david     (1000)     4796 2024-03-25 15:44:57.000000 pytoolbox-14.8.2/pytoolbox/django/test/mixins.py
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2024-04-03 10:21:27.029096 pytoolbox-14.8.2/pytoolbox/django/test/runner/
+-rw-rw-r--   0 david     (1000) david     (1000)        0 2024-03-25 15:44:57.000000 pytoolbox-14.8.2/pytoolbox/django/test/runner/__init__.py
+-rw-rw-r--   0 david     (1000) david     (1000)      878 2024-03-25 15:44:57.000000 pytoolbox-14.8.2/pytoolbox/django/test/runner/mixins.py
+-rw-rw-r--   0 david     (1000) david     (1000)      614 2024-03-25 15:44:57.000000 pytoolbox-14.8.2/pytoolbox/django/urls.py
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2024-04-03 10:21:27.029096 pytoolbox-14.8.2/pytoolbox/django/utils/
+-rw-rw-r--   0 david     (1000) david     (1000)        0 2024-03-25 15:44:57.000000 pytoolbox-14.8.2/pytoolbox/django/utils/__init__.py
+-rw-rw-r--   0 david     (1000) david     (1000)     2375 2024-03-25 15:44:57.000000 pytoolbox-14.8.2/pytoolbox/django/utils/collections.py
+-rw-rw-r--   0 david     (1000) david     (1000)     1660 2024-03-25 15:44:57.000000 pytoolbox-14.8.2/pytoolbox/django/utils/logging.py
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2024-04-03 10:21:27.033096 pytoolbox-14.8.2/pytoolbox/django/views/
+-rw-rw-r--   0 david     (1000) david     (1000)       28 2024-03-25 15:44:57.000000 pytoolbox-14.8.2/pytoolbox/django/views/__init__.py
+-rw-rw-r--   0 david     (1000) david     (1000)      511 2024-03-25 15:44:57.000000 pytoolbox-14.8.2/pytoolbox/django/views/base.py
+-rw-rw-r--   0 david     (1000) david     (1000)     4927 2024-03-25 15:44:57.000000 pytoolbox-14.8.2/pytoolbox/django/views/mixins.py
+-rw-rw-r--   0 david     (1000) david     (1000)      317 2024-03-25 15:44:57.000000 pytoolbox-14.8.2/pytoolbox/django/views/utils.py
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2024-04-03 10:21:27.033096 pytoolbox-14.8.2/pytoolbox/django_datatable_view/
+-rw-rw-r--   0 david     (1000) david     (1000)        0 2024-03-25 15:44:57.000000 pytoolbox-14.8.2/pytoolbox/django_datatable_view/__init__.py
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2024-04-03 10:21:27.033096 pytoolbox-14.8.2/pytoolbox/django_datatable_view/views/
+-rw-rw-r--   0 david     (1000) david     (1000)        0 2024-03-25 15:44:57.000000 pytoolbox-14.8.2/pytoolbox/django_datatable_view/views/__init__.py
+-rw-rw-r--   0 david     (1000) david     (1000)     1767 2024-03-25 15:44:57.000000 pytoolbox-14.8.2/pytoolbox/django_datatable_view/views/mixins.py
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2024-04-03 10:21:27.033096 pytoolbox-14.8.2/pytoolbox/django_filter/
+-rw-rw-r--   0 david     (1000) david     (1000)        0 2024-03-25 15:44:57.000000 pytoolbox-14.8.2/pytoolbox/django_filter/__init__.py
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2024-04-03 10:21:27.033096 pytoolbox-14.8.2/pytoolbox/django_filter/filterset/
+-rw-rw-r--   0 david     (1000) david     (1000)        0 2024-03-25 15:44:57.000000 pytoolbox-14.8.2/pytoolbox/django_filter/filterset/__init__.py
+-rw-rw-r--   0 david     (1000) david     (1000)      752 2024-04-02 11:17:02.000000 pytoolbox-14.8.2/pytoolbox/django_filter/filterset/mixins.py
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2024-04-03 10:21:27.037096 pytoolbox-14.8.2/pytoolbox/django_formtools/
+-rw-rw-r--   0 david     (1000) david     (1000)        0 2024-03-25 15:44:57.000000 pytoolbox-14.8.2/pytoolbox/django_formtools/__init__.py
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2024-04-03 10:21:27.037096 pytoolbox-14.8.2/pytoolbox/django_formtools/views/
+-rw-rw-r--   0 david     (1000) david     (1000)        0 2024-03-25 15:44:57.000000 pytoolbox-14.8.2/pytoolbox/django_formtools/views/__init__.py
+-rw-rw-r--   0 david     (1000) david     (1000)     3091 2024-03-25 15:44:57.000000 pytoolbox-14.8.2/pytoolbox/django_formtools/views/mixins.py
+-rw-rw-r--   0 david     (1000) david     (1000)     1570 2024-04-02 11:17:02.000000 pytoolbox-14.8.2/pytoolbox/enum.py
+-rw-rw-r--   0 david     (1000) david     (1000)     6445 2024-04-02 11:17:02.000000 pytoolbox-14.8.2/pytoolbox/exceptions.py
+-rw-rw-r--   0 david     (1000) david     (1000)    25984 2024-04-02 11:17:02.000000 pytoolbox-14.8.2/pytoolbox/filesystem.py
+-rw-rw-r--   0 david     (1000) david     (1000)     3134 2024-04-02 11:17:02.000000 pytoolbox-14.8.2/pytoolbox/flask.py
+-rw-rw-r--   0 david     (1000) david     (1000)     4322 2024-04-03 09:53:36.000000 pytoolbox-14.8.2/pytoolbox/git.py
+-rw-rw-r--   0 david     (1000) david     (1000)    11833 2024-04-02 11:17:02.000000 pytoolbox-14.8.2/pytoolbox/humanize.py
+-rw-rw-r--   0 david     (1000) david     (1000)     2417 2024-03-25 15:44:57.000000 pytoolbox-14.8.2/pytoolbox/itertools.py
+-rw-rw-r--   0 david     (1000) david     (1000)    49307 2024-04-02 11:17:02.000000 pytoolbox-14.8.2/pytoolbox/juju.py
+-rw-rw-r--   0 david     (1000) david     (1000)     1120 2024-03-25 15:44:57.000000 pytoolbox-14.8.2/pytoolbox/linux.py
+-rw-rw-r--   0 david     (1000) david     (1000)     6085 2024-04-03 09:53:50.000000 pytoolbox-14.8.2/pytoolbox/logging.py
+-rw-rw-r--   0 david     (1000) david     (1000)      424 2024-03-25 15:44:57.000000 pytoolbox-14.8.2/pytoolbox/module.py
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2024-04-03 10:21:27.037096 pytoolbox-14.8.2/pytoolbox/multimedia/
+-rw-rw-r--   0 david     (1000) david     (1000)        0 2024-03-25 15:44:57.000000 pytoolbox-14.8.2/pytoolbox/multimedia/__init__.py
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2024-04-03 10:21:27.045096 pytoolbox-14.8.2/pytoolbox/multimedia/exif/
+-rw-rw-r--   0 david     (1000) david     (1000)      344 2024-03-25 15:44:57.000000 pytoolbox-14.8.2/pytoolbox/multimedia/exif/__init__.py
+-rw-rw-r--   0 david     (1000) david     (1000)     1654 2024-03-25 15:44:57.000000 pytoolbox-14.8.2/pytoolbox/multimedia/exif/brand.py
+-rw-rw-r--   0 david     (1000) david     (1000)      642 2024-03-25 15:44:57.000000 pytoolbox-14.8.2/pytoolbox/multimedia/exif/camera.py
+-rw-rw-r--   0 david     (1000) david     (1000)     1145 2024-04-02 11:17:02.000000 pytoolbox-14.8.2/pytoolbox/multimedia/exif/equipment.py
+-rw-rw-r--   0 david     (1000) david     (1000)     1914 2024-03-25 15:44:57.000000 pytoolbox-14.8.2/pytoolbox/multimedia/exif/image.py
+-rw-rw-r--   0 david     (1000) david     (1000)      907 2024-03-25 15:44:57.000000 pytoolbox-14.8.2/pytoolbox/multimedia/exif/lens.py
+-rw-rw-r--   0 david     (1000) david     (1000)     2579 2024-04-02 11:17:02.000000 pytoolbox-14.8.2/pytoolbox/multimedia/exif/metadata.py
+-rw-rw-r--   0 david     (1000) david     (1000)     1847 2024-03-25 15:44:57.000000 pytoolbox-14.8.2/pytoolbox/multimedia/exif/photo.py
+-rw-rw-r--   0 david     (1000) david     (1000)     3909 2024-04-02 11:17:02.000000 pytoolbox-14.8.2/pytoolbox/multimedia/exif/tag.py
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2024-04-03 10:21:27.045096 pytoolbox-14.8.2/pytoolbox/multimedia/ffmpeg/
+-rw-rw-r--   0 david     (1000) david     (1000)      672 2024-03-25 15:44:57.000000 pytoolbox-14.8.2/pytoolbox/multimedia/ffmpeg/__init__.py
+-rw-rw-r--   0 david     (1000) david     (1000)     7270 2024-03-25 15:44:57.000000 pytoolbox-14.8.2/pytoolbox/multimedia/ffmpeg/encode.py
+-rw-rw-r--   0 david     (1000) david     (1000)     5898 2024-03-25 15:44:57.000000 pytoolbox-14.8.2/pytoolbox/multimedia/ffmpeg/ffmpeg.py
+-rw-rw-r--   0 david     (1000) david     (1000)     8566 2024-03-25 15:44:57.000000 pytoolbox-14.8.2/pytoolbox/multimedia/ffmpeg/ffprobe.py
+-rw-rw-r--   0 david     (1000) david     (1000)     9639 2024-03-25 15:44:57.000000 pytoolbox-14.8.2/pytoolbox/multimedia/ffmpeg/miscellaneous.py
+-rw-rw-r--   0 david     (1000) david     (1000)     1809 2024-03-25 15:44:57.000000 pytoolbox-14.8.2/pytoolbox/multimedia/ffmpeg/utils.py
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2024-04-03 10:21:27.049096 pytoolbox-14.8.2/pytoolbox/multimedia/image/
+-rw-rw-r--   0 david     (1000) david     (1000)     2302 2024-03-25 15:44:57.000000 pytoolbox-14.8.2/pytoolbox/multimedia/image/PIL.py
+-rw-rw-r--   0 david     (1000) david     (1000)        0 2024-03-25 15:44:57.000000 pytoolbox-14.8.2/pytoolbox/multimedia/image/__init__.py
+-rw-rw-r--   0 david     (1000) david     (1000)     1699 2024-03-25 15:44:57.000000 pytoolbox-14.8.2/pytoolbox/multimedia/x264.py
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2024-04-03 10:21:27.053097 pytoolbox-14.8.2/pytoolbox/network/
+-rw-rw-r--   0 david     (1000) david     (1000)        0 2024-03-25 15:44:57.000000 pytoolbox-14.8.2/pytoolbox/network/__init__.py
+-rw-rw-r--   0 david     (1000) david     (1000)    11608 2024-03-25 15:44:57.000000 pytoolbox-14.8.2/pytoolbox/network/http.py
+-rw-rw-r--   0 david     (1000) david     (1000)     1151 2024-03-25 15:44:57.000000 pytoolbox-14.8.2/pytoolbox/network/ip.py
+-rw-rw-r--   0 david     (1000) david     (1000)    15650 2024-04-02 11:17:02.000000 pytoolbox-14.8.2/pytoolbox/network/rtp.py
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2024-04-03 10:21:27.057097 pytoolbox-14.8.2/pytoolbox/network/smpte2022/
+-rw-rw-r--   0 david     (1000) david     (1000)        0 2024-03-25 15:44:57.000000 pytoolbox-14.8.2/pytoolbox/network/smpte2022/__init__.py
+-rw-rw-r--   0 david     (1000) david     (1000)    27733 2024-04-02 11:17:02.000000 pytoolbox-14.8.2/pytoolbox/network/smpte2022/base.py
+-rw-rw-r--   0 david     (1000) david     (1000)    10420 2024-03-25 15:44:57.000000 pytoolbox-14.8.2/pytoolbox/network/smpte2022/generator.py
+-rw-rw-r--   0 david     (1000) david     (1000)    27854 2024-03-25 15:44:57.000000 pytoolbox-14.8.2/pytoolbox/network/smpte2022/receiver.py
+-rw-rw-r--   0 david     (1000) david     (1000)      916 2024-03-25 15:44:57.000000 pytoolbox-14.8.2/pytoolbox/network/url.py
+-rw-rw-r--   0 david     (1000) david     (1000)      527 2024-03-25 15:44:57.000000 pytoolbox-14.8.2/pytoolbox/pandas.py
+-rw-rw-r--   0 david     (1000) david     (1000)      466 2024-03-25 15:44:57.000000 pytoolbox-14.8.2/pytoolbox/private.py
+-rw-rw-r--   0 david     (1000) david     (1000)     5330 2024-04-02 11:17:02.000000 pytoolbox-14.8.2/pytoolbox/regex.py
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2024-04-03 10:21:27.057097 pytoolbox-14.8.2/pytoolbox/rest_framework/
+-rw-rw-r--   0 david     (1000) david     (1000)        0 2024-03-25 15:44:57.000000 pytoolbox-14.8.2/pytoolbox/rest_framework/__init__.py
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2024-04-03 10:21:27.057097 pytoolbox-14.8.2/pytoolbox/rest_framework/metadata/
+-rw-rw-r--   0 david     (1000) david     (1000)        0 2024-03-25 15:44:57.000000 pytoolbox-14.8.2/pytoolbox/rest_framework/metadata/__init__.py
+-rw-rw-r--   0 david     (1000) david     (1000)     1106 2024-04-02 11:17:02.000000 pytoolbox-14.8.2/pytoolbox/rest_framework/metadata/mixins.py
+-rw-rw-r--   0 david     (1000) david     (1000)      717 2024-03-25 15:44:57.000000 pytoolbox-14.8.2/pytoolbox/rest_framework/permissions.py
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2024-04-03 10:21:27.057097 pytoolbox-14.8.2/pytoolbox/rest_framework/serializers/
+-rw-rw-r--   0 david     (1000) david     (1000)        0 2024-03-25 15:44:57.000000 pytoolbox-14.8.2/pytoolbox/rest_framework/serializers/__init__.py
+-rw-rw-r--   0 david     (1000) david     (1000)      777 2024-03-25 15:44:57.000000 pytoolbox-14.8.2/pytoolbox/rest_framework/serializers/fields.py
+-rw-rw-r--   0 david     (1000) david     (1000)     2238 2024-03-25 15:44:57.000000 pytoolbox-14.8.2/pytoolbox/rest_framework/serializers/mixins.py
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2024-04-03 10:21:27.061097 pytoolbox-14.8.2/pytoolbox/rest_framework/views/
+-rw-rw-r--   0 david     (1000) david     (1000)        0 2024-03-25 15:44:57.000000 pytoolbox-14.8.2/pytoolbox/rest_framework/views/__init__.py
+-rw-rw-r--   0 david     (1000) david     (1000)     1571 2024-03-25 15:44:57.000000 pytoolbox-14.8.2/pytoolbox/rest_framework/views/mixins.py
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2024-04-03 10:21:27.065097 pytoolbox-14.8.2/pytoolbox/selenium/
+-rw-rw-r--   0 david     (1000) david     (1000)      149 2024-03-25 15:44:57.000000 pytoolbox-14.8.2/pytoolbox/selenium/__init__.py
+-rw-rw-r--   0 david     (1000) david     (1000)     3349 2024-03-25 15:44:57.000000 pytoolbox-14.8.2/pytoolbox/selenium/client.py
+-rw-rw-r--   0 david     (1000) david     (1000)     1343 2024-03-25 15:44:57.000000 pytoolbox-14.8.2/pytoolbox/selenium/common.py
+-rw-rw-r--   0 david     (1000) david     (1000)      464 2024-03-25 15:44:57.000000 pytoolbox-14.8.2/pytoolbox/selenium/exceptions.py
+-rw-rw-r--   0 david     (1000) david     (1000)      266 2024-03-25 15:44:57.000000 pytoolbox-14.8.2/pytoolbox/selenium/select.py
+-rw-rw-r--   0 david     (1000) david     (1000)     2631 2024-04-02 11:17:02.000000 pytoolbox-14.8.2/pytoolbox/selenium/test.py
+-rw-rw-r--   0 david     (1000) david     (1000)      815 2024-03-25 15:44:57.000000 pytoolbox-14.8.2/pytoolbox/selenium/webdrivers.py
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2024-04-03 10:21:27.069097 pytoolbox-14.8.2/pytoolbox/selenium/webelements/
+-rw-rw-r--   0 david     (1000) david     (1000)      186 2024-03-25 15:44:57.000000 pytoolbox-14.8.2/pytoolbox/selenium/webelements/__init__.py
+-rw-rw-r--   0 david     (1000) david     (1000)     1109 2024-03-25 15:44:57.000000 pytoolbox-14.8.2/pytoolbox/selenium/webelements/base.py
+-rw-rw-r--   0 david     (1000) david     (1000)     1030 2024-03-25 15:44:57.000000 pytoolbox-14.8.2/pytoolbox/selenium/webelements/bootstrap_slider.py
+-rw-rw-r--   0 david     (1000) david     (1000)      473 2024-03-25 15:44:57.000000 pytoolbox-14.8.2/pytoolbox/selenium/webelements/bootstrap_switch.py
+-rw-rw-r--   0 david     (1000) david     (1000)    21143 2024-04-02 11:17:02.000000 pytoolbox-14.8.2/pytoolbox/serialization.py
+-rw-rw-r--   0 david     (1000) david     (1000)      452 2024-03-25 15:44:57.000000 pytoolbox-14.8.2/pytoolbox/setuptools.py
+-rw-rw-r--   0 david     (1000) david     (1000)     1650 2024-03-25 15:44:57.000000 pytoolbox-14.8.2/pytoolbox/signals.py
+-rw-rw-r--   0 david     (1000) david     (1000)     3402 2024-04-02 11:17:02.000000 pytoolbox-14.8.2/pytoolbox/ssh.py
+-rw-rw-r--   0 david     (1000) david     (1000)     2875 2024-03-25 15:44:57.000000 pytoolbox-14.8.2/pytoolbox/states.py
+-rw-rw-r--   0 david     (1000) david     (1000)     4864 2024-03-25 15:44:57.000000 pytoolbox-14.8.2/pytoolbox/string.py
+-rw-rw-r--   0 david     (1000) david     (1000)    13522 2024-04-03 09:19:26.000000 pytoolbox-14.8.2/pytoolbox/subprocess.py
+-rw-rw-r--   0 david     (1000) david     (1000)     3407 2024-03-25 15:44:57.000000 pytoolbox-14.8.2/pytoolbox/throttles.py
+-rw-rw-r--   0 david     (1000) david     (1000)     8965 2024-04-02 11:17:02.000000 pytoolbox-14.8.2/pytoolbox/types.py
+-rw-rw-r--   0 david     (1000) david     (1000)    10931 2024-03-25 15:44:57.000000 pytoolbox-14.8.2/pytoolbox/unittest.py
+-rw-rw-r--   0 david     (1000) david     (1000)     9644 2024-04-02 11:17:02.000000 pytoolbox-14.8.2/pytoolbox/validation.py
+-rw-rw-r--   0 david     (1000) david     (1000)     1164 2024-03-25 15:44:57.000000 pytoolbox-14.8.2/pytoolbox/virtualenv.py
+-rw-rw-r--   0 david     (1000) david     (1000)     2160 2024-03-25 15:44:57.000000 pytoolbox-14.8.2/pytoolbox/voluptuous.py
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2024-04-03 10:21:27.081097 pytoolbox-14.8.2/pytoolbox.egg-info/
+-rw-r--r--   0 david     (1000) david     (1000)    11167 2024-04-03 10:21:26.000000 pytoolbox-14.8.2/pytoolbox.egg-info/PKG-INFO
+-rw-rw-r--   0 david     (1000) david     (1000)     5548 2024-04-03 10:21:26.000000 pytoolbox-14.8.2/pytoolbox.egg-info/SOURCES.txt
+-rw-rw-r--   0 david     (1000) david     (1000)        1 2024-04-03 10:21:26.000000 pytoolbox-14.8.2/pytoolbox.egg-info/dependency_links.txt
+-rw-rw-r--   0 david     (1000) david     (1000)     1042 2024-04-03 10:21:26.000000 pytoolbox-14.8.2/pytoolbox.egg-info/requires.txt
+-rw-rw-r--   0 david     (1000) david     (1000)       10 2024-04-03 10:21:26.000000 pytoolbox-14.8.2/pytoolbox.egg-info/top_level.txt
+-rw-rw-r--   0 david     (1000) david     (1000)      144 2024-04-03 10:21:27.109097 pytoolbox-14.8.2/setup.cfg
+-rwxrwxr-x   0 david     (1000) david     (1000)     8796 2024-03-25 15:44:57.000000 pytoolbox-14.8.2/setup.py
+drwxrwxr-x   0 david     (1000) david     (1000)        0 2024-04-03 10:21:27.081097 pytoolbox-14.8.2/tests/
+-rw-rw-r--   0 david     (1000) david     (1000)     2961 2024-04-02 11:17:02.000000 pytoolbox-14.8.2/tests/test_argparse.py
+-rw-rw-r--   0 david     (1000) david     (1000)     1237 2024-03-25 15:44:57.000000 pytoolbox-14.8.2/tests/test_collections.py
+-rw-rw-r--   0 david     (1000) david     (1000)     4691 2024-04-02 11:17:02.000000 pytoolbox-14.8.2/tests/test_comparison.py
+-rw-rw-r--   0 david     (1000) david     (1000)      832 2024-03-25 15:44:57.000000 pytoolbox-14.8.2/tests/test_console.py
+-rw-rw-r--   0 david     (1000) david     (1000)      514 2024-03-25 15:44:57.000000 pytoolbox-14.8.2/tests/test_decorators.py
+-rw-rw-r--   0 david     (1000) david     (1000)      668 2024-03-25 15:44:57.000000 pytoolbox-14.8.2/tests/test_django_utils.py
+-rw-rw-r--   0 david     (1000) david     (1000)     2185 2024-04-02 11:17:02.000000 pytoolbox-14.8.2/tests/test_exceptions.py
+-rw-rw-r--   0 david     (1000) david     (1000)    16098 2024-03-25 15:44:57.000000 pytoolbox-14.8.2/tests/test_ffmpeg.py
+-rw-rw-r--   0 david     (1000) david     (1000)     2555 2024-03-25 15:44:57.000000 pytoolbox-14.8.2/tests/test_filesystem.py
+-rw-rw-r--   0 david     (1000) david     (1000)     5059 2024-04-02 11:38:59.000000 pytoolbox-14.8.2/tests/test_git.py
+-rw-rw-r--   0 david     (1000) david     (1000)     2887 2024-03-25 15:44:57.000000 pytoolbox-14.8.2/tests/test_juju.py
+-rw-rw-r--   0 david     (1000) david     (1000)      813 2024-04-02 11:17:02.000000 pytoolbox-14.8.2/tests/test_logging.py
+-rw-rw-r--   0 david     (1000) david     (1000)      705 2024-03-25 15:44:57.000000 pytoolbox-14.8.2/tests/test_module.py
+-rw-rw-r--   0 david     (1000) david     (1000)      692 2024-03-25 15:44:57.000000 pytoolbox-14.8.2/tests/test_private.py
+-rw-rw-r--   0 david     (1000) david     (1000)     2068 2024-03-25 15:44:57.000000 pytoolbox-14.8.2/tests/test_regex.py
+-rw-rw-r--   0 david     (1000) david     (1000)     1679 2024-03-25 15:44:57.000000 pytoolbox-14.8.2/tests/test_serialization.py
+-rw-rw-r--   0 david     (1000) david     (1000)     2699 2024-03-25 15:44:57.000000 pytoolbox-14.8.2/tests/test_signals.py
+-rw-rw-r--   0 david     (1000) david     (1000)     4525 2024-03-25 15:44:57.000000 pytoolbox-14.8.2/tests/test_ssh.py
+-rw-rw-r--   0 david     (1000) david     (1000)     4125 2024-03-25 15:44:57.000000 pytoolbox-14.8.2/tests/test_states.py
+-rw-rw-r--   0 david     (1000) david     (1000)     2873 2024-03-25 15:44:57.000000 pytoolbox-14.8.2/tests/test_string.py
+-rw-rw-r--   0 david     (1000) david     (1000)     6002 2024-04-02 11:17:02.000000 pytoolbox-14.8.2/tests/test_subprocess.py
+-rw-rw-r--   0 david     (1000) david     (1000)      338 2024-03-25 15:44:57.000000 pytoolbox-14.8.2/tests/test_types.py
+-rw-rw-r--   0 david     (1000) david     (1000)     5981 2024-03-25 15:44:57.000000 pytoolbox-14.8.2/tests/test_unittest.py
+-rw-rw-r--   0 david     (1000) david     (1000)      637 2024-03-25 15:44:57.000000 pytoolbox-14.8.2/tests/test_validation.py
+-rw-rw-r--   0 david     (1000) david     (1000)      433 2024-03-25 15:44:57.000000 pytoolbox-14.8.2/tests/test_x264.py
```

### Comparing `pytoolbox-14.8.1/CHANGELOG.md` & `pytoolbox-14.8.2/CHANGELOG.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,25 @@
 # Changelog
 
 Roadmap ? Not so, but you can check this: https://github.com/davidfischer-ch/pytoolbox/issues
 
+## v14.8.2 (2024-04-03)
+
+Diff: https://github.com/davidfischer-ch/pytoolbox/compare/14.8.1...14.8.2
+
+### Features
+
+* Add TypeAlias `git.RefKind` and use it
+* Add function `logging.reset_logger` and use it
+
+### Fix and enhancements
+
+* Keep `git` / `subprocess` log records separated
+* Prevent a strange issue when reloading logging module
+
 ## v14.8.1 (2024-04-02)
 
 Diff: https://github.com/davidfischer-ch/pytoolbox/compare/14.8.0...14.8.1
 
 ### Deprecations
 
 * Replace your calls to `argparse.set_columns` by `console.set_columns`
```

### Comparing `pytoolbox-14.8.1/LICENSE.rst` & `pytoolbox-14.8.2/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `pytoolbox-14.8.1/PKG-INFO` & `pytoolbox-14.8.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytoolbox
-Version: 14.8.1
+Version: 14.8.2
 Summary: Toolbox for Python scripts
 Home-page: https://github.com/davidfischer-ch/pytoolbox
 Author: David Fischer
 Author-email: david@fisch3r.net
 License: EUPL 1.1
 Keywords: celery,ffmpeg,django,flask,json,juju,mock,pillow,rsync,rtp,selenium,smpte 2022-1,screen,subprocess
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `pytoolbox-14.8.1/README.rst` & `pytoolbox-14.8.2/README.rst`

 * *Files identical despite different names*

### Comparing `pytoolbox-14.8.1/pytoolbox/ai/vision/face/detect/dlib.py` & `pytoolbox-14.8.2/pytoolbox/ai/vision/face/detect/dlib.py`

 * *Files identical despite different names*

### Comparing `pytoolbox-14.8.1/pytoolbox/ai/vision/face/recognize/nn4_small2.py` & `pytoolbox-14.8.2/pytoolbox/ai/vision/face/recognize/nn4_small2.py`

 * *Files identical despite different names*

### Comparing `pytoolbox-14.8.1/pytoolbox/ai/vision/utils.py` & `pytoolbox-14.8.2/pytoolbox/ai/vision/utils.py`

 * *Files identical despite different names*

### Comparing `pytoolbox-14.8.1/pytoolbox/argparse.py` & `pytoolbox-14.8.2/pytoolbox/argparse.py`

 * *Files identical despite different names*

### Comparing `pytoolbox-14.8.1/pytoolbox/atlassian.py` & `pytoolbox-14.8.2/pytoolbox/atlassian.py`

 * *Files identical despite different names*

### Comparing `pytoolbox-14.8.1/pytoolbox/aws/s3.py` & `pytoolbox-14.8.2/pytoolbox/aws/s3.py`

 * *Files identical despite different names*

### Comparing `pytoolbox-14.8.1/pytoolbox/collections.py` & `pytoolbox-14.8.2/pytoolbox/collections.py`

 * *Files identical despite different names*

### Comparing `pytoolbox-14.8.1/pytoolbox/comparison.py` & `pytoolbox-14.8.2/pytoolbox/comparison.py`

 * *Files identical despite different names*

### Comparing `pytoolbox-14.8.1/pytoolbox/console.py` & `pytoolbox-14.8.2/pytoolbox/console.py`

 * *Files identical despite different names*

### Comparing `pytoolbox-14.8.1/pytoolbox/crypto.py` & `pytoolbox-14.8.2/pytoolbox/crypto.py`

 * *Files identical despite different names*

### Comparing `pytoolbox-14.8.1/pytoolbox/datetime.py` & `pytoolbox-14.8.2/pytoolbox/datetime.py`

 * *Files identical despite different names*

### Comparing `pytoolbox-14.8.1/pytoolbox/decorators.py` & `pytoolbox-14.8.2/pytoolbox/decorators.py`

 * *Files identical despite different names*

### Comparing `pytoolbox-14.8.1/pytoolbox/django/core/exceptions.py` & `pytoolbox-14.8.2/pytoolbox/django/core/exceptions.py`

 * *Files identical despite different names*

### Comparing `pytoolbox-14.8.1/pytoolbox/django/core/validators.py` & `pytoolbox-14.8.2/pytoolbox/django/core/validators.py`

 * *Files identical despite different names*

### Comparing `pytoolbox-14.8.1/pytoolbox/django/forms/base.py` & `pytoolbox-14.8.2/pytoolbox/django/forms/base.py`

 * *Files identical despite different names*

### Comparing `pytoolbox-14.8.1/pytoolbox/django/forms/fields.py` & `pytoolbox-14.8.2/pytoolbox/django/forms/fields.py`

 * *Files identical despite different names*

### Comparing `pytoolbox-14.8.1/pytoolbox/django/forms/mixins.py` & `pytoolbox-14.8.2/pytoolbox/django/forms/mixins.py`

 * *Files identical despite different names*

### Comparing `pytoolbox-14.8.1/pytoolbox/django/forms/utils.py` & `pytoolbox-14.8.2/pytoolbox/django/forms/utils.py`

 * *Files identical despite different names*

### Comparing `pytoolbox-14.8.1/pytoolbox/django/forms/widgets.py` & `pytoolbox-14.8.2/pytoolbox/django/forms/widgets.py`

 * *Files identical despite different names*

### Comparing `pytoolbox-14.8.1/pytoolbox/django/models/decorators.py` & `pytoolbox-14.8.2/pytoolbox/django/models/decorators.py`

 * *Files identical despite different names*

### Comparing `pytoolbox-14.8.1/pytoolbox/django/models/fields/base.py` & `pytoolbox-14.8.2/pytoolbox/django/models/fields/base.py`

 * *Files identical despite different names*

### Comparing `pytoolbox-14.8.1/pytoolbox/django/models/fields/mixins.py` & `pytoolbox-14.8.2/pytoolbox/django/models/fields/mixins.py`

 * *Files identical despite different names*

### Comparing `pytoolbox-14.8.1/pytoolbox/django/models/managers/mixins.py` & `pytoolbox-14.8.2/pytoolbox/django/models/managers/mixins.py`

 * *Files identical despite different names*

### Comparing `pytoolbox-14.8.1/pytoolbox/django/models/mixins.py` & `pytoolbox-14.8.2/pytoolbox/django/models/mixins.py`

 * *Files identical despite different names*

### Comparing `pytoolbox-14.8.1/pytoolbox/django/models/query/mixins.py` & `pytoolbox-14.8.2/pytoolbox/django/models/query/mixins.py`

 * *Files identical despite different names*

### Comparing `pytoolbox-14.8.1/pytoolbox/django/models/utils.py` & `pytoolbox-14.8.2/pytoolbox/django/models/utils.py`

 * *Files identical despite different names*

### Comparing `pytoolbox-14.8.1/pytoolbox/django/signals/dispatch.py` & `pytoolbox-14.8.2/pytoolbox/django/signals/dispatch.py`

 * *Files identical despite different names*

### Comparing `pytoolbox-14.8.1/pytoolbox/django/signals/handlers.py` & `pytoolbox-14.8.2/pytoolbox/django/signals/handlers.py`

 * *Files identical despite different names*

### Comparing `pytoolbox-14.8.1/pytoolbox/django/storage.py` & `pytoolbox-14.8.2/pytoolbox/django/storage.py`

 * *Files identical despite different names*

### Comparing `pytoolbox-14.8.1/pytoolbox/django/templatetags.py` & `pytoolbox-14.8.2/pytoolbox/django/templatetags.py`

 * *Files identical despite different names*

### Comparing `pytoolbox-14.8.1/pytoolbox/django/test/mixins.py` & `pytoolbox-14.8.2/pytoolbox/django/test/mixins.py`

 * *Files identical despite different names*

### Comparing `pytoolbox-14.8.1/pytoolbox/django/test/runner/mixins.py` & `pytoolbox-14.8.2/pytoolbox/django/test/runner/mixins.py`

 * *Files identical despite different names*

### Comparing `pytoolbox-14.8.1/pytoolbox/django/urls.py` & `pytoolbox-14.8.2/pytoolbox/django/urls.py`

 * *Files identical despite different names*

### Comparing `pytoolbox-14.8.1/pytoolbox/django/utils/collections.py` & `pytoolbox-14.8.2/pytoolbox/django/utils/collections.py`

 * *Files identical despite different names*

### Comparing `pytoolbox-14.8.1/pytoolbox/django/utils/logging.py` & `pytoolbox-14.8.2/pytoolbox/django/utils/logging.py`

 * *Files identical despite different names*

### Comparing `pytoolbox-14.8.1/pytoolbox/django/views/mixins.py` & `pytoolbox-14.8.2/pytoolbox/django/views/mixins.py`

 * *Files identical despite different names*

### Comparing `pytoolbox-14.8.1/pytoolbox/django_datatable_view/views/mixins.py` & `pytoolbox-14.8.2/pytoolbox/django_datatable_view/views/mixins.py`

 * *Files identical despite different names*

### Comparing `pytoolbox-14.8.1/pytoolbox/django_filter/filterset/mixins.py` & `pytoolbox-14.8.2/pytoolbox/django_filter/filterset/mixins.py`

 * *Files identical despite different names*

### Comparing `pytoolbox-14.8.1/pytoolbox/django_formtools/views/mixins.py` & `pytoolbox-14.8.2/pytoolbox/django_formtools/views/mixins.py`

 * *Files identical despite different names*

### Comparing `pytoolbox-14.8.1/pytoolbox/enum.py` & `pytoolbox-14.8.2/pytoolbox/enum.py`

 * *Files identical despite different names*

### Comparing `pytoolbox-14.8.1/pytoolbox/exceptions.py` & `pytoolbox-14.8.2/pytoolbox/exceptions.py`

 * *Files identical despite different names*

### Comparing `pytoolbox-14.8.1/pytoolbox/filesystem.py` & `pytoolbox-14.8.2/pytoolbox/filesystem.py`

 * *Files identical despite different names*

### Comparing `pytoolbox-14.8.1/pytoolbox/flask.py` & `pytoolbox-14.8.2/pytoolbox/flask.py`

 * *Files identical despite different names*

### Comparing `pytoolbox-14.8.1/pytoolbox/git.py` & `pytoolbox-14.8.2/pytoolbox/git.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,22 +1,33 @@
 from __future__ import annotations
 
 from collections.abc import Iterable, Iterator
 from pathlib import Path
+from typing import Literal, TypeAlias
 import contextlib
 import os
 import stat
 import tempfile
 
 from . import exceptions, humanize, logging, subprocess
 from .subprocess import CallArgType
 
 log = logging.get_logger(__name__)
 
-__all__ = ['blame', 'clone_or_pull', 'create_tag', 'get_ref', 'get_tags', 'scoped_ssh_key']
+__all__ = [
+    'RefKind',
+    'blame',
+    'clone_or_pull',
+    'create_tag',
+    'get_ref',
+    'get_tags',
+    'scoped_ssh_key'
+]
+
+RefKind: TypeAlias = Literal['branch', 'commit']
 
 
 def blame(file_path: Path) -> list[str]:
     lines = subprocess.cmd(
         ['git', 'blame', file_path],
         cwd=file_path.parent)['stdout'].decode('utf-8')
     return [line for line in lines.split(os.linesep) if line]
@@ -50,33 +61,35 @@
     except exceptions.CalledProcessError as ex:
         if name in get_tags(directory):
             # Parsing output is not robust since it can be in French, English, ...
             raise exceptions.DuplicateGitTagError(tag=name) from ex
         raise
 
 
-def get_ref(directory: Path | None = None, *, ci_vars: bool = True, kind: str = 'branch') -> str:
+def get_ref(
+    directory: Path | None = None,
+    *,
+    ci_vars: bool = True,
+    kind: RefKind = 'branch'
+) -> str:
     """
     Return the Git reference looking first at CI context, then using Git CLI.
 
     This function will return either:
 
     * The content of the environment variable CI_COMMIT_REF_NAME when available (GitLab CI/CD)
     * The git branch reference to point to the branch when running locally (via git CLI)
     """
     if ci_vars and (ref := os.getenv('CI_COMMIT_REF_NAME')):
         log.debug(f'Detected Git ref from GitLab CI context is {ref}')
     else:
         extra = {'branch': ['--abbrev-ref'], 'commit': []}[kind]
-        ref = subprocess.cmd(
-            ['git', 'rev-parse', *extra, 'HEAD'],
-            cwd=directory,
-            fail=False,
-            log=log)['stdout'].decode('utf-8').strip()
-        log.debug(f'Detected Git ref from directory {directory!r} of kind {kind} is {ref}')
+        result = subprocess.cmd(['git', 'rev-parse', *extra, 'HEAD'], cwd=directory, fail=False)
+        ref = result['stdout'].decode('utf-8').strip()
+        log.debug(f'Detected Git ref from directory \'{directory}\' of kind {kind} is {ref}')
     if not ref:
         raise exceptions.GitReferenceError()
     return ref
 
 
 def get_tags(directory: Path, *, ref: str | None = None) -> list[str]:
     """Return tags from local copy. Optionally restrict to tags related to given `ref`."""
```

### Comparing `pytoolbox-14.8.1/pytoolbox/humanize.py` & `pytoolbox-14.8.2/pytoolbox/humanize.py`

 * *Files identical despite different names*

### Comparing `pytoolbox-14.8.1/pytoolbox/itertools.py` & `pytoolbox-14.8.2/pytoolbox/itertools.py`

 * *Files identical despite different names*

### Comparing `pytoolbox-14.8.1/pytoolbox/juju.py` & `pytoolbox-14.8.2/pytoolbox/juju.py`

 * *Files identical despite different names*

### Comparing `pytoolbox-14.8.1/pytoolbox/linux.py` & `pytoolbox-14.8.2/pytoolbox/linux.py`

 * *Files identical despite different names*

### Comparing `pytoolbox-14.8.1/pytoolbox/logging.py` & `pytoolbox-14.8.2/pytoolbox/logging.py`

 * *Files 13% similar despite different names*

```diff
@@ -19,14 +19,15 @@
     'Color',
     'BasicLoggerFunc',
     'BasicFuncLogger',
     'LoggerType',
     'Logger',
     'LogRecord',
     'get_logger',
+    'reset_logger',
     'setup_logging',
     'ColorizeFilter'
 ]
 
 CRITICAL: int = logging.CRITICAL
 FATAL: int = logging.FATAL
 ERROR: int = logging.ERROR
@@ -76,21 +77,41 @@
 LoggerType: TypeAlias = BasicLoggerFunc | logging.Logger | str | None
 Logger = logging.Logger
 LogRecord = logging.LogRecord
 
 
 def get_logger(log: LoggerType) -> logging.Logger:
     """Convenient function returning an instance of logger for various use cases."""
-    if isinstance(log, logging.Logger):
+    if isinstance(log, Logger):
         return log
     if isinstance(log, str):
         return logging.getLogger(log)
     if hasattr(log, '__call__'):
         return BasicFuncLogger(log_func=log)
-    raise NotImplementedError(f'Logging with {log!r}')
+    raise NotImplementedError(f'Logging with {log!r} of type {type(log)}')
+
+
+def reset_logger(log: LoggerType) -> logging.Logger:
+    log = get_logger(log)
+    log.setLevel(logging.NOTSET)
+    log.disabled = False
+    log.propagate = True
+    log.filters.clear()
+    for handler in log.handlers.copy():
+        # Copied from `logging.shutdown`
+        try:
+            handler.acquire()
+            handler.flush()
+            handler.close()
+        except (OSError, ValueError):
+            pass
+        finally:
+            handler.release()
+        log.removeHandler(handler)
+    return log
 
 
 def setup_logging(
     log: LoggerType = '',
     reset: bool = False,
     path: Path | str | None = None,
     console: bool = False,
@@ -150,15 +171,15 @@
     ...     log.info('Ceci va probablement jamais être lu!')
     ...     lines = f.read().split(os.linesep)
     ...
     >>> assert 'INFO     - Ceci va probablement jamais être lu!' in lines[0]
     """
     log = get_logger(log)
     if reset:
-        log.handlers = []
+        reset_logger(log)
     log.setLevel(level)
     if colorize:
         log.addFilter(ColorizeFilter(color_by_level=color_by_level))
     if path:
         file_handler = logging.FileHandler(path)
         file_handler.setFormatter(logging.Formatter(fmt=fmt, datefmt=datefmt))
         log.addHandler(file_handler)
```

### Comparing `pytoolbox-14.8.1/pytoolbox/multimedia/exif/brand.py` & `pytoolbox-14.8.2/pytoolbox/multimedia/exif/brand.py`

 * *Files identical despite different names*

### Comparing `pytoolbox-14.8.1/pytoolbox/multimedia/exif/camera.py` & `pytoolbox-14.8.2/pytoolbox/multimedia/exif/camera.py`

 * *Files identical despite different names*

### Comparing `pytoolbox-14.8.1/pytoolbox/multimedia/exif/equipment.py` & `pytoolbox-14.8.2/pytoolbox/multimedia/exif/equipment.py`

 * *Files identical despite different names*

### Comparing `pytoolbox-14.8.1/pytoolbox/multimedia/exif/image.py` & `pytoolbox-14.8.2/pytoolbox/multimedia/exif/image.py`

 * *Files identical despite different names*

### Comparing `pytoolbox-14.8.1/pytoolbox/multimedia/exif/lens.py` & `pytoolbox-14.8.2/pytoolbox/multimedia/exif/lens.py`

 * *Files identical despite different names*

### Comparing `pytoolbox-14.8.1/pytoolbox/multimedia/exif/metadata.py` & `pytoolbox-14.8.2/pytoolbox/multimedia/exif/metadata.py`

 * *Files identical despite different names*

### Comparing `pytoolbox-14.8.1/pytoolbox/multimedia/exif/photo.py` & `pytoolbox-14.8.2/pytoolbox/multimedia/exif/photo.py`

 * *Files identical despite different names*

### Comparing `pytoolbox-14.8.1/pytoolbox/multimedia/exif/tag.py` & `pytoolbox-14.8.2/pytoolbox/multimedia/exif/tag.py`

 * *Files identical despite different names*

### Comparing `pytoolbox-14.8.1/pytoolbox/multimedia/ffmpeg/__init__.py` & `pytoolbox-14.8.2/pytoolbox/multimedia/ffmpeg/__init__.py`

 * *Files identical despite different names*

### Comparing `pytoolbox-14.8.1/pytoolbox/multimedia/ffmpeg/encode.py` & `pytoolbox-14.8.2/pytoolbox/multimedia/ffmpeg/encode.py`

 * *Files identical despite different names*

### Comparing `pytoolbox-14.8.1/pytoolbox/multimedia/ffmpeg/ffmpeg.py` & `pytoolbox-14.8.2/pytoolbox/multimedia/ffmpeg/ffmpeg.py`

 * *Files identical despite different names*

### Comparing `pytoolbox-14.8.1/pytoolbox/multimedia/ffmpeg/ffprobe.py` & `pytoolbox-14.8.2/pytoolbox/multimedia/ffmpeg/ffprobe.py`

 * *Files identical despite different names*

### Comparing `pytoolbox-14.8.1/pytoolbox/multimedia/ffmpeg/miscellaneous.py` & `pytoolbox-14.8.2/pytoolbox/multimedia/ffmpeg/miscellaneous.py`

 * *Files identical despite different names*

### Comparing `pytoolbox-14.8.1/pytoolbox/multimedia/ffmpeg/utils.py` & `pytoolbox-14.8.2/pytoolbox/multimedia/ffmpeg/utils.py`

 * *Files identical despite different names*

### Comparing `pytoolbox-14.8.1/pytoolbox/multimedia/image/PIL.py` & `pytoolbox-14.8.2/pytoolbox/multimedia/image/PIL.py`

 * *Files identical despite different names*

### Comparing `pytoolbox-14.8.1/pytoolbox/multimedia/x264.py` & `pytoolbox-14.8.2/pytoolbox/multimedia/x264.py`

 * *Files identical despite different names*

### Comparing `pytoolbox-14.8.1/pytoolbox/network/http.py` & `pytoolbox-14.8.2/pytoolbox/network/http.py`

 * *Files identical despite different names*

### Comparing `pytoolbox-14.8.1/pytoolbox/network/ip.py` & `pytoolbox-14.8.2/pytoolbox/network/ip.py`

 * *Files identical despite different names*

### Comparing `pytoolbox-14.8.1/pytoolbox/network/rtp.py` & `pytoolbox-14.8.2/pytoolbox/network/rtp.py`

 * *Files identical despite different names*

### Comparing `pytoolbox-14.8.1/pytoolbox/network/smpte2022/base.py` & `pytoolbox-14.8.2/pytoolbox/network/smpte2022/base.py`

 * *Files identical despite different names*

### Comparing `pytoolbox-14.8.1/pytoolbox/network/smpte2022/generator.py` & `pytoolbox-14.8.2/pytoolbox/network/smpte2022/generator.py`

 * *Files identical despite different names*

### Comparing `pytoolbox-14.8.1/pytoolbox/network/smpte2022/receiver.py` & `pytoolbox-14.8.2/pytoolbox/network/smpte2022/receiver.py`

 * *Files identical despite different names*

### Comparing `pytoolbox-14.8.1/pytoolbox/network/url.py` & `pytoolbox-14.8.2/pytoolbox/network/url.py`

 * *Files identical despite different names*

### Comparing `pytoolbox-14.8.1/pytoolbox/pandas.py` & `pytoolbox-14.8.2/pytoolbox/pandas.py`

 * *Files identical despite different names*

### Comparing `pytoolbox-14.8.1/pytoolbox/regex.py` & `pytoolbox-14.8.2/pytoolbox/regex.py`

 * *Files identical despite different names*

### Comparing `pytoolbox-14.8.1/pytoolbox/rest_framework/metadata/mixins.py` & `pytoolbox-14.8.2/pytoolbox/rest_framework/metadata/mixins.py`

 * *Files identical despite different names*

### Comparing `pytoolbox-14.8.1/pytoolbox/rest_framework/permissions.py` & `pytoolbox-14.8.2/pytoolbox/rest_framework/permissions.py`

 * *Files identical despite different names*

### Comparing `pytoolbox-14.8.1/pytoolbox/rest_framework/serializers/fields.py` & `pytoolbox-14.8.2/pytoolbox/rest_framework/serializers/fields.py`

 * *Files identical despite different names*

### Comparing `pytoolbox-14.8.1/pytoolbox/rest_framework/serializers/mixins.py` & `pytoolbox-14.8.2/pytoolbox/rest_framework/serializers/mixins.py`

 * *Files identical despite different names*

### Comparing `pytoolbox-14.8.1/pytoolbox/rest_framework/views/mixins.py` & `pytoolbox-14.8.2/pytoolbox/rest_framework/views/mixins.py`

 * *Files identical despite different names*

### Comparing `pytoolbox-14.8.1/pytoolbox/selenium/client.py` & `pytoolbox-14.8.2/pytoolbox/selenium/client.py`

 * *Files identical despite different names*

### Comparing `pytoolbox-14.8.1/pytoolbox/selenium/common.py` & `pytoolbox-14.8.2/pytoolbox/selenium/common.py`

 * *Files identical despite different names*

### Comparing `pytoolbox-14.8.1/pytoolbox/selenium/test.py` & `pytoolbox-14.8.2/pytoolbox/selenium/test.py`

 * *Files identical despite different names*

### Comparing `pytoolbox-14.8.1/pytoolbox/selenium/webdrivers.py` & `pytoolbox-14.8.2/pytoolbox/selenium/webdrivers.py`

 * *Files identical despite different names*

### Comparing `pytoolbox-14.8.1/pytoolbox/selenium/webelements/base.py` & `pytoolbox-14.8.2/pytoolbox/selenium/webelements/base.py`

 * *Files identical despite different names*

### Comparing `pytoolbox-14.8.1/pytoolbox/selenium/webelements/bootstrap_slider.py` & `pytoolbox-14.8.2/pytoolbox/selenium/webelements/bootstrap_slider.py`

 * *Files identical despite different names*

### Comparing `pytoolbox-14.8.1/pytoolbox/serialization.py` & `pytoolbox-14.8.2/pytoolbox/serialization.py`

 * *Files identical despite different names*

### Comparing `pytoolbox-14.8.1/pytoolbox/signals.py` & `pytoolbox-14.8.2/pytoolbox/signals.py`

 * *Files identical despite different names*

### Comparing `pytoolbox-14.8.1/pytoolbox/ssh.py` & `pytoolbox-14.8.2/pytoolbox/ssh.py`

 * *Files identical despite different names*

### Comparing `pytoolbox-14.8.1/pytoolbox/states.py` & `pytoolbox-14.8.2/pytoolbox/states.py`

 * *Files identical despite different names*

### Comparing `pytoolbox-14.8.1/pytoolbox/string.py` & `pytoolbox-14.8.2/pytoolbox/string.py`

 * *Files identical despite different names*

### Comparing `pytoolbox-14.8.1/pytoolbox/subprocess.py` & `pytoolbox-14.8.2/pytoolbox/subprocess.py`

 * *Files identical despite different names*

### Comparing `pytoolbox-14.8.1/pytoolbox/throttles.py` & `pytoolbox-14.8.2/pytoolbox/throttles.py`

 * *Files identical despite different names*

### Comparing `pytoolbox-14.8.1/pytoolbox/types.py` & `pytoolbox-14.8.2/pytoolbox/types.py`

 * *Files identical despite different names*

### Comparing `pytoolbox-14.8.1/pytoolbox/unittest.py` & `pytoolbox-14.8.2/pytoolbox/unittest.py`

 * *Files identical despite different names*

### Comparing `pytoolbox-14.8.1/pytoolbox/validation.py` & `pytoolbox-14.8.2/pytoolbox/validation.py`

 * *Files identical despite different names*

### Comparing `pytoolbox-14.8.1/pytoolbox/virtualenv.py` & `pytoolbox-14.8.2/pytoolbox/virtualenv.py`

 * *Files identical despite different names*

### Comparing `pytoolbox-14.8.1/pytoolbox/voluptuous.py` & `pytoolbox-14.8.2/pytoolbox/voluptuous.py`

 * *Files identical despite different names*

### Comparing `pytoolbox-14.8.1/pytoolbox.egg-info/PKG-INFO` & `pytoolbox-14.8.2/pytoolbox.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytoolbox
-Version: 14.8.1
+Version: 14.8.2
 Summary: Toolbox for Python scripts
 Home-page: https://github.com/davidfischer-ch/pytoolbox
 Author: David Fischer
 Author-email: david@fisch3r.net
 License: EUPL 1.1
 Keywords: celery,ffmpeg,django,flask,json,juju,mock,pillow,rsync,rtp,selenium,smpte 2022-1,screen,subprocess
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `pytoolbox-14.8.1/pytoolbox.egg-info/SOURCES.txt` & `pytoolbox-14.8.2/pytoolbox.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pytoolbox-14.8.1/pytoolbox.egg-info/requires.txt` & `pytoolbox-14.8.2/pytoolbox.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `pytoolbox-14.8.1/setup.py` & `pytoolbox-14.8.2/setup.py`

 * *Files identical despite different names*

### Comparing `pytoolbox-14.8.1/tests/test_argparse.py` & `pytoolbox-14.8.2/tests/test_argparse.py`

 * *Files identical despite different names*

### Comparing `pytoolbox-14.8.1/tests/test_collections.py` & `pytoolbox-14.8.2/tests/test_collections.py`

 * *Files identical despite different names*

### Comparing `pytoolbox-14.8.1/tests/test_comparison.py` & `pytoolbox-14.8.2/tests/test_comparison.py`

 * *Files identical despite different names*

### Comparing `pytoolbox-14.8.1/tests/test_console.py` & `pytoolbox-14.8.2/tests/test_console.py`

 * *Files identical despite different names*

### Comparing `pytoolbox-14.8.1/tests/test_decorators.py` & `pytoolbox-14.8.2/tests/test_decorators.py`

 * *Files identical despite different names*

### Comparing `pytoolbox-14.8.1/tests/test_django_utils.py` & `pytoolbox-14.8.2/tests/test_django_utils.py`

 * *Files identical despite different names*

### Comparing `pytoolbox-14.8.1/tests/test_exceptions.py` & `pytoolbox-14.8.2/tests/test_exceptions.py`

 * *Files identical despite different names*

### Comparing `pytoolbox-14.8.1/tests/test_ffmpeg.py` & `pytoolbox-14.8.2/tests/test_ffmpeg.py`

 * *Files identical despite different names*

### Comparing `pytoolbox-14.8.1/tests/test_filesystem.py` & `pytoolbox-14.8.2/tests/test_filesystem.py`

 * *Files identical despite different names*

### Comparing `pytoolbox-14.8.1/tests/test_git.py` & `pytoolbox-14.8.2/tests/test_git.py`

 * *Files identical despite different names*

### Comparing `pytoolbox-14.8.1/tests/test_juju.py` & `pytoolbox-14.8.2/tests/test_juju.py`

 * *Files identical despite different names*

### Comparing `pytoolbox-14.8.1/tests/test_logging.py` & `pytoolbox-14.8.2/tests/test_logging.py`

 * *Files identical despite different names*

### Comparing `pytoolbox-14.8.1/tests/test_module.py` & `pytoolbox-14.8.2/tests/test_module.py`

 * *Files identical despite different names*

### Comparing `pytoolbox-14.8.1/tests/test_private.py` & `pytoolbox-14.8.2/tests/test_private.py`

 * *Files identical despite different names*

### Comparing `pytoolbox-14.8.1/tests/test_regex.py` & `pytoolbox-14.8.2/tests/test_regex.py`

 * *Files identical despite different names*

### Comparing `pytoolbox-14.8.1/tests/test_serialization.py` & `pytoolbox-14.8.2/tests/test_serialization.py`

 * *Files identical despite different names*

### Comparing `pytoolbox-14.8.1/tests/test_signals.py` & `pytoolbox-14.8.2/tests/test_signals.py`

 * *Files identical despite different names*

### Comparing `pytoolbox-14.8.1/tests/test_ssh.py` & `pytoolbox-14.8.2/tests/test_ssh.py`

 * *Files identical despite different names*

### Comparing `pytoolbox-14.8.1/tests/test_states.py` & `pytoolbox-14.8.2/tests/test_states.py`

 * *Files identical despite different names*

### Comparing `pytoolbox-14.8.1/tests/test_string.py` & `pytoolbox-14.8.2/tests/test_string.py`

 * *Files identical despite different names*

### Comparing `pytoolbox-14.8.1/tests/test_subprocess.py` & `pytoolbox-14.8.2/tests/test_subprocess.py`

 * *Files identical despite different names*

### Comparing `pytoolbox-14.8.1/tests/test_unittest.py` & `pytoolbox-14.8.2/tests/test_unittest.py`

 * *Files identical despite different names*

### Comparing `pytoolbox-14.8.1/tests/test_validation.py` & `pytoolbox-14.8.2/tests/test_validation.py`

 * *Files identical despite different names*

