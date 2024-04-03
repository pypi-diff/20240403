# Comparing `tmp/ansible-role-atos-hsm-7.0.0.tar.gz` & `tmp/ansible-role-atos-hsm-7.0.0.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ansible-role-atos-hsm-7.0.0.tar", last modified: Wed Apr  3 11:08:30 2024, max compression
+gzip compressed data, was "ansible-role-atos-hsm-7.0.0.0rc1.tar", last modified: Fri Mar 15 14:33:14 2024, max compression
```

## Comparing `ansible-role-atos-hsm-7.0.0.tar` & `ansible-role-atos-hsm-7.0.0.0rc1.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:08:30.046105 ansible-role-atos-hsm-7.0.0/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       94 2024-04-03 11:08:02.000000 ansible-role-atos-hsm-7.0.0/.ansible-lint
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       68 2024-04-03 11:08:02.000000 ansible-role-atos-hsm-7.0.0/AUTHORS
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    11358 2024-04-03 11:08:02.000000 ansible-role-atos-hsm-7.0.0/LICENSE
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2566 2024-04-03 11:08:30.046105 ansible-role-atos-hsm-7.0.0/PKG-INFO
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1488 2024-04-03 11:08:02.000000 ansible-role-atos-hsm-7.0.0/README.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:08:30.046105 ansible-role-atos-hsm-7.0.0/ansible_role_atos_hsm.egg-info/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2566 2024-04-03 11:08:29.000000 ansible-role-atos-hsm-7.0.0/ansible_role_atos_hsm.egg-info/PKG-INFO
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      601 2024-04-03 11:08:30.000000 ansible-role-atos-hsm-7.0.0/ansible_role_atos_hsm.egg-info/SOURCES.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2024-04-03 11:08:29.000000 ansible-role-atos-hsm-7.0.0/ansible_role_atos_hsm.egg-info/dependency_links.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2024-04-03 11:08:29.000000 ansible-role-atos-hsm-7.0.0/ansible_role_atos_hsm.egg-info/not-zip-safe
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       46 2024-04-03 11:08:29.000000 ansible-role-atos-hsm-7.0.0/ansible_role_atos_hsm.egg-info/pbr.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       17 2024-04-03 11:08:29.000000 ansible-role-atos-hsm-7.0.0/ansible_role_atos_hsm.egg-info/requires.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2024-04-03 11:08:29.000000 ansible-role-atos-hsm-7.0.0/ansible_role_atos_hsm.egg-info/top_level.txt
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:08:30.046105 ansible-role-atos-hsm-7.0.0/defaults/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       54 2024-04-03 11:08:02.000000 ansible-role-atos-hsm-7.0.0/defaults/main.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:08:30.046105 ansible-role-atos-hsm-7.0.0/handlers/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      192 2024-04-03 11:08:02.000000 ansible-role-atos-hsm-7.0.0/handlers/main.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:08:30.042105 ansible-role-atos-hsm-7.0.0/releasenotes/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:08:30.046105 ansible-role-atos-hsm-7.0.0/releasenotes/notes/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      505 2024-04-03 11:08:02.000000 ansible-role-atos-hsm-7.0.0/releasenotes/notes/add-high-availability-support-44343eaf5563f5c7.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       17 2024-04-03 11:08:02.000000 ansible-role-atos-hsm-7.0.0/requirements.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      954 2024-04-03 11:08:30.050105 ansible-role-atos-hsm-7.0.0/setup.cfg
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      712 2024-04-03 11:08:02.000000 ansible-role-atos-hsm-7.0.0/setup.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:08:30.046105 ansible-role-atos-hsm-7.0.0/tasks/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2285 2024-04-03 11:08:02.000000 ansible-role-atos-hsm-7.0.0/tasks/main.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:08:30.046105 ansible-role-atos-hsm-7.0.0/templates/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      312 2024-04-03 11:08:02.000000 ansible-role-atos-hsm-7.0.0/templates/proteccio.rc.j2
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       18 2024-04-03 11:08:02.000000 ansible-role-atos-hsm-7.0.0/test-requirements.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      167 2024-04-03 11:08:02.000000 ansible-role-atos-hsm-7.0.0/tox.ini
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      692 2024-04-03 11:08:02.000000 ansible-role-atos-hsm-7.0.0/vars.yaml.sample
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:08:30.046105 ansible-role-atos-hsm-7.0.0/zuul.d/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      196 2024-04-03 11:08:02.000000 ansible-role-atos-hsm-7.0.0/zuul.d/layout.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-15 14:33:14.903746 ansible-role-atos-hsm-7.0.0.0rc1/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       94 2024-03-15 14:32:33.000000 ansible-role-atos-hsm-7.0.0.0rc1/.ansible-lint
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       68 2024-03-15 14:32:33.000000 ansible-role-atos-hsm-7.0.0.0rc1/AUTHORS
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    11358 2024-03-15 14:32:33.000000 ansible-role-atos-hsm-7.0.0.0rc1/LICENSE
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2571 2024-03-15 14:33:14.903746 ansible-role-atos-hsm-7.0.0.0rc1/PKG-INFO
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1488 2024-03-15 14:32:33.000000 ansible-role-atos-hsm-7.0.0.0rc1/README.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-15 14:33:14.899747 ansible-role-atos-hsm-7.0.0.0rc1/ansible_role_atos_hsm.egg-info/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2571 2024-03-15 14:33:14.000000 ansible-role-atos-hsm-7.0.0.0rc1/ansible_role_atos_hsm.egg-info/PKG-INFO
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      601 2024-03-15 14:33:14.000000 ansible-role-atos-hsm-7.0.0.0rc1/ansible_role_atos_hsm.egg-info/SOURCES.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2024-03-15 14:33:14.000000 ansible-role-atos-hsm-7.0.0.0rc1/ansible_role_atos_hsm.egg-info/dependency_links.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2024-03-15 14:33:14.000000 ansible-role-atos-hsm-7.0.0.0rc1/ansible_role_atos_hsm.egg-info/not-zip-safe
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       46 2024-03-15 14:33:14.000000 ansible-role-atos-hsm-7.0.0.0rc1/ansible_role_atos_hsm.egg-info/pbr.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       17 2024-03-15 14:33:14.000000 ansible-role-atos-hsm-7.0.0.0rc1/ansible_role_atos_hsm.egg-info/requires.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2024-03-15 14:33:14.000000 ansible-role-atos-hsm-7.0.0.0rc1/ansible_role_atos_hsm.egg-info/top_level.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-15 14:33:14.899747 ansible-role-atos-hsm-7.0.0.0rc1/defaults/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       54 2024-03-15 14:32:33.000000 ansible-role-atos-hsm-7.0.0.0rc1/defaults/main.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-15 14:33:14.899747 ansible-role-atos-hsm-7.0.0.0rc1/handlers/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      192 2024-03-15 14:32:33.000000 ansible-role-atos-hsm-7.0.0.0rc1/handlers/main.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-15 14:33:14.895747 ansible-role-atos-hsm-7.0.0.0rc1/releasenotes/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-15 14:33:14.899747 ansible-role-atos-hsm-7.0.0.0rc1/releasenotes/notes/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      505 2024-03-15 14:32:33.000000 ansible-role-atos-hsm-7.0.0.0rc1/releasenotes/notes/add-high-availability-support-44343eaf5563f5c7.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       17 2024-03-15 14:32:33.000000 ansible-role-atos-hsm-7.0.0.0rc1/requirements.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      954 2024-03-15 14:33:14.903746 ansible-role-atos-hsm-7.0.0.0rc1/setup.cfg
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      712 2024-03-15 14:32:33.000000 ansible-role-atos-hsm-7.0.0.0rc1/setup.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-15 14:33:14.899747 ansible-role-atos-hsm-7.0.0.0rc1/tasks/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2285 2024-03-15 14:32:33.000000 ansible-role-atos-hsm-7.0.0.0rc1/tasks/main.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-15 14:33:14.899747 ansible-role-atos-hsm-7.0.0.0rc1/templates/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      312 2024-03-15 14:32:33.000000 ansible-role-atos-hsm-7.0.0.0rc1/templates/proteccio.rc.j2
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       18 2024-03-15 14:32:33.000000 ansible-role-atos-hsm-7.0.0.0rc1/test-requirements.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      167 2024-03-15 14:32:33.000000 ansible-role-atos-hsm-7.0.0.0rc1/tox.ini
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      692 2024-03-15 14:32:33.000000 ansible-role-atos-hsm-7.0.0.0rc1/vars.yaml.sample
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-15 14:33:14.903746 ansible-role-atos-hsm-7.0.0.0rc1/zuul.d/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      196 2024-03-15 14:32:33.000000 ansible-role-atos-hsm-7.0.0.0rc1/zuul.d/layout.yaml
```

### Comparing `ansible-role-atos-hsm-7.0.0/LICENSE` & `ansible-role-atos-hsm-7.0.0.0rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `ansible-role-atos-hsm-7.0.0/PKG-INFO` & `ansible-role-atos-hsm-7.0.0.0rc1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: ansible-role-atos-hsm
-Version: 7.0.0
+Version: 7.0.0.0rc1
 Summary: ansible-role-atos-hsm - Ansible role to configure ATOS HSM clients.
 Home-page: https://opendev.org/openstack/ansible-role-atos-hsm
 Author: OpenStack Barbican Team
 Author-email: alee@redhat.com
 License: UNKNOWN
 Description: atos-hsm
         ========
```

### Comparing `ansible-role-atos-hsm-7.0.0/README.rst` & `ansible-role-atos-hsm-7.0.0.0rc1/README.rst`

 * *Files identical despite different names*

### Comparing `ansible-role-atos-hsm-7.0.0/ansible_role_atos_hsm.egg-info/PKG-INFO` & `ansible-role-atos-hsm-7.0.0.0rc1/ansible_role_atos_hsm.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: ansible-role-atos-hsm
-Version: 7.0.0
+Version: 7.0.0.0rc1
 Summary: ansible-role-atos-hsm - Ansible role to configure ATOS HSM clients.
 Home-page: https://opendev.org/openstack/ansible-role-atos-hsm
 Author: OpenStack Barbican Team
 Author-email: alee@redhat.com
 License: UNKNOWN
 Description: atos-hsm
         ========
```

### Comparing `ansible-role-atos-hsm-7.0.0/ansible_role_atos_hsm.egg-info/SOURCES.txt` & `ansible-role-atos-hsm-7.0.0.0rc1/ansible_role_atos_hsm.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ansible-role-atos-hsm-7.0.0/setup.cfg` & `ansible-role-atos-hsm-7.0.0.0rc1/setup.cfg`

 * *Files identical despite different names*

### Comparing `ansible-role-atos-hsm-7.0.0/setup.py` & `ansible-role-atos-hsm-7.0.0.0rc1/setup.py`

 * *Files identical despite different names*

### Comparing `ansible-role-atos-hsm-7.0.0/tasks/main.yaml` & `ansible-role-atos-hsm-7.0.0.0rc1/tasks/main.yaml`

 * *Files identical despite different names*

### Comparing `ansible-role-atos-hsm-7.0.0/vars.yaml.sample` & `ansible-role-atos-hsm-7.0.0.0rc1/vars.yaml.sample`

 * *Files identical despite different names*

