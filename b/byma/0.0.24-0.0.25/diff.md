# Comparing `tmp/byma-0.0.24.tar.gz` & `tmp/byma-0.0.25.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "byma-0.0.24.tar", last modified: Tue Apr  2 20:20:16 2024, max compression
+gzip compressed data, was "byma-0.0.25.tar", last modified: Wed Apr  3 09:57:07 2024, max compression
```

## Comparing `byma-0.0.24.tar` & `byma-0.0.25.tar`

### file list

```diff
@@ -1,46 +1,94 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 20:20:16.484999 byma-0.0.24/
--rw-rw-rw-   0 root         (0) root         (0)       62 2024-04-02 20:20:03.000000 byma-0.0.24/.gitignore
--rw-rw-rw-   0 root         (0) root         (0)      976 2024-04-02 20:20:03.000000 byma-0.0.24/.gitlab-ci.yml
--rw-rw-rw-   0 root         (0) root         (0)       77 2024-04-02 20:20:03.000000 byma-0.0.24/CHANGELOG.txt
--rwxrwxrwx   0 root         (0) root         (0)     1836 2024-04-02 20:20:03.000000 byma-0.0.24/LICENSE.md
--rw-rw-rw-   0 root         (0) root         (0)       25 2024-04-02 20:20:03.000000 byma-0.0.24/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     1919 2024-04-02 20:20:16.483999 byma-0.0.24/PKG-INFO
--rwxrwxrwx   0 root         (0) root         (0)     1387 2024-04-02 20:20:03.000000 byma-0.0.24/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 20:20:16.478999 byma-0.0.24/byma/
--rw-rw-rw-   0 root         (0) root         (0)     1151 2024-04-02 20:20:03.000000 byma-0.0.24/byma/__init__.py
--rw-r--r--   0 root         (0) root         (0)      413 2024-04-02 20:20:16.000000 byma-0.0.24/byma/_version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 20:20:16.479999 byma-0.0.24/byma/interface/
--rw-rw-rw-   0 root         (0) root         (0)     1022 2024-04-02 20:20:03.000000 byma-0.0.24/byma/interface/BaseInterface.py
--rw-rw-rw-   0 root         (0) root         (0)     2676 2024-04-02 20:20:03.000000 byma-0.0.24/byma/interface/NonlinearHeat.py
--rw-rw-rw-   0 root         (0) root         (0)      127 2024-04-02 20:20:03.000000 byma-0.0.24/byma/interface/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 20:20:16.480999 byma-0.0.24/byma/iteral/
--rw-rw-rw-   0 root         (0) root         (0)       62 2024-04-02 20:20:03.000000 byma-0.0.24/byma/iteral/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 20:20:16.481999 byma-0.0.24/byma/iteral/nonstationary/
--rw-rw-rw-   0 root         (0) root         (0)     4104 2024-04-02 20:20:03.000000 byma-0.0.24/byma/iteral/nonstationary/Newton.py
--rw-rw-rw-   0 root         (0) root         (0)      418 2024-04-02 20:20:03.000000 byma-0.0.24/byma/iteral/nonstationary/NonStationary.py
--rw-rw-rw-   0 root         (0) root         (0)       22 2024-04-02 20:20:03.000000 byma-0.0.24/byma/iteral/nonstationary/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      355 2024-04-02 20:20:03.000000 byma-0.0.24/byma/iteral/part_1.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 20:20:16.481999 byma-0.0.24/byma/iteral/stationary/
--rw-rw-rw-   0 root         (0) root         (0)     5142 2024-04-02 20:20:03.000000 byma-0.0.24/byma/iteral/stationary/OrthogonalSubspace.py
--rw-rw-rw-   0 root         (0) root         (0)      410 2024-04-02 20:20:03.000000 byma-0.0.24/byma/iteral/stationary/Stationary.py
--rw-rw-rw-   0 root         (0) root         (0)       34 2024-04-02 20:20:03.000000 byma-0.0.24/byma/iteral/stationary/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 20:20:16.482999 byma-0.0.24/byma/nuby/
--rw-rw-rw-   0 root         (0) root         (0)      414 2024-04-02 20:20:03.000000 byma-0.0.24/byma/nuby/Bifurcation.py
--rw-rw-rw-   0 root         (0) root         (0)     6412 2024-04-02 20:20:03.000000 byma-0.0.24/byma/nuby/Continuation.py
--rw-rw-rw-   0 root         (0) root         (0)       28 2024-04-02 20:20:03.000000 byma-0.0.24/byma/nuby/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 20:20:16.482999 byma-0.0.24/byma/pyplot/
--rw-rw-rw-   0 root         (0) root         (0)       21 2024-04-02 20:20:03.000000 byma-0.0.24/byma/pyplot/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6594 2024-04-02 20:20:03.000000 byma-0.0.24/byma/pyplot/plots.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 20:20:16.483999 byma-0.0.24/byma.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1919 2024-04-02 20:20:16.000000 byma-0.0.24/byma.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      791 2024-04-02 20:20:16.000000 byma-0.0.24/byma.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-02 20:20:16.000000 byma-0.0.24/byma.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       11 2024-04-02 20:20:16.000000 byma-0.0.24/byma.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 20:20:16.483999 byma-0.0.24/examples/
--rw-rw-rw-   0 root         (0) root         (0)      877 2024-04-02 20:20:03.000000 byma-0.0.24/examples/assignment_4.py
--rwxrwxrwx   0 root         (0) root         (0)      724 2024-04-02 20:20:03.000000 byma-0.0.24/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)       22 2024-04-02 20:20:03.000000 byma-0.0.24/requirements.txt
--rw-r--r--   0 root         (0) root         (0)       38 2024-04-02 20:20:16.484999 byma-0.0.24/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1021 2024-04-02 20:20:03.000000 byma-0.0.24/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-02 20:20:16.483999 byma-0.0.24/tests/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-02 20:20:03.000000 byma-0.0.24/tests/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 09:57:07.288248 byma-0.0.25/
+-rw-rw-rw-   0 root         (0) root         (0)       78 2024-04-03 09:56:54.000000 byma-0.0.25/.gitignore
+-rw-rw-rw-   0 root         (0) root         (0)     1471 2024-04-03 09:56:54.000000 byma-0.0.25/.gitlab-ci.yml
+-rw-rw-rw-   0 root         (0) root         (0)      166 2024-04-03 09:56:54.000000 byma-0.0.25/CHANGELOG.txt
+-rwxrwxrwx   0 root         (0) root         (0)     1836 2024-04-03 09:56:54.000000 byma-0.0.25/LICENSE.md
+-rw-rw-rw-   0 root         (0) root         (0)       25 2024-04-03 09:56:54.000000 byma-0.0.25/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     1969 2024-04-03 09:57:07.287248 byma-0.0.25/PKG-INFO
+-rwxrwxrwx   0 root         (0) root         (0)     1387 2024-04-03 09:56:54.000000 byma-0.0.25/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 09:57:07.277248 byma-0.0.25/byma/
+-rw-rw-rw-   0 root         (0) root         (0)     1375 2024-04-03 09:56:54.000000 byma-0.0.25/byma/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      413 2024-04-03 09:57:06.000000 byma-0.0.25/byma/_version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 09:57:07.279248 byma-0.0.25/byma/interface/
+-rw-rw-rw-   0 root         (0) root         (0)     1022 2024-04-03 09:56:54.000000 byma-0.0.25/byma/interface/BaseInterface.py
+-rw-rw-rw-   0 root         (0) root         (0)     2676 2024-04-03 09:56:54.000000 byma-0.0.25/byma/interface/NonlinearHeat.py
+-rw-rw-rw-   0 root         (0) root         (0)      127 2024-04-03 09:56:54.000000 byma-0.0.25/byma/interface/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 09:57:07.279248 byma-0.0.25/byma/iteral/
+-rw-rw-rw-   0 root         (0) root         (0)      109 2024-04-03 09:56:54.000000 byma-0.0.25/byma/iteral/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 09:57:07.280248 byma-0.0.25/byma/iteral/nonstationary/
+-rw-rw-rw-   0 root         (0) root         (0)     4107 2024-04-03 09:56:54.000000 byma-0.0.25/byma/iteral/nonstationary/Newton.py
+-rw-rw-rw-   0 root         (0) root         (0)      418 2024-04-03 09:56:54.000000 byma-0.0.25/byma/iteral/nonstationary/NonStationary.py
+-rw-rw-rw-   0 root         (0) root         (0)      101 2024-04-03 09:56:54.000000 byma-0.0.25/byma/iteral/nonstationary/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 09:57:07.280248 byma-0.0.25/byma/iteral/stationary/
+-rw-rw-rw-   0 root         (0) root         (0)     5100 2024-04-03 09:56:54.000000 byma-0.0.25/byma/iteral/stationary/OrthogonalSubspace.py
+-rw-rw-rw-   0 root         (0) root         (0)      410 2024-04-03 09:56:54.000000 byma-0.0.25/byma/iteral/stationary/Stationary.py
+-rw-rw-rw-   0 root         (0) root         (0)      116 2024-04-03 09:56:54.000000 byma-0.0.25/byma/iteral/stationary/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 09:57:07.281248 byma-0.0.25/byma/nuby/
+-rw-rw-rw-   0 root         (0) root         (0)      393 2024-04-03 09:56:54.000000 byma-0.0.25/byma/nuby/Bifurcation.py
+-rw-rw-rw-   0 root         (0) root         (0)     6942 2024-04-03 09:56:54.000000 byma-0.0.25/byma/nuby/Continuation.py
+-rw-rw-rw-   0 root         (0) root         (0)      334 2024-04-03 09:56:54.000000 byma-0.0.25/byma/nuby/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      207 2024-04-03 09:56:54.000000 byma-0.0.25/byma/nuby/_nuby.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 09:57:07.281248 byma-0.0.25/byma/pyplot/
+-rw-rw-rw-   0 root         (0) root         (0)       21 2024-04-03 09:56:54.000000 byma-0.0.25/byma/pyplot/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6594 2024-04-03 09:56:54.000000 byma-0.0.25/byma/pyplot/plots.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 09:57:07.287248 byma-0.0.25/byma.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1969 2024-04-03 09:57:07.000000 byma-0.0.25/byma.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1900 2024-04-03 09:57:07.000000 byma-0.0.25/byma.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-03 09:57:07.000000 byma-0.0.25/byma.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       11 2024-04-03 09:57:07.000000 byma-0.0.25/byma.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 09:57:07.282248 byma-0.0.25/docs/
+-rw-rw-rw-   0 root         (0) root         (0)      638 2024-04-03 09:56:54.000000 byma-0.0.25/docs/Makefile
+-rw-rw-rw-   0 root         (0) root         (0)      804 2024-04-03 09:56:54.000000 byma-0.0.25/docs/make.bat
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 09:57:07.282248 byma-0.0.25/docs/source/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 09:57:07.282248 byma-0.0.25/docs/source/autoapi/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 09:57:07.283248 byma-0.0.25/docs/source/autoapi/byma/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 09:57:07.283248 byma-0.0.25/docs/source/autoapi/byma/_version/
+-rw-rw-rw-   0 root         (0) root         (0)      304 2024-04-03 09:56:54.000000 byma-0.0.25/docs/source/autoapi/byma/_version/index.rst
+-rw-rw-rw-   0 root         (0) root         (0)      810 2024-04-03 09:56:54.000000 byma-0.0.25/docs/source/autoapi/byma/index.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 09:57:07.283248 byma-0.0.25/docs/source/autoapi/byma/interface/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 09:57:07.283248 byma-0.0.25/docs/source/autoapi/byma/interface/BaseInterface/
+-rw-rw-rw-   0 root         (0) root         (0)      430 2024-04-03 09:56:54.000000 byma-0.0.25/docs/source/autoapi/byma/interface/BaseInterface/index.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 09:57:07.283248 byma-0.0.25/docs/source/autoapi/byma/interface/NonlinearHeat/
+-rw-rw-rw-   0 root         (0) root         (0)     1351 2024-04-03 09:56:54.000000 byma-0.0.25/docs/source/autoapi/byma/interface/NonlinearHeat/index.rst
+-rw-rw-rw-   0 root         (0) root         (0)     1637 2024-04-03 09:56:54.000000 byma-0.0.25/docs/source/autoapi/byma/interface/index.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 09:57:07.284248 byma-0.0.25/docs/source/autoapi/byma/iteral/
+-rw-rw-rw-   0 root         (0) root         (0)      197 2024-04-03 09:56:54.000000 byma-0.0.25/docs/source/autoapi/byma/iteral/index.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 09:57:07.274248 byma-0.0.25/docs/source/autoapi/byma/iteral/nonstationary/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 09:57:07.284248 byma-0.0.25/docs/source/autoapi/byma/iteral/nonstationary/Newton/
+-rw-rw-rw-   0 root         (0) root         (0)     1917 2024-04-03 09:56:54.000000 byma-0.0.25/docs/source/autoapi/byma/iteral/nonstationary/Newton/index.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 09:57:07.284248 byma-0.0.25/docs/source/autoapi/byma/iteral/nonstationary/NonStationary/
+-rw-rw-rw-   0 root         (0) root         (0)      411 2024-04-03 09:56:54.000000 byma-0.0.25/docs/source/autoapi/byma/iteral/nonstationary/NonStationary/index.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 09:57:07.284248 byma-0.0.25/docs/source/autoapi/byma/iteral/stationary/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 09:57:07.284248 byma-0.0.25/docs/source/autoapi/byma/iteral/stationary/OrthogonalSubspace/
+-rw-rw-rw-   0 root         (0) root         (0)     2437 2024-04-03 09:56:54.000000 byma-0.0.25/docs/source/autoapi/byma/iteral/stationary/OrthogonalSubspace/index.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 09:57:07.285248 byma-0.0.25/docs/source/autoapi/byma/iteral/stationary/Stationary/
+-rw-rw-rw-   0 root         (0) root         (0)      378 2024-04-03 09:56:54.000000 byma-0.0.25/docs/source/autoapi/byma/iteral/stationary/Stationary/index.rst
+-rw-rw-rw-   0 root         (0) root         (0)      462 2024-04-03 09:56:54.000000 byma-0.0.25/docs/source/autoapi/byma/iteral/stationary/index.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 09:57:07.285248 byma-0.0.25/docs/source/autoapi/byma/nuby/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 09:57:07.285248 byma-0.0.25/docs/source/autoapi/byma/nuby/Bifurcation/
+-rw-rw-rw-   0 root         (0) root         (0)      334 2024-04-03 09:56:54.000000 byma-0.0.25/docs/source/autoapi/byma/nuby/Bifurcation/index.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 09:57:07.285248 byma-0.0.25/docs/source/autoapi/byma/nuby/Continuation/
+-rw-rw-rw-   0 root         (0) root         (0)     4433 2024-04-03 09:56:54.000000 byma-0.0.25/docs/source/autoapi/byma/nuby/Continuation/index.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 09:57:07.285248 byma-0.0.25/docs/source/autoapi/byma/nuby/_nuby/
+-rw-rw-rw-   0 root         (0) root         (0)     4692 2024-04-03 09:56:54.000000 byma-0.0.25/docs/source/autoapi/byma/nuby/_nuby/index.rst
+-rw-rw-rw-   0 root         (0) root         (0)     4958 2024-04-03 09:56:54.000000 byma-0.0.25/docs/source/autoapi/byma/nuby/index.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 09:57:07.286248 byma-0.0.25/docs/source/autoapi/byma/pyplot/
+-rw-rw-rw-   0 root         (0) root         (0)     3528 2024-04-03 09:56:54.000000 byma-0.0.25/docs/source/autoapi/byma/pyplot/index.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 09:57:07.286248 byma-0.0.25/docs/source/autoapi/byma/pyplot/plots/
+-rw-rw-rw-   0 root         (0) root         (0)     3479 2024-04-03 09:56:54.000000 byma-0.0.25/docs/source/autoapi/byma/pyplot/plots/index.rst
+-rw-rw-rw-   0 root         (0) root         (0)      257 2024-04-03 09:56:54.000000 byma-0.0.25/docs/source/autoapi/index.rst
+-rw-rw-rw-   0 root         (0) root         (0)     3780 2024-04-03 09:56:54.000000 byma-0.0.25/docs/source/conf.py
+-rw-rw-rw-   0 root         (0) root         (0)     2203 2024-04-03 09:56:54.000000 byma-0.0.25/docs/source/index.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 09:57:07.287248 byma-0.0.25/docs/source/user/
+-rw-rw-rw-   0 root         (0) root         (0)       61 2024-04-03 09:56:54.000000 byma-0.0.25/docs/source/user/Installation.rst
+-rw-rw-rw-   0 root         (0) root         (0)      269 2024-04-03 09:56:54.000000 byma-0.0.25/docs/source/user/index.rst
+-rw-rw-rw-   0 root         (0) root         (0)       58 2024-04-03 09:56:54.000000 byma-0.0.25/docs/source/user/quickstart.rst
+-rw-rw-rw-   0 root         (0) root         (0)       60 2024-04-03 09:56:54.000000 byma-0.0.25/docs/source/user/whatisbyma.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 09:57:07.287248 byma-0.0.25/examples/
+-rw-rw-rw-   0 root         (0) root         (0)      887 2024-04-03 09:56:54.000000 byma-0.0.25/examples/assignment_4.py
+-rwxrwxrwx   0 root         (0) root         (0)      736 2024-04-03 09:56:54.000000 byma-0.0.25/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)       22 2024-04-03 09:56:54.000000 byma-0.0.25/requirements.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-03 09:57:07.288248 byma-0.0.25/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1021 2024-04-03 09:56:54.000000 byma-0.0.25/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 09:57:07.287248 byma-0.0.25/tests/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-03 09:56:54.000000 byma-0.0.25/tests/__init__.py
```

### Comparing `byma-0.0.24/LICENSE.md` & `byma-0.0.25/LICENSE.md`

 * *Files identical despite different names*

### Comparing `byma-0.0.24/PKG-INFO` & `byma-0.0.25/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 Metadata-Version: 2.1
 Name: byma
-Version: 0.0.24
+Version: 0.0.25
 Summary: A Numerical Mathematics Packages with an easier and clean user interface.
 Author: @b64-Lorenzo (Lorenzo Zambelli)
 Author-email: Lorenzo Zambelli <bytemath@lorenzozambelli.it>
 Project-URL: Homepage, https://gitlab.com/ByteMath/python/byma
+Keywords: python,scientific,numerical,bifurcation
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
```

### Comparing `byma-0.0.24/README.md` & `byma-0.0.25/README.md`

 * *Files identical despite different names*

### Comparing `byma-0.0.24/byma/__init__.py` & `byma-0.0.25/byma/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -11,36 +11,42 @@
 ``import byma.nuby``.
 
 ::
 
  nuby                         --- Numerical Bifurcation Analysis Tools
  iteral                       --- Tools for iterative algorithms
  pyplot                       --- Tools for plotting functions
- interface
-
-Public API in the main ByMa namespace
---------------------------------------
-::
-
- __version__       --- ByMa version string
- test              --- Run ByMa unittests
+ interface                    --- Interface functions
 
 """
 
 import importlib as _importlib
 
+try:
+    from importlib.metadata import version  # for Python 3.8+
+except ImportError:
+    from pkg_resources import get_distribution, DistributionNotFound
+    try:
+        __version__ = get_distribution(__name__).version
+    except DistributionNotFound:
+        # Package is not installed
+        __version__ = 'unknown'
+else:
+    __version__ = version(__name__)
+
+
+
 submodules = [
     'nuby',
     'iteral',
     'pyplot',
 ]
 
 __all__ = submodules + [
     'test',
-    '__version__',
 ]
 
 
 def __dir__():
     return __all__
```

### Comparing `byma-0.0.24/byma/interface/BaseInterface.py` & `byma-0.0.25/byma/interface/BaseInterface.py`

 * *Files identical despite different names*

### Comparing `byma-0.0.24/byma/interface/NonlinearHeat.py` & `byma-0.0.25/byma/interface/NonlinearHeat.py`

 * *Files identical despite different names*

### Comparing `byma-0.0.24/byma/iteral/nonstationary/Newton.py` & `byma-0.0.25/byma/iteral/nonstationary/Newton.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import numpy as np
-from interface.BaseInterface import BaseInterface
+from ...interface.BaseInterface import BaseInterface
 from .NonStationary import NonStationary as NonSt
 import scipy.sparse as sp
 
 def opts(interface={}, parameters={}, **kwargs):
     params = {
         'stop': 'matrix',
         'maxit': 1e4,
```

### Comparing `byma-0.0.24/byma/iteral/stationary/OrthogonalSubspace.py` & `byma-0.0.25/byma/iteral/stationary/OrthogonalSubspace.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 import numpy as np
 from scipy.linalg import lu, inv, solve
-# from scipy.sparse.linalg import spsolve
 from numpy.linalg import qr
 
 from interface.BaseInterface import BaseInterface
 from .Stationary import Stationary as St
 
 def opts(interface={}, parameters={}, **kwargs):
     """
```

### Comparing `byma-0.0.24/byma/nuby/Continuation.py` & `byma-0.0.25/byma/nuby/Continuation.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 import numpy as np
 import scipy.sparse as sp
-from iteral.nonstationary import newton
-
-from interface.BaseInterface import BaseInterface
+from ..iteral.nonstationary import newton
+from ..interface.BaseInterface import BaseInterface
 from .Bifurcation import Bifurcation as Bf
 
 def opts(interface={}, parameters={}, **kwargs):
     params = {
         'stop': 'matrix',
         'maxit': 1e4,
         'tol': 1e-8,
@@ -20,15 +19,32 @@
 
     base_interface = BaseInterface(default_cls=Bf, params=parameters, interface=interface)
     interface_opts, params_opts = base_interface.opts(**kwargs)
 
     return interface_opts, params_opts
 
 def step(x, df, dfmu, dx, dmu, **kwargs):
-        ''' Perform one step of the continuation '''
+        """
+    Perform one step of the continuation.
+
+    Parameters:
+        x (array_like): Current state.
+        df (callable): Function to evaluate the Jacobian matrix with respect to state variable x.
+        dfmu (callable): Function to evaluate the Jacobian matrix derivative with respect to parameter mu.
+        dx (array_like): Current tangent with respect to state variable.
+        dmu (float or array_like): Incremental change in the parameter value.
+        **kwargs: Additional keyword arguments.
+
+    Returns:
+        tuple: A tuple containing the updated state x and the norm of the correction.
+
+    Description:
+    This function performs one step of the continuation, updating the state variable x and the tangent dx using the provided functions for evaluating the Jacobian matrix and its derivative with respect to the parameter.
+
+    """
         
         # Predictor
         x += dmu * dx
         kwargs.update({'mode' : True})
         
         # Corrector 
         x, dxnorm = newton(x = x, f = dfmu, df = df, **kwargs)
@@ -46,53 +62,60 @@
             raise Exception('dx too small')
 
         
         return x, dxnorm
 
 def cont(x0, dx0, start, df, dfmu, dmu=None, target=None, **kwargs):
     """
-    Perform a continuation in parameter value from a starting value to a target value or until the maximum iteration is met, with constant step size,
-    starting from an initial state x0 and initial tangent dx0.
-
-    Returns the final state x and the final parameter value mu.
-
-    Parameters:
-        x0 (array_like): Initial state.
-        dx0 (array_like): Initial tangent with respect to state variable.
-        start (float): Starting parameter value.
-        df (callable): Function to evaluate the Jacobian matrix with respect to state variable x and parameter mu.
-        dfmu (callable): Function to evaluate the Jacobian matrix derivative with respect to parameter mu.
-        dmu (float or array_like, optional): Incremental change in the parameter value for each iteration. If None and target is None, raises ValueError.
-        target (float or None, optional): Target parameter value. If None, continuation is performed until maxit_con iterations.
-        **kwargs: Additional keyword arguments for customization.
-
-            - maxit_con (int, optional): Maximum number of continuation steps. Default is 1000.
-            - method (str, optional): Continuation method ('normal' or 'pseudo-arclength'). Default is 'normal'.
-            - mode (str, optional): Return mode ('partial' or 'full'). Default is 'partial'.
-            - Other keyword arguments: Additional parameters specific to the step function used internally.
+    Perform a continuation in parameter value from a starting value to a target value or until the maximum iteration is met, with constant step size.
 
-    Returns:
-        tuple or array_like: Depending on the mode specified in kwargs, returns either a tuple or an array.
+    This function performs a continuation in parameter space from a starting value to a target value, or until the maximum iteration is met, adjusting the state variable x along the way. The continuation is carried out using the provided functions for evaluating the Jacobian matrix and its derivative with respect to the parameter.
 
+    Parameters
+    ----------
+        x0 : array_like
+            Initial state.
+        dx0 : array_like
+            Initial tangent with respect to state variable.
+        start : float
+            Starting parameter value.
+        df : callable
+            Function to evaluate the Jacobian matrix with respect to state variable x and parameter mu.
+        dfmu : callable
+            Function to evaluate the Jacobian matrix derivative with respect to parameter mu.
+        dmu : float or array_like, optional
+            Incremental change in the parameter value for each iteration. If None and target is None, raises ValueError.
+        target : float or None, optional
+            Target parameter value. If None, continuation is performed until maxit_con iterations.
+        **kwargs : dict
+            Additional keyword arguments for customization.
+            maxit_con : int, optional
+                Maximum number of continuation steps. Default is 1000.
+            method : str, optional
+                Continuation method ('normal' or 'pseudo-arclength'). Default is 'normal'.
+            mode : str, optional
+                Return mode ('partial' or 'full'). Default is 'partial'.
+            Other keyword arguments : Additional parameters specific to the step function used internally.
+
+    Returns
+    -------
+        tuple or array_like
+            Depending on the mode specified in kwargs, returns either a tuple or an array.
             - In 'partial' mode, returns a tuple containing the final state x and the final parameter value mu.
-            - In 'full' mode, returns an array Branch containing all the states x, an array of the norm of the correction at each step, and the final parameter value mu (if target is None).
-
-    Description:
-    This function performs a continuation in parameter space from a starting value to a target value, or until the maximum iteration is met, 
-    adjusting the state variable x along the way. The continuation is carried out using the provided functions for evaluating the Jacobian 
-    matrix and its derivative with respect to the parameter. 
-
-    The continuation can be performed using either the 'normal' or 'pseudo-arclength' method, specified in the kwargs. 
-    The 'normal' method performs a simple continuation, adjusting the state variable directly based on the derivatives 
-    evaluated at each step. The 'pseudo-arclength' method is not yet implemented.
+            - In 'full' mode, returns an array containing all the states x, an array of the norm of the correction at each step, and the final parameter value mu (if target is None).
 
-    The function allows for two modes: 'partial' and 'full'. In 'partial' mode, only the final state x is returned. 
-    In 'full' mode, the function also returns an array containing the norm of the correction at each step.
+    Raises
+    ------
+        ValueError
+            If either 'dmu' or 'target' should be not 'None' but are not provided.
+        ValueError
+            If the provided continuation method is invalid. Choose either 'normal' or 'pseudo-arclength'.
 
-    Example:
+    Examples
+    --------
     >>> # Define the functions df and dfmu
     >>> def df(x, mu0):
     >>>     # Compute the Jacobian matrix with respect to state variable x and parameter mu
     >>>     pass
     >>> def dfmu(x, mu0):
     >>>     # Compute the Jacobian matrix derivative with respect to parameter mu
     >>>     pass
```

### Comparing `byma-0.0.24/byma/pyplot/plots.py` & `byma-0.0.25/byma/pyplot/plots.py`

 * *Files identical despite different names*

### Comparing `byma-0.0.24/byma.egg-info/PKG-INFO` & `byma-0.0.25/byma.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 Metadata-Version: 2.1
 Name: byma
-Version: 0.0.24
+Version: 0.0.25
 Summary: A Numerical Mathematics Packages with an easier and clean user interface.
 Author: @b64-Lorenzo (Lorenzo Zambelli)
 Author-email: Lorenzo Zambelli <bytemath@lorenzozambelli.it>
 Project-URL: Homepage, https://gitlab.com/ByteMath/python/byma
+Keywords: python,scientific,numerical,bifurcation
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
```

### Comparing `byma-0.0.24/examples/assignment_4.py` & `byma-0.0.25/examples/assignment_4.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import numpy as np
-from iteral import stationary as st
-from interface import NonlinearHeat
+from byma.iteral import stationary as st
+from byma.interface import NonlinearHeat
 import matplotlib.pyplot as plt
 import pyplot.plots as pplt
 
 
 if __name__ == '__main__':
     
     n = 4
```

### Comparing `byma-0.0.24/pyproject.toml` & `byma-0.0.25/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 requires = ["setuptools>=61.0",
   "setuptools-scm>=8.0",
   ]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "byma"
-dynamic = ["version"]
+dynamic = ["version", "keywords"]
 authors = [
   { name="Lorenzo Zambelli", email="bytemath@lorenzozambelli.it" },
 ]
 description = "A Numerical Mathematics Packages with an easier and clean user interface."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `byma-0.0.24/setup.py` & `byma-0.0.25/setup.py`

 * *Files identical despite different names*

