# Comparing `tmp/ayeaye-fossa-0.0.8.tar.gz` & `tmp/ayeaye-fossa-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ayeaye-fossa-0.0.8.tar", last modified: Thu Mar 21 21:09:02 2024, max compression
+gzip compressed data, was "ayeaye-fossa-0.0.9.tar", last modified: Mon Mar 25 16:40:43 2024, max compression
```

## Comparing `ayeaye-fossa-0.0.8.tar` & `ayeaye-fossa-0.0.9.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxr-xr-x   0 si         (501) staff       (20)        0 2024-03-21 21:09:02.236642 ayeaye-fossa-0.0.8/
--rw-r--r--   0 si         (501) staff       (20)    11357 2022-05-19 13:55:03.000000 ayeaye-fossa-0.0.8/LICENSE
--rw-r--r--   0 si         (501) staff       (20)       86 2024-03-07 11:29:36.000000 ayeaye-fossa-0.0.8/MANIFEST.in
--rw-r--r--   0 si         (501) staff       (20)     4650 2024-03-21 21:09:02.236582 ayeaye-fossa-0.0.8/PKG-INFO
--rw-r--r--   0 si         (501) staff       (20)     3971 2024-03-06 21:32:17.000000 ayeaye-fossa-0.0.8/README.md
-drwxr-xr-x   0 si         (501) staff       (20)        0 2024-03-21 21:09:02.228862 ayeaye-fossa-0.0.8/lib/
-drwxr-xr-x   0 si         (501) staff       (20)        0 2024-03-21 21:09:02.236267 ayeaye-fossa-0.0.8/lib/ayeaye_fossa.egg-info/
--rw-r--r--   0 si         (501) staff       (20)     4650 2024-03-21 21:09:02.000000 ayeaye-fossa-0.0.8/lib/ayeaye_fossa.egg-info/PKG-INFO
--rw-r--r--   0 si         (501) staff       (20)      986 2024-03-21 21:09:02.000000 ayeaye-fossa-0.0.8/lib/ayeaye_fossa.egg-info/SOURCES.txt
--rw-r--r--   0 si         (501) staff       (20)        1 2024-03-21 21:09:02.000000 ayeaye-fossa-0.0.8/lib/ayeaye_fossa.egg-info/dependency_links.txt
--rw-r--r--   0 si         (501) staff       (20)       41 2024-03-21 21:09:02.000000 ayeaye-fossa-0.0.8/lib/ayeaye_fossa.egg-info/requires.txt
--rw-r--r--   0 si         (501) staff       (20)        6 2024-03-21 21:09:02.000000 ayeaye-fossa-0.0.8/lib/ayeaye_fossa.egg-info/top_level.txt
-drwxr-xr-x   0 si         (501) staff       (20)        0 2024-03-21 21:09:02.231868 ayeaye-fossa-0.0.8/lib/fossa/
--rw-r--r--   0 si         (501) staff       (20)      111 2024-03-05 21:33:53.000000 ayeaye-fossa-0.0.8/lib/fossa/__init__.py
--rw-r--r--   0 si         (501) staff       (20)     2800 2024-03-05 13:18:39.000000 ayeaye-fossa-0.0.8/lib/fossa/app.py
-drwxr-xr-x   0 si         (501) staff       (20)        0 2024-03-21 21:09:02.233108 ayeaye-fossa-0.0.8/lib/fossa/control/
--rw-r--r--   0 si         (501) staff       (20)        0 2024-03-05 14:49:10.000000 ayeaye-fossa-0.0.8/lib/fossa/control/__init__.py
--rw-r--r--   0 si         (501) staff       (20)     2594 2024-03-05 13:18:39.000000 ayeaye-fossa-0.0.8/lib/fossa/control/broker.py
--rw-r--r--   0 si         (501) staff       (20)    14429 2024-03-05 13:18:39.000000 ayeaye-fossa-0.0.8/lib/fossa/control/governor.py
--rw-r--r--   0 si         (501) staff       (20)      874 2024-02-06 13:39:00.000000 ayeaye-fossa-0.0.8/lib/fossa/control/message.py
--rw-r--r--   0 si         (501) staff       (20)     5427 2024-03-05 13:18:39.000000 ayeaye-fossa-0.0.8/lib/fossa/control/process.py
-drwxr-xr-x   0 si         (501) staff       (20)        0 2024-03-21 21:09:02.234096 ayeaye-fossa-0.0.8/lib/fossa/control/rabbit_mq/
--rw-r--r--   0 si         (501) staff       (20)        0 2024-03-05 14:49:42.000000 ayeaye-fossa-0.0.8/lib/fossa/control/rabbit_mq/__init__.py
--rw-r--r--   0 si         (501) staff       (20)     3363 2024-03-21 20:57:37.000000 ayeaye-fossa-0.0.8/lib/fossa/control/rabbit_mq/message_exchange.py
--rw-r--r--   0 si         (501) staff       (20)     2609 2024-03-21 21:02:31.000000 ayeaye-fossa-0.0.8/lib/fossa/control/rabbit_mq/pika_client.py
--rw-r--r--   0 si         (501) staff       (20)     1787 2024-03-05 13:18:39.000000 ayeaye-fossa-0.0.8/lib/fossa/control/rabbit_mq/process.py
--rw-r--r--   0 si         (501) staff       (20)     4157 2024-03-21 20:57:37.000000 ayeaye-fossa-0.0.8/lib/fossa/control/rabbit_mq/process_pool.py
--rw-r--r--   0 si         (501) staff       (20)     1453 2024-03-05 21:34:04.000000 ayeaye-fossa-0.0.8/lib/fossa/main.py
-drwxr-xr-x   0 si         (501) staff       (20)        0 2024-03-21 21:09:02.234347 ayeaye-fossa-0.0.8/lib/fossa/settings/
--rw-r--r--   0 si         (501) staff       (20)      404 2024-03-05 21:32:47.000000 ayeaye-fossa-0.0.8/lib/fossa/settings/global_config.py
-drwxr-xr-x   0 si         (501) staff       (20)        0 2024-03-21 21:09:02.234739 ayeaye-fossa-0.0.8/lib/fossa/templates/
--rw-r--r--   0 si         (501) staff       (20)      994 2024-01-23 11:02:48.000000 ayeaye-fossa-0.0.8/lib/fossa/templates/base.html
--rw-r--r--   0 si         (501) staff       (20)     1163 2024-03-18 10:49:05.000000 ayeaye-fossa-0.0.8/lib/fossa/templates/web_root.html
-drwxr-xr-x   0 si         (501) staff       (20)        0 2024-03-21 21:09:02.235103 ayeaye-fossa-0.0.8/lib/fossa/tools/
--rw-r--r--   0 si         (501) staff       (20)        0 2024-03-05 20:52:32.000000 ayeaye-fossa-0.0.8/lib/fossa/tools/__init__.py
--rw-r--r--   0 si         (501) staff       (20)     2458 2024-03-05 13:18:39.000000 ayeaye-fossa-0.0.8/lib/fossa/tools/logging.py
--rw-r--r--   0 si         (501) staff       (20)     2869 2024-03-05 13:18:39.000000 ayeaye-fossa-0.0.8/lib/fossa/tools/logging_cloudwatch.py
--rw-r--r--   0 si         (501) staff       (20)     1979 2024-02-06 13:54:19.000000 ayeaye-fossa-0.0.8/lib/fossa/utils.py
-drwxr-xr-x   0 si         (501) staff       (20)        0 2024-03-21 21:09:02.235957 ayeaye-fossa-0.0.8/lib/fossa/views/
--rw-r--r--   0 si         (501) staff       (20)        0 2024-03-05 14:51:47.000000 ayeaye-fossa-0.0.8/lib/fossa/views/__init__.py
--rw-r--r--   0 si         (501) staff       (20)     2054 2024-03-18 12:18:08.000000 ayeaye-fossa-0.0.8/lib/fossa/views/api.py
--rw-r--r--   0 si         (501) staff       (20)      994 2024-03-18 10:44:52.000000 ayeaye-fossa-0.0.8/lib/fossa/views/controller.py
--rw-r--r--   0 si         (501) staff       (20)      394 2024-03-18 10:38:45.000000 ayeaye-fossa-0.0.8/lib/fossa/views/web.py
--rw-r--r--   0 si         (501) staff       (20)       82 2024-03-05 14:04:08.000000 ayeaye-fossa-0.0.8/pyproject.toml
--rw-r--r--   0 si         (501) staff       (20)      788 2024-03-21 21:09:02.236883 ayeaye-fossa-0.0.8/setup.cfg
+drwxr-xr-x   0 si         (501) staff       (20)        0 2024-03-25 16:40:43.293610 ayeaye-fossa-0.0.9/
+-rw-r--r--   0 si         (501) staff       (20)    11357 2022-05-19 13:55:03.000000 ayeaye-fossa-0.0.9/LICENSE
+-rw-r--r--   0 si         (501) staff       (20)       86 2024-03-07 11:29:36.000000 ayeaye-fossa-0.0.9/MANIFEST.in
+-rw-r--r--   0 si         (501) staff       (20)     4787 2024-03-25 16:40:43.293533 ayeaye-fossa-0.0.9/PKG-INFO
+-rw-r--r--   0 si         (501) staff       (20)     4108 2024-03-25 16:20:32.000000 ayeaye-fossa-0.0.9/README.md
+drwxr-xr-x   0 si         (501) staff       (20)        0 2024-03-25 16:40:43.287522 ayeaye-fossa-0.0.9/lib/
+drwxr-xr-x   0 si         (501) staff       (20)        0 2024-03-25 16:40:43.293289 ayeaye-fossa-0.0.9/lib/ayeaye_fossa.egg-info/
+-rw-r--r--   0 si         (501) staff       (20)     4787 2024-03-25 16:40:43.000000 ayeaye-fossa-0.0.9/lib/ayeaye_fossa.egg-info/PKG-INFO
+-rw-r--r--   0 si         (501) staff       (20)      986 2024-03-25 16:40:43.000000 ayeaye-fossa-0.0.9/lib/ayeaye_fossa.egg-info/SOURCES.txt
+-rw-r--r--   0 si         (501) staff       (20)        1 2024-03-25 16:40:43.000000 ayeaye-fossa-0.0.9/lib/ayeaye_fossa.egg-info/dependency_links.txt
+-rw-r--r--   0 si         (501) staff       (20)       41 2024-03-25 16:40:43.000000 ayeaye-fossa-0.0.9/lib/ayeaye_fossa.egg-info/requires.txt
+-rw-r--r--   0 si         (501) staff       (20)        6 2024-03-25 16:40:43.000000 ayeaye-fossa-0.0.9/lib/ayeaye_fossa.egg-info/top_level.txt
+drwxr-xr-x   0 si         (501) staff       (20)        0 2024-03-25 16:40:43.290228 ayeaye-fossa-0.0.9/lib/fossa/
+-rw-r--r--   0 si         (501) staff       (20)      111 2024-03-05 21:33:53.000000 ayeaye-fossa-0.0.9/lib/fossa/__init__.py
+-rw-r--r--   0 si         (501) staff       (20)     2800 2024-03-05 13:18:39.000000 ayeaye-fossa-0.0.9/lib/fossa/app.py
+drwxr-xr-x   0 si         (501) staff       (20)        0 2024-03-25 16:40:43.291156 ayeaye-fossa-0.0.9/lib/fossa/control/
+-rw-r--r--   0 si         (501) staff       (20)        0 2024-03-05 14:49:10.000000 ayeaye-fossa-0.0.9/lib/fossa/control/__init__.py
+-rw-r--r--   0 si         (501) staff       (20)     2594 2024-03-05 13:18:39.000000 ayeaye-fossa-0.0.9/lib/fossa/control/broker.py
+-rw-r--r--   0 si         (501) staff       (20)    14836 2024-03-25 16:36:43.000000 ayeaye-fossa-0.0.9/lib/fossa/control/governor.py
+-rw-r--r--   0 si         (501) staff       (20)     1015 2024-03-25 15:40:12.000000 ayeaye-fossa-0.0.9/lib/fossa/control/message.py
+-rw-r--r--   0 si         (501) staff       (20)     5856 2024-03-25 16:35:11.000000 ayeaye-fossa-0.0.9/lib/fossa/control/process.py
+drwxr-xr-x   0 si         (501) staff       (20)        0 2024-03-25 16:40:43.291822 ayeaye-fossa-0.0.9/lib/fossa/control/rabbit_mq/
+-rw-r--r--   0 si         (501) staff       (20)        0 2024-03-05 14:49:42.000000 ayeaye-fossa-0.0.9/lib/fossa/control/rabbit_mq/__init__.py
+-rw-r--r--   0 si         (501) staff       (20)     3248 2024-03-25 16:14:31.000000 ayeaye-fossa-0.0.9/lib/fossa/control/rabbit_mq/message_exchange.py
+-rw-r--r--   0 si         (501) staff       (20)     2609 2024-03-21 21:02:31.000000 ayeaye-fossa-0.0.9/lib/fossa/control/rabbit_mq/pika_client.py
+-rw-r--r--   0 si         (501) staff       (20)     1787 2024-03-05 13:18:39.000000 ayeaye-fossa-0.0.9/lib/fossa/control/rabbit_mq/process.py
+-rw-r--r--   0 si         (501) staff       (20)     4559 2024-03-25 15:40:12.000000 ayeaye-fossa-0.0.9/lib/fossa/control/rabbit_mq/process_pool.py
+-rw-r--r--   0 si         (501) staff       (20)     1453 2024-03-05 21:34:04.000000 ayeaye-fossa-0.0.9/lib/fossa/main.py
+drwxr-xr-x   0 si         (501) staff       (20)        0 2024-03-25 16:40:43.291989 ayeaye-fossa-0.0.9/lib/fossa/settings/
+-rw-r--r--   0 si         (501) staff       (20)      404 2024-03-05 21:32:47.000000 ayeaye-fossa-0.0.9/lib/fossa/settings/global_config.py
+drwxr-xr-x   0 si         (501) staff       (20)        0 2024-03-25 16:40:43.292265 ayeaye-fossa-0.0.9/lib/fossa/templates/
+-rw-r--r--   0 si         (501) staff       (20)      994 2024-01-23 11:02:48.000000 ayeaye-fossa-0.0.9/lib/fossa/templates/base.html
+-rw-r--r--   0 si         (501) staff       (20)     1163 2024-03-18 10:49:05.000000 ayeaye-fossa-0.0.9/lib/fossa/templates/web_root.html
+drwxr-xr-x   0 si         (501) staff       (20)        0 2024-03-25 16:40:43.292612 ayeaye-fossa-0.0.9/lib/fossa/tools/
+-rw-r--r--   0 si         (501) staff       (20)        0 2024-03-05 20:52:32.000000 ayeaye-fossa-0.0.9/lib/fossa/tools/__init__.py
+-rw-r--r--   0 si         (501) staff       (20)     2458 2024-03-05 13:18:39.000000 ayeaye-fossa-0.0.9/lib/fossa/tools/logging.py
+-rw-r--r--   0 si         (501) staff       (20)     2869 2024-03-05 13:18:39.000000 ayeaye-fossa-0.0.9/lib/fossa/tools/logging_cloudwatch.py
+-rw-r--r--   0 si         (501) staff       (20)     1979 2024-02-06 13:54:19.000000 ayeaye-fossa-0.0.9/lib/fossa/utils.py
+drwxr-xr-x   0 si         (501) staff       (20)        0 2024-03-25 16:40:43.293119 ayeaye-fossa-0.0.9/lib/fossa/views/
+-rw-r--r--   0 si         (501) staff       (20)        0 2024-03-05 14:51:47.000000 ayeaye-fossa-0.0.9/lib/fossa/views/__init__.py
+-rw-r--r--   0 si         (501) staff       (20)     2141 2024-03-25 10:26:58.000000 ayeaye-fossa-0.0.9/lib/fossa/views/api.py
+-rw-r--r--   0 si         (501) staff       (20)      994 2024-03-18 10:44:52.000000 ayeaye-fossa-0.0.9/lib/fossa/views/controller.py
+-rw-r--r--   0 si         (501) staff       (20)      394 2024-03-18 10:38:45.000000 ayeaye-fossa-0.0.9/lib/fossa/views/web.py
+-rw-r--r--   0 si         (501) staff       (20)       82 2024-03-05 14:04:08.000000 ayeaye-fossa-0.0.9/pyproject.toml
+-rw-r--r--   0 si         (501) staff       (20)      788 2024-03-25 16:40:43.293854 ayeaye-fossa-0.0.9/setup.cfg
```

### Comparing `ayeaye-fossa-0.0.8/LICENSE` & `ayeaye-fossa-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `ayeaye-fossa-0.0.8/PKG-INFO` & `ayeaye-fossa-0.0.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: ayeaye-fossa
-Version: 0.0.8
+Version: 0.0.9
 Summary: Execution engine for Aye-Aye ETL models
 Home-page: https://github.com/Aye-Aye-Dev/Fossa
 Author: Si Parker
 Author-email: ayeaye@plogic.co.uk
 Project-URL: Bug Tracker, https://github.com/Aye-Aye-Dev/Fossa/issues
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: flask
 Requires-Dist: gunicorn
-Requires-Dist: ayeaye>=0.0.55
+Requires-Dist: ayeaye>=0.0.56
 Requires-Dist: pika
 Requires-Dist: boto3
 
 # fossa
 Execution engine for Aye-Aye ETL models
 
 ## Overview
@@ -104,28 +104,34 @@
 
 ```
 python fossa/app.py
 ```
 
 You'll now have a locally running web app. It will output IP addresses it is accepting connections from. Typically just point a browser at `http://0.0.0.0:2345/'
 
+## Running Fossa locally using gunicorn
+
+```shell
+export PYTHONPATH=`pwd`:`pwd`/lib
+DEPLOYMENT_ENVIRONMENT=local python lib/fossa/main.py
+```
 
 ### Posting a task
 
 In a production environment tasks are more likely to arrive through a message queue. But it's also possible to use an HTTP POST to submit a task.
 
 If you used the `local_config_example.py` file as a starting point for your local config it will have a single model already in the `ACCEPTED_MODEL_CLASSES` parameter. This is a tiny example ETL model.
 
 Fossa will only run models that have been pre-defined before start-up. A simple way to supply these models is through the config file but there are other ways too.
 
 POST to your local instance of Fossa a task specification. This example runs the complete `SimpleExampleEtl` model-
 
 ```shell
 curl --header "Content-Type: application/json" \
-     --data '{"model_class":"SimpleExampleEtl"}'  \
+     --data '{"model_class":"NothingEtl"}'  \
      --request POST http://0.0.0.0:2345/api/0.01/task
 ```
 
 
 ### Distributed (but still local) processing
 
 TODO
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `ayeaye-fossa-0.0.8/README.md` & `ayeaye-fossa-0.0.9/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -83,28 +83,34 @@
 
 ```
 python fossa/app.py
 ```
 
 You'll now have a locally running web app. It will output IP addresses it is accepting connections from. Typically just point a browser at `http://0.0.0.0:2345/'
 
+## Running Fossa locally using gunicorn
+
+```shell
+export PYTHONPATH=`pwd`:`pwd`/lib
+DEPLOYMENT_ENVIRONMENT=local python lib/fossa/main.py
+```
 
 ### Posting a task
 
 In a production environment tasks are more likely to arrive through a message queue. But it's also possible to use an HTTP POST to submit a task.
 
 If you used the `local_config_example.py` file as a starting point for your local config it will have a single model already in the `ACCEPTED_MODEL_CLASSES` parameter. This is a tiny example ETL model.
 
 Fossa will only run models that have been pre-defined before start-up. A simple way to supply these models is through the config file but there are other ways too.
 
 POST to your local instance of Fossa a task specification. This example runs the complete `SimpleExampleEtl` model-
 
 ```shell
 curl --header "Content-Type: application/json" \
-     --data '{"model_class":"SimpleExampleEtl"}'  \
+     --data '{"model_class":"NothingEtl"}'  \
      --request POST http://0.0.0.0:2345/api/0.01/task
 ```
 
 
 ### Distributed (but still local) processing
 
 TODO
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `ayeaye-fossa-0.0.8/lib/ayeaye_fossa.egg-info/PKG-INFO` & `ayeaye-fossa-0.0.9/lib/ayeaye_fossa.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: ayeaye-fossa
-Version: 0.0.8
+Version: 0.0.9
 Summary: Execution engine for Aye-Aye ETL models
 Home-page: https://github.com/Aye-Aye-Dev/Fossa
 Author: Si Parker
 Author-email: ayeaye@plogic.co.uk
 Project-URL: Bug Tracker, https://github.com/Aye-Aye-Dev/Fossa/issues
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: flask
 Requires-Dist: gunicorn
-Requires-Dist: ayeaye>=0.0.55
+Requires-Dist: ayeaye>=0.0.56
 Requires-Dist: pika
 Requires-Dist: boto3
 
 # fossa
 Execution engine for Aye-Aye ETL models
 
 ## Overview
@@ -104,28 +104,34 @@
 
 ```
 python fossa/app.py
 ```
 
 You'll now have a locally running web app. It will output IP addresses it is accepting connections from. Typically just point a browser at `http://0.0.0.0:2345/'
 
+## Running Fossa locally using gunicorn
+
+```shell
+export PYTHONPATH=`pwd`:`pwd`/lib
+DEPLOYMENT_ENVIRONMENT=local python lib/fossa/main.py
+```
 
 ### Posting a task
 
 In a production environment tasks are more likely to arrive through a message queue. But it's also possible to use an HTTP POST to submit a task.
 
 If you used the `local_config_example.py` file as a starting point for your local config it will have a single model already in the `ACCEPTED_MODEL_CLASSES` parameter. This is a tiny example ETL model.
 
 Fossa will only run models that have been pre-defined before start-up. A simple way to supply these models is through the config file but there are other ways too.
 
 POST to your local instance of Fossa a task specification. This example runs the complete `SimpleExampleEtl` model-
 
 ```shell
 curl --header "Content-Type: application/json" \
-     --data '{"model_class":"SimpleExampleEtl"}'  \
+     --data '{"model_class":"NothingEtl"}'  \
      --request POST http://0.0.0.0:2345/api/0.01/task
 ```
 
 
 ### Distributed (but still local) processing
 
 TODO
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `ayeaye-fossa-0.0.8/lib/ayeaye_fossa.egg-info/SOURCES.txt` & `ayeaye-fossa-0.0.9/lib/ayeaye_fossa.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ayeaye-fossa-0.0.8/lib/fossa/app.py` & `ayeaye-fossa-0.0.9/lib/fossa/app.py`

 * *Files identical despite different names*

### Comparing `ayeaye-fossa-0.0.8/lib/fossa/control/broker.py` & `ayeaye-fossa-0.0.9/lib/fossa/control/broker.py`

 * *Files identical despite different names*

### Comparing `ayeaye-fossa-0.0.8/lib/fossa/control/governor.py` & `ayeaye-fossa-0.0.9/lib/fossa/control/governor.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 import random
 import string
 
 from ayeaye.runtime.knowledge import RuntimeKnowledge
 
 from fossa.control.broker import AbstractMycorrhiza
 from fossa.control.message import TaskMessage, ResultsMessage, TerminateMessage
-from fossa.control.process import LocalAyeAyeProcessor
+from fossa.control.process import AbstractIsolatedProcessor, LocalAyeAyeProcessor
 from fossa.tools.logging import LoggingMixin, MiniLogger
 
 
 class InvalidTaskSpec(ValueError):
     pass
 
 
@@ -99,14 +99,19 @@
             self._isolated_processor.copy_logging_setup(self)
 
         return self._isolated_processor
 
     @isolated_processor.setter
     def isolated_processor(self, processor):
         "See doc. string in getter version of :meth:`isolated_processor`"
+
+        if not issubclass(processor.__class__, AbstractIsolatedProcessor):
+            msg = "The isolated processor must be a subclass of `AbstractIsolatedProcessor`"
+            raise ValueError(msg)
+
         self._isolated_processor = processor
         self._isolated_processor.set_work_queue(self._task_queue_submit)
 
         # copy logging setup across if supported by processor
         if isinstance(self._isolated_processor, LoggingMixin):
             self._isolated_processor.copy_logging_setup(self)
 
@@ -240,17 +245,19 @@
                     raise InvalidTaskSpec(msg)
 
                 TaskCls = available_classes[task_spec.model_class]
 
                 iso_proc_kwargs = {
                     "task_id": proc_id,
                     "model_cls": TaskCls,
+                    "model_construction_kwargs": task_spec.model_construction_kwargs,
                     "method": task_spec.method,
                     "method_kwargs": task_spec.method_kwargs,
                     "resolver_context": task_spec.resolver_context,
+                    "partition_initialise_kwargs": task_spec.partition_initialise_kwargs,
                 }
 
                 process_table[proc_id] = {
                     "task_spec": task_spec,
                     "started": datetime.utcnow(),
                 }
```

### Comparing `ayeaye-fossa-0.0.8/lib/fossa/control/process.py` & `ayeaye-fossa-0.0.9/lib/fossa/control/process.py`

 * *Files 6% similar despite different names*

```diff
@@ -49,47 +49,63 @@
         For example, if just the `process_pool` needs to be changed then the subclass won't need to
         implement :meth:`__call__` etc.
 
         @param model: (subclass of :class:`ayeaye.Model`)
         """
         return None
 
-    def __call__(self, task_id, model_cls, method, method_kwargs, resolver_context):
+    def __call__(
+        self,
+        task_id,
+        model_cls,
+        model_construction_kwargs,
+        method,
+        method_kwargs,
+        resolver_context,
+        partition_initialise_kwargs,
+    ):
         """
         Run/execute the model.
 
         This method is run in a separate :class:`multiprocessing.Process` so don't mutate any
         instance variables.
 
         The execution is wrapped within an `ayeaye.connector_resolver` and a try except.
 
         Results, stack-traces etc. are sent back to the parent process over the `self.work_queue`
         Pipe.
 
         @param task_id: (str)
         @param model_cls: (Class, not instance)
+        @param model_construction_kwargs: (dict)
         @param method: (str)
         @param method_kwargs: (dict)
         @param resolver_context: (dict)
+        @param partition_initialise_kwargs: (dict)
         @return: None
         """
         try:
             with ayeaye.connector_resolver.context(**resolver_context):
-                model = model_cls()
+                model = model_cls(**model_construction_kwargs)
+
+                if isinstance(model, ayeaye.PartitionedModel):
+                    model.partition_initialise(**partition_initialise_kwargs)
 
                 # optional hook used by subclasses
                 self.on_model_start(model)
 
                 # TODO - attach logging - hint - send TaskLogMessage down self.work_queue
 
                 sub_task_method = getattr(model, method)
                 subtask_return_value = sub_task_method(**method_kwargs)
 
             task_complete = TaskComplete(
-                method_name=method, method_kwargs=method_kwargs, return_value=subtask_return_value
+                method_name=method,
+                method_kwargs=method_kwargs,
+                return_value=subtask_return_value,
             )
 
             result_spec = ResultsMessage(
                 task_id=task_id,
                 task_message=task_complete.to_json(),
             )
```

### Comparing `ayeaye-fossa-0.0.8/lib/fossa/control/rabbit_mq/message_exchange.py` & `ayeaye-fossa-0.0.9/lib/fossa/control/rabbit_mq/message_exchange.py`

 * *Files 5% similar despite different names*

```diff
@@ -48,20 +48,16 @@
         ):
             msg = f"exchange received {body} {properties.correlation_id} -> {properties.reply_to}"
             self.log(msg)
 
             # TODO use proper types
             rabbit_decoded_task = json.loads(body)
 
-            # TODO rename to 'partition_initialise' and use it
-            del rabbit_decoded_task["initialise"]
-
             # keep track of where the sub-task's work should be sent.
             composite_task_id = f"{properties.correlation_id}::{properties.reply_to}"
-
             task_spec = TaskMessage(
                 task_id=composite_task_id,
                 **rabbit_decoded_task,
                 on_completion_callback=self.callback_on_processing_complete,
             )
 
             RabbitMx.submit_task(task_spec, work_queue_submit, available_processing_capacity)
```

### Comparing `ayeaye-fossa-0.0.8/lib/fossa/control/rabbit_mq/pika_client.py` & `ayeaye-fossa-0.0.9/lib/fossa/control/rabbit_mq/pika_client.py`

 * *Files identical despite different names*

### Comparing `ayeaye-fossa-0.0.8/lib/fossa/control/rabbit_mq/process.py` & `ayeaye-fossa-0.0.9/lib/fossa/control/rabbit_mq/process.py`

 * *Files identical despite different names*

### Comparing `ayeaye-fossa-0.0.8/lib/fossa/control/rabbit_mq/process_pool.py` & `ayeaye-fossa-0.0.9/lib/fossa/control/rabbit_mq/process_pool.py`

 * *Files 6% similar despite different names*

```diff
@@ -19,48 +19,46 @@
 
     def __init__(self, broker_url):
         LoggingMixin.__init__(self)
         self.rabbit_mq = BasicPikaClient(url=broker_url)
         self.tasks_in_flight = {}
         self.pool_id = "".join([random.choice(string.ascii_lowercase) for _ in range(5)])
 
-    def run_subtasks(
-        self,
-        model_cls,
-        sub_tasks,
-        initialise=None,
-        context_kwargs=None,
-        processes=None,
-    ):
+    def run_subtasks(self, model_cls, sub_tasks, context_kwargs=None, processes=None):
         """
         Generator yielding instances that are a subclass of :class:`AbstractTaskMessage`. These
         are from subtasks.
 
         @see doc. string in :meth:`AbstractProcessPool.run_subtasks`
         """
         if processes is None:
             # if the count of processes is used to distribute the workers this will work
             processes = len(sub_tasks)
 
         # fortunately sub_tasks is a list (not a generator) so all tasks can be sent
         for subtask_number, sub_task in enumerate(sub_tasks):
+            # sub_task is a :class:`TaskPartition` object
+            # See Aye-aye's `ayeaye.runtime.task_message.TaskPartition`
             subtask_id = f"{self.pool_id}:{subtask_number}"
-            method_name, method_kwargs = sub_task
-
             task_definition = {
                 "model_class": model_cls.__name__,
-                "method": method_name,
-                "method_kwargs": method_kwargs,
+                "method": sub_task.method_name,
+                "method_kwargs": sub_task.method_kwargs,
                 "resolver_context": context_kwargs,
-                "initialise": initialise,
+                "model_construction_kwargs": sub_task.model_construction_kwargs,
+                "partition_initialise_kwargs": sub_task.partition_initialise_kwargs,
             }
             task_definition_json = json.dumps(task_definition)
 
             self.tasks_in_flight[subtask_id] = task_definition
             self.tasks_in_flight[subtask_id]["start_time"] = datetime.utcnow()
+
+            # This JSON encoded payload will be received in :meth:`RabbitMx.run_forever` where
+            # all of it will be used alongside some additional args to build :class:`TaskMessage`
+            # TODO - Better typing should be used
             self.send_task(subtask_id=subtask_id, task_payload=task_definition_json)
 
         for _not_connected in self.rabbit_mq.connect():
             self.log("Waiting to connect to RabbitMQ....", "WARNING")
         self.log("Connected to RabbitMQ")
 
         # Listen for subtasks completing
@@ -88,15 +86,15 @@
 
             if len(self.tasks_in_flight) == 0:
                 self.log("All tasks complete")
                 return
 
     def send_task(self, subtask_id, task_payload):
         """
-        Send a work instruction to be picked up by any worker.
+        Send a work instruction to be picked up by any RabbitMq worker.
         @param subtask_id (str):
         @param task_payload (str):
         """
         for _not_connected in self.rabbit_mq.connect():
             self.log("Waiting to connect to RabbitMQ....", "WARNING")
         self.log("Connected to RabbitMQ")
```

### Comparing `ayeaye-fossa-0.0.8/lib/fossa/main.py` & `ayeaye-fossa-0.0.9/lib/fossa/main.py`

 * *Files identical despite different names*

### Comparing `ayeaye-fossa-0.0.8/lib/fossa/templates/base.html` & `ayeaye-fossa-0.0.9/lib/fossa/templates/base.html`

 * *Files identical despite different names*

### Comparing `ayeaye-fossa-0.0.8/lib/fossa/templates/web_root.html` & `ayeaye-fossa-0.0.9/lib/fossa/templates/web_root.html`

 * *Files identical despite different names*

### Comparing `ayeaye-fossa-0.0.8/lib/fossa/tools/logging.py` & `ayeaye-fossa-0.0.9/lib/fossa/tools/logging.py`

 * *Files identical despite different names*

### Comparing `ayeaye-fossa-0.0.8/lib/fossa/tools/logging_cloudwatch.py` & `ayeaye-fossa-0.0.9/lib/fossa/tools/logging_cloudwatch.py`

 * *Files identical despite different names*

### Comparing `ayeaye-fossa-0.0.8/lib/fossa/utils.py` & `ayeaye-fossa-0.0.9/lib/fossa/utils.py`

 * *Files identical despite different names*

### Comparing `ayeaye-fossa-0.0.8/lib/fossa/views/api.py` & `ayeaye-fossa-0.0.9/lib/fossa/views/api.py`

 * *Files 11% similar despite different names*

```diff
@@ -31,14 +31,15 @@
 
     request_doc = request.get_json()
     if "model_class" not in request_doc:
         raise JsonException(message="'model_class' is a mandatory field", status_code=400)
 
     task_attribs = {
         "model_class": request_doc["model_class"],
+        "model_construction_kwargs": request_doc.get("model_construction_kwargs", {}),
         "method": request_doc.get("method", "go"),  # default for Ayeaye is to run the whole model
         "method_kwargs": request_doc.get("method_kwargs", {}),
         "resolver_context": request_doc.get("resolver_context", {}),
         "on_completion_callback": test_func,
     }
     new_task = TaskMessage(**task_attribs)
```

### Comparing `ayeaye-fossa-0.0.8/lib/fossa/views/controller.py` & `ayeaye-fossa-0.0.9/lib/fossa/views/controller.py`

 * *Files identical despite different names*

### Comparing `ayeaye-fossa-0.0.8/setup.cfg` & `ayeaye-fossa-0.0.9/setup.cfg`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = ayeaye-fossa
-version = 0.0.8
+version = 0.0.9
 author = Si Parker
 author_email = ayeaye@plogic.co.uk
 description = Execution engine for Aye-Aye ETL models
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/Aye-Aye-Dev/Fossa
 project_urls = 
@@ -19,15 +19,15 @@
 packages = find:
 python_requires = >=3.8
 package_dir = 
 	=lib
 install_requires = 
 	flask
 	gunicorn
-	ayeaye >= 0.0.55
+	ayeaye >= 0.0.56
 	pika
 	boto3
 include_package_data = True
 
 [options.packages.find]
 where = lib
 exclude = tests*
```

