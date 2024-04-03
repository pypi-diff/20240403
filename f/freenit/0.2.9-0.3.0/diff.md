# Comparing `tmp/freenit-0.2.9.tar.gz` & `tmp/freenit-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "freenit-0.2.9.tar", last modified: Fri Oct 22 20:45:30 2021, max compression
+gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
```

## Comparing `freenit-0.2.9.tar` & `freenit-0.3.0.tar`

### file list

```diff
@@ -1,88 +1,102 @@
-drwxr-xr-x   0 devel     (1001) devel     (1001)        0 2021-10-22 20:45:30.826010 freenit-0.2.9/
--rw-r--r--   0 devel     (1001) devel     (1001)     1322 2021-10-10 11:13:13.000000 freenit-0.2.9/LICENSE
--rw-r--r--   0 devel     (1001) devel     (1001)      118 2021-10-10 11:13:13.000000 freenit-0.2.9/MANIFEST.in
--rw-r--r--   0 devel     (1001) devel     (1001)      764 2021-10-22 20:45:30.825661 freenit-0.2.9/PKG-INFO
--rw-r--r--   0 devel     (1001) devel     (1001)       18 2021-10-10 11:13:13.000000 freenit-0.2.9/README.md
-drwxr-xr-x   0 devel     (1001) devel     (1001)        0 2021-10-22 20:45:30.790199 freenit-0.2.9/alembic/
--rw-r--r--   0 devel     (1001) devel     (1001)       38 2021-10-10 11:13:13.000000 freenit-0.2.9/alembic/README
-drwxr-xr-x   0 devel     (1001) devel     (1001)        0 2021-10-22 20:45:30.790738 freenit-0.2.9/alembic/__pycache__/
--rw-r--r--   0 devel     (1001) devel     (1001)      354 2021-10-15 21:54:03.000000 freenit-0.2.9/alembic/__pycache__/env.cpython-38.pyc
--rw-r--r--   0 devel     (1001) devel     (1001)      250 2021-10-15 21:52:26.000000 freenit-0.2.9/alembic/env.py
--rw-r--r--   0 devel     (1001) devel     (1001)      494 2021-10-10 11:13:13.000000 freenit-0.2.9/alembic/script.py.mako
-drwxr-xr-x   0 devel     (1001) devel     (1001)        0 2021-10-22 20:45:30.791126 freenit-0.2.9/alembic/versions/
-drwxr-xr-x   0 devel     (1001) devel     (1001)        0 2021-10-22 20:45:30.791442 freenit-0.2.9/alembic/versions/__pycache__/
--rw-r--r--   0 devel     (1001) devel     (1001)     1242 2021-10-21 20:24:48.000000 freenit-0.2.9/alembic/versions/__pycache__/a3ffa1d8ccd5_initial.cpython-38.pyc
--rw-r--r--   0 devel     (1001) devel     (1001)     1435 2021-10-19 23:50:16.000000 freenit-0.2.9/alembic/versions/a3ffa1d8ccd5_initial.py
--rw-r--r--   0 devel     (1001) devel     (1001)     2146 2021-10-15 21:54:16.000000 freenit-0.2.9/alembic.ini
-drwxr-xr-x   0 devel     (1001) devel     (1001)        0 2021-10-22 20:45:30.791726 freenit-0.2.9/bin/
--rwxr-xr-x   0 devel     (1001) devel     (1001)     1641 2021-10-10 11:13:13.000000 freenit-0.2.9/bin/freenit.sh
-drwxr-xr-x   0 devel     (1001) devel     (1001)        0 2021-10-22 20:45:30.793790 freenit-0.2.9/freenit/
--rw-r--r--   0 devel     (1001) devel     (1001)        0 2021-10-18 17:33:16.000000 freenit-0.2.9/freenit/__init__.py
-drwxr-xr-x   0 devel     (1001) devel     (1001)        0 2021-10-22 20:45:30.804201 freenit-0.2.9/freenit/api/
--rw-r--r--   0 devel     (1001) devel     (1001)       49 2021-10-22 20:13:12.000000 freenit-0.2.9/freenit/api/__init__.py
--rw-r--r--   0 devel     (1001) devel     (1001)     1302 2021-10-22 20:05:26.000000 freenit-0.2.9/freenit/api/blog.py
--rw-r--r--   0 devel     (1001) devel     (1001)      445 2021-10-15 20:32:27.000000 freenit-0.2.9/freenit/api/router.py
--rw-r--r--   0 devel     (1001) devel     (1001)      690 2021-10-11 18:54:15.000000 freenit-0.2.9/freenit/api/user.py
--rw-r--r--   0 devel     (1001) devel     (1001)      144 2021-10-18 18:11:02.000000 freenit-0.2.9/freenit/app.py
--rw-r--r--   0 devel     (1001) devel     (1001)      292 2021-10-11 19:13:03.000000 freenit-0.2.9/freenit/auth.py
--rw-r--r--   0 devel     (1001) devel     (1001)     1364 2021-10-15 21:23:22.000000 freenit-0.2.9/freenit/base_config.py
--rw-r--r--   0 devel     (1001) devel     (1001)      627 2021-10-18 17:46:45.000000 freenit-0.2.9/freenit/config.py
--rw-r--r--   0 devel     (1001) devel     (1001)     2099 2021-10-18 17:52:21.000000 freenit-0.2.9/freenit/decorators.py
--rw-r--r--   0 devel     (1001) devel     (1001)      861 2021-10-15 21:51:19.000000 freenit-0.2.9/freenit/migration.py
-drwxr-xr-x   0 devel     (1001) devel     (1001)        0 2021-10-22 20:45:30.806317 freenit-0.2.9/freenit/models/
--rw-r--r--   0 devel     (1001) devel     (1001)        0 2021-10-10 11:13:13.000000 freenit-0.2.9/freenit/models/__init__.py
--rw-r--r--   0 devel     (1001) devel     (1001)      267 2021-10-22 20:05:41.000000 freenit-0.2.9/freenit/models/base.py
--rw-r--r--   0 devel     (1001) devel     (1001)      399 2021-10-22 20:11:49.000000 freenit-0.2.9/freenit/models/blog.py
--rw-r--r--   0 devel     (1001) devel     (1001)      600 2021-10-22 19:20:29.000000 freenit-0.2.9/freenit/models/metaclass.py
--rw-r--r--   0 devel     (1001) devel     (1001)     1735 2021-10-15 21:42:57.000000 freenit-0.2.9/freenit/models/user.py
-drwxr-xr-x   0 devel     (1001) devel     (1001)        0 2021-10-22 20:45:30.808779 freenit-0.2.9/freenit/project/
--rw-r--r--   0 devel     (1001) devel     (1001)      219 2021-10-10 11:13:13.000000 freenit-0.2.9/freenit/project/.gitignore
-drwxr-xr-x   0 devel     (1001) devel     (1001)        0 2021-10-22 20:45:30.809193 freenit-0.2.9/freenit/project/alembic/
--rw-r--r--   0 devel     (1001) devel     (1001)      494 2021-10-10 11:13:13.000000 freenit-0.2.9/freenit/project/alembic/script.py.mako
--rw-r--r--   0 devel     (1001) devel     (1001)     2154 2021-10-10 11:13:13.000000 freenit-0.2.9/freenit/project/alembic.ini
-drwxr-xr-x   0 devel     (1001) devel     (1001)        0 2021-10-22 20:45:30.780470 freenit-0.2.9/freenit/project/ansible/
-drwxr-xr-x   0 devel     (1001) devel     (1001)        0 2021-10-22 20:45:30.809634 freenit-0.2.9/freenit/project/ansible/group_vars/
--rw-r--r--   0 devel     (1001) devel     (1001)        1 2021-10-10 11:13:13.000000 freenit-0.2.9/freenit/project/ansible/group_vars/.keep
-drwxr-xr-x   0 devel     (1001) devel     (1001)        0 2021-10-22 20:45:30.810087 freenit-0.2.9/freenit/project/ansible/inventory/
--rw-r--r--   0 devel     (1001) devel     (1001)        0 2021-10-10 11:13:13.000000 freenit-0.2.9/freenit/project/ansible/inventory/.keep
-drwxr-xr-x   0 devel     (1001) devel     (1001)        0 2021-10-22 20:45:30.780588 freenit-0.2.9/freenit/project/ansible/roles/
-drwxr-xr-x   0 devel     (1001) devel     (1001)        0 2021-10-22 20:45:30.780922 freenit-0.2.9/freenit/project/ansible/roles/devel/
-drwxr-xr-x   0 devel     (1001) devel     (1001)        0 2021-10-22 20:45:30.810490 freenit-0.2.9/freenit/project/ansible/roles/devel/tasks/
--rw-r--r--   0 devel     (1001) devel     (1001)      107 2021-10-10 11:13:13.000000 freenit-0.2.9/freenit/project/ansible/roles/devel/tasks/main.yml
-drwxr-xr-x   0 devel     (1001) devel     (1001)        0 2021-10-22 20:45:30.818223 freenit-0.2.9/freenit/project/ansible/roles/devel/vars/
--rw-r--r--   0 devel     (1001) devel     (1001)      100 2021-10-10 11:13:13.000000 freenit-0.2.9/freenit/project/ansible/roles/devel/vars/main.yml
-drwxr-xr-x   0 devel     (1001) devel     (1001)        0 2021-10-22 20:45:30.820714 freenit-0.2.9/freenit/project/bin/
--rw-r--r--   0 devel     (1001) devel     (1001)      928 2021-10-10 11:13:13.000000 freenit-0.2.9/freenit/project/bin/common.sh
--rwxr-xr-x   0 devel     (1001) devel     (1001)      309 2021-10-10 11:13:13.000000 freenit-0.2.9/freenit/project/bin/devel.sh
--rwxr-xr-x   0 devel     (1001) devel     (1001)       95 2021-10-10 11:13:13.000000 freenit-0.2.9/freenit/project/bin/init.sh
--rwxr-xr-x   0 devel     (1001) devel     (1001)       99 2021-10-10 11:13:13.000000 freenit-0.2.9/freenit/project/bin/test.sh
--rw-r--r--   0 devel     (1001) devel     (1001)      393 2021-10-12 21:09:47.000000 freenit-0.2.9/freenit/project/main.py
-drwxr-xr-x   0 devel     (1001) devel     (1001)        0 2021-10-22 20:45:30.823057 freenit-0.2.9/freenit/project/project/
--rw-r--r--   0 devel     (1001) devel     (1001)        0 2021-10-10 11:13:13.000000 freenit-0.2.9/freenit/project/project/__init__.py
-drwxr-xr-x   0 devel     (1001) devel     (1001)        0 2021-10-22 20:45:30.823656 freenit-0.2.9/freenit/project/project/api/
--rw-r--r--   0 devel     (1001) devel     (1001)       48 2021-10-10 11:13:13.000000 freenit-0.2.9/freenit/project/project/api/__init__.py
--rw-r--r--   0 devel     (1001) devel     (1001)       35 2021-10-10 11:13:13.000000 freenit-0.2.9/freenit/project/project/api/router.py
--rw-r--r--   0 devel     (1001) devel     (1001)      150 2021-10-10 11:13:13.000000 freenit-0.2.9/freenit/project/project/app.py
--rw-r--r--   0 devel     (1001) devel     (1001)       35 2021-10-10 11:13:13.000000 freenit-0.2.9/freenit/project/project/config.py
-drwxr-xr-x   0 devel     (1001) devel     (1001)        0 2021-10-22 20:45:30.823955 freenit-0.2.9/freenit/project/project/models/
--rw-r--r--   0 devel     (1001) devel     (1001)        0 2021-10-10 11:13:13.000000 freenit-0.2.9/freenit/project/project/models/__init__.py
--rw-r--r--   0 devel     (1001) devel     (1001)       40 2021-10-10 11:13:13.000000 freenit-0.2.9/freenit/project/provisioners.mk
--rw-r--r--   0 devel     (1001) devel     (1001)       31 2021-10-10 11:13:13.000000 freenit-0.2.9/freenit/project/requirements.yml
--rw-r--r--   0 devel     (1001) devel     (1001)     1303 2021-10-10 11:13:13.000000 freenit-0.2.9/freenit/project/setup.py
-drwxr-xr-x   0 devel     (1001) devel     (1001)        0 2021-10-22 20:45:30.824209 freenit-0.2.9/freenit/project/templates/
--rw-r--r--   0 devel     (1001) devel     (1001)      154 2021-10-10 11:13:13.000000 freenit-0.2.9/freenit/project/templates/site.yml.tpl
--rw-r--r--   0 devel     (1001) devel     (1001)       18 2021-10-22 20:28:23.000000 freenit-0.2.9/freenit/version.py
-drwxr-xr-x   0 devel     (1001) devel     (1001)        0 2021-10-22 20:45:30.802019 freenit-0.2.9/freenit.egg-info/
--rw-r--r--   0 devel     (1001) devel     (1001)      764 2021-10-22 20:45:30.000000 freenit-0.2.9/freenit.egg-info/PKG-INFO
--rw-r--r--   0 devel     (1001) devel     (1001)     1629 2021-10-22 20:45:30.000000 freenit-0.2.9/freenit.egg-info/SOURCES.txt
--rw-r--r--   0 devel     (1001) devel     (1001)        1 2021-10-22 20:45:30.000000 freenit-0.2.9/freenit.egg-info/dependency_links.txt
--rw-r--r--   0 devel     (1001) devel     (1001)      118 2021-10-22 20:45:30.000000 freenit-0.2.9/freenit.egg-info/requires.txt
--rw-r--r--   0 devel     (1001) devel     (1001)        8 2021-10-22 20:45:30.000000 freenit-0.2.9/freenit.egg-info/top_level.txt
--rw-r--r--   0 devel     (1001) devel     (1001)       19 2021-10-10 11:13:13.000000 freenit-0.2.9/name.py
--rw-r--r--   0 devel     (1001) devel     (1001)       38 2021-10-22 20:45:30.826098 freenit-0.2.9/setup.cfg
--rw-r--r--   0 devel     (1001) devel     (1001)     1942 2021-10-15 21:55:19.000000 freenit-0.2.9/setup.py
-drwxr-xr-x   0 devel     (1001) devel     (1001)        0 2021-10-22 20:45:30.825247 freenit-0.2.9/tests/
--rw-r--r--   0 devel     (1001) devel     (1001)        0 2021-10-10 11:13:13.000000 freenit-0.2.9/tests/__init__.py
--rw-r--r--   0 devel     (1001) devel     (1001)      464 2021-10-10 11:13:13.000000 freenit-0.2.9/tests/conftest.py
--rw-r--r--   0 devel     (1001) devel     (1001)      257 2021-10-10 11:13:13.000000 freenit-0.2.9/tests/factories.py
--rw-r--r--   0 devel     (1001) devel     (1001)      373 2021-10-10 11:13:13.000000 freenit-0.2.9/tests/test_user.py
+-rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 freenit-0.3.0/.pylintrc
+-rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 freenit-0.3.0/MANIFEST.in
+-rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 freenit-0.3.0/Makefile
+-rw-r--r--   0        0        0     2146 2020-02-02 00:00:00.000000 freenit-0.3.0/alembic.ini
+-rw-r--r--   0        0        0      402 2020-02-02 00:00:00.000000 freenit-0.3.0/main.py
+-rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 freenit-0.3.0/name.py
+-rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 freenit-0.3.0/provisioners.mk
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 freenit-0.3.0/pytest.ini
+-rw-r--r--   0        0        0      136 2020-02-02 00:00:00.000000 freenit-0.3.0/requirements.yml
+-rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 freenit-0.3.0/setup.cfg
+-rw-r--r--   0        0        0     2435 2020-02-02 00:00:00.000000 freenit-0.3.0/setup.py
+-rw-r--r--   0        0        0      463 2020-02-02 00:00:00.000000 freenit-0.3.0/.github/workflows/pythonapp.yml
+-rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 freenit-0.3.0/alembic/README
+-rw-r--r--   0        0        0      320 2020-02-02 00:00:00.000000 freenit-0.3.0/alembic/env.py
+-rw-r--r--   0        0        0      494 2020-02-02 00:00:00.000000 freenit-0.3.0/alembic/script.py.mako
+-rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 freenit-0.3.0/ansible/group_vars/.keep
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 freenit-0.3.0/ansible/inventory/.keep
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 freenit-0.3.0/ansible/roles/.keep
+-rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 freenit-0.3.0/ansible/roles/devel/tasks/main.yml
+-rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 freenit-0.3.0/ansible/roles/devel/vars/main.yml
+-rwxr-xr-x   0        0        0      202 2020-02-02 00:00:00.000000 freenit-0.3.0/bin/build.sh
+-rw-r--r--   0        0        0     1024 2020-02-02 00:00:00.000000 freenit-0.3.0/bin/common.sh
+-rwxr-xr-x   0        0        0      335 2020-02-02 00:00:00.000000 freenit-0.3.0/bin/devel.sh
+-rwxr-xr-x   0        0        0    12122 2020-02-02 00:00:00.000000 freenit-0.3.0/bin/freenit.sh
+-rwxr-xr-x   0        0        0       95 2020-02-02 00:00:00.000000 freenit-0.3.0/bin/init.sh
+-rwxr-xr-x   0        0        0      183 2020-02-02 00:00:00.000000 freenit-0.3.0/bin/publish.sh
+-rwxr-xr-x   0        0        0      163 2020-02-02 00:00:00.000000 freenit-0.3.0/bin/security.sh
+-rwxr-xr-x   0        0        0      129 2020-02-02 00:00:00.000000 freenit-0.3.0/bin/test.sh
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 freenit-0.3.0/freenit/__init__.py
+-rw-r--r--   0        0        0      446 2020-02-02 00:00:00.000000 freenit-0.3.0/freenit/app.py
+-rw-r--r--   0        0        0     3405 2020-02-02 00:00:00.000000 freenit-0.3.0/freenit/auth.py
+-rw-r--r--   0        0        0     2710 2020-02-02 00:00:00.000000 freenit-0.3.0/freenit/base_config.py
+-rw-r--r--   0        0        0      256 2020-02-02 00:00:00.000000 freenit-0.3.0/freenit/cli.py
+-rw-r--r--   0        0        0      599 2020-02-02 00:00:00.000000 freenit-0.3.0/freenit/config.py
+-rw-r--r--   0        0        0     2087 2020-02-02 00:00:00.000000 freenit-0.3.0/freenit/decorators.py
+-rw-r--r--   0        0        0      399 2020-02-02 00:00:00.000000 freenit-0.3.0/freenit/mail.py
+-rw-r--r--   0        0        0      816 2020-02-02 00:00:00.000000 freenit-0.3.0/freenit/migration.py
+-rw-r--r--   0        0        0      150 2020-02-02 00:00:00.000000 freenit-0.3.0/freenit/permissions.py
+-rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 freenit-0.3.0/freenit/api/__init__.py
+-rw-r--r--   0        0        0     2869 2020-02-02 00:00:00.000000 freenit-0.3.0/freenit/api/auth.py
+-rw-r--r--   0        0        0     3574 2020-02-02 00:00:00.000000 freenit-0.3.0/freenit/api/role.py
+-rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 freenit-0.3.0/freenit/api/router.py
+-rw-r--r--   0        0        0     2681 2020-02-02 00:00:00.000000 freenit-0.3.0/freenit/api/theme.py
+-rw-r--r--   0        0        0     3749 2020-02-02 00:00:00.000000 freenit-0.3.0/freenit/api/user.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 freenit-0.3.0/freenit/models/__init__.py
+-rw-r--r--   0        0        0      876 2020-02-02 00:00:00.000000 freenit-0.3.0/freenit/models/pagination.py
+-rw-r--r--   0        0        0      141 2020-02-02 00:00:00.000000 freenit-0.3.0/freenit/models/role.py
+-rw-r--r--   0        0        0      404 2020-02-02 00:00:00.000000 freenit-0.3.0/freenit/models/safe.py
+-rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 freenit-0.3.0/freenit/models/theme.py
+-rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 freenit-0.3.0/freenit/models/user.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 freenit-0.3.0/freenit/models/ldap/__init__.py
+-rw-r--r--   0        0        0      491 2020-02-02 00:00:00.000000 freenit-0.3.0/freenit/models/ldap/base.py
+-rw-r--r--   0        0        0     1462 2020-02-02 00:00:00.000000 freenit-0.3.0/freenit/models/ldap/user.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 freenit-0.3.0/freenit/models/ormar/__init__.py
+-rw-r--r--   0        0        0     1114 2020-02-02 00:00:00.000000 freenit-0.3.0/freenit/models/ormar/base.py
+-rw-r--r--   0        0        0      208 2020-02-02 00:00:00.000000 freenit-0.3.0/freenit/models/ormar/role.py
+-rw-r--r--   0        0        0      807 2020-02-02 00:00:00.000000 freenit-0.3.0/freenit/models/ormar/theme.py
+-rw-r--r--   0        0        0     1097 2020-02-02 00:00:00.000000 freenit-0.3.0/freenit/models/ormar/user.py
+-rw-r--r--   0        0        0      219 2020-02-02 00:00:00.000000 freenit-0.3.0/freenit/project/.gitignore
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 freenit-0.3.0/freenit/project/LICENSE
+-rw-r--r--   0        0        0     2154 2020-02-02 00:00:00.000000 freenit-0.3.0/freenit/project/alembic.ini
+-rw-r--r--   0        0        0      400 2020-02-02 00:00:00.000000 freenit-0.3.0/freenit/project/main.py
+-rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 freenit-0.3.0/freenit/project/provisioners.mk
+-rw-r--r--   0        0        0      879 2020-02-02 00:00:00.000000 freenit-0.3.0/freenit/project/pyproject.toml
+-rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 freenit-0.3.0/freenit/project/requirements.yml
+-rw-r--r--   0        0        0     1301 2020-02-02 00:00:00.000000 freenit-0.3.0/freenit/project/setup.py
+-rw-r--r--   0        0        0      494 2020-02-02 00:00:00.000000 freenit-0.3.0/freenit/project/alembic/script.py.mako
+-rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 freenit-0.3.0/freenit/project/ansible/group_vars/.keep
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 freenit-0.3.0/freenit/project/ansible/inventory/.keep
+-rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 freenit-0.3.0/freenit/project/ansible/roles/devel/tasks/main.yml
+-rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 freenit-0.3.0/freenit/project/ansible/roles/devel/vars/main.yml
+-rw-r--r--   0        0        0      928 2020-02-02 00:00:00.000000 freenit-0.3.0/freenit/project/bin/common.sh
+-rwxr-xr-x   0        0        0      309 2020-02-02 00:00:00.000000 freenit-0.3.0/freenit/project/bin/devel.sh
+-rwxr-xr-x   0        0        0       95 2020-02-02 00:00:00.000000 freenit-0.3.0/freenit/project/bin/init.sh
+-rwxr-xr-x   0        0        0       99 2020-02-02 00:00:00.000000 freenit-0.3.0/freenit/project/bin/test.sh
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 freenit-0.3.0/freenit/project/project/__init__.py
+-rw-r--r--   0        0        0      446 2020-02-02 00:00:00.000000 freenit-0.3.0/freenit/project/project/app.py
+-rw-r--r--   0        0        0      464 2020-02-02 00:00:00.000000 freenit-0.3.0/freenit/project/project/base_config.py
+-rw-r--r--   0        0        0      623 2020-02-02 00:00:00.000000 freenit-0.3.0/freenit/project/project/config.py
+-rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 freenit-0.3.0/freenit/project/project/api/__init__.py
+-rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 freenit-0.3.0/freenit/project/project/api/router.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 freenit-0.3.0/freenit/project/project/models/__init__.py
+-rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 freenit-0.3.0/freenit/project/templates/site.yml.tpl
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 freenit-0.3.0/freenit/project/tests/__init__.py
+-rw-r--r--   0        0        0     1318 2020-02-02 00:00:00.000000 freenit-0.3.0/freenit/project/tests/client.py
+-rw-r--r--   0        0        0      541 2020-02-02 00:00:00.000000 freenit-0.3.0/freenit/project/tests/conftest.py
+-rw-r--r--   0        0        0      538 2020-02-02 00:00:00.000000 freenit-0.3.0/freenit/project/tests/factories.py
+-rw-r--r--   0        0        0      358 2020-02-02 00:00:00.000000 freenit-0.3.0/freenit/project/tests/test_user.py
+-rw-r--r--   0        0        0      271 2020-02-02 00:00:00.000000 freenit-0.3.0/templates/site.yml.tpl
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 freenit-0.3.0/tests/__init__.py
+-rw-r--r--   0        0        0     1185 2020-02-02 00:00:00.000000 freenit-0.3.0/tests/client.py
+-rw-r--r--   0        0        0      541 2020-02-02 00:00:00.000000 freenit-0.3.0/tests/conftest.py
+-rw-r--r--   0        0        0      538 2020-02-02 00:00:00.000000 freenit-0.3.0/tests/factories.py
+-rw-r--r--   0        0        0      787 2020-02-02 00:00:00.000000 freenit-0.3.0/tests/test_auth.py
+-rw-r--r--   0        0        0     2157 2020-02-02 00:00:00.000000 freenit-0.3.0/tests/test_permission.py
+-rw-r--r--   0        0        0     2281 2020-02-02 00:00:00.000000 freenit-0.3.0/tests/test_role.py
+-rw-r--r--   0        0        0     1944 2020-02-02 00:00:00.000000 freenit-0.3.0/tests/test_user.py
+-rw-r--r--   0        0        0      312 2020-02-02 00:00:00.000000 freenit-0.3.0/.gitignore
+-rw-r--r--   0        0        0     1322 2020-02-02 00:00:00.000000 freenit-0.3.0/LICENSE
+-rw-r--r--   0        0        0      377 2020-02-02 00:00:00.000000 freenit-0.3.0/README.md
+-rw-r--r--   0        0        0     1287 2020-02-02 00:00:00.000000 freenit-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     3309 2020-02-02 00:00:00.000000 freenit-0.3.0/PKG-INFO
```

### Comparing `freenit-0.2.9/LICENSE` & `freenit-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `freenit-0.2.9/alembic.ini` & `freenit-0.3.0/alembic.ini`

 * *Files identical despite different names*

### Comparing `freenit-0.2.9/freenit/config.py` & `freenit-0.3.0/freenit/project/project/config.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 import os
 
+from freenit.config import configs
+
 try:
     from .local_config import DevConfig
 except ImportError:
     from .base_config import DevConfig
 
 try:
     from .local_config import TestConfig
@@ -11,16 +13,16 @@
     from .base_config import TestConfig
 
 try:
     from .local_config import ProdConfig
 except ImportError:
     from .base_config import ProdConfig
 
-configs = {}
+
 configs[DevConfig.envname()] = DevConfig()
 configs[TestConfig.envname()] = TestConfig()
 configs[ProdConfig.envname()] = ProdConfig()
 
 
 def getConfig():
-    config_name = os.getenv("FREENIT_ENV", ProdConfig.envname())
-    return configs.get(config_name, configs[ProdConfig.envname()])
+    config_name = os.getenv("FREENIT_ENV", "prod")
+    return configs.get(config_name, configs["prod"])
```

### Comparing `freenit-0.2.9/freenit/project/alembic.ini` & `freenit-0.3.0/freenit/project/alembic.ini`

 * *Files identical despite different names*

### Comparing `freenit-0.2.9/freenit/project/bin/common.sh` & `freenit-0.3.0/freenit/project/bin/common.sh`

 * *Files 2% similar despite different names*

```diff
@@ -6,26 +6,26 @@
 . "${PROJECT_ROOT}/name.py"
 export VIRTUALENV=${VIRTUALENV:="${app_name}"}
 export FREENIT_ENV=${FREENIT_ENV:="prod"}
 export SYSPKG=${SYSPKG:="no"}
 
 
 setup() {
-  if [ "${SYSPKG}" = "no" ]; then
+  cd ${PROJECT_ROOT}
+  if [ "${SYSPKG}" != "YES" ]; then
     update=${1}
     if [ ! -d ${HOME}/.virtualenvs/${VIRTUALENV} ]; then
         python${PY_VERSION} -m venv "${HOME}/.virtualenvs/${VIRTUALENV}"
     fi
     . ${HOME}/.virtualenvs/${VIRTUALENV}/bin/activate
 
     INSTALL_TARGET=".[${FREENIT_ENV}]"
     if [ "${FREENIT_ENV}" = "prod" ]; then
       INSTALL_TARGET="."
     fi
-    cd ${PROJECT_ROOT}
     if [ "${update}" != "no" ]; then
       pip install -U pip
       pip install -U wheel
       pip install -U --upgrade-strategy eager -e "${INSTALL_TARGET}"
     fi
   fi
```

### Comparing `freenit-0.2.9/freenit/project/setup.py` & `freenit-0.3.0/freenit/project/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,51 +1,46 @@
 #!/usr/bin/env python
 
 import pathlib
 
 from setuptools import find_packages, setup
 
 PROJECT_ROOT = pathlib.Path(__file__).parent
-README = (PROJECT_ROOT / 'README.md').read_text()
+README = (PROJECT_ROOT / "README.md").read_text()
 
 setup(
-    name='NAME',
-    version='0.0.1',
-    description='REST API framework based on FastAPI',
+    name="NAME",
+    version="0.0.1",
+    description="REST API based on Freenit",
     long_description=README,
-    long_description_content_type='text/markdown',
-    url='https://github.com/freenit-framework/backend',
-    author='Goran Mekić',
-    author_email='meka@tilda.center',
-    license='BSD',
+    long_description_content_type="text/markdown",
+    url="https://github.com/organization/backend",
+    author="John Doe",
+    author_email="john@example.com",
+    license="BSD",
     classifiers=[
-        'Development Status :: 4 - Beta',
-        'Intended Audience :: Developers',
-        'Topic :: Internet :: WWW/HTTP',
-        'Environment :: Web Environment',
-        'Framework :: FastAPI',
-        'License :: OSI Approved :: BSD License',
-        'Programming Language :: Python :: 3.8',
-        'Programming Language :: Python :: 3.9',
+        "Development Status :: 4 - Beta",
+        "Intended Audience :: Developers",
+        "Topic :: Internet :: WWW/HTTP",
+        "Environment :: Web Environment",
+        "Framework :: FastAPI",
+        "License :: OSI Approved :: BSD License",
+        "Programming Language :: Python :: 3.8",
+        "Programming Language :: Python :: 3.9",
+        "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
     ],
     keywords=[
-        'REST',
-        'openapi',
-        'swagger',
-        'fastapi',
+        "REST",
+        "openapi",
+        "swagger",
+        "fastapi",
     ],
-    packages=find_packages(exclude=['tests*']),
-    python_requires='>=3.8',
-    install_requires=['freenit'],
+    packages=find_packages(exclude=["tests*"]),
+    python_requires=">=3.8",
+    install_requires=["freenit[ormar]"],
     extras_require={
-        'build': [
-            'twine',
-        ],
-        'dev': [
-            'uvicorn',
-        ],
-        'test': [
-            'pytest-asyncio',
-            'pytest-factoryboy',
-        ],
+        "build": ["freenit[build]"],
+        "dev": ["freenit[dev]"],
+        "test": ["freenit[test]"],
     },
 )
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

