# Comparing `tmp/sawsi-9.8.tar.gz` & `tmp/sawsi-9.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sawsi-9.8.tar", last modified: Wed Feb  7 03:46:28 2024, max compression
+gzip compressed data, was "sawsi-9.9.tar", last modified: Wed Feb  7 03:52:50 2024, max compression
```

## Comparing `sawsi-9.8.tar` & `sawsi-9.9.tar`

### file list

```diff
@@ -1,110 +1,110 @@
-drwxr-xr-x   0 kch        (501) staff       (20)        0 2024-02-07 03:46:28.980984 sawsi-9.8/
--rw-r--r--   0 kch        (501) staff       (20)     1069 2023-09-07 22:50:01.000000 sawsi-9.8/LICENSE
--rw-r--r--   0 kch        (501) staff       (20)      129 2024-02-07 03:46:28.980675 sawsi-9.8/PKG-INFO
--rw-r--r--   0 kch        (501) staff       (20)     6982 2024-02-07 01:10:06.000000 sawsi-9.8/README.md
--rw-r--r--   0 kch        (501) staff       (20)     4428 2024-02-07 03:44:57.000000 sawsi-9.8/make.py
-drwxr-xr-x   0 kch        (501) staff       (20)        0 2024-02-07 03:46:28.966979 sawsi-9.8/sawsi/
--rw-r--r--   0 kch        (501) staff       (20)        0 2023-09-07 22:56:42.000000 sawsi-9.8/sawsi/__init__.py
-drwxr-xr-x   0 kch        (501) staff       (20)        0 2024-02-07 03:46:28.968277 sawsi-9.8/sawsi/api_doc/
--rw-r--r--   0 kch        (501) staff       (20)        0 2023-12-22 01:38:29.000000 sawsi-9.8/sawsi/api_doc/__init__.py
--rw-r--r--   0 kch        (501) staff       (20)     8094 2023-12-26 06:25:28.000000 sawsi-9.8/sawsi/api_doc/doc_generator.py
-drwxr-xr-x   0 kch        (501) staff       (20)        0 2024-02-07 03:46:28.968567 sawsi-9.8/sawsi/aws/
--rw-r--r--   0 kch        (501) staff       (20)        0 2023-07-06 05:55:04.000000 sawsi-9.8/sawsi/aws/__init__.py
-drwxr-xr-x   0 kch        (501) staff       (20)        0 2024-02-07 03:46:28.968885 sawsi-9.8/sawsi/aws/codecommit/
--rw-r--r--   0 kch        (501) staff       (20)        0 2023-07-06 05:55:04.000000 sawsi-9.8/sawsi/aws/codecommit/__init__.py
--rw-r--r--   0 kch        (501) staff       (20)      931 2023-09-09 02:33:57.000000 sawsi-9.8/sawsi/aws/codecommit/api.py
-drwxr-xr-x   0 kch        (501) staff       (20)        0 2024-02-07 03:46:28.969170 sawsi-9.8/sawsi/aws/cognito/
--rw-r--r--   0 kch        (501) staff       (20)        0 2023-09-08 00:30:19.000000 sawsi-9.8/sawsi/aws/cognito/__init__.py
--rw-r--r--   0 kch        (501) staff       (20)     7306 2023-09-08 04:22:27.000000 sawsi-9.8/sawsi/aws/cognito/api.py
-drwxr-xr-x   0 kch        (501) staff       (20)        0 2024-02-07 03:46:28.970189 sawsi-9.8/sawsi/aws/dynamodb/
--rw-r--r--   0 kch        (501) staff       (20)        0 2023-07-06 05:55:04.000000 sawsi-9.8/sawsi/aws/dynamodb/__init__.py
--rw-r--r--   0 kch        (501) staff       (20)    61057 2024-02-07 01:22:35.000000 sawsi-9.8/sawsi/aws/dynamodb/api.py
--rw-r--r--   0 kch        (501) staff       (20)      613 2023-07-06 05:55:04.000000 sawsi-9.8/sawsi/aws/dynamodb/config.py
--rw-r--r--   0 kch        (501) staff       (20)     4159 2023-12-29 05:24:55.000000 sawsi-9.8/sawsi/aws/dynamodb/util.py
--rw-r--r--   0 kch        (501) staff       (20)    40370 2024-02-06 07:50:13.000000 sawsi-9.8/sawsi/aws/dynamodb/wrapper.py
-drwxr-xr-x   0 kch        (501) staff       (20)        0 2024-02-07 03:46:28.970757 sawsi-9.8/sawsi/aws/firehose/
--rw-r--r--   0 kch        (501) staff       (20)        0 2023-10-26 00:43:42.000000 sawsi-9.8/sawsi/aws/firehose/__init__.py
--rw-r--r--   0 kch        (501) staff       (20)     7567 2023-10-27 06:48:49.000000 sawsi-9.8/sawsi/aws/firehose/api.py
--rw-r--r--   0 kch        (501) staff       (20)     1646 2023-10-26 01:25:24.000000 sawsi-9.8/sawsi/aws/firehose/wrapper.py
-drwxr-xr-x   0 kch        (501) staff       (20)        0 2024-02-07 03:46:28.971092 sawsi-9.8/sawsi/aws/iam/
--rw-r--r--   0 kch        (501) staff       (20)        0 2023-10-26 01:09:48.000000 sawsi-9.8/sawsi/aws/iam/__init__.py
--rw-r--r--   0 kch        (501) staff       (20)     1210 2023-10-26 01:58:59.000000 sawsi-9.8/sawsi/aws/iam/wrapper.py
-drwxr-xr-x   0 kch        (501) staff       (20)        0 2024-02-07 03:46:28.971570 sawsi-9.8/sawsi/aws/locking/
--rw-r--r--   0 kch        (501) staff       (20)        0 2023-10-25 09:05:43.000000 sawsi-9.8/sawsi/aws/locking/__init__.py
--rw-r--r--   0 kch        (501) staff       (20)     3438 2023-11-28 00:38:08.000000 sawsi-9.8/sawsi/aws/locking/api.py
--rw-r--r--   0 kch        (501) staff       (20)    19534 2023-09-09 01:04:51.000000 sawsi-9.8/sawsi/aws/locking/wrapper.py
-drwxr-xr-x   0 kch        (501) staff       (20)        0 2024-02-07 03:46:28.972061 sawsi-9.8/sawsi/aws/s3/
--rw-r--r--   0 kch        (501) staff       (20)        0 2023-07-06 05:55:04.000000 sawsi-9.8/sawsi/aws/s3/__init__.py
--rw-r--r--   0 kch        (501) staff       (20)     6255 2023-12-26 05:55:13.000000 sawsi-9.8/sawsi/aws/s3/api.py
--rw-r--r--   0 kch        (501) staff       (20)     3118 2023-10-26 02:22:17.000000 sawsi-9.8/sawsi/aws/s3/wrapper.py
-drwxr-xr-x   0 kch        (501) staff       (20)        0 2024-02-07 03:46:28.972541 sawsi-9.8/sawsi/aws/secrets_manager/
--rw-r--r--   0 kch        (501) staff       (20)        0 2023-07-06 05:55:04.000000 sawsi-9.8/sawsi/aws/secrets_manager/__init__.py
--rw-r--r--   0 kch        (501) staff       (20)     1468 2023-10-26 12:47:01.000000 sawsi-9.8/sawsi/aws/secrets_manager/api.py
--rw-r--r--   0 kch        (501) staff       (20)      525 2023-09-08 04:52:48.000000 sawsi-9.8/sawsi/aws/secrets_manager/wrapper.py
-drwxr-xr-x   0 kch        (501) staff       (20)        0 2024-02-07 03:46:28.972993 sawsi-9.8/sawsi/aws/ses/
--rw-r--r--   0 kch        (501) staff       (20)        0 2023-09-11 18:51:36.000000 sawsi-9.8/sawsi/aws/ses/__init__.py
--rw-r--r--   0 kch        (501) staff       (20)      802 2023-11-14 06:53:29.000000 sawsi-9.8/sawsi/aws/ses/api.py
--rw-r--r--   0 kch        (501) staff       (20)     1035 2023-11-14 06:29:02.000000 sawsi-9.8/sawsi/aws/ses/wrapper.py
--rw-r--r--   0 kch        (501) staff       (20)      882 2023-10-26 12:43:53.000000 sawsi-9.8/sawsi/aws/shared.py
-drwxr-xr-x   0 kch        (501) staff       (20)        0 2024-02-07 03:46:28.973455 sawsi-9.8/sawsi/aws/sms/
--rw-r--r--   0 kch        (501) staff       (20)        0 2023-09-05 01:18:09.000000 sawsi-9.8/sawsi/aws/sms/__init__.py
--rw-r--r--   0 kch        (501) staff       (20)      714 2023-09-07 22:57:10.000000 sawsi-9.8/sawsi/aws/sms/api.py
--rw-r--r--   0 kch        (501) staff       (20)      430 2023-09-05 01:18:09.000000 sawsi-9.8/sawsi/aws/sms/wrapper.py
-drwxr-xr-x   0 kch        (501) staff       (20)        0 2024-02-07 03:46:28.973916 sawsi-9.8/sawsi/aws/sns/
--rw-r--r--   0 kch        (501) staff       (20)        0 2023-09-11 18:51:36.000000 sawsi-9.8/sawsi/aws/sns/__init__.py
--rw-r--r--   0 kch        (501) staff       (20)      756 2023-11-14 06:28:36.000000 sawsi-9.8/sawsi/aws/sns/api.py
--rw-r--r--   0 kch        (501) staff       (20)      576 2023-11-14 06:28:26.000000 sawsi-9.8/sawsi/aws/sns/wrapper.py
-drwxr-xr-x   0 kch        (501) staff       (20)        0 2024-02-07 03:46:28.974350 sawsi-9.8/sawsi/aws/sqs/
--rw-r--r--   0 kch        (501) staff       (20)        0 2023-11-28 08:02:35.000000 sawsi-9.8/sawsi/aws/sqs/__init__.py
--rw-r--r--   0 kch        (501) staff       (20)      777 2023-11-28 08:08:52.000000 sawsi-9.8/sawsi/aws/sqs/api.py
--rw-r--r--   0 kch        (501) staff       (20)      416 2023-11-28 08:05:24.000000 sawsi-9.8/sawsi/aws/sqs/wrapper.py
-drwxr-xr-x   0 kch        (501) staff       (20)        0 2024-02-07 03:46:28.974798 sawsi-9.8/sawsi/aws/ssm/
--rw-r--r--   0 kch        (501) staff       (20)        0 2023-11-28 04:17:38.000000 sawsi-9.8/sawsi/aws/ssm/__init__.py
--rw-r--r--   0 kch        (501) staff       (20)      903 2023-11-28 04:20:46.000000 sawsi-9.8/sawsi/aws/ssm/api.py
--rw-r--r--   0 kch        (501) staff       (20)      853 2023-11-28 07:00:09.000000 sawsi-9.8/sawsi/aws/ssm/wrapper.py
-drwxr-xr-x   0 kch        (501) staff       (20)        0 2024-02-07 03:46:28.976411 sawsi-9.8/sawsi/shared/
--rw-r--r--   0 kch        (501) staff       (20)        0 2023-06-16 10:36:53.000000 sawsi-9.8/sawsi/shared/__init__.py
--rw-r--r--   0 kch        (501) staff       (20)      754 2023-10-26 12:40:29.000000 sawsi-9.8/sawsi/shared/class_util.py
--rw-r--r--   0 kch        (501) staff       (20)     1611 2023-09-07 21:14:37.000000 sawsi-9.8/sawsi/shared/dict_util.py
--rw-r--r--   0 kch        (501) staff       (20)     2066 2023-10-27 04:58:42.000000 sawsi-9.8/sawsi/shared/error_util.py
--rw-r--r--   0 kch        (501) staff       (20)     2138 2023-12-29 05:31:06.000000 sawsi-9.8/sawsi/shared/filter_exp_util.py
--rw-r--r--   0 kch        (501) staff       (20)     1168 2023-09-07 21:49:18.000000 sawsi-9.8/sawsi/shared/function_util.py
--rw-r--r--   0 kch        (501) staff       (20)     5627 2023-12-29 04:59:13.000000 sawsi-9.8/sawsi/shared/handler_util.py
--rw-r--r--   0 kch        (501) staff       (20)     2657 2023-06-09 05:42:06.000000 sawsi-9.8/sawsi/shared/hash_util.py
--rw-r--r--   0 kch        (501) staff       (20)      494 2022-06-16 07:47:32.000000 sawsi-9.8/sawsi/shared/list_util.py
--rw-r--r--   0 kch        (501) staff       (20)      672 2022-09-15 05:55:49.000000 sawsi-9.8/sawsi/shared/set_util.py
-drwxr-xr-x   0 kch        (501) staff       (20)        0 2024-02-07 03:46:28.980355 sawsi-9.8/sawsi.egg-info/
--rw-r--r--   0 kch        (501) staff       (20)      129 2024-02-07 03:46:28.000000 sawsi-9.8/sawsi.egg-info/PKG-INFO
--rw-r--r--   0 kch        (501) staff       (20)     2354 2024-02-07 03:46:28.000000 sawsi-9.8/sawsi.egg-info/SOURCES.txt
--rw-r--r--   0 kch        (501) staff       (20)        1 2024-02-07 03:46:28.000000 sawsi-9.8/sawsi.egg-info/dependency_links.txt
--rw-r--r--   0 kch        (501) staff       (20)       35 2024-02-07 03:46:28.000000 sawsi-9.8/sawsi.egg-info/entry_points.txt
--rw-r--r--   0 kch        (501) staff       (20)       30 2024-02-07 03:46:28.000000 sawsi-9.8/sawsi.egg-info/requires.txt
--rw-r--r--   0 kch        (501) staff       (20)       29 2024-02-07 03:46:28.000000 sawsi-9.8/sawsi.egg-info/top_level.txt
-drwxr-xr-x   0 kch        (501) staff       (20)        0 2024-02-07 03:46:28.977496 sawsi-9.8/sawsi_boilerplate/
--rw-r--r--   0 kch        (501) staff       (20)        0 2024-01-04 05:46:04.000000 sawsi-9.8/sawsi_boilerplate/__init__.py
--rw-r--r--   0 kch        (501) staff       (20)     1025 2024-02-07 03:31:14.000000 sawsi-9.8/sawsi_boilerplate/api.py
-drwxr-xr-x   0 kch        (501) staff       (20)        0 2024-02-07 03:46:28.977788 sawsi-9.8/sawsi_boilerplate/app/
--rw-r--r--   0 kch        (501) staff       (20)        0 2024-01-04 10:31:48.000000 sawsi-9.8/sawsi_boilerplate/app/__init__.py
--rw-r--r--   0 kch        (501) staff       (20)     2184 2024-02-07 03:44:03.000000 sawsi-9.8/sawsi_boilerplate/app/aws_handler.py
-drwxr-xr-x   0 kch        (501) staff       (20)        0 2024-02-07 03:46:28.978093 sawsi-9.8/sawsi_boilerplate/app/controller/
--rw-r--r--   0 kch        (501) staff       (20)        0 2024-01-04 10:33:52.000000 sawsi-9.8/sawsi_boilerplate/app/controller/__init__.py
--rw-r--r--   0 kch        (501) staff       (20)      747 2024-02-06 08:21:29.000000 sawsi-9.8/sawsi_boilerplate/app/controller/sample_login.py
-drwxr-xr-x   0 kch        (501) staff       (20)        0 2024-02-07 03:46:28.978554 sawsi-9.8/sawsi_boilerplate/app/dao/
--rw-r--r--   0 kch        (501) staff       (20)        0 2024-01-04 10:34:14.000000 sawsi-9.8/sawsi_boilerplate/app/dao/__init__.py
--rw-r--r--   0 kch        (501) staff       (20)      451 2024-02-06 08:21:42.000000 sawsi-9.8/sawsi_boilerplate/app/dao/sample_user_dao.py
-drwxr-xr-x   0 kch        (501) staff       (20)        0 2024-02-07 03:46:28.979174 sawsi-9.8/sawsi_boilerplate/app/doc_make/
--rw-r--r--   0 kch        (501) staff       (20)        0 2024-02-07 02:20:19.000000 sawsi-9.8/sawsi_boilerplate/app/doc_make/__init__.py
--rw-r--r--   0 kch        (501) staff       (20)     3573 2024-02-07 03:46:19.000000 sawsi-9.8/sawsi_boilerplate/app/doc_make/test_and_make_api_doc.py
-drwxr-xr-x   0 kch        (501) staff       (20)        0 2024-02-07 03:46:28.979609 sawsi-9.8/sawsi_boilerplate/app/model/
--rw-r--r--   0 kch        (501) staff       (20)        0 2024-01-04 10:33:57.000000 sawsi-9.8/sawsi_boilerplate/app/model/__init__.py
--rw-r--r--   0 kch        (501) staff       (20)      968 2024-01-04 11:52:37.000000 sawsi-9.8/sawsi_boilerplate/app/model/sample_user.py
-drwxr-xr-x   0 kch        (501) staff       (20)        0 2024-02-07 03:46:28.980069 sawsi-9.8/sawsi_boilerplate/app/view_model/
--rw-r--r--   0 kch        (501) staff       (20)        0 2024-01-04 10:34:04.000000 sawsi-9.8/sawsi_boilerplate/app/view_model/__init__.py
--rw-r--r--   0 kch        (501) staff       (20)      358 2024-02-06 08:48:27.000000 sawsi-9.8/sawsi_boilerplate/app/view_model/sample_user_vm.py
--rw-r--r--   0 kch        (501) staff       (20)      342 2024-02-07 03:21:15.000000 sawsi-9.8/sawsi_boilerplate/build_keeper.py
--rw-r--r--   0 kch        (501) staff       (20)     2345 2024-02-07 01:10:06.000000 sawsi-9.8/sawsi_boilerplate/buildspec.yml
--rw-r--r--   0 kch        (501) staff       (20)      192 2024-02-07 03:14:07.000000 sawsi-9.8/sawsi_boilerplate/config.py
--rw-r--r--   0 kch        (501) staff       (20)      922 2024-01-04 10:45:55.000000 sawsi-9.8/sawsi_boilerplate/errs.py
--rw-r--r--   0 kch        (501) staff       (20)       21 2024-02-07 03:42:19.000000 sawsi-9.8/sawsi_boilerplate/requirements.txt
--rw-r--r--   0 kch        (501) staff       (20)       38 2024-02-07 03:46:28.981051 sawsi-9.8/setup.cfg
--rw-r--r--   0 kch        (501) staff       (20)      406 2024-02-07 03:46:26.000000 sawsi-9.8/setup.py
+drwxr-xr-x   0 kch        (501) staff       (20)        0 2024-02-07 03:52:50.594029 sawsi-9.9/
+-rw-r--r--   0 kch        (501) staff       (20)     1069 2023-09-07 22:50:01.000000 sawsi-9.9/LICENSE
+-rw-r--r--   0 kch        (501) staff       (20)      129 2024-02-07 03:52:50.593715 sawsi-9.9/PKG-INFO
+-rw-r--r--   0 kch        (501) staff       (20)     6982 2024-02-07 01:10:06.000000 sawsi-9.9/README.md
+-rw-r--r--   0 kch        (501) staff       (20)     4482 2024-02-07 03:50:05.000000 sawsi-9.9/make.py
+drwxr-xr-x   0 kch        (501) staff       (20)        0 2024-02-07 03:52:50.578732 sawsi-9.9/sawsi/
+-rw-r--r--   0 kch        (501) staff       (20)        0 2023-09-07 22:56:42.000000 sawsi-9.9/sawsi/__init__.py
+drwxr-xr-x   0 kch        (501) staff       (20)        0 2024-02-07 03:52:50.580076 sawsi-9.9/sawsi/api_doc/
+-rw-r--r--   0 kch        (501) staff       (20)        0 2023-12-22 01:38:29.000000 sawsi-9.9/sawsi/api_doc/__init__.py
+-rw-r--r--   0 kch        (501) staff       (20)     8159 2024-02-07 03:51:24.000000 sawsi-9.9/sawsi/api_doc/doc_generator.py
+drwxr-xr-x   0 kch        (501) staff       (20)        0 2024-02-07 03:52:50.580402 sawsi-9.9/sawsi/aws/
+-rw-r--r--   0 kch        (501) staff       (20)        0 2023-07-06 05:55:04.000000 sawsi-9.9/sawsi/aws/__init__.py
+drwxr-xr-x   0 kch        (501) staff       (20)        0 2024-02-07 03:52:50.580730 sawsi-9.9/sawsi/aws/codecommit/
+-rw-r--r--   0 kch        (501) staff       (20)        0 2023-07-06 05:55:04.000000 sawsi-9.9/sawsi/aws/codecommit/__init__.py
+-rw-r--r--   0 kch        (501) staff       (20)      931 2023-09-09 02:33:57.000000 sawsi-9.9/sawsi/aws/codecommit/api.py
+drwxr-xr-x   0 kch        (501) staff       (20)        0 2024-02-07 03:52:50.581075 sawsi-9.9/sawsi/aws/cognito/
+-rw-r--r--   0 kch        (501) staff       (20)        0 2023-09-08 00:30:19.000000 sawsi-9.9/sawsi/aws/cognito/__init__.py
+-rw-r--r--   0 kch        (501) staff       (20)     7306 2023-09-08 04:22:27.000000 sawsi-9.9/sawsi/aws/cognito/api.py
+drwxr-xr-x   0 kch        (501) staff       (20)        0 2024-02-07 03:52:50.582099 sawsi-9.9/sawsi/aws/dynamodb/
+-rw-r--r--   0 kch        (501) staff       (20)        0 2023-07-06 05:55:04.000000 sawsi-9.9/sawsi/aws/dynamodb/__init__.py
+-rw-r--r--   0 kch        (501) staff       (20)    61057 2024-02-07 01:22:35.000000 sawsi-9.9/sawsi/aws/dynamodb/api.py
+-rw-r--r--   0 kch        (501) staff       (20)      613 2023-07-06 05:55:04.000000 sawsi-9.9/sawsi/aws/dynamodb/config.py
+-rw-r--r--   0 kch        (501) staff       (20)     4159 2023-12-29 05:24:55.000000 sawsi-9.9/sawsi/aws/dynamodb/util.py
+-rw-r--r--   0 kch        (501) staff       (20)    40370 2024-02-06 07:50:13.000000 sawsi-9.9/sawsi/aws/dynamodb/wrapper.py
+drwxr-xr-x   0 kch        (501) staff       (20)        0 2024-02-07 03:52:50.582719 sawsi-9.9/sawsi/aws/firehose/
+-rw-r--r--   0 kch        (501) staff       (20)        0 2023-10-26 00:43:42.000000 sawsi-9.9/sawsi/aws/firehose/__init__.py
+-rw-r--r--   0 kch        (501) staff       (20)     7567 2023-10-27 06:48:49.000000 sawsi-9.9/sawsi/aws/firehose/api.py
+-rw-r--r--   0 kch        (501) staff       (20)     1646 2023-10-26 01:25:24.000000 sawsi-9.9/sawsi/aws/firehose/wrapper.py
+drwxr-xr-x   0 kch        (501) staff       (20)        0 2024-02-07 03:52:50.583047 sawsi-9.9/sawsi/aws/iam/
+-rw-r--r--   0 kch        (501) staff       (20)        0 2023-10-26 01:09:48.000000 sawsi-9.9/sawsi/aws/iam/__init__.py
+-rw-r--r--   0 kch        (501) staff       (20)     1210 2023-10-26 01:58:59.000000 sawsi-9.9/sawsi/aws/iam/wrapper.py
+drwxr-xr-x   0 kch        (501) staff       (20)        0 2024-02-07 03:52:50.583616 sawsi-9.9/sawsi/aws/locking/
+-rw-r--r--   0 kch        (501) staff       (20)        0 2023-10-25 09:05:43.000000 sawsi-9.9/sawsi/aws/locking/__init__.py
+-rw-r--r--   0 kch        (501) staff       (20)     3438 2023-11-28 00:38:08.000000 sawsi-9.9/sawsi/aws/locking/api.py
+-rw-r--r--   0 kch        (501) staff       (20)    19534 2023-09-09 01:04:51.000000 sawsi-9.9/sawsi/aws/locking/wrapper.py
+drwxr-xr-x   0 kch        (501) staff       (20)        0 2024-02-07 03:52:50.584210 sawsi-9.9/sawsi/aws/s3/
+-rw-r--r--   0 kch        (501) staff       (20)        0 2023-07-06 05:55:04.000000 sawsi-9.9/sawsi/aws/s3/__init__.py
+-rw-r--r--   0 kch        (501) staff       (20)     6255 2023-12-26 05:55:13.000000 sawsi-9.9/sawsi/aws/s3/api.py
+-rw-r--r--   0 kch        (501) staff       (20)     3118 2023-10-26 02:22:17.000000 sawsi-9.9/sawsi/aws/s3/wrapper.py
+drwxr-xr-x   0 kch        (501) staff       (20)        0 2024-02-07 03:52:50.584719 sawsi-9.9/sawsi/aws/secrets_manager/
+-rw-r--r--   0 kch        (501) staff       (20)        0 2023-07-06 05:55:04.000000 sawsi-9.9/sawsi/aws/secrets_manager/__init__.py
+-rw-r--r--   0 kch        (501) staff       (20)     1468 2023-10-26 12:47:01.000000 sawsi-9.9/sawsi/aws/secrets_manager/api.py
+-rw-r--r--   0 kch        (501) staff       (20)      525 2023-09-08 04:52:48.000000 sawsi-9.9/sawsi/aws/secrets_manager/wrapper.py
+drwxr-xr-x   0 kch        (501) staff       (20)        0 2024-02-07 03:52:50.585258 sawsi-9.9/sawsi/aws/ses/
+-rw-r--r--   0 kch        (501) staff       (20)        0 2023-09-11 18:51:36.000000 sawsi-9.9/sawsi/aws/ses/__init__.py
+-rw-r--r--   0 kch        (501) staff       (20)      802 2023-11-14 06:53:29.000000 sawsi-9.9/sawsi/aws/ses/api.py
+-rw-r--r--   0 kch        (501) staff       (20)     1035 2023-11-14 06:29:02.000000 sawsi-9.9/sawsi/aws/ses/wrapper.py
+-rw-r--r--   0 kch        (501) staff       (20)      882 2023-10-26 12:43:53.000000 sawsi-9.9/sawsi/aws/shared.py
+drwxr-xr-x   0 kch        (501) staff       (20)        0 2024-02-07 03:52:50.585812 sawsi-9.9/sawsi/aws/sms/
+-rw-r--r--   0 kch        (501) staff       (20)        0 2023-09-05 01:18:09.000000 sawsi-9.9/sawsi/aws/sms/__init__.py
+-rw-r--r--   0 kch        (501) staff       (20)      714 2023-09-07 22:57:10.000000 sawsi-9.9/sawsi/aws/sms/api.py
+-rw-r--r--   0 kch        (501) staff       (20)      430 2023-09-05 01:18:09.000000 sawsi-9.9/sawsi/aws/sms/wrapper.py
+drwxr-xr-x   0 kch        (501) staff       (20)        0 2024-02-07 03:52:50.586338 sawsi-9.9/sawsi/aws/sns/
+-rw-r--r--   0 kch        (501) staff       (20)        0 2023-09-11 18:51:36.000000 sawsi-9.9/sawsi/aws/sns/__init__.py
+-rw-r--r--   0 kch        (501) staff       (20)      756 2023-11-14 06:28:36.000000 sawsi-9.9/sawsi/aws/sns/api.py
+-rw-r--r--   0 kch        (501) staff       (20)      576 2023-11-14 06:28:26.000000 sawsi-9.9/sawsi/aws/sns/wrapper.py
+drwxr-xr-x   0 kch        (501) staff       (20)        0 2024-02-07 03:52:50.586778 sawsi-9.9/sawsi/aws/sqs/
+-rw-r--r--   0 kch        (501) staff       (20)        0 2023-11-28 08:02:35.000000 sawsi-9.9/sawsi/aws/sqs/__init__.py
+-rw-r--r--   0 kch        (501) staff       (20)      777 2023-11-28 08:08:52.000000 sawsi-9.9/sawsi/aws/sqs/api.py
+-rw-r--r--   0 kch        (501) staff       (20)      416 2023-11-28 08:05:24.000000 sawsi-9.9/sawsi/aws/sqs/wrapper.py
+drwxr-xr-x   0 kch        (501) staff       (20)        0 2024-02-07 03:52:50.587318 sawsi-9.9/sawsi/aws/ssm/
+-rw-r--r--   0 kch        (501) staff       (20)        0 2023-11-28 04:17:38.000000 sawsi-9.9/sawsi/aws/ssm/__init__.py
+-rw-r--r--   0 kch        (501) staff       (20)      903 2023-11-28 04:20:46.000000 sawsi-9.9/sawsi/aws/ssm/api.py
+-rw-r--r--   0 kch        (501) staff       (20)      853 2023-11-28 07:00:09.000000 sawsi-9.9/sawsi/aws/ssm/wrapper.py
+drwxr-xr-x   0 kch        (501) staff       (20)        0 2024-02-07 03:52:50.589317 sawsi-9.9/sawsi/shared/
+-rw-r--r--   0 kch        (501) staff       (20)        0 2023-06-16 10:36:53.000000 sawsi-9.9/sawsi/shared/__init__.py
+-rw-r--r--   0 kch        (501) staff       (20)      754 2023-10-26 12:40:29.000000 sawsi-9.9/sawsi/shared/class_util.py
+-rw-r--r--   0 kch        (501) staff       (20)     1611 2023-09-07 21:14:37.000000 sawsi-9.9/sawsi/shared/dict_util.py
+-rw-r--r--   0 kch        (501) staff       (20)     2066 2023-10-27 04:58:42.000000 sawsi-9.9/sawsi/shared/error_util.py
+-rw-r--r--   0 kch        (501) staff       (20)     2138 2023-12-29 05:31:06.000000 sawsi-9.9/sawsi/shared/filter_exp_util.py
+-rw-r--r--   0 kch        (501) staff       (20)     1168 2023-09-07 21:49:18.000000 sawsi-9.9/sawsi/shared/function_util.py
+-rw-r--r--   0 kch        (501) staff       (20)     5627 2023-12-29 04:59:13.000000 sawsi-9.9/sawsi/shared/handler_util.py
+-rw-r--r--   0 kch        (501) staff       (20)     2657 2023-06-09 05:42:06.000000 sawsi-9.9/sawsi/shared/hash_util.py
+-rw-r--r--   0 kch        (501) staff       (20)      494 2022-06-16 07:47:32.000000 sawsi-9.9/sawsi/shared/list_util.py
+-rw-r--r--   0 kch        (501) staff       (20)      672 2022-09-15 05:55:49.000000 sawsi-9.9/sawsi/shared/set_util.py
+drwxr-xr-x   0 kch        (501) staff       (20)        0 2024-02-07 03:52:50.593374 sawsi-9.9/sawsi.egg-info/
+-rw-r--r--   0 kch        (501) staff       (20)      129 2024-02-07 03:52:50.000000 sawsi-9.9/sawsi.egg-info/PKG-INFO
+-rw-r--r--   0 kch        (501) staff       (20)     2354 2024-02-07 03:52:50.000000 sawsi-9.9/sawsi.egg-info/SOURCES.txt
+-rw-r--r--   0 kch        (501) staff       (20)        1 2024-02-07 03:52:50.000000 sawsi-9.9/sawsi.egg-info/dependency_links.txt
+-rw-r--r--   0 kch        (501) staff       (20)       35 2024-02-07 03:52:50.000000 sawsi-9.9/sawsi.egg-info/entry_points.txt
+-rw-r--r--   0 kch        (501) staff       (20)       30 2024-02-07 03:52:50.000000 sawsi-9.9/sawsi.egg-info/requires.txt
+-rw-r--r--   0 kch        (501) staff       (20)       29 2024-02-07 03:52:50.000000 sawsi-9.9/sawsi.egg-info/top_level.txt
+drwxr-xr-x   0 kch        (501) staff       (20)        0 2024-02-07 03:52:50.590617 sawsi-9.9/sawsi_boilerplate/
+-rw-r--r--   0 kch        (501) staff       (20)        0 2024-01-04 05:46:04.000000 sawsi-9.9/sawsi_boilerplate/__init__.py
+-rw-r--r--   0 kch        (501) staff       (20)     1025 2024-02-07 03:31:14.000000 sawsi-9.9/sawsi_boilerplate/api.py
+drwxr-xr-x   0 kch        (501) staff       (20)        0 2024-02-07 03:52:50.591129 sawsi-9.9/sawsi_boilerplate/app/
+-rw-r--r--   0 kch        (501) staff       (20)        0 2024-01-04 10:31:48.000000 sawsi-9.9/sawsi_boilerplate/app/__init__.py
+-rw-r--r--   0 kch        (501) staff       (20)     2184 2024-02-07 03:44:03.000000 sawsi-9.9/sawsi_boilerplate/app/aws_handler.py
+drwxr-xr-x   0 kch        (501) staff       (20)        0 2024-02-07 03:52:50.591587 sawsi-9.9/sawsi_boilerplate/app/controller/
+-rw-r--r--   0 kch        (501) staff       (20)        0 2024-01-04 10:33:52.000000 sawsi-9.9/sawsi_boilerplate/app/controller/__init__.py
+-rw-r--r--   0 kch        (501) staff       (20)      747 2024-02-06 08:21:29.000000 sawsi-9.9/sawsi_boilerplate/app/controller/sample_login.py
+drwxr-xr-x   0 kch        (501) staff       (20)        0 2024-02-07 03:52:50.591960 sawsi-9.9/sawsi_boilerplate/app/dao/
+-rw-r--r--   0 kch        (501) staff       (20)        0 2024-01-04 10:34:14.000000 sawsi-9.9/sawsi_boilerplate/app/dao/__init__.py
+-rw-r--r--   0 kch        (501) staff       (20)      451 2024-02-06 08:21:42.000000 sawsi-9.9/sawsi_boilerplate/app/dao/sample_user_dao.py
+drwxr-xr-x   0 kch        (501) staff       (20)        0 2024-02-07 03:52:50.592340 sawsi-9.9/sawsi_boilerplate/app/doc_make/
+-rw-r--r--   0 kch        (501) staff       (20)        0 2024-02-07 02:20:19.000000 sawsi-9.9/sawsi_boilerplate/app/doc_make/__init__.py
+-rw-r--r--   0 kch        (501) staff       (20)     3472 2024-02-07 03:52:18.000000 sawsi-9.9/sawsi_boilerplate/app/doc_make/test_and_make_api_doc.py
+drwxr-xr-x   0 kch        (501) staff       (20)        0 2024-02-07 03:52:50.592685 sawsi-9.9/sawsi_boilerplate/app/model/
+-rw-r--r--   0 kch        (501) staff       (20)        0 2024-01-04 10:33:57.000000 sawsi-9.9/sawsi_boilerplate/app/model/__init__.py
+-rw-r--r--   0 kch        (501) staff       (20)      968 2024-01-04 11:52:37.000000 sawsi-9.9/sawsi_boilerplate/app/model/sample_user.py
+drwxr-xr-x   0 kch        (501) staff       (20)        0 2024-02-07 03:52:50.593079 sawsi-9.9/sawsi_boilerplate/app/view_model/
+-rw-r--r--   0 kch        (501) staff       (20)        0 2024-01-04 10:34:04.000000 sawsi-9.9/sawsi_boilerplate/app/view_model/__init__.py
+-rw-r--r--   0 kch        (501) staff       (20)      358 2024-02-06 08:48:27.000000 sawsi-9.9/sawsi_boilerplate/app/view_model/sample_user_vm.py
+-rw-r--r--   0 kch        (501) staff       (20)      342 2024-02-07 03:21:15.000000 sawsi-9.9/sawsi_boilerplate/build_keeper.py
+-rw-r--r--   0 kch        (501) staff       (20)     2357 2024-02-07 03:49:10.000000 sawsi-9.9/sawsi_boilerplate/buildspec.yml
+-rw-r--r--   0 kch        (501) staff       (20)      192 2024-02-07 03:14:07.000000 sawsi-9.9/sawsi_boilerplate/config.py
+-rw-r--r--   0 kch        (501) staff       (20)      922 2024-01-04 10:45:55.000000 sawsi-9.9/sawsi_boilerplate/errs.py
+-rw-r--r--   0 kch        (501) staff       (20)       21 2024-02-07 03:42:19.000000 sawsi-9.9/sawsi_boilerplate/requirements.txt
+-rw-r--r--   0 kch        (501) staff       (20)       38 2024-02-07 03:52:50.594087 sawsi-9.9/setup.cfg
+-rw-r--r--   0 kch        (501) staff       (20)      406 2024-02-07 03:52:48.000000 sawsi-9.9/setup.py
```

### Comparing `sawsi-9.8/LICENSE` & `sawsi-9.9/LICENSE`

 * *Files identical despite different names*

### Comparing `sawsi-9.8/README.md` & `sawsi-9.9/README.md`

 * *Files identical despite different names*

### Comparing `sawsi-9.8/make.py` & `sawsi-9.9/make.py`

 * *Files 2% similar despite different names*

```diff
@@ -65,18 +65,21 @@
             copy_without_overwrite(source_file, project_path / rename_to)
             click.echo(f"Created: {project_path}")
 
     # {{app}} 문자열 치환
     files_contain_app_literal = ['buildspec.yml', 'build_keeper.py']
     for file in files_contain_app_literal:
         replace_app(project_path / file, app_name)
-    files_contain_project_literal = ['api.py']
+
+    # {{project}} 문자열 치환
+    files_contain_project_literal = ['buildspec.yml', 'api.py']
     for file in files_contain_project_literal:
         replace_project(project_path / file, project_name)
 
+
 def create_app_dir(app_name, project_path):
     source_dir = boilerplate_dir / 'app'
     destination_dir = project_path / app_name
 
     # 대상 디렉토리가 이미 존재하는 경우에도 복사를 수행
     try:
         shutil.copytree(source_dir, destination_dir, dirs_exist_ok=False)
```

### Comparing `sawsi-9.8/sawsi/api_doc/doc_generator.py` & `sawsi-9.9/sawsi/api_doc/doc_generator.py`

 * *Files 2% similar despite different names*

```diff
@@ -196,23 +196,24 @@
         return openapi_doc
 
     def get_api_list(self)->List[APIInfo]:
         return self.api_list
 
 
     @classmethod
-    def read_doc_html(cls, api_base_url:str= 'main_api.json'):
+    def read_doc_html(cls, api_base_url:str= 'main_api.json', title='API Docs'):
         """
         템플릿 바탕으로 html 파일을 생성해서 반환합니다.
         :return:
         """
-        html = '<!DOCTYPE html><html>  <head>    <meta charset="UTF-8">    <meta name="viewport" content="width=device-width, initial-scale=1">    <link href="https://fonts.googleapis.com/css?family=Montserrat:300,400,700|Roboto:300,400,700" rel="stylesheet">    <title>API 문서</title>    <!-- Redoc 라이브러리 추가 -->  </head>  <body>    <div id="redoc-container"></div>    <script src="https://cdn.jsdelivr.net/npm/redoc@2.0.0-rc.55/bundles/redoc.standalone.min.js"> </script>    <script src="https://cdn.jsdelivr.net/gh/wll8/redoc-try@1.4.9/dist/try.js"></script>    <script>   initTry({        openApi: `{{api_url}}`,        redocOptions: {scrollYOffset: 50},      })    </script>  </body></html>'
+        html = '<!DOCTYPE html><html>  <head>    <meta charset="UTF-8">    <meta name="viewport" content="width=device-width, initial-scale=1">    <link href="https://fonts.googleapis.com/css?family=Montserrat:300,400,700|Roboto:300,400,700" rel="stylesheet">    <title>{{title}}</title>    <!-- Redoc 라이브러리 추가 -->  </head>  <body>    <div id="redoc-container"></div>    <script src="https://cdn.jsdelivr.net/npm/redoc@2.0.0-rc.55/bundles/redoc.standalone.min.js"> </script>    <script src="https://cdn.jsdelivr.net/gh/wll8/redoc-try@1.4.9/dist/try.js"></script>    <script>   initTry({        openApi: `{{api_url}}`,        redocOptions: {scrollYOffset: 50},      })    </script>  </body></html>'
         # with open(html_path, 'r') as fp:
         #     html = fp.read()
         html = html.replace('{{api_url}}', api_base_url)
+        html = html.replace('{{title}}', title)
         return html
 
     @classmethod
     def read_doc_json(cls, json_file_name:str= 'main_api.json'):
         json_path = os.path.join(directory_path, json_file_name)
         with open(json_path, 'r') as fp:
             json_text = fp.read()
```

### Comparing `sawsi-9.8/sawsi/aws/codecommit/api.py` & `sawsi-9.9/sawsi/aws/codecommit/api.py`

 * *Files identical despite different names*

### Comparing `sawsi-9.8/sawsi/aws/cognito/api.py` & `sawsi-9.9/sawsi/aws/cognito/api.py`

 * *Files identical despite different names*

### Comparing `sawsi-9.8/sawsi/aws/dynamodb/api.py` & `sawsi-9.9/sawsi/aws/dynamodb/api.py`

 * *Files identical despite different names*

### Comparing `sawsi-9.8/sawsi/aws/dynamodb/config.py` & `sawsi-9.9/sawsi/aws/dynamodb/config.py`

 * *Files identical despite different names*

### Comparing `sawsi-9.8/sawsi/aws/dynamodb/util.py` & `sawsi-9.9/sawsi/aws/dynamodb/util.py`

 * *Files identical despite different names*

### Comparing `sawsi-9.8/sawsi/aws/dynamodb/wrapper.py` & `sawsi-9.9/sawsi/aws/dynamodb/wrapper.py`

 * *Files identical despite different names*

### Comparing `sawsi-9.8/sawsi/aws/firehose/api.py` & `sawsi-9.9/sawsi/aws/firehose/api.py`

 * *Files identical despite different names*

### Comparing `sawsi-9.8/sawsi/aws/firehose/wrapper.py` & `sawsi-9.9/sawsi/aws/firehose/wrapper.py`

 * *Files identical despite different names*

### Comparing `sawsi-9.8/sawsi/aws/iam/wrapper.py` & `sawsi-9.9/sawsi/aws/iam/wrapper.py`

 * *Files identical despite different names*

### Comparing `sawsi-9.8/sawsi/aws/locking/api.py` & `sawsi-9.9/sawsi/aws/locking/api.py`

 * *Files identical despite different names*

### Comparing `sawsi-9.8/sawsi/aws/locking/wrapper.py` & `sawsi-9.9/sawsi/aws/locking/wrapper.py`

 * *Files identical despite different names*

### Comparing `sawsi-9.8/sawsi/aws/s3/api.py` & `sawsi-9.9/sawsi/aws/s3/api.py`

 * *Files identical despite different names*

### Comparing `sawsi-9.8/sawsi/aws/s3/wrapper.py` & `sawsi-9.9/sawsi/aws/s3/wrapper.py`

 * *Files identical despite different names*

### Comparing `sawsi-9.8/sawsi/aws/secrets_manager/api.py` & `sawsi-9.9/sawsi/aws/secrets_manager/api.py`

 * *Files identical despite different names*

### Comparing `sawsi-9.8/sawsi/aws/secrets_manager/wrapper.py` & `sawsi-9.9/sawsi/aws/secrets_manager/wrapper.py`

 * *Files identical despite different names*

### Comparing `sawsi-9.8/sawsi/aws/ses/api.py` & `sawsi-9.9/sawsi/aws/ses/api.py`

 * *Files identical despite different names*

### Comparing `sawsi-9.8/sawsi/aws/ses/wrapper.py` & `sawsi-9.9/sawsi/aws/ses/wrapper.py`

 * *Files identical despite different names*

### Comparing `sawsi-9.8/sawsi/aws/shared.py` & `sawsi-9.9/sawsi/aws/shared.py`

 * *Files identical despite different names*

### Comparing `sawsi-9.8/sawsi/aws/sms/api.py` & `sawsi-9.9/sawsi/aws/sms/api.py`

 * *Files identical despite different names*

### Comparing `sawsi-9.8/sawsi/aws/sns/api.py` & `sawsi-9.9/sawsi/aws/sns/api.py`

 * *Files identical despite different names*

### Comparing `sawsi-9.8/sawsi/aws/sns/wrapper.py` & `sawsi-9.9/sawsi/aws/sns/wrapper.py`

 * *Files identical despite different names*

### Comparing `sawsi-9.8/sawsi/aws/sqs/api.py` & `sawsi-9.9/sawsi/aws/sqs/api.py`

 * *Files identical despite different names*

### Comparing `sawsi-9.8/sawsi/aws/ssm/api.py` & `sawsi-9.9/sawsi/aws/ssm/api.py`

 * *Files identical despite different names*

### Comparing `sawsi-9.8/sawsi/aws/ssm/wrapper.py` & `sawsi-9.9/sawsi/aws/ssm/wrapper.py`

 * *Files identical despite different names*

### Comparing `sawsi-9.8/sawsi/shared/class_util.py` & `sawsi-9.9/sawsi/shared/class_util.py`

 * *Files identical despite different names*

### Comparing `sawsi-9.8/sawsi/shared/dict_util.py` & `sawsi-9.9/sawsi/shared/dict_util.py`

 * *Files identical despite different names*

### Comparing `sawsi-9.8/sawsi/shared/error_util.py` & `sawsi-9.9/sawsi/shared/error_util.py`

 * *Files identical despite different names*

### Comparing `sawsi-9.8/sawsi/shared/filter_exp_util.py` & `sawsi-9.9/sawsi/shared/filter_exp_util.py`

 * *Files identical despite different names*

### Comparing `sawsi-9.8/sawsi/shared/function_util.py` & `sawsi-9.9/sawsi/shared/function_util.py`

 * *Files identical despite different names*

### Comparing `sawsi-9.8/sawsi/shared/handler_util.py` & `sawsi-9.9/sawsi/shared/handler_util.py`

 * *Files identical despite different names*

### Comparing `sawsi-9.8/sawsi/shared/hash_util.py` & `sawsi-9.9/sawsi/shared/hash_util.py`

 * *Files identical despite different names*

### Comparing `sawsi-9.8/sawsi/shared/set_util.py` & `sawsi-9.9/sawsi/shared/set_util.py`

 * *Files identical despite different names*

### Comparing `sawsi-9.8/sawsi.egg-info/SOURCES.txt` & `sawsi-9.9/sawsi.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `sawsi-9.8/sawsi_boilerplate/api.py` & `sawsi-9.9/sawsi_boilerplate/api.py`

 * *Files identical despite different names*

### Comparing `sawsi-9.8/sawsi_boilerplate/app/aws_handler.py` & `sawsi-9.9/sawsi_boilerplate/app/aws_handler.py`

 * *Files identical despite different names*

### Comparing `sawsi-9.8/sawsi_boilerplate/app/controller/sample_login.py` & `sawsi-9.9/sawsi_boilerplate/app/controller/sample_login.py`

 * *Files identical despite different names*

### Comparing `sawsi-9.8/sawsi_boilerplate/app/doc_make/test_and_make_api_doc.py` & `sawsi-9.9/sawsi_boilerplate/app/doc_make/test_and_make_api_doc.py`

 * *Files 4% similar despite different names*

```diff
@@ -33,15 +33,14 @@
 def test_and_make_api_doc():
     config.build = True
     api_name = '{{app}}_api'
 
     doc = doc_generator.DocMaker(aws_handler.handler, base_url=base_url, test_function=_test_function)
 
     doc.add_header('session_id', 'string', None, '로그인 함수로 발급되는 session_id 값', False)
-    doc.add_header('otp_code', 'string', None, '로그인시 발급되는 otp_secret 으로부터 생성한 값', False)
     doc.add_header('Connection', 'string', 'keep-alive', '고정', False)
     doc.add_header('Accept-Encoding', 'string', 'gzip, deflate, br', '고정', False)
     doc.add_header('Accept', 'string', '*/*', '고정', False)
     doc.add_header('User-Agent', 'string',  'Client', '고정', False)
     doc.add_header('Content-Type', 'string', 'application/json', '고정', False)
 
     headers = {
@@ -86,15 +85,15 @@
     doc_json = json.dumps(doc_dict)
     doc_json_enc = doc_json.encode('utf-8')
     # JSON 파일 먼저 업로드
     main_api_json_url = dev_app_api_doc_s3.upload_file_and_return_url(
         file_bytes=doc_json_enc, extension='json', content_type='application/json', forced_file_id=f'{file_name}.json'
     )
     doc_html = doc.read_doc_html(
-        main_api_json_url
+        main_api_json_url, '{{app}} API Docs'
     )
     doc_html_enc = doc_html.encode('utf-8')
     # 이후에 HTML 파일 업로드
     app_api_html_url = dev_app_api_doc_s3.upload_file_and_return_url(
         file_bytes=doc_html_enc, extension='html', content_type='text/html', forced_file_id=f'{file_name}.html',
     )
     print('api_html_url:', app_api_html_url)
```

### Comparing `sawsi-9.8/sawsi_boilerplate/app/model/sample_user.py` & `sawsi-9.9/sawsi_boilerplate/app/model/sample_user.py`

 * *Files identical despite different names*

### Comparing `sawsi-9.8/sawsi_boilerplate/buildspec.yml` & `sawsi-9.9/sawsi_boilerplate/buildspec.yml`

 * *Files 4% similar despite different names*

```diff
@@ -11,15 +11,15 @@
   variables:
     ARN_BASE: "arn:aws:lambda:us-west-1:<AWS_ACCOUNT_ID>"
     S3_BUCKET: "dev-bucket-build"
     # 아래에 배포할 Lambda 속성들을 리스트업합니다. 필요하면 list 형태로 추가하면 동일한 패키지가 함수에 배포됩니다.
     # 배포전에 함수를 생성해두어야합니다.
     LAMBDAS: |
       [
-        {"name": "dev_{{app}}", "handler": "{{app}}.aws_handler.handler"}
+        {"name": "dev_{{project}}_{{app}}", "handler": "{{app}}.aws_handler.handler"}
       ]
     # 필요하면 추가..
     RUNTIME: "python3.12"
     MEM_SIZE: "1648"
     ENV_NAME: "dev"
 
 phases:
```

### Comparing `sawsi-9.8/sawsi_boilerplate/errs.py` & `sawsi-9.9/sawsi_boilerplate/errs.py`

 * *Files identical despite different names*

