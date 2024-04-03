# Comparing `tmp/EclipsingBinaries-4.0.6.tar.gz` & `tmp/EclipsingBinaries-4.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "EclipsingBinaries-4.0.6.tar", last modified: Tue Feb 13 17:42:08 2024, max compression
+gzip compressed data, was "EclipsingBinaries-4.0.7.tar", last modified: Wed Apr  3 21:13:15 2024, max compression
```

## Comparing `EclipsingBinaries-4.0.6.tar` & `EclipsingBinaries-4.0.7.tar`

### file list

```diff
@@ -1,90 +1,90 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 17:42:08.031850 EclipsingBinaries-4.0.6/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 17:42:08.015850 EclipsingBinaries-4.0.6/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 17:42:08.015850 EclipsingBinaries-4.0.6/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (127)      856 2024-02-13 17:41:48.000000 EclipsingBinaries-4.0.6/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (127)      597 2024-02-13 17:41:48.000000 EclipsingBinaries-4.0.6/.github/ISSUE_TEMPLATE/feature_request.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 17:42:08.015850 EclipsingBinaries-4.0.6/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     3190 2024-02-13 17:41:48.000000 EclipsingBinaries-4.0.6/.github/workflows/ci_tests.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2778 2024-02-13 17:41:48.000000 EclipsingBinaries-4.0.6/.github/workflows/codeql.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1204 2024-02-13 17:41:48.000000 EclipsingBinaries-4.0.6/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)      404 2024-02-13 17:41:48.000000 EclipsingBinaries-4.0.6/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (127)   103415 2024-02-13 17:41:48.000000 EclipsingBinaries-4.0.6/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)     5234 2024-02-13 17:41:48.000000 EclipsingBinaries-4.0.6/CODE_OF_CONDUCT.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 17:42:08.019851 EclipsingBinaries-4.0.6/EclipsingBinaries/
--rw-r--r--   0 runner    (1001) docker     (127)    24369 2024-02-13 17:41:48.000000 EclipsingBinaries-4.0.6/EclipsingBinaries/IRAF_Reduction.py
--rw-r--r--   0 runner    (1001) docker     (127)     8436 2024-02-13 17:41:48.000000 EclipsingBinaries-4.0.6/EclipsingBinaries/Night_Filters.py
--rw-r--r--   0 runner    (1001) docker     (127)    20913 2024-02-13 17:41:48.000000 EclipsingBinaries-4.0.6/EclipsingBinaries/OC_plot.py
--rw-r--r--   0 runner    (1001) docker     (127)    22282 2024-02-13 17:41:48.000000 EclipsingBinaries-4.0.6/EclipsingBinaries/OConnell.py
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-02-13 17:41:48.000000 EclipsingBinaries-4.0.6/EclipsingBinaries/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    19927 2024-02-13 17:41:48.000000 EclipsingBinaries-4.0.6/EclipsingBinaries/apass.py
--rw-r--r--   0 runner    (1001) docker     (127)    30766 2024-02-13 17:41:48.000000 EclipsingBinaries-4.0.6/EclipsingBinaries/color_light_curve.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 17:42:08.027850 EclipsingBinaries-4.0.6/EclipsingBinaries/examples/
--rw-r--r--   0 runner    (1001) docker     (127)     2293 2024-02-13 17:41:48.000000 EclipsingBinaries-4.0.6/EclipsingBinaries/examples/APASS_Catalog_ex.txt
--rw-r--r--   0 runner    (1001) docker     (127)      314 2024-02-13 17:41:48.000000 EclipsingBinaries-4.0.6/EclipsingBinaries/examples/Gaia_output.txt
--rw-r--r--   0 runner    (1001) docker     (127)      968 2024-02-13 17:41:48.000000 EclipsingBinaries-4.0.6/EclipsingBinaries/examples/O-C_paper_table.txt
--rw-r--r--   0 runner    (1001) docker     (127)    85904 2024-02-13 17:41:48.000000 EclipsingBinaries-4.0.6/EclipsingBinaries/examples/OConnell_plot.png
--rw-r--r--   0 runner    (1001) docker     (127)     1009 2024-02-13 17:41:48.000000 EclipsingBinaries-4.0.6/EclipsingBinaries/examples/OConnell_table.txt
--rw-r--r--   0 runner    (1001) docker     (127)    48237 2024-02-13 17:41:48.000000 EclipsingBinaries-4.0.6/EclipsingBinaries/examples/O_C_ex.png
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-13 17:41:48.000000 EclipsingBinaries-4.0.6/EclipsingBinaries/examples/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 17:42:08.027850 EclipsingBinaries-4.0.6/EclipsingBinaries/examples/calibration_images/
--rw-r--r--   0 runner    (1001) docker     (127)      125 2024-02-13 17:41:52.000000 EclipsingBinaries-4.0.6/EclipsingBinaries/examples/calibration_images/purpose.txt
--rw-r--r--   0 runner    (1001) docker     (127)   135237 2024-02-13 17:41:52.000000 EclipsingBinaries-4.0.6/EclipsingBinaries/examples/color_light_curve_ex.png
--rw-r--r--   0 runner    (1001) docker     (127)    35357 2024-02-13 17:41:52.000000 EclipsingBinaries-4.0.6/EclipsingBinaries/examples/example_OC_table.txt
--rw-r--r--   0 runner    (1001) docker     (127)     4442 2024-02-13 17:41:52.000000 EclipsingBinaries-4.0.6/EclipsingBinaries/examples/example_regression.txt
--rw-r--r--   0 runner    (1001) docker     (127)   118184 2024-02-13 17:41:52.000000 EclipsingBinaries-4.0.6/EclipsingBinaries/examples/gui_color_light.png
--rw-r--r--   0 runner    (1001) docker     (127)   109712 2024-02-13 17:41:52.000000 EclipsingBinaries-4.0.6/EclipsingBinaries/examples/light_curve_ex.png
--rw-r--r--   0 runner    (1001) docker     (127)   136591 2024-02-13 17:41:53.000000 EclipsingBinaries-4.0.6/EclipsingBinaries/examples/min_program_demo.png
--rw-r--r--   0 runner    (1001) docker     (127)   131114 2024-02-13 17:41:53.000000 EclipsingBinaries-4.0.6/EclipsingBinaries/examples/overlay_example.png
--rw-r--r--   0 runner    (1001) docker     (127)    31361 2024-02-13 17:41:53.000000 EclipsingBinaries-4.0.6/EclipsingBinaries/examples/test_B.txt
--rw-r--r--   0 runner    (1001) docker     (127)    25814 2024-02-13 17:41:53.000000 EclipsingBinaries-4.0.6/EclipsingBinaries/examples/test_R.txt
--rw-r--r--   0 runner    (1001) docker     (127)    30132 2024-02-13 17:41:53.000000 EclipsingBinaries-4.0.6/EclipsingBinaries/examples/test_V.txt
--rw-r--r--   0 runner    (1001) docker     (127)    39669 2024-02-13 17:41:53.000000 EclipsingBinaries-4.0.6/EclipsingBinaries/examples/test_minimums.txt
--rw-r--r--   0 runner    (1001) docker     (127)    25259 2024-02-13 17:41:53.000000 EclipsingBinaries-4.0.6/EclipsingBinaries/find_min.py
--rw-r--r--   0 runner    (1001) docker     (127)     7284 2024-02-13 17:41:53.000000 EclipsingBinaries-4.0.6/EclipsingBinaries/gaia.py
--rw-r--r--   0 runner    (1001) docker     (127)     3458 2024-02-13 17:41:53.000000 EclipsingBinaries-4.0.6/EclipsingBinaries/menu.py
--rw-r--r--   0 runner    (1001) docker     (127)    16127 2024-02-13 17:41:53.000000 EclipsingBinaries-4.0.6/EclipsingBinaries/multi_aperture_photometry.py
--rw-r--r--   0 runner    (1001) docker     (127)     3680 2024-02-13 17:41:53.000000 EclipsingBinaries-4.0.6/EclipsingBinaries/pipeline.py
--rw-r--r--   0 runner    (1001) docker     (127)     2502 2024-02-13 17:41:53.000000 EclipsingBinaries-4.0.6/EclipsingBinaries/tess_ccd_info.txt
--rw-r--r--   0 runner    (1001) docker     (127)     5623 2024-02-13 17:41:53.000000 EclipsingBinaries-4.0.6/EclipsingBinaries/tess_data_search.py
--rw-r--r--   0 runner    (1001) docker     (127)     4787 2024-02-13 17:41:53.000000 EclipsingBinaries-4.0.6/EclipsingBinaries/tesscut.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 17:42:08.027850 EclipsingBinaries-4.0.6/EclipsingBinaries/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        2 2024-02-13 17:41:53.000000 EclipsingBinaries-4.0.6/EclipsingBinaries/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      564 2024-02-13 17:41:53.000000 EclipsingBinaries-4.0.6/EclipsingBinaries/tests/test_OC_plot.py
--rw-r--r--   0 runner    (1001) docker     (127)    14791 2024-02-13 17:41:53.000000 EclipsingBinaries-4.0.6/EclipsingBinaries/tests/test_apass.py
--rw-r--r--   0 runner    (1001) docker     (127)    90297 2024-02-13 17:41:53.000000 EclipsingBinaries-4.0.6/EclipsingBinaries/vseq_updated.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 17:42:08.031850 EclipsingBinaries-4.0.6/EclipsingBinaries.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3845 2024-02-13 17:42:03.000000 EclipsingBinaries-4.0.6/EclipsingBinaries.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2435 2024-02-13 17:42:08.000000 EclipsingBinaries-4.0.6/EclipsingBinaries.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-13 17:42:03.000000 EclipsingBinaries-4.0.6/EclipsingBinaries.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      125 2024-02-13 17:42:03.000000 EclipsingBinaries-4.0.6/EclipsingBinaries.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-13 17:42:03.000000 EclipsingBinaries-4.0.6/EclipsingBinaries.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      249 2024-02-13 17:42:03.000000 EclipsingBinaries-4.0.6/EclipsingBinaries.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-02-13 17:42:03.000000 EclipsingBinaries-4.0.6/EclipsingBinaries.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-02-13 17:41:53.000000 EclipsingBinaries-4.0.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      161 2024-02-13 17:41:53.000000 EclipsingBinaries-4.0.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     3845 2024-02-13 17:42:08.031850 EclipsingBinaries-4.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2991 2024-02-13 17:41:53.000000 EclipsingBinaries-4.0.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 17:42:08.027850 EclipsingBinaries-4.0.6/changelog/
--rw-r--r--   0 runner    (1001) docker     (127)   222548 2024-02-13 17:41:53.000000 EclipsingBinaries-4.0.6/changelog/package-lock.json
--rw-r--r--   0 runner    (1001) docker     (127)     1347 2024-02-13 17:41:53.000000 EclipsingBinaries-4.0.6/changelog/package.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 17:42:08.027850 EclipsingBinaries-4.0.6/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      286 2024-02-13 17:41:53.000000 EclipsingBinaries-4.0.6/docs/EB.rst
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-13 17:41:53.000000 EclipsingBinaries-4.0.6/docs/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 17:42:08.015850 EclipsingBinaries-4.0.6/docs/_templates/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 17:42:08.031850 EclipsingBinaries-4.0.6/docs/_templates/autosummary/
--rw-r--r--   0 runner    (1001) docker     (127)      251 2024-02-13 17:41:53.000000 EclipsingBinaries-4.0.6/docs/_templates/autosummary/base.rst
--rw-r--r--   0 runner    (1001) docker     (127)      252 2024-02-13 17:41:53.000000 EclipsingBinaries-4.0.6/docs/_templates/autosummary/class.rst
--rw-r--r--   0 runner    (1001) docker     (127)      253 2024-02-13 17:41:53.000000 EclipsingBinaries-4.0.6/docs/_templates/autosummary/module.rst
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-02-13 17:41:53.000000 EclipsingBinaries-4.0.6/docs/changelog.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1612 2024-02-13 17:41:53.000000 EclipsingBinaries-4.0.6/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)      985 2024-02-13 17:41:53.000000 EclipsingBinaries-4.0.6/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (127)      685 2024-02-13 17:41:53.000000 EclipsingBinaries-4.0.6/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)      736 2024-02-13 17:41:53.000000 EclipsingBinaries-4.0.6/docs/installation.rst
--rw-r--r--   0 runner    (1001) docker     (127)      156 2024-02-13 17:41:53.000000 EclipsingBinaries-4.0.6/docs/license.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2028 2024-02-13 17:41:53.000000 EclipsingBinaries-4.0.6/docs/pipeline.rst
--rw-r--r--   0 runner    (1001) docker     (127)    24030 2024-02-13 17:41:53.000000 EclipsingBinaries-4.0.6/docs/toolbox.rst
--rw-r--r--   0 runner    (1001) docker     (127)      132 2024-02-13 17:41:53.000000 EclipsingBinaries-4.0.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      232 2024-02-13 17:41:53.000000 EclipsingBinaries-4.0.6/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2182 2024-02-13 17:42:08.031850 EclipsingBinaries-4.0.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-13 17:41:53.000000 EclipsingBinaries-4.0.6/setup.py
--rw-r--r--   0 runner    (1001) docker     (127)     1975 2024-02-13 17:41:53.000000 EclipsingBinaries-4.0.6/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 21:13:15.655256 EclipsingBinaries-4.0.7/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 21:13:15.639256 EclipsingBinaries-4.0.7/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 21:13:15.643256 EclipsingBinaries-4.0.7/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)      856 2024-04-03 21:12:59.000000 EclipsingBinaries-4.0.7/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (127)      597 2024-04-03 21:12:59.000000 EclipsingBinaries-4.0.7/.github/ISSUE_TEMPLATE/feature_request.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 21:13:15.643256 EclipsingBinaries-4.0.7/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     3190 2024-04-03 21:12:59.000000 EclipsingBinaries-4.0.7/.github/workflows/ci_tests.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1204 2024-04-03 21:12:59.000000 EclipsingBinaries-4.0.7/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      404 2024-04-03 21:12:59.000000 EclipsingBinaries-4.0.7/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)   108265 2024-04-03 21:12:59.000000 EclipsingBinaries-4.0.7/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)     5234 2024-04-03 21:12:59.000000 EclipsingBinaries-4.0.7/CODE_OF_CONDUCT.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 21:13:15.647256 EclipsingBinaries-4.0.7/EclipsingBinaries/
+-rw-r--r--   0 runner    (1001) docker     (127)    24730 2024-04-03 21:12:59.000000 EclipsingBinaries-4.0.7/EclipsingBinaries/IRAF_Reduction.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8436 2024-04-03 21:12:59.000000 EclipsingBinaries-4.0.7/EclipsingBinaries/Night_Filters.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20913 2024-04-03 21:12:59.000000 EclipsingBinaries-4.0.7/EclipsingBinaries/OC_plot.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22282 2024-04-03 21:12:59.000000 EclipsingBinaries-4.0.7/EclipsingBinaries/OConnell.py
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-03 21:12:59.000000 EclipsingBinaries-4.0.7/EclipsingBinaries/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19927 2024-04-03 21:12:59.000000 EclipsingBinaries-4.0.7/EclipsingBinaries/apass.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31251 2024-04-03 21:12:59.000000 EclipsingBinaries-4.0.7/EclipsingBinaries/color_light_curve.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 21:13:15.651256 EclipsingBinaries-4.0.7/EclipsingBinaries/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)     2293 2024-04-03 21:12:59.000000 EclipsingBinaries-4.0.7/EclipsingBinaries/examples/APASS_Catalog_ex.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      314 2024-04-03 21:12:59.000000 EclipsingBinaries-4.0.7/EclipsingBinaries/examples/Gaia_output.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      968 2024-04-03 21:12:59.000000 EclipsingBinaries-4.0.7/EclipsingBinaries/examples/O-C_paper_table.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    85904 2024-04-03 21:12:59.000000 EclipsingBinaries-4.0.7/EclipsingBinaries/examples/OConnell_plot.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1009 2024-04-03 21:12:59.000000 EclipsingBinaries-4.0.7/EclipsingBinaries/examples/OConnell_table.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    48237 2024-04-03 21:12:59.000000 EclipsingBinaries-4.0.7/EclipsingBinaries/examples/O_C_ex.png
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 21:12:59.000000 EclipsingBinaries-4.0.7/EclipsingBinaries/examples/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 21:13:15.651256 EclipsingBinaries-4.0.7/EclipsingBinaries/examples/calibration_images/
+-rw-r--r--   0 runner    (1001) docker     (127)      125 2024-04-03 21:13:03.000000 EclipsingBinaries-4.0.7/EclipsingBinaries/examples/calibration_images/purpose.txt
+-rw-r--r--   0 runner    (1001) docker     (127)   135237 2024-04-03 21:13:03.000000 EclipsingBinaries-4.0.7/EclipsingBinaries/examples/color_light_curve_ex.png
+-rw-r--r--   0 runner    (1001) docker     (127)    35357 2024-04-03 21:13:03.000000 EclipsingBinaries-4.0.7/EclipsingBinaries/examples/example_OC_table.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     4442 2024-04-03 21:13:03.000000 EclipsingBinaries-4.0.7/EclipsingBinaries/examples/example_regression.txt
+-rw-r--r--   0 runner    (1001) docker     (127)   118184 2024-04-03 21:13:03.000000 EclipsingBinaries-4.0.7/EclipsingBinaries/examples/gui_color_light.png
+-rw-r--r--   0 runner    (1001) docker     (127)   109712 2024-04-03 21:13:03.000000 EclipsingBinaries-4.0.7/EclipsingBinaries/examples/light_curve_ex.png
+-rw-r--r--   0 runner    (1001) docker     (127)   136591 2024-04-03 21:13:04.000000 EclipsingBinaries-4.0.7/EclipsingBinaries/examples/min_program_demo.png
+-rw-r--r--   0 runner    (1001) docker     (127)   131114 2024-04-03 21:13:04.000000 EclipsingBinaries-4.0.7/EclipsingBinaries/examples/overlay_example.png
+-rw-r--r--   0 runner    (1001) docker     (127)    31361 2024-04-03 21:13:04.000000 EclipsingBinaries-4.0.7/EclipsingBinaries/examples/test_B.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    25814 2024-04-03 21:13:04.000000 EclipsingBinaries-4.0.7/EclipsingBinaries/examples/test_R.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    30132 2024-04-03 21:13:04.000000 EclipsingBinaries-4.0.7/EclipsingBinaries/examples/test_V.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    39669 2024-04-03 21:13:04.000000 EclipsingBinaries-4.0.7/EclipsingBinaries/examples/test_minimums.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    25259 2024-04-03 21:13:04.000000 EclipsingBinaries-4.0.7/EclipsingBinaries/find_min.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7284 2024-04-03 21:13:04.000000 EclipsingBinaries-4.0.7/EclipsingBinaries/gaia.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3458 2024-04-03 21:13:04.000000 EclipsingBinaries-4.0.7/EclipsingBinaries/menu.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16127 2024-04-03 21:13:04.000000 EclipsingBinaries-4.0.7/EclipsingBinaries/multi_aperture_photometry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3680 2024-04-03 21:13:04.000000 EclipsingBinaries-4.0.7/EclipsingBinaries/pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2502 2024-04-03 21:13:04.000000 EclipsingBinaries-4.0.7/EclipsingBinaries/tess_ccd_info.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     5623 2024-04-03 21:13:04.000000 EclipsingBinaries-4.0.7/EclipsingBinaries/tess_data_search.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4787 2024-04-03 21:13:04.000000 EclipsingBinaries-4.0.7/EclipsingBinaries/tesscut.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 21:13:15.651256 EclipsingBinaries-4.0.7/EclipsingBinaries/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        2 2024-04-03 21:13:04.000000 EclipsingBinaries-4.0.7/EclipsingBinaries/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      843 2024-04-03 21:13:04.000000 EclipsingBinaries-4.0.7/EclipsingBinaries/tests/test_IRAF_Reduction.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1533 2024-04-03 21:13:04.000000 EclipsingBinaries-4.0.7/EclipsingBinaries/tests/test_OC_plot.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14791 2024-04-03 21:13:04.000000 EclipsingBinaries-4.0.7/EclipsingBinaries/tests/test_apass.py
+-rw-r--r--   0 runner    (1001) docker     (127)    90297 2024-04-03 21:13:04.000000 EclipsingBinaries-4.0.7/EclipsingBinaries/vseq_updated.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 21:13:15.655256 EclipsingBinaries-4.0.7/EclipsingBinaries.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4059 2024-04-03 21:13:11.000000 EclipsingBinaries-4.0.7/EclipsingBinaries.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2453 2024-04-03 21:13:15.000000 EclipsingBinaries-4.0.7/EclipsingBinaries.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 21:13:11.000000 EclipsingBinaries-4.0.7/EclipsingBinaries.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      125 2024-04-03 21:13:11.000000 EclipsingBinaries-4.0.7/EclipsingBinaries.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 21:13:11.000000 EclipsingBinaries-4.0.7/EclipsingBinaries.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      262 2024-04-03 21:13:11.000000 EclipsingBinaries-4.0.7/EclipsingBinaries.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-03 21:13:11.000000 EclipsingBinaries-4.0.7/EclipsingBinaries.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1520 2024-04-03 21:13:04.000000 EclipsingBinaries-4.0.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      161 2024-04-03 21:13:04.000000 EclipsingBinaries-4.0.7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     4059 2024-04-03 21:13:15.655256 EclipsingBinaries-4.0.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3177 2024-04-03 21:13:04.000000 EclipsingBinaries-4.0.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 21:13:15.655256 EclipsingBinaries-4.0.7/changelog/
+-rw-r--r--   0 runner    (1001) docker     (127)   222548 2024-04-03 21:13:04.000000 EclipsingBinaries-4.0.7/changelog/package-lock.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1347 2024-04-03 21:13:04.000000 EclipsingBinaries-4.0.7/changelog/package.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 21:13:15.655256 EclipsingBinaries-4.0.7/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      286 2024-04-03 21:13:04.000000 EclipsingBinaries-4.0.7/docs/EB.rst
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 21:13:04.000000 EclipsingBinaries-4.0.7/docs/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 21:13:15.639256 EclipsingBinaries-4.0.7/docs/_templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 21:13:15.655256 EclipsingBinaries-4.0.7/docs/_templates/autosummary/
+-rw-r--r--   0 runner    (1001) docker     (127)      251 2024-04-03 21:13:04.000000 EclipsingBinaries-4.0.7/docs/_templates/autosummary/base.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      252 2024-04-03 21:13:04.000000 EclipsingBinaries-4.0.7/docs/_templates/autosummary/class.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      253 2024-04-03 21:13:04.000000 EclipsingBinaries-4.0.7/docs/_templates/autosummary/module.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-04-03 21:13:04.000000 EclipsingBinaries-4.0.7/docs/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1600 2024-04-03 21:13:04.000000 EclipsingBinaries-4.0.7/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      985 2024-04-03 21:13:04.000000 EclipsingBinaries-4.0.7/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      685 2024-04-03 21:13:04.000000 EclipsingBinaries-4.0.7/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      756 2024-04-03 21:13:04.000000 EclipsingBinaries-4.0.7/docs/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      156 2024-04-03 21:13:04.000000 EclipsingBinaries-4.0.7/docs/license.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2028 2024-04-03 21:13:04.000000 EclipsingBinaries-4.0.7/docs/pipeline.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    24030 2024-04-03 21:13:04.000000 EclipsingBinaries-4.0.7/docs/toolbox.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      132 2024-04-03 21:13:04.000000 EclipsingBinaries-4.0.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      232 2024-04-03 21:13:04.000000 EclipsingBinaries-4.0.7/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2197 2024-04-03 21:13:15.659256 EclipsingBinaries-4.0.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-03 21:13:04.000000 EclipsingBinaries-4.0.7/setup.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1975 2024-04-03 21:13:04.000000 EclipsingBinaries-4.0.7/tox.ini
```

### Comparing `EclipsingBinaries-4.0.6/.github/ISSUE_TEMPLATE/bug_report.md` & `EclipsingBinaries-4.0.7/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `EclipsingBinaries-4.0.6/.github/ISSUE_TEMPLATE/feature_request.md` & `EclipsingBinaries-4.0.7/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `EclipsingBinaries-4.0.6/.github/workflows/ci_tests.yml` & `EclipsingBinaries-4.0.7/.github/workflows/ci_tests.yml`

 * *Files identical despite different names*

### Comparing `EclipsingBinaries-4.0.6/.github/workflows/python-publish.yml` & `EclipsingBinaries-4.0.7/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `EclipsingBinaries-4.0.6/CHANGELOG.md` & `EclipsingBinaries-4.0.7/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -3,14 +3,85 @@
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/)
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
 Generated by [`auto-changelog`](https://github.com/CookPete/auto-changelog).
 
+## [v4.0.6](https://github.com/kjkoeller/Binary_Star_Research_Package/compare/v4.0.5...v4.0.6) - 2024-02-13
+
+### Merged
+
+*   Fixes Rounding Error from Floor Function [`#344`](https://github.com/kjkoeller/Binary_Star_Research_Package/pull/344)
+*   Environment Versions Incorrect [`#346`](https://github.com/kjkoeller/Binary_Star_Research_Package/pull/346)
+*   Pyia Requirement to 1.41 [`#345`](https://github.com/kjkoeller/Binary_Star_Research_Package/pull/345)
+*   Commenting Out Broken Lines [`#343`](https://github.com/kjkoeller/Binary_Star_Research_Package/pull/343)
+*   Python Version to Build.tools [`#342`](https://github.com/kjkoeller/Binary_Star_Research_Package/pull/342)
+*   Switching from Image to OS [`#341`](https://github.com/kjkoeller/Binary_Star_Research_Package/pull/341)
+*   Updating Tests [`#339`](https://github.com/kjkoeller/Binary_Star_Research_Package/pull/339)
+*   Version 2 is Depreciated [`#338`](https://github.com/kjkoeller/Binary_Star_Research_Package/pull/338)
+
+### Commits
+
+*   Changing Pyia Requirement [`33f2bec`](https://github.com/kjkoeller/Binary_Star_Research_Package/commit/33f2bec7ccc7ff1e81c7e183e3e52f7db4e79df1)
+
+## [v4.0.5](https://github.com/kjkoeller/Binary_Star_Research_Package/compare/v4.0.3...v4.0.5) - 2024-01-27
+
+### Merged
+
+*   Incorrect Gain Column [`#337`](https://github.com/kjkoeller/Binary_Star_Research_Package/pull/337)
+*   Adds Paper For TESS CCD Information [`#336`](https://github.com/kjkoeller/Binary_Star_Research_Package/pull/336)
+*   Incorrect Return Type [`#335`](https://github.com/kjkoeller/Binary_Star_Research_Package/pull/335)
+
+### Commits
+
+*   Update python-publish.yml [`6f6814b`](https://github.com/kjkoeller/Binary_Star_Research_Package/commit/6f6814bd4678a81a5e4c18c5c561a03f92a10aa0)
+*   Delete .github/workflows/python-publish.yml [`5561ec2`](https://github.com/kjkoeller/Binary_Star_Research_Package/commit/5561ec2ba79ecb58ed1eb062abc26948d21da7d6)
+*   Create python-publish.yml [`d939d2a`](https://github.com/kjkoeller/Binary_Star_Research_Package/commit/d939d2a67daa733059eecc9f84df0d3cabb58fc1)
+*   Update python-publish.yml [`cee6760`](https://github.com/kjkoeller/Binary_Star_Research_Package/commit/cee67608194645cb70adf6fadb8c776468768ebb)
+*   Update python-publish.yml [`f690a9e`](https://github.com/kjkoeller/Binary_Star_Research_Package/commit/f690a9e933a35130d04ed8fe1c36dae906687d84)
+*   Update python-publish.yml [`434e8bc`](https://github.com/kjkoeller/Binary_Star_Research_Package/commit/434e8bc82231e26e02614a6fb7d299f17fe5ba5b)
+*   Update python-publish.yml [`50680cd`](https://github.com/kjkoeller/Binary_Star_Research_Package/commit/50680cdd99e8f8e61d1aa19bd5e00c6d3a451e50)
+*   Update python-publish.yml [`5dbe692`](https://github.com/kjkoeller/Binary_Star_Research_Package/commit/5dbe692ed6682b14a21ebecba9126049e0b05026)
+*   Update python-publish.yml [`59bcedc`](https://github.com/kjkoeller/Binary_Star_Research_Package/commit/59bcedc02a8e42bac642382731c902d37aa072b6)
+*   Publish Package Update [`ca5fa2c`](https://github.com/kjkoeller/Binary_Star_Research_Package/commit/ca5fa2cc9d457cadfa934cd5cdde8005369168c5)
+*   Add Update Setuptools [`5041a69`](https://github.com/kjkoeller/Binary_Star_Research_Package/commit/5041a695ae36b7fdfa8aa8d7faf4617826a8a93a)
+
+## [v4.0.3](https://github.com/kjkoeller/Binary_Star_Research_Package/compare/v4.0.2...v4.0.3) - 2023-09-29
+
+### Merged
+
+*   Changing in Formatting Output [`#334`](https://github.com/kjkoeller/Binary_Star_Research_Package/pull/334)
+*   Add Photutils Requirement [`#333`](https://github.com/kjkoeller/Binary_Star_Research_Package/pull/333)
+*   Create tox.ini [`#329`](https://github.com/kjkoeller/Binary_Star_Research_Package/pull/329)
+*   Angle Fixes [`#328`](https://github.com/kjkoeller/Binary_Star_Research_Package/pull/328)
+*   Update ci\_tests.yml [`#326`](https://github.com/kjkoeller/Binary_Star_Research_Package/pull/326)
+*   Missing Required Package [`#322`](https://github.com/kjkoeller/Binary_Star_Research_Package/pull/322)
+
+## [v4.0.2](https://github.com/kjkoeller/Binary_Star_Research_Package/compare/v4.0.1...v4.0.2) - 2023-08-16
+
+### Merged
+
+*   Incorrect Import [`#321`](https://github.com/kjkoeller/Binary_Star_Research_Package/pull/321)
+
+### Commits
+
+*   Update **init**.py [`2588bba`](https://github.com/kjkoeller/Binary_Star_Research_Package/commit/2588bba734cd0d426571d35c598fe2223c0c2663)
+
+## [v4.0.1](https://github.com/kjkoeller/Binary_Star_Research_Package/compare/v4.0.0...v4.0.1) - 2023-08-16
+
+### Merged
+
+*   Comment Out Function Call [`#320`](https://github.com/kjkoeller/Binary_Star_Research_Package/pull/320)
+*   v4.0.0 [`#319`](https://github.com/kjkoeller/Binary_Star_Research_Package/pull/319)
+
+### Commits
+
+*   Update **init**.py [`187747b`](https://github.com/kjkoeller/Binary_Star_Research_Package/commit/187747bd2be024552451153ce0ad580f52df92e7)
+
 ## [v4.0.0](https://github.com/kjkoeller/Binary_Star_Research_Package/compare/v3.1.12...v4.0.0) - 2023-08-16
 
 ### Merged
 
 *   Adds in Multi-Aperture Option [`#318`](https://github.com/kjkoeller/Binary_Star_Research_Package/pull/318)
 *   V-R Polynomial Fit [`#312`](https://github.com/kjkoeller/Binary_Star_Research_Package/pull/312)
 *   Major Improvements to Calculations [`#317`](https://github.com/kjkoeller/Binary_Star_Research_Package/pull/317)
```

### Comparing `EclipsingBinaries-4.0.6/CODE_OF_CONDUCT.md` & `EclipsingBinaries-4.0.7/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `EclipsingBinaries-4.0.6/EclipsingBinaries/IRAF_Reduction.py` & `EclipsingBinaries-4.0.7/EclipsingBinaries/IRAF_Reduction.py`

 * *Files 2% similar despite different names*

```diff
@@ -136,15 +136,15 @@
             master_dark = None
         else:
             master_dark = dark(files, zero, calibrated_data, overscan_region, trim_region)
 
         flat(files, zero, master_dark, calibrated_data, overscan_region, trim_region)
         science_images(files, calibrated_data, zero, master_dark, trim_region, overscan_region)
 
-
+# more observatory sites can be found here: https://github.com/astropy/astropy-data/blob/gh-pages/coordinates/sites.json
 def kpno():
     """
     Kitt Peak National Observatory default values
 
     :return: None
     """
     global gain
@@ -550,40 +550,43 @@
     fits.setval(image_name, "OBSERVAT", value=location, comment="Obs. Loc.")
     fits.setval(image_name, "IMAGETYP", value=imagetyp, comment="Image type")
     fits.setval(image_name, "DATASEC", value=trim_region, comment="Trim data section")
     fits.setval(image_name, "BIASSEC", value=overscan_region, comment="Overscan section")
     fits.setval(image_name, "EPOCH", value="J2000.0")
     # fits.setval(bias_image, "FILTER", value=filter_name)
     if imagetyp == "LIGHT":
-        if location.lower() == "bsuo":
-            # location of BSUO
-            obs_location = {
-                'lon': -85.411896,  # degrees
-                'lat': 40.199879,  # degrees
-                'elevation': 0.2873  # kilometers
-            }
-            bjd = BJD_TDB(hjd, obs_location, ra, dec)
-            fits.setval(image_name, "BJD_TDB", value=bjd.value, comment="Bary. Julian Date, Bary. Dynamical Time")
-        else:
-            bjd = BJD_TDB(hjd, location, ra, dec)
-            fits.setval(image_name, "BJD_TDB", value=bjd.value, comment="Bary. Julian Date, Bary. Dynamical Time")
+        bjd = BJD_TDB(hjd, location, ra, dec)
+        fits.setval(image_name, "BJD_TDB", value=bjd.value, comment="Bary. Julian Date, Bary. Dynamical Time")
 
 
-def BJD_TDB(hjd, loc, ra, dec):
+def BJD_TDB(hjd, site_name, ra, dec):
     """
     Converts HJD to BJD_TDB
 
     :param ra: right ascension of target object
     :param dec: declination of target object
     :param hjd: HJD time for the mid-exposure image
     :param loc: location of the observations
     :return: Newly calculated BJD_TDB that is light time corrected
     """
+    
+    if site_name == "bsuo":
+        # set the latitude and longitude of the BSUO site manually
+        loc = {
+            'lon': -85.411896,  # degrees
+            'lat': 40.199879,  # degrees
+            'elevation': 0.2873  # kilometers
+        }
+        obs = EarthLocation.from_geodetic(loc["lat"], loc["lon"], loc["elevation"])
+    else:
+        loc = EarthLocation.of_site(site_name)
+        # need to gather the specific lat, long, and elev. from the .geodetic command. This specifically lists information on each of the parameters but we only want the value and not the units
+        obs = EarthLocation.from_geodetic(loc.geodetic[0].value, loc.geodetic[1].value, loc.geodetic[2].value/1000) # converts the meters of the elevation to km
+        
     helio = Time(hjd, scale='utc', format='jd')
-    obs = EarthLocation.from_geodetic(loc["lon"], loc["lat"], loc["elevation"])
     star = SkyCoord(ra, dec, unit=(u.hour, u.deg))
     ltt = helio.light_travel_time(star, 'heliocentric', location=obs)
     guess = helio - ltt
     # if we assume guess is correct - how far is heliocentric time away from true value?
     delta = (guess + guess.light_travel_time(star, 'heliocentric', obs)).jd - helio.jd
     # apply this correction
     guess -= delta * u.d
```

### Comparing `EclipsingBinaries-4.0.6/EclipsingBinaries/Night_Filters.py` & `EclipsingBinaries-4.0.7/EclipsingBinaries/Night_Filters.py`

 * *Files identical despite different names*

### Comparing `EclipsingBinaries-4.0.6/EclipsingBinaries/OC_plot.py` & `EclipsingBinaries-4.0.7/EclipsingBinaries/OC_plot.py`

 * *Files identical despite different names*

### Comparing `EclipsingBinaries-4.0.6/EclipsingBinaries/OConnell.py` & `EclipsingBinaries-4.0.7/EclipsingBinaries/OConnell.py`

 * *Files identical despite different names*

### Comparing `EclipsingBinaries-4.0.6/EclipsingBinaries/apass.py` & `EclipsingBinaries-4.0.7/EclipsingBinaries/apass.py`

 * *Files identical despite different names*

### Comparing `EclipsingBinaries-4.0.6/EclipsingBinaries/color_light_curve.py` & `EclipsingBinaries-4.0.7/EclipsingBinaries/color_light_curve.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 # -*- coding: utf-8 -*-
 """
 Created on Thu Sep 17 12:45:40 2020
 Created on Tue Feb 16 19:29:16 2021
 @author: Alec Neal
 
-Last Edited: 08/15/2022
+Last Edited: 02/16/2024
 Editor: Kyle Koeller
 """
 
-# import vseq_updated as vseq  # testing purposes
-from . import vseq_updated as vseq
+# from vseq_updated import io, calc, FT, binning, plot, Flower  # testing purposes
+from .vseq_updated import io, calc, FT, binning, plot, Flower
 import numpy as np
 import matplotlib.pyplot as plt
 import statistics as st
 from tkinter import *
 from matplotlib.backends.backend_tkagg import (
     FigureCanvasTkAgg)
 from matplotlib.figure import Figure
@@ -81,37 +81,37 @@
     :param lower_lim: lower limit
     :param FTinterp: interpolates number
     :param quad_range: ?
     :param index: type of color index to use
 
     :return: returns the B-V value and other assorted values
     """
-    B_HJD, B_mag, B_magerr = vseq.io.importFile_pd(Bfile)[:3:]
-    V_HJD, V_mag, V_magerr = vseq.io.importFile_pd(Vfile)[:3:]
+    B_HJD, B_mag, B_magerr = io.importFile_pd(Bfile)[:3:]
+    V_HJD, V_mag, V_magerr = io.importFile_pd(Vfile)[:3:]
 
-    Bpoly = vseq.binning.polybinner(Bfile, Epoch, period, sections=2, section_order=8)
+    Bpoly = binning.polybinner(Bfile, Epoch, period, sections=2, section_order=8)
     Bphase = Bpoly[1][0][0][1]
     aB = Bpoly[0][0]
     bB = Bpoly[0][1]
     Bnorm = Bpoly[1][0][4]
-    Vphase = list(vseq.calc.astro.convert.HJD_phase(V_HJD, period, Epoch))
+    Vphase = list(calc.astro.convert.HJD_phase(V_HJD, period, Epoch))
     B_flux = np.array(10 ** (-0.4 * np.array(B_mag))) / Bnorm
     obs = len(V_HJD)
     tolerance = best_tol(B_HJD, V_HJD, period, lower_lim=lower_lim, max_tol=max_tol)
     before_after = occ2(B_HJD, V_HJD, period, tolerance=tolerance)
     befores = before_after[1]
     afters = before_after[2]
     i_before = before_after[3]
     i_after = before_after[4]
     mean_diff = np.mean(before_after[5])
 
     B_interp_flux = []
     for n in range(obs):
         if len(befores[n]) == 0 or len(afters[n]) == 0:
-            B_interp_flux.append(vseq.FT.sumatphase(Vphase[n], 10, aB, bB))
+            B_interp_flux.append(FT.sumatphase(Vphase[n], 10, aB, bB))
         else:
             B_interp_flux.append(lin_interp(V_HJD[n], befores[n][-1], afters[n][0],
                                             B_flux[i_before[n][-1]], B_flux[i_after[n][0]]))
 
     B_interp_mag = -2.5 * np.log10(np.array(B_interp_flux) * Bnorm)
     # quad_range=0.075
     BVquadphase = []
@@ -127,47 +127,48 @@
 
     B_minus_V = B_interp_mag - np.array(V_mag)
     BV_mean = mean_mag(B_minus_V)
     # print(B_minus_V)
     BV_err = st.stdev(B_minus_V, xbar=BV_mean)
 
     print('ave diff =', round(mean_diff * 100, 3), '% of period')
-    aVphase, aV_mag, aB_interp_mag = vseq.plot.aliasing2(Vphase, V_mag, B_interp_mag)[:3:]
-    aBphase, aB_mag = vseq.plot.aliasing2(Bphase, B_mag, B_mag)[:2:]
-    aB_minus_V = vseq.plot.aliasing2(Vphase, B_minus_V, B_minus_V)[1]
+    aVphase, aV_mag, aB_interp_mag = plot.aliasing2(Vphase, V_mag, B_interp_mag)[:3:]
+    aBphase, aB_mag = plot.aliasing2(Bphase, B_mag, B_mag)[:2:]
+    aB_minus_V = plot.aliasing2(Vphase, B_minus_V, B_minus_V)[1]
     B_V = [B_minus_V, BV_mean, BV_err, aB_minus_V]
     B = [aBphase, aB_mag, aB_interp_mag]
     V = [aVphase, aV_mag]
 
     # print('T =', vseq.Flower.T.Teff(quadcolor - (0.641 / 3.1)))
     if index == "BV":
         temp = []
         # temp = vseq.Flower.T.Teff(quadcolor - (0.641 / 3.1), colorerr)
-        t1 = vseq.Flower.T.Teff(quadcolor - (0.641 / 3.1))
-        temp_high = vseq.Flower.T.Teff(quadcolor - (0.641 / 3.1) - colorerr)
-        temp_low = vseq.Flower.T.Teff(quadcolor - (0.641 / 3.1) + colorerr)
+        t1 = Flower.T.Teff(quadcolor - (0.641 / 3.1))
+        temp_high = Flower.T.Teff(quadcolor - (0.641 / 3.1) - colorerr)
+        temp_low = Flower.T.Teff(quadcolor - (0.641 / 3.1) + colorerr)
 
         temp_err = (temp_high - temp_low)/2
         temp.append(t1)
         temp.append(temp_err)
         print('T_BV =', temp[0], '+/-', temp[1])
     elif index == "VR":
         # temp = vseq.Pecaut.T.Teff(quadcolor - (0.58 / 3.1), colorerr)
         temp = []
-        t1 = vseq.Flower.T.Teff(quadcolor - 0.561 * (0.641 / 3.1))
+        t1 = Flower.T.Teff(quadcolor - 0.561 * (0.641 / 3.1))
         # E_V-R = 0.561*E_B-V
-        temp_high = vseq.Flower.T.Teff(quadcolor - 0.561* (0.641 / 3.1) - colorerr)
-        temp_low = vseq.Flower.T.Teff(quadcolor - 0.561* (0.641 / 3.1) + colorerr)
+        temp_high = Flower.T.Teff(quadcolor - 0.561* (0.641 / 3.1) - colorerr)
+        temp_low = Flower.T.Teff(quadcolor - 0.561* (0.641 / 3.1) + colorerr)
 
         temp_err = (temp_high - temp_low) / 2
         temp.append(t1)
         temp.append(temp_err)
         if temp[0] == 0:
             print("V-R color cannot be used to determine temperature.")
-        print('T_VR =', temp[0], '+/-', temp[1])
+        else:
+            print('T_VR =', temp[0], '+/-', temp[1])
 
     return B_V, B, V, quadcolor, colorerr, temp
 
 
 # use this function below
 def color_plot(Bfile, Vfile, Epoch, period, max_tol=0.03, lower_lim=0.05, Rfile='', FTinterp=True,
                save=False, outName='noname_color.png', fs=12):
@@ -189,26 +190,26 @@
     """
     B_V = subtract_LC(Bfile, Vfile, Epoch, period, max_tol=max_tol, lower_lim=lower_lim, FTinterp=FTinterp, index="BV")
     Bphase, Bmag, B_interp_mag = B_V[1][:3:]
     Vphase, Vmag = B_V[2][:2:]
     aB_minus_V = B_V[0][3]
     quadcolor, colorerr = B_V[3:5:]
     if Rfile == '':
-        axs, fig = vseq.plot.multiplot((7, 7.5), height_ratios=[8, 4.5])
+        axs, _ = plot.multiplot((7, 7.5), height_ratios=[8, 4.5])
         mag = axs[0]
         bv = axs[1]
         mag.plot(Vphase, Vmag, 'og', ms=2)
         mag.plot(Bphase, Bmag, 'ob', ms=2)
         bv.plot(Vphase, aB_minus_V, 'ok', ms=2)
         bv.margins(y=0.1, x=1 / 24)
         mag.set_ylim(mag.get_ylim()[::-1])
         bv.set_ylim(bv.get_ylim()[::-1])
-        vseq.plot.sm_format(mag, X=0.25, x=0.05, Y=None, numbersize=fs, xbottom=False, bottomspine=False, tickwidth=1,
+        plot.sm_format(mag, X=0.25, x=0.05, Y=None, numbersize=fs, xbottom=False, bottomspine=False, tickwidth=1,
                             Xsize=7, xsize=3.5)
-        vseq.plot.sm_format(bv, X=0.25, x=0.05, numbersize=fs, xtop=False, topspine=False, tickwidth=1, Xsize=7,
+        plot.sm_format(bv, X=0.25, x=0.05, numbersize=fs, xtop=False, topspine=False, tickwidth=1, Xsize=7,
                             xsize=3.5)
 
         maxtick = max(list(map(len, (list(map(str, np.array(mag.get_yticks()).round(8)))))))
         if maxtick == 5:
             ytickpad = -0.835
         else:
             ytickpad = -0.81
@@ -220,15 +221,15 @@
         # quadcolor,colorerr=B_V[3:5:]
         bv.axhline(quadcolor, color='gray', linewidth=None)
     else:
         V_R = subtract_LC(Vfile, Rfile, Epoch, period, max_tol, lower_lim=lower_lim, index="VR")
         Rphase, Rmag = V_R[2][:2:]
         V_interp_mag = V_R[1][2]
         aV_minus_R = V_R[0][3]
-        axs, fig = vseq.plot.multiplot((7, 9), height_ratios=[8, 3, 3])
+        axs, fig = plot.multiplot((7, 9), height_ratios=[8, 3, 3])
         mag = axs[0]
         bv = axs[2]
         vr = axs[1]
         mag.plot(Vphase, Vmag, 'og', ms=2)
         mag.plot(Bphase, Bmag, 'ob', ms=2)
         mag.plot(Rphase, Rmag, 'or', ms=2)
 
@@ -236,18 +237,18 @@
         vr.plot(Rphase, aV_minus_R, 'ok', ms=3)
         bv.margins(y=0.07, x=1 / 24)
         vr.margins(y=0.07)
         # mag.margins(y=0.09)
         mag.set_ylim(mag.get_ylim()[::-1])
         bv.set_ylim(bv.get_ylim()[::-1])
         vr.set_ylim(vr.get_ylim()[::-1])
-        vseq.plot.sm_format(mag, X=0.25, x=0.05, numbersize=fs, xbottom=False, bottomspine=False)
-        vseq.plot.sm_format(vr, X=0.25, x=0.05, numbersize=fs, xtop=False, topspine=False, xbottom=False,
+        plot.sm_format(mag, X=0.25, x=0.05, numbersize=fs, xbottom=False, bottomspine=False)
+        plot.sm_format(vr, X=0.25, x=0.05, numbersize=fs, xtop=False, topspine=False, xbottom=False,
                             bottomspine=False)
-        vseq.plot.sm_format(bv, X=0.25, x=0.05, numbersize=fs, xtop=False, topspine=False)
+        plot.sm_format(bv, X=0.25, x=0.05, numbersize=fs, xtop=False, topspine=False)
         maxtick = max(list(map(len, (list(map(str, np.array(mag.get_yticks()).round(8)))))))
         if maxtick == 5:
             ytickpad = -0.835
         else:
             ytickpad = -0.81
         mag.text(ytickpad, (max(Bmag) + min(Bmag)) / 2, r'$\rm B$', rotation=90, fontsize=fs * 1.2)
         mag.text(ytickpad, (max(Vmag) + min(Vmag)) / 2, r'$\rm V$', rotation=90, fontsize=fs * 1.2)
@@ -446,14 +447,18 @@
     BVL.grid(row=len(entries) + 6, column=0, columnspan=2)
     BVL_temp = Label(root, text='')
     BVL_temp.grid(row=len(entries) + 7, column=0, columnspan=2)
     VRL = Label(root, text='')
     VRL_temp = Label(root, text='')
     VRL.grid(row=len(entries) + 4, column=0, columnspan=2)
     VRL_temp.grid(row=len(entries) + 5, column=0, columnspan=2)
+    # max1 = Label(root, text='')
+    # max2 = Label(root, text='')
+    # max1.grid(row=len(entries) + 8, column=0, columnspan=2)
+    # max2.grid(row=len(entries) + 9, column=0, columnspan=2)
     # B2=gui.Field(root,'B file',2,0)
     fs = 14
 
     def call_colorplot2():
         """
         Calls to create the color plot after clicking the plot button.
 
@@ -471,26 +476,26 @@
         if getit(R) == '':
             """
             Checks whether the user has entered a R band text file
             """
             fig = Figure(figsize=(7, 7.8), dpi=90, tight_layout=True)
             # canvas = FigureCanvasTkAgg(fig, master=root)
             # canvas.destroy()
-            axs, _ = vseq.plot.multiplot(height_ratios=[8, 4.5], fig=fig)
+            axs, _ = plot.multiplot(height_ratios=[8, 4.5], fig=fig)
             mag = axs[0]
             bv = axs[1]
             mag.plot(Vphase, Vmag, 'o', ms=2, color='#00FF00')
             mag.plot(Bphase, Bmag, 'ob', ms=2)
             bv.plot(Vphase, aB_minus_V, 'ok', ms=3)
             bv.margins(y=0.1, x=1 / 24)
             mag.set_ylim(mag.get_ylim()[::-1])
             bv.set_ylim(bv.get_ylim()[::-1])
-            vseq.plot.sm_format(mag, X=0.25, x=0.05, Y=None, numbersize=fs, xbottom=False, bottomspine=False,
+            plot.sm_format(mag, X=0.25, x=0.05, Y=None, numbersize=fs, xbottom=False, bottomspine=False,
                                 tickwidth=1, Xsize=7, xsize=3.5)
-            vseq.plot.sm_format(bv, X=0.25, x=0.05, numbersize=fs, xtop=False, topspine=False, tickwidth=1, Xsize=7,
+            plot.sm_format(bv, X=0.25, x=0.05, numbersize=fs, xtop=False, topspine=False, tickwidth=1, Xsize=7,
                                 xsize=3.5)
 
             maxtick = max(list(map(len, (list(map(str, np.array(mag.get_yticks()).round(8)))))))
             if maxtick == 5:
                 ytickpad = -0.835
             else:
                 ytickpad = -0.81
@@ -516,15 +521,15 @@
             Rphase, Rmag = V_R[2][:2:]
             # V_interp_mag = V_R[1][2]
             aV_minus_R = V_R[0][3]
             VR_temp = V_R[5]
             fig = Figure(figsize=(7, 9), dpi=90, tight_layout=True)
             # canvas = FigureCanvasTkAgg(fig, master=root)
             # canvas.destroy()
-            axs, _ = vseq.plot.multiplot(height_ratios=[8, 3, 3], fig=fig)
+            axs, _ = plot.multiplot(height_ratios=[8, 3, 3], fig=fig)
             mag = axs[0]
             bv = axs[2]
             vr = axs[1]
             mag.plot(Vphase, Vmag, 'o', ms=2, color='#00FF00')
             mag.plot(Bphase, Bmag, 'ob', ms=2)
             mag.plot(Rphase, Rmag, 'or', ms=2)
 
@@ -532,18 +537,18 @@
             vr.plot(Rphase, aV_minus_R, 'ok', ms=3)
             bv.margins(y=0.07, x=1 / 24)
             vr.margins(y=0.07)
             # mag.margins(y=0.09)
             mag.set_ylim(mag.get_ylim()[::-1])
             bv.set_ylim(bv.get_ylim()[::-1])
             vr.set_ylim(vr.get_ylim()[::-1])
-            vseq.plot.sm_format(mag, X=0.25, x=0.05, numbersize=fs, xbottom=False, bottomspine=False)
-            vseq.plot.sm_format(vr, X=0.25, x=0.05, numbersize=fs, xtop=False, topspine=False, xbottom=False,
+            plot.sm_format(mag, X=0.25, x=0.05, numbersize=fs, xbottom=False, bottomspine=False)
+            plot.sm_format(vr, X=0.25, x=0.05, numbersize=fs, xtop=False, topspine=False, xbottom=False,
                                 bottomspine=False)
-            vseq.plot.sm_format(bv, X=0.25, x=0.05, numbersize=fs, xtop=False, topspine=False)
+            plot.sm_format(bv, X=0.25, x=0.05, numbersize=fs, xtop=False, topspine=False)
             maxtick = max(list(map(len, (list(map(str, np.array(mag.get_yticks()).round(8)))))))
             if maxtick == 5:
                 ytickpad = -0.835
             else:
                 ytickpad = -0.825
                 # ytickpad=-0.81
             mag.text(ytickpad, (max(Bmag) + min(Bmag)) / 2, r'$\rm B$', rotation=90, fontsize=fs * 1.2)
@@ -590,16 +595,21 @@
             # plt.savefig(getit(Out),bbox_inches='tight')
 
         # temp.config(text='(B-V) = ' + str(round(quadcolor, 6)) + ' +/- ' + str(round(colorerr, 6)), bg='white',
         #            relief='solid', borderwidth=1, padx=5, pady=5, font=('None', 14))
 
         BVL.config(text='(B-V) = ' + str(round(quadcolor, 6)) + ' +/- ' + str(round(colorerr, 6)), bg='white',
                    relief='solid', borderwidth=1, padx=5, pady=5, font=('None', 14))
-        BVL_temp.config(text='T_(B-V) = ' + str(format(BV_temp[0], ".4f")) + " +/- " + str(format(BV_temp[1], ".4f")), bg='white', relief='solid', borderwidth=1, padx=5,
-                        pady=5, font=('None', 14))
+        BVL_temp.config(text='T_(B-V) = ' + str(format(BV_temp[0], ".4f")) + " +/- " + str(format(BV_temp[1], ".4f")),
+                        bg='white', relief='solid', borderwidth=1, padx=5, pady=5, font=('None', 14))
+
+        # max1.config(text='Phase -0.25 = ' + str(round(quadcolor, 6)), bg='white',
+        #            relief='solid', borderwidth=1, padx=5, pady=5, font=('None', 14))
+        # max2.config(text='Phase 0.25 = ' + str(format(BV_temp[0], ".4f")), bg='white',
+        #             relief='solid', borderwidth=1, padx=5, pady=5, font=('None', 14))
         CreateToolTip(BVL, text=autowrap(
             'These values are calculated using an average of the (X-Y) values within phase 0.075 of quadrature (phase = +/- 0.25).'
             ' The given error is the standard\ndeviation of these values.', 50))
 
         CreateToolTip(VRL, text=autowrap(
             'These values are calculated using an average of the (X-Y) values within phase 0.075 of quadrature (phase = +/- 0.25).'
             ' The given error is the standard\ndeviation of these values.', 50))
@@ -630,11 +640,11 @@
 
     root.mainloop()
 
 
 # =======================
 
 # If you want to use the gui
-# color_gui(False)
+color_gui(False)
 
 # or just the function itself
 # color_plot('Bfile','Vfile',Epoch,period)
```

### Comparing `EclipsingBinaries-4.0.6/EclipsingBinaries/examples/APASS_Catalog_ex.txt` & `EclipsingBinaries-4.0.7/EclipsingBinaries/examples/APASS_Catalog_ex.txt`

 * *Files identical despite different names*

### Comparing `EclipsingBinaries-4.0.6/EclipsingBinaries/examples/O-C_paper_table.txt` & `EclipsingBinaries-4.0.7/EclipsingBinaries/examples/O-C_paper_table.txt`

 * *Files identical despite different names*

### Comparing `EclipsingBinaries-4.0.6/EclipsingBinaries/examples/OConnell_plot.png` & `EclipsingBinaries-4.0.7/EclipsingBinaries/examples/OConnell_plot.png`

 * *Files identical despite different names*

### Comparing `EclipsingBinaries-4.0.6/EclipsingBinaries/examples/OConnell_table.txt` & `EclipsingBinaries-4.0.7/EclipsingBinaries/examples/OConnell_table.txt`

 * *Files identical despite different names*

### Comparing `EclipsingBinaries-4.0.6/EclipsingBinaries/examples/O_C_ex.png` & `EclipsingBinaries-4.0.7/EclipsingBinaries/examples/O_C_ex.png`

 * *Files identical despite different names*

### Comparing `EclipsingBinaries-4.0.6/EclipsingBinaries/examples/color_light_curve_ex.png` & `EclipsingBinaries-4.0.7/EclipsingBinaries/examples/color_light_curve_ex.png`

 * *Files identical despite different names*

### Comparing `EclipsingBinaries-4.0.6/EclipsingBinaries/examples/example_OC_table.txt` & `EclipsingBinaries-4.0.7/EclipsingBinaries/examples/example_OC_table.txt`

 * *Files identical despite different names*

### Comparing `EclipsingBinaries-4.0.6/EclipsingBinaries/examples/example_regression.txt` & `EclipsingBinaries-4.0.7/EclipsingBinaries/examples/example_regression.txt`

 * *Files identical despite different names*

### Comparing `EclipsingBinaries-4.0.6/EclipsingBinaries/examples/gui_color_light.png` & `EclipsingBinaries-4.0.7/EclipsingBinaries/examples/gui_color_light.png`

 * *Files identical despite different names*

### Comparing `EclipsingBinaries-4.0.6/EclipsingBinaries/examples/light_curve_ex.png` & `EclipsingBinaries-4.0.7/EclipsingBinaries/examples/light_curve_ex.png`

 * *Files identical despite different names*

### Comparing `EclipsingBinaries-4.0.6/EclipsingBinaries/examples/min_program_demo.png` & `EclipsingBinaries-4.0.7/EclipsingBinaries/examples/min_program_demo.png`

 * *Files identical despite different names*

### Comparing `EclipsingBinaries-4.0.6/EclipsingBinaries/examples/overlay_example.png` & `EclipsingBinaries-4.0.7/EclipsingBinaries/examples/overlay_example.png`

 * *Files identical despite different names*

### Comparing `EclipsingBinaries-4.0.6/EclipsingBinaries/examples/test_B.txt` & `EclipsingBinaries-4.0.7/EclipsingBinaries/examples/test_B.txt`

 * *Files identical despite different names*

### Comparing `EclipsingBinaries-4.0.6/EclipsingBinaries/examples/test_R.txt` & `EclipsingBinaries-4.0.7/EclipsingBinaries/examples/test_R.txt`

 * *Files identical despite different names*

### Comparing `EclipsingBinaries-4.0.6/EclipsingBinaries/examples/test_V.txt` & `EclipsingBinaries-4.0.7/EclipsingBinaries/examples/test_V.txt`

 * *Files identical despite different names*

### Comparing `EclipsingBinaries-4.0.6/EclipsingBinaries/examples/test_minimums.txt` & `EclipsingBinaries-4.0.7/EclipsingBinaries/examples/test_minimums.txt`

 * *Files identical despite different names*

### Comparing `EclipsingBinaries-4.0.6/EclipsingBinaries/find_min.py` & `EclipsingBinaries-4.0.7/EclipsingBinaries/find_min.py`

 * *Files identical despite different names*

### Comparing `EclipsingBinaries-4.0.6/EclipsingBinaries/gaia.py` & `EclipsingBinaries-4.0.7/EclipsingBinaries/gaia.py`

 * *Files identical despite different names*

### Comparing `EclipsingBinaries-4.0.6/EclipsingBinaries/menu.py` & `EclipsingBinaries-4.0.7/EclipsingBinaries/menu.py`

 * *Files identical despite different names*

### Comparing `EclipsingBinaries-4.0.6/EclipsingBinaries/multi_aperture_photometry.py` & `EclipsingBinaries-4.0.7/EclipsingBinaries/multi_aperture_photometry.py`

 * *Files identical despite different names*

### Comparing `EclipsingBinaries-4.0.6/EclipsingBinaries/pipeline.py` & `EclipsingBinaries-4.0.7/EclipsingBinaries/pipeline.py`

 * *Files identical despite different names*

### Comparing `EclipsingBinaries-4.0.6/EclipsingBinaries/tess_ccd_info.txt` & `EclipsingBinaries-4.0.7/EclipsingBinaries/tess_ccd_info.txt`

 * *Files identical despite different names*

### Comparing `EclipsingBinaries-4.0.6/EclipsingBinaries/tess_data_search.py` & `EclipsingBinaries-4.0.7/EclipsingBinaries/tess_data_search.py`

 * *Files identical despite different names*

### Comparing `EclipsingBinaries-4.0.6/EclipsingBinaries/tesscut.py` & `EclipsingBinaries-4.0.7/EclipsingBinaries/tesscut.py`

 * *Files identical despite different names*

### Comparing `EclipsingBinaries-4.0.6/EclipsingBinaries/tests/test_apass.py` & `EclipsingBinaries-4.0.7/EclipsingBinaries/tests/test_apass.py`

 * *Files identical despite different names*

### Comparing `EclipsingBinaries-4.0.6/EclipsingBinaries/vseq_updated.py` & `EclipsingBinaries-4.0.7/EclipsingBinaries/vseq_updated.py`

 * *Files identical despite different names*

### Comparing `EclipsingBinaries-4.0.6/EclipsingBinaries.egg-info/PKG-INFO` & `EclipsingBinaries-4.0.7/EclipsingBinaries.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,52 +1,63 @@
 Metadata-Version: 2.1
 Name: EclipsingBinaries
-Version: 4.0.6
+Version: 4.0.7
 Summary: "Binary Star Package for Ball State University's Astronomy Research Group"
 Home-page: https://eclipsingbinaries.readthedocs.io/
 Author: Kyle Koeller
 License: MIT
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: numpy>=1.21
-Requires-Dist: astropy>=5.1.1
+Requires-Dist: astropy>=5.2.2
 Requires-Dist: astroquery>=0.4.6
 Requires-Dist: ccdproc>=2.4.0
-Requires-Dist: matplotlib>=3.3.1
-Requires-Dist: pandas>=1.1.0
-Requires-Dist: PyAstronomy>=0.18.0
-Requires-Dist: scipy>=1.5.2
+Requires-Dist: matplotlib>=3.5.1
+Requires-Dist: numpy>=1.22.3
+Requires-Dist: pandas>=1.4.2
+Requires-Dist: PyAstronomy>=0.18.1
+Requires-Dist: scipy>=1.9.3
 Requires-Dist: statsmodels>=0.13.5
 Requires-Dist: tqdm>=4.64.1
-Requires-Dist: numba>=0.56.3
+Requires-Dist: numba>=0.57.0
 Requires-Dist: seaborn>=0.12.2
-Requires-Dist: pyia>=1.3
+Requires-Dist: pyia<=1.41
 Requires-Dist: photutils>=1.8.0
+Requires-Dist: sphinx>=5
 Provides-Extra: docs
 Requires-Dist: sphinx-astropy; extra == "docs"
 Requires-Dist: matplotlib; extra == "docs"
 
 [![Python OS 3.8, 3.9, 3.10](https://github.com/kjkoeller/Binary_Star_Research_Package/actions/workflows/ci_tests.yml/badge.svg)](https://github.com/kjkoeller/Binary_Star_Research_Package/actions/workflows/ci_tests.yml)
 [![Documentation Status](https://readthedocs.org/projects/eclipsingbinaries/badge/?version=latest)](https://eclipsingbinaries.readthedocs.io/en/latest/?badge=latest)
 [![PyPI version](https://badge.fury.io/py/EclipsingBinaries.svg)](https://badge.fury.io/py/EclipsingBinaries)
 [![GitHub release](https://img.shields.io/github/v/release/kjkoeller/Variable_Star_Research_Package)](https://github.com/kjkoeller/Variable_Star_Research_Package/releases/)
 ![GitHub](https://img.shields.io/github/license/kjkoeller/Variable_Star_Research_Package)
 [![Codacy Badge](https://app.codacy.com/project/badge/Grade/9cd9a15e47ab4ed7b78071d096ea099d)](https://www.codacy.com/gh/kjkoeller/EclipsingBinaries/dashboard?utm_source=github.com\&utm_medium=referral\&utm_content=kjkoeller/EclipsingBinaries\&utm_campaign=Badge_Grade)
 [![astropy](http://img.shields.io/badge/powered%20by-AstroPy-orange.svg?style=flat)](http://www.astropy.org/)
 
-# Binary Star Research Package
+# EclipsingBinaries
 
-A Python project for Ball State University's Variable Star Research Group. Check the [Wiki](https://github.com/kjkoeller/EclipsingBinaries/wiki) for more detailed descriptions than the ones below and for usage details of each program.
+A Python project for Ball State University's Variable Star Research Group. The package can currently reduce data, find comparison stars from the APASS catalog, calculate and plot O-C values, find the color index and effective temperature, O'Connell effect parameters, and download TESS data and calculate TESS magnitudes from Gaia data.
 
 ***
 
-## Sponsor
+## Documentation
 
-If you would like to sponsor this project go [here](https://github.com/sponsors/kjkoeller) and click the sponsor button.
+You can find the documentation at this [site](https://eclipsingbinaries.readthedocs.io/en/latest/?badge=latest#) and any questions can be talked about in the discussions page or in an issue.
+
+***
+
+## OS and Python Versions Stable On
+
+The list of OS's and Python versions listed below have been tested to be able to build the package on.
+
+*  Macos- 3.8, 3.9, 3.10
+*  Ubuntu- 3.8, 3.9, 3.10
+*  Windows- 3.8, 3.9, 3.10
 
 ***
 
 ## Installation and Usage
 
 To install type the following,
 
@@ -90,14 +101,10 @@
 *   pandas>=1.1.0
 *   PyAstronomy>=0.18.0
 *   scipy>=1.5.2
 *   statsmodels>=0.13.5
 *   tqdm>=4.64.1
 *   numba>=0.56.3
 *   seaborn>=0.12.2
-*   pyia>=1.3
+*   pyia>=1.41
 
 ***
-
-## Documentation
-
-You can find the documentation at this site https://eclipsingbinaries.readthedocs.io/en/latest/?badge=latest# and any questions can be talked about in the discussions page or in an issue.
```

### Comparing `EclipsingBinaries-4.0.6/EclipsingBinaries.egg-info/SOURCES.txt` & `EclipsingBinaries-4.0.7/EclipsingBinaries.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,14 @@
 requirements.txt
 setup.cfg
 setup.py
 tox.ini
 .github/ISSUE_TEMPLATE/bug_report.md
 .github/ISSUE_TEMPLATE/feature_request.md
 .github/workflows/ci_tests.yml
-.github/workflows/codeql.yml
 .github/workflows/python-publish.yml
 EclipsingBinaries/IRAF_Reduction.py
 EclipsingBinaries/Night_Filters.py
 EclipsingBinaries/OC_plot.py
 EclipsingBinaries/OConnell.py
 EclipsingBinaries/__init__.py
 EclipsingBinaries/apass.py
@@ -53,14 +52,15 @@
 EclipsingBinaries/examples/overlay_example.png
 EclipsingBinaries/examples/test_B.txt
 EclipsingBinaries/examples/test_R.txt
 EclipsingBinaries/examples/test_V.txt
 EclipsingBinaries/examples/test_minimums.txt
 EclipsingBinaries/examples/calibration_images/purpose.txt
 EclipsingBinaries/tests/__init__.py
+EclipsingBinaries/tests/test_IRAF_Reduction.py
 EclipsingBinaries/tests/test_OC_plot.py
 EclipsingBinaries/tests/test_apass.py
 changelog/package-lock.json
 changelog/package.json
 docs/EB.rst
 docs/__init__.py
 docs/changelog.rst
```

### Comparing `EclipsingBinaries-4.0.6/PKG-INFO` & `EclipsingBinaries-4.0.7/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,52 +1,63 @@
 Metadata-Version: 2.1
 Name: EclipsingBinaries
-Version: 4.0.6
+Version: 4.0.7
 Summary: "Binary Star Package for Ball State University's Astronomy Research Group"
 Home-page: https://eclipsingbinaries.readthedocs.io/
 Author: Kyle Koeller
 License: MIT
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: numpy>=1.21
-Requires-Dist: astropy>=5.1.1
+Requires-Dist: astropy>=5.2.2
 Requires-Dist: astroquery>=0.4.6
 Requires-Dist: ccdproc>=2.4.0
-Requires-Dist: matplotlib>=3.3.1
-Requires-Dist: pandas>=1.1.0
-Requires-Dist: PyAstronomy>=0.18.0
-Requires-Dist: scipy>=1.5.2
+Requires-Dist: matplotlib>=3.5.1
+Requires-Dist: numpy>=1.22.3
+Requires-Dist: pandas>=1.4.2
+Requires-Dist: PyAstronomy>=0.18.1
+Requires-Dist: scipy>=1.9.3
 Requires-Dist: statsmodels>=0.13.5
 Requires-Dist: tqdm>=4.64.1
-Requires-Dist: numba>=0.56.3
+Requires-Dist: numba>=0.57.0
 Requires-Dist: seaborn>=0.12.2
-Requires-Dist: pyia>=1.3
+Requires-Dist: pyia<=1.41
 Requires-Dist: photutils>=1.8.0
+Requires-Dist: sphinx>=5
 Provides-Extra: docs
 Requires-Dist: sphinx-astropy; extra == "docs"
 Requires-Dist: matplotlib; extra == "docs"
 
 [![Python OS 3.8, 3.9, 3.10](https://github.com/kjkoeller/Binary_Star_Research_Package/actions/workflows/ci_tests.yml/badge.svg)](https://github.com/kjkoeller/Binary_Star_Research_Package/actions/workflows/ci_tests.yml)
 [![Documentation Status](https://readthedocs.org/projects/eclipsingbinaries/badge/?version=latest)](https://eclipsingbinaries.readthedocs.io/en/latest/?badge=latest)
 [![PyPI version](https://badge.fury.io/py/EclipsingBinaries.svg)](https://badge.fury.io/py/EclipsingBinaries)
 [![GitHub release](https://img.shields.io/github/v/release/kjkoeller/Variable_Star_Research_Package)](https://github.com/kjkoeller/Variable_Star_Research_Package/releases/)
 ![GitHub](https://img.shields.io/github/license/kjkoeller/Variable_Star_Research_Package)
 [![Codacy Badge](https://app.codacy.com/project/badge/Grade/9cd9a15e47ab4ed7b78071d096ea099d)](https://www.codacy.com/gh/kjkoeller/EclipsingBinaries/dashboard?utm_source=github.com\&utm_medium=referral\&utm_content=kjkoeller/EclipsingBinaries\&utm_campaign=Badge_Grade)
 [![astropy](http://img.shields.io/badge/powered%20by-AstroPy-orange.svg?style=flat)](http://www.astropy.org/)
 
-# Binary Star Research Package
+# EclipsingBinaries
 
-A Python project for Ball State University's Variable Star Research Group. Check the [Wiki](https://github.com/kjkoeller/EclipsingBinaries/wiki) for more detailed descriptions than the ones below and for usage details of each program.
+A Python project for Ball State University's Variable Star Research Group. The package can currently reduce data, find comparison stars from the APASS catalog, calculate and plot O-C values, find the color index and effective temperature, O'Connell effect parameters, and download TESS data and calculate TESS magnitudes from Gaia data.
 
 ***
 
-## Sponsor
+## Documentation
 
-If you would like to sponsor this project go [here](https://github.com/sponsors/kjkoeller) and click the sponsor button.
+You can find the documentation at this [site](https://eclipsingbinaries.readthedocs.io/en/latest/?badge=latest#) and any questions can be talked about in the discussions page or in an issue.
+
+***
+
+## OS and Python Versions Stable On
+
+The list of OS's and Python versions listed below have been tested to be able to build the package on.
+
+*  Macos- 3.8, 3.9, 3.10
+*  Ubuntu- 3.8, 3.9, 3.10
+*  Windows- 3.8, 3.9, 3.10
 
 ***
 
 ## Installation and Usage
 
 To install type the following,
 
@@ -90,14 +101,10 @@
 *   pandas>=1.1.0
 *   PyAstronomy>=0.18.0
 *   scipy>=1.5.2
 *   statsmodels>=0.13.5
 *   tqdm>=4.64.1
 *   numba>=0.56.3
 *   seaborn>=0.12.2
-*   pyia>=1.3
+*   pyia>=1.41
 
 ***
-
-## Documentation
-
-You can find the documentation at this site https://eclipsingbinaries.readthedocs.io/en/latest/?badge=latest# and any questions can be talked about in the discussions page or in an issue.
```

### Comparing `EclipsingBinaries-4.0.6/README.md` & `EclipsingBinaries-4.0.7/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -2,23 +2,33 @@
 [![Documentation Status](https://readthedocs.org/projects/eclipsingbinaries/badge/?version=latest)](https://eclipsingbinaries.readthedocs.io/en/latest/?badge=latest)
 [![PyPI version](https://badge.fury.io/py/EclipsingBinaries.svg)](https://badge.fury.io/py/EclipsingBinaries)
 [![GitHub release](https://img.shields.io/github/v/release/kjkoeller/Variable_Star_Research_Package)](https://github.com/kjkoeller/Variable_Star_Research_Package/releases/)
 ![GitHub](https://img.shields.io/github/license/kjkoeller/Variable_Star_Research_Package)
 [![Codacy Badge](https://app.codacy.com/project/badge/Grade/9cd9a15e47ab4ed7b78071d096ea099d)](https://www.codacy.com/gh/kjkoeller/EclipsingBinaries/dashboard?utm_source=github.com\&utm_medium=referral\&utm_content=kjkoeller/EclipsingBinaries\&utm_campaign=Badge_Grade)
 [![astropy](http://img.shields.io/badge/powered%20by-AstroPy-orange.svg?style=flat)](http://www.astropy.org/)
 
-# Binary Star Research Package
+# EclipsingBinaries
 
-A Python project for Ball State University's Variable Star Research Group. Check the [Wiki](https://github.com/kjkoeller/EclipsingBinaries/wiki) for more detailed descriptions than the ones below and for usage details of each program.
+A Python project for Ball State University's Variable Star Research Group. The package can currently reduce data, find comparison stars from the APASS catalog, calculate and plot O-C values, find the color index and effective temperature, O'Connell effect parameters, and download TESS data and calculate TESS magnitudes from Gaia data.
 
 ***
 
-## Sponsor
+## Documentation
 
-If you would like to sponsor this project go [here](https://github.com/sponsors/kjkoeller) and click the sponsor button.
+You can find the documentation at this [site](https://eclipsingbinaries.readthedocs.io/en/latest/?badge=latest#) and any questions can be talked about in the discussions page or in an issue.
+
+***
+
+## OS and Python Versions Stable On
+
+The list of OS's and Python versions listed below have been tested to be able to build the package on.
+
+*  Macos- 3.8, 3.9, 3.10
+*  Ubuntu- 3.8, 3.9, 3.10
+*  Windows- 3.8, 3.9, 3.10
 
 ***
 
 ## Installation and Usage
 
 To install type the following,
 
@@ -62,14 +72,10 @@
 *   pandas>=1.1.0
 *   PyAstronomy>=0.18.0
 *   scipy>=1.5.2
 *   statsmodels>=0.13.5
 *   tqdm>=4.64.1
 *   numba>=0.56.3
 *   seaborn>=0.12.2
-*   pyia>=1.3
+*   pyia>=1.41
 
 ***
-
-## Documentation
-
-You can find the documentation at this site https://eclipsingbinaries.readthedocs.io/en/latest/?badge=latest# and any questions can be talked about in the discussions page or in an issue.
```

### Comparing `EclipsingBinaries-4.0.6/changelog/package-lock.json` & `EclipsingBinaries-4.0.7/changelog/package-lock.json`

 * *Files identical despite different names*

### Comparing `EclipsingBinaries-4.0.6/changelog/package.json` & `EclipsingBinaries-4.0.7/changelog/package.json`

 * *Files identical despite different names*

### Comparing `EclipsingBinaries-4.0.6/docs/conf.py` & `EclipsingBinaries-4.0.7/docs/conf.py`

 * *Files 4% similar despite different names*

```diff
@@ -38,15 +38,14 @@
 # The master toctree document.
 root_doc = 'index'
 
 man_pages = [('index', project.lower(), project + u' Documentation',
               [author], 1)]
 
 # -- General configuration
-
 extensions = [
     'sphinx.ext.duration',
     'sphinx.ext.doctest',
     'sphinx.ext.autodoc',
     'sphinx.ext.autosummary',
     'sphinx.ext.intersphinx',
 ]
@@ -56,16 +55,16 @@
     'sphinx': ('https://www.sphinx-doc.org/en/master/', None),
 }
 intersphinx_disabled_domains = ['std']
 
 templates_path = ['_templates']
 
 # -- Options for HTML output
-
-# html_theme = 'sphinx_rtd_theme'
+html_theme = "classic"
 
 # -- Options for EPUB output
 # epub_show_urls = 'footnote'
-
 # github_issues_url = 'https://github.com/astropy/ccdproc/issues/'
 # nitpicky = True
 
+
+
```

### Comparing `EclipsingBinaries-4.0.6/docs/contributing.rst` & `EclipsingBinaries-4.0.7/docs/contributing.rst`

 * *Files identical despite different names*

### Comparing `EclipsingBinaries-4.0.6/docs/index.rst` & `EclipsingBinaries-4.0.7/docs/index.rst`

 * *Files identical despite different names*

### Comparing `EclipsingBinaries-4.0.6/docs/installation.rst` & `EclipsingBinaries-4.0.7/docs/installation.rst`

 * *Files 22% similar despite different names*

```diff
@@ -3,27 +3,28 @@
 ************
 
 Requirements
 ============
 
 EclipsingBinaries has the following requirements:
 
-- astropy>=5.1.1
+- astropy>=6.0.0
 - astroquery>=0.4.6
 - ccdproc>=2.4.0
-- matplotlib>=3.3.1
-- numpy>=1.19.1
-- pandas>=1.1.0
-- PyAstronomy>=0.18.0
-- scipy>=1.5.2
+- matplotlib>=3.5.1
+- numpy>=1.22.3
+- pandas>=1.4.2
+- PyAstronomy>=0.18.1
+- scipy>=1.9.3
 - statsmodels>=0.13.5
 - tqdm>=4.64.1
-- numba>=0.56.3
+- numba>=0.57.0
 - seaborn>=0.12.2
-- pyia>=1.3
+- pyia>=1.41
+- photutils>=1.8.0
 
 
 Installing EclipsingBinaries
 ============================
 
 To install ccdproc with `pip <https://pip.pypa.io/en/latest/>`_, simply run::
```

### Comparing `EclipsingBinaries-4.0.6/docs/pipeline.rst` & `EclipsingBinaries-4.0.7/docs/pipeline.rst`

 * *Files identical despite different names*

### Comparing `EclipsingBinaries-4.0.6/docs/toolbox.rst` & `EclipsingBinaries-4.0.7/docs/toolbox.rst`

 * *Files identical despite different names*

### Comparing `EclipsingBinaries-4.0.6/setup.cfg` & `EclipsingBinaries-4.0.7/setup.cfg`

 * *Files 4% similar despite different names*

```diff
@@ -25,28 +25,29 @@
 github_project = kjkoeller/EclipsingBinaries
 
 [options]
 packages = find:
 zip_safe = False
 setup_requires = setuptools_scm
 install_requires = 
-	numpy>=1.21
-	astropy>=5.1.1
+	astropy>=5.2.2
 	astroquery>=0.4.6
 	ccdproc>=2.4.0
-	matplotlib>=3.3.1
-	pandas>=1.1.0
-	PyAstronomy>=0.18.0
-	scipy>=1.5.2
+	matplotlib>=3.5.1
+	numpy>=1.22.3
+	pandas>=1.4.2
+	PyAstronomy>=0.18.1
+	scipy>=1.9.3
 	statsmodels>=0.13.5
 	tqdm>=4.64.1
-	numba>=0.56.3
+	numba>=0.57.0
 	seaborn>=0.12.2
-	pyia>=1.3
+	pyia<=1.41
 	photutils>=1.8.0
+	sphinx >=5
 python_requires = >=3.8
 test_require = pytest
 include_package_data = True
 
 [aliases]
 test = pytest
```

### Comparing `EclipsingBinaries-4.0.6/tox.ini` & `EclipsingBinaries-4.0.7/tox.ini`

 * *Files identical despite different names*

