# Comparing `tmp/erlab-1.6.0.tar.gz` & `tmp/erlab-1.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "erlab-1.6.0.tar", last modified: Tue Apr  2 04:32:46 2024, max compression
+gzip compressed data, was "erlab-1.6.1.tar", last modified: Wed Apr  3 06:06:53 2024, max compression
```

## Comparing `erlab-1.6.0.tar` & `erlab-1.6.1.tar`

### file list

```diff
@@ -1,159 +1,161 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 04:32:46.824938 erlab-1.6.0/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 04:32:46.784939 erlab-1.6.0/.github/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 04:32:46.788939 erlab-1.6.0/.github/workflows/
--rw-r--r--   0 root         (0) root         (0)     1561 2024-04-02 04:32:41.000000 erlab-1.6.0/.github/workflows/pr.yml
--rw-r--r--   0 root         (0) root         (0)     2420 2024-04-02 04:32:41.000000 erlab-1.6.0/.github/workflows/release.yml
--rw-r--r--   0 root         (0) root         (0)     2897 2024-04-02 04:32:41.000000 erlab-1.6.0/.gitignore
--rw-r--r--   0 root         (0) root         (0)      225 2024-04-02 04:32:41.000000 erlab-1.6.0/.pre-commit-config.yaml
--rw-r--r--   0 root         (0) root         (0)      795 2024-04-02 04:32:41.000000 erlab-1.6.0/.readthedocs.yaml
--rw-r--r--   0 root         (0) root         (0)    94797 2024-04-02 04:32:43.000000 erlab-1.6.0/CHANGELOG.md
--rw-r--r--   0 root         (0) root         (0)    35149 2024-04-02 04:32:41.000000 erlab-1.6.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)    46715 2024-04-02 04:32:46.824938 erlab-1.6.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1485 2024-04-02 04:32:41.000000 erlab-1.6.0/PythonInterface.ipf
--rw-r--r--   0 root         (0) root         (0)     4414 2024-04-02 04:32:41.000000 erlab-1.6.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 04:32:46.788939 erlab-1.6.0/docs/
--rw-r--r--   0 root         (0) root         (0)      638 2024-04-02 04:32:41.000000 erlab-1.6.0/docs/Makefile
--rw-r--r--   0 root         (0) root         (0)      727 2024-04-02 04:32:41.000000 erlab-1.6.0/docs/environment.yml
--rw-r--r--   0 root         (0) root         (0)      804 2024-04-02 04:32:41.000000 erlab-1.6.0/docs/make.bat
--rw-r--r--   0 root         (0) root         (0)      523 2024-04-02 04:32:41.000000 erlab-1.6.0/docs/requirements.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 04:32:46.792939 erlab-1.6.0/docs/source/
--rw-r--r--   0 root         (0) root         (0)       52 2024-04-02 04:32:41.000000 erlab-1.6.0/docs/source/bibliography.rst
--rw-r--r--   0 root         (0) root         (0)    10762 2024-04-02 04:32:41.000000 erlab-1.6.0/docs/source/conf.py
--rw-r--r--   0 root         (0) root         (0)    13434 2024-04-02 04:32:41.000000 erlab-1.6.0/docs/source/development.rst
--rw-r--r--   0 root         (0) root         (0)      267 2024-04-02 04:32:41.000000 erlab-1.6.0/docs/source/erlab.accessors.rst
--rw-r--r--   0 root         (0) root         (0)      117 2024-04-02 04:32:41.000000 erlab-1.6.0/docs/source/erlab.analysis.rst
--rw-r--r--   0 root         (0) root         (0)      196 2024-04-02 04:32:41.000000 erlab-1.6.0/docs/source/erlab.characterization.rst
--rw-r--r--   0 root         (0) root         (0)      546 2024-04-02 04:32:41.000000 erlab-1.6.0/docs/source/erlab.constants.rst
--rw-r--r--   0 root         (0) root         (0)      171 2024-04-02 04:32:41.000000 erlab-1.6.0/docs/source/erlab.interactive.rst
--rw-r--r--   0 root         (0) root         (0)       82 2024-04-02 04:32:41.000000 erlab-1.6.0/docs/source/erlab.io.rst
--rw-r--r--   0 root         (0) root         (0)      291 2024-04-02 04:32:41.000000 erlab-1.6.0/docs/source/erlab.lattice.rst
--rw-r--r--   0 root         (0) root         (0)      297 2024-04-02 04:32:41.000000 erlab-1.6.0/docs/source/erlab.parallel.rst
--rw-r--r--   0 root         (0) root         (0)      229 2024-04-02 04:32:41.000000 erlab-1.6.0/docs/source/erlab.plotting.rst
--rw-r--r--   0 root         (0) root         (0)     2058 2024-04-02 04:32:41.000000 erlab-1.6.0/docs/source/getting-started.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 04:32:46.800938 erlab-1.6.0/docs/source/images/
--rw-r--r--   0 root         (0) root         (0)   996803 2024-04-02 04:32:41.000000 erlab-1.6.0/docs/source/images/imagetool_dark.png
--rw-r--r--   0 root         (0) root         (0)   966547 2024-04-02 04:32:41.000000 erlab-1.6.0/docs/source/images/imagetool_light.png
--rw-r--r--   0 root         (0) root         (0)   709231 2024-04-02 04:32:41.000000 erlab-1.6.0/docs/source/images/ktool_1_dark.png
--rw-r--r--   0 root         (0) root         (0)   694078 2024-04-02 04:32:41.000000 erlab-1.6.0/docs/source/images/ktool_1_light.png
--rw-r--r--   0 root         (0) root         (0)   703343 2024-04-02 04:32:41.000000 erlab-1.6.0/docs/source/images/ktool_2_dark.png
--rw-r--r--   0 root         (0) root         (0)   686688 2024-04-02 04:32:41.000000 erlab-1.6.0/docs/source/images/ktool_2_light.png
--rw-r--r--   0 root         (0) root         (0)     2497 2024-04-02 04:32:41.000000 erlab-1.6.0/docs/source/index.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 04:32:46.800938 erlab-1.6.0/docs/source/notebooks/
--rw-r--r--   0 root         (0) root         (0)   189769 2024-04-02 04:32:41.000000 erlab-1.6.0/docs/source/notebooks/indexing.ipynb
--rw-r--r--   0 root         (0) root         (0)     1582 2024-04-02 04:32:41.000000 erlab-1.6.0/docs/source/notebooks/io.ipynb
--rw-r--r--   0 root         (0) root         (0)   379517 2024-04-02 04:32:41.000000 erlab-1.6.0/docs/source/notebooks/kconv.ipynb
--rw-r--r--   0 root         (0) root         (0)  1541528 2024-04-02 04:32:41.000000 erlab-1.6.0/docs/source/notebooks/plotting.ipynb
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 04:32:46.804938 erlab-1.6.0/docs/source/pyplots/
--rw-r--r--   0 root         (0) root         (0)     2579 2024-04-02 04:32:41.000000 erlab-1.6.0/docs/source/pyplots/norms.py
--rw-r--r--   0 root         (0) root         (0)     1349 2024-04-02 04:32:41.000000 erlab-1.6.0/docs/source/reference.rst
--rw-r--r--   0 root         (0) root         (0)     1316 2024-04-02 04:32:41.000000 erlab-1.6.0/docs/source/refs.bib
--rw-r--r--   0 root         (0) root         (0)     1143 2024-04-02 04:32:41.000000 erlab-1.6.0/docs/source/userguide.rst
--rw-r--r--   0 root         (0) root         (0)      891 2024-04-02 04:32:41.000000 erlab-1.6.0/environment.yml
--rw-r--r--   0 root         (0) root         (0)     1001 2024-04-02 04:32:41.000000 erlab-1.6.0/environment_apple.yml
--rw-r--r--   0 root         (0) root         (0)      888 2024-04-02 04:32:41.000000 erlab-1.6.0/environment_nogit.yml
--rw-r--r--   0 root         (0) root         (0)      860 2024-04-02 04:32:41.000000 erlab-1.6.0/environment_nogit_mkl.yml
--rw-r--r--   0 root         (0) root         (0)     4265 2024-04-02 04:32:41.000000 erlab-1.6.0/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)      339 2024-04-02 04:32:41.000000 erlab-1.6.0/requirements.txt
--rw-r--r--   0 root         (0) root         (0)       38 2024-04-02 04:32:46.824938 erlab-1.6.0/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 04:32:46.784939 erlab-1.6.0/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 04:32:46.804938 erlab-1.6.0/src/erlab/
--rw-r--r--   0 root         (0) root         (0)       60 2024-04-02 04:32:43.000000 erlab-1.6.0/src/erlab/__init__.py
--rw-r--r--   0 root         (0) root         (0)    35539 2024-04-02 04:32:41.000000 erlab-1.6.0/src/erlab/accessors.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 04:32:46.808938 erlab-1.6.0/src/erlab/analysis/
--rw-r--r--   0 root         (0) root         (0)      748 2024-04-02 04:32:41.000000 erlab-1.6.0/src/erlab/analysis/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5514 2024-04-02 04:32:41.000000 erlab-1.6.0/src/erlab/analysis/correlation.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 04:32:46.808938 erlab-1.6.0/src/erlab/analysis/fit/
--rw-r--r--   0 root         (0) root         (0)      459 2024-04-02 04:32:41.000000 erlab-1.6.0/src/erlab/analysis/fit/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 04:32:46.808938 erlab-1.6.0/src/erlab/analysis/fit/functions/
--rw-r--r--   0 root         (0) root         (0)      812 2024-04-02 04:32:41.000000 erlab-1.6.0/src/erlab/analysis/fit/functions/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8766 2024-04-02 04:32:41.000000 erlab-1.6.0/src/erlab/analysis/fit/functions/dynamic.py
--rw-r--r--   0 root         (0) root         (0)     6026 2024-04-02 04:32:41.000000 erlab-1.6.0/src/erlab/analysis/fit/functions/general.py
--rw-r--r--   0 root         (0) root         (0)     6165 2024-04-02 04:32:41.000000 erlab-1.6.0/src/erlab/analysis/fit/minuit.py
--rw-r--r--   0 root         (0) root         (0)    10572 2024-04-02 04:32:41.000000 erlab-1.6.0/src/erlab/analysis/fit/models.py
--rw-r--r--   0 root         (0) root         (0)      982 2024-04-02 04:32:41.000000 erlab-1.6.0/src/erlab/analysis/fit/spline.py
--rw-r--r--   0 root         (0) root         (0)    13815 2024-04-02 04:32:41.000000 erlab-1.6.0/src/erlab/analysis/gold.py
--rw-r--r--   0 root         (0) root         (0)     9811 2024-04-02 04:32:41.000000 erlab-1.6.0/src/erlab/analysis/interpolate.py
--rw-r--r--   0 root         (0) root         (0)    10344 2024-04-02 04:32:41.000000 erlab-1.6.0/src/erlab/analysis/kspace.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 04:32:46.808938 erlab-1.6.0/src/erlab/analysis/mask/
--rw-r--r--   0 root         (0) root         (0)     2768 2024-04-02 04:32:41.000000 erlab-1.6.0/src/erlab/analysis/mask/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7810 2024-04-02 04:32:41.000000 erlab-1.6.0/src/erlab/analysis/mask/polygon.py
--rw-r--r--   0 root         (0) root         (0)      878 2024-04-02 04:32:41.000000 erlab-1.6.0/src/erlab/analysis/transform.py
--rw-r--r--   0 root         (0) root         (0)     8332 2024-04-02 04:32:41.000000 erlab-1.6.0/src/erlab/analysis/utilities.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 04:32:46.812938 erlab-1.6.0/src/erlab/characterization/
--rw-r--r--   0 root         (0) root         (0)      191 2024-04-02 04:32:41.000000 erlab-1.6.0/src/erlab/characterization/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3093 2024-04-02 04:32:41.000000 erlab-1.6.0/src/erlab/characterization/resistance.py
--rw-r--r--   0 root         (0) root         (0)     1903 2024-04-02 04:32:41.000000 erlab-1.6.0/src/erlab/characterization/xrd.py
--rw-r--r--   0 root         (0) root         (0)     2115 2024-04-02 04:32:41.000000 erlab-1.6.0/src/erlab/constants.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 04:32:46.812938 erlab-1.6.0/src/erlab/interactive/
--rw-r--r--   0 root         (0) root         (0)      540 2024-04-02 04:32:41.000000 erlab-1.6.0/src/erlab/interactive/__init__.py
--rw-r--r--   0 root         (0) root         (0)    13943 2024-04-02 04:32:41.000000 erlab-1.6.0/src/erlab/interactive/bzplot.py
--rw-r--r--   0 root         (0) root         (0)    20820 2024-04-02 04:32:41.000000 erlab-1.6.0/src/erlab/interactive/colors.py
--rw-r--r--   0 root         (0) root         (0)    22076 2024-04-02 04:32:41.000000 erlab-1.6.0/src/erlab/interactive/curvefittingtool.py
--rw-r--r--   0 root         (0) root         (0)    19528 2024-04-02 04:32:41.000000 erlab-1.6.0/src/erlab/interactive/derivative.py
--rw-r--r--   0 root         (0) root         (0)     9458 2024-04-02 04:32:41.000000 erlab-1.6.0/src/erlab/interactive/exampledata.py
--rw-r--r--   0 root         (0) root         (0)    19072 2024-04-02 04:32:41.000000 erlab-1.6.0/src/erlab/interactive/fermiedge.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 04:32:46.816938 erlab-1.6.0/src/erlab/interactive/imagetool/
--rw-r--r--   0 root         (0) root         (0)    19391 2024-04-02 04:32:41.000000 erlab-1.6.0/src/erlab/interactive/imagetool/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 04:32:46.816938 erlab-1.6.0/src/erlab/interactive/imagetool/_deprecated/
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-02 04:32:41.000000 erlab-1.6.0/src/erlab/interactive/imagetool/_deprecated/__init__.py
--rw-r--r--   0 root         (0) root         (0)    51730 2024-04-02 04:32:41.000000 erlab-1.6.0/src/erlab/interactive/imagetool/_deprecated/imagetool_mpl.py
--rw-r--r--   0 root         (0) root         (0)   114232 2024-04-02 04:32:41.000000 erlab-1.6.0/src/erlab/interactive/imagetool/_deprecated/imagetool_old.py
--rw-r--r--   0 root         (0) root         (0)    27081 2024-04-02 04:32:41.000000 erlab-1.6.0/src/erlab/interactive/imagetool/controls.py
--rw-r--r--   0 root         (0) root         (0)    53776 2024-04-02 04:32:41.000000 erlab-1.6.0/src/erlab/interactive/imagetool/core.py
--rw-r--r--   0 root         (0) root         (0)    11483 2024-04-02 04:32:41.000000 erlab-1.6.0/src/erlab/interactive/imagetool/fastbinning.py
--rw-r--r--   0 root         (0) root         (0)    23195 2024-04-02 04:32:41.000000 erlab-1.6.0/src/erlab/interactive/imagetool/slicer.py
--rw-r--r--   0 root         (0) root         (0)    16658 2024-04-02 04:32:41.000000 erlab-1.6.0/src/erlab/interactive/kspace.py
--rw-r--r--   0 root         (0) root         (0)    19382 2024-04-02 04:32:41.000000 erlab-1.6.0/src/erlab/interactive/ktool.ui
--rw-r--r--   0 root         (0) root         (0)    21306 2024-04-02 04:32:41.000000 erlab-1.6.0/src/erlab/interactive/ktool_old.py
--rw-r--r--   0 root         (0) root         (0)     3341 2024-04-02 04:32:41.000000 erlab-1.6.0/src/erlab/interactive/masktool.py
--rw-r--r--   0 root         (0) root         (0)    52417 2024-04-02 04:32:41.000000 erlab-1.6.0/src/erlab/interactive/utilities.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 04:32:46.816938 erlab-1.6.0/src/erlab/io/
--rw-r--r--   0 root         (0) root         (0)     1937 2024-04-02 04:32:41.000000 erlab-1.6.0/src/erlab/io/__init__.py
--rw-r--r--   0 root         (0) root         (0)    30047 2024-04-02 04:32:41.000000 erlab-1.6.0/src/erlab/io/dataloader.py
--rw-r--r--   0 root         (0) root         (0)     7887 2024-04-02 04:32:41.000000 erlab-1.6.0/src/erlab/io/igor.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 04:32:46.816938 erlab-1.6.0/src/erlab/io/plugins/
--rw-r--r--   0 root         (0) root         (0)      900 2024-04-02 04:32:41.000000 erlab-1.6.0/src/erlab/io/plugins/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3674 2024-04-02 04:32:41.000000 erlab-1.6.0/src/erlab/io/plugins/da30.py
--rw-r--r--   0 root         (0) root         (0)     1185 2024-04-02 04:32:41.000000 erlab-1.6.0/src/erlab/io/plugins/kriss.py
--rw-r--r--   0 root         (0) root         (0)     7448 2024-04-02 04:32:41.000000 erlab-1.6.0/src/erlab/io/plugins/merlin.py
--rw-r--r--   0 root         (0) root         (0)     7745 2024-04-02 04:32:41.000000 erlab-1.6.0/src/erlab/io/plugins/ssrl52.py
--rw-r--r--   0 root         (0) root         (0)     5630 2024-04-02 04:32:41.000000 erlab-1.6.0/src/erlab/io/utilities.py
--rw-r--r--   0 root         (0) root         (0)     2515 2024-04-02 04:32:41.000000 erlab-1.6.0/src/erlab/lattice.py
--rw-r--r--   0 root         (0) root         (0)     2242 2024-04-02 04:32:41.000000 erlab-1.6.0/src/erlab/parallel.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 04:32:46.820938 erlab-1.6.0/src/erlab/plotting/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 04:32:46.820938 erlab-1.6.0/src/erlab/plotting/IgorCT/
--rw-r--r--   0 root         (0) root         (0)     3379 2024-04-02 04:32:41.000000 erlab-1.6.0/src/erlab/plotting/IgorCT/Blue-White.txt
--rw-r--r--   0 root         (0) root         (0)     3456 2024-04-02 04:32:41.000000 erlab-1.6.0/src/erlab/plotting/IgorCT/BlueHot.ibw
--rw-r--r--   0 root         (0) root         (0)     3526 2024-04-02 04:32:41.000000 erlab-1.6.0/src/erlab/plotting/IgorCT/CTBlueWhite.ibw
--rw-r--r--   0 root         (0) root         (0)     3530 2024-04-02 04:32:41.000000 erlab-1.6.0/src/erlab/plotting/IgorCT/CTRainbowLIght.ibw
--rw-r--r--   0 root         (0) root         (0)     3531 2024-04-02 04:32:41.000000 erlab-1.6.0/src/erlab/plotting/IgorCT/CTRedTemperature.ibw
--rw-r--r--   0 root         (0) root         (0)     3456 2024-04-02 04:32:41.000000 erlab-1.6.0/src/erlab/plotting/IgorCT/ColdWarm.ibw
--rw-r--r--   0 root         (0) root         (0)     3456 2024-04-02 04:32:41.000000 erlab-1.6.0/src/erlab/plotting/IgorCT/PlanetEarth.ibw
--rw-r--r--   0 root         (0) root         (0)     1920 2024-04-02 04:32:41.000000 erlab-1.6.0/src/erlab/plotting/IgorCT/ametrine.ibw
--rw-r--r--   0 root         (0) root         (0)     2048 2024-04-02 04:32:41.000000 erlab-1.6.0/src/erlab/plotting/IgorCT/isolum.ibw
--rw-r--r--   0 root         (0) root         (0)     2048 2024-04-02 04:32:41.000000 erlab-1.6.0/src/erlab/plotting/IgorCT/morgenstemning.ibw
--rw-r--r--   0 root         (0) root         (0)     1784 2024-04-02 04:32:41.000000 erlab-1.6.0/src/erlab/plotting/__init__.py
--rw-r--r--   0 root         (0) root         (0)    29010 2024-04-02 04:32:41.000000 erlab-1.6.0/src/erlab/plotting/annotations.py
--rw-r--r--   0 root         (0) root         (0)    18275 2024-04-02 04:32:41.000000 erlab-1.6.0/src/erlab/plotting/atoms.py
--rw-r--r--   0 root         (0) root         (0)     4294 2024-04-02 04:32:41.000000 erlab-1.6.0/src/erlab/plotting/bz.py
--rw-r--r--   0 root         (0) root         (0)    32411 2024-04-02 04:32:41.000000 erlab-1.6.0/src/erlab/plotting/colors.py
--rw-r--r--   0 root         (0) root         (0)     2657 2024-04-02 04:32:41.000000 erlab-1.6.0/src/erlab/plotting/erplot.py
--rw-r--r--   0 root         (0) root         (0)    30998 2024-04-02 04:32:41.000000 erlab-1.6.0/src/erlab/plotting/general.py
--rw-r--r--   0 root         (0) root         (0)     2726 2024-04-02 04:32:41.000000 erlab-1.6.0/src/erlab/plotting/plot3d.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 04:32:46.824938 erlab-1.6.0/src/erlab/plotting/stylelib/
--rw-r--r--   0 root         (0) root         (0)     6839 2024-04-02 04:32:41.000000 erlab-1.6.0/src/erlab/plotting/stylelib/fira.mplstyle
--rw-r--r--   0 root         (0) root         (0)     6826 2024-04-02 04:32:41.000000 erlab-1.6.0/src/erlab/plotting/stylelib/firalight.mplstyle
--rw-r--r--   0 root         (0) root         (0)    14358 2024-04-02 04:32:41.000000 erlab-1.6.0/src/erlab/plotting/stylelib/khan.mplstyle
--rw-r--r--   0 root         (0) root         (0)     9160 2024-04-02 04:32:41.000000 erlab-1.6.0/src/erlab/plotting/stylelib/nature.mplstyle
--rw-r--r--   0 root         (0) root         (0)      629 2024-04-02 04:32:41.000000 erlab-1.6.0/src/erlab/plotting/stylelib/poster.mplstyle
--rw-r--r--   0 root         (0) root         (0)     7023 2024-04-02 04:32:41.000000 erlab-1.6.0/src/erlab/plotting/stylelib/times.mplstyle
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 04:32:46.824938 erlab-1.6.0/src/erlab.egg-info/
--rw-r--r--   0 root         (0) root         (0)    46715 2024-04-02 04:32:46.000000 erlab-1.6.0/src/erlab.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     4221 2024-04-02 04:32:46.000000 erlab-1.6.0/src/erlab.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-02 04:32:46.000000 erlab-1.6.0/src/erlab.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      329 2024-04-02 04:32:46.000000 erlab-1.6.0/src/erlab.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        6 2024-04-02 04:32:46.000000 erlab-1.6.0/src/erlab.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 04:32:46.824938 erlab-1.6.0/tests/
--rw-r--r--   0 root         (0) root         (0)      595 2024-04-02 04:32:41.000000 erlab-1.6.0/tests/test_fastbinning.py
--rw-r--r--   0 root         (0) root         (0)      598 2024-04-02 04:32:41.000000 erlab-1.6.0/tests/test_interpolate.py
--rw-r--r--   0 root         (0) root         (0)     2419 2024-04-02 04:32:41.000000 erlab-1.6.0/tests/test_kspace.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 06:06:53.069605 erlab-1.6.1/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 06:06:53.025605 erlab-1.6.1/.github/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 06:06:53.033605 erlab-1.6.1/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 root         (0) root         (0)      469 2024-04-03 06:06:47.000000 erlab-1.6.1/.github/ISSUE_TEMPLATE/bug-report.md
+-rw-r--r--   0 root         (0) root         (0)      608 2024-04-03 06:06:47.000000 erlab-1.6.1/.github/ISSUE_TEMPLATE/feature_request.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 06:06:53.033605 erlab-1.6.1/.github/workflows/
+-rw-r--r--   0 root         (0) root         (0)     1047 2024-04-03 06:06:47.000000 erlab-1.6.1/.github/workflows/pr.yml
+-rw-r--r--   0 root         (0) root         (0)     1893 2024-04-03 06:06:47.000000 erlab-1.6.1/.github/workflows/release.yml
+-rw-r--r--   0 root         (0) root         (0)     2898 2024-04-03 06:06:47.000000 erlab-1.6.1/.gitignore
+-rw-r--r--   0 root         (0) root         (0)      893 2024-04-03 06:06:47.000000 erlab-1.6.1/.pre-commit-config.yaml
+-rw-r--r--   0 root         (0) root         (0)      796 2024-04-03 06:06:47.000000 erlab-1.6.1/.readthedocs.yaml
+-rw-r--r--   0 root         (0) root         (0)    96539 2024-04-03 06:06:49.000000 erlab-1.6.1/CHANGELOG.md
+-rw-r--r--   0 root         (0) root         (0)    35149 2024-04-03 06:06:47.000000 erlab-1.6.1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)    46708 2024-04-03 06:06:53.069605 erlab-1.6.1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1473 2024-04-03 06:06:47.000000 erlab-1.6.1/PythonInterface.ipf
+-rw-r--r--   0 root         (0) root         (0)     4414 2024-04-03 06:06:47.000000 erlab-1.6.1/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 06:06:53.033605 erlab-1.6.1/docs/
+-rw-r--r--   0 root         (0) root         (0)      638 2024-04-03 06:06:47.000000 erlab-1.6.1/docs/Makefile
+-rw-r--r--   0 root         (0) root         (0)      752 2024-04-03 06:06:47.000000 erlab-1.6.1/docs/environment.yml
+-rw-r--r--   0 root         (0) root         (0)      804 2024-04-03 06:06:47.000000 erlab-1.6.1/docs/make.bat
+-rw-r--r--   0 root         (0) root         (0)      540 2024-04-03 06:06:47.000000 erlab-1.6.1/docs/requirements.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 06:06:53.037605 erlab-1.6.1/docs/source/
+-rw-r--r--   0 root         (0) root         (0)       52 2024-04-03 06:06:47.000000 erlab-1.6.1/docs/source/bibliography.rst
+-rw-r--r--   0 root         (0) root         (0)    10762 2024-04-03 06:06:47.000000 erlab-1.6.1/docs/source/conf.py
+-rw-r--r--   0 root         (0) root         (0)    13410 2024-04-03 06:06:47.000000 erlab-1.6.1/docs/source/development.rst
+-rw-r--r--   0 root         (0) root         (0)      265 2024-04-03 06:06:47.000000 erlab-1.6.1/docs/source/erlab.accessors.rst
+-rw-r--r--   0 root         (0) root         (0)      101 2024-04-03 06:06:47.000000 erlab-1.6.1/docs/source/erlab.analysis.rst
+-rw-r--r--   0 root         (0) root         (0)      141 2024-04-03 06:06:47.000000 erlab-1.6.1/docs/source/erlab.characterization.rst
+-rw-r--r--   0 root         (0) root         (0)      485 2024-04-03 06:06:47.000000 erlab-1.6.1/docs/source/erlab.constants.rst
+-rw-r--r--   0 root         (0) root         (0)      116 2024-04-03 06:06:47.000000 erlab-1.6.1/docs/source/erlab.interactive.rst
+-rw-r--r--   0 root         (0) root         (0)       81 2024-04-03 06:06:47.000000 erlab-1.6.1/docs/source/erlab.io.rst
+-rw-r--r--   0 root         (0) root         (0)      236 2024-04-03 06:06:47.000000 erlab-1.6.1/docs/source/erlab.lattice.rst
+-rw-r--r--   0 root         (0) root         (0)      242 2024-04-03 06:06:47.000000 erlab-1.6.1/docs/source/erlab.parallel.rst
+-rw-r--r--   0 root         (0) root         (0)      174 2024-04-03 06:06:47.000000 erlab-1.6.1/docs/source/erlab.plotting.rst
+-rw-r--r--   0 root         (0) root         (0)     2888 2024-04-03 06:06:47.000000 erlab-1.6.1/docs/source/getting-started.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 06:06:53.045605 erlab-1.6.1/docs/source/images/
+-rw-r--r--   0 root         (0) root         (0)   996803 2024-04-03 06:06:47.000000 erlab-1.6.1/docs/source/images/imagetool_dark.png
+-rw-r--r--   0 root         (0) root         (0)   966547 2024-04-03 06:06:47.000000 erlab-1.6.1/docs/source/images/imagetool_light.png
+-rw-r--r--   0 root         (0) root         (0)   709231 2024-04-03 06:06:47.000000 erlab-1.6.1/docs/source/images/ktool_1_dark.png
+-rw-r--r--   0 root         (0) root         (0)   694078 2024-04-03 06:06:47.000000 erlab-1.6.1/docs/source/images/ktool_1_light.png
+-rw-r--r--   0 root         (0) root         (0)   703343 2024-04-03 06:06:47.000000 erlab-1.6.1/docs/source/images/ktool_2_dark.png
+-rw-r--r--   0 root         (0) root         (0)   686688 2024-04-03 06:06:47.000000 erlab-1.6.1/docs/source/images/ktool_2_light.png
+-rw-r--r--   0 root         (0) root         (0)     2497 2024-04-03 06:06:47.000000 erlab-1.6.1/docs/source/index.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 06:06:53.049605 erlab-1.6.1/docs/source/notebooks/
+-rw-r--r--   0 root         (0) root         (0)   189769 2024-04-03 06:06:47.000000 erlab-1.6.1/docs/source/notebooks/indexing.ipynb
+-rw-r--r--   0 root         (0) root         (0)     1582 2024-04-03 06:06:47.000000 erlab-1.6.1/docs/source/notebooks/io.ipynb
+-rw-r--r--   0 root         (0) root         (0)   379528 2024-04-03 06:06:47.000000 erlab-1.6.1/docs/source/notebooks/kconv.ipynb
+-rw-r--r--   0 root         (0) root         (0)    15761 2024-04-03 06:06:47.000000 erlab-1.6.1/docs/source/notebooks/plotting.ipynb
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 06:06:53.049605 erlab-1.6.1/docs/source/pyplots/
+-rw-r--r--   0 root         (0) root         (0)     2579 2024-04-03 06:06:47.000000 erlab-1.6.1/docs/source/pyplots/norms.py
+-rw-r--r--   0 root         (0) root         (0)     1344 2024-04-03 06:06:47.000000 erlab-1.6.1/docs/source/reference.rst
+-rw-r--r--   0 root         (0) root         (0)     1316 2024-04-03 06:06:47.000000 erlab-1.6.1/docs/source/refs.bib
+-rw-r--r--   0 root         (0) root         (0)     1142 2024-04-03 06:06:47.000000 erlab-1.6.1/docs/source/userguide.rst
+-rw-r--r--   0 root         (0) root         (0)      880 2024-04-03 06:06:47.000000 erlab-1.6.1/environment.yml
+-rw-r--r--   0 root         (0) root         (0)      990 2024-04-03 06:06:47.000000 erlab-1.6.1/environment_apple.yml
+-rw-r--r--   0 root         (0) root         (0)      876 2024-04-03 06:06:47.000000 erlab-1.6.1/environment_nogit.yml
+-rw-r--r--   0 root         (0) root         (0)      848 2024-04-03 06:06:47.000000 erlab-1.6.1/environment_nogit_mkl.yml
+-rw-r--r--   0 root         (0) root         (0)     4227 2024-04-03 06:06:47.000000 erlab-1.6.1/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)      334 2024-04-03 06:06:47.000000 erlab-1.6.1/requirements.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-03 06:06:53.069605 erlab-1.6.1/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 06:06:53.029605 erlab-1.6.1/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 06:06:53.049605 erlab-1.6.1/src/erlab/
+-rw-r--r--   0 root         (0) root         (0)       60 2024-04-03 06:06:49.000000 erlab-1.6.1/src/erlab/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    35539 2024-04-03 06:06:47.000000 erlab-1.6.1/src/erlab/accessors.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 06:06:53.053605 erlab-1.6.1/src/erlab/analysis/
+-rw-r--r--   0 root         (0) root         (0)      748 2024-04-03 06:06:47.000000 erlab-1.6.1/src/erlab/analysis/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5514 2024-04-03 06:06:47.000000 erlab-1.6.1/src/erlab/analysis/correlation.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 06:06:53.053605 erlab-1.6.1/src/erlab/analysis/fit/
+-rw-r--r--   0 root         (0) root         (0)      459 2024-04-03 06:06:47.000000 erlab-1.6.1/src/erlab/analysis/fit/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 06:06:53.053605 erlab-1.6.1/src/erlab/analysis/fit/functions/
+-rw-r--r--   0 root         (0) root         (0)      812 2024-04-03 06:06:47.000000 erlab-1.6.1/src/erlab/analysis/fit/functions/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8766 2024-04-03 06:06:47.000000 erlab-1.6.1/src/erlab/analysis/fit/functions/dynamic.py
+-rw-r--r--   0 root         (0) root         (0)     6026 2024-04-03 06:06:47.000000 erlab-1.6.1/src/erlab/analysis/fit/functions/general.py
+-rw-r--r--   0 root         (0) root         (0)     6165 2024-04-03 06:06:47.000000 erlab-1.6.1/src/erlab/analysis/fit/minuit.py
+-rw-r--r--   0 root         (0) root         (0)    10572 2024-04-03 06:06:47.000000 erlab-1.6.1/src/erlab/analysis/fit/models.py
+-rw-r--r--   0 root         (0) root         (0)     1168 2024-04-03 06:06:47.000000 erlab-1.6.1/src/erlab/analysis/fit/spline.py
+-rw-r--r--   0 root         (0) root         (0)    13815 2024-04-03 06:06:47.000000 erlab-1.6.1/src/erlab/analysis/gold.py
+-rw-r--r--   0 root         (0) root         (0)     9811 2024-04-03 06:06:47.000000 erlab-1.6.1/src/erlab/analysis/interpolate.py
+-rw-r--r--   0 root         (0) root         (0)    10344 2024-04-03 06:06:47.000000 erlab-1.6.1/src/erlab/analysis/kspace.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 06:06:53.053605 erlab-1.6.1/src/erlab/analysis/mask/
+-rw-r--r--   0 root         (0) root         (0)     2768 2024-04-03 06:06:47.000000 erlab-1.6.1/src/erlab/analysis/mask/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7810 2024-04-03 06:06:47.000000 erlab-1.6.1/src/erlab/analysis/mask/polygon.py
+-rw-r--r--   0 root         (0) root         (0)      878 2024-04-03 06:06:47.000000 erlab-1.6.1/src/erlab/analysis/transform.py
+-rw-r--r--   0 root         (0) root         (0)     8332 2024-04-03 06:06:47.000000 erlab-1.6.1/src/erlab/analysis/utilities.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 06:06:53.053605 erlab-1.6.1/src/erlab/characterization/
+-rw-r--r--   0 root         (0) root         (0)      191 2024-04-03 06:06:47.000000 erlab-1.6.1/src/erlab/characterization/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3093 2024-04-03 06:06:47.000000 erlab-1.6.1/src/erlab/characterization/resistance.py
+-rw-r--r--   0 root         (0) root         (0)     1903 2024-04-03 06:06:47.000000 erlab-1.6.1/src/erlab/characterization/xrd.py
+-rw-r--r--   0 root         (0) root         (0)     2115 2024-04-03 06:06:47.000000 erlab-1.6.1/src/erlab/constants.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 06:06:53.057605 erlab-1.6.1/src/erlab/interactive/
+-rw-r--r--   0 root         (0) root         (0)      540 2024-04-03 06:06:47.000000 erlab-1.6.1/src/erlab/interactive/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    13943 2024-04-03 06:06:47.000000 erlab-1.6.1/src/erlab/interactive/bzplot.py
+-rw-r--r--   0 root         (0) root         (0)    20820 2024-04-03 06:06:47.000000 erlab-1.6.1/src/erlab/interactive/colors.py
+-rw-r--r--   0 root         (0) root         (0)    22076 2024-04-03 06:06:47.000000 erlab-1.6.1/src/erlab/interactive/curvefittingtool.py
+-rw-r--r--   0 root         (0) root         (0)    19528 2024-04-03 06:06:47.000000 erlab-1.6.1/src/erlab/interactive/derivative.py
+-rw-r--r--   0 root         (0) root         (0)     9458 2024-04-03 06:06:47.000000 erlab-1.6.1/src/erlab/interactive/exampledata.py
+-rw-r--r--   0 root         (0) root         (0)    19072 2024-04-03 06:06:47.000000 erlab-1.6.1/src/erlab/interactive/fermiedge.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 06:06:53.057605 erlab-1.6.1/src/erlab/interactive/imagetool/
+-rw-r--r--   0 root         (0) root         (0)    19391 2024-04-03 06:06:47.000000 erlab-1.6.1/src/erlab/interactive/imagetool/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 06:06:53.061605 erlab-1.6.1/src/erlab/interactive/imagetool/_deprecated/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-03 06:06:47.000000 erlab-1.6.1/src/erlab/interactive/imagetool/_deprecated/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    52076 2024-04-03 06:06:47.000000 erlab-1.6.1/src/erlab/interactive/imagetool/_deprecated/imagetool_mpl.py
+-rw-r--r--   0 root         (0) root         (0)   114751 2024-04-03 06:06:47.000000 erlab-1.6.1/src/erlab/interactive/imagetool/_deprecated/imagetool_old.py
+-rw-r--r--   0 root         (0) root         (0)    27081 2024-04-03 06:06:47.000000 erlab-1.6.1/src/erlab/interactive/imagetool/controls.py
+-rw-r--r--   0 root         (0) root         (0)    53776 2024-04-03 06:06:47.000000 erlab-1.6.1/src/erlab/interactive/imagetool/core.py
+-rw-r--r--   0 root         (0) root         (0)    11483 2024-04-03 06:06:47.000000 erlab-1.6.1/src/erlab/interactive/imagetool/fastbinning.py
+-rw-r--r--   0 root         (0) root         (0)    23195 2024-04-03 06:06:47.000000 erlab-1.6.1/src/erlab/interactive/imagetool/slicer.py
+-rw-r--r--   0 root         (0) root         (0)    16658 2024-04-03 06:06:47.000000 erlab-1.6.1/src/erlab/interactive/kspace.py
+-rw-r--r--   0 root         (0) root         (0)    19382 2024-04-03 06:06:47.000000 erlab-1.6.1/src/erlab/interactive/ktool.ui
+-rw-r--r--   0 root         (0) root         (0)     3341 2024-04-03 06:06:47.000000 erlab-1.6.1/src/erlab/interactive/masktool.py
+-rw-r--r--   0 root         (0) root         (0)    52417 2024-04-03 06:06:47.000000 erlab-1.6.1/src/erlab/interactive/utilities.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 06:06:53.061605 erlab-1.6.1/src/erlab/io/
+-rw-r--r--   0 root         (0) root         (0)     1937 2024-04-03 06:06:47.000000 erlab-1.6.1/src/erlab/io/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    30047 2024-04-03 06:06:47.000000 erlab-1.6.1/src/erlab/io/dataloader.py
+-rw-r--r--   0 root         (0) root         (0)     7887 2024-04-03 06:06:47.000000 erlab-1.6.1/src/erlab/io/igor.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 06:06:53.061605 erlab-1.6.1/src/erlab/io/plugins/
+-rw-r--r--   0 root         (0) root         (0)      900 2024-04-03 06:06:47.000000 erlab-1.6.1/src/erlab/io/plugins/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3674 2024-04-03 06:06:47.000000 erlab-1.6.1/src/erlab/io/plugins/da30.py
+-rw-r--r--   0 root         (0) root         (0)     1185 2024-04-03 06:06:47.000000 erlab-1.6.1/src/erlab/io/plugins/kriss.py
+-rw-r--r--   0 root         (0) root         (0)     7448 2024-04-03 06:06:47.000000 erlab-1.6.1/src/erlab/io/plugins/merlin.py
+-rw-r--r--   0 root         (0) root         (0)     7745 2024-04-03 06:06:47.000000 erlab-1.6.1/src/erlab/io/plugins/ssrl52.py
+-rw-r--r--   0 root         (0) root         (0)     5630 2024-04-03 06:06:47.000000 erlab-1.6.1/src/erlab/io/utilities.py
+-rw-r--r--   0 root         (0) root         (0)     2515 2024-04-03 06:06:47.000000 erlab-1.6.1/src/erlab/lattice.py
+-rw-r--r--   0 root         (0) root         (0)     2242 2024-04-03 06:06:47.000000 erlab-1.6.1/src/erlab/parallel.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 06:06:53.065605 erlab-1.6.1/src/erlab/plotting/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 06:06:53.065605 erlab-1.6.1/src/erlab/plotting/IgorCT/
+-rw-r--r--   0 root         (0) root         (0)     3379 2024-04-03 06:06:47.000000 erlab-1.6.1/src/erlab/plotting/IgorCT/Blue-White.txt
+-rw-r--r--   0 root         (0) root         (0)     3456 2024-04-03 06:06:47.000000 erlab-1.6.1/src/erlab/plotting/IgorCT/BlueHot.ibw
+-rw-r--r--   0 root         (0) root         (0)     3526 2024-04-03 06:06:47.000000 erlab-1.6.1/src/erlab/plotting/IgorCT/CTBlueWhite.ibw
+-rw-r--r--   0 root         (0) root         (0)     3530 2024-04-03 06:06:47.000000 erlab-1.6.1/src/erlab/plotting/IgorCT/CTRainbowLIght.ibw
+-rw-r--r--   0 root         (0) root         (0)     3531 2024-04-03 06:06:47.000000 erlab-1.6.1/src/erlab/plotting/IgorCT/CTRedTemperature.ibw
+-rw-r--r--   0 root         (0) root         (0)     3456 2024-04-03 06:06:47.000000 erlab-1.6.1/src/erlab/plotting/IgorCT/ColdWarm.ibw
+-rw-r--r--   0 root         (0) root         (0)     3456 2024-04-03 06:06:47.000000 erlab-1.6.1/src/erlab/plotting/IgorCT/PlanetEarth.ibw
+-rw-r--r--   0 root         (0) root         (0)     1920 2024-04-03 06:06:47.000000 erlab-1.6.1/src/erlab/plotting/IgorCT/ametrine.ibw
+-rw-r--r--   0 root         (0) root         (0)     2048 2024-04-03 06:06:47.000000 erlab-1.6.1/src/erlab/plotting/IgorCT/isolum.ibw
+-rw-r--r--   0 root         (0) root         (0)     2048 2024-04-03 06:06:47.000000 erlab-1.6.1/src/erlab/plotting/IgorCT/morgenstemning.ibw
+-rw-r--r--   0 root         (0) root         (0)     1784 2024-04-03 06:06:47.000000 erlab-1.6.1/src/erlab/plotting/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    29010 2024-04-03 06:06:47.000000 erlab-1.6.1/src/erlab/plotting/annotations.py
+-rw-r--r--   0 root         (0) root         (0)    18275 2024-04-03 06:06:47.000000 erlab-1.6.1/src/erlab/plotting/atoms.py
+-rw-r--r--   0 root         (0) root         (0)     4294 2024-04-03 06:06:47.000000 erlab-1.6.1/src/erlab/plotting/bz.py
+-rw-r--r--   0 root         (0) root         (0)    32411 2024-04-03 06:06:47.000000 erlab-1.6.1/src/erlab/plotting/colors.py
+-rw-r--r--   0 root         (0) root         (0)     2657 2024-04-03 06:06:47.000000 erlab-1.6.1/src/erlab/plotting/erplot.py
+-rw-r--r--   0 root         (0) root         (0)    30998 2024-04-03 06:06:47.000000 erlab-1.6.1/src/erlab/plotting/general.py
+-rw-r--r--   0 root         (0) root         (0)     2726 2024-04-03 06:06:47.000000 erlab-1.6.1/src/erlab/plotting/plot3d.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 06:06:53.065605 erlab-1.6.1/src/erlab/plotting/stylelib/
+-rw-r--r--   0 root         (0) root         (0)     6839 2024-04-03 06:06:47.000000 erlab-1.6.1/src/erlab/plotting/stylelib/fira.mplstyle
+-rw-r--r--   0 root         (0) root         (0)     6826 2024-04-03 06:06:47.000000 erlab-1.6.1/src/erlab/plotting/stylelib/firalight.mplstyle
+-rw-r--r--   0 root         (0) root         (0)    14358 2024-04-03 06:06:47.000000 erlab-1.6.1/src/erlab/plotting/stylelib/khan.mplstyle
+-rw-r--r--   0 root         (0) root         (0)     9160 2024-04-03 06:06:47.000000 erlab-1.6.1/src/erlab/plotting/stylelib/nature.mplstyle
+-rw-r--r--   0 root         (0) root         (0)      630 2024-04-03 06:06:47.000000 erlab-1.6.1/src/erlab/plotting/stylelib/poster.mplstyle
+-rw-r--r--   0 root         (0) root         (0)     7023 2024-04-03 06:06:47.000000 erlab-1.6.1/src/erlab/plotting/stylelib/times.mplstyle
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 06:06:53.069605 erlab-1.6.1/src/erlab.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    46708 2024-04-03 06:06:52.000000 erlab-1.6.1/src/erlab.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     4265 2024-04-03 06:06:53.000000 erlab-1.6.1/src/erlab.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-03 06:06:52.000000 erlab-1.6.1/src/erlab.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      321 2024-04-03 06:06:52.000000 erlab-1.6.1/src/erlab.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        6 2024-04-03 06:06:52.000000 erlab-1.6.1/src/erlab.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 06:06:53.069605 erlab-1.6.1/tests/
+-rw-r--r--   0 root         (0) root         (0)      595 2024-04-03 06:06:47.000000 erlab-1.6.1/tests/test_fastbinning.py
+-rw-r--r--   0 root         (0) root         (0)      598 2024-04-03 06:06:47.000000 erlab-1.6.1/tests/test_interpolate.py
+-rw-r--r--   0 root         (0) root         (0)     2419 2024-04-03 06:06:47.000000 erlab-1.6.1/tests/test_kspace.py
```

### Comparing `erlab-1.6.0/.github/workflows/pr.yml` & `erlab-1.6.1/.github/workflows/release.yml`

 * *Files 20% similar despite different names*

```diff
@@ -1,14 +1,12 @@
-# This workflow will install Python dependencies, run tests and lint with a variety of Python versions
-# For more information see: https://docs.github.com/en/actions/automating-builds-and-tests/building-and-testing-python
-
-name: Test
+name: Release
 
 on:
-  pull_request:
+  push:
+    branches: [ "main" ]
   workflow_dispatch:
 
 jobs:
   test:
     name: Python ${{ matrix.python-version }} tests
     runs-on: ubuntu-latest
     strategy:
@@ -26,32 +24,50 @@
 
       - name: Install pytest and dependencies
         run: |
           sudo apt update && sudo apt install -y libegl1-mesa-dev
           python -m pip install --upgrade pip
           python -m pip install -v . pytest pytest-xdist
           python -m pip install -r requirements.txt
-      
+
 
       - name: Test with pytest
         run: |
           pytest -v -n auto
 
-  lint:
+  release:
+    name: Release
     runs-on: ubuntu-latest
+    concurrency: push
+    needs: test
+    environment:
+      name: pypi
+      url: https://pypi.org/p/erlab
+    permissions:
+      id-token: write
+      contents: write
 
     steps:
       - uses: actions/checkout@v4
         with:
           fetch-depth: 0
-      - name: Set up Python 3.11
-        uses: actions/setup-python@v5
+
+      - name: Python Semantic Release
+        id: release
+        uses: python-semantic-release/python-semantic-release@master
         with:
-          python-version: 3.11
-      - name: Install ruff and dependencies
-        run: |
-          sudo apt update && sudo apt install -y libegl1-mesa-dev
-          python -m pip install --upgrade pip
-          pip install ruff
+          github_token: ${{ secrets.GITHUB_TOKEN }}
 
-      - name: Run Ruff
-        run: ruff check --output-format=github .
+      - name: Publish package distributions to PyPI
+        id: pypi-publish
+        if: steps.release.outputs.released == 'true'
+        uses: pypa/gh-action-pypi-publish@release/v1
+        with:
+          verbose: true
+
+      - name: Publish package distributions to GitHub Releases
+        id: github-release
+        if: steps.release.outputs.released == 'true'
+        uses: python-semantic-release/upload-to-gh-release@main
+        with:
+          github_token: ${{ secrets.GITHUB_TOKEN }}
+          tag: ${{ steps.release.outputs.tag }}
```

### Comparing `erlab-1.6.0/.gitignore` & `erlab-1.6.1/.gitignore`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -159,8 +159,8 @@
 #  option (not recommended) you can uncomment the following to ignore the entire idea folder.
 #.idea/
 
 # VS Code
 .vscode/*
 
 # Misc. files
-itool_testing.ipynb
+itool_testing.ipynb
```

### Comparing `erlab-1.6.0/.readthedocs.yaml` & `erlab-1.6.1/.readthedocs.yaml`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -24,8 +24,8 @@
 # to build your documentation
 # See https://docs.readthedocs.io/en/stable/guides/reproducible-builds.html
 python:
   install:
     - requirements: docs/requirements.txt
 
 # conda:
-#   environment: docs/environment.yml
+#   environment: docs/environment.yml
```

### Comparing `erlab-1.6.0/CHANGELOG.md` & `erlab-1.6.1/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,50 @@
 # CHANGELOG
 
 
 
+## v1.6.1 (2024-04-03)
+
+### Chore
+
+* chore(deps): add pre-commit to dev dependency ([`3a2fccd`](https://github.com/kmnhan/erlabpy/commit/3a2fccd978d23d806d2088ebd9ef60c7a2b20902))
+
+* chore: make csaps optional ([`db31b06`](https://github.com/kmnhan/erlabpy/commit/db31b064c1f46edef7743fdd1c3ab7984e170b3c))
+
+* chore: update issue templates ([`dfc2ab0`](https://github.com/kmnhan/erlabpy/commit/dfc2ab0fdfcf1fd5ab83dac2c9d6473b4d2cb7e1))
+
+### Ci
+
+* ci(github): remove linting, let pre-commit handle it ([`b209ecb`](https://github.com/kmnhan/erlabpy/commit/b209ecbb3c0a35d2bbeba8155bea3da9ffa58fe1))
+
+* ci(pre-commit): add hooks ([`9b401c3`](https://github.com/kmnhan/erlabpy/commit/9b401c328bb3ff18dddcce40b935afa2b6e2624a))
+
+### Documentation
+
+* docs: rephrase kconv guide ([`dd2c022`](https://github.com/kmnhan/erlabpy/commit/dd2c022e42e692c2af640a1fc8d21c3e429781b2))
+
+* docs: add ipykernel dependency to resolve failing builds ([`e5774a5`](https://github.com/kmnhan/erlabpy/commit/e5774a51c14ef6df190eb9f6198c274d2061cdd5))
+
+* docs: add hvplot example ([`6997020`](https://github.com/kmnhan/erlabpy/commit/69970208ba6658f15e900ee6b9367177fcd86d29))
+
+### Fix
+
+* fix: remove all pypi dependencies from pyproject.toml ([`1b2fd55`](https://github.com/kmnhan/erlabpy/commit/1b2fd5594f00bba8367419cd00919eba45cde5a7))
+
+### Refactor
+
+* refactor: remove ktool_old ([`18ea072`](https://github.com/kmnhan/erlabpy/commit/18ea0723fdf538bdbf2789ca73b2b962839ca3e5))
+
+### Style
+
+* style: apply ruff to deprecated imagetools ([`b2c7596`](https://github.com/kmnhan/erlabpy/commit/b2c7596ed12d89edaa2be3fe2923388014c68007))
+
+* style: apply pre-commit fixes ([`12b6441`](https://github.com/kmnhan/erlabpy/commit/12b6441419ed6c4ff4da921790c57a599032dba7))
+
+
 ## v1.6.0 (2024-04-02)
 
 ### Ci
 
 * ci: speedup tests ([`618851e`](https://github.com/kmnhan/erlabpy/commit/618851e74d94301ec4f85a46facd46d3b6272571))
 
 * ci: parallelize tests ([`232301a`](https://github.com/kmnhan/erlabpy/commit/232301a0ab26c9c32a355af11b5458395a1cd832))
```

### Comparing `erlab-1.6.0/LICENSE` & `erlab-1.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `erlab-1.6.0/PKG-INFO` & `erlab-1.6.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: erlab
-Version: 1.6.0
+Version: 1.6.1
 Summary: Python package for ARPES data analysis and visualization.
 Author-email: Kimoon Han <khan@kaist.ac.kr>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -699,31 +699,30 @@
 Requires-Dist: numbagg
 Requires-Dist: numba-progress
 Requires-Dist: joblib
 Requires-Dist: scipy>=1.8.0
 Requires-Dist: lmfit>=1.2.0
 Requires-Dist: uncertainties>=3.0.1
 Requires-Dist: iminuit>=2.25.2
-Requires-Dist: csaps
 Requires-Dist: matplotlib>=3.8.0
 Requires-Dist: xarray
 Requires-Dist: h5netcdf
 Requires-Dist: varname
 Requires-Dist: tqdm
 Requires-Dist: pyperclip
-Requires-Dist: pyqt6>=6.2.2
 Requires-Dist: qtpy
 Requires-Dist: pyqtgraph>=0.13.1
 Requires-Dist: qtawesome
 Requires-Dist: superqt
 Requires-Dist: importlib-metadata; python_version >= "3.11"
 Provides-Extra: dev
 Requires-Dist: pytest; extra == "dev"
 Requires-Dist: python-semantic-release; extra == "dev"
 Requires-Dist: ruff; extra == "dev"
+Requires-Dist: pre-commit; extra == "dev"
 
 # ERLabPy
 [![Supported Python Versions](https://img.shields.io/pypi/pyversions/erlab)](https://pypi.org/project/erlab/)
 [![PyPi](https://img.shields.io/pypi/v/erlab.svg)](https://pypi.org/project/erlab/)
 [![Workflow Status](https://github.com/kmnhan/erlabpy/actions/workflows/release.yml/badge.svg)](https://github.com/kmnhan/erlabpy/actions/workflows/release.yml)
 [![Documentation Status](https://readthedocs.org/projects/erlabpy/badge/)](https://erlabpy.readthedocs.io/)
 [![License](https://img.shields.io/pypi/l/erlab)](https://github.com/kmnhan/erlabpy/blob/main/LICENSE)
```

### Comparing `erlab-1.6.0/PythonInterface.ipf` & `erlab-1.6.1/PythonInterface.ipf`

 * *Files 8% similar despite different names*

```diff
@@ -12,47 +12,46 @@
 
 Menu "Load Waves"
 	"Load ERLabPy HDF5...", /Q, LoadPythonArray()
 End
 
 Function LoadPythonArray([outName, pathName, fileName])
 	// Load .h5 files saved from python
-	
+
 	String outName	 // Name of loaded wave
 	String pathName	 // Name of symbolic path
 	String fileName	 // Name of HDF5 file
-	
+
 	if( ParamIsDefault(pathName) )
 		pathName = ""
 	endif
-	
+
 	if( ParamIsDefault(fileName) )
 		fileName = ""
 	endif
-	
+
 	Variable fileID	// HDF5 file ID will be stored here
-	
+
 	// Open the HDF5 file.
 	HDF5OpenFile /P=$pathName /R fileID as fileName
-	
+
 	// Load the HDF5 dataset.
 	HDF5LoadData /O /Q /IGOR=-1 fileID, "__xarray_dataarray_variable__"
-	
+
 	// Close the HDF5 file.
 	HDF5CloseFile fileID
-	
+
 	if( ParamIsDefault(outName) )
 		outName = RemoveEnding(S_fileName, ".h5")
 		Prompt outName, "Name: "
 		DoPrompt "Enter Wave Name", outName
 		if (V_Flag)
       	return -1
 		endif
 	endif
-	
+
 	// Rename the loaded wave.
 	Duplicate /O '__xarray_dataarray_variable__', $outName; KillWaves '__xarray_dataarray_variable__'
-	
+
 	Print "Loaded Python DataArray as " + outName + " from " + S_path + S_fileName
-	
-End
 
+End
```

### Comparing `erlab-1.6.0/README.md` & `erlab-1.6.1/README.md`

 * *Files identical despite different names*

### Comparing `erlab-1.6.0/docs/Makefile` & `erlab-1.6.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `erlab-1.6.0/docs/environment.yml` & `erlab-1.6.1/docs/environment.yml`

 * *Files 15% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 name: erlabrtd
 channels:
   - conda-forge
 dependencies:
   - python>=3.11
   - pip>=19.3
+  - ipykernel
   - numpy>=1.22.0
   - matplotlib>=3.8.0
+  - hvplot
   - xarray
   - h5netcdf
   - varname
   - numba>=0.56.2
   - numbagg
   - numba-progress
   - joblib
```

### Comparing `erlab-1.6.0/docs/make.bat` & `erlab-1.6.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `erlab-1.6.0/docs/requirements.txt` & `erlab-1.6.1/docs/requirements.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,21 @@
+ipykernel
 sphinx
 sphinx-autodoc-typehints
 setuptools
 nbsphinx
 furo
 sphinx-design
 sphinx-qt-documentation
 sphinx-copybutton
 sphinxcontrib-bibtex
 pybtex
 numpy>=1.22.0
 matplotlib>=3.8.0
+hvplot
 xarray
 h5netcdf
 varname
 numba>=0.56.2
 numbagg
 numba-progress
 joblib
```

### Comparing `erlab-1.6.0/docs/source/conf.py` & `erlab-1.6.1/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `erlab-1.6.0/docs/source/development.rst` & `erlab-1.6.1/docs/source/development.rst`

 * *Files 1% similar despite different names*

```diff
@@ -9,29 +9,29 @@
   `Contributing to xarray
   <https://docs.xarray.dev/en/stable/contributing.html>`_.
 
 
 Creating a development environment
 ==================================
 
-First, you will need to install `git` and `conda` (or `mamba`). 
+First, you will need to install `git` and `conda` (or `mamba`).
 
 Installing git
 --------------
 
 Below are some quick instructions for installing git on various operating systems. For more detailed instructions, see the `git installation guide <https://git-scm.com/book/en/v2/Getting-Started-Installing-Git>`_.
 
-* macOS (Intel & ARM): get Xcode Command Line Tools by running in your terminal window: 
+* macOS (Intel & ARM): get Xcode Command Line Tools by running in your terminal window:
 
   .. code-block:: sh
 
       xcode-select --install
 
 * Windows 10 1709 (build 16299) or later: run in command prompt or PowerShell:
-  
+
   .. code-block:: sh
 
       winget install --id Git.Git -e --source winget
 
 If you are new to contributing to projects through forking on GitHub, take a
 look at the `GitHub documentation for contributing to projects
 <https://docs.github.com/en/get-started/quickstart/contributing-to-projects>`_.
@@ -48,15 +48,15 @@
 
 Cloning the repository
 ----------------------
 
 1. `Create an account <https://github.com/>`_ on GitHub if you do not already
    have one.
 
-2. You will need your own copy of erlabpy (aka fork) to work on the code. 
+2. You will need your own copy of erlabpy (aka fork) to work on the code.
    Go to the `erlabpy repository <https://github.com/kmnhan/erlabpy>`_ and hit
    the ``Fork`` button near the top of the page. This creates a copy of the code
    under your account on the GitHub server.
 
 3. Clone your fork to your machine::
 
     git clone https://github.com/your-user-name/erlabpy.git
@@ -75,15 +75,15 @@
 Before starting any development, you'll need to create an isolated environment
 under a package manager like conda. If you don't have conda installed, `install
 conda <https://docs.conda.io/projects/conda/en/stable/user-guide/install/>`_ or
 `install mamba
 <https://mamba.readthedocs.io/en/latest/installation/mamba-installation.html>`_.
 
 .. hint::
-  
+
   - When using conda, miniconda is recommended to save disk space.
   - `Mamba <https://mamba.readthedocs.io>`_ is a faster alternative
     to conda with additional features.
   - Installing `miniforge <https://github.com/conda-forge/miniforge>`_ will
     install both conda and mamba, and is recommended.
 
 Editable installation from source
@@ -98,28 +98,28 @@
 1. Create and activate a mamba (or conda) environment.
 
    .. note::
 
      Replace :code:`<envname>`  with the environment name you prefer.
 
    .. hint::
-      
+
      | If using conda, replace :code:`mamba` with :code:`conda`.
-     | If on Apple silicon, replace :code:`environment.yml` with :code:`environment_apple.yml` to use `Accelerate <https://developer.apple.com/accelerate/>`_ instead of `OpenBLAS <https://en.wikipedia.org/wiki/OpenBLAS>`_. 
+     | If on Apple silicon, replace :code:`environment.yml` with :code:`environment_apple.yml` to use `Accelerate <https://developer.apple.com/accelerate/>`_ instead of `OpenBLAS <https://en.wikipedia.org/wiki/OpenBLAS>`_.
 
    .. code-block:: sh
 
      mamba env create -f environment.yml -n <envname>
      mamba activate <envname>
 
 
 2. Install the repository.
-   
+
    .. note::
-    
+
       The ``editable_mode=compat`` setting enables static analysis tools to work with
       the package. See `this issue <https://github.com/pypa/setuptools/issues/3518>`_
       for more information.
 
    .. code-block:: sh
 
      pip install -e . --config-settings editable_mode=compat
@@ -169,15 +169,15 @@
     git merge upstream/main
 
 This will combine your commits with the latest *erlabpy* git ``main``. If this
 leads to merge conflicts, you must resolve these before submitting your pull
 request. Remember to follow the commit message guidelines. If you have
 uncommitted changes, you will need to ``git stash`` them prior to updating. This
 will effectively store your changes, which can be reapplied after updating with
-``git stash apply``. 
+``git stash apply``.
 
 
 Create a new feature branch
 ---------------------------
 
 Create a branch to save your changes, even before you start making changes. You
 want your ``main branch`` to contain only production-ready code::
@@ -331,15 +331,15 @@
 or
 
 .. code-block:: sh
 
     mamba env update -f docs/environment.yml -n <envname>
 
 then build the documentation by running:
-  
+
 .. code-block:: sh
 
     cd docs/
     make clean
     make html
 
 Then you can find the HTML output files in the folder
```

### Comparing `erlab-1.6.0/docs/source/getting-started.rst` & `erlab-1.6.1/docs/source/getting-started.rst`

 * *Files 8% similar despite different names*

```diff
@@ -58,10 +58,37 @@
     * - `matplotlib <https://matplotlib.org>`_
       - Plotting
     * - `scipy <https://docs.scipy.org/doc/scipy/index.html>`_
       - Linear algebra, signal processing, and image processing
     * - `lmfit <https://lmfit.github.io/lmfit-py/>`_
       - Optimization problems including curve fitting
     * - `pyqtgraph <https://pyqtgraph.readthedocs.io/en/latest/>`_
-      - Interactive plotting (i.e., imagetool) 
+      - Interactive plotting (i.e., imagetool)
 
-See the :doc:`userguide` to start using ERLabPy!
+For the full list of dependencies, see the `requirements.txt` file.
+
+See the :doc:`userguide` to start using ERLabPy!
+
+
+Optional dependencies
+---------------------
+
+The following packages are optional dependencies that are not installed by
+default. They are used in only specific functions, or is not used at all but is
+listed just for convenience.
+
+.. list-table::
+    :header-rows: 1
+    :stub-columns: 1
+    :widths: auto
+
+    * - Package
+      - Description
+    * - `csaps <https://github.com/espdev/csaps>`_
+      - Multidimensional smoothing splines
+    * - `hvplot <https://github.com/holoviz/hvplot>`_ and `bokeh
+        <https://github.com/bokeh/bokeh>`_
+      - Interactive plotting
+    * - `cmasher <https://cmasher.readthedocs.io>`_,
+        `cmocean <https://matplotlib.org/cmocean/>`_, and
+        `colorcet <https://colorcet.holoviz.org>`_
+      - More colormaps!
```

### Comparing `erlab-1.6.0/docs/source/images/imagetool_dark.png` & `erlab-1.6.1/docs/source/images/imagetool_dark.png`

 * *Files identical despite different names*

### Comparing `erlab-1.6.0/docs/source/images/imagetool_light.png` & `erlab-1.6.1/docs/source/images/imagetool_light.png`

 * *Files identical despite different names*

### Comparing `erlab-1.6.0/docs/source/images/ktool_1_dark.png` & `erlab-1.6.1/docs/source/images/ktool_1_dark.png`

 * *Files identical despite different names*

### Comparing `erlab-1.6.0/docs/source/images/ktool_1_light.png` & `erlab-1.6.1/docs/source/images/ktool_1_light.png`

 * *Files identical despite different names*

### Comparing `erlab-1.6.0/docs/source/images/ktool_2_dark.png` & `erlab-1.6.1/docs/source/images/ktool_2_dark.png`

 * *Files identical despite different names*

### Comparing `erlab-1.6.0/docs/source/images/ktool_2_light.png` & `erlab-1.6.1/docs/source/images/ktool_2_light.png`

 * *Files identical despite different names*

### Comparing `erlab-1.6.0/docs/source/index.rst` & `erlab-1.6.1/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `erlab-1.6.0/docs/source/notebooks/indexing.ipynb` & `erlab-1.6.1/docs/source/notebooks/indexing.ipynb`

 * *Files identical despite different names*

### Comparing `erlab-1.6.0/docs/source/notebooks/io.ipynb` & `erlab-1.6.1/docs/source/notebooks/io.ipynb`

 * *Files identical despite different names*

### Comparing `erlab-1.6.0/docs/source/notebooks/kconv.ipynb` & `erlab-1.6.1/docs/source/notebooks/kconv.ipynb`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9984482429335371%*

 * *Differences: {"'cells'": "{0: {'source': {insert: [(10, 'Momentum conversion in ERLabPy follows the "*

 * *            'nomenclature from :cite:t:`Ishida2018`. All experimental geometry are classified into '*

 * *            "4 types. Definition of angles differ for each geometry.\\n'), (12, 'For instance, "*

 * *            'image a typical Type 1 setup with a vertical slit that acquires maps by rotating '*

 * *            'about the `z` axis in the lab frame. In this case, the polar angle (rotation about '*

 * *            "`z`) is :math:`β`, […]*

```diff
@@ -17,17 +17,19 @@
                 "Momentum conversion in ERLabPy is exact with no small angle approximation, but\n",
                 "is also very fast, thanks to the numba-accelerated trilinear interpolation in\n",
                 ":mod:`erlab.analysis.interpolate`\\ .\n",
                 "\n",
                 "Nomenclature\n",
                 "------------\n",
                 "\n",
-                "Momentum conversion in ERLabPy follows the nomenclature from :cite:t:`Ishida2018`. All experimental geometry are classified into one of 4 types, and the definition of angles differ for each geometry.\n",
+                "Momentum conversion in ERLabPy follows the nomenclature from :cite:t:`Ishida2018`. All experimental geometry are classified into 4 types. Definition of angles differ for each geometry.\n",
                 "\n",
-                "For instance, image a typical Type 1 setup with a vertical slit that acquires maps by rotating about the `z` axis in the lab frame. In this case, the polar angle (rotation about `z`) is :math:`\u03b2`, and the tilt angle is :math:`\u03be`.In all cases, :math:`\u03b4` is the azimuthal angle that indicates in-plane rotation, and :math:`\u03b1` is the angle along the slit."
+                "For instance, image a typical Type 1 setup with a vertical slit that acquires maps by rotating about the `z` axis in the lab frame. In this case, the polar angle (rotation about `z`) is :math:`\u03b2`, and the tilt angle is :math:`\u03be`.\n",
+                "\n",
+                "In all cases, :math:`\u03b4` is the azimuthal angle that indicates in-plane rotation, and :math:`\u03b1` is the angle along the slit."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 1,
             "metadata": {
                 "editable": true,
@@ -1272,15 +1274,15 @@
                 "raw_mimetype": "text/restructuredtext",
                 "slideshow": {
                     "slide_type": ""
                 },
                 "tags": []
             },
             "source": [
-                "Although the functions for momentum conversion are in :mod:`erlab.analysis.kspace`\\ , the actual conversion is implemented as an `xarray accessor <https://docs.xarray.dev/en/stable/internals/extending-xarray.html>`_. Let's see how it works.\n",
+                "Although the functions for momentum conversion are implemented in :mod:`erlab.analysis.kspace`\\ , the actual conversion is performed using an `xarray accessor <https://docs.xarray.dev/en/stable/internals/extending-xarray.html>`_. Let's see how it works.\n",
                 "\n",
                 "Converting to momentum space\n",
                 "----------------------------\n",
                 "\n",
                 "Momentum conversion is done by the :meth:`convert <erlab.accessors.MomentumAccessor.convert>` method of the ``kspace`` accessor. The bounds and resolution are automatically determined from the data if no input is provided. The method returns a new DataArray in momentum space."
             ]
         },
@@ -2704,15 +2706,15 @@
                 "dat.kspace.offsets"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "Since we haven't set any offsets, they are all set to zero. We will set the azimuthal angle to 60 degrees and the polar offset to 30 degrees and see what happens."
+                "Since we haven't set any offsets, they are all zero. We will set the azimuthal angle to 60 degrees and the polar offset to 30 degrees and see what happens."
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 8,
             "metadata": {},
             "outputs": [
```

### Comparing `erlab-1.6.0/docs/source/pyplots/norms.py` & `erlab-1.6.1/docs/source/pyplots/norms.py`

 * *Files identical despite different names*

### Comparing `erlab-1.6.0/docs/source/reference.rst` & `erlab-1.6.1/docs/source/reference.rst`

 * *Files 10% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 `erlab.characterization`   Analyze sample characterization results such as XRD and transport measurements
 ========================   ========================
 
 .. currentmodule:: erlab
 
 .. toctree::
    :hidden:
-   
+
    erlab.analysis
    erlab.io
    erlab.plotting
    erlab.interactive
    erlab.characterization
 
 Submodules
@@ -38,12 +38,12 @@
 `erlab.constants`   Physical constants and unit conversion
 `erlab.accessors`   `xarray accessors <https://docs.xarray.dev/en/stable/internals/extending-xarray.html>`_
 `erlab.parallel`    Helpers for parallel processing
 ==================  ==================
 
 .. toctree::
    :hidden:
-   
+
    erlab.lattice
    erlab.constants
    erlab.accessors
-   erlab.parallel
+   erlab.parallel
```

### Comparing `erlab-1.6.0/docs/source/refs.bib` & `erlab-1.6.1/docs/source/refs.bib`

 * *Files identical despite different names*

### Comparing `erlab-1.6.0/docs/source/userguide.rst` & `erlab-1.6.1/docs/source/userguide.rst`

 * *Files 8% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 **********
 
 .. admonition:: Work in Progress
    :class: warning
 
    The user guide is incomplete. For the full list of packages and modules provided by ERLabPy, see :doc:`reference`.
 
-This section contains some examples for getting started with ARPES data analysis and visualization. 
+This section contains some examples for getting started with ARPES data analysis and visualization.
 
 
 Introduction
 ============
 
 The following documentation assumes basic python programming experience.
```

### Comparing `erlab-1.6.0/environment.yml` & `erlab-1.6.1/environment.yml`

 * *Files 2% similar despite different names*

```diff
@@ -44,10 +44,9 @@
   - qtawesome
   - numbagg
   - numba-progress
   - iminuit>=2.3
   - pyperclip
   - pip:
     - pyqt6>=6.2.2
-    - csaps
     - igor2 @ git+https://github.com/kmnhan/igor2@master
-    - arpes @ git+https://github.com/kmnhan/arpes@master
+    - arpes @ git+https://github.com/kmnhan/arpes@master
```

### Comparing `erlab-1.6.0/environment_apple.yml` & `erlab-1.6.1/environment_apple.yml`

 * *Files 11% similar despite different names*

```diff
@@ -48,10 +48,9 @@
   - qtawesome
   - numbagg
   - numba-progress
   - iminuit>=2.3
   - pyperclip
   - pip:
     - pyqt6>=6.2.2
-    - csaps
     - igor2 @ git+https://github.com/kmnhan/igor2@master
-    - arpes @ git+https://github.com/kmnhan/arpes@master
+    - arpes @ git+https://github.com/kmnhan/arpes@master
```

### Comparing `erlab-1.6.0/environment_nogit.yml` & `erlab-1.6.1/environment_nogit.yml`

 * *Files 1% similar despite different names*

```diff
@@ -48,8 +48,7 @@
   - qtawesome
   - numbagg
   - numba-progress
   - iminuit>=2.3
   - pyperclip
   - pip:
     - pyqt6>=6.2.2
-    - csaps
```

### Comparing `erlab-1.6.0/environment_nogit_mkl.yml` & `erlab-1.6.1/environment_nogit_mkl.yml`

 * *Files 15% similar despite different names*

```diff
@@ -48,8 +48,7 @@
   - qtawesome
   - numbagg
   - numba-progress
   - iminuit>=2.3
   - pyperclip
   - pip:
     - pyqt6>=6.2.2
-    - csaps
```

### Comparing `erlab-1.6.0/pyproject.toml` & `erlab-1.6.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -26,22 +26,20 @@
     "numbagg",
     "numba-progress",
     "joblib",
     "scipy>=1.8.0",
     "lmfit>=1.2.0",
     "uncertainties>=3.0.1",
     "iminuit>=2.25.2",
-    "csaps",
     "matplotlib>=3.8.0",
     "xarray",
     "h5netcdf",
     "varname",
     "tqdm",
     "pyperclip",
-    "pyqt6>=6.2.2",
     "qtpy",
     "pyqtgraph>=0.13.1",
     "qtawesome",
     "superqt",
     'importlib-metadata; python_version>="3.11"',
 ]
 dynamic = ["version"]
@@ -49,15 +47,15 @@
 [project.urls]
 Documentation = "https://erlabpy.readthedocs.io"
 Repository = "https://github.com/kmnhan/erlabpy.git"
 Issues = "https://github.com/kmnhan/erlabpy/issues"
 Changelog = "https://github.com/kmnhan/erlabpy/blob/main/CHANGELOG.md"
 
 [project.optional-dependencies]
-dev = ["pytest", "python-semantic-release", "ruff"]
+dev = ["pytest", "python-semantic-release", "ruff", "pre-commit"]
 
 [tool.setuptools]
 package-dir = { "" = "src" }
 
 [tool.setuptools.dynamic]
 version = { attr = "erlab.__version__" }
 
@@ -156,15 +154,14 @@
     "_build",
     "buck-out",
     "build",
     "dist",
     "node_modules",
     "site-packages",
     "venv",
-    "_deprecated",
 ]
 
 [tool.ruff.lint]
 select = [
     "E4",
     "E7",
     "E9",
```

### Comparing `erlab-1.6.0/src/erlab/accessors.py` & `erlab-1.6.1/src/erlab/accessors.py`

 * *Files identical despite different names*

### Comparing `erlab-1.6.0/src/erlab/analysis/__init__.py` & `erlab-1.6.1/src/erlab/analysis/__init__.py`

 * *Files identical despite different names*

### Comparing `erlab-1.6.0/src/erlab/analysis/correlation.py` & `erlab-1.6.1/src/erlab/analysis/correlation.py`

 * *Files identical despite different names*

### Comparing `erlab-1.6.0/src/erlab/analysis/fit/functions/__init__.py` & `erlab-1.6.1/src/erlab/analysis/fit/functions/__init__.py`

 * *Files identical despite different names*

### Comparing `erlab-1.6.0/src/erlab/analysis/fit/functions/dynamic.py` & `erlab-1.6.1/src/erlab/analysis/fit/functions/dynamic.py`

 * *Files identical despite different names*

### Comparing `erlab-1.6.0/src/erlab/analysis/fit/functions/general.py` & `erlab-1.6.1/src/erlab/analysis/fit/functions/general.py`

 * *Files identical despite different names*

### Comparing `erlab-1.6.0/src/erlab/analysis/fit/minuit.py` & `erlab-1.6.1/src/erlab/analysis/fit/minuit.py`

 * *Files identical despite different names*

### Comparing `erlab-1.6.0/src/erlab/analysis/fit/models.py` & `erlab-1.6.1/src/erlab/analysis/fit/models.py`

 * *Files identical despite different names*

### Comparing `erlab-1.6.0/src/erlab/analysis/fit/spline.py` & `erlab-1.6.1/src/erlab/analysis/fit/spline.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,17 @@
-import csaps
 import xarray as xr
 
+try:
+    import csaps
+except ImportError as e:
+    raise ImportError(
+        "The `csaps` package is required for this module. "
+        "Please install it using `pip install csaps`."
+    ) from e
+
 
 def xcsaps(
     arr: xr.DataArray, **kwargs: dict
 ) -> tuple[xr.DataArray, csaps.ISmoothingSpline]:
     """`xarray` compatible `csaps.csaps`.
 
     Parameters
```

### Comparing `erlab-1.6.0/src/erlab/analysis/gold.py` & `erlab-1.6.1/src/erlab/analysis/gold.py`

 * *Files identical despite different names*

### Comparing `erlab-1.6.0/src/erlab/analysis/interpolate.py` & `erlab-1.6.1/src/erlab/analysis/interpolate.py`

 * *Files identical despite different names*

### Comparing `erlab-1.6.0/src/erlab/analysis/kspace.py` & `erlab-1.6.1/src/erlab/analysis/kspace.py`

 * *Files identical despite different names*

### Comparing `erlab-1.6.0/src/erlab/analysis/mask/__init__.py` & `erlab-1.6.1/src/erlab/analysis/mask/__init__.py`

 * *Files identical despite different names*

### Comparing `erlab-1.6.0/src/erlab/analysis/mask/polygon.py` & `erlab-1.6.1/src/erlab/analysis/mask/polygon.py`

 * *Files identical despite different names*

### Comparing `erlab-1.6.0/src/erlab/analysis/transform.py` & `erlab-1.6.1/src/erlab/analysis/transform.py`

 * *Files identical despite different names*

### Comparing `erlab-1.6.0/src/erlab/analysis/utilities.py` & `erlab-1.6.1/src/erlab/analysis/utilities.py`

 * *Files identical despite different names*

### Comparing `erlab-1.6.0/src/erlab/characterization/resistance.py` & `erlab-1.6.1/src/erlab/characterization/resistance.py`

 * *Files identical despite different names*

### Comparing `erlab-1.6.0/src/erlab/characterization/xrd.py` & `erlab-1.6.1/src/erlab/characterization/xrd.py`

 * *Files identical despite different names*

### Comparing `erlab-1.6.0/src/erlab/constants.py` & `erlab-1.6.1/src/erlab/constants.py`

 * *Files identical despite different names*

### Comparing `erlab-1.6.0/src/erlab/interactive/__init__.py` & `erlab-1.6.1/src/erlab/interactive/__init__.py`

 * *Files identical despite different names*

### Comparing `erlab-1.6.0/src/erlab/interactive/bzplot.py` & `erlab-1.6.1/src/erlab/interactive/bzplot.py`

 * *Files identical despite different names*

### Comparing `erlab-1.6.0/src/erlab/interactive/colors.py` & `erlab-1.6.1/src/erlab/interactive/colors.py`

 * *Files identical despite different names*

### Comparing `erlab-1.6.0/src/erlab/interactive/curvefittingtool.py` & `erlab-1.6.1/src/erlab/interactive/curvefittingtool.py`

 * *Files identical despite different names*

### Comparing `erlab-1.6.0/src/erlab/interactive/derivative.py` & `erlab-1.6.1/src/erlab/interactive/derivative.py`

 * *Files identical despite different names*

### Comparing `erlab-1.6.0/src/erlab/interactive/exampledata.py` & `erlab-1.6.1/src/erlab/interactive/exampledata.py`

 * *Files identical despite different names*

### Comparing `erlab-1.6.0/src/erlab/interactive/fermiedge.py` & `erlab-1.6.1/src/erlab/interactive/fermiedge.py`

 * *Files identical despite different names*

### Comparing `erlab-1.6.0/src/erlab/interactive/imagetool/__init__.py` & `erlab-1.6.1/src/erlab/interactive/imagetool/__init__.py`

 * *Files identical despite different names*

### Comparing `erlab-1.6.0/src/erlab/interactive/imagetool/_deprecated/imagetool_mpl.py` & `erlab-1.6.1/src/erlab/interactive/imagetool/_deprecated/imagetool_mpl.py`

 * *Files 3% similar despite different names*

```diff
@@ -75,18 +75,18 @@
     return val[(slice(None),) * (axis % a.ndim) + (slice(w, -1),)]
 
 
 def move_mean_centered_multiaxis(
     a,
     window_list,
     min_count_list=None,
-    axis_list=[
-        -1,
-    ],
+    axis_list=None,
 ):
+    if axis_list is None:
+        axis_list = [-1]
     if not isinstance(axis_list, list):
         axis_list = [
             axis_list,
         ]
     w_list = [(window - 1) // 2 for window in window_list]
     pad_width = [(0, 0)] * a.ndim
     slicer = [
@@ -254,19 +254,25 @@
         data,
         snap=False,
         gamma=0.5,
         cmap="magma",
         useblit=True,
         parallel=False,
         bench=False,
-        cursorprops={},
-        lineprops={},
-        fermilineprops={},
+        cursorprops=None,
+        lineprops=None,
+        fermilineprops=None,
         **improps,
     ):
+        if fermilineprops is None:
+            fermilineprops = {}
+        if lineprops is None:
+            lineprops = {}
+        if cursorprops is None:
+            cursorprops = {}
         self.canvas = canvas
         self.axes = axes
         self.data = parse_data(data)
         self.snap = snap
         self.gamma = gamma
         self.cmap = cmap
         self.useblit = useblit
@@ -275,66 +281,66 @@
 
         if self.useblit and not self.canvas.supports_blit:
             raise RuntimeError(
                 "Canvas does not support blit. "
                 "If running in ipython, add `%matplotlib qt`."
             )
         for ax in self.axes:
-            for loc, spine in ax.spines.items():
+            for _loc, spine in ax.spines.items():
                 spine.set_position(("outward", 1))
         self.cursorprops = cursorprops
         self.lineprops = lineprops
         self.fermilineprops = fermilineprops
         self.improps = improps
         self.cursorprops.update(
-            dict(
-                linestyle="-",
-                linewidth=0.8,
-                color=colors.to_rgba(plt.rcParams.get("axes.edgecolor"), alpha=0.5),
-                animated=self.useblit,
-                visible=True,
-            )
+            {
+                "linestyle": "-",
+                "linewidth": 0.8,
+                "color": colors.to_rgba(plt.rcParams.get("axes.edgecolor"), alpha=0.5),
+                "animated": self.useblit,
+                "visible": True,
+            }
         )
         self.lineprops.update(
-            dict(
-                linestyle="-",
-                linewidth=0.8,
-                color=colors.to_rgba(plt.rcParams.get("axes.edgecolor"), alpha=1),
-                animated=self.useblit,
-                visible=True,
-            )
+            {
+                "linestyle": "-",
+                "linewidth": 0.8,
+                "color": colors.to_rgba(plt.rcParams.get("axes.edgecolor"), alpha=1),
+                "animated": self.useblit,
+                "visible": True,
+            }
         )
         self.fermilineprops.update(
-            dict(
-                linestyle="--",
-                linewidth=0.8,
-                color=colors.to_rgba(plt.rcParams.get("axes.edgecolor"), alpha=1),
-                animated=False,
-            )
+            {
+                "linestyle": "--",
+                "linewidth": 0.8,
+                "color": colors.to_rgba(plt.rcParams.get("axes.edgecolor"), alpha=1),
+                "animated": False,
+            }
         )
         self.improps.update(
-            dict(
-                animated=self.useblit,
-                visible=True,
-                interpolation="none",
-                aspect="auto",
-                origin="lower",
-                norm=colors.PowerNorm(self.gamma),
-                cmap=self.cmap,
-                rasterized=True,
-            )
+            {
+                "animated": self.useblit,
+                "visible": True,
+                "interpolation": "none",
+                "aspect": "auto",
+                "origin": "lower",
+                "norm": colors.PowerNorm(self.gamma),
+                "cmap": self.cmap,
+                "rasterized": True,
+            }
         )
-        self.spanprops = dict(
+        self.spanprops = {
             # edgecolor=plt.rcParams.get('axes.edgecolor'),
             # lw=0.5, ls='--',
-            facecolor=colors.to_rgba(self.cursorprops["color"], alpha=1),
-            alpha=0.15,
-            animated=self.useblit,
-            visible=True,
-        )
+            "facecolor": colors.to_rgba(self.cursorprops["color"], alpha=1),
+            "alpha": 0.15,
+            "animated": self.useblit,
+            "visible": True,
+        }
         self._get_middle_index = lambda x: len(x) // 2 - (1 if len(x) % 2 == 0 else 0)
 
         self.vals = self.data.values
 
         self.ndim = self.data.ndim
         self._assign_vals_T()
         self.avg_win = [
@@ -720,25 +726,25 @@
                 for span in self.spans[axis]:
                     span.set_visible(False)
         for ax in self.scaling_axes:
             ax.set_ticks([])
 
     def labelify(self, dim):
         """Prettify some frequently used axis labels."""
-        labelformats = dict(
-            kx="$k_x$",
-            ky="$k_y$",
-            kz="$k_z$",
-            alpha="$\\alpha$",
-            beta="$\\beta$",
-            theta="$\\theta$",
-            phi="$\\phi$",
-            chi="$\\chi$",
-            eV="$E$",
-        )
+        labelformats = {
+            "kx": "$k_x$",
+            "ky": "$k_y$",
+            "kz": "$k_z$",
+            "alpha": "$\\alpha$",
+            "beta": "$\\beta$",
+            "theta": "$\\theta$",
+            "phi": "$\\phi$",
+            "chi": "$\\chi$",
+            "eV": "$E$",
+        }
         try:
             return labelformats[dim]
         except KeyError:
             return dim
 
     def onpress(self, event):
         if event.key == "shift":
@@ -1041,37 +1047,37 @@
 
     def _icon(self, name):
         """
         Construct a `.QIcon` from an image file *name*, including the extension
         and relative to Matplotlib's "images" data directory.
         """
         name = name.replace(".png", "")
-        icons_dict = dict(
+        icons_dict = {
             # back = qta.icon('ph.arrow-arc-left-fill'),
             # forward = qta.icon('ph.arrow-arc-right-fill'),
             # filesave = qta.icon('ph.floppy-disk-fill'),
             # home = qta.icon('ph.corners-out-fill'),
             # move = qta.icon('ph.arrows-out-cardinal-fill'),
             # qt4_editor_options = qta.icon('ph.palette-fill'),
             # zoom_to_rect = qta.icon('ph.crop-fill'),
             # subplots = qta.icon('ph.squares-four-fill'),
-            back=qta.icon("msc.chevron-left"),
-            forward=qta.icon("msc.chevron-right"),
-            filesave=qta.icon("msc.save"),
-            home=qta.icon("msc.debug-step-back"),
-            move=qta.icon("msc.move"),
-            qt4_editor_options=qta.icon("msc.graph-line"),
-            zoom_to_rect=qta.icon("msc.search"),
-            subplots=qta.icon("msc.editor-layout"),
-        )
+            "back": qta.icon("msc.chevron-left"),
+            "forward": qta.icon("msc.chevron-right"),
+            "filesave": qta.icon("msc.save"),
+            "home": qta.icon("msc.debug-step-back"),
+            "move": qta.icon("msc.move"),
+            "qt4_editor_options": qta.icon("msc.graph-line"),
+            "zoom_to_rect": qta.icon("msc.search"),
+            "subplots": qta.icon("msc.editor-layout"),
+        }
         try:
             return icons_dict[name]
-        except BaseException:
+        except BaseException as e:
             print(name)
-            raise Exception
+            raise Exception from e
         # name = name.replace('.png', '_large.png')
         # pm = QtGui.QPixmap(str(cbook._get_data_path('images', name)))
         # _setDevicePixelRatio(pm, _devicePixelRatioF(self))
         # if self.palette().color(self.backgroundRole()).value() < 128:
         # icon_color = self.palette().color(self.foregroundRole())
         # mask = pm.createMaskFromColor(
         # QtGui.QColor('black'),
@@ -1216,19 +1222,19 @@
         self.NavBar.home = home_new
         self.NavBar.pan = pan_new
         self.NavBar.zoom = zoom_new
         self.addToolBar(
             QtCore.Qt.BottomToolBarArea, self.NavBar(self.main_canvas, self)
         )
 
-        self.icons = dict(
-            swap=qta.icon("msc.arrow-swap"),
-            lock=qta.icon("msc.lock"),
-            unlock=qta.icon("msc.unlock"),
-        )
+        self.icons = {
+            "swap": qta.icon("msc.arrow-swap"),
+            "lock": qta.icon("msc.lock"),
+            "unlock": qta.icon("msc.unlock"),
+        }
 
         self.cursortab = QtWidgets.QWidget()
         cursortab_content = QtWidgets.QHBoxLayout(self.cursortab)
         spinlabels = tuple(
             QtWidgets.QLabel(self.itool.dims[i]) for i in range(self.ndim)
         )
         self._cursor_spin = tuple(
```

### Comparing `erlab-1.6.0/src/erlab/interactive/imagetool/_deprecated/imagetool_old.py` & `erlab-1.6.1/src/erlab/interactive/imagetool/_deprecated/imagetool_old.py`

 * *Files 2% similar despite different names*

```diff
@@ -41,37 +41,37 @@
 
 __all__ = ["itool_", "pg_itool"]
 
 suppressnanwarning = np.testing.suppress_warnings()
 suppressnanwarning.filter(RuntimeWarning, r"All-NaN (slice|axis) encountered")
 
 
-ICON_NAME = dict(
-    invert="mdi6.invert-colors",
-    invert_off="mdi6.invert-colors-off",
-    contrast="mdi6.contrast-box",
-    lock="mdi6.lock",
-    unlock="mdi6.lock-open-variant",
-    colorbar="mdi6.gradient-vertical",
-    transpose_0="mdi6.arrow-left-right",
-    transpose_1="mdi6.arrow-top-left-bottom-right",
-    transpose_2="mdi6.arrow-up-down",
-    transpose_3="mdi6.arrow-up-down",
-    snap="mdi6.grid",
-    snap_off="mdi6.grid-off",
-    palette="mdi6.palette-advanced",
-    styles="mdi6.palette-swatch",
-    layout="mdi6.page-layout-body",
-    zero_center="mdi6.format-vertical-align-center",
-    table_eye="mdi6.table-eye",
-)
+ICON_NAME = {
+    "invert": "mdi6.invert-colors",
+    "invert_off": "mdi6.invert-colors-off",
+    "contrast": "mdi6.contrast-box",
+    "lock": "mdi6.lock",
+    "unlock": "mdi6.lock-open-variant",
+    "colorbar": "mdi6.gradient-vertical",
+    "transpose_0": "mdi6.arrow-left-right",
+    "transpose_1": "mdi6.arrow-top-left-bottom-right",
+    "transpose_2": "mdi6.arrow-up-down",
+    "transpose_3": "mdi6.arrow-up-down",
+    "snap": "mdi6.grid",
+    "snap_off": "mdi6.grid-off",
+    "palette": "mdi6.palette-advanced",
+    "styles": "mdi6.palette-swatch",
+    "layout": "mdi6.page-layout-body",
+    "zero_center": "mdi6.format-vertical-align-center",
+    "table_eye": "mdi6.table-eye",
+}
 
 
 class IconButton(QtWidgets.QPushButton):
-    def __init__(self, *args, on: str = None, off: str = None, **kwargs):
+    def __init__(self, *args, on: str | None = None, off: str | None = None, **kwargs):
         self.icon_key_on = None
         self.icon_key_off = None
         if on is not None:
             self.icon_key_on = on
             kwargs["icon"] = qta.icon(ICON_NAME[self.icon_key_on])
         if off is not None:
             if on is None and kwargs["icon"] is None:
@@ -904,26 +904,37 @@
         self,
         data,
         snap=False,
         gamma=1.0,
         cmap="magma",
         reverse=False,
         bench=False,
-        plot_kw={},
-        cursor_kw={},
-        image_kw={},
-        profile_kw={},
-        span_kw={},
-        fermi_kw={},
+        plot_kw=None,
+        cursor_kw=None,
+        image_kw=None,
+        profile_kw=None,
+        span_kw=None,
+        fermi_kw=None,
         zero_centered=False,
         rad2deg=False,
-        *args,
         **kwargs,
     ):
-        super().__init__(show=True, *args, **kwargs)
+        if fermi_kw is None:
+            fermi_kw = {}
+        if span_kw is None:
+            span_kw = {}
+        if profile_kw is None:
+            profile_kw = {}
+        if image_kw is None:
+            image_kw = {}
+        if cursor_kw is None:
+            cursor_kw = {}
+        if plot_kw is None:
+            plot_kw = {}
+        super().__init__(show=True, **kwargs)
         self.qapp = QtCore.QCoreApplication.instance()
         self.screen = self.qapp.primaryScreen()
         self.snap = snap
         self.gamma = gamma
         self.cmap = cmap
         self.reverse = reverse
         self.bench = bench
@@ -949,44 +960,44 @@
         cursor_c_hover.setAlphaF(0.95)
         span_c.setAlphaF(0.15)
         span_c_edge.setAlphaF(0.35)
         # span_c_hover = pg.mkColor(0.75)
         # span_c_hover.setAlphaF(0.5)
 
         self.cursor_kw.update(
-            dict(
-                pen=pg.mkPen(cursor_c, width=2.25),
-                hoverPen=pg.mkPen(cursor_c_hover, width=2.5),
-            )
+            {
+                "pen": pg.mkPen(cursor_c, width=2.25),
+                "hoverPen": pg.mkPen(cursor_c_hover, width=2.5),
+            }
         )
-        self.plot_kw.update(dict(defaultPadding=0.0, clipToView=False))
+        self.plot_kw.update({"defaultPadding": 0.0, "clipToView": False})
         # self.profile_kw.update(dict(
         #     linestyle='-', linewidth=.8,
         #     color=colors.to_rgba(plt.rcParams.get('axes.edgecolor'),
         #                          alpha=1),
         #     animated=self.useblit, visible=True,
         # ))
         # self.fermi_kw.update(dict(
         #     linestyle='--', linewidth=.8,
         #     color=colors.to_rgba(plt.rcParams.get('axes.edgecolor'),
         #                          alpha=1),
         #     animated=False,
         # ))
         self.image_kw.update(
-            dict(
-                autoDownsample=False,
-                axisOrder="row-major",
-            )
+            {
+                "autoDownsample": False,
+                "axisOrder": "row-major",
+            }
         )
         self.span_kw.update(
-            dict(
-                movable=False,
-                pen=pg.mkPen(span_c_edge, width=1),
-                brush=pg.mkBrush(span_c),
-            )
+            {
+                "movable": False,
+                "pen": pg.mkPen(span_c_edge, width=1),
+                "brush": pg.mkBrush(span_c),
+            }
         )
         # self.cursor_pos = None
         self.data = None
         if rad2deg is not False:
             if np.iterable(rad2deg):
                 conv_dims = rad2deg
             else:
@@ -1335,15 +1346,15 @@
         target = self.axes[axis]
         toggle = False if target in self.ci.items.keys() else True
 
         if self.data_ndim == 2:
             ref_dims = ((1, 0, 1, 1), (0, 0, 1, 1), (1, 1, 1, 1))
             top_left = (1,)
             bottom_right = (2,)
-            top_right = tuple()
+            top_right = ()
         elif self.data_ndim == 3:
             ref_dims = (
                 (2, 0, 1, 1),
                 (0, 0, 1, 1),
                 (2, 2, 1, 1),
                 (0, 1, 2, 2),
                 (1, 0, 1, 1),
@@ -1572,25 +1583,25 @@
         self._fpsLastUpdate = now
         w = 0.8
         self._avg_fps = self._avg_fps * (1 - w) + fps * w
         self.axes[1].setTitle("%0.2f fps" % self._avg_fps)
 
     def labelify(self, text):
         """Prettify some frequently used axis labels."""
-        labelformats = dict(
-            kx="$k_x$",
-            ky="$k_y$",
-            kz="$k_z$",
-            alpha="$\\alpha$",
-            beta="$\\beta$",
-            theta="$\\theta$",
-            phi="$\\phi$",
-            chi="$\\chi$",
-            eV="$E$",
-        )
+        labelformats = {
+            "kx": "$k_x$",
+            "ky": "$k_y$",
+            "kz": "$k_z$",
+            "alpha": "$\\alpha$",
+            "beta": "$\\beta$",
+            "theta": "$\\theta$",
+            "phi": "$\\phi$",
+            "chi": "$\\chi$",
+            "eV": "$E$",
+        }
         try:
             return labelformats[text]
         except KeyError:
             return text
 
     def set_cmap(
         self,
@@ -2428,19 +2439,23 @@
         self,
         itool,
         width=25,
         horiz_pad=45,
         vert_pad=30,
         inner_pad=5,
         font_size=10,
-        curve_kw={},
-        line_kw={"pen": "cyan"},
+        curve_kw=None,
+        line_kw=None,
         *args,
         **kwargs,
     ):
+        if line_kw is None:
+            line_kw = {"pen": "cyan"}
+        if curve_kw is None:
+            curve_kw = {}
         super().__init__(itool, *args, **kwargs)
         self.setDefaultPadding(0)
         self.cbar = ItoolImageItem(self.itool, axisOrder="row-major")
         self.npts = 4096
         self.autolevels = True
 
         self.cbar.setImage(np.linspace(0, 1, self.npts).reshape((-1, 1)))
@@ -3196,15 +3211,15 @@
     # TODO: implement multiple windows, equal aspect settings
     qapp = QtWidgets.QApplication.instance()
     if not qapp:
         qapp = QtWidgets.QApplication(sys.argv)
     qapp.setStyle("Fusion")
 
     if isinstance(data, list | tuple):
-        win = tuple()
+        win = ()
         for d in data:
             win += (ImageTool(d, *args, **kwargs),)
         for w in win:
             w.show()
         win[-1].activateWindow()
         win[-1].raise_()
     else:
```

### Comparing `erlab-1.6.0/src/erlab/interactive/imagetool/controls.py` & `erlab-1.6.1/src/erlab/interactive/imagetool/controls.py`

 * *Files identical despite different names*

### Comparing `erlab-1.6.0/src/erlab/interactive/imagetool/core.py` & `erlab-1.6.1/src/erlab/interactive/imagetool/core.py`

 * *Files identical despite different names*

### Comparing `erlab-1.6.0/src/erlab/interactive/imagetool/fastbinning.py` & `erlab-1.6.1/src/erlab/interactive/imagetool/fastbinning.py`

 * *Files identical despite different names*

### Comparing `erlab-1.6.0/src/erlab/interactive/imagetool/slicer.py` & `erlab-1.6.1/src/erlab/interactive/imagetool/slicer.py`

 * *Files identical despite different names*

### Comparing `erlab-1.6.0/src/erlab/interactive/kspace.py` & `erlab-1.6.1/src/erlab/interactive/kspace.py`

 * *Files identical despite different names*

### Comparing `erlab-1.6.0/src/erlab/interactive/ktool.ui` & `erlab-1.6.1/src/erlab/interactive/ktool.ui`

 * *Files identical despite different names*

### Comparing `erlab-1.6.0/src/erlab/interactive/masktool.py` & `erlab-1.6.1/src/erlab/interactive/masktool.py`

 * *Files identical despite different names*

### Comparing `erlab-1.6.0/src/erlab/interactive/utilities.py` & `erlab-1.6.1/src/erlab/interactive/utilities.py`

 * *Files identical despite different names*

### Comparing `erlab-1.6.0/src/erlab/io/__init__.py` & `erlab-1.6.1/src/erlab/io/__init__.py`

 * *Files identical despite different names*

### Comparing `erlab-1.6.0/src/erlab/io/dataloader.py` & `erlab-1.6.1/src/erlab/io/dataloader.py`

 * *Files identical despite different names*

### Comparing `erlab-1.6.0/src/erlab/io/igor.py` & `erlab-1.6.1/src/erlab/io/igor.py`

 * *Files identical despite different names*

### Comparing `erlab-1.6.0/src/erlab/io/plugins/__init__.py` & `erlab-1.6.1/src/erlab/io/plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `erlab-1.6.0/src/erlab/io/plugins/da30.py` & `erlab-1.6.1/src/erlab/io/plugins/da30.py`

 * *Files identical despite different names*

### Comparing `erlab-1.6.0/src/erlab/io/plugins/kriss.py` & `erlab-1.6.1/src/erlab/io/plugins/kriss.py`

 * *Files identical despite different names*

### Comparing `erlab-1.6.0/src/erlab/io/plugins/merlin.py` & `erlab-1.6.1/src/erlab/io/plugins/merlin.py`

 * *Files identical despite different names*

### Comparing `erlab-1.6.0/src/erlab/io/plugins/ssrl52.py` & `erlab-1.6.1/src/erlab/io/plugins/ssrl52.py`

 * *Files identical despite different names*

### Comparing `erlab-1.6.0/src/erlab/io/utilities.py` & `erlab-1.6.1/src/erlab/io/utilities.py`

 * *Files identical despite different names*

### Comparing `erlab-1.6.0/src/erlab/lattice.py` & `erlab-1.6.1/src/erlab/lattice.py`

 * *Files identical despite different names*

### Comparing `erlab-1.6.0/src/erlab/parallel.py` & `erlab-1.6.1/src/erlab/parallel.py`

 * *Files identical despite different names*

### Comparing `erlab-1.6.0/src/erlab/plotting/IgorCT/Blue-White.txt` & `erlab-1.6.1/src/erlab/plotting/IgorCT/Blue-White.txt`

 * *Files identical despite different names*

### Comparing `erlab-1.6.0/src/erlab/plotting/IgorCT/BlueHot.ibw` & `erlab-1.6.1/src/erlab/plotting/IgorCT/BlueHot.ibw`

 * *Files identical despite different names*

### Comparing `erlab-1.6.0/src/erlab/plotting/IgorCT/CTBlueWhite.ibw` & `erlab-1.6.1/src/erlab/plotting/IgorCT/CTBlueWhite.ibw`

 * *Files identical despite different names*

### Comparing `erlab-1.6.0/src/erlab/plotting/IgorCT/CTRainbowLIght.ibw` & `erlab-1.6.1/src/erlab/plotting/IgorCT/CTRainbowLIght.ibw`

 * *Files identical despite different names*

### Comparing `erlab-1.6.0/src/erlab/plotting/IgorCT/CTRedTemperature.ibw` & `erlab-1.6.1/src/erlab/plotting/IgorCT/CTRedTemperature.ibw`

 * *Files identical despite different names*

### Comparing `erlab-1.6.0/src/erlab/plotting/IgorCT/ColdWarm.ibw` & `erlab-1.6.1/src/erlab/plotting/IgorCT/ColdWarm.ibw`

 * *Files identical despite different names*

### Comparing `erlab-1.6.0/src/erlab/plotting/IgorCT/PlanetEarth.ibw` & `erlab-1.6.1/src/erlab/plotting/IgorCT/PlanetEarth.ibw`

 * *Files identical despite different names*

### Comparing `erlab-1.6.0/src/erlab/plotting/IgorCT/ametrine.ibw` & `erlab-1.6.1/src/erlab/plotting/IgorCT/ametrine.ibw`

 * *Files identical despite different names*

### Comparing `erlab-1.6.0/src/erlab/plotting/IgorCT/isolum.ibw` & `erlab-1.6.1/src/erlab/plotting/IgorCT/isolum.ibw`

 * *Files identical despite different names*

### Comparing `erlab-1.6.0/src/erlab/plotting/IgorCT/morgenstemning.ibw` & `erlab-1.6.1/src/erlab/plotting/IgorCT/morgenstemning.ibw`

 * *Files identical despite different names*

### Comparing `erlab-1.6.0/src/erlab/plotting/__init__.py` & `erlab-1.6.1/src/erlab/plotting/__init__.py`

 * *Files identical despite different names*

### Comparing `erlab-1.6.0/src/erlab/plotting/annotations.py` & `erlab-1.6.1/src/erlab/plotting/annotations.py`

 * *Files identical despite different names*

### Comparing `erlab-1.6.0/src/erlab/plotting/atoms.py` & `erlab-1.6.1/src/erlab/plotting/atoms.py`

 * *Files identical despite different names*

### Comparing `erlab-1.6.0/src/erlab/plotting/bz.py` & `erlab-1.6.1/src/erlab/plotting/bz.py`

 * *Files identical despite different names*

### Comparing `erlab-1.6.0/src/erlab/plotting/colors.py` & `erlab-1.6.1/src/erlab/plotting/colors.py`

 * *Files identical despite different names*

### Comparing `erlab-1.6.0/src/erlab/plotting/erplot.py` & `erlab-1.6.1/src/erlab/plotting/erplot.py`

 * *Files identical despite different names*

### Comparing `erlab-1.6.0/src/erlab/plotting/general.py` & `erlab-1.6.1/src/erlab/plotting/general.py`

 * *Files identical despite different names*

### Comparing `erlab-1.6.0/src/erlab/plotting/plot3d.py` & `erlab-1.6.1/src/erlab/plotting/plot3d.py`

 * *Files identical despite different names*

### Comparing `erlab-1.6.0/src/erlab/plotting/stylelib/fira.mplstyle` & `erlab-1.6.1/src/erlab/plotting/stylelib/fira.mplstyle`

 * *Files 1% similar despite different names*

```diff
@@ -80,15 +80,15 @@
 
 # ***************************************************************************
 # * LaTeX                                                                   *
 # ***************************************************************************
 # For more information on LaTeX properties, see
 # https://matplotlib.org/tutorials/text/usetex.html
 text.usetex: False
-text.latex.preamble: 
+text.latex.preamble:
 
 # The following settings allow you to select the fonts in math mode.
 mathtext.fontset: custom
 mathtext.bf: "Fira Sans:style=normal:variant=normal:weight=bold:stretch=normal"
 mathtext.cal: cursive
 mathtext.it: "Fira Sans:style=italic:variant=normal:weight=regular:stretch=normal"
 mathtext.rm: "Fira Sans:style=normal:variant=normal:weight=regular:stretch=normal"
@@ -124,8 +124,8 @@
 ## PDF backend params
 pdf.fonttype: 42
 
 ## pgf parameter
 # See https://matplotlib.org/tutorials/text/pgf.html for more information.
 pgf.rcfonts: False
 pgf.preamble: "\\usepackage[silent]{fontspec}\n\\usepackage{unicode-math}\n\\usepackage{newcomputermodern}\n\\usepackage[sfdefault,lf]{FiraSans}\n\\setmathfont{Fira Math}\n\\setmathfont[range=up/{greek,Greek,latin,Latin,num}]{Fira Sans}\n\\setmathfont[range=it/{greek,Greek,latin,Latin}]{Fira Sans Italic}\n\\setmathfont[range=bfup/{greek,Greek,latin,Latin,num}]{Fira Sans Bold}\n\\setmathfont[range=bfit/{greek,Greek,latin,Latin}]{Fira Sans Bold Italic}\n\\renewcommand{\\rmfamily}{\\fontseries{l}}"
-pgf.texsystem: lualatex
+pgf.texsystem: lualatex
```

### Comparing `erlab-1.6.0/src/erlab/plotting/stylelib/firalight.mplstyle` & `erlab-1.6.1/src/erlab/plotting/stylelib/firalight.mplstyle`

 * *Files 1% similar despite different names*

```diff
@@ -80,15 +80,15 @@
 
 # ***************************************************************************
 # * LaTeX                                                                   *
 # ***************************************************************************
 # For more information on LaTeX properties, see
 # https://matplotlib.org/tutorials/text/usetex.html
 text.usetex: False
-text.latex.preamble: 
+text.latex.preamble:
 
 # The following settings allow you to select the fonts in math mode.
 mathtext.fontset: custom
 mathtext.bf: "Fira Sans:style=normal:variant=normal:weight=regular:stretch=normal"
 mathtext.cal: cursive
 mathtext.it: "Fira Sans:style=italic:variant=normal:weight=300:stretch=normal"
 mathtext.rm: "Fira Sans:style=normal:variant=normal:weight=300:stretch=normal"
@@ -124,8 +124,8 @@
 ## PDF backend params
 pdf.fonttype: 42
 
 ## pgf parameter
 # See https://matplotlib.org/tutorials/text/pgf.html for more information.
 pgf.rcfonts: False
 pgf.preamble: "\\usepackage[silent]{fontspec}\n\\usepackage{unicode-math}\n\\usepackage{newcomputermodern}\n\\usepackage[sfdefault,light,lf]{FiraSans}\n\\setmathfont{Fira Math}\n\\setmathfont[range=up/{greek,Greek,latin,Latin,num}]{Fira Sans Light}\n\\setmathfont[range=it/{greek,Greek,latin,Latin}]{Fira Sans Light Italic}\n\\setmathfont[range=bfup/{greek,Greek,latin,Latin,num}]{Fira Sans Regular}\n\\setmathfont[range=bfit/{greek,Greek,latin,Latin}]{Fira Sans Italic}\n\\renewcommand{\\rmfamily}{\\fontseries{l}}"
-pgf.texsystem: lualatex
+pgf.texsystem: lualatex
```

### Comparing `erlab-1.6.0/src/erlab/plotting/stylelib/khan.mplstyle` & `erlab-1.6.1/src/erlab/plotting/stylelib/khan.mplstyle`

 * *Files 1% similar despite different names*

```diff
@@ -385,15 +385,15 @@
 # ***************************************************************************
 # * SAVING FIGURES                                                          *
 # ***************************************************************************
 # The default savefig parameters can be different from the display parameters
 # e.g., you may want a higher resolution, or to make the figure
 # background white
 savefig.dpi: 600
-savefig.facecolor: auto 
+savefig.facecolor: auto
 savefig.edgecolor: auto
 savefig.format: pdf
 savefig.bbox: tight
 savefig.pad_inches: 0.02
 savefig.transparent: False
 savefig.orientation: portrait
 
@@ -409,8 +409,8 @@
 pdf.fonttype: 42
 pdf.use14corefonts: False
 pdf.inheritcolor: False
 
 ## SVG backend params
 svg.image_inline: True
 svg.fonttype: path
-svg.hashsalt: None
+svg.hashsalt: None
```

### Comparing `erlab-1.6.0/src/erlab/plotting/stylelib/nature.mplstyle` & `erlab-1.6.1/src/erlab/plotting/stylelib/nature.mplstyle`

 * *Files 0% similar despite different names*

```diff
@@ -99,15 +99,15 @@
 
 # ***************************************************************************
 # * LaTeX                                                                   *
 # ***************************************************************************
 # For more information on LaTeX properties, see
 # https://matplotlib.org/tutorials/text/usetex.html
 text.usetex: False
-text.latex.preamble: 
+text.latex.preamble:
 
 # The following settings allow you to select the fonts in math mode.
 mathtext.fontset: custom
 mathtext.bf: Arial:style=normal:variant=normal:weight=bold:stretch=normal
 mathtext.cal: cursive
 mathtext.it: Arial:style=italic:variant=normal:weight=normal:stretch=normal,Symbol
 mathtext.rm: Arial:style=normal:variant=normal:weight=normal:stretch=normal,Symbol
@@ -220,8 +220,8 @@
 ## PDF backend params
 pdf.fonttype: 42
 
 ## pgf parameter
 # See https://matplotlib.org/tutorials/text/pgf.html for more information.
 pgf.rcfonts: False
 # pgf.preamble: "\\usepackage[silent]{fontspec}\n\\usepackage{unicode-math}\n\\usepackage{newcomputermodern}\n\\usepackage[sfdefault,light,lf]{FiraSans}\n\\setmathfont{Fira Math}\n\\setmathfont[range=up/{greek,Greek,latin,Latin,num}]{Fira Sans Light}\n\\setmathfont[range=it/{greek,Greek,latin,Latin}]{Fira Sans Light Italic}\n\\setmathfont[range=bfup/{greek,Greek,latin,Latin,num}]{Fira Sans Regular}\n\\setmathfont[range=bfit/{greek,Greek,latin,Latin}]{Fira Sans Italic}\n\\renewcommand{\\rmfamily}{\\fontseries{l}}"
-# pgf.texsystem: lualatex
+# pgf.texsystem: lualatex
```

### Comparing `erlab-1.6.0/src/erlab/plotting/stylelib/poster.mplstyle` & `erlab-1.6.1/src/erlab/plotting/stylelib/poster.mplstyle`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -23,8 +23,8 @@
 ytick.minor.pad: 2.0
 figure.constrained_layout.h_pad: 0.06944444444
 figure.constrained_layout.w_pad: 0.06944444444
 lines.dashed_pattern: 12.0, 6.0
 
 savefig.dpi: 600
 savefig.bbox: tight
-savefig.pad_inches: 0.02
+savefig.pad_inches: 0.02
```

### Comparing `erlab-1.6.0/src/erlab/plotting/stylelib/times.mplstyle` & `erlab-1.6.1/src/erlab/plotting/stylelib/times.mplstyle`

 * *Files 2% similar despite different names*

```diff
@@ -80,15 +80,15 @@
 
 # ***************************************************************************
 # * LaTeX                                                                   *
 # ***************************************************************************
 # For more information on LaTeX properties, see
 # https://matplotlib.org/tutorials/text/usetex.html
 text.usetex: False
-text.latex.preamble: 
+text.latex.preamble:
 
 # The following settings allow you to select the fonts in math mode.
 mathtext.fontset: stix
 # mathtext.bf: "Fira Sans:style=normal:variant=normal:weight=regular:stretch=normal"
 # mathtext.cal: cursive
 # mathtext.it: "Fira Sans:style=italic:variant=normal:weight=300:stretch=normal"
 # mathtext.rm: "Fira Sans:style=normal:variant=normal:weight=300:stretch=normal"
@@ -144,8 +144,8 @@
 xtick.major.pad: 0.75
 xtick.minor.pad: 0.75
 ytick.major.size: 1.75
 ytick.minor.size: 1.25
 ytick.major.width: 0.3
 ytick.minor.width: 0.3
 ytick.major.pad: 0.75
-ytick.minor.pad: 0.75
+ytick.minor.pad: 0.75
```

### Comparing `erlab-1.6.0/src/erlab.egg-info/PKG-INFO` & `erlab-1.6.1/src/erlab.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: erlab
-Version: 1.6.0
+Version: 1.6.1
 Summary: Python package for ARPES data analysis and visualization.
 Author-email: Kimoon Han <khan@kaist.ac.kr>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -699,31 +699,30 @@
 Requires-Dist: numbagg
 Requires-Dist: numba-progress
 Requires-Dist: joblib
 Requires-Dist: scipy>=1.8.0
 Requires-Dist: lmfit>=1.2.0
 Requires-Dist: uncertainties>=3.0.1
 Requires-Dist: iminuit>=2.25.2
-Requires-Dist: csaps
 Requires-Dist: matplotlib>=3.8.0
 Requires-Dist: xarray
 Requires-Dist: h5netcdf
 Requires-Dist: varname
 Requires-Dist: tqdm
 Requires-Dist: pyperclip
-Requires-Dist: pyqt6>=6.2.2
 Requires-Dist: qtpy
 Requires-Dist: pyqtgraph>=0.13.1
 Requires-Dist: qtawesome
 Requires-Dist: superqt
 Requires-Dist: importlib-metadata; python_version >= "3.11"
 Provides-Extra: dev
 Requires-Dist: pytest; extra == "dev"
 Requires-Dist: python-semantic-release; extra == "dev"
 Requires-Dist: ruff; extra == "dev"
+Requires-Dist: pre-commit; extra == "dev"
 
 # ERLabPy
 [![Supported Python Versions](https://img.shields.io/pypi/pyversions/erlab)](https://pypi.org/project/erlab/)
 [![PyPi](https://img.shields.io/pypi/v/erlab.svg)](https://pypi.org/project/erlab/)
 [![Workflow Status](https://github.com/kmnhan/erlabpy/actions/workflows/release.yml/badge.svg)](https://github.com/kmnhan/erlabpy/actions/workflows/release.yml)
 [![Documentation Status](https://readthedocs.org/projects/erlabpy/badge/)](https://erlabpy.readthedocs.io/)
 [![License](https://img.shields.io/pypi/l/erlab)](https://github.com/kmnhan/erlabpy/blob/main/LICENSE)
```

### Comparing `erlab-1.6.0/src/erlab.egg-info/SOURCES.txt` & `erlab-1.6.1/src/erlab.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -7,14 +7,16 @@
 README.md
 environment.yml
 environment_apple.yml
 environment_nogit.yml
 environment_nogit_mkl.yml
 pyproject.toml
 requirements.txt
+.github/ISSUE_TEMPLATE/bug-report.md
+.github/ISSUE_TEMPLATE/feature_request.md
 .github/workflows/pr.yml
 .github/workflows/release.yml
 docs/Makefile
 docs/environment.yml
 docs/make.bat
 docs/requirements.txt
 docs/source/bibliography.rst
@@ -79,15 +81,14 @@
 src/erlab/interactive/colors.py
 src/erlab/interactive/curvefittingtool.py
 src/erlab/interactive/derivative.py
 src/erlab/interactive/exampledata.py
 src/erlab/interactive/fermiedge.py
 src/erlab/interactive/kspace.py
 src/erlab/interactive/ktool.ui
-src/erlab/interactive/ktool_old.py
 src/erlab/interactive/masktool.py
 src/erlab/interactive/utilities.py
 src/erlab/interactive/imagetool/__init__.py
 src/erlab/interactive/imagetool/controls.py
 src/erlab/interactive/imagetool/core.py
 src/erlab/interactive/imagetool/fastbinning.py
 src/erlab/interactive/imagetool/slicer.py
```

### Comparing `erlab-1.6.0/tests/test_fastbinning.py` & `erlab-1.6.1/tests/test_fastbinning.py`

 * *Files identical despite different names*

### Comparing `erlab-1.6.0/tests/test_interpolate.py` & `erlab-1.6.1/tests/test_interpolate.py`

 * *Files identical despite different names*

### Comparing `erlab-1.6.0/tests/test_kspace.py` & `erlab-1.6.1/tests/test_kspace.py`

 * *Files identical despite different names*

