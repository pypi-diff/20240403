# Comparing `tmp/pz-rail-base-0.2.0.tar.gz` & `tmp/pz-rail-base-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pz-rail-base-0.2.0.tar", last modified: Wed Apr  3 16:51:38 2024, max compression
+gzip compressed data, was "pz-rail-base-0.2.1.tar", last modified: Wed Apr  3 18:11:15 2024, max compression
```

## Comparing `pz-rail-base-0.2.0.tar` & `pz-rail-base-0.2.1.tar`

### file list

```diff
@@ -1,152 +1,152 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 16:51:38.547436 pz-rail-base-0.2.0/
--rw-r--r--   0 runner    (1001) docker     (127)      268 2024-04-03 16:51:31.000000 pz-rail-base-0.2.0/.copier-answers.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 16:51:38.515436 pz-rail-base-0.2.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 16:51:38.515436 pz-rail-base-0.2.0/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (127)      101 2024-04-03 16:51:31.000000 pz-rail-base-0.2.0/.github/ISSUE_TEMPLATE/0-general_issue.md
--rw-r--r--   0 runner    (1001) docker     (127)      661 2024-04-03 16:51:31.000000 pz-rail-base-0.2.0/.github/ISSUE_TEMPLATE/1-bug_report.md
--rw-r--r--   0 runner    (1001) docker     (127)      707 2024-04-03 16:51:31.000000 pz-rail-base-0.2.0/.github/ISSUE_TEMPLATE/2-feature_request.md
--rw-r--r--   0 runner    (1001) docker     (127)      783 2024-04-03 16:51:31.000000 pz-rail-base-0.2.0/.github/pull_request_template.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 16:51:38.519436 pz-rail-base-0.2.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      488 2024-04-03 16:51:31.000000 pz-rail-base-0.2.0/.github/workflows/add-issue-to-project-tracker.yml
--rw-r--r--   0 runner    (1001) docker     (127)      977 2024-04-03 16:51:31.000000 pz-rail-base-0.2.0/.github/workflows/linting.yml
--rw-r--r--   0 runner    (1001) docker     (127)      950 2024-04-03 16:51:31.000000 pz-rail-base-0.2.0/.github/workflows/publish-to-pypi.yml
--rw-r--r--   0 runner    (1001) docker     (127)      931 2024-04-03 16:51:31.000000 pz-rail-base-0.2.0/.github/workflows/smoke-test.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1111 2024-04-03 16:51:31.000000 pz-rail-base-0.2.0/.github/workflows/testing-and-coverage.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1912 2024-04-03 16:51:31.000000 pz-rail-base-0.2.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     2623 2024-04-03 16:51:31.000000 pz-rail-base-0.2.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1102 2024-04-03 16:51:31.000000 pz-rail-base-0.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     5736 2024-04-03 16:51:38.547436 pz-rail-base-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3516 2024-04-03 16:51:31.000000 pz-rail-base-0.2.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      163 2024-04-03 16:51:31.000000 pz-rail-base-0.2.0/environment.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1886 2024-04-03 16:51:31.000000 pz-rail-base-0.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-03 16:51:31.000000 pz-rail-base-0.2.0/rail_packages.yml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-03 16:51:38.547436 pz-rail-base-0.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       70 2024-04-03 16:51:31.000000 pz-rail-base-0.2.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 16:51:38.511436 pz-rail-base-0.2.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 16:51:38.543436 pz-rail-base-0.2.0/src/pz_rail_base.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5736 2024-04-03 16:51:38.000000 pz-rail-base-0.2.0/src/pz_rail_base.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5027 2024-04-03 16:51:38.000000 pz-rail-base-0.2.0/src/pz_rail_base.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 16:51:38.000000 pz-rail-base-0.2.0/src/pz_rail_base.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-03 16:51:38.000000 pz-rail-base-0.2.0/src/pz_rail_base.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      136 2024-04-03 16:51:38.000000 pz-rail-base-0.2.0/src/pz_rail_base.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-03 16:51:38.000000 pz-rail-base-0.2.0/src/pz_rail_base.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 16:51:38.515436 pz-rail-base-0.2.0/src/rail/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 16:51:38.519436 pz-rail-base-0.2.0/src/rail/cli/
--rw-r--r--   0 runner    (1001) docker     (127)     1910 2024-04-03 16:51:31.000000 pz-rail-base-0.2.0/src/rail/cli/commands.py
--rw-r--r--   0 runner    (1001) docker     (127)     3610 2024-04-03 16:51:31.000000 pz-rail-base-0.2.0/src/rail/cli/options.py
--rw-r--r--   0 runner    (1001) docker     (127)     6219 2024-04-03 16:51:31.000000 pz-rail-base-0.2.0/src/rail/cli/scripts.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 16:51:38.519436 pz-rail-base-0.2.0/src/rail/core/
--rw-r--r--   0 runner    (1001) docker     (127)      659 2024-04-03 16:51:31.000000 pz-rail-base-0.2.0/src/rail/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-03 16:51:38.000000 pz-rail-base-0.2.0/src/rail/core/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     2890 2024-04-03 16:51:31.000000 pz-rail-base-0.2.0/src/rail/core/algo_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2283 2024-04-03 16:51:31.000000 pz-rail-base-0.2.0/src/rail/core/common_params.py
--rw-r--r--   0 runner    (1001) docker     (127)    17759 2024-04-03 16:51:31.000000 pz-rail-base-0.2.0/src/rail/core/data.py
--rw-r--r--   0 runner    (1001) docker     (127)    10923 2024-04-03 16:51:31.000000 pz-rail-base-0.2.0/src/rail/core/introspection.py
--rw-r--r--   0 runner    (1001) docker     (127)     4632 2024-04-03 16:51:31.000000 pz-rail-base-0.2.0/src/rail/core/point_estimation.py
--rw-r--r--   0 runner    (1001) docker     (127)    14432 2024-04-03 16:51:31.000000 pz-rail-base-0.2.0/src/rail/core/stage.py
--rw-r--r--   0 runner    (1001) docker     (127)     4301 2024-04-03 16:51:31.000000 pz-rail-base-0.2.0/src/rail/core/util_stages.py
--rw-r--r--   0 runner    (1001) docker     (127)      622 2024-04-03 16:51:31.000000 pz-rail-base-0.2.0/src/rail/core/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 16:51:38.523436 pz-rail-base-0.2.0/src/rail/creation/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 16:51:38.523436 pz-rail-base-0.2.0/src/rail/creation/degradation/
--rw-r--r--   0 runner    (1001) docker     (127)     4287 2024-04-03 16:51:31.000000 pz-rail-base-0.2.0/src/rail/creation/degradation/quantityCut.py
--rw-r--r--   0 runner    (1001) docker     (127)     2039 2024-04-03 16:51:31.000000 pz-rail-base-0.2.0/src/rail/creation/degrader.py
--rw-r--r--   0 runner    (1001) docker     (127)     7071 2024-04-03 16:51:31.000000 pz-rail-base-0.2.0/src/rail/creation/engine.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 16:51:38.523436 pz-rail-base-0.2.0/src/rail/estimation/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 16:51:38.523436 pz-rail-base-0.2.0/src/rail/estimation/algos/
--rw-r--r--   0 runner    (1001) docker     (127)     2433 2024-04-03 16:51:31.000000 pz-rail-base-0.2.0/src/rail/estimation/algos/equal_count.py
--rw-r--r--   0 runner    (1001) docker     (127)     3251 2024-04-03 16:51:31.000000 pz-rail-base-0.2.0/src/rail/estimation/algos/naive_stack.py
--rw-r--r--   0 runner    (1001) docker     (127)     3548 2024-04-03 16:51:31.000000 pz-rail-base-0.2.0/src/rail/estimation/algos/point_est_hist.py
--rw-r--r--   0 runner    (1001) docker     (127)     2635 2024-04-03 16:51:31.000000 pz-rail-base-0.2.0/src/rail/estimation/algos/random_gauss.py
--rw-r--r--   0 runner    (1001) docker     (127)     3168 2024-04-03 16:51:31.000000 pz-rail-base-0.2.0/src/rail/estimation/algos/train_z.py
--rw-r--r--   0 runner    (1001) docker     (127)     3936 2024-04-03 16:51:31.000000 pz-rail-base-0.2.0/src/rail/estimation/algos/uniform_binning.py
--rw-r--r--   0 runner    (1001) docker     (127)     4838 2024-04-03 16:51:31.000000 pz-rail-base-0.2.0/src/rail/estimation/algos/var_inf.py
--rw-r--r--   0 runner    (1001) docker     (127)     8041 2024-04-03 16:51:31.000000 pz-rail-base-0.2.0/src/rail/estimation/classifier.py
--rw-r--r--   0 runner    (1001) docker     (127)     4838 2024-04-03 16:51:31.000000 pz-rail-base-0.2.0/src/rail/estimation/estimator.py
--rw-r--r--   0 runner    (1001) docker     (127)     4572 2024-04-03 16:51:31.000000 pz-rail-base-0.2.0/src/rail/estimation/informer.py
--rw-r--r--   0 runner    (1001) docker     (127)     7638 2024-04-03 16:51:31.000000 pz-rail-base-0.2.0/src/rail/estimation/summarizer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 16:51:38.523436 pz-rail-base-0.2.0/src/rail/evaluation/
--rw-r--r--   0 runner    (1001) docker     (127)     5891 2024-04-03 16:51:31.000000 pz-rail-base-0.2.0/src/rail/evaluation/evaluator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 16:51:38.523436 pz-rail-base-0.2.0/src/rail/evaluation/metrics/
--rw-r--r--   0 runner    (1001) docker     (127)      565 2024-04-03 16:51:31.000000 pz-rail-base-0.2.0/src/rail/evaluation/metrics/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     1017 2024-04-03 16:51:31.000000 pz-rail-base-0.2.0/src/rail/evaluation/metrics/cdeloss.py
--rw-r--r--   0 runner    (1001) docker     (127)     2967 2024-04-03 16:51:31.000000 pz-rail-base-0.2.0/src/rail/evaluation/metrics/pointestimates.py
--rw-r--r--   0 runner    (1001) docker     (127)      338 2024-04-03 16:51:31.000000 pz-rail-base-0.2.0/src/rail/evaluation/stats_groups.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 16:51:38.523436 pz-rail-base-0.2.0/src/rail/examples_data/
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-03 16:51:31.000000 pz-rail-base-0.2.0/src/rail/examples_data/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 16:51:38.511436 pz-rail-base-0.2.0/src/rail/examples_data/creation_data/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 16:51:38.523436 pz-rail-base-0.2.0/src/rail/examples_data/creation_data/configs/
--rw-r--r--   0 runner    (1001) docker     (127)      418 2024-04-03 16:51:31.000000 pz-rail-base-0.2.0/src/rail/examples_data/creation_data/configs/flowModeler.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 16:51:38.523436 pz-rail-base-0.2.0/src/rail/examples_data/creation_data/data/
--rw-r--r--   0 runner    (1001) docker     (127)      141 2024-04-03 16:51:31.000000 pz-rail-base-0.2.0/src/rail/examples_data/creation_data/data/HSC_grid_settings.pkl
--rw-r--r--   0 runner    (1001) docker     (127)      313 2024-04-03 16:51:31.000000 pz-rail-base-0.2.0/src/rail/examples_data/creation_data/data/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 16:51:38.527436 pz-rail-base-0.2.0/src/rail/examples_data/creation_data/data/success_rate_data/
--rw-r--r--   0 runner    (1001) docker     (127)      727 2024-04-03 16:51:31.000000 pz-rail-base-0.2.0/src/rail/examples_data/creation_data/data/success_rate_data/DEEP2_success.txt
--rw-r--r--   0 runner    (1001) docker     (127)      428 2024-04-03 16:51:31.000000 pz-rail-base-0.2.0/src/rail/examples_data/creation_data/data/success_rate_data/VVDSf02_I_success.txt
--rw-r--r--   0 runner    (1001) docker     (127)      973 2024-04-03 16:51:31.000000 pz-rail-base-0.2.0/src/rail/examples_data/creation_data/data/success_rate_data/VVDSf02_z_bright_success.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1873 2024-04-03 16:51:31.000000 pz-rail-base-0.2.0/src/rail/examples_data/creation_data/data/success_rate_data/VVDSf02_z_deep_success.txt
--rw-r--r--   0 runner    (1001) docker     (127)  1000000 2024-04-03 16:51:31.000000 pz-rail-base-0.2.0/src/rail/examples_data/creation_data/data/success_rate_data/hsc_success.txt
--rw-r--r--   0 runner    (1001) docker     (127)   431705 2024-04-03 16:51:31.000000 pz-rail-base-0.2.0/src/rail/examples_data/creation_data/data/success_rate_data/zCOSMOS_success.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 16:51:38.511436 pz-rail-base-0.2.0/src/rail/examples_data/estimation_data/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 16:51:38.527436 pz-rail-base-0.2.0/src/rail/examples_data/estimation_data/data/
--rw-r--r--   0 runner    (1001) docker     (127)      219 2024-04-03 16:51:31.000000 pz-rail-base-0.2.0/src/rail/examples_data/estimation_data/data/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 16:51:38.527436 pz-rail-base-0.2.0/src/rail/examples_data/estimation_data/data/AB/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 16:51:31.000000 pz-rail-base-0.2.0/src/rail/examples_data/estimation_data/data/AB/dummy.txt
--rw-r--r--   0 runner    (1001) docker     (127)      454 2024-04-03 16:51:31.000000 pz-rail-base-0.2.0/src/rail/examples_data/estimation_data/data/CWW_HDFN_prior.pkl
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 16:51:38.531436 pz-rail-base-0.2.0/src/rail/examples_data/estimation_data/data/FILTER/
--rw-r--r--   0 runner    (1001) docker     (127)    98003 2024-04-03 16:51:31.000000 pz-rail-base-0.2.0/src/rail/examples_data/estimation_data/data/FILTER/DC2LSST_g.res
--rw-r--r--   0 runner    (1001) docker     (127)    95326 2024-04-03 16:51:31.000000 pz-rail-base-0.2.0/src/rail/examples_data/estimation_data/data/FILTER/DC2LSST_i.res
--rw-r--r--   0 runner    (1001) docker     (127)    96635 2024-04-03 16:51:31.000000 pz-rail-base-0.2.0/src/rail/examples_data/estimation_data/data/FILTER/DC2LSST_r.res
--rw-r--r--   0 runner    (1001) docker     (127)    90216 2024-04-03 16:51:31.000000 pz-rail-base-0.2.0/src/rail/examples_data/estimation_data/data/FILTER/DC2LSST_u.res
--rw-r--r--   0 runner    (1001) docker     (127)   100126 2024-04-03 16:51:31.000000 pz-rail-base-0.2.0/src/rail/examples_data/estimation_data/data/FILTER/DC2LSST_y.res
--rw-r--r--   0 runner    (1001) docker     (127)    93013 2024-04-03 16:51:31.000000 pz-rail-base-0.2.0/src/rail/examples_data/estimation_data/data/FILTER/DC2LSST_z.res
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 16:51:38.531436 pz-rail-base-0.2.0/src/rail/examples_data/estimation_data/data/SED/
--rwxr-xr-x   0 runner    (1001) docker     (127)      125 2024-04-03 16:51:31.000000 pz-rail-base-0.2.0/src/rail/examples_data/estimation_data/data/SED/CWWSB4.list
--rwxr-xr-x   0 runner    (1001) docker     (127)    43750 2024-04-03 16:51:31.000000 pz-rail-base-0.2.0/src/rail/examples_data/estimation_data/data/SED/El_B2004a.sed
--rwxr-xr-x   0 runner    (1001) docker     (127)    42830 2024-04-03 16:51:31.000000 pz-rail-base-0.2.0/src/rail/examples_data/estimation_data/data/SED/Im_B2004a.sed
--rwxr-xr-x   0 runner    (1001) docker     (127)    72228 2024-04-03 16:51:31.000000 pz-rail-base-0.2.0/src/rail/examples_data/estimation_data/data/SED/SB2_B2004a.sed
--rwxr-xr-x   0 runner    (1001) docker     (127)    68560 2024-04-03 16:51:31.000000 pz-rail-base-0.2.0/src/rail/examples_data/estimation_data/data/SED/SB3_B2004a.sed
--rwxr-xr-x   0 runner    (1001) docker     (127)    43351 2024-04-03 16:51:31.000000 pz-rail-base-0.2.0/src/rail/examples_data/estimation_data/data/SED/Sbc_B2004a.sed
--rwxr-xr-x   0 runner    (1001) docker     (127)    42789 2024-04-03 16:51:31.000000 pz-rail-base-0.2.0/src/rail/examples_data/estimation_data/data/SED/Scd_B2004a.sed
--rwxr-xr-x   0 runner    (1001) docker     (127)   179585 2024-04-03 16:51:31.000000 pz-rail-base-0.2.0/src/rail/examples_data/estimation_data/data/SED/ssp_25Myr_z008.sed
--rwxr-xr-x   0 runner    (1001) docker     (127)   179584 2024-04-03 16:51:31.000000 pz-rail-base-0.2.0/src/rail/examples_data/estimation_data/data/SED/ssp_5Myr_z008.sed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 16:51:38.531436 pz-rail-base-0.2.0/src/rail/examples_data/goldenspike_data/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 16:51:38.531436 pz-rail-base-0.2.0/src/rail/examples_data/goldenspike_data/configs/
--rw-r--r--   0 runner    (1001) docker     (127)     6052 2024-04-03 16:51:31.000000 pz-rail-base-0.2.0/src/rail/examples_data/goldenspike_data/configs/goldenspike_config.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 16:51:38.535436 pz-rail-base-0.2.0/src/rail/examples_data/goldenspike_data/data/
--rw-r--r--   0 runner    (1001) docker     (127)  1158108 2024-04-03 16:51:31.000000 pz-rail-base-0.2.0/src/rail/examples_data/goldenspike_data/data/pretrained_flow.pkl
--rw-r--r--   0 runner    (1001) docker     (127)   873947 2024-04-03 16:51:31.000000 pz-rail-base-0.2.0/src/rail/examples_data/goldenspike_data/data/test_flow_data.pq
--rw-r--r--   0 runner    (1001) docker     (127)     1419 2024-04-03 16:51:31.000000 pz-rail-base-0.2.0/src/rail/examples_data/goldenspike_data/goldenspike.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 16:51:38.543436 pz-rail-base-0.2.0/src/rail/examples_data/testdata/
--rw-r--r--   0 runner    (1001) docker     (127)      553 2024-04-03 16:51:31.000000 pz-rail-base-0.2.0/src/rail/examples_data/testdata/README.md
--rw-r--r--   0 runner    (1001) docker     (127)    91936 2024-04-03 16:51:31.000000 pz-rail-base-0.2.0/src/rail/examples_data/testdata/lsst_filters.npy
--rw-r--r--   0 runner    (1001) docker     (127)     4742 2024-04-03 16:51:31.000000 pz-rail-base-0.2.0/src/rail/examples_data/testdata/make_rail_sample_data.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    43200 2024-04-03 16:51:31.000000 pz-rail-base-0.2.0/src/rail/examples_data/testdata/output_BPZ_lite.fits
--rw-r--r--   0 runner    (1001) docker     (127)    37192 2024-04-03 16:51:31.000000 pz-rail-base-0.2.0/src/rail/examples_data/testdata/output_BPZ_lite.hdf5
--rw-r--r--   0 runner    (1001) docker     (127)    24574 2024-04-03 16:51:31.000000 pz-rail-base-0.2.0/src/rail/examples_data/testdata/rubin_dm_dc2_example.pq
--rw-r--r--   0 runner    (1001) docker     (127)   662976 2024-04-03 16:51:31.000000 pz-rail-base-0.2.0/src/rail/examples_data/testdata/test_dc2_training_9816.hdf5
--rw-r--r--   0 runner    (1001) docker     (127)   873930 2024-04-03 16:51:31.000000 pz-rail-base-0.2.0/src/rail/examples_data/testdata/test_dc2_training_9816.pq
--rw-r--r--   0 runner    (1001) docker     (127)  1192254 2024-04-03 16:51:31.000000 pz-rail-base-0.2.0/src/rail/examples_data/testdata/test_dc2_training_9816_hyperbolic.pq
--rw-r--r--   0 runner    (1001) docker     (127)     5625 2024-04-03 16:51:31.000000 pz-rail-base-0.2.0/src/rail/examples_data/testdata/test_dc2_training_9816_smoothing_params.pq
--rw-r--r--   0 runner    (1001) docker     (127)  1316984 2024-04-03 16:51:31.000000 pz-rail-base-0.2.0/src/rail/examples_data/testdata/test_dc2_validation_9816.hdf5
--rw-r--r--   0 runner    (1001) docker     (127)    15192 2024-04-03 16:51:31.000000 pz-rail-base-0.2.0/src/rail/examples_data/testdata/training_100gal.hdf5
--rw-r--r--   0 runner    (1001) docker     (127)     9200 2024-04-03 16:51:31.000000 pz-rail-base-0.2.0/src/rail/examples_data/testdata/validation_10gal.hdf5
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 16:51:38.543436 pz-rail-base-0.2.0/src/rail/stages/
--rw-r--r--   0 runner    (1001) docker     (127)     1230 2024-04-03 16:51:31.000000 pz-rail-base-0.2.0/src/rail/stages/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 16:51:38.515436 pz-rail-base-0.2.0/tests/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 16:51:38.543436 pz-rail-base-0.2.0/tests/cli/
--rw-r--r--   0 runner    (1001) docker     (127)      833 2024-04-03 16:51:31.000000 pz-rail-base-0.2.0/tests/cli/hello_world.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     1095 2024-04-03 16:51:31.000000 pz-rail-base-0.2.0/tests/cli/single_number.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)      974 2024-04-03 16:51:31.000000 pz-rail-base-0.2.0/tests/cli/test_scripts.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 16:51:38.543436 pz-rail-base-0.2.0/tests/core/
--rw-r--r--   0 runner    (1001) docker     (127)    10079 2024-04-03 16:51:31.000000 pz-rail-base-0.2.0/tests/core/test_core.py
--rw-r--r--   0 runner    (1001) docker     (127)      811 2024-04-03 16:51:31.000000 pz-rail-base-0.2.0/tests/core/test_introspection.py
--rw-r--r--   0 runner    (1001) docker     (127)     2780 2024-04-03 16:51:31.000000 pz-rail-base-0.2.0/tests/core/test_pipeline.py
--rw-r--r--   0 runner    (1001) docker     (127)     4521 2024-04-03 16:51:31.000000 pz-rail-base-0.2.0/tests/core/test_point_estimation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 16:51:38.543436 pz-rail-base-0.2.0/tests/creation/
--rw-r--r--   0 runner    (1001) docker     (127)     2369 2024-04-03 16:51:31.000000 pz-rail-base-0.2.0/tests/creation/test_degraders.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 16:51:38.543436 pz-rail-base-0.2.0/tests/estimation/
--rw-r--r--   0 runner    (1001) docker     (127)     1656 2024-04-03 16:51:31.000000 pz-rail-base-0.2.0/tests/estimation/test_algos.py
--rw-r--r--   0 runner    (1001) docker     (127)     4337 2024-04-03 16:51:31.000000 pz-rail-base-0.2.0/tests/estimation/test_classifier.py
--rw-r--r--   0 runner    (1001) docker     (127)     2083 2024-04-03 16:51:31.000000 pz-rail-base-0.2.0/tests/estimation/test_summarizers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 16:51:38.543436 pz-rail-base-0.2.0/tests/evaluation/
--rw-r--r--   0 runner    (1001) docker     (127)     2137 2024-04-03 16:51:31.000000 pz-rail-base-0.2.0/tests/evaluation/test_evaluation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 18:11:15.574290 pz-rail-base-0.2.1/
+-rw-r--r--   0 runner    (1001) docker     (127)      268 2024-04-03 18:11:08.000000 pz-rail-base-0.2.1/.copier-answers.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 18:11:15.546290 pz-rail-base-0.2.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 18:11:15.546290 pz-rail-base-0.2.1/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-04-03 18:11:08.000000 pz-rail-base-0.2.1/.github/ISSUE_TEMPLATE/0-general_issue.md
+-rw-r--r--   0 runner    (1001) docker     (127)      661 2024-04-03 18:11:08.000000 pz-rail-base-0.2.1/.github/ISSUE_TEMPLATE/1-bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (127)      707 2024-04-03 18:11:08.000000 pz-rail-base-0.2.1/.github/ISSUE_TEMPLATE/2-feature_request.md
+-rw-r--r--   0 runner    (1001) docker     (127)      783 2024-04-03 18:11:08.000000 pz-rail-base-0.2.1/.github/pull_request_template.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 18:11:15.546290 pz-rail-base-0.2.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      488 2024-04-03 18:11:08.000000 pz-rail-base-0.2.1/.github/workflows/add-issue-to-project-tracker.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      977 2024-04-03 18:11:08.000000 pz-rail-base-0.2.1/.github/workflows/linting.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      950 2024-04-03 18:11:08.000000 pz-rail-base-0.2.1/.github/workflows/publish-to-pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      931 2024-04-03 18:11:08.000000 pz-rail-base-0.2.1/.github/workflows/smoke-test.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1111 2024-04-03 18:11:08.000000 pz-rail-base-0.2.1/.github/workflows/testing-and-coverage.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1912 2024-04-03 18:11:08.000000 pz-rail-base-0.2.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     2623 2024-04-03 18:11:08.000000 pz-rail-base-0.2.1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1102 2024-04-03 18:11:08.000000 pz-rail-base-0.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     5736 2024-04-03 18:11:15.574290 pz-rail-base-0.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3516 2024-04-03 18:11:08.000000 pz-rail-base-0.2.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      163 2024-04-03 18:11:08.000000 pz-rail-base-0.2.1/environment.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1886 2024-04-03 18:11:08.000000 pz-rail-base-0.2.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-03 18:11:08.000000 pz-rail-base-0.2.1/rail_packages.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-03 18:11:15.574290 pz-rail-base-0.2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-04-03 18:11:08.000000 pz-rail-base-0.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 18:11:15.542290 pz-rail-base-0.2.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 18:11:15.574290 pz-rail-base-0.2.1/src/pz_rail_base.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5736 2024-04-03 18:11:15.000000 pz-rail-base-0.2.1/src/pz_rail_base.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5027 2024-04-03 18:11:15.000000 pz-rail-base-0.2.1/src/pz_rail_base.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 18:11:15.000000 pz-rail-base-0.2.1/src/pz_rail_base.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-03 18:11:15.000000 pz-rail-base-0.2.1/src/pz_rail_base.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      136 2024-04-03 18:11:15.000000 pz-rail-base-0.2.1/src/pz_rail_base.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-03 18:11:15.000000 pz-rail-base-0.2.1/src/pz_rail_base.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 18:11:15.546290 pz-rail-base-0.2.1/src/rail/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 18:11:15.550290 pz-rail-base-0.2.1/src/rail/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)     1910 2024-04-03 18:11:08.000000 pz-rail-base-0.2.1/src/rail/cli/commands.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3610 2024-04-03 18:11:08.000000 pz-rail-base-0.2.1/src/rail/cli/options.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6219 2024-04-03 18:11:08.000000 pz-rail-base-0.2.1/src/rail/cli/scripts.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 18:11:15.550290 pz-rail-base-0.2.1/src/rail/core/
+-rw-r--r--   0 runner    (1001) docker     (127)      659 2024-04-03 18:11:08.000000 pz-rail-base-0.2.1/src/rail/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-03 18:11:15.000000 pz-rail-base-0.2.1/src/rail/core/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2890 2024-04-03 18:11:08.000000 pz-rail-base-0.2.1/src/rail/core/algo_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2283 2024-04-03 18:11:08.000000 pz-rail-base-0.2.1/src/rail/core/common_params.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17759 2024-04-03 18:11:08.000000 pz-rail-base-0.2.1/src/rail/core/data.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10923 2024-04-03 18:11:08.000000 pz-rail-base-0.2.1/src/rail/core/introspection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4632 2024-04-03 18:11:08.000000 pz-rail-base-0.2.1/src/rail/core/point_estimation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14518 2024-04-03 18:11:08.000000 pz-rail-base-0.2.1/src/rail/core/stage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4301 2024-04-03 18:11:08.000000 pz-rail-base-0.2.1/src/rail/core/util_stages.py
+-rw-r--r--   0 runner    (1001) docker     (127)      622 2024-04-03 18:11:08.000000 pz-rail-base-0.2.1/src/rail/core/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 18:11:15.550290 pz-rail-base-0.2.1/src/rail/creation/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 18:11:15.550290 pz-rail-base-0.2.1/src/rail/creation/degradation/
+-rw-r--r--   0 runner    (1001) docker     (127)     4287 2024-04-03 18:11:08.000000 pz-rail-base-0.2.1/src/rail/creation/degradation/quantityCut.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2039 2024-04-03 18:11:08.000000 pz-rail-base-0.2.1/src/rail/creation/degrader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7071 2024-04-03 18:11:08.000000 pz-rail-base-0.2.1/src/rail/creation/engine.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 18:11:15.550290 pz-rail-base-0.2.1/src/rail/estimation/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 18:11:15.554290 pz-rail-base-0.2.1/src/rail/estimation/algos/
+-rw-r--r--   0 runner    (1001) docker     (127)     2433 2024-04-03 18:11:08.000000 pz-rail-base-0.2.1/src/rail/estimation/algos/equal_count.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3251 2024-04-03 18:11:08.000000 pz-rail-base-0.2.1/src/rail/estimation/algos/naive_stack.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3548 2024-04-03 18:11:08.000000 pz-rail-base-0.2.1/src/rail/estimation/algos/point_est_hist.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2635 2024-04-03 18:11:08.000000 pz-rail-base-0.2.1/src/rail/estimation/algos/random_gauss.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3168 2024-04-03 18:11:08.000000 pz-rail-base-0.2.1/src/rail/estimation/algos/train_z.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3936 2024-04-03 18:11:08.000000 pz-rail-base-0.2.1/src/rail/estimation/algos/uniform_binning.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4838 2024-04-03 18:11:08.000000 pz-rail-base-0.2.1/src/rail/estimation/algos/var_inf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8041 2024-04-03 18:11:08.000000 pz-rail-base-0.2.1/src/rail/estimation/classifier.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4838 2024-04-03 18:11:08.000000 pz-rail-base-0.2.1/src/rail/estimation/estimator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4572 2024-04-03 18:11:08.000000 pz-rail-base-0.2.1/src/rail/estimation/informer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7638 2024-04-03 18:11:08.000000 pz-rail-base-0.2.1/src/rail/estimation/summarizer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 18:11:15.554290 pz-rail-base-0.2.1/src/rail/evaluation/
+-rw-r--r--   0 runner    (1001) docker     (127)     5891 2024-04-03 18:11:08.000000 pz-rail-base-0.2.1/src/rail/evaluation/evaluator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 18:11:15.554290 pz-rail-base-0.2.1/src/rail/evaluation/metrics/
+-rw-r--r--   0 runner    (1001) docker     (127)      565 2024-04-03 18:11:08.000000 pz-rail-base-0.2.1/src/rail/evaluation/metrics/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1017 2024-04-03 18:11:08.000000 pz-rail-base-0.2.1/src/rail/evaluation/metrics/cdeloss.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2967 2024-04-03 18:11:08.000000 pz-rail-base-0.2.1/src/rail/evaluation/metrics/pointestimates.py
+-rw-r--r--   0 runner    (1001) docker     (127)      338 2024-04-03 18:11:08.000000 pz-rail-base-0.2.1/src/rail/evaluation/stats_groups.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 18:11:15.554290 pz-rail-base-0.2.1/src/rail/examples_data/
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-03 18:11:08.000000 pz-rail-base-0.2.1/src/rail/examples_data/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 18:11:15.542290 pz-rail-base-0.2.1/src/rail/examples_data/creation_data/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 18:11:15.554290 pz-rail-base-0.2.1/src/rail/examples_data/creation_data/configs/
+-rw-r--r--   0 runner    (1001) docker     (127)      418 2024-04-03 18:11:08.000000 pz-rail-base-0.2.1/src/rail/examples_data/creation_data/configs/flowModeler.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 18:11:15.554290 pz-rail-base-0.2.1/src/rail/examples_data/creation_data/data/
+-rw-r--r--   0 runner    (1001) docker     (127)      141 2024-04-03 18:11:08.000000 pz-rail-base-0.2.1/src/rail/examples_data/creation_data/data/HSC_grid_settings.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)      313 2024-04-03 18:11:08.000000 pz-rail-base-0.2.1/src/rail/examples_data/creation_data/data/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 18:11:15.558290 pz-rail-base-0.2.1/src/rail/examples_data/creation_data/data/success_rate_data/
+-rw-r--r--   0 runner    (1001) docker     (127)      727 2024-04-03 18:11:08.000000 pz-rail-base-0.2.1/src/rail/examples_data/creation_data/data/success_rate_data/DEEP2_success.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      428 2024-04-03 18:11:08.000000 pz-rail-base-0.2.1/src/rail/examples_data/creation_data/data/success_rate_data/VVDSf02_I_success.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      973 2024-04-03 18:11:08.000000 pz-rail-base-0.2.1/src/rail/examples_data/creation_data/data/success_rate_data/VVDSf02_z_bright_success.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1873 2024-04-03 18:11:08.000000 pz-rail-base-0.2.1/src/rail/examples_data/creation_data/data/success_rate_data/VVDSf02_z_deep_success.txt
+-rw-r--r--   0 runner    (1001) docker     (127)  1000000 2024-04-03 18:11:08.000000 pz-rail-base-0.2.1/src/rail/examples_data/creation_data/data/success_rate_data/hsc_success.txt
+-rw-r--r--   0 runner    (1001) docker     (127)   431705 2024-04-03 18:11:08.000000 pz-rail-base-0.2.1/src/rail/examples_data/creation_data/data/success_rate_data/zCOSMOS_success.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 18:11:15.542290 pz-rail-base-0.2.1/src/rail/examples_data/estimation_data/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 18:11:15.558290 pz-rail-base-0.2.1/src/rail/examples_data/estimation_data/data/
+-rw-r--r--   0 runner    (1001) docker     (127)      219 2024-04-03 18:11:08.000000 pz-rail-base-0.2.1/src/rail/examples_data/estimation_data/data/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 18:11:15.558290 pz-rail-base-0.2.1/src/rail/examples_data/estimation_data/data/AB/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 18:11:08.000000 pz-rail-base-0.2.1/src/rail/examples_data/estimation_data/data/AB/dummy.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      454 2024-04-03 18:11:08.000000 pz-rail-base-0.2.1/src/rail/examples_data/estimation_data/data/CWW_HDFN_prior.pkl
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 18:11:15.558290 pz-rail-base-0.2.1/src/rail/examples_data/estimation_data/data/FILTER/
+-rw-r--r--   0 runner    (1001) docker     (127)    98003 2024-04-03 18:11:08.000000 pz-rail-base-0.2.1/src/rail/examples_data/estimation_data/data/FILTER/DC2LSST_g.res
+-rw-r--r--   0 runner    (1001) docker     (127)    95326 2024-04-03 18:11:08.000000 pz-rail-base-0.2.1/src/rail/examples_data/estimation_data/data/FILTER/DC2LSST_i.res
+-rw-r--r--   0 runner    (1001) docker     (127)    96635 2024-04-03 18:11:08.000000 pz-rail-base-0.2.1/src/rail/examples_data/estimation_data/data/FILTER/DC2LSST_r.res
+-rw-r--r--   0 runner    (1001) docker     (127)    90216 2024-04-03 18:11:08.000000 pz-rail-base-0.2.1/src/rail/examples_data/estimation_data/data/FILTER/DC2LSST_u.res
+-rw-r--r--   0 runner    (1001) docker     (127)   100126 2024-04-03 18:11:08.000000 pz-rail-base-0.2.1/src/rail/examples_data/estimation_data/data/FILTER/DC2LSST_y.res
+-rw-r--r--   0 runner    (1001) docker     (127)    93013 2024-04-03 18:11:08.000000 pz-rail-base-0.2.1/src/rail/examples_data/estimation_data/data/FILTER/DC2LSST_z.res
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 18:11:15.562290 pz-rail-base-0.2.1/src/rail/examples_data/estimation_data/data/SED/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      125 2024-04-03 18:11:08.000000 pz-rail-base-0.2.1/src/rail/examples_data/estimation_data/data/SED/CWWSB4.list
+-rwxr-xr-x   0 runner    (1001) docker     (127)    43750 2024-04-03 18:11:08.000000 pz-rail-base-0.2.1/src/rail/examples_data/estimation_data/data/SED/El_B2004a.sed
+-rwxr-xr-x   0 runner    (1001) docker     (127)    42830 2024-04-03 18:11:08.000000 pz-rail-base-0.2.1/src/rail/examples_data/estimation_data/data/SED/Im_B2004a.sed
+-rwxr-xr-x   0 runner    (1001) docker     (127)    72228 2024-04-03 18:11:08.000000 pz-rail-base-0.2.1/src/rail/examples_data/estimation_data/data/SED/SB2_B2004a.sed
+-rwxr-xr-x   0 runner    (1001) docker     (127)    68560 2024-04-03 18:11:08.000000 pz-rail-base-0.2.1/src/rail/examples_data/estimation_data/data/SED/SB3_B2004a.sed
+-rwxr-xr-x   0 runner    (1001) docker     (127)    43351 2024-04-03 18:11:08.000000 pz-rail-base-0.2.1/src/rail/examples_data/estimation_data/data/SED/Sbc_B2004a.sed
+-rwxr-xr-x   0 runner    (1001) docker     (127)    42789 2024-04-03 18:11:08.000000 pz-rail-base-0.2.1/src/rail/examples_data/estimation_data/data/SED/Scd_B2004a.sed
+-rwxr-xr-x   0 runner    (1001) docker     (127)   179585 2024-04-03 18:11:08.000000 pz-rail-base-0.2.1/src/rail/examples_data/estimation_data/data/SED/ssp_25Myr_z008.sed
+-rwxr-xr-x   0 runner    (1001) docker     (127)   179584 2024-04-03 18:11:08.000000 pz-rail-base-0.2.1/src/rail/examples_data/estimation_data/data/SED/ssp_5Myr_z008.sed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 18:11:15.562290 pz-rail-base-0.2.1/src/rail/examples_data/goldenspike_data/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 18:11:15.562290 pz-rail-base-0.2.1/src/rail/examples_data/goldenspike_data/configs/
+-rw-r--r--   0 runner    (1001) docker     (127)     6052 2024-04-03 18:11:08.000000 pz-rail-base-0.2.1/src/rail/examples_data/goldenspike_data/configs/goldenspike_config.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 18:11:15.562290 pz-rail-base-0.2.1/src/rail/examples_data/goldenspike_data/data/
+-rw-r--r--   0 runner    (1001) docker     (127)  1158108 2024-04-03 18:11:09.000000 pz-rail-base-0.2.1/src/rail/examples_data/goldenspike_data/data/pretrained_flow.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)   873947 2024-04-03 18:11:09.000000 pz-rail-base-0.2.1/src/rail/examples_data/goldenspike_data/data/test_flow_data.pq
+-rw-r--r--   0 runner    (1001) docker     (127)     1419 2024-04-03 18:11:09.000000 pz-rail-base-0.2.1/src/rail/examples_data/goldenspike_data/goldenspike.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 18:11:15.570290 pz-rail-base-0.2.1/src/rail/examples_data/testdata/
+-rw-r--r--   0 runner    (1001) docker     (127)      553 2024-04-03 18:11:09.000000 pz-rail-base-0.2.1/src/rail/examples_data/testdata/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)    91936 2024-04-03 18:11:09.000000 pz-rail-base-0.2.1/src/rail/examples_data/testdata/lsst_filters.npy
+-rw-r--r--   0 runner    (1001) docker     (127)     4742 2024-04-03 18:11:09.000000 pz-rail-base-0.2.1/src/rail/examples_data/testdata/make_rail_sample_data.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    43200 2024-04-03 18:11:09.000000 pz-rail-base-0.2.1/src/rail/examples_data/testdata/output_BPZ_lite.fits
+-rw-r--r--   0 runner    (1001) docker     (127)    37192 2024-04-03 18:11:09.000000 pz-rail-base-0.2.1/src/rail/examples_data/testdata/output_BPZ_lite.hdf5
+-rw-r--r--   0 runner    (1001) docker     (127)    24574 2024-04-03 18:11:09.000000 pz-rail-base-0.2.1/src/rail/examples_data/testdata/rubin_dm_dc2_example.pq
+-rw-r--r--   0 runner    (1001) docker     (127)   662976 2024-04-03 18:11:09.000000 pz-rail-base-0.2.1/src/rail/examples_data/testdata/test_dc2_training_9816.hdf5
+-rw-r--r--   0 runner    (1001) docker     (127)   873930 2024-04-03 18:11:09.000000 pz-rail-base-0.2.1/src/rail/examples_data/testdata/test_dc2_training_9816.pq
+-rw-r--r--   0 runner    (1001) docker     (127)  1192254 2024-04-03 18:11:09.000000 pz-rail-base-0.2.1/src/rail/examples_data/testdata/test_dc2_training_9816_hyperbolic.pq
+-rw-r--r--   0 runner    (1001) docker     (127)     5625 2024-04-03 18:11:09.000000 pz-rail-base-0.2.1/src/rail/examples_data/testdata/test_dc2_training_9816_smoothing_params.pq
+-rw-r--r--   0 runner    (1001) docker     (127)  1316984 2024-04-03 18:11:09.000000 pz-rail-base-0.2.1/src/rail/examples_data/testdata/test_dc2_validation_9816.hdf5
+-rw-r--r--   0 runner    (1001) docker     (127)    15192 2024-04-03 18:11:09.000000 pz-rail-base-0.2.1/src/rail/examples_data/testdata/training_100gal.hdf5
+-rw-r--r--   0 runner    (1001) docker     (127)     9200 2024-04-03 18:11:09.000000 pz-rail-base-0.2.1/src/rail/examples_data/testdata/validation_10gal.hdf5
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 18:11:15.570290 pz-rail-base-0.2.1/src/rail/stages/
+-rw-r--r--   0 runner    (1001) docker     (127)     1230 2024-04-03 18:11:09.000000 pz-rail-base-0.2.1/src/rail/stages/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 18:11:15.546290 pz-rail-base-0.2.1/tests/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 18:11:15.574290 pz-rail-base-0.2.1/tests/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)      833 2024-04-03 18:11:09.000000 pz-rail-base-0.2.1/tests/cli/hello_world.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     1095 2024-04-03 18:11:09.000000 pz-rail-base-0.2.1/tests/cli/single_number.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)      974 2024-04-03 18:11:09.000000 pz-rail-base-0.2.1/tests/cli/test_scripts.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 18:11:15.574290 pz-rail-base-0.2.1/tests/core/
+-rw-r--r--   0 runner    (1001) docker     (127)    10079 2024-04-03 18:11:09.000000 pz-rail-base-0.2.1/tests/core/test_core.py
+-rw-r--r--   0 runner    (1001) docker     (127)      811 2024-04-03 18:11:09.000000 pz-rail-base-0.2.1/tests/core/test_introspection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2780 2024-04-03 18:11:09.000000 pz-rail-base-0.2.1/tests/core/test_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4521 2024-04-03 18:11:09.000000 pz-rail-base-0.2.1/tests/core/test_point_estimation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 18:11:15.574290 pz-rail-base-0.2.1/tests/creation/
+-rw-r--r--   0 runner    (1001) docker     (127)     2369 2024-04-03 18:11:09.000000 pz-rail-base-0.2.1/tests/creation/test_degraders.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 18:11:15.574290 pz-rail-base-0.2.1/tests/estimation/
+-rw-r--r--   0 runner    (1001) docker     (127)     1656 2024-04-03 18:11:09.000000 pz-rail-base-0.2.1/tests/estimation/test_algos.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4337 2024-04-03 18:11:09.000000 pz-rail-base-0.2.1/tests/estimation/test_classifier.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2083 2024-04-03 18:11:09.000000 pz-rail-base-0.2.1/tests/estimation/test_summarizers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 18:11:15.574290 pz-rail-base-0.2.1/tests/evaluation/
+-rw-r--r--   0 runner    (1001) docker     (127)     2137 2024-04-03 18:11:09.000000 pz-rail-base-0.2.1/tests/evaluation/test_evaluation.py
```

### Comparing `pz-rail-base-0.2.0/.github/ISSUE_TEMPLATE/1-bug_report.md` & `pz-rail-base-0.2.1/.github/ISSUE_TEMPLATE/1-bug_report.md`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.2.0/.github/ISSUE_TEMPLATE/2-feature_request.md` & `pz-rail-base-0.2.1/.github/ISSUE_TEMPLATE/2-feature_request.md`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.2.0/.github/pull_request_template.md` & `pz-rail-base-0.2.1/.github/pull_request_template.md`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.2.0/.github/workflows/linting.yml` & `pz-rail-base-0.2.1/.github/workflows/linting.yml`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.2.0/.github/workflows/publish-to-pypi.yml` & `pz-rail-base-0.2.1/.github/workflows/publish-to-pypi.yml`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.2.0/.github/workflows/smoke-test.yml` & `pz-rail-base-0.2.1/.github/workflows/smoke-test.yml`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.2.0/.github/workflows/testing-and-coverage.yml` & `pz-rail-base-0.2.1/.github/workflows/testing-and-coverage.yml`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.2.0/.gitignore` & `pz-rail-base-0.2.1/.gitignore`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.2.0/.pre-commit-config.yaml` & `pz-rail-base-0.2.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.2.0/LICENSE` & `pz-rail-base-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.2.0/PKG-INFO` & `pz-rail-base-0.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pz-rail-base
-Version: 0.2.0
+Version: 0.2.1
 Author-email: "LSST Dark Energy Science Collaboration (DESC)" <later@later.com>
 License: MIT License
         
         Copyright (c) 2023 LSST Dark Energy Science Collaboration (DESC)
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
```

### Comparing `pz-rail-base-0.2.0/README.md` & `pz-rail-base-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.2.0/pyproject.toml` & `pz-rail-base-0.2.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.2.0/src/pz_rail_base.egg-info/PKG-INFO` & `pz-rail-base-0.2.1/src/pz_rail_base.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pz-rail-base
-Version: 0.2.0
+Version: 0.2.1
 Author-email: "LSST Dark Energy Science Collaboration (DESC)" <later@later.com>
 License: MIT License
         
         Copyright (c) 2023 LSST Dark Energy Science Collaboration (DESC)
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
```

### Comparing `pz-rail-base-0.2.0/src/pz_rail_base.egg-info/SOURCES.txt` & `pz-rail-base-0.2.1/src/pz_rail_base.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.2.0/src/rail/cli/commands.py` & `pz-rail-base-0.2.1/src/rail/cli/commands.py`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.2.0/src/rail/cli/options.py` & `pz-rail-base-0.2.1/src/rail/cli/options.py`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.2.0/src/rail/cli/scripts.py` & `pz-rail-base-0.2.1/src/rail/cli/scripts.py`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.2.0/src/rail/core/__init__.py` & `pz-rail-base-0.2.1/src/rail/core/__init__.py`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.2.0/src/rail/core/algo_utils.py` & `pz-rail-base-0.2.1/src/rail/core/algo_utils.py`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.2.0/src/rail/core/common_params.py` & `pz-rail-base-0.2.1/src/rail/core/common_params.py`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.2.0/src/rail/core/data.py` & `pz-rail-base-0.2.1/src/rail/core/data.py`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.2.0/src/rail/core/introspection.py` & `pz-rail-base-0.2.1/src/rail/core/introspection.py`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.2.0/src/rail/core/point_estimation.py` & `pz-rail-base-0.2.1/src/rail/core/point_estimation.py`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.2.0/src/rail/core/stage.py` & `pz-rail-base-0.2.1/src/rail/core/stage.py`

 * *Files 0% similar despite different names*

```diff
@@ -392,11 +392,12 @@
     def _finalize_tag(self, tag):
         """Finalize the data for a particular tag.
 
         This can be overridden by sub-classes for more complicated behavior
         """
         handle = self.get_handle(tag, allow_missing=True)
         if self.config.output_mode == 'default':
-            handle.write()
+            if not os.path.exists(handle.path) or not handle.partial:
+                handle.write()            
         final_name = PipelineStage._finalize_tag(self, tag)
         handle.path = final_name
         return final_name
```

### Comparing `pz-rail-base-0.2.0/src/rail/core/util_stages.py` & `pz-rail-base-0.2.1/src/rail/core/util_stages.py`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.2.0/src/rail/core/utils.py` & `pz-rail-base-0.2.1/src/rail/core/utils.py`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.2.0/src/rail/creation/degradation/quantityCut.py` & `pz-rail-base-0.2.1/src/rail/creation/degradation/quantityCut.py`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.2.0/src/rail/creation/degrader.py` & `pz-rail-base-0.2.1/src/rail/creation/degrader.py`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.2.0/src/rail/creation/engine.py` & `pz-rail-base-0.2.1/src/rail/creation/engine.py`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.2.0/src/rail/estimation/algos/equal_count.py` & `pz-rail-base-0.2.1/src/rail/estimation/algos/equal_count.py`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.2.0/src/rail/estimation/algos/naive_stack.py` & `pz-rail-base-0.2.1/src/rail/estimation/algos/naive_stack.py`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.2.0/src/rail/estimation/algos/point_est_hist.py` & `pz-rail-base-0.2.1/src/rail/estimation/algos/point_est_hist.py`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.2.0/src/rail/estimation/algos/random_gauss.py` & `pz-rail-base-0.2.1/src/rail/estimation/algos/random_gauss.py`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.2.0/src/rail/estimation/algos/train_z.py` & `pz-rail-base-0.2.1/src/rail/estimation/algos/train_z.py`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.2.0/src/rail/estimation/algos/uniform_binning.py` & `pz-rail-base-0.2.1/src/rail/estimation/algos/uniform_binning.py`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.2.0/src/rail/estimation/algos/var_inf.py` & `pz-rail-base-0.2.1/src/rail/estimation/algos/var_inf.py`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.2.0/src/rail/estimation/classifier.py` & `pz-rail-base-0.2.1/src/rail/estimation/classifier.py`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.2.0/src/rail/estimation/estimator.py` & `pz-rail-base-0.2.1/src/rail/estimation/estimator.py`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.2.0/src/rail/estimation/informer.py` & `pz-rail-base-0.2.1/src/rail/estimation/informer.py`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.2.0/src/rail/estimation/summarizer.py` & `pz-rail-base-0.2.1/src/rail/estimation/summarizer.py`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.2.0/src/rail/evaluation/evaluator.py` & `pz-rail-base-0.2.1/src/rail/evaluation/evaluator.py`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.2.0/src/rail/evaluation/metrics/base.py` & `pz-rail-base-0.2.1/src/rail/evaluation/metrics/base.py`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.2.0/src/rail/evaluation/metrics/cdeloss.py` & `pz-rail-base-0.2.1/src/rail/evaluation/metrics/cdeloss.py`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.2.0/src/rail/evaluation/metrics/pointestimates.py` & `pz-rail-base-0.2.1/src/rail/evaluation/metrics/pointestimates.py`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.2.0/src/rail/examples_data/creation_data/data/success_rate_data/DEEP2_success.txt` & `pz-rail-base-0.2.1/src/rail/examples_data/creation_data/data/success_rate_data/DEEP2_success.txt`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.2.0/src/rail/examples_data/creation_data/data/success_rate_data/VVDSf02_z_bright_success.txt` & `pz-rail-base-0.2.1/src/rail/examples_data/creation_data/data/success_rate_data/VVDSf02_z_bright_success.txt`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.2.0/src/rail/examples_data/creation_data/data/success_rate_data/VVDSf02_z_deep_success.txt` & `pz-rail-base-0.2.1/src/rail/examples_data/creation_data/data/success_rate_data/VVDSf02_z_deep_success.txt`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.2.0/src/rail/examples_data/creation_data/data/success_rate_data/hsc_success.txt` & `pz-rail-base-0.2.1/src/rail/examples_data/creation_data/data/success_rate_data/hsc_success.txt`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.2.0/src/rail/examples_data/creation_data/data/success_rate_data/zCOSMOS_success.txt` & `pz-rail-base-0.2.1/src/rail/examples_data/creation_data/data/success_rate_data/zCOSMOS_success.txt`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.2.0/src/rail/examples_data/estimation_data/data/FILTER/DC2LSST_g.res` & `pz-rail-base-0.2.1/src/rail/examples_data/estimation_data/data/FILTER/DC2LSST_g.res`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.2.0/src/rail/examples_data/estimation_data/data/FILTER/DC2LSST_i.res` & `pz-rail-base-0.2.1/src/rail/examples_data/estimation_data/data/FILTER/DC2LSST_i.res`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.2.0/src/rail/examples_data/estimation_data/data/FILTER/DC2LSST_r.res` & `pz-rail-base-0.2.1/src/rail/examples_data/estimation_data/data/FILTER/DC2LSST_r.res`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.2.0/src/rail/examples_data/estimation_data/data/FILTER/DC2LSST_u.res` & `pz-rail-base-0.2.1/src/rail/examples_data/estimation_data/data/FILTER/DC2LSST_u.res`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.2.0/src/rail/examples_data/estimation_data/data/FILTER/DC2LSST_y.res` & `pz-rail-base-0.2.1/src/rail/examples_data/estimation_data/data/FILTER/DC2LSST_y.res`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.2.0/src/rail/examples_data/estimation_data/data/FILTER/DC2LSST_z.res` & `pz-rail-base-0.2.1/src/rail/examples_data/estimation_data/data/FILTER/DC2LSST_z.res`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.2.0/src/rail/examples_data/estimation_data/data/SED/El_B2004a.sed` & `pz-rail-base-0.2.1/src/rail/examples_data/estimation_data/data/SED/El_B2004a.sed`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.2.0/src/rail/examples_data/estimation_data/data/SED/Im_B2004a.sed` & `pz-rail-base-0.2.1/src/rail/examples_data/estimation_data/data/SED/Im_B2004a.sed`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.2.0/src/rail/examples_data/estimation_data/data/SED/SB2_B2004a.sed` & `pz-rail-base-0.2.1/src/rail/examples_data/estimation_data/data/SED/SB2_B2004a.sed`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.2.0/src/rail/examples_data/estimation_data/data/SED/SB3_B2004a.sed` & `pz-rail-base-0.2.1/src/rail/examples_data/estimation_data/data/SED/SB3_B2004a.sed`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.2.0/src/rail/examples_data/estimation_data/data/SED/Sbc_B2004a.sed` & `pz-rail-base-0.2.1/src/rail/examples_data/estimation_data/data/SED/Sbc_B2004a.sed`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.2.0/src/rail/examples_data/estimation_data/data/SED/Scd_B2004a.sed` & `pz-rail-base-0.2.1/src/rail/examples_data/estimation_data/data/SED/Scd_B2004a.sed`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.2.0/src/rail/examples_data/estimation_data/data/SED/ssp_25Myr_z008.sed` & `pz-rail-base-0.2.1/src/rail/examples_data/estimation_data/data/SED/ssp_25Myr_z008.sed`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.2.0/src/rail/examples_data/estimation_data/data/SED/ssp_5Myr_z008.sed` & `pz-rail-base-0.2.1/src/rail/examples_data/estimation_data/data/SED/ssp_5Myr_z008.sed`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.2.0/src/rail/examples_data/goldenspike_data/configs/goldenspike_config.yml` & `pz-rail-base-0.2.1/src/rail/examples_data/goldenspike_data/configs/goldenspike_config.yml`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.2.0/src/rail/examples_data/goldenspike_data/data/pretrained_flow.pkl` & `pz-rail-base-0.2.1/src/rail/examples_data/goldenspike_data/data/pretrained_flow.pkl`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.2.0/src/rail/examples_data/goldenspike_data/data/test_flow_data.pq` & `pz-rail-base-0.2.1/src/rail/examples_data/goldenspike_data/data/test_flow_data.pq`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.2.0/src/rail/examples_data/goldenspike_data/goldenspike.yml` & `pz-rail-base-0.2.1/src/rail/examples_data/goldenspike_data/goldenspike.yml`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.2.0/src/rail/examples_data/testdata/README.md` & `pz-rail-base-0.2.1/src/rail/examples_data/testdata/README.md`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.2.0/src/rail/examples_data/testdata/lsst_filters.npy` & `pz-rail-base-0.2.1/src/rail/examples_data/testdata/lsst_filters.npy`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.2.0/src/rail/examples_data/testdata/make_rail_sample_data.ipynb` & `pz-rail-base-0.2.1/src/rail/examples_data/testdata/make_rail_sample_data.ipynb`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.2.0/src/rail/examples_data/testdata/output_BPZ_lite.fits` & `pz-rail-base-0.2.1/src/rail/examples_data/testdata/output_BPZ_lite.fits`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.2.0/src/rail/examples_data/testdata/output_BPZ_lite.hdf5` & `pz-rail-base-0.2.1/src/rail/examples_data/testdata/output_BPZ_lite.hdf5`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.2.0/src/rail/examples_data/testdata/rubin_dm_dc2_example.pq` & `pz-rail-base-0.2.1/src/rail/examples_data/testdata/rubin_dm_dc2_example.pq`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.2.0/src/rail/examples_data/testdata/test_dc2_training_9816.hdf5` & `pz-rail-base-0.2.1/src/rail/examples_data/testdata/test_dc2_training_9816.hdf5`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.2.0/src/rail/examples_data/testdata/test_dc2_training_9816.pq` & `pz-rail-base-0.2.1/src/rail/examples_data/testdata/test_dc2_training_9816.pq`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.2.0/src/rail/examples_data/testdata/test_dc2_training_9816_hyperbolic.pq` & `pz-rail-base-0.2.1/src/rail/examples_data/testdata/test_dc2_training_9816_hyperbolic.pq`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.2.0/src/rail/examples_data/testdata/test_dc2_training_9816_smoothing_params.pq` & `pz-rail-base-0.2.1/src/rail/examples_data/testdata/test_dc2_training_9816_smoothing_params.pq`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.2.0/src/rail/examples_data/testdata/test_dc2_validation_9816.hdf5` & `pz-rail-base-0.2.1/src/rail/examples_data/testdata/test_dc2_validation_9816.hdf5`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.2.0/src/rail/examples_data/testdata/training_100gal.hdf5` & `pz-rail-base-0.2.1/src/rail/examples_data/testdata/training_100gal.hdf5`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.2.0/src/rail/examples_data/testdata/validation_10gal.hdf5` & `pz-rail-base-0.2.1/src/rail/examples_data/testdata/validation_10gal.hdf5`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.2.0/src/rail/stages/__init__.py` & `pz-rail-base-0.2.1/src/rail/stages/__init__.py`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.2.0/tests/cli/hello_world.ipynb` & `pz-rail-base-0.2.1/tests/cli/hello_world.ipynb`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.2.0/tests/cli/single_number.ipynb` & `pz-rail-base-0.2.1/tests/cli/single_number.ipynb`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.2.0/tests/cli/test_scripts.py` & `pz-rail-base-0.2.1/tests/cli/test_scripts.py`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.2.0/tests/core/test_core.py` & `pz-rail-base-0.2.1/tests/core/test_core.py`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.2.0/tests/core/test_introspection.py` & `pz-rail-base-0.2.1/tests/core/test_introspection.py`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.2.0/tests/core/test_pipeline.py` & `pz-rail-base-0.2.1/tests/core/test_pipeline.py`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.2.0/tests/core/test_point_estimation.py` & `pz-rail-base-0.2.1/tests/core/test_point_estimation.py`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.2.0/tests/creation/test_degraders.py` & `pz-rail-base-0.2.1/tests/creation/test_degraders.py`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.2.0/tests/estimation/test_algos.py` & `pz-rail-base-0.2.1/tests/estimation/test_algos.py`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.2.0/tests/estimation/test_classifier.py` & `pz-rail-base-0.2.1/tests/estimation/test_classifier.py`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.2.0/tests/estimation/test_summarizers.py` & `pz-rail-base-0.2.1/tests/estimation/test_summarizers.py`

 * *Files identical despite different names*

### Comparing `pz-rail-base-0.2.0/tests/evaluation/test_evaluation.py` & `pz-rail-base-0.2.1/tests/evaluation/test_evaluation.py`

 * *Files identical despite different names*

