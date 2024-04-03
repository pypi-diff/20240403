# Comparing `tmp/biogeme-optimization-0.0.6.tar.gz` & `tmp/biogeme-optimization-0.0.6a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "biogeme-optimization-0.0.6.tar", last modified: Wed Apr  3 13:30:16 2024, max compression
+gzip compressed data, was "biogeme-optimization-0.0.6a0.tar", last modified: Wed Mar 27 13:04:33 2024, max compression
```

## Comparing `biogeme-optimization-0.0.6.tar` & `biogeme-optimization-0.0.6a0.tar`

### file list

```diff
@@ -1,72 +1,61 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 13:30:16.424909 biogeme-optimization-0.0.6/
--rw-r--r--   0 runner    (1001) docker     (127)     3607 2024-04-03 13:30:16.424909 biogeme-optimization-0.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2533 2024-04-03 13:30:12.000000 biogeme-optimization-0.0.6/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1105 2024-04-03 13:30:16.424909 biogeme-optimization-0.0.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-03 13:30:12.000000 biogeme-optimization-0.0.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 13:30:16.408909 biogeme-optimization-0.0.6/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 13:30:16.412909 biogeme-optimization-0.0.6/src/biogeme_optimization/
--rw-r--r--   0 runner    (1001) docker     (127)      105 2024-04-03 13:30:12.000000 biogeme-optimization-0.0.6/src/biogeme_optimization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7910 2024-04-03 13:30:12.000000 biogeme-optimization-0.0.6/src/biogeme_optimization/algebra.py
--rw-r--r--   0 runner    (1001) docker     (127)     2923 2024-04-03 13:30:12.000000 biogeme-optimization-0.0.6/src/biogeme_optimization/bfgs.py
--rw-r--r--   0 runner    (1001) docker     (127)     1963 2024-04-03 13:30:12.000000 biogeme-optimization-0.0.6/src/biogeme_optimization/biogeme_logging.py
--rw-r--r--   0 runner    (1001) docker     (127)    33178 2024-04-03 13:30:12.000000 biogeme-optimization-0.0.6/src/biogeme_optimization/bounds.py
--rw-r--r--   0 runner    (1001) docker     (127)      819 2024-04-03 13:30:12.000000 biogeme-optimization-0.0.6/src/biogeme_optimization/diagnostics.py
--rw-r--r--   0 runner    (1001) docker     (127)      203 2024-04-03 13:30:12.000000 biogeme-optimization-0.0.6/src/biogeme_optimization/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2848 2024-04-03 13:30:12.000000 biogeme-optimization-0.0.6/src/biogeme_optimization/format.py
--rw-r--r--   0 runner    (1001) docker     (127)    14015 2024-04-03 13:30:12.000000 biogeme-optimization-0.0.6/src/biogeme_optimization/function.py
--rw-r--r--   0 runner    (1001) docker     (127)     6865 2024-04-03 13:30:12.000000 biogeme-optimization-0.0.6/src/biogeme_optimization/hybrid_function.py
--rw-r--r--   0 runner    (1001) docker     (127)    12183 2024-04-03 13:30:12.000000 biogeme-optimization-0.0.6/src/biogeme_optimization/linesearch.py
--rw-r--r--   0 runner    (1001) docker     (127)     8623 2024-04-03 13:30:12.000000 biogeme-optimization-0.0.6/src/biogeme_optimization/neighborhood.py
--rw-r--r--   0 runner    (1001) docker     (127)    14417 2024-04-03 13:30:12.000000 biogeme-optimization-0.0.6/src/biogeme_optimization/pareto.py
--rw-r--r--   0 runner    (1001) docker     (127)    12142 2024-04-03 13:30:12.000000 biogeme-optimization-0.0.6/src/biogeme_optimization/simple_bounds.py
--rw-r--r--   0 runner    (1001) docker     (127)    13907 2024-04-03 13:30:12.000000 biogeme-optimization-0.0.6/src/biogeme_optimization/stochastic_function.py
--rw-r--r--   0 runner    (1001) docker     (127)    10063 2024-04-03 13:30:12.000000 biogeme-optimization-0.0.6/src/biogeme_optimization/stochastic_simple_bounds.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 13:30:16.416909 biogeme-optimization-0.0.6/src/biogeme_optimization/teaching/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 13:30:12.000000 biogeme-optimization-0.0.6/src/biogeme_optimization/teaching/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 13:30:16.416909 biogeme-optimization-0.0.6/src/biogeme_optimization/teaching/linear_constraints/
--rw-r--r--   0 runner    (1001) docker     (127)      606 2024-04-03 13:30:12.000000 biogeme-optimization-0.0.6/src/biogeme_optimization/teaching/linear_constraints/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    17171 2024-04-03 13:30:12.000000 biogeme-optimization-0.0.6/src/biogeme_optimization/teaching/linear_constraints/constraint.py
--rw-r--r--   0 runner    (1001) docker     (127)     6689 2024-04-03 13:30:12.000000 biogeme-optimization-0.0.6/src/biogeme_optimization/teaching/linear_constraints/draw_polyhedron.py
--rw-r--r--   0 runner    (1001) docker     (127)    17310 2024-04-03 13:30:12.000000 biogeme-optimization-0.0.6/src/biogeme_optimization/teaching/linear_constraints/linear_constraints.py
--rw-r--r--   0 runner    (1001) docker     (127)     9518 2024-04-03 13:30:12.000000 biogeme-optimization-0.0.6/src/biogeme_optimization/teaching/linear_constraints/polyhedron_2d.py
--rw-r--r--   0 runner    (1001) docker     (127)    10102 2024-04-03 13:30:12.000000 biogeme-optimization-0.0.6/src/biogeme_optimization/teaching/linear_constraints/standard_canonical.py
--rw-r--r--   0 runner    (1001) docker     (127)     5499 2024-04-03 13:30:12.000000 biogeme-optimization-0.0.6/src/biogeme_optimization/teaching/linear_constraints/standard_form.py
--rw-r--r--   0 runner    (1001) docker     (127)     2050 2024-04-03 13:30:12.000000 biogeme-optimization-0.0.6/src/biogeme_optimization/teaching/linear_constraints/variable.py
--rw-r--r--   0 runner    (1001) docker     (127)     5156 2024-04-03 13:30:12.000000 biogeme-optimization-0.0.6/src/biogeme_optimization/teaching/linear_optimization.py
--rw-r--r--   0 runner    (1001) docker     (127)     3392 2024-04-03 13:30:12.000000 biogeme-optimization-0.0.6/src/biogeme_optimization/teaching/matrices.py
--rw-r--r--   0 runner    (1001) docker     (127)     1907 2024-04-03 13:30:12.000000 biogeme-optimization-0.0.6/src/biogeme_optimization/teaching/plot_function.py
--rw-r--r--   0 runner    (1001) docker     (127)     6468 2024-04-03 13:30:12.000000 biogeme-optimization-0.0.6/src/biogeme_optimization/teaching/simplex.py
--rw-r--r--   0 runner    (1001) docker     (127)     8397 2024-04-03 13:30:12.000000 biogeme-optimization-0.0.6/src/biogeme_optimization/teaching/tableau.py
--rw-r--r--   0 runner    (1001) docker     (127)    10119 2024-04-03 13:30:12.000000 biogeme-optimization-0.0.6/src/biogeme_optimization/teaching/to_jupyter.py
--rw-r--r--   0 runner    (1001) docker     (127)     3518 2024-04-03 13:30:12.000000 biogeme-optimization-0.0.6/src/biogeme_optimization/teaching/variables.py
--rw-r--r--   0 runner    (1001) docker     (127)    22515 2024-04-03 13:30:12.000000 biogeme-optimization-0.0.6/src/biogeme_optimization/trust_region.py
--rw-r--r--   0 runner    (1001) docker     (127)     8279 2024-04-03 13:30:12.000000 biogeme-optimization-0.0.6/src/biogeme_optimization/vns.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 13:30:16.420909 biogeme-optimization-0.0.6/src/biogeme_optimization.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3607 2024-04-03 13:30:16.000000 biogeme-optimization-0.0.6/src/biogeme_optimization.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2484 2024-04-03 13:30:16.000000 biogeme-optimization-0.0.6/src/biogeme_optimization.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 13:30:16.000000 biogeme-optimization-0.0.6/src/biogeme_optimization.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      101 2024-04-03 13:30:16.000000 biogeme-optimization-0.0.6/src/biogeme_optimization.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-03 13:30:16.000000 biogeme-optimization-0.0.6/src/biogeme_optimization.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 13:30:16.420909 biogeme-optimization-0.0.6/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     6377 2024-04-03 13:30:12.000000 biogeme-optimization-0.0.6/tests/test_algebra.py
--rw-r--r--   0 runner    (1001) docker     (127)     3644 2024-04-03 13:30:12.000000 biogeme-optimization-0.0.6/tests/test_bfgs.py
--rw-r--r--   0 runner    (1001) docker     (127)    53852 2024-04-03 13:30:12.000000 biogeme-optimization-0.0.6/tests/test_bounds.py
--rw-r--r--   0 runner    (1001) docker     (127)     4117 2024-04-03 13:30:12.000000 biogeme-optimization-0.0.6/tests/test_constraints.py
--rw-r--r--   0 runner    (1001) docker     (127)     2923 2024-04-03 13:30:12.000000 biogeme-optimization-0.0.6/tests/test_function.py
--rw-r--r--   0 runner    (1001) docker     (127)     4552 2024-04-03 13:30:12.000000 biogeme-optimization-0.0.6/tests/test_hybrid_function.py
--rw-r--r--   0 runner    (1001) docker     (127)     5263 2024-04-03 13:30:12.000000 biogeme-optimization-0.0.6/tests/test_linear_constraints.py
--rw-r--r--   0 runner    (1001) docker     (127)     3146 2024-04-03 13:30:12.000000 biogeme-optimization-0.0.6/tests/test_linear_optimization.py
--rw-r--r--   0 runner    (1001) docker     (127)    10168 2024-04-03 13:30:12.000000 biogeme-optimization-0.0.6/tests/test_linesearch.py
--rw-r--r--   0 runner    (1001) docker     (127)     5179 2024-04-03 13:30:12.000000 biogeme-optimization-0.0.6/tests/test_matrices.py
--rw-r--r--   0 runner    (1001) docker     (127)     4799 2024-04-03 13:30:12.000000 biogeme-optimization-0.0.6/tests/test_neighborhood.py
--rw-r--r--   0 runner    (1001) docker     (127)     6402 2024-04-03 13:30:12.000000 biogeme-optimization-0.0.6/tests/test_pareto.py
--rw-r--r--   0 runner    (1001) docker     (127)     1465 2024-04-03 13:30:12.000000 biogeme-optimization-0.0.6/tests/test_plot_function.py
--rw-r--r--   0 runner    (1001) docker     (127)     2454 2024-04-03 13:30:12.000000 biogeme-optimization-0.0.6/tests/test_polyhedron_2d.py
--rw-r--r--   0 runner    (1001) docker     (127)    10094 2024-04-03 13:30:12.000000 biogeme-optimization-0.0.6/tests/test_simple_bounds.py
--rw-r--r--   0 runner    (1001) docker     (127)     3627 2024-04-03 13:30:12.000000 biogeme-optimization-0.0.6/tests/test_simplex.py
--rw-r--r--   0 runner    (1001) docker     (127)     3271 2024-04-03 13:30:12.000000 biogeme-optimization-0.0.6/tests/test_standard_canonical.py
--rw-r--r--   0 runner    (1001) docker     (127)     5624 2024-04-03 13:30:12.000000 biogeme-optimization-0.0.6/tests/test_standard_form.py
--rw-r--r--   0 runner    (1001) docker     (127)     3109 2024-04-03 13:30:12.000000 biogeme-optimization-0.0.6/tests/test_tableau.py
--rw-r--r--   0 runner    (1001) docker     (127)    23343 2024-04-03 13:30:12.000000 biogeme-optimization-0.0.6/tests/test_trust_region.py
--rw-r--r--   0 runner    (1001) docker     (127)     3389 2024-04-03 13:30:12.000000 biogeme-optimization-0.0.6/tests/test_variables.py
--rw-r--r--   0 runner    (1001) docker     (127)     3674 2024-04-03 13:30:12.000000 biogeme-optimization-0.0.6/tests/test_vns.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 13:04:33.974361 biogeme-optimization-0.0.6a0/
+-rw-r--r--   0 runner    (1001) docker     (127)     3609 2024-03-27 13:04:33.974361 biogeme-optimization-0.0.6a0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2533 2024-03-27 13:04:11.000000 biogeme-optimization-0.0.6a0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1107 2024-03-27 13:04:33.974361 biogeme-optimization-0.0.6a0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-03-27 13:04:11.000000 biogeme-optimization-0.0.6a0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 13:04:33.962361 biogeme-optimization-0.0.6a0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 13:04:33.966361 biogeme-optimization-0.0.6a0/src/biogeme_optimization/
+-rw-r--r--   0 runner    (1001) docker     (127)      105 2024-03-27 13:04:11.000000 biogeme-optimization-0.0.6a0/src/biogeme_optimization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7910 2024-03-27 13:04:11.000000 biogeme-optimization-0.0.6a0/src/biogeme_optimization/algebra.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2923 2024-03-27 13:04:11.000000 biogeme-optimization-0.0.6a0/src/biogeme_optimization/bfgs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1963 2024-03-27 13:04:11.000000 biogeme-optimization-0.0.6a0/src/biogeme_optimization/biogeme_logging.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33178 2024-03-27 13:04:11.000000 biogeme-optimization-0.0.6a0/src/biogeme_optimization/bounds.py
+-rw-r--r--   0 runner    (1001) docker     (127)      819 2024-03-27 13:04:11.000000 biogeme-optimization-0.0.6a0/src/biogeme_optimization/diagnostics.py
+-rw-r--r--   0 runner    (1001) docker     (127)      203 2024-03-27 13:04:11.000000 biogeme-optimization-0.0.6a0/src/biogeme_optimization/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2848 2024-03-27 13:04:11.000000 biogeme-optimization-0.0.6a0/src/biogeme_optimization/format.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14015 2024-03-27 13:04:11.000000 biogeme-optimization-0.0.6a0/src/biogeme_optimization/function.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6865 2024-03-27 13:04:11.000000 biogeme-optimization-0.0.6a0/src/biogeme_optimization/hybrid_function.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12183 2024-03-27 13:04:11.000000 biogeme-optimization-0.0.6a0/src/biogeme_optimization/linesearch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8623 2024-03-27 13:04:11.000000 biogeme-optimization-0.0.6a0/src/biogeme_optimization/neighborhood.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14417 2024-03-27 13:04:11.000000 biogeme-optimization-0.0.6a0/src/biogeme_optimization/pareto.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12142 2024-03-27 13:04:11.000000 biogeme-optimization-0.0.6a0/src/biogeme_optimization/simple_bounds.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13907 2024-03-27 13:04:11.000000 biogeme-optimization-0.0.6a0/src/biogeme_optimization/stochastic_function.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10063 2024-03-27 13:04:11.000000 biogeme-optimization-0.0.6a0/src/biogeme_optimization/stochastic_simple_bounds.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 13:04:33.970361 biogeme-optimization-0.0.6a0/src/biogeme_optimization/teaching/
+-rw-r--r--   0 runner    (1001) docker     (127)     1536 2024-03-27 13:04:11.000000 biogeme-optimization-0.0.6a0/src/biogeme_optimization/teaching/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 13:04:33.970361 biogeme-optimization-0.0.6a0/src/biogeme_optimization/teaching/linear_constraints/
+-rw-r--r--   0 runner    (1001) docker     (127)      346 2024-03-27 13:04:11.000000 biogeme-optimization-0.0.6a0/src/biogeme_optimization/teaching/linear_constraints/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16859 2024-03-27 13:04:11.000000 biogeme-optimization-0.0.6a0/src/biogeme_optimization/teaching/linear_constraints/constraint.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17255 2024-03-27 13:04:11.000000 biogeme-optimization-0.0.6a0/src/biogeme_optimization/teaching/linear_constraints/linear_constraints.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9257 2024-03-27 13:04:11.000000 biogeme-optimization-0.0.6a0/src/biogeme_optimization/teaching/linear_constraints/standard_canonical.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2050 2024-03-27 13:04:11.000000 biogeme-optimization-0.0.6a0/src/biogeme_optimization/teaching/linear_constraints/variable.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1679 2024-03-27 13:04:11.000000 biogeme-optimization-0.0.6a0/src/biogeme_optimization/teaching/matrices.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1907 2024-03-27 13:04:11.000000 biogeme-optimization-0.0.6a0/src/biogeme_optimization/teaching/plot_function.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5145 2024-03-27 13:04:11.000000 biogeme-optimization-0.0.6a0/src/biogeme_optimization/teaching/polyhedron_2d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3518 2024-03-27 13:04:11.000000 biogeme-optimization-0.0.6a0/src/biogeme_optimization/teaching/variables.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22515 2024-03-27 13:04:11.000000 biogeme-optimization-0.0.6a0/src/biogeme_optimization/trust_region.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8279 2024-03-27 13:04:11.000000 biogeme-optimization-0.0.6a0/src/biogeme_optimization/vns.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 13:04:33.974361 biogeme-optimization-0.0.6a0/src/biogeme_optimization.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3609 2024-03-27 13:04:33.000000 biogeme-optimization-0.0.6a0/src/biogeme_optimization.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1994 2024-03-27 13:04:33.000000 biogeme-optimization-0.0.6a0/src/biogeme_optimization.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-27 13:04:33.000000 biogeme-optimization-0.0.6a0/src/biogeme_optimization.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-03-27 13:04:33.000000 biogeme-optimization-0.0.6a0/src/biogeme_optimization.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-03-27 13:04:33.000000 biogeme-optimization-0.0.6a0/src/biogeme_optimization.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 13:04:33.974361 biogeme-optimization-0.0.6a0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     6377 2024-03-27 13:04:11.000000 biogeme-optimization-0.0.6a0/tests/test_algebra.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3644 2024-03-27 13:04:11.000000 biogeme-optimization-0.0.6a0/tests/test_bfgs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    53852 2024-03-27 13:04:11.000000 biogeme-optimization-0.0.6a0/tests/test_bounds.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4117 2024-03-27 13:04:11.000000 biogeme-optimization-0.0.6a0/tests/test_constraints.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2923 2024-03-27 13:04:11.000000 biogeme-optimization-0.0.6a0/tests/test_function.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4552 2024-03-27 13:04:11.000000 biogeme-optimization-0.0.6a0/tests/test_hybrid_function.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5263 2024-03-27 13:04:11.000000 biogeme-optimization-0.0.6a0/tests/test_linear_constraints.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10168 2024-03-27 13:04:11.000000 biogeme-optimization-0.0.6a0/tests/test_linesearch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3192 2024-03-27 13:04:11.000000 biogeme-optimization-0.0.6a0/tests/test_matrices.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4799 2024-03-27 13:04:11.000000 biogeme-optimization-0.0.6a0/tests/test_neighborhood.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6402 2024-03-27 13:04:11.000000 biogeme-optimization-0.0.6a0/tests/test_pareto.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1465 2024-03-27 13:04:11.000000 biogeme-optimization-0.0.6a0/tests/test_plot_function.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10094 2024-03-27 13:04:11.000000 biogeme-optimization-0.0.6a0/tests/test_simple_bounds.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3271 2024-03-27 13:04:11.000000 biogeme-optimization-0.0.6a0/tests/test_standard_canonical.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23343 2024-03-27 13:04:11.000000 biogeme-optimization-0.0.6a0/tests/test_trust_region.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3389 2024-03-27 13:04:11.000000 biogeme-optimization-0.0.6a0/tests/test_variables.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3674 2024-03-27 13:04:11.000000 biogeme-optimization-0.0.6a0/tests/test_vns.py
```

### Comparing `biogeme-optimization-0.0.6/PKG-INFO` & `biogeme-optimization-0.0.6a0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: biogeme-optimization
-Version: 0.0.6
+Version: 0.0.6a0
 Summary: Various optimization algorithms for teaching and research
 Home-page: http://biogeme.epfl.ch
 Author: Michel Bierlaire
 Author-email: michel.bierlaire@epfl.ch
 Project-URL: Code, https://github.com/michelbierlaire/optimization
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
```

### Comparing `biogeme-optimization-0.0.6/README.md` & `biogeme-optimization-0.0.6a0/README.md`

 * *Files identical despite different names*

### Comparing `biogeme-optimization-0.0.6/setup.cfg` & `biogeme-optimization-0.0.6a0/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = biogeme-optimization
-version = 0.0.6
+version = 0.0.6a0
 description = Various optimization algorithms for teaching and research
 long_description = file: README.md
 long_description_content_type = text/markdown
 author = Michel Bierlaire
 author_email = michel.bierlaire@epfl.ch
 url = http://biogeme.epfl.ch
 download_urls = https://pypi.org/project/bierlaire-optimization
```

### Comparing `biogeme-optimization-0.0.6/src/biogeme_optimization/algebra.py` & `biogeme-optimization-0.0.6a0/src/biogeme_optimization/algebra.py`

 * *Files identical despite different names*

### Comparing `biogeme-optimization-0.0.6/src/biogeme_optimization/bfgs.py` & `biogeme-optimization-0.0.6a0/src/biogeme_optimization/bfgs.py`

 * *Files identical despite different names*

### Comparing `biogeme-optimization-0.0.6/src/biogeme_optimization/biogeme_logging.py` & `biogeme-optimization-0.0.6a0/src/biogeme_optimization/biogeme_logging.py`

 * *Files identical despite different names*

### Comparing `biogeme-optimization-0.0.6/src/biogeme_optimization/bounds.py` & `biogeme-optimization-0.0.6a0/src/biogeme_optimization/bounds.py`

 * *Files identical despite different names*

### Comparing `biogeme-optimization-0.0.6/src/biogeme_optimization/diagnostics.py` & `biogeme-optimization-0.0.6a0/src/biogeme_optimization/diagnostics.py`

 * *Files identical despite different names*

### Comparing `biogeme-optimization-0.0.6/src/biogeme_optimization/format.py` & `biogeme-optimization-0.0.6a0/src/biogeme_optimization/format.py`

 * *Files identical despite different names*

### Comparing `biogeme-optimization-0.0.6/src/biogeme_optimization/function.py` & `biogeme-optimization-0.0.6a0/src/biogeme_optimization/function.py`

 * *Files identical despite different names*

### Comparing `biogeme-optimization-0.0.6/src/biogeme_optimization/hybrid_function.py` & `biogeme-optimization-0.0.6a0/src/biogeme_optimization/hybrid_function.py`

 * *Files identical despite different names*

### Comparing `biogeme-optimization-0.0.6/src/biogeme_optimization/linesearch.py` & `biogeme-optimization-0.0.6a0/src/biogeme_optimization/linesearch.py`

 * *Files identical despite different names*

### Comparing `biogeme-optimization-0.0.6/src/biogeme_optimization/neighborhood.py` & `biogeme-optimization-0.0.6a0/src/biogeme_optimization/neighborhood.py`

 * *Files identical despite different names*

### Comparing `biogeme-optimization-0.0.6/src/biogeme_optimization/pareto.py` & `biogeme-optimization-0.0.6a0/src/biogeme_optimization/pareto.py`

 * *Files identical despite different names*

### Comparing `biogeme-optimization-0.0.6/src/biogeme_optimization/simple_bounds.py` & `biogeme-optimization-0.0.6a0/src/biogeme_optimization/simple_bounds.py`

 * *Files identical despite different names*

### Comparing `biogeme-optimization-0.0.6/src/biogeme_optimization/stochastic_function.py` & `biogeme-optimization-0.0.6a0/src/biogeme_optimization/stochastic_function.py`

 * *Files identical despite different names*

### Comparing `biogeme-optimization-0.0.6/src/biogeme_optimization/stochastic_simple_bounds.py` & `biogeme-optimization-0.0.6a0/src/biogeme_optimization/stochastic_simple_bounds.py`

 * *Files identical despite different names*

### Comparing `biogeme-optimization-0.0.6/src/biogeme_optimization/teaching/linear_constraints/constraint.py` & `biogeme-optimization-0.0.6a0/src/biogeme_optimization/teaching/linear_constraints/constraint.py`

 * *Files 5% similar despite different names*

```diff
@@ -453,28 +453,21 @@
         :param vector_x: vector of interest
         :param indices: mapping between the unsorted_set_of_variables and the indices.
         :return: feasibility status
         """
         lhs = self.calculate_left_hand_side(vector_x=vector_x, indices=indices)
 
         def check_lesser_or_equal() -> bool:
-            slack = self.right_hand_side - lhs
-            if np.isclose(slack, 0, atol=np.finfo(float).eps):
-                return True
-            return slack >= 0.0
+            return lhs <= self.right_hand_side
 
         def check_greater_or_equal() -> bool:
-            slack = lhs - self.right_hand_side
-            if np.isclose(slack, 0, atol=np.finfo(float).eps):
-                return True
-            return slack >= 0.0
+            return lhs >= self.right_hand_side
 
         def check_equal() -> bool:
-            slack = lhs - self.right_hand_side
-            return np.isclose(slack, 0, atol=np.finfo(float).eps)
+            return lhs >= self.right_hand_side
 
         dict_of_check: dict[SignConstraint, Callable[[], bool]] = {
             SignConstraint.GREATER_OR_EQUAL: check_greater_or_equal,
             SignConstraint.LESSER_OR_EQUAL: check_lesser_or_equal,
             SignConstraint.EQUAL: check_equal,
         }
         return dict_of_check[self.sign]()
```

### Comparing `biogeme-optimization-0.0.6/src/biogeme_optimization/teaching/linear_constraints/linear_constraints.py` & `biogeme-optimization-0.0.6a0/src/biogeme_optimization/teaching/linear_constraints/linear_constraints.py`

 * *Files 1% similar despite different names*

```diff
@@ -154,15 +154,14 @@
         the_list = find_columns_multiple_identity(matrix=matrix)
         slack_variables_indices = set([col_index for col_index, _ in the_list])
         slacked_constraints_indices = set([row_index for _, row_index in the_list])
         # Make sure the only entry in those columns is positive
         for col_index, row_index in the_list:
             if matrix[row_index, col_index] < 0:
                 matrix[row_index, :] = -matrix[row_index, :]
-                vector[row_index] = -vector[row_index]
 
         regular_variables_indices = set(range(n_variables)) - slack_variables_indices
         regular_variables = {
             index: Variable(
                 name=f'x_{index}', sign=SignVariable.NON_NEGATIVE, slack=False
             )
             for index in regular_variables_indices
```

### Comparing `biogeme-optimization-0.0.6/src/biogeme_optimization/teaching/linear_constraints/standard_canonical.py` & `biogeme-optimization-0.0.6a0/src/biogeme_optimization/teaching/linear_constraints/standard_canonical.py`

 * *Files 7% similar despite different names*

```diff
@@ -195,32 +195,7 @@
                         - standard_x[standard_minus_index]
                     )
             else:
                 error_msg = f'Cannot identify standard variable {variable.name}.'
                 raise ValueError(error_msg)
         assert not np.any(np.isnan(canonical_x)), 'The vector contains NaN entries.'
         return canonical_x
-
-
-def canonical_to_standard(
-    canonical_a: np.ndarray, canonical_b: np.ndarray
-) -> tuple[np.ndarray, np.ndarray, str]:
-    """
-    Transforms a polyhedron in canonical form into one in standard form.
-
-    :param canonical_a: constraints matrix $A$ for the canonical form.
-    :param canonical_b: right hand side for the canonical form.
-    :return: three items:
-
-        - constraints matrix $A$ for the standard form,
-        - right hand side for the standard form,
-        - description of the constraints in standard form.
-    """
-    the_constraints = AllConstraints.from_canonical_form(
-        matrix=canonical_a, vector=canonical_b
-    )
-    the_forms = StandardCanonicalForms(constraints=the_constraints)
-    return (
-        the_forms.standard_matrix,
-        the_forms.standard_vector,
-        str(the_forms.standard_form),
-    )
```

### Comparing `biogeme-optimization-0.0.6/src/biogeme_optimization/teaching/linear_constraints/variable.py` & `biogeme-optimization-0.0.6a0/src/biogeme_optimization/teaching/linear_constraints/variable.py`

 * *Files identical despite different names*

### Comparing `biogeme-optimization-0.0.6/src/biogeme_optimization/teaching/plot_function.py` & `biogeme-optimization-0.0.6a0/src/biogeme_optimization/teaching/plot_function.py`

 * *Files identical despite different names*

### Comparing `biogeme-optimization-0.0.6/src/biogeme_optimization/teaching/variables.py` & `biogeme-optimization-0.0.6a0/src/biogeme_optimization/teaching/variables.py`

 * *Files identical despite different names*

### Comparing `biogeme-optimization-0.0.6/src/biogeme_optimization/trust_region.py` & `biogeme-optimization-0.0.6a0/src/biogeme_optimization/trust_region.py`

 * *Files identical despite different names*

### Comparing `biogeme-optimization-0.0.6/src/biogeme_optimization/vns.py` & `biogeme-optimization-0.0.6a0/src/biogeme_optimization/vns.py`

 * *Files identical despite different names*

### Comparing `biogeme-optimization-0.0.6/src/biogeme_optimization.egg-info/PKG-INFO` & `biogeme-optimization-0.0.6a0/src/biogeme_optimization.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: biogeme-optimization
-Version: 0.0.6
+Version: 0.0.6a0
 Summary: Various optimization algorithms for teaching and research
 Home-page: http://biogeme.epfl.ch
 Author: Michel Bierlaire
 Author-email: michel.bierlaire@epfl.ch
 Project-URL: Code, https://github.com/michelbierlaire/optimization
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
```

### Comparing `biogeme-optimization-0.0.6/src/biogeme_optimization.egg-info/SOURCES.txt` & `biogeme-optimization-0.0.6a0/src/biogeme_optimization.egg-info/SOURCES.txt`

 * *Files 25% similar despite different names*

```diff
@@ -21,44 +21,33 @@
 src/biogeme_optimization/vns.py
 src/biogeme_optimization.egg-info/PKG-INFO
 src/biogeme_optimization.egg-info/SOURCES.txt
 src/biogeme_optimization.egg-info/dependency_links.txt
 src/biogeme_optimization.egg-info/requires.txt
 src/biogeme_optimization.egg-info/top_level.txt
 src/biogeme_optimization/teaching/__init__.py
-src/biogeme_optimization/teaching/linear_optimization.py
 src/biogeme_optimization/teaching/matrices.py
 src/biogeme_optimization/teaching/plot_function.py
-src/biogeme_optimization/teaching/simplex.py
-src/biogeme_optimization/teaching/tableau.py
-src/biogeme_optimization/teaching/to_jupyter.py
+src/biogeme_optimization/teaching/polyhedron_2d.py
 src/biogeme_optimization/teaching/variables.py
 src/biogeme_optimization/teaching/linear_constraints/__init__.py
 src/biogeme_optimization/teaching/linear_constraints/constraint.py
-src/biogeme_optimization/teaching/linear_constraints/draw_polyhedron.py
 src/biogeme_optimization/teaching/linear_constraints/linear_constraints.py
-src/biogeme_optimization/teaching/linear_constraints/polyhedron_2d.py
 src/biogeme_optimization/teaching/linear_constraints/standard_canonical.py
-src/biogeme_optimization/teaching/linear_constraints/standard_form.py
 src/biogeme_optimization/teaching/linear_constraints/variable.py
 tests/test_algebra.py
 tests/test_bfgs.py
 tests/test_bounds.py
 tests/test_constraints.py
 tests/test_function.py
 tests/test_hybrid_function.py
 tests/test_linear_constraints.py
-tests/test_linear_optimization.py
 tests/test_linesearch.py
 tests/test_matrices.py
 tests/test_neighborhood.py
 tests/test_pareto.py
 tests/test_plot_function.py
-tests/test_polyhedron_2d.py
 tests/test_simple_bounds.py
-tests/test_simplex.py
 tests/test_standard_canonical.py
-tests/test_standard_form.py
-tests/test_tableau.py
 tests/test_trust_region.py
 tests/test_variables.py
 tests/test_vns.py
```

### Comparing `biogeme-optimization-0.0.6/tests/test_algebra.py` & `biogeme-optimization-0.0.6a0/tests/test_algebra.py`

 * *Files identical despite different names*

### Comparing `biogeme-optimization-0.0.6/tests/test_bfgs.py` & `biogeme-optimization-0.0.6a0/tests/test_bfgs.py`

 * *Files identical despite different names*

### Comparing `biogeme-optimization-0.0.6/tests/test_bounds.py` & `biogeme-optimization-0.0.6a0/tests/test_bounds.py`

 * *Files identical despite different names*

### Comparing `biogeme-optimization-0.0.6/tests/test_constraints.py` & `biogeme-optimization-0.0.6a0/tests/test_constraints.py`

 * *Files identical despite different names*

### Comparing `biogeme-optimization-0.0.6/tests/test_function.py` & `biogeme-optimization-0.0.6a0/tests/test_function.py`

 * *Files identical despite different names*

### Comparing `biogeme-optimization-0.0.6/tests/test_hybrid_function.py` & `biogeme-optimization-0.0.6a0/tests/test_hybrid_function.py`

 * *Files identical despite different names*

### Comparing `biogeme-optimization-0.0.6/tests/test_linear_constraints.py` & `biogeme-optimization-0.0.6a0/tests/test_linear_constraints.py`

 * *Files identical despite different names*

### Comparing `biogeme-optimization-0.0.6/tests/test_linesearch.py` & `biogeme-optimization-0.0.6a0/tests/test_linesearch.py`

 * *Files identical despite different names*

### Comparing `biogeme-optimization-0.0.6/tests/test_neighborhood.py` & `biogeme-optimization-0.0.6a0/tests/test_neighborhood.py`

 * *Files identical despite different names*

### Comparing `biogeme-optimization-0.0.6/tests/test_pareto.py` & `biogeme-optimization-0.0.6a0/tests/test_pareto.py`

 * *Files identical despite different names*

### Comparing `biogeme-optimization-0.0.6/tests/test_plot_function.py` & `biogeme-optimization-0.0.6a0/tests/test_plot_function.py`

 * *Files identical despite different names*

### Comparing `biogeme-optimization-0.0.6/tests/test_simple_bounds.py` & `biogeme-optimization-0.0.6a0/tests/test_simple_bounds.py`

 * *Files identical despite different names*

### Comparing `biogeme-optimization-0.0.6/tests/test_standard_canonical.py` & `biogeme-optimization-0.0.6a0/tests/test_standard_canonical.py`

 * *Files identical despite different names*

### Comparing `biogeme-optimization-0.0.6/tests/test_trust_region.py` & `biogeme-optimization-0.0.6a0/tests/test_trust_region.py`

 * *Files identical despite different names*

### Comparing `biogeme-optimization-0.0.6/tests/test_variables.py` & `biogeme-optimization-0.0.6a0/tests/test_variables.py`

 * *Files identical despite different names*

### Comparing `biogeme-optimization-0.0.6/tests/test_vns.py` & `biogeme-optimization-0.0.6a0/tests/test_vns.py`

 * *Files identical despite different names*

