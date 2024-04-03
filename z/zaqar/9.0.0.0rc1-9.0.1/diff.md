# Comparing `tmp/zaqar-9.0.0.0rc1.tar.gz` & `tmp/zaqar-9.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/zaqar-9.0.0.0rc1.tar", last modified: Wed Sep 25 09:15:44 2019, max compression
+gzip compressed data, was "dist/zaqar-9.0.1.tar", last modified: Mon Jun 15 09:53:07 2020, max compression
```

## Comparing `zaqar-9.0.0.0rc1.tar` & `zaqar-9.0.1.tar`

### file list

```diff
@@ -1,714 +1,701 @@
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-25 09:15:44.000000 zaqar-9.0.0.0rc1/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3975 2019-09-25 09:15:44.000000 zaqar-9.0.0.0rc1/PKG-INFO
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       93 2019-09-25 09:13:26.000000 zaqar-9.0.0.0rc1/bench-requirements.txt
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-25 09:15:44.000000 zaqar-9.0.0.0rc1/etc/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      144 2019-09-25 09:13:26.000000 zaqar-9.0.0.0rc1/etc/zaqar-benchmark.conf.sample
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      321 2019-09-25 09:13:26.000000 zaqar-9.0.0.0rc1/etc/README-policy.json.sample
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-25 09:15:44.000000 zaqar-9.0.0.0rc1/etc/oslo-config-generator/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      298 2019-09-25 09:13:26.000000 zaqar-9.0.0.0rc1/etc/oslo-config-generator/zaqar.conf
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      133 2019-09-25 09:13:26.000000 zaqar-9.0.0.0rc1/etc/uwsgi.conf
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       71 2019-09-25 09:13:26.000000 zaqar-9.0.0.0rc1/etc/zaqar-policy-generator.conf
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3015 2019-09-25 09:13:26.000000 zaqar-9.0.0.0rc1/etc/zaqar-benchmark-messages.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      908 2019-09-25 09:13:26.000000 zaqar-9.0.0.0rc1/etc/logging.conf.sample
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1030 2019-09-25 09:13:26.000000 zaqar-9.0.0.0rc1/setup.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10143 2019-09-25 09:13:26.000000 zaqar-9.0.0.0rc1/LICENSE
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       17 2019-09-25 09:13:26.000000 zaqar-9.0.0.0rc1/babel.cfg
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3284 2019-09-25 09:15:44.000000 zaqar-9.0.0.0rc1/setup.cfg
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-25 09:15:44.000000 zaqar-9.0.0.0rc1/doc/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       31 2019-09-25 09:13:26.000000 zaqar-9.0.0.0rc1/doc/README.md
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-25 09:15:44.000000 zaqar-9.0.0.0rc1/doc/source/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7940 2019-09-25 09:13:26.000000 zaqar-9.0.0.0rc1/doc/source/conf.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-25 09:15:44.000000 zaqar-9.0.0.0rc1/doc/source/user/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    11218 2019-09-25 09:13:26.000000 zaqar-9.0.0.0rc1/doc/source/user/getting_started.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3347 2019-09-25 09:13:26.000000 zaqar-9.0.0.0rc1/doc/source/user/send_request_api.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1541 2019-09-25 09:13:26.000000 zaqar-9.0.0.0rc1/doc/source/user/authentication_tokens.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      189 2019-09-25 09:13:26.000000 zaqar-9.0.0.0rc1/doc/source/user/index.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    12321 2019-09-25 09:13:26.000000 zaqar-9.0.0.0rc1/doc/source/user/headers_queue_api_working.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2760 2019-09-25 09:13:26.000000 zaqar-9.0.0.0rc1/doc/source/user/notification_delivery_policy.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3934 2019-09-25 09:13:26.000000 zaqar-9.0.0.0rc1/doc/source/index.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-25 09:15:44.000000 zaqar-9.0.0.0rc1/doc/source/cli/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       75 2019-09-25 09:13:26.000000 zaqar-9.0.0.0rc1/doc/source/cli/index.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1752 2019-09-25 09:13:26.000000 zaqar-9.0.0.0rc1/doc/source/cli/zaqar-status.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-25 09:15:44.000000 zaqar-9.0.0.0rc1/doc/source/admin/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6367 2019-09-25 09:13:26.000000 zaqar-9.0.0.0rc1/doc/source/admin/running_benchmark.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3835 2019-09-25 09:13:26.000000 zaqar-9.0.0.0rc1/doc/source/admin/CORS.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    12144 2019-09-25 09:13:26.000000 zaqar-9.0.0.0rc1/doc/source/admin/subscription_confirm.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      195 2019-09-25 09:13:26.000000 zaqar-9.0.0.0rc1/doc/source/admin/index.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3421 2019-09-25 09:13:26.000000 zaqar-9.0.0.0rc1/doc/source/admin/gmr.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8000 2019-09-25 09:13:26.000000 zaqar-9.0.0.0rc1/doc/source/admin/writing_pipeline_stages.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4557 2019-09-25 09:13:26.000000 zaqar-9.0.0.0rc1/doc/source/admin/OSprofiler.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-25 09:15:44.000000 zaqar-9.0.0.0rc1/doc/source/install/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    20158 2019-09-25 09:13:26.000000 zaqar-9.0.0.0rc1/doc/source/install/install-ubuntu.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1564 2019-09-25 09:13:26.000000 zaqar-9.0.0.0rc1/doc/source/install/index.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    20636 2019-09-25 09:13:26.000000 zaqar-9.0.0.0rc1/doc/source/install/install-rdo.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1161 2019-09-25 09:13:26.000000 zaqar-9.0.0.0rc1/doc/source/install/install.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2673 2019-09-25 09:13:26.000000 zaqar-9.0.0.0rc1/doc/source/install/get_started.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      239 2019-09-25 09:13:26.000000 zaqar-9.0.0.0rc1/doc/source/install/next-steps.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1321 2019-09-25 09:13:26.000000 zaqar-9.0.0.0rc1/doc/source/install/verify.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    20622 2019-09-25 09:13:26.000000 zaqar-9.0.0.0rc1/doc/source/install/install-obs.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-25 09:15:44.000000 zaqar-9.0.0.0rc1/doc/source/contributor/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8623 2019-09-25 09:13:26.000000 zaqar-9.0.0.0rc1/doc/source/contributor/welcome.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4934 2019-09-25 09:13:26.000000 zaqar-9.0.0.0rc1/doc/source/contributor/first_review.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8439 2019-09-25 09:13:26.000000 zaqar-9.0.0.0rc1/doc/source/contributor/development.environment.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3310 2019-09-25 09:13:26.000000 zaqar-9.0.0.0rc1/doc/source/contributor/test_suite.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6249 2019-09-25 09:13:26.000000 zaqar-9.0.0.0rc1/doc/source/contributor/project_info.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10773 2019-09-25 09:13:26.000000 zaqar-9.0.0.0rc1/doc/source/contributor/first_patch.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1803 2019-09-25 09:13:26.000000 zaqar-9.0.0.0rc1/doc/source/contributor/launchpad.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6258 2019-09-25 09:13:26.000000 zaqar-9.0.0.0rc1/doc/source/contributor/reviewer_guide.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5145 2019-09-25 09:13:26.000000 zaqar-9.0.0.0rc1/doc/source/contributor/running_tests.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      124 2019-09-25 09:13:26.000000 zaqar-9.0.0.0rc1/doc/source/contributor/transport.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1099 2019-09-25 09:13:26.000000 zaqar-9.0.0.0rc1/doc/source/contributor/index.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      490 2019-09-25 09:13:26.000000 zaqar-9.0.0.0rc1/doc/source/contributor/storage.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1409 2019-09-25 09:13:26.000000 zaqar-9.0.0.0rc1/doc/source/contributor/jenkins.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1159 2019-09-25 09:13:26.000000 zaqar-9.0.0.0rc1/doc/source/contributor/gerrit.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-25 09:15:44.000000 zaqar-9.0.0.0rc1/doc/source/contributor/images/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    77939 2019-09-25 09:13:26.000000 zaqar-9.0.0.0rc1/doc/source/contributor/images/zaqar_review_id.png
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-25 09:15:44.000000 zaqar-9.0.0.0rc1/doc/source/configuration/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6574 2019-09-25 09:13:26.000000 zaqar-9.0.0.0rc1/doc/source/configuration/configuring.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      387 2019-09-25 09:13:26.000000 zaqar-9.0.0.0rc1/doc/source/configuration/index.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      509 2019-09-25 09:13:26.000000 zaqar-9.0.0.0rc1/doc/source/configuration/sample-configuration.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      123 2019-09-25 09:13:26.000000 zaqar-9.0.0.0rc1/doc/source/configuration/zaqar.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3352 2019-09-25 09:13:26.000000 zaqar-9.0.0.0rc1/doc/source/glossary.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-25 09:15:44.000000 zaqar-9.0.0.0rc1/doc/source/_static/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2019-09-25 09:13:26.000000 zaqar-9.0.0.0rc1/doc/source/_static/.placeholder
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      514 2019-09-25 09:13:26.000000 zaqar-9.0.0.0rc1/doc/requirements.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      533 2019-09-25 09:13:26.000000 zaqar-9.0.0.0rc1/bindep.txt
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-25 09:15:44.000000 zaqar-9.0.0.0rc1/samples/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-25 09:15:44.000000 zaqar-9.0.0.0rc1/samples/java-api-for-websocket/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-25 09:15:44.000000 zaqar-9.0.0.0rc1/samples/java-api-for-websocket/receive_message/
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)     2141 2019-09-25 09:13:26.000000 zaqar-9.0.0.0rc1/samples/java-api-for-websocket/receive_message/SampleZaqarEndpoint.java
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)     1215 2019-09-25 09:13:26.000000 zaqar-9.0.0.0rc1/samples/java-api-for-websocket/receive_message/JsonDecoder.java
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-25 09:15:44.000000 zaqar-9.0.0.0rc1/samples/java-api-for-websocket/send_message/
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)     1783 2019-09-25 09:13:26.000000 zaqar-9.0.0.0rc1/samples/java-api-for-websocket/send_message/SampleZaqarEndpoint.java
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-25 09:15:44.000000 zaqar-9.0.0.0rc1/samples/html/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3009 2019-09-25 09:13:26.000000 zaqar-9.0.0.0rc1/samples/html/confirmation_web_service_sample.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4639 2019-09-25 09:13:26.000000 zaqar-9.0.0.0rc1/samples/html/unsubscriptionConfirmation.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5117 2019-09-25 09:13:26.000000 zaqar-9.0.0.0rc1/samples/html/subscriptionConfirmation.html
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-25 09:15:44.000000 zaqar-9.0.0.0rc1/samples/python-zaqarclient/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-25 09:15:44.000000 zaqar-9.0.0.0rc1/samples/python-zaqarclient/receive_message/
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)     1091 2019-09-25 09:13:26.000000 zaqar-9.0.0.0rc1/samples/python-zaqarclient/receive_message/zaqar_sample.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-25 09:15:44.000000 zaqar-9.0.0.0rc1/samples/python-zaqarclient/send_message/
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)     1031 2019-09-25 09:13:26.000000 zaqar-9.0.0.0rc1/samples/python-zaqarclient/send_message/zaqar_sample.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-25 09:15:44.000000 zaqar-9.0.0.0rc1/samples/zaqar/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7995 2019-09-25 09:13:26.000000 zaqar-9.0.0.0rc1/samples/zaqar/sendmail.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2491 2019-09-25 09:13:26.000000 zaqar-9.0.0.0rc1/samples/zaqar/subscriber_service_sample.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-25 09:15:44.000000 zaqar-9.0.0.0rc1/samples/jaxrs/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-25 09:15:44.000000 zaqar-9.0.0.0rc1/samples/jaxrs/receive_message/
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)     2017 2019-09-25 09:13:26.000000 zaqar-9.0.0.0rc1/samples/jaxrs/receive_message/SampleZaqarServlet.java
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-25 09:15:44.000000 zaqar-9.0.0.0rc1/samples/jaxrs/send_message/
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)     1987 2019-09-25 09:13:26.000000 zaqar-9.0.0.0rc1/samples/jaxrs/send_message/SampleZaqarServlet.java
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-25 09:15:44.000000 zaqar-9.0.0.0rc1/samples/nodejs/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-25 09:15:44.000000 zaqar-9.0.0.0rc1/samples/nodejs/receive_message/
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)     1283 2019-09-25 09:13:26.000000 zaqar-9.0.0.0rc1/samples/nodejs/receive_message/zaqar_sample.js
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-25 09:15:44.000000 zaqar-9.0.0.0rc1/samples/nodejs/send_message/
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)     1175 2019-09-25 09:13:26.000000 zaqar-9.0.0.0rc1/samples/nodejs/send_message/zaqar_sample.js
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-25 09:15:44.000000 zaqar-9.0.0.0rc1/samples/javascript/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-25 09:15:44.000000 zaqar-9.0.0.0rc1/samples/javascript/receive_message/
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)     1232 2019-09-25 09:13:26.000000 zaqar-9.0.0.0rc1/samples/javascript/receive_message/zaqar_sample.js
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    12471 2019-09-25 09:13:26.000000 zaqar-9.0.0.0rc1/samples/javascript/websocket.html
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-25 09:15:44.000000 zaqar-9.0.0.0rc1/samples/javascript/send_message/
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)     1137 2019-09-25 09:13:26.000000 zaqar-9.0.0.0rc1/samples/javascript/send_message/zaqar_sample.js
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      541 2019-09-25 09:13:26.000000 zaqar-9.0.0.0rc1/CONTRIBUTING.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4008 2019-09-25 09:13:26.000000 zaqar-9.0.0.0rc1/.zuul.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-25 09:15:44.000000 zaqar-9.0.0.0rc1/playbooks/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-25 09:15:44.000000 zaqar-9.0.0.0rc1/playbooks/legacy/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-25 09:15:44.000000 zaqar-9.0.0.0rc1/playbooks/legacy/grenade-devstack-zaqar-base/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2702 2019-09-25 09:13:26.000000 zaqar-9.0.0.0rc1/playbooks/legacy/grenade-devstack-zaqar-base/run.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      411 2019-09-25 09:13:26.000000 zaqar-9.0.0.0rc1/playbooks/legacy/grenade-devstack-zaqar-base/post.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-25 09:15:44.000000 zaqar-9.0.0.0rc1/playbooks/legacy/rally-dsvm-zaqar-zaqar/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8435 2019-09-25 09:13:26.000000 zaqar-9.0.0.0rc1/playbooks/legacy/rally-dsvm-zaqar-zaqar/run.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1207 2019-09-25 09:13:26.000000 zaqar-9.0.0.0rc1/playbooks/legacy/rally-dsvm-zaqar-zaqar/post.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-25 09:15:44.000000 zaqar-9.0.0.0rc1/playbooks/legacy/tempest-devstack-zaqar-base/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1984 2019-09-25 09:13:26.000000 zaqar-9.0.0.0rc1/playbooks/legacy/tempest-devstack-zaqar-base/run.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2409 2019-09-25 09:13:26.000000 zaqar-9.0.0.0rc1/playbooks/legacy/tempest-devstack-zaqar-base/post.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-25 09:15:44.000000 zaqar-9.0.0.0rc1/api-ref/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-25 09:15:44.000000 zaqar-9.0.0.0rc1/api-ref/source/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7392 2019-09-25 09:13:26.000000 zaqar-9.0.0.0rc1/api-ref/source/conf.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4293 2019-09-25 09:13:26.000000 zaqar-9.0.0.0rc1/api-ref/source/subscription.inc
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10035 2019-09-25 09:13:26.000000 zaqar-9.0.0.0rc1/api-ref/source/messages.inc
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1124 2019-09-25 09:13:26.000000 zaqar-9.0.0.0rc1/api-ref/source/versions.inc
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1635 2019-09-25 09:13:26.000000 zaqar-9.0.0.0rc1/api-ref/source/health.inc
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5367 2019-09-25 09:13:26.000000 zaqar-9.0.0.0rc1/api-ref/source/flavors.inc
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-25 09:15:44.000000 zaqar-9.0.0.0rc1/api-ref/source/samples/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      143 2019-09-25 09:13:26.000000 zaqar-9.0.0.0rc1/api-ref/source/samples/pool-update-request-new.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      130 2019-09-25 09:13:26.000000 zaqar-9.0.0.0rc1/api-ref/source/samples/subscription-create-request-mail.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      107 2019-09-25 09:13:26.000000 zaqar-9.0.0.0rc1/api-ref/source/samples/subscription-update-request.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       55 2019-09-25 09:13:26.000000 zaqar-9.0.0.0rc1/api-ref/source/samples/purge-queue-request.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       26 2019-09-25 09:13:26.000000 zaqar-9.0.0.0rc1/api-ref/source/samples/queue-update-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      172 2019-09-25 09:13:26.000000 zaqar-9.0.0.0rc1/api-ref/source/samples/subscription-show-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       36 2019-09-25 09:13:26.000000 zaqar-9.0.0.0rc1/api-ref/source/samples/claim_messages_request.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      211 2019-09-25 09:13:26.000000 zaqar-9.0.0.0rc1/api-ref/source/samples/flavor-show-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      224 2019-09-25 09:13:26.000000 zaqar-9.0.0.0rc1/api-ref/source/samples/flavor-show-response-new.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      498 2019-09-25 09:13:26.000000 zaqar-9.0.0.0rc1/api-ref/source/samples/pool-list-response-new.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       33 2019-09-25 09:13:26.000000 zaqar-9.0.0.0rc1/api-ref/source/samples/flavor-create-request.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       32 2019-09-25 09:13:26.000000 zaqar-9.0.0.0rc1/api-ref/source/samples/claim_update_request.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      996 2019-09-25 09:13:26.000000 zaqar-9.0.0.0rc1/api-ref/source/samples/messages-list-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      327 2019-09-25 09:13:26.000000 zaqar-9.0.0.0rc1/api-ref/source/samples/claim_query_response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      139 2019-09-25 09:13:26.000000 zaqar-9.0.0.0rc1/api-ref/source/samples/pool-create-request.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      156 2019-09-25 09:13:26.000000 zaqar-9.0.0.0rc1/api-ref/source/samples/pool-update-response-new.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      136 2019-09-25 09:13:26.000000 zaqar-9.0.0.0rc1/api-ref/source/samples/queue-pre-signed-request.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      139 2019-09-25 09:13:26.000000 zaqar-9.0.0.0rc1/api-ref/source/samples/pool-update-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      193 2019-09-25 09:13:26.000000 zaqar-9.0.0.0rc1/api-ref/source/samples/flavor-update-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       51 2019-09-25 09:13:26.000000 zaqar-9.0.0.0rc1/api-ref/source/samples/subscription-create-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      235 2019-09-25 09:13:26.000000 zaqar-9.0.0.0rc1/api-ref/source/samples/queue-show-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      141 2019-09-25 09:13:26.000000 zaqar-9.0.0.0rc1/api-ref/source/samples/pool-create-request-new.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      157 2019-09-25 09:13:26.000000 zaqar-9.0.0.0rc1/api-ref/source/samples/pool-show-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      517 2019-09-25 09:13:26.000000 zaqar-9.0.0.0rc1/api-ref/source/samples/subscriptions-list-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       45 2019-09-25 09:13:26.000000 zaqar-9.0.0.0rc1/api-ref/source/samples/flavor-create-request-new.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1404 2019-09-25 09:13:26.000000 zaqar-9.0.0.0rc1/api-ref/source/samples/health-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      496 2019-09-25 09:13:26.000000 zaqar-9.0.0.0rc1/api-ref/source/samples/pool-list-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      326 2019-09-25 09:13:26.000000 zaqar-9.0.0.0rc1/api-ref/source/samples/messages-post-request.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      378 2019-09-25 09:13:26.000000 zaqar-9.0.0.0rc1/api-ref/source/samples/messages-get-byids-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      319 2019-09-25 09:13:26.000000 zaqar-9.0.0.0rc1/api-ref/source/samples/messages-get-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      394 2019-09-25 09:13:26.000000 zaqar-9.0.0.0rc1/api-ref/source/samples/queue-pre-signed-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      373 2019-09-25 09:13:26.000000 zaqar-9.0.0.0rc1/api-ref/source/samples/queues-list-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      349 2019-09-25 09:13:26.000000 zaqar-9.0.0.0rc1/api-ref/source/samples/claim_messages_response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      286 2019-09-25 09:13:26.000000 zaqar-9.0.0.0rc1/api-ref/source/samples/queue-create-request.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1228 2019-09-25 09:13:26.000000 zaqar-9.0.0.0rc1/api-ref/source/samples/versions-list-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      141 2019-09-25 09:13:26.000000 zaqar-9.0.0.0rc1/api-ref/source/samples/pool-update-request.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      147 2019-09-25 09:13:26.000000 zaqar-9.0.0.0rc1/api-ref/source/samples/messages-post-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      102 2019-09-25 09:13:26.000000 zaqar-9.0.0.0rc1/api-ref/source/samples/queue-update-request.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       82 2019-09-25 09:13:26.000000 zaqar-9.0.0.0rc1/api-ref/source/samples/subscription-create-request-http.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      158 2019-09-25 09:13:26.000000 zaqar-9.0.0.0rc1/api-ref/source/samples/pool-show-response-new.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      205 2019-09-25 09:13:26.000000 zaqar-9.0.0.0rc1/api-ref/source/samples/flavor-update-response-new.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      480 2019-09-25 09:13:26.000000 zaqar-9.0.0.0rc1/api-ref/source/samples/flavor-list-response-new.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      305 2019-09-25 09:13:26.000000 zaqar-9.0.0.0rc1/api-ref/source/samples/messages-delete-bypop-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       33 2019-09-25 09:13:26.000000 zaqar-9.0.0.0rc1/api-ref/source/samples/flavor-update-request.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      454 2019-09-25 09:13:26.000000 zaqar-9.0.0.0rc1/api-ref/source/samples/flavor-list-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       45 2019-09-25 09:13:26.000000 zaqar-9.0.0.0rc1/api-ref/source/samples/flavor-update-request-new.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       92 2019-09-25 09:13:26.000000 zaqar-9.0.0.0rc1/api-ref/source/samples/queue-stats-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      904 2019-09-25 09:13:26.000000 zaqar-9.0.0.0rc1/api-ref/source/index.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8474 2019-09-25 09:13:26.000000 zaqar-9.0.0.0rc1/api-ref/source/queues.inc
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1704 2019-09-25 09:13:26.000000 zaqar-9.0.0.0rc1/api-ref/source/status.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5326 2019-09-25 09:13:26.000000 zaqar-9.0.0.0rc1/api-ref/source/pools.inc
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5946 2019-09-25 09:13:26.000000 zaqar-9.0.0.0rc1/api-ref/source/claims.inc
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    16855 2019-09-25 09:13:26.000000 zaqar-9.0.0.0rc1/api-ref/source/parameters.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-25 09:15:44.000000 zaqar-9.0.0.0rc1/rally-jobs/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-25 09:15:44.000000 zaqar-9.0.0.0rc1/rally-jobs/extra/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      185 2019-09-25 09:13:26.000000 zaqar-9.0.0.0rc1/rally-jobs/extra/README.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-25 09:15:44.000000 zaqar-9.0.0.0rc1/rally-jobs/plugins/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2019-09-25 09:13:26.000000 zaqar-9.0.0.0rc1/rally-jobs/plugins/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      403 2019-09-25 09:13:26.000000 zaqar-9.0.0.0rc1/rally-jobs/plugins/README.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      305 2019-09-25 09:13:26.000000 zaqar-9.0.0.0rc1/rally-jobs/zaqar-zaqar.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      882 2019-09-25 09:13:26.000000 zaqar-9.0.0.0rc1/rally-jobs/README.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      364 2019-09-25 09:13:26.000000 zaqar-9.0.0.0rc1/AUTHORS.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-25 09:15:44.000000 zaqar-9.0.0.0rc1/releasenotes/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-25 09:15:44.000000 zaqar-9.0.0.0rc1/releasenotes/notes/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      474 2019-09-25 09:13:26.000000 zaqar-9.0.0.0rc1/releasenotes/notes/remove-format-contraint-of-client-id-ab787960df6e1606.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      282 2019-09-25 09:13:26.000000 zaqar-9.0.0.0rc1/releasenotes/notes/sql_init-c9b3883241631f24.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      245 2019-09-25 09:13:26.000000 zaqar-9.0.0.0rc1/releasenotes/notes/fix_auth_issue_for_root_path-b15e1c4e92e4e8b1.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      238 2019-09-25 09:13:26.000000 zaqar-9.0.0.0rc1/releasenotes/notes/fix-detailed-queue-without-reserved-metadata-b53857ed9821fe76.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      278 2019-09-25 09:13:26.000000 zaqar-9.0.0.0rc1/releasenotes/notes/deprecate-v11-976cccc1b56a28e7.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      398 2019-09-25 09:13:26.000000 zaqar-9.0.0.0rc1/releasenotes/notes/support-turnoff-deprecated-versions-44656aeb8ebb8881.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      225 2019-09-25 09:13:26.000000 zaqar-9.0.0.0rc1/releasenotes/notes/remove-pool-group-totally-062ecfccd90a6725.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      431 2019-09-25 09:13:26.000000 zaqar-9.0.0.0rc1/releasenotes/notes/introduce-topic-resource-9b40674cac06bdc2.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      196 2019-09-25 09:13:26.000000 zaqar-9.0.0.0rc1/releasenotes/notes/queue-filter-support-b704a1c27f7473b9.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      244 2019-09-25 09:13:26.000000 zaqar-9.0.0.0rc1/releasenotes/notes/return_reserved_metdata_for_dead_letter_queue-da160301f6d8cfa4.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      328 2019-09-25 09:13:26.000000 zaqar-9.0.0.0rc1/releasenotes/notes/email-notification-by-internal-tool-08910ab2247c3864.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      366 2019-09-25 09:13:26.000000 zaqar-9.0.0.0rc1/releasenotes/notes/lazy-queues-in-subscriptions-6bade4a1b8eca3e5.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      462 2019-09-25 09:13:26.000000 zaqar-9.0.0.0rc1/releasenotes/notes/zaqar-status-upgrade-check-framework-09caa1f741f6119d.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      484 2019-09-25 09:13:26.000000 zaqar-9.0.0.0rc1/releasenotes/notes/webhook_subscription_confirmation-883cb7f325885ef0.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      326 2019-09-25 09:13:26.000000 zaqar-9.0.0.0rc1/releasenotes/notes/user_ipv6_sockets-1e1b436de6b81ae3.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      269 2019-09-25 09:13:26.000000 zaqar-9.0.0.0rc1/releasenotes/notes/Integrate-OSprofiler-with-zaqar-59d0dc3d0326947d.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      573 2019-09-25 09:13:26.000000 zaqar-9.0.0.0rc1/releasenotes/notes/add-a-notifier-using-trust-271d9cd1d2b4cdeb.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      297 2019-09-25 09:13:26.000000 zaqar-9.0.0.0rc1/releasenotes/notes/introduce-guru-to-zaqar-ac7b51c764503829.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      211 2019-09-25 09:13:26.000000 zaqar-9.0.0.0rc1/releasenotes/notes/purge-queue-6788a249ee59d55a.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      164 2019-09-25 09:13:26.000000 zaqar-9.0.0.0rc1/releasenotes/notes/remove_pool_group_from_zaqar-f8eafeed21779959.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       84 2019-09-25 09:13:26.000000 zaqar-9.0.0.0rc1/releasenotes/notes/support-dot-in-queue-name-bd2b3d523f55451f.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      250 2019-09-25 09:13:26.000000 zaqar-9.0.0.0rc1/releasenotes/notes/support-notification-delivery-policy-fbc94083b4e6b8d0.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      275 2019-09-25 09:13:26.000000 zaqar-9.0.0.0rc1/releasenotes/notes/support_delayed_queues-1babcaa3f056a39d.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2019-09-25 09:13:26.000000 zaqar-9.0.0.0rc1/releasenotes/notes/.gitignore
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      213 2019-09-25 09:13:26.000000 zaqar-9.0.0.0rc1/releasenotes/notes/fix_subscription_limit-c3cdc9385825285a.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      333 2019-09-25 09:13:26.000000 zaqar-9.0.0.0rc1/releasenotes/notes/support-more-backoff-functions-41e02a5977341576.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      302 2019-09-25 09:13:26.000000 zaqar-9.0.0.0rc1/releasenotes/notes/add-swift-backend-4eb9b43913f39d18.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      479 2019-09-25 09:13:26.000000 zaqar-9.0.0.0rc1/releasenotes/notes/support_md5_of_body-84c1cdc6809b6417.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      294 2019-09-25 09:13:26.000000 zaqar-9.0.0.0rc1/releasenotes/notes/support_password_configure_for_redis_connection-6f169db73ca80416.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      384 2019-09-25 09:13:26.000000 zaqar-9.0.0.0rc1/releasenotes/notes/support_dead_letter_queue-c8b7303319e7f920.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      401 2019-09-25 09:13:26.000000 zaqar-9.0.0.0rc1/releasenotes/notes/show_default_attributes_for_queue-3d87333752484c87.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      226 2019-09-25 09:13:26.000000 zaqar-9.0.0.0rc1/releasenotes/notes/delete_messages_with_claim_ids-64bb8105de3768b1.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      318 2019-09-25 09:13:26.000000 zaqar-9.0.0.0rc1/releasenotes/notes/allow-configuration-of-websocket-notification-fa542fbf761378d3.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      872 2019-09-25 09:13:26.000000 zaqar-9.0.0.0rc1/releasenotes/notes/subscription-confirmation-support-email-0c2a56cfedc5d1e2.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       79 2019-09-25 09:13:26.000000 zaqar-9.0.0.0rc1/releasenotes/notes/sqlalchemy-migration-6b4eaebb6e02a449.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      229 2019-09-25 09:13:26.000000 zaqar-9.0.0.0rc1/releasenotes/notes/support-redis-as-management-storage-backend-a205e3c4c4d01584.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      231 2019-09-25 09:13:26.000000 zaqar-9.0.0.0rc1/releasenotes/notes/remove-pool-group-00f2e69682c48131.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      269 2019-09-25 09:13:26.000000 zaqar-9.0.0.0rc1/releasenotes/notes/configuration-refactor-0ff219ac59c96347.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       75 2019-09-25 09:13:26.000000 zaqar-9.0.0.0rc1/releasenotes/notes/support-cors-af8349382a44aa0d.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-25 09:15:44.000000 zaqar-9.0.0.0rc1/releasenotes/source/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      154 2019-09-25 09:13:26.000000 zaqar-9.0.0.0rc1/releasenotes/source/newton.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8921 2019-09-25 09:13:26.000000 zaqar-9.0.0.0rc1/releasenotes/source/conf.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      112 2019-09-25 09:13:26.000000 zaqar-9.0.0.0rc1/releasenotes/source/unreleased.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      154 2019-09-25 09:13:26.000000 zaqar-9.0.0.0rc1/releasenotes/source/mitaka.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      188 2019-09-25 09:13:26.000000 zaqar-9.0.0.0rc1/releasenotes/source/index.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      152 2019-09-25 09:13:26.000000 zaqar-9.0.0.0rc1/releasenotes/source/ocata.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-25 09:15:44.000000 zaqar-9.0.0.0rc1/releasenotes/source/locale/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-25 09:15:44.000000 zaqar-9.0.0.0rc1/releasenotes/source/locale/en_GB/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-25 09:15:44.000000 zaqar-9.0.0.0rc1/releasenotes/source/locale/en_GB/LC_MESSAGES/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    23445 2019-09-25 09:13:26.000000 zaqar-9.0.0.0rc1/releasenotes/source/locale/en_GB/LC_MESSAGES/releasenotes.po
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-25 09:15:44.000000 zaqar-9.0.0.0rc1/releasenotes/source/locale/id/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-25 09:15:44.000000 zaqar-9.0.0.0rc1/releasenotes/source/locale/id/LC_MESSAGES/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    24457 2019-09-25 09:13:26.000000 zaqar-9.0.0.0rc1/releasenotes/source/locale/id/LC_MESSAGES/releasenotes.po
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-25 09:15:44.000000 zaqar-9.0.0.0rc1/releasenotes/source/locale/de/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-25 09:15:44.000000 zaqar-9.0.0.0rc1/releasenotes/source/locale/de/LC_MESSAGES/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2034 2019-09-25 09:13:26.000000 zaqar-9.0.0.0rc1/releasenotes/source/locale/de/LC_MESSAGES/releasenotes.po
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-25 09:15:44.000000 zaqar-9.0.0.0rc1/releasenotes/source/locale/fr/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-25 09:15:44.000000 zaqar-9.0.0.0rc1/releasenotes/source/locale/fr/LC_MESSAGES/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1238 2019-09-25 09:13:26.000000 zaqar-9.0.0.0rc1/releasenotes/source/locale/fr/LC_MESSAGES/releasenotes.po
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-25 09:15:44.000000 zaqar-9.0.0.0rc1/releasenotes/source/_templates/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2019-09-25 09:13:26.000000 zaqar-9.0.0.0rc1/releasenotes/source/_templates/.gitignore
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      146 2019-09-25 09:13:26.000000 zaqar-9.0.0.0rc1/releasenotes/source/liberty.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      147 2019-09-25 09:13:26.000000 zaqar-9.0.0.0rc1/releasenotes/source/queens.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      145 2019-09-25 09:13:26.000000 zaqar-9.0.0.0rc1/releasenotes/source/rocky.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      143 2019-09-25 09:13:26.000000 zaqar-9.0.0.0rc1/releasenotes/source/pike.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      145 2019-09-25 09:13:26.000000 zaqar-9.0.0.0rc1/releasenotes/source/stein.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-25 09:15:44.000000 zaqar-9.0.0.0rc1/releasenotes/source/_static/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2019-09-25 09:13:26.000000 zaqar-9.0.0.0rc1/releasenotes/source/_static/.gitignore
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-25 09:15:44.000000 zaqar-9.0.0.0rc1/devstack/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-25 09:15:44.000000 zaqar-9.0.0.0rc1/devstack/upgrade/
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)      539 2019-09-25 09:13:26.000000 zaqar-9.0.0.0rc1/devstack/upgrade/shutdown.sh
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)     1400 2019-09-25 09:13:26.000000 zaqar-9.0.0.0rc1/devstack/upgrade/resource.sh
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)     3381 2019-09-25 09:13:26.000000 zaqar-9.0.0.0rc1/devstack/upgrade/upgrade.sh
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      810 2019-09-25 09:13:26.000000 zaqar-9.0.0.0rc1/devstack/upgrade/settings
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)    11746 2019-09-25 09:13:26.000000 zaqar-9.0.0.0rc1/devstack/plugin.sh
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1811 2019-09-25 09:13:26.000000 zaqar-9.0.0.0rc1/devstack/settings
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      619 2019-09-25 09:13:26.000000 zaqar-9.0.0.0rc1/devstack/README.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-25 09:15:44.000000 zaqar-9.0.0.0rc1/devstack/gate/
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)     1550 2019-09-25 09:13:26.000000 zaqar-9.0.0.0rc1/devstack/gate/post_test_hook.sh
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)     2147 2019-09-25 09:13:26.000000 zaqar-9.0.0.0rc1/devstack/gate/gate_hook.sh
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8446 2019-09-25 09:15:43.000000 zaqar-9.0.0.0rc1/AUTHORS
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3369 2019-09-25 09:13:26.000000 zaqar-9.0.0.0rc1/tox.ini
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-25 09:15:44.000000 zaqar-9.0.0.0rc1/zaqar/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-25 09:15:44.000000 zaqar-9.0.0.0rc1/zaqar/notification/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-25 09:15:44.000000 zaqar-9.0.0.0rc1/zaqar/notification/tasks/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6916 2019-09-25 09:13:26.000000 zaqar-9.0.0.0rc1/zaqar/notification/tasks/webhook.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6137 2019-09-25 09:13:26.000000 zaqar-9.0.0.0rc1/zaqar/notification/tasks/mailto.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2019-09-25 09:13:26.000000 zaqar-9.0.0.0rc1/zaqar/notification/tasks/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2272 2019-09-25 09:13:26.000000 zaqar-9.0.0.0rc1/zaqar/notification/tasks/trust.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2019-09-25 09:13:26.000000 zaqar-9.0.0.0rc1/zaqar/notification/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7190 2019-09-25 09:13:26.000000 zaqar-9.0.0.0rc1/zaqar/notification/notifier.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-25 09:15:44.000000 zaqar-9.0.0.0rc1/zaqar/bench/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2555 2019-09-25 09:13:26.000000 zaqar-9.0.0.0rc1/zaqar/bench/config.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4734 2019-09-25 09:13:26.000000 zaqar-9.0.0.0rc1/zaqar/bench/helpers.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3017 2019-09-25 09:13:26.000000 zaqar-9.0.0.0rc1/zaqar/bench/conductor.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6154 2019-09-25 09:13:26.000000 zaqar-9.0.0.0rc1/zaqar/bench/consumer.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5463 2019-09-25 09:13:26.000000 zaqar-9.0.0.0rc1/zaqar/bench/producer.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2019-09-25 09:13:26.000000 zaqar-9.0.0.0rc1/zaqar/bench/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4922 2019-09-25 09:13:26.000000 zaqar-9.0.0.0rc1/zaqar/bench/observer.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-25 09:15:44.000000 zaqar-9.0.0.0rc1/zaqar/common/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      798 2019-09-25 09:13:26.000000 zaqar-9.0.0.0rc1/zaqar/common/cache.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3976 2019-09-25 09:13:26.000000 zaqar-9.0.0.0rc1/zaqar/common/pipeline.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      960 2019-09-25 09:13:26.000000 zaqar-9.0.0.0rc1/zaqar/common/errors.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4143 2019-09-25 09:13:26.000000 zaqar-9.0.0.0rc1/zaqar/common/urls.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      763 2019-09-25 09:13:26.000000 zaqar-9.0.0.0rc1/zaqar/common/access.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3160 2019-09-25 09:13:26.000000 zaqar-9.0.0.0rc1/zaqar/common/auth.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      638 2019-09-25 09:13:26.000000 zaqar-9.0.0.0rc1/zaqar/common/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-25 09:15:44.000000 zaqar-9.0.0.0rc1/zaqar/common/api/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1254 2019-09-25 09:13:26.000000 zaqar-9.0.0.0rc1/zaqar/common/api/errors.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2019-09-25 09:13:26.000000 zaqar-9.0.0.0rc1/zaqar/common/api/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1431 2019-09-25 09:13:26.000000 zaqar-9.0.0.0rc1/zaqar/common/api/response.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2336 2019-09-25 09:13:26.000000 zaqar-9.0.0.0rc1/zaqar/common/api/api.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-25 09:15:44.000000 zaqar-9.0.0.0rc1/zaqar/common/api/schemas/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2102 2019-09-25 09:13:26.000000 zaqar-9.0.0.0rc1/zaqar/common/api/schemas/pools.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-25 09:15:44.000000 zaqar-9.0.0.0rc1/zaqar/common/api/schemas/v1_1/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2019-09-25 09:13:26.000000 zaqar-9.0.0.0rc1/zaqar/common/api/schemas/v1_1/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1327 2019-09-25 09:13:26.000000 zaqar-9.0.0.0rc1/zaqar/common/api/schemas/v1_1/flavors.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2019-09-25 09:13:26.000000 zaqar-9.0.0.0rc1/zaqar/common/api/schemas/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1647 2019-09-25 09:13:26.000000 zaqar-9.0.0.0rc1/zaqar/common/api/schemas/flavors.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1630 2019-09-25 09:13:26.000000 zaqar-9.0.0.0rc1/zaqar/common/api/request.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7356 2019-09-25 09:13:26.000000 zaqar-9.0.0.0rc1/zaqar/common/api/utils.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1481 2019-09-25 09:13:26.000000 zaqar-9.0.0.0rc1/zaqar/common/cli.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-25 09:15:44.000000 zaqar-9.0.0.0rc1/zaqar/common/storage/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2019-09-25 09:13:26.000000 zaqar-9.0.0.0rc1/zaqar/common/storage/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1779 2019-09-25 09:13:26.000000 zaqar-9.0.0.0rc1/zaqar/common/storage/select.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-25 09:15:44.000000 zaqar-9.0.0.0rc1/zaqar/common/transport/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2019-09-25 09:13:26.000000 zaqar-9.0.0.0rc1/zaqar/common/transport/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-25 09:15:44.000000 zaqar-9.0.0.0rc1/zaqar/common/transport/wsgi/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    11697 2019-09-25 09:13:26.000000 zaqar-9.0.0.0rc1/zaqar/common/transport/wsgi/helpers.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2019-09-25 09:13:26.000000 zaqar-9.0.0.0rc1/zaqar/common/transport/wsgi/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2350 2019-09-25 09:13:26.000000 zaqar-9.0.0.0rc1/zaqar/common/consts.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-25 09:15:44.000000 zaqar-9.0.0.0rc1/zaqar/common/policies/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2109 2019-09-25 09:13:26.000000 zaqar-9.0.0.0rc1/zaqar/common/policies/pools.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2060 2019-09-25 09:13:26.000000 zaqar-9.0.0.0rc1/zaqar/common/policies/claims.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3175 2019-09-25 09:13:26.000000 zaqar-9.0.0.0rc1/zaqar/common/policies/queues.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2367 2019-09-25 09:13:26.000000 zaqar-9.0.0.0rc1/zaqar/common/policies/messages.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1305 2019-09-25 09:13:26.000000 zaqar-9.0.0.0rc1/zaqar/common/policies/health.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1260 2019-09-25 09:13:26.000000 zaqar-9.0.0.0rc1/zaqar/common/policies/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      930 2019-09-25 09:13:26.000000 zaqar-9.0.0.0rc1/zaqar/common/policies/base.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2787 2019-09-25 09:13:26.000000 zaqar-9.0.0.0rc1/zaqar/common/policies/topics.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2837 2019-09-25 09:13:26.000000 zaqar-9.0.0.0rc1/zaqar/common/policies/subscription.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2172 2019-09-25 09:13:26.000000 zaqar-9.0.0.0rc1/zaqar/common/policies/flavors.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7272 2019-09-25 09:13:26.000000 zaqar-9.0.0.0rc1/zaqar/common/decorators.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2033 2019-09-25 09:13:26.000000 zaqar-9.0.0.0rc1/zaqar/common/utils.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-25 09:15:44.000000 zaqar-9.0.0.0rc1/zaqar/conf/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4969 2019-09-25 09:13:26.000000 zaqar-9.0.0.0rc1/zaqar/conf/drivers_management_store_mongodb.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1494 2019-09-25 09:13:26.000000 zaqar-9.0.0.0rc1/zaqar/conf/drivers_transport_websocket.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5749 2019-09-25 09:13:26.000000 zaqar-9.0.0.0rc1/zaqar/conf/transport.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      959 2019-09-25 09:13:26.000000 zaqar-9.0.0.0rc1/zaqar/conf/pooling_catalog.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1319 2019-09-25 09:13:26.000000 zaqar-9.0.0.0rc1/zaqar/conf/profiler.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1211 2019-09-25 09:13:26.000000 zaqar-9.0.0.0rc1/zaqar/conf/drivers.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2123 2019-09-25 09:13:26.000000 zaqar-9.0.0.0rc1/zaqar/conf/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2031 2019-09-25 09:13:26.000000 zaqar-9.0.0.0rc1/zaqar/conf/default.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1014 2019-09-25 09:13:26.000000 zaqar-9.0.0.0rc1/zaqar/conf/drivers_management_store_sqlalchemy.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3280 2019-09-25 09:13:26.000000 zaqar-9.0.0.0rc1/zaqar/conf/drivers_message_store_redis.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3283 2019-09-25 09:13:26.000000 zaqar-9.0.0.0rc1/zaqar/conf/drivers_management_store_redis.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4557 2019-09-25 09:13:26.000000 zaqar-9.0.0.0rc1/zaqar/conf/notification.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      879 2019-09-25 09:13:26.000000 zaqar-9.0.0.0rc1/zaqar/conf/signed_url.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1029 2019-09-25 09:13:26.000000 zaqar-9.0.0.0rc1/zaqar/conf/drivers_transport_wsgi.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2136 2019-09-25 09:13:26.000000 zaqar-9.0.0.0rc1/zaqar/conf/storage.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1901 2019-09-25 09:13:26.000000 zaqar-9.0.0.0rc1/zaqar/conf/drivers_message_store_swift.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5533 2019-09-25 09:13:26.000000 zaqar-9.0.0.0rc1/zaqar/conf/drivers_message_store_mongodb.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3623 2019-09-25 09:13:26.000000 zaqar-9.0.0.0rc1/zaqar/conf/opts.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2050 2019-09-25 09:13:27.000000 zaqar-9.0.0.0rc1/zaqar/version.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      743 2019-09-25 09:13:26.000000 zaqar-9.0.0.0rc1/zaqar/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-25 09:15:44.000000 zaqar-9.0.0.0rc1/zaqar/api/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-25 09:15:44.000000 zaqar-9.0.0.0rc1/zaqar/api/v1/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2019-09-25 09:13:26.000000 zaqar-9.0.0.0rc1/zaqar/api/v1/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    11400 2019-09-25 09:13:26.000000 zaqar-9.0.0.0rc1/zaqar/api/v1/response.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    13196 2019-09-25 09:13:26.000000 zaqar-9.0.0.0rc1/zaqar/api/v1/request.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-25 09:15:44.000000 zaqar-9.0.0.0rc1/zaqar/api/v1_1/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2019-09-25 09:13:26.000000 zaqar-9.0.0.0rc1/zaqar/api/v1_1/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    15593 2019-09-25 09:13:26.000000 zaqar-9.0.0.0rc1/zaqar/api/v1_1/response.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8354 2019-09-25 09:13:26.000000 zaqar-9.0.0.0rc1/zaqar/api/v1_1/request.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2019-09-25 09:13:26.000000 zaqar-9.0.0.0rc1/zaqar/api/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4843 2019-09-25 09:13:26.000000 zaqar-9.0.0.0rc1/zaqar/api/handler.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-25 09:15:44.000000 zaqar-9.0.0.0rc1/zaqar/api/v2/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    37805 2019-09-25 09:13:26.000000 zaqar-9.0.0.0rc1/zaqar/api/v2/endpoints.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2019-09-25 09:13:26.000000 zaqar-9.0.0.0rc1/zaqar/api/v2/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    15561 2019-09-25 09:13:26.000000 zaqar-9.0.0.0rc1/zaqar/api/v2/response.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4417 2019-09-25 09:13:26.000000 zaqar-9.0.0.0rc1/zaqar/api/v2/request.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-25 09:15:44.000000 zaqar-9.0.0.0rc1/zaqar/storage/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    33867 2019-09-25 09:13:26.000000 zaqar-9.0.0.0rc1/zaqar/storage/pooling.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-25 09:15:44.000000 zaqar-9.0.0.0rc1/zaqar/storage/redis/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    11283 2019-09-25 09:13:26.000000 zaqar-9.0.0.0rc1/zaqar/storage/redis/subscriptions.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9651 2019-09-25 09:13:26.000000 zaqar-9.0.0.0rc1/zaqar/storage/redis/pools.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    18770 2019-09-25 09:13:26.000000 zaqar-9.0.0.0rc1/zaqar/storage/redis/claims.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6515 2019-09-25 09:13:26.000000 zaqar-9.0.0.0rc1/zaqar/storage/redis/queues.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    11783 2019-09-25 09:13:26.000000 zaqar-9.0.0.0rc1/zaqar/storage/redis/driver.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    24333 2019-09-25 09:13:26.000000 zaqar-9.0.0.0rc1/zaqar/storage/redis/messages.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-25 09:15:44.000000 zaqar-9.0.0.0rc1/zaqar/storage/redis/scripts/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3451 2019-09-25 09:13:26.000000 zaqar-9.0.0.0rc1/zaqar/storage/redis/scripts/claim_messages.lua
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1104 2019-09-25 09:13:26.000000 zaqar-9.0.0.0rc1/zaqar/storage/redis/scripts/index_messages.lua
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1990 2019-09-25 09:13:26.000000 zaqar-9.0.0.0rc1/zaqar/storage/redis/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1198 2019-09-25 09:13:26.000000 zaqar-9.0.0.0rc1/zaqar/storage/redis/controllers.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6517 2019-09-25 09:13:26.000000 zaqar-9.0.0.0rc1/zaqar/storage/redis/flavors.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8964 2019-09-25 09:13:26.000000 zaqar-9.0.0.0rc1/zaqar/storage/redis/catalogue.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1181 2019-09-25 09:13:26.000000 zaqar-9.0.0.0rc1/zaqar/storage/redis/scripting.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10108 2019-09-25 09:13:26.000000 zaqar-9.0.0.0rc1/zaqar/storage/redis/models.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    12597 2019-09-25 09:13:26.000000 zaqar-9.0.0.0rc1/zaqar/storage/redis/utils.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-25 09:15:44.000000 zaqar-9.0.0.0rc1/zaqar/storage/mongodb/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7417 2019-09-25 09:13:26.000000 zaqar-9.0.0.0rc1/zaqar/storage/mongodb/subscriptions.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6198 2019-09-25 09:13:26.000000 zaqar-9.0.0.0rc1/zaqar/storage/mongodb/pools.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    14129 2019-09-25 09:13:26.000000 zaqar-9.0.0.0rc1/zaqar/storage/mongodb/claims.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10656 2019-09-25 09:13:26.000000 zaqar-9.0.0.0rc1/zaqar/storage/mongodb/queues.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    12091 2019-09-25 09:13:26.000000 zaqar-9.0.0.0rc1/zaqar/storage/mongodb/driver.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    42517 2019-09-25 09:13:26.000000 zaqar-9.0.0.0rc1/zaqar/storage/mongodb/messages.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2023 2019-09-25 09:13:26.000000 zaqar-9.0.0.0rc1/zaqar/storage/mongodb/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1625 2019-09-25 09:13:26.000000 zaqar-9.0.0.0rc1/zaqar/storage/mongodb/controllers.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    38641 2019-09-25 09:13:26.000000 zaqar-9.0.0.0rc1/zaqar/storage/mongodb/topic_messages.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10047 2019-09-25 09:13:26.000000 zaqar-9.0.0.0rc1/zaqar/storage/mongodb/topics.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4660 2019-09-25 09:13:26.000000 zaqar-9.0.0.0rc1/zaqar/storage/mongodb/flavors.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3285 2019-09-25 09:13:26.000000 zaqar-9.0.0.0rc1/zaqar/storage/mongodb/catalogue.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10803 2019-09-25 09:13:26.000000 zaqar-9.0.0.0rc1/zaqar/storage/mongodb/utils.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6494 2019-09-25 09:13:26.000000 zaqar-9.0.0.0rc1/zaqar/storage/pipeline.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-25 09:15:44.000000 zaqar-9.0.0.0rc1/zaqar/storage/sqlalchemy/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5509 2019-09-25 09:13:26.000000 zaqar-9.0.0.0rc1/zaqar/storage/sqlalchemy/pools.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4299 2019-09-25 09:13:26.000000 zaqar-9.0.0.0rc1/zaqar/storage/sqlalchemy/queues.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4314 2019-09-25 09:13:26.000000 zaqar-9.0.0.0rc1/zaqar/storage/sqlalchemy/driver.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      713 2019-09-25 09:13:26.000000 zaqar-9.0.0.0rc1/zaqar/storage/sqlalchemy/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      986 2019-09-25 09:13:26.000000 zaqar-9.0.0.0rc1/zaqar/storage/sqlalchemy/controllers.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-25 09:15:44.000000 zaqar-9.0.0.0rc1/zaqar/storage/sqlalchemy/migration/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2019-09-25 09:13:26.000000 zaqar-9.0.0.0rc1/zaqar/storage/sqlalchemy/migration/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3874 2019-09-25 09:13:26.000000 zaqar-9.0.0.0rc1/zaqar/storage/sqlalchemy/migration/cli.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-25 09:15:44.000000 zaqar-9.0.0.0rc1/zaqar/storage/sqlalchemy/migration/alembic_migrations/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2493 2019-09-25 09:13:26.000000 zaqar-9.0.0.0rc1/zaqar/storage/sqlalchemy/migration/alembic_migrations/README.md
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      952 2019-09-25 09:13:26.000000 zaqar-9.0.0.0rc1/zaqar/storage/sqlalchemy/migration/alembic_migrations/script.py.mako
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-25 09:15:44.000000 zaqar-9.0.0.0rc1/zaqar/storage/sqlalchemy/migration/alembic_migrations/versions/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2725 2019-09-25 09:13:26.000000 zaqar-9.0.0.0rc1/zaqar/storage/sqlalchemy/migration/alembic_migrations/versions/001_liberty.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      785 2019-09-25 09:13:26.000000 zaqar-9.0.0.0rc1/zaqar/storage/sqlalchemy/migration/alembic_migrations/versions/003_placeholder.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      785 2019-09-25 09:13:26.000000 zaqar-9.0.0.0rc1/zaqar/storage/sqlalchemy/migration/alembic_migrations/versions/004_placeholder.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      785 2019-09-25 09:13:26.000000 zaqar-9.0.0.0rc1/zaqar/storage/sqlalchemy/migration/alembic_migrations/versions/002_placeholder.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1579 2019-09-25 09:13:26.000000 zaqar-9.0.0.0rc1/zaqar/storage/sqlalchemy/migration/alembic_migrations/versions/007_stein.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      785 2019-09-25 09:13:26.000000 zaqar-9.0.0.0rc1/zaqar/storage/sqlalchemy/migration/alembic_migrations/versions/005_placeholder.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1200 2019-09-25 09:13:26.000000 zaqar-9.0.0.0rc1/zaqar/storage/sqlalchemy/migration/alembic_migrations/versions/006_queens.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2747 2019-09-25 09:13:26.000000 zaqar-9.0.0.0rc1/zaqar/storage/sqlalchemy/migration/alembic_migrations/env.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      975 2019-09-25 09:13:26.000000 zaqar-9.0.0.0rc1/zaqar/storage/sqlalchemy/migration/alembic.ini
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2182 2019-09-25 09:13:26.000000 zaqar-9.0.0.0rc1/zaqar/storage/sqlalchemy/tables.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4684 2019-09-25 09:13:26.000000 zaqar-9.0.0.0rc1/zaqar/storage/sqlalchemy/flavors.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3146 2019-09-25 09:13:26.000000 zaqar-9.0.0.0rc1/zaqar/storage/sqlalchemy/catalogue.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3722 2019-09-25 09:13:26.000000 zaqar-9.0.0.0rc1/zaqar/storage/sqlalchemy/utils.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6831 2019-09-25 09:13:26.000000 zaqar-9.0.0.0rc1/zaqar/storage/errors.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1625 2019-09-25 09:13:26.000000 zaqar-9.0.0.0rc1/zaqar/storage/configuration.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1360 2019-09-25 09:13:26.000000 zaqar-9.0.0.0rc1/zaqar/storage/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    40104 2019-09-25 09:13:26.000000 zaqar-9.0.0.0rc1/zaqar/storage/base.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-25 09:15:44.000000 zaqar-9.0.0.0rc1/zaqar/storage/swift/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7064 2019-09-25 09:13:26.000000 zaqar-9.0.0.0rc1/zaqar/storage/swift/subscriptions.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9911 2019-09-25 09:13:26.000000 zaqar-9.0.0.0rc1/zaqar/storage/swift/claims.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4868 2019-09-25 09:13:26.000000 zaqar-9.0.0.0rc1/zaqar/storage/swift/driver.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    18564 2019-09-25 09:13:26.000000 zaqar-9.0.0.0rc1/zaqar/storage/swift/messages.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2019-09-25 09:13:26.000000 zaqar-9.0.0.0rc1/zaqar/storage/swift/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      824 2019-09-25 09:13:26.000000 zaqar-9.0.0.0rc1/zaqar/storage/swift/controllers.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5169 2019-09-25 09:13:26.000000 zaqar-9.0.0.0rc1/zaqar/storage/swift/utils.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8105 2019-09-25 09:13:26.000000 zaqar-9.0.0.0rc1/zaqar/storage/utils.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-25 09:15:44.000000 zaqar-9.0.0.0rc1/zaqar/transport/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1399 2019-09-25 09:13:27.000000 zaqar-9.0.0.0rc1/zaqar/transport/acl.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    29243 2019-09-25 09:13:27.000000 zaqar-9.0.0.0rc1/zaqar/transport/validation.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      671 2019-09-25 09:13:27.000000 zaqar-9.0.0.0rc1/zaqar/transport/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2327 2019-09-25 09:13:27.000000 zaqar-9.0.0.0rc1/zaqar/transport/base.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-25 09:15:44.000000 zaqar-9.0.0.0rc1/zaqar/transport/wsgi/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-25 09:15:44.000000 zaqar-9.0.0.0rc1/zaqar/transport/wsgi/v2_0/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    13096 2019-09-25 09:13:27.000000 zaqar-9.0.0.0rc1/zaqar/transport/wsgi/v2_0/subscriptions.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8847 2019-09-25 09:13:27.000000 zaqar-9.0.0.0rc1/zaqar/transport/wsgi/v2_0/pools.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7457 2019-09-25 09:13:27.000000 zaqar-9.0.0.0rc1/zaqar/transport/wsgi/v2_0/claims.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    13099 2019-09-25 09:13:27.000000 zaqar-9.0.0.0rc1/zaqar/transport/wsgi/v2_0/queues.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    15541 2019-09-25 09:13:27.000000 zaqar-9.0.0.0rc1/zaqar/transport/wsgi/v2_0/messages.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2659 2019-09-25 09:13:27.000000 zaqar-9.0.0.0rc1/zaqar/transport/wsgi/v2_0/urls.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1411 2019-09-25 09:13:27.000000 zaqar-9.0.0.0rc1/zaqar/transport/wsgi/v2_0/health.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7265 2019-09-25 09:13:27.000000 zaqar-9.0.0.0rc1/zaqar/transport/wsgi/v2_0/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3335 2019-09-25 09:13:27.000000 zaqar-9.0.0.0rc1/zaqar/transport/wsgi/v2_0/topic_purge.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    12611 2019-09-25 09:13:27.000000 zaqar-9.0.0.0rc1/zaqar/transport/wsgi/v2_0/homedoc.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    12928 2019-09-25 09:13:27.000000 zaqar-9.0.0.0rc1/zaqar/transport/wsgi/v2_0/topic.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1178 2019-09-25 09:13:27.000000 zaqar-9.0.0.0rc1/zaqar/transport/wsgi/v2_0/ping.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3410 2019-09-25 09:13:27.000000 zaqar-9.0.0.0rc1/zaqar/transport/wsgi/v2_0/purge.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2533 2019-09-25 09:13:27.000000 zaqar-9.0.0.0rc1/zaqar/transport/wsgi/v2_0/topic_stats.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2533 2019-09-25 09:13:27.000000 zaqar-9.0.0.0rc1/zaqar/transport/wsgi/v2_0/stats.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    14359 2019-09-25 09:13:27.000000 zaqar-9.0.0.0rc1/zaqar/transport/wsgi/v2_0/flavors.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3009 2019-09-25 09:13:27.000000 zaqar-9.0.0.0rc1/zaqar/transport/wsgi/errors.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7410 2019-09-25 09:13:27.000000 zaqar-9.0.0.0rc1/zaqar/transport/wsgi/driver.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-25 09:15:44.000000 zaqar-9.0.0.0rc1/zaqar/transport/wsgi/v1_1/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7822 2019-09-25 09:13:27.000000 zaqar-9.0.0.0rc1/zaqar/transport/wsgi/v1_1/pools.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7289 2019-09-25 09:13:27.000000 zaqar-9.0.0.0rc1/zaqar/transport/wsgi/v1_1/claims.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5754 2019-09-25 09:13:27.000000 zaqar-9.0.0.0rc1/zaqar/transport/wsgi/v1_1/queues.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    12899 2019-09-25 09:13:27.000000 zaqar-9.0.0.0rc1/zaqar/transport/wsgi/v1_1/messages.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1268 2019-09-25 09:13:27.000000 zaqar-9.0.0.0rc1/zaqar/transport/wsgi/v1_1/health.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4113 2019-09-25 09:13:27.000000 zaqar-9.0.0.0rc1/zaqar/transport/wsgi/v1_1/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9225 2019-09-25 09:13:27.000000 zaqar-9.0.0.0rc1/zaqar/transport/wsgi/v1_1/homedoc.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      967 2019-09-25 09:13:27.000000 zaqar-9.0.0.0rc1/zaqar/transport/wsgi/v1_1/ping.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2382 2019-09-25 09:13:27.000000 zaqar-9.0.0.0rc1/zaqar/transport/wsgi/v1_1/stats.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6383 2019-09-25 09:13:27.000000 zaqar-9.0.0.0rc1/zaqar/transport/wsgi/v1_1/flavors.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1075 2019-09-25 09:13:27.000000 zaqar-9.0.0.0rc1/zaqar/transport/wsgi/version.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      670 2019-09-25 09:13:27.000000 zaqar-9.0.0.0rc1/zaqar/transport/wsgi/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-25 09:15:44.000000 zaqar-9.0.0.0rc1/zaqar/transport/wsgi/v1_0/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3648 2019-09-25 09:13:27.000000 zaqar-9.0.0.0rc1/zaqar/transport/wsgi/v1_0/metadata.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7169 2019-09-25 09:13:27.000000 zaqar-9.0.0.0rc1/zaqar/transport/wsgi/v1_0/pools.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6253 2019-09-25 09:13:27.000000 zaqar-9.0.0.0rc1/zaqar/transport/wsgi/v1_0/claims.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4231 2019-09-25 09:13:27.000000 zaqar-9.0.0.0rc1/zaqar/transport/wsgi/v1_0/queues.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10644 2019-09-25 09:13:27.000000 zaqar-9.0.0.0rc1/zaqar/transport/wsgi/v1_0/messages.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      955 2019-09-25 09:13:27.000000 zaqar-9.0.0.0rc1/zaqar/transport/wsgi/v1_0/health.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3443 2019-09-25 09:13:27.000000 zaqar-9.0.0.0rc1/zaqar/transport/wsgi/v1_0/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4656 2019-09-25 09:13:27.000000 zaqar-9.0.0.0rc1/zaqar/transport/wsgi/v1_0/homedoc.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2374 2019-09-25 09:13:27.000000 zaqar-9.0.0.0rc1/zaqar/transport/wsgi/v1_0/stats.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1535 2019-09-25 09:13:27.000000 zaqar-9.0.0.0rc1/zaqar/transport/wsgi/app.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8327 2019-09-25 09:13:27.000000 zaqar-9.0.0.0rc1/zaqar/transport/wsgi/utils.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-25 09:15:44.000000 zaqar-9.0.0.0rc1/zaqar/transport/middleware/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3703 2019-09-25 09:13:27.000000 zaqar-9.0.0.0rc1/zaqar/transport/middleware/cors.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2036 2019-09-25 09:13:27.000000 zaqar-9.0.0.0rc1/zaqar/transport/middleware/auth.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2019-09-25 09:13:27.000000 zaqar-9.0.0.0rc1/zaqar/transport/middleware/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4563 2019-09-25 09:13:27.000000 zaqar-9.0.0.0rc1/zaqar/transport/middleware/profile.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-25 09:15:44.000000 zaqar-9.0.0.0rc1/zaqar/transport/websocket/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4137 2019-09-25 09:13:27.000000 zaqar-9.0.0.0rc1/zaqar/transport/websocket/driver.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      717 2019-09-25 09:13:27.000000 zaqar-9.0.0.0rc1/zaqar/transport/websocket/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10605 2019-09-25 09:13:27.000000 zaqar-9.0.0.0rc1/zaqar/transport/websocket/protocol.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2406 2019-09-25 09:13:27.000000 zaqar-9.0.0.0rc1/zaqar/transport/websocket/factory.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1792 2019-09-25 09:13:27.000000 zaqar-9.0.0.0rc1/zaqar/transport/utils.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-25 09:15:44.000000 zaqar-9.0.0.0rc1/zaqar/tests/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9873 2019-09-25 09:13:26.000000 zaqar-9.0.0.0rc1/zaqar/tests/helpers.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-25 09:15:44.000000 zaqar-9.0.0.0rc1/zaqar/tests/etc/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      454 2019-09-25 09:13:26.000000 zaqar-9.0.0.0rc1/zaqar/tests/etc/wsgi_redis.conf
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      188 2019-09-25 09:13:26.000000 zaqar-9.0.0.0rc1/zaqar/tests/etc/drivers_storage_invalid.conf
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      452 2019-09-25 09:13:26.000000 zaqar-9.0.0.0rc1/zaqar/tests/etc/wsgi_fifo_mongodb.conf
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      219 2019-09-25 09:13:26.000000 zaqar-9.0.0.0rc1/zaqar/tests/etc/functional-tests.conf
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      473 2019-09-25 09:13:26.000000 zaqar-9.0.0.0rc1/zaqar/tests/etc/wsgi_mongodb.conf
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      216 2019-09-25 09:13:26.000000 zaqar-9.0.0.0rc1/zaqar/tests/etc/keystone_auth.conf
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      381 2019-09-25 09:13:26.000000 zaqar-9.0.0.0rc1/zaqar/tests/etc/wsgi_mongodb_pooled.conf
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      197 2019-09-25 09:13:26.000000 zaqar-9.0.0.0rc1/zaqar/tests/etc/wsgi_swift.conf
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      376 2019-09-25 09:13:26.000000 zaqar-9.0.0.0rc1/zaqar/tests/etc/wsgi_redis_pooled.conf
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       41 2019-09-25 09:13:26.000000 zaqar-9.0.0.0rc1/zaqar/tests/etc/policy.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      228 2019-09-25 09:13:26.000000 zaqar-9.0.0.0rc1/zaqar/tests/etc/wsgi_mongodb_validation.conf
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      194 2019-09-25 09:13:26.000000 zaqar-9.0.0.0rc1/zaqar/tests/etc/wsgi_faulty.conf
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      246 2019-09-25 09:13:26.000000 zaqar-9.0.0.0rc1/zaqar/tests/etc/wsgi_sqlalchemy.conf
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      448 2019-09-25 09:13:26.000000 zaqar-9.0.0.0rc1/zaqar/tests/etc/websocket_mongodb_subscriptions.conf
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1471 2019-09-25 09:13:26.000000 zaqar-9.0.0.0rc1/zaqar/tests/etc/functional-zaqar.conf
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      398 2019-09-25 09:13:26.000000 zaqar-9.0.0.0rc1/zaqar/tests/etc/websocket_mongodb_keystone_auth.conf
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      382 2019-09-25 09:13:26.000000 zaqar-9.0.0.0rc1/zaqar/tests/etc/wsgi_mongodb_pooled_disable_virtual_pool.conf
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      390 2019-09-25 09:13:26.000000 zaqar-9.0.0.0rc1/zaqar/tests/etc/websocket_mongodb.conf
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      175 2019-09-25 09:13:26.000000 zaqar-9.0.0.0rc1/zaqar/tests/etc/drivers_transport_invalid.conf
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      248 2019-09-25 09:13:26.000000 zaqar-9.0.0.0rc1/zaqar/tests/etc/wsgi_sqlalchemy_pooled.conf
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      100 2019-09-25 09:13:26.000000 zaqar-9.0.0.0rc1/zaqar/tests/etc/wsgi_mongodb_default_limits.conf
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-25 09:15:44.000000 zaqar-9.0.0.0rc1/zaqar/tests/functional/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1395 2019-09-25 09:13:26.000000 zaqar-9.0.0.0rc1/zaqar/tests/functional/config.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3525 2019-09-25 09:13:26.000000 zaqar-9.0.0.0rc1/zaqar/tests/functional/helpers.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2019-09-25 09:13:26.000000 zaqar-9.0.0.0rc1/zaqar/tests/functional/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    14573 2019-09-25 09:13:26.000000 zaqar-9.0.0.0rc1/zaqar/tests/functional/base.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-25 09:15:44.000000 zaqar-9.0.0.0rc1/zaqar/tests/functional/wsgi/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-25 09:15:44.000000 zaqar-9.0.0.0rc1/zaqar/tests/functional/wsgi/v1/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    14536 2019-09-25 09:13:26.000000 zaqar-9.0.0.0rc1/zaqar/tests/functional/wsgi/v1/test_queues.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2019-09-25 09:13:26.000000 zaqar-9.0.0.0rc1/zaqar/tests/functional/wsgi/v1/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    12997 2019-09-25 09:13:26.000000 zaqar-9.0.0.0rc1/zaqar/tests/functional/wsgi/v1/test_messages.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8395 2019-09-25 09:13:26.000000 zaqar-9.0.0.0rc1/zaqar/tests/functional/wsgi/v1/test_claims.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-25 09:15:44.000000 zaqar-9.0.0.0rc1/zaqar/tests/functional/wsgi/v1_1/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    11897 2019-09-25 09:13:26.000000 zaqar-9.0.0.0rc1/zaqar/tests/functional/wsgi/v1_1/test_queues.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2019-09-25 09:13:26.000000 zaqar-9.0.0.0rc1/zaqar/tests/functional/wsgi/v1_1/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    18199 2019-09-25 09:13:26.000000 zaqar-9.0.0.0rc1/zaqar/tests/functional/wsgi/v1_1/test_messages.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3030 2019-09-25 09:13:26.000000 zaqar-9.0.0.0rc1/zaqar/tests/functional/wsgi/v1_1/test_health.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7332 2019-09-25 09:13:26.000000 zaqar-9.0.0.0rc1/zaqar/tests/functional/wsgi/v1_1/test_pools.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9025 2019-09-25 09:13:26.000000 zaqar-9.0.0.0rc1/zaqar/tests/functional/wsgi/v1_1/test_claims.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2019-09-25 09:13:26.000000 zaqar-9.0.0.0rc1/zaqar/tests/functional/wsgi/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1204 2019-09-25 09:13:26.000000 zaqar-9.0.0.0rc1/zaqar/tests/functional/wsgi/test_versions.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-25 09:15:44.000000 zaqar-9.0.0.0rc1/zaqar/tests/functional/wsgi/v2/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2019-09-25 09:13:26.000000 zaqar-9.0.0.0rc1/zaqar/tests/functional/wsgi/v2/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4658 2019-09-25 09:13:26.000000 zaqar-9.0.0.0rc1/zaqar/tests/functional/wsgi/v2/test_subscriptions.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-25 09:15:44.000000 zaqar-9.0.0.0rc1/zaqar/tests/functional/websocket/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2744 2019-09-25 09:13:26.000000 zaqar-9.0.0.0rc1/zaqar/tests/functional/websocket/test_queues.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2019-09-25 09:13:26.000000 zaqar-9.0.0.0rc1/zaqar/tests/functional/websocket/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6394 2019-09-25 09:13:26.000000 zaqar-9.0.0.0rc1/zaqar/tests/functional/http.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      963 2019-09-25 09:13:26.000000 zaqar-9.0.0.0rc1/zaqar/tests/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-25 09:15:44.000000 zaqar-9.0.0.0rc1/zaqar/tests/unit/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-25 09:15:44.000000 zaqar-9.0.0.0rc1/zaqar/tests/unit/notification/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2019-09-25 09:13:26.000000 zaqar-9.0.0.0rc1/zaqar/tests/unit/notification/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    21777 2019-09-25 09:13:26.000000 zaqar-9.0.0.0rc1/zaqar/tests/unit/notification/test_notifier.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-25 09:15:44.000000 zaqar-9.0.0.0rc1/zaqar/tests/unit/common/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1091 2019-09-25 09:13:26.000000 zaqar-9.0.0.0rc1/zaqar/tests/unit/common/test_request.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4427 2019-09-25 09:13:26.000000 zaqar-9.0.0.0rc1/zaqar/tests/unit/common/test_urls.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2019-09-25 09:13:26.000000 zaqar-9.0.0.0rc1/zaqar/tests/unit/common/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-25 09:15:44.000000 zaqar-9.0.0.0rc1/zaqar/tests/unit/common/storage/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2019-09-25 09:13:26.000000 zaqar-9.0.0.0rc1/zaqar/tests/unit/common/storage/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2663 2019-09-25 09:13:26.000000 zaqar-9.0.0.0rc1/zaqar/tests/unit/common/storage/test_select.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2358 2019-09-25 09:13:26.000000 zaqar-9.0.0.0rc1/zaqar/tests/unit/common/storage/test_utils.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2743 2019-09-25 09:13:26.000000 zaqar-9.0.0.0rc1/zaqar/tests/unit/common/test_pipeline.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1798 2019-09-25 09:13:26.000000 zaqar-9.0.0.0rc1/zaqar/tests/unit/common/test_api.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5740 2019-09-25 09:13:26.000000 zaqar-9.0.0.0rc1/zaqar/tests/unit/common/test_decorators.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2019-09-25 09:13:26.000000 zaqar-9.0.0.0rc1/zaqar/tests/unit/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-25 09:15:44.000000 zaqar-9.0.0.0rc1/zaqar/tests/unit/storage/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    23922 2019-09-25 09:13:26.000000 zaqar-9.0.0.0rc1/zaqar/tests/unit/storage/test_impl_mongodb.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-25 09:15:44.000000 zaqar-9.0.0.0rc1/zaqar/tests/unit/storage/sqlalchemy_migration/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5529 2019-09-25 09:13:26.000000 zaqar-9.0.0.0rc1/zaqar/tests/unit/storage/sqlalchemy_migration/test_migrations.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6931 2019-09-25 09:13:26.000000 zaqar-9.0.0.0rc1/zaqar/tests/unit/storage/sqlalchemy_migration/test_migrations_base.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2019-09-25 09:13:26.000000 zaqar-9.0.0.0rc1/zaqar/tests/unit/storage/sqlalchemy_migration/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3189 2019-09-25 09:13:26.000000 zaqar-9.0.0.0rc1/zaqar/tests/unit/storage/sqlalchemy_migration/test_db_manage_cli.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3350 2019-09-25 09:13:26.000000 zaqar-9.0.0.0rc1/zaqar/tests/unit/storage/test_impl_sqlalchemy.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5432 2019-09-25 09:13:26.000000 zaqar-9.0.0.0rc1/zaqar/tests/unit/storage/test_pool_catalog_new.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2035 2019-09-25 09:13:26.000000 zaqar-9.0.0.0rc1/zaqar/tests/unit/storage/test_impl_swift.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2019-09-25 09:13:26.000000 zaqar-9.0.0.0rc1/zaqar/tests/unit/storage/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    82786 2019-09-25 09:13:26.000000 zaqar-9.0.0.0rc1/zaqar/tests/unit/storage/base.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    22680 2019-09-25 09:13:26.000000 zaqar-9.0.0.0rc1/zaqar/tests/unit/storage/test_impl_redis.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1067 2019-09-25 09:13:26.000000 zaqar-9.0.0.0rc1/zaqar/tests/unit/storage/test_utils.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-25 09:15:44.000000 zaqar-9.0.0.0rc1/zaqar/tests/unit/transport/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1694 2019-09-25 09:13:26.000000 zaqar-9.0.0.0rc1/zaqar/tests/unit/transport/test_acl.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2019-09-25 09:13:26.000000 zaqar-9.0.0.0rc1/zaqar/tests/unit/transport/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-25 09:15:44.000000 zaqar-9.0.0.0rc1/zaqar/tests/unit/transport/wsgi/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-25 09:15:44.000000 zaqar-9.0.0.0rc1/zaqar/tests/unit/transport/wsgi/v2_0/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    15771 2019-09-25 09:13:26.000000 zaqar-9.0.0.0rc1/zaqar/tests/unit/transport/wsgi/v2_0/test_pools_new.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4755 2019-09-25 09:13:26.000000 zaqar-9.0.0.0rc1/zaqar/tests/unit/transport/wsgi/v2_0/test_default_limits.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9557 2019-09-25 09:13:27.000000 zaqar-9.0.0.0rc1/zaqar/tests/unit/transport/wsgi/v2_0/test_validation.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2696 2019-09-25 09:13:26.000000 zaqar-9.0.0.0rc1/zaqar/tests/unit/transport/wsgi/v2_0/test_home.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1256 2019-09-25 09:13:26.000000 zaqar-9.0.0.0rc1/zaqar/tests/unit/transport/wsgi/v2_0/test_ping.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4778 2019-09-25 09:13:26.000000 zaqar-9.0.0.0rc1/zaqar/tests/unit/transport/wsgi/v2_0/test_purge.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    14155 2019-09-25 09:13:26.000000 zaqar-9.0.0.0rc1/zaqar/tests/unit/transport/wsgi/v2_0/test_flavors_new.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8903 2019-09-25 09:13:27.000000 zaqar-9.0.0.0rc1/zaqar/tests/unit/transport/wsgi/v2_0/test_urls.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    25272 2019-09-25 09:13:27.000000 zaqar-9.0.0.0rc1/zaqar/tests/unit/transport/wsgi/v2_0/test_queue_lifecycle.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2019-09-25 09:13:26.000000 zaqar-9.0.0.0rc1/zaqar/tests/unit/transport/wsgi/v2_0/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    28451 2019-09-25 09:13:26.000000 zaqar-9.0.0.0rc1/zaqar/tests/unit/transport/wsgi/v2_0/test_messages.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3094 2019-09-25 09:13:26.000000 zaqar-9.0.0.0rc1/zaqar/tests/unit/transport/wsgi/v2_0/test_health.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3330 2019-09-25 09:13:26.000000 zaqar-9.0.0.0rc1/zaqar/tests/unit/transport/wsgi/v2_0/test_media_type.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    24210 2019-09-25 09:13:27.000000 zaqar-9.0.0.0rc1/zaqar/tests/unit/transport/wsgi/v2_0/test_topic_lifecycle.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1392 2019-09-25 09:13:26.000000 zaqar-9.0.0.0rc1/zaqar/tests/unit/transport/wsgi/v2_0/test_auth.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    19499 2019-09-25 09:13:27.000000 zaqar-9.0.0.0rc1/zaqar/tests/unit/transport/wsgi/v2_0/test_subscriptions.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    12563 2019-09-25 09:13:26.000000 zaqar-9.0.0.0rc1/zaqar/tests/unit/transport/wsgi/v2_0/test_claims.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-25 09:15:44.000000 zaqar-9.0.0.0rc1/zaqar/tests/unit/transport/wsgi/v1/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3543 2019-09-25 09:13:26.000000 zaqar-9.0.0.0rc1/zaqar/tests/unit/transport/wsgi/v1/test_default_limits.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4803 2019-09-25 09:13:26.000000 zaqar-9.0.0.0rc1/zaqar/tests/unit/transport/wsgi/v1/test_validation.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2230 2019-09-25 09:13:26.000000 zaqar-9.0.0.0rc1/zaqar/tests/unit/transport/wsgi/v1/test_home.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    15395 2019-09-25 09:13:26.000000 zaqar-9.0.0.0rc1/zaqar/tests/unit/transport/wsgi/v1/test_queue_lifecycle.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2019-09-25 09:13:26.000000 zaqar-9.0.0.0rc1/zaqar/tests/unit/transport/wsgi/v1/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    19867 2019-09-25 09:13:26.000000 zaqar-9.0.0.0rc1/zaqar/tests/unit/transport/wsgi/v1/test_messages.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1075 2019-09-25 09:13:26.000000 zaqar-9.0.0.0rc1/zaqar/tests/unit/transport/wsgi/v1/test_health.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3332 2019-09-25 09:13:26.000000 zaqar-9.0.0.0rc1/zaqar/tests/unit/transport/wsgi/v1/test_media_type.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1392 2019-09-25 09:13:26.000000 zaqar-9.0.0.0rc1/zaqar/tests/unit/transport/wsgi/v1/test_auth.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    13346 2019-09-25 09:13:26.000000 zaqar-9.0.0.0rc1/zaqar/tests/unit/transport/wsgi/v1/test_pools.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10037 2019-09-25 09:13:26.000000 zaqar-9.0.0.0rc1/zaqar/tests/unit/transport/wsgi/v1/test_claims.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2293 2019-09-25 09:13:26.000000 zaqar-9.0.0.0rc1/zaqar/tests/unit/transport/wsgi/test_version.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-25 09:15:44.000000 zaqar-9.0.0.0rc1/zaqar/tests/unit/transport/wsgi/v1_1/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4757 2019-09-25 09:13:26.000000 zaqar-9.0.0.0rc1/zaqar/tests/unit/transport/wsgi/v1_1/test_default_limits.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5055 2019-09-25 09:13:26.000000 zaqar-9.0.0.0rc1/zaqar/tests/unit/transport/wsgi/v1_1/test_validation.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2698 2019-09-25 09:13:26.000000 zaqar-9.0.0.0rc1/zaqar/tests/unit/transport/wsgi/v1_1/test_home.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1262 2019-09-25 09:13:26.000000 zaqar-9.0.0.0rc1/zaqar/tests/unit/transport/wsgi/v1_1/test_ping.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    14716 2019-09-25 09:13:26.000000 zaqar-9.0.0.0rc1/zaqar/tests/unit/transport/wsgi/v1_1/test_queue_lifecycle.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2019-09-25 09:13:26.000000 zaqar-9.0.0.0rc1/zaqar/tests/unit/transport/wsgi/v1_1/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    25148 2019-09-25 09:13:26.000000 zaqar-9.0.0.0rc1/zaqar/tests/unit/transport/wsgi/v1_1/test_messages.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3098 2019-09-25 09:13:26.000000 zaqar-9.0.0.0rc1/zaqar/tests/unit/transport/wsgi/v1_1/test_health.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3295 2019-09-25 09:13:26.000000 zaqar-9.0.0.0rc1/zaqar/tests/unit/transport/wsgi/v1_1/test_media_type.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1394 2019-09-25 09:13:26.000000 zaqar-9.0.0.0rc1/zaqar/tests/unit/transport/wsgi/v1_1/test_auth.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    12566 2019-09-25 09:13:26.000000 zaqar-9.0.0.0rc1/zaqar/tests/unit/transport/wsgi/v1_1/test_claims.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      826 2019-09-25 09:13:26.000000 zaqar-9.0.0.0rc1/zaqar/tests/unit/transport/wsgi/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5952 2019-09-25 09:13:26.000000 zaqar-9.0.0.0rc1/zaqar/tests/unit/transport/wsgi/base.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6728 2019-09-25 09:13:26.000000 zaqar-9.0.0.0rc1/zaqar/tests/unit/transport/wsgi/test_utils.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-25 09:15:44.000000 zaqar-9.0.0.0rc1/zaqar/tests/unit/transport/websocket/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4253 2019-09-25 09:13:26.000000 zaqar-9.0.0.0rc1/zaqar/tests/unit/transport/websocket/test_protocol.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2019-09-25 09:13:26.000000 zaqar-9.0.0.0rc1/zaqar/tests/unit/transport/websocket/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3046 2019-09-25 09:13:26.000000 zaqar-9.0.0.0rc1/zaqar/tests/unit/transport/websocket/base.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-25 09:15:44.000000 zaqar-9.0.0.0rc1/zaqar/tests/unit/transport/websocket/v2/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    22743 2019-09-25 09:13:26.000000 zaqar-9.0.0.0rc1/zaqar/tests/unit/transport/websocket/v2/test_queue_lifecycle.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2019-09-25 09:13:26.000000 zaqar-9.0.0.0rc1/zaqar/tests/unit/transport/websocket/v2/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    21340 2019-09-25 09:13:26.000000 zaqar-9.0.0.0rc1/zaqar/tests/unit/transport/websocket/v2/test_messages.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10377 2019-09-25 09:13:26.000000 zaqar-9.0.0.0rc1/zaqar/tests/unit/transport/websocket/v2/test_auth.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    16329 2019-09-25 09:13:26.000000 zaqar-9.0.0.0rc1/zaqar/tests/unit/transport/websocket/v2/test_subscriptions.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    16459 2019-09-25 09:13:26.000000 zaqar-9.0.0.0rc1/zaqar/tests/unit/transport/websocket/v2/test_claims.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1704 2019-09-25 09:13:26.000000 zaqar-9.0.0.0rc1/zaqar/tests/unit/transport/websocket/utils.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-25 09:15:44.000000 zaqar-9.0.0.0rc1/zaqar/tests/unit/cmd/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2019-09-25 09:13:26.000000 zaqar-9.0.0.0rc1/zaqar/tests/unit/cmd/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1024 2019-09-25 09:13:26.000000 zaqar-9.0.0.0rc1/zaqar/tests/unit/cmd/test_status.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2031 2019-09-25 09:13:26.000000 zaqar-9.0.0.0rc1/zaqar/tests/unit/test_bootstrap.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-25 09:15:44.000000 zaqar-9.0.0.0rc1/zaqar/tests/unit/hacking/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2019-09-25 09:13:26.000000 zaqar-9.0.0.0rc1/zaqar/tests/unit/hacking/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1160 2019-09-25 09:13:26.000000 zaqar-9.0.0.0rc1/zaqar/tests/unit/hacking/test_hacking.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4210 2019-09-25 09:13:26.000000 zaqar-9.0.0.0rc1/zaqar/tests/base.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4645 2019-09-25 09:13:26.000000 zaqar-9.0.0.0rc1/zaqar/tests/faulty_storage.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-25 09:15:44.000000 zaqar-9.0.0.0rc1/zaqar/locale/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-25 09:15:44.000000 zaqar-9.0.0.0rc1/zaqar/locale/en_GB/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-25 09:15:44.000000 zaqar-9.0.0.0rc1/zaqar/locale/en_GB/LC_MESSAGES/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    23462 2019-09-25 09:13:26.000000 zaqar-9.0.0.0rc1/zaqar/locale/en_GB/LC_MESSAGES/zaqar.po
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-25 09:15:44.000000 zaqar-9.0.0.0rc1/zaqar/locale/es/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-25 09:15:44.000000 zaqar-9.0.0.0rc1/zaqar/locale/es/LC_MESSAGES/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    12000 2019-09-25 09:13:26.000000 zaqar-9.0.0.0rc1/zaqar/locale/es/LC_MESSAGES/zaqar.po
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-25 09:15:44.000000 zaqar-9.0.0.0rc1/zaqar/locale/id/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-25 09:15:44.000000 zaqar-9.0.0.0rc1/zaqar/locale/id/LC_MESSAGES/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    24198 2019-09-25 09:13:26.000000 zaqar-9.0.0.0rc1/zaqar/locale/id/LC_MESSAGES/zaqar.po
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-25 09:15:44.000000 zaqar-9.0.0.0rc1/zaqar/locale/de/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-25 09:15:44.000000 zaqar-9.0.0.0rc1/zaqar/locale/de/LC_MESSAGES/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    26054 2019-09-25 09:13:26.000000 zaqar-9.0.0.0rc1/zaqar/locale/de/LC_MESSAGES/zaqar.po
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-25 09:15:44.000000 zaqar-9.0.0.0rc1/zaqar/cmd/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1079 2019-09-25 09:13:26.000000 zaqar-9.0.0.0rc1/zaqar/cmd/gc.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1853 2019-09-25 09:13:26.000000 zaqar-9.0.0.0rc1/zaqar/cmd/status.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2019-09-25 09:13:26.000000 zaqar-9.0.0.0rc1/zaqar/cmd/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2976 2019-09-25 09:13:26.000000 zaqar-9.0.0.0rc1/zaqar/cmd/server.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      906 2019-09-25 09:13:26.000000 zaqar-9.0.0.0rc1/zaqar/i18n.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2370 2019-09-25 09:13:26.000000 zaqar-9.0.0.0rc1/zaqar/context.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-25 09:15:44.000000 zaqar-9.0.0.0rc1/zaqar/hacking/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1650 2019-09-25 09:13:26.000000 zaqar-9.0.0.0rc1/zaqar/hacking/checks.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2019-09-25 09:13:26.000000 zaqar-9.0.0.0rc1/zaqar/hacking/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4719 2019-09-25 09:13:26.000000 zaqar-9.0.0.0rc1/zaqar/bootstrap.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      835 2019-09-25 09:13:26.000000 zaqar-9.0.0.0rc1/test-requirements.txt
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-25 09:15:44.000000 zaqar-9.0.0.0rc1/tools/
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)     1186 2019-09-25 09:13:26.000000 zaqar-9.0.0.0rc1/tools/test-setup.sh
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-25 09:15:44.000000 zaqar-9.0.0.0rc1/tools/doc/
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)      490 2019-09-25 09:13:26.000000 zaqar-9.0.0.0rc1/tools/doc/find_autodoc_modules.sh
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)     1020 2019-09-25 09:13:26.000000 zaqar-9.0.0.0rc1/tools/doc/generate_autodoc_index.sh
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1377 2019-09-25 09:13:26.000000 zaqar-9.0.0.0rc1/lower-constraints.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      419 2019-09-25 09:13:26.000000 zaqar-9.0.0.0rc1/dox.yml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2494 2019-09-25 09:13:26.000000 zaqar-9.0.0.0rc1/README.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       84 2019-09-25 09:13:26.000000 zaqar-9.0.0.0rc1/.stestr.conf
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-25 09:15:44.000000 zaqar-9.0.0.0rc1/zaqar.egg-info/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3975 2019-09-25 09:15:43.000000 zaqar-9.0.0.0rc1/zaqar.egg-info/PKG-INFO
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2019-09-25 09:15:43.000000 zaqar-9.0.0.0rc1/zaqar.egg-info/dependency_links.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2019-09-25 09:15:43.000000 zaqar-9.0.0.0rc1/zaqar.egg-info/not-zip-safe
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      719 2019-09-25 09:15:43.000000 zaqar-9.0.0.0rc1/zaqar.egg-info/requires.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       47 2019-09-25 09:15:43.000000 zaqar-9.0.0.0rc1/zaqar.egg-info/pbr.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    23336 2019-09-25 09:15:44.000000 zaqar-9.0.0.0rc1/zaqar.egg-info/SOURCES.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        6 2019-09-25 09:15:43.000000 zaqar-9.0.0.0rc1/zaqar.egg-info/top_level.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2066 2019-09-25 09:15:43.000000 zaqar-9.0.0.0rc1/zaqar.egg-info/entry_points.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    65000 2019-09-25 09:15:43.000000 zaqar-9.0.0.0rc1/ChangeLog
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1259 2019-09-25 09:13:26.000000 zaqar-9.0.0.0rc1/requirements.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      120 2019-09-25 09:13:26.000000 zaqar-9.0.0.0rc1/.coveragerc
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4269 2019-09-25 09:13:26.000000 zaqar-9.0.0.0rc1/HACKING.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-25 09:15:44.000000 zaqar-9.0.0.0rc1/zaqar_upgradetests/
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-25 09:13:27.000000 zaqar-9.0.0.0rc1/zaqar_upgradetests/pre_test_hook.sh
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-09-25 09:13:27.000000 zaqar-9.0.0.0rc1/zaqar_upgradetests/post_test_hook.sh
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-15 09:53:07.000000 zaqar-9.0.1/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       17 2020-06-15 09:51:10.000000 zaqar-9.0.1/babel.cfg
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3365 2020-06-15 09:51:10.000000 zaqar-9.0.1/tox.ini
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      533 2020-06-15 09:51:10.000000 zaqar-9.0.1/bindep.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    65132 2020-06-15 09:53:07.000000 zaqar-9.0.1/ChangeLog
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      120 2020-06-15 09:51:10.000000 zaqar-9.0.1/.coveragerc
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10143 2020-06-15 09:51:10.000000 zaqar-9.0.1/LICENSE
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-15 09:53:07.000000 zaqar-9.0.1/api-ref/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-15 09:53:07.000000 zaqar-9.0.1/api-ref/source/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4293 2020-06-15 09:51:10.000000 zaqar-9.0.1/api-ref/source/subscription.inc
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5326 2020-06-15 09:51:10.000000 zaqar-9.0.1/api-ref/source/pools.inc
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1124 2020-06-15 09:51:10.000000 zaqar-9.0.1/api-ref/source/versions.inc
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1704 2020-06-15 09:51:10.000000 zaqar-9.0.1/api-ref/source/status.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5367 2020-06-15 09:51:10.000000 zaqar-9.0.1/api-ref/source/flavors.inc
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      904 2020-06-15 09:51:10.000000 zaqar-9.0.1/api-ref/source/index.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8474 2020-06-15 09:51:10.000000 zaqar-9.0.1/api-ref/source/queues.inc
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    16855 2020-06-15 09:51:10.000000 zaqar-9.0.1/api-ref/source/parameters.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5946 2020-06-15 09:51:10.000000 zaqar-9.0.1/api-ref/source/claims.inc
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7392 2020-06-15 09:51:10.000000 zaqar-9.0.1/api-ref/source/conf.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10035 2020-06-15 09:51:10.000000 zaqar-9.0.1/api-ref/source/messages.inc
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1635 2020-06-15 09:51:10.000000 zaqar-9.0.1/api-ref/source/health.inc
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-15 09:53:07.000000 zaqar-9.0.1/api-ref/source/samples/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      349 2020-06-15 09:51:10.000000 zaqar-9.0.1/api-ref/source/samples/claim_messages_response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      454 2020-06-15 09:51:10.000000 zaqar-9.0.1/api-ref/source/samples/flavor-list-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      496 2020-06-15 09:51:10.000000 zaqar-9.0.1/api-ref/source/samples/pool-list-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      158 2020-06-15 09:51:10.000000 zaqar-9.0.1/api-ref/source/samples/pool-show-response-new.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      141 2020-06-15 09:51:10.000000 zaqar-9.0.1/api-ref/source/samples/pool-update-request.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      139 2020-06-15 09:51:10.000000 zaqar-9.0.1/api-ref/source/samples/pool-create-request.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      211 2020-06-15 09:51:10.000000 zaqar-9.0.1/api-ref/source/samples/flavor-show-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      327 2020-06-15 09:51:10.000000 zaqar-9.0.1/api-ref/source/samples/claim_query_response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      136 2020-06-15 09:51:10.000000 zaqar-9.0.1/api-ref/source/samples/queue-pre-signed-request.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      157 2020-06-15 09:51:10.000000 zaqar-9.0.1/api-ref/source/samples/pool-show-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       33 2020-06-15 09:51:10.000000 zaqar-9.0.1/api-ref/source/samples/flavor-create-request.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       36 2020-06-15 09:51:10.000000 zaqar-9.0.1/api-ref/source/samples/claim_messages_request.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1228 2020-06-15 09:51:10.000000 zaqar-9.0.1/api-ref/source/samples/versions-list-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      996 2020-06-15 09:51:10.000000 zaqar-9.0.1/api-ref/source/samples/messages-list-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       33 2020-06-15 09:51:10.000000 zaqar-9.0.1/api-ref/source/samples/flavor-update-request.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      224 2020-06-15 09:51:10.000000 zaqar-9.0.1/api-ref/source/samples/flavor-show-response-new.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      156 2020-06-15 09:51:10.000000 zaqar-9.0.1/api-ref/source/samples/pool-update-response-new.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      172 2020-06-15 09:51:10.000000 zaqar-9.0.1/api-ref/source/samples/subscription-show-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      193 2020-06-15 09:51:10.000000 zaqar-9.0.1/api-ref/source/samples/flavor-update-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      235 2020-06-15 09:51:10.000000 zaqar-9.0.1/api-ref/source/samples/queue-show-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      480 2020-06-15 09:51:10.000000 zaqar-9.0.1/api-ref/source/samples/flavor-list-response-new.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       32 2020-06-15 09:51:10.000000 zaqar-9.0.1/api-ref/source/samples/claim_update_request.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       55 2020-06-15 09:51:10.000000 zaqar-9.0.1/api-ref/source/samples/purge-queue-request.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      498 2020-06-15 09:51:10.000000 zaqar-9.0.1/api-ref/source/samples/pool-list-response-new.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      378 2020-06-15 09:51:10.000000 zaqar-9.0.1/api-ref/source/samples/messages-get-byids-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       26 2020-06-15 09:51:10.000000 zaqar-9.0.1/api-ref/source/samples/queue-update-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      139 2020-06-15 09:51:10.000000 zaqar-9.0.1/api-ref/source/samples/pool-update-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       51 2020-06-15 09:51:10.000000 zaqar-9.0.1/api-ref/source/samples/subscription-create-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      394 2020-06-15 09:51:10.000000 zaqar-9.0.1/api-ref/source/samples/queue-pre-signed-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       92 2020-06-15 09:51:10.000000 zaqar-9.0.1/api-ref/source/samples/queue-stats-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      373 2020-06-15 09:51:10.000000 zaqar-9.0.1/api-ref/source/samples/queues-list-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      517 2020-06-15 09:51:10.000000 zaqar-9.0.1/api-ref/source/samples/subscriptions-list-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      205 2020-06-15 09:51:10.000000 zaqar-9.0.1/api-ref/source/samples/flavor-update-response-new.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      102 2020-06-15 09:51:10.000000 zaqar-9.0.1/api-ref/source/samples/queue-update-request.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      147 2020-06-15 09:51:10.000000 zaqar-9.0.1/api-ref/source/samples/messages-post-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1404 2020-06-15 09:51:10.000000 zaqar-9.0.1/api-ref/source/samples/health-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      143 2020-06-15 09:51:10.000000 zaqar-9.0.1/api-ref/source/samples/pool-update-request-new.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      319 2020-06-15 09:51:10.000000 zaqar-9.0.1/api-ref/source/samples/messages-get-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      130 2020-06-15 09:51:10.000000 zaqar-9.0.1/api-ref/source/samples/subscription-create-request-mail.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      141 2020-06-15 09:51:10.000000 zaqar-9.0.1/api-ref/source/samples/pool-create-request-new.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      305 2020-06-15 09:51:10.000000 zaqar-9.0.1/api-ref/source/samples/messages-delete-bypop-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       45 2020-06-15 09:51:10.000000 zaqar-9.0.1/api-ref/source/samples/flavor-create-request-new.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      107 2020-06-15 09:51:10.000000 zaqar-9.0.1/api-ref/source/samples/subscription-update-request.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      286 2020-06-15 09:51:10.000000 zaqar-9.0.1/api-ref/source/samples/queue-create-request.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       45 2020-06-15 09:51:10.000000 zaqar-9.0.1/api-ref/source/samples/flavor-update-request-new.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       82 2020-06-15 09:51:10.000000 zaqar-9.0.1/api-ref/source/samples/subscription-create-request-http.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      326 2020-06-15 09:51:10.000000 zaqar-9.0.1/api-ref/source/samples/messages-post-request.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1030 2020-06-15 09:51:10.000000 zaqar-9.0.1/setup.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      419 2020-06-15 09:51:10.000000 zaqar-9.0.1/dox.yml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3970 2020-06-15 09:53:07.000000 zaqar-9.0.1/PKG-INFO
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-15 09:53:07.000000 zaqar-9.0.1/zaqar/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-15 09:53:07.000000 zaqar-9.0.1/zaqar/conf/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2031 2020-06-15 09:51:10.000000 zaqar-9.0.1/zaqar/conf/default.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1211 2020-06-15 09:51:10.000000 zaqar-9.0.1/zaqar/conf/drivers.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1029 2020-06-15 09:51:10.000000 zaqar-9.0.1/zaqar/conf/drivers_transport_wsgi.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4557 2020-06-15 09:51:10.000000 zaqar-9.0.1/zaqar/conf/notification.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5533 2020-06-15 09:51:10.000000 zaqar-9.0.1/zaqar/conf/drivers_message_store_mongodb.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1319 2020-06-15 09:51:10.000000 zaqar-9.0.1/zaqar/conf/profiler.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1901 2020-06-15 09:51:10.000000 zaqar-9.0.1/zaqar/conf/drivers_message_store_swift.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2136 2020-06-15 09:51:10.000000 zaqar-9.0.1/zaqar/conf/storage.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      879 2020-06-15 09:51:10.000000 zaqar-9.0.1/zaqar/conf/signed_url.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1014 2020-06-15 09:51:10.000000 zaqar-9.0.1/zaqar/conf/drivers_management_store_sqlalchemy.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4969 2020-06-15 09:51:10.000000 zaqar-9.0.1/zaqar/conf/drivers_management_store_mongodb.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5749 2020-06-15 09:51:10.000000 zaqar-9.0.1/zaqar/conf/transport.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2123 2020-06-15 09:51:10.000000 zaqar-9.0.1/zaqar/conf/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3623 2020-06-15 09:51:10.000000 zaqar-9.0.1/zaqar/conf/opts.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1494 2020-06-15 09:51:10.000000 zaqar-9.0.1/zaqar/conf/drivers_transport_websocket.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      959 2020-06-15 09:51:10.000000 zaqar-9.0.1/zaqar/conf/pooling_catalog.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3283 2020-06-15 09:51:10.000000 zaqar-9.0.1/zaqar/conf/drivers_management_store_redis.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3280 2020-06-15 09:51:10.000000 zaqar-9.0.1/zaqar/conf/drivers_message_store_redis.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-15 09:53:07.000000 zaqar-9.0.1/zaqar/bench/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4922 2020-06-15 09:51:10.000000 zaqar-9.0.1/zaqar/bench/observer.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3017 2020-06-15 09:51:10.000000 zaqar-9.0.1/zaqar/bench/conductor.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4734 2020-06-15 09:51:10.000000 zaqar-9.0.1/zaqar/bench/helpers.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6154 2020-06-15 09:51:10.000000 zaqar-9.0.1/zaqar/bench/consumer.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2555 2020-06-15 09:51:10.000000 zaqar-9.0.1/zaqar/bench/config.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5463 2020-06-15 09:51:10.000000 zaqar-9.0.1/zaqar/bench/producer.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-06-15 09:51:10.000000 zaqar-9.0.1/zaqar/bench/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2370 2020-06-15 09:51:10.000000 zaqar-9.0.1/zaqar/context.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-15 09:53:07.000000 zaqar-9.0.1/zaqar/hacking/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1650 2020-06-15 09:51:10.000000 zaqar-9.0.1/zaqar/hacking/checks.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-06-15 09:51:10.000000 zaqar-9.0.1/zaqar/hacking/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-15 09:53:07.000000 zaqar-9.0.1/zaqar/storage/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-15 09:53:07.000000 zaqar-9.0.1/zaqar/storage/redis/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6517 2020-06-15 09:51:10.000000 zaqar-9.0.1/zaqar/storage/redis/flavors.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    11283 2020-06-15 09:51:10.000000 zaqar-9.0.1/zaqar/storage/redis/subscriptions.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    11783 2020-06-15 09:51:10.000000 zaqar-9.0.1/zaqar/storage/redis/driver.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    12597 2020-06-15 09:51:10.000000 zaqar-9.0.1/zaqar/storage/redis/utils.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9651 2020-06-15 09:51:10.000000 zaqar-9.0.1/zaqar/storage/redis/pools.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8964 2020-06-15 09:51:10.000000 zaqar-9.0.1/zaqar/storage/redis/catalogue.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6515 2020-06-15 09:51:10.000000 zaqar-9.0.1/zaqar/storage/redis/queues.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    24333 2020-06-15 09:51:10.000000 zaqar-9.0.1/zaqar/storage/redis/messages.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10108 2020-06-15 09:51:10.000000 zaqar-9.0.1/zaqar/storage/redis/models.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1181 2020-06-15 09:51:10.000000 zaqar-9.0.1/zaqar/storage/redis/scripting.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1990 2020-06-15 09:51:10.000000 zaqar-9.0.1/zaqar/storage/redis/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1198 2020-06-15 09:51:10.000000 zaqar-9.0.1/zaqar/storage/redis/controllers.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-15 09:53:07.000000 zaqar-9.0.1/zaqar/storage/redis/scripts/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1104 2020-06-15 09:51:10.000000 zaqar-9.0.1/zaqar/storage/redis/scripts/index_messages.lua
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3451 2020-06-15 09:51:10.000000 zaqar-9.0.1/zaqar/storage/redis/scripts/claim_messages.lua
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    18770 2020-06-15 09:51:10.000000 zaqar-9.0.1/zaqar/storage/redis/claims.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    33867 2020-06-15 09:51:10.000000 zaqar-9.0.1/zaqar/storage/pooling.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-15 09:53:07.000000 zaqar-9.0.1/zaqar/storage/sqlalchemy/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4684 2020-06-15 09:51:10.000000 zaqar-9.0.1/zaqar/storage/sqlalchemy/flavors.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2182 2020-06-15 09:51:10.000000 zaqar-9.0.1/zaqar/storage/sqlalchemy/tables.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4314 2020-06-15 09:51:10.000000 zaqar-9.0.1/zaqar/storage/sqlalchemy/driver.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3722 2020-06-15 09:51:10.000000 zaqar-9.0.1/zaqar/storage/sqlalchemy/utils.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5509 2020-06-15 09:51:10.000000 zaqar-9.0.1/zaqar/storage/sqlalchemy/pools.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-15 09:53:07.000000 zaqar-9.0.1/zaqar/storage/sqlalchemy/migration/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3874 2020-06-15 09:51:10.000000 zaqar-9.0.1/zaqar/storage/sqlalchemy/migration/cli.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      975 2020-06-15 09:51:10.000000 zaqar-9.0.1/zaqar/storage/sqlalchemy/migration/alembic.ini
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-15 09:53:07.000000 zaqar-9.0.1/zaqar/storage/sqlalchemy/migration/alembic_migrations/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      952 2020-06-15 09:51:10.000000 zaqar-9.0.1/zaqar/storage/sqlalchemy/migration/alembic_migrations/script.py.mako
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2747 2020-06-15 09:51:10.000000 zaqar-9.0.1/zaqar/storage/sqlalchemy/migration/alembic_migrations/env.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2493 2020-06-15 09:51:10.000000 zaqar-9.0.1/zaqar/storage/sqlalchemy/migration/alembic_migrations/README.md
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-15 09:53:07.000000 zaqar-9.0.1/zaqar/storage/sqlalchemy/migration/alembic_migrations/versions/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2725 2020-06-15 09:51:10.000000 zaqar-9.0.1/zaqar/storage/sqlalchemy/migration/alembic_migrations/versions/001_liberty.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1579 2020-06-15 09:51:10.000000 zaqar-9.0.1/zaqar/storage/sqlalchemy/migration/alembic_migrations/versions/007_stein.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      785 2020-06-15 09:51:10.000000 zaqar-9.0.1/zaqar/storage/sqlalchemy/migration/alembic_migrations/versions/004_placeholder.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      785 2020-06-15 09:51:10.000000 zaqar-9.0.1/zaqar/storage/sqlalchemy/migration/alembic_migrations/versions/002_placeholder.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      785 2020-06-15 09:51:10.000000 zaqar-9.0.1/zaqar/storage/sqlalchemy/migration/alembic_migrations/versions/005_placeholder.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      785 2020-06-15 09:51:10.000000 zaqar-9.0.1/zaqar/storage/sqlalchemy/migration/alembic_migrations/versions/003_placeholder.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1200 2020-06-15 09:51:10.000000 zaqar-9.0.1/zaqar/storage/sqlalchemy/migration/alembic_migrations/versions/006_queens.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-06-15 09:51:10.000000 zaqar-9.0.1/zaqar/storage/sqlalchemy/migration/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3146 2020-06-15 09:51:10.000000 zaqar-9.0.1/zaqar/storage/sqlalchemy/catalogue.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4299 2020-06-15 09:51:10.000000 zaqar-9.0.1/zaqar/storage/sqlalchemy/queues.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      713 2020-06-15 09:51:10.000000 zaqar-9.0.1/zaqar/storage/sqlalchemy/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      986 2020-06-15 09:51:10.000000 zaqar-9.0.1/zaqar/storage/sqlalchemy/controllers.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1625 2020-06-15 09:51:10.000000 zaqar-9.0.1/zaqar/storage/configuration.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8105 2020-06-15 09:51:10.000000 zaqar-9.0.1/zaqar/storage/utils.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-15 09:53:07.000000 zaqar-9.0.1/zaqar/storage/swift/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7064 2020-06-15 09:51:10.000000 zaqar-9.0.1/zaqar/storage/swift/subscriptions.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4868 2020-06-15 09:51:10.000000 zaqar-9.0.1/zaqar/storage/swift/driver.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5169 2020-06-15 09:51:10.000000 zaqar-9.0.1/zaqar/storage/swift/utils.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    18564 2020-06-15 09:51:10.000000 zaqar-9.0.1/zaqar/storage/swift/messages.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-06-15 09:51:10.000000 zaqar-9.0.1/zaqar/storage/swift/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      824 2020-06-15 09:51:10.000000 zaqar-9.0.1/zaqar/storage/swift/controllers.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9911 2020-06-15 09:51:10.000000 zaqar-9.0.1/zaqar/storage/swift/claims.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6831 2020-06-15 09:51:10.000000 zaqar-9.0.1/zaqar/storage/errors.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6494 2020-06-15 09:51:10.000000 zaqar-9.0.1/zaqar/storage/pipeline.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-15 09:53:07.000000 zaqar-9.0.1/zaqar/storage/mongodb/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4660 2020-06-15 09:51:10.000000 zaqar-9.0.1/zaqar/storage/mongodb/flavors.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10047 2020-06-15 09:51:10.000000 zaqar-9.0.1/zaqar/storage/mongodb/topics.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7417 2020-06-15 09:51:10.000000 zaqar-9.0.1/zaqar/storage/mongodb/subscriptions.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    12091 2020-06-15 09:51:10.000000 zaqar-9.0.1/zaqar/storage/mongodb/driver.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10803 2020-06-15 09:51:10.000000 zaqar-9.0.1/zaqar/storage/mongodb/utils.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6198 2020-06-15 09:51:10.000000 zaqar-9.0.1/zaqar/storage/mongodb/pools.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3285 2020-06-15 09:51:10.000000 zaqar-9.0.1/zaqar/storage/mongodb/catalogue.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10656 2020-06-15 09:51:10.000000 zaqar-9.0.1/zaqar/storage/mongodb/queues.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    42517 2020-06-15 09:51:10.000000 zaqar-9.0.1/zaqar/storage/mongodb/messages.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2023 2020-06-15 09:51:10.000000 zaqar-9.0.1/zaqar/storage/mongodb/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1625 2020-06-15 09:51:10.000000 zaqar-9.0.1/zaqar/storage/mongodb/controllers.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    14129 2020-06-15 09:51:10.000000 zaqar-9.0.1/zaqar/storage/mongodb/claims.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    38641 2020-06-15 09:51:10.000000 zaqar-9.0.1/zaqar/storage/mongodb/topic_messages.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    40104 2020-06-15 09:51:10.000000 zaqar-9.0.1/zaqar/storage/base.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1360 2020-06-15 09:51:10.000000 zaqar-9.0.1/zaqar/storage/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-15 09:53:07.000000 zaqar-9.0.1/zaqar/cmd/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1853 2020-06-15 09:51:10.000000 zaqar-9.0.1/zaqar/cmd/status.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2976 2020-06-15 09:51:10.000000 zaqar-9.0.1/zaqar/cmd/server.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1079 2020-06-15 09:51:10.000000 zaqar-9.0.1/zaqar/cmd/gc.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-06-15 09:51:10.000000 zaqar-9.0.1/zaqar/cmd/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-15 09:53:07.000000 zaqar-9.0.1/zaqar/tests/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9873 2020-06-15 09:51:10.000000 zaqar-9.0.1/zaqar/tests/helpers.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-15 09:53:07.000000 zaqar-9.0.1/zaqar/tests/functional/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3525 2020-06-15 09:51:10.000000 zaqar-9.0.1/zaqar/tests/functional/helpers.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1395 2020-06-15 09:51:10.000000 zaqar-9.0.1/zaqar/tests/functional/config.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-15 09:53:07.000000 zaqar-9.0.1/zaqar/tests/functional/websocket/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2744 2020-06-15 09:51:10.000000 zaqar-9.0.1/zaqar/tests/functional/websocket/test_queues.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-06-15 09:51:10.000000 zaqar-9.0.1/zaqar/tests/functional/websocket/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    14573 2020-06-15 09:51:10.000000 zaqar-9.0.1/zaqar/tests/functional/base.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6394 2020-06-15 09:51:10.000000 zaqar-9.0.1/zaqar/tests/functional/http.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-06-15 09:51:10.000000 zaqar-9.0.1/zaqar/tests/functional/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-15 09:53:07.000000 zaqar-9.0.1/zaqar/tests/functional/wsgi/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-15 09:53:07.000000 zaqar-9.0.1/zaqar/tests/functional/wsgi/v1/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8395 2020-06-15 09:51:10.000000 zaqar-9.0.1/zaqar/tests/functional/wsgi/v1/test_claims.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    12997 2020-06-15 09:51:10.000000 zaqar-9.0.1/zaqar/tests/functional/wsgi/v1/test_messages.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    14536 2020-06-15 09:51:10.000000 zaqar-9.0.1/zaqar/tests/functional/wsgi/v1/test_queues.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-06-15 09:51:10.000000 zaqar-9.0.1/zaqar/tests/functional/wsgi/v1/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1204 2020-06-15 09:51:10.000000 zaqar-9.0.1/zaqar/tests/functional/wsgi/test_versions.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-15 09:53:07.000000 zaqar-9.0.1/zaqar/tests/functional/wsgi/v1_1/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7332 2020-06-15 09:51:10.000000 zaqar-9.0.1/zaqar/tests/functional/wsgi/v1_1/test_pools.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9025 2020-06-15 09:51:10.000000 zaqar-9.0.1/zaqar/tests/functional/wsgi/v1_1/test_claims.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    18199 2020-06-15 09:51:10.000000 zaqar-9.0.1/zaqar/tests/functional/wsgi/v1_1/test_messages.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    11897 2020-06-15 09:51:10.000000 zaqar-9.0.1/zaqar/tests/functional/wsgi/v1_1/test_queues.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-06-15 09:51:10.000000 zaqar-9.0.1/zaqar/tests/functional/wsgi/v1_1/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3030 2020-06-15 09:51:10.000000 zaqar-9.0.1/zaqar/tests/functional/wsgi/v1_1/test_health.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-06-15 09:51:10.000000 zaqar-9.0.1/zaqar/tests/functional/wsgi/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-15 09:53:07.000000 zaqar-9.0.1/zaqar/tests/functional/wsgi/v2/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4658 2020-06-15 09:51:10.000000 zaqar-9.0.1/zaqar/tests/functional/wsgi/v2/test_subscriptions.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-06-15 09:51:10.000000 zaqar-9.0.1/zaqar/tests/functional/wsgi/v2/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-15 09:53:07.000000 zaqar-9.0.1/zaqar/tests/etc/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      197 2020-06-15 09:51:10.000000 zaqar-9.0.1/zaqar/tests/etc/wsgi_swift.conf
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      246 2020-06-15 09:51:10.000000 zaqar-9.0.1/zaqar/tests/etc/wsgi_sqlalchemy.conf
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      390 2020-06-15 09:51:10.000000 zaqar-9.0.1/zaqar/tests/etc/websocket_mongodb.conf
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      376 2020-06-15 09:51:10.000000 zaqar-9.0.1/zaqar/tests/etc/wsgi_redis_pooled.conf
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1471 2020-06-15 09:51:10.000000 zaqar-9.0.1/zaqar/tests/etc/functional-zaqar.conf
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      248 2020-06-15 09:51:10.000000 zaqar-9.0.1/zaqar/tests/etc/wsgi_sqlalchemy_pooled.conf
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      381 2020-06-15 09:51:10.000000 zaqar-9.0.1/zaqar/tests/etc/wsgi_mongodb_pooled.conf
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      175 2020-06-15 09:51:10.000000 zaqar-9.0.1/zaqar/tests/etc/drivers_transport_invalid.conf
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       41 2020-06-15 09:51:10.000000 zaqar-9.0.1/zaqar/tests/etc/policy.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      448 2020-06-15 09:51:10.000000 zaqar-9.0.1/zaqar/tests/etc/websocket_mongodb_subscriptions.conf
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      188 2020-06-15 09:51:10.000000 zaqar-9.0.1/zaqar/tests/etc/drivers_storage_invalid.conf
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      228 2020-06-15 09:51:10.000000 zaqar-9.0.1/zaqar/tests/etc/wsgi_mongodb_validation.conf
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      100 2020-06-15 09:51:10.000000 zaqar-9.0.1/zaqar/tests/etc/wsgi_mongodb_default_limits.conf
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      473 2020-06-15 09:51:10.000000 zaqar-9.0.1/zaqar/tests/etc/wsgi_mongodb.conf
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      216 2020-06-15 09:51:10.000000 zaqar-9.0.1/zaqar/tests/etc/keystone_auth.conf
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      454 2020-06-15 09:51:10.000000 zaqar-9.0.1/zaqar/tests/etc/wsgi_redis.conf
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      452 2020-06-15 09:51:10.000000 zaqar-9.0.1/zaqar/tests/etc/wsgi_fifo_mongodb.conf
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      194 2020-06-15 09:51:10.000000 zaqar-9.0.1/zaqar/tests/etc/wsgi_faulty.conf
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      219 2020-06-15 09:51:10.000000 zaqar-9.0.1/zaqar/tests/etc/functional-tests.conf
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      382 2020-06-15 09:51:10.000000 zaqar-9.0.1/zaqar/tests/etc/wsgi_mongodb_pooled_disable_virtual_pool.conf
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      398 2020-06-15 09:51:10.000000 zaqar-9.0.1/zaqar/tests/etc/websocket_mongodb_keystone_auth.conf
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4210 2020-06-15 09:51:10.000000 zaqar-9.0.1/zaqar/tests/base.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      963 2020-06-15 09:51:10.000000 zaqar-9.0.1/zaqar/tests/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4645 2020-06-15 09:51:10.000000 zaqar-9.0.1/zaqar/tests/faulty_storage.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-15 09:53:07.000000 zaqar-9.0.1/zaqar/tests/unit/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-15 09:53:07.000000 zaqar-9.0.1/zaqar/tests/unit/hacking/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1160 2020-06-15 09:51:10.000000 zaqar-9.0.1/zaqar/tests/unit/hacking/test_hacking.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-06-15 09:51:10.000000 zaqar-9.0.1/zaqar/tests/unit/hacking/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-15 09:53:07.000000 zaqar-9.0.1/zaqar/tests/unit/storage/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5432 2020-06-15 09:51:10.000000 zaqar-9.0.1/zaqar/tests/unit/storage/test_pool_catalog_new.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2035 2020-06-15 09:51:10.000000 zaqar-9.0.1/zaqar/tests/unit/storage/test_impl_swift.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-15 09:53:07.000000 zaqar-9.0.1/zaqar/tests/unit/storage/sqlalchemy_migration/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3189 2020-06-15 09:51:10.000000 zaqar-9.0.1/zaqar/tests/unit/storage/sqlalchemy_migration/test_db_manage_cli.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6931 2020-06-15 09:51:10.000000 zaqar-9.0.1/zaqar/tests/unit/storage/sqlalchemy_migration/test_migrations_base.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-06-15 09:51:10.000000 zaqar-9.0.1/zaqar/tests/unit/storage/sqlalchemy_migration/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5529 2020-06-15 09:51:10.000000 zaqar-9.0.1/zaqar/tests/unit/storage/sqlalchemy_migration/test_migrations.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3350 2020-06-15 09:51:10.000000 zaqar-9.0.1/zaqar/tests/unit/storage/test_impl_sqlalchemy.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1067 2020-06-15 09:51:10.000000 zaqar-9.0.1/zaqar/tests/unit/storage/test_utils.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    82786 2020-06-15 09:51:10.000000 zaqar-9.0.1/zaqar/tests/unit/storage/base.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-06-15 09:51:10.000000 zaqar-9.0.1/zaqar/tests/unit/storage/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    22680 2020-06-15 09:51:10.000000 zaqar-9.0.1/zaqar/tests/unit/storage/test_impl_redis.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    23922 2020-06-15 09:51:10.000000 zaqar-9.0.1/zaqar/tests/unit/storage/test_impl_mongodb.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-15 09:53:07.000000 zaqar-9.0.1/zaqar/tests/unit/cmd/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1024 2020-06-15 09:51:10.000000 zaqar-9.0.1/zaqar/tests/unit/cmd/test_status.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-06-15 09:51:10.000000 zaqar-9.0.1/zaqar/tests/unit/cmd/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-15 09:53:07.000000 zaqar-9.0.1/zaqar/tests/unit/common/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4427 2020-06-15 09:51:10.000000 zaqar-9.0.1/zaqar/tests/unit/common/test_urls.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-15 09:53:07.000000 zaqar-9.0.1/zaqar/tests/unit/common/storage/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2358 2020-06-15 09:51:10.000000 zaqar-9.0.1/zaqar/tests/unit/common/storage/test_utils.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2663 2020-06-15 09:51:10.000000 zaqar-9.0.1/zaqar/tests/unit/common/storage/test_select.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-06-15 09:51:10.000000 zaqar-9.0.1/zaqar/tests/unit/common/storage/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5740 2020-06-15 09:51:10.000000 zaqar-9.0.1/zaqar/tests/unit/common/test_decorators.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1798 2020-06-15 09:51:10.000000 zaqar-9.0.1/zaqar/tests/unit/common/test_api.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1091 2020-06-15 09:51:10.000000 zaqar-9.0.1/zaqar/tests/unit/common/test_request.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2743 2020-06-15 09:51:10.000000 zaqar-9.0.1/zaqar/tests/unit/common/test_pipeline.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-06-15 09:51:10.000000 zaqar-9.0.1/zaqar/tests/unit/common/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-15 09:53:07.000000 zaqar-9.0.1/zaqar/tests/unit/transport/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-15 09:53:07.000000 zaqar-9.0.1/zaqar/tests/unit/transport/websocket/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1704 2020-06-15 09:51:10.000000 zaqar-9.0.1/zaqar/tests/unit/transport/websocket/utils.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4253 2020-06-15 09:51:10.000000 zaqar-9.0.1/zaqar/tests/unit/transport/websocket/test_protocol.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3046 2020-06-15 09:51:10.000000 zaqar-9.0.1/zaqar/tests/unit/transport/websocket/base.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-06-15 09:51:10.000000 zaqar-9.0.1/zaqar/tests/unit/transport/websocket/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-15 09:53:07.000000 zaqar-9.0.1/zaqar/tests/unit/transport/websocket/v2/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    16329 2020-06-15 09:51:10.000000 zaqar-9.0.1/zaqar/tests/unit/transport/websocket/v2/test_subscriptions.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    22743 2020-06-15 09:51:10.000000 zaqar-9.0.1/zaqar/tests/unit/transport/websocket/v2/test_queue_lifecycle.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    16459 2020-06-15 09:51:10.000000 zaqar-9.0.1/zaqar/tests/unit/transport/websocket/v2/test_claims.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10377 2020-06-15 09:51:10.000000 zaqar-9.0.1/zaqar/tests/unit/transport/websocket/v2/test_auth.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    21340 2020-06-15 09:51:10.000000 zaqar-9.0.1/zaqar/tests/unit/transport/websocket/v2/test_messages.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-06-15 09:51:10.000000 zaqar-9.0.1/zaqar/tests/unit/transport/websocket/v2/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1694 2020-06-15 09:51:10.000000 zaqar-9.0.1/zaqar/tests/unit/transport/test_acl.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-06-15 09:51:10.000000 zaqar-9.0.1/zaqar/tests/unit/transport/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-15 09:53:07.000000 zaqar-9.0.1/zaqar/tests/unit/transport/wsgi/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2293 2020-06-15 09:51:10.000000 zaqar-9.0.1/zaqar/tests/unit/transport/wsgi/test_version.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-15 09:53:07.000000 zaqar-9.0.1/zaqar/tests/unit/transport/wsgi/v1/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2230 2020-06-15 09:51:10.000000 zaqar-9.0.1/zaqar/tests/unit/transport/wsgi/v1/test_home.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4803 2020-06-15 09:51:10.000000 zaqar-9.0.1/zaqar/tests/unit/transport/wsgi/v1/test_validation.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3543 2020-06-15 09:51:10.000000 zaqar-9.0.1/zaqar/tests/unit/transport/wsgi/v1/test_default_limits.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    15395 2020-06-15 09:51:10.000000 zaqar-9.0.1/zaqar/tests/unit/transport/wsgi/v1/test_queue_lifecycle.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    13346 2020-06-15 09:51:10.000000 zaqar-9.0.1/zaqar/tests/unit/transport/wsgi/v1/test_pools.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10037 2020-06-15 09:51:10.000000 zaqar-9.0.1/zaqar/tests/unit/transport/wsgi/v1/test_claims.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3332 2020-06-15 09:51:10.000000 zaqar-9.0.1/zaqar/tests/unit/transport/wsgi/v1/test_media_type.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1392 2020-06-15 09:51:10.000000 zaqar-9.0.1/zaqar/tests/unit/transport/wsgi/v1/test_auth.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    19867 2020-06-15 09:51:10.000000 zaqar-9.0.1/zaqar/tests/unit/transport/wsgi/v1/test_messages.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-06-15 09:51:10.000000 zaqar-9.0.1/zaqar/tests/unit/transport/wsgi/v1/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1075 2020-06-15 09:51:10.000000 zaqar-9.0.1/zaqar/tests/unit/transport/wsgi/v1/test_health.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6728 2020-06-15 09:51:10.000000 zaqar-9.0.1/zaqar/tests/unit/transport/wsgi/test_utils.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-15 09:53:07.000000 zaqar-9.0.1/zaqar/tests/unit/transport/wsgi/v1_1/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2698 2020-06-15 09:51:10.000000 zaqar-9.0.1/zaqar/tests/unit/transport/wsgi/v1_1/test_home.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5055 2020-06-15 09:51:10.000000 zaqar-9.0.1/zaqar/tests/unit/transport/wsgi/v1_1/test_validation.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4757 2020-06-15 09:51:10.000000 zaqar-9.0.1/zaqar/tests/unit/transport/wsgi/v1_1/test_default_limits.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    14716 2020-06-15 09:51:10.000000 zaqar-9.0.1/zaqar/tests/unit/transport/wsgi/v1_1/test_queue_lifecycle.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    12566 2020-06-15 09:51:10.000000 zaqar-9.0.1/zaqar/tests/unit/transport/wsgi/v1_1/test_claims.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3295 2020-06-15 09:51:10.000000 zaqar-9.0.1/zaqar/tests/unit/transport/wsgi/v1_1/test_media_type.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1394 2020-06-15 09:51:10.000000 zaqar-9.0.1/zaqar/tests/unit/transport/wsgi/v1_1/test_auth.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1262 2020-06-15 09:51:10.000000 zaqar-9.0.1/zaqar/tests/unit/transport/wsgi/v1_1/test_ping.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    25148 2020-06-15 09:51:10.000000 zaqar-9.0.1/zaqar/tests/unit/transport/wsgi/v1_1/test_messages.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-06-15 09:51:10.000000 zaqar-9.0.1/zaqar/tests/unit/transport/wsgi/v1_1/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3098 2020-06-15 09:51:10.000000 zaqar-9.0.1/zaqar/tests/unit/transport/wsgi/v1_1/test_health.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5952 2020-06-15 09:51:10.000000 zaqar-9.0.1/zaqar/tests/unit/transport/wsgi/base.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-15 09:53:07.000000 zaqar-9.0.1/zaqar/tests/unit/transport/wsgi/v2_0/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2696 2020-06-15 09:51:10.000000 zaqar-9.0.1/zaqar/tests/unit/transport/wsgi/v2_0/test_home.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9557 2020-06-15 09:51:10.000000 zaqar-9.0.1/zaqar/tests/unit/transport/wsgi/v2_0/test_validation.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8903 2020-06-15 09:51:10.000000 zaqar-9.0.1/zaqar/tests/unit/transport/wsgi/v2_0/test_urls.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    19499 2020-06-15 09:51:10.000000 zaqar-9.0.1/zaqar/tests/unit/transport/wsgi/v2_0/test_subscriptions.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4755 2020-06-15 09:51:10.000000 zaqar-9.0.1/zaqar/tests/unit/transport/wsgi/v2_0/test_default_limits.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    25272 2020-06-15 09:51:10.000000 zaqar-9.0.1/zaqar/tests/unit/transport/wsgi/v2_0/test_queue_lifecycle.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    15771 2020-06-15 09:51:10.000000 zaqar-9.0.1/zaqar/tests/unit/transport/wsgi/v2_0/test_pools_new.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    12563 2020-06-15 09:51:10.000000 zaqar-9.0.1/zaqar/tests/unit/transport/wsgi/v2_0/test_claims.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    14155 2020-06-15 09:51:10.000000 zaqar-9.0.1/zaqar/tests/unit/transport/wsgi/v2_0/test_flavors_new.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3330 2020-06-15 09:51:10.000000 zaqar-9.0.1/zaqar/tests/unit/transport/wsgi/v2_0/test_media_type.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1392 2020-06-15 09:51:10.000000 zaqar-9.0.1/zaqar/tests/unit/transport/wsgi/v2_0/test_auth.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1256 2020-06-15 09:51:10.000000 zaqar-9.0.1/zaqar/tests/unit/transport/wsgi/v2_0/test_ping.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4778 2020-06-15 09:51:10.000000 zaqar-9.0.1/zaqar/tests/unit/transport/wsgi/v2_0/test_purge.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    28451 2020-06-15 09:51:10.000000 zaqar-9.0.1/zaqar/tests/unit/transport/wsgi/v2_0/test_messages.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-06-15 09:51:10.000000 zaqar-9.0.1/zaqar/tests/unit/transport/wsgi/v2_0/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    24210 2020-06-15 09:51:10.000000 zaqar-9.0.1/zaqar/tests/unit/transport/wsgi/v2_0/test_topic_lifecycle.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3094 2020-06-15 09:51:10.000000 zaqar-9.0.1/zaqar/tests/unit/transport/wsgi/v2_0/test_health.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      826 2020-06-15 09:51:10.000000 zaqar-9.0.1/zaqar/tests/unit/transport/wsgi/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2031 2020-06-15 09:51:10.000000 zaqar-9.0.1/zaqar/tests/unit/test_bootstrap.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-15 09:53:07.000000 zaqar-9.0.1/zaqar/tests/unit/notification/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    21777 2020-06-15 09:51:10.000000 zaqar-9.0.1/zaqar/tests/unit/notification/test_notifier.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-06-15 09:51:10.000000 zaqar-9.0.1/zaqar/tests/unit/notification/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-06-15 09:51:10.000000 zaqar-9.0.1/zaqar/tests/unit/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-15 09:53:07.000000 zaqar-9.0.1/zaqar/common/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      763 2020-06-15 09:51:10.000000 zaqar-9.0.1/zaqar/common/access.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4143 2020-06-15 09:51:10.000000 zaqar-9.0.1/zaqar/common/urls.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1481 2020-06-15 09:51:10.000000 zaqar-9.0.1/zaqar/common/cli.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-15 09:53:07.000000 zaqar-9.0.1/zaqar/common/storage/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1779 2020-06-15 09:51:10.000000 zaqar-9.0.1/zaqar/common/storage/select.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-06-15 09:51:10.000000 zaqar-9.0.1/zaqar/common/storage/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3160 2020-06-15 09:51:10.000000 zaqar-9.0.1/zaqar/common/auth.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2033 2020-06-15 09:51:10.000000 zaqar-9.0.1/zaqar/common/utils.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2350 2020-06-15 09:51:10.000000 zaqar-9.0.1/zaqar/common/consts.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      960 2020-06-15 09:51:10.000000 zaqar-9.0.1/zaqar/common/errors.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3976 2020-06-15 09:51:10.000000 zaqar-9.0.1/zaqar/common/pipeline.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-15 09:53:07.000000 zaqar-9.0.1/zaqar/common/transport/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-06-15 09:51:10.000000 zaqar-9.0.1/zaqar/common/transport/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-15 09:53:07.000000 zaqar-9.0.1/zaqar/common/transport/wsgi/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    11697 2020-06-15 09:51:10.000000 zaqar-9.0.1/zaqar/common/transport/wsgi/helpers.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-06-15 09:51:10.000000 zaqar-9.0.1/zaqar/common/transport/wsgi/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-15 09:53:07.000000 zaqar-9.0.1/zaqar/common/policies/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2172 2020-06-15 09:51:10.000000 zaqar-9.0.1/zaqar/common/policies/flavors.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2787 2020-06-15 09:51:10.000000 zaqar-9.0.1/zaqar/common/policies/topics.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2109 2020-06-15 09:51:10.000000 zaqar-9.0.1/zaqar/common/policies/pools.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2837 2020-06-15 09:51:10.000000 zaqar-9.0.1/zaqar/common/policies/subscription.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3175 2020-06-15 09:51:10.000000 zaqar-9.0.1/zaqar/common/policies/queues.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2367 2020-06-15 09:51:10.000000 zaqar-9.0.1/zaqar/common/policies/messages.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1305 2020-06-15 09:51:10.000000 zaqar-9.0.1/zaqar/common/policies/health.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      930 2020-06-15 09:51:10.000000 zaqar-9.0.1/zaqar/common/policies/base.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1260 2020-06-15 09:51:10.000000 zaqar-9.0.1/zaqar/common/policies/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2060 2020-06-15 09:51:10.000000 zaqar-9.0.1/zaqar/common/policies/claims.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7272 2020-06-15 09:51:10.000000 zaqar-9.0.1/zaqar/common/decorators.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      638 2020-06-15 09:51:10.000000 zaqar-9.0.1/zaqar/common/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      798 2020-06-15 09:51:10.000000 zaqar-9.0.1/zaqar/common/cache.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-15 09:53:07.000000 zaqar-9.0.1/zaqar/common/api/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-15 09:53:07.000000 zaqar-9.0.1/zaqar/common/api/schemas/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1647 2020-06-15 09:51:10.000000 zaqar-9.0.1/zaqar/common/api/schemas/flavors.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2102 2020-06-15 09:51:10.000000 zaqar-9.0.1/zaqar/common/api/schemas/pools.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-15 09:53:07.000000 zaqar-9.0.1/zaqar/common/api/schemas/v1_1/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1327 2020-06-15 09:51:10.000000 zaqar-9.0.1/zaqar/common/api/schemas/v1_1/flavors.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-06-15 09:51:10.000000 zaqar-9.0.1/zaqar/common/api/schemas/v1_1/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-06-15 09:51:10.000000 zaqar-9.0.1/zaqar/common/api/schemas/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1630 2020-06-15 09:51:10.000000 zaqar-9.0.1/zaqar/common/api/request.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7356 2020-06-15 09:51:10.000000 zaqar-9.0.1/zaqar/common/api/utils.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1254 2020-06-15 09:51:10.000000 zaqar-9.0.1/zaqar/common/api/errors.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1431 2020-06-15 09:51:10.000000 zaqar-9.0.1/zaqar/common/api/response.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2336 2020-06-15 09:51:10.000000 zaqar-9.0.1/zaqar/common/api/api.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-06-15 09:51:10.000000 zaqar-9.0.1/zaqar/common/api/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-15 09:53:07.000000 zaqar-9.0.1/zaqar/transport/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-15 09:53:07.000000 zaqar-9.0.1/zaqar/transport/middleware/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3703 2020-06-15 09:51:10.000000 zaqar-9.0.1/zaqar/transport/middleware/cors.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2036 2020-06-15 09:51:10.000000 zaqar-9.0.1/zaqar/transport/middleware/auth.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4563 2020-06-15 09:51:10.000000 zaqar-9.0.1/zaqar/transport/middleware/profile.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-06-15 09:51:10.000000 zaqar-9.0.1/zaqar/transport/middleware/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    29243 2020-06-15 09:51:10.000000 zaqar-9.0.1/zaqar/transport/validation.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1399 2020-06-15 09:51:10.000000 zaqar-9.0.1/zaqar/transport/acl.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1792 2020-06-15 09:51:10.000000 zaqar-9.0.1/zaqar/transport/utils.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-15 09:53:07.000000 zaqar-9.0.1/zaqar/transport/websocket/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4137 2020-06-15 09:51:10.000000 zaqar-9.0.1/zaqar/transport/websocket/driver.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2406 2020-06-15 09:51:10.000000 zaqar-9.0.1/zaqar/transport/websocket/factory.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10605 2020-06-15 09:51:10.000000 zaqar-9.0.1/zaqar/transport/websocket/protocol.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      717 2020-06-15 09:51:10.000000 zaqar-9.0.1/zaqar/transport/websocket/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2327 2020-06-15 09:51:10.000000 zaqar-9.0.1/zaqar/transport/base.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      671 2020-06-15 09:51:10.000000 zaqar-9.0.1/zaqar/transport/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-15 09:53:07.000000 zaqar-9.0.1/zaqar/transport/wsgi/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-15 09:53:07.000000 zaqar-9.0.1/zaqar/transport/wsgi/v1_0/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4656 2020-06-15 09:51:10.000000 zaqar-9.0.1/zaqar/transport/wsgi/v1_0/homedoc.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3648 2020-06-15 09:51:10.000000 zaqar-9.0.1/zaqar/transport/wsgi/v1_0/metadata.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7169 2020-06-15 09:51:10.000000 zaqar-9.0.1/zaqar/transport/wsgi/v1_0/pools.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4231 2020-06-15 09:51:10.000000 zaqar-9.0.1/zaqar/transport/wsgi/v1_0/queues.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10644 2020-06-15 09:51:10.000000 zaqar-9.0.1/zaqar/transport/wsgi/v1_0/messages.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      955 2020-06-15 09:51:10.000000 zaqar-9.0.1/zaqar/transport/wsgi/v1_0/health.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2374 2020-06-15 09:51:10.000000 zaqar-9.0.1/zaqar/transport/wsgi/v1_0/stats.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3443 2020-06-15 09:51:10.000000 zaqar-9.0.1/zaqar/transport/wsgi/v1_0/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6253 2020-06-15 09:51:10.000000 zaqar-9.0.1/zaqar/transport/wsgi/v1_0/claims.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1535 2020-06-15 09:51:10.000000 zaqar-9.0.1/zaqar/transport/wsgi/app.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7410 2020-06-15 09:51:10.000000 zaqar-9.0.1/zaqar/transport/wsgi/driver.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8327 2020-06-15 09:51:10.000000 zaqar-9.0.1/zaqar/transport/wsgi/utils.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3009 2020-06-15 09:51:10.000000 zaqar-9.0.1/zaqar/transport/wsgi/errors.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-15 09:53:07.000000 zaqar-9.0.1/zaqar/transport/wsgi/v1_1/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6383 2020-06-15 09:51:10.000000 zaqar-9.0.1/zaqar/transport/wsgi/v1_1/flavors.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      967 2020-06-15 09:51:10.000000 zaqar-9.0.1/zaqar/transport/wsgi/v1_1/ping.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9225 2020-06-15 09:51:10.000000 zaqar-9.0.1/zaqar/transport/wsgi/v1_1/homedoc.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7822 2020-06-15 09:51:10.000000 zaqar-9.0.1/zaqar/transport/wsgi/v1_1/pools.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5754 2020-06-15 09:51:10.000000 zaqar-9.0.1/zaqar/transport/wsgi/v1_1/queues.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    12899 2020-06-15 09:51:10.000000 zaqar-9.0.1/zaqar/transport/wsgi/v1_1/messages.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1268 2020-06-15 09:51:10.000000 zaqar-9.0.1/zaqar/transport/wsgi/v1_1/health.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2382 2020-06-15 09:51:10.000000 zaqar-9.0.1/zaqar/transport/wsgi/v1_1/stats.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4113 2020-06-15 09:51:10.000000 zaqar-9.0.1/zaqar/transport/wsgi/v1_1/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7289 2020-06-15 09:51:10.000000 zaqar-9.0.1/zaqar/transport/wsgi/v1_1/claims.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-15 09:53:07.000000 zaqar-9.0.1/zaqar/transport/wsgi/v2_0/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3410 2020-06-15 09:51:10.000000 zaqar-9.0.1/zaqar/transport/wsgi/v2_0/purge.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    14359 2020-06-15 09:51:10.000000 zaqar-9.0.1/zaqar/transport/wsgi/v2_0/flavors.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1178 2020-06-15 09:51:10.000000 zaqar-9.0.1/zaqar/transport/wsgi/v2_0/ping.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    12611 2020-06-15 09:51:10.000000 zaqar-9.0.1/zaqar/transport/wsgi/v2_0/homedoc.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2659 2020-06-15 09:51:10.000000 zaqar-9.0.1/zaqar/transport/wsgi/v2_0/urls.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    13096 2020-06-15 09:51:10.000000 zaqar-9.0.1/zaqar/transport/wsgi/v2_0/subscriptions.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3335 2020-06-15 09:51:10.000000 zaqar-9.0.1/zaqar/transport/wsgi/v2_0/topic_purge.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8847 2020-06-15 09:51:10.000000 zaqar-9.0.1/zaqar/transport/wsgi/v2_0/pools.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    13099 2020-06-15 09:51:10.000000 zaqar-9.0.1/zaqar/transport/wsgi/v2_0/queues.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    15541 2020-06-15 09:51:10.000000 zaqar-9.0.1/zaqar/transport/wsgi/v2_0/messages.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1411 2020-06-15 09:51:10.000000 zaqar-9.0.1/zaqar/transport/wsgi/v2_0/health.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2533 2020-06-15 09:51:10.000000 zaqar-9.0.1/zaqar/transport/wsgi/v2_0/stats.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7265 2020-06-15 09:51:10.000000 zaqar-9.0.1/zaqar/transport/wsgi/v2_0/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2533 2020-06-15 09:51:10.000000 zaqar-9.0.1/zaqar/transport/wsgi/v2_0/topic_stats.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7457 2020-06-15 09:51:10.000000 zaqar-9.0.1/zaqar/transport/wsgi/v2_0/claims.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    12928 2020-06-15 09:51:10.000000 zaqar-9.0.1/zaqar/transport/wsgi/v2_0/topic.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      670 2020-06-15 09:51:10.000000 zaqar-9.0.1/zaqar/transport/wsgi/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1075 2020-06-15 09:51:10.000000 zaqar-9.0.1/zaqar/transport/wsgi/version.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-15 09:53:07.000000 zaqar-9.0.1/zaqar/locale/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-15 09:53:07.000000 zaqar-9.0.1/zaqar/locale/en_GB/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-15 09:53:07.000000 zaqar-9.0.1/zaqar/locale/en_GB/LC_MESSAGES/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    23462 2020-06-15 09:51:10.000000 zaqar-9.0.1/zaqar/locale/en_GB/LC_MESSAGES/zaqar.po
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-15 09:53:07.000000 zaqar-9.0.1/zaqar/locale/id/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-15 09:53:07.000000 zaqar-9.0.1/zaqar/locale/id/LC_MESSAGES/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    24198 2020-06-15 09:51:10.000000 zaqar-9.0.1/zaqar/locale/id/LC_MESSAGES/zaqar.po
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-15 09:53:07.000000 zaqar-9.0.1/zaqar/locale/es/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-15 09:53:07.000000 zaqar-9.0.1/zaqar/locale/es/LC_MESSAGES/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    12000 2020-06-15 09:51:10.000000 zaqar-9.0.1/zaqar/locale/es/LC_MESSAGES/zaqar.po
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-15 09:53:07.000000 zaqar-9.0.1/zaqar/locale/de/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-15 09:53:07.000000 zaqar-9.0.1/zaqar/locale/de/LC_MESSAGES/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    28473 2020-06-15 09:51:10.000000 zaqar-9.0.1/zaqar/locale/de/LC_MESSAGES/zaqar.po
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      906 2020-06-15 09:51:10.000000 zaqar-9.0.1/zaqar/i18n.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-15 09:53:07.000000 zaqar-9.0.1/zaqar/notification/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7190 2020-06-15 09:51:10.000000 zaqar-9.0.1/zaqar/notification/notifier.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-15 09:53:07.000000 zaqar-9.0.1/zaqar/notification/tasks/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6916 2020-06-15 09:51:10.000000 zaqar-9.0.1/zaqar/notification/tasks/webhook.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2272 2020-06-15 09:51:10.000000 zaqar-9.0.1/zaqar/notification/tasks/trust.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6137 2020-06-15 09:51:10.000000 zaqar-9.0.1/zaqar/notification/tasks/mailto.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-06-15 09:51:10.000000 zaqar-9.0.1/zaqar/notification/tasks/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-06-15 09:51:10.000000 zaqar-9.0.1/zaqar/notification/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      743 2020-06-15 09:51:10.000000 zaqar-9.0.1/zaqar/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2050 2020-06-15 09:51:10.000000 zaqar-9.0.1/zaqar/version.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4719 2020-06-15 09:51:10.000000 zaqar-9.0.1/zaqar/bootstrap.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-15 09:53:07.000000 zaqar-9.0.1/zaqar/api/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4843 2020-06-15 09:51:10.000000 zaqar-9.0.1/zaqar/api/handler.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-15 09:53:07.000000 zaqar-9.0.1/zaqar/api/v1/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    13196 2020-06-15 09:51:10.000000 zaqar-9.0.1/zaqar/api/v1/request.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    11400 2020-06-15 09:51:10.000000 zaqar-9.0.1/zaqar/api/v1/response.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-06-15 09:51:10.000000 zaqar-9.0.1/zaqar/api/v1/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-15 09:53:07.000000 zaqar-9.0.1/zaqar/api/v1_1/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8354 2020-06-15 09:51:10.000000 zaqar-9.0.1/zaqar/api/v1_1/request.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    15593 2020-06-15 09:51:10.000000 zaqar-9.0.1/zaqar/api/v1_1/response.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-06-15 09:51:10.000000 zaqar-9.0.1/zaqar/api/v1_1/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-06-15 09:51:10.000000 zaqar-9.0.1/zaqar/api/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-15 09:53:07.000000 zaqar-9.0.1/zaqar/api/v2/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4417 2020-06-15 09:51:10.000000 zaqar-9.0.1/zaqar/api/v2/request.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    37805 2020-06-15 09:51:10.000000 zaqar-9.0.1/zaqar/api/v2/endpoints.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    15561 2020-06-15 09:51:10.000000 zaqar-9.0.1/zaqar/api/v2/response.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-06-15 09:51:10.000000 zaqar-9.0.1/zaqar/api/v2/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      835 2020-06-15 09:51:10.000000 zaqar-9.0.1/test-requirements.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       84 2020-06-15 09:51:10.000000 zaqar-9.0.1/.stestr.conf
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4269 2020-06-15 09:51:10.000000 zaqar-9.0.1/HACKING.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-15 09:53:07.000000 zaqar-9.0.1/zaqar.egg-info/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2020-06-15 09:53:07.000000 zaqar-9.0.1/zaqar.egg-info/dependency_links.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        6 2020-06-15 09:53:07.000000 zaqar-9.0.1/zaqar.egg-info/top_level.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      719 2020-06-15 09:53:07.000000 zaqar-9.0.1/zaqar.egg-info/requires.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3970 2020-06-15 09:53:07.000000 zaqar-9.0.1/zaqar.egg-info/PKG-INFO
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2020-06-15 09:53:07.000000 zaqar-9.0.1/zaqar.egg-info/not-zip-safe
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    23101 2020-06-15 09:53:07.000000 zaqar-9.0.1/zaqar.egg-info/SOURCES.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2066 2020-06-15 09:53:07.000000 zaqar-9.0.1/zaqar.egg-info/entry_points.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       47 2020-06-15 09:53:07.000000 zaqar-9.0.1/zaqar.egg-info/pbr.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      541 2020-06-15 09:51:10.000000 zaqar-9.0.1/CONTRIBUTING.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-15 09:53:07.000000 zaqar-9.0.1/doc/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       31 2020-06-15 09:51:10.000000 zaqar-9.0.1/doc/README.md
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      514 2020-06-15 09:51:10.000000 zaqar-9.0.1/doc/requirements.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-15 09:53:07.000000 zaqar-9.0.1/doc/source/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-15 09:53:07.000000 zaqar-9.0.1/doc/source/contributor/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4934 2020-06-15 09:51:10.000000 zaqar-9.0.1/doc/source/contributor/first_review.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6249 2020-06-15 09:51:10.000000 zaqar-9.0.1/doc/source/contributor/project_info.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5145 2020-06-15 09:51:10.000000 zaqar-9.0.1/doc/source/contributor/running_tests.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8439 2020-06-15 09:51:10.000000 zaqar-9.0.1/doc/source/contributor/development.environment.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      124 2020-06-15 09:51:10.000000 zaqar-9.0.1/doc/source/contributor/transport.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10773 2020-06-15 09:51:10.000000 zaqar-9.0.1/doc/source/contributor/first_patch.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1159 2020-06-15 09:51:10.000000 zaqar-9.0.1/doc/source/contributor/gerrit.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1099 2020-06-15 09:51:10.000000 zaqar-9.0.1/doc/source/contributor/index.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3310 2020-06-15 09:51:10.000000 zaqar-9.0.1/doc/source/contributor/test_suite.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8623 2020-06-15 09:51:10.000000 zaqar-9.0.1/doc/source/contributor/welcome.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6258 2020-06-15 09:51:10.000000 zaqar-9.0.1/doc/source/contributor/reviewer_guide.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-15 09:53:07.000000 zaqar-9.0.1/doc/source/contributor/images/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    77939 2020-06-15 09:51:10.000000 zaqar-9.0.1/doc/source/contributor/images/zaqar_review_id.png
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1803 2020-06-15 09:51:10.000000 zaqar-9.0.1/doc/source/contributor/launchpad.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1409 2020-06-15 09:51:10.000000 zaqar-9.0.1/doc/source/contributor/jenkins.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      490 2020-06-15 09:51:10.000000 zaqar-9.0.1/doc/source/contributor/storage.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-15 09:53:07.000000 zaqar-9.0.1/doc/source/install/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1161 2020-06-15 09:51:10.000000 zaqar-9.0.1/doc/source/install/install.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    20636 2020-06-15 09:51:10.000000 zaqar-9.0.1/doc/source/install/install-rdo.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      239 2020-06-15 09:51:10.000000 zaqar-9.0.1/doc/source/install/next-steps.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1564 2020-06-15 09:51:10.000000 zaqar-9.0.1/doc/source/install/index.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1321 2020-06-15 09:51:10.000000 zaqar-9.0.1/doc/source/install/verify.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2673 2020-06-15 09:51:10.000000 zaqar-9.0.1/doc/source/install/get_started.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    20622 2020-06-15 09:51:10.000000 zaqar-9.0.1/doc/source/install/install-obs.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    20158 2020-06-15 09:51:10.000000 zaqar-9.0.1/doc/source/install/install-ubuntu.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3934 2020-06-15 09:51:10.000000 zaqar-9.0.1/doc/source/index.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-15 09:53:07.000000 zaqar-9.0.1/doc/source/_static/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-06-15 09:51:10.000000 zaqar-9.0.1/doc/source/_static/.placeholder
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-15 09:53:07.000000 zaqar-9.0.1/doc/source/user/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2760 2020-06-15 09:51:10.000000 zaqar-9.0.1/doc/source/user/notification_delivery_policy.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      189 2020-06-15 09:51:10.000000 zaqar-9.0.1/doc/source/user/index.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    12321 2020-06-15 09:51:10.000000 zaqar-9.0.1/doc/source/user/headers_queue_api_working.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    11218 2020-06-15 09:51:10.000000 zaqar-9.0.1/doc/source/user/getting_started.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3347 2020-06-15 09:51:10.000000 zaqar-9.0.1/doc/source/user/send_request_api.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1541 2020-06-15 09:51:10.000000 zaqar-9.0.1/doc/source/user/authentication_tokens.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3352 2020-06-15 09:51:10.000000 zaqar-9.0.1/doc/source/glossary.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-15 09:53:07.000000 zaqar-9.0.1/doc/source/configuration/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      123 2020-06-15 09:51:10.000000 zaqar-9.0.1/doc/source/configuration/zaqar.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      387 2020-06-15 09:51:10.000000 zaqar-9.0.1/doc/source/configuration/index.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6574 2020-06-15 09:51:10.000000 zaqar-9.0.1/doc/source/configuration/configuring.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      509 2020-06-15 09:51:10.000000 zaqar-9.0.1/doc/source/configuration/sample-configuration.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7940 2020-06-15 09:51:10.000000 zaqar-9.0.1/doc/source/conf.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-15 09:53:07.000000 zaqar-9.0.1/doc/source/admin/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      195 2020-06-15 09:51:10.000000 zaqar-9.0.1/doc/source/admin/index.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    12144 2020-06-15 09:51:10.000000 zaqar-9.0.1/doc/source/admin/subscription_confirm.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3835 2020-06-15 09:51:10.000000 zaqar-9.0.1/doc/source/admin/CORS.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3421 2020-06-15 09:51:10.000000 zaqar-9.0.1/doc/source/admin/gmr.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8000 2020-06-15 09:51:10.000000 zaqar-9.0.1/doc/source/admin/writing_pipeline_stages.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4557 2020-06-15 09:51:10.000000 zaqar-9.0.1/doc/source/admin/OSprofiler.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6367 2020-06-15 09:51:10.000000 zaqar-9.0.1/doc/source/admin/running_benchmark.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-15 09:53:07.000000 zaqar-9.0.1/doc/source/cli/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       75 2020-06-15 09:51:10.000000 zaqar-9.0.1/doc/source/cli/index.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1752 2020-06-15 09:51:10.000000 zaqar-9.0.1/doc/source/cli/zaqar-status.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-15 09:53:07.000000 zaqar-9.0.1/tools/
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)     1186 2020-06-15 09:51:10.000000 zaqar-9.0.1/tools/test-setup.sh
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-15 09:53:07.000000 zaqar-9.0.1/tools/doc/
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)     1020 2020-06-15 09:51:10.000000 zaqar-9.0.1/tools/doc/generate_autodoc_index.sh
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)      490 2020-06-15 09:51:10.000000 zaqar-9.0.1/tools/doc/find_autodoc_modules.sh
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3284 2020-06-15 09:53:07.000000 zaqar-9.0.1/setup.cfg
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-15 09:53:07.000000 zaqar-9.0.1/etc/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      133 2020-06-15 09:51:10.000000 zaqar-9.0.1/etc/uwsgi.conf
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      908 2020-06-15 09:51:10.000000 zaqar-9.0.1/etc/logging.conf.sample
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      321 2020-06-15 09:51:10.000000 zaqar-9.0.1/etc/README-policy.json.sample
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      144 2020-06-15 09:51:10.000000 zaqar-9.0.1/etc/zaqar-benchmark.conf.sample
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       71 2020-06-15 09:51:10.000000 zaqar-9.0.1/etc/zaqar-policy-generator.conf
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3015 2020-06-15 09:51:10.000000 zaqar-9.0.1/etc/zaqar-benchmark-messages.json
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-15 09:53:07.000000 zaqar-9.0.1/etc/oslo-config-generator/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      298 2020-06-15 09:51:10.000000 zaqar-9.0.1/etc/oslo-config-generator/zaqar.conf
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1259 2020-06-15 09:51:10.000000 zaqar-9.0.1/requirements.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8446 2020-06-15 09:53:07.000000 zaqar-9.0.1/AUTHORS
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-15 09:53:07.000000 zaqar-9.0.1/rally-jobs/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-15 09:53:07.000000 zaqar-9.0.1/rally-jobs/plugins/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-06-15 09:51:10.000000 zaqar-9.0.1/rally-jobs/plugins/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      403 2020-06-15 09:51:10.000000 zaqar-9.0.1/rally-jobs/plugins/README.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      305 2020-06-15 09:51:10.000000 zaqar-9.0.1/rally-jobs/zaqar-zaqar.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-15 09:53:07.000000 zaqar-9.0.1/rally-jobs/extra/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      185 2020-06-15 09:51:10.000000 zaqar-9.0.1/rally-jobs/extra/README.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      882 2020-06-15 09:51:10.000000 zaqar-9.0.1/rally-jobs/README.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-15 09:53:07.000000 zaqar-9.0.1/releasenotes/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-15 09:53:07.000000 zaqar-9.0.1/releasenotes/notes/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      398 2020-06-15 09:51:10.000000 zaqar-9.0.1/releasenotes/notes/support-turnoff-deprecated-versions-44656aeb8ebb8881.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       75 2020-06-15 09:51:10.000000 zaqar-9.0.1/releasenotes/notes/support-cors-af8349382a44aa0d.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      474 2020-06-15 09:51:10.000000 zaqar-9.0.1/releasenotes/notes/remove-format-contraint-of-client-id-ab787960df6e1606.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      384 2020-06-15 09:51:10.000000 zaqar-9.0.1/releasenotes/notes/support_dead_letter_queue-c8b7303319e7f920.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      269 2020-06-15 09:51:10.000000 zaqar-9.0.1/releasenotes/notes/Integrate-OSprofiler-with-zaqar-59d0dc3d0326947d.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      275 2020-06-15 09:51:10.000000 zaqar-9.0.1/releasenotes/notes/support_delayed_queues-1babcaa3f056a39d.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      164 2020-06-15 09:51:10.000000 zaqar-9.0.1/releasenotes/notes/remove_pool_group_from_zaqar-f8eafeed21779959.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      282 2020-06-15 09:51:10.000000 zaqar-9.0.1/releasenotes/notes/sql_init-c9b3883241631f24.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      244 2020-06-15 09:51:10.000000 zaqar-9.0.1/releasenotes/notes/return_reserved_metdata_for_dead_letter_queue-da160301f6d8cfa4.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      479 2020-06-15 09:51:10.000000 zaqar-9.0.1/releasenotes/notes/support_md5_of_body-84c1cdc6809b6417.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      226 2020-06-15 09:51:10.000000 zaqar-9.0.1/releasenotes/notes/delete_messages_with_claim_ids-64bb8105de3768b1.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      196 2020-06-15 09:51:10.000000 zaqar-9.0.1/releasenotes/notes/queue-filter-support-b704a1c27f7473b9.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      573 2020-06-15 09:51:10.000000 zaqar-9.0.1/releasenotes/notes/add-a-notifier-using-trust-271d9cd1d2b4cdeb.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      333 2020-06-15 09:51:10.000000 zaqar-9.0.1/releasenotes/notes/support-more-backoff-functions-41e02a5977341576.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      401 2020-06-15 09:51:10.000000 zaqar-9.0.1/releasenotes/notes/show_default_attributes_for_queue-3d87333752484c87.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      326 2020-06-15 09:51:10.000000 zaqar-9.0.1/releasenotes/notes/user_ipv6_sockets-1e1b436de6b81ae3.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      484 2020-06-15 09:51:10.000000 zaqar-9.0.1/releasenotes/notes/webhook_subscription_confirmation-883cb7f325885ef0.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      431 2020-06-15 09:51:10.000000 zaqar-9.0.1/releasenotes/notes/introduce-topic-resource-9b40674cac06bdc2.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      278 2020-06-15 09:51:10.000000 zaqar-9.0.1/releasenotes/notes/deprecate-v11-976cccc1b56a28e7.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      366 2020-06-15 09:51:10.000000 zaqar-9.0.1/releasenotes/notes/lazy-queues-in-subscriptions-6bade4a1b8eca3e5.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      238 2020-06-15 09:51:10.000000 zaqar-9.0.1/releasenotes/notes/fix-detailed-queue-without-reserved-metadata-b53857ed9821fe76.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      328 2020-06-15 09:51:10.000000 zaqar-9.0.1/releasenotes/notes/email-notification-by-internal-tool-08910ab2247c3864.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-06-15 09:51:10.000000 zaqar-9.0.1/releasenotes/notes/.gitignore
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       84 2020-06-15 09:51:10.000000 zaqar-9.0.1/releasenotes/notes/support-dot-in-queue-name-bd2b3d523f55451f.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      462 2020-06-15 09:51:10.000000 zaqar-9.0.1/releasenotes/notes/zaqar-status-upgrade-check-framework-09caa1f741f6119d.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      294 2020-06-15 09:51:10.000000 zaqar-9.0.1/releasenotes/notes/support_password_configure_for_redis_connection-6f169db73ca80416.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      213 2020-06-15 09:51:10.000000 zaqar-9.0.1/releasenotes/notes/fix_subscription_limit-c3cdc9385825285a.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      297 2020-06-15 09:51:10.000000 zaqar-9.0.1/releasenotes/notes/introduce-guru-to-zaqar-ac7b51c764503829.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      318 2020-06-15 09:51:10.000000 zaqar-9.0.1/releasenotes/notes/allow-configuration-of-websocket-notification-fa542fbf761378d3.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      269 2020-06-15 09:51:10.000000 zaqar-9.0.1/releasenotes/notes/configuration-refactor-0ff219ac59c96347.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      231 2020-06-15 09:51:10.000000 zaqar-9.0.1/releasenotes/notes/remove-pool-group-00f2e69682c48131.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      245 2020-06-15 09:51:10.000000 zaqar-9.0.1/releasenotes/notes/fix_auth_issue_for_root_path-b15e1c4e92e4e8b1.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      302 2020-06-15 09:51:10.000000 zaqar-9.0.1/releasenotes/notes/add-swift-backend-4eb9b43913f39d18.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      225 2020-06-15 09:51:10.000000 zaqar-9.0.1/releasenotes/notes/remove-pool-group-totally-062ecfccd90a6725.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      872 2020-06-15 09:51:10.000000 zaqar-9.0.1/releasenotes/notes/subscription-confirmation-support-email-0c2a56cfedc5d1e2.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      229 2020-06-15 09:51:10.000000 zaqar-9.0.1/releasenotes/notes/support-redis-as-management-storage-backend-a205e3c4c4d01584.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       79 2020-06-15 09:51:10.000000 zaqar-9.0.1/releasenotes/notes/sqlalchemy-migration-6b4eaebb6e02a449.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      250 2020-06-15 09:51:10.000000 zaqar-9.0.1/releasenotes/notes/support-notification-delivery-policy-fbc94083b4e6b8d0.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      211 2020-06-15 09:51:10.000000 zaqar-9.0.1/releasenotes/notes/purge-queue-6788a249ee59d55a.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-15 09:53:07.000000 zaqar-9.0.1/releasenotes/source/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      188 2020-06-15 09:51:10.000000 zaqar-9.0.1/releasenotes/source/index.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-15 09:53:07.000000 zaqar-9.0.1/releasenotes/source/_static/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-06-15 09:51:10.000000 zaqar-9.0.1/releasenotes/source/_static/.gitignore
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      154 2020-06-15 09:51:10.000000 zaqar-9.0.1/releasenotes/source/mitaka.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      147 2020-06-15 09:51:10.000000 zaqar-9.0.1/releasenotes/source/queens.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-15 09:53:07.000000 zaqar-9.0.1/releasenotes/source/_templates/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-06-15 09:51:10.000000 zaqar-9.0.1/releasenotes/source/_templates/.gitignore
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      154 2020-06-15 09:51:10.000000 zaqar-9.0.1/releasenotes/source/newton.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      145 2020-06-15 09:51:10.000000 zaqar-9.0.1/releasenotes/source/stein.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      152 2020-06-15 09:51:10.000000 zaqar-9.0.1/releasenotes/source/ocata.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8921 2020-06-15 09:51:10.000000 zaqar-9.0.1/releasenotes/source/conf.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      145 2020-06-15 09:51:10.000000 zaqar-9.0.1/releasenotes/source/rocky.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      112 2020-06-15 09:51:10.000000 zaqar-9.0.1/releasenotes/source/unreleased.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      146 2020-06-15 09:51:10.000000 zaqar-9.0.1/releasenotes/source/liberty.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      143 2020-06-15 09:51:10.000000 zaqar-9.0.1/releasenotes/source/pike.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-15 09:53:07.000000 zaqar-9.0.1/devstack/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1811 2020-06-15 09:51:10.000000 zaqar-9.0.1/devstack/settings
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)    11746 2020-06-15 09:51:10.000000 zaqar-9.0.1/devstack/plugin.sh
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-15 09:53:07.000000 zaqar-9.0.1/devstack/gate/
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)     2147 2020-06-15 09:51:10.000000 zaqar-9.0.1/devstack/gate/gate_hook.sh
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)     1550 2020-06-15 09:51:10.000000 zaqar-9.0.1/devstack/gate/post_test_hook.sh
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-15 09:53:07.000000 zaqar-9.0.1/devstack/upgrade/
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)     3381 2020-06-15 09:51:10.000000 zaqar-9.0.1/devstack/upgrade/upgrade.sh
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)     1400 2020-06-15 09:51:10.000000 zaqar-9.0.1/devstack/upgrade/resource.sh
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      810 2020-06-15 09:51:10.000000 zaqar-9.0.1/devstack/upgrade/settings
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)      539 2020-06-15 09:51:10.000000 zaqar-9.0.1/devstack/upgrade/shutdown.sh
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      619 2020-06-15 09:51:10.000000 zaqar-9.0.1/devstack/README.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-15 09:53:07.000000 zaqar-9.0.1/playbooks/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-15 09:53:07.000000 zaqar-9.0.1/playbooks/legacy/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-15 09:53:07.000000 zaqar-9.0.1/playbooks/legacy/grenade-devstack-zaqar-base/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      411 2020-06-15 09:51:10.000000 zaqar-9.0.1/playbooks/legacy/grenade-devstack-zaqar-base/post.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2702 2020-06-15 09:51:10.000000 zaqar-9.0.1/playbooks/legacy/grenade-devstack-zaqar-base/run.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-15 09:53:07.000000 zaqar-9.0.1/playbooks/legacy/rally-dsvm-zaqar-zaqar/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1207 2020-06-15 09:51:10.000000 zaqar-9.0.1/playbooks/legacy/rally-dsvm-zaqar-zaqar/post.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8435 2020-06-15 09:51:10.000000 zaqar-9.0.1/playbooks/legacy/rally-dsvm-zaqar-zaqar/run.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-15 09:53:07.000000 zaqar-9.0.1/playbooks/legacy/tempest-devstack-zaqar-base/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2409 2020-06-15 09:51:10.000000 zaqar-9.0.1/playbooks/legacy/tempest-devstack-zaqar-base/post.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1984 2020-06-15 09:51:10.000000 zaqar-9.0.1/playbooks/legacy/tempest-devstack-zaqar-base/run.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-15 09:53:07.000000 zaqar-9.0.1/zaqar_upgradetests/
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-15 09:51:10.000000 zaqar-9.0.1/zaqar_upgradetests/pre_test_hook.sh
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-15 09:51:10.000000 zaqar-9.0.1/zaqar_upgradetests/post_test_hook.sh
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       93 2020-06-15 09:51:10.000000 zaqar-9.0.1/bench-requirements.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      364 2020-06-15 09:51:10.000000 zaqar-9.0.1/AUTHORS.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1377 2020-06-15 09:51:10.000000 zaqar-9.0.1/lower-constraints.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-15 09:53:07.000000 zaqar-9.0.1/samples/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-15 09:53:07.000000 zaqar-9.0.1/samples/html/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4639 2020-06-15 09:51:10.000000 zaqar-9.0.1/samples/html/unsubscriptionConfirmation.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5117 2020-06-15 09:51:10.000000 zaqar-9.0.1/samples/html/subscriptionConfirmation.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3009 2020-06-15 09:51:10.000000 zaqar-9.0.1/samples/html/confirmation_web_service_sample.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-15 09:53:07.000000 zaqar-9.0.1/samples/zaqar/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7995 2020-06-15 09:51:10.000000 zaqar-9.0.1/samples/zaqar/sendmail.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2491 2020-06-15 09:51:10.000000 zaqar-9.0.1/samples/zaqar/subscriber_service_sample.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-15 09:53:07.000000 zaqar-9.0.1/samples/nodejs/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-15 09:53:07.000000 zaqar-9.0.1/samples/nodejs/receive_message/
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)     1283 2020-06-15 09:51:10.000000 zaqar-9.0.1/samples/nodejs/receive_message/zaqar_sample.js
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-15 09:53:07.000000 zaqar-9.0.1/samples/nodejs/send_message/
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)     1175 2020-06-15 09:51:10.000000 zaqar-9.0.1/samples/nodejs/send_message/zaqar_sample.js
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-15 09:53:07.000000 zaqar-9.0.1/samples/javascript/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-15 09:53:07.000000 zaqar-9.0.1/samples/javascript/receive_message/
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)     1232 2020-06-15 09:51:10.000000 zaqar-9.0.1/samples/javascript/receive_message/zaqar_sample.js
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-15 09:53:07.000000 zaqar-9.0.1/samples/javascript/send_message/
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)     1137 2020-06-15 09:51:10.000000 zaqar-9.0.1/samples/javascript/send_message/zaqar_sample.js
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    12471 2020-06-15 09:51:10.000000 zaqar-9.0.1/samples/javascript/websocket.html
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-15 09:53:07.000000 zaqar-9.0.1/samples/jaxrs/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-15 09:53:07.000000 zaqar-9.0.1/samples/jaxrs/receive_message/
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)     2017 2020-06-15 09:51:10.000000 zaqar-9.0.1/samples/jaxrs/receive_message/SampleZaqarServlet.java
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-15 09:53:07.000000 zaqar-9.0.1/samples/jaxrs/send_message/
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)     1987 2020-06-15 09:51:10.000000 zaqar-9.0.1/samples/jaxrs/send_message/SampleZaqarServlet.java
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-15 09:53:07.000000 zaqar-9.0.1/samples/python-zaqarclient/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-15 09:53:07.000000 zaqar-9.0.1/samples/python-zaqarclient/receive_message/
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)     1091 2020-06-15 09:51:10.000000 zaqar-9.0.1/samples/python-zaqarclient/receive_message/zaqar_sample.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-15 09:53:07.000000 zaqar-9.0.1/samples/python-zaqarclient/send_message/
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)     1031 2020-06-15 09:51:10.000000 zaqar-9.0.1/samples/python-zaqarclient/send_message/zaqar_sample.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-15 09:53:07.000000 zaqar-9.0.1/samples/java-api-for-websocket/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-15 09:53:07.000000 zaqar-9.0.1/samples/java-api-for-websocket/receive_message/
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)     2141 2020-06-15 09:51:10.000000 zaqar-9.0.1/samples/java-api-for-websocket/receive_message/SampleZaqarEndpoint.java
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)     1215 2020-06-15 09:51:10.000000 zaqar-9.0.1/samples/java-api-for-websocket/receive_message/JsonDecoder.java
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-06-15 09:53:07.000000 zaqar-9.0.1/samples/java-api-for-websocket/send_message/
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)     1783 2020-06-15 09:51:10.000000 zaqar-9.0.1/samples/java-api-for-websocket/send_message/SampleZaqarEndpoint.java
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4008 2020-06-15 09:51:10.000000 zaqar-9.0.1/.zuul.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2494 2020-06-15 09:51:10.000000 zaqar-9.0.1/README.rst
```

### Comparing `zaqar-9.0.0.0rc1/PKG-INFO` & `zaqar-9.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: zaqar
-Version: 9.0.0.0rc1
+Version: 9.0.1
 Summary: OpenStack Queuing and Notification Service
 Home-page: https://docs.openstack.org/zaqar/latest/
 Author: OpenStack
 Author-email: openstack-discuss@lists.openstack.org
 License: UNKNOWN
 Description: ========================
         Team and repository tags
```

### Comparing `zaqar-9.0.0.0rc1/etc/zaqar-benchmark-messages.json` & `zaqar-9.0.1/etc/zaqar-benchmark-messages.json`

 * *Files identical despite different names*

### Comparing `zaqar-9.0.0.0rc1/etc/logging.conf.sample` & `zaqar-9.0.1/etc/logging.conf.sample`

 * *Files identical despite different names*

### Comparing `zaqar-9.0.0.0rc1/setup.py` & `zaqar-9.0.1/setup.py`

 * *Files identical despite different names*

### Comparing `zaqar-9.0.0.0rc1/LICENSE` & `zaqar-9.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `zaqar-9.0.0.0rc1/setup.cfg` & `zaqar-9.0.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `zaqar-9.0.0.0rc1/doc/source/conf.py` & `zaqar-9.0.1/doc/source/conf.py`

 * *Files identical despite different names*

### Comparing `zaqar-9.0.0.0rc1/doc/source/user/getting_started.rst` & `zaqar-9.0.1/doc/source/user/getting_started.rst`

 * *Files identical despite different names*

### Comparing `zaqar-9.0.0.0rc1/doc/source/user/send_request_api.rst` & `zaqar-9.0.1/doc/source/user/send_request_api.rst`

 * *Files identical despite different names*

### Comparing `zaqar-9.0.0.0rc1/doc/source/user/authentication_tokens.rst` & `zaqar-9.0.1/doc/source/user/authentication_tokens.rst`

 * *Files identical despite different names*

### Comparing `zaqar-9.0.0.0rc1/doc/source/user/headers_queue_api_working.rst` & `zaqar-9.0.1/doc/source/user/headers_queue_api_working.rst`

 * *Files identical despite different names*

### Comparing `zaqar-9.0.0.0rc1/doc/source/user/notification_delivery_policy.rst` & `zaqar-9.0.1/doc/source/user/notification_delivery_policy.rst`

 * *Files identical despite different names*

### Comparing `zaqar-9.0.0.0rc1/doc/source/index.rst` & `zaqar-9.0.1/doc/source/index.rst`

 * *Files identical despite different names*

### Comparing `zaqar-9.0.0.0rc1/doc/source/cli/zaqar-status.rst` & `zaqar-9.0.1/doc/source/cli/zaqar-status.rst`

 * *Files identical despite different names*

### Comparing `zaqar-9.0.0.0rc1/doc/source/admin/running_benchmark.rst` & `zaqar-9.0.1/doc/source/admin/running_benchmark.rst`

 * *Files identical despite different names*

### Comparing `zaqar-9.0.0.0rc1/doc/source/admin/CORS.rst` & `zaqar-9.0.1/doc/source/admin/CORS.rst`

 * *Files identical despite different names*

### Comparing `zaqar-9.0.0.0rc1/doc/source/admin/subscription_confirm.rst` & `zaqar-9.0.1/doc/source/admin/subscription_confirm.rst`

 * *Files identical despite different names*

### Comparing `zaqar-9.0.0.0rc1/doc/source/admin/gmr.rst` & `zaqar-9.0.1/doc/source/admin/gmr.rst`

 * *Files identical despite different names*

### Comparing `zaqar-9.0.0.0rc1/doc/source/admin/writing_pipeline_stages.rst` & `zaqar-9.0.1/doc/source/admin/writing_pipeline_stages.rst`

 * *Files identical despite different names*

### Comparing `zaqar-9.0.0.0rc1/doc/source/admin/OSprofiler.rst` & `zaqar-9.0.1/doc/source/admin/OSprofiler.rst`

 * *Files identical despite different names*

### Comparing `zaqar-9.0.0.0rc1/doc/source/install/install-ubuntu.rst` & `zaqar-9.0.1/doc/source/install/install-ubuntu.rst`

 * *Files identical despite different names*

### Comparing `zaqar-9.0.0.0rc1/doc/source/install/index.rst` & `zaqar-9.0.1/doc/source/install/index.rst`

 * *Files identical despite different names*

### Comparing `zaqar-9.0.0.0rc1/doc/source/install/install-rdo.rst` & `zaqar-9.0.1/doc/source/install/install-rdo.rst`

 * *Files identical despite different names*

### Comparing `zaqar-9.0.0.0rc1/doc/source/install/install.rst` & `zaqar-9.0.1/doc/source/install/install.rst`

 * *Files identical despite different names*

### Comparing `zaqar-9.0.0.0rc1/doc/source/install/get_started.rst` & `zaqar-9.0.1/doc/source/install/get_started.rst`

 * *Files identical despite different names*

### Comparing `zaqar-9.0.0.0rc1/doc/source/install/verify.rst` & `zaqar-9.0.1/doc/source/install/verify.rst`

 * *Files identical despite different names*

### Comparing `zaqar-9.0.0.0rc1/doc/source/install/install-obs.rst` & `zaqar-9.0.1/doc/source/install/install-obs.rst`

 * *Files identical despite different names*

### Comparing `zaqar-9.0.0.0rc1/doc/source/contributor/welcome.rst` & `zaqar-9.0.1/doc/source/contributor/welcome.rst`

 * *Files identical despite different names*

### Comparing `zaqar-9.0.0.0rc1/doc/source/contributor/first_review.rst` & `zaqar-9.0.1/doc/source/contributor/first_review.rst`

 * *Files identical despite different names*

### Comparing `zaqar-9.0.0.0rc1/doc/source/contributor/development.environment.rst` & `zaqar-9.0.1/doc/source/contributor/development.environment.rst`

 * *Files identical despite different names*

### Comparing `zaqar-9.0.0.0rc1/doc/source/contributor/test_suite.rst` & `zaqar-9.0.1/doc/source/contributor/test_suite.rst`

 * *Files identical despite different names*

### Comparing `zaqar-9.0.0.0rc1/doc/source/contributor/project_info.rst` & `zaqar-9.0.1/doc/source/contributor/project_info.rst`

 * *Files identical despite different names*

### Comparing `zaqar-9.0.0.0rc1/doc/source/contributor/first_patch.rst` & `zaqar-9.0.1/doc/source/contributor/first_patch.rst`

 * *Files identical despite different names*

### Comparing `zaqar-9.0.0.0rc1/doc/source/contributor/launchpad.rst` & `zaqar-9.0.1/doc/source/contributor/launchpad.rst`

 * *Files identical despite different names*

### Comparing `zaqar-9.0.0.0rc1/doc/source/contributor/reviewer_guide.rst` & `zaqar-9.0.1/doc/source/contributor/reviewer_guide.rst`

 * *Files identical despite different names*

### Comparing `zaqar-9.0.0.0rc1/doc/source/contributor/running_tests.rst` & `zaqar-9.0.1/doc/source/contributor/running_tests.rst`

 * *Files identical despite different names*

### Comparing `zaqar-9.0.0.0rc1/doc/source/contributor/index.rst` & `zaqar-9.0.1/doc/source/contributor/index.rst`

 * *Files identical despite different names*

### Comparing `zaqar-9.0.0.0rc1/doc/source/contributor/jenkins.rst` & `zaqar-9.0.1/doc/source/contributor/jenkins.rst`

 * *Files identical despite different names*

### Comparing `zaqar-9.0.0.0rc1/doc/source/contributor/gerrit.rst` & `zaqar-9.0.1/doc/source/contributor/gerrit.rst`

 * *Files identical despite different names*

### Comparing `zaqar-9.0.0.0rc1/doc/source/contributor/images/zaqar_review_id.png` & `zaqar-9.0.1/doc/source/contributor/images/zaqar_review_id.png`

 * *Files identical despite different names*

### Comparing `zaqar-9.0.0.0rc1/doc/source/configuration/configuring.rst` & `zaqar-9.0.1/doc/source/configuration/configuring.rst`

 * *Files identical despite different names*

### Comparing `zaqar-9.0.0.0rc1/doc/source/glossary.rst` & `zaqar-9.0.1/doc/source/glossary.rst`

 * *Files identical despite different names*

### Comparing `zaqar-9.0.0.0rc1/doc/requirements.txt` & `zaqar-9.0.1/doc/requirements.txt`

 * *Files identical despite different names*

### Comparing `zaqar-9.0.0.0rc1/bindep.txt` & `zaqar-9.0.1/bindep.txt`

 * *Files identical despite different names*

### Comparing `zaqar-9.0.0.0rc1/samples/java-api-for-websocket/receive_message/SampleZaqarEndpoint.java` & `zaqar-9.0.1/samples/java-api-for-websocket/receive_message/SampleZaqarEndpoint.java`

 * *Files identical despite different names*

### Comparing `zaqar-9.0.0.0rc1/samples/java-api-for-websocket/receive_message/JsonDecoder.java` & `zaqar-9.0.1/samples/java-api-for-websocket/receive_message/JsonDecoder.java`

 * *Files identical despite different names*

### Comparing `zaqar-9.0.0.0rc1/samples/java-api-for-websocket/send_message/SampleZaqarEndpoint.java` & `zaqar-9.0.1/samples/java-api-for-websocket/send_message/SampleZaqarEndpoint.java`

 * *Files identical despite different names*

### Comparing `zaqar-9.0.0.0rc1/samples/html/confirmation_web_service_sample.py` & `zaqar-9.0.1/samples/html/confirmation_web_service_sample.py`

 * *Files identical despite different names*

### Comparing `zaqar-9.0.0.0rc1/samples/html/unsubscriptionConfirmation.html` & `zaqar-9.0.1/samples/html/unsubscriptionConfirmation.html`

 * *Files identical despite different names*

### Comparing `zaqar-9.0.0.0rc1/samples/html/subscriptionConfirmation.html` & `zaqar-9.0.1/samples/html/subscriptionConfirmation.html`

 * *Files identical despite different names*

### Comparing `zaqar-9.0.0.0rc1/samples/python-zaqarclient/receive_message/zaqar_sample.py` & `zaqar-9.0.1/samples/python-zaqarclient/receive_message/zaqar_sample.py`

 * *Files identical despite different names*

### Comparing `zaqar-9.0.0.0rc1/samples/python-zaqarclient/send_message/zaqar_sample.py` & `zaqar-9.0.1/samples/python-zaqarclient/send_message/zaqar_sample.py`

 * *Files identical despite different names*

### Comparing `zaqar-9.0.0.0rc1/samples/zaqar/sendmail.py` & `zaqar-9.0.1/samples/zaqar/sendmail.py`

 * *Files identical despite different names*

### Comparing `zaqar-9.0.0.0rc1/samples/zaqar/subscriber_service_sample.py` & `zaqar-9.0.1/samples/zaqar/subscriber_service_sample.py`

 * *Files identical despite different names*

### Comparing `zaqar-9.0.0.0rc1/samples/jaxrs/receive_message/SampleZaqarServlet.java` & `zaqar-9.0.1/samples/jaxrs/receive_message/SampleZaqarServlet.java`

 * *Files identical despite different names*

### Comparing `zaqar-9.0.0.0rc1/samples/jaxrs/send_message/SampleZaqarServlet.java` & `zaqar-9.0.1/samples/jaxrs/send_message/SampleZaqarServlet.java`

 * *Files identical despite different names*

### Comparing `zaqar-9.0.0.0rc1/samples/nodejs/receive_message/zaqar_sample.js` & `zaqar-9.0.1/samples/nodejs/receive_message/zaqar_sample.js`

 * *Files identical despite different names*

### Comparing `zaqar-9.0.0.0rc1/samples/nodejs/send_message/zaqar_sample.js` & `zaqar-9.0.1/samples/nodejs/send_message/zaqar_sample.js`

 * *Files identical despite different names*

### Comparing `zaqar-9.0.0.0rc1/samples/javascript/receive_message/zaqar_sample.js` & `zaqar-9.0.1/samples/javascript/receive_message/zaqar_sample.js`

 * *Files identical despite different names*

### Comparing `zaqar-9.0.0.0rc1/samples/javascript/websocket.html` & `zaqar-9.0.1/samples/javascript/websocket.html`

 * *Files identical despite different names*

### Comparing `zaqar-9.0.0.0rc1/samples/javascript/send_message/zaqar_sample.js` & `zaqar-9.0.1/samples/javascript/send_message/zaqar_sample.js`

 * *Files identical despite different names*

### Comparing `zaqar-9.0.0.0rc1/CONTRIBUTING.rst` & `zaqar-9.0.1/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `zaqar-9.0.0.0rc1/.zuul.yaml` & `zaqar-9.0.1/.zuul.yaml`

 * *Files identical despite different names*

### Comparing `zaqar-9.0.0.0rc1/playbooks/legacy/grenade-devstack-zaqar-base/run.yaml` & `zaqar-9.0.1/playbooks/legacy/grenade-devstack-zaqar-base/run.yaml`

 * *Files identical despite different names*

### Comparing `zaqar-9.0.0.0rc1/playbooks/legacy/rally-dsvm-zaqar-zaqar/run.yaml` & `zaqar-9.0.1/playbooks/legacy/rally-dsvm-zaqar-zaqar/run.yaml`

 * *Files identical despite different names*

### Comparing `zaqar-9.0.0.0rc1/playbooks/legacy/rally-dsvm-zaqar-zaqar/post.yaml` & `zaqar-9.0.1/playbooks/legacy/rally-dsvm-zaqar-zaqar/post.yaml`

 * *Files identical despite different names*

### Comparing `zaqar-9.0.0.0rc1/playbooks/legacy/tempest-devstack-zaqar-base/run.yaml` & `zaqar-9.0.1/playbooks/legacy/tempest-devstack-zaqar-base/run.yaml`

 * *Files identical despite different names*

### Comparing `zaqar-9.0.0.0rc1/playbooks/legacy/tempest-devstack-zaqar-base/post.yaml` & `zaqar-9.0.1/playbooks/legacy/tempest-devstack-zaqar-base/post.yaml`

 * *Files identical despite different names*

### Comparing `zaqar-9.0.0.0rc1/api-ref/source/conf.py` & `zaqar-9.0.1/api-ref/source/conf.py`

 * *Files identical despite different names*

### Comparing `zaqar-9.0.0.0rc1/api-ref/source/subscription.inc` & `zaqar-9.0.1/api-ref/source/subscription.inc`

 * *Files identical despite different names*

### Comparing `zaqar-9.0.0.0rc1/api-ref/source/messages.inc` & `zaqar-9.0.1/api-ref/source/messages.inc`

 * *Files identical despite different names*

### Comparing `zaqar-9.0.0.0rc1/api-ref/source/versions.inc` & `zaqar-9.0.1/api-ref/source/versions.inc`

 * *Files identical despite different names*

### Comparing `zaqar-9.0.0.0rc1/api-ref/source/health.inc` & `zaqar-9.0.1/api-ref/source/health.inc`

 * *Files identical despite different names*

### Comparing `zaqar-9.0.0.0rc1/api-ref/source/flavors.inc` & `zaqar-9.0.1/api-ref/source/flavors.inc`

 * *Files identical despite different names*

### Comparing `zaqar-9.0.0.0rc1/api-ref/source/samples/messages-list-response.json` & `zaqar-9.0.1/api-ref/source/samples/messages-list-response.json`

 * *Files identical despite different names*

### Comparing `zaqar-9.0.0.0rc1/api-ref/source/samples/subscriptions-list-response.json` & `zaqar-9.0.1/api-ref/source/samples/subscriptions-list-response.json`

 * *Files identical despite different names*

### Comparing `zaqar-9.0.0.0rc1/api-ref/source/samples/health-response.json` & `zaqar-9.0.1/api-ref/source/samples/health-response.json`

 * *Files identical despite different names*

### Comparing `zaqar-9.0.0.0rc1/api-ref/source/samples/versions-list-response.json` & `zaqar-9.0.1/api-ref/source/samples/versions-list-response.json`

 * *Files identical despite different names*

### Comparing `zaqar-9.0.0.0rc1/api-ref/source/index.rst` & `zaqar-9.0.1/api-ref/source/index.rst`

 * *Files identical despite different names*

### Comparing `zaqar-9.0.0.0rc1/api-ref/source/queues.inc` & `zaqar-9.0.1/api-ref/source/queues.inc`

 * *Files identical despite different names*

### Comparing `zaqar-9.0.0.0rc1/api-ref/source/status.yaml` & `zaqar-9.0.1/api-ref/source/status.yaml`

 * *Files identical despite different names*

### Comparing `zaqar-9.0.0.0rc1/api-ref/source/pools.inc` & `zaqar-9.0.1/api-ref/source/pools.inc`

 * *Files identical despite different names*

### Comparing `zaqar-9.0.0.0rc1/api-ref/source/claims.inc` & `zaqar-9.0.1/api-ref/source/claims.inc`

 * *Files identical despite different names*

### Comparing `zaqar-9.0.0.0rc1/api-ref/source/parameters.yaml` & `zaqar-9.0.1/api-ref/source/parameters.yaml`

 * *Files identical despite different names*

### Comparing `zaqar-9.0.0.0rc1/rally-jobs/README.rst` & `zaqar-9.0.1/rally-jobs/README.rst`

 * *Files identical despite different names*

### Comparing `zaqar-9.0.0.0rc1/releasenotes/notes/add-a-notifier-using-trust-271d9cd1d2b4cdeb.yaml` & `zaqar-9.0.1/releasenotes/notes/add-a-notifier-using-trust-271d9cd1d2b4cdeb.yaml`

 * *Files identical despite different names*

### Comparing `zaqar-9.0.0.0rc1/releasenotes/notes/subscription-confirmation-support-email-0c2a56cfedc5d1e2.yaml` & `zaqar-9.0.1/releasenotes/notes/subscription-confirmation-support-email-0c2a56cfedc5d1e2.yaml`

 * *Files identical despite different names*

### Comparing `zaqar-9.0.0.0rc1/releasenotes/source/conf.py` & `zaqar-9.0.1/releasenotes/source/conf.py`

 * *Files identical despite different names*

### Comparing `zaqar-9.0.0.0rc1/devstack/upgrade/shutdown.sh` & `zaqar-9.0.1/devstack/upgrade/shutdown.sh`

 * *Files identical despite different names*

### Comparing `zaqar-9.0.0.0rc1/devstack/upgrade/resource.sh` & `zaqar-9.0.1/devstack/upgrade/resource.sh`

 * *Files identical despite different names*

### Comparing `zaqar-9.0.0.0rc1/devstack/upgrade/upgrade.sh` & `zaqar-9.0.1/devstack/upgrade/upgrade.sh`

 * *Files identical despite different names*

### Comparing `zaqar-9.0.0.0rc1/devstack/upgrade/settings` & `zaqar-9.0.1/devstack/upgrade/settings`

 * *Files identical despite different names*

### Comparing `zaqar-9.0.0.0rc1/devstack/plugin.sh` & `zaqar-9.0.1/devstack/plugin.sh`

 * *Files identical despite different names*

### Comparing `zaqar-9.0.0.0rc1/devstack/settings` & `zaqar-9.0.1/devstack/settings`

 * *Files identical despite different names*

### Comparing `zaqar-9.0.0.0rc1/devstack/README.rst` & `zaqar-9.0.1/devstack/README.rst`

 * *Files identical despite different names*

### Comparing `zaqar-9.0.0.0rc1/devstack/gate/post_test_hook.sh` & `zaqar-9.0.1/devstack/gate/post_test_hook.sh`

 * *Files identical despite different names*

### Comparing `zaqar-9.0.0.0rc1/devstack/gate/gate_hook.sh` & `zaqar-9.0.1/devstack/gate/gate_hook.sh`

 * *Files identical despite different names*

### Comparing `zaqar-9.0.0.0rc1/AUTHORS` & `zaqar-9.0.1/AUTHORS`

 * *Files identical despite different names*

### Comparing `zaqar-9.0.0.0rc1/tox.ini` & `zaqar-9.0.1/tox.ini`

 * *Files 4% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 setenv = VIRTUAL_ENV={envdir}
          ZAQAR_TESTS_CONFIGS_DIR={toxinidir}/zaqar/tests/etc/
          ZAQAR_TEST_MONGODB=1
          ZAQAR_TEST_SLOW=1
          OS_STDOUT_CAPTURE=1
          OS_STDERR_CAPTURE=1
          OS_TEST_TIMEOUT=60
-deps = -c{env:UPPER_CONSTRAINTS_FILE:https://releases.openstack.org/constraints/upper/master}
+deps = -c{env:UPPER_CONSTRAINTS_FILE:https://releases.openstack.org/constraints/upper/train}
        -r{toxinidir}/requirements.txt
        -r{toxinidir}/test-requirements.txt
 commands =
     find . -type f -name "*.pyc" -delete
     stestr run --serial --slowest {posargs}
 whitelist_externals = find
 
@@ -58,41 +58,41 @@
 [testenv:venv]
 basepython = python3
 commands = {posargs}
 
 [testenv:docs]
 basepython = python3
 deps =
-    -c{env:UPPER_CONSTRAINTS_FILE:https://releases.openstack.org/constraints/upper/master}
+    -c{env:UPPER_CONSTRAINTS_FILE:https://releases.openstack.org/constraints/upper/train}
     -r{toxinidir}/doc/requirements.txt
 commands =
     sphinx-build -W -b html doc/source doc/build/html
 
 [testenv:api-ref]
 basepython = python3
 # This environment is called from CI scripts to test and publish
 # the API Ref to docs.openstack.org.
 #
 whitelist_externals = bash
                       rm
 deps =
-    -c{env:UPPER_CONSTRAINTS_FILE:https://releases.openstack.org/constraints/upper/master}
+    -c{env:UPPER_CONSTRAINTS_FILE:https://releases.openstack.org/constraints/upper/train}
     -r{toxinidir}/doc/requirements.txt
 commands =
     rm -rf api-ref/build
     sphinx-build -W -b html -d api-ref/build/doctrees api-ref/source api-ref/build/html
 
 [testenv:debug]
 basepython = python3
 commands = oslo_debug_helper {posargs}
 
 [testenv:releasenotes]
 basepython = python3
 deps =
-    -c{env:UPPER_CONSTRAINTS_FILE:https://releases.openstack.org/constraints/upper/master}
+    -c{env:UPPER_CONSTRAINTS_FILE:https://releases.openstack.org/constraints/upper/train}
     -r{toxinidir}/doc/requirements.txt
 commands =
     doc8 releasenotes/source releasenotes/notes
     sphinx-build -a -E -d releasenotes/build/doctrees -b html releasenotes/source releasenotes/build/html
 
 [flake8]
 exclude = .venv*,.git,.tox,dist,doc,*lib/python*,*.egg,.update-venv
```

### Comparing `zaqar-9.0.0.0rc1/zaqar/notification/tasks/webhook.py` & `zaqar-9.0.1/zaqar/notification/tasks/webhook.py`

 * *Files identical despite different names*

### Comparing `zaqar-9.0.0.0rc1/zaqar/notification/tasks/mailto.py` & `zaqar-9.0.1/zaqar/notification/tasks/mailto.py`

 * *Files identical despite different names*

### Comparing `zaqar-9.0.0.0rc1/zaqar/notification/tasks/trust.py` & `zaqar-9.0.1/zaqar/notification/tasks/trust.py`

 * *Files identical despite different names*

### Comparing `zaqar-9.0.0.0rc1/zaqar/notification/notifier.py` & `zaqar-9.0.1/zaqar/notification/notifier.py`

 * *Files identical despite different names*

### Comparing `zaqar-9.0.0.0rc1/zaqar/bench/config.py` & `zaqar-9.0.1/zaqar/bench/config.py`

 * *Files identical despite different names*

### Comparing `zaqar-9.0.0.0rc1/zaqar/bench/helpers.py` & `zaqar-9.0.1/zaqar/bench/helpers.py`

 * *Files identical despite different names*

### Comparing `zaqar-9.0.0.0rc1/zaqar/bench/conductor.py` & `zaqar-9.0.1/zaqar/bench/conductor.py`

 * *Files identical despite different names*

### Comparing `zaqar-9.0.0.0rc1/zaqar/bench/consumer.py` & `zaqar-9.0.1/zaqar/bench/consumer.py`

 * *Files identical despite different names*

### Comparing `zaqar-9.0.0.0rc1/zaqar/bench/producer.py` & `zaqar-9.0.1/zaqar/bench/producer.py`

 * *Files identical despite different names*

### Comparing `zaqar-9.0.0.0rc1/zaqar/bench/observer.py` & `zaqar-9.0.1/zaqar/bench/observer.py`

 * *Files identical despite different names*

### Comparing `zaqar-9.0.0.0rc1/zaqar/common/cache.py` & `zaqar-9.0.1/zaqar/common/cache.py`

 * *Files identical despite different names*

### Comparing `zaqar-9.0.0.0rc1/zaqar/common/pipeline.py` & `zaqar-9.0.1/zaqar/common/pipeline.py`

 * *Files identical despite different names*

### Comparing `zaqar-9.0.0.0rc1/zaqar/common/errors.py` & `zaqar-9.0.1/zaqar/common/errors.py`

 * *Files identical despite different names*

### Comparing `zaqar-9.0.0.0rc1/zaqar/common/urls.py` & `zaqar-9.0.1/zaqar/common/urls.py`

 * *Files identical despite different names*

### Comparing `zaqar-9.0.0.0rc1/zaqar/common/access.py` & `zaqar-9.0.1/zaqar/common/access.py`

 * *Files identical despite different names*

### Comparing `zaqar-9.0.0.0rc1/zaqar/common/auth.py` & `zaqar-9.0.1/zaqar/common/auth.py`

 * *Files identical despite different names*

### Comparing `zaqar-9.0.0.0rc1/zaqar/common/__init__.py` & `zaqar-9.0.1/zaqar/common/__init__.py`

 * *Files identical despite different names*

### Comparing `zaqar-9.0.0.0rc1/zaqar/common/api/errors.py` & `zaqar-9.0.1/zaqar/common/api/errors.py`

 * *Files identical despite different names*

### Comparing `zaqar-9.0.0.0rc1/zaqar/common/api/response.py` & `zaqar-9.0.1/zaqar/common/api/response.py`

 * *Files identical despite different names*

### Comparing `zaqar-9.0.0.0rc1/zaqar/common/api/api.py` & `zaqar-9.0.1/zaqar/common/api/api.py`

 * *Files identical despite different names*

### Comparing `zaqar-9.0.0.0rc1/zaqar/common/api/schemas/pools.py` & `zaqar-9.0.1/zaqar/common/api/schemas/pools.py`

 * *Files identical despite different names*

### Comparing `zaqar-9.0.0.0rc1/zaqar/common/api/schemas/v1_1/flavors.py` & `zaqar-9.0.1/zaqar/common/api/schemas/v1_1/flavors.py`

 * *Files identical despite different names*

### Comparing `zaqar-9.0.0.0rc1/zaqar/common/api/schemas/flavors.py` & `zaqar-9.0.1/zaqar/common/api/schemas/flavors.py`

 * *Files identical despite different names*

### Comparing `zaqar-9.0.0.0rc1/zaqar/common/api/request.py` & `zaqar-9.0.1/zaqar/common/api/request.py`

 * *Files identical despite different names*

### Comparing `zaqar-9.0.0.0rc1/zaqar/common/api/utils.py` & `zaqar-9.0.1/zaqar/common/api/utils.py`

 * *Files identical despite different names*

### Comparing `zaqar-9.0.0.0rc1/zaqar/common/cli.py` & `zaqar-9.0.1/zaqar/common/cli.py`

 * *Files identical despite different names*

### Comparing `zaqar-9.0.0.0rc1/zaqar/common/storage/select.py` & `zaqar-9.0.1/zaqar/common/storage/select.py`

 * *Files identical despite different names*

### Comparing `zaqar-9.0.0.0rc1/zaqar/common/transport/wsgi/helpers.py` & `zaqar-9.0.1/zaqar/common/transport/wsgi/helpers.py`

 * *Files identical despite different names*

### Comparing `zaqar-9.0.0.0rc1/zaqar/common/consts.py` & `zaqar-9.0.1/zaqar/common/consts.py`

 * *Files identical despite different names*

### Comparing `zaqar-9.0.0.0rc1/zaqar/common/policies/pools.py` & `zaqar-9.0.1/zaqar/common/policies/pools.py`

 * *Files identical despite different names*

### Comparing `zaqar-9.0.0.0rc1/zaqar/common/policies/claims.py` & `zaqar-9.0.1/zaqar/common/policies/claims.py`

 * *Files identical despite different names*

### Comparing `zaqar-9.0.0.0rc1/zaqar/common/policies/queues.py` & `zaqar-9.0.1/zaqar/common/policies/queues.py`

 * *Files identical despite different names*

### Comparing `zaqar-9.0.0.0rc1/zaqar/common/policies/messages.py` & `zaqar-9.0.1/zaqar/common/policies/messages.py`

 * *Files identical despite different names*

### Comparing `zaqar-9.0.0.0rc1/zaqar/common/policies/health.py` & `zaqar-9.0.1/zaqar/common/policies/health.py`

 * *Files identical despite different names*

### Comparing `zaqar-9.0.0.0rc1/zaqar/common/policies/__init__.py` & `zaqar-9.0.1/zaqar/common/policies/__init__.py`

 * *Files identical despite different names*

### Comparing `zaqar-9.0.0.0rc1/zaqar/common/policies/base.py` & `zaqar-9.0.1/zaqar/common/policies/base.py`

 * *Files identical despite different names*

### Comparing `zaqar-9.0.0.0rc1/zaqar/common/policies/topics.py` & `zaqar-9.0.1/zaqar/common/policies/topics.py`

 * *Files identical despite different names*

### Comparing `zaqar-9.0.0.0rc1/zaqar/common/policies/subscription.py` & `zaqar-9.0.1/zaqar/common/policies/subscription.py`

 * *Files identical despite different names*

### Comparing `zaqar-9.0.0.0rc1/zaqar/common/policies/flavors.py` & `zaqar-9.0.1/zaqar/common/policies/flavors.py`

 * *Files identical despite different names*

### Comparing `zaqar-9.0.0.0rc1/zaqar/common/decorators.py` & `zaqar-9.0.1/zaqar/common/decorators.py`

 * *Files identical despite different names*

### Comparing `zaqar-9.0.0.0rc1/zaqar/common/utils.py` & `zaqar-9.0.1/zaqar/common/utils.py`

 * *Files identical despite different names*

### Comparing `zaqar-9.0.0.0rc1/zaqar/conf/drivers_management_store_mongodb.py` & `zaqar-9.0.1/zaqar/conf/drivers_management_store_mongodb.py`

 * *Files identical despite different names*

### Comparing `zaqar-9.0.0.0rc1/zaqar/conf/drivers_transport_websocket.py` & `zaqar-9.0.1/zaqar/conf/drivers_transport_websocket.py`

 * *Files identical despite different names*

### Comparing `zaqar-9.0.0.0rc1/zaqar/conf/transport.py` & `zaqar-9.0.1/zaqar/conf/transport.py`

 * *Files identical despite different names*

### Comparing `zaqar-9.0.0.0rc1/zaqar/conf/pooling_catalog.py` & `zaqar-9.0.1/zaqar/conf/pooling_catalog.py`

 * *Files identical despite different names*

### Comparing `zaqar-9.0.0.0rc1/zaqar/conf/profiler.py` & `zaqar-9.0.1/zaqar/conf/profiler.py`

 * *Files identical despite different names*

### Comparing `zaqar-9.0.0.0rc1/zaqar/conf/drivers.py` & `zaqar-9.0.1/zaqar/conf/drivers.py`

 * *Files identical despite different names*

### Comparing `zaqar-9.0.0.0rc1/zaqar/conf/__init__.py` & `zaqar-9.0.1/zaqar/conf/__init__.py`

 * *Files identical despite different names*

### Comparing `zaqar-9.0.0.0rc1/zaqar/conf/default.py` & `zaqar-9.0.1/zaqar/conf/default.py`

 * *Files identical despite different names*

### Comparing `zaqar-9.0.0.0rc1/zaqar/conf/drivers_management_store_sqlalchemy.py` & `zaqar-9.0.1/zaqar/conf/drivers_management_store_sqlalchemy.py`

 * *Files identical despite different names*

### Comparing `zaqar-9.0.0.0rc1/zaqar/conf/drivers_message_store_redis.py` & `zaqar-9.0.1/zaqar/conf/drivers_message_store_redis.py`

 * *Files identical despite different names*

### Comparing `zaqar-9.0.0.0rc1/zaqar/conf/drivers_management_store_redis.py` & `zaqar-9.0.1/zaqar/conf/drivers_management_store_redis.py`

 * *Files identical despite different names*

### Comparing `zaqar-9.0.0.0rc1/zaqar/conf/notification.py` & `zaqar-9.0.1/zaqar/conf/notification.py`

 * *Files identical despite different names*

### Comparing `zaqar-9.0.0.0rc1/zaqar/conf/signed_url.py` & `zaqar-9.0.1/zaqar/conf/signed_url.py`

 * *Files identical despite different names*

### Comparing `zaqar-9.0.0.0rc1/zaqar/conf/drivers_transport_wsgi.py` & `zaqar-9.0.1/zaqar/conf/drivers_transport_wsgi.py`

 * *Files identical despite different names*

### Comparing `zaqar-9.0.0.0rc1/zaqar/conf/storage.py` & `zaqar-9.0.1/zaqar/conf/storage.py`

 * *Files identical despite different names*

### Comparing `zaqar-9.0.0.0rc1/zaqar/conf/drivers_message_store_swift.py` & `zaqar-9.0.1/zaqar/conf/drivers_message_store_swift.py`

 * *Files identical despite different names*

### Comparing `zaqar-9.0.0.0rc1/zaqar/conf/drivers_message_store_mongodb.py` & `zaqar-9.0.1/zaqar/conf/drivers_message_store_mongodb.py`

 * *Files identical despite different names*

### Comparing `zaqar-9.0.0.0rc1/zaqar/conf/opts.py` & `zaqar-9.0.1/zaqar/conf/opts.py`

 * *Files identical despite different names*

### Comparing `zaqar-9.0.0.0rc1/zaqar/version.py` & `zaqar-9.0.1/zaqar/version.py`

 * *Files identical despite different names*

### Comparing `zaqar-9.0.0.0rc1/zaqar/__init__.py` & `zaqar-9.0.1/zaqar/__init__.py`

 * *Files identical despite different names*

### Comparing `zaqar-9.0.0.0rc1/zaqar/api/v1/response.py` & `zaqar-9.0.1/zaqar/api/v1/response.py`

 * *Files identical despite different names*

### Comparing `zaqar-9.0.0.0rc1/zaqar/api/v1/request.py` & `zaqar-9.0.1/zaqar/api/v1/request.py`

 * *Files identical despite different names*

### Comparing `zaqar-9.0.0.0rc1/zaqar/api/v1_1/response.py` & `zaqar-9.0.1/zaqar/api/v1_1/response.py`

 * *Files identical despite different names*

### Comparing `zaqar-9.0.0.0rc1/zaqar/api/v1_1/request.py` & `zaqar-9.0.1/zaqar/api/v1_1/request.py`

 * *Files identical despite different names*

### Comparing `zaqar-9.0.0.0rc1/zaqar/api/handler.py` & `zaqar-9.0.1/zaqar/api/handler.py`

 * *Files identical despite different names*

### Comparing `zaqar-9.0.0.0rc1/zaqar/api/v2/endpoints.py` & `zaqar-9.0.1/zaqar/api/v2/endpoints.py`

 * *Files identical despite different names*

### Comparing `zaqar-9.0.0.0rc1/zaqar/api/v2/response.py` & `zaqar-9.0.1/zaqar/api/v2/response.py`

 * *Files identical despite different names*

### Comparing `zaqar-9.0.0.0rc1/zaqar/api/v2/request.py` & `zaqar-9.0.1/zaqar/api/v2/request.py`

 * *Files identical despite different names*

### Comparing `zaqar-9.0.0.0rc1/zaqar/storage/pooling.py` & `zaqar-9.0.1/zaqar/storage/pooling.py`

 * *Files identical despite different names*

### Comparing `zaqar-9.0.0.0rc1/zaqar/storage/redis/subscriptions.py` & `zaqar-9.0.1/zaqar/storage/redis/subscriptions.py`

 * *Files identical despite different names*

### Comparing `zaqar-9.0.0.0rc1/zaqar/storage/redis/pools.py` & `zaqar-9.0.1/zaqar/storage/redis/pools.py`

 * *Files identical despite different names*

### Comparing `zaqar-9.0.0.0rc1/zaqar/storage/redis/claims.py` & `zaqar-9.0.1/zaqar/storage/redis/claims.py`

 * *Files identical despite different names*

### Comparing `zaqar-9.0.0.0rc1/zaqar/storage/redis/queues.py` & `zaqar-9.0.1/zaqar/storage/redis/queues.py`

 * *Files identical despite different names*

### Comparing `zaqar-9.0.0.0rc1/zaqar/storage/redis/driver.py` & `zaqar-9.0.1/zaqar/storage/redis/driver.py`

 * *Files identical despite different names*

### Comparing `zaqar-9.0.0.0rc1/zaqar/storage/redis/messages.py` & `zaqar-9.0.1/zaqar/storage/redis/messages.py`

 * *Files identical despite different names*

### Comparing `zaqar-9.0.0.0rc1/zaqar/storage/redis/scripts/claim_messages.lua` & `zaqar-9.0.1/zaqar/storage/redis/scripts/claim_messages.lua`

 * *Files identical despite different names*

### Comparing `zaqar-9.0.0.0rc1/zaqar/storage/redis/scripts/index_messages.lua` & `zaqar-9.0.1/zaqar/storage/redis/scripts/index_messages.lua`

 * *Files identical despite different names*

### Comparing `zaqar-9.0.0.0rc1/zaqar/storage/redis/__init__.py` & `zaqar-9.0.1/zaqar/storage/redis/__init__.py`

 * *Files identical despite different names*

### Comparing `zaqar-9.0.0.0rc1/zaqar/storage/redis/controllers.py` & `zaqar-9.0.1/zaqar/storage/redis/controllers.py`

 * *Files identical despite different names*

### Comparing `zaqar-9.0.0.0rc1/zaqar/storage/redis/flavors.py` & `zaqar-9.0.1/zaqar/storage/redis/flavors.py`

 * *Files identical despite different names*

### Comparing `zaqar-9.0.0.0rc1/zaqar/storage/redis/catalogue.py` & `zaqar-9.0.1/zaqar/storage/redis/catalogue.py`

 * *Files identical despite different names*

### Comparing `zaqar-9.0.0.0rc1/zaqar/storage/redis/scripting.py` & `zaqar-9.0.1/zaqar/storage/redis/scripting.py`

 * *Files identical despite different names*

### Comparing `zaqar-9.0.0.0rc1/zaqar/storage/redis/models.py` & `zaqar-9.0.1/zaqar/storage/redis/models.py`

 * *Files identical despite different names*

### Comparing `zaqar-9.0.0.0rc1/zaqar/storage/redis/utils.py` & `zaqar-9.0.1/zaqar/storage/redis/utils.py`

 * *Files identical despite different names*

### Comparing `zaqar-9.0.0.0rc1/zaqar/storage/mongodb/subscriptions.py` & `zaqar-9.0.1/zaqar/storage/mongodb/subscriptions.py`

 * *Files identical despite different names*

### Comparing `zaqar-9.0.0.0rc1/zaqar/storage/mongodb/pools.py` & `zaqar-9.0.1/zaqar/storage/mongodb/pools.py`

 * *Files identical despite different names*

### Comparing `zaqar-9.0.0.0rc1/zaqar/storage/mongodb/claims.py` & `zaqar-9.0.1/zaqar/storage/mongodb/claims.py`

 * *Files identical despite different names*

### Comparing `zaqar-9.0.0.0rc1/zaqar/storage/mongodb/queues.py` & `zaqar-9.0.1/zaqar/storage/mongodb/queues.py`

 * *Files identical despite different names*

### Comparing `zaqar-9.0.0.0rc1/zaqar/storage/mongodb/driver.py` & `zaqar-9.0.1/zaqar/storage/mongodb/driver.py`

 * *Files identical despite different names*

### Comparing `zaqar-9.0.0.0rc1/zaqar/storage/mongodb/messages.py` & `zaqar-9.0.1/zaqar/storage/mongodb/messages.py`

 * *Files identical despite different names*

### Comparing `zaqar-9.0.0.0rc1/zaqar/storage/mongodb/__init__.py` & `zaqar-9.0.1/zaqar/storage/mongodb/__init__.py`

 * *Files identical despite different names*

### Comparing `zaqar-9.0.0.0rc1/zaqar/storage/mongodb/controllers.py` & `zaqar-9.0.1/zaqar/storage/mongodb/controllers.py`

 * *Files identical despite different names*

### Comparing `zaqar-9.0.0.0rc1/zaqar/storage/mongodb/topic_messages.py` & `zaqar-9.0.1/zaqar/storage/mongodb/topic_messages.py`

 * *Files identical despite different names*

### Comparing `zaqar-9.0.0.0rc1/zaqar/storage/mongodb/topics.py` & `zaqar-9.0.1/zaqar/storage/mongodb/topics.py`

 * *Files identical despite different names*

### Comparing `zaqar-9.0.0.0rc1/zaqar/storage/mongodb/flavors.py` & `zaqar-9.0.1/zaqar/storage/mongodb/flavors.py`

 * *Files identical despite different names*

### Comparing `zaqar-9.0.0.0rc1/zaqar/storage/mongodb/catalogue.py` & `zaqar-9.0.1/zaqar/storage/mongodb/catalogue.py`

 * *Files identical despite different names*

### Comparing `zaqar-9.0.0.0rc1/zaqar/storage/mongodb/utils.py` & `zaqar-9.0.1/zaqar/storage/mongodb/utils.py`

 * *Files identical despite different names*

### Comparing `zaqar-9.0.0.0rc1/zaqar/storage/pipeline.py` & `zaqar-9.0.1/zaqar/storage/pipeline.py`

 * *Files identical despite different names*

### Comparing `zaqar-9.0.0.0rc1/zaqar/storage/sqlalchemy/pools.py` & `zaqar-9.0.1/zaqar/storage/sqlalchemy/pools.py`

 * *Files identical despite different names*

### Comparing `zaqar-9.0.0.0rc1/zaqar/storage/sqlalchemy/queues.py` & `zaqar-9.0.1/zaqar/storage/sqlalchemy/queues.py`

 * *Files identical despite different names*

### Comparing `zaqar-9.0.0.0rc1/zaqar/storage/sqlalchemy/driver.py` & `zaqar-9.0.1/zaqar/storage/sqlalchemy/driver.py`

 * *Files identical despite different names*

### Comparing `zaqar-9.0.0.0rc1/zaqar/storage/sqlalchemy/__init__.py` & `zaqar-9.0.1/zaqar/storage/sqlalchemy/__init__.py`

 * *Files identical despite different names*

### Comparing `zaqar-9.0.0.0rc1/zaqar/storage/sqlalchemy/controllers.py` & `zaqar-9.0.1/zaqar/storage/sqlalchemy/controllers.py`

 * *Files identical despite different names*

### Comparing `zaqar-9.0.0.0rc1/zaqar/storage/sqlalchemy/migration/cli.py` & `zaqar-9.0.1/zaqar/storage/sqlalchemy/migration/cli.py`

 * *Files identical despite different names*

### Comparing `zaqar-9.0.0.0rc1/zaqar/storage/sqlalchemy/migration/alembic_migrations/README.md` & `zaqar-9.0.1/zaqar/storage/sqlalchemy/migration/alembic_migrations/README.md`

 * *Files identical despite different names*

### Comparing `zaqar-9.0.0.0rc1/zaqar/storage/sqlalchemy/migration/alembic_migrations/script.py.mako` & `zaqar-9.0.1/zaqar/storage/sqlalchemy/migration/alembic_migrations/script.py.mako`

 * *Files identical despite different names*

### Comparing `zaqar-9.0.0.0rc1/zaqar/storage/sqlalchemy/migration/alembic_migrations/versions/001_liberty.py` & `zaqar-9.0.1/zaqar/storage/sqlalchemy/migration/alembic_migrations/versions/001_liberty.py`

 * *Files identical despite different names*

### Comparing `zaqar-9.0.0.0rc1/zaqar/storage/sqlalchemy/migration/alembic_migrations/versions/003_placeholder.py` & `zaqar-9.0.1/zaqar/storage/sqlalchemy/migration/alembic_migrations/versions/003_placeholder.py`

 * *Files identical despite different names*

### Comparing `zaqar-9.0.0.0rc1/zaqar/storage/sqlalchemy/migration/alembic_migrations/versions/004_placeholder.py` & `zaqar-9.0.1/zaqar/storage/sqlalchemy/migration/alembic_migrations/versions/004_placeholder.py`

 * *Files identical despite different names*

### Comparing `zaqar-9.0.0.0rc1/zaqar/storage/sqlalchemy/migration/alembic_migrations/versions/002_placeholder.py` & `zaqar-9.0.1/zaqar/storage/sqlalchemy/migration/alembic_migrations/versions/002_placeholder.py`

 * *Files identical despite different names*

### Comparing `zaqar-9.0.0.0rc1/zaqar/storage/sqlalchemy/migration/alembic_migrations/versions/007_stein.py` & `zaqar-9.0.1/zaqar/storage/sqlalchemy/migration/alembic_migrations/versions/007_stein.py`

 * *Files identical despite different names*

### Comparing `zaqar-9.0.0.0rc1/zaqar/storage/sqlalchemy/migration/alembic_migrations/versions/005_placeholder.py` & `zaqar-9.0.1/zaqar/storage/sqlalchemy/migration/alembic_migrations/versions/005_placeholder.py`

 * *Files identical despite different names*

### Comparing `zaqar-9.0.0.0rc1/zaqar/storage/sqlalchemy/migration/alembic_migrations/versions/006_queens.py` & `zaqar-9.0.1/zaqar/storage/sqlalchemy/migration/alembic_migrations/versions/006_queens.py`

 * *Files identical despite different names*

### Comparing `zaqar-9.0.0.0rc1/zaqar/storage/sqlalchemy/migration/alembic_migrations/env.py` & `zaqar-9.0.1/zaqar/storage/sqlalchemy/migration/alembic_migrations/env.py`

 * *Files identical despite different names*

### Comparing `zaqar-9.0.0.0rc1/zaqar/storage/sqlalchemy/migration/alembic.ini` & `zaqar-9.0.1/zaqar/storage/sqlalchemy/migration/alembic.ini`

 * *Files identical despite different names*

### Comparing `zaqar-9.0.0.0rc1/zaqar/storage/sqlalchemy/tables.py` & `zaqar-9.0.1/zaqar/storage/sqlalchemy/tables.py`

 * *Files identical despite different names*

### Comparing `zaqar-9.0.0.0rc1/zaqar/storage/sqlalchemy/flavors.py` & `zaqar-9.0.1/zaqar/storage/sqlalchemy/flavors.py`

 * *Files identical despite different names*

### Comparing `zaqar-9.0.0.0rc1/zaqar/storage/sqlalchemy/catalogue.py` & `zaqar-9.0.1/zaqar/storage/sqlalchemy/catalogue.py`

 * *Files identical despite different names*

### Comparing `zaqar-9.0.0.0rc1/zaqar/storage/sqlalchemy/utils.py` & `zaqar-9.0.1/zaqar/storage/sqlalchemy/utils.py`

 * *Files identical despite different names*

### Comparing `zaqar-9.0.0.0rc1/zaqar/storage/errors.py` & `zaqar-9.0.1/zaqar/storage/errors.py`

 * *Files identical despite different names*

### Comparing `zaqar-9.0.0.0rc1/zaqar/storage/configuration.py` & `zaqar-9.0.1/zaqar/storage/configuration.py`

 * *Files identical despite different names*

### Comparing `zaqar-9.0.0.0rc1/zaqar/storage/__init__.py` & `zaqar-9.0.1/zaqar/storage/__init__.py`

 * *Files identical despite different names*

### Comparing `zaqar-9.0.0.0rc1/zaqar/storage/base.py` & `zaqar-9.0.1/zaqar/storage/base.py`

 * *Files identical despite different names*

### Comparing `zaqar-9.0.0.0rc1/zaqar/storage/swift/subscriptions.py` & `zaqar-9.0.1/zaqar/storage/swift/subscriptions.py`

 * *Files identical despite different names*

### Comparing `zaqar-9.0.0.0rc1/zaqar/storage/swift/claims.py` & `zaqar-9.0.1/zaqar/storage/swift/claims.py`

 * *Files identical despite different names*

### Comparing `zaqar-9.0.0.0rc1/zaqar/storage/swift/driver.py` & `zaqar-9.0.1/zaqar/storage/swift/driver.py`

 * *Files identical despite different names*

### Comparing `zaqar-9.0.0.0rc1/zaqar/storage/swift/messages.py` & `zaqar-9.0.1/zaqar/storage/swift/messages.py`

 * *Files identical despite different names*

### Comparing `zaqar-9.0.0.0rc1/zaqar/storage/swift/controllers.py` & `zaqar-9.0.1/zaqar/storage/swift/controllers.py`

 * *Files identical despite different names*

### Comparing `zaqar-9.0.0.0rc1/zaqar/storage/swift/utils.py` & `zaqar-9.0.1/zaqar/storage/swift/utils.py`

 * *Files identical despite different names*

### Comparing `zaqar-9.0.0.0rc1/zaqar/storage/utils.py` & `zaqar-9.0.1/zaqar/storage/utils.py`

 * *Files identical despite different names*

### Comparing `zaqar-9.0.0.0rc1/zaqar/transport/acl.py` & `zaqar-9.0.1/zaqar/transport/acl.py`

 * *Files identical despite different names*

### Comparing `zaqar-9.0.0.0rc1/zaqar/transport/validation.py` & `zaqar-9.0.1/zaqar/transport/validation.py`

 * *Files identical despite different names*

### Comparing `zaqar-9.0.0.0rc1/zaqar/transport/__init__.py` & `zaqar-9.0.1/zaqar/transport/__init__.py`

 * *Files identical despite different names*

### Comparing `zaqar-9.0.0.0rc1/zaqar/transport/base.py` & `zaqar-9.0.1/zaqar/transport/base.py`

 * *Files identical despite different names*

### Comparing `zaqar-9.0.0.0rc1/zaqar/transport/wsgi/v2_0/subscriptions.py` & `zaqar-9.0.1/zaqar/transport/wsgi/v2_0/subscriptions.py`

 * *Files identical despite different names*

### Comparing `zaqar-9.0.0.0rc1/zaqar/transport/wsgi/v2_0/pools.py` & `zaqar-9.0.1/zaqar/transport/wsgi/v2_0/pools.py`

 * *Files identical despite different names*

### Comparing `zaqar-9.0.0.0rc1/zaqar/transport/wsgi/v2_0/claims.py` & `zaqar-9.0.1/zaqar/transport/wsgi/v2_0/claims.py`

 * *Files identical despite different names*

### Comparing `zaqar-9.0.0.0rc1/zaqar/transport/wsgi/v2_0/queues.py` & `zaqar-9.0.1/zaqar/transport/wsgi/v2_0/queues.py`

 * *Files identical despite different names*

### Comparing `zaqar-9.0.0.0rc1/zaqar/transport/wsgi/v2_0/messages.py` & `zaqar-9.0.1/zaqar/transport/wsgi/v2_0/messages.py`

 * *Files identical despite different names*

### Comparing `zaqar-9.0.0.0rc1/zaqar/transport/wsgi/v2_0/urls.py` & `zaqar-9.0.1/zaqar/transport/wsgi/v2_0/urls.py`

 * *Files identical despite different names*

### Comparing `zaqar-9.0.0.0rc1/zaqar/transport/wsgi/v2_0/health.py` & `zaqar-9.0.1/zaqar/transport/wsgi/v2_0/health.py`

 * *Files identical despite different names*

### Comparing `zaqar-9.0.0.0rc1/zaqar/transport/wsgi/v2_0/__init__.py` & `zaqar-9.0.1/zaqar/transport/wsgi/v2_0/__init__.py`

 * *Files identical despite different names*

### Comparing `zaqar-9.0.0.0rc1/zaqar/transport/wsgi/v2_0/topic_purge.py` & `zaqar-9.0.1/zaqar/transport/wsgi/v2_0/topic_purge.py`

 * *Files identical despite different names*

### Comparing `zaqar-9.0.0.0rc1/zaqar/transport/wsgi/v2_0/homedoc.py` & `zaqar-9.0.1/zaqar/transport/wsgi/v2_0/homedoc.py`

 * *Files identical despite different names*

### Comparing `zaqar-9.0.0.0rc1/zaqar/transport/wsgi/v2_0/topic.py` & `zaqar-9.0.1/zaqar/transport/wsgi/v2_0/topic.py`

 * *Files identical despite different names*

### Comparing `zaqar-9.0.0.0rc1/zaqar/transport/wsgi/v2_0/ping.py` & `zaqar-9.0.1/zaqar/transport/wsgi/v2_0/ping.py`

 * *Files identical despite different names*

### Comparing `zaqar-9.0.0.0rc1/zaqar/transport/wsgi/v2_0/purge.py` & `zaqar-9.0.1/zaqar/transport/wsgi/v2_0/purge.py`

 * *Files identical despite different names*

### Comparing `zaqar-9.0.0.0rc1/zaqar/transport/wsgi/v2_0/topic_stats.py` & `zaqar-9.0.1/zaqar/transport/wsgi/v2_0/topic_stats.py`

 * *Files identical despite different names*

### Comparing `zaqar-9.0.0.0rc1/zaqar/transport/wsgi/v2_0/stats.py` & `zaqar-9.0.1/zaqar/transport/wsgi/v2_0/stats.py`

 * *Files identical despite different names*

### Comparing `zaqar-9.0.0.0rc1/zaqar/transport/wsgi/v2_0/flavors.py` & `zaqar-9.0.1/zaqar/transport/wsgi/v2_0/flavors.py`

 * *Files identical despite different names*

### Comparing `zaqar-9.0.0.0rc1/zaqar/transport/wsgi/errors.py` & `zaqar-9.0.1/zaqar/transport/wsgi/errors.py`

 * *Files identical despite different names*

### Comparing `zaqar-9.0.0.0rc1/zaqar/transport/wsgi/driver.py` & `zaqar-9.0.1/zaqar/transport/wsgi/driver.py`

 * *Files identical despite different names*

### Comparing `zaqar-9.0.0.0rc1/zaqar/transport/wsgi/v1_1/pools.py` & `zaqar-9.0.1/zaqar/transport/wsgi/v1_1/pools.py`

 * *Files identical despite different names*

### Comparing `zaqar-9.0.0.0rc1/zaqar/transport/wsgi/v1_1/claims.py` & `zaqar-9.0.1/zaqar/transport/wsgi/v1_1/claims.py`

 * *Files identical despite different names*

### Comparing `zaqar-9.0.0.0rc1/zaqar/transport/wsgi/v1_1/queues.py` & `zaqar-9.0.1/zaqar/transport/wsgi/v1_1/queues.py`

 * *Files identical despite different names*

### Comparing `zaqar-9.0.0.0rc1/zaqar/transport/wsgi/v1_1/messages.py` & `zaqar-9.0.1/zaqar/transport/wsgi/v1_1/messages.py`

 * *Files identical despite different names*

### Comparing `zaqar-9.0.0.0rc1/zaqar/transport/wsgi/v1_1/health.py` & `zaqar-9.0.1/zaqar/transport/wsgi/v1_1/health.py`

 * *Files identical despite different names*

### Comparing `zaqar-9.0.0.0rc1/zaqar/transport/wsgi/v1_1/__init__.py` & `zaqar-9.0.1/zaqar/transport/wsgi/v1_1/__init__.py`

 * *Files identical despite different names*

### Comparing `zaqar-9.0.0.0rc1/zaqar/transport/wsgi/v1_1/homedoc.py` & `zaqar-9.0.1/zaqar/transport/wsgi/v1_1/homedoc.py`

 * *Files identical despite different names*

### Comparing `zaqar-9.0.0.0rc1/zaqar/transport/wsgi/v1_1/ping.py` & `zaqar-9.0.1/zaqar/transport/wsgi/v1_1/ping.py`

 * *Files identical despite different names*

### Comparing `zaqar-9.0.0.0rc1/zaqar/transport/wsgi/v1_1/stats.py` & `zaqar-9.0.1/zaqar/transport/wsgi/v1_1/stats.py`

 * *Files identical despite different names*

### Comparing `zaqar-9.0.0.0rc1/zaqar/transport/wsgi/v1_1/flavors.py` & `zaqar-9.0.1/zaqar/transport/wsgi/v1_1/flavors.py`

 * *Files identical despite different names*

### Comparing `zaqar-9.0.0.0rc1/zaqar/transport/wsgi/version.py` & `zaqar-9.0.1/zaqar/transport/wsgi/version.py`

 * *Files identical despite different names*

### Comparing `zaqar-9.0.0.0rc1/zaqar/transport/wsgi/__init__.py` & `zaqar-9.0.1/zaqar/transport/wsgi/__init__.py`

 * *Files identical despite different names*

### Comparing `zaqar-9.0.0.0rc1/zaqar/transport/wsgi/v1_0/metadata.py` & `zaqar-9.0.1/zaqar/transport/wsgi/v1_0/metadata.py`

 * *Files identical despite different names*

### Comparing `zaqar-9.0.0.0rc1/zaqar/transport/wsgi/v1_0/pools.py` & `zaqar-9.0.1/zaqar/transport/wsgi/v1_0/pools.py`

 * *Files identical despite different names*

### Comparing `zaqar-9.0.0.0rc1/zaqar/transport/wsgi/v1_0/claims.py` & `zaqar-9.0.1/zaqar/transport/wsgi/v1_0/claims.py`

 * *Files identical despite different names*

### Comparing `zaqar-9.0.0.0rc1/zaqar/transport/wsgi/v1_0/queues.py` & `zaqar-9.0.1/zaqar/transport/wsgi/v1_0/queues.py`

 * *Files identical despite different names*

### Comparing `zaqar-9.0.0.0rc1/zaqar/transport/wsgi/v1_0/messages.py` & `zaqar-9.0.1/zaqar/transport/wsgi/v1_0/messages.py`

 * *Files identical despite different names*

### Comparing `zaqar-9.0.0.0rc1/zaqar/transport/wsgi/v1_0/health.py` & `zaqar-9.0.1/zaqar/transport/wsgi/v1_0/health.py`

 * *Files identical despite different names*

### Comparing `zaqar-9.0.0.0rc1/zaqar/transport/wsgi/v1_0/__init__.py` & `zaqar-9.0.1/zaqar/transport/wsgi/v1_0/__init__.py`

 * *Files identical despite different names*

### Comparing `zaqar-9.0.0.0rc1/zaqar/transport/wsgi/v1_0/homedoc.py` & `zaqar-9.0.1/zaqar/transport/wsgi/v1_0/homedoc.py`

 * *Files identical despite different names*

### Comparing `zaqar-9.0.0.0rc1/zaqar/transport/wsgi/v1_0/stats.py` & `zaqar-9.0.1/zaqar/transport/wsgi/v1_0/stats.py`

 * *Files identical despite different names*

### Comparing `zaqar-9.0.0.0rc1/zaqar/transport/wsgi/app.py` & `zaqar-9.0.1/zaqar/transport/wsgi/app.py`

 * *Files identical despite different names*

### Comparing `zaqar-9.0.0.0rc1/zaqar/transport/wsgi/utils.py` & `zaqar-9.0.1/zaqar/transport/wsgi/utils.py`

 * *Files identical despite different names*

### Comparing `zaqar-9.0.0.0rc1/zaqar/transport/middleware/cors.py` & `zaqar-9.0.1/zaqar/transport/middleware/cors.py`

 * *Files identical despite different names*

### Comparing `zaqar-9.0.0.0rc1/zaqar/transport/middleware/auth.py` & `zaqar-9.0.1/zaqar/transport/middleware/auth.py`

 * *Files identical despite different names*

### Comparing `zaqar-9.0.0.0rc1/zaqar/transport/middleware/profile.py` & `zaqar-9.0.1/zaqar/transport/middleware/profile.py`

 * *Files identical despite different names*

### Comparing `zaqar-9.0.0.0rc1/zaqar/transport/websocket/driver.py` & `zaqar-9.0.1/zaqar/transport/websocket/driver.py`

 * *Files identical despite different names*

### Comparing `zaqar-9.0.0.0rc1/zaqar/transport/websocket/__init__.py` & `zaqar-9.0.1/zaqar/transport/websocket/__init__.py`

 * *Files identical despite different names*

### Comparing `zaqar-9.0.0.0rc1/zaqar/transport/websocket/protocol.py` & `zaqar-9.0.1/zaqar/transport/websocket/protocol.py`

 * *Files identical despite different names*

### Comparing `zaqar-9.0.0.0rc1/zaqar/transport/websocket/factory.py` & `zaqar-9.0.1/zaqar/transport/websocket/factory.py`

 * *Files identical despite different names*

### Comparing `zaqar-9.0.0.0rc1/zaqar/transport/utils.py` & `zaqar-9.0.1/zaqar/transport/utils.py`

 * *Files identical despite different names*

### Comparing `zaqar-9.0.0.0rc1/zaqar/tests/helpers.py` & `zaqar-9.0.1/zaqar/tests/helpers.py`

 * *Files identical despite different names*

### Comparing `zaqar-9.0.0.0rc1/zaqar/tests/etc/functional-zaqar.conf` & `zaqar-9.0.1/zaqar/tests/etc/functional-zaqar.conf`

 * *Files identical despite different names*

### Comparing `zaqar-9.0.0.0rc1/zaqar/tests/functional/config.py` & `zaqar-9.0.1/zaqar/tests/functional/config.py`

 * *Files identical despite different names*

### Comparing `zaqar-9.0.0.0rc1/zaqar/tests/functional/helpers.py` & `zaqar-9.0.1/zaqar/tests/functional/helpers.py`

 * *Files identical despite different names*

### Comparing `zaqar-9.0.0.0rc1/zaqar/tests/functional/base.py` & `zaqar-9.0.1/zaqar/tests/functional/base.py`

 * *Files identical despite different names*

### Comparing `zaqar-9.0.0.0rc1/zaqar/tests/functional/wsgi/v1/test_queues.py` & `zaqar-9.0.1/zaqar/tests/functional/wsgi/v1/test_queues.py`

 * *Files identical despite different names*

### Comparing `zaqar-9.0.0.0rc1/zaqar/tests/functional/wsgi/v1/test_messages.py` & `zaqar-9.0.1/zaqar/tests/functional/wsgi/v1/test_messages.py`

 * *Files identical despite different names*

### Comparing `zaqar-9.0.0.0rc1/zaqar/tests/functional/wsgi/v1/test_claims.py` & `zaqar-9.0.1/zaqar/tests/functional/wsgi/v1/test_claims.py`

 * *Files identical despite different names*

### Comparing `zaqar-9.0.0.0rc1/zaqar/tests/functional/wsgi/v1_1/test_queues.py` & `zaqar-9.0.1/zaqar/tests/functional/wsgi/v1_1/test_queues.py`

 * *Files identical despite different names*

### Comparing `zaqar-9.0.0.0rc1/zaqar/tests/functional/wsgi/v1_1/test_messages.py` & `zaqar-9.0.1/zaqar/tests/functional/wsgi/v1_1/test_messages.py`

 * *Files identical despite different names*

### Comparing `zaqar-9.0.0.0rc1/zaqar/tests/functional/wsgi/v1_1/test_health.py` & `zaqar-9.0.1/zaqar/tests/functional/wsgi/v1_1/test_health.py`

 * *Files identical despite different names*

### Comparing `zaqar-9.0.0.0rc1/zaqar/tests/functional/wsgi/v1_1/test_pools.py` & `zaqar-9.0.1/zaqar/tests/functional/wsgi/v1_1/test_pools.py`

 * *Files identical despite different names*

### Comparing `zaqar-9.0.0.0rc1/zaqar/tests/functional/wsgi/v1_1/test_claims.py` & `zaqar-9.0.1/zaqar/tests/functional/wsgi/v1_1/test_claims.py`

 * *Files identical despite different names*

### Comparing `zaqar-9.0.0.0rc1/zaqar/tests/functional/wsgi/test_versions.py` & `zaqar-9.0.1/zaqar/tests/functional/wsgi/test_versions.py`

 * *Files identical despite different names*

### Comparing `zaqar-9.0.0.0rc1/zaqar/tests/functional/wsgi/v2/test_subscriptions.py` & `zaqar-9.0.1/zaqar/tests/functional/wsgi/v2/test_subscriptions.py`

 * *Files identical despite different names*

### Comparing `zaqar-9.0.0.0rc1/zaqar/tests/functional/websocket/test_queues.py` & `zaqar-9.0.1/zaqar/tests/functional/websocket/test_queues.py`

 * *Files identical despite different names*

### Comparing `zaqar-9.0.0.0rc1/zaqar/tests/functional/http.py` & `zaqar-9.0.1/zaqar/tests/functional/http.py`

 * *Files identical despite different names*

### Comparing `zaqar-9.0.0.0rc1/zaqar/tests/__init__.py` & `zaqar-9.0.1/zaqar/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `zaqar-9.0.0.0rc1/zaqar/tests/unit/notification/test_notifier.py` & `zaqar-9.0.1/zaqar/tests/unit/notification/test_notifier.py`

 * *Files identical despite different names*

### Comparing `zaqar-9.0.0.0rc1/zaqar/tests/unit/common/test_request.py` & `zaqar-9.0.1/zaqar/tests/unit/common/test_request.py`

 * *Files identical despite different names*

### Comparing `zaqar-9.0.0.0rc1/zaqar/tests/unit/common/test_urls.py` & `zaqar-9.0.1/zaqar/tests/unit/common/test_urls.py`

 * *Files identical despite different names*

### Comparing `zaqar-9.0.0.0rc1/zaqar/tests/unit/common/storage/test_select.py` & `zaqar-9.0.1/zaqar/tests/unit/common/storage/test_select.py`

 * *Files identical despite different names*

### Comparing `zaqar-9.0.0.0rc1/zaqar/tests/unit/common/storage/test_utils.py` & `zaqar-9.0.1/zaqar/tests/unit/common/storage/test_utils.py`

 * *Files identical despite different names*

### Comparing `zaqar-9.0.0.0rc1/zaqar/tests/unit/common/test_pipeline.py` & `zaqar-9.0.1/zaqar/tests/unit/common/test_pipeline.py`

 * *Files identical despite different names*

### Comparing `zaqar-9.0.0.0rc1/zaqar/tests/unit/common/test_api.py` & `zaqar-9.0.1/zaqar/tests/unit/common/test_api.py`

 * *Files identical despite different names*

### Comparing `zaqar-9.0.0.0rc1/zaqar/tests/unit/common/test_decorators.py` & `zaqar-9.0.1/zaqar/tests/unit/common/test_decorators.py`

 * *Files identical despite different names*

### Comparing `zaqar-9.0.0.0rc1/zaqar/tests/unit/storage/test_impl_mongodb.py` & `zaqar-9.0.1/zaqar/tests/unit/storage/test_impl_mongodb.py`

 * *Files identical despite different names*

### Comparing `zaqar-9.0.0.0rc1/zaqar/tests/unit/storage/sqlalchemy_migration/test_migrations.py` & `zaqar-9.0.1/zaqar/tests/unit/storage/sqlalchemy_migration/test_migrations.py`

 * *Files identical despite different names*

### Comparing `zaqar-9.0.0.0rc1/zaqar/tests/unit/storage/sqlalchemy_migration/test_migrations_base.py` & `zaqar-9.0.1/zaqar/tests/unit/storage/sqlalchemy_migration/test_migrations_base.py`

 * *Files identical despite different names*

### Comparing `zaqar-9.0.0.0rc1/zaqar/tests/unit/storage/sqlalchemy_migration/test_db_manage_cli.py` & `zaqar-9.0.1/zaqar/tests/unit/storage/sqlalchemy_migration/test_db_manage_cli.py`

 * *Files identical despite different names*

### Comparing `zaqar-9.0.0.0rc1/zaqar/tests/unit/storage/test_impl_sqlalchemy.py` & `zaqar-9.0.1/zaqar/tests/unit/storage/test_impl_sqlalchemy.py`

 * *Files identical despite different names*

### Comparing `zaqar-9.0.0.0rc1/zaqar/tests/unit/storage/test_pool_catalog_new.py` & `zaqar-9.0.1/zaqar/tests/unit/storage/test_pool_catalog_new.py`

 * *Files identical despite different names*

### Comparing `zaqar-9.0.0.0rc1/zaqar/tests/unit/storage/test_impl_swift.py` & `zaqar-9.0.1/zaqar/tests/unit/storage/test_impl_swift.py`

 * *Files identical despite different names*

### Comparing `zaqar-9.0.0.0rc1/zaqar/tests/unit/storage/base.py` & `zaqar-9.0.1/zaqar/tests/unit/storage/base.py`

 * *Files identical despite different names*

### Comparing `zaqar-9.0.0.0rc1/zaqar/tests/unit/storage/test_impl_redis.py` & `zaqar-9.0.1/zaqar/tests/unit/storage/test_impl_redis.py`

 * *Files identical despite different names*

### Comparing `zaqar-9.0.0.0rc1/zaqar/tests/unit/storage/test_utils.py` & `zaqar-9.0.1/zaqar/tests/unit/storage/test_utils.py`

 * *Files identical despite different names*

### Comparing `zaqar-9.0.0.0rc1/zaqar/tests/unit/transport/test_acl.py` & `zaqar-9.0.1/zaqar/tests/unit/transport/test_acl.py`

 * *Files identical despite different names*

### Comparing `zaqar-9.0.0.0rc1/zaqar/tests/unit/transport/wsgi/v2_0/test_pools_new.py` & `zaqar-9.0.1/zaqar/tests/unit/transport/wsgi/v2_0/test_pools_new.py`

 * *Files identical despite different names*

### Comparing `zaqar-9.0.0.0rc1/zaqar/tests/unit/transport/wsgi/v2_0/test_default_limits.py` & `zaqar-9.0.1/zaqar/tests/unit/transport/wsgi/v2_0/test_default_limits.py`

 * *Files identical despite different names*

### Comparing `zaqar-9.0.0.0rc1/zaqar/tests/unit/transport/wsgi/v2_0/test_validation.py` & `zaqar-9.0.1/zaqar/tests/unit/transport/wsgi/v2_0/test_validation.py`

 * *Files identical despite different names*

### Comparing `zaqar-9.0.0.0rc1/zaqar/tests/unit/transport/wsgi/v2_0/test_home.py` & `zaqar-9.0.1/zaqar/tests/unit/transport/wsgi/v2_0/test_home.py`

 * *Files identical despite different names*

### Comparing `zaqar-9.0.0.0rc1/zaqar/tests/unit/transport/wsgi/v2_0/test_ping.py` & `zaqar-9.0.1/zaqar/tests/unit/transport/wsgi/v2_0/test_ping.py`

 * *Files identical despite different names*

### Comparing `zaqar-9.0.0.0rc1/zaqar/tests/unit/transport/wsgi/v2_0/test_purge.py` & `zaqar-9.0.1/zaqar/tests/unit/transport/wsgi/v2_0/test_purge.py`

 * *Files identical despite different names*

### Comparing `zaqar-9.0.0.0rc1/zaqar/tests/unit/transport/wsgi/v2_0/test_flavors_new.py` & `zaqar-9.0.1/zaqar/tests/unit/transport/wsgi/v2_0/test_flavors_new.py`

 * *Files identical despite different names*

### Comparing `zaqar-9.0.0.0rc1/zaqar/tests/unit/transport/wsgi/v2_0/test_urls.py` & `zaqar-9.0.1/zaqar/tests/unit/transport/wsgi/v2_0/test_urls.py`

 * *Files identical despite different names*

### Comparing `zaqar-9.0.0.0rc1/zaqar/tests/unit/transport/wsgi/v2_0/test_queue_lifecycle.py` & `zaqar-9.0.1/zaqar/tests/unit/transport/wsgi/v2_0/test_queue_lifecycle.py`

 * *Files identical despite different names*

### Comparing `zaqar-9.0.0.0rc1/zaqar/tests/unit/transport/wsgi/v2_0/test_messages.py` & `zaqar-9.0.1/zaqar/tests/unit/transport/wsgi/v2_0/test_messages.py`

 * *Files identical despite different names*

### Comparing `zaqar-9.0.0.0rc1/zaqar/tests/unit/transport/wsgi/v2_0/test_health.py` & `zaqar-9.0.1/zaqar/tests/unit/transport/wsgi/v2_0/test_health.py`

 * *Files identical despite different names*

### Comparing `zaqar-9.0.0.0rc1/zaqar/tests/unit/transport/wsgi/v2_0/test_media_type.py` & `zaqar-9.0.1/zaqar/tests/unit/transport/wsgi/v2_0/test_media_type.py`

 * *Files identical despite different names*

### Comparing `zaqar-9.0.0.0rc1/zaqar/tests/unit/transport/wsgi/v2_0/test_topic_lifecycle.py` & `zaqar-9.0.1/zaqar/tests/unit/transport/wsgi/v2_0/test_topic_lifecycle.py`

 * *Files identical despite different names*

### Comparing `zaqar-9.0.0.0rc1/zaqar/tests/unit/transport/wsgi/v2_0/test_auth.py` & `zaqar-9.0.1/zaqar/tests/unit/transport/wsgi/v2_0/test_auth.py`

 * *Files identical despite different names*

### Comparing `zaqar-9.0.0.0rc1/zaqar/tests/unit/transport/wsgi/v2_0/test_subscriptions.py` & `zaqar-9.0.1/zaqar/tests/unit/transport/wsgi/v2_0/test_subscriptions.py`

 * *Files identical despite different names*

### Comparing `zaqar-9.0.0.0rc1/zaqar/tests/unit/transport/wsgi/v2_0/test_claims.py` & `zaqar-9.0.1/zaqar/tests/unit/transport/wsgi/v2_0/test_claims.py`

 * *Files identical despite different names*

### Comparing `zaqar-9.0.0.0rc1/zaqar/tests/unit/transport/wsgi/v1/test_default_limits.py` & `zaqar-9.0.1/zaqar/tests/unit/transport/wsgi/v1/test_default_limits.py`

 * *Files identical despite different names*

### Comparing `zaqar-9.0.0.0rc1/zaqar/tests/unit/transport/wsgi/v1/test_validation.py` & `zaqar-9.0.1/zaqar/tests/unit/transport/wsgi/v1/test_validation.py`

 * *Files identical despite different names*

### Comparing `zaqar-9.0.0.0rc1/zaqar/tests/unit/transport/wsgi/v1/test_home.py` & `zaqar-9.0.1/zaqar/tests/unit/transport/wsgi/v1/test_home.py`

 * *Files identical despite different names*

### Comparing `zaqar-9.0.0.0rc1/zaqar/tests/unit/transport/wsgi/v1/test_queue_lifecycle.py` & `zaqar-9.0.1/zaqar/tests/unit/transport/wsgi/v1/test_queue_lifecycle.py`

 * *Files identical despite different names*

### Comparing `zaqar-9.0.0.0rc1/zaqar/tests/unit/transport/wsgi/v1/test_messages.py` & `zaqar-9.0.1/zaqar/tests/unit/transport/wsgi/v1/test_messages.py`

 * *Files identical despite different names*

### Comparing `zaqar-9.0.0.0rc1/zaqar/tests/unit/transport/wsgi/v1/test_health.py` & `zaqar-9.0.1/zaqar/tests/unit/transport/wsgi/v1/test_health.py`

 * *Files identical despite different names*

### Comparing `zaqar-9.0.0.0rc1/zaqar/tests/unit/transport/wsgi/v1/test_media_type.py` & `zaqar-9.0.1/zaqar/tests/unit/transport/wsgi/v1/test_media_type.py`

 * *Files identical despite different names*

### Comparing `zaqar-9.0.0.0rc1/zaqar/tests/unit/transport/wsgi/v1/test_auth.py` & `zaqar-9.0.1/zaqar/tests/unit/transport/wsgi/v1/test_auth.py`

 * *Files identical despite different names*

### Comparing `zaqar-9.0.0.0rc1/zaqar/tests/unit/transport/wsgi/v1/test_pools.py` & `zaqar-9.0.1/zaqar/tests/unit/transport/wsgi/v1/test_pools.py`

 * *Files identical despite different names*

### Comparing `zaqar-9.0.0.0rc1/zaqar/tests/unit/transport/wsgi/v1/test_claims.py` & `zaqar-9.0.1/zaqar/tests/unit/transport/wsgi/v1/test_claims.py`

 * *Files identical despite different names*

### Comparing `zaqar-9.0.0.0rc1/zaqar/tests/unit/transport/wsgi/test_version.py` & `zaqar-9.0.1/zaqar/tests/unit/transport/wsgi/test_version.py`

 * *Files identical despite different names*

### Comparing `zaqar-9.0.0.0rc1/zaqar/tests/unit/transport/wsgi/v1_1/test_default_limits.py` & `zaqar-9.0.1/zaqar/tests/unit/transport/wsgi/v1_1/test_default_limits.py`

 * *Files identical despite different names*

### Comparing `zaqar-9.0.0.0rc1/zaqar/tests/unit/transport/wsgi/v1_1/test_validation.py` & `zaqar-9.0.1/zaqar/tests/unit/transport/wsgi/v1_1/test_validation.py`

 * *Files identical despite different names*

### Comparing `zaqar-9.0.0.0rc1/zaqar/tests/unit/transport/wsgi/v1_1/test_home.py` & `zaqar-9.0.1/zaqar/tests/unit/transport/wsgi/v1_1/test_home.py`

 * *Files identical despite different names*

### Comparing `zaqar-9.0.0.0rc1/zaqar/tests/unit/transport/wsgi/v1_1/test_ping.py` & `zaqar-9.0.1/zaqar/tests/unit/transport/wsgi/v1_1/test_ping.py`

 * *Files identical despite different names*

### Comparing `zaqar-9.0.0.0rc1/zaqar/tests/unit/transport/wsgi/v1_1/test_queue_lifecycle.py` & `zaqar-9.0.1/zaqar/tests/unit/transport/wsgi/v1_1/test_queue_lifecycle.py`

 * *Files identical despite different names*

### Comparing `zaqar-9.0.0.0rc1/zaqar/tests/unit/transport/wsgi/v1_1/test_messages.py` & `zaqar-9.0.1/zaqar/tests/unit/transport/wsgi/v1_1/test_messages.py`

 * *Files identical despite different names*

### Comparing `zaqar-9.0.0.0rc1/zaqar/tests/unit/transport/wsgi/v1_1/test_health.py` & `zaqar-9.0.1/zaqar/tests/unit/transport/wsgi/v1_1/test_health.py`

 * *Files identical despite different names*

### Comparing `zaqar-9.0.0.0rc1/zaqar/tests/unit/transport/wsgi/v1_1/test_media_type.py` & `zaqar-9.0.1/zaqar/tests/unit/transport/wsgi/v1_1/test_media_type.py`

 * *Files identical despite different names*

### Comparing `zaqar-9.0.0.0rc1/zaqar/tests/unit/transport/wsgi/v1_1/test_auth.py` & `zaqar-9.0.1/zaqar/tests/unit/transport/wsgi/v1_1/test_auth.py`

 * *Files identical despite different names*

### Comparing `zaqar-9.0.0.0rc1/zaqar/tests/unit/transport/wsgi/v1_1/test_claims.py` & `zaqar-9.0.1/zaqar/tests/unit/transport/wsgi/v1_1/test_claims.py`

 * *Files identical despite different names*

### Comparing `zaqar-9.0.0.0rc1/zaqar/tests/unit/transport/wsgi/__init__.py` & `zaqar-9.0.1/zaqar/tests/unit/transport/wsgi/__init__.py`

 * *Files identical despite different names*

### Comparing `zaqar-9.0.0.0rc1/zaqar/tests/unit/transport/wsgi/base.py` & `zaqar-9.0.1/zaqar/tests/unit/transport/wsgi/base.py`

 * *Files identical despite different names*

### Comparing `zaqar-9.0.0.0rc1/zaqar/tests/unit/transport/wsgi/test_utils.py` & `zaqar-9.0.1/zaqar/tests/unit/transport/wsgi/test_utils.py`

 * *Files identical despite different names*

### Comparing `zaqar-9.0.0.0rc1/zaqar/tests/unit/transport/websocket/test_protocol.py` & `zaqar-9.0.1/zaqar/tests/unit/transport/websocket/test_protocol.py`

 * *Files identical despite different names*

### Comparing `zaqar-9.0.0.0rc1/zaqar/tests/unit/transport/websocket/base.py` & `zaqar-9.0.1/zaqar/tests/unit/transport/websocket/base.py`

 * *Files identical despite different names*

### Comparing `zaqar-9.0.0.0rc1/zaqar/tests/unit/transport/websocket/v2/test_queue_lifecycle.py` & `zaqar-9.0.1/zaqar/tests/unit/transport/websocket/v2/test_queue_lifecycle.py`

 * *Files identical despite different names*

### Comparing `zaqar-9.0.0.0rc1/zaqar/tests/unit/transport/websocket/v2/test_messages.py` & `zaqar-9.0.1/zaqar/tests/unit/transport/websocket/v2/test_messages.py`

 * *Files identical despite different names*

### Comparing `zaqar-9.0.0.0rc1/zaqar/tests/unit/transport/websocket/v2/test_auth.py` & `zaqar-9.0.1/zaqar/tests/unit/transport/websocket/v2/test_auth.py`

 * *Files identical despite different names*

### Comparing `zaqar-9.0.0.0rc1/zaqar/tests/unit/transport/websocket/v2/test_subscriptions.py` & `zaqar-9.0.1/zaqar/tests/unit/transport/websocket/v2/test_subscriptions.py`

 * *Files identical despite different names*

### Comparing `zaqar-9.0.0.0rc1/zaqar/tests/unit/transport/websocket/v2/test_claims.py` & `zaqar-9.0.1/zaqar/tests/unit/transport/websocket/v2/test_claims.py`

 * *Files identical despite different names*

### Comparing `zaqar-9.0.0.0rc1/zaqar/tests/unit/transport/websocket/utils.py` & `zaqar-9.0.1/zaqar/tests/unit/transport/websocket/utils.py`

 * *Files identical despite different names*

### Comparing `zaqar-9.0.0.0rc1/zaqar/tests/unit/cmd/test_status.py` & `zaqar-9.0.1/zaqar/tests/unit/cmd/test_status.py`

 * *Files identical despite different names*

### Comparing `zaqar-9.0.0.0rc1/zaqar/tests/unit/test_bootstrap.py` & `zaqar-9.0.1/zaqar/tests/unit/test_bootstrap.py`

 * *Files identical despite different names*

### Comparing `zaqar-9.0.0.0rc1/zaqar/tests/unit/hacking/test_hacking.py` & `zaqar-9.0.1/zaqar/tests/unit/hacking/test_hacking.py`

 * *Files identical despite different names*

### Comparing `zaqar-9.0.0.0rc1/zaqar/tests/base.py` & `zaqar-9.0.1/zaqar/tests/base.py`

 * *Files identical despite different names*

### Comparing `zaqar-9.0.0.0rc1/zaqar/tests/faulty_storage.py` & `zaqar-9.0.1/zaqar/tests/faulty_storage.py`

 * *Files identical despite different names*

### Comparing `zaqar-9.0.0.0rc1/zaqar/locale/en_GB/LC_MESSAGES/zaqar.po` & `zaqar-9.0.1/zaqar/locale/en_GB/LC_MESSAGES/zaqar.po`

 * *Files identical despite different names*

### Comparing `zaqar-9.0.0.0rc1/zaqar/locale/es/LC_MESSAGES/zaqar.po` & `zaqar-9.0.1/zaqar/locale/es/LC_MESSAGES/zaqar.po`

 * *Files identical despite different names*

### Comparing `zaqar-9.0.0.0rc1/zaqar/locale/id/LC_MESSAGES/zaqar.po` & `zaqar-9.0.1/zaqar/locale/id/LC_MESSAGES/zaqar.po`

 * *Files identical despite different names*

### Comparing `zaqar-9.0.0.0rc1/zaqar/locale/de/LC_MESSAGES/zaqar.po` & `zaqar-9.0.1/zaqar/locale/de/LC_MESSAGES/zaqar.po`

 * *Files 3% similar despite different names*

```diff
@@ -1,33 +1,42 @@
 # Frank Kloeker <eumel@arcor.de>, 2018. #zanata
 # Robert Simai <robert.simai@suse.com>, 2018. #zanata
+# Andreas Jaeger <jaegerandi@gmail.com>, 2019. #zanata
 # Robert Simai <robert.simai@suse.com>, 2019. #zanata
 msgid ""
 msgstr ""
 "Project-Id-Version: zaqar VERSION\n"
 "Report-Msgid-Bugs-To: https://bugs.launchpad.net/openstack-i18n/\n"
-"POT-Creation-Date: 2019-04-25 08:05+0000\n"
+"POT-Creation-Date: 2019-09-09 01:27+0000\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"PO-Revision-Date: 2019-05-03 01:56+0000\n"
-"Last-Translator: Robert Simai <robert.simai@suse.com>\n"
+"PO-Revision-Date: 2019-09-26 06:28+0000\n"
+"Last-Translator: Andreas Jaeger <jaegerandi@gmail.com>\n"
 "Language-Team: German\n"
 "Language: de\n"
 "X-Generator: Zanata 4.3.3\n"
 "Plural-Forms: nplurals=2; plural=(n != 1)\n"
 
 #, python-format
 msgid ""
 "%(attempts)d attempt(s) required to post %(num_messages)d messages to queue "
 "\"%(queue)s\" under project %(project)s"
 msgstr ""
 "%(attempts)d Versuche erforderlich, um %(num_messages)d Nachrichten in die "
 "Warteschlange \"%(queue)s\" unter Projekt %(project)s zu stellen"
 
+#, python-format
+msgid ""
+"%(attempts)d attempt(s) required to post %(num_messages)d messages to queue "
+"\"%(topic)s\" under project %(project)s"
+msgstr ""
+"%(attempts)d Versuche erforderlich, um %(num_messages)d Nachrichten in die "
+"Warteschlange \"%(topic)s\" unter Projekt %(project)s zu stellen"
+
 msgid "A claim was specified, but the message is not currently claimed."
 msgstr ""
 "Ein Auftrag wurde angegeben, aber die Nachricht wird derzeit nicht in "
 "Anspruch genommen."
 
 #, python-format
 msgid "Accepted media type for PATCH: %s."
@@ -135,21 +144,37 @@
 "%(project)s"
 msgstr ""
 "Fehler beim Inkrementieren des Nachrichtenzählers für die Warteschlangen "
 "%(name)s und Projekt %(project)s"
 
 #, python-format
 msgid ""
+"Failed to increment the message counter for topic %(name)s and project "
+"%(project)s"
+msgstr ""
+"Fehler beim Inkrementieren des Nachrichtenzählers für Topic %(name)s und "
+"Projekt %(project)s"
+
+#, python-format
+msgid ""
 "First attempt failed while adding messages to queue \"%(queue)s\" under "
 "project %(project)s"
 msgstr ""
 "Der erste Versuch ist beim Hinzufügen von Nachrichten zur Warteschlange "
 "\"%(queue)s\" unter Projekt %(project)s fehlgeschlagen"
 
 #, python-format
+msgid ""
+"First attempt failed while adding messages to topic \"%(topic)s\" under "
+"project %(project)s"
+msgstr ""
+"Der erste Versuch ist beim Hinzufügen von Nachrichten zum Topic \"%(topic)s"
+"\" unter Projekt %(project)s fehlgeschlagen"
+
+#, python-format
 msgid "Flavor %(flavor)s cant be updated, error:%(msg)s"
 msgstr "Variante %(flavor)s kann nicht aktualisiert werden, Fehler: %(msg)s"
 
 #, python-format
 msgid "Flavor %(flavor)s could not be created, error:%(msg)s"
 msgstr "Variante %(flavor)s konnte nicht erstellt werden, Fehler: %(msg)s"
 
@@ -333,14 +358,22 @@
 "Pipeline to use for processing subscription operations. This pipeline will "
 "be consumed before calling the storage driver's controller methods."
 msgstr ""
 "Pipeline für die Verarbeitung von Abonnementvorgängen. Diese Pipeline wird "
 "verbraucht, bevor die Controller-Methoden des Speichertreibers aufgerufen "
 "werden."
 
+msgid ""
+"Pipeline to use for processing topic operations. This pipeline will be "
+"consumed before calling the storage driver's controller methods."
+msgstr ""
+"Pipeline für die Verarbeitung von Topicorgängen. Diese Pipeline wird "
+"verbraucht, bevor die Controller-Methoden des Speichertreibers aufgerufen "
+"werden."
+
 msgid "Placeholder"
 msgstr "Platzhalter"
 
 msgid "Please try again in a few seconds."
 msgstr "Bitte versuchen Sie es in einigen Sekunden erneut."
 
 #, python-format
@@ -586,14 +619,18 @@
 "als {0} sein."
 
 msgid "The format of the submitted queue name or project id is not valid."
 msgstr ""
 "Das Format des gesendeten Warteschlangennamens oder der Projekt-ID ist nicht "
 "gültig."
 
+msgid "The format of the submitted topic name or project id is not valid."
+msgstr ""
+"Das Format des gesendetenTopic-Namens oder der Projekt-ID ist nicht gültig."
+
 msgid ""
 "The grace for a claim may not exceed {0} seconds, and must be at least {1} "
 "seconds long."
 msgstr ""
 "Die Gnadenfrist für eine Forderung darf nicht länger als {0} Sekunden und "
 "muss mindestens {1} Sekunden betragen."
 
@@ -637,14 +674,44 @@
 "gelöscht werden."
 
 msgid "This pool is used by flavors {flavor}; It cannot be deleted."
 msgstr ""
 "Dieser Pool wird von Variante {flavor} verwendet. Es kann nicht gelöscht "
 "werden."
 
+msgid "Topic could not be created."
+msgstr "Topic konnte nicht erstellt werden."
+
+msgid "Topic could not be deleted."
+msgstr "Topic konnte nicht gelöscht werden."
+
+msgid "Topic could not be purged."
+msgstr "Topic konnte nicht gelöscht werden."
+
+msgid "Topic could not be updated."
+msgstr "Topic konnte nicht aktualisiert werden."
+
+msgid "Topic metadata could not be retrieved."
+msgstr "Topic-Metadaten konnten nicht abgerufen werden."
+
+msgid "Topic names may not be more than {0} characters long."
+msgstr "Topic-Namen dürfen nicht länger als {0} Zeichen lang sein."
+
+msgid ""
+"Topic names may only contain ASCII letters, digits, underscores, and dashes."
+msgstr ""
+"Topic-Namen dürfen nur ASCII-Buchstaben, Ziffern, Unterstriche und "
+"Bindestriche enthalten."
+
+msgid "Topic stats could not be read."
+msgstr "Topicstatistiken konnten nicht gelesen werden."
+
+msgid "Topics could not be listed."
+msgstr "Topi konnten nicht aufgelistet werden."
+
 msgid "Unable to confirm subscription"
 msgstr "Das Abonnement konnte nicht bestätigt werden"
 
 msgid "Unable to create"
 msgstr "Konnte nicht erstellen"
 
 msgid "Unable to create pool"
@@ -744,14 +811,18 @@
 "Pop- und ID-Parameter können nicht zusammen in der Löschanforderung "
 "vorhanden sein."
 
 msgid "register queue to pool: new flavor: None"
 msgstr "Registriere Warteschlange zu Pool: neuer Variante: Keine"
 
 #, python-format
+msgid "register queue to pool: new flavor:%(flavor)s"
+msgstr "registriere Warteschlange zu Pool: neue Variante:%(flavor)s"
+
+#, python-format
 msgid ""
 "register queue to pool: old flavor: %(oldflavor)s , new flavor: %(flavor)s"
 msgstr ""
 "Registrere Warteschlange zu Pool: alte Variante: %(oldflavor)s, neue "
 "Variante: %(flavor)s"
 
 #, python-format
```

### Comparing `zaqar-9.0.0.0rc1/zaqar/cmd/gc.py` & `zaqar-9.0.1/zaqar/cmd/gc.py`

 * *Files identical despite different names*

### Comparing `zaqar-9.0.0.0rc1/zaqar/cmd/status.py` & `zaqar-9.0.1/zaqar/cmd/status.py`

 * *Files identical despite different names*

### Comparing `zaqar-9.0.0.0rc1/zaqar/cmd/server.py` & `zaqar-9.0.1/zaqar/cmd/server.py`

 * *Files identical despite different names*

### Comparing `zaqar-9.0.0.0rc1/zaqar/i18n.py` & `zaqar-9.0.1/zaqar/i18n.py`

 * *Files identical despite different names*

### Comparing `zaqar-9.0.0.0rc1/zaqar/context.py` & `zaqar-9.0.1/zaqar/context.py`

 * *Files identical despite different names*

### Comparing `zaqar-9.0.0.0rc1/zaqar/hacking/checks.py` & `zaqar-9.0.1/zaqar/hacking/checks.py`

 * *Files identical despite different names*

### Comparing `zaqar-9.0.0.0rc1/zaqar/bootstrap.py` & `zaqar-9.0.1/zaqar/bootstrap.py`

 * *Files identical despite different names*

### Comparing `zaqar-9.0.0.0rc1/test-requirements.txt` & `zaqar-9.0.1/test-requirements.txt`

 * *Files identical despite different names*

### Comparing `zaqar-9.0.0.0rc1/tools/test-setup.sh` & `zaqar-9.0.1/tools/test-setup.sh`

 * *Files identical despite different names*

### Comparing `zaqar-9.0.0.0rc1/tools/doc/generate_autodoc_index.sh` & `zaqar-9.0.1/tools/doc/generate_autodoc_index.sh`

 * *Files identical despite different names*

### Comparing `zaqar-9.0.0.0rc1/lower-constraints.txt` & `zaqar-9.0.1/lower-constraints.txt`

 * *Files identical despite different names*

### Comparing `zaqar-9.0.0.0rc1/README.rst` & `zaqar-9.0.1/README.rst`

 * *Files identical despite different names*

### Comparing `zaqar-9.0.0.0rc1/zaqar.egg-info/PKG-INFO` & `zaqar-9.0.1/zaqar.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: zaqar
-Version: 9.0.0.0rc1
+Version: 9.0.1
 Summary: OpenStack Queuing and Notification Service
 Home-page: https://docs.openstack.org/zaqar/latest/
 Author: OpenStack
 Author-email: openstack-discuss@lists.openstack.org
 License: UNKNOWN
 Description: ========================
         Team and repository tags
```

### Comparing `zaqar-9.0.0.0rc1/zaqar.egg-info/requires.txt` & `zaqar-9.0.1/zaqar.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `zaqar-9.0.0.0rc1/zaqar.egg-info/SOURCES.txt` & `zaqar-9.0.1/zaqar.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -200,18 +200,14 @@
 releasenotes/source/pike.rst
 releasenotes/source/queens.rst
 releasenotes/source/rocky.rst
 releasenotes/source/stein.rst
 releasenotes/source/unreleased.rst
 releasenotes/source/_static/.gitignore
 releasenotes/source/_templates/.gitignore
-releasenotes/source/locale/de/LC_MESSAGES/releasenotes.po
-releasenotes/source/locale/en_GB/LC_MESSAGES/releasenotes.po
-releasenotes/source/locale/fr/LC_MESSAGES/releasenotes.po
-releasenotes/source/locale/id/LC_MESSAGES/releasenotes.po
 samples/html/confirmation_web_service_sample.py
 samples/html/subscriptionConfirmation.html
 samples/html/unsubscriptionConfirmation.html
 samples/java-api-for-websocket/receive_message/JsonDecoder.java
 samples/java-api-for-websocket/receive_message/SampleZaqarEndpoint.java
 samples/java-api-for-websocket/send_message/SampleZaqarEndpoint.java
 samples/javascript/websocket.html
```

### Comparing `zaqar-9.0.0.0rc1/zaqar.egg-info/entry_points.txt` & `zaqar-9.0.1/zaqar.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `zaqar-9.0.0.0rc1/ChangeLog` & `zaqar-9.0.1/ChangeLog`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,19 @@
 CHANGES
 =======
 
-9.0.0.0rc1
-----------
+9.0.1
+-----
+
+* Imported Translations from Zanata
+* Update TOX/UPPER\_CONSTRAINTS\_FILE for stable/train
+* Update .gitreview for stable/train
+
+9.0.0
+-----
 
 * Add zaqar-specs link to readme.rst
 * Quick fix for v1.1 api schema
 * Modify api schema for remove pool group
 * Fix api-ref link
 * Fit the StopIteration for py37
 * Update api-ref location
```

### Comparing `zaqar-9.0.0.0rc1/requirements.txt` & `zaqar-9.0.1/requirements.txt`

 * *Files identical despite different names*

### Comparing `zaqar-9.0.0.0rc1/HACKING.rst` & `zaqar-9.0.1/HACKING.rst`

 * *Files identical despite different names*

