# Comparing `tmp/masakari-monitors-9.0.2.tar.gz` & `tmp/masakari-monitors-9.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "masakari-monitors-9.0.2.tar", last modified: Tue Jul 27 11:55:12 2021, max compression
+gzip compressed data, was "masakari-monitors-9.0.3.tar", last modified: Mon Sep 20 15:26:45 2021, max compression
```

## Comparing `masakari-monitors-9.0.2.tar` & `masakari-monitors-9.0.3.tar`

### file list

```diff
@@ -1,173 +1,174 @@
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-07-27 11:55:12.982866 masakari-monitors-9.0.2/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       77 2021-07-27 11:54:27.000000 masakari-monitors-9.0.2/.coveragerc
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       89 2021-07-27 11:54:27.000000 masakari-monitors-9.0.2/.mailmap
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       62 2021-07-27 11:54:27.000000 masakari-monitors-9.0.2/.stestr.conf
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      161 2021-07-27 11:54:27.000000 masakari-monitors-9.0.2/.zuul.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1348 2021-07-27 11:55:12.000000 masakari-monitors-9.0.2/AUTHORS
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      661 2021-07-27 11:54:27.000000 masakari-monitors-9.0.2/CONTRIBUTING.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4750 2021-07-27 11:55:12.000000 masakari-monitors-9.0.2/ChangeLog
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      463 2021-07-27 11:54:27.000000 masakari-monitors-9.0.2/HACKING.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10143 2021-07-27 11:54:27.000000 masakari-monitors-9.0.2/LICENSE
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       94 2021-07-27 11:54:27.000000 masakari-monitors-9.0.2/MANIFEST.in
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3003 2021-07-27 11:55:12.982866 masakari-monitors-9.0.2/PKG-INFO
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1829 2021-07-27 11:54:27.000000 masakari-monitors-9.0.2/README.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       17 2021-07-27 11:54:27.000000 masakari-monitors-9.0.2/babel.cfg
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      301 2021-07-27 11:54:27.000000 masakari-monitors-9.0.2/bindep.txt
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-07-27 11:55:12.966866 masakari-monitors-9.0.2/doc/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      327 2021-07-27 11:54:27.000000 masakari-monitors-9.0.2/doc/requirements.txt
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-07-27 11:55:12.970866 masakari-monitors-9.0.2/doc/source/
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)     2519 2021-07-27 11:54:27.000000 masakari-monitors-9.0.2/doc/source/conf.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       75 2021-07-27 11:54:27.000000 masakari-monitors-9.0.2/doc/source/contributing.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      517 2021-07-27 11:54:27.000000 masakari-monitors-9.0.2/doc/source/index.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      220 2021-07-27 11:54:27.000000 masakari-monitors-9.0.2/doc/source/installation.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       30 2021-07-27 11:54:27.000000 masakari-monitors-9.0.2/doc/source/readme.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       94 2021-07-27 11:54:27.000000 masakari-monitors-9.0.2/doc/source/usage.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-07-27 11:55:12.962866 masakari-monitors-9.0.2/etc/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-07-27 11:55:12.970866 masakari-monitors-9.0.2/etc/masakarimonitors/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      144 2021-07-27 11:54:27.000000 masakari-monitors-9.0.2/etc/masakarimonitors/README-masakarimonitors.conf.txt
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)     1743 2021-07-27 11:54:27.000000 masakari-monitors-9.0.2/etc/masakarimonitors/hostmonitor.conf.sample
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      173 2021-07-27 11:54:27.000000 masakari-monitors-9.0.2/etc/masakarimonitors/masakarimonitors-config-generator.conf
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)      239 2021-07-27 11:54:27.000000 masakari-monitors-9.0.2/etc/masakarimonitors/proc.list.sample
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2188 2021-07-27 11:54:27.000000 masakari-monitors-9.0.2/etc/masakarimonitors/process_list.yaml.sample
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)      290 2021-07-27 11:54:27.000000 masakari-monitors-9.0.2/etc/masakarimonitors/processmonitor.conf.sample
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-07-27 11:55:12.970866 masakari-monitors-9.0.2/masakari_monitors.egg-info/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3003 2021-07-27 11:55:12.000000 masakari-monitors-9.0.2/masakari_monitors.egg-info/PKG-INFO
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5652 2021-07-27 11:55:12.000000 masakari-monitors-9.0.2/masakari_monitors.egg-info/SOURCES.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2021-07-27 11:55:12.000000 masakari-monitors-9.0.2/masakari_monitors.egg-info/dependency_links.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      960 2021-07-27 11:55:12.000000 masakari-monitors-9.0.2/masakari_monitors.egg-info/entry_points.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2021-07-27 11:55:12.000000 masakari-monitors-9.0.2/masakari_monitors.egg-info/not-zip-safe
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       46 2021-07-27 11:55:12.000000 masakari-monitors-9.0.2/masakari_monitors.egg-info/pbr.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      311 2021-07-27 11:55:12.000000 masakari-monitors-9.0.2/masakari_monitors.egg-info/requires.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       17 2021-07-27 11:55:12.000000 masakari-monitors-9.0.2/masakari_monitors.egg-info/top_level.txt
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-07-27 11:55:12.970866 masakari-monitors-9.0.2/masakarimonitors/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      673 2021-07-27 11:54:27.000000 masakari-monitors-9.0.2/masakarimonitors/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-07-27 11:55:12.974866 masakari-monitors-9.0.2/masakarimonitors/cmd/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-07-27 11:54:27.000000 masakari-monitors-9.0.2/masakarimonitors/cmd/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1117 2021-07-27 11:54:27.000000 masakari-monitors-9.0.2/masakarimonitors/cmd/hostmonitor.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1125 2021-07-27 11:54:27.000000 masakari-monitors-9.0.2/masakarimonitors/cmd/instancemonitor.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1136 2021-07-27 11:54:27.000000 masakari-monitors-9.0.2/masakarimonitors/cmd/introspectiveinstancemonitor.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1123 2021-07-27 11:54:27.000000 masakari-monitors-9.0.2/masakarimonitors/cmd/processmonitor.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-07-27 11:55:12.974866 masakari-monitors-9.0.2/masakarimonitors/common/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-07-27 11:54:27.000000 masakari-monitors-9.0.2/masakarimonitors/common/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      829 2021-07-27 11:54:27.000000 masakari-monitors-9.0.2/masakarimonitors/common/config.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-07-27 11:55:12.974866 masakari-monitors-9.0.2/masakarimonitors/conf/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1170 2021-07-27 11:54:27.000000 masakari-monitors-9.0.2/masakarimonitors/conf/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1636 2021-07-27 11:54:27.000000 masakari-monitors-9.0.2/masakarimonitors/conf/api.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1459 2021-07-27 11:54:27.000000 masakari-monitors-9.0.2/masakarimonitors/conf/base.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3578 2021-07-27 11:54:27.000000 masakari-monitors-9.0.2/masakarimonitors/conf/host.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1422 2021-07-27 11:54:27.000000 masakari-monitors-9.0.2/masakarimonitors/conf/instance.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2417 2021-07-27 11:54:27.000000 masakari-monitors-9.0.2/masakarimonitors/conf/introspectiveinstancemonitor.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3013 2021-07-27 11:54:27.000000 masakari-monitors-9.0.2/masakarimonitors/conf/opts.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1767 2021-07-27 11:54:27.000000 masakari-monitors-9.0.2/masakarimonitors/conf/process.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2064 2021-07-27 11:54:27.000000 masakari-monitors-9.0.2/masakarimonitors/conf/service.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1167 2021-07-27 11:54:27.000000 masakari-monitors-9.0.2/masakarimonitors/config.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-07-27 11:55:12.974866 masakari-monitors-9.0.2/masakarimonitors/ha/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-07-27 11:54:27.000000 masakari-monitors-9.0.2/masakarimonitors/ha/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3555 2021-07-27 11:54:27.000000 masakari-monitors-9.0.2/masakarimonitors/ha/masakari.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-07-27 11:55:12.974866 masakari-monitors-9.0.2/masakarimonitors/hacking/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-07-27 11:54:27.000000 masakari-monitors-9.0.2/masakarimonitors/hacking/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3613 2021-07-27 11:54:27.000000 masakari-monitors-9.0.2/masakarimonitors/hacking/checks.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-07-27 11:55:12.974866 masakari-monitors-9.0.2/masakarimonitors/hostmonitor/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-07-27 11:54:27.000000 masakari-monitors-9.0.2/masakarimonitors/hostmonitor/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2024 2021-07-27 11:54:27.000000 masakari-monitors-9.0.2/masakarimonitors/hostmonitor/host.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-07-27 11:55:12.974866 masakari-monitors-9.0.2/masakarimonitors/hostmonitor/host_handler/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-07-27 11:54:27.000000 masakari-monitors-9.0.2/masakarimonitors/hostmonitor/host_handler/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      926 2021-07-27 11:54:27.000000 masakari-monitors-9.0.2/masakarimonitors/hostmonitor/host_handler/driver.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    16102 2021-07-27 11:54:27.000000 masakari-monitors-9.0.2/masakarimonitors/hostmonitor/host_handler/handle_host.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1454 2021-07-27 11:54:27.000000 masakari-monitors-9.0.2/masakarimonitors/hostmonitor/host_handler/hold_host_status.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6372 2021-07-27 11:54:27.000000 masakari-monitors-9.0.2/masakarimonitors/hostmonitor/host_handler/parse_cib_xml.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2490 2021-07-27 11:54:27.000000 masakari-monitors-9.0.2/masakarimonitors/hostmonitor/host_handler/parse_crmmon_xml.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      943 2021-07-27 11:54:27.000000 masakari-monitors-9.0.2/masakarimonitors/i18n.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-07-27 11:55:12.974866 masakari-monitors-9.0.2/masakarimonitors/instancemonitor/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-07-27 11:54:27.000000 masakari-monitors-9.0.2/masakarimonitors/instancemonitor/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6902 2021-07-27 11:54:27.000000 masakari-monitors-9.0.2/masakarimonitors/instancemonitor/instance.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-07-27 11:55:12.974866 masakari-monitors-9.0.2/masakarimonitors/instancemonitor/libvirt_handler/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-07-27 11:54:27.000000 masakari-monitors-9.0.2/masakarimonitors/instancemonitor/libvirt_handler/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2949 2021-07-27 11:54:27.000000 masakari-monitors-9.0.2/masakarimonitors/instancemonitor/libvirt_handler/callback.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3003 2021-07-27 11:54:27.000000 masakari-monitors-9.0.2/masakarimonitors/instancemonitor/libvirt_handler/eventfilter.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4655 2021-07-27 11:54:27.000000 masakari-monitors-9.0.2/masakarimonitors/instancemonitor/libvirt_handler/eventfilter_table.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-07-27 11:55:12.978866 masakari-monitors-9.0.2/masakarimonitors/introspectiveinstancemonitor/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2695 2021-07-27 11:54:27.000000 masakari-monitors-9.0.2/masakarimonitors/introspectiveinstancemonitor/README.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-07-27 11:54:27.000000 masakari-monitors-9.0.2/masakarimonitors/introspectiveinstancemonitor/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5108 2021-07-27 11:54:27.000000 masakari-monitors-9.0.2/masakarimonitors/introspectiveinstancemonitor/cache.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6180 2021-07-27 11:54:27.000000 masakari-monitors-9.0.2/masakarimonitors/introspectiveinstancemonitor/instance.py
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)    13991 2021-07-27 11:54:27.000000 masakari-monitors-9.0.2/masakarimonitors/introspectiveinstancemonitor/qemu_utils.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3187 2021-07-27 11:54:27.000000 masakari-monitors-9.0.2/masakarimonitors/introspectiveinstancemonitor/scheduler.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3556 2021-07-27 11:54:27.000000 masakari-monitors-9.0.2/masakarimonitors/manager.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-07-27 11:55:12.978866 masakari-monitors-9.0.2/masakarimonitors/objects/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-07-27 11:54:27.000000 masakari-monitors-9.0.2/masakarimonitors/objects/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1046 2021-07-27 11:54:27.000000 masakari-monitors-9.0.2/masakarimonitors/objects/event_constants.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      884 2021-07-27 11:54:27.000000 masakari-monitors-9.0.2/masakarimonitors/privsep.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-07-27 11:55:12.978866 masakari-monitors-9.0.2/masakarimonitors/processmonitor/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-07-27 11:54:27.000000 masakari-monitors-9.0.2/masakarimonitors/processmonitor/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3226 2021-07-27 11:54:27.000000 masakari-monitors-9.0.2/masakarimonitors/processmonitor/process.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-07-27 11:55:12.978866 masakari-monitors-9.0.2/masakarimonitors/processmonitor/process_handler/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-07-27 11:54:27.000000 masakari-monitors-9.0.2/masakarimonitors/processmonitor/process_handler/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7555 2021-07-27 11:54:27.000000 masakari-monitors-9.0.2/masakarimonitors/processmonitor/process_handler/handle_process.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-07-27 11:54:27.000000 masakari-monitors-9.0.2/masakarimonitors/processmonitor/typescript
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4017 2021-07-27 11:54:27.000000 masakari-monitors-9.0.2/masakarimonitors/service.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-07-27 11:55:12.978866 masakari-monitors-9.0.2/masakarimonitors/tests/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-07-27 11:54:27.000000 masakari-monitors-9.0.2/masakarimonitors/tests/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      769 2021-07-27 11:54:27.000000 masakari-monitors-9.0.2/masakarimonitors/tests/base.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      779 2021-07-27 11:54:27.000000 masakari-monitors-9.0.2/masakarimonitors/tests/test_masakarimonitors.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-07-27 11:55:12.978866 masakari-monitors-9.0.2/masakarimonitors/tests/unit/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-07-27 11:54:27.000000 masakari-monitors-9.0.2/masakarimonitors/tests/unit/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-07-27 11:55:12.978866 masakari-monitors-9.0.2/masakarimonitors/tests/unit/ha/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-07-27 11:54:27.000000 masakari-monitors-9.0.2/masakarimonitors/tests/unit/ha/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6295 2021-07-27 11:54:27.000000 masakari-monitors-9.0.2/masakarimonitors/tests/unit/ha/test_masakari.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-07-27 11:55:12.978866 masakari-monitors-9.0.2/masakarimonitors/tests/unit/hostmonitor/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-07-27 11:54:27.000000 masakari-monitors-9.0.2/masakarimonitors/tests/unit/hostmonitor/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-07-27 11:55:12.978866 masakari-monitors-9.0.2/masakarimonitors/tests/unit/hostmonitor/host_handler/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-07-27 11:54:27.000000 masakari-monitors-9.0.2/masakarimonitors/tests/unit/hostmonitor/host_handler/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    36023 2021-07-27 11:54:27.000000 masakari-monitors-9.0.2/masakarimonitors/tests/unit/hostmonitor/host_handler/test_handle_host.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1506 2021-07-27 11:54:27.000000 masakari-monitors-9.0.2/masakarimonitors/tests/unit/hostmonitor/host_handler/test_hold_host_status.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5960 2021-07-27 11:54:27.000000 masakari-monitors-9.0.2/masakarimonitors/tests/unit/hostmonitor/host_handler/test_parse_cib_xml.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2725 2021-07-27 11:54:27.000000 masakari-monitors-9.0.2/masakarimonitors/tests/unit/hostmonitor/host_handler/test_parse_crmmon_xml.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3766 2021-07-27 11:54:27.000000 masakari-monitors-9.0.2/masakarimonitors/tests/unit/hostmonitor/test_host.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-07-27 11:55:12.978866 masakari-monitors-9.0.2/masakarimonitors/tests/unit/instancemonitor/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-07-27 11:54:27.000000 masakari-monitors-9.0.2/masakarimonitors/tests/unit/instancemonitor/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-07-27 11:55:12.978866 masakari-monitors-9.0.2/masakarimonitors/tests/unit/instancemonitor/libvirt_handler/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-07-27 11:54:27.000000 masakari-monitors-9.0.2/masakarimonitors/tests/unit/instancemonitor/libvirt_handler/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2122 2021-07-27 11:54:27.000000 masakari-monitors-9.0.2/masakarimonitors/tests/unit/instancemonitor/libvirt_handler/test_callback.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5841 2021-07-27 11:54:27.000000 masakari-monitors-9.0.2/masakarimonitors/tests/unit/instancemonitor/libvirt_handler/test_eventfilter.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9859 2021-07-27 11:54:27.000000 masakari-monitors-9.0.2/masakarimonitors/tests/unit/instancemonitor/test_instance.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-07-27 11:55:12.978866 masakari-monitors-9.0.2/masakarimonitors/tests/unit/introspectiveinstancemonitor/
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-07-27 11:54:27.000000 masakari-monitors-9.0.2/masakarimonitors/tests/unit/introspectiveinstancemonitor/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1400 2021-07-27 11:54:27.000000 masakari-monitors-9.0.2/masakarimonitors/tests/unit/introspectiveinstancemonitor/test_monitor_manager.py
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)     4029 2021-07-27 11:54:27.000000 masakari-monitors-9.0.2/masakarimonitors/tests/unit/introspectiveinstancemonitor/test_qemu_utils.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-07-27 11:55:12.982866 masakari-monitors-9.0.2/masakarimonitors/tests/unit/processmonitor/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-07-27 11:54:27.000000 masakari-monitors-9.0.2/masakarimonitors/tests/unit/processmonitor/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-07-27 11:55:12.982866 masakari-monitors-9.0.2/masakarimonitors/tests/unit/processmonitor/process_handler/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-07-27 11:54:27.000000 masakari-monitors-9.0.2/masakarimonitors/tests/unit/processmonitor/process_handler/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    15151 2021-07-27 11:54:27.000000 masakari-monitors-9.0.2/masakarimonitors/tests/unit/processmonitor/process_handler/test_handle_process.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6440 2021-07-27 11:54:27.000000 masakari-monitors-9.0.2/masakarimonitors/tests/unit/processmonitor/test_process.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6404 2021-07-27 11:54:27.000000 masakari-monitors-9.0.2/masakarimonitors/tests/unit/test_hacking.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4659 2021-07-27 11:54:27.000000 masakari-monitors-9.0.2/masakarimonitors/utils.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2447 2021-07-27 11:54:27.000000 masakari-monitors-9.0.2/masakarimonitors/version.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-07-27 11:55:12.966866 masakari-monitors-9.0.2/releasenotes/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-07-27 11:55:12.982866 masakari-monitors-9.0.2/releasenotes/notes/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-07-27 11:54:27.000000 masakari-monitors-9.0.2/releasenotes/notes/.placeholder
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      429 2021-07-27 11:54:27.000000 masakari-monitors-9.0.2/releasenotes/notes/bug-1866660-ef8624f5283b2e5e.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      137 2021-07-27 11:54:27.000000 masakari-monitors-9.0.2/releasenotes/notes/bug-1930361-fa8ce8e9781ea967.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      224 2021-07-27 11:54:27.000000 masakari-monitors-9.0.2/releasenotes/notes/drop-py-2-7-b28de816eac45468.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      177 2021-07-27 11:54:27.000000 masakari-monitors-9.0.2/releasenotes/notes/introspectiveinstancemonitor-f4bc71f029b61d49.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      320 2021-07-27 11:54:27.000000 masakari-monitors-9.0.2/releasenotes/notes/pythonize-monitors-081e74dfaf78fe99.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-07-27 11:55:12.982866 masakari-monitors-9.0.2/releasenotes/source/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-07-27 11:55:12.982866 masakari-monitors-9.0.2/releasenotes/source/_static/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-07-27 11:54:27.000000 masakari-monitors-9.0.2/releasenotes/source/_static/.placeholder
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-07-27 11:55:12.982866 masakari-monitors-9.0.2/releasenotes/source/_templates/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-07-27 11:54:27.000000 masakari-monitors-9.0.2/releasenotes/source/_templates/.placeholder
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9245 2021-07-27 11:54:27.000000 masakari-monitors-9.0.2/releasenotes/source/conf.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      232 2021-07-27 11:54:27.000000 masakari-monitors-9.0.2/releasenotes/source/index.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      137 2021-07-27 11:54:27.000000 masakari-monitors-9.0.2/releasenotes/source/ocata.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      133 2021-07-27 11:54:27.000000 masakari-monitors-9.0.2/releasenotes/source/pike.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      141 2021-07-27 11:54:27.000000 masakari-monitors-9.0.2/releasenotes/source/queens.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      145 2021-07-27 11:54:27.000000 masakari-monitors-9.0.2/releasenotes/source/rocky.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      145 2021-07-27 11:54:27.000000 masakari-monitors-9.0.2/releasenotes/source/stein.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      126 2021-07-27 11:54:27.000000 masakari-monitors-9.0.2/releasenotes/source/train.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      112 2021-07-27 11:54:27.000000 masakari-monitors-9.0.2/releasenotes/source/unreleased.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      703 2021-07-27 11:54:27.000000 masakari-monitors-9.0.2/requirements.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2226 2021-07-27 11:55:12.986866 masakari-monitors-9.0.2/setup.cfg
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1030 2021-07-27 11:54:27.000000 masakari-monitors-9.0.2/setup.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      582 2021-07-27 11:54:27.000000 masakari-monitors-9.0.2/test-requirements.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3187 2021-07-27 11:54:27.000000 masakari-monitors-9.0.2/tox.ini
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-09-20 15:26:45.481691 masakari-monitors-9.0.3/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       77 2021-09-20 15:26:10.000000 masakari-monitors-9.0.3/.coveragerc
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       89 2021-09-20 15:26:10.000000 masakari-monitors-9.0.3/.mailmap
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       62 2021-09-20 15:26:10.000000 masakari-monitors-9.0.3/.stestr.conf
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      161 2021-09-20 15:26:10.000000 masakari-monitors-9.0.3/.zuul.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1348 2021-09-20 15:26:45.000000 masakari-monitors-9.0.3/AUTHORS
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      661 2021-09-20 15:26:10.000000 masakari-monitors-9.0.3/CONTRIBUTING.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4800 2021-09-20 15:26:45.000000 masakari-monitors-9.0.3/ChangeLog
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      463 2021-09-20 15:26:10.000000 masakari-monitors-9.0.3/HACKING.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10143 2021-09-20 15:26:10.000000 masakari-monitors-9.0.3/LICENSE
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       94 2021-09-20 15:26:10.000000 masakari-monitors-9.0.3/MANIFEST.in
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3003 2021-09-20 15:26:45.481691 masakari-monitors-9.0.3/PKG-INFO
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1829 2021-09-20 15:26:10.000000 masakari-monitors-9.0.3/README.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       17 2021-09-20 15:26:10.000000 masakari-monitors-9.0.3/babel.cfg
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      301 2021-09-20 15:26:10.000000 masakari-monitors-9.0.3/bindep.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-09-20 15:26:45.429691 masakari-monitors-9.0.3/doc/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      327 2021-09-20 15:26:10.000000 masakari-monitors-9.0.3/doc/requirements.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-09-20 15:26:45.433691 masakari-monitors-9.0.3/doc/source/
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)     2519 2021-09-20 15:26:10.000000 masakari-monitors-9.0.3/doc/source/conf.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       75 2021-09-20 15:26:10.000000 masakari-monitors-9.0.3/doc/source/contributing.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      517 2021-09-20 15:26:10.000000 masakari-monitors-9.0.3/doc/source/index.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      220 2021-09-20 15:26:10.000000 masakari-monitors-9.0.3/doc/source/installation.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       30 2021-09-20 15:26:10.000000 masakari-monitors-9.0.3/doc/source/readme.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       94 2021-09-20 15:26:10.000000 masakari-monitors-9.0.3/doc/source/usage.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-09-20 15:26:45.417691 masakari-monitors-9.0.3/etc/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-09-20 15:26:45.433691 masakari-monitors-9.0.3/etc/masakarimonitors/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      144 2021-09-20 15:26:10.000000 masakari-monitors-9.0.3/etc/masakarimonitors/README-masakarimonitors.conf.txt
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)     1743 2021-09-20 15:26:10.000000 masakari-monitors-9.0.3/etc/masakarimonitors/hostmonitor.conf.sample
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      173 2021-09-20 15:26:10.000000 masakari-monitors-9.0.3/etc/masakarimonitors/masakarimonitors-config-generator.conf
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)      239 2021-09-20 15:26:10.000000 masakari-monitors-9.0.3/etc/masakarimonitors/proc.list.sample
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2188 2021-09-20 15:26:10.000000 masakari-monitors-9.0.3/etc/masakarimonitors/process_list.yaml.sample
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)      290 2021-09-20 15:26:10.000000 masakari-monitors-9.0.3/etc/masakarimonitors/processmonitor.conf.sample
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-09-20 15:26:45.437691 masakari-monitors-9.0.3/masakari_monitors.egg-info/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3003 2021-09-20 15:26:45.000000 masakari-monitors-9.0.3/masakari_monitors.egg-info/PKG-INFO
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5705 2021-09-20 15:26:45.000000 masakari-monitors-9.0.3/masakari_monitors.egg-info/SOURCES.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2021-09-20 15:26:45.000000 masakari-monitors-9.0.3/masakari_monitors.egg-info/dependency_links.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      960 2021-09-20 15:26:45.000000 masakari-monitors-9.0.3/masakari_monitors.egg-info/entry_points.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2021-09-20 15:26:45.000000 masakari-monitors-9.0.3/masakari_monitors.egg-info/not-zip-safe
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       46 2021-09-20 15:26:45.000000 masakari-monitors-9.0.3/masakari_monitors.egg-info/pbr.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      311 2021-09-20 15:26:45.000000 masakari-monitors-9.0.3/masakari_monitors.egg-info/requires.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       17 2021-09-20 15:26:45.000000 masakari-monitors-9.0.3/masakari_monitors.egg-info/top_level.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-09-20 15:26:45.441691 masakari-monitors-9.0.3/masakarimonitors/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      673 2021-09-20 15:26:10.000000 masakari-monitors-9.0.3/masakarimonitors/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-09-20 15:26:45.441691 masakari-monitors-9.0.3/masakarimonitors/cmd/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-09-20 15:26:10.000000 masakari-monitors-9.0.3/masakarimonitors/cmd/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1117 2021-09-20 15:26:10.000000 masakari-monitors-9.0.3/masakarimonitors/cmd/hostmonitor.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1125 2021-09-20 15:26:10.000000 masakari-monitors-9.0.3/masakarimonitors/cmd/instancemonitor.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1136 2021-09-20 15:26:10.000000 masakari-monitors-9.0.3/masakarimonitors/cmd/introspectiveinstancemonitor.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1123 2021-09-20 15:26:10.000000 masakari-monitors-9.0.3/masakarimonitors/cmd/processmonitor.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-09-20 15:26:45.441691 masakari-monitors-9.0.3/masakarimonitors/common/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-09-20 15:26:10.000000 masakari-monitors-9.0.3/masakarimonitors/common/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      829 2021-09-20 15:26:10.000000 masakari-monitors-9.0.3/masakarimonitors/common/config.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-09-20 15:26:45.445691 masakari-monitors-9.0.3/masakarimonitors/conf/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1170 2021-09-20 15:26:10.000000 masakari-monitors-9.0.3/masakarimonitors/conf/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1636 2021-09-20 15:26:10.000000 masakari-monitors-9.0.3/masakarimonitors/conf/api.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1459 2021-09-20 15:26:10.000000 masakari-monitors-9.0.3/masakarimonitors/conf/base.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3578 2021-09-20 15:26:10.000000 masakari-monitors-9.0.3/masakarimonitors/conf/host.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1422 2021-09-20 15:26:10.000000 masakari-monitors-9.0.3/masakarimonitors/conf/instance.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2417 2021-09-20 15:26:10.000000 masakari-monitors-9.0.3/masakarimonitors/conf/introspectiveinstancemonitor.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3013 2021-09-20 15:26:10.000000 masakari-monitors-9.0.3/masakarimonitors/conf/opts.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1767 2021-09-20 15:26:10.000000 masakari-monitors-9.0.3/masakarimonitors/conf/process.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2064 2021-09-20 15:26:10.000000 masakari-monitors-9.0.3/masakarimonitors/conf/service.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1167 2021-09-20 15:26:10.000000 masakari-monitors-9.0.3/masakarimonitors/config.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-09-20 15:26:45.445691 masakari-monitors-9.0.3/masakarimonitors/ha/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-09-20 15:26:10.000000 masakari-monitors-9.0.3/masakarimonitors/ha/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3555 2021-09-20 15:26:10.000000 masakari-monitors-9.0.3/masakarimonitors/ha/masakari.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-09-20 15:26:45.445691 masakari-monitors-9.0.3/masakarimonitors/hacking/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-09-20 15:26:10.000000 masakari-monitors-9.0.3/masakarimonitors/hacking/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3613 2021-09-20 15:26:10.000000 masakari-monitors-9.0.3/masakarimonitors/hacking/checks.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-09-20 15:26:45.445691 masakari-monitors-9.0.3/masakarimonitors/hostmonitor/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-09-20 15:26:10.000000 masakari-monitors-9.0.3/masakarimonitors/hostmonitor/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2024 2021-09-20 15:26:10.000000 masakari-monitors-9.0.3/masakarimonitors/hostmonitor/host.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-09-20 15:26:45.449691 masakari-monitors-9.0.3/masakarimonitors/hostmonitor/host_handler/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-09-20 15:26:10.000000 masakari-monitors-9.0.3/masakarimonitors/hostmonitor/host_handler/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      926 2021-09-20 15:26:10.000000 masakari-monitors-9.0.3/masakarimonitors/hostmonitor/host_handler/driver.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    16334 2021-09-20 15:26:10.000000 masakari-monitors-9.0.3/masakarimonitors/hostmonitor/host_handler/handle_host.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1454 2021-09-20 15:26:10.000000 masakari-monitors-9.0.3/masakarimonitors/hostmonitor/host_handler/hold_host_status.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6372 2021-09-20 15:26:10.000000 masakari-monitors-9.0.3/masakarimonitors/hostmonitor/host_handler/parse_cib_xml.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3137 2021-09-20 15:26:10.000000 masakari-monitors-9.0.3/masakarimonitors/hostmonitor/host_handler/parse_crmmon_xml.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      943 2021-09-20 15:26:10.000000 masakari-monitors-9.0.3/masakarimonitors/i18n.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-09-20 15:26:45.449691 masakari-monitors-9.0.3/masakarimonitors/instancemonitor/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-09-20 15:26:10.000000 masakari-monitors-9.0.3/masakarimonitors/instancemonitor/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6902 2021-09-20 15:26:10.000000 masakari-monitors-9.0.3/masakarimonitors/instancemonitor/instance.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-09-20 15:26:45.449691 masakari-monitors-9.0.3/masakarimonitors/instancemonitor/libvirt_handler/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-09-20 15:26:10.000000 masakari-monitors-9.0.3/masakarimonitors/instancemonitor/libvirt_handler/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2949 2021-09-20 15:26:10.000000 masakari-monitors-9.0.3/masakarimonitors/instancemonitor/libvirt_handler/callback.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3003 2021-09-20 15:26:10.000000 masakari-monitors-9.0.3/masakarimonitors/instancemonitor/libvirt_handler/eventfilter.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4655 2021-09-20 15:26:10.000000 masakari-monitors-9.0.3/masakarimonitors/instancemonitor/libvirt_handler/eventfilter_table.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-09-20 15:26:45.453691 masakari-monitors-9.0.3/masakarimonitors/introspectiveinstancemonitor/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2695 2021-09-20 15:26:10.000000 masakari-monitors-9.0.3/masakarimonitors/introspectiveinstancemonitor/README.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-09-20 15:26:10.000000 masakari-monitors-9.0.3/masakarimonitors/introspectiveinstancemonitor/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5108 2021-09-20 15:26:10.000000 masakari-monitors-9.0.3/masakarimonitors/introspectiveinstancemonitor/cache.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6180 2021-09-20 15:26:10.000000 masakari-monitors-9.0.3/masakarimonitors/introspectiveinstancemonitor/instance.py
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)    13991 2021-09-20 15:26:10.000000 masakari-monitors-9.0.3/masakarimonitors/introspectiveinstancemonitor/qemu_utils.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3187 2021-09-20 15:26:10.000000 masakari-monitors-9.0.3/masakarimonitors/introspectiveinstancemonitor/scheduler.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3556 2021-09-20 15:26:10.000000 masakari-monitors-9.0.3/masakarimonitors/manager.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-09-20 15:26:45.453691 masakari-monitors-9.0.3/masakarimonitors/objects/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-09-20 15:26:10.000000 masakari-monitors-9.0.3/masakarimonitors/objects/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1046 2021-09-20 15:26:10.000000 masakari-monitors-9.0.3/masakarimonitors/objects/event_constants.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      884 2021-09-20 15:26:10.000000 masakari-monitors-9.0.3/masakarimonitors/privsep.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-09-20 15:26:45.453691 masakari-monitors-9.0.3/masakarimonitors/processmonitor/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-09-20 15:26:10.000000 masakari-monitors-9.0.3/masakarimonitors/processmonitor/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3226 2021-09-20 15:26:10.000000 masakari-monitors-9.0.3/masakarimonitors/processmonitor/process.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-09-20 15:26:45.453691 masakari-monitors-9.0.3/masakarimonitors/processmonitor/process_handler/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-09-20 15:26:10.000000 masakari-monitors-9.0.3/masakarimonitors/processmonitor/process_handler/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7555 2021-09-20 15:26:10.000000 masakari-monitors-9.0.3/masakarimonitors/processmonitor/process_handler/handle_process.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-09-20 15:26:10.000000 masakari-monitors-9.0.3/masakarimonitors/processmonitor/typescript
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4017 2021-09-20 15:26:10.000000 masakari-monitors-9.0.3/masakarimonitors/service.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-09-20 15:26:45.453691 masakari-monitors-9.0.3/masakarimonitors/tests/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-09-20 15:26:10.000000 masakari-monitors-9.0.3/masakarimonitors/tests/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      769 2021-09-20 15:26:10.000000 masakari-monitors-9.0.3/masakarimonitors/tests/base.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      779 2021-09-20 15:26:10.000000 masakari-monitors-9.0.3/masakarimonitors/tests/test_masakarimonitors.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-09-20 15:26:45.457691 masakari-monitors-9.0.3/masakarimonitors/tests/unit/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-09-20 15:26:10.000000 masakari-monitors-9.0.3/masakarimonitors/tests/unit/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-09-20 15:26:45.457691 masakari-monitors-9.0.3/masakarimonitors/tests/unit/ha/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-09-20 15:26:10.000000 masakari-monitors-9.0.3/masakarimonitors/tests/unit/ha/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6295 2021-09-20 15:26:10.000000 masakari-monitors-9.0.3/masakarimonitors/tests/unit/ha/test_masakari.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-09-20 15:26:45.457691 masakari-monitors-9.0.3/masakarimonitors/tests/unit/hostmonitor/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-09-20 15:26:10.000000 masakari-monitors-9.0.3/masakarimonitors/tests/unit/hostmonitor/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-09-20 15:26:45.457691 masakari-monitors-9.0.3/masakarimonitors/tests/unit/hostmonitor/host_handler/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-09-20 15:26:10.000000 masakari-monitors-9.0.3/masakarimonitors/tests/unit/hostmonitor/host_handler/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    36710 2021-09-20 15:26:10.000000 masakari-monitors-9.0.3/masakarimonitors/tests/unit/hostmonitor/host_handler/test_handle_host.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1506 2021-09-20 15:26:10.000000 masakari-monitors-9.0.3/masakarimonitors/tests/unit/hostmonitor/host_handler/test_hold_host_status.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5960 2021-09-20 15:26:10.000000 masakari-monitors-9.0.3/masakarimonitors/tests/unit/hostmonitor/host_handler/test_parse_cib_xml.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3531 2021-09-20 15:26:10.000000 masakari-monitors-9.0.3/masakarimonitors/tests/unit/hostmonitor/host_handler/test_parse_crmmon_xml.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3766 2021-09-20 15:26:10.000000 masakari-monitors-9.0.3/masakarimonitors/tests/unit/hostmonitor/test_host.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-09-20 15:26:45.461691 masakari-monitors-9.0.3/masakarimonitors/tests/unit/instancemonitor/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-09-20 15:26:10.000000 masakari-monitors-9.0.3/masakarimonitors/tests/unit/instancemonitor/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-09-20 15:26:45.473691 masakari-monitors-9.0.3/masakarimonitors/tests/unit/instancemonitor/libvirt_handler/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-09-20 15:26:10.000000 masakari-monitors-9.0.3/masakarimonitors/tests/unit/instancemonitor/libvirt_handler/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2122 2021-09-20 15:26:10.000000 masakari-monitors-9.0.3/masakarimonitors/tests/unit/instancemonitor/libvirt_handler/test_callback.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5841 2021-09-20 15:26:10.000000 masakari-monitors-9.0.3/masakarimonitors/tests/unit/instancemonitor/libvirt_handler/test_eventfilter.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9859 2021-09-20 15:26:10.000000 masakari-monitors-9.0.3/masakarimonitors/tests/unit/instancemonitor/test_instance.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-09-20 15:26:45.473691 masakari-monitors-9.0.3/masakarimonitors/tests/unit/introspectiveinstancemonitor/
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-09-20 15:26:10.000000 masakari-monitors-9.0.3/masakarimonitors/tests/unit/introspectiveinstancemonitor/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1400 2021-09-20 15:26:10.000000 masakari-monitors-9.0.3/masakarimonitors/tests/unit/introspectiveinstancemonitor/test_monitor_manager.py
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)     4029 2021-09-20 15:26:10.000000 masakari-monitors-9.0.3/masakarimonitors/tests/unit/introspectiveinstancemonitor/test_qemu_utils.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-09-20 15:26:45.473691 masakari-monitors-9.0.3/masakarimonitors/tests/unit/processmonitor/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-09-20 15:26:10.000000 masakari-monitors-9.0.3/masakarimonitors/tests/unit/processmonitor/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-09-20 15:26:45.473691 masakari-monitors-9.0.3/masakarimonitors/tests/unit/processmonitor/process_handler/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-09-20 15:26:10.000000 masakari-monitors-9.0.3/masakarimonitors/tests/unit/processmonitor/process_handler/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    15151 2021-09-20 15:26:10.000000 masakari-monitors-9.0.3/masakarimonitors/tests/unit/processmonitor/process_handler/test_handle_process.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6440 2021-09-20 15:26:10.000000 masakari-monitors-9.0.3/masakarimonitors/tests/unit/processmonitor/test_process.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6404 2021-09-20 15:26:10.000000 masakari-monitors-9.0.3/masakarimonitors/tests/unit/test_hacking.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4659 2021-09-20 15:26:10.000000 masakari-monitors-9.0.3/masakarimonitors/utils.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2447 2021-09-20 15:26:10.000000 masakari-monitors-9.0.3/masakarimonitors/version.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-09-20 15:26:45.425691 masakari-monitors-9.0.3/releasenotes/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-09-20 15:26:45.477691 masakari-monitors-9.0.3/releasenotes/notes/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-09-20 15:26:10.000000 masakari-monitors-9.0.3/releasenotes/notes/.placeholder
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      429 2021-09-20 15:26:10.000000 masakari-monitors-9.0.3/releasenotes/notes/bug-1866660-ef8624f5283b2e5e.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      241 2021-09-20 15:26:10.000000 masakari-monitors-9.0.3/releasenotes/notes/bug-1878548-5fab31aec6ba5407.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      137 2021-09-20 15:26:10.000000 masakari-monitors-9.0.3/releasenotes/notes/bug-1930361-fa8ce8e9781ea967.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      224 2021-09-20 15:26:10.000000 masakari-monitors-9.0.3/releasenotes/notes/drop-py-2-7-b28de816eac45468.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      177 2021-09-20 15:26:10.000000 masakari-monitors-9.0.3/releasenotes/notes/introspectiveinstancemonitor-f4bc71f029b61d49.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      320 2021-09-20 15:26:10.000000 masakari-monitors-9.0.3/releasenotes/notes/pythonize-monitors-081e74dfaf78fe99.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-09-20 15:26:45.477691 masakari-monitors-9.0.3/releasenotes/source/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-09-20 15:26:45.481691 masakari-monitors-9.0.3/releasenotes/source/_static/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-09-20 15:26:10.000000 masakari-monitors-9.0.3/releasenotes/source/_static/.placeholder
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-09-20 15:26:45.481691 masakari-monitors-9.0.3/releasenotes/source/_templates/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-09-20 15:26:10.000000 masakari-monitors-9.0.3/releasenotes/source/_templates/.placeholder
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9245 2021-09-20 15:26:10.000000 masakari-monitors-9.0.3/releasenotes/source/conf.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      232 2021-09-20 15:26:10.000000 masakari-monitors-9.0.3/releasenotes/source/index.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      137 2021-09-20 15:26:10.000000 masakari-monitors-9.0.3/releasenotes/source/ocata.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      133 2021-09-20 15:26:10.000000 masakari-monitors-9.0.3/releasenotes/source/pike.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      141 2021-09-20 15:26:10.000000 masakari-monitors-9.0.3/releasenotes/source/queens.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      145 2021-09-20 15:26:10.000000 masakari-monitors-9.0.3/releasenotes/source/rocky.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      145 2021-09-20 15:26:10.000000 masakari-monitors-9.0.3/releasenotes/source/stein.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      126 2021-09-20 15:26:10.000000 masakari-monitors-9.0.3/releasenotes/source/train.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      112 2021-09-20 15:26:10.000000 masakari-monitors-9.0.3/releasenotes/source/unreleased.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      703 2021-09-20 15:26:10.000000 masakari-monitors-9.0.3/requirements.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2226 2021-09-20 15:26:45.481691 masakari-monitors-9.0.3/setup.cfg
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1030 2021-09-20 15:26:10.000000 masakari-monitors-9.0.3/setup.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      582 2021-09-20 15:26:10.000000 masakari-monitors-9.0.3/test-requirements.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3187 2021-09-20 15:26:10.000000 masakari-monitors-9.0.3/tox.ini
```

### Comparing `masakari-monitors-9.0.2/AUTHORS` & `masakari-monitors-9.0.3/AUTHORS`

 * *Files identical despite different names*

### Comparing `masakari-monitors-9.0.2/CONTRIBUTING.rst` & `masakari-monitors-9.0.3/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `masakari-monitors-9.0.2/ChangeLog` & `masakari-monitors-9.0.3/ChangeLog`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,15 @@
 CHANGES
 =======
 
+9.0.3
+-----
+
+* Fix hostmonitor to respect quorum
+
 9.0.2
 -----
 
 * Fix hostmonitor hanging forever after certain exceptions
 * Drop lower-constraints
 * Fix the release jobs
 * Remove unnecessary continue statement
```

### Comparing `masakari-monitors-9.0.2/LICENSE` & `masakari-monitors-9.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `masakari-monitors-9.0.2/PKG-INFO` & `masakari-monitors-9.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: masakari-monitors
-Version: 9.0.2
+Version: 9.0.3
 Summary: Monitors for Masakari
 Home-page: http://www.openstack.org/
 Author: OpenStack
 Author-email: openstack-dev@lists.openstack.org
 License: UNKNOWN
 Description: ===============================
         masakari-monitors
```

### Comparing `masakari-monitors-9.0.2/README.rst` & `masakari-monitors-9.0.3/README.rst`

 * *Files identical despite different names*

### Comparing `masakari-monitors-9.0.2/doc/source/conf.py` & `masakari-monitors-9.0.3/doc/source/conf.py`

 * *Files identical despite different names*

### Comparing `masakari-monitors-9.0.2/doc/source/index.rst` & `masakari-monitors-9.0.3/doc/source/index.rst`

 * *Files identical despite different names*

### Comparing `masakari-monitors-9.0.2/etc/masakarimonitors/hostmonitor.conf.sample` & `masakari-monitors-9.0.3/etc/masakarimonitors/hostmonitor.conf.sample`

 * *Files identical despite different names*

### Comparing `masakari-monitors-9.0.2/etc/masakarimonitors/process_list.yaml.sample` & `masakari-monitors-9.0.3/etc/masakarimonitors/process_list.yaml.sample`

 * *Files identical despite different names*

### Comparing `masakari-monitors-9.0.2/masakari_monitors.egg-info/PKG-INFO` & `masakari-monitors-9.0.3/masakari_monitors.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: masakari-monitors
-Version: 9.0.2
+Version: 9.0.3
 Summary: Monitors for Masakari
 Home-page: http://www.openstack.org/
 Author: OpenStack
 Author-email: openstack-dev@lists.openstack.org
 License: UNKNOWN
 Description: ===============================
         masakari-monitors
```

### Comparing `masakari-monitors-9.0.2/masakari_monitors.egg-info/SOURCES.txt` & `masakari-monitors-9.0.3/masakari_monitors.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -116,14 +116,15 @@
 masakarimonitors/tests/unit/introspectiveinstancemonitor/test_qemu_utils.py
 masakarimonitors/tests/unit/processmonitor/__init__.py
 masakarimonitors/tests/unit/processmonitor/test_process.py
 masakarimonitors/tests/unit/processmonitor/process_handler/__init__.py
 masakarimonitors/tests/unit/processmonitor/process_handler/test_handle_process.py
 releasenotes/notes/.placeholder
 releasenotes/notes/bug-1866660-ef8624f5283b2e5e.yaml
+releasenotes/notes/bug-1878548-5fab31aec6ba5407.yaml
 releasenotes/notes/bug-1930361-fa8ce8e9781ea967.yaml
 releasenotes/notes/drop-py-2-7-b28de816eac45468.yaml
 releasenotes/notes/introspectiveinstancemonitor-f4bc71f029b61d49.yaml
 releasenotes/notes/pythonize-monitors-081e74dfaf78fe99.yaml
 releasenotes/source/conf.py
 releasenotes/source/index.rst
 releasenotes/source/ocata.rst
```

### Comparing `masakari-monitors-9.0.2/masakari_monitors.egg-info/entry_points.txt` & `masakari-monitors-9.0.3/masakari_monitors.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `masakari-monitors-9.0.2/masakarimonitors/__init__.py` & `masakari-monitors-9.0.3/masakarimonitors/__init__.py`

 * *Files identical despite different names*

### Comparing `masakari-monitors-9.0.2/masakarimonitors/cmd/hostmonitor.py` & `masakari-monitors-9.0.3/masakarimonitors/cmd/hostmonitor.py`

 * *Files identical despite different names*

### Comparing `masakari-monitors-9.0.2/masakarimonitors/cmd/instancemonitor.py` & `masakari-monitors-9.0.3/masakarimonitors/cmd/instancemonitor.py`

 * *Files identical despite different names*

### Comparing `masakari-monitors-9.0.2/masakarimonitors/cmd/introspectiveinstancemonitor.py` & `masakari-monitors-9.0.3/masakarimonitors/cmd/introspectiveinstancemonitor.py`

 * *Files identical despite different names*

### Comparing `masakari-monitors-9.0.2/masakarimonitors/cmd/processmonitor.py` & `masakari-monitors-9.0.3/masakarimonitors/cmd/processmonitor.py`

 * *Files identical despite different names*

### Comparing `masakari-monitors-9.0.2/masakarimonitors/common/config.py` & `masakari-monitors-9.0.3/masakarimonitors/common/config.py`

 * *Files identical despite different names*

### Comparing `masakari-monitors-9.0.2/masakarimonitors/conf/__init__.py` & `masakari-monitors-9.0.3/masakarimonitors/conf/__init__.py`

 * *Files identical despite different names*

### Comparing `masakari-monitors-9.0.2/masakarimonitors/conf/api.py` & `masakari-monitors-9.0.3/masakarimonitors/conf/api.py`

 * *Files identical despite different names*

### Comparing `masakari-monitors-9.0.2/masakarimonitors/conf/base.py` & `masakari-monitors-9.0.3/masakarimonitors/conf/base.py`

 * *Files identical despite different names*

### Comparing `masakari-monitors-9.0.2/masakarimonitors/conf/host.py` & `masakari-monitors-9.0.3/masakarimonitors/conf/host.py`

 * *Files identical despite different names*

### Comparing `masakari-monitors-9.0.2/masakarimonitors/conf/instance.py` & `masakari-monitors-9.0.3/masakarimonitors/conf/instance.py`

 * *Files identical despite different names*

### Comparing `masakari-monitors-9.0.2/masakarimonitors/conf/introspectiveinstancemonitor.py` & `masakari-monitors-9.0.3/masakarimonitors/conf/introspectiveinstancemonitor.py`

 * *Files identical despite different names*

### Comparing `masakari-monitors-9.0.2/masakarimonitors/conf/opts.py` & `masakari-monitors-9.0.3/masakarimonitors/conf/opts.py`

 * *Files identical despite different names*

### Comparing `masakari-monitors-9.0.2/masakarimonitors/conf/process.py` & `masakari-monitors-9.0.3/masakarimonitors/conf/process.py`

 * *Files identical despite different names*

### Comparing `masakari-monitors-9.0.2/masakarimonitors/conf/service.py` & `masakari-monitors-9.0.3/masakarimonitors/conf/service.py`

 * *Files identical despite different names*

### Comparing `masakari-monitors-9.0.2/masakarimonitors/config.py` & `masakari-monitors-9.0.3/masakarimonitors/config.py`

 * *Files identical despite different names*

### Comparing `masakari-monitors-9.0.2/masakarimonitors/ha/masakari.py` & `masakari-monitors-9.0.3/masakarimonitors/ha/masakari.py`

 * *Files identical despite different names*

### Comparing `masakari-monitors-9.0.2/masakarimonitors/hacking/checks.py` & `masakari-monitors-9.0.3/masakarimonitors/hacking/checks.py`

 * *Files identical despite different names*

### Comparing `masakari-monitors-9.0.2/masakarimonitors/hostmonitor/host.py` & `masakari-monitors-9.0.3/masakarimonitors/hostmonitor/host.py`

 * *Files identical despite different names*

### Comparing `masakari-monitors-9.0.2/masakarimonitors/hostmonitor/host_handler/driver.py` & `masakari-monitors-9.0.3/masakarimonitors/hostmonitor/host_handler/driver.py`

 * *Files identical despite different names*

### Comparing `masakari-monitors-9.0.2/masakarimonitors/hostmonitor/host_handler/handle_host.py` & `masakari-monitors-9.0.3/masakarimonitors/hostmonitor/host_handler/handle_host.py`

 * *Files 1% similar despite different names*

```diff
@@ -333,14 +333,20 @@
         if crmmon_xml is None:
             # crm_mon command failure.
             return 1
 
         # Set to the ParseCrmMonXml object.
         self.crmmon_xml_parser.set_crmmon_xml(crmmon_xml)
 
+        # Check if the cluster has quorum.
+        if not self.crmmon_xml_parser.has_quorum():
+            msg = "Pacemaker cluster doesn't have quorum."
+            LOG.warning("%s", msg)
+            return 2
+
         # Get node_state tag list.
         node_state_tag_list = self.crmmon_xml_parser.get_node_state_tag_list()
         if len(node_state_tag_list) == 0:
             # If crmmon xml doesn't have node_state tag,
             # it is an unexpected result.
             raise Exception(
                 "Failed to get nodes tag from crm_mon xml.")
@@ -363,14 +369,15 @@
         # Set to the ParseCibXml object.
         self.xml_parser.set_cib_xml(cib_xml)
 
         # Check if pacemaker cluster have quorum.
         if self.xml_parser.have_quorum() == 0:
             msg = "Pacemaker cluster doesn't have quorum."
             LOG.warning("%s", msg)
+            return 2
 
         # Get node_state tag list.
         node_state_tag_list = self.xml_parser.get_node_state_tag_list()
         if len(node_state_tag_list) == 0:
             # If cib xml doesn't have node_state tag,
             # it is an unexpected result.
             raise Exception(
```

### Comparing `masakari-monitors-9.0.2/masakarimonitors/hostmonitor/host_handler/hold_host_status.py` & `masakari-monitors-9.0.3/masakarimonitors/hostmonitor/host_handler/hold_host_status.py`

 * *Files identical despite different names*

### Comparing `masakari-monitors-9.0.2/masakarimonitors/hostmonitor/host_handler/parse_cib_xml.py` & `masakari-monitors-9.0.3/masakarimonitors/hostmonitor/host_handler/parse_cib_xml.py`

 * *Files identical despite different names*

### Comparing `masakari-monitors-9.0.2/masakarimonitors/hostmonitor/host_handler/parse_crmmon_xml.py` & `masakari-monitors-9.0.3/masakarimonitors/hostmonitor/host_handler/parse_crmmon_xml.py`

 * *Files 23% similar despite different names*

```diff
@@ -35,14 +35,36 @@
         to xml.etree.ElementTree.Element object.
 
         :params crmmon_xml: String of crmmon xml
         """
         # Convert xml.etree.ElementTree.Element object.
         self.crmmon_tag = ElementTree.fromstring(crmmon_xml)
 
+    def has_quorum(self):
+        """Answers if cluster has quorum or not.
+
+        :returns: True if cluster has quorum, False otherwise.
+        """
+        current_dc = self._get_current_dc()
+        return current_dc.get('with_quorum') == 'true'
+
+    def _get_summary(self):
+        child_list = list(self.crmmon_tag)
+        for child in child_list:
+            if child.tag == 'summary':
+                return child
+        return None
+
+    def _get_current_dc(self):
+        child_list = list(self._get_summary())
+        for child in child_list:
+            if child.tag == 'current_dc':
+                return child
+        return None
+
     def _get_nodes(self):
         # status tag exists in the crmmon tag.
         if self.crmmon_tag is None:
             return None
         child_list = self.crmmon_tag.getchildren()
         for child in child_list:
             if child.tag == 'nodes':
```

### Comparing `masakari-monitors-9.0.2/masakarimonitors/i18n.py` & `masakari-monitors-9.0.3/masakarimonitors/i18n.py`

 * *Files identical despite different names*

### Comparing `masakari-monitors-9.0.2/masakarimonitors/instancemonitor/instance.py` & `masakari-monitors-9.0.3/masakarimonitors/instancemonitor/instance.py`

 * *Files identical despite different names*

### Comparing `masakari-monitors-9.0.2/masakarimonitors/instancemonitor/libvirt_handler/callback.py` & `masakari-monitors-9.0.3/masakarimonitors/instancemonitor/libvirt_handler/callback.py`

 * *Files identical despite different names*

### Comparing `masakari-monitors-9.0.2/masakarimonitors/instancemonitor/libvirt_handler/eventfilter.py` & `masakari-monitors-9.0.3/masakarimonitors/instancemonitor/libvirt_handler/eventfilter.py`

 * *Files identical despite different names*

### Comparing `masakari-monitors-9.0.2/masakarimonitors/instancemonitor/libvirt_handler/eventfilter_table.py` & `masakari-monitors-9.0.3/masakarimonitors/instancemonitor/libvirt_handler/eventfilter_table.py`

 * *Files identical despite different names*

### Comparing `masakari-monitors-9.0.2/masakarimonitors/introspectiveinstancemonitor/README.rst` & `masakari-monitors-9.0.3/masakarimonitors/introspectiveinstancemonitor/README.rst`

 * *Files identical despite different names*

### Comparing `masakari-monitors-9.0.2/masakarimonitors/introspectiveinstancemonitor/cache.py` & `masakari-monitors-9.0.3/masakarimonitors/introspectiveinstancemonitor/cache.py`

 * *Files identical despite different names*

### Comparing `masakari-monitors-9.0.2/masakarimonitors/introspectiveinstancemonitor/instance.py` & `masakari-monitors-9.0.3/masakarimonitors/introspectiveinstancemonitor/instance.py`

 * *Files identical despite different names*

### Comparing `masakari-monitors-9.0.2/masakarimonitors/introspectiveinstancemonitor/qemu_utils.py` & `masakari-monitors-9.0.3/masakarimonitors/introspectiveinstancemonitor/qemu_utils.py`

 * *Files identical despite different names*

### Comparing `masakari-monitors-9.0.2/masakarimonitors/introspectiveinstancemonitor/scheduler.py` & `masakari-monitors-9.0.3/masakarimonitors/introspectiveinstancemonitor/scheduler.py`

 * *Files identical despite different names*

### Comparing `masakari-monitors-9.0.2/masakarimonitors/manager.py` & `masakari-monitors-9.0.3/masakarimonitors/manager.py`

 * *Files identical despite different names*

### Comparing `masakari-monitors-9.0.2/masakarimonitors/objects/event_constants.py` & `masakari-monitors-9.0.3/masakarimonitors/objects/event_constants.py`

 * *Files identical despite different names*

### Comparing `masakari-monitors-9.0.2/masakarimonitors/privsep.py` & `masakari-monitors-9.0.3/masakarimonitors/privsep.py`

 * *Files identical despite different names*

### Comparing `masakari-monitors-9.0.2/masakarimonitors/processmonitor/process.py` & `masakari-monitors-9.0.3/masakarimonitors/processmonitor/process.py`

 * *Files identical despite different names*

### Comparing `masakari-monitors-9.0.2/masakarimonitors/processmonitor/process_handler/handle_process.py` & `masakari-monitors-9.0.3/masakarimonitors/processmonitor/process_handler/handle_process.py`

 * *Files identical despite different names*

### Comparing `masakari-monitors-9.0.2/masakarimonitors/service.py` & `masakari-monitors-9.0.3/masakarimonitors/service.py`

 * *Files identical despite different names*

### Comparing `masakari-monitors-9.0.2/masakarimonitors/tests/base.py` & `masakari-monitors-9.0.3/masakarimonitors/tests/base.py`

 * *Files identical despite different names*

### Comparing `masakari-monitors-9.0.2/masakarimonitors/tests/test_masakarimonitors.py` & `masakari-monitors-9.0.3/masakarimonitors/tests/test_masakarimonitors.py`

 * *Files identical despite different names*

### Comparing `masakari-monitors-9.0.2/masakarimonitors/tests/unit/ha/test_masakari.py` & `masakari-monitors-9.0.3/masakarimonitors/tests/unit/ha/test_masakari.py`

 * *Files identical despite different names*

### Comparing `masakari-monitors-9.0.2/masakarimonitors/tests/unit/hostmonitor/host_handler/test_handle_host.py` & `masakari-monitors-9.0.3/masakarimonitors/tests/unit/hostmonitor/host_handler/test_handle_host.py`

 * *Files 2% similar despite different names*

```diff
@@ -638,49 +638,74 @@
         mock_make_event.assert_called_once_with(node4, 'offline')
         mock_send_notification.assert_called_once_with(
             CONF.host.api_retry_max, CONF.host.api_retry_interval, test_event)
 
     @mock.patch.object(handle_host.HandleHost, '_check_if_status_changed')
     @mock.patch.object(parse_crmmon_xml.ParseCrmMonXml,
                        'get_node_state_tag_list')
+    @mock.patch.object(parse_crmmon_xml.ParseCrmMonXml,
+                       'has_quorum')
     @mock.patch.object(parse_crmmon_xml.ParseCrmMonXml, 'set_crmmon_xml')
     @mock.patch.object(handle_host.HandleHost, '_get_crmmon_xml')
     def test_check_host_status_by_crm_mon(
         self, mock_get_crmmon_xml, mock_set_crmmon_xml,
-        mock_get_node_state_tag_list, mock_check_if_status_changed):
+        mock_has_quorum, mock_get_node_state_tag_list,
+        mock_check_if_status_changed):
         mock_get_crmmon_xml.return_value = CRMMON_NODES_TAG_XML
         mock_set_crmmon_xml.return_value = None
+        mock_has_quorum.return_value = True
         status_tag = ElementTree.fromstring(CRMMON_NODES_TAG_XML)
         node_state_tag_list = status_tag.getchildren()
         mock_get_node_state_tag_list.return_value = node_state_tag_list
         mock_check_if_status_changed.return_value = None
 
         obj = handle_host.HandleHost()
         ret = obj._check_host_status_by_crm_mon()
 
         self.assertEqual(0, ret)
-        mock_get_node_state_tag_list.assert_called_once_with()
         mock_set_crmmon_xml.assert_called_once_with(CRMMON_NODES_TAG_XML)
         mock_get_node_state_tag_list.assert_called_once_with()
         mock_check_if_status_changed.assert_called_once_with(
             [
                 {'uname': 'remote1', 'crmd': 'online'},
                 {'uname': 'remote2', 'crmd': 'online'},
                 {'uname': 'remote3', 'crmd': 'online'}])
 
+    @mock.patch.object(handle_host.HandleHost, '_check_if_status_changed')
+    @mock.patch.object(parse_crmmon_xml.ParseCrmMonXml,
+                       'has_quorum')
+    @mock.patch.object(parse_crmmon_xml.ParseCrmMonXml, 'set_crmmon_xml')
+    @mock.patch.object(handle_host.HandleHost, '_get_crmmon_xml')
+    def test_check_host_status_by_crm_mon_no_quorum(
+        self, mock_get_crmmon_xml, mock_set_crmmon_xml,
+        mock_has_quorum, mock_check_if_status_changed):
+        mock_get_crmmon_xml.return_value = CRMMON_NODES_TAG_XML
+        mock_set_crmmon_xml.return_value = None
+        mock_has_quorum.return_value = False
+
+        obj = handle_host.HandleHost()
+        ret = obj._check_host_status_by_crm_mon()
+
+        self.assertEqual(2, ret)
+        mock_set_crmmon_xml.assert_called_once_with(CRMMON_NODES_TAG_XML)
+        mock_check_if_status_changed.assert_not_called()
+
+    @mock.patch.object(parse_crmmon_xml.ParseCrmMonXml,
+                       'has_quorum')
     @mock.patch.object(parse_crmmon_xml.ParseCrmMonXml,
                        'get_node_state_tag_list')
     @mock.patch.object(parse_crmmon_xml.ParseCrmMonXml, 'set_crmmon_xml')
     @mock.patch.object(handle_host.HandleHost, '_get_crmmon_xml')
     def test_check_host_status_by_crm_mon_not_have_node_state_tag(
         self, mock_get_crmmon_xml, mock_set_crmmon_xml,
-        mock_get_node_state_tag_list):
+        mock_get_node_state_tag_list, mock_has_quorum):
         mock_get_crmmon_xml.return_value = CRMMON_NODES_TAG_XML
         mock_set_crmmon_xml.return_value = None
         mock_get_node_state_tag_list.return_value = []
+        mock_has_quorum.return_value = True
 
         obj = handle_host.HandleHost()
 
         self.assertRaisesRegexp(
             Exception, "Failed to get nodes tag from crm_mon xml.",
             obj._check_host_status_by_crm_mon)
         mock_get_crmmon_xml.assert_called_once_with()
@@ -722,39 +747,32 @@
         mock_set_cib_xml.assert_called_once_with(STATUS_TAG_XML)
         mock_have_quorum.assert_called_once_with()
         mock_get_node_state_tag_list.assert_called_once_with()
         mock_check_if_status_changed.assert_called_once_with(
             node_state_tag_list)
 
     @mock.patch.object(handle_host.HandleHost, '_check_if_status_changed')
-    @mock.patch.object(parse_cib_xml.ParseCibXml, 'get_node_state_tag_list')
     @mock.patch.object(parse_cib_xml.ParseCibXml, 'have_quorum')
     @mock.patch.object(parse_cib_xml.ParseCibXml, 'set_cib_xml')
     @mock.patch.object(handle_host.HandleHost, '_get_cib_xml')
     def test_check_host_status_by_cibadmin_no_quorum(
         self, mock_get_cib_xml, mock_set_cib_xml, mock_have_quorum,
-        mock_get_node_state_tag_list, mock_check_if_status_changed):
+        mock_check_if_status_changed):
         mock_get_cib_xml.return_value = STATUS_TAG_XML
         mock_set_cib_xml.return_value = None
         mock_have_quorum.return_value = 0
-        status_tag = ElementTree.fromstring(STATUS_TAG_XML)
-        node_state_tag_list = status_tag.getchildren()
-        mock_get_node_state_tag_list.return_value = node_state_tag_list
-        mock_check_if_status_changed.return_value = None
 
         obj = handle_host.HandleHost()
         ret = obj._check_host_status_by_cibadmin()
 
-        self.assertEqual(0, ret)
+        self.assertEqual(2, ret)
         mock_get_cib_xml.assert_called_once_with()
         mock_set_cib_xml.assert_called_once_with(STATUS_TAG_XML)
         mock_have_quorum.assert_called_once_with()
-        mock_get_node_state_tag_list.assert_called_once_with()
-        mock_check_if_status_changed.assert_called_once_with(
-            node_state_tag_list)
+        mock_check_if_status_changed.assert_not_called()
 
     @mock.patch.object(handle_host.HandleHost, '_get_cib_xml')
     def test_check_host_status_by_cibadmin_cib_xml_is_None(
         self, mock_get_cib_xml):
         mock_get_cib_xml.return_value = None
 
         obj = handle_host.HandleHost()
```

### Comparing `masakari-monitors-9.0.2/masakarimonitors/tests/unit/hostmonitor/host_handler/test_hold_host_status.py` & `masakari-monitors-9.0.3/masakarimonitors/tests/unit/hostmonitor/host_handler/test_hold_host_status.py`

 * *Files identical despite different names*

### Comparing `masakari-monitors-9.0.2/masakarimonitors/tests/unit/hostmonitor/host_handler/test_parse_cib_xml.py` & `masakari-monitors-9.0.3/masakarimonitors/tests/unit/hostmonitor/host_handler/test_parse_cib_xml.py`

 * *Files identical despite different names*

### Comparing `masakari-monitors-9.0.2/masakarimonitors/tests/unit/hostmonitor/host_handler/test_parse_crmmon_xml.py` & `masakari-monitors-9.0.3/masakarimonitors/tests/unit/hostmonitor/host_handler/test_parse_crmmon_xml.py`

 * *Files 17% similar despite different names*

```diff
@@ -16,21 +16,34 @@
 import testtools
 
 from masakarimonitors.hostmonitor.host_handler import parse_crmmon_xml
 
 
 CRMMON_XML = '<?xml version="1.0"?>' \
              '<crm_mon version="1.1.18">' \
+             '    <summary>' \
+             '        <stack type="corosync" />' \
+             '        <current_dc present="true" with_quorum="true" />' \
+             '    </summary>' \
              '    <nodes>' \
              '        <node name="node-1" id="1001" online="true" />' \
              '        <node name="node-2" id="1002" online="false" />' \
              '        <node name="node-3" id="1003" online="true" />' \
              '    </nodes>' \
              '</crm_mon>'
 
+CRMMON_XML_NO_QUORUM = \
+    '<?xml version="1.0"?>' \
+    '<crm_mon version="1.1.18">' \
+    '    <summary>' \
+    '        <stack type="corosync" />' \
+    '        <current_dc present="true" with_quorum="false" />' \
+    '    </summary>' \
+    '</crm_mon>'
+
 CRMMON_NONODES_XML = '<?xml version="1.0"?>' \
                      '<crm_mon version="1.1.18">' \
                      '    <nodes>' \
                      '    </nodes>' \
                      '</crm_mon>'
 
 CRMMON_NONODES_TAG_XML = '<?xml version="1.0"?>' \
@@ -43,14 +56,24 @@
     def setUp(self):
         super(TestParseCrmMonXml, self).setUp()
 
     def test_set_crmmon_xml(self):
         obj = parse_crmmon_xml.ParseCrmMonXml()
         obj.set_crmmon_xml(CRMMON_XML)
 
+    def test_has_quorum(self):
+        obj = parse_crmmon_xml.ParseCrmMonXml()
+        obj.set_crmmon_xml(CRMMON_XML)
+        self.assertEqual(True, obj.has_quorum())
+
+    def test_has_quorum_no_quorum(self):
+        obj = parse_crmmon_xml.ParseCrmMonXml()
+        obj.set_crmmon_xml(CRMMON_XML_NO_QUORUM)
+        self.assertEqual(False, obj.has_quorum())
+
     def test_get_node_state_tag_list(self):
         obj = parse_crmmon_xml.ParseCrmMonXml()
         obj.set_crmmon_xml(CRMMON_XML)
 
         node_state_tag_list = obj.get_node_state_tag_list()
 
         expected = {
```

### Comparing `masakari-monitors-9.0.2/masakarimonitors/tests/unit/hostmonitor/test_host.py` & `masakari-monitors-9.0.3/masakarimonitors/tests/unit/hostmonitor/test_host.py`

 * *Files identical despite different names*

### Comparing `masakari-monitors-9.0.2/masakarimonitors/tests/unit/instancemonitor/libvirt_handler/test_callback.py` & `masakari-monitors-9.0.3/masakarimonitors/tests/unit/instancemonitor/libvirt_handler/test_callback.py`

 * *Files identical despite different names*

### Comparing `masakari-monitors-9.0.2/masakarimonitors/tests/unit/instancemonitor/libvirt_handler/test_eventfilter.py` & `masakari-monitors-9.0.3/masakarimonitors/tests/unit/instancemonitor/libvirt_handler/test_eventfilter.py`

 * *Files identical despite different names*

### Comparing `masakari-monitors-9.0.2/masakarimonitors/tests/unit/instancemonitor/test_instance.py` & `masakari-monitors-9.0.3/masakarimonitors/tests/unit/instancemonitor/test_instance.py`

 * *Files identical despite different names*

### Comparing `masakari-monitors-9.0.2/masakarimonitors/tests/unit/introspectiveinstancemonitor/test_monitor_manager.py` & `masakari-monitors-9.0.3/masakarimonitors/tests/unit/introspectiveinstancemonitor/test_monitor_manager.py`

 * *Files identical despite different names*

### Comparing `masakari-monitors-9.0.2/masakarimonitors/tests/unit/introspectiveinstancemonitor/test_qemu_utils.py` & `masakari-monitors-9.0.3/masakarimonitors/tests/unit/introspectiveinstancemonitor/test_qemu_utils.py`

 * *Files identical despite different names*

### Comparing `masakari-monitors-9.0.2/masakarimonitors/tests/unit/processmonitor/process_handler/test_handle_process.py` & `masakari-monitors-9.0.3/masakarimonitors/tests/unit/processmonitor/process_handler/test_handle_process.py`

 * *Files identical despite different names*

### Comparing `masakari-monitors-9.0.2/masakarimonitors/tests/unit/processmonitor/test_process.py` & `masakari-monitors-9.0.3/masakarimonitors/tests/unit/processmonitor/test_process.py`

 * *Files identical despite different names*

### Comparing `masakari-monitors-9.0.2/masakarimonitors/tests/unit/test_hacking.py` & `masakari-monitors-9.0.3/masakarimonitors/tests/unit/test_hacking.py`

 * *Files identical despite different names*

### Comparing `masakari-monitors-9.0.2/masakarimonitors/utils.py` & `masakari-monitors-9.0.3/masakarimonitors/utils.py`

 * *Files identical despite different names*

### Comparing `masakari-monitors-9.0.2/masakarimonitors/version.py` & `masakari-monitors-9.0.3/masakarimonitors/version.py`

 * *Files identical despite different names*

### Comparing `masakari-monitors-9.0.2/releasenotes/source/conf.py` & `masakari-monitors-9.0.3/releasenotes/source/conf.py`

 * *Files identical despite different names*

### Comparing `masakari-monitors-9.0.2/requirements.txt` & `masakari-monitors-9.0.3/requirements.txt`

 * *Files identical despite different names*

### Comparing `masakari-monitors-9.0.2/setup.cfg` & `masakari-monitors-9.0.3/setup.cfg`

 * *Files identical despite different names*

### Comparing `masakari-monitors-9.0.2/setup.py` & `masakari-monitors-9.0.3/setup.py`

 * *Files identical despite different names*

### Comparing `masakari-monitors-9.0.2/test-requirements.txt` & `masakari-monitors-9.0.3/test-requirements.txt`

 * *Files identical despite different names*

### Comparing `masakari-monitors-9.0.2/tox.ini` & `masakari-monitors-9.0.3/tox.ini`

 * *Files identical despite different names*

