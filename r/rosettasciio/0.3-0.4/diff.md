# Comparing `tmp/rosettasciio-0.3.tar.gz` & `tmp/rosettasciio-0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rosettasciio-0.3.tar", last modified: Wed Dec 13 15:27:24 2023, max compression
+gzip compressed data, was "rosettasciio-0.4.tar", last modified: Wed Apr  3 08:14:55 2024, max compression
```

## Comparing `rosettasciio-0.3.tar` & `rosettasciio-0.4.tar`

### file list

```diff
@@ -1,307 +1,307 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 15:27:24.518115 rosettasciio-0.3/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 15:27:24.474115 rosettasciio-0.3/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 15:27:24.474115 rosettasciio-0.3/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (127)      646 2023-12-13 15:27:14.000000 rosettasciio-0.3/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (127)      111 2023-12-13 15:27:14.000000 rosettasciio-0.3/.github/ISSUE_TEMPLATE/custom.md
--rw-r--r--   0 runner    (1001) docker     (127)      455 2023-12-13 15:27:14.000000 rosettasciio-0.3/.github/ISSUE_TEMPLATE/feature_request.md
--rwxr-xr-x   0 runner    (1001) docker     (127)     1438 2023-12-13 15:27:14.000000 rosettasciio-0.3/.github/PULL_REQUEST_TEMPLATE.md
--rw-r--r--   0 runner    (1001) docker     (127)      513 2023-12-13 15:27:14.000000 rosettasciio-0.3/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 15:27:24.474115 rosettasciio-0.3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      193 2023-12-13 15:27:14.000000 rosettasciio-0.3/.github/workflows/black.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2614 2023-12-13 15:27:14.000000 rosettasciio-0.3/.github/workflows/codeql.yml
--rw-r--r--   0 runner    (1001) docker     (127)      632 2023-12-13 15:27:14.000000 rosettasciio-0.3/.github/workflows/docs.yml
--rw-r--r--   0 runner    (1001) docker     (127)      273 2023-12-13 15:27:14.000000 rosettasciio-0.3/.github/workflows/package_and_test.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3562 2023-12-13 15:27:14.000000 rosettasciio-0.3/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3649 2023-12-13 15:27:14.000000 rosettasciio-0.3/.github/workflows/tests.yml
--rw-r--r--   0 runner    (1001) docker     (127)      180 2023-12-13 15:27:14.000000 rosettasciio-0.3/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      501 2023-12-13 15:27:14.000000 rosettasciio-0.3/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      631 2023-12-13 15:27:14.000000 rosettasciio-0.3/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    13445 2023-12-13 15:27:14.000000 rosettasciio-0.3/CHANGES.rst
--rw-r--r--   0 runner    (1001) docker     (127)     8821 2023-12-13 15:27:14.000000 rosettasciio-0.3/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (127)    35151 2023-12-13 15:27:14.000000 rosettasciio-0.3/COPYING.txt
--rw-r--r--   0 runner    (1001) docker     (127)       23 2023-12-13 15:27:14.000000 rosettasciio-0.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    47272 2023-12-13 15:27:24.518115 rosettasciio-0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2933 2023-12-13 15:27:14.000000 rosettasciio-0.3/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     2793 2023-12-13 15:27:14.000000 rosettasciio-0.3/azure-pipelines.yml
--rw-r--r--   0 runner    (1001) docker     (127)      187 2023-12-13 15:27:14.000000 rosettasciio-0.3/conda_environment.yml
--rw-r--r--   0 runner    (1001) docker     (127)      142 2023-12-13 15:27:14.000000 rosettasciio-0.3/conda_environment_dev.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 15:27:24.478115 rosettasciio-0.3/doc/
--rw-r--r--   0 runner    (1001) docker     (127)      634 2023-12-13 15:27:14.000000 rosettasciio-0.3/doc/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 15:27:24.478115 rosettasciio-0.3/doc/_static/
--rw-r--r--   0 runner    (1001) docker     (127)    55120 2023-12-13 15:27:14.000000 rosettasciio-0.3/doc/_static/logo_rec_dark_oct22.png
--rw-r--r--   0 runner    (1001) docker     (127)     7812 2023-12-13 15:27:14.000000 rosettasciio-0.3/doc/_static/logo_rec_dark_oct22.svg
--rw-r--r--   0 runner    (1001) docker     (127)    42674 2023-12-13 15:27:14.000000 rosettasciio-0.3/doc/_static/logo_rec_oct22.png
--rw-r--r--   0 runner    (1001) docker     (127)     7520 2023-12-13 15:27:14.000000 rosettasciio-0.3/doc/_static/logo_rec_oct22.svg
--rw-r--r--   0 runner    (1001) docker     (127)    16026 2023-12-13 15:27:14.000000 rosettasciio-0.3/doc/_static/logo_sq.png
--rw-r--r--   0 runner    (1001) docker     (127)     1694 2023-12-13 15:27:14.000000 rosettasciio-0.3/doc/_static/logo_sq.svg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 15:27:24.478115 rosettasciio-0.3/doc/api/
--rw-r--r--   0 runner    (1001) docker     (127)     2658 2023-12-13 15:27:14.000000 rosettasciio-0.3/doc/api/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)      606 2023-12-13 15:27:14.000000 rosettasciio-0.3/doc/api/utils.rst
--rw-r--r--   0 runner    (1001) docker     (127)       85 2023-12-13 15:27:14.000000 rosettasciio-0.3/doc/changes.rst
--rw-r--r--   0 runner    (1001) docker     (127)     4491 2023-12-13 15:27:14.000000 rosettasciio-0.3/doc/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)       94 2023-12-13 15:27:14.000000 rosettasciio-0.3/doc/contributing.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 15:27:24.478115 rosettasciio-0.3/doc/file_specification/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 15:27:24.478115 rosettasciio-0.3/doc/file_specification/edax/
--rw-r--r--   0 runner    (1001) docker     (127)    95229 2023-12-13 15:27:14.000000 rosettasciio-0.3/doc/file_specification/edax/ImageIPR.pdf
--rw-r--r--   0 runner    (1001) docker     (127)   221879 2023-12-13 15:27:14.000000 rosettasciio-0.3/doc/file_specification/edax/SPECTRUM-V70.pdf
--rw-r--r--   0 runner    (1001) docker     (127)    87801 2023-12-13 15:27:14.000000 rosettasciio-0.3/doc/file_specification/edax/SpcMap-spd.file.format.pdf
--rw-r--r--   0 runner    (1001) docker     (127)      608 2023-12-13 15:27:14.000000 rosettasciio-0.3/doc/file_specification/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     5069 2023-12-13 15:27:14.000000 rosettasciio-0.3/doc/file_specification/ripple-specs.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2660 2023-12-13 15:27:14.000000 rosettasciio-0.3/doc/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)      765 2023-12-13 15:27:14.000000 rosettasciio-0.3/doc/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 15:27:24.478115 rosettasciio-0.3/doc/user_guide/
--rw-r--r--   0 runner    (1001) docker     (127)      130 2023-12-13 15:27:14.000000 rosettasciio-0.3/doc/user_guide/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     6491 2023-12-13 15:27:14.000000 rosettasciio-0.3/doc/user_guide/install.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2212 2023-12-13 15:27:14.000000 rosettasciio-0.3/doc/user_guide/interoperability.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 15:27:24.486115 rosettasciio-0.3/doc/user_guide/supported_formats/
--rw-r--r--   0 runner    (1001) docker     (127)     1394 2023-12-13 15:27:14.000000 rosettasciio-0.3/doc/user_guide/supported_formats/blockfile.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1112 2023-12-13 15:27:14.000000 rosettasciio-0.3/doc/user_guide/supported_formats/bruker.rst
--rw-r--r--   0 runner    (1001) docker     (127)      376 2023-12-13 15:27:14.000000 rosettasciio-0.3/doc/user_guide/supported_formats/de5.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1484 2023-12-13 15:27:14.000000 rosettasciio-0.3/doc/user_guide/supported_formats/dens.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1279 2023-12-13 15:27:14.000000 rosettasciio-0.3/doc/user_guide/supported_formats/digitalmicrograph.rst
--rw-r--r--   0 runner    (1001) docker     (127)      900 2023-12-13 15:27:14.000000 rosettasciio-0.3/doc/user_guide/supported_formats/digitalsurf.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1564 2023-12-13 15:27:14.000000 rosettasciio-0.3/doc/user_guide/supported_formats/edax.rst
--rw-r--r--   0 runner    (1001) docker     (127)     4029 2023-12-13 15:27:14.000000 rosettasciio-0.3/doc/user_guide/supported_formats/emd.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1135 2023-12-13 15:27:14.000000 rosettasciio-0.3/doc/user_guide/supported_formats/empad.rst
--rw-r--r--   0 runner    (1001) docker     (127)      582 2023-12-13 15:27:14.000000 rosettasciio-0.3/doc/user_guide/supported_formats/hamamatsu.rst
--rw-r--r--   0 runner    (1001) docker     (127)     7350 2023-12-13 15:27:14.000000 rosettasciio-0.3/doc/user_guide/supported_formats/hspy.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1974 2023-12-13 15:27:14.000000 rosettasciio-0.3/doc/user_guide/supported_formats/image.rst
--rw-r--r--   0 runner    (1001) docker     (127)      851 2023-12-13 15:27:14.000000 rosettasciio-0.3/doc/user_guide/supported_formats/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1422 2023-12-13 15:27:14.000000 rosettasciio-0.3/doc/user_guide/supported_formats/jeol.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2047 2023-12-13 15:27:14.000000 rosettasciio-0.3/doc/user_guide/supported_formats/jobinyvon.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2712 2023-12-13 15:27:14.000000 rosettasciio-0.3/doc/user_guide/supported_formats/mrc.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1168 2023-12-13 15:27:14.000000 rosettasciio-0.3/doc/user_guide/supported_formats/mrcz.rst
--rw-r--r--   0 runner    (1001) docker     (127)      991 2023-12-13 15:27:14.000000 rosettasciio-0.3/doc/user_guide/supported_formats/msa.rst
--rw-r--r--   0 runner    (1001) docker     (127)      609 2023-12-13 15:27:14.000000 rosettasciio-0.3/doc/user_guide/supported_formats/netcdf.rst
--rw-r--r--   0 runner    (1001) docker     (127)    12030 2023-12-13 15:27:14.000000 rosettasciio-0.3/doc/user_guide/supported_formats/nexus.rst
--rw-r--r--   0 runner    (1001) docker     (127)      662 2023-12-13 15:27:14.000000 rosettasciio-0.3/doc/user_guide/supported_formats/pantarhei.rst
--rw-r--r--   0 runner    (1001) docker     (127)      781 2023-12-13 15:27:14.000000 rosettasciio-0.3/doc/user_guide/supported_formats/phenom.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1174 2023-12-13 15:27:14.000000 rosettasciio-0.3/doc/user_guide/supported_formats/protochips.rst
--rw-r--r--   0 runner    (1001) docker     (127)      883 2023-12-13 15:27:14.000000 rosettasciio-0.3/doc/user_guide/supported_formats/quantumdetector.rst
--rw-r--r--   0 runner    (1001) docker     (127)      982 2023-12-13 15:27:14.000000 rosettasciio-0.3/doc/user_guide/supported_formats/renishaw.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1272 2023-12-13 15:27:14.000000 rosettasciio-0.3/doc/user_guide/supported_formats/ripple.rst
--rw-r--r--   0 runner    (1001) docker     (127)      735 2023-12-13 15:27:14.000000 rosettasciio-0.3/doc/user_guide/supported_formats/semper.rst
--rw-r--r--   0 runner    (1001) docker     (127)    10475 2023-12-13 15:27:14.000000 rosettasciio-0.3/doc/user_guide/supported_formats/supported_formats.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1020 2023-12-13 15:27:14.000000 rosettasciio-0.3/doc/user_guide/supported_formats/tia.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2287 2023-12-13 15:27:14.000000 rosettasciio-0.3/doc/user_guide/supported_formats/tiff.rst
--rw-r--r--   0 runner    (1001) docker     (127)      560 2023-12-13 15:27:14.000000 rosettasciio-0.3/doc/user_guide/supported_formats/trivista.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1362 2023-12-13 15:27:14.000000 rosettasciio-0.3/doc/user_guide/supported_formats/tvips.rst
--rw-r--r--   0 runner    (1001) docker     (127)     4948 2023-12-13 15:27:14.000000 rosettasciio-0.3/doc/user_guide/supported_formats/usid.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2623 2023-12-13 15:27:14.000000 rosettasciio-0.3/doc/user_guide/supported_formats/zspy.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1275 2023-12-13 15:27:14.000000 rosettasciio-0.3/prepare_release.py
--rw-r--r--   0 runner    (1001) docker     (127)     4781 2023-12-13 15:27:14.000000 rosettasciio-0.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     2079 2023-12-13 15:27:14.000000 rosettasciio-0.3/releasing_guide.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 15:27:24.514115 rosettasciio-0.3/rosettasciio.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    47272 2023-12-13 15:27:23.000000 rosettasciio-0.3/rosettasciio.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     7637 2023-12-13 15:27:24.000000 rosettasciio-0.3/rosettasciio.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 15:27:23.000000 rosettasciio-0.3/rosettasciio.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      856 2023-12-13 15:27:23.000000 rosettasciio-0.3/rosettasciio.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2023-12-13 15:27:23.000000 rosettasciio-0.3/rosettasciio.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 15:27:24.486115 rosettasciio-0.3/rsciio/
--rw-r--r--   0 runner    (1001) docker     (127)     2394 2023-12-13 15:27:14.000000 rosettasciio-0.3/rsciio/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5546 2023-12-13 15:27:14.000000 rosettasciio-0.3/rsciio/_docstrings.py
--rw-r--r--   0 runner    (1001) docker     (127)    36981 2023-12-13 15:27:14.000000 rosettasciio-0.3/rsciio/_hierarchical.py
--rw-r--r--   0 runner    (1001) docker     (127)     3568 2023-12-13 15:27:14.000000 rosettasciio-0.3/rsciio/_logger.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 15:27:24.486115 rosettasciio-0.3/rsciio/blockfile/
--rw-r--r--   0 runner    (1001) docker     (127)      141 2023-12-13 15:27:14.000000 rosettasciio-0.3/rsciio/blockfile/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    17598 2023-12-13 15:27:14.000000 rosettasciio-0.3/rsciio/blockfile/_api.py
--rw-r--r--   0 runner    (1001) docker     (127)      213 2023-12-13 15:27:14.000000 rosettasciio-0.3/rsciio/blockfile/specifications.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 15:27:24.490115 rosettasciio-0.3/rsciio/bruker/
--rw-r--r--   0 runner    (1001) docker     (127)      109 2023-12-13 15:27:14.000000 rosettasciio-0.3/rsciio/bruker/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    62247 2023-12-13 15:27:14.000000 rosettasciio-0.3/rsciio/bruker/_api.py
--rw-r--r--   0 runner    (1001) docker     (127)      446 2023-12-13 15:27:14.000000 rosettasciio-0.3/rsciio/bruker/specifications.yaml
--rw-r--r--   0 runner    (1001) docker     (127)  1320981 2023-12-13 15:27:22.000000 rosettasciio-0.3/rsciio/bruker/unbcf_fast.c
--rw-r--r--   0 runner    (1001) docker     (127)    12210 2023-12-13 15:27:14.000000 rosettasciio-0.3/rsciio/bruker/unbcf_fast.pyx
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 15:27:24.490115 rosettasciio-0.3/rsciio/dens/
--rw-r--r--   0 runner    (1001) docker     (127)      109 2023-12-13 15:27:14.000000 rosettasciio-0.3/rsciio/dens/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4002 2023-12-13 15:27:14.000000 rosettasciio-0.3/rsciio/dens/_api.py
--rw-r--r--   0 runner    (1001) docker     (127)      266 2023-12-13 15:27:14.000000 rosettasciio-0.3/rsciio/dens/specifications.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 15:27:24.490115 rosettasciio-0.3/rsciio/digitalmicrograph/
--rw-r--r--   0 runner    (1001) docker     (127)      109 2023-12-13 15:27:14.000000 rosettasciio-0.3/rsciio/digitalmicrograph/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    52996 2023-12-13 15:27:14.000000 rosettasciio-0.3/rsciio/digitalmicrograph/_api.py
--rw-r--r--   0 runner    (1001) docker     (127)      291 2023-12-13 15:27:14.000000 rosettasciio-0.3/rsciio/digitalmicrograph/specifications.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 15:27:24.490115 rosettasciio-0.3/rsciio/digitalsurf/
--rw-r--r--   0 runner    (1001) docker     (127)      109 2023-12-13 15:27:14.000000 rosettasciio-0.3/rsciio/digitalsurf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    52763 2023-12-13 15:27:14.000000 rosettasciio-0.3/rsciio/digitalsurf/_api.py
--rw-r--r--   0 runner    (1001) docker     (127)      277 2023-12-13 15:27:14.000000 rosettasciio-0.3/rsciio/digitalsurf/specifications.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 15:27:24.490115 rosettasciio-0.3/rsciio/edax/
--rw-r--r--   0 runner    (1001) docker     (127)      109 2023-12-13 15:27:14.000000 rosettasciio-0.3/rsciio/edax/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    40912 2023-12-13 15:27:14.000000 rosettasciio-0.3/rsciio/edax/_api.py
--rw-r--r--   0 runner    (1001) docker     (127)      436 2023-12-13 15:27:14.000000 rosettasciio-0.3/rsciio/edax/specifications.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 15:27:24.490115 rosettasciio-0.3/rsciio/emd/
--rw-r--r--   0 runner    (1001) docker     (127)      154 2023-12-13 15:27:14.000000 rosettasciio-0.3/rsciio/emd/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7764 2023-12-13 15:27:14.000000 rosettasciio-0.3/rsciio/emd/_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    20535 2023-12-13 15:27:14.000000 rosettasciio-0.3/rsciio/emd/_emd_ncem.py
--rw-r--r--   0 runner    (1001) docker     (127)    37581 2023-12-13 15:27:14.000000 rosettasciio-0.3/rsciio/emd/_emd_velox.py
--rw-r--r--   0 runner    (1001) docker     (127)      456 2023-12-13 15:27:14.000000 rosettasciio-0.3/rsciio/emd/specifications.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 15:27:24.490115 rosettasciio-0.3/rsciio/empad/
--rw-r--r--   0 runner    (1001) docker     (127)      109 2023-12-13 15:27:14.000000 rosettasciio-0.3/rsciio/empad/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5921 2023-12-13 15:27:14.000000 rosettasciio-0.3/rsciio/empad/_api.py
--rw-r--r--   0 runner    (1001) docker     (127)      274 2023-12-13 15:27:14.000000 rosettasciio-0.3/rsciio/empad/specifications.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 15:27:24.490115 rosettasciio-0.3/rsciio/hamamatsu/
--rw-r--r--   0 runner    (1001) docker     (127)      109 2023-12-13 15:27:14.000000 rosettasciio-0.3/rsciio/hamamatsu/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    19811 2023-12-13 15:27:14.000000 rosettasciio-0.3/rsciio/hamamatsu/_api.py
--rw-r--r--   0 runner    (1001) docker     (127)      205 2023-12-13 15:27:14.000000 rosettasciio-0.3/rsciio/hamamatsu/specifications.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 15:27:24.494115 rosettasciio-0.3/rsciio/hspy/
--rw-r--r--   0 runner    (1001) docker     (127)      154 2023-12-13 15:27:14.000000 rosettasciio-0.3/rsciio/hspy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8377 2023-12-13 15:27:14.000000 rosettasciio-0.3/rsciio/hspy/_api.py
--rw-r--r--   0 runner    (1001) docker     (127)      255 2023-12-13 15:27:14.000000 rosettasciio-0.3/rsciio/hspy/specifications.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 15:27:24.494115 rosettasciio-0.3/rsciio/image/
--rw-r--r--   0 runner    (1001) docker     (127)      154 2023-12-13 15:27:14.000000 rosettasciio-0.3/rsciio/image/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8934 2023-12-13 15:27:14.000000 rosettasciio-0.3/rsciio/image/_api.py
--rw-r--r--   0 runner    (1001) docker     (127)      357 2023-12-13 15:27:14.000000 rosettasciio-0.3/rsciio/image/specifications.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 15:27:24.494115 rosettasciio-0.3/rsciio/impulse/
--rw-r--r--   0 runner    (1001) docker     (127)      109 2023-12-13 15:27:14.000000 rosettasciio-0.3/rsciio/impulse/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6090 2023-12-13 15:27:14.000000 rosettasciio-0.3/rsciio/impulse/_api.py
--rw-r--r--   0 runner    (1001) docker     (127)      190 2023-12-13 15:27:14.000000 rosettasciio-0.3/rsciio/impulse/specifications.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 15:27:24.494115 rosettasciio-0.3/rsciio/jeol/
--rw-r--r--   0 runner    (1001) docker     (127)      109 2023-12-13 15:27:14.000000 rosettasciio-0.3/rsciio/jeol/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    51281 2023-12-13 15:27:14.000000 rosettasciio-0.3/rsciio/jeol/_api.py
--rw-r--r--   0 runner    (1001) docker     (127)      225 2023-12-13 15:27:14.000000 rosettasciio-0.3/rsciio/jeol/specifications.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 15:27:24.494115 rosettasciio-0.3/rsciio/jobinyvon/
--rw-r--r--   0 runner    (1001) docker     (127)      109 2023-12-13 15:27:14.000000 rosettasciio-0.3/rsciio/jobinyvon/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    27877 2023-12-13 15:27:14.000000 rosettasciio-0.3/rsciio/jobinyvon/_api.py
--rw-r--r--   0 runner    (1001) docker     (127)      235 2023-12-13 15:27:14.000000 rosettasciio-0.3/rsciio/jobinyvon/specifications.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 15:27:24.494115 rosettasciio-0.3/rsciio/mrc/
--rw-r--r--   0 runner    (1001) docker     (127)      109 2023-12-13 15:27:14.000000 rosettasciio-0.3/rsciio/mrc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14169 2023-12-13 15:27:14.000000 rosettasciio-0.3/rsciio/mrc/_api.py
--rw-r--r--   0 runner    (1001) docker     (127)      208 2023-12-13 15:27:14.000000 rosettasciio-0.3/rsciio/mrc/specifications.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 15:27:24.494115 rosettasciio-0.3/rsciio/mrcz/
--rw-r--r--   0 runner    (1001) docker     (127)      154 2023-12-13 15:27:14.000000 rosettasciio-0.3/rsciio/mrcz/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7276 2023-12-13 15:27:14.000000 rosettasciio-0.3/rsciio/mrcz/_api.py
--rw-r--r--   0 runner    (1001) docker     (127)      253 2023-12-13 15:27:14.000000 rosettasciio-0.3/rsciio/mrcz/specifications.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 15:27:24.494115 rosettasciio-0.3/rsciio/msa/
--rw-r--r--   0 runner    (1001) docker     (127)      200 2023-12-13 15:27:14.000000 rosettasciio-0.3/rsciio/msa/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    18489 2023-12-13 15:27:14.000000 rosettasciio-0.3/rsciio/msa/_api.py
--rw-r--r--   0 runner    (1001) docker     (127)      268 2023-12-13 15:27:14.000000 rosettasciio-0.3/rsciio/msa/specifications.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 15:27:24.494115 rosettasciio-0.3/rsciio/netcdf/
--rw-r--r--   0 runner    (1001) docker     (127)      109 2023-12-13 15:27:14.000000 rosettasciio-0.3/rsciio/netcdf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6636 2023-12-13 15:27:14.000000 rosettasciio-0.3/rsciio/netcdf/_api.py
--rw-r--r--   0 runner    (1001) docker     (127)      231 2023-12-13 15:27:14.000000 rosettasciio-0.3/rsciio/netcdf/specifications.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 15:27:24.498115 rosettasciio-0.3/rsciio/nexus/
--rw-r--r--   0 runner    (1001) docker     (127)      154 2023-12-13 15:27:14.000000 rosettasciio-0.3/rsciio/nexus/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    42635 2023-12-13 15:27:14.000000 rosettasciio-0.3/rsciio/nexus/_api.py
--rw-r--r--   0 runner    (1001) docker     (127)      261 2023-12-13 15:27:14.000000 rosettasciio-0.3/rsciio/nexus/specifications.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 15:27:24.498115 rosettasciio-0.3/rsciio/pantarhei/
--rw-r--r--   0 runner    (1001) docker     (127)      141 2023-12-13 15:27:14.000000 rosettasciio-0.3/rsciio/pantarhei/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    20908 2023-12-13 15:27:14.000000 rosettasciio-0.3/rsciio/pantarhei/_api.py
--rw-r--r--   0 runner    (1001) docker     (127)      238 2023-12-13 15:27:14.000000 rosettasciio-0.3/rsciio/pantarhei/specifications.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 15:27:24.498115 rosettasciio-0.3/rsciio/phenom/
--rw-r--r--   0 runner    (1001) docker     (127)      109 2023-12-13 15:27:14.000000 rosettasciio-0.3/rsciio/phenom/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    32084 2023-12-13 15:27:14.000000 rosettasciio-0.3/rsciio/phenom/_api.py
--rw-r--r--   0 runner    (1001) docker     (127)      290 2023-12-13 15:27:14.000000 rosettasciio-0.3/rsciio/phenom/specifications.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 15:27:24.498115 rosettasciio-0.3/rsciio/protochips/
--rw-r--r--   0 runner    (1001) docker     (127)      109 2023-12-13 15:27:14.000000 rosettasciio-0.3/rsciio/protochips/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8968 2023-12-13 15:27:14.000000 rosettasciio-0.3/rsciio/protochips/_api.py
--rw-r--r--   0 runner    (1001) docker     (127)      213 2023-12-13 15:27:14.000000 rosettasciio-0.3/rsciio/protochips/specifications.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 15:27:24.498115 rosettasciio-0.3/rsciio/quantumdetector/
--rw-r--r--   0 runner    (1001) docker     (127)      227 2023-12-13 15:27:14.000000 rosettasciio-0.3/rsciio/quantumdetector/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    17895 2023-12-13 15:27:14.000000 rosettasciio-0.3/rsciio/quantumdetector/_api.py
--rw-r--r--   0 runner    (1001) docker     (127)      224 2023-12-13 15:27:14.000000 rosettasciio-0.3/rsciio/quantumdetector/specifications.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 15:27:24.498115 rosettasciio-0.3/rsciio/renishaw/
--rw-r--r--   0 runner    (1001) docker     (127)      109 2023-12-13 15:27:14.000000 rosettasciio-0.3/rsciio/renishaw/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    50089 2023-12-13 15:27:14.000000 rosettasciio-0.3/rsciio/renishaw/_api.py
--rw-r--r--   0 runner    (1001) docker     (127)      222 2023-12-13 15:27:14.000000 rosettasciio-0.3/rsciio/renishaw/specifications.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 15:27:24.498115 rosettasciio-0.3/rsciio/ripple/
--rw-r--r--   0 runner    (1001) docker     (127)      141 2023-12-13 15:27:14.000000 rosettasciio-0.3/rsciio/ripple/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    21047 2023-12-13 15:27:14.000000 rosettasciio-0.3/rsciio/ripple/_api.py
--rw-r--r--   0 runner    (1001) docker     (127)      269 2023-12-13 15:27:14.000000 rosettasciio-0.3/rsciio/ripple/specifications.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 15:27:24.498115 rosettasciio-0.3/rsciio/semper/
--rw-r--r--   0 runner    (1001) docker     (127)      141 2023-12-13 15:27:14.000000 rosettasciio-0.3/rsciio/semper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    27041 2023-12-13 15:27:14.000000 rosettasciio-0.3/rsciio/semper/_api.py
--rw-r--r--   0 runner    (1001) docker     (127)      285 2023-12-13 15:27:14.000000 rosettasciio-0.3/rsciio/semper/specifications.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 15:27:24.506115 rosettasciio-0.3/rsciio/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      748 2023-12-13 15:27:14.000000 rosettasciio-0.3/rsciio/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1527 2023-12-13 15:27:14.000000 rosettasciio-0.3/rsciio/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     5670 2023-12-13 15:27:14.000000 rosettasciio-0.3/rsciio/tests/generate_dm_testing_files.py
--rw-r--r--   0 runner    (1001) docker     (127)     7237 2023-12-13 15:27:14.000000 rosettasciio-0.3/rsciio/tests/generate_renishaw_test_file.py
--rw-r--r--   0 runner    (1001) docker     (127)     1473 2023-12-13 15:27:14.000000 rosettasciio-0.3/rsciio/tests/registry.py
--rw-r--r--   0 runner    (1001) docker     (127)    51599 2023-12-13 15:27:14.000000 rosettasciio-0.3/rsciio/tests/registry.txt
--rw-r--r--   0 runner    (1001) docker     (127)     4783 2023-12-13 15:27:14.000000 rosettasciio-0.3/rsciio/tests/registry_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    17311 2023-12-13 15:27:14.000000 rosettasciio-0.3/rsciio/tests/test_blockfile.py
--rw-r--r--   0 runner    (1001) docker     (127)    11725 2023-12-13 15:27:14.000000 rosettasciio-0.3/rsciio/tests/test_bruker.py
--rw-r--r--   0 runner    (1001) docker     (127)       29 2023-12-13 15:27:14.000000 rosettasciio-0.3/rsciio/tests/test_compilers.c
--rw-r--r--   0 runner    (1001) docker     (127)     1333 2023-12-13 15:27:14.000000 rosettasciio-0.3/rsciio/tests/test_de5.py
--rw-r--r--   0 runner    (1001) docker     (127)     2660 2023-12-13 15:27:14.000000 rosettasciio-0.3/rsciio/tests/test_dens.py
--rw-r--r--   0 runner    (1001) docker     (127)    30032 2023-12-13 15:27:14.000000 rosettasciio-0.3/rsciio/tests/test_digitalmicrograph.py
--rw-r--r--   0 runner    (1001) docker     (127)    17086 2023-12-13 15:27:14.000000 rosettasciio-0.3/rsciio/tests/test_digitalsurf.py
--rw-r--r--   0 runner    (1001) docker     (127)    20487 2023-12-13 15:27:14.000000 rosettasciio-0.3/rsciio/tests/test_edax.py
--rw-r--r--   0 runner    (1001) docker     (127)    10496 2023-12-13 15:27:14.000000 rosettasciio-0.3/rsciio/tests/test_emd_ncem.py
--rw-r--r--   0 runner    (1001) docker     (127)     8022 2023-12-13 15:27:14.000000 rosettasciio-0.3/rsciio/tests/test_emd_prismatic.py
--rw-r--r--   0 runner    (1001) docker     (127)    21555 2023-12-13 15:27:14.000000 rosettasciio-0.3/rsciio/tests/test_emd_velox.py
--rw-r--r--   0 runner    (1001) docker     (127)     4136 2023-12-13 15:27:14.000000 rosettasciio-0.3/rsciio/tests/test_empad.py
--rw-r--r--   0 runner    (1001) docker     (127)     3022 2023-12-13 15:27:14.000000 rosettasciio-0.3/rsciio/tests/test_fei_stream_readers.py
--rw-r--r--   0 runner    (1001) docker     (127)    14704 2023-12-13 15:27:14.000000 rosettasciio-0.3/rsciio/tests/test_hamamatsu.py
--rw-r--r--   0 runner    (1001) docker     (127)    35195 2023-12-13 15:27:14.000000 rosettasciio-0.3/rsciio/tests/test_hspy.py
--rw-r--r--   0 runner    (1001) docker     (127)     9478 2023-12-13 15:27:14.000000 rosettasciio-0.3/rsciio/tests/test_image.py
--rw-r--r--   0 runner    (1001) docker     (127)     4625 2023-12-13 15:27:14.000000 rosettasciio-0.3/rsciio/tests/test_import.py
--rw-r--r--   0 runner    (1001) docker     (127)     7967 2023-12-13 15:27:14.000000 rosettasciio-0.3/rsciio/tests/test_impulse.py
--rw-r--r--   0 runner    (1001) docker     (127)    11436 2023-12-13 15:27:14.000000 rosettasciio-0.3/rsciio/tests/test_io.py
--rw-r--r--   0 runner    (1001) docker     (127)    25127 2023-12-13 15:27:14.000000 rosettasciio-0.3/rsciio/tests/test_jeol.py
--rw-r--r--   0 runner    (1001) docker     (127)    28144 2023-12-13 15:27:14.000000 rosettasciio-0.3/rsciio/tests/test_jobinyvon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1482 2023-12-13 15:27:14.000000 rosettasciio-0.3/rsciio/tests/test_lazy_not_implemented.py
--rw-r--r--   0 runner    (1001) docker     (127)     3876 2023-12-13 15:27:14.000000 rosettasciio-0.3/rsciio/tests/test_mrc.py
--rw-r--r--   0 runner    (1001) docker     (127)     8189 2023-12-13 15:27:14.000000 rosettasciio-0.3/rsciio/tests/test_mrcz.py
--rw-r--r--   0 runner    (1001) docker     (127)    11694 2023-12-13 15:27:14.000000 rosettasciio-0.3/rsciio/tests/test_msa.py
--rw-r--r--   0 runner    (1001) docker     (127)    21559 2023-12-13 15:27:14.000000 rosettasciio-0.3/rsciio/tests/test_nexus.py
--rw-r--r--   0 runner    (1001) docker     (127)     6965 2023-12-13 15:27:14.000000 rosettasciio-0.3/rsciio/tests/test_pantarhei.py
--rw-r--r--   0 runner    (1001) docker     (127)    17571 2023-12-13 15:27:14.000000 rosettasciio-0.3/rsciio/tests/test_phenom.py
--rw-r--r--   0 runner    (1001) docker     (127)    13233 2023-12-13 15:27:14.000000 rosettasciio-0.3/rsciio/tests/test_protochips.py
--rw-r--r--   0 runner    (1001) docker     (127)    12334 2023-12-13 15:27:14.000000 rosettasciio-0.3/rsciio/tests/test_quantumdetector.py
--rw-r--r--   0 runner    (1001) docker     (127)    54161 2023-12-13 15:27:14.000000 rosettasciio-0.3/rsciio/tests/test_renishaw.py
--rw-r--r--   0 runner    (1001) docker     (127)     7824 2023-12-13 15:27:14.000000 rosettasciio-0.3/rsciio/tests/test_ripple.py
--rw-r--r--   0 runner    (1001) docker     (127)     5808 2023-12-13 15:27:14.000000 rosettasciio-0.3/rsciio/tests/test_semper.py
--rw-r--r--   0 runner    (1001) docker     (127)      944 2023-12-13 15:27:14.000000 rosettasciio-0.3/rsciio/tests/test_set_log_level.py
--rw-r--r--   0 runner    (1001) docker     (127)    22595 2023-12-13 15:27:14.000000 rosettasciio-0.3/rsciio/tests/test_tia.py
--rw-r--r--   0 runner    (1001) docker     (127)    45824 2023-12-13 15:27:14.000000 rosettasciio-0.3/rsciio/tests/test_tiff.py
--rw-r--r--   0 runner    (1001) docker     (127)   119568 2023-12-13 15:27:14.000000 rosettasciio-0.3/rsciio/tests/test_trivista.py
--rw-r--r--   0 runner    (1001) docker     (127)    15141 2023-12-13 15:27:14.000000 rosettasciio-0.3/rsciio/tests/test_tvips.py
--rw-r--r--   0 runner    (1001) docker     (127)    26507 2023-12-13 15:27:14.000000 rosettasciio-0.3/rsciio/tests/test_usid.py
--rw-r--r--   0 runner    (1001) docker     (127)     4420 2023-12-13 15:27:14.000000 rosettasciio-0.3/rsciio/tests/test_zspy.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 15:27:24.506115 rosettasciio-0.3/rsciio/tests/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      748 2023-12-13 15:27:14.000000 rosettasciio-0.3/rsciio/tests/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3562 2023-12-13 15:27:14.000000 rosettasciio-0.3/rsciio/tests/utils/test_rgbtools.py
--rw-r--r--   0 runner    (1001) docker     (127)    12516 2023-12-13 15:27:14.000000 rosettasciio-0.3/rsciio/tests/utils/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 15:27:24.510115 rosettasciio-0.3/rsciio/tia/
--rw-r--r--   0 runner    (1001) docker     (127)      109 2023-12-13 15:27:14.000000 rosettasciio-0.3/rsciio/tia/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    28709 2023-12-13 15:27:14.000000 rosettasciio-0.3/rsciio/tia/_api.py
--rw-r--r--   0 runner    (1001) docker     (127)      245 2023-12-13 15:27:14.000000 rosettasciio-0.3/rsciio/tia/specifications.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 15:27:24.510115 rosettasciio-0.3/rsciio/tiff/
--rw-r--r--   0 runner    (1001) docker     (127)      141 2023-12-13 15:27:14.000000 rosettasciio-0.3/rsciio/tiff/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    44001 2023-12-13 15:27:14.000000 rosettasciio-0.3/rsciio/tiff/_api.py
--rw-r--r--   0 runner    (1001) docker     (127)      247 2023-12-13 15:27:14.000000 rosettasciio-0.3/rsciio/tiff/specifications.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 15:27:24.510115 rosettasciio-0.3/rsciio/trivista/
--rw-r--r--   0 runner    (1001) docker     (127)      109 2023-12-13 15:27:14.000000 rosettasciio-0.3/rsciio/trivista/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    31854 2023-12-13 15:27:14.000000 rosettasciio-0.3/rsciio/trivista/_api.py
--rw-r--r--   0 runner    (1001) docker     (127)      191 2023-12-13 15:27:14.000000 rosettasciio-0.3/rsciio/trivista/specifications.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 15:27:24.510115 rosettasciio-0.3/rsciio/tvips/
--rw-r--r--   0 runner    (1001) docker     (127)      141 2023-12-13 15:27:14.000000 rosettasciio-0.3/rsciio/tvips/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    25509 2023-12-13 15:27:14.000000 rosettasciio-0.3/rsciio/tvips/_api.py
--rw-r--r--   0 runner    (1001) docker     (127)      353 2023-12-13 15:27:14.000000 rosettasciio-0.3/rsciio/tvips/specifications.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 15:27:24.510115 rosettasciio-0.3/rsciio/usid/
--rw-r--r--   0 runner    (1001) docker     (127)      141 2023-12-13 15:27:14.000000 rosettasciio-0.3/rsciio/usid/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    17373 2023-12-13 15:27:14.000000 rosettasciio-0.3/rsciio/usid/_api.py
--rw-r--r--   0 runner    (1001) docker     (127)      367 2023-12-13 15:27:14.000000 rosettasciio-0.3/rsciio/usid/specifications.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 15:27:24.510115 rosettasciio-0.3/rsciio/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-13 15:27:14.000000 rosettasciio-0.3/rsciio/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1190 2023-12-13 15:27:14.000000 rosettasciio-0.3/rsciio/utils/array.py
--rw-r--r--   0 runner    (1001) docker     (127)     4048 2023-12-13 15:27:14.000000 rosettasciio-0.3/rsciio/utils/date_time_tools.py
--rw-r--r--   0 runner    (1001) docker     (127)     5911 2023-12-13 15:27:14.000000 rosettasciio-0.3/rsciio/utils/distributed.py
--rw-r--r--   0 runner    (1001) docker     (127)     1695 2023-12-13 15:27:14.000000 rosettasciio-0.3/rsciio/utils/elements.py
--rw-r--r--   0 runner    (1001) docker     (127)     2486 2023-12-13 15:27:14.000000 rosettasciio-0.3/rsciio/utils/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)    14009 2023-12-13 15:27:14.000000 rosettasciio-0.3/rsciio/utils/fei_stream_readers.py
--rw-r--r--   0 runner    (1001) docker     (127)     5650 2023-12-13 15:27:14.000000 rosettasciio-0.3/rsciio/utils/hdf5.py
--rw-r--r--   0 runner    (1001) docker     (127)     7317 2023-12-13 15:27:14.000000 rosettasciio-0.3/rsciio/utils/readfile.py
--rw-r--r--   0 runner    (1001) docker     (127)     3725 2023-12-13 15:27:14.000000 rosettasciio-0.3/rsciio/utils/rgb_tools.py
--rw-r--r--   0 runner    (1001) docker     (127)     4422 2023-12-13 15:27:14.000000 rosettasciio-0.3/rsciio/utils/skimage_exposure.py
--rw-r--r--   0 runner    (1001) docker     (127)     1111 2023-12-13 15:27:14.000000 rosettasciio-0.3/rsciio/utils/tests.py
--rw-r--r--   0 runner    (1001) docker     (127)    17704 2023-12-13 15:27:14.000000 rosettasciio-0.3/rsciio/utils/tools.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 15:27:24.514115 rosettasciio-0.3/rsciio/zspy/
--rw-r--r--   0 runner    (1001) docker     (127)      141 2023-12-13 15:27:14.000000 rosettasciio-0.3/rsciio/zspy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9421 2023-12-13 15:27:14.000000 rosettasciio-0.3/rsciio/zspy/_api.py
--rw-r--r--   0 runner    (1001) docker     (127)      258 2023-12-13 15:27:14.000000 rosettasciio-0.3/rsciio/zspy/specifications.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-13 15:27:24.518115 rosettasciio-0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     3312 2023-12-13 15:27:14.000000 rosettasciio-0.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-13 15:27:24.514115 rosettasciio-0.3/upcoming_changes/
--rw-r--r--   0 runner    (1001) docker     (127)     1744 2023-12-13 15:27:14.000000 rosettasciio-0.3/upcoming_changes/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)      257 2023-12-13 15:27:14.000000 rosettasciio-0.3/update_registry.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 08:14:55.394397 rosettasciio-0.4/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 08:14:55.346397 rosettasciio-0.4/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 08:14:55.346397 rosettasciio-0.4/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)      646 2024-04-03 08:14:44.000000 rosettasciio-0.4/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (127)      111 2024-04-03 08:14:44.000000 rosettasciio-0.4/.github/ISSUE_TEMPLATE/custom.md
+-rw-r--r--   0 runner    (1001) docker     (127)      455 2024-04-03 08:14:44.000000 rosettasciio-0.4/.github/ISSUE_TEMPLATE/feature_request.md
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1438 2024-04-03 08:14:44.000000 rosettasciio-0.4/.github/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0 runner    (1001) docker     (127)      513 2024-04-03 08:14:44.000000 rosettasciio-0.4/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 08:14:55.346397 rosettasciio-0.4/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     2614 2024-04-03 08:14:44.000000 rosettasciio-0.4/.github/workflows/codeql.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      632 2024-04-03 08:14:44.000000 rosettasciio-0.4/.github/workflows/docs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      815 2024-04-03 08:14:44.000000 rosettasciio-0.4/.github/workflows/package_and_test.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     4263 2024-04-03 08:14:44.000000 rosettasciio-0.4/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     4597 2024-04-03 08:14:44.000000 rosettasciio-0.4/.github/workflows/tests.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      180 2024-04-03 08:14:44.000000 rosettasciio-0.4/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      500 2024-04-03 08:14:44.000000 rosettasciio-0.4/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      631 2024-04-03 08:14:44.000000 rosettasciio-0.4/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    16557 2024-04-03 08:14:44.000000 rosettasciio-0.4/CHANGES.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    10569 2024-04-03 08:14:44.000000 rosettasciio-0.4/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    35151 2024-04-03 08:14:44.000000 rosettasciio-0.4/COPYING.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-03 08:14:44.000000 rosettasciio-0.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    47354 2024-04-03 08:14:55.394397 rosettasciio-0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2933 2024-04-03 08:14:44.000000 rosettasciio-0.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2647 2024-04-03 08:14:44.000000 rosettasciio-0.4/azure-pipelines.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      187 2024-04-03 08:14:44.000000 rosettasciio-0.4/conda_environment.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      161 2024-04-03 08:14:44.000000 rosettasciio-0.4/conda_environment_dev.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 08:14:55.346397 rosettasciio-0.4/doc/
+-rw-r--r--   0 runner    (1001) docker     (127)      634 2024-04-03 08:14:44.000000 rosettasciio-0.4/doc/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 08:14:55.350397 rosettasciio-0.4/doc/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)    55120 2024-04-03 08:14:44.000000 rosettasciio-0.4/doc/_static/logo_rec_dark_oct22.png
+-rw-r--r--   0 runner    (1001) docker     (127)     7812 2024-04-03 08:14:44.000000 rosettasciio-0.4/doc/_static/logo_rec_dark_oct22.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    42674 2024-04-03 08:14:44.000000 rosettasciio-0.4/doc/_static/logo_rec_oct22.png
+-rw-r--r--   0 runner    (1001) docker     (127)     7520 2024-04-03 08:14:44.000000 rosettasciio-0.4/doc/_static/logo_rec_oct22.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    16026 2024-04-03 08:14:44.000000 rosettasciio-0.4/doc/_static/logo_sq.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1694 2024-04-03 08:14:44.000000 rosettasciio-0.4/doc/_static/logo_sq.svg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 08:14:55.350397 rosettasciio-0.4/doc/api/
+-rw-r--r--   0 runner    (1001) docker     (127)     2658 2024-04-03 08:14:44.000000 rosettasciio-0.4/doc/api/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      606 2024-04-03 08:14:44.000000 rosettasciio-0.4/doc/api/utils.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-04-03 08:14:44.000000 rosettasciio-0.4/doc/changes.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     4542 2024-04-03 08:14:44.000000 rosettasciio-0.4/doc/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)       94 2024-04-03 08:14:44.000000 rosettasciio-0.4/doc/contributing.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 08:14:55.350397 rosettasciio-0.4/doc/file_specification/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 08:14:55.350397 rosettasciio-0.4/doc/file_specification/edax/
+-rw-r--r--   0 runner    (1001) docker     (127)    95229 2024-04-03 08:14:44.000000 rosettasciio-0.4/doc/file_specification/edax/ImageIPR.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)   221879 2024-04-03 08:14:44.000000 rosettasciio-0.4/doc/file_specification/edax/SPECTRUM-V70.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)    87801 2024-04-03 08:14:44.000000 rosettasciio-0.4/doc/file_specification/edax/SpcMap-spd.file.format.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)      608 2024-04-03 08:14:44.000000 rosettasciio-0.4/doc/file_specification/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     5069 2024-04-03 08:14:44.000000 rosettasciio-0.4/doc/file_specification/ripple-specs.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2660 2024-04-03 08:14:44.000000 rosettasciio-0.4/doc/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      765 2024-04-03 08:14:44.000000 rosettasciio-0.4/doc/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 08:14:55.350397 rosettasciio-0.4/doc/user_guide/
+-rw-r--r--   0 runner    (1001) docker     (127)      130 2024-04-03 08:14:44.000000 rosettasciio-0.4/doc/user_guide/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     6491 2024-04-03 08:14:44.000000 rosettasciio-0.4/doc/user_guide/install.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2212 2024-04-03 08:14:44.000000 rosettasciio-0.4/doc/user_guide/interoperability.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 08:14:55.358397 rosettasciio-0.4/doc/user_guide/supported_formats/
+-rw-r--r--   0 runner    (1001) docker     (127)     1394 2024-04-03 08:14:44.000000 rosettasciio-0.4/doc/user_guide/supported_formats/blockfile.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1112 2024-04-03 08:14:44.000000 rosettasciio-0.4/doc/user_guide/supported_formats/bruker.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      376 2024-04-03 08:14:44.000000 rosettasciio-0.4/doc/user_guide/supported_formats/de5.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1484 2024-04-03 08:14:44.000000 rosettasciio-0.4/doc/user_guide/supported_formats/dens.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1279 2024-04-03 08:14:44.000000 rosettasciio-0.4/doc/user_guide/supported_formats/digitalmicrograph.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      900 2024-04-03 08:14:44.000000 rosettasciio-0.4/doc/user_guide/supported_formats/digitalsurf.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1564 2024-04-03 08:14:44.000000 rosettasciio-0.4/doc/user_guide/supported_formats/edax.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     4029 2024-04-03 08:14:44.000000 rosettasciio-0.4/doc/user_guide/supported_formats/emd.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1135 2024-04-03 08:14:44.000000 rosettasciio-0.4/doc/user_guide/supported_formats/empad.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      582 2024-04-03 08:14:44.000000 rosettasciio-0.4/doc/user_guide/supported_formats/hamamatsu.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     7344 2024-04-03 08:14:44.000000 rosettasciio-0.4/doc/user_guide/supported_formats/hspy.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1974 2024-04-03 08:14:44.000000 rosettasciio-0.4/doc/user_guide/supported_formats/image.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      851 2024-04-03 08:14:44.000000 rosettasciio-0.4/doc/user_guide/supported_formats/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1422 2024-04-03 08:14:44.000000 rosettasciio-0.4/doc/user_guide/supported_formats/jeol.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2047 2024-04-03 08:14:44.000000 rosettasciio-0.4/doc/user_guide/supported_formats/jobinyvon.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2717 2024-04-03 08:14:44.000000 rosettasciio-0.4/doc/user_guide/supported_formats/mrc.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1168 2024-04-03 08:14:44.000000 rosettasciio-0.4/doc/user_guide/supported_formats/mrcz.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      991 2024-04-03 08:14:44.000000 rosettasciio-0.4/doc/user_guide/supported_formats/msa.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      609 2024-04-03 08:14:44.000000 rosettasciio-0.4/doc/user_guide/supported_formats/netcdf.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    11994 2024-04-03 08:14:44.000000 rosettasciio-0.4/doc/user_guide/supported_formats/nexus.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      662 2024-04-03 08:14:44.000000 rosettasciio-0.4/doc/user_guide/supported_formats/pantarhei.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      781 2024-04-03 08:14:44.000000 rosettasciio-0.4/doc/user_guide/supported_formats/phenom.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1174 2024-04-03 08:14:44.000000 rosettasciio-0.4/doc/user_guide/supported_formats/protochips.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      462 2024-04-03 08:14:44.000000 rosettasciio-0.4/doc/user_guide/supported_formats/quantumdetector.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1269 2024-04-03 08:14:44.000000 rosettasciio-0.4/doc/user_guide/supported_formats/renishaw.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1272 2024-04-03 08:14:44.000000 rosettasciio-0.4/doc/user_guide/supported_formats/ripple.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      735 2024-04-03 08:14:44.000000 rosettasciio-0.4/doc/user_guide/supported_formats/semper.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    10475 2024-04-03 08:14:44.000000 rosettasciio-0.4/doc/user_guide/supported_formats/supported_formats.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1020 2024-04-03 08:14:44.000000 rosettasciio-0.4/doc/user_guide/supported_formats/tia.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2287 2024-04-03 08:14:44.000000 rosettasciio-0.4/doc/user_guide/supported_formats/tiff.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      560 2024-04-03 08:14:44.000000 rosettasciio-0.4/doc/user_guide/supported_formats/trivista.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1362 2024-04-03 08:14:44.000000 rosettasciio-0.4/doc/user_guide/supported_formats/tvips.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     4948 2024-04-03 08:14:44.000000 rosettasciio-0.4/doc/user_guide/supported_formats/usid.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2623 2024-04-03 08:14:44.000000 rosettasciio-0.4/doc/user_guide/supported_formats/zspy.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1275 2024-04-03 08:14:44.000000 rosettasciio-0.4/prepare_release.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4806 2024-04-03 08:14:44.000000 rosettasciio-0.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     2079 2024-04-03 08:14:44.000000 rosettasciio-0.4/releasing_guide.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 08:14:55.390397 rosettasciio-0.4/rosettasciio.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    47354 2024-04-03 08:14:54.000000 rosettasciio-0.4/rosettasciio.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7631 2024-04-03 08:14:55.000000 rosettasciio-0.4/rosettasciio.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 08:14:54.000000 rosettasciio-0.4/rosettasciio.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      873 2024-04-03 08:14:54.000000 rosettasciio-0.4/rosettasciio.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-03 08:14:54.000000 rosettasciio-0.4/rosettasciio.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 08:14:55.358397 rosettasciio-0.4/rsciio/
+-rw-r--r--   0 runner    (1001) docker     (127)     2394 2024-04-03 08:14:44.000000 rosettasciio-0.4/rsciio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5648 2024-04-03 08:14:44.000000 rosettasciio-0.4/rsciio/_docstrings.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38404 2024-04-03 08:14:44.000000 rosettasciio-0.4/rsciio/_hierarchical.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3568 2024-04-03 08:14:44.000000 rosettasciio-0.4/rsciio/_logger.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 08:14:55.358397 rosettasciio-0.4/rsciio/blockfile/
+-rw-r--r--   0 runner    (1001) docker     (127)      141 2024-04-03 08:14:44.000000 rosettasciio-0.4/rsciio/blockfile/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17739 2024-04-03 08:14:44.000000 rosettasciio-0.4/rsciio/blockfile/_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)      213 2024-04-03 08:14:44.000000 rosettasciio-0.4/rsciio/blockfile/specifications.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 08:14:55.362397 rosettasciio-0.4/rsciio/bruker/
+-rw-r--r--   0 runner    (1001) docker     (127)      109 2024-04-03 08:14:44.000000 rosettasciio-0.4/rsciio/bruker/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    62405 2024-04-03 08:14:44.000000 rosettasciio-0.4/rsciio/bruker/_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)      446 2024-04-03 08:14:44.000000 rosettasciio-0.4/rsciio/bruker/specifications.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)  1321097 2024-04-03 08:14:53.000000 rosettasciio-0.4/rsciio/bruker/unbcf_fast.c
+-rw-r--r--   0 runner    (1001) docker     (127)    12210 2024-04-03 08:14:44.000000 rosettasciio-0.4/rsciio/bruker/unbcf_fast.pyx
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 08:14:55.362397 rosettasciio-0.4/rsciio/dens/
+-rw-r--r--   0 runner    (1001) docker     (127)      109 2024-04-03 08:14:44.000000 rosettasciio-0.4/rsciio/dens/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4002 2024-04-03 08:14:44.000000 rosettasciio-0.4/rsciio/dens/_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)      266 2024-04-03 08:14:44.000000 rosettasciio-0.4/rsciio/dens/specifications.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 08:14:55.362397 rosettasciio-0.4/rsciio/digitalmicrograph/
+-rw-r--r--   0 runner    (1001) docker     (127)      109 2024-04-03 08:14:44.000000 rosettasciio-0.4/rsciio/digitalmicrograph/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    53003 2024-04-03 08:14:44.000000 rosettasciio-0.4/rsciio/digitalmicrograph/_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)      291 2024-04-03 08:14:44.000000 rosettasciio-0.4/rsciio/digitalmicrograph/specifications.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 08:14:55.362397 rosettasciio-0.4/rsciio/digitalsurf/
+-rw-r--r--   0 runner    (1001) docker     (127)      109 2024-04-03 08:14:44.000000 rosettasciio-0.4/rsciio/digitalsurf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    52763 2024-04-03 08:14:44.000000 rosettasciio-0.4/rsciio/digitalsurf/_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)      277 2024-04-03 08:14:44.000000 rosettasciio-0.4/rsciio/digitalsurf/specifications.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 08:14:55.362397 rosettasciio-0.4/rsciio/edax/
+-rw-r--r--   0 runner    (1001) docker     (127)      109 2024-04-03 08:14:44.000000 rosettasciio-0.4/rsciio/edax/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    40919 2024-04-03 08:14:44.000000 rosettasciio-0.4/rsciio/edax/_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)      436 2024-04-03 08:14:44.000000 rosettasciio-0.4/rsciio/edax/specifications.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 08:14:55.366397 rosettasciio-0.4/rsciio/emd/
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2024-04-03 08:14:44.000000 rosettasciio-0.4/rsciio/emd/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7764 2024-04-03 08:14:44.000000 rosettasciio-0.4/rsciio/emd/_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20534 2024-04-03 08:14:44.000000 rosettasciio-0.4/rsciio/emd/_emd_ncem.py
+-rw-r--r--   0 runner    (1001) docker     (127)    39451 2024-04-03 08:14:44.000000 rosettasciio-0.4/rsciio/emd/_emd_velox.py
+-rw-r--r--   0 runner    (1001) docker     (127)      456 2024-04-03 08:14:44.000000 rosettasciio-0.4/rsciio/emd/specifications.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 08:14:55.366397 rosettasciio-0.4/rsciio/empad/
+-rw-r--r--   0 runner    (1001) docker     (127)      109 2024-04-03 08:14:44.000000 rosettasciio-0.4/rsciio/empad/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5921 2024-04-03 08:14:44.000000 rosettasciio-0.4/rsciio/empad/_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)      274 2024-04-03 08:14:44.000000 rosettasciio-0.4/rsciio/empad/specifications.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 08:14:55.366397 rosettasciio-0.4/rsciio/hamamatsu/
+-rw-r--r--   0 runner    (1001) docker     (127)      109 2024-04-03 08:14:44.000000 rosettasciio-0.4/rsciio/hamamatsu/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19811 2024-04-03 08:14:44.000000 rosettasciio-0.4/rsciio/hamamatsu/_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)      205 2024-04-03 08:14:44.000000 rosettasciio-0.4/rsciio/hamamatsu/specifications.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 08:14:55.366397 rosettasciio-0.4/rsciio/hspy/
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2024-04-03 08:14:44.000000 rosettasciio-0.4/rsciio/hspy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8731 2024-04-03 08:14:44.000000 rosettasciio-0.4/rsciio/hspy/_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)      255 2024-04-03 08:14:44.000000 rosettasciio-0.4/rsciio/hspy/specifications.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 08:14:55.366397 rosettasciio-0.4/rsciio/image/
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2024-04-03 08:14:44.000000 rosettasciio-0.4/rsciio/image/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9438 2024-04-03 08:14:44.000000 rosettasciio-0.4/rsciio/image/_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)      357 2024-04-03 08:14:44.000000 rosettasciio-0.4/rsciio/image/specifications.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 08:14:55.366397 rosettasciio-0.4/rsciio/impulse/
+-rw-r--r--   0 runner    (1001) docker     (127)      109 2024-04-03 08:14:44.000000 rosettasciio-0.4/rsciio/impulse/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6090 2024-04-03 08:14:44.000000 rosettasciio-0.4/rsciio/impulse/_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)      190 2024-04-03 08:14:44.000000 rosettasciio-0.4/rsciio/impulse/specifications.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 08:14:55.370397 rosettasciio-0.4/rsciio/jeol/
+-rw-r--r--   0 runner    (1001) docker     (127)      109 2024-04-03 08:14:44.000000 rosettasciio-0.4/rsciio/jeol/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    51281 2024-04-03 08:14:44.000000 rosettasciio-0.4/rsciio/jeol/_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)      225 2024-04-03 08:14:44.000000 rosettasciio-0.4/rsciio/jeol/specifications.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 08:14:55.370397 rosettasciio-0.4/rsciio/jobinyvon/
+-rw-r--r--   0 runner    (1001) docker     (127)      109 2024-04-03 08:14:44.000000 rosettasciio-0.4/rsciio/jobinyvon/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27887 2024-04-03 08:14:44.000000 rosettasciio-0.4/rsciio/jobinyvon/_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)      235 2024-04-03 08:14:44.000000 rosettasciio-0.4/rsciio/jobinyvon/specifications.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 08:14:55.370397 rosettasciio-0.4/rsciio/mrc/
+-rw-r--r--   0 runner    (1001) docker     (127)      109 2024-04-03 08:14:44.000000 rosettasciio-0.4/rsciio/mrc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14328 2024-04-03 08:14:44.000000 rosettasciio-0.4/rsciio/mrc/_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)      208 2024-04-03 08:14:44.000000 rosettasciio-0.4/rsciio/mrc/specifications.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 08:14:55.370397 rosettasciio-0.4/rsciio/mrcz/
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2024-04-03 08:14:44.000000 rosettasciio-0.4/rsciio/mrcz/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7276 2024-04-03 08:14:44.000000 rosettasciio-0.4/rsciio/mrcz/_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)      253 2024-04-03 08:14:44.000000 rosettasciio-0.4/rsciio/mrcz/specifications.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 08:14:55.370397 rosettasciio-0.4/rsciio/msa/
+-rw-r--r--   0 runner    (1001) docker     (127)      200 2024-04-03 08:14:44.000000 rosettasciio-0.4/rsciio/msa/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18489 2024-04-03 08:14:44.000000 rosettasciio-0.4/rsciio/msa/_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)      268 2024-04-03 08:14:44.000000 rosettasciio-0.4/rsciio/msa/specifications.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 08:14:55.370397 rosettasciio-0.4/rsciio/netcdf/
+-rw-r--r--   0 runner    (1001) docker     (127)      109 2024-04-03 08:14:44.000000 rosettasciio-0.4/rsciio/netcdf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6636 2024-04-03 08:14:44.000000 rosettasciio-0.4/rsciio/netcdf/_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)      231 2024-04-03 08:14:44.000000 rosettasciio-0.4/rsciio/netcdf/specifications.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 08:14:55.370397 rosettasciio-0.4/rsciio/nexus/
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2024-04-03 08:14:44.000000 rosettasciio-0.4/rsciio/nexus/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    42876 2024-04-03 08:14:44.000000 rosettasciio-0.4/rsciio/nexus/_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)      261 2024-04-03 08:14:44.000000 rosettasciio-0.4/rsciio/nexus/specifications.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 08:14:55.374397 rosettasciio-0.4/rsciio/pantarhei/
+-rw-r--r--   0 runner    (1001) docker     (127)      141 2024-04-03 08:14:44.000000 rosettasciio-0.4/rsciio/pantarhei/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20940 2024-04-03 08:14:44.000000 rosettasciio-0.4/rsciio/pantarhei/_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)      238 2024-04-03 08:14:44.000000 rosettasciio-0.4/rsciio/pantarhei/specifications.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 08:14:55.374397 rosettasciio-0.4/rsciio/phenom/
+-rw-r--r--   0 runner    (1001) docker     (127)      109 2024-04-03 08:14:44.000000 rosettasciio-0.4/rsciio/phenom/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32084 2024-04-03 08:14:44.000000 rosettasciio-0.4/rsciio/phenom/_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)      290 2024-04-03 08:14:44.000000 rosettasciio-0.4/rsciio/phenom/specifications.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 08:14:55.374397 rosettasciio-0.4/rsciio/protochips/
+-rw-r--r--   0 runner    (1001) docker     (127)      109 2024-04-03 08:14:44.000000 rosettasciio-0.4/rsciio/protochips/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8968 2024-04-03 08:14:44.000000 rosettasciio-0.4/rsciio/protochips/_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)      213 2024-04-03 08:14:44.000000 rosettasciio-0.4/rsciio/protochips/specifications.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 08:14:55.374397 rosettasciio-0.4/rsciio/quantumdetector/
+-rw-r--r--   0 runner    (1001) docker     (127)      227 2024-04-03 08:14:44.000000 rosettasciio-0.4/rsciio/quantumdetector/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20585 2024-04-03 08:14:44.000000 rosettasciio-0.4/rsciio/quantumdetector/_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)      224 2024-04-03 08:14:44.000000 rosettasciio-0.4/rsciio/quantumdetector/specifications.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 08:14:55.374397 rosettasciio-0.4/rsciio/renishaw/
+-rw-r--r--   0 runner    (1001) docker     (127)      109 2024-04-03 08:14:44.000000 rosettasciio-0.4/rsciio/renishaw/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    51103 2024-04-03 08:14:44.000000 rosettasciio-0.4/rsciio/renishaw/_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)      222 2024-04-03 08:14:44.000000 rosettasciio-0.4/rsciio/renishaw/specifications.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 08:14:55.374397 rosettasciio-0.4/rsciio/ripple/
+-rw-r--r--   0 runner    (1001) docker     (127)      141 2024-04-03 08:14:44.000000 rosettasciio-0.4/rsciio/ripple/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21049 2024-04-03 08:14:44.000000 rosettasciio-0.4/rsciio/ripple/_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)      269 2024-04-03 08:14:44.000000 rosettasciio-0.4/rsciio/ripple/specifications.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 08:14:55.374397 rosettasciio-0.4/rsciio/semper/
+-rw-r--r--   0 runner    (1001) docker     (127)      141 2024-04-03 08:14:44.000000 rosettasciio-0.4/rsciio/semper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27008 2024-04-03 08:14:44.000000 rosettasciio-0.4/rsciio/semper/_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)      285 2024-04-03 08:14:44.000000 rosettasciio-0.4/rsciio/semper/specifications.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 08:14:55.386397 rosettasciio-0.4/rsciio/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      748 2024-04-03 08:14:44.000000 rosettasciio-0.4/rsciio/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2278 2024-04-03 08:14:44.000000 rosettasciio-0.4/rsciio/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5670 2024-04-03 08:14:45.000000 rosettasciio-0.4/rsciio/tests/generate_dm_testing_files.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7237 2024-04-03 08:14:45.000000 rosettasciio-0.4/rsciio/tests/generate_renishaw_test_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1912 2024-04-03 08:14:45.000000 rosettasciio-0.4/rsciio/tests/registry.py
+-rw-r--r--   0 runner    (1001) docker     (127)    51900 2024-04-03 08:14:45.000000 rosettasciio-0.4/rsciio/tests/registry.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     4783 2024-04-03 08:14:45.000000 rosettasciio-0.4/rsciio/tests/registry_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17311 2024-04-03 08:14:45.000000 rosettasciio-0.4/rsciio/tests/test_blockfile.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11725 2024-04-03 08:14:45.000000 rosettasciio-0.4/rsciio/tests/test_bruker.py
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-04-03 08:14:45.000000 rosettasciio-0.4/rsciio/tests/test_compilers.c
+-rw-r--r--   0 runner    (1001) docker     (127)     1333 2024-04-03 08:14:45.000000 rosettasciio-0.4/rsciio/tests/test_de5.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2660 2024-04-03 08:14:45.000000 rosettasciio-0.4/rsciio/tests/test_dens.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30032 2024-04-03 08:14:45.000000 rosettasciio-0.4/rsciio/tests/test_digitalmicrograph.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17086 2024-04-03 08:14:45.000000 rosettasciio-0.4/rsciio/tests/test_digitalsurf.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20487 2024-04-03 08:14:45.000000 rosettasciio-0.4/rsciio/tests/test_edax.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10496 2024-04-03 08:14:45.000000 rosettasciio-0.4/rsciio/tests/test_emd_ncem.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8022 2024-04-03 08:14:45.000000 rosettasciio-0.4/rsciio/tests/test_emd_prismatic.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22554 2024-04-03 08:14:45.000000 rosettasciio-0.4/rsciio/tests/test_emd_velox.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4136 2024-04-03 08:14:45.000000 rosettasciio-0.4/rsciio/tests/test_empad.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3022 2024-04-03 08:14:45.000000 rosettasciio-0.4/rsciio/tests/test_fei_stream_readers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14704 2024-04-03 08:14:45.000000 rosettasciio-0.4/rsciio/tests/test_hamamatsu.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38369 2024-04-03 08:14:45.000000 rosettasciio-0.4/rsciio/tests/test_hspy.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10662 2024-04-03 08:14:45.000000 rosettasciio-0.4/rsciio/tests/test_image.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4625 2024-04-03 08:14:45.000000 rosettasciio-0.4/rsciio/tests/test_import.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7967 2024-04-03 08:14:45.000000 rosettasciio-0.4/rsciio/tests/test_impulse.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11436 2024-04-03 08:14:45.000000 rosettasciio-0.4/rsciio/tests/test_io.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25127 2024-04-03 08:14:45.000000 rosettasciio-0.4/rsciio/tests/test_jeol.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28144 2024-04-03 08:14:45.000000 rosettasciio-0.4/rsciio/tests/test_jobinyvon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1482 2024-04-03 08:14:45.000000 rosettasciio-0.4/rsciio/tests/test_lazy_not_implemented.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3876 2024-04-03 08:14:45.000000 rosettasciio-0.4/rsciio/tests/test_mrc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8189 2024-04-03 08:14:45.000000 rosettasciio-0.4/rsciio/tests/test_mrcz.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11694 2024-04-03 08:14:45.000000 rosettasciio-0.4/rsciio/tests/test_msa.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21559 2024-04-03 08:14:45.000000 rosettasciio-0.4/rsciio/tests/test_nexus.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6965 2024-04-03 08:14:45.000000 rosettasciio-0.4/rsciio/tests/test_pantarhei.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17571 2024-04-03 08:14:45.000000 rosettasciio-0.4/rsciio/tests/test_phenom.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13233 2024-04-03 08:14:45.000000 rosettasciio-0.4/rsciio/tests/test_protochips.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13541 2024-04-03 08:14:45.000000 rosettasciio-0.4/rsciio/tests/test_quantumdetector.py
+-rw-r--r--   0 runner    (1001) docker     (127)    55343 2024-04-03 08:14:45.000000 rosettasciio-0.4/rsciio/tests/test_renishaw.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7821 2024-04-03 08:14:45.000000 rosettasciio-0.4/rsciio/tests/test_ripple.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5808 2024-04-03 08:14:45.000000 rosettasciio-0.4/rsciio/tests/test_semper.py
+-rw-r--r--   0 runner    (1001) docker     (127)      944 2024-04-03 08:14:45.000000 rosettasciio-0.4/rsciio/tests/test_set_log_level.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22595 2024-04-03 08:14:45.000000 rosettasciio-0.4/rsciio/tests/test_tia.py
+-rw-r--r--   0 runner    (1001) docker     (127)    45824 2024-04-03 08:14:45.000000 rosettasciio-0.4/rsciio/tests/test_tiff.py
+-rw-r--r--   0 runner    (1001) docker     (127)   119568 2024-04-03 08:14:45.000000 rosettasciio-0.4/rsciio/tests/test_trivista.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15141 2024-04-03 08:14:45.000000 rosettasciio-0.4/rsciio/tests/test_tvips.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26507 2024-04-03 08:14:45.000000 rosettasciio-0.4/rsciio/tests/test_usid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4420 2024-04-03 08:14:45.000000 rosettasciio-0.4/rsciio/tests/test_zspy.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 08:14:55.386397 rosettasciio-0.4/rsciio/tests/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      748 2024-04-03 08:14:45.000000 rosettasciio-0.4/rsciio/tests/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3562 2024-04-03 08:14:45.000000 rosettasciio-0.4/rsciio/tests/utils/test_rgbtools.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12627 2024-04-03 08:14:45.000000 rosettasciio-0.4/rsciio/tests/utils/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 08:14:55.386397 rosettasciio-0.4/rsciio/tia/
+-rw-r--r--   0 runner    (1001) docker     (127)      109 2024-04-03 08:14:45.000000 rosettasciio-0.4/rsciio/tia/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28715 2024-04-03 08:14:45.000000 rosettasciio-0.4/rsciio/tia/_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)      245 2024-04-03 08:14:45.000000 rosettasciio-0.4/rsciio/tia/specifications.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 08:14:55.386397 rosettasciio-0.4/rsciio/tiff/
+-rw-r--r--   0 runner    (1001) docker     (127)      141 2024-04-03 08:14:45.000000 rosettasciio-0.4/rsciio/tiff/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    44001 2024-04-03 08:14:45.000000 rosettasciio-0.4/rsciio/tiff/_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)      247 2024-04-03 08:14:45.000000 rosettasciio-0.4/rsciio/tiff/specifications.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 08:14:55.386397 rosettasciio-0.4/rsciio/trivista/
+-rw-r--r--   0 runner    (1001) docker     (127)      109 2024-04-03 08:14:45.000000 rosettasciio-0.4/rsciio/trivista/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31854 2024-04-03 08:14:45.000000 rosettasciio-0.4/rsciio/trivista/_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)      191 2024-04-03 08:14:45.000000 rosettasciio-0.4/rsciio/trivista/specifications.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 08:14:55.386397 rosettasciio-0.4/rsciio/tvips/
+-rw-r--r--   0 runner    (1001) docker     (127)      141 2024-04-03 08:14:45.000000 rosettasciio-0.4/rsciio/tvips/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25509 2024-04-03 08:14:45.000000 rosettasciio-0.4/rsciio/tvips/_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)      353 2024-04-03 08:14:45.000000 rosettasciio-0.4/rsciio/tvips/specifications.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 08:14:55.386397 rosettasciio-0.4/rsciio/usid/
+-rw-r--r--   0 runner    (1001) docker     (127)      141 2024-04-03 08:14:45.000000 rosettasciio-0.4/rsciio/usid/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17373 2024-04-03 08:14:45.000000 rosettasciio-0.4/rsciio/usid/_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)      367 2024-04-03 08:14:45.000000 rosettasciio-0.4/rsciio/usid/specifications.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 08:14:55.390397 rosettasciio-0.4/rsciio/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 08:14:45.000000 rosettasciio-0.4/rsciio/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1190 2024-04-03 08:14:45.000000 rosettasciio-0.4/rsciio/utils/array.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4048 2024-04-03 08:14:45.000000 rosettasciio-0.4/rsciio/utils/date_time_tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5911 2024-04-03 08:14:45.000000 rosettasciio-0.4/rsciio/utils/distributed.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1695 2024-04-03 08:14:45.000000 rosettasciio-0.4/rsciio/utils/elements.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2485 2024-04-03 08:14:45.000000 rosettasciio-0.4/rsciio/utils/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14009 2024-04-03 08:14:45.000000 rosettasciio-0.4/rsciio/utils/fei_stream_readers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5651 2024-04-03 08:14:45.000000 rosettasciio-0.4/rsciio/utils/hdf5.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2739 2024-04-03 08:14:45.000000 rosettasciio-0.4/rsciio/utils/image.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7317 2024-04-03 08:14:45.000000 rosettasciio-0.4/rsciio/utils/readfile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3725 2024-04-03 08:14:45.000000 rosettasciio-0.4/rsciio/utils/rgb_tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4423 2024-04-03 08:14:45.000000 rosettasciio-0.4/rsciio/utils/skimage_exposure.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1111 2024-04-03 08:14:45.000000 rosettasciio-0.4/rsciio/utils/tests.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17703 2024-04-03 08:14:45.000000 rosettasciio-0.4/rsciio/utils/tools.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 08:14:55.390397 rosettasciio-0.4/rsciio/zspy/
+-rw-r--r--   0 runner    (1001) docker     (127)      141 2024-04-03 08:14:45.000000 rosettasciio-0.4/rsciio/zspy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9667 2024-04-03 08:14:45.000000 rosettasciio-0.4/rsciio/zspy/_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)      258 2024-04-03 08:14:45.000000 rosettasciio-0.4/rsciio/zspy/specifications.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-03 08:14:55.394397 rosettasciio-0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3311 2024-04-03 08:14:45.000000 rosettasciio-0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 08:14:55.390397 rosettasciio-0.4/upcoming_changes/
+-rw-r--r--   0 runner    (1001) docker     (127)     1744 2024-04-03 08:14:45.000000 rosettasciio-0.4/upcoming_changes/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      257 2024-04-03 08:14:45.000000 rosettasciio-0.4/update_registry.py
```

### Comparing `rosettasciio-0.3/.github/ISSUE_TEMPLATE/bug_report.md` & `rosettasciio-0.4/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `rosettasciio-0.3/.github/PULL_REQUEST_TEMPLATE.md` & `rosettasciio-0.4/.github/PULL_REQUEST_TEMPLATE.md`

 * *Files identical despite different names*

### Comparing `rosettasciio-0.3/.github/dependabot.yml` & `rosettasciio-0.4/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `rosettasciio-0.3/.github/workflows/codeql.yml` & `rosettasciio-0.4/.github/workflows/codeql.yml`

 * *Files 2% similar despite different names*

```diff
@@ -39,35 +39,35 @@
 
     steps:
     - name: Checkout repository
       uses: actions/checkout@v4
 
     # Initializes the CodeQL tools for scanning.
     - name: Initialize CodeQL
-      uses: github/codeql-action/init@v2
+      uses: github/codeql-action/init@v3
       with:
         languages: ${{ matrix.language }}
         # If you wish to specify custom queries, you can do so here or in a config file.
         # By default, queries listed here will override any specified in a config file.
         # Prefix the list here with "+" to use these queries and those in the config file.
         
         # Details on CodeQL's query packs refer to : https://docs.github.com/en/code-security/code-scanning/automatically-scanning-your-code-for-vulnerabilities-and-errors/configuring-code-scanning#using-queries-in-ql-packs
         queries: +security-extended,security-and-quality
 
         
     # Autobuild attempts to build any compiled languages  (C/C++, C#, or Java).
     # If this step fails, then you should remove it and run the build manually (see below)
     - name: Autobuild
-      uses: github/codeql-action/autobuild@v2
+      uses: github/codeql-action/autobuild@v3
 
     # ℹ️ Command-line programs to run using the OS shell.
     # 📚 See https://docs.github.com/en/actions/using-workflows/workflow-syntax-for-github-actions#jobsjob_idstepsrun
 
     #   If the Autobuild fails above, remove it and uncomment the following three lines. 
     #   modify them (or add more) to build your code if your project, please refer to the EXAMPLE below for guidance.
 
     # - run: |
     #   echo "Run, Build Application using script"
     #   ./location_of_script_within_repo/buildscript.sh
 
     - name: Perform CodeQL Analysis
-      uses: github/codeql-action/analyze@v2
+      uses: github/codeql-action/analyze@v3
```

### Comparing `rosettasciio-0.3/.github/workflows/docs.yml` & `rosettasciio-0.4/.github/workflows/docs.yml`

 * *Files identical despite different names*

### Comparing `rosettasciio-0.3/.github/workflows/release.yml` & `rosettasciio-0.4/.github/workflows/release.yml`

 * *Files 16% similar despite different names*

```diff
@@ -4,125 +4,143 @@
 # If run from the hyperspy/rosettasciio repository, the wheels will be uploaded to pypi ;
 # otherwise, the wheels will be available as a github artifact.
 # Can also run on "workflow dispatch" to test building wheels
 on:
   push:
     # Sequence of patterns matched against refs/tags
     tags:
-    - 'v*' # Push events to matching v*, i.e. v1.0, v20.15.10
+      - 'v*' # Push events to matching v*, i.e. v1.0, v20.15.10
   workflow_dispatch:
 
 jobs:
   build_wheels:
     name: Build wheels on ${{ matrix.os }} ${{ matrix.CIBW_ARCHS }}
-    runs-on: ${{ matrix.os }}-latest
+    runs-on: ${{ matrix.os }}
     env:
+      CIBW_ENVIRONMENT: POOCH_BASE_URL=https://github.com/${{ github.repository }}/raw/${{ github.ref_name }}/rsciio/tests/data/
       CIBW_TEST_COMMAND: "pytest --pyargs rsciio"
       CIBW_TEST_EXTRAS: "tests"
       # No need to build wheels for pypy because the pure python wheels can be used
       # PyPy documentation recommends no to build the C extension
       CIBW_SKIP: "{pp*,*-musllinux*,*win32,*-manylinux_i686}"
     strategy:
       fail-fast: false
       matrix:
         include:
-          - os: "ubuntu"
+          - os: "ubuntu-latest"
             CIBW_ARCHS: "x86_64"
-          - os: "ubuntu"
+          - os: "ubuntu-latest"
             CIBW_ARCHS: "aarch64"
-          - os: "windows"
+          - os: "windows-latest"
             CIBW_ARCHS: "AMD64"
-          - os: "macos"
-            CIBW_ARCHS: "x86_64 universal2 arm64"
+          - os: "macos-13"
+            CIBW_ARCHS: "x86_64"
+          - os: "macos-14"
+            CIBW_ARCHS: "arm64"
 
     steps:
       - name: Set up QEMU
         if: contains(matrix.CIBW_ARCHS, 'aarch64')
         uses: docker/setup-qemu-action@v3
         with:
           platforms: arm64
 
       - uses: actions/checkout@v4
 
       - name: Build wheels for CPython
-        uses: pypa/cibuildwheel@v2.16.2
+        uses: pypa/cibuildwheel@v2.17.0
         env:
           CIBW_ARCHS: ${{ matrix.CIBW_ARCHS }}
 
       - name: List wheels
         run: |
           ls ./wheelhouse
 
-      - uses: actions/upload-artifact@v3
+      - uses: actions/upload-artifact@v4
         with:
-          name: wheels
+          name: artifacts-${{ matrix.os }}-${{ matrix.CIBW_ARCHS }}
           path: ./wheelhouse/*.whl
           if-no-files-found: error
 
   make_sdist:
     name: Make SDist
     runs-on: ubuntu-latest
     steps:
-    - uses: actions/checkout@v4
+      - uses: actions/checkout@v4
 
-    - name: Build SDist
-      run: pipx run build --sdist
+      - name: Build SDist
+        run: pipx run build --sdist
+
+      - name: List SDist
+        run: |
+          ls ./dist
 
-    - uses: actions/upload-artifact@v3
-      with:
-        path: dist/*.tar.gz
+      - uses: actions/upload-artifact@v4
+        with:
+          name: artifacts-${{ matrix.os }}-sdist
+          path: dist/*.tar.gz
 
   pure_python_wheel:
     # Build pure python without C extention to be used by pyodide
     name: Make pure python wheel
     runs-on: ubuntu-latest
     steps:
-    - uses: actions/checkout@v4
+      - uses: actions/checkout@v4
 
-    - name: Build pure python wheel
-      run: DISABLE_C_EXTENTIONS=1 pipx run build --wheel
+      - name: Build pure python wheel
+        run: DISABLE_C_EXTENTIONS=1 pipx run build --wheel
 
-    - uses: actions/upload-artifact@v3
-      with:
-        path: dist/*.whl
+      - name: List SDist
+        run: |
+          ls ./dist
+
+      - uses: actions/upload-artifact@v4
+        with:
+          name: artifacts-${{ matrix.os }}-pure_python
+          path: dist/*.whl
+
+  # Merge all disttribution files into the same directory
+  merge_artifacts:
+    runs-on: ubuntu-latest
+    needs: [ build_wheels, make_sdist, pure_python_wheel ]
+    steps:
+      - name: Merge Artifacts
+        uses: actions/upload-artifact/merge@v4
+        with:
+          name: artifacts
+          pattern:  artifacts-*
 
   upload_to_pypi:
-    needs: [build_wheels, make_sdist]
+    needs: merge_artifacts
     runs-on: ubuntu-latest
     permissions:
       # IMPORTANT: this permission is mandatory for trusted publishing
       id-token: write
     steps:
-    - name: Download dist
-      uses: actions/download-artifact@v3
-      with:
-        name: artifact
-        path: dist
-
-    - name: Download wheels
-      uses: actions/download-artifact@v3
-      with:
-        name: wheels
-        path: dist
-
-    - name: Display structure of downloaded files
-      run: ls -R
-      working-directory: dist
-
-    - uses: pypa/gh-action-pypi-publish@release/v1
-      if: ${{ startsWith(github.ref, 'refs/tags/') && github.repository_owner == 'hyperspy' }}
-      # See https://docs.pypi.org/trusted-publishers/using-a-publisher/
+      - name: Download wheels
+        uses: actions/download-artifact@v4
+        with:
+          name: artifacts
+          path: dist
+
+      - name: Display structure of downloaded files
+        run: ls -R
+        working-directory: dist
+
+      - uses: pypa/gh-action-pypi-publish@release/v1
+        if: ${{ startsWith(github.ref, 'refs/tags/') && github.repository_owner == 'hyperspy' }}
+        # See https://docs.pypi.org/trusted-publishers/using-a-publisher/
 
   create_release:
     # TODO: once we are happy with the workflow
     # setup zenodo to create a DOI automatically
     needs: upload_to_pypi
     permissions:
       contents: write
     name: Create Release
     runs-on: ubuntu-latest
     steps:
       - name: Checkout code
         uses: actions/checkout@v4
       - name: Create Release
         id: create_release
-        uses: softprops/action-gh-release@de2c0eb89ae2a093876385947365aca7b0e5f844
+        uses: softprops/action-gh-release@9d7c94cfd0a1f3ed45544c887983e9fa900f0564
```

### Comparing `rosettasciio-0.3/.github/workflows/tests.yml` & `rosettasciio-0.4/.github/workflows/tests.yml`

 * *Files 16% similar despite different names*

```diff
@@ -1,45 +1,59 @@
 name: Tests
 
 on: [push, pull_request, workflow_dispatch]
 
 jobs:
   run_test_site:
-    name: ${{ matrix.os }}-py${{ matrix.PYTHON_VERSION }}${{ matrix.LABEL }}
-    runs-on: ${{ matrix.os }}-latest
+    name: ${{ matrix.os }}-${{ matrix.os_version }}-py${{ matrix.PYTHON_VERSION }}${{ matrix.LABEL }}
+    runs-on: ${{ matrix.os }}-${{ matrix.os_version }}
     timeout-minutes: 30
     env:
       MPLBACKEND: agg
     strategy:
       fail-fast: false
       matrix:
         os: [ubuntu, windows, macos]
+        os_version: [latest]
         PYTHON_VERSION: ['3.9', '3.10']
         LABEL: ['']
         include:
           # test oldest supported version of main dependencies on python 3.8
           - os: ubuntu
+            os_version: latest
             PYTHON_VERSION: '3.8'
             # Set pillow and scikit-image version to be compatible with imageio and scipy
             # matplotlib needs 3.5 to support markers in hyperspy 2.0 (requires `collection.set_offset_transform`)
             DEPENDENCIES: matplotlib==3.5 numpy==1.20.0 imagecodecs==2020.1.31 tifffile==2020.2.16 dask[array]==2021.3.1 numba==0.52 imageio==2.16 pillow==8.3.2 scikit-image==0.18.0
             LABEL: '-oldest'
           # test minimum requirement
           - os: ubuntu
+            os_version: latest
             PYTHON_VERSION: '3.9'
             LABEL: '-minimum'
           - os: ubuntu
+            os_version: latest
             PYTHON_VERSION: '3.12'
             LABEL: '-minimum-without-hyperspy'
           - os: ubuntu
+            os_version: latest
+            PYTHON_VERSION: '3.11'
+            LABEL: '-hyperspy-dev'
+          - os: ubuntu
+            os_version: latest
             PYTHON_VERSION: '3.9'
             LABEL: '-without-hyperspy'
           - os: ubuntu
+            os_version: latest
             PYTHON_VERSION: '3.8'
           - os: ubuntu
+            os_version: latest
+            PYTHON_VERSION: '3.11'
+          - os: macos
+            os_version: '14'
             PYTHON_VERSION: '3.11'
 
     steps:
       - uses: actions/checkout@v4
         with:
           fetch-depth: 0
 
@@ -55,15 +69,27 @@
           git remote add upstream https://github.com/hyperspy/${{ env.REPOSITORY_NAME }}.git
           git fetch upstream --tags
 
       - uses: actions/setup-python@v5
         name: Install Python
         with:
           python-version: ${{ matrix.PYTHON_VERSION }}
-
+        
+      - name: Get the number of CPUs
+        id: cpus
+        run: |
+          import os, platform
+          num_cpus = os.cpu_count()
+          print(f"Number of CPU: {num_cpus}")
+          print(f"Architecture: {platform.machine()}")
+          output_file = os.environ["GITHUB_OUTPUT"]
+          with open(output_file, "a", encoding="utf-8") as output_stream:
+              output_stream.write(f"count={num_cpus}\n")
+        shell: python
+          
       - name: Set Environment Variable
         shell: bash
         # Set PIP_SELECTOR environment variable according to matrix.LABEL
         run: |
           if [[ -n "${{ matrix.LABEL }}" && "${{ matrix.LABEL }}" == *"minimum"* ]]; then
             PIP_SELECTOR="[tests]"
           else
@@ -77,34 +103,36 @@
           pip --version
 
       - name: Install oldest supported version
         if: contains(matrix.LABEL, 'oldest')
         run: |
           pip install ${{ matrix.DEPENDENCIES }}
 
-      - name: Install (HyperSpy dev)
+      - name: Install hyperspy and exspy
         if: ${{ ! contains(matrix.LABEL, 'without-hyperspy') }}
-        # Need to install hyperspy dev until hyperspy 2.0 is released
         run: |
-          pip install git+https://github.com/hyperspy/hyperspy.git@RELEASE_next_major
+          pip install hyperspy exspy
 
-      - name: Install (exspy)
-        if: ${{ ! contains(matrix.LABEL, '-minimum') && ! contains(matrix.LABEL, 'without-hyperspy') }}
+      - name: Install hyperspy and exspy (dev)
+        if: ${{ contains(matrix.LABEL, 'hyperspy-dev') }}
         run: |
+          pip install git+https://github.com/hyperspy/hyperspy.git
           pip install git+https://github.com/hyperspy/exspy.git
 
       - name: Install
         shell: bash
         run: |
           pip install --upgrade -e .'${{ env.PIP_SELECTOR }}'
 
       - name: Pip list
         run: |
           pip list
 
       - name: Run test suite
         run: |
-          pytest --pyargs rsciio --reruns 3 -n 2 --cov=. --cov-report=xml
+          pytest --pyargs rsciio --reruns 3 -n ${{ steps.cpus.outputs.count }} --cov=. --cov-report=xml
 
       - name: Upload coverage to Codecov
         if: ${{ always() }}
-        uses: codecov/codecov-action@v3
+        uses: codecov/codecov-action@v4
+        env:
+          CODECOV_TOKEN: ${{ secrets.CODECOV_TOKEN }}
```

### Comparing `rosettasciio-0.3/.readthedocs.yaml` & `rosettasciio-0.4/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `rosettasciio-0.3/CHANGES.rst` & `rosettasciio-0.4/CHANGES.rst`

 * *Files 12% similar despite different names*

```diff
@@ -4,14 +4,52 @@
 Changelog entries for the development version are available at
 https://rosettasciio.readthedocs.io/en/latest/changes.html
 
 .. towncrier-draft-entries:: |release| [UNRELEASED]
 
 .. towncrier release notes start
 
+0.4 (2024-04-02)
+================
+
+Enhancements
+------------
+
+- :ref:`Renishaw wdf <renishaw-format>`:
+
+  - return survey image instead of saving it to the metadata and add marker of the mapping area on the survey image.
+  - Add support for reading data with invariant axis, for example when the values of the Z axis doesn't change.
+  - Parse calibration of ``jpg`` images saved with Renishaw Wire software. (`#227 <https://github.com/hyperspy/rosettasciio/issues/227>`_)
+- Add support for reading :ref:`emd <emd_fei-format>` Velox version 11. (`#232 <https://github.com/hyperspy/rosettasciio/issues/232>`_)
+- Add :ref:`making test data files <making_test_files>` section to contributing guide, explain characteristics of "good" test data files. (`#233 <https://github.com/hyperspy/rosettasciio/issues/233>`_)
+- :ref:`Quantum Detector <quantumdetector-format>` reader: use timestamps to get navigation shape when the navigation shape is not available - for example, acquisition with pixel trigger or scan shape not in metadata. (`#235 <https://github.com/hyperspy/rosettasciio/issues/235>`_)
+- Improve setting output size for an image. (`#244 <https://github.com/hyperspy/rosettasciio/issues/244>`_)
+
+
+Bug Fixes
+---------
+
+- Fix saving ``hspy`` file with empty array (signal or metadata) and fix closing ``hspy`` file when a error occurs during reading or writing. (`#206 <https://github.com/hyperspy/rosettasciio/issues/206>`_)
+- Fix saving ragged arrays of vectors from/to a chunked ``hspy`` and ``zspy`` store.  Greatly increases the speed of saving and loading ragged arrays from chunked datasets. (`#211 <https://github.com/hyperspy/rosettasciio/issues/211>`_)
+- Fix saving ragged array of strings in ``hspy`` and ``zspy`` format. (`#217 <https://github.com/hyperspy/rosettasciio/issues/217>`_)
+- Fix setting beam energy for XRF maps in ``bcf`` files. (`#231 <https://github.com/hyperspy/rosettasciio/issues/231>`_)
+- :ref:`Quantum Detector <quantumdetector-format>` reader: fix setting chunks. (`#235 <https://github.com/hyperspy/rosettasciio/issues/235>`_)
+
+
+Maintenance
+-----------
+
+- Add ``POOCH_BASE_URL`` to specify the base url used by pooch to download test data. This fixes the failure of the ``package_and_test.yml`` workflow in pull requests where test data are added or updated. (`#200 <https://github.com/hyperspy/rosettasciio/issues/200>`_)
+- Fix documentation links following release of hyperspy 2.0. (`#210 <https://github.com/hyperspy/rosettasciio/issues/210>`_)
+- Run test suite on osx arm64 on GitHub CI and speed running test suite using all available CPUs (3 or 4) instead of only 2. (`#222 <https://github.com/hyperspy/rosettasciio/issues/222>`_)
+- Fix deprecation warnings introduced with numpy 1.25 ("Conversion of an array with ndim > 0 to a scalar is deprecated, ..."). (`#230 <https://github.com/hyperspy/rosettasciio/issues/230>`_)
+- Fix numpy 2.0 removal (``np.product`` and ``np.string_``). (`#238 <https://github.com/hyperspy/rosettasciio/issues/238>`_)
+- Fix download test data when using ``pytest --pyargs rsciio -n``. (`#245 <https://github.com/hyperspy/rosettasciio/issues/245>`_)
+
+
 0.3 (2023-12-12)
 ================
 
 New features
 ------------
 
 - Add :func:`rsciio.set_log_level` to set the logging level of ``RosettaSciIO`` (`#69 <https://github.com/hyperspy/rosettasciio/issues/69>`_)
@@ -156,18 +194,18 @@
 - Initiate GitHub actions for tests and documentation. (`#1 <https://github.com/hyperspy/rosettasciio/issues/1>`_)
 - Initiate towncrier changelog and create templates for PRs and issues. (`#3 <https://github.com/hyperspy/rosettasciio/issues/3>`_)
 - Add github CI workflow to check links, build docs and push to the ``gh-pages`` branch. Fix links and add EDAX reference file specification (`#4 <https://github.com/hyperspy/rosettasciio/issues/4>`_)
 - Add azure pipelines CI to run test suite using conda-forge packages. Add pytest and coverage configuration in ``pyproject.toml`` (`#6 <https://github.com/hyperspy/rosettasciio/issues/6>`_)
 - Fix minimum install, add corresponding tests build and tidy up leftover code (`#13 <https://github.com/hyperspy/rosettasciio/issues/13>`_)
 - Fixes and code consistency improvements based on analysis provided by lgtm.org (`#23 <https://github.com/hyperspy/rosettasciio/issues/23>`_)
 - Added github action for code scanning using the codeQL engine. (`#26 <https://github.com/hyperspy/rosettasciio/issues/26>`_)
-- Following the deprecation cycle announced in `HyperSpy <https://hyperspy.org/hyperspy-doc/current/user_guide/changes.html>`_,
+- Following the deprecation cycle announced in `HyperSpy <https://hyperspy.org/hyperspy-doc/v2.0/changes.html>`_,
   the following keywords and attributes have been removed:
 
-  - :ref:`Bruker composite file (BCF) <bcf-format>`: The ``'spectrum'`` option for the
+  - :ref:`Bruker composite file (BCF) <bruker-format>`: The ``'spectrum'`` option for the
     ``select_type`` parameter was removed. Use 'spectrum_image' instead.
   - :ref:`Electron Microscopy Dataset (EMD) NCEM <emd_ncem-format>`: Using the
     keyword ``'dataset_name'`` was removed, use ``'dataset_path'`` instead.
   - :ref:`NeXus data format <nexus-format>`: The ``dataset_keys``, ``dataset_paths``
     and ``metadata_keys`` keywords were removed. Use ``dataset_key``, ``dataset_path``
     and ``metadata_key`` instead. (`#30 <https://github.com/hyperspy/rosettasciio/issues/30>`_)
 - Unify the ``format_name`` scheme of IO plugins using ``name`` instead and add ``name_aliases`` (list) for backwards compatibility. (`#35 <https://github.com/hyperspy/rosettasciio/issues/35>`_)
```

### Comparing `rosettasciio-0.3/CONTRIBUTING.rst` & `rosettasciio-0.4/CONTRIBUTING.rst`

 * *Files 20% similar despite different names*

```diff
@@ -12,14 +12,41 @@
 The `issue tracker <https://github.com/hyperspy/rosettasciio/issues>`_ can be used to
 report bugs or propose new features. When reporting a bug, the following is
 useful:
 
 - give a minimal example demonstrating the bug,
 - copy and paste the error traceback.
 
+.. _making_test_files:
+
+Making test data files
+======================
+
+Test data files are typically generated using third party software, for example using a proprietary
+software on a scientific instrument. These files are added to the `test suite <https://en.wikipedia.org/wiki/Test_suite>`_
+of RosettaSciIO to make sure that future code development will not introduce bugs or feature 
+regressions. It is important that the test data files area as small as possible to avoid working
+with a repository that contains GBs of test data. Indeed, the test suite is made of severals hundreds of
+test data files and this number of files will keep growing as new features and formats are added
+to RosettaSciIO.
+
+Users can contribute by generating these files on softwares they have access to and by making these
+files available openly; then a RosettaSciIO developer will help with adding these data to the test suite.
+
+What characterizes good test data files:
+
+- Relevant features: the test data files do not need to contain any meaningful data, but they need to
+  cover as much as possible of the format functionalities.
+- Small size:
+
+  - Acquire minimum number of pixels or channels. In case of maps or spectrum images acquire a non-square grid
+    (e.g. "x" and "y" have different lengths).
+  - If possible, generate data that contains no signal (e.g. zeros) as files containing only very few values will compress very well.
+
+
 Pull Requests
 =============
 
 If you want to contribute to the RosettaSciIO source code, you can send us a
 `pull request <https://github.com/hyperspy/rosettasciio/pulls>`_ against the ``main``
 branch. Small bug fixes are corrections to the user guide are typically a good
 starting point. But don't hesitate also for significant code contributions, such
@@ -28,45 +55,57 @@
 
 Please refer to the
 `HyperSpy developer guide <http://hyperspy.org/hyperspy-doc/current/dev_guide/intro.html>`_
 in order to get started and for detailed contributing guidelines.
 
 Lint
 ----
+
+.. _pre-commit.ci: https://pre-commit.ci
+
 To keep the code style consistent (and more readable), `black <https://black.readthedocs.io/>`_
 is used to check the code formatting. When the code doesn't comply with the expected formatting,
-the `lint <https://github.com/hyperspy/rosettasciio/actions/workflows/black.yml>`_ will fail.
-In practise, the code formatting can be fixed by installing ``black`` and running it on the
+the `pre-commit.ci build <https://results.pre-commit.ci/latest/github/hyperspy/rosettasciio/main>`_
+will fail. In practise, the code formatting can be fixed by installing ``black`` and running it on the
 source code or by using :ref:`pre-commit hooks <pre-commit-hooks>`.
+Alternatively, adding the message ``pre-commit.ci autofix`` in a pull request will push a commit with 
+the fixes using `pre-commit.ci`_.
 
 
 .. _adding-and-updating-test-data:
 
 Adding and Updating Test Data
 -----------------------------
 The test data are located in the corresponding subfolder of the ``rsciio/tests/data`` folder.
+The test data are not packaged in the distribution files (wheel, sdist) to keep the packages
+as small as possible in size. When running the test suite, the test data will be downloaded
+from GitHub using pooch. When adding or updating test data, it is necessary to update the test
+data registry.
+
 To add or update test data:
 
 #. use git as usual to add files to the repository.
-#. Update ``rsciio.tests.registry.txt``.  The test data are not packaged in RosettaSciIO to
-   keep the packages as small as possible in size. However, to be able to run the test suite
-   of RosettaSciIO after installation or when packaging on conda-forge, pooch is used to
-   download the data when necessary. It means that when adding and updating test files, it
-   is necessary to update the registry ``rsciio.tests.registry.txt``, which can be done by
-   running :py:func:`~.tests.registry_utils.update_registry` (Unix only):
+#. Update ``rsciio.tests.registry.txt`` by running
+   :py:func:`~.tests.registry_utils.update_registry` (Unix only):
 
    .. code-block:: python
 
       from rsciio.tests.registry_utils import update_registry
 
       update_registry()
 
    On windows, you can use :ref:`pre-commit.ci <pre-commit-hooks>` by adding a message to
    the pull request to update the registry.
 
+.. note::
+
+  The url used by pooch to download the test data can be set by the environment variable
+  ``POOCH_BASE_URL``, otherwise, the default is to download the data from the
+  `hyperspy/rosettasciio <https://github.com/hyperspy/rosettasciio>`_ GitHub repository.
+
 Review
 ------
 
 As quality assurance, to improve the code, and to ensure a generalized
 functionality, pull requests need to be thoroughly reviewed by at least one
 other member of the development team before being merged.
 
@@ -77,15 +116,15 @@
 Two pre-commit hooks are set up:
 
 * Linting: run ``black``
 * Update test data registry (Unix only)
 
 These can be run locally by using `pre-commit <https://pre-commit.com>`__.
 Alternatively, the comment ``pre-commit.ci autofix`` can be added to a PR to fix the formatting
-using `pre-commit.ci <https://pre-commit.ci>`_.
+using `pre-commit.ci`_.
 
 .. _defining-plugins:
 
 Defining new RosettaSciIO plugins
 =================================
 
 Each read/write plugin resides in a separate directory, e.g. ``spamandeggs`` the
```

### Comparing `rosettasciio-0.3/COPYING.txt` & `rosettasciio-0.4/COPYING.txt`

 * *Files identical despite different names*

### Comparing `rosettasciio-0.3/PKG-INFO` & `rosettasciio-0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rosettasciio
-Version: 0.3
+Version: 0.4
 Summary: Reading and writing scientific file formats
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
          of this license document, but changing it is not allowed.
@@ -723,15 +723,17 @@
 Requires-Dist: tifffile>=2020.2.16; extra == "tiff"
 Requires-Dist: imagecodecs>=2020.1.31; extra == "tiff"
 Provides-Extra: usid
 Requires-Dist: pyUSID; extra == "usid"
 Requires-Dist: sidpy<=0.12.0; extra == "usid"
 Provides-Extra: zspy
 Requires-Dist: zarr; extra == "zspy"
+Requires-Dist: msgpack; extra == "zspy"
 Provides-Extra: tests
+Requires-Dist: filelock; extra == "tests"
 Requires-Dist: pooch; extra == "tests"
 Requires-Dist: pytest>=3.6; extra == "tests"
 Requires-Dist: pytest-xdist; extra == "tests"
 Requires-Dist: pytest-rerunfailures; extra == "tests"
 Requires-Dist: pytest-cov; extra == "tests"
 Requires-Dist: setuptools_scm; extra == "tests"
 Provides-Extra: doc
```

### Comparing `rosettasciio-0.3/README.md` & `rosettasciio-0.4/README.md`

 * *Files identical despite different names*

### Comparing `rosettasciio-0.3/azure-pipelines.yml` & `rosettasciio-0.4/azure-pipelines.yml`

 * *Files 4% similar despite different names*

```diff
@@ -53,34 +53,28 @@
       MAMBAFORGE_PATH: $(Agent.BuildDirectory)\mambaforge
 
 pool:
   vmImage: '$(vmImage)'
 
 steps:
 - checkout: self
-  fetchDepth: 1 # Fetch only one commit
+  fetchDepth: 0 # Fetch all commits for setuptools_scm 
+  fetchTags: true #  tags necessary for setuptools_scm
 - template: azure_pipelines/clone_ci-scripts_repo.yml@templates
 - template: azure_pipelines/install_mambaforge.yml@templates
 - template: azure_pipelines/activate_conda.yml@templates
 - template: azure_pipelines/setup_anaconda_packages.yml@templates
 
 - bash: |
     source activate $ENV_NAME
+    pip install "hyperspy>=2.0rc0"
     pip install --no-deps -e .
     conda list
   displayName: Install package
 
-# Need to install hyperspy dev until hyperspy 2.0 is released
-- bash: |
-    source activate $ENV_NAME
-    pip install https://github.com/hyperspy/hyperspy/archive/refs/heads/RELEASE_next_major.zip
-    conda list
-  displayName: Install (HyperSpy dev)
-
-
 # Note we must use `-n 2` argument for pytest-xdist due to
 # https://github.com/pytest-dev/pytest-xdist/issues/9.
 - bash: |
     source activate $ENV_NAME
     pytest --pyargs rsciio --reruns 3 -n 2
   displayName: Run test suite
```

### Comparing `rosettasciio-0.3/doc/Makefile` & `rosettasciio-0.4/doc/Makefile`

 * *Files identical despite different names*

### Comparing `rosettasciio-0.3/doc/_static/logo_rec_dark_oct22.png` & `rosettasciio-0.4/doc/_static/logo_rec_dark_oct22.png`

 * *Files identical despite different names*

### Comparing `rosettasciio-0.3/doc/_static/logo_rec_dark_oct22.svg` & `rosettasciio-0.4/doc/_static/logo_rec_dark_oct22.svg`

 * *Files identical despite different names*

### Comparing `rosettasciio-0.3/doc/_static/logo_rec_oct22.png` & `rosettasciio-0.4/doc/_static/logo_rec_oct22.png`

 * *Files identical despite different names*

### Comparing `rosettasciio-0.3/doc/_static/logo_rec_oct22.svg` & `rosettasciio-0.4/doc/_static/logo_rec_oct22.svg`

 * *Files identical despite different names*

### Comparing `rosettasciio-0.3/doc/_static/logo_sq.png` & `rosettasciio-0.4/doc/_static/logo_sq.png`

 * *Files identical despite different names*

### Comparing `rosettasciio-0.3/doc/_static/logo_sq.svg` & `rosettasciio-0.4/doc/_static/logo_sq.svg`

 * *Files identical despite different names*

### Comparing `rosettasciio-0.3/doc/api/index.rst` & `rosettasciio-0.4/doc/api/index.rst`

 * *Files identical despite different names*

### Comparing `rosettasciio-0.3/doc/api/utils.rst` & `rosettasciio-0.4/doc/api/utils.rst`

 * *Files identical despite different names*

### Comparing `rosettasciio-0.3/doc/conf.py` & `rosettasciio-0.4/doc/conf.py`

 * *Files 5% similar despite different names*

```diff
@@ -41,14 +41,15 @@
     "sphinx.ext.napoleon",
     "sphinxcontrib.towncrier",
 ]
 
 intersphinx_mapping = {
     "conda": ("https://conda.io/projects/conda/en/latest", None),
     "dask": ("https://docs.dask.org/en/latest", None),
+    "exspy": ("https://hyperspy.org/exspy", None),
     "hyperspy": ("https://hyperspy.org/hyperspy-doc/current/", None),
     "h5py": ("https://docs.h5py.org/en/stable/", None),
     "matplotlib": ("https://matplotlib.org/stable", None),
     "mrcz": ("https://python-mrcz.readthedocs.io", None),
     "numcodecs": ("https://numcodecs.readthedocs.io/en/stable", None),
     "numpy": ("https://numpy.org/doc/stable", None),
     "pooch": ("https://www.fatiando.org/pooch/latest", None),
```

### Comparing `rosettasciio-0.3/doc/file_specification/edax/ImageIPR.pdf` & `rosettasciio-0.4/doc/file_specification/edax/ImageIPR.pdf`

 * *Files identical despite different names*

### Comparing `rosettasciio-0.3/doc/file_specification/edax/SPECTRUM-V70.pdf` & `rosettasciio-0.4/doc/file_specification/edax/SPECTRUM-V70.pdf`

 * *Files identical despite different names*

### Comparing `rosettasciio-0.3/doc/file_specification/edax/SpcMap-spd.file.format.pdf` & `rosettasciio-0.4/doc/file_specification/edax/SpcMap-spd.file.format.pdf`

 * *Files identical despite different names*

### Comparing `rosettasciio-0.3/doc/file_specification/index.rst` & `rosettasciio-0.4/doc/file_specification/index.rst`

 * *Files identical despite different names*

### Comparing `rosettasciio-0.3/doc/file_specification/ripple-specs.rst` & `rosettasciio-0.4/doc/file_specification/ripple-specs.rst`

 * *Files identical despite different names*

### Comparing `rosettasciio-0.3/doc/index.rst` & `rosettasciio-0.4/doc/index.rst`

 * *Files identical despite different names*

### Comparing `rosettasciio-0.3/doc/make.bat` & `rosettasciio-0.4/doc/make.bat`

 * *Files identical despite different names*

### Comparing `rosettasciio-0.3/doc/user_guide/install.rst` & `rosettasciio-0.4/doc/user_guide/install.rst`

 * *Files identical despite different names*

### Comparing `rosettasciio-0.3/doc/user_guide/interoperability.rst` & `rosettasciio-0.4/doc/user_guide/interoperability.rst`

 * *Files identical despite different names*

### Comparing `rosettasciio-0.3/doc/user_guide/supported_formats/blockfile.rst` & `rosettasciio-0.4/doc/user_guide/supported_formats/blockfile.rst`

 * *Files identical despite different names*

### Comparing `rosettasciio-0.3/doc/user_guide/supported_formats/bruker.rst` & `rosettasciio-0.4/doc/user_guide/supported_formats/bruker.rst`

 * *Files identical despite different names*

### Comparing `rosettasciio-0.3/doc/user_guide/supported_formats/dens.rst` & `rosettasciio-0.4/doc/user_guide/supported_formats/dens.rst`

 * *Files identical despite different names*

### Comparing `rosettasciio-0.3/doc/user_guide/supported_formats/digitalmicrograph.rst` & `rosettasciio-0.4/doc/user_guide/supported_formats/digitalmicrograph.rst`

 * *Files identical despite different names*

### Comparing `rosettasciio-0.3/doc/user_guide/supported_formats/digitalsurf.rst` & `rosettasciio-0.4/doc/user_guide/supported_formats/digitalsurf.rst`

 * *Files identical despite different names*

### Comparing `rosettasciio-0.3/doc/user_guide/supported_formats/edax.rst` & `rosettasciio-0.4/doc/user_guide/supported_formats/edax.rst`

 * *Files identical despite different names*

### Comparing `rosettasciio-0.3/doc/user_guide/supported_formats/emd.rst` & `rosettasciio-0.4/doc/user_guide/supported_formats/emd.rst`

 * *Files identical despite different names*

### Comparing `rosettasciio-0.3/doc/user_guide/supported_formats/empad.rst` & `rosettasciio-0.4/doc/user_guide/supported_formats/empad.rst`

 * *Files identical despite different names*

### Comparing `rosettasciio-0.3/doc/user_guide/supported_formats/hamamatsu.rst` & `rosettasciio-0.4/doc/user_guide/supported_formats/hamamatsu.rst`

 * *Files identical despite different names*

### Comparing `rosettasciio-0.3/doc/user_guide/supported_formats/hspy.rst` & `rosettasciio-0.4/doc/user_guide/supported_formats/hspy.rst`

 * *Files 1% similar despite different names*

```diff
@@ -36,15 +36,15 @@
     >>> s.save('test.hdf5')
 
 .. note::
    To read this format, the optional dependency ``h5py`` is required.
 
 
 When saving to ``.hspy``, all supported objects in the signal's
-:external+hyperspy:attr:`hyperspy.signal.BaseSignal.metadata` are stored. This includes lists, tuples
+:external+hyperspy:attr:`hyperspy.api.signals.BaseSignal.metadata` are stored. This includes lists, tuples
 and signals. Please note that in order to increase saving efficiency and speed,
 if possible, the inner-most structures are converted to numpy arrays when saved.
 This procedure homogenizes any types of the objects inside, most notably casting
 numbers as strings if any other strings are present:
 
 .. code-block:: python
 
@@ -54,15 +54,15 @@
     >>> # after saving:
     ['1', '2.0', 'a name']
 
 The change of type is done using numpy "safe" rules, so no information is lost,
 as numbers are represented to full machine precision.
 
 This feature is particularly useful when using
-:external+hyperspy:meth:`hyperspy._signals.eds.EDSSpectrum.get_lines_intensity`:
+:external+exspy:meth:`exspy.signals.EDSSpectrum.get_lines_intensity`:
 
 .. code-block:: python
 
     >>> s = hs.datasets.example_signals.EDS_SEM_Spectrum()
     >>> s.metadata.Sample.intensities = s.get_lines_intensity()
     >>> s.save('EDS_spectrum.hspy')
```

### Comparing `rosettasciio-0.3/doc/user_guide/supported_formats/image.rst` & `rosettasciio-0.4/doc/user_guide/supported_formats/image.rst`

 * *Files identical despite different names*

### Comparing `rosettasciio-0.3/doc/user_guide/supported_formats/index.rst` & `rosettasciio-0.4/doc/user_guide/supported_formats/index.rst`

 * *Files identical despite different names*

### Comparing `rosettasciio-0.3/doc/user_guide/supported_formats/jeol.rst` & `rosettasciio-0.4/doc/user_guide/supported_formats/jeol.rst`

 * *Files identical despite different names*

### Comparing `rosettasciio-0.3/doc/user_guide/supported_formats/jobinyvon.rst` & `rosettasciio-0.4/doc/user_guide/supported_formats/jobinyvon.rst`

 * *Files identical despite different names*

### Comparing `rosettasciio-0.3/doc/user_guide/supported_formats/mrc.rst` & `rosettasciio-0.4/doc/user_guide/supported_formats/mrc.rst`

 * *Files 1% similar despite different names*

```diff
@@ -35,15 +35,15 @@
 
     data = np.random.randint(100, size=(10, 100, 100)).astype('int16')
     s = hs.signals.Signal2D(data)
     s_dict = s.as_dictionary()
 
     mrcz.file_writer('test.mrc', s_dict)
 
-Alternatively, use :py:meth:`hyperspy.signal.BaseSignal.save`, which will pick the
+Alternatively, use :py:meth:`hyperspy.api.signals.BaseSignal.save`, which will pick the
 ``mrcz`` plugin automatically:
 
 .. code-block:: python
 
     import hyperspy.api as hs
     import numpy as np
```

### Comparing `rosettasciio-0.3/doc/user_guide/supported_formats/mrcz.rst` & `rosettasciio-0.4/doc/user_guide/supported_formats/mrcz.rst`

 * *Files identical despite different names*

### Comparing `rosettasciio-0.3/doc/user_guide/supported_formats/msa.rst` & `rosettasciio-0.4/doc/user_guide/supported_formats/msa.rst`

 * *Files identical despite different names*

### Comparing `rosettasciio-0.3/doc/user_guide/supported_formats/netcdf.rst` & `rosettasciio-0.4/doc/user_guide/supported_formats/netcdf.rst`

 * *Files identical despite different names*

### Comparing `rosettasciio-0.3/doc/user_guide/supported_formats/nexus.rst` & `rosettasciio-0.4/doc/user_guide/supported_formats/nexus.rst`

 * *Files 1% similar despite different names*

```diff
@@ -54,15 +54,15 @@
 metadata structured in different ways, the loader is written to be quite
 flexible and can also be used to inspect any hdf5 based file.
 
 
 Differences with respect to HSpy
 ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
 
-The `HyperSpy metadata structure <https://hyperspy.org/hyperspy-doc/current/user_guide/metadata_structure.html>`_
+The :external+hyperspy:ref:`HyperSpy metadata structure <metadata_structure>`
 stores arrays as hdf datasets without attributes
 and stores floats, ints and strings as attributes.
 The NeXus format uses hdf dataset attributes to store additional
 information such as an indication of the units for an axis or the ``NX_class`` which
 the dataset structure follows. The metadata, HyperSpy or ``original_metadata``,
 therefore needs to be able to indicate the values and attributes of a dataset.
 To implement this structure the ``value`` and ``attrs`` of a dataset can also be
```

### Comparing `rosettasciio-0.3/doc/user_guide/supported_formats/pantarhei.rst` & `rosettasciio-0.4/doc/user_guide/supported_formats/pantarhei.rst`

 * *Files identical despite different names*

### Comparing `rosettasciio-0.3/doc/user_guide/supported_formats/phenom.rst` & `rosettasciio-0.4/doc/user_guide/supported_formats/phenom.rst`

 * *Files identical despite different names*

### Comparing `rosettasciio-0.3/doc/user_guide/supported_formats/protochips.rst` & `rosettasciio-0.4/doc/user_guide/supported_formats/protochips.rst`

 * *Files identical despite different names*

### Comparing `rosettasciio-0.3/doc/user_guide/supported_formats/renishaw.rst` & `rosettasciio-0.4/doc/user_guide/supported_formats/renishaw.rst`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,18 @@
 .. _renishaw-format:
 
 Renishaw
 --------
 
 Reader for spectroscopy data saved using Renishaw's WiRE software.
 Currently, RosettaSciIO can only read the ``.wdf`` format from Renishaw.
+When reading spectral images, the white light image will be returned along the 
+spectral images in the list of dictionaries. The position of the mapped area
+is returned in the metadata dictionary of the white light image and this will
+be displayed when plotting the image with HyperSpy.
 
 If `LumiSpy <https://lumispy.org>`_ is installed, ``Luminescence`` will be
 used as the ``signal_type``.
 
 .. Note::
 
    There are many different options for the axes according to the format specifications.
```

### Comparing `rosettasciio-0.3/doc/user_guide/supported_formats/ripple.rst` & `rosettasciio-0.4/doc/user_guide/supported_formats/ripple.rst`

 * *Files identical despite different names*

### Comparing `rosettasciio-0.3/doc/user_guide/supported_formats/semper.rst` & `rosettasciio-0.4/doc/user_guide/supported_formats/semper.rst`

 * *Files identical despite different names*

### Comparing `rosettasciio-0.3/doc/user_guide/supported_formats/supported_formats.rst` & `rosettasciio-0.4/doc/user_guide/supported_formats/supported_formats.rst`

 * *Files identical despite different names*

### Comparing `rosettasciio-0.3/doc/user_guide/supported_formats/tia.rst` & `rosettasciio-0.4/doc/user_guide/supported_formats/tia.rst`

 * *Files identical despite different names*

### Comparing `rosettasciio-0.3/doc/user_guide/supported_formats/tiff.rst` & `rosettasciio-0.4/doc/user_guide/supported_formats/tiff.rst`

 * *Files identical despite different names*

### Comparing `rosettasciio-0.3/doc/user_guide/supported_formats/trivista.rst` & `rosettasciio-0.4/doc/user_guide/supported_formats/trivista.rst`

 * *Files identical despite different names*

### Comparing `rosettasciio-0.3/doc/user_guide/supported_formats/tvips.rst` & `rosettasciio-0.4/doc/user_guide/supported_formats/tvips.rst`

 * *Files identical despite different names*

### Comparing `rosettasciio-0.3/doc/user_guide/supported_formats/usid.rst` & `rosettasciio-0.4/doc/user_guide/supported_formats/usid.rst`

 * *Files identical despite different names*

### Comparing `rosettasciio-0.3/doc/user_guide/supported_formats/zspy.rst` & `rosettasciio-0.4/doc/user_guide/supported_formats/zspy.rst`

 * *Files identical despite different names*

### Comparing `rosettasciio-0.3/prepare_release.py` & `rosettasciio-0.4/prepare_release.py`

 * *Files identical despite different names*

### Comparing `rosettasciio-0.3/pyproject.toml` & `rosettasciio-0.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -94,16 +94,17 @@
 mrcz = ["blosc>=1.5", "mrcz>=0.3.6"]
 scalebar_export = ["matplotlib-scalebar", "matplotlib>=3.5"]
 speed = ["numba>=0.52"]
 tiff = ["tifffile>=2020.2.16", "imagecodecs>=2020.1.31"]
 # Add sidpy dependency and pinning as workaround to fix pyUSID import
 # Remove sidpy dependency once https://github.com/pycroscopy/pyUSID/issues/85 is fixed.
 usid = ["pyUSID", "sidpy<=0.12.0"]
-zspy = ["zarr"]
+zspy = ["zarr", "msgpack"]
 tests = [
+  "filelock",
   "pooch",
   "pytest>=3.6",
   "pytest-xdist",
   "pytest-rerunfailures",
   "pytest-cov",
   "setuptools_scm",
 ]
@@ -154,30 +155,30 @@
 
 [tool.setuptools.package-data]
 "rsciio" = ["*test_compilers.c", "*.yaml", "*registry.txt"]
 
 [tool.setuptools_scm]
 # Presence enables setuptools_scm, the version will be determine at build time from git
 # The version will be updated by the `prepare_release.py` script
-fallback_version = "0.4.dev0"
+fallback_version = "0.5.dev0"
 
 [tool.towncrier]
 directory = "upcoming_changes/"
 filename = "CHANGES.rst"
 issue_format = "`#{issue} <https://github.com/hyperspy/rosettasciio/issues/{issue}>`_"
 title_format = "{version} ({project_date})"
 package = "rsciio"
 type = [
-    { directory = "api", name = "API changes", showcontent = true },
+    { directory = "new", name = "New features", showcontent = true },
+    { directory = "enhancements", name = "Enhancements", showcontent = true },
     { directory = "bugfix", name = "Bug Fixes", showcontent = true },
+    { directory = "api", name = "API changes", showcontent = true },
     { directory = "deprecation", name = "Deprecations", showcontent = true },
     { directory = "doc", name = "Improved Documentation", showcontent = true },
-    { directory = "enhancements", name = "Enhancements", showcontent = true },
     { directory = "maintenance", name = "Maintenance", showcontent = true },
-    { directory = "new", name = "New features", showcontent = true },
 ]
 
 [tool.coverage.run]
 branch = true
 source = ["rsciio"]
 omit = [
   "prepare_release.py",
```

### Comparing `rosettasciio-0.3/releasing_guide.md` & `rosettasciio-0.4/releasing_guide.md`

 * *Files identical despite different names*

### Comparing `rosettasciio-0.3/rosettasciio.egg-info/PKG-INFO` & `rosettasciio-0.4/rosettasciio.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rosettasciio
-Version: 0.3
+Version: 0.4
 Summary: Reading and writing scientific file formats
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
          of this license document, but changing it is not allowed.
@@ -723,15 +723,17 @@
 Requires-Dist: tifffile>=2020.2.16; extra == "tiff"
 Requires-Dist: imagecodecs>=2020.1.31; extra == "tiff"
 Provides-Extra: usid
 Requires-Dist: pyUSID; extra == "usid"
 Requires-Dist: sidpy<=0.12.0; extra == "usid"
 Provides-Extra: zspy
 Requires-Dist: zarr; extra == "zspy"
+Requires-Dist: msgpack; extra == "zspy"
 Provides-Extra: tests
+Requires-Dist: filelock; extra == "tests"
 Requires-Dist: pooch; extra == "tests"
 Requires-Dist: pytest>=3.6; extra == "tests"
 Requires-Dist: pytest-xdist; extra == "tests"
 Requires-Dist: pytest-rerunfailures; extra == "tests"
 Requires-Dist: pytest-cov; extra == "tests"
 Requires-Dist: setuptools_scm; extra == "tests"
 Provides-Extra: doc
```

### Comparing `rosettasciio-0.3/rosettasciio.egg-info/SOURCES.txt` & `rosettasciio-0.4/rosettasciio.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,14 @@
 setup.py
 update_registry.py
 .github/PULL_REQUEST_TEMPLATE.md
 .github/dependabot.yml
 .github/ISSUE_TEMPLATE/bug_report.md
 .github/ISSUE_TEMPLATE/custom.md
 .github/ISSUE_TEMPLATE/feature_request.md
-.github/workflows/black.yml
 .github/workflows/codeql.yml
 .github/workflows/docs.yml
 .github/workflows/package_and_test.yml
 .github/workflows/release.yml
 .github/workflows/tests.yml
 doc/Makefile
 doc/changes.rst
@@ -241,14 +240,15 @@
 rsciio/utils/array.py
 rsciio/utils/date_time_tools.py
 rsciio/utils/distributed.py
 rsciio/utils/elements.py
 rsciio/utils/exceptions.py
 rsciio/utils/fei_stream_readers.py
 rsciio/utils/hdf5.py
+rsciio/utils/image.py
 rsciio/utils/readfile.py
 rsciio/utils/rgb_tools.py
 rsciio/utils/skimage_exposure.py
 rsciio/utils/tests.py
 rsciio/utils/tools.py
 rsciio/zspy/__init__.py
 rsciio/zspy/_api.py
```

### Comparing `rosettasciio-0.3/rosettasciio.egg-info/requires.txt` & `rosettasciio-0.4/rosettasciio.egg-info/requires.txt`

 * *Files 12% similar despite different names*

```diff
@@ -52,14 +52,15 @@
 matplotlib-scalebar
 matplotlib>=3.5
 
 [speed]
 numba>=0.52
 
 [tests]
+filelock
 pooch
 pytest>=3.6
 pytest-xdist
 pytest-rerunfailures
 pytest-cov
 setuptools_scm
 
@@ -69,7 +70,8 @@
 
 [usid]
 pyUSID
 sidpy<=0.12.0
 
 [zspy]
 zarr
+msgpack
```

### Comparing `rosettasciio-0.3/rsciio/__init__.py` & `rosettasciio-0.4/rsciio/__init__.py`

 * *Files identical despite different names*

### Comparing `rosettasciio-0.3/rsciio/_docstrings.py` & `rosettasciio-0.4/rsciio/_docstrings.py`

 * *Files 3% similar despite different names*

```diff
@@ -128,8 +128,10 @@
         - 'data' – multidimensional :py:class:`numpy.ndarray` or :py:class:`dask.array.Array`
         - 'axes' – list of dictionaries describing the axes
           containing the fields 'name', 'units', 'index_in_array', and
           either 'size', 'offset', and 'scale' or a numpy array 'axis'
           containing the full axes vector
         - 'metadata' – dictionary containing the parsed metadata
         - 'original_metadata' – dictionary containing the full metadata tree from the input file
+
+        When the file contains several datasets, each dataset will be loaded as separate dictionary.
     """
```

### Comparing `rosettasciio-0.3/rsciio/_hierarchical.py` & `rosettasciio-0.4/rsciio/_hierarchical.py`

 * *Files 8% similar despite different names*

```diff
@@ -38,27 +38,55 @@
 
 _logger = logging.getLogger(__name__)
 
 # Functions to flatten and unflatten the data to allow for storing
 # ragged arrays in hdf5 with dimensionality higher than 1
 
 
-def flatten_data(x):
+def flatten_data(x, is_hdf5=False):
     new_data = np.empty(shape=x.shape, dtype=object)
     shapes = np.empty(shape=x.shape, dtype=object)
     for i in np.ndindex(x.shape):
-        new_data[i] = x[i].ravel()
-        shapes[i] = np.array(x[i].shape)
+        data_ = np.array(x[i]).ravel()
+        if np.issubdtype(data_.dtype, np.dtype("U")):
+            if is_hdf5:
+                # h5py doesn't support numpy unicode dtype, convert to
+                # compatible dtype
+                new_data[i] = data_.astype(h5py.string_dtype())
+            else:
+                # Convert to list to save ragged array of array with string dtype
+                new_data[i] = data_.tolist()
+        else:
+            new_data[i] = data_
+        shapes[i] = np.array(np.array(x[i]).shape)
     return new_data, shapes
 
 
-def unflatten_data(data, shape):
+def unflatten_data(data, shape, is_hdf5=False):
     new_data = np.empty(shape=data.shape, dtype=object)
     for i in np.ndindex(new_data.shape):
-        new_data[i] = np.reshape(data[i], shape[i])
+        try:
+            # For hspy file, ragged array of string are saving with
+            # "h5py.string_dtype()" type and we need to convert it back
+            # to numpy unicode type. The only to know when this needs to be
+            # done is look at the numpy metadata
+            # This numpy feature is "not well supported in numpy"
+            # https://numpy.org/doc/stable/reference/generated/numpy.dtype.metadata.html
+            convert_to_unicode = (
+                is_hdf5
+                and data.dtype is not None
+                and data.dtype.metadata.get("vlen") is not None
+                and data.dtype.metadata["vlen"].metadata.get("vlen") == str
+            )
+        except (AttributeError, KeyError):
+            # AttributeError in case `dtype.metadata`` is None (most of the time)
+            # KeyError in case "vlen" is not a key
+            convert_to_unicode = False
+        data_ = data[i].astype("U") if convert_to_unicode else data[i]
+        new_data[i] = np.reshape(np.array(data_), shape[i])
     return new_data
 
 
 # ---------------------------------
 
 
 def get_signal_chunks(shape, dtype, signal_axes=None, target_size=1e6):
@@ -75,16 +103,17 @@
     signal_axes : {None, iterable of ints}
         The axes defining "signal space" of the dataset. If None, the default
         h5py chunking is performed.
     target_size : int
         The target number of bytes for one chunk
     """
     typesize = np.dtype(dtype).itemsize
-    if signal_axes is None:
-        return h5py._hl.filters.guess_chunk(shape, None, typesize)
+    if shape == (0,) or signal_axes is None:
+        # enable autochunking from h5py
+        return True
 
     # largely based on the guess_chunk in h5py
     bytes_per_signal = np.prod([shape[i] for i in signal_axes]) * typesize
     signals_per_chunk = int(np.floor_divide(target_size, bytes_per_signal))
     navigation_axes = tuple(i for i in range(len(shape)) if i not in signal_axes)
     num_nav_axes = len(navigation_axes)
     num_signals = np.prod([shape[i] for i in navigation_axes])
@@ -128,30 +157,31 @@
         ]
         return tuple(int(x) for x in chunks)
 
 
 class HierarchicalReader:
     """A generic Reader class for reading data from hierarchical file types."""
 
+    _file_type = ""
+    _is_hdf5 = False
+
     def __init__(self, file):
         """
         Initializes a general reader for hierarchical signals.
 
         Parameters
         ----------
         file: str
             A file to be read.
         """
         self.file = file
         # Getting version also check that this is a hyperspy format
         self.version = self.get_format_version()
         self.Dataset = None
         self.Group = None
-        self.unicode_kwds = None
-        self.ragged_kwds = None
 
         if self.version > Version(version):
             warnings.warn(
                 "This file was written using a newer version of the "
                 f"HyperSpy {self._file_type} file format. I will attempt to "
                 "load it, but, if I fail, it is likely that I will be more "
                 "successful at this and other tasks if you upgrade me."
@@ -244,35 +274,41 @@
         exp_dict_list.extend(standalone_models)
 
         if not len(exp_dict_list):
             raise IOError(f"This is not a valid {self._file_type} file.")
 
         return exp_dict_list
 
-    @staticmethod
-    def _read_array(group, dataset_key):
+    def _read_array(self, group, dataset_key):
         # This is a workaround for the lack of support for n-d ragged array
         # in h5py and zarr. There is work in progress for implementation in zarr:
         # https://github.com/zarr-developers/zarr-specs/issues/62 which may be
         # relevant to implement here when available
         data = group[dataset_key]
         key = f"_ragged_shapes_{dataset_key}"
         if "ragged_shapes" in group:
             # For file saved with rosettaSciIO <= 0.1
             # rename from `ragged_shapes` to `_ragged_shapes_{key}` in v3.3
             key = "ragged_shapes"
         if key in group:
             ragged_shape = group[key]
-            # if the data is chunked saved array we must first
-            # cast to a numpy array to avoid multiple calls to
-            # _decode_chunk in zarr (or h5py)
+            # Use same chunks as data so that apply_gufunc doesn't rechunk
+            # Reduces the transfer of data between workers which
+            # significantly improves performance for distributed loading
             data = da.from_array(data, chunks=data.chunks)
-            shape = da.from_array(ragged_shape, chunks=ragged_shape.chunks)
-            shape = shape.rechunk(data.chunks)
-            data = da.apply_gufunc(unflatten_data, "(),()->()", data, shape)
+            shapes = da.from_array(ragged_shape, chunks=data.chunks)
+
+            data = da.apply_gufunc(
+                unflatten_data,
+                "(),()->()",
+                data,
+                shapes,
+                is_hdf5=self._is_hdf5,
+                output_dtypes=object,
+            )
         return data
 
     def group2signaldict(self, group, lazy=False):
         """
         Reads a h5py/zarr group and returns a signal dictionary.
 
         Parameters
@@ -521,15 +557,15 @@
 
     def _group2dict(self, group, dictionary=None, lazy=False):
         if dictionary is None:
             dictionary = {}
         for key, value in group.attrs.items():
             if isinstance(value, bytes):
                 value = value.decode()
-            if isinstance(value, (np.string_, str)):
+            if isinstance(value, (np.bytes_, str)):
                 if value == "_None_":
                     value = None
             elif isinstance(value, np.bool_):
                 value = bool(value)
             elif isinstance(value, np.ndarray) and value.dtype.char == "S":
                 # Convert strings to unicode
                 value = value.astype("U")
@@ -633,14 +669,16 @@
 class HierarchicalWriter:
     """
     An object used to simplify and organize the process for writing a
     Hierarchical signal, such as hspy/zspy format.
     """
 
     target_size = 1e6
+    _unicode_kwds = None
+    _is_hdf5 = False
 
     def __init__(self, file, signal, group, **kwds):
         """Initialize a generic file writer for hierachical data storage types.
 
         Parameters
         ----------
         file: str
@@ -653,16 +691,14 @@
             Any additional keywords used for saving the data.
         """
         self.file = file
         self.signal = signal
         self.group = group
         self.Dataset = None
         self.Group = None
-        self.unicode_kwds = None
-        self.ragged_kwds = None
         self.kwds = kwds
 
     @staticmethod
     def _get_object_dset(*args, **kwargs):  # pragma: no cover
         raise NotImplementedError("This method must be implemented by subclasses.")
 
     @staticmethod
@@ -715,17 +751,15 @@
                 chunks = get_signal_chunks(
                     data.shape, data.dtype, signal_axes, cls.target_size
                 )
         if np.issubdtype(data.dtype, np.dtype("U")):
             # Saving numpy unicode type is not supported in h5py
             data = data.astype(np.dtype("S"))
 
-        if data.dtype == np.dtype("O"):
-            dset = cls._get_object_dset(group, data, key, chunks, **kwds)
-        else:
+        if data.dtype != np.dtype("O"):
             got_data = False
             while not got_data:
                 try:
                     these_kwds = kwds.copy()
                     these_kwds.update(
                         dict(
                             shape=data.shape,
@@ -747,35 +781,32 @@
         _logger.info(f"Chunks used for saving: {chunks}")
         if data.dtype == np.dtype("O"):
             if isinstance(data, da.Array):
                 new_data, shapes = da.apply_gufunc(
                     flatten_data,
                     "()->(),()",
                     data,
-                    dtype=object,
+                    is_hdf5=cls._is_hdf5,
                     output_dtypes=[object, object],
                     allow_rechunk=False,
                 )
             else:
-                new_data = np.empty(shape=data.shape, dtype=object)
-                shapes = np.empty(shape=data.shape, dtype=object)
-                for i in np.ndindex(data.shape):
-                    new_data[i] = data[i].ravel()
-                    shapes[i] = np.array(data[i].shape)
+                new_data, shapes = flatten_data(data, is_hdf5=cls._is_hdf5)
 
+            dset = cls._get_object_dset(group, new_data, key, chunks, **kwds)
             shape_dset = cls._get_object_dset(
-                group, shapes, f"_ragged_shapes_{key}", shapes.shape, **kwds
+                group, shapes, f"_ragged_shapes_{key}", chunks, dtype=int, **kwds
             )
 
             cls._store_data(
                 (new_data, shapes),
                 (dset, shape_dset),
                 group,
                 (key, f"_ragged_shapes_{key}"),
-                (chunks, shapes.shape),
+                (chunks, chunks),
                 show_progressbar,
             )
         else:
             cls._store_data(data, dset, group, key, chunks, show_progressbar)
 
     def write(self):
         self.write_signal(self.signal, self.group, **self.kwds)
@@ -835,16 +866,16 @@
             model_group = self.file.require_group("Analysis/models")
             self.dict2group(signal["models"], model_group, **kwds)
             for model in model_group.values():
                 model.attrs["_signal"] = group.name
 
     def dict2group(self, dictionary, group, **kwds):
         "Recursive writer of dicts and signals"
-
         for key, value in dictionary.items():
+            _logger.debug("Saving item: {}".format(key))
             if isinstance(value, dict):
                 self.dict2group(value, group.require_group(key), **kwds)
             elif isinstance(value, (np.ndarray, self.Dataset, da.Array)):
                 self.overwrite_dataset(group, value, key, **kwds)
 
             elif value is None:
                 group.attrs[key] = "_None_"
@@ -890,24 +921,24 @@
             if np.any([isinstance(t, dict) and "_sig_" in t for t in value]):
                 tmp = np.array([[0]])
             else:
                 tmp = np.array(value)
         except ValueError:
             tmp = np.array([[0]])
 
-        if tmp.dtype == np.dtype("O") or tmp.ndim != 1:
+        if np.issubdtype(tmp.dtype, object) or tmp.ndim != 1:
             self.dict2group(
                 dict(zip([str(i) for i in range(len(value))], value)),
                 group.require_group(_type + str(len(value)) + "_" + key),
                 **kwds,
             )
-        elif tmp.dtype.type is np.unicode_:
+        elif np.issubdtype(tmp.dtype, np.dtype("U")):
             if _type + key in group:
                 del group[_type + key]
             group.create_dataset(
-                _type + key, shape=tmp.shape, **self.unicode_kwds, **kwds
+                _type + key, shape=tmp.shape, **self._unicode_kwds, **kwds
             )
             group[_type + key][:] = tmp[:]
         else:
             if _type + key in group:
                 del group[_type + key]
             group.create_dataset(_type + key, data=tmp, **kwds)
```

### Comparing `rosettasciio-0.3/rsciio/_logger.py` & `rosettasciio-0.4/rsciio/_logger.py`

 * *Files identical despite different names*

### Comparing `rosettasciio-0.3/rsciio/blockfile/_api.py` & `rosettasciio-0.4/rsciio/blockfile/_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -175,22 +175,26 @@
     elif len(nav_axes) == 1:
         NX = nav_axes[0]["size"]
         NY = 1
         SX = nav_axes[0]["scale"]
         SY = SX
     elif len(nav_axes) == 0:
         NX = NY = SX = SY = 1
+    else:
+        raise ValueError(
+            "Number of navigation axes has to be 0, 1 or 2"
+        )  # pragma: no cover
 
     DP_SZ = [axis["size"] for axis in sig_axes][::-1]
     if DP_SZ[0] != DP_SZ[1]:
         raise ValueError("Blockfiles require signal shape to be square!")
     DP_SZ = DP_SZ[0]
     SDP = 100.0 / sig_axes[1]["scale"]
 
-    offset2 = NX * NY + header["Data_offset_1"]
+    offset2 = NX * NY + header["Data_offset_1"][0]
     # Based on inspected files, the DPs are stored at 16-bit boundary...
     # Normally, you'd expect word alignment (32-bits) ¯\_(°_o)_/¯
     offset2 += offset2 % 16
 
     header = dict2sarray(
         {
             "NX": NX,
@@ -405,19 +409,19 @@
         original_scale = intensity_scaling
 
     header, note = get_header_from_signal(signal, endianess=endianess)
     with open(filename, "wb") as f:
         # Write header
         header.tofile(f)
         # Write header note field:
-        if len(note) > int(header["Data_offset_1"]) - f.tell():
-            note = note[: int(header["Data_offset_1"]) - f.tell() - len(note)]
+        if len(note) > int(header["Data_offset_1"][0]) - f.tell():
+            note = note[: int(header["Data_offset_1"][0]) - f.tell() - len(note)]
         f.write(note.encode())
         # Zero pad until next data block
-        zero_pad = int(header["Data_offset_1"]) - f.tell()
+        zero_pad = int(header["Data_offset_1"][0]) - f.tell()
         np.zeros((zero_pad,), np.byte).tofile(f)
         # Write virtual bright field
         if navigator is None:
             navigator = np.zeros((signal["data"].shape[0], signal["data"].shape[1]))
         elif isinstance(navigator, str) and (navigator == "navigator"):
             if smetadata.get("_HyperSpy._sig_navigator", False):
                 navigator = smetadata["_HyperSpy._sig_navigator.data"]
@@ -436,19 +440,19 @@
         if intensity_scaling is not None:
             navigator = rescale_intensity(
                 navigator, in_range=original_scale, out_range=np.uint8
             )
         navigator = navigator.astype(endianess + "u1")
         np.asanyarray(navigator).tofile(f)
         # Zero pad until next data block
-        if f.tell() > int(header["Data_offset_2"]):
+        if f.tell() > int(header["Data_offset_2"][0]):
             raise ValueError(
                 "Signal navigation size does not match " "data dimensions."
             )
-        zero_pad = int(header["Data_offset_2"]) - f.tell()
+        zero_pad = int(header["Data_offset_2"][0]) - f.tell()
         np.zeros((zero_pad,), np.byte).tofile(f)
         file_location = f.tell()
 
     if intensity_scaling is not None:
         array_data = rescale_intensity(
             signal["data"],
             in_range=original_scale,
@@ -463,15 +467,15 @@
     records = array_data.shape[:-2]
     record_dtype = [
         ("MAGIC", endianess + "u2"),
         ("ID", endianess + "u4"),
         ("IMG", endianess + "u1", pixels),
     ]
     magics = np.full(records, 0x55AA, dtype=endianess + "u2")
-    ids = np.arange(np.product(records), dtype=endianess + "u4").reshape(records)
+    ids = np.arange(np.prod(records), dtype=endianess + "u4").reshape(records)
     file_memmap = np.memmap(
         filename, dtype=record_dtype, mode="r+", offset=file_location, shape=records
     )
     file_memmap["MAGIC"] = magics
     file_memmap["ID"] = ids
     if signal["attributes"]["_lazy"]:
         cm = ProgressBar if show_progressbar else dummy_context_manager
```

### Comparing `rosettasciio-0.3/rsciio/bruker/_api.py` & `rosettasciio-0.4/rsciio/bruker/_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -615,14 +615,18 @@
         if "Mag" in self.sem_metadata:
             acq_inst["magnification"] = self.sem_metadata["Mag"]
         if detector:
             eds_metadata = self.get_spectra_metadata(**kwargs)
             det = gen_detector_node(eds_metadata)
             det["EDS"]["real_time"] = self.calc_real_time()
             acq_inst["Detector"] = det
+            # In case of XRF, the primary energy is only defined in
+            # the spectrum metadata
+            acq_inst["beam_energy"] = eds_metadata.hv
+
         return acq_inst
 
     def _parse_image(self, xml_node, overview=False):
         """parse image from bruker xml image node."""
         if overview:
             overlay_node = xml_node.find(
                 "./ChildClassInstances"
@@ -865,15 +869,14 @@
             },
             "mapping": get_mapping(self.mode),
         }
         return i
 
 
 class BCF_reader(SFS_reader):
-
     """Class to read bcf (Bruker hypermapping) file.
 
     Inherits SFS_reader and all its attributes and methods.
 
     Attributes:
     filename
 
@@ -1406,15 +1409,15 @@
 
 
 def bcf_hyperspectra(
     obj_bcf, index=None, downsample=None, cutoff_at_kV=None, lazy=False  # noqa
 ):
     """Returns list of dict with eds hyperspectra and metadata."""
     global warn_once
-    if (fast_unbcf == False) and warn_once:
+    if (fast_unbcf is False) and warn_once:
         _logger.warning(
             """unbcf_fast library is not present...
 Parsing BCF with Python-only backend, which is slow... please wait.
 If parsing is uncomfortably slow, first install cython, then reinstall RosettaSciIO.
 For more information, check the 'Installing RosettaSciIO' section in the documentation."""
         )
         warn_once = False
```

### Comparing `rosettasciio-0.3/rsciio/bruker/unbcf_fast.c` & `rosettasciio-0.4/rsciio/bruker/unbcf_fast.c`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-/* Generated by Cython 3.0.6 */
+/* Generated by Cython 3.0.10 */
 
 /* BEGIN: Cython Metadata
 {
     "distutils": {
         "depends": [],
         "name": "rsciio.bruker.unbcf_fast",
         "sources": [
@@ -33,18 +33,18 @@
     #error Cython requires Python 2.7+ or Python 3.3+.
 #else
 #if defined(CYTHON_LIMITED_API) && CYTHON_LIMITED_API
 #define __PYX_EXTRA_ABI_MODULE_NAME "limited"
 #else
 #define __PYX_EXTRA_ABI_MODULE_NAME ""
 #endif
-#define CYTHON_ABI "3_0_6" __PYX_EXTRA_ABI_MODULE_NAME
+#define CYTHON_ABI "3_0_10" __PYX_EXTRA_ABI_MODULE_NAME
 #define __PYX_ABI_MODULE_NAME "_cython_" CYTHON_ABI
 #define __PYX_TYPE_MODULE_PREFIX __PYX_ABI_MODULE_NAME "."
-#define CYTHON_HEX_VERSION 0x030006F0
+#define CYTHON_HEX_VERSION 0x03000AF0
 #define CYTHON_FUTURE_DIVISION 1
 #include <stddef.h>
 #ifndef offsetof
   #define offsetof(type, member) ( (size_t) & ((type*)0) -> member )
 #endif
 #if !defined(_WIN32) && !defined(WIN32) && !defined(MS_WINDOWS)
   #ifndef __stdcall
@@ -128,14 +128,16 @@
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
   #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
     #define CYTHON_UPDATE_DESCRIPTOR_DOC 0
   #endif
+  #undef CYTHON_USE_FREELISTS
+  #define CYTHON_USE_FREELISTS 0
 #elif defined(PYPY_VERSION)
   #define CYTHON_COMPILING_IN_PYPY 1
   #define CYTHON_COMPILING_IN_CPYTHON 0
   #define CYTHON_COMPILING_IN_LIMITED_API 0
   #define CYTHON_COMPILING_IN_GRAAL 0
   #define CYTHON_COMPILING_IN_NOGIL 0
   #undef CYTHON_USE_TYPE_SLOTS
@@ -189,14 +191,16 @@
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
   #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
     #define CYTHON_UPDATE_DESCRIPTOR_DOC 0
   #endif
+  #undef CYTHON_USE_FREELISTS
+  #define CYTHON_USE_FREELISTS 0
 #elif defined(CYTHON_LIMITED_API)
   #ifdef Py_LIMITED_API
     #undef __PYX_LIMITED_VERSION_HEX
     #define __PYX_LIMITED_VERSION_HEX Py_LIMITED_API
   #endif
   #define CYTHON_COMPILING_IN_PYPY 0
   #define CYTHON_COMPILING_IN_CPYTHON 0
@@ -250,60 +254,83 @@
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
   #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
     #define CYTHON_UPDATE_DESCRIPTOR_DOC 0
   #endif
+  #undef CYTHON_USE_FREELISTS
+  #define CYTHON_USE_FREELISTS 0
 #elif defined(Py_GIL_DISABLED) || defined(Py_NOGIL)
   #define CYTHON_COMPILING_IN_PYPY 0
   #define CYTHON_COMPILING_IN_CPYTHON 0
   #define CYTHON_COMPILING_IN_LIMITED_API 0
   #define CYTHON_COMPILING_IN_GRAAL 0
   #define CYTHON_COMPILING_IN_NOGIL 1
   #ifndef CYTHON_USE_TYPE_SLOTS
     #define CYTHON_USE_TYPE_SLOTS 1
   #endif
+  #ifndef CYTHON_USE_TYPE_SPECS
+    #define CYTHON_USE_TYPE_SPECS 0
+  #endif
   #undef CYTHON_USE_PYTYPE_LOOKUP
   #define CYTHON_USE_PYTYPE_LOOKUP 0
   #ifndef CYTHON_USE_ASYNC_SLOTS
     #define CYTHON_USE_ASYNC_SLOTS 1
   #endif
+  #ifndef CYTHON_USE_PYLONG_INTERNALS
+    #define CYTHON_USE_PYLONG_INTERNALS 0
+  #endif
   #undef CYTHON_USE_PYLIST_INTERNALS
   #define CYTHON_USE_PYLIST_INTERNALS 0
   #ifndef CYTHON_USE_UNICODE_INTERNALS
     #define CYTHON_USE_UNICODE_INTERNALS 1
   #endif
   #undef CYTHON_USE_UNICODE_WRITER
   #define CYTHON_USE_UNICODE_WRITER 0
-  #undef CYTHON_USE_PYLONG_INTERNALS
-  #define CYTHON_USE_PYLONG_INTERNALS 0
   #ifndef CYTHON_AVOID_BORROWED_REFS
     #define CYTHON_AVOID_BORROWED_REFS 0
   #endif
   #ifndef CYTHON_ASSUME_SAFE_MACROS
     #define CYTHON_ASSUME_SAFE_MACROS 1
   #endif
   #ifndef CYTHON_UNPACK_METHODS
     #define CYTHON_UNPACK_METHODS 1
   #endif
   #undef CYTHON_FAST_THREAD_STATE
   #define CYTHON_FAST_THREAD_STATE 0
+  #undef CYTHON_FAST_GIL
+  #define CYTHON_FAST_GIL 0
+  #ifndef CYTHON_METH_FASTCALL
+    #define CYTHON_METH_FASTCALL 1
+  #endif
   #undef CYTHON_FAST_PYCALL
   #define CYTHON_FAST_PYCALL 0
+  #ifndef CYTHON_PEP487_INIT_SUBCLASS
+    #define CYTHON_PEP487_INIT_SUBCLASS 1
+  #endif
   #ifndef CYTHON_PEP489_MULTI_PHASE_INIT
     #define CYTHON_PEP489_MULTI_PHASE_INIT 1
   #endif
+  #ifndef CYTHON_USE_MODULE_STATE
+    #define CYTHON_USE_MODULE_STATE 0
+  #endif
   #ifndef CYTHON_USE_TP_FINALIZE
     #define CYTHON_USE_TP_FINALIZE 1
   #endif
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
+  #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
+    #define CYTHON_UPDATE_DESCRIPTOR_DOC 1
+  #endif
+  #ifndef CYTHON_USE_FREELISTS
+    #define CYTHON_USE_FREELISTS 0
+  #endif
 #else
   #define CYTHON_COMPILING_IN_PYPY 0
   #define CYTHON_COMPILING_IN_CPYTHON 1
   #define CYTHON_COMPILING_IN_LIMITED_API 0
   #define CYTHON_COMPILING_IN_GRAAL 0
   #define CYTHON_COMPILING_IN_NOGIL 0
   #ifndef CYTHON_USE_TYPE_SLOTS
@@ -386,14 +413,17 @@
     #define CYTHON_USE_EXC_INFO_STACK 0
   #elif !defined(CYTHON_USE_EXC_INFO_STACK)
     #define CYTHON_USE_EXC_INFO_STACK 1
   #endif
   #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
     #define CYTHON_UPDATE_DESCRIPTOR_DOC 1
   #endif
+  #ifndef CYTHON_USE_FREELISTS
+    #define CYTHON_USE_FREELISTS 1
+  #endif
 #endif
 #if !defined(CYTHON_FAST_PYCCALL)
 #define CYTHON_FAST_PYCCALL  (CYTHON_FAST_PYCALL && PY_VERSION_HEX >= 0x030600B1)
 #endif
 #if !defined(CYTHON_VECTORCALL)
 #define CYTHON_VECTORCALL  (CYTHON_FAST_PYCCALL && PY_VERSION_HEX >= 0x030800B1)
 #endif
@@ -578,22 +608,22 @@
     static CYTHON_INLINE PyObject* __Pyx_PyCode_New(int a, int p, int k, int l, int s, int f,
                                                     PyObject *code, PyObject *c, PyObject* n, PyObject *v,
                                                     PyObject *fv, PyObject *cell, PyObject* fn,
                                                     PyObject *name, int fline, PyObject *lnos) {
         PyObject *exception_table = NULL;
         PyObject *types_module=NULL, *code_type=NULL, *result=NULL;
         #if __PYX_LIMITED_VERSION_HEX < 0x030B0000
-        PyObject *version_info; // borrowed
+        PyObject *version_info;
         PyObject *py_minor_version = NULL;
         #endif
         long minor_version = 0;
         PyObject *type, *value, *traceback;
         PyErr_Fetch(&type, &value, &traceback);
         #if __PYX_LIMITED_VERSION_HEX >= 0x030B0000
-        minor_version = 11; // we don't yet need to distinguish between versions > 11
+        minor_version = 11;
         #else
         if (!(version_info = PySys_GetObject("version_info"))) goto end;
         if (!(py_minor_version = PySequence_GetItem(version_info, 1))) goto end;
         minor_version = PyLong_AsLong(py_minor_version);
         Py_DECREF(py_minor_version);
         if (minor_version == -1 && PyErr_Occurred()) goto end;
         #endif
@@ -643,15 +673,15 @@
     #endif
 #elif PY_VERSION_HEX >= 0x030B0000
   static CYTHON_INLINE PyCodeObject* __Pyx_PyCode_New(int a, int p, int k, int l, int s, int f,
                                                     PyObject *code, PyObject *c, PyObject* n, PyObject *v,
                                                     PyObject *fv, PyObject *cell, PyObject* fn,
                                                     PyObject *name, int fline, PyObject *lnos) {
     PyCodeObject *result;
-    PyObject *empty_bytes = PyBytes_FromStringAndSize("", 0);  // we don't have access to __pyx_empty_bytes here
+    PyObject *empty_bytes = PyBytes_FromStringAndSize("", 0);
     if (!empty_bytes) return NULL;
     result =
       #if PY_VERSION_HEX >= 0x030C0000
         PyUnstable_Code_NewWithPosOnlyArgs
       #else
         PyCode_NewWithPosOnlyArgs
       #endif
@@ -729,16 +759,21 @@
   #ifndef METH_FASTCALL
      #define METH_FASTCALL 0x80
   #endif
   typedef PyObject *(*__Pyx_PyCFunctionFast) (PyObject *self, PyObject *const *args, Py_ssize_t nargs);
   typedef PyObject *(*__Pyx_PyCFunctionFastWithKeywords) (PyObject *self, PyObject *const *args,
                                                           Py_ssize_t nargs, PyObject *kwnames);
 #else
-  #define __Pyx_PyCFunctionFast _PyCFunctionFast
-  #define __Pyx_PyCFunctionFastWithKeywords _PyCFunctionFastWithKeywords
+  #if PY_VERSION_HEX >= 0x030d00A4
+  #  define __Pyx_PyCFunctionFast PyCFunctionFast
+  #  define __Pyx_PyCFunctionFastWithKeywords PyCFunctionFastWithKeywords
+  #else
+  #  define __Pyx_PyCFunctionFast _PyCFunctionFast
+  #  define __Pyx_PyCFunctionFastWithKeywords _PyCFunctionFastWithKeywords
+  #endif
 #endif
 #if CYTHON_METH_FASTCALL
   #define __Pyx_METH_FASTCALL METH_FASTCALL
   #define __Pyx_PyCFunction_FastCall __Pyx_PyCFunctionFast
   #define __Pyx_PyCFunction_FastCallWithKeywords __Pyx_PyCFunctionFastWithKeywords
 #else
   #define __Pyx_METH_FASTCALL METH_VARARGS
@@ -1082,15 +1117,15 @@
   #define __Pyx_PyList_SET_ITEM(o, i, v) PyList_SetItem(o, i, v)
   #define __Pyx_PyTuple_GET_SIZE(o) PyTuple_Size(o)
   #define __Pyx_PyList_GET_SIZE(o) PyList_Size(o)
   #define __Pyx_PySet_GET_SIZE(o) PySet_Size(o)
   #define __Pyx_PyBytes_GET_SIZE(o) PyBytes_Size(o)
   #define __Pyx_PyByteArray_GET_SIZE(o) PyByteArray_Size(o)
 #endif
-#if PY_VERSION_HEX >= 0x030d00A1
+#if __PYX_LIMITED_VERSION_HEX >= 0x030d00A1
   #define __Pyx_PyImport_AddModuleRef(name) PyImport_AddModuleRef(name)
 #else
   static CYTHON_INLINE PyObject *__Pyx_PyImport_AddModuleRef(const char *name) {
       PyObject *module = PyImport_AddModule(name);
       Py_XINCREF(module);
       return module;
   }
@@ -1169,15 +1204,15 @@
 #if defined(__CYGWIN__) && defined(_LDBL_EQ_DBL)
 #define __Pyx_truncl trunc
 #else
 #define __Pyx_truncl truncl
 #endif
 
 #define __PYX_MARK_ERR_POS(f_index, lineno) \
-    { __pyx_filename = __pyx_f[f_index]; (void)__pyx_filename; __pyx_lineno = lineno; (void)__pyx_lineno; __pyx_clineno = __LINE__; (void)__pyx_clineno; }
+    { __pyx_filename = __pyx_f[f_index]; (void)__pyx_filename; __pyx_lineno = lineno; (void)__pyx_lineno; __pyx_clineno = __LINE__;  (void)__pyx_clineno; }
 #define __PYX_ERR(f_index, lineno, Ln_error) \
     { __PYX_MARK_ERR_POS(f_index, lineno) goto Ln_error; }
 
 #ifdef CYTHON_EXTERN_C
     #undef __PYX_EXTERN_C
     #define __PYX_EXTERN_C CYTHON_EXTERN_C
 #elif defined(__PYX_EXTERN_C)
@@ -1276,32 +1311,15 @@
 #define __Pyx_PyObject_AsSString(s)    ((const signed char*) __Pyx_PyObject_AsString(s))
 #define __Pyx_PyObject_AsUString(s)    ((const unsigned char*) __Pyx_PyObject_AsString(s))
 #define __Pyx_PyObject_FromCString(s)  __Pyx_PyObject_FromString((const char*)s)
 #define __Pyx_PyBytes_FromCString(s)   __Pyx_PyBytes_FromString((const char*)s)
 #define __Pyx_PyByteArray_FromCString(s)   __Pyx_PyByteArray_FromString((const char*)s)
 #define __Pyx_PyStr_FromCString(s)     __Pyx_PyStr_FromString((const char*)s)
 #define __Pyx_PyUnicode_FromCString(s) __Pyx_PyUnicode_FromString((const char*)s)
-#if CYTHON_COMPILING_IN_LIMITED_API
-static CYTHON_INLINE size_t __Pyx_Py_UNICODE_strlen(const wchar_t *u)
-{
-    const wchar_t *u_end = u;
-    while (*u_end++) ;
-    return (size_t)(u_end - u - 1);
-}
-#else
-static CYTHON_INLINE size_t __Pyx_Py_UNICODE_strlen(const Py_UNICODE *u)
-{
-    const Py_UNICODE *u_end = u;
-    while (*u_end++) ;
-    return (size_t)(u_end - u - 1);
-}
-#endif
 #define __Pyx_PyUnicode_FromOrdinal(o)       PyUnicode_FromOrdinal((int)o)
-#define __Pyx_PyUnicode_FromUnicode(u)       PyUnicode_FromUnicode(u, __Pyx_Py_UNICODE_strlen(u))
-#define __Pyx_PyUnicode_FromUnicodeAndLength PyUnicode_FromUnicode
 #define __Pyx_PyUnicode_AsUnicode            PyUnicode_AsUnicode
 #define __Pyx_NewRef(obj) (Py_INCREF(obj), obj)
 #define __Pyx_Owned_Py_None(b) __Pyx_NewRef(Py_None)
 static CYTHON_INLINE PyObject * __Pyx_PyBool_FromLong(long b);
 static CYTHON_INLINE int __Pyx_PyObject_IsTrue(PyObject*);
 static CYTHON_INLINE int __Pyx_PyObject_IsTrueAndDecref(PyObject*);
 static CYTHON_INLINE PyObject* __Pyx_PyNumber_IntOrLong(PyObject* x);
@@ -1343,15 +1361,15 @@
     #define __Pyx_PyLong_CompactValue(x)  PyUnstable_Long_CompactValue((PyLongObject*) x)
   #else
     #define __Pyx_PyLong_IsCompact(x)     (((PyLongObject*)x)->long_value.lv_tag < (2 << _PyLong_NON_SIZE_BITS))
     #define __Pyx_PyLong_CompactValue(x)  ((1 - (Py_ssize_t) __Pyx_PyLong_Sign(x)) * (Py_ssize_t) __Pyx_PyLong_Digits(x)[0])
   #endif
   typedef Py_ssize_t  __Pyx_compact_pylong;
   typedef size_t  __Pyx_compact_upylong;
-  #else  // Py < 3.12
+  #else
   #define __Pyx_PyLong_IsNeg(x)  (Py_SIZE(x) < 0)
   #define __Pyx_PyLong_IsNonNeg(x)  (Py_SIZE(x) >= 0)
   #define __Pyx_PyLong_IsZero(x)  (Py_SIZE(x) == 0)
   #define __Pyx_PyLong_IsPos(x)  (Py_SIZE(x) > 0)
   #define __Pyx_PyLong_CompactValueUnsigned(x)  ((Py_SIZE(x) == 0) ? 0 : __Pyx_PyLong_Digits(x)[0])
   #define __Pyx_PyLong_DigitCount(x)  __Pyx_sst_abs(Py_SIZE(x))
   #define __Pyx_PyLong_SignedDigitCount(x)  Py_SIZE(x)
@@ -1985,16 +2003,16 @@
 #else
     #define __Pyx_Arg_VARARGS(args, i) PyTuple_GetItem(args, i)
 #endif
 #if CYTHON_AVOID_BORROWED_REFS
     #define __Pyx_Arg_NewRef_VARARGS(arg) __Pyx_NewRef(arg)
     #define __Pyx_Arg_XDECREF_VARARGS(arg) Py_XDECREF(arg)
 #else
-    #define __Pyx_Arg_NewRef_VARARGS(arg) arg // no-op
-    #define __Pyx_Arg_XDECREF_VARARGS(arg) // no-op - arg is borrowed
+    #define __Pyx_Arg_NewRef_VARARGS(arg) arg
+    #define __Pyx_Arg_XDECREF_VARARGS(arg)
 #endif
 #define __Pyx_NumKwargs_VARARGS(kwds) PyDict_Size(kwds)
 #define __Pyx_KwValues_VARARGS(args, nargs) NULL
 #define __Pyx_GetKwValue_VARARGS(kw, kwvalues, s) __Pyx_PyDict_GetItemStrWithError(kw, s)
 #define __Pyx_KwargsAsDict_VARARGS(kw, kwvalues) PyDict_Copy(kw)
 #if CYTHON_METH_FASTCALL
     #define __Pyx_Arg_FASTCALL(args, i) args[i]
@@ -2002,16 +2020,17 @@
     #define __Pyx_KwValues_FASTCALL(args, nargs) ((args) + (nargs))
     static CYTHON_INLINE PyObject * __Pyx_GetKwValue_FASTCALL(PyObject *kwnames, PyObject *const *kwvalues, PyObject *s);
 #if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX >= 0x030d0000
     CYTHON_UNUSED static PyObject *__Pyx_KwargsAsDict_FASTCALL(PyObject *kwnames, PyObject *const *kwvalues);
   #else
     #define __Pyx_KwargsAsDict_FASTCALL(kw, kwvalues) _PyStack_AsDict(kwvalues, kw)
   #endif
-    #define __Pyx_Arg_NewRef_FASTCALL(arg) arg // no-op, __Pyx_Arg_FASTCALL is direct and this needs
-    #define __Pyx_Arg_XDECREF_FASTCALL(arg)  // no-op - arg was returned from array
+    #define __Pyx_Arg_NewRef_FASTCALL(arg) arg  /* no-op, __Pyx_Arg_FASTCALL is direct and this needs
+                                                   to have the same reference counting */
+    #define __Pyx_Arg_XDECREF_FASTCALL(arg)
 #else
     #define __Pyx_Arg_FASTCALL __Pyx_Arg_VARARGS
     #define __Pyx_NumKwargs_FASTCALL __Pyx_NumKwargs_VARARGS
     #define __Pyx_KwValues_FASTCALL __Pyx_KwValues_VARARGS
     #define __Pyx_GetKwValue_FASTCALL __Pyx_GetKwValue_VARARGS
     #define __Pyx_KwargsAsDict_FASTCALL __Pyx_KwargsAsDict_VARARGS
     #define __Pyx_Arg_NewRef_FASTCALL(arg) __Pyx_Arg_NewRef_VARARGS(arg)
@@ -2562,15 +2581,15 @@
     PyObject *func_code;
     PyObject *func_closure;
 #if PY_VERSION_HEX < 0x030900B1 || CYTHON_COMPILING_IN_LIMITED_API
     PyObject *func_classobj;
 #endif
     void *defaults;
     int defaults_pyobjects;
-    size_t defaults_size;  // used by FusedFunction for copying defaults
+    size_t defaults_size;
     int flags;
     PyObject *defaults_tuple;
     PyObject *defaults_kwdict;
     PyObject *(*defaults_getter)(PyObject *);
     PyObject *func_annotations;
     PyObject *func_is_coroutine;
 } __pyx_CyFunctionObject;
@@ -25189,15 +25208,15 @@
   #if PY_MAJOR_VERSION < 3
   __pyx_m = Py_InitModule4("unbcf_fast", __pyx_methods, 0, 0, PYTHON_API_VERSION); Py_XINCREF(__pyx_m);
   if (unlikely(!__pyx_m)) __PYX_ERR(1, 1, __pyx_L1_error)
   #elif CYTHON_USE_MODULE_STATE
   __pyx_t_1 = PyModule_Create(&__pyx_moduledef); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 1, __pyx_L1_error)
   {
     int add_module_result = PyState_AddModule(__pyx_t_1, &__pyx_moduledef);
-    __pyx_t_1 = 0; /* transfer ownership from __pyx_t_1 to unbcf_fast pseudovariable */
+    __pyx_t_1 = 0; /* transfer ownership from __pyx_t_1 to "unbcf_fast" pseudovariable */
     if (unlikely((add_module_result < 0))) __PYX_ERR(1, 1, __pyx_L1_error)
     pystate_addmodule_run = 1;
   }
   #else
   __pyx_m = PyModule_Create(&__pyx_moduledef);
   if (unlikely(!__pyx_m)) __PYX_ERR(1, 1, __pyx_L1_error)
   #endif
@@ -26334,19 +26353,19 @@
     {
         if (s == PyTuple_GET_ITEM(kwnames, i)) return kwvalues[i];
     }
     for (i = 0; i < n; i++)
     {
         int eq = __Pyx_PyUnicode_Equals(s, PyTuple_GET_ITEM(kwnames, i), Py_EQ);
         if (unlikely(eq != 0)) {
-            if (unlikely(eq < 0)) return NULL;  // error
+            if (unlikely(eq < 0)) return NULL;
             return kwvalues[i];
         }
     }
-    return NULL;  // not found (no exception set)
+    return NULL;
 }
 #if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX >= 0x030d0000
 CYTHON_UNUSED static PyObject *__Pyx_KwargsAsDict_FASTCALL(PyObject *kwnames, PyObject *const *kwvalues) {
     Py_ssize_t i, nkwargs = PyTuple_GET_SIZE(kwnames);
     PyObject *dict;
     dict = PyDict_New();
     if (unlikely(!dict))
@@ -26451,15 +26470,15 @@
 #endif
         }
         name = first_kw_arg;
         while (*name && (**name != key)) name++;
         if (*name) {
             values[name-argnames] = value;
 #if CYTHON_AVOID_BORROWED_REFS
-            Py_INCREF(value); // transfer ownership of value to values
+            Py_INCREF(value);
             Py_DECREF(key);
 #endif
             key = NULL;
             value = NULL;
             continue;
         }
 #if !CYTHON_AVOID_BORROWED_REFS
@@ -26470,15 +26489,15 @@
         #if PY_MAJOR_VERSION < 3
         if (likely(PyString_Check(key))) {
             while (*name) {
                 if ((CYTHON_COMPILING_IN_PYPY || PyString_GET_SIZE(**name) == PyString_GET_SIZE(key))
                         && _PyString_Eq(**name, key)) {
                     values[name-argnames] = value;
 #if CYTHON_AVOID_BORROWED_REFS
-                    value = NULL;  // ownership transferred to values
+                    value = NULL;
 #endif
                     break;
                 }
                 name++;
             }
             if (*name) continue;
             else {
@@ -26502,15 +26521,15 @@
                 #endif
                     PyUnicode_Compare(**name, key)
                 );
                 if (cmp < 0 && unlikely(PyErr_Occurred())) goto bad;
                 if (cmp == 0) {
                     values[name-argnames] = value;
 #if CYTHON_AVOID_BORROWED_REFS
-                    value = NULL; // ownership transferred to values
+                    value = NULL;
 #endif
                     break;
                 }
                 name++;
             }
             if (*name) continue;
             else {
@@ -28555,17 +28574,18 @@
     __Pyx_DECREF_TypeName(obj_type_name);
 bad:
     return NULL;
 }
 
 /* IterFinish */
 static CYTHON_INLINE int __Pyx_IterFinish(void) {
+    PyObject* exc_type;
     __Pyx_PyThreadState_declare
     __Pyx_PyThreadState_assign
-    PyObject* exc_type = __Pyx_PyErr_CurrentExceptionType();
+    exc_type = __Pyx_PyErr_CurrentExceptionType();
     if (unlikely(exc_type)) {
         if (unlikely(!__Pyx_PyErr_GivenExceptionMatches(exc_type, PyExc_StopIteration)))
             return -1;
         __Pyx_PyErr_Clear();
         return 0;
     }
     return 0;
@@ -30180,15 +30200,15 @@
         break;
     case 0:
         self = ((PyCFunctionObject*)cyfunc)->m_self;
         break;
     default:
         return NULL;
     }
-    return ((_PyCFunctionFastWithKeywords)(void(*)(void))def->ml_meth)(self, args, nargs, kwnames);
+    return ((__Pyx_PyCFunctionFastWithKeywords)(void(*)(void))def->ml_meth)(self, args, nargs, kwnames);
 }
 static PyObject * __Pyx_CyFunction_Vectorcall_FASTCALL_KEYWORDS_METHOD(PyObject *func, PyObject *const *args, size_t nargsf, PyObject *kwnames)
 {
     __pyx_CyFunctionObject *cyfunc = (__pyx_CyFunctionObject *)func;
     PyMethodDef* def = ((PyCFunctionObject*)cyfunc)->m_ml;
     PyTypeObject *cls = (PyTypeObject *) __Pyx_CyFunction_GetClassObj(cyfunc);
 #if CYTHON_BACKPORT_VECTORCALL
@@ -30639,15 +30659,15 @@
         py_line,
         __pyx_empty_bytes  /*PyObject *lnotab*/
     );
     Py_DECREF(py_srcfile);
     #else
     py_code = PyCode_NewEmpty(filename, funcname, py_line);
     #endif
-    Py_XDECREF(py_funcname);  // XDECREF since it's only set on Py3 if cline
+    Py_XDECREF(py_funcname);
     return py_code;
 bad:
     Py_XDECREF(py_funcname);
     #if PY_MAJOR_VERSION < 3
     Py_XDECREF(py_srcfile);
     #endif
     return NULL;
```

### Comparing `rosettasciio-0.3/rsciio/bruker/unbcf_fast.pyx` & `rosettasciio-0.4/rsciio/bruker/unbcf_fast.pyx`

 * *Files identical despite different names*

### Comparing `rosettasciio-0.3/rsciio/dens/_api.py` & `rosettasciio-0.4/rsciio/dens/_api.py`

 * *Files identical despite different names*

### Comparing `rosettasciio-0.3/rsciio/digitalmicrograph/_api.py` & `rosettasciio-0.4/rsciio/digitalmicrograph/_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -34,15 +34,14 @@
 from box import Box
 
 
 _logger = logging.getLogger(__name__)
 
 
 class DigitalMicrographReader(object):
-
     """Class to read Gatan Digital Micrograph (TM) files.
 
     Currently it supports versions 3 and 4.
 
     Attributes
     ----------
     dm_version, endian, tags_dict
@@ -1149,17 +1148,17 @@
                         tags_path
                     ): ("Acquisition_instrument.Detector.sensor_roi", None),
                     "{}.Acquisition.Parameters.High_Level.Processing".format(
                         tags_path
                     ): ("Acquisition_instrument.Detector.processing", None),
                     "{}.Acquisition.Device.CCD.Pixel_Size_um".format(tags_path): (
                         "Acquisition_instrument.Detector.pixel_size",
-                        lambda x: x[0]
-                        if (isinstance(x, tuple) and x[0] == x[1])
-                        else x,
+                        lambda x: (
+                            x[0] if (isinstance(x, tuple) and x[0] == x[1]) else x
+                        ),
                     ),
                     # Serial Spectrum
                     "{}.CL.Acquisition.Acquisition_begin".format(tags_path): (
                         "General.date",
                         self._get_date,
                     ),
                     "{}.CL.Acquisition.Dwell_time_(s)".format(tags_path): (
```

### Comparing `rosettasciio-0.3/rsciio/digitalsurf/_api.py` & `rosettasciio-0.4/rsciio/digitalsurf/_api.py`

 * *Files identical despite different names*

### Comparing `rosettasciio-0.3/rsciio/edax/_api.py` & `rosettasciio-0.4/rsciio/edax/_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -856,15 +856,15 @@
             original_metadata["ipr_header"] = sarray2dict(ipr_header)
 
             # Workaround for type error when saving hdf5:
             # save as list of strings instead of numpy unicode array
             # see https://github.com/hyperspy/hyperspy/pull/2007 and
             #     https://github.com/h5py/h5py/issues/289 for context
             original_metadata["ipr_header"]["charText"] = [
-                np.string_(i) for i in original_metadata["ipr_header"]["charText"]
+                np.bytes_(i) for i in original_metadata["ipr_header"]["charText"]
             ]
     else:
         _logger.warning(
             "Could not find .ipr file named {}.\n"
             "No spatial calibration will be loaded."
             "\n".format(ipr_fname)
         )
@@ -884,17 +884,17 @@
         )
 
     # create the energy axis dictionary:
     energy_axis = {
         "size": data.shape[2],
         "index_in_array": 2,
         "name": "Energy",
-        "scale": original_metadata["spc_header"]["evPerChan"] / 1000.0
-        if read_spc
-        else 1,
+        "scale": (
+            original_metadata["spc_header"]["evPerChan"] / 1000.0 if read_spc else 1
+        ),
         "offset": original_metadata["spc_header"]["startEnergy"] if read_spc else 1,
         "units": "keV" if read_spc else None,
         "navigate": False,
     }
 
     nav_units = "µm"
     # Create navigation axes dictionaries:
```

### Comparing `rosettasciio-0.3/rsciio/emd/_api.py` & `rosettasciio-0.4/rsciio/emd/_api.py`

 * *Files identical despite different names*

### Comparing `rosettasciio-0.3/rsciio/emd/_emd_ncem.py` & `rosettasciio-0.4/rsciio/emd/_emd_ncem.py`

 * *Files 0% similar despite different names*

```diff
@@ -39,15 +39,14 @@
 
 EMD_VERSION = "0.2"
 
 _logger = logging.getLogger(__name__)
 
 
 class EMD_NCEM:
-
     """Class for reading and writing the Berkeley variant of the electron
     microscopy datasets (EMD) file format. It reads files EMD NCEM, including
     files generated by the prismatic software.
 
     Attributes
     ----------
     dictionaries: list
```

### Comparing `rosettasciio-0.3/rsciio/emd/_emd_velox.py` & `rosettasciio-0.4/rsciio/emd/_emd_velox.py`

 * *Files 4% similar despite different names*

```diff
@@ -42,23 +42,39 @@
 from rsciio.utils.tools import _UREG
 from rsciio.utils.elements import atomic_number2name
 
 
 _logger = logging.getLogger(__name__)
 
 
+def _parse_json(v, encoding="utf-8"):
+    return json.loads(v.decode(encoding))
+
+
 def _get_detector_metadata_dict(om, detector_name):
     detectors_dict = om["Detectors"]
     # find detector dict from the detector_name
     for key in detectors_dict:
         if detectors_dict[key]["DetectorName"] == detector_name:
             return detectors_dict[key]
     return None
 
 
+PRUNE_WARNING = (
+    "No spectrum stream is present in the file and the "
+    "spectrum images are saved in a proprietary format, "
+    "which is not supported by RosettaSciIO. This is "
+    "because it has been 'pruned' or saved a different "
+    "software than Velox, e.g. bcf to emd converter. "
+    "If you want to open this data don't prune the "
+    "file or read bcf file directly (in case the bcf "
+    "to emd converter was used)."
+)
+
+
 class FeiEMDReader(object):
     """
     Class for reading FEI electron microscopy datasets.
 
     The :class:`~.FeiEMDReader` reads EMD files saved by the FEI Velox
     software package.
 
@@ -96,23 +112,31 @@
         self.sum_EDS_detectors = sum_EDS_detectors
         self.rebin_energy = rebin_energy
         self.SI_data_dtype = SI_dtype
         self.load_SI_image_stack = load_SI_image_stack
         self.lazy = lazy
         self.detector_name = None
         self.original_metadata = {}
+        # UUID: label mapping
+        self._map_label_dict = {}
 
     def read_file(self, f):
         self.filename = f.filename
+        self.version = _parse_json(f["Version"][0])["version"]
         self.d_grp = f.get("Data")
         self._check_im_type()
-        self._parse_metadata_group(f.get("Operations"), "Operations")
+        for key in ["Displays", "Operations", "SharedProperties", "Features"]:
+            # In Velox emd v11, the "Operation" group is removed:
+            # 'operation settings' are moved to \SharedProperties
+            # \Features link to \SharedProperties\DataReference
+            # in version <11 \Features linked to \Operations
+            if key in f.keys():
+                self._parse_metadata_group(f.get(key), key)
         if self.im_type == "SpectrumStream":
-            self.p_grp = f.get("Presentation")
-            self._parse_image_display()
+            self._parse_image_display(f)
         self._read_data(self.select_type)
 
     def _read_data(self, select_type):
         self.load_images = self.load_SI = self.load_single_spectrum = True
         if select_type == "single_spectrum":
             self.load_images = self.load_SI = False
         elif select_type == "images":
@@ -237,15 +261,20 @@
         """Return a dictionary ready to parse of return to io module"""
         image_sub_group = image_group[image_sub_group_key]
         original_metadata = _parse_metadata(image_group, image_sub_group_key)
         original_metadata.update(self.original_metadata)
 
         # Can be used in more recent version of velox emd files
         self.detector_information = self._get_detector_information(original_metadata)
-        self.detector_name = self._get_detector_name(image_sub_group_key)
+        try:
+            self.detector_name = self._get_detector_name(image_sub_group_key)
+        except KeyError:
+            # File version >= 11 doesn't have the "Operations" group anymore
+            if self.detector_information is not None:
+                self.detector_name = self.detector_information["DetectorName"]
 
         read_stack = self.load_SI_image_stack or self.im_type == "Image"
         h5data = image_sub_group["Data"]
         # Get the scanning area shape of the SI from the images
         self.spatial_shape = h5data.shape[:-1]
         # For Velox FFT data, dtype must be specified and lazy is not
         # supported due to special dtype. The data is loaded as-is; to get
@@ -362,17 +391,16 @@
         )
 
         md = self._get_metadata_dict(original_metadata)
         if self.detector_name is not None:
             original_metadata["DetectorMetadata"] = _get_detector_metadata_dict(
                 original_metadata, self.detector_name
             )
-        if hasattr(self, "map_label_dict"):
-            if image_sub_group_key in self.map_label_dict:
-                md["General"]["title"] = self.map_label_dict[image_sub_group_key]
+        if image_sub_group_key in self._map_label_dict:
+            md["General"]["title"] = self._map_label_dict[image_sub_group_key]
 
         return {
             "data": data,
             "axes": axes,
             "metadata": md,
             "original_metadata": original_metadata,
             "mapping": self._get_mapping(
@@ -459,54 +487,68 @@
             time_unit = "s"
         except KeyError:
             frame_time, time_unit = None, None
 
         frame_time, time_unit = self._convert_scale_units(frame_time, time_unit, factor)
         return frame_time, time_unit
 
-    def _parse_image_display(self):
-        try:
-            image_display_group = self.p_grp.get("Displays/ImageDisplay")
+    def _parse_image_display(self, f):
+        if int(self.version) >= 11:
+            # - /Displays/ImageDisplay contains the list of all the image displays.
+            #   A EDS Map is just an image display.
+            # - These entries contain a json encoded dictionary that contains
+            #   'data', 'id', 'settings' and 'title'.
+            # - The 'id' is the name of the element. 'data' is pointing to the
+            #   data reference in SharedProperties/ImageSeriesDataReference/<UUID>
+            #   which in turn is pointing to the /Data/Image/<UUID> where the image
+            #   data is located.
+            om_image_display = self.original_metadata["Displays"]["ImageDisplay"]
+            self._map_label_dict = {}
+            for v in om_image_display.values():
+                if "data" in v.keys():
+                    data_key = _parse_json(f.get(v["data"])[0])["dataPath"]
+                    self._map_label_dict[data_key.split("/")[-1]] = v["id"]
+
+        else:
+            image_display_group = f.get("Presentation/Displays/ImageDisplay")
             key_list = _get_keys_from_group(image_display_group)
-            self.map_label_dict = {}
+
             for key in key_list:
-                v = json.loads(image_display_group[key][0].decode("utf-8"))
+                v = _parse_json(image_display_group[key][0])
                 data_key = v["dataPath"].split("/")[-1]  # key in data group
-                self.map_label_dict[data_key] = v["display"]["label"]
-        except KeyError:
-            _logger.warning("The image label can't be read from the metadata.")
+                self._map_label_dict[data_key] = v["display"]["label"]
 
     def _parse_metadata_group(self, group, group_name):
         d = {}
         try:
             for group_key in _get_keys_from_group(group):
                 subgroup = group.get(group_key)
                 if hasattr(subgroup, "keys"):
                     sub_dict = {}
                     for subgroup_key in _get_keys_from_group(subgroup):
-                        v = json.loads(subgroup[subgroup_key][0].decode("utf-8"))
+                        v = _parse_json(subgroup[subgroup_key][0])
                         sub_dict[subgroup_key] = v
                 else:
-                    sub_dict = json.loads(subgroup[0].decode("utf-8"))
+                    sub_dict = _parse_json(subgroup[0])
                 d[group_key] = sub_dict
         except IndexError:
             _logger.warning("Some metadata can't be read.")
         self.original_metadata.update({group_name: d})
 
     def _read_spectrum_stream(self):
         if not self.load_SI:
             return
         self.detector_name = "EDS"
         # Try to read the number of frames from Data/SpectrumImage
         try:
             sig = self.d_grp["SpectrumImage"]
             self.number_of_frames = int(
-                json.loads(
-                    sig[next(iter(sig))]["SpectrumImageSettings"][0].decode("utf8")
-                )["endFramePosition"]
+                _parse_json(sig[next(iter(sig))]["SpectrumImageSettings"][0])[
+                    "endFramePosition"
+                ]
             )
         except Exception:
             _logger.exception(
                 "Failed to read the number of frames from Data/SpectrumImage"
             )
             self.number_of_frames = None
         if self.last_frame is None:
@@ -514,30 +556,31 @@
         elif self.number_of_frames and self.last_frame > self.number_of_frames:
             raise ValueError(
                 "The `last_frame` cannot be greater than"
                 " the number of frames, %i for this file." % self.number_of_frames
             )
 
         spectrum_stream_group = self.d_grp.get("SpectrumStream")
-        if spectrum_stream_group is None:
-            _logger.warning(
-                "No spectrum stream is present in the file. It "
-                "is possible that the file has been pruned: use "
-                "Velox to read the spectrum image (proprietary "
-                "format). If you want to open FEI emd file with "
-                "HyperSpy don't prune the file when saving it in "
-                "Velox."
-            )
+        if spectrum_stream_group is None:  # pragma: no cover
+            # "Pruned" file, EDS SI data are in the
+            # "SpectrumImage" group
+            _logger.warning(PRUNE_WARNING)
+            return
+
+        subgroup_keys = _get_keys_from_group(spectrum_stream_group)
+        if len(subgroup_keys) == 0:
+            # "Pruned" file: in Velox emd v11, the "SpectrumStream"
+            # group exists but it is empty
+            _logger.warning(PRUNE_WARNING)
             return
 
         def _read_stream(key):
             stream = FeiSpectrumStream(spectrum_stream_group[key], self)
             return stream
 
-        subgroup_keys = _get_keys_from_group(spectrum_stream_group)
         if self.sum_EDS_detectors:
             if len(subgroup_keys) == 1:
                 _logger.warning("The file contains only one spectrum stream")
             # Read the first stream
             s0 = _read_stream(subgroup_keys[0])
             streams = [s0]
             # add other stream streams
@@ -847,15 +890,15 @@
     """
 
     def __init__(self, stream_group, reader):
         self.reader = reader
         self.stream_group = stream_group
         # Parse acquisition settings to get bin_count and dtype
         acquisition_settings_group = stream_group["AcquisitionSettings"]
-        acquisition_settings = json.loads(acquisition_settings_group[0].decode("utf-8"))
+        acquisition_settings = _parse_json(acquisition_settings_group[0])
         self.bin_count = int(acquisition_settings["bincount"])
         if self.bin_count % self.reader.rebin_energy != 0:
             raise ValueError(
                 "The `rebin_energy` needs to be a divisor of the",
                 " total number of channels.",
             )
         if self.reader.SI_data_dtype is None:
```

### Comparing `rosettasciio-0.3/rsciio/empad/_api.py` & `rosettasciio-0.4/rsciio/empad/_api.py`

 * *Files identical despite different names*

### Comparing `rosettasciio-0.3/rsciio/hamamatsu/_api.py` & `rosettasciio-0.4/rsciio/hamamatsu/_api.py`

 * *Files identical despite different names*

### Comparing `rosettasciio-0.3/rsciio/hspy/_api.py` & `rosettasciio-0.4/rsciio/hspy/_api.py`

 * *Files 5% similar despite different names*

```diff
@@ -44,36 +44,36 @@
 
 current_file_version = None  # Format version of the file being read
 default_version = Version(version)
 
 
 class HyperspyReader(HierarchicalReader):
     _file_type = "hspy"
+    _is_hdf5 = True
 
     def __init__(self, file):
         super().__init__(file)
         self.Dataset = h5py.Dataset
         self.Group = h5py.Group
-        self.unicode_kwds = {"dtype": h5py.special_dtype(vlen=str)}
 
 
 class HyperspyWriter(HierarchicalWriter):
     """
     An object used to simplify and organize the process for
     writing a hyperspy signal.  (.hspy format)
     """
 
     target_size = 1e6
+    _unicode_kwds = {"dtype": h5py.string_dtype()}
+    _is_hdf5 = True
 
     def __init__(self, file, signal, expg, **kwds):
         super().__init__(file, signal, expg, **kwds)
         self.Dataset = h5py.Dataset
         self.Group = h5py.Group
-        self.unicode_kwds = {"dtype": h5py.special_dtype(vlen=str)}
-        self.ragged_kwds = {"dtype": h5py.special_dtype(vlen=signal["data"][0].dtype)}
 
     @staticmethod
     def _store_data(data, dset, group, key, chunks, show_progressbar=True):
         # Tuple of dask arrays can also be passed, in which case the task graphs
         # are merged and the data is written in a single `da.store` call.
         # This is useful when saving a ragged array, where we need to write
         # the data and the shape at the same time as the ragged array must have
@@ -83,48 +83,52 @@
         elif not isinstance(data, list):
             data = [
                 data,
             ]
             dset = [
                 dset,
             ]
+
         for i, (data_, dset_) in enumerate(zip(data, dset)):
             if isinstance(data_, da.Array):
                 if data_.chunks != dset_.chunks:
                     data[i] = data_.rechunk(dset_.chunks)
                 if data_.ndim == 1 and data_.dtype == object:
+                    # https://github.com/hyperspy/rosettasciio/issues/198
                     raise ValueError(
                         "Saving a 1-D ragged dask array to hspy is not supported yet. "
                         "Please use the .zspy extension."
                     )
                 # for performance reason, we write the data later, with all data
                 # at the same time in a single `da.store` call
-            elif data_.flags.c_contiguous:
+            # "write_direct" doesn't play well with empty array
+            elif data_.flags.c_contiguous and data_.shape != (0,):
                 dset_.write_direct(data_)
             else:
                 dset_[:] = data_
         if isinstance(data[0], da.Array):
             cm = ProgressBar if show_progressbar else dummy_context_manager
             with cm():
                 # da.store of tuple helps to merge task graphs and avoid computing twice
                 da.store(data, dset)
 
     @staticmethod
-    def _get_object_dset(group, data, key, chunks, **kwds):
+    def _get_object_dset(group, data, key, chunks, dtype=None, **kwds):
         """Creates a h5py dataset object for saving ragged data"""
-        # For saving ragged array
-        if chunks is None:
+        if chunks is None:  # pragma: no cover
             chunks = 1
-        test_ind = data.ndim * (0,)
-        if isinstance(data, da.Array):
-            dtype = data[test_ind].compute().dtype
-        else:
-            dtype = data[test_ind].dtype
+
+        if dtype is None:
+            test_data = data[data.ndim * (0,)]
+            if isinstance(test_data, da.Array):
+                test_data = test_data.compute()
+            dtype = test_data.dtype
+
         dset = group.require_dataset(
-            key, data.shape, dtype=h5py.special_dtype(vlen=dtype), chunks=chunks, **kwds
+            key, data.shape, dtype=h5py.vlen_dtype(dtype), chunks=chunks, **kwds
         )
         return dset
 
 
 def file_reader(filename, lazy=False, **kwds):
     """
     Read data from hdf5-files saved with the HyperSpy hdf5-format
@@ -144,17 +148,22 @@
         import hdf5plugin
     except ImportError:
         pass
     mode = kwds.pop("mode", "r")
     f = h5py.File(filename, mode=mode, **kwds)
 
     reader = HyperspyReader(f)
-    exp_dict_list = reader.read(lazy=lazy)
-    if not lazy:
-        f.close()
+    # Use try, except, finally to close file when an error is raised
+    try:
+        exp_dict_list = reader.read(lazy=lazy)
+    except BaseException as err:
+        raise err
+    finally:
+        if not lazy:
+            f.close()
 
     return exp_dict_list
 
 
 file_reader.__doc__ %= (FILENAME_DOC, LAZY_DOC, RETURNS_DOC)
 
 
@@ -240,18 +249,22 @@
         expg,
         chunks=chunks,
         compression=compression,
         write_dataset=write_dataset,
         show_progressbar=show_progressbar,
         **kwds,
     )
-    writer.write()
-
-    if close_file:
-        f.close()
+    # Use try, except, finally to close file when an error is raised
+    try:
+        writer.write()
+    except BaseException as err:
+        raise err
+    finally:
+        if close_file:
+            f.close()
 
 
 file_writer.__doc__ %= (
     FILENAME_DOC.replace("read", "write to"),
     SIGNAL_DOC,
     CHUNKS_DOC,
     COMPRESSION_HDF5_DOC,
```

### Comparing `rosettasciio-0.3/rsciio/image/_api.py` & `rosettasciio-0.4/rsciio/image/_api.py`

 * *Files 3% similar despite different names*

```diff
@@ -12,26 +12,29 @@
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with RosettaSciIO. If not, see <https://www.gnu.org/licenses/#GPL>.
 
+from collections.abc import Iterable
 import os
 import logging
 
 import imageio.v3 as iio
+from PIL import Image
 import numpy as np
 
 from rsciio._docstrings import (
     FILENAME_DOC,
     LAZY_DOC,
     RETURNS_DOC,
     SIGNAL_DOC,
 )
+from rsciio.utils.image import _parse_axes_from_metadata, _parse_exif_tags
 from rsciio.utils.tools import _UREG
 
 
 _logger = logging.getLogger(__name__)
 
 
 def file_writer(
@@ -60,24 +63,24 @@
     scalebar_kwds : dict, optional
         Dictionary of keyword arguments for the scalebar. Useful to set
         formatting, location, etc. of the scalebar. See the documentation of
         the 'matplotlib-scalebar' library for more information.
     output_size : {2-tuple, int, None}, Default=None
         The output size of the image in pixels (width, height):
 
-            * if ``int``, defines the width of the image, the height is
-              determined from the aspec ratio of the image
-            * if ``2-tuple``, defines the width and height of the
-              image. Padding with white pixels is used to maintain the aspect
-              ratio of the image.
-            * if ``None``, the size of the data is used.
+        * if ``int``, defines the width of the image, the height is
+          determined from the aspect ratio of the image
+        * if ``2-tuple``, defines the width and height of the
+          image. Padding with white pixels is used to maintain the aspect
+          ratio of the image.
+        * if ``None``, the size of the data is used.
 
         For output sizes larger than the data size, "nearest" interpolation is
         used by default and this behaviour can be changed through the
-        *imshow_kwds* dictionary.
+        ``imshow_kwds`` dictionary.
 
     imshow_kwds : dict, optional
         Keyword arguments dictionary for :py:func:`~.matplotlib.pyplot.imshow`.
     **kwds : dict, optional
         Allows to pass keyword arguments supported by the individual file
         writers as documented at
         https://imageio.readthedocs.io/en/stable/formats/index.html when
@@ -130,25 +133,25 @@
             axes = sig_axes
         elif len(nav_axes) == 2:
             # Use navigation axes
             axes = nav_axes
         else:
             raise RuntimeError("This dimensionality is not supported.")
 
-        aspect_ratio = imshow_kwds.get("aspect", None)
-        if not isinstance(aspect_ratio, (int, float)):
-            aspect_ratio = data.shape[0] / data.shape[1]
-
+        aspect_ratio = imshow_kwds.get("aspect", 1)
         if output_size is None:
-            # fall back to image size taking into account aspect_ratio
+            # fall back to image size taking into account aspect
             ratio = (1, aspect_ratio)
-            output_size = [axis["size"] * r for axis, r in zip(axes, ratio)]
+            output_size = [axis["size"] * r for axis, r in zip(axes[::-1], ratio)]
         elif isinstance(output_size, (int, float)):
+            aspect_ratio *= data.shape[0] / data.shape[1]
             output_size = [output_size, output_size * aspect_ratio]
-
+        elif isinstance(output_size, Iterable) and len(output_size) != 2:
+            # Catch error here, because matplotlib error is not obvious
+            raise ValueError("If `output_size` is an iterable, it must be of length 2.")
         fig = Figure(figsize=[size / dpi for size in output_size], dpi=dpi)
 
         # List of format supported by matplotlib
         supported_format = sorted(fig.canvas.get_supported_filetypes())
         if os.path.splitext(filename)[1].replace(".", "") not in supported_format:
             if scalebar:
                 raise ValueError(
@@ -226,21 +229,30 @@
         from dask.array import from_delayed
         from dask import delayed
 
         val = delayed(_read_data, pure=True)(filename, **kwds)
         dc = from_delayed(val, shape=dc.shape, dtype=dc.dtype)
     else:
         dc = _read_data(filename, **kwds)
+
+    om = {}
+
+    im = Image.open(filename)
+    om["exif_tags"] = _parse_exif_tags(im)
+    axes = _parse_axes_from_metadata(om["exif_tags"], dc.shape)
+
     return [
         {
             "data": dc,
+            "axes": axes,
             "metadata": {
                 "General": {"original_filename": os.path.split(filename)[1]},
                 "Signal": {"signal_type": ""},
             },
+            "original_metadata": om,
         }
     ]
 
 
 file_reader.__doc__ %= (FILENAME_DOC, LAZY_DOC, RETURNS_DOC)
```

### Comparing `rosettasciio-0.3/rsciio/impulse/_api.py` & `rosettasciio-0.4/rsciio/impulse/_api.py`

 * *Files identical despite different names*

### Comparing `rosettasciio-0.3/rsciio/jeol/_api.py` & `rosettasciio-0.4/rsciio/jeol/_api.py`

 * *Files identical despite different names*

### Comparing `rosettasciio-0.3/rsciio/jobinyvon/_api.py` & `rosettasciio-0.4/rsciio/jobinyvon/_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -219,65 +219,65 @@
             "Laser (nm)",
             "Spectro (nm)",
         ]
 
         ## use second extracted value
         for key in change_to_second_value:
             try:
-                self.original_metadata["experimental_setup"][
-                    key
-                ] = self.original_metadata["experimental_setup"][key]["2"]
+                self.original_metadata["experimental_setup"][key] = (
+                    self.original_metadata["experimental_setup"][key]["2"]
+                )
             except KeyError:
                 pass
 
         ## use first extracted value
         for key, value in self.original_metadata["experimental_setup"].items():
             if isinstance(value, dict):
                 # only if there is an entry/value
                 if bool(value):
-                    self.original_metadata["experimental_setup"][
-                        key
-                    ] = self.original_metadata["experimental_setup"][key]["1"]
+                    self.original_metadata["experimental_setup"][key] = (
+                        self.original_metadata["experimental_setup"][key]["1"]
+                    )
 
         for key, value in self.original_metadata["date"].items():
             if isinstance(value, dict):
                 if bool(value):
                     self.original_metadata["date"][key] = self.original_metadata[
                         "date"
                     ][key]["1"]
 
         for key, value in self.original_metadata["file_information"].items():
             if isinstance(value, dict):
                 if bool(value):
-                    self.original_metadata["file_information"][
-                        key
-                    ] = self.original_metadata["file_information"][key]["1"]
+                    self.original_metadata["file_information"][key] = (
+                        self.original_metadata["file_information"][key]["1"]
+                    )
 
         ## convert strings to float
         for key in convert_to_numeric:
             try:
                 self.original_metadata["experimental_setup"][key] = float(
                     self.original_metadata["experimental_setup"][key]
                 )
             except KeyError:
                 pass
 
         ## move the unit from grating to the key name
         try:
-            self.original_metadata["experimental_setup"][
-                "Grating (gr/mm)"
-            ] = self.original_metadata["experimental_setup"].pop("Grating")
+            self.original_metadata["experimental_setup"]["Grating (gr/mm)"] = (
+                self.original_metadata["experimental_setup"].pop("Grating")
+            )
         except KeyError:  # pragma: no cover
             pass  # pragma: no cover
 
         ## add percentage for filter key name
         try:
-            self.original_metadata["experimental_setup"][
-                "ND Filter (%)"
-            ] = self.original_metadata["experimental_setup"].pop("ND Filter")
+            self.original_metadata["experimental_setup"]["ND Filter (%)"] = (
+                self.original_metadata["experimental_setup"].pop("ND Filter")
+            )
         except KeyError:  # pragma: no cover
             pass  # pragma: no cover
 
     def get_original_metadata(self):
         """Extracts metadata from file."""
         self.original_metadata = {}
         for child in self._metadata_root:
```

### Comparing `rosettasciio-0.3/rsciio/mrc/_api.py` & `rosettasciio-0.4/rsciio/mrc/_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -130,15 +130,15 @@
         1: np.int16,
         2: np.float32,
         4: np.complex64,
         6: np.uint16,
         12: np.float16,
     }
 
-    mode = int(mode)
+    mode = int(mode[0])
     if mode in mode_to_dtype:
         return np.dtype(mode_to_dtype[mode])
     else:
         raise ValueError(f"Unrecognised mode '{mode}'.")
 
 
 def read_de_metadata_file(filename, navigation_shape=None):
@@ -340,28 +340,34 @@
         )
         del fei_dict["empty"]
         original_metadata["fei_header"] = fei_dict
 
     if fei_header is None:
         # The scale is in Angstroms, we convert it to nm
         scales = [
-            float(std_header["Zlen"] / std_header["MZ"]) / 10
-            if float(std_header["Zlen"]) != 0 and float(std_header["MZ"]) != 0
-            else 1,
-            float(std_header["Ylen"] / std_header["MY"]) / 10
-            if float(std_header["MY"]) != 0
-            else 1,
-            float(std_header["Xlen"] / std_header["MX"]) / 10
-            if float(std_header["MX"]) != 0
-            else 1,
+            (
+                float((std_header["Zlen"] / std_header["MZ"])[0]) / 10
+                if float(std_header["Zlen"][0]) != 0 and float(std_header["MZ"][0]) != 0
+                else 1
+            ),
+            (
+                float((std_header["Ylen"] / std_header["MY"])[0]) / 10
+                if float(std_header["MY"][0]) != 0
+                else 1
+            ),
+            (
+                float((std_header["Xlen"] / std_header["MX"])[0]) / 10
+                if float(std_header["MX"][0]) != 0
+                else 1
+            ),
         ]
         offsets = [
-            float(std_header["ZORIGIN"]) / 10,
-            float(std_header["YORIGIN"]) / 10,
-            float(std_header["XORIGIN"]) / 10,
+            float(std_header["ZORIGIN"][0]) / 10,
+            float(std_header["YORIGIN"][0]) / 10,
+            float(std_header["XORIGIN"][0]) / 10,
         ]
 
     else:
         # FEI does not use the standard header to store the scale
         # It does store the spatial scale in pixel_size, one per angle in
         # meters
         scales = [
```

### Comparing `rosettasciio-0.3/rsciio/mrcz/_api.py` & `rosettasciio-0.4/rsciio/mrcz/_api.py`

 * *Files identical despite different names*

### Comparing `rosettasciio-0.3/rsciio/msa/_api.py` & `rosettasciio-0.4/rsciio/msa/_api.py`

 * *Files identical despite different names*

### Comparing `rosettasciio-0.3/rsciio/netcdf/_api.py` & `rosettasciio-0.4/rsciio/netcdf/_api.py`

 * *Files identical despite different names*

### Comparing `rosettasciio-0.3/rsciio/nexus/_api.py` & `rosettasciio-0.4/rsciio/nexus/_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """NeXus file reading and writing."""
+
 # -*- coding: utf-8 -*-
 # Copyright 2007-2023 The HyperSpy developers
 #
 # This file is part of RosettaSciIO.
 #
 # RosettaSciIO is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
@@ -127,15 +128,15 @@
         totest = np.array(value)
     if isinstance(totest, np.ndarray) and totest.dtype.char == "U":
         toreturn = np.array(totest).astype("S")
     elif isinstance(totest, (np.ndarray, da.Array)):
         toreturn = totest
     if isinstance(totest, str):
         toreturn = totest.encode("utf-8")
-        toreturn = np.string_(toreturn)
+        toreturn = np.bytes_(toreturn)
     return toreturn
 
 
 def _text_split(s, sep):
     """Split a string based of list of seperators.
 
     Parameters
@@ -222,15 +223,19 @@
             axes_list[0] = _parse_from_file(axes_key)
 
         named_axes = list(range(len(axes_list)))
         for i, ax in enumerate(axes_list):
             if ax != ".":
                 index_name = ax + "_indices"
                 if index_name in dataentry.attrs:
-                    ind_in_array = int(dataentry.attrs[index_name])
+                    ind_in_array = dataentry.attrs[index_name]
+                    if len(ind_in_array.shape) > 0:
+                        ind_in_array = int(ind_in_array[0])
+                    else:
+                        ind_in_array = int(ind_in_array)
                 else:
                     ind_in_array = i
                 axis_index_list.append(ind_in_array)
                 if "units" in dataentry[ax].attrs:
                     units = _parse_from_file(dataentry[ax].attrs["units"])
                 else:
                     units = ""
@@ -584,18 +589,19 @@
                             dictionary["attributes"]["learning_results"] = learning
                         if "original_metadata" in oma:
                             if metadata_key is None:
                                 dictionary["original_metadata"] = oma[
                                     "original_metadata"
                                 ]
                             else:
-                                dictionary[
-                                    "original_metadata"
-                                ] = _find_search_keys_in_dict(
-                                    (oma["original_metadata"]), search_keys=metadata_key
+                                dictionary["original_metadata"] = (
+                                    _find_search_keys_in_dict(
+                                        (oma["original_metadata"]),
+                                        search_keys=metadata_key,
+                                    )
                                 )
                             # reconstruct the axes_list for axes_manager
                             for k, v in oma["original_metadata"].items():
                                 if k.startswith("_sig_"):
                                     hyper_ax = [
                                         ax_v
                                         for ax_k, ax_v in v.items()
```

### Comparing `rosettasciio-0.3/rsciio/pantarhei/_api.py` & `rosettasciio-0.4/rsciio/pantarhei/_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -177,17 +177,19 @@
         else:
             return len(order)
 
     new_order = sorted(range(len(content_type_np_order)), key=_navigation_first)
     default_labels = reversed(["X", "Y", "Z"][: content_type_np_order.count(None)])
 
     data_labels = [
-        content_type_np_order[i]
-        if content_type_np_order[i] is not None
-        else next(default_labels)
+        (
+            content_type_np_order[i]
+            if content_type_np_order[i] is not None
+            else next(default_labels)
+        )
         for i in new_order
     ]
     calibration_ordered = [calibrations_np_order[i] for i in new_order]
     data = np.moveaxis(data, new_order, list(range(len(content_type_np_order))))
 
     # TODO: Will have to be updated once CEOS adds selectable dispersion orientation
     if meta_data.get("filter.mode") == "EELS":
```

### Comparing `rosettasciio-0.3/rsciio/phenom/_api.py` & `rosettasciio-0.4/rsciio/phenom/_api.py`

 * *Files identical despite different names*

### Comparing `rosettasciio-0.3/rsciio/protochips/_api.py` & `rosettasciio-0.4/rsciio/protochips/_api.py`

 * *Files identical despite different names*

### Comparing `rosettasciio-0.3/rsciio/quantumdetector/_api.py` & `rosettasciio-0.4/rsciio/quantumdetector/_api.py`

 * *Files 9% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 # along with RosettaSciIO. If not, see <https://www.gnu.org/licenses/#GPL>.
 #
 # Adapted from https://github.com/matkraj/read_mib under GPL-3.0 license
 
 import logging
 import os
 from pathlib import Path
+import warnings
 
 import dask.array as da
 import numpy as np
 
 from rsciio._docstrings import (
     CHUNKS_READ_DOC,
     FILENAME_DOC,
@@ -126,22 +127,22 @@
             try:
                 with open(path, "rb") as f:
                     head = f.read(384).decode().split(",")
                     f.seek(0, os.SEEK_END)
                     self.file_size = f.tell()
                     self.buffer = False
                     self.path = path
-            except:  # pragma: no cover
+            except BaseException:  # pragma: no cover
                 raise RuntimeError("File does not contain MIB header.")
         elif isinstance(path, bytes):
             try:
                 head = path[:384].decode().split(",")
                 self.file_size = len(path)
                 self.buffer = True
-            except:  # pragma: no cover
+            except BaseException:  # pragma: no cover
                 raise RuntimeError("Buffer does not contain MIB header.")
         else:  # pragma: no cover
             raise TypeError("`path` must be a str or a buffer.")
 
         # read detector size
         self.merlin_size = (int(head[4]), int(head[5]))
 
@@ -214,15 +215,15 @@
         The ``MIBProperties`` instance of the file. If None, it will be
         parsed from the file.
     return_headers : bool, default=False
         If True, also return headers.
     print_info : bool, default=False
         If True, display information when loading the file.
     return_mmap : bool
-        If True, return the py:func:`numpy.memmap` object. Default is True.
+        If True, return the :class:`numpy.memmap` object. Default is True.
 
     Returns
     -------
     numpy.ndarray or dask.array.Array or numpy.memmap
         The data from the mib reshaped according to the ``navigation_shape``
         argument.
 
@@ -238,15 +239,15 @@
         raise ValueError("Loading memory buffer lazily is not supported.")
 
     # As we save the dtype name, we don't have the endianess and we
     # need to specify it here
     data_dtype = np.dtype(mib_prop.dtype).newbyteorder(">")
     merlin_frame_dtype = np.dtype(
         [
-            ("header", np.string_, mib_prop.head_size),
+            ("header", np.bytes_, mib_prop.head_size),
             ("data", data_dtype, mib_prop.merlin_size),
         ]
     )
     # find the number of frames in the file
     frame_number_in_file = mib_prop.file_size // merlin_frame_dtype.itemsize
 
     # Get the frame slice to load, taking into `None` and negative indexing
@@ -263,17 +264,17 @@
         if frame_number > frame_number_in_file:
             # Case of interrupted acquisition
             # Set the corrected number of lines
             # To keep the implementation simple only load completed line
             # Reshape only when the slice from zeros
             if first_frame == 0 and len(navigation_shape) > 1:
                 navigation_shape = (
-                    navigation_shape[1],
-                    frame_number_in_file // navigation_shape[1],
-                )
+                    navigation_shape[0],
+                    frame_number_in_file // navigation_shape[0],
+                )[::-1]
             else:
                 navigation_shape = (number_of_frames_to_load,)
         elif number_of_frames_to_load < frame_number:
             # in case the given navigation is not None and the total number of frame
             # to load is too small, we can't reshape and we fall back to stack of images
             _logger.warning(
                 "The `navigation_shape` doesn't match the number of frames to load. "
@@ -322,21 +323,30 @@
     else:  # pragma: no cover
         raise TypeError("`path` must be a str or a buffer.")
 
     headers = data["header"]
     data = data["data"]
     if not return_mmap:
         if lazy:
-            data = da.from_array(data, chunks=chunks)
+            if isinstance(chunks, tuple) and len(chunks) > 2:
+                # Since the data is reshaped later on, we set only the
+                # signal dimension chunks here
+                _chunks = ("auto",) + chunks[-2:]
+            else:
+                _chunks = chunks
+            data = da.from_array(data, chunks=_chunks)
         else:
             data = np.array(data)
 
     # remove navigation_dimension with value 1 before reshaping
     navigation_shape = tuple(i for i in navigation_shape if i > 1)
     data = data.reshape(navigation_shape + mib_prop.merlin_size)
+    if lazy and isinstance(chunks, tuple) and len(chunks) > 2:
+        # rechunk navigation space when chunking is specified as a tuple
+        data = data.rechunk(chunks)
 
     if return_headers:
         return data, headers
     else:
         return data
 
 
@@ -397,15 +407,15 @@
 
     Examples
     --------
     Use ``load_mib_data`` function to the headers and parse the exposures
     from the headers. By default, reads only the first 10 000 frames.
 
     >>> from rsciio.quantumdetector import load_mib_data, parse_exposures
-    >>> data, headers = load_mib_data(path, return_header=True, return_mmap=True)
+    >>> data, headers = load_mib_data(path, return_headers=True, return_mmap=True)
     >>> exposures = parse_exposures(headers)
 
     All frames can be parsed by using ``max_index=-1``:
 
     >>> data, headers = load_mib_data(path, return_headers=True)
     >>> timestamps = parse_exposures(headers, max_index=-1)
     >>> len(timestamps)
@@ -481,14 +491,17 @@
     first_frame=None,
     last_frame=None,
     print_info=False,
 ):
     """
     Read a Quantum Detectors ``mib`` file.
 
+    If a ``hdr`` file with the same file name was saved along the ``mib`` file,
+    it will be used to read the metadata.
+
     Parameters
     ----------
     %s
     %s
     %s
     %s
     %s
@@ -499,35 +512,79 @@
     %s
 
     Notes
     -----
     In case of interrupted acquisition, only the completed lines are read and
     the incomplete line are discarded.
 
+    When the scanning shape (i. e. navigation shape) is not available from the
+    metadata (for example with acquisition using pixel trigger), the timestamps
+    will be used to guess the navigation shape.
+
+    Examples
+    --------
+    In case, the navigation shape can't read from the data itself (for example,
+    type of acquisition unsupported), the ``navigation_shape`` can be specified:
+
+    .. code-block:: python
+
+        >>> from rsciio.quantumdetector import file_reader
+        >>> s_dict = file_reader("file.mib", navigation_shape=(256, 256))
+
     """
     mib_prop = MIBProperties()
     mib_prop.parse_file(filename)
     hdr_filename = str(filename).replace(".mib", ".hdr")
 
     original_metadata = {"mib_properties": vars(mib_prop)}
 
     if Path(hdr_filename).exists():
         hdr = parse_hdr_file(hdr_filename)
         original_metadata["hdr_file"] = hdr
     else:
         hdr = None
         _logger.warning("`hdr` file couldn't be found.")
 
-    if navigation_shape is None and hdr is not None:
-        # Use the hdr file to find the number of frames
-        navigation_shape = (
-            int(hdr["Frames per Trigger (Number)"]),
-            int(hdr["Frames in Acquisition (Number)"])
-            // int(hdr["Frames per Trigger (Number)"]),
-        )
+    frame_per_trigger = 1
+    headers = None
+    if navigation_shape is None:
+        if hdr is not None:
+            # Use the hdr file to find the number of frames
+            frame_per_trigger = int(hdr["Frames per Trigger (Number)"])
+            frames_number = int(hdr["Frames in Acquisition (Number)"])
+        else:
+            _, headers = load_mib_data(filename, return_headers=True)
+            frames_number = len(headers)
+
+        if frame_per_trigger == 1:
+            if headers is None:
+                _, headers = load_mib_data(filename, return_headers=True)
+            # Use parse_timestamps to find the number of frame per line
+            # we will get a difference of timestamps at the beginning of each line
+            with warnings.catch_warnings():
+                # Filter warning for converting timezone aware datetime
+                # The time zone is dropped
+                # Changed from `DeprecationWarning` to `UserWarning` in numpy 2.0
+                warnings.simplefilter("ignore")
+                times = np.array(parse_timestamps(headers)).astype(dtype="datetime64")
+
+            times_diff = np.diff(times).astype(float)
+            if len(times_diff) > 0:
+                # Substract the mean and take the first position above 0
+                indices = np.argwhere(times_diff - np.mean(times_diff) > 0)
+                if len(indices) > 0 and len(indices[0]) > 0:
+                    frame_per_trigger = indices[0][0] + 1
+
+        if frames_number == 0:
+            # Some hdf files have the "Frames per Trigger (Number)": 0
+            # in this case, we don't reshape
+            # Possibly for "continuous and indefinite" acquisition
+            navigation_shape = None
+        else:
+            navigation_shape = (frame_per_trigger, frames_number // frame_per_trigger)
 
     data = load_mib_data(
         filename,
         lazy=lazy,
         chunks=chunks,
         mmap_mode=mmap_mode,
         navigation_shape=navigation_shape,
```

### Comparing `rosettasciio-0.3/rsciio/renishaw/_api.py` & `rosettasciio-0.4/rsciio/renishaw/_api.py`

 * *Files 3% similar despite different names*

```diff
@@ -62,29 +62,31 @@
 import datetime
 import importlib.util
 import logging
 from copy import deepcopy
 from enum import IntEnum, Enum, EnumMeta
 from io import BytesIO
 from pathlib import Path
+import os
 
 import numpy as np
 from numpy.polynomial.polynomial import polyfit
 
 from rsciio._docstrings import FILENAME_DOC, LAZY_DOC, RETURNS_DOC
+from rsciio.utils import rgb_tools
+
 
 _logger = logging.getLogger(__name__)
 
-## PIL alternative: imageio.v3.immeta extracts exif as binary
-## but then this binary string needs to be parsed
+
 try:
     from PIL import Image
 except ImportError:
     PIL_installed = False
-    _logger.warning("Pillow not installed. Cannot load whitelight image into metadata")
+    _logger.warning("Pillow not installed. Cannot load whitelight image.")
 else:
     PIL_installed = True
 
 
 def _find_key(data, target):
     """Finds key in nested dictionary. Returns generator object."""
     for key, value in data.items():
@@ -319,29 +321,14 @@
     Mp_WellReference = 25
     EndMarker = 26
     ExposureTime = (
         27  # different from gwyddion, see PR#39 streamhr rapide mode (py-wdf-reader)
     )
 
 
-# for wthl image
-class ExifTags(IntEnum, metaclass=DefaultEnumMeta):
-    # Standard EXIF TAGS
-    ImageDescription = 0x10E  # 270
-    Make = 0x10F  # 271
-    ExifOffset = 0x8769  # 34665
-    FocalPlaneXResolution = 0xA20E  # 41486
-    FocalPlaneYResolution = 0xA20F  # 41487
-    FocalPlaneResolutionUnit = 0xA210  # 41488
-    # Customized EXIF TAGS from Renishaw
-    FocalPlaneXYOrigins = 0xFEA0  # 65184
-    FieldOfViewXY = 0xFEA1  # 65185
-    Unknown = 0xFEA2  # 65186
-
-
 class WDFReader(object):
     """Reader for Renishaw(TM) WiRE Raman spectroscopy files (.wdf format)
 
     The wdf file format is separated into several DataBlocks, with starting 4-char
     strings:
 
     fully parsed blocks:
@@ -465,15 +452,14 @@
         self._parse_metadata("WARP_0")
         self._parse_metadata("WARP_1")
         self._parse_metadata("WXDM_0")
         self._map_WXDM()
         self._parse_MAP("MAP_0")
         self._parse_MAP("MAP_1")
         self._parse_TEXT()
-        self._parse_WHTL()
 
         ## parse blocks with axes information
         signal_dict = self._parse_XLST()
         nav_orgn = self._parse_ORGN(header_data["num_ORGN"])
         nav_wmap = self._parse_WMAP()
 
         ## set axes
@@ -1021,15 +1007,15 @@
             result[ax_name] = axis_tmp
 
         # TODO: differentiate between more map_modes/flags
         flag = wmap_dict["flag"]
         if flag == MapType.xyline.name:
             result = self._set_wmap_nav_linexy(result["X"], result["Y"])
         elif flag == DefaultEnum.Unknown.name:
-            _logger.warning(f"Unknown flag ({wmap_dict['flag']}) for WMAP mapping.")
+            _logger.info(f"Unknown flag ({wmap_dict['flag']}) for WMAP mapping.")
         return result
 
     def _set_wmap_nav_linexy(self, x_axis, y_axis):
         # TODO: save original axis scales and offset in metadata?
         # currently only in original_metadata.WMAP_0
         result = deepcopy(x_axis)
         scale_abs = np.sqrt(x_axis["scale"] ** 2 + y_axis["scale"] ** 2)
@@ -1058,21 +1044,40 @@
         nav_dict = deepcopy(orgn_data)
         if len(nav_dict) != 1:
             _logger.warning(
                 f"Series, but number of navigation axes ({len(nav_dict)}) exist is not 1."
             )
         for axis in orgn_data.keys():
             del nav_dict[axis]["annotation"]
+            data = nav_dict[axis].pop("data")
             nav_dict[axis]["navigate"] = True
-            data = np.unique(nav_dict[axis].pop("data"))
             nav_dict[axis]["size"] = data.size
-            nav_dict[axis]["offset"] = data[0]
-            ## time axis in test data is not perfectly uniform, but X,Y,Z are
-            nav_dict[axis]["scale"] = np.mean(np.diff(data))
             nav_dict[axis]["name"] = axis
+            scale_mean = np.mean(np.diff(data))
+            if axis == "FocusTrack_Z" or scale_mean == 0:
+                # FocusTrack_Z is not uniform and not necessarily ordered
+                # Fix me when hyperspy supports non-ordered non-uniform axis
+                # For now, remove units and fall back on default axis
+                # nav_dict[axis]["axis"] = data
+                if scale_mean == 0:
+                    # case "scale_mean == 0" is for series where the axis is invariant.
+                    # In principle, this should happen but the WiRE software allows it
+                    reason = f"Axis {axis} is invariant"
+                else:
+                    reason = "Non-ordered axis is not supported"
+                _logger.warning(
+                    f"{reason}, a default axis with scale 1 "
+                    "and offset 0 will be used."
+                )
+                del nav_dict[axis]["units"]
+            else:
+                # time axis in test data is not perfectly uniform, but X,Y,Z are
+                nav_dict[axis]["offset"] = data[0]
+                nav_dict[axis]["scale"] = scale_mean
+
         return nav_dict
 
     def _compare_measurement_type_to_ORGN_WMAP(self, orgn_data, wmap_data):
         no_wmap = len(wmap_data) == 0
         no_orgn = len(orgn_data) == 0
 
         if self._measurement_type not in MeasurementType._member_names_:
@@ -1140,29 +1145,29 @@
         self.data = np.reshape(self.data, axes_sizes)
         if self._reverse_signal:
             self.data = np.flip(self.data, len(axes_sizes) - 1)
 
     def _map_general_md(self):
         general = {}
         general["title"] = self.original_metadata.get("WDF1_1", {}).get("title")
-        general["original_filename"] = self._filename
+        general["original_filename"] = os.path.split(self._filename)[1]
         try:
             date, time = self.original_metadata["WDF1_1"]["time_start"].split("#")
         except KeyError:
             pass
         else:
             general["date"] = date
             general["time"] = time
         return general
 
     def _map_signal_md(self):
         signal = {}
         if importlib.util.find_spec("lumispy") is None:
             _logger.warning(
-                "Cannot find package lumispy, using BaseSignal as signal_type."
+                "Cannot find package lumispy, using generic signal class BaseSignal."
             )
             signal["signal_type"] = ""
         else:
             signal["signal_type"] = "Luminescence"  # pragma: no cover
 
         try:
             quantity_unit = self.original_metadata.get("WDF1_1", {}).get(
@@ -1221,14 +1226,16 @@
     def map_metadata(self):
         general = self._map_general_md()
         signal = self._map_signal_md()
         detector = self._map_detector_md()
         laser = self._map_laser_md()
         spectrometer = self._map_spectrometer_md()
 
+        # TODO: find laser power?
+
         metadata = {
             "General": general,
             "Signal": signal,
             "Acquisition_instrument": {
                 "Laser": laser,
                 "Detector": detector,
                 "Spectrometer": spectrometer,
@@ -1241,61 +1248,80 @@
         if not self._check_block_exists("TEXT_0"):
             return
         pos, block_size = self._block_info["TEXT_0"]
         self._file_obj.seek(pos)
         text = self.__read_utf8(block_size - 16)
         self.original_metadata.update({"TEXT_0": text})
 
-    def _parse_WHTL(self):
+    def _get_WHTL(self):
         if not self._check_block_exists("WHTL_0"):
-            return
+            return None
         pos, size = self._block_info["WHTL_0"]
         jpeg_header = 0x10
         self._file_obj.seek(pos)
         img_bytes = self._file_obj.read(size - jpeg_header)
         img = BytesIO(img_bytes)
-        whtl_metadata = {"image": img}
 
-        ## extract EXIF tags and store them in metadata
+        ## extract and parse EXIF tags
         if PIL_installed:
+            from rsciio.utils.image import _parse_axes_from_metadata, _parse_exif_tags
+
             pil_img = Image.open(img)
-            ## missing header keys when Pillow >= 8.2.0 -> does not flatten IFD anymore
-            ## see https://pillow.readthedocs.io/en/stable/releasenotes/8.2.0.html#image-getexif-exif-and-gps-ifd
-            ## Use fall-back _getexif method instead
-            exif_header = dict(pil_img._getexif())
-            whtl_metadata["FocalPlaneResolutionUnit"] = str(
-                UnitType(exif_header.get(ExifTags.FocalPlaneResolutionUnit))
-            )
-            whtl_metadata["FocalPlaneXResolution"] = exif_header.get(
-                ExifTags.FocalPlaneXResolution
-            )
-            whtl_metadata["FocalPlaneYResolution"] = exif_header.get(
-                ExifTags.FocalPlaneYResolution
-            )
-            whtl_metadata["FocalPlaneXYOrigins"] = exif_header.get(
-                ExifTags.FocalPlaneXYOrigins
-            )
-            whtl_metadata["ImageDescription"] = exif_header.get(
-                ExifTags.ImageDescription
-            )
-            whtl_metadata["Make"] = exif_header.get(ExifTags.Make)
-            whtl_metadata["Unknown"] = exif_header.get(ExifTags.Unknown)
-            whtl_metadata["FieldOfViewXY"] = exif_header.get(ExifTags.FieldOfViewXY)
+            original_metadata = {}
+            data = rgb_tools.regular_array2rgbx(np.array(pil_img))
+            original_metadata["exif_tags"] = _parse_exif_tags(pil_img)
+            axes = _parse_axes_from_metadata(original_metadata["exif_tags"], data.shape)
+            metadata = {
+                "General": {"original_filename": os.path.split(self._filename)[1]},
+                "Signal": {"signal_type": ""},
+            }
+
+            map_md = self.original_metadata.get("WMAP_0")
+            if map_md is not None:
+                width = map_md["scale_xyz"][0] * map_md["size_xyz"][0]
+                length = map_md["scale_xyz"][1] * map_md["size_xyz"][1]
+                offset = (
+                    np.array(map_md["offset_xyz"][:2]) + np.array([width, length]) / 2
+                )
+
+                marker_dict = {
+                    "class": "Rectangles",
+                    "name": "Map",
+                    "plot_on_signal": True,
+                    "kwargs": {
+                        "offsets": offset,
+                        "widths": width,
+                        "heights": length,
+                        "color": ("red",),
+                        "facecolor": "none",
+                    },
+                }
+
+                metadata["Markers"] = {"Map": marker_dict}
 
-        self.original_metadata.update({"WHTL_0": whtl_metadata})
+            return {
+                "axes": axes,
+                "data": data,
+                "metadata": metadata,
+                "original_metadata": original_metadata,
+            }
+        else:  # pragma: no cover
+            # Explicit return for readibility
+            return None
 
 
 def file_reader(
     filename,
     lazy=False,
-    use_uniform_signal_axis=True,
+    use_uniform_signal_axis=False,
     load_unmatched_metadata=False,
 ):
     """
-    Read Renishaw's ``.wdf`` file.
+    Read Renishaw's ``.wdf`` file. In case of mapping data, the image area will
+    be returned with a marker showing the mapped area.
 
     Parameters
     ----------
     %s
     %s
     use_uniform_signal_axis : bool, default=False
         Can be specified to choose between non-uniform or uniform signal axes.
@@ -1328,13 +1354,17 @@
         wdf.read_file(filesize)
 
         dictionary["data"] = wdf.data
         dictionary["axes"] = wdf.axes
         dictionary["metadata"] = deepcopy(wdf.metadata)
         dictionary["original_metadata"] = deepcopy(wdf.original_metadata)
 
-    return [
-        dictionary,
-    ]
+        image_dict = wdf._get_WHTL()
+
+    dict_list = [dictionary]
+    if image_dict is not None:
+        dict_list.append(image_dict)
+
+    return dict_list
 
 
 file_reader.__doc__ %= (FILENAME_DOC, LAZY_DOC, RETURNS_DOC)
```

### Comparing `rosettasciio-0.3/rsciio/ripple/_api.py` & `rosettasciio-0.4/rsciio/ripple/_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -580,17 +580,17 @@
         if "Stage.tilt_alpha" in mp:
             keys_dictionary["tilt-stage"] = mp.Stage.tilt_alpha
         if "Detector.EDS.azimuth_angle" in mp:
             keys_dictionary["azimuth-angle"] = mp.Detector.EDS.azimuth_angle
         if "Detector.EDS.live_time" in mp:
             keys_dictionary["live-time"] = mp.Detector.EDS.live_time
         if "Detector.EDS.energy_resolution_MnKa" in mp:
-            keys_dictionary[
-                "detector-peak-width-ev"
-            ] = mp.Detector.EDS.energy_resolution_MnKa
+            keys_dictionary["detector-peak-width-ev"] = (
+                mp.Detector.EDS.energy_resolution_MnKa
+            )
 
     write_rpl(filename, keys_dictionary, encoding)
     write_raw(filename, signal, record_by, sig_axes, nav_axes)
 
 
 file_writer.__doc__ %= (
     FILENAME_DOC.replace("read", "write to"),
```

### Comparing `rosettasciio-0.3/rsciio/semper/_api.py` & `rosettasciio-0.4/rsciio/semper/_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -90,15 +90,14 @@
 from rsciio.utils.tools import sarray2dict, DTBox
 
 
 _logger = logging.getLogger(__name__)
 
 
 class SemperFormat(object):
-
     """Class for importing and exporting SEMPER `.unf`-files.
 
     The :class:`~.SemperFormat` class represents a SEMPER binary file format
     with a header, which holds additional information. `.unf`-files can be
     saved and read from files.
 
     Attributes
@@ -216,17 +215,15 @@
         )  # Unpacking function for 4 byte floats!
         rec_length = np.fromfile(unf_file, dtype="<i", count=1)[0]  # length of label
         label = sarray2dict(np.fromfile(unf_file, dtype=cls.LABEL_DTYPES, count=1))
         label["SEMPER"] = "".join([str(chr(l)) for l in label["SEMPER"]])
         assert label["SEMPER"] == "Semper"
         # Process dimensions:
         for key in ["NCOL", "NROW", "NLAY", "ICCOLN", "ICROWN", "ICLAYN"]:
-            value = (
-                256**2 * label.pop(key + "H") + 256 * label[key][0] + label[key][1]
-            )
+            value = 256**2 * label.pop(key + "H") + 256 * label[key][0] + label[key][1]
             label[key] = value
         # Process date:
         date = "{}-{}-{} {}:{}:{}".format(label["DATE"][0] + 1900, *label["DATE"][1:])
         label["DATE"] = date
         # Process range:
         if label["NCRANG"] == 255:
             range_min = unpack(label["RANGE"][:4])
```

### Comparing `rosettasciio-0.3/rsciio/tests/__init__.py` & `rosettasciio-0.4/rsciio/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `rosettasciio-0.3/rsciio/tests/conftest.py` & `rosettasciio-0.4/rsciio/tests/conftest.py`

 * *Files 24% similar despite different names*

```diff
@@ -12,34 +12,57 @@
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with RosettaSciIO. If not, see <https://www.gnu.org/licenses/#GPL>.
 
-import os
+import json
 from packaging.version import Version
 
-from rsciio.tests.registry_utils import download_all
+from filelock import FileLock
+import pytest
+
 
 try:
     import hyperspy
 
     if Version(hyperspy.__version__) < Version("2.0.dev"):
         raise Exception(
             "To run the test suite using hyperspy, \
             hyperspy 2.0 or higher is required."
         )
 except ImportError:
     pass
 
 
-def pytest_configure(config):
-    # Run in pytest_configure hook to avoid capturing stdout by pytest and
-    # inform user that the test data are being downloaded
-
-    # Workaround to avoid running it for each worker
-    worker_id = os.environ.get("PYTEST_XDIST_WORKER")
-    if worker_id is None:
-        print("Checking if test data need downloading...")
-        download_all()
-        print("All test data available.")
+# From https://pytest-xdist.readthedocs.io/en/latest/how-to.html#making-session-scoped-fixtures-execute-only-once
+@pytest.fixture(scope="session", autouse=True)
+def session_data(request, tmp_path_factory, worker_id):
+    capmanager = request.config.pluginmanager.getplugin("capturemanager")
+
+    def _download_test_data():
+        from rsciio.tests.registry_utils import download_all
+
+        with capmanager.global_and_fixture_disabled():
+            print("Checking if test data need downloading...")
+            download_all()
+            print("All test data available.")
+
+        return "Test data available"
+
+    if worker_id == "master":
+        # not executing in with multiple workers, just produce the data and let
+        # pytest's fixture caching do its job
+        return _download_test_data()
+
+    # get the temp directory shared by all workers
+    root_tmp_dir = tmp_path_factory.getbasetemp().parent
+
+    fn = root_tmp_dir / "data.json"
+    with FileLock(str(fn) + ".lock"):
+        if fn.is_file():
+            data = json.loads(fn.read_text())
+        else:
+            data = _download_test_data()
+            fn.write_text(json.dumps(data))
+    return data
```

### Comparing `rosettasciio-0.3/rsciio/tests/generate_dm_testing_files.py` & `rosettasciio-0.4/rsciio/tests/generate_dm_testing_files.py`

 * *Files identical despite different names*

### Comparing `rosettasciio-0.3/rsciio/tests/generate_renishaw_test_file.py` & `rosettasciio-0.4/rsciio/tests/generate_renishaw_test_file.py`

 * *Files identical despite different names*

### Comparing `rosettasciio-0.3/rsciio/tests/registry.py` & `rosettasciio-0.4/rsciio/tests/test_set_log_level.py`

 * *Files 27% similar despite different names*

```diff
@@ -6,46 +6,23 @@
 # RosettaSciIO is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
 # RosettaSciIO is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
-# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with RosettaSciIO. If not, see <https://www.gnu.org/licenses/#GPL>.
 
-from packaging.version import Version
-from pathlib import Path
-
-import pooch
+import pytest
 
 import rsciio
 
 
-version = rsciio.__version__
-
-
-if Version(version).is_devrelease:
-    version = "main"
-else:
-    version = f"v{version}"
-
-
-TESTS_PATH = Path(__file__).parent
-
-
-TEST_DATA_REGISTRY = pooch.create(
-    path=TESTS_PATH / "data",
-    base_url=f"https://github.com/hyperspy/rosettasciio/raw/{version}/rsciio/tests/data/",
-    # We don't use the version functionality of pooch because we want to use the
-    # local test folder (rsciio.tests.data)
-    version=None,
-    # We'll load it from a file later
-    registry=None,
-    allow_updates=False,
-    retry_if_failed=3,
+@pytest.mark.parametrize(
+    "level", ("CRITICAL", "ERROR", "WARNING", "INFO", "DEBUG", "NOTSET")
 )
-
-TEST_DATA_REGISTRY.load_registry(TESTS_PATH / "registry.txt")
+def test_set_log_level(level):
+    rsciio.set_log_level(level)
```

### Comparing `rosettasciio-0.3/rsciio/tests/registry.txt` & `rosettasciio-0.4/rsciio/tests/registry.txt`

 * *Files 1% similar despite different names*

```diff
@@ -153,14 +153,15 @@
 'emd/example_object_dtype_data.emd' 31d9aa4ccd9991d5e58eb5e86c137c24669fb6f1c469e5ac9717f49fe2c9d25f
 'emd/example_signal.emd' 4a020e8f7588ca0dd97e8e8bad549c33d48bbfb4e5cb8a4a00f58b70a3a04804
 'emd/example_spectrum.emd' 14d30ab9f2b124c1208b36c99729a7c6f73e00d6babd84da1b1a4e14273c32f6
 'emd/fei_emd_files.zip' 101512cb1e0d66b63ac62ef4390a8bd654714a41e416c94230229e14e0d9ea62
 'emd/fei_example_complex_fft.emd' eec20bd422428dc498334143e2a721aa793e79f399bfe16c21cb8b0313ff0c07
 'emd/fei_example_dpc_titles.emd' c06422c623e7a7b18ed8864c99d34590488b98fef85423ac33e1ea10bef66b2f
 'emd/fei_example_tem_stack.emd' 397d5076b0133db608abd985985fad275bf6594823393f72a069020e47c21a1e
+'emd/velox_emd_version11.zip' 125f0f6b1517e6bb2a1c44f2157b874fe244bb7716f37a9efbda853f16e395c1
 'empad/map128x128_version1.2.0.xml' b1cd0dfedc348c9e03ac10e32e3b98a0a0502f87e72069423e7d5f78d40ccae5
 'empad/map4x4.xml' ff1a1a6488c7e525c1386f04d791bf77425e27b334c4301a9e6ec85c7628cbeb
 'empad/stack_images.xml' 7047717786c3773735ff751a3ca797325d7944fe7b70f110cdda55d455a38a55
 'hamamatsu/focus_mode.img' 9c6994e078e8daf941a6a46a0061a543405887e9f61f62618b01b0f754ce5c93
 'hamamatsu/operate_mode.img' 4833dd8e13dc908bf4a716708372ca51f2083a64f874cca0443fad4c03b289c3
 'hamamatsu/photon_counting.img' 899043b308fe736797060fea471acb733e7e23e1bc2367c1bed06c327d5a92ce
 'hamamatsu/shading_file.img' d075910ca724cd9c999c4d5391b61bfde20fd0ee5348e3836b1c5b1239324353
@@ -171,14 +172,15 @@
 'hspy/example2_v3.1.hspy' 7e598f0ba4af5c5ce40d1511c650ddcf3ff387f9d0ddd9bf2baf7c3f60597b60
 'hspy/hspy_ext_missing.hspy' a3219df51a69054e6145a4e37fc33e42088f0e2b10c9b6a37c191ee839ba9ac8
 'hspy/none_metadata.hdf5' aa7638b2bb2822a6979b072d947dde3444c7745a18021e582622661915d88ccd
 'hspy/test_marker_bad_marker_type.hdf5' 2ef59a882ebfec25872a511f7387566087485a808f1139ce4af6dc1664219a0e
 'hspy/test_marker_point_y2_data_deleted.hdf5' 11f24a1d91b3157c12e01929d8bfee9757a5cc29281a6220c13f1638cc3ca49c
 'hspy/test_rgba16.hdf5' 5d76658ae9a9416cbdcb239059ee20d640deb634120e1fa051e3199534c47270
 'hspy/with_lists_etc.hdf5' 16ed9d4bcb44ba3510963c102eab888b89516921cd4acc4fdb85271407dae562
+'image/renishaw_wire.jpg' 21d34f130568e161a3b2c8a213aa28991880ca0265aec8bfa3c6ca4d9897540c
 'impulse/NoMetadata_Synchronized data.csv' 3031a84b6df77f3cfe3808fcf993f3cf95b6a9f67179524200b3129a5de47ef5
 'impulse/StubExperiment_Heat raw.csv' 114ebae61321ceed4c071d35e1240a51c2a3bfe37ff9d507cacb7a7dd3977703
 'impulse/StubExperiment_Metadata.log' 4b034d75685d61810025586231fb0adfecbbacd171d89230dbf82d54dff7a93c
 'impulse/StubExperiment_Synchronized data.csv' 21133d08e6269e2850a7e1568919d092487eba372268a874a706099bf46f304a
 'impulse/StubExperiment_Synchronized data.npy' c2d812390b1ea55e4108534055aa840ee92e0f54af683c3e045873cc13b81ea7
 'impulse/changed_file_name.csv' 3031a84b6df77f3cfe3808fcf993f3cf95b6a9f67179524200b3129a5de47ef5
 'impulse/random_csv_file.csv' 8c34945b377ddc58230c61f2f143e25bda463b291288edddf36122c495581810
@@ -262,14 +264,15 @@
 'protochips/random_csv_file.csv' be37c2ef6a4edbb66b69746d8c05cf860a3e3a321237ded84ad810b2b7c7731d
 'quantumdetector/Merlin_Single_Quad.zip' 38cc7f4f580502c591e4b83c25e15b2e50cdc7e678881698dcd9b17ff5096048
 'quantumdetector/Merlin_navigation4x2_ROI.zip' bde0830c13d1885d822c1df81a26ef20169b84124c372cfa7f7709be0efe78af
 'renishaw/renishaw_test_exptime10_acc1.wdf' c056dc49abaad1e7e9744562d5219f52c7a10534ef052eefd8263ad024bcf43b
 'renishaw/renishaw_test_exptime1_acc1.wdf' bc23e1f2644d37dd5b572e587bbcf6db08f33dc7e1480c232b04ef17efa63ba6
 'renishaw/renishaw_test_exptime1_acc2.wdf' 7fb5fb09a079d1af672d3d37c5cbf3d950a6d0783791505c6f42d7d104790711
 'renishaw/renishaw_test_focustrack.wdf' 73fce4347ece1582afb92cb8cd965e021c825815746037eb7cca7af9133e2350
+'renishaw/renishaw_test_focustrack_invariant.wdf' e2a6d79ab342e7217ed8025c3edd266675112359540bb36a026726bc2513a61a
 'renishaw/renishaw_test_linescan.wdf' 631ac664443822e1393b9feef384b5cf80ad53d07c1ce30b9f1136efa8d6d685
 'renishaw/renishaw_test_map.wdf' 92f9051e9330c9bb61c5eca1b230c1d05137d8596da490b72a3684dc3665b9fe
 'renishaw/renishaw_test_map2.wdf' 72484b2337b9e95676d01b1a6a744a7a82db72af1c58c72ce5b55f07546e49c6
 'renishaw/renishaw_test_spectrum.wdf' 9a7a8489b7e5360bcc76df6e74c8a3f88e40ef8fdbee62db7b18490d4ca76d73
 'renishaw/renishaw_test_streamline.wdf' 857acee66c0c4fa7b009cb68f1eb6ac2493769271de0e0ef81902e64a0890f80
 'renishaw/renishaw_test_timeseries.wdf' 296dc02f76fc1a9b3affca02afe7ca01024f38d1aa7e21e62751d7456c86f4cc
 'renishaw/renishaw_test_undefined.wdf' 05ce6a9d5f477ac122b980a16e4dbc2ca4f08d08d310299f67d4830ddce87cee
```

### Comparing `rosettasciio-0.3/rsciio/tests/registry_utils.py` & `rosettasciio-0.4/rsciio/tests/registry_utils.py`

 * *Files identical despite different names*

### Comparing `rosettasciio-0.3/rsciio/tests/test_blockfile.py` & `rosettasciio-0.4/rsciio/tests/test_blockfile.py`

 * *Files identical despite different names*

### Comparing `rosettasciio-0.3/rsciio/tests/test_bruker.py` & `rosettasciio-0.4/rsciio/tests/test_bruker.py`

 * *Files identical despite different names*

### Comparing `rosettasciio-0.3/rsciio/tests/test_de5.py` & `rosettasciio-0.4/rsciio/tests/test_de5.py`

 * *Files identical despite different names*

### Comparing `rosettasciio-0.3/rsciio/tests/test_dens.py` & `rosettasciio-0.4/rsciio/tests/test_dens.py`

 * *Files identical despite different names*

### Comparing `rosettasciio-0.3/rsciio/tests/test_digitalmicrograph.py` & `rosettasciio-0.4/rsciio/tests/test_digitalmicrograph.py`

 * *Files identical despite different names*

### Comparing `rosettasciio-0.3/rsciio/tests/test_digitalsurf.py` & `rosettasciio-0.4/rsciio/tests/test_digitalsurf.py`

 * *Files identical despite different names*

### Comparing `rosettasciio-0.3/rsciio/tests/test_edax.py` & `rosettasciio-0.4/rsciio/tests/test_edax.py`

 * *Files identical despite different names*

### Comparing `rosettasciio-0.3/rsciio/tests/test_emd_ncem.py` & `rosettasciio-0.4/rsciio/tests/test_emd_ncem.py`

 * *Files identical despite different names*

### Comparing `rosettasciio-0.3/rsciio/tests/test_emd_prismatic.py` & `rosettasciio-0.4/rsciio/tests/test_emd_prismatic.py`

 * *Files identical despite different names*

### Comparing `rosettasciio-0.3/rsciio/tests/test_emd_velox.py` & `rosettasciio-0.4/rsciio/tests/test_emd_velox.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,14 +19,15 @@
 
 # The EMD format is a hdf5 standard proposed at Lawrence Berkeley
 # National Lab (see https://emdatasets.com/ for more information).
 # NOT to be confused with the FEI EMD format which was developed later.
 
 import os
 from pathlib import Path
+import logging
 
 import pytest
 
 hs = pytest.importorskip("hyperspy.api", reason="hyperspy not installed")
 
 import dask.array as da
 from datetime import datetime
@@ -495,18 +496,48 @@
     assert isinstance(signals[6], hs.signals.Signal2D)
     assert isinstance(signals[7], hs.signals.Signal2D)
     assert isinstance(signals[8], hs.signals.Signal2D)
 
 
 @pytest.mark.parametrize("fname", ["FFTComplexEven.emd", "FFTComplexOdd.emd"])
 def test_velox_fft_odd_number(fname):
-    print("0", fname)
-    print(TEST_DATA_PATH / fname)
     s = hs.load(TEST_DATA_PATH / fname)
     assert len(s) == 2
 
     shape = (36, 70) if fname == "FFTComplexEven.emd" else (32, 64)
     assert s[0].axes_manager.signal_shape == shape
     assert np.issubdtype(s[0].data.dtype, np.complex64)
 
     assert s[1].axes_manager.signal_shape == (128, 128)
     assert np.issubdtype(s[1].data.dtype, float)
+
+
+class TestVeloxEMDv11:
+    fei_files_path = TEST_DATA_PATH / "velox_emd_version11"
+
+    @classmethod
+    def setup_class(cls):
+        import zipfile
+
+        zipf = TEST_DATA_PATH / "velox_emd_version11.zip"
+        with zipfile.ZipFile(zipf, "r") as zipped:
+            zipped.extractall(cls.fei_files_path)
+
+    @classmethod
+    def teardown_class(cls):
+        gc.collect()
+        shutil.rmtree(cls.fei_files_path)
+
+    @pytest.mark.parametrize("lazy", (True, False))
+    def test_spectrum_images(self, lazy):
+        s = hs.load(self.fei_files_path / "Test SI 16x16 215 kx.emd", lazy=lazy)
+        assert len(s) == 10
+        for i, v in enumerate(["C", "Ca", "O", "Cu", "HAADF", "EDS"]):
+            assert s[i + 4].metadata.General.title == v
+
+        assert s[-1].data.shape == (16, 16, 4096)
+
+    def test_prune_data(self, caplog):
+        with caplog.at_level(logging.WARNING):
+            _ = hs.load(self.fei_files_path / "Test SI 16x16 ReducedData 215 kx.emd")
+
+        assert "No spectrum stream is present" in caplog.text
```

### Comparing `rosettasciio-0.3/rsciio/tests/test_empad.py` & `rosettasciio-0.4/rsciio/tests/test_empad.py`

 * *Files identical despite different names*

### Comparing `rosettasciio-0.3/rsciio/tests/test_fei_stream_readers.py` & `rosettasciio-0.4/rsciio/tests/test_fei_stream_readers.py`

 * *Files identical despite different names*

### Comparing `rosettasciio-0.3/rsciio/tests/test_hamamatsu.py` & `rosettasciio-0.4/rsciio/tests/test_hamamatsu.py`

 * *Files identical despite different names*

### Comparing `rosettasciio-0.3/rsciio/tests/test_hspy.py` & `rosettasciio-0.4/rsciio/tests/test_hspy.py`

 * *Files 2% similar despite different names*

```diff
@@ -804,14 +804,93 @@
         s.plot()
         s.add_marker(m, permanent=True)
         s.save(fname)
 
         s2 = hs.load(fname)
         s2.plot()
 
+    @zspy_marker
+    def test_texts_markers(self, tmp_path, file):
+        # h5py doesn't support numpy unicode dtype and when saving ragged
+        # array with
+        fname = tmp_path / file
+
+        # Create a Signal2D with 1 navigation dimension
+        rng = np.random.default_rng(0)
+        data = np.ones((5, 100, 100))
+        s = hs.signals.Signal2D(data)
+
+        # Create an navigation dependent (ragged) Texts marker
+        offsets = np.empty(s.axes_manager.navigation_shape, dtype=object)
+        texts = np.empty(s.axes_manager.navigation_shape, dtype=object)
+
+        for index in np.ndindex(offsets.shape):
+            i = index[0]
+            offsets[index] = rng.random((5, 2))[: i + 2] * 100
+            texts[index] = np.array(["a" * (i + 1), "b", "c", "d", "e"][: i + 2])
+
+        m = hs.plot.markers.Texts(
+            offsets=offsets,
+            texts=texts,
+            sizes=3,
+            facecolor="black",
+        )
+
+        s.add_marker(m, permanent=True)
+        s.plot()
+        s.save(fname)
+
+        s2 = hs.load(fname)
+
+        m_texts = m.kwargs["texts"]
+        m2_texts = s2.metadata.Markers.Texts.kwargs["texts"]
+
+        for index in np.ndindex(m_texts.shape):
+            np.testing.assert_equal(m_texts[index], m2_texts[index])
+
+
+@zspy_marker
+@pytest.mark.parametrize("use_list", [True, False])
+def test_saving_ragged_array_string(tmp_path, file, use_list):
+    # h5py doesn't support numpy unicode dtype and when saving ragged
+    # array, we need to change the array dtype
+    fname = tmp_path / file
+
+    string_data = np.empty((5,), dtype=object)
+    for index in np.ndindex(string_data.shape):
+        i = index[0]
+        data = np.array(["a" * (i + 1), "b", "c", "d", "e"][: i + 2])
+        if use_list:
+            data = data.tolist()
+        string_data[index] = data
+
+    s = hs.signals.BaseSignal(string_data, ragged=True)
+    s.save(fname)
+
+    s2 = hs.load(fname)
+    for index in np.ndindex(s.data.shape):
+        np.testing.assert_equal(s.data[index], s2.data[index])
+
+
+@zspy_marker
+def test_saving_ragged_array_single_string(tmp_path, file):
+    fname = tmp_path / file
+
+    string_data = np.empty((2, 5), dtype=object)
+    for i, index in enumerate(np.ndindex(string_data.shape)):
+        string_data[index] = "a" * (i + 1)
+
+    s = hs.signals.BaseSignal(string_data, ragged=True)
+
+    s.save(fname, overwrite=True)
+
+    s2 = hs.load(fname)
+    for index in np.ndindex(s.data.shape):
+        np.testing.assert_equal(s.data[index], s2.data[index])
+
 
 @zspy_marker
 @pytest.mark.parametrize("lazy", [True, False])
 def test_save_load_model(tmp_path, file, lazy):
     from hyperspy._components.gaussian import Gaussian
 
     filename = tmp_path / file
@@ -852,15 +931,15 @@
     assert s1.ragged
     for i in range(len(s.data)):
         np.testing.assert_allclose(s.data[i], s1.data[i])
     assert s.__class__ == s1.__class__
 
 
 @zspy_marker
-@pytest.mark.parametrize("nav_dim", [1, 2, 3])
+@pytest.mark.parametrize("nav_dim", [1, 2])
 @pytest.mark.parametrize("lazy", [True, False])
 def test_save_ragged_dim(tmp_path, file, nav_dim, lazy):
     file = f"nav{nav_dim}_" + file
     rng = np.random.default_rng(0)
     nav_shape = np.arange(10, 10 * (nav_dim + 1), step=10)
     data = np.empty(nav_shape, dtype=object)
     for ind in np.ndindex(data.shape):
@@ -1065,7 +1144,35 @@
 
     with h5py.File(filename, mode="a") as f:
         f.attrs["file_format_version"] = "99999999"
 
     with pytest.warns(UserWarning):
         s2 = hs.load(filename)
     np.testing.assert_allclose(s.data, s2.data)
+
+
+@zspy_marker
+def test_save_metadata_empty_array(tmp_path, file):
+    filename = tmp_path / "test.hspy"
+
+    s = hs.signals.Signal1D(np.arange(100 * 1024).reshape(100, 1024))
+    s.metadata.set_item("Sample.xray_lines", np.array([]))
+
+    s.save(filename)
+    s2 = hs.load(filename)
+
+    np.testing.assert_allclose(
+        s.metadata.Sample.xray_lines, s2.metadata.Sample.xray_lines
+    )
+    np.testing.assert_allclose(s.data, s2.data)
+
+
+@zspy_marker
+def test_save_empty_signal(tmp_path, file):
+    filename = tmp_path / "test.hspy"
+
+    s = hs.signals.Signal1D([])
+
+    s.save(filename)
+    s2 = hs.load(filename)
+
+    np.testing.assert_allclose(s.data, s2.data)
```

### Comparing `rosettasciio-0.3/rsciio/tests/test_image.py` & `rosettasciio-0.4/rsciio/tests/test_image.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,20 +13,23 @@
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with RosettaSciIO. If not, see <https://www.gnu.org/licenses/#GPL>.
 
 from packaging.version import Version
+from pathlib import Path
 
 import numpy as np
 import pytest
 
 imageio = pytest.importorskip("imageio")
 
+testfile_dir = (Path(__file__).parent / "data" / "image").resolve()
+
 from rsciio.image import file_writer
 
 
 @pytest.mark.skipif(
     Version(imageio.__version__) < Version("2.23"),
     reason="needs imageio >=2.23",
 )
@@ -190,24 +193,29 @@
 
     fname = tmp_path / "test_export_size.jpg"
     s.save(fname, scalebar=True, output_size=output_size)
     s_reload = hs.load(fname)
     assert s_reload.data.shape == (512, 512)
 
 
-@pytest.mark.parametrize("output_size", (512, (512, 512)))
-def test_export_output_size_non_square(output_size, tmp_path):
+@pytest.mark.parametrize("scalebar", [True, False])
+@pytest.mark.parametrize("output_size", (None, 512, (512, 512)))
+def test_export_output_size_non_square(output_size, tmp_path, scalebar):
     hs = pytest.importorskip("hyperspy.api", reason="hyperspy not installed")
     pixels = (8, 16)
-    s = hs.signals.Signal2D(np.arange(np.multiply(*pixels)).reshape(pixels))
+    s = hs.signals.Signal2D(
+        np.arange(np.multiply(*pixels), dtype=np.uint8).reshape(pixels)
+    )
 
     fname = tmp_path / "test_export_size_non_square.jpg"
-    s.save(fname, output_size=output_size)
+    s.save(fname, output_size=output_size, scalebar=scalebar)
     s_reload = hs.load(fname)
 
+    if output_size is None:
+        output_size = (8, 16)
     if isinstance(output_size, int):
         output_size = (output_size * np.divide(*pixels), output_size)
 
     assert s_reload.data.shape == output_size
 
 
 @pytest.mark.parametrize("output_size", (None, 512))
@@ -260,7 +268,33 @@
         with pytest.raises(ValueError):
             file_writer(tmp_path / "test_image_error.jpg", signal_dict, output_size=64)
 
         with pytest.raises(ValueError):
             file_writer(
                 tmp_path / "test_image_error.jpg", signal_dict, imshow_kwds={"a": "b"}
             )
+
+
+def test_renishaw_wire():
+    hs = pytest.importorskip("hyperspy.api", reason="hyperspy not installed")
+    s = hs.load(testfile_dir / "renishaw_wire.jpg")
+    assert s.data.shape == (480, 752)
+    for axis, scale, offset, name in zip(
+        s.axes_manager.signal_axes,
+        [2.42207446, 2.503827],
+        [19105.5, -6814.538],
+        ["y", "x"],
+    ):
+        np.testing.assert_allclose(axis.scale, scale)
+        np.testing.assert_allclose(axis.offset, offset)
+        axis.name == name
+        axis.units == "µm"
+
+
+def test_export_output_size_iterable_length_1(tmp_path):
+    hs = pytest.importorskip("hyperspy.api", reason="hyperspy not installed")
+    pixels = (256, 256)
+    s = hs.signals.Signal2D(np.arange(np.multiply(*pixels)).reshape(pixels))
+
+    fname = tmp_path / "test_export_output_size_iterable_length_1.jpg"
+    with pytest.raises(ValueError):
+        s.save(fname, output_size=(256,))
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `rosettasciio-0.3/rsciio/tests/test_import.py` & `rosettasciio-0.4/rsciio/tests/test_import.py`

 * *Files identical despite different names*

### Comparing `rosettasciio-0.3/rsciio/tests/test_impulse.py` & `rosettasciio-0.4/rsciio/tests/test_impulse.py`

 * *Files identical despite different names*

### Comparing `rosettasciio-0.3/rsciio/tests/test_io.py` & `rosettasciio-0.4/rsciio/tests/test_io.py`

 * *Files identical despite different names*

### Comparing `rosettasciio-0.3/rsciio/tests/test_jeol.py` & `rosettasciio-0.4/rsciio/tests/test_jeol.py`

 * *Files identical despite different names*

### Comparing `rosettasciio-0.3/rsciio/tests/test_jobinyvon.py` & `rosettasciio-0.4/rsciio/tests/test_jobinyvon.py`

 * *Files identical despite different names*

### Comparing `rosettasciio-0.3/rsciio/tests/test_lazy_not_implemented.py` & `rosettasciio-0.4/rsciio/tests/test_lazy_not_implemented.py`

 * *Files identical despite different names*

### Comparing `rosettasciio-0.3/rsciio/tests/test_mrc.py` & `rosettasciio-0.4/rsciio/tests/test_mrc.py`

 * *Files identical despite different names*

### Comparing `rosettasciio-0.3/rsciio/tests/test_mrcz.py` & `rosettasciio-0.4/rsciio/tests/test_mrcz.py`

 * *Files identical despite different names*

### Comparing `rosettasciio-0.3/rsciio/tests/test_msa.py` & `rosettasciio-0.4/rsciio/tests/test_msa.py`

 * *Files identical despite different names*

### Comparing `rosettasciio-0.3/rsciio/tests/test_nexus.py` & `rosettasciio-0.4/rsciio/tests/test_nexus.py`

 * *Files identical despite different names*

### Comparing `rosettasciio-0.3/rsciio/tests/test_pantarhei.py` & `rosettasciio-0.4/rsciio/tests/test_pantarhei.py`

 * *Files identical despite different names*

### Comparing `rosettasciio-0.3/rsciio/tests/test_phenom.py` & `rosettasciio-0.4/rsciio/tests/test_phenom.py`

 * *Files identical despite different names*

### Comparing `rosettasciio-0.3/rsciio/tests/test_protochips.py` & `rosettasciio-0.4/rsciio/tests/test_protochips.py`

 * *Files identical despite different names*

### Comparing `rosettasciio-0.3/rsciio/tests/test_quantumdetector.py` & `rosettasciio-0.4/rsciio/tests/test_quantumdetector.py`

 * *Files 7% similar despite different names*

```diff
@@ -26,14 +26,15 @@
 import numpy as np
 import pytest
 
 from rsciio.quantumdetector._api import (
     MIBProperties,
     load_mib_data,
     parse_exposures,
+    parse_hdr_file,
     parse_timestamps,
 )
 
 hs = pytest.importorskip("hyperspy.api", reason="hyperspy not installed")
 zarr = pytest.importorskip("zarr", reason="zarr not installed")
 
 
@@ -116,29 +117,36 @@
         assert axis.units == ""
 
 
 @pytest.mark.parametrize("fname", QUAD_CHIP_FNAME_LIST)
 def test_quad_chip(fname):
     s = hs.load(TEST_DATA_DIR_UNZIPPED / fname)
     if "9_Frame" in fname:
-        navigation_shape = (9,)
+        if "24_Rows_256" in fname:
+            # Unknow why the timestamps of this file are not consistent
+            # with others
+            navigation_shape = (3, 3)
+        else:
+            navigation_shape = (9,)
     else:
         navigation_shape = ()
     assert s.data.shape == navigation_shape + (512, 512)
     assert s.data.dtype == _get_expected_dtype_from_fname(fname)
     assert s.axes_manager.signal_shape == (512, 512)
     assert s.axes_manager.navigation_shape == navigation_shape
 
     for axis in s.axes_manager.signal_axes:
         assert axis.scale == 1
         assert axis.offset == 0
         assert axis.units == ""
 
 
-@pytest.mark.parametrize("chunks", ("auto", (9, 128, 128), ("auto", 128, 128)))
+@pytest.mark.parametrize(
+    "chunks", ("auto", (3, 3, 128, 128), ("auto", "auto", 128, 128))
+)
 def test_chunks(chunks):
     fname = TEST_DATA_DIR_UNZIPPED / "Quad_9_Frame_CounterDepth_24_Rows_256.mib"
     s = hs.load(fname, lazy=True, chunks=chunks)
     chunks = normalize_chunks(chunks, shape=s.data.shape, dtype=s.data.dtype)
     assert s.data.chunks == chunks
 
 
@@ -155,15 +163,15 @@
     mib_prop.parse_file(str(fname))
     assert "\nPath: " == mib_prop.__repr__()[:7]
 
 
 def test_interrupted_acquisition():
     fname = TEST_DATA_DIR_UNZIPPED / "Single_9_Frame_CounterDepth_1_Rows_256.mib"
     # There is only 9 frames, simulate interrupted acquisition using 10 lines
-    s = hs.load(fname, navigation_shape=(10, 2))
+    s = hs.load(fname, navigation_shape=(4, 3))
     assert s.axes_manager.signal_shape == (256, 256)
     assert s.axes_manager.navigation_shape == (4, 2)
 
     s = hs.load(TEST_DATA_DIR_UNZIPPED / fname, navigation_shape=(2, 4))
     assert s.axes_manager.signal_shape == (256, 256)
     assert s.axes_manager.navigation_shape == (2, 4)
 
@@ -176,28 +184,31 @@
     assert s.axes_manager.navigation_shape == (8,)
 
     s = hs.load(fname, navigation_shape=(10, 2), first_frame=2)
     assert s.axes_manager.signal_shape == (256, 256)
     assert s.axes_manager.navigation_shape == (7,)
 
 
-def test_non_square():
+@pytest.mark.parametrize("navigation_shape", (None, (8,), (4, 2)))
+def test_non_square(navigation_shape):
     fname = TEST_DATA_DIR_UNZIPPED / "001_4x2_6bit.mib"
-    s = hs.load(fname, navigation_shape=(4, 2))
+    s = hs.load(fname, navigation_shape=navigation_shape)
     assert s.axes_manager.signal_shape == (256, 256)
-    assert s.axes_manager.navigation_shape == (4, 2)
+    if navigation_shape is None:
+        navigation_shape = (4, 2)
+    assert s.axes_manager.navigation_shape == navigation_shape
 
 
 def test_no_hdr():
     fname = TEST_DATA_DIR_UNZIPPED / "001_4x2_6bit.mib"
     fname2 = str(fname).replace(".mib", "-copy.mib")
     shutil.copyfile(fname, fname2)
     s = hs.load(fname2)
     assert s.axes_manager.signal_shape == (256, 256)
-    assert s.axes_manager.navigation_shape == (8,)
+    assert s.axes_manager.navigation_shape == (4, 2)
 
 
 @pytest.mark.parametrize(
     "kwargs",
     (
         {"first_frame": None, "last_frame": None},
         {"first_frame": 0, "last_frame": 9},
@@ -359,7 +370,27 @@
     s.save(fname2)
     s2 = hs.load(fname2)
 
     np.testing.assert_allclose(s.data, s2.data)
     assert s.axes_manager.navigation_shape == s2.axes_manager.navigation_shape
     assert s.axes_manager.signal_shape == s2.axes_manager.signal_shape
     assert s.data.dtype == s2.data.dtype
+
+
+def test_frames_in_acquisition_zero():
+    # Some hdr file have entry "Frames per Trigger (Number): 0"
+    # Possibly for "continuous and indefinite" acquisition
+    # Copy and edit a file with corresponding changes
+    base_fname = TEST_DATA_DIR_UNZIPPED / "Single_1_Frame_CounterDepth_6_Rows_256"
+    fname = f"{base_fname}_zero_frames_in_acquisition"
+    # Create test file using existing test file
+    shutil.copyfile(f"{base_fname}.mib", f"{fname}.mib")
+    hdf_dict = parse_hdr_file(f"{base_fname}.hdr")
+    hdf_dict["Frames in Acquisition (Number)"] = 0
+    with open(f"{fname}.hdr", "w") as f:
+        f.write("HDR\n")
+        for k, v in hdf_dict.items():
+            f.write(f"{k}:\t{v}\n")
+        f.write("End\t")
+
+    s = hs.load(f"{fname}.mib")
+    assert s.axes_manager.navigation_shape == ()
```

### Comparing `rosettasciio-0.3/rsciio/tests/test_renishaw.py` & `rosettasciio-0.4/rsciio/tests/test_renishaw.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,14 +35,17 @@
 testfile_map = (testfile_dir / "renishaw_test_map.wdf").resolve()
 testfile_zscan = (testfile_dir / "renishaw_test_zscan.wdf").resolve()
 testfile_undefined = (testfile_dir / "renishaw_test_undefined.wdf").resolve()
 testfile_streamline = (testfile_dir / "renishaw_test_streamline.wdf").resolve()
 testfile_map_block = (testfile_dir / "renishaw_test_map2.wdf").resolve()
 testfile_timeseries = (testfile_dir / "renishaw_test_timeseries.wdf").resolve()
 testfile_focustrack = (testfile_dir / "renishaw_test_focustrack.wdf").resolve()
+testfile_focustrack_invariant = (
+    testfile_dir / "renishaw_test_focustrack_invariant.wdf"
+).resolve()
 testfile_acc1_exptime1 = (testfile_dir / "renishaw_test_exptime1_acc1.wdf").resolve()
 testfile_acc1_exptime10 = (testfile_dir / "renishaw_test_exptime10_acc1.wdf").resolve()
 testfile_acc2_exptime1 = (testfile_dir / "renishaw_test_exptime1_acc2.wdf").resolve()
 
 
 class TestSpec:
     @classmethod
@@ -887,15 +890,15 @@
 class TestLinescan:
     @classmethod
     def setup_class(cls):
         cls.s = hs.load(
             testfile_linescan,
             reader="Renishaw",
             use_uniform_signal_axis=True,
-        )
+        )[0]
 
     @classmethod
     def teardown_class(cls):
         del cls.s
         gc.collect()
 
     def test_data(self):
@@ -967,15 +970,15 @@
 class TestMap:
     @classmethod
     def setup_class(cls):
         cls.s = hs.load(
             testfile_map,
             reader="Renishaw",
             use_uniform_signal_axis=True,
-        )
+        )[0]
 
     @classmethod
     def teardown_class(cls):
         del cls.s
         gc.collect()
 
     def test_data(self):
@@ -1176,15 +1179,15 @@
 class TestStreamline:
     @classmethod
     def setup_class(cls):
         cls.s = hs.load(
             testfile_streamline,
             reader="Renishaw",
             use_uniform_signal_axis=True,
-        )
+        )[0]
 
     @classmethod
     def teardown_class(cls):
         del cls.s
         gc.collect()
 
     def test_data(self):
@@ -1192,30 +1195,51 @@
             self.s.inav[0, 0].isig[:3].data, [418.35907, 424.54782, 409.82785]
         )
 
         np.testing.assert_allclose(
             self.s.inav[44, 48].isig[-3:].data, [587.48083, 570.73505, 583.5814]
         )
 
-    def test_original_metadata_WHTL(self):
+    def test_WHTL(self):
+        s = hs.load(
+            testfile_streamline,
+            reader="Renishaw",
+        )[1]
         expected_WTHL = {
-            "FocalPlaneResolutionUnit": "µm",
+            "FocalPlaneResolutionUnit": 5,
             "FocalPlaneXResolution": 445.75,
             "FocalPlaneYResolution": 270.85,
             "FocalPlaneXYOrigins": (-8325.176, -1334.639),
+            "ExifOffset": 114,
             "ImageDescription": "white-light image",
             "Make": "Renishaw",
             "Unknown": 20.0,
             "FieldOfViewXY": (8915.0, 5417.0),
         }
 
-        metadata_WHTL = deepcopy(self.s.original_metadata.WHTL_0.as_dictionary())
-        metadata_WHTL.pop("image", None)
+        for i, (axis, scale) in enumerate(
+            zip(s.axes_manager._axes, (22.570833, 23.710106))
+        ):
+            assert axis.units == "µm"
+            np.testing.assert_allclose(axis.scale, scale)
+            np.testing.assert_allclose(
+                axis.offset, expected_WTHL["FocalPlaneXYOrigins"][::-1][i]
+            )
+
+        metadata_WHTL = s.original_metadata.as_dictionary()["exif_tags"]
         assert metadata_WHTL == expected_WTHL
 
+        md = s.metadata.Markers.as_dictionary()
+        np.testing.assert_allclose(
+            md["Map"]["kwargs"]["offsets"],
+            [-8041.7998, -1137.6001],
+        )
+        np.testing.assert_allclose(md["Map"]["kwargs"]["widths"], 116.99999)
+        np.testing.assert_allclose(md["Map"]["kwargs"]["heights"], 127.39999)
+
     def test_original_metadata_WMAP(self):
         expected_WMAP = {
             "linefocus_size": 0,
             "flag": "column_major",
         }
         metadata_WMAP = deepcopy(self.s.original_metadata.WMAP_0.as_dictionary())
 
@@ -1259,15 +1283,15 @@
 class TestMapBlock:
     @classmethod
     def setup_class(cls):
         cls.s = hs.load(
             testfile_map_block,
             reader="Renishaw",
             use_uniform_signal_axis=True,
-        )
+        )[0]
 
     @classmethod
     def teardown_class(cls):
         del cls.s
         gc.collect()
 
     def test_original_metadata_MAP(self):
@@ -1343,27 +1367,37 @@
         gc.collect()
 
     def test_axes(self):
         axes_manager = self.s.axes_manager.as_dictionary()
         assert len(axes_manager) == 2
         z_axis = axes_manager.pop("axis-0")
 
-        np.testing.assert_allclose(z_axis["scale"], 2.9, atol=0.1)
-        np.testing.assert_allclose(z_axis["offset"], 26, atol=0.5)
+        # As hyperspy doesn't support non-ordered axis, default axis are used
+        np.testing.assert_allclose(z_axis["scale"], 1, atol=0.1)
+        np.testing.assert_allclose(z_axis["offset"], 0, atol=0.5)
 
     def test_data(self):
         np.testing.assert_allclose(
             self.s.inav[0].isig[:3].data, [1.4015186, 1.402039, -0.7012797]
         )
 
         np.testing.assert_allclose(
             self.s.inav[-1].isig[-3:].data, [4.8724666, 5.8486896, 3.8991265]
         )
 
 
+def test_focus_track_invariant():
+    s = hs.load(testfile_focustrack_invariant)
+    assert s.data.shape == (10, 1010)
+    z_axis = s.axes_manager[0]
+    assert z_axis.scale == 1
+    assert z_axis.offset == 0
+    assert str(z_axis.units) == "<undefined>"
+
+
 class TestPSETMetadata:
     data_directory = (
         Path(__file__).parent / "data" / "renishaw" / "generated_files"
     ).resolve()
 
     def get_filepath(self, filename):
         return (self.data_directory / filename).resolve()
```

### Comparing `rosettasciio-0.3/rsciio/tests/test_ripple.py` & `rosettasciio-0.4/rsciio/tests/test_ripple.py`

 * *Files 0% similar despite different names*

```diff
@@ -98,15 +98,15 @@
         s.data.dtype.name,
         "_meta" if metadata else "",
     )
     return filename
 
 
 def _create_signal(shape, dim, dtype, metadata):
-    data = np.arange(np.product(shape)).reshape(shape).astype(dtype)
+    data = np.arange(np.prod(shape)).reshape(shape).astype(dtype)
     if dim == 1:
         if len(shape) > 2:
             s = exspy.signals.EELSSpectrum(data)
             if metadata:
                 s.set_microscope_parameters(
                     beam_energy=100.0, convergence_angle=1.0, collection_angle=10.0
                 )
```

### Comparing `rosettasciio-0.3/rsciio/tests/test_semper.py` & `rosettasciio-0.4/rsciio/tests/test_semper.py`

 * *Files identical despite different names*

### Comparing `rosettasciio-0.3/rsciio/tests/test_set_log_level.py` & `rosettasciio-0.4/rsciio/tests/utils/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -11,18 +11,7 @@
 # RosettaSciIO is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with RosettaSciIO. If not, see <https://www.gnu.org/licenses/#GPL>.
-
-import pytest
-
-import rsciio
-
-
-@pytest.mark.parametrize(
-    "level", ("CRITICAL", "ERROR", "WARNING", "INFO", "DEBUG", "NOTSET")
-)
-def test_set_log_level(level):
-    rsciio.set_log_level(level)
```

### Comparing `rosettasciio-0.3/rsciio/tests/test_tia.py` & `rosettasciio-0.4/rsciio/tests/test_tia.py`

 * *Files identical despite different names*

### Comparing `rosettasciio-0.3/rsciio/tests/test_tiff.py` & `rosettasciio-0.4/rsciio/tests/test_tiff.py`

 * *Files identical despite different names*

### Comparing `rosettasciio-0.3/rsciio/tests/test_trivista.py` & `rosettasciio-0.4/rsciio/tests/test_trivista.py`

 * *Files identical despite different names*

### Comparing `rosettasciio-0.3/rsciio/tests/test_tvips.py` & `rosettasciio-0.4/rsciio/tests/test_tvips.py`

 * *Files identical despite different names*

### Comparing `rosettasciio-0.3/rsciio/tests/test_usid.py` & `rosettasciio-0.4/rsciio/tests/test_usid.py`

 * *Files identical despite different names*

### Comparing `rosettasciio-0.3/rsciio/tests/test_zspy.py` & `rosettasciio-0.4/rsciio/tests/test_zspy.py`

 * *Files identical despite different names*

### Comparing `rosettasciio-0.3/rsciio/tests/utils/__init__.py` & `rosettasciio-0.4/rsciio/utils/array.py`

 * *Files 23% similar despite different names*

```diff
@@ -11,7 +11,29 @@
 # RosettaSciIO is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with RosettaSciIO. If not, see <https://www.gnu.org/licenses/#GPL>.
+
+from packaging.version import Version
+
+import numpy as np
+
+
+def get_numpy_kwargs(array):
+    """
+    Convenience funtion to return a dictionary containing the `like` keyword
+    if numpy>=1.20.
+
+    Note
+    ----
+    `like` keyword is an experimental feature introduced in numpy 1.20 and is
+    pending on acceptance of NEP 35
+
+    """
+    kw = {}
+    if Version(np.__version__) >= Version("1.20"):
+        kw["like"] = array
+
+    return kw
```

### Comparing `rosettasciio-0.3/rsciio/tests/utils/test_rgbtools.py` & `rosettasciio-0.4/rsciio/tests/utils/test_rgbtools.py`

 * *Files identical despite different names*

### Comparing `rosettasciio-0.3/rsciio/tests/utils/test_utils.py` & `rosettasciio-0.4/rsciio/tests/utils/test_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,23 +9,23 @@
 from rsciio.utils.distributed import get_chunk_slice
 import rsciio.utils.date_time_tools as dtt
 
 
 dt = [("x", np.uint8), ("y", np.uint16), ("text", (bytes, 6))]
 
 
-MY_PATH = Path(__file__).parent
-TEST_XML_PATH = MY_PATH / ".." / "data" / "ToastedBreakFastSDD.xml"
+@pytest.fixture
+def XML_TEST_NODE():
+    MY_PATH = Path(__file__).parent
+    TEST_XML_PATH = MY_PATH / ".." / "data" / "ToastedBreakFastSDD.xml"
 
+    with open(TEST_XML_PATH, "r") as fn:
+        weird_but_valid_xml_str = fn.read()
 
-with open(TEST_XML_PATH, "r") as fn:
-    weird_but_valid_xml_str = fn.read()
-
-
-XML_TEST_NODE = ET.fromstring(weird_but_valid_xml_str)
+    yield ET.fromstring(weird_but_valid_xml_str)
 
 
 # fmt: off
 def test_msxml_sanitization():
     bad_msxml = b"""
     <main>
       <simpleFloat>0,2</simpleFloat>
@@ -38,15 +38,15 @@
     et = ET.fromstring(sanitized_xml_bytes)
     assert et[0].text == "0.2"
     assert et[1].text == "1.9E-5"
     assert et[2].text == "0.2E10"
     assert et[3].text == "0,2,3"  # is not float
 
 
-def test_default_x2d():
+def test_default_x2d(XML_TEST_NODE):
     """test of default XmlToDict translation with attributes prefixed with @,
     interchild_text_parsing set to 'first',
     no flattening tags set, and dub_text_str set to '#value'
     """
     x2d = XmlToDict()
     pynode = x2d.dictionarize(XML_TEST_NODE)
     assert (
@@ -55,28 +55,28 @@
         ]["Instance"][0]["name"]
         == 'Eggs'
     )
     t = "With one of these components"
     assert pynode["TestXML"]["Main"]["ClassInstance"]["Sample"]["#value"] == t
 
 
-def test_skip_interchild_text_flatten():
+def test_skip_interchild_text_flatten(XML_TEST_NODE):
     """test of XmlToDict translation with interchild_text_parsing set to 'skip',
     three string containing list set to flattening tags. Other kwrds - default.
     """
     x2d = XmlToDict(
         interchild_text_parsing='skip',
         tags_to_flatten=["ClassInstance", "ComponentChildren", "Instance", "TestXML"],
     )
     pynode = x2d.dictionarize(XML_TEST_NODE)
     assert pynode["Main"]["Sample"]["Components"]["name"][0] == "Eggs"
     assert pynode["Main"]["Sample"].get("#value") is None
 
 
-def test_concat_interchild_text_val_flatten():
+def test_concat_interchild_text_val_flatten(XML_TEST_NODE):
     """test of XmlToDict translator with interchild_text_parsing set to
     'cat' (concatenation), four flattening tags set, and dub_text_str set
     to '#text'
     """
     x2d = XmlToDict(
         dub_text_str="#text",
         interchild_text_parsing='cat',
@@ -87,15 +87,15 @@
     assert pynode["Instrument"]["Type"]["#text"] == "Toaster"
     assert pynode["Sample"].get("#value") is None
     assert pynode["Sample"].get("#text") is None
     t = "With one of these componentsSDD risks to be Toasted."
     assert pynode["Sample"]["#interchild_text"] == t
 
 
-def test_list_interchild_text_val_flatten():
+def test_list_interchild_text_val_flatten(XML_TEST_NODE):
     """test of XmlToDict translator interchild_text_parsing set to 'list'
     """
     x2d = XmlToDict(
         dub_text_str="#value",
         interchild_text_parsing='list',
         tags_to_flatten=["ClassInstance", "ComponentChildren", "Instance"]
     )
@@ -103,15 +103,15 @@
     assert pynode["Sample"]["#interchild_text"] == [
         "With one of these components",
         "",
         "SDD risks to be Toasted.",
     ]
 
 
-def x2d_subclass_for_custom_bool():
+def x2d_subclass_for_custom_bool(XML_TEST_NODE):
     """test subclass of XmlToDict with updated eval function"""
 
     class CustomXmlToDict(XmlToDict):
         @staticmethod
         def eval(string):
             if string == "not today":
                 return False
@@ -386,13 +386,14 @@
 
 @pytest.mark.parametrize("shape", ((10, 20, 30, 512, 512),(20, 30, 512, 512), (10, 512, 512), (512, 512)))
 def test_get_chunk_slice(shape):
     chunk_arr, chunk = get_chunk_slice(shape=shape, chunks=-1)  # 1 chunk
     assert chunk_arr.shape == (1,)*len(shape)+(len(shape), 2)
     assert chunk == tuple([(i,)for i in shape])
 
+
 @pytest.mark.parametrize("shape", ((10, 20, 30, 512, 512),(20, 30, 512, 512), (10, 512, 512), (512, 512)))
 def test_get_chunk_slice(shape):
     chunks =(1,)*(len(shape)-2) +(-1,-1)
     chunk_arr, chunk = get_chunk_slice(shape=shape, chunks=chunks)  # Eveythin is 1 chunk
     assert chunk_arr.shape == shape[:-2]+(1, 1) + (len(shape), 2)
     assert chunk == tuple([(1,)*i for i in shape[:-2]])+tuple([(i,) for i in shape[-2:]])
```

### Comparing `rosettasciio-0.3/rsciio/tia/_api.py` & `rosettasciio-0.4/rsciio/tia/_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -506,15 +506,15 @@
 def ser_reader(filename, objects=None, lazy=False, only_valid_data=True):
     """
     Reads the information from the file and returns it in the HyperSpy
     required format.
     """
     header, data = load_ser_file(filename)
     record_by = guess_record_by(header["DataTypeID"])
-    ndim = int(header["NumberDimensions"])
+    ndim = int(header["NumberDimensions"][0])
     date, time = None, None
     if objects is not None:
         objects_dict = convert_xml_to_dict(objects[0])
         try:
             acq_date = objects_dict.ObjectInfo.AcquireDate
             date, time = _get_date_time(acq_date)
         except AttributeError:
@@ -708,15 +708,15 @@
         header, data = load_ser_file(filename)
     # If the acquisition stops before finishing the job, the stored file will
     # report the requested size even though no values are recorded. Therefore
     # if the shapes of the retrieved array does not match that of the data
     # dimensions we must fill the rest with zeros or (better) nans if the
     # dtype is float
     if np.prod(array_shape) != np.prod(data["Array"].shape):
-        if int(header["NumberDimensions"]) == 1 and only_valid_data:
+        if int(header["NumberDimensions"][0]) == 1 and only_valid_data:
             # No need to fill with zeros if `TotalNumberElements !=
             # ValidNumberElements` for series data.
             # The valid data is always `0:ValidNumberElements`
             dc = data["Array"][0 : header["ValidNumberElements"][0], ...]
             array_shape[0] = header["ValidNumberElements"][0]
         else:
             # Maps will need to be filled with zeros or nans
```

### Comparing `rosettasciio-0.3/rsciio/tiff/_api.py` & `rosettasciio-0.4/rsciio/tiff/_api.py`

 * *Files identical despite different names*

### Comparing `rosettasciio-0.3/rsciio/trivista/_api.py` & `rosettasciio-0.4/rsciio/trivista/_api.py`

 * *Files identical despite different names*

### Comparing `rosettasciio-0.3/rsciio/tvips/_api.py` & `rosettasciio-0.4/rsciio/tvips/_api.py`

 * *Files identical despite different names*

### Comparing `rosettasciio-0.3/rsciio/usid/_api.py` & `rosettasciio-0.4/rsciio/usid/_api.py`

 * *Files identical despite different names*

### Comparing `rosettasciio-0.3/rsciio/utils/date_time_tools.py` & `rosettasciio-0.4/rsciio/utils/date_time_tools.py`

 * *Files identical despite different names*

### Comparing `rosettasciio-0.3/rsciio/utils/distributed.py` & `rosettasciio-0.4/rsciio/utils/distributed.py`

 * *Files identical despite different names*

### Comparing `rosettasciio-0.3/rsciio/utils/elements.py` & `rosettasciio-0.4/rsciio/utils/elements.py`

 * *Files identical despite different names*

### Comparing `rosettasciio-0.3/rsciio/utils/exceptions.py` & `rosettasciio-0.4/rsciio/utils/exceptions.py`

 * *Files 0% similar despite different names*

```diff
@@ -70,15 +70,14 @@
         self.dm3_tagID = value
 
     def __str__(self):
         return repr(self.dm3_tagID)
 
 
 class VisibleDeprecationWarning(UserWarning):
-
     """Visible deprecation warning.
     By default, python will not show deprecation warnings, so this class
     provides a visible one.
 
     """
 
     pass
```

### Comparing `rosettasciio-0.3/rsciio/utils/fei_stream_readers.py` & `rosettasciio-0.4/rsciio/utils/fei_stream_readers.py`

 * *Files identical despite different names*

### Comparing `rosettasciio-0.3/rsciio/utils/hdf5.py` & `rosettasciio-0.4/rsciio/utils/hdf5.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """HDF5 file inspection."""
+
 # -*- coding: utf-8 -*-
 # Copyright 2007-2023 The HyperSpy developers
 #
 # This file is part of RosettaSciIO.
 #
 # RosettaSciIO is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
```

### Comparing `rosettasciio-0.3/rsciio/utils/readfile.py` & `rosettasciio-0.4/rsciio/utils/readfile.py`

 * *Files identical despite different names*

### Comparing `rosettasciio-0.3/rsciio/utils/rgb_tools.py` & `rosettasciio-0.4/rsciio/utils/rgb_tools.py`

 * *Files identical despite different names*

### Comparing `rosettasciio-0.3/rsciio/utils/skimage_exposure.py` & `rosettasciio-0.4/rsciio/utils/skimage_exposure.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 """skimage's `rescale_intensity` that takes and returns dask arrays.
 """
+
 from packaging.version import Version
 import warnings
 
 import numpy as np
 import skimage
 from skimage.exposure.exposure import intensity_range, _output_dtype
```

### Comparing `rosettasciio-0.3/rsciio/utils/tests.py` & `rosettasciio-0.4/rsciio/utils/tests.py`

 * *Files identical despite different names*

### Comparing `rosettasciio-0.3/rsciio/utils/tools.py` & `rosettasciio-0.4/rsciio/utils/tools.py`

 * *Files 0% similar despite different names*

```diff
@@ -478,15 +478,15 @@
             )
     else:
         dic["package_version"] = ""
     return dic
 
 
 def ensure_unicode(stuff, encoding="utf8", encoding2="latin-1"):
-    if not isinstance(stuff, (bytes, np.string_)):
+    if not isinstance(stuff, (bytes, np.bytes_)):
         return stuff
     else:
         string = stuff
     try:
         string = string.decode(encoding)
     except Exception:
         string = string.decode(encoding2, errors="ignore")
```

### Comparing `rosettasciio-0.3/rsciio/zspy/_api.py` & `rosettasciio-0.4/rsciio/zspy/_api.py`

 * *Files 6% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 
 import logging
 from collections.abc import MutableMapping
 
 import dask.array as da
 from dask.diagnostics import ProgressBar
 import numcodecs
+import numpy as np
 import zarr
 
 from rsciio._docstrings import (
     CHUNKS_DOC,
     FILENAME_DOC,
     LAZY_DOC,
     SHOW_PROGRESSBAR_DOC,
@@ -75,48 +76,58 @@
         self.Dataset = zarr.Array
         self.Group = zarr.Group
 
 
 class ZspyWriter(HierarchicalWriter):
     target_size = 1e8
     _file_type = "zspy"
+    _unicode_kwds = dict(dtype=str)
 
     def __init__(self, file, signal, expg, **kwargs):
         super().__init__(file, signal, expg, **kwargs)
         self.Dataset = zarr.Array
-        self.unicode_kwds = {"dtype": object, "object_codec": numcodecs.JSON()}
-        self.ragged_kwds = {
-            "dtype": object,
-            "object_codec": numcodecs.VLenArray(signal["data"][0].dtype),
-            "exact": True,
-        }
 
     @staticmethod
-    def _get_object_dset(group, data, key, chunks, **kwds):
+    def _get_object_dset(group, data, key, chunks, dtype=None, **kwds):
         """Creates a Zarr Array object for saving ragged data
 
         Forces the number of chunks span the array if not a dask array as
         calculating the chunks for a ragged array is not supported. See
         https://github.com/hyperspy/rosettasciio/issues/168 for more details.
         """
         if not isinstance(data, da.Array):
             chunks = data.shape
         these_kwds = kwds.copy()
         these_kwds.update(dict(dtype=object, exact=True, chunks=chunks))
-        test_ind = data.ndim * (0,)
-        # Need to know the underlying dtype for the codec
-        # Note this can't be an object array
-        if isinstance(data, da.Array):
-            dtype = data[test_ind].compute().dtype
+
+        if dtype is None:
+            test_data = data[data.ndim * (0,)]
+            if isinstance(test_data, da.Array):
+                test_data = test_data.compute()
+            if hasattr(test_data, "dtype"):
+                # this is a numpy array
+                dtype = test_data.dtype
+            else:
+                dtype = type(test_data)
+
+        # For python type, JSON / MsgPack codecs, otherwise
+        # use VLenArray with specific numpy dtype
+        if (
+            np.issubdtype(dtype, str)
+            or np.issubdtype(dtype, list)
+            or np.issubdtype(dtype, tuple)
+        ):
+            object_codec = numcodecs.MsgPack()
         else:
-            dtype = data[test_ind].dtype
+            object_codec = numcodecs.VLenArray(dtype)
+
         dset = group.require_dataset(
             key,
             data.shape,
-            object_codec=numcodecs.VLenArray(dtype),
+            object_codec=object_codec,
             **these_kwds,
         )
         return dset
 
     @staticmethod
     def _store_data(data, dset, group, key, chunks, show_progressbar=True):
         # Tuple of dask arrays can also be passed, in which case the task graphs
```

### Comparing `rosettasciio-0.3/setup.py` & `rosettasciio-0.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -89,15 +89,14 @@
 elif len(raw_extensions) > count_c_extensions(raw_extensions):
     extensions = cythonize_extensions(raw_extensions)
 else:
     extensions = no_cythonize(raw_extensions)
 
 
 class Recythonize(Command):
-
     """cythonize all extensions"""
 
     description = "(re-)cythonize all changed cython extensions"
 
     user_options = []
 
     def initialize_options(self):
```

### Comparing `rosettasciio-0.3/upcoming_changes/README.rst` & `rosettasciio-0.4/upcoming_changes/README.rst`

 * *Files identical despite different names*

