# Comparing `tmp/sageworks-0.5.3.tar.gz` & `tmp/sageworks-0.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sageworks-0.5.3.tar", last modified: Mon Apr  1 17:30:52 2024, max compression
+gzip compressed data, was "sageworks-0.5.4.tar", last modified: Wed Apr  3 19:02:27 2024, max compression
```

## Comparing `sageworks-0.5.3.tar` & `sageworks-0.5.4.tar`

### file list

```diff
@@ -1,505 +1,512 @@
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-01 17:30:52.076910 sageworks-0.5.3/
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-01 17:30:52.001831 sageworks-0.5.3/.github/
--rw-r--r--   0 briford    (501) staff       (20)     1338 2024-03-28 17:23:43.000000 sageworks-0.5.3/.github/PULL_REQUEST_TEMPLATE.md
--rw-r--r--   0 briford    (501) staff       (20)      499 2023-12-24 17:18:24.000000 sageworks-0.5.3/.github/dependabot.yml
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-01 17:30:52.002375 sageworks-0.5.3/.github/workflows/
--rw-r--r--   0 briford    (501) staff       (20)      598 2024-01-10 18:45:51.000000 sageworks-0.5.3/.github/workflows/deploy-docs.yml
--rw-r--r--   0 briford    (501) staff       (20)      556 2024-01-23 15:36:53.000000 sageworks-0.5.3/.github/workflows/python-lint.yml
--rw-r--r--   0 briford    (501) staff       (20)     2008 2023-12-24 17:18:24.000000 sageworks-0.5.3/.gitignore
--rw-r--r--   0 briford    (501) staff       (20)      444 2024-03-28 17:23:43.000000 sageworks-0.5.3/CONTRIBUTING.md
--rw-r--r--   0 briford    (501) staff       (20)      102 2024-03-28 17:23:43.000000 sageworks-0.5.3/Dockerfile
--rw-r--r--   0 briford    (501) staff       (20)     1080 2024-03-28 17:23:43.000000 sageworks-0.5.3/LICENSE
--rw-r--r--   0 briford    (501) staff       (20)     1426 2023-12-24 17:18:24.000000 sageworks-0.5.3/Makefile
--rw-r--r--   0 briford    (501) staff       (20)     4118 2024-04-01 17:30:52.076835 sageworks-0.5.3/PKG-INFO
--rw-r--r--   0 briford    (501) staff       (20)     2695 2024-03-28 17:23:43.000000 sageworks-0.5.3/README.md
--rw-r--r--   0 briford    (501) staff       (20)      463 2023-12-24 17:18:24.000000 sageworks-0.5.3/SECURITY.md
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-01 17:30:51.988452 sageworks-0.5.3/applications/
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-01 17:30:52.004396 sageworks-0.5.3/applications/aws_dashboard/
--rw-r--r--   0 briford    (501) staff       (20)     1071 2024-04-01 16:28:50.000000 sageworks-0.5.3/applications/aws_dashboard/Dockerfile
--rw-r--r--   0 briford    (501) staff       (20)      331 2024-03-28 17:23:43.000000 sageworks-0.5.3/applications/aws_dashboard/Dockerfile_plugins
--rw-r--r--   0 briford    (501) staff       (20)      841 2024-01-10 18:45:51.000000 sageworks-0.5.3/applications/aws_dashboard/README.md
--rw-r--r--   0 briford    (501) staff       (20)     1296 2024-03-28 17:23:43.000000 sageworks-0.5.3/applications/aws_dashboard/app.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-01 17:30:52.005245 sageworks-0.5.3/applications/aws_dashboard/assets/
--rw-r--r--   0 briford    (501) staff       (20)    14995 2024-03-28 17:23:43.000000 sageworks-0.5.3/applications/aws_dashboard/assets/custom.css
--rw-r--r--   0 briford    (501) staff       (20)      318 2023-12-24 17:18:24.000000 sageworks-0.5.3/applications/aws_dashboard/assets/favicon.ico
--rw-r--r--   0 briford    (501) staff       (20)      732 2023-12-24 17:18:24.000000 sageworks-0.5.3/applications/aws_dashboard/assets/trash.png
--rwxr-xr-x   0 briford    (501) staff       (20)      644 2024-03-31 16:51:01.000000 sageworks-0.5.3/applications/aws_dashboard/dashboard
--rw-r--r--   0 briford    (501) staff       (20)      205 2023-12-24 17:18:24.000000 sageworks-0.5.3/applications/aws_dashboard/nginx.conf
--rw-r--r--   0 briford    (501) staff       (20)      684 2024-03-28 17:23:43.000000 sageworks-0.5.3/applications/aws_dashboard/open_source_config.json
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-01 17:30:51.988380 sageworks-0.5.3/applications/aws_dashboard/pages/
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-01 17:30:52.005716 sageworks-0.5.3/applications/aws_dashboard/pages/data_sources/
--rw-r--r--   0 briford    (501) staff       (20)    11696 2024-03-30 22:43:51.000000 sageworks-0.5.3/applications/aws_dashboard/pages/data_sources/callbacks.py
--rw-r--r--   0 briford    (501) staff       (20)     2756 2024-03-28 17:23:43.000000 sageworks-0.5.3/applications/aws_dashboard/pages/data_sources/layout.py
--rw-r--r--   0 briford    (501) staff       (20)     2555 2024-03-28 17:23:43.000000 sageworks-0.5.3/applications/aws_dashboard/pages/data_sources/page.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-01 17:30:52.006100 sageworks-0.5.3/applications/aws_dashboard/pages/endpoints/
--rw-r--r--   0 briford    (501) staff       (20)     3975 2024-03-30 22:43:51.000000 sageworks-0.5.3/applications/aws_dashboard/pages/endpoints/callbacks.py
--rw-r--r--   0 briford    (501) staff       (20)     2565 2024-03-28 17:23:43.000000 sageworks-0.5.3/applications/aws_dashboard/pages/endpoints/layout.py
--rw-r--r--   0 briford    (501) staff       (20)     2465 2024-03-28 17:23:43.000000 sageworks-0.5.3/applications/aws_dashboard/pages/endpoints/page.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-01 17:30:52.006464 sageworks-0.5.3/applications/aws_dashboard/pages/feature_sets/
--rw-r--r--   0 briford    (501) staff       (20)    11610 2024-03-30 22:43:51.000000 sageworks-0.5.3/applications/aws_dashboard/pages/feature_sets/callbacks.py
--rw-r--r--   0 briford    (501) staff       (20)     2438 2024-03-28 17:23:43.000000 sageworks-0.5.3/applications/aws_dashboard/pages/feature_sets/layout.py
--rw-r--r--   0 briford    (501) staff       (20)     2505 2024-03-28 17:23:43.000000 sageworks-0.5.3/applications/aws_dashboard/pages/feature_sets/page.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-01 17:30:52.006822 sageworks-0.5.3/applications/aws_dashboard/pages/main/
--rw-r--r--   0 briford    (501) staff       (20)     4899 2024-03-30 22:43:51.000000 sageworks-0.5.3/applications/aws_dashboard/pages/main/callbacks.py
--rw-r--r--   0 briford    (501) staff       (20)     2899 2024-03-28 17:23:43.000000 sageworks-0.5.3/applications/aws_dashboard/pages/main/layout.py
--rw-r--r--   0 briford    (501) staff       (20)     1844 2024-03-28 17:23:43.000000 sageworks-0.5.3/applications/aws_dashboard/pages/main/page.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-01 17:30:52.007172 sageworks-0.5.3/applications/aws_dashboard/pages/models/
--rw-r--r--   0 briford    (501) staff       (20)     3672 2024-03-30 22:43:51.000000 sageworks-0.5.3/applications/aws_dashboard/pages/models/callbacks.py
--rw-r--r--   0 briford    (501) staff       (20)     2020 2024-03-28 17:23:43.000000 sageworks-0.5.3/applications/aws_dashboard/pages/models/layout.py
--rw-r--r--   0 briford    (501) staff       (20)     2341 2024-03-28 17:23:43.000000 sageworks-0.5.3/applications/aws_dashboard/pages/models/page.py
--rw-r--r--   0 briford    (501) staff       (20)      394 2024-04-01 13:00:51.000000 sageworks-0.5.3/applications/aws_dashboard/requirements.txt
--rw-r--r--   0 briford    (501) staff       (20)      457 2023-12-24 17:18:24.000000 sageworks-0.5.3/applications/aws_dashboard/supervisord.conf
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-01 17:30:51.988506 sageworks-0.5.3/applications/experiments/
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-01 17:30:52.008065 sageworks-0.5.3/applications/experiments/compound_explorer/
--rw-r--r--   0 briford    (501) staff       (20)      181 2023-12-24 17:18:24.000000 sageworks-0.5.3/applications/experiments/compound_explorer/Dockerfile
--rw-r--r--   0 briford    (501) staff       (20)      360 2023-12-24 17:18:24.000000 sageworks-0.5.3/applications/experiments/compound_explorer/README.md
--rw-r--r--   0 briford    (501) staff       (20)     3096 2024-03-28 17:23:43.000000 sageworks-0.5.3/applications/experiments/compound_explorer/app.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-01 17:30:52.008508 sageworks-0.5.3/applications/experiments/compound_explorer/assets/
--rw-r--r--   0 briford    (501) staff       (20)    12861 2023-12-24 17:18:24.000000 sageworks-0.5.3/applications/experiments/compound_explorer/assets/custom.css
--rw-r--r--   0 briford    (501) staff       (20)      318 2023-12-24 17:18:24.000000 sageworks-0.5.3/applications/experiments/compound_explorer/assets/favicon.ico
--rw-r--r--   0 briford    (501) staff       (20)     7676 2024-03-30 22:43:51.000000 sageworks-0.5.3/applications/experiments/compound_explorer/callbacks.py
--rw-r--r--   0 briford    (501) staff       (20)     4860 2024-03-28 17:23:43.000000 sageworks-0.5.3/applications/experiments/compound_explorer/layout.py
--rw-r--r--   0 briford    (501) staff       (20)       94 2023-12-24 17:18:24.000000 sageworks-0.5.3/applications/experiments/compound_explorer/requirements.txt
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-01 17:30:52.008921 sageworks-0.5.3/aws_setup/
--rw-r--r--   0 briford    (501) staff       (20)     3582 2024-03-28 17:23:43.000000 sageworks-0.5.3/aws_setup/aws_account_check.py
--rw-r--r--   0 briford    (501) staff       (20)     1403 2024-03-28 17:23:43.000000 sageworks-0.5.3/aws_setup/aws_identity_check.py
--rw-r--r--   0 briford    (501) staff       (20)     2629 2024-03-28 17:23:43.000000 sageworks-0.5.3/aws_setup/build_ml_pipeline.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-01 17:30:52.009041 sageworks-0.5.3/aws_setup/event_bridge/
--rw-r--r--   0 briford    (501) staff       (20)       60 2023-12-24 17:18:24.000000 sageworks-0.5.3/aws_setup/event_bridge/Readme.md
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-01 17:30:52.009787 sageworks-0.5.3/aws_setup/event_bridge/dynamic_docker/
--rw-r--r--   0 briford    (501) staff       (20)       60 2023-12-24 17:18:24.000000 sageworks-0.5.3/aws_setup/event_bridge/dynamic_docker/Readme.md
--rw-r--r--   0 briford    (501) staff       (20)     1007 2023-12-24 17:18:24.000000 sageworks-0.5.3/aws_setup/event_bridge/dynamic_docker/app.py
--rw-r--r--   0 briford    (501) staff       (20)     2567 2023-12-24 17:18:24.000000 sageworks-0.5.3/aws_setup/event_bridge/dynamic_docker/cdk.json
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-01 17:30:52.010041 sageworks-0.5.3/aws_setup/event_bridge/dynamic_docker/lambda/
--rw-r--r--   0 briford    (501) staff       (20)     1812 2024-01-10 18:45:51.000000 sageworks-0.5.3/aws_setup/event_bridge/dynamic_docker/lambda/lambda_replace_task.py
--rw-r--r--   0 briford    (501) staff       (20)     2599 2024-03-27 20:43:31.000000 sageworks-0.5.3/aws_setup/event_bridge/dynamic_docker/sageworks_image_update_stack.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-01 17:30:52.011241 sageworks-0.5.3/aws_setup/sageworks_core/
--rw-r--r--   0 briford    (501) staff       (20)      119 2023-12-24 17:18:24.000000 sageworks-0.5.3/aws_setup/sageworks_core/.gitignore
--rw-r--r--   0 briford    (501) staff       (20)     1028 2023-12-24 17:18:24.000000 sageworks-0.5.3/aws_setup/sageworks_core/README.md
--rw-r--r--   0 briford    (501) staff       (20)     1403 2024-03-28 17:23:43.000000 sageworks-0.5.3/aws_setup/sageworks_core/app.py
--rw-r--r--   0 briford    (501) staff       (20)     1998 2023-12-24 17:18:24.000000 sageworks-0.5.3/aws_setup/sageworks_core/cdk.json
--rw-r--r--   0 briford    (501) staff       (20)       14 2023-12-24 17:18:24.000000 sageworks-0.5.3/aws_setup/sageworks_core/requirements-dev.txt
--rw-r--r--   0 briford    (501) staff       (20)       53 2024-01-10 18:45:51.000000 sageworks-0.5.3/aws_setup/sageworks_core/requirements.txt
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-01 17:30:52.011555 sageworks-0.5.3/aws_setup/sageworks_core/sageworks_core/
--rw-r--r--   0 briford    (501) staff       (20)        0 2024-01-10 18:45:51.000000 sageworks-0.5.3/aws_setup/sageworks_core/sageworks_core/__init__.py
--rw-r--r--   0 briford    (501) staff       (20)    23575 2024-03-28 17:23:43.000000 sageworks-0.5.3/aws_setup/sageworks_core/sageworks_core/sageworks_core_stack.py
--rw-r--r--   0 briford    (501) staff       (20)      437 2023-12-24 17:18:24.000000 sageworks-0.5.3/aws_setup/sageworks_core/source.bat
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-01 17:30:52.011727 sageworks-0.5.3/aws_setup/sageworks_core/tests/
--rw-r--r--   0 briford    (501) staff       (20)        0 2023-12-24 17:18:24.000000 sageworks-0.5.3/aws_setup/sageworks_core/tests/__init__.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-01 17:30:52.011933 sageworks-0.5.3/aws_setup/sageworks_core/tests/unit/
--rw-r--r--   0 briford    (501) staff       (20)        0 2023-12-24 17:18:24.000000 sageworks-0.5.3/aws_setup/sageworks_core/tests/unit/__init__.py
--rw-r--r--   0 briford    (501) staff       (20)      720 2023-12-24 17:18:24.000000 sageworks-0.5.3/aws_setup/sageworks_core/tests/unit/test_sageworks_sandbox_stack.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-01 17:30:52.013132 sageworks-0.5.3/aws_setup/sageworks_dashboard_full/
--rw-r--r--   0 briford    (501) staff       (20)      119 2023-12-24 17:18:24.000000 sageworks-0.5.3/aws_setup/sageworks_dashboard_full/.gitignore
--rw-r--r--   0 briford    (501) staff       (20)     1778 2024-03-28 17:23:43.000000 sageworks-0.5.3/aws_setup/sageworks_dashboard_full/README.md
--rw-r--r--   0 briford    (501) staff       (20)     1907 2024-03-28 17:23:43.000000 sageworks-0.5.3/aws_setup/sageworks_dashboard_full/app.py
--rw-r--r--   0 briford    (501) staff       (20)     2567 2023-12-24 17:18:24.000000 sageworks-0.5.3/aws_setup/sageworks_dashboard_full/cdk.json
--rw-r--r--   0 briford    (501) staff       (20)       14 2023-12-24 17:18:24.000000 sageworks-0.5.3/aws_setup/sageworks_dashboard_full/requirements-dev.txt
--rw-r--r--   0 briford    (501) staff       (20)       47 2023-12-24 17:18:24.000000 sageworks-0.5.3/aws_setup/sageworks_dashboard_full/requirements.txt
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-01 17:30:52.013383 sageworks-0.5.3/aws_setup/sageworks_dashboard_full/sageworks_dashboard_full/
--rw-r--r--   0 briford    (501) staff       (20)        0 2023-12-24 17:18:24.000000 sageworks-0.5.3/aws_setup/sageworks_dashboard_full/sageworks_dashboard_full/__init__.py
--rw-r--r--   0 briford    (501) staff       (20)     7022 2024-04-01 16:30:57.000000 sageworks-0.5.3/aws_setup/sageworks_dashboard_full/sageworks_dashboard_full/sageworks_dashboard_stack.py
--rw-r--r--   0 briford    (501) staff       (20)      437 2023-12-24 17:18:24.000000 sageworks-0.5.3/aws_setup/sageworks_dashboard_full/source.bat
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-01 17:30:52.013510 sageworks-0.5.3/aws_setup/sageworks_dashboard_full/tests/
--rw-r--r--   0 briford    (501) staff       (20)        0 2023-12-24 17:18:24.000000 sageworks-0.5.3/aws_setup/sageworks_dashboard_full/tests/__init__.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-01 17:30:52.013714 sageworks-0.5.3/aws_setup/sageworks_dashboard_full/tests/unit/
--rw-r--r--   0 briford    (501) staff       (20)        0 2023-12-24 17:18:24.000000 sageworks-0.5.3/aws_setup/sageworks_dashboard_full/tests/unit/__init__.py
--rw-r--r--   0 briford    (501) staff       (20)      565 2023-12-24 17:18:24.000000 sageworks-0.5.3/aws_setup/sageworks_dashboard_full/tests/unit/test_sageworks_dashboard_stack.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-01 17:30:52.014482 sageworks-0.5.3/aws_setup/sageworks_dashboard_lite/
--rw-r--r--   0 briford    (501) staff       (20)      119 2024-03-28 17:23:43.000000 sageworks-0.5.3/aws_setup/sageworks_dashboard_lite/.gitignore
--rw-r--r--   0 briford    (501) staff       (20)     1778 2024-03-28 17:23:43.000000 sageworks-0.5.3/aws_setup/sageworks_dashboard_lite/README.md
--rw-r--r--   0 briford    (501) staff       (20)     1928 2024-03-28 17:23:43.000000 sageworks-0.5.3/aws_setup/sageworks_dashboard_lite/app.py
--rw-r--r--   0 briford    (501) staff       (20)     2567 2024-03-28 17:23:43.000000 sageworks-0.5.3/aws_setup/sageworks_dashboard_lite/cdk.json
--rw-r--r--   0 briford    (501) staff       (20)       47 2024-03-28 17:23:43.000000 sageworks-0.5.3/aws_setup/sageworks_dashboard_lite/requirements.txt
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-01 17:30:52.015044 sageworks-0.5.3/aws_setup/sageworks_dashboard_lite/sageworks_dashboard_lite/
--rw-r--r--   0 briford    (501) staff       (20)        0 2024-03-28 17:23:43.000000 sageworks-0.5.3/aws_setup/sageworks_dashboard_lite/sageworks_dashboard_lite/__init__.py
--rw-r--r--   0 briford    (501) staff       (20)     6849 2024-04-01 15:22:44.000000 sageworks-0.5.3/aws_setup/sageworks_dashboard_lite/sageworks_dashboard_lite/sageworks_dashboard_stack.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-01 17:30:52.016296 sageworks-0.5.3/data/
--rw-r--r--   0 briford    (501) staff       (20)   191978 2023-12-24 17:18:24.000000 sageworks-0.5.3/data/abalone.csv
--rw-r--r--   0 briford    (501) staff       (20)     1515 2023-12-24 17:18:24.000000 sageworks-0.5.3/data/test_data.csv
--rw-r--r--   0 briford    (501) staff       (20)     2270 2023-12-24 17:18:24.000000 sageworks-0.5.3/data/test_data.json
--rw-r--r--   0 briford    (501) staff       (20)    12977 2024-01-10 18:45:51.000000 sageworks-0.5.3/data/wine_dataset.csv
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-01 17:30:52.016551 sageworks-0.5.3/docs/
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-01 17:30:52.016852 sageworks-0.5.3/docs/admin/
--rw-r--r--   0 briford    (501) staff       (20)     1825 2024-03-28 17:23:43.000000 sageworks-0.5.3/docs/admin/docker_push.md
--rw-r--r--   0 briford    (501) staff       (20)     1633 2024-01-10 18:45:51.000000 sageworks-0.5.3/docs/admin/pypi_release.md
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-01 17:30:52.018500 sageworks-0.5.3/docs/api_classes/
--rw-r--r--   0 briford    (501) staff       (20)     3595 2024-01-23 15:36:53.000000 sageworks-0.5.3/docs/api_classes/data_source.md
--rw-r--r--   0 briford    (501) staff       (20)     5199 2024-03-28 17:23:43.000000 sageworks-0.5.3/docs/api_classes/endpoint.md
--rw-r--r--   0 briford    (501) staff       (20)     6299 2024-03-28 17:23:43.000000 sageworks-0.5.3/docs/api_classes/feature_set.md
--rw-r--r--   0 briford    (501) staff       (20)     5350 2024-03-30 23:05:32.000000 sageworks-0.5.3/docs/api_classes/meta.md
--rw-r--r--   0 briford    (501) staff       (20)     4356 2024-01-10 18:45:51.000000 sageworks-0.5.3/docs/api_classes/model.md
--rw-r--r--   0 briford    (501) staff       (20)     2218 2024-01-10 18:45:51.000000 sageworks-0.5.3/docs/api_classes/monitor.md
--rw-r--r--   0 briford    (501) staff       (20)     3549 2024-01-10 18:45:51.000000 sageworks-0.5.3/docs/api_classes/overview.md
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-01 17:30:52.019426 sageworks-0.5.3/docs/aws_setup/
--rw-r--r--   0 briford    (501) staff       (20)     1121 2024-03-28 17:23:43.000000 sageworks-0.5.3/docs/aws_setup/aws_access_management.md
--rw-r--r--   0 briford    (501) staff       (20)     7836 2024-01-23 15:36:53.000000 sageworks-0.5.3/docs/aws_setup/aws_tips_and_tricks.md
--rw-r--r--   0 briford    (501) staff       (20)     4229 2024-03-28 17:23:43.000000 sageworks-0.5.3/docs/aws_setup/core_stack.md
--rw-r--r--   0 briford    (501) staff       (20)     2075 2024-03-28 17:23:43.000000 sageworks-0.5.3/docs/aws_setup/dashboard_stack.md
--rw-r--r--   0 briford    (501) staff       (20)     2540 2024-01-23 15:36:53.000000 sageworks-0.5.3/docs/aws_setup/full_pipeline.md
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-01 17:30:52.019674 sageworks-0.5.3/docs/concepts/
--rw-r--r--   0 briford    (501) staff       (20)      907 2024-01-23 15:36:53.000000 sageworks-0.5.3/docs/concepts/model_monitoring.md
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-01 17:30:52.019918 sageworks-0.5.3/docs/core_classes/
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-01 17:30:52.021447 sageworks-0.5.3/docs/core_classes/artifacts/
--rw-r--r--   0 briford    (501) staff       (20)      464 2024-01-23 15:36:53.000000 sageworks-0.5.3/docs/core_classes/artifacts/artifact.md
--rw-r--r--   0 briford    (501) staff       (20)      290 2024-01-10 18:45:51.000000 sageworks-0.5.3/docs/core_classes/artifacts/athena_source.md
--rw-r--r--   0 briford    (501) staff       (20)      479 2024-01-23 15:36:53.000000 sageworks-0.5.3/docs/core_classes/artifacts/data_source_abstract.md
--rw-r--r--   0 briford    (501) staff       (20)      292 2024-01-10 18:45:51.000000 sageworks-0.5.3/docs/core_classes/artifacts/endpoint_core.md
--rw-r--r--   0 briford    (501) staff       (20)      294 2024-01-10 18:45:51.000000 sageworks-0.5.3/docs/core_classes/artifacts/feature_set_core.md
--rw-r--r--   0 briford    (501) staff       (20)      281 2024-01-10 18:45:51.000000 sageworks-0.5.3/docs/core_classes/artifacts/model_core.md
--rw-r--r--   0 briford    (501) staff       (20)      289 2024-01-10 18:45:51.000000 sageworks-0.5.3/docs/core_classes/artifacts/monitor_core.md
--rw-r--r--   0 briford    (501) staff       (20)      861 2024-01-10 18:45:51.000000 sageworks-0.5.3/docs/core_classes/artifacts/overview.md
--rw-r--r--   0 briford    (501) staff       (20)     2119 2024-01-10 18:45:51.000000 sageworks-0.5.3/docs/core_classes/overview.md
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-01 17:30:52.022875 sageworks-0.5.3/docs/core_classes/transforms/
--rw-r--r--   0 briford    (501) staff       (20)      352 2024-01-10 18:45:51.000000 sageworks-0.5.3/docs/core_classes/transforms/data_loaders_heavy.md
--rw-r--r--   0 briford    (501) staff       (20)      396 2024-01-10 18:45:51.000000 sageworks-0.5.3/docs/core_classes/transforms/data_loaders_light.md
--rw-r--r--   0 briford    (501) staff       (20)      349 2024-03-28 17:23:43.000000 sageworks-0.5.3/docs/core_classes/transforms/data_to_features.md
--rw-r--r--   0 briford    (501) staff       (20)      265 2024-01-10 18:45:51.000000 sageworks-0.5.3/docs/core_classes/transforms/features_to_model.md
--rw-r--r--   0 briford    (501) staff       (20)      264 2024-01-10 18:45:51.000000 sageworks-0.5.3/docs/core_classes/transforms/model_to_endpoint.md
--rw-r--r--   0 briford    (501) staff       (20)     1177 2024-01-10 18:45:51.000000 sageworks-0.5.3/docs/core_classes/transforms/overview.md
--rw-r--r--   0 briford    (501) staff       (20)      970 2024-01-23 15:36:53.000000 sageworks-0.5.3/docs/core_classes/transforms/pandas_transforms.md
--rw-r--r--   0 briford    (501) staff       (20)      521 2024-01-23 15:36:53.000000 sageworks-0.5.3/docs/core_classes/transforms/transform.md
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-01 17:30:52.023072 sageworks-0.5.3/docs/glue/
--rw-r--r--   0 briford    (501) staff       (20)     4837 2024-03-28 17:23:43.000000 sageworks-0.5.3/docs/glue/index.md
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-01 17:30:52.028663 sageworks-0.5.3/docs/images/
--rw-r--r--   0 briford    (501) staff       (20)   605827 2023-12-24 17:18:24.000000 sageworks-0.5.3/docs/images/big_spider.png
--rw-r--r--   0 briford    (501) staff       (20)    32320 2023-12-24 17:18:24.000000 sageworks-0.5.3/docs/images/graph_representation.png
--rw-r--r--   0 briford    (501) staff       (20)    15549 2023-12-24 17:18:24.000000 sageworks-0.5.3/docs/images/powered_aws_dark_blue.png
--rw-r--r--   0 briford    (501) staff       (20)    10003 2023-12-24 17:18:24.000000 sageworks-0.5.3/docs/images/powered_aws_transparent.png
--rw-r--r--   0 briford    (501) staff       (20)     6435 2023-12-24 17:18:24.000000 sageworks-0.5.3/docs/images/powered_aws_white.png
--rw-r--r--   0 briford    (501) staff       (20)    21174 2023-12-24 17:18:24.000000 sageworks-0.5.3/docs/images/powered_aws_with_tm_grey.png
--rw-r--r--   0 briford    (501) staff       (20)    51137 2023-12-24 17:18:24.000000 sageworks-0.5.3/docs/images/sageworks.png
--rw-r--r--   0 briford    (501) staff       (20)   489672 2023-12-24 17:18:24.000000 sageworks-0.5.3/docs/images/sageworks_concepts.png
--rw-r--r--   0 briford    (501) staff       (20)    30017 2023-12-24 17:18:24.000000 sageworks-0.5.3/docs/images/scp.png
--rw-r--r--   0 briford    (501) staff       (20)   139307 2023-12-24 17:18:24.000000 sageworks-0.5.3/docs/images/scp_labs.png
--rw-r--r--   0 briford    (501) staff       (20)   381209 2023-12-24 17:18:24.000000 sageworks-0.5.3/docs/images/small_spider.png
--rw-r--r--   0 briford    (501) staff       (20)     3417 2024-03-28 17:23:43.000000 sageworks-0.5.3/docs/index.md
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-01 17:30:52.030239 sageworks-0.5.3/docs/misc/
--rw-r--r--   0 briford    (501) staff       (20)     2791 2024-03-28 17:23:43.000000 sageworks-0.5.3/docs/misc/faq.md
--rw-r--r--   0 briford    (501) staff       (20)     5069 2024-01-10 18:45:51.000000 sageworks-0.5.3/docs/misc/general_info.md
--rw-r--r--   0 briford    (501) staff       (20)      667 2024-01-10 18:45:51.000000 sageworks-0.5.3/docs/misc/sageworks_classes_concepts.md
--rw-r--r--   0 briford    (501) staff       (20)     1873 2024-01-10 18:45:51.000000 sageworks-0.5.3/docs/misc/scp_consulting.md
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-01 17:30:52.030816 sageworks-0.5.3/docs/plugins/
--rw-r--r--   0 briford    (501) staff       (20)     3100 2024-04-01 00:11:00.000000 sageworks-0.5.3/docs/plugins/index.md
--rw-r--r--   0 briford    (501) staff       (20)      750 2024-03-31 15:49:43.000000 sageworks-0.5.3/docs/plugins/plugin_api_changes.md
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-01 17:30:52.031140 sageworks-0.5.3/docs/repl/
--rw-r--r--   0 briford    (501) staff       (20)     2081 2024-03-28 17:23:43.000000 sageworks-0.5.3/docs/repl/index.md
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-01 17:30:52.031583 sageworks-0.5.3/docs/research/
--rw-r--r--   0 briford    (501) staff       (20)      912 2024-03-28 17:23:43.000000 sageworks-0.5.3/docs/research/eda.md
--rw-r--r--   0 briford    (501) staff       (20)     2017 2024-03-28 17:23:43.000000 sageworks-0.5.3/docs/research/htg.md
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-01 17:30:52.036291 sageworks-0.5.3/examples/
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-01 17:30:52.036439 sageworks-0.5.3/examples/ag-grid/
--rw-r--r--   0 briford    (501) staff       (20)      496 2024-03-31 22:06:56.000000 sageworks-0.5.3/examples/ag-grid/hello_world.py
--rw-r--r--   0 briford    (501) staff       (20)      326 2024-01-10 18:45:51.000000 sageworks-0.5.3/examples/datasource_from_df.py
--rw-r--r--   0 briford    (501) staff       (20)      332 2024-01-10 18:45:51.000000 sageworks-0.5.3/examples/datasource_from_s3.py
--rw-r--r--   0 briford    (501) staff       (20)      536 2024-01-23 15:36:53.000000 sageworks-0.5.3/examples/datasource_query.py
--rw-r--r--   0 briford    (501) staff       (20)      680 2024-01-23 15:36:53.000000 sageworks-0.5.3/examples/datasource_stats.py
--rw-r--r--   0 briford    (501) staff       (20)      223 2024-01-10 18:45:51.000000 sageworks-0.5.3/examples/datasource_to_featureset.py
--rw-r--r--   0 briford    (501) staff       (20)      199 2024-01-10 18:45:51.000000 sageworks-0.5.3/examples/endpoint_details.py
--rw-r--r--   0 briford    (501) staff       (20)      834 2024-03-28 17:23:43.000000 sageworks-0.5.3/examples/endpoint_inference.py
--rw-r--r--   0 briford    (501) staff       (20)      481 2024-01-10 18:45:51.000000 sageworks-0.5.3/examples/endpoint_metrics.py
--rw-r--r--   0 briford    (501) staff       (20)      744 2024-01-10 18:45:51.000000 sageworks-0.5.3/examples/featureset_eda.py
--rw-r--r--   0 briford    (501) staff       (20)      560 2024-03-28 17:23:43.000000 sageworks-0.5.3/examples/featureset_query.py
--rw-r--r--   0 briford    (501) staff       (20)      421 2024-03-27 20:32:26.000000 sageworks-0.5.3/examples/featureset_to_model.py
--rw-r--r--   0 briford    (501) staff       (20)     1534 2024-03-28 17:23:43.000000 sageworks-0.5.3/examples/full_ml_pipeline.py
--rw-r--r--   0 briford    (501) staff       (20)      580 2024-01-23 15:36:53.000000 sageworks-0.5.3/examples/glue_hello_world.py
--rw-r--r--   0 briford    (501) staff       (20)      942 2024-01-23 15:36:53.000000 sageworks-0.5.3/examples/glue_hello_world_with_log.py
--rw-r--r--   0 briford    (501) staff       (20)      686 2024-01-23 15:36:53.000000 sageworks-0.5.3/examples/glue_load_s3_bucket.py
--rw-r--r--   0 briford    (501) staff       (20)      363 2024-03-30 22:43:51.000000 sageworks-0.5.3/examples/meta_list_endpoints.py
--rw-r--r--   0 briford    (501) staff       (20)      328 2024-03-30 22:43:51.000000 sageworks-0.5.3/examples/meta_list_models.py
--rw-r--r--   0 briford    (501) staff       (20)      659 2024-03-30 22:43:51.000000 sageworks-0.5.3/examples/meta_model_metrics.py
--rw-r--r--   0 briford    (501) staff       (20)      548 2024-03-28 17:23:43.000000 sageworks-0.5.3/examples/model_metrics.py
--rw-r--r--   0 briford    (501) staff       (20)      312 2024-03-27 20:32:26.000000 sageworks-0.5.3/examples/model_to_endpoint.py
--rw-r--r--   0 briford    (501) staff       (20)      400 2024-01-10 18:45:51.000000 sageworks-0.5.3/examples/monitor_setup.py
--rw-r--r--   0 briford    (501) staff       (20)      765 2024-01-10 18:45:51.000000 sageworks-0.5.3/examples/monitor_usage.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-01 17:30:51.991204 sageworks-0.5.3/examples/plugins/
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-01 17:30:52.036678 sageworks-0.5.3/examples/plugins/pages/
--rw-r--r--   0 briford    (501) staff       (20)     2474 2024-03-31 19:33:46.000000 sageworks-0.5.3/examples/plugins/pages/my_plugin_page.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-01 17:30:52.037048 sageworks-0.5.3/examples/plugins/views/
--rw-r--r--   0 briford    (501) staff       (20)     1264 2024-03-31 19:19:35.000000 sageworks-0.5.3/examples/plugins/views/my_view_plugin.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-01 17:30:52.037693 sageworks-0.5.3/examples/plugins/web_components/
--rw-r--r--   0 briford    (501) staff       (20)     1666 2024-03-31 18:52:26.000000 sageworks-0.5.3/examples/plugins/web_components/endpoint_plugin.py
--rw-r--r--   0 briford    (501) staff       (20)     1942 2024-03-31 22:06:56.000000 sageworks-0.5.3/examples/plugins/web_components/model_plugin.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-01 17:30:52.038156 sageworks-0.5.3/examples/sagemaker_pipelines/
--rw-r--r--   0 briford    (501) staff       (20)      854 2024-03-28 17:23:43.000000 sageworks-0.5.3/examples/sagemaker_pipelines/all_steps.py
--rw-r--r--   0 briford    (501) staff       (20)       40 2024-03-28 17:23:43.000000 sageworks-0.5.3/examples/sagemaker_pipelines/hello.py
--rw-r--r--   0 briford    (501) staff       (20)     1487 2024-03-28 17:23:43.000000 sageworks-0.5.3/examples/sagemaker_pipelines/ml_pipeline.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-01 17:30:51.991418 sageworks-0.5.3/examples/sagemaker_pipelines/storage/
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-01 17:30:52.038755 sageworks-0.5.3/examples/sagemaker_pipelines/storage/full_pipeline_experiment/
--rw-r--r--   0 briford    (501) staff       (20)      854 2024-03-28 17:23:43.000000 sageworks-0.5.3/examples/sagemaker_pipelines/storage/full_pipeline_experiment/data_source.py
--rw-r--r--   0 briford    (501) staff       (20)      203 2024-03-28 17:23:43.000000 sageworks-0.5.3/examples/sagemaker_pipelines/storage/full_pipeline_experiment/endpoint.py
--rw-r--r--   0 briford    (501) staff       (20)      160 2024-03-28 17:23:43.000000 sageworks-0.5.3/examples/sagemaker_pipelines/storage/full_pipeline_experiment/feature_set.py
--rw-r--r--   0 briford    (501) staff       (20)     1599 2024-03-28 17:23:43.000000 sageworks-0.5.3/examples/sagemaker_pipelines/storage/full_pipeline_experiment/ml_pipeline.py
--rw-r--r--   0 briford    (501) staff       (20)      367 2024-03-28 17:23:43.000000 sageworks-0.5.3/examples/sagemaker_pipelines/storage/full_pipeline_experiment/model.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-01 17:30:52.039596 sageworks-0.5.3/examples/storage/
--rw-r--r--   0 briford    (501) staff       (20)     1222 2024-03-27 20:40:53.000000 sageworks-0.5.3/examples/storage/data_to_data.py
--rw-r--r--   0 briford    (501) staff       (20)      856 2024-03-27 20:40:53.000000 sageworks-0.5.3/examples/storage/data_to_features.py
--rw-r--r--   0 briford    (501) staff       (20)     1371 2024-03-28 17:23:43.000000 sageworks-0.5.3/examples/storage/endpoint_inference.py
--rw-r--r--   0 briford    (501) staff       (20)     1847 2024-03-28 17:23:43.000000 sageworks-0.5.3/examples/storage/hello_world_pipeline.py
--rw-r--r--   0 briford    (501) staff       (20)     4378 2024-03-31 17:04:46.000000 sageworks-0.5.3/examples/storage/plugin_page_example.py
--rw-r--r--   0 briford    (501) staff       (20)     2750 2024-03-31 15:47:34.000000 sageworks-0.5.3/mkdocs.yml
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-01 17:30:52.040869 sageworks-0.5.3/notebooks/
--rw-r--r--   0 briford    (501) staff       (20)   185443 2024-03-28 17:23:43.000000 sageworks-0.5.3/notebooks/ML_Pipeline_with_SageWorks.ipynb
--rw-r--r--   0 briford    (501) staff       (20)    36405 2024-03-28 17:23:43.000000 sageworks-0.5.3/notebooks/ML_Pipeline_with_SageWorks_2.ipynb
--rw-r--r--   0 briford    (501) staff       (20)   511134 2024-03-28 17:23:43.000000 sageworks-0.5.3/notebooks/Outliers_in_SageWorks.ipynb
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-01 17:30:52.048410 sageworks-0.5.3/notebooks/images/
--rw-r--r--   0 briford    (501) staff       (20)   142099 2023-12-24 17:18:24.000000 sageworks-0.5.3/notebooks/images/athena_query_aqsol.png
--rw-r--r--   0 briford    (501) staff       (20)   191022 2023-12-24 17:18:24.000000 sageworks-0.5.3/notebooks/images/aws_dashboard_aqsol.png
--rw-r--r--   0 briford    (501) staff       (20)   222686 2023-12-24 17:18:24.000000 sageworks-0.5.3/notebooks/images/dashboard_aqsol_features.png
--rw-r--r--   0 briford    (501) staff       (20)   171441 2023-12-24 17:18:24.000000 sageworks-0.5.3/notebooks/images/model_screenshot.png
--rw-r--r--   0 briford    (501) staff       (20)   489672 2023-12-24 17:18:24.000000 sageworks-0.5.3/notebooks/images/sageworks_concepts.png
--rw-r--r--   0 briford    (501) staff       (20)   139307 2023-12-24 17:18:24.000000 sageworks-0.5.3/notebooks/images/scp_labs.png
--rw-r--r--   0 briford    (501) staff       (20)      431 2024-04-01 12:59:42.000000 sageworks-0.5.3/requirements.txt
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-01 17:30:52.050237 sageworks-0.5.3/scripts/
--rw-r--r--   0 briford    (501) staff       (20)     2290 2024-03-28 17:23:43.000000 sageworks-0.5.3/scripts/athena_ddl_mixed_case.py
--rw-r--r--   0 briford    (501) staff       (20)     2178 2024-03-27 20:32:26.000000 sageworks-0.5.3/scripts/copy_data_catalog_db.py
--rw-r--r--   0 briford    (501) staff       (20)      706 2024-01-10 18:45:51.000000 sageworks-0.5.3/scripts/delete_redis_keys.py
--rw-r--r--   0 briford    (501) staff       (20)     1761 2024-03-28 17:23:43.000000 sageworks-0.5.3/scripts/glue_mixed_case.py
--rw-r--r--   0 briford    (501) staff       (20)     5544 2024-03-28 17:23:43.000000 sageworks-0.5.3/scripts/model_endpoint_sanity_check.py
--rw-r--r--   0 briford    (501) staff       (20)      715 2024-03-28 17:23:43.000000 sageworks-0.5.3/scripts/onboard_endpoints.py
--rw-r--r--   0 briford    (501) staff       (20)      694 2024-03-28 17:23:43.000000 sageworks-0.5.3/scripts/onboard_models.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-01 17:30:52.050695 sageworks-0.5.3/scripts/storage/
--rw-r--r--   0 briford    (501) staff       (20)     1003 2024-03-27 20:32:27.000000 sageworks-0.5.3/scripts/storage/dns_data_to_features.py
--rw-r--r--   0 briford    (501) staff       (20)     1723 2024-03-30 22:43:51.000000 sageworks-0.5.3/scripts/storage/generate_jsonl_data.py
--rw-r--r--   0 briford    (501) staff       (20)      955 2024-03-28 17:23:43.000000 sageworks-0.5.3/scripts/test_feature_resolution.py
--rw-r--r--   0 briford    (501) staff       (20)      533 2024-04-01 17:30:52.077257 sageworks-0.5.3/setup.cfg
--rw-r--r--   0 briford    (501) staff       (20)     1663 2024-03-27 20:32:27.000000 sageworks-0.5.3/setup.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-01 17:30:51.991969 sageworks-0.5.3/src/
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-01 17:30:52.050855 sageworks-0.5.3/src/sageworks/
--rw-r--r--   0 briford    (501) staff       (20)     1091 2024-01-10 18:45:51.000000 sageworks-0.5.3/src/sageworks/__init__.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-01 17:30:52.051894 sageworks-0.5.3/src/sageworks/algorithms/
--rw-r--r--   0 briford    (501) staff       (20)        0 2023-12-24 17:18:24.000000 sageworks-0.5.3/src/sageworks/algorithms/__init__.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-01 17:30:52.053026 sageworks-0.5.3/src/sageworks/algorithms/dataframe/
--rw-r--r--   0 briford    (501) staff       (20)      378 2023-12-24 17:18:24.000000 sageworks-0.5.3/src/sageworks/algorithms/dataframe/Readme.md
--rw-r--r--   0 briford    (501) staff       (20)     2852 2024-03-28 17:23:43.000000 sageworks-0.5.3/src/sageworks/algorithms/dataframe/aggregation.py
--rw-r--r--   0 briford    (501) staff       (20)     1606 2024-03-28 17:23:43.000000 sageworks-0.5.3/src/sageworks/algorithms/dataframe/data_source_eda.py
--rw-r--r--   0 briford    (501) staff       (20)     5388 2024-03-28 17:23:43.000000 sageworks-0.5.3/src/sageworks/algorithms/dataframe/dimensionality_reduction.py
--rw-r--r--   0 briford    (501) staff       (20)     9406 2024-03-28 17:23:43.000000 sageworks-0.5.3/src/sageworks/algorithms/dataframe/feature_resolution.py
--rw-r--r--   0 briford    (501) staff       (20)    12309 2024-03-28 17:23:43.000000 sageworks-0.5.3/src/sageworks/algorithms/dataframe/feature_spider.py
--rw-r--r--   0 briford    (501) staff       (20)     4968 2024-03-28 17:23:43.000000 sageworks-0.5.3/src/sageworks/algorithms/dataframe/row_tagger.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-01 17:30:51.992318 sageworks-0.5.3/src/sageworks/algorithms/graph/
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-01 17:30:52.053188 sageworks-0.5.3/src/sageworks/algorithms/graph/heavy/
--rw-r--r--   0 briford    (501) staff       (20)       96 2023-12-24 17:18:24.000000 sageworks-0.5.3/src/sageworks/algorithms/graph/heavy/Readme.md
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-01 17:30:52.053419 sageworks-0.5.3/src/sageworks/algorithms/graph/light/
--rw-r--r--   0 briford    (501) staff       (20)      122 2023-12-24 17:18:24.000000 sageworks-0.5.3/src/sageworks/algorithms/graph/light/Readme.md
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-01 17:30:52.053594 sageworks-0.5.3/src/sageworks/algorithms/spark/
--rw-r--r--   0 briford    (501) staff       (20)      615 2023-12-24 17:18:24.000000 sageworks-0.5.3/src/sageworks/algorithms/spark/Readme.md
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-01 17:30:52.054640 sageworks-0.5.3/src/sageworks/algorithms/sql/
--rw-r--r--   0 briford    (501) staff       (20)      685 2023-12-24 17:18:24.000000 sageworks-0.5.3/src/sageworks/algorithms/sql/Readme.md
--rw-r--r--   0 briford    (501) staff       (20)     6192 2024-03-28 17:23:43.000000 sageworks-0.5.3/src/sageworks/algorithms/sql/column_stats.py
--rw-r--r--   0 briford    (501) staff       (20)     3645 2024-03-28 17:23:43.000000 sageworks-0.5.3/src/sageworks/algorithms/sql/correlations.py
--rw-r--r--   0 briford    (501) staff       (20)     3622 2024-03-28 17:23:43.000000 sageworks-0.5.3/src/sageworks/algorithms/sql/descriptive_stats.py
--rw-r--r--   0 briford    (501) staff       (20)    10174 2024-03-28 17:23:43.000000 sageworks-0.5.3/src/sageworks/algorithms/sql/outliers.py
--rw-r--r--   0 briford    (501) staff       (20)     2352 2024-03-28 17:23:43.000000 sageworks-0.5.3/src/sageworks/algorithms/sql/sample_rows.py
--rw-r--r--   0 briford    (501) staff       (20)     3437 2024-03-28 17:23:43.000000 sageworks-0.5.3/src/sageworks/algorithms/sql/value_counts.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-01 17:30:52.055506 sageworks-0.5.3/src/sageworks/api/
--rw-r--r--   0 briford    (501) staff       (20)      708 2024-03-30 22:43:51.000000 sageworks-0.5.3/src/sageworks/api/__init__.py
--rw-r--r--   0 briford    (501) staff       (20)     7811 2024-03-28 17:23:43.000000 sageworks-0.5.3/src/sageworks/api/data_source.py
--rw-r--r--   0 briford    (501) staff       (20)     2505 2024-03-28 17:23:43.000000 sageworks-0.5.3/src/sageworks/api/endpoint.py
--rw-r--r--   0 briford    (501) staff       (20)     4242 2024-03-28 17:23:43.000000 sageworks-0.5.3/src/sageworks/api/feature_set.py
--rw-r--r--   0 briford    (501) staff       (20)    15642 2024-03-30 22:43:51.000000 sageworks-0.5.3/src/sageworks/api/meta.py
--rw-r--r--   0 briford    (501) staff       (20)     2577 2024-03-28 17:23:43.000000 sageworks-0.5.3/src/sageworks/api/model.py
--rw-r--r--   0 briford    (501) staff       (20)     5261 2024-03-28 17:23:43.000000 sageworks-0.5.3/src/sageworks/api/monitor.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-01 17:30:52.055763 sageworks-0.5.3/src/sageworks/aws_service_broker/
--rw-r--r--   0 briford    (501) staff       (20)     9393 2024-03-28 17:23:43.000000 sageworks-0.5.3/src/sageworks/aws_service_broker/aws_account_clamp.py
--rw-r--r--   0 briford    (501) staff       (20)    10908 2024-03-30 22:43:51.000000 sageworks-0.5.3/src/sageworks/aws_service_broker/aws_service_broker.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-01 17:30:52.056701 sageworks-0.5.3/src/sageworks/aws_service_broker/aws_service_connectors/
--rw-r--r--   0 briford    (501) staff       (20)        0 2023-12-24 17:18:24.000000 sageworks-0.5.3/src/sageworks/aws_service_broker/aws_service_connectors/__init__.py
--rw-r--r--   0 briford    (501) staff       (20)     1834 2024-03-28 17:23:43.000000 sageworks-0.5.3/src/sageworks/aws_service_broker/aws_service_connectors/connector.py
--rw-r--r--   0 briford    (501) staff       (20)     3258 2024-03-28 17:23:43.000000 sageworks-0.5.3/src/sageworks/aws_service_broker/aws_service_connectors/data_catalog.py
--rw-r--r--   0 briford    (501) staff       (20)     4055 2024-03-28 17:23:43.000000 sageworks-0.5.3/src/sageworks/aws_service_broker/aws_service_connectors/endpoints.py
--rw-r--r--   0 briford    (501) staff       (20)     5238 2024-03-28 17:23:43.000000 sageworks-0.5.3/src/sageworks/aws_service_broker/aws_service_connectors/feature_store.py
--rw-r--r--   0 briford    (501) staff       (20)     3712 2024-03-28 17:23:43.000000 sageworks-0.5.3/src/sageworks/aws_service_broker/aws_service_connectors/glue_jobs.py
--rw-r--r--   0 briford    (501) staff       (20)     3889 2024-03-28 17:23:43.000000 sageworks-0.5.3/src/sageworks/aws_service_broker/aws_service_connectors/model_registry.py
--rw-r--r--   0 briford    (501) staff       (20)     3736 2024-03-28 17:23:43.000000 sageworks-0.5.3/src/sageworks/aws_service_broker/aws_service_connectors/s3_bucket.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-01 17:30:52.056820 sageworks-0.5.3/src/sageworks/core/
--rw-r--r--   0 briford    (501) staff       (20)        0 2024-01-10 18:45:51.000000 sageworks-0.5.3/src/sageworks/core/__init__.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-01 17:30:52.058002 sageworks-0.5.3/src/sageworks/core/artifacts/
--rw-r--r--   0 briford    (501) staff       (20)      941 2024-03-28 17:23:43.000000 sageworks-0.5.3/src/sageworks/core/artifacts/__init__.py
--rw-r--r--   0 briford    (501) staff       (20)    17938 2024-03-30 22:43:51.000000 sageworks-0.5.3/src/sageworks/core/artifacts/artifact.py
--rw-r--r--   0 briford    (501) staff       (20)    22432 2024-03-30 22:43:51.000000 sageworks-0.5.3/src/sageworks/core/artifacts/athena_source.py
--rw-r--r--   0 briford    (501) staff       (20)    12683 2024-03-28 17:23:43.000000 sageworks-0.5.3/src/sageworks/core/artifacts/data_source_abstract.py
--rw-r--r--   0 briford    (501) staff       (20)     2447 2024-03-28 17:23:43.000000 sageworks-0.5.3/src/sageworks/core/artifacts/data_source_factory.py
--rw-r--r--   0 briford    (501) staff       (20)    36414 2024-03-28 17:23:43.000000 sageworks-0.5.3/src/sageworks/core/artifacts/endpoint_core.py
--rw-r--r--   0 briford    (501) staff       (20)    29123 2024-03-28 17:23:43.000000 sageworks-0.5.3/src/sageworks/core/artifacts/feature_set_core.py
--rw-r--r--   0 briford    (501) staff       (20)    35018 2024-03-29 21:27:39.000000 sageworks-0.5.3/src/sageworks/core/artifacts/model_core.py
--rw-r--r--   0 briford    (501) staff       (20)    21029 2024-03-28 17:23:43.000000 sageworks-0.5.3/src/sageworks/core/artifacts/monitor_core.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-01 17:30:52.058502 sageworks-0.5.3/src/sageworks/core/transforms/
--rw-r--r--   0 briford    (501) staff       (20)     1432 2024-01-10 18:45:51.000000 sageworks-0.5.3/src/sageworks/core/transforms/Readme.md
--rw-r--r--   0 briford    (501) staff       (20)        0 2024-01-10 18:45:51.000000 sageworks-0.5.3/src/sageworks/core/transforms/__init__.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-01 17:30:52.058642 sageworks-0.5.3/src/sageworks/core/transforms/data_loaders/
--rw-r--r--   0 briford    (501) staff       (20)        0 2024-01-10 18:45:51.000000 sageworks-0.5.3/src/sageworks/core/transforms/data_loaders/__init__.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-01 17:30:52.058874 sageworks-0.5.3/src/sageworks/core/transforms/data_loaders/heavy/
--rw-r--r--   0 briford    (501) staff       (20)      298 2024-03-28 17:23:43.000000 sageworks-0.5.3/src/sageworks/core/transforms/data_loaders/heavy/__init__.py
--rw-r--r--   0 briford    (501) staff       (20)     9866 2024-03-28 17:23:43.000000 sageworks-0.5.3/src/sageworks/core/transforms/data_loaders/heavy/s3_heavy_to_data_source.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-01 17:30:52.059360 sageworks-0.5.3/src/sageworks/core/transforms/data_loaders/light/
--rw-r--r--   0 briford    (501) staff       (20)      543 2024-03-28 17:23:43.000000 sageworks-0.5.3/src/sageworks/core/transforms/data_loaders/light/__init__.py
--rw-r--r--   0 briford    (501) staff       (20)     3011 2024-03-28 17:23:43.000000 sageworks-0.5.3/src/sageworks/core/transforms/data_loaders/light/csv_to_data_source.py
--rw-r--r--   0 briford    (501) staff       (20)     2927 2024-03-28 17:23:43.000000 sageworks-0.5.3/src/sageworks/core/transforms/data_loaders/light/json_to_data_source.py
--rw-r--r--   0 briford    (501) staff       (20)     4225 2024-03-28 17:23:43.000000 sageworks-0.5.3/src/sageworks/core/transforms/data_loaders/light/s3_to_data_source_light.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-01 17:30:52.059490 sageworks-0.5.3/src/sageworks/core/transforms/data_to_data/
--rw-r--r--   0 briford    (501) staff       (20)        0 2024-01-10 18:45:51.000000 sageworks-0.5.3/src/sageworks/core/transforms/data_to_data/__init__.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-01 17:30:52.059596 sageworks-0.5.3/src/sageworks/core/transforms/data_to_data/heavy/
--rw-r--r--   0 briford    (501) staff       (20)        0 2024-01-10 18:45:51.000000 sageworks-0.5.3/src/sageworks/core/transforms/data_to_data/heavy/__init__.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-01 17:30:52.059695 sageworks-0.5.3/src/sageworks/core/transforms/data_to_data/heavy/emr/
--rw-r--r--   0 briford    (501) staff       (20)       68 2024-01-10 18:45:51.000000 sageworks-0.5.3/src/sageworks/core/transforms/data_to_data/heavy/emr/Readme.md
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-01 17:30:52.060005 sageworks-0.5.3/src/sageworks/core/transforms/data_to_data/heavy/glue/
--rw-r--r--   0 briford    (501) staff       (20)       48 2024-01-10 18:45:51.000000 sageworks-0.5.3/src/sageworks/core/transforms/data_to_data/heavy/glue/Readme.md
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-01 17:30:52.060505 sageworks-0.5.3/src/sageworks/core/transforms/data_to_data/light/
--rw-r--r--   0 briford    (501) staff       (20)        0 2024-01-10 18:45:51.000000 sageworks-0.5.3/src/sageworks/core/transforms/data_to_data/light/__init__.py
--rw-r--r--   0 briford    (501) staff       (20)     2237 2024-03-27 20:40:53.000000 sageworks-0.5.3/src/sageworks/core/transforms/data_to_data/light/clean_data.py
--rw-r--r--   0 briford    (501) staff       (20)     2687 2024-03-27 20:40:53.000000 sageworks-0.5.3/src/sageworks/core/transforms/data_to_data/light/data_to_data_light.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-01 17:30:52.060626 sageworks-0.5.3/src/sageworks/core/transforms/data_to_features/
--rw-r--r--   0 briford    (501) staff       (20)        0 2024-01-10 18:45:51.000000 sageworks-0.5.3/src/sageworks/core/transforms/data_to_features/__init__.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-01 17:30:52.060726 sageworks-0.5.3/src/sageworks/core/transforms/data_to_features/heavy/
--rw-r--r--   0 briford    (501) staff       (20)        0 2024-01-10 18:45:51.000000 sageworks-0.5.3/src/sageworks/core/transforms/data_to_features/heavy/__init__.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-01 17:30:52.060934 sageworks-0.5.3/src/sageworks/core/transforms/data_to_features/heavy/chunk/
--rw-r--r--   0 briford    (501) staff       (20)        0 2024-01-10 18:45:51.000000 sageworks-0.5.3/src/sageworks/core/transforms/data_to_features/heavy/chunk/__init__.py
--rw-r--r--   0 briford    (501) staff       (20)     4551 2024-03-28 17:23:43.000000 sageworks-0.5.3/src/sageworks/core/transforms/data_to_features/heavy/chunk/data_to_features_chunk.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-01 17:30:52.061079 sageworks-0.5.3/src/sageworks/core/transforms/data_to_features/heavy/emr/
--rw-r--r--   0 briford    (501) staff       (20)       68 2024-01-10 18:45:51.000000 sageworks-0.5.3/src/sageworks/core/transforms/data_to_features/heavy/emr/Readme.md
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-01 17:30:52.061325 sageworks-0.5.3/src/sageworks/core/transforms/data_to_features/heavy/glue/
--rw-r--r--   0 briford    (501) staff       (20)       48 2024-01-10 18:45:51.000000 sageworks-0.5.3/src/sageworks/core/transforms/data_to_features/heavy/glue/Readme.md
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-01 17:30:52.061536 sageworks-0.5.3/src/sageworks/core/transforms/data_to_features/heavy/storage/
--rw-r--r--   0 briford    (501) staff       (20)     6702 2024-03-28 17:23:43.000000 sageworks-0.5.3/src/sageworks/core/transforms/data_to_features/heavy/storage/data_to_features_heavy_old.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-01 17:30:52.061923 sageworks-0.5.3/src/sageworks/core/transforms/data_to_features/light/
--rw-r--r--   0 briford    (501) staff       (20)        0 2024-01-10 18:45:51.000000 sageworks-0.5.3/src/sageworks/core/transforms/data_to_features/light/__init__.py
--rw-r--r--   0 briford    (501) staff       (20)     3827 2024-03-28 17:23:43.000000 sageworks-0.5.3/src/sageworks/core/transforms/data_to_features/light/data_to_features_light.py
--rw-r--r--   0 briford    (501) staff       (20)     4778 2024-03-28 17:23:43.000000 sageworks-0.5.3/src/sageworks/core/transforms/data_to_features/light/molecular_descriptors.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-01 17:30:52.062062 sageworks-0.5.3/src/sageworks/core/transforms/features_to_features/
--rw-r--r--   0 briford    (501) staff       (20)        0 2024-01-10 18:45:51.000000 sageworks-0.5.3/src/sageworks/core/transforms/features_to_features/__init__.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-01 17:30:51.994494 sageworks-0.5.3/src/sageworks/core/transforms/features_to_features/heavy/
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-01 17:30:52.062171 sageworks-0.5.3/src/sageworks/core/transforms/features_to_features/heavy/emr/
--rw-r--r--   0 briford    (501) staff       (20)       68 2024-01-10 18:45:51.000000 sageworks-0.5.3/src/sageworks/core/transforms/features_to_features/heavy/emr/Readme.md
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-01 17:30:52.062378 sageworks-0.5.3/src/sageworks/core/transforms/features_to_features/heavy/glue/
--rw-r--r--   0 briford    (501) staff       (20)       48 2024-01-10 18:45:51.000000 sageworks-0.5.3/src/sageworks/core/transforms/features_to_features/heavy/glue/Readme.md
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-01 17:30:52.062680 sageworks-0.5.3/src/sageworks/core/transforms/features_to_model/
--rw-r--r--   0 briford    (501) staff       (20)        0 2024-01-10 18:45:51.000000 sageworks-0.5.3/src/sageworks/core/transforms/features_to_model/__init__.py
--rw-r--r--   0 briford    (501) staff       (20)    13050 2024-03-28 17:23:43.000000 sageworks-0.5.3/src/sageworks/core/transforms/features_to_model/features_to_model.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-01 17:30:52.063102 sageworks-0.5.3/src/sageworks/core/transforms/features_to_model/light_model_harness/
--rw-r--r--   0 briford    (501) staff       (20)       19 2024-02-27 23:40:48.000000 sageworks-0.5.3/src/sageworks/core/transforms/features_to_model/light_model_harness/requirements.txt
--rw-r--r--   0 briford    (501) staff       (20)    10806 2024-03-28 17:23:43.000000 sageworks-0.5.3/src/sageworks/core/transforms/features_to_model/light_model_harness/xgb_model.template
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-01 17:30:52.063522 sageworks-0.5.3/src/sageworks/core/transforms/model_to_endpoint/
--rw-r--r--   0 briford    (501) staff       (20)        0 2024-01-10 18:45:51.000000 sageworks-0.5.3/src/sageworks/core/transforms/model_to_endpoint/__init__.py
--rw-r--r--   0 briford    (501) staff       (20)     8185 2024-03-28 17:23:43.000000 sageworks-0.5.3/src/sageworks/core/transforms/model_to_endpoint/model_to_endpoint.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-01 17:30:52.064341 sageworks-0.5.3/src/sageworks/core/transforms/pandas_transforms/
--rw-r--r--   0 briford    (501) staff       (20)      894 2024-03-28 17:23:43.000000 sageworks-0.5.3/src/sageworks/core/transforms/pandas_transforms/__init__.py
--rw-r--r--   0 briford    (501) staff       (20)     3615 2024-03-28 17:23:43.000000 sageworks-0.5.3/src/sageworks/core/transforms/pandas_transforms/data_to_pandas.py
--rw-r--r--   0 briford    (501) staff       (20)     3445 2024-03-28 17:23:43.000000 sageworks-0.5.3/src/sageworks/core/transforms/pandas_transforms/features_to_pandas.py
--rw-r--r--   0 briford    (501) staff       (20)     8604 2024-03-30 22:43:51.000000 sageworks-0.5.3/src/sageworks/core/transforms/pandas_transforms/pandas_to_data.py
--rw-r--r--   0 briford    (501) staff       (20)    18139 2024-03-30 22:43:51.000000 sageworks-0.5.3/src/sageworks/core/transforms/pandas_transforms/pandas_to_features.py
--rw-r--r--   0 briford    (501) staff       (20)     4440 2024-03-28 17:23:43.000000 sageworks-0.5.3/src/sageworks/core/transforms/pandas_transforms/pandas_to_features_chunked.py
--rw-r--r--   0 briford    (501) staff       (20)     5391 2024-03-28 17:23:43.000000 sageworks-0.5.3/src/sageworks/core/transforms/transform.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-01 17:30:52.064509 sageworks-0.5.3/src/sageworks/experiments/
--rw-r--r--   0 briford    (501) staff       (20)    10658 2024-03-28 17:23:43.000000 sageworks-0.5.3/src/sageworks/experiments/view_manager.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-01 17:30:52.064771 sageworks-0.5.3/src/sageworks/repl/
--rw-r--r--   0 briford    (501) staff       (20)        0 2024-01-10 18:45:51.000000 sageworks-0.5.3/src/sageworks/repl/__init__.py
--rw-r--r--   0 briford    (501) staff       (20)    14538 2024-03-30 22:43:51.000000 sageworks-0.5.3/src/sageworks/repl/sageworks_shell.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-01 17:30:52.065175 sageworks-0.5.3/src/sageworks/resources/
--rw-r--r--   0 briford    (501) staff       (20)      361 2024-01-23 15:36:53.000000 sageworks-0.5.3/src/sageworks/resources/open_source_api.key
--rw-r--r--   0 briford    (501) staff       (20)      272 2024-01-10 18:45:51.000000 sageworks-0.5.3/src/sageworks/resources/signature_verify_pub.pem
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-01 17:30:52.068982 sageworks-0.5.3/src/sageworks/utils/
--rw-r--r--   0 briford    (501) staff       (20)        0 2023-12-24 17:18:24.000000 sageworks-0.5.3/src/sageworks/utils/__init__.py
--rw-r--r--   0 briford    (501) staff       (20)    15587 2024-03-30 22:43:51.000000 sageworks-0.5.3/src/sageworks/utils/aws_utils.py
--rw-r--r--   0 briford    (501) staff       (20)     5455 2024-03-28 17:23:43.000000 sageworks-0.5.3/src/sageworks/utils/cache.py
--rw-r--r--   0 briford    (501) staff       (20)      722 2024-03-28 17:23:43.000000 sageworks-0.5.3/src/sageworks/utils/chem_utils.py
--rw-r--r--   0 briford    (501) staff       (20)    16234 2024-03-28 17:23:43.000000 sageworks-0.5.3/src/sageworks/utils/config_manager.py
--rw-r--r--   0 briford    (501) staff       (20)     7392 2024-03-28 17:23:43.000000 sageworks-0.5.3/src/sageworks/utils/dashboard_metrics.py
--rw-r--r--   0 briford    (501) staff       (20)     4194 2024-03-30 22:43:51.000000 sageworks-0.5.3/src/sageworks/utils/datetime_utils.py
--rw-r--r--   0 briford    (501) staff       (20)     5292 2024-03-28 17:23:43.000000 sageworks-0.5.3/src/sageworks/utils/df_to_endpoint.py
--rw-r--r--   0 briford    (501) staff       (20)     1681 2024-03-28 17:23:43.000000 sageworks-0.5.3/src/sageworks/utils/docker_utils.py
--rw-r--r--   0 briford    (501) staff       (20)     2866 2024-03-27 20:43:31.000000 sageworks-0.5.3/src/sageworks/utils/ecs_info.py
--rw-r--r--   0 briford    (501) staff       (20)     7657 2024-03-28 17:23:43.000000 sageworks-0.5.3/src/sageworks/utils/endpoint_metrics.py
--rw-r--r--   0 briford    (501) staff       (20)     3097 2024-03-28 17:23:43.000000 sageworks-0.5.3/src/sageworks/utils/endpoint_utils.py
--rw-r--r--   0 briford    (501) staff       (20)     6979 2024-03-28 17:23:43.000000 sageworks-0.5.3/src/sageworks/utils/extract_model_artifact.py
--rw-r--r--   0 briford    (501) staff       (20)     1131 2024-03-28 17:23:43.000000 sageworks-0.5.3/src/sageworks/utils/glue_utils.py
--rw-r--r--   0 briford    (501) staff       (20)     5757 2024-03-28 17:23:43.000000 sageworks-0.5.3/src/sageworks/utils/license_manager.py
--rw-r--r--   0 briford    (501) staff       (20)     1439 2024-03-28 17:32:59.000000 sageworks-0.5.3/src/sageworks/utils/markdown_utils.py
--rw-r--r--   0 briford    (501) staff       (20)    13241 2024-03-28 17:23:43.000000 sageworks-0.5.3/src/sageworks/utils/pandas_utils.py
--rw-r--r--   0 briford    (501) staff       (20)    11623 2024-03-28 17:23:43.000000 sageworks-0.5.3/src/sageworks/utils/plugin_manager.py
--rw-r--r--   0 briford    (501) staff       (20)     9533 2024-03-30 22:43:51.000000 sageworks-0.5.3/src/sageworks/utils/redis_cache.py
--rw-r--r--   0 briford    (501) staff       (20)     4166 2024-03-28 17:23:43.000000 sageworks-0.5.3/src/sageworks/utils/repl_utils.py
--rw-r--r--   0 briford    (501) staff       (20)     2089 2024-03-28 17:23:43.000000 sageworks-0.5.3/src/sageworks/utils/s3_utils.py
--rw-r--r--   0 briford    (501) staff       (20)     2163 2024-03-28 17:23:43.000000 sageworks-0.5.3/src/sageworks/utils/sageworks_cache.py
--rw-r--r--   0 briford    (501) staff       (20)     3474 2024-03-28 17:23:43.000000 sageworks-0.5.3/src/sageworks/utils/sageworks_event_bridge.py
--rw-r--r--   0 briford    (501) staff       (20)     5359 2024-03-28 17:23:43.000000 sageworks-0.5.3/src/sageworks/utils/sageworks_logging.py
--rw-r--r--   0 briford    (501) staff       (20)     2120 2024-03-28 17:23:43.000000 sageworks-0.5.3/src/sageworks/utils/sageworks_sqs.py
--rw-r--r--   0 briford    (501) staff       (20)     1108 2024-01-10 18:45:51.000000 sageworks-0.5.3/src/sageworks/utils/symbols.py
--rw-r--r--   0 briford    (501) staff       (20)     6414 2024-03-28 17:23:43.000000 sageworks-0.5.3/src/sageworks/utils/test_data_generator.py
--rw-r--r--   0 briford    (501) staff       (20)     2092 2024-03-27 20:43:31.000000 sageworks-0.5.3/src/sageworks/utils/trace_calls.py
--rw-r--r--   0 briford    (501) staff       (20)     1470 2024-03-28 17:23:43.000000 sageworks-0.5.3/src/sageworks/utils/type_abbrev.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-01 17:30:52.069886 sageworks-0.5.3/src/sageworks/views/
--rw-r--r--   0 briford    (501) staff       (20)     3318 2024-03-30 22:43:51.000000 sageworks-0.5.3/src/sageworks/views/artifacts_text_view.py
--rw-r--r--   0 briford    (501) staff       (20)     7008 2024-03-30 22:43:51.000000 sageworks-0.5.3/src/sageworks/views/artifacts_web_view.py
--rw-r--r--   0 briford    (501) staff       (20)     3158 2024-03-30 22:43:51.000000 sageworks-0.5.3/src/sageworks/views/data_source_web_view.py
--rw-r--r--   0 briford    (501) staff       (20)     2150 2024-03-30 22:43:51.000000 sageworks-0.5.3/src/sageworks/views/endpoint_web_view.py
--rw-r--r--   0 briford    (501) staff       (20)     3206 2024-03-30 22:43:51.000000 sageworks-0.5.3/src/sageworks/views/feature_set_web_view.py
--rw-r--r--   0 briford    (501) staff       (20)     2029 2024-03-30 22:43:51.000000 sageworks-0.5.3/src/sageworks/views/model_web_view.py
--rw-r--r--   0 briford    (501) staff       (20)     1092 2024-03-28 17:23:43.000000 sageworks-0.5.3/src/sageworks/views/view.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-01 17:30:52.071921 sageworks-0.5.3/src/sageworks/web_components/
--rw-r--r--   0 briford    (501) staff       (20)      837 2023-12-24 17:18:24.000000 sageworks-0.5.3/src/sageworks/web_components/color_maps.py
--rw-r--r--   0 briford    (501) staff       (20)     4902 2024-03-31 15:44:39.000000 sageworks-0.5.3/src/sageworks/web_components/component_interface.py
--rw-r--r--   0 briford    (501) staff       (20)     3521 2024-03-30 22:43:51.000000 sageworks-0.5.3/src/sageworks/web_components/confusion_matrix.py
--rw-r--r--   0 briford    (501) staff       (20)     5850 2024-03-30 22:43:51.000000 sageworks-0.5.3/src/sageworks/web_components/correlation_matrix.py
--rw-r--r--   0 briford    (501) staff       (20)     2970 2024-03-30 22:43:51.000000 sageworks-0.5.3/src/sageworks/web_components/dashboard_metric_plots.py
--rw-r--r--   0 briford    (501) staff       (20)     9335 2024-03-28 17:23:43.000000 sageworks-0.5.3/src/sageworks/web_components/data_details_markdown.py
--rw-r--r--   0 briford    (501) staff       (20)     4565 2024-03-28 17:35:30.000000 sageworks-0.5.3/src/sageworks/web_components/endpoint_details.py
--rw-r--r--   0 briford    (501) staff       (20)     3064 2024-03-30 22:43:51.000000 sageworks-0.5.3/src/sageworks/web_components/endpoint_metric_plots.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-01 17:30:52.072502 sageworks-0.5.3/src/sageworks/web_components/experiments/
--rw-r--r--   0 briford    (501) staff       (20)     1633 2024-03-28 17:23:43.000000 sageworks-0.5.3/src/sageworks/web_components/experiments/compound_details.py
--rw-r--r--   0 briford    (501) staff       (20)     1183 2024-03-28 17:23:43.000000 sageworks-0.5.3/src/sageworks/web_components/experiments/histogram.py
--rw-r--r--   0 briford    (501) staff       (20)     3680 2024-03-28 17:23:43.000000 sageworks-0.5.3/src/sageworks/web_components/experiments/outlier_plot.py
--rw-r--r--   0 briford    (501) staff       (20)     2279 2024-03-28 17:23:43.000000 sageworks-0.5.3/src/sageworks/web_components/experiments/scatter_plot.py
--rw-r--r--   0 briford    (501) staff       (20)      838 2024-03-28 17:23:43.000000 sageworks-0.5.3/src/sageworks/web_components/line_chart.py
--rw-r--r--   0 briford    (501) staff       (20)     8818 2024-04-01 17:28:51.000000 sageworks-0.5.3/src/sageworks/web_components/model_details.py
--rw-r--r--   0 briford    (501) staff       (20)     2270 2024-03-30 22:43:51.000000 sageworks-0.5.3/src/sageworks/web_components/model_plot.py
--rw-r--r--   0 briford    (501) staff       (20)     6713 2024-03-31 15:44:39.000000 sageworks-0.5.3/src/sageworks/web_components/plugin_interface.py
--rw-r--r--   0 briford    (501) staff       (20)     2941 2024-03-30 22:43:51.000000 sageworks-0.5.3/src/sageworks/web_components/regression_plot.py
--rw-r--r--   0 briford    (501) staff       (20)     6535 2024-03-28 17:23:43.000000 sageworks-0.5.3/src/sageworks/web_components/table.py
--rw-r--r--   0 briford    (501) staff       (20)     5181 2024-03-30 22:43:51.000000 sageworks-0.5.3/src/sageworks/web_components/violin_plots.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-01 17:30:52.076392 sageworks-0.5.3/src/sageworks.egg-info/
--rw-r--r--   0 briford    (501) staff       (20)     4118 2024-04-01 17:30:51.000000 sageworks-0.5.3/src/sageworks.egg-info/PKG-INFO
--rw-r--r--   0 briford    (501) staff       (20)    17057 2024-04-01 17:30:51.000000 sageworks-0.5.3/src/sageworks.egg-info/SOURCES.txt
--rw-r--r--   0 briford    (501) staff       (20)        1 2024-04-01 17:30:51.000000 sageworks-0.5.3/src/sageworks.egg-info/dependency_links.txt
--rw-r--r--   0 briford    (501) staff       (20)       74 2024-04-01 17:30:51.000000 sageworks-0.5.3/src/sageworks.egg-info/entry_points.txt
--rw-r--r--   0 briford    (501) staff       (20)      408 2024-04-01 17:30:51.000000 sageworks-0.5.3/src/sageworks.egg-info/requires.txt
--rw-r--r--   0 briford    (501) staff       (20)       10 2024-04-01 17:30:51.000000 sageworks-0.5.3/src/sageworks.egg-info/top_level.txt
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-01 17:30:52.073270 sageworks-0.5.3/tests/
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-01 17:30:52.073803 sageworks-0.5.3/tests/artifacts/
--rw-r--r--   0 briford    (501) staff       (20)     1548 2024-03-30 19:27:28.000000 sageworks-0.5.3/tests/artifacts/data_source_tests.py
--rw-r--r--   0 briford    (501) staff       (20)     2442 2024-03-28 17:23:43.000000 sageworks-0.5.3/tests/artifacts/endpoint_tests.py
--rw-r--r--   0 briford    (501) staff       (20)     1160 2024-03-28 17:23:43.000000 sageworks-0.5.3/tests/artifacts/feature_set_tests.py
--rw-r--r--   0 briford    (501) staff       (20)      805 2024-03-28 17:23:43.000000 sageworks-0.5.3/tests/artifacts/model_tests.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-01 17:30:52.074044 sageworks-0.5.3/tests/aws_account/
--rw-r--r--   0 briford    (501) staff       (20)      962 2023-12-24 17:18:24.000000 sageworks-0.5.3/tests/aws_account/aws_account_clamp_tests.py
--rw-r--r--   0 briford    (501) staff       (20)      642 2023-12-24 17:18:24.000000 sageworks-0.5.3/tests/aws_account/aws_service_broker_tests.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-01 17:30:52.074740 sageworks-0.5.3/tests/connectors/
--rw-r--r--   0 briford    (501) staff       (20)      725 2024-03-28 17:23:43.000000 sageworks-0.5.3/tests/connectors/data_catalog.py
--rw-r--r--   0 briford    (501) staff       (20)      737 2024-03-28 17:23:43.000000 sageworks-0.5.3/tests/connectors/endpoints.py
--rw-r--r--   0 briford    (501) staff       (20)      702 2024-03-28 17:23:43.000000 sageworks-0.5.3/tests/connectors/feature_store.py
--rw-r--r--   0 briford    (501) staff       (20)      644 2024-03-28 17:23:43.000000 sageworks-0.5.3/tests/connectors/glue_jobs.py
--rw-r--r--   0 briford    (501) staff       (20)      799 2024-03-28 17:23:43.000000 sageworks-0.5.3/tests/connectors/model_registry.py
--rw-r--r--   0 briford    (501) staff       (20)     1008 2024-03-28 17:23:43.000000 sageworks-0.5.3/tests/connectors/s3_bucket.py
--rw-r--r--   0 briford    (501) staff       (20)     5408 2024-03-28 17:23:43.000000 sageworks-0.5.3/tests/create_aqsol_artifacts.py
--rw-r--r--   0 briford    (501) staff       (20)     3217 2024-03-28 17:23:43.000000 sageworks-0.5.3/tests/create_basic_test_artifacts.py
--rw-r--r--   0 briford    (501) staff       (20)      870 2024-03-28 17:23:43.000000 sageworks-0.5.3/tests/create_realtime_endpoint.py
--rw-r--r--   0 briford    (501) staff       (20)     2379 2024-03-28 17:23:43.000000 sageworks-0.5.3/tests/create_training_adjusted_artifacts.py
--rw-r--r--   0 briford    (501) staff       (20)     2096 2024-03-28 17:23:43.000000 sageworks-0.5.3/tests/create_wine_artifacts.py
--rw-r--r--   0 briford    (501) staff       (20)     4310 2024-03-28 17:23:43.000000 sageworks-0.5.3/tests/delete_test_artifacts.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-01 17:30:52.074861 sageworks-0.5.3/tests/plugin_tests/
--rw-r--r--   0 briford    (501) staff       (20)     1888 2024-03-30 22:43:51.000000 sageworks-0.5.3/tests/plugin_tests/crashing_plugin.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-01 17:30:52.075095 sageworks-0.5.3/tests/specific/
--rw-r--r--   0 briford    (501) staff       (20)      639 2024-03-28 17:23:43.000000 sageworks-0.5.3/tests/specific/capital_tests.py
--rw-r--r--   0 briford    (501) staff       (20)     1513 2024-03-28 17:23:43.000000 sageworks-0.5.3/tests/specific/deletion_tests.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-01 17:30:52.075809 sageworks-0.5.3/tests/transforms/
--rw-r--r--   0 briford    (501) staff       (20)      592 2024-03-28 17:23:43.000000 sageworks-0.5.3/tests/transforms/data_to_data_tests.py
--rw-r--r--   0 briford    (501) staff       (20)     1025 2024-03-28 17:23:43.000000 sageworks-0.5.3/tests/transforms/data_to_features_tests.py
--rw-r--r--   0 briford    (501) staff       (20)      773 2024-03-28 17:23:43.000000 sageworks-0.5.3/tests/transforms/features_to_model_tests.py
--rw-r--r--   0 briford    (501) staff       (20)     4864 2024-03-28 17:23:43.000000 sageworks-0.5.3/tests/transforms/model_metrics_tests.py
--rw-r--r--   0 briford    (501) staff       (20)      795 2024-03-28 17:23:43.000000 sageworks-0.5.3/tests/transforms/model_to_endpoint_tests.py
--rw-r--r--   0 briford    (501) staff       (20)      633 2024-03-27 20:40:53.000000 sageworks-0.5.3/tests/transforms/pandas_to_data_tests.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-01 17:30:52.076165 sageworks-0.5.3/tests/web_components/
--rw-r--r--   0 briford    (501) staff       (20)      679 2024-03-30 22:43:51.000000 sageworks-0.5.3/tests/web_components/confusion_matrix_test.py
--rw-r--r--   0 briford    (501) staff       (20)      675 2024-03-30 22:43:51.000000 sageworks-0.5.3/tests/web_components/correlation_matrix_test.py
--rw-r--r--   0 briford    (501) staff       (20)     5210 2024-03-30 22:43:51.000000 sageworks-0.5.3/tests/web_components/plugin_interface_test.py
--rw-r--r--   0 briford    (501) staff       (20)     1115 2024-03-27 20:43:31.000000 sageworks-0.5.3/tox.ini
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-03 19:02:27.720978 sageworks-0.5.4/
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-03 19:02:27.665006 sageworks-0.5.4/.github/
+-rw-r--r--   0 briford    (501) staff       (20)     1338 2024-03-28 17:23:43.000000 sageworks-0.5.4/.github/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0 briford    (501) staff       (20)      499 2023-12-24 17:18:24.000000 sageworks-0.5.4/.github/dependabot.yml
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-03 19:02:27.665257 sageworks-0.5.4/.github/workflows/
+-rw-r--r--   0 briford    (501) staff       (20)      598 2024-01-10 18:45:51.000000 sageworks-0.5.4/.github/workflows/deploy-docs.yml
+-rw-r--r--   0 briford    (501) staff       (20)      556 2024-01-23 15:36:53.000000 sageworks-0.5.4/.github/workflows/python-lint.yml
+-rw-r--r--   0 briford    (501) staff       (20)     2008 2023-12-24 17:18:24.000000 sageworks-0.5.4/.gitignore
+-rw-r--r--   0 briford    (501) staff       (20)      444 2024-03-28 17:23:43.000000 sageworks-0.5.4/CONTRIBUTING.md
+-rw-r--r--   0 briford    (501) staff       (20)      102 2024-03-28 17:23:43.000000 sageworks-0.5.4/Dockerfile
+-rw-r--r--   0 briford    (501) staff       (20)     1080 2024-03-28 17:23:43.000000 sageworks-0.5.4/LICENSE
+-rw-r--r--   0 briford    (501) staff       (20)     1426 2023-12-24 17:18:24.000000 sageworks-0.5.4/Makefile
+-rw-r--r--   0 briford    (501) staff       (20)     4118 2024-04-03 19:02:27.720896 sageworks-0.5.4/PKG-INFO
+-rw-r--r--   0 briford    (501) staff       (20)     2695 2024-03-28 17:23:43.000000 sageworks-0.5.4/README.md
+-rw-r--r--   0 briford    (501) staff       (20)      463 2023-12-24 17:18:24.000000 sageworks-0.5.4/SECURITY.md
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-03 19:02:27.655807 sageworks-0.5.4/applications/
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-03 19:02:27.666406 sageworks-0.5.4/applications/aws_dashboard/
+-rw-r--r--   0 briford    (501) staff       (20)     1071 2024-04-02 13:06:54.000000 sageworks-0.5.4/applications/aws_dashboard/Dockerfile
+-rw-r--r--   0 briford    (501) staff       (20)      331 2024-03-28 17:23:43.000000 sageworks-0.5.4/applications/aws_dashboard/Dockerfile_plugins
+-rw-r--r--   0 briford    (501) staff       (20)      841 2024-01-10 18:45:51.000000 sageworks-0.5.4/applications/aws_dashboard/README.md
+-rw-r--r--   0 briford    (501) staff       (20)     1526 2024-04-02 16:53:34.000000 sageworks-0.5.4/applications/aws_dashboard/app.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-03 19:02:27.667116 sageworks-0.5.4/applications/aws_dashboard/assets/
+-rw-r--r--   0 briford    (501) staff       (20)   232839 2024-04-02 13:06:54.000000 sageworks-0.5.4/applications/aws_dashboard/assets/bootstrap_darkly.min.css
+-rw-r--r--   0 briford    (501) staff       (20)    14995 2024-04-02 13:06:54.000000 sageworks-0.5.4/applications/aws_dashboard/assets/default.css
+-rw-r--r--   0 briford    (501) staff       (20)      318 2023-12-24 17:18:24.000000 sageworks-0.5.4/applications/aws_dashboard/assets/favicon.ico
+-rw-r--r--   0 briford    (501) staff       (20)      732 2023-12-24 17:18:24.000000 sageworks-0.5.4/applications/aws_dashboard/assets/trash.png
+-rwxr-xr-x   0 briford    (501) staff       (20)      637 2024-04-02 15:05:11.000000 sageworks-0.5.4/applications/aws_dashboard/dashboard
+-rw-r--r--   0 briford    (501) staff       (20)      205 2023-12-24 17:18:24.000000 sageworks-0.5.4/applications/aws_dashboard/nginx.conf
+-rw-r--r--   0 briford    (501) staff       (20)      684 2024-03-28 17:23:43.000000 sageworks-0.5.4/applications/aws_dashboard/open_source_config.json
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-03 19:02:27.655732 sageworks-0.5.4/applications/aws_dashboard/pages/
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-03 19:02:27.667560 sageworks-0.5.4/applications/aws_dashboard/pages/data_sources/
+-rw-r--r--   0 briford    (501) staff       (20)    11696 2024-03-30 22:43:51.000000 sageworks-0.5.4/applications/aws_dashboard/pages/data_sources/callbacks.py
+-rw-r--r--   0 briford    (501) staff       (20)     2756 2024-03-28 17:23:43.000000 sageworks-0.5.4/applications/aws_dashboard/pages/data_sources/layout.py
+-rw-r--r--   0 briford    (501) staff       (20)     2555 2024-03-28 17:23:43.000000 sageworks-0.5.4/applications/aws_dashboard/pages/data_sources/page.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-03 19:02:27.667958 sageworks-0.5.4/applications/aws_dashboard/pages/endpoints/
+-rw-r--r--   0 briford    (501) staff       (20)     3975 2024-03-30 22:43:51.000000 sageworks-0.5.4/applications/aws_dashboard/pages/endpoints/callbacks.py
+-rw-r--r--   0 briford    (501) staff       (20)     2565 2024-03-28 17:23:43.000000 sageworks-0.5.4/applications/aws_dashboard/pages/endpoints/layout.py
+-rw-r--r--   0 briford    (501) staff       (20)     2465 2024-03-28 17:23:43.000000 sageworks-0.5.4/applications/aws_dashboard/pages/endpoints/page.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-03 19:02:27.668398 sageworks-0.5.4/applications/aws_dashboard/pages/feature_sets/
+-rw-r--r--   0 briford    (501) staff       (20)    11610 2024-03-30 22:43:51.000000 sageworks-0.5.4/applications/aws_dashboard/pages/feature_sets/callbacks.py
+-rw-r--r--   0 briford    (501) staff       (20)     2438 2024-03-28 17:23:43.000000 sageworks-0.5.4/applications/aws_dashboard/pages/feature_sets/layout.py
+-rw-r--r--   0 briford    (501) staff       (20)     2505 2024-03-28 17:23:43.000000 sageworks-0.5.4/applications/aws_dashboard/pages/feature_sets/page.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-03 19:02:27.668822 sageworks-0.5.4/applications/aws_dashboard/pages/main/
+-rw-r--r--   0 briford    (501) staff       (20)     4899 2024-03-30 22:43:51.000000 sageworks-0.5.4/applications/aws_dashboard/pages/main/callbacks.py
+-rw-r--r--   0 briford    (501) staff       (20)     2899 2024-03-28 17:23:43.000000 sageworks-0.5.4/applications/aws_dashboard/pages/main/layout.py
+-rw-r--r--   0 briford    (501) staff       (20)     1844 2024-03-28 17:23:43.000000 sageworks-0.5.4/applications/aws_dashboard/pages/main/page.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-03 19:02:27.669240 sageworks-0.5.4/applications/aws_dashboard/pages/models/
+-rw-r--r--   0 briford    (501) staff       (20)     3760 2024-04-03 18:28:10.000000 sageworks-0.5.4/applications/aws_dashboard/pages/models/callbacks.py
+-rw-r--r--   0 briford    (501) staff       (20)     2020 2024-03-28 17:23:43.000000 sageworks-0.5.4/applications/aws_dashboard/pages/models/layout.py
+-rw-r--r--   0 briford    (501) staff       (20)     2341 2024-03-28 17:23:43.000000 sageworks-0.5.4/applications/aws_dashboard/pages/models/page.py
+-rw-r--r--   0 briford    (501) staff       (20)      394 2024-04-02 13:06:54.000000 sageworks-0.5.4/applications/aws_dashboard/requirements.txt
+-rw-r--r--   0 briford    (501) staff       (20)      457 2023-12-24 17:18:24.000000 sageworks-0.5.4/applications/aws_dashboard/supervisord.conf
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-03 19:02:27.655867 sageworks-0.5.4/applications/experiments/
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-03 19:02:27.670057 sageworks-0.5.4/applications/experiments/compound_explorer/
+-rw-r--r--   0 briford    (501) staff       (20)      181 2023-12-24 17:18:24.000000 sageworks-0.5.4/applications/experiments/compound_explorer/Dockerfile
+-rw-r--r--   0 briford    (501) staff       (20)      360 2023-12-24 17:18:24.000000 sageworks-0.5.4/applications/experiments/compound_explorer/README.md
+-rw-r--r--   0 briford    (501) staff       (20)     3082 2024-04-02 16:53:34.000000 sageworks-0.5.4/applications/experiments/compound_explorer/app.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-03 19:02:27.670304 sageworks-0.5.4/applications/experiments/compound_explorer/assets/
+-rw-r--r--   0 briford    (501) staff       (20)    12861 2023-12-24 17:18:24.000000 sageworks-0.5.4/applications/experiments/compound_explorer/assets/custom.css
+-rw-r--r--   0 briford    (501) staff       (20)      318 2023-12-24 17:18:24.000000 sageworks-0.5.4/applications/experiments/compound_explorer/assets/favicon.ico
+-rw-r--r--   0 briford    (501) staff       (20)     7676 2024-03-30 22:43:51.000000 sageworks-0.5.4/applications/experiments/compound_explorer/callbacks.py
+-rw-r--r--   0 briford    (501) staff       (20)     4860 2024-03-28 17:23:43.000000 sageworks-0.5.4/applications/experiments/compound_explorer/layout.py
+-rw-r--r--   0 briford    (501) staff       (20)       94 2023-12-24 17:18:24.000000 sageworks-0.5.4/applications/experiments/compound_explorer/requirements.txt
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-03 19:02:27.670695 sageworks-0.5.4/aws_setup/
+-rw-r--r--   0 briford    (501) staff       (20)     3582 2024-03-28 17:23:43.000000 sageworks-0.5.4/aws_setup/aws_account_check.py
+-rw-r--r--   0 briford    (501) staff       (20)     1403 2024-03-28 17:23:43.000000 sageworks-0.5.4/aws_setup/aws_identity_check.py
+-rw-r--r--   0 briford    (501) staff       (20)     2629 2024-03-28 17:23:43.000000 sageworks-0.5.4/aws_setup/build_ml_pipeline.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-03 19:02:27.670820 sageworks-0.5.4/aws_setup/event_bridge/
+-rw-r--r--   0 briford    (501) staff       (20)       60 2023-12-24 17:18:24.000000 sageworks-0.5.4/aws_setup/event_bridge/Readme.md
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-03 19:02:27.671354 sageworks-0.5.4/aws_setup/event_bridge/dynamic_docker/
+-rw-r--r--   0 briford    (501) staff       (20)       60 2023-12-24 17:18:24.000000 sageworks-0.5.4/aws_setup/event_bridge/dynamic_docker/Readme.md
+-rw-r--r--   0 briford    (501) staff       (20)     1007 2023-12-24 17:18:24.000000 sageworks-0.5.4/aws_setup/event_bridge/dynamic_docker/app.py
+-rw-r--r--   0 briford    (501) staff       (20)     2567 2023-12-24 17:18:24.000000 sageworks-0.5.4/aws_setup/event_bridge/dynamic_docker/cdk.json
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-03 19:02:27.671484 sageworks-0.5.4/aws_setup/event_bridge/dynamic_docker/lambda/
+-rw-r--r--   0 briford    (501) staff       (20)     1812 2024-01-10 18:45:51.000000 sageworks-0.5.4/aws_setup/event_bridge/dynamic_docker/lambda/lambda_replace_task.py
+-rw-r--r--   0 briford    (501) staff       (20)     2599 2024-03-27 20:43:31.000000 sageworks-0.5.4/aws_setup/event_bridge/dynamic_docker/sageworks_image_update_stack.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-03 19:02:27.672386 sageworks-0.5.4/aws_setup/sageworks_core/
+-rw-r--r--   0 briford    (501) staff       (20)      119 2023-12-24 17:18:24.000000 sageworks-0.5.4/aws_setup/sageworks_core/.gitignore
+-rw-r--r--   0 briford    (501) staff       (20)     1028 2023-12-24 17:18:24.000000 sageworks-0.5.4/aws_setup/sageworks_core/README.md
+-rw-r--r--   0 briford    (501) staff       (20)     1403 2024-03-28 17:23:43.000000 sageworks-0.5.4/aws_setup/sageworks_core/app.py
+-rw-r--r--   0 briford    (501) staff       (20)     1998 2023-12-24 17:18:24.000000 sageworks-0.5.4/aws_setup/sageworks_core/cdk.json
+-rw-r--r--   0 briford    (501) staff       (20)       14 2023-12-24 17:18:24.000000 sageworks-0.5.4/aws_setup/sageworks_core/requirements-dev.txt
+-rw-r--r--   0 briford    (501) staff       (20)       53 2024-01-10 18:45:51.000000 sageworks-0.5.4/aws_setup/sageworks_core/requirements.txt
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-03 19:02:27.672609 sageworks-0.5.4/aws_setup/sageworks_core/sageworks_core/
+-rw-r--r--   0 briford    (501) staff       (20)        0 2024-01-10 18:45:51.000000 sageworks-0.5.4/aws_setup/sageworks_core/sageworks_core/__init__.py
+-rw-r--r--   0 briford    (501) staff       (20)    23575 2024-03-28 17:23:43.000000 sageworks-0.5.4/aws_setup/sageworks_core/sageworks_core/sageworks_core_stack.py
+-rw-r--r--   0 briford    (501) staff       (20)      437 2023-12-24 17:18:24.000000 sageworks-0.5.4/aws_setup/sageworks_core/source.bat
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-03 19:02:27.672758 sageworks-0.5.4/aws_setup/sageworks_core/tests/
+-rw-r--r--   0 briford    (501) staff       (20)        0 2023-12-24 17:18:24.000000 sageworks-0.5.4/aws_setup/sageworks_core/tests/__init__.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-03 19:02:27.672953 sageworks-0.5.4/aws_setup/sageworks_core/tests/unit/
+-rw-r--r--   0 briford    (501) staff       (20)        0 2023-12-24 17:18:24.000000 sageworks-0.5.4/aws_setup/sageworks_core/tests/unit/__init__.py
+-rw-r--r--   0 briford    (501) staff       (20)      720 2023-12-24 17:18:24.000000 sageworks-0.5.4/aws_setup/sageworks_core/tests/unit/test_sageworks_sandbox_stack.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-03 19:02:27.673884 sageworks-0.5.4/aws_setup/sageworks_dashboard_full/
+-rw-r--r--   0 briford    (501) staff       (20)      119 2023-12-24 17:18:24.000000 sageworks-0.5.4/aws_setup/sageworks_dashboard_full/.gitignore
+-rw-r--r--   0 briford    (501) staff       (20)     1778 2024-03-28 17:23:43.000000 sageworks-0.5.4/aws_setup/sageworks_dashboard_full/README.md
+-rw-r--r--   0 briford    (501) staff       (20)     1907 2024-03-28 17:23:43.000000 sageworks-0.5.4/aws_setup/sageworks_dashboard_full/app.py
+-rw-r--r--   0 briford    (501) staff       (20)     2567 2023-12-24 17:18:24.000000 sageworks-0.5.4/aws_setup/sageworks_dashboard_full/cdk.json
+-rw-r--r--   0 briford    (501) staff       (20)       14 2023-12-24 17:18:24.000000 sageworks-0.5.4/aws_setup/sageworks_dashboard_full/requirements-dev.txt
+-rw-r--r--   0 briford    (501) staff       (20)       47 2023-12-24 17:18:24.000000 sageworks-0.5.4/aws_setup/sageworks_dashboard_full/requirements.txt
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-03 19:02:27.674115 sageworks-0.5.4/aws_setup/sageworks_dashboard_full/sageworks_dashboard_full/
+-rw-r--r--   0 briford    (501) staff       (20)        0 2023-12-24 17:18:24.000000 sageworks-0.5.4/aws_setup/sageworks_dashboard_full/sageworks_dashboard_full/__init__.py
+-rw-r--r--   0 briford    (501) staff       (20)     7022 2024-04-02 13:06:54.000000 sageworks-0.5.4/aws_setup/sageworks_dashboard_full/sageworks_dashboard_full/sageworks_dashboard_stack.py
+-rw-r--r--   0 briford    (501) staff       (20)      437 2023-12-24 17:18:24.000000 sageworks-0.5.4/aws_setup/sageworks_dashboard_full/source.bat
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-03 19:02:27.674258 sageworks-0.5.4/aws_setup/sageworks_dashboard_full/tests/
+-rw-r--r--   0 briford    (501) staff       (20)        0 2023-12-24 17:18:24.000000 sageworks-0.5.4/aws_setup/sageworks_dashboard_full/tests/__init__.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-03 19:02:27.674452 sageworks-0.5.4/aws_setup/sageworks_dashboard_full/tests/unit/
+-rw-r--r--   0 briford    (501) staff       (20)        0 2023-12-24 17:18:24.000000 sageworks-0.5.4/aws_setup/sageworks_dashboard_full/tests/unit/__init__.py
+-rw-r--r--   0 briford    (501) staff       (20)      565 2023-12-24 17:18:24.000000 sageworks-0.5.4/aws_setup/sageworks_dashboard_full/tests/unit/test_sageworks_dashboard_stack.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-03 19:02:27.675075 sageworks-0.5.4/aws_setup/sageworks_dashboard_lite/
+-rw-r--r--   0 briford    (501) staff       (20)      119 2024-03-28 17:23:43.000000 sageworks-0.5.4/aws_setup/sageworks_dashboard_lite/.gitignore
+-rw-r--r--   0 briford    (501) staff       (20)     1778 2024-03-28 17:23:43.000000 sageworks-0.5.4/aws_setup/sageworks_dashboard_lite/README.md
+-rw-r--r--   0 briford    (501) staff       (20)     1928 2024-03-28 17:23:43.000000 sageworks-0.5.4/aws_setup/sageworks_dashboard_lite/app.py
+-rw-r--r--   0 briford    (501) staff       (20)     2567 2024-03-28 17:23:43.000000 sageworks-0.5.4/aws_setup/sageworks_dashboard_lite/cdk.json
+-rw-r--r--   0 briford    (501) staff       (20)       47 2024-03-28 17:23:43.000000 sageworks-0.5.4/aws_setup/sageworks_dashboard_lite/requirements.txt
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-03 19:02:27.675309 sageworks-0.5.4/aws_setup/sageworks_dashboard_lite/sageworks_dashboard_lite/
+-rw-r--r--   0 briford    (501) staff       (20)        0 2024-03-28 17:23:43.000000 sageworks-0.5.4/aws_setup/sageworks_dashboard_lite/sageworks_dashboard_lite/__init__.py
+-rw-r--r--   0 briford    (501) staff       (20)     6849 2024-04-02 13:06:54.000000 sageworks-0.5.4/aws_setup/sageworks_dashboard_lite/sageworks_dashboard_lite/sageworks_dashboard_stack.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-03 19:02:27.675970 sageworks-0.5.4/data/
+-rw-r--r--   0 briford    (501) staff       (20)   191978 2023-12-24 17:18:24.000000 sageworks-0.5.4/data/abalone.csv
+-rw-r--r--   0 briford    (501) staff       (20)     1515 2023-12-24 17:18:24.000000 sageworks-0.5.4/data/test_data.csv
+-rw-r--r--   0 briford    (501) staff       (20)     2270 2023-12-24 17:18:24.000000 sageworks-0.5.4/data/test_data.json
+-rw-r--r--   0 briford    (501) staff       (20)    12977 2024-01-10 18:45:51.000000 sageworks-0.5.4/data/wine_dataset.csv
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-03 19:02:27.676200 sageworks-0.5.4/docs/
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-03 19:02:27.676513 sageworks-0.5.4/docs/admin/
+-rw-r--r--   0 briford    (501) staff       (20)     1825 2024-03-28 17:23:43.000000 sageworks-0.5.4/docs/admin/docker_push.md
+-rw-r--r--   0 briford    (501) staff       (20)     1633 2024-01-10 18:45:51.000000 sageworks-0.5.4/docs/admin/pypi_release.md
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-03 19:02:27.677585 sageworks-0.5.4/docs/api_classes/
+-rw-r--r--   0 briford    (501) staff       (20)     3595 2024-01-23 15:36:53.000000 sageworks-0.5.4/docs/api_classes/data_source.md
+-rw-r--r--   0 briford    (501) staff       (20)     5199 2024-03-28 17:23:43.000000 sageworks-0.5.4/docs/api_classes/endpoint.md
+-rw-r--r--   0 briford    (501) staff       (20)     6299 2024-03-28 17:23:43.000000 sageworks-0.5.4/docs/api_classes/feature_set.md
+-rw-r--r--   0 briford    (501) staff       (20)     5350 2024-03-30 23:05:32.000000 sageworks-0.5.4/docs/api_classes/meta.md
+-rw-r--r--   0 briford    (501) staff       (20)     4356 2024-01-10 18:45:51.000000 sageworks-0.5.4/docs/api_classes/model.md
+-rw-r--r--   0 briford    (501) staff       (20)     2218 2024-01-10 18:45:51.000000 sageworks-0.5.4/docs/api_classes/monitor.md
+-rw-r--r--   0 briford    (501) staff       (20)     3549 2024-01-10 18:45:51.000000 sageworks-0.5.4/docs/api_classes/overview.md
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-03 19:02:27.678278 sageworks-0.5.4/docs/aws_setup/
+-rw-r--r--   0 briford    (501) staff       (20)     1121 2024-03-28 17:23:43.000000 sageworks-0.5.4/docs/aws_setup/aws_access_management.md
+-rw-r--r--   0 briford    (501) staff       (20)     7836 2024-01-23 15:36:53.000000 sageworks-0.5.4/docs/aws_setup/aws_tips_and_tricks.md
+-rw-r--r--   0 briford    (501) staff       (20)     4229 2024-03-28 17:23:43.000000 sageworks-0.5.4/docs/aws_setup/core_stack.md
+-rw-r--r--   0 briford    (501) staff       (20)     2075 2024-03-28 17:23:43.000000 sageworks-0.5.4/docs/aws_setup/dashboard_stack.md
+-rw-r--r--   0 briford    (501) staff       (20)     2540 2024-01-23 15:36:53.000000 sageworks-0.5.4/docs/aws_setup/full_pipeline.md
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-03 19:02:27.678409 sageworks-0.5.4/docs/concepts/
+-rw-r--r--   0 briford    (501) staff       (20)      907 2024-01-23 15:36:53.000000 sageworks-0.5.4/docs/concepts/model_monitoring.md
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-03 19:02:27.678538 sageworks-0.5.4/docs/core_classes/
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-03 19:02:27.679573 sageworks-0.5.4/docs/core_classes/artifacts/
+-rw-r--r--   0 briford    (501) staff       (20)      464 2024-01-23 15:36:53.000000 sageworks-0.5.4/docs/core_classes/artifacts/artifact.md
+-rw-r--r--   0 briford    (501) staff       (20)      290 2024-01-10 18:45:51.000000 sageworks-0.5.4/docs/core_classes/artifacts/athena_source.md
+-rw-r--r--   0 briford    (501) staff       (20)      479 2024-01-23 15:36:53.000000 sageworks-0.5.4/docs/core_classes/artifacts/data_source_abstract.md
+-rw-r--r--   0 briford    (501) staff       (20)      292 2024-01-10 18:45:51.000000 sageworks-0.5.4/docs/core_classes/artifacts/endpoint_core.md
+-rw-r--r--   0 briford    (501) staff       (20)      294 2024-01-10 18:45:51.000000 sageworks-0.5.4/docs/core_classes/artifacts/feature_set_core.md
+-rw-r--r--   0 briford    (501) staff       (20)      281 2024-01-10 18:45:51.000000 sageworks-0.5.4/docs/core_classes/artifacts/model_core.md
+-rw-r--r--   0 briford    (501) staff       (20)      289 2024-01-10 18:45:51.000000 sageworks-0.5.4/docs/core_classes/artifacts/monitor_core.md
+-rw-r--r--   0 briford    (501) staff       (20)      861 2024-01-10 18:45:51.000000 sageworks-0.5.4/docs/core_classes/artifacts/overview.md
+-rw-r--r--   0 briford    (501) staff       (20)     2119 2024-01-10 18:45:51.000000 sageworks-0.5.4/docs/core_classes/overview.md
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-03 19:02:27.680637 sageworks-0.5.4/docs/core_classes/transforms/
+-rw-r--r--   0 briford    (501) staff       (20)      352 2024-01-10 18:45:51.000000 sageworks-0.5.4/docs/core_classes/transforms/data_loaders_heavy.md
+-rw-r--r--   0 briford    (501) staff       (20)      396 2024-01-10 18:45:51.000000 sageworks-0.5.4/docs/core_classes/transforms/data_loaders_light.md
+-rw-r--r--   0 briford    (501) staff       (20)      349 2024-03-28 17:23:43.000000 sageworks-0.5.4/docs/core_classes/transforms/data_to_features.md
+-rw-r--r--   0 briford    (501) staff       (20)      265 2024-01-10 18:45:51.000000 sageworks-0.5.4/docs/core_classes/transforms/features_to_model.md
+-rw-r--r--   0 briford    (501) staff       (20)      264 2024-01-10 18:45:51.000000 sageworks-0.5.4/docs/core_classes/transforms/model_to_endpoint.md
+-rw-r--r--   0 briford    (501) staff       (20)     1177 2024-01-10 18:45:51.000000 sageworks-0.5.4/docs/core_classes/transforms/overview.md
+-rw-r--r--   0 briford    (501) staff       (20)      970 2024-01-23 15:36:53.000000 sageworks-0.5.4/docs/core_classes/transforms/pandas_transforms.md
+-rw-r--r--   0 briford    (501) staff       (20)      521 2024-01-23 15:36:53.000000 sageworks-0.5.4/docs/core_classes/transforms/transform.md
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-03 19:02:27.680781 sageworks-0.5.4/docs/glue/
+-rw-r--r--   0 briford    (501) staff       (20)     4837 2024-03-28 17:23:43.000000 sageworks-0.5.4/docs/glue/index.md
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-03 19:02:27.683011 sageworks-0.5.4/docs/images/
+-rw-r--r--   0 briford    (501) staff       (20)   605827 2023-12-24 17:18:24.000000 sageworks-0.5.4/docs/images/big_spider.png
+-rw-r--r--   0 briford    (501) staff       (20)    32320 2023-12-24 17:18:24.000000 sageworks-0.5.4/docs/images/graph_representation.png
+-rw-r--r--   0 briford    (501) staff       (20)    15549 2023-12-24 17:18:24.000000 sageworks-0.5.4/docs/images/powered_aws_dark_blue.png
+-rw-r--r--   0 briford    (501) staff       (20)    10003 2023-12-24 17:18:24.000000 sageworks-0.5.4/docs/images/powered_aws_transparent.png
+-rw-r--r--   0 briford    (501) staff       (20)     6435 2023-12-24 17:18:24.000000 sageworks-0.5.4/docs/images/powered_aws_white.png
+-rw-r--r--   0 briford    (501) staff       (20)    21174 2023-12-24 17:18:24.000000 sageworks-0.5.4/docs/images/powered_aws_with_tm_grey.png
+-rw-r--r--   0 briford    (501) staff       (20)    51137 2023-12-24 17:18:24.000000 sageworks-0.5.4/docs/images/sageworks.png
+-rw-r--r--   0 briford    (501) staff       (20)   489672 2023-12-24 17:18:24.000000 sageworks-0.5.4/docs/images/sageworks_concepts.png
+-rw-r--r--   0 briford    (501) staff       (20)    30017 2023-12-24 17:18:24.000000 sageworks-0.5.4/docs/images/scp.png
+-rw-r--r--   0 briford    (501) staff       (20)   139307 2023-12-24 17:18:24.000000 sageworks-0.5.4/docs/images/scp_labs.png
+-rw-r--r--   0 briford    (501) staff       (20)   381209 2023-12-24 17:18:24.000000 sageworks-0.5.4/docs/images/small_spider.png
+-rw-r--r--   0 briford    (501) staff       (20)     3417 2024-03-28 17:23:43.000000 sageworks-0.5.4/docs/index.md
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-03 19:02:27.683704 sageworks-0.5.4/docs/misc/
+-rw-r--r--   0 briford    (501) staff       (20)     2791 2024-03-28 17:23:43.000000 sageworks-0.5.4/docs/misc/faq.md
+-rw-r--r--   0 briford    (501) staff       (20)     5069 2024-01-10 18:45:51.000000 sageworks-0.5.4/docs/misc/general_info.md
+-rw-r--r--   0 briford    (501) staff       (20)      667 2024-01-10 18:45:51.000000 sageworks-0.5.4/docs/misc/sageworks_classes_concepts.md
+-rw-r--r--   0 briford    (501) staff       (20)     1873 2024-01-10 18:45:51.000000 sageworks-0.5.4/docs/misc/scp_consulting.md
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-03 19:02:27.683967 sageworks-0.5.4/docs/plugins/
+-rw-r--r--   0 briford    (501) staff       (20)     3221 2024-04-03 13:42:22.000000 sageworks-0.5.4/docs/plugins/index.md
+-rw-r--r--   0 briford    (501) staff       (20)      750 2024-03-31 15:49:43.000000 sageworks-0.5.4/docs/plugins/plugin_api_changes.md
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-03 19:02:27.684091 sageworks-0.5.4/docs/repl/
+-rw-r--r--   0 briford    (501) staff       (20)     2081 2024-03-28 17:23:43.000000 sageworks-0.5.4/docs/repl/index.md
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-03 19:02:27.684337 sageworks-0.5.4/docs/research/
+-rw-r--r--   0 briford    (501) staff       (20)      912 2024-03-28 17:23:43.000000 sageworks-0.5.4/docs/research/eda.md
+-rw-r--r--   0 briford    (501) staff       (20)     2017 2024-03-28 17:23:43.000000 sageworks-0.5.4/docs/research/htg.md
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-03 19:02:27.687286 sageworks-0.5.4/examples/
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-03 19:02:27.687422 sageworks-0.5.4/examples/ag-grid/
+-rw-r--r--   0 briford    (501) staff       (20)      496 2024-04-02 13:06:54.000000 sageworks-0.5.4/examples/ag-grid/hello_world.py
+-rw-r--r--   0 briford    (501) staff       (20)      326 2024-01-10 18:45:51.000000 sageworks-0.5.4/examples/datasource_from_df.py
+-rw-r--r--   0 briford    (501) staff       (20)      332 2024-01-10 18:45:51.000000 sageworks-0.5.4/examples/datasource_from_s3.py
+-rw-r--r--   0 briford    (501) staff       (20)      536 2024-01-23 15:36:53.000000 sageworks-0.5.4/examples/datasource_query.py
+-rw-r--r--   0 briford    (501) staff       (20)      680 2024-01-23 15:36:53.000000 sageworks-0.5.4/examples/datasource_stats.py
+-rw-r--r--   0 briford    (501) staff       (20)      223 2024-01-10 18:45:51.000000 sageworks-0.5.4/examples/datasource_to_featureset.py
+-rw-r--r--   0 briford    (501) staff       (20)      199 2024-01-10 18:45:51.000000 sageworks-0.5.4/examples/endpoint_details.py
+-rw-r--r--   0 briford    (501) staff       (20)      834 2024-03-28 17:23:43.000000 sageworks-0.5.4/examples/endpoint_inference.py
+-rw-r--r--   0 briford    (501) staff       (20)      481 2024-01-10 18:45:51.000000 sageworks-0.5.4/examples/endpoint_metrics.py
+-rw-r--r--   0 briford    (501) staff       (20)      744 2024-01-10 18:45:51.000000 sageworks-0.5.4/examples/featureset_eda.py
+-rw-r--r--   0 briford    (501) staff       (20)      560 2024-03-28 17:23:43.000000 sageworks-0.5.4/examples/featureset_query.py
+-rw-r--r--   0 briford    (501) staff       (20)      421 2024-03-27 20:32:26.000000 sageworks-0.5.4/examples/featureset_to_model.py
+-rw-r--r--   0 briford    (501) staff       (20)     1534 2024-03-28 17:23:43.000000 sageworks-0.5.4/examples/full_ml_pipeline.py
+-rw-r--r--   0 briford    (501) staff       (20)      580 2024-01-23 15:36:53.000000 sageworks-0.5.4/examples/glue_hello_world.py
+-rw-r--r--   0 briford    (501) staff       (20)      942 2024-01-23 15:36:53.000000 sageworks-0.5.4/examples/glue_hello_world_with_log.py
+-rw-r--r--   0 briford    (501) staff       (20)      686 2024-01-23 15:36:53.000000 sageworks-0.5.4/examples/glue_load_s3_bucket.py
+-rw-r--r--   0 briford    (501) staff       (20)      363 2024-03-30 22:43:51.000000 sageworks-0.5.4/examples/meta_list_endpoints.py
+-rw-r--r--   0 briford    (501) staff       (20)      328 2024-03-30 22:43:51.000000 sageworks-0.5.4/examples/meta_list_models.py
+-rw-r--r--   0 briford    (501) staff       (20)      659 2024-03-30 22:43:51.000000 sageworks-0.5.4/examples/meta_model_metrics.py
+-rw-r--r--   0 briford    (501) staff       (20)      548 2024-03-28 17:23:43.000000 sageworks-0.5.4/examples/model_metrics.py
+-rw-r--r--   0 briford    (501) staff       (20)      312 2024-03-27 20:32:26.000000 sageworks-0.5.4/examples/model_to_endpoint.py
+-rw-r--r--   0 briford    (501) staff       (20)      400 2024-01-10 18:45:51.000000 sageworks-0.5.4/examples/monitor_setup.py
+-rw-r--r--   0 briford    (501) staff       (20)      765 2024-01-10 18:45:51.000000 sageworks-0.5.4/examples/monitor_usage.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-03 19:02:27.658584 sageworks-0.5.4/examples/plugins/
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-03 19:02:27.687948 sageworks-0.5.4/examples/plugins/pages/
+-rw-r--r--   0 briford    (501) staff       (20)     2467 2024-04-02 16:53:34.000000 sageworks-0.5.4/examples/plugins/pages/my_plugin_page.py
+-rw-r--r--   0 briford    (501) staff       (20)     1621 2024-04-02 17:39:18.000000 sageworks-0.5.4/examples/plugins/pages/plugin_page_1.py
+-rw-r--r--   0 briford    (501) staff       (20)     2461 2024-04-02 17:39:30.000000 sageworks-0.5.4/examples/plugins/pages/plugin_page_2.py
+-rw-r--r--   0 briford    (501) staff       (20)     4473 2024-04-02 17:39:18.000000 sageworks-0.5.4/examples/plugins/pages/plugin_page_3.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-03 19:02:27.688212 sageworks-0.5.4/examples/plugins/views/
+-rw-r--r--   0 briford    (501) staff       (20)     1588 2024-04-02 13:46:33.000000 sageworks-0.5.4/examples/plugins/views/model_plugin_view.py
+-rw-r--r--   0 briford    (501) staff       (20)     1264 2024-04-02 13:06:54.000000 sageworks-0.5.4/examples/plugins/views/my_view_plugin.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-03 19:02:27.688763 sageworks-0.5.4/examples/plugins/web_components/
+-rw-r--r--   0 briford    (501) staff       (20)     1576 2024-04-02 13:46:33.000000 sageworks-0.5.4/examples/plugins/web_components/custom_plugin.py
+-rw-r--r--   0 briford    (501) staff       (20)     1666 2024-04-02 13:06:54.000000 sageworks-0.5.4/examples/plugins/web_components/endpoint_plugin.py
+-rw-r--r--   0 briford    (501) staff       (20)     3600 2024-04-02 13:46:33.000000 sageworks-0.5.4/examples/plugins/web_components/endpoint_turbo.py
+-rw-r--r--   0 briford    (501) staff       (20)     1942 2024-04-02 13:06:54.000000 sageworks-0.5.4/examples/plugins/web_components/model_plugin.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-03 19:02:27.689207 sageworks-0.5.4/examples/sagemaker_pipelines/
+-rw-r--r--   0 briford    (501) staff       (20)      854 2024-03-28 17:23:43.000000 sageworks-0.5.4/examples/sagemaker_pipelines/all_steps.py
+-rw-r--r--   0 briford    (501) staff       (20)       40 2024-03-28 17:23:43.000000 sageworks-0.5.4/examples/sagemaker_pipelines/hello.py
+-rw-r--r--   0 briford    (501) staff       (20)     1487 2024-03-28 17:23:43.000000 sageworks-0.5.4/examples/sagemaker_pipelines/ml_pipeline.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-03 19:02:27.658797 sageworks-0.5.4/examples/sagemaker_pipelines/storage/
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-03 19:02:27.689986 sageworks-0.5.4/examples/sagemaker_pipelines/storage/full_pipeline_experiment/
+-rw-r--r--   0 briford    (501) staff       (20)      854 2024-03-28 17:23:43.000000 sageworks-0.5.4/examples/sagemaker_pipelines/storage/full_pipeline_experiment/data_source.py
+-rw-r--r--   0 briford    (501) staff       (20)      203 2024-03-28 17:23:43.000000 sageworks-0.5.4/examples/sagemaker_pipelines/storage/full_pipeline_experiment/endpoint.py
+-rw-r--r--   0 briford    (501) staff       (20)      160 2024-03-28 17:23:43.000000 sageworks-0.5.4/examples/sagemaker_pipelines/storage/full_pipeline_experiment/feature_set.py
+-rw-r--r--   0 briford    (501) staff       (20)     1599 2024-03-28 17:23:43.000000 sageworks-0.5.4/examples/sagemaker_pipelines/storage/full_pipeline_experiment/ml_pipeline.py
+-rw-r--r--   0 briford    (501) staff       (20)      367 2024-03-28 17:23:43.000000 sageworks-0.5.4/examples/sagemaker_pipelines/storage/full_pipeline_experiment/model.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-03 19:02:27.690804 sageworks-0.5.4/examples/storage/
+-rw-r--r--   0 briford    (501) staff       (20)     1222 2024-03-27 20:40:53.000000 sageworks-0.5.4/examples/storage/data_to_data.py
+-rw-r--r--   0 briford    (501) staff       (20)      856 2024-03-27 20:40:53.000000 sageworks-0.5.4/examples/storage/data_to_features.py
+-rw-r--r--   0 briford    (501) staff       (20)     1371 2024-03-28 17:23:43.000000 sageworks-0.5.4/examples/storage/endpoint_inference.py
+-rw-r--r--   0 briford    (501) staff       (20)     1847 2024-03-28 17:23:43.000000 sageworks-0.5.4/examples/storage/hello_world_pipeline.py
+-rw-r--r--   0 briford    (501) staff       (20)     4378 2024-04-02 13:06:34.000000 sageworks-0.5.4/examples/storage/plugin_page_example.py
+-rw-r--r--   0 briford    (501) staff       (20)     2750 2024-03-31 15:47:34.000000 sageworks-0.5.4/mkdocs.yml
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-03 19:02:27.691312 sageworks-0.5.4/notebooks/
+-rw-r--r--   0 briford    (501) staff       (20)   185443 2024-03-28 17:23:43.000000 sageworks-0.5.4/notebooks/ML_Pipeline_with_SageWorks.ipynb
+-rw-r--r--   0 briford    (501) staff       (20)    36405 2024-03-28 17:23:43.000000 sageworks-0.5.4/notebooks/ML_Pipeline_with_SageWorks_2.ipynb
+-rw-r--r--   0 briford    (501) staff       (20)   511134 2024-03-28 17:23:43.000000 sageworks-0.5.4/notebooks/Outliers_in_SageWorks.ipynb
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-03 19:02:27.692865 sageworks-0.5.4/notebooks/images/
+-rw-r--r--   0 briford    (501) staff       (20)   142099 2023-12-24 17:18:24.000000 sageworks-0.5.4/notebooks/images/athena_query_aqsol.png
+-rw-r--r--   0 briford    (501) staff       (20)   191022 2023-12-24 17:18:24.000000 sageworks-0.5.4/notebooks/images/aws_dashboard_aqsol.png
+-rw-r--r--   0 briford    (501) staff       (20)   222686 2023-12-24 17:18:24.000000 sageworks-0.5.4/notebooks/images/dashboard_aqsol_features.png
+-rw-r--r--   0 briford    (501) staff       (20)   171441 2023-12-24 17:18:24.000000 sageworks-0.5.4/notebooks/images/model_screenshot.png
+-rw-r--r--   0 briford    (501) staff       (20)   489672 2023-12-24 17:18:24.000000 sageworks-0.5.4/notebooks/images/sageworks_concepts.png
+-rw-r--r--   0 briford    (501) staff       (20)   139307 2023-12-24 17:18:24.000000 sageworks-0.5.4/notebooks/images/scp_labs.png
+-rw-r--r--   0 briford    (501) staff       (20)      431 2024-04-02 13:06:54.000000 sageworks-0.5.4/requirements.txt
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-03 19:02:27.693960 sageworks-0.5.4/scripts/
+-rw-r--r--   0 briford    (501) staff       (20)     2290 2024-03-28 17:23:43.000000 sageworks-0.5.4/scripts/athena_ddl_mixed_case.py
+-rw-r--r--   0 briford    (501) staff       (20)     2178 2024-03-27 20:32:26.000000 sageworks-0.5.4/scripts/copy_data_catalog_db.py
+-rw-r--r--   0 briford    (501) staff       (20)      706 2024-01-10 18:45:51.000000 sageworks-0.5.4/scripts/delete_redis_keys.py
+-rw-r--r--   0 briford    (501) staff       (20)     1761 2024-03-28 17:23:43.000000 sageworks-0.5.4/scripts/glue_mixed_case.py
+-rw-r--r--   0 briford    (501) staff       (20)     5544 2024-03-28 17:23:43.000000 sageworks-0.5.4/scripts/model_endpoint_sanity_check.py
+-rw-r--r--   0 briford    (501) staff       (20)      715 2024-03-28 17:23:43.000000 sageworks-0.5.4/scripts/onboard_endpoints.py
+-rw-r--r--   0 briford    (501) staff       (20)      694 2024-03-28 17:23:43.000000 sageworks-0.5.4/scripts/onboard_models.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-03 19:02:27.694299 sageworks-0.5.4/scripts/storage/
+-rw-r--r--   0 briford    (501) staff       (20)     1003 2024-03-27 20:32:27.000000 sageworks-0.5.4/scripts/storage/dns_data_to_features.py
+-rw-r--r--   0 briford    (501) staff       (20)     1723 2024-03-30 22:43:51.000000 sageworks-0.5.4/scripts/storage/generate_jsonl_data.py
+-rw-r--r--   0 briford    (501) staff       (20)      955 2024-03-28 17:23:43.000000 sageworks-0.5.4/scripts/test_feature_resolution.py
+-rw-r--r--   0 briford    (501) staff       (20)      533 2024-04-03 19:02:27.721338 sageworks-0.5.4/setup.cfg
+-rw-r--r--   0 briford    (501) staff       (20)     1663 2024-03-27 20:32:27.000000 sageworks-0.5.4/setup.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-03 19:02:27.659354 sageworks-0.5.4/src/
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-03 19:02:27.694447 sageworks-0.5.4/src/sageworks/
+-rw-r--r--   0 briford    (501) staff       (20)     1091 2024-01-10 18:45:51.000000 sageworks-0.5.4/src/sageworks/__init__.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-03 19:02:27.695744 sageworks-0.5.4/src/sageworks/algorithms/
+-rw-r--r--   0 briford    (501) staff       (20)        0 2023-12-24 17:18:24.000000 sageworks-0.5.4/src/sageworks/algorithms/__init__.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-03 19:02:27.696700 sageworks-0.5.4/src/sageworks/algorithms/dataframe/
+-rw-r--r--   0 briford    (501) staff       (20)      378 2023-12-24 17:18:24.000000 sageworks-0.5.4/src/sageworks/algorithms/dataframe/Readme.md
+-rw-r--r--   0 briford    (501) staff       (20)     2852 2024-03-28 17:23:43.000000 sageworks-0.5.4/src/sageworks/algorithms/dataframe/aggregation.py
+-rw-r--r--   0 briford    (501) staff       (20)     1606 2024-03-28 17:23:43.000000 sageworks-0.5.4/src/sageworks/algorithms/dataframe/data_source_eda.py
+-rw-r--r--   0 briford    (501) staff       (20)     5388 2024-03-28 17:23:43.000000 sageworks-0.5.4/src/sageworks/algorithms/dataframe/dimensionality_reduction.py
+-rw-r--r--   0 briford    (501) staff       (20)     9406 2024-03-28 17:23:43.000000 sageworks-0.5.4/src/sageworks/algorithms/dataframe/feature_resolution.py
+-rw-r--r--   0 briford    (501) staff       (20)    12309 2024-03-28 17:23:43.000000 sageworks-0.5.4/src/sageworks/algorithms/dataframe/feature_spider.py
+-rw-r--r--   0 briford    (501) staff       (20)     4968 2024-03-28 17:23:43.000000 sageworks-0.5.4/src/sageworks/algorithms/dataframe/row_tagger.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-03 19:02:27.659713 sageworks-0.5.4/src/sageworks/algorithms/graph/
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-03 19:02:27.696845 sageworks-0.5.4/src/sageworks/algorithms/graph/heavy/
+-rw-r--r--   0 briford    (501) staff       (20)       96 2023-12-24 17:18:24.000000 sageworks-0.5.4/src/sageworks/algorithms/graph/heavy/Readme.md
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-03 19:02:27.696974 sageworks-0.5.4/src/sageworks/algorithms/graph/light/
+-rw-r--r--   0 briford    (501) staff       (20)      122 2023-12-24 17:18:24.000000 sageworks-0.5.4/src/sageworks/algorithms/graph/light/Readme.md
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-03 19:02:27.697097 sageworks-0.5.4/src/sageworks/algorithms/spark/
+-rw-r--r--   0 briford    (501) staff       (20)      615 2023-12-24 17:18:24.000000 sageworks-0.5.4/src/sageworks/algorithms/spark/Readme.md
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-03 19:02:27.698141 sageworks-0.5.4/src/sageworks/algorithms/sql/
+-rw-r--r--   0 briford    (501) staff       (20)      685 2023-12-24 17:18:24.000000 sageworks-0.5.4/src/sageworks/algorithms/sql/Readme.md
+-rw-r--r--   0 briford    (501) staff       (20)     6192 2024-03-28 17:23:43.000000 sageworks-0.5.4/src/sageworks/algorithms/sql/column_stats.py
+-rw-r--r--   0 briford    (501) staff       (20)     3645 2024-03-28 17:23:43.000000 sageworks-0.5.4/src/sageworks/algorithms/sql/correlations.py
+-rw-r--r--   0 briford    (501) staff       (20)     3622 2024-03-28 17:23:43.000000 sageworks-0.5.4/src/sageworks/algorithms/sql/descriptive_stats.py
+-rw-r--r--   0 briford    (501) staff       (20)    10174 2024-03-28 17:23:43.000000 sageworks-0.5.4/src/sageworks/algorithms/sql/outliers.py
+-rw-r--r--   0 briford    (501) staff       (20)     2352 2024-03-28 17:23:43.000000 sageworks-0.5.4/src/sageworks/algorithms/sql/sample_rows.py
+-rw-r--r--   0 briford    (501) staff       (20)     3437 2024-03-28 17:23:43.000000 sageworks-0.5.4/src/sageworks/algorithms/sql/value_counts.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-03 19:02:27.699053 sageworks-0.5.4/src/sageworks/api/
+-rw-r--r--   0 briford    (501) staff       (20)      708 2024-03-30 22:43:51.000000 sageworks-0.5.4/src/sageworks/api/__init__.py
+-rw-r--r--   0 briford    (501) staff       (20)     7811 2024-03-28 17:23:43.000000 sageworks-0.5.4/src/sageworks/api/data_source.py
+-rw-r--r--   0 briford    (501) staff       (20)     2505 2024-03-28 17:23:43.000000 sageworks-0.5.4/src/sageworks/api/endpoint.py
+-rw-r--r--   0 briford    (501) staff       (20)     4242 2024-03-28 17:23:43.000000 sageworks-0.5.4/src/sageworks/api/feature_set.py
+-rw-r--r--   0 briford    (501) staff       (20)    15642 2024-03-30 22:43:51.000000 sageworks-0.5.4/src/sageworks/api/meta.py
+-rw-r--r--   0 briford    (501) staff       (20)     2577 2024-03-28 17:23:43.000000 sageworks-0.5.4/src/sageworks/api/model.py
+-rw-r--r--   0 briford    (501) staff       (20)     5261 2024-03-28 17:23:43.000000 sageworks-0.5.4/src/sageworks/api/monitor.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-03 19:02:27.699349 sageworks-0.5.4/src/sageworks/aws_service_broker/
+-rw-r--r--   0 briford    (501) staff       (20)     9393 2024-03-28 17:23:43.000000 sageworks-0.5.4/src/sageworks/aws_service_broker/aws_account_clamp.py
+-rw-r--r--   0 briford    (501) staff       (20)    10908 2024-03-30 22:43:51.000000 sageworks-0.5.4/src/sageworks/aws_service_broker/aws_service_broker.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-03 19:02:27.700396 sageworks-0.5.4/src/sageworks/aws_service_broker/aws_service_connectors/
+-rw-r--r--   0 briford    (501) staff       (20)        0 2023-12-24 17:18:24.000000 sageworks-0.5.4/src/sageworks/aws_service_broker/aws_service_connectors/__init__.py
+-rw-r--r--   0 briford    (501) staff       (20)     1834 2024-03-28 17:23:43.000000 sageworks-0.5.4/src/sageworks/aws_service_broker/aws_service_connectors/connector.py
+-rw-r--r--   0 briford    (501) staff       (20)     3258 2024-03-28 17:23:43.000000 sageworks-0.5.4/src/sageworks/aws_service_broker/aws_service_connectors/data_catalog.py
+-rw-r--r--   0 briford    (501) staff       (20)     4055 2024-03-28 17:23:43.000000 sageworks-0.5.4/src/sageworks/aws_service_broker/aws_service_connectors/endpoints.py
+-rw-r--r--   0 briford    (501) staff       (20)     5238 2024-03-28 17:23:43.000000 sageworks-0.5.4/src/sageworks/aws_service_broker/aws_service_connectors/feature_store.py
+-rw-r--r--   0 briford    (501) staff       (20)     3712 2024-03-28 17:23:43.000000 sageworks-0.5.4/src/sageworks/aws_service_broker/aws_service_connectors/glue_jobs.py
+-rw-r--r--   0 briford    (501) staff       (20)     3889 2024-03-28 17:23:43.000000 sageworks-0.5.4/src/sageworks/aws_service_broker/aws_service_connectors/model_registry.py
+-rw-r--r--   0 briford    (501) staff       (20)     3736 2024-03-28 17:23:43.000000 sageworks-0.5.4/src/sageworks/aws_service_broker/aws_service_connectors/s3_bucket.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-03 19:02:27.700525 sageworks-0.5.4/src/sageworks/core/
+-rw-r--r--   0 briford    (501) staff       (20)        0 2024-01-10 18:45:51.000000 sageworks-0.5.4/src/sageworks/core/__init__.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-03 19:02:27.701722 sageworks-0.5.4/src/sageworks/core/artifacts/
+-rw-r--r--   0 briford    (501) staff       (20)      941 2024-03-28 17:23:43.000000 sageworks-0.5.4/src/sageworks/core/artifacts/__init__.py
+-rw-r--r--   0 briford    (501) staff       (20)    17938 2024-03-30 22:43:51.000000 sageworks-0.5.4/src/sageworks/core/artifacts/artifact.py
+-rw-r--r--   0 briford    (501) staff       (20)    22432 2024-03-30 22:43:51.000000 sageworks-0.5.4/src/sageworks/core/artifacts/athena_source.py
+-rw-r--r--   0 briford    (501) staff       (20)    12683 2024-03-28 17:23:43.000000 sageworks-0.5.4/src/sageworks/core/artifacts/data_source_abstract.py
+-rw-r--r--   0 briford    (501) staff       (20)     2447 2024-03-28 17:23:43.000000 sageworks-0.5.4/src/sageworks/core/artifacts/data_source_factory.py
+-rw-r--r--   0 briford    (501) staff       (20)    36414 2024-03-28 17:23:43.000000 sageworks-0.5.4/src/sageworks/core/artifacts/endpoint_core.py
+-rw-r--r--   0 briford    (501) staff       (20)    29123 2024-03-28 17:23:43.000000 sageworks-0.5.4/src/sageworks/core/artifacts/feature_set_core.py
+-rw-r--r--   0 briford    (501) staff       (20)    35018 2024-03-29 21:27:39.000000 sageworks-0.5.4/src/sageworks/core/artifacts/model_core.py
+-rw-r--r--   0 briford    (501) staff       (20)    21029 2024-03-28 17:23:43.000000 sageworks-0.5.4/src/sageworks/core/artifacts/monitor_core.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-03 19:02:27.702133 sageworks-0.5.4/src/sageworks/core/transforms/
+-rw-r--r--   0 briford    (501) staff       (20)     1432 2024-01-10 18:45:51.000000 sageworks-0.5.4/src/sageworks/core/transforms/Readme.md
+-rw-r--r--   0 briford    (501) staff       (20)        0 2024-01-10 18:45:51.000000 sageworks-0.5.4/src/sageworks/core/transforms/__init__.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-03 19:02:27.702419 sageworks-0.5.4/src/sageworks/core/transforms/data_loaders/
+-rw-r--r--   0 briford    (501) staff       (20)        0 2024-01-10 18:45:51.000000 sageworks-0.5.4/src/sageworks/core/transforms/data_loaders/__init__.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-03 19:02:27.702700 sageworks-0.5.4/src/sageworks/core/transforms/data_loaders/heavy/
+-rw-r--r--   0 briford    (501) staff       (20)      298 2024-03-28 17:23:43.000000 sageworks-0.5.4/src/sageworks/core/transforms/data_loaders/heavy/__init__.py
+-rw-r--r--   0 briford    (501) staff       (20)     9866 2024-03-28 17:23:43.000000 sageworks-0.5.4/src/sageworks/core/transforms/data_loaders/heavy/s3_heavy_to_data_source.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-03 19:02:27.703441 sageworks-0.5.4/src/sageworks/core/transforms/data_loaders/light/
+-rw-r--r--   0 briford    (501) staff       (20)      543 2024-03-28 17:23:43.000000 sageworks-0.5.4/src/sageworks/core/transforms/data_loaders/light/__init__.py
+-rw-r--r--   0 briford    (501) staff       (20)     3011 2024-03-28 17:23:43.000000 sageworks-0.5.4/src/sageworks/core/transforms/data_loaders/light/csv_to_data_source.py
+-rw-r--r--   0 briford    (501) staff       (20)     2927 2024-03-28 17:23:43.000000 sageworks-0.5.4/src/sageworks/core/transforms/data_loaders/light/json_to_data_source.py
+-rw-r--r--   0 briford    (501) staff       (20)     4225 2024-03-28 17:23:43.000000 sageworks-0.5.4/src/sageworks/core/transforms/data_loaders/light/s3_to_data_source_light.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-03 19:02:27.703603 sageworks-0.5.4/src/sageworks/core/transforms/data_to_data/
+-rw-r--r--   0 briford    (501) staff       (20)        0 2024-01-10 18:45:51.000000 sageworks-0.5.4/src/sageworks/core/transforms/data_to_data/__init__.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-03 19:02:27.703715 sageworks-0.5.4/src/sageworks/core/transforms/data_to_data/heavy/
+-rw-r--r--   0 briford    (501) staff       (20)        0 2024-01-10 18:45:51.000000 sageworks-0.5.4/src/sageworks/core/transforms/data_to_data/heavy/__init__.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-03 19:02:27.703824 sageworks-0.5.4/src/sageworks/core/transforms/data_to_data/heavy/emr/
+-rw-r--r--   0 briford    (501) staff       (20)       68 2024-01-10 18:45:51.000000 sageworks-0.5.4/src/sageworks/core/transforms/data_to_data/heavy/emr/Readme.md
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-03 19:02:27.703962 sageworks-0.5.4/src/sageworks/core/transforms/data_to_data/heavy/glue/
+-rw-r--r--   0 briford    (501) staff       (20)       48 2024-01-10 18:45:51.000000 sageworks-0.5.4/src/sageworks/core/transforms/data_to_data/heavy/glue/Readme.md
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-03 19:02:27.704335 sageworks-0.5.4/src/sageworks/core/transforms/data_to_data/light/
+-rw-r--r--   0 briford    (501) staff       (20)        0 2024-01-10 18:45:51.000000 sageworks-0.5.4/src/sageworks/core/transforms/data_to_data/light/__init__.py
+-rw-r--r--   0 briford    (501) staff       (20)     2237 2024-03-27 20:40:53.000000 sageworks-0.5.4/src/sageworks/core/transforms/data_to_data/light/clean_data.py
+-rw-r--r--   0 briford    (501) staff       (20)     2687 2024-03-27 20:40:53.000000 sageworks-0.5.4/src/sageworks/core/transforms/data_to_data/light/data_to_data_light.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-03 19:02:27.704481 sageworks-0.5.4/src/sageworks/core/transforms/data_to_features/
+-rw-r--r--   0 briford    (501) staff       (20)        0 2024-01-10 18:45:51.000000 sageworks-0.5.4/src/sageworks/core/transforms/data_to_features/__init__.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-03 19:02:27.704582 sageworks-0.5.4/src/sageworks/core/transforms/data_to_features/heavy/
+-rw-r--r--   0 briford    (501) staff       (20)        0 2024-01-10 18:45:51.000000 sageworks-0.5.4/src/sageworks/core/transforms/data_to_features/heavy/__init__.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-03 19:02:27.704777 sageworks-0.5.4/src/sageworks/core/transforms/data_to_features/heavy/chunk/
+-rw-r--r--   0 briford    (501) staff       (20)        0 2024-01-10 18:45:51.000000 sageworks-0.5.4/src/sageworks/core/transforms/data_to_features/heavy/chunk/__init__.py
+-rw-r--r--   0 briford    (501) staff       (20)     4551 2024-03-28 17:23:43.000000 sageworks-0.5.4/src/sageworks/core/transforms/data_to_features/heavy/chunk/data_to_features_chunk.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-03 19:02:27.704931 sageworks-0.5.4/src/sageworks/core/transforms/data_to_features/heavy/emr/
+-rw-r--r--   0 briford    (501) staff       (20)       68 2024-01-10 18:45:51.000000 sageworks-0.5.4/src/sageworks/core/transforms/data_to_features/heavy/emr/Readme.md
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-03 19:02:27.705069 sageworks-0.5.4/src/sageworks/core/transforms/data_to_features/heavy/glue/
+-rw-r--r--   0 briford    (501) staff       (20)       48 2024-01-10 18:45:51.000000 sageworks-0.5.4/src/sageworks/core/transforms/data_to_features/heavy/glue/Readme.md
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-03 19:02:27.705209 sageworks-0.5.4/src/sageworks/core/transforms/data_to_features/heavy/storage/
+-rw-r--r--   0 briford    (501) staff       (20)     6702 2024-03-28 17:23:43.000000 sageworks-0.5.4/src/sageworks/core/transforms/data_to_features/heavy/storage/data_to_features_heavy_old.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-03 19:02:27.705591 sageworks-0.5.4/src/sageworks/core/transforms/data_to_features/light/
+-rw-r--r--   0 briford    (501) staff       (20)        0 2024-01-10 18:45:51.000000 sageworks-0.5.4/src/sageworks/core/transforms/data_to_features/light/__init__.py
+-rw-r--r--   0 briford    (501) staff       (20)     3827 2024-03-28 17:23:43.000000 sageworks-0.5.4/src/sageworks/core/transforms/data_to_features/light/data_to_features_light.py
+-rw-r--r--   0 briford    (501) staff       (20)     4778 2024-03-28 17:23:43.000000 sageworks-0.5.4/src/sageworks/core/transforms/data_to_features/light/molecular_descriptors.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-03 19:02:27.705743 sageworks-0.5.4/src/sageworks/core/transforms/features_to_features/
+-rw-r--r--   0 briford    (501) staff       (20)        0 2024-01-10 18:45:51.000000 sageworks-0.5.4/src/sageworks/core/transforms/features_to_features/__init__.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-03 19:02:27.661755 sageworks-0.5.4/src/sageworks/core/transforms/features_to_features/heavy/
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-03 19:02:27.705841 sageworks-0.5.4/src/sageworks/core/transforms/features_to_features/heavy/emr/
+-rw-r--r--   0 briford    (501) staff       (20)       68 2024-01-10 18:45:51.000000 sageworks-0.5.4/src/sageworks/core/transforms/features_to_features/heavy/emr/Readme.md
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-03 19:02:27.705980 sageworks-0.5.4/src/sageworks/core/transforms/features_to_features/heavy/glue/
+-rw-r--r--   0 briford    (501) staff       (20)       48 2024-01-10 18:45:51.000000 sageworks-0.5.4/src/sageworks/core/transforms/features_to_features/heavy/glue/Readme.md
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-03 19:02:27.706212 sageworks-0.5.4/src/sageworks/core/transforms/features_to_model/
+-rw-r--r--   0 briford    (501) staff       (20)        0 2024-01-10 18:45:51.000000 sageworks-0.5.4/src/sageworks/core/transforms/features_to_model/__init__.py
+-rw-r--r--   0 briford    (501) staff       (20)    13050 2024-03-28 17:23:43.000000 sageworks-0.5.4/src/sageworks/core/transforms/features_to_model/features_to_model.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-03 19:02:27.706477 sageworks-0.5.4/src/sageworks/core/transforms/features_to_model/light_model_harness/
+-rw-r--r--   0 briford    (501) staff       (20)       19 2024-02-27 23:40:48.000000 sageworks-0.5.4/src/sageworks/core/transforms/features_to_model/light_model_harness/requirements.txt
+-rw-r--r--   0 briford    (501) staff       (20)    10806 2024-03-28 17:23:43.000000 sageworks-0.5.4/src/sageworks/core/transforms/features_to_model/light_model_harness/xgb_model.template
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-03 19:02:27.706730 sageworks-0.5.4/src/sageworks/core/transforms/model_to_endpoint/
+-rw-r--r--   0 briford    (501) staff       (20)        0 2024-01-10 18:45:51.000000 sageworks-0.5.4/src/sageworks/core/transforms/model_to_endpoint/__init__.py
+-rw-r--r--   0 briford    (501) staff       (20)     8185 2024-03-28 17:23:43.000000 sageworks-0.5.4/src/sageworks/core/transforms/model_to_endpoint/model_to_endpoint.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-03 19:02:27.707585 sageworks-0.5.4/src/sageworks/core/transforms/pandas_transforms/
+-rw-r--r--   0 briford    (501) staff       (20)      894 2024-03-28 17:23:43.000000 sageworks-0.5.4/src/sageworks/core/transforms/pandas_transforms/__init__.py
+-rw-r--r--   0 briford    (501) staff       (20)     3615 2024-03-28 17:23:43.000000 sageworks-0.5.4/src/sageworks/core/transforms/pandas_transforms/data_to_pandas.py
+-rw-r--r--   0 briford    (501) staff       (20)     3445 2024-03-28 17:23:43.000000 sageworks-0.5.4/src/sageworks/core/transforms/pandas_transforms/features_to_pandas.py
+-rw-r--r--   0 briford    (501) staff       (20)     8604 2024-03-30 22:43:51.000000 sageworks-0.5.4/src/sageworks/core/transforms/pandas_transforms/pandas_to_data.py
+-rw-r--r--   0 briford    (501) staff       (20)    18139 2024-03-30 22:43:51.000000 sageworks-0.5.4/src/sageworks/core/transforms/pandas_transforms/pandas_to_features.py
+-rw-r--r--   0 briford    (501) staff       (20)     4440 2024-03-28 17:23:43.000000 sageworks-0.5.4/src/sageworks/core/transforms/pandas_transforms/pandas_to_features_chunked.py
+-rw-r--r--   0 briford    (501) staff       (20)     5391 2024-03-28 17:23:43.000000 sageworks-0.5.4/src/sageworks/core/transforms/transform.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-03 19:02:27.707750 sageworks-0.5.4/src/sageworks/experiments/
+-rw-r--r--   0 briford    (501) staff       (20)    10658 2024-03-28 17:23:43.000000 sageworks-0.5.4/src/sageworks/experiments/view_manager.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-03 19:02:27.708028 sageworks-0.5.4/src/sageworks/repl/
+-rw-r--r--   0 briford    (501) staff       (20)        0 2024-01-10 18:45:51.000000 sageworks-0.5.4/src/sageworks/repl/__init__.py
+-rw-r--r--   0 briford    (501) staff       (20)    14538 2024-03-30 22:43:51.000000 sageworks-0.5.4/src/sageworks/repl/sageworks_shell.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-03 19:02:27.708309 sageworks-0.5.4/src/sageworks/resources/
+-rw-r--r--   0 briford    (501) staff       (20)      361 2024-01-23 15:36:53.000000 sageworks-0.5.4/src/sageworks/resources/open_source_api.key
+-rw-r--r--   0 briford    (501) staff       (20)      272 2024-01-10 18:45:51.000000 sageworks-0.5.4/src/sageworks/resources/signature_verify_pub.pem
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-03 19:02:27.712096 sageworks-0.5.4/src/sageworks/utils/
+-rw-r--r--   0 briford    (501) staff       (20)        0 2023-12-24 17:18:24.000000 sageworks-0.5.4/src/sageworks/utils/__init__.py
+-rw-r--r--   0 briford    (501) staff       (20)    15587 2024-03-30 22:43:51.000000 sageworks-0.5.4/src/sageworks/utils/aws_utils.py
+-rw-r--r--   0 briford    (501) staff       (20)     5455 2024-03-28 17:23:43.000000 sageworks-0.5.4/src/sageworks/utils/cache.py
+-rw-r--r--   0 briford    (501) staff       (20)      722 2024-03-28 17:23:43.000000 sageworks-0.5.4/src/sageworks/utils/chem_utils.py
+-rw-r--r--   0 briford    (501) staff       (20)    16234 2024-03-28 17:23:43.000000 sageworks-0.5.4/src/sageworks/utils/config_manager.py
+-rw-r--r--   0 briford    (501) staff       (20)     7392 2024-03-28 17:23:43.000000 sageworks-0.5.4/src/sageworks/utils/dashboard_metrics.py
+-rw-r--r--   0 briford    (501) staff       (20)     4194 2024-03-30 22:43:51.000000 sageworks-0.5.4/src/sageworks/utils/datetime_utils.py
+-rw-r--r--   0 briford    (501) staff       (20)     5292 2024-03-28 17:23:43.000000 sageworks-0.5.4/src/sageworks/utils/df_to_endpoint.py
+-rw-r--r--   0 briford    (501) staff       (20)     1681 2024-03-28 17:23:43.000000 sageworks-0.5.4/src/sageworks/utils/docker_utils.py
+-rw-r--r--   0 briford    (501) staff       (20)     2866 2024-03-27 20:43:31.000000 sageworks-0.5.4/src/sageworks/utils/ecs_info.py
+-rw-r--r--   0 briford    (501) staff       (20)     7657 2024-03-28 17:23:43.000000 sageworks-0.5.4/src/sageworks/utils/endpoint_metrics.py
+-rw-r--r--   0 briford    (501) staff       (20)     3097 2024-03-28 17:23:43.000000 sageworks-0.5.4/src/sageworks/utils/endpoint_utils.py
+-rw-r--r--   0 briford    (501) staff       (20)     6979 2024-03-28 17:23:43.000000 sageworks-0.5.4/src/sageworks/utils/extract_model_artifact.py
+-rw-r--r--   0 briford    (501) staff       (20)     1131 2024-03-28 17:23:43.000000 sageworks-0.5.4/src/sageworks/utils/glue_utils.py
+-rw-r--r--   0 briford    (501) staff       (20)     5757 2024-03-28 17:23:43.000000 sageworks-0.5.4/src/sageworks/utils/license_manager.py
+-rw-r--r--   0 briford    (501) staff       (20)     1439 2024-03-28 17:32:59.000000 sageworks-0.5.4/src/sageworks/utils/markdown_utils.py
+-rw-r--r--   0 briford    (501) staff       (20)    13241 2024-03-28 17:23:43.000000 sageworks-0.5.4/src/sageworks/utils/pandas_utils.py
+-rw-r--r--   0 briford    (501) staff       (20)    12681 2024-04-02 13:06:54.000000 sageworks-0.5.4/src/sageworks/utils/plugin_manager.py
+-rw-r--r--   0 briford    (501) staff       (20)     9533 2024-03-30 22:43:51.000000 sageworks-0.5.4/src/sageworks/utils/redis_cache.py
+-rw-r--r--   0 briford    (501) staff       (20)     4166 2024-03-28 17:23:43.000000 sageworks-0.5.4/src/sageworks/utils/repl_utils.py
+-rw-r--r--   0 briford    (501) staff       (20)     2089 2024-03-28 17:23:43.000000 sageworks-0.5.4/src/sageworks/utils/s3_utils.py
+-rw-r--r--   0 briford    (501) staff       (20)     2163 2024-03-28 17:23:43.000000 sageworks-0.5.4/src/sageworks/utils/sageworks_cache.py
+-rw-r--r--   0 briford    (501) staff       (20)     3474 2024-03-28 17:23:43.000000 sageworks-0.5.4/src/sageworks/utils/sageworks_event_bridge.py
+-rw-r--r--   0 briford    (501) staff       (20)     5359 2024-03-28 17:23:43.000000 sageworks-0.5.4/src/sageworks/utils/sageworks_logging.py
+-rw-r--r--   0 briford    (501) staff       (20)     2120 2024-03-28 17:23:43.000000 sageworks-0.5.4/src/sageworks/utils/sageworks_sqs.py
+-rw-r--r--   0 briford    (501) staff       (20)     1108 2024-01-10 18:45:51.000000 sageworks-0.5.4/src/sageworks/utils/symbols.py
+-rw-r--r--   0 briford    (501) staff       (20)     6414 2024-03-28 17:23:43.000000 sageworks-0.5.4/src/sageworks/utils/test_data_generator.py
+-rw-r--r--   0 briford    (501) staff       (20)     2092 2024-03-27 20:43:31.000000 sageworks-0.5.4/src/sageworks/utils/trace_calls.py
+-rw-r--r--   0 briford    (501) staff       (20)     1470 2024-03-28 17:23:43.000000 sageworks-0.5.4/src/sageworks/utils/type_abbrev.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-03 19:02:27.712991 sageworks-0.5.4/src/sageworks/views/
+-rw-r--r--   0 briford    (501) staff       (20)     3318 2024-03-30 22:43:51.000000 sageworks-0.5.4/src/sageworks/views/artifacts_text_view.py
+-rw-r--r--   0 briford    (501) staff       (20)     7008 2024-03-30 22:43:51.000000 sageworks-0.5.4/src/sageworks/views/artifacts_web_view.py
+-rw-r--r--   0 briford    (501) staff       (20)     3158 2024-03-30 22:43:51.000000 sageworks-0.5.4/src/sageworks/views/data_source_web_view.py
+-rw-r--r--   0 briford    (501) staff       (20)     2150 2024-03-30 22:43:51.000000 sageworks-0.5.4/src/sageworks/views/endpoint_web_view.py
+-rw-r--r--   0 briford    (501) staff       (20)     3206 2024-03-30 22:43:51.000000 sageworks-0.5.4/src/sageworks/views/feature_set_web_view.py
+-rw-r--r--   0 briford    (501) staff       (20)     2029 2024-03-30 22:43:51.000000 sageworks-0.5.4/src/sageworks/views/model_web_view.py
+-rw-r--r--   0 briford    (501) staff       (20)     1092 2024-03-28 17:23:43.000000 sageworks-0.5.4/src/sageworks/views/view.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-03 19:02:27.715432 sageworks-0.5.4/src/sageworks/web_components/
+-rw-r--r--   0 briford    (501) staff       (20)      837 2023-12-24 17:18:24.000000 sageworks-0.5.4/src/sageworks/web_components/color_maps.py
+-rw-r--r--   0 briford    (501) staff       (20)     4902 2024-03-31 15:44:39.000000 sageworks-0.5.4/src/sageworks/web_components/component_interface.py
+-rw-r--r--   0 briford    (501) staff       (20)     3521 2024-03-30 22:43:51.000000 sageworks-0.5.4/src/sageworks/web_components/confusion_matrix.py
+-rw-r--r--   0 briford    (501) staff       (20)     5850 2024-03-30 22:43:51.000000 sageworks-0.5.4/src/sageworks/web_components/correlation_matrix.py
+-rw-r--r--   0 briford    (501) staff       (20)     2970 2024-03-30 22:43:51.000000 sageworks-0.5.4/src/sageworks/web_components/dashboard_metric_plots.py
+-rw-r--r--   0 briford    (501) staff       (20)     9328 2024-04-02 16:53:34.000000 sageworks-0.5.4/src/sageworks/web_components/data_details_markdown.py
+-rw-r--r--   0 briford    (501) staff       (20)     4558 2024-04-02 16:53:34.000000 sageworks-0.5.4/src/sageworks/web_components/endpoint_details.py
+-rw-r--r--   0 briford    (501) staff       (20)     3064 2024-03-30 22:43:51.000000 sageworks-0.5.4/src/sageworks/web_components/endpoint_metric_plots.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-03 19:02:27.716035 sageworks-0.5.4/src/sageworks/web_components/experiments/
+-rw-r--r--   0 briford    (501) staff       (20)     1633 2024-03-28 17:23:43.000000 sageworks-0.5.4/src/sageworks/web_components/experiments/compound_details.py
+-rw-r--r--   0 briford    (501) staff       (20)     1183 2024-03-28 17:23:43.000000 sageworks-0.5.4/src/sageworks/web_components/experiments/histogram.py
+-rw-r--r--   0 briford    (501) staff       (20)     3680 2024-03-28 17:23:43.000000 sageworks-0.5.4/src/sageworks/web_components/experiments/outlier_plot.py
+-rw-r--r--   0 briford    (501) staff       (20)     2279 2024-03-28 17:23:43.000000 sageworks-0.5.4/src/sageworks/web_components/experiments/scatter_plot.py
+-rw-r--r--   0 briford    (501) staff       (20)      838 2024-03-28 17:23:43.000000 sageworks-0.5.4/src/sageworks/web_components/line_chart.py
+-rw-r--r--   0 briford    (501) staff       (20)     8731 2024-04-03 14:14:37.000000 sageworks-0.5.4/src/sageworks/web_components/model_details.py
+-rw-r--r--   0 briford    (501) staff       (20)     2270 2024-03-30 22:43:51.000000 sageworks-0.5.4/src/sageworks/web_components/model_plot.py
+-rw-r--r--   0 briford    (501) staff       (20)     6737 2024-04-03 18:50:52.000000 sageworks-0.5.4/src/sageworks/web_components/plugin_interface.py
+-rw-r--r--   0 briford    (501) staff       (20)     2941 2024-03-30 22:43:51.000000 sageworks-0.5.4/src/sageworks/web_components/regression_plot.py
+-rw-r--r--   0 briford    (501) staff       (20)     6535 2024-03-28 17:23:43.000000 sageworks-0.5.4/src/sageworks/web_components/table.py
+-rw-r--r--   0 briford    (501) staff       (20)     5181 2024-03-30 22:43:51.000000 sageworks-0.5.4/src/sageworks/web_components/violin_plots.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-03 19:02:27.720468 sageworks-0.5.4/src/sageworks.egg-info/
+-rw-r--r--   0 briford    (501) staff       (20)     4118 2024-04-03 19:02:27.000000 sageworks-0.5.4/src/sageworks.egg-info/PKG-INFO
+-rw-r--r--   0 briford    (501) staff       (20)    17380 2024-04-03 19:02:27.000000 sageworks-0.5.4/src/sageworks.egg-info/SOURCES.txt
+-rw-r--r--   0 briford    (501) staff       (20)        1 2024-04-03 19:02:27.000000 sageworks-0.5.4/src/sageworks.egg-info/dependency_links.txt
+-rw-r--r--   0 briford    (501) staff       (20)       74 2024-04-03 19:02:27.000000 sageworks-0.5.4/src/sageworks.egg-info/entry_points.txt
+-rw-r--r--   0 briford    (501) staff       (20)      408 2024-04-03 19:02:27.000000 sageworks-0.5.4/src/sageworks.egg-info/requires.txt
+-rw-r--r--   0 briford    (501) staff       (20)       10 2024-04-03 19:02:27.000000 sageworks-0.5.4/src/sageworks.egg-info/top_level.txt
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-03 19:02:27.716911 sageworks-0.5.4/tests/
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-03 19:02:27.717492 sageworks-0.5.4/tests/artifacts/
+-rw-r--r--   0 briford    (501) staff       (20)     1548 2024-03-30 19:27:28.000000 sageworks-0.5.4/tests/artifacts/data_source_tests.py
+-rw-r--r--   0 briford    (501) staff       (20)     2442 2024-03-28 17:23:43.000000 sageworks-0.5.4/tests/artifacts/endpoint_tests.py
+-rw-r--r--   0 briford    (501) staff       (20)     1160 2024-03-28 17:23:43.000000 sageworks-0.5.4/tests/artifacts/feature_set_tests.py
+-rw-r--r--   0 briford    (501) staff       (20)      805 2024-03-28 17:23:43.000000 sageworks-0.5.4/tests/artifacts/model_tests.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-03 19:02:27.717764 sageworks-0.5.4/tests/aws_account/
+-rw-r--r--   0 briford    (501) staff       (20)      962 2023-12-24 17:18:24.000000 sageworks-0.5.4/tests/aws_account/aws_account_clamp_tests.py
+-rw-r--r--   0 briford    (501) staff       (20)      642 2023-12-24 17:18:24.000000 sageworks-0.5.4/tests/aws_account/aws_service_broker_tests.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-03 19:02:27.718595 sageworks-0.5.4/tests/connectors/
+-rw-r--r--   0 briford    (501) staff       (20)      725 2024-03-28 17:23:43.000000 sageworks-0.5.4/tests/connectors/data_catalog.py
+-rw-r--r--   0 briford    (501) staff       (20)      737 2024-03-28 17:23:43.000000 sageworks-0.5.4/tests/connectors/endpoints.py
+-rw-r--r--   0 briford    (501) staff       (20)      702 2024-03-28 17:23:43.000000 sageworks-0.5.4/tests/connectors/feature_store.py
+-rw-r--r--   0 briford    (501) staff       (20)      644 2024-03-28 17:23:43.000000 sageworks-0.5.4/tests/connectors/glue_jobs.py
+-rw-r--r--   0 briford    (501) staff       (20)      799 2024-03-28 17:23:43.000000 sageworks-0.5.4/tests/connectors/model_registry.py
+-rw-r--r--   0 briford    (501) staff       (20)     1008 2024-03-28 17:23:43.000000 sageworks-0.5.4/tests/connectors/s3_bucket.py
+-rw-r--r--   0 briford    (501) staff       (20)     5408 2024-03-28 17:23:43.000000 sageworks-0.5.4/tests/create_aqsol_artifacts.py
+-rw-r--r--   0 briford    (501) staff       (20)     3217 2024-03-28 17:23:43.000000 sageworks-0.5.4/tests/create_basic_test_artifacts.py
+-rw-r--r--   0 briford    (501) staff       (20)      870 2024-03-28 17:23:43.000000 sageworks-0.5.4/tests/create_realtime_endpoint.py
+-rw-r--r--   0 briford    (501) staff       (20)     2379 2024-03-28 17:23:43.000000 sageworks-0.5.4/tests/create_training_adjusted_artifacts.py
+-rw-r--r--   0 briford    (501) staff       (20)     2096 2024-03-28 17:23:43.000000 sageworks-0.5.4/tests/create_wine_artifacts.py
+-rw-r--r--   0 briford    (501) staff       (20)     4310 2024-03-28 17:23:43.000000 sageworks-0.5.4/tests/delete_test_artifacts.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-03 19:02:27.718727 sageworks-0.5.4/tests/plugin_tests/
+-rw-r--r--   0 briford    (501) staff       (20)     1888 2024-03-30 22:43:51.000000 sageworks-0.5.4/tests/plugin_tests/crashing_plugin.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-03 19:02:27.719001 sageworks-0.5.4/tests/specific/
+-rw-r--r--   0 briford    (501) staff       (20)      639 2024-03-28 17:23:43.000000 sageworks-0.5.4/tests/specific/capital_tests.py
+-rw-r--r--   0 briford    (501) staff       (20)     1513 2024-03-28 17:23:43.000000 sageworks-0.5.4/tests/specific/deletion_tests.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-03 19:02:27.719869 sageworks-0.5.4/tests/transforms/
+-rw-r--r--   0 briford    (501) staff       (20)      592 2024-03-28 17:23:43.000000 sageworks-0.5.4/tests/transforms/data_to_data_tests.py
+-rw-r--r--   0 briford    (501) staff       (20)     1025 2024-03-28 17:23:43.000000 sageworks-0.5.4/tests/transforms/data_to_features_tests.py
+-rw-r--r--   0 briford    (501) staff       (20)      773 2024-03-28 17:23:43.000000 sageworks-0.5.4/tests/transforms/features_to_model_tests.py
+-rw-r--r--   0 briford    (501) staff       (20)     4864 2024-03-28 17:23:43.000000 sageworks-0.5.4/tests/transforms/model_metrics_tests.py
+-rw-r--r--   0 briford    (501) staff       (20)      795 2024-03-28 17:23:43.000000 sageworks-0.5.4/tests/transforms/model_to_endpoint_tests.py
+-rw-r--r--   0 briford    (501) staff       (20)      633 2024-03-27 20:40:53.000000 sageworks-0.5.4/tests/transforms/pandas_to_data_tests.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-04-03 19:02:27.720255 sageworks-0.5.4/tests/web_components/
+-rw-r--r--   0 briford    (501) staff       (20)      679 2024-03-30 22:43:51.000000 sageworks-0.5.4/tests/web_components/confusion_matrix_test.py
+-rw-r--r--   0 briford    (501) staff       (20)      675 2024-03-30 22:43:51.000000 sageworks-0.5.4/tests/web_components/correlation_matrix_test.py
+-rw-r--r--   0 briford    (501) staff       (20)     5210 2024-03-30 22:43:51.000000 sageworks-0.5.4/tests/web_components/plugin_interface_test.py
+-rw-r--r--   0 briford    (501) staff       (20)     1115 2024-03-27 20:43:31.000000 sageworks-0.5.4/tox.ini
```

### Comparing `sageworks-0.5.3/.github/PULL_REQUEST_TEMPLATE.md` & `sageworks-0.5.4/.github/PULL_REQUEST_TEMPLATE.md`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.3/.github/workflows/deploy-docs.yml` & `sageworks-0.5.4/.github/workflows/deploy-docs.yml`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.3/.github/workflows/python-lint.yml` & `sageworks-0.5.4/.github/workflows/python-lint.yml`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.3/.gitignore` & `sageworks-0.5.4/.gitignore`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.3/LICENSE` & `sageworks-0.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.3/Makefile` & `sageworks-0.5.4/Makefile`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.3/PKG-INFO` & `sageworks-0.5.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sageworks
-Version: 0.5.3
+Version: 0.5.4
 Summary: SageWorks: A Python WorkBench for creating and deploying AWS SageMaker Models
 Home-page: https://github.com/SuperCowPowers/sageworks
 Author: SuperCowPowers LLC
 Author-email: support@supercowpowers.com
 License: MIT
 Keywords: SageMaker,Machine Learning,AWS,Python,Utilities
 Classifier: Development Status :: 4 - Beta
```

### Comparing `sageworks-0.5.3/README.md` & `sageworks-0.5.4/README.md`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.3/applications/aws_dashboard/Dockerfile` & `sageworks-0.5.4/applications/aws_dashboard/Dockerfile`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 RUN pip install --no-cache-dir -r requirements.txt
 
 # Copy the Nginx and Supervisor configuration files
 COPY nginx.conf /etc/nginx/sites-available/default
 COPY supervisord.conf /etc/supervisor/conf.d/supervisord.conf
 
 # Install Sageworks (changes often)
-RUN pip install --no-cache-dir sageworks==0.5.2
+RUN pip install --no-cache-dir sageworks==0.5.3
 
 # Copy the current directory contents into the container at /app
 COPY . /app
 
 # Grab the config file from build args, copy, and set ENV var
 ARG SAGEWORKS_CONFIG
 COPY $SAGEWORKS_CONFIG /app/sageworks_config.json
```

### Comparing `sageworks-0.5.3/applications/aws_dashboard/README.md` & `sageworks-0.5.4/applications/aws_dashboard/README.md`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.3/applications/aws_dashboard/assets/custom.css` & `sageworks-0.5.4/applications/aws_dashboard/assets/default.css`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.3/applications/aws_dashboard/assets/trash.png` & `sageworks-0.5.4/applications/aws_dashboard/assets/trash.png`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.3/applications/aws_dashboard/dashboard` & `sageworks-0.5.4/applications/aws_dashboard/dashboard`

 * *Files 27% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 def start_dashboard(debug: bool):
     """Open a browser and start the Dash app"""
     url = "http://localhost:8000"
     webbrowser.open(url)
 
     # Note: This 'main' is purely for running/testing locally
-    app.run_server(host="0.0.0.0", port=8000, debug=debug)
+    app.run(host="0.0.0.0", port=8000, debug=debug)
 
 
 if __name__ == "__main__":
     """Run our web application in TEST mode"""
     parser = argparse.ArgumentParser(description='Start the Dash app')
     parser.add_argument('--debug', action='store_true', help='Run the app in debug mode')
     args = parser.parse_args()
```

### Comparing `sageworks-0.5.3/applications/aws_dashboard/open_source_config.json` & `sageworks-0.5.4/applications/aws_dashboard/open_source_config.json`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.3/applications/aws_dashboard/pages/data_sources/callbacks.py` & `sageworks-0.5.4/applications/aws_dashboard/pages/data_sources/callbacks.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.3/applications/aws_dashboard/pages/data_sources/layout.py` & `sageworks-0.5.4/applications/aws_dashboard/pages/data_sources/layout.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.3/applications/aws_dashboard/pages/data_sources/page.py` & `sageworks-0.5.4/applications/aws_dashboard/pages/data_sources/page.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.3/applications/aws_dashboard/pages/endpoints/callbacks.py` & `sageworks-0.5.4/applications/aws_dashboard/pages/endpoints/callbacks.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.3/applications/aws_dashboard/pages/endpoints/layout.py` & `sageworks-0.5.4/applications/aws_dashboard/pages/endpoints/layout.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.3/applications/aws_dashboard/pages/endpoints/page.py` & `sageworks-0.5.4/applications/aws_dashboard/pages/endpoints/page.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.3/applications/aws_dashboard/pages/feature_sets/callbacks.py` & `sageworks-0.5.4/applications/aws_dashboard/pages/feature_sets/callbacks.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.3/applications/aws_dashboard/pages/feature_sets/layout.py` & `sageworks-0.5.4/applications/aws_dashboard/pages/feature_sets/layout.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.3/applications/aws_dashboard/pages/feature_sets/page.py` & `sageworks-0.5.4/applications/aws_dashboard/pages/feature_sets/page.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.3/applications/aws_dashboard/pages/main/callbacks.py` & `sageworks-0.5.4/applications/aws_dashboard/pages/main/callbacks.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.3/applications/aws_dashboard/pages/main/layout.py` & `sageworks-0.5.4/applications/aws_dashboard/pages/main/layout.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.3/applications/aws_dashboard/pages/main/page.py` & `sageworks-0.5.4/applications/aws_dashboard/pages/main/page.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.3/applications/aws_dashboard/pages/models/callbacks.py` & `sageworks-0.5.4/applications/aws_dashboard/pages/models/callbacks.py`

 * *Files 2% similar despite different names*

```diff
@@ -77,23 +77,23 @@
         return model_plot_fig
 
 
 # Updates the plugin component when a model row is selected
 def update_plugin(app: Dash, plugin, model_web_view: ModelWebView):
     @app.callback(
         Output(plugin.component_id(), "figure"),
-        Input("models_table", "derived_viewport_selected_row_ids"),
+        [Input("model_details-dropdown", "value"), Input("models_table", "derived_viewport_selected_row_ids")],
         State("models_table", "data"),
         prevent_initial_call=True,
     )
-    def update_plugin_figure(selected_rows, table_data):
+    def update_plugin_figure(inference_run, selected_rows, table_data):
         # Check for no selected rows
         if not selected_rows or selected_rows[0] is None:
             return no_update
 
         # Get the selected row data and grab the uuid
         selected_row_data = table_data[selected_rows[0]]
         model_uuid = selected_row_data["uuid"]
 
         # Instantiate the Model and send it to the plugin
         model = Model(model_uuid, legacy=True)
-        return plugin.update_contents(model)
+        return plugin.update_contents(model, inference_run=inference_run)
```

### Comparing `sageworks-0.5.3/applications/aws_dashboard/pages/models/layout.py` & `sageworks-0.5.4/applications/aws_dashboard/pages/models/layout.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.3/applications/aws_dashboard/pages/models/page.py` & `sageworks-0.5.4/applications/aws_dashboard/pages/models/page.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.3/applications/experiments/compound_explorer/app.py` & `sageworks-0.5.4/applications/experiments/compound_explorer/app.py`

 * *Files 4% similar despite different names*

```diff
@@ -87,9 +87,9 @@
 callbacks.update_violin_plots(app, data_source_broker)
 callbacks.update_compound_rows(app, data_source_broker)
 callbacks.update_compound_diagram(app)
 
 if __name__ == "__main__":
     """Run our web application in TEST mode"""
     # Note: This 'main' is purely for running/testing locally
-    app.run_server(host="0.0.0.0", port=8082, debug=True)
-    # app.run_server(host="0.0.0.0", port=8082)
+    app.run(host="0.0.0.0", port=8082, debug=True)
+    # app.run(host="0.0.0.0", port=8082)
```

### Comparing `sageworks-0.5.3/applications/experiments/compound_explorer/assets/custom.css` & `sageworks-0.5.4/applications/experiments/compound_explorer/assets/custom.css`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.3/applications/experiments/compound_explorer/callbacks.py` & `sageworks-0.5.4/applications/experiments/compound_explorer/callbacks.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.3/applications/experiments/compound_explorer/layout.py` & `sageworks-0.5.4/applications/experiments/compound_explorer/layout.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.3/aws_setup/aws_account_check.py` & `sageworks-0.5.4/aws_setup/aws_account_check.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.3/aws_setup/aws_identity_check.py` & `sageworks-0.5.4/aws_setup/aws_identity_check.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.3/aws_setup/build_ml_pipeline.py` & `sageworks-0.5.4/aws_setup/build_ml_pipeline.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.3/aws_setup/event_bridge/dynamic_docker/app.py` & `sageworks-0.5.4/aws_setup/event_bridge/dynamic_docker/app.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.3/aws_setup/event_bridge/dynamic_docker/cdk.json` & `sageworks-0.5.4/aws_setup/event_bridge/dynamic_docker/cdk.json`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.3/aws_setup/event_bridge/dynamic_docker/lambda/lambda_replace_task.py` & `sageworks-0.5.4/aws_setup/event_bridge/dynamic_docker/lambda/lambda_replace_task.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.3/aws_setup/event_bridge/dynamic_docker/sageworks_image_update_stack.py` & `sageworks-0.5.4/aws_setup/event_bridge/dynamic_docker/sageworks_image_update_stack.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.3/aws_setup/sageworks_core/README.md` & `sageworks-0.5.4/aws_setup/sageworks_core/README.md`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.3/aws_setup/sageworks_core/app.py` & `sageworks-0.5.4/aws_setup/sageworks_core/app.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.3/aws_setup/sageworks_core/cdk.json` & `sageworks-0.5.4/aws_setup/sageworks_core/cdk.json`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.3/aws_setup/sageworks_core/sageworks_core/sageworks_core_stack.py` & `sageworks-0.5.4/aws_setup/sageworks_core/sageworks_core/sageworks_core_stack.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.3/aws_setup/sageworks_core/tests/unit/test_sageworks_sandbox_stack.py` & `sageworks-0.5.4/aws_setup/sageworks_core/tests/unit/test_sageworks_sandbox_stack.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.3/aws_setup/sageworks_dashboard_full/README.md` & `sageworks-0.5.4/aws_setup/sageworks_dashboard_full/README.md`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.3/aws_setup/sageworks_dashboard_full/app.py` & `sageworks-0.5.4/aws_setup/sageworks_dashboard_full/app.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.3/aws_setup/sageworks_dashboard_full/cdk.json` & `sageworks-0.5.4/aws_setup/sageworks_dashboard_full/cdk.json`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.3/aws_setup/sageworks_dashboard_full/sageworks_dashboard_full/sageworks_dashboard_stack.py` & `sageworks-0.5.4/aws_setup/sageworks_dashboard_full/sageworks_dashboard_full/sageworks_dashboard_stack.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 )
 from aws_cdk.aws_ec2 import Subnet
 from aws_cdk.aws_certificatemanager import Certificate
 from aws_cdk.aws_ecs_patterns import ApplicationLoadBalancedFargateService
 from constructs import Construct
 
 # When you want a different version change this line
-dashboard_image = "public.ecr.aws/m6i5k1r2/sageworks_dashboard:v0_5_2_amd64"
+dashboard_image = "public.ecr.aws/m6i5k1r2/sageworks_dashboard:v0_5_3_amd64"
 
 
 class SageworksDashboardStackProps(StackProps):
     def __init__(
         self,
         sageworks_bucket: str,
         sageworks_api_key: str,
```

### Comparing `sageworks-0.5.3/aws_setup/sageworks_dashboard_full/tests/unit/test_sageworks_dashboard_stack.py` & `sageworks-0.5.4/aws_setup/sageworks_dashboard_full/tests/unit/test_sageworks_dashboard_stack.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.3/aws_setup/sageworks_dashboard_lite/README.md` & `sageworks-0.5.4/aws_setup/sageworks_dashboard_lite/README.md`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.3/aws_setup/sageworks_dashboard_lite/app.py` & `sageworks-0.5.4/aws_setup/sageworks_dashboard_lite/app.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.3/aws_setup/sageworks_dashboard_lite/cdk.json` & `sageworks-0.5.4/aws_setup/sageworks_dashboard_lite/cdk.json`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.3/aws_setup/sageworks_dashboard_lite/sageworks_dashboard_lite/sageworks_dashboard_stack.py` & `sageworks-0.5.4/aws_setup/sageworks_dashboard_lite/sageworks_dashboard_lite/sageworks_dashboard_stack.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.3/data/abalone.csv` & `sageworks-0.5.4/data/abalone.csv`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.3/data/test_data.csv` & `sageworks-0.5.4/data/test_data.csv`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.3/data/test_data.json` & `sageworks-0.5.4/data/test_data.json`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.3/data/wine_dataset.csv` & `sageworks-0.5.4/data/wine_dataset.csv`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.3/docs/admin/docker_push.md` & `sageworks-0.5.4/docs/admin/docker_push.md`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.3/docs/admin/pypi_release.md` & `sageworks-0.5.4/docs/admin/pypi_release.md`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.3/docs/api_classes/data_source.md` & `sageworks-0.5.4/docs/api_classes/data_source.md`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.3/docs/api_classes/endpoint.md` & `sageworks-0.5.4/docs/api_classes/endpoint.md`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.3/docs/api_classes/feature_set.md` & `sageworks-0.5.4/docs/api_classes/feature_set.md`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.3/docs/api_classes/meta.md` & `sageworks-0.5.4/docs/api_classes/meta.md`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.3/docs/api_classes/model.md` & `sageworks-0.5.4/docs/api_classes/model.md`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.3/docs/api_classes/monitor.md` & `sageworks-0.5.4/docs/api_classes/monitor.md`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.3/docs/api_classes/overview.md` & `sageworks-0.5.4/docs/api_classes/overview.md`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.3/docs/aws_setup/aws_access_management.md` & `sageworks-0.5.4/docs/aws_setup/aws_access_management.md`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.3/docs/aws_setup/aws_tips_and_tricks.md` & `sageworks-0.5.4/docs/aws_setup/aws_tips_and_tricks.md`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.3/docs/aws_setup/core_stack.md` & `sageworks-0.5.4/docs/aws_setup/core_stack.md`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.3/docs/aws_setup/dashboard_stack.md` & `sageworks-0.5.4/docs/aws_setup/dashboard_stack.md`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.3/docs/aws_setup/full_pipeline.md` & `sageworks-0.5.4/docs/aws_setup/full_pipeline.md`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.3/docs/concepts/model_monitoring.md` & `sageworks-0.5.4/docs/concepts/model_monitoring.md`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.3/docs/core_classes/artifacts/overview.md` & `sageworks-0.5.4/docs/core_classes/artifacts/overview.md`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.3/docs/core_classes/overview.md` & `sageworks-0.5.4/docs/core_classes/overview.md`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.3/docs/core_classes/transforms/overview.md` & `sageworks-0.5.4/docs/core_classes/transforms/overview.md`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.3/docs/core_classes/transforms/pandas_transforms.md` & `sageworks-0.5.4/docs/core_classes/transforms/pandas_transforms.md`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.3/docs/core_classes/transforms/transform.md` & `sageworks-0.5.4/docs/core_classes/transforms/transform.md`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.3/docs/glue/index.md` & `sageworks-0.5.4/docs/glue/index.md`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.3/docs/images/big_spider.png` & `sageworks-0.5.4/docs/images/big_spider.png`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.3/docs/images/graph_representation.png` & `sageworks-0.5.4/docs/images/graph_representation.png`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.3/docs/images/powered_aws_dark_blue.png` & `sageworks-0.5.4/docs/images/powered_aws_dark_blue.png`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.3/docs/images/powered_aws_transparent.png` & `sageworks-0.5.4/docs/images/powered_aws_transparent.png`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.3/docs/images/powered_aws_white.png` & `sageworks-0.5.4/docs/images/powered_aws_white.png`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.3/docs/images/powered_aws_with_tm_grey.png` & `sageworks-0.5.4/docs/images/powered_aws_with_tm_grey.png`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.3/docs/images/sageworks.png` & `sageworks-0.5.4/docs/images/sageworks.png`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.3/docs/images/sageworks_concepts.png` & `sageworks-0.5.4/docs/images/sageworks_concepts.png`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.3/docs/images/scp.png` & `sageworks-0.5.4/docs/images/scp.png`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.3/docs/images/scp_labs.png` & `sageworks-0.5.4/docs/images/scp_labs.png`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.3/docs/images/small_spider.png` & `sageworks-0.5.4/docs/images/small_spider.png`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.3/docs/index.md` & `sageworks-0.5.4/docs/index.md`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.3/docs/misc/faq.md` & `sageworks-0.5.4/docs/misc/faq.md`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.3/docs/misc/general_info.md` & `sageworks-0.5.4/docs/misc/general_info.md`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.3/docs/misc/sageworks_classes_concepts.md` & `sageworks-0.5.4/docs/misc/sageworks_classes_concepts.md`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.3/docs/misc/scp_consulting.md` & `sageworks-0.5.4/docs/misc/scp_consulting.md`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.3/docs/plugins/index.md` & `sageworks-0.5.4/docs/plugins/index.md`

 * *Files 4% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 
 The SageWorks Plugin system allows clients to customize how their AWS Machine Learning Pipeline is displayed, analyzed, and visualized. Our easy to use Python API enables developers to make new [Dash/Plotly](https://plotly.com/) components, data views, and entirely new web pages focused on business use cases.
 
 ### Concept Docs
 Many classes in SageWorks need additional high-level material that covers class design and illustrates class usage. Here's the Concept Docs for Plugins:
  
 - [Getting Started]( https://docs.google.com/presentation/d/1S_-XapmyTsXIkO6od9AVkTbEU2nqS-mEZwFrtUucUME/edit?usp=sharing) 
+- [Plugin Pages](https://docs.google.com/presentation/d/1Yp4ka8DGPdRs8WfsAAUTnc0SHzkkcdJY2TABKxD_CPo/edit?usp=sharing)
 - [Plugins Advanced](https://docs.google.com/presentation/d/1sByTnZa24lY6d4INRMm7OHmQndIZmLbTxOyTeAJol20/edit?usp=sharing)
 
 ## Make a plugin
 
 Each plugin class inherits from the SageWorks PluginInterface class and needs to set two attributes and implement two methods. These requirements are set so that each Plugin will conform to the Sageworks infrastructure; if the required attributes and methods aren’t included in the class definition, errors will be raised during tests and at runtime.
 
 ```
@@ -35,15 +36,15 @@
 ```
   
 
 
 
 ### Required Attributes
 
-The class variable plugin_page determines what type of plugin the MyPlugin class is. This variable is inspected during plugin loading at runtime in order to load the plugin to the correct artifact page in the Sageworks dashboard. The PluginPage class can be DATA_SOURCE, FEATURE_SET, MODEL, or ENDPOINT.
+The class variable plugin\_page determines what type of plugin the MyPlugin class is. This variable is inspected during plugin loading at runtime in order to load the plugin to the correct artifact page in the Sageworks dashboard. The PluginPage class can be DATA_SOURCE, FEATURE\_SET, MODEL, or ENDPOINT.
 
 ## S3 Bucket Plugins (Work in Progress)
 Note: This functionality is coming soon
 
 Offers the most flexibility and fast prototyping. Simple set your config/env for  blah to an S3 Path and SageWorks will load the plugins from S3 directly.
 
 **Helpful Tip**
```

### Comparing `sageworks-0.5.3/docs/plugins/plugin_api_changes.md` & `sageworks-0.5.4/docs/plugins/plugin_api_changes.md`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.3/docs/repl/index.md` & `sageworks-0.5.4/docs/repl/index.md`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.3/docs/research/eda.md` & `sageworks-0.5.4/docs/research/eda.md`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.3/docs/research/htg.md` & `sageworks-0.5.4/docs/research/htg.md`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.3/examples/datasource_query.py` & `sageworks-0.5.4/examples/datasource_query.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.3/examples/datasource_stats.py` & `sageworks-0.5.4/examples/datasource_stats.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.3/examples/endpoint_inference.py` & `sageworks-0.5.4/examples/endpoint_inference.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.3/examples/featureset_eda.py` & `sageworks-0.5.4/examples/featureset_eda.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.3/examples/featureset_query.py` & `sageworks-0.5.4/examples/featureset_query.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.3/examples/full_ml_pipeline.py` & `sageworks-0.5.4/examples/full_ml_pipeline.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.3/examples/glue_hello_world.py` & `sageworks-0.5.4/examples/glue_hello_world.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.3/examples/glue_hello_world_with_log.py` & `sageworks-0.5.4/examples/glue_hello_world_with_log.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.3/examples/glue_load_s3_bucket.py` & `sageworks-0.5.4/examples/glue_load_s3_bucket.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.3/examples/meta_model_metrics.py` & `sageworks-0.5.4/examples/meta_model_metrics.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.3/examples/model_metrics.py` & `sageworks-0.5.4/examples/model_metrics.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.3/examples/monitor_usage.py` & `sageworks-0.5.4/examples/monitor_usage.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.3/examples/plugins/pages/my_plugin_page.py` & `sageworks-0.5.4/examples/plugins/pages/my_plugin_page.py`

 * *Files 4% similar despite different names*

```diff
@@ -78,8 +78,8 @@
     # Call page setup
     plugin_page.page_setup(app)
 
     # Manually set the layout of the app to the layout of the plugin page
     app.layout = plugin_page.page_layout()
 
     # Run the app in debug mode
-    app.run_server(debug=True)
+    app.run(debug=True)
```

### Comparing `sageworks-0.5.3/examples/plugins/views/my_view_plugin.py` & `sageworks-0.5.4/examples/plugins/views/my_view_plugin.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.3/examples/plugins/web_components/endpoint_plugin.py` & `sageworks-0.5.4/examples/plugins/web_components/endpoint_plugin.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.3/examples/plugins/web_components/model_plugin.py` & `sageworks-0.5.4/examples/plugins/web_components/model_plugin.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.3/examples/sagemaker_pipelines/all_steps.py` & `sageworks-0.5.4/examples/sagemaker_pipelines/all_steps.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.3/examples/sagemaker_pipelines/ml_pipeline.py` & `sageworks-0.5.4/examples/sagemaker_pipelines/ml_pipeline.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.3/examples/sagemaker_pipelines/storage/full_pipeline_experiment/data_source.py` & `sageworks-0.5.4/examples/sagemaker_pipelines/storage/full_pipeline_experiment/data_source.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.3/examples/sagemaker_pipelines/storage/full_pipeline_experiment/ml_pipeline.py` & `sageworks-0.5.4/examples/sagemaker_pipelines/storage/full_pipeline_experiment/ml_pipeline.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.3/examples/storage/data_to_data.py` & `sageworks-0.5.4/examples/storage/data_to_data.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.3/examples/storage/data_to_features.py` & `sageworks-0.5.4/examples/storage/data_to_features.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.3/examples/storage/endpoint_inference.py` & `sageworks-0.5.4/examples/storage/endpoint_inference.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.3/examples/storage/hello_world_pipeline.py` & `sageworks-0.5.4/examples/storage/hello_world_pipeline.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.3/examples/storage/plugin_page_example.py` & `sageworks-0.5.4/examples/storage/plugin_page_example.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.3/mkdocs.yml` & `sageworks-0.5.4/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.3/notebooks/ML_Pipeline_with_SageWorks.ipynb` & `sageworks-0.5.4/notebooks/ML_Pipeline_with_SageWorks.ipynb`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.3/notebooks/ML_Pipeline_with_SageWorks_2.ipynb` & `sageworks-0.5.4/notebooks/ML_Pipeline_with_SageWorks_2.ipynb`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.3/notebooks/Outliers_in_SageWorks.ipynb` & `sageworks-0.5.4/notebooks/Outliers_in_SageWorks.ipynb`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.3/notebooks/images/athena_query_aqsol.png` & `sageworks-0.5.4/notebooks/images/athena_query_aqsol.png`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.3/notebooks/images/aws_dashboard_aqsol.png` & `sageworks-0.5.4/notebooks/images/aws_dashboard_aqsol.png`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.3/notebooks/images/dashboard_aqsol_features.png` & `sageworks-0.5.4/notebooks/images/dashboard_aqsol_features.png`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.3/notebooks/images/model_screenshot.png` & `sageworks-0.5.4/notebooks/images/model_screenshot.png`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.3/notebooks/images/sageworks_concepts.png` & `sageworks-0.5.4/notebooks/images/sageworks_concepts.png`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.3/notebooks/images/scp_labs.png` & `sageworks-0.5.4/notebooks/images/scp_labs.png`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.3/scripts/athena_ddl_mixed_case.py` & `sageworks-0.5.4/scripts/athena_ddl_mixed_case.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.3/scripts/copy_data_catalog_db.py` & `sageworks-0.5.4/scripts/copy_data_catalog_db.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.3/scripts/delete_redis_keys.py` & `sageworks-0.5.4/scripts/delete_redis_keys.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.3/scripts/glue_mixed_case.py` & `sageworks-0.5.4/scripts/glue_mixed_case.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.3/scripts/model_endpoint_sanity_check.py` & `sageworks-0.5.4/scripts/model_endpoint_sanity_check.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.3/scripts/onboard_endpoints.py` & `sageworks-0.5.4/scripts/onboard_endpoints.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.3/scripts/onboard_models.py` & `sageworks-0.5.4/scripts/onboard_models.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.3/scripts/storage/dns_data_to_features.py` & `sageworks-0.5.4/scripts/storage/dns_data_to_features.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.3/scripts/storage/generate_jsonl_data.py` & `sageworks-0.5.4/scripts/storage/generate_jsonl_data.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.3/scripts/test_feature_resolution.py` & `sageworks-0.5.4/scripts/test_feature_resolution.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.3/setup.cfg` & `sageworks-0.5.4/setup.cfg`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.3/setup.py` & `sageworks-0.5.4/setup.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.3/src/sageworks/__init__.py` & `sageworks-0.5.4/src/sageworks/__init__.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.3/src/sageworks/algorithms/dataframe/aggregation.py` & `sageworks-0.5.4/src/sageworks/algorithms/dataframe/aggregation.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.3/src/sageworks/algorithms/dataframe/data_source_eda.py` & `sageworks-0.5.4/src/sageworks/algorithms/dataframe/data_source_eda.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.3/src/sageworks/algorithms/dataframe/dimensionality_reduction.py` & `sageworks-0.5.4/src/sageworks/algorithms/dataframe/dimensionality_reduction.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.3/src/sageworks/algorithms/dataframe/feature_resolution.py` & `sageworks-0.5.4/src/sageworks/algorithms/dataframe/feature_resolution.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.3/src/sageworks/algorithms/dataframe/feature_spider.py` & `sageworks-0.5.4/src/sageworks/algorithms/dataframe/feature_spider.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.3/src/sageworks/algorithms/dataframe/row_tagger.py` & `sageworks-0.5.4/src/sageworks/algorithms/dataframe/row_tagger.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.3/src/sageworks/algorithms/spark/Readme.md` & `sageworks-0.5.4/src/sageworks/algorithms/spark/Readme.md`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.3/src/sageworks/algorithms/sql/Readme.md` & `sageworks-0.5.4/src/sageworks/algorithms/sql/Readme.md`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.3/src/sageworks/algorithms/sql/column_stats.py` & `sageworks-0.5.4/src/sageworks/algorithms/sql/column_stats.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.3/src/sageworks/algorithms/sql/correlations.py` & `sageworks-0.5.4/src/sageworks/algorithms/sql/correlations.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.3/src/sageworks/algorithms/sql/descriptive_stats.py` & `sageworks-0.5.4/src/sageworks/algorithms/sql/descriptive_stats.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.3/src/sageworks/algorithms/sql/outliers.py` & `sageworks-0.5.4/src/sageworks/algorithms/sql/outliers.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.3/src/sageworks/algorithms/sql/sample_rows.py` & `sageworks-0.5.4/src/sageworks/algorithms/sql/sample_rows.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.3/src/sageworks/algorithms/sql/value_counts.py` & `sageworks-0.5.4/src/sageworks/algorithms/sql/value_counts.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.3/src/sageworks/api/__init__.py` & `sageworks-0.5.4/src/sageworks/api/__init__.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.3/src/sageworks/api/data_source.py` & `sageworks-0.5.4/src/sageworks/api/data_source.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.3/src/sageworks/api/endpoint.py` & `sageworks-0.5.4/src/sageworks/api/endpoint.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.3/src/sageworks/api/feature_set.py` & `sageworks-0.5.4/src/sageworks/api/feature_set.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.3/src/sageworks/api/meta.py` & `sageworks-0.5.4/src/sageworks/api/meta.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.3/src/sageworks/api/model.py` & `sageworks-0.5.4/src/sageworks/api/model.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.3/src/sageworks/api/monitor.py` & `sageworks-0.5.4/src/sageworks/api/monitor.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.3/src/sageworks/aws_service_broker/aws_account_clamp.py` & `sageworks-0.5.4/src/sageworks/aws_service_broker/aws_account_clamp.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.3/src/sageworks/aws_service_broker/aws_service_broker.py` & `sageworks-0.5.4/src/sageworks/aws_service_broker/aws_service_broker.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.3/src/sageworks/aws_service_broker/aws_service_connectors/connector.py` & `sageworks-0.5.4/src/sageworks/aws_service_broker/aws_service_connectors/connector.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.3/src/sageworks/aws_service_broker/aws_service_connectors/data_catalog.py` & `sageworks-0.5.4/src/sageworks/aws_service_broker/aws_service_connectors/data_catalog.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.3/src/sageworks/aws_service_broker/aws_service_connectors/endpoints.py` & `sageworks-0.5.4/src/sageworks/aws_service_broker/aws_service_connectors/endpoints.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.3/src/sageworks/aws_service_broker/aws_service_connectors/feature_store.py` & `sageworks-0.5.4/src/sageworks/aws_service_broker/aws_service_connectors/feature_store.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.3/src/sageworks/aws_service_broker/aws_service_connectors/glue_jobs.py` & `sageworks-0.5.4/src/sageworks/aws_service_broker/aws_service_connectors/glue_jobs.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.3/src/sageworks/aws_service_broker/aws_service_connectors/model_registry.py` & `sageworks-0.5.4/src/sageworks/aws_service_broker/aws_service_connectors/model_registry.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.3/src/sageworks/aws_service_broker/aws_service_connectors/s3_bucket.py` & `sageworks-0.5.4/src/sageworks/aws_service_broker/aws_service_connectors/s3_bucket.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.3/src/sageworks/core/artifacts/__init__.py` & `sageworks-0.5.4/src/sageworks/core/artifacts/__init__.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.3/src/sageworks/core/artifacts/artifact.py` & `sageworks-0.5.4/src/sageworks/core/artifacts/artifact.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.3/src/sageworks/core/artifacts/athena_source.py` & `sageworks-0.5.4/src/sageworks/core/artifacts/athena_source.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.3/src/sageworks/core/artifacts/data_source_abstract.py` & `sageworks-0.5.4/src/sageworks/core/artifacts/data_source_abstract.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.3/src/sageworks/core/artifacts/data_source_factory.py` & `sageworks-0.5.4/src/sageworks/core/artifacts/data_source_factory.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.3/src/sageworks/core/artifacts/endpoint_core.py` & `sageworks-0.5.4/src/sageworks/core/artifacts/endpoint_core.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.3/src/sageworks/core/artifacts/feature_set_core.py` & `sageworks-0.5.4/src/sageworks/core/artifacts/feature_set_core.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.3/src/sageworks/core/artifacts/model_core.py` & `sageworks-0.5.4/src/sageworks/core/artifacts/model_core.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.3/src/sageworks/core/artifacts/monitor_core.py` & `sageworks-0.5.4/src/sageworks/core/artifacts/monitor_core.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.3/src/sageworks/core/transforms/Readme.md` & `sageworks-0.5.4/src/sageworks/core/transforms/Readme.md`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.3/src/sageworks/core/transforms/data_loaders/heavy/s3_heavy_to_data_source.py` & `sageworks-0.5.4/src/sageworks/core/transforms/data_loaders/heavy/s3_heavy_to_data_source.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.3/src/sageworks/core/transforms/data_loaders/light/__init__.py` & `sageworks-0.5.4/src/sageworks/core/transforms/data_loaders/light/__init__.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.3/src/sageworks/core/transforms/data_loaders/light/csv_to_data_source.py` & `sageworks-0.5.4/src/sageworks/core/transforms/data_loaders/light/csv_to_data_source.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.3/src/sageworks/core/transforms/data_loaders/light/json_to_data_source.py` & `sageworks-0.5.4/src/sageworks/core/transforms/data_loaders/light/json_to_data_source.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.3/src/sageworks/core/transforms/data_loaders/light/s3_to_data_source_light.py` & `sageworks-0.5.4/src/sageworks/core/transforms/data_loaders/light/s3_to_data_source_light.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.3/src/sageworks/core/transforms/data_to_data/light/clean_data.py` & `sageworks-0.5.4/src/sageworks/core/transforms/data_to_data/light/clean_data.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.3/src/sageworks/core/transforms/data_to_data/light/data_to_data_light.py` & `sageworks-0.5.4/src/sageworks/core/transforms/data_to_data/light/data_to_data_light.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.3/src/sageworks/core/transforms/data_to_features/heavy/chunk/data_to_features_chunk.py` & `sageworks-0.5.4/src/sageworks/core/transforms/data_to_features/heavy/chunk/data_to_features_chunk.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.3/src/sageworks/core/transforms/data_to_features/heavy/storage/data_to_features_heavy_old.py` & `sageworks-0.5.4/src/sageworks/core/transforms/data_to_features/heavy/storage/data_to_features_heavy_old.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.3/src/sageworks/core/transforms/data_to_features/light/data_to_features_light.py` & `sageworks-0.5.4/src/sageworks/core/transforms/data_to_features/light/data_to_features_light.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.3/src/sageworks/core/transforms/data_to_features/light/molecular_descriptors.py` & `sageworks-0.5.4/src/sageworks/core/transforms/data_to_features/light/molecular_descriptors.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.3/src/sageworks/core/transforms/features_to_model/features_to_model.py` & `sageworks-0.5.4/src/sageworks/core/transforms/features_to_model/features_to_model.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.3/src/sageworks/core/transforms/features_to_model/light_model_harness/xgb_model.template` & `sageworks-0.5.4/src/sageworks/core/transforms/features_to_model/light_model_harness/xgb_model.template`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.3/src/sageworks/core/transforms/model_to_endpoint/model_to_endpoint.py` & `sageworks-0.5.4/src/sageworks/core/transforms/model_to_endpoint/model_to_endpoint.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.3/src/sageworks/core/transforms/pandas_transforms/__init__.py` & `sageworks-0.5.4/src/sageworks/core/transforms/pandas_transforms/__init__.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.3/src/sageworks/core/transforms/pandas_transforms/data_to_pandas.py` & `sageworks-0.5.4/src/sageworks/core/transforms/pandas_transforms/data_to_pandas.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.3/src/sageworks/core/transforms/pandas_transforms/features_to_pandas.py` & `sageworks-0.5.4/src/sageworks/core/transforms/pandas_transforms/features_to_pandas.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.3/src/sageworks/core/transforms/pandas_transforms/pandas_to_data.py` & `sageworks-0.5.4/src/sageworks/core/transforms/pandas_transforms/pandas_to_data.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.3/src/sageworks/core/transforms/pandas_transforms/pandas_to_features.py` & `sageworks-0.5.4/src/sageworks/core/transforms/pandas_transforms/pandas_to_features.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.3/src/sageworks/core/transforms/pandas_transforms/pandas_to_features_chunked.py` & `sageworks-0.5.4/src/sageworks/core/transforms/pandas_transforms/pandas_to_features_chunked.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.3/src/sageworks/core/transforms/transform.py` & `sageworks-0.5.4/src/sageworks/core/transforms/transform.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.3/src/sageworks/experiments/view_manager.py` & `sageworks-0.5.4/src/sageworks/experiments/view_manager.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.3/src/sageworks/repl/sageworks_shell.py` & `sageworks-0.5.4/src/sageworks/repl/sageworks_shell.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.3/src/sageworks/utils/aws_utils.py` & `sageworks-0.5.4/src/sageworks/utils/aws_utils.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.3/src/sageworks/utils/cache.py` & `sageworks-0.5.4/src/sageworks/utils/cache.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.3/src/sageworks/utils/chem_utils.py` & `sageworks-0.5.4/src/sageworks/utils/chem_utils.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.3/src/sageworks/utils/config_manager.py` & `sageworks-0.5.4/src/sageworks/utils/config_manager.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.3/src/sageworks/utils/dashboard_metrics.py` & `sageworks-0.5.4/src/sageworks/utils/dashboard_metrics.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.3/src/sageworks/utils/datetime_utils.py` & `sageworks-0.5.4/src/sageworks/utils/datetime_utils.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.3/src/sageworks/utils/df_to_endpoint.py` & `sageworks-0.5.4/src/sageworks/utils/df_to_endpoint.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.3/src/sageworks/utils/docker_utils.py` & `sageworks-0.5.4/src/sageworks/utils/docker_utils.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.3/src/sageworks/utils/ecs_info.py` & `sageworks-0.5.4/src/sageworks/utils/ecs_info.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.3/src/sageworks/utils/endpoint_metrics.py` & `sageworks-0.5.4/src/sageworks/utils/endpoint_metrics.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.3/src/sageworks/utils/endpoint_utils.py` & `sageworks-0.5.4/src/sageworks/utils/endpoint_utils.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.3/src/sageworks/utils/extract_model_artifact.py` & `sageworks-0.5.4/src/sageworks/utils/extract_model_artifact.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.3/src/sageworks/utils/glue_utils.py` & `sageworks-0.5.4/src/sageworks/utils/glue_utils.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.3/src/sageworks/utils/license_manager.py` & `sageworks-0.5.4/src/sageworks/utils/license_manager.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.3/src/sageworks/utils/markdown_utils.py` & `sageworks-0.5.4/src/sageworks/utils/markdown_utils.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.3/src/sageworks/utils/pandas_utils.py` & `sageworks-0.5.4/src/sageworks/utils/pandas_utils.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.3/src/sageworks/utils/plugin_manager.py` & `sageworks-0.5.4/src/sageworks/utils/plugin_manager.py`

 * *Files 4% similar despite different names*

```diff
@@ -33,15 +33,15 @@
         if self.__initialized:
             return
 
         self.log = logging.getLogger("sageworks")
         self.config_plugin_dir = None
         self.loading_dir = False
         self.plugin_modified_time = None
-        self.plugins: Dict[str, dict] = {"web_components": {}, "transforms": {}, "views": {}, "pages": {}}
+        self.plugins: Dict[str, dict] = {"web_components": {}, "transforms": {}, "views": {}, "pages": {}, "css": {}}
 
         # Get the plugin directory from the config
         cm = ConfigManager()
         self.config_plugin_dir = cm.get_config("SAGEWORKS_PLUGINS")
         if not self.config_plugin_dir:
             self.log.warning("SAGEWORKS_PLUGINS not set. No plugins will be loaded.")
             return
@@ -111,14 +111,29 @@
                                     f"Class {attr_name} in {filename} does not have all required page methods"
                                 )
 
                         # Unexpected type
                         else:
                             self.log.warning(f"Class {attr_name} in {filename} invalid {plugin_type} plugin")
 
+            # Check for CSS files
+            else:
+                # For CSS, check if the file ends with .css
+                if plugin_type == "css":
+                    if filename.endswith(".css"):
+                        self.log.important(f"Storing {plugin_type} plugin: {filename}")
+                        # Basename of the filename without the extension
+                        basename = os.path.splitext(filename)[0]
+
+                        # Full path to the CSS file
+                        fullpath = os.path.join(type_dir, filename)
+                        self.plugins[plugin_type][basename] = fullpath
+                    else:
+                        self.log.warning(f"{fullpath} is not a CSS file")
+
     @staticmethod
     def _load_module(dir_path: str, filename: str):
         """Internal: Load a module from a file"""
         if filename.endswith(".py") and not filename.startswith("_"):
             file_path = os.path.join(dir_path, filename)
             module_name = filename[:-3]
             spec = importlib.util.spec_from_file_location(module_name, file_path)
@@ -188,14 +203,24 @@
 
         Returns:
            dict: A dict of INSTANTIATED plugin pages.
         """
         pages = self.plugins["pages"]
         return {name: page() for name, page in pages.items()}
 
+    def get_css_files(self) -> List[str]:
+        """
+        Retrieve a list of CSS files
+
+        Returns:
+            List[str]: A list of CSS files
+        """
+        css_files = list(self.plugins["css"].values())
+        return css_files
+
     def _cleanup_temp_dir(self):
         """Cleans up the temporary directory created for S3 files."""
         if self.loading_dir and os.path.isdir(self.loading_dir):
             self.log.important(f"Cleaning up temporary directory: {self.loading_dir}")
             shutil.rmtree(self.loading_dir)
             self.loading_dir = None
 
@@ -265,37 +290,42 @@
     print(my_plugin)
 
     # Test REPR
     print(manager)
 
     # Test Modified Time by modifying a plugin file
     cm = ConfigManager()
-    plugin_path = cm.get_config("SAGEWORKS_PLUGINS") + "/web_components/custom_turbo.py"
+    plugin_path = cm.get_config("SAGEWORKS_PLUGINS") + "/web_components/model_plugin.py"
     print(manager.plugins_modified())
     # Modify the plugin file modified time to now
     os.utime(plugin_path, None)
     print(manager.plugins_modified())
 
     # Test S3 Plugin Loading
+    """
     print("\n\n*** Testing S3 Plugin Loading ***\n\n")
     s3_path = "s3://sandbox-sageworks-artifacts/sageworks_plugins"
     cm = ConfigManager()
     cm.set_config("SAGEWORKS_PLUGINS", s3_path)
 
     # Since we're using a singleton, we need to create a new instance
     PluginManager._instance = None
     manager = PluginManager()
+    """
 
     # Get web components for the model view
     model_plugin = manager.get_list_of_web_plugins(PluginPage.MODEL)
 
     # Get web components for the endpoint view
     endpoint_plugin = manager.get_list_of_web_plugins(PluginPage.ENDPOINT)
 
     # Get view plugin
     my_view = manager.get_view("ModelPluginView")
 
     # Get plugin pages
     plugin_pages = manager.get_pages()
 
+    # Get css files
+    plugin_pages = manager.get_css_files()
+
     # Get all the plugins
     pprint(manager.get_all_plugins())
```

### Comparing `sageworks-0.5.3/src/sageworks/utils/redis_cache.py` & `sageworks-0.5.4/src/sageworks/utils/redis_cache.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.3/src/sageworks/utils/repl_utils.py` & `sageworks-0.5.4/src/sageworks/utils/repl_utils.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.3/src/sageworks/utils/s3_utils.py` & `sageworks-0.5.4/src/sageworks/utils/s3_utils.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.3/src/sageworks/utils/sageworks_cache.py` & `sageworks-0.5.4/src/sageworks/utils/sageworks_cache.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.3/src/sageworks/utils/sageworks_event_bridge.py` & `sageworks-0.5.4/src/sageworks/utils/sageworks_event_bridge.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.3/src/sageworks/utils/sageworks_logging.py` & `sageworks-0.5.4/src/sageworks/utils/sageworks_logging.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.3/src/sageworks/utils/sageworks_sqs.py` & `sageworks-0.5.4/src/sageworks/utils/sageworks_sqs.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.3/src/sageworks/utils/symbols.py` & `sageworks-0.5.4/src/sageworks/utils/symbols.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.3/src/sageworks/utils/test_data_generator.py` & `sageworks-0.5.4/src/sageworks/utils/test_data_generator.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.3/src/sageworks/utils/trace_calls.py` & `sageworks-0.5.4/src/sageworks/utils/trace_calls.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.3/src/sageworks/utils/type_abbrev.py` & `sageworks-0.5.4/src/sageworks/utils/type_abbrev.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.3/src/sageworks/views/artifacts_text_view.py` & `sageworks-0.5.4/src/sageworks/views/artifacts_text_view.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.3/src/sageworks/views/artifacts_web_view.py` & `sageworks-0.5.4/src/sageworks/views/artifacts_web_view.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.3/src/sageworks/views/data_source_web_view.py` & `sageworks-0.5.4/src/sageworks/views/data_source_web_view.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.3/src/sageworks/views/endpoint_web_view.py` & `sageworks-0.5.4/src/sageworks/views/endpoint_web_view.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.3/src/sageworks/views/feature_set_web_view.py` & `sageworks-0.5.4/src/sageworks/views/feature_set_web_view.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.3/src/sageworks/views/model_web_view.py` & `sageworks-0.5.4/src/sageworks/views/model_web_view.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.3/src/sageworks/views/view.py` & `sageworks-0.5.4/src/sageworks/views/view.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.3/src/sageworks/web_components/color_maps.py` & `sageworks-0.5.4/src/sageworks/web_components/color_maps.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.3/src/sageworks/web_components/component_interface.py` & `sageworks-0.5.4/src/sageworks/web_components/component_interface.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.3/src/sageworks/web_components/confusion_matrix.py` & `sageworks-0.5.4/src/sageworks/web_components/confusion_matrix.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.3/src/sageworks/web_components/correlation_matrix.py` & `sageworks-0.5.4/src/sageworks/web_components/correlation_matrix.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.3/src/sageworks/web_components/dashboard_metric_plots.py` & `sageworks-0.5.4/src/sageworks/web_components/dashboard_metric_plots.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.3/src/sageworks/web_components/data_details_markdown.py` & `sageworks-0.5.4/src/sageworks/web_components/data_details_markdown.py`

 * *Files 0% similar despite different names*

```diff
@@ -235,8 +235,8 @@
     # Initialize Dash app
     app = dash.Dash(__name__)
 
     app.layout = html.Div([component])
     component.children = markdown
 
     if __name__ == "__main__":
-        app.run_server(debug=True)
+        app.run(debug=True)
```

### Comparing `sageworks-0.5.3/src/sageworks/web_components/endpoint_details.py` & `sageworks-0.5.4/src/sageworks/web_components/endpoint_details.py`

 * *Files 1% similar despite different names*

```diff
@@ -126,8 +126,8 @@
     app = dash.Dash(
         __name__,
         external_stylesheets=[dbc.themes.DARKLY],
         assets_folder="/Users/briford/work/sageworks/applications/aws_dashboard/assets",
     )
 
     app.layout = html.Div([endpoints_table, details_component])
-    app.run_server(debug=True)
+    app.run(debug=True)
```

### Comparing `sageworks-0.5.3/src/sageworks/web_components/endpoint_metric_plots.py` & `sageworks-0.5.4/src/sageworks/web_components/endpoint_metric_plots.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.3/src/sageworks/web_components/experiments/compound_details.py` & `sageworks-0.5.4/src/sageworks/web_components/experiments/compound_details.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.3/src/sageworks/web_components/experiments/histogram.py` & `sageworks-0.5.4/src/sageworks/web_components/experiments/histogram.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.3/src/sageworks/web_components/experiments/outlier_plot.py` & `sageworks-0.5.4/src/sageworks/web_components/experiments/outlier_plot.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.3/src/sageworks/web_components/experiments/scatter_plot.py` & `sageworks-0.5.4/src/sageworks/web_components/experiments/scatter_plot.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.3/src/sageworks/web_components/line_chart.py` & `sageworks-0.5.4/src/sageworks/web_components/line_chart.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.3/src/sageworks/web_components/model_details.py` & `sageworks-0.5.4/src/sageworks/web_components/model_details.py`

 * *Files 1% similar despite different names*

```diff
@@ -211,34 +211,33 @@
     import dash
     import dash_bootstrap_components as dbc
     from sageworks.web_components.table import Table
     from sageworks.api.meta import Meta
 
     # Create a model table
     models_table = Table().create_component(
-        "models_table", header_color="rgb(60, 100, 60)", row_select="single", max_height=270
+        "my_models_table", header_color="rgb(60, 100, 60)", row_select="single", max_height=270
     )
 
     # Populate the table with data
     models = Meta().models()
     models["uuid"] = models["Model Group"]
     models["id"] = range(len(models))
     column_setup_list = Table().column_setup(models)
     models_table.columns = column_setup_list
     models_table.data = models.to_dict("records")
 
     # Instantiate the ModelDetails class
     md = ModelDetails()
-    details_component = md.create_component("model_details")
+    details_component = md.create_component("my_model_details")
 
     # Register the callbacks
-    md.register_callbacks("models_table")
+    md.register_callbacks("my_models_table")
 
     # Initialize Dash app
     app = dash.Dash(
         __name__,
         external_stylesheets=[dbc.themes.DARKLY],
-        assets_folder="/Users/briford/work/sageworks/applications/aws_dashboard/assets",
     )
 
     app.layout = html.Div([models_table, details_component])
-    app.run_server(debug=True)
+    app.run(debug=True)
```

### Comparing `sageworks-0.5.3/src/sageworks/web_components/model_plot.py` & `sageworks-0.5.4/src/sageworks/web_components/model_plot.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.3/src/sageworks/web_components/plugin_interface.py` & `sageworks-0.5.4/src/sageworks/web_components/plugin_interface.py`

 * *Files 0% similar despite different names*

```diff
@@ -44,15 +44,17 @@
             component_id (str): The ID of the web component
         Returns:
             Union[dcc.Graph, dash_table.DataTable, dcc.Markdown, html.Div] The Dash Web component
         """
         pass
 
     @abstractmethod
-    def update_contents(self, data_object: ComponentInterface.SageworksObject) -> ComponentInterface.ContentTypes:
+    def update_contents(
+        self, data_object: ComponentInterface.SageworksObject, **kwargs
+    ) -> ComponentInterface.ContentTypes:
         """Generate a figure from the data in the given dataframe.
         Args:
             data_object (sageworks_object): The instantiated data object for the plugin type.
         Returns:
             Union[go.Figure, str]: A Plotly Figure or a Markdown string
         """
         pass
```

### Comparing `sageworks-0.5.3/src/sageworks/web_components/regression_plot.py` & `sageworks-0.5.4/src/sageworks/web_components/regression_plot.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.3/src/sageworks/web_components/table.py` & `sageworks-0.5.4/src/sageworks/web_components/table.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.3/src/sageworks/web_components/violin_plots.py` & `sageworks-0.5.4/src/sageworks/web_components/violin_plots.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.3/src/sageworks.egg-info/PKG-INFO` & `sageworks-0.5.4/src/sageworks.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sageworks
-Version: 0.5.3
+Version: 0.5.4
 Summary: SageWorks: A Python WorkBench for creating and deploying AWS SageMaker Models
 Home-page: https://github.com/SuperCowPowers/sageworks
 Author: SuperCowPowers LLC
 Author-email: support@supercowpowers.com
 License: MIT
 Keywords: SageMaker,Machine Learning,AWS,Python,Utilities
 Classifier: Development Status :: 4 - Beta
```

### Comparing `sageworks-0.5.3/src/sageworks.egg-info/SOURCES.txt` & `sageworks-0.5.4/src/sageworks.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -19,15 +19,16 @@
 applications/aws_dashboard/README.md
 applications/aws_dashboard/app.py
 applications/aws_dashboard/dashboard
 applications/aws_dashboard/nginx.conf
 applications/aws_dashboard/open_source_config.json
 applications/aws_dashboard/requirements.txt
 applications/aws_dashboard/supervisord.conf
-applications/aws_dashboard/assets/custom.css
+applications/aws_dashboard/assets/bootstrap_darkly.min.css
+applications/aws_dashboard/assets/default.css
 applications/aws_dashboard/assets/favicon.ico
 applications/aws_dashboard/assets/trash.png
 applications/aws_dashboard/pages/data_sources/callbacks.py
 applications/aws_dashboard/pages/data_sources/layout.py
 applications/aws_dashboard/pages/data_sources/page.py
 applications/aws_dashboard/pages/endpoints/callbacks.py
 applications/aws_dashboard/pages/endpoints/layout.py
@@ -167,16 +168,22 @@
 examples/meta_model_metrics.py
 examples/model_metrics.py
 examples/model_to_endpoint.py
 examples/monitor_setup.py
 examples/monitor_usage.py
 examples/ag-grid/hello_world.py
 examples/plugins/pages/my_plugin_page.py
+examples/plugins/pages/plugin_page_1.py
+examples/plugins/pages/plugin_page_2.py
+examples/plugins/pages/plugin_page_3.py
+examples/plugins/views/model_plugin_view.py
 examples/plugins/views/my_view_plugin.py
+examples/plugins/web_components/custom_plugin.py
 examples/plugins/web_components/endpoint_plugin.py
+examples/plugins/web_components/endpoint_turbo.py
 examples/plugins/web_components/model_plugin.py
 examples/sagemaker_pipelines/all_steps.py
 examples/sagemaker_pipelines/hello.py
 examples/sagemaker_pipelines/ml_pipeline.py
 examples/sagemaker_pipelines/storage/full_pipeline_experiment/data_source.py
 examples/sagemaker_pipelines/storage/full_pipeline_experiment/endpoint.py
 examples/sagemaker_pipelines/storage/full_pipeline_experiment/feature_set.py
```

### Comparing `sageworks-0.5.3/tests/artifacts/data_source_tests.py` & `sageworks-0.5.4/tests/artifacts/data_source_tests.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.3/tests/artifacts/endpoint_tests.py` & `sageworks-0.5.4/tests/artifacts/endpoint_tests.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.3/tests/artifacts/feature_set_tests.py` & `sageworks-0.5.4/tests/artifacts/feature_set_tests.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.3/tests/artifacts/model_tests.py` & `sageworks-0.5.4/tests/artifacts/model_tests.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.3/tests/aws_account/aws_account_clamp_tests.py` & `sageworks-0.5.4/tests/aws_account/aws_account_clamp_tests.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.3/tests/aws_account/aws_service_broker_tests.py` & `sageworks-0.5.4/tests/aws_account/aws_service_broker_tests.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.3/tests/connectors/data_catalog.py` & `sageworks-0.5.4/tests/connectors/data_catalog.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.3/tests/connectors/endpoints.py` & `sageworks-0.5.4/tests/connectors/endpoints.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.3/tests/connectors/feature_store.py` & `sageworks-0.5.4/tests/connectors/feature_store.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.3/tests/connectors/glue_jobs.py` & `sageworks-0.5.4/tests/connectors/glue_jobs.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.3/tests/connectors/model_registry.py` & `sageworks-0.5.4/tests/connectors/model_registry.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.3/tests/connectors/s3_bucket.py` & `sageworks-0.5.4/tests/connectors/s3_bucket.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.3/tests/create_aqsol_artifacts.py` & `sageworks-0.5.4/tests/create_aqsol_artifacts.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.3/tests/create_basic_test_artifacts.py` & `sageworks-0.5.4/tests/create_basic_test_artifacts.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.3/tests/create_realtime_endpoint.py` & `sageworks-0.5.4/tests/create_realtime_endpoint.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.3/tests/create_training_adjusted_artifacts.py` & `sageworks-0.5.4/tests/create_training_adjusted_artifacts.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.3/tests/create_wine_artifacts.py` & `sageworks-0.5.4/tests/create_wine_artifacts.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.3/tests/delete_test_artifacts.py` & `sageworks-0.5.4/tests/delete_test_artifacts.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.3/tests/plugin_tests/crashing_plugin.py` & `sageworks-0.5.4/tests/plugin_tests/crashing_plugin.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.3/tests/specific/capital_tests.py` & `sageworks-0.5.4/tests/specific/capital_tests.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.3/tests/specific/deletion_tests.py` & `sageworks-0.5.4/tests/specific/deletion_tests.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.3/tests/transforms/data_to_data_tests.py` & `sageworks-0.5.4/tests/transforms/data_to_data_tests.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.3/tests/transforms/data_to_features_tests.py` & `sageworks-0.5.4/tests/transforms/data_to_features_tests.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.3/tests/transforms/features_to_model_tests.py` & `sageworks-0.5.4/tests/transforms/features_to_model_tests.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.3/tests/transforms/model_metrics_tests.py` & `sageworks-0.5.4/tests/transforms/model_metrics_tests.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.3/tests/transforms/model_to_endpoint_tests.py` & `sageworks-0.5.4/tests/transforms/model_to_endpoint_tests.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.3/tests/transforms/pandas_to_data_tests.py` & `sageworks-0.5.4/tests/transforms/pandas_to_data_tests.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.3/tests/web_components/confusion_matrix_test.py` & `sageworks-0.5.4/tests/web_components/confusion_matrix_test.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.3/tests/web_components/correlation_matrix_test.py` & `sageworks-0.5.4/tests/web_components/correlation_matrix_test.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.3/tests/web_components/plugin_interface_test.py` & `sageworks-0.5.4/tests/web_components/plugin_interface_test.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.5.3/tox.ini` & `sageworks-0.5.4/tox.ini`

 * *Files identical despite different names*

