# Comparing `tmp/python-watcher-9.0.0.0rc1.tar.gz` & `tmp/python-watcher-9.0.0.0rc2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-watcher-9.0.0.0rc1.tar", last modified: Tue Sep 13 12:47:17 2022, max compression
+gzip compressed data, was "python-watcher-9.0.0.0rc2.tar", last modified: Tue Sep 27 15:24:05 2022, max compression
```

## Comparing `python-watcher-9.0.0.0rc1.tar` & `python-watcher-9.0.0.0rc2.tar`

### file list

```diff
@@ -1,984 +1,984 @@
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-09-13 12:47:17.348571 python-watcher-9.0.0.0rc1/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      181 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/.coveragerc
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       89 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/.mailmap
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       48 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/.stestr.conf
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6228 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/.zuul.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7369 2022-09-13 12:47:17.000000 python-watcher-9.0.0.0rc1/AUTHORS
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      540 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/CONTRIBUTING.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    56263 2022-09-13 12:47:16.000000 python-watcher-9.0.0.0rc1/ChangeLog
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      369 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/HACKING.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10143 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/LICENSE
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2421 2022-09-13 12:47:17.348571 python-watcher-9.0.0.0rc1/PKG-INFO
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1163 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/README.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-09-13 12:47:17.224571 python-watcher-9.0.0.0rc1/api-ref/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-09-13 12:47:17.240571 python-watcher-9.0.0.0rc1/api-ref/source/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2566 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/api-ref/source/conf.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      534 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/api-ref/source/index.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    14658 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/api-ref/source/parameters.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-09-13 12:47:17.244571 python-watcher-9.0.0.0rc1/api-ref/source/samples/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       96 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/api-ref/source/samples/actionplan-cancel-request-cancelling.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       95 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/api-ref/source/samples/actionplan-cancel-request-pending.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      990 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/api-ref/source/samples/actionplan-list-detailed-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      857 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/api-ref/source/samples/actionplan-list-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      695 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/api-ref/source/samples/actionplan-show-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      765 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/api-ref/source/samples/actionplan-start-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      999 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/api-ref/source/samples/actions-list-detailed-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      724 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/api-ref/source/samples/actions-list-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      783 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/api-ref/source/samples/actions-show-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      643 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/api-ref/source/samples/api-root-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1591 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/api-ref/source/samples/api-v1-root-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       95 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/api-ref/source/samples/audit-cancel-request.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1596 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/api-ref/source/samples/audit-cancel-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      366 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/api-ref/source/samples/audit-create-request-continuous.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      145 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/api-ref/source/samples/audit-create-request-oneshot.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1543 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/api-ref/source/samples/audit-create-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2057 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/api-ref/source/samples/audit-list-detailed-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      944 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/api-ref/source/samples/audit-list-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1598 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/api-ref/source/samples/audit-show-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      184 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/api-ref/source/samples/audit-update-request.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1596 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/api-ref/source/samples/audit-update-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      132 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/api-ref/source/samples/audittemplate-create-request-full.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       42 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/api-ref/source/samples/audittemplate-create-request-minimal.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      674 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/api-ref/source/samples/audittemplate-create-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      754 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/api-ref/source/samples/audittemplate-list-detailed-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      721 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/api-ref/source/samples/audittemplate-list-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      708 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/api-ref/source/samples/audittemplate-show-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       93 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/api-ref/source/samples/audittemplate-update-request.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      709 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/api-ref/source/samples/audittemplate-update-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1296 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/api-ref/source/samples/datamodel-list-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2163 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/api-ref/source/samples/goal-list-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      556 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/api-ref/source/samples/goal-show-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      654 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/api-ref/source/samples/scoring_engine-list-detailed-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      626 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/api-ref/source/samples/scoring_engine-list-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      491 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/api-ref/source/samples/scoring_engine-show-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      702 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/api-ref/source/samples/service-list-detailed-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      958 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/api-ref/source/samples/service-list-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      514 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/api-ref/source/samples/service-show-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1320 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/api-ref/source/samples/strategy-list-detailed-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      672 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/api-ref/source/samples/strategy-list-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      964 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/api-ref/source/samples/strategy-show-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1036 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/api-ref/source/samples/strategy-state-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5886 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/api-ref/source/watcher-api-v1-actionplans.inc
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3682 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/api-ref/source/watcher-api-v1-actions.inc
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7991 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/api-ref/source/watcher-api-v1-audits.inc
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5539 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/api-ref/source/watcher-api-v1-audittemplates.inc
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1159 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/api-ref/source/watcher-api-v1-datamodel.inc
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2483 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/api-ref/source/watcher-api-v1-goals.inc
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2581 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/api-ref/source/watcher-api-v1-scoring_engines.inc
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1982 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/api-ref/source/watcher-api-v1-services.inc
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3318 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/api-ref/source/watcher-api-v1-strategies.inc
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      327 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/api-ref/source/watcher-api-v1-webhooks.inc
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2054 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/api-ref/source/watcher-api-versions.inc
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-09-13 12:47:17.248571 python-watcher-9.0.0.0rc1/devstack/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-09-13 12:47:17.248571 python-watcher-9.0.0.0rc1/devstack/files/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1509 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/devstack/files/apache-watcher-api.template
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-09-13 12:47:17.248571 python-watcher-9.0.0.0rc1/devstack/lib/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    11762 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/devstack/lib/watcher
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1681 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/devstack/local.conf.compute
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1763 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/devstack/local.conf.controller
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      410 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/devstack/override-defaults
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1350 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/devstack/plugin.sh
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      248 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/devstack/settings
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-09-13 12:47:17.248571 python-watcher-9.0.0.0rc1/devstack/upgrade/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-09-13 12:47:17.248571 python-watcher-9.0.0.0rc1/devstack/upgrade/from_rocky/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      418 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/devstack/upgrade/from_rocky/upgrade-watcher
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)     3316 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/devstack/upgrade/resources.sh
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      818 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/devstack/upgrade/settings
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)      620 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/devstack/upgrade/shutdown.sh
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)     2485 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/devstack/upgrade/upgrade.sh
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-09-13 12:47:17.248571 python-watcher-9.0.0.0rc1/doc/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-09-13 12:47:17.248571 python-watcher-9.0.0.0rc1/doc/ext/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/doc/ext/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5324 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/doc/ext/term.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4243 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/doc/ext/versioned_notifications.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-09-13 12:47:17.252571 python-watcher-9.0.0.0rc1/doc/notification_samples/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1294 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/doc/notification_samples/action-cancel-end.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1708 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/doc/notification_samples/action-cancel-error.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1297 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/doc/notification_samples/action-cancel-start.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1264 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/doc/notification_samples/action-create.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1264 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/doc/notification_samples/action-delete.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1297 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/doc/notification_samples/action-execution-end.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1713 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/doc/notification_samples/action-execution-error.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1297 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/doc/notification_samples/action-execution-start.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1550 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/doc/notification_samples/action-update.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1873 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/doc/notification_samples/action_plan-cancel-end.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2301 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/doc/notification_samples/action_plan-cancel-error.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1876 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/doc/notification_samples/action_plan-cancel-start.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1860 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/doc/notification_samples/action_plan-create.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1874 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/doc/notification_samples/action_plan-delete.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1904 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/doc/notification_samples/action_plan-execution-end.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2329 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/doc/notification_samples/action_plan-execution-error.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1904 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/doc/notification_samples/action_plan-execution-start.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2164 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/doc/notification_samples/action_plan-update.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2269 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/doc/notification_samples/audit-create.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2269 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/doc/notification_samples/audit-delete.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2295 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/doc/notification_samples/audit-planner-end.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2710 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/doc/notification_samples/audit-planner-error.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2297 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/doc/notification_samples/audit-planner-start.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2296 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/doc/notification_samples/audit-strategy-end.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2711 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/doc/notification_samples/audit-strategy-error.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2298 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/doc/notification_samples/audit-strategy-start.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2554 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/doc/notification_samples/audit-update.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      593 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/doc/notification_samples/infra-optim-exception.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      908 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/doc/notification_samples/service-update.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      456 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/doc/requirements.txt
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-09-13 12:47:17.252571 python-watcher-9.0.0.0rc1/doc/source/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-09-13 12:47:17.252571 python-watcher-9.0.0.0rc1/doc/source/_static/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/doc/source/_static/.placeholder
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-09-13 12:47:17.252571 python-watcher-9.0.0.0rc1/doc/source/admin/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1415 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/doc/source/admin/apache-mod-wsgi.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1696 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/doc/source/admin/gmr.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      236 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/doc/source/admin/index.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4623 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/doc/source/admin/policy.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    19148 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/doc/source/architecture.rst
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)     4764 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/doc/source/conf.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-09-13 12:47:17.252571 python-watcher-9.0.0.0rc1/doc/source/configuration/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    16807 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/doc/source/configuration/configuring.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      117 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/doc/source/configuration/index.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      254 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/doc/source/configuration/watcher.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-09-13 12:47:17.252571 python-watcher-9.0.0.0rc1/doc/source/contributor/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       75 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/doc/source/contributor/api_microversion_history.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    11476 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/doc/source/contributor/concurrency.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4720 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/doc/source/contributor/contributing.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10531 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/doc/source/contributor/devstack.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7899 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/doc/source/contributor/environment.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      156 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/doc/source/contributor/index.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      339 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/doc/source/contributor/notifications.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-09-13 12:47:17.256571 python-watcher-9.0.0.0rc1/doc/source/contributor/plugin/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7796 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/doc/source/contributor/plugin/action-plugin.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3297 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/doc/source/contributor/plugin/base-setup.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9795 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/doc/source/contributor/plugin/cdmc-plugin.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7862 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/doc/source/contributor/plugin/goal-plugin.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      204 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/doc/source/contributor/plugin/index.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6113 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/doc/source/contributor/plugin/planner-plugin.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1388 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/doc/source/contributor/plugin/plugins.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7943 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/doc/source/contributor/plugin/scoring-engine-plugin.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    11870 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/doc/source/contributor/plugin/strategy-plugin.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       44 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/doc/source/contributor/rally_link.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1404 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/doc/source/contributor/testing.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-09-13 12:47:17.256571 python-watcher-9.0.0.0rc1/doc/source/datasources/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    17515 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/doc/source/datasources/grafana.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       72 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/doc/source/datasources/index.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    12056 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/doc/source/glossary.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-09-13 12:47:17.228571 python-watcher-9.0.0.0rc1/doc/source/image_src/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-09-13 12:47:17.256571 python-watcher-9.0.0.0rc1/doc/source/image_src/dia/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3198 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/doc/source/image_src/dia/architecture.dia
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3212 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/doc/source/image_src/dia/functional_data_model.dia
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-09-13 12:47:17.256571 python-watcher-9.0.0.0rc1/doc/source/image_src/plantuml/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      375 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/doc/source/image_src/plantuml/README.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1038 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/doc/source/image_src/plantuml/action_plan_state_machine.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      835 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/doc/source/image_src/plantuml/audit_state_machine.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1406 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/doc/source/image_src/plantuml/sequence_architecture_cdmc_sync.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      660 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/doc/source/image_src/plantuml/sequence_create_and_launch_audit.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      751 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/doc/source/image_src/plantuml/sequence_create_audit_template.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1622 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/doc/source/image_src/plantuml/sequence_from_audit_execution_to_actionplan_creation.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      553 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/doc/source/image_src/plantuml/sequence_launch_action_plan.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1367 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/doc/source/image_src/plantuml/sequence_launch_action_plan_in_applier.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1376 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/doc/source/image_src/plantuml/sequence_overview_watcher_usage.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1995 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/doc/source/image_src/plantuml/sequence_trigger_audit_in_decision_engine.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3537 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/doc/source/image_src/plantuml/watcher_db_schema_diagram.txt
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-09-13 12:47:17.260571 python-watcher-9.0.0.0rc1/doc/source/images/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    77970 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/doc/source/images/action_plan_state_machine.png
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    65012 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/doc/source/images/architecture.svg
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    46772 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/doc/source/images/audit_state_machine.png
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    87643 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/doc/source/images/functional_data_model.svg
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    46795 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/doc/source/images/sequence_architecture_cdmc_sync.png
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    33521 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/doc/source/images/sequence_create_and_launch_audit.png
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    30711 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/doc/source/images/sequence_create_audit_template.png
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    47585 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/doc/source/images/sequence_from_audit_execution_to_actionplan_creation.png
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    27899 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/doc/source/images/sequence_launch_action_plan.png
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    42190 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/doc/source/images/sequence_launch_action_plan_in_applier.png
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    46482 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/doc/source/images/sequence_overview_watcher_usage.png
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    73345 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/doc/source/images/sequence_trigger_audit_in_decision_engine.png
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    73815 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/doc/source/images/watcher_db_schema_diagram.png
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1906 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/doc/source/index.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-09-13 12:47:17.260571 python-watcher-9.0.0.0rc1/doc/source/install/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2577 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/doc/source/install/common_configure.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5458 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/doc/source/install/common_prerequisites.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1055 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/doc/source/install/get_started.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1295 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/doc/source/install/index.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1048 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/doc/source/install/install-rdo.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      918 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/doc/source/install/install-ubuntu.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      528 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/doc/source/install/install.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      178 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/doc/source/install/next-steps.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8019 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/doc/source/install/verify.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-09-13 12:47:17.260571 python-watcher-9.0.0.0rc1/doc/source/man/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      114 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/doc/source/man/footer.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2397 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/doc/source/man/general-options.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      204 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/doc/source/man/index.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      569 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/doc/source/man/watcher-api.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      594 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/doc/source/man/watcher-applier.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6589 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/doc/source/man/watcher-db-manage.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      674 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/doc/source/man/watcher-decision-engine.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2068 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/doc/source/man/watcher-status.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-09-13 12:47:17.264571 python-watcher-9.0.0.0rc1/doc/source/strategies/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2141 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/doc/source/strategies/actuation.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3263 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/doc/source/strategies/basic-server-consolidation.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2150 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/doc/source/strategies/host_maintenance.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       70 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/doc/source/strategies/index.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2291 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/doc/source/strategies/node_resource_consolidation.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2443 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/doc/source/strategies/noisy_neighbor.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2784 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/doc/source/strategies/outlet_temp_control.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2616 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/doc/source/strategies/saving_energy.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1893 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/doc/source/strategies/storage_capacity_balance.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2819 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/doc/source/strategies/strategy-template.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3212 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/doc/source/strategies/uniform_airflow.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3155 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/doc/source/strategies/vm_workload_consolidation.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6025 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/doc/source/strategies/workload-stabilization.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2782 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/doc/source/strategies/workload_balance.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5428 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/doc/source/strategies/zone_migration.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-09-13 12:47:17.264571 python-watcher-9.0.0.0rc1/doc/source/user/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    12578 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/doc/source/user/event_type_audit.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      117 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/doc/source/user/index.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5981 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/doc/source/user/user-guide.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4427 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/doc/source/user/ways-to-install.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-09-13 12:47:17.228571 python-watcher-9.0.0.0rc1/etc/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-09-13 12:47:17.264571 python-watcher-9.0.0.0rc1/etc/apache2/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1190 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/etc/apache2/watcher
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-09-13 12:47:17.264571 python-watcher-9.0.0.0rc1/etc/watcher/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      131 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/etc/watcher/README-watcher.conf.txt
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-09-13 12:47:17.264571 python-watcher-9.0.0.0rc1/etc/watcher/oslo-config-generator/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      406 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/etc/watcher/oslo-config-generator/watcher.conf
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-09-13 12:47:17.264571 python-watcher-9.0.0.0rc1/etc/watcher/oslo-policy-generator/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       76 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/etc/watcher/oslo-policy-generator/watcher-policy-generator.conf
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-09-13 12:47:17.264571 python-watcher-9.0.0.0rc1/python_watcher.egg-info/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2421 2022-09-13 12:47:17.000000 python-watcher-9.0.0.0rc1/python_watcher.egg-info/PKG-INFO
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    41188 2022-09-13 12:47:17.000000 python-watcher-9.0.0.0rc1/python_watcher.egg-info/SOURCES.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2022-09-13 12:47:17.000000 python-watcher-9.0.0.0rc1/python_watcher.egg-info/dependency_links.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4397 2022-09-13 12:47:17.000000 python-watcher-9.0.0.0rc1/python_watcher.egg-info/entry_points.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2022-09-13 12:47:17.000000 python-watcher-9.0.0.0rc1/python_watcher.egg-info/not-zip-safe
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       47 2022-09-13 12:47:17.000000 python-watcher-9.0.0.0rc1/python_watcher.egg-info/pbr.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      917 2022-09-13 12:47:17.000000 python-watcher-9.0.0.0rc1/python_watcher.egg-info/requires.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        8 2022-09-13 12:47:17.000000 python-watcher-9.0.0.0rc1/python_watcher.egg-info/top_level.txt
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-09-13 12:47:17.264571 python-watcher-9.0.0.0rc1/rally-jobs/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1421 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/rally-jobs/README.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1370 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/rally-jobs/watcher-watcher.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-09-13 12:47:17.228571 python-watcher-9.0.0.0rc1/releasenotes/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-09-13 12:47:17.276571 python-watcher-9.0.0.0rc1/releasenotes/notes/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/releasenotes/notes/.placeholder
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       63 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/releasenotes/notes/action-plan-cancel-c54726378019e096.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       67 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/releasenotes/notes/action-plan-versioned-notifications-api-e8ca4f5d37aa5b4b.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       62 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/releasenotes/notes/action-versioned-notifications-api-ff94fc0f401292d0.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       93 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/releasenotes/notes/add-baremetal-scoper-9ef23f5fb8f0be6a.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      279 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/releasenotes/notes/add-force-field-to-audit-4bcaeedfe27233ad.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      322 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/releasenotes/notes/add-ha-support-b9042255e5b76e42.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      129 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/releasenotes/notes/add-name-for-audit-0df1f39f00736f06.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      274 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/releasenotes/notes/add-plugins-parameters-376eb6b0b8978b44.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       59 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/releasenotes/notes/add-power-on-off-a77673d482568a8b.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      266 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/releasenotes/notes/add-scoring-module-fa00d013ed2d614e.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      156 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/releasenotes/notes/add-start-end-time-for-continuous-audit-52c45052cb06d153.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      472 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/releasenotes/notes/add-upgrade-check-framework-5bb9693c8a78931c.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      416 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/releasenotes/notes/api-call-retry-fef741ac684c58dd.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      432 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/releasenotes/notes/api-microversioning-7999a3ee8073bf32.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      165 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/releasenotes/notes/audit-scoper-for-storage-data-model-cdccc803542d22db.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      262 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/releasenotes/notes/audit-tag-vm-metadata-47a3e4468748853c.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       61 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/releasenotes/notes/audit-versioned-notifications-api-bca7738e16954bad.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      205 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/releasenotes/notes/automatic-triggering-audit-8a9b0540d547db60.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      148 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/releasenotes/notes/background-jobs-ha-9d3cf3fe356f4705.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      221 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/releasenotes/notes/bp-audit-scope-exclude-project-511a7720aac00dff.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       61 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/releasenotes/notes/build-baremetal-data-model-in-watcher-3023453a47b61dab.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      231 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/releasenotes/notes/cdm-scoping-8d9c307bad46bfa1.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       68 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/releasenotes/notes/centralise-config-opts-95670987dfbdb0e7.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      284 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/releasenotes/notes/change-ram-util-metric-4a3e6984b9dd968d.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      264 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/releasenotes/notes/check-strategy-requirements-66f9e9262412f8ec.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       56 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/releasenotes/notes/cinder-model-integration-baa394a72a0a33bf.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      183 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/releasenotes/notes/cluster-model-objects-wrapper-9c799ea262c56a5b.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      190 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/releasenotes/notes/compute-cdm-include-all-instances-f7506ded2d57732f.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      118 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/releasenotes/notes/configurable-weights-default-planner-3746b33160bc7347.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      898 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/releasenotes/notes/consume-nova-versioned-notifications-f98361b37e546b4d.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      121 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/releasenotes/notes/continuously-optimization-35364f4d2c0b81fc.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      363 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/releasenotes/notes/cron-based-continuous-audits-c3eedf28d9752b37.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      764 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/releasenotes/notes/datasource-query-retry-00cba5f7e68aec39.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       74 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/releasenotes/notes/db-migration-e1a705a8b54ccdd2.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      220 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/releasenotes/notes/define-the-audit-scope-e89edc5051dcf3f2.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      305 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/releasenotes/notes/deprecate-ceilometer-datasource-446b0be70fbce28b.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1008 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/releasenotes/notes/deprecate-json-formatted-policy-file-3a92379e9f5dd203.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      199 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/releasenotes/notes/drop-py-2-7-54f8e806d71f19a7.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      123 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/releasenotes/notes/dynamic-action-description-0e947b9e7ef2a134.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      112 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/releasenotes/notes/efficacy-indicator-95380ad7b84e3be2.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      824 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/releasenotes/notes/enhance-watcher-applier-engine-86c676ce8f179e68.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      318 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/releasenotes/notes/event-driven-optimization-based-4870f112bef8a560.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      576 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/releasenotes/notes/file-based-metric-map-c2af62b5067895df.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      782 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/releasenotes/notes/formal-datasource-interface-implementation-222769d55a127d33.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1024 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/releasenotes/notes/general-purpose-decision-engine-threadpool-0711b23abfc9d409.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      170 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/releasenotes/notes/get-goal-from-strategy-396c9b13a38bb650.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      391 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/releasenotes/notes/global-datasource-preference-3ab47b4be09ff3a5.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      146 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/releasenotes/notes/gnocchi-watcher-43c25d391fbd3e9c.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      547 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/releasenotes/notes/grafana-datasource-b672367c23ffa0c6.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      266 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/releasenotes/notes/graph-based-cluster-model-523937a6f5e66537.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      365 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/releasenotes/notes/host-maintenance-strategy-41f640927948fb56.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      957 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/releasenotes/notes/improve-compute-data-model-b427c85e4ed2b6fb.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       87 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/releasenotes/notes/jsonschema-validation-79cab05d5295da00.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      272 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/releasenotes/notes/min-required-nova-train-71f124192d88ae52.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      102 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/releasenotes/notes/monasca-support-0b0486b8572ac38b.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      267 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/releasenotes/notes/multiple-global-efficacy-indicator-fc11c4844a12a7d5.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      245 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/releasenotes/notes/node-resource-consolidation-73bc0c0abfeb0b03.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      196 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/releasenotes/notes/noisy-neighbor-strategy-a71342740b59dddc.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      155 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/releasenotes/notes/notifications-actionplan-cancel-edb2a4a12543e2d0.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      182 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/releasenotes/notes/optimization-threshold-21ad38f0470d0e1a.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      127 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/releasenotes/notes/persistent-audit-parameters-ae41dd7252ba9672.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      142 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/releasenotes/notes/planner-storage-action-plan-26ef37893c5e8648.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      126 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/releasenotes/notes/remove-nova-legacy-notifications-e1b6d10eff58f30a.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      519 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/releasenotes/notes/replace-cold-migrate-to-use-nova-migration-api-cecd9a39ddd3bc58.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      221 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/releasenotes/notes/scope-for-data-model-ea9792f90db14343.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       63 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/releasenotes/notes/service-versioned-notifications-api-70367b79a565d900.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      578 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/releasenotes/notes/show-datamodel-api-6945b744fd5d25d5.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      118 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/releasenotes/notes/stale-action-plan-b6a6b08df873c128.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      246 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/releasenotes/notes/standard-deviation-strategy-cd1d0c443fdfde9c.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       65 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/releasenotes/notes/storage-workload-balance-0ecabbc1791e6894.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      168 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/releasenotes/notes/support-keystoneclient-option-b30d1ff45f86a2e7.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      380 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/releasenotes/notes/support-placement-api-58ce6bef1bbbe98a.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       52 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/releasenotes/notes/suspended-audit-state-07f998c94e9d9a47.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      154 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/releasenotes/notes/uniform-airflow-strategy-68cdba1419c3f770.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      427 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/releasenotes/notes/uwsgi-support-8dcea6961e56dad0.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       52 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/releasenotes/notes/volume-migrate-action-fc57b0ce0e4c39ae.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      473 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/releasenotes/notes/watcher-notifications-ovo-7b44d52ef6400dd0.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      153 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/releasenotes/notes/watcher-planner-selector-84d77549d46f362a.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       82 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/releasenotes/notes/watcher-policies-1e86a30f0f11c6fa.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       69 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/releasenotes/notes/watcher-service-list-7b2f4b64f71e9b89.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      183 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/releasenotes/notes/watcher-versioned-objects-fc5abf5c81c4590c.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      241 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/releasenotes/notes/workload-balance-base-on-cpu-or-ram-util-3ff4ee968c32b2ed.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      265 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/releasenotes/notes/workload-balance-migration-strategy-a0b05148a57815c0.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      200 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/releasenotes/notes/zone-migration-strategy-10f7656a2a01e607.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-09-13 12:47:17.280571 python-watcher-9.0.0.0rc1/releasenotes/source/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-09-13 12:47:17.280571 python-watcher-9.0.0.0rc1/releasenotes/source/_static/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/releasenotes/source/_static/.placeholder
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8395 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/releasenotes/source/conf.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      902 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/releasenotes/source/index.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-09-13 12:47:17.228571 python-watcher-9.0.0.0rc1/releasenotes/source/locale/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-09-13 12:47:17.228571 python-watcher-9.0.0.0rc1/releasenotes/source/locale/en_GB/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-09-13 12:47:17.280571 python-watcher-9.0.0.0rc1/releasenotes/source/locale/en_GB/LC_MESSAGES/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    45874 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/releasenotes/source/locale/en_GB/LC_MESSAGES/releasenotes.po
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-09-13 12:47:17.228571 python-watcher-9.0.0.0rc1/releasenotes/source/locale/fr/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-09-13 12:47:17.280571 python-watcher-9.0.0.0rc1/releasenotes/source/locale/fr/LC_MESSAGES/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      914 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/releasenotes/source/locale/fr/LC_MESSAGES/releasenotes.po
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      154 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/releasenotes/source/newton.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      152 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/releasenotes/source/ocata.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      143 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/releasenotes/source/pike.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      147 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/releasenotes/source/queens.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      145 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/releasenotes/source/rocky.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      145 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/releasenotes/source/stein.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      126 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/releasenotes/source/train.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      112 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/releasenotes/source/unreleased.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      130 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/releasenotes/source/ussuri.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      138 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/releasenotes/source/victoria.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      134 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/releasenotes/source/wallaby.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      122 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/releasenotes/source/xena.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      122 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/releasenotes/source/yoga.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1620 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/requirements.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5423 2022-09-13 12:47:17.348571 python-watcher-9.0.0.0rc1/setup.cfg
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      697 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/setup.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      527 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/test-requirements.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3808 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/tox.ini
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-09-13 12:47:17.280571 python-watcher-9.0.0.0rc1/watcher/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      640 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1295 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/_i18n.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-09-13 12:47:17.280571 python-watcher-9.0.0.0rc1/watcher/api/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/api/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1474 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/api/acl.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1660 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/api/app.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      906 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/api/app.wsgi
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1631 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/api/config.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-09-13 12:47:17.280571 python-watcher-9.0.0.0rc1/watcher/api/controllers/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/api/controllers/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4397 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/api/controllers/base.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2035 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/api/controllers/link.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1026 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/api/controllers/rest_api_version_history.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3650 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/api/controllers/root.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-09-13 12:47:17.284571 python-watcher-9.0.0.0rc1/watcher/api/controllers/v1/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10926 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/api/controllers/v1/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    16676 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/api/controllers/v1/action.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    23842 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/api/controllers/v1/action_plan.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    28050 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/api/controllers/v1/audit.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    28005 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/api/controllers/v1/audit_template.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1756 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/api/controllers/v1/collection.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2661 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/api/controllers/v1/data_model.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2719 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/api/controllers/v1/efficacy_indicator.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8924 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/api/controllers/v1/goal.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9262 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/api/controllers/v1/scoring_engine.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9645 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/api/controllers/v1/service.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    12595 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/api/controllers/v1/strategy.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6526 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/api/controllers/v1/types.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6112 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/api/controllers/v1/utils.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1827 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/api/controllers/v1/versions.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2215 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/api/controllers/v1/webhooks.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3984 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/api/hooks.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-09-13 12:47:17.284571 python-watcher-9.0.0.0rc1/watcher/api/middleware/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/api/middleware/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2104 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/api/middleware/auth_token.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3814 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/api/middleware/parsable_error.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5283 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/api/scheduling.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1269 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/api/wsgi.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-09-13 12:47:17.284571 python-watcher-9.0.0.0rc1/watcher/applier/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/applier/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-09-13 12:47:17.284571 python-watcher-9.0.0.0rc1/watcher/applier/action_plan/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/applier/action_plan/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      820 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/applier/action_plan/base.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4286 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/applier/action_plan/default.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-09-13 12:47:17.284571 python-watcher-9.0.0.0rc1/watcher/applier/actions/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/applier/actions/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4876 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/applier/actions/base.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4047 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/applier/actions/change_node_power_state.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4484 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/applier/actions/change_nova_service_state.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1568 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/applier/actions/factory.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7989 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/applier/actions/migration.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1877 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/applier/actions/nop.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3379 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/applier/actions/resize.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2024 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/applier/actions/sleep.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8523 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/applier/actions/volume_migration.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1073 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/applier/base.py
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)     2093 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/applier/default.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-09-13 12:47:17.284571 python-watcher-9.0.0.0rc1/watcher/applier/loading/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/applier/loading/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      946 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/applier/loading/default.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1446 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/applier/manager.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-09-13 12:47:17.284571 python-watcher-9.0.0.0rc1/watcher/applier/messaging/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/applier/messaging/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1728 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/applier/messaging/trigger.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1894 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/applier/rpcapi.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3020 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/applier/sync.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-09-13 12:47:17.288571 python-watcher-9.0.0.0rc1/watcher/applier/workflow_engine/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/applier/workflow_engine/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    12117 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/applier/workflow_engine/base.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7890 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/applier/workflow_engine/default.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-09-13 12:47:17.288571 python-watcher-9.0.0.0rc1/watcher/cmd/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1228 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/cmd/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1733 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/cmd/api.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1335 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/cmd/applier.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5369 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/cmd/dbmanage.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1626 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/cmd/decisionengine.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1829 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/cmd/status.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1059 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/cmd/sync.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-09-13 12:47:17.288571 python-watcher-9.0.0.0rc1/watcher/common/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/common/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9599 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/common/cinder_helper.py
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)    12032 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/common/clients.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1465 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/common/config.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4555 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/common/context.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    14304 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/common/exception.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1609 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/common/ironic_helper.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4487 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/common/keystone_helper.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-09-13 12:47:17.292571 python-watcher-9.0.0.0rc1/watcher/common/loader/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/common/loader/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      842 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/common/loader/base.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3076 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/common/loader/default.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2224 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/common/loader/loadable.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    29807 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/common/nova_helper.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1178 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/common/paths.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6652 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/common/placement_helper.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-09-13 12:47:17.292571 python-watcher-9.0.0.0rc1/watcher/common/policies/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1384 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/common/policies/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1617 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/common/policies/action.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2597 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/common/policies/action_plan.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2434 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/common/policies/audit.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2654 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/common/policies/audit_template.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      938 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/common/policies/base.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1052 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/common/policies/data_model.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1551 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/common/policies/goal.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2136 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/common/policies/scoring_engine.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1577 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/common/policies/service.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1904 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/common/policies/strategy.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5250 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/common/policy.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4410 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/common/rpc.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2145 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/common/scheduling.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9715 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/common/service.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1337 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/common/service_manager.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4758 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/common/utils.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-09-13 12:47:17.296571 python-watcher-9.0.0.0rc1/watcher/conf/
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)     2340 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/conf/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2792 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/conf/api.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2207 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/conf/applier.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2503 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/conf/ceilometer_client.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1593 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/conf/cinder_client.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1085 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/conf/clients_auth.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1753 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/conf/collector.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2225 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/conf/datasources.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1344 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/conf/db.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4056 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/conf/decision_engine.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      989 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/conf/exception.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1593 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/conf/glance_client.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1581 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/conf/gnocchi_client.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6746 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/conf/grafana_client.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1651 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/conf/grafana_translators.py
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)     1589 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/conf/ironic_client.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1349 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/conf/keystone_client.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1596 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/conf/monasca_client.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1608 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/conf/neutron_client.py
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)     1923 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/conf/nova_client.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2547 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/conf/opts.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1774 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/conf/paths.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1513 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/conf/placement_client.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1305 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/conf/planner.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2426 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/conf/plugins.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1593 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/conf/service.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-09-13 12:47:17.296571 python-watcher-9.0.0.0rc1/watcher/db/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/db/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    32292 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/db/api.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1636 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/db/migration.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    16858 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/db/purge.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-09-13 12:47:17.296571 python-watcher-9.0.0.0rc1/watcher/db/sqlalchemy/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/db/sqlalchemy/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-09-13 12:47:17.296571 python-watcher-9.0.0.0rc1/watcher/db/sqlalchemy/alembic/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1942 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/db/sqlalchemy/alembic/README.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1769 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/db/sqlalchemy/alembic/env.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      412 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/db/sqlalchemy/alembic/script.py.mako
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-09-13 12:47:17.296571 python-watcher-9.0.0.0rc1/watcher/db/sqlalchemy/alembic/versions/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9500 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/db/sqlalchemy/alembic/versions/001_ocata.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1172 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/db/sqlalchemy/alembic/versions/0f6042416884_add_apscheduler_jobs.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      420 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/db/sqlalchemy/alembic/versions/3cfc94cecf4e_add_name_for_audit.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      547 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/db/sqlalchemy/alembic/versions/4b16194c56bc_add_start_end_time.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      583 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/db/sqlalchemy/alembic/versions/52804f2498c4_add_hostname.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      409 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/db/sqlalchemy/alembic/versions/609bec748f2a_add_force_field.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1342 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/db/sqlalchemy/alembic/versions/a86240e89a29_.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      673 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/db/sqlalchemy/alembic/versions/d098df6021e2_cron_support_for_audit.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1076 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/db/sqlalchemy/alembic/versions/d09a5945e4a0_add_action_description_table.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      975 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/db/sqlalchemy/alembic.ini
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    44089 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/db/sqlalchemy/api.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4441 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/db/sqlalchemy/job_store.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3676 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/db/sqlalchemy/migration.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10945 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/db/sqlalchemy/models.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-09-13 12:47:17.300571 python-watcher-9.0.0.0rc1/watcher/decision_engine/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/decision_engine/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-09-13 12:47:17.300571 python-watcher-9.0.0.0rc1/watcher/decision_engine/audit/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/decision_engine/audit/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5669 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/decision_engine/audit/base.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9490 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/decision_engine/audit/continuous.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1049 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/decision_engine/audit/event.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1046 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/decision_engine/audit/oneshot.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-09-13 12:47:17.300571 python-watcher-9.0.0.0rc1/watcher/decision_engine/datasources/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/decision_engine/datasources/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9376 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/decision_engine/datasources/base.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10668 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/decision_engine/datasources/ceilometer.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8788 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/decision_engine/datasources/gnocchi.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10217 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/decision_engine/datasources/grafana.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-09-13 12:47:17.300571 python-watcher-9.0.0.0rc1/watcher/decision_engine/datasources/grafana_translator/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/decision_engine/datasources/grafana_translator/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4554 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/decision_engine/datasources/grafana_translator/base.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3240 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/decision_engine/datasources/grafana_translator/influxdb.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5680 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/decision_engine/datasources/manager.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6950 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/decision_engine/datasources/monasca.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1504 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/decision_engine/gmr.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-09-13 12:47:17.300571 python-watcher-9.0.0.0rc1/watcher/decision_engine/goal/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1189 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/decision_engine/goal/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2011 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/decision_engine/goal/base.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-09-13 12:47:17.300571 python-watcher-9.0.0.0rc1/watcher/decision_engine/goal/efficacy/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/decision_engine/goal/efficacy/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3135 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/decision_engine/goal/efficacy/base.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8243 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/decision_engine/goal/efficacy/indicators.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6016 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/decision_engine/goal/efficacy/specs.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6789 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/decision_engine/goal/goals.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-09-13 12:47:17.300571 python-watcher-9.0.0.0rc1/watcher/decision_engine/loading/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/decision_engine/loading/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1928 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/decision_engine/loading/default.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2901 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/decision_engine/manager.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-09-13 12:47:17.300571 python-watcher-9.0.0.0rc1/watcher/decision_engine/messaging/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/decision_engine/messaging/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2144 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/decision_engine/messaging/audit_endpoint.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2180 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/decision_engine/messaging/data_model_endpoint.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-09-13 12:47:17.300571 python-watcher-9.0.0.0rc1/watcher/decision_engine/model/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/decision_engine/model/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1131 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/decision_engine/model/base.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-09-13 12:47:17.304571 python-watcher-9.0.0.0rc1/watcher/decision_engine/model/collector/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/decision_engine/model/collector/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9607 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/decision_engine/model/collector/base.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    11683 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/decision_engine/model/collector/cinder.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4037 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/decision_engine/model/collector/ironic.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2327 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/decision_engine/model/collector/manager.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    21542 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/decision_engine/model/collector/nova.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-09-13 12:47:17.304571 python-watcher-9.0.0.0rc1/watcher/decision_engine/model/element/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1320 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/decision_engine/model/element/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      924 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/decision_engine/model/element/baremetal_resource.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2063 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/decision_engine/model/element/base.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      860 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/decision_engine/model/element/compute_resource.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2162 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/decision_engine/model/element/instance.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3777 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/decision_engine/model/element/node.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      928 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/decision_engine/model/element/storage_resource.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1856 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/decision_engine/model/element/volume.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    23973 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/decision_engine/model/model_root.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-09-13 12:47:17.304571 python-watcher-9.0.0.0rc1/watcher/decision_engine/model/notification/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/decision_engine/model/notification/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1108 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/decision_engine/model/notification/base.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    14150 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/decision_engine/model/notification/cinder.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2887 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/decision_engine/model/notification/filtering.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    14709 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/decision_engine/model/notification/nova.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-09-13 12:47:17.304571 python-watcher-9.0.0.0rc1/watcher/decision_engine/planner/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/decision_engine/planner/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3069 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/decision_engine/planner/base.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1026 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/decision_engine/planner/manager.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5916 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/decision_engine/planner/node_resource_consolidation.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8282 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/decision_engine/planner/weight.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    11192 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/decision_engine/planner/workload_stabilization.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2286 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/decision_engine/rpcapi.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4349 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/decision_engine/scheduling.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-09-13 12:47:17.304571 python-watcher-9.0.0.0rc1/watcher/decision_engine/scope/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/decision_engine/scope/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2182 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/decision_engine/scope/baremetal.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1192 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/decision_engine/scope/base.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9321 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/decision_engine/scope/compute.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6418 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/decision_engine/scope/storage.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-09-13 12:47:17.308571 python-watcher-9.0.0.0rc1/watcher/decision_engine/scoring/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/decision_engine/scoring/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4341 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/decision_engine/scoring/base.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6519 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/decision_engine/scoring/dummy_scorer.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3400 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/decision_engine/scoring/dummy_scoring_container.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3663 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/decision_engine/scoring/scoring_factory.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-09-13 12:47:17.308571 python-watcher-9.0.0.0rc1/watcher/decision_engine/solution/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/decision_engine/solution/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4705 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/decision_engine/solution/base.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2480 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/decision_engine/solution/default.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3636 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/decision_engine/solution/efficacy.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      832 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/decision_engine/solution/solution_comparator.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      830 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/decision_engine/solution/solution_evaluator.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-09-13 12:47:17.308571 python-watcher-9.0.0.0rc1/watcher/decision_engine/strategy/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/decision_engine/strategy/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-09-13 12:47:17.308571 python-watcher-9.0.0.0rc1/watcher/decision_engine/strategy/common/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/decision_engine/strategy/common/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      822 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/decision_engine/strategy/common/level.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-09-13 12:47:17.308571 python-watcher-9.0.0.0rc1/watcher/decision_engine/strategy/context/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/decision_engine/strategy/context/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2654 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/decision_engine/strategy/context/base.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2591 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/decision_engine/strategy/context/default.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-09-13 12:47:17.308571 python-watcher-9.0.0.0rc1/watcher/decision_engine/strategy/selection/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/decision_engine/strategy/selection/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      810 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/decision_engine/strategy/selection/base.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2756 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/decision_engine/strategy/selection/default.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-09-13 12:47:17.312571 python-watcher-9.0.0.0rc1/watcher/decision_engine/strategy/strategies/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3053 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/decision_engine/strategy/strategies/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3009 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/decision_engine/strategy/strategies/actuation.py
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)    18295 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/decision_engine/strategy/strategies/base.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    18447 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/decision_engine/strategy/strategies/basic_consolidation.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2858 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/decision_engine/strategy/strategies/dummy_strategy.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3601 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/decision_engine/strategy/strategies/dummy_with_resize.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6266 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/decision_engine/strategy/strategies/dummy_with_scorer.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    11550 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/decision_engine/strategy/strategies/host_maintenance.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    11292 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/decision_engine/strategy/strategies/node_resource_consolidation.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9922 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/decision_engine/strategy/strategies/noisy_neighbor.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    11010 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/decision_engine/strategy/strategies/outlet_temp_control.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8734 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/decision_engine/strategy/strategies/saving_energy.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    15669 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/decision_engine/strategy/strategies/storage_capacity_balance.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    13390 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/decision_engine/strategy/strategies/uniform_airflow.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    23147 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/decision_engine/strategy/strategies/vm_workload_consolidation.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    14332 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/decision_engine/strategy/strategies/workload_balance.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    24902 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/decision_engine/strategy/strategies/workload_stabilization.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    33189 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/decision_engine/strategy/strategies/zone_migration.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    25320 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/decision_engine/sync.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3811 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/decision_engine/threading.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-09-13 12:47:17.312571 python-watcher-9.0.0.0rc1/watcher/hacking/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/hacking/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10378 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/hacking/checks.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-09-13 12:47:17.232571 python-watcher-9.0.0.0rc1/watcher/locale/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-09-13 12:47:17.232571 python-watcher-9.0.0.0rc1/watcher/locale/de/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-09-13 12:47:17.312571 python-watcher-9.0.0.0rc1/watcher/locale/de/LC_MESSAGES/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    26447 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/locale/de/LC_MESSAGES/watcher.po
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-09-13 12:47:17.232571 python-watcher-9.0.0.0rc1/watcher/locale/en_GB/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-09-13 12:47:17.312571 python-watcher-9.0.0.0rc1/watcher/locale/en_GB/LC_MESSAGES/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    26943 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/locale/en_GB/LC_MESSAGES/watcher.po
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-09-13 12:47:17.312571 python-watcher-9.0.0.0rc1/watcher/notifications/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1278 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/notifications/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    11699 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/notifications/action.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    13581 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/notifications/action_plan.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    12071 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/notifications/audit.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8094 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/notifications/base.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1990 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/notifications/exception.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1843 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/notifications/goal.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3885 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/notifications/service.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1877 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/notifications/strategy.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-09-13 12:47:17.316571 python-watcher-9.0.0.0rc1/watcher/objects/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1632 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/objects/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6945 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/objects/action.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5536 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/objects/action_description.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    13441 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/objects/action_plan.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    14365 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/objects/audit.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10374 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/objects/audit_template.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6546 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/objects/base.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7588 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/objects/efficacy_indicator.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4747 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/objects/fields.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6773 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/objects/goal.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8450 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/objects/scoring_engine.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5415 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/objects/service.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10140 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/objects/strategy.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-09-13 12:47:17.316571 python-watcher-9.0.0.0rc1/watcher/tests/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      962 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/tests/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-09-13 12:47:17.316571 python-watcher-9.0.0.0rc1/watcher/tests/api/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/tests/api/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    11971 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/tests/api/base.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1197 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/tests/api/test_base.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1369 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/tests/api/test_config.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10476 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/tests/api/test_hooks.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2830 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/tests/api/test_root.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5128 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/tests/api/test_scheduling.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1999 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/tests/api/test_utils.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3738 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/tests/api/utils.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-09-13 12:47:17.320571 python-watcher-9.0.0.0rc1/watcher/tests/api/v1/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/tests/api/v1/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    23438 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/tests/api/v1/test_actions.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    29901 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/tests/api/v1/test_actions_plans.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    38337 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/tests/api/v1/test_audit_templates.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    49443 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/tests/api/v1/test_audits.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3250 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/tests/api/v1/test_data_model.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7335 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/tests/api/v1/test_goals.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4998 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/tests/api/v1/test_microversions.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      702 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/tests/api/v1/test_root.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8033 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/tests/api/v1/test_scoring_engines.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8084 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/tests/api/v1/test_services.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    12214 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/tests/api/v1/test_strategies.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9313 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/tests/api/v1/test_types.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2219 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/tests/api/v1/test_utils.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3148 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/tests/api/v1/test_webhooks.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-09-13 12:47:17.320571 python-watcher-9.0.0.0rc1/watcher/tests/applier/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/tests/applier/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-09-13 12:47:17.320571 python-watcher-9.0.0.0rc1/watcher/tests/applier/action_plan/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/tests/applier/action_plan/__init__.py
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)     5488 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/tests/applier/action_plan/test_default_action_handler.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-09-13 12:47:17.320571 python-watcher-9.0.0.0rc1/watcher/tests/applier/actions/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/tests/applier/actions/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-09-13 12:47:17.320571 python-watcher-9.0.0.0rc1/watcher/tests/applier/actions/loading/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/tests/applier/actions/loading/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1109 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/tests/applier/actions/loading/test_default_actions_loader.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6267 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/tests/applier/actions/test_change_node_power_state.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5154 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/tests/applier/actions/test_change_nova_service_state.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8654 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/tests/applier/actions/test_migration.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3470 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/tests/applier/actions/test_resize.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1637 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/tests/applier/actions/test_sleep.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8973 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/tests/applier/actions/test_volume_migration.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-09-13 12:47:17.320571 python-watcher-9.0.0.0rc1/watcher/tests/applier/messaging/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/tests/applier/messaging/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1351 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/tests/applier/messaging/test_trigger_action_plan_endpoint.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1527 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/tests/applier/test_applier_manager.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1968 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/tests/applier/test_rpcapi.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3402 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/tests/applier/test_sync.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-09-13 12:47:17.320571 python-watcher-9.0.0.0rc1/watcher/tests/applier/workflow_engine/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/tests/applier/workflow_engine/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-09-13 12:47:17.320571 python-watcher-9.0.0.0rc1/watcher/tests/applier/workflow_engine/loading/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/tests/applier/workflow_engine/loading/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1159 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/tests/applier/workflow_engine/loading/test_default_engine_loader.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    16567 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/tests/applier/workflow_engine/test_default_workflow_engine.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6774 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/tests/applier/workflow_engine/test_taskflow_action_container.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4740 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/tests/base.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-09-13 12:47:17.320571 python-watcher-9.0.0.0rc1/watcher/tests/cmd/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/tests/cmd/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2199 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/tests/cmd/test_api.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1803 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/tests/cmd/test_applier.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7477 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/tests/cmd/test_db_manage.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2114 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/tests/cmd/test_decision_engine.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1586 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/tests/cmd/test_status.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-09-13 12:47:17.324571 python-watcher-9.0.0.0rc1/watcher/tests/common/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/tests/common/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-09-13 12:47:17.324571 python-watcher-9.0.0.0rc1/watcher/tests/common/loader/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/tests/common/loader/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3612 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/tests/common/loader/test_loader.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    16716 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/tests/common/test_cinder_helper.py
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)    17818 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/tests/common/test_clients.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2162 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/tests/common/test_ironic_helper.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    28524 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/tests/common/test_nova_helper.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    11761 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/tests/common/test_placement_helper.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3533 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/tests/common/test_service.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-09-13 12:47:17.324571 python-watcher-9.0.0.0rc1/watcher/tests/conf/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/tests/conf/__init__.py
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)     7028 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/tests/conf/test_list_opts.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1794 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/tests/conf_fixture.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1068 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/tests/config.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-09-13 12:47:17.324571 python-watcher-9.0.0.0rc1/watcher/tests/db/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/tests/db/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2588 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/tests/db/base.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    15255 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/tests/db/test_action.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    11274 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/tests/db/test_action_description.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    15616 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/tests/db/test_action_plan.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    16749 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/tests/db/test_audit.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    16525 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/tests/db/test_audit_template.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    17420 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/tests/db/test_efficacy_indicator.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    12103 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/tests/db/test_goal.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    23464 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/tests/db/test_purge.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    13916 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/tests/db/test_scoring_engine.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    11013 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/tests/db/test_service.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    14160 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/tests/db/test_strategy.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    13532 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/tests/db/utils.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-09-13 12:47:17.328571 python-watcher-9.0.0.0rc1/watcher/tests/decision_engine/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       65 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/tests/decision_engine/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-09-13 12:47:17.328571 python-watcher-9.0.0.0rc1/watcher/tests/decision_engine/audit/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/tests/decision_engine/audit/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    24158 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/tests/decision_engine/audit/test_audit_handlers.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-09-13 12:47:17.328571 python-watcher-9.0.0.0rc1/watcher/tests/decision_engine/cluster/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/tests/decision_engine/cluster/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5280 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/tests/decision_engine/cluster/test_cinder_cdmc.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3034 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/tests/decision_engine/cluster/test_cluster_data_model_collector.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    19581 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/tests/decision_engine/cluster/test_nova_cdmc.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-09-13 12:47:17.328571 python-watcher-9.0.0.0rc1/watcher/tests/decision_engine/datasources/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/tests/decision_engine/datasources/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-09-13 12:47:17.328571 python-watcher-9.0.0.0rc1/watcher/tests/decision_engine/datasources/grafana_translators/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/tests/decision_engine/datasources/grafana_translators/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3694 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/tests/decision_engine/datasources/grafana_translators/test_base.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5816 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/tests/decision_engine/datasources/grafana_translators/test_influxdb.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2391 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/tests/decision_engine/datasources/test_base.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8381 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/tests/decision_engine/datasources/test_gnocchi_helper.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    11858 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/tests/decision_engine/datasources/test_grafana_helper.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6822 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/tests/decision_engine/datasources/test_manager.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5697 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/tests/decision_engine/datasources/test_monasca_helper.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-09-13 12:47:17.328571 python-watcher-9.0.0.0rc1/watcher/tests/decision_engine/event_consumer/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/tests/decision_engine/event_consumer/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2203 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/tests/decision_engine/fake_goals.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1996 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/tests/decision_engine/fake_strategies.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-09-13 12:47:17.328571 python-watcher-9.0.0.0rc1/watcher/tests/decision_engine/loading/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/tests/decision_engine/loading/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3169 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/tests/decision_engine/loading/test_collector_loader.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1156 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/tests/decision_engine/loading/test_default_planner_loader.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2950 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/tests/decision_engine/loading/test_default_strategy_loader.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2736 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/tests/decision_engine/loading/test_goal_loader.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-09-13 12:47:17.328571 python-watcher-9.0.0.0rc1/watcher/tests/decision_engine/messaging/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/tests/decision_engine/messaging/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2990 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/tests/decision_engine/messaging/test_audit_endpoint.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2008 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/tests/decision_engine/messaging/test_data_model_endpoint.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-09-13 12:47:17.332571 python-watcher-9.0.0.0rc1/watcher/tests/decision_engine/model/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/tests/decision_engine/model/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9723 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/tests/decision_engine/model/ceilometer_metrics.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-09-13 12:47:17.332571 python-watcher-9.0.0.0rc1/watcher/tests/decision_engine/model/data/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      451 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/tests/decision_engine/model/data/ironic_scenario_1.xml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10426 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/tests/decision_engine/model/data/scenario_1.xml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4984 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/tests/decision_engine/model/data/scenario_10.xml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9920 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/tests/decision_engine/model/data/scenario_1_with_1_node_unavailable.xml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7721 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/tests/decision_engine/model/data/scenario_1_with_all_instances_exclude.xml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1130 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/tests/decision_engine/model/data/scenario_1_with_all_nodes_disable.xml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1057 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/tests/decision_engine/model/data/scenario_1_with_metrics.xml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2539 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/tests/decision_engine/model/data/scenario_2_with_metrics.xml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1195 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/tests/decision_engine/model/data/scenario_3_with_2_nodes.xml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1535 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/tests/decision_engine/model/data/scenario_3_with_metrics.xml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      278 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/tests/decision_engine/model/data/scenario_4_with_1_node_no_instance.xml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      423 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/tests/decision_engine/model/data/scenario_5_with_instance_disk_0.xml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1587 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/tests/decision_engine/model/data/scenario_6_with_2_nodes.xml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1709 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/tests/decision_engine/model/data/scenario_7_with_2_nodes.xml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2581 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/tests/decision_engine/model/data/scenario_8_with_4_nodes.xml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2617 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/tests/decision_engine/model/data/scenario_9_with_3_active_plus_1_disabled_nodes.xml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4147 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/tests/decision_engine/model/data/storage_scenario_1.xml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10175 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/tests/decision_engine/model/faker_cluster_and_metrics.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    12405 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/tests/decision_engine/model/faker_cluster_state.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9358 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/tests/decision_engine/model/gnocchi_metrics.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4121 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/tests/decision_engine/model/monasca_metrics.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-09-13 12:47:17.336571 python-watcher-9.0.0.0rc1/watcher/tests/decision_engine/model/notification/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/tests/decision_engine/model/notification/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-09-13 12:47:17.340571 python-watcher-9.0.0.0rc1/watcher/tests/decision_engine/model/notification/data/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      318 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/tests/decision_engine/model/notification/data/capacity.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4171 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/tests/decision_engine/model/notification/data/instance-create-end.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1726 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/tests/decision_engine/model/notification/data/instance-delete-end.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3781 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/tests/decision_engine/model/notification/data/instance-live_migration_force_complete-end.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3757 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/tests/decision_engine/model/notification/data/instance-live_migration_post-end.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3741 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/tests/decision_engine/model/notification/data/instance-lock.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3749 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/tests/decision_engine/model/notification/data/instance-pause-end.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3755 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/tests/decision_engine/model/notification/data/instance-power_off-end.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3752 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/tests/decision_engine/model/notification/data/instance-power_on-end.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3885 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/tests/decision_engine/model/notification/data/instance-rebuild-end.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3830 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/tests/decision_engine/model/notification/data/instance-rescue-end.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3721 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/tests/decision_engine/model/notification/data/instance-resize_confirm-end.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3751 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/tests/decision_engine/model/notification/data/instance-restore-end.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3750 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/tests/decision_engine/model/notification/data/instance-resume-end.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3752 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/tests/decision_engine/model/notification/data/instance-shelve-end.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3129 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/tests/decision_engine/model/notification/data/instance-shutdown-end.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3780 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/tests/decision_engine/model/notification/data/instance-soft_delete-end.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3754 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/tests/decision_engine/model/notification/data/instance-suspend-end.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3744 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/tests/decision_engine/model/notification/data/instance-unlock.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3751 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/tests/decision_engine/model/notification/data/instance-unpause-end.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3752 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/tests/decision_engine/model/notification/data/instance-unrescue-end.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3752 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/tests/decision_engine/model/notification/data/instance-unshelve-end.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2503 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/tests/decision_engine/model/notification/data/instance-update.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2510 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/tests/decision_engine/model/notification/data/scenario3_instance-update.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2582 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/tests/decision_engine/model/notification/data/scenario3_notfound_instance-update.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1626 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/tests/decision_engine/model/notification/data/scenario3_notfound_legacy_instance-update.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      628 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/tests/decision_engine/model/notification/data/scenario3_service-update-disabled.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      616 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/tests/decision_engine/model/notification/data/scenario3_service-update-enabled.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      555 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/tests/decision_engine/model/notification/data/scenario_1_bootable-volume-create.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      323 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/tests/decision_engine/model/notification/data/scenario_1_capacity.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      323 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/tests/decision_engine/model/notification/data/scenario_1_capacity_node_notfound.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      325 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/tests/decision_engine/model/notification/data/scenario_1_capacity_pool_notfound.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      407 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/tests/decision_engine/model/notification/data/scenario_1_error-volume-create.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      524 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/tests/decision_engine/model/notification/data/scenario_1_volume-attach.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      528 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/tests/decision_engine/model/notification/data/scenario_1_volume-create.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      528 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/tests/decision_engine/model/notification/data/scenario_1_volume-create_pool_notfound.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      526 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/tests/decision_engine/model/notification/data/scenario_1_volume-delete.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      433 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/tests/decision_engine/model/notification/data/scenario_1_volume-detach.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      524 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/tests/decision_engine/model/notification/data/scenario_1_volume-resize.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      526 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/tests/decision_engine/model/notification/data/scenario_1_volume-update.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      692 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/tests/decision_engine/model/notification/data/service-create.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      697 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/tests/decision_engine/model/notification/data/service-delete.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      709 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/tests/decision_engine/model/notification/data/service-update.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2308 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/tests/decision_engine/model/notification/fake_managers.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    25527 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/tests/decision_engine/model/notification/test_cinder_notifications.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3715 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/tests/decision_engine/model/notification/test_notifications.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    35232 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/tests/decision_engine/model/notification/test_nova_notifications.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5637 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/tests/decision_engine/model/test_element.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    20671 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/tests/decision_engine/model/test_model.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-09-13 12:47:17.340571 python-watcher-9.0.0.0rc1/watcher/tests/decision_engine/planner/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/tests/decision_engine/planner/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10549 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/tests/decision_engine/planner/test_node_resource_consolidation.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1134 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/tests/decision_engine/planner/test_planner_manager.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    43556 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/tests/decision_engine/planner/test_weight_planner.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    16277 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/tests/decision_engine/planner/test_workload_stabilization_planner.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-09-13 12:47:17.340571 python-watcher-9.0.0.0rc1/watcher/tests/decision_engine/scope/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/tests/decision_engine/scope/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2674 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/tests/decision_engine/scope/fake_scopes.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2318 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/tests/decision_engine/scope/test_baremetal.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    14315 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/tests/decision_engine/scope/test_compute.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9901 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/tests/decision_engine/scope/test_storage.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-09-13 12:47:17.340571 python-watcher-9.0.0.0rc1/watcher/tests/decision_engine/scoring/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/tests/decision_engine/scoring/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2002 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/tests/decision_engine/scoring/test_dummy_scorer.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1901 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/tests/decision_engine/scoring/test_dummy_scoring_container.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1840 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/tests/decision_engine/scoring/test_scoring_factory.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-09-13 12:47:17.340571 python-watcher-9.0.0.0rc1/watcher/tests/decision_engine/solution/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/tests/decision_engine/solution/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2671 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/tests/decision_engine/solution/test_default_solution.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-09-13 12:47:17.340571 python-watcher-9.0.0.0rc1/watcher/tests/decision_engine/strategy/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/tests/decision_engine/strategy/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-09-13 12:47:17.340571 python-watcher-9.0.0.0rc1/watcher/tests/decision_engine/strategy/context/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/tests/decision_engine/strategy/context/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4261 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/tests/decision_engine/strategy/context/test_strategy_context.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-09-13 12:47:17.344571 python-watcher-9.0.0.0rc1/watcher/tests/decision_engine/strategy/selector/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/tests/decision_engine/strategy/selector/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2578 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/tests/decision_engine/strategy/selector/test_strategy_selector.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-09-13 12:47:17.344571 python-watcher-9.0.0.0rc1/watcher/tests/decision_engine/strategy/strategies/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/tests/decision_engine/strategy/strategies/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1342 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/tests/decision_engine/strategy/strategies/test_actuator.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5171 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/tests/decision_engine/strategy/strategies/test_base.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10009 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/tests/decision_engine/strategy/strategies/test_basic_consolidation.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1936 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/tests/decision_engine/strategy/strategies/test_dummy_strategy.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1951 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/tests/decision_engine/strategy/strategies/test_dummy_with_scorer.py
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)    10284 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/tests/decision_engine/strategy/strategies/test_host_maintenance.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    15906 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/tests/decision_engine/strategy/strategies/test_node_resource_consolidation.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5609 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/tests/decision_engine/strategy/strategies/test_noisy_neighbor.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4902 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/tests/decision_engine/strategy/strategies/test_outlet_temp_control.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8589 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/tests/decision_engine/strategy/strategies/test_saving_energy.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9419 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/tests/decision_engine/strategy/strategies/test_storage_capacity_balance.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2886 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/tests/decision_engine/strategy/strategies/test_strategy_endpoint.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7470 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/tests/decision_engine/strategy/strategies/test_uniform_airflow.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    16970 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/tests/decision_engine/strategy/strategies/test_vm_workload_consolidation.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6279 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/tests/decision_engine/strategy/strategies/test_workload_balance.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    12007 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/tests/decision_engine/strategy/strategies/test_workload_stabilization.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    30679 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/tests/decision_engine/strategy/strategies/test_zone_migration.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1319 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/tests/decision_engine/test_gmr.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2534 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/tests/decision_engine/test_rpcapi.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5376 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/tests/decision_engine/test_scheduling.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    30575 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/tests/decision_engine/test_sync.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2048 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/tests/fake_policy.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4132 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/tests/fakes.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-09-13 12:47:17.344571 python-watcher-9.0.0.0rc1/watcher/tests/notifications/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/tests/notifications/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    22457 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/tests/notifications/test_action_notification.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    28848 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/tests/notifications/test_action_plan_notification.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    22000 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/tests/notifications/test_audit_notification.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    15426 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/tests/notifications/test_notification.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2930 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/tests/notifications/test_service_notifications.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-09-13 12:47:17.348571 python-watcher-9.0.0.0rc1/watcher/tests/objects/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/tests/objects/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10241 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/tests/objects/test_action.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5683 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/tests/objects/test_action_description.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    14722 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/tests/objects/test_action_plan.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    14272 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/tests/objects/test_audit.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10670 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/tests/objects/test_audit_template.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6888 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/tests/objects/test_efficacy_indicator.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6177 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/tests/objects/test_goal.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    21201 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/tests/objects/test_objects.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7617 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/tests/objects/test_scoring_engine.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5100 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/tests/objects/test_service.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7364 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/tests/objects/test_strategy.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8058 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/tests/objects/utils.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1607 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/tests/policy_fixture.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5817 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/tests/test_threading.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      760 2022-09-13 12:45:39.000000 python-watcher-9.0.0.0rc1/watcher/version.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-09-27 15:24:05.225966 python-watcher-9.0.0.0rc2/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      181 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/.coveragerc
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       89 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/.mailmap
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       48 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/.stestr.conf
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6226 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/.zuul.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7408 2022-09-27 15:24:04.000000 python-watcher-9.0.0.0rc2/AUTHORS
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      540 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/CONTRIBUTING.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    56327 2022-09-27 15:24:04.000000 python-watcher-9.0.0.0rc2/ChangeLog
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      369 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/HACKING.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10143 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/LICENSE
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2421 2022-09-27 15:24:05.225966 python-watcher-9.0.0.0rc2/PKG-INFO
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1163 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/README.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-09-27 15:24:05.129966 python-watcher-9.0.0.0rc2/api-ref/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-09-27 15:24:05.137966 python-watcher-9.0.0.0rc2/api-ref/source/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2566 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/api-ref/source/conf.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      534 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/api-ref/source/index.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    14658 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/api-ref/source/parameters.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-09-27 15:24:05.141966 python-watcher-9.0.0.0rc2/api-ref/source/samples/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       96 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/api-ref/source/samples/actionplan-cancel-request-cancelling.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       95 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/api-ref/source/samples/actionplan-cancel-request-pending.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      990 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/api-ref/source/samples/actionplan-list-detailed-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      857 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/api-ref/source/samples/actionplan-list-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      695 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/api-ref/source/samples/actionplan-show-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      765 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/api-ref/source/samples/actionplan-start-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      999 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/api-ref/source/samples/actions-list-detailed-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      724 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/api-ref/source/samples/actions-list-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      783 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/api-ref/source/samples/actions-show-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      643 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/api-ref/source/samples/api-root-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1591 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/api-ref/source/samples/api-v1-root-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       95 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/api-ref/source/samples/audit-cancel-request.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1596 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/api-ref/source/samples/audit-cancel-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      366 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/api-ref/source/samples/audit-create-request-continuous.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      145 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/api-ref/source/samples/audit-create-request-oneshot.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1543 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/api-ref/source/samples/audit-create-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2057 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/api-ref/source/samples/audit-list-detailed-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      944 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/api-ref/source/samples/audit-list-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1598 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/api-ref/source/samples/audit-show-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      184 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/api-ref/source/samples/audit-update-request.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1596 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/api-ref/source/samples/audit-update-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      132 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/api-ref/source/samples/audittemplate-create-request-full.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       42 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/api-ref/source/samples/audittemplate-create-request-minimal.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      674 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/api-ref/source/samples/audittemplate-create-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      754 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/api-ref/source/samples/audittemplate-list-detailed-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      721 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/api-ref/source/samples/audittemplate-list-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      708 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/api-ref/source/samples/audittemplate-show-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       93 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/api-ref/source/samples/audittemplate-update-request.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      709 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/api-ref/source/samples/audittemplate-update-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1296 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/api-ref/source/samples/datamodel-list-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2163 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/api-ref/source/samples/goal-list-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      556 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/api-ref/source/samples/goal-show-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      654 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/api-ref/source/samples/scoring_engine-list-detailed-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      626 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/api-ref/source/samples/scoring_engine-list-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      491 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/api-ref/source/samples/scoring_engine-show-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      702 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/api-ref/source/samples/service-list-detailed-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      958 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/api-ref/source/samples/service-list-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      514 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/api-ref/source/samples/service-show-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1320 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/api-ref/source/samples/strategy-list-detailed-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      672 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/api-ref/source/samples/strategy-list-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      964 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/api-ref/source/samples/strategy-show-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1036 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/api-ref/source/samples/strategy-state-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5886 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/api-ref/source/watcher-api-v1-actionplans.inc
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3682 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/api-ref/source/watcher-api-v1-actions.inc
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7991 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/api-ref/source/watcher-api-v1-audits.inc
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5539 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/api-ref/source/watcher-api-v1-audittemplates.inc
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1159 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/api-ref/source/watcher-api-v1-datamodel.inc
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2483 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/api-ref/source/watcher-api-v1-goals.inc
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2581 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/api-ref/source/watcher-api-v1-scoring_engines.inc
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1982 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/api-ref/source/watcher-api-v1-services.inc
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3318 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/api-ref/source/watcher-api-v1-strategies.inc
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      327 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/api-ref/source/watcher-api-v1-webhooks.inc
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2054 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/api-ref/source/watcher-api-versions.inc
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-09-27 15:24:05.145966 python-watcher-9.0.0.0rc2/devstack/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-09-27 15:24:05.145966 python-watcher-9.0.0.0rc2/devstack/files/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1509 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/devstack/files/apache-watcher-api.template
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-09-27 15:24:05.145966 python-watcher-9.0.0.0rc2/devstack/lib/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    11762 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/devstack/lib/watcher
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1681 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/devstack/local.conf.compute
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1763 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/devstack/local.conf.controller
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      410 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/devstack/override-defaults
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1350 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/devstack/plugin.sh
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      248 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/devstack/settings
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-09-27 15:24:05.145966 python-watcher-9.0.0.0rc2/devstack/upgrade/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-09-27 15:24:05.145966 python-watcher-9.0.0.0rc2/devstack/upgrade/from_rocky/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      418 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/devstack/upgrade/from_rocky/upgrade-watcher
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)     3316 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/devstack/upgrade/resources.sh
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      818 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/devstack/upgrade/settings
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)      620 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/devstack/upgrade/shutdown.sh
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)     2485 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/devstack/upgrade/upgrade.sh
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-09-27 15:24:05.145966 python-watcher-9.0.0.0rc2/doc/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-09-27 15:24:05.145966 python-watcher-9.0.0.0rc2/doc/ext/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/doc/ext/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5324 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/doc/ext/term.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4243 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/doc/ext/versioned_notifications.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-09-27 15:24:05.149966 python-watcher-9.0.0.0rc2/doc/notification_samples/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1294 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/doc/notification_samples/action-cancel-end.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1708 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/doc/notification_samples/action-cancel-error.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1297 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/doc/notification_samples/action-cancel-start.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1264 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/doc/notification_samples/action-create.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1264 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/doc/notification_samples/action-delete.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1297 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/doc/notification_samples/action-execution-end.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1713 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/doc/notification_samples/action-execution-error.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1297 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/doc/notification_samples/action-execution-start.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1550 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/doc/notification_samples/action-update.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1873 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/doc/notification_samples/action_plan-cancel-end.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2301 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/doc/notification_samples/action_plan-cancel-error.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1876 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/doc/notification_samples/action_plan-cancel-start.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1860 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/doc/notification_samples/action_plan-create.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1874 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/doc/notification_samples/action_plan-delete.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1904 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/doc/notification_samples/action_plan-execution-end.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2329 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/doc/notification_samples/action_plan-execution-error.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1904 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/doc/notification_samples/action_plan-execution-start.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2164 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/doc/notification_samples/action_plan-update.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2269 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/doc/notification_samples/audit-create.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2269 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/doc/notification_samples/audit-delete.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2295 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/doc/notification_samples/audit-planner-end.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2710 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/doc/notification_samples/audit-planner-error.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2297 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/doc/notification_samples/audit-planner-start.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2296 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/doc/notification_samples/audit-strategy-end.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2711 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/doc/notification_samples/audit-strategy-error.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2298 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/doc/notification_samples/audit-strategy-start.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2554 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/doc/notification_samples/audit-update.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      593 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/doc/notification_samples/infra-optim-exception.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      908 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/doc/notification_samples/service-update.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      456 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/doc/requirements.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-09-27 15:24:05.149966 python-watcher-9.0.0.0rc2/doc/source/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-09-27 15:24:05.149966 python-watcher-9.0.0.0rc2/doc/source/_static/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/doc/source/_static/.placeholder
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-09-27 15:24:05.149966 python-watcher-9.0.0.0rc2/doc/source/admin/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1415 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/doc/source/admin/apache-mod-wsgi.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1696 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/doc/source/admin/gmr.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      236 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/doc/source/admin/index.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4623 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/doc/source/admin/policy.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    19148 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/doc/source/architecture.rst
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)     4764 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/doc/source/conf.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-09-27 15:24:05.149966 python-watcher-9.0.0.0rc2/doc/source/configuration/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    16807 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/doc/source/configuration/configuring.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      117 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/doc/source/configuration/index.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      254 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/doc/source/configuration/watcher.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-09-27 15:24:05.149966 python-watcher-9.0.0.0rc2/doc/source/contributor/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       75 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/doc/source/contributor/api_microversion_history.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    11476 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/doc/source/contributor/concurrency.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4720 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/doc/source/contributor/contributing.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10531 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/doc/source/contributor/devstack.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7899 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/doc/source/contributor/environment.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      156 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/doc/source/contributor/index.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      339 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/doc/source/contributor/notifications.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-09-27 15:24:05.149966 python-watcher-9.0.0.0rc2/doc/source/contributor/plugin/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7796 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/doc/source/contributor/plugin/action-plugin.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3297 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/doc/source/contributor/plugin/base-setup.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9795 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/doc/source/contributor/plugin/cdmc-plugin.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7862 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/doc/source/contributor/plugin/goal-plugin.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      204 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/doc/source/contributor/plugin/index.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6113 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/doc/source/contributor/plugin/planner-plugin.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1388 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/doc/source/contributor/plugin/plugins.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7943 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/doc/source/contributor/plugin/scoring-engine-plugin.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    11870 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/doc/source/contributor/plugin/strategy-plugin.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       44 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/doc/source/contributor/rally_link.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1404 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/doc/source/contributor/testing.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-09-27 15:24:05.149966 python-watcher-9.0.0.0rc2/doc/source/datasources/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    17515 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/doc/source/datasources/grafana.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       72 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/doc/source/datasources/index.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    12056 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/doc/source/glossary.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-09-27 15:24:05.129966 python-watcher-9.0.0.0rc2/doc/source/image_src/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-09-27 15:24:05.149966 python-watcher-9.0.0.0rc2/doc/source/image_src/dia/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3198 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/doc/source/image_src/dia/architecture.dia
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3212 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/doc/source/image_src/dia/functional_data_model.dia
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-09-27 15:24:05.153966 python-watcher-9.0.0.0rc2/doc/source/image_src/plantuml/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      375 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/doc/source/image_src/plantuml/README.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1038 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/doc/source/image_src/plantuml/action_plan_state_machine.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      835 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/doc/source/image_src/plantuml/audit_state_machine.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1406 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/doc/source/image_src/plantuml/sequence_architecture_cdmc_sync.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      660 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/doc/source/image_src/plantuml/sequence_create_and_launch_audit.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      751 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/doc/source/image_src/plantuml/sequence_create_audit_template.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1622 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/doc/source/image_src/plantuml/sequence_from_audit_execution_to_actionplan_creation.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      553 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/doc/source/image_src/plantuml/sequence_launch_action_plan.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1367 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/doc/source/image_src/plantuml/sequence_launch_action_plan_in_applier.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1376 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/doc/source/image_src/plantuml/sequence_overview_watcher_usage.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1995 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/doc/source/image_src/plantuml/sequence_trigger_audit_in_decision_engine.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3537 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/doc/source/image_src/plantuml/watcher_db_schema_diagram.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-09-27 15:24:05.153966 python-watcher-9.0.0.0rc2/doc/source/images/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    77970 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/doc/source/images/action_plan_state_machine.png
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    65012 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/doc/source/images/architecture.svg
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    46772 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/doc/source/images/audit_state_machine.png
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    87643 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/doc/source/images/functional_data_model.svg
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    46795 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/doc/source/images/sequence_architecture_cdmc_sync.png
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    33521 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/doc/source/images/sequence_create_and_launch_audit.png
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    30711 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/doc/source/images/sequence_create_audit_template.png
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    47585 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/doc/source/images/sequence_from_audit_execution_to_actionplan_creation.png
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    27899 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/doc/source/images/sequence_launch_action_plan.png
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    42190 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/doc/source/images/sequence_launch_action_plan_in_applier.png
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    46482 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/doc/source/images/sequence_overview_watcher_usage.png
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    73345 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/doc/source/images/sequence_trigger_audit_in_decision_engine.png
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    73815 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/doc/source/images/watcher_db_schema_diagram.png
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1906 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/doc/source/index.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-09-27 15:24:05.157966 python-watcher-9.0.0.0rc2/doc/source/install/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2577 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/doc/source/install/common_configure.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5458 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/doc/source/install/common_prerequisites.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1055 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/doc/source/install/get_started.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1295 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/doc/source/install/index.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1048 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/doc/source/install/install-rdo.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      918 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/doc/source/install/install-ubuntu.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      528 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/doc/source/install/install.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      178 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/doc/source/install/next-steps.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8019 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/doc/source/install/verify.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-09-27 15:24:05.157966 python-watcher-9.0.0.0rc2/doc/source/man/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      114 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/doc/source/man/footer.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2397 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/doc/source/man/general-options.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      204 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/doc/source/man/index.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      569 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/doc/source/man/watcher-api.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      594 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/doc/source/man/watcher-applier.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6589 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/doc/source/man/watcher-db-manage.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      674 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/doc/source/man/watcher-decision-engine.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2068 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/doc/source/man/watcher-status.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-09-27 15:24:05.157966 python-watcher-9.0.0.0rc2/doc/source/strategies/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2141 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/doc/source/strategies/actuation.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3263 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/doc/source/strategies/basic-server-consolidation.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2150 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/doc/source/strategies/host_maintenance.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       70 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/doc/source/strategies/index.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2291 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/doc/source/strategies/node_resource_consolidation.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2443 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/doc/source/strategies/noisy_neighbor.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2784 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/doc/source/strategies/outlet_temp_control.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2616 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/doc/source/strategies/saving_energy.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1893 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/doc/source/strategies/storage_capacity_balance.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2819 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/doc/source/strategies/strategy-template.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3212 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/doc/source/strategies/uniform_airflow.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3155 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/doc/source/strategies/vm_workload_consolidation.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6025 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/doc/source/strategies/workload-stabilization.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2782 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/doc/source/strategies/workload_balance.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5428 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/doc/source/strategies/zone_migration.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-09-27 15:24:05.157966 python-watcher-9.0.0.0rc2/doc/source/user/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    12578 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/doc/source/user/event_type_audit.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      117 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/doc/source/user/index.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5981 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/doc/source/user/user-guide.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4427 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/doc/source/user/ways-to-install.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-09-27 15:24:05.129966 python-watcher-9.0.0.0rc2/etc/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-09-27 15:24:05.157966 python-watcher-9.0.0.0rc2/etc/apache2/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1190 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/etc/apache2/watcher
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-09-27 15:24:05.157966 python-watcher-9.0.0.0rc2/etc/watcher/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      131 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/etc/watcher/README-watcher.conf.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-09-27 15:24:05.157966 python-watcher-9.0.0.0rc2/etc/watcher/oslo-config-generator/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      406 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/etc/watcher/oslo-config-generator/watcher.conf
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-09-27 15:24:05.157966 python-watcher-9.0.0.0rc2/etc/watcher/oslo-policy-generator/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       76 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/etc/watcher/oslo-policy-generator/watcher-policy-generator.conf
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-09-27 15:24:05.157966 python-watcher-9.0.0.0rc2/python_watcher.egg-info/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2421 2022-09-27 15:24:05.000000 python-watcher-9.0.0.0rc2/python_watcher.egg-info/PKG-INFO
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    41188 2022-09-27 15:24:05.000000 python-watcher-9.0.0.0rc2/python_watcher.egg-info/SOURCES.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2022-09-27 15:24:05.000000 python-watcher-9.0.0.0rc2/python_watcher.egg-info/dependency_links.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4397 2022-09-27 15:24:05.000000 python-watcher-9.0.0.0rc2/python_watcher.egg-info/entry_points.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2022-09-27 15:24:05.000000 python-watcher-9.0.0.0rc2/python_watcher.egg-info/not-zip-safe
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       47 2022-09-27 15:24:05.000000 python-watcher-9.0.0.0rc2/python_watcher.egg-info/pbr.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      917 2022-09-27 15:24:05.000000 python-watcher-9.0.0.0rc2/python_watcher.egg-info/requires.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        8 2022-09-27 15:24:05.000000 python-watcher-9.0.0.0rc2/python_watcher.egg-info/top_level.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-09-27 15:24:05.161966 python-watcher-9.0.0.0rc2/rally-jobs/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1421 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/rally-jobs/README.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1370 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/rally-jobs/watcher-watcher.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-09-27 15:24:05.129966 python-watcher-9.0.0.0rc2/releasenotes/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-09-27 15:24:05.169966 python-watcher-9.0.0.0rc2/releasenotes/notes/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/releasenotes/notes/.placeholder
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       63 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/releasenotes/notes/action-plan-cancel-c54726378019e096.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       67 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/releasenotes/notes/action-plan-versioned-notifications-api-e8ca4f5d37aa5b4b.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       62 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/releasenotes/notes/action-versioned-notifications-api-ff94fc0f401292d0.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       93 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/releasenotes/notes/add-baremetal-scoper-9ef23f5fb8f0be6a.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      279 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/releasenotes/notes/add-force-field-to-audit-4bcaeedfe27233ad.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      322 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/releasenotes/notes/add-ha-support-b9042255e5b76e42.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      129 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/releasenotes/notes/add-name-for-audit-0df1f39f00736f06.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      274 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/releasenotes/notes/add-plugins-parameters-376eb6b0b8978b44.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       59 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/releasenotes/notes/add-power-on-off-a77673d482568a8b.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      266 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/releasenotes/notes/add-scoring-module-fa00d013ed2d614e.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      156 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/releasenotes/notes/add-start-end-time-for-continuous-audit-52c45052cb06d153.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      472 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/releasenotes/notes/add-upgrade-check-framework-5bb9693c8a78931c.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      416 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/releasenotes/notes/api-call-retry-fef741ac684c58dd.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      432 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/releasenotes/notes/api-microversioning-7999a3ee8073bf32.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      165 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/releasenotes/notes/audit-scoper-for-storage-data-model-cdccc803542d22db.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      262 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/releasenotes/notes/audit-tag-vm-metadata-47a3e4468748853c.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       61 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/releasenotes/notes/audit-versioned-notifications-api-bca7738e16954bad.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      205 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/releasenotes/notes/automatic-triggering-audit-8a9b0540d547db60.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      148 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/releasenotes/notes/background-jobs-ha-9d3cf3fe356f4705.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      221 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/releasenotes/notes/bp-audit-scope-exclude-project-511a7720aac00dff.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       61 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/releasenotes/notes/build-baremetal-data-model-in-watcher-3023453a47b61dab.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      231 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/releasenotes/notes/cdm-scoping-8d9c307bad46bfa1.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       68 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/releasenotes/notes/centralise-config-opts-95670987dfbdb0e7.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      284 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/releasenotes/notes/change-ram-util-metric-4a3e6984b9dd968d.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      264 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/releasenotes/notes/check-strategy-requirements-66f9e9262412f8ec.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       56 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/releasenotes/notes/cinder-model-integration-baa394a72a0a33bf.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      183 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/releasenotes/notes/cluster-model-objects-wrapper-9c799ea262c56a5b.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      190 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/releasenotes/notes/compute-cdm-include-all-instances-f7506ded2d57732f.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      118 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/releasenotes/notes/configurable-weights-default-planner-3746b33160bc7347.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      898 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/releasenotes/notes/consume-nova-versioned-notifications-f98361b37e546b4d.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      121 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/releasenotes/notes/continuously-optimization-35364f4d2c0b81fc.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      363 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/releasenotes/notes/cron-based-continuous-audits-c3eedf28d9752b37.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      764 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/releasenotes/notes/datasource-query-retry-00cba5f7e68aec39.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       74 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/releasenotes/notes/db-migration-e1a705a8b54ccdd2.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      220 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/releasenotes/notes/define-the-audit-scope-e89edc5051dcf3f2.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      305 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/releasenotes/notes/deprecate-ceilometer-datasource-446b0be70fbce28b.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1008 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/releasenotes/notes/deprecate-json-formatted-policy-file-3a92379e9f5dd203.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      199 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/releasenotes/notes/drop-py-2-7-54f8e806d71f19a7.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      123 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/releasenotes/notes/dynamic-action-description-0e947b9e7ef2a134.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      112 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/releasenotes/notes/efficacy-indicator-95380ad7b84e3be2.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      824 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/releasenotes/notes/enhance-watcher-applier-engine-86c676ce8f179e68.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      318 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/releasenotes/notes/event-driven-optimization-based-4870f112bef8a560.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      576 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/releasenotes/notes/file-based-metric-map-c2af62b5067895df.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      782 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/releasenotes/notes/formal-datasource-interface-implementation-222769d55a127d33.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1024 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/releasenotes/notes/general-purpose-decision-engine-threadpool-0711b23abfc9d409.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      170 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/releasenotes/notes/get-goal-from-strategy-396c9b13a38bb650.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      391 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/releasenotes/notes/global-datasource-preference-3ab47b4be09ff3a5.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      146 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/releasenotes/notes/gnocchi-watcher-43c25d391fbd3e9c.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      547 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/releasenotes/notes/grafana-datasource-b672367c23ffa0c6.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      266 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/releasenotes/notes/graph-based-cluster-model-523937a6f5e66537.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      365 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/releasenotes/notes/host-maintenance-strategy-41f640927948fb56.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      957 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/releasenotes/notes/improve-compute-data-model-b427c85e4ed2b6fb.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       87 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/releasenotes/notes/jsonschema-validation-79cab05d5295da00.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      272 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/releasenotes/notes/min-required-nova-train-71f124192d88ae52.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      102 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/releasenotes/notes/monasca-support-0b0486b8572ac38b.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      267 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/releasenotes/notes/multiple-global-efficacy-indicator-fc11c4844a12a7d5.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      245 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/releasenotes/notes/node-resource-consolidation-73bc0c0abfeb0b03.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      196 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/releasenotes/notes/noisy-neighbor-strategy-a71342740b59dddc.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      155 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/releasenotes/notes/notifications-actionplan-cancel-edb2a4a12543e2d0.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      182 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/releasenotes/notes/optimization-threshold-21ad38f0470d0e1a.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      127 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/releasenotes/notes/persistent-audit-parameters-ae41dd7252ba9672.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      142 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/releasenotes/notes/planner-storage-action-plan-26ef37893c5e8648.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      126 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/releasenotes/notes/remove-nova-legacy-notifications-e1b6d10eff58f30a.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      519 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/releasenotes/notes/replace-cold-migrate-to-use-nova-migration-api-cecd9a39ddd3bc58.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      221 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/releasenotes/notes/scope-for-data-model-ea9792f90db14343.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       63 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/releasenotes/notes/service-versioned-notifications-api-70367b79a565d900.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      578 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/releasenotes/notes/show-datamodel-api-6945b744fd5d25d5.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      118 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/releasenotes/notes/stale-action-plan-b6a6b08df873c128.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      246 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/releasenotes/notes/standard-deviation-strategy-cd1d0c443fdfde9c.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       65 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/releasenotes/notes/storage-workload-balance-0ecabbc1791e6894.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      168 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/releasenotes/notes/support-keystoneclient-option-b30d1ff45f86a2e7.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      380 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/releasenotes/notes/support-placement-api-58ce6bef1bbbe98a.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       52 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/releasenotes/notes/suspended-audit-state-07f998c94e9d9a47.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      154 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/releasenotes/notes/uniform-airflow-strategy-68cdba1419c3f770.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      427 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/releasenotes/notes/uwsgi-support-8dcea6961e56dad0.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       52 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/releasenotes/notes/volume-migrate-action-fc57b0ce0e4c39ae.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      473 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/releasenotes/notes/watcher-notifications-ovo-7b44d52ef6400dd0.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      153 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/releasenotes/notes/watcher-planner-selector-84d77549d46f362a.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       82 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/releasenotes/notes/watcher-policies-1e86a30f0f11c6fa.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       69 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/releasenotes/notes/watcher-service-list-7b2f4b64f71e9b89.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      183 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/releasenotes/notes/watcher-versioned-objects-fc5abf5c81c4590c.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      241 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/releasenotes/notes/workload-balance-base-on-cpu-or-ram-util-3ff4ee968c32b2ed.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      265 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/releasenotes/notes/workload-balance-migration-strategy-a0b05148a57815c0.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      200 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/releasenotes/notes/zone-migration-strategy-10f7656a2a01e607.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-09-27 15:24:05.169966 python-watcher-9.0.0.0rc2/releasenotes/source/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-09-27 15:24:05.169966 python-watcher-9.0.0.0rc2/releasenotes/source/_static/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/releasenotes/source/_static/.placeholder
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8395 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/releasenotes/source/conf.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      902 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/releasenotes/source/index.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-09-27 15:24:05.133966 python-watcher-9.0.0.0rc2/releasenotes/source/locale/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-09-27 15:24:05.133966 python-watcher-9.0.0.0rc2/releasenotes/source/locale/en_GB/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-09-27 15:24:05.169966 python-watcher-9.0.0.0rc2/releasenotes/source/locale/en_GB/LC_MESSAGES/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    45874 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/releasenotes/source/locale/en_GB/LC_MESSAGES/releasenotes.po
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-09-27 15:24:05.133966 python-watcher-9.0.0.0rc2/releasenotes/source/locale/fr/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-09-27 15:24:05.169966 python-watcher-9.0.0.0rc2/releasenotes/source/locale/fr/LC_MESSAGES/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      914 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/releasenotes/source/locale/fr/LC_MESSAGES/releasenotes.po
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      154 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/releasenotes/source/newton.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      152 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/releasenotes/source/ocata.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      143 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/releasenotes/source/pike.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      147 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/releasenotes/source/queens.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      145 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/releasenotes/source/rocky.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      145 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/releasenotes/source/stein.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      126 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/releasenotes/source/train.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      112 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/releasenotes/source/unreleased.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      130 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/releasenotes/source/ussuri.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      138 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/releasenotes/source/victoria.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      134 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/releasenotes/source/wallaby.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      122 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/releasenotes/source/xena.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      122 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/releasenotes/source/yoga.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1620 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/requirements.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5423 2022-09-27 15:24:05.225966 python-watcher-9.0.0.0rc2/setup.cfg
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      697 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/setup.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      527 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/test-requirements.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3808 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/tox.ini
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-09-27 15:24:05.169966 python-watcher-9.0.0.0rc2/watcher/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      640 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1295 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/_i18n.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-09-27 15:24:05.169966 python-watcher-9.0.0.0rc2/watcher/api/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/api/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1474 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/api/acl.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1660 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/api/app.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      906 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/api/app.wsgi
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1631 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/api/config.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-09-27 15:24:05.169966 python-watcher-9.0.0.0rc2/watcher/api/controllers/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/api/controllers/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4397 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/api/controllers/base.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2035 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/api/controllers/link.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1026 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/api/controllers/rest_api_version_history.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3650 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/api/controllers/root.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-09-27 15:24:05.173966 python-watcher-9.0.0.0rc2/watcher/api/controllers/v1/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10926 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/api/controllers/v1/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    16676 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/api/controllers/v1/action.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    23842 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/api/controllers/v1/action_plan.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    28050 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/api/controllers/v1/audit.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    28005 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/api/controllers/v1/audit_template.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1756 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/api/controllers/v1/collection.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2661 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/api/controllers/v1/data_model.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2719 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/api/controllers/v1/efficacy_indicator.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8924 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/api/controllers/v1/goal.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9262 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/api/controllers/v1/scoring_engine.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9645 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/api/controllers/v1/service.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    12595 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/api/controllers/v1/strategy.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6526 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/api/controllers/v1/types.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6112 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/api/controllers/v1/utils.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1827 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/api/controllers/v1/versions.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2215 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/api/controllers/v1/webhooks.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3984 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/api/hooks.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-09-27 15:24:05.173966 python-watcher-9.0.0.0rc2/watcher/api/middleware/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/api/middleware/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2104 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/api/middleware/auth_token.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3814 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/api/middleware/parsable_error.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5283 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/api/scheduling.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1269 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/api/wsgi.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-09-27 15:24:05.173966 python-watcher-9.0.0.0rc2/watcher/applier/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/applier/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-09-27 15:24:05.173966 python-watcher-9.0.0.0rc2/watcher/applier/action_plan/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/applier/action_plan/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      820 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/applier/action_plan/base.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4286 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/applier/action_plan/default.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-09-27 15:24:05.173966 python-watcher-9.0.0.0rc2/watcher/applier/actions/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/applier/actions/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4876 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/applier/actions/base.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4047 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/applier/actions/change_node_power_state.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4484 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/applier/actions/change_nova_service_state.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1568 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/applier/actions/factory.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7989 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/applier/actions/migration.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1877 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/applier/actions/nop.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3379 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/applier/actions/resize.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2024 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/applier/actions/sleep.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8523 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/applier/actions/volume_migration.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1073 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/applier/base.py
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)     2093 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/applier/default.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-09-27 15:24:05.173966 python-watcher-9.0.0.0rc2/watcher/applier/loading/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/applier/loading/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      946 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/applier/loading/default.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1446 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/applier/manager.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-09-27 15:24:05.173966 python-watcher-9.0.0.0rc2/watcher/applier/messaging/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/applier/messaging/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1728 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/applier/messaging/trigger.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1894 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/applier/rpcapi.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3020 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/applier/sync.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-09-27 15:24:05.177966 python-watcher-9.0.0.0rc2/watcher/applier/workflow_engine/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/applier/workflow_engine/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    12117 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/applier/workflow_engine/base.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7890 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/applier/workflow_engine/default.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-09-27 15:24:05.177966 python-watcher-9.0.0.0rc2/watcher/cmd/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1228 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/cmd/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1733 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/cmd/api.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1335 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/cmd/applier.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5369 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/cmd/dbmanage.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1626 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/cmd/decisionengine.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1829 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/cmd/status.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1059 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/cmd/sync.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-09-27 15:24:05.177966 python-watcher-9.0.0.0rc2/watcher/common/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/common/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9599 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/common/cinder_helper.py
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)    12032 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/common/clients.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1465 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/common/config.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4555 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/common/context.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    14304 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/common/exception.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1609 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/common/ironic_helper.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4487 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/common/keystone_helper.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-09-27 15:24:05.177966 python-watcher-9.0.0.0rc2/watcher/common/loader/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/common/loader/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      842 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/common/loader/base.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3076 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/common/loader/default.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2224 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/common/loader/loadable.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    29807 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/common/nova_helper.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1178 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/common/paths.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6652 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/common/placement_helper.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-09-27 15:24:05.181966 python-watcher-9.0.0.0rc2/watcher/common/policies/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1384 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/common/policies/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1617 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/common/policies/action.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2597 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/common/policies/action_plan.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2434 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/common/policies/audit.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2654 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/common/policies/audit_template.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      938 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/common/policies/base.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1052 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/common/policies/data_model.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1551 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/common/policies/goal.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2136 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/common/policies/scoring_engine.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1577 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/common/policies/service.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1904 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/common/policies/strategy.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5250 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/common/policy.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4410 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/common/rpc.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2145 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/common/scheduling.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9715 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/common/service.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1337 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/common/service_manager.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4758 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/common/utils.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-09-27 15:24:05.181966 python-watcher-9.0.0.0rc2/watcher/conf/
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)     2340 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/conf/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2792 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/conf/api.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2207 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/conf/applier.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2503 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/conf/ceilometer_client.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1593 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/conf/cinder_client.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1085 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/conf/clients_auth.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1753 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/conf/collector.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2225 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/conf/datasources.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1344 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/conf/db.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4056 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/conf/decision_engine.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      989 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/conf/exception.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1593 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/conf/glance_client.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1581 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/conf/gnocchi_client.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6746 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/conf/grafana_client.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1651 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/conf/grafana_translators.py
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)     1589 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/conf/ironic_client.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1349 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/conf/keystone_client.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1596 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/conf/monasca_client.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1608 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/conf/neutron_client.py
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)     1923 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/conf/nova_client.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2547 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/conf/opts.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1774 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/conf/paths.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1513 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/conf/placement_client.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1305 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/conf/planner.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2426 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/conf/plugins.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1593 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/conf/service.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-09-27 15:24:05.181966 python-watcher-9.0.0.0rc2/watcher/db/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/db/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    32292 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/db/api.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1636 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/db/migration.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    16858 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/db/purge.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-09-27 15:24:05.181966 python-watcher-9.0.0.0rc2/watcher/db/sqlalchemy/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/db/sqlalchemy/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-09-27 15:24:05.181966 python-watcher-9.0.0.0rc2/watcher/db/sqlalchemy/alembic/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1942 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/db/sqlalchemy/alembic/README.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1769 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/db/sqlalchemy/alembic/env.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      412 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/db/sqlalchemy/alembic/script.py.mako
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-09-27 15:24:05.185966 python-watcher-9.0.0.0rc2/watcher/db/sqlalchemy/alembic/versions/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9500 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/db/sqlalchemy/alembic/versions/001_ocata.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1172 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/db/sqlalchemy/alembic/versions/0f6042416884_add_apscheduler_jobs.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      420 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/db/sqlalchemy/alembic/versions/3cfc94cecf4e_add_name_for_audit.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      547 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/db/sqlalchemy/alembic/versions/4b16194c56bc_add_start_end_time.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      583 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/db/sqlalchemy/alembic/versions/52804f2498c4_add_hostname.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      409 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/db/sqlalchemy/alembic/versions/609bec748f2a_add_force_field.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1342 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/db/sqlalchemy/alembic/versions/a86240e89a29_.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      673 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/db/sqlalchemy/alembic/versions/d098df6021e2_cron_support_for_audit.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1076 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/db/sqlalchemy/alembic/versions/d09a5945e4a0_add_action_description_table.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      975 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/db/sqlalchemy/alembic.ini
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    44322 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/db/sqlalchemy/api.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4441 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/db/sqlalchemy/job_store.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3676 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/db/sqlalchemy/migration.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10945 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/db/sqlalchemy/models.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-09-27 15:24:05.185966 python-watcher-9.0.0.0rc2/watcher/decision_engine/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/decision_engine/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-09-27 15:24:05.185966 python-watcher-9.0.0.0rc2/watcher/decision_engine/audit/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/decision_engine/audit/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5669 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/decision_engine/audit/base.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9490 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/decision_engine/audit/continuous.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1049 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/decision_engine/audit/event.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1046 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/decision_engine/audit/oneshot.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-09-27 15:24:05.185966 python-watcher-9.0.0.0rc2/watcher/decision_engine/datasources/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/decision_engine/datasources/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9376 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/decision_engine/datasources/base.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10668 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/decision_engine/datasources/ceilometer.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8788 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/decision_engine/datasources/gnocchi.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10217 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/decision_engine/datasources/grafana.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-09-27 15:24:05.185966 python-watcher-9.0.0.0rc2/watcher/decision_engine/datasources/grafana_translator/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/decision_engine/datasources/grafana_translator/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4554 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/decision_engine/datasources/grafana_translator/base.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3240 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/decision_engine/datasources/grafana_translator/influxdb.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5680 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/decision_engine/datasources/manager.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6950 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/decision_engine/datasources/monasca.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1504 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/decision_engine/gmr.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-09-27 15:24:05.185966 python-watcher-9.0.0.0rc2/watcher/decision_engine/goal/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1189 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/decision_engine/goal/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2011 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/decision_engine/goal/base.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-09-27 15:24:05.185966 python-watcher-9.0.0.0rc2/watcher/decision_engine/goal/efficacy/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/decision_engine/goal/efficacy/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3135 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/decision_engine/goal/efficacy/base.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8243 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/decision_engine/goal/efficacy/indicators.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6016 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/decision_engine/goal/efficacy/specs.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6789 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/decision_engine/goal/goals.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-09-27 15:24:05.185966 python-watcher-9.0.0.0rc2/watcher/decision_engine/loading/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/decision_engine/loading/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1928 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/decision_engine/loading/default.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2901 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/decision_engine/manager.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-09-27 15:24:05.185966 python-watcher-9.0.0.0rc2/watcher/decision_engine/messaging/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/decision_engine/messaging/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2144 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/decision_engine/messaging/audit_endpoint.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2180 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/decision_engine/messaging/data_model_endpoint.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-09-27 15:24:05.189966 python-watcher-9.0.0.0rc2/watcher/decision_engine/model/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/decision_engine/model/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1131 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/decision_engine/model/base.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-09-27 15:24:05.189966 python-watcher-9.0.0.0rc2/watcher/decision_engine/model/collector/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/decision_engine/model/collector/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9607 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/decision_engine/model/collector/base.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    11683 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/decision_engine/model/collector/cinder.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4037 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/decision_engine/model/collector/ironic.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2327 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/decision_engine/model/collector/manager.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    21542 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/decision_engine/model/collector/nova.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-09-27 15:24:05.189966 python-watcher-9.0.0.0rc2/watcher/decision_engine/model/element/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1320 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/decision_engine/model/element/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      924 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/decision_engine/model/element/baremetal_resource.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2063 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/decision_engine/model/element/base.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      860 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/decision_engine/model/element/compute_resource.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2162 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/decision_engine/model/element/instance.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3777 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/decision_engine/model/element/node.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      928 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/decision_engine/model/element/storage_resource.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1856 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/decision_engine/model/element/volume.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    23973 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/decision_engine/model/model_root.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-09-27 15:24:05.189966 python-watcher-9.0.0.0rc2/watcher/decision_engine/model/notification/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/decision_engine/model/notification/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1108 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/decision_engine/model/notification/base.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    14150 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/decision_engine/model/notification/cinder.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2887 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/decision_engine/model/notification/filtering.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    14709 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/decision_engine/model/notification/nova.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-09-27 15:24:05.189966 python-watcher-9.0.0.0rc2/watcher/decision_engine/planner/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/decision_engine/planner/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3069 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/decision_engine/planner/base.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1026 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/decision_engine/planner/manager.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5916 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/decision_engine/planner/node_resource_consolidation.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8282 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/decision_engine/planner/weight.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    11192 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/decision_engine/planner/workload_stabilization.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2286 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/decision_engine/rpcapi.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4349 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/decision_engine/scheduling.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-09-27 15:24:05.189966 python-watcher-9.0.0.0rc2/watcher/decision_engine/scope/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/decision_engine/scope/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2182 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/decision_engine/scope/baremetal.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1192 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/decision_engine/scope/base.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9321 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/decision_engine/scope/compute.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6418 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/decision_engine/scope/storage.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-09-27 15:24:05.189966 python-watcher-9.0.0.0rc2/watcher/decision_engine/scoring/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/decision_engine/scoring/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4341 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/decision_engine/scoring/base.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6519 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/decision_engine/scoring/dummy_scorer.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3400 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/decision_engine/scoring/dummy_scoring_container.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3663 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/decision_engine/scoring/scoring_factory.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-09-27 15:24:05.193966 python-watcher-9.0.0.0rc2/watcher/decision_engine/solution/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/decision_engine/solution/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4705 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/decision_engine/solution/base.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2480 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/decision_engine/solution/default.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3636 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/decision_engine/solution/efficacy.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      832 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/decision_engine/solution/solution_comparator.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      830 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/decision_engine/solution/solution_evaluator.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-09-27 15:24:05.193966 python-watcher-9.0.0.0rc2/watcher/decision_engine/strategy/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/decision_engine/strategy/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-09-27 15:24:05.193966 python-watcher-9.0.0.0rc2/watcher/decision_engine/strategy/common/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/decision_engine/strategy/common/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      822 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/decision_engine/strategy/common/level.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-09-27 15:24:05.193966 python-watcher-9.0.0.0rc2/watcher/decision_engine/strategy/context/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/decision_engine/strategy/context/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2654 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/decision_engine/strategy/context/base.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2591 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/decision_engine/strategy/context/default.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-09-27 15:24:05.193966 python-watcher-9.0.0.0rc2/watcher/decision_engine/strategy/selection/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/decision_engine/strategy/selection/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      810 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/decision_engine/strategy/selection/base.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2756 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/decision_engine/strategy/selection/default.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-09-27 15:24:05.193966 python-watcher-9.0.0.0rc2/watcher/decision_engine/strategy/strategies/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3053 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/decision_engine/strategy/strategies/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3009 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/decision_engine/strategy/strategies/actuation.py
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)    18295 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/decision_engine/strategy/strategies/base.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    18447 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/decision_engine/strategy/strategies/basic_consolidation.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2858 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/decision_engine/strategy/strategies/dummy_strategy.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3601 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/decision_engine/strategy/strategies/dummy_with_resize.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6266 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/decision_engine/strategy/strategies/dummy_with_scorer.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    11550 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/decision_engine/strategy/strategies/host_maintenance.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    11292 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/decision_engine/strategy/strategies/node_resource_consolidation.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9922 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/decision_engine/strategy/strategies/noisy_neighbor.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    11010 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/decision_engine/strategy/strategies/outlet_temp_control.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8734 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/decision_engine/strategy/strategies/saving_energy.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    15669 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/decision_engine/strategy/strategies/storage_capacity_balance.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    13390 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/decision_engine/strategy/strategies/uniform_airflow.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    23147 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/decision_engine/strategy/strategies/vm_workload_consolidation.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    14332 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/decision_engine/strategy/strategies/workload_balance.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    24902 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/decision_engine/strategy/strategies/workload_stabilization.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    33189 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/decision_engine/strategy/strategies/zone_migration.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    25320 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/decision_engine/sync.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3811 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/decision_engine/threading.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-09-27 15:24:05.193966 python-watcher-9.0.0.0rc2/watcher/hacking/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/hacking/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10378 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/hacking/checks.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-09-27 15:24:05.133966 python-watcher-9.0.0.0rc2/watcher/locale/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-09-27 15:24:05.133966 python-watcher-9.0.0.0rc2/watcher/locale/de/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-09-27 15:24:05.193966 python-watcher-9.0.0.0rc2/watcher/locale/de/LC_MESSAGES/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    26447 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/locale/de/LC_MESSAGES/watcher.po
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-09-27 15:24:05.133966 python-watcher-9.0.0.0rc2/watcher/locale/en_GB/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-09-27 15:24:05.193966 python-watcher-9.0.0.0rc2/watcher/locale/en_GB/LC_MESSAGES/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    26943 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/locale/en_GB/LC_MESSAGES/watcher.po
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-09-27 15:24:05.197966 python-watcher-9.0.0.0rc2/watcher/notifications/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1278 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/notifications/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    11699 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/notifications/action.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    13581 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/notifications/action_plan.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    12071 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/notifications/audit.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8094 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/notifications/base.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1990 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/notifications/exception.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1843 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/notifications/goal.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3885 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/notifications/service.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1877 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/notifications/strategy.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-09-27 15:24:05.197966 python-watcher-9.0.0.0rc2/watcher/objects/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1632 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/objects/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6945 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/objects/action.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5536 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/objects/action_description.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    13441 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/objects/action_plan.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    14365 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/objects/audit.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10374 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/objects/audit_template.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6546 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/objects/base.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7588 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/objects/efficacy_indicator.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4747 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/objects/fields.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6773 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/objects/goal.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8450 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/objects/scoring_engine.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5415 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/objects/service.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10140 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/objects/strategy.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-09-27 15:24:05.197966 python-watcher-9.0.0.0rc2/watcher/tests/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      962 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/tests/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-09-27 15:24:05.197966 python-watcher-9.0.0.0rc2/watcher/tests/api/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/tests/api/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    11971 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/tests/api/base.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1197 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/tests/api/test_base.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1369 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/tests/api/test_config.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10476 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/tests/api/test_hooks.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2830 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/tests/api/test_root.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5128 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/tests/api/test_scheduling.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1999 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/tests/api/test_utils.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3738 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/tests/api/utils.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-09-27 15:24:05.201966 python-watcher-9.0.0.0rc2/watcher/tests/api/v1/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/tests/api/v1/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    23438 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/tests/api/v1/test_actions.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    29901 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/tests/api/v1/test_actions_plans.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    38337 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/tests/api/v1/test_audit_templates.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    49443 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/tests/api/v1/test_audits.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3250 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/tests/api/v1/test_data_model.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7335 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/tests/api/v1/test_goals.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4998 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/tests/api/v1/test_microversions.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      702 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/tests/api/v1/test_root.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8033 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/tests/api/v1/test_scoring_engines.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8084 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/tests/api/v1/test_services.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    12214 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/tests/api/v1/test_strategies.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9313 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/tests/api/v1/test_types.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2219 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/tests/api/v1/test_utils.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3148 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/tests/api/v1/test_webhooks.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-09-27 15:24:05.201966 python-watcher-9.0.0.0rc2/watcher/tests/applier/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/tests/applier/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-09-27 15:24:05.201966 python-watcher-9.0.0.0rc2/watcher/tests/applier/action_plan/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/tests/applier/action_plan/__init__.py
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)     5488 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/tests/applier/action_plan/test_default_action_handler.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-09-27 15:24:05.201966 python-watcher-9.0.0.0rc2/watcher/tests/applier/actions/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/tests/applier/actions/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-09-27 15:24:05.201966 python-watcher-9.0.0.0rc2/watcher/tests/applier/actions/loading/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/tests/applier/actions/loading/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1109 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/tests/applier/actions/loading/test_default_actions_loader.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6267 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/tests/applier/actions/test_change_node_power_state.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5154 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/tests/applier/actions/test_change_nova_service_state.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8654 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/tests/applier/actions/test_migration.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3470 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/tests/applier/actions/test_resize.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1637 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/tests/applier/actions/test_sleep.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8973 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/tests/applier/actions/test_volume_migration.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-09-27 15:24:05.201966 python-watcher-9.0.0.0rc2/watcher/tests/applier/messaging/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/tests/applier/messaging/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1351 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/tests/applier/messaging/test_trigger_action_plan_endpoint.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1527 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/tests/applier/test_applier_manager.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1968 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/tests/applier/test_rpcapi.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3402 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/tests/applier/test_sync.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-09-27 15:24:05.201966 python-watcher-9.0.0.0rc2/watcher/tests/applier/workflow_engine/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/tests/applier/workflow_engine/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-09-27 15:24:05.201966 python-watcher-9.0.0.0rc2/watcher/tests/applier/workflow_engine/loading/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/tests/applier/workflow_engine/loading/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1159 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/tests/applier/workflow_engine/loading/test_default_engine_loader.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    16567 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/tests/applier/workflow_engine/test_default_workflow_engine.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6774 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/tests/applier/workflow_engine/test_taskflow_action_container.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4740 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/tests/base.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-09-27 15:24:05.205966 python-watcher-9.0.0.0rc2/watcher/tests/cmd/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/tests/cmd/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2199 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/tests/cmd/test_api.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1803 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/tests/cmd/test_applier.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7477 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/tests/cmd/test_db_manage.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2114 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/tests/cmd/test_decision_engine.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1586 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/tests/cmd/test_status.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-09-27 15:24:05.205966 python-watcher-9.0.0.0rc2/watcher/tests/common/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/tests/common/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-09-27 15:24:05.205966 python-watcher-9.0.0.0rc2/watcher/tests/common/loader/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/tests/common/loader/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3612 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/tests/common/loader/test_loader.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    16716 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/tests/common/test_cinder_helper.py
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)    17818 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/tests/common/test_clients.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2162 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/tests/common/test_ironic_helper.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    28524 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/tests/common/test_nova_helper.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    11761 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/tests/common/test_placement_helper.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3533 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/tests/common/test_service.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-09-27 15:24:05.205966 python-watcher-9.0.0.0rc2/watcher/tests/conf/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/tests/conf/__init__.py
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)     7028 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/tests/conf/test_list_opts.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1794 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/tests/conf_fixture.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1068 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/tests/config.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-09-27 15:24:05.205966 python-watcher-9.0.0.0rc2/watcher/tests/db/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/tests/db/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2588 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/tests/db/base.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    15255 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/tests/db/test_action.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    11274 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/tests/db/test_action_description.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    15616 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/tests/db/test_action_plan.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    16749 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/tests/db/test_audit.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    16525 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/tests/db/test_audit_template.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    17420 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/tests/db/test_efficacy_indicator.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    12103 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/tests/db/test_goal.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    23464 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/tests/db/test_purge.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    13916 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/tests/db/test_scoring_engine.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    11013 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/tests/db/test_service.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    14160 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/tests/db/test_strategy.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    13532 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/tests/db/utils.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-09-27 15:24:05.205966 python-watcher-9.0.0.0rc2/watcher/tests/decision_engine/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       65 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/tests/decision_engine/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-09-27 15:24:05.205966 python-watcher-9.0.0.0rc2/watcher/tests/decision_engine/audit/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/tests/decision_engine/audit/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    24158 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/tests/decision_engine/audit/test_audit_handlers.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-09-27 15:24:05.209966 python-watcher-9.0.0.0rc2/watcher/tests/decision_engine/cluster/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/tests/decision_engine/cluster/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5280 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/tests/decision_engine/cluster/test_cinder_cdmc.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3034 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/tests/decision_engine/cluster/test_cluster_data_model_collector.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    19581 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/tests/decision_engine/cluster/test_nova_cdmc.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-09-27 15:24:05.209966 python-watcher-9.0.0.0rc2/watcher/tests/decision_engine/datasources/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/tests/decision_engine/datasources/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-09-27 15:24:05.209966 python-watcher-9.0.0.0rc2/watcher/tests/decision_engine/datasources/grafana_translators/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/tests/decision_engine/datasources/grafana_translators/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3694 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/tests/decision_engine/datasources/grafana_translators/test_base.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5816 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/tests/decision_engine/datasources/grafana_translators/test_influxdb.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2391 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/tests/decision_engine/datasources/test_base.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8381 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/tests/decision_engine/datasources/test_gnocchi_helper.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    11858 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/tests/decision_engine/datasources/test_grafana_helper.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6822 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/tests/decision_engine/datasources/test_manager.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5697 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/tests/decision_engine/datasources/test_monasca_helper.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-09-27 15:24:05.209966 python-watcher-9.0.0.0rc2/watcher/tests/decision_engine/event_consumer/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/tests/decision_engine/event_consumer/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2203 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/tests/decision_engine/fake_goals.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1996 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/tests/decision_engine/fake_strategies.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-09-27 15:24:05.209966 python-watcher-9.0.0.0rc2/watcher/tests/decision_engine/loading/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/tests/decision_engine/loading/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3169 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/tests/decision_engine/loading/test_collector_loader.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1156 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/tests/decision_engine/loading/test_default_planner_loader.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2950 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/tests/decision_engine/loading/test_default_strategy_loader.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2736 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/tests/decision_engine/loading/test_goal_loader.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-09-27 15:24:05.209966 python-watcher-9.0.0.0rc2/watcher/tests/decision_engine/messaging/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/tests/decision_engine/messaging/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2990 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/tests/decision_engine/messaging/test_audit_endpoint.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2008 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/tests/decision_engine/messaging/test_data_model_endpoint.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-09-27 15:24:05.209966 python-watcher-9.0.0.0rc2/watcher/tests/decision_engine/model/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/tests/decision_engine/model/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9723 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/tests/decision_engine/model/ceilometer_metrics.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-09-27 15:24:05.213966 python-watcher-9.0.0.0rc2/watcher/tests/decision_engine/model/data/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      451 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/tests/decision_engine/model/data/ironic_scenario_1.xml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10426 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/tests/decision_engine/model/data/scenario_1.xml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4984 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/tests/decision_engine/model/data/scenario_10.xml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9920 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/tests/decision_engine/model/data/scenario_1_with_1_node_unavailable.xml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7721 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/tests/decision_engine/model/data/scenario_1_with_all_instances_exclude.xml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1130 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/tests/decision_engine/model/data/scenario_1_with_all_nodes_disable.xml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1057 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/tests/decision_engine/model/data/scenario_1_with_metrics.xml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2539 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/tests/decision_engine/model/data/scenario_2_with_metrics.xml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1195 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/tests/decision_engine/model/data/scenario_3_with_2_nodes.xml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1535 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/tests/decision_engine/model/data/scenario_3_with_metrics.xml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      278 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/tests/decision_engine/model/data/scenario_4_with_1_node_no_instance.xml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      423 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/tests/decision_engine/model/data/scenario_5_with_instance_disk_0.xml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1587 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/tests/decision_engine/model/data/scenario_6_with_2_nodes.xml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1709 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/tests/decision_engine/model/data/scenario_7_with_2_nodes.xml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2581 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/tests/decision_engine/model/data/scenario_8_with_4_nodes.xml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2617 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/tests/decision_engine/model/data/scenario_9_with_3_active_plus_1_disabled_nodes.xml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4147 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/tests/decision_engine/model/data/storage_scenario_1.xml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10175 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/tests/decision_engine/model/faker_cluster_and_metrics.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    12405 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/tests/decision_engine/model/faker_cluster_state.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9358 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/tests/decision_engine/model/gnocchi_metrics.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4121 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/tests/decision_engine/model/monasca_metrics.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-09-27 15:24:05.213966 python-watcher-9.0.0.0rc2/watcher/tests/decision_engine/model/notification/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/tests/decision_engine/model/notification/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-09-27 15:24:05.217966 python-watcher-9.0.0.0rc2/watcher/tests/decision_engine/model/notification/data/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      318 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/tests/decision_engine/model/notification/data/capacity.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4171 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/tests/decision_engine/model/notification/data/instance-create-end.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1726 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/tests/decision_engine/model/notification/data/instance-delete-end.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3781 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/tests/decision_engine/model/notification/data/instance-live_migration_force_complete-end.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3757 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/tests/decision_engine/model/notification/data/instance-live_migration_post-end.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3741 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/tests/decision_engine/model/notification/data/instance-lock.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3749 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/tests/decision_engine/model/notification/data/instance-pause-end.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3755 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/tests/decision_engine/model/notification/data/instance-power_off-end.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3752 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/tests/decision_engine/model/notification/data/instance-power_on-end.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3885 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/tests/decision_engine/model/notification/data/instance-rebuild-end.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3830 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/tests/decision_engine/model/notification/data/instance-rescue-end.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3721 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/tests/decision_engine/model/notification/data/instance-resize_confirm-end.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3751 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/tests/decision_engine/model/notification/data/instance-restore-end.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3750 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/tests/decision_engine/model/notification/data/instance-resume-end.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3752 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/tests/decision_engine/model/notification/data/instance-shelve-end.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3129 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/tests/decision_engine/model/notification/data/instance-shutdown-end.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3780 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/tests/decision_engine/model/notification/data/instance-soft_delete-end.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3754 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/tests/decision_engine/model/notification/data/instance-suspend-end.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3744 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/tests/decision_engine/model/notification/data/instance-unlock.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3751 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/tests/decision_engine/model/notification/data/instance-unpause-end.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3752 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/tests/decision_engine/model/notification/data/instance-unrescue-end.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3752 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/tests/decision_engine/model/notification/data/instance-unshelve-end.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2503 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/tests/decision_engine/model/notification/data/instance-update.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2510 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/tests/decision_engine/model/notification/data/scenario3_instance-update.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2582 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/tests/decision_engine/model/notification/data/scenario3_notfound_instance-update.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1626 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/tests/decision_engine/model/notification/data/scenario3_notfound_legacy_instance-update.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      628 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/tests/decision_engine/model/notification/data/scenario3_service-update-disabled.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      616 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/tests/decision_engine/model/notification/data/scenario3_service-update-enabled.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      555 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/tests/decision_engine/model/notification/data/scenario_1_bootable-volume-create.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      323 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/tests/decision_engine/model/notification/data/scenario_1_capacity.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      323 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/tests/decision_engine/model/notification/data/scenario_1_capacity_node_notfound.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      325 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/tests/decision_engine/model/notification/data/scenario_1_capacity_pool_notfound.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      407 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/tests/decision_engine/model/notification/data/scenario_1_error-volume-create.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      524 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/tests/decision_engine/model/notification/data/scenario_1_volume-attach.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      528 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/tests/decision_engine/model/notification/data/scenario_1_volume-create.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      528 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/tests/decision_engine/model/notification/data/scenario_1_volume-create_pool_notfound.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      526 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/tests/decision_engine/model/notification/data/scenario_1_volume-delete.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      433 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/tests/decision_engine/model/notification/data/scenario_1_volume-detach.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      524 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/tests/decision_engine/model/notification/data/scenario_1_volume-resize.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      526 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/tests/decision_engine/model/notification/data/scenario_1_volume-update.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      692 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/tests/decision_engine/model/notification/data/service-create.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      697 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/tests/decision_engine/model/notification/data/service-delete.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      709 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/tests/decision_engine/model/notification/data/service-update.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2308 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/tests/decision_engine/model/notification/fake_managers.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    25527 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/tests/decision_engine/model/notification/test_cinder_notifications.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3715 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/tests/decision_engine/model/notification/test_notifications.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    35232 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/tests/decision_engine/model/notification/test_nova_notifications.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5637 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/tests/decision_engine/model/test_element.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    20671 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/tests/decision_engine/model/test_model.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-09-27 15:24:05.217966 python-watcher-9.0.0.0rc2/watcher/tests/decision_engine/planner/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/tests/decision_engine/planner/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10549 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/tests/decision_engine/planner/test_node_resource_consolidation.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1134 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/tests/decision_engine/planner/test_planner_manager.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    43556 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/tests/decision_engine/planner/test_weight_planner.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    16277 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/tests/decision_engine/planner/test_workload_stabilization_planner.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-09-27 15:24:05.217966 python-watcher-9.0.0.0rc2/watcher/tests/decision_engine/scope/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/tests/decision_engine/scope/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2674 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/tests/decision_engine/scope/fake_scopes.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2318 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/tests/decision_engine/scope/test_baremetal.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    14315 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/tests/decision_engine/scope/test_compute.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9901 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/tests/decision_engine/scope/test_storage.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-09-27 15:24:05.217966 python-watcher-9.0.0.0rc2/watcher/tests/decision_engine/scoring/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/tests/decision_engine/scoring/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2002 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/tests/decision_engine/scoring/test_dummy_scorer.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1901 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/tests/decision_engine/scoring/test_dummy_scoring_container.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1840 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/tests/decision_engine/scoring/test_scoring_factory.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-09-27 15:24:05.217966 python-watcher-9.0.0.0rc2/watcher/tests/decision_engine/solution/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/tests/decision_engine/solution/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2671 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/tests/decision_engine/solution/test_default_solution.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-09-27 15:24:05.217966 python-watcher-9.0.0.0rc2/watcher/tests/decision_engine/strategy/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/tests/decision_engine/strategy/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-09-27 15:24:05.217966 python-watcher-9.0.0.0rc2/watcher/tests/decision_engine/strategy/context/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/tests/decision_engine/strategy/context/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4261 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/tests/decision_engine/strategy/context/test_strategy_context.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-09-27 15:24:05.217966 python-watcher-9.0.0.0rc2/watcher/tests/decision_engine/strategy/selector/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/tests/decision_engine/strategy/selector/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2578 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/tests/decision_engine/strategy/selector/test_strategy_selector.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-09-27 15:24:05.221966 python-watcher-9.0.0.0rc2/watcher/tests/decision_engine/strategy/strategies/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/tests/decision_engine/strategy/strategies/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1342 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/tests/decision_engine/strategy/strategies/test_actuator.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5171 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/tests/decision_engine/strategy/strategies/test_base.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10009 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/tests/decision_engine/strategy/strategies/test_basic_consolidation.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1936 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/tests/decision_engine/strategy/strategies/test_dummy_strategy.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1951 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/tests/decision_engine/strategy/strategies/test_dummy_with_scorer.py
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)    10284 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/tests/decision_engine/strategy/strategies/test_host_maintenance.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    15906 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/tests/decision_engine/strategy/strategies/test_node_resource_consolidation.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5609 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/tests/decision_engine/strategy/strategies/test_noisy_neighbor.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4902 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/tests/decision_engine/strategy/strategies/test_outlet_temp_control.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8589 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/tests/decision_engine/strategy/strategies/test_saving_energy.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9419 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/tests/decision_engine/strategy/strategies/test_storage_capacity_balance.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2886 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/tests/decision_engine/strategy/strategies/test_strategy_endpoint.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7470 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/tests/decision_engine/strategy/strategies/test_uniform_airflow.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    16970 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/tests/decision_engine/strategy/strategies/test_vm_workload_consolidation.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6279 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/tests/decision_engine/strategy/strategies/test_workload_balance.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    12007 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/tests/decision_engine/strategy/strategies/test_workload_stabilization.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    30679 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/tests/decision_engine/strategy/strategies/test_zone_migration.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1319 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/tests/decision_engine/test_gmr.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2534 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/tests/decision_engine/test_rpcapi.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5376 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/tests/decision_engine/test_scheduling.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    30575 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/tests/decision_engine/test_sync.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2048 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/tests/fake_policy.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4132 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/tests/fakes.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-09-27 15:24:05.221966 python-watcher-9.0.0.0rc2/watcher/tests/notifications/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/tests/notifications/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    22457 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/tests/notifications/test_action_notification.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    28848 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/tests/notifications/test_action_plan_notification.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    22000 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/tests/notifications/test_audit_notification.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    15426 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/tests/notifications/test_notification.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2930 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/tests/notifications/test_service_notifications.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-09-27 15:24:05.221966 python-watcher-9.0.0.0rc2/watcher/tests/objects/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/tests/objects/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10241 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/tests/objects/test_action.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5683 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/tests/objects/test_action_description.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    14722 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/tests/objects/test_action_plan.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    14272 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/tests/objects/test_audit.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10670 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/tests/objects/test_audit_template.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6888 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/tests/objects/test_efficacy_indicator.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6177 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/tests/objects/test_goal.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    21201 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/tests/objects/test_objects.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7617 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/tests/objects/test_scoring_engine.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5100 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/tests/objects/test_service.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7364 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/tests/objects/test_strategy.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8058 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/tests/objects/utils.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1607 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/tests/policy_fixture.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5817 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/tests/test_threading.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      760 2022-09-27 15:23:29.000000 python-watcher-9.0.0.0rc2/watcher/version.py
```

### Comparing `python-watcher-9.0.0.0rc1/.zuul.yaml` & `python-watcher-9.0.0.0rc2/.zuul.yaml`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 - project:
+    queue: watcher
     templates:
       - check-requirements
       - openstack-cover-jobs
       - openstack-python3-zed-jobs
       - publish-openstack-docs-pti
       - release-notes-jobs-python3
     check:
@@ -10,15 +11,14 @@
         - watcher-tempest-functional
         - watcher-grenade
         - watcher-tempest-strategies
         - watcher-tempest-actuator
         - watcherclient-tempest-functional
         - watcher-tempest-functional-ipv6-only
     gate:
-      queue: watcher
       jobs:
         - watcher-tempest-functional
         - watcher-tempest-functional-ipv6-only
 
 - job:
     name: watcher-tempest-dummy_optim
     parent: watcher-tempest-multinode
```

### Comparing `python-watcher-9.0.0.0rc1/AUTHORS` & `python-watcher-9.0.0.0rc2/AUTHORS`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 98k <18552437190@163.com>
 Akihito INOH <aki-inou@rs.jp.nec.com>
 Alexander Chadin <a.chadin@servionica.ru>
 Alexander Chadin <aschadin@sbcloud.ru>
 Alexandr Stavitskiy <stavitskiy@servionica.ru>
+Alfredo Moralejo <amoralej@redhat.com>
 Amy Fong <amy.fong@windriver.com>
 Andrea Frittoli <andrea.frittoli@gmail.com>
 Andreas Jaeger <aj@suse.com>
 Andreas Jaeger <jaegerandi@gmail.com>
 Antoine Cabot <antoine.cabot@b-com.com>
 Anton Khaldin <anton.haldin@gmail.com>
 Atul Pandey <atul.pandey@nectechnologies.in>
```

### Comparing `python-watcher-9.0.0.0rc1/CONTRIBUTING.rst` & `python-watcher-9.0.0.0rc2/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/ChangeLog` & `python-watcher-9.0.0.0rc2/ChangeLog`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,15 @@
 CHANGES
 =======
 
+9.0.0.0rc2
+----------
+
+* Fix compatibility with oslo.db 12.1.0
+
 9.0.0.0rc1
 ----------
 
 * Imported Translations from Zanata
 * remove unicode from code
 * Tests: fix requirements for unit tests
 * Watcher DB upgrde compatibility consideration for add\_apscheduler\_jobs
```

### Comparing `python-watcher-9.0.0.0rc1/LICENSE` & `python-watcher-9.0.0.0rc2/LICENSE`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/PKG-INFO` & `python-watcher-9.0.0.0rc2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: python-watcher
-Version: 9.0.0.0rc1
+Version: 9.0.0.0rc2
 Summary: OpenStack Watcher provides a flexible and scalable resource optimization service for multi-tenant OpenStack-based clouds.
 Home-page: https://docs.openstack.org/watcher/latest/
 Author: OpenStack
 Author-email: openstack-discuss@lists.openstack.org
 License: UNKNOWN
 Description: =======
         Watcher
```

### Comparing `python-watcher-9.0.0.0rc1/README.rst` & `python-watcher-9.0.0.0rc2/README.rst`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/api-ref/source/conf.py` & `python-watcher-9.0.0.0rc2/api-ref/source/conf.py`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/api-ref/source/index.rst` & `python-watcher-9.0.0.0rc2/api-ref/source/index.rst`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/api-ref/source/parameters.yaml` & `python-watcher-9.0.0.0rc2/api-ref/source/parameters.yaml`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/api-ref/source/samples/actionplan-list-detailed-response.json` & `python-watcher-9.0.0.0rc2/api-ref/source/samples/actionplan-list-detailed-response.json`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/api-ref/source/samples/actionplan-list-response.json` & `python-watcher-9.0.0.0rc2/api-ref/source/samples/actionplan-list-response.json`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/api-ref/source/samples/actionplan-show-response.json` & `python-watcher-9.0.0.0rc2/api-ref/source/samples/actionplan-show-response.json`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/api-ref/source/samples/actionplan-start-response.json` & `python-watcher-9.0.0.0rc2/api-ref/source/samples/actionplan-start-response.json`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/api-ref/source/samples/actions-list-detailed-response.json` & `python-watcher-9.0.0.0rc2/api-ref/source/samples/actions-list-detailed-response.json`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/api-ref/source/samples/actions-list-response.json` & `python-watcher-9.0.0.0rc2/api-ref/source/samples/actions-list-response.json`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/api-ref/source/samples/actions-show-response.json` & `python-watcher-9.0.0.0rc2/api-ref/source/samples/actions-show-response.json`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/api-ref/source/samples/api-root-response.json` & `python-watcher-9.0.0.0rc2/api-ref/source/samples/api-root-response.json`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/api-ref/source/samples/api-v1-root-response.json` & `python-watcher-9.0.0.0rc2/api-ref/source/samples/api-v1-root-response.json`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/api-ref/source/samples/audit-cancel-response.json` & `python-watcher-9.0.0.0rc2/api-ref/source/samples/audit-cancel-response.json`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/api-ref/source/samples/audit-create-response.json` & `python-watcher-9.0.0.0rc2/api-ref/source/samples/audit-create-response.json`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/api-ref/source/samples/audit-list-detailed-response.json` & `python-watcher-9.0.0.0rc2/api-ref/source/samples/audit-list-detailed-response.json`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/api-ref/source/samples/audit-list-response.json` & `python-watcher-9.0.0.0rc2/api-ref/source/samples/audit-list-response.json`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/api-ref/source/samples/audit-show-response.json` & `python-watcher-9.0.0.0rc2/api-ref/source/samples/audit-show-response.json`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/api-ref/source/samples/audit-update-response.json` & `python-watcher-9.0.0.0rc2/api-ref/source/samples/audit-update-response.json`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/api-ref/source/samples/audittemplate-create-response.json` & `python-watcher-9.0.0.0rc2/api-ref/source/samples/audittemplate-create-response.json`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/api-ref/source/samples/audittemplate-list-detailed-response.json` & `python-watcher-9.0.0.0rc2/api-ref/source/samples/audittemplate-list-detailed-response.json`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/api-ref/source/samples/audittemplate-list-response.json` & `python-watcher-9.0.0.0rc2/api-ref/source/samples/audittemplate-list-response.json`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/api-ref/source/samples/audittemplate-show-response.json` & `python-watcher-9.0.0.0rc2/api-ref/source/samples/audittemplate-show-response.json`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/api-ref/source/samples/audittemplate-update-response.json` & `python-watcher-9.0.0.0rc2/api-ref/source/samples/audittemplate-update-response.json`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/api-ref/source/samples/datamodel-list-response.json` & `python-watcher-9.0.0.0rc2/api-ref/source/samples/datamodel-list-response.json`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/api-ref/source/samples/goal-list-response.json` & `python-watcher-9.0.0.0rc2/api-ref/source/samples/goal-list-response.json`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/api-ref/source/samples/goal-show-response.json` & `python-watcher-9.0.0.0rc2/api-ref/source/samples/goal-show-response.json`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/api-ref/source/samples/scoring_engine-list-detailed-response.json` & `python-watcher-9.0.0.0rc2/api-ref/source/samples/scoring_engine-list-detailed-response.json`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/api-ref/source/samples/scoring_engine-list-response.json` & `python-watcher-9.0.0.0rc2/api-ref/source/samples/scoring_engine-list-response.json`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/api-ref/source/samples/service-list-detailed-response.json` & `python-watcher-9.0.0.0rc2/api-ref/source/samples/service-list-detailed-response.json`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/api-ref/source/samples/service-list-response.json` & `python-watcher-9.0.0.0rc2/api-ref/source/samples/service-list-response.json`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/api-ref/source/samples/service-show-response.json` & `python-watcher-9.0.0.0rc2/api-ref/source/samples/service-show-response.json`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/api-ref/source/samples/strategy-list-detailed-response.json` & `python-watcher-9.0.0.0rc2/api-ref/source/samples/strategy-list-detailed-response.json`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/api-ref/source/samples/strategy-list-response.json` & `python-watcher-9.0.0.0rc2/api-ref/source/samples/strategy-list-response.json`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/api-ref/source/samples/strategy-show-response.json` & `python-watcher-9.0.0.0rc2/api-ref/source/samples/strategy-show-response.json`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/api-ref/source/samples/strategy-state-response.json` & `python-watcher-9.0.0.0rc2/api-ref/source/samples/strategy-state-response.json`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/api-ref/source/watcher-api-v1-actionplans.inc` & `python-watcher-9.0.0.0rc2/api-ref/source/watcher-api-v1-actionplans.inc`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/api-ref/source/watcher-api-v1-actions.inc` & `python-watcher-9.0.0.0rc2/api-ref/source/watcher-api-v1-actions.inc`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/api-ref/source/watcher-api-v1-audits.inc` & `python-watcher-9.0.0.0rc2/api-ref/source/watcher-api-v1-audits.inc`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/api-ref/source/watcher-api-v1-audittemplates.inc` & `python-watcher-9.0.0.0rc2/api-ref/source/watcher-api-v1-audittemplates.inc`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/api-ref/source/watcher-api-v1-datamodel.inc` & `python-watcher-9.0.0.0rc2/api-ref/source/watcher-api-v1-datamodel.inc`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/api-ref/source/watcher-api-v1-goals.inc` & `python-watcher-9.0.0.0rc2/api-ref/source/watcher-api-v1-goals.inc`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/api-ref/source/watcher-api-v1-scoring_engines.inc` & `python-watcher-9.0.0.0rc2/api-ref/source/watcher-api-v1-scoring_engines.inc`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/api-ref/source/watcher-api-v1-services.inc` & `python-watcher-9.0.0.0rc2/api-ref/source/watcher-api-v1-services.inc`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/api-ref/source/watcher-api-v1-strategies.inc` & `python-watcher-9.0.0.0rc2/api-ref/source/watcher-api-v1-strategies.inc`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/api-ref/source/watcher-api-versions.inc` & `python-watcher-9.0.0.0rc2/api-ref/source/watcher-api-versions.inc`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/devstack/files/apache-watcher-api.template` & `python-watcher-9.0.0.0rc2/devstack/files/apache-watcher-api.template`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/devstack/lib/watcher` & `python-watcher-9.0.0.0rc2/devstack/lib/watcher`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/devstack/local.conf.compute` & `python-watcher-9.0.0.0rc2/devstack/local.conf.compute`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/devstack/local.conf.controller` & `python-watcher-9.0.0.0rc2/devstack/local.conf.controller`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/devstack/plugin.sh` & `python-watcher-9.0.0.0rc2/devstack/plugin.sh`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/devstack/upgrade/resources.sh` & `python-watcher-9.0.0.0rc2/devstack/upgrade/resources.sh`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/devstack/upgrade/settings` & `python-watcher-9.0.0.0rc2/devstack/upgrade/settings`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/devstack/upgrade/shutdown.sh` & `python-watcher-9.0.0.0rc2/devstack/upgrade/shutdown.sh`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/devstack/upgrade/upgrade.sh` & `python-watcher-9.0.0.0rc2/devstack/upgrade/upgrade.sh`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/doc/ext/term.py` & `python-watcher-9.0.0.0rc2/doc/ext/term.py`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/doc/ext/versioned_notifications.py` & `python-watcher-9.0.0.0rc2/doc/ext/versioned_notifications.py`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/doc/notification_samples/action-cancel-end.json` & `python-watcher-9.0.0.0rc2/doc/notification_samples/action-cancel-end.json`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/doc/notification_samples/action-cancel-error.json` & `python-watcher-9.0.0.0rc2/doc/notification_samples/action-cancel-error.json`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/doc/notification_samples/action-cancel-start.json` & `python-watcher-9.0.0.0rc2/doc/notification_samples/action-cancel-start.json`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/doc/notification_samples/action-create.json` & `python-watcher-9.0.0.0rc2/doc/notification_samples/action-create.json`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/doc/notification_samples/action-delete.json` & `python-watcher-9.0.0.0rc2/doc/notification_samples/action-delete.json`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/doc/notification_samples/action-execution-end.json` & `python-watcher-9.0.0.0rc2/doc/notification_samples/action-execution-end.json`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/doc/notification_samples/action-execution-error.json` & `python-watcher-9.0.0.0rc2/doc/notification_samples/action-execution-error.json`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/doc/notification_samples/action-execution-start.json` & `python-watcher-9.0.0.0rc2/doc/notification_samples/action-execution-start.json`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/doc/notification_samples/action-update.json` & `python-watcher-9.0.0.0rc2/doc/notification_samples/action-update.json`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/doc/notification_samples/action_plan-cancel-end.json` & `python-watcher-9.0.0.0rc2/doc/notification_samples/action_plan-cancel-end.json`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/doc/notification_samples/action_plan-cancel-error.json` & `python-watcher-9.0.0.0rc2/doc/notification_samples/action_plan-cancel-error.json`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/doc/notification_samples/action_plan-cancel-start.json` & `python-watcher-9.0.0.0rc2/doc/notification_samples/action_plan-cancel-start.json`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/doc/notification_samples/action_plan-create.json` & `python-watcher-9.0.0.0rc2/doc/notification_samples/action_plan-create.json`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/doc/notification_samples/action_plan-delete.json` & `python-watcher-9.0.0.0rc2/doc/notification_samples/action_plan-delete.json`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/doc/notification_samples/action_plan-execution-end.json` & `python-watcher-9.0.0.0rc2/doc/notification_samples/action_plan-execution-end.json`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/doc/notification_samples/action_plan-execution-error.json` & `python-watcher-9.0.0.0rc2/doc/notification_samples/action_plan-execution-error.json`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/doc/notification_samples/action_plan-execution-start.json` & `python-watcher-9.0.0.0rc2/doc/notification_samples/action_plan-execution-start.json`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/doc/notification_samples/action_plan-update.json` & `python-watcher-9.0.0.0rc2/doc/notification_samples/action_plan-update.json`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/doc/notification_samples/audit-create.json` & `python-watcher-9.0.0.0rc2/doc/notification_samples/audit-create.json`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/doc/notification_samples/audit-delete.json` & `python-watcher-9.0.0.0rc2/doc/notification_samples/audit-delete.json`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/doc/notification_samples/audit-planner-end.json` & `python-watcher-9.0.0.0rc2/doc/notification_samples/audit-planner-end.json`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/doc/notification_samples/audit-planner-error.json` & `python-watcher-9.0.0.0rc2/doc/notification_samples/audit-planner-error.json`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/doc/notification_samples/audit-planner-start.json` & `python-watcher-9.0.0.0rc2/doc/notification_samples/audit-planner-start.json`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/doc/notification_samples/audit-strategy-end.json` & `python-watcher-9.0.0.0rc2/doc/notification_samples/audit-strategy-end.json`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/doc/notification_samples/audit-strategy-error.json` & `python-watcher-9.0.0.0rc2/doc/notification_samples/audit-strategy-error.json`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/doc/notification_samples/audit-strategy-start.json` & `python-watcher-9.0.0.0rc2/doc/notification_samples/audit-strategy-start.json`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/doc/notification_samples/audit-update.json` & `python-watcher-9.0.0.0rc2/doc/notification_samples/audit-update.json`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/doc/notification_samples/infra-optim-exception.json` & `python-watcher-9.0.0.0rc2/doc/notification_samples/infra-optim-exception.json`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/doc/notification_samples/service-update.json` & `python-watcher-9.0.0.0rc2/doc/notification_samples/service-update.json`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/doc/source/admin/apache-mod-wsgi.rst` & `python-watcher-9.0.0.0rc2/doc/source/admin/apache-mod-wsgi.rst`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/doc/source/admin/gmr.rst` & `python-watcher-9.0.0.0rc2/doc/source/admin/gmr.rst`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/doc/source/admin/policy.rst` & `python-watcher-9.0.0.0rc2/doc/source/admin/policy.rst`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/doc/source/architecture.rst` & `python-watcher-9.0.0.0rc2/doc/source/architecture.rst`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/doc/source/conf.py` & `python-watcher-9.0.0.0rc2/doc/source/conf.py`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/doc/source/configuration/configuring.rst` & `python-watcher-9.0.0.0rc2/doc/source/configuration/configuring.rst`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/doc/source/contributor/concurrency.rst` & `python-watcher-9.0.0.0rc2/doc/source/contributor/concurrency.rst`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/doc/source/contributor/contributing.rst` & `python-watcher-9.0.0.0rc2/doc/source/contributor/contributing.rst`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/doc/source/contributor/devstack.rst` & `python-watcher-9.0.0.0rc2/doc/source/contributor/devstack.rst`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/doc/source/contributor/environment.rst` & `python-watcher-9.0.0.0rc2/doc/source/contributor/environment.rst`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/doc/source/contributor/plugin/action-plugin.rst` & `python-watcher-9.0.0.0rc2/doc/source/contributor/plugin/action-plugin.rst`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/doc/source/contributor/plugin/base-setup.rst` & `python-watcher-9.0.0.0rc2/doc/source/contributor/plugin/base-setup.rst`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/doc/source/contributor/plugin/cdmc-plugin.rst` & `python-watcher-9.0.0.0rc2/doc/source/contributor/plugin/cdmc-plugin.rst`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/doc/source/contributor/plugin/goal-plugin.rst` & `python-watcher-9.0.0.0rc2/doc/source/contributor/plugin/goal-plugin.rst`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/doc/source/contributor/plugin/planner-plugin.rst` & `python-watcher-9.0.0.0rc2/doc/source/contributor/plugin/planner-plugin.rst`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/doc/source/contributor/plugin/plugins.rst` & `python-watcher-9.0.0.0rc2/doc/source/contributor/plugin/plugins.rst`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/doc/source/contributor/plugin/scoring-engine-plugin.rst` & `python-watcher-9.0.0.0rc2/doc/source/contributor/plugin/scoring-engine-plugin.rst`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/doc/source/contributor/plugin/strategy-plugin.rst` & `python-watcher-9.0.0.0rc2/doc/source/contributor/plugin/strategy-plugin.rst`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/doc/source/contributor/testing.rst` & `python-watcher-9.0.0.0rc2/doc/source/contributor/testing.rst`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/doc/source/datasources/grafana.rst` & `python-watcher-9.0.0.0rc2/doc/source/datasources/grafana.rst`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/doc/source/glossary.rst` & `python-watcher-9.0.0.0rc2/doc/source/glossary.rst`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/doc/source/image_src/dia/architecture.dia` & `python-watcher-9.0.0.0rc2/doc/source/image_src/dia/architecture.dia`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/doc/source/image_src/dia/functional_data_model.dia` & `python-watcher-9.0.0.0rc2/doc/source/image_src/dia/functional_data_model.dia`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/doc/source/image_src/plantuml/action_plan_state_machine.txt` & `python-watcher-9.0.0.0rc2/doc/source/image_src/plantuml/action_plan_state_machine.txt`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/doc/source/image_src/plantuml/audit_state_machine.txt` & `python-watcher-9.0.0.0rc2/doc/source/image_src/plantuml/audit_state_machine.txt`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/doc/source/image_src/plantuml/sequence_architecture_cdmc_sync.txt` & `python-watcher-9.0.0.0rc2/doc/source/image_src/plantuml/sequence_architecture_cdmc_sync.txt`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/doc/source/image_src/plantuml/sequence_create_and_launch_audit.txt` & `python-watcher-9.0.0.0rc2/doc/source/image_src/plantuml/sequence_create_and_launch_audit.txt`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/doc/source/image_src/plantuml/sequence_create_audit_template.txt` & `python-watcher-9.0.0.0rc2/doc/source/image_src/plantuml/sequence_create_audit_template.txt`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/doc/source/image_src/plantuml/sequence_from_audit_execution_to_actionplan_creation.txt` & `python-watcher-9.0.0.0rc2/doc/source/image_src/plantuml/sequence_from_audit_execution_to_actionplan_creation.txt`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/doc/source/image_src/plantuml/sequence_launch_action_plan.txt` & `python-watcher-9.0.0.0rc2/doc/source/image_src/plantuml/sequence_launch_action_plan.txt`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/doc/source/image_src/plantuml/sequence_launch_action_plan_in_applier.txt` & `python-watcher-9.0.0.0rc2/doc/source/image_src/plantuml/sequence_launch_action_plan_in_applier.txt`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/doc/source/image_src/plantuml/sequence_overview_watcher_usage.txt` & `python-watcher-9.0.0.0rc2/doc/source/image_src/plantuml/sequence_overview_watcher_usage.txt`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/doc/source/image_src/plantuml/sequence_trigger_audit_in_decision_engine.txt` & `python-watcher-9.0.0.0rc2/doc/source/image_src/plantuml/sequence_trigger_audit_in_decision_engine.txt`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/doc/source/image_src/plantuml/watcher_db_schema_diagram.txt` & `python-watcher-9.0.0.0rc2/doc/source/image_src/plantuml/watcher_db_schema_diagram.txt`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/doc/source/images/action_plan_state_machine.png` & `python-watcher-9.0.0.0rc2/doc/source/images/action_plan_state_machine.png`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/doc/source/images/architecture.svg` & `python-watcher-9.0.0.0rc2/doc/source/images/architecture.svg`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/doc/source/images/audit_state_machine.png` & `python-watcher-9.0.0.0rc2/doc/source/images/audit_state_machine.png`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/doc/source/images/functional_data_model.svg` & `python-watcher-9.0.0.0rc2/doc/source/images/functional_data_model.svg`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/doc/source/images/sequence_architecture_cdmc_sync.png` & `python-watcher-9.0.0.0rc2/doc/source/images/sequence_architecture_cdmc_sync.png`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/doc/source/images/sequence_create_and_launch_audit.png` & `python-watcher-9.0.0.0rc2/doc/source/images/sequence_create_and_launch_audit.png`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/doc/source/images/sequence_create_audit_template.png` & `python-watcher-9.0.0.0rc2/doc/source/images/sequence_create_audit_template.png`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/doc/source/images/sequence_from_audit_execution_to_actionplan_creation.png` & `python-watcher-9.0.0.0rc2/doc/source/images/sequence_from_audit_execution_to_actionplan_creation.png`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/doc/source/images/sequence_launch_action_plan.png` & `python-watcher-9.0.0.0rc2/doc/source/images/sequence_launch_action_plan.png`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/doc/source/images/sequence_launch_action_plan_in_applier.png` & `python-watcher-9.0.0.0rc2/doc/source/images/sequence_launch_action_plan_in_applier.png`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/doc/source/images/sequence_overview_watcher_usage.png` & `python-watcher-9.0.0.0rc2/doc/source/images/sequence_overview_watcher_usage.png`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/doc/source/images/sequence_trigger_audit_in_decision_engine.png` & `python-watcher-9.0.0.0rc2/doc/source/images/sequence_trigger_audit_in_decision_engine.png`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/doc/source/images/watcher_db_schema_diagram.png` & `python-watcher-9.0.0.0rc2/doc/source/images/watcher_db_schema_diagram.png`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/doc/source/index.rst` & `python-watcher-9.0.0.0rc2/doc/source/index.rst`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/doc/source/install/common_configure.rst` & `python-watcher-9.0.0.0rc2/doc/source/install/common_configure.rst`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/doc/source/install/common_prerequisites.rst` & `python-watcher-9.0.0.0rc2/doc/source/install/common_prerequisites.rst`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/doc/source/install/get_started.rst` & `python-watcher-9.0.0.0rc2/doc/source/install/get_started.rst`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/doc/source/install/index.rst` & `python-watcher-9.0.0.0rc2/doc/source/install/index.rst`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/doc/source/install/install-rdo.rst` & `python-watcher-9.0.0.0rc2/doc/source/install/install-rdo.rst`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/doc/source/install/install-ubuntu.rst` & `python-watcher-9.0.0.0rc2/doc/source/install/install-ubuntu.rst`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/doc/source/install/install.rst` & `python-watcher-9.0.0.0rc2/doc/source/install/install.rst`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/doc/source/install/verify.rst` & `python-watcher-9.0.0.0rc2/doc/source/install/verify.rst`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/doc/source/man/general-options.rst` & `python-watcher-9.0.0.0rc2/doc/source/man/general-options.rst`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/doc/source/man/watcher-api.rst` & `python-watcher-9.0.0.0rc2/doc/source/man/watcher-api.rst`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/doc/source/man/watcher-applier.rst` & `python-watcher-9.0.0.0rc2/doc/source/man/watcher-applier.rst`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/doc/source/man/watcher-db-manage.rst` & `python-watcher-9.0.0.0rc2/doc/source/man/watcher-db-manage.rst`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/doc/source/man/watcher-decision-engine.rst` & `python-watcher-9.0.0.0rc2/doc/source/man/watcher-decision-engine.rst`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/doc/source/man/watcher-status.rst` & `python-watcher-9.0.0.0rc2/doc/source/man/watcher-status.rst`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/doc/source/strategies/actuation.rst` & `python-watcher-9.0.0.0rc2/doc/source/strategies/actuation.rst`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/doc/source/strategies/basic-server-consolidation.rst` & `python-watcher-9.0.0.0rc2/doc/source/strategies/basic-server-consolidation.rst`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/doc/source/strategies/host_maintenance.rst` & `python-watcher-9.0.0.0rc2/doc/source/strategies/host_maintenance.rst`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/doc/source/strategies/node_resource_consolidation.rst` & `python-watcher-9.0.0.0rc2/doc/source/strategies/node_resource_consolidation.rst`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/doc/source/strategies/noisy_neighbor.rst` & `python-watcher-9.0.0.0rc2/doc/source/strategies/noisy_neighbor.rst`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/doc/source/strategies/outlet_temp_control.rst` & `python-watcher-9.0.0.0rc2/doc/source/strategies/outlet_temp_control.rst`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/doc/source/strategies/saving_energy.rst` & `python-watcher-9.0.0.0rc2/doc/source/strategies/saving_energy.rst`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/doc/source/strategies/storage_capacity_balance.rst` & `python-watcher-9.0.0.0rc2/doc/source/strategies/storage_capacity_balance.rst`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/doc/source/strategies/strategy-template.rst` & `python-watcher-9.0.0.0rc2/doc/source/strategies/strategy-template.rst`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/doc/source/strategies/uniform_airflow.rst` & `python-watcher-9.0.0.0rc2/doc/source/strategies/uniform_airflow.rst`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/doc/source/strategies/vm_workload_consolidation.rst` & `python-watcher-9.0.0.0rc2/doc/source/strategies/vm_workload_consolidation.rst`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/doc/source/strategies/workload-stabilization.rst` & `python-watcher-9.0.0.0rc2/doc/source/strategies/workload-stabilization.rst`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/doc/source/strategies/workload_balance.rst` & `python-watcher-9.0.0.0rc2/doc/source/strategies/workload_balance.rst`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/doc/source/strategies/zone_migration.rst` & `python-watcher-9.0.0.0rc2/doc/source/strategies/zone_migration.rst`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/doc/source/user/event_type_audit.rst` & `python-watcher-9.0.0.0rc2/doc/source/user/event_type_audit.rst`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/doc/source/user/user-guide.rst` & `python-watcher-9.0.0.0rc2/doc/source/user/user-guide.rst`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/doc/source/user/ways-to-install.rst` & `python-watcher-9.0.0.0rc2/doc/source/user/ways-to-install.rst`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/etc/apache2/watcher` & `python-watcher-9.0.0.0rc2/etc/apache2/watcher`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/python_watcher.egg-info/PKG-INFO` & `python-watcher-9.0.0.0rc2/python_watcher.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: python-watcher
-Version: 9.0.0.0rc1
+Version: 9.0.0.0rc2
 Summary: OpenStack Watcher provides a flexible and scalable resource optimization service for multi-tenant OpenStack-based clouds.
 Home-page: https://docs.openstack.org/watcher/latest/
 Author: OpenStack
 Author-email: openstack-discuss@lists.openstack.org
 License: UNKNOWN
 Description: =======
         Watcher
```

### Comparing `python-watcher-9.0.0.0rc1/python_watcher.egg-info/SOURCES.txt` & `python-watcher-9.0.0.0rc2/python_watcher.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/python_watcher.egg-info/entry_points.txt` & `python-watcher-9.0.0.0rc2/python_watcher.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/python_watcher.egg-info/requires.txt` & `python-watcher-9.0.0.0rc2/python_watcher.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/rally-jobs/README.rst` & `python-watcher-9.0.0.0rc2/rally-jobs/README.rst`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/rally-jobs/watcher-watcher.yaml` & `python-watcher-9.0.0.0rc2/rally-jobs/watcher-watcher.yaml`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/releasenotes/notes/consume-nova-versioned-notifications-f98361b37e546b4d.yaml` & `python-watcher-9.0.0.0rc2/releasenotes/notes/consume-nova-versioned-notifications-f98361b37e546b4d.yaml`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/releasenotes/notes/datasource-query-retry-00cba5f7e68aec39.yaml` & `python-watcher-9.0.0.0rc2/releasenotes/notes/datasource-query-retry-00cba5f7e68aec39.yaml`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/releasenotes/notes/deprecate-json-formatted-policy-file-3a92379e9f5dd203.yaml` & `python-watcher-9.0.0.0rc2/releasenotes/notes/deprecate-json-formatted-policy-file-3a92379e9f5dd203.yaml`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/releasenotes/notes/enhance-watcher-applier-engine-86c676ce8f179e68.yaml` & `python-watcher-9.0.0.0rc2/releasenotes/notes/enhance-watcher-applier-engine-86c676ce8f179e68.yaml`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/releasenotes/notes/file-based-metric-map-c2af62b5067895df.yaml` & `python-watcher-9.0.0.0rc2/releasenotes/notes/file-based-metric-map-c2af62b5067895df.yaml`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/releasenotes/notes/formal-datasource-interface-implementation-222769d55a127d33.yaml` & `python-watcher-9.0.0.0rc2/releasenotes/notes/formal-datasource-interface-implementation-222769d55a127d33.yaml`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/releasenotes/notes/general-purpose-decision-engine-threadpool-0711b23abfc9d409.yaml` & `python-watcher-9.0.0.0rc2/releasenotes/notes/general-purpose-decision-engine-threadpool-0711b23abfc9d409.yaml`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/releasenotes/notes/grafana-datasource-b672367c23ffa0c6.yaml` & `python-watcher-9.0.0.0rc2/releasenotes/notes/grafana-datasource-b672367c23ffa0c6.yaml`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/releasenotes/notes/improve-compute-data-model-b427c85e4ed2b6fb.yaml` & `python-watcher-9.0.0.0rc2/releasenotes/notes/improve-compute-data-model-b427c85e4ed2b6fb.yaml`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/releasenotes/notes/replace-cold-migrate-to-use-nova-migration-api-cecd9a39ddd3bc58.yaml` & `python-watcher-9.0.0.0rc2/releasenotes/notes/replace-cold-migrate-to-use-nova-migration-api-cecd9a39ddd3bc58.yaml`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/releasenotes/notes/show-datamodel-api-6945b744fd5d25d5.yaml` & `python-watcher-9.0.0.0rc2/releasenotes/notes/show-datamodel-api-6945b744fd5d25d5.yaml`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/releasenotes/source/conf.py` & `python-watcher-9.0.0.0rc2/releasenotes/source/conf.py`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/releasenotes/source/index.rst` & `python-watcher-9.0.0.0rc2/releasenotes/source/index.rst`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/releasenotes/source/locale/en_GB/LC_MESSAGES/releasenotes.po` & `python-watcher-9.0.0.0rc2/releasenotes/source/locale/en_GB/LC_MESSAGES/releasenotes.po`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/releasenotes/source/locale/fr/LC_MESSAGES/releasenotes.po` & `python-watcher-9.0.0.0rc2/releasenotes/source/locale/fr/LC_MESSAGES/releasenotes.po`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/requirements.txt` & `python-watcher-9.0.0.0rc2/requirements.txt`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/setup.cfg` & `python-watcher-9.0.0.0rc2/setup.cfg`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/setup.py` & `python-watcher-9.0.0.0rc2/setup.py`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/test-requirements.txt` & `python-watcher-9.0.0.0rc2/test-requirements.txt`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/tox.ini` & `python-watcher-9.0.0.0rc2/tox.ini`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/watcher/__init__.py` & `python-watcher-9.0.0.0rc2/watcher/__init__.py`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/watcher/_i18n.py` & `python-watcher-9.0.0.0rc2/watcher/_i18n.py`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/watcher/api/acl.py` & `python-watcher-9.0.0.0rc2/watcher/api/acl.py`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/watcher/api/app.py` & `python-watcher-9.0.0.0rc2/watcher/api/app.py`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/watcher/api/app.wsgi` & `python-watcher-9.0.0.0rc2/watcher/api/app.wsgi`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/watcher/api/config.py` & `python-watcher-9.0.0.0rc2/watcher/api/config.py`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/watcher/api/controllers/base.py` & `python-watcher-9.0.0.0rc2/watcher/api/controllers/base.py`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/watcher/api/controllers/link.py` & `python-watcher-9.0.0.0rc2/watcher/api/controllers/link.py`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/watcher/api/controllers/rest_api_version_history.rst` & `python-watcher-9.0.0.0rc2/watcher/api/controllers/rest_api_version_history.rst`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/watcher/api/controllers/root.py` & `python-watcher-9.0.0.0rc2/watcher/api/controllers/root.py`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/watcher/api/controllers/v1/__init__.py` & `python-watcher-9.0.0.0rc2/watcher/api/controllers/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/watcher/api/controllers/v1/action.py` & `python-watcher-9.0.0.0rc2/watcher/api/controllers/v1/action.py`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/watcher/api/controllers/v1/action_plan.py` & `python-watcher-9.0.0.0rc2/watcher/api/controllers/v1/action_plan.py`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/watcher/api/controllers/v1/audit.py` & `python-watcher-9.0.0.0rc2/watcher/api/controllers/v1/audit.py`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/watcher/api/controllers/v1/audit_template.py` & `python-watcher-9.0.0.0rc2/watcher/api/controllers/v1/audit_template.py`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/watcher/api/controllers/v1/collection.py` & `python-watcher-9.0.0.0rc2/watcher/api/controllers/v1/collection.py`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/watcher/api/controllers/v1/data_model.py` & `python-watcher-9.0.0.0rc2/watcher/api/controllers/v1/data_model.py`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/watcher/api/controllers/v1/efficacy_indicator.py` & `python-watcher-9.0.0.0rc2/watcher/api/controllers/v1/efficacy_indicator.py`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/watcher/api/controllers/v1/goal.py` & `python-watcher-9.0.0.0rc2/watcher/api/controllers/v1/goal.py`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/watcher/api/controllers/v1/scoring_engine.py` & `python-watcher-9.0.0.0rc2/watcher/api/controllers/v1/scoring_engine.py`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/watcher/api/controllers/v1/service.py` & `python-watcher-9.0.0.0rc2/watcher/api/controllers/v1/service.py`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/watcher/api/controllers/v1/strategy.py` & `python-watcher-9.0.0.0rc2/watcher/api/controllers/v1/strategy.py`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/watcher/api/controllers/v1/types.py` & `python-watcher-9.0.0.0rc2/watcher/api/controllers/v1/types.py`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/watcher/api/controllers/v1/utils.py` & `python-watcher-9.0.0.0rc2/watcher/api/controllers/v1/utils.py`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/watcher/api/controllers/v1/versions.py` & `python-watcher-9.0.0.0rc2/watcher/api/controllers/v1/versions.py`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/watcher/api/controllers/v1/webhooks.py` & `python-watcher-9.0.0.0rc2/watcher/api/controllers/v1/webhooks.py`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/watcher/api/hooks.py` & `python-watcher-9.0.0.0rc2/watcher/api/hooks.py`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/watcher/api/middleware/auth_token.py` & `python-watcher-9.0.0.0rc2/watcher/api/middleware/auth_token.py`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/watcher/api/middleware/parsable_error.py` & `python-watcher-9.0.0.0rc2/watcher/api/middleware/parsable_error.py`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/watcher/api/scheduling.py` & `python-watcher-9.0.0.0rc2/watcher/api/scheduling.py`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/watcher/api/wsgi.py` & `python-watcher-9.0.0.0rc2/watcher/api/wsgi.py`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/watcher/applier/action_plan/base.py` & `python-watcher-9.0.0.0rc2/watcher/applier/action_plan/base.py`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/watcher/applier/action_plan/default.py` & `python-watcher-9.0.0.0rc2/watcher/applier/action_plan/default.py`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/watcher/applier/actions/base.py` & `python-watcher-9.0.0.0rc2/watcher/applier/actions/base.py`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/watcher/applier/actions/change_node_power_state.py` & `python-watcher-9.0.0.0rc2/watcher/applier/actions/change_node_power_state.py`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/watcher/applier/actions/change_nova_service_state.py` & `python-watcher-9.0.0.0rc2/watcher/applier/actions/change_nova_service_state.py`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/watcher/applier/actions/factory.py` & `python-watcher-9.0.0.0rc2/watcher/applier/actions/factory.py`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/watcher/applier/actions/migration.py` & `python-watcher-9.0.0.0rc2/watcher/applier/actions/migration.py`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/watcher/applier/actions/nop.py` & `python-watcher-9.0.0.0rc2/watcher/applier/actions/nop.py`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/watcher/applier/actions/resize.py` & `python-watcher-9.0.0.0rc2/watcher/applier/actions/resize.py`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/watcher/applier/actions/sleep.py` & `python-watcher-9.0.0.0rc2/watcher/applier/actions/sleep.py`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/watcher/applier/actions/volume_migration.py` & `python-watcher-9.0.0.0rc2/watcher/applier/actions/volume_migration.py`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/watcher/applier/base.py` & `python-watcher-9.0.0.0rc2/watcher/applier/base.py`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/watcher/applier/default.py` & `python-watcher-9.0.0.0rc2/watcher/applier/default.py`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/watcher/applier/loading/default.py` & `python-watcher-9.0.0.0rc2/watcher/applier/loading/default.py`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/watcher/applier/manager.py` & `python-watcher-9.0.0.0rc2/watcher/applier/manager.py`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/watcher/applier/messaging/trigger.py` & `python-watcher-9.0.0.0rc2/watcher/applier/messaging/trigger.py`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/watcher/applier/rpcapi.py` & `python-watcher-9.0.0.0rc2/watcher/applier/rpcapi.py`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/watcher/applier/sync.py` & `python-watcher-9.0.0.0rc2/watcher/applier/sync.py`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/watcher/applier/workflow_engine/base.py` & `python-watcher-9.0.0.0rc2/watcher/applier/workflow_engine/base.py`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/watcher/applier/workflow_engine/default.py` & `python-watcher-9.0.0.0rc2/watcher/applier/workflow_engine/default.py`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/watcher/cmd/__init__.py` & `python-watcher-9.0.0.0rc2/watcher/cmd/__init__.py`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/watcher/cmd/api.py` & `python-watcher-9.0.0.0rc2/watcher/cmd/api.py`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/watcher/cmd/applier.py` & `python-watcher-9.0.0.0rc2/watcher/cmd/applier.py`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/watcher/cmd/dbmanage.py` & `python-watcher-9.0.0.0rc2/watcher/cmd/dbmanage.py`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/watcher/cmd/decisionengine.py` & `python-watcher-9.0.0.0rc2/watcher/cmd/decisionengine.py`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/watcher/cmd/status.py` & `python-watcher-9.0.0.0rc2/watcher/cmd/status.py`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/watcher/cmd/sync.py` & `python-watcher-9.0.0.0rc2/watcher/cmd/sync.py`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/watcher/common/cinder_helper.py` & `python-watcher-9.0.0.0rc2/watcher/common/cinder_helper.py`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/watcher/common/clients.py` & `python-watcher-9.0.0.0rc2/watcher/common/clients.py`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/watcher/common/config.py` & `python-watcher-9.0.0.0rc2/watcher/common/config.py`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/watcher/common/context.py` & `python-watcher-9.0.0.0rc2/watcher/common/context.py`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/watcher/common/exception.py` & `python-watcher-9.0.0.0rc2/watcher/common/exception.py`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/watcher/common/ironic_helper.py` & `python-watcher-9.0.0.0rc2/watcher/common/ironic_helper.py`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/watcher/common/keystone_helper.py` & `python-watcher-9.0.0.0rc2/watcher/common/keystone_helper.py`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/watcher/common/loader/base.py` & `python-watcher-9.0.0.0rc2/watcher/common/loader/base.py`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/watcher/common/loader/default.py` & `python-watcher-9.0.0.0rc2/watcher/common/loader/default.py`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/watcher/common/loader/loadable.py` & `python-watcher-9.0.0.0rc2/watcher/common/loader/loadable.py`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/watcher/common/nova_helper.py` & `python-watcher-9.0.0.0rc2/watcher/common/nova_helper.py`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/watcher/common/paths.py` & `python-watcher-9.0.0.0rc2/watcher/common/paths.py`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/watcher/common/placement_helper.py` & `python-watcher-9.0.0.0rc2/watcher/common/placement_helper.py`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/watcher/common/policies/__init__.py` & `python-watcher-9.0.0.0rc2/watcher/common/policies/__init__.py`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/watcher/common/policies/action.py` & `python-watcher-9.0.0.0rc2/watcher/common/policies/action.py`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/watcher/common/policies/action_plan.py` & `python-watcher-9.0.0.0rc2/watcher/common/policies/action_plan.py`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/watcher/common/policies/audit.py` & `python-watcher-9.0.0.0rc2/watcher/common/policies/audit.py`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/watcher/common/policies/audit_template.py` & `python-watcher-9.0.0.0rc2/watcher/common/policies/audit_template.py`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/watcher/common/policies/base.py` & `python-watcher-9.0.0.0rc2/watcher/common/policies/base.py`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/watcher/common/policies/data_model.py` & `python-watcher-9.0.0.0rc2/watcher/common/policies/data_model.py`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/watcher/common/policies/goal.py` & `python-watcher-9.0.0.0rc2/watcher/common/policies/goal.py`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/watcher/common/policies/scoring_engine.py` & `python-watcher-9.0.0.0rc2/watcher/common/policies/scoring_engine.py`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/watcher/common/policies/service.py` & `python-watcher-9.0.0.0rc2/watcher/common/policies/service.py`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/watcher/common/policies/strategy.py` & `python-watcher-9.0.0.0rc2/watcher/common/policies/strategy.py`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/watcher/common/policy.py` & `python-watcher-9.0.0.0rc2/watcher/common/policy.py`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/watcher/common/rpc.py` & `python-watcher-9.0.0.0rc2/watcher/common/rpc.py`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/watcher/common/scheduling.py` & `python-watcher-9.0.0.0rc2/watcher/common/scheduling.py`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/watcher/common/service.py` & `python-watcher-9.0.0.0rc2/watcher/common/service.py`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/watcher/common/service_manager.py` & `python-watcher-9.0.0.0rc2/watcher/common/service_manager.py`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/watcher/common/utils.py` & `python-watcher-9.0.0.0rc2/watcher/common/utils.py`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/watcher/conf/__init__.py` & `python-watcher-9.0.0.0rc2/watcher/conf/__init__.py`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/watcher/conf/api.py` & `python-watcher-9.0.0.0rc2/watcher/conf/api.py`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/watcher/conf/applier.py` & `python-watcher-9.0.0.0rc2/watcher/conf/applier.py`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/watcher/conf/ceilometer_client.py` & `python-watcher-9.0.0.0rc2/watcher/conf/ceilometer_client.py`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/watcher/conf/cinder_client.py` & `python-watcher-9.0.0.0rc2/watcher/conf/cinder_client.py`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/watcher/conf/clients_auth.py` & `python-watcher-9.0.0.0rc2/watcher/conf/clients_auth.py`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/watcher/conf/collector.py` & `python-watcher-9.0.0.0rc2/watcher/conf/collector.py`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/watcher/conf/datasources.py` & `python-watcher-9.0.0.0rc2/watcher/conf/datasources.py`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/watcher/conf/db.py` & `python-watcher-9.0.0.0rc2/watcher/conf/db.py`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/watcher/conf/decision_engine.py` & `python-watcher-9.0.0.0rc2/watcher/conf/decision_engine.py`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/watcher/conf/exception.py` & `python-watcher-9.0.0.0rc2/watcher/conf/exception.py`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/watcher/conf/glance_client.py` & `python-watcher-9.0.0.0rc2/watcher/conf/glance_client.py`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/watcher/conf/gnocchi_client.py` & `python-watcher-9.0.0.0rc2/watcher/conf/gnocchi_client.py`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/watcher/conf/grafana_client.py` & `python-watcher-9.0.0.0rc2/watcher/conf/grafana_client.py`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/watcher/conf/grafana_translators.py` & `python-watcher-9.0.0.0rc2/watcher/conf/grafana_translators.py`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/watcher/conf/ironic_client.py` & `python-watcher-9.0.0.0rc2/watcher/conf/ironic_client.py`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/watcher/conf/keystone_client.py` & `python-watcher-9.0.0.0rc2/watcher/conf/keystone_client.py`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/watcher/conf/monasca_client.py` & `python-watcher-9.0.0.0rc2/watcher/conf/monasca_client.py`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/watcher/conf/neutron_client.py` & `python-watcher-9.0.0.0rc2/watcher/conf/neutron_client.py`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/watcher/conf/nova_client.py` & `python-watcher-9.0.0.0rc2/watcher/conf/nova_client.py`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/watcher/conf/opts.py` & `python-watcher-9.0.0.0rc2/watcher/conf/opts.py`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/watcher/conf/paths.py` & `python-watcher-9.0.0.0rc2/watcher/conf/paths.py`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/watcher/conf/placement_client.py` & `python-watcher-9.0.0.0rc2/watcher/conf/placement_client.py`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/watcher/conf/planner.py` & `python-watcher-9.0.0.0rc2/watcher/conf/planner.py`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/watcher/conf/plugins.py` & `python-watcher-9.0.0.0rc2/watcher/conf/plugins.py`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/watcher/conf/service.py` & `python-watcher-9.0.0.0rc2/watcher/conf/service.py`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/watcher/db/api.py` & `python-watcher-9.0.0.0rc2/watcher/db/api.py`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/watcher/db/migration.py` & `python-watcher-9.0.0.0rc2/watcher/db/migration.py`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/watcher/db/purge.py` & `python-watcher-9.0.0.0rc2/watcher/db/purge.py`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/watcher/db/sqlalchemy/alembic/README.rst` & `python-watcher-9.0.0.0rc2/watcher/db/sqlalchemy/alembic/README.rst`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/watcher/db/sqlalchemy/alembic/env.py` & `python-watcher-9.0.0.0rc2/watcher/db/sqlalchemy/alembic/env.py`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/watcher/db/sqlalchemy/alembic/versions/001_ocata.py` & `python-watcher-9.0.0.0rc2/watcher/db/sqlalchemy/alembic/versions/001_ocata.py`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/watcher/db/sqlalchemy/alembic/versions/0f6042416884_add_apscheduler_jobs.py` & `python-watcher-9.0.0.0rc2/watcher/db/sqlalchemy/alembic/versions/0f6042416884_add_apscheduler_jobs.py`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/watcher/db/sqlalchemy/alembic/versions/4b16194c56bc_add_start_end_time.py` & `python-watcher-9.0.0.0rc2/watcher/db/sqlalchemy/alembic/versions/4b16194c56bc_add_start_end_time.py`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/watcher/db/sqlalchemy/alembic/versions/52804f2498c4_add_hostname.py` & `python-watcher-9.0.0.0rc2/watcher/db/sqlalchemy/alembic/versions/52804f2498c4_add_hostname.py`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/watcher/db/sqlalchemy/alembic/versions/a86240e89a29_.py` & `python-watcher-9.0.0.0rc2/watcher/db/sqlalchemy/alembic/versions/a86240e89a29_.py`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/watcher/db/sqlalchemy/alembic/versions/d098df6021e2_cron_support_for_audit.py` & `python-watcher-9.0.0.0rc2/watcher/db/sqlalchemy/alembic/versions/d098df6021e2_cron_support_for_audit.py`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/watcher/db/sqlalchemy/alembic/versions/d09a5945e4a0_add_action_description_table.py` & `python-watcher-9.0.0.0rc2/watcher/db/sqlalchemy/alembic/versions/d09a5945e4a0_add_action_description_table.py`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/watcher/db/sqlalchemy/alembic.ini` & `python-watcher-9.0.0.0rc2/watcher/db/sqlalchemy/alembic.ini`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/watcher/db/sqlalchemy/api.py` & `python-watcher-9.0.0.0rc2/watcher/db/sqlalchemy/api.py`

 * *Files 0% similar despite different names*

```diff
@@ -40,15 +40,19 @@
 
 _FACADE = None
 
 
 def _create_facade_lazily():
     global _FACADE
     if _FACADE is None:
-        _FACADE = db_session.EngineFacade.from_config(CONF)
+        # FIXME(amoralej): Remove autocommit=True (and ideally use of
+        # LegacyEngineFacade) asap since it's not compatible with SQLAlchemy
+        # 2.0.
+        _FACADE = db_session.EngineFacade.from_config(CONF,
+                                                      autocommit=True)
     return _FACADE
 
 
 def get_engine():
     facade = _create_facade_lazily()
     return facade.get_engine()
```

### Comparing `python-watcher-9.0.0.0rc1/watcher/db/sqlalchemy/job_store.py` & `python-watcher-9.0.0.0rc2/watcher/db/sqlalchemy/job_store.py`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/watcher/db/sqlalchemy/migration.py` & `python-watcher-9.0.0.0rc2/watcher/db/sqlalchemy/migration.py`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/watcher/db/sqlalchemy/models.py` & `python-watcher-9.0.0.0rc2/watcher/db/sqlalchemy/models.py`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/watcher/decision_engine/audit/base.py` & `python-watcher-9.0.0.0rc2/watcher/decision_engine/audit/base.py`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/watcher/decision_engine/audit/continuous.py` & `python-watcher-9.0.0.0rc2/watcher/decision_engine/audit/continuous.py`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/watcher/decision_engine/audit/event.py` & `python-watcher-9.0.0.0rc2/watcher/decision_engine/audit/event.py`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/watcher/decision_engine/audit/oneshot.py` & `python-watcher-9.0.0.0rc2/watcher/decision_engine/audit/oneshot.py`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/watcher/decision_engine/datasources/base.py` & `python-watcher-9.0.0.0rc2/watcher/decision_engine/datasources/base.py`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/watcher/decision_engine/datasources/ceilometer.py` & `python-watcher-9.0.0.0rc2/watcher/decision_engine/datasources/ceilometer.py`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/watcher/decision_engine/datasources/gnocchi.py` & `python-watcher-9.0.0.0rc2/watcher/decision_engine/datasources/gnocchi.py`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/watcher/decision_engine/datasources/grafana.py` & `python-watcher-9.0.0.0rc2/watcher/decision_engine/datasources/grafana.py`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/watcher/decision_engine/datasources/grafana_translator/base.py` & `python-watcher-9.0.0.0rc2/watcher/decision_engine/datasources/grafana_translator/base.py`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/watcher/decision_engine/datasources/grafana_translator/influxdb.py` & `python-watcher-9.0.0.0rc2/watcher/decision_engine/datasources/grafana_translator/influxdb.py`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/watcher/decision_engine/datasources/manager.py` & `python-watcher-9.0.0.0rc2/watcher/decision_engine/datasources/manager.py`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/watcher/decision_engine/datasources/monasca.py` & `python-watcher-9.0.0.0rc2/watcher/decision_engine/datasources/monasca.py`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/watcher/decision_engine/gmr.py` & `python-watcher-9.0.0.0rc2/watcher/decision_engine/gmr.py`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/watcher/decision_engine/goal/__init__.py` & `python-watcher-9.0.0.0rc2/watcher/decision_engine/goal/__init__.py`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/watcher/decision_engine/goal/base.py` & `python-watcher-9.0.0.0rc2/watcher/decision_engine/goal/base.py`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/watcher/decision_engine/goal/efficacy/base.py` & `python-watcher-9.0.0.0rc2/watcher/decision_engine/goal/efficacy/base.py`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/watcher/decision_engine/goal/efficacy/indicators.py` & `python-watcher-9.0.0.0rc2/watcher/decision_engine/goal/efficacy/indicators.py`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/watcher/decision_engine/goal/efficacy/specs.py` & `python-watcher-9.0.0.0rc2/watcher/decision_engine/goal/efficacy/specs.py`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/watcher/decision_engine/goal/goals.py` & `python-watcher-9.0.0.0rc2/watcher/decision_engine/goal/goals.py`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/watcher/decision_engine/loading/default.py` & `python-watcher-9.0.0.0rc2/watcher/decision_engine/loading/default.py`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/watcher/decision_engine/manager.py` & `python-watcher-9.0.0.0rc2/watcher/decision_engine/manager.py`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/watcher/decision_engine/messaging/audit_endpoint.py` & `python-watcher-9.0.0.0rc2/watcher/decision_engine/messaging/audit_endpoint.py`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/watcher/decision_engine/messaging/data_model_endpoint.py` & `python-watcher-9.0.0.0rc2/watcher/decision_engine/messaging/data_model_endpoint.py`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/watcher/decision_engine/model/base.py` & `python-watcher-9.0.0.0rc2/watcher/decision_engine/model/base.py`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/watcher/decision_engine/model/collector/base.py` & `python-watcher-9.0.0.0rc2/watcher/decision_engine/model/collector/base.py`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/watcher/decision_engine/model/collector/cinder.py` & `python-watcher-9.0.0.0rc2/watcher/decision_engine/model/collector/cinder.py`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/watcher/decision_engine/model/collector/ironic.py` & `python-watcher-9.0.0.0rc2/watcher/decision_engine/model/collector/ironic.py`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/watcher/decision_engine/model/collector/manager.py` & `python-watcher-9.0.0.0rc2/watcher/decision_engine/model/collector/manager.py`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/watcher/decision_engine/model/collector/nova.py` & `python-watcher-9.0.0.0rc2/watcher/decision_engine/model/collector/nova.py`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/watcher/decision_engine/model/element/__init__.py` & `python-watcher-9.0.0.0rc2/watcher/decision_engine/model/element/__init__.py`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/watcher/decision_engine/model/element/baremetal_resource.py` & `python-watcher-9.0.0.0rc2/watcher/decision_engine/model/element/baremetal_resource.py`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/watcher/decision_engine/model/element/base.py` & `python-watcher-9.0.0.0rc2/watcher/decision_engine/model/element/base.py`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/watcher/decision_engine/model/element/compute_resource.py` & `python-watcher-9.0.0.0rc2/watcher/decision_engine/model/element/compute_resource.py`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/watcher/decision_engine/model/element/instance.py` & `python-watcher-9.0.0.0rc2/watcher/decision_engine/model/element/instance.py`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/watcher/decision_engine/model/element/node.py` & `python-watcher-9.0.0.0rc2/watcher/decision_engine/model/element/node.py`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/watcher/decision_engine/model/element/storage_resource.py` & `python-watcher-9.0.0.0rc2/watcher/decision_engine/model/element/storage_resource.py`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/watcher/decision_engine/model/element/volume.py` & `python-watcher-9.0.0.0rc2/watcher/decision_engine/model/element/volume.py`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/watcher/decision_engine/model/model_root.py` & `python-watcher-9.0.0.0rc2/watcher/decision_engine/model/model_root.py`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/watcher/decision_engine/model/notification/base.py` & `python-watcher-9.0.0.0rc2/watcher/decision_engine/model/notification/base.py`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/watcher/decision_engine/model/notification/cinder.py` & `python-watcher-9.0.0.0rc2/watcher/decision_engine/model/notification/cinder.py`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/watcher/decision_engine/model/notification/filtering.py` & `python-watcher-9.0.0.0rc2/watcher/decision_engine/model/notification/filtering.py`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/watcher/decision_engine/model/notification/nova.py` & `python-watcher-9.0.0.0rc2/watcher/decision_engine/model/notification/nova.py`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/watcher/decision_engine/planner/base.py` & `python-watcher-9.0.0.0rc2/watcher/decision_engine/planner/base.py`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/watcher/decision_engine/planner/manager.py` & `python-watcher-9.0.0.0rc2/watcher/decision_engine/planner/manager.py`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/watcher/decision_engine/planner/node_resource_consolidation.py` & `python-watcher-9.0.0.0rc2/watcher/decision_engine/planner/node_resource_consolidation.py`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/watcher/decision_engine/planner/weight.py` & `python-watcher-9.0.0.0rc2/watcher/decision_engine/planner/weight.py`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/watcher/decision_engine/planner/workload_stabilization.py` & `python-watcher-9.0.0.0rc2/watcher/decision_engine/planner/workload_stabilization.py`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/watcher/decision_engine/rpcapi.py` & `python-watcher-9.0.0.0rc2/watcher/decision_engine/rpcapi.py`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/watcher/decision_engine/scheduling.py` & `python-watcher-9.0.0.0rc2/watcher/decision_engine/scheduling.py`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/watcher/decision_engine/scope/baremetal.py` & `python-watcher-9.0.0.0rc2/watcher/decision_engine/scope/baremetal.py`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/watcher/decision_engine/scope/base.py` & `python-watcher-9.0.0.0rc2/watcher/decision_engine/scope/base.py`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/watcher/decision_engine/scope/compute.py` & `python-watcher-9.0.0.0rc2/watcher/decision_engine/scope/compute.py`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/watcher/decision_engine/scope/storage.py` & `python-watcher-9.0.0.0rc2/watcher/decision_engine/scope/storage.py`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/watcher/decision_engine/scoring/base.py` & `python-watcher-9.0.0.0rc2/watcher/decision_engine/scoring/base.py`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/watcher/decision_engine/scoring/dummy_scorer.py` & `python-watcher-9.0.0.0rc2/watcher/decision_engine/scoring/dummy_scorer.py`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/watcher/decision_engine/scoring/dummy_scoring_container.py` & `python-watcher-9.0.0.0rc2/watcher/decision_engine/scoring/dummy_scoring_container.py`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/watcher/decision_engine/scoring/scoring_factory.py` & `python-watcher-9.0.0.0rc2/watcher/decision_engine/scoring/scoring_factory.py`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/watcher/decision_engine/solution/base.py` & `python-watcher-9.0.0.0rc2/watcher/decision_engine/solution/base.py`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/watcher/decision_engine/solution/default.py` & `python-watcher-9.0.0.0rc2/watcher/decision_engine/solution/default.py`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/watcher/decision_engine/solution/efficacy.py` & `python-watcher-9.0.0.0rc2/watcher/decision_engine/solution/efficacy.py`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/watcher/decision_engine/solution/solution_comparator.py` & `python-watcher-9.0.0.0rc2/watcher/decision_engine/solution/solution_comparator.py`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/watcher/decision_engine/solution/solution_evaluator.py` & `python-watcher-9.0.0.0rc2/watcher/decision_engine/solution/solution_evaluator.py`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/watcher/decision_engine/strategy/common/level.py` & `python-watcher-9.0.0.0rc2/watcher/decision_engine/strategy/common/level.py`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/watcher/decision_engine/strategy/context/base.py` & `python-watcher-9.0.0.0rc2/watcher/decision_engine/strategy/context/base.py`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/watcher/decision_engine/strategy/context/default.py` & `python-watcher-9.0.0.0rc2/watcher/decision_engine/strategy/context/default.py`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/watcher/decision_engine/strategy/selection/base.py` & `python-watcher-9.0.0.0rc2/watcher/decision_engine/strategy/selection/base.py`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/watcher/decision_engine/strategy/selection/default.py` & `python-watcher-9.0.0.0rc2/watcher/decision_engine/strategy/selection/default.py`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/watcher/decision_engine/strategy/strategies/__init__.py` & `python-watcher-9.0.0.0rc2/watcher/decision_engine/strategy/strategies/__init__.py`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/watcher/decision_engine/strategy/strategies/actuation.py` & `python-watcher-9.0.0.0rc2/watcher/decision_engine/strategy/strategies/actuation.py`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/watcher/decision_engine/strategy/strategies/base.py` & `python-watcher-9.0.0.0rc2/watcher/decision_engine/strategy/strategies/base.py`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/watcher/decision_engine/strategy/strategies/basic_consolidation.py` & `python-watcher-9.0.0.0rc2/watcher/decision_engine/strategy/strategies/basic_consolidation.py`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/watcher/decision_engine/strategy/strategies/dummy_strategy.py` & `python-watcher-9.0.0.0rc2/watcher/decision_engine/strategy/strategies/dummy_strategy.py`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/watcher/decision_engine/strategy/strategies/dummy_with_resize.py` & `python-watcher-9.0.0.0rc2/watcher/decision_engine/strategy/strategies/dummy_with_resize.py`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/watcher/decision_engine/strategy/strategies/dummy_with_scorer.py` & `python-watcher-9.0.0.0rc2/watcher/decision_engine/strategy/strategies/dummy_with_scorer.py`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/watcher/decision_engine/strategy/strategies/host_maintenance.py` & `python-watcher-9.0.0.0rc2/watcher/decision_engine/strategy/strategies/host_maintenance.py`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/watcher/decision_engine/strategy/strategies/node_resource_consolidation.py` & `python-watcher-9.0.0.0rc2/watcher/decision_engine/strategy/strategies/node_resource_consolidation.py`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/watcher/decision_engine/strategy/strategies/noisy_neighbor.py` & `python-watcher-9.0.0.0rc2/watcher/decision_engine/strategy/strategies/noisy_neighbor.py`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/watcher/decision_engine/strategy/strategies/outlet_temp_control.py` & `python-watcher-9.0.0.0rc2/watcher/decision_engine/strategy/strategies/outlet_temp_control.py`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/watcher/decision_engine/strategy/strategies/saving_energy.py` & `python-watcher-9.0.0.0rc2/watcher/decision_engine/strategy/strategies/saving_energy.py`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/watcher/decision_engine/strategy/strategies/storage_capacity_balance.py` & `python-watcher-9.0.0.0rc2/watcher/decision_engine/strategy/strategies/storage_capacity_balance.py`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/watcher/decision_engine/strategy/strategies/uniform_airflow.py` & `python-watcher-9.0.0.0rc2/watcher/decision_engine/strategy/strategies/uniform_airflow.py`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/watcher/decision_engine/strategy/strategies/vm_workload_consolidation.py` & `python-watcher-9.0.0.0rc2/watcher/decision_engine/strategy/strategies/vm_workload_consolidation.py`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/watcher/decision_engine/strategy/strategies/workload_balance.py` & `python-watcher-9.0.0.0rc2/watcher/decision_engine/strategy/strategies/workload_balance.py`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/watcher/decision_engine/strategy/strategies/workload_stabilization.py` & `python-watcher-9.0.0.0rc2/watcher/decision_engine/strategy/strategies/workload_stabilization.py`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/watcher/decision_engine/strategy/strategies/zone_migration.py` & `python-watcher-9.0.0.0rc2/watcher/decision_engine/strategy/strategies/zone_migration.py`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/watcher/decision_engine/sync.py` & `python-watcher-9.0.0.0rc2/watcher/decision_engine/sync.py`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/watcher/decision_engine/threading.py` & `python-watcher-9.0.0.0rc2/watcher/decision_engine/threading.py`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/watcher/hacking/checks.py` & `python-watcher-9.0.0.0rc2/watcher/hacking/checks.py`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/watcher/locale/de/LC_MESSAGES/watcher.po` & `python-watcher-9.0.0.0rc2/watcher/locale/de/LC_MESSAGES/watcher.po`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/watcher/locale/en_GB/LC_MESSAGES/watcher.po` & `python-watcher-9.0.0.0rc2/watcher/locale/en_GB/LC_MESSAGES/watcher.po`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/watcher/notifications/__init__.py` & `python-watcher-9.0.0.0rc2/watcher/notifications/__init__.py`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/watcher/notifications/action.py` & `python-watcher-9.0.0.0rc2/watcher/notifications/action.py`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/watcher/notifications/action_plan.py` & `python-watcher-9.0.0.0rc2/watcher/notifications/action_plan.py`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/watcher/notifications/audit.py` & `python-watcher-9.0.0.0rc2/watcher/notifications/audit.py`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/watcher/notifications/base.py` & `python-watcher-9.0.0.0rc2/watcher/notifications/base.py`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/watcher/notifications/exception.py` & `python-watcher-9.0.0.0rc2/watcher/notifications/exception.py`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/watcher/notifications/goal.py` & `python-watcher-9.0.0.0rc2/watcher/notifications/goal.py`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/watcher/notifications/service.py` & `python-watcher-9.0.0.0rc2/watcher/notifications/service.py`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/watcher/notifications/strategy.py` & `python-watcher-9.0.0.0rc2/watcher/notifications/strategy.py`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/watcher/objects/__init__.py` & `python-watcher-9.0.0.0rc2/watcher/objects/__init__.py`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/watcher/objects/action.py` & `python-watcher-9.0.0.0rc2/watcher/objects/action.py`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/watcher/objects/action_description.py` & `python-watcher-9.0.0.0rc2/watcher/objects/action_description.py`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/watcher/objects/action_plan.py` & `python-watcher-9.0.0.0rc2/watcher/objects/action_plan.py`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/watcher/objects/audit.py` & `python-watcher-9.0.0.0rc2/watcher/objects/audit.py`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/watcher/objects/audit_template.py` & `python-watcher-9.0.0.0rc2/watcher/objects/audit_template.py`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/watcher/objects/base.py` & `python-watcher-9.0.0.0rc2/watcher/objects/base.py`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/watcher/objects/efficacy_indicator.py` & `python-watcher-9.0.0.0rc2/watcher/objects/efficacy_indicator.py`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/watcher/objects/fields.py` & `python-watcher-9.0.0.0rc2/watcher/objects/fields.py`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/watcher/objects/goal.py` & `python-watcher-9.0.0.0rc2/watcher/objects/goal.py`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/watcher/objects/scoring_engine.py` & `python-watcher-9.0.0.0rc2/watcher/objects/scoring_engine.py`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/watcher/objects/service.py` & `python-watcher-9.0.0.0rc2/watcher/objects/service.py`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/watcher/objects/strategy.py` & `python-watcher-9.0.0.0rc2/watcher/objects/strategy.py`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/watcher/tests/__init__.py` & `python-watcher-9.0.0.0rc2/watcher/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/watcher/tests/api/base.py` & `python-watcher-9.0.0.0rc2/watcher/tests/api/base.py`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/watcher/tests/api/test_base.py` & `python-watcher-9.0.0.0rc2/watcher/tests/api/test_base.py`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/watcher/tests/api/test_config.py` & `python-watcher-9.0.0.0rc2/watcher/tests/api/test_config.py`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/watcher/tests/api/test_hooks.py` & `python-watcher-9.0.0.0rc2/watcher/tests/api/test_hooks.py`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/watcher/tests/api/test_root.py` & `python-watcher-9.0.0.0rc2/watcher/tests/api/test_root.py`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/watcher/tests/api/test_scheduling.py` & `python-watcher-9.0.0.0rc2/watcher/tests/api/test_scheduling.py`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/watcher/tests/api/test_utils.py` & `python-watcher-9.0.0.0rc2/watcher/tests/api/test_utils.py`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/watcher/tests/api/utils.py` & `python-watcher-9.0.0.0rc2/watcher/tests/api/utils.py`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/watcher/tests/api/v1/test_actions.py` & `python-watcher-9.0.0.0rc2/watcher/tests/api/v1/test_actions.py`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/watcher/tests/api/v1/test_actions_plans.py` & `python-watcher-9.0.0.0rc2/watcher/tests/api/v1/test_actions_plans.py`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/watcher/tests/api/v1/test_audit_templates.py` & `python-watcher-9.0.0.0rc2/watcher/tests/api/v1/test_audit_templates.py`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/watcher/tests/api/v1/test_audits.py` & `python-watcher-9.0.0.0rc2/watcher/tests/api/v1/test_audits.py`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/watcher/tests/api/v1/test_data_model.py` & `python-watcher-9.0.0.0rc2/watcher/tests/api/v1/test_data_model.py`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/watcher/tests/api/v1/test_goals.py` & `python-watcher-9.0.0.0rc2/watcher/tests/api/v1/test_goals.py`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/watcher/tests/api/v1/test_microversions.py` & `python-watcher-9.0.0.0rc2/watcher/tests/api/v1/test_microversions.py`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/watcher/tests/api/v1/test_root.py` & `python-watcher-9.0.0.0rc2/watcher/tests/api/v1/test_root.py`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/watcher/tests/api/v1/test_scoring_engines.py` & `python-watcher-9.0.0.0rc2/watcher/tests/api/v1/test_scoring_engines.py`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/watcher/tests/api/v1/test_services.py` & `python-watcher-9.0.0.0rc2/watcher/tests/api/v1/test_services.py`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/watcher/tests/api/v1/test_strategies.py` & `python-watcher-9.0.0.0rc2/watcher/tests/api/v1/test_strategies.py`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/watcher/tests/api/v1/test_types.py` & `python-watcher-9.0.0.0rc2/watcher/tests/api/v1/test_types.py`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/watcher/tests/api/v1/test_utils.py` & `python-watcher-9.0.0.0rc2/watcher/tests/api/v1/test_utils.py`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/watcher/tests/api/v1/test_webhooks.py` & `python-watcher-9.0.0.0rc2/watcher/tests/api/v1/test_webhooks.py`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/watcher/tests/applier/action_plan/test_default_action_handler.py` & `python-watcher-9.0.0.0rc2/watcher/tests/applier/action_plan/test_default_action_handler.py`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/watcher/tests/applier/actions/loading/test_default_actions_loader.py` & `python-watcher-9.0.0.0rc2/watcher/tests/applier/actions/loading/test_default_actions_loader.py`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/watcher/tests/applier/actions/test_change_node_power_state.py` & `python-watcher-9.0.0.0rc2/watcher/tests/applier/actions/test_change_node_power_state.py`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/watcher/tests/applier/actions/test_change_nova_service_state.py` & `python-watcher-9.0.0.0rc2/watcher/tests/applier/actions/test_change_nova_service_state.py`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/watcher/tests/applier/actions/test_migration.py` & `python-watcher-9.0.0.0rc2/watcher/tests/applier/actions/test_migration.py`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/watcher/tests/applier/actions/test_resize.py` & `python-watcher-9.0.0.0rc2/watcher/tests/applier/actions/test_resize.py`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/watcher/tests/applier/actions/test_sleep.py` & `python-watcher-9.0.0.0rc2/watcher/tests/applier/actions/test_sleep.py`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/watcher/tests/applier/actions/test_volume_migration.py` & `python-watcher-9.0.0.0rc2/watcher/tests/applier/actions/test_volume_migration.py`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/watcher/tests/applier/messaging/test_trigger_action_plan_endpoint.py` & `python-watcher-9.0.0.0rc2/watcher/tests/applier/messaging/test_trigger_action_plan_endpoint.py`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/watcher/tests/applier/test_applier_manager.py` & `python-watcher-9.0.0.0rc2/watcher/tests/applier/test_applier_manager.py`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/watcher/tests/applier/test_rpcapi.py` & `python-watcher-9.0.0.0rc2/watcher/tests/applier/test_rpcapi.py`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/watcher/tests/applier/test_sync.py` & `python-watcher-9.0.0.0rc2/watcher/tests/applier/test_sync.py`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/watcher/tests/applier/workflow_engine/loading/test_default_engine_loader.py` & `python-watcher-9.0.0.0rc2/watcher/tests/applier/workflow_engine/loading/test_default_engine_loader.py`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/watcher/tests/applier/workflow_engine/test_default_workflow_engine.py` & `python-watcher-9.0.0.0rc2/watcher/tests/applier/workflow_engine/test_default_workflow_engine.py`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/watcher/tests/applier/workflow_engine/test_taskflow_action_container.py` & `python-watcher-9.0.0.0rc2/watcher/tests/applier/workflow_engine/test_taskflow_action_container.py`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/watcher/tests/base.py` & `python-watcher-9.0.0.0rc2/watcher/tests/base.py`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/watcher/tests/cmd/test_api.py` & `python-watcher-9.0.0.0rc2/watcher/tests/cmd/test_api.py`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/watcher/tests/cmd/test_applier.py` & `python-watcher-9.0.0.0rc2/watcher/tests/cmd/test_applier.py`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/watcher/tests/cmd/test_db_manage.py` & `python-watcher-9.0.0.0rc2/watcher/tests/cmd/test_db_manage.py`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/watcher/tests/cmd/test_decision_engine.py` & `python-watcher-9.0.0.0rc2/watcher/tests/cmd/test_decision_engine.py`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/watcher/tests/cmd/test_status.py` & `python-watcher-9.0.0.0rc2/watcher/tests/cmd/test_status.py`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/watcher/tests/common/loader/test_loader.py` & `python-watcher-9.0.0.0rc2/watcher/tests/common/loader/test_loader.py`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/watcher/tests/common/test_cinder_helper.py` & `python-watcher-9.0.0.0rc2/watcher/tests/common/test_cinder_helper.py`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/watcher/tests/common/test_clients.py` & `python-watcher-9.0.0.0rc2/watcher/tests/common/test_clients.py`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/watcher/tests/common/test_ironic_helper.py` & `python-watcher-9.0.0.0rc2/watcher/tests/common/test_ironic_helper.py`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/watcher/tests/common/test_nova_helper.py` & `python-watcher-9.0.0.0rc2/watcher/tests/common/test_nova_helper.py`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/watcher/tests/common/test_placement_helper.py` & `python-watcher-9.0.0.0rc2/watcher/tests/common/test_placement_helper.py`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/watcher/tests/common/test_service.py` & `python-watcher-9.0.0.0rc2/watcher/tests/common/test_service.py`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/watcher/tests/conf/test_list_opts.py` & `python-watcher-9.0.0.0rc2/watcher/tests/conf/test_list_opts.py`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/watcher/tests/conf_fixture.py` & `python-watcher-9.0.0.0rc2/watcher/tests/conf_fixture.py`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/watcher/tests/config.py` & `python-watcher-9.0.0.0rc2/watcher/tests/config.py`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/watcher/tests/db/base.py` & `python-watcher-9.0.0.0rc2/watcher/tests/db/base.py`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/watcher/tests/db/test_action.py` & `python-watcher-9.0.0.0rc2/watcher/tests/db/test_action.py`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/watcher/tests/db/test_action_description.py` & `python-watcher-9.0.0.0rc2/watcher/tests/db/test_action_description.py`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/watcher/tests/db/test_action_plan.py` & `python-watcher-9.0.0.0rc2/watcher/tests/db/test_action_plan.py`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/watcher/tests/db/test_audit.py` & `python-watcher-9.0.0.0rc2/watcher/tests/db/test_audit.py`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/watcher/tests/db/test_audit_template.py` & `python-watcher-9.0.0.0rc2/watcher/tests/db/test_audit_template.py`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/watcher/tests/db/test_efficacy_indicator.py` & `python-watcher-9.0.0.0rc2/watcher/tests/db/test_efficacy_indicator.py`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/watcher/tests/db/test_goal.py` & `python-watcher-9.0.0.0rc2/watcher/tests/db/test_goal.py`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/watcher/tests/db/test_purge.py` & `python-watcher-9.0.0.0rc2/watcher/tests/db/test_purge.py`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/watcher/tests/db/test_scoring_engine.py` & `python-watcher-9.0.0.0rc2/watcher/tests/db/test_scoring_engine.py`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/watcher/tests/db/test_service.py` & `python-watcher-9.0.0.0rc2/watcher/tests/db/test_service.py`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/watcher/tests/db/test_strategy.py` & `python-watcher-9.0.0.0rc2/watcher/tests/db/test_strategy.py`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/watcher/tests/db/utils.py` & `python-watcher-9.0.0.0rc2/watcher/tests/db/utils.py`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/watcher/tests/decision_engine/audit/test_audit_handlers.py` & `python-watcher-9.0.0.0rc2/watcher/tests/decision_engine/audit/test_audit_handlers.py`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/watcher/tests/decision_engine/cluster/test_cinder_cdmc.py` & `python-watcher-9.0.0.0rc2/watcher/tests/decision_engine/cluster/test_cinder_cdmc.py`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/watcher/tests/decision_engine/cluster/test_cluster_data_model_collector.py` & `python-watcher-9.0.0.0rc2/watcher/tests/decision_engine/cluster/test_cluster_data_model_collector.py`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/watcher/tests/decision_engine/cluster/test_nova_cdmc.py` & `python-watcher-9.0.0.0rc2/watcher/tests/decision_engine/cluster/test_nova_cdmc.py`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/watcher/tests/decision_engine/datasources/grafana_translators/test_base.py` & `python-watcher-9.0.0.0rc2/watcher/tests/decision_engine/datasources/grafana_translators/test_base.py`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/watcher/tests/decision_engine/datasources/grafana_translators/test_influxdb.py` & `python-watcher-9.0.0.0rc2/watcher/tests/decision_engine/datasources/grafana_translators/test_influxdb.py`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/watcher/tests/decision_engine/datasources/test_base.py` & `python-watcher-9.0.0.0rc2/watcher/tests/decision_engine/datasources/test_base.py`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/watcher/tests/decision_engine/datasources/test_gnocchi_helper.py` & `python-watcher-9.0.0.0rc2/watcher/tests/decision_engine/datasources/test_gnocchi_helper.py`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/watcher/tests/decision_engine/datasources/test_grafana_helper.py` & `python-watcher-9.0.0.0rc2/watcher/tests/decision_engine/datasources/test_grafana_helper.py`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/watcher/tests/decision_engine/datasources/test_manager.py` & `python-watcher-9.0.0.0rc2/watcher/tests/decision_engine/datasources/test_manager.py`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/watcher/tests/decision_engine/datasources/test_monasca_helper.py` & `python-watcher-9.0.0.0rc2/watcher/tests/decision_engine/datasources/test_monasca_helper.py`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/watcher/tests/decision_engine/fake_goals.py` & `python-watcher-9.0.0.0rc2/watcher/tests/decision_engine/fake_goals.py`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/watcher/tests/decision_engine/fake_strategies.py` & `python-watcher-9.0.0.0rc2/watcher/tests/decision_engine/fake_strategies.py`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/watcher/tests/decision_engine/loading/test_collector_loader.py` & `python-watcher-9.0.0.0rc2/watcher/tests/decision_engine/loading/test_collector_loader.py`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/watcher/tests/decision_engine/loading/test_default_planner_loader.py` & `python-watcher-9.0.0.0rc2/watcher/tests/decision_engine/loading/test_default_planner_loader.py`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/watcher/tests/decision_engine/loading/test_default_strategy_loader.py` & `python-watcher-9.0.0.0rc2/watcher/tests/decision_engine/loading/test_default_strategy_loader.py`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/watcher/tests/decision_engine/loading/test_goal_loader.py` & `python-watcher-9.0.0.0rc2/watcher/tests/decision_engine/loading/test_goal_loader.py`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/watcher/tests/decision_engine/messaging/test_audit_endpoint.py` & `python-watcher-9.0.0.0rc2/watcher/tests/decision_engine/messaging/test_audit_endpoint.py`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/watcher/tests/decision_engine/messaging/test_data_model_endpoint.py` & `python-watcher-9.0.0.0rc2/watcher/tests/decision_engine/messaging/test_data_model_endpoint.py`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/watcher/tests/decision_engine/model/ceilometer_metrics.py` & `python-watcher-9.0.0.0rc2/watcher/tests/decision_engine/model/ceilometer_metrics.py`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/watcher/tests/decision_engine/model/data/scenario_1.xml` & `python-watcher-9.0.0.0rc2/watcher/tests/decision_engine/model/data/scenario_1.xml`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/watcher/tests/decision_engine/model/data/scenario_10.xml` & `python-watcher-9.0.0.0rc2/watcher/tests/decision_engine/model/data/scenario_10.xml`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/watcher/tests/decision_engine/model/data/scenario_1_with_1_node_unavailable.xml` & `python-watcher-9.0.0.0rc2/watcher/tests/decision_engine/model/data/scenario_1_with_1_node_unavailable.xml`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/watcher/tests/decision_engine/model/data/scenario_1_with_all_instances_exclude.xml` & `python-watcher-9.0.0.0rc2/watcher/tests/decision_engine/model/data/scenario_1_with_all_instances_exclude.xml`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/watcher/tests/decision_engine/model/data/scenario_1_with_all_nodes_disable.xml` & `python-watcher-9.0.0.0rc2/watcher/tests/decision_engine/model/data/scenario_1_with_all_nodes_disable.xml`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/watcher/tests/decision_engine/model/data/scenario_1_with_metrics.xml` & `python-watcher-9.0.0.0rc2/watcher/tests/decision_engine/model/data/scenario_1_with_metrics.xml`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/watcher/tests/decision_engine/model/data/scenario_2_with_metrics.xml` & `python-watcher-9.0.0.0rc2/watcher/tests/decision_engine/model/data/scenario_2_with_metrics.xml`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/watcher/tests/decision_engine/model/data/scenario_3_with_2_nodes.xml` & `python-watcher-9.0.0.0rc2/watcher/tests/decision_engine/model/data/scenario_3_with_2_nodes.xml`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/watcher/tests/decision_engine/model/data/scenario_3_with_metrics.xml` & `python-watcher-9.0.0.0rc2/watcher/tests/decision_engine/model/data/scenario_3_with_metrics.xml`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/watcher/tests/decision_engine/model/data/scenario_6_with_2_nodes.xml` & `python-watcher-9.0.0.0rc2/watcher/tests/decision_engine/model/data/scenario_6_with_2_nodes.xml`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/watcher/tests/decision_engine/model/data/scenario_7_with_2_nodes.xml` & `python-watcher-9.0.0.0rc2/watcher/tests/decision_engine/model/data/scenario_7_with_2_nodes.xml`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/watcher/tests/decision_engine/model/data/scenario_8_with_4_nodes.xml` & `python-watcher-9.0.0.0rc2/watcher/tests/decision_engine/model/data/scenario_8_with_4_nodes.xml`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/watcher/tests/decision_engine/model/data/scenario_9_with_3_active_plus_1_disabled_nodes.xml` & `python-watcher-9.0.0.0rc2/watcher/tests/decision_engine/model/data/scenario_9_with_3_active_plus_1_disabled_nodes.xml`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/watcher/tests/decision_engine/model/data/storage_scenario_1.xml` & `python-watcher-9.0.0.0rc2/watcher/tests/decision_engine/model/data/storage_scenario_1.xml`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/watcher/tests/decision_engine/model/faker_cluster_and_metrics.py` & `python-watcher-9.0.0.0rc2/watcher/tests/decision_engine/model/faker_cluster_and_metrics.py`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/watcher/tests/decision_engine/model/faker_cluster_state.py` & `python-watcher-9.0.0.0rc2/watcher/tests/decision_engine/model/faker_cluster_state.py`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/watcher/tests/decision_engine/model/gnocchi_metrics.py` & `python-watcher-9.0.0.0rc2/watcher/tests/decision_engine/model/gnocchi_metrics.py`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/watcher/tests/decision_engine/model/monasca_metrics.py` & `python-watcher-9.0.0.0rc2/watcher/tests/decision_engine/model/monasca_metrics.py`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/watcher/tests/decision_engine/model/notification/data/instance-create-end.json` & `python-watcher-9.0.0.0rc2/watcher/tests/decision_engine/model/notification/data/instance-create-end.json`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/watcher/tests/decision_engine/model/notification/data/instance-delete-end.json` & `python-watcher-9.0.0.0rc2/watcher/tests/decision_engine/model/notification/data/instance-delete-end.json`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/watcher/tests/decision_engine/model/notification/data/instance-live_migration_force_complete-end.json` & `python-watcher-9.0.0.0rc2/watcher/tests/decision_engine/model/notification/data/instance-live_migration_force_complete-end.json`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/watcher/tests/decision_engine/model/notification/data/instance-live_migration_post-end.json` & `python-watcher-9.0.0.0rc2/watcher/tests/decision_engine/model/notification/data/instance-live_migration_post-end.json`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/watcher/tests/decision_engine/model/notification/data/instance-lock.json` & `python-watcher-9.0.0.0rc2/watcher/tests/decision_engine/model/notification/data/instance-lock.json`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/watcher/tests/decision_engine/model/notification/data/instance-pause-end.json` & `python-watcher-9.0.0.0rc2/watcher/tests/decision_engine/model/notification/data/instance-pause-end.json`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/watcher/tests/decision_engine/model/notification/data/instance-power_off-end.json` & `python-watcher-9.0.0.0rc2/watcher/tests/decision_engine/model/notification/data/instance-power_off-end.json`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/watcher/tests/decision_engine/model/notification/data/instance-power_on-end.json` & `python-watcher-9.0.0.0rc2/watcher/tests/decision_engine/model/notification/data/instance-power_on-end.json`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/watcher/tests/decision_engine/model/notification/data/instance-rebuild-end.json` & `python-watcher-9.0.0.0rc2/watcher/tests/decision_engine/model/notification/data/instance-rebuild-end.json`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/watcher/tests/decision_engine/model/notification/data/instance-rescue-end.json` & `python-watcher-9.0.0.0rc2/watcher/tests/decision_engine/model/notification/data/instance-rescue-end.json`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/watcher/tests/decision_engine/model/notification/data/instance-resize_confirm-end.json` & `python-watcher-9.0.0.0rc2/watcher/tests/decision_engine/model/notification/data/instance-resize_confirm-end.json`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/watcher/tests/decision_engine/model/notification/data/instance-restore-end.json` & `python-watcher-9.0.0.0rc2/watcher/tests/decision_engine/model/notification/data/instance-restore-end.json`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/watcher/tests/decision_engine/model/notification/data/instance-resume-end.json` & `python-watcher-9.0.0.0rc2/watcher/tests/decision_engine/model/notification/data/instance-resume-end.json`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/watcher/tests/decision_engine/model/notification/data/instance-shelve-end.json` & `python-watcher-9.0.0.0rc2/watcher/tests/decision_engine/model/notification/data/instance-shelve-end.json`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/watcher/tests/decision_engine/model/notification/data/instance-shutdown-end.json` & `python-watcher-9.0.0.0rc2/watcher/tests/decision_engine/model/notification/data/instance-shutdown-end.json`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/watcher/tests/decision_engine/model/notification/data/instance-soft_delete-end.json` & `python-watcher-9.0.0.0rc2/watcher/tests/decision_engine/model/notification/data/instance-soft_delete-end.json`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/watcher/tests/decision_engine/model/notification/data/instance-suspend-end.json` & `python-watcher-9.0.0.0rc2/watcher/tests/decision_engine/model/notification/data/instance-suspend-end.json`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/watcher/tests/decision_engine/model/notification/data/instance-unlock.json` & `python-watcher-9.0.0.0rc2/watcher/tests/decision_engine/model/notification/data/instance-unlock.json`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/watcher/tests/decision_engine/model/notification/data/instance-unpause-end.json` & `python-watcher-9.0.0.0rc2/watcher/tests/decision_engine/model/notification/data/instance-unpause-end.json`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/watcher/tests/decision_engine/model/notification/data/instance-unrescue-end.json` & `python-watcher-9.0.0.0rc2/watcher/tests/decision_engine/model/notification/data/instance-unrescue-end.json`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/watcher/tests/decision_engine/model/notification/data/instance-unshelve-end.json` & `python-watcher-9.0.0.0rc2/watcher/tests/decision_engine/model/notification/data/instance-unshelve-end.json`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/watcher/tests/decision_engine/model/notification/data/instance-update.json` & `python-watcher-9.0.0.0rc2/watcher/tests/decision_engine/model/notification/data/instance-update.json`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/watcher/tests/decision_engine/model/notification/data/scenario3_instance-update.json` & `python-watcher-9.0.0.0rc2/watcher/tests/decision_engine/model/notification/data/scenario3_instance-update.json`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/watcher/tests/decision_engine/model/notification/data/scenario3_notfound_instance-update.json` & `python-watcher-9.0.0.0rc2/watcher/tests/decision_engine/model/notification/data/scenario3_notfound_instance-update.json`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/watcher/tests/decision_engine/model/notification/data/scenario3_notfound_legacy_instance-update.json` & `python-watcher-9.0.0.0rc2/watcher/tests/decision_engine/model/notification/data/scenario3_notfound_legacy_instance-update.json`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/watcher/tests/decision_engine/model/notification/data/scenario3_service-update-disabled.json` & `python-watcher-9.0.0.0rc2/watcher/tests/decision_engine/model/notification/data/scenario3_service-update-disabled.json`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/watcher/tests/decision_engine/model/notification/data/scenario3_service-update-enabled.json` & `python-watcher-9.0.0.0rc2/watcher/tests/decision_engine/model/notification/data/scenario3_service-update-enabled.json`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/watcher/tests/decision_engine/model/notification/data/scenario_1_bootable-volume-create.json` & `python-watcher-9.0.0.0rc2/watcher/tests/decision_engine/model/notification/data/scenario_1_bootable-volume-create.json`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/watcher/tests/decision_engine/model/notification/data/scenario_1_volume-attach.json` & `python-watcher-9.0.0.0rc2/watcher/tests/decision_engine/model/notification/data/scenario_1_volume-attach.json`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/watcher/tests/decision_engine/model/notification/data/scenario_1_volume-create.json` & `python-watcher-9.0.0.0rc2/watcher/tests/decision_engine/model/notification/data/scenario_1_volume-create.json`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/watcher/tests/decision_engine/model/notification/data/scenario_1_volume-create_pool_notfound.json` & `python-watcher-9.0.0.0rc2/watcher/tests/decision_engine/model/notification/data/scenario_1_volume-create_pool_notfound.json`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/watcher/tests/decision_engine/model/notification/data/scenario_1_volume-delete.json` & `python-watcher-9.0.0.0rc2/watcher/tests/decision_engine/model/notification/data/scenario_1_volume-delete.json`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/watcher/tests/decision_engine/model/notification/data/scenario_1_volume-resize.json` & `python-watcher-9.0.0.0rc2/watcher/tests/decision_engine/model/notification/data/scenario_1_volume-resize.json`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/watcher/tests/decision_engine/model/notification/data/scenario_1_volume-update.json` & `python-watcher-9.0.0.0rc2/watcher/tests/decision_engine/model/notification/data/scenario_1_volume-update.json`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/watcher/tests/decision_engine/model/notification/data/service-create.json` & `python-watcher-9.0.0.0rc2/watcher/tests/decision_engine/model/notification/data/service-create.json`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/watcher/tests/decision_engine/model/notification/data/service-delete.json` & `python-watcher-9.0.0.0rc2/watcher/tests/decision_engine/model/notification/data/service-delete.json`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/watcher/tests/decision_engine/model/notification/data/service-update.json` & `python-watcher-9.0.0.0rc2/watcher/tests/decision_engine/model/notification/data/service-update.json`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/watcher/tests/decision_engine/model/notification/fake_managers.py` & `python-watcher-9.0.0.0rc2/watcher/tests/decision_engine/model/notification/fake_managers.py`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/watcher/tests/decision_engine/model/notification/test_cinder_notifications.py` & `python-watcher-9.0.0.0rc2/watcher/tests/decision_engine/model/notification/test_cinder_notifications.py`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/watcher/tests/decision_engine/model/notification/test_notifications.py` & `python-watcher-9.0.0.0rc2/watcher/tests/decision_engine/model/notification/test_notifications.py`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/watcher/tests/decision_engine/model/notification/test_nova_notifications.py` & `python-watcher-9.0.0.0rc2/watcher/tests/decision_engine/model/notification/test_nova_notifications.py`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/watcher/tests/decision_engine/model/test_element.py` & `python-watcher-9.0.0.0rc2/watcher/tests/decision_engine/model/test_element.py`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/watcher/tests/decision_engine/model/test_model.py` & `python-watcher-9.0.0.0rc2/watcher/tests/decision_engine/model/test_model.py`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/watcher/tests/decision_engine/planner/test_node_resource_consolidation.py` & `python-watcher-9.0.0.0rc2/watcher/tests/decision_engine/planner/test_node_resource_consolidation.py`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/watcher/tests/decision_engine/planner/test_planner_manager.py` & `python-watcher-9.0.0.0rc2/watcher/tests/decision_engine/planner/test_planner_manager.py`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/watcher/tests/decision_engine/planner/test_weight_planner.py` & `python-watcher-9.0.0.0rc2/watcher/tests/decision_engine/planner/test_weight_planner.py`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/watcher/tests/decision_engine/planner/test_workload_stabilization_planner.py` & `python-watcher-9.0.0.0rc2/watcher/tests/decision_engine/planner/test_workload_stabilization_planner.py`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/watcher/tests/decision_engine/scope/fake_scopes.py` & `python-watcher-9.0.0.0rc2/watcher/tests/decision_engine/scope/fake_scopes.py`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/watcher/tests/decision_engine/scope/test_baremetal.py` & `python-watcher-9.0.0.0rc2/watcher/tests/decision_engine/scope/test_baremetal.py`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/watcher/tests/decision_engine/scope/test_compute.py` & `python-watcher-9.0.0.0rc2/watcher/tests/decision_engine/scope/test_compute.py`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/watcher/tests/decision_engine/scope/test_storage.py` & `python-watcher-9.0.0.0rc2/watcher/tests/decision_engine/scope/test_storage.py`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/watcher/tests/decision_engine/scoring/test_dummy_scorer.py` & `python-watcher-9.0.0.0rc2/watcher/tests/decision_engine/scoring/test_dummy_scorer.py`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/watcher/tests/decision_engine/scoring/test_dummy_scoring_container.py` & `python-watcher-9.0.0.0rc2/watcher/tests/decision_engine/scoring/test_dummy_scoring_container.py`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/watcher/tests/decision_engine/scoring/test_scoring_factory.py` & `python-watcher-9.0.0.0rc2/watcher/tests/decision_engine/scoring/test_scoring_factory.py`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/watcher/tests/decision_engine/solution/test_default_solution.py` & `python-watcher-9.0.0.0rc2/watcher/tests/decision_engine/solution/test_default_solution.py`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/watcher/tests/decision_engine/strategy/context/test_strategy_context.py` & `python-watcher-9.0.0.0rc2/watcher/tests/decision_engine/strategy/context/test_strategy_context.py`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/watcher/tests/decision_engine/strategy/selector/test_strategy_selector.py` & `python-watcher-9.0.0.0rc2/watcher/tests/decision_engine/strategy/selector/test_strategy_selector.py`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/watcher/tests/decision_engine/strategy/strategies/test_actuator.py` & `python-watcher-9.0.0.0rc2/watcher/tests/decision_engine/strategy/strategies/test_actuator.py`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/watcher/tests/decision_engine/strategy/strategies/test_base.py` & `python-watcher-9.0.0.0rc2/watcher/tests/decision_engine/strategy/strategies/test_base.py`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/watcher/tests/decision_engine/strategy/strategies/test_basic_consolidation.py` & `python-watcher-9.0.0.0rc2/watcher/tests/decision_engine/strategy/strategies/test_basic_consolidation.py`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/watcher/tests/decision_engine/strategy/strategies/test_dummy_strategy.py` & `python-watcher-9.0.0.0rc2/watcher/tests/decision_engine/strategy/strategies/test_dummy_strategy.py`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/watcher/tests/decision_engine/strategy/strategies/test_dummy_with_scorer.py` & `python-watcher-9.0.0.0rc2/watcher/tests/decision_engine/strategy/strategies/test_dummy_with_scorer.py`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/watcher/tests/decision_engine/strategy/strategies/test_host_maintenance.py` & `python-watcher-9.0.0.0rc2/watcher/tests/decision_engine/strategy/strategies/test_host_maintenance.py`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/watcher/tests/decision_engine/strategy/strategies/test_node_resource_consolidation.py` & `python-watcher-9.0.0.0rc2/watcher/tests/decision_engine/strategy/strategies/test_node_resource_consolidation.py`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/watcher/tests/decision_engine/strategy/strategies/test_noisy_neighbor.py` & `python-watcher-9.0.0.0rc2/watcher/tests/decision_engine/strategy/strategies/test_noisy_neighbor.py`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/watcher/tests/decision_engine/strategy/strategies/test_outlet_temp_control.py` & `python-watcher-9.0.0.0rc2/watcher/tests/decision_engine/strategy/strategies/test_outlet_temp_control.py`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/watcher/tests/decision_engine/strategy/strategies/test_saving_energy.py` & `python-watcher-9.0.0.0rc2/watcher/tests/decision_engine/strategy/strategies/test_saving_energy.py`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/watcher/tests/decision_engine/strategy/strategies/test_storage_capacity_balance.py` & `python-watcher-9.0.0.0rc2/watcher/tests/decision_engine/strategy/strategies/test_storage_capacity_balance.py`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/watcher/tests/decision_engine/strategy/strategies/test_strategy_endpoint.py` & `python-watcher-9.0.0.0rc2/watcher/tests/decision_engine/strategy/strategies/test_strategy_endpoint.py`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/watcher/tests/decision_engine/strategy/strategies/test_uniform_airflow.py` & `python-watcher-9.0.0.0rc2/watcher/tests/decision_engine/strategy/strategies/test_uniform_airflow.py`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/watcher/tests/decision_engine/strategy/strategies/test_vm_workload_consolidation.py` & `python-watcher-9.0.0.0rc2/watcher/tests/decision_engine/strategy/strategies/test_vm_workload_consolidation.py`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/watcher/tests/decision_engine/strategy/strategies/test_workload_balance.py` & `python-watcher-9.0.0.0rc2/watcher/tests/decision_engine/strategy/strategies/test_workload_balance.py`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/watcher/tests/decision_engine/strategy/strategies/test_workload_stabilization.py` & `python-watcher-9.0.0.0rc2/watcher/tests/decision_engine/strategy/strategies/test_workload_stabilization.py`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/watcher/tests/decision_engine/strategy/strategies/test_zone_migration.py` & `python-watcher-9.0.0.0rc2/watcher/tests/decision_engine/strategy/strategies/test_zone_migration.py`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/watcher/tests/decision_engine/test_gmr.py` & `python-watcher-9.0.0.0rc2/watcher/tests/decision_engine/test_gmr.py`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/watcher/tests/decision_engine/test_rpcapi.py` & `python-watcher-9.0.0.0rc2/watcher/tests/decision_engine/test_rpcapi.py`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/watcher/tests/decision_engine/test_scheduling.py` & `python-watcher-9.0.0.0rc2/watcher/tests/decision_engine/test_scheduling.py`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/watcher/tests/decision_engine/test_sync.py` & `python-watcher-9.0.0.0rc2/watcher/tests/decision_engine/test_sync.py`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/watcher/tests/fake_policy.py` & `python-watcher-9.0.0.0rc2/watcher/tests/fake_policy.py`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/watcher/tests/fakes.py` & `python-watcher-9.0.0.0rc2/watcher/tests/fakes.py`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/watcher/tests/notifications/test_action_notification.py` & `python-watcher-9.0.0.0rc2/watcher/tests/notifications/test_action_notification.py`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/watcher/tests/notifications/test_action_plan_notification.py` & `python-watcher-9.0.0.0rc2/watcher/tests/notifications/test_action_plan_notification.py`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/watcher/tests/notifications/test_audit_notification.py` & `python-watcher-9.0.0.0rc2/watcher/tests/notifications/test_audit_notification.py`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/watcher/tests/notifications/test_notification.py` & `python-watcher-9.0.0.0rc2/watcher/tests/notifications/test_notification.py`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/watcher/tests/notifications/test_service_notifications.py` & `python-watcher-9.0.0.0rc2/watcher/tests/notifications/test_service_notifications.py`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/watcher/tests/objects/test_action.py` & `python-watcher-9.0.0.0rc2/watcher/tests/objects/test_action.py`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/watcher/tests/objects/test_action_description.py` & `python-watcher-9.0.0.0rc2/watcher/tests/objects/test_action_description.py`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/watcher/tests/objects/test_action_plan.py` & `python-watcher-9.0.0.0rc2/watcher/tests/objects/test_action_plan.py`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/watcher/tests/objects/test_audit.py` & `python-watcher-9.0.0.0rc2/watcher/tests/objects/test_audit.py`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/watcher/tests/objects/test_audit_template.py` & `python-watcher-9.0.0.0rc2/watcher/tests/objects/test_audit_template.py`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/watcher/tests/objects/test_efficacy_indicator.py` & `python-watcher-9.0.0.0rc2/watcher/tests/objects/test_efficacy_indicator.py`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/watcher/tests/objects/test_goal.py` & `python-watcher-9.0.0.0rc2/watcher/tests/objects/test_goal.py`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/watcher/tests/objects/test_objects.py` & `python-watcher-9.0.0.0rc2/watcher/tests/objects/test_objects.py`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/watcher/tests/objects/test_scoring_engine.py` & `python-watcher-9.0.0.0rc2/watcher/tests/objects/test_scoring_engine.py`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/watcher/tests/objects/test_service.py` & `python-watcher-9.0.0.0rc2/watcher/tests/objects/test_service.py`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/watcher/tests/objects/test_strategy.py` & `python-watcher-9.0.0.0rc2/watcher/tests/objects/test_strategy.py`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/watcher/tests/objects/utils.py` & `python-watcher-9.0.0.0rc2/watcher/tests/objects/utils.py`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/watcher/tests/policy_fixture.py` & `python-watcher-9.0.0.0rc2/watcher/tests/policy_fixture.py`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/watcher/tests/test_threading.py` & `python-watcher-9.0.0.0rc2/watcher/tests/test_threading.py`

 * *Files identical despite different names*

### Comparing `python-watcher-9.0.0.0rc1/watcher/version.py` & `python-watcher-9.0.0.0rc2/watcher/version.py`

 * *Files identical despite different names*

