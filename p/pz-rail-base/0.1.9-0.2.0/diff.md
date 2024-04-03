# Comparing `tmp/pz-rail-base-0.1.9.tar.gz` & `tmp/pz-rail-base-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pz-rail-base-0.1.9.tar", last modified: Mon Nov 27 18:05:47 2023, max compression
+gzip compressed data, was "pz-rail-base-0.2.0.tar", last modified: Wed Apr  3 16:51:38 2024, max compression
```

## Comparing `pz-rail-base-0.1.9.tar` & `pz-rail-base-0.2.0.tar`

### file list

```diff
@@ -1,152 +1,152 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-27 18:05:47.792651 pz-rail-base-0.1.9/
--rw-r--r--   0 runner    (1001) docker     (127)      268 2023-11-27 18:05:33.000000 pz-rail-base-0.1.9/.copier-answers.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-27 18:05:47.760650 pz-rail-base-0.1.9/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-27 18:05:47.760650 pz-rail-base-0.1.9/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (127)      101 2023-11-27 18:05:33.000000 pz-rail-base-0.1.9/.github/ISSUE_TEMPLATE/0-general_issue.md
--rw-r--r--   0 runner    (1001) docker     (127)      661 2023-11-27 18:05:33.000000 pz-rail-base-0.1.9/.github/ISSUE_TEMPLATE/1-bug_report.md
--rw-r--r--   0 runner    (1001) docker     (127)      707 2023-11-27 18:05:33.000000 pz-rail-base-0.1.9/.github/ISSUE_TEMPLATE/2-feature_request.md
--rw-r--r--   0 runner    (1001) docker     (127)      783 2023-11-27 18:05:33.000000 pz-rail-base-0.1.9/.github/pull_request_template.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-27 18:05:47.760650 pz-rail-base-0.1.9/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      488 2023-11-27 18:05:33.000000 pz-rail-base-0.1.9/.github/workflows/add-issue-to-project-tracker.yml
--rw-r--r--   0 runner    (1001) docker     (127)      977 2023-11-27 18:05:33.000000 pz-rail-base-0.1.9/.github/workflows/linting.yml
--rw-r--r--   0 runner    (1001) docker     (127)      950 2023-11-27 18:05:33.000000 pz-rail-base-0.1.9/.github/workflows/publish-to-pypi.yml
--rw-r--r--   0 runner    (1001) docker     (127)      931 2023-11-27 18:05:33.000000 pz-rail-base-0.1.9/.github/workflows/smoke-test.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1111 2023-11-27 18:05:33.000000 pz-rail-base-0.1.9/.github/workflows/testing-and-coverage.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1912 2023-11-27 18:05:33.000000 pz-rail-base-0.1.9/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     2623 2023-11-27 18:05:33.000000 pz-rail-base-0.1.9/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1102 2023-11-27 18:05:33.000000 pz-rail-base-0.1.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     5740 2023-11-27 18:05:47.792651 pz-rail-base-0.1.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3520 2023-11-27 18:05:33.000000 pz-rail-base-0.1.9/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      163 2023-11-27 18:05:33.000000 pz-rail-base-0.1.9/environment.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1886 2023-11-27 18:05:33.000000 pz-rail-base-0.1.9/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       14 2023-11-27 18:05:33.000000 pz-rail-base-0.1.9/rail_packages.yml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-11-27 18:05:47.792651 pz-rail-base-0.1.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       70 2023-11-27 18:05:33.000000 pz-rail-base-0.1.9/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-27 18:05:47.752650 pz-rail-base-0.1.9/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-27 18:05:47.792651 pz-rail-base-0.1.9/src/pz_rail_base.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5740 2023-11-27 18:05:47.000000 pz-rail-base-0.1.9/src/pz_rail_base.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5081 2023-11-27 18:05:47.000000 pz-rail-base-0.1.9/src/pz_rail_base.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-27 18:05:47.000000 pz-rail-base-0.1.9/src/pz_rail_base.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       47 2023-11-27 18:05:47.000000 pz-rail-base-0.1.9/src/pz_rail_base.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      136 2023-11-27 18:05:47.000000 pz-rail-base-0.1.9/src/pz_rail_base.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2023-11-27 18:05:47.000000 pz-rail-base-0.1.9/src/pz_rail_base.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-27 18:05:47.756650 pz-rail-base-0.1.9/src/rail/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-27 18:05:47.764650 pz-rail-base-0.1.9/src/rail/cli/
--rw-r--r--   0 runner    (1001) docker     (127)     1910 2023-11-27 18:05:33.000000 pz-rail-base-0.1.9/src/rail/cli/commands.py
--rw-r--r--   0 runner    (1001) docker     (127)     3610 2023-11-27 18:05:33.000000 pz-rail-base-0.1.9/src/rail/cli/options.py
--rw-r--r--   0 runner    (1001) docker     (127)     6219 2023-11-27 18:05:33.000000 pz-rail-base-0.1.9/src/rail/cli/scripts.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-27 18:05:47.764650 pz-rail-base-0.1.9/src/rail/core/
--rw-r--r--   0 runner    (1001) docker     (127)      659 2023-11-27 18:05:33.000000 pz-rail-base-0.1.9/src/rail/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2023-11-27 18:05:47.000000 pz-rail-base-0.1.9/src/rail/core/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     2886 2023-11-27 18:05:33.000000 pz-rail-base-0.1.9/src/rail/core/algo_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2283 2023-11-27 18:05:33.000000 pz-rail-base-0.1.9/src/rail/core/common_params.py
--rw-r--r--   0 runner    (1001) docker     (127)    17153 2023-11-27 18:05:33.000000 pz-rail-base-0.1.9/src/rail/core/data.py
--rw-r--r--   0 runner    (1001) docker     (127)    10923 2023-11-27 18:05:33.000000 pz-rail-base-0.1.9/src/rail/core/introspection.py
--rw-r--r--   0 runner    (1001) docker     (127)     4523 2023-11-27 18:05:33.000000 pz-rail-base-0.1.9/src/rail/core/point_estimation.py
--rw-r--r--   0 runner    (1001) docker     (127)    14484 2023-11-27 18:05:33.000000 pz-rail-base-0.1.9/src/rail/core/stage.py
--rw-r--r--   0 runner    (1001) docker     (127)     4301 2023-11-27 18:05:33.000000 pz-rail-base-0.1.9/src/rail/core/util_stages.py
--rw-r--r--   0 runner    (1001) docker     (127)      622 2023-11-27 18:05:33.000000 pz-rail-base-0.1.9/src/rail/core/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-27 18:05:47.764650 pz-rail-base-0.1.9/src/rail/creation/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-27 18:05:47.764650 pz-rail-base-0.1.9/src/rail/creation/degradation/
--rw-r--r--   0 runner    (1001) docker     (127)     4287 2023-11-27 18:05:33.000000 pz-rail-base-0.1.9/src/rail/creation/degradation/quantityCut.py
--rw-r--r--   0 runner    (1001) docker     (127)    22129 2023-11-27 18:05:33.000000 pz-rail-base-0.1.9/src/rail/creation/degradation/spectroscopic_selections.py
--rw-r--r--   0 runner    (1001) docker     (127)     2039 2023-11-27 18:05:33.000000 pz-rail-base-0.1.9/src/rail/creation/degrader.py
--rw-r--r--   0 runner    (1001) docker     (127)     7071 2023-11-27 18:05:33.000000 pz-rail-base-0.1.9/src/rail/creation/engine.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-27 18:05:47.768650 pz-rail-base-0.1.9/src/rail/estimation/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-27 18:05:47.768650 pz-rail-base-0.1.9/src/rail/estimation/algos/
--rw-r--r--   0 runner    (1001) docker     (127)     2433 2023-11-27 18:05:33.000000 pz-rail-base-0.1.9/src/rail/estimation/algos/equal_count.py
--rw-r--r--   0 runner    (1001) docker     (127)     3251 2023-11-27 18:05:33.000000 pz-rail-base-0.1.9/src/rail/estimation/algos/naive_stack.py
--rw-r--r--   0 runner    (1001) docker     (127)     3548 2023-11-27 18:05:33.000000 pz-rail-base-0.1.9/src/rail/estimation/algos/point_est_hist.py
--rw-r--r--   0 runner    (1001) docker     (127)     2635 2023-11-27 18:05:33.000000 pz-rail-base-0.1.9/src/rail/estimation/algos/random_gauss.py
--rw-r--r--   0 runner    (1001) docker     (127)     3168 2023-11-27 18:05:33.000000 pz-rail-base-0.1.9/src/rail/estimation/algos/train_z.py
--rw-r--r--   0 runner    (1001) docker     (127)     3018 2023-11-27 18:05:33.000000 pz-rail-base-0.1.9/src/rail/estimation/algos/uniform_binning.py
--rw-r--r--   0 runner    (1001) docker     (127)     4838 2023-11-27 18:05:33.000000 pz-rail-base-0.1.9/src/rail/estimation/algos/var_inf.py
--rw-r--r--   0 runner    (1001) docker     (127)     4816 2023-11-27 18:05:33.000000 pz-rail-base-0.1.9/src/rail/estimation/classifier.py
--rw-r--r--   0 runner    (1001) docker     (127)     4767 2023-11-27 18:05:33.000000 pz-rail-base-0.1.9/src/rail/estimation/estimator.py
--rw-r--r--   0 runner    (1001) docker     (127)     4572 2023-11-27 18:05:33.000000 pz-rail-base-0.1.9/src/rail/estimation/informer.py
--rw-r--r--   0 runner    (1001) docker     (127)     7638 2023-11-27 18:05:33.000000 pz-rail-base-0.1.9/src/rail/estimation/summarizer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-27 18:05:47.768650 pz-rail-base-0.1.9/src/rail/evaluation/
--rw-r--r--   0 runner    (1001) docker     (127)     5565 2023-11-27 18:05:33.000000 pz-rail-base-0.1.9/src/rail/evaluation/evaluator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-27 18:05:47.768650 pz-rail-base-0.1.9/src/rail/evaluation/metrics/
--rw-r--r--   0 runner    (1001) docker     (127)      565 2023-11-27 18:05:33.000000 pz-rail-base-0.1.9/src/rail/evaluation/metrics/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     1017 2023-11-27 18:05:33.000000 pz-rail-base-0.1.9/src/rail/evaluation/metrics/cdeloss.py
--rw-r--r--   0 runner    (1001) docker     (127)     3069 2023-11-27 18:05:33.000000 pz-rail-base-0.1.9/src/rail/evaluation/metrics/pointestimates.py
--rw-r--r--   0 runner    (1001) docker     (127)      337 2023-11-27 18:05:33.000000 pz-rail-base-0.1.9/src/rail/evaluation/stats_groups.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-27 18:05:47.768650 pz-rail-base-0.1.9/src/rail/examples_data/
--rw-r--r--   0 runner    (1001) docker     (127)        8 2023-11-27 18:05:33.000000 pz-rail-base-0.1.9/src/rail/examples_data/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-27 18:05:47.756650 pz-rail-base-0.1.9/src/rail/examples_data/creation_data/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-27 18:05:47.768650 pz-rail-base-0.1.9/src/rail/examples_data/creation_data/configs/
--rw-r--r--   0 runner    (1001) docker     (127)      418 2023-11-27 18:05:33.000000 pz-rail-base-0.1.9/src/rail/examples_data/creation_data/configs/flowModeler.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-27 18:05:47.768650 pz-rail-base-0.1.9/src/rail/examples_data/creation_data/data/
--rw-r--r--   0 runner    (1001) docker     (127)      141 2023-11-27 18:05:33.000000 pz-rail-base-0.1.9/src/rail/examples_data/creation_data/data/HSC_grid_settings.pkl
--rw-r--r--   0 runner    (1001) docker     (127)      313 2023-11-27 18:05:33.000000 pz-rail-base-0.1.9/src/rail/examples_data/creation_data/data/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-27 18:05:47.772650 pz-rail-base-0.1.9/src/rail/examples_data/creation_data/data/success_rate_data/
--rw-r--r--   0 runner    (1001) docker     (127)      727 2023-11-27 18:05:33.000000 pz-rail-base-0.1.9/src/rail/examples_data/creation_data/data/success_rate_data/DEEP2_success.txt
--rw-r--r--   0 runner    (1001) docker     (127)      428 2023-11-27 18:05:33.000000 pz-rail-base-0.1.9/src/rail/examples_data/creation_data/data/success_rate_data/VVDSf02_I_success.txt
--rw-r--r--   0 runner    (1001) docker     (127)      973 2023-11-27 18:05:33.000000 pz-rail-base-0.1.9/src/rail/examples_data/creation_data/data/success_rate_data/VVDSf02_z_bright_success.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1873 2023-11-27 18:05:33.000000 pz-rail-base-0.1.9/src/rail/examples_data/creation_data/data/success_rate_data/VVDSf02_z_deep_success.txt
--rw-r--r--   0 runner    (1001) docker     (127)  1000000 2023-11-27 18:05:33.000000 pz-rail-base-0.1.9/src/rail/examples_data/creation_data/data/success_rate_data/hsc_success.txt
--rw-r--r--   0 runner    (1001) docker     (127)   431705 2023-11-27 18:05:33.000000 pz-rail-base-0.1.9/src/rail/examples_data/creation_data/data/success_rate_data/zCOSMOS_success.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-27 18:05:47.756650 pz-rail-base-0.1.9/src/rail/examples_data/estimation_data/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-27 18:05:47.772650 pz-rail-base-0.1.9/src/rail/examples_data/estimation_data/data/
--rw-r--r--   0 runner    (1001) docker     (127)      219 2023-11-27 18:05:33.000000 pz-rail-base-0.1.9/src/rail/examples_data/estimation_data/data/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-27 18:05:47.772650 pz-rail-base-0.1.9/src/rail/examples_data/estimation_data/data/AB/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-27 18:05:33.000000 pz-rail-base-0.1.9/src/rail/examples_data/estimation_data/data/AB/dummy.txt
--rw-r--r--   0 runner    (1001) docker     (127)      454 2023-11-27 18:05:33.000000 pz-rail-base-0.1.9/src/rail/examples_data/estimation_data/data/CWW_HDFN_prior.pkl
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-27 18:05:47.776651 pz-rail-base-0.1.9/src/rail/examples_data/estimation_data/data/FILTER/
--rw-r--r--   0 runner    (1001) docker     (127)    98003 2023-11-27 18:05:33.000000 pz-rail-base-0.1.9/src/rail/examples_data/estimation_data/data/FILTER/DC2LSST_g.res
--rw-r--r--   0 runner    (1001) docker     (127)    95326 2023-11-27 18:05:33.000000 pz-rail-base-0.1.9/src/rail/examples_data/estimation_data/data/FILTER/DC2LSST_i.res
--rw-r--r--   0 runner    (1001) docker     (127)    96635 2023-11-27 18:05:33.000000 pz-rail-base-0.1.9/src/rail/examples_data/estimation_data/data/FILTER/DC2LSST_r.res
--rw-r--r--   0 runner    (1001) docker     (127)    90216 2023-11-27 18:05:33.000000 pz-rail-base-0.1.9/src/rail/examples_data/estimation_data/data/FILTER/DC2LSST_u.res
--rw-r--r--   0 runner    (1001) docker     (127)   100126 2023-11-27 18:05:33.000000 pz-rail-base-0.1.9/src/rail/examples_data/estimation_data/data/FILTER/DC2LSST_y.res
--rw-r--r--   0 runner    (1001) docker     (127)    93013 2023-11-27 18:05:33.000000 pz-rail-base-0.1.9/src/rail/examples_data/estimation_data/data/FILTER/DC2LSST_z.res
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-27 18:05:47.776651 pz-rail-base-0.1.9/src/rail/examples_data/estimation_data/data/SED/
--rwxr-xr-x   0 runner    (1001) docker     (127)      125 2023-11-27 18:05:33.000000 pz-rail-base-0.1.9/src/rail/examples_data/estimation_data/data/SED/CWWSB4.list
--rwxr-xr-x   0 runner    (1001) docker     (127)    43750 2023-11-27 18:05:33.000000 pz-rail-base-0.1.9/src/rail/examples_data/estimation_data/data/SED/El_B2004a.sed
--rwxr-xr-x   0 runner    (1001) docker     (127)    42830 2023-11-27 18:05:33.000000 pz-rail-base-0.1.9/src/rail/examples_data/estimation_data/data/SED/Im_B2004a.sed
--rwxr-xr-x   0 runner    (1001) docker     (127)    72228 2023-11-27 18:05:33.000000 pz-rail-base-0.1.9/src/rail/examples_data/estimation_data/data/SED/SB2_B2004a.sed
--rwxr-xr-x   0 runner    (1001) docker     (127)    68560 2023-11-27 18:05:33.000000 pz-rail-base-0.1.9/src/rail/examples_data/estimation_data/data/SED/SB3_B2004a.sed
--rwxr-xr-x   0 runner    (1001) docker     (127)    43351 2023-11-27 18:05:33.000000 pz-rail-base-0.1.9/src/rail/examples_data/estimation_data/data/SED/Sbc_B2004a.sed
--rwxr-xr-x   0 runner    (1001) docker     (127)    42789 2023-11-27 18:05:33.000000 pz-rail-base-0.1.9/src/rail/examples_data/estimation_data/data/SED/Scd_B2004a.sed
--rwxr-xr-x   0 runner    (1001) docker     (127)   179585 2023-11-27 18:05:33.000000 pz-rail-base-0.1.9/src/rail/examples_data/estimation_data/data/SED/ssp_25Myr_z008.sed
--rwxr-xr-x   0 runner    (1001) docker     (127)   179584 2023-11-27 18:05:33.000000 pz-rail-base-0.1.9/src/rail/examples_data/estimation_data/data/SED/ssp_5Myr_z008.sed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-27 18:05:47.776651 pz-rail-base-0.1.9/src/rail/examples_data/goldenspike_data/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-27 18:05:47.776651 pz-rail-base-0.1.9/src/rail/examples_data/goldenspike_data/configs/
--rw-r--r--   0 runner    (1001) docker     (127)     6052 2023-11-27 18:05:33.000000 pz-rail-base-0.1.9/src/rail/examples_data/goldenspike_data/configs/goldenspike_config.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-27 18:05:47.780650 pz-rail-base-0.1.9/src/rail/examples_data/goldenspike_data/data/
--rw-r--r--   0 runner    (1001) docker     (127)  1158108 2023-11-27 18:05:33.000000 pz-rail-base-0.1.9/src/rail/examples_data/goldenspike_data/data/pretrained_flow.pkl
--rw-r--r--   0 runner    (1001) docker     (127)   873947 2023-11-27 18:05:33.000000 pz-rail-base-0.1.9/src/rail/examples_data/goldenspike_data/data/test_flow_data.pq
--rw-r--r--   0 runner    (1001) docker     (127)     1419 2023-11-27 18:05:33.000000 pz-rail-base-0.1.9/src/rail/examples_data/goldenspike_data/goldenspike.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-27 18:05:47.788650 pz-rail-base-0.1.9/src/rail/examples_data/testdata/
--rw-r--r--   0 runner    (1001) docker     (127)      553 2023-11-27 18:05:33.000000 pz-rail-base-0.1.9/src/rail/examples_data/testdata/README.md
--rw-r--r--   0 runner    (1001) docker     (127)    91936 2023-11-27 18:05:33.000000 pz-rail-base-0.1.9/src/rail/examples_data/testdata/lsst_filters.npy
--rw-r--r--   0 runner    (1001) docker     (127)     4742 2023-11-27 18:05:33.000000 pz-rail-base-0.1.9/src/rail/examples_data/testdata/make_rail_sample_data.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    43200 2023-11-27 18:05:33.000000 pz-rail-base-0.1.9/src/rail/examples_data/testdata/output_BPZ_lite.fits
--rw-r--r--   0 runner    (1001) docker     (127)    37192 2023-11-27 18:05:33.000000 pz-rail-base-0.1.9/src/rail/examples_data/testdata/output_BPZ_lite.hdf5
--rw-r--r--   0 runner    (1001) docker     (127)    24574 2023-11-27 18:05:33.000000 pz-rail-base-0.1.9/src/rail/examples_data/testdata/rubin_dm_dc2_example.pq
--rw-r--r--   0 runner    (1001) docker     (127)   662976 2023-11-27 18:05:33.000000 pz-rail-base-0.1.9/src/rail/examples_data/testdata/test_dc2_training_9816.hdf5
--rw-r--r--   0 runner    (1001) docker     (127)   873930 2023-11-27 18:05:33.000000 pz-rail-base-0.1.9/src/rail/examples_data/testdata/test_dc2_training_9816.pq
--rw-r--r--   0 runner    (1001) docker     (127)  1192254 2023-11-27 18:05:33.000000 pz-rail-base-0.1.9/src/rail/examples_data/testdata/test_dc2_training_9816_hyperbolic.pq
--rw-r--r--   0 runner    (1001) docker     (127)     5625 2023-11-27 18:05:33.000000 pz-rail-base-0.1.9/src/rail/examples_data/testdata/test_dc2_training_9816_smoothing_params.pq
--rw-r--r--   0 runner    (1001) docker     (127)  1316984 2023-11-27 18:05:33.000000 pz-rail-base-0.1.9/src/rail/examples_data/testdata/test_dc2_validation_9816.hdf5
--rw-r--r--   0 runner    (1001) docker     (127)    15192 2023-11-27 18:05:33.000000 pz-rail-base-0.1.9/src/rail/examples_data/testdata/training_100gal.hdf5
--rw-r--r--   0 runner    (1001) docker     (127)     9200 2023-11-27 18:05:33.000000 pz-rail-base-0.1.9/src/rail/examples_data/testdata/validation_10gal.hdf5
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-27 18:05:47.788650 pz-rail-base-0.1.9/src/rail/stages/
--rw-r--r--   0 runner    (1001) docker     (127)     1228 2023-11-27 18:05:33.000000 pz-rail-base-0.1.9/src/rail/stages/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-27 18:05:47.756650 pz-rail-base-0.1.9/tests/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-27 18:05:47.788650 pz-rail-base-0.1.9/tests/cli/
--rw-r--r--   0 runner    (1001) docker     (127)      833 2023-11-27 18:05:33.000000 pz-rail-base-0.1.9/tests/cli/hello_world.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     1095 2023-11-27 18:05:33.000000 pz-rail-base-0.1.9/tests/cli/single_number.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)      974 2023-11-27 18:05:33.000000 pz-rail-base-0.1.9/tests/cli/test_scripts.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-27 18:05:47.792651 pz-rail-base-0.1.9/tests/core/
--rw-r--r--   0 runner    (1001) docker     (127)    10079 2023-11-27 18:05:33.000000 pz-rail-base-0.1.9/tests/core/test_core.py
--rw-r--r--   0 runner    (1001) docker     (127)     5941 2023-11-27 18:05:33.000000 pz-rail-base-0.1.9/tests/core/test_degraders.py
--rw-r--r--   0 runner    (1001) docker     (127)      628 2023-11-27 18:05:33.000000 pz-rail-base-0.1.9/tests/core/test_introspection.py
--rw-r--r--   0 runner    (1001) docker     (127)     2780 2023-11-27 18:05:33.000000 pz-rail-base-0.1.9/tests/core/test_pipeline.py
--rw-r--r--   0 runner    (1001) docker     (127)     2994 2023-11-27 18:05:33.000000 pz-rail-base-0.1.9/tests/core/test_point_estimation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-27 18:05:47.792651 pz-rail-base-0.1.9/tests/estimation/
--rw-r--r--   0 runner    (1001) docker     (127)     1656 2023-11-27 18:05:33.000000 pz-rail-base-0.1.9/tests/estimation/test_algos.py
--rw-r--r--   0 runner    (1001) docker     (127)     4337 2023-11-27 18:05:33.000000 pz-rail-base-0.1.9/tests/estimation/test_classifier.py
--rw-r--r--   0 runner    (1001) docker     (127)     2083 2023-11-27 18:05:33.000000 pz-rail-base-0.1.9/tests/estimation/test_summarizers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-27 18:05:47.792651 pz-rail-base-0.1.9/tests/evaluation/
--rw-r--r--   0 runner    (1001) docker     (127)     2137 2023-11-27 18:05:33.000000 pz-rail-base-0.1.9/tests/evaluation/test_evaluation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 16:51:38.547436 pz-rail-base-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (127)      268 2024-04-03 16:51:31.000000 pz-rail-base-0.2.0/.copier-answers.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 16:51:38.515436 pz-rail-base-0.2.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 16:51:38.515436 pz-rail-base-0.2.0/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-04-03 16:51:31.000000 pz-rail-base-0.2.0/.github/ISSUE_TEMPLATE/0-general_issue.md
+-rw-r--r--   0 runner    (1001) docker     (127)      661 2024-04-03 16:51:31.000000 pz-rail-base-0.2.0/.github/ISSUE_TEMPLATE/1-bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (127)      707 2024-04-03 16:51:31.000000 pz-rail-base-0.2.0/.github/ISSUE_TEMPLATE/2-feature_request.md
+-rw-r--r--   0 runner    (1001) docker     (127)      783 2024-04-03 16:51:31.000000 pz-rail-base-0.2.0/.github/pull_request_template.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 16:51:38.519436 pz-rail-base-0.2.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      488 2024-04-03 16:51:31.000000 pz-rail-base-0.2.0/.github/workflows/add-issue-to-project-tracker.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      977 2024-04-03 16:51:31.000000 pz-rail-base-0.2.0/.github/workflows/linting.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      950 2024-04-03 16:51:31.000000 pz-rail-base-0.2.0/.github/workflows/publish-to-pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      931 2024-04-03 16:51:31.000000 pz-rail-base-0.2.0/.github/workflows/smoke-test.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1111 2024-04-03 16:51:31.000000 pz-rail-base-0.2.0/.github/workflows/testing-and-coverage.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1912 2024-04-03 16:51:31.000000 pz-rail-base-0.2.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     2623 2024-04-03 16:51:31.000000 pz-rail-base-0.2.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1102 2024-04-03 16:51:31.000000 pz-rail-base-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     5736 2024-04-03 16:51:38.547436 pz-rail-base-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3516 2024-04-03 16:51:31.000000 pz-rail-base-0.2.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      163 2024-04-03 16:51:31.000000 pz-rail-base-0.2.0/environment.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1886 2024-04-03 16:51:31.000000 pz-rail-base-0.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-03 16:51:31.000000 pz-rail-base-0.2.0/rail_packages.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-03 16:51:38.547436 pz-rail-base-0.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-04-03 16:51:31.000000 pz-rail-base-0.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 16:51:38.511436 pz-rail-base-0.2.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 16:51:38.543436 pz-rail-base-0.2.0/src/pz_rail_base.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5736 2024-04-03 16:51:38.000000 pz-rail-base-0.2.0/src/pz_rail_base.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5027 2024-04-03 16:51:38.000000 pz-rail-base-0.2.0/src/pz_rail_base.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 16:51:38.000000 pz-rail-base-0.2.0/src/pz_rail_base.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-03 16:51:38.000000 pz-rail-base-0.2.0/src/pz_rail_base.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      136 2024-04-03 16:51:38.000000 pz-rail-base-0.2.0/src/pz_rail_base.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-03 16:51:38.000000 pz-rail-base-0.2.0/src/pz_rail_base.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 16:51:38.515436 pz-rail-base-0.2.0/src/rail/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 16:51:38.519436 pz-rail-base-0.2.0/src/rail/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)     1910 2024-04-03 16:51:31.000000 pz-rail-base-0.2.0/src/rail/cli/commands.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3610 2024-04-03 16:51:31.000000 pz-rail-base-0.2.0/src/rail/cli/options.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6219 2024-04-03 16:51:31.000000 pz-rail-base-0.2.0/src/rail/cli/scripts.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 16:51:38.519436 pz-rail-base-0.2.0/src/rail/core/
+-rw-r--r--   0 runner    (1001) docker     (127)      659 2024-04-03 16:51:31.000000 pz-rail-base-0.2.0/src/rail/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-03 16:51:38.000000 pz-rail-base-0.2.0/src/rail/core/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2890 2024-04-03 16:51:31.000000 pz-rail-base-0.2.0/src/rail/core/algo_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2283 2024-04-03 16:51:31.000000 pz-rail-base-0.2.0/src/rail/core/common_params.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17759 2024-04-03 16:51:31.000000 pz-rail-base-0.2.0/src/rail/core/data.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10923 2024-04-03 16:51:31.000000 pz-rail-base-0.2.0/src/rail/core/introspection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4632 2024-04-03 16:51:31.000000 pz-rail-base-0.2.0/src/rail/core/point_estimation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14432 2024-04-03 16:51:31.000000 pz-rail-base-0.2.0/src/rail/core/stage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4301 2024-04-03 16:51:31.000000 pz-rail-base-0.2.0/src/rail/core/util_stages.py
+-rw-r--r--   0 runner    (1001) docker     (127)      622 2024-04-03 16:51:31.000000 pz-rail-base-0.2.0/src/rail/core/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 16:51:38.523436 pz-rail-base-0.2.0/src/rail/creation/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 16:51:38.523436 pz-rail-base-0.2.0/src/rail/creation/degradation/
+-rw-r--r--   0 runner    (1001) docker     (127)     4287 2024-04-03 16:51:31.000000 pz-rail-base-0.2.0/src/rail/creation/degradation/quantityCut.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2039 2024-04-03 16:51:31.000000 pz-rail-base-0.2.0/src/rail/creation/degrader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7071 2024-04-03 16:51:31.000000 pz-rail-base-0.2.0/src/rail/creation/engine.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 16:51:38.523436 pz-rail-base-0.2.0/src/rail/estimation/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 16:51:38.523436 pz-rail-base-0.2.0/src/rail/estimation/algos/
+-rw-r--r--   0 runner    (1001) docker     (127)     2433 2024-04-03 16:51:31.000000 pz-rail-base-0.2.0/src/rail/estimation/algos/equal_count.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3251 2024-04-03 16:51:31.000000 pz-rail-base-0.2.0/src/rail/estimation/algos/naive_stack.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3548 2024-04-03 16:51:31.000000 pz-rail-base-0.2.0/src/rail/estimation/algos/point_est_hist.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2635 2024-04-03 16:51:31.000000 pz-rail-base-0.2.0/src/rail/estimation/algos/random_gauss.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3168 2024-04-03 16:51:31.000000 pz-rail-base-0.2.0/src/rail/estimation/algos/train_z.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3936 2024-04-03 16:51:31.000000 pz-rail-base-0.2.0/src/rail/estimation/algos/uniform_binning.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4838 2024-04-03 16:51:31.000000 pz-rail-base-0.2.0/src/rail/estimation/algos/var_inf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8041 2024-04-03 16:51:31.000000 pz-rail-base-0.2.0/src/rail/estimation/classifier.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4838 2024-04-03 16:51:31.000000 pz-rail-base-0.2.0/src/rail/estimation/estimator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4572 2024-04-03 16:51:31.000000 pz-rail-base-0.2.0/src/rail/estimation/informer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7638 2024-04-03 16:51:31.000000 pz-rail-base-0.2.0/src/rail/estimation/summarizer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 16:51:38.523436 pz-rail-base-0.2.0/src/rail/evaluation/
+-rw-r--r--   0 runner    (1001) docker     (127)     5891 2024-04-03 16:51:31.000000 pz-rail-base-0.2.0/src/rail/evaluation/evaluator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 16:51:38.523436 pz-rail-base-0.2.0/src/rail/evaluation/metrics/
+-rw-r--r--   0 runner    (1001) docker     (127)      565 2024-04-03 16:51:31.000000 pz-rail-base-0.2.0/src/rail/evaluation/metrics/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1017 2024-04-03 16:51:31.000000 pz-rail-base-0.2.0/src/rail/evaluation/metrics/cdeloss.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2967 2024-04-03 16:51:31.000000 pz-rail-base-0.2.0/src/rail/evaluation/metrics/pointestimates.py
+-rw-r--r--   0 runner    (1001) docker     (127)      338 2024-04-03 16:51:31.000000 pz-rail-base-0.2.0/src/rail/evaluation/stats_groups.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 16:51:38.523436 pz-rail-base-0.2.0/src/rail/examples_data/
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-03 16:51:31.000000 pz-rail-base-0.2.0/src/rail/examples_data/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 16:51:38.511436 pz-rail-base-0.2.0/src/rail/examples_data/creation_data/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 16:51:38.523436 pz-rail-base-0.2.0/src/rail/examples_data/creation_data/configs/
+-rw-r--r--   0 runner    (1001) docker     (127)      418 2024-04-03 16:51:31.000000 pz-rail-base-0.2.0/src/rail/examples_data/creation_data/configs/flowModeler.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 16:51:38.523436 pz-rail-base-0.2.0/src/rail/examples_data/creation_data/data/
+-rw-r--r--   0 runner    (1001) docker     (127)      141 2024-04-03 16:51:31.000000 pz-rail-base-0.2.0/src/rail/examples_data/creation_data/data/HSC_grid_settings.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)      313 2024-04-03 16:51:31.000000 pz-rail-base-0.2.0/src/rail/examples_data/creation_data/data/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 16:51:38.527436 pz-rail-base-0.2.0/src/rail/examples_data/creation_data/data/success_rate_data/
+-rw-r--r--   0 runner    (1001) docker     (127)      727 2024-04-03 16:51:31.000000 pz-rail-base-0.2.0/src/rail/examples_data/creation_data/data/success_rate_data/DEEP2_success.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      428 2024-04-03 16:51:31.000000 pz-rail-base-0.2.0/src/rail/examples_data/creation_data/data/success_rate_data/VVDSf02_I_success.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      973 2024-04-03 16:51:31.000000 pz-rail-base-0.2.0/src/rail/examples_data/creation_data/data/success_rate_data/VVDSf02_z_bright_success.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1873 2024-04-03 16:51:31.000000 pz-rail-base-0.2.0/src/rail/examples_data/creation_data/data/success_rate_data/VVDSf02_z_deep_success.txt
+-rw-r--r--   0 runner    (1001) docker     (127)  1000000 2024-04-03 16:51:31.000000 pz-rail-base-0.2.0/src/rail/examples_data/creation_data/data/success_rate_data/hsc_success.txt
+-rw-r--r--   0 runner    (1001) docker     (127)   431705 2024-04-03 16:51:31.000000 pz-rail-base-0.2.0/src/rail/examples_data/creation_data/data/success_rate_data/zCOSMOS_success.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 16:51:38.511436 pz-rail-base-0.2.0/src/rail/examples_data/estimation_data/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 16:51:38.527436 pz-rail-base-0.2.0/src/rail/examples_data/estimation_data/data/
+-rw-r--r--   0 runner    (1001) docker     (127)      219 2024-04-03 16:51:31.000000 pz-rail-base-0.2.0/src/rail/examples_data/estimation_data/data/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 16:51:38.527436 pz-rail-base-0.2.0/src/rail/examples_data/estimation_data/data/AB/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 16:51:31.000000 pz-rail-base-0.2.0/src/rail/examples_data/estimation_data/data/AB/dummy.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      454 2024-04-03 16:51:31.000000 pz-rail-base-0.2.0/src/rail/examples_data/estimation_data/data/CWW_HDFN_prior.pkl
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 16:51:38.531436 pz-rail-base-0.2.0/src/rail/examples_data/estimation_data/data/FILTER/
+-rw-r--r--   0 runner    (1001) docker     (127)    98003 2024-04-03 16:51:31.000000 pz-rail-base-0.2.0/src/rail/examples_data/estimation_data/data/FILTER/DC2LSST_g.res
+-rw-r--r--   0 runner    (1001) docker     (127)    95326 2024-04-03 16:51:31.000000 pz-rail-base-0.2.0/src/rail/examples_data/estimation_data/data/FILTER/DC2LSST_i.res
+-rw-r--r--   0 runner    (1001) docker     (127)    96635 2024-04-03 16:51:31.000000 pz-rail-base-0.2.0/src/rail/examples_data/estimation_data/data/FILTER/DC2LSST_r.res
+-rw-r--r--   0 runner    (1001) docker     (127)    90216 2024-04-03 16:51:31.000000 pz-rail-base-0.2.0/src/rail/examples_data/estimation_data/data/FILTER/DC2LSST_u.res
+-rw-r--r--   0 runner    (1001) docker     (127)   100126 2024-04-03 16:51:31.000000 pz-rail-base-0.2.0/src/rail/examples_data/estimation_data/data/FILTER/DC2LSST_y.res
+-rw-r--r--   0 runner    (1001) docker     (127)    93013 2024-04-03 16:51:31.000000 pz-rail-base-0.2.0/src/rail/examples_data/estimation_data/data/FILTER/DC2LSST_z.res
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 16:51:38.531436 pz-rail-base-0.2.0/src/rail/examples_data/estimation_data/data/SED/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      125 2024-04-03 16:51:31.000000 pz-rail-base-0.2.0/src/rail/examples_data/estimation_data/data/SED/CWWSB4.list
+-rwxr-xr-x   0 runner    (1001) docker     (127)    43750 2024-04-03 16:51:31.000000 pz-rail-base-0.2.0/src/rail/examples_data/estimation_data/data/SED/El_B2004a.sed
+-rwxr-xr-x   0 runner    (1001) docker     (127)    42830 2024-04-03 16:51:31.000000 pz-rail-base-0.2.0/src/rail/examples_data/estimation_data/data/SED/Im_B2004a.sed
+-rwxr-xr-x   0 runner    (1001) docker     (127)    72228 2024-04-03 16:51:31.000000 pz-rail-base-0.2.0/src/rail/examples_data/estimation_data/data/SED/SB2_B2004a.sed
+-rwxr-xr-x   0 runner    (1001) docker     (127)    68560 2024-04-03 16:51:31.000000 pz-rail-base-0.2.0/src/rail/examples_data/estimation_data/data/SED/SB3_B2004a.sed
+-rwxr-xr-x   0 runner    (1001) docker     (127)    43351 2024-04-03 16:51:31.000000 pz-rail-base-0.2.0/src/rail/examples_data/estimation_data/data/SED/Sbc_B2004a.sed
+-rwxr-xr-x   0 runner    (1001) docker     (127)    42789 2024-04-03 16:51:31.000000 pz-rail-base-0.2.0/src/rail/examples_data/estimation_data/data/SED/Scd_B2004a.sed
+-rwxr-xr-x   0 runner    (1001) docker     (127)   179585 2024-04-03 16:51:31.000000 pz-rail-base-0.2.0/src/rail/examples_data/estimation_data/data/SED/ssp_25Myr_z008.sed
+-rwxr-xr-x   0 runner    (1001) docker     (127)   179584 2024-04-03 16:51:31.000000 pz-rail-base-0.2.0/src/rail/examples_data/estimation_data/data/SED/ssp_5Myr_z008.sed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 16:51:38.531436 pz-rail-base-0.2.0/src/rail/examples_data/goldenspike_data/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 16:51:38.531436 pz-rail-base-0.2.0/src/rail/examples_data/goldenspike_data/configs/
+-rw-r--r--   0 runner    (1001) docker     (127)     6052 2024-04-03 16:51:31.000000 pz-rail-base-0.2.0/src/rail/examples_data/goldenspike_data/configs/goldenspike_config.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 16:51:38.535436 pz-rail-base-0.2.0/src/rail/examples_data/goldenspike_data/data/
+-rw-r--r--   0 runner    (1001) docker     (127)  1158108 2024-04-03 16:51:31.000000 pz-rail-base-0.2.0/src/rail/examples_data/goldenspike_data/data/pretrained_flow.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)   873947 2024-04-03 16:51:31.000000 pz-rail-base-0.2.0/src/rail/examples_data/goldenspike_data/data/test_flow_data.pq
+-rw-r--r--   0 runner    (1001) docker     (127)     1419 2024-04-03 16:51:31.000000 pz-rail-base-0.2.0/src/rail/examples_data/goldenspike_data/goldenspike.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 16:51:38.543436 pz-rail-base-0.2.0/src/rail/examples_data/testdata/
+-rw-r--r--   0 runner    (1001) docker     (127)      553 2024-04-03 16:51:31.000000 pz-rail-base-0.2.0/src/rail/examples_data/testdata/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)    91936 2024-04-03 16:51:31.000000 pz-rail-base-0.2.0/src/rail/examples_data/testdata/lsst_filters.npy
+-rw-r--r--   0 runner    (1001) docker     (127)     4742 2024-04-03 16:51:31.000000 pz-rail-base-0.2.0/src/rail/examples_data/testdata/make_rail_sample_data.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    43200 2024-04-03 16:51:31.000000 pz-rail-base-0.2.0/src/rail/examples_data/testdata/output_BPZ_lite.fits
+-rw-r--r--   0 runner    (1001) docker     (127)    37192 2024-04-03 16:51:31.000000 pz-rail-base-0.2.0/src/rail/examples_data/testdata/output_BPZ_lite.hdf5
+-rw-r--r--   0 runner    (1001) docker     (127)    24574 2024-04-03 16:51:31.000000 pz-rail-base-0.2.0/src/rail/examples_data/testdata/rubin_dm_dc2_example.pq
+-rw-r--r--   0 runner    (1001) docker     (127)   662976 2024-04-03 16:51:31.000000 pz-rail-base-0.2.0/src/rail/examples_data/testdata/test_dc2_training_9816.hdf5
+-rw-r--r--   0 runner    (1001) docker     (127)   873930 2024-04-03 16:51:31.000000 pz-rail-base-0.2.0/src/rail/examples_data/testdata/test_dc2_training_9816.pq
+-rw-r--r--   0 runner    (1001) docker     (127)  1192254 2024-04-03 16:51:31.000000 pz-rail-base-0.2.0/src/rail/examples_data/testdata/test_dc2_training_9816_hyperbolic.pq
+-rw-r--r--   0 runner    (1001) docker     (127)     5625 2024-04-03 16:51:31.000000 pz-rail-base-0.2.0/src/rail/examples_data/testdata/test_dc2_training_9816_smoothing_params.pq
+-rw-r--r--   0 runner    (1001) docker     (127)  1316984 2024-04-03 16:51:31.000000 pz-rail-base-0.2.0/src/rail/examples_data/testdata/test_dc2_validation_9816.hdf5
+-rw-r--r--   0 runner    (1001) docker     (127)    15192 2024-04-03 16:51:31.000000 pz-rail-base-0.2.0/src/rail/examples_data/testdata/training_100gal.hdf5
+-rw-r--r--   0 runner    (1001) docker     (127)     9200 2024-04-03 16:51:31.000000 pz-rail-base-0.2.0/src/rail/examples_data/testdata/validation_10gal.hdf5
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 16:51:38.543436 pz-rail-base-0.2.0/src/rail/stages/
+-rw-r--r--   0 runner    (1001) docker     (127)     1230 2024-04-03 16:51:31.000000 pz-rail-base-0.2.0/src/rail/stages/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 16:51:38.515436 pz-rail-base-0.2.0/tests/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 16:51:38.543436 pz-rail-base-0.2.0/tests/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)      833 2024-04-03 16:51:31.000000 pz-rail-base-0.2.0/tests/cli/hello_world.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     1095 2024-04-03 16:51:31.000000 pz-rail-base-0.2.0/tests/cli/single_number.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)      974 2024-04-03 16:51:31.000000 pz-rail-base-0.2.0/tests/cli/test_scripts.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 16:51:38.543436 pz-rail-base-0.2.0/tests/core/
+-rw-r--r--   0 runner    (1001) docker     (127)    10079 2024-04-03 16:51:31.000000 pz-rail-base-0.2.0/tests/core/test_core.py
+-rw-r--r--   0 runner    (1001) docker     (127)      811 2024-04-03 16:51:31.000000 pz-rail-base-0.2.0/tests/core/test_introspection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2780 2024-04-03 16:51:31.000000 pz-rail-base-0.2.0/tests/core/test_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4521 2024-04-03 16:51:31.000000 pz-rail-base-0.2.0/tests/core/test_point_estimation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 16:51:38.543436 pz-rail-base-0.2.0/tests/creation/
+-rw-r--r--   0 runner    (1001) docker     (127)     2369 2024-04-03 16:51:31.000000 pz-rail-base-0.2.0/tests/creation/test_degraders.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 16:51:38.543436 pz-rail-base-0.2.0/tests/estimation/
+-rw-r--r--   0 runner    (1001) docker     (127)     1656 2024-04-03 16:51:31.000000 pz-rail-base-0.2.0/tests/estimation/test_algos.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4337 2024-04-03 16:51:31.000000 pz-rail-base-0.2.0/tests/estimation/test_classifier.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2083 2024-04-03 16:51:31.000000 pz-rail-base-0.2.0/tests/estimation/test_summarizers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 16:51:38.543436 pz-rail-base-0.2.0/tests/evaluation/
+-rw-r--r--   0 runner    (1001) docker     (127)     2137 2024-04-03 16:51:31.000000 pz-rail-base-0.2.0/tests/evaluation/test_evaluation.py
```

### Comparing `pz-rail-base-0.1.9/.github/ISSUE_TEMPLATE/1-bug_report.md` & `pz-rail-base-0.2.0/.github/ISSUE_TEMPLATE/1-bug_report.md`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.1.9/.github/ISSUE_TEMPLATE/2-feature_request.md` & `pz-rail-base-0.2.0/.github/ISSUE_TEMPLATE/2-feature_request.md`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.1.9/.github/pull_request_template.md` & `pz-rail-base-0.2.0/.github/pull_request_template.md`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.1.9/.github/workflows/linting.yml` & `pz-rail-base-0.2.0/.github/workflows/linting.yml`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.1.9/.github/workflows/publish-to-pypi.yml` & `pz-rail-base-0.2.0/.github/workflows/publish-to-pypi.yml`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.1.9/.github/workflows/smoke-test.yml` & `pz-rail-base-0.2.0/.github/workflows/smoke-test.yml`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.1.9/.github/workflows/testing-and-coverage.yml` & `pz-rail-base-0.2.0/.github/workflows/testing-and-coverage.yml`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.1.9/.gitignore` & `pz-rail-base-0.2.0/.gitignore`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.1.9/.pre-commit-config.yaml` & `pz-rail-base-0.2.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.1.9/LICENSE` & `pz-rail-base-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.1.9/PKG-INFO` & `pz-rail-base-0.2.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pz-rail-base
-Version: 0.1.9
+Version: 0.2.0
 Author-email: "LSST Dark Energy Science Collaboration (DESC)" <later@later.com>
 License: MIT License
         
         Copyright (c) 2023 LSST Dark Energy Science Collaboration (DESC)
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
@@ -60,15 +60,15 @@
 
 # RAIL: Redshift Assessment Infrastructure Layers
 
 RAIL is a flexible software library providing tools to produce at-scale
 photometric redshift data products, including uncertainties and summary
 statistics, and stress-test them under realistically complex systematics.
 A detailed description of RAIL's modular structure is available in the 
-[Overview](https://lsstdescrail.readthedocs.io/en/latest/source/overview.html) 
+[Overview](https://rail-hub.readthedocs.io/en/latest/source/overview.html) 
 on ReadTheDocs.
 
 RAIL serves as the infrastructure supporting many extragalactic applications 
 of the Legacy Survey of Space and Time (LSST) on the Vera C. Rubin Observatory,
 including Rubin-wide commissioning activities. RAIL was initiated by the
 Photometric Redshifts (PZ) Working Group (WG) of the LSST Dark Energy Science 
 Collaboration (DESC) as a result of the lessons learned from the
```

### Comparing `pz-rail-base-0.1.9/README.md` & `pz-rail-base-0.2.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 # RAIL: Redshift Assessment Infrastructure Layers
 
 RAIL is a flexible software library providing tools to produce at-scale
 photometric redshift data products, including uncertainties and summary
 statistics, and stress-test them under realistically complex systematics.
 A detailed description of RAIL's modular structure is available in the 
-[Overview](https://lsstdescrail.readthedocs.io/en/latest/source/overview.html) 
+[Overview](https://rail-hub.readthedocs.io/en/latest/source/overview.html) 
 on ReadTheDocs.
 
 RAIL serves as the infrastructure supporting many extragalactic applications 
 of the Legacy Survey of Space and Time (LSST) on the Vera C. Rubin Observatory,
 including Rubin-wide commissioning activities. RAIL was initiated by the
 Photometric Redshifts (PZ) Working Group (WG) of the LSST Dark Energy Science 
 Collaboration (DESC) as a result of the lessons learned from the
```

### Comparing `pz-rail-base-0.1.9/pyproject.toml` & `pz-rail-base-0.2.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.1.9/src/pz_rail_base.egg-info/PKG-INFO` & `pz-rail-base-0.2.0/src/pz_rail_base.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pz-rail-base
-Version: 0.1.9
+Version: 0.2.0
 Author-email: "LSST Dark Energy Science Collaboration (DESC)" <later@later.com>
 License: MIT License
         
         Copyright (c) 2023 LSST Dark Energy Science Collaboration (DESC)
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
@@ -60,15 +60,15 @@
 
 # RAIL: Redshift Assessment Infrastructure Layers
 
 RAIL is a flexible software library providing tools to produce at-scale
 photometric redshift data products, including uncertainties and summary
 statistics, and stress-test them under realistically complex systematics.
 A detailed description of RAIL's modular structure is available in the 
-[Overview](https://lsstdescrail.readthedocs.io/en/latest/source/overview.html) 
+[Overview](https://rail-hub.readthedocs.io/en/latest/source/overview.html) 
 on ReadTheDocs.
 
 RAIL serves as the infrastructure supporting many extragalactic applications 
 of the Legacy Survey of Space and Time (LSST) on the Vera C. Rubin Observatory,
 including Rubin-wide commissioning activities. RAIL was initiated by the
 Photometric Redshifts (PZ) Working Group (WG) of the LSST Dark Energy Science 
 Collaboration (DESC) as a result of the lessons learned from the
```

### Comparing `pz-rail-base-0.1.9/src/pz_rail_base.egg-info/SOURCES.txt` & `pz-rail-base-0.2.0/src/pz_rail_base.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -34,15 +34,14 @@
 src/rail/core/point_estimation.py
 src/rail/core/stage.py
 src/rail/core/util_stages.py
 src/rail/core/utils.py
 src/rail/creation/degrader.py
 src/rail/creation/engine.py
 src/rail/creation/degradation/quantityCut.py
-src/rail/creation/degradation/spectroscopic_selections.py
 src/rail/estimation/classifier.py
 src/rail/estimation/estimator.py
 src/rail/estimation/informer.py
 src/rail/estimation/summarizer.py
 src/rail/estimation/algos/equal_count.py
 src/rail/estimation/algos/naive_stack.py
 src/rail/estimation/algos/point_est_hist.py
@@ -101,15 +100,15 @@
 src/rail/examples_data/testdata/training_100gal.hdf5
 src/rail/examples_data/testdata/validation_10gal.hdf5
 src/rail/stages/__init__.py
 tests/cli/hello_world.ipynb
 tests/cli/single_number.ipynb
 tests/cli/test_scripts.py
 tests/core/test_core.py
-tests/core/test_degraders.py
 tests/core/test_introspection.py
 tests/core/test_pipeline.py
 tests/core/test_point_estimation.py
+tests/creation/test_degraders.py
 tests/estimation/test_algos.py
 tests/estimation/test_classifier.py
 tests/estimation/test_summarizers.py
 tests/evaluation/test_evaluation.py
```

### Comparing `pz-rail-base-0.1.9/src/rail/cli/commands.py` & `pz-rail-base-0.2.0/src/rail/cli/commands.py`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.1.9/src/rail/cli/options.py` & `pz-rail-base-0.2.0/src/rail/cli/options.py`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.1.9/src/rail/cli/scripts.py` & `pz-rail-base-0.2.0/src/rail/cli/scripts.py`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.1.9/src/rail/core/__init__.py` & `pz-rail-base-0.2.0/src/rail/core/__init__.py`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.1.9/src/rail/core/algo_utils.py` & `pz-rail-base-0.2.0/src/rail/core/algo_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,18 +11,18 @@
 validdata = os.path.join(RAILDIR, 'rail/examples_data/testdata/validation_10gal.hdf5')
 DS = RailStage.data_store
 DS.__class__.allow_overwrite = True
 
 
 def one_algo(key, single_trainer, single_estimator, train_kwargs, estim_kwargs, is_classifier=False):
     """
-    A basic test of running an estimator subclass
+    A basic test of running an estimator subclass.
     Run inform, write temporary trained model to
     'tempmodelfile.tmp', run photo-z algorithm.
-    Then, load temp modelfile and re-run, return
+    Then, load tempmodelfile.tmp and re-run, return
     both datasets.
     """
     DS.clear()
     training_data = DS.read_file('training_data', TableHandle, traindata)
     validation_data = DS.read_file('validation_data', TableHandle, validdata)
 
     if single_trainer is not None:
```

### Comparing `pz-rail-base-0.1.9/src/rail/core/common_params.py` & `pz-rail-base-0.2.0/src/rail/core/common_params.py`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.1.9/src/rail/core/data.py` & `pz-rail-base-0.2.0/src/rail/core/data.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,26 +20,44 @@
     path : str or None
         The path to the associated file
     creator : str or None
         The name of the stage that created this data handle
     """
     suffix = ''
 
+    # This is to keep track of all the sub-types
+    data_handle_type_dict = {}
+
     def __init__(self, tag, data=None, path=None, creator=None):
         """Constructor """
         self.tag = tag
         if data is not None:
             self._validate_data(data)
         self.data = data
         self.path = path
         self.creator = creator
         self.fileObj = None
         self.groups = None
         self.partial = False
         self.length = None
+        
+    def __init_subclass__(cls, **kwargs):
+        """Register the subclass with the dict"""
+        cls.data_handle_type_dict[cls.__name__] = cls
+
+    @classmethod
+    def get_sub_class(cls, class_name):
+        """Get a particular subclass by name"""
+        return cls.data_handle_type_dict[class_name]
+
+    @classmethod
+    def print_sub_classes(cls):
+        """Print the list of all the subclasses"""
+        for key, val in cls.data_handle_type_dict.items():
+            print(f"{key}: {val}")    
 
     def open(self, **kwargs):
         """Open and return the associated file
 
         Notes
         -----
         This will simply open the file and return a file-like object to the caller.
@@ -72,15 +90,15 @@
         return self.read(force=True, **kwargs)
 
     @classmethod
     def _read(cls, path, **kwargs):
         raise NotImplementedError("DataHandle._read")  #pragma: no cover
 
     def write(self, **kwargs):
-        """Write the data to the associatied file """
+        """Write the data to the associated file """
         if self.path is None:
             raise ValueError("TableHandle.write() called but path has not been specified")
         if self.data is None:
             raise ValueError(f"TableHandle.write() called for path {self.path} with no data")
         outdir = os.path.dirname(os.path.abspath(os.path.expandvars(self.path)))
         if not os.path.exists(outdir):  #pragma: no cover
             os.makedirs(outdir, exist_ok=True)
@@ -97,15 +115,15 @@
         self.groups, self.fileObj = self._initialize_write(self.data, os.path.expandvars(self.path), data_length, **kwargs)
 
     @classmethod
     def _initialize_write(cls, data, path, data_length, **kwargs):
         raise NotImplementedError("DataHandle._initialize_write") #pragma: no cover
 
     def write_chunk(self, start, end, **kwargs):
-        """Write the data to the associatied file """
+        """Write the data to the associated file """
         if self.data is None:
             raise ValueError(f"TableHandle.write_chunk() called for path {self.path} with no data")
         if self.fileObj is None:
             raise ValueError(f"TableHandle.write_chunk() called before open for {self.tag} : {self.path}")
         return self._write_chunk(self.data, self.fileObj, self.groups, start, end, **kwargs)
 
 
@@ -211,15 +229,15 @@
     @classmethod
     def _read(cls, path, **kwargs):
         """Read and return the data from the associated file """
         return tables_io.read(path, **kwargs)
 
     @classmethod
     def _write(cls, data, path, **kwargs):
-        """Write the data to the associatied file """
+        """Write the data to the associated file """
         return tables_io.write(data, path, **kwargs)
 
     @classmethod
     def _size(cls, path, **kwargs):
         return tables_io.io.getInputDataLengthHdf5(path, **kwargs)
 
     @classmethod
@@ -285,15 +303,15 @@
     @classmethod
     def _read(cls, path, **kwargs):
         """Read and return the data from the associated file """
         return qp.read(path)
 
     @classmethod
     def _write(cls, data, path, **kwargs):
-        """Write the data to the associatied file """
+        """Write the data to the associated file """
         return data.write_to(path)
 
     @classmethod
     def _initialize_write(cls, data, path, data_length, **kwargs):
         comm = kwargs.get('communicator', None)
         return data.initializeHdf5Write(path, data_length, comm)
 
@@ -331,18 +349,20 @@
     """Write the model, this default implementation uses pickle"""
     with open(path, 'wb') as fout:
         pickle.dump(obj=model, file=fout, protocol=pickle.HIGHEST_PROTOCOL)
 
 
 class ModelDict(dict):
     """
-    A specialized dict to keep track of individual estimation models objects: this is just a dict these additional features
+    A specialized dict to keep track of individual estimation models objects.
+    This is just a dict with these additional features:
 
     1. Keys are paths
-    2. There is a read(path, force=False) method that reads a model object and inserts it into the dictionary
+    2. There is a read(path, force=False) method that reads a model object and
+    inserts it into the dictionary
     3. There is a single static instance of this class
     """
     def open(self, path, mode, **kwargs):  #pylint: disable=no-self-use
         """Open the file and return the file handle"""
         return open(path, mode, **kwargs)
 
     def read(self, path, force=False, reader=None, **kwargs):  #pylint: disable=unused-argument
@@ -423,15 +443,15 @@
     def __repr__(self):
         """ A custom representation """
         s = "DataStore\n"
         s += self.__str__()
         return s
 
     def __setitem__(self, key, value):
-        """ Override the __setitem__ to work with `TableHandle` """
+        """ Override the __setitem__ to work with ``TableHandle`` """
         if not isinstance(value, DataHandle):
             raise TypeError(f"Can only add objects of type DataHandle to DataStore, not {type(value)}")
         check = self.get(key)
         if check is not None and not self.allow_overwrite:
             raise ValueError(f"DataStore already has an item with key {key}, of type {type(check)}, created by {check.creator}")
         dict.__setitem__(self, key, value)
         return value
```

### Comparing `pz-rail-base-0.1.9/src/rail/core/introspection.py` & `pz-rail-base-0.2.0/src/rail/core/introspection.py`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.1.9/src/rail/core/point_estimation.py` & `pz-rail-base-0.2.0/src/rail/core/point_estimation.py`

 * *Files 14% similar despite different names*

```diff
@@ -48,15 +48,18 @@
             ancil_dict.update(mean = mean_value)
 
         if 'median' in calculated_point_estimates:
             median_value = self._calculate_median_point_estimate(qp_dist)
             ancil_dict.update(median = median_value)
 
         if calculated_point_estimates:
-            qp_dist.set_ancil(ancil_dict)
+            if qp_dist.ancil is None:
+                qp_dist.set_ancil(ancil_dict)
+            else:
+                qp_dist.add_to_ancil(ancil_dict)
 
         return qp_dist
 
     def _calculate_mode_point_estimate(self, qp_dist, grid=None) -> NDArray:
         """Calculates and returns the mode values for a set of posterior estimates
         in a qp.Ensemble instance.
```

### Comparing `pz-rail-base-0.1.9/src/rail/core/stage.py` & `pz-rail-base-0.2.0/src/rail/core/stage.py`

 * *Files 1% similar despite different names*

```diff
@@ -392,12 +392,11 @@
     def _finalize_tag(self, tag):
         """Finalize the data for a particular tag.
 
         This can be overridden by sub-classes for more complicated behavior
         """
         handle = self.get_handle(tag, allow_missing=True)
         if self.config.output_mode == 'default':
-            if not os.path.exists(handle.path):
-                handle.write()
+            handle.write()
         final_name = PipelineStage._finalize_tag(self, tag)
         handle.path = final_name
         return final_name
```

### Comparing `pz-rail-base-0.1.9/src/rail/core/util_stages.py` & `pz-rail-base-0.2.0/src/rail/core/util_stages.py`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.1.9/src/rail/core/utils.py` & `pz-rail-base-0.2.0/src/rail/core/utils.py`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.1.9/src/rail/creation/degradation/quantityCut.py` & `pz-rail-base-0.2.0/src/rail/creation/degradation/quantityCut.py`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.1.9/src/rail/creation/degrader.py` & `pz-rail-base-0.2.0/src/rail/creation/degrader.py`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.1.9/src/rail/creation/engine.py` & `pz-rail-base-0.2.0/src/rail/creation/engine.py`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.1.9/src/rail/estimation/algos/equal_count.py` & `pz-rail-base-0.2.0/src/rail/estimation/algos/equal_count.py`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.1.9/src/rail/estimation/algos/naive_stack.py` & `pz-rail-base-0.2.0/src/rail/estimation/algos/naive_stack.py`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.1.9/src/rail/estimation/algos/point_est_hist.py` & `pz-rail-base-0.2.0/src/rail/estimation/algos/point_est_hist.py`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.1.9/src/rail/estimation/algos/random_gauss.py` & `pz-rail-base-0.2.0/src/rail/estimation/algos/random_gauss.py`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.1.9/src/rail/estimation/algos/train_z.py` & `pz-rail-base-0.2.0/src/rail/estimation/algos/train_z.py`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.1.9/src/rail/estimation/algos/uniform_binning.py` & `pz-rail-base-0.2.0/src/rail/estimation/algos/uniform_binning.py`

 * *Files 26% similar despite different names*

```diff
@@ -2,67 +2,91 @@
 A classifier that uses pz point estimate to assign
 tomographic bins with uniform binning. 
 """
 
 import numpy as np
 from ceci.config import StageParameter as Param
 from rail.estimation.classifier import PZClassifier
-from rail.core.data import TableHandle
+from rail.core.data import TableHandle, Hdf5Handle
 
 class UniformBinningClassifier(PZClassifier):
-    """Classifier that simply assign tomographic
-    bins based on point estimate according to SRD"""
-
+    """Classifier that simply assigns tomographic bins based on a point estimate 
+    according to SRD.
+    """
     name = 'UniformBinningClassifier'
     config_options = PZClassifier.config_options.copy()
     config_options.update(
         id_name=Param(str, "", msg="Column name for the object ID in the input data, if empty the row index is used as the ID."),
         point_estimate=Param(str, 'zmode', msg="Which point estimate to use"),
         zbin_edges=Param(list, [], msg="The tomographic redshift bin edges. If this is given (contains two or more entries), all settings below will be ignored."),
         zmin=Param(float, 0.0, msg="Minimum redshift of the sample"),
         zmax=Param(float, 3.0, msg="Maximum redshift of the sample"),
         nbins=Param(int, 5, msg="Number of tomographic bins"),
         no_assign=Param(int, -99, msg="Value for no assignment flag"),
         )
-    outputs = [('output', TableHandle)]
-
+    outputs = [('output', Hdf5Handle)]
+    
+    
     def __init__(self, args, comm=None):
+        """Initialize the UniformBinningClassifier.
+
+        Parameters
+        ----------
+        args : dict
+            Configuration arguments for the classifier.
+        comm : MPI.Comm, optional
+            MPI communicator for parallel processing.
+        """
         PZClassifier.__init__(self, args, comm=comm)
+    
 
-    def run(self):
-        test_data = self.get_data('input')
-        npdf = test_data.npdf
-        
+    def _process_chunk(self, start, end, test_data, first):
+        """Process a chunk of data for uniform binning classification.
+
+        Parameters
+        ----------
+        start : int
+            The starting index of the chunk.
+        end : int
+            The ending index of the chunk.
+        test_data : qp.Ensemble
+            The data chunk to be processed.
+        first : bool
+            True if this is the first chunk, False otherwise.
+        """
         try:
             zb = test_data.ancil[self.config.point_estimate]
         except KeyError:
             raise KeyError(f"{self.config.point_estimate} is not contained in the data ancil, you will need to compute it explicitly.")
+        
+        try:
+            npdf = test_data.npdf
+        except KeyError:
+            raise KeyError(f"npdf is not a supported attribute of {type(test_data)}. Are you sure you don't mean to be using a qp ensemble?")
 
         # binning options
         if len(self.config.zbin_edges)>=2:
             # this overwrites all other key words
             # linear binning defined by zmin, zmax, and nbins
             bin_index = np.digitize(zb, self.config.zbin_edges)
             # assign -99 to objects not in any bin:
             bin_index[bin_index==0]=self.config.no_assign
             bin_index[bin_index==len(self.config.zbin_edges)]=self.config.no_assign
-
         else:
             # linear binning defined by zmin, zmax, and nbins
             bin_index = np.digitize(zb, np.linspace(self.config.zmin, self.config.zmax, self.config.nbins+1))
             # assign -99 to objects not in any bin:
             bin_index[bin_index==0]=self.config.no_assign
             bin_index[bin_index==(self.config.nbins+1)]=self.config.no_assign
         
-        
         if self.config.id_name != "":
             # below is commented out and replaced by a redundant line
             # because the data doesn't have ID yet
             # obj_id = test_data[self.config.id_name]
-            obj_id = np.arange(npdf)
+            obj_id = np.arange(test_data.npdf)
         elif self.config.id_name == "":
             # ID set to row index
-            obj_id = np.arange(npdf)
+            obj_id = np.arange(test_data.npdf)
             self.config.id_name="row_index"
         
         class_id = {self.config.id_name: obj_id, "class_id": bin_index}
-        self.add_data('output', class_id)
+        self._do_chunk_output(class_id, start, end, first)
```

### Comparing `pz-rail-base-0.1.9/src/rail/estimation/algos/var_inf.py` & `pz-rail-base-0.2.0/src/rail/estimation/algos/var_inf.py`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.1.9/src/rail/estimation/classifier.py` & `pz-rail-base-0.2.0/src/rail/estimation/estimator.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,54 +1,61 @@
 """
-Abstract base classes defining classifiers.
+Abstract base classes defining Estimators of individual galaxy redshift uncertainties.
 """
-from rail.core.data import QPHandle, TableHandle, ModelHandle
+import gc
+
+from rail.core.common_params import SHARED_PARAMS
+from rail.core.data import TableHandle, QPHandle, ModelHandle
 from rail.core.stage import RailStage
 
+from rail.estimation.informer import CatInformer
+from rail.core.point_estimation import PointEstimationMixin
+# for backwards compatibility
+
+
+class CatEstimator(RailStage, PointEstimationMixin):
+    """The base class for making photo-z posterior estimates from catalog-like inputs
+    (i.e., tables with fluxes in photometric bands among the set of columns)
 
-class CatClassifier(RailStage):  #pragma: no cover
-    """The base class for assigning classes to catalogue-like table.
+    Estimators use a generic "model", the details of which depends on the sub-class.
 
-    Classifier uses a generic "model", the details of which depends on the sub-class.
+    Estimators take as "input" tabular data, apply the photo-z estimation and
+    provide as "output" a ``QPEnsemble``, with per-object p(z).
 
-    CatClassifier take as "input" a catalogue-like table, assign each object into
-    a tomographic bin, and provide as "output" a tabular data which can be appended 
-    to the catalogue.
     """
-    
-    name='CatClassifier'
+
+    name = 'CatEstimator'
     config_options = RailStage.config_options.copy()
-    config_options.update(chunk_size=10000, hdf5_groupname=str)
+    config_options.update(
+        chunk_size=10000,
+        hdf5_groupname=SHARED_PARAMS['hdf5_groupname'],
+        calculated_point_estimates=SHARED_PARAMS['calculated_point_estimates'])
     inputs = [('model', ModelHandle),
               ('input', TableHandle)]
-    outputs = [('output', TableHandle)]
-    
+    outputs = [('output', QPHandle)]
+
     def __init__(self, args, comm=None):
-        """Initialize Classifier"""
+        """Initialize Estimator"""
         RailStage.__init__(self, args, comm=comm)
         self._output_handle = None
         self.model = None
-        if not isinstance(args, dict):  #pragma: no cover
-            args = vars(args)
-        self.open_model(**args)
-        
-    
+
     def open_model(self, **kwargs):
-        """Load the model and/or attach it to this Classifier
+        """Load the model and attach it to this Estimator
 
         Parameters
         ----------
-        model : `object`, `str` or `ModelHandle`
-            Either an object with a trained model,
-            a path pointing to a file that can be read to obtain the trained model,
-            or a `ModelHandle` providing access to the trained model.
+        model : ``object``, ``str`` or ``ModelHandle``
+            Either an object with a trained model, a path pointing to a file
+            that can be read to obtain the trained model, or a `ModelHandle`
+            providing access to the trained model.
 
         Returns
         -------
-        self.model : `object`
+        self.model : ``object``
             The object encapsulating the trained model.
         """
         model = kwargs.get('model', None)
         if model is None or model == 'None':
             self.model = None
             return self.model
         if isinstance(model, str):
@@ -56,87 +63,70 @@
             self.config['model'] = model
             return self.model
         if isinstance(model, ModelHandle):
             if model.has_path:
                 self.config['model'] = model.path
         self.model = self.set_data('model', model)
         return self.model
-        
-        
-    def classify(self, input_data):
-        """The main run method for the classifier, should be implemented
-        in the specific subclass.
-
-        This will attach the input_data to this `CatClassifier`
-        (for introspection and provenance tracking).
 
-        Then it will call the run() and finalize() methods, which need to
-        be implemented by the sub-classes.
+    def estimate(self, input_data):
+        """The main interface method for the photo-z estimation
 
-        The run() method will need to register the data that it creates to this Classifier
-        by using `self.add_data('output', output_data)`.
+        This will attach the input data (defined in ``inputs`` as "input") to this
+        ``Estimator`` (for introspection and provenance tracking). Then call the
+        ``run()`` and ``finalize()`` methods.
+
+        The run method will call ``_process_chunk()``, which needs to be implemented
+        in the subclass, to process input data in batches. See ``RandomGaussEstimator``
+        for a simple example. 
 
-        Finally, this will return a TableHandle providing access to that output data.
+        Finally, this will return a ``QPHandle`` for access to that output data.
 
         Parameters
         ----------
-        input_data : `dict`
-            A dictionary of all input data
+        input_data : ``dict`` or ``ModelHandle``
+            Either a dictionary of all input data or a ``ModelHandle`` providing
+            access to the same
 
         Returns
         -------
-        output: `dict`
-            Class assignment for each galaxy.
+        output: ``QPHandle``
+            Handle providing access to QP ensemble with output data
         """
         self.set_data('input', input_data)
         self.run()
         self.finalize()
         return self.get_handle('output')
-    
 
-    
-class PZClassifier(RailStage):
-    """The base class for assigning classes (tomographic bins) to per-galaxy PZ estimates
-
-    PZClassifier take as "input" a `qp.Ensemble` with per-galaxy PDFs, and
-    provide as "output" a tabular data which can be appended to the catalogue.
-    """
-    
-    name='PZClassifier'
-    config_options = RailStage.config_options.copy()
-    config_options.update(chunk_size=10000)
-    inputs = [('input', QPHandle)]
-    outputs = [('output', TableHandle)]
-    
-    def __init__(self, args, comm=None):
-        """Initialize Classifier"""
-        RailStage.__init__(self, args, comm=comm)
-        
-    def classify(self, input_data):
-        """The main run method for the classifier, should be implemented
-        in the specific subclass.
+    def run(self):
 
-        This will attach the input_data to this `PZClassifier`
-        (for introspection and provenance tracking).
+        self.open_model(**self.config)
 
-        Then it will call the run() and finalize() methods, which need to
-        be implemented by the sub-classes.
+        iterator = self.input_iterator('input')
+        first = True
+        self._initialize_run()
+        self._output_handle = None
+        for s, e, test_data in iterator:
+            print(f"Process {self.rank} running estimator on chunk {s} - {e}")
+            self._process_chunk(s, e, test_data, first)
+            first = False
+            # Running garbage collection manually seems to be needed
+            # to avoid memory growth for some estimators
+            gc.collect()
+        self._finalize_run()
 
-        The run() method will need to register the data that it creates to this Classifier
-        by using `self.add_data('output', output_data)`.
+    def _initialize_run(self):
+        self._output_handle = None
 
-        Finally, this will return a TableHandle providing access to that output data.
+    def _finalize_run(self):
+        self._output_handle.finalize_write()
 
-        Parameters
-        ----------
-        input_data : `qp.Ensemble`
-            Per-galaxy p(z), and any ancilary data associated with it
+    def _process_chunk(self, start, end, data, first):
+        raise NotImplementedError(f"{self.name}._process_chunk is not implemented")  # pragma: no cover
 
-        Returns
-        -------
-        output: `dict`
-            Class assignment for each galaxy.
-        """
-        self.set_data('input', input_data)
-        self.run()
-        self.finalize()
-        return self.get_handle('output')
+    def _do_chunk_output(self, qp_dstn, start, end, first):
+        qp_dstn = self.calculate_point_estimates(qp_dstn)
+        if first:
+            self._output_handle = self.add_handle('output', data=qp_dstn)
+            self._output_handle.initialize_write(self._input_length, communicator=self.comm)
+        self._output_handle.set_data(qp_dstn, partial=True)
+        self._output_handle.write_chunk(start, end)
```

### Comparing `pz-rail-base-0.1.9/src/rail/estimation/estimator.py` & `pz-rail-base-0.2.0/src/rail/estimation/informer.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,132 +1,121 @@
 """
-Abstract base classes defining Estimators of individual galaxy redshift uncertainties
+Abstract base classes for Informers.
+These superstages ingest prior information, including training sets and explicit
+priors, and prepare a model that can be used to produce photo-z data products.
+They are distinguished by their input data types, and the models they output can
+be used for their corresponding Estimator, Summarizer, or Classifier stages.
 """
-import gc
 
-from rail.core.common_params import SHARED_PARAMS
 from rail.core.data import TableHandle, QPHandle, ModelHandle
 from rail.core.stage import RailStage
 
-from rail.estimation.informer import CatInformer
-from rail.core.point_estimation import PointEstimationMixin
-# for backwards compatibility
-
-
-class CatEstimator(RailStage, PointEstimationMixin):
-    """The base class for making photo-z posterior estimates from catalog-like inputs
-    (i.e., tables with fluxes in photometric bands among the set of columns)
+class CatInformer(RailStage):
+    """The base class for informing models used to make photo-z data products  
+    from catalog-like inputs (i.e., tables with fluxes in photometric bands among
+    the set of columns).
 
     Estimators use a generic "model", the details of which depends on the sub-class.
+    Most estimators will have associated Informer classes, which can be used to inform
+    those models.
 
-    They take as "input" tabular data, apply the photo-z estimation and
-    provide as "output" a QPEnsemble, with per-object p(z).
+    (Note, "Inform" is more generic than "Train" as it also applies to algorithms that
+    are template-based rather than machine learning-based.)
 
+    Informer will produce as output a generic "model", the details of which depends on the sub-class.
+
+    They take as "input" catalog-like tabular data, which is used to "inform" the model.
     """
 
-    name = 'CatEstimator'
+    name = 'CatInformer'
     config_options = RailStage.config_options.copy()
-    config_options.update(
-        chunk_size=10000,
-        hdf5_groupname=SHARED_PARAMS['hdf5_groupname'],
-        calculated_point_estimates=SHARED_PARAMS['calculated_point_estimates'])
-    inputs = [('model', ModelHandle),
-              ('input', TableHandle)]
-    outputs = [('output', QPHandle)]
+    inputs = [('input', TableHandle)]
+    outputs = [('model', ModelHandle)]
 
     def __init__(self, args, comm=None):
-        """Initialize Estimator"""
+        """Initialize Informer that can inform models for redshift estimation """
         RailStage.__init__(self, args, comm=comm)
-        self._output_handle = None
         self.model = None
 
-    def open_model(self, **kwargs):
-        """Load the mode and/or attach it to this Estimator
+    def inform(self, training_data):
+        """The main interface method for Informers
+
+        This will attach the input_data to this `Informer`
+        (for introspection and provenance tracking).
+
+        Then it will call the run() and finalize() methods, which need to
+        be implemented by the sub-classes.
+
+        The run() method will need to register the model that it creates to this Estimator
+        by using `self.add_data('model', model)`.
+
+        Finally, this will return a ModelHandle providing access to the trained model.
 
         Parameters
         ----------
-        model : `object`, `str` or `ModelHandle`
-            Either an object with a trained model,
-            a path pointing to a file that can be read to obtain the trained model,
-            or a `ModelHandle` providing access to the trained model.
+        input_data : `dict` or `TableHandle`
+            dictionary of all input data, or a `TableHandle` providing access to it
 
         Returns
         -------
-        self.model : `object`
-            The object encapsulating the trained model.
+        model : ModelHandle
+            Handle providing access to trained model
         """
-        model = kwargs.get('model', None)
-        if model is None or model == 'None':
-            self.model = None
-            return self.model
-        if isinstance(model, str):
-            self.model = self.set_data('model', data=None, path=model)
-            self.config['model'] = model
-            return self.model
-        if isinstance(model, ModelHandle):
-            if model.has_path:
-                self.config['model'] = model.path
-        self.model = self.set_data('model', model)
-        return self.model
+        self.set_data('input', training_data)
+        self.run()
+        self.finalize()
+        return self.get_handle('model')
+
+class PzInformer(RailStage):
+    """The base class for informing models used to make photo-z data products from
+    existing ensembles of p(z) distributions.
+
+    PzSummarizers can use a generic "model", the details of which depends on the sub-class.
+    Some summaer will have associated PzInformer classes, which can be used to inform
+    those models.
 
-    def estimate(self, input_data):
-        """The main interface method for the photo-z estimation
+    (Note, "Inform" is more generic than "Train" as it also applies to algorithms that
+    are template-based rather than machine learning-based.)
 
-        This will attach the input_data to this `Estimator`
+    PzInformer will produce as output a generic "model", the details of which depends on the sub-class.
+
+    They take as "input" a qp.Ensemble of per-galaxy p(z) data, which is used to "inform" the model.
+    """
+
+    name = 'PzInformer'
+    config_options = RailStage.config_options.copy()
+    inputs = [('input', QPHandle)]
+    outputs = [('model', ModelHandle)]
+
+    def __init__(self, args, comm=None):
+        """Initialize Informer that can inform models for redshift estimation """
+        RailStage.__init__(self, args, comm=comm)
+        self.model = None
+
+    def inform(self, training_data):
+        """The main interface method for Informers
+
+        This will attach the input_data to this `Informer`
         (for introspection and provenance tracking).
 
         Then it will call the run() and finalize() methods, which need to
         be implemented by the sub-classes.
 
-        The run() method will need to register the data that it creates to this Estimator
-        by using `self.add_data('output', output_data)`.
+        The run() method will need to register the model that it creates to this Estimator
+        by using `self.add_data('model', model)`.
 
-        Finally, this will return a QPHandle providing access to that output data.
+        Finally, this will return a ModelHandle providing access to the trained model.
 
         Parameters
         ----------
-        input_data : `dict` or `ModelHandle`
-            Either a dictionary of all input data or a `ModelHandle` providing access to the same
+        input_data :  `qp.Ensemble`
+            Per-galaxy p(z), and any ancilary data associated with it
 
         Returns
         -------
-        output: `QPHandle`
-            Handle providing access to QP ensemble with output data
+        model : ModelHandle
+            Handle providing access to trained model
         """
-        self.set_data('input', input_data)
+        self.set_data('input', training_data)
         self.run()
         self.finalize()
-        return self.get_handle('output')
-
-    def run(self):
-
-        self.open_model(**self.config)
-
-        iterator = self.input_iterator('input')
-        first = True
-        self._initialize_run()
-        self._output_handle = None
-        for s, e, test_data in iterator:
-            print(f"Process {self.rank} running estimator on chunk {s} - {e}")
-            self._process_chunk(s, e, test_data, first)
-            first = False
-            # Running garbage collection manually seems to be needed
-            # to avoid memory growth for some estimators
-            gc.collect()
-        self._finalize_run()
-
-    def _initialize_run(self):
-        self._output_handle = None
-
-    def _finalize_run(self):
-        self._output_handle.finalize_write()
-
-    def _process_chunk(self, start, end, data, first):
-        raise NotImplementedError(f"{self.name}._process_chunk is not implemented")  # pragma: no cover
-
-    def _do_chunk_output(self, qp_dstn, start, end, first):
-        qp_dstn = self.calculate_point_estimates(qp_dstn)
-        if first:
-            self._output_handle = self.add_handle('output', data=qp_dstn)
-            self._output_handle.initialize_write(self._input_length, communicator=self.comm)
-        self._output_handle.set_data(qp_dstn, partial=True)
-        self._output_handle.write_chunk(start, end)
+        return self.get_handle('model')
```

### Comparing `pz-rail-base-0.1.9/src/rail/estimation/summarizer.py` & `pz-rail-base-0.2.0/src/rail/estimation/summarizer.py`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.1.9/src/rail/evaluation/evaluator.py` & `pz-rail-base-0.2.0/src/rail/evaluation/evaluator.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,35 +1,35 @@
 """
-" Abstract base class defining an Evaluator
+Abstract base class defining an Evaluator
 
 The key feature is that the evaluate method.
 """
 
 import numpy as np
 
 from ceci.config import StageParameter as Param
+from qp.metrics.pit import PIT
 from rail.core.data import Hdf5Handle, QPHandle
 from rail.core.stage import RailStage
 from rail.core.common_params import SHARED_PARAMS
-
 from rail.evaluation.metrics.cdeloss import CDELoss
-from qp.metrics.pit import PIT
 from rail.evaluation.metrics.pointestimates import PointSigmaIQR, PointBias, PointOutlierRate, PointSigmaMAD
 
 
 class Evaluator(RailStage):
     """Evaluate the performance of a photo-Z estimator """
 
     name = 'Evaluator'
     config_options = RailStage.config_options.copy()
     config_options.update(zmin=Param(float, 0., msg="min z for grid"),
                           zmax=Param(float, 3.0, msg="max z for grid"),
                           nzbins=Param(int, 301, msg="# of bins in zgrid"),
                           pit_metrics=Param(str, 'all', msg='PIT-based metrics to include'),
                           point_metrics=Param(str, 'all', msg='Point-estimate metrics to include'),
+                          hdf5_groupname=Param(str, '', msg='Name of group in hdf5 where redshift data is located'),
                           do_cde=Param(bool, True, msg='Evaluate CDE Metric'),
                           redshift_col=SHARED_PARAMS)
     inputs = [('input', QPHandle),
               ('truth', Hdf5Handle)]
     outputs = [('output', Hdf5Handle)]
 
     def __init__(self, args, comm=None):
@@ -76,15 +76,20 @@
         -----
         Get the input data from the data store under this stages 'input' tag
         Get the truth data from the data store under this stages 'truth' tag
         Puts the data into the data store under this stages 'output' tag
         """
 
         pz_data = self.get_data('input')
-        z_true = self.get_data('truth')[self.config.redshift_col]
+        if self.config.hdf5_groupname:  # pragma: no cover
+            specz_data = self.get_data('truth')[self.config.hdf5_groupname]
+        else: 
+            specz_data = self.get_data('truth')
+        z_true = specz_data[self.config['redshift_col']]
+
         zgrid = np.linspace(self.config.zmin, self.config.zmax, self.config.nzbins+1)
 
         # Create an instance of the PIT class
         pitobj = PIT(pz_data, z_true)
 
         # Build reference dictionary of the PIT meta-metrics from this PIT instance
         PIT_METRICS = dict(
@@ -108,15 +113,16 @@
             # The result objects of some meta-metrics are bespoke scipy objects with inconsistent fields.
             # Here we do our best to store the relevant fields in `out_table`.
             if isinstance(value, list):  # pragma: no cover
                 out_table[f'PIT_{pit_metric}'] = value
             else:
                 out_table[f'PIT_{pit_metric}_stat'] = [getattr(value, 'statistic', None)]
                 out_table[f'PIT_{pit_metric}_pval'] = [getattr(value, 'p_value', None)]
-                out_table[f'PIT_{pit_metric}_significance_level'] = [getattr(value, 'significance_level', None)]
+                out_table[f'PIT_{pit_metric}_significance_level'] = \
+                    [getattr(value, 'significance_level', None)]
 
         POINT_METRICS = dict(SimgaIQR=PointSigmaIQR,
                              Bias=PointBias,
                              OutlierRate=PointOutlierRate,
                              SigmaMAD=PointSigmaMAD)
         if self.config.point_metrics == 'all':
             point_metrics = list(POINT_METRICS.keys())
```

### Comparing `pz-rail-base-0.1.9/src/rail/evaluation/metrics/base.py` & `pz-rail-base-0.2.0/src/rail/evaluation/metrics/base.py`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.1.9/src/rail/evaluation/metrics/cdeloss.py` & `pz-rail-base-0.2.0/src/rail/evaluation/metrics/cdeloss.py`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.1.9/src/rail/evaluation/metrics/pointestimates.py` & `pz-rail-base-0.2.0/src/rail/evaluation/metrics/pointestimates.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,25 +3,29 @@
 from .base import MetricEvaluator
 
 class PointStatsEz(MetricEvaluator):
     """Copied from PZDC1paper repo. Adapted to remove the cut based on
     magnitude."""
 
     def __init__(self, pzvec, szvec):
-        """An object that takes in the vectors of the point photo-z
+        """ An object that takes in the vectors of the point photo-z
         the spec-z, and the i-band magnitudes for calculating the
         point statistics
-        Parameters:
-        pzvec: Numpy 1d array of the point photo-z values
-        szvec: Numpy 1d array of the spec-z values
-        magvec: Numpy 1d array of the i-band magnitudes
-        imagcut: float: i-band magnitude cut for the sample
+
         Calculates:
-        ez: (pz-sz)/(1+sz), the quantity will be useful for
-          calculating statistics
+        ez = (pz - sz) / (1 + sz), the quantity will be useful for calculating
+        statistics
+
+
+        Parameters
+        ----------
+        pzvec : ndarray
+            Array of the point photo-z values
+        szvec : ndarray
+            array of the spec-z values
         """
         super().__init__(None)
         self.pzs = pzvec
         self.szs = szvec
         ez = (pzvec - szvec) / (1. + szvec)
         self.ez = ez
 
@@ -32,70 +36,72 @@
 
 class PointSigmaIQR(PointStatsEz):
     """Calculate sigmaIQR"""
 
     def evaluate(self):
         """Calculate the width of the e_z distribution
         using the Interquartile range
-        Parameters:
-        imagcut: float: i-band magnitude cut for the sample
-        Returns:
-        sigma_IQR float: width of ez distribution for full sample
-        sigma_IQR_magcut float: width of ez distribution for magcut sample
+
+        Returns
+        -------
+        ``sigma_IQR`` float. Width of ez distribution for full sample
         """
         x75, x25 = np.percentile(self.ez, [75., 25.])
         iqr = x75 - x25
         sigma_iqr = iqr / 1.349
         return sigma_iqr
 
 
 class PointBias(PointStatsEz):
     """calculates the bias of the ez and ez_magcut samples.
 
     In keeping with the Science Book, this is just the median of the ez values
     """
     def evaluate(self):
         """
-        Returns:
-        bias: median of the full ez sample
+        Returns
+        -------
+        ``bias`` ndarray. Median of the full ez sample
         """
         return np.median(self.ez)
 
 
 class PointOutlierRate(PointStatsEz):
     """Calculates the catastrophic outlier rate, defined in the
     Science Book as the number of galaxies with ez larger than
     max(0.06,3sigma).  This keeps the fraction reasonable when
     sigma is very small.
     """
 
     def evaluate(self):
         """
-        Returns:
-        frac: fraction of catastrophic outliers for full sample
+        Returns
+        -------
+        ``frac`` float. Fraction of catastrophic outliers for full sample
         """
         num = len(self.ez)
         sig_iqr = PointSigmaIQR(self.pzs, self.szs).evaluate()
         threesig = 3.0 * sig_iqr
         cutcriterion = np.maximum(0.06, threesig)
-        mask = (np.fabs(self.ez) > cutcriterion)
+        mask = np.fabs(self.ez) > cutcriterion
         outlier = np.sum(mask)
         frac = float(outlier) / float(num)
         return frac
 
 
 class PointSigmaMAD(PointStatsEz):
     """Function to calculate median absolute deviation and sigma
     based on MAD (just scaled up by 1.4826) for the full and
     magnitude trimmed samples of ez values
     """
 
     def evaluate(self):
         """
-        Returns:
-        sigma_mad: sigma_MAD for full sample
+        Returns
+        -------
+        ``sigma_mad`` float. Sigma median absolute deviation for full sample.
         """
         tmpmed = np.median(self.ez)
         tmpx = np.fabs(self.ez - tmpmed)
         mad = np.median(tmpx)
         sigma_mad = mad * 1.4826
         return sigma_mad
```

### Comparing `pz-rail-base-0.1.9/src/rail/examples_data/creation_data/data/success_rate_data/DEEP2_success.txt` & `pz-rail-base-0.2.0/src/rail/examples_data/creation_data/data/success_rate_data/DEEP2_success.txt`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.1.9/src/rail/examples_data/creation_data/data/success_rate_data/VVDSf02_z_bright_success.txt` & `pz-rail-base-0.2.0/src/rail/examples_data/creation_data/data/success_rate_data/VVDSf02_z_bright_success.txt`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.1.9/src/rail/examples_data/creation_data/data/success_rate_data/VVDSf02_z_deep_success.txt` & `pz-rail-base-0.2.0/src/rail/examples_data/creation_data/data/success_rate_data/VVDSf02_z_deep_success.txt`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.1.9/src/rail/examples_data/creation_data/data/success_rate_data/hsc_success.txt` & `pz-rail-base-0.2.0/src/rail/examples_data/creation_data/data/success_rate_data/hsc_success.txt`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.1.9/src/rail/examples_data/creation_data/data/success_rate_data/zCOSMOS_success.txt` & `pz-rail-base-0.2.0/src/rail/examples_data/creation_data/data/success_rate_data/zCOSMOS_success.txt`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.1.9/src/rail/examples_data/estimation_data/data/FILTER/DC2LSST_g.res` & `pz-rail-base-0.2.0/src/rail/examples_data/estimation_data/data/FILTER/DC2LSST_g.res`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.1.9/src/rail/examples_data/estimation_data/data/FILTER/DC2LSST_i.res` & `pz-rail-base-0.2.0/src/rail/examples_data/estimation_data/data/FILTER/DC2LSST_i.res`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.1.9/src/rail/examples_data/estimation_data/data/FILTER/DC2LSST_r.res` & `pz-rail-base-0.2.0/src/rail/examples_data/estimation_data/data/FILTER/DC2LSST_r.res`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.1.9/src/rail/examples_data/estimation_data/data/FILTER/DC2LSST_u.res` & `pz-rail-base-0.2.0/src/rail/examples_data/estimation_data/data/FILTER/DC2LSST_u.res`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.1.9/src/rail/examples_data/estimation_data/data/FILTER/DC2LSST_y.res` & `pz-rail-base-0.2.0/src/rail/examples_data/estimation_data/data/FILTER/DC2LSST_y.res`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.1.9/src/rail/examples_data/estimation_data/data/FILTER/DC2LSST_z.res` & `pz-rail-base-0.2.0/src/rail/examples_data/estimation_data/data/FILTER/DC2LSST_z.res`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.1.9/src/rail/examples_data/estimation_data/data/SED/El_B2004a.sed` & `pz-rail-base-0.2.0/src/rail/examples_data/estimation_data/data/SED/El_B2004a.sed`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.1.9/src/rail/examples_data/estimation_data/data/SED/Im_B2004a.sed` & `pz-rail-base-0.2.0/src/rail/examples_data/estimation_data/data/SED/Im_B2004a.sed`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.1.9/src/rail/examples_data/estimation_data/data/SED/SB2_B2004a.sed` & `pz-rail-base-0.2.0/src/rail/examples_data/estimation_data/data/SED/SB2_B2004a.sed`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.1.9/src/rail/examples_data/estimation_data/data/SED/SB3_B2004a.sed` & `pz-rail-base-0.2.0/src/rail/examples_data/estimation_data/data/SED/SB3_B2004a.sed`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.1.9/src/rail/examples_data/estimation_data/data/SED/Sbc_B2004a.sed` & `pz-rail-base-0.2.0/src/rail/examples_data/estimation_data/data/SED/Sbc_B2004a.sed`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.1.9/src/rail/examples_data/estimation_data/data/SED/Scd_B2004a.sed` & `pz-rail-base-0.2.0/src/rail/examples_data/estimation_data/data/SED/Scd_B2004a.sed`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.1.9/src/rail/examples_data/estimation_data/data/SED/ssp_25Myr_z008.sed` & `pz-rail-base-0.2.0/src/rail/examples_data/estimation_data/data/SED/ssp_25Myr_z008.sed`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.1.9/src/rail/examples_data/estimation_data/data/SED/ssp_5Myr_z008.sed` & `pz-rail-base-0.2.0/src/rail/examples_data/estimation_data/data/SED/ssp_5Myr_z008.sed`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.1.9/src/rail/examples_data/goldenspike_data/configs/goldenspike_config.yml` & `pz-rail-base-0.2.0/src/rail/examples_data/goldenspike_data/configs/goldenspike_config.yml`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.1.9/src/rail/examples_data/goldenspike_data/data/pretrained_flow.pkl` & `pz-rail-base-0.2.0/src/rail/examples_data/goldenspike_data/data/pretrained_flow.pkl`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.1.9/src/rail/examples_data/goldenspike_data/data/test_flow_data.pq` & `pz-rail-base-0.2.0/src/rail/examples_data/goldenspike_data/data/test_flow_data.pq`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.1.9/src/rail/examples_data/goldenspike_data/goldenspike.yml` & `pz-rail-base-0.2.0/src/rail/examples_data/goldenspike_data/goldenspike.yml`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.1.9/src/rail/examples_data/testdata/README.md` & `pz-rail-base-0.2.0/src/rail/examples_data/testdata/README.md`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.1.9/src/rail/examples_data/testdata/lsst_filters.npy` & `pz-rail-base-0.2.0/src/rail/examples_data/testdata/lsst_filters.npy`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.1.9/src/rail/examples_data/testdata/make_rail_sample_data.ipynb` & `pz-rail-base-0.2.0/src/rail/examples_data/testdata/make_rail_sample_data.ipynb`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.1.9/src/rail/examples_data/testdata/output_BPZ_lite.fits` & `pz-rail-base-0.2.0/src/rail/examples_data/testdata/output_BPZ_lite.fits`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.1.9/src/rail/examples_data/testdata/output_BPZ_lite.hdf5` & `pz-rail-base-0.2.0/src/rail/examples_data/testdata/output_BPZ_lite.hdf5`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.1.9/src/rail/examples_data/testdata/rubin_dm_dc2_example.pq` & `pz-rail-base-0.2.0/src/rail/examples_data/testdata/rubin_dm_dc2_example.pq`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.1.9/src/rail/examples_data/testdata/test_dc2_training_9816.hdf5` & `pz-rail-base-0.2.0/src/rail/examples_data/testdata/test_dc2_training_9816.hdf5`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.1.9/src/rail/examples_data/testdata/test_dc2_training_9816.pq` & `pz-rail-base-0.2.0/src/rail/examples_data/testdata/test_dc2_training_9816.pq`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.1.9/src/rail/examples_data/testdata/test_dc2_training_9816_hyperbolic.pq` & `pz-rail-base-0.2.0/src/rail/examples_data/testdata/test_dc2_training_9816_hyperbolic.pq`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.1.9/src/rail/examples_data/testdata/test_dc2_training_9816_smoothing_params.pq` & `pz-rail-base-0.2.0/src/rail/examples_data/testdata/test_dc2_training_9816_smoothing_params.pq`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.1.9/src/rail/examples_data/testdata/test_dc2_validation_9816.hdf5` & `pz-rail-base-0.2.0/src/rail/examples_data/testdata/test_dc2_validation_9816.hdf5`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.1.9/src/rail/examples_data/testdata/training_100gal.hdf5` & `pz-rail-base-0.2.0/src/rail/examples_data/testdata/training_100gal.hdf5`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.1.9/src/rail/examples_data/testdata/validation_10gal.hdf5` & `pz-rail-base-0.2.0/src/rail/examples_data/testdata/validation_10gal.hdf5`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.1.9/src/rail/stages/__init__.py` & `pz-rail-base-0.2.0/src/rail/stages/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 from rail.estimation.algos.var_inf import *
 from rail.estimation.algos.uniform_binning import *
 from rail.estimation.algos.equal_count import *
 
 
 from rail.creation.degrader import *
 #from rail.creation.degradation.spectroscopic_degraders import *
-from rail.creation.degradation.spectroscopic_selections import *
+# from rail.creation.degradation.spectroscopic_selections import *
 from rail.creation.degradation.quantityCut import *
 
 from rail.creation.engine import *
 #from rail.creation.engines.flowEngine import *
 #from rail.creation.engines.galaxy_population_components import *
 #from rail.creation.engines.dsps_photometry_creator import *
 #from rail.creation.engines.dsps_sed_modeler import *
```

### Comparing `pz-rail-base-0.1.9/tests/cli/hello_world.ipynb` & `pz-rail-base-0.2.0/tests/cli/hello_world.ipynb`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.1.9/tests/cli/single_number.ipynb` & `pz-rail-base-0.2.0/tests/cli/single_number.ipynb`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.1.9/tests/cli/test_scripts.py` & `pz-rail-base-0.2.0/tests/cli/test_scripts.py`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.1.9/tests/core/test_core.py` & `pz-rail-base-0.2.0/tests/core/test_core.py`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.1.9/tests/core/test_introspection.py` & `pz-rail-base-0.2.0/tests/core/test_introspection.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import tempfile
 import pkgutil
 import setuptools
 
 import rail
 from rail.core import RailEnv
+from rail.core.data import DataHandle, TableHandle
 import rail.stages
 
 
 def test_print_rail_packages():
     RailEnv.print_rail_packages()
 
     
@@ -27,7 +28,12 @@
     rail.stages.import_and_attach_all()
     RailEnv.print_rail_stage_dict()
 
 
 def test_api_rst():
     with tempfile.TemporaryDirectory() as tmpdirname:
         RailEnv.do_api_rst(tmpdirname)
+
+
+def test_data_handle_dict():
+    DataHandle.print_sub_classes()
+    assert DataHandle.get_sub_class('TableHandle') == TableHandle
```

### Comparing `pz-rail-base-0.1.9/tests/core/test_pipeline.py` & `pz-rail-base-0.2.0/tests/core/test_pipeline.py`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.1.9/tests/core/test_point_estimation.py` & `pz-rail-base-0.2.0/tests/core/test_point_estimation.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+# pylint: disable=no-member
 import pytest
 import numpy as np
 
 import qp
 from rail.estimation.estimator import CatEstimator
 
 
@@ -77,7 +78,44 @@
     locs = 2* (np.random.uniform(size=(100,1))-0.5)
     scales = 1 + 0.2*(np.random.uniform(size=(100,1))-0.5)
     test_ensemble = qp.Ensemble(qp.stats.norm, data=dict(loc=locs, scale=scales))
 
     output_ensemble = test_estimator.calculate_point_estimates(test_ensemble, None)
 
     assert output_ensemble.ancil is None
+
+def test_keep_existing_ancil_data():
+    """Make sure that we don't overwrite the ancil data if it already exists.
+    """
+    config_dict = {'zmin':0.0, 'zmax': 3.0, 'nzbins':100, 'calculated_point_estimates': ['mode']}
+
+    test_estimator = CatEstimator.make_stage(name='test', **config_dict)
+
+    locs = 2* (np.random.uniform(size=(100,1))-0.5)
+    scales = 1 + 0.2*(np.random.uniform(size=(100,1))-0.5)
+    test_ensemble = qp.Ensemble(qp.stats.norm, data=dict(loc=locs, scale=scales))
+
+    test_ensemble.set_ancil({'foo': np.zeros(100)})
+
+    output_ensemble = test_estimator.calculate_point_estimates(test_ensemble, None)
+
+    assert 'foo' in output_ensemble.ancil
+    assert np.all(output_ensemble.ancil['foo'] == 0.0)
+    assert len(output_ensemble.ancil['foo']) == 100
+
+def test_write_new_ancil_data():
+    """Make sure that we don't overwrite the ancil data if it already exists.
+    """
+    config_dict = {'zmin':0.0, 'zmax': 3.0, 'nzbins':100, 'calculated_point_estimates': ['mode']}
+
+    test_estimator = CatEstimator.make_stage(name='test', **config_dict)
+
+    locs = 2* (np.random.uniform(size=(100,1))-0.5)
+    scales = 1 + 0.2*(np.random.uniform(size=(100,1))-0.5)
+    test_ensemble = qp.Ensemble(qp.stats.norm, data=dict(loc=locs, scale=scales))
+
+    test_ensemble.set_ancil({'foo': np.zeros(100)})
+
+    output_ensemble = test_estimator.calculate_point_estimates(test_ensemble, None)
+
+    assert 'mode' in output_ensemble.ancil
+    assert len(output_ensemble.ancil['mode']) == 100
```

### Comparing `pz-rail-base-0.1.9/tests/estimation/test_algos.py` & `pz-rail-base-0.2.0/tests/estimation/test_algos.py`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.1.9/tests/estimation/test_classifier.py` & `pz-rail-base-0.2.0/tests/estimation/test_classifier.py`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.1.9/tests/estimation/test_summarizers.py` & `pz-rail-base-0.2.0/tests/estimation/test_summarizers.py`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.1.9/tests/evaluation/test_evaluation.py` & `pz-rail-base-0.2.0/tests/evaluation/test_evaluation.py`

 * *Files identical despite different names*

