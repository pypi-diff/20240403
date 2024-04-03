# Comparing `tmp/SensiML-2023.2.1.tar.gz` & `tmp/SensiML-2023.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SensiML-2023.2.1.tar", last modified: Thu Sep 28 00:27:35 2023, max compression
+gzip compressed data, was "SensiML-2023.3.0.tar", last modified: Mon Nov  6 23:02:13 2023, max compression
```

## Comparing `SensiML-2023.2.1.tar` & `SensiML-2023.3.0.tar`

### file list

```diff
@@ -1,110 +1,110 @@
-drwxrwxr-x   0 sml-app   (1000) sml-app   (1000)        0 2023-09-28 00:27:35.028533 SensiML-2023.2.1/
--rw-rw-r--   0 sml-app   (1000) sml-app   (1000)     2186 2022-02-08 07:37:16.000000 SensiML-2023.2.1/LICENSE
--rw-rw-r--   0 sml-app   (1000) sml-app   (1000)     1666 2023-09-28 00:27:35.024533 SensiML-2023.2.1/PKG-INFO
--rw-rw-r--   0 sml-app   (1000) sml-app   (1000)     1304 2022-02-03 00:12:15.000000 SensiML-2023.2.1/README.md
-drwxrwxr-x   0 sml-app   (1000) sml-app   (1000)        0 2023-09-28 00:27:34.992532 SensiML-2023.2.1/SensiML.egg-info/
--rw-rw-r--   0 sml-app   (1000) sml-app   (1000)     1666 2023-09-28 00:27:34.000000 SensiML-2023.2.1/SensiML.egg-info/PKG-INFO
--rw-rw-r--   0 sml-app   (1000) sml-app   (1000)     3107 2023-09-28 00:27:34.000000 SensiML-2023.2.1/SensiML.egg-info/SOURCES.txt
--rw-rw-r--   0 sml-app   (1000) sml-app   (1000)        1 2023-09-28 00:27:34.000000 SensiML-2023.2.1/SensiML.egg-info/dependency_links.txt
--rw-rw-r--   0 sml-app   (1000) sml-app   (1000)      157 2023-09-28 00:27:34.000000 SensiML-2023.2.1/SensiML.egg-info/requires.txt
--rw-rw-r--   0 sml-app   (1000) sml-app   (1000)        8 2023-09-28 00:27:34.000000 SensiML-2023.2.1/SensiML.egg-info/top_level.txt
-drwxrwxr-x   0 sml-app   (1000) sml-app   (1000)        0 2023-09-28 00:27:34.996532 SensiML-2023.2.1/sensiml/
--rw-rw-r--   0 sml-app   (1000) sml-app   (1000)      309 2022-09-07 03:55:16.000000 SensiML-2023.2.1/sensiml/__init__.py
-drwxrwxr-x   0 sml-app   (1000) sml-app   (1000)        0 2023-09-28 00:27:34.996532 SensiML-2023.2.1/sensiml/base/
--rw-rw-r--   0 sml-app   (1000) sml-app   (1000)        0 2021-07-02 06:14:18.000000 SensiML-2023.2.1/sensiml/base/__init__.py
--rw-rw-r--   0 sml-app   (1000) sml-app   (1000)     1061 2021-07-02 06:14:18.000000 SensiML-2023.2.1/sensiml/base/exceptions.py
--rw-rw-r--   0 sml-app   (1000) sml-app   (1000)    11356 2023-09-28 00:26:57.000000 SensiML-2023.2.1/sensiml/base/snippets.py
--rw-rw-r--   0 sml-app   (1000) sml-app   (1000)    14417 2023-02-02 21:47:32.000000 SensiML-2023.2.1/sensiml/base/utility.py
--rw-rw-r--   0 sml-app   (1000) sml-app   (1000)    34321 2023-09-28 00:26:57.000000 SensiML-2023.2.1/sensiml/client.py
-drwxrwxr-x   0 sml-app   (1000) sml-app   (1000)        0 2023-09-28 00:27:34.996532 SensiML-2023.2.1/sensiml/connection/
--rw-rw-r--   0 sml-app   (1000) sml-app   (1000)      129 2021-07-02 06:14:18.000000 SensiML-2023.2.1/sensiml/connection/__init__.py
--rw-rw-r--   0 sml-app   (1000) sml-app   (1000)    18409 2023-09-28 00:26:57.000000 SensiML-2023.2.1/sensiml/connection/connection.py
--rw-rw-r--   0 sml-app   (1000) sml-app   (1000)     4730 2021-09-22 23:18:11.000000 SensiML-2023.2.1/sensiml/connection/connection_config.py
--rw-rw-r--   0 sml-app   (1000) sml-app   (1000)      626 2021-07-02 06:14:18.000000 SensiML-2023.2.1/sensiml/connection/errors.py
-drwxrwxr-x   0 sml-app   (1000) sml-app   (1000)        0 2023-09-28 00:27:35.000532 SensiML-2023.2.1/sensiml/data/
--rw-rw-r--   0 sml-app   (1000) sml-app   (1000)        0 2021-07-02 06:14:18.000000 SensiML-2023.2.1/sensiml/data/__init__.py
-drwxrwxr-x   0 sml-app   (1000) sml-app   (1000)        0 2023-09-28 00:27:35.012533 SensiML-2023.2.1/sensiml/datamanager/
--rw-rw-r--   0 sml-app   (1000) sml-app   (1000)      583 2022-05-19 23:26:20.000000 SensiML-2023.2.1/sensiml/datamanager/__init__.py
--rw-rw-r--   0 sml-app   (1000) sml-app   (1000)     6285 2022-08-05 16:07:43.000000 SensiML-2023.2.1/sensiml/datamanager/base.py
--rw-rw-r--   0 sml-app   (1000) sml-app   (1000)    11460 2023-09-28 00:26:57.000000 SensiML-2023.2.1/sensiml/datamanager/capture.py
--rw-rw-r--   0 sml-app   (1000) sml-app   (1000)     3853 2022-02-03 00:12:15.000000 SensiML-2023.2.1/sensiml/datamanager/capture_configuration.py
--rw-rw-r--   0 sml-app   (1000) sml-app   (1000)     3708 2022-02-03 00:12:15.000000 SensiML-2023.2.1/sensiml/datamanager/capture_configurations.py
--rw-rw-r--   0 sml-app   (1000) sml-app   (1000)    11277 2023-09-28 00:26:57.000000 SensiML-2023.2.1/sensiml/datamanager/captures.py
--rw-rw-r--   0 sml-app   (1000) sml-app   (1000)    11830 2022-02-03 00:12:15.000000 SensiML-2023.2.1/sensiml/datamanager/clientplatformdescription.py
--rw-rw-r--   0 sml-app   (1000) sml-app   (1000)     3505 2021-10-29 11:29:06.000000 SensiML-2023.2.1/sensiml/datamanager/clientplatformdescriptions.py
--rw-rw-r--   0 sml-app   (1000) sml-app   (1000)    26763 2023-08-22 07:14:14.000000 SensiML-2023.2.1/sensiml/datamanager/confusion_matrix.py
--rw-rw-r--   0 sml-app   (1000) sml-app   (1000)     6017 2021-11-03 22:39:59.000000 SensiML-2023.2.1/sensiml/datamanager/custom_functions.py
--rw-rw-r--   0 sml-app   (1000) sml-app   (1000)     2089 2021-09-22 23:18:11.000000 SensiML-2023.2.1/sensiml/datamanager/deviceconfig.py
--rw-rw-r--   0 sml-app   (1000) sml-app   (1000)      646 2021-09-22 23:18:11.000000 SensiML-2023.2.1/sensiml/datamanager/errors.py
--rw-rw-r--   0 sml-app   (1000) sml-app   (1000)     6796 2023-02-02 21:47:32.000000 SensiML-2023.2.1/sensiml/datamanager/featurefile.py
--rw-rw-r--   0 sml-app   (1000) sml-app   (1000)     4952 2023-02-02 21:47:32.000000 SensiML-2023.2.1/sensiml/datamanager/featurefiles.py
--rw-rw-r--   0 sml-app   (1000) sml-app   (1000)     2382 2022-03-23 19:36:48.000000 SensiML-2023.2.1/sensiml/datamanager/foundation_model.py
--rw-rw-r--   0 sml-app   (1000) sml-app   (1000)     6281 2021-11-03 22:39:59.000000 SensiML-2023.2.1/sensiml/datamanager/function.py
--rw-rw-r--   0 sml-app   (1000) sml-app   (1000)    16530 2022-08-05 16:07:43.000000 SensiML-2023.2.1/sensiml/datamanager/functions.py
--rw-rw-r--   0 sml-app   (1000) sml-app   (1000)    37980 2023-09-28 00:26:57.000000 SensiML-2023.2.1/sensiml/datamanager/knowledgepack.py
--rw-rw-r--   0 sml-app   (1000) sml-app   (1000)     5024 2022-10-03 21:54:12.000000 SensiML-2023.2.1/sensiml/datamanager/label.py
--rw-rw-r--   0 sml-app   (1000) sml-app   (1000)     5663 2023-09-28 00:26:57.000000 SensiML-2023.2.1/sensiml/datamanager/label_relationship.py
--rw-rw-r--   0 sml-app   (1000) sml-app   (1000)     5519 2022-08-05 16:07:43.000000 SensiML-2023.2.1/sensiml/datamanager/labelvalue.py
--rw-rw-r--   0 sml-app   (1000) sml-app   (1000)     3907 2021-09-22 23:18:11.000000 SensiML-2023.2.1/sensiml/datamanager/library_pack.py
--rw-rw-r--   0 sml-app   (1000) sml-app   (1000)     1179 2022-10-03 21:54:12.000000 SensiML-2023.2.1/sensiml/datamanager/metadata.py
--rw-rw-r--   0 sml-app   (1000) sml-app   (1000)     7280 2023-09-28 00:26:57.000000 SensiML-2023.2.1/sensiml/datamanager/metadata_relationship.py
--rw-rw-r--   0 sml-app   (1000) sml-app   (1000)     2341 2021-09-22 23:18:11.000000 SensiML-2023.2.1/sensiml/datamanager/metadata_value.py
--rw-rw-r--   0 sml-app   (1000) sml-app   (1000)    17363 2023-08-22 07:14:14.000000 SensiML-2023.2.1/sensiml/datamanager/modelresults.py
--rw-rw-r--   0 sml-app   (1000) sml-app   (1000)     2843 2021-07-02 06:14:18.000000 SensiML-2023.2.1/sensiml/datamanager/pipeline.py
--rw-rw-r--   0 sml-app   (1000) sml-app   (1000)    15540 2023-08-22 07:14:14.000000 SensiML-2023.2.1/sensiml/datamanager/project.py
--rw-rw-r--   0 sml-app   (1000) sml-app   (1000)     4089 2022-03-02 07:28:57.000000 SensiML-2023.2.1/sensiml/datamanager/projects.py
--rw-rw-r--   0 sml-app   (1000) sml-app   (1000)     5226 2022-02-15 23:58:11.000000 SensiML-2023.2.1/sensiml/datamanager/queries.py
--rw-rw-r--   0 sml-app   (1000) sml-app   (1000)    19674 2022-02-15 23:58:11.000000 SensiML-2023.2.1/sensiml/datamanager/query.py
--rw-rw-r--   0 sml-app   (1000) sml-app   (1000)    31939 2023-09-28 00:26:57.000000 SensiML-2023.2.1/sensiml/datamanager/sandbox.py
--rw-rw-r--   0 sml-app   (1000) sml-app   (1000)     3615 2022-03-02 07:28:57.000000 SensiML-2023.2.1/sensiml/datamanager/sandboxes.py
--rw-rw-r--   0 sml-app   (1000) sml-app   (1000)     4223 2021-09-22 23:18:11.000000 SensiML-2023.2.1/sensiml/datamanager/segmenter.py
--rw-rw-r--   0 sml-app   (1000) sml-app   (1000)     1041 2022-11-18 15:39:39.000000 SensiML-2023.2.1/sensiml/datamanager/team.py
--rw-rw-r--   0 sml-app   (1000) sml-app   (1000)     7885 2021-07-02 06:14:18.000000 SensiML-2023.2.1/sensiml/datasets.py
-drwxrwxr-x   0 sml-app   (1000) sml-app   (1000)        0 2023-09-28 00:27:35.016533 SensiML-2023.2.1/sensiml/dclproj/
--rw-rw-r--   0 sml-app   (1000) sml-app   (1000)      570 2023-02-28 03:42:07.000000 SensiML-2023.2.1/sensiml/dclproj/__init__.py
--rw-rw-r--   0 sml-app   (1000) sml-app   (1000)    27439 2023-02-28 03:42:07.000000 SensiML-2023.2.1/sensiml/dclproj/confusion_matrix.py
--rw-rw-r--   0 sml-app   (1000) sml-app   (1000)     3901 2022-04-07 18:29:01.000000 SensiML-2023.2.1/sensiml/dclproj/csv_to_dcli.py
--rw-rw-r--   0 sml-app   (1000) sml-app   (1000)    33503 2023-02-28 03:42:07.000000 SensiML-2023.2.1/sensiml/dclproj/datasegments.py
--rw-rw-r--   0 sml-app   (1000) sml-app   (1000)    21333 2023-08-22 07:14:14.000000 SensiML-2023.2.1/sensiml/dclproj/dclproj.py
--rw-rw-r--   0 sml-app   (1000) sml-app   (1000)    12912 2023-09-28 00:26:57.000000 SensiML-2023.2.1/sensiml/dclproj/upload.py
--rw-rw-r--   0 sml-app   (1000) sml-app   (1000)    13281 2023-09-28 00:26:57.000000 SensiML-2023.2.1/sensiml/dclproj/utils.py
--rw-rw-r--   0 sml-app   (1000) sml-app   (1000)     3397 2023-08-22 07:14:14.000000 SensiML-2023.2.1/sensiml/dclproj/vizualization.py
-drwxrwxr-x   0 sml-app   (1000) sml-app   (1000)        0 2023-09-28 00:27:35.016533 SensiML-2023.2.1/sensiml/image/
--rw-rw-r--   0 sml-app   (1000) sml-app   (1000)        0 2021-07-02 06:14:18.000000 SensiML-2023.2.1/sensiml/image/__init__.py
--rw-rw-r--   0 sml-app   (1000) sml-app   (1000)    14012 2021-07-02 06:14:18.000000 SensiML-2023.2.1/sensiml/image/sensiml.png
-drwxrwxr-x   0 sml-app   (1000) sml-app   (1000)        0 2023-09-28 00:27:35.024533 SensiML-2023.2.1/sensiml/method_calls/
--rw-rw-r--   0 sml-app   (1000) sml-app   (1000)     1434 2022-08-05 16:07:43.000000 SensiML-2023.2.1/sensiml/method_calls/__init__.py
--rw-rw-r--   0 sml-app   (1000) sml-app   (1000)      650 2021-07-02 06:14:18.000000 SensiML-2023.2.1/sensiml/method_calls/augmentationcall.py
--rw-rw-r--   0 sml-app   (1000) sml-app   (1000)     3425 2023-08-22 07:14:14.000000 SensiML-2023.2.1/sensiml/method_calls/augmentationcallset.py
--rw-rw-r--   0 sml-app   (1000) sml-app   (1000)      783 2021-07-02 06:14:18.000000 SensiML-2023.2.1/sensiml/method_calls/basemethodcall.py
--rw-rw-r--   0 sml-app   (1000) sml-app   (1000)     1533 2022-08-05 16:07:43.000000 SensiML-2023.2.1/sensiml/method_calls/capturefilecall.py
--rw-rw-r--   0 sml-app   (1000) sml-app   (1000)      294 2021-07-02 06:14:18.000000 SensiML-2023.2.1/sensiml/method_calls/classifiercall.py
--rw-rw-r--   0 sml-app   (1000) sml-app   (1000)     1659 2022-08-05 16:07:43.000000 SensiML-2023.2.1/sensiml/method_calls/datafilecall.py
--rw-rw-r--   0 sml-app   (1000) sml-app   (1000)     2042 2022-08-05 16:07:43.000000 SensiML-2023.2.1/sensiml/method_calls/featurefilecall.py
--rw-rw-r--   0 sml-app   (1000) sml-app   (1000)     2029 2021-09-22 23:18:11.000000 SensiML-2023.2.1/sensiml/method_calls/functioncall.py
--rw-rw-r--   0 sml-app   (1000) sml-app   (1000)     1160 2021-09-22 23:18:11.000000 SensiML-2023.2.1/sensiml/method_calls/functioncalls.py
--rw-rw-r--   0 sml-app   (1000) sml-app   (1000)      756 2021-07-02 06:14:18.000000 SensiML-2023.2.1/sensiml/method_calls/generatorcall.py
--rw-rw-r--   0 sml-app   (1000) sml-app   (1000)     2563 2021-09-22 23:18:11.000000 SensiML-2023.2.1/sensiml/method_calls/generatorcallset.py
--rw-rw-r--   0 sml-app   (1000) sml-app   (1000)      408 2021-07-02 06:14:18.000000 SensiML-2023.2.1/sensiml/method_calls/optimizercall.py
--rw-rw-r--   0 sml-app   (1000) sml-app   (1000)     1142 2021-07-29 17:52:20.000000 SensiML-2023.2.1/sensiml/method_calls/querycall.py
--rw-rw-r--   0 sml-app   (1000) sml-app   (1000)      642 2021-07-02 06:14:18.000000 SensiML-2023.2.1/sensiml/method_calls/selectorcall.py
--rw-rw-r--   0 sml-app   (1000) sml-app   (1000)     4401 2021-09-22 23:18:11.000000 SensiML-2023.2.1/sensiml/method_calls/selectorcallset.py
--rw-rw-r--   0 sml-app   (1000) sml-app   (1000)     4857 2021-09-22 23:18:11.000000 SensiML-2023.2.1/sensiml/method_calls/trainandvalidationcall.py
--rw-rw-r--   0 sml-app   (1000) sml-app   (1000)      463 2021-07-02 06:14:18.000000 SensiML-2023.2.1/sensiml/method_calls/trainingalgorithmcall.py
--rw-rw-r--   0 sml-app   (1000) sml-app   (1000)      429 2021-07-02 06:14:18.000000 SensiML-2023.2.1/sensiml/method_calls/validationmethodcall.py
--rw-rw-r--   0 sml-app   (1000) sml-app   (1000)    39652 2023-09-28 00:26:57.000000 SensiML-2023.2.1/sensiml/model_runner.py
--rw-rw-r--   0 sml-app   (1000) sml-app   (1000)    59498 2023-09-28 00:26:57.000000 SensiML-2023.2.1/sensiml/pipeline.py
-drwxrwxr-x   0 sml-app   (1000) sml-app   (1000)        0 2023-09-28 00:27:35.024533 SensiML-2023.2.1/sensiml/profile/
--rw-rw-r--   0 sml-app   (1000) sml-app   (1000)       91 2021-07-02 06:14:18.000000 SensiML-2023.2.1/sensiml/profile/__init__.py
--rw-rw-r--   0 sml-app   (1000) sml-app   (1000)     6739 2021-07-29 17:52:20.000000 SensiML-2023.2.1/sensiml/profile/profile_data_parser.py
--rw-rw-r--   0 sml-app   (1000) sml-app   (1000)       97 2021-07-02 06:14:18.000000 SensiML-2023.2.1/sensiml/render.py
--rw-rw-r--   0 sml-app   (1000) sml-app   (1000)      147 2023-09-28 00:26:57.000000 SensiML-2023.2.1/sensiml/sml_runner.py
-drwxrwxr-x   0 sml-app   (1000) sml-app   (1000)        0 2023-09-28 00:27:35.024533 SensiML-2023.2.1/sensiml/tensorflow/
--rw-rw-r--   0 sml-app   (1000) sml-app   (1000)        0 2021-07-02 06:14:18.000000 SensiML-2023.2.1/sensiml/tensorflow/__init__.py
--rw-rw-r--   0 sml-app   (1000) sml-app   (1000)     6619 2021-11-29 20:51:38.000000 SensiML-2023.2.1/sensiml/tensorflow/utils.py
-drwxrwxr-x   0 sml-app   (1000) sml-app   (1000)        0 2023-09-28 00:27:35.024533 SensiML-2023.2.1/sensiml/visualize/
--rw-rw-r--   0 sml-app   (1000) sml-app   (1000)       80 2021-07-02 06:14:18.000000 SensiML-2023.2.1/sensiml/visualize/__init__.py
--rw-rw-r--   0 sml-app   (1000) sml-app   (1000)     1170 2021-10-29 11:29:06.000000 SensiML-2023.2.1/sensiml/visualize/knowledgepack_visualize_mixin.py
--rw-rw-r--   0 sml-app   (1000) sml-app   (1000)    14329 2022-02-03 00:12:15.000000 SensiML-2023.2.1/sensiml/visualize/visualize.py
--rw-rw-r--   0 sml-app   (1000) sml-app   (1000)       38 2023-09-28 00:27:35.028533 SensiML-2023.2.1/setup.cfg
--rw-rw-r--   0 sml-app   (1000) sml-app   (1000)     1479 2023-09-28 00:26:57.000000 SensiML-2023.2.1/setup.py
+drwxrwxr-x   0 sml-app   (1000) sml-app   (1000)        0 2023-11-06 23:02:13.129785 SensiML-2023.3.0/
+-rw-rw-r--   0 sml-app   (1000) sml-app   (1000)     2186 2022-02-08 07:37:16.000000 SensiML-2023.3.0/LICENSE
+-rw-rw-r--   0 sml-app   (1000) sml-app   (1000)     1666 2023-11-06 23:02:13.129785 SensiML-2023.3.0/PKG-INFO
+-rw-rw-r--   0 sml-app   (1000) sml-app   (1000)     1304 2022-02-03 00:12:15.000000 SensiML-2023.3.0/README.md
+drwxrwxr-x   0 sml-app   (1000) sml-app   (1000)        0 2023-11-06 23:02:13.093784 SensiML-2023.3.0/SensiML.egg-info/
+-rw-rw-r--   0 sml-app   (1000) sml-app   (1000)     1666 2023-11-06 23:02:13.000000 SensiML-2023.3.0/SensiML.egg-info/PKG-INFO
+-rw-rw-r--   0 sml-app   (1000) sml-app   (1000)     3107 2023-11-06 23:02:13.000000 SensiML-2023.3.0/SensiML.egg-info/SOURCES.txt
+-rw-rw-r--   0 sml-app   (1000) sml-app   (1000)        1 2023-11-06 23:02:13.000000 SensiML-2023.3.0/SensiML.egg-info/dependency_links.txt
+-rw-rw-r--   0 sml-app   (1000) sml-app   (1000)      157 2023-11-06 23:02:13.000000 SensiML-2023.3.0/SensiML.egg-info/requires.txt
+-rw-rw-r--   0 sml-app   (1000) sml-app   (1000)        8 2023-11-06 23:02:13.000000 SensiML-2023.3.0/SensiML.egg-info/top_level.txt
+drwxrwxr-x   0 sml-app   (1000) sml-app   (1000)        0 2023-11-06 23:02:13.093784 SensiML-2023.3.0/sensiml/
+-rw-rw-r--   0 sml-app   (1000) sml-app   (1000)      309 2022-09-07 03:55:16.000000 SensiML-2023.3.0/sensiml/__init__.py
+drwxrwxr-x   0 sml-app   (1000) sml-app   (1000)        0 2023-11-06 23:02:13.097784 SensiML-2023.3.0/sensiml/base/
+-rw-rw-r--   0 sml-app   (1000) sml-app   (1000)        0 2021-07-02 06:14:18.000000 SensiML-2023.3.0/sensiml/base/__init__.py
+-rw-rw-r--   0 sml-app   (1000) sml-app   (1000)     1061 2021-07-02 06:14:18.000000 SensiML-2023.3.0/sensiml/base/exceptions.py
+-rw-rw-r--   0 sml-app   (1000) sml-app   (1000)    11356 2023-09-28 00:26:57.000000 SensiML-2023.3.0/sensiml/base/snippets.py
+-rw-rw-r--   0 sml-app   (1000) sml-app   (1000)    14664 2023-11-06 23:01:54.000000 SensiML-2023.3.0/sensiml/base/utility.py
+-rw-rw-r--   0 sml-app   (1000) sml-app   (1000)    34946 2023-11-06 23:01:54.000000 SensiML-2023.3.0/sensiml/client.py
+drwxrwxr-x   0 sml-app   (1000) sml-app   (1000)        0 2023-11-06 23:02:13.097784 SensiML-2023.3.0/sensiml/connection/
+-rw-rw-r--   0 sml-app   (1000) sml-app   (1000)      129 2021-07-02 06:14:18.000000 SensiML-2023.3.0/sensiml/connection/__init__.py
+-rw-rw-r--   0 sml-app   (1000) sml-app   (1000)    18409 2023-09-28 00:26:57.000000 SensiML-2023.3.0/sensiml/connection/connection.py
+-rw-rw-r--   0 sml-app   (1000) sml-app   (1000)     4730 2021-09-22 23:18:11.000000 SensiML-2023.3.0/sensiml/connection/connection_config.py
+-rw-rw-r--   0 sml-app   (1000) sml-app   (1000)      626 2021-07-02 06:14:18.000000 SensiML-2023.3.0/sensiml/connection/errors.py
+drwxrwxr-x   0 sml-app   (1000) sml-app   (1000)        0 2023-11-06 23:02:13.097784 SensiML-2023.3.0/sensiml/data/
+-rw-rw-r--   0 sml-app   (1000) sml-app   (1000)        0 2021-07-02 06:14:18.000000 SensiML-2023.3.0/sensiml/data/__init__.py
+drwxrwxr-x   0 sml-app   (1000) sml-app   (1000)        0 2023-11-06 23:02:13.113785 SensiML-2023.3.0/sensiml/datamanager/
+-rw-rw-r--   0 sml-app   (1000) sml-app   (1000)      583 2022-05-19 23:26:20.000000 SensiML-2023.3.0/sensiml/datamanager/__init__.py
+-rw-rw-r--   0 sml-app   (1000) sml-app   (1000)     6285 2022-08-05 16:07:43.000000 SensiML-2023.3.0/sensiml/datamanager/base.py
+-rw-rw-r--   0 sml-app   (1000) sml-app   (1000)    11460 2023-09-28 00:26:57.000000 SensiML-2023.3.0/sensiml/datamanager/capture.py
+-rw-rw-r--   0 sml-app   (1000) sml-app   (1000)     3853 2022-02-03 00:12:15.000000 SensiML-2023.3.0/sensiml/datamanager/capture_configuration.py
+-rw-rw-r--   0 sml-app   (1000) sml-app   (1000)     3708 2022-02-03 00:12:15.000000 SensiML-2023.3.0/sensiml/datamanager/capture_configurations.py
+-rw-rw-r--   0 sml-app   (1000) sml-app   (1000)    11277 2023-09-28 00:26:57.000000 SensiML-2023.3.0/sensiml/datamanager/captures.py
+-rw-rw-r--   0 sml-app   (1000) sml-app   (1000)    11830 2022-02-03 00:12:15.000000 SensiML-2023.3.0/sensiml/datamanager/clientplatformdescription.py
+-rw-rw-r--   0 sml-app   (1000) sml-app   (1000)     3505 2021-10-29 11:29:06.000000 SensiML-2023.3.0/sensiml/datamanager/clientplatformdescriptions.py
+-rw-rw-r--   0 sml-app   (1000) sml-app   (1000)    26763 2023-08-22 07:14:14.000000 SensiML-2023.3.0/sensiml/datamanager/confusion_matrix.py
+-rw-rw-r--   0 sml-app   (1000) sml-app   (1000)     6017 2021-11-03 22:39:59.000000 SensiML-2023.3.0/sensiml/datamanager/custom_functions.py
+-rw-rw-r--   0 sml-app   (1000) sml-app   (1000)     2089 2021-09-22 23:18:11.000000 SensiML-2023.3.0/sensiml/datamanager/deviceconfig.py
+-rw-rw-r--   0 sml-app   (1000) sml-app   (1000)      646 2021-09-22 23:18:11.000000 SensiML-2023.3.0/sensiml/datamanager/errors.py
+-rw-rw-r--   0 sml-app   (1000) sml-app   (1000)     6796 2023-02-02 21:47:32.000000 SensiML-2023.3.0/sensiml/datamanager/featurefile.py
+-rw-rw-r--   0 sml-app   (1000) sml-app   (1000)     4952 2023-02-02 21:47:32.000000 SensiML-2023.3.0/sensiml/datamanager/featurefiles.py
+-rw-rw-r--   0 sml-app   (1000) sml-app   (1000)     2382 2022-03-23 19:36:48.000000 SensiML-2023.3.0/sensiml/datamanager/foundation_model.py
+-rw-rw-r--   0 sml-app   (1000) sml-app   (1000)     6281 2021-11-03 22:39:59.000000 SensiML-2023.3.0/sensiml/datamanager/function.py
+-rw-rw-r--   0 sml-app   (1000) sml-app   (1000)    16530 2022-08-05 16:07:43.000000 SensiML-2023.3.0/sensiml/datamanager/functions.py
+-rw-rw-r--   0 sml-app   (1000) sml-app   (1000)    38044 2023-11-06 23:01:54.000000 SensiML-2023.3.0/sensiml/datamanager/knowledgepack.py
+-rw-rw-r--   0 sml-app   (1000) sml-app   (1000)     5024 2022-10-03 21:54:12.000000 SensiML-2023.3.0/sensiml/datamanager/label.py
+-rw-rw-r--   0 sml-app   (1000) sml-app   (1000)     5663 2023-09-28 00:26:57.000000 SensiML-2023.3.0/sensiml/datamanager/label_relationship.py
+-rw-rw-r--   0 sml-app   (1000) sml-app   (1000)     5519 2022-08-05 16:07:43.000000 SensiML-2023.3.0/sensiml/datamanager/labelvalue.py
+-rw-rw-r--   0 sml-app   (1000) sml-app   (1000)     3907 2021-09-22 23:18:11.000000 SensiML-2023.3.0/sensiml/datamanager/library_pack.py
+-rw-rw-r--   0 sml-app   (1000) sml-app   (1000)     1179 2022-10-03 21:54:12.000000 SensiML-2023.3.0/sensiml/datamanager/metadata.py
+-rw-rw-r--   0 sml-app   (1000) sml-app   (1000)     7280 2023-09-28 00:26:57.000000 SensiML-2023.3.0/sensiml/datamanager/metadata_relationship.py
+-rw-rw-r--   0 sml-app   (1000) sml-app   (1000)     2341 2021-09-22 23:18:11.000000 SensiML-2023.3.0/sensiml/datamanager/metadata_value.py
+-rw-rw-r--   0 sml-app   (1000) sml-app   (1000)    17363 2023-08-22 07:14:14.000000 SensiML-2023.3.0/sensiml/datamanager/modelresults.py
+-rw-rw-r--   0 sml-app   (1000) sml-app   (1000)     2843 2021-07-02 06:14:18.000000 SensiML-2023.3.0/sensiml/datamanager/pipeline.py
+-rw-rw-r--   0 sml-app   (1000) sml-app   (1000)    15540 2023-08-22 07:14:14.000000 SensiML-2023.3.0/sensiml/datamanager/project.py
+-rw-rw-r--   0 sml-app   (1000) sml-app   (1000)     4089 2022-03-02 07:28:57.000000 SensiML-2023.3.0/sensiml/datamanager/projects.py
+-rw-rw-r--   0 sml-app   (1000) sml-app   (1000)     5226 2022-02-15 23:58:11.000000 SensiML-2023.3.0/sensiml/datamanager/queries.py
+-rw-rw-r--   0 sml-app   (1000) sml-app   (1000)    19674 2022-02-15 23:58:11.000000 SensiML-2023.3.0/sensiml/datamanager/query.py
+-rw-rw-r--   0 sml-app   (1000) sml-app   (1000)    32008 2023-11-06 23:01:54.000000 SensiML-2023.3.0/sensiml/datamanager/sandbox.py
+-rw-rw-r--   0 sml-app   (1000) sml-app   (1000)     3615 2022-03-02 07:28:57.000000 SensiML-2023.3.0/sensiml/datamanager/sandboxes.py
+-rw-rw-r--   0 sml-app   (1000) sml-app   (1000)     4223 2021-09-22 23:18:11.000000 SensiML-2023.3.0/sensiml/datamanager/segmenter.py
+-rw-rw-r--   0 sml-app   (1000) sml-app   (1000)     1041 2022-11-18 15:39:39.000000 SensiML-2023.3.0/sensiml/datamanager/team.py
+-rw-rw-r--   0 sml-app   (1000) sml-app   (1000)     7885 2021-07-02 06:14:18.000000 SensiML-2023.3.0/sensiml/datasets.py
+drwxrwxr-x   0 sml-app   (1000) sml-app   (1000)        0 2023-11-06 23:02:13.117785 SensiML-2023.3.0/sensiml/dclproj/
+-rw-rw-r--   0 sml-app   (1000) sml-app   (1000)      570 2023-02-28 03:42:07.000000 SensiML-2023.3.0/sensiml/dclproj/__init__.py
+-rw-rw-r--   0 sml-app   (1000) sml-app   (1000)    27439 2023-02-28 03:42:07.000000 SensiML-2023.3.0/sensiml/dclproj/confusion_matrix.py
+-rw-rw-r--   0 sml-app   (1000) sml-app   (1000)     3901 2022-04-07 18:29:01.000000 SensiML-2023.3.0/sensiml/dclproj/csv_to_dcli.py
+-rw-rw-r--   0 sml-app   (1000) sml-app   (1000)    33503 2023-02-28 03:42:07.000000 SensiML-2023.3.0/sensiml/dclproj/datasegments.py
+-rw-rw-r--   0 sml-app   (1000) sml-app   (1000)    21333 2023-08-22 07:14:14.000000 SensiML-2023.3.0/sensiml/dclproj/dclproj.py
+-rw-rw-r--   0 sml-app   (1000) sml-app   (1000)    12912 2023-09-28 00:26:57.000000 SensiML-2023.3.0/sensiml/dclproj/upload.py
+-rw-rw-r--   0 sml-app   (1000) sml-app   (1000)    13281 2023-09-28 00:26:57.000000 SensiML-2023.3.0/sensiml/dclproj/utils.py
+-rw-rw-r--   0 sml-app   (1000) sml-app   (1000)     3397 2023-08-22 07:14:14.000000 SensiML-2023.3.0/sensiml/dclproj/vizualization.py
+drwxrwxr-x   0 sml-app   (1000) sml-app   (1000)        0 2023-11-06 23:02:13.117785 SensiML-2023.3.0/sensiml/image/
+-rw-rw-r--   0 sml-app   (1000) sml-app   (1000)        0 2021-07-02 06:14:18.000000 SensiML-2023.3.0/sensiml/image/__init__.py
+-rw-rw-r--   0 sml-app   (1000) sml-app   (1000)    14012 2021-07-02 06:14:18.000000 SensiML-2023.3.0/sensiml/image/sensiml.png
+drwxrwxr-x   0 sml-app   (1000) sml-app   (1000)        0 2023-11-06 23:02:13.125785 SensiML-2023.3.0/sensiml/method_calls/
+-rw-rw-r--   0 sml-app   (1000) sml-app   (1000)     1434 2022-08-05 16:07:43.000000 SensiML-2023.3.0/sensiml/method_calls/__init__.py
+-rw-rw-r--   0 sml-app   (1000) sml-app   (1000)      650 2021-07-02 06:14:18.000000 SensiML-2023.3.0/sensiml/method_calls/augmentationcall.py
+-rw-rw-r--   0 sml-app   (1000) sml-app   (1000)     3425 2023-08-22 07:14:14.000000 SensiML-2023.3.0/sensiml/method_calls/augmentationcallset.py
+-rw-rw-r--   0 sml-app   (1000) sml-app   (1000)      783 2021-07-02 06:14:18.000000 SensiML-2023.3.0/sensiml/method_calls/basemethodcall.py
+-rw-rw-r--   0 sml-app   (1000) sml-app   (1000)     1533 2022-08-05 16:07:43.000000 SensiML-2023.3.0/sensiml/method_calls/capturefilecall.py
+-rw-rw-r--   0 sml-app   (1000) sml-app   (1000)      294 2021-07-02 06:14:18.000000 SensiML-2023.3.0/sensiml/method_calls/classifiercall.py
+-rw-rw-r--   0 sml-app   (1000) sml-app   (1000)     1659 2022-08-05 16:07:43.000000 SensiML-2023.3.0/sensiml/method_calls/datafilecall.py
+-rw-rw-r--   0 sml-app   (1000) sml-app   (1000)     2042 2022-08-05 16:07:43.000000 SensiML-2023.3.0/sensiml/method_calls/featurefilecall.py
+-rw-rw-r--   0 sml-app   (1000) sml-app   (1000)     2029 2021-09-22 23:18:11.000000 SensiML-2023.3.0/sensiml/method_calls/functioncall.py
+-rw-rw-r--   0 sml-app   (1000) sml-app   (1000)     1160 2021-09-22 23:18:11.000000 SensiML-2023.3.0/sensiml/method_calls/functioncalls.py
+-rw-rw-r--   0 sml-app   (1000) sml-app   (1000)      756 2021-07-02 06:14:18.000000 SensiML-2023.3.0/sensiml/method_calls/generatorcall.py
+-rw-rw-r--   0 sml-app   (1000) sml-app   (1000)     2563 2021-09-22 23:18:11.000000 SensiML-2023.3.0/sensiml/method_calls/generatorcallset.py
+-rw-rw-r--   0 sml-app   (1000) sml-app   (1000)      408 2021-07-02 06:14:18.000000 SensiML-2023.3.0/sensiml/method_calls/optimizercall.py
+-rw-rw-r--   0 sml-app   (1000) sml-app   (1000)     1142 2021-07-29 17:52:20.000000 SensiML-2023.3.0/sensiml/method_calls/querycall.py
+-rw-rw-r--   0 sml-app   (1000) sml-app   (1000)      642 2021-07-02 06:14:18.000000 SensiML-2023.3.0/sensiml/method_calls/selectorcall.py
+-rw-rw-r--   0 sml-app   (1000) sml-app   (1000)     4401 2021-09-22 23:18:11.000000 SensiML-2023.3.0/sensiml/method_calls/selectorcallset.py
+-rw-rw-r--   0 sml-app   (1000) sml-app   (1000)     4857 2021-09-22 23:18:11.000000 SensiML-2023.3.0/sensiml/method_calls/trainandvalidationcall.py
+-rw-rw-r--   0 sml-app   (1000) sml-app   (1000)      463 2021-07-02 06:14:18.000000 SensiML-2023.3.0/sensiml/method_calls/trainingalgorithmcall.py
+-rw-rw-r--   0 sml-app   (1000) sml-app   (1000)      429 2021-07-02 06:14:18.000000 SensiML-2023.3.0/sensiml/method_calls/validationmethodcall.py
+-rw-rw-r--   0 sml-app   (1000) sml-app   (1000)    39569 2023-11-06 23:01:54.000000 SensiML-2023.3.0/sensiml/model_runner.py
+-rw-rw-r--   0 sml-app   (1000) sml-app   (1000)    59619 2023-11-06 23:01:54.000000 SensiML-2023.3.0/sensiml/pipeline.py
+drwxrwxr-x   0 sml-app   (1000) sml-app   (1000)        0 2023-11-06 23:02:13.125785 SensiML-2023.3.0/sensiml/profile/
+-rw-rw-r--   0 sml-app   (1000) sml-app   (1000)       91 2021-07-02 06:14:18.000000 SensiML-2023.3.0/sensiml/profile/__init__.py
+-rw-rw-r--   0 sml-app   (1000) sml-app   (1000)     6739 2021-07-29 17:52:20.000000 SensiML-2023.3.0/sensiml/profile/profile_data_parser.py
+-rw-rw-r--   0 sml-app   (1000) sml-app   (1000)       97 2021-07-02 06:14:18.000000 SensiML-2023.3.0/sensiml/render.py
+-rw-rw-r--   0 sml-app   (1000) sml-app   (1000)      147 2023-09-28 00:26:57.000000 SensiML-2023.3.0/sensiml/sml_runner.py
+drwxrwxr-x   0 sml-app   (1000) sml-app   (1000)        0 2023-11-06 23:02:13.125785 SensiML-2023.3.0/sensiml/tensorflow/
+-rw-rw-r--   0 sml-app   (1000) sml-app   (1000)        0 2021-07-02 06:14:18.000000 SensiML-2023.3.0/sensiml/tensorflow/__init__.py
+-rw-rw-r--   0 sml-app   (1000) sml-app   (1000)     6619 2021-11-29 20:51:38.000000 SensiML-2023.3.0/sensiml/tensorflow/utils.py
+drwxrwxr-x   0 sml-app   (1000) sml-app   (1000)        0 2023-11-06 23:02:13.129785 SensiML-2023.3.0/sensiml/visualize/
+-rw-rw-r--   0 sml-app   (1000) sml-app   (1000)       80 2021-07-02 06:14:18.000000 SensiML-2023.3.0/sensiml/visualize/__init__.py
+-rw-rw-r--   0 sml-app   (1000) sml-app   (1000)     1170 2021-10-29 11:29:06.000000 SensiML-2023.3.0/sensiml/visualize/knowledgepack_visualize_mixin.py
+-rw-rw-r--   0 sml-app   (1000) sml-app   (1000)    14329 2022-02-03 00:12:15.000000 SensiML-2023.3.0/sensiml/visualize/visualize.py
+-rw-rw-r--   0 sml-app   (1000) sml-app   (1000)       38 2023-11-06 23:02:13.129785 SensiML-2023.3.0/setup.cfg
+-rw-rw-r--   0 sml-app   (1000) sml-app   (1000)     1479 2023-11-06 23:01:54.000000 SensiML-2023.3.0/setup.py
```

### Comparing `SensiML-2023.2.1/LICENSE` & `SensiML-2023.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `SensiML-2023.2.1/PKG-INFO` & `SensiML-2023.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SensiML
-Version: 2023.2.1
+Version: 2023.3.0
 Summary: SensiML Python SDK
 Home-page: UNKNOWN
 Author: SensiML
 Author-email: support@sensiml.com
 License: Proprietary
 Platform: UNKNOWN
 Classifier: Operating System :: OS Independent
```

### Comparing `SensiML-2023.2.1/README.md` & `SensiML-2023.3.0/README.md`

 * *Files identical despite different names*

### Comparing `SensiML-2023.2.1/SensiML.egg-info/PKG-INFO` & `SensiML-2023.3.0/SensiML.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SensiML
-Version: 2023.2.1
+Version: 2023.3.0
 Summary: SensiML Python SDK
 Home-page: UNKNOWN
 Author: SensiML
 Author-email: support@sensiml.com
 License: Proprietary
 Platform: UNKNOWN
 Classifier: Operating System :: OS Independent
```

### Comparing `SensiML-2023.2.1/SensiML.egg-info/SOURCES.txt` & `SensiML-2023.3.0/SensiML.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `SensiML-2023.2.1/sensiml/base/exceptions.py` & `SensiML-2023.3.0/sensiml/base/exceptions.py`

 * *Files identical despite different names*

### Comparing `SensiML-2023.2.1/sensiml/base/snippets.py` & `SensiML-2023.3.0/sensiml/base/snippets.py`

 * *Files identical despite different names*

### Comparing `SensiML-2023.2.1/sensiml/base/utility.py` & `SensiML-2023.3.0/sensiml/base/utility.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,14 @@
 from pandas import DataFrame
 from six.moves import input
 
 logger = logging.getLogger(__name__)
 
 
 def prompt_for_overwrite(file_that_exists):
-
     acceptable = {"yes": True, "y": True, "n": False, "no": False}
 
     prompts = 0
     while prompts < 3:
         print("{0} Exists. Do you wish to overwrite?".format(file_that_exists))
         answer = input().lower()
         if answer in acceptable.keys():
@@ -122,31 +121,35 @@
             else:
                 logger.warning("{error}: {message}".format(**error))
 
     # If there is a status, the pipeline is Pending, Not Running, Failed, or in the Queue
     status = response_data.get("status", "SUCCESS")
     if status in ["PENDING", "STARTED", "SENT"]:
         if not silent:
-            print(response_data.get("message", None), end="")
+            print(response_data.get("message", None))
+            print(response_data.get("detail", None))
         return None, response_data.get("message", None)
-    elif status in ["FAILURE", "REVOKED", None]:
+    elif status in ["FAILURE", "REVOKED"]:
         print(response_data.get("message", None))
+        print(response_data.get("detail", None))
+        return response_data, None
+    elif status in [None]:
         return response_data, None
 
     return parse_results(response_data, **kwargs)
 
 
 def wait_for_pipeline_result(
     requester,
     lock=True,
     silent=True,
     wait_time=15,
     skip_printing=4,
     renderer=None,
-    **kwargs
+    **kwargs,
 ):
     count = 0
     start = time.time()
 
     results = requester.retrieve(silent=silent, **kwargs)
     if results[0] is not None:
         lock = False
@@ -163,18 +166,19 @@
                 print(" ", end="")
             else:
                 print(".", end="")
             count += 1
         else:
             lock = False
 
-    execution_time = time.time() - start
-    msg = "\n\nResults Retrieved... Execution Time: {0} min. {1} sec.".format(
-        int(execution_time / 60), int(execution_time % 60)
-    )
+    if isinstance(results[0], dict) and results[0].get("status") is None:
+        msg = "No results stored"
+    else:
+        execution_time = time.time() - start
+        msg = f"\n\nResults Retrieved. Wall Time: {int(execution_time / 60)} min. {int(execution_time % 60)} sec."
 
     if renderer:
         renderer.render(msg)
 
     print(msg)
 
     return results
@@ -276,15 +280,15 @@
         print(
             format_budget.format(
                 "Budgets ("
                 + device_config["target_platform"]
                 + " "
                 + device_config["platform_version"]
                 + ")",
-                **full_budget
+                **full_budget,
             )
         )
     else:
         print("There is no budget defined")
 
     if cost_dict.get("neurons", None):
         print("\n\nPattern Matching Engine Costs")
@@ -312,15 +316,15 @@
                     " - {} ({})".format(step["name"], step["type"]), *costs
                 )
             )
         elif step["type"] == "generatorset":
             print(
                 step_format.format(
                     " - {} ({})".format(step["name"], step["type"]),
-                    *["" for cost in cost_columns]
+                    *["" for cost in cost_columns],
                 )
             )
             if step.get("per_generator_costs", None):
                 for feature_generator in step["per_generator_costs"].keys():
                     print(
                         step_format_sub.format(
                             "",
@@ -333,15 +337,15 @@
                             *[
                                 val_or_string(
                                     step["per_generator_costs"][feature_generator],
                                     cost,
                                     na_string,
                                 )
                                 for cost in cost_columns
-                            ]
+                            ],
                         )
                     )
     horizontal_line()
 
     format_fe_totals = "{:>45}" + "{:>17}" * number_of_costs
     print(format_fe_totals.format("Feature Extraction Subtotals:", *fe_subtotals))
 
@@ -362,15 +366,15 @@
         cost: sum_or_string(cost_dict_minus_sensors, cost, na_string)
         for cost in cost_columns
     }
     format_totals = "{:>45}" + "{:>17}" * number_of_costs
     print(
         format_totals.format(
             "Totals Excluding Sensor Costs:",
-            *[totals_minus_sensors[cost] for cost in cost_columns]
+            *[totals_minus_sensors[cost] for cost in cost_columns],
         )
     )
 
     if cost_dict.get("sensors", None):
         print("\n\nSensor Costs")
         horizontal_line()
         sensor_costs = populate_cost_keys(cost_columns, cost_dict["sensors"], na_string)
```

### Comparing `SensiML-2023.2.1/sensiml/client.py` & `SensiML-2023.3.0/sensiml/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,30 +30,34 @@
     ClientPlatformDescriptions,
     Functions,
     Projects,
     SegmenterSet,
     Team,
 )
 from sensiml.datamanager.captures import CaptureExistsError
-from sensiml.datamanager.knowledgepack import delete_knowledgepack, get_knowledgepack
+from sensiml.datamanager.knowledgepack import (
+    KnowledgePack,
+    delete_knowledgepack,
+    get_knowledgepack,
+)
 from sensiml.datasets import DataSets
 from sensiml.dclproj.upload import upload_project, upload_project_dcli
 
 # from sensiml.base.exceptions import *
 from sensiml.pipeline import Pipeline
 
 config_dir = user_config_dir(__name__.split(".")[0], False)
 
 SERVER_URL = "https://sensiml.cloud/"
 
 AUTH2_PRIMARY = True
 
 logger = logging.getLogger("SensiML")
 
-__version__ = "2023.2.1"
+__version__ = "2023.3.0"
 
 
 def project_set(func):
     def wrapper(*args, **kwargs):
         self = args[0]
         if self._project is None:
             print("Project must be set.")
@@ -64,15 +68,14 @@
     return wrapper
 
 
 def print_list(func):
     """This is a wrapper for printing out lists of objects stored in SensiML Cloud"""
 
     def wrapper(*args, **kwargs):
-
         result = func(*args, **kwargs)
 
         if len(result.keys()) == 0 and kwargs.get("silent", False) == False:
             print(
                 "No {} stored on SensiML Cloud for this project.".format(
                     " ".join(func.__name__.split("_")[1:])
                 )
@@ -126,15 +129,14 @@
         path="connect.cfg",
         use_jedi=False,
         insecure=False,
         skip_validate=False,
         verbose_connection=False,
         **kwargs,
     ):
-
         self._project = None
         self._pipeline = None
         auth_url = server + "oauth/"
 
         self._connection = Connection(
             server=server,
             auth_url=auth_url,
@@ -204,15 +206,14 @@
         """Logs out of the current connection."""
         if name is None:
             name = self._connection.server_name
 
         Connection.logout(name)
 
     def get_url(self, url):
-
         response = self._connection.request("get", url)
         print(response.json())
         return response
 
     def account_info(self):
         """Get information about your account Usage"""
 
@@ -457,20 +458,20 @@
     def _download_captures(
         self,
         filenames: List[str],
         outdir: Optional[str] = None,
         expires_in: int = 100,
         verbose=True,
     ):
-
         capture_response = self.project.captures.get_capture_urls_by_name(
             filenames, expires_in=expires_in
         )
 
         for capture in capture_response:
+            print(f"capture: {capture['name']}, url: {capture['url']}")
             url = capture["url"]
 
             if capture.get("local"):
                 response = self._connection.request("get", url)
             else:
                 response = requests.get(url)
 
@@ -661,14 +662,32 @@
     @pipeline.setter
     def pipeline(self, name):
         if self._project is None:
             raise Exception("Project must be set before a pipeline can be created")
 
         self._pipeline = Pipeline(self, name=name)
 
+    def import_knowledgepack(self, name: str, path: str):
+        """import a model from a json file
+
+        Args:
+            path (str): path to json containing an exported model
+        """
+        if self._project is None:
+            raise Exception("Project must be set to perform this action.")
+
+        model_json = json.load(open(path, "r"))
+        kp = KnowledgePack(self._connection, self.project.uuid)
+        kp.initialize_from_dict(model_json)
+        kp._name = name
+
+        kp.create()
+
+        return kp
+
     def create_query(
         self,
         name: str,
         columns: list = [],
         metadata_columns: list = [],
         metadata_filter: str = "",
         segmenter=None,
```

### Comparing `SensiML-2023.2.1/sensiml/connection/connection.py` & `SensiML-2023.3.0/sensiml/connection/connection.py`

 * *Files identical despite different names*

### Comparing `SensiML-2023.2.1/sensiml/connection/connection_config.py` & `SensiML-2023.3.0/sensiml/connection/connection_config.py`

 * *Files identical despite different names*

### Comparing `SensiML-2023.2.1/sensiml/connection/errors.py` & `SensiML-2023.3.0/sensiml/connection/errors.py`

 * *Files identical despite different names*

### Comparing `SensiML-2023.2.1/sensiml/datamanager/__init__.py` & `SensiML-2023.3.0/sensiml/datamanager/__init__.py`

 * *Files identical despite different names*

### Comparing `SensiML-2023.2.1/sensiml/datamanager/base.py` & `SensiML-2023.3.0/sensiml/datamanager/base.py`

 * *Files identical despite different names*

### Comparing `SensiML-2023.2.1/sensiml/datamanager/capture.py` & `SensiML-2023.3.0/sensiml/datamanager/capture.py`

 * *Files identical despite different names*

### Comparing `SensiML-2023.2.1/sensiml/datamanager/capture_configuration.py` & `SensiML-2023.3.0/sensiml/datamanager/capture_configuration.py`

 * *Files identical despite different names*

### Comparing `SensiML-2023.2.1/sensiml/datamanager/capture_configurations.py` & `SensiML-2023.3.0/sensiml/datamanager/capture_configurations.py`

 * *Files identical despite different names*

### Comparing `SensiML-2023.2.1/sensiml/datamanager/captures.py` & `SensiML-2023.3.0/sensiml/datamanager/captures.py`

 * *Files identical despite different names*

### Comparing `SensiML-2023.2.1/sensiml/datamanager/clientplatformdescription.py` & `SensiML-2023.3.0/sensiml/datamanager/clientplatformdescription.py`

 * *Files identical despite different names*

### Comparing `SensiML-2023.2.1/sensiml/datamanager/clientplatformdescriptions.py` & `SensiML-2023.3.0/sensiml/datamanager/clientplatformdescriptions.py`

 * *Files identical despite different names*

### Comparing `SensiML-2023.2.1/sensiml/datamanager/confusion_matrix.py` & `SensiML-2023.3.0/sensiml/datamanager/confusion_matrix.py`

 * *Files identical despite different names*

### Comparing `SensiML-2023.2.1/sensiml/datamanager/custom_functions.py` & `SensiML-2023.3.0/sensiml/datamanager/custom_functions.py`

 * *Files identical despite different names*

### Comparing `SensiML-2023.2.1/sensiml/datamanager/deviceconfig.py` & `SensiML-2023.3.0/sensiml/datamanager/deviceconfig.py`

 * *Files identical despite different names*

### Comparing `SensiML-2023.2.1/sensiml/datamanager/errors.py` & `SensiML-2023.3.0/sensiml/datamanager/errors.py`

 * *Files identical despite different names*

### Comparing `SensiML-2023.2.1/sensiml/datamanager/featurefile.py` & `SensiML-2023.3.0/sensiml/datamanager/featurefile.py`

 * *Files identical despite different names*

### Comparing `SensiML-2023.2.1/sensiml/datamanager/featurefiles.py` & `SensiML-2023.3.0/sensiml/datamanager/featurefiles.py`

 * *Files identical despite different names*

### Comparing `SensiML-2023.2.1/sensiml/datamanager/foundation_model.py` & `SensiML-2023.3.0/sensiml/datamanager/foundation_model.py`

 * *Files identical despite different names*

### Comparing `SensiML-2023.2.1/sensiml/datamanager/function.py` & `SensiML-2023.3.0/sensiml/datamanager/function.py`

 * *Files identical despite different names*

### Comparing `SensiML-2023.2.1/sensiml/datamanager/functions.py` & `SensiML-2023.3.0/sensiml/datamanager/functions.py`

 * *Files identical despite different names*

### Comparing `SensiML-2023.2.1/sensiml/datamanager/knowledgepack.py` & `SensiML-2023.3.0/sensiml/datamanager/knowledgepack.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,15 +24,14 @@
 from sensiml.method_calls.functioncall import FunctionCall
 from sensiml.visualize.knowledgepack_visualize_mixin import VisualizeMixin
 
 logger = logging.getLogger(__name__)
 
 
 def render_confusion_matrix(cm):
-
     GT_txt = "GroundTruth_Total"
     keys = [k for k, v in cm.items()]
     gt = [cm[k][GT_txt] for k in keys]
     df = pd.DataFrame.from_dict(
         {k: [cm[k][_] for _ in keys] for k in keys}, orient="index"
     )
     df.columns = keys
@@ -342,17 +341,15 @@
             segmenter (bool or FunctionCall): to suppress or override the segmentation algorithm in the original
               pipeline, set this to False or a function call of type 'segmenter' (defaults to True)
             lock (bool, True): If True, waits for the result to return before releasing the ipython cell.
 
         Returns:
             (dict): dictionary of results and summary statistics from the executed pipeline and recognition
         """
-        url = "project/{0}/sandbox/{1}/knowledgepack/{2}/recognize_signal/".format(
-            self._project_uuid, self._sandbox_uuid, self.uuid
-        )
+        url = f"project/{self._project_uuid}/sandbox/{self._project_uuid}/knowledgepack/{self.uuid}/recognize_signal/"
 
         if capture:
             data_for_recognition = {"capture": capture}
         elif datafile:
             if datafile[-4:] != ".csv":
                 datafile = "{}.csv".format(datafile)
             data_for_recognition = {"datafile": datafile}
@@ -514,15 +511,18 @@
             ]
 
             return df_result
 
         summary = {}
         for key in response_data:
             if key not in ["results"]:
-                summary[key] = DataFrame(response_data[key])
+                try:
+                    summary[key] = DataFrame(response_data[key])
+                except:
+                    summary[key] = response_data[key]
 
         # Check for a unicode string which can be returned sometimes
         if isinstance(response_data["results"], str):
             return fix_index(DataFrame(json.loads(response_data["results"]))), summary
 
         # Check for the results vector and parse appropriately
         if isinstance(response_data["results"], dict) and response_data["results"].get(
@@ -884,15 +884,14 @@
             err_msg = response_data.body
             print(err_msg)
             if renderer:
                 renderer.render(err_msg)
             return err_msg, False
 
     def get_featurefile(self):
-
         if self._feature_file_cache is not None:
             return self._feature_file_cache
 
         class DummyProject:
             def __init__(self, uuid):
                 self.uuid = uuid
```

### Comparing `SensiML-2023.2.1/sensiml/datamanager/label.py` & `SensiML-2023.3.0/sensiml/datamanager/label.py`

 * *Files identical despite different names*

### Comparing `SensiML-2023.2.1/sensiml/datamanager/label_relationship.py` & `SensiML-2023.3.0/sensiml/datamanager/label_relationship.py`

 * *Files identical despite different names*

### Comparing `SensiML-2023.2.1/sensiml/datamanager/labelvalue.py` & `SensiML-2023.3.0/sensiml/datamanager/labelvalue.py`

 * *Files identical despite different names*

### Comparing `SensiML-2023.2.1/sensiml/datamanager/library_pack.py` & `SensiML-2023.3.0/sensiml/datamanager/library_pack.py`

 * *Files identical despite different names*

### Comparing `SensiML-2023.2.1/sensiml/datamanager/metadata.py` & `SensiML-2023.3.0/sensiml/datamanager/metadata.py`

 * *Files identical despite different names*

### Comparing `SensiML-2023.2.1/sensiml/datamanager/metadata_relationship.py` & `SensiML-2023.3.0/sensiml/datamanager/metadata_relationship.py`

 * *Files identical despite different names*

### Comparing `SensiML-2023.2.1/sensiml/datamanager/metadata_value.py` & `SensiML-2023.3.0/sensiml/datamanager/metadata_value.py`

 * *Files identical despite different names*

### Comparing `SensiML-2023.2.1/sensiml/datamanager/modelresults.py` & `SensiML-2023.3.0/sensiml/datamanager/modelresults.py`

 * *Files identical despite different names*

### Comparing `SensiML-2023.2.1/sensiml/datamanager/pipeline.py` & `SensiML-2023.3.0/sensiml/datamanager/pipeline.py`

 * *Files identical despite different names*

### Comparing `SensiML-2023.2.1/sensiml/datamanager/project.py` & `SensiML-2023.3.0/sensiml/datamanager/project.py`

 * *Files identical despite different names*

### Comparing `SensiML-2023.2.1/sensiml/datamanager/projects.py` & `SensiML-2023.3.0/sensiml/datamanager/projects.py`

 * *Files identical despite different names*

### Comparing `SensiML-2023.2.1/sensiml/datamanager/queries.py` & `SensiML-2023.3.0/sensiml/datamanager/queries.py`

 * *Files identical despite different names*

### Comparing `SensiML-2023.2.1/sensiml/datamanager/query.py` & `SensiML-2023.3.0/sensiml/datamanager/query.py`

 * *Files identical despite different names*

### Comparing `SensiML-2023.2.1/sensiml/datamanager/sandbox.py` & `SensiML-2023.3.0/sensiml/datamanager/sandbox.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from __future__ import print_function
 
 import datetime
 import inspect
 import json
 import os
+import pprint
 import sys
 from copy import deepcopy
 from logging import debug
 from numbers import Number
 
 import pandas as pd
 from pandas import DataFrame
@@ -417,14 +418,15 @@
         if err is False:
             self.uuid = response_data["uuid"]
             self._init_device_config(response_data)
             self._dirty = False
 
     def update(self):
         """Calls the REST API to update the object on the server."""
+
         self._pipeline._check_integrity()
         if self._check_sandbox_inserted():
             url = "project/{0}/sandbox/{1}/".format(self._project.uuid, self.uuid)
             sandbox_info = {
                 "name": self.name,
                 "pipeline": self.pipeline.to_list(),
                 "cache_enabled": self.cache,
@@ -473,17 +475,17 @@
         response = self._connection.request("get", url)
         response_data, err = utility.check_server_response(response)
         if err is False:
             return pd.DataFrame(response_data)
 
     def _handle_result(self, data, pipeline_step=-1):
         """Decides what type of results have been returned and creates a DataFrame or stores model results accordingly."""
-        if data.get("status"):
-            print(data.get("status"))
-            return None, None
+
+        if data.get("status") not in ["SUCCESS"]:
+            return data, None
 
         execution_type = data.get("execution_type")
 
         if data.get("number_of_pages", 0) > 1:
             print(
                 "\nRetrieving page {0} of {1}.".format(
                     data.get("page_index", 1), data["number_of_pages"]
@@ -491,20 +493,23 @@
             )
             if data["number_of_pages"] > 1:
                 print(
                     "To get more pages, use: \n"
                     + "next_results, next_stats = client.pipeline.get_results(page_index=<desired page number>)."
                 )
 
-        summary = pd.DataFrame(data.get("summary", [])).fillna("")
-        extra = pd.DataFrame(data.get("extra", []))
-        results = data.get("results", [])
+        summary = {}
+        for key in ["execution_summary", "feature_table", "fitness_summary"]:
+            if data.get(key):
+                summary[key] = pd.DataFrame(data.get(key)).fillna("")
 
-        self._execution_summary = summary
-        self._features = extra
+        self._execution_summary = summary.get("execution_summary")
+        self._features = summary.get("feature_table")
+
+        results = data.get("results", [])
 
         if (
             self.pipeline._get_pipeline_step_value(pipeline_step, key="type") == "tvo"
             and execution_type == "pipeline"
         ) or execution_type == "auto":
             if isinstance(results, list):
                 data = []
@@ -521,18 +526,15 @@
 
         else:
             if isinstance(results, list):
                 data = map(lambda x: DataFrame(x), results)
             else:
                 data = DataFrame(results)
 
-        if execution_type == "auto" and "fitness" in extra.columns:
-            return data, {"execution_summary": summary, "fitness_summary": extra}
-        else:
-            return data, {"execution_summary": summary, "features": extra}
+        return data, summary
 
     def intermediate_data(self, pipeline_step, page_index=0):
         """Retrieves intermediate pipeline step data from a previously executed pipeline.
 
         Args:
             pipeline_step (int): The pipeline step to retrieve from and executed pipeline.
             page_index (int): the index to pull form the cache
@@ -543,20 +545,19 @@
         """
         url = "project/{0}/sandbox/{1}/data/".format(self._project.uuid, self.uuid)
         payload = {"pipeline_step": pipeline_step, "page_index": page_index}
         response = self._connection.request("get", url, params=payload)
 
         data, err = utility.check_server_response(response)
         if err is False:
-            response_data = data
-            data, summary = self._handle_result(
-                response_data, pipeline_step=pipeline_step
-            )
+            results = data.pop("results")
+
+            return results, data
 
-            return data, summary
+        return response
 
     def get_metrics_set(self, data):
         """retrieves metrics set from server
 
         Args:
             data (dict): dictionary containing
                         - 'y_true' and 'y_pred' keys
@@ -664,38 +665,47 @@
 
         return self.async_submit(data)
 
     def retrieve_autosegment(self):
         result = self.retrieve()
         return result
 
-    def retrieve(self, silent=False, page_index=0, **kwargs):
+    def retrieve(
+        self,
+        silent: bool = False,
+        page_index: int = 0,
+        status_only: bool = False,
+        **kwargs
+    ):
         """Gets the result of a prior asynchronous execution of the sandbox.
 
+        silent(bool): silence all messages
+        page_index(int): The page of data to retrieve
+        status_only(bool): Return only the status message, don't retrieve any data
+
         Returns:
             (DataFrame or ModelResultSet): result of executed pipeline, specified by the sandbox
             (dict): execution summary including execution time and whether cache was used for each
             step; also contains a feature cost table if applicable
         """
-        if self._dirty:
-            self.update()
 
         url = "project/{0}/sandbox-async/{1}/?{2}".format(
-            self._project.uuid, self.uuid, urlencode({"page_index": page_index})
+            self._project.uuid,
+            self.uuid,
+            urlencode({"page_index": page_index, "status_only": status_only}),
         )
         response = self._connection.request("get", url)
 
         data, err = utility.check_server_response(response)
         if err is False:
             response_data = data or {}
             return utility.check_pipeline_status(
                 response_data, self._handle_result, silent=silent
             )
 
-        print(response.json())
         return response
 
     def kill_pipeline(self):
         url = "project/{0}/sandbox-async/{1}/".format(self._project.uuid, self.uuid)
         response = self._connection.request("delete", url)
         response_data, err = utility.check_server_response(response)
         if err is False:
```

### Comparing `SensiML-2023.2.1/sensiml/datamanager/sandboxes.py` & `SensiML-2023.3.0/sensiml/datamanager/sandboxes.py`

 * *Files identical despite different names*

### Comparing `SensiML-2023.2.1/sensiml/datamanager/segmenter.py` & `SensiML-2023.3.0/sensiml/datamanager/segmenter.py`

 * *Files identical despite different names*

### Comparing `SensiML-2023.2.1/sensiml/datamanager/team.py` & `SensiML-2023.3.0/sensiml/datamanager/team.py`

 * *Files identical despite different names*

### Comparing `SensiML-2023.2.1/sensiml/datasets.py` & `SensiML-2023.3.0/sensiml/datasets.py`

 * *Files identical despite different names*

### Comparing `SensiML-2023.2.1/sensiml/dclproj/__init__.py` & `SensiML-2023.3.0/sensiml/dclproj/__init__.py`

 * *Files identical despite different names*

### Comparing `SensiML-2023.2.1/sensiml/dclproj/confusion_matrix.py` & `SensiML-2023.3.0/sensiml/dclproj/confusion_matrix.py`

 * *Files identical despite different names*

### Comparing `SensiML-2023.2.1/sensiml/dclproj/csv_to_dcli.py` & `SensiML-2023.3.0/sensiml/dclproj/csv_to_dcli.py`

 * *Files identical despite different names*

### Comparing `SensiML-2023.2.1/sensiml/dclproj/datasegments.py` & `SensiML-2023.3.0/sensiml/dclproj/datasegments.py`

 * *Files identical despite different names*

### Comparing `SensiML-2023.2.1/sensiml/dclproj/dclproj.py` & `SensiML-2023.3.0/sensiml/dclproj/dclproj.py`

 * *Files identical despite different names*

### Comparing `SensiML-2023.2.1/sensiml/dclproj/upload.py` & `SensiML-2023.3.0/sensiml/dclproj/upload.py`

 * *Files identical despite different names*

### Comparing `SensiML-2023.2.1/sensiml/dclproj/utils.py` & `SensiML-2023.3.0/sensiml/dclproj/utils.py`

 * *Files identical despite different names*

### Comparing `SensiML-2023.2.1/sensiml/dclproj/vizualization.py` & `SensiML-2023.3.0/sensiml/dclproj/vizualization.py`

 * *Files identical despite different names*

### Comparing `SensiML-2023.2.1/sensiml/image/sensiml.png` & `SensiML-2023.3.0/sensiml/image/sensiml.png`

 * *Files identical despite different names*

### Comparing `SensiML-2023.2.1/sensiml/method_calls/__init__.py` & `SensiML-2023.3.0/sensiml/method_calls/__init__.py`

 * *Files identical despite different names*

### Comparing `SensiML-2023.2.1/sensiml/method_calls/augmentationcall.py` & `SensiML-2023.3.0/sensiml/method_calls/augmentationcall.py`

 * *Files identical despite different names*

### Comparing `SensiML-2023.2.1/sensiml/method_calls/augmentationcallset.py` & `SensiML-2023.3.0/sensiml/method_calls/augmentationcallset.py`

 * *Files identical despite different names*

### Comparing `SensiML-2023.2.1/sensiml/method_calls/basemethodcall.py` & `SensiML-2023.3.0/sensiml/method_calls/basemethodcall.py`

 * *Files identical despite different names*

### Comparing `SensiML-2023.2.1/sensiml/method_calls/capturefilecall.py` & `SensiML-2023.3.0/sensiml/method_calls/capturefilecall.py`

 * *Files identical despite different names*

### Comparing `SensiML-2023.2.1/sensiml/method_calls/datafilecall.py` & `SensiML-2023.3.0/sensiml/method_calls/datafilecall.py`

 * *Files identical despite different names*

### Comparing `SensiML-2023.2.1/sensiml/method_calls/featurefilecall.py` & `SensiML-2023.3.0/sensiml/method_calls/featurefilecall.py`

 * *Files identical despite different names*

### Comparing `SensiML-2023.2.1/sensiml/method_calls/functioncall.py` & `SensiML-2023.3.0/sensiml/method_calls/functioncall.py`

 * *Files identical despite different names*

### Comparing `SensiML-2023.2.1/sensiml/method_calls/functioncalls.py` & `SensiML-2023.3.0/sensiml/method_calls/functioncalls.py`

 * *Files identical despite different names*

### Comparing `SensiML-2023.2.1/sensiml/method_calls/generatorcall.py` & `SensiML-2023.3.0/sensiml/method_calls/generatorcall.py`

 * *Files identical despite different names*

### Comparing `SensiML-2023.2.1/sensiml/method_calls/generatorcallset.py` & `SensiML-2023.3.0/sensiml/method_calls/generatorcallset.py`

 * *Files identical despite different names*

### Comparing `SensiML-2023.2.1/sensiml/method_calls/querycall.py` & `SensiML-2023.3.0/sensiml/method_calls/querycall.py`

 * *Files identical despite different names*

### Comparing `SensiML-2023.2.1/sensiml/method_calls/selectorcall.py` & `SensiML-2023.3.0/sensiml/method_calls/selectorcall.py`

 * *Files identical despite different names*

### Comparing `SensiML-2023.2.1/sensiml/method_calls/selectorcallset.py` & `SensiML-2023.3.0/sensiml/method_calls/selectorcallset.py`

 * *Files identical despite different names*

### Comparing `SensiML-2023.2.1/sensiml/method_calls/trainandvalidationcall.py` & `SensiML-2023.3.0/sensiml/method_calls/trainandvalidationcall.py`

 * *Files identical despite different names*

### Comparing `SensiML-2023.2.1/sensiml/model_runner.py` & `SensiML-2023.3.0/sensiml/model_runner.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,15 +33,14 @@
 
 def dummy_function(*args, **kwrags):
     print("Not Supported by this version of the Knowledge Pack.")
     return None
 
 
 def compile_libsensiml_shared_library(path):
-
     current_dir = os.getcwd()
     try:
         os.chdir(path)
 
         if os.path.exists("libtensorflow-microlite.a"):
             print("calling: g++ --shared libtensorflow-microlite.a")
             subprocess.call(
@@ -61,36 +60,33 @@
     finally:
         os.chdir(current_dir)
 
     os.chdir(current_dir)
 
 
 def parse_model_json_for_class_map(path):
-
     if os.path.exists(os.path.join(path, "model.json")):
         model_info = json.load(open(os.path.join(path, "model.json"), "r"))
         class_maps = [x["ClassMaps"] for x in model_info["ModelDescriptions"]]
         return [{int(k): v for k, v in class_map.items()} for class_map in class_maps]
 
     return None
 
 
 def parse_model_json_for_model_type(path):
-
     if os.path.exists(os.path.join(path, "model.json")):
         model_info = json.load(open(os.path.join(path, "model.json"), "r"))
         return [
             description["ModelType"] for description in model_info["ModelDescriptions"]
         ]
 
     return None
 
 
 def is_tensorflow(ModelType):
-
     if type(ModelType) != str:
         return False
 
     if "TF Micro" in ModelType:
         return True
 
     if "TensorFlow Lite for Microcontrollers" in ModelType:
@@ -114,20 +110,30 @@
 
     _fields_ = [
         ("number_patterns", ctypes.c_uint16),
         ("pattern_length", ctypes.c_uint16),
     ]
 
 
+class struct_float_data_t(ctypes.Structure):
+    __slots__ = ["data", "size"]
+
+    _fields_ = [
+        ("data", ctypes.POINTER(ctypes.c_float)),
+        ("size", ctypes.c_int),
+    ]
+
+
 class struct_model_result(ctypes.Structure):
-    __slots__ = ["num_outputs", "output_tensor"]
+    __slots__ = ["model_type", "result", "output_tensor"]
 
     _fields_ = [
-        ("num_outputs", ctypes.c_ubyte),
-        ("output_tensor", ctypes.POINTER(ctypes.c_int16)),
+        ("model_type", ctypes.c_uint8),
+        ("result", ctypes.c_float),
+        ("output_tensor", ctypes.POINTER(struct_float_data_t)),
     ]
 
 
 def empty_function(*args, **kwargs):
     print("Not Supported by this Knowledge Pack.")
     return
 
@@ -300,36 +306,36 @@
 
         self._kb_get_sg_start_index = clf_lib.kb_get_sg_start_index
         self._kb_get_sg_start_index.argtypes = [
             ctypes.c_int,
         ]
         self._kb_get_sg_start_index.restype = ctypes.c_int
 
-        self._sml_get_segment_length = clf_lib.sml_get_segment_length
-        self._sml_get_segment_length.argtypes = [
+        self._kb_get_segment_length = clf_lib.kb_get_segment_length
+        self._kb_get_segment_length.argtypes = [
             ctypes.c_int,
-            ctypes.POINTER(ctypes.c_int),
         ]
+        self._kb_get_segment_length.restype = ctypes.c_int
 
         self._sml_get_feature_bank_number = clf_lib.sml_get_feature_bank_number
         self._sml_get_feature_bank_number.argtypes = [
             ctypes.c_int,
-            ctypes.POINTER(ctypes.c_int),
         ]
+        self._sml_get_feature_bank_number.restype = ctypes.c_int
 
         self._kb_get_segment_data = clf_lib.kb_get_segment_data
         self._kb_get_segment_data.argtypes = [
             ctypes.c_int,
             ctypes.c_int,
             ctypes.c_int,
             ctypes.POINTER(ctypes.c_int16),
         ]
 
-        self._kb_get_model_framelen = clf_lib.kb_get_model_framelen
-        self._kb_get_model_framelen.argtypes = [
+        self._kb_get_num_sensor_buffers = clf_lib.kb_get_num_sensor_buffers
+        self._kb_get_num_sensor_buffers.argtypes = [
             ctypes.c_int,
         ]
 
         # self._print_model_map = clf_lib.kb_print_model_map
 
         # self._print_model_result = clf_lib.kb_print_model_result
         # self._print_model_result.argtypes = [ctypes.c_int, ctypes.c_int]
@@ -357,22 +363,19 @@
         self._add_last_pattern_to_model.argtypes = [
             ctypes.c_int,
             ctypes.c_uint16,
             ctypes.c_uint16,
         ]
         self._add_last_pattern_to_model.restype = ctypes.c_int
 
-        self._kb_get_classification_result_info = (
-            clf_lib.kb_get_classification_result_info
-        )
-        self._kb_get_classification_result_info.argtypes = [
+        self._kb_get_model_result_info = clf_lib.kb_get_model_result_info
+        self._kb_get_model_result_info.argtypes = [
             ctypes.c_int,
-            ctypes.c_void_p,
         ]
-        self._kb_get_classification_result_info.restype = ctypes.c_int
+        self._kb_get_model_result_info.restype = ctypes.POINTER(struct_model_result)
 
         self._add_custom_pattern_to_model = clf_lib.kb_add_custom_pattern_to_model
         self._add_custom_pattern_to_model.argtypes = [
             ctypes.c_int,
             ctypes.POINTER(ctypes.c_uint8),
             ctypes.c_uint16,
             ctypes.c_uint16,
@@ -408,49 +411,46 @@
                 ctypes.c_int,
             ]
             self._sml_recognition_run.restype = ctypes.c_int
         except:
             self._sml_recognition_run = None
 
         try:
-            self._get_feature_vector = clf_lib.kb_get_feature_vector
-            self._get_feature_vector.argtypes = [
+            self._get_feature_vector_type = clf_lib.get_feature_vector_type
+            self._get_feature_vector_type.argtypes = [
                 ctypes.c_int,
-                ctypes.POINTER(ctypes.c_uint8),
-                ctypes.POINTER(ctypes.c_uint8),
             ]
+            self._get_feature_vector_type.restype = ctypes.c_uint8
         except:
-            self._get_feature_vector = empty_function
+            self._get_feature_vector_type = empty_function
 
         try:
-            self._get_feature_vector = clf_lib.kb_get_feature_vector
-            self._get_feature_vector.argtypes = [
+            self._get_feature_vector_size = clf_lib.kb_get_feature_vector_size
+            self._get_feature_vector_size.argtypes = [
                 ctypes.c_int,
-                ctypes.POINTER(ctypes.c_uint8),
-                ctypes.POINTER(ctypes.c_uint8),
             ]
+            self._get_feature_vector_size.restype = ctypes.c_uint16
         except:
-            self._get_feature_vector = empty_function
+            self._get_feature_vector_size = empty_function
 
         try:
-            self._set_feature_vector = clf_lib.kb_set_feature_vector
-            self._set_feature_vector.argtypes = [
+            self._copy_feature_vector = clf_lib.copy_feature_vector
+            self._copy_feature_vector.argtypes = [
                 ctypes.c_int,
-                ctypes.POINTER(ctypes.c_uint8),
+                ctypes.c_void_p,
             ]
         except:
-            self._set_feature_vector = empty_function
+            self._copy_feature_vector = empty_function
 
         try:
             self._set_feature_vector = clf_lib.kb_set_feature_vector
             self._set_feature_vector.argtypes = [
                 ctypes.c_int,
-                ctypes.POINTER(ctypes.c_uint8),
+                ctypes.POINTER(ctypes.c_void_p),
             ]
-            self._set_feature_vector.restype = ctypes.c_int
         except:
             self._set_feature_vector = empty_function
 
         try:
             self._recognize_feature_vector = clf_lib.kb_recognize_feature_vector
             self._recognize_feature_vector.argtypes = [ctypes.c_int]
             self._recognize_feature_vector.restype = ctypes.c_uint16
@@ -698,15 +698,14 @@
         for i in range(0, len(data)):
             # pass a single sample
             ret = self.run_model(
                 data.iloc[i], model_index=model_index, model_api=model_api
             )
 
             if ret >= 0:
-
                 output_columns = {
                     "label_value": ret
                     if self.get_class_map(model_index) is None
                     else self.get_class_map(model_index).get(ret, ret),
                     "capture_sample_sequence_start": i
                     + 1
                     - self.get_segment_length(model_index=model_index),
@@ -858,15 +857,14 @@
             tmp_dict["AIF"] = pattern.influence
             tmp_dict["Identifier"] = index
             model.append(tmp_dict)
 
         return DataFrame(model)
 
     def get_model_score(self, model_index):
-
         if not self._initialized():
             return
 
         model_index_ctype = ctypes.c_int(model_index)
 
         with pipes() as (out, _):
             self._print_model_score(model_index_ctype)
@@ -949,15 +947,15 @@
         """
 
         if not self._initialized():
             return
 
         model_index_ctype = ctypes.c_int(model_index)
 
-        n_sensors = self._kb_get_model_framelen(model_index_ctype)
+        n_sensors = self._kb_get_num_sensor_buffers(model_index_ctype)
 
         number_samples = self._kb_get_model_sg_length(model_index_ctype)
         index = self._kb_get_sg_start_index(model_index_ctype)
 
         number_samples_ctype = ctypes.c_int(number_samples)
         index_ctype = ctypes.c_int(index)
 
@@ -986,43 +984,46 @@
         """
 
         if not self._initialized():
             return
 
         model_index_ctype = ctypes.c_int(model_index)
 
-        framelen = self._kb_get_model_framelen(model_index_ctype)
+        framelen = self._kb_get_num_sensor_buffers(model_index_ctype)
 
         return int(framelen)
 
-    def get_feature_vector(
-        self, model_index: int = 0, feature_vector_buffer_size: int = 4096
-    ) -> List:
+    def get_feature_vector(self, model_index: int = 0) -> List:
         """Get the current feature vector from the model
 
         Args:
             model_index (int, optional): The model index. Defaults to 0.
             feature_vector_buffer_size (int, optional): The size of the array to use for getting the feature vector (This should be equal to or greater the size of the feature vector used by the model). Defaults to 4096.
 
         Returns:
             List: The models current feature vector
         """
 
         if not self._initialized():
             return
 
         model_index_ctype = ctypes.c_int(model_index)
-        feature_vector_ctype = (ctypes.c_ubyte * feature_vector_buffer_size)()
-        feature_length_ctype = ctypes.c_ubyte(0)
 
-        self._get_feature_vector(
-            model_index_ctype, feature_vector_ctype, ctypes.byref(feature_length_ctype)
-        )
+        size = self._get_feature_vector_size(model_index_ctype)
+        fv_type = self._get_feature_vector_type(model_index_ctype)
+        if fv_type == 1:
+            feature_vector_ctype = (ctypes.c_ubyte * size)()
+        else:
+            feature_vector_ctype = (ctypes.c_float * size)()
+
+        void_pointer = ctypes.cast(feature_vector_ctype, ctypes.c_void_p)
 
-        return list(feature_vector_ctype[: feature_length_ctype.value])
+        self._copy_feature_vector(model_index, void_pointer)
+
+        return list(feature_vector_ctype)
 
     def get_segment_length(self, model_index: int = 0) -> int:
         """Get the length of the current segment
 
         Args:
             model_index (int, optional): The model index. Defaults to 0.
 
@@ -1030,19 +1031,18 @@
             int: The length of the current segment
         """
 
         if not self._initialized():
             return
 
         model_index_ctype = ctypes.c_int(model_index)
-        segment_length = ctypes.c_int(0)
 
-        self._sml_get_segment_length(model_index_ctype, ctypes.byref(segment_length))
+        segment_length = self._kb_get_segment_length(model_index_ctype)
 
-        return segment_length.value
+        return segment_length
 
     def get_feature_bank_number(self, model_index: int = 0) -> int:
         """Get the number of feature banks this model uses
 
         Args:
             model_index (int, optional): The model index. Defaults to 0.
 
@@ -1050,18 +1050,17 @@
             int: The number of feature banks
         """
 
         if not self._initialized():
             return
 
         model_index_ctype = ctypes.c_int(model_index)
-        feature_bank_number = ctypes.c_int(0)
 
-        self._sml_get_feature_bank_number(
-            model_index_ctype, ctypes.byref(feature_bank_number)
+        feature_bank_number = self._sml_get_feature_bank_number(
+            model_index_ctype,
         )
 
         return feature_bank_number.value
 
     def set_feature_vector(self, model_index: int, feature_vector: list):
         """Sets the models feature vector to the specified values
 
@@ -1109,25 +1108,20 @@
         Returns:
             model results object for the specified model
         """
         if not self._initialized():
             return
 
         model_index_ctype = ctypes.c_int(model_index)
-        model_result = struct_model_result()
-        output_tensor = (ctypes.c_int16 * tensor_size)()
-        model_result.output_tensor = output_tensor
 
-        self._kb_get_classification_result_info(
-            model_index_ctype, ctypes.cast(ctypes.byref(model_result), ctypes.c_void_p)
-        )
+        model_results = self._kb_get_model_result_info(model_index_ctype)
 
         outputs = []
-        for i in range(model_result.num_outputs):
-            outputs.append(model_result.output_tensor[i])
+        for i in range(model_results.contents.output_tensor.contents.size):
+            outputs.append(model_results.contents.output_tensor.contents.data[i])
 
         return outputs
 
     def knowledgepack(
         self, model_index: int = 0, distance_mode: int = 0, feature_list=None
     ):
         """
```

### Comparing `SensiML-2023.2.1/sensiml/pipeline.py` & `SensiML-2023.3.0/sensiml/pipeline.py`

 * *Files 0% similar despite different names*

```diff
@@ -614,17 +614,17 @@
         Returns:
             A ModelResultSet if the selected pipeline step is TVO step, otherwise the output of the pipeline
             step is returned as a DataFrame.
         """
         try:
             return self._sandbox.intermediate_data(
                 pipeline_step=pipeline_step, page_index=page_index
-            )[0]
+            )
         except HTTPError:
-            return None
+            return None, None
 
     def visualize_features(self, feature_vector, label_column=None):
         """Makes a plot of feature vectors by class to aid in understanding your model
 
         Args:
             feature_vector (DataFrame): Dataframe containing feature vectors and label column
         """
@@ -669,22 +669,24 @@
         ).neuron_feature_map(featureX, featureY, neuron_alpha=neuron_alpha)
 
     def clear_cache(self):
         """Deletes the cache on KB cloud for this pipeline."""
         if self._sandbox is not None:
             self._sandbox.delete_cache()
 
-    def reset(self, delete_cache=False):
+    def reset(self, delete_cache: bool = False, update: bool = False):
         """Reset the current pipeline steps.
 
         Args:
             delete_cache (bool, False): Delete the cache from KB cloud.
+            update (bool, False): Push cleared pipeline to the server
         """
         self._sandbox.clear()
-        self._sandbox.update()
+        if update:
+            self._sandbox.update()
         self._generator_index = 0
         self._selector_index = 0
         self._data_columns = ""
         self._tvo_call = None
         self._classifier_call = None
         self._training_algorithm_call = None
         self._validation_call = None
@@ -1190,15 +1192,14 @@
         self._add_label_column(call)
         self._add_ignore_columns(call)
 
         self.tvo_index = self.get_pipeline_length()
         self._sandbox.add_linear_step(call)
 
     def _add_transform(self, transform, overwrite=True):
-
         if (
             self.get_function_type(transform["name"]) == "Segmenter"
             and self._use_query_session
         ):
             raise Exception(
                 "You have set use query session True, can't add a segmentation step."
             )
@@ -1236,15 +1237,14 @@
 
     def _add_feature_generator(
         self,
         feature_generators,
         feature_generator_params={},
         return_generator_set=False,
     ):
-
         self._check_for_input_data()
 
         generator_set = self._kb.functions.create_generator_call_set("generator_set")
 
         logger.debug("feature_generator_set")
 
         # set any generator set params given
@@ -1285,15 +1285,14 @@
         self._add_group_columns(generator_set)
 
         self._generator_index = self.get_pipeline_length()
 
         self._sandbox.add_linear_step(generator_set)
 
     def _add_augmentation(self, augmentations, augmentation_set_params, overwrite=True):
-
         self._check_for_input_data()
 
         augmentation_set = self._kb.functions.create_augmentation_call_set(
             "augmentation_set"
         )
 
         logger.debug("augmentation_set")
@@ -1318,15 +1317,14 @@
         self._add_label_column(augmentation_set)
 
         self._augmentation_index = self.get_pipeline_length()
 
         self._sandbox.add_linear_step(augmentation_set, overwrite)
 
     def _add_feature_selector(self, feature_selectors, selector_set_params={}):
-
         self._check_for_input_data()
         selector_set = self._kb.functions.create_selector_call_set("selector_set")
         logger.debug("feature_selector_set")
 
         for k, v in selector_set_params.items():
             setattr(selector_set, k, v)
 
@@ -1480,15 +1478,14 @@
             y_test.astype(dtype),
             y_validate.astype(dtype),
             class_map,
         )
 
 
 def get_contract_column_type(input_contract):
-
     column_contract = None
 
     for elem in input_contract:
         if elem.get("name", None) == "columns":
             column_contract = elem
             break
```

### Comparing `SensiML-2023.2.1/sensiml/profile/profile_data_parser.py` & `SensiML-2023.3.0/sensiml/profile/profile_data_parser.py`

 * *Files identical despite different names*

### Comparing `SensiML-2023.2.1/sensiml/tensorflow/utils.py` & `SensiML-2023.3.0/sensiml/tensorflow/utils.py`

 * *Files identical despite different names*

### Comparing `SensiML-2023.2.1/sensiml/visualize/knowledgepack_visualize_mixin.py` & `SensiML-2023.3.0/sensiml/visualize/knowledgepack_visualize_mixin.py`

 * *Files identical despite different names*

### Comparing `SensiML-2023.2.1/sensiml/visualize/visualize.py` & `SensiML-2023.3.0/sensiml/visualize/visualize.py`

 * *Files identical despite different names*

### Comparing `SensiML-2023.2.1/setup.py` & `SensiML-2023.3.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import os
 import sys
 
 from setuptools import find_packages, setup
 
-__version__ = "2023.2.1"
+__version__ = "2023.3.0"
 
 # 'setup.py publish' shortcut.
 if sys.argv[-1] == "publish":
     os.system("python setup.py sdist bdist_wheel")
     os.system("twine upload dist/*")
     sys.exit()
```

