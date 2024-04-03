# Comparing `tmp/JaxFin-0.2.0.dev0.tar.gz` & `tmp/JaxFin-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "JaxFin-0.2.0.dev0.tar", last modified: Tue Mar  5 22:50:01 2024, max compression
+gzip compressed data, was "JaxFin-0.3.0.tar", last modified: Wed Apr  3 16:01:42 2024, max compression
```

## Comparing `JaxFin-0.2.0.dev0.tar` & `JaxFin-0.3.0.tar`

### file list

```diff
@@ -1,77 +1,83 @@
-drwxrwxrwx   0        0        0        0 2024-03-05 22:50:01.475960 JaxFin-0.2.0.dev0/
-drwxrwxrwx   0        0        0        0 2024-03-05 22:50:00.982516 JaxFin-0.2.0.dev0/.github/
-drwxrwxrwx   0        0        0        0 2024-03-05 22:50:01.083466 JaxFin-0.2.0.dev0/.github/workflows/
--rw-rw-rw-   0        0        0      642 2024-02-17 15:56:37.000000 JaxFin-0.2.0.dev0/.github/workflows/pylint.yml
--rw-rw-rw-   0        0        0      617 2024-02-20 14:16:18.000000 JaxFin-0.2.0.dev0/.github/workflows/pytest.yml
--rw-rw-rw-   0        0        0      822 2024-03-05 14:09:37.000000 JaxFin-0.2.0.dev0/.github/workflows/quality_check.yml
--rw-rw-rw-   0        0        0      464 2024-03-05 13:53:59.000000 JaxFin-0.2.0.dev0/.gitignore
-drwxrwxrwx   0        0        0        0 2024-03-05 22:50:01.152773 JaxFin-0.2.0.dev0/.idea/
--rw-rw-rw-   0        0        0      184 2023-11-27 18:39:40.000000 JaxFin-0.2.0.dev0/.idea/.gitignore
--rw-rw-rw-   0        0        0      435 2024-03-05 13:42:17.000000 JaxFin-0.2.0.dev0/.idea/aws.xml
-drwxrwxrwx   0        0        0        0 2024-03-05 22:50:01.158257 JaxFin-0.2.0.dev0/.idea/inspectionProfiles/
--rw-rw-rw-   0        0        0      179 2023-11-27 18:39:40.000000 JaxFin-0.2.0.dev0/.idea/inspectionProfiles/profiles_settings.xml
--rw-rw-rw-   0        0        0      434 2024-02-20 14:21:44.000000 JaxFin-0.2.0.dev0/.idea/misc.xml
--rw-rw-rw-   0        0        0      283 2023-11-27 18:39:40.000000 JaxFin-0.2.0.dev0/.idea/modules.xml
--rw-rw-rw-   0        0        0      191 2023-12-15 20:40:10.000000 JaxFin-0.2.0.dev0/.idea/other.xml
--rw-rw-rw-   0        0        0      409 2024-02-20 14:21:44.000000 JaxFin-0.2.0.dev0/.idea/py-exopricer.iml
--rw-rw-rw-   0        0        0      172 2023-11-27 18:39:40.000000 JaxFin-0.2.0.dev0/.idea/vcs.xml
--rw-rw-rw-   0        0        0     2418 2024-02-16 14:21:51.000000 JaxFin-0.2.0.dev0/CONTRIBUTING.md
-drwxrwxrwx   0        0        0        0 2024-03-05 22:50:01.472881 JaxFin-0.2.0.dev0/JaxFin.egg-info/
--rw-rw-rw-   0        0        0     7117 2024-03-05 22:50:00.000000 JaxFin-0.2.0.dev0/JaxFin.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1465 2024-03-05 22:50:00.000000 JaxFin-0.2.0.dev0/JaxFin.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-05 22:50:00.000000 JaxFin-0.2.0.dev0/JaxFin.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       55 2024-03-05 22:50:00.000000 JaxFin-0.2.0.dev0/JaxFin.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2024-03-05 22:50:00.000000 JaxFin-0.2.0.dev0/JaxFin.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1098 2024-02-10 17:05:30.000000 JaxFin-0.2.0.dev0/LICENSE
--rw-rw-rw-   0        0        0     7117 2024-03-05 22:50:01.474897 JaxFin-0.2.0.dev0/PKG-INFO
--rw-rw-rw-   0        0        0     6168 2024-03-05 14:09:37.000000 JaxFin-0.2.0.dev0/README.md
-drwxrwxrwx   0        0        0        0 2024-03-05 22:50:01.211932 JaxFin-0.2.0.dev0/jaxfin/
--rw-rw-rw-   0        0        0        0 2024-02-17 09:50:48.000000 JaxFin-0.2.0.dev0/jaxfin/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-05 22:50:01.214116 JaxFin-0.2.0.dev0/jaxfin/models/
--rw-rw-rw-   0        0        0      211 2024-02-17 10:10:13.000000 JaxFin-0.2.0.dev0/jaxfin/models/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-05 22:50:01.218107 JaxFin-0.2.0.dev0/jaxfin/models/gbm/
--rw-rw-rw-   0        0        0      230 2024-02-20 14:21:44.000000 JaxFin-0.2.0.dev0/jaxfin/models/gbm/__init__.py
--rw-rw-rw-   0        0        0     7873 2024-03-05 22:22:03.000000 JaxFin-0.2.0.dev0/jaxfin/models/gbm/gbm.py
-drwxrwxrwx   0        0        0        0 2024-03-05 22:50:01.221348 JaxFin-0.2.0.dev0/jaxfin/models/heston/
--rw-rw-rw-   0        0        0        0 2024-03-05 22:22:03.000000 JaxFin-0.2.0.dev0/jaxfin/models/heston/__init__.py
--rw-rw-rw-   0        0        0     5819 2024-03-05 22:22:03.000000 JaxFin-0.2.0.dev0/jaxfin/models/heston/heston.py
-drwxrwxrwx   0        0        0        0 2024-03-05 22:50:01.221348 JaxFin-0.2.0.dev0/jaxfin/price_engine/
--rw-rw-rw-   0        0        0        0 2024-02-17 09:50:48.000000 JaxFin-0.2.0.dev0/jaxfin/price_engine/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-05 22:50:01.229775 JaxFin-0.2.0.dev0/jaxfin/price_engine/black/
--rw-rw-rw-   0        0        0      249 2024-02-20 14:16:18.000000 JaxFin-0.2.0.dev0/jaxfin/price_engine/black/__init__.py
--rw-rw-rw-   0        0        0     4809 2024-03-05 14:09:37.000000 JaxFin-0.2.0.dev0/jaxfin/price_engine/black/black_model.py
-drwxrwxrwx   0        0        0        0 2024-03-05 22:50:01.233530 JaxFin-0.2.0.dev0/jaxfin/price_engine/black_scholes/
--rw-rw-rw-   0        0        0      423 2024-03-04 19:28:01.000000 JaxFin-0.2.0.dev0/jaxfin/price_engine/black_scholes/__init__.py
--rw-rw-rw-   0        0        0     8033 2024-03-05 14:09:37.000000 JaxFin-0.2.0.dev0/jaxfin/price_engine/black_scholes/vanilla_options.py
-drwxrwxrwx   0        0        0        0 2024-03-05 22:50:01.239100 JaxFin-0.2.0.dev0/jaxfin/price_engine/math/
--rw-rw-rw-   0        0        0        0 2024-03-05 14:09:37.000000 JaxFin-0.2.0.dev0/jaxfin/price_engine/math/__init__.py
--rw-rw-rw-   0        0        0     2609 2024-03-05 14:09:37.000000 JaxFin-0.2.0.dev0/jaxfin/price_engine/math/bs_common.py
--rw-rw-rw-   0        0        0      640 2024-03-05 14:09:37.000000 JaxFin-0.2.0.dev0/jaxfin/price_engine/math/norm.py
-drwxrwxrwx   0        0        0        0 2024-03-05 22:50:01.248162 JaxFin-0.2.0.dev0/jaxfin/price_engine/utils/
--rw-rw-rw-   0        0        0        0 2024-03-05 14:09:37.000000 JaxFin-0.2.0.dev0/jaxfin/price_engine/utils/__init__.py
--rw-rw-rw-   0        0        0      920 2024-03-05 14:09:37.000000 JaxFin-0.2.0.dev0/jaxfin/price_engine/utils/arrays.py
--rw-rw-rw-   0        0        0     2788 2024-03-05 14:09:37.000000 JaxFin-0.2.0.dev0/jaxfin/price_engine/utils/vect.py
--rw-rw-rw-   0        0        0      175 2024-02-10 14:03:34.000000 JaxFin-0.2.0.dev0/noxfile.py
--rw-rw-rw-   0        0        0    22980 2024-03-05 22:22:03.000000 JaxFin-0.2.0.dev0/pyproject.toml
-drwxrwxrwx   0        0        0        0 2024-03-05 22:50:01.269559 JaxFin-0.2.0.dev0/requirements/
--rw-rw-rw-   0        0        0      507 2024-03-05 14:09:37.000000 JaxFin-0.2.0.dev0/requirements/build.txt
--rw-rw-rw-   0        0        0     2530 2024-02-10 17:11:27.000000 JaxFin-0.2.0.dev0/requirements/dev.txt
-drwxrwxrwx   0        0        0        0 2024-03-05 22:50:01.409880 JaxFin-0.2.0.dev0/scripts/
--rwxrwxrwx   0        0        0       61 2023-12-19 18:23:50.000000 JaxFin-0.2.0.dev0/scripts/basedir.bat
--rwxrwxrwx   0        0        0       68 2024-02-10 16:19:46.000000 JaxFin-0.2.0.dev0/scripts/black-reformat.bat
--rwxrwxrwx   0        0        0       76 2024-02-10 16:19:46.000000 JaxFin-0.2.0.dev0/scripts/check-black.bat
--rwxrwxrwx   0        0        0      376 2024-02-17 11:13:18.000000 JaxFin-0.2.0.dev0/scripts/configure-python.bat
--rwxrwxrwx   0        0        0      720 2024-02-17 11:22:03.000000 JaxFin-0.2.0.dev0/scripts/create-new-version.bat
--rwxrwxrwx   0        0        0      102 2024-02-20 14:16:18.000000 JaxFin-0.2.0.dev0/scripts/get-tests-cov.bat
--rwxrwxrwx   0        0        0       69 2024-02-10 17:00:41.000000 JaxFin-0.2.0.dev0/scripts/run-mypy.bat
--rwxrwxrwx   0        0        0      117 2024-02-17 11:13:37.000000 JaxFin-0.2.0.dev0/scripts/run-pylint.bat
--rwxrwxrwx   0        0        0      126 2024-02-10 16:58:40.000000 JaxFin-0.2.0.dev0/scripts/run-tests.bat
--rw-rw-rw-   0        0        0       42 2024-03-05 22:50:01.475960 JaxFin-0.2.0.dev0/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-03-05 22:50:01.409880 JaxFin-0.2.0.dev0/tests/
--rw-rw-rw-   0        0        0        0 2023-11-27 18:43:58.000000 JaxFin-0.2.0.dev0/tests/.gitkeep
-drwxrwxrwx   0        0        0        0 2024-03-05 22:50:01.438614 JaxFin-0.2.0.dev0/tests/models/
--rw-rw-rw-   0        0        0     1764 2024-03-05 22:22:03.000000 JaxFin-0.2.0.dev0/tests/models/test_gbm.py
--rw-rw-rw-   0        0        0     1377 2024-03-05 22:22:03.000000 JaxFin-0.2.0.dev0/tests/models/test_heston.py
-drwxrwxrwx   0        0        0        0 2024-03-05 22:50:01.470271 JaxFin-0.2.0.dev0/tests/price_engine/
--rw-rw-rw-   0        0        0     6330 2024-03-05 14:09:37.000000 JaxFin-0.2.0.dev0/tests/price_engine/test_black.py
--rw-rw-rw-   0        0        0    11453 2024-03-05 14:09:37.000000 JaxFin-0.2.0.dev0/tests/price_engine/test_bs.py
+drwxrwxrwx   0        0        0        0 2024-04-03 16:01:42.317427 JaxFin-0.3.0/
+drwxrwxrwx   0        0        0        0 2024-04-03 16:01:42.046569 JaxFin-0.3.0/.github/
+drwxrwxrwx   0        0        0        0 2024-04-03 16:01:42.106186 JaxFin-0.3.0/.github/workflows/
+-rw-rw-rw-   0        0        0      597 2024-03-17 17:34:48.000000 JaxFin-0.3.0/.github/workflows/linting.yml
+-rw-rw-rw-   0        0        0      617 2024-02-20 14:16:18.000000 JaxFin-0.3.0/.github/workflows/pytest.yml
+-rw-rw-rw-   0        0        0      822 2024-03-05 14:09:37.000000 JaxFin-0.3.0/.github/workflows/quality_check.yml
+-rw-rw-rw-   0        0        0      497 2024-03-17 17:29:55.000000 JaxFin-0.3.0/.gitignore
+drwxrwxrwx   0        0        0        0 2024-04-03 16:01:42.126677 JaxFin-0.3.0/.idea/
+-rw-rw-rw-   0        0        0      184 2023-11-27 18:39:40.000000 JaxFin-0.3.0/.idea/.gitignore
+-rw-rw-rw-   0        0        0      435 2024-03-05 13:42:17.000000 JaxFin-0.3.0/.idea/aws.xml
+drwxrwxrwx   0        0        0        0 2024-04-03 16:01:42.129477 JaxFin-0.3.0/.idea/inspectionProfiles/
+-rw-rw-rw-   0        0        0      179 2023-11-27 18:39:40.000000 JaxFin-0.3.0/.idea/inspectionProfiles/profiles_settings.xml
+-rw-rw-rw-   0        0        0      434 2024-02-20 14:21:44.000000 JaxFin-0.3.0/.idea/misc.xml
+-rw-rw-rw-   0        0        0      283 2023-11-27 18:39:40.000000 JaxFin-0.3.0/.idea/modules.xml
+-rw-rw-rw-   0        0        0      191 2023-12-15 20:40:10.000000 JaxFin-0.3.0/.idea/other.xml
+-rw-rw-rw-   0        0        0      409 2024-02-20 14:21:44.000000 JaxFin-0.3.0/.idea/py-exopricer.iml
+-rw-rw-rw-   0        0        0      172 2023-11-27 18:39:40.000000 JaxFin-0.3.0/.idea/vcs.xml
+-rw-rw-rw-   0        0        0     2418 2024-02-16 14:21:51.000000 JaxFin-0.3.0/CONTRIBUTING.md
+drwxrwxrwx   0        0        0        0 2024-04-03 16:01:42.311379 JaxFin-0.3.0/JaxFin.egg-info/
+-rw-rw-rw-   0        0        0     7516 2024-04-03 16:01:41.000000 JaxFin-0.3.0/JaxFin.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1608 2024-04-03 16:01:42.000000 JaxFin-0.3.0/JaxFin.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-03 16:01:41.000000 JaxFin-0.3.0/JaxFin.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       27 2024-04-03 16:01:41.000000 JaxFin-0.3.0/JaxFin.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2024-04-03 16:01:41.000000 JaxFin-0.3.0/JaxFin.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1098 2024-02-10 17:05:30.000000 JaxFin-0.3.0/LICENSE
+-rw-rw-rw-   0        0        0      637 2024-04-03 15:58:34.000000 JaxFin-0.3.0/Makefile
+-rw-rw-rw-   0        0        0     7516 2024-04-03 16:01:42.313856 JaxFin-0.3.0/PKG-INFO
+-rw-rw-rw-   0        0        0     6632 2024-04-03 15:58:34.000000 JaxFin-0.3.0/README.md
+drwxrwxrwx   0        0        0        0 2024-04-03 16:01:42.187832 JaxFin-0.3.0/jaxfin/
+-rw-rw-rw-   0        0        0        0 2024-02-17 09:50:48.000000 JaxFin-0.3.0/jaxfin/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-03 16:01:42.194131 JaxFin-0.3.0/jaxfin/models/
+-rw-rw-rw-   0        0        0      211 2024-02-17 10:10:13.000000 JaxFin-0.3.0/jaxfin/models/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-03 16:01:42.199669 JaxFin-0.3.0/jaxfin/models/gbm/
+-rw-rw-rw-   0        0        0      230 2024-02-20 14:21:44.000000 JaxFin-0.3.0/jaxfin/models/gbm/__init__.py
+-rw-rw-rw-   0        0        0     7604 2024-03-07 14:43:03.000000 JaxFin-0.3.0/jaxfin/models/gbm/gbm.py
+drwxrwxrwx   0        0        0        0 2024-04-03 16:01:42.207091 JaxFin-0.3.0/jaxfin/models/heston/
+-rw-rw-rw-   0        0        0      159 2024-03-07 14:43:03.000000 JaxFin-0.3.0/jaxfin/models/heston/__init__.py
+-rw-rw-rw-   0        0        0    12759 2024-03-07 14:43:03.000000 JaxFin-0.3.0/jaxfin/models/heston/heston.py
+-rw-rw-rw-   0        0        0      381 2024-03-07 14:43:03.000000 JaxFin-0.3.0/jaxfin/models/utils.py
+drwxrwxrwx   0        0        0        0 2024-04-03 16:01:42.209728 JaxFin-0.3.0/jaxfin/price_engine/
+-rw-rw-rw-   0        0        0        0 2024-02-17 09:50:48.000000 JaxFin-0.3.0/jaxfin/price_engine/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-03 16:01:42.215098 JaxFin-0.3.0/jaxfin/price_engine/black/
+-rw-rw-rw-   0        0        0      249 2024-02-20 14:16:18.000000 JaxFin-0.3.0/jaxfin/price_engine/black/__init__.py
+-rw-rw-rw-   0        0        0     4809 2024-03-05 14:09:37.000000 JaxFin-0.3.0/jaxfin/price_engine/black/black_model.py
+drwxrwxrwx   0        0        0        0 2024-04-03 16:01:42.221477 JaxFin-0.3.0/jaxfin/price_engine/black_scholes/
+-rw-rw-rw-   0        0        0      423 2024-03-04 19:28:01.000000 JaxFin-0.3.0/jaxfin/price_engine/black_scholes/__init__.py
+-rw-rw-rw-   0        0        0     8033 2024-03-05 14:09:37.000000 JaxFin-0.3.0/jaxfin/price_engine/black_scholes/vanilla_options.py
+drwxrwxrwx   0        0        0        0 2024-04-03 16:01:42.227259 JaxFin-0.3.0/jaxfin/price_engine/fft/
+-rw-rw-rw-   0        0        0      290 2024-04-03 15:58:34.000000 JaxFin-0.3.0/jaxfin/price_engine/fft/__init__.py
+-rw-rw-rw-   0        0        0     5916 2024-04-03 15:58:34.000000 JaxFin-0.3.0/jaxfin/price_engine/fft/vanilla_options.py
+drwxrwxrwx   0        0        0        0 2024-04-03 16:01:42.234534 JaxFin-0.3.0/jaxfin/price_engine/math/
+-rw-rw-rw-   0        0        0        0 2024-03-05 14:09:37.000000 JaxFin-0.3.0/jaxfin/price_engine/math/__init__.py
+-rw-rw-rw-   0        0        0     2609 2024-03-05 14:09:37.000000 JaxFin-0.3.0/jaxfin/price_engine/math/bs_common.py
+-rw-rw-rw-   0        0        0      640 2024-03-05 14:09:37.000000 JaxFin-0.3.0/jaxfin/price_engine/math/norm.py
+drwxrwxrwx   0        0        0        0 2024-04-03 16:01:42.245290 JaxFin-0.3.0/jaxfin/price_engine/utils/
+-rw-rw-rw-   0        0        0        0 2024-03-05 14:09:37.000000 JaxFin-0.3.0/jaxfin/price_engine/utils/__init__.py
+-rw-rw-rw-   0        0        0      920 2024-03-05 14:09:37.000000 JaxFin-0.3.0/jaxfin/price_engine/utils/arrays.py
+-rw-rw-rw-   0        0        0     2788 2024-03-05 14:09:37.000000 JaxFin-0.3.0/jaxfin/price_engine/utils/vect.py
+-rw-rw-rw-   0        0        0      175 2024-02-10 14:03:34.000000 JaxFin-0.3.0/noxfile.py
+-rw-rw-rw-   0        0        0    23014 2024-03-23 15:48:12.000000 JaxFin-0.3.0/pyproject.toml
+drwxrwxrwx   0        0        0        0 2024-04-03 16:01:42.251698 JaxFin-0.3.0/requirements/
+-rw-rw-rw-   0        0        0      505 2024-03-17 17:32:57.000000 JaxFin-0.3.0/requirements/build.txt
+-rw-rw-rw-   0        0        0     2528 2024-03-17 17:26:30.000000 JaxFin-0.3.0/requirements/dev.txt
+drwxrwxrwx   0        0        0        0 2024-04-03 16:01:42.284511 JaxFin-0.3.0/scripts/
+-rwxrwxrwx   0        0        0       61 2023-12-19 18:23:50.000000 JaxFin-0.3.0/scripts/basedir.bat
+-rwxrwxrwx   0        0        0       68 2024-02-10 16:19:46.000000 JaxFin-0.3.0/scripts/black-reformat.bat
+-rwxrwxrwx   0        0        0       76 2024-02-10 16:19:46.000000 JaxFin-0.3.0/scripts/check-black.bat
+-rwxrwxrwx   0        0        0      376 2024-02-17 11:13:18.000000 JaxFin-0.3.0/scripts/configure-python.bat
+-rwxrwxrwx   0        0        0      720 2024-02-17 11:22:03.000000 JaxFin-0.3.0/scripts/create-new-version.bat
+-rwxrwxrwx   0        0        0      102 2024-02-20 14:16:18.000000 JaxFin-0.3.0/scripts/get-tests-cov.bat
+-rwxrwxrwx   0        0        0       96 2024-03-17 17:31:24.000000 JaxFin-0.3.0/scripts/run-linter.bat
+-rwxrwxrwx   0        0        0       69 2024-02-10 17:00:41.000000 JaxFin-0.3.0/scripts/run-mypy.bat
+-rwxrwxrwx   0        0        0      126 2024-02-10 16:58:40.000000 JaxFin-0.3.0/scripts/run-tests.bat
+-rw-rw-rw-   0        0        0       42 2024-04-03 16:01:42.317427 JaxFin-0.3.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-03 16:01:42.291126 JaxFin-0.3.0/tests/
+-rw-rw-rw-   0        0        0        0 2023-11-27 18:43:58.000000 JaxFin-0.3.0/tests/.gitkeep
+drwxrwxrwx   0        0        0        0 2024-04-03 16:01:42.295482 JaxFin-0.3.0/tests/models/
+-rw-rw-rw-   0        0        0     1760 2024-04-03 15:58:34.000000 JaxFin-0.3.0/tests/models/test_gbm.py
+-rw-rw-rw-   0        0        0     3177 2024-04-03 15:58:34.000000 JaxFin-0.3.0/tests/models/test_heston.py
+drwxrwxrwx   0        0        0        0 2024-04-03 16:01:42.307829 JaxFin-0.3.0/tests/price_engine/
+-rw-rw-rw-   0        0        0     6518 2024-04-03 15:58:34.000000 JaxFin-0.3.0/tests/price_engine/test_black.py
+-rw-rw-rw-   0        0        0    11089 2024-04-03 15:58:34.000000 JaxFin-0.3.0/tests/price_engine/test_bs.py
+-rw-rw-rw-   0        0        0     3335 2024-04-03 15:58:34.000000 JaxFin-0.3.0/tests/price_engine/test_fft.py
```

### Comparing `JaxFin-0.2.0.dev0/.github/workflows/pytest.yml` & `JaxFin-0.3.0/.github/workflows/pytest.yml`

 * *Files identical despite different names*

### Comparing `JaxFin-0.2.0.dev0/.github/workflows/quality_check.yml` & `JaxFin-0.3.0/.github/workflows/quality_check.yml`

 * *Files identical despite different names*

### Comparing `JaxFin-0.2.0.dev0/CONTRIBUTING.md` & `JaxFin-0.3.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `JaxFin-0.2.0.dev0/JaxFin.egg-info/PKG-INFO` & `JaxFin-0.3.0/JaxFin.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: JaxFin
-Version: 0.2.0.dev0
+Version: 0.3.0
 Summary: JaxFin is a powerful and versatile Python library designed for pricing exotic options using a range of advanced financial techniques.
 Author-email: Paolo D'Elia <paolo.delia99@gmail.com>, Samuele D'Elia <delia.samuele00@gmail.com>
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Scientific/Engineering :: Mathematics
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
@@ -12,16 +12,14 @@
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Developers
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: jax==0.4.23
 Requires-Dist: jaxlib==0.4.23
-Requires-Dist: numpy==1.26.2
-Requires-Dist: scipy==1.11.4
 
 # JaxFin
 
 `JaxFin` is a powerful and versatile Python library designed for pricing exotic options using a range of advanced financial techniques. The library is built with the aim of providing a robust, flexible, and efficient tool for quantitative finance professionals, researchers, and students alike. It offers a comprehensive suite of features that allow users to model, price, and analyze a wide variety of exotic options.
 
 The core strength of `JaxFin` lies in its use of the [jax](https://github.com/google/jax) library. Jax is a high-performance library for accelerated array computing, offering features such as automatic differentiation (AutoGrad), accelerated linear algebra (XLA), and just-in-time compilation to GPU/TPU. By leveraging these capabilities, `JaxFin` is able to perform complex financial computations with exceptional speed and efficiency.
 
@@ -61,28 +59,32 @@
 strikes = jnp.asarray([110])
 expires = jnp.asarray([1.0])
 vols = jnp.asarray([0.2])
 discount_rates = jnp.asarray([0.0])
 european_price(spots, strikes, expires, vols, discount_rates, dtype=jnp.float32)
 ```
 
-Computing the price price of a single option, nahh that's boring! what we can do with jaxfin is to compute the price of a basket of options leveraging the vectorization capabilities of `jax`:
+Computing the price price of a single option, nahh that's boring! what we can do with jaxfin is to compute the price of a basket of options leveraging the vectorization capabilities of `jax` using `jax.vmap`:
 
 ```python
+from jax import vmap
 import jax.numpy as jnp
 from jaxfin.price_engine.black_scholes import european_price
 
+v_european_price = vmap(european_price, in_axes=(0, None, None, None, None))
+
 # Black-Scholes price of an european option
-spots = jnp.asarray([100, 110, 120])
-strikes = jnp.asarray([110, 120, 130])
-expires = jnp.asarray([1.0, 1.0, 1.0])
-vols = jnp.asarray([0.2, 0.2, 0.2])
-discount_rates = jnp.asarray([0.0, 0.0, 0.0])
-are_calls = jnp.array([True, False, False, True, True], dtype=jnp.bool_)
-european_price(spots, strikes, expires, vols, discount_rates, are_calls, dtype=jnp.float32)
+spots = jnp.asarray([80, 90, 100, 110, 120])
+strikes = jnp.asarray(110)
+expires = jnp.asarray(1.0)
+vols = jnp.asarray(0.2)
+discount_rates = jnp.asarray(0.0)
+v_european_price(spots, strikes, expires, vols, discount_rates)
+
+>> Array([0.4424405, 1.6421748, 4.292015, 8.762122, 15.010387], dtype=float32)
 ```
 
 In addition to that the calculation of the greeks, is done not throught the closed form formulas but through the automatic differentiation capabilities of `jax`. For example the function that calculates the delta of the european option under the Black Scholes model can be simply obtained as follows:
 
 ```python
 delta_european = jax.grad(european_price, argnums=0)
 
@@ -100,18 +102,24 @@
 - Price engine
     - Black scholes
         - Pricing european options
         - Greeks of european options
     - Black model
         - Pricing european options
         - Greeks of european options (just delta and gamma)
+    - Fourier methods
+        - Pricing european options using inverse fourier transform
+        - Greeks of european options (just delta)
 - Models
     - Geometric brownian motion
       - Univariate 
       - Multivariate
+    - Heston
+      - Univariate
+      - Multivariate
 
 ## Building the Library Locally
 
 To build the library locally, follow these steps:
 
 1. Clone the repository:
 
@@ -143,14 +151,26 @@
 To achieve that the following scripts have been provided
 
 - `scripts\run-pylint.bat`: This script runs Pylint, a tool that checks for errors in Python code, enforces a coding standard, and looks for code smells. It can also look for certain type errors, it can recommend suggestions about how particular blocks can be refactored and can offer you details about the code's complexity.
 - `scripts\run-tests.bat`: This script runs the unit tests for the project.
 - `scripts\run-mypy.bat`: This script runs Mypy, a static type checker for Python. Mypy can catch certain types of errors at compile time that would otherwise only be caught at runtime in standard Python. It's a way to get some of the benefits of static typing in a dynamically typed language.
 - `scripts\check-black.bat`: This script runs Black, the "uncompromising" Python code formatter. By using it, you ensure that your codebase has a consistent style, which can make it easier to read and maintain.
 
+Otherwise a `Makefile` have been provided to run all the pre-commit checks at once:
+
+```bash
+make commit-checks
+```
+
+To run the tests you can use the following command:
+
+```bash
+make pytest
+```
+
 ## Contributing
 
 Contributions are welcome! Please follow these steps:
 
 1. Fork the repository
 2. Create your feature branch (`git checkout -b feature`)
 3. Commit your changes (`git commit -am 'Add new feature'`)
```

### Comparing `JaxFin-0.2.0.dev0/JaxFin.egg-info/SOURCES.txt` & `JaxFin-0.3.0/JaxFin.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 .gitignore
 CONTRIBUTING.md
 LICENSE
+Makefile
 README.md
 noxfile.py
 pyproject.toml
-.github/workflows/pylint.yml
+.github/workflows/linting.yml
 .github/workflows/pytest.yml
 .github/workflows/quality_check.yml
 .idea/.gitignore
 .idea/aws.xml
 .idea/misc.xml
 .idea/modules.xml
 .idea/other.xml
@@ -18,38 +19,42 @@
 JaxFin.egg-info/PKG-INFO
 JaxFin.egg-info/SOURCES.txt
 JaxFin.egg-info/dependency_links.txt
 JaxFin.egg-info/requires.txt
 JaxFin.egg-info/top_level.txt
 jaxfin/__init__.py
 jaxfin/models/__init__.py
+jaxfin/models/utils.py
 jaxfin/models/gbm/__init__.py
 jaxfin/models/gbm/gbm.py
 jaxfin/models/heston/__init__.py
 jaxfin/models/heston/heston.py
 jaxfin/price_engine/__init__.py
 jaxfin/price_engine/black/__init__.py
 jaxfin/price_engine/black/black_model.py
 jaxfin/price_engine/black_scholes/__init__.py
 jaxfin/price_engine/black_scholes/vanilla_options.py
+jaxfin/price_engine/fft/__init__.py
+jaxfin/price_engine/fft/vanilla_options.py
 jaxfin/price_engine/math/__init__.py
 jaxfin/price_engine/math/bs_common.py
 jaxfin/price_engine/math/norm.py
 jaxfin/price_engine/utils/__init__.py
 jaxfin/price_engine/utils/arrays.py
 jaxfin/price_engine/utils/vect.py
 requirements/build.txt
 requirements/dev.txt
 scripts/basedir.bat
 scripts/black-reformat.bat
 scripts/check-black.bat
 scripts/configure-python.bat
 scripts/create-new-version.bat
 scripts/get-tests-cov.bat
+scripts/run-linter.bat
 scripts/run-mypy.bat
-scripts/run-pylint.bat
 scripts/run-tests.bat
 tests/.gitkeep
 tests/models/test_gbm.py
 tests/models/test_heston.py
 tests/price_engine/test_black.py
-tests/price_engine/test_bs.py
+tests/price_engine/test_bs.py
+tests/price_engine/test_fft.py
```

### Comparing `JaxFin-0.2.0.dev0/LICENSE` & `JaxFin-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `JaxFin-0.2.0.dev0/PKG-INFO` & `JaxFin-0.3.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: JaxFin
-Version: 0.2.0.dev0
+Version: 0.3.0
 Summary: JaxFin is a powerful and versatile Python library designed for pricing exotic options using a range of advanced financial techniques.
 Author-email: Paolo D'Elia <paolo.delia99@gmail.com>, Samuele D'Elia <delia.samuele00@gmail.com>
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Scientific/Engineering :: Mathematics
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
@@ -12,16 +12,14 @@
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Developers
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: jax==0.4.23
 Requires-Dist: jaxlib==0.4.23
-Requires-Dist: numpy==1.26.2
-Requires-Dist: scipy==1.11.4
 
 # JaxFin
 
 `JaxFin` is a powerful and versatile Python library designed for pricing exotic options using a range of advanced financial techniques. The library is built with the aim of providing a robust, flexible, and efficient tool for quantitative finance professionals, researchers, and students alike. It offers a comprehensive suite of features that allow users to model, price, and analyze a wide variety of exotic options.
 
 The core strength of `JaxFin` lies in its use of the [jax](https://github.com/google/jax) library. Jax is a high-performance library for accelerated array computing, offering features such as automatic differentiation (AutoGrad), accelerated linear algebra (XLA), and just-in-time compilation to GPU/TPU. By leveraging these capabilities, `JaxFin` is able to perform complex financial computations with exceptional speed and efficiency.
 
@@ -61,28 +59,32 @@
 strikes = jnp.asarray([110])
 expires = jnp.asarray([1.0])
 vols = jnp.asarray([0.2])
 discount_rates = jnp.asarray([0.0])
 european_price(spots, strikes, expires, vols, discount_rates, dtype=jnp.float32)
 ```
 
-Computing the price price of a single option, nahh that's boring! what we can do with jaxfin is to compute the price of a basket of options leveraging the vectorization capabilities of `jax`:
+Computing the price price of a single option, nahh that's boring! what we can do with jaxfin is to compute the price of a basket of options leveraging the vectorization capabilities of `jax` using `jax.vmap`:
 
 ```python
+from jax import vmap
 import jax.numpy as jnp
 from jaxfin.price_engine.black_scholes import european_price
 
+v_european_price = vmap(european_price, in_axes=(0, None, None, None, None))
+
 # Black-Scholes price of an european option
-spots = jnp.asarray([100, 110, 120])
-strikes = jnp.asarray([110, 120, 130])
-expires = jnp.asarray([1.0, 1.0, 1.0])
-vols = jnp.asarray([0.2, 0.2, 0.2])
-discount_rates = jnp.asarray([0.0, 0.0, 0.0])
-are_calls = jnp.array([True, False, False, True, True], dtype=jnp.bool_)
-european_price(spots, strikes, expires, vols, discount_rates, are_calls, dtype=jnp.float32)
+spots = jnp.asarray([80, 90, 100, 110, 120])
+strikes = jnp.asarray(110)
+expires = jnp.asarray(1.0)
+vols = jnp.asarray(0.2)
+discount_rates = jnp.asarray(0.0)
+v_european_price(spots, strikes, expires, vols, discount_rates)
+
+>> Array([0.4424405, 1.6421748, 4.292015, 8.762122, 15.010387], dtype=float32)
 ```
 
 In addition to that the calculation of the greeks, is done not throught the closed form formulas but through the automatic differentiation capabilities of `jax`. For example the function that calculates the delta of the european option under the Black Scholes model can be simply obtained as follows:
 
 ```python
 delta_european = jax.grad(european_price, argnums=0)
 
@@ -100,18 +102,24 @@
 - Price engine
     - Black scholes
         - Pricing european options
         - Greeks of european options
     - Black model
         - Pricing european options
         - Greeks of european options (just delta and gamma)
+    - Fourier methods
+        - Pricing european options using inverse fourier transform
+        - Greeks of european options (just delta)
 - Models
     - Geometric brownian motion
       - Univariate 
       - Multivariate
+    - Heston
+      - Univariate
+      - Multivariate
 
 ## Building the Library Locally
 
 To build the library locally, follow these steps:
 
 1. Clone the repository:
 
@@ -143,14 +151,26 @@
 To achieve that the following scripts have been provided
 
 - `scripts\run-pylint.bat`: This script runs Pylint, a tool that checks for errors in Python code, enforces a coding standard, and looks for code smells. It can also look for certain type errors, it can recommend suggestions about how particular blocks can be refactored and can offer you details about the code's complexity.
 - `scripts\run-tests.bat`: This script runs the unit tests for the project.
 - `scripts\run-mypy.bat`: This script runs Mypy, a static type checker for Python. Mypy can catch certain types of errors at compile time that would otherwise only be caught at runtime in standard Python. It's a way to get some of the benefits of static typing in a dynamically typed language.
 - `scripts\check-black.bat`: This script runs Black, the "uncompromising" Python code formatter. By using it, you ensure that your codebase has a consistent style, which can make it easier to read and maintain.
 
+Otherwise a `Makefile` have been provided to run all the pre-commit checks at once:
+
+```bash
+make commit-checks
+```
+
+To run the tests you can use the following command:
+
+```bash
+make pytest
+```
+
 ## Contributing
 
 Contributions are welcome! Please follow these steps:
 
 1. Fork the repository
 2. Create your feature branch (`git checkout -b feature`)
 3. Commit your changes (`git commit -am 'Add new feature'`)
```

### Comparing `JaxFin-0.2.0.dev0/README.md` & `JaxFin-0.3.0/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -40,28 +40,32 @@
 strikes = jnp.asarray([110])
 expires = jnp.asarray([1.0])
 vols = jnp.asarray([0.2])
 discount_rates = jnp.asarray([0.0])
 european_price(spots, strikes, expires, vols, discount_rates, dtype=jnp.float32)
 ```
 
-Computing the price price of a single option, nahh that's boring! what we can do with jaxfin is to compute the price of a basket of options leveraging the vectorization capabilities of `jax`:
+Computing the price price of a single option, nahh that's boring! what we can do with jaxfin is to compute the price of a basket of options leveraging the vectorization capabilities of `jax` using `jax.vmap`:
 
 ```python
+from jax import vmap
 import jax.numpy as jnp
 from jaxfin.price_engine.black_scholes import european_price
 
+v_european_price = vmap(european_price, in_axes=(0, None, None, None, None))
+
 # Black-Scholes price of an european option
-spots = jnp.asarray([100, 110, 120])
-strikes = jnp.asarray([110, 120, 130])
-expires = jnp.asarray([1.0, 1.0, 1.0])
-vols = jnp.asarray([0.2, 0.2, 0.2])
-discount_rates = jnp.asarray([0.0, 0.0, 0.0])
-are_calls = jnp.array([True, False, False, True, True], dtype=jnp.bool_)
-european_price(spots, strikes, expires, vols, discount_rates, are_calls, dtype=jnp.float32)
+spots = jnp.asarray([80, 90, 100, 110, 120])
+strikes = jnp.asarray(110)
+expires = jnp.asarray(1.0)
+vols = jnp.asarray(0.2)
+discount_rates = jnp.asarray(0.0)
+v_european_price(spots, strikes, expires, vols, discount_rates)
+
+>> Array([0.4424405, 1.6421748, 4.292015, 8.762122, 15.010387], dtype=float32)
 ```
 
 In addition to that the calculation of the greeks, is done not throught the closed form formulas but through the automatic differentiation capabilities of `jax`. For example the function that calculates the delta of the european option under the Black Scholes model can be simply obtained as follows:
 
 ```python
 delta_european = jax.grad(european_price, argnums=0)
 
@@ -79,18 +83,24 @@
 - Price engine
     - Black scholes
         - Pricing european options
         - Greeks of european options
     - Black model
         - Pricing european options
         - Greeks of european options (just delta and gamma)
+    - Fourier methods
+        - Pricing european options using inverse fourier transform
+        - Greeks of european options (just delta)
 - Models
     - Geometric brownian motion
       - Univariate 
       - Multivariate
+    - Heston
+      - Univariate
+      - Multivariate
 
 ## Building the Library Locally
 
 To build the library locally, follow these steps:
 
 1. Clone the repository:
 
@@ -122,14 +132,26 @@
 To achieve that the following scripts have been provided
 
 - `scripts\run-pylint.bat`: This script runs Pylint, a tool that checks for errors in Python code, enforces a coding standard, and looks for code smells. It can also look for certain type errors, it can recommend suggestions about how particular blocks can be refactored and can offer you details about the code's complexity.
 - `scripts\run-tests.bat`: This script runs the unit tests for the project.
 - `scripts\run-mypy.bat`: This script runs Mypy, a static type checker for Python. Mypy can catch certain types of errors at compile time that would otherwise only be caught at runtime in standard Python. It's a way to get some of the benefits of static typing in a dynamically typed language.
 - `scripts\check-black.bat`: This script runs Black, the "uncompromising" Python code formatter. By using it, you ensure that your codebase has a consistent style, which can make it easier to read and maintain.
 
+Otherwise a `Makefile` have been provided to run all the pre-commit checks at once:
+
+```bash
+make commit-checks
+```
+
+To run the tests you can use the following command:
+
+```bash
+make pytest
+```
+
 ## Contributing
 
 Contributions are welcome! Please follow these steps:
 
 1. Fork the repository
 2. Create your feature branch (`git checkout -b feature`)
 3. Commit your changes (`git commit -am 'Add new feature'`)
```

### Comparing `JaxFin-0.2.0.dev0/jaxfin/models/gbm/gbm.py` & `JaxFin-0.3.0/jaxfin/models/gbm/gbm.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 """Geometric Brownian Motion class implementation"""
 from typing import List, Optional, Union
 
 import jax
 import jax.numpy as jnp
 from jax import random
 
+from ..utils import check_symmetric
+
 
 class UnivGeometricBrownianMotion:
     """
     Geometric Brownian Motion
 
     Represent a 1-dimensional GBM
 
@@ -146,15 +148,15 @@
             ValueError: when the dtype is None
             ValueError: When the correlation matrix is not symmetric
             ValueError: When the correlation matrix does not have ones as diagonal elements
         """
         if dtype is None:
             raise ValueError("dtype must not be None")
 
-        if not _check_symmetric(corr, 1e-8):
+        if not check_symmetric(corr, 1e-8):
             raise ValueError("Correlation matrix must be symmetric")
 
         if not jnp.array_equal(jnp.diag(corr), jnp.ones(corr.shape[0])):
             raise ValueError("Correlation matrix must have ones as diagonal elements")
 
         self._dtype = dtype
         self._s0 = jnp.asarray(s0, dtype=dtype)
@@ -209,15 +211,15 @@
         """
         Simulate a sample of paths from the Multivariate Geometric Brownian Motion (GBM).
 
         Args:
             maturity (float): Time in years.
             n (int): Number of steps.
             n_sim (int): Number of simulations.
-        
+
         Returns:
             jax.Array: Array containing the sample paths.
         """
         key = random.PRNGKey(seed)
 
         dt = maturity / n
 
@@ -236,18 +238,7 @@
 
         once = jnp.ones([n, n], dtype=self._dtype)
         lower_triangular = jnp.tril(once, k=-1)
         cumsum = log_increments.transpose() @ lower_triangular
         cumsum = cumsum.transpose((1, 2, 0))
         samples = self._s0 * jnp.exp(cumsum)
         return samples.transpose(1, 0, 2)[::-1, :, :]
-
-
-def _check_symmetric(a: jax.Array, tol=1e-8):
-    """
-    Check if a matrix is symmetric
-
-    :param a: (jax.Array): Matrix to check
-    :param tol: (float): Tolerance for the check
-    :return: (bool): True if the matrix is symmetric
-    """
-    return jnp.all(jnp.abs(a - a.T) < tol)
```

### Comparing `JaxFin-0.2.0.dev0/jaxfin/price_engine/black/black_model.py` & `JaxFin-0.3.0/jaxfin/price_engine/black/black_model.py`

 * *Files identical despite different names*

### Comparing `JaxFin-0.2.0.dev0/jaxfin/price_engine/black_scholes/vanilla_options.py` & `JaxFin-0.3.0/jaxfin/price_engine/black_scholes/vanilla_options.py`

 * *Files identical despite different names*

### Comparing `JaxFin-0.2.0.dev0/jaxfin/price_engine/math/bs_common.py` & `JaxFin-0.3.0/jaxfin/price_engine/math/bs_common.py`

 * *Files identical despite different names*

### Comparing `JaxFin-0.2.0.dev0/jaxfin/price_engine/math/norm.py` & `JaxFin-0.3.0/jaxfin/price_engine/math/norm.py`

 * *Files identical despite different names*

### Comparing `JaxFin-0.2.0.dev0/jaxfin/price_engine/utils/arrays.py` & `JaxFin-0.3.0/jaxfin/price_engine/utils/arrays.py`

 * *Files identical despite different names*

### Comparing `JaxFin-0.2.0.dev0/jaxfin/price_engine/utils/vect.py` & `JaxFin-0.3.0/jaxfin/price_engine/utils/vect.py`

 * *Files identical despite different names*

### Comparing `JaxFin-0.2.0.dev0/pyproject.toml` & `JaxFin-0.3.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -19,17 +19,15 @@
     "Topic :: Software Development :: Libraries :: Python Modules",
     "Intended Audience :: Financial and Insurance Industry",
     "Intended Audience :: Education",
     "Intended Audience :: Developers"
 ]
 dependencies = [
     "jax==0.4.23",
-    "jaxlib==0.4.23",
-    "numpy==1.26.2",
-    "scipy==1.11.4"
+    "jaxlib==0.4.23"
 ]
 dynamic = ["version"]
 
 [tool.setuptools.packages.find]
 include = ["jaxfin*"]
 exclude = ["examples*"]
 
@@ -584,7 +582,13 @@
 [tool.pytest.ini_options]
 pythonpath = [
     "."
 ]
 addopts = [
     "--import-mode=importlib",
 ]
+
+[tool.ruff]
+line-length = 120
+indent-width = 4
+
+target-version = "py312"
```

### Comparing `JaxFin-0.2.0.dev0/requirements/dev.txt` & `JaxFin-0.3.0/requirements/dev.txt`

 * *Files 2% similar despite different names*

```diff
@@ -86,15 +86,14 @@
 pluggy==1.3.0
 prometheus-client==0.19.0
 prompt-toolkit==3.0.43
 psutil==5.9.8
 pure-eval==0.2.2
 pycparser==2.21
 Pygments==2.17.2
-pylint==3.0.3
 pyparsing==3.1.1
 pytest==7.4.3
 pytest-html==4.1.1
 pytest-metadata==3.1.0
 python-dateutil==2.8.2
 python-json-logger==2.0.7
 pywin32==306
@@ -104,14 +103,15 @@
 qtconsole==5.5.1
 QtPy==2.4.1
 referencing==0.33.0
 requests==2.31.0
 rfc3339-validator==0.1.4
 rfc3986-validator==0.1.1
 rpds-py==0.17.1
+ruff==0.3.3
 SciencePlots==2.1.1
 scipy==1.11.4
 Send2Trash==1.8.2
 six==1.16.0
 sniffio==1.3.0
 soupsieve==2.5
 stack-data==0.6.3
```

### Comparing `JaxFin-0.2.0.dev0/scripts/create-new-version.bat` & `JaxFin-0.3.0/scripts/create-new-version.bat`

 * *Files identical despite different names*

### Comparing `JaxFin-0.2.0.dev0/tests/models/test_gbm.py` & `JaxFin-0.3.0/tests/models/test_gbm.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import jax.numpy as jnp
 
-from jaxfin.models.gbm import UnivGeometricBrownianMotion, MultiGeometricBrownianMotion
+from jaxfin.models.gbm import MultiGeometricBrownianMotion, UnivGeometricBrownianMotion
 
 SEED: int = 42
 
-class TestUnivGBM:
 
+class TestUnivGBM:
     def test_init(self):
         s0 = 10
         mean = 0.1
         sigma = 0.3
         dtype = jnp.float32
         gbm = UnivGeometricBrownianMotion(s0, mean, sigma, dtype)
 
@@ -27,15 +27,14 @@
 
         stock_paths = gbm.sample_paths(SEED, 1.0, 52, 100)
 
         assert stock_paths.shape == (52, 100)
 
 
 class TestMultiGBM:
-
     def test_init(self):
         s0 = jnp.array([10, 12])
         mean = jnp.array([0.1, 0.0])
         sigma = jnp.array([0.3, 0.5])
         corr = jnp.array([[1, 0.1], [0.1, 1]])
         dtype = jnp.float32
         gbm = MultiGeometricBrownianMotion(s0, mean, sigma, corr, dtype)
@@ -43,15 +42,14 @@
         assert jnp.array_equal(gbm.mean, mean)
         assert jnp.array_equal(gbm.sigma, sigma)
         assert jnp.array_equal(gbm.corr, corr)
         assert gbm.dtype == dtype
         assert jnp.array_equal(gbm.s0, s0)
         assert gbm.dimension == 2
 
-
     def test_sample_path(self):
         s0 = jnp.array([10, 12])
         mean = jnp.array([0.1, 0.0])
         sigma = jnp.array([0.3, 0.5])
         corr = jnp.array([[1, 0.1], [0.1, 1]])
         dtype = jnp.float32
         gbm = MultiGeometricBrownianMotion(s0, mean, sigma, corr, dtype)
```

### Comparing `JaxFin-0.2.0.dev0/tests/models/test_heston.py` & `JaxFin-0.3.0/tests/models/test_heston.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,25 +1,28 @@
 import jax.numpy as jnp
-from jaxfin.models.heston.heston import UnivHestonModel
+
+from jaxfin.models.heston.heston import MultiHestonModel, UnivHestonModel
 
 SEED: int = 42
 
-class TestUnivHestonModel():
 
+class TestUnivHestonModel:
     def test_init(self):
         s0 = 100
         v0 = 0.2
         mean = 0.2
         kappa = 2.0
         theta = 0.25
         sigma = 0.3
         rho = -0.7
         dtype = jnp.float32
 
-        heston_model = UnivHestonModel(s0, v0, mean, kappa, theta, sigma, rho, dtype=dtype)
+        heston_model = UnivHestonModel(
+            s0, v0, mean, kappa, theta, sigma, rho, dtype=dtype
+        )
 
         assert heston_model.mean == mean
         assert heston_model.kappa == kappa
         assert heston_model.theta == theta
         assert heston_model.sigma == sigma
         assert heston_model.rho == rho
         assert heston_model.dtype == dtype
@@ -31,11 +34,54 @@
         v0 = jnp.array(0.2, dtype=jnp.float32)
         mean = jnp.array(0.2, dtype=jnp.float32)
         kappa = jnp.array(2.0, dtype=jnp.float32)
         theta = jnp.array(0.25, dtype=jnp.float32)
         sigma = jnp.array(0.3, dtype=jnp.float32)
         rho = jnp.array(-0.7, dtype=jnp.float32)
 
-        heston_model = UnivHestonModel(s0, v0, mean, kappa, theta, sigma, rho, dtype=jnp.float32)
+        heston_model = UnivHestonModel(
+            s0, v0, mean, kappa, theta, sigma, rho, dtype=jnp.float32
+        )
         paths = heston_model.sample_paths(seed=SEED, maturity=1.0, n=100, n_sim=100)
 
         assert paths.shape == (100, 100)
+
+
+class TestMultiHestonModel:
+    def test_init(self):
+        s0 = jnp.array([100, 100], dtype=jnp.float32)
+        v0 = jnp.array([0.2, 0.2], dtype=jnp.float32)
+        mean = jnp.array([0.2, 0.2], dtype=jnp.float32)
+        kappa = jnp.array([2.0, 2.0], dtype=jnp.float32)
+        theta = jnp.array([0.25, 0.25], dtype=jnp.float32)
+        sigma = jnp.array([0.3, 0.3], dtype=jnp.float32)
+        corr = jnp.array([[1.0, 0.5], [0.5, 1.0]], dtype=jnp.float32)
+        dtype = jnp.float32
+
+        heston_model = MultiHestonModel(
+            s0, v0, mean, kappa, theta, sigma, corr, dtype=dtype
+        )
+
+        assert jnp.all(heston_model.mean == mean)
+        assert jnp.all(heston_model.kappa == kappa)
+        assert jnp.all(heston_model.theta == theta)
+        assert jnp.all(heston_model.sigma == sigma)
+        assert jnp.all(heston_model.corr == corr)
+        assert heston_model.dtype == dtype
+        assert jnp.all(heston_model.s0 == s0)
+        assert jnp.all(heston_model.v0 == v0)
+
+    def test_sample_paths(self):
+        s0 = jnp.array([100, 100], dtype=jnp.float32)
+        v0 = jnp.array([0.2, 0.2], dtype=jnp.float32)
+        mean = jnp.array([0.2, 0.2], dtype=jnp.float32)
+        kappa = jnp.array([2.0, 2.0], dtype=jnp.float32)
+        theta = jnp.array([0.25, 0.25], dtype=jnp.float32)
+        sigma = jnp.array([0.3, 0.3], dtype=jnp.float32)
+        corr = jnp.array([[1.0, 0.5], [0.5, 1.0]], dtype=jnp.float32)
+
+        heston_model = MultiHestonModel(
+            s0, v0, mean, kappa, theta, sigma, corr, dtype=jnp.float32
+        )
+        paths = heston_model.sample_paths(seed=SEED, maturity=1.0, n=100, n_sim=100)
+
+        assert paths.shape == (100, 100, 2)
```

### Comparing `JaxFin-0.2.0.dev0/tests/price_engine/test_black.py` & `JaxFin-0.3.0/tests/price_engine/test_black.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,28 +1,33 @@
 import jax.numpy as jnp
-
 import pytest
 
-from jaxfin.price_engine.black import future_option_price, future_option_delta, future_option_gamma
+from jaxfin.price_engine.black import (
+    future_option_delta,
+    future_option_gamma,
+    future_option_price,
+)
 from jaxfin.price_engine.utils.vect import get_vfunction
 
 TOL = 1e-3
 DTYPE = jnp.float32
 
+
 def test_one_future_option_float():
     spot = jnp.array(100, dtype=DTYPE)
     expire = jnp.array(1.0, dtype=DTYPE)
     vol = jnp.array(0.3, dtype=DTYPE)
     strike = jnp.array(110, dtype=DTYPE)
     risk_free_rate = jnp.array(0.0, dtype=DTYPE)
 
     price = future_option_price(spot, strike, expire, vol, risk_free_rate, dtype=DTYPE)
 
     assert price == 8.141014
 
+
 def test_one_future_option():
     spot = jnp.array([100], dtype=DTYPE)
     expire = jnp.array([1.0], dtype=DTYPE)
     vol = jnp.array([0.3], dtype=DTYPE)
     strike = jnp.array([110], dtype=DTYPE)
     risk_free_rate = jnp.array([0.0], dtype=DTYPE)
 
@@ -30,107 +35,139 @@
 
     assert price[0] == 8.141014
 
 
 def test_foption_batch_calls():
     spots = jnp.array([100, 90, 80, 110, 120], dtype=DTYPE)
     expires = jnp.array([1.0, 1.0, 1.0, 1.0, 1.0], dtype=DTYPE)
-    vols = jnp.array([.3, .25, .4, .2, .1], dtype=DTYPE)
+    vols = jnp.array([0.3, 0.25, 0.4, 0.2, 0.1], dtype=DTYPE)
     strikes = jnp.array([120, 120, 120, 120, 120], dtype=DTYPE)
     discount_rates = jnp.array([0.00, 0.00, 0.00, 0.00, 0.00], dtype=DTYPE)
 
-    prices = future_option_price(spots, strikes, expires, vols, discount_rates,
-                                  dtype=DTYPE)
+    prices = future_option_price(
+        spots, strikes, expires, vols, discount_rates, dtype=DTYPE
+    )
     expected = jnp.array([5.440567, 1.602787, 3.140933, 5.010391, 4.7853127])
 
     assert jnp.isclose(prices, expected, atol=TOL).all()
 
 
 def test_foption_batch_mixed():
     spots = jnp.array([100, 90, 80, 110, 120], dtype=DTYPE)
     expires = jnp.array([1.0, 1.0, 1.0, 1.0, 1.0], dtype=DTYPE)
-    vols = jnp.array([.3, .25, .4, .2, .1], dtype=DTYPE)
+    vols = jnp.array([0.3, 0.25, 0.4, 0.2, 0.1], dtype=DTYPE)
     strikes = jnp.array([120, 75, 75, 120, 120], dtype=DTYPE)
     are_calls = jnp.array([True, False, False, True, True], dtype=jnp.bool_)
     discount_rates = jnp.array([0.00, 0.00, 0.00, 0.00, 0.00], dtype=DTYPE)
 
-    prices = future_option_price(spots, strikes, expires, vols, discount_rates,
-                                 are_calls=are_calls, dtype=DTYPE)
+    prices = future_option_price(
+        spots, strikes, expires, vols, discount_rates, are_calls=are_calls, dtype=DTYPE
+    )
     expected = jnp.array([5.440567, 2.7794075, 9.942638, 5.010391, 4.7853127])
 
     assert jnp.isclose(prices, expected, atol=TOL).all()
 
 
 def test_foption_batch_mixed_disc():
     spots = jnp.array([100, 90, 80, 110, 120], dtype=DTYPE)
     expires = jnp.array([1.0, 1.0, 1.0, 1.0, 1.0], dtype=DTYPE)
-    vols = jnp.array([.3, .25, .4, .2, .1], dtype=DTYPE)
+    vols = jnp.array([0.3, 0.25, 0.4, 0.2, 0.1], dtype=DTYPE)
     strikes = jnp.array([120, 75, 75, 120, 120], dtype=DTYPE)
     are_calls = jnp.array([True, False, False, True, True], dtype=jnp.bool_)
     discount_rates = jnp.array([0.01, 0.0125, 0.02, 0.03, 0.05], dtype=DTYPE)
 
-    prices = future_option_price(spots, strikes, expires, vols,
-                                 are_calls=are_calls, discount_rates=discount_rates, dtype=DTYPE)
+    prices = future_option_price(
+        spots,
+        strikes,
+        expires,
+        vols,
+        are_calls=are_calls,
+        discount_rates=discount_rates,
+        dtype=DTYPE,
+    )
     expected = jnp.array([5.7082324, 2.5256162, 9.177393, 6.055744, 7.7550125])
 
     assert jnp.isclose(prices, expected, atol=TOL).all()
 
-class TestDelta:
 
+class TestDelta:
     def test_delta_float(self):
         spot = jnp.array(100, dtype=DTYPE)
         strike = jnp.array(120, dtype=DTYPE)
         expire = jnp.array(1, dtype=DTYPE)
         vol = jnp.array(0.3, dtype=DTYPE)
         rate = jnp.array(0.0, dtype=DTYPE)
         expected_delta = jnp.array(0.32357, dtype=DTYPE)
         expected_put_delta = jnp.array(-0.67643, dtype=DTYPE)
 
         call_delta = future_option_delta(spot, strike, expire, vol, rate)
-        put_delta = future_option_delta(spot, strike, expire, vol, rate, are_calls=False)
+        put_delta = future_option_delta(
+            spot, strike, expire, vol, rate, are_calls=False
+        )
 
         assert jnp.isclose(call_delta, expected_delta, atol=TOL)
         assert jnp.isclose(put_delta, expected_put_delta, atol=TOL)
 
     def test_delta(self):
         spots = jnp.array([100, 100, 100, 80, 170], dtype=DTYPE)
         strikes = jnp.array([120, 110, 120, 150, 160], dtype=DTYPE)
         expires = jnp.array([1, 1, 1, 0.5, 0.25], dtype=DTYPE)
         vols = jnp.array([0.3, 0.3, 0.2, 0.5, 0.15], dtype=DTYPE)
         rates = jnp.array([0.0, 0.0, 0.05, 0.02, 0.01], dtype=DTYPE)
         dividends = jnp.array([0.0, 0.0, 0.0, 0.0, 0.0], dtype=DTYPE)
         call_flags = jnp.array([True, True, True, True, True], dtype=jnp.bool_)
         put_flags = jnp.array([False, False, False, False, False], dtype=jnp.bool_)
-        e_call_deltas = jnp.array([0.32357, 0.43340, 0.28024, 0.05777, 0.81046], dtype=DTYPE)
-        e_put_deltas = jnp.array([-0.67643, -0.56659, -0.71975, -0.94222, -0.18953], dtype=DTYPE)
-        vmap_delta = get_vfunction(future_option_delta, spots, strikes, expires, vols, rates, dividends, are_calls=put_flags)
-
-        call_deltas = vmap_delta(spots, strikes, expires, vols, rates, dividends, call_flags)
-        put_deltas = vmap_delta(spots, strikes, expires, vols, rates, dividends, put_flags)
+        e_call_deltas = jnp.array(
+            [0.32357, 0.43340, 0.28024, 0.05777, 0.81046], dtype=DTYPE
+        )
+        e_put_deltas = jnp.array(
+            [-0.67643, -0.56659, -0.71975, -0.94222, -0.18953], dtype=DTYPE
+        )
+        vmap_delta = get_vfunction(
+            future_option_delta,
+            spots,
+            strikes,
+            expires,
+            vols,
+            rates,
+            dividends,
+            are_calls=put_flags,
+        )
+
+        call_deltas = vmap_delta(
+            spots, strikes, expires, vols, rates, dividends, call_flags
+        )
+        put_deltas = vmap_delta(
+            spots, strikes, expires, vols, rates, dividends, put_flags
+        )
 
         assert jnp.allclose(call_deltas, e_call_deltas, atol=TOL)
         assert jnp.allclose(put_deltas, e_put_deltas, atol=TOL)
 
 
-@pytest.mark.parametrize("spot, strike, expire, vol, rate, expected_gamma",
-                            [(100, 120, 1, 0.3, 0.0, 0.01197),
-                            (100, 110, 1, 0.3, 0.0, 0.013112),
-                            (100, 120, 1, 0.2, 0.01, 0.01523321),
-                            (80, 150, 0.5, 0.5, 0.02, 0.00417),
-                            (170, 160, 0.25, 0.15, 0.01, 0.02136)
-                            ])
+@pytest.mark.parametrize(
+    "spot, strike, expire, vol, rate, expected_gamma",
+    [
+        (100, 120, 1, 0.3, 0.0, 0.01197),
+        (100, 110, 1, 0.3, 0.0, 0.013112),
+        (100, 120, 1, 0.2, 0.01, 0.01523321),
+        (80, 150, 0.5, 0.5, 0.02, 0.00417),
+        (170, 160, 0.25, 0.15, 0.01, 0.02136),
+    ],
+)
 class TestGamma:
-
     def test_gamma_bs(self, spot, strike, expire, vol, rate, expected_gamma):
         spot = jnp.array(spot, dtype=DTYPE)
         strike = jnp.array(strike, dtype=DTYPE)
         expire = jnp.array(expire, dtype=DTYPE)
         vol = jnp.array(vol, dtype=DTYPE)
         rate = jnp.array(rate, dtype=DTYPE)
         dividends = jnp.array(0.0, dtype=DTYPE)
         put_flag = jnp.array(False, dtype=jnp.bool_)
         expected_gamma = jnp.array(expected_gamma, dtype=DTYPE)
         call_gamma = future_option_gamma(spot, strike, expire, vol, rate, dividends)
-        put_gamma = future_option_gamma(spot, strike, expire, vol, rate, dividends, are_calls=put_flag)
+        put_gamma = future_option_gamma(
+            spot, strike, expire, vol, rate, dividends, are_calls=put_flag
+        )
 
         assert jnp.isclose(call_gamma, expected_gamma, atol=TOL).all()
         assert jnp.isclose(put_gamma, call_gamma, atol=TOL).all()
```

### Comparing `JaxFin-0.2.0.dev0/tests/price_engine/test_bs.py` & `JaxFin-0.3.0/tests/price_engine/test_bs.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,21 +1,28 @@
-import jax.numpy as jnp
-
-from jaxfin.price_engine.black_scholes import european_price, delta_european, gamma_european, theta_european, rho_european, vega_european
-from jaxfin.price_engine.utils.vect import get_vfunction
-
 import logging
 
+import jax.numpy as jnp
 import pytest
 
+from jaxfin.price_engine.black_scholes import (
+    delta_european,
+    european_price,
+    gamma_european,
+    rho_european,
+    theta_european,
+    vega_european,
+)
+from jaxfin.price_engine.utils.vect import get_vfunction
+
 TOL = 1e-3
 DTYPE = jnp.float32
 
 logging.basicConfig(level=logging.INFO)
 
+
 def test_one_vanilla():
     dtype = jnp.float32
     spot = jnp.array([100], dtype=dtype)
     expire = jnp.array([1.0], dtype=dtype)
     vol = jnp.array([0.3], dtype=dtype)
     strike = jnp.array([110], dtype=dtype)
     risk_free_rate = jnp.array([0.0], dtype=dtype)
@@ -24,64 +31,76 @@
 
     assert price[0] == 8.141014
 
 
 def test_vanilla_batch_calls():
     spots = jnp.array([100, 90, 80, 110, 120], dtype=DTYPE)
     expires = jnp.array([1.0, 1.0, 1.0, 1.0, 1.0], dtype=DTYPE)
-    vols = jnp.array([.3, .25, .4, .2, .1], dtype=DTYPE)
+    vols = jnp.array([0.3, 0.25, 0.4, 0.2, 0.1], dtype=DTYPE)
     strikes = jnp.array([120, 120, 120, 120, 120], dtype=DTYPE)
     discount_rates = jnp.array([0.00, 0.00, 0.00, 0.00, 0.00], dtype=DTYPE)
 
     prices = european_price(spots, strikes, expires, vols, discount_rates, dtype=DTYPE)
     expected = jnp.array([5.440567, 1.602787, 3.140933, 5.010391, 4.7853127])
 
     assert jnp.isclose(prices, expected, atol=TOL).all()
 
 
 def test_vanilla_batch_mixed():
     spots = jnp.array([100, 90, 80, 110, 120], dtype=DTYPE)
     expires = jnp.array([1.0, 1.0, 1.0, 1.0, 1.0], dtype=DTYPE)
-    vols = jnp.array([.3, .25, .4, .2, .1], dtype=DTYPE)
+    vols = jnp.array([0.3, 0.25, 0.4, 0.2, 0.1], dtype=DTYPE)
     strikes = jnp.array([120, 75, 75, 120, 120], dtype=DTYPE)
     are_calls = jnp.array([True, False, False, True, True], dtype=jnp.bool_)
     discount_rates = jnp.array([0.00, 0.00, 0.00, 0.00, 0.00], dtype=DTYPE)
 
-    prices = european_price(spots, strikes, expires, vols, discount_rates,
-                            are_calls=are_calls, dtype=DTYPE)
+    prices = european_price(
+        spots, strikes, expires, vols, discount_rates, are_calls=are_calls, dtype=DTYPE
+    )
     expected = jnp.array([5.440567, 2.7794075, 9.942638, 5.010391, 4.7853127])
 
     assert jnp.isclose(prices, expected, atol=TOL).all()
 
 
 def test_vanilla_batch_mixed_disc():
     spots = jnp.array([100, 90, 80, 110, 120], dtype=DTYPE)
     expires = jnp.array([1.0, 1.0, 1.0, 1.0, 1.0], dtype=DTYPE)
-    vols = jnp.array([.3, .25, .4, .2, .1], dtype=DTYPE)
+    vols = jnp.array([0.3, 0.25, 0.4, 0.2, 0.1], dtype=DTYPE)
     strikes = jnp.array([120, 75, 75, 120, 120], dtype=DTYPE)
     are_calls = jnp.array([True, False, False, True, True], dtype=jnp.bool_)
     discount_rates = jnp.array([0.01, 0.0125, 0.02, 0.03, 0.05], dtype=DTYPE)
 
-    prices = european_price(spots, strikes, expires, vols,
-                            are_calls=are_calls, discount_rates=discount_rates, dtype=DTYPE)
-    expected = jnp.array([5.714386,  2.5328674, 9.19194, 6.155064, 8.165947])
+    prices = european_price(
+        spots,
+        strikes,
+        expires,
+        vols,
+        are_calls=are_calls,
+        discount_rates=discount_rates,
+        dtype=DTYPE,
+    )
+    expected = jnp.array([5.714386, 2.5328674, 9.19194, 6.155064, 8.165947])
 
     assert jnp.isclose(prices, expected, atol=TOL).all()
 
+
 ### Test Greeks Calculations ###
 
-@pytest.mark.parametrize("spot, strike, expire, vol, rate, e_call_delta, e_put_delta",
-                         [(100, 120, 1, 0.3, 0.0, 0.32357, -0.67643),
-                          (100, 110, 1, 0.3, 0.0, 0.43341, -0.56659),
-                          (100, 120, 1, 0.2, 0.05, 0.28719, -0.71281),
-                          (80, 150, 0.5, 0.5, 0.02, 0.05787, -0.94213),
-                          (170, 160, 0.25, 0.15, 0.01, 0.81034, -0.18966)
-                        ])
-class TestDelta:
 
+@pytest.mark.parametrize(
+    "spot, strike, expire, vol, rate, e_call_delta, e_put_delta",
+    [
+        (100, 120, 1, 0.3, 0.0, 0.32357, -0.67643),
+        (100, 110, 1, 0.3, 0.0, 0.43341, -0.56659),
+        (100, 120, 1, 0.2, 0.05, 0.28719, -0.71281),
+        (80, 150, 0.5, 0.5, 0.02, 0.05787, -0.94213),
+        (170, 160, 0.25, 0.15, 0.01, 0.81034, -0.18966),
+    ],
+)
+class TestDelta:
     def test_delta_bs(self, spot, strike, expire, vol, rate, e_call_delta, e_put_delta):
         spot = jnp.array(spot, dtype=DTYPE)
         strike = jnp.array(strike, dtype=DTYPE)
         expire = jnp.array(expire, dtype=DTYPE)
         vol = jnp.array(vol, dtype=DTYPE)
         rate = jnp.array(rate, dtype=DTYPE)
         put_flag = jnp.array(False, dtype=jnp.bool_)
@@ -90,101 +109,115 @@
         put_delta = delta_european(spot, strike, expire, vol, rate, are_calls=put_flag)
 
         assert jnp.isclose(call_delta, e_call_delta, atol=TOL).all()
         assert jnp.isclose(put_delta, e_put_delta, atol=TOL).all()
         assert jnp.isclose(call_delta - 1.0, put_delta, atol=TOL).all()
 
 
-
 class TestDeltaBatch:
-
     def test_delta_bs_scalar(self):
         spot = jnp.array(100, dtype=DTYPE)
         strike = jnp.array(120, dtype=DTYPE)
         expire = jnp.array(1, dtype=DTYPE)
         vol = jnp.array(0.3, dtype=DTYPE)
         rate = jnp.array(0.0, dtype=DTYPE)
         expected_delta = jnp.array(0.32357, dtype=DTYPE)
         expected_put_delta = jnp.array(-0.67643, dtype=DTYPE)
 
-        logging.info(f"Testing with spot={spot}, strike={strike}, expire={expire}, vol={vol}, rate={rate}")
+        logging.info(
+            f"Testing with spot={spot}, strike={strike}, expire={expire}, vol={vol}, rate={rate}"
+        )
 
         call_delta = delta_european(spot, strike, expire, vol, rate)
         put_delta = delta_european(spot, strike, expire, vol, rate, are_calls=False)
 
         assert jnp.isclose(call_delta, expected_delta, atol=TOL)
         assert jnp.isclose(put_delta, expected_put_delta, atol=TOL)
         assert jnp.isclose(call_delta - 1.0, put_delta, atol=TOL)
 
     def test_delta_bs_batch(self):
         spots = jnp.array([100, 90, 80, 110, 120], dtype=DTYPE)
         expires = jnp.array([1.0, 1.0, 1.0, 1.0, 1.0], dtype=DTYPE)
-        vols = jnp.array([.3, .25, .4, .2, .1], dtype=DTYPE)
+        vols = jnp.array([0.3, 0.25, 0.4, 0.2, 0.1], dtype=DTYPE)
         strikes = jnp.array([120, 120, 120, 120, 120], dtype=DTYPE)
         discount_rates = jnp.array([0.00, 0.00, 0.00, 0.00, 0.00], dtype=DTYPE)
         call_flag = jnp.array([True, True, True, True, True], dtype=jnp.bool_)
 
-        vmap_delta = get_vfunction(delta_european, spots, strikes, expires, vols, discount_rates, call_flag)
-
-        logging.info(f"Testing with spots={spots}, strikes={strikes}, expires={expires}, vols={vols}, rates={discount_rates}")
-
-        call_delta = vmap_delta(spots, strikes, expires, vols, discount_rates, call_flag)
+        vmap_delta = get_vfunction(
+            delta_european, spots, strikes, expires, vols, discount_rates, call_flag
+        )
+
+        logging.info(
+            f"Testing with spots={spots}, strikes={strikes}, expires={expires}, vols={vols}, rates={discount_rates}"
+        )
+
+        call_delta = vmap_delta(
+            spots, strikes, expires, vols, discount_rates, call_flag
+        )
         put_flag = jnp.array([False, False, False, False, False], dtype=jnp.bool_)
         put_delta = vmap_delta(spots, strikes, expires, vols, discount_rates, put_flag)
 
         expected_call = jnp.array([0.323570, 0.152509, 0.207919, 0.36879, 0.51993])
         expected_put = jnp.array([-0.676429, -0.847490, -0.79208, -0.63120, -0.480061])
 
         assert jnp.isclose(call_delta, expected_call, atol=TOL).all()
         assert jnp.isclose(put_delta, expected_put, atol=TOL).all()
         assert jnp.isclose(call_delta - 1.0, put_delta, atol=TOL).all()
 
-@pytest.mark.parametrize("spot, strike, expire, vol, rate, expected_gamma",
-                            [(100, 120, 1, 0.3, 0.0, 0.01198),
-                            (100, 110, 1, 0.3, 0.0, 0.01311),
-                            (100, 120, 1, 0.2, 0.05, 0.01704),
-                            (80, 150, 0.5, 0.5, 0.02, 0.00409),
-                            (170, 160, 0.25, 0.15, 0.01, 0.02126)
-                            ])
-class TestGamma:
 
+@pytest.mark.parametrize(
+    "spot, strike, expire, vol, rate, expected_gamma",
+    [
+        (100, 120, 1, 0.3, 0.0, 0.01198),
+        (100, 110, 1, 0.3, 0.0, 0.01311),
+        (100, 120, 1, 0.2, 0.05, 0.01704),
+        (80, 150, 0.5, 0.5, 0.02, 0.00409),
+        (170, 160, 0.25, 0.15, 0.01, 0.02126),
+    ],
+)
+class TestGamma:
     def test_gamma_bs(self, spot, strike, expire, vol, rate, expected_gamma):
         spot = jnp.array(spot, dtype=DTYPE)
         strike = jnp.array(strike, dtype=DTYPE)
         expire = jnp.array(expire, dtype=DTYPE)
         vol = jnp.array(vol, dtype=DTYPE)
         rate = jnp.array(rate, dtype=DTYPE)
         gamma = gamma_european(spot, strike, expire, vol, rate)
 
         assert jnp.isclose(gamma, expected_gamma, atol=TOL).all()
 
-class TestGammaBatch:
 
+class TestGammaBatch:
     def test_gamma_bs_vectorized(self):
         spots = jnp.array([100, 100, 100, 80, 170], dtype=DTYPE)
         strikes = jnp.array([120, 110, 120, 150, 160], dtype=DTYPE)
         expires = jnp.array([1, 1, 1, 0.5, 0.25], dtype=DTYPE)
         vols = jnp.array([0.3, 0.3, 0.2, 0.5, 0.15], dtype=DTYPE)
         rates = jnp.array([0.0, 0.0, 0.05, 0.02, 0.01], dtype=DTYPE)
-        expected_gammas = jnp.array([0.01198, 0.01311, 0.01704, 0.00409, 0.02126], dtype=DTYPE)
+        expected_gammas = jnp.array(
+            [0.01198, 0.01311, 0.01704, 0.00409, 0.02126], dtype=DTYPE
+        )
         vmap_gamma = get_vfunction(gamma_european, spots, strikes, expires, vols, rates)
 
         gammas = vmap_gamma(spots, strikes, expires, vols, rates)
 
         assert jnp.allclose(gammas, expected_gammas, atol=TOL)
 
-@pytest.mark.parametrize("spot, strike, expire, vol, rate, e_call_theta, e_put_theta",
-                            [(100, 120, 1, 0.3, 0.0, 5.38894, 5.38894),
-                            (100, 110, 1, 0.3, 0.0, 5.90058, 5.90058),
-                            (100, 120, 1, 0.2, 0.05, 4.68097, -1.02641),
-                            (80, 150, 0.5, 0.5, 0.02, 3.35533, 0.38519),
-                            (170, 160, 0.25, 0.15, 0.01, 8.17193, 6.57593)
-                            ])
-class TestTheta:
 
+@pytest.mark.parametrize(
+    "spot, strike, expire, vol, rate, e_call_theta, e_put_theta",
+    [
+        (100, 120, 1, 0.3, 0.0, 5.38894, 5.38894),
+        (100, 110, 1, 0.3, 0.0, 5.90058, 5.90058),
+        (100, 120, 1, 0.2, 0.05, 4.68097, -1.02641),
+        (80, 150, 0.5, 0.5, 0.02, 3.35533, 0.38519),
+        (170, 160, 0.25, 0.15, 0.01, 8.17193, 6.57593),
+    ],
+)
+class TestTheta:
     def test_theta_bs(self, spot, strike, expire, vol, rate, e_call_theta, e_put_theta):
         spot = jnp.array(spot, dtype=DTYPE)
         strike = jnp.array(strike, dtype=DTYPE)
         expire = jnp.array(expire, dtype=DTYPE)
         vol = jnp.array(vol, dtype=DTYPE)
         rate = jnp.array(rate, dtype=DTYPE)
         put_flag = jnp.array(False, dtype=jnp.bool_)
@@ -192,48 +225,54 @@
         e_put_theta = jnp.array(e_put_theta, dtype=DTYPE)
         theta = theta_european(spot, strike, expire, vol, rate)
         p_theta = theta_european(spot, strike, expire, vol, rate, are_calls=put_flag)
 
         assert jnp.isclose(theta, e_call_theta, atol=TOL).all()
         assert jnp.isclose(p_theta, e_put_theta, atol=TOL).all()
 
-@pytest.mark.parametrize("spot, strike, expire, vol, rate, e_call_rho, e_put_rho",
-                            [(100, 120, 1, 0.3, 0.0, 26.91644, -93.08356),
-                            (100, 110, 1, 0.3, 0.0, 35.19993, -74.80007),
-                            (100, 120, 1, 0.2, 0.05, 25.47168, -88.67585),
-                            (80, 150, 0.5, 0.5, 0.02, 2.00656, -72.24718),
-                            (170, 160, 0.25, 0.15, 0.01, 31.49509, -8.40503)
-                            ]) 
-class TestRho:
 
+@pytest.mark.parametrize(
+    "spot, strike, expire, vol, rate, e_call_rho, e_put_rho",
+    [
+        (100, 120, 1, 0.3, 0.0, 26.91644, -93.08356),
+        (100, 110, 1, 0.3, 0.0, 35.19993, -74.80007),
+        (100, 120, 1, 0.2, 0.05, 25.47168, -88.67585),
+        (80, 150, 0.5, 0.5, 0.02, 2.00656, -72.24718),
+        (170, 160, 0.25, 0.15, 0.01, 31.49509, -8.40503),
+    ],
+)
+class TestRho:
     def test_rho_bs(self, spot, strike, expire, vol, rate, e_call_rho, e_put_rho):
         spot = jnp.array(spot, dtype=DTYPE)
         strike = jnp.array(strike, dtype=DTYPE)
         expire = jnp.array(expire, dtype=DTYPE)
         vol = jnp.array(vol, dtype=DTYPE)
         rate = jnp.array(rate, dtype=DTYPE)
         put_flag = jnp.array(False, dtype=jnp.bool_)
         e_call_rho = jnp.array(e_call_rho, dtype=DTYPE)
         call_rho = rho_european(spot, strike, expire, vol, rate)
         put_rho = rho_european(spot, strike, expire, vol, rate, are_calls=put_flag)
 
         assert jnp.isclose(call_rho, e_call_rho, atol=TOL).all()
         assert jnp.isclose(put_rho, e_put_rho, atol=TOL).all()
 
-@pytest.mark.parametrize("spot, strike, expire, vol, rate, expected_vega",
-                            [(100, 120, 1, 0.3, 0.0, 35.92629),
-                            (100, 110, 1, 0.3, 0.0, 39.33717),
-                            (100, 120, 1, 0.2, 0.05, 34.07384),
-                            (80, 150, 0.5, 0.5, 0.02, 6.55014),
-                            (170, 160, 0.25, 0.15, 0.01, 23.04042)
-                            ])
+
+@pytest.mark.parametrize(
+    "spot, strike, expire, vol, rate, expected_vega",
+    [
+        (100, 120, 1, 0.3, 0.0, 35.92629),
+        (100, 110, 1, 0.3, 0.0, 39.33717),
+        (100, 120, 1, 0.2, 0.05, 34.07384),
+        (80, 150, 0.5, 0.5, 0.02, 6.55014),
+        (170, 160, 0.25, 0.15, 0.01, 23.04042),
+    ],
+)
 class TestVega:
-    
-        def test_vega_bs(self, spot, strike, expire, vol, rate, expected_vega):
-            spot = jnp.array(spot, dtype=DTYPE)
-            strike = jnp.array(strike, dtype=DTYPE)
-            expire = jnp.array(expire, dtype=DTYPE)
-            vol = jnp.array(vol, dtype=DTYPE)
-            rate = jnp.array(rate, dtype=DTYPE)
-            vega = vega_european(spot, strike, expire, vol, rate)
-    
-            assert jnp.isclose(vega, expected_vega, atol=TOL).all()
+    def test_vega_bs(self, spot, strike, expire, vol, rate, expected_vega):
+        spot = jnp.array(spot, dtype=DTYPE)
+        strike = jnp.array(strike, dtype=DTYPE)
+        expire = jnp.array(expire, dtype=DTYPE)
+        vol = jnp.array(vol, dtype=DTYPE)
+        rate = jnp.array(rate, dtype=DTYPE)
+        vega = vega_european(spot, strike, expire, vol, rate)
+
+        assert jnp.isclose(vega, expected_vega, atol=TOL).all()
```

