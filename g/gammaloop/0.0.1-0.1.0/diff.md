# Comparing `tmp/gammaloop-0.0.1.tar.gz` & `tmp/gammaloop-0.1.0.tar.gz`

## Comparing `gammaloop-0.0.1.tar` & `gammaloop-0.1.0.tar`

### file list

```diff
@@ -1,99 +1,516 @@
--rw-r--r--   0        0        0     1832 1970-01-01 00:00:00.000000 gammaloop-0.0.1/Cargo.toml
--rw-r--r--   0      501       20     2119 2023-09-12 23:04:29.000000 gammaloop-0.0.1/.gitignore
--rw-r--r--   0      501       20    38525 2023-09-13 15:42:22.000000 gammaloop-0.0.1/Cargo.lock
--rw-r--r--   0      501       20      195 2023-09-12 21:50:55.000000 gammaloop-0.0.1/LICENSE.md
--rw-r--r--   0      501       20      195 2023-09-12 21:50:55.000000 gammaloop-0.0.1/License.md
--rw-r--r--   0      501       20     2576 2023-09-12 22:14:58.000000 gammaloop-0.0.1/README.md
--rwxr-xr-x   0      501       20      443 2023-09-13 16:09:24.000000 gammaloop-0.0.1/bin/build_dependencies.sh
--rwxr-xr-x   0      501       20       96 2023-09-13 16:06:49.000000 gammaloop-0.0.1/bin/compile.sh
--rwxr-xr-x   0      501       20      117 2023-09-13 16:04:49.000000 gammaloop-0.0.1/bin/compile_bin.sh
--rwxr-xr-x   0      501       20      349 2023-09-13 16:05:03.000000 gammaloop-0.0.1/bin/compile_lib.sh
--rwxr-xr-x   0      501       20      296 2023-09-11 14:53:20.000000 gammaloop-0.0.1/bin/gammaloop
--rwxr-xr-x   0      501       20      975 2023-09-12 22:07:20.000000 gammaloop-0.0.1/bin/run_tests.sh
--rwxr-xr-x   0      501       20      882 2023-09-13 16:22:49.000000 gammaloop-0.0.1/bin/test_deployment.sh
--rw-r--r--   0      501       20      368 2023-09-11 15:49:19.000000 gammaloop-0.0.1/build.rs
--rw-r--r--   0      501       20      252 2023-09-07 13:50:13.000000 gammaloop-0.0.1/dependencies/fjcore/Makefile
--rw-r--r--   0      501       20   234477 2023-09-07 13:50:13.000000 gammaloop-0.0.1/dependencies/fjcore/fjcore.cc
--rw-r--r--   0      501       20    71944 2023-09-07 13:50:13.000000 gammaloop-0.0.1/dependencies/fjcore/fjcore.hh
--rw-r--r--   0      501       20     9295 2023-09-07 13:50:13.000000 gammaloop-0.0.1/dependencies/fjcore/wrapper.cc
--rw-r--r--   0      501       20      972 2023-09-13 16:19:06.000000 gammaloop-0.0.1/pyproject.toml
--rw-r--r--   0      501       20     2310 2023-09-11 16:40:08.000000 gammaloop-0.0.1/python/gammaloop/__init__.py
--rw-r--r--   0      501       20        0 2023-09-01 11:42:35.000000 gammaloop-0.0.1/python/gammaloop/base_objects/__init__.py
--rw-r--r--   0      501       20     2064 2023-09-12 18:00:52.000000 gammaloop-0.0.1/python/gammaloop/base_objects/graph.py
--rw-r--r--   0      501       20    23199 2023-09-12 17:46:23.000000 gammaloop-0.0.1/python/gammaloop/base_objects/model.py
--rw-r--r--   0      501       20        0 2023-09-11 14:36:09.000000 gammaloop-0.0.1/python/gammaloop/bin/__init__.py
--rwxr-xr-x   0      501       20      296 2023-09-11 14:53:20.000000 gammaloop-0.0.1/python/gammaloop/bin/gammaloop
--rw-r--r--   0      501       20        0 2023-09-05 12:02:31.000000 gammaloop-0.0.1/python/gammaloop/cross_section/__init__.py
--rw-r--r--   0      501       20     1325 2023-09-06 14:12:34.000000 gammaloop-0.0.1/python/gammaloop/cross_section/supergraph.py
--rw-r--r--   0      501       20       35 2023-09-11 16:39:41.000000 gammaloop-0.0.1/python/gammaloop/data/config/symbolica_license.txt
--rw-r--r--   0      501       20      637 2023-09-05 08:40:18.000000 gammaloop-0.0.1/python/gammaloop/data/models/scalars/__init__.py
--rw-r--r--   0      501       20      414 2023-09-05 08:10:36.000000 gammaloop-0.0.1/python/gammaloop/data/models/scalars/coupling_orders.py
--rw-r--r--   0      501       20      224 2023-09-05 08:53:45.000000 gammaloop-0.0.1/python/gammaloop/data/models/scalars/couplings.py
--rw-r--r--   0      501       20     1340 2023-09-05 08:07:27.000000 gammaloop-0.0.1/python/gammaloop/data/models/scalars/function_library.py
--rw-r--r--   0      501       20      537 2023-09-05 09:29:12.000000 gammaloop-0.0.1/python/gammaloop/data/models/scalars/lorentz.py
--rw-r--r--   0      501       20     7078 2023-09-05 08:07:27.000000 gammaloop-0.0.1/python/gammaloop/data/models/scalars/object_library.py
--rw-r--r--   0      501       20     3315 2023-09-05 09:24:52.000000 gammaloop-0.0.1/python/gammaloop/data/models/scalars/parameters.py
--rw-r--r--   0      501       20      938 2023-09-05 08:39:38.000000 gammaloop-0.0.1/python/gammaloop/data/models/scalars/particles.py
--rw-r--r--   0      501       20     1761 2023-09-05 09:24:12.000000 gammaloop-0.0.1/python/gammaloop/data/models/scalars/restrict_default.dat
--rwxr-xr-x   0      501       20      514 2023-09-05 09:13:37.000000 gammaloop-0.0.1/python/gammaloop/data/models/scalars/run_write_param_card.py
--rw-r--r--   0      501       20     1078 2023-09-05 09:02:20.000000 gammaloop-0.0.1/python/gammaloop/data/models/scalars/vertices.py
--rw-r--r--   0      501       20     6805 2023-09-05 09:13:30.000000 gammaloop-0.0.1/python/gammaloop/data/models/scalars/write_param_card.py
--rw-r--r--   0      501       20      873 2023-09-01 11:54:08.000000 gammaloop-0.0.1/python/gammaloop/data/models/sm/__init__.py
--rw-r--r--   0      501       20     2860 2023-09-01 11:54:08.000000 gammaloop-0.0.1/python/gammaloop/data/models/sm/build_restrict.py
--rw-r--r--   0      501       20      483 2023-09-01 11:54:08.000000 gammaloop-0.0.1/python/gammaloop/data/models/sm/coupling_orders.py
--rw-r--r--   0      501       20    14158 2023-09-01 11:54:08.000000 gammaloop-0.0.1/python/gammaloop/data/models/sm/couplings.py
--rw-r--r--   0      501       20    13626 2023-09-01 11:54:08.000000 gammaloop-0.0.1/python/gammaloop/data/models/sm/decays.py
--rw-r--r--   0      501       20     1340 2023-09-01 11:54:08.000000 gammaloop-0.0.1/python/gammaloop/data/models/sm/function_library.py
--rw-r--r--   0      501       20     3363 2023-09-01 11:54:08.000000 gammaloop-0.0.1/python/gammaloop/data/models/sm/lorentz.py
--rw-r--r--   0      501       20     7078 2023-09-01 11:54:08.000000 gammaloop-0.0.1/python/gammaloop/data/models/sm/object_library.py
--rw-r--r--   0      501       20    15734 2023-09-01 11:54:08.000000 gammaloop-0.0.1/python/gammaloop/data/models/sm/parameters.py
--rw-r--r--   0      501       20    10491 2023-09-01 11:54:08.000000 gammaloop-0.0.1/python/gammaloop/data/models/sm/particles.py
--rw-r--r--   0      501       20     1436 2023-09-01 11:54:08.000000 gammaloop-0.0.1/python/gammaloop/data/models/sm/restrict_VH.dat
--rw-r--r--   0      501       20     1437 2023-09-01 11:54:08.000000 gammaloop-0.0.1/python/gammaloop/data/models/sm/restrict_c_mass.dat
--rw-r--r--   0      501       20     1438 2023-09-01 11:54:08.000000 gammaloop-0.0.1/python/gammaloop/data/models/sm/restrict_ckm.dat
--rw-r--r--   0      501       20     1437 2023-09-01 11:54:08.000000 gammaloop-0.0.1/python/gammaloop/data/models/sm/restrict_default.dat
--rw-r--r--   0      501       20     1436 2023-09-01 11:54:08.000000 gammaloop-0.0.1/python/gammaloop/data/models/sm/restrict_lepton_masses.dat
--rw-r--r--   0      501       20     1438 2023-09-01 11:54:08.000000 gammaloop-0.0.1/python/gammaloop/data/models/sm/restrict_no_b_mass.dat
--rw-r--r--   0      501       20     1438 2023-09-01 11:54:08.000000 gammaloop-0.0.1/python/gammaloop/data/models/sm/restrict_no_masses.dat
--rw-r--r--   0      501       20     1437 2023-09-01 11:54:08.000000 gammaloop-0.0.1/python/gammaloop/data/models/sm/restrict_no_tau_mass.dat
--rw-r--r--   0      501       20     1438 2023-09-01 11:54:08.000000 gammaloop-0.0.1/python/gammaloop/data/models/sm/restrict_no_widths.dat
--rw-r--r--   0      501       20     1438 2023-09-01 11:54:08.000000 gammaloop-0.0.1/python/gammaloop/data/models/sm/restrict_zeromass_ckm.dat
--rwxr-xr-x   0      501       20      514 2023-09-05 09:13:55.000000 gammaloop-0.0.1/python/gammaloop/data/models/sm/run_write_param_card.py
--rw-r--r--   0      501       20    32557 2023-09-01 11:54:08.000000 gammaloop-0.0.1/python/gammaloop/data/models/sm/vertices.py
--rw-r--r--   0      501       20     6963 2023-09-01 11:54:08.000000 gammaloop-0.0.1/python/gammaloop/data/models/sm/write_param_card.py
--rw-r--r--   0      501       20       54 2023-09-12 15:36:28.000000 gammaloop-0.0.1/python/gammaloop/data/run_cards/cmd.gL
--rw-r--r--   0      501       20      833 2023-09-11 17:43:02.000000 gammaloop-0.0.1/python/gammaloop/data/run_cards/rust_run_config.yaml
--rw-r--r--   0      501       20       35 2023-09-12 06:40:58.000000 gammaloop-0.0.1/python/gammaloop/data/symbolica_license.txt
--rw-r--r--   0      501       20        0 2023-09-05 12:02:39.000000 gammaloop-0.0.1/python/gammaloop/exporters/__init__.py
--rw-r--r--   0      501       20        0 2023-09-11 15:40:13.000000 gammaloop-0.0.1/python/gammaloop/gammaloop.pyi
--rw-r--r--   0      501       20        0 2023-09-01 09:32:10.000000 gammaloop-0.0.1/python/gammaloop/interface/__init__.py
--rw-r--r--   0      501       20     7964 2023-09-12 19:47:25.000000 gammaloop-0.0.1/python/gammaloop/interface/gammaloop_interface.py
--rw-r--r--   0      501       20        0 2023-09-01 09:38:23.000000 gammaloop-0.0.1/python/gammaloop/misc/__init__.py
--rw-r--r--   0      501       20     2366 2023-09-13 16:15:51.000000 gammaloop-0.0.1/python/gammaloop/misc/common.py
--rw-r--r--   0      501       20     3210 2023-09-12 16:14:42.000000 gammaloop-0.0.1/python/gammaloop/misc/utils.py
--rw-r--r--   0      501       20        0 2023-09-11 15:39:58.000000 gammaloop-0.0.1/python/gammaloop/py.typed
--rw-r--r--   0      501       20       30 2023-09-12 22:17:41.000000 gammaloop-0.0.1/python/gammaloop/requirements.txt
--rwxr-xr-x   0      501       20       86 2023-09-11 16:50:00.000000 gammaloop-0.0.1/python/gammaloop/run_python_tests.sh
--rw-r--r--   0      501       20      190 2023-09-11 16:41:13.000000 gammaloop-0.0.1/python/gammaloop/tests/__init__.py
--rw-r--r--   0      501       20      381 2023-09-12 17:48:01.000000 gammaloop-0.0.1/python/gammaloop/tests/common.py
--rw-r--r--   0      501       20        0 2023-09-05 10:38:09.000000 gammaloop-0.0.1/python/gammaloop/tests/integration/__init__.py
--rw-r--r--   0      501       20      273 2023-09-12 18:02:59.000000 gammaloop-0.0.1/python/gammaloop/tests/integration/test_integral.py
--rw-r--r--   0      501       20    13004 2023-09-05 12:46:18.000000 gammaloop-0.0.1/python/gammaloop/tests/test_data/qgraf_outputs/epem_a_ddx_NLO.py
--rw-r--r--   0      501       20        0 2023-09-05 10:38:04.000000 gammaloop-0.0.1/python/gammaloop/tests/unit/__init__.py
--rw-r--r--   0      501       20      423 2023-09-13 10:24:42.000000 gammaloop-0.0.1/python/gammaloop/tests/unit/conftest.py
--rw-r--r--   0      501       20     1779 2023-09-12 18:03:17.000000 gammaloop-0.0.1/python/gammaloop/tests/unit/test_commands.py
--rw-r--r--   0      501       20     2803 2023-09-12 18:52:30.000000 gammaloop-0.0.1/src/api/python.rs
--rw-r--r--   0      501       20       47 2023-09-11 08:31:47.000000 gammaloop-0.0.1/src/api.rs
--rw-r--r--   0      501       20      460 2023-09-12 19:08:01.000000 gammaloop-0.0.1/src/bin/cli.rs
--rw-r--r--   0      501       20     8214 2023-09-12 19:02:45.000000 gammaloop-0.0.1/src/cli_functions.rs
--rw-r--r--   0      501       20     4163 2023-09-07 14:58:50.000000 gammaloop-0.0.1/src/h_function_test.rs
--rw-r--r--   0      501       20     2224 2023-09-12 19:03:07.000000 gammaloop-0.0.1/src/inspect.rs
--rw-r--r--   0      501       20    10045 2023-09-12 19:03:14.000000 gammaloop-0.0.1/src/integrands.rs
--rw-r--r--   0      501       20    15887 2023-09-13 15:43:03.000000 gammaloop-0.0.1/src/integrate.rs
--rw-r--r--   0      501       20     4826 2023-09-11 14:08:04.000000 gammaloop-0.0.1/src/lib.rs
--rw-r--r--   0      501       20    23453 2023-09-13 13:14:11.000000 gammaloop-0.0.1/src/model.rs
--rw-r--r--   0      501       20    42698 2023-09-12 19:03:49.000000 gammaloop-0.0.1/src/observables.rs
--rw-r--r--   0      501       20      472 2023-09-07 15:05:16.000000 gammaloop-0.0.1/src/test_resources/default_tests_config.yaml
--rw-r--r--   0      501       20    12081 2023-09-11 17:21:36.000000 gammaloop-0.0.1/src/tests.rs
--rw-r--r--   0      501       20    53158 2023-09-12 19:01:40.000000 gammaloop-0.0.1/src/utils.rs
--rw-r--r--   0        0        0     3263 1970-01-01 00:00:00.000000 gammaloop-0.0.1/PKG-INFO
+-rw-r--r--   0      501       20     1881 2024-04-02 19:06:10.000000 gammaloop-0.1.0/python/gammaloop/dependencies/symbolica/Cargo.toml
+-rw-r--r--   0      501       20      521 2024-04-02 19:06:10.000000 gammaloop-0.1.0/python/gammaloop/dependencies/symbolica/.envrc
+-rw-r--r--   0      501       20     1608 2024-04-02 19:06:10.000000 gammaloop-0.1.0/python/gammaloop/dependencies/symbolica/.github/workflows/symbolica_tests.yml
+-rw-r--r--   0      501       20       27 2024-04-02 19:06:10.000000 gammaloop-0.1.0/python/gammaloop/dependencies/symbolica/.gitignore
+-rw-r--r--   0      501       20    34268 2024-04-02 19:06:16.000000 gammaloop-0.1.0/python/gammaloop/dependencies/symbolica/Cargo.lock
+-rw-r--r--   0      501       20      812 2024-04-02 19:06:10.000000 gammaloop-0.1.0/python/gammaloop/dependencies/symbolica/License.md
+-rw-r--r--   0      501       20     5200 2024-04-02 19:06:10.000000 gammaloop-0.1.0/python/gammaloop/dependencies/symbolica/Readme.md
+-rw-r--r--   0      501       20      422 2024-04-02 19:06:10.000000 gammaloop-0.1.0/python/gammaloop/dependencies/symbolica/build.rs
+-rw-r--r--   0      501       20      362 2024-04-02 19:06:10.000000 gammaloop-0.1.0/python/gammaloop/dependencies/symbolica/examples/builder.rs
+-rw-r--r--   0      501       20      741 2024-04-02 19:06:10.000000 gammaloop-0.1.0/python/gammaloop/dependencies/symbolica/examples/coefficient_ring.rs
+-rw-r--r--   0      501       20     1062 2024-04-02 19:06:10.000000 gammaloop-0.1.0/python/gammaloop/dependencies/symbolica/examples/collect.rs
+-rw-r--r--   0      501       20      425 2024-04-02 19:06:10.000000 gammaloop-0.1.0/python/gammaloop/dependencies/symbolica/examples/derivative.rs
+-rw-r--r--   0      501       20     1172 2024-04-02 19:06:10.000000 gammaloop-0.1.0/python/gammaloop/dependencies/symbolica/examples/evaluate.rs
+-rw-r--r--   0      501       20      181 2024-04-02 19:06:10.000000 gammaloop-0.1.0/python/gammaloop/dependencies/symbolica/examples/expansion.rs
+-rw-r--r--   0      501       20     3956 2024-04-02 19:06:10.000000 gammaloop-0.1.0/python/gammaloop/dependencies/symbolica/examples/factorization.rs
+-rw-r--r--   0      501       20     1458 2024-04-02 19:06:10.000000 gammaloop-0.1.0/python/gammaloop/dependencies/symbolica/examples/fibonacci.rs
+-rw-r--r--   0      501       20     2392 2024-04-02 19:06:10.000000 gammaloop-0.1.0/python/gammaloop/dependencies/symbolica/examples/fuel_backend.rs
+-rw-r--r--   0      501       20     1193 2024-04-02 19:06:10.000000 gammaloop-0.1.0/python/gammaloop/dependencies/symbolica/examples/groebner_basis.rs
+-rw-r--r--   0      501       20     1362 2024-04-02 19:06:10.000000 gammaloop-0.1.0/python/gammaloop/dependencies/symbolica/examples/numerical_integration.rs
+-rw-r--r--   0      501       20   191465 2024-04-02 19:06:10.000000 gammaloop-0.1.0/python/gammaloop/dependencies/symbolica/examples/optimize.rs
+-rw-r--r--   0      501       20   191177 2024-04-02 19:06:10.000000 gammaloop-0.1.0/python/gammaloop/dependencies/symbolica/examples/optimize_multiple.rs
+-rw-r--r--   0      501       20     1329 2024-04-02 19:06:10.000000 gammaloop-0.1.0/python/gammaloop/dependencies/symbolica/examples/partial_fraction.rs
+-rw-r--r--   0      501       20      633 2024-04-02 19:06:10.000000 gammaloop-0.1.0/python/gammaloop/dependencies/symbolica/examples/partition.rs
+-rw-r--r--   0      501       20     1343 2024-04-02 19:06:10.000000 gammaloop-0.1.0/python/gammaloop/dependencies/symbolica/examples/pattern_match.rs
+-rw-r--r--   0      501       20     2806 2024-04-02 19:06:10.000000 gammaloop-0.1.0/python/gammaloop/dependencies/symbolica/examples/pattern_restrictions.rs
+-rw-r--r--   0      501       20     1700 2024-04-02 19:06:10.000000 gammaloop-0.1.0/python/gammaloop/dependencies/symbolica/examples/polynomial.rs
+-rw-r--r--   0      501       20     1191 2024-04-02 19:06:10.000000 gammaloop-0.1.0/python/gammaloop/dependencies/symbolica/examples/polynomial_gcd.rs
+-rw-r--r--   0      501       20      317 2024-04-02 19:06:10.000000 gammaloop-0.1.0/python/gammaloop/dependencies/symbolica/examples/rational_polynomial.rs
+-rw-r--r--   0      501       20      678 2024-04-02 19:06:10.000000 gammaloop-0.1.0/python/gammaloop/dependencies/symbolica/examples/rational_reconstruction.rs
+-rw-r--r--   0      501       20      326 2024-04-02 19:06:10.000000 gammaloop-0.1.0/python/gammaloop/dependencies/symbolica/examples/replace_all.rs
+-rw-r--r--   0      501       20      807 2024-04-02 19:06:10.000000 gammaloop-0.1.0/python/gammaloop/dependencies/symbolica/examples/replace_once.rs
+-rw-r--r--   0      501       20     2499 2024-04-02 19:06:10.000000 gammaloop-0.1.0/python/gammaloop/dependencies/symbolica/examples/solve_linear_system.rs
+-rw-r--r--   0      501       20      618 2024-04-02 19:06:10.000000 gammaloop-0.1.0/python/gammaloop/dependencies/symbolica/examples/streaming.rs
+-rw-r--r--   0      501       20      278 2024-04-02 19:06:10.000000 gammaloop-0.1.0/python/gammaloop/dependencies/symbolica/examples/taylor_series.rs
+-rw-r--r--   0      501       20     1351 2024-04-02 19:06:10.000000 gammaloop-0.1.0/python/gammaloop/dependencies/symbolica/examples/tree_replace.rs
+-rw-r--r--   0      501       20      495 2024-04-02 19:06:10.000000 gammaloop-0.1.0/python/gammaloop/dependencies/symbolica/examples/tree_walk.rs
+-rw-r--r--   0      501       20     2461 2024-04-02 19:06:10.000000 gammaloop-0.1.0/python/gammaloop/dependencies/symbolica/flake.lock
+-rw-r--r--   0      501       20     1649 2024-04-02 19:06:10.000000 gammaloop-0.1.0/python/gammaloop/dependencies/symbolica/flake.nix
+-rw-r--r--   0      501       20      691 2024-04-02 19:06:10.000000 gammaloop-0.1.0/python/gammaloop/dependencies/symbolica/pyproject.toml
+-rw-r--r--   0      501       20    14790 2024-04-02 19:06:10.000000 gammaloop-0.1.0/python/gammaloop/dependencies/symbolica/src/api/cpp.rs
+-rw-r--r--   0      501       20     7286 2024-04-02 19:06:10.000000 gammaloop-0.1.0/python/gammaloop/dependencies/symbolica/src/api/mathematica.rs
+-rw-r--r--   0      501       20   182082 2024-04-02 19:06:10.000000 gammaloop-0.1.0/python/gammaloop/dependencies/symbolica/src/api/python.rs
+-rw-r--r--   0      501       20      117 2024-04-02 19:06:10.000000 gammaloop-0.1.0/python/gammaloop/dependencies/symbolica/src/api.rs
+-rw-r--r--   0      501       20    33822 2024-04-02 19:06:10.000000 gammaloop-0.1.0/python/gammaloop/dependencies/symbolica/src/coefficient.rs
+-rw-r--r--   0      501       20     9518 2024-04-02 19:06:10.000000 gammaloop-0.1.0/python/gammaloop/dependencies/symbolica/src/collect.rs
+-rw-r--r--   0      501       20     9629 2024-04-02 19:06:10.000000 gammaloop-0.1.0/python/gammaloop/dependencies/symbolica/src/combinatorics.rs
+-rw-r--r--   0      501       20    16599 2024-04-02 19:06:10.000000 gammaloop-0.1.0/python/gammaloop/dependencies/symbolica/src/derivative.rs
+-rw-r--r--   0      501       20     7607 2024-04-02 19:06:10.000000 gammaloop-0.1.0/python/gammaloop/dependencies/symbolica/src/domains/algebraic_number.rs
+-rw-r--r--   0      501       20    34611 2024-04-02 19:06:10.000000 gammaloop-0.1.0/python/gammaloop/dependencies/symbolica/src/domains/factorized_rational_polynomial.rs
+-rw-r--r--   0      501       20    32040 2024-04-02 19:06:10.000000 gammaloop-0.1.0/python/gammaloop/dependencies/symbolica/src/domains/finite_field.rs
+-rw-r--r--   0      501       20    19712 2024-04-02 19:06:10.000000 gammaloop-0.1.0/python/gammaloop/dependencies/symbolica/src/domains/float.rs
+-rw-r--r--   0      501       20    48186 2024-04-02 19:06:10.000000 gammaloop-0.1.0/python/gammaloop/dependencies/symbolica/src/domains/integer.rs
+-rw-r--r--   0      501       20    15400 2024-04-02 19:06:10.000000 gammaloop-0.1.0/python/gammaloop/dependencies/symbolica/src/domains/linear_system.rs
+-rw-r--r--   0      501       20    28830 2024-04-02 19:06:10.000000 gammaloop-0.1.0/python/gammaloop/dependencies/symbolica/src/domains/rational.rs
+-rw-r--r--   0      501       20    24150 2024-04-02 19:06:10.000000 gammaloop-0.1.0/python/gammaloop/dependencies/symbolica/src/domains/rational_polynomial.rs
+-rw-r--r--   0      501       20     3157 2024-04-02 19:06:10.000000 gammaloop-0.1.0/python/gammaloop/dependencies/symbolica/src/domains.rs
+-rw-r--r--   0      501       20     5315 2024-04-02 19:06:10.000000 gammaloop-0.1.0/python/gammaloop/dependencies/symbolica/src/evaluate.rs
+-rw-r--r--   0      501       20    10704 2024-04-02 19:06:10.000000 gammaloop-0.1.0/python/gammaloop/dependencies/symbolica/src/expand.rs
+-rw-r--r--   0      501       20    87160 2024-04-02 19:06:10.000000 gammaloop-0.1.0/python/gammaloop/dependencies/symbolica/src/id.rs
+-rw-r--r--   0      501       20    17678 2024-04-02 19:06:10.000000 gammaloop-0.1.0/python/gammaloop/dependencies/symbolica/src/lib.rs
+-rw-r--r--   0      501       20    43250 2024-04-02 19:06:10.000000 gammaloop-0.1.0/python/gammaloop/dependencies/symbolica/src/normalize.rs
+-rw-r--r--   0      501       20    38912 2024-04-02 19:06:10.000000 gammaloop-0.1.0/python/gammaloop/dependencies/symbolica/src/numerical_integration.rs
+-rw-r--r--   0      501       20    44316 2024-04-02 19:06:10.000000 gammaloop-0.1.0/python/gammaloop/dependencies/symbolica/src/parser.rs
+-rw-r--r--   0      501       20    65447 2024-04-02 19:06:10.000000 gammaloop-0.1.0/python/gammaloop/dependencies/symbolica/src/poly/evaluate.rs
+-rw-r--r--   0      501       20   105286 2024-04-02 19:06:10.000000 gammaloop-0.1.0/python/gammaloop/dependencies/symbolica/src/poly/factor.rs
+-rwxr-xr-x   0      501       20   113386 2024-04-02 19:06:10.000000 gammaloop-0.1.0/python/gammaloop/dependencies/symbolica/src/poly/gcd.rs
+-rw-r--r--   0      501       20    31024 2024-04-02 19:06:10.000000 gammaloop-0.1.0/python/gammaloop/dependencies/symbolica/src/poly/groebner.rs
+-rwxr-xr-x   0      501       20   106868 2024-04-02 19:06:10.000000 gammaloop-0.1.0/python/gammaloop/dependencies/symbolica/src/poly/polynomial.rs
+-rw-r--r--   0      501       20    62700 2024-04-02 19:06:10.000000 gammaloop-0.1.0/python/gammaloop/dependencies/symbolica/src/poly.rs
+-rw-r--r--   0      501       20    40747 2024-04-02 19:06:10.000000 gammaloop-0.1.0/python/gammaloop/dependencies/symbolica/src/printer.rs
+-rw-r--r--   0      501       20    15177 2024-04-02 19:06:10.000000 gammaloop-0.1.0/python/gammaloop/dependencies/symbolica/src/representations/coefficient.rs
+-rw-r--r--   0      501       20    35254 2024-04-02 19:06:10.000000 gammaloop-0.1.0/python/gammaloop/dependencies/symbolica/src/representations/default.rs
+-rw-r--r--   0      501       20    27843 2024-04-02 19:06:10.000000 gammaloop-0.1.0/python/gammaloop/dependencies/symbolica/src/representations.rs
+-rw-r--r--   0      501       20     2999 2024-04-02 19:06:10.000000 gammaloop-0.1.0/python/gammaloop/dependencies/symbolica/src/solve.rs
+-rw-r--r--   0      501       20    12741 2024-04-02 19:06:10.000000 gammaloop-0.1.0/python/gammaloop/dependencies/symbolica/src/state.rs
+-rw-r--r--   0      501       20     4534 2024-04-02 19:06:10.000000 gammaloop-0.1.0/python/gammaloop/dependencies/symbolica/src/streaming.rs
+-rw-r--r--   0      501       20    23339 2024-04-02 19:06:10.000000 gammaloop-0.1.0/python/gammaloop/dependencies/symbolica/src/tensors/matrix.rs
+-rw-r--r--   0      501       20       16 2024-04-02 19:06:10.000000 gammaloop-0.1.0/python/gammaloop/dependencies/symbolica/src/tensors.rs
+-rw-r--r--   0      501       20    18012 2024-04-02 19:06:10.000000 gammaloop-0.1.0/python/gammaloop/dependencies/symbolica/src/transformer.rs
+-rw-r--r--   0      501       20      796 2024-04-02 19:06:10.000000 gammaloop-0.1.0/python/gammaloop/dependencies/symbolica/src/utils.rs
+-rw-r--r--   0      501       20    85476 2024-04-02 19:06:10.000000 gammaloop-0.1.0/python/gammaloop/dependencies/symbolica/symbolica.pyi
+-rw-r--r--   0        0        0     3110 1970-01-01 00:00:00.000000 gammaloop-0.1.0/Cargo.toml
+-rw-r--r--   0      501       20     1445 2024-04-02 22:34:14.000000 gammaloop-0.1.0/.github/workflows/gamma_loop_tests.yml
+-rw-r--r--   0      501       20     2753 2024-04-02 22:34:14.000000 gammaloop-0.1.0/.gitignore
+-rw-r--r--   0      501       20      323 2023-09-25 15:26:40.000000 gammaloop-0.1.0/.pylintrc
+-rw-r--r--   0      501       20    61585 2024-04-02 22:34:28.000000 gammaloop-0.1.0/Cargo.lock
+-rw-r--r--   0      501       20      195 2023-09-12 21:50:55.000000 gammaloop-0.1.0/LICENSE.md
+-rw-r--r--   0      501       20     4569 2024-04-02 22:34:14.000000 gammaloop-0.1.0/README.md
+-rw-r--r--   0      501       20     1006 2024-03-28 12:43:14.000000 gammaloop-0.1.0/WORKING/cards/new_run_card.yaml
+-rw-r--r--   0      501       20      952 2024-03-28 12:43:14.000000 gammaloop-0.1.0/WORKING/cards/old_run_card.yaml
+-rw-r--r--   0      501       20     1592 2024-03-28 12:43:14.000000 gammaloop-0.1.0/WORKING/cards/param_card.dat
+-rw-r--r--   0      501       20      273 2024-03-28 12:43:14.000000 gammaloop-0.1.0/WORKING/cards/proc_card.gL
+-rw-r--r--   0      501       20      958 2024-03-28 12:43:14.000000 gammaloop-0.1.0/WORKING/cards/run_card.yaml
+-rw-r--r--   0      501       20       74 2024-03-28 12:43:14.000000 gammaloop-0.1.0/WORKING/output_metadata.yaml
+-rw-r--r--   0      501       20      134 2024-03-28 12:43:14.000000 gammaloop-0.1.0/WORKING/runs/run.yaml
+-rw-r--r--   0      501       20     2455 2024-03-28 12:43:14.000000 gammaloop-0.1.0/WORKING/sources/amplitudes/massless_triangle/amplitude.yaml
+-rw-r--r--   0      501       20     5995 2024-03-28 12:43:14.000000 gammaloop-0.1.0/WORKING/sources/amplitudes/massless_triangle/derived_data_massless_triangle_0.bin
+-rw-r--r--   0      501       20        8 2024-03-28 12:43:14.000000 gammaloop-0.1.0/WORKING/sources/amplitudes/massless_triangle/drawings/0_massless_triangle_0.aux
+-rw-r--r--   0      501       20     1204 2024-03-28 12:43:14.000000 gammaloop-0.1.0/WORKING/sources/amplitudes/massless_triangle/drawings/0_massless_triangle_0.dvi
+-rw-r--r--   0      501       20     9894 2024-03-28 12:43:14.000000 gammaloop-0.1.0/WORKING/sources/amplitudes/massless_triangle/drawings/0_massless_triangle_0.log
+-rw-r--r--   0      501       20    18374 2024-03-28 12:43:14.000000 gammaloop-0.1.0/WORKING/sources/amplitudes/massless_triangle/drawings/0_massless_triangle_0.pdf
+-rw-r--r--   0      501       20   187556 2024-03-28 12:43:14.000000 gammaloop-0.1.0/WORKING/sources/amplitudes/massless_triangle/drawings/0_massless_triangle_0.ps
+-rw-r--r--   0      501       20     5889 2024-03-28 12:43:14.000000 gammaloop-0.1.0/WORKING/sources/amplitudes/massless_triangle/drawings/0_massless_triangle_0.tex
+-rw-r--r--   0      501       20    18214 2024-03-28 12:43:14.000000 gammaloop-0.1.0/WORKING/sources/amplitudes/massless_triangle/drawings/all_graphs.pdf
+-rwxr-xr-x   0      501       20     2885 2024-03-28 12:43:14.000000 gammaloop-0.1.0/WORKING/sources/amplitudes/massless_triangle/drawings/combine_pages.py
+-rw-r--r--   0      501       20     6805 2024-03-28 12:43:14.000000 gammaloop-0.1.0/WORKING/sources/amplitudes/massless_triangle/drawings/compilation.log
+-rw-r--r--   0      501       20    31646 2024-03-28 12:43:14.000000 gammaloop-0.1.0/WORKING/sources/amplitudes/massless_triangle/drawings/diagram_0_massless_triangle_0.1
+-rw-r--r--   0      501       20      660 2024-03-28 12:43:14.000000 gammaloop-0.1.0/WORKING/sources/amplitudes/massless_triangle/drawings/diagram_0_massless_triangle_0.log
+-rw-r--r--   0      501       20     2544 2024-03-28 12:43:14.000000 gammaloop-0.1.0/WORKING/sources/amplitudes/massless_triangle/drawings/diagram_0_massless_triangle_0.mp
+-rw-r--r--   0      501       20      526 2024-03-28 12:43:14.000000 gammaloop-0.1.0/WORKING/sources/amplitudes/massless_triangle/drawings/diagram_0_massless_triangle_0.t1
+-rw-r--r--   0      501       20    18135 2024-03-28 12:43:14.000000 gammaloop-0.1.0/WORKING/sources/amplitudes/massless_triangle/drawings/feynman_diagrams.pdf
+-rw-r--r--   0      501       20      924 2024-03-28 12:43:14.000000 gammaloop-0.1.0/WORKING/sources/amplitudes/massless_triangle/drawings/makefile
+-rw-r--r--   0      501       20     8192 2024-03-28 12:43:14.000000 gammaloop-0.1.0/WORKING/sources/model/scalars.yaml
+-rw-r--r--   0      501       20     9019 2024-03-28 12:43:14.000000 gammaloop-0.1.0/WORKING/workspace/integration_state
+-rw-r--r--   0      501       20     2659 2024-03-28 12:43:14.000000 gammaloop-0.1.0/WORKING/workspace/settings.yaml
+-rw-r--r--   0      501       20     4670 2024-04-02 22:34:14.000000 gammaloop-0.1.0/benches/evaluate_net.rs
+-rw-r--r--   0      501       20     4792 2024-03-20 12:28:49.000000 gammaloop-0.1.0/benches/gamma_net.rs
+-rwxr-xr-x   0      501       20       54 2024-04-02 22:34:14.000000 gammaloop-0.1.0/bin/build_dependencies.sh
+-rwxr-xr-x   0      501       20      193 2024-03-21 17:29:46.000000 gammaloop-0.1.0/bin/compile.sh
+-rwxr-xr-x   0      501       20      138 2024-04-02 22:34:14.000000 gammaloop-0.1.0/bin/compile_bin.sh
+-rwxr-xr-x   0      501       20      456 2024-04-02 22:34:14.000000 gammaloop-0.1.0/bin/compile_lib.sh
+-rwxr-xr-x   0      501       20      318 2024-04-02 22:34:14.000000 gammaloop-0.1.0/bin/gammaloop
+-rwxr-xr-x   0      501       20     1446 2024-04-02 22:34:14.000000 gammaloop-0.1.0/bin/run_tests.sh
+-rwxr-xr-x   0      501       20     1082 2024-04-02 22:34:14.000000 gammaloop-0.1.0/bin/test_deployment.sh
+-rw-r--r--   0      501       20      385 2024-04-02 22:34:14.000000 gammaloop-0.1.0/build.rs
+-rw-r--r--   0      501       20        0 2024-04-02 22:34:14.000000 gammaloop-0.1.0/deny.toml
+-rw-r--r--   0      501       20        0 2024-04-02 22:34:14.000000 gammaloop-0.1.0/examples/cards/__init__.py
+-rw-r--r--   0      501       20     1592 2024-03-31 16:28:52.000000 gammaloop-0.1.0/examples/cards/scalar_mercedes/cards/param_card.dat
+-rw-r--r--   0      501       20      308 2024-03-31 16:28:52.000000 gammaloop-0.1.0/examples/cards/scalar_mercedes/cards/proc_card.gL
+-rw-r--r--   0      501       20      933 2024-03-31 16:28:52.000000 gammaloop-0.1.0/examples/cards/scalar_mercedes/cards/run_card.yaml
+-rw-r--r--   0      501       20       71 2024-03-31 16:28:52.000000 gammaloop-0.1.0/examples/cards/scalar_mercedes/output_metadata.yaml
+-rw-r--r--   0      501       20     3018 2024-03-31 16:30:32.000000 gammaloop-0.1.0/examples/cards/scalar_mercedes/pysecdec/ltd_topology_f_0/Makefile
+-rw-r--r--   0      501       20     1734 2024-03-31 16:30:32.000000 gammaloop-0.1.0/examples/cards/scalar_mercedes/pysecdec/ltd_topology_f_0/Makefile.conf
+-rw-r--r--   0      501       20      133 2024-03-31 16:30:32.000000 gammaloop-0.1.0/examples/cards/scalar_mercedes/pysecdec/ltd_topology_f_0/README
+-rw-r--r--   0      501       20        1 2024-03-31 16:30:32.000000 gammaloop-0.1.0/examples/cards/scalar_mercedes/pysecdec/ltd_topology_f_0/disteval/coefficients/ltd_topology_f_0_integral_coefficient0.txt
+-rw-r--r--   0      501       20       43 2024-03-31 16:30:32.000000 gammaloop-0.1.0/examples/cards/scalar_mercedes/pysecdec/ltd_topology_f_0/integral_names.txt
+-rw-r--r--   0      501       20     5194 2024-03-31 16:30:32.000000 gammaloop-0.1.0/examples/cards/scalar_mercedes/pysecdec/ltd_topology_f_0/integrate_ltd_topology_f_0.cpp
+-rw-r--r--   0      501       20        1 2024-03-31 16:30:32.000000 gammaloop-0.1.0/examples/cards/scalar_mercedes/pysecdec/ltd_topology_f_0/ltd_topology_f_0_data/ltd_topology_f_0_integral_coefficient0.txt
+-rw-r--r--   0      501       20     3057 2024-03-31 16:30:32.000000 gammaloop-0.1.0/examples/cards/scalar_mercedes/pysecdec/ltd_topology_f_0/ltd_topology_f_0_integral/Makefile
+-rw-r--r--   0      501       20     2234 2024-03-31 16:30:32.000000 gammaloop-0.1.0/examples/cards/scalar_mercedes/pysecdec/ltd_topology_f_0/ltd_topology_f_0_integral/Makefile.conf
+-rw-r--r--   0      501       20      261 2024-03-31 16:30:32.000000 gammaloop-0.1.0/examples/cards/scalar_mercedes/pysecdec/ltd_topology_f_0/ltd_topology_f_0_integral/README
+-rw-r--r--   0      501       20      117 2024-03-31 16:30:32.000000 gammaloop-0.1.0/examples/cards/scalar_mercedes/pysecdec/ltd_topology_f_0/ltd_topology_f_0_integral/codegen/form.set
+-rw-r--r--   0      501       20      253 2024-03-31 16:30:37.000000 gammaloop-0.1.0/examples/cards/scalar_mercedes/pysecdec/ltd_topology_f_0/ltd_topology_f_0_integral/codegen/sector1.d
+-rw-r--r--   0      501       20     4459 2024-03-31 16:30:37.000000 gammaloop-0.1.0/examples/cards/scalar_mercedes/pysecdec/ltd_topology_f_0/ltd_topology_f_0_integral/codegen/sector1.h
+-rw-r--r--   0      501       20      264 2024-03-31 16:30:37.000000 gammaloop-0.1.0/examples/cards/scalar_mercedes/pysecdec/ltd_topology_f_0/ltd_topology_f_0_integral/codegen/sector10.d
+-rw-r--r--   0      501       20     4477 2024-03-31 16:30:37.000000 gammaloop-0.1.0/examples/cards/scalar_mercedes/pysecdec/ltd_topology_f_0/ltd_topology_f_0_integral/codegen/sector10.h
+-rw-r--r--   0      501       20      264 2024-03-31 16:30:37.000000 gammaloop-0.1.0/examples/cards/scalar_mercedes/pysecdec/ltd_topology_f_0/ltd_topology_f_0_integral/codegen/sector13.d
+-rw-r--r--   0      501       20     4570 2024-03-31 16:30:37.000000 gammaloop-0.1.0/examples/cards/scalar_mercedes/pysecdec/ltd_topology_f_0/ltd_topology_f_0_integral/codegen/sector13.h
+-rw-r--r--   0      501       20      264 2024-03-31 16:30:37.000000 gammaloop-0.1.0/examples/cards/scalar_mercedes/pysecdec/ltd_topology_f_0/ltd_topology_f_0_integral/codegen/sector14.d
+-rw-r--r--   0      501       20     4570 2024-03-31 16:30:37.000000 gammaloop-0.1.0/examples/cards/scalar_mercedes/pysecdec/ltd_topology_f_0/ltd_topology_f_0_integral/codegen/sector14.h
+-rw-r--r--   0      501       20      264 2024-03-31 16:30:37.000000 gammaloop-0.1.0/examples/cards/scalar_mercedes/pysecdec/ltd_topology_f_0/ltd_topology_f_0_integral/codegen/sector17.d
+-rw-r--r--   0      501       20     4579 2024-03-31 16:30:37.000000 gammaloop-0.1.0/examples/cards/scalar_mercedes/pysecdec/ltd_topology_f_0/ltd_topology_f_0_integral/codegen/sector17.h
+-rw-r--r--   0      501       20      264 2024-03-31 16:30:37.000000 gammaloop-0.1.0/examples/cards/scalar_mercedes/pysecdec/ltd_topology_f_0/ltd_topology_f_0_integral/codegen/sector18.d
+-rw-r--r--   0      501       20     4452 2024-03-31 16:30:37.000000 gammaloop-0.1.0/examples/cards/scalar_mercedes/pysecdec/ltd_topology_f_0/ltd_topology_f_0_integral/codegen/sector18.h
+-rw-r--r--   0      501       20      253 2024-03-31 16:30:37.000000 gammaloop-0.1.0/examples/cards/scalar_mercedes/pysecdec/ltd_topology_f_0/ltd_topology_f_0_integral/codegen/sector2.d
+-rw-r--r--   0      501       20     4468 2024-03-31 16:30:37.000000 gammaloop-0.1.0/examples/cards/scalar_mercedes/pysecdec/ltd_topology_f_0/ltd_topology_f_0_integral/codegen/sector2.h
+-rw-r--r--   0      501       20      264 2024-03-31 16:30:37.000000 gammaloop-0.1.0/examples/cards/scalar_mercedes/pysecdec/ltd_topology_f_0/ltd_topology_f_0_integral/codegen/sector21.d
+-rw-r--r--   0      501       20     4461 2024-03-31 16:30:37.000000 gammaloop-0.1.0/examples/cards/scalar_mercedes/pysecdec/ltd_topology_f_0/ltd_topology_f_0_integral/codegen/sector21.h
+-rw-r--r--   0      501       20      264 2024-03-31 16:30:37.000000 gammaloop-0.1.0/examples/cards/scalar_mercedes/pysecdec/ltd_topology_f_0/ltd_topology_f_0_integral/codegen/sector22.d
+-rw-r--r--   0      501       20     4470 2024-03-31 16:30:37.000000 gammaloop-0.1.0/examples/cards/scalar_mercedes/pysecdec/ltd_topology_f_0/ltd_topology_f_0_integral/codegen/sector22.h
+-rw-r--r--   0      501       20      264 2024-03-31 16:30:37.000000 gammaloop-0.1.0/examples/cards/scalar_mercedes/pysecdec/ltd_topology_f_0/ltd_topology_f_0_integral/codegen/sector25.d
+-rw-r--r--   0      501       20     4524 2024-03-31 16:30:37.000000 gammaloop-0.1.0/examples/cards/scalar_mercedes/pysecdec/ltd_topology_f_0/ltd_topology_f_0_integral/codegen/sector25.h
+-rw-r--r--   0      501       20      264 2024-03-31 16:30:37.000000 gammaloop-0.1.0/examples/cards/scalar_mercedes/pysecdec/ltd_topology_f_0/ltd_topology_f_0_integral/codegen/sector26.d
+-rw-r--r--   0      501       20     4484 2024-03-31 16:30:37.000000 gammaloop-0.1.0/examples/cards/scalar_mercedes/pysecdec/ltd_topology_f_0/ltd_topology_f_0_integral/codegen/sector26.h
+-rw-r--r--   0      501       20      264 2024-03-31 16:30:37.000000 gammaloop-0.1.0/examples/cards/scalar_mercedes/pysecdec/ltd_topology_f_0/ltd_topology_f_0_integral/codegen/sector29.d
+-rw-r--r--   0      501       20     4484 2024-03-31 16:30:37.000000 gammaloop-0.1.0/examples/cards/scalar_mercedes/pysecdec/ltd_topology_f_0/ltd_topology_f_0_integral/codegen/sector29.h
+-rw-r--r--   0      501       20      264 2024-03-31 16:30:37.000000 gammaloop-0.1.0/examples/cards/scalar_mercedes/pysecdec/ltd_topology_f_0/ltd_topology_f_0_integral/codegen/sector30.d
+-rw-r--r--   0      501       20     4452 2024-03-31 16:30:37.000000 gammaloop-0.1.0/examples/cards/scalar_mercedes/pysecdec/ltd_topology_f_0/ltd_topology_f_0_integral/codegen/sector30.h
+-rw-r--r--   0      501       20      264 2024-03-31 16:30:37.000000 gammaloop-0.1.0/examples/cards/scalar_mercedes/pysecdec/ltd_topology_f_0/ltd_topology_f_0_integral/codegen/sector33.d
+-rw-r--r--   0      501       20     4470 2024-03-31 16:30:37.000000 gammaloop-0.1.0/examples/cards/scalar_mercedes/pysecdec/ltd_topology_f_0/ltd_topology_f_0_integral/codegen/sector33.h
+-rw-r--r--   0      501       20       58 2024-03-31 16:30:37.000000 gammaloop-0.1.0/examples/cards/scalar_mercedes/pysecdec/ltd_topology_f_0/ltd_topology_f_0_integral/codegen/sector34.d
+-rw-r--r--   0      501       20     4501 2024-03-31 16:30:37.000000 gammaloop-0.1.0/examples/cards/scalar_mercedes/pysecdec/ltd_topology_f_0/ltd_topology_f_0_integral/codegen/sector34.h
+-rw-r--r--   0      501       20      264 2024-03-31 16:30:37.000000 gammaloop-0.1.0/examples/cards/scalar_mercedes/pysecdec/ltd_topology_f_0/ltd_topology_f_0_integral/codegen/sector37.d
+-rw-r--r--   0      501       20     4525 2024-03-31 16:30:37.000000 gammaloop-0.1.0/examples/cards/scalar_mercedes/pysecdec/ltd_topology_f_0/ltd_topology_f_0_integral/codegen/sector37.h
+-rw-r--r--   0      501       20      264 2024-03-31 16:30:37.000000 gammaloop-0.1.0/examples/cards/scalar_mercedes/pysecdec/ltd_topology_f_0/ltd_topology_f_0_integral/codegen/sector41.d
+-rw-r--r--   0      501       20     4516 2024-03-31 16:30:37.000000 gammaloop-0.1.0/examples/cards/scalar_mercedes/pysecdec/ltd_topology_f_0/ltd_topology_f_0_integral/codegen/sector41.h
+-rw-r--r--   0      501       20      264 2024-03-31 16:30:37.000000 gammaloop-0.1.0/examples/cards/scalar_mercedes/pysecdec/ltd_topology_f_0/ltd_topology_f_0_integral/codegen/sector45.d
+-rw-r--r--   0      501       20     4461 2024-03-31 16:30:37.000000 gammaloop-0.1.0/examples/cards/scalar_mercedes/pysecdec/ltd_topology_f_0/ltd_topology_f_0_integral/codegen/sector45.h
+-rw-r--r--   0      501       20      264 2024-03-31 16:30:37.000000 gammaloop-0.1.0/examples/cards/scalar_mercedes/pysecdec/ltd_topology_f_0/ltd_topology_f_0_integral/codegen/sector49.d
+-rw-r--r--   0      501       20     4516 2024-03-31 16:30:37.000000 gammaloop-0.1.0/examples/cards/scalar_mercedes/pysecdec/ltd_topology_f_0/ltd_topology_f_0_integral/codegen/sector49.h
+-rw-r--r--   0      501       20      253 2024-03-31 16:30:37.000000 gammaloop-0.1.0/examples/cards/scalar_mercedes/pysecdec/ltd_topology_f_0/ltd_topology_f_0_integral/codegen/sector5.d
+-rw-r--r--   0      501       20     4459 2024-03-31 16:30:37.000000 gammaloop-0.1.0/examples/cards/scalar_mercedes/pysecdec/ltd_topology_f_0/ltd_topology_f_0_integral/codegen/sector5.h
+-rw-r--r--   0      501       20      264 2024-03-31 16:30:37.000000 gammaloop-0.1.0/examples/cards/scalar_mercedes/pysecdec/ltd_topology_f_0/ltd_topology_f_0_integral/codegen/sector50.d
+-rw-r--r--   0      501       20     4461 2024-03-31 16:30:37.000000 gammaloop-0.1.0/examples/cards/scalar_mercedes/pysecdec/ltd_topology_f_0/ltd_topology_f_0_integral/codegen/sector50.h
+-rw-r--r--   0      501       20      264 2024-03-31 16:30:37.000000 gammaloop-0.1.0/examples/cards/scalar_mercedes/pysecdec/ltd_topology_f_0/ltd_topology_f_0_integral/codegen/sector53.d
+-rw-r--r--   0      501       20     4470 2024-03-31 16:30:37.000000 gammaloop-0.1.0/examples/cards/scalar_mercedes/pysecdec/ltd_topology_f_0/ltd_topology_f_0_integral/codegen/sector53.h
+-rw-r--r--   0      501       20      264 2024-03-31 16:30:37.000000 gammaloop-0.1.0/examples/cards/scalar_mercedes/pysecdec/ltd_topology_f_0/ltd_topology_f_0_integral/codegen/sector54.d
+-rw-r--r--   0      501       20     4516 2024-03-31 16:30:37.000000 gammaloop-0.1.0/examples/cards/scalar_mercedes/pysecdec/ltd_topology_f_0/ltd_topology_f_0_integral/codegen/sector54.h
+-rw-r--r--   0      501       20      264 2024-03-31 16:30:37.000000 gammaloop-0.1.0/examples/cards/scalar_mercedes/pysecdec/ltd_topology_f_0/ltd_topology_f_0_integral/codegen/sector57.d
+-rw-r--r--   0      501       20     4507 2024-03-31 16:30:37.000000 gammaloop-0.1.0/examples/cards/scalar_mercedes/pysecdec/ltd_topology_f_0/ltd_topology_f_0_integral/codegen/sector57.h
+-rw-r--r--   0      501       20      253 2024-03-31 16:30:37.000000 gammaloop-0.1.0/examples/cards/scalar_mercedes/pysecdec/ltd_topology_f_0/ltd_topology_f_0_integral/codegen/sector6.d
+-rw-r--r--   0      501       20     4468 2024-03-31 16:30:37.000000 gammaloop-0.1.0/examples/cards/scalar_mercedes/pysecdec/ltd_topology_f_0/ltd_topology_f_0_integral/codegen/sector6.h
+-rw-r--r--   0      501       20      264 2024-03-31 16:30:37.000000 gammaloop-0.1.0/examples/cards/scalar_mercedes/pysecdec/ltd_topology_f_0/ltd_topology_f_0_integral/codegen/sector61.d
+-rw-r--r--   0      501       20     4516 2024-03-31 16:30:37.000000 gammaloop-0.1.0/examples/cards/scalar_mercedes/pysecdec/ltd_topology_f_0/ltd_topology_f_0_integral/codegen/sector61.h
+-rw-r--r--   0      501       20      253 2024-03-31 16:30:37.000000 gammaloop-0.1.0/examples/cards/scalar_mercedes/pysecdec/ltd_topology_f_0/ltd_topology_f_0_integral/codegen/sector9.d
+-rw-r--r--   0      501       20     4468 2024-03-31 16:30:37.000000 gammaloop-0.1.0/examples/cards/scalar_mercedes/pysecdec/ltd_topology_f_0/ltd_topology_f_0_integral/codegen/sector9.h
+-rw-r--r--   0      501       20     6477 2024-03-31 16:30:32.000000 gammaloop-0.1.0/examples/cards/scalar_mercedes/pysecdec/ltd_topology_f_0/ltd_topology_f_0_integral/cuda_integrate_ltd_topology_f_0_integral.cpp
+-rw-r--r--   0      501       20     7187 2024-03-31 16:30:32.000000 gammaloop-0.1.0/examples/cards/scalar_mercedes/pysecdec/ltd_topology_f_0/ltd_topology_f_0_integral/distsrc/builtin.cpp
+-rw-r--r--   0      501       20     9392 2024-03-31 16:30:32.000000 gammaloop-0.1.0/examples/cards/scalar_mercedes/pysecdec/ltd_topology_f_0/ltd_topology_f_0_integral/distsrc/builtin.cu
+-rw-r--r--   0      501       20    19363 2024-03-31 16:30:32.000000 gammaloop-0.1.0/examples/cards/scalar_mercedes/pysecdec/ltd_topology_f_0/ltd_topology_f_0_integral/distsrc/common_cpu.h
+-rw-r--r--   0      501       20     3573 2024-03-31 16:30:32.000000 gammaloop-0.1.0/examples/cards/scalar_mercedes/pysecdec/ltd_topology_f_0/ltd_topology_f_0_integral/distsrc/common_cuda.h
+-rw-r--r--   0      501       20     6084 2024-03-31 16:30:32.000000 gammaloop-0.1.0/examples/cards/scalar_mercedes/pysecdec/ltd_topology_f_0/ltd_topology_f_0_integral/integrate_ltd_topology_f_0_integral.cpp
+-rw-r--r--   0      501       20    10677 2024-03-31 16:30:32.000000 gammaloop-0.1.0/examples/cards/scalar_mercedes/pysecdec/ltd_topology_f_0/ltd_topology_f_0_integral/src/SecDecInternalFunctions.hpp
+-rw-r--r--   0      501       20    41255 2024-03-31 16:30:32.000000 gammaloop-0.1.0/examples/cards/scalar_mercedes/pysecdec/ltd_topology_f_0/pylink/pylink.cpp
+-rw-r--r--   0      501       20    15741 2024-03-31 16:30:32.000000 gammaloop-0.1.0/examples/cards/scalar_mercedes/pysecdec/ltd_topology_f_0/pylink/qmc_template_instantiations_0.cpp
+-rw-r--r--   0      501       20    51608 2024-03-31 16:30:32.000000 gammaloop-0.1.0/examples/cards/scalar_mercedes/pysecdec/ltd_topology_f_0/src/amplitude.cpp
+-rw-r--r--   0      501       20    42991 2024-03-31 16:30:32.000000 gammaloop-0.1.0/examples/cards/scalar_mercedes/pysecdec/ltd_topology_f_0/src/ltd_topology_f_0_integral_weighted_integral.cpp
+-rw-r--r--   0      501       20     1300 2024-03-31 16:30:32.000000 gammaloop-0.1.0/examples/cards/scalar_mercedes/pysecdec/ltd_topology_f_0/src/ltd_topology_f_0_integral_weighted_integral.hpp
+-rw-r--r--   0      501       20        1 2024-03-31 16:29:02.000000 gammaloop-0.1.0/examples/cards/scalar_mercedes/pysecdec/numerator_ltd_topology_f_0.txt
+-rw-r--r--   0      501       20    15024 2024-03-31 16:29:02.000000 gammaloop-0.1.0/examples/cards/scalar_mercedes/pysecdec/run_ltd_topology_f_0.py
+-rw-r--r--   0      501       20      135 2024-03-31 16:28:59.000000 gammaloop-0.1.0/examples/cards/scalar_mercedes/runs/run.yaml
+-rw-r--r--   0      501       20     3332 2024-03-31 16:28:52.000000 gammaloop-0.1.0/examples/cards/scalar_mercedes/sources/amplitudes/ltd_topology_f/amplitude.yaml
+-rw-r--r--   0      501       20   153769 2024-03-31 16:28:52.000000 gammaloop-0.1.0/examples/cards/scalar_mercedes/sources/amplitudes/ltd_topology_f/derived_data_ltd_topology_f_0.bin
+-rw-r--r--   0      501       20     7787 2024-03-31 16:28:52.000000 gammaloop-0.1.0/examples/cards/scalar_mercedes/sources/amplitudes/ltd_topology_f/drawings/0_ltd_topology_f_0.tex
+-rwxr-xr-x   0      501       20     2885 2024-03-31 16:28:52.000000 gammaloop-0.1.0/examples/cards/scalar_mercedes/sources/amplitudes/ltd_topology_f/drawings/combine_pages.py
+-rw-r--r--   0      501       20      921 2024-03-31 16:28:52.000000 gammaloop-0.1.0/examples/cards/scalar_mercedes/sources/amplitudes/ltd_topology_f/drawings/makefile
+-rw-r--r--   0      501       20     8192 2024-03-31 16:28:52.000000 gammaloop-0.1.0/examples/cards/scalar_mercedes/sources/model/scalars.yaml
+-rw-r--r--   0      501       20    64931 2024-03-31 16:28:58.000000 gammaloop-0.1.0/examples/cards/scalar_mercedes/workspace/integration_state
+-rw-r--r--   0      501       20     2642 2024-03-31 16:28:58.000000 gammaloop-0.1.0/examples/cards/scalar_mercedes/workspace/settings.yaml
+-rw-r--r--   0      501       20     1035 2024-04-02 22:34:14.000000 gammaloop-0.1.0/examples/cards/scalar_mercedes.gL
+-rw-r--r--   0      501       20     5672 2024-03-22 17:20:59.000000 gammaloop-0.1.0/examples/jupyter/.ipynb_checkpoints/steer_gammaloop-checkpoint.ipynb
+-rw-r--r--   0      501       20        0 2024-04-02 22:34:14.000000 gammaloop-0.1.0/examples/jupyter/__init__.py
+-rw-r--r--   0      501       20     5672 2024-04-02 22:34:14.000000 gammaloop-0.1.0/examples/jupyter/steer_gammaloop.ipynb
+-rw-r--r--   0      501       20     4943 2024-04-02 22:34:14.000000 gammaloop-0.1.0/examples/rust/tensors/evaluate_network.rs
+-rw-r--r--   0      501       20    24059 2024-04-02 22:34:14.000000 gammaloop-0.1.0/examples/rust/tensors/gamma_chain.rs
+-rw-r--r--   0      501       20     2754 2024-04-02 22:34:14.000000 gammaloop-0.1.0/examples/rust/tensors/gamma_network.rs
+-rw-r--r--   0      501       20     2330 2024-04-02 22:34:14.000000 gammaloop-0.1.0/examples/rust/tensors/load_nested_tensornet.rs
+-rw-r--r--   0      501       20     1377 2024-04-02 22:34:14.000000 gammaloop-0.1.0/examples/rust/tensors/symbolica_nested_eval.rs
+-rw-r--r--   0      501       20     3036 2024-04-02 22:34:14.000000 gammaloop-0.1.0/flake.lock
+-rw-r--r--   0      501       20     4613 2024-04-02 22:34:14.000000 gammaloop-0.1.0/flake.nix
+-rw-r--r--   0      501       20     1940 2024-01-09 10:38:51.000000 gammaloop-0.1.0/mod_Cargo.toml
+-rw-r--r--   0      501       20    10100 2024-04-02 22:34:14.000000 gammaloop-0.1.0/python/gammaloop/__init__.py
+-rw-r--r--   0      501       20     4578 2024-04-02 22:34:14.000000 gammaloop-0.1.0/python/gammaloop/_gammaloop.pyi
+-rw-r--r--   0      501       20        0 2023-09-01 11:42:35.000000 gammaloop-0.1.0/python/gammaloop/base_objects/__init__.py
+-rw-r--r--   0      501       20    48814 2024-04-02 22:34:14.000000 gammaloop-0.1.0/python/gammaloop/base_objects/graph.py
+-rw-r--r--   0      501       20    49900 2024-04-02 22:34:14.000000 gammaloop-0.1.0/python/gammaloop/base_objects/model.py
+-rw-r--r--   0      501       20    30892 2023-10-24 19:20:56.000000 gammaloop-0.1.0/python/gammaloop/base_objects/param_card.py
+-rw-r--r--   0      501       20        0 2023-09-11 14:36:09.000000 gammaloop-0.1.0/python/gammaloop/bin/__init__.py
+-rwxr-xr-x   0      501       20     3870 2024-04-02 22:34:14.000000 gammaloop-0.1.0/python/gammaloop/bin/build_dependencies.sh
+-rwxr-xr-x   0      501       20      318 2024-04-02 22:34:14.000000 gammaloop-0.1.0/python/gammaloop/bin/gammaloop
+-rw-r--r--   0      501       20        0 2023-09-05 12:02:31.000000 gammaloop-0.1.0/python/gammaloop/cross_section/__init__.py
+-rw-r--r--   0      501       20     5295 2023-10-11 18:27:55.000000 gammaloop-0.1.0/python/gammaloop/cross_section/cross_section.py
+-rw-r--r--   0      501       20     7880 2024-04-02 22:34:14.000000 gammaloop-0.1.0/python/gammaloop/cross_section/supergraph.py
+-rw-r--r--   0      501       20      840 2024-04-02 22:34:14.000000 gammaloop-0.1.0/python/gammaloop/data/config/gammaloop_config.yaml
+-rw-r--r--   0      501       20      652 2023-10-17 13:06:17.000000 gammaloop-0.1.0/python/gammaloop/data/models/scalars/__init__.py
+-rw-r--r--   0      501       20      416 2023-10-11 20:54:39.000000 gammaloop-0.1.0/python/gammaloop/data/models/scalars/coupling_orders.py
+-rw-r--r--   0      501       20      257 2023-10-11 20:54:38.000000 gammaloop-0.1.0/python/gammaloop/data/models/scalars/couplings.py
+-rw-r--r--   0      501       20     1332 2023-10-11 20:54:34.000000 gammaloop-0.1.0/python/gammaloop/data/models/scalars/function_library.py
+-rw-r--r--   0      501       20      726 2023-10-11 20:54:32.000000 gammaloop-0.1.0/python/gammaloop/data/models/scalars/lorentz.py
+-rw-r--r--   0      501       20     7079 2023-10-11 20:54:25.000000 gammaloop-0.1.0/python/gammaloop/data/models/scalars/object_library.py
+-rw-r--r--   0      501       20     3511 2024-03-20 12:28:49.000000 gammaloop-0.1.0/python/gammaloop/data/models/scalars/parameters.py
+-rw-r--r--   0      501       20     1221 2023-10-17 12:03:34.000000 gammaloop-0.1.0/python/gammaloop/data/models/scalars/particles.py
+-rw-r--r--   0      501       20     7602 2024-03-31 17:27:41.000000 gammaloop-0.1.0/python/gammaloop/data/models/scalars/py3_model.pkl
+-rw-r--r--   0      501       20     1761 2023-09-05 09:24:12.000000 gammaloop-0.1.0/python/gammaloop/data/models/scalars/restrict_default.dat
+-rw-r--r--   0      501       20     1592 2023-10-24 23:36:16.000000 gammaloop-0.1.0/python/gammaloop/data/models/scalars/restrict_full.dat
+-rwxr-xr-x   0      501       20      543 2023-10-11 20:55:57.000000 gammaloop-0.1.0/python/gammaloop/data/models/scalars/run_write_param_card.py
+-rw-r--r--   0      501       20     1103 2023-10-11 20:56:44.000000 gammaloop-0.1.0/python/gammaloop/data/models/scalars/vertices.py
+-rw-r--r--   0      501       20     6558 2023-10-11 19:56:33.000000 gammaloop-0.1.0/python/gammaloop/data/models/scalars/write_param_card.py
+-rw-r--r--   0      501       20      886 2023-10-11 19:56:38.000000 gammaloop-0.1.0/python/gammaloop/data/models/sm/__init__.py
+-rw-r--r--   0      501       20     2887 2023-10-11 19:56:43.000000 gammaloop-0.1.0/python/gammaloop/data/models/sm/build_restrict.py
+-rw-r--r--   0      501       20      485 2023-10-11 19:56:47.000000 gammaloop-0.1.0/python/gammaloop/data/models/sm/coupling_orders.py
+-rw-r--r--   0      501       20    14158 2023-09-01 11:54:08.000000 gammaloop-0.1.0/python/gammaloop/data/models/sm/couplings.py
+-rw-r--r--   0      501       20    13626 2023-09-01 11:54:08.000000 gammaloop-0.1.0/python/gammaloop/data/models/sm/decays.py
+-rw-r--r--   0      501       20     1340 2023-09-01 11:54:08.000000 gammaloop-0.1.0/python/gammaloop/data/models/sm/function_library.py
+-rw-r--r--   0      501       20     3202 2023-10-11 20:56:31.000000 gammaloop-0.1.0/python/gammaloop/data/models/sm/lorentz.py
+-rw-r--r--   0      501       20     7078 2023-09-01 11:54:08.000000 gammaloop-0.1.0/python/gammaloop/data/models/sm/object_library.py
+-rw-r--r--   0      501       20    14852 2023-10-24 16:08:31.000000 gammaloop-0.1.0/python/gammaloop/data/models/sm/parameters.py
+-rw-r--r--   0      501       20    10248 2023-10-07 17:17:26.000000 gammaloop-0.1.0/python/gammaloop/data/models/sm/particles.py
+-rw-r--r--   0      501       20     1437 2023-09-01 11:54:08.000000 gammaloop-0.1.0/python/gammaloop/data/models/sm/restrict_c_mass.dat
+-rw-r--r--   0      501       20     1438 2023-09-01 11:54:08.000000 gammaloop-0.1.0/python/gammaloop/data/models/sm/restrict_ckm.dat
+-rw-r--r--   0      501       20     1462 2023-10-24 16:08:31.000000 gammaloop-0.1.0/python/gammaloop/data/models/sm/restrict_default.dat
+-rw-r--r--   0      501       20     4734 2023-10-24 22:52:08.000000 gammaloop-0.1.0/python/gammaloop/data/models/sm/restrict_full.dat
+-rw-r--r--   0      501       20     1460 2023-10-24 17:09:06.000000 gammaloop-0.1.0/python/gammaloop/data/models/sm/restrict_lepton_masses.dat
+-rw-r--r--   0      501       20     1438 2023-09-01 11:54:08.000000 gammaloop-0.1.0/python/gammaloop/data/models/sm/restrict_no_b_mass.dat
+-rw-r--r--   0      501       20     1438 2023-09-01 11:54:08.000000 gammaloop-0.1.0/python/gammaloop/data/models/sm/restrict_no_masses.dat
+-rw-r--r--   0      501       20     1437 2023-09-01 11:54:08.000000 gammaloop-0.1.0/python/gammaloop/data/models/sm/restrict_no_tau_mass.dat
+-rw-r--r--   0      501       20     1438 2023-09-01 11:54:08.000000 gammaloop-0.1.0/python/gammaloop/data/models/sm/restrict_no_widths.dat
+-rw-r--r--   0      501       20     1438 2023-09-01 11:54:08.000000 gammaloop-0.1.0/python/gammaloop/data/models/sm/restrict_zeromass_ckm.dat
+-rwxr-xr-x   0      501       20      543 2023-10-11 20:55:43.000000 gammaloop-0.1.0/python/gammaloop/data/models/sm/run_write_param_card.py
+-rw-r--r--   0      501       20    32557 2023-09-01 11:54:08.000000 gammaloop-0.1.0/python/gammaloop/data/models/sm/vertices.py
+-rw-r--r--   0      501       20     6963 2023-09-01 11:54:08.000000 gammaloop-0.1.0/python/gammaloop/data/models/sm/write_param_card.py
+-rw-r--r--   0      501       20     1906 2024-04-02 22:34:14.000000 gammaloop-0.1.0/python/gammaloop/data/run_cards/cmd.gL
+-rw-r--r--   0      501       20      897 2024-04-02 22:34:14.000000 gammaloop-0.1.0/python/gammaloop/data/run_cards/rust_run_config.yaml
+-rw-r--r--   0      501       20       35 2023-09-12 06:40:58.000000 gammaloop-0.1.0/python/gammaloop/data/symbolica_license.txt
+-rwxr-xr-x   0      501       20     2885 2023-10-11 18:45:31.000000 gammaloop-0.1.0/python/gammaloop/data/templates/drawing/combine_pages.py
+-rw-r--r--   0      501       20     2088 2023-10-11 19:57:02.000000 gammaloop-0.1.0/python/gammaloop/data/templates/drawing/drawing.tex.template
+-rw-r--r--   0      501       20      927 2024-04-02 22:34:14.000000 gammaloop-0.1.0/python/gammaloop/data/templates/drawing/makefile
+-rw-r--r--   0      501       20      252 2024-04-02 22:34:14.000000 gammaloop-0.1.0/python/gammaloop/dependencies/fjcore/Makefile
+-rw-r--r--   0      501       20   234477 2024-04-02 22:34:14.000000 gammaloop-0.1.0/python/gammaloop/dependencies/fjcore/fjcore.cc
+-rw-r--r--   0      501       20    71944 2024-04-02 22:34:14.000000 gammaloop-0.1.0/python/gammaloop/dependencies/fjcore/fjcore.hh
+-rw-r--r--   0      501       20     9295 2024-04-02 22:34:14.000000 gammaloop-0.1.0/python/gammaloop/dependencies/fjcore/wrapper.cc
+-rw-r--r--   0      501       20        0 2024-04-02 22:34:14.000000 gammaloop-0.1.0/python/gammaloop/examples/__init__.py
+-rw-r--r--   0      501       20        0 2024-04-02 22:34:14.000000 gammaloop-0.1.0/python/gammaloop/examples/cards/__init__.py
+-rw-r--r--   0      501       20     1592 2024-03-31 16:28:52.000000 gammaloop-0.1.0/python/gammaloop/examples/cards/scalar_mercedes/cards/param_card.dat
+-rw-r--r--   0      501       20      308 2024-03-31 16:28:52.000000 gammaloop-0.1.0/python/gammaloop/examples/cards/scalar_mercedes/cards/proc_card.gL
+-rw-r--r--   0      501       20      933 2024-03-31 16:28:52.000000 gammaloop-0.1.0/python/gammaloop/examples/cards/scalar_mercedes/cards/run_card.yaml
+-rw-r--r--   0      501       20       71 2024-03-31 16:28:52.000000 gammaloop-0.1.0/python/gammaloop/examples/cards/scalar_mercedes/output_metadata.yaml
+-rw-r--r--   0      501       20     3018 2024-03-31 16:30:32.000000 gammaloop-0.1.0/python/gammaloop/examples/cards/scalar_mercedes/pysecdec/ltd_topology_f_0/Makefile
+-rw-r--r--   0      501       20     1734 2024-03-31 16:30:32.000000 gammaloop-0.1.0/python/gammaloop/examples/cards/scalar_mercedes/pysecdec/ltd_topology_f_0/Makefile.conf
+-rw-r--r--   0      501       20      133 2024-03-31 16:30:32.000000 gammaloop-0.1.0/python/gammaloop/examples/cards/scalar_mercedes/pysecdec/ltd_topology_f_0/README
+-rw-r--r--   0      501       20        1 2024-03-31 16:30:32.000000 gammaloop-0.1.0/python/gammaloop/examples/cards/scalar_mercedes/pysecdec/ltd_topology_f_0/disteval/coefficients/ltd_topology_f_0_integral_coefficient0.txt
+-rw-r--r--   0      501       20       43 2024-03-31 16:30:32.000000 gammaloop-0.1.0/python/gammaloop/examples/cards/scalar_mercedes/pysecdec/ltd_topology_f_0/integral_names.txt
+-rw-r--r--   0      501       20     5194 2024-03-31 16:30:32.000000 gammaloop-0.1.0/python/gammaloop/examples/cards/scalar_mercedes/pysecdec/ltd_topology_f_0/integrate_ltd_topology_f_0.cpp
+-rw-r--r--   0      501       20        1 2024-03-31 16:30:32.000000 gammaloop-0.1.0/python/gammaloop/examples/cards/scalar_mercedes/pysecdec/ltd_topology_f_0/ltd_topology_f_0_data/ltd_topology_f_0_integral_coefficient0.txt
+-rw-r--r--   0      501       20     3057 2024-03-31 16:30:32.000000 gammaloop-0.1.0/python/gammaloop/examples/cards/scalar_mercedes/pysecdec/ltd_topology_f_0/ltd_topology_f_0_integral/Makefile
+-rw-r--r--   0      501       20     2234 2024-03-31 16:30:32.000000 gammaloop-0.1.0/python/gammaloop/examples/cards/scalar_mercedes/pysecdec/ltd_topology_f_0/ltd_topology_f_0_integral/Makefile.conf
+-rw-r--r--   0      501       20      261 2024-03-31 16:30:32.000000 gammaloop-0.1.0/python/gammaloop/examples/cards/scalar_mercedes/pysecdec/ltd_topology_f_0/ltd_topology_f_0_integral/README
+-rw-r--r--   0      501       20      117 2024-03-31 16:30:32.000000 gammaloop-0.1.0/python/gammaloop/examples/cards/scalar_mercedes/pysecdec/ltd_topology_f_0/ltd_topology_f_0_integral/codegen/form.set
+-rw-r--r--   0      501       20      253 2024-03-31 16:30:37.000000 gammaloop-0.1.0/python/gammaloop/examples/cards/scalar_mercedes/pysecdec/ltd_topology_f_0/ltd_topology_f_0_integral/codegen/sector1.d
+-rw-r--r--   0      501       20     4459 2024-03-31 16:30:37.000000 gammaloop-0.1.0/python/gammaloop/examples/cards/scalar_mercedes/pysecdec/ltd_topology_f_0/ltd_topology_f_0_integral/codegen/sector1.h
+-rw-r--r--   0      501       20      264 2024-03-31 16:30:37.000000 gammaloop-0.1.0/python/gammaloop/examples/cards/scalar_mercedes/pysecdec/ltd_topology_f_0/ltd_topology_f_0_integral/codegen/sector10.d
+-rw-r--r--   0      501       20     4477 2024-03-31 16:30:37.000000 gammaloop-0.1.0/python/gammaloop/examples/cards/scalar_mercedes/pysecdec/ltd_topology_f_0/ltd_topology_f_0_integral/codegen/sector10.h
+-rw-r--r--   0      501       20      264 2024-03-31 16:30:37.000000 gammaloop-0.1.0/python/gammaloop/examples/cards/scalar_mercedes/pysecdec/ltd_topology_f_0/ltd_topology_f_0_integral/codegen/sector13.d
+-rw-r--r--   0      501       20     4570 2024-03-31 16:30:37.000000 gammaloop-0.1.0/python/gammaloop/examples/cards/scalar_mercedes/pysecdec/ltd_topology_f_0/ltd_topology_f_0_integral/codegen/sector13.h
+-rw-r--r--   0      501       20      264 2024-03-31 16:30:37.000000 gammaloop-0.1.0/python/gammaloop/examples/cards/scalar_mercedes/pysecdec/ltd_topology_f_0/ltd_topology_f_0_integral/codegen/sector14.d
+-rw-r--r--   0      501       20     4570 2024-03-31 16:30:37.000000 gammaloop-0.1.0/python/gammaloop/examples/cards/scalar_mercedes/pysecdec/ltd_topology_f_0/ltd_topology_f_0_integral/codegen/sector14.h
+-rw-r--r--   0      501       20      264 2024-03-31 16:30:37.000000 gammaloop-0.1.0/python/gammaloop/examples/cards/scalar_mercedes/pysecdec/ltd_topology_f_0/ltd_topology_f_0_integral/codegen/sector17.d
+-rw-r--r--   0      501       20     4579 2024-03-31 16:30:37.000000 gammaloop-0.1.0/python/gammaloop/examples/cards/scalar_mercedes/pysecdec/ltd_topology_f_0/ltd_topology_f_0_integral/codegen/sector17.h
+-rw-r--r--   0      501       20      264 2024-03-31 16:30:37.000000 gammaloop-0.1.0/python/gammaloop/examples/cards/scalar_mercedes/pysecdec/ltd_topology_f_0/ltd_topology_f_0_integral/codegen/sector18.d
+-rw-r--r--   0      501       20     4452 2024-03-31 16:30:37.000000 gammaloop-0.1.0/python/gammaloop/examples/cards/scalar_mercedes/pysecdec/ltd_topology_f_0/ltd_topology_f_0_integral/codegen/sector18.h
+-rw-r--r--   0      501       20      253 2024-03-31 16:30:37.000000 gammaloop-0.1.0/python/gammaloop/examples/cards/scalar_mercedes/pysecdec/ltd_topology_f_0/ltd_topology_f_0_integral/codegen/sector2.d
+-rw-r--r--   0      501       20     4468 2024-03-31 16:30:37.000000 gammaloop-0.1.0/python/gammaloop/examples/cards/scalar_mercedes/pysecdec/ltd_topology_f_0/ltd_topology_f_0_integral/codegen/sector2.h
+-rw-r--r--   0      501       20      264 2024-03-31 16:30:37.000000 gammaloop-0.1.0/python/gammaloop/examples/cards/scalar_mercedes/pysecdec/ltd_topology_f_0/ltd_topology_f_0_integral/codegen/sector21.d
+-rw-r--r--   0      501       20     4461 2024-03-31 16:30:37.000000 gammaloop-0.1.0/python/gammaloop/examples/cards/scalar_mercedes/pysecdec/ltd_topology_f_0/ltd_topology_f_0_integral/codegen/sector21.h
+-rw-r--r--   0      501       20      264 2024-03-31 16:30:37.000000 gammaloop-0.1.0/python/gammaloop/examples/cards/scalar_mercedes/pysecdec/ltd_topology_f_0/ltd_topology_f_0_integral/codegen/sector22.d
+-rw-r--r--   0      501       20     4470 2024-03-31 16:30:37.000000 gammaloop-0.1.0/python/gammaloop/examples/cards/scalar_mercedes/pysecdec/ltd_topology_f_0/ltd_topology_f_0_integral/codegen/sector22.h
+-rw-r--r--   0      501       20      264 2024-03-31 16:30:37.000000 gammaloop-0.1.0/python/gammaloop/examples/cards/scalar_mercedes/pysecdec/ltd_topology_f_0/ltd_topology_f_0_integral/codegen/sector25.d
+-rw-r--r--   0      501       20     4524 2024-03-31 16:30:37.000000 gammaloop-0.1.0/python/gammaloop/examples/cards/scalar_mercedes/pysecdec/ltd_topology_f_0/ltd_topology_f_0_integral/codegen/sector25.h
+-rw-r--r--   0      501       20      264 2024-03-31 16:30:37.000000 gammaloop-0.1.0/python/gammaloop/examples/cards/scalar_mercedes/pysecdec/ltd_topology_f_0/ltd_topology_f_0_integral/codegen/sector26.d
+-rw-r--r--   0      501       20     4484 2024-03-31 16:30:37.000000 gammaloop-0.1.0/python/gammaloop/examples/cards/scalar_mercedes/pysecdec/ltd_topology_f_0/ltd_topology_f_0_integral/codegen/sector26.h
+-rw-r--r--   0      501       20      264 2024-03-31 16:30:37.000000 gammaloop-0.1.0/python/gammaloop/examples/cards/scalar_mercedes/pysecdec/ltd_topology_f_0/ltd_topology_f_0_integral/codegen/sector29.d
+-rw-r--r--   0      501       20     4484 2024-03-31 16:30:37.000000 gammaloop-0.1.0/python/gammaloop/examples/cards/scalar_mercedes/pysecdec/ltd_topology_f_0/ltd_topology_f_0_integral/codegen/sector29.h
+-rw-r--r--   0      501       20      264 2024-03-31 16:30:37.000000 gammaloop-0.1.0/python/gammaloop/examples/cards/scalar_mercedes/pysecdec/ltd_topology_f_0/ltd_topology_f_0_integral/codegen/sector30.d
+-rw-r--r--   0      501       20     4452 2024-03-31 16:30:37.000000 gammaloop-0.1.0/python/gammaloop/examples/cards/scalar_mercedes/pysecdec/ltd_topology_f_0/ltd_topology_f_0_integral/codegen/sector30.h
+-rw-r--r--   0      501       20      264 2024-03-31 16:30:37.000000 gammaloop-0.1.0/python/gammaloop/examples/cards/scalar_mercedes/pysecdec/ltd_topology_f_0/ltd_topology_f_0_integral/codegen/sector33.d
+-rw-r--r--   0      501       20     4470 2024-03-31 16:30:37.000000 gammaloop-0.1.0/python/gammaloop/examples/cards/scalar_mercedes/pysecdec/ltd_topology_f_0/ltd_topology_f_0_integral/codegen/sector33.h
+-rw-r--r--   0      501       20       58 2024-03-31 16:30:37.000000 gammaloop-0.1.0/python/gammaloop/examples/cards/scalar_mercedes/pysecdec/ltd_topology_f_0/ltd_topology_f_0_integral/codegen/sector34.d
+-rw-r--r--   0      501       20     4501 2024-03-31 16:30:37.000000 gammaloop-0.1.0/python/gammaloop/examples/cards/scalar_mercedes/pysecdec/ltd_topology_f_0/ltd_topology_f_0_integral/codegen/sector34.h
+-rw-r--r--   0      501       20      264 2024-03-31 16:30:37.000000 gammaloop-0.1.0/python/gammaloop/examples/cards/scalar_mercedes/pysecdec/ltd_topology_f_0/ltd_topology_f_0_integral/codegen/sector37.d
+-rw-r--r--   0      501       20     4525 2024-03-31 16:30:37.000000 gammaloop-0.1.0/python/gammaloop/examples/cards/scalar_mercedes/pysecdec/ltd_topology_f_0/ltd_topology_f_0_integral/codegen/sector37.h
+-rw-r--r--   0      501       20      264 2024-03-31 16:30:37.000000 gammaloop-0.1.0/python/gammaloop/examples/cards/scalar_mercedes/pysecdec/ltd_topology_f_0/ltd_topology_f_0_integral/codegen/sector41.d
+-rw-r--r--   0      501       20     4516 2024-03-31 16:30:37.000000 gammaloop-0.1.0/python/gammaloop/examples/cards/scalar_mercedes/pysecdec/ltd_topology_f_0/ltd_topology_f_0_integral/codegen/sector41.h
+-rw-r--r--   0      501       20      264 2024-03-31 16:30:37.000000 gammaloop-0.1.0/python/gammaloop/examples/cards/scalar_mercedes/pysecdec/ltd_topology_f_0/ltd_topology_f_0_integral/codegen/sector45.d
+-rw-r--r--   0      501       20     4461 2024-03-31 16:30:37.000000 gammaloop-0.1.0/python/gammaloop/examples/cards/scalar_mercedes/pysecdec/ltd_topology_f_0/ltd_topology_f_0_integral/codegen/sector45.h
+-rw-r--r--   0      501       20      264 2024-03-31 16:30:37.000000 gammaloop-0.1.0/python/gammaloop/examples/cards/scalar_mercedes/pysecdec/ltd_topology_f_0/ltd_topology_f_0_integral/codegen/sector49.d
+-rw-r--r--   0      501       20     4516 2024-03-31 16:30:37.000000 gammaloop-0.1.0/python/gammaloop/examples/cards/scalar_mercedes/pysecdec/ltd_topology_f_0/ltd_topology_f_0_integral/codegen/sector49.h
+-rw-r--r--   0      501       20      253 2024-03-31 16:30:37.000000 gammaloop-0.1.0/python/gammaloop/examples/cards/scalar_mercedes/pysecdec/ltd_topology_f_0/ltd_topology_f_0_integral/codegen/sector5.d
+-rw-r--r--   0      501       20     4459 2024-03-31 16:30:37.000000 gammaloop-0.1.0/python/gammaloop/examples/cards/scalar_mercedes/pysecdec/ltd_topology_f_0/ltd_topology_f_0_integral/codegen/sector5.h
+-rw-r--r--   0      501       20      264 2024-03-31 16:30:37.000000 gammaloop-0.1.0/python/gammaloop/examples/cards/scalar_mercedes/pysecdec/ltd_topology_f_0/ltd_topology_f_0_integral/codegen/sector50.d
+-rw-r--r--   0      501       20     4461 2024-03-31 16:30:37.000000 gammaloop-0.1.0/python/gammaloop/examples/cards/scalar_mercedes/pysecdec/ltd_topology_f_0/ltd_topology_f_0_integral/codegen/sector50.h
+-rw-r--r--   0      501       20      264 2024-03-31 16:30:37.000000 gammaloop-0.1.0/python/gammaloop/examples/cards/scalar_mercedes/pysecdec/ltd_topology_f_0/ltd_topology_f_0_integral/codegen/sector53.d
+-rw-r--r--   0      501       20     4470 2024-03-31 16:30:37.000000 gammaloop-0.1.0/python/gammaloop/examples/cards/scalar_mercedes/pysecdec/ltd_topology_f_0/ltd_topology_f_0_integral/codegen/sector53.h
+-rw-r--r--   0      501       20      264 2024-03-31 16:30:37.000000 gammaloop-0.1.0/python/gammaloop/examples/cards/scalar_mercedes/pysecdec/ltd_topology_f_0/ltd_topology_f_0_integral/codegen/sector54.d
+-rw-r--r--   0      501       20     4516 2024-03-31 16:30:37.000000 gammaloop-0.1.0/python/gammaloop/examples/cards/scalar_mercedes/pysecdec/ltd_topology_f_0/ltd_topology_f_0_integral/codegen/sector54.h
+-rw-r--r--   0      501       20      264 2024-03-31 16:30:37.000000 gammaloop-0.1.0/python/gammaloop/examples/cards/scalar_mercedes/pysecdec/ltd_topology_f_0/ltd_topology_f_0_integral/codegen/sector57.d
+-rw-r--r--   0      501       20     4507 2024-03-31 16:30:37.000000 gammaloop-0.1.0/python/gammaloop/examples/cards/scalar_mercedes/pysecdec/ltd_topology_f_0/ltd_topology_f_0_integral/codegen/sector57.h
+-rw-r--r--   0      501       20      253 2024-03-31 16:30:37.000000 gammaloop-0.1.0/python/gammaloop/examples/cards/scalar_mercedes/pysecdec/ltd_topology_f_0/ltd_topology_f_0_integral/codegen/sector6.d
+-rw-r--r--   0      501       20     4468 2024-03-31 16:30:37.000000 gammaloop-0.1.0/python/gammaloop/examples/cards/scalar_mercedes/pysecdec/ltd_topology_f_0/ltd_topology_f_0_integral/codegen/sector6.h
+-rw-r--r--   0      501       20      264 2024-03-31 16:30:37.000000 gammaloop-0.1.0/python/gammaloop/examples/cards/scalar_mercedes/pysecdec/ltd_topology_f_0/ltd_topology_f_0_integral/codegen/sector61.d
+-rw-r--r--   0      501       20     4516 2024-03-31 16:30:37.000000 gammaloop-0.1.0/python/gammaloop/examples/cards/scalar_mercedes/pysecdec/ltd_topology_f_0/ltd_topology_f_0_integral/codegen/sector61.h
+-rw-r--r--   0      501       20      253 2024-03-31 16:30:37.000000 gammaloop-0.1.0/python/gammaloop/examples/cards/scalar_mercedes/pysecdec/ltd_topology_f_0/ltd_topology_f_0_integral/codegen/sector9.d
+-rw-r--r--   0      501       20     4468 2024-03-31 16:30:37.000000 gammaloop-0.1.0/python/gammaloop/examples/cards/scalar_mercedes/pysecdec/ltd_topology_f_0/ltd_topology_f_0_integral/codegen/sector9.h
+-rw-r--r--   0      501       20     6477 2024-03-31 16:30:32.000000 gammaloop-0.1.0/python/gammaloop/examples/cards/scalar_mercedes/pysecdec/ltd_topology_f_0/ltd_topology_f_0_integral/cuda_integrate_ltd_topology_f_0_integral.cpp
+-rw-r--r--   0      501       20     7187 2024-03-31 16:30:32.000000 gammaloop-0.1.0/python/gammaloop/examples/cards/scalar_mercedes/pysecdec/ltd_topology_f_0/ltd_topology_f_0_integral/distsrc/builtin.cpp
+-rw-r--r--   0      501       20     9392 2024-03-31 16:30:32.000000 gammaloop-0.1.0/python/gammaloop/examples/cards/scalar_mercedes/pysecdec/ltd_topology_f_0/ltd_topology_f_0_integral/distsrc/builtin.cu
+-rw-r--r--   0      501       20    19363 2024-03-31 16:30:32.000000 gammaloop-0.1.0/python/gammaloop/examples/cards/scalar_mercedes/pysecdec/ltd_topology_f_0/ltd_topology_f_0_integral/distsrc/common_cpu.h
+-rw-r--r--   0      501       20     3573 2024-03-31 16:30:32.000000 gammaloop-0.1.0/python/gammaloop/examples/cards/scalar_mercedes/pysecdec/ltd_topology_f_0/ltd_topology_f_0_integral/distsrc/common_cuda.h
+-rw-r--r--   0      501       20     6084 2024-03-31 16:30:32.000000 gammaloop-0.1.0/python/gammaloop/examples/cards/scalar_mercedes/pysecdec/ltd_topology_f_0/ltd_topology_f_0_integral/integrate_ltd_topology_f_0_integral.cpp
+-rw-r--r--   0      501       20    10677 2024-03-31 16:30:32.000000 gammaloop-0.1.0/python/gammaloop/examples/cards/scalar_mercedes/pysecdec/ltd_topology_f_0/ltd_topology_f_0_integral/src/SecDecInternalFunctions.hpp
+-rw-r--r--   0      501       20    41255 2024-03-31 16:30:32.000000 gammaloop-0.1.0/python/gammaloop/examples/cards/scalar_mercedes/pysecdec/ltd_topology_f_0/pylink/pylink.cpp
+-rw-r--r--   0      501       20    15741 2024-03-31 16:30:32.000000 gammaloop-0.1.0/python/gammaloop/examples/cards/scalar_mercedes/pysecdec/ltd_topology_f_0/pylink/qmc_template_instantiations_0.cpp
+-rw-r--r--   0      501       20    51608 2024-03-31 16:30:32.000000 gammaloop-0.1.0/python/gammaloop/examples/cards/scalar_mercedes/pysecdec/ltd_topology_f_0/src/amplitude.cpp
+-rw-r--r--   0      501       20    42991 2024-03-31 16:30:32.000000 gammaloop-0.1.0/python/gammaloop/examples/cards/scalar_mercedes/pysecdec/ltd_topology_f_0/src/ltd_topology_f_0_integral_weighted_integral.cpp
+-rw-r--r--   0      501       20     1300 2024-03-31 16:30:32.000000 gammaloop-0.1.0/python/gammaloop/examples/cards/scalar_mercedes/pysecdec/ltd_topology_f_0/src/ltd_topology_f_0_integral_weighted_integral.hpp
+-rw-r--r--   0      501       20        1 2024-03-31 16:29:02.000000 gammaloop-0.1.0/python/gammaloop/examples/cards/scalar_mercedes/pysecdec/numerator_ltd_topology_f_0.txt
+-rw-r--r--   0      501       20    15024 2024-03-31 16:29:02.000000 gammaloop-0.1.0/python/gammaloop/examples/cards/scalar_mercedes/pysecdec/run_ltd_topology_f_0.py
+-rw-r--r--   0      501       20      135 2024-03-31 16:28:59.000000 gammaloop-0.1.0/python/gammaloop/examples/cards/scalar_mercedes/runs/run.yaml
+-rw-r--r--   0      501       20     3332 2024-03-31 16:28:52.000000 gammaloop-0.1.0/python/gammaloop/examples/cards/scalar_mercedes/sources/amplitudes/ltd_topology_f/amplitude.yaml
+-rw-r--r--   0      501       20   153769 2024-03-31 16:28:52.000000 gammaloop-0.1.0/python/gammaloop/examples/cards/scalar_mercedes/sources/amplitudes/ltd_topology_f/derived_data_ltd_topology_f_0.bin
+-rw-r--r--   0      501       20     7787 2024-03-31 16:28:52.000000 gammaloop-0.1.0/python/gammaloop/examples/cards/scalar_mercedes/sources/amplitudes/ltd_topology_f/drawings/0_ltd_topology_f_0.tex
+-rwxr-xr-x   0      501       20     2885 2024-03-31 16:28:52.000000 gammaloop-0.1.0/python/gammaloop/examples/cards/scalar_mercedes/sources/amplitudes/ltd_topology_f/drawings/combine_pages.py
+-rw-r--r--   0      501       20      921 2024-03-31 16:28:52.000000 gammaloop-0.1.0/python/gammaloop/examples/cards/scalar_mercedes/sources/amplitudes/ltd_topology_f/drawings/makefile
+-rw-r--r--   0      501       20     8192 2024-03-31 16:28:52.000000 gammaloop-0.1.0/python/gammaloop/examples/cards/scalar_mercedes/sources/model/scalars.yaml
+-rw-r--r--   0      501       20    64931 2024-03-31 16:28:58.000000 gammaloop-0.1.0/python/gammaloop/examples/cards/scalar_mercedes/workspace/integration_state
+-rw-r--r--   0      501       20     2642 2024-03-31 16:28:58.000000 gammaloop-0.1.0/python/gammaloop/examples/cards/scalar_mercedes/workspace/settings.yaml
+-rw-r--r--   0      501       20     1035 2024-04-02 22:34:14.000000 gammaloop-0.1.0/python/gammaloop/examples/cards/scalar_mercedes.gL
+-rw-r--r--   0      501       20        0 2024-04-02 22:34:14.000000 gammaloop-0.1.0/python/gammaloop/examples/jupyter/__init__.py
+-rw-r--r--   0      501       20     5672 2024-04-02 22:34:14.000000 gammaloop-0.1.0/python/gammaloop/examples/jupyter/steer_gammaloop.ipynb
+-rw-r--r--   0      501       20        0 2023-09-05 12:02:39.000000 gammaloop-0.1.0/python/gammaloop/exporters/__init__.py
+-rw-r--r--   0      501       20    15844 2024-04-02 22:34:14.000000 gammaloop-0.1.0/python/gammaloop/exporters/exporters.py
+-rw-r--r--   0      501       20      353 2024-04-02 22:34:14.000000 gammaloop-0.1.0/python/gammaloop/interface/__init__.py
+-rw-r--r--   0      501       20    48537 2024-04-02 22:34:14.000000 gammaloop-0.1.0/python/gammaloop/interface/gammaloop_interface.py
+-rw-r--r--   0      501       20       81 2024-04-02 22:34:14.000000 gammaloop-0.1.0/python/gammaloop/misc/__init__.py
+-rw-r--r--   0      501       20     5658 2024-04-02 22:34:14.000000 gammaloop-0.1.0/python/gammaloop/misc/common.py
+-rw-r--r--   0      501       20    23669 2024-04-02 22:34:14.000000 gammaloop-0.1.0/python/gammaloop/misc/utils.py
+-rw-r--r--   0      501       20        0 2023-09-11 15:39:58.000000 gammaloop-0.1.0/python/gammaloop/py.typed
+-rw-r--r--   0      501       20      347 2024-03-20 12:28:49.000000 gammaloop-0.1.0/python/gammaloop/pytest.ini
+-rw-r--r--   0      501       20       30 2024-04-02 22:34:14.000000 gammaloop-0.1.0/python/gammaloop/requirements.txt
+-rwxr-xr-x   0      501       20      210 2024-03-20 12:28:49.000000 gammaloop-0.1.0/python/gammaloop/run_python_tests.sh
+-rw-r--r--   0      501       20      428 2024-04-02 22:34:14.000000 gammaloop-0.1.0/python/gammaloop/tests/__init__.py
+-rw-r--r--   0      501       20     3424 2024-04-02 22:34:14.000000 gammaloop-0.1.0/python/gammaloop/tests/common.py
+-rw-r--r--   0      501       20    11386 2024-04-02 22:34:14.000000 gammaloop-0.1.0/python/gammaloop/tests/conftest.py
+-rw-r--r--   0      501       20        0 2023-09-05 10:38:09.000000 gammaloop-0.1.0/python/gammaloop/tests/integration/__init__.py
+-rw-r--r--   0      501       20     3798 2024-04-02 22:34:14.000000 gammaloop-0.1.0/python/gammaloop/tests/integration/test_integral.py
+-rw-r--r--   0      501       20     1579 2024-04-02 18:22:38.000000 gammaloop-0.1.0/python/gammaloop/tests/test_data/models/loop_sm/.restrict_parallel_test.dat
+-rw-r--r--   0      501       20     1579 2024-04-02 18:22:38.000000 gammaloop-0.1.0/python/gammaloop/tests/test_data/models/loop_sm/.restrict_parallel_test_c_massive.dat
+-rw-r--r--   0      501       20    28489 2024-04-02 22:34:14.000000 gammaloop-0.1.0/python/gammaloop/tests/test_data/models/loop_sm/CT_couplings.py
+-rw-r--r--   0      501       20     7383 2024-04-02 22:34:14.000000 gammaloop-0.1.0/python/gammaloop/tests/test_data/models/loop_sm/CT_parameters.py
+-rw-r--r--   0      501       20    40823 2024-04-02 22:34:14.000000 gammaloop-0.1.0/python/gammaloop/tests/test_data/models/loop_sm/CT_vertices.py
+-rw-r--r--   0      501       20      892 2024-04-02 22:34:14.000000 gammaloop-0.1.0/python/gammaloop/tests/test_data/models/loop_sm/__init__.py
+-rw-r--r--   0      501       20      586 2024-04-02 22:34:14.000000 gammaloop-0.1.0/python/gammaloop/tests/test_data/models/loop_sm/coupling_orders.py
+-rw-r--r--   0      501       20    13624 2024-04-02 22:34:14.000000 gammaloop-0.1.0/python/gammaloop/tests/test_data/models/loop_sm/couplings.py
+-rw-r--r--   0      501       20     1817 2024-04-02 22:34:14.000000 gammaloop-0.1.0/python/gammaloop/tests/test_data/models/loop_sm/function_library.py
+-rw-r--r--   0      501       20     6273 2024-04-02 22:34:14.000000 gammaloop-0.1.0/python/gammaloop/tests/test_data/models/loop_sm/lorentz.py
+-rw-r--r--   0      501       20     8686 2024-04-02 22:34:14.000000 gammaloop-0.1.0/python/gammaloop/tests/test_data/models/loop_sm/object_library.py
+-rw-r--r--   0      501       20    26880 2024-04-02 22:34:14.000000 gammaloop-0.1.0/python/gammaloop/tests/test_data/models/loop_sm/parameters.py
+-rw-r--r--   0      501       20     9783 2024-04-02 22:34:14.000000 gammaloop-0.1.0/python/gammaloop/tests/test_data/models/loop_sm/particles.py
+-rw-r--r--   0      501       20     1574 2024-04-02 22:34:14.000000 gammaloop-0.1.0/python/gammaloop/tests/test_data/models/loop_sm/restrict_c_mass.dat
+-rw-r--r--   0      501       20     1574 2024-04-02 22:34:14.000000 gammaloop-0.1.0/python/gammaloop/tests/test_data/models/loop_sm/restrict_ckm.dat
+-rw-r--r--   0      501       20     1573 2024-04-02 22:34:14.000000 gammaloop-0.1.0/python/gammaloop/tests/test_data/models/loop_sm/restrict_default.dat
+-rw-r--r--   0      501       20     3649 2024-04-02 22:34:14.000000 gammaloop-0.1.0/python/gammaloop/tests/test_data/models/loop_sm/restrict_full.dat
+-rw-r--r--   0      501       20     1570 2024-04-02 22:34:14.000000 gammaloop-0.1.0/python/gammaloop/tests/test_data/models/loop_sm/restrict_lepton_masses.dat
+-rw-r--r--   0      501       20     1574 2024-04-02 22:34:14.000000 gammaloop-0.1.0/python/gammaloop/tests/test_data/models/loop_sm/restrict_no_b_mass.dat
+-rw-r--r--   0      501       20     1574 2024-04-02 22:34:14.000000 gammaloop-0.1.0/python/gammaloop/tests/test_data/models/loop_sm/restrict_no_masses.dat
+-rw-r--r--   0      501       20     1574 2024-04-02 22:34:14.000000 gammaloop-0.1.0/python/gammaloop/tests/test_data/models/loop_sm/restrict_no_tau_mass.dat
+-rw-r--r--   0      501       20     1568 2024-04-02 22:34:14.000000 gammaloop-0.1.0/python/gammaloop/tests/test_data/models/loop_sm/restrict_no_widths.dat
+-rw-r--r--   0      501       20     1579 2024-04-02 22:34:14.000000 gammaloop-0.1.0/python/gammaloop/tests/test_data/models/loop_sm/restrict_parallel_test.dat
+-rw-r--r--   0      501       20     1625 2024-04-02 22:34:14.000000 gammaloop-0.1.0/python/gammaloop/tests/test_data/models/loop_sm/restrict_test.dat
+-rw-r--r--   0      501       20     1574 2024-04-02 22:34:14.000000 gammaloop-0.1.0/python/gammaloop/tests/test_data/models/loop_sm/restrict_zeromass_ckm.dat
+-rw-r--r--   0      501       20    28414 2024-04-02 22:34:14.000000 gammaloop-0.1.0/python/gammaloop/tests/test_data/models/loop_sm/vertices.py
+-rwxr-xr-x   0      501       20     6826 2024-04-02 22:34:14.000000 gammaloop-0.1.0/python/gammaloop/tests/test_data/models/loop_sm/write_param_card.py
+-rw-r--r--   0      501       20     1927 2023-10-24 16:08:30.000000 gammaloop-0.1.0/python/gammaloop/tests/test_data/qgraf_outputs/bubble.py
+-rw-r--r--   0      501       20     8480 2023-10-07 18:01:33.000000 gammaloop-0.1.0/python/gammaloop/tests/test_data/qgraf_outputs/cube.py
+-rw-r--r--   0      501       20     3124 2023-11-08 15:11:24.000000 gammaloop-0.1.0/python/gammaloop/tests/test_data/qgraf_outputs/double_triangle.py
+-rw-r--r--   0      501       20    13004 2023-09-05 12:46:18.000000 gammaloop-0.1.0/python/gammaloop/tests/test_data/qgraf_outputs/epem_a_ddx_NLO.py
+-rw-r--r--   0      501       20     7127 2023-09-29 14:40:59.000000 gammaloop-0.1.0/python/gammaloop/tests/test_data/qgraf_outputs/fishnet_2x2.py
+-rw-r--r--   0      501       20     9012 2023-09-29 14:48:10.000000 gammaloop-0.1.0/python/gammaloop/tests/test_data/qgraf_outputs/fishnet_2x3.py
+-rw-r--r--   0      501       20     5184 2023-11-08 15:11:24.000000 gammaloop-0.1.0/python/gammaloop/tests/test_data/qgraf_outputs/isopod.py
+-rw-r--r--   0      501       20     3697 2024-04-02 22:34:14.000000 gammaloop-0.1.0/python/gammaloop/tests/test_data/qgraf_outputs/lbl_box.py
+-rw-r--r--   0      501       20     6540 2024-04-02 22:34:14.000000 gammaloop-0.1.0/python/gammaloop/tests/test_data/qgraf_outputs/ltd_paper/topology_c.py
+-rw-r--r--   0      501       20     6450 2024-04-02 22:34:14.000000 gammaloop-0.1.0/python/gammaloop/tests/test_data/qgraf_outputs/ltd_paper/topology_cstar.py
+-rw-r--r--   0      501       20     5925 2024-04-02 22:34:14.000000 gammaloop-0.1.0/python/gammaloop/tests/test_data/qgraf_outputs/ltd_paper/topology_e.py
+-rw-r--r--   0      501       20     3452 2024-04-02 22:34:14.000000 gammaloop-0.1.0/python/gammaloop/tests/test_data/qgraf_outputs/ltd_paper/topology_f.py
+-rw-r--r--   0      501       20     3452 2024-04-02 22:34:14.000000 gammaloop-0.1.0/python/gammaloop/tests/test_data/qgraf_outputs/ltd_paper/topology_fstar.py
+-rw-r--r--   0      501       20     7112 2024-04-02 22:34:14.000000 gammaloop-0.1.0/python/gammaloop/tests/test_data/qgraf_outputs/ltd_paper/topology_g.py
+-rw-r--r--   0      501       20     4296 2024-04-02 22:34:14.000000 gammaloop-0.1.0/python/gammaloop/tests/test_data/qgraf_outputs/ltd_paper/topology_h.py
+-rw-r--r--   0      501       20     3452 2024-04-02 22:34:14.000000 gammaloop-0.1.0/python/gammaloop/tests/test_data/qgraf_outputs/ltd_topology_f.py
+-rw-r--r--   0      501       20     4296 2024-04-02 22:34:14.000000 gammaloop-0.1.0/python/gammaloop/tests/test_data/qgraf_outputs/ltd_topology_h.py
+-rw-r--r--   0      501       20     3757 2023-11-08 15:11:24.000000 gammaloop-0.1.0/python/gammaloop/tests/test_data/qgraf_outputs/massless_box.py
+-rw-r--r--   0      501       20     2888 2023-09-29 13:33:20.000000 gammaloop-0.1.0/python/gammaloop/tests/test_data/qgraf_outputs/massless_triangle.py
+-rw-r--r--   0      501       20     3713 2023-11-08 15:11:24.000000 gammaloop-0.1.0/python/gammaloop/tests/test_data/qgraf_outputs/mercedes.py
+-rw-r--r--   0      501       20     2193 2023-11-08 15:11:24.000000 gammaloop-0.1.0/python/gammaloop/tests/test_data/qgraf_outputs/sunrise.py
+-rw-r--r--   0      501       20     3686 2024-04-02 22:34:14.000000 gammaloop-0.1.0/python/gammaloop/tests/test_data/qgraf_outputs/tree_triangle.py
+-rw-r--r--   0      501       20     4021 2023-11-08 15:11:24.000000 gammaloop-0.1.0/python/gammaloop/tests/test_data/qgraf_outputs/triangle_box.py
+-rw-r--r--   0      501       20      947 2024-04-02 22:34:14.000000 gammaloop-0.1.0/python/gammaloop/tests/test_data/test_configs/ltd_topology_f.yaml
+-rw-r--r--   0      501       20      947 2024-04-02 22:34:14.000000 gammaloop-0.1.0/python/gammaloop/tests/test_data/test_configs/ltd_topology_h.yaml
+-rw-r--r--   0      501       20     1006 2024-04-02 22:34:14.000000 gammaloop-0.1.0/python/gammaloop/tests/test_data/test_configs/massless_triangle.yaml
+-rw-r--r--   0      501       20     1062 2024-04-02 22:34:14.000000 gammaloop-0.1.0/python/gammaloop/tests/test_data/test_configs/tree_triangle.yaml
+-rw-r--r--   0      501       20        0 2023-09-05 10:38:04.000000 gammaloop-0.1.0/python/gammaloop/tests/unit/__init__.py
+-rw-r--r--   0      501       20    19222 2024-04-02 22:34:14.000000 gammaloop-0.1.0/python/gammaloop/tests/unit/test_commands.py
+-rw-r--r--   0      501       20      956 2023-10-11 21:13:09.000000 gammaloop-0.1.0/python/gammaloop/tests/unit/test_graph_functions.py
+-rw-r--r--   0      501       20     2718 2024-04-02 22:34:14.000000 gammaloop-0.1.0/python/gammaloop/tests/unit/test_misc.py
+-rw-r--r--   0      501       20     4686 2024-03-20 12:28:49.000000 gammaloop-0.1.0/python/gammaloop/tests/unit/test_objects.py
+-rw-r--r--   0      501       20     2826 2024-04-02 22:34:14.000000 gammaloop-0.1.0/python/gammaloop/tests/unit/test_rust.py
+-rw-r--r--   0      501       20    47442 2024-03-21 10:12:49.000000 gammaloop-0.1.0/sm.yaml
+-rw-r--r--   0      501       20    22613 2024-04-02 22:34:14.000000 gammaloop-0.1.0/src/api/python.rs
+-rw-r--r--   0      501       20       47 2023-09-11 08:31:47.000000 gammaloop-0.1.0/src/api.rs
+-rw-r--r--   0      501       20      441 2023-10-16 08:31:15.000000 gammaloop-0.1.0/src/bin/cli.rs
+-rw-r--r--   0      501       20    72475 2024-04-02 22:34:14.000000 gammaloop-0.1.0/src/cff.rs
+-rw-r--r--   0      501       20    13773 2024-04-02 22:34:14.000000 gammaloop-0.1.0/src/cli_functions.rs
+-rw-r--r--   0      501       20    28006 2024-04-02 22:34:14.000000 gammaloop-0.1.0/src/cross_section.rs
+-rw-r--r--   0      501       20     8750 2024-04-02 22:34:14.000000 gammaloop-0.1.0/src/evaluation_result.rs
+-rw-r--r--   0      501       20    42280 2024-04-02 22:34:14.000000 gammaloop-0.1.0/src/gammaloop_integrand.rs
+-rw-r--r--   0      501       20    53894 2024-04-02 22:34:14.000000 gammaloop-0.1.0/src/graph.rs
+-rw-r--r--   0      501       20     6100 2024-04-02 22:34:14.000000 gammaloop-0.1.0/src/h_function_test.rs
+-rw-r--r--   0      501       20     2584 2024-04-02 22:34:14.000000 gammaloop-0.1.0/src/inspect.rs
+-rw-r--r--   0      501       20    12573 2024-04-02 22:34:14.000000 gammaloop-0.1.0/src/integrands.rs
+-rw-r--r--   0      501       20    43608 2024-04-02 22:34:14.000000 gammaloop-0.1.0/src/integrate.rs
+-rw-r--r--   0      501       20    10167 2024-04-02 22:34:14.000000 gammaloop-0.1.0/src/lib.rs
+-rw-r--r--   0      501       20    11451 2024-04-02 22:34:14.000000 gammaloop-0.1.0/src/linalg.rs
+-rw-r--r--   0      501       20    25144 2024-04-02 22:34:14.000000 gammaloop-0.1.0/src/ltd.rs
+-rw-r--r--   0      501       20    29313 2024-04-02 22:34:14.000000 gammaloop-0.1.0/src/model.rs
+-rw-r--r--   0      501       20     1060 2024-04-02 22:34:14.000000 gammaloop-0.1.0/src/numerator/tests.rs
+-rw-r--r--   0      501       20     2786 2024-04-02 22:34:14.000000 gammaloop-0.1.0/src/numerator.rs
+-rw-r--r--   0      501       20    44710 2024-04-02 22:34:14.000000 gammaloop-0.1.0/src/observables.rs
+-rw-r--r--   0      501       20    16966 2024-04-02 22:34:14.000000 gammaloop-0.1.0/src/tensor/arithmetic.rs
+-rw-r--r--   0      501       20    27638 2024-04-02 22:34:14.000000 gammaloop-0.1.0/src/tensor/contraction.rs
+-rw-r--r--   0      501       20    25311 2024-04-02 22:34:14.000000 gammaloop-0.1.0/src/tensor/data.rs
+-rw-r--r--   0      501       20    43115 2024-03-20 12:28:49.000000 gammaloop-0.1.0/src/tensor/iterators.rs
+-rw-r--r--   0      501       20    24274 2024-04-02 22:34:14.000000 gammaloop-0.1.0/src/tensor/network.rs
+-rw-r--r--   0      501       20     7293 2024-04-02 22:34:14.000000 gammaloop-0.1.0/src/tensor/num_tensor.rs
+-rw-r--r--   0      501       20     8673 2024-03-20 12:28:49.000000 gammaloop-0.1.0/src/tensor/parametric.rs
+-rw-r--r--   0      501       20    56368 2024-04-02 22:34:14.000000 gammaloop-0.1.0/src/tensor/structure.rs
+-rw-r--r--   0      501       20     9258 2024-04-02 22:34:14.000000 gammaloop-0.1.0/src/tensor/symbolic.rs
+-rw-r--r--   0      501       20    28347 2024-04-02 22:34:14.000000 gammaloop-0.1.0/src/tensor/tests.rs
+-rw-r--r--   0      501       20    15548 2024-04-02 22:34:14.000000 gammaloop-0.1.0/src/tensor/ufo.rs
+-rw-r--r--   0      501       20    10037 2024-04-02 22:34:14.000000 gammaloop-0.1.0/src/tensor/upgrading_arithmetic.rs
+-rw-r--r--   0      501       20     1847 2024-03-20 12:28:49.000000 gammaloop-0.1.0/src/tensor.rs
+-rw-r--r--   0      501       20      977 2024-04-02 22:34:14.000000 gammaloop-0.1.0/src/test_resources/default_tests_config.yaml
+-rw-r--r--   0      501       20       59 2024-04-02 22:34:14.000000 gammaloop-0.1.0/src/test_resources/lbl/output_metadata.yaml
+-rw-r--r--   0      501       20     3072 2024-04-02 22:34:14.000000 gammaloop-0.1.0/src/test_resources/lbl/sources/amplitudes/lbl_box/amplitude.yaml
+-rw-r--r--   0      501       20     3719 2024-04-02 22:34:14.000000 gammaloop-0.1.0/src/test_resources/lbl/sources/model/coupling_replacements.json
+-rw-r--r--   0      501       20    51441 2024-04-02 22:34:14.000000 gammaloop-0.1.0/src/test_resources/lbl/sources/model/sm.yaml
+-rw-r--r--   0      501       20    12262 2024-04-02 22:34:14.000000 gammaloop-0.1.0/src/tests.rs
+-rw-r--r--   0      501       20    28312 2024-04-02 22:34:14.000000 gammaloop-0.1.0/src/tests_from_pytest.rs
+-rw-r--r--   0      501       20    49704 2024-04-02 22:34:14.000000 gammaloop-0.1.0/src/tropical.rs
+-rw-r--r--   0      501       20    58803 2024-04-02 22:34:14.000000 gammaloop-0.1.0/src/utils.rs
+-rw-r--r--   0      501       20      112 2023-11-27 15:12:18.000000 gammaloop-0.1.0/test_inspect.gL
+-rw-r--r--   0      501       20       76 2024-03-14 20:21:25.000000 gammaloop-0.1.0/test_load_model.gL
+-rw-r--r--   0      501       20       34 2024-03-20 18:09:51.000000 gammaloop-0.1.0/test_me.py
+-rw-r--r--   0      501       20     1961 2024-03-28 13:22:31.000000 gammaloop-0.1.0/test_opts.gL
+-rw-r--r--   0      501       20     1908 2024-03-31 16:33:17.000000 gammaloop-0.1.0/test_scalar_triangle.gL
+-rw-r--r--   0      501       20       97 2024-01-09 19:55:55.000000 gammaloop-0.1.0/tt.sh
+-rw-r--r--   0      501       20     2587 2024-04-02 22:34:14.000000 gammaloop-0.1.0/pyproject.toml
+-rw-r--r--   0      501       20        0 2024-04-02 19:19:18.000000 gammaloop-0.1.0/python/gammaloop/dependencies/INSTALLED
+-rw-r--r--   0        0        0     5377 1970-01-01 00:00:00.000000 gammaloop-0.1.0/PKG-INFO
```

### Comparing `gammaloop-0.0.1/Cargo.toml` & `gammaloop-0.1.0/mod_Cargo.toml`

 * *Files 14% similar despite different names*

```diff
@@ -2,30 +2,31 @@
 name = "gammalooprs"
 version = "0.0.1"
 edition = "2021"
 authors = ["Valentin Hirschi <valentin.hirschi@gmail.com>"]
 categories = ["science"]
 description = "An implementation of the Local Unitarity method for computing differential collider cross-sections."
 keywords = ["loop", "cross-section", "perturbative", "physics"]
-license-file = "License.md"
+license-file = "LICENSE.md"
 readme = "README.md"
 repository = "https://github.com/alphal00p/gammaloop"
 
 
 [profile.dev-optim]
 inherits = "dev"
 opt-level = 2
 
 [dependencies]
 # You may need bleeding edge changes
 symbolica = { git = "https://github.com/alphal00p/symbolica" }
 #symbolica = "*"
-#symbolica = { path = "YOUR_LOCAL_SYMBOLICA_BRANCH" }
+#symbolica = { path = "../symbolica" }
 serde = { version = "1.0", features = ["derive"] }
 serde_yaml = "*"
+bincode = "1.3.3"
 clap = "2.34"
 color-eyre = { version = "^0.3", default-features = false }
 eyre = "^0.4"
 f128 = { git = "https://github.com/benruijl/f128" }
 lorentz_vector = { git = "https://github.com/benruijl/lorentz_vector", branch = "hyperdual", features = [
     "serde_support",
     "hyperdual_support",
@@ -47,17 +48,20 @@
 itertools = "0.8"
 smartstring = { version = "*", features = ["serde"] }
 ahash = "*"
 vectorize = "0.2.0"
 log = "*"
 env_logger = "*"
 pyo3-log = "*"
+nalgebra = "0.32.3"
+num-complex = "0.4.4"
+rug = "1.22.0"
 
 [dependencies.pyo3]
-features = ["extension-module", "multiple-pymethods"]
+features = ["multiple-pymethods"]
 optional = true
 version = "0.19"
 
 [build-dependencies]
 pyo3-build-config = "*"
 
 [lib]
@@ -66,10 +70,13 @@
 required-features = ["python_api"]
 
 [[bin]]
 name = "cli"
 required-features = ["binary"]
 
 [features]
+extension-module = ["pyo3/extension-module"]
 default = ["python_api"]
+
 python_api = ["pyo3"]
 binary = []
+fail-on-warnings = []
```

### Comparing `gammaloop-0.0.1/.gitignore` & `gammaloop-0.1.0/.gitignore`

 * *Files 14% similar despite different names*

```diff
@@ -21,34 +21,56 @@
 wheels/
 share/python-wheels/
 *.egg-info/
 .installed.cfg
 *.egg
 MANIFEST
 
+out.yaml
+outmap.yaml
+params.yaml
+find-baseline.svg
+*.data
+*.old
+eval.cpp
+evaluate.cpp
+perf.data
 # logos
 logos/
 
 # C compiled objects
 *.o
 
+# Ignore swap files
+*.swp
+
+# ignore vscode repo
+.vscode/
+
 # compiled library
 *.a
 *.dylib
 
 # PyInstaller
 #  Usually these files are written by a python script from a template
 #  before PyInstaller builds the exe, so as to inject date/other infos into it.
 *.manifest
 *.spec
 
 # Installer logs
 pip-log.txt
 pip-delete-this-directory.txt
 
+# GammaLoop test outputs
+TEST_OUTPUT*/
+
+
+# General ignored directory
+ignore/
+
 # Unit test / coverage reports
 htmlcov/
 .tox/
 .nox/
 .coverage
 .coverage.*
 .cache
@@ -56,14 +78,21 @@
 coverage.xml
 *.cover
 *.py,cover
 .hypothesis/
 .pytest_cache/
 cover/
 
+# dependencies
+python/gammaloop/dependencies/LOCK
+python/gammaloop/dependencies/INSTALLED
+python/gammaloop/dependencies/dependency_build.log
+python/gammaloop/dependencies/venv/
+python/gammaloop/dependencies/symbolica/
+
 # Translations
 *.mo
 *.pot
 
 # Sphinx documentation
 docs/_build/
 
@@ -93,14 +122,17 @@
 .env
 .venv
 env/
 venv/
 ENV/
 env.bak/
 venv.bak/
+.devenv
+.direnv
+.envrc
 
 # mkdocs documentation
 /site
 
 # mypy
 .mypy_cache/
 .dmypy.json
@@ -121,16 +153,27 @@
 ### Rust ###
 # Generated by Cargo
 # will have compiled files and executables
 target/
 
 # Remove Cargo.lock from gitignore if creating an executable, leave it for libraries
 # More information here https://doc.rust-lang.org/cargo/guide/cargo-toml-vs-cargo-lock.html
-Cargo.lock
+# Cargo.lock
+
+poetry.lock
+
+# Target directory of rust tests
+rust_test_binaries
 
 # These are backup files generated by rustfmt
 **/*.rs.bk
 
 # MSVC Windows builds of rustc generate these, which store debugging information
 *.pdb
+default.nix
+
+# latex logs
+*.log
+# End of https://www.toptal.com/developers/gitignore/api/rust,python
 
-# End of https://www.toptal.com/developers/gitignore/api/rust,python
+# Ignore the local test resources
+src/test_resources/qqddg/
```

### Comparing `gammaloop-0.0.1/Cargo.lock` & `gammaloop-0.1.0/python/gammaloop/dependencies/symbolica/Cargo.lock`

 * *Files 4% similar despite different names*

```diff
@@ -15,885 +15,541 @@
 name = "adler"
 version = "1.0.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "f26201604c87b1e01bd3d98f8d5d9a8fcbb815e8cedb41ffccbeb4bf593a35fe"
 
 [[package]]
 name = "ahash"
-version = "0.8.3"
+version = "0.8.11"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "2c99f64d1e06488f620f932677e24bc6e2897582980441ae90a671415bd7ec2f"
+checksum = "e89da841a80418a9b391ebaea17f5c112ffaaa96f621d2c285b5174da76b9011"
 dependencies = [
  "cfg-if",
  "getrandom",
  "once_cell",
  "version_check",
+ "zerocopy",
 ]
 
 [[package]]
 name = "aho-corasick"
-version = "1.0.5"
+version = "1.1.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "0c378d78423fdad8089616f827526ee33c19f2fddbd5de1629152c9593ba4783"
+checksum = "8e60d3430d3a69478ad0993f19238d2df97c507009a52b3c10addcd7f6bcb916"
 dependencies = [
  "memchr",
 ]
 
 [[package]]
-name = "ansi_term"
-version = "0.11.0"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ee49baf6cb617b853aa8d93bf420db2383fab46d314482ca2803b40d5fde979b"
-dependencies = [
- "winapi",
-]
-
-[[package]]
-name = "ansi_term"
-version = "0.12.1"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d52a9bb7ec0cf484c551830a7ce27bd20d67eac647e1befb56b0be4ee39a55d2"
-dependencies = [
- "winapi",
-]
-
-[[package]]
-name = "approx"
-version = "0.5.1"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "cab112f0a86d568ea0e627cc1d6be74a1e9cd55214684db5561995f6dad897c6"
-dependencies = [
- "num-traits",
-]
-
-[[package]]
-name = "arc-swap"
-version = "1.6.0"
+name = "append-only-vec"
+version = "0.1.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "bddcadddf5e9015d310179a59bb28c4d4b9920ad0f11e8e14dbadf654890c9a6"
-
-[[package]]
-name = "atty"
-version = "0.2.14"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d9b39be18770d11421cdb1b9947a45dd3f37e93092cbf377614828a319d5fee8"
-dependencies = [
- "hermit-abi 0.1.19",
- "libc",
- "winapi",
-]
+checksum = "f3cb8f874ecf419dd8165d0279746de966cb8966636d028845e3bd65d519812a"
 
 [[package]]
 name = "autocfg"
-version = "1.1.0"
+version = "1.2.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d468802bab17cbc0cc575e9b053f41e72aa36bfa6b7f55e3529ffa43161b97fa"
+checksum = "f1fdabc7756949593fe60f30ec81974b613357de856987752631dea1e3394c80"
 
 [[package]]
 name = "az"
 version = "1.2.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "7b7e4c2464d97fe331d41de9d5db0def0a96f4d823b8b32a2efd503578988973"
 
 [[package]]
 name = "backtrace"
-version = "0.3.69"
+version = "0.3.71"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "2089b7e3f35b9dd2d0ed921ead4f6d318c27680d4a5bd167b3ee120edb105837"
+checksum = "26b05800d2e817c8b3b4b54abd461726265fa9789ae34330622f2db9ee696f9d"
 dependencies = [
  "addr2line",
  "cc",
  "cfg-if",
  "libc",
  "miniz_oxide",
  "object",
  "rustc-demangle",
 ]
 
 [[package]]
-name = "bitflags"
-version = "1.3.2"
+name = "bincode"
+version = "1.3.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "bef38d45163c2f1dde094a7dfd33ccf595c92905c8f8f4fdc18d06fb1037718a"
+checksum = "b1f45e9417d87227c7a56d22e471c6206462cba514c7590c09aff4cf6d1ddcad"
+dependencies = [
+ "serde",
+]
 
 [[package]]
 name = "bitflags"
-version = "2.4.0"
+version = "1.3.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b4682ae6287fcf752ecaabbfcc7b6f9b72aa33933dc23a554d853aea8eea8635"
+checksum = "bef38d45163c2f1dde094a7dfd33ccf595c92905c8f8f4fdc18d06fb1037718a"
 
 [[package]]
 name = "bytemuck"
-version = "1.14.0"
+version = "1.15.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "374d28ec25809ee0e23827c2ab573d729e293f281dfe393500e7ad618baa61c6"
+checksum = "5d6d68c57235a3a081186990eca2867354726650f42f7516ca50c28d6281fd15"
 
 [[package]]
 name = "byteorder"
-version = "1.4.3"
+version = "1.5.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "14c189c53d098945499cdfa7ecc63567cf3886b3332b312a5b4585d8d3a6a610"
+checksum = "1fd0f2584146f6f2ef48085050886acf353beff7305ebd1ae69500e27c67f64b"
 
 [[package]]
 name = "bytes"
-version = "1.5.0"
+version = "1.6.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a2bd12c1caf447e69cd4528f47f94d203fd2582878ecb9e9465484c4148a8223"
+checksum = "514de17de45fdb8dc022b1a7975556c53c86f9f0aa5f534b98977b171857c2c9"
 
 [[package]]
 name = "cc"
-version = "1.0.83"
+version = "1.0.90"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f1174fb0b6ec23863f8b971027804a42614e347eafb0a95bf0b12cdae21fc4d0"
-dependencies = [
- "libc",
-]
+checksum = "8cd6604a82acf3039f1144f54b8eb34e91ffba622051189e71b781822d5ee1f5"
 
 [[package]]
 name = "cfg-if"
 version = "1.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "baf1de4339761588bc0619e3cbc0120ee582ebb74b53b4efbf79117bd2da40fd"
 
 [[package]]
-name = "clap"
-version = "2.34.0"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a0610544180c38b88101fecf2dd634b174a62eef6946f84dfc6a7127512b381c"
-dependencies = [
- "ansi_term 0.12.1",
- "atty",
- "bitflags 1.3.2",
- "strsim",
- "textwrap",
- "unicode-width",
- "vec_map",
-]
-
-[[package]]
-name = "color-backtrace"
-version = "0.4.2"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5356ae4e07c994a2763226a8a991e5829ded78ac23f8ac88b3f3e69970db5163"
-dependencies = [
- "atty",
- "backtrace",
- "termcolor",
-]
-
-[[package]]
-name = "color-eyre"
-version = "0.3.4"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "2aaa5f071a62a9c06ebab653ec2e2ba76cb936548a83e7af7f0c5dac525067ff"
-dependencies = [
- "ansi_term 0.11.0",
- "backtrace",
- "color-backtrace",
- "eyre",
- "indenter",
- "once_cell",
-]
-
-[[package]]
 name = "colored"
-version = "2.0.4"
+version = "2.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "2674ec482fbc38012cf31e6c42ba0177b431a0cb6f15fe40efa5aab1bda516f6"
+checksum = "cbf2150cce219b664a8a70df7a1f933836724b503f8a413af9365b4dcc4d90b8"
 dependencies = [
- "is-terminal",
  "lazy_static",
  "windows-sys 0.48.0",
 ]
 
 [[package]]
-name = "crossbeam-channel"
-version = "0.5.8"
+name = "core-foundation"
+version = "0.9.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a33c2bf77f2df06183c3aa30d1e96c0695a313d4f9c453cc3762a6db39f99200"
+checksum = "91e195e091a93c46f7102ec7818a2aa394e1e1771c3ab4825963fa03e45afb8f"
 dependencies = [
- "cfg-if",
- "crossbeam-utils",
+ "core-foundation-sys",
+ "libc",
 ]
 
 [[package]]
+name = "core-foundation-sys"
+version = "0.8.6"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "06ea2b9bc92be3c2baa9334a323ebca2d6f074ff852cd1d7b11064035cd3868f"
+
+[[package]]
 name = "crossbeam-deque"
-version = "0.8.3"
+version = "0.8.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ce6fd6f855243022dcecf8702fef0c297d4338e226845fe067f6341ad9fa0cef"
+checksum = "613f8cc01fe9cf1a3eb3d7f488fd2fa8388403e97039e2f73692932e291a770d"
 dependencies = [
- "cfg-if",
  "crossbeam-epoch",
  "crossbeam-utils",
 ]
 
 [[package]]
 name = "crossbeam-epoch"
-version = "0.9.15"
+version = "0.9.18"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ae211234986c545741a7dc064309f67ee1e5ad243d0e48335adc0484d960bcc7"
+checksum = "5b82ac4a3c2ca9c3460964f020e1402edd5753411d7737aa39c3714ad1b5420e"
 dependencies = [
- "autocfg",
- "cfg-if",
  "crossbeam-utils",
- "memoffset",
- "scopeguard",
 ]
 
 [[package]]
 name = "crossbeam-utils"
-version = "0.8.16"
+version = "0.8.19"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "248e3bacc7dc6baa3b21e405ee045c3047101a49145e7e9eca583ab4c2ca5345"
+
+[[package]]
+name = "ctor"
+version = "0.1.26"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5a22b2d63d4d1dc0b7f1b6b2747dd0088008a9be28b6ddf0b1e7d335e3037294"
+checksum = "6d2301688392eb071b0bf1a37be05c469d3cc4dbbd95df672fe28ab021e6a096"
 dependencies = [
- "cfg-if",
+ "quote",
+ "syn 1.0.109",
 ]
 
 [[package]]
 name = "dyn-clone"
-version = "1.0.13"
+version = "1.0.17"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "bbfc4744c1b8f2a09adc0e55242f60b1af195d88596bd8700be74418c056c555"
+checksum = "0d6ef0072f8a535281e4876be788938b528e9a1d43900b82c2569af7da799125"
 
 [[package]]
 name = "either"
-version = "1.9.0"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a26ae43d7bcc3b814de94796a5e736d4029efb0ee900c12e2d54c993ad1a1e07"
-
-[[package]]
-name = "enum_dispatch"
-version = "0.3.12"
+version = "1.10.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8f33313078bb8d4d05a2733a94ac4c2d8a0df9a2b84424ebf4f33bfc224a890e"
-dependencies = [
- "once_cell",
- "proc-macro2",
- "quote",
- "syn 2.0.32",
-]
+checksum = "11157ac094ffbdde99aa67b23417ebdd801842852b500e395a45a9c0aac03e4a"
 
 [[package]]
 name = "env_logger"
-version = "0.10.0"
+version = "0.10.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "85cdab6a89accf66733ad5a1693a4dcced6aeff64602b634530dd73c1f3ee9f0"
+checksum = "4cd405aab171cb85d6735e5c8d9db038c17d3ca007a4d2c25f337935c3d90580"
 dependencies = [
  "humantime",
  "is-terminal",
  "log",
  "regex",
  "termcolor",
 ]
 
 [[package]]
-name = "equivalent"
-version = "1.0.1"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5443807d6dff69373d433ab9ef5378ad8df50ca6298caf15de6e52e24aaf54d5"
-
-[[package]]
-name = "errno"
-version = "0.3.3"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "136526188508e25c6fef639d7927dfb3e0e3084488bf202267829cf7fc23dbdd"
-dependencies = [
- "errno-dragonfly",
- "libc",
- "windows-sys 0.48.0",
-]
-
-[[package]]
-name = "errno-dragonfly"
-version = "0.1.2"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "aa68f1b12764fab894d2755d2518754e71b4fd80ecfb822714a1206c2aab39bf"
-dependencies = [
- "cc",
- "libc",
-]
-
-[[package]]
-name = "eyre"
-version = "0.4.3"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e9e412cbea04ea7af520b2f4d4ac1677ce546027a7237d8a40b494e34e1e0e31"
-dependencies = [
- "indenter",
-]
-
-[[package]]
-name = "f128"
-version = "0.2.2"
-source = "git+https://github.com/benruijl/f128#8fa3132068b4ad2b9833016eaa4cfa8968499e9b"
-dependencies = [
- "cc",
- "libc",
- "num-traits",
-]
-
-[[package]]
-name = "gammalooprs"
-version = "0.0.1"
-dependencies = [
- "ahash",
- "clap",
- "color-eyre",
- "colored",
- "enum_dispatch",
- "env_logger",
- "eyre",
- "f128",
- "git-version",
- "hyperdual",
- "itertools",
- "libc",
- "log",
- "lorentz_vector",
- "num",
- "num-traits",
- "pyo3",
- "pyo3-build-config",
- "pyo3-log",
- "rand",
- "rayon",
- "serde",
- "serde_yaml",
- "smallvec",
- "smartstring",
- "statrs",
- "symbolica",
- "tabled",
- "vectorize",
- "yaml-rust",
-]
-
-[[package]]
 name = "getrandom"
-version = "0.2.10"
+version = "0.2.12"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "be4136b2a15dd319360be1c07d9933517ccf0be8f16bf62a3bee4f0d618df427"
+checksum = "190092ea657667030ac6a35e305e62fc4dd69fd98ac98631e5d3a2b1575a12b5"
 dependencies = [
  "cfg-if",
  "libc",
  "wasi",
 ]
 
 [[package]]
-name = "gimli"
-version = "0.28.0"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "6fb8d784f27acf97159b40fc4db5ecd8aa23b9ad5ef69cdd136d3bc80665f0c0"
-
-[[package]]
-name = "git-version"
-version = "0.3.5"
+name = "ghost"
+version = "0.1.17"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f6b0decc02f4636b9ccad390dcbe77b722a77efedfa393caf8379a51d5c61899"
+checksum = "b0e085ded9f1267c32176b40921b9754c474f7dd96f7e808d4a982e48aa1e854"
 dependencies = [
- "git-version-macro",
- "proc-macro-hack",
+ "proc-macro2",
+ "quote",
+ "syn 2.0.57",
 ]
 
 [[package]]
-name = "git-version-macro"
-version = "0.3.5"
+name = "gimli"
+version = "0.28.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "fe69f1cbdb6e28af2bac214e943b99ce8a0a06b447d15d3e61161b0423139f3f"
-dependencies = [
- "proc-macro-hack",
- "proc-macro2",
- "quote",
- "syn 1.0.109",
-]
+checksum = "4271d37baee1b8c7e4b708028c57d816cf9d2434acb33a549475f78c181f6253"
 
 [[package]]
 name = "gmp-mpfr-sys"
-version = "1.6.1"
+version = "1.6.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "19c5c67d8c29fe87e3266e691dd60948e6e4df4496c53355ef3551142945721b"
+checksum = "362a6cc3cbe9f41aebe49c03b91aee8fa8fc69d32fb90533f6ed965a882e08e3"
 dependencies = [
  "libc",
- "windows-sys 0.42.0",
+ "windows-sys 0.52.0",
 ]
 
 [[package]]
-name = "hashbrown"
-version = "0.14.0"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "2c6201b9ff9fd90a5a3bac2e56a830d0caa509576f0e503818ee82c181b3437a"
-
-[[package]]
-name = "hermit-abi"
-version = "0.1.19"
+name = "heck"
+version = "0.4.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "62b467343b94ba476dcb2500d242dadbb39557df889310ac77c5d99100aaac33"
-dependencies = [
- "libc",
-]
+checksum = "95505c38b4572b2d910cecb0281560f54b440a19336cbbcb27bf6ce6adc6f5a8"
 
 [[package]]
 name = "hermit-abi"
-version = "0.3.2"
+version = "0.3.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "443144c8cdadd93ebf52ddb4056d257f5b52c04d3c804e657d19eb73fc33668b"
+checksum = "d231dfb89cfffdbc30e7fc41579ed6066ad03abda9e567ccafae602b97ec5024"
 
 [[package]]
 name = "humantime"
 version = "2.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9a3a5bfb195931eeb336b2a7b4d761daec841b97f947d34394601737a7bba5e4"
 
 [[package]]
-name = "hyperdual"
-version = "0.5.0"
-source = "git+https://gitlab.com/benruijl/hyperdual#57ec74523111f89c0ec799375c406a444ced0112"
-dependencies = [
- "nalgebra",
- "num-traits",
-]
-
-[[package]]
-name = "indenter"
-version = "0.3.3"
+name = "indoc"
+version = "2.0.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ce23b50ad8242c51a442f3ff322d56b02f08852c77e4c0b4d3fd684abc89c683"
+checksum = "b248f5224d1d606005e02c97f5aa4e88eeb230488bcc03bc9ca4d7991399f2b5"
 
 [[package]]
-name = "indexmap"
-version = "2.0.0"
+name = "inventory"
+version = "0.2.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d5477fe2230a79769d8dc68e0eabf5437907c0457a5614a9e8dddb67f65eb65d"
+checksum = "84344c6e0b90a9e2b6f3f9abe5cc74402684e348df7b32adca28747e0cef091a"
 dependencies = [
- "equivalent",
- "hashbrown",
+ "ctor",
+ "ghost",
 ]
 
 [[package]]
-name = "indoc"
-version = "1.0.9"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "bfa799dd5ed20a7e349f3b4639aa80d74549c81716d9ec4f994c9b5815598306"
-
-[[package]]
 name = "inventory"
-version = "0.3.12"
+version = "0.3.15"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e1be380c410bf0595e94992a648ea89db4dd3f3354ba54af206fd2a68cf5ac8e"
+checksum = "f958d3d68f4167080a18141e10381e7634563984a537f2a49a30fd8e53ac5767"
 
 [[package]]
 name = "is-terminal"
-version = "0.4.9"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "cb0889898416213fab133e1d33a0e5858a48177452750691bde3666d0fdbaf8b"
-dependencies = [
- "hermit-abi 0.3.2",
- "rustix",
- "windows-sys 0.48.0",
-]
-
-[[package]]
-name = "itertools"
-version = "0.8.2"
+version = "0.4.12"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f56a2d0bc861f9165be4eb3442afd3c236d8a98afd426f65d92324ae1091a484"
+checksum = "f23ff5ef2b80d608d61efee834934d862cd92461afc0560dedf493e4c033738b"
 dependencies = [
- "either",
+ "hermit-abi",
+ "libc",
+ "windows-sys 0.52.0",
 ]
 
 [[package]]
-name = "itoa"
-version = "1.0.9"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "af150ab688ff2122fcef229be89cb50dd66af9e01a4ff320cc137eecc9bacc38"
-
-[[package]]
 name = "lazy_static"
 version = "1.4.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e2abad23fbc42b3700f2f279844dc832adb2b2eb069b2df918f455c4e18cc646"
 
 [[package]]
 name = "libc"
-version = "0.2.148"
+version = "0.2.153"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9cdc71e17332e86d2e1d38c1f99edcb6288ee11b815fb1a4b049eaa2114d369b"
+checksum = "9c198f91728a82281a64e1f4f9eeb25d82cb32a5de251c6bd1b5154d63a8e7bd"
 
 [[package]]
 name = "libm"
-version = "0.2.7"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f7012b1bbb0719e1097c47611d3898568c546d597c2e74d66f6087edd5233ff4"
-
-[[package]]
-name = "linked-hash-map"
-version = "0.5.6"
+version = "0.2.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "0717cef1bc8b636c6e1c1bbdefc09e6322da8a9321966e8928ef80d20f7f770f"
+checksum = "4ec2a862134d2a7d32d7983ddcdd1c4923530833c9f2ea1a44fc5fa473989058"
 
 [[package]]
-name = "linux-raw-sys"
-version = "0.4.7"
+name = "link-cplusplus"
+version = "1.0.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "1a9bad9f94746442c783ca431b22403b519cd7fbeed0533fdd6328b2f2212128"
+checksum = "9d240c6f7e1ba3a28b0249f774e6a9dd0175054b52dfbb61b16eb8505c3785c9"
+dependencies = [
+ "cc",
+]
 
 [[package]]
 name = "lock_api"
-version = "0.4.10"
+version = "0.4.11"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c1cc9717a20b1bb222f333e6a92fd32f7d8a18ddc5a3191a11af45dcbf4dcd16"
+checksum = "3c168f8615b12bc01f9c17e2eb0cc07dcae1940121185446edc3744920e8ef45"
 dependencies = [
  "autocfg",
  "scopeguard",
 ]
 
 [[package]]
 name = "log"
-version = "0.4.20"
+version = "0.4.21"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b5e6163cb8c49088c2c36f57875e58ccd8c87c7427f7fbd50ea6710b2f3f2e8f"
-
-[[package]]
-name = "lorentz_vector"
-version = "0.1.4"
-source = "git+https://github.com/benruijl/lorentz_vector?branch=hyperdual#c2d8d6f527455ec1c380ae39d69f395d710dd1d4"
-dependencies = [
- "f128",
- "hyperdual",
- "num",
- "serde",
-]
+checksum = "90ed8c1e510134f979dbc4f070f87d4313098b704861a105fe34231c70a3901c"
 
 [[package]]
-name = "matrixmultiply"
-version = "0.3.7"
+name = "matchers"
+version = "0.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "090126dc04f95dc0d1c1c91f61bdd474b3930ca064c1edc8a849da2c6cbe1e77"
+checksum = "8263075bb86c5a1b1427b5ae862e8889656f126e9f77c484496e8b47cf5c5558"
 dependencies = [
- "autocfg",
- "rawpointer",
+ "regex-automata 0.1.10",
 ]
 
 [[package]]
 name = "memchr"
-version = "2.6.3"
+version = "2.7.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8f232d6ef707e1956a43342693d2a31e72989554d58299d7a88738cc95b0d35c"
+checksum = "6c8640c5d730cb13ebd907d8d04b52f55ac9a2eec55b440c8892f40d56c76c1d"
 
 [[package]]
 name = "memoffset"
-version = "0.9.0"
+version = "0.9.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5a634b1c61a95585bd15607c6ab0c4e5b226e695ff2800ba0cdccddf208c406c"
+checksum = "488016bfae457b036d996092f6cb448677611ce4449e970ceaf42695203f218a"
 dependencies = [
  "autocfg",
 ]
 
 [[package]]
 name = "miniz_oxide"
-version = "0.7.1"
+version = "0.7.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e7810e0be55b428ada41041c41f32c9f1a42817901b4ccf45fa3d4b6561e74c7"
+checksum = "9d811f3e15f28568be3407c8e7fdb6514c1cda3cb30683f15b6a1a1dc4ea14a7"
 dependencies = [
  "adler",
 ]
 
 [[package]]
-name = "nalgebra"
-version = "0.29.0"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d506eb7e08d6329505faa8a3a00a5dcc6de9f76e0c77e4b75763ae3c770831ff"
-dependencies = [
- "approx",
- "matrixmultiply",
- "nalgebra-macros",
- "num-complex 0.4.4",
- "num-rational 0.4.1",
- "num-traits",
- "rand",
- "rand_distr",
- "simba",
- "typenum",
-]
-
-[[package]]
-name = "nalgebra-macros"
-version = "0.1.0"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "01fcc0b8149b4632adc89ac3b7b31a12fb6099a0317a4eb2ebff574ef7de7218"
-dependencies = [
- "proc-macro2",
- "quote",
- "syn 1.0.109",
-]
-
-[[package]]
-name = "num"
-version = "0.3.1"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8b7a8e9be5e039e2ff869df49155f1c06bd01ade2117ec783e56ab0932b67a8f"
-dependencies = [
- "num-bigint",
- "num-complex 0.3.1",
- "num-integer",
- "num-iter",
- "num-rational 0.3.2",
- "num-traits",
-]
-
-[[package]]
-name = "num-bigint"
-version = "0.3.3"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5f6f7833f2cbf2360a6cfd58cd41a53aa7a90bd4c202f5b1c7dd2ed73c57b2c3"
-dependencies = [
- "autocfg",
- "num-integer",
- "num-traits",
-]
-
-[[package]]
-name = "num-complex"
-version = "0.3.1"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "747d632c0c558b87dbabbe6a82f3b4ae03720d0646ac5b7b4dae89394be5f2c5"
-dependencies = [
- "num-traits",
-]
-
-[[package]]
-name = "num-complex"
-version = "0.4.4"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "1ba157ca0885411de85d6ca030ba7e2a83a28636056c7c699b07c8b6f7383214"
-dependencies = [
- "num-traits",
-]
-
-[[package]]
-name = "num-integer"
-version = "0.1.45"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "225d3389fb3509a24c93f5c29eb6bde2586b98d9f016636dff58d7c6f7569cd9"
-dependencies = [
- "autocfg",
- "num-traits",
-]
-
-[[package]]
-name = "num-iter"
-version = "0.1.43"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7d03e6c028c5dc5cac6e2dec0efda81fc887605bb3d884578bb6d6bf7514e252"
-dependencies = [
- "autocfg",
- "num-integer",
- "num-traits",
-]
-
-[[package]]
-name = "num-rational"
-version = "0.3.2"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "12ac428b1cb17fce6f731001d307d351ec70a6d202fc2e60f7d4c5e42d8f4f07"
-dependencies = [
- "autocfg",
- "num-bigint",
- "num-integer",
- "num-traits",
-]
-
-[[package]]
-name = "num-rational"
-version = "0.4.1"
+name = "nu-ansi-term"
+version = "0.46.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "0638a1c9d0a3c0914158145bc76cff373a75a627e6ecbfb71cbe6f453a5a19b0"
+checksum = "77a8165726e8236064dbb45459242600304b42a5ea24ee2948e18e023bf7ba84"
 dependencies = [
- "autocfg",
- "num-integer",
- "num-traits",
+ "overload",
+ "winapi",
 ]
 
 [[package]]
 name = "num-traits"
-version = "0.2.16"
+version = "0.2.18"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f30b0abd723be7e2ffca1272140fac1a2f084c77ec3e123c192b66af1ee9e6c2"
+checksum = "da0df0e5185db44f69b44f26786fe401b6c293d1907744beaa7fa62b2e5a517a"
 dependencies = [
  "autocfg",
- "libm",
-]
-
-[[package]]
-name = "num_cpus"
-version = "1.16.0"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "4161fcb6d602d4d2081af7c3a45852d875a03dd337a6bfdd6e06407b61342a43"
-dependencies = [
- "hermit-abi 0.3.2",
- "libc",
 ]
 
 [[package]]
 name = "object"
-version = "0.32.1"
+version = "0.32.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9cf5f9dd3933bd50a9e1f149ec995f39ae2c496d31fd772c1fd45ebc27e902b0"
+checksum = "a6a622008b6e321afc04970976f62ee297fdbaa6f95318ca343e3eebb9648441"
 dependencies = [
  "memchr",
 ]
 
 [[package]]
 name = "once_cell"
-version = "1.18.0"
+version = "1.19.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "dd8b5dd2ae5ed71462c540258bedcb51965123ad7e7ccf4b9a8cafaa4a63576d"
+checksum = "3fdb12b2476b595f9358c5161aa467c2438859caa136dec86c26fdd2efe17b92"
 
 [[package]]
-name = "papergrid"
-version = "0.4.0"
+name = "ordered-float"
+version = "3.9.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "608b6444acf7f5ea39e8bd06dd6037e34a4b5ddfb29ae840edad49ea798e9e79"
+checksum = "f1e1c390732d15f1d48471625cd92d154e66db2c56645e29a9cd26f4699f72dc"
 dependencies = [
- "unicode-width",
+ "num-traits",
 ]
 
 [[package]]
+name = "overload"
+version = "0.1.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "b15813163c1d831bf4a13c3610c05c0d03b39feb07f7e09fa234dac9b15aaf39"
+
+[[package]]
 name = "parking_lot"
 version = "0.12.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "3742b2c103b9f06bc9fff0a37ff4912935851bee6d36f3c02bcc755bcfec228f"
 dependencies = [
  "lock_api",
  "parking_lot_core",
 ]
 
 [[package]]
 name = "parking_lot_core"
-version = "0.9.8"
+version = "0.9.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "93f00c865fe7cabf650081affecd3871070f26767e7b2070a3ffae14c654b447"
+checksum = "4c42a9226546d68acdd9c0a280d17ce19bfe27a46bf68784e4066115788d008e"
 dependencies = [
  "cfg-if",
  "libc",
  "redox_syscall",
  "smallvec",
- "windows-targets",
+ "windows-targets 0.48.5",
 ]
 
 [[package]]
-name = "paste"
-version = "1.0.14"
+name = "pin-project-lite"
+version = "0.2.14"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "de3145af08024dea9fa9914f381a17b8fc6034dfb00f3a84013f7ff43f29ed4c"
+checksum = "bda66fc9667c18cb2758a2ac84d1167245054bcf85d5d1aaa6923f45801bdd02"
 
 [[package]]
-name = "pin-project-lite"
-version = "0.2.13"
+name = "portable-atomic"
+version = "1.6.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8afb450f006bf6385ca15ef45d71d2288452bc3683ce2e2cacc0d18e4be60b58"
+checksum = "7170ef9988bc169ba16dd36a7fa041e5c4cbeb6a35b76d4c03daded371eae7c0"
 
 [[package]]
 name = "ppv-lite86"
 version = "0.2.17"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "5b40af805b3121feab8a3c29f04d8ad262fa8e0561883e7653e024ae4479e6de"
 
 [[package]]
-name = "proc-macro-hack"
-version = "0.5.20+deprecated"
+name = "proc-macro2"
+version = "1.0.79"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "dc375e1527247fe1a97d8b7156678dfe7c1af2fc075c9a4db3690ecd2a148068"
+checksum = "e835ff2298f5721608eb1a980ecaee1aef2c132bf95ecc026a11b7bf3c01c02e"
+dependencies = [
+ "unicode-ident",
+]
 
 [[package]]
-name = "proc-macro2"
-version = "1.0.66"
+name = "process_path"
+version = "0.1.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "18fb31db3f9bddb2ea821cde30a9f70117e3f119938b5ee630b7403aa6e2ead9"
+checksum = "f676f11eb0b3e2ea0fbaee218fa6b806689e2297b8c8adc5bf73df465c4f6171"
 dependencies = [
- "unicode-ident",
+ "libc",
+ "winapi",
 ]
 
 [[package]]
 name = "pyo3"
-version = "0.19.2"
+version = "0.20.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e681a6cfdc4adcc93b4d3cf993749a4552018ee0a9b65fc0ccfad74352c72a38"
+checksum = "53bdbb96d49157e65d45cc287af5f32ffadd5f4761438b527b055fb0d4bb8233"
 dependencies = [
  "cfg-if",
  "indoc",
- "inventory",
+ "inventory 0.3.15",
  "libc",
  "memoffset",
  "parking_lot",
+ "portable-atomic",
  "pyo3-build-config",
  "pyo3-ffi",
  "pyo3-macros",
  "unindent",
 ]
 
 [[package]]
 name = "pyo3-build-config"
-version = "0.19.2"
+version = "0.20.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "076c73d0bc438f7a4ef6fdd0c3bb4732149136abd952b110ac93e4edb13a6ba5"
+checksum = "deaa5745de3f5231ce10517a1f5dd97d53e5a2fd77aa6b5842292085831d48d7"
 dependencies = [
  "once_cell",
  "target-lexicon",
 ]
 
 [[package]]
 name = "pyo3-ffi"
-version = "0.19.2"
+version = "0.20.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e53cee42e77ebe256066ba8aa77eff722b3bb91f3419177cf4cd0f304d3284d9"
+checksum = "62b42531d03e08d4ef1f6e85a2ed422eb678b8cd62b762e53891c05faf0d4afa"
 dependencies = [
  "libc",
  "pyo3-build-config",
 ]
 
 [[package]]
-name = "pyo3-log"
-version = "0.8.3"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f47b0777feb17f61eea78667d61103758b243a871edc09a7786500a50467b605"
-dependencies = [
- "arc-swap",
- "log",
- "pyo3",
-]
-
-[[package]]
 name = "pyo3-macros"
-version = "0.19.2"
+version = "0.20.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "dfeb4c99597e136528c6dd7d5e3de5434d1ceaf487436a3f03b2d56b6fc9efd1"
+checksum = "7305c720fa01b8055ec95e484a6eca7a83c841267f0dd5280f0c8b8551d2c158"
 dependencies = [
  "proc-macro2",
  "pyo3-macros-backend",
  "quote",
- "syn 1.0.109",
+ "syn 2.0.57",
 ]
 
 [[package]]
 name = "pyo3-macros-backend"
-version = "0.19.2"
+version = "0.20.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "947dc12175c254889edc0c02e399476c2f652b4b9ebd123aa655c224de259536"
+checksum = "7c7e9b68bb9c3149c5b0cade5d07f953d6d125eb4337723c4ccdb665f1f96185"
 dependencies = [
+ "heck",
  "proc-macro2",
+ "pyo3-build-config",
  "quote",
- "syn 1.0.109",
+ "syn 2.0.57",
 ]
 
 [[package]]
 name = "quote"
-version = "1.0.33"
+version = "1.0.35"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5267fca4496028628a95160fc423a33e8b2e6af8a5302579e322e4b520293cae"
+checksum = "291ec9ab5efd934aaf503a6466c5d5251535d108ee747472c3977cc5acc868ef"
 dependencies = [
  "proc-macro2",
 ]
 
 [[package]]
 name = "rand"
 version = "0.8.5"
@@ -921,126 +577,134 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "ec0be4795e2f6a28069bec0b5ff3e2ac9bafc99e6a9a7dc3547996c5c816922c"
 dependencies = [
  "getrandom",
 ]
 
 [[package]]
-name = "rand_distr"
-version = "0.4.3"
+name = "rand_xoshiro"
+version = "0.6.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "32cb0b9bc82b0a0876c2dd994a7e7a2683d3e7390ca40e6886785ef0c7e3ee31"
+checksum = "6f97cdb2a36ed4183de61b2f824cc45c9f1037f28afe0a322e9fff4c108b5aaa"
 dependencies = [
- "num-traits",
- "rand",
+ "rand_core",
 ]
 
 [[package]]
-name = "rawpointer"
-version = "0.2.1"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "60a357793950651c4ed0f3f52338f53b2f809f32d83a07f72909fa13e4c6c1e3"
-
-[[package]]
 name = "rayon"
-version = "1.7.0"
+version = "1.10.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "1d2df5196e37bcc87abebc0053e20787d73847bb33134a69841207dd0a47f03b"
+checksum = "b418a60154510ca1a002a752ca9714984e21e4241e804d32555251faf8b78ffa"
 dependencies = [
  "either",
  "rayon-core",
 ]
 
 [[package]]
 name = "rayon-core"
-version = "1.11.0"
+version = "1.12.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "4b8f95bd6966f5c87776639160a66bd8ab9895d9d4ab01ddba9fc60661aebe8d"
+checksum = "1465873a3dfdaa8ae7cb14b4383657caab0b3e8a0aa9ae8e04b044854c8dfce2"
 dependencies = [
- "crossbeam-channel",
  "crossbeam-deque",
  "crossbeam-utils",
- "num_cpus",
 ]
 
 [[package]]
 name = "redox_syscall"
-version = "0.3.5"
+version = "0.4.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "567664f262709473930a4bf9e51bf2ebf3348f2e748ccc50dea20646858f8f29"
+checksum = "4722d768eff46b75989dd134e5c353f0d6296e5aaa3132e776cbdb56be7731aa"
 dependencies = [
- "bitflags 1.3.2",
+ "bitflags",
+]
+
+[[package]]
+name = "ref-cast"
+version = "1.0.22"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "c4846d4c50d1721b1a3bef8af76924eef20d5e723647333798c1b519b3a9473f"
+dependencies = [
+ "ref-cast-impl",
+]
+
+[[package]]
+name = "ref-cast-impl"
+version = "1.0.22"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "5fddb4f8d99b0a2ebafc65a87a69a7b9875e4b1ae1f00db265d300ef7f28bccc"
+dependencies = [
+ "proc-macro2",
+ "quote",
+ "syn 2.0.57",
 ]
 
 [[package]]
 name = "regex"
-version = "1.9.5"
+version = "1.10.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "697061221ea1b4a94a624f67d0ae2bfe4e22b8a17b6a192afb11046542cc8c47"
+checksum = "c117dbdfde9c8308975b6a18d71f3f385c89461f7b3fb054288ecf2a2058ba4c"
 dependencies = [
  "aho-corasick",
  "memchr",
- "regex-automata",
- "regex-syntax",
+ "regex-automata 0.4.6",
+ "regex-syntax 0.8.3",
 ]
 
 [[package]]
 name = "regex-automata"
-version = "0.3.8"
+version = "0.1.10"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c2f401f4955220693b56f8ec66ee9c78abffd8d1c4f23dc41a23839eb88f0795"
+checksum = "6c230d73fb8d8c1b9c0b3135c5142a8acee3a0558fb8db5cf1cb65f8d7862132"
+dependencies = [
+ "regex-syntax 0.6.29",
+]
+
+[[package]]
+name = "regex-automata"
+version = "0.4.6"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "86b83b8b9847f9bf95ef68afb0b8e6cdb80f498442f5179a29fad448fcc1eaea"
 dependencies = [
  "aho-corasick",
  "memchr",
- "regex-syntax",
+ "regex-syntax 0.8.3",
 ]
 
 [[package]]
 name = "regex-syntax"
-version = "0.7.5"
+version = "0.6.29"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "dbb5fb1acd8a1a18b3dd5be62d25485eb770e05afb408a9627d14d451bae12da"
+checksum = "f162c6dd7b008981e4d40210aca20b4bd0f9b60ca9271061b07f78537722f2e1"
+
+[[package]]
+name = "regex-syntax"
+version = "0.8.3"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "adad44e29e4c806119491a7f06f03de4d1af22c3a680dd47f1e6e179439d1f56"
 
 [[package]]
 name = "rug"
-version = "1.22.0"
+version = "1.24.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5a118f8296241f6952511e8f9ab5b8a759c0d9ed902159b0aeed82d902e84ca6"
+checksum = "a8df4099c6fa90a1a7f5ddc0c7fba50991080fa2084d5a78808a5a3cab406bb9"
 dependencies = [
  "az",
  "gmp-mpfr-sys",
  "libc",
+ "libm",
 ]
 
 [[package]]
 name = "rustc-demangle"
 version = "0.1.23"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d626bb9dae77e28219937af045c257c28bfd3f69333c512553507f5f9798cb76"
 
 [[package]]
-name = "rustix"
-version = "0.38.13"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d7db8590df6dfcd144d22afd1b83b36c21a18d7cbc1dc4bb5295a8712e9eb662"
-dependencies = [
- "bitflags 2.4.0",
- "errno",
- "libc",
- "linux-raw-sys",
- "windows-sys 0.48.0",
-]
-
-[[package]]
-name = "ryu"
-version = "1.0.15"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "1ad4cc8da4ef723ed60bced201181d83791ad433213d8c24efffda1eec85d741"
-
-[[package]]
 name = "safe_arch"
 version = "0.7.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "f398075ce1e6a179b46f51bd88d0598b92b00d3551f1a2d4ac49e771b56ac354"
 dependencies = [
  "bytemuck",
 ]
@@ -1048,122 +712,98 @@
 [[package]]
 name = "scopeguard"
 version = "1.2.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "94143f37725109f92c262ed2cf5e59bce7498c01bcc1502d7b9afe439a4e9f49"
 
 [[package]]
+name = "self_cell"
+version = "1.0.3"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "58bf37232d3bb9a2c4e641ca2a11d83b5062066f88df7fed36c28772046d65ba"
+
+[[package]]
 name = "serde"
-version = "1.0.188"
+version = "1.0.197"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "cf9e0fcba69a370eed61bcf2b728575f726b50b55cba78064753d708ddc7549e"
+checksum = "3fb1c873e1b9b056a4dc4c0c198b24c3ffa059243875552b2bd0933b1aee4ce2"
 dependencies = [
  "serde_derive",
 ]
 
 [[package]]
 name = "serde_derive"
-version = "1.0.188"
+version = "1.0.197"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "4eca7ac642d82aa35b60049a6eccb4be6be75e599bd2e9adb5f875a737654af2"
+checksum = "7eb0b34b42edc17f6b7cac84a52a1c5f0e1bb2227e997ca9011ea3dd34e8610b"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.32",
-]
-
-[[package]]
-name = "serde_yaml"
-version = "0.9.25"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "1a49e178e4452f45cb61d0cd8cebc1b0fafd3e41929e996cef79aa3aca91f574"
-dependencies = [
- "indexmap",
- "itoa",
- "ryu",
- "serde",
- "unsafe-libyaml",
+ "syn 2.0.57",
 ]
 
 [[package]]
-name = "simba"
-version = "0.6.0"
+name = "sharded-slab"
+version = "0.1.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f0b7840f121a46d63066ee7a99fc81dcabbc6105e437cae43528cea199b5a05f"
+checksum = "f40ca3c46823713e0d4209592e8d6e826aa57e928f09752619fc696c499637f6"
 dependencies = [
- "approx",
- "num-complex 0.4.4",
- "num-traits",
- "paste",
- "wide",
+ "lazy_static",
 ]
 
 [[package]]
 name = "smallvec"
-version = "1.11.0"
+version = "1.13.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "62bb4feee49fdd9f707ef802e22365a35de4b7b299de4763d44bfea899442ff9"
+checksum = "3c5e1a9a646d36c3599cd173a41282daf47c44583ad367b8e6837255952e5c67"
 
 [[package]]
 name = "smartstring"
 version = "1.0.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "3fb72c633efbaa2dd666986505016c32c3044395ceaf881518399d2f4127ee29"
 dependencies = [
  "autocfg",
- "serde",
  "static_assertions",
  "version_check",
 ]
 
 [[package]]
 name = "static_assertions"
 version = "1.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "a2eb9349b6444b326872e140eb1cf5e7c522154d69e7a0ffb0fb81c06b37543f"
 
 [[package]]
-name = "statrs"
-version = "0.16.0"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "2d08e5e1748192713cc281da8b16924fb46be7b0c2431854eadc785823e5696e"
-dependencies = [
- "approx",
- "lazy_static",
- "nalgebra",
- "num-traits",
- "rand",
-]
-
-[[package]]
-name = "strsim"
-version = "0.8.0"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8ea5119cdb4c55b55d432abb513a0429384878c15dde60cc77b1c99de1a95a6a"
-
-[[package]]
 name = "symbolica"
-version = "0.1.0"
-source = "git+https://github.com/alphal00p/symbolica#0263c98ee48e06d61307f47f15517ac215488628"
+version = "0.3.0"
 dependencies = [
  "ahash",
+ "append-only-vec",
+ "bincode",
  "byteorder",
  "bytes",
  "colored",
  "dyn-clone",
  "once_cell",
- "pyo3-build-config",
+ "pyo3",
  "rand",
+ "rand_xoshiro",
  "rayon",
  "rug",
+ "self_cell",
+ "serde",
  "smallvec",
  "smartstring",
+ "tikv-jemallocator",
  "tinyjson",
  "tracing",
+ "tracing-subscriber",
  "wide",
+ "wolfram-library-link",
 ]
 
 [[package]]
 name = "syn"
 version = "1.0.109"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "72b64191b275b66ffe2469e8af2c1cfe3bafa67b529ead792a6d0160888b4237"
@@ -1171,150 +811,152 @@
  "proc-macro2",
  "quote",
  "unicode-ident",
 ]
 
 [[package]]
 name = "syn"
-version = "2.0.32"
+version = "2.0.57"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "239814284fd6f1a4ffe4ca893952cdd93c224b6a1571c9a9eadd670295c0c9e2"
+checksum = "11a6ae1e52eb25aab8f3fb9fca13be982a373b8f1157ca14b897a825ba4a2d35"
 dependencies = [
  "proc-macro2",
  "quote",
  "unicode-ident",
 ]
 
 [[package]]
-name = "tabled"
-version = "0.7.0"
+name = "target-lexicon"
+version = "0.12.14"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "2407502760ccfd538f2fb1f843dd87b6daf1a17848d57bc5a25617e408ef4c7a"
-dependencies = [
- "papergrid",
- "tabled_derive",
-]
+checksum = "e1fc403891a21bcfb7c37834ba66a547a8f402146eba7265b5a6d88059c9ff2f"
 
 [[package]]
-name = "tabled_derive"
-version = "0.3.0"
+name = "termcolor"
+version = "1.4.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "278ea3921cee8c5a69e0542998a089f7a14fa43c9c4e4f9951295da89bd0c943"
+checksum = "06794f8f6c5c898b3275aebefa6b8a1cb24cd2c6c79397ab15774837a0bc5755"
 dependencies = [
- "proc-macro2",
- "quote",
- "syn 1.0.109",
+ "winapi-util",
 ]
 
 [[package]]
-name = "target-lexicon"
-version = "0.12.11"
+name = "thread_local"
+version = "1.1.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9d0e916b1148c8e263850e1ebcbd046f333e0683c724876bb0da63ea4373dc8a"
+checksum = "8b9ef9bad013ada3808854ceac7b46812a6465ba368859a37e2100283d2d719c"
+dependencies = [
+ "cfg-if",
+ "once_cell",
+]
 
 [[package]]
-name = "termcolor"
-version = "1.2.0"
+name = "tikv-jemalloc-sys"
+version = "0.5.4+5.3.0-patched"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "be55cf8942feac5c765c2c993422806843c9a9a45d4d5c407ad6dd2ea95eb9b6"
+checksum = "9402443cb8fd499b6f327e40565234ff34dbda27460c5b47db0db77443dd85d1"
 dependencies = [
- "winapi-util",
+ "cc",
+ "libc",
 ]
 
 [[package]]
-name = "textwrap"
-version = "0.11.0"
+name = "tikv-jemallocator"
+version = "0.5.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d326610f408c7a4eb6f51c37c330e496b08506c9457c9d34287ecc38809fb060"
+checksum = "965fe0c26be5c56c94e38ba547249074803efd52adfb66de62107d95aab3eaca"
 dependencies = [
- "unicode-width",
+ "libc",
+ "tikv-jemalloc-sys",
 ]
 
 [[package]]
 name = "tinyjson"
 version = "2.5.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9ab95735ea2c8fd51154d01e39cf13912a78071c2d89abc49a7ef102a7dd725a"
 
 [[package]]
 name = "tracing"
-version = "0.1.37"
+version = "0.1.40"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8ce8c33a8d48bd45d624a6e523445fd21ec13d3653cd51f681abf67418f54eb8"
+checksum = "c3523ab5a71916ccf420eebdf5521fcef02141234bbc0b8a49f2fdc4544364ef"
 dependencies = [
- "cfg-if",
  "pin-project-lite",
  "tracing-attributes",
  "tracing-core",
 ]
 
 [[package]]
 name = "tracing-attributes"
-version = "0.1.26"
+version = "0.1.27"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5f4f31f56159e98206da9efd823404b79b6ef3143b4a7ab76e67b1751b25a4ab"
+checksum = "34704c8d6ebcbc939824180af020566b01a7c01f80641264eba0999f6c2b6be7"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.32",
+ "syn 2.0.57",
 ]
 
 [[package]]
 name = "tracing-core"
-version = "0.1.31"
+version = "0.1.32"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "0955b8137a1df6f1a2e9a37d8a6656291ff0297c1a97c24e0d8425fe2312f79a"
+checksum = "c06d3da6113f116aaee68e4d601191614c9053067f9ab7f6edbcb161237daa54"
 dependencies = [
  "once_cell",
+ "valuable",
 ]
 
 [[package]]
-name = "typenum"
-version = "1.16.0"
+name = "tracing-log"
+version = "0.2.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "497961ef93d974e23eb6f433eb5fe1b7930b659f06d12dec6fc44a8f554c0bba"
+checksum = "ee855f1f400bd0e5c02d150ae5de3840039a3f54b025156404e34c23c03f47c3"
+dependencies = [
+ "log",
+ "once_cell",
+ "tracing-core",
+]
 
 [[package]]
-name = "unicode-ident"
-version = "1.0.12"
+name = "tracing-subscriber"
+version = "0.3.18"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "3354b9ac3fae1ff6755cb6db53683adb661634f67557942dea4facebec0fee4b"
+checksum = "ad0f048c97dbd9faa9b7df56362b8ebcaa52adb06b498c050d2f4e32f90a7a8b"
+dependencies = [
+ "matchers",
+ "nu-ansi-term",
+ "once_cell",
+ "regex",
+ "sharded-slab",
+ "smallvec",
+ "thread_local",
+ "tracing",
+ "tracing-core",
+ "tracing-log",
+]
 
 [[package]]
-name = "unicode-width"
-version = "0.1.10"
+name = "unicode-ident"
+version = "1.0.12"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c0edd1e5b14653f783770bce4a4dabb4a5108a5370a5f5d8cfe8710c361f6c8b"
+checksum = "3354b9ac3fae1ff6755cb6db53683adb661634f67557942dea4facebec0fee4b"
 
 [[package]]
 name = "unindent"
-version = "0.1.11"
+version = "0.2.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e1766d682d402817b5ac4490b3c3002d91dfa0d22812f341609f97b08757359c"
+checksum = "c7de7d73e1754487cb58364ee906a499937a0dfabd86bcb980fa99ec8c8fa2ce"
 
 [[package]]
-name = "unsafe-libyaml"
-version = "0.2.9"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f28467d3e1d3c6586d8f25fa243f544f5800fec42d97032474e17222c2b75cfa"
-
-[[package]]
-name = "vec_map"
-version = "0.8.2"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f1bddf1187be692e79c5ffeab891132dfb0f236ed36a43c7ed39f1165ee20191"
-
-[[package]]
-name = "vectorize"
-version = "0.2.0"
+name = "valuable"
+version = "0.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "25e3bbfdfdcc4ea60ce183b1b45c936aacd69fe097ebf137984a32faf80e365b"
-dependencies = [
- "serde",
-]
+checksum = "830b7e5d4d90034032940e4ace0d9a9a057e7a45cd94e6c007832e39edb82f6d"
 
 [[package]]
 name = "version_check"
 version = "0.9.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "49874b5167b65d7193b8aba1567f5c7d93d001cafc34600cee003eda787e483f"
 
@@ -1322,17 +964,17 @@
 name = "wasi"
 version = "0.11.0+wasi-snapshot-preview1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9c8d87e72b64a3b4db28d11ce29237c246188f4f51057d65a7eab63b7987e423"
 
 [[package]]
 name = "wide"
-version = "0.7.11"
+version = "0.7.15"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "aa469ffa65ef7e0ba0f164183697b89b854253fd31aeb92358b7b6155177d62f"
+checksum = "89beec544f246e679fc25490e3f8e08003bc4bf612068f325120dad4cea02c1c"
 dependencies = [
  "bytemuck",
  "safe_arch",
 ]
 
 [[package]]
 name = "winapi"
@@ -1348,49 +990,56 @@
 name = "winapi-i686-pc-windows-gnu"
 version = "0.4.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "ac3b87c63620426dd9b991e5ce0329eff545bccbbb34f3be09ff6fb6ab51b7b6"
 
 [[package]]
 name = "winapi-util"
-version = "0.1.5"
+version = "0.1.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "70ec6ce85bb158151cae5e5c87f95a8e97d2c0c4b001223f33a334e3ce5de178"
+checksum = "f29e6f9198ba0d26b4c9f07dbe6f9ed633e1f3d5b8b414090084349e46a52596"
 dependencies = [
  "winapi",
 ]
 
 [[package]]
 name = "winapi-x86_64-pc-windows-gnu"
 version = "0.4.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "712e227841d057c1ee1cd2fb22fa7e5a5461ae8e48fa2ca79ec42cfc1931183f"
 
 [[package]]
-name = "windows-sys"
-version = "0.42.0"
+name = "windows"
+version = "0.32.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5a3e1820f08b8513f676f7ab6c1f99ff312fb97b553d30ff4dd86f9f15728aa7"
+checksum = "fbedf6db9096bc2364adce0ae0aa636dcd89f3c3f2cd67947062aaf0ca2a10ec"
 dependencies = [
- "windows_aarch64_gnullvm 0.42.2",
- "windows_aarch64_msvc 0.42.2",
- "windows_i686_gnu 0.42.2",
- "windows_i686_msvc 0.42.2",
- "windows_x86_64_gnu 0.42.2",
- "windows_x86_64_gnullvm 0.42.2",
- "windows_x86_64_msvc 0.42.2",
+ "windows_aarch64_msvc 0.32.0",
+ "windows_i686_gnu 0.32.0",
+ "windows_i686_msvc 0.32.0",
+ "windows_x86_64_gnu 0.32.0",
+ "windows_x86_64_msvc 0.32.0",
 ]
 
 [[package]]
 name = "windows-sys"
 version = "0.48.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "677d2418bec65e3338edb076e806bc1ec15693c5d0104683f2efe857f61056a9"
 dependencies = [
- "windows-targets",
+ "windows-targets 0.48.5",
+]
+
+[[package]]
+name = "windows-sys"
+version = "0.52.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "282be5f36a8ce781fad8c8ae18fa3f9beff57ec1b52cb3de0789201425d9a33d"
+dependencies = [
+ "windows-targets 0.52.4",
 ]
 
 [[package]]
 name = "windows-targets"
 version = "0.48.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9a2fa6e2155d7247be68c096456083145c183cbbbc2764150dda45a87197940c"
@@ -1401,98 +1050,237 @@
  "windows_i686_msvc 0.48.5",
  "windows_x86_64_gnu 0.48.5",
  "windows_x86_64_gnullvm 0.48.5",
  "windows_x86_64_msvc 0.48.5",
 ]
 
 [[package]]
-name = "windows_aarch64_gnullvm"
-version = "0.42.2"
+name = "windows-targets"
+version = "0.52.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "597a5118570b68bc08d8d59125332c54f1ba9d9adeedeef5b99b02ba2b0698f8"
+checksum = "7dd37b7e5ab9018759f893a1952c9420d060016fc19a472b4bb20d1bdd694d1b"
+dependencies = [
+ "windows_aarch64_gnullvm 0.52.4",
+ "windows_aarch64_msvc 0.52.4",
+ "windows_i686_gnu 0.52.4",
+ "windows_i686_msvc 0.52.4",
+ "windows_x86_64_gnu 0.52.4",
+ "windows_x86_64_gnullvm 0.52.4",
+ "windows_x86_64_msvc 0.52.4",
+]
 
 [[package]]
 name = "windows_aarch64_gnullvm"
 version = "0.48.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "2b38e32f0abccf9987a4e3079dfb67dcd799fb61361e53e2882c3cbaf0d905d8"
 
 [[package]]
+name = "windows_aarch64_gnullvm"
+version = "0.52.4"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "bcf46cf4c365c6f2d1cc93ce535f2c8b244591df96ceee75d8e83deb70a9cac9"
+
+[[package]]
 name = "windows_aarch64_msvc"
-version = "0.42.2"
+version = "0.32.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e08e8864a60f06ef0d0ff4ba04124db8b0fb3be5776a5cd47641e942e58c4d43"
+checksum = "d8e92753b1c443191654ec532f14c199742964a061be25d77d7a96f09db20bf5"
 
 [[package]]
 name = "windows_aarch64_msvc"
 version = "0.48.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "dc35310971f3b2dbbf3f0690a219f40e2d9afcf64f9ab7cc1be722937c26b4bc"
 
 [[package]]
+name = "windows_aarch64_msvc"
+version = "0.52.4"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "da9f259dd3bcf6990b55bffd094c4f7235817ba4ceebde8e6d11cd0c5633b675"
+
+[[package]]
 name = "windows_i686_gnu"
-version = "0.42.2"
+version = "0.32.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c61d927d8da41da96a81f029489353e68739737d3beca43145c8afec9a31a84f"
+checksum = "6a711c68811799e017b6038e0922cb27a5e2f43a2ddb609fe0b6f3eeda9de615"
 
 [[package]]
 name = "windows_i686_gnu"
 version = "0.48.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "a75915e7def60c94dcef72200b9a8e58e5091744960da64ec734a6c6e9b3743e"
 
 [[package]]
+name = "windows_i686_gnu"
+version = "0.52.4"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "b474d8268f99e0995f25b9f095bc7434632601028cf86590aea5c8a5cb7801d3"
+
+[[package]]
 name = "windows_i686_msvc"
-version = "0.42.2"
+version = "0.32.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "44d840b6ec649f480a41c8d80f9c65108b92d89345dd94027bfe06ac444d1060"
+checksum = "146c11bb1a02615db74680b32a68e2d61f553cc24c4eb5b4ca10311740e44172"
 
 [[package]]
 name = "windows_i686_msvc"
 version = "0.48.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "8f55c233f70c4b27f66c523580f78f1004e8b5a8b659e05a4eb49d4166cca406"
 
 [[package]]
+name = "windows_i686_msvc"
+version = "0.52.4"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "1515e9a29e5bed743cb4415a9ecf5dfca648ce85ee42e15873c3cd8610ff8e02"
+
+[[package]]
 name = "windows_x86_64_gnu"
-version = "0.42.2"
+version = "0.32.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8de912b8b8feb55c064867cf047dda097f92d51efad5b491dfb98f6bbb70cb36"
+checksum = "c912b12f7454c6620635bbff3450962753834be2a594819bd5e945af18ec64bc"
 
 [[package]]
 name = "windows_x86_64_gnu"
 version = "0.48.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "53d40abd2583d23e4718fddf1ebec84dbff8381c07cae67ff7768bbf19c6718e"
 
 [[package]]
-name = "windows_x86_64_gnullvm"
-version = "0.42.2"
+name = "windows_x86_64_gnu"
+version = "0.52.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "26d41b46a36d453748aedef1486d5c7a85db22e56aff34643984ea85514e94a3"
+checksum = "5eee091590e89cc02ad514ffe3ead9eb6b660aedca2183455434b93546371a03"
 
 [[package]]
 name = "windows_x86_64_gnullvm"
 version = "0.48.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "0b7b52767868a23d5bab768e390dc5f5c55825b6d30b86c844ff2dc7414044cc"
 
 [[package]]
+name = "windows_x86_64_gnullvm"
+version = "0.52.4"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "77ca79f2451b49fa9e2af39f0747fe999fcda4f5e241b2898624dca97a1f2177"
+
+[[package]]
 name = "windows_x86_64_msvc"
-version = "0.42.2"
+version = "0.32.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9aec5da331524158c6d1a4ac0ab1541149c0b9505fde06423b02f5ef0106b9f0"
+checksum = "504a2476202769977a040c6364301a3f65d0cc9e3fb08600b2bda150a0488316"
 
 [[package]]
 name = "windows_x86_64_msvc"
 version = "0.48.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "ed94fce61571a4006852b7389a063ab983c02eb1bb37b47f8272ce92d06d9538"
 
 [[package]]
-name = "yaml-rust"
-version = "0.4.5"
+name = "windows_x86_64_msvc"
+version = "0.52.4"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "32b752e52a2da0ddfbdbcc6fceadfeede4c939ed16d13e648833a61dfb611ed8"
+
+[[package]]
+name = "wolfram-app-discovery"
+version = "0.4.8"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "1fcac5bdcf7a95e6981e73b69ba9a9c360cb64d50739e3713236caaa2f026b60"
+dependencies = [
+ "core-foundation",
+ "log",
+ "once_cell",
+ "regex",
+ "windows",
+]
+
+[[package]]
+name = "wolfram-expr"
+version = "0.1.4"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "614f5538290eb531931222ac71322f5b2617cd80243e24d02a1c28cfa172eebd"
+dependencies = [
+ "ordered-float",
+]
+
+[[package]]
+name = "wolfram-library-link"
+version = "0.2.10"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "abf93d7cfb152efab7f896ea3809b2a1dd821af4c00c9b2b7faca8cd1b507e1d"
+dependencies = [
+ "backtrace",
+ "inventory 0.2.3",
+ "once_cell",
+ "process_path",
+ "ref-cast",
+ "static_assertions",
+ "wolfram-expr",
+ "wolfram-library-link-macros",
+ "wolfram-library-link-sys",
+ "wstp",
+]
+
+[[package]]
+name = "wolfram-library-link-macros"
+version = "0.2.10"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "f9da237114db065ed3177d08c51ca767edd0a4c0af31c6eddefb8a062f99ae06"
+dependencies = [
+ "proc-macro2",
+ "quote",
+ "syn 1.0.109",
+]
+
+[[package]]
+name = "wolfram-library-link-sys"
+version = "0.2.10"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "56c1936c4cc7a1c9ab21a1ebb602eb942ba868cbd44a99cb7cdc5892335e1c85"
+checksum = "69358da18474cd46c5f7177018700ff255e13f9221c30b738f327eb005f8a17d"
 dependencies = [
- "linked-hash-map",
+ "env_logger",
+ "wolfram-app-discovery",
+]
+
+[[package]]
+name = "wstp"
+version = "0.2.9"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "b55ec3b0db4cf2ba433f65d972db6a2b9b9d69cd1b535a816713408a238cd75b"
+dependencies = [
+ "ref-cast",
+ "wolfram-expr",
+ "wstp-sys",
+]
+
+[[package]]
+name = "wstp-sys"
+version = "0.2.8"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "80076a52358dff4df32e337421844541a1e07a973162ee0b65093bbc4164ad3a"
+dependencies = [
+ "env_logger",
+ "link-cplusplus",
+ "wolfram-app-discovery",
+]
+
+[[package]]
+name = "zerocopy"
+version = "0.7.32"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "74d4d3961e53fa4c9a25a8637fc2bfaf2595b3d3ae34875568a5cf64787716be"
+dependencies = [
+ "zerocopy-derive",
+]
+
+[[package]]
+name = "zerocopy-derive"
+version = "0.7.32"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "9ce1b18ccd8e73a9321186f97e46f9f04b778851177567b1975109d26a08d2a6"
+dependencies = [
+ "proc-macro2",
+ "quote",
+ "syn 2.0.57",
 ]
```

### Comparing `gammaloop-0.0.1/dependencies/fjcore/fjcore.cc` & `gammaloop-0.1.0/python/gammaloop/dependencies/fjcore/fjcore.cc`

 * *Files identical despite different names*

### Comparing `gammaloop-0.0.1/dependencies/fjcore/fjcore.hh` & `gammaloop-0.1.0/python/gammaloop/dependencies/fjcore/fjcore.hh`

 * *Files identical despite different names*

### Comparing `gammaloop-0.0.1/dependencies/fjcore/wrapper.cc` & `gammaloop-0.1.0/python/gammaloop/dependencies/fjcore/wrapper.cc`

 * *Files identical despite different names*

### Comparing `gammaloop-0.0.1/python/gammaloop/data/models/scalars/__init__.py` & `gammaloop-0.1.0/python/gammaloop/data/models/scalars/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+# type: ignore
 from __future__ import absolute_import
 from . import particles
 from . import couplings
 from . import lorentz
 from . import parameters
 from . import vertices
 from . import coupling_orders
```

### Comparing `gammaloop-0.0.1/python/gammaloop/data/models/scalars/function_library.py` & `gammaloop-0.1.0/python/gammaloop/data/models/sm/function_library.py`

 * *Files identical despite different names*

### Comparing `gammaloop-0.0.1/python/gammaloop/data/models/scalars/lorentz.py` & `gammaloop-0.1.0/python/gammaloop/data/models/scalars/lorentz.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,16 +1,18 @@
+# type: ignore
 from __future__ import absolute_import
 from .object_library import all_lorentz, Lorentz
 
 from .function_library import complexconjugate, re, im, csc, sec, acsc, asec
 from . import parameters as Param
 
 try:
-   import form_factors as ForFac 
+    import form_factors as ForFac
 except ImportError:
-   pass
+    pass
 
 scalar_lorentz_structures = {}
 for n_point_interaction in Param.N_POINT_INTERACTIONS:
-   scalar_lorentz_structures[n_point_interaction] = Lorentz(name = 'SCALAR_%d_LORENTZ_STRUCTURE'%n_point_interaction,
-      spins = [ 1, ]*n_point_interaction,
-      structure = '1')
+    scalar_lorentz_structures[n_point_interaction] = Lorentz(name='SCALAR_%d_LORENTZ_STRUCTURE' % n_point_interaction,
+                                                             spins=[
+                                                                 1, ]*n_point_interaction,
+                                                             structure='1')
```

### Comparing `gammaloop-0.0.1/python/gammaloop/data/models/scalars/object_library.py` & `gammaloop-0.1.0/python/gammaloop/data/models/sm/object_library.py`

 * *Files identical despite different names*

### Comparing `gammaloop-0.0.1/python/gammaloop/data/models/scalars/particles.py` & `gammaloop-0.1.0/python/gammaloop/data/models/scalars/particles.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,25 +1,26 @@
+# type: ignore
 # This file was automatically created by FeynRules 1.7.69
 # Mathematica version: 8.0 for Mac OS X x86 (64-bit) (November 6, 2010)
 # Date: Mon 1 Oct 2012 14:58:25
 
 
 from __future__ import division
 from __future__ import absolute_import
-from .object_library import all_particles, Particle
+from .object_library import all_particles, Particle  # pylint: disable=unused-import
 from . import parameters as Param
 
 scalar_particles = []
 for i_scalar in range(Param.N_SCALARS):
-    scalar_particles.append(Particle(pdg_code = 1000+i_scalar,
-                name = 'scalar_%d'%i_scalar,
-                antiname = 'scalar_%d'%i_scalar,
-                spin = 1,
-                color = 1,
-                mass = Param.scalar_mass_parameters[i_scalar],
-                width = Param.scalar_width_parameters[i_scalar],
-                texname = '\\phi_%d'%i_scalar,
-                antitexname = '\\phi_%d'%i_scalar,
-                charge = 0,
-                GhostNumber = 0,
-                LeptonNumber = 0,
-                Y = 0))
+    scalar_particles.append(Particle(pdg_code=1000+i_scalar,
+                                     name='scalar_%d' % i_scalar,
+                                     antiname='scalar_%d' % i_scalar,
+                                     spin=1,
+                                     color=1,
+                                     mass=Param.scalar_mass_parameters[i_scalar],
+                                     width=Param.scalar_width_parameters[i_scalar],
+                                     texname='\\phi_%d' % i_scalar,
+                                     antitexname='\\phi_%d' % i_scalar,
+                                     charge=0,
+                                     GhostNumber=0,
+                                     LeptonNumber=0,
+                                     Y=0))
```

### Comparing `gammaloop-0.0.1/python/gammaloop/data/models/scalars/restrict_default.dat` & `gammaloop-0.1.0/python/gammaloop/data/models/scalars/restrict_default.dat`

 * *Files identical despite different names*

### Comparing `gammaloop-0.0.1/python/gammaloop/data/models/scalars/run_write_param_card.py` & `gammaloop-0.1.0/python/gammaloop/data/models/scalars/run_write_param_card.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,17 +1,19 @@
+# type: ignore
 #!/usr/bin/env python
 from __future__ import absolute_import
 from __future__ import print_function
 from six.moves import range
 
 import sys
 import os
 import importlib
 
 if '__main__' == __name__:
     dir_path = os.path.join(os.path.dirname(__file__))
-    sys.path.insert(0,os.path.join(dir_path,os.path.pardir))
-    pw = importlib.import_module('%s.%s'%(os.path.basename(dir_path),'write_param_card'))
+    sys.path.insert(0, os.path.join(dir_path, os.path.pardir))
+    pw = importlib.import_module('%s.%s' % (
+        os.path.basename(dir_path), 'write_param_card'))
     del sys.path[0]
 
     pw.ParamCardWriter('./param_card.dat', generic=True)
     print('write ./param_card.dat')
```

### Comparing `gammaloop-0.0.1/python/gammaloop/data/models/scalars/vertices.py` & `gammaloop-0.1.0/python/gammaloop/data/models/scalars/vertices.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,21 +1,23 @@
+# type: ignore
 # This file was automatically created by FeynRules 1.7.69
 # Mathematica version: 8.0 for Mac OS X x86 (64-bit) (November 6, 2010)
 # Date: Mon 1 Oct 2012 14:58:25
 
 
 from __future__ import absolute_import
 from .object_library import all_vertices, Vertex
 from . import particles as P
 from . import couplings as C
 from . import lorentz as L
 from . import parameters as Param
 import itertools
 
 for n_point_interaction in Param.N_POINT_INTERACTIONS:
-    for i_inter, interaction in enumerate(sorted(list(set( tuple(sorted(inter)) for inter in itertools.product( *[list(range(Param.N_SCALARS)),]*n_point_interaction ) )))):
+    for i_inter, interaction in enumerate(sorted(list(set(tuple(sorted(inter)) for inter in itertools.product(*[list(range(Param.N_SCALARS)),]*n_point_interaction))))):
         # Remember that the constructor automatically adds the objects to all_vertices
-        Vertex(name = 'V_%d_SCALAR_%s'%(n_point_interaction,''.join('%d'%scalar_id for scalar_id in interaction)),
-                particles = [ P.scalar_particles[scalar_id] for scalar_id in interaction ],
-                color = [ '1' ],
-                lorentz = [ L.scalar_lorentz_structures[n_point_interaction] ],
-                couplings = {(0,0):C.SCALAR_COUPLING})
+        Vertex(name='V_%d_SCALAR_%s' % (n_point_interaction, ''.join('%d' % scalar_id for scalar_id in interaction)),
+               particles=[P.scalar_particles[scalar_id]
+                          for scalar_id in interaction],
+               color=['1'],
+               lorentz=[L.scalar_lorentz_structures[n_point_interaction]],
+               couplings={(0, 0): C.SCALAR_COUPLING})
```

### Comparing `gammaloop-0.0.1/python/gammaloop/data/models/scalars/write_param_card.py` & `gammaloop-0.1.0/python/gammaloop/tests/test_data/models/loop_sm/write_param_card.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,14 @@
 
 from __future__ import absolute_import
-from __future__ import print_function
-from six.moves import range
+#from six.moves import range
+__date__ = "3 june 2010"
+__author__ = 'olivier.mattelaer@uclouvain.be'
+
+from .function_library import *
 
 class ParamCardWriter(object):
     
     header = \
     """######################################################################\n""" + \
     """## PARAM_CARD AUTOMATICALY GENERATED BY THE UFO  #####################\n""" + \
     """######################################################################\n"""   
@@ -76,16 +79,15 @@
                 all_lhablock.remove(name)
                 all_lhablock.insert(0, name)
         
         for lhablock in all_lhablock:
             self.write_block(lhablock)
             need_writing = [ param for param in all_ext_param if \
                                                      param.lhablock == lhablock]
-            from functools import cmp_to_key
-            need_writing.sort(key=cmp_to_key(self.order_param))
+            need_writing.sort(self.order_param)
             [self.write_param(param, lhablock) for param in need_writing]
             
             if self.generic_output:
                 if lhablock in ['MASS', 'DECAY']:
                     self.write_dep_param_block(lhablock)
 
         if self.generic_output:
@@ -114,18 +116,15 @@
 
 
     
     def write_dep_param_block(self, lhablock):
         import cmath
         from .parameters import all_parameters
         for parameter in all_parameters:
-            try:
-                exec("%s = %s" % (parameter.name, parameter.value))
-            except Exception:
-                pass
+            exec("%s = %s" % (parameter.name, parameter.value))
         text = "##  Not dependent paramater.\n"
         text += "## Those values should be edited following analytical the \n"
         text += "## analytical expression. Some generator could simply ignore \n"
         text += "## those values and use the analytical expression\n"
         
         if lhablock == 'MASS':
             data = self.dep_mass
@@ -165,12 +164,19 @@
                                  'name': part.name,
                                  'charge': 3 * part.charge,
                                  'spin': 2 * part.spin + 1,
                                  'color': part.color,
                                  'antipart': part.name != part.antiname and 1 or 0}
         
         self.fsock.write(text)
-    
+        
+        
+            
+            
+            
+            
+        
+            
 if '__main__' == __name__:
     ParamCardWriter('./param_card.dat', generic=True)
     print('write ./param_card.dat')
```

### Comparing `gammaloop-0.0.1/python/gammaloop/data/models/sm/__init__.py` & `gammaloop-0.1.0/python/gammaloop/data/models/sm/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,21 +1,22 @@
+# type: ignore
 from __future__ import absolute_import
 from . import particles
 from . import couplings
 from . import lorentz
 from . import parameters
 from . import vertices
 from . import coupling_orders
 from . import function_library
 from . import object_library
-#from . import write_param_card
+# from . import write_param_card
 try:
     from . import decays
 except ImportError:
-    pass    
+    pass
 try:
     from . import build_restrict
 except ImportError:
     pass
 
 # model options
 gauge = [0, 1]
@@ -24,13 +25,13 @@
 all_particles = particles.all_particles
 all_vertices = vertices.all_vertices
 all_couplings = couplings.all_couplings
 all_lorentz = lorentz.all_lorentz
 all_parameters = parameters.all_parameters
 all_orders = coupling_orders.all_orders
 all_functions = function_library.all_functions
-#all_decays = decays.all_decays
+# all_decays = decays.all_decays
 
 
 __author__ = "N. Christensen, C. Duhr"
 __version__ = "1.3"
 __email__ = "neil@pa.msu.edu, claude.duhr@uclouvain.be"
```

### Comparing `gammaloop-0.0.1/python/gammaloop/data/models/sm/build_restrict.py` & `gammaloop-0.1.0/python/gammaloop/data/models/sm/build_restrict.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,23 +1,24 @@
+# type: ignore
 ################################################################################
 #
 # Copyright (c) 2012 The MadGraph5_aMC@NLO Development team and Contributors
 #
-# This file is a part of the MadGraph5_aMC@NLO project, an application which 
+# This file is a part of the MadGraph5_aMC@NLO project, an application which
 # automatically generates Feynman diagrams and matrix elements for arbitrary
 # high-energy processes in the Standard Model and beyond.
 #
-# It is subject to the MadGraph5_aMC@NLO license which should accompany this 
+# It is subject to the MadGraph5_aMC@NLO license which should accompany this
 # distribution.
 #
 # For more information, visit madgraph.phys.ucl.ac.be and amcatnlo.web.cern.ch
 #
 ################################################################################
 """ This part is not part of the UFO Model but only of MG5 suite. 
-This files defines how the restrict card can be build automatically """ 
+This files defines how the restrict card can be build automatically """
 
 ### Important Warning ###
 # When you develop such file. Please cross check that they are NO
 # unwanted simplification to your model. This can happen especially
 # if a bunch of value are set to 1.0 by default. This YOUR responsability
 # to check that you get the expected behavior
 ### Important Warning ###
@@ -26,45 +27,44 @@
 import models.build_restriction_lib as build_restrict_lib
 all_categories = []
 
 
 first_category = build_restrict_lib.Category('sm customization')
 all_categories.append(first_category)
 
-first_category.add_options(name='diagonal ckm', # name
+first_category.add_options(name='diagonal ckm',  # name
                            default=True,          # default
-                           rules=[('WOLFENSTEIN',[1], 0.0),
-                                  ('WOLFENSTEIN',[2], 0.0),
-                                  ('WOLFENSTEIN',[3], 0.0),
-                                  ('WOLFENSTEIN',[4], 0.0)]
+                           rules=[('WOLFENSTEIN', [1], 0.0),
+                                  ('WOLFENSTEIN', [2], 0.0),
+                                  ('WOLFENSTEIN', [3], 0.0),
+                                  ('WOLFENSTEIN', [4], 0.0)]
                            )
 
-first_category.add_options(name='c mass = 0', # name
+first_category.add_options(name='c mass = 0',  # name
                            default=True,        # default
-                           rules=[('MASS',[4], 0.0),
-                                  ('YUKAWA',[4], 0.0)]
+                           rules=[('MASS', [4], 0.0),
+                                  ('YUKAWA', [4], 0.0)]
                            )
 
 first_category.add_options(name='b mass = 0',
                            default=False,
-                           rules=[('MASS',[5], 0.0),
-                                  ('YUKAWA',[5], 0.0)]
+                           rules=[('MASS', [5], 0.0),
+                                  ('YUKAWA', [5], 0.0)]
                            )
 
 first_category.add_options(name='tau mass = 0',
                            default=False,
-                           rules=[('MASS',[15], 0.0),
-                                  ('YUKAWA',[15], 0.0)]
+                           rules=[('MASS', [15], 0.0),
+                                  ('YUKAWA', [15], 0.0)]
                            )
 
 first_category.add_options(name='muon mass = 0',
                            default=True,
-                           rules=[('MASS',[13], 0.0),
-                                  ('YUKAWA',[13], 0.0)]
+                           rules=[('MASS', [13], 0.0),
+                                  ('YUKAWA', [13], 0.0)]
                            )
 
 first_category.add_options(name='electron mass = 0',
                            default=True,
-                           rules=[('MASS',[11], 0.0),
-                                  ('YUKAWA',[11], 0.0)]
+                           rules=[('MASS', [11], 0.0),
+                                  ('YUKAWA', [11], 0.0)]
                            )
-
```

### Comparing `gammaloop-0.0.1/python/gammaloop/data/models/sm/couplings.py` & `gammaloop-0.1.0/python/gammaloop/data/models/sm/couplings.py`

 * *Files identical despite different names*

### Comparing `gammaloop-0.0.1/python/gammaloop/data/models/sm/decays.py` & `gammaloop-0.1.0/python/gammaloop/data/models/sm/decays.py`

 * *Files identical despite different names*

### Comparing `gammaloop-0.0.1/python/gammaloop/data/models/sm/function_library.py` & `gammaloop-0.1.0/python/gammaloop/tests/test_data/models/loop_sm/function_library.py`

 * *Files 14% similar despite different names*

```diff
@@ -3,21 +3,25 @@
 # This file contains definitions for functions that
 # are extensions of the cmath library, and correspond
 # either to functions that are in cmath, but inconvenient
 # to access from there (e.g. z.conjugate()),
 # or functions that are simply not defined.
 #
 #
+
 from __future__ import absolute_import
 __date__ = "22 July 2010"
 __author__ = "claude.duhr@durham.ac.uk"
 
-from cmath import cos, sin, acos, asin
-from .object_library import all_functions, Function
-
+import cmath
+try:
+    from .object_library import all_functions, Function
+except:
+    from . import object_library
+    all_functions, Function = object_library.all_functions , object_library.Function
 #
 # shortcuts for functions from cmath
 #
 
 complexconjugate = Function(name = 'complexconjugate',
                             arguments = ('z',),
                             expression = 'z.conjugate()')
@@ -27,26 +31,38 @@
               arguments = ('z',),
               expression = 'z.real')
 
 im = Function(name = 'im',
               arguments = ('z',),
               expression = 'z.imag')
 
+# Auxiliary functions for NLO
+
+cond = Function(name = 'cond',
+                arguments = ('condition','ExprTrue','ExprFalse'),
+                expression = '(ExprTrue if condition==0.0 else ExprFalse)')
+
+reglog = Function(name = 'reglog',
+                arguments = ('z'),
+                expression = '(0.0 if z==0.0 else cmath.log(z))')
 
 # New functions (trigonometric)
 
 sec = Function(name = 'sec',
              arguments = ('z',),
-             expression = '1./cos(z)')
+             expression = '1./cmath.cos(z)')
 
 asec = Function(name = 'asec',
              arguments = ('z',),
-             expression = 'acos(1./z)')
+             expression = 'cmath.acos(1./z)')
 
 csc = Function(name = 'csc',
              arguments = ('z',),
-             expression = '1./sin(z)')
+             expression = '1./cmath.sin(z)')
 
 acsc = Function(name = 'acsc',
              arguments = ('z',),
-             expression = 'asin(1./z)')
+             expression = 'cmath.asin(1./z)')
+
+
+
```

### Comparing `gammaloop-0.0.1/python/gammaloop/data/models/sm/object_library.py` & `gammaloop-0.1.0/python/gammaloop/data/models/scalars/object_library.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,11 @@
+# type: ignore
 ##
 ##
-## Feynrules Header
+# Feynrules Header
 ##
 ##
 ##
 ##
 ##
 
 from __future__ import absolute_import
@@ -13,260 +14,267 @@
 
 class UFOBaseClass(object):
     """The class from which all FeynRules classes are derived."""
 
     require_args = []
 
     def __init__(self, *args, **options):
-        assert(len(self.require_args) == len (args))
-    
+        assert (len(self.require_args) == len(args))
+
         for i, name in enumerate(self.require_args):
             setattr(self, name, args[i])
-    
+
         for (option, value) in options.items():
             setattr(self, option, value)
 
     def get(self, name):
         return getattr(self, name)
-    
+
     def set(self, name, value):
         setattr(self, name, value)
-        
+
     def get_all(self):
         """Return a dictionary containing all the information of the object"""
         return self.__dict__
 
     def __str__(self):
         return self.name
 
     def nice_string(self):
         """ return string with the full information """
-        return '\n'.join(['%s \t: %s' %(name, value) for name, value in self.__dict__.items()])
+        return '\n'.join(['%s \t: %s' % (name, value) for name, value in self.__dict__.items()])
 
     def __repr__(self):
         replacements = [
-            ('+','__plus__'),
-            ('-','__minus__'),
-            ('@','__at__'),
-            ('!','__exclam__'),
-            ('?','__quest__'),
-            ('*','__star__'),
-            ('~','__tilde__')
-            ]
+            ('+', '__plus__'),
+            ('-', '__minus__'),
+            ('@', '__at__'),
+            ('!', '__exclam__'),
+            ('?', '__quest__'),
+            ('*', '__star__'),
+            ('~', '__tilde__')
+        ]
         text = self.name
-        for orig,sub in replacements:
-            text = text.replace(orig,sub)
+        for orig, sub in replacements:
+            text = text.replace(orig, sub)
         return text
 
 
-
 all_particles = []
 
-    
 
 class Particle(UFOBaseClass):
     """A standard Particle"""
 
-    require_args=['pdg_code', 'name', 'antiname', 'spin', 'color', 'mass', 'width', 'texname', 'antitexname', 'charge']
+    require_args = ['pdg_code', 'name', 'antiname', 'spin',
+                    'color', 'mass', 'width', 'texname', 'antitexname', 'charge']
 
-    require_args_all = ['pdg_code', 'name', 'antiname', 'spin', 'color', 'mass', 'width', 'texname', 'antitexname', 'charge', 'line', 'propagating', 'goldstoneboson']
+    require_args_all = ['pdg_code', 'name', 'antiname', 'spin', 'color', 'mass', 'width',
+                        'texname', 'antitexname', 'charge', 'line', 'propagating', 'goldstoneboson']
 
     def __init__(self, pdg_code, name, antiname, spin, color, mass, width, texname,
-                 antitexname, charge , line=None, propagating=True, goldstoneboson=False, **options):
+                 antitexname, charge, line=None, propagating=True, goldstoneboson=False, **options):
 
-        args= (pdg_code, name, antiname, spin, color, mass, width, texname,
-                 antitexname, float(charge))
+        args = (pdg_code, name, antiname, spin, color, mass, width, texname,
+                antitexname, float(charge))
 
         UFOBaseClass.__init__(self, *args,  **options)
 
         global all_particles
         all_particles.append(self)
 
         self.propagating = propagating
-        self.goldstoneboson= goldstoneboson
+        self.goldstoneboson = goldstoneboson
 
         self.selfconjugate = (name == antiname)
-        if 1: #not line:
+        if 1:  # not line:
             self.line = self.find_line_type()
         else:
             self.line = line
 
-
-
-
     def find_line_type(self):
         """ find how we draw a line if not defined
         valid output: dashed/straight/wavy/curly/double/swavy/scurly
         """
-        
+
         spin = self.spin
         color = self.color
-        
-        #use default
+
+        # use default
         if spin == 1:
             return 'dashed'
         elif spin == 2:
             if not self.selfconjugate:
                 return 'straight'
             elif color == 1:
                 return 'swavy'
             else:
                 return 'scurly'
         elif spin == 3:
             if color == 1:
                 return 'wavy'
-            
+
             else:
                 return 'curly'
         elif spin == 5:
             return 'double'
         elif spin == -1:
             return 'dotted'
         else:
-            return 'dashed' # not supported yet
+            return 'dashed'  # not supported yet
 
     def anti(self):
         if self.selfconjugate:
-            raise Exception('%s has no anti particle.' % self.name) 
+            raise Exception('%s has no anti particle.' % self.name)
         outdic = {}
-        for k,v in self.__dict__.items():
-            if k not in self.require_args_all:                
+        for k, v in self.__dict__.items():
+            if k not in self.require_args_all:
                 outdic[k] = -v
-        if self.color in [1,8]:
+        if self.color in [1, 8]:
             newcolor = self.color
         else:
             newcolor = -self.color
-                
+
         return Particle(-self.pdg_code, self.antiname, self.name, self.spin, newcolor, self.mass, self.width,
                         self.antitexname, self.texname, -self.charge, self.line, self.propagating, self.goldstoneboson, **outdic)
 
 
-
 all_parameters = []
 
+
 class Parameter(UFOBaseClass):
 
-    require_args=['name', 'nature', 'type', 'value', 'texname']
+    require_args = ['name', 'nature', 'type', 'value', 'texname']
 
     def __init__(self, name, nature, type, value, texname, lhablock=None, lhacode=None):
 
-        args = (name,nature,type,value,texname)
+        args = (name, nature, type, value, texname)
 
         UFOBaseClass.__init__(self, *args)
 
-        args=(name,nature,type,value,texname)
+        args = (name, nature, type, value, texname)
 
         global all_parameters
         all_parameters.append(self)
 
-        if (lhablock is None or lhacode is None)  and nature == 'external':
-            raise Exception('Need LHA information for external parameter "%s".' % name)
+        if (lhablock is None or lhacode is None) and nature == 'external':
+            raise Exception(
+                'Need LHA information for external parameter "%s".' % name)
         self.lhablock = lhablock
         self.lhacode = lhacode
 
+
 all_vertices = []
 
+
 class Vertex(UFOBaseClass):
 
-    require_args=['name', 'particles', 'color', 'lorentz', 'couplings']
+    require_args = ['name', 'particles', 'color', 'lorentz', 'couplings']
 
     def __init__(self, name, particles, color, lorentz, couplings, **opt):
- 
+
         args = (name, particles, color, lorentz, couplings)
 
         UFOBaseClass.__init__(self, *args, **opt)
 
-        args=(particles,color,lorentz,couplings)
+        args = (particles, color, lorentz, couplings)
 
         global all_vertices
         all_vertices.append(self)
 
+
 all_couplings = []
 
+
 class Coupling(UFOBaseClass):
 
-    require_args=['name', 'value', 'order']
+    require_args = ['name', 'value', 'order']
 
     def __init__(self, name, value, order, **opt):
 
-        args =(name, value, order)	
+        args = (name, value, order)
         UFOBaseClass.__init__(self, *args, **opt)
         global all_couplings
         all_couplings.append(self)
-  
 
 
 all_lorentz = []
 
+
 class Lorentz(UFOBaseClass):
 
-    require_args=['name','spins','structure']
-    
+    require_args = ['name', 'spins', 'structure']
+
     def __init__(self, name, spins, structure='external', **opt):
         args = (name, spins, structure)
         UFOBaseClass.__init__(self, *args, **opt)
 
         global all_lorentz
         all_lorentz.append(self)
 
 
 all_functions = []
 
+
 class Function(object):
 
     def __init__(self, name, arguments, expression):
 
         global all_functions
         all_functions.append(self)
 
         self.name = name
         self.arguments = arguments
         self.expr = expression
-    
+
     def __call__(self, *opt):
 
         for i, arg in enumerate(self.arguments):
-            exec('%s = %s' % (arg, opt[i] ))
+            exec('%s = %s' % (arg, opt[i]))
 
         return eval(self.expr)
 
+
 all_orders = []
 
+
 class CouplingOrder(object):
 
-    def __init__(self, name, expansion_order, hierarchy, perturbative_expansion = 0):
-        
+    def __init__(self, name, expansion_order, hierarchy, perturbative_expansion=0):
+
         global all_orders
         all_orders.append(self)
 
         self.name = name
         self.expansion_order = expansion_order
         self.hierarchy = hierarchy
 
+
 all_decays = []
 
+
 class Decay(UFOBaseClass):
-    require_args = ['particle','partial_widths']
+    require_args = ['particle', 'partial_widths']
 
     def __init__(self, particle, partial_widths, **opt):
         args = (particle, partial_widths)
         UFOBaseClass.__init__(self, *args, **opt)
 
         global all_decays
         all_decays.append(self)
-    
+
         # Add the information directly to the particle
         particle.partial_widths = partial_widths
 
+
 all_form_factors = []
 
+
 class FormFactor(UFOBaseClass):
-    require_args = ['name','type','value']
+    require_args = ['name', 'type', 'value']
 
     def __init__(self, name, type, value, **opt):
         args = (name, type, value)
         UFOBaseClass.__init__(self, *args, **opt)
 
         global all_form_factors
         all_form_factors.append(self)
-
-
```

### Comparing `gammaloop-0.0.1/python/gammaloop/data/models/sm/particles.py` & `gammaloop-0.1.0/python/gammaloop/tests/test_data/models/loop_sm/particles.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,386 +1,343 @@
-# This file was automatically created by FeynRules 1.7.69
-# Mathematica version: 8.0 for Mac OS X x86 (64-bit) (November 6, 2010)
-# Date: Mon 1 Oct 2012 14:58:25
+# This file was automatically created by FeynRules $Revision: 535 $
+# Mathematica version: 7.0 for Mac OS X x86 (64-bit) (November 11, 2008)
+# Date: Fri 18 Mar 2011 18:40:51
 
 
 from __future__ import division
 from __future__ import absolute_import
 from .object_library import all_particles, Particle
 from . import parameters as Param
+from . import CT_parameters as CTParam
 
-a = Particle(pdg_code = 22,
-             name = 'a',
-             antiname = 'a',
-             spin = 3,
-             color = 1,
+# ======================================================================
+# QCD particles
+# ======================================================================
+
+d = Particle(pdg_code = 1,
+             name = 'd',
+             antiname = 'd~',
+             spin = 2,
+             color = 3,
              mass = Param.ZERO,
              width = Param.ZERO,
-             texname = 'a',
-             antitexname = 'a',
-             charge = 0,
-             GhostNumber = 0,
+             texname = 'd',
+             antitexname = 'd',
+             charge = -1/3,
              LeptonNumber = 0,
-             Y = 0)
+             GhostNumber = 0)
 
-Z = Particle(pdg_code = 23,
-             name = 'Z',
-             antiname = 'Z',
-             spin = 3,
-             color = 1,
-             mass = Param.MZ,
-             width = Param.WZ,
-             texname = 'Z',
-             antitexname = 'Z',
-             charge = 0,
-             GhostNumber = 0,
+d__tilde__ = d.anti()
+
+u = Particle(pdg_code = 2,
+             name = 'u',
+             antiname = 'u~',
+             spin = 2,
+             color = 3,
+             mass = Param.ZERO,
+             width = Param.ZERO,
+             texname = 'u',
+             antitexname = 'u',
+             charge = 2/3,
              LeptonNumber = 0,
-             Y = 0)
+             GhostNumber = 0)
 
-W__plus__ = Particle(pdg_code = 24,
-                     name = 'W+',
-                     antiname = 'W-',
-                     spin = 3,
-                     color = 1,
-                     mass = Param.MW,
-                     width = Param.WW,
-                     texname = 'W+',
-                     antitexname = 'W-',
-                     charge = 1,
-                     GhostNumber = 0,
-                     LeptonNumber = 0,
-                     Y = 0)
+u__tilde__ = u.anti()
 
-W__minus__ = W__plus__.anti()
+s = Particle(pdg_code = 3,
+             name = 's',
+             antiname = 's~',
+             spin = 2,
+             color = 3,
+             mass = Param.ZERO,
+             width = Param.ZERO,
+             texname = 's',
+             antitexname = 's',
+             charge = -1/3,
+             LeptonNumber = 0,
+             GhostNumber = 0)
+
+s__tilde__ = s.anti()
 
-g = Particle(pdg_code = 21,
-             name = 'g',
-             antiname = 'g',
+c = Particle(pdg_code = 4,
+             name = 'c',
+             antiname = 'c~',
+             spin = 2,
+             color = 3,
+             mass = Param.MC,
+             width = Param.ZERO,
+             texname = 'c',
+             antitexname = 'c',
+             charge = 2/3,
+             LeptonNumber = 0,
+             GhostNumber = 0)
+
+c__tilde__ = c.anti()
+
+b = Particle(pdg_code = 5,
+             name = 'b',
+             antiname = 'b~',
+             spin = 2,
+             color = 3,
+             mass = Param.MB,
+             width = Param.ZERO,
+             texname = 'b',
+             antitexname = 'b',
+             charge = -1/3,
+             LeptonNumber = 0,
+             GhostNumber = 0)
+
+b__tilde__ = b.anti()
+
+t = Particle(pdg_code = 6,
+             name = 't',
+             antiname = 't~',
+             spin = 2,
+             color = 3,
+             mass = Param.MT,
+             width = Param.WT,
+             texname = 't',
+             antitexname = 't',
+             charge = 2/3,
+             LeptonNumber = 0,
+             GhostNumber = 0)
+
+t__tilde__ = t.anti()
+
+G = Particle(pdg_code = 21,
+             name = 'G',
+             antiname = 'G',
              spin = 3,
              color = 8,
              mass = Param.ZERO,
              width = Param.ZERO,
-             texname = 'g',
-             antitexname = 'g',
+             texname = 'G',
+             antitexname = 'G',
              charge = 0,
-             GhostNumber = 0,
              LeptonNumber = 0,
-             Y = 0)
+             GhostNumber = 0)
 
-ghA = Particle(pdg_code = 9000001,
-               name = 'ghA',
-               antiname = 'ghA~',
-               spin = -1,
-               color = 1,
-               mass = Param.ZERO,
-               width = Param.ZERO,
-               texname = 'ghA',
-               antitexname = 'ghA~',
-               charge = 0,
-               GhostNumber = 1,
-               LeptonNumber = 0,
-               Y = 0)
-
-ghA__tilde__ = ghA.anti()
-
-ghZ = Particle(pdg_code = 9000002,
-               name = 'ghZ',
-               antiname = 'ghZ~',
-               spin = -1,
-               color = 1,
-               mass = Param.MZ,
-               width = Param.WZ,
-               texname = 'ghZ',
-               antitexname = 'ghZ~',
-               charge = 0,
-               GhostNumber = 1,
-               LeptonNumber = 0,
-               Y = 0)
-
-ghZ__tilde__ = ghZ.anti()
-
-ghWp = Particle(pdg_code = 9000003,
-                name = 'ghWp',
-                antiname = 'ghWp~',
-                spin = -1,
-                color = 1,
-                mass = Param.MW,
-                width = Param.WW,
-                texname = 'ghWp',
-                antitexname = 'ghWp~',
-                charge = 1,
-                GhostNumber = 1,
-                LeptonNumber = 0,
-                Y = 0)
-
-ghWp__tilde__ = ghWp.anti()
-
-ghWm = Particle(pdg_code = 9000004,
-                name = 'ghWm',
-                antiname = 'ghWm~',
-                spin = -1,
-                color = 1,
-                mass = Param.MW,
-                width = Param.WW,
-                texname = 'ghWm',
-                antitexname = 'ghWm~',
-                charge = -1,
-                GhostNumber = 1,
-                LeptonNumber = 0,
-                Y = 0)
-
-ghWm__tilde__ = ghWm.anti()
-
-ghG = Particle(pdg_code = 9000005,
-               name = 'ghG',
-               antiname = 'ghG~',
-               spin = -1,
-               color = 8,
-               mass = Param.ZERO,
-               width = Param.ZERO,
-               texname = 'ghG',
-               antitexname = 'ghG~',
-               charge = 0,
-               GhostNumber = 1,
-               LeptonNumber = 0,
-               Y = 0)
+gh = Particle(pdg_code = 82,
+             name = 'gh',
+             antiname = 'gh~',
+             spin = -1,
+             color = 8,
+             mass = Param.ZERO,
+             width = Param.ZERO,
+             texname = 'gh',
+             antitexname = 'gh',
+             charge = 0,
+             LeptonNumber = 0,
+             line='dashed',
+             GhostNumber = 1)
+
+gh__tilde__ = gh.anti()
 
-ghG__tilde__ = ghG.anti()
+# ======================================================================
+# Other particles 
+# ======================================================================
 
 ve = Particle(pdg_code = 12,
               name = 've',
               antiname = 've~',
               spin = 2,
               color = 1,
               mass = Param.ZERO,
               width = Param.ZERO,
               texname = 've',
-              antitexname = 've~',
+              antitexname = 've',
               charge = 0,
-              GhostNumber = 0,
               LeptonNumber = 1,
-              Y = 0)
+              GhostNumber = 0)
 
 ve__tilde__ = ve.anti()
 
 vm = Particle(pdg_code = 14,
               name = 'vm',
               antiname = 'vm~',
               spin = 2,
               color = 1,
               mass = Param.ZERO,
               width = Param.ZERO,
               texname = 'vm',
-              antitexname = 'vm~',
+              antitexname = 'vm',
               charge = 0,
-              GhostNumber = 0,
               LeptonNumber = 1,
-              Y = 0)
+              GhostNumber = 0)
 
 vm__tilde__ = vm.anti()
 
 vt = Particle(pdg_code = 16,
               name = 'vt',
               antiname = 'vt~',
               spin = 2,
               color = 1,
               mass = Param.ZERO,
               width = Param.ZERO,
               texname = 'vt',
-              antitexname = 'vt~',
+              antitexname = 'vt',
               charge = 0,
-              GhostNumber = 0,
               LeptonNumber = 1,
-              Y = 0)
+              GhostNumber = 0)
 
 vt__tilde__ = vt.anti()
 
-u = Particle(pdg_code = 2,
-             name = 'u',
-             antiname = 'u~',
-             spin = 2,
-             color = 3,
-             mass = Param.ZERO,
-             width = Param.ZERO,
-             texname = 'u',
-             antitexname = 'u~',
-             charge = 2/3,
-             GhostNumber = 0,
-             LeptonNumber = 0,
-             Y = 0)
-
-u__tilde__ = u.anti()
-
-c = Particle(pdg_code = 4,
-             name = 'c',
-             antiname = 'c~',
-             spin = 2,
-             color = 3,
-             mass = Param.MC,
-             width = Param.ZERO,
-             texname = 'c',
-             antitexname = 'c~',
-             charge = 2/3,
-             GhostNumber = 0,
-             LeptonNumber = 0,
-             Y = 0)
-
-c__tilde__ = c.anti()
-
-t = Particle(pdg_code = 6,
-             name = 't',
-             antiname = 't~',
-             spin = 2,
-             color = 3,
-             mass = Param.MT,
-             width = Param.WT,
-             texname = 't',
-             antitexname = 't~',
-             charge = 2/3,
-             GhostNumber = 0,
-             LeptonNumber = 0,
-             Y = 0)
-
-t__tilde__ = t.anti()
-
-d = Particle(pdg_code = 1,
-             name = 'd',
-             antiname = 'd~',
-             spin = 2,
-             color = 3,
+A = Particle(pdg_code = 22,
+             name = 'A',
+             antiname = 'A',
+             spin = 3,
+             color = 1,
              mass = Param.ZERO,
              width = Param.ZERO,
-             texname = 'd',
-             antitexname = 'd~',
-             charge = -1/3,
-             GhostNumber = 0,
+             texname = 'A',
+             antitexname = 'A',
+             charge = 0,
              LeptonNumber = 0,
-             Y = 0)
-
-d__tilde__ = d.anti()
+             GhostNumber = 0)
 
-s = Particle(pdg_code = 3,
-             name = 's',
-             antiname = 's~',
-             spin = 2,
-             color = 3,
-             mass = Param.ZERO,
-             width = Param.ZERO,
-             texname = 's',
-             antitexname = 's~',
-             charge = -1/3,
-             GhostNumber = 0,
+Z = Particle(pdg_code = 23,
+             name = 'Z',
+             antiname = 'Z',
+             spin = 3,
+             color = 1,
+             mass = Param.MZ,
+             width = Param.WZ,
+             texname = 'Z',
+             antitexname = 'Z',
+             charge = 0,
              LeptonNumber = 0,
-             Y = 0)
+             GhostNumber = 0)
 
-s__tilde__ = s.anti()
-
-b = Particle(pdg_code = 5,
-             name = 'b',
-             antiname = 'b~',
-             spin = 2,
-             color = 3,
-             mass = Param.MB,
-             width = Param.ZERO,
-             texname = 'b',
-             antitexname = 'b~',
-             charge = -1/3,
-             GhostNumber = 0,
-             LeptonNumber = 0,
-             Y = 0)
+W__plus__ = Particle(pdg_code = 24,
+                     name = 'W+',
+                     antiname = 'W-',
+                     spin = 3,
+                     color = 1,
+                     mass = Param.MW,
+                     width = Param.WW,
+                     texname = 'W+',
+                     antitexname = 'W+',
+                     charge = 1,
+                     LeptonNumber = 0,
+                     GhostNumber = 0)
 
-b__tilde__ = b.anti()
+W__minus__ = W__plus__.anti()
 
 H = Particle(pdg_code = 25,
              name = 'H',
              antiname = 'H',
              spin = 1,
              color = 1,
              mass = Param.MH,
              width = Param.WH,
-             texname = 'H',
-             antitexname = 'H',
+             texname = '\\phi',
+             antitexname = '\\phi',
              charge = 0,
-             GhostNumber = 0,
              LeptonNumber = 0,
-             Y = 0)
+             GhostNumber = 0)
+
+e__minus__ = Particle(pdg_code = 11,
+                      name = 'e-',
+                      antiname = 'e+',
+                      spin = 2,
+                      color = 1,
+                      mass = Param.Me,
+                      width = Param.ZERO,
+                      texname = 'e-',
+                      antitexname = 'e-',
+                      charge = -1,
+                      LeptonNumber = 1,
+                      GhostNumber = 0)
+
+e__plus__ = e__minus__.anti()
+
+m__minus__ = Particle(pdg_code = 13,
+                      name = 'm-',
+                      antiname = 'm+',
+                      spin = 2,
+                      color = 1,
+                      mass = Param.MM,
+                      width = Param.ZERO,
+                      texname = 'm-',
+                      antitexname = 'm-',
+                      charge = -1,
+                      LeptonNumber = 1,
+                      GhostNumber = 0)
+
+m__plus__ = m__minus__.anti()
+
+tt__minus__ = Particle(pdg_code = 15,
+                       name = 'tt-',
+                       antiname = 'tt+',
+                       spin = 2,
+                       color = 1,
+                       mass = Param.MTA,
+                       width = Param.WTau,
+                       texname = 'tt-',
+                       antitexname = 'tt-',
+                       charge = -1,
+                       LeptonNumber = 1,
+                       GhostNumber = 0)
+
+tt__plus__ = tt__minus__.anti()
+
+# ======================================================================
+# Goldstones 
+# ======================================================================
 
 G0 = Particle(pdg_code = 250,
               name = 'G0',
               antiname = 'G0',
               spin = 1,
               color = 1,
               mass = Param.MZ,
               width = Param.WZ,
               texname = 'G0',
               antitexname = 'G0',
               GoldstoneBoson = True,
               charge = 0,
               GhostNumber = 0,
-              LeptonNumber = 0,
-              Y = 0)
+              LeptonNumber = 0)
 
 G__plus__ = Particle(pdg_code = 251,
                      name = 'G+',
                      antiname = 'G-',
                      spin = 1,
                      color = 1,
                      mass = Param.MW,
                      width = Param.WW,
                      texname = 'G+',
                      antitexname = 'G-',
                      GoldstoneBoson = True,
                      charge = 1,
                      GhostNumber = 0,
-                     LeptonNumber = 0,
-                     Y = 0)
+                     LeptonNumber = 0)
 
 G__minus__ = G__plus__.anti()
 
-e__minus__ = Particle(pdg_code = 11,
-                      name = 'e-',
-                      antiname = 'e+',
-                      spin = 2,
-                      color = 1,
-                      mass = Param.Me,
-                      width = Param.ZERO,
-                      texname = 'e-',
-                      antitexname = 'e+',
-                      charge = -1,
-                      GhostNumber = 0,
-                      LeptonNumber = 1,
-                      Y = 0)
+# Wavefunction renormalization
 
-e__plus__ = e__minus__.anti()
+b.loop_particles = [[[5,21]]]
+b.counterterm = {(1,0,0):CTParam.bWcft_UV.value}
 
-mu__minus__ = Particle(pdg_code = 13,
-                       name = 'mu-',
-                       antiname = 'mu+',
-                       spin = 2,
-                       color = 1,
-                       mass = Param.MM,
-                       width = Param.ZERO,
-                       texname = 'mu-',
-                       antitexname = 'mu+',
-                       charge = -1,
-                       GhostNumber = 0,
-                       LeptonNumber = 1,
-                       Y = 0)
+c.loop_particles = [[[4,21]]]
+c.counterterm = {(1,0,0):CTParam.cWcft_UV.value}
 
-mu__plus__ = mu__minus__.anti()
+t.loop_particles = [[[6,21]]]
+t.counterterm = {(1,0,0):CTParam.tWcft_UV.value}
 
-ta__minus__ = Particle(pdg_code = 15,
-                       name = 'ta-',
-                       antiname = 'ta+',
-                       spin = 2,
-                       color = 1,
-                       mass = Param.MTA,
-                       width = Param.WTau,
-                       texname = 'ta-',
-                       antitexname = 'ta+',
-                       charge = -1,
-                       GhostNumber = 0,
-                       LeptonNumber = 1,
-                       Y = 0)
+G.loop_particles = [[[4]],[[5]],[[6]]]
+G.counterterm = {(1,0,0):CTParam.GWcft_UV_c.value,(1,0,1):CTParam.GWcft_UV_b.value,(1,0,2):CTParam.GWcft_UV_t.value}
+
+# Set counterterms values
+
+#Param.MB.loop_particles= [[[5,21]]]
+#Param.MB.counterterm = {(1,0,0):CTParam.bMass_UV.value}
+
+#Param.MC.loop_particles= [[[4,21]]]
+#Param.MC.counterterm = {(1,0,0):CTParam.cMass_UV.value}
 
-ta__plus__ = ta__minus__.anti()
+#Param.MT.loop_particles= [[[6,21]]]
+#Param.MT.counterterm = {(1,0,0):CTParam.tMass_UV.value}
 
+#Param.G.loop_particles = [[[2],[1],[3]],[[4]],[[5]],[[6]],[[21]]],
+#Param.G.counterterm = {(1,0,0):CTParam.G_UVq.value,(1,0,1):CTParam.G_UVc.value,(1,0,2):CTParam.G_UVb.value,(1,0,3):CTParam.G_UVt.value,(1,0,4):CTParam.G_UVg.value},
```

### Comparing `gammaloop-0.0.1/python/gammaloop/data/models/sm/restrict_VH.dat` & `gammaloop-0.1.0/python/gammaloop/data/models/sm/restrict_c_mass.dat`

 * *Files 6% similar despite different names*

```diff
@@ -10,44 +10,44 @@
     2 1.166390e-05 # Gf 
     3 1.180000e-01 # aS 
 
 ###################################
 ## INFORMATION FOR MASS
 ###################################
 Block MASS 
-    4 0.000000e+00 # MC 
+    4 1.550000e+00 # MC 
     5 4.700000e+00 # MB 
     6 1.730000e+02 # MT 
    11 0.000000e+00 # Me 
-   13 1.056600e-01 # MM 
+   13 0.000000e+00 # MM 
    15 1.777000e+00 # MTA 
    23 9.118800e+01 # MZ 
    25 1.250000e+02 # MH 
 
 ###################################
 ## INFORMATION FOR DECAY
 ###################################
 DECAY   6 1.491500E+00
-DECAY  15 2.270000e-12
+DECAY  15 0.000000e+00
 DECAY  23 2.441404e+00 
 DECAY  24 2.047600e+00 
-DECAY  25 6.38233934e-03 
+DECAY  25 6.38233934e-03
 
 ###################################
 ## INFORMATION FOR WOLFENSTEIN
 ###################################
 Block Wolfenstein 
     1 0.000000e+00 # lamWS 
     2 0.000000e+00 # AWS 
     3 0.000000e+00 # rhoWS 
     4 0.000000e+00 # etaWS 
 
 ###################################
 ## INFORMATION FOR YUKAWA
 ###################################
 Block YUKAWA 
-    4 0.000000e+00 # ymc 
+    4 1.550000e+00 # ymc 
     5 4.700000e+00 # ymb
     6 1.730000e+02 # ymt
-   11 5.110000e-04 # yme
-   13 1.056600e-01 # ymm
+   11 0.000000e+00 # yme 
+   13 0.000000e+00 # ymm 
    15 1.777000e+00 # ymtau
```

### Comparing `gammaloop-0.0.1/python/gammaloop/data/models/sm/restrict_c_mass.dat` & `gammaloop-0.1.0/python/gammaloop/tests/test_data/models/loop_sm/restrict_ckm.dat`

 * *Files 9% similar despite different names*

```diff
@@ -1,24 +1,30 @@
 ######################################################################
 ## PARAM_CARD AUTOMATICALY GENERATED BY THE UFO  #####################
 ######################################################################
 
 ###################################
+### INFORMATION FOR LOOP
+####################################
+Block loop
+  1 9.118800e+01 # MU_R
+
+###################################
 ## INFORMATION FOR SMINPUTS
 ###################################
 Block SMINPUTS 
     1 1.325070e+02 # aEWM1 
     2 1.166390e-05 # Gf 
     3 1.180000e-01 # aS 
 
 ###################################
 ## INFORMATION FOR MASS
 ###################################
 Block MASS 
-    4 1.550000e+00 # MC 
+    4 0.000000e+00 # MC 
     5 4.700000e+00 # MB 
     6 1.730000e+02 # MT 
    11 0.000000e+00 # Me 
    13 0.000000e+00 # MM 
    15 1.777000e+00 # MTA 
    23 9.118800e+01 # MZ 
    25 1.250000e+02 # MH 
@@ -26,28 +32,28 @@
 ###################################
 ## INFORMATION FOR DECAY
 ###################################
 DECAY   6 1.491500E+00
 DECAY  15 0.000000e+00
 DECAY  23 2.441404e+00 
 DECAY  24 2.047600e+00 
-DECAY  25 6.38233934e-03
+DECAY  25 6.38233934e-03 
 
 ###################################
 ## INFORMATION FOR WOLFENSTEIN
 ###################################
 Block Wolfenstein 
-    1 0.000000e+00 # lamWS 
-    2 0.000000e+00 # AWS 
-    3 0.000000e+00 # rhoWS 
-    4 0.000000e+00 # etaWS 
+    1 2.253000e-01 # lamWS 
+    2 8.080000e-01 # AWS 
+    3 1.320000e-01 # rhoWS 
+    4 3.410000e-01 # etaWS 
 
 ###################################
 ## INFORMATION FOR YUKAWA
 ###################################
 Block YUKAWA 
-    4 1.550000e+00 # ymc 
-    5 4.700000e+00 # ymb
-    6 1.730000e+02 # ymt
+    4 0.000000e+00 # ymc 
+    5 4.700000e+00 # ymb 
+    6 1.730000e+02 # ymt 
    11 0.000000e+00 # yme 
    13 0.000000e+00 # ymm 
    15 1.777000e+00 # ymtau
```

### Comparing `gammaloop-0.0.1/python/gammaloop/data/models/sm/restrict_ckm.dat` & `gammaloop-0.1.0/python/gammaloop/data/models/sm/restrict_ckm.dat`

 * *Files identical despite different names*

### Comparing `gammaloop-0.0.1/python/gammaloop/data/models/sm/restrict_default.dat` & `gammaloop-0.1.0/python/gammaloop/tests/test_data/models/loop_sm/restrict_default.dat`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,18 @@
 ######################################################################
 ## PARAM_CARD AUTOMATICALY GENERATED BY THE UFO  #####################
 ######################################################################
 
 ###################################
+### INFORMATION FOR LOOP
+####################################
+Block loop
+  1 9.118800e+01 # MU_R
+
+###################################
 ## INFORMATION FOR SMINPUTS
 ###################################
 Block SMINPUTS 
     1 1.325070e+02 # aEWM1 
     2 1.166390e-05 # Gf 
     3 1.180000e-01 # aS 
 
@@ -42,12 +48,12 @@
     4 0.000000e+00 # etaWS 
 
 ###################################
 ## INFORMATION FOR YUKAWA
 ###################################
 Block YUKAWA 
     4 0.000000e+00 # ymc 
-    5 4.700000e+00 # ymb
-    6 1.730000e+02 # ymt
+    5 4.700000e+00 # ymb 
+    6 1.730000e+02 # ymt 
    11 0.000000e+00 # yme 
    13 0.000000e+00 # ymm 
    15 1.777000e+00 # ymtau
```

### Comparing `gammaloop-0.0.1/python/gammaloop/data/models/sm/restrict_lepton_masses.dat` & `gammaloop-0.1.0/python/gammaloop/tests/test_data/models/loop_sm/restrict_lepton_masses.dat`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,18 @@
 ######################################################################
 ## PARAM_CARD AUTOMATICALY GENERATED BY THE UFO  #####################
 ######################################################################
 
 ###################################
+### INFORMATION FOR LOOP
+####################################
+Block loop
+  1 9.118800e+01 # MU_R
+
+###################################
 ## INFORMATION FOR SMINPUTS
 ###################################
 Block SMINPUTS 
     1 1.325070e+02 # aEWM1 
     2 1.166390e-05 # Gf 
     3 1.180000e-01 # aS
```

### Comparing `gammaloop-0.0.1/python/gammaloop/data/models/sm/restrict_no_b_mass.dat` & `gammaloop-0.1.0/python/gammaloop/data/models/sm/restrict_no_b_mass.dat`

 * *Files identical despite different names*

### Comparing `gammaloop-0.0.1/python/gammaloop/data/models/sm/restrict_no_masses.dat` & `gammaloop-0.1.0/python/gammaloop/data/models/sm/restrict_no_masses.dat`

 * *Files identical despite different names*

### Comparing `gammaloop-0.0.1/python/gammaloop/data/models/sm/restrict_no_tau_mass.dat` & `gammaloop-0.1.0/python/gammaloop/data/models/sm/restrict_no_tau_mass.dat`

 * *Files identical despite different names*

### Comparing `gammaloop-0.0.1/python/gammaloop/data/models/sm/restrict_no_widths.dat` & `gammaloop-0.1.0/python/gammaloop/data/models/sm/restrict_no_widths.dat`

 * *Files identical despite different names*

### Comparing `gammaloop-0.0.1/python/gammaloop/data/models/sm/restrict_zeromass_ckm.dat` & `gammaloop-0.1.0/python/gammaloop/data/models/sm/restrict_zeromass_ckm.dat`

 * *Files identical despite different names*

### Comparing `gammaloop-0.0.1/python/gammaloop/data/models/sm/run_write_param_card.py` & `gammaloop-0.1.0/python/gammaloop/data/models/sm/run_write_param_card.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,17 +1,19 @@
+# type: ignore
 #!/usr/bin/env python
 from __future__ import absolute_import
 from __future__ import print_function
 from six.moves import range
 
 import sys
 import os
 import importlib
 
 if '__main__' == __name__:
     dir_path = os.path.join(os.path.dirname(__file__))
-    sys.path.insert(0,os.path.join(dir_path,os.path.pardir))
-    pw = importlib.import_module('%s.%s'%(os.path.basename(dir_path),'write_param_card'))
+    sys.path.insert(0, os.path.join(dir_path, os.path.pardir))
+    pw = importlib.import_module('%s.%s' % (
+        os.path.basename(dir_path), 'write_param_card'))
     del sys.path[0]
 
     pw.ParamCardWriter('./param_card.dat', generic=True)
     print('write ./param_card.dat')
```

### Comparing `gammaloop-0.0.1/python/gammaloop/data/models/sm/vertices.py` & `gammaloop-0.1.0/python/gammaloop/data/models/sm/vertices.py`

 * *Files identical despite different names*

### Comparing `gammaloop-0.0.1/python/gammaloop/data/models/sm/write_param_card.py` & `gammaloop-0.1.0/python/gammaloop/data/models/sm/write_param_card.py`

 * *Files identical despite different names*

### Comparing `gammaloop-0.0.1/python/gammaloop/tests/test_data/qgraf_outputs/epem_a_ddx_NLO.py` & `gammaloop-0.1.0/python/gammaloop/tests/test_data/qgraf_outputs/epem_a_ddx_NLO.py`

 * *Files identical despite different names*

### Comparing `gammaloop-0.0.1/src/inspect.rs` & `gammaloop-0.1.0/src/inspect.rs`

 * *Files 14% similar despite different names*

```diff
@@ -2,23 +2,25 @@
 #[allow(unused_imports)]
 use log::{debug, error, info, trace, warn};
 use symbolica::numerical_integration::Sample;
 
 use crate::integrands::HasIntegrand;
 use crate::utils;
 use crate::Integrand;
+use crate::SamplingSettings;
 use crate::Settings;
 use lorentz_vector::LorentzVector;
+use num::traits::ToPrimitive;
 use num::Complex;
-use num_traits::ToPrimitive;
 
 pub fn inspect(
     settings: &Settings,
     integrand: &mut Integrand,
     mut pt: Vec<f64>,
+    _term: &[usize],
     mut force_radius: bool,
     is_momentum_space: bool,
     use_f128: bool,
 ) -> Complex<f64> {
     if integrand.get_n_dim() == pt.len() - 1 {
         force_radius = true;
     }
@@ -43,27 +45,35 @@
         pt.iter().map(|x| f128::f128::from(*x)).collect::<Vec<_>>()
     };
     let xs_f64 = xs_f128
         .iter()
         .map(|x| f128::f128::to_f64(x).unwrap())
         .collect::<Vec<_>>();
 
-    let eval = integrand.evaluate_sample(
-        &Sample::Continuous(
+    let sample = {
+        let cont_sample = Sample::Continuous(
             1.,
             if force_radius {
-                xs_f64.clone()[1..].iter().map(|x| *x).collect::<Vec<_>>()
+                xs_f64.clone()[1..].to_vec()
             } else {
                 xs_f64.clone()
             },
-        ),
-        1.,
-        1,
-        use_f128,
-    );
+        );
+        match &settings.sampling {
+            SamplingSettings::DiscreteGraphs(_) => {
+                let graph_id = _term[0];
+                Sample::Discrete(1., graph_id, Some(Box::new(cont_sample)))
+            }
+            _ => cont_sample,
+        }
+    };
+
+    let eval_result = integrand.evaluate_sample(&sample, 0., 1, use_f128, 0.0);
+    let eval = eval_result.integrand_result;
+
     info!(
         "\nFor input point xs: \n\n{}\n\nThe evaluation of integrand '{}' is:\n\n{}\n",
         format!(
             "( {} )",
             xs_f64
                 .iter()
                 .map(|&x| format!("{:.16}", x))
```

### Comparing `gammaloop-0.0.1/src/integrands.rs` & `gammaloop-0.1.0/src/integrands.rs`

 * *Files 24% similar despite different names*

```diff
@@ -1,40 +1,45 @@
+use crate::evaluation_result::{EvaluationMetaData, EvaluationResult};
+use crate::gammaloop_integrand::GammaLoopIntegrand;
 use crate::h_function_test::{HFunctionTestIntegrand, HFunctionTestSettings};
 use crate::observables::EventManager;
 use crate::utils::FloatLike;
-use crate::{utils, Settings};
+use crate::{utils, IntegratorSettings, Precision, Settings};
 use enum_dispatch::enum_dispatch;
 #[allow(unused_imports)]
 use log::{debug, error, info, trace, warn};
 use lorentz_vector::LorentzVector;
 use num::Complex;
-use serde::Deserialize;
+use serde::{Deserialize, Serialize};
 use std::fmt::{Display, Formatter};
 use symbolica::numerical_integration::{ContinuousGrid, Grid, Sample};
 
-#[derive(Debug, Clone, Deserialize)]
+#[derive(Debug, Clone, Serialize, Deserialize)]
 #[allow(non_snake_case)]
 #[serde(tag = "type")]
 pub enum IntegrandSettings {
     #[serde(rename = "unit_surface")]
     UnitSurface(UnitSurfaceSettings),
     #[serde(rename = "unit_volume")]
     UnitVolume(UnitVolumeSettings),
     #[serde(rename = "h_function_test")]
     HFunctionTest(HFunctionTestSettings),
+    #[serde(rename = "gamma_loop")]
+    GammaLoop,
 }
 
 impl Display for IntegrandSettings {
     fn fmt(&self, f: &mut Formatter<'_>) -> std::fmt::Result {
         match self {
             IntegrandSettings::UnitSurface(_) => write!(f, "unit_surface"),
             IntegrandSettings::UnitVolume(_) => write!(f, "unit_volume"),
             IntegrandSettings::HFunctionTest(_) => {
                 write!(f, "h_function_test")
             }
+            IntegrandSettings::GammaLoop => write!(f, "gamma_loop"),
         }
     }
 }
 
 impl Default for IntegrandSettings {
     fn default() -> IntegrandSettings {
         IntegrandSettings::UnitSurface(UnitSurfaceSettings { n_3d_momenta: 1 })
@@ -42,91 +47,106 @@
 }
 
 #[enum_dispatch]
 pub trait HasIntegrand {
     fn create_grid(&self) -> Grid<f64>;
 
     fn evaluate_sample(
-        &mut self,
+        &self,
         sample: &Sample<f64>,
         wgt: f64,
         iter: usize,
         use_f128: bool,
-    ) -> Complex<f64>;
+        max_eval: f64,
+    ) -> EvaluationResult;
 
     fn get_n_dim(&self) -> usize;
 
+    fn get_integrator_settings(&self) -> IntegratorSettings {
+        IntegratorSettings::default()
+    }
+
     // In case your integrand supports observable, then overload this function to combine the observables
     fn merge_results<I: HasIntegrand>(&mut self, _other: &mut I, _iter: usize) {}
 
     // In case your integrand supports observable, then overload this function to write the observables to file
     fn update_results(&mut self, _iter: usize) {}
 
     // In case your integrand has an EventManager, overload this function to return it
     fn get_event_manager_mut(&mut self) -> &mut EventManager {
         panic!("This integrand does not have an EventManager");
     }
 }
 
 #[enum_dispatch(HasIntegrand)]
+#[derive(Clone)]
 pub enum Integrand {
     UnitSurface(UnitSurfaceIntegrand),
     UnitVolume(UnitVolumeIntegrand),
     HFunctionTest(HFunctionTestIntegrand),
+    GammaLoopIntegrand(GammaLoopIntegrand),
 }
 
 pub fn integrand_factory(settings: &Settings) -> Integrand {
     match settings.hard_coded_integrand.clone() {
         IntegrandSettings::UnitSurface(integrand_settings) => Integrand::UnitSurface(
             UnitSurfaceIntegrand::new(settings.clone(), integrand_settings),
         ),
         IntegrandSettings::UnitVolume(integrand_settings) => Integrand::UnitVolume(
             UnitVolumeIntegrand::new(settings.clone(), integrand_settings),
         ),
         IntegrandSettings::HFunctionTest(integrand_settings) => Integrand::HFunctionTest(
             HFunctionTestIntegrand::new(settings.clone(), integrand_settings),
         ),
+        IntegrandSettings::GammaLoop => {
+            unimplemented!("unsupported integrand construction method, please use the exporter to generate the integrand");
+        }
     }
 }
 
-#[derive(Debug, Clone, Default, Deserialize)]
+#[derive(Debug, Clone, Default, Serialize, Deserialize)]
 pub struct UnitSurfaceSettings {
     pub n_3d_momenta: usize,
 }
 
+#[derive(Clone)]
 pub struct UnitSurfaceIntegrand {
     pub settings: Settings,
     pub n_dim: usize,
     pub n_3d_momenta: usize,
     pub surface: f64,
 }
 
 #[allow(unused)]
 impl UnitSurfaceIntegrand {
     pub fn new(
         settings: Settings,
         integrand_settings: UnitSurfaceSettings,
     ) -> UnitSurfaceIntegrand {
-        let n_dim =
-            utils::get_n_dim_for_n_loop_momenta(&settings, integrand_settings.n_3d_momenta, true);
+        let n_dim = utils::get_n_dim_for_n_loop_momenta(
+            &settings,
+            integrand_settings.n_3d_momenta,
+            true,
+            None,
+        );
         let surface = utils::compute_surface_and_volume(
             integrand_settings.n_3d_momenta * 3 - 1,
             settings.kinematics.e_cm,
         )
         .0;
         UnitSurfaceIntegrand {
             settings,
             n_3d_momenta: integrand_settings.n_3d_momenta,
-            n_dim: n_dim,
-            surface: surface,
+            n_dim,
+            surface,
         }
     }
 
     fn evaluate_numerator<T: FloatLike>(&self, loop_momenta: &[LorentzVector<T>]) -> T {
-        return T::from_f64(1.0).unwrap();
+        T::from_f64(1.0).unwrap()
     }
 
     fn parameterize<T: FloatLike>(&self, xs: &[T]) -> (Vec<[T; 3]>, T) {
         utils::global_parameterize(
             xs,
             Into::<T>::into(self.settings.kinematics.e_cm * self.settings.kinematics.e_cm),
             &self.settings,
@@ -144,40 +164,49 @@
             self.settings.integrator.min_samples_for_update,
             self.settings.integrator.bin_number_evolution.clone(),
             self.settings.integrator.train_on_avg,
         ))
     }
 
     fn get_n_dim(&self) -> usize {
-        return self.n_dim;
+        self.n_dim
     }
 
     fn evaluate_sample(
-        &mut self,
+        &self,
         sample: &Sample<f64>,
         wgt: f64,
         iter: usize,
         use_f128: bool,
-    ) -> Complex<f64> {
+        max_eval: f64,
+    ) -> EvaluationResult {
+        let start_evaluate_sample = std::time::Instant::now();
+
         let xs = match sample {
             Sample::Continuous(_w, v) => v,
             _ => panic!("Wrong sample type"),
         };
         let mut sample_xs = vec![self.settings.kinematics.e_cm];
         sample_xs.extend(xs);
+
+        let before_parameterization = std::time::Instant::now();
         let (moms, jac) = self.parameterize(sample_xs.as_slice());
         let mut loop_momenta = vec![];
         for m in &moms {
             loop_momenta.push(LorentzVector {
                 t: ((m[0] + m[1] + m[2]) * (m[0] + m[1] + m[2])).sqrt(),
                 x: m[0],
                 y: m[1],
                 z: m[2],
             });
         }
+
+        let parameterization_time = before_parameterization.elapsed();
+
+        let before_evaluation = std::time::Instant::now();
         let mut itg_wgt = self.evaluate_numerator(loop_momenta.as_slice());
         // Normalize the integral
         itg_wgt /= self.surface;
         if self.settings.general.debug > 1 {
             info!("Sampled loop momenta:");
             for (i, l) in loop_momenta.iter().enumerate() {
                 info!(
@@ -190,59 +219,83 @@
                 );
             }
             info!("Integrator weight : {:+.16e}", wgt);
             info!("Integrand weight  : {:+.16e}", itg_wgt);
             info!("Sampling jacobian : {:+.16e}", jac);
             info!("Final contribution: {:+.16e}", itg_wgt * jac);
         }
-        return Complex::new(itg_wgt, 0.) * jac;
+
+        let is_nan = itg_wgt.is_nan();
+
+        let evaluation_time = before_evaluation.elapsed();
+
+        let evaluation_metadata = EvaluationMetaData {
+            total_timing: start_evaluate_sample.elapsed(),
+            rep3d_evaluation_time: evaluation_time,
+            parameterization_time,
+            relative_instability_error: Complex::new(0., 0.),
+            highest_precision: Precision::Double,
+            is_nan,
+        };
+
+        EvaluationResult {
+            integrand_result: Complex::new(itg_wgt, 0.) * jac,
+            integrator_weight: wgt,
+            event_buffer: vec![],
+            evaluation_metadata,
+        }
     }
 }
 
-#[derive(Debug, Clone, Default, Deserialize)]
+#[derive(Debug, Clone, Default, Serialize, Deserialize)]
 pub struct UnitVolumeSettings {
     pub n_3d_momenta: usize,
 }
 
+#[derive(Clone)]
 pub struct UnitVolumeIntegrand {
     pub settings: Settings,
     pub n_dim: usize,
     pub n_3d_momenta: usize,
     pub volume: f64,
 }
 
 #[allow(unused)]
 impl UnitVolumeIntegrand {
     pub fn new(settings: Settings, integrand_settings: UnitVolumeSettings) -> UnitVolumeIntegrand {
-        let n_dim =
-            utils::get_n_dim_for_n_loop_momenta(&settings, integrand_settings.n_3d_momenta, false);
+        let n_dim = utils::get_n_dim_for_n_loop_momenta(
+            &settings,
+            integrand_settings.n_3d_momenta,
+            false,
+            None,
+        );
         let volume = utils::compute_surface_and_volume(
             integrand_settings.n_3d_momenta * 3,
             settings.kinematics.e_cm,
         )
         .1;
         UnitVolumeIntegrand {
             settings,
             n_3d_momenta: integrand_settings.n_3d_momenta,
-            n_dim: n_dim,
-            volume: volume,
+            n_dim,
+            volume,
         }
     }
 
     fn evaluate_numerator<T: FloatLike>(&self, loop_momenta: &[LorentzVector<T>]) -> T {
         if loop_momenta
             .iter()
             .map(|l| l.spatial_squared())
             .sum::<T>()
             .sqrt()
             > Into::<T>::into(self.settings.kinematics.e_cm)
         {
-            return T::from_f64(0.0).unwrap();
+            T::from_f64(0.0).unwrap()
         } else {
-            return T::from_f64(1.0).unwrap();
+            T::from_f64(1.0).unwrap()
         }
     }
 
     fn parameterize<T: FloatLike>(&self, xs: &[T]) -> (Vec<[T; 3]>, T) {
         utils::global_parameterize(
             xs,
             Into::<T>::into(self.settings.kinematics.e_cm * self.settings.kinematics.e_cm),
@@ -261,38 +314,48 @@
             self.settings.integrator.min_samples_for_update,
             self.settings.integrator.bin_number_evolution.clone(),
             self.settings.integrator.train_on_avg,
         ))
     }
 
     fn get_n_dim(&self) -> usize {
-        return self.n_dim;
+        self.n_dim
     }
 
     fn evaluate_sample(
-        &mut self,
+        &self,
         sample: &Sample<f64>,
         wgt: f64,
         iter: usize,
         use_f128: bool,
-    ) -> Complex<f64> {
+        max_eval: f64,
+    ) -> EvaluationResult {
+        let start_evaluate_sample = std::time::Instant::now();
+
         let xs = match sample {
             Sample::Continuous(_w, v) => v,
             _ => panic!("Wrong sample type"),
         };
+
+        let before_parameterization = std::time::Instant::now();
+
         let (moms, jac) = self.parameterize(xs);
         let mut loop_momenta = vec![];
         for m in &moms {
             loop_momenta.push(LorentzVector {
                 t: 0.,
                 x: m[0],
                 y: m[1],
                 z: m[2],
             });
         }
+
+        let parameterization_time = before_parameterization.elapsed();
+
+        let before_evaluation = std::time::Instant::now();
         let mut itg_wgt = self.evaluate_numerator(loop_momenta.as_slice());
         // Normalize the integral
         itg_wgt /= self.volume;
         if self.settings.general.debug > 1 {
             info!("Sampled loop momenta:");
             for (i, l) in loop_momenta.iter().enumerate() {
                 info!(
@@ -305,10 +368,29 @@
                 );
             }
             info!("Integrator weight : {:+.16e}", wgt);
             info!("Integrand weight  : {:+.16e}", itg_wgt);
             info!("Sampling jacobian : {:+.16e}", jac);
             info!("Final contribution: {:+.16e}", itg_wgt * jac);
         }
-        return Complex::new(itg_wgt, 0.) * jac;
+
+        let is_nan = itg_wgt.is_nan();
+
+        let evaluation_time = before_evaluation.elapsed();
+
+        let evaluation_metadata = EvaluationMetaData {
+            total_timing: start_evaluate_sample.elapsed(),
+            rep3d_evaluation_time: evaluation_time,
+            parameterization_time,
+            relative_instability_error: Complex::new(0., 0.),
+            highest_precision: Precision::Double,
+            is_nan,
+        };
+
+        EvaluationResult {
+            integrand_result: Complex::new(itg_wgt, 0.) * jac,
+            integrator_weight: wgt,
+            event_buffer: vec![],
+            evaluation_metadata,
+        }
     }
 }
```

### Comparing `gammaloop-0.0.1/src/model.rs` & `gammaloop-0.1.0/src/model.rs`

 * *Files 23% similar despite different names*

```diff
@@ -1,16 +1,39 @@
+use crate::tensor::AbstractIndex;
 use crate::utils;
 use ahash::RandomState;
 use color_eyre::{Help, Report};
-use eyre::Context;
+use eyre::{eyre, Context};
+use num::Complex;
 use serde::{Deserialize, Serialize};
+use serde_yaml::Error;
 use smartstring::{LazyCompact, SmartString};
+use std::fs;
+use std::path::Path;
 use std::sync::Arc;
 use std::{collections::HashMap, fs::File};
-use symbolica::representations::Atom;
+use symbolica::fun;
+use symbolica::printer::{AtomPrinter, PrintOptions};
+use symbolica::representations::{Atom, FunctionBuilder};
+use symbolica::state::State;
+
+#[allow(unused)]
+fn normalise_complex(atom: &Atom) -> Atom {
+    let re = Atom::parse("re_").unwrap();
+    let im = Atom::parse("im_").unwrap();
+
+    let comp_id = State::get_symbol("complex");
+
+    let complexfn = fun!(comp_id, re, im).into_pattern();
+
+    let i = Atom::new_var(State::I);
+    let complexpanded = &re + i * &im;
+
+    complexfn.replace_all(atom.as_view(), &complexpanded.into_pattern(), None, None)
+}
 
 #[derive(Debug, Clone, Default, Serialize, Deserialize, PartialEq)]
 pub enum ParameterNature {
     #[default]
     #[serde(rename = "external")]
     External,
     #[serde(rename = "internal")]
@@ -32,29 +55,27 @@
     pub particles: Vec<SmartString<LazyCompact>>,
     pub color_structures: Vec<SmartString<LazyCompact>>,
     pub lorentz_structures: Vec<SmartString<LazyCompact>>,
     pub couplings: Vec<Vec<Option<SmartString<LazyCompact>>>>,
 }
 
 impl SerializableVertexRule {
-    pub fn from_vertex_rule(
-        vertex_rule: &VertexRule,
-        sb_state: &symbolica::state::State,
-    ) -> SerializableVertexRule {
+    pub fn from_vertex_rule(vertex_rule: &VertexRule) -> SerializableVertexRule {
         SerializableVertexRule {
             name: vertex_rule.name.clone(),
             particles: vertex_rule
                 .particles
                 .iter()
                 .map(|particle| particle.name.clone())
                 .collect(),
             color_structures: vertex_rule
                 .color_structures
                 .iter()
-                .map(|color_structure| utils::to_str_expression(color_structure, sb_state))
+                .map(utils::to_str_expression)
+                .map(SmartString::from)
                 .collect(),
             lorentz_structures: vertex_rule
                 .lorentz_structures
                 .iter()
                 .map(|lorentz_structure| lorentz_structure.name.clone())
                 .collect(),
             couplings: vertex_rule
@@ -67,45 +88,63 @@
                         .collect()
                 })
                 .collect(),
         }
     }
 }
 
+#[derive(Debug, Clone)]
+pub struct ColorStructure {
+    color_structure: Vec<Atom>,
+}
+
+impl ColorStructure {
+    pub fn new(color_structure: Vec<Atom>) -> Self {
+        ColorStructure { color_structure }
+    }
+
+    pub fn iter(&self) -> std::slice::Iter<Atom> {
+        self.color_structure.iter()
+    }
+}
+
+impl FromIterator<Atom> for ColorStructure {
+    fn from_iter<T: IntoIterator<Item = Atom>>(iter: T) -> Self {
+        ColorStructure {
+            color_structure: iter.into_iter().collect(),
+        }
+    }
+}
+
+#[derive(Debug, Clone)]
 pub struct VertexRule {
     pub name: SmartString<LazyCompact>,
     pub particles: Vec<Arc<Particle>>,
-    pub color_structures: Vec<Atom>,
+    pub color_structures: ColorStructure,
     pub lorentz_structures: Vec<Arc<LorentzStructure>>,
     pub couplings: Vec<Vec<Option<Arc<Coupling>>>>,
 }
 
 impl VertexRule {
     pub fn from_serializable_vertex_rule(
         model: &Model,
         vertex_rule: &SerializableVertexRule,
-        sb_state: &mut symbolica::state::State,
-        sb_workspace: &symbolica::state::Workspace,
     ) -> VertexRule {
         VertexRule {
             name: vertex_rule.name.clone(),
             particles: vertex_rule
                 .particles
                 .iter()
                 .map(|particle_name| model.get_particle(particle_name).clone())
                 .collect(),
             color_structures: vertex_rule
                 .color_structures
                 .iter()
                 .map(|color_structure_name| {
-                    utils::parse_python_expression(
-                        color_structure_name.as_str(),
-                        sb_state,
-                        sb_workspace,
-                    )
+                    utils::parse_python_expression(color_structure_name.as_str())
                 })
                 .collect(),
             lorentz_structures: vertex_rule
                 .lorentz_structures
                 .iter()
                 .map(|lorentz_structure_name| {
                     model.get_lorentz_structure(lorentz_structure_name).clone()
@@ -116,351 +155,428 @@
                 .iter()
                 .map(|coupling_names| {
                     coupling_names
                         .iter()
                         .map(|coupling_name| {
                             coupling_name
                                 .as_ref()
-                                .map(|cpl_name| model.get_coupling(&cpl_name))
+                                .map(|cpl_name| model.get_coupling(cpl_name))
                         })
                         .collect()
                 })
                 .collect(),
         }
     }
 }
 
 #[derive(Debug, Clone, Serialize, Deserialize)]
+pub struct SerializablePropagator {
+    pub name: SmartString<LazyCompact>,
+    pub particle: SmartString<LazyCompact>,
+    pub numerator: SmartString<LazyCompact>,
+    pub denominator: SmartString<LazyCompact>,
+}
+
+impl SerializablePropagator {
+    pub fn from_propagator(propagator: &Propagator) -> SerializablePropagator {
+        SerializablePropagator {
+            name: propagator.name.clone(),
+            particle: propagator.particle.name.clone(),
+            numerator: utils::to_str_expression(&propagator.numerator).into(),
+            denominator: utils::to_str_expression(&propagator.denominator).into(),
+        }
+    }
+}
+
+#[derive(Debug, Clone)]
+pub struct Propagator {
+    pub name: SmartString<LazyCompact>,
+    pub particle: Arc<Particle>,
+    pub numerator: Atom,
+    pub denominator: Atom,
+}
+
+impl Propagator {
+    pub fn from_serializable_propagator(
+        model: &Model,
+        propagator: &SerializablePropagator,
+    ) -> Propagator {
+        Propagator {
+            name: propagator.name.clone(),
+            particle: model.get_particle(&propagator.particle).clone(),
+            numerator: utils::parse_python_expression(propagator.numerator.as_str()),
+            denominator: utils::parse_python_expression(propagator.denominator.as_str()),
+        }
+    }
+}
+
+#[derive(Debug, Clone, Serialize, Deserialize)]
 pub struct SerializableCoupling {
     name: SmartString<LazyCompact>,
     expression: SmartString<LazyCompact>,
     #[serde(with = "vectorize")]
     orders: HashMap<SmartString<LazyCompact>, usize, RandomState>,
+    value: Option<(f64, f64)>,
 }
 
 impl SerializableCoupling {
-    pub fn from_coupling(
-        coupling: &Coupling,
-        sb_state: &symbolica::state::State,
-    ) -> SerializableCoupling {
+    pub fn from_coupling(coupling: &Coupling) -> SerializableCoupling {
         SerializableCoupling {
             name: coupling.name.clone(),
-            expression: utils::to_str_expression(&coupling.expression, sb_state),
+            expression: utils::to_str_expression(&coupling.expression).into(),
             orders: coupling.orders.clone(),
+            value: coupling.value.map(|value| (value.re, value.im)),
         }
     }
 }
 
+#[derive(Debug, Clone)]
 pub struct Coupling {
-    name: SmartString<LazyCompact>,
-    expression: Atom,
-    orders: HashMap<SmartString<LazyCompact>, usize, RandomState>,
+    pub name: SmartString<LazyCompact>,
+    pub expression: Atom,
+    pub orders: HashMap<SmartString<LazyCompact>, usize, RandomState>,
+    pub value: Option<Complex<f64>>,
 }
 
 impl Coupling {
-    pub fn from_serializable_coupling(
-        coupling: &SerializableCoupling,
-        sb_state: &mut symbolica::state::State,
-        sb_workspace: &symbolica::state::Workspace,
-    ) -> Coupling {
+    pub fn from_serializable_coupling(coupling: &SerializableCoupling) -> Coupling {
         Coupling {
             name: coupling.name.clone(),
-            expression: utils::parse_python_expression(
-                coupling.expression.as_str(),
-                sb_state,
-                sb_workspace,
-            ),
+            expression: utils::parse_python_expression(coupling.expression.as_str()),
             orders: coupling.orders.clone(),
+            value: coupling.value.map(|value| Complex::new(value.0, value.1)),
         }
     }
+
+    pub fn rep_rule(&self) -> [Atom; 2] {
+        let lhs = Atom::parse(&self.name).unwrap();
+        //let rhs = normalise_complex(&self.expression);
+        let rhs = self.expression.clone();
+
+        [lhs, rhs]
+    }
 }
 
 #[derive(Debug, Clone, Serialize, Deserialize)]
 pub struct SerializableParticle {
     pdg_code: isize,
     name: SmartString<LazyCompact>,
     antiname: SmartString<LazyCompact>,
-    spin: usize,
+    spin: isize,
     color: isize,
     mass: SmartString<LazyCompact>,
     width: SmartString<LazyCompact>,
     texname: SmartString<LazyCompact>,
     antitexname: SmartString<LazyCompact>,
     charge: f64,
     ghost_number: isize,
     lepton_number: isize,
-    y: isize,
+    y_charge: isize,
 }
 
 impl SerializableParticle {
     pub fn from_particle(particle: &Particle) -> SerializableParticle {
         SerializableParticle {
-            pdg_code: particle.pdg_code.clone(),
+            pdg_code: particle.pdg_code,
             name: particle.name.clone(),
             antiname: particle.antiname.clone(),
-            spin: particle.spin.clone(),
-            color: particle.color.clone(),
+            spin: particle.spin,
+            color: particle.color,
             mass: particle.mass.name.clone(),
             width: particle.width.name.clone(),
             texname: particle.texname.clone(),
             antitexname: particle.antitexname.clone(),
-            charge: particle.charge.clone(),
-            ghost_number: particle.ghost_number.clone(),
-            lepton_number: particle.lepton_number.clone(),
-            y: particle.y.clone(),
+            charge: particle.charge,
+            ghost_number: particle.ghost_number,
+            lepton_number: particle.lepton_number,
+            y_charge: particle.y_charge,
         }
     }
 }
 
-#[derive(Clone)]
+#[derive(Debug, Clone)]
 pub struct Particle {
-    pdg_code: isize,
-    name: SmartString<LazyCompact>,
-    antiname: SmartString<LazyCompact>,
-    spin: usize,
-    color: isize,
-    mass: Arc<Parameter>,
-    width: Arc<Parameter>,
-    texname: SmartString<LazyCompact>,
-    antitexname: SmartString<LazyCompact>,
-    charge: f64,
-    ghost_number: isize,
-    lepton_number: isize,
-    y: isize,
+    pub pdg_code: isize,
+    pub name: SmartString<LazyCompact>,
+    pub antiname: SmartString<LazyCompact>,
+    pub spin: isize,
+    pub color: isize,
+    pub mass: Arc<Parameter>,
+    pub width: Arc<Parameter>,
+    pub texname: SmartString<LazyCompact>,
+    pub antitexname: SmartString<LazyCompact>,
+    pub charge: f64,
+    pub ghost_number: isize,
+    pub lepton_number: isize,
+    pub y_charge: isize,
 }
 
 impl Particle {
     pub fn from_serializable_particle(model: &Model, particle: &SerializableParticle) -> Particle {
         Particle {
-            pdg_code: particle.pdg_code.clone(),
+            pdg_code: particle.pdg_code,
             name: particle.name.clone(),
             antiname: particle.antiname.clone(),
-            spin: particle.spin.clone(),
-            color: particle.color.clone(),
+            spin: particle.spin,
+            color: particle.color,
             mass: model.get_parameter(&particle.mass),
             width: model.get_parameter(&particle.width),
             texname: particle.texname.clone(),
             antitexname: particle.antitexname.clone(),
-            charge: particle.charge.clone(),
-            ghost_number: particle.ghost_number.clone(),
-            lepton_number: particle.lepton_number.clone(),
-            y: particle.y.clone(),
+            charge: particle.charge,
+            ghost_number: particle.ghost_number,
+            lepton_number: particle.lepton_number,
+            y_charge: particle.y_charge,
+        }
+    }
+
+    pub fn incoming_polarization_atom(&self, num: usize) -> Atom {
+        let id = AbstractIndex::try_from(format!("in{}", num)).unwrap().0;
+        match self.spin {
+            1 => Atom::parse("1").unwrap(),
+            2 => {
+                if self.pdg_code > 0 {
+                    Atom::parse(&format!("u{num}(bis(4,{id}))")).unwrap()
+                } else {
+                    Atom::parse(&format!("vbar{num}(bis(4,{id}))")).unwrap()
+                }
+            }
+            3 => Atom::parse(&format!("ϵ{num}(lor(4,{id}))")).unwrap(),
+            _ => Atom::parse("1").unwrap(),
+        }
+    }
+
+    pub fn outgoing_polarization_atom(&self, num: usize) -> Atom {
+        let id = AbstractIndex::try_from(format!("out{}", num)).unwrap().0;
+        match self.spin {
+            1 => Atom::parse("1").unwrap(),
+            2 => {
+                if self.pdg_code > 0 {
+                    Atom::parse(&format!("ubar{num}(bis(4,{id}))")).unwrap()
+                } else {
+                    Atom::parse(&format!("v{num}(bis(4,{id}))")).unwrap()
+                }
+            }
+            3 => Atom::parse(&format!("ϵbar{num}(lor(4,{id}))")).unwrap(),
+            _ => Atom::parse("1").unwrap(),
         }
     }
 }
 
 #[derive(Debug, Clone, Serialize, Deserialize)]
 pub struct SerializableLorentzStructure {
     name: SmartString<LazyCompact>,
-    spins: Vec<usize>,
+    spins: Vec<isize>,
     structure: SmartString<LazyCompact>,
 }
 
 impl SerializableLorentzStructure {
-    pub fn from_lorentz_structure(
-        ls: &LorentzStructure,
-        sb_state: &symbolica::state::State,
-    ) -> SerializableLorentzStructure {
+    pub fn from_lorentz_structure(ls: &LorentzStructure) -> SerializableLorentzStructure {
         SerializableLorentzStructure {
             name: ls.name.clone(),
             spins: ls.spins.clone(),
-            structure: utils::to_str_expression(&ls.structure, sb_state),
+            structure: utils::to_str_expression(&ls.structure).into(),
         }
     }
 }
 
+#[derive(Debug, Clone)]
 pub struct LorentzStructure {
-    name: SmartString<LazyCompact>,
-    spins: Vec<usize>,
-    structure: Atom,
+    pub name: SmartString<LazyCompact>,
+    pub spins: Vec<isize>,
+    pub structure: Atom,
 }
 
 impl LorentzStructure {
     pub fn from_serializable_lorentz_structure(
         ls: &SerializableLorentzStructure,
-        sb_state: &mut symbolica::state::State,
-        sb_workspace: &symbolica::state::Workspace,
     ) -> LorentzStructure {
         LorentzStructure {
             name: ls.name.clone(),
             spins: ls.spins.clone(),
-            structure: utils::parse_python_expression(
-                ls.structure.as_str(),
-                sb_state,
-                sb_workspace,
-            ),
+            structure: utils::parse_python_expression(ls.structure.as_str()),
         }
     }
 }
 
 #[derive(Debug, Clone, Serialize, Deserialize)]
 pub struct SerializableParameter {
     name: SmartString<LazyCompact>,
     lhablock: Option<SmartString<LazyCompact>>,
     lhacode: Option<Vec<usize>>,
     nature: ParameterNature,
     parameter_type: ParameterType,
-    value: Option<f64>,
+    value: Option<(f64, f64)>,
     expression: Option<SmartString<LazyCompact>>,
 }
 
 impl SerializableParameter {
-    pub fn from_parameter(
-        param: &Parameter,
-        sb_state: &symbolica::state::State,
-    ) -> SerializableParameter {
+    pub fn from_parameter(param: &Parameter) -> SerializableParameter {
         SerializableParameter {
             name: param.name.clone(),
             lhablock: param.lhablock.clone(),
             lhacode: param.lhacode.clone(),
             nature: param.nature.clone(),
             parameter_type: param.parameter_type.clone(),
-            value: param.value.clone(),
+            value: param.value.map(|value| (value.re, value.im)),
             expression: param
                 .expression
                 .as_ref()
-                .map(|expr| utils::to_str_expression(expr, sb_state)),
+                .map(utils::to_str_expression)
+                .map(SmartString::from),
         }
     }
 }
 
+#[derive(Debug, Clone)]
 pub struct Parameter {
-    name: SmartString<LazyCompact>,
-    lhablock: Option<SmartString<LazyCompact>>,
-    lhacode: Option<Vec<usize>>,
-    nature: ParameterNature,
-    parameter_type: ParameterType,
-    value: Option<f64>,
-    expression: Option<Atom>,
+    pub name: SmartString<LazyCompact>,
+    pub lhablock: Option<SmartString<LazyCompact>>,
+    pub lhacode: Option<Vec<usize>>,
+    pub nature: ParameterNature,
+    pub parameter_type: ParameterType,
+    pub value: Option<Complex<f64>>,
+    pub expression: Option<Atom>,
 }
 
 impl Parameter {
-    pub fn from_serializable_parameter(
-        param: &SerializableParameter,
-        sb_state: &mut symbolica::state::State,
-        sb_workspace: &symbolica::state::Workspace,
-    ) -> Parameter {
+    pub fn from_serializable_parameter(param: &SerializableParameter) -> Parameter {
         Parameter {
             name: param.name.clone(),
             lhablock: param.lhablock.clone(),
             lhacode: param.lhacode.clone(),
             nature: param.nature.clone(),
             parameter_type: param.parameter_type.clone(),
-            value: param.value.clone(),
+            value: param.value.map(|value| Complex::new(value.0, value.1)),
             expression: param
                 .expression
                 .as_ref()
-                .map(|expr| utils::parse_python_expression(expr.as_str(), sb_state, sb_workspace)),
+                .map(|expr| utils::parse_python_expression(expr.as_str())),
         }
     }
+
+    pub fn rep_rule(&self) -> Option<[Atom; 2]> {
+        let lhs = Atom::parse(&self.name).unwrap();
+        let rhs = self.expression.clone();
+
+        //Some([lhs, normalise_complex(&rhs?)])
+        Some([lhs, rhs?])
+    }
 }
 #[derive(Debug, Clone, Serialize, Deserialize)]
 pub struct Order {
-    name: SmartString<LazyCompact>,
-    expansion_order: isize,
-    hierarchy: isize,
+    pub name: SmartString<LazyCompact>,
+    pub expansion_order: isize,
+    pub hierarchy: isize,
 }
 
 #[derive(Debug, Clone, Serialize, Deserialize)]
 pub struct SerializableModel {
     pub name: SmartString<LazyCompact>,
+    pub restriction: Option<SmartString<LazyCompact>>,
     orders: Vec<Order>,
     parameters: Vec<SerializableParameter>,
     particles: Vec<SerializableParticle>,
+    propagators: Vec<SerializablePropagator>,
     lorentz_structures: Vec<SerializableLorentzStructure>,
     couplings: Vec<SerializableCoupling>,
     vertex_rules: Vec<SerializableVertexRule>,
 }
 
 impl SerializableModel {
     pub fn from_file(file_path: String) -> Result<SerializableModel, Report> {
         let f = File::open(file_path.clone())
             .wrap_err_with(|| format!("Could not open model yaml file {}", file_path))
             .suggestion("Does the path exist?")?;
         serde_yaml::from_reader(f)
-            .wrap_err("Could not parse model yaml content")
+            .map_err(|e| eyre!(format!("Error parsing model yaml: {}", e)))
             .suggestion("Is it a correct yaml file")
     }
 
     pub fn from_yaml_str(yaml_str: String) -> Result<SerializableModel, Report> {
         serde_yaml::from_str(yaml_str.as_str())
-            .wrap_err("Could not parse model yaml content")
+            .map_err(|e| eyre!(format!("Error parsing model yaml: {}", e)))
             .suggestion("Is it a correct yaml file")
     }
 
-    pub fn from_model(model: Model, sb_state: &symbolica::state::State) -> SerializableModel {
+    pub fn from_model(model: &Model) -> SerializableModel {
         SerializableModel {
             name: model.name.clone(),
+            restriction: model.restriction.clone(),
             orders: model
                 .orders
                 .iter()
                 .map(|order| order.as_ref().clone())
                 .collect(),
             parameters: model
                 .parameters
                 .iter()
-                .map(|parameter| {
-                    SerializableParameter::from_parameter(parameter.as_ref(), sb_state)
-                })
+                .map(|parameter| SerializableParameter::from_parameter(parameter.as_ref()))
                 .collect(),
             particles: model
                 .particles
                 .iter()
                 .map(|particle| SerializableParticle::from_particle(particle.as_ref()))
                 .collect(),
+            propagators: model
+                .propagators
+                .iter()
+                .map(|propagator| SerializablePropagator::from_propagator(propagator.as_ref()))
+                .collect(),
             lorentz_structures: model
                 .lorentz_structures
                 .iter()
                 .map(|lorentz_structure| {
-                    SerializableLorentzStructure::from_lorentz_structure(
-                        lorentz_structure.as_ref(),
-                        sb_state,
-                    )
+                    SerializableLorentzStructure::from_lorentz_structure(lorentz_structure.as_ref())
                 })
                 .collect(),
             couplings: model
                 .couplings
                 .iter()
-                .map(|coupling| SerializableCoupling::from_coupling(coupling.as_ref(), sb_state))
+                .map(|coupling| SerializableCoupling::from_coupling(coupling.as_ref()))
                 .collect(),
             vertex_rules: model
                 .vertex_rules
                 .iter()
-                .map(|vertex_rule| {
-                    SerializableVertexRule::from_vertex_rule(vertex_rule.as_ref(), sb_state)
-                })
+                .map(|vertex_rule| SerializableVertexRule::from_vertex_rule(vertex_rule.as_ref()))
                 .collect(),
         }
     }
 }
 
+#[derive(Debug, Clone)]
 pub struct Model {
     pub name: SmartString<LazyCompact>,
-    orders: Vec<Arc<Order>>,
-    parameters: Vec<Arc<Parameter>>,
-    particles: Vec<Arc<Particle>>,
-    lorentz_structures: Vec<Arc<LorentzStructure>>,
-    couplings: Vec<Arc<Coupling>>,
-    vertex_rules: Vec<Arc<VertexRule>>,
-    order_name_to_position: HashMap<SmartString<LazyCompact>, usize, RandomState>,
-    parameter_name_to_position: HashMap<SmartString<LazyCompact>, usize, RandomState>,
-    lorentz_structure_name_to_position: HashMap<SmartString<LazyCompact>, usize, RandomState>,
-    particle_name_to_position: HashMap<SmartString<LazyCompact>, usize, RandomState>,
-    particle_pdg_to_position: HashMap<isize, usize, RandomState>,
-    coupling_name_to_position: HashMap<SmartString<LazyCompact>, usize, RandomState>,
-    vertex_rule_name_to_position: HashMap<SmartString<LazyCompact>, usize, RandomState>,
+    pub restriction: Option<SmartString<LazyCompact>>,
+    pub orders: Vec<Arc<Order>>,
+    pub parameters: Vec<Arc<Parameter>>,
+    pub particles: Vec<Arc<Particle>>,
+    pub propagators: Vec<Arc<Propagator>>,
+    pub lorentz_structures: Vec<Arc<LorentzStructure>>,
+    pub couplings: Vec<Arc<Coupling>>,
+    pub vertex_rules: Vec<Arc<VertexRule>>,
+    pub order_name_to_position: HashMap<SmartString<LazyCompact>, usize, RandomState>,
+    pub parameter_name_to_position: HashMap<SmartString<LazyCompact>, usize, RandomState>,
+    pub lorentz_structure_name_to_position: HashMap<SmartString<LazyCompact>, usize, RandomState>,
+    pub particle_name_to_position: HashMap<SmartString<LazyCompact>, usize, RandomState>,
+    pub particle_pdg_to_position: HashMap<isize, usize, RandomState>,
+    pub propagator_name_to_position: HashMap<SmartString<LazyCompact>, usize, RandomState>,
+    pub coupling_name_to_position: HashMap<SmartString<LazyCompact>, usize, RandomState>,
+    pub vertex_rule_name_to_position: HashMap<SmartString<LazyCompact>, usize, RandomState>,
 }
 
-impl Model {
-    pub fn default() -> Model {
+impl Default for Model {
+    fn default() -> Self {
         Model {
             name: SmartString::<LazyCompact>::from("ModelNotLoaded"),
+            restriction: None,
             orders: vec![],
             parameters: vec![],
             particles: vec![],
+            propagators: vec![],
             lorentz_structures: vec![],
             couplings: vec![],
             vertex_rules: vec![],
             order_name_to_position:
                 HashMap::<SmartString<LazyCompact>, usize, RandomState>::default(),
             parameter_name_to_position:
                 HashMap::<SmartString<LazyCompact>, usize, RandomState>::default(),
@@ -468,58 +584,96 @@
                 SmartString<LazyCompact>,
                 usize,
                 RandomState,
             >::default(),
             particle_name_to_position:
                 HashMap::<SmartString<LazyCompact>, usize, RandomState>::default(),
             particle_pdg_to_position: HashMap::<isize, usize, RandomState>::default(),
+            propagator_name_to_position:
+                HashMap::<SmartString<LazyCompact>, usize, RandomState>::default(),
             coupling_name_to_position:
                 HashMap::<SmartString<LazyCompact>, usize, RandomState>::default(),
             vertex_rule_name_to_position:
                 HashMap::<SmartString<LazyCompact>, usize, RandomState>::default(),
         }
     }
+}
+impl Model {
+    pub fn is_empty(&self) -> bool {
+        self.name == "ModelNotLoaded" || self.particles.is_empty()
+    }
+
+    pub fn export_coupling_replacement_rules(
+        &self,
+        export_root: &str,
+        print_ops: PrintOptions,
+    ) -> Result<(), Report> {
+        let path = Path::new(export_root).join("sources").join("model");
+
+        if !path.exists() {
+            fs::create_dir_all(&path)?;
+        }
+        let mut reps = Vec::new();
+
+        for cpl in self.couplings.iter() {
+            reps.push(
+                cpl.rep_rule()
+                    .map(|a| format!("{}", AtomPrinter::new_with_options(a.as_view(), print_ops))),
+            );
+        }
+
+        for para in self.parameters.iter() {
+            if let Some(rule) = para.rep_rule() {
+                reps.push(
+                    rule.map(|a| {
+                        format!("{}", AtomPrinter::new_with_options(a.as_view(), print_ops))
+                    }),
+                );
+            }
+        }
+
+        fs::write(
+            path.join("model_replacements.json"),
+            serde_json::to_string_pretty(&reps)?,
+        )?;
+
+        Ok(())
+    }
 
-    pub fn from_serializable_model(
-        serializable_model: SerializableModel,
-        sb_state: &mut symbolica::state::State,
-        sb_workspace: &symbolica::state::Workspace,
-    ) -> Model {
+    pub fn from_serializable_model(serializable_model: SerializableModel) -> Model {
         let mut model: Model = Model::default();
         model.name = serializable_model.name;
+        model.restriction = serializable_model.restriction;
 
         // Extract coupling orders
         model.orders = serializable_model
             .orders
             .iter()
             .enumerate()
             .map(|(i_order, serializable_order)| {
                 let order = Arc::new(Order {
                     name: serializable_order.name.clone(),
-                    expansion_order: serializable_order.expansion_order.clone(),
-                    hierarchy: serializable_order.hierarchy.clone(),
+                    expansion_order: serializable_order.expansion_order,
+                    hierarchy: serializable_order.hierarchy,
                 });
                 model
                     .order_name_to_position
                     .insert(order.name.clone(), i_order);
                 order
             })
             .collect();
 
         // Extract parameters
         model.parameters = serializable_model
             .parameters
             .iter()
             .enumerate()
             .map(|(i_param, serializable_param)| {
-                let parameter = Arc::new(Parameter::from_serializable_parameter(
-                    serializable_param,
-                    sb_state,
-                    sb_workspace,
-                ));
+                let parameter =
+                    Arc::new(Parameter::from_serializable_parameter(serializable_param));
                 model
                     .parameter_name_to_position
                     .insert(parameter.name.clone(), i_param);
                 parameter
             })
             .collect();
 
@@ -539,44 +693,57 @@
                 model
                     .particle_pdg_to_position
                     .insert(particle.pdg_code, i_part);
                 particle
             })
             .collect();
 
+        // Extract propagators
+
+        model.propagators = serializable_model
+            .propagators
+            .iter()
+            .enumerate()
+            .map(|(i_prop, serializable_propagator)| {
+                let propagator = Arc::new(Propagator::from_serializable_propagator(
+                    &model,
+                    serializable_propagator,
+                ));
+                model
+                    .propagator_name_to_position
+                    .insert(propagator.name.clone(), i_prop);
+                propagator
+            })
+            .collect();
+
         // Extract Lorentz structures
         model.lorentz_structures = serializable_model
             .lorentz_structures
             .iter()
             .enumerate()
             .map(|(i_lor, serializable_lorentz_structure)| {
                 let lorentz_structure =
                     Arc::new(LorentzStructure::from_serializable_lorentz_structure(
                         serializable_lorentz_structure,
-                        sb_state,
-                        sb_workspace,
                     ));
                 model
                     .lorentz_structure_name_to_position
                     .insert(lorentz_structure.name.clone(), i_lor);
                 lorentz_structure
             })
             .collect();
 
         // Extract couplings
         model.couplings = serializable_model
             .couplings
             .iter()
             .enumerate()
             .map(|(i_coupl, serializable_coupling)| {
-                let coupling = Arc::new(Coupling::from_serializable_coupling(
-                    serializable_coupling,
-                    sb_state,
-                    sb_workspace,
-                ));
+                let coupling =
+                    Arc::new(Coupling::from_serializable_coupling(serializable_coupling));
                 model
                     .coupling_name_to_position
                     .insert(coupling.name.clone(), i_coupl);
                 coupling
             })
             .collect();
 
@@ -585,99 +752,110 @@
             .vertex_rules
             .iter()
             .enumerate()
             .map(|(i_vr, serializable_vertex_rule)| {
                 let vertex_rule = Arc::new(VertexRule::from_serializable_vertex_rule(
                     &model,
                     serializable_vertex_rule,
-                    sb_state,
-                    sb_workspace,
                 ));
                 model
                     .vertex_rule_name_to_position
                     .insert(vertex_rule.name.clone(), i_vr);
                 vertex_rule
             })
             .collect();
 
         model
     }
 
-    pub fn from_file(
-        file_path: String,
-        sb_state: &mut symbolica::state::State,
-        sb_workspace: &symbolica::state::Workspace,
-    ) -> Result<Model, Report> {
-        SerializableModel::from_file(file_path).map(|serializable_model| {
-            Model::from_serializable_model(serializable_model, sb_state, sb_workspace)
-        })
-    }
-
-    pub fn from_yaml_str(
-        yaml_str: String,
-        sb_state: &mut symbolica::state::State,
-        sb_workspace: &symbolica::state::Workspace,
-    ) -> Result<Model, Report> {
-        SerializableModel::from_yaml_str(yaml_str).map(|serializable_model| {
-            Model::from_serializable_model(serializable_model, sb_state, sb_workspace)
-        })
+    pub fn to_serializable(&self) -> SerializableModel {
+        SerializableModel::from_model(self)
+    }
+
+    pub fn to_yaml(&self) -> Result<String, Error> {
+        serde_yaml::to_string(&self.to_serializable())
     }
 
+    pub fn from_file(file_path: String) -> Result<Model, Report> {
+        SerializableModel::from_file(file_path).map(Model::from_serializable_model)
+    }
+
+    pub fn from_yaml_str(yaml_str: String) -> Result<Model, Report> {
+        SerializableModel::from_yaml_str(yaml_str).map(Model::from_serializable_model)
+    }
+
+    #[inline]
     pub fn get_particle(&self, name: &SmartString<LazyCompact>) -> Arc<Particle> {
         if let Some(position) = self.particle_name_to_position.get(name) {
-            return self.particles[*position].clone();
+            self.particles[*position].clone()
         } else {
             panic!("Particle '{}' not found in model '{}'.", name, self.name);
         }
     }
+    #[inline]
     pub fn get_particle_from_pdg(&self, pdg: isize) -> Arc<Particle> {
         if let Some(position) = self.particle_pdg_to_position.get(&pdg) {
-            return self.particles[*position].clone();
+            self.particles[*position].clone()
         } else {
             panic!(
                 "Particle with PDG {} not found in model '{}'.",
                 pdg, self.name
             );
         }
     }
+
+    #[inline]
+    pub fn get_propagator(&self, name: &SmartString<LazyCompact>) -> Arc<Propagator> {
+        if let Some(position) = self.propagator_name_to_position.get(name) {
+            self.propagators[*position].clone()
+        } else {
+            panic!("Propagator '{}' not found in model '{}'.", name, self.name);
+        }
+    }
+
+    #[inline]
     pub fn get_parameter(&self, name: &SmartString<LazyCompact>) -> Arc<Parameter> {
         if let Some(position) = self.parameter_name_to_position.get(name) {
-            return self.parameters[*position].clone();
+            self.parameters[*position].clone()
         } else {
             panic!("Parameter '{}' not found in model '{}'.", name, self.name);
         }
     }
+    #[inline]
     pub fn get_order(&self, name: &SmartString<LazyCompact>) -> Arc<Order> {
         if let Some(position) = self.order_name_to_position.get(name) {
-            return self.orders[*position].clone();
+            self.orders[*position].clone()
         } else {
             panic!(
                 "Coupling order '{}' not found in model '{}'.",
                 name, self.name
             );
         }
     }
+    #[inline]
     pub fn get_lorentz_structure(&self, name: &SmartString<LazyCompact>) -> Arc<LorentzStructure> {
         if let Some(position) = self.lorentz_structure_name_to_position.get(name) {
-            return self.lorentz_structures[*position].clone();
+            self.lorentz_structures[*position].clone()
         } else {
             panic!(
                 "Lorentz structure '{}' not found in model '{}'.",
                 name, self.name
             );
         }
     }
+    #[inline]
     pub fn get_coupling(&self, name: &SmartString<LazyCompact>) -> Arc<Coupling> {
         if let Some(position) = self.coupling_name_to_position.get(name) {
-            return self.couplings[*position].clone();
+            self.couplings[*position].clone()
         } else {
             panic!("Coupling '{}' not found in model '{}'.", name, self.name);
         }
     }
+    #[inline]
     pub fn get_vertex_rule(&self, name: &SmartString<LazyCompact>) -> Arc<VertexRule> {
         if let Some(position) = self.vertex_rule_name_to_position.get(name) {
-            return self.vertex_rules[*position].clone();
+            self.vertex_rules[*position].clone()
         } else {
             panic!("Vertex rule '{}' not found in model '{}'.", name, self.name);
         }
     }
 }
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `gammaloop-0.0.1/src/observables.rs` & `gammaloop-0.1.0/src/observables.rs`

 * *Files 4% similar despite different names*

```diff
@@ -2,89 +2,89 @@
 use crate::Settings;
 use itertools::Itertools;
 use libc::{c_double, c_int, c_void};
 #[allow(unused_imports)]
 use log::{debug, error, info, trace, warn};
 use lorentz_vector::LorentzVector;
 use num::Complex;
-use serde::Deserialize;
+use serde::{Deserialize, Serialize};
 use smallvec::SmallVec;
 use std::fmt;
 use std::fs::File;
 use std::io::{BufWriter, Write};
 use std::path::Path;
 
-#[derive(Debug, Clone, Deserialize)]
+#[derive(Debug, Clone, Serialize, Deserialize)]
 #[allow(non_snake_case)]
 #[serde(tag = "type")]
 pub enum PhaseSpaceSelectorSettings {
     #[serde(rename = "jet")]
     Jet(JetSliceSettings),
     #[serde(rename = "ranged")]
     RangeFilter(RangeFilterSettings),
 }
 
-#[derive(Debug, Clone, Deserialize)]
+#[derive(Debug, Clone, Deserialize, Serialize)]
 #[allow(non_snake_case)]
 #[serde(tag = "type")]
 pub enum ObservableSettings {
     #[serde(rename = "jet1pt")]
     Jet1PT(Jet1PTSettings),
     #[serde(rename = "one_particle_obs")]
     SingleParticleObservable(SingleParticleObservableSettings),
     AFB(AFBSettings),
     #[serde(rename = "cross_section")]
     CrossSection,
 }
 
-#[derive(Debug, Clone, Deserialize)]
+#[derive(Debug, Clone, Serialize, Deserialize)]
 #[allow(non_snake_case)]
 pub struct RangeFilterSettings {
     pub pdgs: Vec<isize>,
     pub filter: FilterQuantity,
     pub min_value: f64,
     pub max_value: f64,
 }
 
-#[derive(Debug, Clone, Default, Deserialize)]
+#[derive(Debug, Clone, Default, Serialize, Deserialize)]
 #[allow(non_snake_case)]
 pub struct JetSliceSettings {
     pub min_jets: usize,
     pub max_jets: usize,
     pub min_j1pt: f64,
     pub max_j1pt: f64,
     pub dR: f64,
     pub min_jpt: f64,
     pub use_fastjet: bool,
 }
 
-#[derive(Debug, Clone, Default, Deserialize)]
+#[derive(Debug, Clone, Default, Serialize, Deserialize)]
 #[allow(non_snake_case)]
 pub struct Jet1PTSettings {
     pub x_min: f64,
     pub x_max: f64,
     pub dR: f64,
     pub min_jpt: f64,
     pub n_bins: usize,
     pub write_to_file: bool,
     pub filename: String,
     pub use_fastjet: bool,
 }
 
-#[derive(Debug, Clone, Default, Deserialize)]
+#[derive(Debug, Clone, Default, Serialize, Deserialize)]
 #[allow(non_snake_case)]
 pub struct AFBSettings {
     pub x_min: f64,
     pub x_max: f64,
     pub n_bins: usize,
     pub write_to_file: bool,
     pub filename: String,
 }
 
-#[derive(Debug, Clone, Deserialize)]
+#[derive(Debug, Clone, Serialize, Deserialize)]
 #[allow(non_snake_case)]
 pub struct SingleParticleObservableSettings {
     pub x_min: f64,
     pub x_max: f64,
     pub n_bins: usize,
     #[serde(default = "default_true")]
     pub write_to_file: bool,
@@ -103,15 +103,15 @@
     true
 }
 
 fn default_false() -> bool {
     false
 }
 
-#[derive(Debug, Copy, Clone, Deserialize, PartialEq)]
+#[derive(Debug, Copy, Clone, Serialize, Deserialize, PartialEq)]
 pub enum FilterQuantity {
     #[serde(rename = "E")]
     Energy,
     #[serde(rename = "CosTheta")]
     CosThetaP,
     #[serde(rename = "PT")]
     PT,
@@ -268,15 +268,15 @@
                             settings.write_to_file,
                             settings.filename.clone(),
                             settings.use_fastjet,
                         )));
                     }
                 }
                 ObservableSettings::CrossSection => {
-                    observables.push(Observables::CrossSection(CrossSectionObservable::new()));
+                    observables.push(Observables::CrossSection(CrossSectionObservable::default()));
                 }
                 ObservableSettings::AFB(settings) => {
                     if track_events {
                         observables.push(Observables::AFB(AFBObservable::new(
                             settings.x_min,
                             settings.x_max,
                             settings.n_bins,
@@ -309,15 +309,15 @@
         let mut selectors = vec![];
         for s in &settings.selectors {
             match s {
                 PhaseSpaceSelectorSettings::RangeFilter(settings) => {
                     selectors.push(Selectors::RangeFilter(RangedSelector::new(settings)));
                 }
                 PhaseSpaceSelectorSettings::Jet(settings) => {
-                    selectors.push(Selectors::Jet(JetSelector::new(&settings)));
+                    selectors.push(Selectors::Jet(JetSelector::new(settings)));
                 }
             }
         }
 
         EventManager {
             event_selector: selectors,
             observables,
@@ -358,15 +358,15 @@
 
     pub fn pass_selection(&mut self, event: &mut Event) -> bool {
         for f in &mut self.event_selector {
             if !f.process_event(event) {
                 return false;
             }
         }
-        return true;
+        true
     }
 
     pub fn add_event(&mut self, mut event: Event) -> bool {
         if !self.track_events && self.event_selector.is_empty() {
             return true;
         }
 
@@ -415,14 +415,15 @@
             o.update_result(self.event_group_counter, iter);
         }
     }
 
     pub fn update_live_result(&mut self) {
         for o in &mut self.observables {
             // for now, only live update the cross section
+            #[allow(clippy::single_match)]
             match o {
                 Observables::CrossSection(c) => c.update_live_result(),
                 _ => {}
             }
         }
     }
 
@@ -452,23 +453,88 @@
 
         self.event_group_counter += 1;
     }
 }
 
 #[derive(Default, Debug, Clone)]
 pub struct Event {
+    #[allow(clippy::type_complexity)]
     pub kinematic_configuration: (
         SmallVec<[LorentzVector<f64>; 2]>,
         SmallVec<[LorentzVector<f64>; 4]>,
     ),
     pub final_state_particle_ids: SmallVec<[isize; 5]>,
     pub integrand: Complex<f64>,
     pub weights: SmallVec<[f64; 1]>,
 }
 
+#[derive(Serialize, Deserialize)]
+pub struct SerializableEvent {
+    pub kinematic_configuration: (Vec<[f64; 4]>, Vec<[f64; 4]>),
+    pub final_state_particle_ids: Vec<isize>,
+    pub integrand: (f64, f64),
+    pub weights: Vec<f64>,
+}
+
+impl SerializableEvent {
+    pub fn from_event(event: &Event) -> Self {
+        let kinematic_configuration = (
+            event
+                .kinematic_configuration
+                .0
+                .iter()
+                .map(|k| [k.t, k.x, k.y, k.z])
+                .collect::<Vec<_>>(),
+            event
+                .kinematic_configuration
+                .1
+                .iter()
+                .map(|k| [k.t, k.x, k.y, k.z])
+                .collect::<Vec<_>>(),
+        );
+
+        let final_state_particle_ids = event.final_state_particle_ids.to_vec();
+        let integrand = (event.integrand.re, event.integrand.im);
+        let weights = event.weights.to_vec();
+
+        Self {
+            kinematic_configuration,
+            final_state_particle_ids,
+            integrand,
+            weights,
+        }
+    }
+
+    pub fn into_event(self) -> Event {
+        let kinematic_configuration = (
+            self.kinematic_configuration
+                .0
+                .iter()
+                .map(|k| LorentzVector::from_args(k[0], k[1], k[2], k[3]))
+                .collect::<SmallVec<[LorentzVector<f64>; 2]>>(),
+            self.kinematic_configuration
+                .1
+                .iter()
+                .map(|k| LorentzVector::from_args(k[0], k[1], k[2], k[3]))
+                .collect::<SmallVec<[LorentzVector<f64>; 4]>>(),
+        );
+
+        let final_state_particle_ids: SmallVec<[isize; 5]> = self.final_state_particle_ids.into();
+        let integrand = Complex::new(self.integrand.0, self.integrand.1);
+        let weights: SmallVec<[f64; 1]> = self.weights.into();
+
+        Event {
+            kinematic_configuration,
+            final_state_particle_ids,
+            integrand,
+            weights,
+        }
+    }
+}
+
 #[allow(unused)]
 pub enum Selectors {
     All(NoEventSelector),
     Jet(JetSelector),
     RangeFilter(RangedSelector),
 }
 
@@ -651,29 +717,29 @@
         //self.jet_structure.clear();
 
         // group jets based on their dR
         let ext = &event.kinematic_configuration.1;
 
         let index_offset = 2;
         if ext.len() == 5 {
-            let pt1 = ext[index_offset + 0].pt();
+            let pt1 = ext[index_offset].pt();
             let pt2 = ext[index_offset + 1].pt();
             let pt3 = ext[index_offset + 2].pt();
-            let dr12 = ext[index_offset + 0].delta_r(&ext[index_offset + 1]);
-            let dr13 = ext[index_offset + 0].delta_r(&ext[index_offset + 2]);
+            let dr12 = ext[index_offset].delta_r(&ext[index_offset + 1]);
+            let dr13 = ext[index_offset].delta_r(&ext[index_offset + 2]);
             let dr23 = ext[index_offset + 1].delta_r(&ext[index_offset + 2]);
 
             // we have at least 2 jets
             if dr12 < self.d_r {
-                let m12 = ext[index_offset + 0] + ext[index_offset + 1];
+                let m12 = ext[index_offset] + ext[index_offset + 1];
                 let pt12 = m12.pt();
                 self.ordered_pt.push(pt12);
                 self.ordered_pt.push(pt3);
             } else if dr13 < self.d_r {
-                let m13 = ext[index_offset + 0] + ext[index_offset + 2];
+                let m13 = ext[index_offset] + ext[index_offset + 2];
                 let pt13 = m13.pt();
                 self.ordered_pt.push(pt13);
                 self.ordered_pt.push(pt2);
             } else if dr23 < self.d_r {
                 let m23 = ext[index_offset + 1] + ext[index_offset + 2];
                 let pt23 = m23.pt();
                 self.ordered_pt.push(pt23);
@@ -725,15 +791,15 @@
         // if self.clustering.ordered_pt[0] > 30. {
         //     info!("Event: {:#?}", event);
         //     info!("clustering: {:#?}", self.clustering);
         //     panic!("Ordered pt too large!: {:?}", self.clustering.ordered_pt);
         // }
         self.clustering.ordered_pt.len() >= self.jet_selector_settings.min_jets
             && self.clustering.ordered_pt.len() <= self.jet_selector_settings.max_jets
-            && (self.clustering.ordered_pt.len() == 0
+            && (self.clustering.ordered_pt.is_empty()
                 || (self.clustering.ordered_pt[0] >= self.jet_selector_settings.min_j1pt
                     && (self.jet_selector_settings.max_j1pt < 0.0
                         || (self.clustering.ordered_pt[0] <= self.jet_selector_settings.max_j1pt))))
     }
 }
 
 #[allow(dead_code)]
@@ -794,28 +860,21 @@
     where
         Self: Sized;
 
     /// Produce the result (histogram, etc.) of the observable from all processed event groups.
     fn update_result(&mut self, total_events: usize, iter: usize);
 }
 
-#[derive(Debug, Clone)]
+#[derive(Debug, Clone, Default)]
 pub struct CrossSectionObservable {
     pub re: AverageAndErrorAccumulator,
     pub im: AverageAndErrorAccumulator,
 }
 
 impl CrossSectionObservable {
-    pub fn new() -> CrossSectionObservable {
-        CrossSectionObservable {
-            re: AverageAndErrorAccumulator::default(),
-            im: AverageAndErrorAccumulator::default(),
-        }
-    }
-
     pub fn add_sample(&mut self, integrand: Complex<f64>, integrator_weight: f64) {
         self.re.add_sample(integrand.re * integrator_weight);
         self.im.add_sample(integrand.im * integrator_weight);
     }
 
     /// Give a live update on a copy of the statistics
     pub fn update_live_result(&self) {
@@ -857,14 +916,15 @@
     bins: Vec<AverageAndErrorAccumulator>,
     write_to_file: bool,
     filename: String,
     num_events: usize,
 }
 
 impl Jet1PTObservable {
+    #[allow(clippy::too_many_arguments)]
     pub fn new(
         x_min: f64,
         x_max: f64,
         num_bins: usize,
         d_r: f64,
         min_jpt: f64,
         write_to_file: bool,
@@ -935,15 +995,15 @@
             b.sum *= scaling;
             b.sum_sq *= scaling * scaling;
             b.update_iter();
         }
 
         if self.write_to_file {
             let file_name = {
-                let split = self.filename.split(".").collect::<Vec<_>>();
+                let split = self.filename.split('.').collect::<Vec<_>>();
                 if split.len() == 1 {
                     format!("{}_iter_{}", self.filename, iter)
                 } else {
                     format!(
                         "{}_iter_{}.{}",
                         split.as_slice()[..split.len() - 1].join("."),
                         iter,
@@ -1078,15 +1138,15 @@
             b.sum *= scaling;
             b.sum_sq *= scaling * scaling;
             b.update_iter();
         }
 
         if self.write_to_file {
             let file_name = {
-                let split = self.filename.split(".").collect::<Vec<_>>();
+                let split = self.filename.split('.').collect::<Vec<_>>();
                 if split.len() == 1 {
                     format!("{}_iter_{}", self.filename, iter)
                 } else {
                     format!(
                         "{}_iter_{}.{}",
                         split.as_slice()[..split.len() - 1].join("."),
                         iter,
@@ -1141,14 +1201,15 @@
     pdgs: Vec<isize>,
     log_obs: bool,
     log_x_axis: bool,
     log_y_axis: bool,
 }
 
 impl SingleParticleObservable {
+    #[allow(clippy::too_many_arguments)]
     pub fn new(
         x_min: f64,
         x_max: f64,
         num_bins: usize,
         write_to_file: bool,
         filename: String,
         quantity: FilterQuantity,
@@ -1243,27 +1304,25 @@
             let scaling = b.num_samples as f64 / diff as f64;
             b.sum *= scaling;
             b.sum_sq *= scaling * scaling;
             b.update_iter();
         }
 
         //let title = format!("{}({})", self.quantity, self.pdgs.iter().map(|&pdg| pdg.to_string()).join(",") );
-        let title = format!(
-            "{}",
-            Path::new(&self.filename)
-                .file_stem()
-                .unwrap()
-                .to_str()
-                .unwrap()
-        );
+        let title = Path::new(&self.filename)
+            .file_stem()
+            .unwrap()
+            .to_str()
+            .unwrap()
+            .to_string();
         let x_axis_mode = if self.log_x_axis { "LOG" } else { "LIN" };
         let y_axis_mode = if self.log_y_axis { "LOG" } else { "LIN" };
         if self.write_to_file {
             let file_name = {
-                let split = self.filename.split(".").collect::<Vec<_>>();
+                let split = self.filename.split('.').collect::<Vec<_>>();
                 if split.len() == 1 {
                     format!("{}_iter_{}", self.filename, iter)
                 } else {
                     format!(
                         "{}_iter_{}.{}",
                         split.as_slice()[..split.len() - 1].join("."),
                         iter,
```

### Comparing `gammaloop-0.0.1/src/tests.rs` & `gammaloop-0.1.0/src/tests.rs`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,16 @@
-#![allow(dead_code)]
-use crate::*;
-#[allow(unused)]
+#![allow(unused)]
+use crate::integrands::IntegrandSettings;
+use crate::utils::{self, approx_eq};
 use crate::{
-    h_function_test::HFunctionTestSettings, integrands::UnitVolumeSettings,
-    observables::JetSliceSettings, observables::PhaseSpaceSelectorSettings,
+    h_function_test::HFunctionTestSettings, integrand_factory, integrands::UnitVolumeSettings,
+    observables::JetSliceSettings, observables::PhaseSpaceSelectorSettings, Complex,
+    IntegratedPhase, Settings,
 };
+use colored::Colorize;
 
 use crate::inspect::inspect;
 use crate::integrate::{havana_integrate, UserData};
 
 const CENTRAL_VALUE_TOLERANCE: f64 = 2.0e-2;
 const INSPECT_TOLERANCE: f64 = 1.0e-15;
 const DIFF_TARGET_TO_ERROR_MUST_BE_LESS_THAN: f64 = 3.;
@@ -16,25 +18,17 @@
 
 const N_CORES_FOR_INTEGRATION_IN_TESTS: usize = 16;
 
 fn load_default_settings() -> Settings {
     Settings::from_file("./src/test_resources/default_tests_config.yaml").unwrap()
 }
 
-fn approx_eq(res: f64, target: f64, tolerance: f64) -> bool {
-    if target == 0.0 {
-        return res.abs() < tolerance;
-    } else {
-        ((res - target) / target).abs() < tolerance
-    }
-}
-
 fn validate_error(error: f64, target_diff: f64) -> bool {
     if target_diff == 0.0 {
-        return true;
+        true
     } else {
         (error / target_diff).abs() < DIFF_TARGET_TO_ERROR_MUST_BE_LESS_THAN
     }
 }
 
 fn compare_integration(
     settings: &mut Settings,
@@ -46,25 +40,25 @@
         Some(t) => t,
         None => CENTRAL_VALUE_TOLERANCE,
     };
     // Allow this to fail as it may be called more than once
     rayon::ThreadPoolBuilder::new()
         .num_threads(N_CORES_FOR_INTEGRATION_IN_TESTS)
         .build_global()
-        .unwrap_or_else(|_| {});
+        .unwrap_or(());
 
     let user_data_generator = |settings: &Settings| UserData {
         integrand: (0..N_CORES_FOR_INTEGRATION_IN_TESTS)
             .map(|_i| crate::integrand_factory(settings))
             .collect(),
     };
     match phase {
         IntegratedPhase::Both => {
-            (*settings).integrator.integrated_phase = IntegratedPhase::Real;
-            let res = havana_integrate(&settings, user_data_generator, Some(target));
+            settings.integrator.integrated_phase = IntegratedPhase::Real;
+            let res = havana_integrate(settings, user_data_generator, Some(target), None, None);
             if !approx_eq(res.result[0], target.re, applied_tolerance)
                 || !validate_error(res.error[0], target.re - res.result[0])
             {
                 println!(
                     "Incorrect real part of result: {:-19} vs {:.16e}",
                     format!(
                         "{:-19}",
@@ -72,16 +66,16 @@
                     )
                     .red()
                     .bold(),
                     target.re
                 );
                 return false;
             }
-            (*settings).integrator.integrated_phase = IntegratedPhase::Imag;
-            let res = havana_integrate(&settings, user_data_generator, Some(target));
+            settings.integrator.integrated_phase = IntegratedPhase::Imag;
+            let res = havana_integrate(settings, user_data_generator, Some(target), None, None);
             if !approx_eq(res.result[1], target.im, applied_tolerance)
                 || !validate_error(res.error[1], target.re - res.result[1])
             {
                 println!(
                     "Incorrect imag part of result: {:-19} vs {:.16e}",
                     format!(
                         "{:-19}",
@@ -91,16 +85,16 @@
                     .bold(),
                     target.im
                 );
                 return false;
             }
         }
         IntegratedPhase::Real => {
-            (*settings).integrator.integrated_phase = IntegratedPhase::Real;
-            let res = havana_integrate(&settings, user_data_generator, Some(target));
+            settings.integrator.integrated_phase = IntegratedPhase::Real;
+            let res = havana_integrate(settings, user_data_generator, Some(target), None, None);
             if !approx_eq(res.result[0], target.re, applied_tolerance)
                 || !validate_error(res.error[0], target.im - res.result[0])
             {
                 println!(
                     "Incorrect real part of result: {:-19} vs {:.16e}",
                     format!(
                         "{:-19}",
@@ -110,16 +104,16 @@
                     .bold(),
                     target.re
                 );
                 return false;
             }
         }
         IntegratedPhase::Imag => {
-            (*settings).integrator.integrated_phase = IntegratedPhase::Imag;
-            let res = havana_integrate(&settings, user_data_generator, Some(target));
+            settings.integrator.integrated_phase = IntegratedPhase::Imag;
+            let res = havana_integrate(settings, user_data_generator, Some(target), None, None);
             if !approx_eq(res.result[1], target.im, applied_tolerance)
                 || !validate_error(res.error[1], target.im - res.result[1])
             {
                 println!(
                     "Incorrect imag part of result: {:-19} vs {:.16e}",
                     format!(
                         "{:-19}",
@@ -135,22 +129,24 @@
     }
     true
 }
 
 fn compare_inspect(
     settings: &mut Settings,
     pt: Vec<f64>,
+    term: &[usize],
     is_momentum_space: bool,
     target: Complex<f64>,
 ) -> bool {
-    let mut integrand = integrand_factory(&settings);
+    let mut integrand = integrand_factory(settings);
     let res = inspect(
-        &settings,
+        settings,
         &mut integrand,
         pt,
+        term,
         false,
         is_momentum_space,
         true,
     );
     if !approx_eq(res.re, target.re, INSPECT_TOLERANCE)
         || !approx_eq(res.im, target.im, INSPECT_TOLERANCE)
     {
@@ -159,15 +155,15 @@
             format!("{:+16e} + i {:+16e}", res.re, res.im).red().bold(),
             format!("{:.16e} + i {:+16e}", target.re, target.im)
                 .red()
                 .bold()
         );
         return false;
     }
-    return true;
+    true
 }
 
 fn get_h_function_test_integrand() -> HFunctionTestSettings {
     let parsed_itg = serde_yaml::from_str(
         "
     type: h_function_test
     h_function:
@@ -195,14 +191,16 @@
         IntegrandSettings::UnitVolume(itg) => itg,
         _ => panic!("Wrong type of integrand"),
     }
 }
 
 #[cfg(test)]
 mod tests_integral {
+    use crate::{HFunction, HFunctionSettings, ParameterizationMode};
+
     use super::*;
 
     #[test]
     fn unit_volume_11_momenta_hyperspherical_flat() {
         let mut settings = load_default_settings();
         let mut itg = get_unit_volume_integrand();
         settings.integrator.n_start = 5 * BASE_N_START_SAMPLE;
@@ -288,14 +286,16 @@
             None
         ));
     }
 }
 
 #[cfg(test)]
 mod tests_inspect {
+    use crate::{HFunction, HFunctionSettings, ParameterizationMode};
+
     use super::*;
 
     // Amazingly enough, a simple failing test induces a segfault on MacOS... :/
     // #[test]
     // fn this_test_will_not_pass() {
     //     assert!(false);
     // }
@@ -307,25 +307,27 @@
         itg.n_3d_momenta = 6;
         settings.kinematics.e_cm = 1.;
         settings.parameterization.mode = ParameterizationMode::Spherical;
         settings.hard_coded_integrand = IntegrandSettings::UnitVolume(itg.clone());
         assert!(compare_inspect(
             &mut settings,
             vec![0.1, 0.2, 0.3, 0.4, 0.5, 0.6],
+            &[0],
             true,
             Complex::new(1.3793965770302298e3, 0.0)
         ));
 
         itg.n_3d_momenta = 9;
         settings.kinematics.e_cm = 100.;
         settings.parameterization.mode = ParameterizationMode::HyperSpherical;
         settings.hard_coded_integrand = IntegrandSettings::UnitVolume(itg.clone());
         assert!(compare_inspect(
             &mut settings,
             vec![0.1, 0.2, 0.3, 0.4, 0.5, 0.6, 0.7, 0.8, 0.9],
+            &[0],
             true,
             Complex::new(4.792927924134406e-45, 0.0)
         ));
     }
 
     #[test]
     fn inspect_h_function_test() {
@@ -339,26 +341,28 @@
             power: Some(12),
             enabled_dampening: true,
         };
         settings.hard_coded_integrand = IntegrandSettings::HFunctionTest(itg.clone());
         assert!(compare_inspect(
             &mut settings,
             vec![0.2188450233532342,],
+            &[0],
             false,
             Complex::new(1.4016882047579115e-34, 0.0)
         ));
 
         itg.h_function = HFunctionSettings {
             function: HFunction::PolyLeftRightExponential,
             sigma: 0.3,
             power: Some(9),
             enabled_dampening: false,
         };
         settings.hard_coded_integrand = IntegrandSettings::HFunctionTest(itg.clone());
         assert!(compare_inspect(
             &mut settings,
             vec![0.2188450233532342,],
+            &[0],
             false,
             Complex::new(3.112977432926161e-4, 0.0)
         ));
     }
 }
```

### Comparing `gammaloop-0.0.1/src/utils.rs` & `gammaloop-0.1.0/src/utils.rs`

 * *Files 9% similar despite different names*

```diff
@@ -1,20 +1,23 @@
+use crate::SamplingSettings;
 use crate::{ParameterizationMapping, ParameterizationMode, Settings, MAX_LOOP};
 use colored::Colorize;
 use hyperdual::Hyperdual;
 use itertools::{izip, Itertools};
 use lorentz_vector::{Field, LorentzVector, RealNumberLike};
+use num::traits::{Float, FloatConst, FromPrimitive, Num, NumAssign, NumCast, Signed};
+use num::traits::{Inv, One, Zero};
 use num::Complex;
 use num::ToPrimitive;
-use num_traits::{Float, FloatConst, FromPrimitive, Num, NumAssign, NumCast, Signed};
-use num_traits::{Inv, One, Zero};
-use smartstring::{LazyCompact, SmartString};
+use serde::{Deserialize, Serialize};
 use statrs::function::gamma::{gamma, gamma_lr, gamma_ur};
 use std::cmp::{Ord, Ordering};
 use std::ops::Neg;
+use std::time::Duration;
+use symbolica::numerical_integration::Sample;
 
 #[allow(unused_imports)]
 use log::{debug, info};
 use symbolica::printer::{AtomPrinter, PrintOptions};
 use symbolica::representations::Atom;
 
 use git_version::git_version;
@@ -22,14 +25,29 @@
 pub const VERSION: &str = "0.0.1";
 
 #[allow(unused)]
 const MAX_DIMENSION: usize = MAX_LOOP * 3;
 
 pub const PINCH_TEST_THRESHOLD: f64 = 1e-10;
 
+pub const LEFT: usize = 0;
+pub const RIGHT: usize = 1;
+
+#[derive(Debug, Clone, Serialize, Deserialize, PartialEq)]
+pub enum Side {
+    LEFT = 0,
+    RIGHT = 1,
+}
+
+impl From<Side> for usize {
+    fn from(val: Side) -> Self {
+        val as usize
+    }
+}
+
 pub trait FloatConvertFrom<U> {
     fn convert_from(x: &U) -> Self;
 }
 
 impl FloatConvertFrom<f64> for f64 {
     fn convert_from(x: &f64) -> f64 {
         *x
@@ -132,60 +150,52 @@
 impl<I, J> ExactSizeIterator for ZipEq<I, J>
 where
     I: ExactSizeIterator,
     J: ExactSizeIterator,
 {
 }
 
-pub fn parse_python_expression(
-    expression: &str,
-    sb_state: &mut symbolica::state::State,
-    sb_workspace: &symbolica::state::Workspace,
-) -> Atom {
+pub fn parse_python_expression(expression: &str) -> Atom {
     let processed_string = String::from(expression)
         .replace("**", "^")
         .replace("cmath.sqrt", "sqrt")
         .replace("cmath.pi", "pi")
         .replace("math.sqrt", "sqrt")
         .replace("math.pi", "pi");
-    Atom::parse(processed_string.as_str(), sb_state, sb_workspace)
+    Atom::parse(processed_string.as_str())
         .map_err(|e| {
             format!(
                 "Failed to parse expression : '{}'\nError: {}",
-                processed_string,
-                e.to_string()
+                processed_string, e
             )
         })
         .unwrap()
 }
 
-pub fn to_str_expression(
-    expression: &Atom,
-    sb_state: &symbolica::state::State,
-) -> SmartString<LazyCompact> {
+pub fn to_str_expression(expression: &Atom) -> String {
     format!(
         "{}",
         AtomPrinter::new_with_options(
             expression.as_view(),
             PrintOptions {
                 terms_on_new_line: false,
+                color: false,
                 color_top_level_sum: false,
                 color_builtin_functions: false,
                 print_finite_field: false,
                 explicit_rational_polynomial: false,
+                symmetric_representation_for_finite_field: false,
                 number_thousands_separator: None,
                 multiplication_operator: '*',
                 square_brackets_for_function: false,
                 num_exp_as_superscript: false,
                 latex: false
             },
-            sb_state
         )
     )
-    .into()
 }
 
 /// Format a mean ± sdev as mean(sdev) with the correct number of digits.
 /// Based on the Python package gvar.
 pub fn format_uncertainty(mean: f64, sdev: f64) -> String {
     fn ndec(x: f64, offset: usize) -> i32 {
         let mut ans = (offset as f64 - x.log10()) as i32;
@@ -202,15 +212,15 @@
     let dv = sdev.abs();
 
     // special cases
     if v.is_nan() || dv.is_nan() {
         format!("{:e} ± {:e}", v, dv)
     } else if dv.is_infinite() {
         format!("{:e} ± inf", v)
-    } else if v == 0. && (dv >= 1e5 || dv < 1e-4) {
+    } else if v == 0. && !(1e-4..1e5).contains(&dv) {
         if dv == 0. {
             "0(0)".to_owned()
         } else {
             let e = format!("{:.1e}", dv);
             let mut ans = e.split('e');
             let e1 = ans.next().unwrap();
             let e2 = ans.next().unwrap();
@@ -305,34 +315,46 @@
     fn multiply_sign(&self, sign: i8) -> Self;
 }
 
 impl Signum for f128::f128 {
     #[inline]
     fn multiply_sign(&self, sign: i8) -> f128::f128 {
         match sign {
-            1 => self.clone(),
+            1 => *self,
             0 => f128::f128::zero(),
             -1 => self.neg(),
             _ => unreachable!("Sign should be -1,0,1"),
         }
     }
 }
 
 impl Signum for f64 {
     #[inline]
     fn multiply_sign(&self, sign: i8) -> f64 {
         match sign {
-            1 => self.clone(),
+            1 => *self,
             0 => f64::zero(),
             -1 => self.neg(),
             _ => unreachable!("Sign should be -1,0,1"),
         }
     }
 }
 
+impl Signum for f32 {
+    #[inline]
+    fn multiply_sign(&self, sign: i8) -> Self {
+        match sign {
+            1 => *self,
+            0 => f32::zero(),
+            -1 => self.neg(),
+            _ => unreachable!("Sign should be -1,0,1"),
+        }
+    }
+}
+
 impl<T: Num + Neg<Output = T> + Copy> Signum for Complex<T> {
     #[inline]
     fn multiply_sign(&self, sign: i8) -> Complex<T> {
         match sign {
             1 => *self,
             0 => Complex::zero(),
             -1 => Complex::new(-self.re, -self.im),
@@ -422,87 +444,87 @@
     delta_t: T,
     powers: (i32, i32),
     multiplier: f64,
 ) -> T {
     // Make sure the function is even in t-tstar
     assert!(powers.1 % 2 == 0);
     let a = dampening_arg.powi(powers.0);
-    return a / (a + Into::<T>::into(multiplier as f64) * delta_t.powi(powers.1));
+    a / (a + Into::<T>::into(multiplier) * delta_t.powi(powers.1))
 }
 
 pub fn h<T: FloatLike>(
     t: T,
     tstar: Option<T>,
     sigma: Option<T>,
     h_function_settings: &crate::HFunctionSettings,
 ) -> T {
     let sig = if let Some(s) = sigma {
         s
     } else {
-        Into::<T>::into(h_function_settings.sigma as f64)
+        Into::<T>::into(h_function_settings.sigma)
     };
     let power = h_function_settings.power;
     match h_function_settings.function {
         crate::HFunction::Exponential => {
-            (-(t * t) / (sig * sig)).exp() * Into::<T>::into(2 as f64)
+            (-(t * t) / (sig * sig)).exp() * Into::<T>::into(2_f64)
                 / (<T as FloatConst>::PI().sqrt() * sig)
         }
         crate::HFunction::PolyExponential => {
             // Result of \int_0^{\infty} dt (t/sigma)^{-p} exp(2-t^2/sigma^2-sigma^2/t^2)
             let normalisation = match power {
-                None | Some(0) => <T as FloatConst>::PI().sqrt() * sig / Into::<T>::into(2 as f64),
-                Some(1) => Into::<T>::into(0.84156821507077141791912486734584) * sig,
-                Some(3) => Into::<T>::into(1.0334768470686885731753571058796) * sig,
-                Some(4) => Into::<T>::into(1.3293403881791370204736256125059) * sig,
-                Some(6) => Into::<T>::into(2.8802375077214635443595221604294) * sig,
-                Some(7) => Into::<T>::into(4.7835669713476085553643210523305) * sig,
-                Some(9) => Into::<T>::into(16.225745976182285657187445130217) * sig,
-                Some(10) => Into::<T>::into(32.735007058911249129163030707957) * sig,
-                Some(12) => Into::<T>::into(155.83746592258341696260606919938) * sig,
-                Some(13) => Into::<T>::into(364.65850035656604157775795299621) * sig,
-                Some(15) => Into::<T>::into(2257.6375530154730006506618195504) * sig,
-                Some(16) => Into::<T>::into(5939.8044185378636927153327426791) * sig,
+                None | Some(0) => <T as FloatConst>::PI().sqrt() * sig / Into::<T>::into(2_f64),
+                Some(1) => Into::<T>::into(0.841_568_215_070_771_4) * sig,
+                Some(3) => Into::<T>::into(1.033_476_847_068_688_6) * sig,
+                Some(4) => Into::<T>::into(1.329_340_388_179_137) * sig,
+                Some(6) => Into::<T>::into(2.880_237_507_721_463_7) * sig,
+                Some(7) => Into::<T>::into(4.783_566_971_347_609) * sig,
+                Some(9) => Into::<T>::into(16.225_745_976_182_285) * sig,
+                Some(10) => Into::<T>::into(32.735_007_058_911_25) * sig,
+                Some(12) => Into::<T>::into(155.837_465_922_583_42) * sig,
+                Some(13) => Into::<T>::into(364.658_500_356_566_04) * sig,
+                Some(15) => Into::<T>::into(2_257.637_553_015_473) * sig,
+                Some(16) => Into::<T>::into(5_939.804_418_537_864) * sig,
                 _ => panic!(
                     "Value {} of power in poly exponential h function not supported",
                     power.unwrap()
                 ),
             };
             let prefactor = match power {
                 None | Some(0) => normalisation.inv(),
                 Some(p) => (t / sig).powi(-(p as i32)) / normalisation,
             };
             prefactor
-                * (Into::<T>::into(2 as f64) - (t * t) / (sig * sig) - (sig * sig) / (t * t)).exp()
+                * (Into::<T>::into(2_f64) - (t * t) / (sig * sig) - (sig * sig) / (t * t)).exp()
         }
         crate::HFunction::PolyLeftRightExponential => {
             // Result of \int_0^{\infty} dt (t/sigma)^{-p} exp( -((t^2/sigma^2 +1)/ (t/sigma) -2) )
             let normalisation = match power {
-                None | Some(0) => Into::<T>::into(2.0669536941373771463507142117592) * sig,
-                Some(1) => Into::<T>::into(1.6831364301415428358382497346917) * sig,
-                Some(3) => Into::<T>::into(3.7500901242789199821889639464509) * sig,
-                Some(4) => Into::<T>::into(9.567133942695217110728642104661) * sig,
-                Some(6) => Into::<T>::into(139.3731017521535023682282031464) * sig,
-                Some(7) => Into::<T>::into(729.31700071313208315551590599241) * sig,
-                Some(9) => Into::<T>::into(32336.242742929754092264781379699) * sig,
-                Some(10) => Into::<T>::into(263205.21704946897873941957467669) * sig,
-                Some(12) => Into::<T>::into(2.4275037178930974606209829109376e7) * sig,
-                Some(13) => Into::<T>::into(2.694265921644288712310551611566e8) * sig,
-                Some(15) => Into::<T>::into(9.0407420577601240420566809613266e12) * sig,
-                Some(16) => Into::<T>::into(1.4525174802464911684668046368611e14) * sig,
+                None | Some(0) => Into::<T>::into(2.066_953_694_137_377) * sig,
+                Some(1) => Into::<T>::into(1.683_136_430_141_542_8) * sig,
+                Some(3) => Into::<T>::into(3.750_090_124_278_92) * sig,
+                Some(4) => Into::<T>::into(9.567_133_942_695_218) * sig,
+                Some(6) => Into::<T>::into(139.373_101_752_153_5) * sig,
+                Some(7) => Into::<T>::into(729.317_000_713_132_1) * sig,
+                Some(9) => Into::<T>::into(32_336.242_742_929_753) * sig,
+                Some(10) => Into::<T>::into(263_205.217_049_469) * sig,
+                Some(12) => Into::<T>::into(2.427_503_717_893_097_5e7) * sig,
+                Some(13) => Into::<T>::into(2.694_265_921_644_289e8) * sig,
+                Some(15) => Into::<T>::into(9.040_742_057_760_125e12) * sig,
+                Some(16) => Into::<T>::into(1.452_517_480_246_491_3e14) * sig,
                 _ => panic!(
                     "Value {} of power in poly exponential h function not supported",
                     power.unwrap()
                 ),
             };
             let prefactor = match power {
                 None | Some(0) => normalisation.inv(),
                 Some(p) => (t / sig).powi(-(p as i32)) / normalisation,
             };
             prefactor
-                * (Into::<T>::into(2 as f64) - ((t * t) / (sig * sig) + T::one()) / (t / sig)).exp()
+                * (Into::<T>::into(2_f64) - ((t * t) / (sig * sig) + T::one()) / (t / sig)).exp()
         }
         crate::HFunction::ExponentialCT => {
             let delta_t_sq = (t - tstar.unwrap()) * (t - tstar.unwrap());
             let tstar_sq = tstar.unwrap() * tstar.unwrap();
             // info!("dampener: {}", dampener);
             // info!("delta_t_sq: {}", delta_t_sq);
             // info!("tstar_sq: {}", tstar_sq);
@@ -523,25 +545,22 @@
         }
     }
 }
 
 /// Calculate the determinant of any complex-valued input matrix using LU-decomposition.
 /// Original C-code by W. Gong and D.E. Soper.
 #[allow(unused)]
-pub fn determinant<T: Float + RealNumberLike>(
-    bb: &Vec<Complex<T>>,
-    dimension: usize,
-) -> Complex<T> {
+pub fn determinant<T: Float + RealNumberLike>(bb: &[Complex<T>], dimension: usize) -> Complex<T> {
     // Define matrix related variables.
     let mut determinant = Complex::new(T::one(), T::zero());
     let mut indx = [0; MAX_DIMENSION];
     let mut d = 1; // initialize parity parameter
 
     // Inintialize the matrix to be decomposed with the transferred matrix b.
-    let mut aa = bb.clone();
+    let mut aa = bb.to_vec();
 
     // Define parameters used in decomposition.
     let mut imax = 0;
     let mut flag = 1;
     let mut dumc;
     let mut sum;
 
@@ -566,24 +585,24 @@
         vv[i] = aamax.inv();
     }
     if flag == 1 {
         for j in 0..dimension {
             for i in 0..j {
                 sum = aa[i * dimension + j];
                 for k in 0..i {
-                    sum = sum - aa[i * dimension + k] * aa[k * dimension + j];
+                    sum -= aa[i * dimension + k] * aa[k * dimension + j];
                 }
                 aa[i * dimension + j] = sum;
             }
             //Initialize for the search for largest pivot element.
             aamax = T::zero();
             for i in j..dimension {
                 sum = aa[i * dimension + j];
                 for k in 0..j {
-                    sum = sum - aa[i * dimension + k] * aa[k * dimension + j];
+                    sum -= aa[i * dimension + k] * aa[k * dimension + j];
                 }
                 aa[i * dimension + j] = sum;
                 // Figure of merit for the pivot.
                 dumr = vv[i] * sum.norm_sqr();
                 // Is it better than the best so far?
                 if dumr >= aamax {
                     imax = i;
@@ -602,28 +621,28 @@
                 // Interchange the scale factor.
                 vv[imax] = vv[j];
             }
             indx[j] = imax;
             if j + 1 != dimension {
                 dumc = aa[j * dimension + j].inv();
                 for i in j + 1..dimension {
-                    aa[i * dimension + j] = aa[i * dimension + j] * dumc;
+                    aa[i * dimension + j] *= dumc;
                 }
             }
         }
     }
     // Calculate the determinant using the decomposed matrix.
     if flag == 0 {
         determinant = Complex::default();
     } else {
         // Multiply the diagonal elements.
         for diagonal in 0..dimension {
-            determinant = determinant * aa[diagonal * dimension + diagonal];
+            determinant *= aa[diagonal * dimension + diagonal];
         }
-        determinant = determinant * <T as NumCast>::from(d).unwrap();
+        determinant *= <T as NumCast>::from(d).unwrap();
     }
     determinant
 }
 
 #[allow(unused)]
 pub fn next_combination_with_replacement(state: &mut [usize], max_entry: usize) -> bool {
     for i in (0..state.len()).rev() {
@@ -637,38 +656,56 @@
     }
     false
 }
 
 #[allow(unused)]
 pub fn compute_momentum<T: FloatLike>(
     signature: &(Vec<isize>, Vec<isize>),
-    loop_moms: &Vec<LorentzVector<T>>,
-    external_moms: &Vec<LorentzVector<T>>,
+    loop_moms: &[LorentzVector<T>],
+    external_moms: &[LorentzVector<T>],
 ) -> LorentzVector<T> {
     let mut res = LorentzVector::default();
     for (i_l, sign) in signature.0.iter().enumerate() {
-        res += loop_moms[i_l] * Into::<T>::into(*sign as f64);
+        match sign {
+            1 => {
+                res += loop_moms[i_l];
+            }
+            -1 => {
+                res -= loop_moms[i_l];
+            }
+            0 => {}
+            _ => unreachable!("Sign should be -1,0,1"),
+        }
     }
     for (i_l, sign) in signature.1.iter().enumerate() {
-        res += external_moms[i_l] * Into::<T>::into(*sign as f64);
+        match sign {
+            1 => {
+                res += external_moms[i_l];
+            }
+            -1 => {
+                res -= external_moms[i_l];
+            }
+            0 => {}
+            _ => unreachable!("Sign should be, -1,0,1"),
+        }
     }
     res
 }
 
 // Bilinear form for E-surface defined as sqrt[(k+p1)^2+m1sq] + sqrt[(k+p2)^2+m2sq] + e_shift
 // The Bilinear system then reads 4 k.a.k + 4 k.n + C = 0
 #[allow(unused)]
 pub fn one_loop_e_surface_bilinear_form<T: FloatLike>(
     p1: &[T; 3],
     p2: &[T; 3],
     m1_sq: T,
     m2_sq: T,
     e_shift: T,
 ) -> ([[T; 3]; 3], [T; 3], T) {
-    let two = Into::<T>::into(2 as f64);
+    let two = Into::<T>::into(2_f64);
     let e_shift_sq = e_shift * e_shift;
     let p1_sq = p1[0] * p1[0] + p1[1] * p1[1] + p1[2] * p1[2];
     let p2_sq = p2[0] * p2[0] + p2[1] * p2[1] + p2[2] * p2[2];
 
     let mut a = [[T::zero(); 3]; 3];
     a[0][0] = (p1[0] - p2[0] - e_shift) * (p2[0] - p1[0] - e_shift);
     a[0][1] = (p1[0] - p2[0]) * (p2[1] - p1[1]);
@@ -708,21 +745,39 @@
     // i.e. such cases should be *both* existing and pinched!
     if e_shift > Into::<T>::into(PINCH_TEST_THRESHOLD) {
         return (false, false);
     }
     let test = (e_shift * e_shift - p_norm_sq)
         - (m1_sq.sqrt() + m2_sq.sqrt()) * (m1_sq.sqrt() + m2_sq.sqrt());
     if test.abs() < Into::<T>::into(PINCH_TEST_THRESHOLD) {
-        return (false, true);
+        (false, true)
+    } else if test < T::zero() {
+        (false, false)
     } else {
-        if test < T::zero() {
-            return (false, false);
-        } else {
-            return (true, false);
-        }
+        (true, false)
+    }
+}
+
+pub fn approx_eq(res: f64, target: f64, tolerance: f64) -> bool {
+    if target == 0.0 {
+        res.abs() < tolerance
+    } else {
+        ((res - target) / target).abs() < tolerance
+    }
+}
+
+// panics with useful error message
+#[allow(unused)]
+pub fn assert_approx_eq(res: f64, target: f64, tolerance: f64) {
+    if approx_eq(res, target, tolerance) {
+    } else {
+        panic!(
+            "assert_approx_eq failed: \n{:+e} != \n{:+e} with tolerance {:+e}",
+            res, target, tolerance
+        )
     }
 }
 
 #[allow(unused)]
 pub fn one_loop_eval_e_surf<T: FloatLike>(
     k: &[T; 3],
     p1: &[T; 3],
@@ -781,27 +836,27 @@
     let (a, b, c_coef) = one_loop_e_surface_bilinear_form(p1, p2, m1_sq, m2_sq, e_shift);
     let mut a_coef = T::zero();
     for i in 0..=2 {
         for j in 0..=2 {
             a_coef += k[i] * a[i][j] * k[j];
         }
     }
-    a_coef *= Into::<T>::into(4 as f64);
+    a_coef *= Into::<T>::into(4_f64);
     let mut b_coef = T::zero();
     for i in 0..=2 {
         b_coef += k[i] * b[i];
     }
-    b_coef *= Into::<T>::into(4 as f64);
-    let discr = b_coef * b_coef - Into::<T>::into(4 as f64) * a_coef * c_coef;
+    b_coef *= Into::<T>::into(4_f64);
+    let discr = b_coef * b_coef - Into::<T>::into(4_f64) * a_coef * c_coef;
     if discr < T::zero() {
         [T::zero(), T::zero()]
     } else {
         [
-            (-b_coef + discr.sqrt()) / (Into::<T>::into(2 as f64) * a_coef),
-            (-b_coef - discr.sqrt()) / (Into::<T>::into(2 as f64) * a_coef),
+            (-b_coef + discr.sqrt()) / (Into::<T>::into(2_f64) * a_coef),
+            (-b_coef - discr.sqrt()) / (Into::<T>::into(2_f64) * a_coef),
         ]
     }
 }
 
 pub fn box_muller<T: FloatLike>(x1: T, x2: T) -> (T, T) {
     let r = (-Into::<T>::into(2.) * x1.ln()).sqrt();
     let theta = Into::<T>::into(2.) * T::PI() * x2;
@@ -823,35 +878,47 @@
     )
 }
 
 pub fn get_n_dim_for_n_loop_momenta(
     settings: &Settings,
     n_loop_momenta: usize,
     force_radius: bool,
+    n_edges: Option<usize>, // for tropical parameterization, we need to know the number of edges
 ) -> usize {
+    if settings.sampling
+        == SamplingSettings::DiscreteGraphs(crate::DiscreteGraphSamplingSettings::TropicalSampling)
+    {
+        let tropical_part = 2 * n_edges.unwrap() - 1;
+        let d_l = 3 * n_loop_momenta;
+        return if d_l % 2 == 1 {
+            tropical_part + d_l + 1
+        } else {
+            tropical_part + d_l
+        };
+    }
     match settings.parameterization.mode {
         ParameterizationMode::HyperSphericalFlat => {
             // Because we use Box-Muller, we need to have an even number of angular dimensions
             let mut n_dim = 3 * n_loop_momenta;
             if n_dim % 2 == 1 {
                 n_dim += 1;
             }
             // Then if the radius is not forced, then we need to add one more dimension
             if !force_radius {
                 n_dim += 1;
             }
-            return n_dim;
+            n_dim
         }
         ParameterizationMode::HyperSpherical
         | ParameterizationMode::Cartesian
         | ParameterizationMode::Spherical => {
             if force_radius {
-                return 3 * n_loop_momenta - 1;
+                3 * n_loop_momenta - 1
             } else {
-                return 3 * n_loop_momenta;
+                3 * n_loop_momenta
             }
         }
     }
 }
 
 pub fn global_parameterize<T: FloatLike>(
     x: &[T],
@@ -896,15 +963,15 @@
                             e_cm * b / (T::one() - x_r[0]) / (T::one() + x_r[0] * (b - T::one()));
                         radius
                     }
                     ParameterizationMapping::Linear => {
                         // r = e_cm * b * x/(1-x)
                         let b = Into::<T>::into(settings.parameterization.b);
                         let radius = e_cm * b * x_r[0] / (T::one() - x_r[0]);
-                        jac *= <T as num_traits::Float>::powi(e_cm * b + radius, 2) / e_cm / b;
+                        jac *= <T as num::traits::Float>::powi(e_cm * b + radius, 2) / e_cm / b;
                         radius
                     }
                 }
             };
             match settings.parameterization.mode {
                 ParameterizationMode::HyperSpherical => {
                     let phi = Into::<T>::into(2.) * <T as FloatConst>::PI() * x_r[1];
@@ -922,17 +989,15 @@
                         }
                         cos_thetas.push(cos_theta);
                         sin_thetas.push(sin_theta);
                     }
 
                     let mut concatenated_vecs = Vec::with_capacity(x.len() / 3);
                     let mut base = radius;
-                    for (_i, (cos_theta, sin_theta)) in
-                        cos_thetas.iter().zip(sin_thetas.iter()).enumerate()
-                    {
+                    for (cos_theta, sin_theta) in cos_thetas.iter().zip(sin_thetas.iter()) {
                         concatenated_vecs.push(base * cos_theta);
                         base *= *sin_theta;
                     }
                     concatenated_vecs.push(base * phi.cos());
                     concatenated_vecs.push(base * phi.sin());
 
                     jac *= radius.powi((x.len() - 1) as i32); // hyperspherical coords
@@ -998,29 +1063,33 @@
             (vecs, jac)
         }
     }
 }
 
 #[allow(unused)]
 pub fn global_inv_parameterize<T: FloatLike>(
-    moms: &Vec<LorentzVector<T>>,
+    moms: &[LorentzVector<T>],
     e_cm_squared: T,
     settings: &Settings,
     force_radius: bool,
 ) -> (Vec<T>, T) {
+    if settings.sampling
+        == SamplingSettings::DiscreteGraphs(crate::DiscreteGraphSamplingSettings::TropicalSampling)
+    {
+        panic!("Trying to inverse parameterize a tropical parametrization.")
+    }
     match settings.parameterization.mode {
         ParameterizationMode::HyperSpherical => {
             let e_cm = e_cm_squared.sqrt() * Into::<T>::into(settings.parameterization.shifts[0].0);
             let mut inv_jac = T::one();
             let mut xs = Vec::with_capacity(moms.len() * 3);
 
             let cartesian_xs = moms
                 .iter()
-                .map(|lv| [lv.x, lv.y, lv.z])
-                .flatten()
+                .flat_map(|lv| [lv.x, lv.y, lv.z])
                 .collect::<Vec<_>>();
 
             let mut k_r_sq = cartesian_xs.iter().map(|xi| *xi * xi).sum::<T>();
             // cover the degenerate case
             if k_r_sq.is_zero() {
                 return (vec![T::zero(); cartesian_xs.len()], T::zero());
             }
@@ -1033,15 +1102,15 @@
                         let b = Into::<T>::into(settings.parameterization.b);
                         let x1 = T::one() - b / (-T::one() + b + (k_r / e_cm).exp());
                         inv_jac /= e_cm * b / (T::one() - x1) / (T::one() + x1 * (b - T::one()));
                         xs.push(x1);
                     }
                     ParameterizationMapping::Linear => {
                         let b = Into::<T>::into(settings.parameterization.b);
-                        inv_jac /= <T as num_traits::Float>::powi(e_cm * b + k_r, 2) / e_cm / b;
+                        inv_jac /= <T as num::traits::Float>::powi(e_cm * b + k_r, 2) / e_cm / b;
                         xs.push(k_r / (e_cm * b + k_r));
                     }
                 }
             };
 
             let y = cartesian_xs[cartesian_xs.len() - 2];
             let x = cartesian_xs[cartesian_xs.len() - 1];
@@ -1156,15 +1225,15 @@
 
                     radius
                 }
                 ParameterizationMapping::Linear => {
                     // r = e_cm * b * x/(1-x)
                     let b = Into::<T>::into(settings.parameterization.b);
                     let radius = e_cm * b * x_r[0] / (T::one() - x_r[0]);
-                    jac *= <T as num_traits::Float>::powi(e_cm * b + radius, 2) / e_cm / b;
+                    jac *= <T as num::traits::Float>::powi(e_cm * b + radius, 2) / e_cm / b;
                     radius
                 }
             };
             let phi = Into::<T>::into(2.) * <T as FloatConst>::PI() * x_r[1];
             jac *= Into::<T>::into(2.) * <T as FloatConst>::PI();
 
             let cos_theta = -T::one() + Into::<T>::into(2.) * x_r[2]; // out of range
@@ -1230,15 +1299,15 @@
             let b = Into::<T>::into(settings.parameterization.b);
             let x1 = T::one() - b / (-T::one() + b + (k_r / e_cm).exp());
             jac /= e_cm * b / (T::one() - x1) / (T::one() + x1 * (b - T::one()));
             x1
         }
         ParameterizationMapping::Linear => {
             let b = Into::<T>::into(settings.parameterization.b);
-            jac /= <T as num_traits::Float>::powi(e_cm * b + k_r, 2) / e_cm / b;
+            jac /= <T as num::traits::Float>::powi(e_cm * b + k_r, 2) / e_cm / b;
             k_r / (e_cm * b + k_r)
         }
     };
 
     let x3 = Into::<T>::into(0.5) * (T::one() + z / k_r);
 
     jac /= Into::<T>::into(2.) * <T as FloatConst>::PI();
@@ -1260,15 +1329,15 @@
 pub const MINUTE: usize = 60;
 pub const HOUR: usize = 3_600;
 pub const DAY: usize = 86_400;
 pub const WEEK: usize = 604_800;
 pub fn format_wdhms(seconds: usize) -> String {
     let mut compound_duration = vec![];
     if seconds == 0 {
-        compound_duration.push(format!("{}", "0s"));
+        compound_duration.push("0s".to_string());
         return compound_duration.join(" ");
     }
 
     let mut sec = seconds % WEEK;
     // weeks
     let ws = seconds / WEEK;
     if ws != 0 {
@@ -1307,37 +1376,36 @@
 #[allow(unused)]
 pub fn inverse_gamma_lr(a: f64, p: f64, n_iter: usize) -> f64 {
     // this algorithm is taken from https://dl.acm.org/doi/pdf/10.1145/22721.23109
 
     // get an estimate for x0 to start newton iterations.
     let q = 1.0 - p;
 
-    if 1.0 - 1.0e-8 <= a && a <= 1.0 + 1.0e-8 {
+    if (1.0 - 1.0e-8..=1.0 + 1.0e-8).contains(&a) {
         return -q.ln();
     }
 
     let gamma_a = gamma(a);
     let b = q * gamma_a;
-    let c = 0.57721566490153286060651209008240;
+    let c = 0.577_215_664_901_532_9;
 
     let mut x0 = 0.5;
     if a < 1.0 {
         if b > 0.6 || (b >= 0.45 && a >= 0.3) {
-            let u: f64;
-            if b * q > 10e-8 {
-                u = (p * gamma(a + 1.0)).powf(a.recip());
+            let u = if b * q > 10e-8 {
+                (p * gamma(a + 1.0)).powf(a.recip())
             } else {
-                u = (-q / a - c).exp();
-            }
+                (-q / a - c).exp()
+            };
             x0 = u / (1.0 - u / (a + 1.0));
-        } else if a < 0.3 && 0.35 <= b && b <= 0.6 {
+        } else if a < 0.3 && (0.35..=0.6).contains(&b) {
             let t = (-c - b).exp();
             let u = t * t.exp();
             x0 = t * u.exp();
-        } else if (0.15 <= b && b <= 0.35) || (0.15 <= b && b < 0.45 && a >= 0.3) {
+        } else if (0.15..=0.35).contains(&b) || ((0.15..0.45).contains(&b) && a >= 0.3) {
             let y = -b.ln();
             let u = y - (1.0 - a) * y.ln();
             x0 = y - (1.0 - a) * y.ln() - (1.0 + (1.0 - a) / (1.0 + u)).ln();
         } else if 0.01 < b && b < 0.15 {
             let y = -b.ln();
             let u = y - (1.0 - a) * y.ln();
             x0 = y
@@ -1382,15 +1450,15 @@
         let a_1 = 11.6616720288968;
         let a_2 = 4.28342155967104;
         let a_3 = 0.213623493715853;
 
         let b_1 = 6.61053765625462;
         let b_2 = 6.40691597760039;
         let b_3 = 1.27364489782223;
-        let b_4 = 0.3611708101884203e-1;
+        let b_4 = 3.611_708_101_884_203e-2;
 
         let t2 = t * t;
         let t3 = t2 * t;
         let t4 = t3 * t;
 
         let numerator = a_0 + a_1 * t + a_2 * t2 + a_3 * t3;
         let denominator = 1.0 + b_1 * t + b_2 * t2 + b_3 * t3 + b_4 * t4;
@@ -1405,79 +1473,72 @@
 
         let w = a + s * a_sqrt + (s2 - 1.0) / 3.0 + (s3 - 7.0 * s) / (36.0 * a_sqrt)
             - (3.0 * s4 + 7.0 * s2 - 16.0) / (810.0 * a)
             + (9.0 * s5 + 256.0 * s3 - 433.0 * s) / (38880.0 * a * a_sqrt);
 
         if a >= 500.0 && (1.0 - w / a).abs() < 1.0e-6 {
             return w;
-        } else {
-            if p > 0.5 {
-                if w < 3.0 * a {
-                    x0 = w;
+        } else if p > 0.5 {
+            if w < 3.0 * a {
+                x0 = w;
+            } else {
+                let d = 2f64.max(a * (a - 1.0));
+                if b > 10f64.powf(-d) {
+                    let u = -b.ln() + (a - 1.0) * w.ln() - (1.0 + (1.0 - a) / (1.0 + w)).ln();
+                    x0 = -b.ln() + (a - 1.0) * u.ln() - (1.0 + (1.0 - a) / (1.0 + u)).ln();
                 } else {
-                    let d = 2f64.max(a * (a - 1.0));
-                    if b > 10f64.powf(-d) {
-                        let u = -b.ln() + (a - 1.0) * w.ln() - (1.0 + (1.0 - a) / (1.0 + w)).ln();
-                        x0 = -b.ln() + (a - 1.0) * u.ln() - (1.0 + (1.0 - a) / (1.0 + u)).ln();
-                    } else {
-                        let y = -b.ln();
-                        let c1 = (a - 1.0) * y.ln();
-                        let c2 = (a - 1.0) * (1.0 + c1);
-                        let c3 =
-                            (a - 1.0) * (-0.5 * c1 * c1 + (a - 2.0) * c1 + (3.0 * a - 5.0) * 0.5);
-                        let c4 = (a - 1.0)
-                            * (1.0 / 3.0 * c1 * c1 * c1 - (3.0 * a - 5.0) * 0.5 * c1 * c1
-                                + (a * a - 6.0 * a + 7.0) * c1
-                                + (11.0 * a * a - 46.0 * a + 47.0) / 6.0);
-                        let c5 = (a - 1.0)
-                            * (-0.25 * c1 * c1 * c1 * c1
-                                + (11.0 * a - 7.0) / 6.0 * c1 * c1 * c1
-                                + (-3.0 * a * a - 13.0) * c1 * c1
-                                + (2.0 * a * a * a - 25.0 * a * a + 72.0 * a - 61.0) * 0.5 * c1
-                                + (25.0 * a * a * a - 195.0 * a * a + 477.0 * a - 379.0) / 12.0);
-                        x0 = y
-                            + c1
-                            + c2 / (y)
-                            + c3 / (y * y)
-                            + c4 / (y * y * y)
-                            + c5 / (y * y * y * y);
-                    }
+                    let y = -b.ln();
+                    let c1 = (a - 1.0) * y.ln();
+                    let c2 = (a - 1.0) * (1.0 + c1);
+                    let c3 = (a - 1.0) * (-0.5 * c1 * c1 + (a - 2.0) * c1 + (3.0 * a - 5.0) * 0.5);
+                    let c4 = (a - 1.0)
+                        * (1.0 / 3.0 * c1 * c1 * c1 - (3.0 * a - 5.0) * 0.5 * c1 * c1
+                            + (a * a - 6.0 * a + 7.0) * c1
+                            + (11.0 * a * a - 46.0 * a + 47.0) / 6.0);
+                    let c5 = (a - 1.0)
+                        * (-0.25 * c1 * c1 * c1 * c1
+                            + (11.0 * a - 7.0) / 6.0 * c1 * c1 * c1
+                            + (-3.0 * a * a - 13.0) * c1 * c1
+                            + (2.0 * a * a * a - 25.0 * a * a + 72.0 * a - 61.0) * 0.5 * c1
+                            + (25.0 * a * a * a - 195.0 * a * a + 477.0 * a - 379.0) / 12.0);
+                    x0 = y + c1 + c2 / (y) + c3 / (y * y) + c4 / (y * y * y) + c5 / (y * y * y * y);
                 }
-            } else {
-                // this part is heavily simplified from the paper, if any issues occur this estimate
-                // will need more refinement.
-                let v = (p * gamma(a + 1.0)).ln();
-                x0 = ((v + w) / a).exp();
             }
+        } else {
+            // this part is heavily simplified from the paper, if any issues occur this estimate
+            // will need more refinement.
+            let v = (p * gamma(a + 1.0)).ln();
+            x0 = ((v + w) / a).exp();
         }
     }
 
     // start iteration
     let mut x_n = x0;
     for _ in 0..n_iter {
         let r = x_n.powf(a - 1.0) * (-x_n).exp() / gamma_a;
-        let t_n;
-        if p <= 0.5 {
-            t_n = (gamma_lr(a, x_n) - p) / r;
-        } else {
-            t_n = -(gamma_ur(a, x_n) - q) / r;
+        if x_n <= 0. {
+            x_n = 1.0e-16;
         }
+        let t_n = if p <= 0.5 {
+            (gamma_lr(a, x_n) - p) / r
+        } else {
+            -(gamma_ur(a, x_n) - q) / r
+        };
         let w_n = (a - 1.0 - x_n) / 2.0;
 
-        let h_n;
-        if t_n.abs() <= 0.1 && (w_n * t_n).abs() <= 0.1 {
-            h_n = t_n + w_n * t_n * t_n;
+        let h_n = if t_n.abs() <= 0.1 && (w_n * t_n).abs() <= 0.1 {
+            t_n + w_n * t_n * t_n
         } else {
-            h_n = t_n;
-        }
+            t_n
+        };
 
         x_n -= h_n;
     }
 
-    return x_n;
+    x_n
 }
 
 #[allow(unused)]
 pub fn inv_3x3_sig_matrix(mat: [[isize; 3]; 3]) -> [[isize; 3]; 3] {
     let denom = -mat[0][2] * mat[1][1] * mat[2][0]
         + mat[0][1] * mat[1][2] * mat[2][0]
         + mat[0][2] * mat[1][0] * mat[2][1]
@@ -1500,28 +1561,162 @@
 
     inv_mat
 }
 
 pub fn print_banner() {
     info!(
         "\n{}{}\n",
-        format!(
-            "{}",
-            r#"                                        _                       
+        r"                                        _                       
                                        | |                      
    __ _  __ _ _ __ ___  _ __ ___   __ _| |     ___   ___  _ __  
   / _` |/ _` | '_ ` _ \| '_ ` _ \ / _` | |    / _ \ / _ \| '_ \ 
  | (_| | (_| | | | | | | | | | | | (_| | |___| (_) | (_) | |_) |
   \__, |\__,_|_| |_| |_|_| |_| |_|\__,_|______\___/ \___/| .__/ 
    __/ |                                                 | |    
-"#
-        )
+"
+        .to_string()
         .bold()
         .blue(),
         format!(
             r#"  |___/    {}                    |_|    "#,
             format!("{:-26}", GIT_VERSION).green(),
         )
         .bold()
         .blue(),
     );
 }
+
+#[allow(unused)]
+#[inline]
+pub fn upgrade_lorentz_vector(k: &LorentzVector<f64>) -> LorentzVector<f128::f128> {
+    cast_lorentz_vector(k)
+}
+
+#[allow(unused)]
+#[inline]
+pub fn cast_lorentz_vector<T1: Into<T2> + Field, T2: Field>(
+    k: &LorentzVector<T1>,
+) -> LorentzVector<T2> {
+    LorentzVector::from_args(
+        Into::<T2>::into(k.t),
+        Into::<T2>::into(k.x),
+        Into::<T2>::into(k.y),
+        Into::<T2>::into(k.z),
+    )
+}
+
+#[allow(unused)]
+#[inline]
+pub fn cast_complex<T1: Into<T2>, T2>(z: Complex<T1>) -> Complex<T2> {
+    Complex::new(Into::<T2>::into(z.re), Into::<T2>::into(z.im))
+}
+
+#[allow(unused)]
+pub fn perform_spatial_rotation<T: FloatLike>(
+    k: &LorentzVector<T>,
+    alpha: f64,
+    beta: f64,
+    gamma: f64,
+) -> LorentzVector<T> {
+    let sin_alpha = Into::<T>::into(alpha).sin();
+    let cos_alpha = Into::<T>::into(alpha).cos();
+    let sin_beta = Into::<T>::into(beta).sin();
+    let cos_beta = Into::<T>::into(beta).cos();
+    let sin_gamma = Into::<T>::into(gamma).sin();
+    let cos_gamma = Into::<T>::into(gamma).cos();
+
+    LorentzVector::from_args(
+        k.t,
+        cos_beta * cos_gamma * k.x
+            + (-cos_alpha * sin_gamma + sin_alpha * sin_beta * cos_gamma) * k.y
+            + (sin_alpha * sin_gamma + cos_alpha * sin_beta * cos_gamma) * k.z,
+        cos_beta * sin_gamma * k.x
+            + (cos_alpha * cos_gamma + sin_alpha * sin_beta * sin_gamma) * k.y
+            + (-sin_alpha * cos_gamma + cos_alpha * sin_beta * sin_gamma) * k.z,
+        -sin_beta * k.x + sin_alpha * cos_beta * k.y + cos_alpha * cos_beta * k.z,
+    )
+}
+
+#[allow(unused)]
+pub fn perform_pi2_rotation_x<T: FloatLike>(k: &LorentzVector<T>) -> LorentzVector<T> {
+    LorentzVector::from_args(k.t, k.x, -k.z, k.y)
+}
+
+#[allow(unused)]
+pub fn perform_pi2_rotation_y<T: FloatLike>(k: &LorentzVector<T>) -> LorentzVector<T> {
+    LorentzVector::from_args(k.t, k.z, k.y, -k.x)
+}
+
+#[allow(unused)]
+pub fn perform_pi2_rotation_z<T: FloatLike>(k: &LorentzVector<T>) -> LorentzVector<T> {
+    LorentzVector::from_args(k.t, -k.y, k.x, k.z)
+}
+
+#[allow(unused)]
+pub fn format_for_compare_digits(x: f64, y: f64) -> (String, String) {
+    let string_x = format!("{:.16e}", x);
+    let string_y = format!("{:.16e}", y);
+
+    let string_vec = string_x
+        .chars()
+        .zip(string_y.chars())
+        .map(|(char_x, char_y)| {
+            if char_x == char_y {
+                (char_x.to_string().green(), char_y.to_string().green())
+            } else {
+                (char_x.to_string().red(), char_y.to_string().red())
+            }
+        })
+        .collect_vec();
+
+    let string_x = string_vec.iter().map(|(x, _)| x).join("");
+    let string_y = string_vec.iter().map(|(_, y)| y).join("");
+
+    (string_x, string_y)
+}
+
+#[allow(unused)]
+pub fn format_evaluation_time(time: Duration) -> String {
+    let time_secs = time.as_secs_f64();
+    if time_secs < 1e-6 {
+        format!("{} ns", time.as_nanos())
+    } else if time_secs < 1e-3 {
+        format!("{:.2} µs", (time.as_nanos() as f64) / 1000.)
+    } else if time_secs < 1.0 {
+        format!("{:.2} ms", (time.as_micros() as f64) / 1000.)
+    } else {
+        format!("{:.2} s", (time.as_millis() as f64) / 1000.)
+    }
+}
+
+pub fn format_evaluation_time_from_f64(time: f64) -> String {
+    format_evaluation_time(Duration::from_secs_f64(time))
+}
+
+pub fn format_sample(sample: &Sample<f64>) -> String {
+    match sample {
+        Sample::Continuous(_, xs) => {
+            let xs_point = xs.iter().map(|x| format!("{:.16}", x)).join(", ");
+            format!("xs: [{}]", xs_point)
+        }
+        Sample::Discrete(_, graph_index, Some(nested_sample)) => match nested_sample.as_ref() {
+            Sample::Continuous(_, xs) => {
+                let xs_point = xs.iter().map(|x| format!("{:.16}", x)).join(", ");
+                format!("graph: {}, xs: [{}]", graph_index, xs_point)
+            }
+            Sample::Discrete(_, channel_index, Some(nested_cont_sample)) => {
+                match nested_cont_sample.as_ref() {
+                    Sample::Continuous(_, xs) => {
+                        let xs_point = xs.iter().map(|x| format!("{:.16}", x)).join(", ");
+                        format!(
+                            "graph: {}, channel: {}, xs: [{}]",
+                            graph_index, channel_index, xs_point
+                        )
+                    }
+                    _ => String::from("N/A"),
+                }
+            }
+            _ => String::from("N/A"),
+        },
+        _ => String::from("N/A"),
+    }
+}
```

### Comparing `gammaloop-0.0.1/PKG-INFO` & `gammaloop-0.1.0/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -1,50 +1,60 @@
-Metadata-Version: 2.1
-Name: gammaloop
-Version: 0.0.1
-Classifier: Development Status :: 3 - Alpha
-Classifier: Programming Language :: Rust
-Classifier: Topic :: Scientific/Engineering :: Physics
-Requires-Dist: PyYAML >=6.0.1
-Requires-Dist: symbolica >=0.1.0
-License-File: License.md
-License-File: LICENSE.md
-Summary: Gammaloop computes differential cross-sections using Local Unitarity
-Keywords: physics,collider,cross-section,perturbative,loop
-Author: Valentin Hirschi
-Author-email: valentin.hirschi@gmail.com
-Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
-Project-URL: homepage, https://alphaloop.ch
-Project-URL: repository, https://github.com/alphal00p/gammaloop
-
-# GammaLoop
+# gammaLoop
+![tests status](https://github.com/alphal00p/gammaloop/actions/workflows/gamma_loop_tests.yml/badge.svg?event=push)
 
 *Computation of differential cross-sections using Local Unitarity.*
 
 See [www.alphaloop.ch](www.alphaloop.ch) for details on the theoretical framework and related literature.
 
 See the [wiki](https://wiki.alphaloop.ch/) for more information on the project.
 
+## TL;DR: I want to be running γLoop already!
+
+We salute the eagerness of our users.
+
+If you want to jump right in, run the following to immediately start integrating the scalar three-loop mercedes diagram!
+
+```
+git clone https://github.com/alphal00p/gammaloop.git && cd gammaloop
+./bin/compile.sh
+source python/gammaloop/dependencies/venv/bin/activate
+./bin/gammaloop example/cards/scalar_mercedes.gL
+```
+
 ## Installation
 
+### > Requirements
+
+* `Rust`: You can easily instal Rust with this [one-liner](https://www.rust-lang.org/tools/install)
+
+* `Python3`: v3.10+
+
+* `gcc`: v10+
+
+*Note*: The project has been tested on Linux and MacOS. 
+
+Windows users are encouraged to use [WSL 2](https://learn.microsoft.com/en-us/windows/wsl/).
+
 ### > Installation using `pip`
 ```
 pip install gammaloop
+gammaloop --build_dependencies
+source `gammaloop -venv`
 ```
 
+*Note:* when using the `fish` shell, the last command should be replaced by: `. (./bin/gammaloop -venv).fish`
+
 ### > Installation from sources
 ```
 git clone https://github.com/alphal00p/gammaloop.git
 cd gammaloop
-python -m pip install -r ./python/gammaloop/requirements.txt
-./bin/build_dependencies.sh
-./bin/compile_bin.sh --release
-./bin/compile_lib.sh --release
+./bin/compile.sh
+source python/gammaloop/dependencies/venv/bin/activate
 ```
-The relevant binaries will then be in `./bin/` and the python module in `./python/gammalop`.
+The relevant binaries will then be in `./bin/` and the gammaloop python module is located at `./python/gammaloop`.
 
 ## Tests
 
 ### > Testing an installation from `pip`
 
 Testing your installation can be done by running
 ```
@@ -53,28 +63,40 @@
 from within the installation directory of the gammaloop module, which you can `cd` into with e.g.:
 ```
 bash -c 'cd `python -c "import os; import gammaloop; print(os.path.dirname(gammaloop.__file__))"`; pwd'
 ```
 
 ### > Testing an installation from sources
 
-Simply run:
+Run:
 ```
 /bin/run_tests.sh python
 /bin/run_tests.sh rust
 ```
 
 ## Usage
 
-`GammaLoop` can be used as a python command line interface (`gammaloop`) for scattering process code generation or also directly as a binary (`gammaloop_rust_cli`) for steering the Monte-Carlo integration. Both programs are installed as scripts in the `bin` directly when installing `GammaLoop` using `pip` or when installing it from sources.
+There are three entry points to the `GammaLoop` functionalities:
+
+1. Preferred method is through the Python command-line interface `gammaloop`.
+
+2. Alternatively, the same functionalities can be accessed programmatically, e.g. in a Jupyter notebook, through the Python API, by importing the `gammaloop` library.
+
+3. Finally, expert users may also find it useful to steer some of functionalities directly from the rust binary `gammaloop_rust_cli`.
+
+Both executables `gammaloop` and `gammaloop_rust_cli` are made available as scripts in the `bin` directory.
+The `gammaloop` Python module is also exposed after installation and ready to be imported in user custom Python scripts.
 
-### > Generating scattering process code with ./gammaloop
+### 1. Usage from the Python command-line interface: ./gammaloop
 
+`GammaLoop` is typically used through the python command-line interface `gammaloop`.
 Place your list of commands in a file named e.g. `cmd.gL`, for instance:
+
 ```
+# Content of file 'cmd.gL'
 import_model sm --format ufo
 export_model ./sm.yaml --format yaml
 ```
 and run it with:
 ```
 ./gammaloop cmd.gL
 ```
@@ -83,19 +105,32 @@
 ./gammaloop --help
 ```
 to get an overview of available commands and:
 ```
 ./bin/gammaloop -c "help import_model"
 ```
 to get help on any specific command.
+
 You can find example of command files in the `<MODULE_PATH>/data/run_cards/` directory.
 
-### > Steering Monte-Carlo integration with ./gammaloop_rust_cli
+### 2. Usage from within a Jupyter notebook: the Python API
+
+Follow the example jupyter notebook given in example to get started with the Python API.
+```
+cd <GAMMALOOP_INSTALLATION_DIRECTORY>/examples/jupyter
+jupyter notebook steer_gammaloop.ipynb
+``` 
+
+### 3. Usage from the rust binary executable: ./gammaloop_rust_cli
 
-Steering a Monte-Carlo integration with `gammaloop_rust_cli` can be done by running:
+All typical usecases of `GammaLoop` are available through the Python command-line interface mentioned earlier.
+However, expert users might want to steer the Monte-Carlo integration directly using the `gammaloop_rust_cli` binary.
+This is possible throught the `gammaloop_rust_cli` binary, which can be used as follows:
 ```
 ./bin/gammaloop_rust_cli --config <MODULE_PATH>/gammaloop/data/run_cards/rust_run_config.yaml
 ```
+*Note*: You have to manually define your desired external momenta in this default `rust_run_config.yaml` file.
+
 You will find more information on the content of the run configuration file and steering options in the [wiki](https://wiki.alphaloop.ch/) and by running:
 ```
 ./bin/gammaloop_rust_cli --help
 ```
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

