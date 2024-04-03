# Comparing `tmp/gotranx-0.3.3.tar.gz` & `tmp/gotranx-0.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gotranx-0.3.3.tar", last modified: Wed Mar 13 12:29:42 2024, max compression
+gzip compressed data, was "gotranx-0.3.4.tar", last modified: Wed Apr  3 19:37:17 2024, max compression
```

## Comparing `gotranx-0.3.3.tar` & `gotranx-0.3.4.tar`

### file list

```diff
@@ -1,64 +1,64 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 12:29:42.536748 gotranx-0.3.3/
--rw-r--r--   0 runner    (1001) docker     (127)     7946 2024-03-13 12:29:42.536748 gotranx-0.3.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6146 2024-03-13 12:29:39.000000 gotranx-0.3.3/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     3487 2024-03-13 12:29:39.000000 gotranx-0.3.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-13 12:29:42.536748 gotranx-0.3.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 12:29:42.524748 gotranx-0.3.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 12:29:42.528748 gotranx-0.3.3/src/gotranx/
--rw-r--r--   0 runner    (1001) docker     (127)      947 2024-03-13 12:29:39.000000 gotranx-0.3.3/src/gotranx/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       77 2024-03-13 12:29:39.000000 gotranx-0.3.3/src/gotranx/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6522 2024-03-13 12:29:39.000000 gotranx-0.3.3/src/gotranx/atoms.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 12:29:42.528748 gotranx-0.3.3/src/gotranx/cli/
--rw-r--r--   0 runner    (1001) docker     (127)     3351 2024-03-13 12:29:39.000000 gotranx-0.3.3/src/gotranx/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      773 2024-03-13 12:29:39.000000 gotranx-0.3.3/src/gotranx/cli/cellml2ode.py
--rw-r--r--   0 runner    (1001) docker     (127)     2322 2024-03-13 12:29:39.000000 gotranx-0.3.3/src/gotranx/cli/gotran2c.py
--rw-r--r--   0 runner    (1001) docker     (127)     2357 2024-03-13 12:29:39.000000 gotranx-0.3.3/src/gotranx/cli/gotran2py.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 12:29:42.528748 gotranx-0.3.3/src/gotranx/codegen/
--rw-r--r--   0 runner    (1001) docker     (127)      622 2024-03-13 12:29:39.000000 gotranx-0.3.3/src/gotranx/codegen/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15171 2024-03-13 12:29:39.000000 gotranx-0.3.3/src/gotranx/codegen/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     4273 2024-03-13 12:29:39.000000 gotranx-0.3.3/src/gotranx/codegen/c.py
--rw-r--r--   0 runner    (1001) docker     (127)     5652 2024-03-13 12:29:39.000000 gotranx-0.3.3/src/gotranx/codegen/ode.py
--rw-r--r--   0 runner    (1001) docker     (127)     6008 2024-03-13 12:29:39.000000 gotranx-0.3.3/src/gotranx/codegen/python.py
--rw-r--r--   0 runner    (1001) docker     (127)     2531 2024-03-13 12:29:39.000000 gotranx-0.3.3/src/gotranx/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     4894 2024-03-13 12:29:39.000000 gotranx-0.3.3/src/gotranx/expressions.py
--rw-r--r--   0 runner    (1001) docker     (127)      879 2024-03-13 12:29:39.000000 gotranx-0.3.3/src/gotranx/load.py
--rw-r--r--   0 runner    (1001) docker     (127)     7523 2024-03-13 12:29:39.000000 gotranx-0.3.3/src/gotranx/myokit.py
--rw-r--r--   0 runner    (1001) docker     (127)     2335 2024-03-13 12:29:39.000000 gotranx-0.3.3/src/gotranx/ode.lark
--rw-r--r--   0 runner    (1001) docker     (127)    11529 2024-03-13 12:29:39.000000 gotranx-0.3.3/src/gotranx/ode.py
--rw-r--r--   0 runner    (1001) docker     (127)     7095 2024-03-13 12:29:39.000000 gotranx-0.3.3/src/gotranx/ode_component.py
--rw-r--r--   0 runner    (1001) docker     (127)      334 2024-03-13 12:29:39.000000 gotranx-0.3.3/src/gotranx/parser.py
--rw-r--r--   0 runner    (1001) docker     (127)      601 2024-03-13 12:29:39.000000 gotranx-0.3.3/src/gotranx/save.py
--rw-r--r--   0 runner    (1001) docker     (127)     5073 2024-03-13 12:29:39.000000 gotranx-0.3.3/src/gotranx/schemes.py
--rw-r--r--   0 runner    (1001) docker     (127)     3237 2024-03-13 12:29:39.000000 gotranx-0.3.3/src/gotranx/sympytools.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 12:29:42.528748 gotranx-0.3.3/src/gotranx/templates/
--rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-03-13 12:29:39.000000 gotranx-0.3.3/src/gotranx/templates/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2343 2024-03-13 12:29:39.000000 gotranx-0.3.3/src/gotranx/templates/c.py
--rw-r--r--   0 runner    (1001) docker     (127)     3932 2024-03-13 12:29:39.000000 gotranx-0.3.3/src/gotranx/templates/python.py
--rw-r--r--   0 runner    (1001) docker     (127)     7125 2024-03-13 12:29:39.000000 gotranx-0.3.3/src/gotranx/transformer.py
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-03-13 12:29:39.000000 gotranx-0.3.3/src/gotranx/units.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 12:29:42.532748 gotranx-0.3.3/src/gotranx.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     7946 2024-03-13 12:29:42.000000 gotranx-0.3.3/src/gotranx.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1418 2024-03-13 12:29:42.000000 gotranx-0.3.3/src/gotranx.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-13 12:29:42.000000 gotranx-0.3.3/src/gotranx.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-03-13 12:29:42.000000 gotranx-0.3.3/src/gotranx.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-13 12:29:42.000000 gotranx-0.3.3/src/gotranx.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      402 2024-03-13 12:29:42.000000 gotranx-0.3.3/src/gotranx.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-03-13 12:29:42.000000 gotranx-0.3.3/src/gotranx.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 12:29:42.532748 gotranx-0.3.3/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     4798 2024-03-13 12:29:39.000000 gotranx-0.3.3/tests/test_atoms.py
--rw-r--r--   0 runner    (1001) docker     (127)    21223 2024-03-13 12:29:39.000000 gotranx-0.3.3/tests/test_c_codegen.py
--rw-r--r--   0 runner    (1001) docker     (127)     2241 2024-03-13 12:29:39.000000 gotranx-0.3.3/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     2757 2024-03-13 12:29:39.000000 gotranx-0.3.3/tests/test_conditionals.py
--rw-r--r--   0 runner    (1001) docker     (127)     3172 2024-03-13 12:29:39.000000 gotranx-0.3.3/tests/test_expressions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1208 2024-03-13 12:29:39.000000 gotranx-0.3.3/tests/test_load.py
--rw-r--r--   0 runner    (1001) docker     (127)      949 2024-03-13 12:29:39.000000 gotranx-0.3.3/tests/test_myokit.py
--rw-r--r--   0 runner    (1001) docker     (127)     4867 2024-03-13 12:29:39.000000 gotranx-0.3.3/tests/test_ode.py
--rw-r--r--   0 runner    (1001) docker     (127)     5922 2024-03-13 12:29:39.000000 gotranx-0.3.3/tests/test_ode_component.py
--rw-r--r--   0 runner    (1001) docker     (127)    20546 2024-03-13 12:29:39.000000 gotranx-0.3.3/tests/test_python_codegen.py
--rw-r--r--   0 runner    (1001) docker     (127)     1761 2024-03-13 12:29:39.000000 gotranx-0.3.3/tests/test_save.py
--rw-r--r--   0 runner    (1001) docker     (127)     2023 2024-03-13 12:29:39.000000 gotranx-0.3.3/tests/test_schemes.py
--rw-r--r--   0 runner    (1001) docker     (127)     7465 2024-03-13 12:29:39.000000 gotranx-0.3.3/tests/test_subodes.py
--rw-r--r--   0 runner    (1001) docker     (127)     1894 2024-03-13 12:29:39.000000 gotranx-0.3.3/tests/test_sympytools.py
--rw-r--r--   0 runner    (1001) docker     (127)    19349 2024-03-13 12:29:39.000000 gotranx-0.3.3/tests/test_transformer_assignments.py
--rw-r--r--   0 runner    (1001) docker     (127)     3983 2024-03-13 12:29:39.000000 gotranx-0.3.3/tests/test_transformer_parameters.py
--rw-r--r--   0 runner    (1001) docker     (127)     4775 2024-03-13 12:29:39.000000 gotranx-0.3.3/tests/test_transformer_states.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 19:37:17.374737 gotranx-0.3.4/
+-rw-r--r--   0 runner    (1001) docker     (127)     4612 2024-04-03 19:37:17.374737 gotranx-0.3.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2812 2024-04-03 19:37:13.000000 gotranx-0.3.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3487 2024-04-03 19:37:13.000000 gotranx-0.3.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-03 19:37:17.374737 gotranx-0.3.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 19:37:17.362737 gotranx-0.3.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 19:37:17.366737 gotranx-0.3.4/src/gotranx/
+-rw-r--r--   0 runner    (1001) docker     (127)      947 2024-04-03 19:37:13.000000 gotranx-0.3.4/src/gotranx/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-04-03 19:37:13.000000 gotranx-0.3.4/src/gotranx/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6522 2024-04-03 19:37:13.000000 gotranx-0.3.4/src/gotranx/atoms.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 19:37:17.370737 gotranx-0.3.4/src/gotranx/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)     3351 2024-04-03 19:37:13.000000 gotranx-0.3.4/src/gotranx/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      773 2024-04-03 19:37:13.000000 gotranx-0.3.4/src/gotranx/cli/cellml2ode.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2322 2024-04-03 19:37:13.000000 gotranx-0.3.4/src/gotranx/cli/gotran2c.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2357 2024-04-03 19:37:13.000000 gotranx-0.3.4/src/gotranx/cli/gotran2py.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 19:37:17.370737 gotranx-0.3.4/src/gotranx/codegen/
+-rw-r--r--   0 runner    (1001) docker     (127)      622 2024-04-03 19:37:13.000000 gotranx-0.3.4/src/gotranx/codegen/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15171 2024-04-03 19:37:13.000000 gotranx-0.3.4/src/gotranx/codegen/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4273 2024-04-03 19:37:13.000000 gotranx-0.3.4/src/gotranx/codegen/c.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5607 2024-04-03 19:37:13.000000 gotranx-0.3.4/src/gotranx/codegen/ode.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6008 2024-04-03 19:37:13.000000 gotranx-0.3.4/src/gotranx/codegen/python.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2531 2024-04-03 19:37:13.000000 gotranx-0.3.4/src/gotranx/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4894 2024-04-03 19:37:13.000000 gotranx-0.3.4/src/gotranx/expressions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      879 2024-04-03 19:37:13.000000 gotranx-0.3.4/src/gotranx/load.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7523 2024-04-03 19:37:13.000000 gotranx-0.3.4/src/gotranx/myokit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2335 2024-04-03 19:37:13.000000 gotranx-0.3.4/src/gotranx/ode.lark
+-rw-r--r--   0 runner    (1001) docker     (127)    11529 2024-04-03 19:37:13.000000 gotranx-0.3.4/src/gotranx/ode.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7095 2024-04-03 19:37:13.000000 gotranx-0.3.4/src/gotranx/ode_component.py
+-rw-r--r--   0 runner    (1001) docker     (127)      334 2024-04-03 19:37:13.000000 gotranx-0.3.4/src/gotranx/parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)      601 2024-04-03 19:37:13.000000 gotranx-0.3.4/src/gotranx/save.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5073 2024-04-03 19:37:13.000000 gotranx-0.3.4/src/gotranx/schemes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3237 2024-04-03 19:37:13.000000 gotranx-0.3.4/src/gotranx/sympytools.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 19:37:17.370737 gotranx-0.3.4/src/gotranx/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-04-03 19:37:13.000000 gotranx-0.3.4/src/gotranx/templates/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2343 2024-04-03 19:37:13.000000 gotranx-0.3.4/src/gotranx/templates/c.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3934 2024-04-03 19:37:13.000000 gotranx-0.3.4/src/gotranx/templates/python.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7125 2024-04-03 19:37:13.000000 gotranx-0.3.4/src/gotranx/transformer.py
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-04-03 19:37:13.000000 gotranx-0.3.4/src/gotranx/units.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 19:37:17.374737 gotranx-0.3.4/src/gotranx.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4612 2024-04-03 19:37:17.000000 gotranx-0.3.4/src/gotranx.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1418 2024-04-03 19:37:17.000000 gotranx-0.3.4/src/gotranx.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 19:37:17.000000 gotranx-0.3.4/src/gotranx.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-03 19:37:17.000000 gotranx-0.3.4/src/gotranx.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 19:37:17.000000 gotranx-0.3.4/src/gotranx.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      402 2024-04-03 19:37:17.000000 gotranx-0.3.4/src/gotranx.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-03 19:37:17.000000 gotranx-0.3.4/src/gotranx.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 19:37:17.374737 gotranx-0.3.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     4798 2024-04-03 19:37:13.000000 gotranx-0.3.4/tests/test_atoms.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21223 2024-04-03 19:37:13.000000 gotranx-0.3.4/tests/test_c_codegen.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2241 2024-04-03 19:37:13.000000 gotranx-0.3.4/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2757 2024-04-03 19:37:13.000000 gotranx-0.3.4/tests/test_conditionals.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3172 2024-04-03 19:37:13.000000 gotranx-0.3.4/tests/test_expressions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1208 2024-04-03 19:37:13.000000 gotranx-0.3.4/tests/test_load.py
+-rw-r--r--   0 runner    (1001) docker     (127)      949 2024-04-03 19:37:13.000000 gotranx-0.3.4/tests/test_myokit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4867 2024-04-03 19:37:13.000000 gotranx-0.3.4/tests/test_ode.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5922 2024-04-03 19:37:13.000000 gotranx-0.3.4/tests/test_ode_component.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20662 2024-04-03 19:37:13.000000 gotranx-0.3.4/tests/test_python_codegen.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1761 2024-04-03 19:37:13.000000 gotranx-0.3.4/tests/test_save.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2023 2024-04-03 19:37:13.000000 gotranx-0.3.4/tests/test_schemes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7521 2024-04-03 19:37:13.000000 gotranx-0.3.4/tests/test_subodes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1894 2024-04-03 19:37:13.000000 gotranx-0.3.4/tests/test_sympytools.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19349 2024-04-03 19:37:13.000000 gotranx-0.3.4/tests/test_transformer_assignments.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3983 2024-04-03 19:37:13.000000 gotranx-0.3.4/tests/test_transformer_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4775 2024-04-03 19:37:13.000000 gotranx-0.3.4/tests/test_transformer_states.py
```

### Comparing `gotranx-0.3.3/pyproject.toml` & `gotranx-0.3.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.2"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "gotranx"
-version = "0.3.3"
+version = "0.3.4"
 description = "A declarative language describing ordinary differential equations"
 authors = [{name = "Henrik Finsberg", email = "henriknf@simula.no"}]
 license = {text = "MIT"}
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3 :: Only",
@@ -153,14 +153,14 @@
 allow_dirty = false
 commit = true
 message = "Bump version: {current_version} → {new_version}"
 tag = true
 sign_tags = false
 tag_name = "v{new_version}"
 tag_message = "Bump version: {current_version} → {new_version}"
-current_version = "0.3.3"
+current_version = "0.3.4"
 
 
 [[tool.bumpversion.files]]
 filename = "pyproject.toml"
 search = 'version = "{current_version}"'
 replace = 'version = "{new_version}"'
```

### Comparing `gotranx-0.3.3/src/gotranx/__init__.py` & `gotranx-0.3.4/src/gotranx/__init__.py`

 * *Files identical despite different names*

### Comparing `gotranx-0.3.3/src/gotranx/atoms.py` & `gotranx-0.3.4/src/gotranx/atoms.py`

 * *Files identical despite different names*

### Comparing `gotranx-0.3.3/src/gotranx/cli/__init__.py` & `gotranx-0.3.4/src/gotranx/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `gotranx-0.3.3/src/gotranx/cli/cellml2ode.py` & `gotranx-0.3.4/src/gotranx/cli/cellml2ode.py`

 * *Files identical despite different names*

### Comparing `gotranx-0.3.3/src/gotranx/cli/gotran2c.py` & `gotranx-0.3.4/src/gotranx/cli/gotran2c.py`

 * *Files identical despite different names*

### Comparing `gotranx-0.3.3/src/gotranx/cli/gotran2py.py` & `gotranx-0.3.4/src/gotranx/cli/gotran2py.py`

 * *Files identical despite different names*

### Comparing `gotranx-0.3.3/src/gotranx/codegen/__init__.py` & `gotranx-0.3.4/src/gotranx/codegen/__init__.py`

 * *Files identical despite different names*

### Comparing `gotranx-0.3.3/src/gotranx/codegen/base.py` & `gotranx-0.3.4/src/gotranx/codegen/base.py`

 * *Files identical despite different names*

### Comparing `gotranx-0.3.3/src/gotranx/codegen/c.py` & `gotranx-0.3.4/src/gotranx/codegen/c.py`

 * *Files identical despite different names*

### Comparing `gotranx-0.3.3/src/gotranx/codegen/ode.py` & `gotranx-0.3.4/src/gotranx/codegen/ode.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,15 +35,14 @@
             "<=": "Le",
             ">": "Gt",
             ">=": "Ge",
             "==": "Eq",
             "!=": "Ne",
         }
         relop = relop2str[expr.rel_op]
-        print(expr, f"{relop}({lhs}, {rhs})")
         return f"{relop}({lhs}, {rhs})"
 
     def _print_Or(self, expr):
         return f"Or({', '.join(self._print(a) for a in expr.args)})"
 
     def _print_And(self, expr):
         return f"And({', '.join(self._print(a) for a in expr.args)})"
@@ -99,15 +98,15 @@
         d: dict[tuple[str, ...], list[atoms.State]] = defaultdict(list)
         for state in self.ode.states:
             d[state.components].append(state)
 
         text = ""
         for components, states in d.items():
             text += start_odeblock("states", names=components) + "\n"
-            text += ", ".join([print_ScalarParam(s, doprint=self.doprint) for s in states])
+            text += ",\n".join([print_ScalarParam(s, doprint=self.doprint) for s in states])
             text += "\n)\n\n"
         return text
 
     def print_parameters(self) -> str:
         d: dict[tuple[str, ...], list[atoms.Parameter]] = defaultdict(list)
         for parameter in self.ode.parameters:
             d[parameter.components].append(parameter)
```

### Comparing `gotranx-0.3.3/src/gotranx/codegen/python.py` & `gotranx-0.3.4/src/gotranx/codegen/python.py`

 * *Files identical despite different names*

### Comparing `gotranx-0.3.3/src/gotranx/exceptions.py` & `gotranx-0.3.4/src/gotranx/exceptions.py`

 * *Files identical despite different names*

### Comparing `gotranx-0.3.3/src/gotranx/expressions.py` & `gotranx-0.3.4/src/gotranx/expressions.py`

 * *Files identical despite different names*

### Comparing `gotranx-0.3.3/src/gotranx/load.py` & `gotranx-0.3.4/src/gotranx/load.py`

 * *Files identical despite different names*

### Comparing `gotranx-0.3.3/src/gotranx/myokit.py` & `gotranx-0.3.4/src/gotranx/myokit.py`

 * *Files identical despite different names*

### Comparing `gotranx-0.3.3/src/gotranx/ode.lark` & `gotranx-0.3.4/src/gotranx/ode.lark`

 * *Files identical despite different names*

### Comparing `gotranx-0.3.3/src/gotranx/ode.py` & `gotranx-0.3.4/src/gotranx/ode.py`

 * *Files identical despite different names*

### Comparing `gotranx-0.3.3/src/gotranx/ode_component.py` & `gotranx-0.3.4/src/gotranx/ode_component.py`

 * *Files identical despite different names*

### Comparing `gotranx-0.3.3/src/gotranx/save.py` & `gotranx-0.3.4/src/gotranx/save.py`

 * *Files identical despite different names*

### Comparing `gotranx-0.3.3/src/gotranx/schemes.py` & `gotranx-0.3.4/src/gotranx/schemes.py`

 * *Files identical despite different names*

### Comparing `gotranx-0.3.3/src/gotranx/sympytools.py` & `gotranx-0.3.4/src/gotranx/sympytools.py`

 * *Files identical despite different names*

### Comparing `gotranx-0.3.3/src/gotranx/templates/__init__.py` & `gotranx-0.3.4/src/gotranx/templates/__init__.py`

 * *Files identical despite different names*

### Comparing `gotranx-0.3.3/src/gotranx/templates/c.py` & `gotranx-0.3.4/src/gotranx/templates/c.py`

 * *Files identical despite different names*

### Comparing `gotranx-0.3.3/src/gotranx/templates/python.py` & `gotranx-0.3.4/src/gotranx/templates/python.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,14 +12,17 @@
     else:
         return all_values + ", " + next_value
 
 
 def _index(data: dict[str, int], name: str) -> str:
     return dedent(
         f'''
+{name} = {repr(data)}
+
+
 def {name}_index(name: str) -> int:
     """Return the index of the {name} with the given name
 
     Arguments
     ---------
     name : str
         The name of the {name}
@@ -31,16 +34,15 @@
 
     Raises
     ------
     KeyError
         If the name is not a valid {name}
     """
 
-    data = {repr(data)}
-    return data[name]
+    return {name}[name]
 ''',
     )
 
 
 def state_index(data: dict[str, int]) -> str:
     logger.debug(f"Generating state_index with {len(data)} values")
     return _index(data, "state")
```

### Comparing `gotranx-0.3.3/src/gotranx/transformer.py` & `gotranx-0.3.4/src/gotranx/transformer.py`

 * *Files identical despite different names*

### Comparing `gotranx-0.3.3/src/gotranx.egg-info/SOURCES.txt` & `gotranx-0.3.4/src/gotranx.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gotranx-0.3.3/tests/test_atoms.py` & `gotranx-0.3.4/tests/test_atoms.py`

 * *Files identical despite different names*

### Comparing `gotranx-0.3.3/tests/test_c_codegen.py` & `gotranx-0.3.4/tests/test_c_codegen.py`

 * *Files identical despite different names*

### Comparing `gotranx-0.3.3/tests/test_cli.py` & `gotranx-0.3.4/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `gotranx-0.3.3/tests/test_conditionals.py` & `gotranx-0.3.4/tests/test_conditionals.py`

 * *Files identical despite different names*

### Comparing `gotranx-0.3.3/tests/test_expressions.py` & `gotranx-0.3.4/tests/test_expressions.py`

 * *Files identical despite different names*

### Comparing `gotranx-0.3.3/tests/test_load.py` & `gotranx-0.3.4/tests/test_load.py`

 * *Files identical despite different names*

### Comparing `gotranx-0.3.3/tests/test_myokit.py` & `gotranx-0.3.4/tests/test_myokit.py`

 * *Files identical despite different names*

### Comparing `gotranx-0.3.3/tests/test_ode.py` & `gotranx-0.3.4/tests/test_ode.py`

 * *Files identical despite different names*

### Comparing `gotranx-0.3.3/tests/test_ode_component.py` & `gotranx-0.3.4/tests/test_ode_component.py`

 * *Files identical despite different names*

### Comparing `gotranx-0.3.3/tests/test_python_codegen.py` & `gotranx-0.3.4/tests/test_python_codegen.py`

 * *Files 4% similar despite different names*

```diff
@@ -38,15 +38,18 @@
 def codegen_no_black(ode) -> PythonCodeGenerator:
     with mock.patch.dict(sys.modules, {"black": None}):
         return PythonCodeGenerator(ode)
 
 
 def test_python_codegen_state_index_no_black(codegen: PythonCodeGenerator):
     assert codegen.state_index() == (
-        "def state_index(name: str) -> int:"
+        'state = {"x": 0, "z": 1, "y": 2}'
+        "\n"
+        "\n"
+        "\ndef state_index(name: str) -> int:"
         '\n    """Return the index of the state with the given name'
         "\n"
         "\n    Arguments"
         "\n    ---------"
         "\n    name : str"
         "\n        The name of the state"
         "\n"
@@ -57,16 +60,15 @@
         "\n"
         "\n    Raises"
         "\n    ------"
         "\n    KeyError"
         "\n        If the name is not a valid state"
         '\n    """'
         "\n"
-        '\n    data = {"x": 0, "z": 1, "y": 2}'
-        "\n    return data[name]"
+        "\n    return state[name]"
         "\n"
     )
 
 
 def test_python_codegen_initial_state_values(codegen: PythonCodeGenerator):
     assert codegen.initial_state_values() == (
         "def init_state_values(**values):"
@@ -81,14 +83,17 @@
         "\n    return states"
         "\n"
     )
 
 
 def test_python_codegen_parameter_index_no_black(codegen_no_black: PythonCodeGenerator):
     assert codegen_no_black.parameter_index() == (
+        "\nparameter = {'a': 0, 'beta': 1, 'rho': 2, 'sigma': 3}"
+        "\n"
+        "\n"
         "\ndef parameter_index(name: str) -> int:"
         '\n    """Return the index of the parameter with the given name'
         "\n"
         "\n    Arguments"
         "\n    ---------"
         "\n    name : str"
         "\n        The name of the parameter"
@@ -100,23 +105,25 @@
         "\n"
         "\n    Raises"
         "\n    ------"
         "\n    KeyError"
         "\n        If the name is not a valid parameter"
         '\n    """'
         "\n"
-        "\n    data = {'a': 0, 'beta': 1, 'rho': 2, 'sigma': 3}"
-        "\n    return data[name]"
+        "\n    return parameter[name]"
         "\n"
     )
 
 
 def test_python_codegen_parameter_index(codegen: PythonCodeGenerator):
     assert codegen.parameter_index() == (
-        "def parameter_index(name: str) -> int:"
+        'parameter = {"a": 0, "beta": 1, "rho": 2, "sigma": 3}'
+        "\n"
+        "\n"
+        "\ndef parameter_index(name: str) -> int:"
         '\n    """Return the index of the parameter with the given name'
         "\n"
         "\n    Arguments"
         "\n    ---------"
         "\n    name : str"
         "\n        The name of the parameter"
         "\n"
@@ -127,16 +134,15 @@
         "\n"
         "\n    Raises"
         "\n    ------"
         "\n    KeyError"
         "\n        If the name is not a valid parameter"
         '\n    """'
         "\n"
-        '\n    data = {"a": 0, "beta": 1, "rho": 2, "sigma": 3}'
-        "\n    return data[name]"
+        "\n    return parameter[name]"
         "\n"
     )
 
 
 def test_python_codegen_initial_parameter_values(codegen: PythonCodeGenerator):
     assert codegen.initial_parameter_values() == (
         "def init_parameter_values(**values):"
@@ -600,15 +606,18 @@
         "\n    return values"
         "\n"
     )
 
 
 def test_python_monitored_index(codegen: PythonCodeGenerator):
     assert codegen.monitor_index() == (
-        "def monitor_index(name: str) -> int:"
+        'monitor = {"betaz": 0, "rhoz": 1, "dx_dt": 2, "dz_dt": 3, "dy_dt": 4}'
+        "\n"
+        "\n"
+        "\ndef monitor_index(name: str) -> int:"
         '\n    """Return the index of the monitor with the given name'
         "\n"
         "\n    Arguments"
         "\n    ---------"
         "\n    name : str"
         "\n        The name of the monitor"
         "\n"
@@ -619,11 +628,10 @@
         "\n"
         "\n    Raises"
         "\n    ------"
         "\n    KeyError"
         "\n        If the name is not a valid monitor"
         '\n    """'
         "\n"
-        '\n    data = {"betaz": 0, "rhoz": 1, "dx_dt": 2, "dz_dt": 3, "dy_dt": 4}'
-        "\n    return data[name]"
+        "\n    return monitor[name]"
         "\n"
     )
```

### Comparing `gotranx-0.3.3/tests/test_save.py` & `gotranx-0.3.4/tests/test_save.py`

 * *Files identical despite different names*

### Comparing `gotranx-0.3.3/tests/test_schemes.py` & `gotranx-0.3.4/tests/test_schemes.py`

 * *Files identical despite different names*

### Comparing `gotranx-0.3.3/tests/test_subodes.py` & `gotranx-0.3.4/tests/test_subodes.py`

 * *Files 1% similar despite different names*

```diff
@@ -58,15 +58,18 @@
     z_comp = main_ode.get_component("Z component")
     z_ode = z_comp.to_ode()
     return gotranx.codegen.PythonCodeGenerator(z_ode)
 
 
 def test_codegen_component_ode_missing_index(z_ode_codegen):
     assert z_ode_codegen.missing_index() == (
-        "def missing_index(name: str) -> int:"
+        'missing = {"x": 0, "y": 1}'
+        "\n"
+        "\n"
+        "\ndef missing_index(name: str) -> int:"
         '\n    """Return the index of the missing with the given name'
         "\n"
         "\n    Arguments"
         "\n    ---------"
         "\n    name : str"
         "\n        The name of the missing"
         "\n"
@@ -77,16 +80,15 @@
         "\n"
         "\n    Raises"
         "\n    ------"
         "\n    KeyError"
         "\n        If the name is not a valid missing"
         '\n    """'
         "\n"
-        '\n    data = {"x": 0, "y": 1}'
-        "\n    return data[name]"
+        "\n    return missing[name]"
         "\n"
     )
 
 
 def test_codegen_component_ode_rhs(z_ode_codegen):
     assert z_ode_codegen.rhs() == (
         "def rhs(t, states, parameters, missing_variables):"
@@ -171,15 +173,18 @@
     z_comp = main_ode.get_component("Z component")
     remaining_ode = main_ode - z_comp
     return gotranx.codegen.PythonCodeGenerator(remaining_ode)
 
 
 def test_codegen_remaining_ode_missing_index(remaining_ode_codegen):
     assert remaining_ode_codegen.missing_index() == (
-        "def missing_index(name: str) -> int:"
+        'missing = {"z": 0}'
+        "\n"
+        "\n"
+        "\ndef missing_index(name: str) -> int:"
         '\n    """Return the index of the missing with the given name'
         "\n"
         "\n    Arguments"
         "\n    ---------"
         "\n    name : str"
         "\n        The name of the missing"
         "\n"
@@ -190,16 +195,15 @@
         "\n"
         "\n    Raises"
         "\n    ------"
         "\n    KeyError"
         "\n        If the name is not a valid missing"
         '\n    """'
         "\n"
-        '\n    data = {"z": 0}'
-        "\n    return data[name]"
+        "\n    return missing[name]"
         "\n"
     )
 
 
 def test_codegen_remaining_ode_rhs(remaining_ode_codegen):
     assert remaining_ode_codegen.rhs() == (
         "def rhs(t, states, parameters, missing_variables):"
```

### Comparing `gotranx-0.3.3/tests/test_sympytools.py` & `gotranx-0.3.4/tests/test_sympytools.py`

 * *Files identical despite different names*

### Comparing `gotranx-0.3.3/tests/test_transformer_assignments.py` & `gotranx-0.3.4/tests/test_transformer_assignments.py`

 * *Files identical despite different names*

### Comparing `gotranx-0.3.3/tests/test_transformer_parameters.py` & `gotranx-0.3.4/tests/test_transformer_parameters.py`

 * *Files identical despite different names*

### Comparing `gotranx-0.3.3/tests/test_transformer_states.py` & `gotranx-0.3.4/tests/test_transformer_states.py`

 * *Files identical despite different names*

