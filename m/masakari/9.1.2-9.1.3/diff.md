# Comparing `tmp/masakari-9.1.2.tar.gz` & `tmp/masakari-9.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/masakari-9.1.2.tar", last modified: Thu Apr 29 16:51:14 2021, max compression
+gzip compressed data, was "masakari-9.1.3.tar", last modified: Thu Aug 19 12:40:25 2021, max compression
```

## Comparing `masakari-9.1.2.tar` & `masakari-9.1.3.tar`

### file list

```diff
@@ -1,434 +1,435 @@
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-29 16:51:14.269740 masakari-9.1.2/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       97 2021-04-29 16:50:35.000000 masakari-9.1.2/.coveragerc
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       89 2021-04-29 16:50:35.000000 masakari-9.1.2/.mailmap
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       53 2021-04-29 16:50:35.000000 masakari-9.1.2/.stestr.conf
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3624 2021-04-29 16:50:35.000000 masakari-9.1.2/.zuul.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2932 2021-04-29 16:51:14.000000 masakari-9.1.2/AUTHORS
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      654 2021-04-29 16:50:35.000000 masakari-9.1.2/CONTRIBUTING.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    12305 2021-04-29 16:51:13.000000 masakari-9.1.2/ChangeLog
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2415 2021-04-29 16:50:35.000000 masakari-9.1.2/HACKING.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10143 2021-04-29 16:50:35.000000 masakari-9.1.2/LICENSE
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-04-29 16:50:35.000000 masakari-9.1.2/MANIFEST.in
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4486 2021-04-29 16:51:14.273740 masakari-9.1.2/PKG-INFO
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2906 2021-04-29 16:50:35.000000 masakari-9.1.2/README.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-29 16:51:14.209740 masakari-9.1.2/api-ref/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-29 16:51:14.217740 masakari-9.1.2/api-ref/source/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7864 2021-04-29 16:50:35.000000 masakari-9.1.2/api-ref/source/conf.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7439 2021-04-29 16:50:35.000000 masakari-9.1.2/api-ref/source/failover-segments.inc
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7047 2021-04-29 16:50:35.000000 masakari-9.1.2/api-ref/source/hosts.inc
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      291 2021-04-29 16:50:35.000000 masakari-9.1.2/api-ref/source/index.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5425 2021-04-29 16:50:35.000000 masakari-9.1.2/api-ref/source/notifications.inc
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10493 2021-04-29 16:50:35.000000 masakari-9.1.2/api-ref/source/parameters.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1791 2021-04-29 16:50:35.000000 masakari-9.1.2/api-ref/source/status.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2191 2021-04-29 16:50:35.000000 masakari-9.1.2/api-ref/source/versions.inc
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       17 2021-04-29 16:50:35.000000 masakari-9.1.2/babel.cfg
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      288 2021-04-29 16:50:35.000000 masakari-9.1.2/bindep.txt
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-29 16:51:14.217740 masakari-9.1.2/devstack/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      886 2021-04-29 16:50:35.000000 masakari-9.1.2/devstack/README.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    15009 2021-04-29 16:50:35.000000 masakari-9.1.2/devstack/plugin.sh
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2500 2021-04-29 16:50:35.000000 masakari-9.1.2/devstack/settings
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-29 16:51:14.217740 masakari-9.1.2/doc/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-29 16:51:14.209740 masakari-9.1.2/doc/api_samples/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-29 16:51:14.217740 masakari-9.1.2/doc/api_samples/hosts/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      127 2021-04-29 16:50:35.000000 masakari-9.1.2/doc/api_samples/hosts/host-create-req.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      883 2021-04-29 16:50:35.000000 masakari-9.1.2/doc/api_samples/hosts/host-create-resp.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      883 2021-04-29 16:50:35.000000 masakari-9.1.2/doc/api_samples/hosts/host-get-resp.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       51 2021-04-29 16:50:35.000000 masakari-9.1.2/doc/api_samples/hosts/host-update-req.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      905 2021-04-29 16:50:35.000000 masakari-9.1.2/doc/api_samples/hosts/host-update-resp.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1000 2021-04-29 16:50:35.000000 masakari-9.1.2/doc/api_samples/hosts/hosts-list-resp.json
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-29 16:51:14.221740 masakari-9.1.2/doc/api_samples/notifications/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      298 2021-04-29 16:50:35.000000 masakari-9.1.2/doc/api_samples/notifications/host-notification-create-req.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      574 2021-04-29 16:50:35.000000 masakari-9.1.2/doc/api_samples/notifications/host-notification-create-resp.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      611 2021-04-29 16:50:35.000000 masakari-9.1.2/doc/api_samples/notifications/notifcations-list-resp.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2257 2021-04-29 16:50:35.000000 masakari-9.1.2/doc/api_samples/notifications/notification-get-resp.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      258 2021-04-29 16:50:35.000000 masakari-9.1.2/doc/api_samples/notifications/process-notification-create-req.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      534 2021-04-29 16:50:35.000000 masakari-9.1.2/doc/api_samples/notifications/process-notification-create-resp.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      340 2021-04-29 16:50:35.000000 masakari-9.1.2/doc/api_samples/notifications/vm-notification-create-req.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      609 2021-04-29 16:50:35.000000 masakari-9.1.2/doc/api_samples/notifications/vm-notification-create-resp.json
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-29 16:51:14.221740 masakari-9.1.2/doc/api_samples/segments/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      127 2021-04-29 16:50:35.000000 masakari-9.1.2/doc/api_samples/segments/segment-create-req.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      363 2021-04-29 16:50:35.000000 masakari-9.1.2/doc/api_samples/segments/segment-create-resp.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      363 2021-04-29 16:50:35.000000 masakari-9.1.2/doc/api_samples/segments/segment-get-resp.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       57 2021-04-29 16:50:35.000000 masakari-9.1.2/doc/api_samples/segments/segment-update-req.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      387 2021-04-29 16:50:35.000000 masakari-9.1.2/doc/api_samples/segments/segment-update-resp.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      426 2021-04-29 16:50:35.000000 masakari-9.1.2/doc/api_samples/segments/segments-list-resp.json
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-29 16:51:14.221740 masakari-9.1.2/doc/api_samples/versions/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      662 2021-04-29 16:50:35.000000 masakari-9.1.2/doc/api_samples/versions/v1-version-get-resp.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      388 2021-04-29 16:50:35.000000 masakari-9.1.2/doc/api_samples/versions/versions-get-resp.json
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-29 16:51:14.221740 masakari-9.1.2/doc/ext/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-04-29 16:50:35.000000 masakari-9.1.2/doc/ext/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5430 2021-04-29 16:50:35.000000 masakari-9.1.2/doc/ext/versioned_notifications.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-29 16:51:14.225740 masakari-9.1.2/doc/notification_samples/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1498 2021-04-29 16:50:35.000000 masakari-9.1.2/doc/notification_samples/create-host-end.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      700 2021-04-29 16:50:35.000000 masakari-9.1.2/doc/notification_samples/create-host-start.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      797 2021-04-29 16:50:35.000000 masakari-9.1.2/doc/notification_samples/create-notification-end.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      705 2021-04-29 16:50:35.000000 masakari-9.1.2/doc/notification_samples/create-notification-start.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      677 2021-04-29 16:50:35.000000 masakari-9.1.2/doc/notification_samples/create-segment-end.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      574 2021-04-29 16:50:35.000000 masakari-9.1.2/doc/notification_samples/create-segment-start.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1496 2021-04-29 16:50:35.000000 masakari-9.1.2/doc/notification_samples/delete-host-end.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1520 2021-04-29 16:50:35.000000 masakari-9.1.2/doc/notification_samples/delete-host-start.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      655 2021-04-29 16:50:35.000000 masakari-9.1.2/doc/notification_samples/delete-segment-end.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      680 2021-04-29 16:50:35.000000 masakari-9.1.2/doc/notification_samples/delete-segment-start.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1251 2021-04-29 16:50:35.000000 masakari-9.1.2/doc/notification_samples/error-exception.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      806 2021-04-29 16:50:35.000000 masakari-9.1.2/doc/notification_samples/process-notification-end.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1460 2021-04-29 16:50:35.000000 masakari-9.1.2/doc/notification_samples/process-notification-error.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      809 2021-04-29 16:50:35.000000 masakari-9.1.2/doc/notification_samples/process-notification-start.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1518 2021-04-29 16:50:35.000000 masakari-9.1.2/doc/notification_samples/update-host-end.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1500 2021-04-29 16:50:35.000000 masakari-9.1.2/doc/notification_samples/update-host-start.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      678 2021-04-29 16:50:35.000000 masakari-9.1.2/doc/notification_samples/update-segment-end.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      679 2021-04-29 16:50:35.000000 masakari-9.1.2/doc/notification_samples/update-segment-start.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      490 2021-04-29 16:50:35.000000 masakari-9.1.2/doc/requirements.txt
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-29 16:51:14.225740 masakari-9.1.2/doc/source/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-29 16:51:14.225740 masakari-9.1.2/doc/source/_static/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    46429 2021-04-29 16:50:35.000000 masakari-9.1.2/doc/source/_static/Masakari_spec_process.svg
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    55916 2021-04-29 16:50:35.000000 masakari-9.1.2/doc/source/_static/architecture.png
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-29 16:51:14.225740 masakari-9.1.2/doc/source/cli/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      255 2021-04-29 16:50:35.000000 masakari-9.1.2/doc/source/cli/index.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1178 2021-04-29 16:50:35.000000 masakari-9.1.2/doc/source/cli/masakari-manage.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1982 2021-04-29 16:50:35.000000 masakari-9.1.2/doc/source/cli/masakari-status.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      235 2021-04-29 16:50:35.000000 masakari-9.1.2/doc/source/cli/openstack-masakari.rst
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)     3195 2021-04-29 16:50:35.000000 masakari-9.1.2/doc/source/conf.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-29 16:51:14.225740 masakari-9.1.2/doc/source/configuration/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      188 2021-04-29 16:50:35.000000 masakari-9.1.2/doc/source/configuration/api-paste.ini.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      292 2021-04-29 16:50:35.000000 masakari-9.1.2/doc/source/configuration/config.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1223 2021-04-29 16:50:35.000000 masakari-9.1.2/doc/source/configuration/index.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      266 2021-04-29 16:50:35.000000 masakari-9.1.2/doc/source/configuration/policy.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      335 2021-04-29 16:50:35.000000 masakari-9.1.2/doc/source/configuration/recovery_config.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2506 2021-04-29 16:50:35.000000 masakari-9.1.2/doc/source/configuration/recovery_workflow_custom_task.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      519 2021-04-29 16:50:35.000000 masakari-9.1.2/doc/source/configuration/recovery_workflow_sample_config.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1793 2021-04-29 16:50:35.000000 masakari-9.1.2/doc/source/configuration/sample_config.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      429 2021-04-29 16:50:35.000000 masakari-9.1.2/doc/source/configuration/sample_policy.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3311 2021-04-29 16:50:35.000000 masakari-9.1.2/doc/source/index.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-29 16:51:14.229740 masakari-9.1.2/doc/source/install/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2914 2021-04-29 16:50:35.000000 masakari-9.1.2/doc/source/install/development.environment.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      116 2021-04-29 16:50:35.000000 masakari-9.1.2/doc/source/install/index.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1088 2021-04-29 16:50:35.000000 masakari-9.1.2/doc/source/install/install_and_configure.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9806 2021-04-29 16:50:35.000000 masakari-9.1.2/doc/source/install/install_and_configure_ubuntu.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1165 2021-04-29 16:50:35.000000 masakari-9.1.2/doc/source/install/overview.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4766 2021-04-29 16:50:35.000000 masakari-9.1.2/doc/source/install/verify.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-29 16:51:14.229740 masakari-9.1.2/doc/source/user/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1756 2021-04-29 16:50:35.000000 masakari-9.1.2/doc/source/user/architecture.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    12221 2021-04-29 16:50:35.000000 masakari-9.1.2/doc/source/user/how_to_get_involved.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5384 2021-04-29 16:50:35.000000 masakari-9.1.2/doc/source/user/notifications.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7315 2021-04-29 16:50:35.000000 masakari-9.1.2/doc/source/user/process.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-29 16:51:14.209740 masakari-9.1.2/etc/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-29 16:51:14.229740 masakari-9.1.2/etc/masakari/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      136 2021-04-29 16:50:35.000000 masakari-9.1.2/etc/masakari/README-masakari.conf.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1422 2021-04-29 16:50:35.000000 masakari-9.1.2/etc/masakari/api-paste.ini
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      391 2021-04-29 16:50:35.000000 masakari-9.1.2/etc/masakari/masakari-config-generator.conf
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3583 2021-04-29 16:50:35.000000 masakari-9.1.2/etc/masakari/masakari-custom-recovery-methods.conf
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      139 2021-04-29 16:50:35.000000 masakari-9.1.2/etc/masakari/masakari-customized-recovery-flow-config-generator.conf
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       77 2021-04-29 16:50:35.000000 masakari-9.1.2/etc/masakari/masakari-policy-generator.conf
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      650 2021-04-29 16:50:35.000000 masakari-9.1.2/etc/masakari/masakari.conf
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-29 16:51:14.233740 masakari-9.1.2/masakari/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1098 2021-04-29 16:50:35.000000 masakari-9.1.2/masakari/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-29 16:51:14.233740 masakari-9.1.2/masakari/api/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-04-29 16:50:35.000000 masakari-9.1.2/masakari/api/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6576 2021-04-29 16:50:35.000000 masakari-9.1.2/masakari/api/api_version_request.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6042 2021-04-29 16:50:35.000000 masakari-9.1.2/masakari/api/auth.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-29 16:51:14.233740 masakari-9.1.2/masakari/api/openstack/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10180 2021-04-29 16:50:35.000000 masakari-9.1.2/masakari/api/openstack/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9311 2021-04-29 16:50:35.000000 masakari-9.1.2/masakari/api/openstack/common.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    13528 2021-04-29 16:50:35.000000 masakari-9.1.2/masakari/api/openstack/extensions.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-29 16:51:14.237740 masakari-9.1.2/masakari/api/openstack/ha/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1341 2021-04-29 16:50:35.000000 masakari-9.1.2/masakari/api/openstack/ha/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4390 2021-04-29 16:50:35.000000 masakari-9.1.2/masakari/api/openstack/ha/extension_info.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7552 2021-04-29 16:50:35.000000 masakari-9.1.2/masakari/api/openstack/ha/hosts.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6257 2021-04-29 16:50:35.000000 masakari-9.1.2/masakari/api/openstack/ha/notifications.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-29 16:51:14.237740 masakari-9.1.2/masakari/api/openstack/ha/schemas/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-04-29 16:50:35.000000 masakari-9.1.2/masakari/api/openstack/ha/schemas/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1811 2021-04-29 16:50:35.000000 masakari-9.1.2/masakari/api/openstack/ha/schemas/hosts.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1451 2021-04-29 16:50:35.000000 masakari-9.1.2/masakari/api/openstack/ha/schemas/notifications.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1965 2021-04-29 16:50:35.000000 masakari-9.1.2/masakari/api/openstack/ha/schemas/payload.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1875 2021-04-29 16:50:35.000000 masakari-9.1.2/masakari/api/openstack/ha/schemas/segments.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5494 2021-04-29 16:50:35.000000 masakari-9.1.2/masakari/api/openstack/ha/segments.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2338 2021-04-29 16:50:35.000000 masakari-9.1.2/masakari/api/openstack/ha/versions.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2041 2021-04-29 16:50:35.000000 masakari-9.1.2/masakari/api/openstack/ha/versionsV1.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-29 16:51:14.237740 masakari-9.1.2/masakari/api/openstack/ha/views/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-04-29 16:50:35.000000 masakari-9.1.2/masakari/api/openstack/ha/views/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3167 2021-04-29 16:50:35.000000 masakari-9.1.2/masakari/api/openstack/ha/views/versions.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    38792 2021-04-29 16:50:35.000000 masakari-9.1.2/masakari/api/openstack/wsgi.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10294 2021-04-29 16:50:35.000000 masakari-9.1.2/masakari/api/urlmap.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4498 2021-04-29 16:50:35.000000 masakari-9.1.2/masakari/api/utils.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-29 16:51:14.237740 masakari-9.1.2/masakari/api/validation/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1974 2021-04-29 16:50:35.000000 masakari-9.1.2/masakari/api/validation/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5286 2021-04-29 16:50:35.000000 masakari-9.1.2/masakari/api/validation/parameter_types.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8109 2021-04-29 16:50:35.000000 masakari-9.1.2/masakari/api/validation/validators.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1252 2021-04-29 16:50:35.000000 masakari-9.1.2/masakari/api/versioned_method.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-29 16:51:14.237740 masakari-9.1.2/masakari/cmd/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      991 2021-04-29 16:50:35.000000 masakari-9.1.2/masakari/cmd/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2767 2021-04-29 16:50:35.000000 masakari-9.1.2/masakari/cmd/api.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1182 2021-04-29 16:50:35.000000 masakari-9.1.2/masakari/cmd/engine.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6671 2021-04-29 16:50:35.000000 masakari-9.1.2/masakari/cmd/manage.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1537 2021-04-29 16:50:35.000000 masakari-9.1.2/masakari/cmd/status.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-29 16:51:14.237740 masakari-9.1.2/masakari/common/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-04-29 16:50:35.000000 masakari-9.1.2/masakari/common/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1642 2021-04-29 16:50:35.000000 masakari-9.1.2/masakari/common/config.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-29 16:51:14.237740 masakari-9.1.2/masakari/compute/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      753 2021-04-29 16:50:35.000000 masakari-9.1.2/masakari/compute/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9889 2021-04-29 16:50:35.000000 masakari-9.1.2/masakari/compute/nova.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-29 16:51:14.241740 masakari-9.1.2/masakari/conf/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1397 2021-04-29 16:50:35.000000 masakari-9.1.2/masakari/conf/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2597 2021-04-29 16:50:35.000000 masakari-9.1.2/masakari/conf/api.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1500 2021-04-29 16:50:35.000000 masakari-9.1.2/masakari/conf/base.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      939 2021-04-29 16:50:35.000000 masakari-9.1.2/masakari/conf/database.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4625 2021-04-29 16:50:35.000000 masakari-9.1.2/masakari/conf/engine.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9167 2021-04-29 16:50:35.000000 masakari-9.1.2/masakari/conf/engine_driver.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      940 2021-04-29 16:50:35.000000 masakari-9.1.2/masakari/conf/exceptions.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2736 2021-04-29 16:50:35.000000 masakari-9.1.2/masakari/conf/nova.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3344 2021-04-29 16:50:35.000000 masakari-9.1.2/masakari/conf/opts.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3064 2021-04-29 16:50:35.000000 masakari-9.1.2/masakari/conf/osapi_v1.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1741 2021-04-29 16:50:35.000000 masakari-9.1.2/masakari/conf/paths.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2725 2021-04-29 16:50:35.000000 masakari-9.1.2/masakari/conf/service.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      769 2021-04-29 16:50:35.000000 masakari-9.1.2/masakari/conf/ssl.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4103 2021-04-29 16:50:35.000000 masakari-9.1.2/masakari/conf/wsgi.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1481 2021-04-29 16:50:35.000000 masakari-9.1.2/masakari/config.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9579 2021-04-29 16:50:35.000000 masakari-9.1.2/masakari/context.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-29 16:51:14.241740 masakari-9.1.2/masakari/db/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      699 2021-04-29 16:50:35.000000 masakari-9.1.2/masakari/db/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    13109 2021-04-29 16:50:35.000000 masakari-9.1.2/masakari/db/api.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      876 2021-04-29 16:50:35.000000 masakari-9.1.2/masakari/db/migration.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-29 16:51:14.241740 masakari-9.1.2/masakari/db/sqlalchemy/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-04-29 16:50:35.000000 masakari-9.1.2/masakari/db/sqlalchemy/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    23995 2021-04-29 16:50:35.000000 masakari-9.1.2/masakari/db/sqlalchemy/api.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-29 16:51:14.241740 masakari-9.1.2/masakari/db/sqlalchemy/migrate_repo/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      110 2021-04-29 16:50:35.000000 masakari-9.1.2/masakari/db/sqlalchemy/migrate_repo/README.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-04-29 16:50:35.000000 masakari-9.1.2/masakari/db/sqlalchemy/migrate_repo/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      857 2021-04-29 16:50:35.000000 masakari-9.1.2/masakari/db/sqlalchemy/migrate_repo/manage.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      983 2021-04-29 16:50:35.000000 masakari-9.1.2/masakari/db/sqlalchemy/migrate_repo/migrate.cfg
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-29 16:51:14.245740 masakari-9.1.2/masakari/db/sqlalchemy/migrate_repo/versions/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2805 2021-04-29 16:50:35.000000 masakari-9.1.2/masakari/db/sqlalchemy/migrate_repo/versions/001_add_failover_segments_table.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2499 2021-04-29 16:50:35.000000 masakari-9.1.2/masakari/db/sqlalchemy/migrate_repo/versions/002_add_hosts_table.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1940 2021-04-29 16:50:35.000000 masakari-9.1.2/masakari/db/sqlalchemy/migrate_repo/versions/003_update_unique_constraint_hosts.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2433 2021-04-29 16:50:35.000000 masakari-9.1.2/masakari/db/sqlalchemy/migrate_repo/versions/004_add_notifications_table.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      951 2021-04-29 16:50:35.000000 masakari-9.1.2/masakari/db/sqlalchemy/migrate_repo/versions/005_remove_nullable_mismatch.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1182 2021-04-29 16:50:35.000000 masakari-9.1.2/masakari/db/sqlalchemy/migrate_repo/versions/006_add_persistence_tables.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2450 2021-04-29 16:50:35.000000 masakari-9.1.2/masakari/db/sqlalchemy/migration.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6115 2021-04-29 16:50:35.000000 masakari-9.1.2/masakari/db/sqlalchemy/models.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-29 16:51:14.245740 masakari-9.1.2/masakari/engine/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-04-29 16:50:35.000000 masakari-9.1.2/masakari/engine/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2965 2021-04-29 16:50:35.000000 masakari-9.1.2/masakari/engine/driver.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-29 16:51:14.245740 masakari-9.1.2/masakari/engine/drivers/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      680 2021-04-29 16:50:35.000000 masakari-9.1.2/masakari/engine/drivers/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-29 16:51:14.245740 masakari-9.1.2/masakari/engine/drivers/taskflow/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      716 2021-04-29 16:50:35.000000 masakari-9.1.2/masakari/engine/drivers/taskflow/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5279 2021-04-29 16:50:35.000000 masakari-9.1.2/masakari/engine/drivers/taskflow/base.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    15189 2021-04-29 16:50:35.000000 masakari-9.1.2/masakari/engine/drivers/taskflow/driver.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    20923 2021-04-29 16:50:35.000000 masakari-9.1.2/masakari/engine/drivers/taskflow/host_failure.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8616 2021-04-29 16:50:35.000000 masakari-9.1.2/masakari/engine/drivers/taskflow/instance_failure.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1015 2021-04-29 16:50:35.000000 masakari-9.1.2/masakari/engine/drivers/taskflow/no_op.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5373 2021-04-29 16:50:35.000000 masakari-9.1.2/masakari/engine/drivers/taskflow/process_failure.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1228 2021-04-29 16:50:35.000000 masakari-9.1.2/masakari/engine/instance_events.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    18776 2021-04-29 16:50:35.000000 masakari-9.1.2/masakari/engine/manager.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2077 2021-04-29 16:50:35.000000 masakari-9.1.2/masakari/engine/rpcapi.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2352 2021-04-29 16:50:35.000000 masakari-9.1.2/masakari/engine/utils.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    11511 2021-04-29 16:50:35.000000 masakari-9.1.2/masakari/exception.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-29 16:51:14.245740 masakari-9.1.2/masakari/ha/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-04-29 16:50:35.000000 masakari-9.1.2/masakari/ha/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    15855 2021-04-29 16:50:35.000000 masakari-9.1.2/masakari/ha/api.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-29 16:51:14.245740 masakari-9.1.2/masakari/hacking/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-04-29 16:50:35.000000 masakari-9.1.2/masakari/hacking/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    16659 2021-04-29 16:50:35.000000 masakari-9.1.2/masakari/hacking/checks.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1041 2021-04-29 16:50:35.000000 masakari-9.1.2/masakari/i18n.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3546 2021-04-29 16:50:35.000000 masakari-9.1.2/masakari/manager.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-29 16:51:14.245740 masakari-9.1.2/masakari/notifications/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-04-29 16:50:35.000000 masakari-9.1.2/masakari/notifications/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-29 16:51:14.249740 masakari-9.1.2/masakari/notifications/objects/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-04-29 16:50:35.000000 masakari-9.1.2/masakari/notifications/objects/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6378 2021-04-29 16:50:35.000000 masakari-9.1.2/masakari/notifications/objects/base.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2544 2021-04-29 16:50:35.000000 masakari-9.1.2/masakari/notifications/objects/exception.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7005 2021-04-29 16:50:35.000000 masakari-9.1.2/masakari/notifications/objects/notification.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-29 16:51:14.249740 masakari-9.1.2/masakari/objects/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      958 2021-04-29 16:50:35.000000 masakari-9.1.2/masakari/objects/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10468 2021-04-29 16:50:35.000000 masakari-9.1.2/masakari/objects/base.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7454 2021-04-29 16:50:35.000000 masakari-9.1.2/masakari/objects/fields.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6284 2021-04-29 16:50:35.000000 masakari-9.1.2/masakari/objects/host.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7279 2021-04-29 16:50:35.000000 masakari-9.1.2/masakari/objects/notification.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5881 2021-04-29 16:50:35.000000 masakari-9.1.2/masakari/objects/segment.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-29 16:51:14.249740 masakari-9.1.2/masakari/policies/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1128 2021-04-29 16:50:35.000000 masakari-9.1.2/masakari/policies/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1259 2021-04-29 16:50:35.000000 masakari-9.1.2/masakari/policies/base.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1586 2021-04-29 16:50:35.000000 masakari-9.1.2/masakari/policies/extension_info.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2609 2021-04-29 16:50:35.000000 masakari-9.1.2/masakari/policies/hosts.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1997 2021-04-29 16:50:35.000000 masakari-9.1.2/masakari/policies/notifications.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2532 2021-04-29 16:50:35.000000 masakari-9.1.2/masakari/policies/segments.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1226 2021-04-29 16:50:35.000000 masakari-9.1.2/masakari/policies/versions.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7641 2021-04-29 16:50:35.000000 masakari-9.1.2/masakari/policy.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4955 2021-04-29 16:50:35.000000 masakari-9.1.2/masakari/rpc.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1396 2021-04-29 16:50:35.000000 masakari-9.1.2/masakari/safe_utils.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9696 2021-04-29 16:50:35.000000 masakari-9.1.2/masakari/service.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7322 2021-04-29 16:50:35.000000 masakari-9.1.2/masakari/test.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-29 16:51:14.249740 masakari-9.1.2/masakari/tests/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-04-29 16:50:35.000000 masakari-9.1.2/masakari/tests/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      719 2021-04-29 16:50:35.000000 masakari-9.1.2/masakari/tests/base.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4934 2021-04-29 16:50:35.000000 masakari-9.1.2/masakari/tests/fixtures.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-29 16:51:14.253740 masakari-9.1.2/masakari/tests/functional/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-04-29 16:50:35.000000 masakari-9.1.2/masakari/tests/functional/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2456 2021-04-29 16:50:35.000000 masakari-9.1.2/masakari/tests/functional/base.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4195 2021-04-29 16:50:35.000000 masakari-9.1.2/masakari/tests/functional/notification_base.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6822 2021-04-29 16:50:35.000000 masakari-9.1.2/masakari/tests/functional/test_hosts.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5009 2021-04-29 16:50:35.000000 masakari-9.1.2/masakari/tests/functional/test_process_notifications.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6413 2021-04-29 16:50:35.000000 masakari-9.1.2/masakari/tests/functional/test_segments.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3138 2021-04-29 16:50:35.000000 masakari-9.1.2/masakari/tests/functional/test_vm_notifications.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2397 2021-04-29 16:50:35.000000 masakari-9.1.2/masakari/tests/json_ref.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-29 16:51:14.257740 masakari-9.1.2/masakari/tests/unit/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      841 2021-04-29 16:50:35.000000 masakari-9.1.2/masakari/tests/unit/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-29 16:51:14.257740 masakari-9.1.2/masakari/tests/unit/api/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-04-29 16:50:35.000000 masakari-9.1.2/masakari/tests/unit/api/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-29 16:51:14.257740 masakari-9.1.2/masakari/tests/unit/api/openstack/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-04-29 16:50:35.000000 masakari-9.1.2/masakari/tests/unit/api/openstack/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4148 2021-04-29 16:50:35.000000 masakari-9.1.2/masakari/tests/unit/api/openstack/fakes.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-29 16:51:14.257740 masakari-9.1.2/masakari/tests/unit/api/openstack/ha/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-04-29 16:50:35.000000 masakari-9.1.2/masakari/tests/unit/api/openstack/ha/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4027 2021-04-29 16:50:35.000000 masakari-9.1.2/masakari/tests/unit/api/openstack/ha/test_extension_info.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    22396 2021-04-29 16:50:35.000000 masakari-9.1.2/masakari/tests/unit/api/openstack/ha/test_hosts.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    21557 2021-04-29 16:50:35.000000 masakari-9.1.2/masakari/tests/unit/api/openstack/ha/test_notifications.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    15281 2021-04-29 16:50:35.000000 masakari-9.1.2/masakari/tests/unit/api/openstack/ha/test_segments.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8269 2021-04-29 16:50:35.000000 masakari-9.1.2/masakari/tests/unit/api/openstack/ha/test_versions.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    14458 2021-04-29 16:50:35.000000 masakari-9.1.2/masakari/tests/unit/api/openstack/test_common.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3347 2021-04-29 16:50:35.000000 masakari-9.1.2/masakari/tests/unit/api/openstack/test_extensions.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    38013 2021-04-29 16:50:35.000000 masakari-9.1.2/masakari/tests/unit/api/openstack/test_wsgi.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3802 2021-04-29 16:50:35.000000 masakari-9.1.2/masakari/tests/unit/api/test_api_version_request.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7838 2021-04-29 16:50:35.000000 masakari-9.1.2/masakari/tests/unit/api/test_auth.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7693 2021-04-29 16:50:35.000000 masakari-9.1.2/masakari/tests/unit/api/test_utils.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-29 16:51:14.257740 masakari-9.1.2/masakari/tests/unit/cmd/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-04-29 16:50:35.000000 masakari-9.1.2/masakari/tests/unit/cmd/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2085 2021-04-29 16:50:35.000000 masakari-9.1.2/masakari/tests/unit/cmd/test_masakari_api.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1014 2021-04-29 16:50:35.000000 masakari-9.1.2/masakari/tests/unit/cmd/test_status.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-29 16:51:14.257740 masakari-9.1.2/masakari/tests/unit/compute/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-04-29 16:50:35.000000 masakari-9.1.2/masakari/tests/unit/compute/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    15540 2021-04-29 16:50:35.000000 masakari-9.1.2/masakari/tests/unit/compute/test_nova.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1556 2021-04-29 16:50:35.000000 masakari-9.1.2/masakari/tests/unit/conf_fixture.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-29 16:51:14.261740 masakari-9.1.2/masakari/tests/unit/db/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-04-29 16:50:35.000000 masakari-9.1.2/masakari/tests/unit/db/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    22215 2021-04-29 16:50:35.000000 masakari-9.1.2/masakari/tests/unit/db/test_db_api.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10513 2021-04-29 16:50:35.000000 masakari-9.1.2/masakari/tests/unit/db/test_migrations.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6824 2021-04-29 16:50:35.000000 masakari-9.1.2/masakari/tests/unit/db/test_purge.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-29 16:51:14.261740 masakari-9.1.2/masakari/tests/unit/engine/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-04-29 16:50:35.000000 masakari-9.1.2/masakari/tests/unit/engine/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-29 16:51:14.261740 masakari-9.1.2/masakari/tests/unit/engine/drivers/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-04-29 16:50:35.000000 masakari-9.1.2/masakari/tests/unit/engine/drivers/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-29 16:51:14.261740 masakari-9.1.2/masakari/tests/unit/engine/drivers/taskflow/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-04-29 16:50:35.000000 masakari-9.1.2/masakari/tests/unit/engine/drivers/taskflow/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    37972 2021-04-29 16:50:35.000000 masakari-9.1.2/masakari/tests/unit/engine/drivers/taskflow/test_host_failure_flow.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    12277 2021-04-29 16:50:35.000000 masakari-9.1.2/masakari/tests/unit/engine/drivers/taskflow/test_instance_failure_flow.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6436 2021-04-29 16:50:35.000000 masakari-9.1.2/masakari/tests/unit/engine/drivers/taskflow/test_process_failure_flow.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    18931 2021-04-29 16:50:35.000000 masakari-9.1.2/masakari/tests/unit/engine/drivers/taskflow/test_taskflow_driver.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1881 2021-04-29 16:50:35.000000 masakari-9.1.2/masakari/tests/unit/engine/fake_engine.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    58476 2021-04-29 16:50:35.000000 masakari-9.1.2/masakari/tests/unit/engine/test_engine_mgr.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3769 2021-04-29 16:50:35.000000 masakari-9.1.2/masakari/tests/unit/engine/test_rpcapi.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3341 2021-04-29 16:50:35.000000 masakari-9.1.2/masakari/tests/unit/engine/test_utils.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2853 2021-04-29 16:50:35.000000 masakari-9.1.2/masakari/tests/unit/fake_notifier.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1325 2021-04-29 16:50:35.000000 masakari-9.1.2/masakari/tests/unit/fake_policy.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7855 2021-04-29 16:50:35.000000 masakari-9.1.2/masakari/tests/unit/fakes.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-29 16:51:14.261740 masakari-9.1.2/masakari/tests/unit/ha/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-04-29 16:50:35.000000 masakari-9.1.2/masakari/tests/unit/ha/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    45120 2021-04-29 16:50:35.000000 masakari-9.1.2/masakari/tests/unit/ha/test_api.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1744 2021-04-29 16:50:35.000000 masakari-9.1.2/masakari/tests/unit/matchers.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-29 16:51:14.261740 masakari-9.1.2/masakari/tests/unit/monkey_patch_example/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1099 2021-04-29 16:50:35.000000 masakari-9.1.2/masakari/tests/unit/monkey_patch_example/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      905 2021-04-29 16:50:35.000000 masakari-9.1.2/masakari/tests/unit/monkey_patch_example/example_a.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      906 2021-04-29 16:50:35.000000 masakari-9.1.2/masakari/tests/unit/monkey_patch_example/example_b.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-29 16:51:14.261740 masakari-9.1.2/masakari/tests/unit/notifications/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-04-29 16:50:35.000000 masakari-9.1.2/masakari/tests/unit/notifications/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-29 16:51:14.261740 masakari-9.1.2/masakari/tests/unit/notifications/objects/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-04-29 16:50:35.000000 masakari-9.1.2/masakari/tests/unit/notifications/objects/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10810 2021-04-29 16:50:35.000000 masakari-9.1.2/masakari/tests/unit/notifications/objects/test_notification.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-29 16:51:14.265740 masakari-9.1.2/masakari/tests/unit/objects/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-04-29 16:50:35.000000 masakari-9.1.2/masakari/tests/unit/objects/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2735 2021-04-29 16:50:35.000000 masakari-9.1.2/masakari/tests/unit/objects/fake_args.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8095 2021-04-29 16:50:35.000000 masakari-9.1.2/masakari/tests/unit/objects/test_fields.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    12394 2021-04-29 16:50:35.000000 masakari-9.1.2/masakari/tests/unit/objects/test_hosts.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    11272 2021-04-29 16:50:35.000000 masakari-9.1.2/masakari/tests/unit/objects/test_notifications.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    33197 2021-04-29 16:50:35.000000 masakari-9.1.2/masakari/tests/unit/objects/test_objects.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    12312 2021-04-29 16:50:35.000000 masakari-9.1.2/masakari/tests/unit/objects/test_segments.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3663 2021-04-29 16:50:35.000000 masakari-9.1.2/masakari/tests/unit/policy_fixture.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    21707 2021-04-29 16:50:35.000000 masakari-9.1.2/masakari/tests/unit/test_api_validation.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2940 2021-04-29 16:50:35.000000 masakari-9.1.2/masakari/tests/unit/test_conf.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6127 2021-04-29 16:50:35.000000 masakari-9.1.2/masakari/tests/unit/test_context.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5907 2021-04-29 16:50:35.000000 masakari-9.1.2/masakari/tests/unit/test_exception.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    20938 2021-04-29 16:50:35.000000 masakari-9.1.2/masakari/tests/unit/test_hacking.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3157 2021-04-29 16:50:35.000000 masakari-9.1.2/masakari/tests/unit/test_masakari_manage.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10359 2021-04-29 16:50:35.000000 masakari-9.1.2/masakari/tests/unit/test_policy.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10831 2021-04-29 16:50:35.000000 masakari-9.1.2/masakari/tests/unit/test_rpc.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2544 2021-04-29 16:50:35.000000 masakari-9.1.2/masakari/tests/unit/test_safeutils.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6569 2021-04-29 16:50:35.000000 masakari-9.1.2/masakari/tests/unit/test_service.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9193 2021-04-29 16:50:35.000000 masakari-9.1.2/masakari/tests/unit/test_utils.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2177 2021-04-29 16:50:35.000000 masakari-9.1.2/masakari/tests/unit/test_versions.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8203 2021-04-29 16:50:35.000000 masakari-9.1.2/masakari/tests/unit/test_wsgi.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2038 2021-04-29 16:50:35.000000 masakari-9.1.2/masakari/tests/unit/utils.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1091 2021-04-29 16:50:35.000000 masakari-9.1.2/masakari/tests/uuidsentinel.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9364 2021-04-29 16:50:35.000000 masakari-9.1.2/masakari/utils.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2395 2021-04-29 16:50:35.000000 masakari-9.1.2/masakari/version.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    16879 2021-04-29 16:50:35.000000 masakari-9.1.2/masakari/wsgi.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-29 16:51:14.233740 masakari-9.1.2/masakari.egg-info/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4486 2021-04-29 16:51:14.000000 masakari-9.1.2/masakari.egg-info/PKG-INFO
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    14139 2021-04-29 16:51:14.000000 masakari-9.1.2/masakari.egg-info/SOURCES.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2021-04-29 16:51:14.000000 masakari-9.1.2/masakari.egg-info/dependency_links.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2007 2021-04-29 16:51:14.000000 masakari-9.1.2/masakari.egg-info/entry_points.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2021-04-29 16:51:14.000000 masakari-9.1.2/masakari.egg-info/not-zip-safe
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       46 2021-04-29 16:51:14.000000 masakari-9.1.2/masakari.egg-info/pbr.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      540 2021-04-29 16:51:14.000000 masakari-9.1.2/masakari.egg-info/requires.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        9 2021-04-29 16:51:14.000000 masakari-9.1.2/masakari.egg-info/top_level.txt
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-29 16:51:14.213740 masakari-9.1.2/playbooks/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-29 16:51:14.265740 masakari-9.1.2/playbooks/devstack/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       71 2021-04-29 16:50:35.000000 masakari-9.1.2/playbooks/devstack/post.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      152 2021-04-29 16:50:35.000000 masakari-9.1.2/playbooks/devstack/pre.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       39 2021-04-29 16:50:35.000000 masakari-9.1.2/playbooks/devstack/run.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-29 16:51:14.213740 masakari-9.1.2/releasenotes/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-29 16:51:14.269740 masakari-9.1.2/releasenotes/notes/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-04-29 16:50:35.000000 masakari-9.1.2/releasenotes/notes/.placeholder
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      998 2021-04-29 16:50:35.000000 masakari-9.1.2/releasenotes/notes/add-periodic-tasks-0c96d6f620502a75.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      477 2021-04-29 16:50:35.000000 masakari-9.1.2/releasenotes/notes/add-upgrade-check-framework-52268130b25317ab.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      686 2021-04-29 16:50:35.000000 masakari-9.1.2/releasenotes/notes/add_evacuate_error_instances_conf_option-5b4d1906137395f0.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1477 2021-04-29 16:50:35.000000 masakari-9.1.2/releasenotes/notes/add_ha_enabled_config_options-54a9270a5993d20a.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      416 2021-04-29 16:50:35.000000 masakari-9.1.2/releasenotes/notes/add_reserved_host_to_aggregates-5f506d08354ec148.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      327 2021-04-29 16:50:35.000000 masakari-9.1.2/releasenotes/notes/adopt-oslo-config-generator-cf2fdb17cf7f13db.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      699 2021-04-29 16:50:35.000000 masakari-9.1.2/releasenotes/notes/auto_priority_and_rh_priority_recovery_methods-b88cc00041fa2c4d.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      250 2021-04-29 16:50:35.000000 masakari-9.1.2/releasenotes/notes/bp-mutable-config-57efdd467c01aa7b.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      176 2021-04-29 16:50:35.000000 masakari-9.1.2/releasenotes/notes/bug-1685145-3d93145bfc76c660.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      136 2021-04-29 16:50:35.000000 masakari-9.1.2/releasenotes/notes/bug-1776385-0bcf0a0b3fad359e.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      179 2021-04-29 16:50:35.000000 masakari-9.1.2/releasenotes/notes/bug-1782517-e4dc70bad9e4e131.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      174 2021-04-29 16:50:35.000000 masakari-9.1.2/releasenotes/notes/bug-1856164-6601a6e6280eba4d.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      175 2021-04-29 16:50:35.000000 masakari-9.1.2/releasenotes/notes/bug-1859406-6b041a26acf6c7f6.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      159 2021-04-29 16:50:35.000000 masakari-9.1.2/releasenotes/notes/bug-1882516-e8dc7fd2b55f065f.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      284 2021-04-29 16:50:35.000000 masakari-9.1.2/releasenotes/notes/bug-add-missing-domain-name-5181c02f3f033a22.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      304 2021-04-29 16:50:35.000000 masakari-9.1.2/releasenotes/notes/compute_search-3da97e69e661a73f.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      681 2021-04-29 16:50:35.000000 masakari-9.1.2/releasenotes/notes/correct_response_code-df8b43a201efa1b4.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      434 2021-04-29 16:50:35.000000 masakari-9.1.2/releasenotes/notes/db-purge-support-7a33e2ea5d2a624b.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      130 2021-04-29 16:50:35.000000 masakari-9.1.2/releasenotes/notes/deprecate-topic-opt-af83f82143143c61.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      206 2021-04-29 16:50:35.000000 masakari-9.1.2/releasenotes/notes/drop-py-2-7-059d3cd5e7cb4e1a.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      642 2021-04-29 16:50:35.000000 masakari-9.1.2/releasenotes/notes/evacuation_in_threads-cc9c79b10acfb5f6.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      444 2021-04-29 16:50:35.000000 masakari-9.1.2/releasenotes/notes/failover_segment_apis-f5bea1cd6d103048.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      219 2021-04-29 16:50:35.000000 masakari-9.1.2/releasenotes/notes/fix-endless-periodic-f223845f3044b166.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      625 2021-04-29 16:50:35.000000 masakari-9.1.2/releasenotes/notes/host-apis-46a87fcd56d8ed30.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      658 2021-04-29 16:50:35.000000 masakari-9.1.2/releasenotes/notes/notifications-in-masakari-f5d79838fc23cb9b.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      303 2021-04-29 16:50:35.000000 masakari-9.1.2/releasenotes/notes/notifications_apis-3c3d5055ae9c6649.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1148 2021-04-29 16:50:35.000000 masakari-9.1.2/releasenotes/notes/policy-in-code-8740d51624055044.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1235 2021-04-29 16:50:35.000000 masakari-9.1.2/releasenotes/notes/progress-details-recovery-workflows-5b14b7b3f87374f4.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      865 2021-04-29 16:50:35.000000 masakari-9.1.2/releasenotes/notes/recovery-method-customization-3438b0e26e322b88.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      392 2021-04-29 16:50:35.000000 masakari-9.1.2/releasenotes/notes/reserved_host_recovery_method-d2de1f205136c8d5.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      350 2021-04-29 16:50:35.000000 masakari-9.1.2/releasenotes/notes/wsgi-applications-3ed7d6b89f1a5785.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-29 16:51:14.269740 masakari-9.1.2/releasenotes/source/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-29 16:51:14.269740 masakari-9.1.2/releasenotes/source/_static/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-04-29 16:50:35.000000 masakari-9.1.2/releasenotes/source/_static/.placeholder
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-29 16:51:14.269740 masakari-9.1.2/releasenotes/source/_templates/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-04-29 16:50:35.000000 masakari-9.1.2/releasenotes/source/_templates/.placeholder
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8995 2021-04-29 16:50:35.000000 masakari-9.1.2/releasenotes/source/conf.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      217 2021-04-29 16:50:35.000000 masakari-9.1.2/releasenotes/source/index.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      137 2021-04-29 16:50:35.000000 masakari-9.1.2/releasenotes/source/ocata.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      133 2021-04-29 16:50:35.000000 masakari-9.1.2/releasenotes/source/pike.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      141 2021-04-29 16:50:35.000000 masakari-9.1.2/releasenotes/source/queens.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      145 2021-04-29 16:50:35.000000 masakari-9.1.2/releasenotes/source/rocky.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      145 2021-04-29 16:50:35.000000 masakari-9.1.2/releasenotes/source/stein.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      126 2021-04-29 16:50:35.000000 masakari-9.1.2/releasenotes/source/train.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      112 2021-04-29 16:50:35.000000 masakari-9.1.2/releasenotes/source/unreleased.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1047 2021-04-29 16:50:35.000000 masakari-9.1.2/requirements.txt
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-29 16:51:14.213740 masakari-9.1.2/roles/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-29 16:51:14.213740 masakari-9.1.2/roles/devstack-config/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-04-29 16:51:14.269740 masakari-9.1.2/roles/devstack-config/tasks/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      418 2021-04-29 16:50:35.000000 masakari-9.1.2/roles/devstack-config/tasks/main.yml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3159 2021-04-29 16:51:14.273740 masakari-9.1.2/setup.cfg
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1030 2021-04-29 16:50:35.000000 masakari-9.1.2/setup.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      693 2021-04-29 16:50:35.000000 masakari-9.1.2/test-requirements.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3503 2021-04-29 16:50:35.000000 masakari-9.1.2/tox.ini
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-08-19 12:40:25.240568 masakari-9.1.3/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       97 2021-08-19 12:39:51.000000 masakari-9.1.3/.coveragerc
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       89 2021-08-19 12:39:51.000000 masakari-9.1.3/.mailmap
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       53 2021-08-19 12:39:51.000000 masakari-9.1.3/.stestr.conf
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3624 2021-08-19 12:39:51.000000 masakari-9.1.3/.zuul.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2967 2021-08-19 12:40:24.000000 masakari-9.1.3/AUTHORS
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      654 2021-08-19 12:39:51.000000 masakari-9.1.3/CONTRIBUTING.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    12369 2021-08-19 12:40:24.000000 masakari-9.1.3/ChangeLog
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2415 2021-08-19 12:39:51.000000 masakari-9.1.3/HACKING.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10143 2021-08-19 12:39:51.000000 masakari-9.1.3/LICENSE
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-08-19 12:39:51.000000 masakari-9.1.3/MANIFEST.in
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4486 2021-08-19 12:40:25.240568 masakari-9.1.3/PKG-INFO
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2906 2021-08-19 12:39:51.000000 masakari-9.1.3/README.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-08-19 12:40:25.168567 masakari-9.1.3/api-ref/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-08-19 12:40:25.180567 masakari-9.1.3/api-ref/source/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7864 2021-08-19 12:39:51.000000 masakari-9.1.3/api-ref/source/conf.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7439 2021-08-19 12:39:51.000000 masakari-9.1.3/api-ref/source/failover-segments.inc
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7047 2021-08-19 12:39:51.000000 masakari-9.1.3/api-ref/source/hosts.inc
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      291 2021-08-19 12:39:51.000000 masakari-9.1.3/api-ref/source/index.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5425 2021-08-19 12:39:51.000000 masakari-9.1.3/api-ref/source/notifications.inc
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10493 2021-08-19 12:39:51.000000 masakari-9.1.3/api-ref/source/parameters.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1791 2021-08-19 12:39:51.000000 masakari-9.1.3/api-ref/source/status.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2191 2021-08-19 12:39:51.000000 masakari-9.1.3/api-ref/source/versions.inc
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       17 2021-08-19 12:39:51.000000 masakari-9.1.3/babel.cfg
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      288 2021-08-19 12:39:51.000000 masakari-9.1.3/bindep.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-08-19 12:40:25.180567 masakari-9.1.3/devstack/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      886 2021-08-19 12:39:51.000000 masakari-9.1.3/devstack/README.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    15009 2021-08-19 12:39:51.000000 masakari-9.1.3/devstack/plugin.sh
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2500 2021-08-19 12:39:51.000000 masakari-9.1.3/devstack/settings
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-08-19 12:40:25.180567 masakari-9.1.3/doc/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-08-19 12:40:25.172567 masakari-9.1.3/doc/api_samples/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-08-19 12:40:25.184567 masakari-9.1.3/doc/api_samples/hosts/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      127 2021-08-19 12:39:51.000000 masakari-9.1.3/doc/api_samples/hosts/host-create-req.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      883 2021-08-19 12:39:51.000000 masakari-9.1.3/doc/api_samples/hosts/host-create-resp.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      883 2021-08-19 12:39:51.000000 masakari-9.1.3/doc/api_samples/hosts/host-get-resp.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       51 2021-08-19 12:39:51.000000 masakari-9.1.3/doc/api_samples/hosts/host-update-req.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      905 2021-08-19 12:39:51.000000 masakari-9.1.3/doc/api_samples/hosts/host-update-resp.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1000 2021-08-19 12:39:51.000000 masakari-9.1.3/doc/api_samples/hosts/hosts-list-resp.json
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-08-19 12:40:25.184567 masakari-9.1.3/doc/api_samples/notifications/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      298 2021-08-19 12:39:51.000000 masakari-9.1.3/doc/api_samples/notifications/host-notification-create-req.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      574 2021-08-19 12:39:51.000000 masakari-9.1.3/doc/api_samples/notifications/host-notification-create-resp.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      611 2021-08-19 12:39:51.000000 masakari-9.1.3/doc/api_samples/notifications/notifcations-list-resp.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2257 2021-08-19 12:39:51.000000 masakari-9.1.3/doc/api_samples/notifications/notification-get-resp.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      258 2021-08-19 12:39:51.000000 masakari-9.1.3/doc/api_samples/notifications/process-notification-create-req.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      534 2021-08-19 12:39:51.000000 masakari-9.1.3/doc/api_samples/notifications/process-notification-create-resp.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      340 2021-08-19 12:39:51.000000 masakari-9.1.3/doc/api_samples/notifications/vm-notification-create-req.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      609 2021-08-19 12:39:51.000000 masakari-9.1.3/doc/api_samples/notifications/vm-notification-create-resp.json
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-08-19 12:40:25.184567 masakari-9.1.3/doc/api_samples/segments/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      127 2021-08-19 12:39:51.000000 masakari-9.1.3/doc/api_samples/segments/segment-create-req.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      363 2021-08-19 12:39:51.000000 masakari-9.1.3/doc/api_samples/segments/segment-create-resp.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      363 2021-08-19 12:39:51.000000 masakari-9.1.3/doc/api_samples/segments/segment-get-resp.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       57 2021-08-19 12:39:51.000000 masakari-9.1.3/doc/api_samples/segments/segment-update-req.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      387 2021-08-19 12:39:51.000000 masakari-9.1.3/doc/api_samples/segments/segment-update-resp.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      426 2021-08-19 12:39:51.000000 masakari-9.1.3/doc/api_samples/segments/segments-list-resp.json
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-08-19 12:40:25.184567 masakari-9.1.3/doc/api_samples/versions/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      662 2021-08-19 12:39:51.000000 masakari-9.1.3/doc/api_samples/versions/v1-version-get-resp.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      388 2021-08-19 12:39:51.000000 masakari-9.1.3/doc/api_samples/versions/versions-get-resp.json
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-08-19 12:40:25.184567 masakari-9.1.3/doc/ext/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-08-19 12:39:51.000000 masakari-9.1.3/doc/ext/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5430 2021-08-19 12:39:51.000000 masakari-9.1.3/doc/ext/versioned_notifications.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-08-19 12:40:25.188567 masakari-9.1.3/doc/notification_samples/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1498 2021-08-19 12:39:51.000000 masakari-9.1.3/doc/notification_samples/create-host-end.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      700 2021-08-19 12:39:51.000000 masakari-9.1.3/doc/notification_samples/create-host-start.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      797 2021-08-19 12:39:51.000000 masakari-9.1.3/doc/notification_samples/create-notification-end.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      705 2021-08-19 12:39:51.000000 masakari-9.1.3/doc/notification_samples/create-notification-start.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      677 2021-08-19 12:39:51.000000 masakari-9.1.3/doc/notification_samples/create-segment-end.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      574 2021-08-19 12:39:51.000000 masakari-9.1.3/doc/notification_samples/create-segment-start.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1496 2021-08-19 12:39:51.000000 masakari-9.1.3/doc/notification_samples/delete-host-end.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1520 2021-08-19 12:39:51.000000 masakari-9.1.3/doc/notification_samples/delete-host-start.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      655 2021-08-19 12:39:51.000000 masakari-9.1.3/doc/notification_samples/delete-segment-end.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      680 2021-08-19 12:39:51.000000 masakari-9.1.3/doc/notification_samples/delete-segment-start.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1251 2021-08-19 12:39:51.000000 masakari-9.1.3/doc/notification_samples/error-exception.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      806 2021-08-19 12:39:51.000000 masakari-9.1.3/doc/notification_samples/process-notification-end.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1460 2021-08-19 12:39:51.000000 masakari-9.1.3/doc/notification_samples/process-notification-error.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      809 2021-08-19 12:39:51.000000 masakari-9.1.3/doc/notification_samples/process-notification-start.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1518 2021-08-19 12:39:51.000000 masakari-9.1.3/doc/notification_samples/update-host-end.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1500 2021-08-19 12:39:51.000000 masakari-9.1.3/doc/notification_samples/update-host-start.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      678 2021-08-19 12:39:51.000000 masakari-9.1.3/doc/notification_samples/update-segment-end.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      679 2021-08-19 12:39:51.000000 masakari-9.1.3/doc/notification_samples/update-segment-start.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      490 2021-08-19 12:39:51.000000 masakari-9.1.3/doc/requirements.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-08-19 12:40:25.188567 masakari-9.1.3/doc/source/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-08-19 12:40:25.188567 masakari-9.1.3/doc/source/_static/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    46429 2021-08-19 12:39:51.000000 masakari-9.1.3/doc/source/_static/Masakari_spec_process.svg
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    55916 2021-08-19 12:39:51.000000 masakari-9.1.3/doc/source/_static/architecture.png
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-08-19 12:40:25.192567 masakari-9.1.3/doc/source/cli/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      255 2021-08-19 12:39:51.000000 masakari-9.1.3/doc/source/cli/index.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1178 2021-08-19 12:39:51.000000 masakari-9.1.3/doc/source/cli/masakari-manage.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1982 2021-08-19 12:39:51.000000 masakari-9.1.3/doc/source/cli/masakari-status.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      235 2021-08-19 12:39:51.000000 masakari-9.1.3/doc/source/cli/openstack-masakari.rst
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)     3195 2021-08-19 12:39:51.000000 masakari-9.1.3/doc/source/conf.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-08-19 12:40:25.192567 masakari-9.1.3/doc/source/configuration/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      188 2021-08-19 12:39:51.000000 masakari-9.1.3/doc/source/configuration/api-paste.ini.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      292 2021-08-19 12:39:51.000000 masakari-9.1.3/doc/source/configuration/config.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1223 2021-08-19 12:39:51.000000 masakari-9.1.3/doc/source/configuration/index.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      266 2021-08-19 12:39:51.000000 masakari-9.1.3/doc/source/configuration/policy.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      335 2021-08-19 12:39:51.000000 masakari-9.1.3/doc/source/configuration/recovery_config.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2506 2021-08-19 12:39:51.000000 masakari-9.1.3/doc/source/configuration/recovery_workflow_custom_task.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      519 2021-08-19 12:39:51.000000 masakari-9.1.3/doc/source/configuration/recovery_workflow_sample_config.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1793 2021-08-19 12:39:51.000000 masakari-9.1.3/doc/source/configuration/sample_config.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      429 2021-08-19 12:39:51.000000 masakari-9.1.3/doc/source/configuration/sample_policy.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3311 2021-08-19 12:39:51.000000 masakari-9.1.3/doc/source/index.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-08-19 12:40:25.192567 masakari-9.1.3/doc/source/install/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2914 2021-08-19 12:39:51.000000 masakari-9.1.3/doc/source/install/development.environment.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      116 2021-08-19 12:39:51.000000 masakari-9.1.3/doc/source/install/index.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1088 2021-08-19 12:39:51.000000 masakari-9.1.3/doc/source/install/install_and_configure.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9806 2021-08-19 12:39:51.000000 masakari-9.1.3/doc/source/install/install_and_configure_ubuntu.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1165 2021-08-19 12:39:51.000000 masakari-9.1.3/doc/source/install/overview.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4766 2021-08-19 12:39:51.000000 masakari-9.1.3/doc/source/install/verify.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-08-19 12:40:25.196567 masakari-9.1.3/doc/source/user/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1756 2021-08-19 12:39:51.000000 masakari-9.1.3/doc/source/user/architecture.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    12221 2021-08-19 12:39:51.000000 masakari-9.1.3/doc/source/user/how_to_get_involved.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5384 2021-08-19 12:39:51.000000 masakari-9.1.3/doc/source/user/notifications.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7315 2021-08-19 12:39:51.000000 masakari-9.1.3/doc/source/user/process.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-08-19 12:40:25.172567 masakari-9.1.3/etc/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-08-19 12:40:25.196567 masakari-9.1.3/etc/masakari/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      136 2021-08-19 12:39:51.000000 masakari-9.1.3/etc/masakari/README-masakari.conf.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1422 2021-08-19 12:39:51.000000 masakari-9.1.3/etc/masakari/api-paste.ini
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      391 2021-08-19 12:39:51.000000 masakari-9.1.3/etc/masakari/masakari-config-generator.conf
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3583 2021-08-19 12:39:51.000000 masakari-9.1.3/etc/masakari/masakari-custom-recovery-methods.conf
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      139 2021-08-19 12:39:51.000000 masakari-9.1.3/etc/masakari/masakari-customized-recovery-flow-config-generator.conf
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       77 2021-08-19 12:39:51.000000 masakari-9.1.3/etc/masakari/masakari-policy-generator.conf
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      650 2021-08-19 12:39:51.000000 masakari-9.1.3/etc/masakari/masakari.conf
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-08-19 12:40:25.196567 masakari-9.1.3/masakari/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1098 2021-08-19 12:39:51.000000 masakari-9.1.3/masakari/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-08-19 12:40:25.200567 masakari-9.1.3/masakari/api/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-08-19 12:39:51.000000 masakari-9.1.3/masakari/api/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6576 2021-08-19 12:39:51.000000 masakari-9.1.3/masakari/api/api_version_request.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6042 2021-08-19 12:39:51.000000 masakari-9.1.3/masakari/api/auth.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-08-19 12:40:25.200567 masakari-9.1.3/masakari/api/openstack/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10180 2021-08-19 12:39:51.000000 masakari-9.1.3/masakari/api/openstack/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9311 2021-08-19 12:39:51.000000 masakari-9.1.3/masakari/api/openstack/common.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    13528 2021-08-19 12:39:51.000000 masakari-9.1.3/masakari/api/openstack/extensions.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-08-19 12:40:25.204568 masakari-9.1.3/masakari/api/openstack/ha/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1341 2021-08-19 12:39:51.000000 masakari-9.1.3/masakari/api/openstack/ha/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4390 2021-08-19 12:39:51.000000 masakari-9.1.3/masakari/api/openstack/ha/extension_info.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7552 2021-08-19 12:39:51.000000 masakari-9.1.3/masakari/api/openstack/ha/hosts.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6257 2021-08-19 12:39:51.000000 masakari-9.1.3/masakari/api/openstack/ha/notifications.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-08-19 12:40:25.204568 masakari-9.1.3/masakari/api/openstack/ha/schemas/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-08-19 12:39:51.000000 masakari-9.1.3/masakari/api/openstack/ha/schemas/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1811 2021-08-19 12:39:51.000000 masakari-9.1.3/masakari/api/openstack/ha/schemas/hosts.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1451 2021-08-19 12:39:51.000000 masakari-9.1.3/masakari/api/openstack/ha/schemas/notifications.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1965 2021-08-19 12:39:51.000000 masakari-9.1.3/masakari/api/openstack/ha/schemas/payload.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1875 2021-08-19 12:39:51.000000 masakari-9.1.3/masakari/api/openstack/ha/schemas/segments.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5494 2021-08-19 12:39:51.000000 masakari-9.1.3/masakari/api/openstack/ha/segments.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2338 2021-08-19 12:39:51.000000 masakari-9.1.3/masakari/api/openstack/ha/versions.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2041 2021-08-19 12:39:51.000000 masakari-9.1.3/masakari/api/openstack/ha/versionsV1.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-08-19 12:40:25.204568 masakari-9.1.3/masakari/api/openstack/ha/views/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-08-19 12:39:51.000000 masakari-9.1.3/masakari/api/openstack/ha/views/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3167 2021-08-19 12:39:51.000000 masakari-9.1.3/masakari/api/openstack/ha/views/versions.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    38792 2021-08-19 12:39:51.000000 masakari-9.1.3/masakari/api/openstack/wsgi.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10294 2021-08-19 12:39:51.000000 masakari-9.1.3/masakari/api/urlmap.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4498 2021-08-19 12:39:51.000000 masakari-9.1.3/masakari/api/utils.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-08-19 12:40:25.204568 masakari-9.1.3/masakari/api/validation/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1974 2021-08-19 12:39:51.000000 masakari-9.1.3/masakari/api/validation/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5286 2021-08-19 12:39:51.000000 masakari-9.1.3/masakari/api/validation/parameter_types.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8109 2021-08-19 12:39:51.000000 masakari-9.1.3/masakari/api/validation/validators.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1252 2021-08-19 12:39:51.000000 masakari-9.1.3/masakari/api/versioned_method.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-08-19 12:40:25.204568 masakari-9.1.3/masakari/cmd/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      991 2021-08-19 12:39:51.000000 masakari-9.1.3/masakari/cmd/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2767 2021-08-19 12:39:51.000000 masakari-9.1.3/masakari/cmd/api.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1182 2021-08-19 12:39:51.000000 masakari-9.1.3/masakari/cmd/engine.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6671 2021-08-19 12:39:51.000000 masakari-9.1.3/masakari/cmd/manage.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1537 2021-08-19 12:39:51.000000 masakari-9.1.3/masakari/cmd/status.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-08-19 12:40:25.204568 masakari-9.1.3/masakari/common/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-08-19 12:39:51.000000 masakari-9.1.3/masakari/common/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1642 2021-08-19 12:39:51.000000 masakari-9.1.3/masakari/common/config.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-08-19 12:40:25.204568 masakari-9.1.3/masakari/compute/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      753 2021-08-19 12:39:51.000000 masakari-9.1.3/masakari/compute/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9889 2021-08-19 12:39:51.000000 masakari-9.1.3/masakari/compute/nova.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-08-19 12:40:25.208567 masakari-9.1.3/masakari/conf/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1397 2021-08-19 12:39:51.000000 masakari-9.1.3/masakari/conf/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2597 2021-08-19 12:39:51.000000 masakari-9.1.3/masakari/conf/api.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1500 2021-08-19 12:39:51.000000 masakari-9.1.3/masakari/conf/base.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      939 2021-08-19 12:39:51.000000 masakari-9.1.3/masakari/conf/database.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4625 2021-08-19 12:39:51.000000 masakari-9.1.3/masakari/conf/engine.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9167 2021-08-19 12:39:51.000000 masakari-9.1.3/masakari/conf/engine_driver.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      940 2021-08-19 12:39:51.000000 masakari-9.1.3/masakari/conf/exceptions.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2736 2021-08-19 12:39:51.000000 masakari-9.1.3/masakari/conf/nova.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3344 2021-08-19 12:39:51.000000 masakari-9.1.3/masakari/conf/opts.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3064 2021-08-19 12:39:51.000000 masakari-9.1.3/masakari/conf/osapi_v1.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1741 2021-08-19 12:39:51.000000 masakari-9.1.3/masakari/conf/paths.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2725 2021-08-19 12:39:51.000000 masakari-9.1.3/masakari/conf/service.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      769 2021-08-19 12:39:51.000000 masakari-9.1.3/masakari/conf/ssl.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4103 2021-08-19 12:39:51.000000 masakari-9.1.3/masakari/conf/wsgi.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1481 2021-08-19 12:39:51.000000 masakari-9.1.3/masakari/config.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9579 2021-08-19 12:39:51.000000 masakari-9.1.3/masakari/context.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-08-19 12:40:25.208567 masakari-9.1.3/masakari/db/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      699 2021-08-19 12:39:51.000000 masakari-9.1.3/masakari/db/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    13109 2021-08-19 12:39:51.000000 masakari-9.1.3/masakari/db/api.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      876 2021-08-19 12:39:51.000000 masakari-9.1.3/masakari/db/migration.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-08-19 12:40:25.208567 masakari-9.1.3/masakari/db/sqlalchemy/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-08-19 12:39:51.000000 masakari-9.1.3/masakari/db/sqlalchemy/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    23995 2021-08-19 12:39:51.000000 masakari-9.1.3/masakari/db/sqlalchemy/api.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-08-19 12:40:25.212567 masakari-9.1.3/masakari/db/sqlalchemy/migrate_repo/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      110 2021-08-19 12:39:51.000000 masakari-9.1.3/masakari/db/sqlalchemy/migrate_repo/README.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-08-19 12:39:51.000000 masakari-9.1.3/masakari/db/sqlalchemy/migrate_repo/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      857 2021-08-19 12:39:51.000000 masakari-9.1.3/masakari/db/sqlalchemy/migrate_repo/manage.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      983 2021-08-19 12:39:51.000000 masakari-9.1.3/masakari/db/sqlalchemy/migrate_repo/migrate.cfg
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-08-19 12:40:25.212567 masakari-9.1.3/masakari/db/sqlalchemy/migrate_repo/versions/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2805 2021-08-19 12:39:51.000000 masakari-9.1.3/masakari/db/sqlalchemy/migrate_repo/versions/001_add_failover_segments_table.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2499 2021-08-19 12:39:51.000000 masakari-9.1.3/masakari/db/sqlalchemy/migrate_repo/versions/002_add_hosts_table.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1940 2021-08-19 12:39:51.000000 masakari-9.1.3/masakari/db/sqlalchemy/migrate_repo/versions/003_update_unique_constraint_hosts.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2433 2021-08-19 12:39:51.000000 masakari-9.1.3/masakari/db/sqlalchemy/migrate_repo/versions/004_add_notifications_table.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      951 2021-08-19 12:39:51.000000 masakari-9.1.3/masakari/db/sqlalchemy/migrate_repo/versions/005_remove_nullable_mismatch.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1182 2021-08-19 12:39:51.000000 masakari-9.1.3/masakari/db/sqlalchemy/migrate_repo/versions/006_add_persistence_tables.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2450 2021-08-19 12:39:51.000000 masakari-9.1.3/masakari/db/sqlalchemy/migration.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6115 2021-08-19 12:39:51.000000 masakari-9.1.3/masakari/db/sqlalchemy/models.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-08-19 12:40:25.212567 masakari-9.1.3/masakari/engine/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-08-19 12:39:51.000000 masakari-9.1.3/masakari/engine/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2965 2021-08-19 12:39:51.000000 masakari-9.1.3/masakari/engine/driver.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-08-19 12:40:25.212567 masakari-9.1.3/masakari/engine/drivers/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      680 2021-08-19 12:39:51.000000 masakari-9.1.3/masakari/engine/drivers/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-08-19 12:40:25.212567 masakari-9.1.3/masakari/engine/drivers/taskflow/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      716 2021-08-19 12:39:51.000000 masakari-9.1.3/masakari/engine/drivers/taskflow/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5279 2021-08-19 12:39:51.000000 masakari-9.1.3/masakari/engine/drivers/taskflow/base.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    15189 2021-08-19 12:39:51.000000 masakari-9.1.3/masakari/engine/drivers/taskflow/driver.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    20923 2021-08-19 12:39:51.000000 masakari-9.1.3/masakari/engine/drivers/taskflow/host_failure.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8616 2021-08-19 12:39:51.000000 masakari-9.1.3/masakari/engine/drivers/taskflow/instance_failure.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1015 2021-08-19 12:39:51.000000 masakari-9.1.3/masakari/engine/drivers/taskflow/no_op.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5373 2021-08-19 12:39:51.000000 masakari-9.1.3/masakari/engine/drivers/taskflow/process_failure.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1228 2021-08-19 12:39:51.000000 masakari-9.1.3/masakari/engine/instance_events.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    18776 2021-08-19 12:39:51.000000 masakari-9.1.3/masakari/engine/manager.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2077 2021-08-19 12:39:51.000000 masakari-9.1.3/masakari/engine/rpcapi.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2352 2021-08-19 12:39:51.000000 masakari-9.1.3/masakari/engine/utils.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    11516 2021-08-19 12:39:51.000000 masakari-9.1.3/masakari/exception.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-08-19 12:40:25.216568 masakari-9.1.3/masakari/ha/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-08-19 12:39:51.000000 masakari-9.1.3/masakari/ha/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    15855 2021-08-19 12:39:51.000000 masakari-9.1.3/masakari/ha/api.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-08-19 12:40:25.216568 masakari-9.1.3/masakari/hacking/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-08-19 12:39:51.000000 masakari-9.1.3/masakari/hacking/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    16659 2021-08-19 12:39:51.000000 masakari-9.1.3/masakari/hacking/checks.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1041 2021-08-19 12:39:51.000000 masakari-9.1.3/masakari/i18n.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3546 2021-08-19 12:39:51.000000 masakari-9.1.3/masakari/manager.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-08-19 12:40:25.216568 masakari-9.1.3/masakari/notifications/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-08-19 12:39:51.000000 masakari-9.1.3/masakari/notifications/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-08-19 12:40:25.216568 masakari-9.1.3/masakari/notifications/objects/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-08-19 12:39:51.000000 masakari-9.1.3/masakari/notifications/objects/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6378 2021-08-19 12:39:51.000000 masakari-9.1.3/masakari/notifications/objects/base.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2544 2021-08-19 12:39:51.000000 masakari-9.1.3/masakari/notifications/objects/exception.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7005 2021-08-19 12:39:51.000000 masakari-9.1.3/masakari/notifications/objects/notification.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-08-19 12:40:25.216568 masakari-9.1.3/masakari/objects/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      958 2021-08-19 12:39:51.000000 masakari-9.1.3/masakari/objects/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10468 2021-08-19 12:39:51.000000 masakari-9.1.3/masakari/objects/base.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7454 2021-08-19 12:39:51.000000 masakari-9.1.3/masakari/objects/fields.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6284 2021-08-19 12:39:51.000000 masakari-9.1.3/masakari/objects/host.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7279 2021-08-19 12:39:51.000000 masakari-9.1.3/masakari/objects/notification.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5881 2021-08-19 12:39:51.000000 masakari-9.1.3/masakari/objects/segment.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-08-19 12:40:25.216568 masakari-9.1.3/masakari/policies/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1128 2021-08-19 12:39:51.000000 masakari-9.1.3/masakari/policies/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1259 2021-08-19 12:39:51.000000 masakari-9.1.3/masakari/policies/base.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1586 2021-08-19 12:39:51.000000 masakari-9.1.3/masakari/policies/extension_info.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2609 2021-08-19 12:39:51.000000 masakari-9.1.3/masakari/policies/hosts.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1997 2021-08-19 12:39:51.000000 masakari-9.1.3/masakari/policies/notifications.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2532 2021-08-19 12:39:51.000000 masakari-9.1.3/masakari/policies/segments.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1226 2021-08-19 12:39:51.000000 masakari-9.1.3/masakari/policies/versions.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7641 2021-08-19 12:39:51.000000 masakari-9.1.3/masakari/policy.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4955 2021-08-19 12:39:51.000000 masakari-9.1.3/masakari/rpc.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1396 2021-08-19 12:39:51.000000 masakari-9.1.3/masakari/safe_utils.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9696 2021-08-19 12:39:51.000000 masakari-9.1.3/masakari/service.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7322 2021-08-19 12:39:51.000000 masakari-9.1.3/masakari/test.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-08-19 12:40:25.220568 masakari-9.1.3/masakari/tests/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-08-19 12:39:51.000000 masakari-9.1.3/masakari/tests/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      719 2021-08-19 12:39:51.000000 masakari-9.1.3/masakari/tests/base.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4934 2021-08-19 12:39:51.000000 masakari-9.1.3/masakari/tests/fixtures.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-08-19 12:40:25.220568 masakari-9.1.3/masakari/tests/functional/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-08-19 12:39:51.000000 masakari-9.1.3/masakari/tests/functional/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2456 2021-08-19 12:39:51.000000 masakari-9.1.3/masakari/tests/functional/base.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4195 2021-08-19 12:39:51.000000 masakari-9.1.3/masakari/tests/functional/notification_base.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6822 2021-08-19 12:39:51.000000 masakari-9.1.3/masakari/tests/functional/test_hosts.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5009 2021-08-19 12:39:51.000000 masakari-9.1.3/masakari/tests/functional/test_process_notifications.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6413 2021-08-19 12:39:51.000000 masakari-9.1.3/masakari/tests/functional/test_segments.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3138 2021-08-19 12:39:51.000000 masakari-9.1.3/masakari/tests/functional/test_vm_notifications.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2397 2021-08-19 12:39:51.000000 masakari-9.1.3/masakari/tests/json_ref.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-08-19 12:40:25.224568 masakari-9.1.3/masakari/tests/unit/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      841 2021-08-19 12:39:51.000000 masakari-9.1.3/masakari/tests/unit/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-08-19 12:40:25.224568 masakari-9.1.3/masakari/tests/unit/api/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-08-19 12:39:51.000000 masakari-9.1.3/masakari/tests/unit/api/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-08-19 12:40:25.224568 masakari-9.1.3/masakari/tests/unit/api/openstack/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-08-19 12:39:51.000000 masakari-9.1.3/masakari/tests/unit/api/openstack/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4148 2021-08-19 12:39:51.000000 masakari-9.1.3/masakari/tests/unit/api/openstack/fakes.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-08-19 12:40:25.228568 masakari-9.1.3/masakari/tests/unit/api/openstack/ha/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-08-19 12:39:51.000000 masakari-9.1.3/masakari/tests/unit/api/openstack/ha/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4027 2021-08-19 12:39:51.000000 masakari-9.1.3/masakari/tests/unit/api/openstack/ha/test_extension_info.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    22396 2021-08-19 12:39:51.000000 masakari-9.1.3/masakari/tests/unit/api/openstack/ha/test_hosts.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    21557 2021-08-19 12:39:51.000000 masakari-9.1.3/masakari/tests/unit/api/openstack/ha/test_notifications.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    15281 2021-08-19 12:39:51.000000 masakari-9.1.3/masakari/tests/unit/api/openstack/ha/test_segments.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8269 2021-08-19 12:39:51.000000 masakari-9.1.3/masakari/tests/unit/api/openstack/ha/test_versions.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    14458 2021-08-19 12:39:51.000000 masakari-9.1.3/masakari/tests/unit/api/openstack/test_common.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3347 2021-08-19 12:39:51.000000 masakari-9.1.3/masakari/tests/unit/api/openstack/test_extensions.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    38059 2021-08-19 12:39:51.000000 masakari-9.1.3/masakari/tests/unit/api/openstack/test_wsgi.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3802 2021-08-19 12:39:51.000000 masakari-9.1.3/masakari/tests/unit/api/test_api_version_request.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7838 2021-08-19 12:39:51.000000 masakari-9.1.3/masakari/tests/unit/api/test_auth.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7693 2021-08-19 12:39:51.000000 masakari-9.1.3/masakari/tests/unit/api/test_utils.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-08-19 12:40:25.228568 masakari-9.1.3/masakari/tests/unit/cmd/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-08-19 12:39:51.000000 masakari-9.1.3/masakari/tests/unit/cmd/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2085 2021-08-19 12:39:51.000000 masakari-9.1.3/masakari/tests/unit/cmd/test_masakari_api.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1014 2021-08-19 12:39:51.000000 masakari-9.1.3/masakari/tests/unit/cmd/test_status.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-08-19 12:40:25.228568 masakari-9.1.3/masakari/tests/unit/compute/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-08-19 12:39:51.000000 masakari-9.1.3/masakari/tests/unit/compute/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    15540 2021-08-19 12:39:51.000000 masakari-9.1.3/masakari/tests/unit/compute/test_nova.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1556 2021-08-19 12:39:51.000000 masakari-9.1.3/masakari/tests/unit/conf_fixture.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-08-19 12:40:25.228568 masakari-9.1.3/masakari/tests/unit/db/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-08-19 12:39:51.000000 masakari-9.1.3/masakari/tests/unit/db/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    22215 2021-08-19 12:39:51.000000 masakari-9.1.3/masakari/tests/unit/db/test_db_api.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10513 2021-08-19 12:39:51.000000 masakari-9.1.3/masakari/tests/unit/db/test_migrations.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6824 2021-08-19 12:39:51.000000 masakari-9.1.3/masakari/tests/unit/db/test_purge.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-08-19 12:40:25.228568 masakari-9.1.3/masakari/tests/unit/engine/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-08-19 12:39:51.000000 masakari-9.1.3/masakari/tests/unit/engine/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-08-19 12:40:25.228568 masakari-9.1.3/masakari/tests/unit/engine/drivers/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-08-19 12:39:51.000000 masakari-9.1.3/masakari/tests/unit/engine/drivers/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-08-19 12:40:25.232568 masakari-9.1.3/masakari/tests/unit/engine/drivers/taskflow/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-08-19 12:39:51.000000 masakari-9.1.3/masakari/tests/unit/engine/drivers/taskflow/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    37972 2021-08-19 12:39:51.000000 masakari-9.1.3/masakari/tests/unit/engine/drivers/taskflow/test_host_failure_flow.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    12277 2021-08-19 12:39:51.000000 masakari-9.1.3/masakari/tests/unit/engine/drivers/taskflow/test_instance_failure_flow.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6436 2021-08-19 12:39:51.000000 masakari-9.1.3/masakari/tests/unit/engine/drivers/taskflow/test_process_failure_flow.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    18931 2021-08-19 12:39:51.000000 masakari-9.1.3/masakari/tests/unit/engine/drivers/taskflow/test_taskflow_driver.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1881 2021-08-19 12:39:51.000000 masakari-9.1.3/masakari/tests/unit/engine/fake_engine.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    58476 2021-08-19 12:39:51.000000 masakari-9.1.3/masakari/tests/unit/engine/test_engine_mgr.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3769 2021-08-19 12:39:51.000000 masakari-9.1.3/masakari/tests/unit/engine/test_rpcapi.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3341 2021-08-19 12:39:51.000000 masakari-9.1.3/masakari/tests/unit/engine/test_utils.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2853 2021-08-19 12:39:51.000000 masakari-9.1.3/masakari/tests/unit/fake_notifier.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1325 2021-08-19 12:39:51.000000 masakari-9.1.3/masakari/tests/unit/fake_policy.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7855 2021-08-19 12:39:51.000000 masakari-9.1.3/masakari/tests/unit/fakes.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-08-19 12:40:25.232568 masakari-9.1.3/masakari/tests/unit/ha/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-08-19 12:39:51.000000 masakari-9.1.3/masakari/tests/unit/ha/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    45120 2021-08-19 12:39:51.000000 masakari-9.1.3/masakari/tests/unit/ha/test_api.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1744 2021-08-19 12:39:51.000000 masakari-9.1.3/masakari/tests/unit/matchers.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-08-19 12:40:25.232568 masakari-9.1.3/masakari/tests/unit/monkey_patch_example/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1099 2021-08-19 12:39:51.000000 masakari-9.1.3/masakari/tests/unit/monkey_patch_example/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      905 2021-08-19 12:39:51.000000 masakari-9.1.3/masakari/tests/unit/monkey_patch_example/example_a.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      906 2021-08-19 12:39:51.000000 masakari-9.1.3/masakari/tests/unit/monkey_patch_example/example_b.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-08-19 12:40:25.232568 masakari-9.1.3/masakari/tests/unit/notifications/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-08-19 12:39:51.000000 masakari-9.1.3/masakari/tests/unit/notifications/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-08-19 12:40:25.232568 masakari-9.1.3/masakari/tests/unit/notifications/objects/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-08-19 12:39:51.000000 masakari-9.1.3/masakari/tests/unit/notifications/objects/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10810 2021-08-19 12:39:51.000000 masakari-9.1.3/masakari/tests/unit/notifications/objects/test_notification.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-08-19 12:40:25.232568 masakari-9.1.3/masakari/tests/unit/objects/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-08-19 12:39:51.000000 masakari-9.1.3/masakari/tests/unit/objects/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2735 2021-08-19 12:39:51.000000 masakari-9.1.3/masakari/tests/unit/objects/fake_args.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8095 2021-08-19 12:39:51.000000 masakari-9.1.3/masakari/tests/unit/objects/test_fields.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    12394 2021-08-19 12:39:51.000000 masakari-9.1.3/masakari/tests/unit/objects/test_hosts.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    11272 2021-08-19 12:39:51.000000 masakari-9.1.3/masakari/tests/unit/objects/test_notifications.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    33197 2021-08-19 12:39:51.000000 masakari-9.1.3/masakari/tests/unit/objects/test_objects.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    12312 2021-08-19 12:39:51.000000 masakari-9.1.3/masakari/tests/unit/objects/test_segments.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3663 2021-08-19 12:39:51.000000 masakari-9.1.3/masakari/tests/unit/policy_fixture.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    21707 2021-08-19 12:39:51.000000 masakari-9.1.3/masakari/tests/unit/test_api_validation.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2940 2021-08-19 12:39:51.000000 masakari-9.1.3/masakari/tests/unit/test_conf.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6127 2021-08-19 12:39:51.000000 masakari-9.1.3/masakari/tests/unit/test_context.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5907 2021-08-19 12:39:51.000000 masakari-9.1.3/masakari/tests/unit/test_exception.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    20938 2021-08-19 12:39:51.000000 masakari-9.1.3/masakari/tests/unit/test_hacking.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3157 2021-08-19 12:39:51.000000 masakari-9.1.3/masakari/tests/unit/test_masakari_manage.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10359 2021-08-19 12:39:51.000000 masakari-9.1.3/masakari/tests/unit/test_policy.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10831 2021-08-19 12:39:51.000000 masakari-9.1.3/masakari/tests/unit/test_rpc.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2544 2021-08-19 12:39:51.000000 masakari-9.1.3/masakari/tests/unit/test_safeutils.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6569 2021-08-19 12:39:51.000000 masakari-9.1.3/masakari/tests/unit/test_service.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9193 2021-08-19 12:39:51.000000 masakari-9.1.3/masakari/tests/unit/test_utils.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2177 2021-08-19 12:39:51.000000 masakari-9.1.3/masakari/tests/unit/test_versions.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8203 2021-08-19 12:39:51.000000 masakari-9.1.3/masakari/tests/unit/test_wsgi.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2038 2021-08-19 12:39:51.000000 masakari-9.1.3/masakari/tests/unit/utils.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1091 2021-08-19 12:39:51.000000 masakari-9.1.3/masakari/tests/uuidsentinel.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9364 2021-08-19 12:39:51.000000 masakari-9.1.3/masakari/utils.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2395 2021-08-19 12:39:51.000000 masakari-9.1.3/masakari/version.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    16879 2021-08-19 12:39:51.000000 masakari-9.1.3/masakari/wsgi.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-08-19 12:40:25.200567 masakari-9.1.3/masakari.egg-info/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4486 2021-08-19 12:40:25.000000 masakari-9.1.3/masakari.egg-info/PKG-INFO
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    14192 2021-08-19 12:40:25.000000 masakari-9.1.3/masakari.egg-info/SOURCES.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2021-08-19 12:40:25.000000 masakari-9.1.3/masakari.egg-info/dependency_links.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2007 2021-08-19 12:40:25.000000 masakari-9.1.3/masakari.egg-info/entry_points.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2021-08-19 12:40:25.000000 masakari-9.1.3/masakari.egg-info/not-zip-safe
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       46 2021-08-19 12:40:25.000000 masakari-9.1.3/masakari.egg-info/pbr.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      540 2021-08-19 12:40:25.000000 masakari-9.1.3/masakari.egg-info/requires.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        9 2021-08-19 12:40:25.000000 masakari-9.1.3/masakari.egg-info/top_level.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-08-19 12:40:25.176567 masakari-9.1.3/playbooks/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-08-19 12:40:25.232568 masakari-9.1.3/playbooks/devstack/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       71 2021-08-19 12:39:51.000000 masakari-9.1.3/playbooks/devstack/post.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      152 2021-08-19 12:39:51.000000 masakari-9.1.3/playbooks/devstack/pre.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       39 2021-08-19 12:39:51.000000 masakari-9.1.3/playbooks/devstack/run.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-08-19 12:40:25.176567 masakari-9.1.3/releasenotes/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-08-19 12:40:25.240568 masakari-9.1.3/releasenotes/notes/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-08-19 12:39:51.000000 masakari-9.1.3/releasenotes/notes/.placeholder
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      998 2021-08-19 12:39:51.000000 masakari-9.1.3/releasenotes/notes/add-periodic-tasks-0c96d6f620502a75.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      477 2021-08-19 12:39:51.000000 masakari-9.1.3/releasenotes/notes/add-upgrade-check-framework-52268130b25317ab.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      686 2021-08-19 12:39:51.000000 masakari-9.1.3/releasenotes/notes/add_evacuate_error_instances_conf_option-5b4d1906137395f0.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1477 2021-08-19 12:39:51.000000 masakari-9.1.3/releasenotes/notes/add_ha_enabled_config_options-54a9270a5993d20a.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      416 2021-08-19 12:39:51.000000 masakari-9.1.3/releasenotes/notes/add_reserved_host_to_aggregates-5f506d08354ec148.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      327 2021-08-19 12:39:51.000000 masakari-9.1.3/releasenotes/notes/adopt-oslo-config-generator-cf2fdb17cf7f13db.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      699 2021-08-19 12:39:51.000000 masakari-9.1.3/releasenotes/notes/auto_priority_and_rh_priority_recovery_methods-b88cc00041fa2c4d.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      250 2021-08-19 12:39:51.000000 masakari-9.1.3/releasenotes/notes/bp-mutable-config-57efdd467c01aa7b.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      176 2021-08-19 12:39:51.000000 masakari-9.1.3/releasenotes/notes/bug-1685145-3d93145bfc76c660.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      136 2021-08-19 12:39:51.000000 masakari-9.1.3/releasenotes/notes/bug-1776385-0bcf0a0b3fad359e.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      179 2021-08-19 12:39:51.000000 masakari-9.1.3/releasenotes/notes/bug-1782517-e4dc70bad9e4e131.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      174 2021-08-19 12:39:51.000000 masakari-9.1.3/releasenotes/notes/bug-1856164-6601a6e6280eba4d.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      175 2021-08-19 12:39:51.000000 masakari-9.1.3/releasenotes/notes/bug-1859406-6b041a26acf6c7f6.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      159 2021-08-19 12:39:51.000000 masakari-9.1.3/releasenotes/notes/bug-1882516-e8dc7fd2b55f065f.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      180 2021-08-19 12:39:51.000000 masakari-9.1.3/releasenotes/notes/bug-1932194-2b721860bbc26819.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      284 2021-08-19 12:39:51.000000 masakari-9.1.3/releasenotes/notes/bug-add-missing-domain-name-5181c02f3f033a22.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      304 2021-08-19 12:39:51.000000 masakari-9.1.3/releasenotes/notes/compute_search-3da97e69e661a73f.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      681 2021-08-19 12:39:51.000000 masakari-9.1.3/releasenotes/notes/correct_response_code-df8b43a201efa1b4.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      434 2021-08-19 12:39:51.000000 masakari-9.1.3/releasenotes/notes/db-purge-support-7a33e2ea5d2a624b.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      130 2021-08-19 12:39:51.000000 masakari-9.1.3/releasenotes/notes/deprecate-topic-opt-af83f82143143c61.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      206 2021-08-19 12:39:51.000000 masakari-9.1.3/releasenotes/notes/drop-py-2-7-059d3cd5e7cb4e1a.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      642 2021-08-19 12:39:51.000000 masakari-9.1.3/releasenotes/notes/evacuation_in_threads-cc9c79b10acfb5f6.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      444 2021-08-19 12:39:51.000000 masakari-9.1.3/releasenotes/notes/failover_segment_apis-f5bea1cd6d103048.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      219 2021-08-19 12:39:51.000000 masakari-9.1.3/releasenotes/notes/fix-endless-periodic-f223845f3044b166.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      625 2021-08-19 12:39:51.000000 masakari-9.1.3/releasenotes/notes/host-apis-46a87fcd56d8ed30.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      658 2021-08-19 12:39:51.000000 masakari-9.1.3/releasenotes/notes/notifications-in-masakari-f5d79838fc23cb9b.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      303 2021-08-19 12:39:51.000000 masakari-9.1.3/releasenotes/notes/notifications_apis-3c3d5055ae9c6649.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1148 2021-08-19 12:39:51.000000 masakari-9.1.3/releasenotes/notes/policy-in-code-8740d51624055044.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1235 2021-08-19 12:39:51.000000 masakari-9.1.3/releasenotes/notes/progress-details-recovery-workflows-5b14b7b3f87374f4.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      865 2021-08-19 12:39:51.000000 masakari-9.1.3/releasenotes/notes/recovery-method-customization-3438b0e26e322b88.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      392 2021-08-19 12:39:51.000000 masakari-9.1.3/releasenotes/notes/reserved_host_recovery_method-d2de1f205136c8d5.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      350 2021-08-19 12:39:51.000000 masakari-9.1.3/releasenotes/notes/wsgi-applications-3ed7d6b89f1a5785.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-08-19 12:40:25.240568 masakari-9.1.3/releasenotes/source/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-08-19 12:40:25.240568 masakari-9.1.3/releasenotes/source/_static/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-08-19 12:39:51.000000 masakari-9.1.3/releasenotes/source/_static/.placeholder
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-08-19 12:40:25.240568 masakari-9.1.3/releasenotes/source/_templates/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-08-19 12:39:51.000000 masakari-9.1.3/releasenotes/source/_templates/.placeholder
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8995 2021-08-19 12:39:51.000000 masakari-9.1.3/releasenotes/source/conf.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      217 2021-08-19 12:39:51.000000 masakari-9.1.3/releasenotes/source/index.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      137 2021-08-19 12:39:51.000000 masakari-9.1.3/releasenotes/source/ocata.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      133 2021-08-19 12:39:51.000000 masakari-9.1.3/releasenotes/source/pike.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      141 2021-08-19 12:39:51.000000 masakari-9.1.3/releasenotes/source/queens.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      145 2021-08-19 12:39:51.000000 masakari-9.1.3/releasenotes/source/rocky.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      145 2021-08-19 12:39:51.000000 masakari-9.1.3/releasenotes/source/stein.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      126 2021-08-19 12:39:51.000000 masakari-9.1.3/releasenotes/source/train.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      112 2021-08-19 12:39:51.000000 masakari-9.1.3/releasenotes/source/unreleased.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1047 2021-08-19 12:39:51.000000 masakari-9.1.3/requirements.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-08-19 12:40:25.176567 masakari-9.1.3/roles/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-08-19 12:40:25.176567 masakari-9.1.3/roles/devstack-config/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-08-19 12:40:25.240568 masakari-9.1.3/roles/devstack-config/tasks/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      418 2021-08-19 12:39:51.000000 masakari-9.1.3/roles/devstack-config/tasks/main.yml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3159 2021-08-19 12:40:25.244568 masakari-9.1.3/setup.cfg
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1030 2021-08-19 12:39:51.000000 masakari-9.1.3/setup.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      693 2021-08-19 12:39:51.000000 masakari-9.1.3/test-requirements.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3503 2021-08-19 12:39:51.000000 masakari-9.1.3/tox.ini
```

### Comparing `masakari-9.1.2/.zuul.yaml` & `masakari-9.1.3/.zuul.yaml`

 * *Files identical despite different names*

### Comparing `masakari-9.1.2/AUTHORS` & `masakari-9.1.3/AUTHORS`

 * *Files 6% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 James Page <james.page@ubuntu.com>
 Jean-Philippe Evrard <jean-philippe@evrard.me>
 Ji-Wei <ji.wei3@zte.com.cn>
 Kengo Takahara <takahara-kn@njk.co.jp>
 Kengo Takahara <takahara.kengo.z03@as.ntts.co.jp>
 Louie KWAN <louie.kwan@windriver.com>
 Mark Goddard <mark@stackhpc.com>
+Mitya_Eremeev <mitossvyaz@mail.ru>
 Neha Alhat <neha.alhat@nttdata.com>
 Nguyen Hai <nguyentrihai93@gmail.com>
 Nguyen Hung Phuong <phuongnh@vn.fujitsu.com>
 OpenStack Release Bot <infra-root@openstack.org>
 Radosław Piliszek <radoslaw.piliszek@gmail.com>
 Rikimaru Honjo <honjo.rikimaru@po.ntt-tx.co.jp>
 Rikimaru Honjo <honjo.rikimaru@po.ntts.co.jp>
```

### Comparing `masakari-9.1.2/CONTRIBUTING.rst` & `masakari-9.1.3/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `masakari-9.1.2/ChangeLog` & `masakari-9.1.3/ChangeLog`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,15 @@
 CHANGES
 =======
 
+9.1.3
+-----
+
+* Fix Masakari API to properly return error codes
+
 9.1.2
 -----
 
 * Search in nova services instead of hypervisors
 * Fix some errors in the document
 * Assign all aggregates to reserved\_host
 * Fix response of microversions API
```

### Comparing `masakari-9.1.2/HACKING.rst` & `masakari-9.1.3/HACKING.rst`

 * *Files identical despite different names*

### Comparing `masakari-9.1.2/LICENSE` & `masakari-9.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `masakari-9.1.2/PKG-INFO` & `masakari-9.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: masakari
-Version: 9.1.2
+Version: 9.1.3
 Summary: Virtual Machine High Availability (VMHA) service for OpenStack
 Home-page: https://docs.openstack.org/masakari/latest/
 Author: OpenStack
 Author-email: openstack-discuss@lists.openstack.org
 License: UNKNOWN
 Description: ========
         Masakari
```

### Comparing `masakari-9.1.2/README.rst` & `masakari-9.1.3/README.rst`

 * *Files identical despite different names*

### Comparing `masakari-9.1.2/api-ref/source/conf.py` & `masakari-9.1.3/api-ref/source/conf.py`

 * *Files identical despite different names*

### Comparing `masakari-9.1.2/api-ref/source/failover-segments.inc` & `masakari-9.1.3/api-ref/source/failover-segments.inc`

 * *Files identical despite different names*

### Comparing `masakari-9.1.2/api-ref/source/hosts.inc` & `masakari-9.1.3/api-ref/source/hosts.inc`

 * *Files identical despite different names*

### Comparing `masakari-9.1.2/api-ref/source/notifications.inc` & `masakari-9.1.3/api-ref/source/notifications.inc`

 * *Files identical despite different names*

### Comparing `masakari-9.1.2/api-ref/source/parameters.yaml` & `masakari-9.1.3/api-ref/source/parameters.yaml`

 * *Files identical despite different names*

### Comparing `masakari-9.1.2/api-ref/source/status.yaml` & `masakari-9.1.3/api-ref/source/status.yaml`

 * *Files identical despite different names*

### Comparing `masakari-9.1.2/api-ref/source/versions.inc` & `masakari-9.1.3/api-ref/source/versions.inc`

 * *Files identical despite different names*

### Comparing `masakari-9.1.2/devstack/README.rst` & `masakari-9.1.3/devstack/README.rst`

 * *Files identical despite different names*

### Comparing `masakari-9.1.2/devstack/plugin.sh` & `masakari-9.1.3/devstack/plugin.sh`

 * *Files identical despite different names*

### Comparing `masakari-9.1.2/devstack/settings` & `masakari-9.1.3/devstack/settings`

 * *Files identical despite different names*

### Comparing `masakari-9.1.2/doc/api_samples/hosts/host-create-resp.json` & `masakari-9.1.3/doc/api_samples/hosts/host-create-resp.json`

 * *Files identical despite different names*

### Comparing `masakari-9.1.2/doc/api_samples/hosts/host-get-resp.json` & `masakari-9.1.3/doc/api_samples/hosts/host-get-resp.json`

 * *Files identical despite different names*

### Comparing `masakari-9.1.2/doc/api_samples/hosts/host-update-resp.json` & `masakari-9.1.3/doc/api_samples/hosts/host-update-resp.json`

 * *Files identical despite different names*

### Comparing `masakari-9.1.2/doc/api_samples/hosts/hosts-list-resp.json` & `masakari-9.1.3/doc/api_samples/hosts/hosts-list-resp.json`

 * *Files identical despite different names*

### Comparing `masakari-9.1.2/doc/api_samples/notifications/host-notification-create-resp.json` & `masakari-9.1.3/doc/api_samples/notifications/host-notification-create-resp.json`

 * *Files identical despite different names*

### Comparing `masakari-9.1.2/doc/api_samples/notifications/notifcations-list-resp.json` & `masakari-9.1.3/doc/api_samples/notifications/notifcations-list-resp.json`

 * *Files identical despite different names*

### Comparing `masakari-9.1.2/doc/api_samples/notifications/notification-get-resp.json` & `masakari-9.1.3/doc/api_samples/notifications/notification-get-resp.json`

 * *Files identical despite different names*

### Comparing `masakari-9.1.2/doc/api_samples/notifications/process-notification-create-resp.json` & `masakari-9.1.3/doc/api_samples/notifications/process-notification-create-resp.json`

 * *Files identical despite different names*

### Comparing `masakari-9.1.2/doc/api_samples/notifications/vm-notification-create-resp.json` & `masakari-9.1.3/doc/api_samples/notifications/vm-notification-create-resp.json`

 * *Files identical despite different names*

### Comparing `masakari-9.1.2/doc/api_samples/versions/v1-version-get-resp.json` & `masakari-9.1.3/doc/api_samples/versions/v1-version-get-resp.json`

 * *Files identical despite different names*

### Comparing `masakari-9.1.2/doc/ext/versioned_notifications.py` & `masakari-9.1.3/doc/ext/versioned_notifications.py`

 * *Files identical despite different names*

### Comparing `masakari-9.1.2/doc/notification_samples/create-host-end.json` & `masakari-9.1.3/doc/notification_samples/create-host-end.json`

 * *Files identical despite different names*

### Comparing `masakari-9.1.2/doc/notification_samples/create-host-start.json` & `masakari-9.1.3/doc/notification_samples/create-host-start.json`

 * *Files identical despite different names*

### Comparing `masakari-9.1.2/doc/notification_samples/create-notification-end.json` & `masakari-9.1.3/doc/notification_samples/create-notification-end.json`

 * *Files identical despite different names*

### Comparing `masakari-9.1.2/doc/notification_samples/create-notification-start.json` & `masakari-9.1.3/doc/notification_samples/create-notification-start.json`

 * *Files identical despite different names*

### Comparing `masakari-9.1.2/doc/notification_samples/create-segment-end.json` & `masakari-9.1.3/doc/notification_samples/create-segment-end.json`

 * *Files identical despite different names*

### Comparing `masakari-9.1.2/doc/notification_samples/create-segment-start.json` & `masakari-9.1.3/doc/notification_samples/create-segment-start.json`

 * *Files identical despite different names*

### Comparing `masakari-9.1.2/doc/notification_samples/delete-host-end.json` & `masakari-9.1.3/doc/notification_samples/delete-host-end.json`

 * *Files identical despite different names*

### Comparing `masakari-9.1.2/doc/notification_samples/delete-host-start.json` & `masakari-9.1.3/doc/notification_samples/delete-host-start.json`

 * *Files identical despite different names*

### Comparing `masakari-9.1.2/doc/notification_samples/delete-segment-end.json` & `masakari-9.1.3/doc/notification_samples/delete-segment-end.json`

 * *Files identical despite different names*

### Comparing `masakari-9.1.2/doc/notification_samples/delete-segment-start.json` & `masakari-9.1.3/doc/notification_samples/delete-segment-start.json`

 * *Files identical despite different names*

### Comparing `masakari-9.1.2/doc/notification_samples/error-exception.json` & `masakari-9.1.3/doc/notification_samples/error-exception.json`

 * *Files identical despite different names*

### Comparing `masakari-9.1.2/doc/notification_samples/process-notification-end.json` & `masakari-9.1.3/doc/notification_samples/process-notification-end.json`

 * *Files identical despite different names*

### Comparing `masakari-9.1.2/doc/notification_samples/process-notification-error.json` & `masakari-9.1.3/doc/notification_samples/process-notification-error.json`

 * *Files identical despite different names*

### Comparing `masakari-9.1.2/doc/notification_samples/process-notification-start.json` & `masakari-9.1.3/doc/notification_samples/process-notification-start.json`

 * *Files identical despite different names*

### Comparing `masakari-9.1.2/doc/notification_samples/update-host-end.json` & `masakari-9.1.3/doc/notification_samples/update-host-end.json`

 * *Files identical despite different names*

### Comparing `masakari-9.1.2/doc/notification_samples/update-host-start.json` & `masakari-9.1.3/doc/notification_samples/update-host-start.json`

 * *Files identical despite different names*

### Comparing `masakari-9.1.2/doc/notification_samples/update-segment-end.json` & `masakari-9.1.3/doc/notification_samples/update-segment-end.json`

 * *Files identical despite different names*

### Comparing `masakari-9.1.2/doc/notification_samples/update-segment-start.json` & `masakari-9.1.3/doc/notification_samples/update-segment-start.json`

 * *Files identical despite different names*

### Comparing `masakari-9.1.2/doc/source/_static/Masakari_spec_process.svg` & `masakari-9.1.3/doc/source/_static/Masakari_spec_process.svg`

 * *Files identical despite different names*

### Comparing `masakari-9.1.2/doc/source/_static/architecture.png` & `masakari-9.1.3/doc/source/_static/architecture.png`

 * *Files identical despite different names*

### Comparing `masakari-9.1.2/doc/source/cli/masakari-manage.rst` & `masakari-9.1.3/doc/source/cli/masakari-manage.rst`

 * *Files identical despite different names*

### Comparing `masakari-9.1.2/doc/source/cli/masakari-status.rst` & `masakari-9.1.3/doc/source/cli/masakari-status.rst`

 * *Files identical despite different names*

### Comparing `masakari-9.1.2/doc/source/conf.py` & `masakari-9.1.3/doc/source/conf.py`

 * *Files identical despite different names*

### Comparing `masakari-9.1.2/doc/source/configuration/index.rst` & `masakari-9.1.3/doc/source/configuration/index.rst`

 * *Files identical despite different names*

### Comparing `masakari-9.1.2/doc/source/configuration/recovery_workflow_custom_task.rst` & `masakari-9.1.3/doc/source/configuration/recovery_workflow_custom_task.rst`

 * *Files identical despite different names*

### Comparing `masakari-9.1.2/doc/source/configuration/recovery_workflow_sample_config.rst` & `masakari-9.1.3/doc/source/configuration/recovery_workflow_sample_config.rst`

 * *Files identical despite different names*

### Comparing `masakari-9.1.2/doc/source/configuration/sample_config.rst` & `masakari-9.1.3/doc/source/configuration/sample_config.rst`

 * *Files identical despite different names*

### Comparing `masakari-9.1.2/doc/source/index.rst` & `masakari-9.1.3/doc/source/index.rst`

 * *Files identical despite different names*

### Comparing `masakari-9.1.2/doc/source/install/development.environment.rst` & `masakari-9.1.3/doc/source/install/development.environment.rst`

 * *Files identical despite different names*

### Comparing `masakari-9.1.2/doc/source/install/install_and_configure.rst` & `masakari-9.1.3/doc/source/install/install_and_configure.rst`

 * *Files identical despite different names*

### Comparing `masakari-9.1.2/doc/source/install/install_and_configure_ubuntu.rst` & `masakari-9.1.3/doc/source/install/install_and_configure_ubuntu.rst`

 * *Files identical despite different names*

### Comparing `masakari-9.1.2/doc/source/install/overview.rst` & `masakari-9.1.3/doc/source/install/overview.rst`

 * *Files identical despite different names*

### Comparing `masakari-9.1.2/doc/source/install/verify.rst` & `masakari-9.1.3/doc/source/install/verify.rst`

 * *Files identical despite different names*

### Comparing `masakari-9.1.2/doc/source/user/architecture.rst` & `masakari-9.1.3/doc/source/user/architecture.rst`

 * *Files identical despite different names*

### Comparing `masakari-9.1.2/doc/source/user/how_to_get_involved.rst` & `masakari-9.1.3/doc/source/user/how_to_get_involved.rst`

 * *Files identical despite different names*

### Comparing `masakari-9.1.2/doc/source/user/notifications.rst` & `masakari-9.1.3/doc/source/user/notifications.rst`

 * *Files identical despite different names*

### Comparing `masakari-9.1.2/doc/source/user/process.rst` & `masakari-9.1.3/doc/source/user/process.rst`

 * *Files identical despite different names*

### Comparing `masakari-9.1.2/etc/masakari/api-paste.ini` & `masakari-9.1.3/etc/masakari/api-paste.ini`

 * *Files identical despite different names*

### Comparing `masakari-9.1.2/etc/masakari/masakari-custom-recovery-methods.conf` & `masakari-9.1.3/etc/masakari/masakari-custom-recovery-methods.conf`

 * *Files identical despite different names*

### Comparing `masakari-9.1.2/etc/masakari/masakari.conf` & `masakari-9.1.3/etc/masakari/masakari.conf`

 * *Files identical despite different names*

### Comparing `masakari-9.1.2/masakari/__init__.py` & `masakari-9.1.3/masakari/__init__.py`

 * *Files identical despite different names*

### Comparing `masakari-9.1.2/masakari/api/api_version_request.py` & `masakari-9.1.3/masakari/api/api_version_request.py`

 * *Files identical despite different names*

### Comparing `masakari-9.1.2/masakari/api/auth.py` & `masakari-9.1.3/masakari/api/auth.py`

 * *Files identical despite different names*

### Comparing `masakari-9.1.2/masakari/api/openstack/__init__.py` & `masakari-9.1.3/masakari/api/openstack/__init__.py`

 * *Files identical despite different names*

### Comparing `masakari-9.1.2/masakari/api/openstack/common.py` & `masakari-9.1.3/masakari/api/openstack/common.py`

 * *Files identical despite different names*

### Comparing `masakari-9.1.2/masakari/api/openstack/extensions.py` & `masakari-9.1.3/masakari/api/openstack/extensions.py`

 * *Files identical despite different names*

### Comparing `masakari-9.1.2/masakari/api/openstack/ha/__init__.py` & `masakari-9.1.3/masakari/api/openstack/ha/__init__.py`

 * *Files identical despite different names*

### Comparing `masakari-9.1.2/masakari/api/openstack/ha/extension_info.py` & `masakari-9.1.3/masakari/api/openstack/ha/extension_info.py`

 * *Files identical despite different names*

### Comparing `masakari-9.1.2/masakari/api/openstack/ha/hosts.py` & `masakari-9.1.3/masakari/api/openstack/ha/hosts.py`

 * *Files identical despite different names*

### Comparing `masakari-9.1.2/masakari/api/openstack/ha/notifications.py` & `masakari-9.1.3/masakari/api/openstack/ha/notifications.py`

 * *Files identical despite different names*

### Comparing `masakari-9.1.2/masakari/api/openstack/ha/schemas/hosts.py` & `masakari-9.1.3/masakari/api/openstack/ha/schemas/hosts.py`

 * *Files identical despite different names*

### Comparing `masakari-9.1.2/masakari/api/openstack/ha/schemas/notifications.py` & `masakari-9.1.3/masakari/api/openstack/ha/schemas/notifications.py`

 * *Files identical despite different names*

### Comparing `masakari-9.1.2/masakari/api/openstack/ha/schemas/payload.py` & `masakari-9.1.3/masakari/api/openstack/ha/schemas/payload.py`

 * *Files identical despite different names*

### Comparing `masakari-9.1.2/masakari/api/openstack/ha/schemas/segments.py` & `masakari-9.1.3/masakari/api/openstack/ha/schemas/segments.py`

 * *Files identical despite different names*

### Comparing `masakari-9.1.2/masakari/api/openstack/ha/segments.py` & `masakari-9.1.3/masakari/api/openstack/ha/segments.py`

 * *Files identical despite different names*

### Comparing `masakari-9.1.2/masakari/api/openstack/ha/versions.py` & `masakari-9.1.3/masakari/api/openstack/ha/versions.py`

 * *Files identical despite different names*

### Comparing `masakari-9.1.2/masakari/api/openstack/ha/versionsV1.py` & `masakari-9.1.3/masakari/api/openstack/ha/versionsV1.py`

 * *Files identical despite different names*

### Comparing `masakari-9.1.2/masakari/api/openstack/ha/views/versions.py` & `masakari-9.1.3/masakari/api/openstack/ha/views/versions.py`

 * *Files identical despite different names*

### Comparing `masakari-9.1.2/masakari/api/openstack/wsgi.py` & `masakari-9.1.3/masakari/api/openstack/wsgi.py`

 * *Files identical despite different names*

### Comparing `masakari-9.1.2/masakari/api/urlmap.py` & `masakari-9.1.3/masakari/api/urlmap.py`

 * *Files identical despite different names*

### Comparing `masakari-9.1.2/masakari/api/utils.py` & `masakari-9.1.3/masakari/api/utils.py`

 * *Files identical despite different names*

### Comparing `masakari-9.1.2/masakari/api/validation/__init__.py` & `masakari-9.1.3/masakari/api/validation/__init__.py`

 * *Files identical despite different names*

### Comparing `masakari-9.1.2/masakari/api/validation/parameter_types.py` & `masakari-9.1.3/masakari/api/validation/parameter_types.py`

 * *Files identical despite different names*

### Comparing `masakari-9.1.2/masakari/api/validation/validators.py` & `masakari-9.1.3/masakari/api/validation/validators.py`

 * *Files identical despite different names*

### Comparing `masakari-9.1.2/masakari/api/versioned_method.py` & `masakari-9.1.3/masakari/api/versioned_method.py`

 * *Files identical despite different names*

### Comparing `masakari-9.1.2/masakari/cmd/__init__.py` & `masakari-9.1.3/masakari/cmd/__init__.py`

 * *Files identical despite different names*

### Comparing `masakari-9.1.2/masakari/cmd/api.py` & `masakari-9.1.3/masakari/cmd/api.py`

 * *Files identical despite different names*

### Comparing `masakari-9.1.2/masakari/cmd/engine.py` & `masakari-9.1.3/masakari/cmd/engine.py`

 * *Files identical despite different names*

### Comparing `masakari-9.1.2/masakari/cmd/manage.py` & `masakari-9.1.3/masakari/cmd/manage.py`

 * *Files identical despite different names*

### Comparing `masakari-9.1.2/masakari/cmd/status.py` & `masakari-9.1.3/masakari/cmd/status.py`

 * *Files identical despite different names*

### Comparing `masakari-9.1.2/masakari/common/config.py` & `masakari-9.1.3/masakari/common/config.py`

 * *Files identical despite different names*

### Comparing `masakari-9.1.2/masakari/compute/__init__.py` & `masakari-9.1.3/masakari/compute/__init__.py`

 * *Files identical despite different names*

### Comparing `masakari-9.1.2/masakari/compute/nova.py` & `masakari-9.1.3/masakari/compute/nova.py`

 * *Files identical despite different names*

### Comparing `masakari-9.1.2/masakari/conf/__init__.py` & `masakari-9.1.3/masakari/conf/__init__.py`

 * *Files identical despite different names*

### Comparing `masakari-9.1.2/masakari/conf/api.py` & `masakari-9.1.3/masakari/conf/api.py`

 * *Files identical despite different names*

### Comparing `masakari-9.1.2/masakari/conf/base.py` & `masakari-9.1.3/masakari/conf/base.py`

 * *Files identical despite different names*

### Comparing `masakari-9.1.2/masakari/conf/database.py` & `masakari-9.1.3/masakari/conf/database.py`

 * *Files identical despite different names*

### Comparing `masakari-9.1.2/masakari/conf/engine.py` & `masakari-9.1.3/masakari/conf/engine.py`

 * *Files identical despite different names*

### Comparing `masakari-9.1.2/masakari/conf/engine_driver.py` & `masakari-9.1.3/masakari/conf/engine_driver.py`

 * *Files identical despite different names*

### Comparing `masakari-9.1.2/masakari/conf/exceptions.py` & `masakari-9.1.3/masakari/conf/exceptions.py`

 * *Files identical despite different names*

### Comparing `masakari-9.1.2/masakari/conf/nova.py` & `masakari-9.1.3/masakari/conf/nova.py`

 * *Files identical despite different names*

### Comparing `masakari-9.1.2/masakari/conf/opts.py` & `masakari-9.1.3/masakari/conf/opts.py`

 * *Files identical despite different names*

### Comparing `masakari-9.1.2/masakari/conf/osapi_v1.py` & `masakari-9.1.3/masakari/conf/osapi_v1.py`

 * *Files identical despite different names*

### Comparing `masakari-9.1.2/masakari/conf/paths.py` & `masakari-9.1.3/masakari/conf/paths.py`

 * *Files identical despite different names*

### Comparing `masakari-9.1.2/masakari/conf/service.py` & `masakari-9.1.3/masakari/conf/service.py`

 * *Files identical despite different names*

### Comparing `masakari-9.1.2/masakari/conf/ssl.py` & `masakari-9.1.3/masakari/conf/ssl.py`

 * *Files identical despite different names*

### Comparing `masakari-9.1.2/masakari/conf/wsgi.py` & `masakari-9.1.3/masakari/conf/wsgi.py`

 * *Files identical despite different names*

### Comparing `masakari-9.1.2/masakari/config.py` & `masakari-9.1.3/masakari/config.py`

 * *Files identical despite different names*

### Comparing `masakari-9.1.2/masakari/context.py` & `masakari-9.1.3/masakari/context.py`

 * *Files identical despite different names*

### Comparing `masakari-9.1.2/masakari/db/__init__.py` & `masakari-9.1.3/masakari/db/__init__.py`

 * *Files identical despite different names*

### Comparing `masakari-9.1.2/masakari/db/api.py` & `masakari-9.1.3/masakari/db/api.py`

 * *Files identical despite different names*

### Comparing `masakari-9.1.2/masakari/db/migration.py` & `masakari-9.1.3/masakari/db/migration.py`

 * *Files identical despite different names*

### Comparing `masakari-9.1.2/masakari/db/sqlalchemy/api.py` & `masakari-9.1.3/masakari/db/sqlalchemy/api.py`

 * *Files identical despite different names*

### Comparing `masakari-9.1.2/masakari/db/sqlalchemy/migrate_repo/manage.py` & `masakari-9.1.3/masakari/db/sqlalchemy/migrate_repo/manage.py`

 * *Files identical despite different names*

### Comparing `masakari-9.1.2/masakari/db/sqlalchemy/migrate_repo/migrate.cfg` & `masakari-9.1.3/masakari/db/sqlalchemy/migrate_repo/migrate.cfg`

 * *Files identical despite different names*

### Comparing `masakari-9.1.2/masakari/db/sqlalchemy/migrate_repo/versions/001_add_failover_segments_table.py` & `masakari-9.1.3/masakari/db/sqlalchemy/migrate_repo/versions/001_add_failover_segments_table.py`

 * *Files identical despite different names*

### Comparing `masakari-9.1.2/masakari/db/sqlalchemy/migrate_repo/versions/002_add_hosts_table.py` & `masakari-9.1.3/masakari/db/sqlalchemy/migrate_repo/versions/002_add_hosts_table.py`

 * *Files identical despite different names*

### Comparing `masakari-9.1.2/masakari/db/sqlalchemy/migrate_repo/versions/003_update_unique_constraint_hosts.py` & `masakari-9.1.3/masakari/db/sqlalchemy/migrate_repo/versions/003_update_unique_constraint_hosts.py`

 * *Files identical despite different names*

### Comparing `masakari-9.1.2/masakari/db/sqlalchemy/migrate_repo/versions/004_add_notifications_table.py` & `masakari-9.1.3/masakari/db/sqlalchemy/migrate_repo/versions/004_add_notifications_table.py`

 * *Files identical despite different names*

### Comparing `masakari-9.1.2/masakari/db/sqlalchemy/migrate_repo/versions/005_remove_nullable_mismatch.py` & `masakari-9.1.3/masakari/db/sqlalchemy/migrate_repo/versions/005_remove_nullable_mismatch.py`

 * *Files identical despite different names*

### Comparing `masakari-9.1.2/masakari/db/sqlalchemy/migrate_repo/versions/006_add_persistence_tables.py` & `masakari-9.1.3/masakari/db/sqlalchemy/migrate_repo/versions/006_add_persistence_tables.py`

 * *Files identical despite different names*

### Comparing `masakari-9.1.2/masakari/db/sqlalchemy/migration.py` & `masakari-9.1.3/masakari/db/sqlalchemy/migration.py`

 * *Files identical despite different names*

### Comparing `masakari-9.1.2/masakari/db/sqlalchemy/models.py` & `masakari-9.1.3/masakari/db/sqlalchemy/models.py`

 * *Files identical despite different names*

### Comparing `masakari-9.1.2/masakari/engine/driver.py` & `masakari-9.1.3/masakari/engine/driver.py`

 * *Files identical despite different names*

### Comparing `masakari-9.1.2/masakari/engine/drivers/__init__.py` & `masakari-9.1.3/masakari/engine/drivers/__init__.py`

 * *Files identical despite different names*

### Comparing `masakari-9.1.2/masakari/engine/drivers/taskflow/__init__.py` & `masakari-9.1.3/masakari/engine/drivers/taskflow/__init__.py`

 * *Files identical despite different names*

### Comparing `masakari-9.1.2/masakari/engine/drivers/taskflow/base.py` & `masakari-9.1.3/masakari/engine/drivers/taskflow/base.py`

 * *Files identical despite different names*

### Comparing `masakari-9.1.2/masakari/engine/drivers/taskflow/driver.py` & `masakari-9.1.3/masakari/engine/drivers/taskflow/driver.py`

 * *Files identical despite different names*

### Comparing `masakari-9.1.2/masakari/engine/drivers/taskflow/host_failure.py` & `masakari-9.1.3/masakari/engine/drivers/taskflow/host_failure.py`

 * *Files identical despite different names*

### Comparing `masakari-9.1.2/masakari/engine/drivers/taskflow/instance_failure.py` & `masakari-9.1.3/masakari/engine/drivers/taskflow/instance_failure.py`

 * *Files identical despite different names*

### Comparing `masakari-9.1.2/masakari/engine/drivers/taskflow/no_op.py` & `masakari-9.1.3/masakari/engine/drivers/taskflow/no_op.py`

 * *Files identical despite different names*

### Comparing `masakari-9.1.2/masakari/engine/drivers/taskflow/process_failure.py` & `masakari-9.1.3/masakari/engine/drivers/taskflow/process_failure.py`

 * *Files identical despite different names*

### Comparing `masakari-9.1.2/masakari/engine/instance_events.py` & `masakari-9.1.3/masakari/engine/instance_events.py`

 * *Files identical despite different names*

### Comparing `masakari-9.1.2/masakari/engine/manager.py` & `masakari-9.1.3/masakari/engine/manager.py`

 * *Files identical despite different names*

### Comparing `masakari-9.1.2/masakari/engine/rpcapi.py` & `masakari-9.1.3/masakari/engine/rpcapi.py`

 * *Files identical despite different names*

### Comparing `masakari-9.1.2/masakari/engine/utils.py` & `masakari-9.1.3/masakari/engine/utils.py`

 * *Files identical despite different names*

### Comparing `masakari-9.1.2/masakari/exception.py` & `masakari-9.1.3/masakari/exception.py`

 * *Files 0% similar despite different names*

```diff
@@ -40,15 +40,15 @@
 
 
 CONF = masakari.conf.CONF
 
 
 class ConvertedException(webob.exc.WSGIHTTPException):
     def __init__(self, code, title="", explanation=""):
-        self.code = code
+        self.code = int(code)
         # There is a strict rule about constructing status line for HTTP:
         # '...Status-Line, consisting of the protocol version followed by a
         # numeric status code and its associated textual phrase, with each
         # element separated by SP characters'
         # (http://www.faqs.org/rfcs/rfc2616.html)
         # 'code' and 'title' can not be empty because they correspond
         # to numeric status code and its associated text
```

### Comparing `masakari-9.1.2/masakari/ha/api.py` & `masakari-9.1.3/masakari/ha/api.py`

 * *Files identical despite different names*

### Comparing `masakari-9.1.2/masakari/hacking/checks.py` & `masakari-9.1.3/masakari/hacking/checks.py`

 * *Files identical despite different names*

### Comparing `masakari-9.1.2/masakari/i18n.py` & `masakari-9.1.3/masakari/i18n.py`

 * *Files identical despite different names*

### Comparing `masakari-9.1.2/masakari/manager.py` & `masakari-9.1.3/masakari/manager.py`

 * *Files identical despite different names*

### Comparing `masakari-9.1.2/masakari/notifications/objects/base.py` & `masakari-9.1.3/masakari/notifications/objects/base.py`

 * *Files identical despite different names*

### Comparing `masakari-9.1.2/masakari/notifications/objects/exception.py` & `masakari-9.1.3/masakari/notifications/objects/exception.py`

 * *Files identical despite different names*

### Comparing `masakari-9.1.2/masakari/notifications/objects/notification.py` & `masakari-9.1.3/masakari/notifications/objects/notification.py`

 * *Files identical despite different names*

### Comparing `masakari-9.1.2/masakari/objects/__init__.py` & `masakari-9.1.3/masakari/objects/__init__.py`

 * *Files identical despite different names*

### Comparing `masakari-9.1.2/masakari/objects/base.py` & `masakari-9.1.3/masakari/objects/base.py`

 * *Files identical despite different names*

### Comparing `masakari-9.1.2/masakari/objects/fields.py` & `masakari-9.1.3/masakari/objects/fields.py`

 * *Files identical despite different names*

### Comparing `masakari-9.1.2/masakari/objects/host.py` & `masakari-9.1.3/masakari/objects/host.py`

 * *Files identical despite different names*

### Comparing `masakari-9.1.2/masakari/objects/notification.py` & `masakari-9.1.3/masakari/objects/notification.py`

 * *Files identical despite different names*

### Comparing `masakari-9.1.2/masakari/objects/segment.py` & `masakari-9.1.3/masakari/objects/segment.py`

 * *Files identical despite different names*

### Comparing `masakari-9.1.2/masakari/policies/__init__.py` & `masakari-9.1.3/masakari/policies/__init__.py`

 * *Files identical despite different names*

### Comparing `masakari-9.1.2/masakari/policies/base.py` & `masakari-9.1.3/masakari/policies/base.py`

 * *Files identical despite different names*

### Comparing `masakari-9.1.2/masakari/policies/extension_info.py` & `masakari-9.1.3/masakari/policies/extension_info.py`

 * *Files identical despite different names*

### Comparing `masakari-9.1.2/masakari/policies/hosts.py` & `masakari-9.1.3/masakari/policies/hosts.py`

 * *Files identical despite different names*

### Comparing `masakari-9.1.2/masakari/policies/notifications.py` & `masakari-9.1.3/masakari/policies/notifications.py`

 * *Files identical despite different names*

### Comparing `masakari-9.1.2/masakari/policies/segments.py` & `masakari-9.1.3/masakari/policies/segments.py`

 * *Files identical despite different names*

### Comparing `masakari-9.1.2/masakari/policies/versions.py` & `masakari-9.1.3/masakari/policies/versions.py`

 * *Files identical despite different names*

### Comparing `masakari-9.1.2/masakari/policy.py` & `masakari-9.1.3/masakari/policy.py`

 * *Files identical despite different names*

### Comparing `masakari-9.1.2/masakari/rpc.py` & `masakari-9.1.3/masakari/rpc.py`

 * *Files identical despite different names*

### Comparing `masakari-9.1.2/masakari/safe_utils.py` & `masakari-9.1.3/masakari/safe_utils.py`

 * *Files identical despite different names*

### Comparing `masakari-9.1.2/masakari/service.py` & `masakari-9.1.3/masakari/service.py`

 * *Files identical despite different names*

### Comparing `masakari-9.1.2/masakari/test.py` & `masakari-9.1.3/masakari/test.py`

 * *Files identical despite different names*

### Comparing `masakari-9.1.2/masakari/tests/base.py` & `masakari-9.1.3/masakari/tests/base.py`

 * *Files identical despite different names*

### Comparing `masakari-9.1.2/masakari/tests/fixtures.py` & `masakari-9.1.3/masakari/tests/fixtures.py`

 * *Files identical despite different names*

### Comparing `masakari-9.1.2/masakari/tests/functional/base.py` & `masakari-9.1.3/masakari/tests/functional/base.py`

 * *Files identical despite different names*

### Comparing `masakari-9.1.2/masakari/tests/functional/notification_base.py` & `masakari-9.1.3/masakari/tests/functional/notification_base.py`

 * *Files identical despite different names*

### Comparing `masakari-9.1.2/masakari/tests/functional/test_hosts.py` & `masakari-9.1.3/masakari/tests/functional/test_hosts.py`

 * *Files identical despite different names*

### Comparing `masakari-9.1.2/masakari/tests/functional/test_process_notifications.py` & `masakari-9.1.3/masakari/tests/functional/test_process_notifications.py`

 * *Files identical despite different names*

### Comparing `masakari-9.1.2/masakari/tests/functional/test_segments.py` & `masakari-9.1.3/masakari/tests/functional/test_segments.py`

 * *Files identical despite different names*

### Comparing `masakari-9.1.2/masakari/tests/functional/test_vm_notifications.py` & `masakari-9.1.3/masakari/tests/functional/test_vm_notifications.py`

 * *Files identical despite different names*

### Comparing `masakari-9.1.2/masakari/tests/json_ref.py` & `masakari-9.1.3/masakari/tests/json_ref.py`

 * *Files identical despite different names*

### Comparing `masakari-9.1.2/masakari/tests/unit/__init__.py` & `masakari-9.1.3/masakari/tests/unit/__init__.py`

 * *Files identical despite different names*

### Comparing `masakari-9.1.2/masakari/tests/unit/api/openstack/fakes.py` & `masakari-9.1.3/masakari/tests/unit/api/openstack/fakes.py`

 * *Files identical despite different names*

### Comparing `masakari-9.1.2/masakari/tests/unit/api/openstack/ha/test_extension_info.py` & `masakari-9.1.3/masakari/tests/unit/api/openstack/ha/test_extension_info.py`

 * *Files identical despite different names*

### Comparing `masakari-9.1.2/masakari/tests/unit/api/openstack/ha/test_hosts.py` & `masakari-9.1.3/masakari/tests/unit/api/openstack/ha/test_hosts.py`

 * *Files identical despite different names*

### Comparing `masakari-9.1.2/masakari/tests/unit/api/openstack/ha/test_notifications.py` & `masakari-9.1.3/masakari/tests/unit/api/openstack/ha/test_notifications.py`

 * *Files identical despite different names*

### Comparing `masakari-9.1.2/masakari/tests/unit/api/openstack/ha/test_segments.py` & `masakari-9.1.3/masakari/tests/unit/api/openstack/ha/test_segments.py`

 * *Files identical despite different names*

### Comparing `masakari-9.1.2/masakari/tests/unit/api/openstack/ha/test_versions.py` & `masakari-9.1.3/masakari/tests/unit/api/openstack/ha/test_versions.py`

 * *Files identical despite different names*

### Comparing `masakari-9.1.2/masakari/tests/unit/api/openstack/test_common.py` & `masakari-9.1.3/masakari/tests/unit/api/openstack/test_common.py`

 * *Files identical despite different names*

### Comparing `masakari-9.1.2/masakari/tests/unit/api/openstack/test_extensions.py` & `masakari-9.1.3/masakari/tests/unit/api/openstack/test_extensions.py`

 * *Files identical despite different names*

### Comparing `masakari-9.1.2/masakari/tests/unit/api/openstack/test_wsgi.py` & `masakari-9.1.3/masakari/tests/unit/api/openstack/test_wsgi.py`

 * *Files 0% similar despite different names*

```diff
@@ -251,16 +251,17 @@
         self.assertEqual(response.status_int, http.OK)
 
     def test_resource_call_with_method_post(self):
         class Controller(object):
             @extensions.expected_errors(http.BAD_REQUEST)
             def create(self, req, body):
                 if expected_body != body:
-                    msg = "The request body invalid"
-                    raise webob.exc.HTTPBadRequest(explanation=msg)
+                    raise exception.ConvertedException(
+                        code=http.BAD_REQUEST,
+                        explanation="The request body invalid")
                 return "success"
         # verify the method: POST
         app = fakes.TestRouter(Controller())
         req = webob.Request.blank('/tests', method="POST",
                                   content_type='application/json')
         req.body = b'{"body": {"key": "value"}}'
         expected_body = {'body': {
```

### Comparing `masakari-9.1.2/masakari/tests/unit/api/test_api_version_request.py` & `masakari-9.1.3/masakari/tests/unit/api/test_api_version_request.py`

 * *Files identical despite different names*

### Comparing `masakari-9.1.2/masakari/tests/unit/api/test_auth.py` & `masakari-9.1.3/masakari/tests/unit/api/test_auth.py`

 * *Files identical despite different names*

### Comparing `masakari-9.1.2/masakari/tests/unit/api/test_utils.py` & `masakari-9.1.3/masakari/tests/unit/api/test_utils.py`

 * *Files identical despite different names*

### Comparing `masakari-9.1.2/masakari/tests/unit/cmd/test_masakari_api.py` & `masakari-9.1.3/masakari/tests/unit/cmd/test_masakari_api.py`

 * *Files identical despite different names*

### Comparing `masakari-9.1.2/masakari/tests/unit/cmd/test_status.py` & `masakari-9.1.3/masakari/tests/unit/cmd/test_status.py`

 * *Files identical despite different names*

### Comparing `masakari-9.1.2/masakari/tests/unit/compute/test_nova.py` & `masakari-9.1.3/masakari/tests/unit/compute/test_nova.py`

 * *Files identical despite different names*

### Comparing `masakari-9.1.2/masakari/tests/unit/conf_fixture.py` & `masakari-9.1.3/masakari/tests/unit/conf_fixture.py`

 * *Files identical despite different names*

### Comparing `masakari-9.1.2/masakari/tests/unit/db/test_db_api.py` & `masakari-9.1.3/masakari/tests/unit/db/test_db_api.py`

 * *Files identical despite different names*

### Comparing `masakari-9.1.2/masakari/tests/unit/db/test_migrations.py` & `masakari-9.1.3/masakari/tests/unit/db/test_migrations.py`

 * *Files identical despite different names*

### Comparing `masakari-9.1.2/masakari/tests/unit/db/test_purge.py` & `masakari-9.1.3/masakari/tests/unit/db/test_purge.py`

 * *Files identical despite different names*

### Comparing `masakari-9.1.2/masakari/tests/unit/engine/drivers/taskflow/test_host_failure_flow.py` & `masakari-9.1.3/masakari/tests/unit/engine/drivers/taskflow/test_host_failure_flow.py`

 * *Files identical despite different names*

### Comparing `masakari-9.1.2/masakari/tests/unit/engine/drivers/taskflow/test_instance_failure_flow.py` & `masakari-9.1.3/masakari/tests/unit/engine/drivers/taskflow/test_instance_failure_flow.py`

 * *Files identical despite different names*

### Comparing `masakari-9.1.2/masakari/tests/unit/engine/drivers/taskflow/test_process_failure_flow.py` & `masakari-9.1.3/masakari/tests/unit/engine/drivers/taskflow/test_process_failure_flow.py`

 * *Files identical despite different names*

### Comparing `masakari-9.1.2/masakari/tests/unit/engine/drivers/taskflow/test_taskflow_driver.py` & `masakari-9.1.3/masakari/tests/unit/engine/drivers/taskflow/test_taskflow_driver.py`

 * *Files identical despite different names*

### Comparing `masakari-9.1.2/masakari/tests/unit/engine/fake_engine.py` & `masakari-9.1.3/masakari/tests/unit/engine/fake_engine.py`

 * *Files identical despite different names*

### Comparing `masakari-9.1.2/masakari/tests/unit/engine/test_engine_mgr.py` & `masakari-9.1.3/masakari/tests/unit/engine/test_engine_mgr.py`

 * *Files identical despite different names*

### Comparing `masakari-9.1.2/masakari/tests/unit/engine/test_rpcapi.py` & `masakari-9.1.3/masakari/tests/unit/engine/test_rpcapi.py`

 * *Files identical despite different names*

### Comparing `masakari-9.1.2/masakari/tests/unit/engine/test_utils.py` & `masakari-9.1.3/masakari/tests/unit/engine/test_utils.py`

 * *Files identical despite different names*

### Comparing `masakari-9.1.2/masakari/tests/unit/fake_notifier.py` & `masakari-9.1.3/masakari/tests/unit/fake_notifier.py`

 * *Files identical despite different names*

### Comparing `masakari-9.1.2/masakari/tests/unit/fake_policy.py` & `masakari-9.1.3/masakari/tests/unit/fake_policy.py`

 * *Files identical despite different names*

### Comparing `masakari-9.1.2/masakari/tests/unit/fakes.py` & `masakari-9.1.3/masakari/tests/unit/fakes.py`

 * *Files identical despite different names*

### Comparing `masakari-9.1.2/masakari/tests/unit/ha/test_api.py` & `masakari-9.1.3/masakari/tests/unit/ha/test_api.py`

 * *Files identical despite different names*

### Comparing `masakari-9.1.2/masakari/tests/unit/matchers.py` & `masakari-9.1.3/masakari/tests/unit/matchers.py`

 * *Files identical despite different names*

### Comparing `masakari-9.1.2/masakari/tests/unit/monkey_patch_example/__init__.py` & `masakari-9.1.3/masakari/tests/unit/monkey_patch_example/__init__.py`

 * *Files identical despite different names*

### Comparing `masakari-9.1.2/masakari/tests/unit/monkey_patch_example/example_a.py` & `masakari-9.1.3/masakari/tests/unit/monkey_patch_example/example_a.py`

 * *Files identical despite different names*

### Comparing `masakari-9.1.2/masakari/tests/unit/monkey_patch_example/example_b.py` & `masakari-9.1.3/masakari/tests/unit/monkey_patch_example/example_b.py`

 * *Files identical despite different names*

### Comparing `masakari-9.1.2/masakari/tests/unit/notifications/objects/test_notification.py` & `masakari-9.1.3/masakari/tests/unit/notifications/objects/test_notification.py`

 * *Files identical despite different names*

### Comparing `masakari-9.1.2/masakari/tests/unit/objects/fake_args.py` & `masakari-9.1.3/masakari/tests/unit/objects/fake_args.py`

 * *Files identical despite different names*

### Comparing `masakari-9.1.2/masakari/tests/unit/objects/test_fields.py` & `masakari-9.1.3/masakari/tests/unit/objects/test_fields.py`

 * *Files identical despite different names*

### Comparing `masakari-9.1.2/masakari/tests/unit/objects/test_hosts.py` & `masakari-9.1.3/masakari/tests/unit/objects/test_hosts.py`

 * *Files identical despite different names*

### Comparing `masakari-9.1.2/masakari/tests/unit/objects/test_notifications.py` & `masakari-9.1.3/masakari/tests/unit/objects/test_notifications.py`

 * *Files identical despite different names*

### Comparing `masakari-9.1.2/masakari/tests/unit/objects/test_objects.py` & `masakari-9.1.3/masakari/tests/unit/objects/test_objects.py`

 * *Files identical despite different names*

### Comparing `masakari-9.1.2/masakari/tests/unit/objects/test_segments.py` & `masakari-9.1.3/masakari/tests/unit/objects/test_segments.py`

 * *Files identical despite different names*

### Comparing `masakari-9.1.2/masakari/tests/unit/policy_fixture.py` & `masakari-9.1.3/masakari/tests/unit/policy_fixture.py`

 * *Files identical despite different names*

### Comparing `masakari-9.1.2/masakari/tests/unit/test_api_validation.py` & `masakari-9.1.3/masakari/tests/unit/test_api_validation.py`

 * *Files identical despite different names*

### Comparing `masakari-9.1.2/masakari/tests/unit/test_conf.py` & `masakari-9.1.3/masakari/tests/unit/test_conf.py`

 * *Files identical despite different names*

### Comparing `masakari-9.1.2/masakari/tests/unit/test_context.py` & `masakari-9.1.3/masakari/tests/unit/test_context.py`

 * *Files identical despite different names*

### Comparing `masakari-9.1.2/masakari/tests/unit/test_exception.py` & `masakari-9.1.3/masakari/tests/unit/test_exception.py`

 * *Files identical despite different names*

### Comparing `masakari-9.1.2/masakari/tests/unit/test_hacking.py` & `masakari-9.1.3/masakari/tests/unit/test_hacking.py`

 * *Files identical despite different names*

### Comparing `masakari-9.1.2/masakari/tests/unit/test_masakari_manage.py` & `masakari-9.1.3/masakari/tests/unit/test_masakari_manage.py`

 * *Files identical despite different names*

### Comparing `masakari-9.1.2/masakari/tests/unit/test_policy.py` & `masakari-9.1.3/masakari/tests/unit/test_policy.py`

 * *Files identical despite different names*

### Comparing `masakari-9.1.2/masakari/tests/unit/test_rpc.py` & `masakari-9.1.3/masakari/tests/unit/test_rpc.py`

 * *Files identical despite different names*

### Comparing `masakari-9.1.2/masakari/tests/unit/test_safeutils.py` & `masakari-9.1.3/masakari/tests/unit/test_safeutils.py`

 * *Files identical despite different names*

### Comparing `masakari-9.1.2/masakari/tests/unit/test_service.py` & `masakari-9.1.3/masakari/tests/unit/test_service.py`

 * *Files identical despite different names*

### Comparing `masakari-9.1.2/masakari/tests/unit/test_utils.py` & `masakari-9.1.3/masakari/tests/unit/test_utils.py`

 * *Files identical despite different names*

### Comparing `masakari-9.1.2/masakari/tests/unit/test_versions.py` & `masakari-9.1.3/masakari/tests/unit/test_versions.py`

 * *Files identical despite different names*

### Comparing `masakari-9.1.2/masakari/tests/unit/test_wsgi.py` & `masakari-9.1.3/masakari/tests/unit/test_wsgi.py`

 * *Files identical despite different names*

### Comparing `masakari-9.1.2/masakari/tests/unit/utils.py` & `masakari-9.1.3/masakari/tests/unit/utils.py`

 * *Files identical despite different names*

### Comparing `masakari-9.1.2/masakari/tests/uuidsentinel.py` & `masakari-9.1.3/masakari/tests/uuidsentinel.py`

 * *Files identical despite different names*

### Comparing `masakari-9.1.2/masakari/utils.py` & `masakari-9.1.3/masakari/utils.py`

 * *Files identical despite different names*

### Comparing `masakari-9.1.2/masakari/version.py` & `masakari-9.1.3/masakari/version.py`

 * *Files identical despite different names*

### Comparing `masakari-9.1.2/masakari/wsgi.py` & `masakari-9.1.3/masakari/wsgi.py`

 * *Files identical despite different names*

### Comparing `masakari-9.1.2/masakari.egg-info/PKG-INFO` & `masakari-9.1.3/masakari.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: masakari
-Version: 9.1.2
+Version: 9.1.3
 Summary: Virtual Machine High Availability (VMHA) service for OpenStack
 Home-page: https://docs.openstack.org/masakari/latest/
 Author: OpenStack
 Author-email: openstack-discuss@lists.openstack.org
 License: UNKNOWN
 Description: ========
         Masakari
```

### Comparing `masakari-9.1.2/masakari.egg-info/SOURCES.txt` & `masakari-9.1.3/masakari.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -326,14 +326,15 @@
 releasenotes/notes/bp-mutable-config-57efdd467c01aa7b.yaml
 releasenotes/notes/bug-1685145-3d93145bfc76c660.yaml
 releasenotes/notes/bug-1776385-0bcf0a0b3fad359e.yaml
 releasenotes/notes/bug-1782517-e4dc70bad9e4e131.yaml
 releasenotes/notes/bug-1856164-6601a6e6280eba4d.yaml
 releasenotes/notes/bug-1859406-6b041a26acf6c7f6.yaml
 releasenotes/notes/bug-1882516-e8dc7fd2b55f065f.yaml
+releasenotes/notes/bug-1932194-2b721860bbc26819.yaml
 releasenotes/notes/bug-add-missing-domain-name-5181c02f3f033a22.yaml
 releasenotes/notes/compute_search-3da97e69e661a73f.yaml
 releasenotes/notes/correct_response_code-df8b43a201efa1b4.yaml
 releasenotes/notes/db-purge-support-7a33e2ea5d2a624b.yaml
 releasenotes/notes/deprecate-topic-opt-af83f82143143c61.yaml
 releasenotes/notes/drop-py-2-7-059d3cd5e7cb4e1a.yaml
 releasenotes/notes/evacuation_in_threads-cc9c79b10acfb5f6.yaml
```

### Comparing `masakari-9.1.2/masakari.egg-info/entry_points.txt` & `masakari-9.1.3/masakari.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `masakari-9.1.2/masakari.egg-info/requires.txt` & `masakari-9.1.3/masakari.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `masakari-9.1.2/releasenotes/notes/add-periodic-tasks-0c96d6f620502a75.yaml` & `masakari-9.1.3/releasenotes/notes/add-periodic-tasks-0c96d6f620502a75.yaml`

 * *Files identical despite different names*

### Comparing `masakari-9.1.2/releasenotes/notes/add_evacuate_error_instances_conf_option-5b4d1906137395f0.yaml` & `masakari-9.1.3/releasenotes/notes/add_evacuate_error_instances_conf_option-5b4d1906137395f0.yaml`

 * *Files identical despite different names*

### Comparing `masakari-9.1.2/releasenotes/notes/add_ha_enabled_config_options-54a9270a5993d20a.yaml` & `masakari-9.1.3/releasenotes/notes/add_ha_enabled_config_options-54a9270a5993d20a.yaml`

 * *Files identical despite different names*

### Comparing `masakari-9.1.2/releasenotes/notes/auto_priority_and_rh_priority_recovery_methods-b88cc00041fa2c4d.yaml` & `masakari-9.1.3/releasenotes/notes/auto_priority_and_rh_priority_recovery_methods-b88cc00041fa2c4d.yaml`

 * *Files identical despite different names*

### Comparing `masakari-9.1.2/releasenotes/notes/correct_response_code-df8b43a201efa1b4.yaml` & `masakari-9.1.3/releasenotes/notes/correct_response_code-df8b43a201efa1b4.yaml`

 * *Files identical despite different names*

### Comparing `masakari-9.1.2/releasenotes/notes/evacuation_in_threads-cc9c79b10acfb5f6.yaml` & `masakari-9.1.3/releasenotes/notes/evacuation_in_threads-cc9c79b10acfb5f6.yaml`

 * *Files identical despite different names*

### Comparing `masakari-9.1.2/releasenotes/notes/host-apis-46a87fcd56d8ed30.yaml` & `masakari-9.1.3/releasenotes/notes/host-apis-46a87fcd56d8ed30.yaml`

 * *Files identical despite different names*

### Comparing `masakari-9.1.2/releasenotes/notes/notifications-in-masakari-f5d79838fc23cb9b.yaml` & `masakari-9.1.3/releasenotes/notes/notifications-in-masakari-f5d79838fc23cb9b.yaml`

 * *Files identical despite different names*

### Comparing `masakari-9.1.2/releasenotes/notes/policy-in-code-8740d51624055044.yaml` & `masakari-9.1.3/releasenotes/notes/policy-in-code-8740d51624055044.yaml`

 * *Files identical despite different names*

### Comparing `masakari-9.1.2/releasenotes/notes/progress-details-recovery-workflows-5b14b7b3f87374f4.yaml` & `masakari-9.1.3/releasenotes/notes/progress-details-recovery-workflows-5b14b7b3f87374f4.yaml`

 * *Files identical despite different names*

### Comparing `masakari-9.1.2/releasenotes/notes/recovery-method-customization-3438b0e26e322b88.yaml` & `masakari-9.1.3/releasenotes/notes/recovery-method-customization-3438b0e26e322b88.yaml`

 * *Files identical despite different names*

### Comparing `masakari-9.1.2/releasenotes/source/conf.py` & `masakari-9.1.3/releasenotes/source/conf.py`

 * *Files identical despite different names*

### Comparing `masakari-9.1.2/requirements.txt` & `masakari-9.1.3/requirements.txt`

 * *Files identical despite different names*

### Comparing `masakari-9.1.2/setup.cfg` & `masakari-9.1.3/setup.cfg`

 * *Files identical despite different names*

### Comparing `masakari-9.1.2/setup.py` & `masakari-9.1.3/setup.py`

 * *Files identical despite different names*

### Comparing `masakari-9.1.2/test-requirements.txt` & `masakari-9.1.3/test-requirements.txt`

 * *Files identical despite different names*

### Comparing `masakari-9.1.2/tox.ini` & `masakari-9.1.3/tox.ini`

 * *Files identical despite different names*

