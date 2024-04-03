# Comparing `tmp/voxcell-3.1.7.tar.gz` & `tmp/voxcell-3.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "voxcell-3.1.7.tar", last modified: Mon Mar 25 13:31:26 2024, max compression
+gzip compressed data, was "voxcell-3.1.8.tar", last modified: Wed Apr  3 13:57:03 2024, max compression
```

## Comparing `voxcell-3.1.7.tar` & `voxcell-3.1.8.tar`

### file list

```diff
@@ -1,97 +1,97 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 13:31:26.129420 voxcell-3.1.7/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 13:31:26.117420 voxcell-3.1.7/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 13:31:26.121420 voxcell-3.1.7/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      618 2024-03-25 13:31:22.000000 voxcell-3.1.7/.github/workflows/publish-sdist.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1554 2024-03-25 13:31:22.000000 voxcell-3.1.7/.github/workflows/run-tox.yml
--rw-r--r--   0 runner    (1001) docker     (127)      114 2024-03-25 13:31:22.000000 voxcell-3.1.7/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1583 2024-03-25 13:31:22.000000 voxcell-3.1.7/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (127)      367 2024-03-25 13:31:22.000000 voxcell-3.1.7/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      309 2024-03-25 13:31:22.000000 voxcell-3.1.7/AUTHORS.txt
--rw-r--r--   0 runner    (1001) docker     (127)     5071 2024-03-25 13:31:22.000000 voxcell-3.1.7/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1005 2024-03-25 13:31:22.000000 voxcell-3.1.7/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (127)    11363 2024-03-25 13:31:22.000000 voxcell-3.1.7/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-03-25 13:31:22.000000 voxcell-3.1.7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     4092 2024-03-25 13:31:26.129420 voxcell-3.1.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2648 2024-03-25 13:31:22.000000 voxcell-3.1.7/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 13:31:26.121420 voxcell-3.1.7/doc/
--rw-r--r--   0 runner    (1001) docker     (127)     1490 2024-03-25 13:31:22.000000 voxcell-3.1.7/doc/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 13:31:26.121420 voxcell-3.1.7/doc/source/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 13:31:26.121420 voxcell-3.1.7/doc/source/_static/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-25 13:31:22.000000 voxcell-3.1.7/doc/source/_static/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     2356 2024-03-25 13:31:22.000000 voxcell-3.1.7/doc/source/aibs.rst
--rw-r--r--   0 runner    (1001) docker     (127)      529 2024-03-25 13:31:22.000000 voxcell-3.1.7/doc/source/api.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 13:31:26.121420 voxcell-3.1.7/doc/source/assets/
--rw-r--r--   0 runner    (1001) docker     (127)    45749 2024-03-25 13:31:22.000000 voxcell-3.1.7/doc/source/assets/combined_dist.png
--rw-r--r--   0 runner    (1001) docker     (127)    32876 2024-03-25 13:31:22.000000 voxcell-3.1.7/doc/source/assets/size_dist.png
--rw-r--r--   0 runner    (1001) docker     (127)     8539 2024-03-25 13:31:22.000000 voxcell-3.1.7/doc/source/atlas.rst
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-03-25 13:31:22.000000 voxcell-3.1.7/doc/source/changelog.rst
--rw-r--r--   0 runner    (1001) docker     (127)     7626 2024-03-25 13:31:22.000000 voxcell-3.1.7/doc/source/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 13:31:26.117420 voxcell-3.1.7/doc/source/extensions/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 13:31:26.121420 voxcell-3.1.7/doc/source/extensions/bbp-table/
--rw-r--r--   0 runner    (1001) docker     (127)     4442 2024-03-25 13:31:22.000000 voxcell-3.1.7/doc/source/extensions/bbp-table/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4821 2024-03-25 13:31:22.000000 voxcell-3.1.7/doc/source/extras.rst
--rw-r--r--   0 runner    (1001) docker     (127)       97 2024-03-25 13:31:22.000000 voxcell-3.1.7/doc/source/formats.rst
--rw-r--r--   0 runner    (1001) docker     (127)      575 2024-03-25 13:31:22.000000 voxcell-3.1.7/doc/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)      172 2024-03-25 13:31:22.000000 voxcell-3.1.7/doc/source/install.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2423 2024-03-25 13:31:22.000000 voxcell-3.1.7/doc/source/mask.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2862 2024-03-25 13:31:22.000000 voxcell-3.1.7/doc/source/orientation.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2519 2024-03-25 13:31:22.000000 voxcell-3.1.7/doc/source/scalar.rst
--rw-r--r--   0 runner    (1001) docker     (127)      260 2024-03-25 13:31:22.000000 voxcell-3.1.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-25 13:31:26.129420 voxcell-3.1.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1471 2024-03-25 13:31:22.000000 voxcell-3.1.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 13:31:26.125420 voxcell-3.1.7/tests/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 13:31:26.125420 voxcell-3.1.7/tests/data/
--rw-r--r--   0 runner    (1001) docker     (127)     2186 2024-03-25 13:31:22.000000 voxcell-3.1.7/tests/data/hierarchy.json
--rw-r--r--   0 runner    (1001) docker     (127)      234 2024-03-25 13:31:22.000000 voxcell-3.1.7/tests/data/metadata.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 13:31:26.125420 voxcell-3.1.7/tests/data/mvd2_mvd3/
--rw-r--r--   0 runner    (1001) docker     (127)      366 2024-03-25 13:31:22.000000 voxcell-3.1.7/tests/data/mvd2_mvd3/README.txt
--rw-r--r--   0 runner    (1001) docker     (127)   153026 2024-03-25 13:31:22.000000 voxcell-3.1.7/tests/data/mvd2_mvd3/circuit.mvd2
--rw-r--r--   0 runner    (1001) docker     (127)   175072 2024-03-25 13:31:22.000000 voxcell-3.1.7/tests/data/mvd2_mvd3/circuit.mvd3
--rw-r--r--   0 runner    (1001) docker     (127)      327 2024-03-25 13:31:22.000000 voxcell-3.1.7/tests/data/no_spacings_fail.nrrd
--rw-r--r--   0 runner    (1001) docker     (127)     1372 2024-03-25 13:31:22.000000 voxcell-3.1.7/tests/data/region_map.json
--rw-r--r--   0 runner    (1001) docker     (127)      354 2024-03-25 13:31:22.000000 voxcell-3.1.7/tests/data/scalar.nrrd
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 13:31:26.129420 voxcell-3.1.7/tests/data/sonata/
--rw-r--r--   0 runner    (1001) docker     (127)    40840 2024-03-25 13:31:22.000000 voxcell-3.1.7/tests/data/sonata/nodes_eulers.h5
--rw-r--r--   0 runner    (1001) docker     (127)    13136 2024-03-25 13:31:22.000000 voxcell-3.1.7/tests/data/sonata/nodes_multi_types.h5
--rw-r--r--   0 runner    (1001) docker     (127)    12904 2024-03-25 13:31:22.000000 voxcell-3.1.7/tests/data/sonata/nodes_no_rotation.h5
--rw-r--r--   0 runner    (1001) docker     (127)    28912 2024-03-25 13:31:22.000000 voxcell-3.1.7/tests/data/sonata/nodes_quaternions.h5
--rw-r--r--   0 runner    (1001) docker     (127)    14224 2024-03-25 13:31:22.000000 voxcell-3.1.7/tests/data/sonata/nodes_quaternions_w_missing.h5
--rw-r--r--   0 runner    (1001) docker     (127)      372 2024-03-25 13:31:22.000000 voxcell-3.1.7/tests/data/space_directions.nrrd
--rw-r--r--   0 runner    (1001) docker     (127)      369 2024-03-25 13:31:22.000000 voxcell-3.1.7/tests/data/space_directions_fail.nrrd
--rw-r--r--   0 runner    (1001) docker     (127)      346 2024-03-25 13:31:22.000000 voxcell-3.1.7/tests/data/vector.nrrd
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 13:31:26.129420 voxcell-3.1.7/tests/sonata/
--rw-r--r--   0 runner    (1001) docker     (127)      200 2024-03-25 13:31:22.000000 voxcell-3.1.7/tests/sonata/test_node_population.py
--rw-r--r--   0 runner    (1001) docker     (127)    18412 2024-03-25 13:31:22.000000 voxcell-3.1.7/tests/test_cell_collection.py
--rw-r--r--   0 runner    (1001) docker     (127)    16706 2024-03-25 13:31:22.000000 voxcell-3.1.7/tests/test_math_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     5734 2024-03-25 13:31:22.000000 voxcell-3.1.7/tests/test_quaternion.py
--rw-r--r--   0 runner    (1001) docker     (127)     4855 2024-03-25 13:31:22.000000 voxcell-3.1.7/tests/test_region_map.py
--rw-r--r--   0 runner    (1001) docker     (127)    13325 2024-03-25 13:31:22.000000 voxcell-3.1.7/tests/test_traits.py
--rw-r--r--   0 runner    (1001) docker     (127)     3243 2024-03-25 13:31:22.000000 voxcell-3.1.7/tests/test_vector_fields.py
--rw-r--r--   0 runner    (1001) docker     (127)    16004 2024-03-25 13:31:22.000000 voxcell-3.1.7/tests/test_voxel_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     5403 2024-03-25 13:31:22.000000 voxcell-3.1.7/tests/test_voxelbrain.py
--rw-r--r--   0 runner    (1001) docker     (127)     1214 2024-03-25 13:31:22.000000 voxcell-3.1.7/tox.ini
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 13:31:26.129420 voxcell-3.1.7/voxcell/
--rw-r--r--   0 runner    (1001) docker     (127)      295 2024-03-25 13:31:22.000000 voxcell-3.1.7/voxcell/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    20040 2024-03-25 13:31:22.000000 voxcell-3.1.7/voxcell/cell_collection.py
--rw-r--r--   0 runner    (1001) docker     (127)      120 2024-03-25 13:31:22.000000 voxcell-3.1.7/voxcell/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     8835 2024-03-25 13:31:22.000000 voxcell-3.1.7/voxcell/math_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 13:31:26.129420 voxcell-3.1.7/voxcell/nexus/
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-03-25 13:31:22.000000 voxcell-3.1.7/voxcell/nexus/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12854 2024-03-25 13:31:22.000000 voxcell-3.1.7/voxcell/nexus/voxelbrain.py
--rw-r--r--   0 runner    (1001) docker     (127)     3755 2024-03-25 13:31:22.000000 voxcell-3.1.7/voxcell/quaternion.py
--rw-r--r--   0 runner    (1001) docker     (127)     6924 2024-03-25 13:31:22.000000 voxcell-3.1.7/voxcell/region_map.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 13:31:26.129420 voxcell-3.1.7/voxcell/sonata/
--rw-r--r--   0 runner    (1001) docker     (127)      188 2024-03-25 13:31:22.000000 voxcell-3.1.7/voxcell/sonata/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      378 2024-03-25 13:31:22.000000 voxcell-3.1.7/voxcell/sonata/node_population.py
--rw-r--r--   0 runner    (1001) docker     (127)    12823 2024-03-25 13:31:22.000000 voxcell-3.1.7/voxcell/traits.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 13:31:26.129420 voxcell-3.1.7/voxcell/utils/
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-03-25 13:31:22.000000 voxcell-3.1.7/voxcell/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      475 2024-03-25 13:31:22.000000 voxcell-3.1.7/voxcell/utils/deprecate.py
--rw-r--r--   0 runner    (1001) docker     (127)     3573 2024-03-25 13:31:22.000000 voxcell-3.1.7/voxcell/vector_fields.py
--rw-r--r--   0 runner    (1001) docker     (127)    19317 2024-03-25 13:31:22.000000 voxcell-3.1.7/voxcell/voxel_data.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 13:31:26.129420 voxcell-3.1.7/voxcell.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4092 2024-03-25 13:31:26.000000 voxcell-3.1.7/voxcell.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1922 2024-03-25 13:31:26.000000 voxcell-3.1.7/voxcell.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-25 13:31:26.000000 voxcell-3.1.7/voxcell.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      111 2024-03-25 13:31:26.000000 voxcell-3.1.7/voxcell.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-03-25 13:31:26.000000 voxcell-3.1.7/voxcell.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 13:57:03.725449 voxcell-3.1.8/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 13:57:03.713449 voxcell-3.1.8/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 13:57:03.717449 voxcell-3.1.8/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      618 2024-04-03 13:56:59.000000 voxcell-3.1.8/.github/workflows/publish-sdist.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1554 2024-04-03 13:56:59.000000 voxcell-3.1.8/.github/workflows/run-tox.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      114 2024-04-03 13:56:59.000000 voxcell-3.1.8/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1583 2024-04-03 13:56:59.000000 voxcell-3.1.8/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (127)      367 2024-04-03 13:56:59.000000 voxcell-3.1.8/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      309 2024-04-03 13:56:59.000000 voxcell-3.1.8/AUTHORS.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     5071 2024-04-03 13:56:59.000000 voxcell-3.1.8/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1005 2024-04-03 13:56:59.000000 voxcell-3.1.8/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    11363 2024-04-03 13:56:59.000000 voxcell-3.1.8/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-03 13:56:59.000000 voxcell-3.1.8/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     4092 2024-04-03 13:57:03.725449 voxcell-3.1.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2648 2024-04-03 13:56:59.000000 voxcell-3.1.8/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 13:57:03.717449 voxcell-3.1.8/doc/
+-rw-r--r--   0 runner    (1001) docker     (127)     1490 2024-04-03 13:56:59.000000 voxcell-3.1.8/doc/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 13:57:03.717449 voxcell-3.1.8/doc/source/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 13:57:03.721449 voxcell-3.1.8/doc/source/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 13:56:59.000000 voxcell-3.1.8/doc/source/_static/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     2356 2024-04-03 13:56:59.000000 voxcell-3.1.8/doc/source/aibs.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      529 2024-04-03 13:56:59.000000 voxcell-3.1.8/doc/source/api.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 13:57:03.721449 voxcell-3.1.8/doc/source/assets/
+-rw-r--r--   0 runner    (1001) docker     (127)    45749 2024-04-03 13:56:59.000000 voxcell-3.1.8/doc/source/assets/combined_dist.png
+-rw-r--r--   0 runner    (1001) docker     (127)    32876 2024-04-03 13:56:59.000000 voxcell-3.1.8/doc/source/assets/size_dist.png
+-rw-r--r--   0 runner    (1001) docker     (127)     8539 2024-04-03 13:56:59.000000 voxcell-3.1.8/doc/source/atlas.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-03 13:56:59.000000 voxcell-3.1.8/doc/source/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     7626 2024-04-03 13:56:59.000000 voxcell-3.1.8/doc/source/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 13:57:03.713449 voxcell-3.1.8/doc/source/extensions/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 13:57:03.721449 voxcell-3.1.8/doc/source/extensions/bbp-table/
+-rw-r--r--   0 runner    (1001) docker     (127)     4442 2024-04-03 13:56:59.000000 voxcell-3.1.8/doc/source/extensions/bbp-table/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4821 2024-04-03 13:56:59.000000 voxcell-3.1.8/doc/source/extras.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       97 2024-04-03 13:56:59.000000 voxcell-3.1.8/doc/source/formats.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      575 2024-04-03 13:56:59.000000 voxcell-3.1.8/doc/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      172 2024-04-03 13:56:59.000000 voxcell-3.1.8/doc/source/install.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2423 2024-04-03 13:56:59.000000 voxcell-3.1.8/doc/source/mask.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2862 2024-04-03 13:56:59.000000 voxcell-3.1.8/doc/source/orientation.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2519 2024-04-03 13:56:59.000000 voxcell-3.1.8/doc/source/scalar.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      260 2024-04-03 13:56:59.000000 voxcell-3.1.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-03 13:57:03.725449 voxcell-3.1.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1471 2024-04-03 13:56:59.000000 voxcell-3.1.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 13:57:03.721449 voxcell-3.1.8/tests/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 13:57:03.721449 voxcell-3.1.8/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (127)     2186 2024-04-03 13:56:59.000000 voxcell-3.1.8/tests/data/hierarchy.json
+-rw-r--r--   0 runner    (1001) docker     (127)      234 2024-04-03 13:56:59.000000 voxcell-3.1.8/tests/data/metadata.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 13:57:03.721449 voxcell-3.1.8/tests/data/mvd2_mvd3/
+-rw-r--r--   0 runner    (1001) docker     (127)      366 2024-04-03 13:56:59.000000 voxcell-3.1.8/tests/data/mvd2_mvd3/README.txt
+-rw-r--r--   0 runner    (1001) docker     (127)   153026 2024-04-03 13:56:59.000000 voxcell-3.1.8/tests/data/mvd2_mvd3/circuit.mvd2
+-rw-r--r--   0 runner    (1001) docker     (127)   175072 2024-04-03 13:56:59.000000 voxcell-3.1.8/tests/data/mvd2_mvd3/circuit.mvd3
+-rw-r--r--   0 runner    (1001) docker     (127)      327 2024-04-03 13:56:59.000000 voxcell-3.1.8/tests/data/no_spacings_fail.nrrd
+-rw-r--r--   0 runner    (1001) docker     (127)     1404 2024-04-03 13:56:59.000000 voxcell-3.1.8/tests/data/region_map.json
+-rw-r--r--   0 runner    (1001) docker     (127)      354 2024-04-03 13:56:59.000000 voxcell-3.1.8/tests/data/scalar.nrrd
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 13:57:03.725449 voxcell-3.1.8/tests/data/sonata/
+-rw-r--r--   0 runner    (1001) docker     (127)    40840 2024-04-03 13:56:59.000000 voxcell-3.1.8/tests/data/sonata/nodes_eulers.h5
+-rw-r--r--   0 runner    (1001) docker     (127)    13136 2024-04-03 13:56:59.000000 voxcell-3.1.8/tests/data/sonata/nodes_multi_types.h5
+-rw-r--r--   0 runner    (1001) docker     (127)    12904 2024-04-03 13:56:59.000000 voxcell-3.1.8/tests/data/sonata/nodes_no_rotation.h5
+-rw-r--r--   0 runner    (1001) docker     (127)    28912 2024-04-03 13:56:59.000000 voxcell-3.1.8/tests/data/sonata/nodes_quaternions.h5
+-rw-r--r--   0 runner    (1001) docker     (127)    14224 2024-04-03 13:56:59.000000 voxcell-3.1.8/tests/data/sonata/nodes_quaternions_w_missing.h5
+-rw-r--r--   0 runner    (1001) docker     (127)      372 2024-04-03 13:56:59.000000 voxcell-3.1.8/tests/data/space_directions.nrrd
+-rw-r--r--   0 runner    (1001) docker     (127)      369 2024-04-03 13:56:59.000000 voxcell-3.1.8/tests/data/space_directions_fail.nrrd
+-rw-r--r--   0 runner    (1001) docker     (127)      346 2024-04-03 13:56:59.000000 voxcell-3.1.8/tests/data/vector.nrrd
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 13:57:03.725449 voxcell-3.1.8/tests/sonata/
+-rw-r--r--   0 runner    (1001) docker     (127)      200 2024-04-03 13:56:59.000000 voxcell-3.1.8/tests/sonata/test_node_population.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18412 2024-04-03 13:56:59.000000 voxcell-3.1.8/tests/test_cell_collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16706 2024-04-03 13:56:59.000000 voxcell-3.1.8/tests/test_math_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5734 2024-04-03 13:56:59.000000 voxcell-3.1.8/tests/test_quaternion.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6170 2024-04-03 13:56:59.000000 voxcell-3.1.8/tests/test_region_map.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13325 2024-04-03 13:56:59.000000 voxcell-3.1.8/tests/test_traits.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3243 2024-04-03 13:56:59.000000 voxcell-3.1.8/tests/test_vector_fields.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18569 2024-04-03 13:56:59.000000 voxcell-3.1.8/tests/test_voxel_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5403 2024-04-03 13:56:59.000000 voxcell-3.1.8/tests/test_voxelbrain.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1214 2024-04-03 13:56:59.000000 voxcell-3.1.8/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 13:57:03.725449 voxcell-3.1.8/voxcell/
+-rw-r--r--   0 runner    (1001) docker     (127)      295 2024-04-03 13:56:59.000000 voxcell-3.1.8/voxcell/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20040 2024-04-03 13:56:59.000000 voxcell-3.1.8/voxcell/cell_collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)      120 2024-04-03 13:56:59.000000 voxcell-3.1.8/voxcell/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8835 2024-04-03 13:56:59.000000 voxcell-3.1.8/voxcell/math_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 13:57:03.725449 voxcell-3.1.8/voxcell/nexus/
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-03 13:56:59.000000 voxcell-3.1.8/voxcell/nexus/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12854 2024-04-03 13:56:59.000000 voxcell-3.1.8/voxcell/nexus/voxelbrain.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3755 2024-04-03 13:56:59.000000 voxcell-3.1.8/voxcell/quaternion.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9659 2024-04-03 13:56:59.000000 voxcell-3.1.8/voxcell/region_map.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 13:57:03.725449 voxcell-3.1.8/voxcell/sonata/
+-rw-r--r--   0 runner    (1001) docker     (127)      188 2024-04-03 13:56:59.000000 voxcell-3.1.8/voxcell/sonata/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      378 2024-04-03 13:56:59.000000 voxcell-3.1.8/voxcell/sonata/node_population.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12823 2024-04-03 13:56:59.000000 voxcell-3.1.8/voxcell/traits.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 13:57:03.725449 voxcell-3.1.8/voxcell/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-03 13:56:59.000000 voxcell-3.1.8/voxcell/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      475 2024-04-03 13:56:59.000000 voxcell-3.1.8/voxcell/utils/deprecate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3573 2024-04-03 13:56:59.000000 voxcell-3.1.8/voxcell/vector_fields.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20082 2024-04-03 13:56:59.000000 voxcell-3.1.8/voxcell/voxel_data.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 13:57:03.725449 voxcell-3.1.8/voxcell.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4092 2024-04-03 13:57:03.000000 voxcell-3.1.8/voxcell.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1922 2024-04-03 13:57:03.000000 voxcell-3.1.8/voxcell.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 13:57:03.000000 voxcell-3.1.8/voxcell.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      111 2024-04-03 13:57:03.000000 voxcell-3.1.8/voxcell.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-03 13:57:03.000000 voxcell-3.1.8/voxcell.egg-info/top_level.txt
```

### Comparing `voxcell-3.1.7/.github/workflows/publish-sdist.yml` & `voxcell-3.1.8/.github/workflows/publish-sdist.yml`

 * *Files identical despite different names*

### Comparing `voxcell-3.1.7/.github/workflows/run-tox.yml` & `voxcell-3.1.8/.github/workflows/run-tox.yml`

 * *Files identical despite different names*

### Comparing `voxcell-3.1.7/.pylintrc` & `voxcell-3.1.8/.pylintrc`

 * *Files identical despite different names*

### Comparing `voxcell-3.1.7/CHANGELOG.rst` & `voxcell-3.1.8/CHANGELOG.rst`

 * *Files identical despite different names*

### Comparing `voxcell-3.1.7/CONTRIBUTING.rst` & `voxcell-3.1.8/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `voxcell-3.1.7/LICENSE.txt` & `voxcell-3.1.8/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `voxcell-3.1.7/PKG-INFO` & `voxcell-3.1.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: voxcell
-Version: 3.1.7
+Version: 3.1.8
 Summary: Voxcell is a small library to handle probability distributions that have a spatial component and to use them to build collection of cells in space.
 Home-page: https://github.com/BlueBrain/voxcell
 Author: Blue Brain Project, EPFL
 License: Apache-2
 Download-URL: https://github.com/BlueBrain/voxcell
 Description: Overview
         ========
```

### Comparing `voxcell-3.1.7/README.rst` & `voxcell-3.1.8/README.rst`

 * *Files identical despite different names*

### Comparing `voxcell-3.1.7/doc/Makefile` & `voxcell-3.1.8/doc/Makefile`

 * *Files identical despite different names*

### Comparing `voxcell-3.1.7/doc/source/aibs.rst` & `voxcell-3.1.8/doc/source/aibs.rst`

 * *Files identical despite different names*

### Comparing `voxcell-3.1.7/doc/source/api.rst` & `voxcell-3.1.8/doc/source/api.rst`

 * *Files identical despite different names*

### Comparing `voxcell-3.1.7/doc/source/assets/combined_dist.png` & `voxcell-3.1.8/doc/source/assets/combined_dist.png`

 * *Files identical despite different names*

### Comparing `voxcell-3.1.7/doc/source/assets/size_dist.png` & `voxcell-3.1.8/doc/source/assets/size_dist.png`

 * *Files identical despite different names*

### Comparing `voxcell-3.1.7/doc/source/atlas.rst` & `voxcell-3.1.8/doc/source/atlas.rst`

 * *Files identical despite different names*

### Comparing `voxcell-3.1.7/doc/source/conf.py` & `voxcell-3.1.8/doc/source/conf.py`

 * *Files identical despite different names*

### Comparing `voxcell-3.1.7/doc/source/extensions/bbp-table/__init__.py` & `voxcell-3.1.8/doc/source/extensions/bbp-table/__init__.py`

 * *Files identical despite different names*

### Comparing `voxcell-3.1.7/doc/source/extras.rst` & `voxcell-3.1.8/doc/source/extras.rst`

 * *Files identical despite different names*

### Comparing `voxcell-3.1.7/doc/source/index.rst` & `voxcell-3.1.8/doc/source/index.rst`

 * *Files identical despite different names*

### Comparing `voxcell-3.1.7/doc/source/mask.rst` & `voxcell-3.1.8/doc/source/mask.rst`

 * *Files identical despite different names*

### Comparing `voxcell-3.1.7/doc/source/orientation.rst` & `voxcell-3.1.8/doc/source/orientation.rst`

 * *Files identical despite different names*

### Comparing `voxcell-3.1.7/doc/source/scalar.rst` & `voxcell-3.1.8/doc/source/scalar.rst`

 * *Files identical despite different names*

### Comparing `voxcell-3.1.7/setup.py` & `voxcell-3.1.8/setup.py`

 * *Files identical despite different names*

### Comparing `voxcell-3.1.7/tests/data/hierarchy.json` & `voxcell-3.1.8/tests/data/hierarchy.json`

 * *Files identical despite different names*

### Comparing `voxcell-3.1.7/tests/data/mvd2_mvd3/circuit.mvd2` & `voxcell-3.1.8/tests/data/mvd2_mvd3/circuit.mvd2`

 * *Files identical despite different names*

### Comparing `voxcell-3.1.7/tests/data/mvd2_mvd3/circuit.mvd3` & `voxcell-3.1.8/tests/data/mvd2_mvd3/circuit.mvd3`

 * *Files identical despite different names*

### Comparing `voxcell-3.1.7/tests/data/region_map.json` & `voxcell-3.1.8/tests/data/region_map.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999914623318079%*

 * *Differences: {"'children'": "{0: {'children': {0: {'children': {0: {'children': []}}}}}}"}*

```diff
@@ -9,14 +9,15 @@
                 {
                     "acronym": "CH",
                     "atlas_id": 70,
                     "children": [
                         {
                             "acronym": "CTX",
                             "atlas_id": 85,
+                            "children": [],
                             "color_hex_triplet": "B0FFB8",
                             "graph_order": 3,
                             "hemisphere_id": 3,
                             "id": 688,
                             "name": "Cerebral cortex",
                             "ontology_id": 1,
                             "parent_structure_id": 567,
```

### Comparing `voxcell-3.1.7/tests/data/sonata/nodes_eulers.h5` & `voxcell-3.1.8/tests/data/sonata/nodes_eulers.h5`

 * *Files identical despite different names*

### Comparing `voxcell-3.1.7/tests/data/sonata/nodes_multi_types.h5` & `voxcell-3.1.8/tests/data/sonata/nodes_multi_types.h5`

 * *Files identical despite different names*

### Comparing `voxcell-3.1.7/tests/data/sonata/nodes_no_rotation.h5` & `voxcell-3.1.8/tests/data/sonata/nodes_no_rotation.h5`

 * *Files identical despite different names*

### Comparing `voxcell-3.1.7/tests/data/sonata/nodes_quaternions.h5` & `voxcell-3.1.8/tests/data/sonata/nodes_quaternions.h5`

 * *Files identical despite different names*

### Comparing `voxcell-3.1.7/tests/data/sonata/nodes_quaternions_w_missing.h5` & `voxcell-3.1.8/tests/data/sonata/nodes_quaternions_w_missing.h5`

 * *Files identical despite different names*

### Comparing `voxcell-3.1.7/tests/test_cell_collection.py` & `voxcell-3.1.8/tests/test_cell_collection.py`

 * *Files identical despite different names*

### Comparing `voxcell-3.1.7/tests/test_math_utils.py` & `voxcell-3.1.8/tests/test_math_utils.py`

 * *Files identical despite different names*

### Comparing `voxcell-3.1.7/tests/test_quaternion.py` & `voxcell-3.1.8/tests/test_quaternion.py`

 * *Files identical despite different names*

### Comparing `voxcell-3.1.7/tests/test_region_map.py` & `voxcell-3.1.8/tests/test_region_map.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,45 +1,52 @@
 import json
+import os
 from unittest.mock import mock_open, patch
 
 import pytest
 
 import voxcell.region_map as test_module
 from voxcell.exceptions import VoxcellError
 
-TEST_RMAP = test_module.RegionMap.from_dict({
-    'id': -1,
+DATA_PATH = os.path.join(os.path.dirname(__file__), 'data')
+
+TEST_RMAP_DICT = {
+    'id': 0,
     'name': 'root',
     'fullname': 'The Root Node',
     'children': [
         {
         'id': 1,
         'name': 'A',
         'fullname': 'aA',
         'children': [
             {
                 'id': 2,
                 'name': 'B',
                 'fullname': 'Bb',
+                'children': [],
             },
             {
                 'id': 3,
                 'name': 'C',
                 'fullname': 'cC',
                 'children': [
                     {
                         'id': 4,
                         'name': 'B',
                         'fullname': 'bB',
+                        'children': [],
                     }
                 ]
             }
         ]}
     ]
-})
+}
+
+TEST_RMAP = test_module.RegionMap.from_dict(TEST_RMAP_DICT)
 
 
 def test_find_basic():
     assert TEST_RMAP.find('B', 'name') == {2, 4}
     assert TEST_RMAP.find('C', 'name') == {3}
     assert TEST_RMAP.find('cC', attr='fullname') == {3}
 
@@ -152,36 +159,66 @@
                 {
                     'id': 1
                 }
             ]
         })
 
 
+def test_as_dict():
+    res = TEST_RMAP.as_dict()
+    assert res == TEST_RMAP_DICT
+
+    with open(os.path.join(DATA_PATH, "region_map.json")) as f:
+        initial_dict = json.load(f)
+    rmap = test_module.RegionMap.from_dict(initial_dict)
+    assert rmap.as_dict() == initial_dict
+
+
 def test_is_leaf_id():
     assert TEST_RMAP.is_leaf_id(1) is False
     assert TEST_RMAP.is_leaf_id(2) is True
     assert TEST_RMAP.is_leaf_id(3) is False
     assert TEST_RMAP.is_leaf_id(4) is True
 
 
 def test_is_leaf_id_non_existing_id():
     with pytest.raises(VoxcellError):
-        TEST_RMAP.is_leaf_id(0)  # non-existing id
+        TEST_RMAP.is_leaf_id(9999)  # non-existing id
 
 
 def test_as_dataframe():
     df = TEST_RMAP.as_dataframe()
-    assert df.loc[-1].parent_id == -1
-    assert df.loc[1].parent_id == -1
+    assert df.loc[0].parent_id == -1
+    assert df.loc[1].parent_id == 0
     assert df.loc[2].parent_id == 1
     assert df.loc[3].parent_id == 1
     assert df.loc[4].parent_id == 3
 
     assert df.loc[1]['name'] == 'A'
     assert df.loc[1]['fullname'] == 'aA'
 
-    assert df.loc[-1].children_count == 1
+    assert df.loc[0].children_count == 1
     assert df.loc[1].children_count == 2
     assert df.loc[2].children_count == 0
     assert df.loc[3].children_count == 1
     assert df.loc[4].children_count == 0
 
+
+def test_from_dataframe():
+    # Test with a simple RegionMap
+    rmap = test_module.RegionMap.from_dataframe(TEST_RMAP.as_dataframe())
+    assert rmap._data == TEST_RMAP._data
+    assert rmap._parent == TEST_RMAP._parent
+    assert rmap._children == TEST_RMAP._children
+
+    # Test with more complex data
+    initial_rmap = test_module.RegionMap.load_json(os.path.join(DATA_PATH, "region_map.json"))
+    final_rmap = test_module.RegionMap.from_dataframe(initial_rmap.as_dataframe())
+    assert final_rmap._data == initial_rmap._data
+    assert final_rmap._parent == initial_rmap._parent
+    assert final_rmap._children == initial_rmap._children
+
+    # Test with multiple root nodes
+    rmap_df = initial_rmap.as_dataframe()
+    rmap_df.loc[8, "parent_id"] = -1
+    with pytest.raises(RuntimeError):
+        test_module.RegionMap.from_dataframe(rmap_df)
```

### Comparing `voxcell-3.1.7/tests/test_traits.py` & `voxcell-3.1.8/tests/test_traits.py`

 * *Files identical despite different names*

### Comparing `voxcell-3.1.7/tests/test_vector_fields.py` & `voxcell-3.1.8/tests/test_vector_fields.py`

 * *Files identical despite different names*

### Comparing `voxcell-3.1.7/tests/test_voxel_data.py` & `voxcell-3.1.8/tests/test_voxel_data.py`

 * *Files 9% similar despite different names*

```diff
@@ -436,7 +436,86 @@
     npt.assert_array_equal(vtiv.value_to_1d_indices(2), [4, 7])
     npt.assert_array_equal(vtiv.value_to_1d_indices(3), [2, 5, 8])
     npt.assert_array_equal(vtiv.value_to_1d_indices(4), [])
 
     for order in ('K', 'A', 'C', 'F'):
         r = vtiv.ravel(np.array(values, order=order))
         npt.assert_array_equal(r[vtiv.value_to_1d_indices(1)], [1., 1., 1., 1.])
+
+
+def test_ValueToIndexVoxels__raveling():
+
+    # c-contiguous index values
+    index_values = np.array([[1., 2., 3.], [4., 5., 6.], [7., 8., 9.]])
+    index = test_module.ValueToIndexVoxels(index_values)
+    assert index._order == "C"
+    
+    # c-contiguous volume to ravel with a c-order index
+    c_values = np.array([[1., 2., 3.], [4., 5., 6.], [7., 8., 9.]])
+    c_raveled = index.ravel(c_values)
+    c_unraveled = index.unravel(c_raveled)
+
+    # check the reconstruction is correct
+    npt.assert_array_equal(c_unraveled, c_values)
+
+    # should not create a copy
+    assert c_raveled.base is c_values
+    assert c_unraveled.base is c_values
+
+    # f-contiguous volume to ravel with a c-order index
+    f_values = np.asfortranarray(c_values)
+    f_raveled = index.ravel(f_values)
+    f_unraveled = index.unravel(f_raveled)
+
+    # check the reconstruction is correct
+    npt.assert_array_equal(f_unraveled, f_values)
+
+    # should create a copy
+    assert f_raveled.base is None
+    # should not create a copy because 1d array are both C and F contiguous
+    assert f_unraveled.base is f_raveled
+
+    # f-contiguous index values
+    index_values = np.asfortranarray(index_values)
+    index = test_module.ValueToIndexVoxels(index_values)
+    assert index._order == "F"
+
+    # c-contiguous volume to ravel with a f-order index
+    c_values = np.array([[1., 2., 3.], [4., 5., 6.], [7., 8., 9.]])
+    c_raveled = index.ravel(c_values)
+    c_unraveled = index.unravel(c_raveled)
+
+    # check the reconstruction is correct
+    npt.assert_array_equal(c_unraveled, c_values)
+
+    # should create a copy
+    assert c_raveled.base is None
+    # should not create a copy because 1d array are both C and F contiguous
+    assert c_unraveled.base is c_raveled
+
+    # f-contiguous volume to ravel with a f-order index
+    f_values = np.asfortranarray(c_values)
+    f_raveled = index.ravel(f_values)
+    f_unraveled = index.unravel(f_raveled)
+
+    # check the reconstruction is correct
+    npt.assert_array_equal(f_unraveled, f_values)
+
+    # should not create a copy
+    assert f_raveled.base is f_values
+    assert f_unraveled.base is f_values
+
+
+def test_ValueToIndexVoxels__raises():
+
+    index_values = np.array([[1., 2., 3.], [4., 5., 6.], [7., 8., 9.]])
+    index = test_module.ValueToIndexVoxels(index_values)
+
+    data = np.array([[0., 1.], [1., 2]])
+
+    with pytest.raises(VoxcellError, match="Shape mismatch"):
+        index.ravel(data)
+
+    data = np.array([0., 1.])
+
+    with pytest.raises(VoxcellError, match="Array size mismatch"):
+        index.unravel(data)
```

### Comparing `voxcell-3.1.7/tests/test_voxelbrain.py` & `voxcell-3.1.8/tests/test_voxelbrain.py`

 * *Files identical despite different names*

### Comparing `voxcell-3.1.7/tox.ini` & `voxcell-3.1.8/tox.ini`

 * *Files identical despite different names*

### Comparing `voxcell-3.1.7/voxcell/cell_collection.py` & `voxcell-3.1.8/voxcell/cell_collection.py`

 * *Files identical despite different names*

### Comparing `voxcell-3.1.7/voxcell/math_utils.py` & `voxcell-3.1.8/voxcell/math_utils.py`

 * *Files identical despite different names*

### Comparing `voxcell-3.1.7/voxcell/nexus/voxelbrain.py` & `voxcell-3.1.8/voxcell/nexus/voxelbrain.py`

 * *Files identical despite different names*

### Comparing `voxcell-3.1.7/voxcell/quaternion.py` & `voxcell-3.1.8/voxcell/quaternion.py`

 * *Files identical despite different names*

### Comparing `voxcell-3.1.7/voxcell/region_map.py` & `voxcell-3.1.8/voxcell/region_map.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """Region hierarchy tree."""
 
 import copy
 import json
 import logging
 import re
 
+import numpy as np
 import pandas as pd
 
 from voxcell.exceptions import VoxcellError
 
 L = logging.getLogger(__name__)
 
 
@@ -138,14 +139,25 @@
         """
         ret = pd.DataFrame.from_dict(self._data, orient='index').set_index('id')
         parents = {k: v if v is not None else -1 for k, v in self._parent.items()}
         ret.loc[:, 'parent_id'] = pd.DataFrame.from_dict(parents, orient='index')
         ret.loc[:, 'children_count'] = [len(self._children[_id]) for _id in ret.index.to_list()]
         return ret
 
+    @classmethod
+    def from_dataframe(cls, hierarchy_df):
+        """Converts a DataFrame to a region_map.
+
+        Note: the 'root' node should have a parent value of -1.
+
+        Note: if it is possible to cast all non-null values of a column with float dtype to int,
+            then it will be done.
+        """
+        return cls.from_dict(_dataframe_to_dict(hierarchy_df))
+
     def _get(self, _id, attr):
         """Fetch attribute value for a given region ID."""
         if _id not in self._data:
             raise VoxcellError(f"Region ID not found: {_id}")
         node = self._data[_id]
         if attr not in node:
             raise VoxcellError(f"Attribute not found: '{attr}' [region ID = {_id}]")
@@ -181,14 +193,36 @@
             result._children[_id] = [c['id'] for c in children]
             for c in children:
                 include(c, _id)
         result = cls()
         include(copy.deepcopy(d), None)
         return result
 
+    def as_dict(self):
+        """Converts a region_map to a dict."""
+        root_idx = None
+        for k, v in self._parent.items():
+            if v is None:
+                root_idx = k
+                break
+
+        def create_node(key):
+            return copy.deepcopy(self._data[key])
+
+        def add_children(data, key):
+            data["children"] = []
+            for i in self._children[key]:
+                new_node = create_node(i)
+                add_children(new_node, i)
+                data["children"].append(new_node)
+
+        res = create_node(root_idx)
+        add_children(res, root_idx)
+        return res
+
     @classmethod
     def load_json(cls, filepath):
         """Construct RegionMap from JSON file.
 
         Note:
             If top-most object contains 'msg' field, Allen Brain Institute JSON layout is assumed.
         """
@@ -197,7 +231,52 @@
 
         if 'msg' in content:
             if len(content['msg']) > 1:
                 raise VoxcellError("Unexpected JSON layout (more than one 'msg' child)")
             content = content['msg'][0]
 
         return cls.from_dict(content)
+
+
+def _dataframe_to_dict(hierarchy_df):
+    """Use a dataframe to create a dict that can then be used by RegionMap.from_dict()."""
+    nodes = hierarchy_df.to_dict(orient="index")
+    float_cols = hierarchy_df.dtypes.loc[hierarchy_df.dtypes == float].index.to_list()
+    dropna_float_cols = {
+        float_col: hierarchy_df[float_col].dropna()
+        for float_col in float_cols
+    }
+    float_int_cols = {
+        float_col
+        for float_col, col in dropna_float_cols.items()
+        if (col.astype(int) == col).all()
+    }
+    root_idx = None
+    for k, v in nodes.items():
+        v["id"] = k
+        v.pop("children_count", None)
+        parent_id = v.pop("parent_id", None)
+        for float_col in float_cols:
+            if float_col in v:
+                if np.isnan(v[float_col]):
+                    v[float_col] = None
+                elif float_col in float_int_cols:
+                    v[float_col] = int(v[float_col])
+        if parent_id == -1:
+            if root_idx is not None:
+                msg = (
+                    f"Only one node can be the root node with parent_id == -1 but the node "
+                    f"{root_idx} was already defined as root"
+                )
+                raise RuntimeError(msg)
+            root_idx = k
+            if "children" not in v:
+                v["children"] = []
+            continue
+        parent_node = nodes[parent_id]
+        if "children" not in parent_node:
+            parent_node["children"] = []
+        parent_node["children"].append(v)
+
+    # Here the root element is extracted since each element is referenced at both the root of
+    # the dict and in the children of another element
+    return nodes[root_idx]
```

### Comparing `voxcell-3.1.7/voxcell/traits.py` & `voxcell-3.1.8/voxcell/traits.py`

 * *Files identical despite different names*

### Comparing `voxcell-3.1.7/voxcell/vector_fields.py` & `voxcell-3.1.8/voxcell/vector_fields.py`

 * *Files identical despite different names*

### Comparing `voxcell-3.1.7/voxcell/voxel_data.py` & `voxcell-3.1.8/voxcell/voxel_data.py`

 * *Files 4% similar despite different names*

```diff
@@ -427,14 +427,15 @@
     def __init__(self, values):
         """Initialize.
 
         Args:
             values(np.array): volume with each voxel marked with a value; usually to group regions
         """
         self._order = "C" if values.flags["C_CONTIGUOUS"] else "F"
+        self._shape = values.shape
 
         values = values.ravel(order=self._order)
         uniques, counts = np.unique(values, return_counts=True)
 
         offsets = np.empty(len(counts) + 1, dtype=np.uint64)
         offsets[0] = 0
         offsets[1:] = np.cumsum(counts)
@@ -468,17 +469,33 @@
         if value not in self._mapping:
             return np.array([], dtype=self._indices.dtype)
 
         group_index = self._mapping[value]
         return self._indices[self._offsets[group_index]:self._offsets[group_index + 1]]
 
     def ravel(self, voxel_data):
-        """Ensures `voxel_data` matches the layout that the 1D indices can be used."""
+        """Ensure `voxel_data` matches the layout that the 1D indices can be used."""
+        if voxel_data.shape != self._shape:
+            raise VoxcellError(
+                f"Shape mismatch:\n"
+                f"Index initial shape: {self._shape}\n"
+                f"Argument shape: {voxel_data.shape}"
+            )
         return voxel_data.ravel(order=self._order)
 
+    def unravel(self, raveled_voxel_array):
+        """Ensure `raveled_voxel_array` is reshaped with the contiguous order used to be raveled."""
+        if raveled_voxel_array.size != np.prod(self._shape):
+            raise VoxcellError(
+                "Array size mismatch:\n"
+                f"Index initial size: {np.prod(self._shape)}\n"
+                f"Argument size: {raveled_voxel_array.size}"
+            )
+        return raveled_voxel_array.reshape(self._shape, order=self._order)
+
 
 def values_to_region_attribute(values, region_map, attr="acronym"):
     """Convert region ids to the corresponding region attribute.
 
     It can be used to convert the values retrieved with `VoxelData.lookup()`.
 
     Args:
```

### Comparing `voxcell-3.1.7/voxcell.egg-info/PKG-INFO` & `voxcell-3.1.8/voxcell.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: voxcell
-Version: 3.1.7
+Version: 3.1.8
 Summary: Voxcell is a small library to handle probability distributions that have a spatial component and to use them to build collection of cells in space.
 Home-page: https://github.com/BlueBrain/voxcell
 Author: Blue Brain Project, EPFL
 License: Apache-2
 Download-URL: https://github.com/BlueBrain/voxcell
 Description: Overview
         ========
```

### Comparing `voxcell-3.1.7/voxcell.egg-info/SOURCES.txt` & `voxcell-3.1.8/voxcell.egg-info/SOURCES.txt`

 * *Files identical despite different names*

