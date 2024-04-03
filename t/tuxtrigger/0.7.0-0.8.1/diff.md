# Comparing `tmp/tuxtrigger-0.7.0.tar.gz` & `tmp/tuxtrigger-0.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tuxtrigger-0.7.0.tar", last modified: Tue Sep 26 12:29:50 2023, max compression
+gzip compressed data, was "tuxtrigger-0.8.1.tar", last modified: Wed Apr  3 07:25:19 2024, max compression
```

## Comparing `tuxtrigger-0.7.0.tar` & `tuxtrigger-0.8.1.tar`

### file list

```diff
@@ -1,55 +1,68 @@
--rw-r--r--   0        0        0       81 2023-09-26 12:29:49.510225 tuxtrigger-0.7.0/.flake8
--rw-r--r--   0        0        0       95 2023-09-26 12:29:49.511225 tuxtrigger-0.7.0/.gitignore
--rw-r--r--   0        0        0     1242 2023-09-26 12:29:49.511225 tuxtrigger-0.7.0/.gitlab-ci.yml
--rw-r--r--   0        0        0      427 2023-09-26 12:29:49.511225 tuxtrigger-0.7.0/Dockerfile
--rw-r--r--   0        0        0      135 2023-09-26 12:29:49.511225 tuxtrigger-0.7.0/Dockerfile.ci
--rw-r--r--   0        0        0      752 2023-09-26 12:29:49.511225 tuxtrigger-0.7.0/Dockerfile.ci-debian
--rw-r--r--   0        0        0      469 2023-09-26 12:29:49.511225 tuxtrigger-0.7.0/Dockerfile.ci-fedora
--rw-r--r--   0        0        0     1054 2023-09-26 12:29:49.511225 tuxtrigger-0.7.0/LICENSE
--rw-r--r--   0        0        0      458 2023-09-26 12:29:49.511225 tuxtrigger-0.7.0/Makefile
--rw-r--r--   0        0        0     2168 2023-09-26 12:29:49.511225 tuxtrigger-0.7.0/README.md
--rw-r--r--   0        0        0      151 2023-09-26 12:29:49.511225 tuxtrigger-0.7.0/debian/changelog
--rw-r--r--   0        0        0      961 2023-09-26 12:29:49.511225 tuxtrigger-0.7.0/debian/control
--rw-r--r--   0        0        0      100 2023-09-26 12:29:49.511225 tuxtrigger-0.7.0/debian/gbp.conf
--rwxr-xr-x   0        0        0      105 2023-09-26 12:29:49.511225 tuxtrigger-0.7.0/debian/rules
--rw-r--r--   0        0        0       12 2023-09-26 12:29:49.511225 tuxtrigger-0.7.0/debian/source/format
--rw-r--r--   0        0        0      635 2023-09-26 12:29:49.511225 tuxtrigger-0.7.0/docs/install-deb.md
--rw-r--r--   0        0        0      377 2023-09-26 12:29:49.511225 tuxtrigger-0.7.0/docs/install-pypi.md
--rw-r--r--   0        0        0      663 2023-09-26 12:29:49.511225 tuxtrigger-0.7.0/docs/install-rpm.md
--rw-r--r--   0        0        0      519 2023-09-26 12:29:49.511225 tuxtrigger-0.7.0/docs/run-uninstalled.md
--rw-r--r--   0        0        0     2465 2023-09-26 12:29:49.511225 tuxtrigger-0.7.0/docs/run.md
--rw-r--r--   0        0        0     3394 2023-09-26 12:29:49.511225 tuxtrigger-0.7.0/docs/subcommands.md
--rw-r--r--   0        0        0      774 2023-09-26 12:29:49.511225 tuxtrigger-0.7.0/mkdocs.yml
--rw-r--r--   0        0        0       36 2023-09-26 12:29:49.511225 tuxtrigger-0.7.0/mypy.ini
--rw-r--r--   0        0        0      510 2023-09-26 12:29:49.511225 tuxtrigger-0.7.0/pyproject.toml
--rw-r--r--   0        0        0       50 2023-09-26 12:29:49.511225 tuxtrigger-0.7.0/requirements-dev.txt
--rw-r--r--   0        0        0       28 2023-09-26 12:29:49.511225 tuxtrigger-0.7.0/requirements.txt
--rwxr-xr-x   0        0        0      125 2023-09-26 12:29:49.512225 tuxtrigger-0.7.0/run
--rwxr-xr-x   0        0        0      166 2023-09-26 12:29:49.512225 tuxtrigger-0.7.0/scripts/readme2index.sh
--rw-r--r--   0        0        0       75 2023-09-26 12:29:49.512225 tuxtrigger-0.7.0/test/__init__.py
--rw-r--r--   0        0        0     1528 2023-09-26 12:29:49.512225 tuxtrigger-0.7.0/test/conftest.py
--rw-r--r--   0        0        0      650 2023-09-26 12:29:49.512225 tuxtrigger-0.7.0/test/test_argparser.py
--rw-r--r--   0        0        0     7395 2023-09-26 12:29:49.512225 tuxtrigger-0.7.0/test/test_builder.py
--rw-r--r--   0        0        0      678 2023-09-26 12:29:49.512225 tuxtrigger-0.7.0/test/test_exceptions.py
--rw-r--r--   0        0        0      292 2023-09-26 12:29:49.512225 tuxtrigger-0.7.0/test/test_files/error_path.yaml
--rw-r--r--   0        0        0      491 2023-09-26 12:29:49.512225 tuxtrigger-0.7.0/test/test_files/gitsha.yaml
--rw-r--r--   0        0        0      379 2023-09-26 12:29:49.512225 tuxtrigger-0.7.0/test/test_files/gitsha2.yaml
--rw-r--r--   0        0        0     1058 2023-09-26 12:29:49.512225 tuxtrigger-0.7.0/test/test_files/happy_path.yaml
--rw-r--r--   0        0        0    82080 2023-09-26 12:29:49.512225 tuxtrigger-0.7.0/test/test_files/manifest.js.gz
--rw-r--r--   0        0        0      125 2023-09-26 12:29:49.512225 tuxtrigger-0.7.0/test/test_files/planTest.yaml
--rw-r--r--   0        0        0      163 2023-09-26 12:29:49.512225 tuxtrigger-0.7.0/test/test_files/test.json
--rw-r--r--   0        0        0    12215 2023-09-26 12:29:49.512225 tuxtrigger-0.7.0/test/test_main.py
--rw-r--r--   0        0        0     2724 2023-09-26 12:29:49.512225 tuxtrigger-0.7.0/test/test_manifest.py
--rw-r--r--   0        0        0     1983 2023-09-26 12:29:49.512225 tuxtrigger-0.7.0/test/test_request.py
--rw-r--r--   0        0        0     7825 2023-09-26 12:29:49.513225 tuxtrigger-0.7.0/test/test_yamlload.py
--rw-r--r--   0        0        0     1579 2023-09-26 12:29:49.513225 tuxtrigger-0.7.0/tuxtrigger.spec
--rw-r--r--   0        0        0      134 2023-09-26 12:29:49.513225 tuxtrigger-0.7.0/tuxtrigger/__init__.py
--rw-r--r--   0        0        0     7979 2023-09-26 12:29:49.513225 tuxtrigger-0.7.0/tuxtrigger/__main__.py
--rw-r--r--   0        0        0     2401 2023-09-26 12:29:49.513225 tuxtrigger-0.7.0/tuxtrigger/argparser.py
--rw-r--r--   0        0        0    10713 2023-09-26 12:29:49.513225 tuxtrigger-0.7.0/tuxtrigger/builder.py
--rw-r--r--   0        0        0      454 2023-09-26 12:29:49.513225 tuxtrigger-0.7.0/tuxtrigger/exceptions.py
--rw-r--r--   0        0        0      856 2023-09-26 12:29:49.513225 tuxtrigger-0.7.0/tuxtrigger/inputvalidation.py
--rw-r--r--   0        0        0     2275 2023-09-26 12:29:49.513225 tuxtrigger-0.7.0/tuxtrigger/manifest.py
--rw-r--r--   0        0        0      890 2023-09-26 12:29:49.513225 tuxtrigger-0.7.0/tuxtrigger/request.py
--rw-r--r--   0        0        0     5896 2023-09-26 12:29:49.513225 tuxtrigger-0.7.0/tuxtrigger/yamlload.py
--rw-r--r--   0        0        0     2594 1970-01-01 00:00:00.000000 tuxtrigger-0.7.0/PKG-INFO
+-rw-r--r--   0        0        0       81 2024-04-03 07:25:18.460079 tuxtrigger-0.8.1/.flake8
+-rw-r--r--   0        0        0       86 2024-04-03 07:25:18.461079 tuxtrigger-0.8.1/.gitignore
+-rw-r--r--   0        0        0     1590 2024-04-03 07:25:18.461079 tuxtrigger-0.8.1/.gitlab-ci.yml
+-rw-r--r--   0        0        0       27 2024-04-03 07:25:18.461079 tuxtrigger-0.8.1/.isort.cfg
+-rw-r--r--   0        0        0      428 2024-04-03 07:25:18.461079 tuxtrigger-0.8.1/Dockerfile
+-rw-r--r--   0        0        0      141 2024-04-03 07:25:18.461079 tuxtrigger-0.8.1/Dockerfile.ci
+-rw-r--r--   0        0        0      761 2024-04-03 07:25:18.461079 tuxtrigger-0.8.1/Dockerfile.ci-debian
+-rw-r--r--   0        0        0      469 2024-04-03 07:25:18.461079 tuxtrigger-0.8.1/Dockerfile.ci-fedora
+-rw-r--r--   0        0        0     1054 2024-04-03 07:25:18.461079 tuxtrigger-0.8.1/LICENSE
+-rw-r--r--   0        0        0      605 2024-04-03 07:25:18.461079 tuxtrigger-0.8.1/Makefile
+-rw-r--r--   0        0        0     2199 2024-04-03 07:25:18.461079 tuxtrigger-0.8.1/README.md
+-rw-r--r--   0        0        0      151 2024-04-03 07:25:18.461079 tuxtrigger-0.8.1/debian/changelog
+-rw-r--r--   0        0        0      963 2024-04-03 07:25:18.461079 tuxtrigger-0.8.1/debian/control
+-rw-r--r--   0        0        0      100 2024-04-03 07:25:18.461079 tuxtrigger-0.8.1/debian/gbp.conf
+-rwxr-xr-x   0        0        0      105 2024-04-03 07:25:18.461079 tuxtrigger-0.8.1/debian/rules
+-rw-r--r--   0        0        0       12 2024-04-03 07:25:18.461079 tuxtrigger-0.8.1/debian/source/format
+-rw-r--r--   0        0        0      635 2024-04-03 07:25:18.461079 tuxtrigger-0.8.1/docs/install-deb.md
+-rw-r--r--   0        0        0      377 2024-04-03 07:25:18.461079 tuxtrigger-0.8.1/docs/install-pypi.md
+-rw-r--r--   0        0        0      663 2024-04-03 07:25:18.461079 tuxtrigger-0.8.1/docs/install-rpm.md
+-rw-r--r--   0        0        0      519 2024-04-03 07:25:18.461079 tuxtrigger-0.8.1/docs/run-uninstalled.md
+-rw-r--r--   0        0        0     3817 2024-04-03 07:25:18.461079 tuxtrigger-0.8.1/docs/run.md
+-rw-r--r--   0        0        0     4401 2024-04-03 07:25:18.461079 tuxtrigger-0.8.1/docs/subcommands.md
+-rw-r--r--   0        0        0      836 2024-04-03 07:25:18.461079 tuxtrigger-0.8.1/mkdocs.yml
+-rw-r--r--   0        0        0       36 2024-04-03 07:25:18.461079 tuxtrigger-0.8.1/mypy.ini
+-rw-r--r--   0        0        0      508 2024-04-03 07:25:18.462079 tuxtrigger-0.8.1/pyproject.toml
+-rw-r--r--   0        0        0       50 2024-04-03 07:25:18.462079 tuxtrigger-0.8.1/requirements-dev.txt
+-rw-r--r--   0        0        0       38 2024-04-03 07:25:18.462079 tuxtrigger-0.8.1/requirements.txt
+-rwxr-xr-x   0        0        0      126 2024-04-03 07:25:18.462079 tuxtrigger-0.8.1/run
+-rwxr-xr-x   0        0        0      166 2024-04-03 07:25:18.462079 tuxtrigger-0.8.1/scripts/readme2index.sh
+-rw-r--r--   0        0        0       75 2024-04-03 07:25:18.462079 tuxtrigger-0.8.1/test/__init__.py
+-rw-r--r--   0        0        0     3611 2024-04-03 07:25:18.462079 tuxtrigger-0.8.1/test/conftest.py
+-rw-r--r--   0        0        0      647 2024-04-03 07:25:18.462079 tuxtrigger-0.8.1/test/test_argparser.py
+-rw-r--r--   0        0        0    10902 2024-04-03 07:25:18.462079 tuxtrigger-0.8.1/test/test_configparser.py
+-rw-r--r--   0        0        0      678 2024-04-03 07:25:18.462079 tuxtrigger-0.8.1/test/test_exceptions.py
+-rw-r--r--   0        0        0      292 2024-04-03 07:25:18.462079 tuxtrigger-0.8.1/test/test_files/error_path.yaml
+-rw-r--r--   0        0        0      163 2024-04-03 07:25:18.462079 tuxtrigger-0.8.1/test/test_files/example_project_test-rc.json
+-rw-r--r--   0        0        0      472 2024-04-03 07:25:18.462079 tuxtrigger-0.8.1/test/test_files/gitsha.yaml
+-rw-r--r--   0        0        0      379 2024-04-03 07:25:18.462079 tuxtrigger-0.8.1/test/test_files/gitsha2.yaml
+-rw-r--r--   0        0        0     1246 2024-04-03 07:25:18.462079 tuxtrigger-0.8.1/test/test_files/happy_path.yaml
+-rw-r--r--   0        0        0      509 2024-04-03 07:25:18.462079 tuxtrigger-0.8.1/test/test_files/happy_path2.yaml
+-rw-r--r--   0        0        0    82080 2024-04-03 07:25:18.462079 tuxtrigger-0.8.1/test/test_files/manifest.js.gz
+-rw-r--r--   0        0        0      125 2024-04-03 07:25:18.462079 tuxtrigger-0.8.1/test/test_files/planTest.yaml
+-rw-r--r--   0        0        0      163 2024-04-03 07:25:18.462079 tuxtrigger-0.8.1/test/test_files/test.json
+-rw-r--r--   0        0        0     2734 2024-04-03 07:25:18.462079 tuxtrigger-0.8.1/test/test_inputvalidation.py
+-rw-r--r--   0        0        0     5841 2024-04-03 07:25:18.463079 tuxtrigger-0.8.1/test/test_main.py
+-rw-r--r--   0        0        0     1974 2024-04-03 07:25:18.463079 tuxtrigger-0.8.1/test/test_manifest.py
+-rw-r--r--   0        0        0     8526 2024-04-03 07:25:18.463079 tuxtrigger-0.8.1/test/test_repository.py
+-rw-r--r--   0        0        0     2058 2024-04-03 07:25:18.463079 tuxtrigger-0.8.1/test/test_request.py
+-rw-r--r--   0        0        0     4257 2024-04-03 07:25:18.463079 tuxtrigger-0.8.1/test/test_storage.py
+-rw-r--r--   0        0        0     9162 2024-04-03 07:25:18.463079 tuxtrigger-0.8.1/test/test_tuxintegration.py
+-rw-r--r--   0        0        0     3463 2024-04-03 07:25:18.463079 tuxtrigger-0.8.1/test/test_utils.py
+-rw-r--r--   0        0        0     1077 2024-04-03 07:25:18.463079 tuxtrigger-0.8.1/test/test_yamlload.py
+-rw-r--r--   0        0        0     1580 2024-04-03 07:25:18.463079 tuxtrigger-0.8.1/tuxtrigger.spec
+-rw-r--r--   0        0        0      134 2024-04-03 07:25:18.463079 tuxtrigger-0.8.1/tuxtrigger/__init__.py
+-rw-r--r--   0        0        0     3613 2024-04-03 07:25:18.463079 tuxtrigger-0.8.1/tuxtrigger/__main__.py
+-rw-r--r--   0        0        0     2683 2024-04-03 07:25:18.463079 tuxtrigger-0.8.1/tuxtrigger/argparser.py
+-rw-r--r--   0        0        0     4929 2024-04-03 07:25:18.463079 tuxtrigger-0.8.1/tuxtrigger/configparser.py
+-rw-r--r--   0        0        0      671 2024-04-03 07:25:18.463079 tuxtrigger-0.8.1/tuxtrigger/constants.py
+-rw-r--r--   0        0        0      454 2024-04-03 07:25:18.463079 tuxtrigger-0.8.1/tuxtrigger/exceptions.py
+-rw-r--r--   0        0        0     4707 2024-04-03 07:25:18.463079 tuxtrigger-0.8.1/tuxtrigger/inputvalidation.py
+-rw-r--r--   0        0        0     1169 2024-04-03 07:25:18.463079 tuxtrigger-0.8.1/tuxtrigger/manifest.py
+-rw-r--r--   0        0        0     7970 2024-04-03 07:25:18.463079 tuxtrigger-0.8.1/tuxtrigger/repository.py
+-rw-r--r--   0        0        0      938 2024-04-03 07:25:18.464079 tuxtrigger-0.8.1/tuxtrigger/request.py
+-rw-r--r--   0        0        0     1933 2024-04-03 07:25:18.464079 tuxtrigger-0.8.1/tuxtrigger/storage.py
+-rw-r--r--   0        0        0     9041 2024-04-03 07:25:18.464079 tuxtrigger-0.8.1/tuxtrigger/tuxintegration.py
+-rw-r--r--   0        0        0     2388 2024-04-03 07:25:18.464079 tuxtrigger-0.8.1/tuxtrigger/utils.py
+-rw-r--r--   0        0        0      260 2024-04-03 07:25:18.464079 tuxtrigger-0.8.1/tuxtrigger/yamlload.py
+-rw-r--r--   0        0        0     2625 1970-01-01 00:00:00.000000 tuxtrigger-0.8.1/PKG-INFO
```

### Comparing `tuxtrigger-0.7.0/.gitlab-ci.yml` & `tuxtrigger-0.8.1/.gitlab-ci.yml`

 * *Files 22% similar despite different names*

```diff
@@ -1,19 +1,37 @@
+image: python:3.10
+
 include: 
   - https://gitlab.com/Linaro/tuxpkg/-/raw/main/gitlab-ci-pipeline.yml
 
 variables:
   TUXPKG_PROJECT: tuxtrigger
   TUXSUITE_TOKEN: $TUXSUITE_TOKEN
+  SKIP_BUILD_DEB: 1
+  SKIP_BUILD_RPM: 1
 
 .job:
   image: $CI_REGISTRY_IMAGE:ci-debian
+  before_script:
+  - python3 -m pip install --upgrade isort --break-system-packages
   script:
   - make $CI_JOB_NAME
 
+test:
+  extends: .job
+  stage: test
+  coverage: '/(?i)total.*? (100(?:\.0+)?\%|[1-9]?\d(?:\.\d+)?\%)$/'
+  before_script:
+  - python3 -m pip install --upgrade -r requirements-dev.txt --break-system-packages
+  artifacts:
+    reports:
+      coverage_report:
+        coverage_format: cobertura
+        path: coverage.xml
+
 stylecheck:
   extends: .job
   stage: test
 
 typecheck: 
   extends: .job
   stage: test
@@ -42,27 +60,22 @@
 doc:
   extends: .job
   stage: build
   artifacts:
     paths:
       - public
   before_script:
-    - apt install -y python3-venv
-    - python3 -m venv .venv
-    - source .venv/bin/activate
-    - pip install mkdocs-material
-
-    - pip3 install pymdown-extensions
+    - python3 -m pip install mkdocs-material --break-system-packages
   
 pages:
   extends: .job
   stage: deploy
   needs:
     - doc
-    - repository
   artifacts:
     paths:
       - public
   only:
     - tags
   script:
     - cp -r dist/repo public/packages/
+
```

### Comparing `tuxtrigger-0.7.0/Dockerfile.ci-debian` & `tuxtrigger-0.8.1/Dockerfile.ci-debian`

 * *Files 2% similar despite different names*

```diff
@@ -11,14 +11,15 @@
         codespell \
         flake8 \
         flit \
         git \
         make \
         mkdocs \
         mypy \
+	isort \
         ${EXTRA_PACKAGES} \
     && true
 
 RUN if grep '^Source: tuxpkg' /tuxpkg/debian/control; then exit; fi; \
     /usr/lib/apt/apt-helper download-file https://linaro.gitlab.io/tuxpkg/packages/signing-key.gpg /etc/apt/trusted.gpg.d/tuxpkg.gpg \
     && echo 'deb https://linaro.gitlab.io/tuxpkg/packages/ ./' > /etc/apt/sources.list.d/tuxpkg.list \
     && apt-get update \
```

### Comparing `tuxtrigger-0.7.0/LICENSE` & `tuxtrigger-0.8.1/LICENSE`

 * *Files identical despite different names*

### Comparing `tuxtrigger-0.7.0/README.md` & `tuxtrigger-0.8.1/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -46,11 +46,11 @@
 4. [Create configuration.yaml file](docs/run.md#create-configuration-file)
 5. Provide [plan.yaml](https://docs.tuxsuite.com/plan/) file(s) from [TuxSuite](https://tuxsuite.com)
 6. Run TuxTrigger
 
 Call tuxtrigger:
 
 ```shell
-tuxtrigger /path/to/config.yaml
+tuxtrigger /path/to/config.yaml --plan /path/to/plan_directory
 ```
 
 Tuxtrigger will automatically start.
```

### Comparing `tuxtrigger-0.7.0/debian/control` & `tuxtrigger-0.8.1/debian/control`

 * *Files 1% similar despite different names*

```diff
@@ -16,16 +16,16 @@
                python3-pip,
                python3-yaml,
 Standards-Version: 4.6.0.1
 Homepage: https://tuxsuite.org/
 
 Package: tuxtrigger
 Architecture: all
-Depends: python3 (>= 3.6),
+Depends: python3 (>= 3.10),
          python3-requests,
          python3-jinja2,
          python3-yaml,
          ${python3:Depends},
          ${misc:Depends}, 
 Description: TuxTrigger
  TuxTrigger allows to automatically track a set of git repositories and branches.
- When a change occurs, TuxTrigger will build, test and track the results using Tuxsuite and SQUAD.
+ When a change occurs, TuxTrigger will build, test and track the results using Tuxsuite and SQUAD.
```

### Comparing `tuxtrigger-0.7.0/docs/install-deb.md` & `tuxtrigger-0.8.1/docs/install-deb.md`

 * *Files identical despite different names*

### Comparing `tuxtrigger-0.7.0/docs/install-rpm.md` & `tuxtrigger-0.8.1/docs/install-rpm.md`

 * *Files identical despite different names*

### Comparing `tuxtrigger-0.7.0/docs/run-uninstalled.md` & `tuxtrigger-0.8.1/docs/run-uninstalled.md`

 * *Files identical despite different names*

### Comparing `tuxtrigger-0.7.0/docs/run.md` & `tuxtrigger-0.8.1/docs/run.md`

 * *Files 16% similar despite different names*

```diff
@@ -24,33 +24,61 @@
 
 Tuxtrigger enables dynamically generated branch list in config file:
 
 - 'regex' - match branch names in selected repository
 - 'default_plan' - plan to be assigned for matched branches
 - 'squad_project_prefix' - prefix added to 'squad_project' value in matched branches
 - 'default_squad_project' - Use this squad_project value in matched branches
+- 'default_lava_test_plans_project' - Use to set value in matched branches
+- 'default_lab' - Use to set lab for all matched branches
 - 'lava_test_plans_project' - Use to say what project in lava-test-plans to use
 - 'lab' - Use to say what LAVA lab to submit jobs to
- 
+
 ```yaml
 repositories:
 - url: https://git.kernel.org/pub/scm/linux/kernel/git/arm64/linux.git
   squad_group: ~pawel.szymaszek
-  regex: for-next/* 
+  regex: for-next/*
   default_plan: stable.yaml
   squad_project_prefix: generator
-  lava_test_plans_project: lkft
-  lab: https://lkft.validation.linaro.org
+  default_lava_test_plans_project: lkft
+  default_lab: https://lkft.validation.linaro.org
   branches:
   - name: for-next/acpi # hardcoded values won't be overwritten
     squad_project: generator-linux-for-next-acpi
     plan: stable_next.yaml
 ```
 
-To check results of dynamically generated config use "--generate-config" argument. 
+Tuxtrigger enables SQAUD project configuration. By setting values in config file you are able to 
+create or update squad project.
+- in ```config``` section you are able to specify one or more options from listed below
+
+```yaml
+config:
+  plugins: linux_log_parser,ltp
+  wait_before_notification_timeout: 600
+  notification_timeout: 28800
+  force_finishing_builds_on_timeout: False
+  important_metadata_keys: build-url,git_ref,git_describe,git_repo,kernel_version
+  thresholds: build/*-warnings
+  data_retention: 0
+repositories:
+- url: https://git.kernel.org/pub/scm/linux/kernel/git/arm64/linux.git
+  squad_group: ~pawel.szymaszek
+  regex: for-next/*
+  default_plan: stable.yaml
+  squad_project_prefix: generator
+  default_lava_test_plans_project: lkft
+  default_lab: https://lkft.validation.linaro.org
+  branches:
+  - name: for-next/acpi # hardcoded values won't be overwritten
+    squad_project: generator-linux-for-next-acpi
+    plan: stable_next.yaml
+```
+To check results of dynamically generated config use "--generate-config" argument.
 Tuxtrigger will perform 'dry-run' and prompt generated config.
 
 ```shell
 tuxtrigger /path/to/config.yaml --generate-config
 ```
 
 ## Create Plan for TuxSuite
@@ -67,15 +95,22 @@
 description: stable_plan
 jobs:
 - tests:
     - {device: qemu-x86_64, tests: [ltp-smoke]}
 ```
 For further information about plans and TuxSuite configuration please Visit: [TuxSuite Home](https://docs.tuxsuite.com/)
 
+!!! note "Usage"
+    By default TuxTrigger takes plans from `share/plans` folder Custom path can be set by argument --plan `<path>`
+    ```shell
+    tuxtrigger path/to/config.yaml --plan=path/to/plan/folder
+
+    ```
+
 ## Running TuxTrigger
 
 To run tuxtrigger with the default configuration file:
 ```shell
-tuxtrigger /path/to/config.yaml
+tuxtrigger /path/to/config.yaml --plan /path/to/plan_directory
 ```
```

### Comparing `tuxtrigger-0.7.0/docs/subcommands.md` & `tuxtrigger-0.8.1/docs/subcommands.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,13 +1,23 @@
 # TuxTrigger Subcommands
 
 ## Run mode yaml/squad
 
 TuxTrigger checks out repositories by comparing fingerprint from git.kernel.org manifest file and/or git sha value.
 
+## From version 0.8.0
+
+Tuxtrigger is storing fingerprint and/or git sha values ONLY in output yaml file.
+
+!!! note
+	- ```sha-compare``` subcommand is no longer available
+
+
+## Version up to 0.7.0
+
 There are two options where those values are stored in order to compare.
 
 1. SQUAD - recommended sha-compare argument is set by default to squad, fingerprint and git sha are stored in squad_project metadata
 
 ```shell
 tuxtrigger path/to/config.yaml --sha-compare=squad
 ```
@@ -15,15 +25,14 @@
 2. YAML fingerprint and git-sha values are stored in .yaml file created by tuxtrigger in share folder
 
 ```shell
 tuxtrigger path/to/config.yaml --sha-compare=yaml
 ```
 
 
-
 ## Output File
 
 TuxTrigger is storing the state of each repositories in yaml file.
 To declare a custom output file path type:
 
 ```shell
 tuxtrigger path/to/config.yaml --output path/to/output.yaml
@@ -43,28 +52,39 @@
 ## Pre submit script
 
 When tracked repository has changed tuxtrigger can invoke your custom script. 
 By passing ```--pre-submit``` argument you are able to define the path to script, which receives three values from tuxtrigger
 
 1. repository url
 2. branch name
-3. new SHA value
+3. SHA value
 
 ```shell 
 tuxtrigger path/to/config.yaml --pre-submit path/to/script.sh
 ```
 ## Disabling Tuxplan submit
 
-Tuxtrigger can be used without sending a plan file to tuxsuite, by adding an argument ```--plan-disabled```
+Tuxtrigger can be used without sending a plan file to tuxsuite, by adding an argument ```--disable-plan```
 With that option tuxtrigger will check repositories for changes and can invoke the script if repo has changed.
-After script execution tuxtrigger will submit new sha/fingerprint data to squad project.
+After script execution tuxtrigger will save new sha/fingerprint data to output file.
 (even when tuxplan option is disabled tuxtrigger will still invoke tuxsuite build for receiving ‘git_describe’ value).
 
 ```shell 
-tuxtrigger path/to/config.yaml --plan-disabled
+tuxtrigger path/to/config.yaml --disable-plan
+```
+
+## Disabling SQUAD submit
+
+Tuxtrigger can be used without sending/using SQUAD ```--disable-squad```
+With that option tuxtrigger will check repositories for changes and invoke tuxbuild and tuxplan when repo has changed. 
+It can also invoke the script when this command is specified.
+After script execution tuxtrigger will save new sha/fingerprint data to output file.
+
+```shell 
+tuxtrigger path/to/config.yaml --disable-squad
 ```
 
 ## Generate config
 
 Argument ```--generate-config``` invoke tuxtrigger dry-run to prompt the result of generating configuration from config.yaml file. (also, you can check if regex value set in config file matches any branches from tracked repository)
 
 ```shell 
@@ -86,26 +106,41 @@
 ```shell
 tuxtrigger path/to/config.yaml --log-file path/to/log-file.txt
 ```
 
 ## Change Log Level
 
 By default TuxTrigger log level is set to: info
-You can adjust log level by choosing one of the levels (debug, info, warn, error)
+You can adjust log level by choosing one of the levels (DEBUG, INFO, WARN, ERROR)
 
 ```shell
-tuxtrigger path/to/config.yaml --log-level=warn
+tuxtrigger path/to/config.yaml --log-level=WARN
 ```
 
-## TuxSuite Plan Folder
+## TuxSuite Plan Dir
 
 All the plans should be in one directory:
 
 ```shell
-tuxtrigger path/to/config.yaml --plan path/to/plan-folder
+tuxtrigger path/to/config.yaml --plan path/to/plan_directory
+```
+
+## Callback url
+
+It is possible to set callback-url inside tuxtrigger with ```--callback-url``` command
+
+```shell
+tuxtrigger path/to/config.yaml --callback-url https://url
+```
+
+## Callback headers
+
+To specify headers passed to callback-url you can set ```--callback-headers``` subcommand formatted as 'header':'value' pairs
+```shell
+tuxtrigger path/to/config.yaml --callback-headers XYZ
 ```
 
 ## Current version
 
 ```shell
 tuxtrigger -v
 ```
```

### Comparing `tuxtrigger-0.7.0/mkdocs.yml` & `tuxtrigger-0.8.1/mkdocs.yml`

 * *Files 23% similar despite different names*

```diff
@@ -4,18 +4,21 @@
 site_dir: public
 site_description: |
   TuxTrigger, by Linaro, is a command line tool.  TuxTrigger is a part of TuxSuite, a suite of tools and
   services to help with Linux kernel development.
 repo_url: https://gitlab.com/Linaro/TuxTrigger/
 
 theme:
-  name: material
+  name: 'material'
   logo: tuxtrigger.svg
   favicon: tuxtrigger.svg
   font: false
+  features:
+    - content.code.copy
+    - navigation.footer
 
 markdown_extensions:
 - admonition
 - pymdownx.highlight
 - pymdownx.superfences
 - pymdownx.tabbed
 - toc:
```

### Comparing `tuxtrigger-0.7.0/test/test_argparser.py` & `tuxtrigger-0.8.1/test/test_argparser.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 #
 # Copyright 2022-present Linaro Limited
 #
 # SPDX-License-Identifier: MIT
 
 import subprocess
+from pathlib import Path
 
 from tuxtrigger import __version__
-from pathlib import Path
 
 BASE = (Path(__file__) / "../..").resolve()
 
 
 def test_setup_parser():
     version_result = subprocess.run(
         ["sh", f"{BASE}/run", "-v"], stdout=subprocess.PIPE, text=True
     )
     help_result = subprocess.run(
         ["sh", f"{BASE}/run", "--help"], stdout=subprocess.PIPE, text=True
     )
     assert f"TuxTrigger, {__version__}" in version_result.stdout
     assert (
-        "usage: TuxTrigger [-h] [--sha-compare {squad,yaml}] [--output OUTPUT]"
+        "usage: TuxTrigger [-h] [--output OUTPUT] [--pre-submit PRE_SUBMIT]"
         in help_result.stdout
     )
```

### Comparing `tuxtrigger-0.7.0/test/test_builder.py` & `tuxtrigger-0.8.1/test/test_tuxintegration.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,29 +1,26 @@
 #
 # Copyright 2022-present Linaro Limited
 #
 # SPDX-License-Identifier: MIT
 
-
 import json
-from requests import Session
+from pathlib import Path
+from test.test_configparser import MockedStdout
 from unittest import mock
 
 import pytest
 
-from pathlib import Path
-from tuxtrigger.builder import (
-    compare_squad_sha,
-    squad_metadata_request,
-    tux_console_build,
-    tux_console_plan,
-    build_result,
-    update_squad_metadata,
+from tuxtrigger.exceptions import TuxsuiteException, TuxtriggerException
+from tuxtrigger.repository import Branch, Repository
+from tuxtrigger.tuxintegration import (
+    TuxSuiteIntegration,
+    tux_plan_submitter,
+    tuxsuite_trigger,
 )
-from tuxtrigger.exceptions import SquadException, TuxtriggerException, TuxsuiteException
 
 BASE = (Path(__file__) / "..").resolve()
 
 PLAN = BASE / "test_files/planTest.yaml"
 PLAN_FAIL = BASE / "test_files/planTestc.yaml"
 JSON_PLAN_RESULT = BASE / "test_files/plan_result.json"
 JSON_OUT = BASE / "test_files/"
@@ -53,189 +50,220 @@
     "git_repo": "https://gitlab.com/no_real_repo",
     "git_ref": "master",
     "git_describe": "test-rc",
 }
 
 JSON_RESPONSE = """{
 "count":1,
+"version": "example_branch_with_additional_values",
 "git_sha":"1234",
 "tux_fingerprint":"8fa23329efa65477f077d99e145e4087190a55cc",
 "results":[
 {
 "metadata":"https://www.example_metadata.pl",
 "id":1234
 }
 ]
 }"""
 
 
-class MockedStdout:
-    def __init__(self, returncode, stdout, stderr=None) -> None:
-        self.returncode = returncode
-        self.stdout = stdout
-        self.stderr = stderr
-
-
-class MockedSession:
-    def __init__(self, status_code, content, ok=True) -> None:
-        self.status_code = status_code
-        self.content = content
-        self.ok = ok
-
-
-@mock.patch("tuxtrigger.builder.subprocess.run")
+@mock.patch("tuxtrigger.tuxintegration.subprocess.run")
 @mock.patch("tempfile.NamedTemporaryFile")
-def test_tux_console_build(mock_temp_file, mock_run):
+def test_tux__build_call(mock_temp_file, mock_run, tux_config, squad_group_good):
+    test_repo = Repository("not_existing_url", squad_group_good)
+    test_branch = Branch(
+        test_repo, "master", "stable_plan", "example_project", None, None, None
+    )
+    test_tux = TuxSuiteIntegration(True, test_branch, tux_config)
     build = MockedStdout(returncode=0, stdout=JSON_DATA)
     mock_run.return_value = build
     with open(BASE / "test_files/test.json", "r") as temp_file:
         mock_temp_file.return_value.__enter__.return_value = temp_file
-        result = tux_console_build(**PARAMS)
-    assert result == JSON_DATA["uid"]
+        result = test_tux.tux_build_call(**PARAMS)
+    assert result.uid == JSON_DATA["uid"]
 
     build_error = MockedStdout(returncode=1, stdout="", stderr="Tuxsuite Failure")
     mock_run.return_value = build_error
     with pytest.raises(TuxsuiteException) as exc:
-        tux_console_build(**PARAMS)
+        test_tux.tux_build_call(**PARAMS)
     assert "Tuxsuite not build repo" in str(exc)
 
 
 @mock.patch(
-    "tuxtrigger.builder.subprocess.run",
+    "tuxtrigger.tuxintegration.subprocess.run",
     side_effect=TuxsuiteException("*** Tuxsuite not build repo"),
 )
-def test_tux_console_build_error(mock_run):
+def test_tux_build_call_error(mock_run, squad_group_good, tux_config):
+    test_repo = Repository("not_existing_url", squad_group_good)
+    test_branch = Branch(
+        test_repo, "master", "stable_plan", "example_project", None, None, None
+    )
+    test_tux = TuxSuiteIntegration(True, test_branch, tux_config)
     build = MockedStdout(returncode=1, stdout=None)
     mock_run.return_value = build
     with pytest.raises(TuxsuiteException) as ex:
-        tux_console_build(**PARAMS)
+        test_tux.tux_build_call(**PARAMS)
     assert "Tuxsuite not build" in str(ex.value)
 
 
-@mock.patch("tuxtrigger.builder.subprocess.run")
-def test_tux_console_plan_error(
-    mock_run,
-    squad_group_good,
-    squad_project_good,
-    lab_good,
-    lava_test_plans_project_good,
+@mock.patch("tuxtrigger.tuxintegration.subprocess.run")
+@mock.patch("tempfile.NamedTemporaryFile")
+def test_tux_plan_call(
+    mock_temp_file, mock_run, squad_group_good, tux_config, tmp_path
 ):
-    build = MockedStdout(returncode=1, stdout=JSON_DATA)
-    mock_run.return_value = build
+    test_repo = Repository("not_existing_url", squad_group_good)
+    test_branch = Branch(
+        test_repo, "master", "stable_plan", "example_project", None, None, None
+    )
+    test_tux = TuxSuiteIntegration(True, test_branch, tux_config)
+
+    build_err = MockedStdout(returncode=1, stdout=JSON_DATA)
+    mock_run.return_value = build_err
     with pytest.raises(TuxtriggerException) as exc_tuxtrigger:
-        tux_console_plan(
+        test_tux.tux_plan_call(
             None,
-            PLAN,
-            squad_group_good,
-            squad_project_good,
-            JSON_OUT,
-            FINGERPRINT,
-            lab_good,
-            lava_test_plans_project_good,
         )
 
     assert "*** Not able to submit plan" in str(exc_tuxtrigger)
     with pytest.raises(TuxsuiteException) as exc_tuxsuite:
-        tux_console_plan(
+        test_tux.tux_plan_call(
             JSON_DATA,
-            PLAN,
-            squad_group_good,
-            squad_project_good,
-            JSON_OUT,
-            FINGERPRINT,
-            lab_good,
-            lava_test_plans_project_good,
         )
-    assert "Submiting Plan for example_project_test-rc failed" in str(exc_tuxsuite)
-
+    assert "Submitting Plan for master_test-rc failed" in str(exc_tuxsuite)
 
-@mock.patch("tuxtrigger.builder.subprocess.run")
-@mock.patch("tempfile.NamedTemporaryFile")
-def test_tux_console_plan(
-    mock_temp_file,
-    mock_run,
-    squad_group_good,
-    squad_project_good,
-    lab_good,
-    lava_test_plans_project_good,
-):
     build = MockedStdout(returncode=0, stdout=JSON_DATA)
     mock_run.return_value = build
-    with open(BASE / "test_files/test.json", "r") as test_file:
-        mock_temp_file.return_value.__enter__.return_value = test_file
-        tux_console_plan(
-            JSON_DATA,
-            PLAN_FAIL,
-            squad_group_good,
-            squad_project_good,
-            JSON_OUT,
-            FINGERPRINT,
-            lab_good,
-            lava_test_plans_project_good,
-        )
+    test_tux.tux_plan_call(JSON_DATA)
+    mock_run.assert_called_with(
+        [
+            "tuxsuite",
+            "plan",
+            "--git-repo",
+            "https://gitlab.com/no_real_repo",
+            "--git-ref",
+            "master",
+            "--name",
+            "test-rc",
+            "--no-wait",
+            BASE / "stable_plan",
+            "--json-out",
+            mock_temp_file().__enter__().name,
+            "--callback",
+            "https://dummy-qa-reports.org/api/fetchjob/~non.existing/example_project/test-rc/env/tuxsuite.com",
+            "--parameters",
+            "SQUAD_URL=https://dummy-qa-reports.org/api/submit/~non.existing/example_project/test-rc/env/",
+        ]
+    )
 
+    test_tux.branch_object.lab = "test_lab"
+    test_tux.branch_object.lava_test_plans_project = "test_lava_project"
+    test_tux.tux_plan_call(JSON_DATA)
+    mock_run.assert_called_with(
+        [
+            "tuxsuite",
+            "plan",
+            "--git-repo",
+            "https://gitlab.com/no_real_repo",
+            "--git-ref",
+            "master",
+            "--name",
+            "test-rc",
+            "--no-wait",
+            BASE / "stable_plan",
+            "--json-out",
+            mock_temp_file().__enter__().name,
+            "--callback",
+            "https://dummy-qa-reports.org/api/fetchjob/~non.existing/example_project/test-rc/env/tuxsuite.com",
+            "--parameters",
+            "SQUAD_URL=https://dummy-qa-reports.org/api/submit/~non.existing/example_project/test-rc/env/",
+            "--lab",
+            "test_lab",
+            "--lava-test-plans-project",
+            "test_lava_project",
+        ]
+    )
 
-@mock.patch("tuxtrigger.builder.subprocess.run")
-def test_build_result(mock_run):
+
+@mock.patch("tuxtrigger.tuxintegration.subprocess.run")
+def test_build_result(mock_run, tux_config, squad_group_good):
+    test_repo = Repository("not_existing_url", squad_group_good)
+    test_branch = Branch(
+        test_repo, "master", "stable_plan", "example_project", None, None, None
+    )
+    test_tux = TuxSuiteIntegration(True, test_branch, tux_config)
+    test_tux.uid = UID
     build = MockedStdout(returncode=0, stdout=json.dumps(JSON_BUILD_DATA))
     mock_run.return_value = build
-    json_output = build_result(UID)
+    json_output = test_tux.build_result()
     mock_run.assert_called_once_with(
-        ["tuxsuite", "build", "get", UID, "--json"], stdout=-1, stderr=-1, text=True
+        ["tuxsuite", "build", "get", test_tux.uid, "--json"],
+        stdout=-1,
+        stderr=-1,
+        text=True,
     )
-    assert build_result(None) is None
-    assert JSON_BUILD_DATA == json_output
-
-
-@mock.patch("tuxtrigger.builder.subprocess.run")
-def test_build_result_error(mock_run):
     build = MockedStdout(returncode=1, stdout="Oops!")
     mock_run.return_value = build
     with pytest.raises(TuxsuiteException) as exc:
-        build_result(UID)
+        test_tux.build_result()
     assert "*** Build result for UID:2CCI3BkwKdqM4wOOwB5xRRxvOha failed" in str(exc)
 
-
-def test_update_squad_metadata_error(squad_project_good):
-    with pytest.raises(TuxtriggerException) as exc:
-        update_squad_metadata(JSON_DATA, None, squad_project_good, FINGERPRINT)
-    assert "SQUAD config is not available!" in str(exc)
+    test_tux.uid = None
+    assert test_tux.build_result() is None
+    assert JSON_BUILD_DATA == json_output
 
 
-@mock.patch.object(Session, "post")
-def test_update_squad_metadata(mock_session, squad_group_good, squad_project_good):
-    session_ok = MockedSession(status_code=200, content=JSON_RESPONSE, ok=True)
-    mock_session.return_value = session_ok
-    update_result = update_squad_metadata(
-        JSON_DATA, squad_group_good, squad_project_good, FINGERPRINT
+@mock.patch("tuxtrigger.tuxintegration.pre_tux_run")
+@mock.patch("tuxtrigger.tuxintegration.Branch.check_squad_project")
+@mock.patch("tuxtrigger.tuxintegration.Branch.configure_squad_client")
+@mock.patch("tuxtrigger.tuxintegration.TuxSuiteIntegration.tux_build_call")
+@mock.patch("tuxtrigger.tuxintegration.Branch.compare_sha")
+def test_tuxsuite_trigger(
+    mock_change,
+    mock_tux_build,
+    mock_squad_config,
+    mock_squad_project,
+    mock_custom_script,
+    squad_group_good,
+    tux_config,
+):
+    test_repo = Repository("not_existing_url", squad_group_good)
+    test_branch = Branch(
+        test_repo, "master", "stable_plan", "example_project", None, None, None
     )
-    assert update_result == 0
-
-
-@mock.patch.object(Session, "get")
-def test_squad_sha_request(mock_session):
-    session_ok = MockedSession(status_code=200, content=JSON_RESPONSE)
-    mock_session.return_value = session_ok
-    squad_sha = squad_metadata_request("1111", "tuxtrigger")
-    assert squad_sha == ("8fa23329efa65477f077d99e145e4087190a55cc", "1234")
-
+    test_branch.input_dict = {}
 
-@mock.patch.object(Session, "get")
-def test_squad_sha_request_fail(mock_session):
-    session_fail = MockedSession(status_code=404, content=(None, None))
-    mock_session.return_value = session_fail
-    with pytest.raises(SquadException) as exc:
-        squad_metadata_request("1112", "tuxtrigger")
-    assert "SQUAD response error - (get latest build) 404" in str(exc)
-
-    assert squad_metadata_request(None, None) == (None, None)
-
-
-@mock.patch("tuxtrigger.builder.squad_metadata_request")
-def test_compare_squad_sha(mock_sha):
-    mock_sha.return_value = ("1234", "1234")
-    assert compare_squad_sha("1111", "tuxtrigger", "1234") is False
-    assert compare_squad_sha("1112", "tuxtrigger", "5678") is True
+    mock_change.return_value = True
+    tux_config.pre_submit_path = BASE
+    tuxsuite_trigger(tux_config, test_branch)
+    mock_squad_config.assert_called()
+    mock_squad_project.assert_called()
+    mock_tux_build.assert_called()
+    mock_custom_script.assert_called()
+
+    tux_config.submit_mode = "always"
+    tuxsuite_trigger(tux_config, test_branch)
+    mock_tux_build.assert_called()
+    tux_config.submit_mode = "never"
+    result = tuxsuite_trigger(tux_config, test_branch)
+    assert result is None
+
+
+@mock.patch("tuxtrigger.tuxintegration.TuxSuiteIntegration.build_result")
+@mock.patch("tuxtrigger.tuxintegration.TuxSuiteIntegration.tux_plan_call")
+def test_tux_plan_submitter(mock_plan, mock_build, tux_config, squad_group_good):
+    test_repo = Repository("not_existing_url", squad_group_good)
+    test_branch = Branch(
+        test_repo, "master", "stable_plan", "example_project", None, None, None
+    )
+    test_tux = TuxSuiteIntegration(True, test_branch, tux_config)
+    test_tux.uid = UID
 
+    assert tux_plan_submitter(tux_config, None) is None
 
-def test_compare_squad_sha_none():
-    assert compare_squad_sha(None, None, "1234") is True
+    mock_build.return_value = JSON_BUILD_DATA
+    tux_plan_submitter(tux_config, [test_tux])
+    mock_plan.assert_called()
+
+    tux_config.disable_squad = True
+    tux_plan_submitter(tux_config, [test_tux])
+    assert tux_config.json_out == Path(".")
+    assert test_tux.branch_object.repository.squad_group is None
```

### Comparing `tuxtrigger-0.7.0/test/test_exceptions.py` & `tuxtrigger-0.8.1/test/test_exceptions.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -2,16 +2,16 @@
 # Copyright 2022-present Linaro Limited
 #
 # SPDX-License-Identifier: MIT
 
 from tuxtrigger.exceptions import (
     InvalidArgument,
     SquadException,
-    TuxtriggerException,
     TuxsuiteException,
+    TuxtriggerException,
 )
 
 
 def test_tux_trig_exception():
     exc = TuxtriggerException("test message")
     assert isinstance(exc, Exception) is True
     assert exc.__str__() == "test message"
```

### Comparing `tuxtrigger-0.7.0/test/test_files/happy_path.yaml` & `tuxtrigger-0.8.1/test/test_files/happy_path.yaml`

 * *Files 21% similar despite different names*

```diff
@@ -1,32 +1,37 @@
+squad_config:
+  plugins: linux_log_parser
+  force_finishing_builds_on_timeout: True
+  important_metadata_keys: kernel_version,git_ref
+  data_retention: 2137
 repositories:
 - url: https://git.kernel.org/pub/scm/linux/kernel/git/tomba/linux.git
   squad_group: ~non.existing
   branches:
     - name: master
       squad_project: example_project
       plan: stable.yaml
-      lab: https://lkft.validation.linaro.org
-      lava_test_plans_project: lkft
+      lab: default
+      lava_test_plans_project: https://lkft.validation.linaro.org
     - name: for-laurent
       squad_project: example_project
       plan: stable-next.yaml
-      lab: https://lkft.validation.linaro.org
-      lava_test_plans_project: lkft
+      lab: default
+      lava_test_plans_project: https://lkft.validation.linaro.org
 - url: https://git.kernel.org/pub/scm/linux/kernel/git/torvalds/linux.git
   squad_group: ~non.existing
   regex: for-next/*
   default_plan: default_plan
   squad_project_prefix: testing
-  lab: https://lkft.validation.linaro.org
-  lava_test_plans_project: lkft
+  default_lab: default
+  default_lava_test_plans_project: https://lkft.validation.linaro.org
   branches:
     - name: master
       squad_project: example_project
       plan: stable.yaml
-      lab: https://lkft.validation.linaro.org
-      lava_test_plans_project: lkft
+      lab: default
+      lava_test_plans_project: https://lkft.validation.linaro.org
     - name: v5.19
       squad_project: example_project
       plan: stable-next.yaml
-      lab: https://lkft.validation.linaro.org
-      lava_test_plans_project: lkft
+      lab: default
+      lava_test_plans_project: https://lkft.validation.linaro.org
```

### Comparing `tuxtrigger-0.7.0/test/test_files/manifest.js.gz` & `tuxtrigger-0.8.1/test/test_files/manifest.js.gz`

 * *Files identical despite different names*

### Comparing `tuxtrigger-0.7.0/test/test_manifest.py` & `tuxtrigger-0.8.1/test/test_manifest.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,29 +1,26 @@
 #
 # Copyright 2022-present Linaro Limited
 #
 # SPDX-License-Identifier: MIT
 
+import json
 from pathlib import Path
 from unittest import mock
+
 import pytest
-import json
 
 from tuxtrigger.exceptions import TuxtriggerException
-from tuxtrigger.manifest import (
-    git_manifest_download,
-    git_repository_fingerprint,
-    manifest_changed,
-)
+from tuxtrigger.manifest import git_manifest_download, git_repository_fingerprint
 
 BASE = (Path(__file__) / "..").resolve()
 
 FINGERPRINT = "c8f105f060651674a38b2103190f2ca52381ce76"
 
-REPO_URL = "https://git.kernel.org/pub/scm/linux/kernel/git/torvalds/linux.git"
+REPO_URL = "https://git.kernel.org/pub/dummy/repo.git"
 MANIFEST_REPO = "/pub/scm/linux/kernel/git/wwguy/iwlwifi.git"
 
 
 class RequestMock:
     def __init__(self, status_code, content):
         self.status_code = status_code
         self.content = content
@@ -54,26 +51,7 @@
         mock_manifest.return_value = manifest
         output = git_manifest_download()
     test_fingerprint = git_repository_fingerprint(output, MANIFEST_REPO)
     assert test_fingerprint == FINGERPRINT
     with pytest.raises(KeyError) as exc:
         git_repository_fingerprint(output, "REPO_URL")
     assert "Tracked Repository does not exist in manifest" in str(exc)
-
-
-def test_manifest_changed_true(correct_archive_read):
-    assert manifest_changed(REPO_URL, FINGERPRINT, correct_archive_read) is True
-
-
-def test_manifest_changed_false(
-    wrong_archive_read, correct_archive_read, correct_archive_read_no_fingerprint
-):
-    assert manifest_changed(REPO_URL, FINGERPRINT, wrong_archive_read) is False
-
-    with pytest.raises(KeyError):
-        manifest_changed("", FINGERPRINT, correct_archive_read)
-        manifest_changed(REPO_URL, "", correct_archive_read)
-    assert (
-        manifest_changed(REPO_URL, FINGERPRINT, correct_archive_read_no_fingerprint)
-        is False
-    )
-    assert manifest_changed(REPO_URL, FINGERPRINT, FINGERPRINT) is False
```

### Comparing `tuxtrigger-0.7.0/test/test_request.py` & `tuxtrigger-0.8.1/test/test_request.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,26 +1,30 @@
-#
 # Copyright 2022-present Linaro Limited
 #
 # SPDX-License-Identifier: MIT
 
 
-from http.client import HTTPMessage
 import json
 import os
+
+# from http.client import HTTPMessage
 from unittest import mock
-from unittest.mock import Mock, ANY, call
+
 from tuxtrigger import request
 
+# from unittest.mock import ANY, Mock, call
+
 
 class MockedRequest:
     def __init__(self, status_code):
         self.status_code = status_code
 
 
+"""
+temporary disabled function - throwing an error on local repo
 @mock.patch("urllib3.connectionpool.HTTPConnectionPool._get_conn")
 def test_get_session(connection_mock):
     connection_mock.return_value.getresponse.side_effect = [
         Mock(status=500, msg=HTTPMessage()),
         Mock(status=429, msg=HTTPMessage()),
         Mock(status=200, msg=HTTPMessage()),
     ]
@@ -28,14 +32,15 @@
     response = r.get(url="http://anyurl.pl/testme")
     response.raise_for_status()
     assert connection_mock.return_value.request.mock_calls == [
         call("GET", "/testme", body=None, headers=ANY),
         call("GET", "/testme", body=None, headers=ANY),
         call("GET", "/testme", body=None, headers=ANY),
     ]
+"""
 
 
 @mock.patch("tuxtrigger.request.requests_get")
 def test_requests_get(mock_session):
     mock_req = MockedRequest(status_code=200)
     mock_session.return_value = mock_req
     req = request.requests_get(url="https://example.pl/xyz")
```

### Comparing `tuxtrigger-0.7.0/tuxtrigger.spec` & `tuxtrigger-0.8.1/tuxtrigger.spec`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 Name:      tuxtrigger
-Version:   0.7.0
+Version:   0.8.1
 Release:   0%{?dist}
 Summary:   FIXME
 License:   MIT
 URL:       https://tuxsuite.org/
 Source0:   %{pypi_source}
 
 
@@ -62,8 +62,8 @@
 
 %doc README.md
 %license LICENSE
 
 %changelog
 
 * Tue Aug 30 2022 Pawel Szymaszek <pawel.szymaszek@linaro.org> - 0.0.1
-- Initial version of the package
+- Initial version of the package
```

### Comparing `tuxtrigger-0.7.0/tuxtrigger/argparser.py` & `tuxtrigger-0.8.1/tuxtrigger/argparser.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #
 # Copyright 2022-present Linaro Limited
 #
 # SPDX-License-Identifier: MIT
 import argparse
 from pathlib import Path
-from tuxtrigger import __version__
 
+from tuxtrigger import __version__
 
 OUTPUT_FILE = Path("share/gitsha.yaml")
 PLAN_PATH = Path("share/plans/")
 LOG_FILE = Path("log.txt")
 
 
 def setup_parser() -> argparse.ArgumentParser:
@@ -17,41 +17,27 @@
         prog="TuxTrigger",
         description="TuxTrigger command line tool for controlling changes in repositories",
     )
     parser.add_argument(
         "config", type=Path, help="config yaml file name", action="store"
     )
     parser.add_argument(
-        "--sha-compare",
-        type=str,
-        help="choose compare method",
-        default="squad",
-        choices=["squad", "yaml"],
-    )
-    parser.add_argument(
         "--output",
         type=Path,
         help="path for storing output file",
         action="store",
         default=OUTPUT_FILE,
     )
     parser.add_argument(
         "--pre-submit",
         type=Path,
         help="pre-tuxsuite script to run",
         action="store",
     )
     parser.add_argument(
-        "-v",
-        "--version",
-        help="prints current version",
-        action="version",
-        version=f"%(prog)s, {__version__}",
-    )
-    parser.add_argument(
         "--submit",
         "-s",
         type=str,
         help="trigger build on change",
         default="change",
         choices=["never", "change", "always"],
     )
@@ -66,31 +52,56 @@
         "--plan",
         type=Path,
         help="path to plan files",
         default=PLAN_PATH,
         action="store",
     )
     parser.add_argument(
+        "--callback-url",
+        type=str,
+        help="Callback URL to post event on a plan execution",
+        action="store",
+    )
+    parser.add_argument(
+        "--callback-headers",
+        type=str,
+        help="Headers to be passed to callback-url",
+        action="store",
+    )
+
+    parser.add_argument(
         "--log-level",
         "-l",
         type=str,
         help="set log level to more specific information",
         default="info",
-        choices=["debug", "info", "warn", "error"],
+        choices=["DEBUG", "INFO", "WARN", "ERROR"],
     )
     parser.add_argument(
         "--json-out",
         type=Path,
         help="json output folder path",
         action="store",
     )
     parser.add_argument(
-        "--plan-disabled",
-        help="disable submiting plan to tuxsuite",
-        action="store_false",
+        "--disable-plan",
+        help="disable submitting plan to tuxsuite",
+        action="store_true",
+    )
+    parser.add_argument(
+        "--disable-squad",
+        help="disable submitting data to squad",
+        action="store_true",
     )
     parser.add_argument(
         "--generate-config",
         help="dry-run to show generated config from regex value",
         action="store_true",
     )
+    parser.add_argument(
+        "-v",
+        "--version",
+        help="prints current version",
+        action="version",
+        version=f"%(prog)s, {__version__}",
+    )
     return parser
```

### Comparing `tuxtrigger-0.7.0/tuxtrigger/request.py` & `tuxtrigger-0.8.1/tuxtrigger/request.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,23 +1,21 @@
 #
 # Copyright 2022-present Linaro Limited
 #
 # SPDX-License-Identifier: MIT
 
 
+import requests
 from requests.adapters import HTTPAdapter
 from urllib3.util.retry import Retry
 
-import requests
-
-
 TIMEOUT = 60
 
 
-def get_session(retries):
+def _get_session(retries: int):
     session = requests.Session()
 
     retry_strategy = Retry(
         total=retries,
         status_forcelist=[408, 413, 429, 500, 502, 503, 504],
         allowed_methods=["HEAD", "GET", "OPTIONS", "DELETE", "PUT", "TRACE"],
         backoff_factor=1,
@@ -26,15 +24,15 @@
     adapter = HTTPAdapter(max_retries=retry_strategy)
     session.mount("http://", adapter)
     session.mount("https://", adapter)
 
     return session
 
 
-def requests_get(*args, **kwargs):
-    session = get_session(retries=10)
+def requests_get(*args, **kwargs) -> requests.Response:
+    session = _get_session(retries=10)
     return session.get(*args, timeout=TIMEOUT, **kwargs)
 
 
-def requests_post(*args, **kwargs):
-    session = get_session(retries=0)
+def requests_post(*args, **kwargs) -> requests.Response:
+    session = _get_session(retries=0)
     return session.post(*args, timeout=TIMEOUT, **kwargs)
```

### Comparing `tuxtrigger-0.7.0/PKG-INFO` & `tuxtrigger-0.8.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tuxtrigger
-Version: 0.7.0
+Version: 0.8.1
 Summary: TuxTrigger Project by Linaro
 Home-page: https://tuxsuite.com/
 Author: Pawel Szymaszek
 Author-email: pawel.szymaszek@linaro.org
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: MIT License
@@ -62,12 +62,12 @@
 4. [Create configuration.yaml file](docs/run.md#create-configuration-file)
 5. Provide [plan.yaml](https://docs.tuxsuite.com/plan/) file(s) from [TuxSuite](https://tuxsuite.com)
 6. Run TuxTrigger
 
 Call tuxtrigger:
 
 ```shell
-tuxtrigger /path/to/config.yaml
+tuxtrigger /path/to/config.yaml --plan /path/to/plan_directory
 ```
 
 Tuxtrigger will automatically start.
```

