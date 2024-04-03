# Comparing `tmp/ansible-role-thales-hsm-7.0.0.tar.gz` & `tmp/ansible-role-thales-hsm-7.0.0.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ansible-role-thales-hsm-7.0.0.tar", last modified: Wed Apr  3 11:08:27 2024, max compression
+gzip compressed data, was "ansible-role-thales-hsm-7.0.0.0rc1.tar", last modified: Fri Mar 15 14:44:44 2024, max compression
```

## Comparing `ansible-role-thales-hsm-7.0.0.tar` & `ansible-role-thales-hsm-7.0.0.0rc1.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:08:27.798638 ansible-role-thales-hsm-7.0.0/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       84 2024-04-03 11:08:02.000000 ansible-role-thales-hsm-7.0.0/.ansible-lint
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       68 2024-04-03 11:08:02.000000 ansible-role-thales-hsm-7.0.0/AUTHORS
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    11358 2024-04-03 11:08:02.000000 ansible-role-thales-hsm-7.0.0/LICENSE
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3251 2024-04-03 11:08:27.798638 ansible-role-thales-hsm-7.0.0/PKG-INFO
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2054 2024-04-03 11:08:02.000000 ansible-role-thales-hsm-7.0.0/README.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:08:27.794638 ansible-role-thales-hsm-7.0.0/ansible_role_thales_hsm.egg-info/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3251 2024-04-03 11:08:27.000000 ansible-role-thales-hsm-7.0.0/ansible_role_thales_hsm.egg-info/PKG-INFO
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      788 2024-04-03 11:08:27.000000 ansible-role-thales-hsm-7.0.0/ansible_role_thales_hsm.egg-info/SOURCES.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2024-04-03 11:08:27.000000 ansible-role-thales-hsm-7.0.0/ansible_role_thales_hsm.egg-info/dependency_links.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2024-04-03 11:08:27.000000 ansible-role-thales-hsm-7.0.0/ansible_role_thales_hsm.egg-info/not-zip-safe
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       46 2024-04-03 11:08:27.000000 ansible-role-thales-hsm-7.0.0/ansible_role_thales_hsm.egg-info/pbr.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       24 2024-04-03 11:08:27.000000 ansible-role-thales-hsm-7.0.0/ansible_role_thales_hsm.egg-info/requires.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2024-04-03 11:08:27.000000 ansible-role-thales-hsm-7.0.0/ansible_role_thales_hsm.egg-info/top_level.txt
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:08:27.794638 ansible-role-thales-hsm-7.0.0/defaults/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      166 2024-04-03 11:08:02.000000 ansible-role-thales-hsm-7.0.0/defaults/main.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:08:27.794638 ansible-role-thales-hsm-7.0.0/files/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4906 2024-04-03 11:08:02.000000 ansible-role-thales-hsm-7.0.0/files/add_ips.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:08:27.794638 ansible-role-thales-hsm-7.0.0/handlers/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      207 2024-04-03 11:08:02.000000 ansible-role-thales-hsm-7.0.0/handlers/main.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:08:27.794638 ansible-role-thales-hsm-7.0.0/meta/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      187 2024-04-03 11:08:02.000000 ansible-role-thales-hsm-7.0.0/meta/main.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:08:27.790638 ansible-role-thales-hsm-7.0.0/releasenotes/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:08:27.798638 ansible-role-thales-hsm-7.0.0/releasenotes/notes/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      536 2024-04-03 11:08:02.000000 ansible-role-thales-hsm-7.0.0/releasenotes/notes/add-ha-c41f45eaa1aba077.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      299 2024-04-03 11:08:02.000000 ansible-role-thales-hsm-7.0.0/releasenotes/notes/add-support-for-security-world-v13.4-2cb8688bcc072db1.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       24 2024-04-03 11:08:02.000000 ansible-role-thales-hsm-7.0.0/requirements.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      971 2024-04-03 11:08:27.798638 ansible-role-thales-hsm-7.0.0/setup.cfg
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      712 2024-04-03 11:08:02.000000 ansible-role-thales-hsm-7.0.0/setup.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:08:27.798638 ansible-role-thales-hsm-7.0.0/tasks/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3037 2024-04-03 11:08:02.000000 ansible-role-thales-hsm-7.0.0/tasks/client.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      389 2024-04-03 11:08:02.000000 ansible-role-thales-hsm-7.0.0/tasks/client_enroll.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      783 2024-04-03 11:08:02.000000 ansible-role-thales-hsm-7.0.0/tasks/main.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      352 2024-04-03 11:08:02.000000 ansible-role-thales-hsm-7.0.0/tasks/rfs.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      917 2024-04-03 11:08:02.000000 ansible-role-thales-hsm-7.0.0/tasks/rfs_register_client.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:08:27.798638 ansible-role-thales-hsm-7.0.0/templates/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      117 2024-04-03 11:08:02.000000 ansible-role-thales-hsm-7.0.0/templates/cknfastrc.j2
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       13 2024-04-03 11:08:02.000000 ansible-role-thales-hsm-7.0.0/test-requirements.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      209 2024-04-03 11:08:02.000000 ansible-role-thales-hsm-7.0.0/tox.ini
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      356 2024-04-03 11:08:02.000000 ansible-role-thales-hsm-7.0.0/vars.yaml.sample
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:08:27.798638 ansible-role-thales-hsm-7.0.0/zuul.d/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      196 2024-04-03 11:08:02.000000 ansible-role-thales-hsm-7.0.0/zuul.d/layout.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-15 14:44:44.066775 ansible-role-thales-hsm-7.0.0.0rc1/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       84 2024-03-15 14:42:35.000000 ansible-role-thales-hsm-7.0.0.0rc1/.ansible-lint
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       68 2024-03-15 14:42:35.000000 ansible-role-thales-hsm-7.0.0.0rc1/AUTHORS
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    11358 2024-03-15 14:42:35.000000 ansible-role-thales-hsm-7.0.0.0rc1/LICENSE
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3256 2024-03-15 14:44:44.066775 ansible-role-thales-hsm-7.0.0.0rc1/PKG-INFO
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2054 2024-03-15 14:42:35.000000 ansible-role-thales-hsm-7.0.0.0rc1/README.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-15 14:44:44.066775 ansible-role-thales-hsm-7.0.0.0rc1/ansible_role_thales_hsm.egg-info/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3256 2024-03-15 14:44:44.000000 ansible-role-thales-hsm-7.0.0.0rc1/ansible_role_thales_hsm.egg-info/PKG-INFO
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      788 2024-03-15 14:44:44.000000 ansible-role-thales-hsm-7.0.0.0rc1/ansible_role_thales_hsm.egg-info/SOURCES.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2024-03-15 14:44:44.000000 ansible-role-thales-hsm-7.0.0.0rc1/ansible_role_thales_hsm.egg-info/dependency_links.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2024-03-15 14:44:44.000000 ansible-role-thales-hsm-7.0.0.0rc1/ansible_role_thales_hsm.egg-info/not-zip-safe
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       46 2024-03-15 14:44:44.000000 ansible-role-thales-hsm-7.0.0.0rc1/ansible_role_thales_hsm.egg-info/pbr.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       24 2024-03-15 14:44:44.000000 ansible-role-thales-hsm-7.0.0.0rc1/ansible_role_thales_hsm.egg-info/requires.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2024-03-15 14:44:44.000000 ansible-role-thales-hsm-7.0.0.0rc1/ansible_role_thales_hsm.egg-info/top_level.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-15 14:44:44.066775 ansible-role-thales-hsm-7.0.0.0rc1/defaults/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      166 2024-03-15 14:42:35.000000 ansible-role-thales-hsm-7.0.0.0rc1/defaults/main.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-15 14:44:44.066775 ansible-role-thales-hsm-7.0.0.0rc1/files/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4906 2024-03-15 14:42:35.000000 ansible-role-thales-hsm-7.0.0.0rc1/files/add_ips.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-15 14:44:44.066775 ansible-role-thales-hsm-7.0.0.0rc1/handlers/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      207 2024-03-15 14:42:35.000000 ansible-role-thales-hsm-7.0.0.0rc1/handlers/main.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-15 14:44:44.066775 ansible-role-thales-hsm-7.0.0.0rc1/meta/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      187 2024-03-15 14:42:35.000000 ansible-role-thales-hsm-7.0.0.0rc1/meta/main.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-15 14:44:44.062775 ansible-role-thales-hsm-7.0.0.0rc1/releasenotes/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-15 14:44:44.066775 ansible-role-thales-hsm-7.0.0.0rc1/releasenotes/notes/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      536 2024-03-15 14:42:35.000000 ansible-role-thales-hsm-7.0.0.0rc1/releasenotes/notes/add-ha-c41f45eaa1aba077.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      299 2024-03-15 14:42:35.000000 ansible-role-thales-hsm-7.0.0.0rc1/releasenotes/notes/add-support-for-security-world-v13.4-2cb8688bcc072db1.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       24 2024-03-15 14:42:35.000000 ansible-role-thales-hsm-7.0.0.0rc1/requirements.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      971 2024-03-15 14:44:44.066775 ansible-role-thales-hsm-7.0.0.0rc1/setup.cfg
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      712 2024-03-15 14:42:35.000000 ansible-role-thales-hsm-7.0.0.0rc1/setup.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-15 14:44:44.066775 ansible-role-thales-hsm-7.0.0.0rc1/tasks/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3037 2024-03-15 14:42:35.000000 ansible-role-thales-hsm-7.0.0.0rc1/tasks/client.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      389 2024-03-15 14:42:35.000000 ansible-role-thales-hsm-7.0.0.0rc1/tasks/client_enroll.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      783 2024-03-15 14:42:35.000000 ansible-role-thales-hsm-7.0.0.0rc1/tasks/main.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      352 2024-03-15 14:42:35.000000 ansible-role-thales-hsm-7.0.0.0rc1/tasks/rfs.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      917 2024-03-15 14:42:35.000000 ansible-role-thales-hsm-7.0.0.0rc1/tasks/rfs_register_client.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-15 14:44:44.066775 ansible-role-thales-hsm-7.0.0.0rc1/templates/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      117 2024-03-15 14:42:35.000000 ansible-role-thales-hsm-7.0.0.0rc1/templates/cknfastrc.j2
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       13 2024-03-15 14:42:35.000000 ansible-role-thales-hsm-7.0.0.0rc1/test-requirements.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      209 2024-03-15 14:42:35.000000 ansible-role-thales-hsm-7.0.0.0rc1/tox.ini
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      356 2024-03-15 14:42:35.000000 ansible-role-thales-hsm-7.0.0.0rc1/vars.yaml.sample
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-15 14:44:44.066775 ansible-role-thales-hsm-7.0.0.0rc1/zuul.d/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      196 2024-03-15 14:42:35.000000 ansible-role-thales-hsm-7.0.0.0rc1/zuul.d/layout.yaml
```

### Comparing `ansible-role-thales-hsm-7.0.0/LICENSE` & `ansible-role-thales-hsm-7.0.0.0rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `ansible-role-thales-hsm-7.0.0/PKG-INFO` & `ansible-role-thales-hsm-7.0.0.0rc1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: ansible-role-thales-hsm
-Version: 7.0.0
+Version: 7.0.0.0rc1
 Summary: ansible-role-thales-hsm - Ansible role to configure nShileld Connect HSM clients.
 Home-page: https://opendev.org/openstack/ansible-role-thales-hsm
 Author: TripleO Team
 Author-email: alee@redhat.com
 License: UNKNOWN
 Description: thales-hsm
         ==========
```

### Comparing `ansible-role-thales-hsm-7.0.0/README.rst` & `ansible-role-thales-hsm-7.0.0.0rc1/README.rst`

 * *Files identical despite different names*

### Comparing `ansible-role-thales-hsm-7.0.0/ansible_role_thales_hsm.egg-info/PKG-INFO` & `ansible-role-thales-hsm-7.0.0.0rc1/ansible_role_thales_hsm.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: ansible-role-thales-hsm
-Version: 7.0.0
+Version: 7.0.0.0rc1
 Summary: ansible-role-thales-hsm - Ansible role to configure nShileld Connect HSM clients.
 Home-page: https://opendev.org/openstack/ansible-role-thales-hsm
 Author: TripleO Team
 Author-email: alee@redhat.com
 License: UNKNOWN
 Description: thales-hsm
         ==========
```

### Comparing `ansible-role-thales-hsm-7.0.0/ansible_role_thales_hsm.egg-info/SOURCES.txt` & `ansible-role-thales-hsm-7.0.0.0rc1/ansible_role_thales_hsm.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ansible-role-thales-hsm-7.0.0/files/add_ips.py` & `ansible-role-thales-hsm-7.0.0.0rc1/files/add_ips.py`

 * *Files identical despite different names*

### Comparing `ansible-role-thales-hsm-7.0.0/releasenotes/notes/add-ha-c41f45eaa1aba077.yaml` & `ansible-role-thales-hsm-7.0.0.0rc1/releasenotes/notes/add-ha-c41f45eaa1aba077.yaml`

 * *Files identical despite different names*

### Comparing `ansible-role-thales-hsm-7.0.0/setup.cfg` & `ansible-role-thales-hsm-7.0.0.0rc1/setup.cfg`

 * *Files identical despite different names*

### Comparing `ansible-role-thales-hsm-7.0.0/setup.py` & `ansible-role-thales-hsm-7.0.0.0rc1/setup.py`

 * *Files identical despite different names*

### Comparing `ansible-role-thales-hsm-7.0.0/tasks/client.yaml` & `ansible-role-thales-hsm-7.0.0.0rc1/tasks/client.yaml`

 * *Files identical despite different names*

### Comparing `ansible-role-thales-hsm-7.0.0/tasks/main.yaml` & `ansible-role-thales-hsm-7.0.0.0rc1/tasks/main.yaml`

 * *Files identical despite different names*

### Comparing `ansible-role-thales-hsm-7.0.0/tasks/rfs_register_client.yaml` & `ansible-role-thales-hsm-7.0.0.0rc1/tasks/rfs_register_client.yaml`

 * *Files identical despite different names*

