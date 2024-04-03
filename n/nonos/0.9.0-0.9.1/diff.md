# Comparing `tmp/nonos-0.9.0.tar.gz` & `tmp/nonos-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/wafflarg/nonos/dist/.tmp-q9slxm44/nonos-0.9.0.tar", last modified: Tue Jun 27 15:38:07 2023, max compression
+gzip compressed data, was "/home/wafflarg/nonos/dist/.tmp-xdlv33yb/nonos-0.9.1.tar", last modified: Mon Jul 31 15:30:05 2023, max compression
```

## Comparing `nonos-0.9.0.tar` & `nonos-0.9.1.tar`

### file list

```diff
@@ -1,73 +1,73 @@
-drwxrwxr-x   0 wafflarg  (1001) wafflarg  (1001)        0 2023-06-27 15:38:07.902330 nonos-0.9.0/
-drwxrwxr-x   0 wafflarg  (1001) wafflarg  (1001)        0 2023-06-27 15:38:07.882331 nonos-0.9.0/.github/
-drwxrwxr-x   0 wafflarg  (1001) wafflarg  (1001)        0 2023-06-27 15:38:07.882331 nonos-0.9.0/.github/workflows/
--rw-rw-r--   0 wafflarg  (1001) wafflarg  (1001)     2992 2023-03-09 13:44:29.000000 nonos-0.9.0/.github/workflows/ci.yml
--rw-rw-r--   0 wafflarg  (1001) wafflarg  (1001)      749 2023-05-31 10:33:03.000000 nonos-0.9.0/.pre-commit-config.yaml
--rw-rw-r--   0 wafflarg  (1001) wafflarg  (1001)    35149 2021-03-19 13:34:53.000000 nonos-0.9.0/LICENSE
--rw-rw-r--   0 wafflarg  (1001) wafflarg  (1001)    11036 2023-06-27 15:38:07.902330 nonos-0.9.0/PKG-INFO
--rw-rw-r--   0 wafflarg  (1001) wafflarg  (1001)    10462 2023-06-13 13:00:11.000000 nonos-0.9.0/README.md
-drwxrwxr-x   0 wafflarg  (1001) wafflarg  (1001)        0 2023-06-27 15:38:07.882331 nonos-0.9.0/nonos/
--rw-rw-r--   0 wafflarg  (1001) wafflarg  (1001)       37 2023-02-02 16:13:06.000000 nonos-0.9.0/nonos/__init__.py
--rw-rw-r--   0 wafflarg  (1001) wafflarg  (1001)       73 2021-12-17 15:56:12.000000 nonos-0.9.0/nonos/__main__.py
--rw-rw-r--   0 wafflarg  (1001) wafflarg  (1001)       22 2023-06-27 15:37:20.000000 nonos-0.9.0/nonos/__version__.py
-drwxrwxr-x   0 wafflarg  (1001) wafflarg  (1001)        0 2023-06-27 15:38:07.886330 nonos-0.9.0/nonos/api/
--rw-rw-r--   0 wafflarg  (1001) wafflarg  (1001)      365 2023-03-09 13:44:29.000000 nonos-0.9.0/nonos/api/__init__.py
--rw-rw-r--   0 wafflarg  (1001) wafflarg  (1001)    20614 2022-11-16 09:58:36.000000 nonos-0.9.0/nonos/api/_adapt_clm_vtk.py
--rw-rw-r--   0 wafflarg  (1001) wafflarg  (1001)    61648 2023-06-27 07:49:11.000000 nonos-0.9.0/nonos/api/analysis.py
--rw-rw-r--   0 wafflarg  (1001) wafflarg  (1001)    31352 2023-03-08 16:19:23.000000 nonos-0.9.0/nonos/api/from_simulation.py
--rw-rw-r--   0 wafflarg  (1001) wafflarg  (1001)     7346 2023-06-27 08:45:04.000000 nonos-0.9.0/nonos/api/satellite.py
--rw-rw-r--   0 wafflarg  (1001) wafflarg  (1001)      438 2022-11-21 14:54:36.000000 nonos-0.9.0/nonos/api/tools.py
--rw-rw-r--   0 wafflarg  (1001) wafflarg  (1001)     1392 2022-11-21 14:54:36.000000 nonos-0.9.0/nonos/config.py
--rw-rw-r--   0 wafflarg  (1001) wafflarg  (1001)      111 2023-03-09 13:44:29.000000 nonos-0.9.0/nonos/default.mplstyle
--rw-rw-r--   0 wafflarg  (1001) wafflarg  (1001)     1031 2023-02-02 16:13:06.000000 nonos-0.9.0/nonos/logging.py
--rw-rw-r--   0 wafflarg  (1001) wafflarg  (1001)     1765 2021-12-17 15:56:12.000000 nonos-0.9.0/nonos/logo.txt
--rw-rw-r--   0 wafflarg  (1001) wafflarg  (1001)    17408 2023-06-27 08:45:04.000000 nonos-0.9.0/nonos/main.py
--rw-rw-r--   0 wafflarg  (1001) wafflarg  (1001)     2335 2022-11-21 14:54:36.000000 nonos-0.9.0/nonos/parsing.py
--rw-rw-r--   0 wafflarg  (1001) wafflarg  (1001)        0 2022-11-21 14:54:36.000000 nonos-0.9.0/nonos/py.typed
--rw-rw-r--   0 wafflarg  (1001) wafflarg  (1001)     2004 2023-03-09 13:44:29.000000 nonos-0.9.0/nonos/styling.py
-drwxrwxr-x   0 wafflarg  (1001) wafflarg  (1001)        0 2023-06-27 15:38:07.882331 nonos-0.9.0/nonos.egg-info/
--rw-rw-r--   0 wafflarg  (1001) wafflarg  (1001)    11036 2023-06-27 15:38:07.000000 nonos-0.9.0/nonos.egg-info/PKG-INFO
--rw-rw-r--   0 wafflarg  (1001) wafflarg  (1001)     1693 2023-06-27 15:38:07.000000 nonos-0.9.0/nonos.egg-info/SOURCES.txt
--rw-rw-r--   0 wafflarg  (1001) wafflarg  (1001)        1 2023-06-27 15:38:07.000000 nonos-0.9.0/nonos.egg-info/dependency_links.txt
--rw-rw-r--   0 wafflarg  (1001) wafflarg  (1001)       42 2023-06-27 15:38:07.000000 nonos-0.9.0/nonos.egg-info/entry_points.txt
--rw-rw-r--   0 wafflarg  (1001) wafflarg  (1001)      165 2023-06-27 15:38:07.000000 nonos-0.9.0/nonos.egg-info/requires.txt
--rw-rw-r--   0 wafflarg  (1001) wafflarg  (1001)        6 2023-06-27 15:38:07.000000 nonos-0.9.0/nonos.egg-info/top_level.txt
--rw-rw-r--   0 wafflarg  (1001) wafflarg  (1001)     2057 2023-06-27 08:45:04.000000 nonos-0.9.0/pyproject.toml
--rw-rw-r--   0 wafflarg  (1001) wafflarg  (1001)       38 2023-06-27 15:38:07.902330 nonos-0.9.0/setup.cfg
-drwxrwxr-x   0 wafflarg  (1001) wafflarg  (1001)        0 2023-06-27 15:38:07.886330 nonos-0.9.0/tests/
--rw-rw-r--   0 wafflarg  (1001) wafflarg  (1001)      686 2023-06-26 16:17:24.000000 nonos-0.9.0/tests/conftest.py
-drwxrwxr-x   0 wafflarg  (1001) wafflarg  (1001)        0 2023-06-27 15:38:07.882331 nonos-0.9.0/tests/data/
-drwxrwxr-x   0 wafflarg  (1001) wafflarg  (1001)        0 2023-06-27 15:38:07.886330 nonos-0.9.0/tests/data/fargo3d_planet2d/
--rw-rw-r--   0 wafflarg  (1001) wafflarg  (1001)     5525 2022-11-21 14:54:36.000000 nonos-0.9.0/tests/data/fargo3d_planet2d/domain_x.dat
--rw-rw-r--   0 wafflarg  (1001) wafflarg  (1001)     5523 2022-11-21 14:54:36.000000 nonos-0.9.0/tests/data/fargo3d_planet2d/domain_y.dat
--rw-rw-r--   0 wafflarg  (1001) wafflarg  (1001)       42 2022-11-21 14:54:36.000000 nonos-0.9.0/tests/data/fargo3d_planet2d/domain_z.dat
--rw-rw-r--   0 wafflarg  (1001) wafflarg  (1001)   524289 2022-11-21 14:54:36.000000 nonos-0.9.0/tests/data/fargo3d_planet2d/gasdens0.dat
--rw-rw-r--   0 wafflarg  (1001) wafflarg  (1001)   524288 2022-11-21 14:54:36.000000 nonos-0.9.0/tests/data/fargo3d_planet2d/gasdens40.dat
--rw-rw-r--   0 wafflarg  (1001) wafflarg  (1001)   524288 2022-11-21 14:54:36.000000 nonos-0.9.0/tests/data/fargo3d_planet2d/gasvy40.dat
--rw-rw-r--   0 wafflarg  (1001) wafflarg  (1001)      263 2022-11-21 14:54:36.000000 nonos-0.9.0/tests/data/fargo3d_planet2d/myplanet.cfg
--rw-rw-r--   0 wafflarg  (1001) wafflarg  (1001)     7886 2022-11-21 14:54:36.000000 nonos-0.9.0/tests/data/fargo3d_planet2d/planet0.dat
--rw-rw-r--   0 wafflarg  (1001) wafflarg  (1001)     1014 2022-11-21 14:54:36.000000 nonos-0.9.0/tests/data/fargo3d_planet2d/variables.par
-drwxrwxr-x   0 wafflarg  (1001) wafflarg  (1001)        0 2023-06-27 15:38:07.886330 nonos-0.9.0/tests/data/idefix_newvtk_planet2d/
--rw-rw-r--   0 wafflarg  (1001) wafflarg  (1001)   298359 2022-11-21 14:54:36.000000 nonos-0.9.0/tests/data/idefix_newvtk_planet2d/data.0000.vtk
--rw-rw-r--   0 wafflarg  (1001) wafflarg  (1001)   298359 2022-11-21 14:54:36.000000 nonos-0.9.0/tests/data/idefix_newvtk_planet2d/data.0023.vtk
--rw-rw-r--   0 wafflarg  (1001) wafflarg  (1001)     1007 2022-11-21 14:54:36.000000 nonos-0.9.0/tests/data/idefix_newvtk_planet2d/idefix.ini
--rw-rw-r--   0 wafflarg  (1001) wafflarg  (1001)     3717 2022-11-21 14:54:36.000000 nonos-0.9.0/tests/data/idefix_newvtk_planet2d/planet0.dat
-drwxrwxr-x   0 wafflarg  (1001) wafflarg  (1001)        0 2023-06-27 15:38:07.898331 nonos-0.9.0/tests/data/idefix_planet3d/
--rw-rw-r--   0 wafflarg  (1001) wafflarg  (1001)  7490113 2021-03-30 18:17:30.000000 nonos-0.9.0/tests/data/idefix_planet3d/data.0000.vtk
--rw-rw-r--   0 wafflarg  (1001) wafflarg  (1001)  7490113 2021-03-30 18:22:00.000000 nonos-0.9.0/tests/data/idefix_planet3d/data.0043.vtk
--rwxrwxr-x   0 wafflarg  (1001) wafflarg  (1001)      213 2022-11-21 14:54:36.000000 nonos-0.9.0/tests/data/idefix_planet3d/definitions.hpp
--rw-rw-r--   0 wafflarg  (1001) wafflarg  (1001)      805 2022-11-21 14:54:36.000000 nonos-0.9.0/tests/data/idefix_planet3d/idefix.ini
--rw-rw-r--   0 wafflarg  (1001) wafflarg  (1001)    11155 2021-03-30 18:24:51.000000 nonos-0.9.0/tests/data/idefix_planet3d/planet0.dat
-drwxrwxr-x   0 wafflarg  (1001) wafflarg  (1001)        0 2023-06-27 15:38:07.898331 nonos-0.9.0/tests/data/idefix_rwi/
--rw-rw-r--   0 wafflarg  (1001) wafflarg  (1001)  1579289 2021-04-12 13:19:18.000000 nonos-0.9.0/tests/data/idefix_rwi/data.0000.vtk
--rw-rw-r--   0 wafflarg  (1001) wafflarg  (1001)  1579289 2021-04-12 13:19:18.000000 nonos-0.9.0/tests/data/idefix_rwi/data.0001.vtk
--rwxrwxr-x   0 wafflarg  (1001) wafflarg  (1001)      213 2022-11-21 14:54:36.000000 nonos-0.9.0/tests/data/idefix_rwi/definitions.hpp
--rw-rw-r--   0 wafflarg  (1001) wafflarg  (1001)      543 2022-11-21 14:54:36.000000 nonos-0.9.0/tests/data/idefix_rwi/idefix.ini
--rw-rw-r--   0 wafflarg  (1001) wafflarg  (1001)     3260 2022-11-21 14:54:36.000000 nonos-0.9.0/tests/test_cli.py
--rw-rw-r--   0 wafflarg  (1001) wafflarg  (1001)      253 2023-06-26 16:17:24.000000 nonos-0.9.0/tests/test_errors.py
--rw-rw-r--   0 wafflarg  (1001) wafflarg  (1001)     1631 2023-02-02 16:13:07.000000 nonos-0.9.0/tests/test_image_comp.py
--rw-rw-r--   0 wafflarg  (1001) wafflarg  (1001)     1449 2022-11-21 14:54:36.000000 nonos-0.9.0/tests/test_load_config.py
--rw-rw-r--   0 wafflarg  (1001) wafflarg  (1001)      763 2022-11-21 14:54:36.000000 nonos-0.9.0/tests/test_params_usage.py
--rw-rw-r--   0 wafflarg  (1001) wafflarg  (1001)     3541 2023-06-26 16:17:24.000000 nonos-0.9.0/tests/test_parsing.py
--rw-rw-r--   0 wafflarg  (1001) wafflarg  (1001)     5791 2023-06-27 08:45:04.000000 nonos-0.9.0/tests/test_plotting.py
--rw-rw-r--   0 wafflarg  (1001) wafflarg  (1001)      604 2023-02-08 18:05:36.000000 nonos-0.9.0/tests/test_readme.py
+drwxrwxr-x   0 wafflarg  (1001) wafflarg  (1001)        0 2023-07-31 15:30:05.769287 nonos-0.9.1/
+drwxrwxr-x   0 wafflarg  (1001) wafflarg  (1001)        0 2023-07-31 15:30:05.749287 nonos-0.9.1/.github/
+drwxrwxr-x   0 wafflarg  (1001) wafflarg  (1001)        0 2023-07-31 15:30:05.749287 nonos-0.9.1/.github/workflows/
+-rw-rw-r--   0 wafflarg  (1001) wafflarg  (1001)     2992 2023-03-09 13:44:29.000000 nonos-0.9.1/.github/workflows/ci.yml
+-rw-rw-r--   0 wafflarg  (1001) wafflarg  (1001)      745 2023-07-31 15:22:23.000000 nonos-0.9.1/.pre-commit-config.yaml
+-rw-rw-r--   0 wafflarg  (1001) wafflarg  (1001)    35149 2021-03-19 13:34:53.000000 nonos-0.9.1/LICENSE
+-rw-rw-r--   0 wafflarg  (1001) wafflarg  (1001)    11036 2023-07-31 15:30:05.769287 nonos-0.9.1/PKG-INFO
+-rw-rw-r--   0 wafflarg  (1001) wafflarg  (1001)    10462 2023-06-13 13:00:11.000000 nonos-0.9.1/README.md
+drwxrwxr-x   0 wafflarg  (1001) wafflarg  (1001)        0 2023-07-31 15:30:05.749287 nonos-0.9.1/nonos/
+-rw-rw-r--   0 wafflarg  (1001) wafflarg  (1001)       37 2023-02-02 16:13:06.000000 nonos-0.9.1/nonos/__init__.py
+-rw-rw-r--   0 wafflarg  (1001) wafflarg  (1001)       73 2021-12-17 15:56:12.000000 nonos-0.9.1/nonos/__main__.py
+-rw-rw-r--   0 wafflarg  (1001) wafflarg  (1001)       22 2023-07-31 15:26:25.000000 nonos-0.9.1/nonos/__version__.py
+drwxrwxr-x   0 wafflarg  (1001) wafflarg  (1001)        0 2023-07-31 15:30:05.753287 nonos-0.9.1/nonos/api/
+-rw-rw-r--   0 wafflarg  (1001) wafflarg  (1001)      297 2023-07-31 15:22:23.000000 nonos-0.9.1/nonos/api/__init__.py
+-rw-rw-r--   0 wafflarg  (1001) wafflarg  (1001)    20614 2022-11-16 09:58:36.000000 nonos-0.9.1/nonos/api/_adapt_clm_vtk.py
+-rw-rw-r--   0 wafflarg  (1001) wafflarg  (1001)    57598 2023-07-31 15:22:23.000000 nonos-0.9.1/nonos/api/analysis.py
+-rw-rw-r--   0 wafflarg  (1001) wafflarg  (1001)    31352 2023-03-08 16:19:23.000000 nonos-0.9.1/nonos/api/from_simulation.py
+-rw-rw-r--   0 wafflarg  (1001) wafflarg  (1001)     6508 2023-07-31 15:22:23.000000 nonos-0.9.1/nonos/api/satellite.py
+-rw-rw-r--   0 wafflarg  (1001) wafflarg  (1001)      438 2022-11-21 14:54:36.000000 nonos-0.9.1/nonos/api/tools.py
+-rw-rw-r--   0 wafflarg  (1001) wafflarg  (1001)     1392 2022-11-21 14:54:36.000000 nonos-0.9.1/nonos/config.py
+-rw-rw-r--   0 wafflarg  (1001) wafflarg  (1001)      111 2023-03-09 13:44:29.000000 nonos-0.9.1/nonos/default.mplstyle
+-rw-rw-r--   0 wafflarg  (1001) wafflarg  (1001)     1031 2023-02-02 16:13:06.000000 nonos-0.9.1/nonos/logging.py
+-rw-rw-r--   0 wafflarg  (1001) wafflarg  (1001)     1765 2021-12-17 15:56:12.000000 nonos-0.9.1/nonos/logo.txt
+-rw-rw-r--   0 wafflarg  (1001) wafflarg  (1001)    17408 2023-06-27 08:45:04.000000 nonos-0.9.1/nonos/main.py
+-rw-rw-r--   0 wafflarg  (1001) wafflarg  (1001)     2335 2022-11-21 14:54:36.000000 nonos-0.9.1/nonos/parsing.py
+-rw-rw-r--   0 wafflarg  (1001) wafflarg  (1001)        0 2022-11-21 14:54:36.000000 nonos-0.9.1/nonos/py.typed
+-rw-rw-r--   0 wafflarg  (1001) wafflarg  (1001)     2004 2023-03-09 13:44:29.000000 nonos-0.9.1/nonos/styling.py
+drwxrwxr-x   0 wafflarg  (1001) wafflarg  (1001)        0 2023-07-31 15:30:05.753287 nonos-0.9.1/nonos.egg-info/
+-rw-rw-r--   0 wafflarg  (1001) wafflarg  (1001)    11036 2023-07-31 15:30:05.000000 nonos-0.9.1/nonos.egg-info/PKG-INFO
+-rw-rw-r--   0 wafflarg  (1001) wafflarg  (1001)     1693 2023-07-31 15:30:05.000000 nonos-0.9.1/nonos.egg-info/SOURCES.txt
+-rw-rw-r--   0 wafflarg  (1001) wafflarg  (1001)        1 2023-07-31 15:30:05.000000 nonos-0.9.1/nonos.egg-info/dependency_links.txt
+-rw-rw-r--   0 wafflarg  (1001) wafflarg  (1001)       42 2023-07-31 15:30:05.000000 nonos-0.9.1/nonos.egg-info/entry_points.txt
+-rw-rw-r--   0 wafflarg  (1001) wafflarg  (1001)      165 2023-07-31 15:30:05.000000 nonos-0.9.1/nonos.egg-info/requires.txt
+-rw-rw-r--   0 wafflarg  (1001) wafflarg  (1001)        6 2023-07-31 15:30:05.000000 nonos-0.9.1/nonos.egg-info/top_level.txt
+-rw-rw-r--   0 wafflarg  (1001) wafflarg  (1001)     2057 2023-06-28 09:53:47.000000 nonos-0.9.1/pyproject.toml
+-rw-rw-r--   0 wafflarg  (1001) wafflarg  (1001)       38 2023-07-31 15:30:05.769287 nonos-0.9.1/setup.cfg
+drwxrwxr-x   0 wafflarg  (1001) wafflarg  (1001)        0 2023-07-31 15:30:05.753287 nonos-0.9.1/tests/
+-rw-rw-r--   0 wafflarg  (1001) wafflarg  (1001)      686 2023-06-26 16:17:24.000000 nonos-0.9.1/tests/conftest.py
+drwxrwxr-x   0 wafflarg  (1001) wafflarg  (1001)        0 2023-07-31 15:30:05.749287 nonos-0.9.1/tests/data/
+drwxrwxr-x   0 wafflarg  (1001) wafflarg  (1001)        0 2023-07-31 15:30:05.753287 nonos-0.9.1/tests/data/fargo3d_planet2d/
+-rw-rw-r--   0 wafflarg  (1001) wafflarg  (1001)     5525 2022-11-21 14:54:36.000000 nonos-0.9.1/tests/data/fargo3d_planet2d/domain_x.dat
+-rw-rw-r--   0 wafflarg  (1001) wafflarg  (1001)     5523 2022-11-21 14:54:36.000000 nonos-0.9.1/tests/data/fargo3d_planet2d/domain_y.dat
+-rw-rw-r--   0 wafflarg  (1001) wafflarg  (1001)       42 2022-11-21 14:54:36.000000 nonos-0.9.1/tests/data/fargo3d_planet2d/domain_z.dat
+-rw-rw-r--   0 wafflarg  (1001) wafflarg  (1001)   524289 2022-11-21 14:54:36.000000 nonos-0.9.1/tests/data/fargo3d_planet2d/gasdens0.dat
+-rw-rw-r--   0 wafflarg  (1001) wafflarg  (1001)   524288 2022-11-21 14:54:36.000000 nonos-0.9.1/tests/data/fargo3d_planet2d/gasdens40.dat
+-rw-rw-r--   0 wafflarg  (1001) wafflarg  (1001)   524288 2022-11-21 14:54:36.000000 nonos-0.9.1/tests/data/fargo3d_planet2d/gasvy40.dat
+-rw-rw-r--   0 wafflarg  (1001) wafflarg  (1001)      263 2022-11-21 14:54:36.000000 nonos-0.9.1/tests/data/fargo3d_planet2d/myplanet.cfg
+-rw-rw-r--   0 wafflarg  (1001) wafflarg  (1001)     7886 2022-11-21 14:54:36.000000 nonos-0.9.1/tests/data/fargo3d_planet2d/planet0.dat
+-rw-rw-r--   0 wafflarg  (1001) wafflarg  (1001)     1014 2022-11-21 14:54:36.000000 nonos-0.9.1/tests/data/fargo3d_planet2d/variables.par
+drwxrwxr-x   0 wafflarg  (1001) wafflarg  (1001)        0 2023-07-31 15:30:05.757287 nonos-0.9.1/tests/data/idefix_newvtk_planet2d/
+-rw-rw-r--   0 wafflarg  (1001) wafflarg  (1001)   298359 2022-11-21 14:54:36.000000 nonos-0.9.1/tests/data/idefix_newvtk_planet2d/data.0000.vtk
+-rw-rw-r--   0 wafflarg  (1001) wafflarg  (1001)   298359 2022-11-21 14:54:36.000000 nonos-0.9.1/tests/data/idefix_newvtk_planet2d/data.0023.vtk
+-rw-rw-r--   0 wafflarg  (1001) wafflarg  (1001)     1007 2022-11-21 14:54:36.000000 nonos-0.9.1/tests/data/idefix_newvtk_planet2d/idefix.ini
+-rw-rw-r--   0 wafflarg  (1001) wafflarg  (1001)     3717 2022-11-21 14:54:36.000000 nonos-0.9.1/tests/data/idefix_newvtk_planet2d/planet0.dat
+drwxrwxr-x   0 wafflarg  (1001) wafflarg  (1001)        0 2023-07-31 15:30:05.765287 nonos-0.9.1/tests/data/idefix_planet3d/
+-rw-rw-r--   0 wafflarg  (1001) wafflarg  (1001)  7490113 2021-03-30 18:17:30.000000 nonos-0.9.1/tests/data/idefix_planet3d/data.0000.vtk
+-rw-rw-r--   0 wafflarg  (1001) wafflarg  (1001)  7490113 2021-03-30 18:22:00.000000 nonos-0.9.1/tests/data/idefix_planet3d/data.0043.vtk
+-rwxrwxr-x   0 wafflarg  (1001) wafflarg  (1001)      213 2022-11-21 14:54:36.000000 nonos-0.9.1/tests/data/idefix_planet3d/definitions.hpp
+-rw-rw-r--   0 wafflarg  (1001) wafflarg  (1001)      805 2022-11-21 14:54:36.000000 nonos-0.9.1/tests/data/idefix_planet3d/idefix.ini
+-rw-rw-r--   0 wafflarg  (1001) wafflarg  (1001)    11155 2021-03-30 18:24:51.000000 nonos-0.9.1/tests/data/idefix_planet3d/planet0.dat
+drwxrwxr-x   0 wafflarg  (1001) wafflarg  (1001)        0 2023-07-31 15:30:05.769287 nonos-0.9.1/tests/data/idefix_rwi/
+-rw-rw-r--   0 wafflarg  (1001) wafflarg  (1001)  1579289 2021-04-12 13:19:18.000000 nonos-0.9.1/tests/data/idefix_rwi/data.0000.vtk
+-rw-rw-r--   0 wafflarg  (1001) wafflarg  (1001)  1579289 2021-04-12 13:19:18.000000 nonos-0.9.1/tests/data/idefix_rwi/data.0001.vtk
+-rwxrwxr-x   0 wafflarg  (1001) wafflarg  (1001)      213 2022-11-21 14:54:36.000000 nonos-0.9.1/tests/data/idefix_rwi/definitions.hpp
+-rw-rw-r--   0 wafflarg  (1001) wafflarg  (1001)      543 2022-11-21 14:54:36.000000 nonos-0.9.1/tests/data/idefix_rwi/idefix.ini
+-rw-rw-r--   0 wafflarg  (1001) wafflarg  (1001)     3260 2022-11-21 14:54:36.000000 nonos-0.9.1/tests/test_cli.py
+-rw-rw-r--   0 wafflarg  (1001) wafflarg  (1001)      253 2023-06-26 16:17:24.000000 nonos-0.9.1/tests/test_errors.py
+-rw-rw-r--   0 wafflarg  (1001) wafflarg  (1001)     1631 2023-02-02 16:13:07.000000 nonos-0.9.1/tests/test_image_comp.py
+-rw-rw-r--   0 wafflarg  (1001) wafflarg  (1001)     1449 2022-11-21 14:54:36.000000 nonos-0.9.1/tests/test_load_config.py
+-rw-rw-r--   0 wafflarg  (1001) wafflarg  (1001)      763 2022-11-21 14:54:36.000000 nonos-0.9.1/tests/test_params_usage.py
+-rw-rw-r--   0 wafflarg  (1001) wafflarg  (1001)     3541 2023-06-26 16:17:24.000000 nonos-0.9.1/tests/test_parsing.py
+-rw-rw-r--   0 wafflarg  (1001) wafflarg  (1001)     5791 2023-06-27 08:45:04.000000 nonos-0.9.1/tests/test_plotting.py
+-rw-rw-r--   0 wafflarg  (1001) wafflarg  (1001)      604 2023-02-08 18:05:36.000000 nonos-0.9.1/tests/test_readme.py
```

### Comparing `nonos-0.9.0/.github/workflows/ci.yml` & `nonos-0.9.1/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `nonos-0.9.0/.pre-commit-config.yaml` & `nonos-0.9.1/.pre-commit-config.yaml`

 * *Files 3% similar despite different names*

```diff
@@ -10,27 +10,27 @@
   - id: debug-statements
   - id: check-merge-conflict
   - id: trailing-whitespace
   - id: end-of-file-fixer
   - id: check-toml
 
 - repo: https://github.com/neutrinoceros/inifix.git
-  rev: v4.3.2
+  rev: v4.4.0
   hooks:
   - id: inifix-format
 
 - repo: https://github.com/psf/black
   rev: 23.3.0
   hooks:
   - id: black
 
-- repo: https://github.com/charliermarsh/ruff-pre-commit
-  rev: v0.0.260
+- repo: https://github.com/astral-sh/ruff-pre-commit
+  rev: v0.0.276
   hooks:
   - id: ruff
     args: [--fix]
 
 - repo: https://github.com/macisamuele/language-formatters-pre-commit-hooks
-  rev: v2.8.0
+  rev: v2.9.0
   hooks:
   - id: pretty-format-yaml
     args: [--autofix, --indent, '2']
```

### Comparing `nonos-0.9.0/LICENSE` & `nonos-0.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `nonos-0.9.0/PKG-INFO` & `nonos-0.9.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonos
-Version: 0.9.0
+Version: 0.9.1
 Summary: A tool to analyze results from idefix/pluto simulations (for protoplanetary disks more specifically)
 Author: G. Wafflard-Fernandez, C.M.T. Robert
 License: GPL-3.0
 Project-URL: Homepage, https://github.com/volodia99/nonos
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
```

### Comparing `nonos-0.9.0/README.md` & `nonos-0.9.1/README.md`

 * *Files identical despite different names*

### Comparing `nonos-0.9.0/nonos/api/_adapt_clm_vtk.py` & `nonos-0.9.1/nonos/api/_adapt_clm_vtk.py`

 * *Files identical despite different names*

### Comparing `nonos-0.9.0/nonos/api/analysis.py` & `nonos-0.9.1/nonos/api/analysis.py`

 * *Files 10% similar despite different names*

```diff
@@ -1464,149 +1464,7 @@
     def items(self):
         """
         Returns
         =======
         items of the dict
         """
         return self.dict.items()
-
-
-def from_file(*, field: str, filename: str, on: int, directory=""):
-    repout = field.lower()
-    headername = os.path.join(directory, "header", f"header_{filename}.npy")
-    with open(headername, "rb") as file:
-        dict_coords = np.load(file, allow_pickle=True).item()
-
-    geometry, coord0, coord1, coord2 = dict_coords.values()
-    ret_coords = Coordinates(geometry, coord0, coord1, coord2)
-
-    fileout = os.path.join(directory, repout, f"_{filename}_{field}.{on:04d}.npy")
-    with open(fileout, "rb") as file:
-        ret_data = np.load(file, allow_pickle=True)
-
-    return GasField(
-        field,
-        ret_data,
-        ret_coords,
-        geometry,
-        on,
-        operation=filename,
-        directory=directory,
-    )
-
-
-def from_data(
-    *,
-    field: str,
-    data: np.ndarray,
-    coords: Coordinates,
-    on: int,
-    operation: str,
-    inifile: str = "",
-    code: str = "",
-    directory: str = "",
-    rotate_grid: int = -1,
-):
-    ret_data = data
-    ret_coords = coords
-    geometry = coords.geometry
-    return GasField(
-        field,
-        ret_data,
-        ret_coords,
-        geometry,
-        on,
-        operation=operation,
-        inifile=inifile,
-        code=code,
-        directory=directory,
-        rotate_grid=rotate_grid,
-    )
-
-
-def temporal_all(
-    field: str,
-    operation: str,
-    onall,
-    directory: str = "",
-    planet_corotation: Optional[int] = None,
-):
-    datasum = 0
-    don = len(onall)
-    for on in sorted(onall):
-        datafield = from_file(
-            field=field, filename=operation, on=on, directory=directory
-        )
-        if planet_corotation is not None:
-            datafield_rot = datafield.rotate(planet_corotation=planet_corotation)
-            datasum += datafield_rot.data
-        else:
-            datasum += datafield.data
-    datafieldsum = from_data(
-        field="".join([field, "T_ALL"]),
-        data=np.array(datasum / don),
-        coords=datafield.coords,
-        on=0,
-        operation="_" + operation,
-        directory=directory,
-        rotate_grid=datafield.rotate_grid,
-    )
-    return datafieldsum
-
-
-def temporal(
-    field: str,
-    operation: str,
-    onbeg: int,
-    *,
-    onend: Optional[int] = None,
-    directory: str = "",
-    planet_corotation: Optional[int] = None,
-):
-    datasum = 0
-    if onend is None:
-        datafield = from_file(
-            field=field, filename=operation, on=onbeg, directory=directory
-        )
-        if planet_corotation is not None:
-            datafield_rot = datafield.rotate(planet_corotation=planet_corotation)
-            datafieldsum = from_data(
-                field=field,
-                data=datafield_rot.data,
-                coords=datafield_rot.coords,
-                on=onbeg,
-                operation="_" + operation,
-                directory=directory,
-                rotate_grid=datafield_rot.rotate_grid,
-            )
-        else:
-            datafieldsum = from_data(
-                field=field,
-                data=datafield.data,
-                coords=datafield.coords,
-                on=onbeg,
-                operation="_" + operation,
-                directory=directory,
-                rotate_grid=datafield.rotate_grid,
-            )
-        return datafieldsum
-    else:
-        don = onend - onbeg
-        for on in range(onbeg, onend + 1):
-            datafield = from_file(
-                field=field, filename=operation, on=on, directory=directory
-            )
-            if planet_corotation is not None:
-                datafield_rot = datafield.rotate(planet_corotation=planet_corotation)
-                datasum += datafield_rot.data
-            else:
-                datasum += datafield.data
-        datafieldsum = from_data(
-            field="".join([field, f"T_{onbeg}_{onend}"]),
-            data=np.array(datasum / don),
-            coords=datafield.coords,
-            on=onend,
-            operation="_" + operation,
-            directory=directory,
-            rotate_grid=datafield.rotate_grid,
-        )
-        return datafieldsum
```

### Comparing `nonos-0.9.0/nonos/api/from_simulation.py` & `nonos-0.9.1/nonos/api/from_simulation.py`

 * *Files identical despite different names*

### Comparing `nonos-0.9.0/nonos/api/satellite.py` & `nonos-0.9.1/nonos/api/satellite.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import os
 import warnings
-from typing import Any, Dict, List, Optional, Tuple
+from typing import Optional
 
 import numpy as np
 from lick.lick import lick_box
 
-from nonos.api.analysis import GasField, Plotable, temporal
+from nonos.api.analysis import Coordinates, GasField, Plotable
 from nonos.api.from_simulation import Parameters
 
 
 def file_analysis(filename, *, inifile="", code="", directory="", norb=None):
     from scipy.ndimage import uniform_filter1d
 
     columns = np.loadtxt(os.path.join(directory, filename), dtype="float64").T
@@ -37,85 +37,14 @@
         )
     init = Parameters(inifile=inifile, code=code, directory=directory)
     init.loadIniFile()
     init.loadPlanetFile(planet_number=planet_number)
     return init
 
 
-def save_temporal(
-    field: str,
-    onbeg: int,
-    onend: int,
-    operation: str,
-    *,
-    directory: str = "",
-    planet_corotation=0,
-):
-    temporal_evolution = temporal(
-        field,
-        operation,
-        onbeg,
-        onend=onend,
-        directory=directory,
-        planet_corotation=planet_corotation,
-    ).save(directory=directory)
-    return temporal_evolution
-
-
-def load_fields(
-    field_operation: Dict[str, Any],
-    fields: List[str],
-    operations: List[Tuple[str, str]],
-    onbeg: int,
-    onend: int,
-    *,
-    directory: str = "",
-    temporal_bool: bool = True,
-    snapshot_bool: bool = True,
-    planet_corotation=0,
-):
-    for field in fields:
-        for operation, operation_shortcut in operations:
-            if snapshot_bool:
-                field_operation[f"{field}{operation_shortcut}"] = temporal(
-                    field,
-                    operation,
-                    onend,
-                    onend=None,
-                    directory=directory,
-                    planet_corotation=planet_corotation,
-                )
-            if temporal_bool:
-                try:
-                    field_operation[f"{field}T{operation_shortcut}"] = temporal(
-                        f"{field}T_{onbeg}_{onend}",
-                        operation,
-                        onend,
-                        onend=None,
-                        directory=directory,
-                    )
-                except FileNotFoundError:
-                    save_temporal(
-                        field,
-                        onbeg,
-                        onend,
-                        operation,
-                        directory=directory,
-                        planet_corotation=planet_corotation,
-                    )
-                    field_operation[f"{field}T{operation_shortcut}"] = temporal(
-                        f"{field}T_{onbeg}_{onend}",
-                        operation,
-                        onend,
-                        onend=None,
-                        directory=directory,
-                    )
-    return field_operation
-
-
 class NonosLick:
     def __init__(
         self,
         x: np.ndarray,
         y: np.ndarray,
         lx: GasField,
         ly: GasField,
@@ -242,7 +171,60 @@
         ref.on,
         operation=ref.operation,
         inifile=ref.inifile,
         code=ref.code,
         directory=ref.directory,
         rotate_grid=ref._rotate_grid,
     )
+
+
+def from_data(
+    *,
+    field: str,
+    data: np.ndarray,
+    coords: Coordinates,
+    on: int,
+    operation: str,
+    inifile: str = "",
+    code: str = "",
+    directory: str = "",
+    rotate_grid: int = -1,
+):
+    ret_data = data
+    ret_coords = coords
+    geometry = coords.geometry
+    return GasField(
+        field,
+        ret_data,
+        ret_coords,
+        geometry,
+        on,
+        operation=operation,
+        inifile=inifile,
+        code=code,
+        directory=directory,
+        rotate_grid=rotate_grid,
+    )
+
+
+def from_file(*, field: str, operation: str, on: int, directory=""):
+    repout = field.lower()
+    headername = os.path.join(directory, "header", f"header_{operation}.npy")
+    with open(headername, "rb") as file:
+        dict_coords = np.load(file, allow_pickle=True).item()
+
+    geometry, coord0, coord1, coord2 = dict_coords.values()
+    ret_coords = Coordinates(geometry, coord0, coord1, coord2)
+
+    fileout = os.path.join(directory, repout, f"_{operation}_{field}.{on:04d}.npy")
+    with open(fileout, "rb") as file:
+        ret_data = np.load(file, allow_pickle=True)
+
+    return GasField(
+        field,
+        ret_data,
+        ret_coords,
+        geometry,
+        on,
+        operation=operation,
+        directory=directory,
+    )
```

### Comparing `nonos-0.9.0/nonos/config.py` & `nonos-0.9.1/nonos/config.py`

 * *Files identical despite different names*

### Comparing `nonos-0.9.0/nonos/logging.py` & `nonos-0.9.1/nonos/logging.py`

 * *Files identical despite different names*

### Comparing `nonos-0.9.0/nonos/logo.txt` & `nonos-0.9.1/nonos/logo.txt`

 * *Files identical despite different names*

### Comparing `nonos-0.9.0/nonos/main.py` & `nonos-0.9.1/nonos/main.py`

 * *Files identical despite different names*

### Comparing `nonos-0.9.0/nonos/parsing.py` & `nonos-0.9.1/nonos/parsing.py`

 * *Files identical despite different names*

### Comparing `nonos-0.9.0/nonos/styling.py` & `nonos-0.9.1/nonos/styling.py`

 * *Files identical despite different names*

### Comparing `nonos-0.9.0/nonos.egg-info/PKG-INFO` & `nonos-0.9.1/nonos.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonos
-Version: 0.9.0
+Version: 0.9.1
 Summary: A tool to analyze results from idefix/pluto simulations (for protoplanetary disks more specifically)
 Author: G. Wafflard-Fernandez, C.M.T. Robert
 License: GPL-3.0
 Project-URL: Homepage, https://github.com/volodia99/nonos
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
```

### Comparing `nonos-0.9.0/nonos.egg-info/SOURCES.txt` & `nonos-0.9.1/nonos.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nonos-0.9.0/pyproject.toml` & `nonos-0.9.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `nonos-0.9.0/tests/conftest.py` & `nonos-0.9.1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `nonos-0.9.0/tests/data/fargo3d_planet2d/domain_x.dat` & `nonos-0.9.1/tests/data/fargo3d_planet2d/domain_x.dat`

 * *Files identical despite different names*

### Comparing `nonos-0.9.0/tests/data/fargo3d_planet2d/domain_y.dat` & `nonos-0.9.1/tests/data/fargo3d_planet2d/domain_y.dat`

 * *Files identical despite different names*

### Comparing `nonos-0.9.0/tests/data/fargo3d_planet2d/gasdens0.dat` & `nonos-0.9.1/tests/data/fargo3d_planet2d/gasdens0.dat`

 * *Files identical despite different names*

### Comparing `nonos-0.9.0/tests/data/fargo3d_planet2d/gasdens40.dat` & `nonos-0.9.1/tests/data/fargo3d_planet2d/gasdens40.dat`

 * *Files identical despite different names*

### Comparing `nonos-0.9.0/tests/data/fargo3d_planet2d/gasvy40.dat` & `nonos-0.9.1/tests/data/fargo3d_planet2d/gasvy40.dat`

 * *Files identical despite different names*

### Comparing `nonos-0.9.0/tests/data/fargo3d_planet2d/planet0.dat` & `nonos-0.9.1/tests/data/fargo3d_planet2d/planet0.dat`

 * *Files identical despite different names*

### Comparing `nonos-0.9.0/tests/data/fargo3d_planet2d/variables.par` & `nonos-0.9.1/tests/data/fargo3d_planet2d/variables.par`

 * *Files identical despite different names*

### Comparing `nonos-0.9.0/tests/data/idefix_newvtk_planet2d/data.0000.vtk` & `nonos-0.9.1/tests/data/idefix_newvtk_planet2d/data.0000.vtk`

 * *Files identical despite different names*

### Comparing `nonos-0.9.0/tests/data/idefix_newvtk_planet2d/data.0023.vtk` & `nonos-0.9.1/tests/data/idefix_newvtk_planet2d/data.0023.vtk`

 * *Files identical despite different names*

### Comparing `nonos-0.9.0/tests/data/idefix_newvtk_planet2d/idefix.ini` & `nonos-0.9.1/tests/data/idefix_newvtk_planet2d/idefix.ini`

 * *Files identical despite different names*

### Comparing `nonos-0.9.0/tests/data/idefix_newvtk_planet2d/planet0.dat` & `nonos-0.9.1/tests/data/idefix_newvtk_planet2d/planet0.dat`

 * *Files identical despite different names*

### Comparing `nonos-0.9.0/tests/data/idefix_planet3d/data.0000.vtk` & `nonos-0.9.1/tests/data/idefix_planet3d/data.0000.vtk`

 * *Files identical despite different names*

### Comparing `nonos-0.9.0/tests/data/idefix_planet3d/data.0043.vtk` & `nonos-0.9.1/tests/data/idefix_planet3d/data.0043.vtk`

 * *Files identical despite different names*

### Comparing `nonos-0.9.0/tests/data/idefix_planet3d/idefix.ini` & `nonos-0.9.1/tests/data/idefix_planet3d/idefix.ini`

 * *Files identical despite different names*

### Comparing `nonos-0.9.0/tests/data/idefix_planet3d/planet0.dat` & `nonos-0.9.1/tests/data/idefix_planet3d/planet0.dat`

 * *Files identical despite different names*

### Comparing `nonos-0.9.0/tests/data/idefix_rwi/data.0000.vtk` & `nonos-0.9.1/tests/data/idefix_rwi/data.0000.vtk`

 * *Files identical despite different names*

### Comparing `nonos-0.9.0/tests/data/idefix_rwi/data.0001.vtk` & `nonos-0.9.1/tests/data/idefix_rwi/data.0001.vtk`

 * *Files identical despite different names*

### Comparing `nonos-0.9.0/tests/data/idefix_rwi/idefix.ini` & `nonos-0.9.1/tests/data/idefix_rwi/idefix.ini`

 * *Files identical despite different names*

### Comparing `nonos-0.9.0/tests/test_cli.py` & `nonos-0.9.1/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `nonos-0.9.0/tests/test_image_comp.py` & `nonos-0.9.1/tests/test_image_comp.py`

 * *Files identical despite different names*

### Comparing `nonos-0.9.0/tests/test_load_config.py` & `nonos-0.9.1/tests/test_load_config.py`

 * *Files identical despite different names*

### Comparing `nonos-0.9.0/tests/test_params_usage.py` & `nonos-0.9.1/tests/test_params_usage.py`

 * *Files identical despite different names*

### Comparing `nonos-0.9.0/tests/test_parsing.py` & `nonos-0.9.1/tests/test_parsing.py`

 * *Files identical despite different names*

### Comparing `nonos-0.9.0/tests/test_plotting.py` & `nonos-0.9.1/tests/test_plotting.py`

 * *Files identical despite different names*

### Comparing `nonos-0.9.0/tests/test_readme.py` & `nonos-0.9.1/tests/test_readme.py`

 * *Files identical despite different names*

