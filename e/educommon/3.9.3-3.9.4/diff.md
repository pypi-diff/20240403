# Comparing `tmp/educommon-3.9.3.tar.gz` & `tmp/educommon-3.9.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "educommon-3.9.3.tar", last modified: Mon Mar 18 07:43:51 2024, max compression
+gzip compressed data, was "educommon-3.9.4.tar", last modified: Wed Apr  3 06:43:20 2024, max compression
```

## Comparing `educommon-3.9.3.tar` & `educommon-3.9.4.tar`

### file list

```diff
@@ -1,460 +1,460 @@
-drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-03-18 07:43:51.029514 educommon-3.9.3/
--rw-r--r--   0 toor      (1000) toor      (1000)      102 2022-07-05 14:23:59.000000 educommon-3.9.3/MANIFEST.in
--rw-r--r--   0 toor      (1000) toor      (1000)     1472 2024-03-18 07:43:51.028514 educommon-3.9.3/PKG-INFO
--rw-r--r--   0 toor      (1000) toor      (1000)     1042 2022-07-05 14:23:59.000000 educommon-3.9.3/README.rst
--rw-r--r--   0 toor      (1000) toor      (1000)     1981 2022-07-05 14:23:59.000000 educommon-3.9.3/UPGRADE.rst
--rw-r--r--   0 toor      (1000) toor      (1000)       38 2024-03-18 07:43:51.029514 educommon-3.9.3/setup.cfg
--rw-r--r--   0 toor      (1000) toor      (1000)     2223 2024-03-18 07:43:43.000000 educommon-3.9.3/setup.py
-drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-03-18 07:43:50.602514 educommon-3.9.3/src/
-drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-03-18 07:43:50.630514 educommon-3.9.3/src/educommon/
--rw-r--r--   0 toor      (1000) toor      (1000)      419 2024-03-18 07:43:43.000000 educommon-3.9.3/src/educommon/__init__.py
-drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-03-18 07:43:50.643514 educommon-3.9.3/src/educommon/about/
--rw-r--r--   0 toor      (1000) toor      (1000)     2685 2022-07-05 14:23:59.000000 educommon-3.9.3/src/educommon/about/README.rst
--rw-r--r--   0 toor      (1000) toor      (1000)      132 2024-03-18 07:43:43.000000 educommon-3.9.3/src/educommon/about/__init__.py
--rw-r--r--   0 toor      (1000) toor      (1000)      259 2024-03-18 07:43:43.000000 educommon-3.9.3/src/educommon/about/apps.py
-drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-03-18 07:43:50.602514 educommon-3.9.3/src/educommon/about/static/
-drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-03-18 07:43:50.644514 educommon-3.9.3/src/educommon/about/static/edu_about/
--rw-r--r--   0 toor      (1000) toor      (1000)     8382 2022-07-05 14:23:59.000000 educommon-3.9.3/src/educommon/about/static/edu_about/barsgroup.png
-drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-03-18 07:43:50.652514 educommon-3.9.3/src/educommon/about/ui/
--rw-r--r--   0 toor      (1000) toor      (1000)        1 2024-03-18 07:43:43.000000 educommon-3.9.3/src/educommon/about/ui/__init__.py
--rw-r--r--   0 toor      (1000) toor      (1000)      535 2022-07-05 14:23:59.000000 educommon-3.9.3/src/educommon/about/ui/about-window.js
--rw-r--r--   0 toor      (1000) toor      (1000)     5975 2024-03-18 07:43:43.000000 educommon-3.9.3/src/educommon/about/ui/actions.py
--rw-r--r--   0 toor      (1000) toor      (1000)      700 2022-07-05 14:23:59.000000 educommon-3.9.3/src/educommon/about/ui/common-tab.html
--rw-r--r--   0 toor      (1000) toor      (1000)    11192 2022-07-05 14:23:59.000000 educommon-3.9.3/src/educommon/about/ui/packages-tab.js
--rw-r--r--   0 toor      (1000) toor      (1000)      129 2022-07-05 14:23:59.000000 educommon-3.9.3/src/educommon/about/ui/postgresql-extensions-tab.js
--rw-r--r--   0 toor      (1000) toor      (1000)     5272 2024-03-18 07:43:43.000000 educommon-3.9.3/src/educommon/about/ui/ui.py
--rw-r--r--   0 toor      (1000) toor      (1000)      625 2024-03-18 07:43:43.000000 educommon-3.9.3/src/educommon/about/utils.py
-drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-03-18 07:43:50.656514 educommon-3.9.3/src/educommon/async_task/
--rw-r--r--   0 toor      (1000) toor      (1000)      110 2024-03-18 07:43:43.000000 educommon-3.9.3/src/educommon/async_task/__init__.py
--rw-r--r--   0 toor      (1000) toor      (1000)     6654 2024-03-18 07:43:43.000000 educommon-3.9.3/src/educommon/async_task/actions.py
--rw-r--r--   0 toor      (1000) toor      (1000)      143 2024-03-18 07:43:43.000000 educommon-3.9.3/src/educommon/async_task/apps.py
--rw-r--r--   0 toor      (1000) toor      (1000)      242 2024-03-18 07:43:43.000000 educommon-3.9.3/src/educommon/async_task/consts.py
--rw-r--r--   0 toor      (1000) toor      (1000)      117 2024-03-18 07:43:43.000000 educommon-3.9.3/src/educommon/async_task/exceptions.py
--rw-r--r--   0 toor      (1000) toor      (1000)     2706 2024-03-18 07:43:43.000000 educommon-3.9.3/src/educommon/async_task/helpers.py
--rw-r--r--   0 toor      (1000) toor      (1000)     3844 2024-03-18 07:43:43.000000 educommon-3.9.3/src/educommon/async_task/locker.py
-drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-03-18 07:43:50.658514 educommon-3.9.3/src/educommon/async_task/migrations/
--rw-r--r--   0 toor      (1000) toor      (1000)     3677 2024-03-18 07:43:43.000000 educommon-3.9.3/src/educommon/async_task/migrations/0001_initial.py
--rw-r--r--   0 toor      (1000) toor      (1000)     3359 2024-03-18 07:43:43.000000 educommon-3.9.3/src/educommon/async_task/migrations/0002_task_type_and_status_data.py
--rw-r--r--   0 toor      (1000) toor      (1000)        0 2024-03-18 07:43:43.000000 educommon-3.9.3/src/educommon/async_task/migrations/__init__.py
--rw-r--r--   0 toor      (1000) toor      (1000)     7430 2024-03-18 07:43:43.000000 educommon-3.9.3/src/educommon/async_task/models.py
--rw-r--r--   0 toor      (1000) toor      (1000)    11533 2024-03-18 07:43:43.000000 educommon-3.9.3/src/educommon/async_task/tasks.py
-drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-03-18 07:43:50.604514 educommon-3.9.3/src/educommon/async_task/templates/
-drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-03-18 07:43:50.659514 educommon-3.9.3/src/educommon/async_task/templates/ui-js/
--rw-r--r--   0 toor      (1000) toor      (1000)      749 2024-03-18 07:43:43.000000 educommon-3.9.3/src/educommon/async_task/templates/ui-js/async-task-list-win.js
--rw-r--r--   0 toor      (1000) toor      (1000)     1257 2024-03-18 07:43:43.000000 educommon-3.9.3/src/educommon/async_task/templates/ui-js/async-task-revoke.js
--rw-r--r--   0 toor      (1000) toor      (1000)      260 2024-03-18 07:43:43.000000 educommon-3.9.3/src/educommon/async_task/templates/ui-js/async-task-view-win.js
--rw-r--r--   0 toor      (1000) toor      (1000)     5446 2024-03-18 07:43:43.000000 educommon-3.9.3/src/educommon/async_task/ui.py
-drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-03-18 07:43:50.662514 educommon-3.9.3/src/educommon/async_tasks/
--rw-r--r--   0 toor      (1000) toor      (1000)      110 2024-03-18 07:43:43.000000 educommon-3.9.3/src/educommon/async_tasks/__init__.py
--rw-r--r--   0 toor      (1000) toor      (1000)      138 2024-03-18 07:43:43.000000 educommon-3.9.3/src/educommon/async_tasks/apps.py
--rw-r--r--   0 toor      (1000) toor      (1000)      251 2024-03-18 07:43:43.000000 educommon-3.9.3/src/educommon/async_tasks/exceptions.py
-drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-03-18 07:43:50.662514 educommon-3.9.3/src/educommon/async_tasks/fixtures/
--rw-r--r--   0 toor      (1000) toor      (1000)      303 2022-07-05 14:23:59.000000 educommon-3.9.3/src/educommon/async_tasks/fixtures/initial_data.json
--rw-r--r--   0 toor      (1000) toor      (1000)     3489 2024-03-18 07:43:43.000000 educommon-3.9.3/src/educommon/async_tasks/locks.py
-drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-03-18 07:43:50.665514 educommon-3.9.3/src/educommon/async_tasks/migrations/
--rw-r--r--   0 toor      (1000) toor      (1000)     4205 2024-03-18 07:43:43.000000 educommon-3.9.3/src/educommon/async_tasks/migrations/0001_initial.py
--rw-r--r--   0 toor      (1000) toor      (1000)      478 2024-03-18 07:43:43.000000 educommon-3.9.3/src/educommon/async_tasks/migrations/0002_load_initial_data.py
--rw-r--r--   0 toor      (1000) toor      (1000)        0 2024-03-18 07:43:43.000000 educommon-3.9.3/src/educommon/async_tasks/migrations/__init__.py
--rw-r--r--   0 toor      (1000) toor      (1000)     3539 2024-03-18 07:43:43.000000 educommon-3.9.3/src/educommon/async_tasks/models.py
--rw-r--r--   0 toor      (1000) toor      (1000)     1413 2024-03-18 07:43:43.000000 educommon-3.9.3/src/educommon/async_tasks/statuses.py
--rw-r--r--   0 toor      (1000) toor      (1000)    11374 2024-03-18 07:43:43.000000 educommon-3.9.3/src/educommon/async_tasks/tasks.py
-drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-03-18 07:43:50.669514 educommon-3.9.3/src/educommon/audit_log/
--rw-r--r--   0 toor      (1000) toor      (1000)     2772 2024-03-18 07:43:43.000000 educommon-3.9.3/src/educommon/audit_log/__init__.py
--rw-r--r--   0 toor      (1000) toor      (1000)     5980 2024-03-18 07:43:43.000000 educommon-3.9.3/src/educommon/audit_log/actions.py
--rw-r--r--   0 toor      (1000) toor      (1000)      310 2024-03-18 07:43:43.000000 educommon-3.9.3/src/educommon/audit_log/app_meta.py
--rw-r--r--   0 toor      (1000) toor      (1000)     5033 2024-03-18 07:43:43.000000 educommon-3.9.3/src/educommon/audit_log/apps.py
--rw-r--r--   0 toor      (1000) toor      (1000)      880 2024-03-18 07:43:43.000000 educommon-3.9.3/src/educommon/audit_log/constants.py
-drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-03-18 07:43:50.669514 educommon-3.9.3/src/educommon/audit_log/error_log/
--rw-r--r--   0 toor      (1000) toor      (1000)       97 2024-03-18 07:43:43.000000 educommon-3.9.3/src/educommon/audit_log/error_log/__init__.py
--rw-r--r--   0 toor      (1000) toor      (1000)     2327 2024-03-18 07:43:43.000000 educommon-3.9.3/src/educommon/audit_log/error_log/actions.py
--rw-r--r--   0 toor      (1000) toor      (1000)      738 2024-03-18 07:43:43.000000 educommon-3.9.3/src/educommon/audit_log/helpers.py
-drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-03-18 07:43:50.670514 educommon-3.9.3/src/educommon/audit_log/management/
--rw-r--r--   0 toor      (1000) toor      (1000)        0 2024-03-18 07:43:43.000000 educommon-3.9.3/src/educommon/audit_log/management/__init__.py
-drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-03-18 07:43:50.670514 educommon-3.9.3/src/educommon/audit_log/management/commands/
--rw-r--r--   0 toor      (1000) toor      (1000)        0 2024-03-18 07:43:43.000000 educommon-3.9.3/src/educommon/audit_log/management/commands/__init__.py
--rw-r--r--   0 toor      (1000) toor      (1000)     2945 2024-03-18 07:43:43.000000 educommon-3.9.3/src/educommon/audit_log/management/commands/reinstall_audit_log.py
--rw-r--r--   0 toor      (1000) toor      (1000)     1140 2024-03-18 07:43:43.000000 educommon-3.9.3/src/educommon/audit_log/middleware.py
-drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-03-18 07:43:50.674514 educommon-3.9.3/src/educommon/audit_log/migrations/
--rw-r--r--   0 toor      (1000) toor      (1000)     4461 2024-03-18 07:43:43.000000 educommon-3.9.3/src/educommon/audit_log/migrations/0001_initial.py
--rw-r--r--   0 toor      (1000) toor      (1000)     2831 2024-03-18 07:43:43.000000 educommon-3.9.3/src/educommon/audit_log/migrations/0002_install_audit_log.py
--rw-r--r--   0 toor      (1000) toor      (1000)      405 2024-03-18 07:43:43.000000 educommon-3.9.3/src/educommon/audit_log/migrations/0003_logproxy.py
--rw-r--r--   0 toor      (1000) toor      (1000)      282 2024-03-18 07:43:43.000000 educommon-3.9.3/src/educommon/audit_log/migrations/0004_reinstall_audit_log.py
--rw-r--r--   0 toor      (1000) toor      (1000)      709 2024-03-18 07:43:43.000000 educommon-3.9.3/src/educommon/audit_log/migrations/0005_postgresql_error.py
--rw-r--r--   0 toor      (1000) toor      (1000)      611 2024-03-18 07:43:43.000000 educommon-3.9.3/src/educommon/audit_log/migrations/0006_auto_20200806_1707.py
--rw-r--r--   0 toor      (1000) toor      (1000)      812 2024-03-18 07:43:43.000000 educommon-3.9.3/src/educommon/audit_log/migrations/0007_create_selective_tables_function.py
--rw-r--r--   0 toor      (1000) toor      (1000)      477 2024-03-18 07:43:43.000000 educommon-3.9.3/src/educommon/audit_log/migrations/0008_table_logged.py
--rw-r--r--   0 toor      (1000) toor      (1000)      287 2024-03-18 07:43:43.000000 educommon-3.9.3/src/educommon/audit_log/migrations/0009_reinstall_audit_log.py
--rw-r--r--   0 toor      (1000) toor      (1000)        1 2024-03-18 07:43:43.000000 educommon-3.9.3/src/educommon/audit_log/migrations/__init__.py
--rw-r--r--   0 toor      (1000) toor      (1000)    11682 2024-03-18 07:43:43.000000 educommon-3.9.3/src/educommon/audit_log/models.py
--rw-r--r--   0 toor      (1000) toor      (1000)     1241 2024-03-18 07:43:43.000000 educommon-3.9.3/src/educommon/audit_log/permissions.py
--rw-r--r--   0 toor      (1000) toor      (1000)     8559 2024-03-18 07:43:43.000000 educommon-3.9.3/src/educommon/audit_log/proxies.py
--rw-r--r--   0 toor      (1000) toor      (1000)      204 2024-03-18 07:43:43.000000 educommon-3.9.3/src/educommon/audit_log/routers.py
-drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-03-18 07:43:50.675514 educommon-3.9.3/src/educommon/audit_log/sql/
--rw-r--r--   0 toor      (1000) toor      (1000)     1511 2024-03-18 07:43:43.000000 educommon-3.9.3/src/educommon/audit_log/sql/configure_audit_log.sql
--rw-r--r--   0 toor      (1000) toor      (1000)    14107 2024-03-18 07:43:43.000000 educommon-3.9.3/src/educommon/audit_log/sql/install_audit_log.sql
--rw-r--r--   0 toor      (1000) toor      (1000)     2117 2024-03-18 07:43:43.000000 educommon-3.9.3/src/educommon/audit_log/ui.py
-drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-03-18 07:43:50.676514 educommon-3.9.3/src/educommon/audit_log/utils/
--rw-r--r--   0 toor      (1000) toor      (1000)    15603 2024-03-18 07:43:43.000000 educommon-3.9.3/src/educommon/audit_log/utils/__init__.py
--rw-r--r--   0 toor      (1000) toor      (1000)     1661 2024-03-18 07:43:43.000000 educommon-3.9.3/src/educommon/audit_log/utils/operations.py
-drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-03-18 07:43:50.676514 educommon-3.9.3/src/educommon/auth/
--rw-r--r--   0 toor      (1000) toor      (1000)      127 2024-03-18 07:43:43.000000 educommon-3.9.3/src/educommon/auth/__init__.py
-drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-03-18 07:43:50.681514 educommon-3.9.3/src/educommon/auth/rbac/
--rw-r--r--   0 toor      (1000) toor      (1000)      329 2024-03-18 07:43:43.000000 educommon-3.9.3/src/educommon/auth/rbac/__init__.py
--rw-r--r--   0 toor      (1000) toor      (1000)    26872 2024-03-18 07:43:43.000000 educommon-3.9.3/src/educommon/auth/rbac/actions.py
--rw-r--r--   0 toor      (1000) toor      (1000)      450 2024-03-18 07:43:43.000000 educommon-3.9.3/src/educommon/auth/rbac/app_meta.py
-drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-03-18 07:43:50.683514 educommon-3.9.3/src/educommon/auth/rbac/backends/
--rw-r--r--   0 toor      (1000) toor      (1000)        1 2024-03-18 07:43:43.000000 educommon-3.9.3/src/educommon/auth/rbac/backends/__init__.py
--rw-r--r--   0 toor      (1000) toor      (1000)     2995 2024-03-18 07:43:43.000000 educommon-3.9.3/src/educommon/auth/rbac/backends/base.py
--rw-r--r--   0 toor      (1000) toor      (1000)    10290 2024-03-18 07:43:43.000000 educommon-3.9.3/src/educommon/auth/rbac/backends/caching.py
--rw-r--r--   0 toor      (1000) toor      (1000)     5038 2024-03-18 07:43:43.000000 educommon-3.9.3/src/educommon/auth/rbac/backends/simple.py
--rw-r--r--   0 toor      (1000) toor      (1000)     2957 2024-03-18 07:43:43.000000 educommon-3.9.3/src/educommon/auth/rbac/checker.py
--rw-r--r--   0 toor      (1000) toor      (1000)     1074 2024-03-18 07:43:43.000000 educommon-3.9.3/src/educommon/auth/rbac/config.py
--rw-r--r--   0 toor      (1000) toor      (1000)      502 2024-03-18 07:43:43.000000 educommon-3.9.3/src/educommon/auth/rbac/constants.py
-drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-03-18 07:43:50.683514 educommon-3.9.3/src/educommon/auth/rbac/management/
--rw-r--r--   0 toor      (1000) toor      (1000)       71 2024-03-18 07:43:43.000000 educommon-3.9.3/src/educommon/auth/rbac/management/__init__.py
-drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-03-18 07:43:50.684514 educommon-3.9.3/src/educommon/auth/rbac/management/commands/
--rw-r--r--   0 toor      (1000) toor      (1000)        1 2024-03-18 07:43:43.000000 educommon-3.9.3/src/educommon/auth/rbac/management/commands/__init__.py
--rw-r--r--   0 toor      (1000) toor      (1000)     5520 2024-03-18 07:43:43.000000 educommon-3.9.3/src/educommon/auth/rbac/management/commands/rbac.py
--rw-r--r--   0 toor      (1000) toor      (1000)    16250 2024-03-18 07:43:43.000000 educommon-3.9.3/src/educommon/auth/rbac/manager.py
-drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-03-18 07:43:50.686514 educommon-3.9.3/src/educommon/auth/rbac/migrations/
--rw-r--r--   0 toor      (1000) toor      (1000)     5474 2024-03-18 07:43:43.000000 educommon-3.9.3/src/educommon/auth/rbac/migrations/0001_initial.py
--rw-r--r--   0 toor      (1000) toor      (1000)      577 2024-03-18 07:43:43.000000 educommon-3.9.3/src/educommon/auth/rbac/migrations/0002_model_modifier_metaclass_fix.py
--rw-r--r--   0 toor      (1000) toor      (1000)      470 2024-03-18 07:43:43.000000 educommon-3.9.3/src/educommon/auth/rbac/migrations/0003_permission_hidden.py
--rw-r--r--   0 toor      (1000) toor      (1000)     2077 2024-03-18 07:43:43.000000 educommon-3.9.3/src/educommon/auth/rbac/migrations/0004_auto_20171024_1245.py
--rw-r--r--   0 toor      (1000) toor      (1000)        1 2024-03-18 07:43:43.000000 educommon-3.9.3/src/educommon/auth/rbac/migrations/__init__.py
--rw-r--r--   0 toor      (1000) toor      (1000)    15146 2024-03-18 07:43:43.000000 educommon-3.9.3/src/educommon/auth/rbac/models.py
--rw-r--r--   0 toor      (1000) toor      (1000)      865 2024-03-18 07:43:43.000000 educommon-3.9.3/src/educommon/auth/rbac/permissions.py
-drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-03-18 07:43:50.608514 educommon-3.9.3/src/educommon/auth/rbac/templates/
-drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-03-18 07:43:50.696514 educommon-3.9.3/src/educommon/auth/rbac/templates/rbac/
--rw-r--r--   0 toor      (1000) toor      (1000)      335 2022-07-05 14:23:59.000000 educommon-3.9.3/src/educommon/auth/rbac/templates/rbac/role-add-window.js
--rw-r--r--   0 toor      (1000) toor      (1000)     7914 2022-07-05 14:23:59.000000 educommon-3.9.3/src/educommon/auth/rbac/templates/rbac/role-edit-window.js
--rw-r--r--   0 toor      (1000) toor      (1000)     3768 2022-07-05 14:23:59.000000 educommon-3.9.3/src/educommon/auth/rbac/templates/rbac/roles-list-window.js
--rw-r--r--   0 toor      (1000) toor      (1000)      536 2022-07-05 14:23:59.000000 educommon-3.9.3/src/educommon/auth/rbac/templates/rbac/roles-view-list-window.js
--rw-r--r--   0 toor      (1000) toor      (1000)    15735 2024-03-18 07:43:43.000000 educommon-3.9.3/src/educommon/auth/rbac/ui.py
--rw-r--r--   0 toor      (1000) toor      (1000)     7819 2024-03-18 07:43:43.000000 educommon-3.9.3/src/educommon/auth/rbac/utils.py
--rw-r--r--   0 toor      (1000) toor      (1000)      483 2024-03-18 07:43:43.000000 educommon-3.9.3/src/educommon/auth/rbac/validators.py
-drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-03-18 07:43:50.701514 educommon-3.9.3/src/educommon/auth/simple_auth/
--rw-r--r--   0 toor      (1000) toor      (1000)      267 2024-03-18 07:43:43.000000 educommon-3.9.3/src/educommon/auth/simple_auth/__init__.py
--rw-r--r--   0 toor      (1000) toor      (1000)    11943 2024-03-18 07:43:43.000000 educommon-3.9.3/src/educommon/auth/simple_auth/actions.py
--rw-r--r--   0 toor      (1000) toor      (1000)     1088 2024-03-18 07:43:43.000000 educommon-3.9.3/src/educommon/auth/simple_auth/app_meta.py
--rw-r--r--   0 toor      (1000) toor      (1000)     2522 2024-03-18 07:43:43.000000 educommon-3.9.3/src/educommon/auth/simple_auth/checkers.py
--rw-r--r--   0 toor      (1000) toor      (1000)      396 2024-03-18 07:43:43.000000 educommon-3.9.3/src/educommon/auth/simple_auth/const.py
-drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-03-18 07:43:50.702514 educommon-3.9.3/src/educommon/auth/simple_auth/migrations/
--rw-r--r--   0 toor      (1000) toor      (1000)     1396 2024-03-18 07:43:43.000000 educommon-3.9.3/src/educommon/auth/simple_auth/migrations/0001_initial.py
--rw-r--r--   0 toor      (1000) toor      (1000)        1 2024-03-18 07:43:43.000000 educommon-3.9.3/src/educommon/auth/simple_auth/migrations/__init__.py
--rw-r--r--   0 toor      (1000) toor      (1000)      700 2024-03-18 07:43:43.000000 educommon-3.9.3/src/educommon/auth/simple_auth/models.py
-drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-03-18 07:43:50.609514 educommon-3.9.3/src/educommon/auth/simple_auth/static/
-drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-03-18 07:43:50.703514 educommon-3.9.3/src/educommon/auth/simple_auth/static/simple_auth/
--rw-r--r--   0 toor      (1000) toor      (1000)      123 2022-07-05 14:23:59.000000 educommon-3.9.3/src/educommon/auth/simple_auth/static/simple_auth/simple_auth.css
-drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-03-18 07:43:50.609514 educommon-3.9.3/src/educommon/auth/simple_auth/templates/
-drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-03-18 07:43:50.722514 educommon-3.9.3/src/educommon/auth/simple_auth/templates/simple_auth/
--rw-r--r--   0 toor      (1000) toor      (1000)     1577 2022-07-05 14:23:59.000000 educommon-3.9.3/src/educommon/auth/simple_auth/templates/simple_auth/change_reset_password_page.html
-drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-03-18 07:43:50.731514 educommon-3.9.3/src/educommon/auth/simple_auth/templates/simple_auth/email/
--rw-r--r--   0 toor      (1000) toor      (1000)      635 2022-07-05 14:23:59.000000 educommon-3.9.3/src/educommon/auth/simple_auth/templates/simple_auth/email/reset_password.html
--rw-r--r--   0 toor      (1000) toor      (1000)     1444 2022-07-05 14:23:59.000000 educommon-3.9.3/src/educommon/auth/simple_auth/templates/simple_auth/login_page.html
--rw-r--r--   0 toor      (1000) toor      (1000)     1340 2022-07-05 14:23:59.000000 educommon-3.9.3/src/educommon/auth/simple_auth/templates/simple_auth/reset_password_page.html
--rw-r--r--   0 toor      (1000) toor      (1000)     4620 2024-03-18 07:43:43.000000 educommon-3.9.3/src/educommon/auth/simple_auth/ui.py
--rw-r--r--   0 toor      (1000) toor      (1000)      204 2024-03-18 07:43:43.000000 educommon-3.9.3/src/educommon/auth/simple_auth/validators.py
-drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-03-18 07:43:50.739514 educommon-3.9.3/src/educommon/contingent/
--rw-r--r--   0 toor      (1000) toor      (1000)        0 2024-03-18 07:43:43.000000 educommon-3.9.3/src/educommon/contingent/__init__.py
--rw-r--r--   0 toor      (1000) toor      (1000)     3035 2024-03-18 07:43:43.000000 educommon-3.9.3/src/educommon/contingent/actions.py
--rw-r--r--   0 toor      (1000) toor      (1000)      273 2024-03-18 07:43:43.000000 educommon-3.9.3/src/educommon/contingent/app_meta.py
--rw-r--r--   0 toor      (1000) toor      (1000)     6854 2024-03-18 07:43:43.000000 educommon-3.9.3/src/educommon/contingent/base.py
--rw-r--r--   0 toor      (1000) toor      (1000)    61449 2024-03-18 07:43:43.000000 educommon-3.9.3/src/educommon/contingent/catalogs.py
-drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-03-18 07:43:50.751514 educommon-3.9.3/src/educommon/contingent/contingent_plugin/
--rw-r--r--   0 toor      (1000) toor      (1000)        0 2024-03-18 07:43:43.000000 educommon-3.9.3/src/educommon/contingent/contingent_plugin/__init__.py
--rw-r--r--   0 toor      (1000) toor      (1000)      717 2024-03-18 07:43:43.000000 educommon-3.9.3/src/educommon/contingent/contingent_plugin/actions.py
--rw-r--r--   0 toor      (1000) toor      (1000)      697 2024-03-18 07:43:43.000000 educommon-3.9.3/src/educommon/contingent/contingent_plugin/apps.py
-drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-03-18 07:43:50.752514 educommon-3.9.3/src/educommon/contingent/contingent_plugin/migrations/
--rw-r--r--   0 toor      (1000) toor      (1000)     1594 2024-03-18 07:43:43.000000 educommon-3.9.3/src/educommon/contingent/contingent_plugin/migrations/0001_initial.py
--rw-r--r--   0 toor      (1000) toor      (1000)     1176 2024-03-18 07:43:43.000000 educommon-3.9.3/src/educommon/contingent/contingent_plugin/migrations/0002_add_contingent_model_deleted.py
--rw-r--r--   0 toor      (1000) toor      (1000)        1 2024-03-18 07:43:43.000000 educommon-3.9.3/src/educommon/contingent/contingent_plugin/migrations/__init__.py
--rw-r--r--   0 toor      (1000) toor      (1000)      769 2024-03-18 07:43:43.000000 educommon-3.9.3/src/educommon/contingent/contingent_plugin/model_views.py
--rw-r--r--   0 toor      (1000) toor      (1000)     2506 2024-03-18 07:43:43.000000 educommon-3.9.3/src/educommon/contingent/contingent_plugin/models.py
--rw-r--r--   0 toor      (1000) toor      (1000)     5181 2024-03-18 07:43:43.000000 educommon-3.9.3/src/educommon/contingent/contingent_plugin/observer.py
--rw-r--r--   0 toor      (1000) toor      (1000)      148 2024-03-18 07:43:43.000000 educommon-3.9.3/src/educommon/contingent/contingent_plugin/plugin_meta.py
--rw-r--r--   0 toor      (1000) toor      (1000)     3314 2024-03-18 07:43:43.000000 educommon-3.9.3/src/educommon/contingent/contingent_plugin/storage.py
--rw-r--r--   0 toor      (1000) toor      (1000)     7161 2024-03-18 07:43:43.000000 educommon-3.9.3/src/educommon/contingent/contingent_plugin/utils.py
-drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-03-18 07:43:50.764514 educommon-3.9.3/src/educommon/contingent/json_data/
--rw-r--r--   0 toor      (1000) toor      (1000)    20078 2024-03-18 07:43:43.000000 educommon-3.9.3/src/educommon/contingent/json_data/icao.json
--rw-r--r--   0 toor      (1000) toor      (1000)    53540 2022-07-05 14:23:59.000000 educommon-3.9.3/src/educommon/contingent/json_data/okogu.json
--rw-r--r--   0 toor      (1000) toor      (1000)    30877 2024-03-18 07:43:43.000000 educommon-3.9.3/src/educommon/contingent/json_data/oksm.json
-drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-03-18 07:43:50.764514 educommon-3.9.3/src/educommon/django/
--rw-r--r--   0 toor      (1000) toor      (1000)       69 2024-03-18 07:43:43.000000 educommon-3.9.3/src/educommon/django/__init__.py
-drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-03-18 07:43:50.770514 educommon-3.9.3/src/educommon/django/db/
--rw-r--r--   0 toor      (1000) toor      (1000)       73 2024-03-18 07:43:43.000000 educommon-3.9.3/src/educommon/django/db/__init__.py
--rw-r--r--   0 toor      (1000) toor      (1000)     7049 2024-03-18 07:43:43.000000 educommon-3.9.3/src/educommon/django/db/fields.py
-drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-03-18 07:43:50.771514 educommon-3.9.3/src/educommon/django/db/migration/
--rw-r--r--   0 toor      (1000) toor      (1000)     1882 2024-03-18 07:43:43.000000 educommon-3.9.3/src/educommon/django/db/migration/__init__.py
--rw-r--r--   0 toor      (1000) toor      (1000)     9527 2024-03-18 07:43:43.000000 educommon-3.9.3/src/educommon/django/db/migration/operations.py
-drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-03-18 07:43:50.772514 educommon-3.9.3/src/educommon/django/db/mixins/
--rw-r--r--   0 toor      (1000) toor      (1000)    14740 2024-03-18 07:43:43.000000 educommon-3.9.3/src/educommon/django/db/mixins/__init__.py
--rw-r--r--   0 toor      (1000) toor      (1000)    24715 2024-03-18 07:43:43.000000 educommon-3.9.3/src/educommon/django/db/mixins/date_interval.py
--rw-r--r--   0 toor      (1000) toor      (1000)    12173 2024-03-18 07:43:43.000000 educommon-3.9.3/src/educommon/django/db/mixins/validation.py
-drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-03-18 07:43:50.773514 educommon-3.9.3/src/educommon/django/db/model_view/
--rw-r--r--   0 toor      (1000) toor      (1000)    12363 2024-03-18 07:43:43.000000 educommon-3.9.3/src/educommon/django/db/model_view/__init__.py
--rw-r--r--   0 toor      (1000) toor      (1000)      631 2022-07-05 14:23:59.000000 educommon-3.9.3/src/educommon/django/db/model_view/table-view.html
--rw-r--r--   0 toor      (1000) toor      (1000)     2107 2024-03-18 07:43:43.000000 educommon-3.9.3/src/educommon/django/db/models.py
--rw-r--r--   0 toor      (1000) toor      (1000)    10990 2024-03-18 07:43:43.000000 educommon-3.9.3/src/educommon/django/db/observer.py
-drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-03-18 07:43:50.817514 educommon-3.9.3/src/educommon/django/db/partitioning/
--rw-r--r--   0 toor      (1000) toor      (1000)     4455 2022-07-05 14:23:59.000000 educommon-3.9.3/src/educommon/django/db/partitioning/README.md
--rw-r--r--   0 toor      (1000) toor      (1000)    22376 2024-03-18 07:43:43.000000 educommon-3.9.3/src/educommon/django/db/partitioning/__init__.py
-drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-03-18 07:43:50.824514 educommon-3.9.3/src/educommon/django/db/partitioning/management/
--rw-r--r--   0 toor      (1000) toor      (1000)        0 2024-03-18 07:43:43.000000 educommon-3.9.3/src/educommon/django/db/partitioning/management/__init__.py
-drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-03-18 07:43:50.826514 educommon-3.9.3/src/educommon/django/db/partitioning/management/commands/
--rw-r--r--   0 toor      (1000) toor      (1000)        0 2024-03-18 07:43:43.000000 educommon-3.9.3/src/educommon/django/db/partitioning/management/commands/__init__.py
--rw-r--r--   0 toor      (1000) toor      (1000)     1612 2024-03-18 07:43:43.000000 educommon-3.9.3/src/educommon/django/db/partitioning/management/commands/apply_partitioning.py
--rw-r--r--   0 toor      (1000) toor      (1000)     2235 2024-03-18 07:43:44.000000 educommon-3.9.3/src/educommon/django/db/partitioning/management/commands/clear_table.py
--rw-r--r--   0 toor      (1000) toor      (1000)     2082 2024-03-18 07:43:44.000000 educommon-3.9.3/src/educommon/django/db/partitioning/management/commands/split_table.py
--rw-r--r--   0 toor      (1000) toor      (1000)    20345 2022-07-05 14:23:59.000000 educommon-3.9.3/src/educommon/django/db/partitioning/partitioning.sql
--rw-r--r--   0 toor      (1000) toor      (1000)     3401 2022-07-05 14:23:59.000000 educommon-3.9.3/src/educommon/django/db/partitioning/triggers.sql
--rw-r--r--   0 toor      (1000) toor      (1000)     3268 2024-03-18 07:43:44.000000 educommon-3.9.3/src/educommon/django/db/routers.py
--rw-r--r--   0 toor      (1000) toor      (1000)      136 2024-03-18 07:43:44.000000 educommon-3.9.3/src/educommon/django/db/signals.py
--rw-r--r--   0 toor      (1000) toor      (1000)     9206 2024-03-18 07:43:44.000000 educommon-3.9.3/src/educommon/django/db/utils.py
-drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-03-18 07:43:50.827514 educommon-3.9.3/src/educommon/django/db/validators/
--rw-r--r--   0 toor      (1000) toor      (1000)     1986 2024-03-18 07:43:44.000000 educommon-3.9.3/src/educommon/django/db/validators/__init__.py
--rw-r--r--   0 toor      (1000) toor      (1000)    38886 2024-03-18 07:43:44.000000 educommon-3.9.3/src/educommon/django/db/validators/simple.py
-drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-03-18 07:43:50.827514 educommon-3.9.3/src/educommon/django/storages/
--rw-r--r--   0 toor      (1000) toor      (1000)        0 2024-03-18 07:43:44.000000 educommon-3.9.3/src/educommon/django/storages/__init__.py
-drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-03-18 07:43:50.834514 educommon-3.9.3/src/educommon/django/storages/atcfs/
--rw-r--r--   0 toor      (1000) toor      (1000)     2656 2022-07-05 14:23:59.000000 educommon-3.9.3/src/educommon/django/storages/atcfs/README.rst
--rw-r--r--   0 toor      (1000) toor      (1000)        0 2024-03-18 07:43:44.000000 educommon-3.9.3/src/educommon/django/storages/atcfs/__init__.py
--rw-r--r--   0 toor      (1000) toor      (1000)     6004 2024-03-18 07:43:44.000000 educommon-3.9.3/src/educommon/django/storages/atcfs/api.py
--rw-r--r--   0 toor      (1000) toor      (1000)      352 2024-03-18 07:43:44.000000 educommon-3.9.3/src/educommon/django/storages/atcfs/app_meta.py
--rw-r--r--   0 toor      (1000) toor      (1000)      106 2024-03-18 07:43:44.000000 educommon-3.9.3/src/educommon/django/storages/atcfs/exceptions.py
-drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-03-18 07:43:50.835514 educommon-3.9.3/src/educommon/django/storages/atcfs/management/
--rw-r--r--   0 toor      (1000) toor      (1000)        0 2024-03-18 07:43:44.000000 educommon-3.9.3/src/educommon/django/storages/atcfs/management/__init__.py
-drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-03-18 07:43:50.836514 educommon-3.9.3/src/educommon/django/storages/atcfs/management/commands/
--rw-r--r--   0 toor      (1000) toor      (1000)        0 2024-03-18 07:43:44.000000 educommon-3.9.3/src/educommon/django/storages/atcfs/management/commands/__init__.py
--rw-r--r--   0 toor      (1000) toor      (1000)     7416 2024-03-18 07:43:44.000000 educommon-3.9.3/src/educommon/django/storages/atcfs/management/commands/atcfs_migrate.py
--rw-r--r--   0 toor      (1000) toor      (1000)      160 2024-03-18 07:43:44.000000 educommon-3.9.3/src/educommon/django/storages/atcfs/models.py
--rw-r--r--   0 toor      (1000) toor      (1000)     2623 2024-03-18 07:43:44.000000 educommon-3.9.3/src/educommon/django/storages/atcfs/monkey_patching.py
--rw-r--r--   0 toor      (1000) toor      (1000)      808 2024-03-18 07:43:44.000000 educommon-3.9.3/src/educommon/django/storages/atcfs/settings.py
--rw-r--r--   0 toor      (1000) toor      (1000)     4180 2024-03-18 07:43:44.000000 educommon-3.9.3/src/educommon/django/storages/atcfs/storage.py
-drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-03-18 07:43:50.836514 educommon-3.9.3/src/educommon/django/storages/atcfs/templates/
--rw-r--r--   0 toor      (1000) toor      (1000)      196 2022-07-05 14:23:59.000000 educommon-3.9.3/src/educommon/django/storages/atcfs/templates/atcfs_unavailable.html
-drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-03-18 07:43:50.842514 educommon-3.9.3/src/educommon/extjs/
--rw-r--r--   0 toor      (1000) toor      (1000)       87 2024-03-18 07:43:44.000000 educommon-3.9.3/src/educommon/extjs/__init__.py
-drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-03-18 07:43:50.843514 educommon-3.9.3/src/educommon/extjs/fields/
--rw-r--r--   0 toor      (1000) toor      (1000)      110 2024-03-18 07:43:44.000000 educommon-3.9.3/src/educommon/extjs/fields/__init__.py
--rw-r--r--   0 toor      (1000) toor      (1000)     4099 2024-03-18 07:43:44.000000 educommon-3.9.3/src/educommon/extjs/fields/input_params.py
-drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-03-18 07:43:50.864514 educommon-3.9.3/src/educommon/importer/
--rw-r--r--   0 toor      (1000) toor      (1000)    37531 2024-03-18 07:43:44.000000 educommon-3.9.3/src/educommon/importer/XLSReader.py
--rw-r--r--   0 toor      (1000) toor      (1000)      147 2024-03-18 07:43:44.000000 educommon-3.9.3/src/educommon/importer/__init__.py
--rw-r--r--   0 toor      (1000) toor      (1000)    13402 2024-03-18 07:43:44.000000 educommon-3.9.3/src/educommon/importer/api.py
--rw-r--r--   0 toor      (1000) toor      (1000)      733 2024-03-18 07:43:44.000000 educommon-3.9.3/src/educommon/importer/constants.py
--rw-r--r--   0 toor      (1000) toor      (1000)    10270 2024-03-18 07:43:44.000000 educommon-3.9.3/src/educommon/importer/loggers.py
--rw-r--r--   0 toor      (1000) toor      (1000)    37353 2024-03-18 07:43:44.000000 educommon-3.9.3/src/educommon/importer/proxy.py
--rw-r--r--   0 toor      (1000) toor      (1000)     6244 2024-03-18 07:43:44.000000 educommon-3.9.3/src/educommon/importer/proxy_import.py
--rw-r--r--   0 toor      (1000) toor      (1000)     2087 2022-07-05 14:23:59.000000 educommon-3.9.3/src/educommon/importer/refactoring-notes.txt
--rw-r--r--   0 toor      (1000) toor      (1000)     1506 2024-03-18 07:43:44.000000 educommon-3.9.3/src/educommon/importer/report.py
--rw-r--r--   0 toor      (1000) toor      (1000)     8704 2022-07-05 14:23:59.000000 educommon-3.9.3/src/educommon/importer/test_file.xls
--rw-r--r--   0 toor      (1000) toor      (1000)     3918 2024-03-18 07:43:44.000000 educommon-3.9.3/src/educommon/importer/ui.py
--rw-r--r--   0 toor      (1000) toor      (1000)     1182 2024-03-18 07:43:44.000000 educommon-3.9.3/src/educommon/importer/validators.py
-drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-03-18 07:43:50.868514 educommon-3.9.3/src/educommon/integration_entities/
--rw-r--r--   0 toor      (1000) toor      (1000)      158 2024-03-18 07:43:44.000000 educommon-3.9.3/src/educommon/integration_entities/README.rst
--rw-r--r--   0 toor      (1000) toor      (1000)        0 2024-03-18 07:43:44.000000 educommon-3.9.3/src/educommon/integration_entities/__init__.py
--rw-r--r--   0 toor      (1000) toor      (1000)      448 2024-03-18 07:43:44.000000 educommon-3.9.3/src/educommon/integration_entities/consts.py
--rw-r--r--   0 toor      (1000) toor      (1000)     2005 2024-03-18 07:43:44.000000 educommon-3.9.3/src/educommon/integration_entities/entities.py
--rw-r--r--   0 toor      (1000) toor      (1000)      335 2024-03-18 07:43:44.000000 educommon-3.9.3/src/educommon/integration_entities/enums.py
--rw-r--r--   0 toor      (1000) toor      (1000)     9888 2024-03-18 07:43:44.000000 educommon-3.9.3/src/educommon/integration_entities/helpers.py
--rw-r--r--   0 toor      (1000) toor      (1000)     1115 2024-03-18 07:43:44.000000 educommon-3.9.3/src/educommon/integration_entities/mixins.py
-drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-03-18 07:43:50.868514 educommon-3.9.3/src/educommon/ioc/
--rw-r--r--   0 toor      (1000) toor      (1000)     4028 2024-03-18 07:43:44.000000 educommon-3.9.3/src/educommon/ioc/__init__.py
-drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-03-18 07:43:50.872514 educommon-3.9.3/src/educommon/logger/
--rw-r--r--   0 toor      (1000) toor      (1000)      822 2024-03-18 07:43:44.000000 educommon-3.9.3/src/educommon/logger/__init__.py
--rw-r--r--   0 toor      (1000) toor      (1000)        0 2024-03-18 07:43:44.000000 educommon-3.9.3/src/educommon/logger/app_settings.py
--rw-r--r--   0 toor      (1000) toor      (1000)      944 2024-03-18 07:43:44.000000 educommon-3.9.3/src/educommon/logger/apps.py
--rw-r--r--   0 toor      (1000) toor      (1000)      238 2024-03-18 07:43:44.000000 educommon-3.9.3/src/educommon/logger/consts.py
--rw-r--r--   0 toor      (1000) toor      (1000)      400 2024-03-18 07:43:44.000000 educommon-3.9.3/src/educommon/logger/formatters.py
--rw-r--r--   0 toor      (1000) toor      (1000)     1596 2024-03-18 07:43:44.000000 educommon-3.9.3/src/educommon/logger/helpers.py
--rw-r--r--   0 toor      (1000) toor      (1000)     2965 2024-03-18 07:43:44.000000 educommon-3.9.3/src/educommon/logger/loggers.py
--rw-r--r--   0 toor      (1000) toor      (1000)      138 2024-03-18 07:43:44.000000 educommon-3.9.3/src/educommon/logger/records.py
-drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-03-18 07:43:50.874514 educommon-3.9.3/src/educommon/m3/
--rw-r--r--   0 toor      (1000) toor      (1000)    17568 2024-03-18 07:43:44.000000 educommon-3.9.3/src/educommon/m3/__init__.py
-drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-03-18 07:43:50.875514 educommon-3.9.3/src/educommon/m3/extensions/
--rw-r--r--   0 toor      (1000) toor      (1000)      258 2024-03-18 07:43:44.000000 educommon-3.9.3/src/educommon/m3/extensions/__init__.py
-drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-03-18 07:43:50.875514 educommon-3.9.3/src/educommon/m3/extensions/listeners/
--rw-r--r--   0 toor      (1000) toor      (1000)     8897 2024-03-18 07:43:44.000000 educommon-3.9.3/src/educommon/m3/extensions/listeners/__init__.py
-drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-03-18 07:43:50.884514 educommon-3.9.3/src/educommon/m3/extensions/listeners/delete_check/
--rw-r--r--   0 toor      (1000) toor      (1000)        0 2024-03-18 07:43:44.000000 educommon-3.9.3/src/educommon/m3/extensions/listeners/delete_check/__init__.py
--rw-r--r--   0 toor      (1000) toor      (1000)      916 2022-07-05 14:23:59.000000 educommon-3.9.3/src/educommon/m3/extensions/listeners/delete_check/cancel-confirm-window.js
--rw-r--r--   0 toor      (1000) toor      (1000)     6131 2024-03-18 07:43:44.000000 educommon-3.9.3/src/educommon/m3/extensions/listeners/delete_check/listeners.py
--rw-r--r--   0 toor      (1000) toor      (1000)     7660 2024-03-18 07:43:44.000000 educommon-3.9.3/src/educommon/m3/extensions/listeners/delete_check/mixins.py
--rw-r--r--   0 toor      (1000) toor      (1000)       94 2022-07-05 14:23:59.000000 educommon-3.9.3/src/educommon/m3/extensions/listeners/delete_check/related-objects-window.html
--rw-r--r--   0 toor      (1000) toor      (1000)      467 2024-03-18 07:43:44.000000 educommon-3.9.3/src/educommon/m3/extensions/listeners/delete_check/signals.py
--rw-r--r--   0 toor      (1000) toor      (1000)     3507 2024-03-18 07:43:44.000000 educommon-3.9.3/src/educommon/m3/extensions/listeners/delete_check/ui.py
--rw-r--r--   0 toor      (1000) toor      (1000)     2979 2024-03-18 07:43:44.000000 educommon-3.9.3/src/educommon/m3/extensions/listeners/delete_check/utils.py
--rw-r--r--   0 toor      (1000) toor      (1000)     6912 2024-03-18 07:43:44.000000 educommon-3.9.3/src/educommon/m3/extensions/ui.py
--rw-r--r--   0 toor      (1000) toor      (1000)     5150 2024-03-18 07:43:44.000000 educommon-3.9.3/src/educommon/m3/transaction_context.py
-drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-03-18 07:43:50.886514 educommon-3.9.3/src/educommon/objectpack/
--rw-r--r--   0 toor      (1000) toor      (1000)       69 2024-03-18 07:43:44.000000 educommon-3.9.3/src/educommon/objectpack/__init__.py
--rw-r--r--   0 toor      (1000) toor      (1000)    14735 2024-03-18 07:43:44.000000 educommon-3.9.3/src/educommon/objectpack/actions.py
--rw-r--r--   0 toor      (1000) toor      (1000)      220 2024-03-18 07:43:44.000000 educommon-3.9.3/src/educommon/objectpack/apps.py
--rw-r--r--   0 toor      (1000) toor      (1000)     5166 2024-03-18 07:43:44.000000 educommon-3.9.3/src/educommon/objectpack/filters.py
-drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-03-18 07:43:50.902514 educommon-3.9.3/src/educommon/objectpack/templates/
--rw-r--r--   0 toor      (1000) toor      (1000)      437 2022-07-05 14:23:59.000000 educommon-3.9.3/src/educommon/objectpack/templates/base-grid-window.js
--rw-r--r--   0 toor      (1000) toor      (1000)     1408 2022-07-05 14:23:59.000000 educommon-3.9.3/src/educommon/objectpack/templates/filter-panel.js
--rw-r--r--   0 toor      (1000) toor      (1000)     1544 2022-07-05 14:23:59.000000 educommon-3.9.3/src/educommon/objectpack/templates/grid-panel.js
--rw-r--r--   0 toor      (1000) toor      (1000)     1842 2022-07-05 14:23:59.000000 educommon-3.9.3/src/educommon/objectpack/templates/multiSelectWindow.js
--rw-r--r--   0 toor      (1000) toor      (1000)     6741 2022-07-05 14:23:59.000000 educommon-3.9.3/src/educommon/objectpack/templates/multiselect-page-fix.js
--rw-r--r--   0 toor      (1000) toor      (1000)     1838 2022-07-05 14:23:59.000000 educommon-3.9.3/src/educommon/objectpack/templates/relations-check-mixin-template.html
--rw-r--r--   0 toor      (1000) toor      (1000)    14752 2024-03-18 07:43:44.000000 educommon-3.9.3/src/educommon/objectpack/ui.py
-drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-03-18 07:43:50.905514 educommon-3.9.3/src/educommon/report/
--rw-r--r--   0 toor      (1000) toor      (1000)    17854 2024-03-18 07:43:44.000000 educommon-3.9.3/src/educommon/report/__init__.py
--rw-r--r--   0 toor      (1000) toor      (1000)     8705 2024-03-18 07:43:44.000000 educommon-3.9.3/src/educommon/report/actions.py
-drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-03-18 07:43:50.913514 educommon-3.9.3/src/educommon/report/constructor/
--rw-r--r--   0 toor      (1000) toor      (1000)     1138 2022-07-05 14:23:59.000000 educommon-3.9.3/src/educommon/report/constructor/README.rst
--rw-r--r--   0 toor      (1000) toor      (1000)     1252 2024-03-18 07:43:44.000000 educommon-3.9.3/src/educommon/report/constructor/__init__.py
--rw-r--r--   0 toor      (1000) toor      (1000)      200 2024-03-18 07:43:44.000000 educommon-3.9.3/src/educommon/report/constructor/app_meta.py
--rw-r--r--   0 toor      (1000) toor      (1000)      371 2024-03-18 07:43:44.000000 educommon-3.9.3/src/educommon/report/constructor/apps.py
--rw-r--r--   0 toor      (1000) toor      (1000)    26007 2024-03-18 07:43:44.000000 educommon-3.9.3/src/educommon/report/constructor/base.py
-drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-03-18 07:43:50.913514 educommon-3.9.3/src/educommon/report/constructor/builders/
--rw-r--r--   0 toor      (1000) toor      (1000)        1 2024-03-18 07:43:44.000000 educommon-3.9.3/src/educommon/report/constructor/builders/__init__.py
-drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-03-18 07:43:50.916514 educommon-3.9.3/src/educommon/report/constructor/builders/excel/
--rw-r--r--   0 toor      (1000) toor      (1000)      104 2024-03-18 07:43:44.000000 educommon-3.9.3/src/educommon/report/constructor/builders/excel/__init__.py
--rw-r--r--   0 toor      (1000) toor      (1000)    55789 2024-03-18 07:43:44.000000 educommon-3.9.3/src/educommon/report/constructor/builders/excel/_base.py
--rw-r--r--   0 toor      (1000) toor      (1000)     4758 2024-03-18 07:43:44.000000 educommon-3.9.3/src/educommon/report/constructor/builders/excel/_header.py
--rw-r--r--   0 toor      (1000) toor      (1000)       28 2024-03-18 07:43:44.000000 educommon-3.9.3/src/educommon/report/constructor/builders/excel/constants.py
--rw-r--r--   0 toor      (1000) toor      (1000)     6229 2024-03-18 07:43:44.000000 educommon-3.9.3/src/educommon/report/constructor/builders/excel/product.py
--rw-r--r--   0 toor      (1000) toor      (1000)     5150 2024-03-18 07:43:44.000000 educommon-3.9.3/src/educommon/report/constructor/builders/excel/with_merged_cells.py
--rw-r--r--   0 toor      (1000) toor      (1000)     1058 2024-03-18 07:43:44.000000 educommon-3.9.3/src/educommon/report/constructor/config.py
--rw-r--r--   0 toor      (1000) toor      (1000)     3381 2024-03-18 07:43:44.000000 educommon-3.9.3/src/educommon/report/constructor/constants.py
-drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-03-18 07:43:50.928514 educommon-3.9.3/src/educommon/report/constructor/editor/
--rw-r--r--   0 toor      (1000) toor      (1000)       41 2024-03-18 07:43:44.000000 educommon-3.9.3/src/educommon/report/constructor/editor/__init__.py
--rw-r--r--   0 toor      (1000) toor      (1000)    38810 2024-03-18 07:43:44.000000 educommon-3.9.3/src/educommon/report/constructor/editor/actions.py
--rw-r--r--   0 toor      (1000) toor      (1000)    39225 2022-07-05 14:23:59.000000 educommon-3.9.3/src/educommon/report/constructor/editor/edit-window.js
--rw-r--r--   0 toor      (1000) toor      (1000)     3247 2022-07-05 14:23:59.000000 educommon-3.9.3/src/educommon/report/constructor/editor/list-window.js
--rw-r--r--   0 toor      (1000) toor      (1000)    24628 2024-03-18 07:43:44.000000 educommon-3.9.3/src/educommon/report/constructor/editor/ui.py
--rw-r--r--   0 toor      (1000) toor      (1000)     1287 2024-03-18 07:43:44.000000 educommon-3.9.3/src/educommon/report/constructor/exceptions.py
-drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-03-18 07:43:50.933514 educommon-3.9.3/src/educommon/report/constructor/migrations/
--rw-r--r--   0 toor      (1000) toor      (1000)     3393 2024-03-18 07:43:44.000000 educommon-3.9.3/src/educommon/report/constructor/migrations/0001_initial.py
--rw-r--r--   0 toor      (1000) toor      (1000)     5009 2024-03-18 07:43:44.000000 educommon-3.9.3/src/educommon/report/constructor/migrations/0002_report_filters.py
--rw-r--r--   0 toor      (1000) toor      (1000)      472 2024-03-18 07:43:44.000000 educommon-3.9.3/src/educommon/report/constructor/migrations/0003_reportfilter_exclude.py
--rw-r--r--   0 toor      (1000) toor      (1000)     1369 2024-03-18 07:43:44.000000 educommon-3.9.3/src/educommon/report/constructor/migrations/0004_reportfilter_fields.py
--rw-r--r--   0 toor      (1000) toor      (1000)      431 2024-03-18 07:43:44.000000 educommon-3.9.3/src/educommon/report/constructor/migrations/0005_reportcolumn_visible.py
--rw-r--r--   0 toor      (1000) toor      (1000)     1284 2024-03-18 07:43:44.000000 educommon-3.9.3/src/educommon/report/constructor/migrations/0006_reportsorting.py
--rw-r--r--   0 toor      (1000) toor      (1000)     1541 2024-03-18 07:43:44.000000 educommon-3.9.3/src/educommon/report/constructor/migrations/0007_include_available_units.py
--rw-r--r--   0 toor      (1000) toor      (1000)      557 2024-03-18 07:43:44.000000 educommon-3.9.3/src/educommon/report/constructor/migrations/0008_auto_20170407_1318.py
--rw-r--r--   0 toor      (1000) toor      (1000)      519 2024-03-18 07:43:44.000000 educommon-3.9.3/src/educommon/report/constructor/migrations/0009_auto_20180405_0642.py
--rw-r--r--   0 toor      (1000) toor      (1000)      949 2024-03-18 07:43:44.000000 educommon-3.9.3/src/educommon/report/constructor/migrations/0010_add_aggregate_fields.py
--rw-r--r--   0 toor      (1000) toor      (1000)        1 2024-03-18 07:43:44.000000 educommon-3.9.3/src/educommon/report/constructor/migrations/__init__.py
--rw-r--r--   0 toor      (1000) toor      (1000)     2377 2024-03-18 07:43:44.000000 educommon-3.9.3/src/educommon/report/constructor/mixins.py
--rw-r--r--   0 toor      (1000) toor      (1000)    18764 2024-03-18 07:43:44.000000 educommon-3.9.3/src/educommon/report/constructor/models.py
--rw-r--r--   0 toor      (1000) toor      (1000)      114 2024-03-18 07:43:44.000000 educommon-3.9.3/src/educommon/report/constructor/plugin_meta.py
--rw-r--r--   0 toor      (1000) toor      (1000)     1883 2024-03-18 07:43:44.000000 educommon-3.9.3/src/educommon/report/constructor/registries.py
--rw-r--r--   0 toor      (1000) toor      (1000)     6557 2024-03-18 07:43:44.000000 educommon-3.9.3/src/educommon/report/constructor/utils.py
--rw-r--r--   0 toor      (1000) toor      (1000)      524 2024-03-18 07:43:44.000000 educommon-3.9.3/src/educommon/report/constructor/validators.py
--rw-r--r--   0 toor      (1000) toor      (1000)    10026 2024-03-18 07:43:44.000000 educommon-3.9.3/src/educommon/report/reporter.py
--rw-r--r--   0 toor      (1000) toor      (1000)     9974 2024-03-18 07:43:44.000000 educommon-3.9.3/src/educommon/report/utils.py
-drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-03-18 07:43:50.936514 educommon-3.9.3/src/educommon/rest/
--rw-r--r--   0 toor      (1000) toor      (1000)        1 2024-03-18 07:43:44.000000 educommon-3.9.3/src/educommon/rest/__init__.py
--rw-r--r--   0 toor      (1000) toor      (1000)     1278 2024-03-18 07:43:44.000000 educommon-3.9.3/src/educommon/rest/actions.py
--rw-r--r--   0 toor      (1000) toor      (1000)     3908 2024-03-18 07:43:44.000000 educommon-3.9.3/src/educommon/rest/context.py
--rw-r--r--   0 toor      (1000) toor      (1000)     2516 2024-03-18 07:43:44.000000 educommon-3.9.3/src/educommon/rest/controllers.py
--rw-r--r--   0 toor      (1000) toor      (1000)      475 2024-03-18 07:43:44.000000 educommon-3.9.3/src/educommon/rest/misc.py
--rw-r--r--   0 toor      (1000) toor      (1000)     4840 2024-03-18 07:43:44.000000 educommon-3.9.3/src/educommon/rest/mixins.py
-drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-03-18 07:43:50.938514 educommon-3.9.3/src/educommon/secure_media/
--rw-r--r--   0 toor      (1000) toor      (1000)     4001 2022-07-05 14:23:59.000000 educommon-3.9.3/src/educommon/secure_media/README.rst
--rw-r--r--   0 toor      (1000) toor      (1000)        0 2024-03-18 07:43:44.000000 educommon-3.9.3/src/educommon/secure_media/__init__.py
--rw-r--r--   0 toor      (1000) toor      (1000)     1317 2024-03-18 07:43:44.000000 educommon-3.9.3/src/educommon/secure_media/app_meta.py
--rw-r--r--   0 toor      (1000) toor      (1000)       61 2024-03-18 07:43:44.000000 educommon-3.9.3/src/educommon/thread_data.py
-drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-03-18 07:43:50.947514 educommon-3.9.3/src/educommon/utils/
--rw-r--r--   0 toor      (1000) toor      (1000)     2441 2024-03-18 07:43:44.000000 educommon-3.9.3/src/educommon/utils/__init__.py
--rw-r--r--   0 toor      (1000) toor      (1000)     4063 2024-03-18 07:43:44.000000 educommon-3.9.3/src/educommon/utils/caching.py
--rw-r--r--   0 toor      (1000) toor      (1000)     1966 2024-03-18 07:43:44.000000 educommon-3.9.3/src/educommon/utils/conversion.py
--rw-r--r--   0 toor      (1000) toor      (1000)     2158 2024-03-18 07:43:44.000000 educommon-3.9.3/src/educommon/utils/crypto.py
--rw-r--r--   0 toor      (1000) toor      (1000)    16800 2024-03-18 07:43:44.000000 educommon-3.9.3/src/educommon/utils/date.py
-drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-03-18 07:43:50.948514 educommon-3.9.3/src/educommon/utils/db/
--rw-r--r--   0 toor      (1000) toor      (1000)     7734 2024-03-18 07:43:44.000000 educommon-3.9.3/src/educommon/utils/db/__init__.py
--rw-r--r--   0 toor      (1000) toor      (1000)     2820 2024-03-18 07:43:44.000000 educommon-3.9.3/src/educommon/utils/db/postgresql.py
-drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-03-18 07:43:50.987514 educommon-3.9.3/src/educommon/utils/fonts/
--rw-r--r--   0 toor      (1000) toor      (1000)   275572 2022-07-05 14:23:59.000000 educommon-3.9.3/src/educommon/utils/fonts/Arial.ttf
--rw-r--r--   0 toor      (1000) toor      (1000)   811820 2022-07-05 14:23:59.000000 educommon-3.9.3/src/educommon/utils/fonts/Calibri.ttf
--rw-r--r--   0 toor      (1000) toor      (1000)   265528 2022-07-05 14:23:59.000000 educommon-3.9.3/src/educommon/utils/fonts/Tahoma.ttf
--rw-r--r--   0 toor      (1000) toor      (1000)     4815 2024-03-18 07:43:44.000000 educommon-3.9.3/src/educommon/utils/fonts/__init__.py
-drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-03-18 07:43:50.989514 educommon-3.9.3/src/educommon/utils/licence/
--rw-r--r--   0 toor      (1000) toor      (1000)     5095 2024-03-18 07:43:44.000000 educommon-3.9.3/src/educommon/utils/licence/__init__.py
--rw-r--r--   0 toor      (1000) toor      (1000)     1174 2024-03-18 07:43:44.000000 educommon-3.9.3/src/educommon/utils/licence/converters.py
--rw-r--r--   0 toor      (1000) toor      (1000)     4254 2024-03-18 07:43:44.000000 educommon-3.9.3/src/educommon/utils/misc.py
--rw-r--r--   0 toor      (1000) toor      (1000)     9048 2024-03-18 07:43:44.000000 educommon-3.9.3/src/educommon/utils/object_grid.py
--rw-r--r--   0 toor      (1000) toor      (1000)     1157 2024-03-18 07:43:44.000000 educommon-3.9.3/src/educommon/utils/patches.py
--rw-r--r--   0 toor      (1000) toor      (1000)     9469 2024-03-18 07:43:44.000000 educommon-3.9.3/src/educommon/utils/plugins.py
--rw-r--r--   0 toor      (1000) toor      (1000)     1995 2024-03-18 07:43:44.000000 educommon-3.9.3/src/educommon/utils/registry.py
--rw-r--r--   0 toor      (1000) toor      (1000)      520 2024-03-18 07:43:44.000000 educommon-3.9.3/src/educommon/utils/seqtools.py
--rw-r--r--   0 toor      (1000) toor      (1000)     8787 2024-03-18 07:43:44.000000 educommon-3.9.3/src/educommon/utils/serializer.py
--rw-r--r--   0 toor      (1000) toor      (1000)     2883 2024-03-18 07:43:44.000000 educommon-3.9.3/src/educommon/utils/storage.py
--rw-r--r--   0 toor      (1000) toor      (1000)     2834 2024-03-18 07:43:44.000000 educommon-3.9.3/src/educommon/utils/system.py
-drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-03-18 07:43:50.989514 educommon-3.9.3/src/educommon/utils/system_app/
--rw-r--r--   0 toor      (1000) toor      (1000)        0 2024-03-18 07:43:44.000000 educommon-3.9.3/src/educommon/utils/system_app/__init__.py
-drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-03-18 07:43:50.989514 educommon-3.9.3/src/educommon/utils/system_app/management/
--rw-r--r--   0 toor      (1000) toor      (1000)        0 2024-03-18 07:43:44.000000 educommon-3.9.3/src/educommon/utils/system_app/management/__init__.py
-drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-03-18 07:43:50.990514 educommon-3.9.3/src/educommon/utils/system_app/management/commands/
--rw-r--r--   0 toor      (1000) toor      (1000)        0 2024-03-18 07:43:44.000000 educommon-3.9.3/src/educommon/utils/system_app/management/commands/__init__.py
--rw-r--r--   0 toor      (1000) toor      (1000)     9295 2024-03-18 07:43:44.000000 educommon-3.9.3/src/educommon/utils/system_app/management/commands/delete_objects.py
-drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-03-18 07:43:50.991514 educommon-3.9.3/src/educommon/utils/system_app/templatetags/
--rw-r--r--   0 toor      (1000) toor      (1000)        1 2024-03-18 07:43:44.000000 educommon-3.9.3/src/educommon/utils/system_app/templatetags/__init__.py
--rw-r--r--   0 toor      (1000) toor      (1000)      273 2024-03-18 07:43:44.000000 educommon-3.9.3/src/educommon/utils/system_app/templatetags/educommon.py
--rw-r--r--   0 toor      (1000) toor      (1000)    16082 2024-03-18 07:43:44.000000 educommon-3.9.3/src/educommon/utils/ui.py
-drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-03-18 07:43:51.002514 educommon-3.9.3/src/educommon/utils/xml/
--rw-r--r--   0 toor      (1000) toor      (1000)     2194 2024-03-18 07:43:44.000000 educommon-3.9.3/src/educommon/utils/xml/__init__.py
--rw-r--r--   0 toor      (1000) toor      (1000)      875 2022-07-05 14:23:59.000000 educommon-3.9.3/src/educommon/utils/xml/catalog.json
--rw-r--r--   0 toor      (1000) toor      (1000)     1750 2024-03-18 07:43:44.000000 educommon-3.9.3/src/educommon/utils/xml/resolver.py
--rw-r--r--   0 toor      (1000) toor      (1000)    13160 2022-07-05 14:23:59.000000 educommon-3.9.3/src/educommon/utils/xml/saml-schema-assertion-2.0.xsd
--rw-r--r--   0 toor      (1000) toor      (1000)    13465 2022-07-05 14:23:59.000000 educommon-3.9.3/src/educommon/utils/xml/saml-schema-protocol-2.0.xsd
--rw-r--r--   0 toor      (1000) toor      (1000)     5234 2022-07-05 14:23:59.000000 educommon-3.9.3/src/educommon/utils/xml/xenc-schema.xsd
--rw-r--r--   0 toor      (1000) toor      (1000)    10293 2022-07-05 14:23:59.000000 educommon-3.9.3/src/educommon/utils/xml/xmldsig-core-schema.xsd
--rw-r--r--   0 toor      (1000) toor      (1000)      448 2024-03-18 07:43:50.000000 educommon-3.9.3/src/educommon/version.conf
-drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-03-18 07:43:51.007514 educommon-3.9.3/src/educommon/ws_log/
--rw-r--r--   0 toor      (1000) toor      (1000)     5467 2022-07-05 14:23:59.000000 educommon-3.9.3/src/educommon/ws_log/README.rst
--rw-r--r--   0 toor      (1000) toor      (1000)      932 2024-03-18 07:43:44.000000 educommon-3.9.3/src/educommon/ws_log/__init__.py
--rw-r--r--   0 toor      (1000) toor      (1000)     9153 2024-03-18 07:43:44.000000 educommon-3.9.3/src/educommon/ws_log/actions.py
--rw-r--r--   0 toor      (1000) toor      (1000)       94 2024-03-18 07:43:44.000000 educommon-3.9.3/src/educommon/ws_log/app_meta.py
--rw-r--r--   0 toor      (1000) toor      (1000)     7138 2024-03-18 07:43:44.000000 educommon-3.9.3/src/educommon/ws_log/base.py
-drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-03-18 07:43:51.011514 educommon-3.9.3/src/educommon/ws_log/migrations/
--rw-r--r--   0 toor      (1000) toor      (1000)     2706 2024-03-18 07:43:44.000000 educommon-3.9.3/src/educommon/ws_log/migrations/0001_initial.py
--rw-r--r--   0 toor      (1000) toor      (1000)      910 2024-03-18 07:43:44.000000 educommon-3.9.3/src/educommon/ws_log/migrations/0002_auto_20160628_1334.py
--rw-r--r--   0 toor      (1000) toor      (1000)     1682 2024-03-18 07:43:44.000000 educommon-3.9.3/src/educommon/ws_log/migrations/0003_add_fields_to_smev_logs.py
--rw-r--r--   0 toor      (1000) toor      (1000)      932 2024-03-18 07:43:44.000000 educommon-3.9.3/src/educommon/ws_log/migrations/0004_auto_20160727_1600.py
--rw-r--r--   0 toor      (1000) toor      (1000)     1586 2024-03-18 07:43:44.000000 educommon-3.9.3/src/educommon/ws_log/migrations/0005_auto_20161130_1615.py
--rw-r--r--   0 toor      (1000) toor      (1000)      479 2024-03-18 07:43:44.000000 educommon-3.9.3/src/educommon/ws_log/migrations/0006_auto_20170327_1027.py
--rw-r--r--   0 toor      (1000) toor      (1000)     1171 2024-03-18 07:43:44.000000 educommon-3.9.3/src/educommon/ws_log/migrations/0007_auto_20180607_1040.py
--rw-r--r--   0 toor      (1000) toor      (1000)     1311 2024-03-18 07:43:44.000000 educommon-3.9.3/src/educommon/ws_log/migrations/0008_auto_20180713_1445.py
--rw-r--r--   0 toor      (1000) toor      (1000)      516 2024-03-18 07:43:44.000000 educommon-3.9.3/src/educommon/ws_log/migrations/0009_auto_20201130_1553.py
--rw-r--r--   0 toor      (1000) toor      (1000)        1 2024-03-18 07:43:44.000000 educommon-3.9.3/src/educommon/ws_log/migrations/__init__.py
--rw-r--r--   0 toor      (1000) toor      (1000)     5634 2024-03-18 07:43:44.000000 educommon-3.9.3/src/educommon/ws_log/models.py
--rw-r--r--   0 toor      (1000) toor      (1000)      885 2024-03-18 07:43:44.000000 educommon-3.9.3/src/educommon/ws_log/provider.py
--rw-r--r--   0 toor      (1000) toor      (1000)     3487 2024-03-18 07:43:44.000000 educommon-3.9.3/src/educommon/ws_log/report.py
-drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-03-18 07:43:51.012514 educommon-3.9.3/src/educommon/ws_log/smev/
--rw-r--r--   0 toor      (1000) toor      (1000)       84 2024-03-18 07:43:44.000000 educommon-3.9.3/src/educommon/ws_log/smev/__init__.py
--rw-r--r--   0 toor      (1000) toor      (1000)     5866 2024-03-18 07:43:44.000000 educommon-3.9.3/src/educommon/ws_log/smev/applications.py
--rw-r--r--   0 toor      (1000) toor      (1000)      601 2024-03-18 07:43:44.000000 educommon-3.9.3/src/educommon/ws_log/smev/exceptions.py
-drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-03-18 07:43:50.625514 educommon-3.9.3/src/educommon/ws_log/templates/
-drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-03-18 07:43:51.012514 educommon-3.9.3/src/educommon/ws_log/templates/report/
--rw-r--r--   0 toor      (1000) toor      (1000)    10439 2022-07-05 14:23:59.000000 educommon-3.9.3/src/educommon/ws_log/templates/report/smev_logs.xlsx
-drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-03-18 07:43:51.017514 educommon-3.9.3/src/educommon/ws_log/templates/ui-js/
--rw-r--r--   0 toor      (1000) toor      (1000)      513 2022-07-05 14:23:59.000000 educommon-3.9.3/src/educommon/ws_log/templates/ui-js/smev-logs-list-window.js
--rw-r--r--   0 toor      (1000) toor      (1000)     1103 2022-07-05 14:23:59.000000 educommon-3.9.3/src/educommon/ws_log/templates/ui-js/smev-logs-report-setting-window.js
--rw-r--r--   0 toor      (1000) toor      (1000)     4038 2024-03-18 07:43:44.000000 educommon-3.9.3/src/educommon/ws_log/ui.py
--rw-r--r--   0 toor      (1000) toor      (1000)     1753 2024-03-18 07:43:44.000000 educommon-3.9.3/src/educommon/ws_log/utils.py
-drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-03-18 07:43:51.027514 educommon-3.9.3/src/educommon.egg-info/
--rw-r--r--   0 toor      (1000) toor      (1000)     1472 2024-03-18 07:43:50.000000 educommon-3.9.3/src/educommon.egg-info/PKG-INFO
--rw-r--r--   0 toor      (1000) toor      (1000)    16404 2024-03-18 07:43:50.000000 educommon-3.9.3/src/educommon.egg-info/SOURCES.txt
--rw-r--r--   0 toor      (1000) toor      (1000)       43 2024-03-18 07:43:50.000000 educommon-3.9.3/src/educommon.egg-info/dependency_links.txt
--rw-r--r--   0 toor      (1000) toor      (1000)      351 2024-03-18 07:43:50.000000 educommon-3.9.3/src/educommon.egg-info/requires.txt
--rw-r--r--   0 toor      (1000) toor      (1000)       10 2024-03-18 07:43:50.000000 educommon-3.9.3/src/educommon.egg-info/top_level.txt
-drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-03-18 07:43:51.024514 educommon-3.9.3/tests/
--rw-r--r--   0 toor      (1000) toor      (1000)     6188 2024-03-18 07:43:44.000000 educommon-3.9.3/tests/test_contingent_plugin_utils.py
--rw-r--r--   0 toor      (1000) toor      (1000)    28100 2024-03-18 07:43:44.000000 educommon-3.9.3/tests/test_dates_splitter.py
--rw-r--r--   0 toor      (1000) toor      (1000)     2500 2024-03-18 07:43:44.000000 educommon-3.9.3/tests/test_delete_check.py
--rw-r--r--   0 toor      (1000) toor      (1000)     5018 2024-03-18 07:43:44.000000 educommon-3.9.3/tests/test_delete_objects.py
--rw-r--r--   0 toor      (1000) toor      (1000)     3203 2024-03-18 07:43:44.000000 educommon-3.9.3/tests/test_django_db_utils.py
--rw-r--r--   0 toor      (1000) toor      (1000)    21544 2024-03-18 07:43:44.000000 educommon-3.9.3/tests/test_interval_mixins.py
--rw-r--r--   0 toor      (1000) toor      (1000)     1817 2024-03-18 07:43:44.000000 educommon-3.9.3/tests/test_patches.py
--rw-r--r--   0 toor      (1000) toor      (1000)     7024 2024-03-18 07:43:44.000000 educommon-3.9.3/tests/test_personal_data_fields.py
--rw-r--r--   0 toor      (1000) toor      (1000)    14369 2024-03-18 07:43:44.000000 educommon-3.9.3/tests/test_report.py
--rw-r--r--   0 toor      (1000) toor      (1000)     1688 2024-03-18 07:43:44.000000 educommon-3.9.3/tests/test_service_db_router.py
--rw-r--r--   0 toor      (1000) toor      (1000)     2332 2024-03-18 07:43:44.000000 educommon-3.9.3/tests/test_utils.py
--rw-r--r--   0 toor      (1000) toor      (1000)     2137 2024-03-18 07:43:44.000000 educommon-3.9.3/tests/test_utils_plugins.py
--rw-r--r--   0 toor      (1000) toor      (1000)     9435 2024-03-18 07:43:44.000000 educommon-3.9.3/tests/test_validators.py
--rw-r--r--   0 toor      (1000) toor      (1000)     5881 2024-03-18 07:43:44.000000 educommon-3.9.3/tests/tests_rbac.py
+drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-04-03 06:43:20.586266 educommon-3.9.4/
+-rw-r--r--   0 toor      (1000) toor      (1000)      102 2022-07-05 14:23:59.000000 educommon-3.9.4/MANIFEST.in
+-rw-r--r--   0 toor      (1000) toor      (1000)     1472 2024-04-03 06:43:20.585266 educommon-3.9.4/PKG-INFO
+-rw-r--r--   0 toor      (1000) toor      (1000)     1042 2022-07-05 14:23:59.000000 educommon-3.9.4/README.rst
+-rw-r--r--   0 toor      (1000) toor      (1000)     1981 2022-07-05 14:23:59.000000 educommon-3.9.4/UPGRADE.rst
+-rw-r--r--   0 toor      (1000) toor      (1000)       38 2024-04-03 06:43:20.586266 educommon-3.9.4/setup.cfg
+-rw-r--r--   0 toor      (1000) toor      (1000)     2223 2024-04-03 06:43:15.000000 educommon-3.9.4/setup.py
+drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-04-03 06:43:20.362266 educommon-3.9.4/src/
+drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-04-03 06:43:20.383266 educommon-3.9.4/src/educommon/
+-rw-r--r--   0 toor      (1000) toor      (1000)      419 2024-04-03 06:43:15.000000 educommon-3.9.4/src/educommon/__init__.py
+drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-04-03 06:43:20.388266 educommon-3.9.4/src/educommon/about/
+-rw-r--r--   0 toor      (1000) toor      (1000)     2685 2022-07-05 14:23:59.000000 educommon-3.9.4/src/educommon/about/README.rst
+-rw-r--r--   0 toor      (1000) toor      (1000)      132 2024-04-03 06:43:15.000000 educommon-3.9.4/src/educommon/about/__init__.py
+-rw-r--r--   0 toor      (1000) toor      (1000)      259 2024-04-03 06:43:15.000000 educommon-3.9.4/src/educommon/about/apps.py
+drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-04-03 06:43:20.363266 educommon-3.9.4/src/educommon/about/static/
+drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-04-03 06:43:20.388266 educommon-3.9.4/src/educommon/about/static/edu_about/
+-rw-r--r--   0 toor      (1000) toor      (1000)     8382 2022-07-05 14:23:59.000000 educommon-3.9.4/src/educommon/about/static/edu_about/barsgroup.png
+drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-04-03 06:43:20.397266 educommon-3.9.4/src/educommon/about/ui/
+-rw-r--r--   0 toor      (1000) toor      (1000)        1 2024-04-03 06:43:15.000000 educommon-3.9.4/src/educommon/about/ui/__init__.py
+-rw-r--r--   0 toor      (1000) toor      (1000)      535 2022-07-05 14:23:59.000000 educommon-3.9.4/src/educommon/about/ui/about-window.js
+-rw-r--r--   0 toor      (1000) toor      (1000)     5975 2024-04-03 06:43:15.000000 educommon-3.9.4/src/educommon/about/ui/actions.py
+-rw-r--r--   0 toor      (1000) toor      (1000)      700 2022-07-05 14:23:59.000000 educommon-3.9.4/src/educommon/about/ui/common-tab.html
+-rw-r--r--   0 toor      (1000) toor      (1000)    11192 2022-07-05 14:23:59.000000 educommon-3.9.4/src/educommon/about/ui/packages-tab.js
+-rw-r--r--   0 toor      (1000) toor      (1000)      129 2022-07-05 14:23:59.000000 educommon-3.9.4/src/educommon/about/ui/postgresql-extensions-tab.js
+-rw-r--r--   0 toor      (1000) toor      (1000)     5272 2024-04-03 06:43:15.000000 educommon-3.9.4/src/educommon/about/ui/ui.py
+-rw-r--r--   0 toor      (1000) toor      (1000)      625 2024-04-03 06:43:15.000000 educommon-3.9.4/src/educommon/about/utils.py
+drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-04-03 06:43:20.399266 educommon-3.9.4/src/educommon/async_task/
+-rw-r--r--   0 toor      (1000) toor      (1000)      110 2024-04-03 06:43:15.000000 educommon-3.9.4/src/educommon/async_task/__init__.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     6654 2024-04-03 06:43:15.000000 educommon-3.9.4/src/educommon/async_task/actions.py
+-rw-r--r--   0 toor      (1000) toor      (1000)      143 2024-04-03 06:43:15.000000 educommon-3.9.4/src/educommon/async_task/apps.py
+-rw-r--r--   0 toor      (1000) toor      (1000)      242 2024-04-03 06:43:15.000000 educommon-3.9.4/src/educommon/async_task/consts.py
+-rw-r--r--   0 toor      (1000) toor      (1000)      117 2024-04-03 06:43:15.000000 educommon-3.9.4/src/educommon/async_task/exceptions.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     2706 2024-04-03 06:43:15.000000 educommon-3.9.4/src/educommon/async_task/helpers.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     3844 2024-04-03 06:43:15.000000 educommon-3.9.4/src/educommon/async_task/locker.py
+drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-04-03 06:43:20.401266 educommon-3.9.4/src/educommon/async_task/migrations/
+-rw-r--r--   0 toor      (1000) toor      (1000)     3677 2024-04-03 06:43:15.000000 educommon-3.9.4/src/educommon/async_task/migrations/0001_initial.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     3359 2024-04-03 06:43:15.000000 educommon-3.9.4/src/educommon/async_task/migrations/0002_task_type_and_status_data.py
+-rw-r--r--   0 toor      (1000) toor      (1000)        0 2024-04-03 06:43:15.000000 educommon-3.9.4/src/educommon/async_task/migrations/__init__.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     7430 2024-04-03 06:43:15.000000 educommon-3.9.4/src/educommon/async_task/models.py
+-rw-r--r--   0 toor      (1000) toor      (1000)    11533 2024-04-03 06:43:15.000000 educommon-3.9.4/src/educommon/async_task/tasks.py
+drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-04-03 06:43:20.363266 educommon-3.9.4/src/educommon/async_task/templates/
+drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-04-03 06:43:20.402266 educommon-3.9.4/src/educommon/async_task/templates/ui-js/
+-rw-r--r--   0 toor      (1000) toor      (1000)      749 2024-04-03 06:43:15.000000 educommon-3.9.4/src/educommon/async_task/templates/ui-js/async-task-list-win.js
+-rw-r--r--   0 toor      (1000) toor      (1000)     1257 2024-04-03 06:43:15.000000 educommon-3.9.4/src/educommon/async_task/templates/ui-js/async-task-revoke.js
+-rw-r--r--   0 toor      (1000) toor      (1000)      260 2024-04-03 06:43:15.000000 educommon-3.9.4/src/educommon/async_task/templates/ui-js/async-task-view-win.js
+-rw-r--r--   0 toor      (1000) toor      (1000)     5446 2024-04-03 06:43:15.000000 educommon-3.9.4/src/educommon/async_task/ui.py
+drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-04-03 06:43:20.403266 educommon-3.9.4/src/educommon/async_tasks/
+-rw-r--r--   0 toor      (1000) toor      (1000)      110 2024-04-03 06:43:15.000000 educommon-3.9.4/src/educommon/async_tasks/__init__.py
+-rw-r--r--   0 toor      (1000) toor      (1000)      138 2024-04-03 06:43:15.000000 educommon-3.9.4/src/educommon/async_tasks/apps.py
+-rw-r--r--   0 toor      (1000) toor      (1000)      251 2024-04-03 06:43:15.000000 educommon-3.9.4/src/educommon/async_tasks/exceptions.py
+drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-04-03 06:43:20.404266 educommon-3.9.4/src/educommon/async_tasks/fixtures/
+-rw-r--r--   0 toor      (1000) toor      (1000)      303 2022-07-05 14:23:59.000000 educommon-3.9.4/src/educommon/async_tasks/fixtures/initial_data.json
+-rw-r--r--   0 toor      (1000) toor      (1000)     3489 2024-04-03 06:43:15.000000 educommon-3.9.4/src/educommon/async_tasks/locks.py
+drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-04-03 06:43:20.405266 educommon-3.9.4/src/educommon/async_tasks/migrations/
+-rw-r--r--   0 toor      (1000) toor      (1000)     4205 2024-04-03 06:43:15.000000 educommon-3.9.4/src/educommon/async_tasks/migrations/0001_initial.py
+-rw-r--r--   0 toor      (1000) toor      (1000)      478 2024-04-03 06:43:15.000000 educommon-3.9.4/src/educommon/async_tasks/migrations/0002_load_initial_data.py
+-rw-r--r--   0 toor      (1000) toor      (1000)        0 2024-04-03 06:43:15.000000 educommon-3.9.4/src/educommon/async_tasks/migrations/__init__.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     3539 2024-04-03 06:43:15.000000 educommon-3.9.4/src/educommon/async_tasks/models.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     1413 2024-04-03 06:43:15.000000 educommon-3.9.4/src/educommon/async_tasks/statuses.py
+-rw-r--r--   0 toor      (1000) toor      (1000)    11374 2024-04-03 06:43:15.000000 educommon-3.9.4/src/educommon/async_tasks/tasks.py
+drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-04-03 06:43:20.408266 educommon-3.9.4/src/educommon/audit_log/
+-rw-r--r--   0 toor      (1000) toor      (1000)     2772 2024-04-03 06:43:15.000000 educommon-3.9.4/src/educommon/audit_log/__init__.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     5980 2024-04-03 06:43:15.000000 educommon-3.9.4/src/educommon/audit_log/actions.py
+-rw-r--r--   0 toor      (1000) toor      (1000)      310 2024-04-03 06:43:15.000000 educommon-3.9.4/src/educommon/audit_log/app_meta.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     5033 2024-04-03 06:43:15.000000 educommon-3.9.4/src/educommon/audit_log/apps.py
+-rw-r--r--   0 toor      (1000) toor      (1000)      880 2024-04-03 06:43:15.000000 educommon-3.9.4/src/educommon/audit_log/constants.py
+drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-04-03 06:43:20.409266 educommon-3.9.4/src/educommon/audit_log/error_log/
+-rw-r--r--   0 toor      (1000) toor      (1000)       97 2024-04-03 06:43:15.000000 educommon-3.9.4/src/educommon/audit_log/error_log/__init__.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     2327 2024-04-03 06:43:15.000000 educommon-3.9.4/src/educommon/audit_log/error_log/actions.py
+-rw-r--r--   0 toor      (1000) toor      (1000)      738 2024-04-03 06:43:15.000000 educommon-3.9.4/src/educommon/audit_log/helpers.py
+drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-04-03 06:43:20.409266 educommon-3.9.4/src/educommon/audit_log/management/
+-rw-r--r--   0 toor      (1000) toor      (1000)        0 2024-04-03 06:43:15.000000 educommon-3.9.4/src/educommon/audit_log/management/__init__.py
+drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-04-03 06:43:20.410266 educommon-3.9.4/src/educommon/audit_log/management/commands/
+-rw-r--r--   0 toor      (1000) toor      (1000)        0 2024-04-03 06:43:15.000000 educommon-3.9.4/src/educommon/audit_log/management/commands/__init__.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     2945 2024-04-03 06:43:15.000000 educommon-3.9.4/src/educommon/audit_log/management/commands/reinstall_audit_log.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     1140 2024-04-03 06:43:15.000000 educommon-3.9.4/src/educommon/audit_log/middleware.py
+drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-04-03 06:43:20.412266 educommon-3.9.4/src/educommon/audit_log/migrations/
+-rw-r--r--   0 toor      (1000) toor      (1000)     4461 2024-04-03 06:43:15.000000 educommon-3.9.4/src/educommon/audit_log/migrations/0001_initial.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     2831 2024-04-03 06:43:15.000000 educommon-3.9.4/src/educommon/audit_log/migrations/0002_install_audit_log.py
+-rw-r--r--   0 toor      (1000) toor      (1000)      405 2024-04-03 06:43:15.000000 educommon-3.9.4/src/educommon/audit_log/migrations/0003_logproxy.py
+-rw-r--r--   0 toor      (1000) toor      (1000)      282 2024-04-03 06:43:15.000000 educommon-3.9.4/src/educommon/audit_log/migrations/0004_reinstall_audit_log.py
+-rw-r--r--   0 toor      (1000) toor      (1000)      709 2024-04-03 06:43:15.000000 educommon-3.9.4/src/educommon/audit_log/migrations/0005_postgresql_error.py
+-rw-r--r--   0 toor      (1000) toor      (1000)      611 2024-04-03 06:43:15.000000 educommon-3.9.4/src/educommon/audit_log/migrations/0006_auto_20200806_1707.py
+-rw-r--r--   0 toor      (1000) toor      (1000)      812 2024-04-03 06:43:15.000000 educommon-3.9.4/src/educommon/audit_log/migrations/0007_create_selective_tables_function.py
+-rw-r--r--   0 toor      (1000) toor      (1000)      477 2024-04-03 06:43:15.000000 educommon-3.9.4/src/educommon/audit_log/migrations/0008_table_logged.py
+-rw-r--r--   0 toor      (1000) toor      (1000)      287 2024-04-03 06:43:15.000000 educommon-3.9.4/src/educommon/audit_log/migrations/0009_reinstall_audit_log.py
+-rw-r--r--   0 toor      (1000) toor      (1000)        1 2024-04-03 06:43:15.000000 educommon-3.9.4/src/educommon/audit_log/migrations/__init__.py
+-rw-r--r--   0 toor      (1000) toor      (1000)    11682 2024-04-03 06:43:15.000000 educommon-3.9.4/src/educommon/audit_log/models.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     1241 2024-04-03 06:43:15.000000 educommon-3.9.4/src/educommon/audit_log/permissions.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     8559 2024-04-03 06:43:15.000000 educommon-3.9.4/src/educommon/audit_log/proxies.py
+-rw-r--r--   0 toor      (1000) toor      (1000)      204 2024-04-03 06:43:15.000000 educommon-3.9.4/src/educommon/audit_log/routers.py
+drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-04-03 06:43:20.413266 educommon-3.9.4/src/educommon/audit_log/sql/
+-rw-r--r--   0 toor      (1000) toor      (1000)     1511 2024-04-03 06:43:15.000000 educommon-3.9.4/src/educommon/audit_log/sql/configure_audit_log.sql
+-rw-r--r--   0 toor      (1000) toor      (1000)    14107 2024-04-03 06:43:15.000000 educommon-3.9.4/src/educommon/audit_log/sql/install_audit_log.sql
+-rw-r--r--   0 toor      (1000) toor      (1000)     2117 2024-04-03 06:43:15.000000 educommon-3.9.4/src/educommon/audit_log/ui.py
+drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-04-03 06:43:20.413266 educommon-3.9.4/src/educommon/audit_log/utils/
+-rw-r--r--   0 toor      (1000) toor      (1000)    15603 2024-04-03 06:43:15.000000 educommon-3.9.4/src/educommon/audit_log/utils/__init__.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     1661 2024-04-03 06:43:15.000000 educommon-3.9.4/src/educommon/audit_log/utils/operations.py
+drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-04-03 06:43:20.413266 educommon-3.9.4/src/educommon/auth/
+-rw-r--r--   0 toor      (1000) toor      (1000)      127 2024-04-03 06:43:15.000000 educommon-3.9.4/src/educommon/auth/__init__.py
+drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-04-03 06:43:20.416266 educommon-3.9.4/src/educommon/auth/rbac/
+-rw-r--r--   0 toor      (1000) toor      (1000)      329 2024-04-03 06:43:15.000000 educommon-3.9.4/src/educommon/auth/rbac/__init__.py
+-rw-r--r--   0 toor      (1000) toor      (1000)    26872 2024-04-03 06:43:15.000000 educommon-3.9.4/src/educommon/auth/rbac/actions.py
+-rw-r--r--   0 toor      (1000) toor      (1000)      450 2024-04-03 06:43:15.000000 educommon-3.9.4/src/educommon/auth/rbac/app_meta.py
+drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-04-03 06:43:20.417266 educommon-3.9.4/src/educommon/auth/rbac/backends/
+-rw-r--r--   0 toor      (1000) toor      (1000)        1 2024-04-03 06:43:15.000000 educommon-3.9.4/src/educommon/auth/rbac/backends/__init__.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     2995 2024-04-03 06:43:15.000000 educommon-3.9.4/src/educommon/auth/rbac/backends/base.py
+-rw-r--r--   0 toor      (1000) toor      (1000)    10290 2024-04-03 06:43:15.000000 educommon-3.9.4/src/educommon/auth/rbac/backends/caching.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     5038 2024-04-03 06:43:15.000000 educommon-3.9.4/src/educommon/auth/rbac/backends/simple.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     2957 2024-04-03 06:43:15.000000 educommon-3.9.4/src/educommon/auth/rbac/checker.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     1074 2024-04-03 06:43:15.000000 educommon-3.9.4/src/educommon/auth/rbac/config.py
+-rw-r--r--   0 toor      (1000) toor      (1000)      502 2024-04-03 06:43:15.000000 educommon-3.9.4/src/educommon/auth/rbac/constants.py
+drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-04-03 06:43:20.418266 educommon-3.9.4/src/educommon/auth/rbac/management/
+-rw-r--r--   0 toor      (1000) toor      (1000)       71 2024-04-03 06:43:15.000000 educommon-3.9.4/src/educommon/auth/rbac/management/__init__.py
+drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-04-03 06:43:20.418266 educommon-3.9.4/src/educommon/auth/rbac/management/commands/
+-rw-r--r--   0 toor      (1000) toor      (1000)        1 2024-04-03 06:43:15.000000 educommon-3.9.4/src/educommon/auth/rbac/management/commands/__init__.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     5520 2024-04-03 06:43:15.000000 educommon-3.9.4/src/educommon/auth/rbac/management/commands/rbac.py
+-rw-r--r--   0 toor      (1000) toor      (1000)    16250 2024-04-03 06:43:15.000000 educommon-3.9.4/src/educommon/auth/rbac/manager.py
+drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-04-03 06:43:20.419266 educommon-3.9.4/src/educommon/auth/rbac/migrations/
+-rw-r--r--   0 toor      (1000) toor      (1000)     5474 2024-04-03 06:43:15.000000 educommon-3.9.4/src/educommon/auth/rbac/migrations/0001_initial.py
+-rw-r--r--   0 toor      (1000) toor      (1000)      577 2024-04-03 06:43:15.000000 educommon-3.9.4/src/educommon/auth/rbac/migrations/0002_model_modifier_metaclass_fix.py
+-rw-r--r--   0 toor      (1000) toor      (1000)      470 2024-04-03 06:43:15.000000 educommon-3.9.4/src/educommon/auth/rbac/migrations/0003_permission_hidden.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     2077 2024-04-03 06:43:15.000000 educommon-3.9.4/src/educommon/auth/rbac/migrations/0004_auto_20171024_1245.py
+-rw-r--r--   0 toor      (1000) toor      (1000)        1 2024-04-03 06:43:15.000000 educommon-3.9.4/src/educommon/auth/rbac/migrations/__init__.py
+-rw-r--r--   0 toor      (1000) toor      (1000)    15146 2024-04-03 06:43:15.000000 educommon-3.9.4/src/educommon/auth/rbac/models.py
+-rw-r--r--   0 toor      (1000) toor      (1000)      865 2024-04-03 06:43:15.000000 educommon-3.9.4/src/educommon/auth/rbac/permissions.py
+drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-04-03 06:43:20.366266 educommon-3.9.4/src/educommon/auth/rbac/templates/
+drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-04-03 06:43:20.423266 educommon-3.9.4/src/educommon/auth/rbac/templates/rbac/
+-rw-r--r--   0 toor      (1000) toor      (1000)      335 2022-07-05 14:23:59.000000 educommon-3.9.4/src/educommon/auth/rbac/templates/rbac/role-add-window.js
+-rw-r--r--   0 toor      (1000) toor      (1000)     7914 2022-07-05 14:23:59.000000 educommon-3.9.4/src/educommon/auth/rbac/templates/rbac/role-edit-window.js
+-rw-r--r--   0 toor      (1000) toor      (1000)     3768 2022-07-05 14:23:59.000000 educommon-3.9.4/src/educommon/auth/rbac/templates/rbac/roles-list-window.js
+-rw-r--r--   0 toor      (1000) toor      (1000)      536 2022-07-05 14:23:59.000000 educommon-3.9.4/src/educommon/auth/rbac/templates/rbac/roles-view-list-window.js
+-rw-r--r--   0 toor      (1000) toor      (1000)    15735 2024-04-03 06:43:15.000000 educommon-3.9.4/src/educommon/auth/rbac/ui.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     7819 2024-04-03 06:43:15.000000 educommon-3.9.4/src/educommon/auth/rbac/utils.py
+-rw-r--r--   0 toor      (1000) toor      (1000)      483 2024-04-03 06:43:15.000000 educommon-3.9.4/src/educommon/auth/rbac/validators.py
+drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-04-03 06:43:20.425266 educommon-3.9.4/src/educommon/auth/simple_auth/
+-rw-r--r--   0 toor      (1000) toor      (1000)      267 2024-04-03 06:43:15.000000 educommon-3.9.4/src/educommon/auth/simple_auth/__init__.py
+-rw-r--r--   0 toor      (1000) toor      (1000)    11943 2024-04-03 06:43:15.000000 educommon-3.9.4/src/educommon/auth/simple_auth/actions.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     1088 2024-04-03 06:43:15.000000 educommon-3.9.4/src/educommon/auth/simple_auth/app_meta.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     2522 2024-04-03 06:43:15.000000 educommon-3.9.4/src/educommon/auth/simple_auth/checkers.py
+-rw-r--r--   0 toor      (1000) toor      (1000)      396 2024-04-03 06:43:15.000000 educommon-3.9.4/src/educommon/auth/simple_auth/const.py
+drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-04-03 06:43:20.426266 educommon-3.9.4/src/educommon/auth/simple_auth/migrations/
+-rw-r--r--   0 toor      (1000) toor      (1000)     1396 2024-04-03 06:43:15.000000 educommon-3.9.4/src/educommon/auth/simple_auth/migrations/0001_initial.py
+-rw-r--r--   0 toor      (1000) toor      (1000)        1 2024-04-03 06:43:15.000000 educommon-3.9.4/src/educommon/auth/simple_auth/migrations/__init__.py
+-rw-r--r--   0 toor      (1000) toor      (1000)      700 2024-04-03 06:43:15.000000 educommon-3.9.4/src/educommon/auth/simple_auth/models.py
+drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-04-03 06:43:20.367266 educommon-3.9.4/src/educommon/auth/simple_auth/static/
+drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-04-03 06:43:20.426266 educommon-3.9.4/src/educommon/auth/simple_auth/static/simple_auth/
+-rw-r--r--   0 toor      (1000) toor      (1000)      123 2022-07-05 14:23:59.000000 educommon-3.9.4/src/educommon/auth/simple_auth/static/simple_auth/simple_auth.css
+drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-04-03 06:43:20.367266 educommon-3.9.4/src/educommon/auth/simple_auth/templates/
+drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-04-03 06:43:20.428266 educommon-3.9.4/src/educommon/auth/simple_auth/templates/simple_auth/
+-rw-r--r--   0 toor      (1000) toor      (1000)     1577 2022-07-05 14:23:59.000000 educommon-3.9.4/src/educommon/auth/simple_auth/templates/simple_auth/change_reset_password_page.html
+drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-04-03 06:43:20.429266 educommon-3.9.4/src/educommon/auth/simple_auth/templates/simple_auth/email/
+-rw-r--r--   0 toor      (1000) toor      (1000)      635 2022-07-05 14:23:59.000000 educommon-3.9.4/src/educommon/auth/simple_auth/templates/simple_auth/email/reset_password.html
+-rw-r--r--   0 toor      (1000) toor      (1000)     1444 2022-07-05 14:23:59.000000 educommon-3.9.4/src/educommon/auth/simple_auth/templates/simple_auth/login_page.html
+-rw-r--r--   0 toor      (1000) toor      (1000)     1340 2022-07-05 14:23:59.000000 educommon-3.9.4/src/educommon/auth/simple_auth/templates/simple_auth/reset_password_page.html
+-rw-r--r--   0 toor      (1000) toor      (1000)     4620 2024-04-03 06:43:15.000000 educommon-3.9.4/src/educommon/auth/simple_auth/ui.py
+-rw-r--r--   0 toor      (1000) toor      (1000)      204 2024-04-03 06:43:15.000000 educommon-3.9.4/src/educommon/auth/simple_auth/validators.py
+drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-04-03 06:43:20.433266 educommon-3.9.4/src/educommon/contingent/
+-rw-r--r--   0 toor      (1000) toor      (1000)        0 2024-04-03 06:43:15.000000 educommon-3.9.4/src/educommon/contingent/__init__.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     3035 2024-04-03 06:43:15.000000 educommon-3.9.4/src/educommon/contingent/actions.py
+-rw-r--r--   0 toor      (1000) toor      (1000)      273 2024-04-03 06:43:15.000000 educommon-3.9.4/src/educommon/contingent/app_meta.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     6854 2024-04-03 06:43:15.000000 educommon-3.9.4/src/educommon/contingent/base.py
+-rw-r--r--   0 toor      (1000) toor      (1000)    61449 2024-04-03 06:43:15.000000 educommon-3.9.4/src/educommon/contingent/catalogs.py
+drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-04-03 06:43:20.436266 educommon-3.9.4/src/educommon/contingent/contingent_plugin/
+-rw-r--r--   0 toor      (1000) toor      (1000)        0 2024-04-03 06:43:15.000000 educommon-3.9.4/src/educommon/contingent/contingent_plugin/__init__.py
+-rw-r--r--   0 toor      (1000) toor      (1000)      717 2024-04-03 06:43:15.000000 educommon-3.9.4/src/educommon/contingent/contingent_plugin/actions.py
+-rw-r--r--   0 toor      (1000) toor      (1000)      697 2024-04-03 06:43:15.000000 educommon-3.9.4/src/educommon/contingent/contingent_plugin/apps.py
+drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-04-03 06:43:20.437266 educommon-3.9.4/src/educommon/contingent/contingent_plugin/migrations/
+-rw-r--r--   0 toor      (1000) toor      (1000)     1594 2024-04-03 06:43:15.000000 educommon-3.9.4/src/educommon/contingent/contingent_plugin/migrations/0001_initial.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     1176 2024-04-03 06:43:15.000000 educommon-3.9.4/src/educommon/contingent/contingent_plugin/migrations/0002_add_contingent_model_deleted.py
+-rw-r--r--   0 toor      (1000) toor      (1000)        1 2024-04-03 06:43:15.000000 educommon-3.9.4/src/educommon/contingent/contingent_plugin/migrations/__init__.py
+-rw-r--r--   0 toor      (1000) toor      (1000)      769 2024-04-03 06:43:15.000000 educommon-3.9.4/src/educommon/contingent/contingent_plugin/model_views.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     2506 2024-04-03 06:43:15.000000 educommon-3.9.4/src/educommon/contingent/contingent_plugin/models.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     5181 2024-04-03 06:43:15.000000 educommon-3.9.4/src/educommon/contingent/contingent_plugin/observer.py
+-rw-r--r--   0 toor      (1000) toor      (1000)      148 2024-04-03 06:43:15.000000 educommon-3.9.4/src/educommon/contingent/contingent_plugin/plugin_meta.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     3314 2024-04-03 06:43:15.000000 educommon-3.9.4/src/educommon/contingent/contingent_plugin/storage.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     7161 2024-04-03 06:43:15.000000 educommon-3.9.4/src/educommon/contingent/contingent_plugin/utils.py
+drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-04-03 06:43:20.441266 educommon-3.9.4/src/educommon/contingent/json_data/
+-rw-r--r--   0 toor      (1000) toor      (1000)    20078 2024-04-03 06:43:15.000000 educommon-3.9.4/src/educommon/contingent/json_data/icao.json
+-rw-r--r--   0 toor      (1000) toor      (1000)    53540 2022-07-05 14:23:59.000000 educommon-3.9.4/src/educommon/contingent/json_data/okogu.json
+-rw-r--r--   0 toor      (1000) toor      (1000)    30877 2024-04-03 06:43:15.000000 educommon-3.9.4/src/educommon/contingent/json_data/oksm.json
+drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-04-03 06:43:20.441266 educommon-3.9.4/src/educommon/django/
+-rw-r--r--   0 toor      (1000) toor      (1000)       69 2024-04-03 06:43:15.000000 educommon-3.9.4/src/educommon/django/__init__.py
+drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-04-03 06:43:20.443266 educommon-3.9.4/src/educommon/django/db/
+-rw-r--r--   0 toor      (1000) toor      (1000)       73 2024-04-03 06:43:15.000000 educommon-3.9.4/src/educommon/django/db/__init__.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     7049 2024-04-03 06:43:15.000000 educommon-3.9.4/src/educommon/django/db/fields.py
+drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-04-03 06:43:20.444266 educommon-3.9.4/src/educommon/django/db/migration/
+-rw-r--r--   0 toor      (1000) toor      (1000)     1882 2024-04-03 06:43:15.000000 educommon-3.9.4/src/educommon/django/db/migration/__init__.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     9527 2024-04-03 06:43:15.000000 educommon-3.9.4/src/educommon/django/db/migration/operations.py
+drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-04-03 06:43:20.445266 educommon-3.9.4/src/educommon/django/db/mixins/
+-rw-r--r--   0 toor      (1000) toor      (1000)    14740 2024-04-03 06:43:15.000000 educommon-3.9.4/src/educommon/django/db/mixins/__init__.py
+-rw-r--r--   0 toor      (1000) toor      (1000)    24715 2024-04-03 06:43:15.000000 educommon-3.9.4/src/educommon/django/db/mixins/date_interval.py
+-rw-r--r--   0 toor      (1000) toor      (1000)    12173 2024-04-03 06:43:15.000000 educommon-3.9.4/src/educommon/django/db/mixins/validation.py
+drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-04-03 06:43:20.445266 educommon-3.9.4/src/educommon/django/db/model_view/
+-rw-r--r--   0 toor      (1000) toor      (1000)    12363 2024-04-03 06:43:15.000000 educommon-3.9.4/src/educommon/django/db/model_view/__init__.py
+-rw-r--r--   0 toor      (1000) toor      (1000)      631 2022-07-05 14:23:59.000000 educommon-3.9.4/src/educommon/django/db/model_view/table-view.html
+-rw-r--r--   0 toor      (1000) toor      (1000)     2107 2024-04-03 06:43:15.000000 educommon-3.9.4/src/educommon/django/db/models.py
+-rw-r--r--   0 toor      (1000) toor      (1000)    10990 2024-04-03 06:43:15.000000 educommon-3.9.4/src/educommon/django/db/observer.py
+drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-04-03 06:43:20.450266 educommon-3.9.4/src/educommon/django/db/partitioning/
+-rw-r--r--   0 toor      (1000) toor      (1000)     4455 2022-07-05 14:23:59.000000 educommon-3.9.4/src/educommon/django/db/partitioning/README.md
+-rw-r--r--   0 toor      (1000) toor      (1000)    22376 2024-04-03 06:43:15.000000 educommon-3.9.4/src/educommon/django/db/partitioning/__init__.py
+drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-04-03 06:43:20.451266 educommon-3.9.4/src/educommon/django/db/partitioning/management/
+-rw-r--r--   0 toor      (1000) toor      (1000)        0 2024-04-03 06:43:15.000000 educommon-3.9.4/src/educommon/django/db/partitioning/management/__init__.py
+drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-04-03 06:43:20.453266 educommon-3.9.4/src/educommon/django/db/partitioning/management/commands/
+-rw-r--r--   0 toor      (1000) toor      (1000)        0 2024-04-03 06:43:15.000000 educommon-3.9.4/src/educommon/django/db/partitioning/management/commands/__init__.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     1612 2024-04-03 06:43:15.000000 educommon-3.9.4/src/educommon/django/db/partitioning/management/commands/apply_partitioning.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     2235 2024-04-03 06:43:15.000000 educommon-3.9.4/src/educommon/django/db/partitioning/management/commands/clear_table.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     2082 2024-04-03 06:43:15.000000 educommon-3.9.4/src/educommon/django/db/partitioning/management/commands/split_table.py
+-rw-r--r--   0 toor      (1000) toor      (1000)    20345 2022-07-05 14:23:59.000000 educommon-3.9.4/src/educommon/django/db/partitioning/partitioning.sql
+-rw-r--r--   0 toor      (1000) toor      (1000)     3401 2022-07-05 14:23:59.000000 educommon-3.9.4/src/educommon/django/db/partitioning/triggers.sql
+-rw-r--r--   0 toor      (1000) toor      (1000)     3268 2024-04-03 06:43:15.000000 educommon-3.9.4/src/educommon/django/db/routers.py
+-rw-r--r--   0 toor      (1000) toor      (1000)      136 2024-04-03 06:43:15.000000 educommon-3.9.4/src/educommon/django/db/signals.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     9206 2024-04-03 06:43:15.000000 educommon-3.9.4/src/educommon/django/db/utils.py
+drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-04-03 06:43:20.454266 educommon-3.9.4/src/educommon/django/db/validators/
+-rw-r--r--   0 toor      (1000) toor      (1000)     1986 2024-04-03 06:43:15.000000 educommon-3.9.4/src/educommon/django/db/validators/__init__.py
+-rw-r--r--   0 toor      (1000) toor      (1000)    38886 2024-04-03 06:43:15.000000 educommon-3.9.4/src/educommon/django/db/validators/simple.py
+drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-04-03 06:43:20.454266 educommon-3.9.4/src/educommon/django/storages/
+-rw-r--r--   0 toor      (1000) toor      (1000)        0 2024-04-03 06:43:15.000000 educommon-3.9.4/src/educommon/django/storages/__init__.py
+drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-04-03 06:43:20.459266 educommon-3.9.4/src/educommon/django/storages/atcfs/
+-rw-r--r--   0 toor      (1000) toor      (1000)     2656 2022-07-05 14:23:59.000000 educommon-3.9.4/src/educommon/django/storages/atcfs/README.rst
+-rw-r--r--   0 toor      (1000) toor      (1000)        0 2024-04-03 06:43:15.000000 educommon-3.9.4/src/educommon/django/storages/atcfs/__init__.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     6004 2024-04-03 06:43:15.000000 educommon-3.9.4/src/educommon/django/storages/atcfs/api.py
+-rw-r--r--   0 toor      (1000) toor      (1000)      352 2024-04-03 06:43:15.000000 educommon-3.9.4/src/educommon/django/storages/atcfs/app_meta.py
+-rw-r--r--   0 toor      (1000) toor      (1000)      106 2024-04-03 06:43:15.000000 educommon-3.9.4/src/educommon/django/storages/atcfs/exceptions.py
+drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-04-03 06:43:20.459266 educommon-3.9.4/src/educommon/django/storages/atcfs/management/
+-rw-r--r--   0 toor      (1000) toor      (1000)        0 2024-04-03 06:43:15.000000 educommon-3.9.4/src/educommon/django/storages/atcfs/management/__init__.py
+drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-04-03 06:43:20.460266 educommon-3.9.4/src/educommon/django/storages/atcfs/management/commands/
+-rw-r--r--   0 toor      (1000) toor      (1000)        0 2024-04-03 06:43:15.000000 educommon-3.9.4/src/educommon/django/storages/atcfs/management/commands/__init__.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     7416 2024-04-03 06:43:15.000000 educommon-3.9.4/src/educommon/django/storages/atcfs/management/commands/atcfs_migrate.py
+-rw-r--r--   0 toor      (1000) toor      (1000)      160 2024-04-03 06:43:15.000000 educommon-3.9.4/src/educommon/django/storages/atcfs/models.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     2623 2024-04-03 06:43:15.000000 educommon-3.9.4/src/educommon/django/storages/atcfs/monkey_patching.py
+-rw-r--r--   0 toor      (1000) toor      (1000)      808 2024-04-03 06:43:15.000000 educommon-3.9.4/src/educommon/django/storages/atcfs/settings.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     4180 2024-04-03 06:43:15.000000 educommon-3.9.4/src/educommon/django/storages/atcfs/storage.py
+drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-04-03 06:43:20.460266 educommon-3.9.4/src/educommon/django/storages/atcfs/templates/
+-rw-r--r--   0 toor      (1000) toor      (1000)      196 2022-07-05 14:23:59.000000 educommon-3.9.4/src/educommon/django/storages/atcfs/templates/atcfs_unavailable.html
+drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-04-03 06:43:20.461266 educommon-3.9.4/src/educommon/extjs/
+-rw-r--r--   0 toor      (1000) toor      (1000)       87 2024-04-03 06:43:15.000000 educommon-3.9.4/src/educommon/extjs/__init__.py
+drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-04-03 06:43:20.462266 educommon-3.9.4/src/educommon/extjs/fields/
+-rw-r--r--   0 toor      (1000) toor      (1000)      110 2024-04-03 06:43:15.000000 educommon-3.9.4/src/educommon/extjs/fields/__init__.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     4099 2024-04-03 06:43:15.000000 educommon-3.9.4/src/educommon/extjs/fields/input_params.py
+drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-04-03 06:43:20.471266 educommon-3.9.4/src/educommon/importer/
+-rw-r--r--   0 toor      (1000) toor      (1000)    37531 2024-04-03 06:43:15.000000 educommon-3.9.4/src/educommon/importer/XLSReader.py
+-rw-r--r--   0 toor      (1000) toor      (1000)      147 2024-04-03 06:43:15.000000 educommon-3.9.4/src/educommon/importer/__init__.py
+-rw-r--r--   0 toor      (1000) toor      (1000)    13402 2024-04-03 06:43:15.000000 educommon-3.9.4/src/educommon/importer/api.py
+-rw-r--r--   0 toor      (1000) toor      (1000)      733 2024-04-03 06:43:15.000000 educommon-3.9.4/src/educommon/importer/constants.py
+-rw-r--r--   0 toor      (1000) toor      (1000)    10270 2024-04-03 06:43:15.000000 educommon-3.9.4/src/educommon/importer/loggers.py
+-rw-r--r--   0 toor      (1000) toor      (1000)    37353 2024-04-03 06:43:15.000000 educommon-3.9.4/src/educommon/importer/proxy.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     6244 2024-04-03 06:43:15.000000 educommon-3.9.4/src/educommon/importer/proxy_import.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     2087 2022-07-05 14:23:59.000000 educommon-3.9.4/src/educommon/importer/refactoring-notes.txt
+-rw-r--r--   0 toor      (1000) toor      (1000)     1506 2024-04-03 06:43:15.000000 educommon-3.9.4/src/educommon/importer/report.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     8704 2022-07-05 14:23:59.000000 educommon-3.9.4/src/educommon/importer/test_file.xls
+-rw-r--r--   0 toor      (1000) toor      (1000)     3918 2024-04-03 06:43:15.000000 educommon-3.9.4/src/educommon/importer/ui.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     1182 2024-04-03 06:43:15.000000 educommon-3.9.4/src/educommon/importer/validators.py
+drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-04-03 06:43:20.473266 educommon-3.9.4/src/educommon/integration_entities/
+-rw-r--r--   0 toor      (1000) toor      (1000)      158 2024-04-03 06:43:15.000000 educommon-3.9.4/src/educommon/integration_entities/README.rst
+-rw-r--r--   0 toor      (1000) toor      (1000)        0 2024-04-03 06:43:15.000000 educommon-3.9.4/src/educommon/integration_entities/__init__.py
+-rw-r--r--   0 toor      (1000) toor      (1000)      448 2024-04-03 06:43:15.000000 educommon-3.9.4/src/educommon/integration_entities/consts.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     2005 2024-04-03 06:43:15.000000 educommon-3.9.4/src/educommon/integration_entities/entities.py
+-rw-r--r--   0 toor      (1000) toor      (1000)      335 2024-04-03 06:43:15.000000 educommon-3.9.4/src/educommon/integration_entities/enums.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     9888 2024-04-03 06:43:15.000000 educommon-3.9.4/src/educommon/integration_entities/helpers.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     1115 2024-04-03 06:43:15.000000 educommon-3.9.4/src/educommon/integration_entities/mixins.py
+drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-04-03 06:43:20.473266 educommon-3.9.4/src/educommon/ioc/
+-rw-r--r--   0 toor      (1000) toor      (1000)     4028 2024-04-03 06:43:15.000000 educommon-3.9.4/src/educommon/ioc/__init__.py
+drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-04-03 06:43:20.476266 educommon-3.9.4/src/educommon/logger/
+-rw-r--r--   0 toor      (1000) toor      (1000)      822 2024-04-03 06:43:15.000000 educommon-3.9.4/src/educommon/logger/__init__.py
+-rw-r--r--   0 toor      (1000) toor      (1000)        0 2024-04-03 06:43:15.000000 educommon-3.9.4/src/educommon/logger/app_settings.py
+-rw-r--r--   0 toor      (1000) toor      (1000)      944 2024-04-03 06:43:15.000000 educommon-3.9.4/src/educommon/logger/apps.py
+-rw-r--r--   0 toor      (1000) toor      (1000)      238 2024-04-03 06:43:15.000000 educommon-3.9.4/src/educommon/logger/consts.py
+-rw-r--r--   0 toor      (1000) toor      (1000)      400 2024-04-03 06:43:15.000000 educommon-3.9.4/src/educommon/logger/formatters.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     1596 2024-04-03 06:43:15.000000 educommon-3.9.4/src/educommon/logger/helpers.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     2965 2024-04-03 06:43:15.000000 educommon-3.9.4/src/educommon/logger/loggers.py
+-rw-r--r--   0 toor      (1000) toor      (1000)      138 2024-04-03 06:43:15.000000 educommon-3.9.4/src/educommon/logger/records.py
+drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-04-03 06:43:20.477266 educommon-3.9.4/src/educommon/m3/
+-rw-r--r--   0 toor      (1000) toor      (1000)    17568 2024-04-03 06:43:15.000000 educommon-3.9.4/src/educommon/m3/__init__.py
+drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-04-03 06:43:20.477266 educommon-3.9.4/src/educommon/m3/extensions/
+-rw-r--r--   0 toor      (1000) toor      (1000)      258 2024-04-03 06:43:15.000000 educommon-3.9.4/src/educommon/m3/extensions/__init__.py
+drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-04-03 06:43:20.478266 educommon-3.9.4/src/educommon/m3/extensions/listeners/
+-rw-r--r--   0 toor      (1000) toor      (1000)     8897 2024-04-03 06:43:15.000000 educommon-3.9.4/src/educommon/m3/extensions/listeners/__init__.py
+drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-04-03 06:43:20.481266 educommon-3.9.4/src/educommon/m3/extensions/listeners/delete_check/
+-rw-r--r--   0 toor      (1000) toor      (1000)        0 2024-04-03 06:43:15.000000 educommon-3.9.4/src/educommon/m3/extensions/listeners/delete_check/__init__.py
+-rw-r--r--   0 toor      (1000) toor      (1000)      916 2022-07-05 14:23:59.000000 educommon-3.9.4/src/educommon/m3/extensions/listeners/delete_check/cancel-confirm-window.js
+-rw-r--r--   0 toor      (1000) toor      (1000)     6131 2024-04-03 06:43:15.000000 educommon-3.9.4/src/educommon/m3/extensions/listeners/delete_check/listeners.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     7660 2024-04-03 06:43:15.000000 educommon-3.9.4/src/educommon/m3/extensions/listeners/delete_check/mixins.py
+-rw-r--r--   0 toor      (1000) toor      (1000)       94 2022-07-05 14:23:59.000000 educommon-3.9.4/src/educommon/m3/extensions/listeners/delete_check/related-objects-window.html
+-rw-r--r--   0 toor      (1000) toor      (1000)      467 2024-04-03 06:43:15.000000 educommon-3.9.4/src/educommon/m3/extensions/listeners/delete_check/signals.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     3507 2024-04-03 06:43:15.000000 educommon-3.9.4/src/educommon/m3/extensions/listeners/delete_check/ui.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     2979 2024-04-03 06:43:15.000000 educommon-3.9.4/src/educommon/m3/extensions/listeners/delete_check/utils.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     6912 2024-04-03 06:43:15.000000 educommon-3.9.4/src/educommon/m3/extensions/ui.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     5150 2024-04-03 06:43:15.000000 educommon-3.9.4/src/educommon/m3/transaction_context.py
+drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-04-03 06:43:20.482266 educommon-3.9.4/src/educommon/objectpack/
+-rw-r--r--   0 toor      (1000) toor      (1000)       69 2024-04-03 06:43:15.000000 educommon-3.9.4/src/educommon/objectpack/__init__.py
+-rw-r--r--   0 toor      (1000) toor      (1000)    14735 2024-04-03 06:43:15.000000 educommon-3.9.4/src/educommon/objectpack/actions.py
+-rw-r--r--   0 toor      (1000) toor      (1000)      220 2024-04-03 06:43:15.000000 educommon-3.9.4/src/educommon/objectpack/apps.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     5166 2024-04-03 06:43:15.000000 educommon-3.9.4/src/educommon/objectpack/filters.py
+drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-04-03 06:43:20.490266 educommon-3.9.4/src/educommon/objectpack/templates/
+-rw-r--r--   0 toor      (1000) toor      (1000)      437 2022-07-05 14:23:59.000000 educommon-3.9.4/src/educommon/objectpack/templates/base-grid-window.js
+-rw-r--r--   0 toor      (1000) toor      (1000)     1408 2022-07-05 14:23:59.000000 educommon-3.9.4/src/educommon/objectpack/templates/filter-panel.js
+-rw-r--r--   0 toor      (1000) toor      (1000)     1544 2022-07-05 14:23:59.000000 educommon-3.9.4/src/educommon/objectpack/templates/grid-panel.js
+-rw-r--r--   0 toor      (1000) toor      (1000)     1842 2022-07-05 14:23:59.000000 educommon-3.9.4/src/educommon/objectpack/templates/multiSelectWindow.js
+-rw-r--r--   0 toor      (1000) toor      (1000)     6741 2022-07-05 14:23:59.000000 educommon-3.9.4/src/educommon/objectpack/templates/multiselect-page-fix.js
+-rw-r--r--   0 toor      (1000) toor      (1000)     1838 2022-07-05 14:23:59.000000 educommon-3.9.4/src/educommon/objectpack/templates/relations-check-mixin-template.html
+-rw-r--r--   0 toor      (1000) toor      (1000)    14752 2024-04-03 06:43:15.000000 educommon-3.9.4/src/educommon/objectpack/ui.py
+drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-04-03 06:43:20.492266 educommon-3.9.4/src/educommon/report/
+-rw-r--r--   0 toor      (1000) toor      (1000)    17854 2024-04-03 06:43:15.000000 educommon-3.9.4/src/educommon/report/__init__.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     8705 2024-04-03 06:43:15.000000 educommon-3.9.4/src/educommon/report/actions.py
+drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-04-03 06:43:20.496266 educommon-3.9.4/src/educommon/report/constructor/
+-rw-r--r--   0 toor      (1000) toor      (1000)     1138 2022-07-05 14:23:59.000000 educommon-3.9.4/src/educommon/report/constructor/README.rst
+-rw-r--r--   0 toor      (1000) toor      (1000)     1252 2024-04-03 06:43:15.000000 educommon-3.9.4/src/educommon/report/constructor/__init__.py
+-rw-r--r--   0 toor      (1000) toor      (1000)      200 2024-04-03 06:43:15.000000 educommon-3.9.4/src/educommon/report/constructor/app_meta.py
+-rw-r--r--   0 toor      (1000) toor      (1000)      371 2024-04-03 06:43:15.000000 educommon-3.9.4/src/educommon/report/constructor/apps.py
+-rw-r--r--   0 toor      (1000) toor      (1000)    27289 2024-04-03 06:43:15.000000 educommon-3.9.4/src/educommon/report/constructor/base.py
+drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-04-03 06:43:20.497266 educommon-3.9.4/src/educommon/report/constructor/builders/
+-rw-r--r--   0 toor      (1000) toor      (1000)        1 2024-04-03 06:43:15.000000 educommon-3.9.4/src/educommon/report/constructor/builders/__init__.py
+drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-04-03 06:43:20.498266 educommon-3.9.4/src/educommon/report/constructor/builders/excel/
+-rw-r--r--   0 toor      (1000) toor      (1000)      104 2024-04-03 06:43:15.000000 educommon-3.9.4/src/educommon/report/constructor/builders/excel/__init__.py
+-rw-r--r--   0 toor      (1000) toor      (1000)    55789 2024-04-03 06:43:15.000000 educommon-3.9.4/src/educommon/report/constructor/builders/excel/_base.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     4758 2024-04-03 06:43:15.000000 educommon-3.9.4/src/educommon/report/constructor/builders/excel/_header.py
+-rw-r--r--   0 toor      (1000) toor      (1000)       28 2024-04-03 06:43:15.000000 educommon-3.9.4/src/educommon/report/constructor/builders/excel/constants.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     6229 2024-04-03 06:43:15.000000 educommon-3.9.4/src/educommon/report/constructor/builders/excel/product.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     5150 2024-04-03 06:43:15.000000 educommon-3.9.4/src/educommon/report/constructor/builders/excel/with_merged_cells.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     1058 2024-04-03 06:43:15.000000 educommon-3.9.4/src/educommon/report/constructor/config.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     3381 2024-04-03 06:43:15.000000 educommon-3.9.4/src/educommon/report/constructor/constants.py
+drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-04-03 06:43:20.502266 educommon-3.9.4/src/educommon/report/constructor/editor/
+-rw-r--r--   0 toor      (1000) toor      (1000)       41 2024-04-03 06:43:15.000000 educommon-3.9.4/src/educommon/report/constructor/editor/__init__.py
+-rw-r--r--   0 toor      (1000) toor      (1000)    38810 2024-04-03 06:43:15.000000 educommon-3.9.4/src/educommon/report/constructor/editor/actions.py
+-rw-r--r--   0 toor      (1000) toor      (1000)    39225 2022-07-05 14:23:59.000000 educommon-3.9.4/src/educommon/report/constructor/editor/edit-window.js
+-rw-r--r--   0 toor      (1000) toor      (1000)     3247 2022-07-05 14:23:59.000000 educommon-3.9.4/src/educommon/report/constructor/editor/list-window.js
+-rw-r--r--   0 toor      (1000) toor      (1000)    24628 2024-04-03 06:43:15.000000 educommon-3.9.4/src/educommon/report/constructor/editor/ui.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     1287 2024-04-03 06:43:15.000000 educommon-3.9.4/src/educommon/report/constructor/exceptions.py
+drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-04-03 06:43:20.505266 educommon-3.9.4/src/educommon/report/constructor/migrations/
+-rw-r--r--   0 toor      (1000) toor      (1000)     3393 2024-04-03 06:43:15.000000 educommon-3.9.4/src/educommon/report/constructor/migrations/0001_initial.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     5009 2024-04-03 06:43:15.000000 educommon-3.9.4/src/educommon/report/constructor/migrations/0002_report_filters.py
+-rw-r--r--   0 toor      (1000) toor      (1000)      472 2024-04-03 06:43:15.000000 educommon-3.9.4/src/educommon/report/constructor/migrations/0003_reportfilter_exclude.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     1369 2024-04-03 06:43:15.000000 educommon-3.9.4/src/educommon/report/constructor/migrations/0004_reportfilter_fields.py
+-rw-r--r--   0 toor      (1000) toor      (1000)      431 2024-04-03 06:43:15.000000 educommon-3.9.4/src/educommon/report/constructor/migrations/0005_reportcolumn_visible.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     1284 2024-04-03 06:43:15.000000 educommon-3.9.4/src/educommon/report/constructor/migrations/0006_reportsorting.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     1541 2024-04-03 06:43:15.000000 educommon-3.9.4/src/educommon/report/constructor/migrations/0007_include_available_units.py
+-rw-r--r--   0 toor      (1000) toor      (1000)      557 2024-04-03 06:43:15.000000 educommon-3.9.4/src/educommon/report/constructor/migrations/0008_auto_20170407_1318.py
+-rw-r--r--   0 toor      (1000) toor      (1000)      519 2024-04-03 06:43:15.000000 educommon-3.9.4/src/educommon/report/constructor/migrations/0009_auto_20180405_0642.py
+-rw-r--r--   0 toor      (1000) toor      (1000)      949 2024-04-03 06:43:15.000000 educommon-3.9.4/src/educommon/report/constructor/migrations/0010_add_aggregate_fields.py
+-rw-r--r--   0 toor      (1000) toor      (1000)        1 2024-04-03 06:43:15.000000 educommon-3.9.4/src/educommon/report/constructor/migrations/__init__.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     2377 2024-04-03 06:43:15.000000 educommon-3.9.4/src/educommon/report/constructor/mixins.py
+-rw-r--r--   0 toor      (1000) toor      (1000)    18764 2024-04-03 06:43:15.000000 educommon-3.9.4/src/educommon/report/constructor/models.py
+-rw-r--r--   0 toor      (1000) toor      (1000)      114 2024-04-03 06:43:15.000000 educommon-3.9.4/src/educommon/report/constructor/plugin_meta.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     1883 2024-04-03 06:43:15.000000 educommon-3.9.4/src/educommon/report/constructor/registries.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     6557 2024-04-03 06:43:15.000000 educommon-3.9.4/src/educommon/report/constructor/utils.py
+-rw-r--r--   0 toor      (1000) toor      (1000)      524 2024-04-03 06:43:15.000000 educommon-3.9.4/src/educommon/report/constructor/validators.py
+-rw-r--r--   0 toor      (1000) toor      (1000)    10026 2024-04-03 06:43:15.000000 educommon-3.9.4/src/educommon/report/reporter.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     9974 2024-04-03 06:43:15.000000 educommon-3.9.4/src/educommon/report/utils.py
+drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-04-03 06:43:20.507266 educommon-3.9.4/src/educommon/rest/
+-rw-r--r--   0 toor      (1000) toor      (1000)        1 2024-04-03 06:43:15.000000 educommon-3.9.4/src/educommon/rest/__init__.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     1278 2024-04-03 06:43:15.000000 educommon-3.9.4/src/educommon/rest/actions.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     3908 2024-04-03 06:43:15.000000 educommon-3.9.4/src/educommon/rest/context.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     2516 2024-04-03 06:43:15.000000 educommon-3.9.4/src/educommon/rest/controllers.py
+-rw-r--r--   0 toor      (1000) toor      (1000)      475 2024-04-03 06:43:15.000000 educommon-3.9.4/src/educommon/rest/misc.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     4840 2024-04-03 06:43:15.000000 educommon-3.9.4/src/educommon/rest/mixins.py
+drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-04-03 06:43:20.511266 educommon-3.9.4/src/educommon/secure_media/
+-rw-r--r--   0 toor      (1000) toor      (1000)     4001 2022-07-05 14:23:59.000000 educommon-3.9.4/src/educommon/secure_media/README.rst
+-rw-r--r--   0 toor      (1000) toor      (1000)        0 2024-04-03 06:43:15.000000 educommon-3.9.4/src/educommon/secure_media/__init__.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     1317 2024-04-03 06:43:15.000000 educommon-3.9.4/src/educommon/secure_media/app_meta.py
+-rw-r--r--   0 toor      (1000) toor      (1000)       61 2024-04-03 06:43:15.000000 educommon-3.9.4/src/educommon/thread_data.py
+drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-04-03 06:43:20.515266 educommon-3.9.4/src/educommon/utils/
+-rw-r--r--   0 toor      (1000) toor      (1000)     2441 2024-04-03 06:43:15.000000 educommon-3.9.4/src/educommon/utils/__init__.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     4063 2024-04-03 06:43:15.000000 educommon-3.9.4/src/educommon/utils/caching.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     1966 2024-04-03 06:43:15.000000 educommon-3.9.4/src/educommon/utils/conversion.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     2158 2024-04-03 06:43:15.000000 educommon-3.9.4/src/educommon/utils/crypto.py
+-rw-r--r--   0 toor      (1000) toor      (1000)    16800 2024-04-03 06:43:15.000000 educommon-3.9.4/src/educommon/utils/date.py
+drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-04-03 06:43:20.516266 educommon-3.9.4/src/educommon/utils/db/
+-rw-r--r--   0 toor      (1000) toor      (1000)     7734 2024-04-03 06:43:15.000000 educommon-3.9.4/src/educommon/utils/db/__init__.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     2820 2024-04-03 06:43:15.000000 educommon-3.9.4/src/educommon/utils/db/postgresql.py
+drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-04-03 06:43:20.535266 educommon-3.9.4/src/educommon/utils/fonts/
+-rw-r--r--   0 toor      (1000) toor      (1000)   275572 2022-07-05 14:23:59.000000 educommon-3.9.4/src/educommon/utils/fonts/Arial.ttf
+-rw-r--r--   0 toor      (1000) toor      (1000)   811820 2022-07-05 14:23:59.000000 educommon-3.9.4/src/educommon/utils/fonts/Calibri.ttf
+-rw-r--r--   0 toor      (1000) toor      (1000)   265528 2022-07-05 14:23:59.000000 educommon-3.9.4/src/educommon/utils/fonts/Tahoma.ttf
+-rw-r--r--   0 toor      (1000) toor      (1000)     4815 2024-04-03 06:43:15.000000 educommon-3.9.4/src/educommon/utils/fonts/__init__.py
+drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-04-03 06:43:20.537266 educommon-3.9.4/src/educommon/utils/licence/
+-rw-r--r--   0 toor      (1000) toor      (1000)     5095 2024-04-03 06:43:15.000000 educommon-3.9.4/src/educommon/utils/licence/__init__.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     1174 2024-04-03 06:43:15.000000 educommon-3.9.4/src/educommon/utils/licence/converters.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     4254 2024-04-03 06:43:15.000000 educommon-3.9.4/src/educommon/utils/misc.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     9048 2024-04-03 06:43:15.000000 educommon-3.9.4/src/educommon/utils/object_grid.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     1157 2024-04-03 06:43:15.000000 educommon-3.9.4/src/educommon/utils/patches.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     9469 2024-04-03 06:43:15.000000 educommon-3.9.4/src/educommon/utils/plugins.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     1995 2024-04-03 06:43:15.000000 educommon-3.9.4/src/educommon/utils/registry.py
+-rw-r--r--   0 toor      (1000) toor      (1000)      520 2024-04-03 06:43:15.000000 educommon-3.9.4/src/educommon/utils/seqtools.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     8787 2024-04-03 06:43:15.000000 educommon-3.9.4/src/educommon/utils/serializer.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     2883 2024-04-03 06:43:15.000000 educommon-3.9.4/src/educommon/utils/storage.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     2834 2024-04-03 06:43:15.000000 educommon-3.9.4/src/educommon/utils/system.py
+drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-04-03 06:43:20.538266 educommon-3.9.4/src/educommon/utils/system_app/
+-rw-r--r--   0 toor      (1000) toor      (1000)        0 2024-04-03 06:43:15.000000 educommon-3.9.4/src/educommon/utils/system_app/__init__.py
+drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-04-03 06:43:20.539266 educommon-3.9.4/src/educommon/utils/system_app/management/
+-rw-r--r--   0 toor      (1000) toor      (1000)        0 2024-04-03 06:43:15.000000 educommon-3.9.4/src/educommon/utils/system_app/management/__init__.py
+drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-04-03 06:43:20.540266 educommon-3.9.4/src/educommon/utils/system_app/management/commands/
+-rw-r--r--   0 toor      (1000) toor      (1000)        0 2024-04-03 06:43:15.000000 educommon-3.9.4/src/educommon/utils/system_app/management/commands/__init__.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     9295 2024-04-03 06:43:15.000000 educommon-3.9.4/src/educommon/utils/system_app/management/commands/delete_objects.py
+drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-04-03 06:43:20.542266 educommon-3.9.4/src/educommon/utils/system_app/templatetags/
+-rw-r--r--   0 toor      (1000) toor      (1000)        1 2024-04-03 06:43:15.000000 educommon-3.9.4/src/educommon/utils/system_app/templatetags/__init__.py
+-rw-r--r--   0 toor      (1000) toor      (1000)      273 2024-04-03 06:43:15.000000 educommon-3.9.4/src/educommon/utils/system_app/templatetags/educommon.py
+-rw-r--r--   0 toor      (1000) toor      (1000)    16082 2024-04-03 06:43:15.000000 educommon-3.9.4/src/educommon/utils/ui.py
+drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-04-03 06:43:20.551266 educommon-3.9.4/src/educommon/utils/xml/
+-rw-r--r--   0 toor      (1000) toor      (1000)     2194 2024-04-03 06:43:15.000000 educommon-3.9.4/src/educommon/utils/xml/__init__.py
+-rw-r--r--   0 toor      (1000) toor      (1000)      875 2022-07-05 14:23:59.000000 educommon-3.9.4/src/educommon/utils/xml/catalog.json
+-rw-r--r--   0 toor      (1000) toor      (1000)     1750 2024-04-03 06:43:15.000000 educommon-3.9.4/src/educommon/utils/xml/resolver.py
+-rw-r--r--   0 toor      (1000) toor      (1000)    13160 2022-07-05 14:23:59.000000 educommon-3.9.4/src/educommon/utils/xml/saml-schema-assertion-2.0.xsd
+-rw-r--r--   0 toor      (1000) toor      (1000)    13465 2022-07-05 14:23:59.000000 educommon-3.9.4/src/educommon/utils/xml/saml-schema-protocol-2.0.xsd
+-rw-r--r--   0 toor      (1000) toor      (1000)     5234 2022-07-05 14:23:59.000000 educommon-3.9.4/src/educommon/utils/xml/xenc-schema.xsd
+-rw-r--r--   0 toor      (1000) toor      (1000)    10293 2022-07-05 14:23:59.000000 educommon-3.9.4/src/educommon/utils/xml/xmldsig-core-schema.xsd
+-rw-r--r--   0 toor      (1000) toor      (1000)      450 2024-04-03 06:43:20.000000 educommon-3.9.4/src/educommon/version.conf
+drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-04-03 06:43:20.558266 educommon-3.9.4/src/educommon/ws_log/
+-rw-r--r--   0 toor      (1000) toor      (1000)     5467 2022-07-05 14:23:59.000000 educommon-3.9.4/src/educommon/ws_log/README.rst
+-rw-r--r--   0 toor      (1000) toor      (1000)      932 2024-04-03 06:43:15.000000 educommon-3.9.4/src/educommon/ws_log/__init__.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     9153 2024-04-03 06:43:15.000000 educommon-3.9.4/src/educommon/ws_log/actions.py
+-rw-r--r--   0 toor      (1000) toor      (1000)       94 2024-04-03 06:43:15.000000 educommon-3.9.4/src/educommon/ws_log/app_meta.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     7138 2024-04-03 06:43:15.000000 educommon-3.9.4/src/educommon/ws_log/base.py
+drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-04-03 06:43:20.563266 educommon-3.9.4/src/educommon/ws_log/migrations/
+-rw-r--r--   0 toor      (1000) toor      (1000)     2706 2024-04-03 06:43:15.000000 educommon-3.9.4/src/educommon/ws_log/migrations/0001_initial.py
+-rw-r--r--   0 toor      (1000) toor      (1000)      910 2024-04-03 06:43:15.000000 educommon-3.9.4/src/educommon/ws_log/migrations/0002_auto_20160628_1334.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     1682 2024-04-03 06:43:15.000000 educommon-3.9.4/src/educommon/ws_log/migrations/0003_add_fields_to_smev_logs.py
+-rw-r--r--   0 toor      (1000) toor      (1000)      932 2024-04-03 06:43:15.000000 educommon-3.9.4/src/educommon/ws_log/migrations/0004_auto_20160727_1600.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     1586 2024-04-03 06:43:15.000000 educommon-3.9.4/src/educommon/ws_log/migrations/0005_auto_20161130_1615.py
+-rw-r--r--   0 toor      (1000) toor      (1000)      479 2024-04-03 06:43:15.000000 educommon-3.9.4/src/educommon/ws_log/migrations/0006_auto_20170327_1027.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     1171 2024-04-03 06:43:15.000000 educommon-3.9.4/src/educommon/ws_log/migrations/0007_auto_20180607_1040.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     1311 2024-04-03 06:43:15.000000 educommon-3.9.4/src/educommon/ws_log/migrations/0008_auto_20180713_1445.py
+-rw-r--r--   0 toor      (1000) toor      (1000)      516 2024-04-03 06:43:15.000000 educommon-3.9.4/src/educommon/ws_log/migrations/0009_auto_20201130_1553.py
+-rw-r--r--   0 toor      (1000) toor      (1000)        1 2024-04-03 06:43:15.000000 educommon-3.9.4/src/educommon/ws_log/migrations/__init__.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     5634 2024-04-03 06:43:15.000000 educommon-3.9.4/src/educommon/ws_log/models.py
+-rw-r--r--   0 toor      (1000) toor      (1000)      885 2024-04-03 06:43:15.000000 educommon-3.9.4/src/educommon/ws_log/provider.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     3487 2024-04-03 06:43:15.000000 educommon-3.9.4/src/educommon/ws_log/report.py
+drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-04-03 06:43:20.565266 educommon-3.9.4/src/educommon/ws_log/smev/
+-rw-r--r--   0 toor      (1000) toor      (1000)       84 2024-04-03 06:43:15.000000 educommon-3.9.4/src/educommon/ws_log/smev/__init__.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     5866 2024-04-03 06:43:15.000000 educommon-3.9.4/src/educommon/ws_log/smev/applications.py
+-rw-r--r--   0 toor      (1000) toor      (1000)      601 2024-04-03 06:43:15.000000 educommon-3.9.4/src/educommon/ws_log/smev/exceptions.py
+drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-04-03 06:43:20.378266 educommon-3.9.4/src/educommon/ws_log/templates/
+drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-04-03 06:43:20.565266 educommon-3.9.4/src/educommon/ws_log/templates/report/
+-rw-r--r--   0 toor      (1000) toor      (1000)    10439 2022-07-05 14:23:59.000000 educommon-3.9.4/src/educommon/ws_log/templates/report/smev_logs.xlsx
+drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-04-03 06:43:20.568266 educommon-3.9.4/src/educommon/ws_log/templates/ui-js/
+-rw-r--r--   0 toor      (1000) toor      (1000)      513 2022-07-05 14:23:59.000000 educommon-3.9.4/src/educommon/ws_log/templates/ui-js/smev-logs-list-window.js
+-rw-r--r--   0 toor      (1000) toor      (1000)     1103 2022-07-05 14:23:59.000000 educommon-3.9.4/src/educommon/ws_log/templates/ui-js/smev-logs-report-setting-window.js
+-rw-r--r--   0 toor      (1000) toor      (1000)     4038 2024-04-03 06:43:15.000000 educommon-3.9.4/src/educommon/ws_log/ui.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     1753 2024-04-03 06:43:15.000000 educommon-3.9.4/src/educommon/ws_log/utils.py
+drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-04-03 06:43:20.583266 educommon-3.9.4/src/educommon.egg-info/
+-rw-r--r--   0 toor      (1000) toor      (1000)     1472 2024-04-03 06:43:20.000000 educommon-3.9.4/src/educommon.egg-info/PKG-INFO
+-rw-r--r--   0 toor      (1000) toor      (1000)    16404 2024-04-03 06:43:20.000000 educommon-3.9.4/src/educommon.egg-info/SOURCES.txt
+-rw-r--r--   0 toor      (1000) toor      (1000)       43 2024-04-03 06:43:20.000000 educommon-3.9.4/src/educommon.egg-info/dependency_links.txt
+-rw-r--r--   0 toor      (1000) toor      (1000)      351 2024-04-03 06:43:20.000000 educommon-3.9.4/src/educommon.egg-info/requires.txt
+-rw-r--r--   0 toor      (1000) toor      (1000)       10 2024-04-03 06:43:20.000000 educommon-3.9.4/src/educommon.egg-info/top_level.txt
+drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2024-04-03 06:43:20.580266 educommon-3.9.4/tests/
+-rw-r--r--   0 toor      (1000) toor      (1000)     6188 2024-04-03 06:43:15.000000 educommon-3.9.4/tests/test_contingent_plugin_utils.py
+-rw-r--r--   0 toor      (1000) toor      (1000)    28100 2024-04-03 06:43:15.000000 educommon-3.9.4/tests/test_dates_splitter.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     2500 2024-04-03 06:43:15.000000 educommon-3.9.4/tests/test_delete_check.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     5018 2024-04-03 06:43:15.000000 educommon-3.9.4/tests/test_delete_objects.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     3203 2024-04-03 06:43:15.000000 educommon-3.9.4/tests/test_django_db_utils.py
+-rw-r--r--   0 toor      (1000) toor      (1000)    21544 2024-04-03 06:43:15.000000 educommon-3.9.4/tests/test_interval_mixins.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     1817 2024-04-03 06:43:15.000000 educommon-3.9.4/tests/test_patches.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     7024 2024-04-03 06:43:15.000000 educommon-3.9.4/tests/test_personal_data_fields.py
+-rw-r--r--   0 toor      (1000) toor      (1000)    14369 2024-04-03 06:43:15.000000 educommon-3.9.4/tests/test_report.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     1688 2024-04-03 06:43:15.000000 educommon-3.9.4/tests/test_service_db_router.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     2332 2024-04-03 06:43:15.000000 educommon-3.9.4/tests/test_utils.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     2137 2024-04-03 06:43:15.000000 educommon-3.9.4/tests/test_utils_plugins.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     9435 2024-04-03 06:43:15.000000 educommon-3.9.4/tests/test_validators.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     5881 2024-04-03 06:43:15.000000 educommon-3.9.4/tests/tests_rbac.py
```

### Comparing `educommon-3.9.3/PKG-INFO` & `educommon-3.9.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: educommon
-Version: 3.9.3
+Version: 3.9.4
 Summary: Общая кодовая база для проектов БЦ Образование
 Home-page: https://stash.bars-open.ru/projects/EDUBASE/repos/educommon
 Author: BARS Group
 Author-email: education_dev@bars-open.ru
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Web Environment
 Classifier: Natural Language :: Russian
```

### Comparing `educommon-3.9.3/README.rst` & `educommon-3.9.4/README.rst`

 * *Files identical despite different names*

### Comparing `educommon-3.9.3/UPGRADE.rst` & `educommon-3.9.4/UPGRADE.rst`

 * *Files identical despite different names*

### Comparing `educommon-3.9.3/setup.py` & `educommon-3.9.4/setup.py`

 * *Files identical despite different names*

### Comparing `educommon-3.9.3/src/educommon/about/README.rst` & `educommon-3.9.4/src/educommon/about/README.rst`

 * *Files identical despite different names*

### Comparing `educommon-3.9.3/src/educommon/about/static/edu_about/barsgroup.png` & `educommon-3.9.4/src/educommon/about/static/edu_about/barsgroup.png`

 * *Files identical despite different names*

### Comparing `educommon-3.9.3/src/educommon/about/ui/about-window.js` & `educommon-3.9.4/src/educommon/about/ui/about-window.js`

 * *Files identical despite different names*

### Comparing `educommon-3.9.3/src/educommon/about/ui/actions.py` & `educommon-3.9.4/src/educommon/about/ui/actions.py`

 * *Files identical despite different names*

### Comparing `educommon-3.9.3/src/educommon/about/ui/common-tab.html` & `educommon-3.9.4/src/educommon/about/ui/common-tab.html`

 * *Files identical despite different names*

### Comparing `educommon-3.9.3/src/educommon/about/ui/packages-tab.js` & `educommon-3.9.4/src/educommon/about/ui/packages-tab.js`

 * *Files identical despite different names*

### Comparing `educommon-3.9.3/src/educommon/about/ui/ui.py` & `educommon-3.9.4/src/educommon/about/ui/ui.py`

 * *Files identical despite different names*

### Comparing `educommon-3.9.3/src/educommon/about/utils.py` & `educommon-3.9.4/src/educommon/about/utils.py`

 * *Files identical despite different names*

### Comparing `educommon-3.9.3/src/educommon/async_task/actions.py` & `educommon-3.9.4/src/educommon/async_task/actions.py`

 * *Files identical despite different names*

### Comparing `educommon-3.9.3/src/educommon/async_task/helpers.py` & `educommon-3.9.4/src/educommon/async_task/helpers.py`

 * *Files identical despite different names*

### Comparing `educommon-3.9.3/src/educommon/async_task/locker.py` & `educommon-3.9.4/src/educommon/async_task/locker.py`

 * *Files identical despite different names*

### Comparing `educommon-3.9.3/src/educommon/async_task/migrations/0001_initial.py` & `educommon-3.9.4/src/educommon/async_task/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `educommon-3.9.3/src/educommon/async_task/migrations/0002_task_type_and_status_data.py` & `educommon-3.9.4/src/educommon/async_task/migrations/0002_task_type_and_status_data.py`

 * *Files identical despite different names*

### Comparing `educommon-3.9.3/src/educommon/async_task/models.py` & `educommon-3.9.4/src/educommon/async_task/models.py`

 * *Files identical despite different names*

### Comparing `educommon-3.9.3/src/educommon/async_task/tasks.py` & `educommon-3.9.4/src/educommon/async_task/tasks.py`

 * *Files identical despite different names*

### Comparing `educommon-3.9.3/src/educommon/async_task/templates/ui-js/async-task-list-win.js` & `educommon-3.9.4/src/educommon/async_task/templates/ui-js/async-task-list-win.js`

 * *Files identical despite different names*

### Comparing `educommon-3.9.3/src/educommon/async_task/templates/ui-js/async-task-revoke.js` & `educommon-3.9.4/src/educommon/async_task/templates/ui-js/async-task-revoke.js`

 * *Files identical despite different names*

### Comparing `educommon-3.9.3/src/educommon/async_task/ui.py` & `educommon-3.9.4/src/educommon/async_task/ui.py`

 * *Files identical despite different names*

### Comparing `educommon-3.9.3/src/educommon/async_tasks/locks.py` & `educommon-3.9.4/src/educommon/async_tasks/locks.py`

 * *Files identical despite different names*

### Comparing `educommon-3.9.3/src/educommon/async_tasks/migrations/0001_initial.py` & `educommon-3.9.4/src/educommon/async_tasks/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `educommon-3.9.3/src/educommon/async_tasks/models.py` & `educommon-3.9.4/src/educommon/async_tasks/models.py`

 * *Files identical despite different names*

### Comparing `educommon-3.9.3/src/educommon/async_tasks/statuses.py` & `educommon-3.9.4/src/educommon/async_tasks/statuses.py`

 * *Files identical despite different names*

### Comparing `educommon-3.9.3/src/educommon/async_tasks/tasks.py` & `educommon-3.9.4/src/educommon/async_tasks/tasks.py`

 * *Files identical despite different names*

### Comparing `educommon-3.9.3/src/educommon/audit_log/__init__.py` & `educommon-3.9.4/src/educommon/audit_log/__init__.py`

 * *Files identical despite different names*

### Comparing `educommon-3.9.3/src/educommon/audit_log/actions.py` & `educommon-3.9.4/src/educommon/audit_log/actions.py`

 * *Files identical despite different names*

### Comparing `educommon-3.9.3/src/educommon/audit_log/apps.py` & `educommon-3.9.4/src/educommon/audit_log/apps.py`

 * *Files identical despite different names*

### Comparing `educommon-3.9.3/src/educommon/audit_log/constants.py` & `educommon-3.9.4/src/educommon/audit_log/constants.py`

 * *Files identical despite different names*

### Comparing `educommon-3.9.3/src/educommon/audit_log/error_log/actions.py` & `educommon-3.9.4/src/educommon/audit_log/error_log/actions.py`

 * *Files identical despite different names*

### Comparing `educommon-3.9.3/src/educommon/audit_log/helpers.py` & `educommon-3.9.4/src/educommon/audit_log/helpers.py`

 * *Files identical despite different names*

### Comparing `educommon-3.9.3/src/educommon/audit_log/management/commands/reinstall_audit_log.py` & `educommon-3.9.4/src/educommon/audit_log/management/commands/reinstall_audit_log.py`

 * *Files identical despite different names*

### Comparing `educommon-3.9.3/src/educommon/audit_log/middleware.py` & `educommon-3.9.4/src/educommon/audit_log/middleware.py`

 * *Files identical despite different names*

### Comparing `educommon-3.9.3/src/educommon/audit_log/migrations/0001_initial.py` & `educommon-3.9.4/src/educommon/audit_log/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `educommon-3.9.3/src/educommon/audit_log/migrations/0002_install_audit_log.py` & `educommon-3.9.4/src/educommon/audit_log/migrations/0002_install_audit_log.py`

 * *Files identical despite different names*

### Comparing `educommon-3.9.3/src/educommon/audit_log/migrations/0005_postgresql_error.py` & `educommon-3.9.4/src/educommon/audit_log/migrations/0005_postgresql_error.py`

 * *Files identical despite different names*

### Comparing `educommon-3.9.3/src/educommon/audit_log/migrations/0006_auto_20200806_1707.py` & `educommon-3.9.4/src/educommon/audit_log/migrations/0006_auto_20200806_1707.py`

 * *Files identical despite different names*

### Comparing `educommon-3.9.3/src/educommon/audit_log/migrations/0007_create_selective_tables_function.py` & `educommon-3.9.4/src/educommon/audit_log/migrations/0007_create_selective_tables_function.py`

 * *Files identical despite different names*

### Comparing `educommon-3.9.3/src/educommon/audit_log/models.py` & `educommon-3.9.4/src/educommon/audit_log/models.py`

 * *Files identical despite different names*

### Comparing `educommon-3.9.3/src/educommon/audit_log/permissions.py` & `educommon-3.9.4/src/educommon/audit_log/permissions.py`

 * *Files identical despite different names*

### Comparing `educommon-3.9.3/src/educommon/audit_log/proxies.py` & `educommon-3.9.4/src/educommon/audit_log/proxies.py`

 * *Files identical despite different names*

### Comparing `educommon-3.9.3/src/educommon/audit_log/sql/configure_audit_log.sql` & `educommon-3.9.4/src/educommon/audit_log/sql/configure_audit_log.sql`

 * *Files identical despite different names*

### Comparing `educommon-3.9.3/src/educommon/audit_log/sql/install_audit_log.sql` & `educommon-3.9.4/src/educommon/audit_log/sql/install_audit_log.sql`

 * *Files identical despite different names*

### Comparing `educommon-3.9.3/src/educommon/audit_log/ui.py` & `educommon-3.9.4/src/educommon/audit_log/ui.py`

 * *Files identical despite different names*

### Comparing `educommon-3.9.3/src/educommon/audit_log/utils/__init__.py` & `educommon-3.9.4/src/educommon/audit_log/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `educommon-3.9.3/src/educommon/audit_log/utils/operations.py` & `educommon-3.9.4/src/educommon/audit_log/utils/operations.py`

 * *Files identical despite different names*

### Comparing `educommon-3.9.3/src/educommon/auth/rbac/actions.py` & `educommon-3.9.4/src/educommon/auth/rbac/actions.py`

 * *Files identical despite different names*

### Comparing `educommon-3.9.3/src/educommon/auth/rbac/backends/base.py` & `educommon-3.9.4/src/educommon/auth/rbac/backends/base.py`

 * *Files identical despite different names*

### Comparing `educommon-3.9.3/src/educommon/auth/rbac/backends/caching.py` & `educommon-3.9.4/src/educommon/auth/rbac/backends/caching.py`

 * *Files identical despite different names*

### Comparing `educommon-3.9.3/src/educommon/auth/rbac/backends/simple.py` & `educommon-3.9.4/src/educommon/auth/rbac/backends/simple.py`

 * *Files identical despite different names*

### Comparing `educommon-3.9.3/src/educommon/auth/rbac/checker.py` & `educommon-3.9.4/src/educommon/auth/rbac/checker.py`

 * *Files identical despite different names*

### Comparing `educommon-3.9.3/src/educommon/auth/rbac/config.py` & `educommon-3.9.4/src/educommon/auth/rbac/config.py`

 * *Files identical despite different names*

### Comparing `educommon-3.9.3/src/educommon/auth/rbac/management/commands/rbac.py` & `educommon-3.9.4/src/educommon/auth/rbac/management/commands/rbac.py`

 * *Files identical despite different names*

### Comparing `educommon-3.9.3/src/educommon/auth/rbac/manager.py` & `educommon-3.9.4/src/educommon/auth/rbac/manager.py`

 * *Files identical despite different names*

### Comparing `educommon-3.9.3/src/educommon/auth/rbac/migrations/0001_initial.py` & `educommon-3.9.4/src/educommon/auth/rbac/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `educommon-3.9.3/src/educommon/auth/rbac/migrations/0002_model_modifier_metaclass_fix.py` & `educommon-3.9.4/src/educommon/auth/rbac/migrations/0002_model_modifier_metaclass_fix.py`

 * *Files identical despite different names*

### Comparing `educommon-3.9.3/src/educommon/auth/rbac/migrations/0004_auto_20171024_1245.py` & `educommon-3.9.4/src/educommon/auth/rbac/migrations/0004_auto_20171024_1245.py`

 * *Files identical despite different names*

### Comparing `educommon-3.9.3/src/educommon/auth/rbac/models.py` & `educommon-3.9.4/src/educommon/auth/rbac/models.py`

 * *Files identical despite different names*

### Comparing `educommon-3.9.3/src/educommon/auth/rbac/permissions.py` & `educommon-3.9.4/src/educommon/auth/rbac/permissions.py`

 * *Files identical despite different names*

### Comparing `educommon-3.9.3/src/educommon/auth/rbac/templates/rbac/role-edit-window.js` & `educommon-3.9.4/src/educommon/auth/rbac/templates/rbac/role-edit-window.js`

 * *Files identical despite different names*

### Comparing `educommon-3.9.3/src/educommon/auth/rbac/templates/rbac/roles-list-window.js` & `educommon-3.9.4/src/educommon/auth/rbac/templates/rbac/roles-list-window.js`

 * *Files identical despite different names*

### Comparing `educommon-3.9.3/src/educommon/auth/rbac/templates/rbac/roles-view-list-window.js` & `educommon-3.9.4/src/educommon/auth/rbac/templates/rbac/roles-view-list-window.js`

 * *Files identical despite different names*

### Comparing `educommon-3.9.3/src/educommon/auth/rbac/ui.py` & `educommon-3.9.4/src/educommon/auth/rbac/ui.py`

 * *Files identical despite different names*

### Comparing `educommon-3.9.3/src/educommon/auth/rbac/utils.py` & `educommon-3.9.4/src/educommon/auth/rbac/utils.py`

 * *Files identical despite different names*

### Comparing `educommon-3.9.3/src/educommon/auth/simple_auth/actions.py` & `educommon-3.9.4/src/educommon/auth/simple_auth/actions.py`

 * *Files identical despite different names*

### Comparing `educommon-3.9.3/src/educommon/auth/simple_auth/app_meta.py` & `educommon-3.9.4/src/educommon/auth/simple_auth/app_meta.py`

 * *Files identical despite different names*

### Comparing `educommon-3.9.3/src/educommon/auth/simple_auth/checkers.py` & `educommon-3.9.4/src/educommon/auth/simple_auth/checkers.py`

 * *Files identical despite different names*

### Comparing `educommon-3.9.3/src/educommon/auth/simple_auth/migrations/0001_initial.py` & `educommon-3.9.4/src/educommon/auth/simple_auth/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `educommon-3.9.3/src/educommon/auth/simple_auth/models.py` & `educommon-3.9.4/src/educommon/auth/simple_auth/models.py`

 * *Files identical despite different names*

### Comparing `educommon-3.9.3/src/educommon/auth/simple_auth/templates/simple_auth/change_reset_password_page.html` & `educommon-3.9.4/src/educommon/auth/simple_auth/templates/simple_auth/change_reset_password_page.html`

 * *Files identical despite different names*

### Comparing `educommon-3.9.3/src/educommon/auth/simple_auth/templates/simple_auth/email/reset_password.html` & `educommon-3.9.4/src/educommon/auth/simple_auth/templates/simple_auth/email/reset_password.html`

 * *Files identical despite different names*

### Comparing `educommon-3.9.3/src/educommon/auth/simple_auth/templates/simple_auth/login_page.html` & `educommon-3.9.4/src/educommon/auth/simple_auth/templates/simple_auth/login_page.html`

 * *Files identical despite different names*

### Comparing `educommon-3.9.3/src/educommon/auth/simple_auth/templates/simple_auth/reset_password_page.html` & `educommon-3.9.4/src/educommon/auth/simple_auth/templates/simple_auth/reset_password_page.html`

 * *Files identical despite different names*

### Comparing `educommon-3.9.3/src/educommon/auth/simple_auth/ui.py` & `educommon-3.9.4/src/educommon/auth/simple_auth/ui.py`

 * *Files identical despite different names*

### Comparing `educommon-3.9.3/src/educommon/contingent/actions.py` & `educommon-3.9.4/src/educommon/contingent/actions.py`

 * *Files identical despite different names*

### Comparing `educommon-3.9.3/src/educommon/contingent/base.py` & `educommon-3.9.4/src/educommon/contingent/base.py`

 * *Files identical despite different names*

### Comparing `educommon-3.9.3/src/educommon/contingent/catalogs.py` & `educommon-3.9.4/src/educommon/contingent/catalogs.py`

 * *Files identical despite different names*

### Comparing `educommon-3.9.3/src/educommon/contingent/contingent_plugin/actions.py` & `educommon-3.9.4/src/educommon/contingent/contingent_plugin/actions.py`

 * *Files identical despite different names*

### Comparing `educommon-3.9.3/src/educommon/contingent/contingent_plugin/apps.py` & `educommon-3.9.4/src/educommon/contingent/contingent_plugin/apps.py`

 * *Files identical despite different names*

### Comparing `educommon-3.9.3/src/educommon/contingent/contingent_plugin/migrations/0001_initial.py` & `educommon-3.9.4/src/educommon/contingent/contingent_plugin/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `educommon-3.9.3/src/educommon/contingent/contingent_plugin/migrations/0002_add_contingent_model_deleted.py` & `educommon-3.9.4/src/educommon/contingent/contingent_plugin/migrations/0002_add_contingent_model_deleted.py`

 * *Files identical despite different names*

### Comparing `educommon-3.9.3/src/educommon/contingent/contingent_plugin/model_views.py` & `educommon-3.9.4/src/educommon/contingent/contingent_plugin/model_views.py`

 * *Files identical despite different names*

### Comparing `educommon-3.9.3/src/educommon/contingent/contingent_plugin/models.py` & `educommon-3.9.4/src/educommon/contingent/contingent_plugin/models.py`

 * *Files identical despite different names*

### Comparing `educommon-3.9.3/src/educommon/contingent/contingent_plugin/observer.py` & `educommon-3.9.4/src/educommon/contingent/contingent_plugin/observer.py`

 * *Files identical despite different names*

### Comparing `educommon-3.9.3/src/educommon/contingent/contingent_plugin/storage.py` & `educommon-3.9.4/src/educommon/contingent/contingent_plugin/storage.py`

 * *Files identical despite different names*

### Comparing `educommon-3.9.3/src/educommon/contingent/contingent_plugin/utils.py` & `educommon-3.9.4/src/educommon/contingent/contingent_plugin/utils.py`

 * *Files identical despite different names*

### Comparing `educommon-3.9.3/src/educommon/contingent/json_data/icao.json` & `educommon-3.9.4/src/educommon/contingent/json_data/icao.json`

 * *Files identical despite different names*

### Comparing `educommon-3.9.3/src/educommon/contingent/json_data/okogu.json` & `educommon-3.9.4/src/educommon/contingent/json_data/okogu.json`

 * *Files identical despite different names*

### Comparing `educommon-3.9.3/src/educommon/contingent/json_data/oksm.json` & `educommon-3.9.4/src/educommon/contingent/json_data/oksm.json`

 * *Files identical despite different names*

### Comparing `educommon-3.9.3/src/educommon/django/db/fields.py` & `educommon-3.9.4/src/educommon/django/db/fields.py`

 * *Files identical despite different names*

### Comparing `educommon-3.9.3/src/educommon/django/db/migration/__init__.py` & `educommon-3.9.4/src/educommon/django/db/migration/__init__.py`

 * *Files identical despite different names*

### Comparing `educommon-3.9.3/src/educommon/django/db/migration/operations.py` & `educommon-3.9.4/src/educommon/django/db/migration/operations.py`

 * *Files identical despite different names*

### Comparing `educommon-3.9.3/src/educommon/django/db/mixins/__init__.py` & `educommon-3.9.4/src/educommon/django/db/mixins/__init__.py`

 * *Files identical despite different names*

### Comparing `educommon-3.9.3/src/educommon/django/db/mixins/date_interval.py` & `educommon-3.9.4/src/educommon/django/db/mixins/date_interval.py`

 * *Files identical despite different names*

### Comparing `educommon-3.9.3/src/educommon/django/db/mixins/validation.py` & `educommon-3.9.4/src/educommon/django/db/mixins/validation.py`

 * *Files identical despite different names*

### Comparing `educommon-3.9.3/src/educommon/django/db/model_view/__init__.py` & `educommon-3.9.4/src/educommon/django/db/model_view/__init__.py`

 * *Files identical despite different names*

### Comparing `educommon-3.9.3/src/educommon/django/db/model_view/table-view.html` & `educommon-3.9.4/src/educommon/django/db/model_view/table-view.html`

 * *Files identical despite different names*

### Comparing `educommon-3.9.3/src/educommon/django/db/models.py` & `educommon-3.9.4/src/educommon/django/db/models.py`

 * *Files identical despite different names*

### Comparing `educommon-3.9.3/src/educommon/django/db/observer.py` & `educommon-3.9.4/src/educommon/django/db/observer.py`

 * *Files identical despite different names*

### Comparing `educommon-3.9.3/src/educommon/django/db/partitioning/README.md` & `educommon-3.9.4/src/educommon/django/db/partitioning/README.md`

 * *Files identical despite different names*

### Comparing `educommon-3.9.3/src/educommon/django/db/partitioning/__init__.py` & `educommon-3.9.4/src/educommon/django/db/partitioning/__init__.py`

 * *Files identical despite different names*

### Comparing `educommon-3.9.3/src/educommon/django/db/partitioning/management/commands/apply_partitioning.py` & `educommon-3.9.4/src/educommon/django/db/partitioning/management/commands/apply_partitioning.py`

 * *Files identical despite different names*

### Comparing `educommon-3.9.3/src/educommon/django/db/partitioning/management/commands/clear_table.py` & `educommon-3.9.4/src/educommon/django/db/partitioning/management/commands/clear_table.py`

 * *Files identical despite different names*

### Comparing `educommon-3.9.3/src/educommon/django/db/partitioning/management/commands/split_table.py` & `educommon-3.9.4/src/educommon/django/db/partitioning/management/commands/split_table.py`

 * *Files identical despite different names*

### Comparing `educommon-3.9.3/src/educommon/django/db/partitioning/partitioning.sql` & `educommon-3.9.4/src/educommon/django/db/partitioning/partitioning.sql`

 * *Files identical despite different names*

### Comparing `educommon-3.9.3/src/educommon/django/db/partitioning/triggers.sql` & `educommon-3.9.4/src/educommon/django/db/partitioning/triggers.sql`

 * *Files identical despite different names*

### Comparing `educommon-3.9.3/src/educommon/django/db/routers.py` & `educommon-3.9.4/src/educommon/django/db/routers.py`

 * *Files identical despite different names*

### Comparing `educommon-3.9.3/src/educommon/django/db/utils.py` & `educommon-3.9.4/src/educommon/django/db/utils.py`

 * *Files identical despite different names*

### Comparing `educommon-3.9.3/src/educommon/django/db/validators/__init__.py` & `educommon-3.9.4/src/educommon/django/db/validators/__init__.py`

 * *Files identical despite different names*

### Comparing `educommon-3.9.3/src/educommon/django/db/validators/simple.py` & `educommon-3.9.4/src/educommon/django/db/validators/simple.py`

 * *Files identical despite different names*

### Comparing `educommon-3.9.3/src/educommon/django/storages/atcfs/README.rst` & `educommon-3.9.4/src/educommon/django/storages/atcfs/README.rst`

 * *Files identical despite different names*

### Comparing `educommon-3.9.3/src/educommon/django/storages/atcfs/api.py` & `educommon-3.9.4/src/educommon/django/storages/atcfs/api.py`

 * *Files identical despite different names*

### Comparing `educommon-3.9.3/src/educommon/django/storages/atcfs/management/commands/atcfs_migrate.py` & `educommon-3.9.4/src/educommon/django/storages/atcfs/management/commands/atcfs_migrate.py`

 * *Files identical despite different names*

### Comparing `educommon-3.9.3/src/educommon/django/storages/atcfs/monkey_patching.py` & `educommon-3.9.4/src/educommon/django/storages/atcfs/monkey_patching.py`

 * *Files identical despite different names*

### Comparing `educommon-3.9.3/src/educommon/django/storages/atcfs/settings.py` & `educommon-3.9.4/src/educommon/django/storages/atcfs/settings.py`

 * *Files identical despite different names*

### Comparing `educommon-3.9.3/src/educommon/django/storages/atcfs/storage.py` & `educommon-3.9.4/src/educommon/django/storages/atcfs/storage.py`

 * *Files identical despite different names*

### Comparing `educommon-3.9.3/src/educommon/extjs/fields/input_params.py` & `educommon-3.9.4/src/educommon/extjs/fields/input_params.py`

 * *Files identical despite different names*

### Comparing `educommon-3.9.3/src/educommon/importer/XLSReader.py` & `educommon-3.9.4/src/educommon/importer/XLSReader.py`

 * *Files identical despite different names*

### Comparing `educommon-3.9.3/src/educommon/importer/api.py` & `educommon-3.9.4/src/educommon/importer/api.py`

 * *Files identical despite different names*

### Comparing `educommon-3.9.3/src/educommon/importer/constants.py` & `educommon-3.9.4/src/educommon/importer/constants.py`

 * *Files identical despite different names*

### Comparing `educommon-3.9.3/src/educommon/importer/loggers.py` & `educommon-3.9.4/src/educommon/importer/loggers.py`

 * *Files identical despite different names*

### Comparing `educommon-3.9.3/src/educommon/importer/proxy.py` & `educommon-3.9.4/src/educommon/importer/proxy.py`

 * *Files identical despite different names*

### Comparing `educommon-3.9.3/src/educommon/importer/proxy_import.py` & `educommon-3.9.4/src/educommon/importer/proxy_import.py`

 * *Files identical despite different names*

### Comparing `educommon-3.9.3/src/educommon/importer/refactoring-notes.txt` & `educommon-3.9.4/src/educommon/importer/refactoring-notes.txt`

 * *Files identical despite different names*

### Comparing `educommon-3.9.3/src/educommon/importer/report.py` & `educommon-3.9.4/src/educommon/importer/report.py`

 * *Files identical despite different names*

### Comparing `educommon-3.9.3/src/educommon/importer/test_file.xls` & `educommon-3.9.4/src/educommon/importer/test_file.xls`

 * *Files identical despite different names*

### Comparing `educommon-3.9.3/src/educommon/importer/ui.py` & `educommon-3.9.4/src/educommon/importer/ui.py`

 * *Files identical despite different names*

### Comparing `educommon-3.9.3/src/educommon/importer/validators.py` & `educommon-3.9.4/src/educommon/importer/validators.py`

 * *Files identical despite different names*

### Comparing `educommon-3.9.3/src/educommon/integration_entities/entities.py` & `educommon-3.9.4/src/educommon/integration_entities/entities.py`

 * *Files identical despite different names*

### Comparing `educommon-3.9.3/src/educommon/integration_entities/helpers.py` & `educommon-3.9.4/src/educommon/integration_entities/helpers.py`

 * *Files identical despite different names*

### Comparing `educommon-3.9.3/src/educommon/integration_entities/mixins.py` & `educommon-3.9.4/src/educommon/integration_entities/mixins.py`

 * *Files identical despite different names*

### Comparing `educommon-3.9.3/src/educommon/ioc/__init__.py` & `educommon-3.9.4/src/educommon/ioc/__init__.py`

 * *Files identical despite different names*

### Comparing `educommon-3.9.3/src/educommon/logger/__init__.py` & `educommon-3.9.4/src/educommon/logger/__init__.py`

 * *Files identical despite different names*

### Comparing `educommon-3.9.3/src/educommon/logger/apps.py` & `educommon-3.9.4/src/educommon/logger/apps.py`

 * *Files identical despite different names*

### Comparing `educommon-3.9.3/src/educommon/logger/helpers.py` & `educommon-3.9.4/src/educommon/logger/helpers.py`

 * *Files identical despite different names*

### Comparing `educommon-3.9.3/src/educommon/logger/loggers.py` & `educommon-3.9.4/src/educommon/logger/loggers.py`

 * *Files identical despite different names*

### Comparing `educommon-3.9.3/src/educommon/m3/__init__.py` & `educommon-3.9.4/src/educommon/m3/__init__.py`

 * *Files identical despite different names*

### Comparing `educommon-3.9.3/src/educommon/m3/extensions/listeners/__init__.py` & `educommon-3.9.4/src/educommon/m3/extensions/listeners/__init__.py`

 * *Files identical despite different names*

### Comparing `educommon-3.9.3/src/educommon/m3/extensions/listeners/delete_check/cancel-confirm-window.js` & `educommon-3.9.4/src/educommon/m3/extensions/listeners/delete_check/cancel-confirm-window.js`

 * *Files identical despite different names*

### Comparing `educommon-3.9.3/src/educommon/m3/extensions/listeners/delete_check/listeners.py` & `educommon-3.9.4/src/educommon/m3/extensions/listeners/delete_check/listeners.py`

 * *Files identical despite different names*

### Comparing `educommon-3.9.3/src/educommon/m3/extensions/listeners/delete_check/mixins.py` & `educommon-3.9.4/src/educommon/m3/extensions/listeners/delete_check/mixins.py`

 * *Files identical despite different names*

### Comparing `educommon-3.9.3/src/educommon/m3/extensions/listeners/delete_check/ui.py` & `educommon-3.9.4/src/educommon/m3/extensions/listeners/delete_check/ui.py`

 * *Files identical despite different names*

### Comparing `educommon-3.9.3/src/educommon/m3/extensions/listeners/delete_check/utils.py` & `educommon-3.9.4/src/educommon/m3/extensions/listeners/delete_check/utils.py`

 * *Files identical despite different names*

### Comparing `educommon-3.9.3/src/educommon/m3/extensions/ui.py` & `educommon-3.9.4/src/educommon/m3/extensions/ui.py`

 * *Files identical despite different names*

### Comparing `educommon-3.9.3/src/educommon/m3/transaction_context.py` & `educommon-3.9.4/src/educommon/m3/transaction_context.py`

 * *Files identical despite different names*

### Comparing `educommon-3.9.3/src/educommon/objectpack/actions.py` & `educommon-3.9.4/src/educommon/objectpack/actions.py`

 * *Files identical despite different names*

### Comparing `educommon-3.9.3/src/educommon/objectpack/filters.py` & `educommon-3.9.4/src/educommon/objectpack/filters.py`

 * *Files identical despite different names*

### Comparing `educommon-3.9.3/src/educommon/objectpack/templates/filter-panel.js` & `educommon-3.9.4/src/educommon/objectpack/templates/filter-panel.js`

 * *Files identical despite different names*

### Comparing `educommon-3.9.3/src/educommon/objectpack/templates/grid-panel.js` & `educommon-3.9.4/src/educommon/objectpack/templates/grid-panel.js`

 * *Files identical despite different names*

### Comparing `educommon-3.9.3/src/educommon/objectpack/templates/multiSelectWindow.js` & `educommon-3.9.4/src/educommon/objectpack/templates/multiSelectWindow.js`

 * *Files identical despite different names*

### Comparing `educommon-3.9.3/src/educommon/objectpack/templates/multiselect-page-fix.js` & `educommon-3.9.4/src/educommon/objectpack/templates/multiselect-page-fix.js`

 * *Files identical despite different names*

### Comparing `educommon-3.9.3/src/educommon/objectpack/templates/relations-check-mixin-template.html` & `educommon-3.9.4/src/educommon/objectpack/templates/relations-check-mixin-template.html`

 * *Files identical despite different names*

### Comparing `educommon-3.9.3/src/educommon/objectpack/ui.py` & `educommon-3.9.4/src/educommon/objectpack/ui.py`

 * *Files identical despite different names*

### Comparing `educommon-3.9.3/src/educommon/report/__init__.py` & `educommon-3.9.4/src/educommon/report/__init__.py`

 * *Files identical despite different names*

### Comparing `educommon-3.9.3/src/educommon/report/actions.py` & `educommon-3.9.4/src/educommon/report/actions.py`

 * *Files identical despite different names*

### Comparing `educommon-3.9.3/src/educommon/report/constructor/README.rst` & `educommon-3.9.4/src/educommon/report/constructor/README.rst`

 * *Files identical despite different names*

### Comparing `educommon-3.9.3/src/educommon/report/constructor/__init__.py` & `educommon-3.9.4/src/educommon/report/constructor/__init__.py`

 * *Files identical despite different names*

### Comparing `educommon-3.9.3/src/educommon/report/constructor/base.py` & `educommon-3.9.4/src/educommon/report/constructor/base.py`

 * *Files 4% similar despite different names*

```diff
@@ -227,14 +227,19 @@
         accessor_name = fld_accessor_name
         while descriptor.parent:
             accessor_name = '.'.join(
                 (descriptor.accessor_name, accessor_name)
             )
             if skip_field(descriptor.parent.model, field, accessor_name):
                 return True
+            # проверка, что связанная модель поля, не связана с родительскими моделями полей
+            if (getattr(field, 'related_model', None) and
+                field.related_model in descriptor.parent.related_field_models
+            ):
+                return True
 
             descriptor = descriptor.parent
         # проверка модели источника данных
         accessor_name = '.'.join((self.full_accessor_name, fld_accessor_name))
         if skip_field(self.data_source.model, field, accessor_name):
             return True
 
@@ -247,14 +252,33 @@
         elif isinstance(self.field, RelatedField):
             model = get_related(self.field).parent_model
         else:
             model = None
 
         return model
 
+    @cached_property
+    def related_field_models(self):
+        """Связанные модели полей."""
+        fields_models = set()
+        # Для первых в корне добавляем модели источника данных.
+        if self.parent is None:
+            data_source_columns = tuple(self.data_source.get_available_columns())
+            fields_models.update({column.model for column in data_source_columns if column.model})
+            fields_models.add(self.data_source.model)
+
+        # получаем поля текущего экземпляра
+        if self.model:
+            fields = self.model._meta.get_fields()
+            fields_models.update({field.related_model for field in fields if field.related_model})
+            # добавляем саму модель экземпляра, если она есть
+            fields_models.add(self.model)
+
+        return fields_models
+
     @property
     def accessor_name(self):
         return force_str(_get_accessor_name(self.field))
 
     @property
     def lookup(self):
         return force_str(self.field.name)
```

### Comparing `educommon-3.9.3/src/educommon/report/constructor/builders/excel/_base.py` & `educommon-3.9.4/src/educommon/report/constructor/builders/excel/_base.py`

 * *Files identical despite different names*

### Comparing `educommon-3.9.3/src/educommon/report/constructor/builders/excel/_header.py` & `educommon-3.9.4/src/educommon/report/constructor/builders/excel/_header.py`

 * *Files identical despite different names*

### Comparing `educommon-3.9.3/src/educommon/report/constructor/builders/excel/product.py` & `educommon-3.9.4/src/educommon/report/constructor/builders/excel/product.py`

 * *Files identical despite different names*

### Comparing `educommon-3.9.3/src/educommon/report/constructor/builders/excel/with_merged_cells.py` & `educommon-3.9.4/src/educommon/report/constructor/builders/excel/with_merged_cells.py`

 * *Files identical despite different names*

### Comparing `educommon-3.9.3/src/educommon/report/constructor/config.py` & `educommon-3.9.4/src/educommon/report/constructor/config.py`

 * *Files identical despite different names*

### Comparing `educommon-3.9.3/src/educommon/report/constructor/constants.py` & `educommon-3.9.4/src/educommon/report/constructor/constants.py`

 * *Files identical despite different names*

### Comparing `educommon-3.9.3/src/educommon/report/constructor/editor/actions.py` & `educommon-3.9.4/src/educommon/report/constructor/editor/actions.py`

 * *Files identical despite different names*

### Comparing `educommon-3.9.3/src/educommon/report/constructor/editor/edit-window.js` & `educommon-3.9.4/src/educommon/report/constructor/editor/edit-window.js`

 * *Files identical despite different names*

### Comparing `educommon-3.9.3/src/educommon/report/constructor/editor/list-window.js` & `educommon-3.9.4/src/educommon/report/constructor/editor/list-window.js`

 * *Files identical despite different names*

### Comparing `educommon-3.9.3/src/educommon/report/constructor/editor/ui.py` & `educommon-3.9.4/src/educommon/report/constructor/editor/ui.py`

 * *Files identical despite different names*

### Comparing `educommon-3.9.3/src/educommon/report/constructor/exceptions.py` & `educommon-3.9.4/src/educommon/report/constructor/exceptions.py`

 * *Files identical despite different names*

### Comparing `educommon-3.9.3/src/educommon/report/constructor/migrations/0001_initial.py` & `educommon-3.9.4/src/educommon/report/constructor/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `educommon-3.9.3/src/educommon/report/constructor/migrations/0002_report_filters.py` & `educommon-3.9.4/src/educommon/report/constructor/migrations/0002_report_filters.py`

 * *Files identical despite different names*

### Comparing `educommon-3.9.3/src/educommon/report/constructor/migrations/0004_reportfilter_fields.py` & `educommon-3.9.4/src/educommon/report/constructor/migrations/0004_reportfilter_fields.py`

 * *Files identical despite different names*

### Comparing `educommon-3.9.3/src/educommon/report/constructor/migrations/0006_reportsorting.py` & `educommon-3.9.4/src/educommon/report/constructor/migrations/0006_reportsorting.py`

 * *Files identical despite different names*

### Comparing `educommon-3.9.3/src/educommon/report/constructor/migrations/0007_include_available_units.py` & `educommon-3.9.4/src/educommon/report/constructor/migrations/0007_include_available_units.py`

 * *Files identical despite different names*

### Comparing `educommon-3.9.3/src/educommon/report/constructor/migrations/0008_auto_20170407_1318.py` & `educommon-3.9.4/src/educommon/report/constructor/migrations/0008_auto_20170407_1318.py`

 * *Files identical despite different names*

### Comparing `educommon-3.9.3/src/educommon/report/constructor/migrations/0009_auto_20180405_0642.py` & `educommon-3.9.4/src/educommon/report/constructor/migrations/0009_auto_20180405_0642.py`

 * *Files identical despite different names*

### Comparing `educommon-3.9.3/src/educommon/report/constructor/migrations/0010_add_aggregate_fields.py` & `educommon-3.9.4/src/educommon/report/constructor/migrations/0010_add_aggregate_fields.py`

 * *Files identical despite different names*

### Comparing `educommon-3.9.3/src/educommon/report/constructor/mixins.py` & `educommon-3.9.4/src/educommon/report/constructor/mixins.py`

 * *Files identical despite different names*

### Comparing `educommon-3.9.3/src/educommon/report/constructor/models.py` & `educommon-3.9.4/src/educommon/report/constructor/models.py`

 * *Files identical despite different names*

### Comparing `educommon-3.9.3/src/educommon/report/constructor/registries.py` & `educommon-3.9.4/src/educommon/report/constructor/registries.py`

 * *Files identical despite different names*

### Comparing `educommon-3.9.3/src/educommon/report/constructor/utils.py` & `educommon-3.9.4/src/educommon/report/constructor/utils.py`

 * *Files identical despite different names*

### Comparing `educommon-3.9.3/src/educommon/report/constructor/validators.py` & `educommon-3.9.4/src/educommon/report/constructor/validators.py`

 * *Files identical despite different names*

### Comparing `educommon-3.9.3/src/educommon/report/reporter.py` & `educommon-3.9.4/src/educommon/report/reporter.py`

 * *Files identical despite different names*

### Comparing `educommon-3.9.3/src/educommon/report/utils.py` & `educommon-3.9.4/src/educommon/report/utils.py`

 * *Files identical despite different names*

### Comparing `educommon-3.9.3/src/educommon/rest/actions.py` & `educommon-3.9.4/src/educommon/rest/actions.py`

 * *Files identical despite different names*

### Comparing `educommon-3.9.3/src/educommon/rest/context.py` & `educommon-3.9.4/src/educommon/rest/context.py`

 * *Files identical despite different names*

### Comparing `educommon-3.9.3/src/educommon/rest/controllers.py` & `educommon-3.9.4/src/educommon/rest/controllers.py`

 * *Files identical despite different names*

### Comparing `educommon-3.9.3/src/educommon/rest/mixins.py` & `educommon-3.9.4/src/educommon/rest/mixins.py`

 * *Files identical despite different names*

### Comparing `educommon-3.9.3/src/educommon/secure_media/README.rst` & `educommon-3.9.4/src/educommon/secure_media/README.rst`

 * *Files identical despite different names*

### Comparing `educommon-3.9.3/src/educommon/secure_media/app_meta.py` & `educommon-3.9.4/src/educommon/secure_media/app_meta.py`

 * *Files identical despite different names*

### Comparing `educommon-3.9.3/src/educommon/utils/__init__.py` & `educommon-3.9.4/src/educommon/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `educommon-3.9.3/src/educommon/utils/caching.py` & `educommon-3.9.4/src/educommon/utils/caching.py`

 * *Files identical despite different names*

### Comparing `educommon-3.9.3/src/educommon/utils/conversion.py` & `educommon-3.9.4/src/educommon/utils/conversion.py`

 * *Files identical despite different names*

### Comparing `educommon-3.9.3/src/educommon/utils/crypto.py` & `educommon-3.9.4/src/educommon/utils/crypto.py`

 * *Files identical despite different names*

### Comparing `educommon-3.9.3/src/educommon/utils/date.py` & `educommon-3.9.4/src/educommon/utils/date.py`

 * *Files identical despite different names*

### Comparing `educommon-3.9.3/src/educommon/utils/db/__init__.py` & `educommon-3.9.4/src/educommon/utils/db/__init__.py`

 * *Files identical despite different names*

### Comparing `educommon-3.9.3/src/educommon/utils/db/postgresql.py` & `educommon-3.9.4/src/educommon/utils/db/postgresql.py`

 * *Files identical despite different names*

### Comparing `educommon-3.9.3/src/educommon/utils/fonts/Arial.ttf` & `educommon-3.9.4/src/educommon/utils/fonts/Arial.ttf`

 * *Files identical despite different names*

### Comparing `educommon-3.9.3/src/educommon/utils/fonts/Calibri.ttf` & `educommon-3.9.4/src/educommon/utils/fonts/Calibri.ttf`

 * *Files identical despite different names*

### Comparing `educommon-3.9.3/src/educommon/utils/fonts/Tahoma.ttf` & `educommon-3.9.4/src/educommon/utils/fonts/Tahoma.ttf`

 * *Files identical despite different names*

### Comparing `educommon-3.9.3/src/educommon/utils/fonts/__init__.py` & `educommon-3.9.4/src/educommon/utils/fonts/__init__.py`

 * *Files identical despite different names*

### Comparing `educommon-3.9.3/src/educommon/utils/licence/__init__.py` & `educommon-3.9.4/src/educommon/utils/licence/__init__.py`

 * *Files identical despite different names*

### Comparing `educommon-3.9.3/src/educommon/utils/licence/converters.py` & `educommon-3.9.4/src/educommon/utils/licence/converters.py`

 * *Files identical despite different names*

### Comparing `educommon-3.9.3/src/educommon/utils/misc.py` & `educommon-3.9.4/src/educommon/utils/misc.py`

 * *Files identical despite different names*

### Comparing `educommon-3.9.3/src/educommon/utils/object_grid.py` & `educommon-3.9.4/src/educommon/utils/object_grid.py`

 * *Files identical despite different names*

### Comparing `educommon-3.9.3/src/educommon/utils/patches.py` & `educommon-3.9.4/src/educommon/utils/patches.py`

 * *Files identical despite different names*

### Comparing `educommon-3.9.3/src/educommon/utils/plugins.py` & `educommon-3.9.4/src/educommon/utils/plugins.py`

 * *Files identical despite different names*

### Comparing `educommon-3.9.3/src/educommon/utils/registry.py` & `educommon-3.9.4/src/educommon/utils/registry.py`

 * *Files identical despite different names*

### Comparing `educommon-3.9.3/src/educommon/utils/seqtools.py` & `educommon-3.9.4/src/educommon/utils/seqtools.py`

 * *Files identical despite different names*

### Comparing `educommon-3.9.3/src/educommon/utils/serializer.py` & `educommon-3.9.4/src/educommon/utils/serializer.py`

 * *Files identical despite different names*

### Comparing `educommon-3.9.3/src/educommon/utils/storage.py` & `educommon-3.9.4/src/educommon/utils/storage.py`

 * *Files identical despite different names*

### Comparing `educommon-3.9.3/src/educommon/utils/system.py` & `educommon-3.9.4/src/educommon/utils/system.py`

 * *Files identical despite different names*

### Comparing `educommon-3.9.3/src/educommon/utils/system_app/management/commands/delete_objects.py` & `educommon-3.9.4/src/educommon/utils/system_app/management/commands/delete_objects.py`

 * *Files identical despite different names*

### Comparing `educommon-3.9.3/src/educommon/utils/ui.py` & `educommon-3.9.4/src/educommon/utils/ui.py`

 * *Files identical despite different names*

### Comparing `educommon-3.9.3/src/educommon/utils/xml/__init__.py` & `educommon-3.9.4/src/educommon/utils/xml/__init__.py`

 * *Files identical despite different names*

### Comparing `educommon-3.9.3/src/educommon/utils/xml/catalog.json` & `educommon-3.9.4/src/educommon/utils/xml/catalog.json`

 * *Files identical despite different names*

### Comparing `educommon-3.9.3/src/educommon/utils/xml/resolver.py` & `educommon-3.9.4/src/educommon/utils/xml/resolver.py`

 * *Files identical despite different names*

### Comparing `educommon-3.9.3/src/educommon/utils/xml/saml-schema-assertion-2.0.xsd` & `educommon-3.9.4/src/educommon/utils/xml/saml-schema-assertion-2.0.xsd`

 * *Files identical despite different names*

### Comparing `educommon-3.9.3/src/educommon/utils/xml/saml-schema-protocol-2.0.xsd` & `educommon-3.9.4/src/educommon/utils/xml/saml-schema-protocol-2.0.xsd`

 * *Files identical despite different names*

### Comparing `educommon-3.9.3/src/educommon/utils/xml/xenc-schema.xsd` & `educommon-3.9.4/src/educommon/utils/xml/xenc-schema.xsd`

 * *Files identical despite different names*

### Comparing `educommon-3.9.3/src/educommon/utils/xml/xmldsig-core-schema.xsd` & `educommon-3.9.4/src/educommon/utils/xml/xmldsig-core-schema.xsd`

 * *Files identical despite different names*

### Comparing `educommon-3.9.3/src/educommon/ws_log/README.rst` & `educommon-3.9.4/src/educommon/ws_log/README.rst`

 * *Files identical despite different names*

### Comparing `educommon-3.9.3/src/educommon/ws_log/__init__.py` & `educommon-3.9.4/src/educommon/ws_log/__init__.py`

 * *Files identical despite different names*

### Comparing `educommon-3.9.3/src/educommon/ws_log/actions.py` & `educommon-3.9.4/src/educommon/ws_log/actions.py`

 * *Files identical despite different names*

### Comparing `educommon-3.9.3/src/educommon/ws_log/base.py` & `educommon-3.9.4/src/educommon/ws_log/base.py`

 * *Files identical despite different names*

### Comparing `educommon-3.9.3/src/educommon/ws_log/migrations/0001_initial.py` & `educommon-3.9.4/src/educommon/ws_log/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `educommon-3.9.3/src/educommon/ws_log/migrations/0002_auto_20160628_1334.py` & `educommon-3.9.4/src/educommon/ws_log/migrations/0002_auto_20160628_1334.py`

 * *Files identical despite different names*

### Comparing `educommon-3.9.3/src/educommon/ws_log/migrations/0003_add_fields_to_smev_logs.py` & `educommon-3.9.4/src/educommon/ws_log/migrations/0003_add_fields_to_smev_logs.py`

 * *Files identical despite different names*

### Comparing `educommon-3.9.3/src/educommon/ws_log/migrations/0004_auto_20160727_1600.py` & `educommon-3.9.4/src/educommon/ws_log/migrations/0004_auto_20160727_1600.py`

 * *Files identical despite different names*

### Comparing `educommon-3.9.3/src/educommon/ws_log/migrations/0005_auto_20161130_1615.py` & `educommon-3.9.4/src/educommon/ws_log/migrations/0005_auto_20161130_1615.py`

 * *Files identical despite different names*

### Comparing `educommon-3.9.3/src/educommon/ws_log/migrations/0007_auto_20180607_1040.py` & `educommon-3.9.4/src/educommon/ws_log/migrations/0007_auto_20180607_1040.py`

 * *Files identical despite different names*

### Comparing `educommon-3.9.3/src/educommon/ws_log/migrations/0008_auto_20180713_1445.py` & `educommon-3.9.4/src/educommon/ws_log/migrations/0008_auto_20180713_1445.py`

 * *Files identical despite different names*

### Comparing `educommon-3.9.3/src/educommon/ws_log/migrations/0009_auto_20201130_1553.py` & `educommon-3.9.4/src/educommon/ws_log/migrations/0009_auto_20201130_1553.py`

 * *Files identical despite different names*

### Comparing `educommon-3.9.3/src/educommon/ws_log/models.py` & `educommon-3.9.4/src/educommon/ws_log/models.py`

 * *Files identical despite different names*

### Comparing `educommon-3.9.3/src/educommon/ws_log/provider.py` & `educommon-3.9.4/src/educommon/ws_log/provider.py`

 * *Files identical despite different names*

### Comparing `educommon-3.9.3/src/educommon/ws_log/report.py` & `educommon-3.9.4/src/educommon/ws_log/report.py`

 * *Files identical despite different names*

### Comparing `educommon-3.9.3/src/educommon/ws_log/smev/applications.py` & `educommon-3.9.4/src/educommon/ws_log/smev/applications.py`

 * *Files identical despite different names*

### Comparing `educommon-3.9.3/src/educommon/ws_log/smev/exceptions.py` & `educommon-3.9.4/src/educommon/ws_log/smev/exceptions.py`

 * *Files identical despite different names*

### Comparing `educommon-3.9.3/src/educommon/ws_log/templates/report/smev_logs.xlsx` & `educommon-3.9.4/src/educommon/ws_log/templates/report/smev_logs.xlsx`

 * *Files identical despite different names*

### Comparing `educommon-3.9.3/src/educommon/ws_log/templates/ui-js/smev-logs-list-window.js` & `educommon-3.9.4/src/educommon/ws_log/templates/ui-js/smev-logs-list-window.js`

 * *Files identical despite different names*

### Comparing `educommon-3.9.3/src/educommon/ws_log/templates/ui-js/smev-logs-report-setting-window.js` & `educommon-3.9.4/src/educommon/ws_log/templates/ui-js/smev-logs-report-setting-window.js`

 * *Files identical despite different names*

### Comparing `educommon-3.9.3/src/educommon/ws_log/ui.py` & `educommon-3.9.4/src/educommon/ws_log/ui.py`

 * *Files identical despite different names*

### Comparing `educommon-3.9.3/src/educommon/ws_log/utils.py` & `educommon-3.9.4/src/educommon/ws_log/utils.py`

 * *Files identical despite different names*

### Comparing `educommon-3.9.3/src/educommon.egg-info/PKG-INFO` & `educommon-3.9.4/src/educommon.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: educommon
-Version: 3.9.3
+Version: 3.9.4
 Summary: Общая кодовая база для проектов БЦ Образование
 Home-page: https://stash.bars-open.ru/projects/EDUBASE/repos/educommon
 Author: BARS Group
 Author-email: education_dev@bars-open.ru
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Web Environment
 Classifier: Natural Language :: Russian
```

### Comparing `educommon-3.9.3/src/educommon.egg-info/SOURCES.txt` & `educommon-3.9.4/src/educommon.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `educommon-3.9.3/tests/test_contingent_plugin_utils.py` & `educommon-3.9.4/tests/test_contingent_plugin_utils.py`

 * *Files identical despite different names*

### Comparing `educommon-3.9.3/tests/test_dates_splitter.py` & `educommon-3.9.4/tests/test_dates_splitter.py`

 * *Files identical despite different names*

### Comparing `educommon-3.9.3/tests/test_delete_check.py` & `educommon-3.9.4/tests/test_delete_check.py`

 * *Files identical despite different names*

### Comparing `educommon-3.9.3/tests/test_delete_objects.py` & `educommon-3.9.4/tests/test_delete_objects.py`

 * *Files identical despite different names*

### Comparing `educommon-3.9.3/tests/test_django_db_utils.py` & `educommon-3.9.4/tests/test_django_db_utils.py`

 * *Files identical despite different names*

### Comparing `educommon-3.9.3/tests/test_interval_mixins.py` & `educommon-3.9.4/tests/test_interval_mixins.py`

 * *Files identical despite different names*

### Comparing `educommon-3.9.3/tests/test_patches.py` & `educommon-3.9.4/tests/test_patches.py`

 * *Files identical despite different names*

### Comparing `educommon-3.9.3/tests/test_personal_data_fields.py` & `educommon-3.9.4/tests/test_personal_data_fields.py`

 * *Files identical despite different names*

### Comparing `educommon-3.9.3/tests/test_report.py` & `educommon-3.9.4/tests/test_report.py`

 * *Files identical despite different names*

### Comparing `educommon-3.9.3/tests/test_service_db_router.py` & `educommon-3.9.4/tests/test_service_db_router.py`

 * *Files identical despite different names*

### Comparing `educommon-3.9.3/tests/test_utils.py` & `educommon-3.9.4/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `educommon-3.9.3/tests/test_utils_plugins.py` & `educommon-3.9.4/tests/test_utils_plugins.py`

 * *Files identical despite different names*

### Comparing `educommon-3.9.3/tests/test_validators.py` & `educommon-3.9.4/tests/test_validators.py`

 * *Files identical despite different names*

### Comparing `educommon-3.9.3/tests/tests_rbac.py` & `educommon-3.9.4/tests/tests_rbac.py`

 * *Files identical despite different names*

