# Comparing `tmp/python-adjutant-8.0.0.tar.gz` & `tmp/python-adjutant-8.0.0.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-adjutant-8.0.0.tar", last modified: Wed Apr  3 11:08:28 2024, max compression
+gzip compressed data, was "python-adjutant-8.0.0.0rc1.tar", last modified: Fri Mar 15 14:52:52 2024, max compression
```

## Comparing `python-adjutant-8.0.0.tar` & `python-adjutant-8.0.0.0rc1.tar`

### file list

```diff
@@ -1,218 +1,218 @@
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:08:28.965181 python-adjutant-8.0.0/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      215 2024-04-03 11:08:02.000000 python-adjutant-8.0.0/.coveragerc
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      133 2024-04-03 11:08:02.000000 python-adjutant-8.0.0/.git-blame-ignore-revs
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      535 2024-04-03 11:08:02.000000 python-adjutant-8.0.0/.zuul.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1396 2024-04-03 11:08:28.000000 python-adjutant-8.0.0/AUTHORS
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    14151 2024-04-03 11:08:28.000000 python-adjutant-8.0.0/ChangeLog
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10143 2024-04-03 11:08:02.000000 python-adjutant-8.0.0/LICENSE
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2483 2024-04-03 11:08:28.965181 python-adjutant-8.0.0/PKG-INFO
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1464 2024-04-03 11:08:02.000000 python-adjutant-8.0.0/README.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:08:28.929180 python-adjutant-8.0.0/adjutant/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1177 2024-04-03 11:08:02.000000 python-adjutant-8.0.0/adjutant/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:08:28.933180 python-adjutant-8.0.0/adjutant/actions/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      741 2024-04-03 11:08:02.000000 python-adjutant-8.0.0/adjutant/actions/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:08:28.933180 python-adjutant-8.0.0/adjutant/actions/migrations/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1410 2024-04-03 11:08:02.000000 python-adjutant-8.0.0/adjutant/actions/migrations/0001_initial.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      360 2024-04-03 11:08:02.000000 python-adjutant-8.0.0/adjutant/actions/migrations/0002_action_auto_approve.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      501 2024-04-03 11:08:02.000000 python-adjutant-8.0.0/adjutant/actions/migrations/0003_auto_20190610_0205.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      555 2024-04-03 11:08:02.000000 python-adjutant-8.0.0/adjutant/actions/migrations/0004_auto_20190610_0209.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      405 2024-04-03 11:08:02.000000 python-adjutant-8.0.0/adjutant/actions/migrations/0005_alter_action_auto_approve.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:08:02.000000 python-adjutant-8.0.0/adjutant/actions/migrations/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2062 2024-04-03 11:08:02.000000 python-adjutant-8.0.0/adjutant/actions/models.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3124 2024-04-03 11:08:02.000000 python-adjutant-8.0.0/adjutant/actions/utils.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:08:28.933180 python-adjutant-8.0.0/adjutant/actions/v1/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:08:02.000000 python-adjutant-8.0.0/adjutant/actions/v1/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    18823 2024-04-03 11:08:02.000000 python-adjutant-8.0.0/adjutant/actions/v1/base.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6806 2024-04-03 11:08:02.000000 python-adjutant-8.0.0/adjutant/actions/v1/misc.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    18642 2024-04-03 11:08:02.000000 python-adjutant-8.0.0/adjutant/actions/v1/projects.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    16615 2024-04-03 11:08:02.000000 python-adjutant-8.0.0/adjutant/actions/v1/resources.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5704 2024-04-03 11:08:02.000000 python-adjutant-8.0.0/adjutant/actions/v1/serializers.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:08:28.937180 python-adjutant-8.0.0/adjutant/actions/v1/tests/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:08:02.000000 python-adjutant-8.0.0/adjutant/actions/v1/tests/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7259 2024-04-03 11:08:02.000000 python-adjutant-8.0.0/adjutant/actions/v1/tests/test_misc_actions.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    30748 2024-04-03 11:08:02.000000 python-adjutant-8.0.0/adjutant/actions/v1/tests/test_project_actions.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    28343 2024-04-03 11:08:02.000000 python-adjutant-8.0.0/adjutant/actions/v1/tests/test_resource_actions.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    38511 2024-04-03 11:08:02.000000 python-adjutant-8.0.0/adjutant/actions/v1/tests/test_user_actions.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    16713 2024-04-03 11:08:02.000000 python-adjutant-8.0.0/adjutant/actions/v1/users.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:08:28.937180 python-adjutant-8.0.0/adjutant/api/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      736 2024-04-03 11:08:02.000000 python-adjutant-8.0.0/adjutant/api/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2041 2024-04-03 11:08:02.000000 python-adjutant-8.0.0/adjutant/api/exception_handler.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:08:28.937180 python-adjutant-8.0.0/adjutant/api/migrations/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3233 2024-04-03 11:08:02.000000 python-adjutant-8.0.0/adjutant/api/migrations/0001_initial.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      361 2024-04-03 11:08:02.000000 python-adjutant-8.0.0/adjutant/api/migrations/0002_auto_20160815_2249.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      389 2024-04-03 11:08:02.000000 python-adjutant-8.0.0/adjutant/api/migrations/0003_task_approved_by.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      383 2024-04-03 11:08:02.000000 python-adjutant-8.0.0/adjutant/api/migrations/0004_auto_20160929_0317.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      507 2024-04-03 11:08:02.000000 python-adjutant-8.0.0/adjutant/api/migrations/0005_auto_20190610_0209.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      554 2024-04-03 11:08:02.000000 python-adjutant-8.0.0/adjutant/api/migrations/0006_auto_20190610_0209.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      561 2024-04-03 11:08:02.000000 python-adjutant-8.0.0/adjutant/api/migrations/0007_auto_20190610_0209.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      611 2024-04-03 11:08:02.000000 python-adjutant-8.0.0/adjutant/api/migrations/0008_auto_20190610_0209.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:08:02.000000 python-adjutant-8.0.0/adjutant/api/migrations/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2201 2024-04-03 11:08:02.000000 python-adjutant-8.0.0/adjutant/api/models.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1334 2024-04-03 11:08:02.000000 python-adjutant-8.0.0/adjutant/api/urls.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2825 2024-04-03 11:08:02.000000 python-adjutant-8.0.0/adjutant/api/utils.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:08:28.941180 python-adjutant-8.0.0/adjutant/api/v1/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:08:02.000000 python-adjutant-8.0.0/adjutant/api/v1/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1197 2024-04-03 11:08:02.000000 python-adjutant-8.0.0/adjutant/api/v1/base.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    16422 2024-04-03 11:08:02.000000 python-adjutant-8.0.0/adjutant/api/v1/openstack.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6624 2024-04-03 11:08:02.000000 python-adjutant-8.0.0/adjutant/api/v1/tasks.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:08:28.941180 python-adjutant-8.0.0/adjutant/api/v1/tests/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:08:02.000000 python-adjutant-8.0.0/adjutant/api/v1/tests/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    61455 2024-04-03 11:08:02.000000 python-adjutant-8.0.0/adjutant/api/v1/tests/test_api_admin.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    47657 2024-04-03 11:08:02.000000 python-adjutant-8.0.0/adjutant/api/v1/tests/test_api_openstack.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    64254 2024-04-03 11:08:02.000000 python-adjutant-8.0.0/adjutant/api/v1/tests/test_api_taskview.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1361 2024-04-03 11:08:02.000000 python-adjutant-8.0.0/adjutant/api/v1/urls.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2076 2024-04-03 11:08:02.000000 python-adjutant-8.0.0/adjutant/api/v1/utils.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    15168 2024-04-03 11:08:02.000000 python-adjutant-8.0.0/adjutant/api/v1/views.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1811 2024-04-03 11:08:02.000000 python-adjutant-8.0.0/adjutant/api/views.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:08:28.941180 python-adjutant-8.0.0/adjutant/commands/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:08:02.000000 python-adjutant-8.0.0/adjutant/commands/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:08:28.941180 python-adjutant-8.0.0/adjutant/commands/management/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:08:02.000000 python-adjutant-8.0.0/adjutant/commands/management/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:08:28.941180 python-adjutant-8.0.0/adjutant/commands/management/commands/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:08:02.000000 python-adjutant-8.0.0/adjutant/commands/management/commands/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      503 2024-04-03 11:08:02.000000 python-adjutant-8.0.0/adjutant/commands/management/commands/exampleconfig.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:08:28.941180 python-adjutant-8.0.0/adjutant/common/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:08:02.000000 python-adjutant-8.0.0/adjutant/common/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      904 2024-04-03 11:08:02.000000 python-adjutant-8.0.0/adjutant/common/constants.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2923 2024-04-03 11:08:02.000000 python-adjutant-8.0.0/adjutant/common/openstack_clients.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    13668 2024-04-03 11:08:02.000000 python-adjutant-8.0.0/adjutant/common/quota.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:08:28.945180 python-adjutant-8.0.0/adjutant/common/tests/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:08:02.000000 python-adjutant-8.0.0/adjutant/common/tests/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    30345 2024-04-03 11:08:02.000000 python-adjutant-8.0.0/adjutant/common/tests/fake_clients.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1201 2024-04-03 11:08:02.000000 python-adjutant-8.0.0/adjutant/common/tests/utils.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    13747 2024-04-03 11:08:02.000000 python-adjutant-8.0.0/adjutant/common/user_store.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      905 2024-04-03 11:08:02.000000 python-adjutant-8.0.0/adjutant/common/utils.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:08:28.945180 python-adjutant-8.0.0/adjutant/config/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3736 2024-04-03 11:08:02.000000 python-adjutant-8.0.0/adjutant/config/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1627 2024-04-03 11:08:02.000000 python-adjutant-8.0.0/adjutant/config/api.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3929 2024-04-03 11:08:02.000000 python-adjutant-8.0.0/adjutant/config/django.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      715 2024-04-03 11:08:02.000000 python-adjutant-8.0.0/adjutant/config/feature_sets.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4187 2024-04-03 11:08:02.000000 python-adjutant-8.0.0/adjutant/config/identity.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      840 2024-04-03 11:08:02.000000 python-adjutant-8.0.0/adjutant/config/notification.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4774 2024-04-03 11:08:02.000000 python-adjutant-8.0.0/adjutant/config/quota.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5297 2024-04-03 11:08:02.000000 python-adjutant-8.0.0/adjutant/config/workflow.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2706 2024-04-03 11:08:02.000000 python-adjutant-8.0.0/adjutant/core.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4665 2024-04-03 11:08:02.000000 python-adjutant-8.0.0/adjutant/exceptions.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6313 2024-04-03 11:08:02.000000 python-adjutant-8.0.0/adjutant/feature_set.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4010 2024-04-03 11:08:02.000000 python-adjutant-8.0.0/adjutant/middleware.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:08:28.945180 python-adjutant-8.0.0/adjutant/notifications/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      642 2024-04-03 11:08:02.000000 python-adjutant-8.0.0/adjutant/notifications/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:08:28.945180 python-adjutant-8.0.0/adjutant/notifications/migrations/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:08:02.000000 python-adjutant-8.0.0/adjutant/notifications/migrations/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:08:28.945180 python-adjutant-8.0.0/adjutant/notifications/templates/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      914 2024-04-03 11:08:02.000000 python-adjutant-8.0.0/adjutant/notifications/templates/notification.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1311 2024-04-03 11:08:02.000000 python-adjutant-8.0.0/adjutant/notifications/utils.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:08:28.949180 python-adjutant-8.0.0/adjutant/notifications/v1/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:08:02.000000 python-adjutant-8.0.0/adjutant/notifications/v1/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1964 2024-04-03 11:08:02.000000 python-adjutant-8.0.0/adjutant/notifications/v1/base.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5386 2024-04-03 11:08:02.000000 python-adjutant-8.0.0/adjutant/notifications/v1/email.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:08:28.949180 python-adjutant-8.0.0/adjutant/notifications/v1/tests/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:08:02.000000 python-adjutant-8.0.0/adjutant/notifications/v1/tests/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4401 2024-04-03 11:08:02.000000 python-adjutant-8.0.0/adjutant/notifications/v1/tests/test_notifications.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4435 2024-04-03 11:08:02.000000 python-adjutant-8.0.0/adjutant/settings.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:08:28.949180 python-adjutant-8.0.0/adjutant/startup/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       61 2024-04-03 11:08:02.000000 python-adjutant-8.0.0/adjutant/startup/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1753 2024-04-03 11:08:02.000000 python-adjutant-8.0.0/adjutant/startup/checks.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1346 2024-04-03 11:08:02.000000 python-adjutant-8.0.0/adjutant/startup/config.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      814 2024-04-03 11:08:02.000000 python-adjutant-8.0.0/adjutant/startup/loading.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:08:02.000000 python-adjutant-8.0.0/adjutant/startup/models.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:08:28.949180 python-adjutant-8.0.0/adjutant/tasks/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      630 2024-04-03 11:08:02.000000 python-adjutant-8.0.0/adjutant/tasks/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:08:28.949180 python-adjutant-8.0.0/adjutant/tasks/migrations/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2496 2024-04-03 11:08:02.000000 python-adjutant-8.0.0/adjutant/tasks/migrations/0001_initial.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2756 2024-04-03 11:08:02.000000 python-adjutant-8.0.0/adjutant/tasks/migrations/0002_auto_20190619_0613.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:08:02.000000 python-adjutant-8.0.0/adjutant/tasks/migrations/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4764 2024-04-03 11:08:02.000000 python-adjutant-8.0.0/adjutant/tasks/models.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:08:28.953181 python-adjutant-8.0.0/adjutant/tasks/templates/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      165 2024-04-03 11:08:02.000000 python-adjutant-8.0.0/adjutant/tasks/templates/completed.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      762 2024-04-03 11:08:02.000000 python-adjutant-8.0.0/adjutant/tasks/templates/create_project_and_user_completed.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      158 2024-04-03 11:08:02.000000 python-adjutant-8.0.0/adjutant/tasks/templates/create_project_and_user_initial.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      869 2024-04-03 11:08:02.000000 python-adjutant-8.0.0/adjutant/tasks/templates/create_project_and_user_token.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      257 2024-04-03 11:08:02.000000 python-adjutant-8.0.0/adjutant/tasks/templates/initial.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      325 2024-04-03 11:08:02.000000 python-adjutant-8.0.0/adjutant/tasks/templates/invite_user_to_project_completed.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1264 2024-04-03 11:08:02.000000 python-adjutant-8.0.0/adjutant/tasks/templates/invite_user_to_project_token.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      271 2024-04-03 11:08:02.000000 python-adjutant-8.0.0/adjutant/tasks/templates/reset_user_password_completed.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      458 2024-04-03 11:08:02.000000 python-adjutant-8.0.0/adjutant/tasks/templates/reset_user_password_token.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      244 2024-04-03 11:08:02.000000 python-adjutant-8.0.0/adjutant/tasks/templates/token.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      323 2024-04-03 11:08:02.000000 python-adjutant-8.0.0/adjutant/tasks/templates/update_quota_completed.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      115 2024-04-03 11:08:02.000000 python-adjutant-8.0.0/adjutant/tasks/templates/update_user_email_completed.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      258 2024-04-03 11:08:02.000000 python-adjutant-8.0.0/adjutant/tasks/templates/update_user_email_started.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      456 2024-04-03 11:08:02.000000 python-adjutant-8.0.0/adjutant/tasks/templates/update_user_email_token.txt
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:08:28.957181 python-adjutant-8.0.0/adjutant/tasks/v1/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:08:02.000000 python-adjutant-8.0.0/adjutant/tasks/v1/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    18124 2024-04-03 11:08:02.000000 python-adjutant-8.0.0/adjutant/tasks/v1/base.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3184 2024-04-03 11:08:02.000000 python-adjutant-8.0.0/adjutant/tasks/v1/manager.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1335 2024-04-03 11:08:02.000000 python-adjutant-8.0.0/adjutant/tasks/v1/projects.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1000 2024-04-03 11:08:02.000000 python-adjutant-8.0.0/adjutant/tasks/v1/resources.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2836 2024-04-03 11:08:02.000000 python-adjutant-8.0.0/adjutant/tasks/v1/users.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4544 2024-04-03 11:08:02.000000 python-adjutant-8.0.0/adjutant/tasks/v1/utils.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      718 2024-04-03 11:08:02.000000 python-adjutant-8.0.0/adjutant/urls.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      737 2024-04-03 11:08:02.000000 python-adjutant-8.0.0/adjutant/version.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1753 2024-04-03 11:08:02.000000 python-adjutant-8.0.0/adjutant/wsgi.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:08:28.925179 python-adjutant-8.0.0/api-ref/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:08:28.925179 python-adjutant-8.0.0/api-ref/_static/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:08:28.957181 python-adjutant-8.0.0/api-ref/_static/fonts/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    45404 2024-04-03 11:08:02.000000 python-adjutant-8.0.0/api-ref/_static/fonts/glyphicons-halflings-regular.ttf
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    23424 2024-04-03 11:08:02.000000 python-adjutant-8.0.0/api-ref/_static/fonts/glyphicons-halflings-regular.woff
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:08:28.957181 python-adjutant-8.0.0/api-ref/source/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    11082 2024-04-03 11:08:02.000000 python-adjutant-8.0.0/api-ref/source/admin-api.inc
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9373 2024-04-03 11:08:02.000000 python-adjutant-8.0.0/api-ref/source/conf.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10685 2024-04-03 11:08:02.000000 python-adjutant-8.0.0/api-ref/source/delegate-apis.inc
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      903 2024-04-03 11:08:02.000000 python-adjutant-8.0.0/api-ref/source/http-status.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      354 2024-04-03 11:08:02.000000 python-adjutant-8.0.0/api-ref/source/index.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3852 2024-04-03 11:08:02.000000 python-adjutant-8.0.0/api-ref/source/parameters.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2067 2024-04-03 11:08:02.000000 python-adjutant-8.0.0/api-ref/source/v1-api-reference.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      483 2024-04-03 11:08:02.000000 python-adjutant-8.0.0/bindep.txt
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:08:28.957181 python-adjutant-8.0.0/doc/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      613 2024-04-03 11:08:02.000000 python-adjutant-8.0.0/doc/Makefile
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      123 2024-04-03 11:08:02.000000 python-adjutant-8.0.0/doc/requirements.txt
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:08:28.961181 python-adjutant-8.0.0/doc/source/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4156 2024-04-03 11:08:02.000000 python-adjutant-8.0.0/doc/source/conf.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3366 2024-04-03 11:08:02.000000 python-adjutant-8.0.0/doc/source/configuration.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2297 2024-04-03 11:08:02.000000 python-adjutant-8.0.0/doc/source/contributing.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5858 2024-04-03 11:08:02.000000 python-adjutant-8.0.0/doc/source/development.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8432 2024-04-03 11:08:02.000000 python-adjutant-8.0.0/doc/source/devstack-guide.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8761 2024-04-03 11:08:02.000000 python-adjutant-8.0.0/doc/source/feature-sets.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3614 2024-04-03 11:08:02.000000 python-adjutant-8.0.0/doc/source/features.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5139 2024-04-03 11:08:02.000000 python-adjutant-8.0.0/doc/source/guide-lines.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4890 2024-04-03 11:08:02.000000 python-adjutant-8.0.0/doc/source/history.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2795 2024-04-03 11:08:02.000000 python-adjutant-8.0.0/doc/source/index.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1451 2024-04-03 11:08:02.000000 python-adjutant-8.0.0/doc/source/quota.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4073 2024-04-03 11:08:02.000000 python-adjutant-8.0.0/doc/source/release-notes.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:08:28.961181 python-adjutant-8.0.0/etc/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    24085 2024-04-03 11:08:02.000000 python-adjutant-8.0.0/etc/adjutant.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1151 2024-04-03 11:08:02.000000 python-adjutant-8.0.0/package_readme.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:08:28.961181 python-adjutant-8.0.0/python_adjutant.egg-info/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2483 2024-04-03 11:08:28.000000 python-adjutant-8.0.0/python_adjutant.egg-info/PKG-INFO
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6136 2024-04-03 11:08:28.000000 python-adjutant-8.0.0/python_adjutant.egg-info/SOURCES.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2024-04-03 11:08:28.000000 python-adjutant-8.0.0/python_adjutant.egg-info/dependency_links.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      121 2024-04-03 11:08:28.000000 python-adjutant-8.0.0/python_adjutant.egg-info/entry_points.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2024-04-03 11:08:28.000000 python-adjutant-8.0.0/python_adjutant.egg-info/not-zip-safe
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       46 2024-04-03 11:08:28.000000 python-adjutant-8.0.0/python_adjutant.egg-info/pbr.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      374 2024-04-03 11:08:28.000000 python-adjutant-8.0.0/python_adjutant.egg-info/requires.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        9 2024-04-03 11:08:28.000000 python-adjutant-8.0.0/python_adjutant.egg-info/top_level.txt
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:08:28.925179 python-adjutant-8.0.0/releasenotes/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:08:28.961181 python-adjutant-8.0.0/releasenotes/notes/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      124 2024-04-03 11:08:02.000000 python-adjutant-8.0.0/releasenotes/notes/add-trove-quota-helper-9c5c96a941ac740c.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      646 2024-04-03 11:08:02.000000 python-adjutant-8.0.0/releasenotes/notes/authed_token-6d29688676e7ee32.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      532 2024-04-03 11:08:02.000000 python-adjutant-8.0.0/releasenotes/notes/django-2-2-465a8bb124f1f7fe.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      705 2024-04-03 11:08:02.000000 python-adjutant-8.0.0/releasenotes/notes/feature-sets-f363d132c8c377cf.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      194 2024-04-03 11:08:02.000000 python-adjutant-8.0.0/releasenotes/notes/remove_mysqlclient-74299a42f0d0483e.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      545 2024-04-03 11:08:02.000000 python-adjutant-8.0.0/releasenotes/notes/story-2004488-5468c184cc3a4691.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1495 2024-04-03 11:08:02.000000 python-adjutant-8.0.0/releasenotes/notes/story-2004489-857f37e4f6a0fe5c.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      187 2024-04-03 11:08:02.000000 python-adjutant-8.0.0/releasenotes/notes/toml-d8fba261f61313bf.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:08:28.965181 python-adjutant-8.0.0/releasenotes/source/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8860 2024-04-03 11:08:02.000000 python-adjutant-8.0.0/releasenotes/source/conf.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      752 2024-04-03 11:08:02.000000 python-adjutant-8.0.0/releasenotes/source/index.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      108 2024-04-03 11:08:02.000000 python-adjutant-8.0.0/releasenotes/source/unreleased.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      130 2024-04-03 11:08:02.000000 python-adjutant-8.0.0/releasenotes/source/ussuri.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      138 2024-04-03 11:08:02.000000 python-adjutant-8.0.0/releasenotes/source/victoria.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      134 2024-04-03 11:08:02.000000 python-adjutant-8.0.0/releasenotes/source/wallaby.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      122 2024-04-03 11:08:02.000000 python-adjutant-8.0.0/releasenotes/source/xena.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      122 2024-04-03 11:08:02.000000 python-adjutant-8.0.0/releasenotes/source/yoga.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      118 2024-04-03 11:08:02.000000 python-adjutant-8.0.0/releasenotes/source/zed.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      375 2024-04-03 11:08:02.000000 python-adjutant-8.0.0/requirements.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1169 2024-04-03 11:08:28.965181 python-adjutant-8.0.0/setup.cfg
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      693 2024-04-03 11:08:02.000000 python-adjutant-8.0.0/setup.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      409 2024-04-03 11:08:02.000000 python-adjutant-8.0.0/test-requirements.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2122 2024-04-03 11:08:02.000000 python-adjutant-8.0.0/tox.ini
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-15 14:52:52.694368 python-adjutant-8.0.0.0rc1/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      215 2024-03-15 14:52:19.000000 python-adjutant-8.0.0.0rc1/.coveragerc
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      133 2024-03-15 14:52:19.000000 python-adjutant-8.0.0.0rc1/.git-blame-ignore-revs
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      535 2024-03-15 14:52:19.000000 python-adjutant-8.0.0.0rc1/.zuul.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1396 2024-03-15 14:52:52.000000 python-adjutant-8.0.0.0rc1/AUTHORS
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    14161 2024-03-15 14:52:52.000000 python-adjutant-8.0.0.0rc1/ChangeLog
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10143 2024-03-15 14:52:19.000000 python-adjutant-8.0.0.0rc1/LICENSE
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2488 2024-03-15 14:52:52.694368 python-adjutant-8.0.0.0rc1/PKG-INFO
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1464 2024-03-15 14:52:19.000000 python-adjutant-8.0.0.0rc1/README.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-15 14:52:52.650363 python-adjutant-8.0.0.0rc1/adjutant/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1177 2024-03-15 14:52:19.000000 python-adjutant-8.0.0.0rc1/adjutant/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-15 14:52:52.650363 python-adjutant-8.0.0.0rc1/adjutant/actions/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      741 2024-03-15 14:52:19.000000 python-adjutant-8.0.0.0rc1/adjutant/actions/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-15 14:52:52.650363 python-adjutant-8.0.0.0rc1/adjutant/actions/migrations/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1410 2024-03-15 14:52:19.000000 python-adjutant-8.0.0.0rc1/adjutant/actions/migrations/0001_initial.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      360 2024-03-15 14:52:19.000000 python-adjutant-8.0.0.0rc1/adjutant/actions/migrations/0002_action_auto_approve.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      501 2024-03-15 14:52:19.000000 python-adjutant-8.0.0.0rc1/adjutant/actions/migrations/0003_auto_20190610_0205.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      555 2024-03-15 14:52:19.000000 python-adjutant-8.0.0.0rc1/adjutant/actions/migrations/0004_auto_20190610_0209.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      405 2024-03-15 14:52:19.000000 python-adjutant-8.0.0.0rc1/adjutant/actions/migrations/0005_alter_action_auto_approve.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-03-15 14:52:19.000000 python-adjutant-8.0.0.0rc1/adjutant/actions/migrations/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2062 2024-03-15 14:52:19.000000 python-adjutant-8.0.0.0rc1/adjutant/actions/models.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3124 2024-03-15 14:52:19.000000 python-adjutant-8.0.0.0rc1/adjutant/actions/utils.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-15 14:52:52.654363 python-adjutant-8.0.0.0rc1/adjutant/actions/v1/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-03-15 14:52:19.000000 python-adjutant-8.0.0.0rc1/adjutant/actions/v1/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    18823 2024-03-15 14:52:19.000000 python-adjutant-8.0.0.0rc1/adjutant/actions/v1/base.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6806 2024-03-15 14:52:19.000000 python-adjutant-8.0.0.0rc1/adjutant/actions/v1/misc.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    18642 2024-03-15 14:52:19.000000 python-adjutant-8.0.0.0rc1/adjutant/actions/v1/projects.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    16615 2024-03-15 14:52:19.000000 python-adjutant-8.0.0.0rc1/adjutant/actions/v1/resources.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5704 2024-03-15 14:52:19.000000 python-adjutant-8.0.0.0rc1/adjutant/actions/v1/serializers.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-15 14:52:52.654363 python-adjutant-8.0.0.0rc1/adjutant/actions/v1/tests/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-03-15 14:52:19.000000 python-adjutant-8.0.0.0rc1/adjutant/actions/v1/tests/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7259 2024-03-15 14:52:19.000000 python-adjutant-8.0.0.0rc1/adjutant/actions/v1/tests/test_misc_actions.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    30748 2024-03-15 14:52:19.000000 python-adjutant-8.0.0.0rc1/adjutant/actions/v1/tests/test_project_actions.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    28343 2024-03-15 14:52:19.000000 python-adjutant-8.0.0.0rc1/adjutant/actions/v1/tests/test_resource_actions.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    38511 2024-03-15 14:52:19.000000 python-adjutant-8.0.0.0rc1/adjutant/actions/v1/tests/test_user_actions.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    16713 2024-03-15 14:52:19.000000 python-adjutant-8.0.0.0rc1/adjutant/actions/v1/users.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-15 14:52:52.658363 python-adjutant-8.0.0.0rc1/adjutant/api/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      736 2024-03-15 14:52:19.000000 python-adjutant-8.0.0.0rc1/adjutant/api/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2041 2024-03-15 14:52:19.000000 python-adjutant-8.0.0.0rc1/adjutant/api/exception_handler.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-15 14:52:52.658363 python-adjutant-8.0.0.0rc1/adjutant/api/migrations/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3233 2024-03-15 14:52:19.000000 python-adjutant-8.0.0.0rc1/adjutant/api/migrations/0001_initial.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      361 2024-03-15 14:52:19.000000 python-adjutant-8.0.0.0rc1/adjutant/api/migrations/0002_auto_20160815_2249.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      389 2024-03-15 14:52:19.000000 python-adjutant-8.0.0.0rc1/adjutant/api/migrations/0003_task_approved_by.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      383 2024-03-15 14:52:19.000000 python-adjutant-8.0.0.0rc1/adjutant/api/migrations/0004_auto_20160929_0317.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      507 2024-03-15 14:52:19.000000 python-adjutant-8.0.0.0rc1/adjutant/api/migrations/0005_auto_20190610_0209.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      554 2024-03-15 14:52:19.000000 python-adjutant-8.0.0.0rc1/adjutant/api/migrations/0006_auto_20190610_0209.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      561 2024-03-15 14:52:19.000000 python-adjutant-8.0.0.0rc1/adjutant/api/migrations/0007_auto_20190610_0209.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      611 2024-03-15 14:52:19.000000 python-adjutant-8.0.0.0rc1/adjutant/api/migrations/0008_auto_20190610_0209.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-03-15 14:52:19.000000 python-adjutant-8.0.0.0rc1/adjutant/api/migrations/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2201 2024-03-15 14:52:19.000000 python-adjutant-8.0.0.0rc1/adjutant/api/models.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1334 2024-03-15 14:52:19.000000 python-adjutant-8.0.0.0rc1/adjutant/api/urls.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2825 2024-03-15 14:52:19.000000 python-adjutant-8.0.0.0rc1/adjutant/api/utils.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-15 14:52:52.662364 python-adjutant-8.0.0.0rc1/adjutant/api/v1/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-03-15 14:52:19.000000 python-adjutant-8.0.0.0rc1/adjutant/api/v1/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1197 2024-03-15 14:52:19.000000 python-adjutant-8.0.0.0rc1/adjutant/api/v1/base.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    16422 2024-03-15 14:52:19.000000 python-adjutant-8.0.0.0rc1/adjutant/api/v1/openstack.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6624 2024-03-15 14:52:19.000000 python-adjutant-8.0.0.0rc1/adjutant/api/v1/tasks.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-15 14:52:52.662364 python-adjutant-8.0.0.0rc1/adjutant/api/v1/tests/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-03-15 14:52:19.000000 python-adjutant-8.0.0.0rc1/adjutant/api/v1/tests/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    61455 2024-03-15 14:52:19.000000 python-adjutant-8.0.0.0rc1/adjutant/api/v1/tests/test_api_admin.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    47657 2024-03-15 14:52:19.000000 python-adjutant-8.0.0.0rc1/adjutant/api/v1/tests/test_api_openstack.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    64254 2024-03-15 14:52:19.000000 python-adjutant-8.0.0.0rc1/adjutant/api/v1/tests/test_api_taskview.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1361 2024-03-15 14:52:19.000000 python-adjutant-8.0.0.0rc1/adjutant/api/v1/urls.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2076 2024-03-15 14:52:19.000000 python-adjutant-8.0.0.0rc1/adjutant/api/v1/utils.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    15168 2024-03-15 14:52:19.000000 python-adjutant-8.0.0.0rc1/adjutant/api/v1/views.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1811 2024-03-15 14:52:19.000000 python-adjutant-8.0.0.0rc1/adjutant/api/views.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-15 14:52:52.662364 python-adjutant-8.0.0.0rc1/adjutant/commands/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-03-15 14:52:19.000000 python-adjutant-8.0.0.0rc1/adjutant/commands/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-15 14:52:52.662364 python-adjutant-8.0.0.0rc1/adjutant/commands/management/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-03-15 14:52:19.000000 python-adjutant-8.0.0.0rc1/adjutant/commands/management/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-15 14:52:52.662364 python-adjutant-8.0.0.0rc1/adjutant/commands/management/commands/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-03-15 14:52:19.000000 python-adjutant-8.0.0.0rc1/adjutant/commands/management/commands/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      503 2024-03-15 14:52:19.000000 python-adjutant-8.0.0.0rc1/adjutant/commands/management/commands/exampleconfig.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-15 14:52:52.666364 python-adjutant-8.0.0.0rc1/adjutant/common/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-03-15 14:52:19.000000 python-adjutant-8.0.0.0rc1/adjutant/common/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      904 2024-03-15 14:52:19.000000 python-adjutant-8.0.0.0rc1/adjutant/common/constants.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2923 2024-03-15 14:52:19.000000 python-adjutant-8.0.0.0rc1/adjutant/common/openstack_clients.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    13668 2024-03-15 14:52:19.000000 python-adjutant-8.0.0.0rc1/adjutant/common/quota.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-15 14:52:52.666364 python-adjutant-8.0.0.0rc1/adjutant/common/tests/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-03-15 14:52:19.000000 python-adjutant-8.0.0.0rc1/adjutant/common/tests/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    30345 2024-03-15 14:52:19.000000 python-adjutant-8.0.0.0rc1/adjutant/common/tests/fake_clients.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1201 2024-03-15 14:52:19.000000 python-adjutant-8.0.0.0rc1/adjutant/common/tests/utils.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    13747 2024-03-15 14:52:19.000000 python-adjutant-8.0.0.0rc1/adjutant/common/user_store.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      905 2024-03-15 14:52:19.000000 python-adjutant-8.0.0.0rc1/adjutant/common/utils.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-15 14:52:52.670365 python-adjutant-8.0.0.0rc1/adjutant/config/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3736 2024-03-15 14:52:19.000000 python-adjutant-8.0.0.0rc1/adjutant/config/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1627 2024-03-15 14:52:19.000000 python-adjutant-8.0.0.0rc1/adjutant/config/api.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3929 2024-03-15 14:52:19.000000 python-adjutant-8.0.0.0rc1/adjutant/config/django.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      715 2024-03-15 14:52:19.000000 python-adjutant-8.0.0.0rc1/adjutant/config/feature_sets.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4187 2024-03-15 14:52:19.000000 python-adjutant-8.0.0.0rc1/adjutant/config/identity.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      840 2024-03-15 14:52:19.000000 python-adjutant-8.0.0.0rc1/adjutant/config/notification.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4774 2024-03-15 14:52:19.000000 python-adjutant-8.0.0.0rc1/adjutant/config/quota.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5297 2024-03-15 14:52:19.000000 python-adjutant-8.0.0.0rc1/adjutant/config/workflow.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2706 2024-03-15 14:52:19.000000 python-adjutant-8.0.0.0rc1/adjutant/core.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4665 2024-03-15 14:52:19.000000 python-adjutant-8.0.0.0rc1/adjutant/exceptions.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6313 2024-03-15 14:52:19.000000 python-adjutant-8.0.0.0rc1/adjutant/feature_set.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4010 2024-03-15 14:52:19.000000 python-adjutant-8.0.0.0rc1/adjutant/middleware.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-15 14:52:52.670365 python-adjutant-8.0.0.0rc1/adjutant/notifications/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      642 2024-03-15 14:52:19.000000 python-adjutant-8.0.0.0rc1/adjutant/notifications/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-15 14:52:52.670365 python-adjutant-8.0.0.0rc1/adjutant/notifications/migrations/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-03-15 14:52:19.000000 python-adjutant-8.0.0.0rc1/adjutant/notifications/migrations/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-15 14:52:52.670365 python-adjutant-8.0.0.0rc1/adjutant/notifications/templates/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      914 2024-03-15 14:52:19.000000 python-adjutant-8.0.0.0rc1/adjutant/notifications/templates/notification.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1311 2024-03-15 14:52:19.000000 python-adjutant-8.0.0.0rc1/adjutant/notifications/utils.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-15 14:52:52.670365 python-adjutant-8.0.0.0rc1/adjutant/notifications/v1/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-03-15 14:52:19.000000 python-adjutant-8.0.0.0rc1/adjutant/notifications/v1/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1964 2024-03-15 14:52:19.000000 python-adjutant-8.0.0.0rc1/adjutant/notifications/v1/base.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5386 2024-03-15 14:52:19.000000 python-adjutant-8.0.0.0rc1/adjutant/notifications/v1/email.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-15 14:52:52.670365 python-adjutant-8.0.0.0rc1/adjutant/notifications/v1/tests/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-03-15 14:52:19.000000 python-adjutant-8.0.0.0rc1/adjutant/notifications/v1/tests/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4401 2024-03-15 14:52:19.000000 python-adjutant-8.0.0.0rc1/adjutant/notifications/v1/tests/test_notifications.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4435 2024-03-15 14:52:19.000000 python-adjutant-8.0.0.0rc1/adjutant/settings.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-15 14:52:52.674365 python-adjutant-8.0.0.0rc1/adjutant/startup/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       61 2024-03-15 14:52:19.000000 python-adjutant-8.0.0.0rc1/adjutant/startup/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1753 2024-03-15 14:52:19.000000 python-adjutant-8.0.0.0rc1/adjutant/startup/checks.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1346 2024-03-15 14:52:19.000000 python-adjutant-8.0.0.0rc1/adjutant/startup/config.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      814 2024-03-15 14:52:19.000000 python-adjutant-8.0.0.0rc1/adjutant/startup/loading.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-03-15 14:52:19.000000 python-adjutant-8.0.0.0rc1/adjutant/startup/models.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-15 14:52:52.674365 python-adjutant-8.0.0.0rc1/adjutant/tasks/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      630 2024-03-15 14:52:19.000000 python-adjutant-8.0.0.0rc1/adjutant/tasks/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-15 14:52:52.674365 python-adjutant-8.0.0.0rc1/adjutant/tasks/migrations/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2496 2024-03-15 14:52:19.000000 python-adjutant-8.0.0.0rc1/adjutant/tasks/migrations/0001_initial.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2756 2024-03-15 14:52:19.000000 python-adjutant-8.0.0.0rc1/adjutant/tasks/migrations/0002_auto_20190619_0613.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-03-15 14:52:19.000000 python-adjutant-8.0.0.0rc1/adjutant/tasks/migrations/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4764 2024-03-15 14:52:19.000000 python-adjutant-8.0.0.0rc1/adjutant/tasks/models.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-15 14:52:52.678366 python-adjutant-8.0.0.0rc1/adjutant/tasks/templates/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      165 2024-03-15 14:52:19.000000 python-adjutant-8.0.0.0rc1/adjutant/tasks/templates/completed.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      762 2024-03-15 14:52:19.000000 python-adjutant-8.0.0.0rc1/adjutant/tasks/templates/create_project_and_user_completed.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      158 2024-03-15 14:52:19.000000 python-adjutant-8.0.0.0rc1/adjutant/tasks/templates/create_project_and_user_initial.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      869 2024-03-15 14:52:19.000000 python-adjutant-8.0.0.0rc1/adjutant/tasks/templates/create_project_and_user_token.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      257 2024-03-15 14:52:19.000000 python-adjutant-8.0.0.0rc1/adjutant/tasks/templates/initial.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      325 2024-03-15 14:52:19.000000 python-adjutant-8.0.0.0rc1/adjutant/tasks/templates/invite_user_to_project_completed.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1264 2024-03-15 14:52:19.000000 python-adjutant-8.0.0.0rc1/adjutant/tasks/templates/invite_user_to_project_token.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      271 2024-03-15 14:52:19.000000 python-adjutant-8.0.0.0rc1/adjutant/tasks/templates/reset_user_password_completed.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      458 2024-03-15 14:52:19.000000 python-adjutant-8.0.0.0rc1/adjutant/tasks/templates/reset_user_password_token.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      244 2024-03-15 14:52:19.000000 python-adjutant-8.0.0.0rc1/adjutant/tasks/templates/token.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      323 2024-03-15 14:52:19.000000 python-adjutant-8.0.0.0rc1/adjutant/tasks/templates/update_quota_completed.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      115 2024-03-15 14:52:19.000000 python-adjutant-8.0.0.0rc1/adjutant/tasks/templates/update_user_email_completed.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      258 2024-03-15 14:52:19.000000 python-adjutant-8.0.0.0rc1/adjutant/tasks/templates/update_user_email_started.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      456 2024-03-15 14:52:19.000000 python-adjutant-8.0.0.0rc1/adjutant/tasks/templates/update_user_email_token.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-15 14:52:52.678366 python-adjutant-8.0.0.0rc1/adjutant/tasks/v1/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-03-15 14:52:19.000000 python-adjutant-8.0.0.0rc1/adjutant/tasks/v1/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    18124 2024-03-15 14:52:19.000000 python-adjutant-8.0.0.0rc1/adjutant/tasks/v1/base.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3184 2024-03-15 14:52:19.000000 python-adjutant-8.0.0.0rc1/adjutant/tasks/v1/manager.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1335 2024-03-15 14:52:19.000000 python-adjutant-8.0.0.0rc1/adjutant/tasks/v1/projects.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1000 2024-03-15 14:52:19.000000 python-adjutant-8.0.0.0rc1/adjutant/tasks/v1/resources.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2836 2024-03-15 14:52:19.000000 python-adjutant-8.0.0.0rc1/adjutant/tasks/v1/users.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4544 2024-03-15 14:52:19.000000 python-adjutant-8.0.0.0rc1/adjutant/tasks/v1/utils.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      718 2024-03-15 14:52:19.000000 python-adjutant-8.0.0.0rc1/adjutant/urls.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      737 2024-03-15 14:52:19.000000 python-adjutant-8.0.0.0rc1/adjutant/version.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1753 2024-03-15 14:52:19.000000 python-adjutant-8.0.0.0rc1/adjutant/wsgi.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-15 14:52:52.642361 python-adjutant-8.0.0.0rc1/api-ref/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-15 14:52:52.642361 python-adjutant-8.0.0.0rc1/api-ref/_static/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-15 14:52:52.678366 python-adjutant-8.0.0.0rc1/api-ref/_static/fonts/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    45404 2024-03-15 14:52:19.000000 python-adjutant-8.0.0.0rc1/api-ref/_static/fonts/glyphicons-halflings-regular.ttf
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    23424 2024-03-15 14:52:19.000000 python-adjutant-8.0.0.0rc1/api-ref/_static/fonts/glyphicons-halflings-regular.woff
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-15 14:52:52.682366 python-adjutant-8.0.0.0rc1/api-ref/source/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    11082 2024-03-15 14:52:19.000000 python-adjutant-8.0.0.0rc1/api-ref/source/admin-api.inc
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9373 2024-03-15 14:52:19.000000 python-adjutant-8.0.0.0rc1/api-ref/source/conf.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10685 2024-03-15 14:52:19.000000 python-adjutant-8.0.0.0rc1/api-ref/source/delegate-apis.inc
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      903 2024-03-15 14:52:19.000000 python-adjutant-8.0.0.0rc1/api-ref/source/http-status.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      354 2024-03-15 14:52:19.000000 python-adjutant-8.0.0.0rc1/api-ref/source/index.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3852 2024-03-15 14:52:19.000000 python-adjutant-8.0.0.0rc1/api-ref/source/parameters.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2067 2024-03-15 14:52:19.000000 python-adjutant-8.0.0.0rc1/api-ref/source/v1-api-reference.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      483 2024-03-15 14:52:19.000000 python-adjutant-8.0.0.0rc1/bindep.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-15 14:52:52.682366 python-adjutant-8.0.0.0rc1/doc/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      613 2024-03-15 14:52:19.000000 python-adjutant-8.0.0.0rc1/doc/Makefile
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      123 2024-03-15 14:52:19.000000 python-adjutant-8.0.0.0rc1/doc/requirements.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-15 14:52:52.686367 python-adjutant-8.0.0.0rc1/doc/source/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4156 2024-03-15 14:52:19.000000 python-adjutant-8.0.0.0rc1/doc/source/conf.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3366 2024-03-15 14:52:19.000000 python-adjutant-8.0.0.0rc1/doc/source/configuration.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2297 2024-03-15 14:52:19.000000 python-adjutant-8.0.0.0rc1/doc/source/contributing.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5858 2024-03-15 14:52:19.000000 python-adjutant-8.0.0.0rc1/doc/source/development.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8432 2024-03-15 14:52:19.000000 python-adjutant-8.0.0.0rc1/doc/source/devstack-guide.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8761 2024-03-15 14:52:19.000000 python-adjutant-8.0.0.0rc1/doc/source/feature-sets.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3614 2024-03-15 14:52:19.000000 python-adjutant-8.0.0.0rc1/doc/source/features.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5139 2024-03-15 14:52:19.000000 python-adjutant-8.0.0.0rc1/doc/source/guide-lines.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4890 2024-03-15 14:52:19.000000 python-adjutant-8.0.0.0rc1/doc/source/history.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2795 2024-03-15 14:52:19.000000 python-adjutant-8.0.0.0rc1/doc/source/index.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1451 2024-03-15 14:52:19.000000 python-adjutant-8.0.0.0rc1/doc/source/quota.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4073 2024-03-15 14:52:19.000000 python-adjutant-8.0.0.0rc1/doc/source/release-notes.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-15 14:52:52.686367 python-adjutant-8.0.0.0rc1/etc/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    24085 2024-03-15 14:52:19.000000 python-adjutant-8.0.0.0rc1/etc/adjutant.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1151 2024-03-15 14:52:19.000000 python-adjutant-8.0.0.0rc1/package_readme.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-15 14:52:52.686367 python-adjutant-8.0.0.0rc1/python_adjutant.egg-info/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2488 2024-03-15 14:52:52.000000 python-adjutant-8.0.0.0rc1/python_adjutant.egg-info/PKG-INFO
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6136 2024-03-15 14:52:52.000000 python-adjutant-8.0.0.0rc1/python_adjutant.egg-info/SOURCES.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2024-03-15 14:52:52.000000 python-adjutant-8.0.0.0rc1/python_adjutant.egg-info/dependency_links.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      121 2024-03-15 14:52:52.000000 python-adjutant-8.0.0.0rc1/python_adjutant.egg-info/entry_points.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2024-03-15 14:52:52.000000 python-adjutant-8.0.0.0rc1/python_adjutant.egg-info/not-zip-safe
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       46 2024-03-15 14:52:52.000000 python-adjutant-8.0.0.0rc1/python_adjutant.egg-info/pbr.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      374 2024-03-15 14:52:52.000000 python-adjutant-8.0.0.0rc1/python_adjutant.egg-info/requires.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        9 2024-03-15 14:52:52.000000 python-adjutant-8.0.0.0rc1/python_adjutant.egg-info/top_level.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-15 14:52:52.642361 python-adjutant-8.0.0.0rc1/releasenotes/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-15 14:52:52.690367 python-adjutant-8.0.0.0rc1/releasenotes/notes/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      124 2024-03-15 14:52:19.000000 python-adjutant-8.0.0.0rc1/releasenotes/notes/add-trove-quota-helper-9c5c96a941ac740c.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      646 2024-03-15 14:52:19.000000 python-adjutant-8.0.0.0rc1/releasenotes/notes/authed_token-6d29688676e7ee32.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      532 2024-03-15 14:52:19.000000 python-adjutant-8.0.0.0rc1/releasenotes/notes/django-2-2-465a8bb124f1f7fe.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      705 2024-03-15 14:52:19.000000 python-adjutant-8.0.0.0rc1/releasenotes/notes/feature-sets-f363d132c8c377cf.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      194 2024-03-15 14:52:19.000000 python-adjutant-8.0.0.0rc1/releasenotes/notes/remove_mysqlclient-74299a42f0d0483e.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      545 2024-03-15 14:52:19.000000 python-adjutant-8.0.0.0rc1/releasenotes/notes/story-2004488-5468c184cc3a4691.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1495 2024-03-15 14:52:19.000000 python-adjutant-8.0.0.0rc1/releasenotes/notes/story-2004489-857f37e4f6a0fe5c.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      187 2024-03-15 14:52:19.000000 python-adjutant-8.0.0.0rc1/releasenotes/notes/toml-d8fba261f61313bf.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-15 14:52:52.694368 python-adjutant-8.0.0.0rc1/releasenotes/source/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8860 2024-03-15 14:52:19.000000 python-adjutant-8.0.0.0rc1/releasenotes/source/conf.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      752 2024-03-15 14:52:19.000000 python-adjutant-8.0.0.0rc1/releasenotes/source/index.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      108 2024-03-15 14:52:19.000000 python-adjutant-8.0.0.0rc1/releasenotes/source/unreleased.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      130 2024-03-15 14:52:19.000000 python-adjutant-8.0.0.0rc1/releasenotes/source/ussuri.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      138 2024-03-15 14:52:19.000000 python-adjutant-8.0.0.0rc1/releasenotes/source/victoria.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      134 2024-03-15 14:52:19.000000 python-adjutant-8.0.0.0rc1/releasenotes/source/wallaby.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      122 2024-03-15 14:52:19.000000 python-adjutant-8.0.0.0rc1/releasenotes/source/xena.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      122 2024-03-15 14:52:19.000000 python-adjutant-8.0.0.0rc1/releasenotes/source/yoga.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      118 2024-03-15 14:52:19.000000 python-adjutant-8.0.0.0rc1/releasenotes/source/zed.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      375 2024-03-15 14:52:19.000000 python-adjutant-8.0.0.0rc1/requirements.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1169 2024-03-15 14:52:52.694368 python-adjutant-8.0.0.0rc1/setup.cfg
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      693 2024-03-15 14:52:19.000000 python-adjutant-8.0.0.0rc1/setup.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      409 2024-03-15 14:52:19.000000 python-adjutant-8.0.0.0rc1/test-requirements.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2122 2024-03-15 14:52:19.000000 python-adjutant-8.0.0.0rc1/tox.ini
```

### Comparing `python-adjutant-8.0.0/.zuul.yaml` & `python-adjutant-8.0.0.0rc1/.zuul.yaml`

 * *Files identical despite different names*

### Comparing `python-adjutant-8.0.0/AUTHORS` & `python-adjutant-8.0.0.0rc1/AUTHORS`

 * *Files identical despite different names*

### Comparing `python-adjutant-8.0.0/ChangeLog` & `python-adjutant-8.0.0.0rc1/ChangeLog`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 CHANGES
 =======
 
-8.0.0
------
+8.0.0.0rc1
+----------
 
 * Simplify Adjutant bindep dependencies
 
 7.0.0
 -----
 
 * Update documentation to reflect newer OpenStack and confspirator
```

### Comparing `python-adjutant-8.0.0/LICENSE` & `python-adjutant-8.0.0.0rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `python-adjutant-8.0.0/PKG-INFO` & `python-adjutant-8.0.0.0rc1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-adjutant
-Version: 8.0.0
+Version: 8.0.0.0rc1
 Summary: An admin task workflow service for openstack.
 Home-page: https://opendev.org/openstack/adjutant
 Author: OpenStack
 Author-email: openstack-discuss@lists.openstack.org
 License: Apache-2
 Project-URL: Bug Tracker, https://storyboard.openstack.org/#!/project/openstack/adjutant
 Project-URL: Documentation, https://docs.openstack.org/adjutant/latest/
```

### Comparing `python-adjutant-8.0.0/README.rst` & `python-adjutant-8.0.0.0rc1/README.rst`

 * *Files identical despite different names*

### Comparing `python-adjutant-8.0.0/adjutant/__init__.py` & `python-adjutant-8.0.0.0rc1/adjutant/__init__.py`

 * *Files identical despite different names*

### Comparing `python-adjutant-8.0.0/adjutant/actions/__init__.py` & `python-adjutant-8.0.0.0rc1/adjutant/actions/__init__.py`

 * *Files identical despite different names*

### Comparing `python-adjutant-8.0.0/adjutant/actions/migrations/0001_initial.py` & `python-adjutant-8.0.0.0rc1/adjutant/actions/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `python-adjutant-8.0.0/adjutant/actions/migrations/0004_auto_20190610_0209.py` & `python-adjutant-8.0.0.0rc1/adjutant/actions/migrations/0004_auto_20190610_0209.py`

 * *Files identical despite different names*

### Comparing `python-adjutant-8.0.0/adjutant/actions/models.py` & `python-adjutant-8.0.0.0rc1/adjutant/actions/models.py`

 * *Files identical despite different names*

### Comparing `python-adjutant-8.0.0/adjutant/actions/utils.py` & `python-adjutant-8.0.0.0rc1/adjutant/actions/utils.py`

 * *Files identical despite different names*

### Comparing `python-adjutant-8.0.0/adjutant/actions/v1/base.py` & `python-adjutant-8.0.0.0rc1/adjutant/actions/v1/base.py`

 * *Files identical despite different names*

### Comparing `python-adjutant-8.0.0/adjutant/actions/v1/misc.py` & `python-adjutant-8.0.0.0rc1/adjutant/actions/v1/misc.py`

 * *Files identical despite different names*

### Comparing `python-adjutant-8.0.0/adjutant/actions/v1/projects.py` & `python-adjutant-8.0.0.0rc1/adjutant/actions/v1/projects.py`

 * *Files identical despite different names*

### Comparing `python-adjutant-8.0.0/adjutant/actions/v1/resources.py` & `python-adjutant-8.0.0.0rc1/adjutant/actions/v1/resources.py`

 * *Files identical despite different names*

### Comparing `python-adjutant-8.0.0/adjutant/actions/v1/serializers.py` & `python-adjutant-8.0.0.0rc1/adjutant/actions/v1/serializers.py`

 * *Files identical despite different names*

### Comparing `python-adjutant-8.0.0/adjutant/actions/v1/tests/test_misc_actions.py` & `python-adjutant-8.0.0.0rc1/adjutant/actions/v1/tests/test_misc_actions.py`

 * *Files identical despite different names*

### Comparing `python-adjutant-8.0.0/adjutant/actions/v1/tests/test_project_actions.py` & `python-adjutant-8.0.0.0rc1/adjutant/actions/v1/tests/test_project_actions.py`

 * *Files identical despite different names*

### Comparing `python-adjutant-8.0.0/adjutant/actions/v1/tests/test_resource_actions.py` & `python-adjutant-8.0.0.0rc1/adjutant/actions/v1/tests/test_resource_actions.py`

 * *Files identical despite different names*

### Comparing `python-adjutant-8.0.0/adjutant/actions/v1/tests/test_user_actions.py` & `python-adjutant-8.0.0.0rc1/adjutant/actions/v1/tests/test_user_actions.py`

 * *Files identical despite different names*

### Comparing `python-adjutant-8.0.0/adjutant/actions/v1/users.py` & `python-adjutant-8.0.0.0rc1/adjutant/actions/v1/users.py`

 * *Files identical despite different names*

### Comparing `python-adjutant-8.0.0/adjutant/api/__init__.py` & `python-adjutant-8.0.0.0rc1/adjutant/api/__init__.py`

 * *Files identical despite different names*

### Comparing `python-adjutant-8.0.0/adjutant/api/exception_handler.py` & `python-adjutant-8.0.0.0rc1/adjutant/api/exception_handler.py`

 * *Files identical despite different names*

### Comparing `python-adjutant-8.0.0/adjutant/api/migrations/0001_initial.py` & `python-adjutant-8.0.0.0rc1/adjutant/api/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `python-adjutant-8.0.0/adjutant/api/migrations/0006_auto_20190610_0209.py` & `python-adjutant-8.0.0.0rc1/adjutant/api/migrations/0006_auto_20190610_0209.py`

 * *Files identical despite different names*

### Comparing `python-adjutant-8.0.0/adjutant/api/migrations/0007_auto_20190610_0209.py` & `python-adjutant-8.0.0.0rc1/adjutant/api/migrations/0007_auto_20190610_0209.py`

 * *Files identical despite different names*

### Comparing `python-adjutant-8.0.0/adjutant/api/migrations/0008_auto_20190610_0209.py` & `python-adjutant-8.0.0.0rc1/adjutant/api/migrations/0008_auto_20190610_0209.py`

 * *Files identical despite different names*

### Comparing `python-adjutant-8.0.0/adjutant/api/models.py` & `python-adjutant-8.0.0.0rc1/adjutant/api/models.py`

 * *Files identical despite different names*

### Comparing `python-adjutant-8.0.0/adjutant/api/urls.py` & `python-adjutant-8.0.0.0rc1/adjutant/api/urls.py`

 * *Files identical despite different names*

### Comparing `python-adjutant-8.0.0/adjutant/api/utils.py` & `python-adjutant-8.0.0.0rc1/adjutant/api/utils.py`

 * *Files identical despite different names*

### Comparing `python-adjutant-8.0.0/adjutant/api/v1/base.py` & `python-adjutant-8.0.0.0rc1/adjutant/api/v1/base.py`

 * *Files identical despite different names*

### Comparing `python-adjutant-8.0.0/adjutant/api/v1/openstack.py` & `python-adjutant-8.0.0.0rc1/adjutant/api/v1/openstack.py`

 * *Files identical despite different names*

### Comparing `python-adjutant-8.0.0/adjutant/api/v1/tasks.py` & `python-adjutant-8.0.0.0rc1/adjutant/api/v1/tasks.py`

 * *Files identical despite different names*

### Comparing `python-adjutant-8.0.0/adjutant/api/v1/tests/test_api_admin.py` & `python-adjutant-8.0.0.0rc1/adjutant/api/v1/tests/test_api_admin.py`

 * *Files identical despite different names*

### Comparing `python-adjutant-8.0.0/adjutant/api/v1/tests/test_api_openstack.py` & `python-adjutant-8.0.0.0rc1/adjutant/api/v1/tests/test_api_openstack.py`

 * *Files identical despite different names*

### Comparing `python-adjutant-8.0.0/adjutant/api/v1/tests/test_api_taskview.py` & `python-adjutant-8.0.0.0rc1/adjutant/api/v1/tests/test_api_taskview.py`

 * *Files identical despite different names*

### Comparing `python-adjutant-8.0.0/adjutant/api/v1/urls.py` & `python-adjutant-8.0.0.0rc1/adjutant/api/v1/urls.py`

 * *Files identical despite different names*

### Comparing `python-adjutant-8.0.0/adjutant/api/v1/utils.py` & `python-adjutant-8.0.0.0rc1/adjutant/api/v1/utils.py`

 * *Files identical despite different names*

### Comparing `python-adjutant-8.0.0/adjutant/api/v1/views.py` & `python-adjutant-8.0.0.0rc1/adjutant/api/v1/views.py`

 * *Files identical despite different names*

### Comparing `python-adjutant-8.0.0/adjutant/api/views.py` & `python-adjutant-8.0.0.0rc1/adjutant/api/views.py`

 * *Files identical despite different names*

### Comparing `python-adjutant-8.0.0/adjutant/common/constants.py` & `python-adjutant-8.0.0.0rc1/adjutant/common/constants.py`

 * *Files identical despite different names*

### Comparing `python-adjutant-8.0.0/adjutant/common/openstack_clients.py` & `python-adjutant-8.0.0.0rc1/adjutant/common/openstack_clients.py`

 * *Files identical despite different names*

### Comparing `python-adjutant-8.0.0/adjutant/common/quota.py` & `python-adjutant-8.0.0.0rc1/adjutant/common/quota.py`

 * *Files identical despite different names*

### Comparing `python-adjutant-8.0.0/adjutant/common/tests/fake_clients.py` & `python-adjutant-8.0.0.0rc1/adjutant/common/tests/fake_clients.py`

 * *Files identical despite different names*

### Comparing `python-adjutant-8.0.0/adjutant/common/tests/utils.py` & `python-adjutant-8.0.0.0rc1/adjutant/common/tests/utils.py`

 * *Files identical despite different names*

### Comparing `python-adjutant-8.0.0/adjutant/common/user_store.py` & `python-adjutant-8.0.0.0rc1/adjutant/common/user_store.py`

 * *Files identical despite different names*

### Comparing `python-adjutant-8.0.0/adjutant/common/utils.py` & `python-adjutant-8.0.0.0rc1/adjutant/common/utils.py`

 * *Files identical despite different names*

### Comparing `python-adjutant-8.0.0/adjutant/config/__init__.py` & `python-adjutant-8.0.0.0rc1/adjutant/config/__init__.py`

 * *Files identical despite different names*

### Comparing `python-adjutant-8.0.0/adjutant/config/api.py` & `python-adjutant-8.0.0.0rc1/adjutant/config/api.py`

 * *Files identical despite different names*

### Comparing `python-adjutant-8.0.0/adjutant/config/django.py` & `python-adjutant-8.0.0.0rc1/adjutant/config/django.py`

 * *Files identical despite different names*

### Comparing `python-adjutant-8.0.0/adjutant/config/feature_sets.py` & `python-adjutant-8.0.0.0rc1/adjutant/config/feature_sets.py`

 * *Files identical despite different names*

### Comparing `python-adjutant-8.0.0/adjutant/config/identity.py` & `python-adjutant-8.0.0.0rc1/adjutant/config/identity.py`

 * *Files identical despite different names*

### Comparing `python-adjutant-8.0.0/adjutant/config/notification.py` & `python-adjutant-8.0.0.0rc1/adjutant/config/notification.py`

 * *Files identical despite different names*

### Comparing `python-adjutant-8.0.0/adjutant/config/quota.py` & `python-adjutant-8.0.0.0rc1/adjutant/config/quota.py`

 * *Files identical despite different names*

### Comparing `python-adjutant-8.0.0/adjutant/config/workflow.py` & `python-adjutant-8.0.0.0rc1/adjutant/config/workflow.py`

 * *Files identical despite different names*

### Comparing `python-adjutant-8.0.0/adjutant/core.py` & `python-adjutant-8.0.0.0rc1/adjutant/core.py`

 * *Files identical despite different names*

### Comparing `python-adjutant-8.0.0/adjutant/exceptions.py` & `python-adjutant-8.0.0.0rc1/adjutant/exceptions.py`

 * *Files identical despite different names*

### Comparing `python-adjutant-8.0.0/adjutant/feature_set.py` & `python-adjutant-8.0.0.0rc1/adjutant/feature_set.py`

 * *Files identical despite different names*

### Comparing `python-adjutant-8.0.0/adjutant/middleware.py` & `python-adjutant-8.0.0.0rc1/adjutant/middleware.py`

 * *Files identical despite different names*

### Comparing `python-adjutant-8.0.0/adjutant/notifications/__init__.py` & `python-adjutant-8.0.0.0rc1/adjutant/notifications/__init__.py`

 * *Files identical despite different names*

### Comparing `python-adjutant-8.0.0/adjutant/notifications/templates/notification.txt` & `python-adjutant-8.0.0.0rc1/adjutant/notifications/templates/notification.txt`

 * *Files identical despite different names*

### Comparing `python-adjutant-8.0.0/adjutant/notifications/utils.py` & `python-adjutant-8.0.0.0rc1/adjutant/notifications/utils.py`

 * *Files identical despite different names*

### Comparing `python-adjutant-8.0.0/adjutant/notifications/v1/base.py` & `python-adjutant-8.0.0.0rc1/adjutant/notifications/v1/base.py`

 * *Files identical despite different names*

### Comparing `python-adjutant-8.0.0/adjutant/notifications/v1/email.py` & `python-adjutant-8.0.0.0rc1/adjutant/notifications/v1/email.py`

 * *Files identical despite different names*

### Comparing `python-adjutant-8.0.0/adjutant/notifications/v1/tests/test_notifications.py` & `python-adjutant-8.0.0.0rc1/adjutant/notifications/v1/tests/test_notifications.py`

 * *Files identical despite different names*

### Comparing `python-adjutant-8.0.0/adjutant/settings.py` & `python-adjutant-8.0.0.0rc1/adjutant/settings.py`

 * *Files identical despite different names*

### Comparing `python-adjutant-8.0.0/adjutant/startup/checks.py` & `python-adjutant-8.0.0.0rc1/adjutant/startup/checks.py`

 * *Files identical despite different names*

### Comparing `python-adjutant-8.0.0/adjutant/startup/config.py` & `python-adjutant-8.0.0.0rc1/adjutant/startup/config.py`

 * *Files identical despite different names*

### Comparing `python-adjutant-8.0.0/adjutant/startup/loading.py` & `python-adjutant-8.0.0.0rc1/adjutant/startup/loading.py`

 * *Files identical despite different names*

### Comparing `python-adjutant-8.0.0/adjutant/tasks/__init__.py` & `python-adjutant-8.0.0.0rc1/adjutant/tasks/__init__.py`

 * *Files identical despite different names*

### Comparing `python-adjutant-8.0.0/adjutant/tasks/migrations/0001_initial.py` & `python-adjutant-8.0.0.0rc1/adjutant/tasks/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `python-adjutant-8.0.0/adjutant/tasks/migrations/0002_auto_20190619_0613.py` & `python-adjutant-8.0.0.0rc1/adjutant/tasks/migrations/0002_auto_20190619_0613.py`

 * *Files identical despite different names*

### Comparing `python-adjutant-8.0.0/adjutant/tasks/models.py` & `python-adjutant-8.0.0.0rc1/adjutant/tasks/models.py`

 * *Files identical despite different names*

### Comparing `python-adjutant-8.0.0/adjutant/tasks/templates/create_project_and_user_completed.txt` & `python-adjutant-8.0.0.0rc1/adjutant/tasks/templates/create_project_and_user_completed.txt`

 * *Files identical despite different names*

### Comparing `python-adjutant-8.0.0/adjutant/tasks/templates/create_project_and_user_token.txt` & `python-adjutant-8.0.0.0rc1/adjutant/tasks/templates/create_project_and_user_token.txt`

 * *Files identical despite different names*

### Comparing `python-adjutant-8.0.0/adjutant/tasks/templates/invite_user_to_project_token.txt` & `python-adjutant-8.0.0.0rc1/adjutant/tasks/templates/invite_user_to_project_token.txt`

 * *Files identical despite different names*

### Comparing `python-adjutant-8.0.0/adjutant/tasks/v1/base.py` & `python-adjutant-8.0.0.0rc1/adjutant/tasks/v1/base.py`

 * *Files identical despite different names*

### Comparing `python-adjutant-8.0.0/adjutant/tasks/v1/manager.py` & `python-adjutant-8.0.0.0rc1/adjutant/tasks/v1/manager.py`

 * *Files identical despite different names*

### Comparing `python-adjutant-8.0.0/adjutant/tasks/v1/projects.py` & `python-adjutant-8.0.0.0rc1/adjutant/tasks/v1/projects.py`

 * *Files identical despite different names*

### Comparing `python-adjutant-8.0.0/adjutant/tasks/v1/resources.py` & `python-adjutant-8.0.0.0rc1/adjutant/tasks/v1/resources.py`

 * *Files identical despite different names*

### Comparing `python-adjutant-8.0.0/adjutant/tasks/v1/users.py` & `python-adjutant-8.0.0.0rc1/adjutant/tasks/v1/users.py`

 * *Files identical despite different names*

### Comparing `python-adjutant-8.0.0/adjutant/tasks/v1/utils.py` & `python-adjutant-8.0.0.0rc1/adjutant/tasks/v1/utils.py`

 * *Files identical despite different names*

### Comparing `python-adjutant-8.0.0/adjutant/urls.py` & `python-adjutant-8.0.0.0rc1/adjutant/urls.py`

 * *Files identical despite different names*

### Comparing `python-adjutant-8.0.0/adjutant/version.py` & `python-adjutant-8.0.0.0rc1/adjutant/version.py`

 * *Files identical despite different names*

### Comparing `python-adjutant-8.0.0/adjutant/wsgi.py` & `python-adjutant-8.0.0.0rc1/adjutant/wsgi.py`

 * *Files identical despite different names*

### Comparing `python-adjutant-8.0.0/api-ref/_static/fonts/glyphicons-halflings-regular.ttf` & `python-adjutant-8.0.0.0rc1/api-ref/_static/fonts/glyphicons-halflings-regular.ttf`

 * *Files identical despite different names*

### Comparing `python-adjutant-8.0.0/api-ref/_static/fonts/glyphicons-halflings-regular.woff` & `python-adjutant-8.0.0.0rc1/api-ref/_static/fonts/glyphicons-halflings-regular.woff`

 * *Files identical despite different names*

### Comparing `python-adjutant-8.0.0/api-ref/source/admin-api.inc` & `python-adjutant-8.0.0.0rc1/api-ref/source/admin-api.inc`

 * *Files identical despite different names*

### Comparing `python-adjutant-8.0.0/api-ref/source/conf.py` & `python-adjutant-8.0.0.0rc1/api-ref/source/conf.py`

 * *Files identical despite different names*

### Comparing `python-adjutant-8.0.0/api-ref/source/delegate-apis.inc` & `python-adjutant-8.0.0.0rc1/api-ref/source/delegate-apis.inc`

 * *Files identical despite different names*

### Comparing `python-adjutant-8.0.0/api-ref/source/http-status.yaml` & `python-adjutant-8.0.0.0rc1/api-ref/source/http-status.yaml`

 * *Files identical despite different names*

### Comparing `python-adjutant-8.0.0/api-ref/source/parameters.yaml` & `python-adjutant-8.0.0.0rc1/api-ref/source/parameters.yaml`

 * *Files identical despite different names*

### Comparing `python-adjutant-8.0.0/api-ref/source/v1-api-reference.rst` & `python-adjutant-8.0.0.0rc1/api-ref/source/v1-api-reference.rst`

 * *Files identical despite different names*

### Comparing `python-adjutant-8.0.0/doc/Makefile` & `python-adjutant-8.0.0.0rc1/doc/Makefile`

 * *Files identical despite different names*

### Comparing `python-adjutant-8.0.0/doc/source/conf.py` & `python-adjutant-8.0.0.0rc1/doc/source/conf.py`

 * *Files identical despite different names*

### Comparing `python-adjutant-8.0.0/doc/source/configuration.rst` & `python-adjutant-8.0.0.0rc1/doc/source/configuration.rst`

 * *Files identical despite different names*

### Comparing `python-adjutant-8.0.0/doc/source/contributing.rst` & `python-adjutant-8.0.0.0rc1/doc/source/contributing.rst`

 * *Files identical despite different names*

### Comparing `python-adjutant-8.0.0/doc/source/development.rst` & `python-adjutant-8.0.0.0rc1/doc/source/development.rst`

 * *Files identical despite different names*

### Comparing `python-adjutant-8.0.0/doc/source/devstack-guide.rst` & `python-adjutant-8.0.0.0rc1/doc/source/devstack-guide.rst`

 * *Files identical despite different names*

### Comparing `python-adjutant-8.0.0/doc/source/feature-sets.rst` & `python-adjutant-8.0.0.0rc1/doc/source/feature-sets.rst`

 * *Files identical despite different names*

### Comparing `python-adjutant-8.0.0/doc/source/features.rst` & `python-adjutant-8.0.0.0rc1/doc/source/features.rst`

 * *Files identical despite different names*

### Comparing `python-adjutant-8.0.0/doc/source/guide-lines.rst` & `python-adjutant-8.0.0.0rc1/doc/source/guide-lines.rst`

 * *Files identical despite different names*

### Comparing `python-adjutant-8.0.0/doc/source/history.rst` & `python-adjutant-8.0.0.0rc1/doc/source/history.rst`

 * *Files identical despite different names*

### Comparing `python-adjutant-8.0.0/doc/source/index.rst` & `python-adjutant-8.0.0.0rc1/doc/source/index.rst`

 * *Files identical despite different names*

### Comparing `python-adjutant-8.0.0/doc/source/quota.rst` & `python-adjutant-8.0.0.0rc1/doc/source/quota.rst`

 * *Files identical despite different names*

### Comparing `python-adjutant-8.0.0/doc/source/release-notes.rst` & `python-adjutant-8.0.0.0rc1/doc/source/release-notes.rst`

 * *Files identical despite different names*

### Comparing `python-adjutant-8.0.0/etc/adjutant.yaml` & `python-adjutant-8.0.0.0rc1/etc/adjutant.yaml`

 * *Files identical despite different names*

### Comparing `python-adjutant-8.0.0/package_readme.rst` & `python-adjutant-8.0.0.0rc1/package_readme.rst`

 * *Files identical despite different names*

### Comparing `python-adjutant-8.0.0/python_adjutant.egg-info/PKG-INFO` & `python-adjutant-8.0.0.0rc1/python_adjutant.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-adjutant
-Version: 8.0.0
+Version: 8.0.0.0rc1
 Summary: An admin task workflow service for openstack.
 Home-page: https://opendev.org/openstack/adjutant
 Author: OpenStack
 Author-email: openstack-discuss@lists.openstack.org
 License: Apache-2
 Project-URL: Bug Tracker, https://storyboard.openstack.org/#!/project/openstack/adjutant
 Project-URL: Documentation, https://docs.openstack.org/adjutant/latest/
```

### Comparing `python-adjutant-8.0.0/python_adjutant.egg-info/SOURCES.txt` & `python-adjutant-8.0.0.0rc1/python_adjutant.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `python-adjutant-8.0.0/releasenotes/notes/authed_token-6d29688676e7ee32.yaml` & `python-adjutant-8.0.0.0rc1/releasenotes/notes/authed_token-6d29688676e7ee32.yaml`

 * *Files identical despite different names*

### Comparing `python-adjutant-8.0.0/releasenotes/notes/django-2-2-465a8bb124f1f7fe.yaml` & `python-adjutant-8.0.0.0rc1/releasenotes/notes/django-2-2-465a8bb124f1f7fe.yaml`

 * *Files identical despite different names*

### Comparing `python-adjutant-8.0.0/releasenotes/notes/feature-sets-f363d132c8c377cf.yaml` & `python-adjutant-8.0.0.0rc1/releasenotes/notes/feature-sets-f363d132c8c377cf.yaml`

 * *Files identical despite different names*

### Comparing `python-adjutant-8.0.0/releasenotes/notes/story-2004488-5468c184cc3a4691.yaml` & `python-adjutant-8.0.0.0rc1/releasenotes/notes/story-2004488-5468c184cc3a4691.yaml`

 * *Files identical despite different names*

### Comparing `python-adjutant-8.0.0/releasenotes/notes/story-2004489-857f37e4f6a0fe5c.yaml` & `python-adjutant-8.0.0.0rc1/releasenotes/notes/story-2004489-857f37e4f6a0fe5c.yaml`

 * *Files identical despite different names*

### Comparing `python-adjutant-8.0.0/releasenotes/source/conf.py` & `python-adjutant-8.0.0.0rc1/releasenotes/source/conf.py`

 * *Files identical despite different names*

### Comparing `python-adjutant-8.0.0/releasenotes/source/index.rst` & `python-adjutant-8.0.0.0rc1/releasenotes/source/index.rst`

 * *Files identical despite different names*

### Comparing `python-adjutant-8.0.0/setup.cfg` & `python-adjutant-8.0.0.0rc1/setup.cfg`

 * *Files identical despite different names*

### Comparing `python-adjutant-8.0.0/setup.py` & `python-adjutant-8.0.0.0rc1/setup.py`

 * *Files identical despite different names*

### Comparing `python-adjutant-8.0.0/tox.ini` & `python-adjutant-8.0.0.0rc1/tox.ini`

 * *Files identical despite different names*

