# Comparing `tmp/byma-0.0.25.tar.gz` & `tmp/byma-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "byma-0.0.25.tar", last modified: Wed Apr  3 09:57:07 2024, max compression
+gzip compressed data, was "byma-0.1.0.tar", last modified: Wed Apr  3 20:18:16 2024, max compression
```

## Comparing `byma-0.0.25.tar` & `byma-0.1.0.tar`

### file list

```diff
@@ -1,94 +1,96 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 09:57:07.288248 byma-0.0.25/
--rw-rw-rw-   0 root         (0) root         (0)       78 2024-04-03 09:56:54.000000 byma-0.0.25/.gitignore
--rw-rw-rw-   0 root         (0) root         (0)     1471 2024-04-03 09:56:54.000000 byma-0.0.25/.gitlab-ci.yml
--rw-rw-rw-   0 root         (0) root         (0)      166 2024-04-03 09:56:54.000000 byma-0.0.25/CHANGELOG.txt
--rwxrwxrwx   0 root         (0) root         (0)     1836 2024-04-03 09:56:54.000000 byma-0.0.25/LICENSE.md
--rw-rw-rw-   0 root         (0) root         (0)       25 2024-04-03 09:56:54.000000 byma-0.0.25/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     1969 2024-04-03 09:57:07.287248 byma-0.0.25/PKG-INFO
--rwxrwxrwx   0 root         (0) root         (0)     1387 2024-04-03 09:56:54.000000 byma-0.0.25/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 09:57:07.277248 byma-0.0.25/byma/
--rw-rw-rw-   0 root         (0) root         (0)     1375 2024-04-03 09:56:54.000000 byma-0.0.25/byma/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      413 2024-04-03 09:57:06.000000 byma-0.0.25/byma/_version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 09:57:07.279248 byma-0.0.25/byma/interface/
--rw-rw-rw-   0 root         (0) root         (0)     1022 2024-04-03 09:56:54.000000 byma-0.0.25/byma/interface/BaseInterface.py
--rw-rw-rw-   0 root         (0) root         (0)     2676 2024-04-03 09:56:54.000000 byma-0.0.25/byma/interface/NonlinearHeat.py
--rw-rw-rw-   0 root         (0) root         (0)      127 2024-04-03 09:56:54.000000 byma-0.0.25/byma/interface/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 09:57:07.279248 byma-0.0.25/byma/iteral/
--rw-rw-rw-   0 root         (0) root         (0)      109 2024-04-03 09:56:54.000000 byma-0.0.25/byma/iteral/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 09:57:07.280248 byma-0.0.25/byma/iteral/nonstationary/
--rw-rw-rw-   0 root         (0) root         (0)     4107 2024-04-03 09:56:54.000000 byma-0.0.25/byma/iteral/nonstationary/Newton.py
--rw-rw-rw-   0 root         (0) root         (0)      418 2024-04-03 09:56:54.000000 byma-0.0.25/byma/iteral/nonstationary/NonStationary.py
--rw-rw-rw-   0 root         (0) root         (0)      101 2024-04-03 09:56:54.000000 byma-0.0.25/byma/iteral/nonstationary/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 09:57:07.280248 byma-0.0.25/byma/iteral/stationary/
--rw-rw-rw-   0 root         (0) root         (0)     5100 2024-04-03 09:56:54.000000 byma-0.0.25/byma/iteral/stationary/OrthogonalSubspace.py
--rw-rw-rw-   0 root         (0) root         (0)      410 2024-04-03 09:56:54.000000 byma-0.0.25/byma/iteral/stationary/Stationary.py
--rw-rw-rw-   0 root         (0) root         (0)      116 2024-04-03 09:56:54.000000 byma-0.0.25/byma/iteral/stationary/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 09:57:07.281248 byma-0.0.25/byma/nuby/
--rw-rw-rw-   0 root         (0) root         (0)      393 2024-04-03 09:56:54.000000 byma-0.0.25/byma/nuby/Bifurcation.py
--rw-rw-rw-   0 root         (0) root         (0)     6942 2024-04-03 09:56:54.000000 byma-0.0.25/byma/nuby/Continuation.py
--rw-rw-rw-   0 root         (0) root         (0)      334 2024-04-03 09:56:54.000000 byma-0.0.25/byma/nuby/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      207 2024-04-03 09:56:54.000000 byma-0.0.25/byma/nuby/_nuby.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 09:57:07.281248 byma-0.0.25/byma/pyplot/
--rw-rw-rw-   0 root         (0) root         (0)       21 2024-04-03 09:56:54.000000 byma-0.0.25/byma/pyplot/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6594 2024-04-03 09:56:54.000000 byma-0.0.25/byma/pyplot/plots.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 09:57:07.287248 byma-0.0.25/byma.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1969 2024-04-03 09:57:07.000000 byma-0.0.25/byma.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1900 2024-04-03 09:57:07.000000 byma-0.0.25/byma.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-03 09:57:07.000000 byma-0.0.25/byma.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       11 2024-04-03 09:57:07.000000 byma-0.0.25/byma.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 09:57:07.282248 byma-0.0.25/docs/
--rw-rw-rw-   0 root         (0) root         (0)      638 2024-04-03 09:56:54.000000 byma-0.0.25/docs/Makefile
--rw-rw-rw-   0 root         (0) root         (0)      804 2024-04-03 09:56:54.000000 byma-0.0.25/docs/make.bat
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 09:57:07.282248 byma-0.0.25/docs/source/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 09:57:07.282248 byma-0.0.25/docs/source/autoapi/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 09:57:07.283248 byma-0.0.25/docs/source/autoapi/byma/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 09:57:07.283248 byma-0.0.25/docs/source/autoapi/byma/_version/
--rw-rw-rw-   0 root         (0) root         (0)      304 2024-04-03 09:56:54.000000 byma-0.0.25/docs/source/autoapi/byma/_version/index.rst
--rw-rw-rw-   0 root         (0) root         (0)      810 2024-04-03 09:56:54.000000 byma-0.0.25/docs/source/autoapi/byma/index.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 09:57:07.283248 byma-0.0.25/docs/source/autoapi/byma/interface/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 09:57:07.283248 byma-0.0.25/docs/source/autoapi/byma/interface/BaseInterface/
--rw-rw-rw-   0 root         (0) root         (0)      430 2024-04-03 09:56:54.000000 byma-0.0.25/docs/source/autoapi/byma/interface/BaseInterface/index.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 09:57:07.283248 byma-0.0.25/docs/source/autoapi/byma/interface/NonlinearHeat/
--rw-rw-rw-   0 root         (0) root         (0)     1351 2024-04-03 09:56:54.000000 byma-0.0.25/docs/source/autoapi/byma/interface/NonlinearHeat/index.rst
--rw-rw-rw-   0 root         (0) root         (0)     1637 2024-04-03 09:56:54.000000 byma-0.0.25/docs/source/autoapi/byma/interface/index.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 09:57:07.284248 byma-0.0.25/docs/source/autoapi/byma/iteral/
--rw-rw-rw-   0 root         (0) root         (0)      197 2024-04-03 09:56:54.000000 byma-0.0.25/docs/source/autoapi/byma/iteral/index.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 09:57:07.274248 byma-0.0.25/docs/source/autoapi/byma/iteral/nonstationary/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 09:57:07.284248 byma-0.0.25/docs/source/autoapi/byma/iteral/nonstationary/Newton/
--rw-rw-rw-   0 root         (0) root         (0)     1917 2024-04-03 09:56:54.000000 byma-0.0.25/docs/source/autoapi/byma/iteral/nonstationary/Newton/index.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 09:57:07.284248 byma-0.0.25/docs/source/autoapi/byma/iteral/nonstationary/NonStationary/
--rw-rw-rw-   0 root         (0) root         (0)      411 2024-04-03 09:56:54.000000 byma-0.0.25/docs/source/autoapi/byma/iteral/nonstationary/NonStationary/index.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 09:57:07.284248 byma-0.0.25/docs/source/autoapi/byma/iteral/stationary/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 09:57:07.284248 byma-0.0.25/docs/source/autoapi/byma/iteral/stationary/OrthogonalSubspace/
--rw-rw-rw-   0 root         (0) root         (0)     2437 2024-04-03 09:56:54.000000 byma-0.0.25/docs/source/autoapi/byma/iteral/stationary/OrthogonalSubspace/index.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 09:57:07.285248 byma-0.0.25/docs/source/autoapi/byma/iteral/stationary/Stationary/
--rw-rw-rw-   0 root         (0) root         (0)      378 2024-04-03 09:56:54.000000 byma-0.0.25/docs/source/autoapi/byma/iteral/stationary/Stationary/index.rst
--rw-rw-rw-   0 root         (0) root         (0)      462 2024-04-03 09:56:54.000000 byma-0.0.25/docs/source/autoapi/byma/iteral/stationary/index.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 09:57:07.285248 byma-0.0.25/docs/source/autoapi/byma/nuby/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 09:57:07.285248 byma-0.0.25/docs/source/autoapi/byma/nuby/Bifurcation/
--rw-rw-rw-   0 root         (0) root         (0)      334 2024-04-03 09:56:54.000000 byma-0.0.25/docs/source/autoapi/byma/nuby/Bifurcation/index.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 09:57:07.285248 byma-0.0.25/docs/source/autoapi/byma/nuby/Continuation/
--rw-rw-rw-   0 root         (0) root         (0)     4433 2024-04-03 09:56:54.000000 byma-0.0.25/docs/source/autoapi/byma/nuby/Continuation/index.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 09:57:07.285248 byma-0.0.25/docs/source/autoapi/byma/nuby/_nuby/
--rw-rw-rw-   0 root         (0) root         (0)     4692 2024-04-03 09:56:54.000000 byma-0.0.25/docs/source/autoapi/byma/nuby/_nuby/index.rst
--rw-rw-rw-   0 root         (0) root         (0)     4958 2024-04-03 09:56:54.000000 byma-0.0.25/docs/source/autoapi/byma/nuby/index.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 09:57:07.286248 byma-0.0.25/docs/source/autoapi/byma/pyplot/
--rw-rw-rw-   0 root         (0) root         (0)     3528 2024-04-03 09:56:54.000000 byma-0.0.25/docs/source/autoapi/byma/pyplot/index.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 09:57:07.286248 byma-0.0.25/docs/source/autoapi/byma/pyplot/plots/
--rw-rw-rw-   0 root         (0) root         (0)     3479 2024-04-03 09:56:54.000000 byma-0.0.25/docs/source/autoapi/byma/pyplot/plots/index.rst
--rw-rw-rw-   0 root         (0) root         (0)      257 2024-04-03 09:56:54.000000 byma-0.0.25/docs/source/autoapi/index.rst
--rw-rw-rw-   0 root         (0) root         (0)     3780 2024-04-03 09:56:54.000000 byma-0.0.25/docs/source/conf.py
--rw-rw-rw-   0 root         (0) root         (0)     2203 2024-04-03 09:56:54.000000 byma-0.0.25/docs/source/index.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 09:57:07.287248 byma-0.0.25/docs/source/user/
--rw-rw-rw-   0 root         (0) root         (0)       61 2024-04-03 09:56:54.000000 byma-0.0.25/docs/source/user/Installation.rst
--rw-rw-rw-   0 root         (0) root         (0)      269 2024-04-03 09:56:54.000000 byma-0.0.25/docs/source/user/index.rst
--rw-rw-rw-   0 root         (0) root         (0)       58 2024-04-03 09:56:54.000000 byma-0.0.25/docs/source/user/quickstart.rst
--rw-rw-rw-   0 root         (0) root         (0)       60 2024-04-03 09:56:54.000000 byma-0.0.25/docs/source/user/whatisbyma.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 09:57:07.287248 byma-0.0.25/examples/
--rw-rw-rw-   0 root         (0) root         (0)      887 2024-04-03 09:56:54.000000 byma-0.0.25/examples/assignment_4.py
--rwxrwxrwx   0 root         (0) root         (0)      736 2024-04-03 09:56:54.000000 byma-0.0.25/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)       22 2024-04-03 09:56:54.000000 byma-0.0.25/requirements.txt
--rw-r--r--   0 root         (0) root         (0)       38 2024-04-03 09:57:07.288248 byma-0.0.25/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1021 2024-04-03 09:56:54.000000 byma-0.0.25/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 09:57:07.287248 byma-0.0.25/tests/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-03 09:56:54.000000 byma-0.0.25/tests/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 20:18:16.496358 byma-0.1.0/
+-rw-rw-rw-   0 root         (0) root         (0)       78 2024-04-03 20:18:02.000000 byma-0.1.0/.gitignore
+-rw-rw-rw-   0 root         (0) root         (0)     1604 2024-04-03 20:18:02.000000 byma-0.1.0/.gitlab-ci.yml
+-rw-rw-rw-   0 root         (0) root         (0)      166 2024-04-03 20:18:02.000000 byma-0.1.0/CHANGELOG.txt
+-rwxrwxrwx   0 root         (0) root         (0)     1836 2024-04-03 20:18:02.000000 byma-0.1.0/LICENSE.md
+-rw-rw-rw-   0 root         (0) root         (0)       25 2024-04-03 20:18:02.000000 byma-0.1.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     3119 2024-04-03 20:18:16.496358 byma-0.1.0/PKG-INFO
+-rwxrwxrwx   0 root         (0) root         (0)     2538 2024-04-03 20:18:02.000000 byma-0.1.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 20:18:16.485358 byma-0.1.0/byma/
+-rw-rw-rw-   0 root         (0) root         (0)     1375 2024-04-03 20:18:02.000000 byma-0.1.0/byma/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      411 2024-04-03 20:18:16.000000 byma-0.1.0/byma/_version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 20:18:16.487357 byma-0.1.0/byma/interface/
+-rw-rw-rw-   0 root         (0) root         (0)     1833 2024-04-03 20:18:02.000000 byma-0.1.0/byma/interface/BaseInterface.py
+-rw-rw-rw-   0 root         (0) root         (0)     2970 2024-04-03 20:18:02.000000 byma-0.1.0/byma/interface/NonlinearHeat.py
+-rw-rw-rw-   0 root         (0) root         (0)      379 2024-04-03 20:18:02.000000 byma-0.1.0/byma/interface/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 20:18:16.487357 byma-0.1.0/byma/iteral/
+-rw-rw-rw-   0 root         (0) root         (0)      109 2024-04-03 20:18:02.000000 byma-0.1.0/byma/iteral/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 20:18:16.488358 byma-0.1.0/byma/iteral/nonstationary/
+-rw-rw-rw-   0 root         (0) root         (0)     4058 2024-04-03 20:18:02.000000 byma-0.1.0/byma/iteral/nonstationary/Newton.py
+-rw-rw-rw-   0 root         (0) root         (0)      185 2024-04-03 20:18:02.000000 byma-0.1.0/byma/iteral/nonstationary/NonStationary.py
+-rw-rw-rw-   0 root         (0) root         (0)      101 2024-04-03 20:18:02.000000 byma-0.1.0/byma/iteral/nonstationary/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 20:18:16.488358 byma-0.1.0/byma/iteral/stationary/
+-rw-rw-rw-   0 root         (0) root         (0)     4730 2024-04-03 20:18:02.000000 byma-0.1.0/byma/iteral/stationary/OrthogonalSubspace.py
+-rw-rw-rw-   0 root         (0) root         (0)      173 2024-04-03 20:18:02.000000 byma-0.1.0/byma/iteral/stationary/Stationary.py
+-rw-rw-rw-   0 root         (0) root         (0)      116 2024-04-03 20:18:02.000000 byma-0.1.0/byma/iteral/stationary/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 20:18:16.489358 byma-0.1.0/byma/nuby/
+-rw-rw-rw-   0 root         (0) root         (0)      160 2024-04-03 20:18:02.000000 byma-0.1.0/byma/nuby/Bifurcation.py
+-rw-rw-rw-   0 root         (0) root         (0)     6929 2024-04-03 20:18:02.000000 byma-0.1.0/byma/nuby/Continuation.py
+-rw-rw-rw-   0 root         (0) root         (0)      334 2024-04-03 20:18:02.000000 byma-0.1.0/byma/nuby/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      199 2024-04-03 20:18:02.000000 byma-0.1.0/byma/nuby/_nuby.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 20:18:16.489358 byma-0.1.0/byma/pyplot/
+-rw-rw-rw-   0 root         (0) root         (0)       21 2024-04-03 20:18:02.000000 byma-0.1.0/byma/pyplot/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4998 2024-04-03 20:18:02.000000 byma-0.1.0/byma/pyplot/plots.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 20:18:16.496358 byma-0.1.0/byma.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3119 2024-04-03 20:18:16.000000 byma-0.1.0/byma.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1978 2024-04-03 20:18:16.000000 byma-0.1.0/byma.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-03 20:18:16.000000 byma-0.1.0/byma.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       11 2024-04-03 20:18:16.000000 byma-0.1.0/byma.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 20:18:16.490357 byma-0.1.0/docs/
+-rw-rw-rw-   0 root         (0) root         (0)      638 2024-04-03 20:18:02.000000 byma-0.1.0/docs/Makefile
+-rw-rw-rw-   0 root         (0) root         (0)      804 2024-04-03 20:18:02.000000 byma-0.1.0/docs/make.bat
+-rw-rw-rw-   0 root         (0) root         (0)      123 2024-04-03 20:18:02.000000 byma-0.1.0/docs/requirements.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 20:18:16.490357 byma-0.1.0/docs/source/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 20:18:16.491358 byma-0.1.0/docs/source/autoapi/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 20:18:16.491358 byma-0.1.0/docs/source/autoapi/byma/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 20:18:16.491358 byma-0.1.0/docs/source/autoapi/byma/_version/
+-rw-rw-rw-   0 root         (0) root         (0)      304 2024-04-03 20:18:02.000000 byma-0.1.0/docs/source/autoapi/byma/_version/index.rst
+-rw-rw-rw-   0 root         (0) root         (0)      810 2024-04-03 20:18:02.000000 byma-0.1.0/docs/source/autoapi/byma/index.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 20:18:16.491358 byma-0.1.0/docs/source/autoapi/byma/interface/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 20:18:16.491358 byma-0.1.0/docs/source/autoapi/byma/interface/BaseInterface/
+-rw-rw-rw-   0 root         (0) root         (0)     1132 2024-04-03 20:18:02.000000 byma-0.1.0/docs/source/autoapi/byma/interface/BaseInterface/index.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 20:18:16.492358 byma-0.1.0/docs/source/autoapi/byma/interface/NonlinearHeat/
+-rw-rw-rw-   0 root         (0) root         (0)     2120 2024-04-03 20:18:02.000000 byma-0.1.0/docs/source/autoapi/byma/interface/NonlinearHeat/index.rst
+-rw-rw-rw-   0 root         (0) root         (0)     3387 2024-04-03 20:18:02.000000 byma-0.1.0/docs/source/autoapi/byma/interface/index.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 20:18:16.492358 byma-0.1.0/docs/source/autoapi/byma/iteral/
+-rw-rw-rw-   0 root         (0) root         (0)      197 2024-04-03 20:18:02.000000 byma-0.1.0/docs/source/autoapi/byma/iteral/index.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 20:18:16.492358 byma-0.1.0/docs/source/autoapi/byma/iteral/nonstationary/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 20:18:16.492358 byma-0.1.0/docs/source/autoapi/byma/iteral/nonstationary/Newton/
+-rw-rw-rw-   0 root         (0) root         (0)     1901 2024-04-03 20:18:02.000000 byma-0.1.0/docs/source/autoapi/byma/iteral/nonstationary/Newton/index.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 20:18:16.492358 byma-0.1.0/docs/source/autoapi/byma/iteral/nonstationary/NonStationary/
+-rw-rw-rw-   0 root         (0) root         (0)      378 2024-04-03 20:18:02.000000 byma-0.1.0/docs/source/autoapi/byma/iteral/nonstationary/NonStationary/index.rst
+-rw-rw-rw-   0 root         (0) root         (0)      441 2024-04-03 20:18:02.000000 byma-0.1.0/docs/source/autoapi/byma/iteral/nonstationary/index.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 20:18:16.493358 byma-0.1.0/docs/source/autoapi/byma/iteral/stationary/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 20:18:16.493358 byma-0.1.0/docs/source/autoapi/byma/iteral/stationary/OrthogonalSubspace/
+-rw-rw-rw-   0 root         (0) root         (0)     2167 2024-04-03 20:18:02.000000 byma-0.1.0/docs/source/autoapi/byma/iteral/stationary/OrthogonalSubspace/index.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 20:18:16.493358 byma-0.1.0/docs/source/autoapi/byma/iteral/stationary/Stationary/
+-rw-rw-rw-   0 root         (0) root         (0)      345 2024-04-03 20:18:02.000000 byma-0.1.0/docs/source/autoapi/byma/iteral/stationary/Stationary/index.rst
+-rw-rw-rw-   0 root         (0) root         (0)      429 2024-04-03 20:18:02.000000 byma-0.1.0/docs/source/autoapi/byma/iteral/stationary/index.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 20:18:16.493358 byma-0.1.0/docs/source/autoapi/byma/nuby/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 20:18:16.493358 byma-0.1.0/docs/source/autoapi/byma/nuby/Bifurcation/
+-rw-rw-rw-   0 root         (0) root         (0)      301 2024-04-03 20:18:02.000000 byma-0.1.0/docs/source/autoapi/byma/nuby/Bifurcation/index.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 20:18:16.494358 byma-0.1.0/docs/source/autoapi/byma/nuby/Continuation/
+-rw-rw-rw-   0 root         (0) root         (0)     4354 2024-04-03 20:18:02.000000 byma-0.1.0/docs/source/autoapi/byma/nuby/Continuation/index.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 20:18:16.494358 byma-0.1.0/docs/source/autoapi/byma/nuby/_nuby/
+-rw-rw-rw-   0 root         (0) root         (0)     4587 2024-04-03 20:18:02.000000 byma-0.1.0/docs/source/autoapi/byma/nuby/_nuby/index.rst
+-rw-rw-rw-   0 root         (0) root         (0)     4859 2024-04-03 20:18:02.000000 byma-0.1.0/docs/source/autoapi/byma/nuby/index.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 20:18:16.494358 byma-0.1.0/docs/source/autoapi/byma/pyplot/
+-rw-rw-rw-   0 root         (0) root         (0)     2752 2024-04-03 20:18:02.000000 byma-0.1.0/docs/source/autoapi/byma/pyplot/index.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 20:18:16.494358 byma-0.1.0/docs/source/autoapi/byma/pyplot/plots/
+-rw-rw-rw-   0 root         (0) root         (0)     2697 2024-04-03 20:18:02.000000 byma-0.1.0/docs/source/autoapi/byma/pyplot/plots/index.rst
+-rw-rw-rw-   0 root         (0) root         (0)      241 2024-04-03 20:18:02.000000 byma-0.1.0/docs/source/autoapi/index.rst
+-rw-rw-rw-   0 root         (0) root         (0)     3805 2024-04-03 20:18:02.000000 byma-0.1.0/docs/source/conf.py
+-rw-rw-rw-   0 root         (0) root         (0)     2203 2024-04-03 20:18:02.000000 byma-0.1.0/docs/source/index.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 20:18:16.495358 byma-0.1.0/docs/source/user/
+-rw-rw-rw-   0 root         (0) root         (0)       61 2024-04-03 20:18:02.000000 byma-0.1.0/docs/source/user/Installation.rst
+-rw-rw-rw-   0 root         (0) root         (0)      269 2024-04-03 20:18:02.000000 byma-0.1.0/docs/source/user/index.rst
+-rw-rw-rw-   0 root         (0) root         (0)       58 2024-04-03 20:18:02.000000 byma-0.1.0/docs/source/user/quickstart.rst
+-rw-rw-rw-   0 root         (0) root         (0)       60 2024-04-03 20:18:02.000000 byma-0.1.0/docs/source/user/whatisbyma.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 20:18:16.495358 byma-0.1.0/examples/
+-rw-rw-rw-   0 root         (0) root         (0)      887 2024-04-03 20:18:02.000000 byma-0.1.0/examples/assignment_4.py
+-rwxrwxrwx   0 root         (0) root         (0)      736 2024-04-03 20:18:02.000000 byma-0.1.0/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)       22 2024-04-03 20:18:02.000000 byma-0.1.0/requirements.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-03 20:18:16.496358 byma-0.1.0/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1021 2024-04-03 20:18:02.000000 byma-0.1.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 20:18:16.495358 byma-0.1.0/tests/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-03 20:18:02.000000 byma-0.1.0/tests/__init__.py
```

### Comparing `byma-0.0.25/.gitlab-ci.yml` & `byma-0.1.0/.gitlab-ci.yml`

 * *Files 16% similar despite different names*

```diff
@@ -1,50 +1,54 @@
 image: python:latest
 
 stages:
   - Packages
-  - Build & Publish
+  - Build
+  - Publish
   - Pages deployment
 
 install-framework:
   stage: Packages
   script:
     - python -m pip install --upgrade pip
     - pip install -r requirements.txt
     - pip install twine
     - pip install .
+  rules:
+    - if: '$CI_COMMIT_TAG'
 
 publish-testpypi:
-  stage: Build & Publish
+  stage: Publish
   script: 
     - pip install build twine
     - python -m build
     - python -m twine upload --repository testpypi --username $TEST_PYPI_USERNAME --password $TEST_PYPI_PASSWORD dist/*
-  except:
-    - /^v\d+\.\d+\.\d+$/
+  rules:
+    - if: '$CI_COMMIT_TAG && $CI_COMMIT_TAG != /^v\d+\.\d+\.\d+$/'
+
 
 publish:
-  stage: Build & Publish
-  script: 
+  stage: Publish
+  script:
     - pip install build twine
     - python -m build
     - TWINE_PASSWORD=${CI_JOB_TOKEN} TWINE_USERNAME=gitlab-ci-token python -m twine upload --repository-url ${CI_API_V4_URL}/projects/${CI_PROJECT_ID}/packages/pypi dist/*
     - python -m twine upload --repository pypi --username "${PYPI_USERNAME}" --password "${PYPI_PASSWORD}" --verbose dist/*
   only:
     - /^v\d+\.\d+\.\d+$/  # This will match tags with the format vX.Y.Z
 
 # Push the book's HTML to gitlab-pages
 pages:
   stage: Pages deployment
   image: python:3.9-slim
-  before_script:
-    - apt-get update && apt-get install make --no-install-recommends -y
-    - python -m pip install sphinx furo sphinx_rtd_theme sphinx-build
   script:
+    - apt-get update && apt-get install make --no-install-recommends -y
+    - python -m pip install -r docs/requirements.txt
+    - pip install -r requirements.txt
+    - pip install byma
     - sphinx-build -M html docs/source/ docs/build/  
     - mv docs/build/html/ public/
   artifacts:
     paths:
       - public
   rules:
-    - allow_failure: true
-    - if: $CI_COMMIT_BRANCH == $CI_DEFAULT_BRANCH
+    - if: ('$CI_COMMIT_TAG =~ /^v\d+\.\d+\.\d+$/ || $CI_COMMIT_TAG == null') && $CI_COMMIT_BRANCH == $CI_DEFAULT_BRANCH
```

### Comparing `byma-0.0.25/LICENSE.md` & `byma-0.1.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `byma-0.0.25/PKG-INFO` & `byma-0.1.0/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,23 +1,33 @@
 Metadata-Version: 2.1
 Name: byma
-Version: 0.0.25
+Version: 0.1.0
 Summary: A Numerical Mathematics Packages with an easier and clean user interface.
 Author: @b64-Lorenzo (Lorenzo Zambelli)
 Author-email: Lorenzo Zambelli <bytemath@lorenzozambelli.it>
 Project-URL: Homepage, https://gitlab.com/ByteMath/python/byma
 Keywords: python,scientific,numerical,bifurcation
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 
 # ByMa
+![PyPI - Version](https://img.shields.io/pypi/v/byma?style=plastic&label=ByMa&labelColor=green&color=blue&link=https%3A%2F%2Fbytemath.gitlab.io%2Fpython%2FByMa%2Findex.html)
+[![PyPI Downloads](https://img.shields.io/pypi/dm/label=PyPI%20downloads)](
+https://pypi.org/project/byma/)
+[![Conda Downloads](https://img.shields.io/conda/dn/conda-forge/label=Conda%20downloads)](https://anaconda.org/conda-forge/byma)
+![Libraries.io dependency status for specific release](https://img.shields.io/librariesio/release/pypi/numpy/1.1.1?style=plastic&logo=numpy&label=NumPy&labelColor=blue&link=https%3A%2F%2Fnumpy.org%2F)
+![Libraries.io dependency status for specific release](https://img.shields.io/librariesio/release/pypi/scipy/1.0.0?style=plastic&logo=scipy&label=SciPy&labelColor=light%20blue&link=https%3A%2F%2Fscipy.org%2F)
+![GitLab Last Commit](https://img.shields.io/gitlab/last-commit/ByteMath%2Fpython%2FByMa?gitlab_url=https%3A%2F%2Fgitlab.com%2FByteMath%2Fpython%2FByMa&style=plastic)
+![Static Badge](https://img.shields.io/badge/Docs-Read?style=plastic&label=Read&color=purple&link=https%3A%2F%2Fbytemath.gitlab.io%2Fpython%2FByMa%2Findex.html)
+
+
 
 ByMa is a Python package designed to facilitate numerical mathematics tasks by implementing a range of standard methods, from iterative techniques to bifurcation methods. Noted for its simplicity, clarity, and efficiency, ByMa aims to enhance the learning experience for newcomers to numerical mathematics while streamlining the implementation and utilization of popular scientific libraries such as NumPy, SciPy, and Matplotlib.
 
 
 ## Installation
 
 ByMa is best installed in a [virtual environment](https://docs.python.org/3/library/venv.html).
```

### Comparing `byma-0.0.25/byma/__init__.py` & `byma-0.1.0/byma/__init__.py`

 * *Files identical despite different names*

### Comparing `byma-0.0.25/byma/iteral/nonstationary/Newton.py` & `byma-0.1.0/byma/iteral/nonstationary/Newton.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,73 +1,79 @@
 import numpy as np
-from ...interface.BaseInterface import BaseInterface
+from ...interface.BaseInterface import BaseInterface as bs
 from .NonStationary import NonStationary as NonSt
 import scipy.sparse as sp
 
-def opts(interface={}, parameters={}, **kwargs):
-    params = {
-        'stop': 'matrix',
-        'maxit': 1e4,
-        'tol': 1e-8,
-        'method': 'standard'  # Default linear system solving method
+_DEFAULT_OPTS = {
+    'stop': 'normal', 
+    'maxit': 1e4, 
+    'tol': 1e-8, 
+    'verbose': False,
+    'mode': None, 
+    'method': 'normal',
     }
-    intf = {
-        'verbose': True,
-        'mode': True,
-    }
-    parameters.update(params)
-    interface.update(intf)
-
-    base_interface = BaseInterface(default_cls=NonSt, params=parameters, interface=interface)
-    interface_opts, params_opts = base_interface.opts(**kwargs)
 
-    return interface_opts, params_opts
 
+@bs.set_defaults(default_cls = NonSt, default_opts=_DEFAULT_OPTS)
 def newton(x, f, df, **kwargs):
     """
-    Newton iterations.
-    
-    Parameters:
-        x (array_like): Initial guess for the root.
-        f (callable): Function to evaluate the residuals.
-        df (callable): Function to evaluate the Jacobian matrix.
-        **kwargs: Additional keyword arguments for customization.
-            - tol (float): Tolerance for convergence. Default is 1e-8.
-            - maxit (int): Maximum number of iterations. Default is 10000.
-            - verbose (bool): If True, prints iteration information. Default is True.
-            - mode (bool): If True, returns additional iteration information. Default is True.
+    Perform Newton iterations to find the root of a given function.
     
-    
-    Returns:
-        tuple: Tuple containing the root and optionally the number of iterations and norm of correction.
-               If mode is True, returns (root, iterations, norm_correction), otherwise just returns root.
-    
-    Raises:
+    :param x: array_like
+        Initial guess for the root.
+    :param f: callable
+        Function to evaluate the residuals.
+    :param df: callable
+        Function to evaluate the Jacobian matrix.
+    :param kwargs: dict
+        Additional keyword arguments for customization.
+        - tol (float): Tolerance for convergence. Default is 1e-8.
+        - maxit (int): Maximum number of iterations. Default is 10000.
+        - verbose (bool): If True, prints iteration information. Default is True.
+        - mode (bool): If True, returns additional iteration information. Default is True.
+
+    :return: tuple
+        Tuple containing the root and optionally the number of iterations and norm of correction.
+        If mode is True, returns (root, iterations, norm_correction), otherwise just returns root.
+
+    Raises
+    ============
         ValueError: If the maximum number of iterations or tolerance is not a positive integer.
-    
-    Examples:
-    >>> # Example 1: Basic usage
-    >>> root, iterations, norm_correction = newton(2.0, lambda x: x**2 - 4, lambda x: 2 * x, verbose=True)
-    >>> print("Root:", root, "Iterations:", iterations, "Norm of correction:", norm_correction)
-        
-    >>> # Example 2: Usage with kwargs provided as a dictionary
-    >>> kwargs = {'verbose': True, 'tol': 1e-6, 'maxit': 20}
-    >>> root, iterations, norm_correction = newton(3.0, lambda x: x**3 - 27, lambda x: 3 * x**2, **kwargs)
-    >>> print("Root:", root, "Iterations:", iterations, "Norm of correction:", norm_correction)
+
+    Examples
+    ============
+        Example 1: Basic usage
+        >>> root, iterations, norm_correction = newton(2.0, lambda x: x**2 - 4, lambda x: 2 * x, verbose=True)
+        >>> print("Root:", root, "Iterations:", iterations, "Norm of correction:", norm_correction)
+        
+        Example 2: Usage with kwargs provided as a dictionary
+        >>> kwargs = {'verbose': True, 'tol': 1e-6, 'maxit': 20}
+        >>> root, iterations, norm_correction = newton(3.0, lambda x: x**3 - 27, lambda x: 3 * x**2, **kwargs)
+        >>> print("Root:", root, "Iterations:", iterations, "Norm of correction:", norm_correction)
     """
-    interface_opts, params_opts = opts(**kwargs)
-    verbose = interface_opts['verbose']
-    mode = interface_opts['mode']
-    tol = params_opts['tol']
-    maxit = int(params_opts['maxit'])
+    _opts = bs.opts(**kwargs)
+    verbose = _opts['verbose']
+    mode = _opts['mode']
+    tol = _opts['tol']
+    maxit = int(_opts['maxit'])
+    stop = _opts['stop']
     
     if maxit <= 0 or not isinstance(maxit, int):
         raise ValueError("Maximum number of iterations 'maxit' must be a positive integer.")
     if tol <= 0:
         raise ValueError("Tolerance 'tol' must be a positive value.")
+    
+    if verbose:
+        print('------ Newton Method summary ------')
+        print(f'tollerence: {tol}')
+        print(f'maximum iter: {maxit}')
+        print(f'stopping criteria: {stop}')
+        print(f'starting guess: {x}')
+    
+        print('------ Start iteration ------')
 
     for iter in range(maxit):
         f_value = f(x)
         df_value = df(x)
         
         if sp.issparse(df_value) and sp.issparse(df_value):
             dx = sp.linalg.spsolve(df_value, -f_value)
@@ -77,28 +83,28 @@
             dx = np.linalg.solve(df_value, -f_value)
             dxnorm = np.linalg.norm(dx)
             fnorm = np.linalg.norm(f_value)
         
         x += dx
         
         if sp.issparse(df_value) and sp.issparse(df_value):
-            fnorm = sp.linalg.norm(f(x))
+            fnorm = sp.linalg.norm(df(x)-f(x))
         else:
-            fnorm = np.linalg.norm(f(x))
+            fnorm = np.linalg.norm(df(x) - f(x))
         
-        if (fnorm < tol and (verbose or kwargs.get('residual_check', 'F') == 'F')):
+        if (fnorm < tol and stop == 'residual-check'):
             if verbose:
                 print(f'Newton converged in {iter + 1} iterations with ||F|| = {fnorm}')
-            return (x, iter + 1, dxnorm) if mode else x
+            return x, dxnorm if mode else x
         
-        if (dxnorm < tol and (verbose or kwargs.get('residual_check', 'F') != 'F')):
+        if (dxnorm < tol and stop == 'normal'):
             if verbose:
                 print(f'Newton converged in {iter + 1} iterations with ||dx|| = {dxnorm}')
-            return (x, iter + 1, dxnorm) if mode else x
+            return x, dxnorm if mode else x
         
         if verbose:
             print(f'Newton status at iteration {iter + 1}: ||F|| = {fnorm}, ||dx|| = {dxnorm}')
 
     if verbose:
         print(f'Newton did not converge within {maxit} iterations')
 
-    return (x, dxnorm) if mode else x
+    return x, dxnorm if mode else x
```

### Comparing `byma-0.0.25/byma/iteral/stationary/OrthogonalSubspace.py` & `byma-0.1.0/byma/iteral/stationary/OrthogonalSubspace.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,102 +1,92 @@
 import numpy as np
 from scipy.linalg import lu, inv, solve
 from numpy.linalg import qr
-
-from interface.BaseInterface import BaseInterface
+from ...interface.BaseInterface import BaseInterface as bs
 from .Stationary import Stationary as St
 
-def opts(interface={}, parameters={}, **kwargs):
-    """
-    Options handler for OSIM function.
-
-    Keyword Arguments:
-    interface (dict): Dictionary containing interface options.
-    parameters (dict): Dictionary containing parameter options.
-
-    Returns:
-    dict: Interface options.
-    dict: Parameter options.
-    """
-    params = {
+_DEFAULT_OPTS = {
         'stop': 'matrix',
         'maxit': 1e4,
         'tol': 1e-8,
-        'method': 'standard'  # Default linear system solving method
-    }
-    intf = {
+        'method': 'standard',
         'verbose': True,
     }
-    parameters.update(params)
-    interface.update(intf)
-
-    base_interface = BaseInterface(default_cls=St, params=parameters, interface=interface)
-    interface_opts, params_opts = base_interface.opts(**kwargs)
 
-    return interface_opts, params_opts
 
     
-def Z(V, A = None, P=None, L=None, U=None, method = 'standard'):
+def _Z(V, A = None, P=None, L=None, U=None, method = 'standard'):
     if method == 'LU':
         y = solve(inv(U), P.dot(V))
         z = solve(inv(L), y)
     else:
         z = A @ V
     return z
 
+@bs.set_defaults(default_cls = St, default_opts=_DEFAULT_OPTS)
 def osim(A, V, **kwargs):
     """
     Orthogonal Subspace Iteration Method (OSIM).
 
     Args:
-    A (numpy.ndarray): The matrix to compute the eigenvalues and eigenvectors for.
-    V (numpy.ndarray): Initial guess of eigenvectors.
+    A : numpy.ndarray
+        The matrix to compute the eigenvalues and eigenvectors for.
+    V : numpy.ndarray
+        Initial guess of eigenvectors.
 
     Keyword Arguments:
-    tol (float): Tolerance for convergence (default: 1e-6).
-    maxit (int): Maximum number of iterations (default: 100).
-    stop (str): Stopping criteria for convergence. Options are 'eig' (default), 'matrix', or 'residual'.
-    method (str): Method for solving linear systems. Options are 'LU' (default) or any method supported by scipy.linalg.lu.
+        tol : float, optional
+            Tolerance for convergence (default: 1e-8).
+        maxit : int, optional
+            Maximum number of iterations (default: 100).
+        stop : str, optional
+            Stopping criteria for convergence. Options are 'eig' (default), 'matrix', or 'residual'.
+        method : str, optional
+            Method for solving linear systems. Options are 'LU' (default) or any method supported by scipy.linalg.lu.
+        verbose : bool, optional
+            If True, prints iteration information (default: True).
 
     Returns:
-    numpy.ndarray: Matrix of eigenvectors.
-    numpy.ndarray: Matrix of transformed eigenvectors.
-    tuple: Tuple containing eigenvalues at each iteration.
+    numpy.ndarray
+        Matrix of eigenvectors.
+    numpy.ndarray
+        Matrix of transformed eigenvectors.
+    tuple
+        Tuple containing eigenvalues at each iteration.
 
     Notes:
-    This function implements the Orthogonal Subspace Iteration Method (OSIM) to
-    compute eigenvectors and eigenvalues of a matrix A.
+    This function implements the Orthogonal Subspace Iteration Method (OSIM) to compute eigenvectors and eigenvalues of a matrix A.
 
     Examples:
     >>> import numpy as np
     >>> from iteral import stationary as st
     >>> A = np.array([[1, 0], [0, 1]])
     >>> V = np.array([[1], [0]])
     >>> V, BV, iter = st.osim(A, V, tol=1e-8, maxit=1000, stop='eig', method='LU')
 
     You can also pass keyword arguments using a dictionary. For example:
     >>> kwargs = {'tol': 1e-8, 'maxit': 1000, 'stop': 'eig', 'method': 'LU'}
     >>> V, BV, iter = osim(A, V, **kwargs)
-    
+
     You can also pass keyword arguments using two separate dictionaries for parameters and interface. For example:
     >>> parameters = {'tol': 1e-8, 'maxit': 1000, 'stop': 'eig', 'method': 'LU'}
     >>> interface = {'verbose': True}
     >>> V, BV, iter = st.osim(A, V, parameters=parameters, interface=interface)
     """
     
     # Check if the number of rows of V matches the number of columns of A
     if V.shape[0] != A.shape[1]:
         raise ValueError("Number of rows of V must match the number of columns of A.")
     
-    interface, parameters = opts(**kwargs)
-    verbose = interface['verbose']
-    tol = parameters['tol']
-    maxit = int(parameters['maxit'])
-    stop = parameters['stop']
-    method = parameters['method']
+    _opts = bs.opts(**kwargs)
+    verbose = _opts['verbose']
+    tol = _opts['tol']
+    maxit = int(_opts['maxit'])
+    stop = _opts['stop']
+    method = _opts['method']
     
     if verbose:
         print('------ OSIM initialization summary ------')
         print(f'tollerence: {tol}')
         print(f'maximum iter: {maxit}')
         print(f'stopping criteria: {stop}')
         print(f'Linear system solving method: {method}')
@@ -104,19 +94,19 @@
         print('------ Start iteration ------')
     
     if method == 'LU':
         P, L, U = lu(A.toarray())
     else:
         P = L = U = None
 
-    B = lambda V: V.T @ Z(V = V, A = A, P = P, L = L, U = U, method = method)
+    B = lambda V: V.T @ _Z(V = V, A = A, P = P, L = L, U = U, method = method)
 
     iter = []
     for n in range(maxit):
-        Zn = Z(V = V, A = A, P = P, L = L, U = U, method = method)
+        Zn = _Z(V = V, A = A, P = P, L = L, U = U, method = method)
         BV = B(V = V)
         eig = np.diag(BV)
         if verbose != False: 
             if (n % verbose == 0):
                 print(f"Eigenvalues at n = {n}: {eig}")
         else:
             if (n % 5000 == 0):
```

### Comparing `byma-0.0.25/byma/nuby/Continuation.py` & `byma-0.1.0/byma/nuby/Continuation.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,49 +1,43 @@
 import numpy as np
 import scipy.sparse as sp
 from ..iteral.nonstationary import newton
-from ..interface.BaseInterface import BaseInterface
+from ..interface.BaseInterface import BaseInterface as bs
 from .Bifurcation import Bifurcation as Bf
 
-def opts(interface={}, parameters={}, **kwargs):
-    params = {
-        'stop': 'matrix',
-        'maxit': 1e4,
-        'tol': 1e-8,
-        'method': 'standard'  # Default linear system solving method
+_DEFAULT_OPTS = {
+    'maxit_cont' : 1000,
+    'verbose': True,
+    'mode': None, 
+    'method': 'normal',
     }
-    intf = {
-        'verbose': True,
-    }
-    parameters.update(params)
-    interface.update(intf)
-
-    base_interface = BaseInterface(default_cls=Bf, params=parameters, interface=interface)
-    interface_opts, params_opts = base_interface.opts(**kwargs)
 
-    return interface_opts, params_opts
 
 def step(x, df, dfmu, dx, dmu, **kwargs):
         """
     Perform one step of the continuation.
 
-    Parameters:
-        x (array_like): Current state.
-        df (callable): Function to evaluate the Jacobian matrix with respect to state variable x.
-        dfmu (callable): Function to evaluate the Jacobian matrix derivative with respect to parameter mu.
-        dx (array_like): Current tangent with respect to state variable.
-        dmu (float or array_like): Incremental change in the parameter value.
-        **kwargs: Additional keyword arguments.
+    :param x: array_like
+        Current state.
+    :param df: callable
+        Function to evaluate the Jacobian matrix with respect to state variable x.
+    :param dfmu: callable
+        Function to evaluate the Jacobian matrix derivative with respect to parameter mu.
+    :param dx: array_like
+        Current tangent with respect to state variable.
+    :param dmu: float or array_like
+        Incremental change in the parameter value.
+    :param kwargs: dict
+        Additional keyword arguments.
 
-    Returns:
-        tuple: A tuple containing the updated state x and the norm of the correction.
+    :return: tuple
+        A tuple containing the updated state x and the norm of the correction.
 
-    Description:
+    :description:
     This function performs one step of the continuation, updating the state variable x and the tangent dx using the provided functions for evaluating the Jacobian matrix and its derivative with respect to the parameter.
-
     """
         
         # Predictor
         x += dmu * dx
         kwargs.update({'mode' : True})
         
         # Corrector 
@@ -54,128 +48,134 @@
         dfmu1 = dfmu(x)
         if sp.issparse(dfx1) and sp.issparse(dfmu1):
             dx = sp.linalg.spsolve(dfx1, -dfmu1)
             
         else:
             dx = np.linalg.solve(dfx1, -dfmu1)
             
-        if abs(dx) < 1e-12:
-            raise Exception('dx too small')
-
-        
         return x, dxnorm
 
+@bs.set_defaults(default_cls = Bf, default_opts=_DEFAULT_OPTS)
 def cont(x0, dx0, start, df, dfmu, dmu=None, target=None, **kwargs):
     """
     Perform a continuation in parameter value from a starting value to a target value or until the maximum iteration is met, with constant step size.
 
     This function performs a continuation in parameter space from a starting value to a target value, or until the maximum iteration is met, adjusting the state variable x along the way. The continuation is carried out using the provided functions for evaluating the Jacobian matrix and its derivative with respect to the parameter.
 
-    Parameters
-    ----------
-        x0 : array_like
-            Initial state.
-        dx0 : array_like
-            Initial tangent with respect to state variable.
-        start : float
-            Starting parameter value.
-        df : callable
-            Function to evaluate the Jacobian matrix with respect to state variable x and parameter mu.
-        dfmu : callable
-            Function to evaluate the Jacobian matrix derivative with respect to parameter mu.
-        dmu : float or array_like, optional
-            Incremental change in the parameter value for each iteration. If None and target is None, raises ValueError.
-        target : float or None, optional
-            Target parameter value. If None, continuation is performed until maxit_con iterations.
-        **kwargs : dict
-            Additional keyword arguments for customization.
+    :param x0: array_like
+        Initial state.
+    :param dx0: array_like
+        Initial tangent with respect to state variable.
+    :param start: float
+        Starting parameter value.
+    :param df: callable
+        Function to evaluate the Jacobian matrix with respect to state variable x and parameter mu.
+    :param dfmu: callable
+        Function to evaluate the Jacobian matrix derivative with respect to parameter mu.
+    :param dmu: float or array_like, optional
+        Incremental change in the parameter value for each iteration. If None and target is None, raises ValueError.
+    :param target: float or None, optional
+        Target parameter value. If None, continuation is performed until maxit_con iterations.
+    :param kwargs: dict
+        Additional keyword arguments for customization.
             maxit_con : int, optional
                 Maximum number of continuation steps. Default is 1000.
             method : str, optional
                 Continuation method ('normal' or 'pseudo-arclength'). Default is 'normal'.
             mode : str, optional
                 Return mode ('partial' or 'full'). Default is 'partial'.
             Other keyword arguments : Additional parameters specific to the step function used internally.
 
-    Returns
-    -------
-        tuple or array_like
-            Depending on the mode specified in kwargs, returns either a tuple or an array.
+    :return: tuple or array_like
+        Depending on the mode specified in kwargs, returns either a tuple or an array.
             - In 'partial' mode, returns a tuple containing the final state x and the final parameter value mu.
             - In 'full' mode, returns an array containing all the states x, an array of the norm of the correction at each step, and the final parameter value mu (if target is None).
 
-    Raises
-    ------
-        ValueError
-            If either 'dmu' or 'target' should be not 'None' but are not provided.
-        ValueError
-            If the provided continuation method is invalid. Choose either 'normal' or 'pseudo-arclength'.
+    :raises:
+        ValueError: If either 'dmu' or 'target' should be not 'None' but are not provided.
+        ValueError: If the provided continuation method is invalid. Choose either 'normal' or 'pseudo-arclength'.
 
     Examples
-    --------
-    >>> # Define the functions df and dfmu
-    >>> def df(x, mu0):
-    >>>     # Compute the Jacobian matrix with respect to state variable x and parameter mu
-    >>>     pass
-    >>> def dfmu(x, mu0):
-    >>>     # Compute the Jacobian matrix derivative with respect to parameter mu
-    >>>     pass
-    >>> 
-    >>> # Define the initial state and tangent
-    >>> x0 = np.array([1.0, 2.0])
-    >>> dx0 = np.array([0.1, 0.1])
-    >>> 
-    >>> # Perform continuation from start value to target value
-    >>> start = 0.0
-    >>> target = 1.0
-    >>> result = cont(x0, dx0, start, df, dfmu, target=target, maxit_con=1000, method='normal', mode='full')
-    >>> print(result)
+    =============
+        >>> # Define the functions df and dfmu
+        >>> def df(x, mu0):
+        >>>     # Compute the Jacobian matrix with respect to state variable x and parameter mu
+        >>>     pass
+        >>> def dfmu(x, mu0):
+        >>>     # Compute the Jacobian matrix derivative with respect to parameter mu
+        >>>     pass
+        >>> 
+        >>> # Define the initial state and tangent
+        >>> x0 = np.array([1.0, 2.0])
+        >>> dx0 = np.array([0.1, 0.1])
+        >>> 
+        >>> # Perform continuation from start value to target value
+        >>> start = 0.0
+        >>> target = 1.0
+        >>> result = cont(x0, dx0, start, df, dfmu, target=target, maxit_con=1000, method='normal', mode='full')
+        >>> print(result)
     """
-    interface_opts, params_opts = opts(**kwargs)
-    verbose = interface_opts['verbose']
-    mode = interface_opts['mode']
-    method = interface_opts['method']
-    maxit_con = params_opts['maxit_cont']
+    _opts = bs.opts(**kwargs)
+    mode_con = _opts['mode']
+    method = _opts['method']
+    maxit_con = _opts['maxit_cont']
+    verbose = _opts['verbose']
     
     x = x0
     dx = dx0
     mu = start
 
     # Set some parameters
-    if target is None:
-        maxit = maxit_con
-        if dmu is None:
-            raise ValueError("Either 'dmu' or 'target' should be not 'None'")
+    if (target is None) and (dmu is None):
+        raise ValueError("Either 'dmu' or 'target' should be not 'None'")
+    
     else:
         mus = np.linspace(mu, target, maxit_con)
         
     # Perform the continuation
     branch = []
     dxnorms = []
+    
+    if verbose:
+        print('------ Continuation Method summary ------')
+        print(f'starting solution: {x0}')
+        print(f'starting parameter: {start}')
+        print(f'maximum iter: {maxit_con}')
+        print(f'method: {method}')
+    
+        print('------ Start iteration ------')
 
-    for j in range(maxit):
+    for j in range(maxit_con):
         
         if target is None:
             mu0 = mu0 + dmu if isinstance(dmu, float) else mu0 + dmu[j]
         else:
             mu0 = mus[j]
             dmu = mu - mu0 if mu != start else mu0 - mus[j]
 
-        df = lambda x: df(x = x, mu0 = mu0)
-        dfmu = lambda x: dfmu(x = x, mu0 = mu0)
+        df1 = lambda x: df(x = x, mu = mu0)
+        dfmu1 = lambda x: dfmu(x = x, mu = mu0)
         
         if method == 'normal':
-            x, dxnorm = step(x, df, dfmu, dx, dmu, **kwargs)
+            x, dxnorm = step(x, df=df1, dfmu=dfmu1, dx=dx, dmu=dmu, **kwargs)
         elif method == 'pseudo-arclength':
             raise ValueError("Pseudo-arclength'conitnuation is not yet avialible")
         else:
             raise ValueError("Invalid continuation method. Choose either 'normal' or 'pseudo-arclength'.")
 
         branch.append(x)
         dxnorms.append(dxnorm)
 
-    if mode == 'partial':
-        return branch, mu0 if target is None else branch
-    elif mode == 'full':
-        return branch, dxnorms, mu0 if target is None else branch, dxnorms
+    if target == None:
+        if mode_con == 'full':
+            return branch, dxnorms, mu0 
+        elif mode_con == 'partial':
+            return branch, mu0
+        else:
+            return x, mu0
     else:
-        return x, mu0 if target is None else x
+        if mode_con == 'full':
+            return branch, dxnorms
+        elif mode_con == 'partial':
+            return branch
+        else:
+            return x
```

### Comparing `byma-0.0.25/byma.egg-info/PKG-INFO` & `byma-0.1.0/byma.egg-info/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,23 +1,33 @@
 Metadata-Version: 2.1
 Name: byma
-Version: 0.0.25
+Version: 0.1.0
 Summary: A Numerical Mathematics Packages with an easier and clean user interface.
 Author: @b64-Lorenzo (Lorenzo Zambelli)
 Author-email: Lorenzo Zambelli <bytemath@lorenzozambelli.it>
 Project-URL: Homepage, https://gitlab.com/ByteMath/python/byma
 Keywords: python,scientific,numerical,bifurcation
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 
 # ByMa
+![PyPI - Version](https://img.shields.io/pypi/v/byma?style=plastic&label=ByMa&labelColor=green&color=blue&link=https%3A%2F%2Fbytemath.gitlab.io%2Fpython%2FByMa%2Findex.html)
+[![PyPI Downloads](https://img.shields.io/pypi/dm/label=PyPI%20downloads)](
+https://pypi.org/project/byma/)
+[![Conda Downloads](https://img.shields.io/conda/dn/conda-forge/label=Conda%20downloads)](https://anaconda.org/conda-forge/byma)
+![Libraries.io dependency status for specific release](https://img.shields.io/librariesio/release/pypi/numpy/1.1.1?style=plastic&logo=numpy&label=NumPy&labelColor=blue&link=https%3A%2F%2Fnumpy.org%2F)
+![Libraries.io dependency status for specific release](https://img.shields.io/librariesio/release/pypi/scipy/1.0.0?style=plastic&logo=scipy&label=SciPy&labelColor=light%20blue&link=https%3A%2F%2Fscipy.org%2F)
+![GitLab Last Commit](https://img.shields.io/gitlab/last-commit/ByteMath%2Fpython%2FByMa?gitlab_url=https%3A%2F%2Fgitlab.com%2FByteMath%2Fpython%2FByMa&style=plastic)
+![Static Badge](https://img.shields.io/badge/Docs-Read?style=plastic&label=Read&color=purple&link=https%3A%2F%2Fbytemath.gitlab.io%2Fpython%2FByMa%2Findex.html)
+
+
 
 ByMa is a Python package designed to facilitate numerical mathematics tasks by implementing a range of standard methods, from iterative techniques to bifurcation methods. Noted for its simplicity, clarity, and efficiency, ByMa aims to enhance the learning experience for newcomers to numerical mathematics while streamlining the implementation and utilization of popular scientific libraries such as NumPy, SciPy, and Matplotlib.
 
 
 ## Installation
 
 ByMa is best installed in a [virtual environment](https://docs.python.org/3/library/venv.html).
```

### Comparing `byma-0.0.25/byma.egg-info/SOURCES.txt` & `byma-0.1.0/byma.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -27,23 +27,25 @@
 byma/nuby/Continuation.py
 byma/nuby/__init__.py
 byma/nuby/_nuby.py
 byma/pyplot/__init__.py
 byma/pyplot/plots.py
 docs/Makefile
 docs/make.bat
+docs/requirements.txt
 docs/source/conf.py
 docs/source/index.rst
 docs/source/autoapi/index.rst
 docs/source/autoapi/byma/index.rst
 docs/source/autoapi/byma/_version/index.rst
 docs/source/autoapi/byma/interface/index.rst
 docs/source/autoapi/byma/interface/BaseInterface/index.rst
 docs/source/autoapi/byma/interface/NonlinearHeat/index.rst
 docs/source/autoapi/byma/iteral/index.rst
+docs/source/autoapi/byma/iteral/nonstationary/index.rst
 docs/source/autoapi/byma/iteral/nonstationary/Newton/index.rst
 docs/source/autoapi/byma/iteral/nonstationary/NonStationary/index.rst
 docs/source/autoapi/byma/iteral/stationary/index.rst
 docs/source/autoapi/byma/iteral/stationary/OrthogonalSubspace/index.rst
 docs/source/autoapi/byma/iteral/stationary/Stationary/index.rst
 docs/source/autoapi/byma/nuby/index.rst
 docs/source/autoapi/byma/nuby/Bifurcation/index.rst
```

### Comparing `byma-0.0.25/docs/Makefile` & `byma-0.1.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `byma-0.0.25/docs/make.bat` & `byma-0.1.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `byma-0.0.25/docs/source/autoapi/byma/index.rst` & `byma-0.1.0/docs/source/autoapi/byma/index.rst`

 * *Files identical despite different names*

### Comparing `byma-0.0.25/docs/source/autoapi/byma/iteral/nonstationary/Newton/index.rst` & `byma-0.1.0/docs/source/autoapi/byma/iteral/nonstationary/Newton/index.rst`

 * *Files 9% similar despite different names*

```diff
@@ -9,48 +9,48 @@
 
 
 Functions
 ~~~~~~~~~
 
 .. autoapisummary::
 
-   byma.iteral.nonstationary.Newton.opts
    byma.iteral.nonstationary.Newton.newton
 
 
 
-.. py:function:: opts(interface={}, parameters={}, **kwargs)
-
-
 .. py:function:: newton(x, f, df, **kwargs)
 
-   Newton iterations.
+   Perform Newton iterations to find the root of a given function.
 
-   Parameters:
-       x (array_like): Initial guess for the root.
-       f (callable): Function to evaluate the residuals.
-       df (callable): Function to evaluate the Jacobian matrix.
-       **kwargs: Additional keyword arguments for customization.
-           - tol (float): Tolerance for convergence. Default is 1e-8.
-           - maxit (int): Maximum number of iterations. Default is 10000.
-           - verbose (bool): If True, prints iteration information. Default is True.
-           - mode (bool): If True, returns additional iteration information. Default is True.
-
-
-   Returns:
-       tuple: Tuple containing the root and optionally the number of iterations and norm of correction.
-              If mode is True, returns (root, iterations, norm_correction), otherwise just returns root.
+   :param x: array_like
+       Initial guess for the root.
+   :param f: callable
+       Function to evaluate the residuals.
+   :param df: callable
+       Function to evaluate the Jacobian matrix.
+   :param kwargs: dict
+       Additional keyword arguments for customization.
+       - tol (float): Tolerance for convergence. Default is 1e-8.
+       - maxit (int): Maximum number of iterations. Default is 10000.
+       - verbose (bool): If True, prints iteration information. Default is True.
+       - mode (bool): If True, returns additional iteration information. Default is True.
+
+   :return: tuple
+       Tuple containing the root and optionally the number of iterations and norm of correction.
+       If mode is True, returns (root, iterations, norm_correction), otherwise just returns root.
 
-   Raises:
+   Raises
+   ============
        ValueError: If the maximum number of iterations or tolerance is not a positive integer.
 
-   Examples:
-   >>> # Example 1: Basic usage
-   >>> root, iterations, norm_correction = newton(2.0, lambda x: x**2 - 4, lambda x: 2 * x, verbose=True)
-   >>> print("Root:", root, "Iterations:", iterations, "Norm of correction:", norm_correction)
+   Examples
+   ============
+       Example 1: Basic usage
+       >>> root, iterations, norm_correction = newton(2.0, lambda x: x**2 - 4, lambda x: 2 * x, verbose=True)
+       >>> print("Root:", root, "Iterations:", iterations, "Norm of correction:", norm_correction)
        
-   >>> # Example 2: Usage with kwargs provided as a dictionary
-   >>> kwargs = {'verbose': True, 'tol': 1e-6, 'maxit': 20}
-   >>> root, iterations, norm_correction = newton(3.0, lambda x: x**3 - 27, lambda x: 3 * x**2, **kwargs)
-   >>> print("Root:", root, "Iterations:", iterations, "Norm of correction:", norm_correction)
+       Example 2: Usage with kwargs provided as a dictionary
+       >>> kwargs = {'verbose': True, 'tol': 1e-6, 'maxit': 20}
+       >>> root, iterations, norm_correction = newton(3.0, lambda x: x**3 - 27, lambda x: 3 * x**2, **kwargs)
+       >>> print("Root:", root, "Iterations:", iterations, "Norm of correction:", norm_correction)
```

### Comparing `byma-0.0.25/docs/source/autoapi/byma/iteral/stationary/OrthogonalSubspace/index.rst` & `byma-0.1.0/docs/source/autoapi/byma/iteral/stationary/OrthogonalSubspace/index.rst`

 * *Files 14% similar despite different names*

```diff
@@ -9,58 +9,50 @@
 
 
 Functions
 ~~~~~~~~~
 
 .. autoapisummary::
 
-   byma.iteral.stationary.OrthogonalSubspace.opts
-   byma.iteral.stationary.OrthogonalSubspace.Z
    byma.iteral.stationary.OrthogonalSubspace.osim
 
 
 
-.. py:function:: opts(interface={}, parameters={}, **kwargs)
-
-   Options handler for OSIM function.
-
-   Keyword Arguments:
-   interface (dict): Dictionary containing interface options.
-   parameters (dict): Dictionary containing parameter options.
-
-   Returns:
-   dict: Interface options.
-   dict: Parameter options.
-
-
-.. py:function:: Z(V, A=None, P=None, L=None, U=None, method='standard')
-
-
 .. py:function:: osim(A, V, **kwargs)
 
    Orthogonal Subspace Iteration Method (OSIM).
 
    Args:
-   A (numpy.ndarray): The matrix to compute the eigenvalues and eigenvectors for.
-   V (numpy.ndarray): Initial guess of eigenvectors.
+   A : numpy.ndarray
+       The matrix to compute the eigenvalues and eigenvectors for.
+   V : numpy.ndarray
+       Initial guess of eigenvectors.
 
    Keyword Arguments:
-   tol (float): Tolerance for convergence (default: 1e-6).
-   maxit (int): Maximum number of iterations (default: 100).
-   stop (str): Stopping criteria for convergence. Options are 'eig' (default), 'matrix', or 'residual'.
-   method (str): Method for solving linear systems. Options are 'LU' (default) or any method supported by scipy.linalg.lu.
+       tol : float, optional
+           Tolerance for convergence (default: 1e-8).
+       maxit : int, optional
+           Maximum number of iterations (default: 100).
+       stop : str, optional
+           Stopping criteria for convergence. Options are 'eig' (default), 'matrix', or 'residual'.
+       method : str, optional
+           Method for solving linear systems. Options are 'LU' (default) or any method supported by scipy.linalg.lu.
+       verbose : bool, optional
+           If True, prints iteration information (default: True).
 
    Returns:
-   numpy.ndarray: Matrix of eigenvectors.
-   numpy.ndarray: Matrix of transformed eigenvectors.
-   tuple: Tuple containing eigenvalues at each iteration.
+   numpy.ndarray
+       Matrix of eigenvectors.
+   numpy.ndarray
+       Matrix of transformed eigenvectors.
+   tuple
+       Tuple containing eigenvalues at each iteration.
 
    Notes:
-   This function implements the Orthogonal Subspace Iteration Method (OSIM) to
-   compute eigenvectors and eigenvalues of a matrix A.
+   This function implements the Orthogonal Subspace Iteration Method (OSIM) to compute eigenvectors and eigenvalues of a matrix A.
 
    Examples:
    >>> import numpy as np
    >>> from iteral import stationary as st
    >>> A = np.array([[1, 0], [0, 1]])
    >>> V = np.array([[1], [0]])
    >>> V, BV, iter = st.osim(A, V, tol=1e-8, maxit=1000, stop='eig', method='LU')
```

### Comparing `byma-0.0.25/docs/source/autoapi/byma/nuby/Continuation/index.rst` & `byma-0.1.0/docs/source/autoapi/byma/nuby/index.rst`

 * *Files 10% similar despite different names*

```diff
@@ -1,111 +1,151 @@
-:py:mod:`byma.nuby.Continuation`
-================================
+:py:mod:`byma.nuby`
+===================
 
-.. py:module:: byma.nuby.Continuation
+.. py:module:: byma.nuby
 
+.. autoapi-nested-parse::
 
-Module Contents
----------------
+   ``byma.nuby``
+   ================
 
+   The ByMa numerical bifurcation functions rely on 
 
-Functions
-~~~~~~~~~
+   Functions present in byma.nuby are listed below.
+
+
+   Continuation
+   --------------------------
+
+      step
+      cont
+      
+
+   Exceptions
+   ----------
+
+      NuByError
+
+
+
+Submodules
+----------
+.. toctree::
+   :titlesonly:
+   :maxdepth: 1
+
+   Bifurcation/index.rst
+   Continuation/index.rst
+
+
+Package Contents
+----------------
+
+Classes
+~~~~~~~
 
 .. autoapisummary::
 
-   byma.nuby.Continuation.opts
-   byma.nuby.Continuation.step
-   byma.nuby.Continuation.cont
+   byma.nuby.Bifurcation
+
 
 
+Functions
+~~~~~~~~~
+
+.. autoapisummary::
+
+   byma.nuby.step
+   byma.nuby.cont
 
-.. py:function:: opts(interface={}, parameters={}, **kwargs)
 
 
 .. py:function:: step(x, df, dfmu, dx, dmu, **kwargs)
 
    Perform one step of the continuation.
 
-   Parameters:
-       x (array_like): Current state.
-       df (callable): Function to evaluate the Jacobian matrix with respect to state variable x.
-       dfmu (callable): Function to evaluate the Jacobian matrix derivative with respect to parameter mu.
-       dx (array_like): Current tangent with respect to state variable.
-       dmu (float or array_like): Incremental change in the parameter value.
-       **kwargs: Additional keyword arguments.
+   :param x: array_like
+       Current state.
+   :param df: callable
+       Function to evaluate the Jacobian matrix with respect to state variable x.
+   :param dfmu: callable
+       Function to evaluate the Jacobian matrix derivative with respect to parameter mu.
+   :param dx: array_like
+       Current tangent with respect to state variable.
+   :param dmu: float or array_like
+       Incremental change in the parameter value.
+   :param kwargs: dict
+       Additional keyword arguments.
 
-   Returns:
-       tuple: A tuple containing the updated state x and the norm of the correction.
+   :return: tuple
+       A tuple containing the updated state x and the norm of the correction.
 
-   Description:
+   :description:
    This function performs one step of the continuation, updating the state variable x and the tangent dx using the provided functions for evaluating the Jacobian matrix and its derivative with respect to the parameter.
 
 
-
 .. py:function:: cont(x0, dx0, start, df, dfmu, dmu=None, target=None, **kwargs)
 
    Perform a continuation in parameter value from a starting value to a target value or until the maximum iteration is met, with constant step size.
 
    This function performs a continuation in parameter space from a starting value to a target value, or until the maximum iteration is met, adjusting the state variable x along the way. The continuation is carried out using the provided functions for evaluating the Jacobian matrix and its derivative with respect to the parameter.
 
-   Parameters
-   ----------
-       x0 : array_like
-           Initial state.
-       dx0 : array_like
-           Initial tangent with respect to state variable.
-       start : float
-           Starting parameter value.
-       df : callable
-           Function to evaluate the Jacobian matrix with respect to state variable x and parameter mu.
-       dfmu : callable
-           Function to evaluate the Jacobian matrix derivative with respect to parameter mu.
-       dmu : float or array_like, optional
-           Incremental change in the parameter value for each iteration. If None and target is None, raises ValueError.
-       target : float or None, optional
-           Target parameter value. If None, continuation is performed until maxit_con iterations.
-       **kwargs : dict
-           Additional keyword arguments for customization.
+   :param x0: array_like
+       Initial state.
+   :param dx0: array_like
+       Initial tangent with respect to state variable.
+   :param start: float
+       Starting parameter value.
+   :param df: callable
+       Function to evaluate the Jacobian matrix with respect to state variable x and parameter mu.
+   :param dfmu: callable
+       Function to evaluate the Jacobian matrix derivative with respect to parameter mu.
+   :param dmu: float or array_like, optional
+       Incremental change in the parameter value for each iteration. If None and target is None, raises ValueError.
+   :param target: float or None, optional
+       Target parameter value. If None, continuation is performed until maxit_con iterations.
+   :param kwargs: dict
+       Additional keyword arguments for customization.
            maxit_con : int, optional
                Maximum number of continuation steps. Default is 1000.
            method : str, optional
                Continuation method ('normal' or 'pseudo-arclength'). Default is 'normal'.
            mode : str, optional
                Return mode ('partial' or 'full'). Default is 'partial'.
            Other keyword arguments : Additional parameters specific to the step function used internally.
 
-   Returns
-   -------
-       tuple or array_like
-           Depending on the mode specified in kwargs, returns either a tuple or an array.
+   :return: tuple or array_like
+       Depending on the mode specified in kwargs, returns either a tuple or an array.
            - In 'partial' mode, returns a tuple containing the final state x and the final parameter value mu.
            - In 'full' mode, returns an array containing all the states x, an array of the norm of the correction at each step, and the final parameter value mu (if target is None).
 
-   Raises
-   ------
-       ValueError
-           If either 'dmu' or 'target' should be not 'None' but are not provided.
-       ValueError
-           If the provided continuation method is invalid. Choose either 'normal' or 'pseudo-arclength'.
+   :raises:
+       ValueError: If either 'dmu' or 'target' should be not 'None' but are not provided.
+       ValueError: If the provided continuation method is invalid. Choose either 'normal' or 'pseudo-arclength'.
 
    Examples
-   --------
-   >>> # Define the functions df and dfmu
-   >>> def df(x, mu0):
-   >>>     # Compute the Jacobian matrix with respect to state variable x and parameter mu
-   >>>     pass
-   >>> def dfmu(x, mu0):
-   >>>     # Compute the Jacobian matrix derivative with respect to parameter mu
-   >>>     pass
-   >>> 
-   >>> # Define the initial state and tangent
-   >>> x0 = np.array([1.0, 2.0])
-   >>> dx0 = np.array([0.1, 0.1])
-   >>> 
-   >>> # Perform continuation from start value to target value
-   >>> start = 0.0
-   >>> target = 1.0
-   >>> result = cont(x0, dx0, start, df, dfmu, target=target, maxit_con=1000, method='normal', mode='full')
-   >>> print(result)
+   =============
+       >>> # Define the functions df and dfmu
+       >>> def df(x, mu0):
+       >>>     # Compute the Jacobian matrix with respect to state variable x and parameter mu
+       >>>     pass
+       >>> def dfmu(x, mu0):
+       >>>     # Compute the Jacobian matrix derivative with respect to parameter mu
+       >>>     pass
+       >>> 
+       >>> # Define the initial state and tangent
+       >>> x0 = np.array([1.0, 2.0])
+       >>> dx0 = np.array([0.1, 0.1])
+       >>> 
+       >>> # Perform continuation from start value to target value
+       >>> start = 0.0
+       >>> target = 1.0
+       >>> result = cont(x0, dx0, start, df, dfmu, target=target, maxit_con=1000, method='normal', mode='full')
+       >>> print(result)
+
+
+.. py:class:: Bifurcation
+
+
+   Defines default options for the Bifurcation package
```

### Comparing `byma-0.0.25/docs/source/autoapi/byma/nuby/index.rst` & `byma-0.1.0/docs/source/autoapi/byma/nuby/_nuby/index.rst`

 * *Files 14% similar despite different names*

```diff
@@ -1,158 +1,127 @@
-:py:mod:`byma.nuby`
-===================
+:orphan:
 
-.. py:module:: byma.nuby
-
-.. autoapi-nested-parse::
-
-   ``byma.nuby``
-   ================
-
-   The ByMa numerical bifurcation functions rely on 
-
-   Functions present in byma.nuby are listed below.
-
-
-   Continuation
-   --------------------------
-
-      step
-      cont
-      
-
-   Exceptions
-   ----------
-
-      NuByError
+:py:mod:`byma.nuby._nuby`
+=========================
 
+.. py:module:: byma.nuby._nuby
 
+.. autoapi-nested-parse::
 
-Submodules
-----------
-.. toctree::
-   :titlesonly:
-   :maxdepth: 1
+   Notes
+   -----
+   This module is has basic bifurcation analysis tools
 
-   Bifurcation/index.rst
-   Continuation/index.rst
 
 
-Package Contents
-----------------
+Module Contents
+---------------
 
 Classes
 ~~~~~~~
 
 .. autoapisummary::
 
-   byma.nuby.Bifurcation
+   byma.nuby._nuby.Bifurcation
 
 
 
 Functions
 ~~~~~~~~~
 
 .. autoapisummary::
 
-   byma.nuby.step
-   byma.nuby.cont
-   byma.nuby.opts
+   byma.nuby._nuby.step
+   byma.nuby._nuby.cont
 
 
 
 .. py:function:: step(x, df, dfmu, dx, dmu, **kwargs)
 
    Perform one step of the continuation.
 
-   Parameters:
-       x (array_like): Current state.
-       df (callable): Function to evaluate the Jacobian matrix with respect to state variable x.
-       dfmu (callable): Function to evaluate the Jacobian matrix derivative with respect to parameter mu.
-       dx (array_like): Current tangent with respect to state variable.
-       dmu (float or array_like): Incremental change in the parameter value.
-       **kwargs: Additional keyword arguments.
+   :param x: array_like
+       Current state.
+   :param df: callable
+       Function to evaluate the Jacobian matrix with respect to state variable x.
+   :param dfmu: callable
+       Function to evaluate the Jacobian matrix derivative with respect to parameter mu.
+   :param dx: array_like
+       Current tangent with respect to state variable.
+   :param dmu: float or array_like
+       Incremental change in the parameter value.
+   :param kwargs: dict
+       Additional keyword arguments.
 
-   Returns:
-       tuple: A tuple containing the updated state x and the norm of the correction.
+   :return: tuple
+       A tuple containing the updated state x and the norm of the correction.
 
-   Description:
+   :description:
    This function performs one step of the continuation, updating the state variable x and the tangent dx using the provided functions for evaluating the Jacobian matrix and its derivative with respect to the parameter.
 
 
-
 .. py:function:: cont(x0, dx0, start, df, dfmu, dmu=None, target=None, **kwargs)
 
    Perform a continuation in parameter value from a starting value to a target value or until the maximum iteration is met, with constant step size.
 
    This function performs a continuation in parameter space from a starting value to a target value, or until the maximum iteration is met, adjusting the state variable x along the way. The continuation is carried out using the provided functions for evaluating the Jacobian matrix and its derivative with respect to the parameter.
 
-   Parameters
-   ----------
-       x0 : array_like
-           Initial state.
-       dx0 : array_like
-           Initial tangent with respect to state variable.
-       start : float
-           Starting parameter value.
-       df : callable
-           Function to evaluate the Jacobian matrix with respect to state variable x and parameter mu.
-       dfmu : callable
-           Function to evaluate the Jacobian matrix derivative with respect to parameter mu.
-       dmu : float or array_like, optional
-           Incremental change in the parameter value for each iteration. If None and target is None, raises ValueError.
-       target : float or None, optional
-           Target parameter value. If None, continuation is performed until maxit_con iterations.
-       **kwargs : dict
-           Additional keyword arguments for customization.
+   :param x0: array_like
+       Initial state.
+   :param dx0: array_like
+       Initial tangent with respect to state variable.
+   :param start: float
+       Starting parameter value.
+   :param df: callable
+       Function to evaluate the Jacobian matrix with respect to state variable x and parameter mu.
+   :param dfmu: callable
+       Function to evaluate the Jacobian matrix derivative with respect to parameter mu.
+   :param dmu: float or array_like, optional
+       Incremental change in the parameter value for each iteration. If None and target is None, raises ValueError.
+   :param target: float or None, optional
+       Target parameter value. If None, continuation is performed until maxit_con iterations.
+   :param kwargs: dict
+       Additional keyword arguments for customization.
            maxit_con : int, optional
                Maximum number of continuation steps. Default is 1000.
            method : str, optional
                Continuation method ('normal' or 'pseudo-arclength'). Default is 'normal'.
            mode : str, optional
                Return mode ('partial' or 'full'). Default is 'partial'.
            Other keyword arguments : Additional parameters specific to the step function used internally.
 
-   Returns
-   -------
-       tuple or array_like
-           Depending on the mode specified in kwargs, returns either a tuple or an array.
+   :return: tuple or array_like
+       Depending on the mode specified in kwargs, returns either a tuple or an array.
            - In 'partial' mode, returns a tuple containing the final state x and the final parameter value mu.
            - In 'full' mode, returns an array containing all the states x, an array of the norm of the correction at each step, and the final parameter value mu (if target is None).
 
-   Raises
-   ------
-       ValueError
-           If either 'dmu' or 'target' should be not 'None' but are not provided.
-       ValueError
-           If the provided continuation method is invalid. Choose either 'normal' or 'pseudo-arclength'.
+   :raises:
+       ValueError: If either 'dmu' or 'target' should be not 'None' but are not provided.
+       ValueError: If the provided continuation method is invalid. Choose either 'normal' or 'pseudo-arclength'.
 
    Examples
-   --------
-   >>> # Define the functions df and dfmu
-   >>> def df(x, mu0):
-   >>>     # Compute the Jacobian matrix with respect to state variable x and parameter mu
-   >>>     pass
-   >>> def dfmu(x, mu0):
-   >>>     # Compute the Jacobian matrix derivative with respect to parameter mu
-   >>>     pass
-   >>> 
-   >>> # Define the initial state and tangent
-   >>> x0 = np.array([1.0, 2.0])
-   >>> dx0 = np.array([0.1, 0.1])
-   >>> 
-   >>> # Perform continuation from start value to target value
-   >>> start = 0.0
-   >>> target = 1.0
-   >>> result = cont(x0, dx0, start, df, dfmu, target=target, maxit_con=1000, method='normal', mode='full')
-   >>> print(result)
-
-
-.. py:function:: opts(interface={}, parameters={}, **kwargs)
+   =============
+       >>> # Define the functions df and dfmu
+       >>> def df(x, mu0):
+       >>>     # Compute the Jacobian matrix with respect to state variable x and parameter mu
+       >>>     pass
+       >>> def dfmu(x, mu0):
+       >>>     # Compute the Jacobian matrix derivative with respect to parameter mu
+       >>>     pass
+       >>> 
+       >>> # Define the initial state and tangent
+       >>> x0 = np.array([1.0, 2.0])
+       >>> dx0 = np.array([0.1, 0.1])
+       >>> 
+       >>> # Perform continuation from start value to target value
+       >>> start = 0.0
+       >>> target = 1.0
+       >>> result = cont(x0, dx0, start, df, dfmu, target=target, maxit_con=1000, method='normal', mode='full')
+       >>> print(result)
 
 
-.. py:class:: Bifurcation(interface=None, parameters=None)
+.. py:class:: Bifurcation
 
 
    Defines default options for the Bifurcation package
```

### Comparing `byma-0.0.25/docs/source/autoapi/byma/pyplot/index.rst` & `byma-0.1.0/docs/source/autoapi/byma/pyplot/plots/index.rst`

 * *Files 21% similar despite different names*

```diff
@@ -1,100 +1,97 @@
-:py:mod:`byma.pyplot`
-=====================
+:py:mod:`byma.pyplot.plots`
+===========================
 
-.. py:module:: byma.pyplot
+.. py:module:: byma.pyplot.plots
 
 
-Submodules
-----------
-.. toctree::
-   :titlesonly:
-   :maxdepth: 1
-
-   plots/index.rst
-
-
-Package Contents
-----------------
+Module Contents
+---------------
 
 
 Functions
 ~~~~~~~~~
 
 .. autoapisummary::
 
-   byma.pyplot.plot_numerical_error
-   byma.pyplot.plot_loglog_convergence
-   byma.pyplot.plot_scale
-   byma.pyplot.plot
-
-
+   byma.pyplot.plots.plot_scale
+   byma.pyplot.plots.plot
+   byma.pyplot.plots.plot_numerical_error
 
-.. py:function:: plot_numerical_error(n, func, solve_func, save_title=None, save_path=None, **kwargs)
-
-   Plot the numerical error between the exact and numerical solutions and print the maximum error.
-
-   Parameters:
-       n (int): Number of grid points.
-       func (object): Instance of the class containing the exact solution.
-       solve_func (function): Function to solve the system.
-       save_title (str): file name plot
-       save_path (str): Path to save the plot. If None, the plot will be saved in the current directory.
-       **kwargs: Additional keyword arguments to customize the plot and title for saving.
-
-
-.. py:function:: plot_loglog_convergence(step, erros, **kwargs)
-
-   Plot the convergence of error using log-log scale for (non)-equidistant grids.
-
-   Parameters:
-       step (array-like): Array of step sizes for grid 1.
-       erro (array-like): Array of errors for grid 1.
-       **kwargs:
-           stept (array-like): Array of step sizes fro grid 2.
-           errot (array-like): Array of errors for grid 2.
-           title (str): Title of the plot.
-           x_label (str): Label for the x-axis.
-           y_label (str): Label for the y-axis.
-           label1 (str): Label for grid 1.
-           label2 (str): Label for grid 2.
-           save_title (str): file name plot
-           save_path (str): Path to save the plot. If None, the plot will be saved in the current directory.
 
 
 .. py:function:: plot_scale(x, y, label, scale, style=None)
 
    Plot data with specified scale and style.
 
-   Parameters:
-       x (array-like): Data points for the x-axis.
-       y (array-like): Data points for the y-axis.
-       label (str): Label for the data.
-       scale (str): Scale for the plot. Options: 'normal', 'loglog', 'xlog', 'ylog'.
-       style (dict or None): Dictionary specifying line style. If None, default style is used.
+   Parameters
+   ----------
+   x : array-like
+       Data points for the x-axis.
+   y : array-like
+       Data points for the y-axis.
+   label : str
+       Label for the data.
+   scale : str
+       Scale for the plot. Options: 'normal', 'loglog', 'xlog', 'ylog'.
+   style : dict or None, optional
+       Dictionary specifying line style. If None, default style is used.
+
+   Returns
+   -------
+   None
 
 
 .. py:function:: plot(x, y, **kwargs)
 
    Function that create plots of different kinds. With this function it is possible to plots n numbers of 
-   function in the same figure quickly and with high personalization. 
+   function in the same figure quickly and with high personalization.
+
+   Parameters
+   ----------
+   x : array-like
+       Array of x values.
+   y : array-like
+       Array of y values.
+   **kwargs : dict, optional
+       settings (dict): Overall plot settings.
+           title (str): Title of the plot.
+           xlabel (str): Label for the x-axis.
+           ylabel (str): Label for the y-axis.
+           label (str):  Label for the 1st function.
+           label{i} (str): Label for the ith function from i=2.
+           x{i} (array-like): Array of x values for the ith function from i=2.
+           y{i} (array-like): Array of y values for the ith function from i=2.
+           save_title (str): File name to save the plot.
+           save_path (str): Path to save the plot. If None, the plot will be saved in the current directory.
+           scale (str): Scale for the plot. Options: 'normal', 'loglog', 'xlog', 'ylog'.
+       style (dict or list of dicts): Line style(s) for the plot. (Not yet working)
+
+   Returns
+   -------
+   None
+
+
+.. py:function:: plot_numerical_error(n, func, solve_func, save_title=None, save_path=None, **kwargs)
+
+   Plot the numerical error between the exact and numerical solutions and print the maximum error.
 
-   Parameters:
-       x (array-like): Array of x values.
-       y (array-like): Array of y values.
-       **kwargs:
-           settings (dict): Overall plot settings.
-               title (str): Title of the plot.
-               xlabel (str): Label for the x-axis.
-               ylabel (str): Label for the y-axis.
-               label (str):  Label for the 1st function.
-               label{i} (str): Label for the ith function from i=2.
-               x{i} (array-like): Array of x values for the ith function from i=2.
-               y{i} (array-like): Array of y values for the ith function from i=2.
-               save_title (str): File name to save the plot.
-               save_path (str): Path to save the plot. If None, the plot will be saved in the current directory.
-               scale (str): Scale for the plot. Options: 'normal', 'loglog', 'xlog', 'ylog'.
-           style (dict or list of dicts): Line style(s) for the plot. (Not yet working)
-           
-   N.B Every element in the settings dict can be used as a normal kwargs when calling the function.
+   Parameters
+   ----------
+   n : int
+       Number of grid points.
+   func : object
+       Instance of the class containing the exact solution.
+   solve_func : function
+       Function to solve the system.
+   save_title : str, optional
+       File name plot.
+   save_path : str, optional
+       Path to save the plot. If None, the plot will be saved in the current directory.
+   **kwargs : dict, optional
+       Additional keyword arguments to customize the plot and title for saving.
+
+   Returns
+   -------
+   None
```

### Comparing `byma-0.0.25/docs/source/autoapi/byma/pyplot/plots/index.rst` & `byma-0.1.0/docs/source/autoapi/byma/pyplot/index.rst`

 * *Files 21% similar despite different names*

```diff
@@ -1,91 +1,106 @@
-:py:mod:`byma.pyplot.plots`
-===========================
+:py:mod:`byma.pyplot`
+=====================
 
-.. py:module:: byma.pyplot.plots
+.. py:module:: byma.pyplot
 
 
-Module Contents
----------------
+Submodules
+----------
+.. toctree::
+   :titlesonly:
+   :maxdepth: 1
 
+   plots/index.rst
 
-Functions
-~~~~~~~~~
 
-.. autoapisummary::
-
-   byma.pyplot.plots.plot_numerical_error
-   byma.pyplot.plots.plot_loglog_convergence
-   byma.pyplot.plots.plot_scale
-   byma.pyplot.plots.plot
+Package Contents
+----------------
 
 
+Functions
+~~~~~~~~~
 
-.. py:function:: plot_numerical_error(n, func, solve_func, save_title=None, save_path=None, **kwargs)
+.. autoapisummary::
 
-   Plot the numerical error between the exact and numerical solutions and print the maximum error.
+   byma.pyplot.plot_scale
+   byma.pyplot.plot
+   byma.pyplot.plot_numerical_error
 
-   Parameters:
-       n (int): Number of grid points.
-       func (object): Instance of the class containing the exact solution.
-       solve_func (function): Function to solve the system.
-       save_title (str): file name plot
-       save_path (str): Path to save the plot. If None, the plot will be saved in the current directory.
-       **kwargs: Additional keyword arguments to customize the plot and title for saving.
-
-
-.. py:function:: plot_loglog_convergence(step, erros, **kwargs)
-
-   Plot the convergence of error using log-log scale for (non)-equidistant grids.
-
-   Parameters:
-       step (array-like): Array of step sizes for grid 1.
-       erro (array-like): Array of errors for grid 1.
-       **kwargs:
-           stept (array-like): Array of step sizes fro grid 2.
-           errot (array-like): Array of errors for grid 2.
-           title (str): Title of the plot.
-           x_label (str): Label for the x-axis.
-           y_label (str): Label for the y-axis.
-           label1 (str): Label for grid 1.
-           label2 (str): Label for grid 2.
-           save_title (str): file name plot
-           save_path (str): Path to save the plot. If None, the plot will be saved in the current directory.
 
 
 .. py:function:: plot_scale(x, y, label, scale, style=None)
 
    Plot data with specified scale and style.
 
-   Parameters:
-       x (array-like): Data points for the x-axis.
-       y (array-like): Data points for the y-axis.
-       label (str): Label for the data.
-       scale (str): Scale for the plot. Options: 'normal', 'loglog', 'xlog', 'ylog'.
-       style (dict or None): Dictionary specifying line style. If None, default style is used.
+   Parameters
+   ----------
+   x : array-like
+       Data points for the x-axis.
+   y : array-like
+       Data points for the y-axis.
+   label : str
+       Label for the data.
+   scale : str
+       Scale for the plot. Options: 'normal', 'loglog', 'xlog', 'ylog'.
+   style : dict or None, optional
+       Dictionary specifying line style. If None, default style is used.
+
+   Returns
+   -------
+   None
 
 
 .. py:function:: plot(x, y, **kwargs)
 
    Function that create plots of different kinds. With this function it is possible to plots n numbers of 
-   function in the same figure quickly and with high personalization. 
+   function in the same figure quickly and with high personalization.
+
+   Parameters
+   ----------
+   x : array-like
+       Array of x values.
+   y : array-like
+       Array of y values.
+   **kwargs : dict, optional
+       settings (dict): Overall plot settings.
+           title (str): Title of the plot.
+           xlabel (str): Label for the x-axis.
+           ylabel (str): Label for the y-axis.
+           label (str):  Label for the 1st function.
+           label{i} (str): Label for the ith function from i=2.
+           x{i} (array-like): Array of x values for the ith function from i=2.
+           y{i} (array-like): Array of y values for the ith function from i=2.
+           save_title (str): File name to save the plot.
+           save_path (str): Path to save the plot. If None, the plot will be saved in the current directory.
+           scale (str): Scale for the plot. Options: 'normal', 'loglog', 'xlog', 'ylog'.
+       style (dict or list of dicts): Line style(s) for the plot. (Not yet working)
+
+   Returns
+   -------
+   None
+
+
+.. py:function:: plot_numerical_error(n, func, solve_func, save_title=None, save_path=None, **kwargs)
+
+   Plot the numerical error between the exact and numerical solutions and print the maximum error.
 
-   Parameters:
-       x (array-like): Array of x values.
-       y (array-like): Array of y values.
-       **kwargs:
-           settings (dict): Overall plot settings.
-               title (str): Title of the plot.
-               xlabel (str): Label for the x-axis.
-               ylabel (str): Label for the y-axis.
-               label (str):  Label for the 1st function.
-               label{i} (str): Label for the ith function from i=2.
-               x{i} (array-like): Array of x values for the ith function from i=2.
-               y{i} (array-like): Array of y values for the ith function from i=2.
-               save_title (str): File name to save the plot.
-               save_path (str): Path to save the plot. If None, the plot will be saved in the current directory.
-               scale (str): Scale for the plot. Options: 'normal', 'loglog', 'xlog', 'ylog'.
-           style (dict or list of dicts): Line style(s) for the plot. (Not yet working)
-           
-   N.B Every element in the settings dict can be used as a normal kwargs when calling the function.
+   Parameters
+   ----------
+   n : int
+       Number of grid points.
+   func : object
+       Instance of the class containing the exact solution.
+   solve_func : function
+       Function to solve the system.
+   save_title : str, optional
+       File name plot.
+   save_path : str, optional
+       Path to save the plot. If None, the plot will be saved in the current directory.
+   **kwargs : dict, optional
+       Additional keyword arguments to customize the plot and title for saving.
+
+   Returns
+   -------
+   None
```

### Comparing `byma-0.0.25/docs/source/conf.py` & `byma-0.1.0/docs/source/conf.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,14 +25,15 @@
 
 sys.path.insert(0, os.path.abspath('../sphinxext'))
 
 extensions = [
     'sphinx.ext.duration',
     'sphinx.ext.doctest',
     'sphinx.ext.autodoc',
+    'sphinx.ext.apidoc',
     'autoapi.extension',
     'sphinx.ext.todo',
     'sphinx.ext.autosummary',
     'sphinx.ext.intersphinx',
     'sphinx.ext.coverage',
     'sphinx.ext.graphviz',
     'sphinx.ext.ifconfig',
```

### Comparing `byma-0.0.25/docs/source/index.rst` & `byma-0.1.0/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `byma-0.0.25/examples/assignment_4.py` & `byma-0.1.0/examples/assignment_4.py`

 * *Files identical despite different names*

### Comparing `byma-0.0.25/pyproject.toml` & `byma-0.1.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `byma-0.0.25/setup.py` & `byma-0.1.0/setup.py`

 * *Files identical despite different names*

