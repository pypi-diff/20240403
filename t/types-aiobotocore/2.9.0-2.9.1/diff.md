# Comparing `tmp/types-aiobotocore-2.9.0.tar.gz` & `tmp/types-aiobotocore-2.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-2.9.0.tar", last modified: Wed Dec 13 19:58:26 2023, max compression
+gzip compressed data, was "types-aiobotocore-2.9.1.tar", last modified: Thu Jan 18 01:19:55 2024, max compression
```

## Comparing `types-aiobotocore-2.9.0.tar` & `types-aiobotocore-2.9.1.tar`

### file list

```diff
@@ -1,39 +1,40 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:58:26.466164 types-aiobotocore-2.9.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2023-12-13 19:40:28.000000 types-aiobotocore-2.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    85455 2023-12-13 19:58:26.466164 types-aiobotocore-2.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    73164 2023-12-13 19:40:28.000000 types-aiobotocore-2.9.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:58:26.466164 types-aiobotocore-2.9.0/aiobotocore-stubs/
--rw-r--r--   0 runner    (1001) docker     (127)       17 2023-12-13 19:40:26.000000 types-aiobotocore-2.9.0/aiobotocore-stubs/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1628 2023-12-13 19:40:26.000000 types-aiobotocore-2.9.0/aiobotocore-stubs/args.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      175 2023-12-13 19:40:26.000000 types-aiobotocore-2.9.0/aiobotocore-stubs/awsrequest.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1349 2023-12-13 19:40:26.000000 types-aiobotocore-2.9.0/aiobotocore-stubs/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      300 2023-12-13 19:40:26.000000 types-aiobotocore-2.9.0/aiobotocore-stubs/config.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      399 2023-12-13 19:40:26.000000 types-aiobotocore-2.9.0/aiobotocore-stubs/configprovider.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     5723 2023-12-13 19:40:26.000000 types-aiobotocore-2.9.0/aiobotocore-stubs/credentials.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      477 2023-12-13 19:40:26.000000 types-aiobotocore-2.9.0/aiobotocore-stubs/discovery.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1467 2023-12-13 19:40:26.000000 types-aiobotocore-2.9.0/aiobotocore-stubs/endpoint.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      394 2023-12-13 19:40:26.000000 types-aiobotocore-2.9.0/aiobotocore-stubs/eventstream.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      595 2023-12-13 19:40:26.000000 types-aiobotocore-2.9.0/aiobotocore-stubs/handlers.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      261 2023-12-13 19:40:26.000000 types-aiobotocore-2.9.0/aiobotocore-stubs/hooks.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      643 2023-12-13 19:40:26.000000 types-aiobotocore-2.9.0/aiobotocore-stubs/httpchecksum.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      960 2023-12-13 19:40:26.000000 types-aiobotocore-2.9.0/aiobotocore-stubs/httpsession.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      732 2023-12-13 19:40:26.000000 types-aiobotocore-2.9.0/aiobotocore-stubs/paginate.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      745 2023-12-13 19:40:26.000000 types-aiobotocore-2.9.0/aiobotocore-stubs/parsers.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-13 19:40:30.000000 types-aiobotocore-2.9.0/aiobotocore-stubs/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)      541 2023-12-13 19:40:26.000000 types-aiobotocore-2.9.0/aiobotocore-stubs/regions.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1381 2023-12-13 19:40:26.000000 types-aiobotocore-2.9.0/aiobotocore-stubs/response.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      819 2023-12-13 19:40:26.000000 types-aiobotocore-2.9.0/aiobotocore-stubs/retryhandler.pyi
--rw-r--r--   0 runner    (1001) docker     (127)   227048 2023-12-13 19:40:30.000000 types-aiobotocore-2.9.0/aiobotocore-stubs/session.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2182 2023-12-13 19:40:26.000000 types-aiobotocore-2.9.0/aiobotocore-stubs/signers.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      775 2023-12-13 19:40:26.000000 types-aiobotocore-2.9.0/aiobotocore-stubs/tokens.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2147 2023-12-13 19:40:26.000000 types-aiobotocore-2.9.0/aiobotocore-stubs/utils.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      581 2023-12-13 19:40:26.000000 types-aiobotocore-2.9.0/aiobotocore-stubs/waiter.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-13 19:58:26.466164 types-aiobotocore-2.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)    54001 2023-12-13 19:40:27.000000 types-aiobotocore-2.9.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 19:58:26.466164 types-aiobotocore-2.9.0/types_aiobotocore.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    85455 2023-12-13 19:58:26.000000 types-aiobotocore-2.9.0/types_aiobotocore.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1045 2023-12-13 19:58:26.000000 types-aiobotocore-2.9.0/types_aiobotocore.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 19:58:26.000000 types-aiobotocore-2.9.0/types_aiobotocore.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 19:58:26.000000 types-aiobotocore-2.9.0/types_aiobotocore.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)    40320 2023-12-13 19:58:26.000000 types-aiobotocore-2.9.0/types_aiobotocore.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2023-12-13 19:58:26.000000 types-aiobotocore-2.9.0/types_aiobotocore.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:19:55.485550 types-aiobotocore-2.9.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-01-18 01:02:26.000000 types-aiobotocore-2.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)   146624 2024-01-18 01:19:55.485550 types-aiobotocore-2.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    73164 2024-01-18 01:02:26.000000 types-aiobotocore-2.9.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:19:55.389550 types-aiobotocore-2.9.1/aiobotocore-stubs/
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-01-18 01:02:25.000000 types-aiobotocore-2.9.1/aiobotocore-stubs/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1628 2024-01-18 01:02:25.000000 types-aiobotocore-2.9.1/aiobotocore-stubs/args.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      175 2024-01-18 01:02:25.000000 types-aiobotocore-2.9.1/aiobotocore-stubs/awsrequest.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1349 2024-01-18 01:02:25.000000 types-aiobotocore-2.9.1/aiobotocore-stubs/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      300 2024-01-18 01:02:25.000000 types-aiobotocore-2.9.1/aiobotocore-stubs/config.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      399 2024-01-18 01:02:25.000000 types-aiobotocore-2.9.1/aiobotocore-stubs/configprovider.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     5912 2024-01-18 01:02:25.000000 types-aiobotocore-2.9.1/aiobotocore-stubs/credentials.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      477 2024-01-18 01:02:25.000000 types-aiobotocore-2.9.1/aiobotocore-stubs/discovery.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1467 2024-01-18 01:02:25.000000 types-aiobotocore-2.9.1/aiobotocore-stubs/endpoint.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      394 2024-01-18 01:02:25.000000 types-aiobotocore-2.9.1/aiobotocore-stubs/eventstream.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      595 2024-01-18 01:02:25.000000 types-aiobotocore-2.9.1/aiobotocore-stubs/handlers.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      261 2024-01-18 01:02:25.000000 types-aiobotocore-2.9.1/aiobotocore-stubs/hooks.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      643 2024-01-18 01:02:25.000000 types-aiobotocore-2.9.1/aiobotocore-stubs/httpchecksum.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      960 2024-01-18 01:02:25.000000 types-aiobotocore-2.9.1/aiobotocore-stubs/httpsession.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      732 2024-01-18 01:02:25.000000 types-aiobotocore-2.9.1/aiobotocore-stubs/paginate.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      745 2024-01-18 01:02:25.000000 types-aiobotocore-2.9.1/aiobotocore-stubs/parsers.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-18 01:02:30.000000 types-aiobotocore-2.9.1/aiobotocore-stubs/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)      541 2024-01-18 01:02:25.000000 types-aiobotocore-2.9.1/aiobotocore-stubs/regions.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1381 2024-01-18 01:02:25.000000 types-aiobotocore-2.9.1/aiobotocore-stubs/response.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      819 2024-01-18 01:02:25.000000 types-aiobotocore-2.9.1/aiobotocore-stubs/retryhandler.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)   227048 2024-01-18 01:02:30.000000 types-aiobotocore-2.9.1/aiobotocore-stubs/session.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2182 2024-01-18 01:02:25.000000 types-aiobotocore-2.9.1/aiobotocore-stubs/signers.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      537 2024-01-18 01:02:25.000000 types-aiobotocore-2.9.1/aiobotocore-stubs/stub.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      775 2024-01-18 01:02:25.000000 types-aiobotocore-2.9.1/aiobotocore-stubs/tokens.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2162 2024-01-18 01:02:25.000000 types-aiobotocore-2.9.1/aiobotocore-stubs/utils.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      581 2024-01-18 01:02:25.000000 types-aiobotocore-2.9.1/aiobotocore-stubs/waiter.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-18 01:19:55.485550 types-aiobotocore-2.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)    53952 2024-01-18 01:02:25.000000 types-aiobotocore-2.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 01:19:55.389550 types-aiobotocore-2.9.1/types_aiobotocore.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)   146624 2024-01-18 01:19:55.000000 types-aiobotocore-2.9.1/types_aiobotocore.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-01-18 01:19:55.000000 types-aiobotocore-2.9.1/types_aiobotocore.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:19:55.000000 types-aiobotocore-2.9.1/types_aiobotocore.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 01:19:55.000000 types-aiobotocore-2.9.1/types_aiobotocore.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)    40320 2024-01-18 01:19:55.000000 types-aiobotocore-2.9.1/types_aiobotocore.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-01-18 01:19:55.000000 types-aiobotocore-2.9.1/types_aiobotocore.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-2.9.0/LICENSE` & `types-aiobotocore-2.9.1/LICENSE`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2023 Vlad Emelianov
+Copyright (c) 2024 Vlad Emelianov
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `types-aiobotocore-2.9.0/PKG-INFO` & `types-aiobotocore-2.9.1/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,439 +1,29 @@
-Metadata-Version: 2.1
-Name: types-aiobotocore
-Version: 2.9.0
-Summary: Type annotations for aiobotocore 2.9.0 generated with mypy-boto3-builder 7.21.0
-Home-page: https://github.com/youtype/mypy_boto3_builder
-Author: Vlad Emelianov
-Author-email: vlad.emelianov.nz@gmail.com
-License: MIT License
-Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/
-Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
-Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: aiobotocore type-annotations aiobotocore-stubs botocore-stubs mypy typeshed autocomplete
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Intended Audience :: Developers
-Classifier: Environment :: Console
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Natural Language :: English
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
-Classifier: Programming Language :: Python :: 3.13
-Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: Implementation :: CPython
-Classifier: Typing :: Stubs Only
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-Provides-Extra: all
-Provides-Extra: essential
-Provides-Extra: aiobotocore
-Provides-Extra: accessanalyzer
-Provides-Extra: account
-Provides-Extra: acm
-Provides-Extra: acm-pca
-Provides-Extra: alexaforbusiness
-Provides-Extra: amp
-Provides-Extra: amplify
-Provides-Extra: amplifybackend
-Provides-Extra: amplifyuibuilder
-Provides-Extra: apigateway
-Provides-Extra: apigatewaymanagementapi
-Provides-Extra: apigatewayv2
-Provides-Extra: appconfig
-Provides-Extra: appconfigdata
-Provides-Extra: appfabric
-Provides-Extra: appflow
-Provides-Extra: appintegrations
-Provides-Extra: application-autoscaling
-Provides-Extra: application-insights
-Provides-Extra: applicationcostprofiler
-Provides-Extra: appmesh
-Provides-Extra: apprunner
-Provides-Extra: appstream
-Provides-Extra: appsync
-Provides-Extra: arc-zonal-shift
-Provides-Extra: athena
-Provides-Extra: auditmanager
-Provides-Extra: autoscaling
-Provides-Extra: autoscaling-plans
-Provides-Extra: b2bi
-Provides-Extra: backup
-Provides-Extra: backup-gateway
-Provides-Extra: backupstorage
-Provides-Extra: batch
-Provides-Extra: bcm-data-exports
-Provides-Extra: bedrock
-Provides-Extra: bedrock-agent
-Provides-Extra: bedrock-agent-runtime
-Provides-Extra: bedrock-runtime
-Provides-Extra: billingconductor
-Provides-Extra: braket
-Provides-Extra: budgets
-Provides-Extra: ce
-Provides-Extra: chime
-Provides-Extra: chime-sdk-identity
-Provides-Extra: chime-sdk-media-pipelines
-Provides-Extra: chime-sdk-meetings
-Provides-Extra: chime-sdk-messaging
-Provides-Extra: chime-sdk-voice
-Provides-Extra: cleanrooms
-Provides-Extra: cleanroomsml
-Provides-Extra: cloud9
-Provides-Extra: cloudcontrol
-Provides-Extra: clouddirectory
-Provides-Extra: cloudformation
-Provides-Extra: cloudfront
-Provides-Extra: cloudfront-keyvaluestore
-Provides-Extra: cloudhsm
-Provides-Extra: cloudhsmv2
-Provides-Extra: cloudsearch
-Provides-Extra: cloudsearchdomain
-Provides-Extra: cloudtrail
-Provides-Extra: cloudtrail-data
-Provides-Extra: cloudwatch
-Provides-Extra: codeartifact
-Provides-Extra: codebuild
-Provides-Extra: codecatalyst
-Provides-Extra: codecommit
-Provides-Extra: codedeploy
-Provides-Extra: codeguru-reviewer
-Provides-Extra: codeguru-security
-Provides-Extra: codeguruprofiler
-Provides-Extra: codepipeline
-Provides-Extra: codestar
-Provides-Extra: codestar-connections
-Provides-Extra: codestar-notifications
-Provides-Extra: cognito-identity
-Provides-Extra: cognito-idp
-Provides-Extra: cognito-sync
-Provides-Extra: comprehend
-Provides-Extra: comprehendmedical
-Provides-Extra: compute-optimizer
-Provides-Extra: config
-Provides-Extra: connect
-Provides-Extra: connect-contact-lens
-Provides-Extra: connectcampaigns
-Provides-Extra: connectcases
-Provides-Extra: connectparticipant
-Provides-Extra: controltower
-Provides-Extra: cost-optimization-hub
-Provides-Extra: cur
-Provides-Extra: customer-profiles
-Provides-Extra: databrew
-Provides-Extra: dataexchange
-Provides-Extra: datapipeline
-Provides-Extra: datasync
-Provides-Extra: datazone
-Provides-Extra: dax
-Provides-Extra: detective
-Provides-Extra: devicefarm
-Provides-Extra: devops-guru
-Provides-Extra: directconnect
-Provides-Extra: discovery
-Provides-Extra: dlm
-Provides-Extra: dms
-Provides-Extra: docdb
-Provides-Extra: docdb-elastic
-Provides-Extra: drs
-Provides-Extra: ds
-Provides-Extra: dynamodb
-Provides-Extra: dynamodbstreams
-Provides-Extra: ebs
-Provides-Extra: ec2
-Provides-Extra: ec2-instance-connect
-Provides-Extra: ecr
-Provides-Extra: ecr-public
-Provides-Extra: ecs
-Provides-Extra: efs
-Provides-Extra: eks
-Provides-Extra: eks-auth
-Provides-Extra: elastic-inference
-Provides-Extra: elasticache
-Provides-Extra: elasticbeanstalk
-Provides-Extra: elastictranscoder
-Provides-Extra: elb
-Provides-Extra: elbv2
-Provides-Extra: emr
-Provides-Extra: emr-containers
-Provides-Extra: emr-serverless
-Provides-Extra: entityresolution
-Provides-Extra: es
-Provides-Extra: events
-Provides-Extra: evidently
-Provides-Extra: finspace
-Provides-Extra: finspace-data
-Provides-Extra: firehose
-Provides-Extra: fis
-Provides-Extra: fms
-Provides-Extra: forecast
-Provides-Extra: forecastquery
-Provides-Extra: frauddetector
-Provides-Extra: freetier
-Provides-Extra: fsx
-Provides-Extra: gamelift
-Provides-Extra: glacier
-Provides-Extra: globalaccelerator
-Provides-Extra: glue
-Provides-Extra: grafana
-Provides-Extra: greengrass
-Provides-Extra: greengrassv2
-Provides-Extra: groundstation
-Provides-Extra: guardduty
-Provides-Extra: health
-Provides-Extra: healthlake
-Provides-Extra: honeycode
-Provides-Extra: iam
-Provides-Extra: identitystore
-Provides-Extra: imagebuilder
-Provides-Extra: importexport
-Provides-Extra: inspector
-Provides-Extra: inspector-scan
-Provides-Extra: inspector2
-Provides-Extra: internetmonitor
-Provides-Extra: iot
-Provides-Extra: iot-data
-Provides-Extra: iot-jobs-data
-Provides-Extra: iot-roborunner
-Provides-Extra: iot1click-devices
-Provides-Extra: iot1click-projects
-Provides-Extra: iotanalytics
-Provides-Extra: iotdeviceadvisor
-Provides-Extra: iotevents
-Provides-Extra: iotevents-data
-Provides-Extra: iotfleethub
-Provides-Extra: iotfleetwise
-Provides-Extra: iotsecuretunneling
-Provides-Extra: iotsitewise
-Provides-Extra: iotthingsgraph
-Provides-Extra: iottwinmaker
-Provides-Extra: iotwireless
-Provides-Extra: ivs
-Provides-Extra: ivs-realtime
-Provides-Extra: ivschat
-Provides-Extra: kafka
-Provides-Extra: kafkaconnect
-Provides-Extra: kendra
-Provides-Extra: kendra-ranking
-Provides-Extra: keyspaces
-Provides-Extra: kinesis
-Provides-Extra: kinesis-video-archived-media
-Provides-Extra: kinesis-video-media
-Provides-Extra: kinesis-video-signaling
-Provides-Extra: kinesis-video-webrtc-storage
-Provides-Extra: kinesisanalytics
-Provides-Extra: kinesisanalyticsv2
-Provides-Extra: kinesisvideo
-Provides-Extra: kms
-Provides-Extra: lakeformation
-Provides-Extra: lambda
-Provides-Extra: launch-wizard
-Provides-Extra: lex-models
-Provides-Extra: lex-runtime
-Provides-Extra: lexv2-models
-Provides-Extra: lexv2-runtime
-Provides-Extra: license-manager
-Provides-Extra: license-manager-linux-subscriptions
-Provides-Extra: license-manager-user-subscriptions
-Provides-Extra: lightsail
-Provides-Extra: location
-Provides-Extra: logs
-Provides-Extra: lookoutequipment
-Provides-Extra: lookoutmetrics
-Provides-Extra: lookoutvision
-Provides-Extra: m2
-Provides-Extra: machinelearning
-Provides-Extra: macie2
-Provides-Extra: managedblockchain
-Provides-Extra: managedblockchain-query
-Provides-Extra: marketplace-agreement
-Provides-Extra: marketplace-catalog
-Provides-Extra: marketplace-deployment
-Provides-Extra: marketplace-entitlement
-Provides-Extra: marketplacecommerceanalytics
-Provides-Extra: mediaconnect
-Provides-Extra: mediaconvert
-Provides-Extra: medialive
-Provides-Extra: mediapackage
-Provides-Extra: mediapackage-vod
-Provides-Extra: mediapackagev2
-Provides-Extra: mediastore
-Provides-Extra: mediastore-data
-Provides-Extra: mediatailor
-Provides-Extra: medical-imaging
-Provides-Extra: memorydb
-Provides-Extra: meteringmarketplace
-Provides-Extra: mgh
-Provides-Extra: mgn
-Provides-Extra: migration-hub-refactor-spaces
-Provides-Extra: migrationhub-config
-Provides-Extra: migrationhuborchestrator
-Provides-Extra: migrationhubstrategy
-Provides-Extra: mobile
-Provides-Extra: mq
-Provides-Extra: mturk
-Provides-Extra: mwaa
-Provides-Extra: neptune
-Provides-Extra: neptunedata
-Provides-Extra: network-firewall
-Provides-Extra: networkmanager
-Provides-Extra: nimble
-Provides-Extra: oam
-Provides-Extra: omics
-Provides-Extra: opensearch
-Provides-Extra: opensearchserverless
-Provides-Extra: opsworks
-Provides-Extra: opsworkscm
-Provides-Extra: organizations
-Provides-Extra: osis
-Provides-Extra: outposts
-Provides-Extra: panorama
-Provides-Extra: payment-cryptography
-Provides-Extra: payment-cryptography-data
-Provides-Extra: pca-connector-ad
-Provides-Extra: personalize
-Provides-Extra: personalize-events
-Provides-Extra: personalize-runtime
-Provides-Extra: pi
-Provides-Extra: pinpoint
-Provides-Extra: pinpoint-email
-Provides-Extra: pinpoint-sms-voice
-Provides-Extra: pinpoint-sms-voice-v2
-Provides-Extra: pipes
-Provides-Extra: polly
-Provides-Extra: pricing
-Provides-Extra: privatenetworks
-Provides-Extra: proton
-Provides-Extra: qbusiness
-Provides-Extra: qconnect
-Provides-Extra: qldb
-Provides-Extra: qldb-session
-Provides-Extra: quicksight
-Provides-Extra: ram
-Provides-Extra: rbin
-Provides-Extra: rds
-Provides-Extra: rds-data
-Provides-Extra: redshift
-Provides-Extra: redshift-data
-Provides-Extra: redshift-serverless
-Provides-Extra: rekognition
-Provides-Extra: repostspace
-Provides-Extra: resiliencehub
-Provides-Extra: resource-explorer-2
-Provides-Extra: resource-groups
-Provides-Extra: resourcegroupstaggingapi
-Provides-Extra: robomaker
-Provides-Extra: rolesanywhere
-Provides-Extra: route53
-Provides-Extra: route53-recovery-cluster
-Provides-Extra: route53-recovery-control-config
-Provides-Extra: route53-recovery-readiness
-Provides-Extra: route53domains
-Provides-Extra: route53resolver
-Provides-Extra: rum
-Provides-Extra: s3
-Provides-Extra: s3control
-Provides-Extra: s3outposts
-Provides-Extra: sagemaker
-Provides-Extra: sagemaker-a2i-runtime
-Provides-Extra: sagemaker-edge
-Provides-Extra: sagemaker-featurestore-runtime
-Provides-Extra: sagemaker-geospatial
-Provides-Extra: sagemaker-metrics
-Provides-Extra: sagemaker-runtime
-Provides-Extra: savingsplans
-Provides-Extra: scheduler
-Provides-Extra: schemas
-Provides-Extra: sdb
-Provides-Extra: secretsmanager
-Provides-Extra: securityhub
-Provides-Extra: securitylake
-Provides-Extra: serverlessrepo
-Provides-Extra: service-quotas
-Provides-Extra: servicecatalog
-Provides-Extra: servicecatalog-appregistry
-Provides-Extra: servicediscovery
-Provides-Extra: ses
-Provides-Extra: sesv2
-Provides-Extra: shield
-Provides-Extra: signer
-Provides-Extra: simspaceweaver
-Provides-Extra: sms
-Provides-Extra: sms-voice
-Provides-Extra: snow-device-management
-Provides-Extra: snowball
-Provides-Extra: sns
-Provides-Extra: sqs
-Provides-Extra: ssm
-Provides-Extra: ssm-contacts
-Provides-Extra: ssm-incidents
-Provides-Extra: ssm-sap
-Provides-Extra: sso
-Provides-Extra: sso-admin
-Provides-Extra: sso-oidc
-Provides-Extra: stepfunctions
-Provides-Extra: storagegateway
-Provides-Extra: sts
-Provides-Extra: support
-Provides-Extra: support-app
-Provides-Extra: swf
-Provides-Extra: synthetics
-Provides-Extra: textract
-Provides-Extra: timestream-query
-Provides-Extra: timestream-write
-Provides-Extra: tnb
-Provides-Extra: transcribe
-Provides-Extra: transfer
-Provides-Extra: translate
-Provides-Extra: trustedadvisor
-Provides-Extra: verifiedpermissions
-Provides-Extra: voice-id
-Provides-Extra: vpc-lattice
-Provides-Extra: waf
-Provides-Extra: waf-regional
-Provides-Extra: wafv2
-Provides-Extra: wellarchitected
-Provides-Extra: wisdom
-Provides-Extra: workdocs
-Provides-Extra: worklink
-Provides-Extra: workmail
-Provides-Extra: workmailmessageflow
-Provides-Extra: workspaces
-Provides-Extra: workspaces-thin-client
-Provides-Extra: workspaces-web
-Provides-Extra: xray
-License-File: LICENSE
-
 <a id="types-aiobotocore"></a>
 
 # types-aiobotocore
 
 [![PyPI - types-aiobotocore](https://img.shields.io/pypi/v/types-aiobotocore.svg?color=blue)](https://pypi.org/project/types-aiobotocore)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore.svg?color=blue)](https://pypi.org/project/types-aiobotocore)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore)](https://pepy.tech/project/types-aiobotocore)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[aiobotocore 2.9.0](https://github.com/aio-libs/aiobotocore) compatible with
+[aiobotocore 2.9.1](https://github.com/aio-libs/aiobotocore) compatible with
 [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.21.0](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.23.1](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found in
 [types-aiobotocore docs](https://youtype.github.io/types_aiobotocore_docs/).
 
 See how it helps to find and fix potential bugs:
 
 ![boto3-stubs demo](https://github.com/youtype/mypy_boto3_builder/raw/main/demo.gif)
```

### Comparing `types-aiobotocore-2.9.0/aiobotocore-stubs/args.pyi` & `types-aiobotocore-2.9.1/aiobotocore-stubs/args.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-2.9.0/aiobotocore-stubs/client.pyi` & `types-aiobotocore-2.9.1/aiobotocore-stubs/client.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-2.9.0/aiobotocore-stubs/credentials.pyi` & `types-aiobotocore-2.9.1/aiobotocore-stubs/credentials.pyi`

 * *Files 8% similar despite different names*

```diff
@@ -73,15 +73,15 @@
 
 class AioDeferredRefreshableCredentials(AioRefreshableCredentials):
     method: Any
     def __init__(self, refresh_using: Any, method: Any, time_fetcher: Any = ...) -> None: ...
     def refresh_needed(self, refresh_in: Optional[Any] = ...) -> bool: ...
 
 class AioCachedCredentialFetcher(CachedCredentialFetcher):
-    async def fetch_credentials(self) -> Any: ...
+    async def fetch_credentials(self) -> Any: ...  # type: ignore [override]
 
 class AioBaseAssumeRoleCredentialFetcher(
     BaseAssumeRoleCredentialFetcher, AioCachedCredentialFetcher
 ): ...
 class AioAssumeRoleCredentialFetcher(
     AssumeRoleCredentialFetcher, AioBaseAssumeRoleCredentialFetcher
 ): ...
@@ -95,30 +95,30 @@
         extra_args: Optional[Any] = ...,
         cache: Optional[Any] = ...,
         expiry_window_seconds: Optional[Any] = ...,
     ) -> None: ...
 
 class AioProcessProvider(ProcessProvider):
     def __init__(self, *args: Any, popen: Any = ..., **kwargs: Any) -> None: ...
-    async def load(self) -> AioCredentials: ...
+    async def load(self) -> AioCredentials: ...  # type: ignore [override]
 
 class AioInstanceMetadataProvider(InstanceMetadataProvider):
-    async def load(self) -> AioRefreshableCredentials: ...
+    async def load(self) -> AioRefreshableCredentials: ...  # type: ignore [override]
 
 class AioEnvProvider(EnvProvider):
-    async def load(self) -> Any: ...
+    async def load(self) -> Any: ...  # type: ignore [override]
 
 class AioOriginalEC2Provider(OriginalEC2Provider):
-    async def load(self) -> AioCredentials: ...
+    async def load(self) -> AioCredentials: ...  # type: ignore [override]
 
 class AioSharedCredentialProvider(SharedCredentialProvider):
-    async def load(self) -> AioCredentials: ...
+    async def load(self) -> AioCredentials: ...  # type: ignore [override]
 
 class AioConfigProvider(ConfigProvider):
-    async def load(self) -> AioCredentials: ...
+    async def load(self) -> AioCredentials: ...  # type: ignore [override]
 
 class AioBotoProvider(BotoProvider):
     async def load(self) -> AioCredentials: ...  # type: ignore [override]
 
 class AioAssumeRoleProvider(AssumeRoleProvider):
     async def load(self) -> AioDeferredRefreshableCredentials: ...  # type: ignore [override]
```

### Comparing `types-aiobotocore-2.9.0/aiobotocore-stubs/endpoint.pyi` & `types-aiobotocore-2.9.1/aiobotocore-stubs/endpoint.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-2.9.0/aiobotocore-stubs/handlers.pyi` & `types-aiobotocore-2.9.1/aiobotocore-stubs/handlers.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-2.9.0/aiobotocore-stubs/httpchecksum.pyi` & `types-aiobotocore-2.9.1/aiobotocore-stubs/httpchecksum.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-2.9.0/aiobotocore-stubs/httpsession.pyi` & `types-aiobotocore-2.9.1/aiobotocore-stubs/httpsession.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-2.9.0/aiobotocore-stubs/paginate.pyi` & `types-aiobotocore-2.9.1/aiobotocore-stubs/paginate.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-2.9.0/aiobotocore-stubs/parsers.pyi` & `types-aiobotocore-2.9.1/aiobotocore-stubs/parsers.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-2.9.0/aiobotocore-stubs/regions.pyi` & `types-aiobotocore-2.9.1/aiobotocore-stubs/regions.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-2.9.0/aiobotocore-stubs/response.pyi` & `types-aiobotocore-2.9.1/aiobotocore-stubs/response.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-2.9.0/aiobotocore-stubs/retryhandler.pyi` & `types-aiobotocore-2.9.1/aiobotocore-stubs/retryhandler.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-2.9.0/aiobotocore-stubs/session.pyi` & `types-aiobotocore-2.9.1/aiobotocore-stubs/session.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-2.9.0/aiobotocore-stubs/signers.pyi` & `types-aiobotocore-2.9.1/aiobotocore-stubs/signers.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-2.9.0/aiobotocore-stubs/tokens.pyi` & `types-aiobotocore-2.9.1/aiobotocore-stubs/tokens.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-2.9.0/aiobotocore-stubs/utils.pyi` & `types-aiobotocore-2.9.1/aiobotocore-stubs/utils.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Any, Dict, Optional
+from typing import Any, Dict, Mapping, Optional
 
 from botocore.utils import DEFAULT_METADATA_SERVICE_TIMEOUT as DEFAULT_METADATA_SERVICE_TIMEOUT
 from botocore.utils import METADATA_BASE_URL as METADATA_BASE_URL
 from botocore.utils import (
     ContainerMetadataFetcher,
     IMDSFetcher,
     IMDSRegionProvider,
@@ -36,24 +36,24 @@
 
 class AioInstanceMetadataRegionFetcher(AioIMDSFetcher, InstanceMetadataRegionFetcher):
     async def retrieve_region(self) -> Optional[str]: ...  # type: ignore [override]
 
 class AioS3RegionRedirectorv2(S3RegionRedirectorv2):
     async def redirect_from_error(
         self,
-        request_dict: Dict[str, Any],
+        request_dict: Mapping[str, Any],
         response: Response,
         operation: Any,
         **kwargs: Any,
     ) -> None: ...
     async def get_bucket_region(self, bucket: Any, response: Response) -> Any: ...
 
 class AioS3RegionRedirector(S3RegionRedirector):
     async def redirect_from_error(
-        self, request_dict: Dict[str, Any], response: Response, operation: Any, **kwargs: Any
+        self, request_dict: Mapping[str, Any], response: Response, operation: Any, **kwargs: Any
     ) -> Optional[int]: ...
     async def get_bucket_region(self, bucket: str, response: Response) -> str: ...
 
 class AioContainerMetadataFetcher(ContainerMetadataFetcher):
     def __init__(self, session: Optional[Any] = ..., sleep: Any = ...) -> None: ...
     async def retrieve_full_uri(self, full_url: str, headers: Optional[Any] = ...) -> str: ...
     async def retrieve_uri(self, relative_uri: str) -> Any: ...
```

### Comparing `types-aiobotocore-2.9.0/aiobotocore-stubs/waiter.pyi` & `types-aiobotocore-2.9.1/aiobotocore-stubs/waiter.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-2.9.0/setup.py` & `types-aiobotocore-2.9.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,30 +7,29 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore",
-    version="2.9.0",
+    version="2.9.1",
     packages=["aiobotocore-stubs"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
-    description="Type annotations for aiobotocore 2.9.0 generated with mypy-boto3-builder 7.21.0",
+    description="Type annotations for aiobotocore 2.9.1 generated with mypy-boto3-builder 7.23.1",
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
         "Operating System :: OS Independent",
         "Programming Language :: Python :: 3",
-        "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
         "Programming Language :: Python :: 3.12",
         "Programming Language :: Python :: 3.13",
         "Programming Language :: Python :: 3 :: Only",
@@ -39,15 +38,15 @@
     ],
     keywords=(
         "aiobotocore type-annotations aiobotocore-stubs botocore-stubs mypy typeshed autocomplete"
     ),
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"aiobotocore-stubs": ["py.typed", "*.pyi", "*/*.pyi"]},
-    python_requires=">=3.7",
+    python_requires=">=3.8",
     project_urls={
         "Documentation": "https://youtype.github.io/types_aiobotocore_docs/",
         "Source": "https://github.com/youtype/mypy_boto3_builder",
         "Tracker": "https://github.com/youtype/mypy_boto3_builder/issues",
     },
     install_requires=[
         "botocore-stubs",
@@ -435,15 +434,15 @@
             "types-aiobotocore-dynamodb>=2.9.0, <2.10.0",
             "types-aiobotocore-ec2>=2.9.0, <2.10.0",
             "types-aiobotocore-lambda>=2.9.0, <2.10.0",
             "types-aiobotocore-rds>=2.9.0, <2.10.0",
             "types-aiobotocore-s3>=2.9.0, <2.10.0",
             "types-aiobotocore-sqs>=2.9.0, <2.10.0",
         ],
-        "aiobotocore": ["aiobotocore==2.9.0", "botocore==1.33.13"],
+        "aiobotocore": ["aiobotocore==2.9.1", "botocore==1.33.13"],
         "accessanalyzer": ["types-aiobotocore-accessanalyzer>=2.9.0, <2.10.0"],
         "account": ["types-aiobotocore-account>=2.9.0, <2.10.0"],
         "acm": ["types-aiobotocore-acm>=2.9.0, <2.10.0"],
         "acm-pca": ["types-aiobotocore-acm-pca>=2.9.0, <2.10.0"],
         "alexaforbusiness": ["types-aiobotocore-alexaforbusiness>=2.9.0, <2.10.0"],
         "amp": ["types-aiobotocore-amp>=2.9.0, <2.10.0"],
         "amplify": ["types-aiobotocore-amplify>=2.9.0, <2.10.0"],
```

### Comparing `types-aiobotocore-2.9.0/types_aiobotocore.egg-info/SOURCES.txt` & `types-aiobotocore-2.9.1/types_aiobotocore.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -19,14 +19,15 @@
 aiobotocore-stubs/parsers.pyi
 aiobotocore-stubs/py.typed
 aiobotocore-stubs/regions.pyi
 aiobotocore-stubs/response.pyi
 aiobotocore-stubs/retryhandler.pyi
 aiobotocore-stubs/session.pyi
 aiobotocore-stubs/signers.pyi
+aiobotocore-stubs/stub.pyi
 aiobotocore-stubs/tokens.pyi
 aiobotocore-stubs/utils.pyi
 aiobotocore-stubs/waiter.pyi
 types_aiobotocore.egg-info/PKG-INFO
 types_aiobotocore.egg-info/SOURCES.txt
 types_aiobotocore.egg-info/dependency_links.txt
 types_aiobotocore.egg-info/not-zip-safe
```

### Comparing `types-aiobotocore-2.9.0/types_aiobotocore.egg-info/requires.txt` & `types-aiobotocore-2.9.1/types_aiobotocore.egg-info/requires.txt`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 [acm]
 types-aiobotocore-acm<2.10.0,>=2.9.0
 
 [acm-pca]
 types-aiobotocore-acm-pca<2.10.0,>=2.9.0
 
 [aiobotocore]
-aiobotocore==2.9.0
+aiobotocore==2.9.1
 botocore==1.33.13
 
 [alexaforbusiness]
 types-aiobotocore-alexaforbusiness<2.10.0,>=2.9.0
 
 [all]
 types-aiobotocore-accessanalyzer<2.10.0,>=2.9.0
```

