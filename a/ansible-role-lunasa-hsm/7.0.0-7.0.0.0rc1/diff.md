# Comparing `tmp/ansible-role-lunasa-hsm-7.0.0.tar.gz` & `tmp/ansible-role-lunasa-hsm-7.0.0.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ansible-role-lunasa-hsm-7.0.0.tar", last modified: Wed Apr  3 11:08:32 2024, max compression
+gzip compressed data, was "ansible-role-lunasa-hsm-7.0.0.0rc1.tar", last modified: Tue Mar 19 10:03:27 2024, max compression
```

## Comparing `ansible-role-lunasa-hsm-7.0.0.tar` & `ansible-role-lunasa-hsm-7.0.0.0rc1.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:08:32.594312 ansible-role-lunasa-hsm-7.0.0/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      192 2024-04-03 11:08:03.000000 ansible-role-lunasa-hsm-7.0.0/.zuul.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      216 2024-04-03 11:08:32.000000 ansible-role-lunasa-hsm-7.0.0/AUTHORS
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      685 2024-04-03 11:08:32.000000 ansible-role-lunasa-hsm-7.0.0/ChangeLog
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    11358 2024-04-03 11:08:03.000000 ansible-role-lunasa-hsm-7.0.0/LICENSE
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2499 2024-04-03 11:08:32.594312 ansible-role-lunasa-hsm-7.0.0/PKG-INFO
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1477 2024-04-03 11:08:03.000000 ansible-role-lunasa-hsm-7.0.0/README.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:08:32.594312 ansible-role-lunasa-hsm-7.0.0/ansible_role_lunasa_hsm.egg-info/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2499 2024-04-03 11:08:32.000000 ansible-role-lunasa-hsm-7.0.0/ansible_role_lunasa_hsm.egg-info/PKG-INFO
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      526 2024-04-03 11:08:32.000000 ansible-role-lunasa-hsm-7.0.0/ansible_role_lunasa_hsm.egg-info/SOURCES.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2024-04-03 11:08:32.000000 ansible-role-lunasa-hsm-7.0.0/ansible_role_lunasa_hsm.egg-info/dependency_links.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2024-04-03 11:08:32.000000 ansible-role-lunasa-hsm-7.0.0/ansible_role_lunasa_hsm.egg-info/not-zip-safe
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       46 2024-04-03 11:08:32.000000 ansible-role-lunasa-hsm-7.0.0/ansible_role_lunasa_hsm.egg-info/pbr.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       17 2024-04-03 11:08:32.000000 ansible-role-lunasa-hsm-7.0.0/ansible_role_lunasa_hsm.egg-info/requires.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2024-04-03 11:08:32.000000 ansible-role-lunasa-hsm-7.0.0/ansible_role_lunasa_hsm.egg-info/top_level.txt
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:08:32.594312 ansible-role-lunasa-hsm-7.0.0/defaults/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      118 2024-04-03 11:08:03.000000 ansible-role-lunasa-hsm-7.0.0/defaults/main.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       17 2024-04-03 11:08:03.000000 ansible-role-lunasa-hsm-7.0.0/requirements.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      829 2024-04-03 11:08:32.598312 ansible-role-lunasa-hsm-7.0.0/setup.cfg
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      712 2024-04-03 11:08:03.000000 ansible-role-lunasa-hsm-7.0.0/setup.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:08:32.594312 ansible-role-lunasa-hsm-7.0.0/tasks/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4635 2024-04-03 11:08:03.000000 ansible-role-lunasa-hsm-7.0.0/tasks/main.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2989 2024-04-03 11:08:03.000000 ansible-role-lunasa-hsm-7.0.0/tasks/register_client.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      317 2024-04-03 11:08:03.000000 ansible-role-lunasa-hsm-7.0.0/tasks/unregister_client.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       13 2024-04-03 11:08:03.000000 ansible-role-lunasa-hsm-7.0.0/test-requirements.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      526 2024-04-03 11:08:03.000000 ansible-role-lunasa-hsm-7.0.0/tox.ini
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-19 10:03:27.276222 ansible-role-lunasa-hsm-7.0.0.0rc1/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      192 2024-03-19 10:03:00.000000 ansible-role-lunasa-hsm-7.0.0.0rc1/.zuul.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      216 2024-03-19 10:03:27.000000 ansible-role-lunasa-hsm-7.0.0.0rc1/AUTHORS
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      695 2024-03-19 10:03:27.000000 ansible-role-lunasa-hsm-7.0.0.0rc1/ChangeLog
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    11358 2024-03-19 10:03:00.000000 ansible-role-lunasa-hsm-7.0.0.0rc1/LICENSE
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2504 2024-03-19 10:03:27.276222 ansible-role-lunasa-hsm-7.0.0.0rc1/PKG-INFO
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1477 2024-03-19 10:03:00.000000 ansible-role-lunasa-hsm-7.0.0.0rc1/README.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-19 10:03:27.276222 ansible-role-lunasa-hsm-7.0.0.0rc1/ansible_role_lunasa_hsm.egg-info/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2504 2024-03-19 10:03:27.000000 ansible-role-lunasa-hsm-7.0.0.0rc1/ansible_role_lunasa_hsm.egg-info/PKG-INFO
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      526 2024-03-19 10:03:27.000000 ansible-role-lunasa-hsm-7.0.0.0rc1/ansible_role_lunasa_hsm.egg-info/SOURCES.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2024-03-19 10:03:27.000000 ansible-role-lunasa-hsm-7.0.0.0rc1/ansible_role_lunasa_hsm.egg-info/dependency_links.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2024-03-19 10:03:27.000000 ansible-role-lunasa-hsm-7.0.0.0rc1/ansible_role_lunasa_hsm.egg-info/not-zip-safe
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       46 2024-03-19 10:03:27.000000 ansible-role-lunasa-hsm-7.0.0.0rc1/ansible_role_lunasa_hsm.egg-info/pbr.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       17 2024-03-19 10:03:27.000000 ansible-role-lunasa-hsm-7.0.0.0rc1/ansible_role_lunasa_hsm.egg-info/requires.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2024-03-19 10:03:27.000000 ansible-role-lunasa-hsm-7.0.0.0rc1/ansible_role_lunasa_hsm.egg-info/top_level.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-19 10:03:27.276222 ansible-role-lunasa-hsm-7.0.0.0rc1/defaults/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      118 2024-03-19 10:03:00.000000 ansible-role-lunasa-hsm-7.0.0.0rc1/defaults/main.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       17 2024-03-19 10:03:00.000000 ansible-role-lunasa-hsm-7.0.0.0rc1/requirements.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      829 2024-03-19 10:03:27.276222 ansible-role-lunasa-hsm-7.0.0.0rc1/setup.cfg
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      712 2024-03-19 10:03:00.000000 ansible-role-lunasa-hsm-7.0.0.0rc1/setup.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-19 10:03:27.276222 ansible-role-lunasa-hsm-7.0.0.0rc1/tasks/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4635 2024-03-19 10:03:00.000000 ansible-role-lunasa-hsm-7.0.0.0rc1/tasks/main.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2989 2024-03-19 10:03:00.000000 ansible-role-lunasa-hsm-7.0.0.0rc1/tasks/register_client.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      317 2024-03-19 10:03:00.000000 ansible-role-lunasa-hsm-7.0.0.0rc1/tasks/unregister_client.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       13 2024-03-19 10:03:00.000000 ansible-role-lunasa-hsm-7.0.0.0rc1/test-requirements.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      526 2024-03-19 10:03:00.000000 ansible-role-lunasa-hsm-7.0.0.0rc1/tox.ini
```

### Comparing `ansible-role-lunasa-hsm-7.0.0/ChangeLog` & `ansible-role-lunasa-hsm-7.0.0.0rc1/ChangeLog`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 CHANGES
 =======
 
-7.0.0
------
+7.0.0.0rc1
+----------
 
 * Disable auto-discovery for setuptools
 * Fix vtl verification
 * Fix permissions error during client installation
 * setup.cfg: Replace dashes with underscores
 * Fix lint errors
```

### Comparing `ansible-role-lunasa-hsm-7.0.0/LICENSE` & `ansible-role-lunasa-hsm-7.0.0.0rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `ansible-role-lunasa-hsm-7.0.0/PKG-INFO` & `ansible-role-lunasa-hsm-7.0.0.0rc1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: ansible-role-lunasa-hsm
-Version: 7.0.0
+Version: 7.0.0.0rc1
 Summary: ansible-role-lunasa-hsm - Ansible role to configure Lunasa HSM clients.
 Home-page: https://opendev.org/openstack/ansible-role-lunasa-hsm
 Author: TripleO Team
 Author-email: alee@redhat.com
 License: UNKNOWN
 Description: lunasa-hsm
         ==========
```

### Comparing `ansible-role-lunasa-hsm-7.0.0/README.rst` & `ansible-role-lunasa-hsm-7.0.0.0rc1/README.rst`

 * *Files identical despite different names*

### Comparing `ansible-role-lunasa-hsm-7.0.0/ansible_role_lunasa_hsm.egg-info/PKG-INFO` & `ansible-role-lunasa-hsm-7.0.0.0rc1/ansible_role_lunasa_hsm.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: ansible-role-lunasa-hsm
-Version: 7.0.0
+Version: 7.0.0.0rc1
 Summary: ansible-role-lunasa-hsm - Ansible role to configure Lunasa HSM clients.
 Home-page: https://opendev.org/openstack/ansible-role-lunasa-hsm
 Author: TripleO Team
 Author-email: alee@redhat.com
 License: UNKNOWN
 Description: lunasa-hsm
         ==========
```

### Comparing `ansible-role-lunasa-hsm-7.0.0/ansible_role_lunasa_hsm.egg-info/SOURCES.txt` & `ansible-role-lunasa-hsm-7.0.0.0rc1/ansible_role_lunasa_hsm.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ansible-role-lunasa-hsm-7.0.0/setup.cfg` & `ansible-role-lunasa-hsm-7.0.0.0rc1/setup.cfg`

 * *Files identical despite different names*

### Comparing `ansible-role-lunasa-hsm-7.0.0/setup.py` & `ansible-role-lunasa-hsm-7.0.0.0rc1/setup.py`

 * *Files identical despite different names*

### Comparing `ansible-role-lunasa-hsm-7.0.0/tasks/main.yaml` & `ansible-role-lunasa-hsm-7.0.0.0rc1/tasks/main.yaml`

 * *Files identical despite different names*

### Comparing `ansible-role-lunasa-hsm-7.0.0/tasks/register_client.yaml` & `ansible-role-lunasa-hsm-7.0.0.0rc1/tasks/register_client.yaml`

 * *Files identical despite different names*

### Comparing `ansible-role-lunasa-hsm-7.0.0/tox.ini` & `ansible-role-lunasa-hsm-7.0.0.0rc1/tox.ini`

 * *Files identical despite different names*

