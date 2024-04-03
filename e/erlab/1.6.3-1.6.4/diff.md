# Comparing `tmp/erlab-1.6.3.tar.gz` & `tmp/erlab-1.6.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "erlab-1.6.3.tar", last modified: Wed Apr  3 08:07:48 2024, max compression
+gzip compressed data, was "erlab-1.6.4.tar", last modified: Wed Apr  3 08:23:58 2024, max compression
```

## Comparing `erlab-1.6.3.tar` & `erlab-1.6.4.tar`

### file list

```diff
@@ -1,161 +1,161 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 08:07:48.416785 erlab-1.6.3/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 08:07:48.376785 erlab-1.6.3/.github/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 08:07:48.380785 erlab-1.6.3/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 root         (0) root         (0)      469 2024-04-03 08:07:42.000000 erlab-1.6.3/.github/ISSUE_TEMPLATE/bug-report.md
--rw-r--r--   0 root         (0) root         (0)      608 2024-04-03 08:07:42.000000 erlab-1.6.3/.github/ISSUE_TEMPLATE/feature_request.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 08:07:48.380785 erlab-1.6.3/.github/workflows/
--rw-r--r--   0 root         (0) root         (0)     1047 2024-04-03 08:07:42.000000 erlab-1.6.3/.github/workflows/pr.yml
--rw-r--r--   0 root         (0) root         (0)     1893 2024-04-03 08:07:42.000000 erlab-1.6.3/.github/workflows/release.yml
--rw-r--r--   0 root         (0) root         (0)     2898 2024-04-03 08:07:42.000000 erlab-1.6.3/.gitignore
--rw-r--r--   0 root         (0) root         (0)      893 2024-04-03 08:07:42.000000 erlab-1.6.3/.pre-commit-config.yaml
--rw-r--r--   0 root         (0) root         (0)      796 2024-04-03 08:07:42.000000 erlab-1.6.3/.readthedocs.yaml
--rw-r--r--   0 root         (0) root         (0)    96912 2024-04-03 08:07:44.000000 erlab-1.6.3/CHANGELOG.md
--rw-r--r--   0 root         (0) root         (0)    35149 2024-04-03 08:07:42.000000 erlab-1.6.3/LICENSE
--rw-r--r--   0 root         (0) root         (0)    46708 2024-04-03 08:07:48.416785 erlab-1.6.3/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1473 2024-04-03 08:07:42.000000 erlab-1.6.3/PythonInterface.ipf
--rw-r--r--   0 root         (0) root         (0)     4414 2024-04-03 08:07:42.000000 erlab-1.6.3/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 08:07:48.384785 erlab-1.6.3/docs/
--rw-r--r--   0 root         (0) root         (0)      638 2024-04-03 08:07:42.000000 erlab-1.6.3/docs/Makefile
--rw-r--r--   0 root         (0) root         (0)      752 2024-04-03 08:07:42.000000 erlab-1.6.3/docs/environment.yml
--rw-r--r--   0 root         (0) root         (0)      804 2024-04-03 08:07:42.000000 erlab-1.6.3/docs/make.bat
--rw-r--r--   0 root         (0) root         (0)      540 2024-04-03 08:07:42.000000 erlab-1.6.3/docs/requirements.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 08:07:48.388785 erlab-1.6.3/docs/source/
--rw-r--r--   0 root         (0) root         (0)       52 2024-04-03 08:07:42.000000 erlab-1.6.3/docs/source/bibliography.rst
--rw-r--r--   0 root         (0) root         (0)    10762 2024-04-03 08:07:42.000000 erlab-1.6.3/docs/source/conf.py
--rw-r--r--   0 root         (0) root         (0)    13410 2024-04-03 08:07:42.000000 erlab-1.6.3/docs/source/development.rst
--rw-r--r--   0 root         (0) root         (0)      265 2024-04-03 08:07:42.000000 erlab-1.6.3/docs/source/erlab.accessors.rst
--rw-r--r--   0 root         (0) root         (0)      101 2024-04-03 08:07:42.000000 erlab-1.6.3/docs/source/erlab.analysis.rst
--rw-r--r--   0 root         (0) root         (0)      141 2024-04-03 08:07:42.000000 erlab-1.6.3/docs/source/erlab.characterization.rst
--rw-r--r--   0 root         (0) root         (0)      485 2024-04-03 08:07:42.000000 erlab-1.6.3/docs/source/erlab.constants.rst
--rw-r--r--   0 root         (0) root         (0)      116 2024-04-03 08:07:42.000000 erlab-1.6.3/docs/source/erlab.interactive.rst
--rw-r--r--   0 root         (0) root         (0)       81 2024-04-03 08:07:42.000000 erlab-1.6.3/docs/source/erlab.io.rst
--rw-r--r--   0 root         (0) root         (0)      236 2024-04-03 08:07:42.000000 erlab-1.6.3/docs/source/erlab.lattice.rst
--rw-r--r--   0 root         (0) root         (0)      242 2024-04-03 08:07:42.000000 erlab-1.6.3/docs/source/erlab.parallel.rst
--rw-r--r--   0 root         (0) root         (0)      174 2024-04-03 08:07:42.000000 erlab-1.6.3/docs/source/erlab.plotting.rst
--rw-r--r--   0 root         (0) root         (0)     2888 2024-04-03 08:07:42.000000 erlab-1.6.3/docs/source/getting-started.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 08:07:48.392785 erlab-1.6.3/docs/source/images/
--rw-r--r--   0 root         (0) root         (0)   996803 2024-04-03 08:07:42.000000 erlab-1.6.3/docs/source/images/imagetool_dark.png
--rw-r--r--   0 root         (0) root         (0)   966547 2024-04-03 08:07:42.000000 erlab-1.6.3/docs/source/images/imagetool_light.png
--rw-r--r--   0 root         (0) root         (0)   709231 2024-04-03 08:07:42.000000 erlab-1.6.3/docs/source/images/ktool_1_dark.png
--rw-r--r--   0 root         (0) root         (0)   694078 2024-04-03 08:07:42.000000 erlab-1.6.3/docs/source/images/ktool_1_light.png
--rw-r--r--   0 root         (0) root         (0)   703343 2024-04-03 08:07:42.000000 erlab-1.6.3/docs/source/images/ktool_2_dark.png
--rw-r--r--   0 root         (0) root         (0)   686688 2024-04-03 08:07:42.000000 erlab-1.6.3/docs/source/images/ktool_2_light.png
--rw-r--r--   0 root         (0) root         (0)     2497 2024-04-03 08:07:42.000000 erlab-1.6.3/docs/source/index.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 08:07:48.396785 erlab-1.6.3/docs/source/notebooks/
--rw-r--r--   0 root         (0) root         (0)   189769 2024-04-03 08:07:42.000000 erlab-1.6.3/docs/source/notebooks/indexing.ipynb
--rw-r--r--   0 root         (0) root         (0)     1582 2024-04-03 08:07:42.000000 erlab-1.6.3/docs/source/notebooks/io.ipynb
--rw-r--r--   0 root         (0) root         (0)   379528 2024-04-03 08:07:42.000000 erlab-1.6.3/docs/source/notebooks/kconv.ipynb
--rw-r--r--   0 root         (0) root         (0)    15761 2024-04-03 08:07:42.000000 erlab-1.6.3/docs/source/notebooks/plotting.ipynb
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 08:07:48.396785 erlab-1.6.3/docs/source/pyplots/
--rw-r--r--   0 root         (0) root         (0)     2579 2024-04-03 08:07:42.000000 erlab-1.6.3/docs/source/pyplots/norms.py
--rw-r--r--   0 root         (0) root         (0)     1344 2024-04-03 08:07:42.000000 erlab-1.6.3/docs/source/reference.rst
--rw-r--r--   0 root         (0) root         (0)     1316 2024-04-03 08:07:42.000000 erlab-1.6.3/docs/source/refs.bib
--rw-r--r--   0 root         (0) root         (0)     1142 2024-04-03 08:07:42.000000 erlab-1.6.3/docs/source/userguide.rst
--rw-r--r--   0 root         (0) root         (0)      880 2024-04-03 08:07:42.000000 erlab-1.6.3/environment.yml
--rw-r--r--   0 root         (0) root         (0)      990 2024-04-03 08:07:42.000000 erlab-1.6.3/environment_apple.yml
--rw-r--r--   0 root         (0) root         (0)      876 2024-04-03 08:07:42.000000 erlab-1.6.3/environment_nogit.yml
--rw-r--r--   0 root         (0) root         (0)      848 2024-04-03 08:07:42.000000 erlab-1.6.3/environment_nogit_mkl.yml
--rw-r--r--   0 root         (0) root         (0)     4227 2024-04-03 08:07:42.000000 erlab-1.6.3/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)      334 2024-04-03 08:07:42.000000 erlab-1.6.3/requirements.txt
--rw-r--r--   0 root         (0) root         (0)       38 2024-04-03 08:07:48.416785 erlab-1.6.3/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 08:07:48.376785 erlab-1.6.3/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 08:07:48.396785 erlab-1.6.3/src/erlab/
--rw-r--r--   0 root         (0) root         (0)       60 2024-04-03 08:07:44.000000 erlab-1.6.3/src/erlab/__init__.py
--rw-r--r--   0 root         (0) root         (0)    35539 2024-04-03 08:07:42.000000 erlab-1.6.3/src/erlab/accessors.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 08:07:48.400785 erlab-1.6.3/src/erlab/analysis/
--rw-r--r--   0 root         (0) root         (0)      748 2024-04-03 08:07:42.000000 erlab-1.6.3/src/erlab/analysis/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5514 2024-04-03 08:07:42.000000 erlab-1.6.3/src/erlab/analysis/correlation.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 08:07:48.400785 erlab-1.6.3/src/erlab/analysis/fit/
--rw-r--r--   0 root         (0) root         (0)      459 2024-04-03 08:07:42.000000 erlab-1.6.3/src/erlab/analysis/fit/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 08:07:48.400785 erlab-1.6.3/src/erlab/analysis/fit/functions/
--rw-r--r--   0 root         (0) root         (0)      812 2024-04-03 08:07:42.000000 erlab-1.6.3/src/erlab/analysis/fit/functions/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8766 2024-04-03 08:07:42.000000 erlab-1.6.3/src/erlab/analysis/fit/functions/dynamic.py
--rw-r--r--   0 root         (0) root         (0)     6026 2024-04-03 08:07:42.000000 erlab-1.6.3/src/erlab/analysis/fit/functions/general.py
--rw-r--r--   0 root         (0) root         (0)     6165 2024-04-03 08:07:42.000000 erlab-1.6.3/src/erlab/analysis/fit/minuit.py
--rw-r--r--   0 root         (0) root         (0)    10572 2024-04-03 08:07:42.000000 erlab-1.6.3/src/erlab/analysis/fit/models.py
--rw-r--r--   0 root         (0) root         (0)     1168 2024-04-03 08:07:42.000000 erlab-1.6.3/src/erlab/analysis/fit/spline.py
--rw-r--r--   0 root         (0) root         (0)    13815 2024-04-03 08:07:42.000000 erlab-1.6.3/src/erlab/analysis/gold.py
--rw-r--r--   0 root         (0) root         (0)     9811 2024-04-03 08:07:42.000000 erlab-1.6.3/src/erlab/analysis/interpolate.py
--rw-r--r--   0 root         (0) root         (0)    10344 2024-04-03 08:07:42.000000 erlab-1.6.3/src/erlab/analysis/kspace.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 08:07:48.400785 erlab-1.6.3/src/erlab/analysis/mask/
--rw-r--r--   0 root         (0) root         (0)     2768 2024-04-03 08:07:42.000000 erlab-1.6.3/src/erlab/analysis/mask/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7810 2024-04-03 08:07:42.000000 erlab-1.6.3/src/erlab/analysis/mask/polygon.py
--rw-r--r--   0 root         (0) root         (0)      878 2024-04-03 08:07:42.000000 erlab-1.6.3/src/erlab/analysis/transform.py
--rw-r--r--   0 root         (0) root         (0)     8332 2024-04-03 08:07:42.000000 erlab-1.6.3/src/erlab/analysis/utilities.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 08:07:48.400785 erlab-1.6.3/src/erlab/characterization/
--rw-r--r--   0 root         (0) root         (0)      191 2024-04-03 08:07:42.000000 erlab-1.6.3/src/erlab/characterization/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3093 2024-04-03 08:07:42.000000 erlab-1.6.3/src/erlab/characterization/resistance.py
--rw-r--r--   0 root         (0) root         (0)     1903 2024-04-03 08:07:42.000000 erlab-1.6.3/src/erlab/characterization/xrd.py
--rw-r--r--   0 root         (0) root         (0)     2115 2024-04-03 08:07:42.000000 erlab-1.6.3/src/erlab/constants.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 08:07:48.404785 erlab-1.6.3/src/erlab/interactive/
--rw-r--r--   0 root         (0) root         (0)      540 2024-04-03 08:07:42.000000 erlab-1.6.3/src/erlab/interactive/__init__.py
--rw-r--r--   0 root         (0) root         (0)    13943 2024-04-03 08:07:42.000000 erlab-1.6.3/src/erlab/interactive/bzplot.py
--rw-r--r--   0 root         (0) root         (0)    20820 2024-04-03 08:07:42.000000 erlab-1.6.3/src/erlab/interactive/colors.py
--rw-r--r--   0 root         (0) root         (0)    22076 2024-04-03 08:07:42.000000 erlab-1.6.3/src/erlab/interactive/curvefittingtool.py
--rw-r--r--   0 root         (0) root         (0)    19528 2024-04-03 08:07:42.000000 erlab-1.6.3/src/erlab/interactive/derivative.py
--rw-r--r--   0 root         (0) root         (0)     9458 2024-04-03 08:07:42.000000 erlab-1.6.3/src/erlab/interactive/exampledata.py
--rw-r--r--   0 root         (0) root         (0)    19072 2024-04-03 08:07:42.000000 erlab-1.6.3/src/erlab/interactive/fermiedge.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 08:07:48.404785 erlab-1.6.3/src/erlab/interactive/imagetool/
--rw-r--r--   0 root         (0) root         (0)    19391 2024-04-03 08:07:42.000000 erlab-1.6.3/src/erlab/interactive/imagetool/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 08:07:48.404785 erlab-1.6.3/src/erlab/interactive/imagetool/_deprecated/
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-03 08:07:42.000000 erlab-1.6.3/src/erlab/interactive/imagetool/_deprecated/__init__.py
--rw-r--r--   0 root         (0) root         (0)    52076 2024-04-03 08:07:42.000000 erlab-1.6.3/src/erlab/interactive/imagetool/_deprecated/imagetool_mpl.py
--rw-r--r--   0 root         (0) root         (0)   114751 2024-04-03 08:07:42.000000 erlab-1.6.3/src/erlab/interactive/imagetool/_deprecated/imagetool_old.py
--rw-r--r--   0 root         (0) root         (0)    27081 2024-04-03 08:07:42.000000 erlab-1.6.3/src/erlab/interactive/imagetool/controls.py
--rw-r--r--   0 root         (0) root         (0)    53776 2024-04-03 08:07:42.000000 erlab-1.6.3/src/erlab/interactive/imagetool/core.py
--rw-r--r--   0 root         (0) root         (0)    11483 2024-04-03 08:07:42.000000 erlab-1.6.3/src/erlab/interactive/imagetool/fastbinning.py
--rw-r--r--   0 root         (0) root         (0)    23195 2024-04-03 08:07:42.000000 erlab-1.6.3/src/erlab/interactive/imagetool/slicer.py
--rw-r--r--   0 root         (0) root         (0)    16658 2024-04-03 08:07:42.000000 erlab-1.6.3/src/erlab/interactive/kspace.py
--rw-r--r--   0 root         (0) root         (0)    19382 2024-04-03 08:07:42.000000 erlab-1.6.3/src/erlab/interactive/ktool.ui
--rw-r--r--   0 root         (0) root         (0)     3341 2024-04-03 08:07:42.000000 erlab-1.6.3/src/erlab/interactive/masktool.py
--rw-r--r--   0 root         (0) root         (0)    52417 2024-04-03 08:07:42.000000 erlab-1.6.3/src/erlab/interactive/utilities.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 08:07:48.408785 erlab-1.6.3/src/erlab/io/
--rw-r--r--   0 root         (0) root         (0)     1937 2024-04-03 08:07:42.000000 erlab-1.6.3/src/erlab/io/__init__.py
--rw-r--r--   0 root         (0) root         (0)    30047 2024-04-03 08:07:42.000000 erlab-1.6.3/src/erlab/io/dataloader.py
--rw-r--r--   0 root         (0) root         (0)     8084 2024-04-03 08:07:42.000000 erlab-1.6.3/src/erlab/io/igor.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 08:07:48.408785 erlab-1.6.3/src/erlab/io/plugins/
--rw-r--r--   0 root         (0) root         (0)      900 2024-04-03 08:07:42.000000 erlab-1.6.3/src/erlab/io/plugins/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3674 2024-04-03 08:07:42.000000 erlab-1.6.3/src/erlab/io/plugins/da30.py
--rw-r--r--   0 root         (0) root         (0)     1185 2024-04-03 08:07:42.000000 erlab-1.6.3/src/erlab/io/plugins/kriss.py
--rw-r--r--   0 root         (0) root         (0)     7448 2024-04-03 08:07:42.000000 erlab-1.6.3/src/erlab/io/plugins/merlin.py
--rw-r--r--   0 root         (0) root         (0)     7745 2024-04-03 08:07:42.000000 erlab-1.6.3/src/erlab/io/plugins/ssrl52.py
--rw-r--r--   0 root         (0) root         (0)     5630 2024-04-03 08:07:42.000000 erlab-1.6.3/src/erlab/io/utilities.py
--rw-r--r--   0 root         (0) root         (0)     2515 2024-04-03 08:07:42.000000 erlab-1.6.3/src/erlab/lattice.py
--rw-r--r--   0 root         (0) root         (0)     2242 2024-04-03 08:07:42.000000 erlab-1.6.3/src/erlab/parallel.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 08:07:48.408785 erlab-1.6.3/src/erlab/plotting/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 08:07:48.412785 erlab-1.6.3/src/erlab/plotting/IgorCT/
--rw-r--r--   0 root         (0) root         (0)     3379 2024-04-03 08:07:42.000000 erlab-1.6.3/src/erlab/plotting/IgorCT/Blue-White.txt
--rw-r--r--   0 root         (0) root         (0)     3456 2024-04-03 08:07:42.000000 erlab-1.6.3/src/erlab/plotting/IgorCT/BlueHot.ibw
--rw-r--r--   0 root         (0) root         (0)     3526 2024-04-03 08:07:42.000000 erlab-1.6.3/src/erlab/plotting/IgorCT/CTBlueWhite.ibw
--rw-r--r--   0 root         (0) root         (0)     3530 2024-04-03 08:07:42.000000 erlab-1.6.3/src/erlab/plotting/IgorCT/CTRainbowLIght.ibw
--rw-r--r--   0 root         (0) root         (0)     3531 2024-04-03 08:07:42.000000 erlab-1.6.3/src/erlab/plotting/IgorCT/CTRedTemperature.ibw
--rw-r--r--   0 root         (0) root         (0)     3456 2024-04-03 08:07:42.000000 erlab-1.6.3/src/erlab/plotting/IgorCT/ColdWarm.ibw
--rw-r--r--   0 root         (0) root         (0)     3456 2024-04-03 08:07:42.000000 erlab-1.6.3/src/erlab/plotting/IgorCT/PlanetEarth.ibw
--rw-r--r--   0 root         (0) root         (0)     1920 2024-04-03 08:07:42.000000 erlab-1.6.3/src/erlab/plotting/IgorCT/ametrine.ibw
--rw-r--r--   0 root         (0) root         (0)     2048 2024-04-03 08:07:42.000000 erlab-1.6.3/src/erlab/plotting/IgorCT/isolum.ibw
--rw-r--r--   0 root         (0) root         (0)     2048 2024-04-03 08:07:42.000000 erlab-1.6.3/src/erlab/plotting/IgorCT/morgenstemning.ibw
--rw-r--r--   0 root         (0) root         (0)     1784 2024-04-03 08:07:42.000000 erlab-1.6.3/src/erlab/plotting/__init__.py
--rw-r--r--   0 root         (0) root         (0)    29010 2024-04-03 08:07:42.000000 erlab-1.6.3/src/erlab/plotting/annotations.py
--rw-r--r--   0 root         (0) root         (0)    18275 2024-04-03 08:07:42.000000 erlab-1.6.3/src/erlab/plotting/atoms.py
--rw-r--r--   0 root         (0) root         (0)     4294 2024-04-03 08:07:42.000000 erlab-1.6.3/src/erlab/plotting/bz.py
--rw-r--r--   0 root         (0) root         (0)    32411 2024-04-03 08:07:42.000000 erlab-1.6.3/src/erlab/plotting/colors.py
--rw-r--r--   0 root         (0) root         (0)     2657 2024-04-03 08:07:42.000000 erlab-1.6.3/src/erlab/plotting/erplot.py
--rw-r--r--   0 root         (0) root         (0)    30998 2024-04-03 08:07:42.000000 erlab-1.6.3/src/erlab/plotting/general.py
--rw-r--r--   0 root         (0) root         (0)     2726 2024-04-03 08:07:42.000000 erlab-1.6.3/src/erlab/plotting/plot3d.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 08:07:48.412785 erlab-1.6.3/src/erlab/plotting/stylelib/
--rw-r--r--   0 root         (0) root         (0)     6839 2024-04-03 08:07:42.000000 erlab-1.6.3/src/erlab/plotting/stylelib/fira.mplstyle
--rw-r--r--   0 root         (0) root         (0)     6826 2024-04-03 08:07:42.000000 erlab-1.6.3/src/erlab/plotting/stylelib/firalight.mplstyle
--rw-r--r--   0 root         (0) root         (0)    14358 2024-04-03 08:07:42.000000 erlab-1.6.3/src/erlab/plotting/stylelib/khan.mplstyle
--rw-r--r--   0 root         (0) root         (0)     9160 2024-04-03 08:07:42.000000 erlab-1.6.3/src/erlab/plotting/stylelib/nature.mplstyle
--rw-r--r--   0 root         (0) root         (0)      630 2024-04-03 08:07:42.000000 erlab-1.6.3/src/erlab/plotting/stylelib/poster.mplstyle
--rw-r--r--   0 root         (0) root         (0)     7023 2024-04-03 08:07:42.000000 erlab-1.6.3/src/erlab/plotting/stylelib/times.mplstyle
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 08:07:48.412785 erlab-1.6.3/src/erlab.egg-info/
--rw-r--r--   0 root         (0) root         (0)    46708 2024-04-03 08:07:48.000000 erlab-1.6.3/src/erlab.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     4265 2024-04-03 08:07:48.000000 erlab-1.6.3/src/erlab.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-03 08:07:48.000000 erlab-1.6.3/src/erlab.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      321 2024-04-03 08:07:48.000000 erlab-1.6.3/src/erlab.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        6 2024-04-03 08:07:48.000000 erlab-1.6.3/src/erlab.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 08:07:48.412785 erlab-1.6.3/tests/
--rw-r--r--   0 root         (0) root         (0)      595 2024-04-03 08:07:42.000000 erlab-1.6.3/tests/test_fastbinning.py
--rw-r--r--   0 root         (0) root         (0)      598 2024-04-03 08:07:42.000000 erlab-1.6.3/tests/test_interpolate.py
--rw-r--r--   0 root         (0) root         (0)     2419 2024-04-03 08:07:42.000000 erlab-1.6.3/tests/test_kspace.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 08:23:58.650098 erlab-1.6.4/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 08:23:58.610097 erlab-1.6.4/.github/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 08:23:58.614097 erlab-1.6.4/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 root         (0) root         (0)      469 2024-04-03 08:23:52.000000 erlab-1.6.4/.github/ISSUE_TEMPLATE/bug-report.md
+-rw-r--r--   0 root         (0) root         (0)      608 2024-04-03 08:23:52.000000 erlab-1.6.4/.github/ISSUE_TEMPLATE/feature_request.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 08:23:58.618097 erlab-1.6.4/.github/workflows/
+-rw-r--r--   0 root         (0) root         (0)     1047 2024-04-03 08:23:52.000000 erlab-1.6.4/.github/workflows/pr.yml
+-rw-r--r--   0 root         (0) root         (0)     1893 2024-04-03 08:23:52.000000 erlab-1.6.4/.github/workflows/release.yml
+-rw-r--r--   0 root         (0) root         (0)     2898 2024-04-03 08:23:52.000000 erlab-1.6.4/.gitignore
+-rw-r--r--   0 root         (0) root         (0)      893 2024-04-03 08:23:52.000000 erlab-1.6.4/.pre-commit-config.yaml
+-rw-r--r--   0 root         (0) root         (0)      796 2024-04-03 08:23:52.000000 erlab-1.6.4/.readthedocs.yaml
+-rw-r--r--   0 root         (0) root         (0)    97096 2024-04-03 08:23:55.000000 erlab-1.6.4/CHANGELOG.md
+-rw-r--r--   0 root         (0) root         (0)    35149 2024-04-03 08:23:52.000000 erlab-1.6.4/LICENSE
+-rw-r--r--   0 root         (0) root         (0)    46708 2024-04-03 08:23:58.650098 erlab-1.6.4/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1473 2024-04-03 08:23:52.000000 erlab-1.6.4/PythonInterface.ipf
+-rw-r--r--   0 root         (0) root         (0)     4414 2024-04-03 08:23:52.000000 erlab-1.6.4/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 08:23:58.618097 erlab-1.6.4/docs/
+-rw-r--r--   0 root         (0) root         (0)      638 2024-04-03 08:23:52.000000 erlab-1.6.4/docs/Makefile
+-rw-r--r--   0 root         (0) root         (0)      752 2024-04-03 08:23:52.000000 erlab-1.6.4/docs/environment.yml
+-rw-r--r--   0 root         (0) root         (0)      804 2024-04-03 08:23:52.000000 erlab-1.6.4/docs/make.bat
+-rw-r--r--   0 root         (0) root         (0)      540 2024-04-03 08:23:52.000000 erlab-1.6.4/docs/requirements.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 08:23:58.622097 erlab-1.6.4/docs/source/
+-rw-r--r--   0 root         (0) root         (0)       52 2024-04-03 08:23:52.000000 erlab-1.6.4/docs/source/bibliography.rst
+-rw-r--r--   0 root         (0) root         (0)    10762 2024-04-03 08:23:52.000000 erlab-1.6.4/docs/source/conf.py
+-rw-r--r--   0 root         (0) root         (0)    13410 2024-04-03 08:23:52.000000 erlab-1.6.4/docs/source/development.rst
+-rw-r--r--   0 root         (0) root         (0)      265 2024-04-03 08:23:52.000000 erlab-1.6.4/docs/source/erlab.accessors.rst
+-rw-r--r--   0 root         (0) root         (0)      101 2024-04-03 08:23:52.000000 erlab-1.6.4/docs/source/erlab.analysis.rst
+-rw-r--r--   0 root         (0) root         (0)      141 2024-04-03 08:23:52.000000 erlab-1.6.4/docs/source/erlab.characterization.rst
+-rw-r--r--   0 root         (0) root         (0)      485 2024-04-03 08:23:52.000000 erlab-1.6.4/docs/source/erlab.constants.rst
+-rw-r--r--   0 root         (0) root         (0)      116 2024-04-03 08:23:52.000000 erlab-1.6.4/docs/source/erlab.interactive.rst
+-rw-r--r--   0 root         (0) root         (0)       81 2024-04-03 08:23:52.000000 erlab-1.6.4/docs/source/erlab.io.rst
+-rw-r--r--   0 root         (0) root         (0)      236 2024-04-03 08:23:52.000000 erlab-1.6.4/docs/source/erlab.lattice.rst
+-rw-r--r--   0 root         (0) root         (0)      242 2024-04-03 08:23:52.000000 erlab-1.6.4/docs/source/erlab.parallel.rst
+-rw-r--r--   0 root         (0) root         (0)      174 2024-04-03 08:23:52.000000 erlab-1.6.4/docs/source/erlab.plotting.rst
+-rw-r--r--   0 root         (0) root         (0)     2888 2024-04-03 08:23:52.000000 erlab-1.6.4/docs/source/getting-started.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 08:23:58.626097 erlab-1.6.4/docs/source/images/
+-rw-r--r--   0 root         (0) root         (0)   996803 2024-04-03 08:23:53.000000 erlab-1.6.4/docs/source/images/imagetool_dark.png
+-rw-r--r--   0 root         (0) root         (0)   966547 2024-04-03 08:23:53.000000 erlab-1.6.4/docs/source/images/imagetool_light.png
+-rw-r--r--   0 root         (0) root         (0)   709231 2024-04-03 08:23:53.000000 erlab-1.6.4/docs/source/images/ktool_1_dark.png
+-rw-r--r--   0 root         (0) root         (0)   694078 2024-04-03 08:23:53.000000 erlab-1.6.4/docs/source/images/ktool_1_light.png
+-rw-r--r--   0 root         (0) root         (0)   703343 2024-04-03 08:23:53.000000 erlab-1.6.4/docs/source/images/ktool_2_dark.png
+-rw-r--r--   0 root         (0) root         (0)   686688 2024-04-03 08:23:53.000000 erlab-1.6.4/docs/source/images/ktool_2_light.png
+-rw-r--r--   0 root         (0) root         (0)     2497 2024-04-03 08:23:53.000000 erlab-1.6.4/docs/source/index.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 08:23:58.630097 erlab-1.6.4/docs/source/notebooks/
+-rw-r--r--   0 root         (0) root         (0)   189769 2024-04-03 08:23:53.000000 erlab-1.6.4/docs/source/notebooks/indexing.ipynb
+-rw-r--r--   0 root         (0) root         (0)     1582 2024-04-03 08:23:53.000000 erlab-1.6.4/docs/source/notebooks/io.ipynb
+-rw-r--r--   0 root         (0) root         (0)   379528 2024-04-03 08:23:53.000000 erlab-1.6.4/docs/source/notebooks/kconv.ipynb
+-rw-r--r--   0 root         (0) root         (0)    15761 2024-04-03 08:23:53.000000 erlab-1.6.4/docs/source/notebooks/plotting.ipynb
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 08:23:58.630097 erlab-1.6.4/docs/source/pyplots/
+-rw-r--r--   0 root         (0) root         (0)     2579 2024-04-03 08:23:53.000000 erlab-1.6.4/docs/source/pyplots/norms.py
+-rw-r--r--   0 root         (0) root         (0)     1344 2024-04-03 08:23:53.000000 erlab-1.6.4/docs/source/reference.rst
+-rw-r--r--   0 root         (0) root         (0)     1316 2024-04-03 08:23:53.000000 erlab-1.6.4/docs/source/refs.bib
+-rw-r--r--   0 root         (0) root         (0)     1142 2024-04-03 08:23:53.000000 erlab-1.6.4/docs/source/userguide.rst
+-rw-r--r--   0 root         (0) root         (0)      880 2024-04-03 08:23:53.000000 erlab-1.6.4/environment.yml
+-rw-r--r--   0 root         (0) root         (0)      990 2024-04-03 08:23:53.000000 erlab-1.6.4/environment_apple.yml
+-rw-r--r--   0 root         (0) root         (0)      876 2024-04-03 08:23:53.000000 erlab-1.6.4/environment_nogit.yml
+-rw-r--r--   0 root         (0) root         (0)      848 2024-04-03 08:23:53.000000 erlab-1.6.4/environment_nogit_mkl.yml
+-rw-r--r--   0 root         (0) root         (0)     4227 2024-04-03 08:23:53.000000 erlab-1.6.4/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)      334 2024-04-03 08:23:53.000000 erlab-1.6.4/requirements.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-03 08:23:58.650098 erlab-1.6.4/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 08:23:58.610097 erlab-1.6.4/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 08:23:58.630097 erlab-1.6.4/src/erlab/
+-rw-r--r--   0 root         (0) root         (0)       60 2024-04-03 08:23:55.000000 erlab-1.6.4/src/erlab/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    35539 2024-04-03 08:23:53.000000 erlab-1.6.4/src/erlab/accessors.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 08:23:58.634097 erlab-1.6.4/src/erlab/analysis/
+-rw-r--r--   0 root         (0) root         (0)      748 2024-04-03 08:23:53.000000 erlab-1.6.4/src/erlab/analysis/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5514 2024-04-03 08:23:53.000000 erlab-1.6.4/src/erlab/analysis/correlation.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 08:23:58.634097 erlab-1.6.4/src/erlab/analysis/fit/
+-rw-r--r--   0 root         (0) root         (0)      459 2024-04-03 08:23:53.000000 erlab-1.6.4/src/erlab/analysis/fit/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 08:23:58.634097 erlab-1.6.4/src/erlab/analysis/fit/functions/
+-rw-r--r--   0 root         (0) root         (0)      812 2024-04-03 08:23:53.000000 erlab-1.6.4/src/erlab/analysis/fit/functions/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8766 2024-04-03 08:23:53.000000 erlab-1.6.4/src/erlab/analysis/fit/functions/dynamic.py
+-rw-r--r--   0 root         (0) root         (0)     6026 2024-04-03 08:23:53.000000 erlab-1.6.4/src/erlab/analysis/fit/functions/general.py
+-rw-r--r--   0 root         (0) root         (0)     6165 2024-04-03 08:23:53.000000 erlab-1.6.4/src/erlab/analysis/fit/minuit.py
+-rw-r--r--   0 root         (0) root         (0)    10572 2024-04-03 08:23:53.000000 erlab-1.6.4/src/erlab/analysis/fit/models.py
+-rw-r--r--   0 root         (0) root         (0)     1168 2024-04-03 08:23:53.000000 erlab-1.6.4/src/erlab/analysis/fit/spline.py
+-rw-r--r--   0 root         (0) root         (0)    13815 2024-04-03 08:23:53.000000 erlab-1.6.4/src/erlab/analysis/gold.py
+-rw-r--r--   0 root         (0) root         (0)     9811 2024-04-03 08:23:53.000000 erlab-1.6.4/src/erlab/analysis/interpolate.py
+-rw-r--r--   0 root         (0) root         (0)    10344 2024-04-03 08:23:53.000000 erlab-1.6.4/src/erlab/analysis/kspace.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 08:23:58.634097 erlab-1.6.4/src/erlab/analysis/mask/
+-rw-r--r--   0 root         (0) root         (0)     2768 2024-04-03 08:23:53.000000 erlab-1.6.4/src/erlab/analysis/mask/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7810 2024-04-03 08:23:53.000000 erlab-1.6.4/src/erlab/analysis/mask/polygon.py
+-rw-r--r--   0 root         (0) root         (0)      878 2024-04-03 08:23:53.000000 erlab-1.6.4/src/erlab/analysis/transform.py
+-rw-r--r--   0 root         (0) root         (0)     8332 2024-04-03 08:23:53.000000 erlab-1.6.4/src/erlab/analysis/utilities.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 08:23:58.634097 erlab-1.6.4/src/erlab/characterization/
+-rw-r--r--   0 root         (0) root         (0)      191 2024-04-03 08:23:53.000000 erlab-1.6.4/src/erlab/characterization/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3093 2024-04-03 08:23:53.000000 erlab-1.6.4/src/erlab/characterization/resistance.py
+-rw-r--r--   0 root         (0) root         (0)     1903 2024-04-03 08:23:53.000000 erlab-1.6.4/src/erlab/characterization/xrd.py
+-rw-r--r--   0 root         (0) root         (0)     2115 2024-04-03 08:23:53.000000 erlab-1.6.4/src/erlab/constants.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 08:23:58.638097 erlab-1.6.4/src/erlab/interactive/
+-rw-r--r--   0 root         (0) root         (0)      540 2024-04-03 08:23:53.000000 erlab-1.6.4/src/erlab/interactive/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    13943 2024-04-03 08:23:53.000000 erlab-1.6.4/src/erlab/interactive/bzplot.py
+-rw-r--r--   0 root         (0) root         (0)    20820 2024-04-03 08:23:53.000000 erlab-1.6.4/src/erlab/interactive/colors.py
+-rw-r--r--   0 root         (0) root         (0)    22076 2024-04-03 08:23:53.000000 erlab-1.6.4/src/erlab/interactive/curvefittingtool.py
+-rw-r--r--   0 root         (0) root         (0)    19528 2024-04-03 08:23:53.000000 erlab-1.6.4/src/erlab/interactive/derivative.py
+-rw-r--r--   0 root         (0) root         (0)     9458 2024-04-03 08:23:53.000000 erlab-1.6.4/src/erlab/interactive/exampledata.py
+-rw-r--r--   0 root         (0) root         (0)    19072 2024-04-03 08:23:53.000000 erlab-1.6.4/src/erlab/interactive/fermiedge.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 08:23:58.638097 erlab-1.6.4/src/erlab/interactive/imagetool/
+-rw-r--r--   0 root         (0) root         (0)    19391 2024-04-03 08:23:53.000000 erlab-1.6.4/src/erlab/interactive/imagetool/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 08:23:58.638097 erlab-1.6.4/src/erlab/interactive/imagetool/_deprecated/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-03 08:23:53.000000 erlab-1.6.4/src/erlab/interactive/imagetool/_deprecated/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    52076 2024-04-03 08:23:53.000000 erlab-1.6.4/src/erlab/interactive/imagetool/_deprecated/imagetool_mpl.py
+-rw-r--r--   0 root         (0) root         (0)   114751 2024-04-03 08:23:53.000000 erlab-1.6.4/src/erlab/interactive/imagetool/_deprecated/imagetool_old.py
+-rw-r--r--   0 root         (0) root         (0)    27081 2024-04-03 08:23:53.000000 erlab-1.6.4/src/erlab/interactive/imagetool/controls.py
+-rw-r--r--   0 root         (0) root         (0)    53776 2024-04-03 08:23:53.000000 erlab-1.6.4/src/erlab/interactive/imagetool/core.py
+-rw-r--r--   0 root         (0) root         (0)    11483 2024-04-03 08:23:53.000000 erlab-1.6.4/src/erlab/interactive/imagetool/fastbinning.py
+-rw-r--r--   0 root         (0) root         (0)    23195 2024-04-03 08:23:53.000000 erlab-1.6.4/src/erlab/interactive/imagetool/slicer.py
+-rw-r--r--   0 root         (0) root         (0)    16658 2024-04-03 08:23:53.000000 erlab-1.6.4/src/erlab/interactive/kspace.py
+-rw-r--r--   0 root         (0) root         (0)    19382 2024-04-03 08:23:53.000000 erlab-1.6.4/src/erlab/interactive/ktool.ui
+-rw-r--r--   0 root         (0) root         (0)     3341 2024-04-03 08:23:53.000000 erlab-1.6.4/src/erlab/interactive/masktool.py
+-rw-r--r--   0 root         (0) root         (0)    52417 2024-04-03 08:23:53.000000 erlab-1.6.4/src/erlab/interactive/utilities.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 08:23:58.642098 erlab-1.6.4/src/erlab/io/
+-rw-r--r--   0 root         (0) root         (0)     1937 2024-04-03 08:23:53.000000 erlab-1.6.4/src/erlab/io/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    30047 2024-04-03 08:23:53.000000 erlab-1.6.4/src/erlab/io/dataloader.py
+-rw-r--r--   0 root         (0) root         (0)     8084 2024-04-03 08:23:53.000000 erlab-1.6.4/src/erlab/io/igor.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 08:23:58.642098 erlab-1.6.4/src/erlab/io/plugins/
+-rw-r--r--   0 root         (0) root         (0)      900 2024-04-03 08:23:53.000000 erlab-1.6.4/src/erlab/io/plugins/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3674 2024-04-03 08:23:53.000000 erlab-1.6.4/src/erlab/io/plugins/da30.py
+-rw-r--r--   0 root         (0) root         (0)     1185 2024-04-03 08:23:53.000000 erlab-1.6.4/src/erlab/io/plugins/kriss.py
+-rw-r--r--   0 root         (0) root         (0)     7448 2024-04-03 08:23:53.000000 erlab-1.6.4/src/erlab/io/plugins/merlin.py
+-rw-r--r--   0 root         (0) root         (0)     7745 2024-04-03 08:23:53.000000 erlab-1.6.4/src/erlab/io/plugins/ssrl52.py
+-rw-r--r--   0 root         (0) root         (0)     5630 2024-04-03 08:23:53.000000 erlab-1.6.4/src/erlab/io/utilities.py
+-rw-r--r--   0 root         (0) root         (0)     2515 2024-04-03 08:23:53.000000 erlab-1.6.4/src/erlab/lattice.py
+-rw-r--r--   0 root         (0) root         (0)     2242 2024-04-03 08:23:53.000000 erlab-1.6.4/src/erlab/parallel.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 08:23:58.642098 erlab-1.6.4/src/erlab/plotting/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 08:23:58.646098 erlab-1.6.4/src/erlab/plotting/IgorCT/
+-rw-r--r--   0 root         (0) root         (0)     3379 2024-04-03 08:23:53.000000 erlab-1.6.4/src/erlab/plotting/IgorCT/Blue-White.txt
+-rw-r--r--   0 root         (0) root         (0)     3456 2024-04-03 08:23:53.000000 erlab-1.6.4/src/erlab/plotting/IgorCT/BlueHot.ibw
+-rw-r--r--   0 root         (0) root         (0)     3526 2024-04-03 08:23:53.000000 erlab-1.6.4/src/erlab/plotting/IgorCT/CTBlueWhite.ibw
+-rw-r--r--   0 root         (0) root         (0)     3530 2024-04-03 08:23:53.000000 erlab-1.6.4/src/erlab/plotting/IgorCT/CTRainbowLIght.ibw
+-rw-r--r--   0 root         (0) root         (0)     3531 2024-04-03 08:23:53.000000 erlab-1.6.4/src/erlab/plotting/IgorCT/CTRedTemperature.ibw
+-rw-r--r--   0 root         (0) root         (0)     3456 2024-04-03 08:23:53.000000 erlab-1.6.4/src/erlab/plotting/IgorCT/ColdWarm.ibw
+-rw-r--r--   0 root         (0) root         (0)     3456 2024-04-03 08:23:53.000000 erlab-1.6.4/src/erlab/plotting/IgorCT/PlanetEarth.ibw
+-rw-r--r--   0 root         (0) root         (0)     1920 2024-04-03 08:23:53.000000 erlab-1.6.4/src/erlab/plotting/IgorCT/ametrine.ibw
+-rw-r--r--   0 root         (0) root         (0)     2048 2024-04-03 08:23:53.000000 erlab-1.6.4/src/erlab/plotting/IgorCT/isolum.ibw
+-rw-r--r--   0 root         (0) root         (0)     2048 2024-04-03 08:23:53.000000 erlab-1.6.4/src/erlab/plotting/IgorCT/morgenstemning.ibw
+-rw-r--r--   0 root         (0) root         (0)     1857 2024-04-03 08:23:53.000000 erlab-1.6.4/src/erlab/plotting/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    29010 2024-04-03 08:23:53.000000 erlab-1.6.4/src/erlab/plotting/annotations.py
+-rw-r--r--   0 root         (0) root         (0)    18275 2024-04-03 08:23:53.000000 erlab-1.6.4/src/erlab/plotting/atoms.py
+-rw-r--r--   0 root         (0) root         (0)     4294 2024-04-03 08:23:53.000000 erlab-1.6.4/src/erlab/plotting/bz.py
+-rw-r--r--   0 root         (0) root         (0)    32411 2024-04-03 08:23:53.000000 erlab-1.6.4/src/erlab/plotting/colors.py
+-rw-r--r--   0 root         (0) root         (0)     2657 2024-04-03 08:23:53.000000 erlab-1.6.4/src/erlab/plotting/erplot.py
+-rw-r--r--   0 root         (0) root         (0)    30998 2024-04-03 08:23:53.000000 erlab-1.6.4/src/erlab/plotting/general.py
+-rw-r--r--   0 root         (0) root         (0)     2726 2024-04-03 08:23:53.000000 erlab-1.6.4/src/erlab/plotting/plot3d.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 08:23:58.646098 erlab-1.6.4/src/erlab/plotting/stylelib/
+-rw-r--r--   0 root         (0) root         (0)     6839 2024-04-03 08:23:53.000000 erlab-1.6.4/src/erlab/plotting/stylelib/fira.mplstyle
+-rw-r--r--   0 root         (0) root         (0)     6826 2024-04-03 08:23:53.000000 erlab-1.6.4/src/erlab/plotting/stylelib/firalight.mplstyle
+-rw-r--r--   0 root         (0) root         (0)    14358 2024-04-03 08:23:53.000000 erlab-1.6.4/src/erlab/plotting/stylelib/khan.mplstyle
+-rw-r--r--   0 root         (0) root         (0)     9160 2024-04-03 08:23:53.000000 erlab-1.6.4/src/erlab/plotting/stylelib/nature.mplstyle
+-rw-r--r--   0 root         (0) root         (0)      630 2024-04-03 08:23:53.000000 erlab-1.6.4/src/erlab/plotting/stylelib/poster.mplstyle
+-rw-r--r--   0 root         (0) root         (0)     7023 2024-04-03 08:23:53.000000 erlab-1.6.4/src/erlab/plotting/stylelib/times.mplstyle
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 08:23:58.646098 erlab-1.6.4/src/erlab.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    46708 2024-04-03 08:23:58.000000 erlab-1.6.4/src/erlab.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     4265 2024-04-03 08:23:58.000000 erlab-1.6.4/src/erlab.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-03 08:23:58.000000 erlab-1.6.4/src/erlab.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      321 2024-04-03 08:23:58.000000 erlab-1.6.4/src/erlab.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        6 2024-04-03 08:23:58.000000 erlab-1.6.4/src/erlab.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 08:23:58.646098 erlab-1.6.4/tests/
+-rw-r--r--   0 root         (0) root         (0)      595 2024-04-03 08:23:53.000000 erlab-1.6.4/tests/test_fastbinning.py
+-rw-r--r--   0 root         (0) root         (0)      598 2024-04-03 08:23:53.000000 erlab-1.6.4/tests/test_interpolate.py
+-rw-r--r--   0 root         (0) root         (0)     2419 2024-04-03 08:23:53.000000 erlab-1.6.4/tests/test_kspace.py
```

### Comparing `erlab-1.6.3/.github/ISSUE_TEMPLATE/feature_request.md` & `erlab-1.6.4/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `erlab-1.6.3/.github/workflows/pr.yml` & `erlab-1.6.4/.github/workflows/pr.yml`

 * *Files identical despite different names*

### Comparing `erlab-1.6.3/.github/workflows/release.yml` & `erlab-1.6.4/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `erlab-1.6.3/.gitignore` & `erlab-1.6.4/.gitignore`

 * *Files identical despite different names*

### Comparing `erlab-1.6.3/.pre-commit-config.yaml` & `erlab-1.6.4/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `erlab-1.6.3/.readthedocs.yaml` & `erlab-1.6.4/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `erlab-1.6.3/CHANGELOG.md` & `erlab-1.6.4/CHANGELOG.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,18 @@
 # CHANGELOG
 
 
 
+## v1.6.4 (2024-04-03)
+
+### Fix
+
+* fix: load colormaps only when igor2 is  available ([`7927c7d`](https://github.com/kmnhan/erlabpy/commit/7927c7db264bedb1a27b980d820d352f779b64c9))
+
+
 ## v1.6.3 (2024-04-03)
 
 ### Fix
 
 * fix: leave out type annotation for passing tests ([`eb25008`](https://github.com/kmnhan/erlabpy/commit/eb2500838820172529ee751b5d8a624c950f66d2))
```

### Comparing `erlab-1.6.3/LICENSE` & `erlab-1.6.4/LICENSE`

 * *Files identical despite different names*

### Comparing `erlab-1.6.3/PKG-INFO` & `erlab-1.6.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: erlab
-Version: 1.6.3
+Version: 1.6.4
 Summary: Python package for ARPES data analysis and visualization.
 Author-email: Kimoon Han <khan@kaist.ac.kr>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `erlab-1.6.3/PythonInterface.ipf` & `erlab-1.6.4/PythonInterface.ipf`

 * *Files identical despite different names*

### Comparing `erlab-1.6.3/README.md` & `erlab-1.6.4/README.md`

 * *Files identical despite different names*

### Comparing `erlab-1.6.3/docs/Makefile` & `erlab-1.6.4/docs/Makefile`

 * *Files identical despite different names*

### Comparing `erlab-1.6.3/docs/environment.yml` & `erlab-1.6.4/docs/environment.yml`

 * *Files identical despite different names*

### Comparing `erlab-1.6.3/docs/make.bat` & `erlab-1.6.4/docs/make.bat`

 * *Files identical despite different names*

### Comparing `erlab-1.6.3/docs/requirements.txt` & `erlab-1.6.4/docs/requirements.txt`

 * *Files identical despite different names*

### Comparing `erlab-1.6.3/docs/source/conf.py` & `erlab-1.6.4/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `erlab-1.6.3/docs/source/development.rst` & `erlab-1.6.4/docs/source/development.rst`

 * *Files identical despite different names*

### Comparing `erlab-1.6.3/docs/source/getting-started.rst` & `erlab-1.6.4/docs/source/getting-started.rst`

 * *Files identical despite different names*

### Comparing `erlab-1.6.3/docs/source/images/imagetool_dark.png` & `erlab-1.6.4/docs/source/images/imagetool_dark.png`

 * *Files identical despite different names*

### Comparing `erlab-1.6.3/docs/source/images/imagetool_light.png` & `erlab-1.6.4/docs/source/images/imagetool_light.png`

 * *Files identical despite different names*

### Comparing `erlab-1.6.3/docs/source/images/ktool_1_dark.png` & `erlab-1.6.4/docs/source/images/ktool_1_dark.png`

 * *Files identical despite different names*

### Comparing `erlab-1.6.3/docs/source/images/ktool_1_light.png` & `erlab-1.6.4/docs/source/images/ktool_1_light.png`

 * *Files identical despite different names*

### Comparing `erlab-1.6.3/docs/source/images/ktool_2_dark.png` & `erlab-1.6.4/docs/source/images/ktool_2_dark.png`

 * *Files identical despite different names*

### Comparing `erlab-1.6.3/docs/source/images/ktool_2_light.png` & `erlab-1.6.4/docs/source/images/ktool_2_light.png`

 * *Files identical despite different names*

### Comparing `erlab-1.6.3/docs/source/index.rst` & `erlab-1.6.4/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `erlab-1.6.3/docs/source/notebooks/indexing.ipynb` & `erlab-1.6.4/docs/source/notebooks/indexing.ipynb`

 * *Files identical despite different names*

### Comparing `erlab-1.6.3/docs/source/notebooks/io.ipynb` & `erlab-1.6.4/docs/source/notebooks/io.ipynb`

 * *Files identical despite different names*

### Comparing `erlab-1.6.3/docs/source/notebooks/kconv.ipynb` & `erlab-1.6.4/docs/source/notebooks/kconv.ipynb`

 * *Files identical despite different names*

### Comparing `erlab-1.6.3/docs/source/notebooks/plotting.ipynb` & `erlab-1.6.4/docs/source/notebooks/plotting.ipynb`

 * *Files identical despite different names*

### Comparing `erlab-1.6.3/docs/source/pyplots/norms.py` & `erlab-1.6.4/docs/source/pyplots/norms.py`

 * *Files identical despite different names*

### Comparing `erlab-1.6.3/docs/source/reference.rst` & `erlab-1.6.4/docs/source/reference.rst`

 * *Files identical despite different names*

### Comparing `erlab-1.6.3/docs/source/refs.bib` & `erlab-1.6.4/docs/source/refs.bib`

 * *Files identical despite different names*

### Comparing `erlab-1.6.3/docs/source/userguide.rst` & `erlab-1.6.4/docs/source/userguide.rst`

 * *Files identical despite different names*

### Comparing `erlab-1.6.3/environment.yml` & `erlab-1.6.4/environment.yml`

 * *Files identical despite different names*

### Comparing `erlab-1.6.3/environment_apple.yml` & `erlab-1.6.4/environment_apple.yml`

 * *Files identical despite different names*

### Comparing `erlab-1.6.3/environment_nogit.yml` & `erlab-1.6.4/environment_nogit.yml`

 * *Files identical despite different names*

### Comparing `erlab-1.6.3/environment_nogit_mkl.yml` & `erlab-1.6.4/environment_nogit_mkl.yml`

 * *Files identical despite different names*

### Comparing `erlab-1.6.3/pyproject.toml` & `erlab-1.6.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `erlab-1.6.3/src/erlab/accessors.py` & `erlab-1.6.4/src/erlab/accessors.py`

 * *Files identical despite different names*

### Comparing `erlab-1.6.3/src/erlab/analysis/__init__.py` & `erlab-1.6.4/src/erlab/analysis/__init__.py`

 * *Files identical despite different names*

### Comparing `erlab-1.6.3/src/erlab/analysis/correlation.py` & `erlab-1.6.4/src/erlab/analysis/correlation.py`

 * *Files identical despite different names*

### Comparing `erlab-1.6.3/src/erlab/analysis/fit/functions/__init__.py` & `erlab-1.6.4/src/erlab/analysis/fit/functions/__init__.py`

 * *Files identical despite different names*

### Comparing `erlab-1.6.3/src/erlab/analysis/fit/functions/dynamic.py` & `erlab-1.6.4/src/erlab/analysis/fit/functions/dynamic.py`

 * *Files identical despite different names*

### Comparing `erlab-1.6.3/src/erlab/analysis/fit/functions/general.py` & `erlab-1.6.4/src/erlab/analysis/fit/functions/general.py`

 * *Files identical despite different names*

### Comparing `erlab-1.6.3/src/erlab/analysis/fit/minuit.py` & `erlab-1.6.4/src/erlab/analysis/fit/minuit.py`

 * *Files identical despite different names*

### Comparing `erlab-1.6.3/src/erlab/analysis/fit/models.py` & `erlab-1.6.4/src/erlab/analysis/fit/models.py`

 * *Files identical despite different names*

### Comparing `erlab-1.6.3/src/erlab/analysis/fit/spline.py` & `erlab-1.6.4/src/erlab/analysis/fit/spline.py`

 * *Files identical despite different names*

### Comparing `erlab-1.6.3/src/erlab/analysis/gold.py` & `erlab-1.6.4/src/erlab/analysis/gold.py`

 * *Files identical despite different names*

### Comparing `erlab-1.6.3/src/erlab/analysis/interpolate.py` & `erlab-1.6.4/src/erlab/analysis/interpolate.py`

 * *Files identical despite different names*

### Comparing `erlab-1.6.3/src/erlab/analysis/kspace.py` & `erlab-1.6.4/src/erlab/analysis/kspace.py`

 * *Files identical despite different names*

### Comparing `erlab-1.6.3/src/erlab/analysis/mask/__init__.py` & `erlab-1.6.4/src/erlab/analysis/mask/__init__.py`

 * *Files identical despite different names*

### Comparing `erlab-1.6.3/src/erlab/analysis/mask/polygon.py` & `erlab-1.6.4/src/erlab/analysis/mask/polygon.py`

 * *Files identical despite different names*

### Comparing `erlab-1.6.3/src/erlab/analysis/transform.py` & `erlab-1.6.4/src/erlab/analysis/transform.py`

 * *Files identical despite different names*

### Comparing `erlab-1.6.3/src/erlab/analysis/utilities.py` & `erlab-1.6.4/src/erlab/analysis/utilities.py`

 * *Files identical despite different names*

### Comparing `erlab-1.6.3/src/erlab/characterization/resistance.py` & `erlab-1.6.4/src/erlab/characterization/resistance.py`

 * *Files identical despite different names*

### Comparing `erlab-1.6.3/src/erlab/characterization/xrd.py` & `erlab-1.6.4/src/erlab/characterization/xrd.py`

 * *Files identical despite different names*

### Comparing `erlab-1.6.3/src/erlab/constants.py` & `erlab-1.6.4/src/erlab/constants.py`

 * *Files identical despite different names*

### Comparing `erlab-1.6.3/src/erlab/interactive/__init__.py` & `erlab-1.6.4/src/erlab/interactive/__init__.py`

 * *Files identical despite different names*

### Comparing `erlab-1.6.3/src/erlab/interactive/bzplot.py` & `erlab-1.6.4/src/erlab/interactive/bzplot.py`

 * *Files identical despite different names*

### Comparing `erlab-1.6.3/src/erlab/interactive/colors.py` & `erlab-1.6.4/src/erlab/interactive/colors.py`

 * *Files identical despite different names*

### Comparing `erlab-1.6.3/src/erlab/interactive/curvefittingtool.py` & `erlab-1.6.4/src/erlab/interactive/curvefittingtool.py`

 * *Files identical despite different names*

### Comparing `erlab-1.6.3/src/erlab/interactive/derivative.py` & `erlab-1.6.4/src/erlab/interactive/derivative.py`

 * *Files identical despite different names*

### Comparing `erlab-1.6.3/src/erlab/interactive/exampledata.py` & `erlab-1.6.4/src/erlab/interactive/exampledata.py`

 * *Files identical despite different names*

### Comparing `erlab-1.6.3/src/erlab/interactive/fermiedge.py` & `erlab-1.6.4/src/erlab/interactive/fermiedge.py`

 * *Files identical despite different names*

### Comparing `erlab-1.6.3/src/erlab/interactive/imagetool/__init__.py` & `erlab-1.6.4/src/erlab/interactive/imagetool/__init__.py`

 * *Files identical despite different names*

### Comparing `erlab-1.6.3/src/erlab/interactive/imagetool/_deprecated/imagetool_mpl.py` & `erlab-1.6.4/src/erlab/interactive/imagetool/_deprecated/imagetool_mpl.py`

 * *Files identical despite different names*

### Comparing `erlab-1.6.3/src/erlab/interactive/imagetool/_deprecated/imagetool_old.py` & `erlab-1.6.4/src/erlab/interactive/imagetool/_deprecated/imagetool_old.py`

 * *Files identical despite different names*

### Comparing `erlab-1.6.3/src/erlab/interactive/imagetool/controls.py` & `erlab-1.6.4/src/erlab/interactive/imagetool/controls.py`

 * *Files identical despite different names*

### Comparing `erlab-1.6.3/src/erlab/interactive/imagetool/core.py` & `erlab-1.6.4/src/erlab/interactive/imagetool/core.py`

 * *Files identical despite different names*

### Comparing `erlab-1.6.3/src/erlab/interactive/imagetool/fastbinning.py` & `erlab-1.6.4/src/erlab/interactive/imagetool/fastbinning.py`

 * *Files identical despite different names*

### Comparing `erlab-1.6.3/src/erlab/interactive/imagetool/slicer.py` & `erlab-1.6.4/src/erlab/interactive/imagetool/slicer.py`

 * *Files identical despite different names*

### Comparing `erlab-1.6.3/src/erlab/interactive/kspace.py` & `erlab-1.6.4/src/erlab/interactive/kspace.py`

 * *Files identical despite different names*

### Comparing `erlab-1.6.3/src/erlab/interactive/ktool.ui` & `erlab-1.6.4/src/erlab/interactive/ktool.ui`

 * *Files identical despite different names*

### Comparing `erlab-1.6.3/src/erlab/interactive/masktool.py` & `erlab-1.6.4/src/erlab/interactive/masktool.py`

 * *Files identical despite different names*

### Comparing `erlab-1.6.3/src/erlab/interactive/utilities.py` & `erlab-1.6.4/src/erlab/interactive/utilities.py`

 * *Files identical despite different names*

### Comparing `erlab-1.6.3/src/erlab/io/__init__.py` & `erlab-1.6.4/src/erlab/io/__init__.py`

 * *Files identical despite different names*

### Comparing `erlab-1.6.3/src/erlab/io/dataloader.py` & `erlab-1.6.4/src/erlab/io/dataloader.py`

 * *Files identical despite different names*

### Comparing `erlab-1.6.3/src/erlab/io/igor.py` & `erlab-1.6.4/src/erlab/io/igor.py`

 * *Files identical despite different names*

### Comparing `erlab-1.6.3/src/erlab/io/plugins/__init__.py` & `erlab-1.6.4/src/erlab/io/plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `erlab-1.6.3/src/erlab/io/plugins/da30.py` & `erlab-1.6.4/src/erlab/io/plugins/da30.py`

 * *Files identical despite different names*

### Comparing `erlab-1.6.3/src/erlab/io/plugins/kriss.py` & `erlab-1.6.4/src/erlab/io/plugins/kriss.py`

 * *Files identical despite different names*

### Comparing `erlab-1.6.3/src/erlab/io/plugins/merlin.py` & `erlab-1.6.4/src/erlab/io/plugins/merlin.py`

 * *Files identical despite different names*

### Comparing `erlab-1.6.3/src/erlab/io/plugins/ssrl52.py` & `erlab-1.6.4/src/erlab/io/plugins/ssrl52.py`

 * *Files identical despite different names*

### Comparing `erlab-1.6.3/src/erlab/io/utilities.py` & `erlab-1.6.4/src/erlab/io/utilities.py`

 * *Files identical despite different names*

### Comparing `erlab-1.6.3/src/erlab/lattice.py` & `erlab-1.6.4/src/erlab/lattice.py`

 * *Files identical despite different names*

### Comparing `erlab-1.6.3/src/erlab/parallel.py` & `erlab-1.6.4/src/erlab/parallel.py`

 * *Files identical despite different names*

### Comparing `erlab-1.6.3/src/erlab/plotting/IgorCT/Blue-White.txt` & `erlab-1.6.4/src/erlab/plotting/IgorCT/Blue-White.txt`

 * *Files identical despite different names*

### Comparing `erlab-1.6.3/src/erlab/plotting/IgorCT/BlueHot.ibw` & `erlab-1.6.4/src/erlab/plotting/IgorCT/BlueHot.ibw`

 * *Files identical despite different names*

### Comparing `erlab-1.6.3/src/erlab/plotting/IgorCT/CTBlueWhite.ibw` & `erlab-1.6.4/src/erlab/plotting/IgorCT/CTBlueWhite.ibw`

 * *Files identical despite different names*

### Comparing `erlab-1.6.3/src/erlab/plotting/IgorCT/CTRainbowLIght.ibw` & `erlab-1.6.4/src/erlab/plotting/IgorCT/CTRainbowLIght.ibw`

 * *Files identical despite different names*

### Comparing `erlab-1.6.3/src/erlab/plotting/IgorCT/CTRedTemperature.ibw` & `erlab-1.6.4/src/erlab/plotting/IgorCT/CTRedTemperature.ibw`

 * *Files identical despite different names*

### Comparing `erlab-1.6.3/src/erlab/plotting/IgorCT/ColdWarm.ibw` & `erlab-1.6.4/src/erlab/plotting/IgorCT/ColdWarm.ibw`

 * *Files identical despite different names*

### Comparing `erlab-1.6.3/src/erlab/plotting/IgorCT/PlanetEarth.ibw` & `erlab-1.6.4/src/erlab/plotting/IgorCT/PlanetEarth.ibw`

 * *Files identical despite different names*

### Comparing `erlab-1.6.3/src/erlab/plotting/IgorCT/ametrine.ibw` & `erlab-1.6.4/src/erlab/plotting/IgorCT/ametrine.ibw`

 * *Files identical despite different names*

### Comparing `erlab-1.6.3/src/erlab/plotting/IgorCT/isolum.ibw` & `erlab-1.6.4/src/erlab/plotting/IgorCT/isolum.ibw`

 * *Files identical despite different names*

### Comparing `erlab-1.6.3/src/erlab/plotting/IgorCT/morgenstemning.ibw` & `erlab-1.6.4/src/erlab/plotting/IgorCT/morgenstemning.ibw`

 * *Files identical despite different names*

### Comparing `erlab-1.6.3/src/erlab/plotting/__init__.py` & `erlab-1.6.4/src/erlab/plotting/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -34,15 +34,14 @@
 import pkgutil
 
 import matplotlib
 import matplotlib.colors
 import matplotlib.font_manager
 import matplotlib.style
 import numpy as np
-
 import erlab.io
 
 # Import colormaps if available
 if importlib.util.find_spec("cmasher"):
     importlib.import_module("cmasher")
 if importlib.util.find_spec("cmocean"):
     importlib.import_module("cmocean")
@@ -58,22 +57,23 @@
         values = erlab.io.load_wave(io.BytesIO(file)).values
 
     cmap = matplotlib.colors.LinearSegmentedColormap.from_list(name, values / 65535)
     matplotlib.colormaps.register(cmap)
     matplotlib.colormaps.register(cmap.reversed())
 
 
-load_igor_ct("CTBlueWhite.ibw", "BuWh")
-load_igor_ct("CTRainbowLIght.ibw", "RainbowLight")
-# load_igor_ct("CTRedTemperature.ibw", "RedTemperature")
-load_igor_ct("ColdWarm.ibw", "ColdWarm")
-load_igor_ct("BlueHot.ibw", "BlueHot")
-# load_igor_ct("PlanetEarth.ibw", "PlanetEarth")
-# load_igor_ct("ametrine.ibw", "ametrine")
-# load_igor_ct("isolum.ibw", "isolum")
-# load_igor_ct("morgenstemning.ibw", "morgenstemning")
+if importlib.util.find_spec("igor2"):
+    load_igor_ct("CTBlueWhite.ibw", "BuWh")
+    load_igor_ct("CTRainbowLIght.ibw", "RainbowLight")
+    # load_igor_ct("CTRedTemperature.ibw", "RedTemperature")
+    load_igor_ct("ColdWarm.ibw", "ColdWarm")
+    load_igor_ct("BlueHot.ibw", "BlueHot")
+    # load_igor_ct("PlanetEarth.ibw", "PlanetEarth")
+    # load_igor_ct("ametrine.ibw", "ametrine")
+    # load_igor_ct("isolum.ibw", "isolum")
+    # load_igor_ct("morgenstemning.ibw", "morgenstemning")
 
 
 matplotlib.style.core.USER_LIBRARY_PATHS.append(
     os.path.join(os.path.dirname(__file__), "stylelib")
 )
 matplotlib.style.core.reload_library()
```

### Comparing `erlab-1.6.3/src/erlab/plotting/annotations.py` & `erlab-1.6.4/src/erlab/plotting/annotations.py`

 * *Files identical despite different names*

### Comparing `erlab-1.6.3/src/erlab/plotting/atoms.py` & `erlab-1.6.4/src/erlab/plotting/atoms.py`

 * *Files identical despite different names*

### Comparing `erlab-1.6.3/src/erlab/plotting/bz.py` & `erlab-1.6.4/src/erlab/plotting/bz.py`

 * *Files identical despite different names*

### Comparing `erlab-1.6.3/src/erlab/plotting/colors.py` & `erlab-1.6.4/src/erlab/plotting/colors.py`

 * *Files identical despite different names*

### Comparing `erlab-1.6.3/src/erlab/plotting/erplot.py` & `erlab-1.6.4/src/erlab/plotting/erplot.py`

 * *Files identical despite different names*

### Comparing `erlab-1.6.3/src/erlab/plotting/general.py` & `erlab-1.6.4/src/erlab/plotting/general.py`

 * *Files identical despite different names*

### Comparing `erlab-1.6.3/src/erlab/plotting/plot3d.py` & `erlab-1.6.4/src/erlab/plotting/plot3d.py`

 * *Files identical despite different names*

### Comparing `erlab-1.6.3/src/erlab/plotting/stylelib/fira.mplstyle` & `erlab-1.6.4/src/erlab/plotting/stylelib/fira.mplstyle`

 * *Files identical despite different names*

### Comparing `erlab-1.6.3/src/erlab/plotting/stylelib/firalight.mplstyle` & `erlab-1.6.4/src/erlab/plotting/stylelib/firalight.mplstyle`

 * *Files identical despite different names*

### Comparing `erlab-1.6.3/src/erlab/plotting/stylelib/khan.mplstyle` & `erlab-1.6.4/src/erlab/plotting/stylelib/khan.mplstyle`

 * *Files identical despite different names*

### Comparing `erlab-1.6.3/src/erlab/plotting/stylelib/nature.mplstyle` & `erlab-1.6.4/src/erlab/plotting/stylelib/nature.mplstyle`

 * *Files identical despite different names*

### Comparing `erlab-1.6.3/src/erlab/plotting/stylelib/poster.mplstyle` & `erlab-1.6.4/src/erlab/plotting/stylelib/poster.mplstyle`

 * *Files identical despite different names*

### Comparing `erlab-1.6.3/src/erlab/plotting/stylelib/times.mplstyle` & `erlab-1.6.4/src/erlab/plotting/stylelib/times.mplstyle`

 * *Files identical despite different names*

### Comparing `erlab-1.6.3/src/erlab.egg-info/PKG-INFO` & `erlab-1.6.4/src/erlab.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: erlab
-Version: 1.6.3
+Version: 1.6.4
 Summary: Python package for ARPES data analysis and visualization.
 Author-email: Kimoon Han <khan@kaist.ac.kr>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `erlab-1.6.3/src/erlab.egg-info/SOURCES.txt` & `erlab-1.6.4/src/erlab.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `erlab-1.6.3/tests/test_fastbinning.py` & `erlab-1.6.4/tests/test_fastbinning.py`

 * *Files identical despite different names*

### Comparing `erlab-1.6.3/tests/test_interpolate.py` & `erlab-1.6.4/tests/test_interpolate.py`

 * *Files identical despite different names*

### Comparing `erlab-1.6.3/tests/test_kspace.py` & `erlab-1.6.4/tests/test_kspace.py`

 * *Files identical despite different names*

