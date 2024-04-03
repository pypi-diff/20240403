# Comparing `tmp/freenit-0.3.0.tar.gz` & `tmp/freenit-0.3.1.tar.gz`

## Comparing `freenit-0.3.0.tar` & `freenit-0.3.1.tar`

### file list

```diff
@@ -1,102 +1,103 @@
--rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 freenit-0.3.0/.pylintrc
--rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 freenit-0.3.0/MANIFEST.in
--rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 freenit-0.3.0/Makefile
--rw-r--r--   0        0        0     2146 2020-02-02 00:00:00.000000 freenit-0.3.0/alembic.ini
--rw-r--r--   0        0        0      402 2020-02-02 00:00:00.000000 freenit-0.3.0/main.py
--rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 freenit-0.3.0/name.py
--rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 freenit-0.3.0/provisioners.mk
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 freenit-0.3.0/pytest.ini
--rw-r--r--   0        0        0      136 2020-02-02 00:00:00.000000 freenit-0.3.0/requirements.yml
--rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 freenit-0.3.0/setup.cfg
--rw-r--r--   0        0        0     2435 2020-02-02 00:00:00.000000 freenit-0.3.0/setup.py
--rw-r--r--   0        0        0      463 2020-02-02 00:00:00.000000 freenit-0.3.0/.github/workflows/pythonapp.yml
--rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 freenit-0.3.0/alembic/README
--rw-r--r--   0        0        0      320 2020-02-02 00:00:00.000000 freenit-0.3.0/alembic/env.py
--rw-r--r--   0        0        0      494 2020-02-02 00:00:00.000000 freenit-0.3.0/alembic/script.py.mako
--rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 freenit-0.3.0/ansible/group_vars/.keep
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 freenit-0.3.0/ansible/inventory/.keep
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 freenit-0.3.0/ansible/roles/.keep
--rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 freenit-0.3.0/ansible/roles/devel/tasks/main.yml
--rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 freenit-0.3.0/ansible/roles/devel/vars/main.yml
--rwxr-xr-x   0        0        0      202 2020-02-02 00:00:00.000000 freenit-0.3.0/bin/build.sh
--rw-r--r--   0        0        0     1024 2020-02-02 00:00:00.000000 freenit-0.3.0/bin/common.sh
--rwxr-xr-x   0        0        0      335 2020-02-02 00:00:00.000000 freenit-0.3.0/bin/devel.sh
--rwxr-xr-x   0        0        0    12122 2020-02-02 00:00:00.000000 freenit-0.3.0/bin/freenit.sh
--rwxr-xr-x   0        0        0       95 2020-02-02 00:00:00.000000 freenit-0.3.0/bin/init.sh
--rwxr-xr-x   0        0        0      183 2020-02-02 00:00:00.000000 freenit-0.3.0/bin/publish.sh
--rwxr-xr-x   0        0        0      163 2020-02-02 00:00:00.000000 freenit-0.3.0/bin/security.sh
--rwxr-xr-x   0        0        0      129 2020-02-02 00:00:00.000000 freenit-0.3.0/bin/test.sh
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 freenit-0.3.0/freenit/__init__.py
--rw-r--r--   0        0        0      446 2020-02-02 00:00:00.000000 freenit-0.3.0/freenit/app.py
--rw-r--r--   0        0        0     3405 2020-02-02 00:00:00.000000 freenit-0.3.0/freenit/auth.py
--rw-r--r--   0        0        0     2710 2020-02-02 00:00:00.000000 freenit-0.3.0/freenit/base_config.py
--rw-r--r--   0        0        0      256 2020-02-02 00:00:00.000000 freenit-0.3.0/freenit/cli.py
--rw-r--r--   0        0        0      599 2020-02-02 00:00:00.000000 freenit-0.3.0/freenit/config.py
--rw-r--r--   0        0        0     2087 2020-02-02 00:00:00.000000 freenit-0.3.0/freenit/decorators.py
--rw-r--r--   0        0        0      399 2020-02-02 00:00:00.000000 freenit-0.3.0/freenit/mail.py
--rw-r--r--   0        0        0      816 2020-02-02 00:00:00.000000 freenit-0.3.0/freenit/migration.py
--rw-r--r--   0        0        0      150 2020-02-02 00:00:00.000000 freenit-0.3.0/freenit/permissions.py
--rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 freenit-0.3.0/freenit/api/__init__.py
--rw-r--r--   0        0        0     2869 2020-02-02 00:00:00.000000 freenit-0.3.0/freenit/api/auth.py
--rw-r--r--   0        0        0     3574 2020-02-02 00:00:00.000000 freenit-0.3.0/freenit/api/role.py
--rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 freenit-0.3.0/freenit/api/router.py
--rw-r--r--   0        0        0     2681 2020-02-02 00:00:00.000000 freenit-0.3.0/freenit/api/theme.py
--rw-r--r--   0        0        0     3749 2020-02-02 00:00:00.000000 freenit-0.3.0/freenit/api/user.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 freenit-0.3.0/freenit/models/__init__.py
--rw-r--r--   0        0        0      876 2020-02-02 00:00:00.000000 freenit-0.3.0/freenit/models/pagination.py
--rw-r--r--   0        0        0      141 2020-02-02 00:00:00.000000 freenit-0.3.0/freenit/models/role.py
--rw-r--r--   0        0        0      404 2020-02-02 00:00:00.000000 freenit-0.3.0/freenit/models/safe.py
--rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 freenit-0.3.0/freenit/models/theme.py
--rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 freenit-0.3.0/freenit/models/user.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 freenit-0.3.0/freenit/models/ldap/__init__.py
--rw-r--r--   0        0        0      491 2020-02-02 00:00:00.000000 freenit-0.3.0/freenit/models/ldap/base.py
--rw-r--r--   0        0        0     1462 2020-02-02 00:00:00.000000 freenit-0.3.0/freenit/models/ldap/user.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 freenit-0.3.0/freenit/models/ormar/__init__.py
--rw-r--r--   0        0        0     1114 2020-02-02 00:00:00.000000 freenit-0.3.0/freenit/models/ormar/base.py
--rw-r--r--   0        0        0      208 2020-02-02 00:00:00.000000 freenit-0.3.0/freenit/models/ormar/role.py
--rw-r--r--   0        0        0      807 2020-02-02 00:00:00.000000 freenit-0.3.0/freenit/models/ormar/theme.py
--rw-r--r--   0        0        0     1097 2020-02-02 00:00:00.000000 freenit-0.3.0/freenit/models/ormar/user.py
--rw-r--r--   0        0        0      219 2020-02-02 00:00:00.000000 freenit-0.3.0/freenit/project/.gitignore
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 freenit-0.3.0/freenit/project/LICENSE
--rw-r--r--   0        0        0     2154 2020-02-02 00:00:00.000000 freenit-0.3.0/freenit/project/alembic.ini
--rw-r--r--   0        0        0      400 2020-02-02 00:00:00.000000 freenit-0.3.0/freenit/project/main.py
--rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 freenit-0.3.0/freenit/project/provisioners.mk
--rw-r--r--   0        0        0      879 2020-02-02 00:00:00.000000 freenit-0.3.0/freenit/project/pyproject.toml
--rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 freenit-0.3.0/freenit/project/requirements.yml
--rw-r--r--   0        0        0     1301 2020-02-02 00:00:00.000000 freenit-0.3.0/freenit/project/setup.py
--rw-r--r--   0        0        0      494 2020-02-02 00:00:00.000000 freenit-0.3.0/freenit/project/alembic/script.py.mako
--rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 freenit-0.3.0/freenit/project/ansible/group_vars/.keep
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 freenit-0.3.0/freenit/project/ansible/inventory/.keep
--rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 freenit-0.3.0/freenit/project/ansible/roles/devel/tasks/main.yml
--rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 freenit-0.3.0/freenit/project/ansible/roles/devel/vars/main.yml
--rw-r--r--   0        0        0      928 2020-02-02 00:00:00.000000 freenit-0.3.0/freenit/project/bin/common.sh
--rwxr-xr-x   0        0        0      309 2020-02-02 00:00:00.000000 freenit-0.3.0/freenit/project/bin/devel.sh
--rwxr-xr-x   0        0        0       95 2020-02-02 00:00:00.000000 freenit-0.3.0/freenit/project/bin/init.sh
--rwxr-xr-x   0        0        0       99 2020-02-02 00:00:00.000000 freenit-0.3.0/freenit/project/bin/test.sh
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 freenit-0.3.0/freenit/project/project/__init__.py
--rw-r--r--   0        0        0      446 2020-02-02 00:00:00.000000 freenit-0.3.0/freenit/project/project/app.py
--rw-r--r--   0        0        0      464 2020-02-02 00:00:00.000000 freenit-0.3.0/freenit/project/project/base_config.py
--rw-r--r--   0        0        0      623 2020-02-02 00:00:00.000000 freenit-0.3.0/freenit/project/project/config.py
--rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 freenit-0.3.0/freenit/project/project/api/__init__.py
--rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 freenit-0.3.0/freenit/project/project/api/router.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 freenit-0.3.0/freenit/project/project/models/__init__.py
--rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 freenit-0.3.0/freenit/project/templates/site.yml.tpl
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 freenit-0.3.0/freenit/project/tests/__init__.py
--rw-r--r--   0        0        0     1318 2020-02-02 00:00:00.000000 freenit-0.3.0/freenit/project/tests/client.py
--rw-r--r--   0        0        0      541 2020-02-02 00:00:00.000000 freenit-0.3.0/freenit/project/tests/conftest.py
--rw-r--r--   0        0        0      538 2020-02-02 00:00:00.000000 freenit-0.3.0/freenit/project/tests/factories.py
--rw-r--r--   0        0        0      358 2020-02-02 00:00:00.000000 freenit-0.3.0/freenit/project/tests/test_user.py
--rw-r--r--   0        0        0      271 2020-02-02 00:00:00.000000 freenit-0.3.0/templates/site.yml.tpl
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 freenit-0.3.0/tests/__init__.py
--rw-r--r--   0        0        0     1185 2020-02-02 00:00:00.000000 freenit-0.3.0/tests/client.py
--rw-r--r--   0        0        0      541 2020-02-02 00:00:00.000000 freenit-0.3.0/tests/conftest.py
--rw-r--r--   0        0        0      538 2020-02-02 00:00:00.000000 freenit-0.3.0/tests/factories.py
--rw-r--r--   0        0        0      787 2020-02-02 00:00:00.000000 freenit-0.3.0/tests/test_auth.py
--rw-r--r--   0        0        0     2157 2020-02-02 00:00:00.000000 freenit-0.3.0/tests/test_permission.py
--rw-r--r--   0        0        0     2281 2020-02-02 00:00:00.000000 freenit-0.3.0/tests/test_role.py
--rw-r--r--   0        0        0     1944 2020-02-02 00:00:00.000000 freenit-0.3.0/tests/test_user.py
--rw-r--r--   0        0        0      312 2020-02-02 00:00:00.000000 freenit-0.3.0/.gitignore
--rw-r--r--   0        0        0     1322 2020-02-02 00:00:00.000000 freenit-0.3.0/LICENSE
--rw-r--r--   0        0        0      377 2020-02-02 00:00:00.000000 freenit-0.3.0/README.md
--rw-r--r--   0        0        0     1287 2020-02-02 00:00:00.000000 freenit-0.3.0/pyproject.toml
--rw-r--r--   0        0        0     3309 2020-02-02 00:00:00.000000 freenit-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 freenit-0.3.1/.pylintrc
+-rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 freenit-0.3.1/MANIFEST.in
+-rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 freenit-0.3.1/Makefile
+-rw-r--r--   0        0        0     2146 2020-02-02 00:00:00.000000 freenit-0.3.1/alembic.ini
+-rw-r--r--   0        0        0      402 2020-02-02 00:00:00.000000 freenit-0.3.1/main.py
+-rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 freenit-0.3.1/name.py
+-rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 freenit-0.3.1/provisioners.mk
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 freenit-0.3.1/pytest.ini
+-rw-r--r--   0        0        0      136 2020-02-02 00:00:00.000000 freenit-0.3.1/requirements.yml
+-rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 freenit-0.3.1/setup.cfg
+-rw-r--r--   0        0        0     2435 2020-02-02 00:00:00.000000 freenit-0.3.1/setup.py
+-rw-r--r--   0        0        0      463 2020-02-02 00:00:00.000000 freenit-0.3.1/.github/workflows/pythonapp.yml
+-rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 freenit-0.3.1/alembic/README
+-rw-r--r--   0        0        0      320 2020-02-02 00:00:00.000000 freenit-0.3.1/alembic/env.py
+-rw-r--r--   0        0        0      494 2020-02-02 00:00:00.000000 freenit-0.3.1/alembic/script.py.mako
+-rw-r--r--   0        0        0     3029 2020-02-02 00:00:00.000000 freenit-0.3.1/alembic/versions/06a043f2516a_initial.py
+-rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 freenit-0.3.1/ansible/group_vars/.keep
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 freenit-0.3.1/ansible/inventory/.keep
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 freenit-0.3.1/ansible/roles/.keep
+-rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 freenit-0.3.1/ansible/roles/devel/tasks/main.yml
+-rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 freenit-0.3.1/ansible/roles/devel/vars/main.yml
+-rwxr-xr-x   0        0        0      202 2020-02-02 00:00:00.000000 freenit-0.3.1/bin/build.sh
+-rw-r--r--   0        0        0     1024 2020-02-02 00:00:00.000000 freenit-0.3.1/bin/common.sh
+-rwxr-xr-x   0        0        0      335 2020-02-02 00:00:00.000000 freenit-0.3.1/bin/devel.sh
+-rwxr-xr-x   0        0        0    12122 2020-02-02 00:00:00.000000 freenit-0.3.1/bin/freenit.sh
+-rwxr-xr-x   0        0        0       95 2020-02-02 00:00:00.000000 freenit-0.3.1/bin/init.sh
+-rwxr-xr-x   0        0        0      183 2020-02-02 00:00:00.000000 freenit-0.3.1/bin/publish.sh
+-rwxr-xr-x   0        0        0      163 2020-02-02 00:00:00.000000 freenit-0.3.1/bin/security.sh
+-rwxr-xr-x   0        0        0      129 2020-02-02 00:00:00.000000 freenit-0.3.1/bin/test.sh
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 freenit-0.3.1/freenit/__init__.py
+-rw-r--r--   0        0        0      446 2020-02-02 00:00:00.000000 freenit-0.3.1/freenit/app.py
+-rw-r--r--   0        0        0     3405 2020-02-02 00:00:00.000000 freenit-0.3.1/freenit/auth.py
+-rw-r--r--   0        0        0     2710 2020-02-02 00:00:00.000000 freenit-0.3.1/freenit/base_config.py
+-rw-r--r--   0        0        0      256 2020-02-02 00:00:00.000000 freenit-0.3.1/freenit/cli.py
+-rw-r--r--   0        0        0      599 2020-02-02 00:00:00.000000 freenit-0.3.1/freenit/config.py
+-rw-r--r--   0        0        0     2087 2020-02-02 00:00:00.000000 freenit-0.3.1/freenit/decorators.py
+-rw-r--r--   0        0        0      399 2020-02-02 00:00:00.000000 freenit-0.3.1/freenit/mail.py
+-rw-r--r--   0        0        0      816 2020-02-02 00:00:00.000000 freenit-0.3.1/freenit/migration.py
+-rw-r--r--   0        0        0      150 2020-02-02 00:00:00.000000 freenit-0.3.1/freenit/permissions.py
+-rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 freenit-0.3.1/freenit/api/__init__.py
+-rw-r--r--   0        0        0     2869 2020-02-02 00:00:00.000000 freenit-0.3.1/freenit/api/auth.py
+-rw-r--r--   0        0        0     3574 2020-02-02 00:00:00.000000 freenit-0.3.1/freenit/api/role.py
+-rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 freenit-0.3.1/freenit/api/router.py
+-rw-r--r--   0        0        0     2681 2020-02-02 00:00:00.000000 freenit-0.3.1/freenit/api/theme.py
+-rw-r--r--   0        0        0     3749 2020-02-02 00:00:00.000000 freenit-0.3.1/freenit/api/user.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 freenit-0.3.1/freenit/models/__init__.py
+-rw-r--r--   0        0        0      876 2020-02-02 00:00:00.000000 freenit-0.3.1/freenit/models/pagination.py
+-rw-r--r--   0        0        0      141 2020-02-02 00:00:00.000000 freenit-0.3.1/freenit/models/role.py
+-rw-r--r--   0        0        0      404 2020-02-02 00:00:00.000000 freenit-0.3.1/freenit/models/safe.py
+-rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 freenit-0.3.1/freenit/models/theme.py
+-rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 freenit-0.3.1/freenit/models/user.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 freenit-0.3.1/freenit/models/ldap/__init__.py
+-rw-r--r--   0        0        0      491 2020-02-02 00:00:00.000000 freenit-0.3.1/freenit/models/ldap/base.py
+-rw-r--r--   0        0        0     1462 2020-02-02 00:00:00.000000 freenit-0.3.1/freenit/models/ldap/user.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 freenit-0.3.1/freenit/models/ormar/__init__.py
+-rw-r--r--   0        0        0     1114 2020-02-02 00:00:00.000000 freenit-0.3.1/freenit/models/ormar/base.py
+-rw-r--r--   0        0        0      208 2020-02-02 00:00:00.000000 freenit-0.3.1/freenit/models/ormar/role.py
+-rw-r--r--   0        0        0      807 2020-02-02 00:00:00.000000 freenit-0.3.1/freenit/models/ormar/theme.py
+-rw-r--r--   0        0        0     1097 2020-02-02 00:00:00.000000 freenit-0.3.1/freenit/models/ormar/user.py
+-rw-r--r--   0        0        0      219 2020-02-02 00:00:00.000000 freenit-0.3.1/freenit/project/.gitignore
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 freenit-0.3.1/freenit/project/LICENSE
+-rw-r--r--   0        0        0     2154 2020-02-02 00:00:00.000000 freenit-0.3.1/freenit/project/alembic.ini
+-rw-r--r--   0        0        0      400 2020-02-02 00:00:00.000000 freenit-0.3.1/freenit/project/main.py
+-rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 freenit-0.3.1/freenit/project/provisioners.mk
+-rw-r--r--   0        0        0      879 2020-02-02 00:00:00.000000 freenit-0.3.1/freenit/project/pyproject.toml
+-rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 freenit-0.3.1/freenit/project/requirements.yml
+-rw-r--r--   0        0        0     1301 2020-02-02 00:00:00.000000 freenit-0.3.1/freenit/project/setup.py
+-rw-r--r--   0        0        0      494 2020-02-02 00:00:00.000000 freenit-0.3.1/freenit/project/alembic/script.py.mako
+-rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 freenit-0.3.1/freenit/project/ansible/group_vars/.keep
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 freenit-0.3.1/freenit/project/ansible/inventory/.keep
+-rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 freenit-0.3.1/freenit/project/ansible/roles/devel/tasks/main.yml
+-rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 freenit-0.3.1/freenit/project/ansible/roles/devel/vars/main.yml
+-rw-r--r--   0        0        0      928 2020-02-02 00:00:00.000000 freenit-0.3.1/freenit/project/bin/common.sh
+-rwxr-xr-x   0        0        0      309 2020-02-02 00:00:00.000000 freenit-0.3.1/freenit/project/bin/devel.sh
+-rwxr-xr-x   0        0        0       95 2020-02-02 00:00:00.000000 freenit-0.3.1/freenit/project/bin/init.sh
+-rwxr-xr-x   0        0        0       99 2020-02-02 00:00:00.000000 freenit-0.3.1/freenit/project/bin/test.sh
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 freenit-0.3.1/freenit/project/project/__init__.py
+-rw-r--r--   0        0        0      446 2020-02-02 00:00:00.000000 freenit-0.3.1/freenit/project/project/app.py
+-rw-r--r--   0        0        0      464 2020-02-02 00:00:00.000000 freenit-0.3.1/freenit/project/project/base_config.py
+-rw-r--r--   0        0        0      623 2020-02-02 00:00:00.000000 freenit-0.3.1/freenit/project/project/config.py
+-rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 freenit-0.3.1/freenit/project/project/api/__init__.py
+-rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 freenit-0.3.1/freenit/project/project/api/router.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 freenit-0.3.1/freenit/project/project/models/__init__.py
+-rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 freenit-0.3.1/freenit/project/templates/site.yml.tpl
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 freenit-0.3.1/freenit/project/tests/__init__.py
+-rw-r--r--   0        0        0     1318 2020-02-02 00:00:00.000000 freenit-0.3.1/freenit/project/tests/client.py
+-rw-r--r--   0        0        0      541 2020-02-02 00:00:00.000000 freenit-0.3.1/freenit/project/tests/conftest.py
+-rw-r--r--   0        0        0      538 2020-02-02 00:00:00.000000 freenit-0.3.1/freenit/project/tests/factories.py
+-rw-r--r--   0        0        0      358 2020-02-02 00:00:00.000000 freenit-0.3.1/freenit/project/tests/test_user.py
+-rw-r--r--   0        0        0      271 2020-02-02 00:00:00.000000 freenit-0.3.1/templates/site.yml.tpl
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 freenit-0.3.1/tests/__init__.py
+-rw-r--r--   0        0        0     1185 2020-02-02 00:00:00.000000 freenit-0.3.1/tests/client.py
+-rw-r--r--   0        0        0      541 2020-02-02 00:00:00.000000 freenit-0.3.1/tests/conftest.py
+-rw-r--r--   0        0        0      538 2020-02-02 00:00:00.000000 freenit-0.3.1/tests/factories.py
+-rw-r--r--   0        0        0      787 2020-02-02 00:00:00.000000 freenit-0.3.1/tests/test_auth.py
+-rw-r--r--   0        0        0     2157 2020-02-02 00:00:00.000000 freenit-0.3.1/tests/test_permission.py
+-rw-r--r--   0        0        0     2281 2020-02-02 00:00:00.000000 freenit-0.3.1/tests/test_role.py
+-rw-r--r--   0        0        0     1944 2020-02-02 00:00:00.000000 freenit-0.3.1/tests/test_user.py
+-rw-r--r--   0        0        0      293 2020-02-02 00:00:00.000000 freenit-0.3.1/.gitignore
+-rw-r--r--   0        0        0     1322 2020-02-02 00:00:00.000000 freenit-0.3.1/LICENSE
+-rw-r--r--   0        0        0      377 2020-02-02 00:00:00.000000 freenit-0.3.1/README.md
+-rw-r--r--   0        0        0     1287 2020-02-02 00:00:00.000000 freenit-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0     3309 2020-02-02 00:00:00.000000 freenit-0.3.1/PKG-INFO
```

### Comparing `freenit-0.3.0/alembic.ini` & `freenit-0.3.1/alembic.ini`

 * *Files identical despite different names*

### Comparing `freenit-0.3.0/setup.py` & `freenit-0.3.1/setup.py`

 * *Files identical despite different names*

### Comparing `freenit-0.3.0/bin/common.sh` & `freenit-0.3.1/bin/common.sh`

 * *Files identical despite different names*

### Comparing `freenit-0.3.0/bin/freenit.sh` & `freenit-0.3.1/bin/freenit.sh`

 * *Files identical despite different names*

### Comparing `freenit-0.3.0/freenit/auth.py` & `freenit-0.3.1/freenit/auth.py`

 * *Files identical despite different names*

### Comparing `freenit-0.3.0/freenit/base_config.py` & `freenit-0.3.1/freenit/base_config.py`

 * *Files identical despite different names*

### Comparing `freenit-0.3.0/freenit/config.py` & `freenit-0.3.1/freenit/config.py`

 * *Files identical despite different names*

### Comparing `freenit-0.3.0/freenit/decorators.py` & `freenit-0.3.1/freenit/decorators.py`

 * *Files identical despite different names*

### Comparing `freenit-0.3.0/freenit/migration.py` & `freenit-0.3.1/freenit/migration.py`

 * *Files identical despite different names*

### Comparing `freenit-0.3.0/freenit/api/auth.py` & `freenit-0.3.1/freenit/api/auth.py`

 * *Files identical despite different names*

### Comparing `freenit-0.3.0/freenit/api/role.py` & `freenit-0.3.1/freenit/api/role.py`

 * *Files identical despite different names*

### Comparing `freenit-0.3.0/freenit/api/theme.py` & `freenit-0.3.1/freenit/api/theme.py`

 * *Files identical despite different names*

### Comparing `freenit-0.3.0/freenit/api/user.py` & `freenit-0.3.1/freenit/api/user.py`

 * *Files identical despite different names*

### Comparing `freenit-0.3.0/freenit/models/pagination.py` & `freenit-0.3.1/freenit/models/pagination.py`

 * *Files identical despite different names*

### Comparing `freenit-0.3.0/freenit/models/ldap/user.py` & `freenit-0.3.1/freenit/models/ldap/user.py`

 * *Files identical despite different names*

### Comparing `freenit-0.3.0/freenit/models/ormar/base.py` & `freenit-0.3.1/freenit/models/ormar/base.py`

 * *Files identical despite different names*

### Comparing `freenit-0.3.0/freenit/models/ormar/theme.py` & `freenit-0.3.1/freenit/models/ormar/theme.py`

 * *Files identical despite different names*

### Comparing `freenit-0.3.0/freenit/models/ormar/user.py` & `freenit-0.3.1/freenit/models/ormar/user.py`

 * *Files identical despite different names*

### Comparing `freenit-0.3.0/freenit/project/alembic.ini` & `freenit-0.3.1/freenit/project/alembic.ini`

 * *Files identical despite different names*

### Comparing `freenit-0.3.0/freenit/project/pyproject.toml` & `freenit-0.3.1/freenit/project/pyproject.toml`

 * *Files identical despite different names*

### Comparing `freenit-0.3.0/freenit/project/setup.py` & `freenit-0.3.1/freenit/project/setup.py`

 * *Files identical despite different names*

### Comparing `freenit-0.3.0/freenit/project/bin/common.sh` & `freenit-0.3.1/freenit/project/bin/common.sh`

 * *Files identical despite different names*

### Comparing `freenit-0.3.0/freenit/project/project/config.py` & `freenit-0.3.1/freenit/project/project/config.py`

 * *Files identical despite different names*

### Comparing `freenit-0.3.0/freenit/project/tests/client.py` & `freenit-0.3.1/freenit/project/tests/client.py`

 * *Files identical despite different names*

### Comparing `freenit-0.3.0/freenit/project/tests/conftest.py` & `freenit-0.3.1/freenit/project/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `freenit-0.3.0/freenit/project/tests/factories.py` & `freenit-0.3.1/freenit/project/tests/factories.py`

 * *Files identical despite different names*

### Comparing `freenit-0.3.0/tests/client.py` & `freenit-0.3.1/tests/client.py`

 * *Files identical despite different names*

### Comparing `freenit-0.3.0/tests/conftest.py` & `freenit-0.3.1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `freenit-0.3.0/tests/factories.py` & `freenit-0.3.1/tests/factories.py`

 * *Files identical despite different names*

### Comparing `freenit-0.3.0/tests/test_auth.py` & `freenit-0.3.1/tests/test_auth.py`

 * *Files identical despite different names*

### Comparing `freenit-0.3.0/tests/test_permission.py` & `freenit-0.3.1/tests/test_permission.py`

 * *Files identical despite different names*

### Comparing `freenit-0.3.0/tests/test_role.py` & `freenit-0.3.1/tests/test_role.py`

 * *Files identical despite different names*

### Comparing `freenit-0.3.0/tests/test_user.py` & `freenit-0.3.1/tests/test_user.py`

 * *Files identical despite different names*

### Comparing `freenit-0.3.0/LICENSE` & `freenit-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `freenit-0.3.0/pyproject.toml` & `freenit-0.3.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `freenit-0.3.0/PKG-INFO` & `freenit-0.3.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: freenit
-Version: 0.3.0
+Version: 0.3.1
 Summary: REST API framework based on FastAPI
 Project-URL: Homepage, https://freenit.org
 Project-URL: Repository, https://github.com/freenit-framework/backend
 Author-email: Goran Mekić <meka@tilda.center>
 License: BSD 2-Clause License
         
         Copyright (c) 2021, Goran Mekić
```

