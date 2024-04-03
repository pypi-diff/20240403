# Comparing `tmp/docplex-2.8.125.tar.gz` & `tmp/docplex-2.9.141.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/docplex-2.8.125.tar", last modified: Fri Oct 19 12:46:09 2018, max compression
+gzip compressed data, was "dist/docplex-2.9.141.tar", last modified: Thu Mar 14 11:18:48 2019, max compression
```

## Comparing `docplex-2.8.125.tar` & `docplex-2.9.141.tar`

### file list

```diff
@@ -1,131 +1,132 @@
-drwxrwxr-x   0 root         (0) root         (0)        0 2018-10-19 12:46:09.000000 docplex-2.8.125/
-drwxrwxr-x   0 root         (0) root         (0)        0 2018-10-19 12:46:09.000000 docplex-2.8.125/docplex/
-drwxrwxr-x   0 root         (0) root         (0)        0 2018-10-19 12:46:09.000000 docplex-2.8.125/docplex/cp/
-drwxrwxr-x   0 root         (0) root         (0)        0 2018-10-19 12:46:09.000000 docplex-2.8.125/docplex/cp/fzn/
--rw-rw-r--   0 root         (0) root         (0)      494 2018-10-17 14:31:00.000000 docplex-2.8.125/docplex/cp/fzn/__init__.py
--rw-rw-r--   0 root         (0) root         (0)    73140 2018-10-17 14:31:00.000000 docplex-2.8.125/docplex/cp/fzn/fzn_parser.py
--rw-rw-r--   0 root         (0) root         (0)     3596 2018-10-17 14:31:00.000000 docplex-2.8.125/docplex/cp/fzn/fzn_tokenizer.py
-drwxrwxr-x   0 root         (0) root         (0)        0 2018-10-19 12:46:09.000000 docplex-2.8.125/docplex/cp/solver/
--rw-rw-r--   0 root         (0) root         (0)      515 2018-10-17 14:31:00.000000 docplex-2.8.125/docplex/cp/solver/__init__.py
--rw-rw-r--   0 root         (0) root         (0)    11894 2018-10-17 14:31:00.000000 docplex-2.8.125/docplex/cp/solver/docloud_client.py
--rw-rw-r--   0 root         (0) root         (0)    10261 2018-10-17 14:31:00.000000 docplex-2.8.125/docplex/cp/solver/environment_client.py
--rw-rw-r--   0 root         (0) root         (0)    39789 2018-10-17 14:31:00.000000 docplex-2.8.125/docplex/cp/solver/solver.py
--rw-rw-r--   0 root         (0) root         (0)     9765 2018-10-17 14:31:00.000000 docplex-2.8.125/docplex/cp/solver/solver_docloud.py
--rw-rw-r--   0 root         (0) root         (0)    23567 2018-10-17 14:31:00.000000 docplex-2.8.125/docplex/cp/solver/solver_listener.py
--rw-rw-r--   0 root         (0) root         (0)    19648 2018-10-17 14:31:00.000000 docplex-2.8.125/docplex/cp/solver/solver_local.py
--rw-rw-r--   0 root         (0) root         (0)    11663 2018-10-17 14:31:00.000000 docplex-2.8.125/docplex/cp/solver/solver_simulator.py
--rw-rw-r--   0 root         (0) root         (0)     1355 2018-10-17 14:30:54.000000 docplex-2.8.125/docplex/cp/__init__.py
--rw-rw-r--   0 root         (0) root         (0)    64455 2018-10-17 14:30:54.000000 docplex-2.8.125/docplex/cp/catalog.py
--rw-rw-r--   0 root         (0) root         (0)    10598 2018-10-17 14:30:54.000000 docplex-2.8.125/docplex/cp/catalog_elements.py
--rw-rw-r--   0 root         (0) root         (0)    21412 2018-10-17 14:30:54.000000 docplex-2.8.125/docplex/cp/config.py
--rw-rw-r--   0 root         (0) root         (0)    40597 2018-10-17 14:30:54.000000 docplex-2.8.125/docplex/cp/cpo_compiler.py
--rw-rw-r--   0 root         (0) root         (0)    31497 2018-10-17 14:30:54.000000 docplex-2.8.125/docplex/cp/cpo_parser.py
--rw-rw-r--   0 root         (0) root         (0)     3775 2018-10-17 14:30:54.000000 docplex-2.8.125/docplex/cp/cpo_tokenizer.py
--rw-rw-r--   0 root         (0) root         (0)    92708 2018-10-17 14:30:54.000000 docplex-2.8.125/docplex/cp/expression.py
--rw-rw-r--   0 root         (0) root         (0)    20770 2018-10-17 14:30:54.000000 docplex-2.8.125/docplex/cp/function.py
--rw-rw-r--   0 root         (0) root         (0)    60766 2018-10-17 14:30:54.000000 docplex-2.8.125/docplex/cp/model.py
--rw-rw-r--   0 root         (0) root         (0)   179327 2018-10-17 14:30:54.000000 docplex-2.8.125/docplex/cp/modeler.py
--rw-rw-r--   0 root         (0) root         (0)    57508 2018-10-17 14:30:54.000000 docplex-2.8.125/docplex/cp/parameters.py
--rw-rw-r--   0 root         (0) root         (0)    69549 2018-10-17 14:30:54.000000 docplex-2.8.125/docplex/cp/solution.py
--rw-rw-r--   0 root         (0) root         (0)    16931 2018-10-17 14:30:54.000000 docplex-2.8.125/docplex/cp/tokenizer.py
--rw-rw-r--   0 root         (0) root         (0)    49739 2018-10-17 14:30:54.000000 docplex-2.8.125/docplex/cp/utils.py
--rw-rw-r--   0 root         (0) root         (0)    61202 2018-10-17 14:30:54.000000 docplex-2.8.125/docplex/cp/utils_visu.py
-drwxrwxr-x   0 root         (0) root         (0)        0 2018-10-19 12:46:09.000000 docplex-2.8.125/docplex/mp/
-drwxrwxr-x   0 root         (0) root         (0)        0 2018-10-19 12:46:09.000000 docplex-2.8.125/docplex/mp/callbacks/
--rw-rw-r--   0 root         (0) root         (0)      296 2018-10-17 14:31:04.000000 docplex-2.8.125/docplex/mp/callbacks/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     5360 2018-10-17 14:31:04.000000 docplex-2.8.125/docplex/mp/callbacks/cb_mixin.py
-drwxrwxr-x   0 root         (0) root         (0)        0 2018-10-19 12:46:09.000000 docplex-2.8.125/docplex/mp/internal/
--rw-rw-r--   0 root         (0) root         (0)      314 2018-10-17 14:31:04.000000 docplex-2.8.125/docplex/mp/internal/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     3167 2018-10-17 14:31:04.000000 docplex-2.8.125/docplex/mp/internal/json_conflict_handler.py
--rw-rw-r--   0 root         (0) root         (0)      790 2018-10-17 14:31:04.000000 docplex-2.8.125/docplex/mp/internal/json_infeasibility_handler.py
--rw-rw-r--   0 root         (0) root         (0)     4181 2018-10-17 14:31:04.000000 docplex-2.8.125/docplex/mp/internal/json_solution_handler.py
-drwxrwxr-x   0 root         (0) root         (0)        0 2018-10-19 12:46:09.000000 docplex-2.8.125/docplex/mp/params/
--rw-rw-r--   0 root         (0) root         (0)      361 2018-10-17 14:31:04.000000 docplex-2.8.125/docplex/mp/params/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     1815 2018-10-17 14:31:04.000000 docplex-2.8.125/docplex/mp/params/cplex_params.py
--rw-rw-r--   0 root         (0) root         (0)    35064 2018-10-17 14:31:04.000000 docplex-2.8.125/docplex/mp/params/parameter_hierarchy_12620.py
--rw-rw-r--   0 root         (0) root         (0)    35478 2018-10-17 14:31:04.000000 docplex-2.8.125/docplex/mp/params/parameter_hierarchy_12630.py
--rw-rw-r--   0 root         (0) root         (0)    37179 2018-10-17 14:31:04.000000 docplex-2.8.125/docplex/mp/params/parameter_hierarchy_12700.py
--rw-rw-r--   0 root         (0) root         (0)    37325 2018-10-17 14:31:04.000000 docplex-2.8.125/docplex/mp/params/parameter_hierarchy_12710.py
--rw-rw-r--   0 root         (0) root         (0)    40345 2018-10-17 14:31:04.000000 docplex-2.8.125/docplex/mp/params/parameter_hierarchy_12800.py
--rw-rw-r--   0 root         (0) root         (0)    40045 2018-10-17 14:31:04.000000 docplex-2.8.125/docplex/mp/params/parameter_hierarchy_12900.py
--rw-rw-r--   0 root         (0) root         (0)    29307 2018-10-17 14:31:04.000000 docplex-2.8.125/docplex/mp/params/parameters.py
-drwxrwxr-x   0 root         (0) root         (0)        0 2018-10-19 12:46:09.000000 docplex-2.8.125/docplex/mp/sktrans/
--rw-rw-r--   0 root         (0) root         (0)      316 2018-10-17 14:31:04.000000 docplex-2.8.125/docplex/mp/sktrans/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     9813 2018-10-17 14:31:04.000000 docplex-2.8.125/docplex/mp/sktrans/cpx_mdlr.py
--rw-rw-r--   0 root         (0) root         (0)     4530 2018-10-17 14:31:04.000000 docplex-2.8.125/docplex/mp/sktrans/docplex_mdlr.py
--rw-rw-r--   0 root         (0) root         (0)      843 2018-10-17 14:31:04.000000 docplex-2.8.125/docplex/mp/sktrans/modeler.py
--rw-rw-r--   0 root         (0) root         (0)      954 2018-10-17 14:31:04.000000 docplex-2.8.125/docplex/mp/sktrans/pd_utils.py
--rw-rw-r--   0 root         (0) root         (0)    14045 2018-10-17 14:31:04.000000 docplex-2.8.125/docplex/mp/sktrans/transformers.py
-drwxrwxr-x   0 root         (0) root         (0)        0 2018-10-19 12:46:09.000000 docplex-2.8.125/docplex/mp/sparktrans/
--rw-rw-r--   0 root         (0) root         (0)      316 2018-10-17 14:31:04.000000 docplex-2.8.125/docplex/mp/sparktrans/__init__.py
--rw-rw-r--   0 root         (0) root         (0)      541 2018-10-17 14:31:04.000000 docplex-2.8.125/docplex/mp/sparktrans/spark_utils.py
--rw-rw-r--   0 root         (0) root         (0)    13041 2018-10-17 14:31:04.000000 docplex-2.8.125/docplex/mp/sparktrans/transformers.py
-drwxrwxr-x   0 root         (0) root         (0)        0 2018-10-19 12:46:09.000000 docplex-2.8.125/docplex/mp/worker/
--rw-rw-r--   0 root         (0) root         (0)      322 2018-10-17 14:31:04.000000 docplex-2.8.125/docplex/mp/worker/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     1755 2018-10-17 14:31:04.000000 docplex-2.8.125/docplex/mp/worker/solve_hook.py
--rw-rw-r--   0 root         (0) root         (0)      584 2018-10-17 14:31:04.000000 docplex-2.8.125/docplex/mp/worker/worker_env.py
--rw-rw-r--   0 root         (0) root         (0)     1467 2018-10-17 14:31:02.000000 docplex-2.8.125/docplex/mp/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     2728 2018-10-17 14:31:02.000000 docplex-2.8.125/docplex/mp/absmodel.py
--rw-rw-r--   0 root         (0) root         (0)    29114 2018-10-17 14:31:02.000000 docplex-2.8.125/docplex/mp/advmodel.py
--rw-rw-r--   0 root         (0) root         (0)    13490 2018-10-17 14:31:02.000000 docplex-2.8.125/docplex/mp/aggregator.py
--rw-rw-r--   0 root         (0) root         (0)     4167 2018-10-17 14:31:02.000000 docplex-2.8.125/docplex/mp/anno.py
--rw-rw-r--   0 root         (0) root         (0)    14850 2018-10-17 14:31:02.000000 docplex-2.8.125/docplex/mp/basic.py
--rw-rw-r--   0 root         (0) root         (0)     3042 2018-10-17 14:31:02.000000 docplex-2.8.125/docplex/mp/cloudutils.py
--rw-rw-r--   0 root         (0) root         (0)     1789 2018-10-17 14:31:02.000000 docplex-2.8.125/docplex/mp/compat23.py
--rw-rw-r--   0 root         (0) root         (0)    12075 2018-10-17 14:31:02.000000 docplex-2.8.125/docplex/mp/conflict_refiner.py
--rw-rw-r--   0 root         (0) root         (0)    14936 2018-10-17 14:31:02.000000 docplex-2.8.125/docplex/mp/constants.py
--rw-rw-r--   0 root         (0) root         (0)    49277 2018-10-17 14:31:02.000000 docplex-2.8.125/docplex/mp/constr.py
--rw-rw-r--   0 root         (0) root         (0)    26906 2018-10-17 14:31:02.000000 docplex-2.8.125/docplex/mp/context.py
--rw-rw-r--   0 root         (0) root         (0)    98117 2018-10-17 14:31:02.000000 docplex-2.8.125/docplex/mp/cplex_engine.py
--rw-rw-r--   0 root         (0) root         (0)    22377 2018-10-17 14:31:02.000000 docplex-2.8.125/docplex/mp/docloud_connector.py
--rw-rw-r--   0 root         (0) root         (0)    34252 2018-10-17 14:31:00.000000 docplex-2.8.125/docplex/mp/docloud_engine.py
--rw-rw-r--   0 root         (0) root         (0)    22970 2018-10-17 14:31:00.000000 docplex-2.8.125/docplex/mp/engine.py
--rw-rw-r--   0 root         (0) root         (0)     4537 2018-10-17 14:31:02.000000 docplex-2.8.125/docplex/mp/engine_factory.py
--rw-rw-r--   0 root         (0) root         (0)     8485 2018-10-17 14:31:02.000000 docplex-2.8.125/docplex/mp/environment.py
--rw-rw-r--   0 root         (0) root         (0)     8376 2018-10-17 14:31:02.000000 docplex-2.8.125/docplex/mp/error_handler.py
--rw-rw-r--   0 root         (0) root         (0)     2228 2018-10-17 14:31:00.000000 docplex-2.8.125/docplex/mp/format.py
--rw-rw-r--   0 root         (0) root         (0)    19603 2018-10-17 14:31:02.000000 docplex-2.8.125/docplex/mp/functional.py
--rw-rw-r--   0 root         (0) root         (0)     6567 2018-10-17 14:31:00.000000 docplex-2.8.125/docplex/mp/kpi.py
--rw-rw-r--   0 root         (0) root         (0)    55106 2018-10-17 14:31:02.000000 docplex-2.8.125/docplex/mp/linear.py
--rw-rw-r--   0 root         (0) root         (0)    18845 2018-10-17 14:31:02.000000 docplex-2.8.125/docplex/mp/lp_printer.py
--rw-rw-r--   0 root         (0) root         (0)    40622 2018-10-17 14:31:02.000000 docplex-2.8.125/docplex/mp/mfactory.py
--rw-rw-r--   0 root         (0) root         (0)   223123 2018-10-17 14:31:02.000000 docplex-2.8.125/docplex/mp/model.py
--rw-rw-r--   0 root         (0) root         (0)    23493 2018-10-17 14:31:00.000000 docplex-2.8.125/docplex/mp/model_reader.py
--rw-rw-r--   0 root         (0) root         (0)    10901 2018-10-17 14:31:02.000000 docplex-2.8.125/docplex/mp/model_stats.py
--rw-rw-r--   0 root         (0) root         (0)    19329 2018-10-17 14:31:02.000000 docplex-2.8.125/docplex/mp/mprinter.py
--rw-rw-r--   0 root         (0) root         (0)     2218 2018-10-17 14:31:02.000000 docplex-2.8.125/docplex/mp/numutils.py
--rw-rw-r--   0 root         (0) root         (0)     3417 2018-10-17 14:31:02.000000 docplex-2.8.125/docplex/mp/operand.py
--rw-rw-r--   0 root         (0) root         (0)    11732 2018-10-17 14:31:02.000000 docplex-2.8.125/docplex/mp/ppretty.py
--rw-rw-r--   0 root         (0) root         (0)     1106 2018-10-17 14:31:00.000000 docplex-2.8.125/docplex/mp/printer_factory.py
--rw-rw-r--   0 root         (0) root         (0)    19431 2018-10-17 14:31:00.000000 docplex-2.8.125/docplex/mp/progress.py
--rw-rw-r--   0 root         (0) root         (0)    40813 2018-10-17 14:31:02.000000 docplex-2.8.125/docplex/mp/pwl.py
--rw-rw-r--   0 root         (0) root         (0)    25471 2018-10-17 14:31:02.000000 docplex-2.8.125/docplex/mp/quad.py
--rw-rw-r--   0 root         (0) root         (0)     7465 2018-10-17 14:31:02.000000 docplex-2.8.125/docplex/mp/quadfact.py
--rw-rw-r--   0 root         (0) root         (0)    24471 2018-10-17 14:31:02.000000 docplex-2.8.125/docplex/mp/relaxer.py
--rw-rw-r--   0 root         (0) root         (0)    15149 2018-10-17 14:31:02.000000 docplex-2.8.125/docplex/mp/sdetails.py
--rw-rw-r--   0 root         (0) root         (0)    42547 2018-10-17 14:31:02.000000 docplex-2.8.125/docplex/mp/solution.py
--rw-rw-r--   0 root         (0) root         (0)     4153 2018-10-17 14:31:02.000000 docplex-2.8.125/docplex/mp/sosvarset.py
--rw-rw-r--   0 root         (0) root         (0)     2095 2018-10-17 14:31:02.000000 docplex-2.8.125/docplex/mp/sttck.py
--rw-rw-r--   0 root         (0) root         (0)     1759 2018-10-17 14:31:02.000000 docplex-2.8.125/docplex/mp/sumfn.py
--rw-rw-r--   0 root         (0) root         (0)    19287 2018-10-17 14:31:02.000000 docplex-2.8.125/docplex/mp/tck.py
--rw-rw-r--   0 root         (0) root         (0)    29341 2018-10-17 14:31:02.000000 docplex-2.8.125/docplex/mp/utils.py
--rw-rw-r--   0 root         (0) root         (0)    11652 2018-10-17 14:31:02.000000 docplex-2.8.125/docplex/mp/vartype.py
--rw-rw-r--   0 root         (0) root         (0)     7973 2018-10-17 14:31:02.000000 docplex-2.8.125/docplex/mp/xcounter.py
-drwxrwxr-x   0 root         (0) root         (0)        0 2018-10-19 12:46:09.000000 docplex-2.8.125/docplex/util/
-drwxrwxr-x   0 root         (0) root         (0)        0 2018-10-19 12:46:09.000000 docplex-2.8.125/docplex/util/dods/
--rw-rw-r--   0 root         (0) root         (0)      340 2018-10-17 14:31:02.000000 docplex-2.8.125/docplex/util/dods/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     5025 2018-10-17 14:31:02.000000 docplex-2.8.125/docplex/util/dods/executor.py
--rw-rw-r--   0 root         (0) root         (0)     6971 2018-10-17 14:31:02.000000 docplex-2.8.125/docplex/util/dods/project_handler.py
--rw-rw-r--   0 root         (0) root         (0)      791 2018-10-17 14:31:00.000000 docplex-2.8.125/docplex/util/__init__.py
--rw-rw-r--   0 root         (0) root         (0)    38648 2018-10-17 14:31:00.000000 docplex-2.8.125/docplex/util/environment.py
--rw-rw-r--   0 root         (0) root         (0)     2376 2018-10-17 14:31:00.000000 docplex-2.8.125/docplex/util/logging_utils.py
--rw-rw-r--   0 root         (0) root         (0)     2786 2018-10-17 14:31:00.000000 docplex-2.8.125/docplex/util/status.py
--rw-rw-r--   0 root         (0) root         (0)      622 2018-10-17 14:30:56.000000 docplex-2.8.125/docplex/__init__.py
--rw-rw-r--   0 root         (0) root         (0)    13800 2018-10-17 14:30:56.000000 docplex-2.8.125/docplex/cli.py
--rw-rw-r--   0 root         (0) root         (0)      491 2018-10-17 14:40:14.000000 docplex-2.8.125/docplex/version.py
--rw-rw-r--   0 root         (0) root         (0)    14824 2018-10-17 14:40:14.000000 docplex-2.8.125/CHANGELOG.rst
--rw-rw-r--   0 root         (0) root         (0)    11350 2018-10-17 14:30:52.000000 docplex-2.8.125/LICENSE.txt
--rw-rw-r--   0 root         (0) root         (0)     1279 2018-10-17 14:30:52.000000 docplex-2.8.125/README.rst
--rw-rw-r--   0 root         (0) root         (0)       40 2018-10-17 14:30:52.000000 docplex-2.8.125/setup.cfg
--rw-rw-r--   0 root         (0) root         (0)     2880 2018-10-17 14:40:14.000000 docplex-2.8.125/setup.py
--rw-rw-r--   0 root         (0) root         (0)    30874 2018-10-19 12:46:09.000000 docplex-2.8.125/PKG-INFO
+drwxrwxr-x   0 root         (0) root         (0)        0 2019-03-14 11:18:48.000000 docplex-2.9.141/
+drwxrwxr-x   0 root         (0) root         (0)        0 2019-03-14 11:18:48.000000 docplex-2.9.141/docplex/
+drwxrwxr-x   0 root         (0) root         (0)        0 2019-03-14 11:18:48.000000 docplex-2.9.141/docplex/cp/
+drwxrwxr-x   0 root         (0) root         (0)        0 2019-03-14 11:18:48.000000 docplex-2.9.141/docplex/cp/fzn/
+-rw-rw-r--   0 root         (0) root         (0)      494 2019-03-13 10:42:28.000000 docplex-2.9.141/docplex/cp/fzn/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)    73140 2019-03-13 10:42:28.000000 docplex-2.9.141/docplex/cp/fzn/fzn_parser.py
+-rw-rw-r--   0 root         (0) root         (0)     3596 2019-03-13 10:42:28.000000 docplex-2.9.141/docplex/cp/fzn/fzn_tokenizer.py
+drwxrwxr-x   0 root         (0) root         (0)        0 2019-03-14 11:18:48.000000 docplex-2.9.141/docplex/cp/solver/
+-rw-rw-r--   0 root         (0) root         (0)      515 2019-03-13 10:42:28.000000 docplex-2.9.141/docplex/cp/solver/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)    11900 2019-03-13 10:42:28.000000 docplex-2.9.141/docplex/cp/solver/docloud_client.py
+-rw-rw-r--   0 root         (0) root         (0)    13238 2019-03-13 10:42:28.000000 docplex-2.9.141/docplex/cp/solver/environment_client.py
+-rw-rw-r--   0 root         (0) root         (0)    41328 2019-03-13 10:42:28.000000 docplex-2.9.141/docplex/cp/solver/solver.py
+-rw-rw-r--   0 root         (0) root         (0)     9765 2019-03-13 10:42:28.000000 docplex-2.9.141/docplex/cp/solver/solver_docloud.py
+-rw-rw-r--   0 root         (0) root         (0)    24032 2019-03-13 10:42:28.000000 docplex-2.9.141/docplex/cp/solver/solver_listener.py
+-rw-rw-r--   0 root         (0) root         (0)    19646 2019-03-13 10:42:28.000000 docplex-2.9.141/docplex/cp/solver/solver_local.py
+-rw-rw-r--   0 root         (0) root         (0)    11663 2019-03-13 10:42:28.000000 docplex-2.9.141/docplex/cp/solver/solver_simulator.py
+-rw-rw-r--   0 root         (0) root         (0)     1348 2019-03-13 10:42:22.000000 docplex-2.9.141/docplex/cp/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)    64467 2019-03-13 10:42:22.000000 docplex-2.9.141/docplex/cp/catalog.py
+-rw-rw-r--   0 root         (0) root         (0)    10598 2019-03-13 10:42:22.000000 docplex-2.9.141/docplex/cp/catalog_elements.py
+-rw-rw-r--   0 root         (0) root         (0)    21776 2019-03-13 10:42:22.000000 docplex-2.9.141/docplex/cp/config.py
+-rw-rw-r--   0 root         (0) root         (0)    40609 2019-03-13 10:42:22.000000 docplex-2.9.141/docplex/cp/cpo_compiler.py
+-rw-rw-r--   0 root         (0) root         (0)    31549 2019-03-13 10:42:22.000000 docplex-2.9.141/docplex/cp/cpo_parser.py
+-rw-rw-r--   0 root         (0) root         (0)     3781 2019-03-13 10:42:22.000000 docplex-2.9.141/docplex/cp/cpo_tokenizer.py
+-rw-rw-r--   0 root         (0) root         (0)    92720 2019-03-13 10:42:22.000000 docplex-2.9.141/docplex/cp/expression.py
+-rw-rw-r--   0 root         (0) root         (0)    20770 2019-03-13 10:42:22.000000 docplex-2.9.141/docplex/cp/function.py
+-rw-rw-r--   0 root         (0) root         (0)    62415 2019-03-13 10:42:22.000000 docplex-2.9.141/docplex/cp/model.py
+-rw-rw-r--   0 root         (0) root         (0)   179506 2019-03-13 10:42:22.000000 docplex-2.9.141/docplex/cp/modeler.py
+-rw-rw-r--   0 root         (0) root         (0)    58751 2019-03-13 10:42:22.000000 docplex-2.9.141/docplex/cp/parameters.py
+-rw-rw-r--   0 root         (0) root         (0)    72418 2019-03-13 10:42:22.000000 docplex-2.9.141/docplex/cp/solution.py
+-rw-rw-r--   0 root         (0) root         (0)    16931 2019-03-13 10:42:22.000000 docplex-2.9.141/docplex/cp/tokenizer.py
+-rw-rw-r--   0 root         (0) root         (0)    50181 2019-03-13 10:42:22.000000 docplex-2.9.141/docplex/cp/utils.py
+-rw-rw-r--   0 root         (0) root         (0)    61202 2019-03-13 10:42:22.000000 docplex-2.9.141/docplex/cp/utils_visu.py
+drwxrwxr-x   0 root         (0) root         (0)        0 2019-03-14 11:18:48.000000 docplex-2.9.141/docplex/mp/
+drwxrwxr-x   0 root         (0) root         (0)        0 2019-03-14 11:18:48.000000 docplex-2.9.141/docplex/mp/callbacks/
+-rw-rw-r--   0 root         (0) root         (0)      296 2019-03-13 10:42:32.000000 docplex-2.9.141/docplex/mp/callbacks/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     5360 2019-03-13 10:42:32.000000 docplex-2.9.141/docplex/mp/callbacks/cb_mixin.py
+drwxrwxr-x   0 root         (0) root         (0)        0 2019-03-14 11:18:48.000000 docplex-2.9.141/docplex/mp/internal/
+-rw-rw-r--   0 root         (0) root         (0)      314 2019-03-13 10:42:32.000000 docplex-2.9.141/docplex/mp/internal/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     3167 2019-03-13 10:42:32.000000 docplex-2.9.141/docplex/mp/internal/json_conflict_handler.py
+-rw-rw-r--   0 root         (0) root         (0)      790 2019-03-13 10:42:32.000000 docplex-2.9.141/docplex/mp/internal/json_infeasibility_handler.py
+-rw-rw-r--   0 root         (0) root         (0)     4181 2019-03-13 10:42:32.000000 docplex-2.9.141/docplex/mp/internal/json_solution_handler.py
+drwxrwxr-x   0 root         (0) root         (0)        0 2019-03-14 11:18:48.000000 docplex-2.9.141/docplex/mp/params/
+-rw-rw-r--   0 root         (0) root         (0)      361 2019-03-13 10:42:32.000000 docplex-2.9.141/docplex/mp/params/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     1763 2019-03-13 10:42:32.000000 docplex-2.9.141/docplex/mp/params/cplex_params.py
+-rw-rw-r--   0 root         (0) root         (0)    35064 2019-03-13 10:42:32.000000 docplex-2.9.141/docplex/mp/params/parameter_hierarchy_12620.py
+-rw-rw-r--   0 root         (0) root         (0)    35478 2019-03-13 10:42:32.000000 docplex-2.9.141/docplex/mp/params/parameter_hierarchy_12630.py
+-rw-rw-r--   0 root         (0) root         (0)    37277 2019-03-13 10:42:32.000000 docplex-2.9.141/docplex/mp/params/parameter_hierarchy_12700.py
+-rw-rw-r--   0 root         (0) root         (0)    37425 2019-03-13 10:42:32.000000 docplex-2.9.141/docplex/mp/params/parameter_hierarchy_12710.py
+-rw-rw-r--   0 root         (0) root         (0)    40443 2019-03-13 10:42:32.000000 docplex-2.9.141/docplex/mp/params/parameter_hierarchy_12800.py
+-rw-rw-r--   0 root         (0) root         (0)    40773 2019-03-13 10:44:40.000000 docplex-2.9.141/docplex/mp/params/parameter_hierarchy_12900.py
+-rw-rw-r--   0 root         (0) root         (0)    29889 2019-03-13 10:42:32.000000 docplex-2.9.141/docplex/mp/params/parameters.py
+drwxrwxr-x   0 root         (0) root         (0)        0 2019-03-14 11:18:48.000000 docplex-2.9.141/docplex/mp/sktrans/
+-rw-rw-r--   0 root         (0) root         (0)      316 2019-03-13 10:42:32.000000 docplex-2.9.141/docplex/mp/sktrans/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     9813 2019-03-13 10:42:32.000000 docplex-2.9.141/docplex/mp/sktrans/cpx_mdlr.py
+-rw-rw-r--   0 root         (0) root         (0)     4530 2019-03-13 10:42:32.000000 docplex-2.9.141/docplex/mp/sktrans/docplex_mdlr.py
+-rw-rw-r--   0 root         (0) root         (0)      843 2019-03-13 10:42:32.000000 docplex-2.9.141/docplex/mp/sktrans/modeler.py
+-rw-rw-r--   0 root         (0) root         (0)      954 2019-03-13 10:42:32.000000 docplex-2.9.141/docplex/mp/sktrans/pd_utils.py
+-rw-rw-r--   0 root         (0) root         (0)    14045 2019-03-13 10:42:32.000000 docplex-2.9.141/docplex/mp/sktrans/transformers.py
+drwxrwxr-x   0 root         (0) root         (0)        0 2019-03-14 11:18:48.000000 docplex-2.9.141/docplex/mp/sparktrans/
+-rw-rw-r--   0 root         (0) root         (0)      316 2019-03-13 10:42:32.000000 docplex-2.9.141/docplex/mp/sparktrans/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)      541 2019-03-13 10:42:32.000000 docplex-2.9.141/docplex/mp/sparktrans/spark_utils.py
+-rw-rw-r--   0 root         (0) root         (0)    13041 2019-03-13 10:42:32.000000 docplex-2.9.141/docplex/mp/sparktrans/transformers.py
+drwxrwxr-x   0 root         (0) root         (0)        0 2019-03-14 11:18:48.000000 docplex-2.9.141/docplex/mp/worker/
+-rw-rw-r--   0 root         (0) root         (0)      322 2019-03-13 10:42:32.000000 docplex-2.9.141/docplex/mp/worker/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     1755 2019-03-13 10:42:32.000000 docplex-2.9.141/docplex/mp/worker/solve_hook.py
+-rw-rw-r--   0 root         (0) root         (0)      584 2019-03-13 10:42:32.000000 docplex-2.9.141/docplex/mp/worker/worker_env.py
+-rw-rw-r--   0 root         (0) root         (0)     1467 2019-03-13 10:42:30.000000 docplex-2.9.141/docplex/mp/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     2728 2019-03-13 10:42:30.000000 docplex-2.9.141/docplex/mp/absmodel.py
+-rw-rw-r--   0 root         (0) root         (0)    29114 2019-03-13 10:42:30.000000 docplex-2.9.141/docplex/mp/advmodel.py
+-rw-rw-r--   0 root         (0) root         (0)    13490 2019-03-13 10:42:30.000000 docplex-2.9.141/docplex/mp/aggregator.py
+-rw-rw-r--   0 root         (0) root         (0)     4065 2019-03-13 10:42:30.000000 docplex-2.9.141/docplex/mp/anno.py
+-rw-rw-r--   0 root         (0) root         (0)    15562 2019-03-13 10:42:30.000000 docplex-2.9.141/docplex/mp/basic.py
+-rw-rw-r--   0 root         (0) root         (0)     3042 2019-03-13 10:42:30.000000 docplex-2.9.141/docplex/mp/cloudutils.py
+-rw-rw-r--   0 root         (0) root         (0)     1789 2019-03-13 10:42:30.000000 docplex-2.9.141/docplex/mp/compat23.py
+-rw-rw-r--   0 root         (0) root         (0)    12343 2019-03-13 10:42:30.000000 docplex-2.9.141/docplex/mp/conflict_refiner.py
+-rw-rw-r--   0 root         (0) root         (0)    15505 2019-03-13 10:42:30.000000 docplex-2.9.141/docplex/mp/constants.py
+-rw-rw-r--   0 root         (0) root         (0)    50808 2019-03-13 10:42:30.000000 docplex-2.9.141/docplex/mp/constr.py
+-rw-rw-r--   0 root         (0) root         (0)    26294 2019-03-13 10:42:30.000000 docplex-2.9.141/docplex/mp/context.py
+-rw-rw-r--   0 root         (0) root         (0)   110486 2019-03-13 10:42:30.000000 docplex-2.9.141/docplex/mp/cplex_engine.py
+-rw-rw-r--   0 root         (0) root         (0)    22377 2019-03-13 10:42:30.000000 docplex-2.9.141/docplex/mp/docloud_connector.py
+-rw-rw-r--   0 root         (0) root         (0)    34122 2019-03-13 10:42:30.000000 docplex-2.9.141/docplex/mp/docloud_engine.py
+-rw-rw-r--   0 root         (0) root         (0)    23945 2019-03-13 10:42:30.000000 docplex-2.9.141/docplex/mp/engine.py
+-rw-rw-r--   0 root         (0) root         (0)     4537 2019-03-13 10:42:30.000000 docplex-2.9.141/docplex/mp/engine_factory.py
+-rw-rw-r--   0 root         (0) root         (0)     8485 2019-03-13 10:42:30.000000 docplex-2.9.141/docplex/mp/environment.py
+-rw-rw-r--   0 root         (0) root         (0)     8376 2019-03-13 10:42:30.000000 docplex-2.9.141/docplex/mp/error_handler.py
+-rw-rw-r--   0 root         (0) root         (0)     5065 2019-03-13 10:42:30.000000 docplex-2.9.141/docplex/mp/format.py
+-rw-rw-r--   0 root         (0) root         (0)    19230 2019-03-13 10:42:30.000000 docplex-2.9.141/docplex/mp/functional.py
+-rw-rw-r--   0 root         (0) root         (0)     7467 2019-03-13 10:42:30.000000 docplex-2.9.141/docplex/mp/kpi.py
+-rw-rw-r--   0 root         (0) root         (0)    58765 2019-03-13 10:42:30.000000 docplex-2.9.141/docplex/mp/linear.py
+-rw-rw-r--   0 root         (0) root         (0)    18952 2019-03-13 10:42:30.000000 docplex-2.9.141/docplex/mp/lp_printer.py
+-rw-rw-r--   0 root         (0) root         (0)    42085 2019-03-13 10:42:30.000000 docplex-2.9.141/docplex/mp/mfactory.py
+-rw-rw-r--   0 root         (0) root         (0)   239134 2019-03-13 10:42:30.000000 docplex-2.9.141/docplex/mp/model.py
+-rw-rw-r--   0 root         (0) root         (0)    25324 2019-03-13 10:42:30.000000 docplex-2.9.141/docplex/mp/model_reader.py
+-rw-rw-r--   0 root         (0) root         (0)    10901 2019-03-13 10:42:30.000000 docplex-2.9.141/docplex/mp/model_stats.py
+-rw-rw-r--   0 root         (0) root         (0)    19142 2019-03-13 10:42:30.000000 docplex-2.9.141/docplex/mp/mprinter.py
+-rw-rw-r--   0 root         (0) root         (0)     2218 2019-03-13 10:42:30.000000 docplex-2.9.141/docplex/mp/numutils.py
+-rw-rw-r--   0 root         (0) root         (0)     3605 2019-03-13 10:42:30.000000 docplex-2.9.141/docplex/mp/operand.py
+-rw-rw-r--   0 root         (0) root         (0)    11732 2019-03-13 10:42:30.000000 docplex-2.9.141/docplex/mp/ppretty.py
+-rw-rw-r--   0 root         (0) root         (0)     1106 2019-03-13 10:42:30.000000 docplex-2.9.141/docplex/mp/printer_factory.py
+-rw-rw-r--   0 root         (0) root         (0)    19431 2019-03-13 10:42:30.000000 docplex-2.9.141/docplex/mp/progress.py
+-rw-rw-r--   0 root         (0) root         (0)    40769 2019-03-13 10:42:30.000000 docplex-2.9.141/docplex/mp/pwl.py
+-rw-rw-r--   0 root         (0) root         (0)    25713 2019-03-13 10:42:30.000000 docplex-2.9.141/docplex/mp/quad.py
+-rw-rw-r--   0 root         (0) root         (0)     7465 2019-03-13 10:42:30.000000 docplex-2.9.141/docplex/mp/quadfact.py
+-rw-rw-r--   0 root         (0) root         (0)    27310 2019-03-13 10:42:30.000000 docplex-2.9.141/docplex/mp/relaxer.py
+-rw-rw-r--   0 root         (0) root         (0)    16261 2019-03-13 10:42:30.000000 docplex-2.9.141/docplex/mp/sdetails.py
+-rw-rw-r--   0 root         (0) root         (0)     5636 2019-03-13 10:42:30.000000 docplex-2.9.141/docplex/mp/solmst.py
+-rw-rw-r--   0 root         (0) root         (0)    42749 2019-03-13 10:42:30.000000 docplex-2.9.141/docplex/mp/solution.py
+-rw-rw-r--   0 root         (0) root         (0)     4153 2019-03-13 10:42:30.000000 docplex-2.9.141/docplex/mp/sosvarset.py
+-rw-rw-r--   0 root         (0) root         (0)     2842 2019-03-13 10:42:30.000000 docplex-2.9.141/docplex/mp/sttck.py
+-rw-rw-r--   0 root         (0) root         (0)     1759 2019-03-13 10:42:30.000000 docplex-2.9.141/docplex/mp/sumfn.py
+-rw-rw-r--   0 root         (0) root         (0)    20513 2019-03-13 10:42:30.000000 docplex-2.9.141/docplex/mp/tck.py
+-rw-rw-r--   0 root         (0) root         (0)    34798 2019-03-13 10:42:30.000000 docplex-2.9.141/docplex/mp/utils.py
+-rw-rw-r--   0 root         (0) root         (0)    11652 2019-03-13 10:42:30.000000 docplex-2.9.141/docplex/mp/vartype.py
+-rw-rw-r--   0 root         (0) root         (0)     7973 2019-03-13 10:42:30.000000 docplex-2.9.141/docplex/mp/xcounter.py
+drwxrwxr-x   0 root         (0) root         (0)        0 2019-03-14 11:18:48.000000 docplex-2.9.141/docplex/util/
+drwxrwxr-x   0 root         (0) root         (0)        0 2019-03-14 11:18:48.000000 docplex-2.9.141/docplex/util/dods/
+-rw-rw-r--   0 root         (0) root         (0)      340 2019-03-13 10:42:30.000000 docplex-2.9.141/docplex/util/dods/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     5025 2019-03-13 10:42:30.000000 docplex-2.9.141/docplex/util/dods/executor.py
+-rw-rw-r--   0 root         (0) root         (0)     6971 2019-03-13 10:42:30.000000 docplex-2.9.141/docplex/util/dods/project_handler.py
+-rw-rw-r--   0 root         (0) root         (0)      791 2019-03-13 10:42:28.000000 docplex-2.9.141/docplex/util/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)    39493 2019-03-13 10:42:28.000000 docplex-2.9.141/docplex/util/environment.py
+-rw-rw-r--   0 root         (0) root         (0)     2376 2019-03-13 10:42:28.000000 docplex-2.9.141/docplex/util/logging_utils.py
+-rw-rw-r--   0 root         (0) root         (0)     2786 2019-03-13 10:42:28.000000 docplex-2.9.141/docplex/util/status.py
+-rw-rw-r--   0 root         (0) root         (0)      622 2019-03-13 10:42:24.000000 docplex-2.9.141/docplex/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)    16751 2019-03-13 10:42:24.000000 docplex-2.9.141/docplex/cli.py
+-rw-rw-r--   0 root         (0) root         (0)      491 2019-03-13 10:48:54.000000 docplex-2.9.141/docplex/version.py
+-rw-rw-r--   0 root         (0) root         (0)    15332 2019-03-13 10:48:54.000000 docplex-2.9.141/CHANGELOG.rst
+-rw-rw-r--   0 root         (0) root         (0)    11350 2019-03-13 10:42:22.000000 docplex-2.9.141/LICENSE.txt
+-rw-rw-r--   0 root         (0) root         (0)     1277 2019-03-13 10:42:22.000000 docplex-2.9.141/README.rst
+-rw-rw-r--   0 root         (0) root         (0)       40 2019-03-13 10:42:22.000000 docplex-2.9.141/setup.cfg
+-rw-rw-r--   0 root         (0) root         (0)     2880 2019-03-13 10:48:54.000000 docplex-2.9.141/setup.py
+-rw-rw-r--   0 root         (0) root         (0)    31492 2019-03-14 11:18:48.000000 docplex-2.9.141/PKG-INFO
```

### Comparing `docplex-2.8.125/docplex/cp/fzn/fzn_parser.py` & `docplex-2.9.141/docplex/cp/fzn/fzn_parser.py`

 * *Files identical despite different names*

### Comparing `docplex-2.8.125/docplex/cp/fzn/fzn_tokenizer.py` & `docplex-2.9.141/docplex/cp/fzn/fzn_tokenizer.py`

 * *Files identical despite different names*

### Comparing `docplex-2.8.125/docplex/cp/solver/__init__.py` & `docplex-2.9.141/docplex/cp/solver/__init__.py`

 * *Files identical despite different names*

### Comparing `docplex-2.8.125/docplex/cp/solver/docloud_client.py` & `docplex-2.9.141/docplex/cp/solver/docloud_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,16 @@
 # Author: Olivier OUDOT, IBM Analytics, France Lab, Sophia-Antipolis
 #         with help from previous version written by Viu LONG KONG
 
 """
 This module implements a DOcplexcloud client allowing to submit a CPO model for solving on DOcplexcloud.
 """
 
-import time, json, requests
+import time, json
+import requests
 
 from docplex.cp.utils import CpoException, is_symbol_char, Context
 
 
 ###############################################################################
 ##  Constants
 ###############################################################################
```

### Comparing `docplex-2.8.125/docplex/cp/solver/solver.py` & `docplex-2.9.141/docplex/cp/solver/solver.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # --------------------------------------------------------------------------
 # Source file provided under Apache License, Version 2.0, January 2004,
 # http://www.apache.org/licenses/
-# (c) Copyright IBM Corp. 2015, 2016
+# (c) Copyright IBM Corp. 2015, 2016, 2017, 2018
 # --------------------------------------------------------------------------
 # Author: Olivier OUDOT, IBM Analytics, France Lab, Sophia-Antipolis
 
 """
 This module implements appropriate software to solve a CPO model represented by a
 :class:`docplex.cp.model.CpoModel` object.
 
@@ -56,15 +56,14 @@
 --------------------
 """
 
 import docplex.cp.config as config
 from docplex.cp.utils import CpoException, CpoNotSupportedException, make_directories, Context, is_array, is_string, parse_json_string
 import docplex.cp.utils as utils
 from docplex.cp.cpo_compiler import CpoCompiler
-import docplex.cp.solver.environment_client as runenv
 from docplex.cp.solution import *
 from docplex.cp.solver.solver_listener import CpoSolverListener
 
 import time, importlib, inspect
 import traceback
 import threading
 
@@ -274,14 +273,17 @@
         # Dump in dump directory if required
         if ctx.model.dump_directory:
             stime = time.time()
             make_directories(ctx.model.dump_directory)
             mname = self.model.get_name()
             if mname is None:
                 mname = "Anonymous"
+            else:
+                # Remove special characters introduced by Jupyter
+                mname = mname.replace('<', '').replace('>', '')
             file = ctx.model.dump_directory + "/" + mname + ".cpo"
             with utils.open_utf8(file, 'w') as f:
                 f.write(cpostr)
             self.process_infos.incr(CpoProcessInfos.MODEL_DUMP_TIME, time.time() - stime)
 
         # Return
         return cpostr
@@ -428,18 +430,23 @@
         # Save attributes
         self.model = model
         self.context = context
 
         # Determine appropriate solver agent
         self.agent = self._get_solver_agent()
 
-        # Add solver listener for environment
-        env = runenv.get_environment()
-        if env is not None:
-            self.add_listener(runenv.EnvSolverListener())
+        # Add configured default listeners if any
+        # Note: calling solver_created() is not required as it is done by add_listener().
+        lstnrs = context.solver.listeners
+        if lstnrs is not None:
+            if is_array(lstnrs):
+                for lstnr in lstnrs:
+                    self._add_listener_from_class(lstnr)
+            else:
+                self._add_listener_from_class(lstnrs)
 
 
     def __iter__(self):
         """  Define solver as an iterator """
         return self
 
 
@@ -569,15 +576,15 @@
                 # Search has been aborted externally
                 for lstnr in self.listeners:
                     lstnr.end_solve(self)
                 self._set_status(STATUS_RELEASED)
                 self.last_result = self._create_solution_aborted()
                 return self.last_result
             else:
-                #traceback.print_exc()
+                traceback.print_exc()
                 raise e
         self._set_status(STATUS_SEARCH_WAITING)
         stime = time.time() - stime
         self.context.solver.log(1, "Model '", self.model.get_name(), "' next solution in ", round(stime, 2), " sec.")
 
         # Set solve time in solution if not done
         if msol.get_solve_time() == 0:
@@ -645,18 +652,31 @@
 
         Returns:
             List of constraints that cause the conflict,
             object of class :class:`~docplex.cp.solution.CpoRefineConflictResult`.
         Raises:
             CpoNotSupportedException: if method not available in the solver agent.
         """
+        # Start refine conflict
         self._check_status(STATUS_IDLE)
         self._set_status(STATUS_REFINING_CONFLICT)
+        for lstnr in self.listeners:
+            lstnr.start_refine_conflict(self)
+
+        # Start refine conflict
         msol = self.agent.refine_conflict()
+        for lstnr in self.listeners:
+            lstnr.conflict_found(self, msol)
+
+        # End refine conflict
         self._set_status(STATUS_IDLE)
+        for lstnr in self.listeners:
+            lstnr.end_refine_conflict(self)
+
+
         return msol
 
 
     def propagate(self):
         """ This method invokes the propagation on the current model.
 
         Constraint propagation is the process of communicating the domain reduction of a decision variable to
@@ -787,14 +807,40 @@
         assert isinstance(lstnr, CpoSolverListener), \
             "Listener should be an object of class docplex.cp.solver.solver_listener.CpoSolverListener"
         self.listeners.append(lstnr)
         # Notify listener
         lstnr.solver_created(self)
 
 
+    def _add_listener_from_class(self, lstnr):
+        """ Add a solver listener from its class (instance is created).
+
+        Args:
+            lstnr:  Solver listener class, or string identifying the class
+        """
+        if is_string(lstnr):
+            # Get listener class from string
+            try:
+                lclass = utils.get_module_element_from_path(lstnr)
+            except Exception as e:
+                raise CpoException("Unable to retrieve solver listener class '{}': {}".format(lstnr, e))
+            if not inspect.isclass(lclass):
+                raise CpoException("Solver listener '{}' is not a class.".format(lstnr))
+            if not issubclass(lclass, CpoSolverListener):
+                raise CpoException("Solver listener class '{}' should extend CpoSolverListener.".format(lstnr))
+        else:
+            # Listener is assumed to directly be a class
+            lclass = lstnr
+            if not inspect.isclass(lclass):
+                raise CpoException("Solver listener '{}' is not a class.".format(lclass))
+            if not issubclass(lclass, CpoSolverListener):
+                raise CpoException("Solver listener class '{}' should extend CpoSolverListener.".format(lclass))
+        # Add listener
+        self.add_listener(lclass())
+
     def remove_listener(self, lstnr):
         """ Remove a solver listener previously added with :meth:`~docplex.cp.solver.solver.CpoSolver.add_listener`.
 
         Args:
             lstnr:  Listener to remove.
         """
         self.listeners.remove(lstnr)
@@ -930,37 +976,25 @@
         if not isinstance(sctx, Context):
             raise CpoException("Unknown solving agent '" + aname + "'. Check config.context.solver.agent parameter.")
         if sctx.is_log_enabled(3):
             sctx.log(3, "Context for solving agent '", aname, "':")
             sctx.write(out=sctx.get_log_output())
         cpath = sctx.class_name
         if cpath is None:
-            raise CpoException("Solving agent '" + aname + "' context does not contain attribute 'class_name'")
+            raise CpoException("Solving agent '" + aname + "' context should contain an attribute 'class_name'")
 
-        # Split class name
-        pnx = cpath.rfind('.')
-        if pnx < 0:
-            raise CpoException("Invalid class name '" + cpath + "' for solving agent '" + aname + "'. Should be <package>.<module>.<class>.")
-        mname = cpath[:pnx]
-        cname = cpath[pnx + 1:]
-
-        # Load module
+        # Retrieve solver agent class
         try:
-            module = importlib.import_module(mname)
+            sclass = utils.get_module_element_from_path(cpath)
         except Exception as e:
-            raise CpoException("Module '" + mname + "' import error: " + str(e))
-
-        # Create and check class
-        sclass = getattr(module, cname, None)
-        if sclass is None:
-            raise CpoException("Module '" + mname + "' does not contain a class '" + cname + "'")
+            raise CpoException("Unable to retrieve solver agent class '{}': {}".format(cpath, e))
         if not inspect.isclass(sclass):
-            raise CpoException("Agent class '" + cpath + "' is not a class.")
+            raise CpoException("Solver agent '{}' is not a class.".format(cpath))
         if not issubclass(sclass, CpoSolverAgent):
-            raise CpoException("Solver agent class '" + cpath + "' does not extend CpoSolverAgent.")
+            raise CpoException("Solver agent class '{}' should extend CpoSolverAgent.".format(cpath))
 
         # Create agent instance
         agent = sclass(self, sctx.params, sctx)
         return agent
 
 
 ###############################################################################
```

### Comparing `docplex-2.8.125/docplex/cp/solver/solver_docloud.py` & `docplex-2.9.141/docplex/cp/solver/solver_docloud.py`

 * *Files identical despite different names*

### Comparing `docplex-2.8.125/docplex/cp/solver/solver_listener.py` & `docplex-2.9.141/docplex/cp/solver/solver_listener.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # --------------------------------------------------------------------------
 # Source file provided under Apache License, Version 2.0, January 2004,
 # http://www.apache.org/licenses/
-# (c) Copyright IBM Corp. 2015, 2016
+# (c) Copyright IBM Corp. 2017, 2018
 # --------------------------------------------------------------------------
 # Author: Olivier OUDOT, IBM Analytics, France Lab, Sophia-Antipolis
 
 """
 This module defines the class :class:`CpoSolverListener` that allows to be warned about different steps of the solve.
 
 Any number of listeners can be added to a solver using the method :meth:`docplex.cp.solver.solver.CpoSolver.add_listener`.
@@ -39,18 +39,14 @@
 class CpoSolverListener(object):
     """ Solve listener allowing to be warned about different solving steps.
 
     This class is an 'abstract' class that must be extended by actual listener implementation.
     All method of this class are empty.
     """
 
-    def __init__(self):
-        super(CpoSolverListener, self).__init__()
-
-
     def solver_created(self, solver):
         """ Notify the listener that the solver object has been created.
 
         Args:
             solver: Originator CPO solver (object of class :class:`~docplex.cp.solver.solver.CpoSolver`)
         """
         pass
@@ -86,24 +82,42 @@
         Args:
             solver: Originator CPO solver (object of class :class:`~docplex.cp.solver.solver.CpoSolver`)
             sres:   Solve result, object of class :class:`~docplex.cp.solution.CpoSolveResult`
         """
         pass
 
 
-    def solution_found(self, solver, msol):
-        """ Signal that a solution has been found.
+    def start_refine_conflict(self, solver):
+        """ Notify that the refine conflict is started.
+
+        Args:
+            solver: Originator CPO solver (object of class :class:`~docplex.cp.solver.solver.CpoSolver`)
+        """
+        pass
 
-        Deprecated. Use :meth:`result_found` instead.
+
+    def end_refine_conflict(self, solver):
+        """ Notify that the refine conflict is ended.
 
         Args:
             solver: Originator CPO solver (object of class :class:`~docplex.cp.solver.solver.CpoSolver`)
-            msol:   Model solution, object of class :class:`~docplex.cp.solution.CpoSolveResult`
         """
-        self.solution_found(solver, msol)
+        pass
+
+
+    def conflict_found(self, solver, cflct):
+        """ Signal that a conflict has been found.
+
+        This method is called when a conflict result is found by the solver when method refine_conflict() is called.
+
+        Args:
+            solver: Originator CPO solver (object of class :class:`~docplex.cp.solver.solver.CpoSolver`)
+            cflct:  Conflict descriptor, object of class :class:`~docplex.cp.solution.CpoRefineConflictResult`
+        """
+        pass
 
 
     def new_log_data(self, solver, data):
         """ Signal a new peace of log data.
 
         Args:
             solver: Originator CPO solver (object of class :class:`~docplex.cp.solver.solver.CpoSolver`)
```

### Comparing `docplex-2.8.125/docplex/cp/solver/solver_local.py` & `docplex-2.9.141/docplex/cp/solver/solver_local.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # --------------------------------------------------------------------------
 # Source file provided under Apache License, Version 2.0, January 2004,
 # http://www.apache.org/licenses/
-# (c) Copyright IBM Corp. 2015, 2016
+# (c) Copyright IBM Corp. 2016, 2017, 2018
 # --------------------------------------------------------------------------
 # Author: Olivier OUDOT, IBM Analytics, France Lab, Sophia-Antipolis
 
 """
 This module allows to solve a model expressed as a CPO file using
 a local CP Optimizer Interactive (cpoptimizer(.exe)).
 """
@@ -496,15 +496,15 @@
                         raise LocalSolverException("Nothing to read from local solver process. Check its availability.")
                 else:
                     try:
                         self.process.wait()
                         rc = self.process.returncode
                     except:
                         rc = "unknown"
-                    raise LocalSolverException("Nothing to read from local solver process. Process seems to have been stopped (current rc={}).".format(rc))
+                    raise LocalSolverException("Nothing to read from local solver process. Process seems to have been stopped (rc={}).".format(rc))
             else:
                 raise LocalSolverException("Read only {} bytes when {} was expected.".format(len(data), nbb))
 
         # Return
         if IS_PYTHON_2:
             return bytearray(data)
         return data
```

### Comparing `docplex-2.8.125/docplex/cp/solver/solver_simulator.py` & `docplex-2.9.141/docplex/cp/solver/solver_simulator.py`

 * *Files identical despite different names*

### Comparing `docplex-2.8.125/docplex/cp/__init__.py` & `docplex-2.9.141/docplex/cp/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -20,14 +20,14 @@
 psyst = platform.system()
 if psyst.lower() not in ('darwin', 'linux', 'windows', 'microsoft', 'aix'):
     msg = "DOcplex.CP is supported on Linux, Windows, Darwin and AIX, not on '{}'. Use it at your own risk.".format(psyst)
     warnings.warn(msg, RuntimeWarning)
 
 # Check version of Python
 pv = sys.version_info
-if (pv < (2, 7)) or ((pv[0] == 3) and (pv < (3, 4) or pv >= (3, 7))):
-    msg = "DOcplex.CP is supported by Python versions 2.7.9+, 3.4.x, 3.5.x and 3.6.x, not '{}'. Use it at your own risk."\
+if (pv < (2, 7)) or ((pv[0] == 3) and (pv < (3, 4) or pv >= (3, 8))):
+    msg = "DOcplex.CP is supported by Python versions 2.7.9+, 3.4.x, to 3.7.x, not '{}'. Use it at your own risk."\
         .format('.'.join(str(x) for x in pv))
     warnings.warn(msg, RuntimeWarning)
 
 # Set version information
 __version_info__ = (dcpv.docplex_version_major, dcpv.docplex_version_minor, dcpv.docplex_version_micro)
```

### Comparing `docplex-2.8.125/docplex/cp/catalog.py` & `docplex-2.9.141/docplex/cp/catalog.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # --------------------------------------------------------------------------
 # Source file provided under Apache License, Version 2.0, January 2004,
 # http://www.apache.org/licenses/
-# (c) Copyright IBM Corp. 2015, 2016
+# (c) Copyright IBM Corp. 2015, 2016, 2017, 2018
 # --------------------------------------------------------------------------
 # Generated automatically
 
 """
 This module contains the Python descriptors of the different CPO types and operations.
 """
```

### Comparing `docplex-2.8.125/docplex/cp/catalog_elements.py` & `docplex-2.9.141/docplex/cp/catalog_elements.py`

 * *Files identical despite different names*

### Comparing `docplex-2.8.125/docplex/cp/config.py` & `docplex-2.9.141/docplex/cp/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # --------------------------------------------------------------------------
 # Source file provided under Apache License, Version 2.0, January 2004,
 # http://www.apache.org/licenses/
-# (c) Copyright IBM Corp. 2015, 2016
+# (c) Copyright IBM Corp. 2015, 2016, 2017, 2018
 # --------------------------------------------------------------------------
 
 """
 Configuration of the CP Optimizer Python API
 
 This module is the top-level handler of the configuration parameters for
 the CP Optimizer Python API. It contains the default values of the different
@@ -272,15 +272,15 @@
 # Minimal variable name length that trigger use of shorter alias. None for no alias.
 context.model.length_for_alias = 15
 
 # Automatically add a name to every top-level constraint
 context.model.name_all_constraints = False
 
 # Model format generation version
-context.model.version = '12.8.0.0'
+context.model.version = '12.9.0.0'
 
 # Name of the directory where store copy of the generated CPO files. None for no dump.
 context.model.dump_directory = None
 
 # Flag to generate short model output (internal)
 context.model.short_output = False
 
@@ -348,14 +348,23 @@
 
 # Indicate to auto-publish results in environment
 context.solver.auto_publish.result_output = "solution.json"
 
 # Indicate to auto-publish kpis in environment
 context.solver.auto_publish.kpis_output = "kpis.csv"
 
+# Indicate to auto-publish conflicts in environment
+context.solver.auto_publish.conflicts_output = "conflicts.csv"
+
+# Indicate to enable auto-publish also with local environment
+context.solver.auto_publish.local_publish = False
+
+# Default solver listeners
+context.solver.listeners = ["docplex.cp.solver.environment_client.EnvSolverListener"]
+
 
 #-----------------------------------------------------------------------------
 # Local solving agent context
 
 context.solver.local = Context()
 
 # Python class implementing the agent
```

### Comparing `docplex-2.8.125/docplex/cp/cpo_compiler.py` & `docplex-2.9.141/docplex/cp/cpo_compiler.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # --------------------------------------------------------------------------
 # Source file provided under Apache License, Version 2.0, January 2004,
 # http://www.apache.org/licenses/
-# (c) Copyright IBM Corp. 2015, 2016
+# (c) Copyright IBM Corp. 2015, 2016, 2017, 2018
 # --------------------------------------------------------------------------
 # Author: Olivier OUDOT, IBM Analytics, France Lab, Sophia-Antipolis
 
 """
 Compiler converting internal model representation to CPO file format.
 """
```

### Comparing `docplex-2.8.125/docplex/cp/cpo_parser.py` & `docplex-2.9.141/docplex/cp/cpo_parser.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # --------------------------------------------------------------------------
 # Source file provided under Apache License, Version 2.0, January 2004,
 # http://www.apache.org/licenses/
-# (c) Copyright IBM Corp. 2015, 2016
+# (c) Copyright IBM Corp. 2015, 2016, 2017, 2018
 # --------------------------------------------------------------------------
 # Author: Olivier OUDOT, IBM Analytics, France Lab, Sophia-Antipolis
 
 """
 Parser converting a CPO file to internal model representation.
 """
 
@@ -23,15 +23,15 @@
 ## Constants
 ###############################################################################
 
 # Minimum CPO format version number
 MIN_CPO_VERSION_NUMBER = "12.6.0.0"
 
 # Maximum CPO format version number
-MAX_CPO_VERSION_NUMBER = "12.8.0.0"
+MAX_CPO_VERSION_NUMBER = "12.9.0.0"
 
 # Map of all operators. Key is operator, value is list of corresponding operation descriptors
 _ALL_OPERATORS = {}
 
 # Map of all operations. Key is CPO operation name, value is list corresponding operation descriptor
 _ALL_OPERATIONS = {}
 
@@ -618,18 +618,18 @@
         # Skip all until section end
         tok = self._next_token()
         while (tok is not TOKEN_EOF) and (tok.value != '}'):
             if self.token.value == "version":
                 self._check_token(self._next_token(), TOKEN_PARENT_OPEN)
                 ver = self._next_token().get_string()
                 self.model.set_format_version(ver)
-                if ver < MIN_CPO_VERSION_NUMBER:
+                if compare_natural(ver, MIN_CPO_VERSION_NUMBER) < 0:
                     raise CpoUnsupportedFormatVersionException("Can not parse a CPO file with version {}, lower than {}"
                                                                .format(ver, MIN_CPO_VERSION_NUMBER))
-                if ver > MAX_CPO_VERSION_NUMBER:
+                if compare_natural(ver, MAX_CPO_VERSION_NUMBER) > 0:
                     raise CpoUnsupportedFormatVersionException("Can not parse a CPO file with version {}, greater than {}"
                                                                .format(ver, MAX_CPO_VERSION_NUMBER))
                 self._check_token(self._next_token(), TOKEN_PARENT_CLOSE)
             tok = self._next_token()
 
 
     def _read_section_search(self):
```

### Comparing `docplex-2.8.125/docplex/cp/cpo_tokenizer.py` & `docplex-2.9.141/docplex/cp/cpo_tokenizer.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # --------------------------------------------------------------------------
 # Source file provided under Apache License, Version 2.0, January 2004,
 # http://www.apache.org/licenses/
-# (c) Copyright IBM Corp. 2015, 2016, 2017
+# (c) Copyright IBM Corp. 2015, 2016, 2017, 2018
 # --------------------------------------------------------------------------
 # Author: Olivier OUDOT, IBM Analytics, France Lab, Sophia-Antipolis
 
 """
 Tokenizer for reading CPO file format
 """
```

### Comparing `docplex-2.8.125/docplex/cp/expression.py` & `docplex-2.9.141/docplex/cp/expression.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # --------------------------------------------------------------------------
 # Source file provided under Apache License, Version 2.0, January 2004,
 # http://www.apache.org/licenses/
-# (c) Copyright IBM Corp. 2015, 2016
+# (c) Copyright IBM Corp. 2015, 2016, 2017, 2018
 # --------------------------------------------------------------------------
 # Author: Olivier OUDOT, IBM Analytics, France Lab, Sophia-Antipolis
 
 """
 This module contains the basic classes representing the expressions required to
 describe a constraint programming model.
```

### Comparing `docplex-2.8.125/docplex/cp/function.py` & `docplex-2.9.141/docplex/cp/function.py`

 * *Files identical despite different names*

### Comparing `docplex-2.8.125/docplex/cp/model.py` & `docplex-2.9.141/docplex/cp/model.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # --------------------------------------------------------------------------
 # Source file provided under Apache License, Version 2.0, January 2004,
 # http://www.apache.org/licenses/
-# (c) Copyright IBM Corp. 2015, 2016
+# (c) Copyright IBM Corp. 2015, 2016, 2017, 2018
 # --------------------------------------------------------------------------
 # Author: Olivier OUDOT, IBM Analytics, France Lab, Sophia-Antipolis
 
 """
 This module contains principally the class :class:`CpoModel` that handles all the elements that compose a CPO model:
 
  * the variables of the domain (integer variables, interval variables, sequence variables and state functions),
@@ -513,14 +513,29 @@
         with the following restrictions:
 
          * Only integer and interval variables are taken into account.
            If present, all other elements are simply ignored.
          * In integer variable, if the domain is not fixed to a single value, only a single range of values is allowed.
            If the variable domain is sparse, the range domain_min..domain_max is used.
 
+        An empty starting point can be created using method :meth:`~CpoModel.create_empty_solution`, and then filled
+        using dedicated methods :meth:`~docplex.cp.solution.CpoModelSolution.add_integer_var_solution` and
+        :meth:`~docplex.cp.solution.CpoModelSolution.add_interval_var_solution`, or using indexed assignment
+        as in the following example:
+        ::
+
+            mdl = CpoModel()
+            a = integer_var(0, 3)
+            b = interval_var(length=(1, 4))
+            . . .
+            stp = mdl.create_empty_solution()
+            stp[a] = 2
+            stp[b] = (2, 3, 4)
+            mdl.set_starting_point(stp)
+
         Starting point is available for CPO solver release greater or equal to 12.7.0.
 
         Args:
             stpoint: Starting point, object of class :class:`~docplex.cp.solution.CpoModelSolution`
         """
         assert (stpoint is None) or isinstance(stpoint, CpoModelSolution), \
             "Argument 'stpoint' should be None or an object of class CpoModelSolution"
@@ -532,45 +547,63 @@
 
         Returns:
             Model starting point, None if none
         """
         return self.starting_point
 
 
+    def create_empty_solution(self):
+        """ Create an empty model solution that can be filled to be used as a starting point.
+
+        Returns:
+            New empty model solution, object of class :class:`~docplex.cp.solution.CpoModelSolution`
+        """
+        return CpoModelSolution()
+
+
     def add_kpi(self, expr, name=None):
         """ Add a Key Performance Indicator to the model.
 
         A Key Performance Indicators (KPI) is an expression whose value is considered as representative of the
         model solution and its quality.
 
-        The KPI expression can be:
+        For example, in a scheduling problem one may wish to minimize the makespan
+        (date at which all tasks are completed), but other values may be of interest, like the average job
+        completion time, or the maximum number of tasks executing in parallel over the horizon.
+        One can identify such expressions in the model by marking them as KPIs.
+
+        For CPO solver version lower than 12.9, KPI expressions are limited to:
 
          * an integer variable,
          * a Python lambda expression that computes the value of the KPI from the solve result given as parameter.
 
         Example of lambda expression used as KPI:
         ::
 
             mdl = CpoModel()
             a = integer_var(0, 3)
             b = integer_var(0, 3)
             mdl.add(a < b)
             mdl.add_kpi(lambda res: (res[a] + res[b]) / 2, "Average")
 
-        If the model is solved in a cloud context, these KPIs are associated to the objective value in the
+        For CPO solver version greater or equal to 12.9, KPI expressions can be any model expression.
+        KPI values are automatically displayed in the log, can be queried after the solve or for each solution,
+        and are exported to a CPO file when the model is exported.
+
+        If the model is solved in a cloud context, the KPIs are associated to the objective value in the
         solve details that are sent periodically to the client.
 
         Args:
             expr:             Model variable to be used as KPI(s).
             name (optional):  Name used to publish this KPI.
                               If absent the expression name is used.
                               If the expression has no name, an exception is raised.
         """
         ver = self.get_usable_format_version()
-        iskexpr = ver is not None and compare_natural(ver, '12.8.9') > 0
+        iskexpr = ver is not None and compare_natural(ver, '12.9') >= 0
 
         if isinstance(expr, CpoExpr):
             if iskexpr:
                 assert expr.type != Type_Constraint, "KPI expression can not be a top-level constraint"
             else:
                 assert expr.type == Type_IntVar, "KPI expression can only be an integer variable."
         else:
@@ -1431,15 +1464,15 @@
                 estack.extend(e.children)
         return None
 
 
     def _get_calling_location(self):
         """ Determine the calling location, outside docplex.cp
         Returns:
-             Couplt (file, line), or None if impossible to determine
+             Couple (file, line), or None if impossible to determine
         """
         frm = inspect.currentframe()
         # Skip at least 2 frames (first called method + this one)
         if frm is None:
             return None
         frm = frm.f_back
         if frm is None:
```

### Comparing `docplex-2.8.125/docplex/cp/modeler.py` & `docplex-2.9.141/docplex/cp/modeler.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # --------------------------------------------------------------------------
 # Source file provided under Apache License, Version 2.0, January 2004,
 # http://www.apache.org/licenses/
-# (c) Copyright IBM Corp. 2015, 2016
+# (c) Copyright IBM Corp. 2015, 2016, 2017, 2018
 # --------------------------------------------------------------------------
 # Author: Olivier OUDOT, IBM Analytics, France Lab, Sophia-Antipolis
 
 """
 This module contains the functions that allows to construct all operations
 and constraints that can be used in a *CP Optimizer* model.
 
@@ -1481,19 +1481,22 @@
         values: An array of integer expressions, or a set of tuples,
                 that specifies the combinations of forbidden values of the expressions exprs.
     Returns:
         A boolean expression
     """
     exprs = build_cpo_expr(exprs)
     if exprs.is_kind_of(Type_IntExpr):
+        # Expr is a single integer
         return CpoFunctionCall(Oper_allowed_assignments, Type_BoolExpr, (exprs, _convert_arg(values, values, Type_IntArray)))
 
     # 'expr' is an array of expressions, and 'values' a tupleset
     assert exprs.is_kind_of(Type_IntExprArray), "Argument 'exprs' should be an array of integer or an array of integer expressions"
-    return CpoFunctionCall(Oper_allowed_assignments, Type_BoolExpr, (exprs, build_cpo_tupleset(values)))
+    tset = build_cpo_tupleset(values)
+    assert len(exprs.children) == len(tset.value[0]), "Arity of tupleset should match the number of expressions"
+    return CpoFunctionCall(Oper_allowed_assignments, Type_BoolExpr, (exprs, tset))
 
 
 def forbidden_assignments(exprs, values):
     """ Explicitly defines forbidden assignments for one or more integer expressions.
 
     This boolean expression (which is interpreted as a constraint outside of an expression)
     determines whether the assignment to a single expression or to an array of expressions
```

### Comparing `docplex-2.8.125/docplex/cp/parameters.py` & `docplex-2.9.141/docplex/cp/parameters.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # --------------------------------------------------------------------------
 # Source file provided under Apache License, Version 2.0, January 2004,
 # http://www.apache.org/licenses/
-# (c) Copyright IBM Corp. 2015, 2016
+# (c) Copyright IBM Corp. 2015, 2016, 2017, 2018
 # --------------------------------------------------------------------------
 # Author: Olivier OUDOT, IBM Analytics, France Lab, Sophia-Antipolis
 
 """
 This module handles the parameters that can be assigned to CP Optimizer to configure
 the solving of a model.
 
@@ -54,16 +54,18 @@
    The value is an integer in [0..3]. Default value is 2.
  * :attr:`~CpoParameters.PrintModelDetailsInMessages`: Controls printing of additional information on error and warning messages.
    The value is a symbol in ['On', 'Off']. Default value is 'On'.
  * :attr:`~CpoParameters.ModelAnonymizer`: Controls anonymization of a model dumped via dumpModel.
    The value is a symbol in ['On', 'Off']. Default value is 'Off'.
  * :attr:`~CpoParameters.UseFileLocations`: Controls whether location information (file, line) is added to the model.
    The value is a symbol in ['On', 'Off']. Default value is 'On'.
- * :attr:`~CpoParameters.LogSearchTags`: Controls the log activation. Possible values are 'On' or 'Off'.
+ * :attr:`~CpoParameters.LogSearchTags`: Controls the log activation.
    The value is a symbol in ['On', 'Off']. Default value is 'Off'.
+ * :attr:`~CpoParameters.KPIDisplay`: Controls the display of the KPI values in the log.
+   The value is a symbol in ['SingleLine', 'MultipleLines']. Default value is 'SingleLine'.
    
 **Presolve**
 
  * :attr:`~CpoParameters.Presolve`: Controls the presolve of the model to produce more compact formulations and to achieve more domain reduction.
 
 **Optimality tolerances**
 
@@ -73,15 +75,15 @@
    The value is a non-negative float. Default value is 0.0001.
 
 **Search control**
 
  * :attr:`~CpoParameters.Workers`: Number of workers to run in parallel to solve the model.
    The value is a positive integer. Default value is Auto.
  * :attr:`~CpoParameters.SearchType`: Type of search that is applied when solving a problem.
-   The value is a symbol in ['DepthFirst', 'Restart', 'MultiPoint', 'Auto']. Default value is 'Auto'.
+   The value is a symbol in ['DepthFirst', 'Restart', 'MultiPoint', 'IterativeDiving', 'Auto']. Default value is 'Auto'.
  * :attr:`~CpoParameters.RandomSeed`: Seed of the random generator used by search strategies.
    The value is a non-negative integer. Default value is 0.
  * :attr:`~CpoParameters.RestartFailLimit`: Controls the number of failures that must occur before restarting search.
    The value is an integer greater than 0. Default value is 100.
  * :attr:`~CpoParameters.RestartGrowthFactor`: Controls the increase of the number of failures between restarts.
    The value is a float greater or equal to 1. Default value is 1.15.
  * :attr:`~CpoParameters.DynamicProbing`: Controls probing carried out during search.
@@ -168,46 +170,51 @@
      "CumulFunctionInferenceLevel", "DefaultInferenceLevel", "DistributeInferenceLevel", "DynamicProbing",
      "DynamicProbingStrength", "ElementInferenceLevel", "FailLimit", "FailureDirectedSearch",
      "FailureDirectedSearchEmphasis", "FailureDirectedSearchMaxMemory", "IntervalSequenceInferenceLevel", "LogPeriod",
      "LogSearchTags", "LogVerbosity", "ModelAnonymizer", "MultiPointNumberOfSearchPoints", "NoOverlapInferenceLevel",
      "OptimalityTolerance", "PrecedenceInferenceLevel", "Presolve", "PrintModelDetailsInMessages", "RandomSeed",
      "RelativeOptimalityTolerance", "RestartFailLimit", "RestartGrowthFactor", "SearchType", "SequenceInferenceLevel",
      "SolutionLimit", "StateFunctionInferenceLevel", "TemporalRelaxation", "TimeLimit", "TimeMode", "UseFileLocations",
-     "WarningLevel", "Workers",}
+     "WarningLevel", "Workers", "KPIDisplay"}
 
 # Set of all private but accepted parameter names
 PRIVATE_PARAMETER_NAMES = {"ObjectiveLimit",}
 
 # Set of all authorized parameter names
 ALL_PARAMETER_NAMES = PUBLIC_PARAMETER_NAMES | PRIVATE_PARAMETER_NAMES
 
 # Symbolic parameter values
-VALUE_AUTO         = 'Auto'
-VALUE_OFF          = 'Off'
-VALUE_ON           = 'On'
-VALUE_DEFAULT      = 'Default'
-VALUE_LOW          = 'Low'
-VALUE_BASIC        = 'Basic'
-VALUE_MEDIUM       = 'Medium'
-VALUE_EXTENDED     = 'Extended'
-VALUE_QUIET        = 'Quiet'
-VALUE_TERSE        = 'Terse'
-VALUE_NORMAL       = 'Normal'
-VALUE_VERBOSE      = 'Verbose'
-VALUE_DEPTH_FIRST  = 'DepthFirst'
-VALUE_RESTART      = 'Restart'
-VALUE_MULTI_POINT  = 'MultiPoint'
-VALUE_DIVERSE      = 'Diverse'
-VALUE_CPU_TIME     = 'CPUTime'
-VALUE_ELAPSED_TIME = 'ElapsedTime'
+VALUE_AUTO             = 'Auto'
+VALUE_OFF              = 'Off'
+VALUE_ON               = 'On'
+VALUE_DEFAULT          = 'Default'
+VALUE_LOW              = 'Low'
+VALUE_BASIC            = 'Basic'
+VALUE_MEDIUM           = 'Medium'
+VALUE_EXTENDED         = 'Extended'
+VALUE_QUIET            = 'Quiet'
+VALUE_TERSE            = 'Terse'
+VALUE_NORMAL           = 'Normal'
+VALUE_VERBOSE          = 'Verbose'
+VALUE_DEPTH_FIRST      = 'DepthFirst'
+VALUE_RESTART          = 'Restart'
+VALUE_MULTI_POINT      = 'MultiPoint'
+VALUE_ITERATIVE_DIVING = 'IterativeDiving'
+VALUE_DIVERSE          = 'Diverse'
+VALUE_CPU_TIME         = 'CPUTime'
+VALUE_ELAPSED_TIME     = 'ElapsedTime'
+VALUE_SINGLE_LINE      = 'SingleLine'
+VALUE_MULTIPLE_LINES   = 'MultipleLines'
 
 # Authorized sets of values
 _INFERENCE_LEVELS = (VALUE_DEFAULT, VALUE_LOW, VALUE_BASIC, VALUE_MEDIUM, VALUE_EXTENDED)
 _ON_OFF_AUTO = (VALUE_ON, VALUE_OFF, VALUE_AUTO)
 _ON_OFF = (VALUE_ON, VALUE_OFF)
+_KPI_DISPLAY = (VALUE_SINGLE_LINE, VALUE_MULTIPLE_LINES)
+_SEARCH_TYPES = (VALUE_DEPTH_FIRST, VALUE_RESTART, VALUE_MULTI_POINT, VALUE_ITERATIVE_DIVING, VALUE_AUTO)
 
 
 ###############################################################################
 ## Public classes
 ###############################################################################
 
 class CpoParameters(Context):
@@ -682,14 +689,28 @@
 
     def set_LogSearchTags(self, val):
         self._set_value_enum('LogSearchTags', val, _ON_OFF)
 
     LogSearchTags = property(get_LogSearchTags, set_LogSearchTags)
 
 
+    def get_KPIDisplay(self):
+        """
+        This parameter determines how KPIs are displayed in the log during the search.
+
+        The value is a symbol in ['SingleLine', 'MultipleLines']. Default value is 'SingleLine'.
+        """
+        return self.get_attribute('KPIDisplay')
+
+    def set_KPIDisplay(self, val):
+        self._set_value_enum('KPIDisplay', val, _KPI_DISPLAY)
+
+    KPIDisplay = property(get_KPIDisplay, set_KPIDisplay)
+
+
     def get_LogVerbosity(self):
         """
         This parameter determines the verbosity of the search log. The possible values are Quiet, Terse,
         Normal, and Verbose. Mode Quiet does not display any information, the other modes display
         progressively more information. The default value is Normal. The CP Optimizer search log is meant
         for visual inspection only, not for mechanized parsing. In particular, the log may change from
         version to version of CP Optimizer in order to improve the quality of information displayed in the
@@ -894,32 +915,37 @@
         self._set_value_float('RestartGrowthFactor', val, min=1)
 
     RestartGrowthFactor = property(get_RestartGrowthFactor, set_RestartGrowthFactor)
 
 
     def get_SearchType(self):
         """
-        This parameter determines the type of search that is applied when solving a problem. When set to
-        DepthFirst, a regular depth-first search is applied. When set to Restart, a depth-first search that
-        restarts from time to time is applied. When set to MultiPoint, a method that combines a set of -
-        possibly partial - solutions is applied. When set to Auto in sequential mode, this value chooses the
-        appropriate search method to be used. In general Auto will be the Restart search. The default value
-        is Auto. In parallel mode (i.e, when the number of workers is greater than one - see the Workers
+        This parameter determines the type of search that is applied when solving a problem.
+
+         * When set to *DepthFirst*, a regular depth-first search is applied.
+         * When set to *Restart*, a depth-first search that restarts from time to time is applied.
+         * When set to *IterativeDiving* on scheduling problems (ones with at least one interval variable),
+           a more aggressive diving technique is applied in order to find solutions to large problems more quickly.
+         * When set to *MultiPoint*, a method that combines a set of - possibly partial - solutions is applied.
+         * When set to *Auto* in sequential mode, this value chooses the appropriate search method to be used.
+           In general Auto will be the Restart search. The default value is Auto.
+
+        In parallel mode (i.e, when the number of workers is greater than one - see the Workers
         parameter), the different searches described above are spread over the workers. When the value of
         SearchType is Auto, then the decision of choosing the search type for a worker is automatically
         made; otherwise, all workers execute the same type of search. Note that in the latter case, the
         workers will not do the same exploration due to some randomness introduced to break ties in decision
         making.
 
-        The value is a symbol in ['DepthFirst', 'Restart', 'MultiPoint', 'Auto']. Default value is 'Auto'.
+        The value is a symbol in ['DepthFirst', 'Restart', 'MultiPoint', 'IterativeDiving', 'Auto']. Default value is 'Auto'.
         """
         return self.get_attribute('SearchType')
 
     def set_SearchType(self, val):
-        self._set_value_enum('SearchType', val, (VALUE_DEPTH_FIRST, VALUE_RESTART, VALUE_MULTI_POINT, VALUE_AUTO))
+        self._set_value_enum('SearchType', val, _SEARCH_TYPES)
 
     SearchType = property(get_SearchType, set_SearchType)
 
 
     def get_SequenceInferenceLevel(self):
         """
         This parameter specifies the inference level for every constraint Sequence extracted to the invoked
```

### Comparing `docplex-2.8.125/docplex/cp/solution.py` & `docplex-2.9.141/docplex/cp/solution.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # --------------------------------------------------------------------------
 # Source file provided under Apache License, Version 2.0, January 2004,
 # http://www.apache.org/licenses/
-# (c) Copyright IBM Corp. 2015, 2016
+# (c) Copyright IBM Corp. 2015, 2016, 2017, 2018
 # --------------------------------------------------------------------------
 # Author: Olivier OUDOT, IBM Analytics, France Lab, Sophia-Antipolis
 
 """
 This module contains the different elements that represent a solution resulting
 from the solve of a model.
 
@@ -232,68 +232,74 @@
     For example, following are valid domains for an integer variable:
      * 7 (complete solution)
      * (1, 2, 4, 9)
      * (2, 3, (5, 7), 9, (11, 13))
     """
     __slots__ = ('value',  # Variable value / domain
                 )
-    
+
     def __init__(self, expr, value):
         """ Constructor:
 
         Args:
             expr:  Variable expression, object of class :class:`~docplex.cp.expression.CpoIntVar`.
             value: Variable value, or domain if not completely instantiated
         """
         assert isinstance(expr, CpoIntVar), "Expression 'expr' should be a CpoIntVar expression"
         super(CpoIntVarSolution, self).__init__(expr)
         self.value = _check_arg_domain(value, 'value')
 
+
     def get_value(self):
         """ Gets the value of the variable.
 
         Returns:
             Variable value (integer), or domain (list of integers or intervals)
         """
         return self.value
 
+
     def get_domain_min(self):
         """ Gets the domain lower bound.
 
         Returns:
             Domain lower bound.
         """
         return _domain_min(self.value)
 
+
     def get_domain_max(self):
         """ Gets the domain upper bound.
 
         Returns:
             Domain upper bound.
         """
         return _domain_max(self.value)
 
+
     def domain_iterator(self):
         """ Iterator on the individual values of an integer variable domain.
 
         Returns:
             Value iterator on the domain of this variable.
         """
         return _domain_iterator(self.value)
 
+
     def domain_contains(self, value):
         """ Check whether a given value is in the domain of the variable
 
         Args:
             val: Value to check
         Returns:
             True if the value is in the domain, False otherwise
         """
         return _domain_contains(self.value, value)
 
+
     def __str__(self):
         """ Convert this expression into a string """
         return str(self.get_name()) + ": " + str(self.get_value())
         
 
 class CpoIntervalVarSolution(CpoVarSolution):
     """ This class represents a solution to an interval variable.
@@ -304,31 +310,33 @@
     __slots__ = ('start',    # Interval start
                  'end',      # Interval end
                  'size',     # Interval size
                  'length',   # Interval length
                  'presence', # Presence indicator
                 )
     
-    def __init__(self, expr, presence=None, start=None, end=None, size=None):
+    def __init__(self, expr, presence=None, start=None, end=None, size=None, length=None):
         """ Constructor:
 
         Args:
             expr:     Variable expression, object of class :class:`~docplex.cp.expression.CpoIntervalVar`.
             presence: Presence indicator (True for present, False for absent, None for undetermined). Default is None.
             start:    Value of start, or tuple representing the start range. Default is None.
             end:      Value of end, or tuple representing the end range. Default is None.
             size:     Value of size, or tuple representing the size range. Default is None.
+            length:   Value of the length, or tuple representing the length range. Default is None.
+                      Not to be used if other values are integers.
         """
         assert isinstance(expr, CpoIntervalVar), "Expression 'expr' should be a CpoIntervalVar expression"
         super(CpoIntervalVarSolution, self).__init__(expr)
         self.presence = presence
         self.start    = start
         self.end      = end
         self.size     = size
-        self.length   = None
+        self.length   = length
 
 
     def is_present(self):
         """ Check if the interval is present.
 
         Returns:
             True if interval is present, False otherwise.
@@ -415,17 +423,17 @@
         individual value can be an integer or an interval expressed as a tuple.
 
         Returns:
             Interval variable value as a tuple.
         """
         if self.is_present():
             if self.length is None:
-                return self.start, self.end, self.size
+                return (self.start, self.end, self.size, )
             else:
-                return self.start, self.end, self.size, self.length
+                return (self.start, self.end, self.size, self.length, )
         return ()
 
 
     def __str__(self):
         """ Convert this expression into a string """
         res = [str(self.get_name()), ': ']
         if self.is_absent():
@@ -656,28 +664,30 @@
         Args:
             var:   Variable expression, object of class :class:`~docplex.cp.expression.CpoIntVar`.
             value: Variable value, or domain if not completely instantiated
         """
         self.add_var_solution(CpoIntVarSolution(var, value))
 
 
-    def add_interval_var_solution(self, var, presence=None, start=None, end=None, size=None):
+    def add_interval_var_solution(self, var, presence=None, start=None, end=None, size=None, length=None):
         """ Add a new interval variable solution.
 
         The solution can be complete if all attribute values are integers, or partial if at least one
         of them is an interval expressed as a tuple.
 
         Args:
             var:      Variable expression, object of class :class:`~docplex.cp.expression.CpoIntervalVar`.
             presence: Presence indicator (true for present, false for absent, None for undetermined). Default is None.
             start:    Value of start, or tuple representing the start range
             end:      Value of end, or tuple representing the end range
             size:     Value of size, or tuple representing the size range
+            length:   Value of the length, or tuple representing the length range. Default is None.
+                      Not to be used if other values are integers.
         """
-        self.add_var_solution(CpoIntervalVarSolution(var, presence, start, end, size))
+        self.add_var_solution(CpoIntervalVarSolution(var, presence, start, end, size, length))
 
 
     def get_var_solution(self, expr):
         """ Gets a variable solution from this model solution.
 
         Args:
             expr: Variable expression or variable name if any
@@ -709,24 +719,65 @@
 
          * :meth:`CpoIntVarSolution.get_value`
          * :meth:`CpoIntervalVarSolution.get_value`
          * :meth:`CpoSequenceVarSolution.get_value`
          * :meth:`CpoStateFunctionSolution.get_value`
 
         Args:
-            expr: Variable expression, variable name  or KPI name.
+            expr: Variable expression, variable name or KPI name.
         Returns:
             Variable value, None if variable is not found.
         """
         var = self.get_var_solution(expr)
         if var is not None:
             return var.get_value()
         return self.get_kpi_value(expr)
 
 
+    def set_value(self, var, value):
+        """ Sets the value of a variable.
+
+        This method allows to set an integer variable or an interval variable with the short representation
+        used to represent it, as returned by :meth:`CpoIntVarSolution.get_value`
+        or :meth:`CpoIntervalVarSolution.get_value`.
+
+        For an integer variable, value can be:
+
+         * If the variable is fully instantiated, a single integer.
+         * If the variable is partially instantiated, a domain expressed as a list of integers or intervals.
+
+
+        For an interval variable, value can be:
+
+         * If the variable is absent, an empty tuple.
+         * If the variable is fully instantiated, a tuple of 3 integers (start, end, size).
+         * If the variable is partially instantiated, a tuple (start, end, size, length) where each
+           individual value can be an integer or an interval expressed as a tuple.
+
+        Args:
+            var: Model variable
+            value: short representation of the variable value
+        """
+        if isinstance(var, CpoIntVar):
+            self.add_integer_var_solution(var, value)
+        elif isinstance(var, CpoIntervalVar):
+            if not value:
+                self.add_interval_var_solution(var, presence=False)
+            elif len(value) == 3:
+                start, end, size = value
+                self.add_interval_var_solution(var, presence=True, start=start, end=end, size=size)
+            elif len(value) == 4:
+                start, end, size, length = value
+                self.add_interval_var_solution(var, presence=True, start=start, end=end, size=size, length=length)
+            else:
+                raise AssertionError("Invalid value format for an interval variable")
+        else:
+            raise AssertionError("Variable that can be set directly are restricted to integer and interval variables")
+
+
     def add_kpi_value(self, name, value):
         """ Add a KPI value to this solution
 
         Args:
             name:    Name of the KPI
             value:   Model variable representing this KPI
         """
@@ -839,37 +890,56 @@
         funs = jsol.get('stateFunctions', ())
         for fname in funs:
             fun = _get_expr_from_map(expr_map, fname)
             lpts = [( _get_num_value(v['start']), _get_num_value(v['end']), _get_num_value(v['value'])) for v in funs[fname]]
             self.add_var_solution(CpoStateFunctionSolution(fun, lpts))
 
         # Set kpis
-        kpi_values = jsol.get('KPIs', ())
+        kpi_values = jsol.get('KPIs', {})
         kpis = model.get_kpis()
-        for name, (expr, loc) in kpis.items():
-            if isinstance(expr, types.FunctionType):
-                value = expr(self)
-            elif name in kpi_values:
-                value = kpi_values[name]
-            else:
-                value = self.get_value(expr)
-            self.add_kpi_value(name, value)
+        try:
+            for name, (expr, loc) in kpis.items():
+                if isinstance(expr, types.FunctionType):
+                    # KPI is a lambda expression
+                    value = expr(self)
+                elif name in kpi_values:
+                    # KPI is a solver KPI
+                    value = kpi_values[name]
+                else:
+                    # KPI is a model variable
+                    value = self.get_value(expr)
+                self.add_kpi_value(name, value)
+        except:
+            # Solution has no values
+            pass
 
 
     def __getitem__(self, expr):
         """ Overloading of [] to get a variable solution from this model solution
 
         Args:
             expr: Variable expression or variable name if any
         Returns:
             Variable solution (class CpoVarSolution)
         """
         return self.get_value(expr)
 
 
+    def __setitem__(self, var, value):
+        """ Overloading of [] to set a variable solution in this model solution
+
+        Args:
+            var: Variable expression
+            value:  Variable value
+        Returns:
+            Variable solution (class CpoVarSolution)
+        """
+        return self.set_value(var, value)
+
+
     def __contains__(self, expr):
         """ Overloading of 'in' to check that a variable solution is in this model solution
 
         Args:
             expr: Variable expression or variable name if any
         Returns:
             True if this model solution contains a solution for this variable.
```

### Comparing `docplex-2.8.125/docplex/cp/tokenizer.py` & `docplex-2.9.141/docplex/cp/tokenizer.py`

 * *Files identical despite different names*

### Comparing `docplex-2.8.125/docplex/cp/utils.py` & `docplex-2.9.141/docplex/cp/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # --------------------------------------------------------------------------
 # Source file provided under Apache License, Version 2.0, January 2004,
 # http://www.apache.org/licenses/
-# (c) Copyright IBM Corp. 2015, 2016
+# (c) Copyright IBM Corp. 2015, 2016, 2017, 2018
 # --------------------------------------------------------------------------
 # Author: Olivier OUDOT, IBM Analytics, France Lab, Sophia-Antipolis
 
 """
 Miscellaneous utility functions. Some of theme are here to prevent possible
 port problems between the different versions of Python.
 """
@@ -16,14 +16,15 @@
 import sys
 import threading
 import io
 import inspect
 from collections import deque, Iterable
 import json
 import platform
+import importlib
 
 try:
     from StringIO import StringIO
 except ImportError:
     from io import StringIO
 
 
@@ -1204,15 +1205,32 @@
 
     Args:
         mod:  Module to parse
         excepted:  List of function names to not include. Default is none.
     Returns:
         List of public functions declared in this module
     """
-    return [t[1] for t in inspect.getmembers(mod, inspect.isfunction) if not t[0].startswith('_') and inspect.getmodule(t[1]) == mod and not t[0] in excepted]
+    return [t[1] for t in inspect.getmembers(mod, inspect.isfunction) if not t[0].startswith('_')
+            and inspect.getmodule(t[1]) == mod
+            and not t[0] in excepted]
+
+
+def get_module_element_from_path(opath):
+    """ Retrieve an element from a python module using its path <package>.<module>.<object>
+
+    This can be for example a global function or a class.
+
+    Args:
+        opath:  Object path
+    Returns:
+        Module object
+    """
+    module, oname = opath.rsplit('.', 1)
+    mod = importlib.import_module(module)
+    return getattr(mod, oname)
 
 
 #-----------------------------------------------------------------------------
 # Checking of object types
 #-----------------------------------------------------------------------------
 
 # Determine list of types representing the different python scalar types
@@ -1668,15 +1686,14 @@
     """
     # Check null strings
     if s1 is None:
         return 0 if s2 is None else -1
     if s2 is None:
         return 1
 
-
     # Skip all identical characters
     len1 = len(s1)
     len2 = len(s2)
     i = 0
     while i < len1 and i < len2 and s1[i] == s2[i]:
         i += 1
```

### Comparing `docplex-2.8.125/docplex/cp/utils_visu.py` & `docplex-2.9.141/docplex/cp/utils_visu.py`

 * *Files identical despite different names*

### Comparing `docplex-2.8.125/docplex/mp/callbacks/cb_mixin.py` & `docplex-2.9.141/docplex/mp/callbacks/cb_mixin.py`

 * *Files identical despite different names*

### Comparing `docplex-2.8.125/docplex/mp/internal/json_conflict_handler.py` & `docplex-2.9.141/docplex/mp/internal/json_conflict_handler.py`

 * *Files identical despite different names*

### Comparing `docplex-2.8.125/docplex/mp/internal/json_infeasibility_handler.py` & `docplex-2.9.141/docplex/mp/internal/json_infeasibility_handler.py`

 * *Files identical despite different names*

### Comparing `docplex-2.8.125/docplex/mp/internal/json_solution_handler.py` & `docplex-2.9.141/docplex/mp/internal/json_solution_handler.py`

 * *Files identical despite different names*

### Comparing `docplex-2.8.125/docplex/mp/params/cplex_params.py` & `docplex-2.9.141/docplex/mp/params/cplex_params.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 # --------------------------------------------------------------------------
 # Source file provided under Apache License, Version 2.0, January 2004,
 # http://www.apache.org/licenses/
-# (c) Copyright IBM Corp. 2015, 2016
+# (c) Copyright IBM Corp. 2015, 2018
 # --------------------------------------------------------------------------
 
 # gendoc: ignore
 from docplex.mp.params.parameter_hierarchy_12620 import make_root_params_12620
 from docplex.mp.params.parameter_hierarchy_12630 import make_root_params_12630
 from docplex.mp.params.parameter_hierarchy_12700 import make_root_params_12700
 from docplex.mp.params.parameter_hierarchy_12710 import make_root_params_12710
 from docplex.mp.params.parameter_hierarchy_12800 import make_root_params_12800
 from docplex.mp.params.parameter_hierarchy_12900 import make_root_params_12900
 
 def _make_default_parameters():
-    # when cloudcplex switches to 12.7.1 use this.
     return make_root_params_12800()
 
 
 def get_params_from_cplex_version(cpx_version):
     # INTERNAL
     # returns a parameter tree depending on the cplex version, if any.
     # if none is found, returns a default version.
```

### Comparing `docplex-2.8.125/docplex/mp/params/parameter_hierarchy_12620.py` & `docplex-2.9.141/docplex/mp/params/parameter_hierarchy_12620.py`

 * *Files identical despite different names*

### Comparing `docplex-2.8.125/docplex/mp/params/parameter_hierarchy_12630.py` & `docplex-2.9.141/docplex/mp/params/parameter_hierarchy_12630.py`

 * *Files identical despite different names*

### Comparing `docplex-2.8.125/docplex/mp/params/parameter_hierarchy_12700.py` & `docplex-2.9.141/docplex/mp/params/parameter_hierarchy_12700.py`

 * *Files 0% similar despite different names*

```diff
@@ -441,9 +441,12 @@
                 read=_group_read_make,
                 sifting=_group_sifting_make,
                 simplex=_group_simplex_make,
                 tune=_group_tune_make)
 
 
 def make_root_params_12700():
-    return RootParameterGroup.make("parameters", _group_cpxparam_params, _group_cpxparam_subgroups, "12.7.0.0")
+    proot = RootParameterGroup.make("parameters", _group_cpxparam_params, _group_cpxparam_subgroups, "12.7.0.0")
+    # -- set synchronous params
+    proot.read.datacheck._synchronous = True
+    return proot
 #  --- end of generated code ---
```

### Comparing `docplex-2.8.125/docplex/mp/params/parameter_hierarchy_12710.py` & `docplex-2.9.141/docplex/mp/params/parameter_hierarchy_12710.py`

 * *Files 0% similar despite different names*

```diff
@@ -442,9 +442,13 @@
                 read=_group_read_make,
                 sifting=_group_sifting_make,
                 simplex=_group_simplex_make,
                 tune=_group_tune_make)
 
 
 def make_root_params_12710():
-    return RootParameterGroup.make("parameters", _group_cpxparam_params, _group_cpxparam_subgroups, "12.7.1.0")
+    proot = RootParameterGroup.make("parameters", _group_cpxparam_params, _group_cpxparam_subgroups, "12.7.1.0")
+    # -- set synchronous params
+    proot.read.datacheck._synchronous = True
+    return proot
+
 #  --- end of generated code ---
```

### Comparing `docplex-2.8.125/docplex/mp/params/parameter_hierarchy_12800.py` & `docplex-2.9.141/docplex/mp/params/parameter_hierarchy_12800.py`

 * *Files 0% similar despite different names*

```diff
@@ -487,9 +487,12 @@
                 read=_group_read_make,
                 sifting=_group_sifting_make,
                 simplex=_group_simplex_make,
                 tune=_group_tune_make)
 
 
 def make_root_params_12800():
-    return RootParameterGroup.make("parameters", _group_cpxparam_params, _group_cpxparam_subgroups, "12.8.0.0")
+    proot = RootParameterGroup.make("parameters", _group_cpxparam_params, _group_cpxparam_subgroups, "12.8.0.0")
+    # -- set synchronous params
+    proot.read.datacheck._synchronous = True
+    return proot
 #  --- end of generated code ---
```

### Comparing `docplex-2.8.125/docplex/mp/params/parameter_hierarchy_12900.py` & `docplex-2.9.141/docplex/mp/params/parameter_hierarchy_12900.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from docplex.mp.params.parameters import *
 
 
 
 # generating code for group: Barrier_Limits
 def _group_barrier_limits_params(pgroup):
     return dict(corrections=IntParameter(pgroup, "corrections", "CPX_PARAM_BARMAXCOR", 3013, "maximum correction limit", default_value=-1, min_value=-1.0, max_value=9223372036800000000),
-                growth=NumParameter(pgroup, "growth", "CPX_PARAM_BARGROWTH", 3003, "factor used to determine unbounded optimal face", default_value=1000000000000.0, min_value=1.0, max_value=1e+75),
+                growth=NumParameter(pgroup, "growth", "CPX_PARAM_BARGROWTH", 3003, "factor used to determine unbounded optimal face", default_value=1e+12, min_value=1.0, max_value=1e+75),
                 iteration=IntParameter(pgroup, "iteration", "CPX_PARAM_BARITLIM", 3012, "barrier iteration limit", default_value=9223372036800000000, min_value=0.0, max_value=9223372036800000000),
                 objrange=NumParameter(pgroup, "objrange", "CPX_PARAM_BAROBJRNG", 3004, "barrier objective range (above and below zero)", default_value=1e+20, min_value=0.0, max_value=1e+75)
                 )
 
 
 def _group_barrier_limits_make(pgroup):
     return ParameterGroup.make("limits", _group_barrier_limits_params, None, pgroup)
@@ -203,27 +203,14 @@
                 )
 
 
 def _group_mip_pool_make(pgroup):
     return ParameterGroup.make("pool", _group_mip_pool_params, None, pgroup)
 
 
-# generating code for group: MIP_SubMIP
-def _group_mip_submip_params(pgroup):
-    return dict(startalg=IntParameter(pgroup, "startalg", "CPX_PARAM_SUBMIPSTARTALG", 2205, "algorithm to solve initial relaxation for sub-MIPs", default_value=0, min_value=0.0, max_value=5.0),
-                subalg=IntParameter(pgroup, "subalg", "CPX_PARAM_SUBMIPSUBALG", 2206, "algorithm to solve subproblems for sub-MIPs", default_value=0, min_value=0.0, max_value=5.0),
-                nodelimit=IntParameter(pgroup, "nodelimit", "CPX_PARAM_SUBMIPNODELIMIT", 2212, "sub-MIP node limit", default_value=500, min_value=1.0, max_value=9223372036800000000),
-                scale=IntParameter(pgroup, "scale", "CPX_PARAM_SUBMIPSCAIND", 2207, "type of scaling used for sub-MIPs", default_value=0, min_value=-1.0, max_value=1.0)
-                )
-
-
-def _group_mip_submip_make(pgroup):
-    return ParameterGroup.make("submip", _group_mip_submip_params, None, pgroup)
-
-
 # generating code for group: MIP_Strategy
 def _group_mip_strategy_params(pgroup):
     return dict(backtrack=NumParameter(pgroup, "backtrack", "CPX_PARAM_BTTOL", 2002, "factor for backtracking, lower values give more", default_value=0.9999, min_value=0.0, max_value=1.0),
                 bbinterval=IntParameter(pgroup, "bbinterval", "CPX_PARAM_BBINTERVAL", 2039, "interval to select best bound node", default_value=7, min_value=0.0, max_value=9223372036800000000),
                 branch=IntParameter(pgroup, "branch", "CPX_PARAM_BRDIR", 2001, "direction of first branch", default_value=0, min_value=-1.0, max_value=1.0),
                 dive=IntParameter(pgroup, "dive", "CPX_PARAM_DIVETYPE", 2060, "dive strategy", default_value=0, min_value=0.0, max_value=3.0),
                 file=IntParameter(pgroup, "file", "CPX_PARAM_NODEFILEIND", 2016, "file for node storage when tree memory limit is reached", default_value=1, min_value=0.0, max_value=4),
@@ -244,14 +231,27 @@
                 )
 
 
 def _group_mip_strategy_make(pgroup):
     return ParameterGroup.make("strategy", _group_mip_strategy_params, None, pgroup)
 
 
+# generating code for group: MIP_SubMIP
+def _group_mip_submip_params(pgroup):
+    return dict(startalg=IntParameter(pgroup, "startalg", "CPX_PARAM_SUBMIPSTARTALG", 2205, "algorithm to solve initial relaxation for sub-MIPs", default_value=0, min_value=0.0, max_value=5.0),
+                subalg=IntParameter(pgroup, "subalg", "CPX_PARAM_SUBMIPSUBALG", 2206, "algorithm to solve subproblems for sub-MIPs", default_value=0, min_value=0.0, max_value=5.0),
+                nodelimit=IntParameter(pgroup, "nodelimit", "CPX_PARAM_SUBMIPNODELIMIT", 2212, "sub-MIP node limit", default_value=500, min_value=1.0, max_value=9223372036800000000),
+                scale=IntParameter(pgroup, "scale", "CPX_PARAM_SUBMIPSCAIND", 2207, "type of scaling used for sub-MIPs", default_value=0, min_value=-1.0, max_value=1.0)
+                )
+
+
+def _group_mip_submip_make(pgroup):
+    return ParameterGroup.make("submip", _group_mip_submip_params, None, pgroup)
+
+
 # generating code for group: MIP_Tolerances
 def _group_mip_tolerances_params(pgroup):
     return dict(absmipgap=NumParameter(pgroup, "absmipgap", "CPX_PARAM_EPAGAP", 2008, "absolute mixed integer optimality gap tolerance", default_value=1e-06, min_value=0.0),
                 integrality=NumParameter(pgroup, "integrality", "CPX_PARAM_EPINT", 2010, "integrality tolerance", default_value=1e-05, min_value=0.0, max_value=0.5),
                 lowercutoff=NumParameter(pgroup, "lowercutoff", "CPX_PARAM_CUTLO", 2006, "lower objective cutoff", default_value=-1e+75),
                 mipgap=NumParameter(pgroup, "mipgap", "CPX_PARAM_EPGAP", 2009, "mixed integer optimality gap tolerance", default_value=0.0001, min_value=0.0, max_value=1.0),
                 objdifference=NumParameter(pgroup, "objdifference", "CPX_PARAM_OBJDIF", 2019, "absolute amount successive objective values should differ", default_value=0.0),
@@ -273,23 +273,33 @@
 
 
 def _group_mip_subgroups():
     return dict(cuts=_group_mip_cuts_make,
                 limits=_group_mip_limits_make,
                 polishafter=_group_mip_polishafter_make,
                 pool=_group_mip_pool_make,
-                submip=_group_mip_submip_make,
                 strategy=_group_mip_strategy_make,
+                submip=_group_mip_submip_make,
                 tolerances=_group_mip_tolerances_make)
 
 
 def _group_mip_make(pgroup):
     return ParameterGroup.make("mip", _group_mip_params, _group_mip_subgroups, pgroup)
 
 
+# generating code for group: MultiObjective
+def _group_multiobjective_params(pgroup):
+    return dict(display=IntParameter(pgroup, "display", "CPX_PARAM_MULTIOBJDISPLAY", 1600, "level of display during multi-objective optimization", default_value=1, min_value=0.0, max_value=2.0)
+)
+
+
+def _group_multiobjective_make(pgroup):
+    return ParameterGroup.make("multiobjective", _group_multiobjective_params, None, pgroup)
+
+
 # generating code for group: Network_Tolerances
 def _group_network_tolerances_params(pgroup):
     return dict(feasibility=NumParameter(pgroup, "feasibility", "CPX_PARAM_NETEPRHS", 5003, "feasibility tolerance", default_value=1e-06, min_value=1e-11, max_value=0.1),
                 optimality=NumParameter(pgroup, "optimality", "CPX_PARAM_NETEPOPT", 5002, "reduced cost optimality tolerance", default_value=1e-06, min_value=1e-11, max_value=0.1)
                 )
 
 
@@ -330,14 +340,15 @@
 def _group_preprocessing_params(pgroup):
     return dict(aggregator=IntParameter(pgroup, "aggregator", "CPX_PARAM_AGGIND", 1003, "limit on applications of the aggregator", default_value=-1, min_value=-1.0, max_value=2100000000),
                 boundstrength=IntParameter(pgroup, "boundstrength", "CPX_PARAM_BNDSTRENIND", 2029, "type of bound strengthening", default_value=-1, min_value=-1.0, max_value=1.0),
                 coeffreduce=IntParameter(pgroup, "coeffreduce", "CPX_PARAM_COEREDIND", 2004, "level of coefficient reduction", default_value=-1, min_value=-1.0, max_value=3.0),
                 dependency=IntParameter(pgroup, "dependency", "CPX_PARAM_DEPIND", 1008, "indicator for preprocessing dependency checker", default_value=-1, min_value=-1.0, max_value=3.0),
                 dual=IntParameter(pgroup, "dual", "CPX_PARAM_PREDUAL", 1044, "take dual in preprocessing", default_value=0, min_value=-1.0, max_value=1.0),
                 fill=PositiveIntParameter(pgroup, "fill", "CPX_PARAM_AGGFILL", 1002, "limit on fill in aggregation", default_value=10, max_value=2100000000),
+                folding=IntParameter(pgroup, "folding", "CPX_PARAM_FOLDING", 1164, "indicator for folding of LPs", default_value=-1, min_value=-1.0, max_value=5.0),
                 linear=IntParameter(pgroup, "linear", "CPX_PARAM_PRELINEAR", 1058, "indicator for linear reductions", default_value=1, min_value=0.0, max_value=1.0),
                 numpass=IntParameter(pgroup, "numpass", "CPX_PARAM_PREPASS", 1052, "limit on applications of presolve", default_value=-1, min_value=-1.0, max_value=2100000000),
                 presolve=BoolParameter(pgroup, "presolve", "CPX_PARAM_PREIND", 1030, "presolve indicator", default_value=1),
                 qcpduals=IntParameter(pgroup, "qcpduals", "CPX_PARAM_CALCQCPDUALS", 4003, "dual calculation for QCPs", default_value=1, min_value=0.0, max_value=2.0),
                 qpmakepsd=BoolParameter(pgroup, "qpmakepsd", "CPX_PARAM_QPMAKEPSDIND", 4010, "indicator to make a binary qp psd or tighter", default_value=1),
                 qtolin=IntParameter(pgroup, "qtolin", "CPX_PARAM_QTOLININD", 4012, "indicator to linearize products in the objective involving binary variables (for convex MIQP), or all products of bounded variables (for global QP)", default_value=-1, min_value=-1.0, max_value=1.0),
                 reduce=IntParameter(pgroup, "reduce", "CPX_PARAM_REDUCE", 1057, "type of primal and dual reductions", default_value=3, min_value=0.0, max_value=3.0),
@@ -460,15 +471,15 @@
                 clocktype=IntParameter(pgroup, "clocktype", "CPX_PARAM_CLOCKTYPE", 1006, "type of clock used to measure time", default_value=2, min_value=0.0, max_value=2.0),
                 dettimelimit=NumParameter(pgroup, "dettimelimit", "CPX_PARAM_DETTILIM", 1127, "deterministic time limit in ticks", default_value=1e+75, min_value=0.0, max_value=1e+75),
                 lpmethod=IntParameter(pgroup, "lpmethod", "CPX_PARAM_LPMETHOD", 1062, "method for linear optimization", default_value=0, min_value=0.0, max_value=6.0),
                 optimalitytarget=IntParameter(pgroup, "optimalitytarget", "CPX_PARAM_OPTIMALITYTARGET", 1131, "type of solution CPLEX will attempt to compute", default_value=0, min_value=0.0, max_value=3.0),
                 parallel=IntParameter(pgroup, "parallel", "CPX_PARAM_PARALLELMODE", 1109, "parallel optimization mode", default_value=0, min_value=-1, max_value=2),
                 paramdisplay=BoolParameter(pgroup, "paramdisplay", "CPX_PARAM_PARAMDISPLAY", 1163, "whether to display changed parameters before optimization", default_value=1),
                 qpmethod=IntParameter(pgroup, "qpmethod", "CPX_PARAM_QPMETHOD", 1063, "method for quadratic optimization", default_value=0, min_value=0.0, max_value=6.0),
-                randomseed=IntParameter(pgroup, "randomseed", "CPX_PARAM_RANDOMSEED", 1124, "seed to initialize the random number generator", default_value=201804051, min_value=0.0, max_value=2100000000),
+                randomseed=IntParameter(pgroup, "randomseed", "CPX_PARAM_RANDOMSEED", 1124, "seed to initialize the random number generator", default_value=201808295, min_value=0.0, max_value=2100000000),
                 record=BoolParameter(pgroup, "record", "CPX_PARAM_RECORD", 1162, "record calls to C API", default_value=0),
                 solutiontype=IntParameter(pgroup, "solutiontype", "CPX_PARAM_SOLUTIONTYPE", 1147, "solution information CPLEX will attempt to compute", default_value=0, min_value=0.0, max_value=2.0),
                 threads=IntParameter(pgroup, "threads", "CPX_PARAM_THREADS", 1067, "default parallel thread count", default_value=0, min_value=0.0, max_value=2100000000),
                 timelimit=NumParameter(pgroup, "timelimit", "CPX_PARAM_TILIM", 1039, "time limit in seconds", default_value=1e+75, min_value=0.0, max_value=1e+75),
                 workdir=StrParameter(pgroup, "workdir", "CPX_PARAM_WORKDIR", 1064, "directory for CPLEX working files", default_value="."),
                 workmem=NumParameter(pgroup, "workmem", "CPX_PARAM_WORKMEM", 1065, "memory available for working storage (in megabytes)", default_value=2048.0, min_value=0.0, max_value=1e+75)
                 )
@@ -478,19 +489,23 @@
     return dict(barrier=_group_barrier_make,
                 benders=_group_benders_make,
                 conflict=_group_conflict_make,
                 distmip=_group_distmip_make,
                 emphasis=_group_emphasis_make,
                 feasopt=_group_feasopt_make,
                 mip=_group_mip_make,
+                multiobjective=_group_multiobjective_make,
                 network=_group_network_make,
                 output=_group_output_make,
                 preprocessing=_group_preprocessing_make,
                 read=_group_read_make,
                 sifting=_group_sifting_make,
                 simplex=_group_simplex_make,
                 tune=_group_tune_make)
 
 
 def make_root_params_12900():
-    return RootParameterGroup.make("parameters", _group_cpxparam_params, _group_cpxparam_subgroups, "12.9.0.0")
+    proot = RootParameterGroup.make("parameters", _group_cpxparam_params, _group_cpxparam_subgroups, "12.9.0.0")
+    # -- set synchronous params
+    proot.read.datacheck._synchronous = True
+    return proot
 #  --- end of generated code ---
```

### Comparing `docplex-2.8.125/docplex/mp/params/parameters.py` & `docplex-2.9.141/docplex/mp/params/parameters.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 # (c) Copyright IBM Corp. 2015, 2016
 # --------------------------------------------------------------------------
 
 from __future__ import print_function
 
 from six import iteritems
 
-from docplex.mp.utils import is_int, is_number, is_string
+from docplex.mp.utils import is_int, is_string
 from docplex.mp.compat23 import StringIO
 from docplex.mp.error_handler import docplex_fatal
 
 
 class ParameterGroup(object):
     """ A group of parameters.
 
@@ -287,15 +287,16 @@
 
 class Parameter(object):
     """ Base class for all parameters.
 
     This class is not meant to be instantiated but subclassed.
 
     """
-    __slots__ = ('_parent', '_short_name', '_cpx_name', '_id', '_description', '_default_value', '_current_value')
+    __slots__ = ('_parent', '_short_name', '_cpx_name', '_id', '_description', '_default_value',
+                 '_current_value', '_synchronous')
 
     # This global flag controls checking new values.
     # If set to False, assigned values are not checked for min/max ranges
     skip_range_check = False
 
     # noinspection PyProtectedMember
     def __init__(self, group, short_name, cpx_name, param_key, description, default_value):
@@ -304,21 +305,23 @@
         self._short_name = short_name
         self._cpx_name = cpx_name
         self._id = param_key
         self._description = description
         self._default_value = default_value
         # current = default at start...
         self._current_value = default_value
+        self._synchronous = False
         # link to parent group
         group._add_param(self)
 
     def ctor_name(self):
         return self.__class__.__name__
 
-
+    def is_synchronous(self):
+        return self._synchronous
 
     @property
     def short_name(self):
         return self._short_name
 
     @property
     def qualified_name(self):
@@ -447,14 +450,18 @@
 
         Raises:
             An exception if the value is not valid.
         """
         accepted_value = self._check_value(new_value)
         if accepted_value is not None:
             self._current_value = accepted_value
+            if self._synchronous:
+                #print(" syncing {0!s} to {1}".format(self, accepted_value))
+                self.root_group().apply(self)
+
         return accepted_value
 
     def get(self):
         """ Returns the current value of the parameter.
         """
         return self._current_value
 
@@ -493,28 +500,28 @@
         """ Converts the parameter to a string.
 
         This method is used in the `__str__` method to convert a parameter to a string.
 
         :rtype:
             string
         """
-        return "{0}:{1:s}(2!s)".format(self._short_name, self.type_name(), self._current_value)
+        return "{0}:{1:s}({2!s})".format(self._short_name, self.type_name(), self._current_value)
 
     def __str__(self):
         return self.to_string()
 
     def is_numeric(self):
         # INTERNAL
         return False  # pragma: no cover
 
     def type_name(self):
         # INTERNAL
         raise NotImplementedError  # pragma: no cover
 
-    def _root_group(self):
+    def root_group(self):
         return self._parent.root_group()
 
     def _repr_classname(self):
         return "docplex.mp.params.{0}".format(self.__class__.__name__)
 
     def __repr__(self):
         return "{0}({1},{2!s})".format(self._repr_classname(), self.qualified_name, self._current_value)
@@ -575,18 +582,19 @@
     def _get_min_value(self):
         return self._min_value  # pragma: no cover
 
     def _get_max_value(self):
         return self._max_value  # pragma: no cover
 
     def __init__(self, group, short_name, cpx_name, param_key, description, default_value, min_value=None,
-                 max_value=None):
+                 max_value=None, sync=False):
         Parameter.__init__(self, group, short_name, cpx_name, param_key, description, default_value)
         self._min_value = min_value
         self._max_value = max_value
+        self._synchronous = sync
 
     def type_name(self):
         return "int"
 
     def __repr__(self):
         return "{0}({1},{2!s})".format(self._repr_classname(), self.qualified_name, self._current_value)
 
@@ -648,14 +656,24 @@
 class RootParameterGroup(ParameterGroup):
     """ The root parameter group (there should be only one instance at the root of the tree).
     """
 
     def __init__(self, name, cplex_version):
         ParameterGroup.__init__(self, name)
         self._cplex_version = cplex_version
+        self._models = []
+
+    def connect_model(self, m):
+        self._models.append(m)
+
+    def apply(self, param):
+        # apply one parameter to connected models
+        for m in self._models:
+            m.apply_one_parameter(param)
+
 
     @property
     def cplex_version(self):
         return self._cplex_version
 
     def is_root(self):
         return True
```

### Comparing `docplex-2.8.125/docplex/mp/sktrans/cpx_mdlr.py` & `docplex-2.9.141/docplex/mp/sktrans/cpx_mdlr.py`

 * *Files identical despite different names*

### Comparing `docplex-2.8.125/docplex/mp/sktrans/docplex_mdlr.py` & `docplex-2.9.141/docplex/mp/sktrans/docplex_mdlr.py`

 * *Files identical despite different names*

### Comparing `docplex-2.8.125/docplex/mp/sktrans/modeler.py` & `docplex-2.9.141/docplex/mp/sktrans/modeler.py`

 * *Files identical despite different names*

### Comparing `docplex-2.8.125/docplex/mp/sktrans/pd_utils.py` & `docplex-2.9.141/docplex/mp/sktrans/pd_utils.py`

 * *Files identical despite different names*

### Comparing `docplex-2.8.125/docplex/mp/sktrans/transformers.py` & `docplex-2.9.141/docplex/mp/sktrans/transformers.py`

 * *Files identical despite different names*

### Comparing `docplex-2.8.125/docplex/mp/sparktrans/spark_utils.py` & `docplex-2.9.141/docplex/mp/sparktrans/spark_utils.py`

 * *Files identical despite different names*

### Comparing `docplex-2.8.125/docplex/mp/sparktrans/transformers.py` & `docplex-2.9.141/docplex/mp/sparktrans/transformers.py`

 * *Files identical despite different names*

### Comparing `docplex-2.8.125/docplex/mp/worker/solve_hook.py` & `docplex-2.9.141/docplex/mp/worker/solve_hook.py`

 * *Files identical despite different names*

### Comparing `docplex-2.8.125/docplex/mp/worker/worker_env.py` & `docplex-2.9.141/docplex/mp/worker/worker_env.py`

 * *Files identical despite different names*

### Comparing `docplex-2.8.125/docplex/mp/__init__.py` & `docplex-2.9.141/docplex/mp/__init__.py`

 * *Files identical despite different names*

### Comparing `docplex-2.8.125/docplex/mp/absmodel.py` & `docplex-2.9.141/docplex/mp/absmodel.py`

 * *Files identical despite different names*

### Comparing `docplex-2.8.125/docplex/mp/advmodel.py` & `docplex-2.9.141/docplex/mp/advmodel.py`

 * *Files identical despite different names*

### Comparing `docplex-2.8.125/docplex/mp/aggregator.py` & `docplex-2.9.141/docplex/mp/aggregator.py`

 * *Files identical despite different names*

### Comparing `docplex-2.8.125/docplex/mp/anno.py` & `docplex-2.9.141/docplex/mp/anno.py`

 * *Files 5% similar despite different names*

```diff
@@ -15,16 +15,14 @@
 
 from six import iteritems
 
 
 class ModelAnnotationPrinter(object):
     # header contains the final newline
     mst_header = """<?xml version = "1.0" standalone="yes"?>
-<?xml-stylesheet href="https://www.ilog.com/products/cplex/xmlv1.0/solution.xsl" type="text/xsl"?>
-
 """
     anno_extension = ".ann"
 
     annotations_start_tag = "<CPLEXAnnotations>\n"
     annotations_end_tag   = "</CPLEXAnnotations>\n"
     benders_start_tag     = " <CPLEXAnnotation name='cpxBendersPartition' type='long' default='0'>\n"
     benders_end_tag       = " </CPLEXAnnotation>\n"
```

### Comparing `docplex-2.8.125/docplex/mp/basic.py` & `docplex-2.9.141/docplex/mp/basic.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 import sys
 from io import StringIO
 
 from enum import Enum
 
 from docplex.mp.operand import Operand
 from docplex.mp.utils import is_number, is_string, str_holo
+from docplex.mp.format import LP_format
 
 
 class ModelingObjectBase(object):
     """ModelingObjectBase()
 
     Parent class for all modeling objects (variables and constraints).
 
@@ -54,14 +55,25 @@
         # INTERNAL: always return a string
         return self._name or ''
 
     def check_name(self, new_name):
         # INTERNAL: basic method for checking names.
         pass  # pragma: no cover
 
+    def check_lp_name(self, new_name):
+        #ModelingObject.check_name(self, new_name)
+        if not is_string(new_name) or not new_name:
+            self.fatal("Variable name accepts only non-empty strings, {0!r} was passed", new_name)
+        elif new_name.find(' ') >= 0:
+            self.warning("Variable name contains blank space, var: {0!s}, name: \'{1!s}\'", self, new_name)
+        elif not LP_format.is_lp_compliant(new_name):
+            self.warning("Candidate variable name is not LP-compliant: '{1}', old_name was: {0} (name will be changed to x<nn>)", self.name, new_name)
+
+
+
     def has_name(self):
         """ Checks whether the object has a name.
 
         Returns:
             True if the object has a name.
 
         """
@@ -139,15 +151,16 @@
         else:  # pragma: no cover
             return self.__unicode__()
 
 
 class ModelingObject(ModelingObjectBase):
     __slots__ = ("_index", "_origin", "_container")
 
-    def is_valid_index(self, idx):
+    @staticmethod
+    def is_valid_index(idx):
         # INTERNAL: This is where the valid index check is performed
         return idx >= 0
 
     _invalid_index = -2
 
     # @profile
     def __init__(self, model, name=None, index=_invalid_index):
@@ -305,16 +318,16 @@
         raise NotImplementedError  # pragma: no cover
 
     @property
     def solution_value(self):
         self._check_model_has_solution()
         return self._get_solution_value()
 
-    def __ne__(self, other):
-        self.model.unsupported_neq_error(self, other)
+    # def __ne__(self, other):
+    #     self.model.unsupported_neq_error(self, other)
 
     def __pow__(self, power):
         # INTERNAL
         # power must be checke in {0, 1, 2}
         self.model.typecheck_as_power(self, power)
         if 0 == power:
             return 1
@@ -371,18 +384,20 @@
     def cplex_preference(self):
         return self._get_geometric_preference_factor(base=10.0)
 
     def _get_geometric_preference_factor(self, base):
         # INTERNAL: returns a CPLEX preference factor as a power of "base"
         # MEDIUM priority is the balance point with a preference of 1.
         assert is_number(base)
-        medium_index = Priority.MEDIUM.value / 100
+
         if self.is_mandatory():
             return 1e+20
         else:
+            # noinspection PyTypeChecker
+            medium_index = Priority.MEDIUM.value / 100
             # pylint complains about no value member but is wrong!
             diff = self.value / 100 - medium_index
             factor = 1.0
             pdiff = diff if diff >= 0 else -diff
             for _ in range(0, int(pdiff)):
                 factor *= base
             return factor if diff >= 0 else 1.0 / factor
```

### Comparing `docplex-2.8.125/docplex/mp/cloudutils.py` & `docplex-2.9.141/docplex/mp/cloudutils.py`

 * *Files identical despite different names*

### Comparing `docplex-2.8.125/docplex/mp/compat23.py` & `docplex-2.9.141/docplex/mp/compat23.py`

 * *Files identical despite different names*

### Comparing `docplex-2.8.125/docplex/mp/conflict_refiner.py` & `docplex-2.9.141/docplex/mp/conflict_refiner.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,20 +4,63 @@
 # (c) Copyright IBM Corp. 2015, 2016
 # --------------------------------------------------------------------------
 
 from collections import namedtuple, Iterable
 from docplex.mp.constants import ComparisonType
 from docplex.mp.context import check_credentials
 from docplex.mp.cloudutils import context_must_use_docloud
+
+from docplex.mp.utils import PublishResultAsDf
+
 import warnings
 
 
+try:
+    import pandas
+except ImportError:
+    pandas = None
+
+
 TConflictConstraint = namedtuple("_TConflictConstraint", ["name", "element", "status"])
 
 
+def trim_field(element):
+    s = str(element)
+    suffix = '...' if len(s) > 100 else ''
+    return s[:100] + suffix
+
+
+def to_output_table(conflicts, use_df=True):
+    # Returns the output tables, as df if pandas is available or as a list
+    # of named tuple ['Type', 'Status', 'Name', 'Expression']
+    columns = ['Type', 'Status', 'Name', 'Expression']
+    TOutputTables = namedtuple('TOutputTables', columns)
+
+    def data_for_df(c):
+        return {'Type': 'Constraint',
+                'Status': c.status.name if c.status is not None else '',
+                'Name': c.name if c.name else '',
+                'Expression': trim_field(c.element)}
+
+    def data_for_namedtuples(c):
+        return TOutputTables('Constraint',
+                             c.status,
+                             c.name if c.name else '',
+                             trim_field(c.element))
+
+    output_data = []
+    data_converter = data_for_df if pandas and use_df else data_for_namedtuples
+    for c in conflicts:
+        output_data.append(data_converter(c))
+    if pandas and use_df:
+        output_data = pandas.DataFrame(columns=columns,
+                                       data=output_data)
+    return output_data
+
+
 class VarUbConstraintWrapper(object):
     """
     This class is a wrapper for a model variable and its associated upper bound.
 
     Instances of this class are created by the ``refine_conflict`` method when the conflict involves
     a variable upper bound. Each of these instances is then referenced by a ``TConflictConstraint`` namedtuple
     in the conflict list returned by ``refine_conflict``.
@@ -123,63 +166,32 @@
         else:
             self.add_constraint(cts)
 
     def get_group_constraints(self):
         return self._cts
 
 
-class ConflictRefiner(object):
+class ConflictRefiner(PublishResultAsDf, object):
     ''' This class is an abstract algorithm; it operates on interfaces.
 
     A conflict is a set of mutually contradictory constraints and bounds within a model.
     Given an infeasible model, the conflict refiner can identify conflicting constraints and bounds
     within it. CPLEX refines an infeasible model by examining elements that can be removed from the
     conflict to arrive at a minimal conflict.
     '''
 
-    def __init__(self):
-        pass
+    def __init__(self, output_processing=None):
+        self.output_table_customizer = output_processing
+        self.output_table_property_name = 'conflicts_output'
+        self.default_output_table_name = 'conflicts.csv'
+        self.output_table_using_df = True
 
     def refine_conflict(self, mdl, preferences=None, groups=None, **kwargs):
         """ Starts the conflict refiner on the model.
 
-        If CPLEX is available, the conflict refinement operation will be performed using the native CPLEX.
-        If CPLEX is not available, the conflict refinement operation will be started on DOcplexcloud.
-        The DOcplexcloud connection parameters are checked in the following order:
-
-            - If ``kwargs`` contains valid ``url`` and ``key`` values, they are used.
-            - If ``kwargs`` contains a ``context`` and that context contains a
-              valid ``solver.docloud.url`` and ``solver.docloud.key`` values,
-              those values are used. Other attributes of ``solver.docloud``
-              can also be used. See :class:`docplex.mp.context.Context`.
-            - Finally, the model's attribute ``context`` is used. This ``context``
-              is set at model creation time.
-
-        If CPLEX is not available and the model has no valid credentials, an error is raised, because there is
-        no way to perform the conflict refinement.
-
-        Note that if the ``url`` and ``key`` parameters are present and the
-        values of the parameters are not in the ignored url or key list,
-        the conflict refinement operation will be started on DOcplexcloud even if CPLEX is
-        available.
-
-        Example::
-
-            # forces the conflict refiner on DOcplexcloud with the specified url and keys
-            crefiner.refine_conflict(url='https://foo.com', key='bar')
-
-        Example::
-
-            # set some DOcplexcloud credentials, but depend on another
-            # method to decide if conflict refiner is local or not
-            ctx.solver.docloud.url = 'https://foo.com'
-            ctx.solver.docloud.key = 'bar'
-            agent = 'local' if method_that_decides_if_solve_is_local() or 'docloud'
-            crefiner.conflict_refiner(context=ctx, agent=agent)
-
         Args:
             mdl: The model to be relaxed.
             preferences: A dictionary defining constraint preferences.
             groups: A list of ConstraintsGroups.
             kwargs: Accepts named arguments similar to solve.
 
         Returns:
@@ -191,47 +203,58 @@
                 - a reference to the constraint or to a wrapper representing a Var upper or lower bound.
                 - a ``docplex.mp.constants.ConflictStatus`` object that indicates the
                   conflict status type (Excluded, Possible_member, Member...).
 
             This list is empty if no conflict is found by the conflict refiner.
         """
 
+        if mdl.has_multi_objective():
+            mdl.fatal("Conflict refiner is not supported for multi-objective")
+
         # take into account local argument overrides
         context = mdl.prepare_actual_context(**kwargs)
 
         # log stuff
         saved_context_log_output = mdl.context.solver.log_output
         saved_log_output_stream = mdl.log_output
 
         try:
             mdl.set_log_output(context.solver.log_output)
 
             forced_docloud = context_must_use_docloud(context, **kwargs)
 
+            results = None
+
             have_credentials = False
             if context.solver.docloud:
                 have_credentials, error_message = check_credentials(context.solver.docloud)
                 if error_message is not None:
                     warnings.warn(error_message, stacklevel=2)
             if forced_docloud:
                 if have_credentials:
-                    return self._refine_conflict_cloud(mdl, context, preferences, groups)
+                    results = self._refine_conflict_cloud(mdl, context, preferences, groups)
                 else:
                     mdl.fatal("DOcplexcloud context has no valid credentials: {0!s}",
                                context.solver.docloud)
             # from now on docloud_context is None
             elif mdl.environment.has_cplex:
                 # if CPLEX is installed go for it
-                return self._refine_conflict_local(mdl, context, preferences, groups)
+                results = self._refine_conflict_local(mdl, context, preferences, groups)
             elif have_credentials:
                 # no context passed as argument, no Cplex installed, try model's own context
-                return self._refine_conflict_cloud(mdl, context, preferences, groups)
+                results = self._refine_conflict_cloud(mdl, context, preferences, groups)
             else:
                 # no way to solve.. really
                 return mdl.fatal("CPLEX DLL not found: please provide DOcplexcloud credentials")
+
+            # write conflicts table.write_output_table() handles everything related to
+            # whether the table should be published etc...
+            if self.is_publishing_output_table(mdl.context):
+                self.write_output_table(to_output_table(results, self.output_table_using_df), mdl.context)
+            return results
         finally:
             if saved_log_output_stream != mdl.log_output:
                 mdl.set_log_output_as_stream(saved_log_output_stream)
             if saved_context_log_output != mdl.context.solver.log_output:
                 mdl.context.solver.log_output = saved_context_log_output
 
     def _refine_conflict_cloud(self, mdl, context, preferences=None, groups=None):
```

### Comparing `docplex-2.8.125/docplex/mp/constants.py` & `docplex-2.9.141/docplex/mp/constants.py`

 * *Files 2% similar despite different names*

```diff
@@ -448,7 +448,31 @@
         else:
             fmt = '* cannot interpret this as a QualityMetric enum: {0!r}'
             if raise_on_error:
                 docplex_fatal(fmt, txt)
             else:
                 print(fmt.format(txt))
                 return None
+
+
+class BasisStatus(Enum):
+
+    def __new__(cls, code, cpx_codename):
+        obj = object.__new__(cls)
+        # predefined
+        obj._value_ = code
+        obj.codename = cpx_codename
+        return obj
+
+    unknown = -1, "Unknown"
+    AtLowerBound = 0, "CPX_AT_LOWER"
+    Basic = 1, "CPX_BASIC"
+    AtUpperBound = 2, "CPX_AT_UPPER"
+    FreeNonBasic = 3, "CPX_FREE_SUPER"
+
+    @classmethod
+    def parse(cls, code):
+        for bs in cls:
+            if bs.value == code:
+                return bs
+        else:
+            return cls.unknown
```

### Comparing `docplex-2.8.125/docplex/mp/constr.py` & `docplex-2.9.141/docplex/mp/constr.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # --------------------------------------------------------------------------
 # Source file provided under Apache License, Version 2.0, January 2004,
 # http://www.apache.org/licenses/
 # (c) Copyright IBM Corp. 2015, 2016
 # --------------------------------------------------------------------------
-from docplex.mp.basic import ModelingObject, Priority, _BendersAnnotatedMixin
-from docplex.mp.constants import ComparisonType, UpdateEvent, CplexScope
+from docplex.mp.basic import ModelingObject, ModelingObjectBase, Priority, _BendersAnnotatedMixin
+from docplex.mp.constants import ComparisonType, UpdateEvent
 from docplex.mp.operand import LinearOperand
 from docplex.mp.sttck import StaticTypeChecker
 
 
 import warnings
 
 
@@ -188,14 +188,17 @@
         """ This property returns the right expression in the constraint.
 
         Example:
             (X+Y <= Z+1) has right expression (Z+1).
         """
         return self._right_expr
 
+    def get_var_coef(self, dvar):
+        return self._left_expr.unchecked_get_coef(dvar) - self._right_expr.unchecked_get_coef(dvar)
+
     def to_string(self):
         """ Returns a string representation of the constraint.
 
         The operators in this representation are the usual operators <=, ==, and >=.
 
         Example:
             The constraint (X+Y <= Z+1) is represented as "X+Y <= Z+1".
@@ -341,47 +344,61 @@
         right_value = self._right_expr._get_solution_value(solution)
         return ComparisonType.almost_compare(left_value, self._ctsense, right_value, eps=tolerance)
 
     def resolve(self):
         self._left_expr.resolve()
         self._right_expr.resolve()
 
+    def is_discrete(self):
+        return self.get_left_expr().is_discrete() and self.get_right_expr().is_discrete()
+
 
 class LinearConstraint(BinaryConstraint, LinearOperand):
     """ The class that models all constraints of the form `<expr1> <OP> <expr2>`,
             where <expr1> and <expr2> are linear expressions.
     """
     __slots__ = ('_super_ct', '_status_var')  # for enclosing indicator if any
 
     def __init__(self, model, left_expr, ctsense, right_expr, name=None):
         BinaryConstraint.__init__(self, model, left_expr, ctsense, right_expr, name)
         left_expr.notify_used(self)
         right_expr.notify_used(self)
 
+    def check_name(self, new_name):
+        if new_name is not None:
+            self.check_lp_name(new_name)
+
+    def set_name(self, new_name):
+        # INTERNAL
+        self.check_name(new_name)
+        if self.has_valid_index():
+            self._model.set_linear_constraint_name(self, new_name)
+        else:
+            self._set_name(new_name)
+
+    name = property(ModelingObjectBase.get_name, set_name)
+
     def notify_used_in_logical_ct(self, lct):
         self._super_ct = lct
 
     def get_super_logical_ct(self):
         # INTERNAL
         return getattr(self, '_super_ct', None)
 
     def is_linear(self):
         return True
 
     def cplex_range_value(self):
         return 0.0
 
-    def is_discrete(self):
-        return self.get_left_expr().is_discrete() and self.get_right_expr().is_discrete()
-
     def copy(self, target_model, var_map):
         copied_left = self.left_expr.copy(target_model, var_map)
         copied_right = self.right_expr.copy(target_model, var_map)
         copy_name = self.name
-        return LinearConstraint(target_model, copied_left, self.sense, copied_right, copy_name)
+        return self.__class__(target_model, copied_left, self.sense, copied_right, copy_name)
 
     @property
     def sense(self):
         """ This property is used to get or set the sense of the constraint; sense is an enumerated value
         of type :class:`ComparisonType`, with three possible values:
 
         - LE for e1 <= e2 constraints
@@ -445,15 +462,15 @@
     # aliases
     lhs = left_expr
     rhs = right_expr
 
     def _no_linear_ct_in_logical_test_error(self):
         if self.sense == ComparisonType.EQ:
             # for equality testing there -is- a workaround
-            msg = "Cannot use == to test expression equality, try using Python is: {0!s}".format(self)
+            msg = "Cannot use == to test expression equality, try using Python is operator or method equals: {0!s}".format(self)
         else:
             msg = "Cannot convert a linear constraint to boolean: {0!s}".format(self)
         raise TypeError(msg)
 
     def _cannot_promote_from_linear_to_quadratic(self, old_expr, new_expr):
         msg = 'Cannot change linear constraint expr from linear to quadratic'
         if new_expr is None:
@@ -600,26 +617,14 @@
             consider using Model.slack_values() with a sequence of constraints.
             
         See Also:
             `func:docplex.mp.model.Model.slack_values()`
         """
         return self._model._slack_value1(self)
 
-    def generate_ordered_vars(self):
-        # INTERNAL
-        left_expr = self.left_expr
-        for lv in left_expr.iter_variables():
-            yield lv
-        for rv in self.right_expr.iter_variables():
-            if rv not in left_expr:
-                yield rv
-
-    def get_var_coef(self, dvar):
-        return self._left_expr.unchecked_get_coef(dvar) - self._right_expr.unchecked_get_coef(dvar)
-
     def iter_net_linear_coefs(self):
         # INTERNAL
         left_expr = self._left_expr
         right_expr = self._right_expr
         if right_expr.is_constant():
             return left_expr.iter_sorted_terms()
         elif left_expr.is_constant():
@@ -727,25 +732,25 @@
 
     def __or__(self, other):
         return self.logical_or(other)
 
     def __and__(self, other):
         return self.logical_and(other)
 
-    def _check_logical_operand(self, other):
+    def _check_logical_operand(self, banner, other):
         if not isinstance(other, LinearConstraint):
-            self.fatal('LinearConstraint.or() expects another linear constraint, got: {0!r}', other)
+            self.fatal('{0} expects another linear constraint, {1!r} was passed', banner, other)
         self._check_is_discrete(other)
 
     def logical_or(self, other):
-        self._check_logical_operand(other)
+        self._check_logical_operand("LinearConstraint.or()", other)
         return self.get_linear_factory().new_constraint_or(self, other)
 
     def logical_and(self, other):
-        self._check_logical_operand(other)
+        self._check_logical_operand("LinearConstraint.and()", other)
         return self.get_linear_factory().new_constraint_and(self, other)
 
     def __rshift__(self, other):
         """ Redefines the right-shift operator to define if-then constraints.
 
             This operator allows to create if-then constraint with the `>>` operator.
             It expects a linear constraint as second argument.
@@ -911,15 +916,15 @@
         """
         return self._expr.iter_variables()
 
     def iter_exprs(self):
         yield self._expr
 
     def cplex_range_value(self, do_raise=True):
-        return self.static_cplex_range_value(self, self._lb, self._ub, lambda : "Range has infeasible domain: {0!s}".format(self),
+        return self.static_cplex_range_value(self, self._lb, self._ub, lambda: "Range has infeasible domain: {0!s}".format(self),
                                              do_raise=do_raise)
 
     @classmethod
     def static_cplex_range_value(cls, logger, lbval, ubval, msg_fun, do_raise=True):
         rangeval = float(lbval - ubval)
         # this should be negative, otherwise fails....
         # no way to model infeasible ranges with cplex rngval.
@@ -959,15 +964,14 @@
         return self.to_string()
 
     def __repr__(self):
         printable_name = self._get_safe_name()
         return "docplex.mp.RangeConstraint[{0}]({1},{2!s},{3})".\
             format(printable_name, self.lb, self._expr, self.ub)
 
-
     def resolve(self):
         self._expr.resolve()
 
     @property
     def benders_annotation(self):
         """
         This property is used to get or set the Benders annotation of a constraint.
@@ -977,14 +981,48 @@
         return self.get_benders_annotation()
 
     @benders_annotation.setter
     def benders_annotation(self, new_anno):
         self.set_benders_annotation(new_anno)
 
 
+class NotEqualConstraint(LinearConstraint):
+
+    def __init__(self, model, negated_eqct, name=None):
+        # assume negated_eqct is the equality constraint we want to negate
+        self._negated_ct = negated_eqct
+        aux_eq_ct_status = self._negated_ct.get_resolved_status_var()
+        zero = model._lfactory.new_zero_expr()
+        LinearConstraint.__init__(self, model, aux_eq_ct_status, ComparisonType.EQ, zero, name)
+        self.lock_discrete()
+
+    def to_string(self):
+        eqct = self._negated_ct
+        return "{0} != {1}".format(eqct._left_expr, eqct._right_expr)
+
+    def set_sense(self, new_sense):
+        self.fatal("cannot modify sense of a not_equal constraint: {0!s}", self)
+
+    @property
+    def negated_constraint(self):
+        return self._negated_ct
+
+    def __str__(self):
+        """ Returns a string representation of the not equals constraint.
+
+        Returns:
+            A string.
+        """
+        return self.to_string()
+
+    def __repr__(self):
+        return "docplex.mp.NotEquals({0}, {1})". \
+            format(self._left_expr, self._right_expr)
+
+
 class LogicalConstraint(AbstractConstraint):
     """ This class models logical constraints.
 
     An equivalence constraint links (both ways) the value of a binary variable
     to the satisfaction of a linear constraint.
     
     If the binary variable equals the truth value (default is 1),
@@ -1239,16 +1277,14 @@
 
     def is_quadratic(self):
         return True
 
     def _get_index_scope(self):
         return self._model._quadct_scope
 
-
-
     __slots__ = ()
 
     def is_trivial(self):
         for qv, nqk in self.iter_net_quads():
             if nqk:
                 return False
         # now check linear parts
@@ -1358,38 +1394,37 @@
 
     This class is not meant to be instantiated by the user.
     To create a piecewise constraint, use the factory method :func:`docplex.mp.model.Model.piecewise`
     defined on :class:`docplex.mp.model.Model`.
 
     """
 
-    __slots__ = ('_pwl_expr', '_pwl_func', '_expr', '_y')
+    __slots__ = ('_pwl_expr', '_pwl_func', '_input_var', '_y')
 
     def __init__(self, model, pwl_expr, name=None):
         AbstractConstraint.__init__(self, model, name)
         self._pwl_expr = pwl_expr
         self._pwl_func = pwl_expr.pwl_func
-        self._expr = pwl_expr._x_var
+        self._input_var = pwl_expr._x_var
         self._y = None
 
     def resolve(self):
         self._pwl_expr.resolve()
 
     def is_satisfied(self, solution, tolerance):
-        expr_value = self._expr._get_solution_value(solution)
+        expr_value = self._input_var._get_solution_value(solution)
         y_value = solution._get_var_value(self._y)
         computed_f_expr_value = self._pwl_func.evaluate(expr_value)
         return ComparisonType.almost_equal(y_value, computed_f_expr_value, tolerance)
 
-
     @property
     def expr(self):
         """ This property returns the linear expression of the piecewise linear constraint.
         """
-        return self._expr
+        return self._input_var
 
     @property
     def pwl_func(self):
         """ This property returns the piecewise linear function of the piecewise linear constraint.
         """
         return self._pwl_func
 
@@ -1399,33 +1434,38 @@
         """
         if self._y is None:
             self._y = self._pwl_expr._get_allocated_f_var()
         return self._y
 
     @property
     def usage_counter(self):
-        """ This property returns the usage counter of the piecewise linear function associated with the
-        piecewise linear constraint.
-        """
         return self._pwl_expr.usage_counter
 
     def _get_index_scope(self):
         return self._model._pwl_scope
 
     def iter_variables(self):
         """Iterates over all the variables of the piecewise linear constraint.
 
         Returns:
            An iterator object.
         """
-        y = self.y
-        yield y
-        for v in self.expr.iter_variables():
-            if v is not y:
-                yield v
+        yield self.y
+        yield self._input_var
+
+
+    def iter_extended_variables(self):
+        # iterates on all extended variables involved in the computation
+        # yvar, xavr, plus all argument rexpr vars
+        # if argument var is identical to the input var, it is returned twice...?
+        yield self.y
+        yield self._input_var
+        for v in self._pwl_expr._argument_expr.iter_variables():
+            yield v
+
 
     def get_var_coef(self, dvar):
         if dvar is self.y:
             return 1
         else:
             return self.expr.unchecked_get_coef(dvar)
```

### Comparing `docplex-2.8.125/docplex/mp/context.py` & `docplex-2.9.141/docplex/mp/context.py`

 * *Files 4% similar despite different names*

```diff
@@ -41,15 +41,15 @@
 import socket
 import sys
 import warnings
 from os.path import isfile, isabs
 
 from docplex.util.environment import get_environment
 
-from docplex.mp.utils import is_string, open_universal_newline
+from docplex.mp.utils import is_string, open_universal_newline, get_auto_publish_names
 from docplex.mp.environment import Environment
 from docplex.mp.params.cplex_params import get_params_from_cplex_version
 from docplex.mp.params.parameters import RootParameterGroup
 from docplex.mp.utils import DOcplexException
 from docplex.mp.error_handler import docplex_fatal
 
 try:
@@ -139,38 +139,14 @@
         try:
             auto_publish_details = context.solver.auto_publish
         except AttributeError:
             auto_publish_details = False
     return auto_publish_details
 
 
-def get_auto_publish_names(context, prop_name, default_name):
-    # comparing auto_publish to boolean values because it can be a non-boolean
-    if context.solver.auto_publish is True:
-        return [default_name]
-    elif context.solver.auto_publish is False:
-        return None
-    name = context.solver.auto_publish[prop_name]
-    if isinstance(name, six.string_types):
-        # only one string value: make this the name of the table
-        # in a list with one object
-        name = [name]
-    elif name is True:
-        # if true, then use default name:
-        name = [default_name]
-    elif name is False:
-        # Need to compare explicitely to False
-        name = None
-    else:
-        # otherwise the kpi_table_name can be a collection-like of names,
-        # just return it
-        pass
-    return name
-
-
 def auto_publishing_result_output_names(context):
     # Return the list of result output names for saving
     return get_auto_publish_names(context, 'result_output', 'solution.json')
 
 
 def auto_publising_kpis_table_names(context):
     # Return the list of kpi table names for saving
@@ -643,18 +619,22 @@
     # in a future version, we might want to be able to set individual
     # default values with a dict => that's why we compare to True and False
     if defaults is True and get_solve_hook:
         # Set default values when in a worker
         auto_publish.solve_details = True
         auto_publish.result_output = 'solution.json'
         auto_publish.kpis_output = 'kpis.csv'
+        auto_publish.relaxations_output = 'relaxations.csv'
+        auto_publish.conflicts_output = 'conflicts.csv'
     else:
         auto_publish.solve_details = False
         auto_publish.result_output = None
         auto_publish.kpis_output = None
+        auto_publish.relaxations_output = None
+        auto_publish.conflicts_output = None
     return auto_publish
 
 
 def CreateDefaultDOcloudContext():
     # Returns a context to use as the context.solver.docloud member.
     #
     # This is a Context with predefined fields.
```

### Comparing `docplex-2.8.125/docplex/mp/cplex_engine.py` & `docplex-2.9.141/docplex/mp/cplex_engine.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 from collections import defaultdict
 
 from docplex.mp.engine import DummyEngine
 from docplex.mp.utils import DOcplexException, str_holo, iter_one
 from docplex.mp.compat23 import izip
 
-from docplex.mp.constants import ConflictStatus, SolveAttribute
+from docplex.mp.constants import ConflictStatus
 from docplex.mp.constr import IndicatorConstraint, QuadraticConstraint, LinearConstraint, RangeConstraint, BinaryConstraint, \
     EquivalenceConstraint
 from docplex.mp.progress import ProgressData
 from docplex.mp.solution import SolveSolution
 from docplex.mp.sdetails import SolveDetails
 from docplex.mp.conflict_refiner import TConflictConstraint, VarLbConstraintWrapper, VarUbConstraintWrapper
 import cplex
@@ -35,14 +35,42 @@
 
 # noinspection PyProtectedMember
 import cplex._internal._constants as cpx_cst
 from cplex._internal._procedural import chgcoeflist, chgobj, chgrhs, chgqpcoef, newcols, setintparam, \
     addindconstr, addrows, chgrngval, addpwl, getnumpwl
 from cplex._internal._subinterfaces import IndicatorConstraintInterface
 from cplex.exceptions import CplexError, CplexSolverError
+try:
+    # from 12.9 up
+    from cplex._internal._procedural import multiobjsetobj
+    DEFAULT_CPX_NO_WEIGHT_CHANGE = cpx_cst.CPX_NO_WEIGHT_CHANGE
+    DEFAULT_CPX_NO_PRIORITY_CHANGE = cpx_cst.CPX_NO_PRIORITY_CHANGE
+    DEFAULT_CPX_NO_ABSTOL_CHANGE = cpx_cst.CPX_NO_ABSTOL_CHANGE
+    DEFAULT_CPX_NO_RELTOL_CHANGE = cpx_cst.CPX_NO_RELTOL_CHANGE
+
+    DEFAULT_CPX_STAT_MULTIOBJ_OPTIMAL = cpx_cst.CPX_STAT_MULTIOBJ_OPTIMAL
+    DEFAULT_CPX_STAT_MULTIOBJ_INForUNBD = cpx_cst.CPX_STAT_MULTIOBJ_INForUNBD
+    DEFAULT_CPX_STAT_MULTIOBJ_UNBOUNDED = cpx_cst.CPX_STAT_MULTIOBJ_UNBOUNDED
+    DEFAULT_CPX_STAT_MULTIOBJ_INFEASIBLE = cpx_cst.CPX_STAT_MULTIOBJ_INFEASIBLE
+    DEFAULT_CPX_STAT_MULTIOBJ_NON_OPTIMAL = cpx_cst.CPX_STAT_MULTIOBJ_NON_OPTIMAL
+    DEFAULT_CPX_STAT_MULTIOBJ_STOPPED = cpx_cst.CPX_STAT_MULTIOBJ_STOPPED
+
+except ImportError:
+    multiobjsetobj = None
+    DEFAULT_CPX_NO_WEIGHT_CHANGE = None
+    DEFAULT_CPX_NO_PRIORITY_CHANGE = None
+    DEFAULT_CPX_NO_ABSTOL_CHANGE = None
+    DEFAULT_CPX_NO_RELTOL_CHANGE = None
+
+    DEFAULT_CPX_STAT_MULTIOBJ_OPTIMAL = None
+    DEFAULT_CPX_STAT_MULTIOBJ_INForUNBD = None
+    DEFAULT_CPX_STAT_MULTIOBJ_UNBOUNDED = None
+    DEFAULT_CPX_STAT_MULTIOBJ_INFEASIBLE = None
+    DEFAULT_CPX_STAT_MULTIOBJ_NON_OPTIMAL = None
+    DEFAULT_CPX_STAT_MULTIOBJ_STOPPED = None
 
 try:
     # from 12.7.1 up
     from cplex._internal._procedural import chbmatrix
 except ImportError:  # pragma: no cover
     # up to 12.7.0
     try:
@@ -58,21 +86,21 @@
 from docplex.mp.constants import QualityMetric, UpdateEvent as upd
 
 from docplex.mp.environment import Environment
 from docplex.mp.engine import NoSolveEngine
 
 try:
     from cplex._internal._pwl import PWLConstraintInterface
-except ImportError:  #  pragma: no cover
+except ImportError:  # pragma: no cover
     PWLConstraintInterface = None
 
 try:
     cpx_indicator_type_ifthen = cpx_cst.CPX_INDICATOR_IF
     cpx_indicator_type_equiv = cpx_cst.CPX_INDICATOR_IFANDONLYIF
-except AttributeError:  #  pragma: no cover
+except AttributeError:  # pragma: no cover
     # handle previous versions without indicator type
     cpx_indicator_type_ifthen = None
     cpx_indicator_type_equiv = None
 
 # -- build annotation map if possible
 
 from docplex.mp.constants import CplexScope
@@ -83,15 +111,15 @@
 
     annotation_map = {CplexScope.VAR_SCOPE: cpx_cst.CPX_ANNOTATIONOBJ_COL,
                       CplexScope.LINEAR_CT_SCOPE: cpx_cst.CPX_ANNOTATIONOBJ_ROW,
                       CplexScope.IND_CT_SCOPE: cpx_cst.CPX_ANNOTATIONOBJ_IND,
                       CplexScope.QUAD_CT_SCOPE: cpx_cst.CPX_ANNOTATIONOBJ_QC,
                       CplexScope.SOS_SCOPE: cpx_cst.CPX_ANNOTATIONOBJ_SOS}
 
-except (ImportError, AttributeError):  #  pragma: no cover
+except (ImportError, AttributeError):  # pragma: no cover
     LongAnnotationInterface = None
     setlonganno = None
     annotation_map = {}
 
 
 # gendoc: ignore
 def fast_add_linear(cpx, lin_expr, cpx_senses, rhs, names, ranges=None):
@@ -114,17 +142,24 @@
 
         return six.moves.range(num_old_rows, cpx_linearcts.get_num())
     else:  #  pragma: no cover
         return cpx.linear_constraints.add(lin_expr=lin_expr, senses=cpx_senses, rhs=rhs, names=names,
                                           range_values=ranges)
 
 
+def _is_defined_multiobjsetobj():
+    if multiobjsetobj is None:
+        return False
+    return True
+
+
 def static_fast_set_linear_obj(cpx, indices, obj_coefs):
     chgobj(cpx._env._e, cpx._lp, indices, obj_coefs)
 
+
 class ConnectListenersCallback(MIPInfoCallback):
     RELATIVE_EPS = 1e-5
     ABS_EPS = 1e-4
 
     # noinspection PyAttributeOutsideInit
     def initialize(self, listeners):
         self.__listeners = listeners
@@ -165,16 +200,14 @@
             if has_incumbent:
                 # get incumbent values as a list of values (value[v] at position index[v])
                 cpx_incumbent_values = self.get_incumbent_values()
                 for sl in self.__solution_listeners:
                     sl.notify_solution(cpx_incumbent_values)
 
 
-
-
 # internal
 class _CplexSyncMode(Enum):
     InSync, InResync, OutOfSync = [1, 2, 3]
 
 
 class CplexIndexMode(Enum):
     # enumerated value for different ways to handle cplex indices.
@@ -284,20 +317,20 @@
             self.long_annotations._setup(self)
 
 
 def _safe_cplex():
     try:
         cpxv = cplex.__version__
         cpx = cplex.Cplex()
-    except AttributeError:  #  pragma: no cover
+    except AttributeError:  # pragma: no cover
         # older version: use an instance
         cpx = cplex.Cplex()
         cpxv = cpx.get_version()
 
-    if cpxv.startswith('12.7.0'):  #  pragma: no cover
+    if cpxv.startswith('12.7.0'):  # pragma: no cover
         if cpx:
             del cpx
         # create a safe wrapper for RTC-31555
         return _SafeCplexWrapper()
     else:
         return cpx
 
@@ -308,42 +341,43 @@
         CPLEX engine wrapper.
     """
     CPX_RANGE_SYMBOL = 'R'
 
     cplex_error_re = re.compile(r'CPLEX Error\s+(\d+)')
 
     if cpx_indicator_type_equiv is None:
-        supports_typed_indicators = False  #  pragma: no cover
+        supports_typed_indicators = False  # pragma: no cover
     else:
         try:
             # noinspection PyStatementEffect
             IndicatorConstraintInterface.type_
             supports_typed_indicators = True
         except AttributeError:  # pragma: no cover
             supports_typed_indicators = False
 
     def supports_logical_constraints(self):
         ok = self._cplex.get_version() >= '12.8.0' and self.supports_typed_indicators
         msg = 'Logical constraints require CPLEX version 12.8 or above, this is CPLEX version: {0}'.format(
             self._cplex.get_version()) if not ok else None
         return ok, msg
 
-    def solved_as_lp(self):
-        return self._cplex.get_problem_type() == 0
+    def solved_as_mip(self):
+        return self._cplex.get_problem_type() not in\
+               {cpx_cst.CPXPROB_LP, cpx_cst.CPXPROB_QP, cpx_cst.CPXPROB_QCP}
 
     def __init__(self, mdl, **kwargs):
         """
         INTERNAL
         :param mdl: the model
         :param index_mode: a string describing how cplex indices are to be managed
         :return:
         """
         DummyEngine.__init__(self)
         cpx = cplex.Cplex()
-        if cpx.get_version().startswith('12.7.0'):  #  pragma: no cover
+        if cpx.get_version().startswith('12.7.0'):  # pragma: no cover
             del cpx
             # create a safe wrapper for RTC-31555
             cpx = _SafeCplexWrapper()
 
         # resetting DATACHECK to 0 has no measurable effect
         # cpx.parameters._set(1056, 0)
 
@@ -423,15 +457,14 @@
             error_handler.fatal("Wrong number of streams, should be 4: {0!s}", len(streams))
         else:
             cpx.set_log_stream(streams[0])
             cpx.set_results_stream(streams[1])
             cpx.set_error_stream(streams[2])
             cpx.set_warning_stream(streams[3])
 
-
     def set_streams(self, out):
         self_log_output = self._saved_log_output
         if self_log_output != out:
             self._cpx_set_all_streams(self._cplex, out)
             self._saved_log_output = out
 
     def get_var_index(self, dvar):  # pragma: no cover
@@ -577,43 +610,58 @@
 
     def set_var_ub(self, dvar, ub):
         self._resync_if_needed()
         self_var_ubs = self._var_ub_changed
         self_var_ubs[dvar] = float(ub)  # force float here: numpy types will crash
 
 
-    def make_attribute_map_from_scope(self, mdl, cplexfn, scope):
+    def make_attribute_map_from_scope_fn(self, mdl, cplexfn, scope):
         # transforms an array of cplex values into a map
         # using the scope object as a mapper
         all_values = cplexfn()
+        return self.make_attribute_map_from_scope_list(mdl, all_values, scope)
+
+    @classmethod
+    def make_attribute_map_from_scope_list(cls, mdl, values, scope, keep_zeros=False):
         value_map = {}
-        for ix, cplex_value in enumerate(all_values):
+        for ix, cplex_value in enumerate(values):
             mobj = scope(ix)
             if mobj is None:
                 mdl.warning("No object with index: {}", ix)
-            elif cplex_value:
+            elif keep_zeros or cplex_value:
                 value_map[mobj] = cplex_value
 
         return value_map
 
     def get_all_reduced_costs(self, mdl):
-        return self.make_attribute_map_from_scope(mdl, self._cplex.solution.get_reduced_costs, mdl._var_scope)
+        return self.make_attribute_map_from_scope_fn(mdl, self._cplex.solution.get_reduced_costs, mdl._var_scope)
 
     def get_all_dual_values(self, mdl):
-        return self.make_attribute_map_from_scope(mdl, self._cplex.solution.get_dual_values, mdl._linct_scope)
+        return self.make_attribute_map_from_scope_fn(mdl, self._cplex.solution.get_dual_values, mdl._linct_scope)
 
     def get_all_slack_values(self, mdl):
-        lin_slacks =  self.make_attribute_map_from_scope(mdl, self._cplex.solution.get_linear_slacks, mdl._linct_scope)
-        quad_slacks = self.make_attribute_map_from_scope(mdl, self._cplex.solution.get_quadratic_slacks, mdl._quadct_scope)
-        ind_slacks = self.make_attribute_map_from_scope(mdl, self._cplex.solution.get_indicator_slacks, mdl._indicator_scope)
+        lin_slacks  = self.make_attribute_map_from_scope_fn(mdl, self._cplex.solution.get_linear_slacks,    mdl._linct_scope)
+        quad_slacks = self.make_attribute_map_from_scope_fn(mdl, self._cplex.solution.get_quadratic_slacks, mdl._quadct_scope)
+        ind_slacks  = self.make_attribute_map_from_scope_fn(mdl, self._cplex.solution.get_indicator_slacks, mdl._indicator_scope)
         # dict : cplex_scope -> dict from obj to slack
         return {CplexScope.LINEAR_CT_SCOPE: lin_slacks,
                 CplexScope.QUAD_CT_SCOPE: quad_slacks,
                 CplexScope.IND_CT_SCOPE: ind_slacks}
 
+    def get_basis(self, mdl):
+        try:
+            status_vars, status_licnts = self._cplex.solution.basis.get_basis()
+            var_statuses_map = self.make_attribute_map_from_scope_list(mdl, status_vars, mdl._var_scope, keep_zeros=True)
+            status_linearct_map = self.make_attribute_map_from_scope_list(mdl, status_licnts, mdl._linct_scope, keep_zeros=True)
+            return var_statuses_map, status_linearct_map
+        except CplexError as cpxe:
+            if cpxe.args[2] == 1262:  # code 1262 is "no basis exists"
+                return {}, {}
+            else:
+                raise
 
     # the returned list MUST be of size 2 otherwise the wrapper will crash.
     _trivial_linexpr = [[], []]
 
     @classmethod
     def linear_ct_to_cplex(cls, linear_ct):
         # INTERNAL
@@ -704,18 +752,15 @@
         has_ranges = False
         for ct in linct_seq:
             if ct.cplex_range_value():
                 has_ranges = True
                 break
 
         range_values = [ct.cplex_range_value() for ct in linct_seq] if has_ranges else None
-
-        ret_add = fast_add_linear(self._cplex, cpx_linexprs, cpx_sense_string, cpx_rhss, cpx_names,
-                                        ranges=range_values)
-
+        ret_add = fast_add_linear(self._cplex, cpx_linexprs, cpx_sense_string, cpx_rhss, cpx_names, ranges=range_values)
         return self._allocate_range_index(size=block_size, ret_value=ret_add, scope=self._lincts_scope)
 
     def create_range_constraint(self, range_ct):
         self._resync_if_needed()
 
         expr = range_ct.expr
 
@@ -735,14 +780,20 @@
         # ret_add = linearcts.add(lin_expr=cpx_linexpr2,
         #                         senses=range_ct.cplex_code(),
         #                         rhs=cpx_rhs,
         #                         range_values=cpx_range_values,
         #                         names=cpx_names)
         return self._allocate_one_index(ret_value=ret_add, scope=self._lincts_scope, expect_range=True)
 
+    def rename_linear_constraint(self, linct, new_name):
+        safe_new_name = new_name or ""
+        linct_index = linct.get_index()
+        cpxlinears = self._cplex.linear_constraints
+        cpxlinears.set_names([(linct_index, safe_new_name)])
+
     def create_indicator_constraint(self, indicator):
         ret = self.create_batch_indicator_constraints(iter_one(indicator))
         return ret[0]
         # self._resync_if_needed()
         # linear_ct = indicator.linear_constraint
         # ct_name = indicator.get_name()
         # active_value = indicator._active_value
@@ -967,14 +1018,34 @@
                 indices[i] = dv._index
                 koefs[i] = float(k)
                 i += 1
 
             cpx = self._cplex
             chgobj(cpx._env._e, cpx._lp, indices, koefs)
 
+    def _fast_set_linear_multiobj(self, objidx, linexpr,
+                                  weight=DEFAULT_CPX_NO_WEIGHT_CHANGE,
+                                  priority=DEFAULT_CPX_NO_PRIORITY_CHANGE,
+                                  abstol=DEFAULT_CPX_NO_ABSTOL_CHANGE,
+                                  reltol=DEFAULT_CPX_NO_RELTOL_CHANGE,
+                                  objname=None):
+        nterms = linexpr.number_of_terms()
+        indices = [-1] * nterms
+        koefs = [0] * nterms
+        if nterms:
+            i = 0
+            for dv, k in linexpr.iter_terms():
+                indices[i] = dv._index
+                koefs[i] = float(k)
+                i += 1
+
+        cpx = self._cplex
+        multiobjsetobj(cpx._env._e, cpx._lp, objidx, objind=indices, objval=koefs,
+                       priority=priority, weight=weight, abstol=abstol, reltol=reltol, objname=objname)
+
     def _fast_update_linearct_coefs(self, ct_index, var_indices, coefs):
         assert len(var_indices) == len(coefs)
 
         num_coefs = len(coefs)
         cpx = self._cplex
         chgcoeflist(cpx._env._e, cpx._lp, [ct_index] * num_coefs, var_indices, coefs)
 
@@ -1099,14 +1170,22 @@
         cpx_obj_sense = 1 if sense.is_minimize() else -1
         self._cplex.objective.set_sense(cpx_obj_sense)
 
     def _clear_objective_from_cplex(self, cpxobj):
         self._clear_linear_objective_from_cplex(cpxobj)
         self._clear_quad_objective_from_cplex(cpxobj)
 
+    def _clear_multiobj_from_cplex(self, cpx_multiobj):
+        numobj = cpx_multiobj.get_num()
+        for objidx in range(numobj):
+            cpx_linear = cpx_multiobj.get_linear(objidx)
+            zap_linear = [(idx, 0) for idx, k in enumerate(cpx_linear) if k]
+            if zap_linear:
+                cpx_multiobj.set_linear(objidx, zap_linear)
+
     def _clear_linear_objective_from_cplex(self, cpxobj):
         # clear linear part
         cpx_linear = cpxobj.get_linear()
         zap_linear = [(idx, 0) for idx, k in enumerate(cpx_linear) if k]
         if zap_linear:
             cpxobj.set_linear(zap_linear)
 
@@ -1154,24 +1233,70 @@
             # cannot use the old expression for clearing, it has been modified
             self._clear_objective_from_cplex(cpxobj=cpx_objective)
         elif old_objexpr is not None:
             self._clear_objective(old_objexpr)
         else:
             # no clearing
             pass
+        # # if a multi-objective has been defined, clear it
+        # cpx_multiobj = self._cplex.multiobj
+        # if cpx_multiobj is not None:
+        #     self._clear_multiobj_from_cplex(cpx_multiobj=cpx_multiobj)
 
         # --- set offset
         cpx_objective.set_offset(float(new_objexpr.get_constant()))
         # --- set coefficients
         if new_objexpr.is_quad_expr():
             self._fast_set_quadratic_objective(quad_expr=new_objexpr)
             self._fast_set_linear_objective(new_objexpr.linear_part)
         else:
             self._fast_set_linear_objective2(linexpr=new_objexpr)
 
+    def set_multi_objective_exprs(self, new_multiobjexprs, old_multiobjexprs, multiobj_params=None,
+                                  priorities=None, weights=None, abstols=None, reltols=None, objnames=None):
+        self._check_multi_objective_support()
+
+        cpx_multiobj = self._cplex.multiobj
+        # old multi objective
+
+        if old_multiobjexprs is not None:
+            # Not safe to use the old expressions for clearing, in case they have been modified for the new expressions
+            self._clear_multiobj_from_cplex(cpx_multiobj=cpx_multiobj)
+        else:
+            # no clearing
+            pass
+        # # if a regular single objective has been defined, clear it
+        # cpx_objective = self._cplex.objective
+        # if cpx_objective is not None:
+        #     self._clear_objective_from_cplex(cpxobj=cpx_objective)
+
+        # --- set number of objectives
+        cpx_multiobj.set_num(len(new_multiobjexprs))
+        for objidx, new_objexpr in enumerate(new_multiobjexprs):
+            # --- set offset
+            cpx_multiobj.set_offset(objidx, float(new_objexpr.get_constant()))
+            # --- set coefficients
+            weight = DEFAULT_CPX_NO_WEIGHT_CHANGE
+            priority = DEFAULT_CPX_NO_PRIORITY_CHANGE
+            abstol = DEFAULT_CPX_NO_ABSTOL_CHANGE
+            reltol = DEFAULT_CPX_NO_RELTOL_CHANGE
+            objname = None
+            if priorities is not None and len(priorities) >= objidx + 1:
+                priority = priorities[objidx]
+            if weights is not None and len(weights) >= objidx + 1:
+                weight = weights[objidx]
+            if abstols is not None and len(abstols) >= objidx + 1:
+                abstol = abstols[objidx]
+            if reltols is not None and len(reltols) >= objidx + 1:
+                reltol = reltols[objidx]
+            if objnames is not None and len(objnames) >= objidx + 1:
+                objname = objnames[objidx]
+            self._fast_set_linear_multiobj(objidx, linexpr=new_objexpr, weight=weight, priority=priority,
+                                           abstol=abstol, reltol=reltol, objname=objname)
+
     def _set_linear_objective_coefs(self, cpx_objective, linexpr):
         # NOTE: convert to float as numpy doubles will crash cplex....
         #     index_coef_seq = [(dv._index, float(k)) for dv, k in linexpr.iter_terms()]
         #     if index_coef_seq:
         #         # if list is empty, cplex will crash.
         #         cpx_objective.set_linear(index_coef_seq)
         self._fast_set_linear_objective(linexpr)
@@ -1196,27 +1321,49 @@
             if quad_reset_triplets:
                 cpx_objective.set_quadratic_coefficients(quad_reset_triplets)
             # 2. reset linear part
             self._clear_linear_objective(expr.linear_part)
         else:
             self._clear_linear_objective(expr)
 
+    def _clear_multiobj(self, exprs):
+        # INTERNAL
+        self._resync_if_needed()
+        for objidx, expr in enumerate(exprs):
+            if expr.is_constant():
+                pass  # resetting offset will do.
+            else:
+                self._clear_linear_multiobj(objidx, expr)
+
     def _clear_linear_objective(self, linexpr):
         # compute the sequence of  var indices, then an array of zeroes
         size = linexpr.number_of_terms()
         if size:
             indices = [-1] * size
             i = 0
             for dv, _ in linexpr.iter_terms():
                 indices[i] = dv._index
                 i += 1
             zeros = [0] * size
             cpx = self._cplex
             chgobj(cpx._env._e, cpx._lp, indices, zeros)
 
+    def _clear_linear_multiobj(self, objidx, linexpr):
+        # compute the sequence of var indices, then an array of zeroes
+        size = linexpr.number_of_terms()
+        if size:
+            indices = [-1] * size
+            i = 0
+            for dv, _ in linexpr.iter_terms():
+                indices[i] = dv._index
+                i += 1
+            zeros = [0] * size
+            cpx = self._cplex
+            multiobjsetobj(cpx._env._e, cpx._lp, objidx, objind=indices, objval=zeros)
+
     @staticmethod
     def status2string(cpx_status):  # pragma: no cover
         ''' Converts a CPLEX integer status value to a string'''
         return _subinterfaces.SolutionInterface.status.__getitem__(cpx_status)
 
     _CPLEX_SOLVE_OK_STATUSES = frozenset({1,  # CPX_STAT_OPTIMAL
                                           6,  # CPX_STAT_NUM_BEST: solution exists but numerical issues
@@ -1227,15 +1374,17 @@
                                           105,  # CPXMPI_NODE_LIM_FEAS
                                           107,  # CPXMIP_TIME_LIM_FEAS
                                           109,  # CPXMIP_FAIL_FEAS : what is this ??
                                           111,  # CPXMIP_MEM_LIM_FEAS
                                           113,  # CPXMIP_ABORT_FEAS
                                           116,  # CPXMIP_FAIL_FEAS_NO_TREE : integer sol exists (????)
                                           129,  # CPXMIP_OPTIMAL_POPULATED
-                                          130  # CPXMIP_OPTIMAL_POPULATED_TOL
+                                          130,  # CPXMIP_OPTIMAL_POPULATED_TOL
+                                          301,  # CPX_STAT_MULTIOBJ_OPTIMAL
+                                          305  # CPX_STAT_MULTIOBJ_NON_OPTIMAL
                                           })
 
     @classmethod
     def _is_solve_status_ok(cls, status):
         # Converts a raw CPLEX status to a boolean
         return status in cls._CPLEX_SOLVE_OK_STATUSES
 
@@ -1246,15 +1395,16 @@
                                           cpx_cst.CPXMIP_FEASIBLE_RELAXED_INF,
                                           cpx_cst.CPXMIP_FEASIBLE_RELAXED_QUAD,
                                           cpx_cst.CPXMIP_FEASIBLE_RELAXED_SUM,
                                           cpx_cst.CPX_STAT_FEASIBLE_RELAXED_SUM,
                                           cpx_cst.CPX_STAT_FEASIBLE_RELAXED_INF,
                                           cpx_cst.CPX_STAT_FEASIBLE_RELAXED_QUAD,
                                           cpx_cst.CPX_STAT_OPTIMAL_RELAXED_INF,
-                                          cpx_cst.CPX_STAT_OPTIMAL_RELAXED_SUM
+                                          cpx_cst.CPX_STAT_OPTIMAL_RELAXED_SUM,
+                                          cpx_cst.CPXMIP_ABORT_RELAXED
                                           }).union(_CPLEX_SOLVE_OK_STATUSES)
 
     @classmethod
     def _is_relaxed_status_ok(cls, status):
         # list all status values for which there is a relaxed solution.
         # also consider solve statuses in case  the model is indeed feasible
         return status in cls._CPLEX_RELAX_OK_STATUSES
@@ -1328,28 +1478,45 @@
             elif cpx_anno.get_num():
                 cpx_anno.delete()
 
         except AttributeError:  #  pragma: no cover
             if annotated_by_scope:
                 self._model.fatal('Annotations require CPLEX 12.7.1 or higher')
 
-    def _apply_sos(self, mdl):
-        # INTERNAL
-        cpx_sos = self._cplex.SOS
-        # start by deleting all SOS: du passe faisons table rase....
-        cpx_sos.delete()
-        for sos_set in mdl.iter_sos():
-            cpx_sos_type = sos_set.sos_type._cpx_sos_type()
-            indices = [dv.index for dv in sos_set.iter_variables()]
-            weights = sos_set.get_ranks()
-            # do NOT pass None to cplex/swig here --> crash
-            cpx_sos_name = sos_set._get_safe_name()
-            # call cplex...
-            sos_index = cpx_sos.add(type=cpx_sos_type, SOS=cplex.SparsePair(ind=indices, val=weights),
-                                    name=cpx_sos_name)
+    def create_sos(self, sos_set):
+        cpx_sos_type = sos_set.sos_type._cpx_sos_type()
+        indices = [dv.index for dv in sos_set.iter_variables()]
+        weights = sos_set.get_ranks()
+        # do NOT pass None to cplex/swig here --> crash
+        cpx_sos_name = sos_set._get_safe_name()
+        # call cplex...
+        sos_index = self._cplex.SOS.add(type=cpx_sos_type,
+                                        SOS=cplex.SparsePair(ind=indices, val=weights),
+                                        name=cpx_sos_name)
+        return sos_index
+
+    def clear_all_sos(self):
+        self._cplex.SOS.delete()
+
+    def add_lazy_constraints(self, lazy_cts):
+        # lazy_cts is a sequence of linear constraints
+        cpx_rhss = [ct.cplex_num_rhs() for ct in lazy_cts]
+        cpx_senses = "".join(ct.cplex_code() for ct in lazy_cts)
+        if self._model.ignore_names:
+            cpx_names = []
+        else:
+            cpx_names = [ct._get_safe_name() for ct in lazy_cts]
+        cpx_convert_fn = self.linear_ct_to_cplex
+        cpx_linexprs = [cpx_convert_fn(ct) for ct in lazy_cts]
+        # TODO: switch to proecedural API at some point...
+        self._cplex.linear_constraints.advanced.add_lazy_constraints(cpx_linexprs, cpx_senses, cpx_rhss, cpx_names)
+
+    def clear_lazy_constraints(self):
+        self._cplex.linear_constraints.advanced.free_lazy_constraints()
+
 
     def sync_equivalence_cts(self, mdl):
         if self.supports_typed_indicators:
             posted_eqcts = []
             for eqct in mdl.iter_implicit_equivalence_cts():
                 if eqct._index < 0:
                     posted_eqcts.append(eqct)
@@ -1365,20 +1532,19 @@
     def _format_cplex_message(self, cpx_msg):
         if 'CPLEX' not in cpx_msg:
             cpx_msg = 'CPLEX: %s' % cpx_msg
         return cpx_msg.rstrip(' .\n')
 
     def _parse_cplex_exception_as_status(self, cpx_ex):
         cpx_ex_s = str(cpx_ex)
+        msg = cpx_ex_s
         for extype in ['CplexSolverError', 'CplexError']:
             prefix = 'cplex.exceptions.errors.{0}: '.format(extype)
             if cpx_ex_s.startswith(prefix):
                 msg = cpx_ex_s[len(prefix):]
-        else:
-            msg = cpx_ex_s
 
         cpx_code_match = self.cplex_error_re.match(msg)
         code = -1
         if cpx_code_match:
             try:
                 code = int(cpx_code_match.group(1))
             except ValueError:
@@ -1398,15 +1564,29 @@
         if cpx.variables.get_num() > 0:
             cpx.variables.set_lower_bounds(0, cpx.variables.get_lower_bounds(0))
         elif cpx.linear_constraints.get_num() > 0:
             cpx.linear_constraints.set_senses(0, cpx.linear_constraints.get_senses(0))
         else:
             pass
 
-    def solve(self, mdl, parameters=None, lex_mipstart=None):
+    def _get_priorities_list_in_decreasing_order(self):
+        # Compute list of priorities in decreasing order
+        prio_list = [self._cplex.multiobj.get_priority(oidx) for oidx in range(self._cplex.multiobj.get_num())]
+        prio_set = set(prio_list)
+        inversed_ordered_prio = sorted(list(prio_set))
+        inversed_ordered_prio.reverse()
+        return inversed_ordered_prio
+
+    def _check_multi_objective_support(self):
+        if not _is_defined_multiobjsetobj():
+            msg = 'Multi-objectives require CPLEX version 12.9 or above, this is CPLEX version: {0}'.format(
+                self._cplex.get_version())
+            self._model.fatal(msg)
+
+    def solve(self, mdl, parameters=None, lex_mipstart=None, lex_timelimits=None, lex_mipgaps=None):
         self._resync_if_needed()
 
         cpx = self._cplex
         # keep this line until RTC28217 is solved and closed !!! ----------------
         # see RTC 28217 item #18 for details
         cpx.get_problem_name()  # workaround from Ryan
 
@@ -1424,15 +1604,15 @@
         # print("--> starting CPLEX solve #", self.__solveCount)
         cpx_status_string = None
         try:
             # keep this in the protected  block...
             self._sync_var_bounds()
             self._sync_annotations(mdl)
             self.sync_equivalence_cts(mdl)
-            self._apply_sos(mdl)
+            #self._apply_sos(mdl)
 
             if mdl.clean_before_solve:
                 self.clean_before_solve()
 
             # --- mipstart block ---
             mip_starts = mdl.mip_starts
             cpx_mip_starts = cpx.MIP_starts
@@ -1443,21 +1623,53 @@
                     if not isinstance(mp, SolveSolution):  # pragma: no cover
                         mdl.fatal("mip_starts expects Solution, got: {0!r} - ignored", mp)
                     cpx_sol = self.sol_to_cpx_mipstart(mdl, mp, effort_level)
                     cpx_mip_starts.add(cpx_sol, effort_level)
             elif mip_starts:
                 self._model.warning("Lexicographic solve ignored {0} mipstarts".format(len(mip_starts)))
 
-
             # --- end of mipstart block ---
 
             linear_nonzeros = cpx.linear_constraints.get_num_nonzeros()
             nb_columns = cpx.variables.get_num()
             cpx_probtype = cpx.problem_type[cpx.get_problem_type()]
-            cpx.solve()  # returns nothing in Python
+
+
+            # # FOR TEST PURPOSE ---- TEMPORARY **************************************************************************
+            # cpx.write("/temp/cplex_model.lp", filetype="lp")
+
+            #Handle lex_timelimits list
+            if lex_timelimits is not None or lex_mipgaps is not None:
+                self._check_multi_objective_support()
+
+                # Get list of priorities in decreasing order
+                decreasing_ordered_prio = self._get_priorities_list_in_decreasing_order()
+
+                if lex_timelimits is not None and len(lex_timelimits) != len(decreasing_ordered_prio):
+                    mdl.fatal("lex_timelimits list length does not match number of priorities for multiobjective solve")
+                if lex_mipgaps is not None and len(lex_mipgaps) != len(decreasing_ordered_prio):
+                    mdl.fatal("lex_mipgaps list length does not match number of priorities for multiobjective solve")
+                paramsets = []
+                for _ in decreasing_ordered_prio:
+                    paramset = cpx.create_parameter_set()
+                    paramsets.append(paramset)
+                if lex_timelimits is not None:
+                    for paramIdx, timelimit in enumerate(lex_timelimits):
+                        paramsets[paramIdx].add(cpx_cst.CPX_PARAM_TILIM, timelimit)
+                if lex_mipgaps is not None:
+                    for paramIdx, mipgap in enumerate(lex_mipgaps):
+                        paramsets[paramIdx].add(cpx_cst.CPX_PARAM_EPGAP, mipgap)
+                # If there is a single priority level, timelimit and mipgaps are handled at the cplex_parameters level
+                paramsets = paramsets if len(paramsets) > 1 else None
+
+                cpx.solve(paramsets=paramsets)
+
+            else:
+                cpx.solve()
+
             cpx_status = cpx.solution.get_status()
             cpx_status_string = self._cplex.solution.get_status_string(cpx_status)
             is_mip = cpx._is_MIP()
 
             solve_ok = self._is_solve_status_ok(cpx_status)
             if solve_ok:
                 if is_mip:
@@ -1530,29 +1742,40 @@
         if cpx_status_string:
             mdl.error_handler.trace("CPLEX solve returns with status: {0}", (cpx_status_string,))
         return new_solution
 
     def _make_solution(self, mdl, job_solve_status):
         cpx = self._cplex
         full_obj = cpx.solution.get_objective_value()
+        if _is_defined_multiobjsetobj() and cpx.multiobj.get_num() > 1:
+            full_obj = [cpx.solution.multiobj.get_objective_value(objidx) for objidx in range(cpx.multiobj.get_num())]
         rounded_obj = mdl.round_objective_if_discrete(full_obj)
 
+        # Build list of objectives value by priority level (ie: each priority level corresponds to blended objectives
+        # with same priority)
+        full_obj_by_prio = [full_obj]
+        if _is_defined_multiobjsetobj() and cpx.multiobj.get_num() > 1:
+            decreasing_ordered_prio = self._get_priorities_list_in_decreasing_order()
+            full_obj_by_prio = [cpx.solution.multiobj.get_objval_by_priority(prio) for prio in decreasing_ordered_prio]
+        rounded_obj_by_prio = mdl.round_objective_if_discrete(full_obj_by_prio)
+
         if mdl.number_of_variables > 0:
             all_var_indices = [dvar.get_index() for dvar in mdl.iter_variables()]
             # do not query values on an empty model...
             all_var_values = cpx.solution.get_values(all_var_indices)
             var_value_map = dict(izip(mdl.iter_variables(), all_var_values))
         else:
             var_value_map = {}
 
         solve_details = self._last_solve_details
         assert solve_details is not None
         solution = SolveSolution.make_engine_solution(model=mdl,
                                                       var_value_map=var_value_map,
                                                       obj=rounded_obj,
+                                                      blended_obj_by_priority=rounded_obj_by_prio,
                                                       solved_by=self.get_name(),
                                                       solve_details=solve_details,
                                                       job_solve_status=job_solve_status)
         return solution
 
     def _run_cpx_op_with_details(self, cpx_fn, *args):
         cpx = self._cplex
@@ -1564,15 +1787,16 @@
         linear_nonzeros = -1
         nb_columns = 0
         cpx_probtype = None
         # noinspection PyPep8
         try:
             linear_nonzeros = cpx.linear_constraints.get_num_nonzeros()
             nb_columns = cpx.variables.get_num()
-            cpx_fn(*args)
+            if args:
+                cpx_fn(*args)
             cpx_status = cpx.solution.get_status()
             cpx_probtype = cpx.problem_type[cpx.get_problem_type()]
             cpx_status_string = self._cplex.solution.get_status_string(cpx_status)
             solve_ok = self._is_relaxed_status_ok(cpx_status)
             if solve_ok:
                 if cpx._is_MIP():
                     cpx_miprelgap = cpx.solution.MIP.get_mip_relative_gap()
@@ -1706,14 +1930,15 @@
         with _CplexOverwriteParametersCtx(self_cplex, feasopt_override_params) as cpx:
             # at this stage, we have a list of groups
             # each group is itself a list
             # the first item is a number, the preference
             # the second item is a list of constraint indices.
             self._last_solve_details = self._run_cpx_op_with_details(cpx.feasopt, *cpx_relax_groups)
 
+
         # feasopt state is restored by now
         cpx_solution = self_cplex.solution
         feas_status = cpx_solution.get_status()
         if self._is_relaxed_status_ok(feas_status):
             infeas_map = self._decode_infeasibilities(self_cplex, mdl, cpx_relax_groups)
 
             # all_ct_indices = []
@@ -1973,15 +2198,19 @@
             return parameter.default_value
 
     def get_solve_status(self):  # pragma: no cover
         from docplex.util.status import JobSolveStatus
         # In this function we try to do the exact same mappings as the IloCplex C++ and Java classes.
         # However, this is not always possible since the C++ and Java implementations are not consistent
         # and sometimes they are even in error (see RTC-21923).
+
         cpx_status = self._cplex.solution.get_status()
+        # what status for relaxed solutions??
+        relaxed_solution_status = JobSolveStatus.INFEASIBLE_SOLUTION
+        #
         if cpx_status in {cpx_cst.CPXMIP_ABORT_FEAS,
                           cpx_cst.CPXMIP_DETTIME_LIM_FEAS,
                           cpx_cst.CPXMIP_FAIL_FEAS,
                           cpx_cst.CPXMIP_FAIL_FEAS_NO_TREE,
                           cpx_cst.CPXMIP_MEM_LIM_FEAS,
                           cpx_cst.CPXMIP_NODE_LIM_FEAS,
                           cpx_cst.CPXMIP_TIME_LIM_FEAS
@@ -1995,61 +2224,80 @@
                             cpx_cst.CPXMIP_MEM_LIM_INFEAS,
                             cpx_cst.CPXMIP_NODE_LIM_INFEAS,
                             cpx_cst.CPXMIP_TIME_LIM_INFEAS
                             }:
             # Hit a limit without a feasible solution: We don't know anything about the solution.
             return JobSolveStatus.UNKNOWN
         elif cpx_status in {cpx_cst.CPXMIP_OPTIMAL,
-                            cpx_cst.CPXMIP_OPTIMAL_TOL}:
+                            cpx_cst.CPXMIP_OPTIMAL_TOL,
+                            DEFAULT_CPX_STAT_MULTIOBJ_OPTIMAL}:
             return JobSolveStatus.OPTIMAL_SOLUTION
         elif cpx_status is cpx_cst.CPXMIP_SOL_LIM:
             #  return hasSolution(env, lp) ? JobSolveStatus.FEASIBLE_SOLUTION : JobSolveStatus.UNKNOWN;
             return JobSolveStatus.FEASIBLE_SOLUTION
-        elif cpx_status is cpx_cst.CPXMIP_INForUNBD:
+        elif cpx_status in {cpx_cst.CPXMIP_INForUNBD,
+                            DEFAULT_CPX_STAT_MULTIOBJ_INForUNBD}:
             return JobSolveStatus.INFEASIBLE_OR_UNBOUNDED_SOLUTION
         elif cpx_status in {cpx_cst.CPXMIP_UNBOUNDED,
-                            cpx_cst.CPXMIP_ABORT_RELAXATION_UNBOUNDED}:
+                            cpx_cst.CPXMIP_ABORT_RELAXATION_UNBOUNDED,
+                            DEFAULT_CPX_STAT_MULTIOBJ_UNBOUNDED}:
             return JobSolveStatus.UNBOUNDED_SOLUTION
-        elif cpx_status is cpx_cst.CPXMIP_INFEASIBLE:  # proven infeasible
+        elif cpx_status in {cpx_cst.CPXMIP_INFEASIBLE,
+                            DEFAULT_CPX_STAT_MULTIOBJ_INFEASIBLE}:  # proven infeasible
             return JobSolveStatus.INFEASIBLE_SOLUTION
-        elif cpx_status is cpx_cst.CPXMIP_OPTIMAL_INFEAS:  # optimal with unscaled infeasibilities
+        elif cpx_status == cpx_cst.CPXMIP_OPTIMAL_INFEAS:  # optimal with unscaled infeasibilities
             # DANIEL: What exactly do we return here? There is an optimal solution but that solution is
             # infeasible after unscaling.
             return JobSolveStatus.OPTIMAL_SOLUTION
 
         # feasopt status values
         elif cpx_status in frozenset({
             cpx_cst.CPXMIP_ABORT_RELAXED,  # relaxed solution is available and can be queried
             cpx_cst.CPXMIP_FEASIBLE  # problem feasible after phase I and solution available
         }):
             return JobSolveStatus.FEASIBLE_SOLUTION
+        ## -----------------
+        ## relaxation (feasopt) there is a relaxed (but infeasible) solution
+        ## for now we choose to return INFEASIBLE_SOLUTION
+        ##
         elif cpx_status in {cpx_cst.CPXMIP_FEASIBLE_RELAXED_INF,
                             cpx_cst.CPXMIP_FEASIBLE_RELAXED_QUAD,
                             cpx_cst.CPXMIP_FEASIBLE_RELAXED_SUM
                             }:
-            return JobSolveStatus.UNKNOWN
+            return relaxed_solution_status
         elif cpx_status in {cpx_cst.CPXMIP_OPTIMAL_RELAXED_INF,
                             cpx_cst.CPXMIP_OPTIMAL_RELAXED_QUAD,
                             cpx_cst.CPXMIP_OPTIMAL_RELAXED_SUM
                             }:
-            return JobSolveStatus.INFEASIBLE_SOLUTION
+            return relaxed_solution_status
+        elif cpx_status in {cpx_cst.CPX_STAT_FEASIBLE_RELAXED_INF,
+                            cpx_cst.CPX_STAT_FEASIBLE_RELAXED_QUAD,
+                            cpx_cst.CPX_STAT_FEASIBLE_RELAXED_SUM,
+                            }:
+            return relaxed_solution_status
+        elif cpx_status in {cpx_cst.CPX_STAT_OPTIMAL_RELAXED_INF,
+                            cpx_cst.CPX_STAT_OPTIMAL_RELAXED_QUAD,
+                            cpx_cst.CPX_STAT_OPTIMAL_RELAXED_SUM}:
+            return relaxed_solution_status
+
+        ## -------------------
 
         # populate status values
         elif cpx_status in {cpx_cst.CPXMIP_OPTIMAL_POPULATED
                             # ,cpx_cst.CPXMIP_OPTIMAL_POPULATED_TO
                             }:
             return JobSolveStatus.OPTIMAL_SOLUTION
-        elif cpx_status is cpx_cst.CPXMIP_POPULATESOL_LIM:
+        elif cpx_status == cpx_cst.CPXMIP_POPULATESOL_LIM:
             # minimal value for CPX_PARAM_POPULATE_LIM is 1! So there must be a solution
             return JobSolveStatus.FEASIBLE_SOLUTION
 
-        elif cpx_status is cpx_cst.CPX_STAT_OPTIMAL:
+        elif cpx_status == cpx_cst.CPX_STAT_OPTIMAL:
             return JobSolveStatus.OPTIMAL_SOLUTION
 
-        elif cpx_status is cpx_cst.CPX_STAT_INFEASIBLE:
+        elif cpx_status == cpx_cst.CPX_STAT_INFEASIBLE:
             return JobSolveStatus.INFEASIBLE_SOLUTION
 
         # cpx_cst.CPX_STAT_ABORT_USER:
         # cpx_cst.CPX_STAT_ABORT_DETTIME_LIM:
         # cpx_cst.CPX_STAT_ABORT_DUAL_OBJ_LIM:
         # cpx_cst.CPX_STAT_ABORT_IT_LIM:
         # cpx_cst.CPX_STAT_ABORT_PRIM_OBJ_LIM:
@@ -2073,15 +2321,15 @@
         #   default: return JobSolveStatus.UNKNOWN;
         #   }
         #
         # cpx_cst.CPX_STAT_FIRSTORDER:
         #   // See IloCplexI::CplexToAlgorithmStatus()
         #   return primalFeasible(env, lp) ? JobSolveStatus.FEASIBLE_SOLUTION : JobSolveStatus.UNKNOWN;
 
-        elif cpx_status is cpx_cst.CPX_STAT_CONFLICT_ABORT_CONTRADICTION:
+        elif cpx_status == cpx_cst.CPX_STAT_CONFLICT_ABORT_CONTRADICTION:
             # Numerical trouble in conflict refiner.
             #  DANIEL: C++ and Java both return Error here although a conflict is
             #          available (but nor proven to be minimal). This looks like a bug
             #          since no exception is thrown there. In IloSolveStatus we don't
             #          have ERROR, so we return UNKNOWN instead. This is fine for now
             #          since we do not support the conflict refiner anyway.
             #
@@ -2102,53 +2350,51 @@
             #  *         This is particularly erroneous if no exception gets thrown.
             #  *         See RTC-21923.
             #  *         In IloSolveStatus we don't have ERROR, so we return UNKNOWN instead.
             #  *         This should not be a problem since right now we don't support the
             #  *         conflict refiner anyway.
             #  */
             return JobSolveStatus.UNKNOWN
-        elif cpx_status is cpx_cst.CPX_STAT_CONFLICT_FEASIBLE:
+        elif cpx_status == cpx_cst.CPX_STAT_CONFLICT_FEASIBLE:
             return JobSolveStatus.FEASIBLE_SOLUTION
-        elif cpx_status is cpx_cst.CPX_STAT_CONFLICT_MINIMAL:
+        elif cpx_status == cpx_cst.CPX_STAT_CONFLICT_MINIMAL:
             return JobSolveStatus.INFEASIBLE_SOLUTION
-        elif cpx_status in {cpx_cst.CPX_STAT_FEASIBLE_RELAXED_INF,
-                            cpx_cst.CPX_STAT_FEASIBLE_RELAXED_QUAD,
-                            cpx_cst.CPX_STAT_FEASIBLE_RELAXED_SUM,
-                            }:
-            return JobSolveStatus.UNKNOWN
 
-        elif cpx_status is cpx_cst.CPX_STAT_FEASIBLE:
+        elif cpx_status == cpx_cst.CPX_STAT_FEASIBLE:
             return JobSolveStatus.FEASIBLE_SOLUTION
-        elif cpx_status in {cpx_cst.CPX_STAT_OPTIMAL_RELAXED_INF,
-                            cpx_cst.CPX_STAT_OPTIMAL_RELAXED_QUAD,
-                            cpx_cst.CPX_STAT_OPTIMAL_RELAXED_SUM}:
-            return JobSolveStatus.INFEASIBLE_SOLUTION
 
-        elif cpx_status is cpx_cst.CPX_STAT_NUM_BEST:
+        elif cpx_status == cpx_cst.CPX_STAT_NUM_BEST:
             #  Solution available but not proved optimal (due to numeric difficulties)
             # assert(hasSolution(env, lp));
             return JobSolveStatus.UNKNOWN
 
-        elif cpx_status is cpx_cst.CPX_STAT_OPTIMAL_INFEAS:  # infeasibilities after unscaling
+        elif cpx_status == cpx_cst.CPX_STAT_OPTIMAL_INFEAS:  # infeasibilities after unscaling
             # assert(hasSolution(env, lp));
             return JobSolveStatus.OPTIMAL_SOLUTION
 
-        elif cpx_status is cpx_cst.CPX_STAT_INForUNBD:  # Infeasible or unbounded in presolve.
+        elif cpx_status == cpx_cst.CPX_STAT_INForUNBD:  # Infeasible or unbounded in presolve.
             return JobSolveStatus.INFEASIBLE_OR_UNBOUNDED_SOLUTION
-        elif cpx_status is cpx_cst.CPX_STAT_OPTIMAL_FACE_UNBOUNDED:
+        elif cpx_status == cpx_cst.CPX_STAT_OPTIMAL_FACE_UNBOUNDED:
             #    unbounded optimal face (barrier only)
             # // CPX_STAT_OPTIMAL_FACE_UNBOUNDED is explicitly an error in Java and implicitly (fallthrough)
             # // an error in C++. So it should be fine to produce an error here as well.
             # // In IloSolveStatus we don't have ERROR, so we return UNKNOWN instead.
             # // In case of ERROR we should have seen a non-zero status anyway and the
             # // user should not care too much about the returned status.
             return JobSolveStatus.UNKNOWN
-        elif cpx_status is cpx_cst.CPX_STAT_UNBOUNDED:
+        elif cpx_status == cpx_cst.CPX_STAT_UNBOUNDED:
             # definitely unbounded
             return JobSolveStatus.UNBOUNDED_SOLUTION
+        elif cpx_status == DEFAULT_CPX_STAT_MULTIOBJ_NON_OPTIMAL:
+            # Solution available but not proved optimal
+            return JobSolveStatus.FEASIBLE_SOLUTION
+        elif cpx_status == DEFAULT_CPX_STAT_MULTIOBJ_STOPPED:
+            # The solve of a multi-objective problem was interrupted (a global work limit was hit or solution process
+            # was aborted)
+            return JobSolveStatus.UNKNOWN
         else:
             return JobSolveStatus.UNBOUNDED_SOLUTION
 
     def _resync_if_needed(self):
         if self._resync is _CplexSyncMode.OutOfSync:
             # print("-- resync cplex from model...")
             # send whole model to engine.
```

### Comparing `docplex-2.8.125/docplex/mp/docloud_connector.py` & `docplex-2.9.141/docplex/mp/docloud_connector.py`

 * *Files identical despite different names*

### Comparing `docplex-2.8.125/docplex/mp/docloud_engine.py` & `docplex-2.9.141/docplex/mp/docloud_engine.py`

 * *Files 1% similar despite different names*

```diff
@@ -233,19 +233,14 @@
         # noinspection PyPep8
         self.debug_dump = docloud_context.debug_dump
         self.debug_dump_dir = docloud_context.debug_dump_dir
 
 
     def _new_printer(self, ctx):
         return self._printer
-        # printer = ModelPrinterFactory.new_printer(self._exchange_format, full_obj=True)
-        # if ctx.solver.docloud.mangle_names:
-        #     print('LP names will be mangled')
-        #     printer.hide_use_names = True
-        # return printer
 
     def supports_logical_constraints(self):
         # <-> is supposed to be supported in LP?
         return True, None
 
     @property
     def name(self):
@@ -566,15 +561,15 @@
 
         return result
 
     def _make_attachment_name(self, basename, extension):
         return make_attachment_name(basename + extension)
 
     # noinspection PyProtectedMember
-    def solve(self, mdl, parameters=None, lex_mipstart=None):
+    def solve(self, mdl, parameters=None, lex_mipstart=None, lex_timelimits=None, lex_mipgaps=None):
         # Before submitting the job, we will build the list of attachments
         # parameters are CPLEX parameters
         attachments = []
 
 
         # make sure model is the first attachment: that will be the name of the job on the console
         job_name = normalize_basename("python_%s" % mdl.name)
@@ -680,14 +675,15 @@
                         # more than one is an issue.
                         if count_nonmatching_cloud_vars:
                             mdl.info("Cannot find matching variable, cloud name is {0!s}", cloud_name)
                         count_nonmatching_cloud_vars += 1
 
         sol = SolveSolution.make_engine_solution(model=mdl,
                                                  obj=docloud_obj,
+                                                 blended_obj_by_priority=[docloud_obj],
                                                  var_value_map=docloud_values_by_vars,
                                                  solved_by=self.get_name(),
                                                  solve_details=self._solve_details,
                                                  job_solve_status=self.get_solve_status())
 
         # attributes
         docloud_ct_duals, docloud_ct_slacks = solution_handler.constraint_results()
```

### Comparing `docplex-2.8.125/docplex/mp/engine.py` & `docplex-2.9.141/docplex/mp/engine.py`

 * *Files 1% similar despite different names*

```diff
@@ -32,15 +32,15 @@
         """
         Connects progress listeners
         :param listeners:
         :return:
         """
         raise NotImplementedError  # pragma: no cover
 
-    def solve(self, mdl, parameters, lex_mipstart=None, lex_timelimits=None):
+    def solve(self, mdl, parameters, lex_mipstart=None, lex_timelimits=None, lex_mipgaps=None):
         ''' Redefine this method for the real solve.
             Returns a solution object or None.
         '''
         raise NotImplementedError  # pragma: no cover
 
     def solve_relaxed(self, mdl, prio_name, relaxable_groups, relax_mode, parameters=None):
         """
@@ -109,15 +109,15 @@
 
     def clean_before_solve(self):
         raise NotImplementedError  # pragma: no cover
 
     def supports_logical_constraints(self):
         raise NotImplementedError  # pragma: no cover
 
-    def solved_as_lp(self):
+    def solved_as_mip(self):
         return False
 
 
 # noinspection PyAbstractClass
 class IEngine(ISolver):
     """ interface for all engine facades
     """
@@ -224,14 +224,28 @@
 
     def check_var_indices(self, dvars):
         raise NotImplementedError  # pragma: no cover
 
     def check_constraint_indices(self, cts):
         raise NotImplementedError  # pragma: no cover
 
+    def create_sos(self, sos):
+        raise NotImplementedError  # pragma: no cover
+
+    def clear_all_sos(self):
+        raise NotImplementedError  # pragma: no cover
+
+    def add_lazy_constraints(self, lazy_cts):
+        raise NotImplementedError  # pragma: no cover
+
+    def clear_lazy_constraints(self):
+        raise NotImplementedError  # pragma: no cover
+
+    def get_basis(self, mdl):
+        raise NotImplementedError  # pragma: no cover
 
 # noinspection PyAbstractClass
 class DummyEngine(IEngine):
     def create_range_constraint(self, rangect):
         return -1  # pragma: no cover
 
     def create_indicator_constraint(self, ind):
@@ -272,14 +286,17 @@
 
     def set_var_ub(self, var, ub):
         pass
 
     def rename_var(self, var, new_name):
         pass  # nothing to do, except in cplex...
 
+    def rename_linear_constraint(selfself, linct, new_name):
+        pass # nothing to do, except in cplex...
+
     def set_var_type(self, var, new_type):
         pass  # nothing to do, except in cplex...
 
     def create_linear_constraint(self, binaryct):
         return -1  # pragma: no cover
 
     def create_block_linear_constraints(self, ct_seq):
@@ -320,15 +337,15 @@
 
     def disconnect_progress_listeners(self, listeners):
         pass  # pragma: no cover
 
     def can_solve(self):
         return False  # pragma: no cover
 
-    def solve(self, mdl, parameters, lex_mipstart=None, lex_timelimits=None):
+    def solve(self, mdl, parameters, lex_mipstart=None, lex_timelimits=None, lex_mipgaps=None):
         return None  # pragma: no cover
 
     def get_solve_status(self):
         return JobSolveStatus.UNKNOWN  # pragma: no cover
 
     def solve_relaxed(self, mdl, prio_name, relaxable_groups, relax_mode, parameters=None):
         raise None  # pragma: no cover
@@ -364,14 +381,29 @@
 
     def check_var_indices(self, dvars):
         pass
 
     def check_constraint_indices(self, cts):
         pass
 
+    def create_sos(self, sos):
+        pass
+
+    def clear_all_sos(self):
+        pass
+
+    def add_lazy_constraints(self, lazy_cts):
+        pass
+
+    def clear_lazy_constraints(self):
+        pass
+
+    def get_basis(self, mdl):
+        return None, None
+
 
 # noinspection PyAbstractClass,PyUnusedLocal
 class IndexerEngine(DummyEngine):
     """
     An abstract engine facade which generates unique indices for variables, constraints
     """
 
@@ -495,15 +527,15 @@
 
     def get_ct_index(self, ct):
         return ct.index
 
     def can_solve(self):
         return False
 
-    def solve(self, mdl, parameters, lex_mipstart=None, lex_timelimits=None):
+    def solve(self, mdl, parameters, lex_mipstart=None, lex_timelimits=None, lex_mipgaps=None):
         """
         This solver cannot solve. never ever.
         """
         mdl.fatal("No CPLEX DLL and no DOcplexcloud credentials: model cannot be solved!")
         return None
 
     def solve_relaxed(self, mdl, prio_name, relaxable_groups, relax_mode, parameters=None):
@@ -549,15 +581,15 @@
     @property
     def name(self):
         return self.get_name()
 
     def get_var_zero_solution(self, dvar):
         return max(0, dvar.lb)
 
-    def solve(self, mdl, parameters, lex_mipstart=None, lex_timelimits=None):
+    def solve(self, mdl, parameters, lex_mipstart=None, lex_timelimits=None, lex_mipgaps=None):
         # remember last solved params
         self._last_solved_parameters = parameters.clone() if parameters is not None else None
         self.show_parameters(parameters)
         return self.make_zero_solution(mdl)
 
     def get_solutions(self, args):
         if not args:
@@ -592,15 +624,15 @@
     # but always fail, and returns None.
     def __init__(self, mdl, **kwargs):
         IndexerEngine.__init__(self)  # pragma: no cover
 
     def get_name(self):
         return "no_solution_solve"  # pragma: no cover
 
-    def solve(self, mdl, parameters, lex_mipstart=None, lex_timelimits=None):
+    def solve(self, mdl, parameters, lex_mipstart=None, lex_timelimits=None, lex_mipgaps=None):
         # solve fails equivalent to returning None
         return None  # pragma: no cover
 
     def can_solve(self):
         return True  # pragma: no cover
 
     def solve_relaxed(self, mdl, prio_name, relaxable_groups, relax_mode, parameters=None):
@@ -624,15 +656,15 @@
 
     def __init__(self, mdl, **kwargs):
         IndexerEngine.__init__(self)  # pragma: no cover
 
     def name(self):
         return "exception"  # pragma: no cover
 
-    def solve(self, mdl, parameters, lex_mipstart=None, lex_timelimits=None):
+    def solve(self, mdl, parameters, lex_mipstart=None, lex_timelimits=None, lex_mipgaps=None):
         # solve fails equivalent to returning None
         self.terminate()
         return None  # pragma: no cover
 
     def can_solve(self):
         return True  # pragma: no cover
 
@@ -661,15 +693,15 @@
 
     def __init__(self, mdl, **kwargs):
         IndexerEngine.__init__(self)  # pragma: no cover
 
     def get_name(self):
         return "raise"  # pragma: no cover
 
-    def solve(self, mdl, parameters, lex_mipstart=None, lex_timelimits=None):
+    def solve(self, mdl, parameters, lex_mipstart=None, lex_timelimits=None, lex_mipgaps=None):
         # solve fails equivalent to returning None
         self._simulate_error()
         return None  # pragma: no cover
 
     def can_solve(self):
         return True  # pragma: no cover
```

### Comparing `docplex-2.8.125/docplex/mp/engine_factory.py` & `docplex-2.9.141/docplex/mp/engine_factory.py`

 * *Files identical despite different names*

### Comparing `docplex-2.8.125/docplex/mp/environment.py` & `docplex-2.9.141/docplex/mp/environment.py`

 * *Files identical despite different names*

### Comparing `docplex-2.8.125/docplex/mp/error_handler.py` & `docplex-2.9.141/docplex/mp/error_handler.py`

 * *Files identical despite different names*

### Comparing `docplex-2.8.125/docplex/mp/functional.py` & `docplex-2.9.141/docplex/mp/functional.py`

 * *Files 4% similar despite different names*

```diff
@@ -121,26 +121,23 @@
         if not self._resolved:
             self._resolve()
             self._resolved = True
 
     def _is_resolved(self):
         return self._resolved and self._f_var is not None
 
+    def name_functional_var_name(self, fvar, fvar_meta_format="_%s%d"):
+        fname = fvar_meta_format % (self.function_symbol, fvar.index)
+        fvar.set_name(fname)
+
     def _create_functional_var(self, named=True):
+        fvar = self._new_generated_free_continuous_var(name=None)
         if named:
-            # add a unique counter suffix cf. RTC
-            unique_counter = self._model._new_unique_counter()
-            if unique_counter == 0:
-                # the first time, we use the the raw name, else we suffix #<unique>
-                fname = self.to_string()
-            else:
-                fname = "%s#%d" % (self.to_string(), unique_counter)
-        else:
-            fname = None
-        return self._new_generated_free_continuous_var(name=fname)
+            self.name_functional_var_name(fvar)
+        return fvar
 
     @property
     def functional_var(self):
         return self._get_resolved_f_var()
 
     as_var = functional_var
 
@@ -238,28 +235,26 @@
 class AbsExpr(FunctionalExpr):
     def copy(self, target_model, var_mapping):
         copied_arg_expr = self._argument_expr.copy(target_model, var_mapping)
         return AbsExpr(model=target_model, argument_expr=copied_arg_expr)
 
     def __init__(self, model, argument_expr):
         FunctionalExpr.__init__(self, model, argument_expr)
-        #self._ensure_resolved_f_var()
 
     def _get_function_symbol(self):
         return "abs"
 
     def clone(self):
         return AbsExpr(self.model, self._argument_expr)
 
     # noinspection PyArgumentEqualDefault,PyArgumentEqualDefault
     def _resolve(self):
         self_f_var = self._f_var
         assert self_f_var
-        m = self.model
-        abs_index = m._new_unique_counter()
+        abs_index = self_f_var.index
         abs_names = ["_abs_pp_%d" % abs_index, "_abs_np_%d" % abs_index] if use_debug_names else [None, None]
         # 1. allocate two variables in one pass.
         positive_var = self._new_generated_continuous_var(lb=0, name=abs_names[0])
         negative_var = self._new_generated_continuous_var(lb=0, name=abs_names[1])
 
         # F(x) = p + n
         ct1 = (self_f_var == positive_var + negative_var)
@@ -352,15 +347,14 @@
     This expression can be used in all arithmetic operations.
     After a solve, the value of this expression is equal to the minimum of the values
     of its argument expressions.
     """
 
     def __init__(self, model, exprs, name=None):
         _SequenceExpr.__init__(self, model, exprs, name)
-        #self._ensure_resolved_f_var()
 
     def _get_function_symbol(self):
         return "min"
 
     def __repr__(self):
         str_args = self._get_args_string()
         return "docplex.mp.MinExpr({0!s})".format(str_args)
@@ -400,15 +394,14 @@
     This expression can be used in all arithmetic operations.
     After a solve, the value of this expression is equal to the minimum of the values
     of its argument expressions.
     """
 
     def __init__(self, model, exprs, name=None):
         _SequenceExpr.__init__(self, model, exprs, name)
-        #self._ensure_resolved_f_var()
 
     def _get_function_symbol(self):
         return "max"
 
     def __repr__(self):
         str_args = self._get_args_string()
         return "docplex.mp.MaxExpr({0!s})".format(str_args)
@@ -436,31 +429,26 @@
 
     def compute_solution_value(self, s):
         return max(expr._get_solution_value(s) for expr in self._exprs)
 
 
 class _LogicalSequenceExpr(_SequenceExpr):
 
-    def _create_functional_var(self):
+    def _create_functional_var(self, named=True):
         # the resulting variable is a binary variable...
-        unique_counter = self._model._new_unique_counter()
-        if unique_counter == 0:
-            # the first time, we use the the raw name, else we suffix #<unique>
-            fname = self.to_string()
-        else:
-            fname = "%s#%d" % (self.to_string(), unique_counter)
-        return self._new_generated_binary_var(name=fname)
+        bvar = self._new_generated_binary_var(name=None)
+        self.name_functional_var_name(bvar)
+        return bvar
 
     def __init__(self, model, exprs, name=None):
         _IAdvancedExpr.__init__(self, model, name)
         assert is_iterable(exprs) or is_iterator(exprs)
         self._exprs = exprs
         # never allocate vars: arguments --are-- binary variables.
         self._xvars = exprs
-        #self._ensure_resolved_f_var()
 
     def is_discrete(self):
         return True
 
     precision = 1e-5
 
 
@@ -528,16 +516,19 @@
                 self.name = '{0}_{1!s}'.format(self._pwl_func.name, self._usage_counter)
             else:
                 self.name = self._pwl_func.name
         if resolve:
             self._ensure_resolved()
 
     def _get_function_symbol(self):
+        # this method determines the name of the generated variable
+        # as usual it starts with "_" to mark this is a generated variable.
         pwl_name = self._pwl_func.get_name()
-        return pwl_name or '_pwl{0}'.format(self._usage_counter)
+        # TODO: what if pwl_name is not LP-compliant??
+        return "pwl" if not pwl_name else "pwl_%s#" % pwl_name
 
     def _get_solution_value(self, s=None):
         raw = self._f_var._get_solution_value(s)
         return self._round_if_discrete(raw)
 
     def iter_variables(self):
         for v in self._argument_expr.iter_variables():
@@ -545,15 +536,14 @@
         yield self._get_resolved_f_var()
 
     def _resolve(self):
         mdl = self._model
         pwl_constraint = mdl._lfactory.new_pwl_constraint(self, self.get_name())
         mdl._add_pwl_constraint_internal(pwl_constraint)
 
-
     @property
     def pwl_func(self):
         return self._pwl_func
 
     @property
     def usage_counter(self):
         return self._usage_counter
```

### Comparing `docplex-2.8.125/docplex/mp/kpi.py` & `docplex-2.9.141/docplex/mp/kpi.py`

 * *Files 18% similar despite different names*

```diff
@@ -10,15 +10,18 @@
 from docplex.mp.utils import is_number, is_string, is_function, str_holo
 
 
 class KPI(object):
     """ Abstract class for key performance indicators (KPIs).
 
     Each KPI has a unique name. A KPI is attached to a model instance and can compute a numerical value,
-    using the :func:`compute` method.
+    using the :func:`compute` method. The `compute` method takes an optional solution argument;
+    if passed a valid SolveSolution object, this solution is used to evaluate the KPI, else compute()
+    will attempt to access th emodel's solution. If the model has no attached solution, then an exception
+    is raised by `compute`.
 
     Some KPIs require a valid solution of the model, while others do not. Use :func:`requires_solution` to
     check whether a given KPI requires a solution.
     """
 
     def __init__(self):
         pass
@@ -94,15 +97,17 @@
         pass
 
 
 class DecisionKPI(KPI):
     """ Specialized class of Key Performance Indicator, based on expressions.
 
     This subclass is built from a decision variable or a linear expression.
-    The :func:`compute` method returns the solution value after a successful solve.
+    The :func:`compute` method evaluate the value of the KPI in a solution. This solution can either be passed
+    to the `compute` method, or using th emodel's solution. In the latter case, the model must have been solved
+    with a solution.
 
     """
     def __init__(self, kpi_op, name=None):
         KPI.__init__(self)
         if is_number(kpi_op):
             self._expr = self.get_model().linear_expr(arg=kpi_op)
             self._name = name
@@ -130,21 +135,30 @@
 
     name = property(get_name, set_name)
 
     def get_model(self):
         return self._expr.model
 
     def compute(self, s=None):
-        """ Redefinition of the abstract `compute()` method.
+        """ Redefinition of the abstract `compute(s=None)` method.
 
         Returns:
-            float: The value of the decision expression at the solution.
+            float: The value of the decision expression in the solution.
+
+        Note:
+            Evaluating a KPI requires a solution object. This solution can either be passed explicitly
+            in the `s` argument, otherwise the model solution is used. In the latter case, th emodel must
+            have been solved with a solution, otherwise an exception is raised.
 
         Raises:
-            Evaluating this KPI raises an exception if the underlying model has not been solved successfully.
+            Evaluating a KPI raises an exception if no `s` solution has been passed
+            and the underlying model has not been solved with a solution.
+
+        See Also:
+            :class:`docplex.mp.solution.SolveSolution`
         """
         return self._expr._get_solution_value(s)
 
     def requires_solution(self):
         return True
 
     def to_expr(self):
```

### Comparing `docplex-2.8.125/docplex/mp/linear.py` & `docplex-2.9.141/docplex/mp/linear.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,25 +11,23 @@
 
 from docplex.mp.constants import ComparisonType, UpdateEvent, CplexScope
 from docplex.mp.compat23 import unitext
 from docplex.mp.basic import ModelingObject, Expr, ModelingObjectBase, _SubscriptionMixin, _BendersAnnotatedMixin
 from docplex.mp.operand import LinearOperand
 from docplex.mp.vartype import BinaryVarType, IntegerVarType, ContinuousVarType
 from docplex.mp.utils import *
+from docplex.mp.format import LP_format
 from docplex.mp.sttck import StaticTypeChecker
 
 
 class DOCplexQuadraticArithException(Exception):
     # INTERNAL
     pass
 
 
-# from docplex.mp.xcounter import ExprCounter
-
-
 class Var(ModelingObject, LinearOperand, _BendersAnnotatedMixin):
     """Var()
 
     This class models decision variables.
     Decision variables are instantiated by :class:`docplex.mp.model.Model` methods such as :func:`docplex.mp.model.Model.var`.
 
     """
@@ -86,19 +84,21 @@
     def contains_var(self, dvar):
         return self is dvar
 
     def accept_initial_value(self, candidate_value):
         return self.vartype.accept_domain_value(candidate_value, lb=self._lb, ub=self._ub)
 
     def check_name(self, new_name):
-        ModelingObject.check_name(self, new_name)
+        #ModelingObject.check_name(self, new_name)
         if not is_string(new_name) or not new_name:
-            self.fatal("Variable name accepts only non-empty strings, got: {0!s}", new_name)
+            self.fatal("Variable name accepts only non-empty strings, {0!r} was passed", new_name)
         elif new_name.find(' ') >= 0:
             self.warning("Variable name contains blank space, var: {0!s}, name: \'{1!s}\'", self, new_name)
+        elif not LP_format.is_lp_compliant(new_name):
+            self.warning("Candidate variable name is not LP-compliant, old name was: {0}, new name: \'{1!s}\' (will be changed to x<nn>)", self.name, new_name)
 
     def __hash__(self):
         return self._index
 
     def to_linear_expr(self):
         # INTERNAL
         return LinearExpr(model=self._model, e=self, safe=True, transient=True)
@@ -280,17 +280,17 @@
 
         :return:
             a Python object, possibly None.
         """
         self_container = self.get_container()
         return self_container.get_var_key(self) if self_container else None
 
-    def __ne__(self, other):
-        # INTERNAL: For now, not supported
-        self.model.unsupported_neq_error(self, other)
+    # def __ne__(self, other):
+    #     # INTERNAL: For now, not supported
+    #     self.model.unsupported_neq_error(self, other)
 
     def __mul__(self, e):
         return self.times(e)
 
     def times(self, e):
         if is_number(e):
             if e:
@@ -477,25 +477,28 @@
         Returns:
             string: A string representation of the variable.
 
         """
         return self.to_string()
 
     def to_string(self):
-        str_name = self.get_name() or ('_x%d' % (self.unchecked_index + 1))
+        str_name = self.get_name() or ("x%d" % (self.unchecked_index + 1))
         return str_name
 
     def print_name(self):
         # INTERNAL
-        return self._name or self._model._var_scope.new_obj_symbol(self)
+        return self.lp_name
+
+    @property
+    def lp_name(self):
+        return self._name or "x%s" % (self.index+1)
 
     def _must_print_lb(self):
         self_vartype = self._vartype
-        return self_vartype.get_cplex_typecode() not in 'SN'\
-               and self._lb == self_vartype.get_default_lb()
+        return self_vartype.get_cplex_typecode() not in 'SN' and self._lb == self_vartype.get_default_lb()
 
     def __repr__(self):
         self_vartype, self_lb, self_ub = self._vartype, self._lb, self._ub
         # print lb for semi-xx
         if self._must_print_lb():
             repr_lb = ''
         else:
@@ -526,14 +529,39 @@
         See Also:
 
             :func:`docplex.mp.model.Model.reduced_costs`
         """
         return self._model._reduced_cost1(self)
 
     @property
+    def basis_status(self):
+        """
+        This property returns the basis status of the variable, if any.
+        The variable must be continuous, otherwise an exception is raised.
+
+        Returns:
+            An enumerated value from the enumerated type `docplex.constants.BasisStatus`.
+            The integer value of this enum is equal to Cplex's basis status value;
+            for example, BasisStatus.Basic has value 1, BasisStatus.AtLower has value 0, etc...
+
+        Note:
+            for the model to hold basis information, the model must have been solved as a LP problem.
+            In some cases, a model which failed to solve may still have a basis available. Use
+            `Model.has_basis()` to check whether the model has basis information or not.
+
+        See Also:
+            :func:`docplex.mp.model.Model.has_basis`
+
+
+        """
+        if not self.is_continuous():
+            self.fatal("Basis status is for continuous variables, {0!s} has type {1!s}", self, self.vartype.short_name)
+        return self._model._var_basis_status1(self)
+
+    @property
     def benders_annotation(self):
         """
         This property is used to get or set the Benders annotation of a variable.
         The value of the annotation must be a positive integer
 
         """
         return self.get_benders_annotation()
@@ -550,14 +578,39 @@
         """
         for ct in self._model.iter_constraints():
             for ctv in ct.iter_variables():
                 if ctv is self:
                     yield ct
                     break
 
+    def equals(self, other):
+        """
+        This method is used to test equality to an expression.
+        Because of the overloading of operator `==` through the redefinition of
+        the `__eq__` method, you cannot use `==` to test for equality.
+        In order to test that two decision variables ar ethe same, use th` Python `is` operator;
+        use the `equals` method to test whether a given expression is equivalent to a variable:
+        for example, calling `equals` with a linear expression which consists of this variable only,
+        with a coefficient of 1, returns True.
+
+        Args:
+            other: an expression or a variable.
+
+        :return:
+            A boolean value, True if the passed variable is this very variable, or
+            if the passed expression is equivalent to the variable, else False.
+
+        """
+        # noinspection PyPep8
+        return self is other or \
+               (isinstance(other, LinearOperand) and
+                other.get_constant() == 0 and
+                other.number_of_terms() == 1 and
+                other.unchecked_get_coef(self) == 1)
+
 
 # noinspection PyAbstractClass
 class AbstractLinearExpr(Expr, LinearOperand):
     __slots__ = ('_discrete_locked',)
 
     def get_coef(self, dvar):
         """ Returns the coefficient of a variable in the expression.
@@ -764,14 +817,15 @@
             self.notify_modified(event=UpdateEvent.LinExprCoef)
         elif coef:
             # monomail is extended to a linear expr
             new_self = self.to_linear_expr()
             new_self._add_term(dvar, coef)
             # beware self is modified here
             self.notify_replaced(new_self)
+            # noinspection PyMethodFirstArgAssignment
             self = new_self
         return self
 
     # -- arithmetic to self
     def __iadd__(self, other):
         self.check_discrete_lock_frozen(item=other)
         if isinstance(other, LinearOperand) or is_number(other):
@@ -819,30 +873,30 @@
             product = self.to_linear_expr().multiply(e)
             self.notify_replaced(product)
         return product
 
     def __idiv__(self, other):
         return self.divide(other)
 
-    def __itruediv__(self, other):   # pragma: no cover
+    def __itruediv__(self, other):  # pragma: no cover
         # for py3
         return self.divide(other)
 
     def divide(self, other):
         self._model.typecheck_as_denominator(other, self)
         inverse = 1.0 / float(other)
         self.check_discrete_lock_frozen(inverse)
         self._coef *= inverse
         self.notify_modified(event=UpdateEvent.LinExprCoef)
         return self
 
     def equals(self, other):
         return isinstance(other, LinearOperand) and \
-               other.get_constant() == 0 and\
-               other.number_of_terms() == 1 and\
+               other.get_constant() == 0 and \
+               other.number_of_terms() == 1 and \
                other.unchecked_get_coef(self._dvar) == self._coef
 
     # conversion
     def to_linear_expr(self):
         e = LinearExpr(self._model, e=(self._dvar, self._coef), safe=True, transient=True)
         return e
 
@@ -866,15 +920,16 @@
     """LinearExpr()
 
     This class models linear expressions.
     This class is not intended to be instantiated. Expressions are built
     either using operators or using `Model.linear_expr()`.
     """
 
-    def _new_terms_dict(self, model, *args, **kwargs):
+    @staticmethod
+    def _new_terms_dict(model, *args, **kwargs):
         return model._term_dict_type(*args, **kwargs)
 
     @staticmethod
     def _new_empty_terms_dict(model):
         return model._term_dict_type()
 
     def to_linear_expr(self):
@@ -1195,14 +1250,36 @@
 
         Returns:
             Boolean: True if `dvar` is mentioned in the expression with a nonzero coefficient.
         """
         return dvar in self.__terms
 
     def equals(self, other):
+        """
+         This method is used to test equality between expressions.
+         Because of the overloading of operator `==` through the redefinition of
+         the `__eq__` method, you cannot use `==` to test for equality.
+         The `equals` method to test whether a given expression is equivalent to a variable.
+         Two linear expressions are equivalent if they have the same coefficient for all
+         variables.
+
+         Args:
+            other: a number or any expression.
+
+
+
+         Returns:
+             A boolean value, True if the passed expression is equivalent, else False.
+
+
+         Note:
+            A constant expression is considered equivalent to its constant number.
+
+                m.linear_expression(3).equals(3) returns True
+        """
         if is_number(other):
             return self.is_constant() and other == self.constant
         else:
             if not isinstance(other, LinearOperand):
                 return False
             if self.constant != other.get_constant():
                 return False
@@ -1220,15 +1297,15 @@
         # Writes unicode representation of self
         c = 0
         # noinspection PyPep8Naming
         SP = u' '
 
         for v, coeff in self.iter_sorted_terms():
             if not coeff:
-                continue  #  pragma: no cover
+                continue  # pragma: no cover
 
             # 1 separator
             if use_space and c > 0:
                 oss.write(SP)
 
             # ---
             # sign is printed if  non-first OR negative
@@ -1302,15 +1379,17 @@
         elif isinstance(e, LinearExpr):
             self._add_expr(e)
         elif isinstance(e, MonomialExpr):
             self._add_term(e._dvar, e._coef)
         elif isinstance(e, ZeroExpr):
             event = None
         elif is_number(e):
-            self._constant += e
+            validfn = self._model._checker.get_number_validation_fn()
+            valid_e= validfn(e) if validfn else e
+            self._constant += valid_e
             event = UpdateEvent.ExprConstant
         elif isinstance(e, Expr) and e.is_quad_expr():
             raise DOCplexQuadraticArithException
         else:
             try:
                 self.add(e.to_linear_expr())
             except AttributeError:
@@ -1749,15 +1828,17 @@
         self.model.typecheck_as_denominator(numerator=self, denominator=other)
         return self
 
     def __repr__(self):
         return "docplex.mp.ZeroExpr()"
 
     def equals(self, other):
-        return isinstance(other, ZeroExpr)
+        return (isinstance(other, LinearOperand) and (
+                           0 == other.get_constant() and (0 == other.number_of_terms()))) or\
+               (is_number(other) and other == 0)
 
     def square(self):
         return self
 
     # arithmetic to self
     add = plus
     subtract = minus
```

### Comparing `docplex-2.8.125/docplex/mp/lp_printer.py` & `docplex-2.9.141/docplex/mp/lp_printer.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,33 +2,34 @@
 # Source file provided under Apache License, Version 2.0, January 2004,
 # http://www.apache.org/licenses/
 # (c) Copyright IBM Corp. 2015, 2016
 # --------------------------------------------------------------------------
 
 
 from __future__ import print_function
-# from six import iteritems, itervalues
 
-import re
 
 from docplex.mp.linear import *
 from docplex.mp.constants import ComparisonType
 from docplex.mp.constr import LinearConstraint, RangeConstraint, QuadraticConstraint, PwlConstraint
 from docplex.mp.environment import env_is_64_bit
 from docplex.mp.mprinter import TextModelPrinter, _ExportWrapper, _NumPrinter
 
 from docplex.mp.format import LP_format
 from itertools import chain
 
 
 # gendoc: ignore
 
+def _non_compliant_lp_name_stop_here(name):
+    pass
+
 
 class LPModelPrinter(TextModelPrinter):
-    _lp_re = re.compile(r"[a-df-zA-DF-Z!#$%&()/,;?@_`'{}|\"][a-zA-Z0-9!#$%&()/.,;?@_`'{}|\"]*")
+    #_lp_re = re.compile(r"[a-df-zA-DF-Z!#$%&()/,;?@_`'{}|\"][a-zA-Z0-9!#$%&()/.,;?@_`'{}|\"]*")
 
     _lp_symbol_map = {ComparisonType.EQ: " = ",  # BEWARE NOT ==
                       ComparisonType.LE: " <= ",
                       ComparisonType.GE: " >= "}
 
     __new_line_sep = '\n'
     __expr_indent = ' ' * 6
@@ -85,24 +86,22 @@
         (varname, rhs, _) = self._rangeData[ranged_ct]
         self._print_lexpr(wrapper, num_printer, var_name_map, exp)
         wrapper.write('-', separator=False)
         wrapper.write(varname)
         wrapper.write('=')
         wrapper.write(self._num_to_string(rhs))
 
-
     def _print_logical_ct(self, wrapper, num_printer, var_name_map, logical_ct,
                           logical_symbol):
         wrapper.write(self._var_print_name(logical_ct.binary_var))
         wrapper.write("=")
         wrapper.write("%d" % logical_ct.active_value)
         wrapper.write(logical_symbol)
         self._print_binary_ct(wrapper, num_printer, var_name_map, logical_ct.linear_constraint)
 
-
     def _print_quadratic_ct(self, wrapper, num_printer, var_name_map, qct):
         q = self._print_qexpr_iter(wrapper, num_printer, var_name_map, qct.iter_net_quads())
         # force a '+' ?
         has_quads = q > 0
         self._print_binary_ct(wrapper, num_printer, var_name_map, qct, allow_empty=has_quads,
                               force_first_sign=has_quads)
 
@@ -196,62 +195,64 @@
         else:
             out.write("%s %s %s %s %s\n" % (num_printer.to_string(lb),
                                             le_symbol, varname, le_symbol,
                                             num_printer.to_string(ub)))
 
     TRUNCATE = 200
 
-    @staticmethod
-    def _non_compliant_lp_name_stop_here(name):
-        pass
-
-    def fix_name(self, mobj, prefix, local_index_map, hide_names):
-        raw_name = mobj.get_name()
-
-        # anonymous constraints must be named in a LP (we follow CPLEX here)
-        if hide_names or not raw_name or mobj.is_generated():
-            return self._make_prefix_name(mobj, prefix, local_index_map, offset=1)
-        elif not self.is_lp_compliant(raw_name):
-            if raw_name[0] in 'eE':
-                # fixing eE non-LP names
-                fixed_name = '_' + raw_name
-                if  self.is_lp_compliant(fixed_name):
-                    return fixed_name
-            # -- stats
-            self._nb_noncompliant_ids += 1
-            if not self._noncompliant_justifier:
-                self._noncompliant_justifier = raw_name
-            # --
-            self._non_compliant_lp_name_stop_here(raw_name)
-            return self._make_prefix_name(mobj, prefix, local_index_map, offset=1)
-        else:
-            # swap blanks with underscores
-            fixed_name = self._translate_chars(raw_name)
-            # truncate if necessary, again this does nothing if name is too short
-            return fixed_name[:self.TRUNCATE]
+    def _notify_new_non_compliant_name(self, non_lp_name):
+        _non_compliant_lp_name_stop_here(non_lp_name)
+        self._nb_noncompliant_ids += 1
+        if not self._noncompliant_justifier:
+            self._noncompliant_justifier = non_lp_name
+
+    def fix_name(self, mobj, prefix, local_index, hide_names):
+        return LP_format.lp_name(mobj.name, prefix, local_index, hide_names,
+                                 noncompliant_hook=self._notify_new_non_compliant_name)
+
+    # def fix_name(self, mobj, prefix, local_index, hide_names):
+    #     raw_name = mobj.get_name()
+    #
+    #     # anonymous constraints must be named in a LP (we follow CPLEX here)
+    #     if hide_names or not raw_name: # or mobj.is_generated():
+    #         return self._make_prefix_name(mobj, prefix, local_index, offset=1)
+    #
+    #     # # swap blanks with underscores
+    #     ws_name = self._translate_chars(raw_name)
+    #     if not self.is_lp_compliant(ws_name, fix_whitespace=False):
+    #         if raw_name[0] in 'eE':
+    #             # fixing eE non-LP names
+    #             fixed_name = '_' + raw_name
+    #             if self.is_lp_compliant(fixed_name, fix_whitespace=False):
+    #                 return fixed_name
+    #         # -- stats
+    #         self._notify_new_non_compliant_name(raw_name)
+    #         # --
+    #         return self._make_prefix_name(mobj, prefix, local_index, offset=1)
+    #     else:
+    #
+    #         # truncate if necessary, again this does nothing if name is too short
+    #         return ws_name[:self.TRUNCATE]
 
     def _print_model_name(self, out, model):
         model_name = None
         if model.name:
             # make sure model name is ascii
             encoded = model.name.encode('ascii', 'backslashreplace')
             if sys.version_info[0] == 3:  # pragma: no cover
                 # in python 3, encoded is a bytes at this point. Make it a string again
                 encoded = encoded.decode('ascii')
             model_name = encoded.replace('\\\\', '_').replace('\\', '_')
         printed_name = model_name or 'CPLEX'
         out.write("\\Problem name: %s\n" % printed_name)
 
     @staticmethod
-    def is_lp_compliant(name, fix_whitespace=True, _lpname_regexp=_lp_re):
-        if name is None:
-            return True  # pragma: no cover
+    def is_lp_compliant(name, fix_whitespace=True):
         fixed_name = LPModelPrinter.fix_whitespace(name) if fix_whitespace else name
-        lp_match = _lpname_regexp.match(fixed_name)
-        return lp_match and lp_match.start() == 0 and lp_match.end() == len(fixed_name)
+        return LP_format.is_lp_compliant(fixed_name)
 
     @staticmethod
     def _is_injective(name_map):
         nb_keys = len(name_map)
         nb_different_names = len(set(name_map.values()))
         return nb_different_names == nb_keys
 
@@ -276,39 +277,38 @@
 
     def _get_forced_predeclared_variables(self, model):
         # compute predeclared variables
         predeclared_variables = set()
         for sos in model.iter_sos():
             for sos_var in sos.iter_variables():
                 predeclared_variables.add(sos_var)
-        for pwl in model.iter_pwl_constraints():
-            predeclared_variables.add(pwl.y)
-            for pwv in pwl.expr.iter_variables():
+        for pwlc in model.iter_pwl_constraints():
+            for pwv in pwlc.iter_extended_variables():
                 predeclared_variables.add(pwv)
         return predeclared_variables
 
     def post_print_hook(self, model):
         nb_non_compliants = self._nb_noncompliant_ids
         if nb_non_compliants:
             try:
                 model.warning('Some identifiers are not valid LP identifiers: %d (e.g.: "%s")',
-                                   nb_non_compliants, self._noncompliant_justifier)
+                               nb_non_compliants, self._noncompliant_justifier)
             except UnicodeEncodeError:  # pragma: no cover
                 model.warning('Some identifiers are not valid LP identifiers: %d (e.g.: "%s")',
                               nb_non_compliants, self._noncompliant_justifier.encode('utf-8'))
 
     #  @profile
     def print_model_to_stream(self, out, model):
         # reset noncompliant stats
         self._nb_noncompliant_ids = 0
         self._noncompliant_justifier = None
 
         if not self._is_injective(self._var_name_map):
             # use indices to differentiate names
-            sys.__stdout__.write("\DOcplex: refine variable names\n")
+            sys.__stdout__.write("DOcplex: refine variable names\n")
             k = 0
             for dv, lp_varname in iteritems(self._var_name_map):
                 refined_name = "%s#%d" % (lp_varname, k)
                 self._var_name_map[dv] = refined_name
                 k += 1
 
         TextModelPrinter.prepare(self, model)
@@ -344,15 +344,14 @@
             # write the linear part first
             # prints an expr to a stream
             iter_linear_terms = objlin.iter_sorted_terms()
 
         printed= self._print_expr_iter(wrapper, self_num_printer, var_name_map, iter_linear_terms,
                               allow_empty=True, accept_zero=True)
 
-
         if objexpr.is_quad_expr() and objexpr.has_quadratic_term():
             self._print_qexpr_obj(wrapper, self_num_printer, var_name_map,
                                   quad_expr=objexpr,
                                   force_initial_plus=printed)
             printed = True
 
         obj_offset = objexpr.get_constant()
```

### Comparing `docplex-2.8.125/docplex/mp/mfactory.py` & `docplex-2.9.141/docplex/mp/mfactory.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,26 +8,26 @@
 
 from docplex.mp.sosvarset import SOSVariableSet
 from docplex.mp.operand import LinearOperand
 from docplex.mp.linear import Var, LinearExpr, AbstractLinearExpr, ZeroExpr
 from docplex.mp.operand import Operand
 from docplex.mp.constants import ComparisonType, UpdateEvent, ObjectiveSense
 from docplex.mp.constr import LinearConstraint, RangeConstraint, \
-    IndicatorConstraint, PwlConstraint, EquivalenceConstraint, IfThenConstraint
+    IndicatorConstraint, PwlConstraint, EquivalenceConstraint, IfThenConstraint, NotEqualConstraint
 from docplex.mp.functional import MaximumExpr, MinimumExpr, AbsExpr, PwlExpr, LogicalAndExpr, LogicalOrExpr
 from docplex.mp.pwl import PwlFunction
 from docplex.mp.compat23 import fast_range, izip_longest
+from docplex.mp.environment import Environment
 from docplex.mp.utils import *
 from docplex.mp.kpi import KPI
 from docplex.mp.solution import SolveSolution
+from docplex.mp.sttck import StaticTypeChecker
 
 from itertools import product, islice
 
-from collections import OrderedDict
-
 
 
 def fix_format_string(fmt, dimen=1, key_format='_%s'):
     ''' Fixes a format string so that it contains dimen slots with %s inside
         arguments are:
          --- dimen is the number of slots we need
          --- key_format is the format in which the %s is embedded. By default '_%s'
@@ -45,21 +45,23 @@
         if actual_nb_slots >= dimen:
             break
         curpos = new_pos + 2
     # how much slots do we need to add to the end of the string??
     nb_missing = max(0, dimen - actual_nb_slots)
     return fmt + nb_missing * (key_format % '%s')
 
+
 def is_tuple_w_standard_str(z):
     if isinstance(z, tuple):
         zclass = z.__class__
         return zclass is tuple or not ("__str__" in zclass.__dict__)
     else:
         return False
 
+
 def str_flatten_tuple(key, sep="_"):
     if is_tuple_w_standard_str(key):
         return sep.join(str(f) for f in key)
     else:
         return str(key)
 
 
@@ -108,14 +110,24 @@
                                .format(user_name))
 
 
 class _AbstractModelFactory(object):
     def __init__(self, model):
         self._model = model
         self._checker = model._checker
+        if Environment.env_is_python36:
+            # for python >= 3.6, dict is ordered
+            self._ordered_dict_type = dict
+        else:
+            from collections import OrderedDict
+            self._ordered_dict_type = OrderedDict
+
+    def dict_type(self, ordered):
+        # internal
+        return self._ordered_dict_type if ordered else dict
 
 
 class ModelFactory(_AbstractModelFactory):
 
     status_var_fmt = '[{0:s}]'
 
 
@@ -193,15 +205,15 @@
             varname = None
         else:
             # use name if any else use truncated ct string representation
             base_varname = self.status_var_fmt.format(ct.name or str_holo(ct, maxlen=20))
             # if name is already taken, use unique index at end to disambiguate
             varname = model._get_non_ambiguous_varname(base_varname)
 
-        svar = Var(model, binary_vartype, lb=0, ub=1, _safe_lb=True, _safe_ub=1, name=varname)
+        svar = Var(model, binary_vartype, lb=0, ub=1, _safe_lb=True, _safe_ub=True, name=varname)
         svar.notify_origin(ct)  # generated
 
         idx = self._engine.create_one_variable(binary_vartype, 0, 1, varname)
         model._register_one_var(svar, idx, varname)
         return svar
 
     # --- sequences
@@ -381,15 +393,15 @@
         mdl._register_block_vars(allvars, indices, all_names)
         return allvars
 
     def new_var_dict(self, keys, vartype, lb, ub, name, key_format, ordered=False):
         actual_name, key_seq = self.make_key_seq(keys, name)
         ctn = self._new_var_container(vartype, key_list=[key_seq], lb=lb, ub=ub, name=name)
         var_list = self.new_var_list(ctn, key_seq, vartype, lb, ub, actual_name, 1, key_format)
-        _dict_type = OrderedDict if ordered else dict
+        _dict_type = self.dict_type(ordered)
         return _dict_type(izip(key_seq, var_list))
 
     def new_var_multidict(self, seq_of_key_seqs, vartype, lb, ub, name, key_format=None, ordered=False):
         # ---
         fixed_keys = [self.make_key_seq(ks, name)[1] for ks in seq_of_key_seqs]
         # the sequence of keysets should answer to len(no generators here)
         dimension = len(fixed_keys)
@@ -402,15 +414,15 @@
         if not all_key_tuples:
             self.fatal('multidict has no keys to index the variables')
 
         # always pass a sequence of sequences
         ctn = self._new_var_container(vartype, key_list=fixed_keys, lb=lb, ub=ub, name=name)
         cube_vars = self.new_var_list(ctn, all_key_tuples, vartype, lb, ub, name, dimension, key_format)
 
-        _dict_type = OrderedDict if ordered else dict
+        _dict_type = self.dict_type(ordered)
         var_dict = _dict_type(izip(all_key_tuples, cube_vars))
         return var_dict
 
     def new_var_df(self, keys1, keys2, vartype, lb=None, ub=None, name=None):
         try:
             from pandas import DataFrame
         except ImportError:
@@ -455,28 +467,32 @@
 
     _operand_types = (AbstractLinearExpr, Var, ZeroExpr)
 
     @staticmethod
     def _is_operand(arg, accept_numbers=False):
         return isinstance(arg, Operand) or (accept_numbers and is_number(arg))
 
-    def _to_linear_operand(self, e, force_clone=False, context=None):
+    def _to_linear_operand(self, e, force_clone=False, msg=None):
         if isinstance(e, LinearOperand):
             if force_clone:
                 return e.clone()
             else:
                 return e
         elif is_number(e):
             return self.constant_expr(cst=e, force_clone=force_clone, safe_number=False)
         else:
             try:
                 return e.to_linear_expr()
             except AttributeError:
                 # delegate to the factory
                 return self.linear_expr(e)
+            except DocplexQuadToLinearException as qe:
+                used_msg = msg.format(e) if msg else qe.message
+                raise DOcplexException(used_msg)
+
 
     def _to_linear_expr(self, e, linexpr_class=LinearExpr, force_clone=False):
         # TODO: replace by to_linear_operand
         if isinstance(e, linexpr_class):
             if force_clone:
                 return e.clone()
             else:
@@ -506,29 +522,40 @@
 
     def new_binary_constraint(self, lhs, sense, rhs, name=None):
         ctsense = ComparisonType.parse(sense)
         return self._new_binary_constraint(lhs, ctsense, rhs, name)
 
     def _new_binary_constraint(self, lhs, sense, rhs, name=None):
         # noinspection PyPep8
-        left_expr = self._to_linear_operand(lhs, context="LinearConstraint.left_expr")
-        right_expr = self._to_linear_operand(rhs, context="LinearConstraint.right_expr")
+        left_expr = self._to_linear_operand(lhs, msg="LinearConstraint. expects linear expressions, {0} was passed")
+        right_expr = self._to_linear_operand(rhs, msg="LinearConstraint. expects linear expressions, {0} was passed")
         self._checker.typecheck_two_in_model(self._model, left_expr, right_expr, "new_binary_constraint")
         ct = LinearConstraint(self._model, left_expr, sense, right_expr, name)
         return ct
 
     def new_le_constraint(self, e, rhs, ctname=None):
         return self._new_binary_constraint(e, ComparisonType.LE, rhs, name=ctname)
 
     def new_eq_constraint(self, e, rhs, ctname=None):
         return self._new_binary_constraint(e, ComparisonType.EQ, rhs, name=ctname)
 
     def new_ge_constraint(self, e, rhs, ctname=None):
         return self._new_binary_constraint(e, ComparisonType.GE, rhs, name=ctname)
 
+    def new_neq_constraint(self, lhs, rhs, ctname=None):
+        m = self._model
+        left_expr  = self._to_linear_operand (lhs, msg="The `!=` operator requires two linear expressions, {0} was passed (left)")
+        right_expr = self._to_linear_operand(rhs, msg="The `!=` operator requires two linear expressions, {0} was passed (right)")
+        StaticTypeChecker.typecheck_discrete_expression(m, msg="NotEqualConstraint", expr=left_expr)
+        StaticTypeChecker.typecheck_discrete_expression(m, msg="NotEqualConstraint", expr=right_expr)
+        self._checker.typecheck_two_in_model(m, left_expr, right_expr, "new_binary_constraint")
+        negated_ct = self.new_eq_constraint(lhs, rhs)
+        ct = NotEqualConstraint(self._model, negated_ct, ctname)
+        return ct
+
     def _check_range_feasibility(self, lb, ub, expr):
         # INTERNAL
         if not lb <= ub:
             self._model.error("infeasible range constraint, lb={0}, ub={1}, expr={2}", lb, ub, expr)
 
     def new_range_constraint(self, lb, expr, ub, name=None, check_feasible=True):
         self._check_range_feasibility(lb, ub, expr)
@@ -761,15 +788,16 @@
                        y_var=y_var,
                        resolve=resolve)
 
     def new_pwl_constraint(self, pwl_expr, name=None):
         self_model = self._model
         return PwlConstraint(self_model, pwl_expr, name)
 
-    def default_objective_sense(self):
+    @staticmethod
+    def default_objective_sense():
         return ObjectiveSense.Minimize
 
     def new_kpi(self, kpi_arg, name_arg):
         # make a name
         if name_arg:
             publish_name = name_arg
         elif hasattr(kpi_arg, 'name') and kpi_arg.name:
@@ -791,15 +819,15 @@
             # no separator added, use a terminal "_" if need be
             ctnames = _AutomaticSymbolGenerator(ctnames)
 
         for ct, ctname in izip_longest(cts, ctnames):  # use izip_longest so as not to forget any ct
             if ct is None:  # izip stops
                 break
 
-            checker.typecheck_linear_constraint(ct, accept_ranges=False)
+            checker.typecheck_linear_constraint(ct, accept_range=False)
             checker.typecheck_string(ctname, accept_none=True, accept_empty=False, header="Model.add_constraints()")
             if prepfn(ct, ctname, check_for_trivial_ct=check_trivials):
                 posted_cts.append(ct)
         self._post_constraint_block(posted_cts)
         return posted_cts
 
     def _new_constraint_block1(self, cts):
@@ -819,32 +847,31 @@
             # TypeError is for non-tuple
             # ValueError is for nonlength-2 tuples
             # not a tuple: we have only constraints and no names
             tuple_mode = False
 
         if tuple_mode:
             for ct, ctname in ctseq:
-                checker.typecheck_linear_constraint(ct, accept_ranges=False)
+                checker.typecheck_linear_constraint(ct, accept_range=False)
                 checker.typecheck_string(ctname, accept_empty=True)
                 if prepfn(ct, ctname, check_for_trivial_ct=check_trivial, arg_checker=checker):
                     posted_cts.append(ct)
         else:
             for ct in ctseq:
-                checker.typecheck_linear_constraint(ct, accept_ranges=True)
+                checker.typecheck_linear_constraint(ct, accept_range=True)
                 if prepfn(ct, ctname=None, check_for_trivial_ct=check_trivial, arg_checker=checker):
                     posted_cts.append(ct)
         self._post_constraint_block(posted_cts)
         return posted_cts
 
     def _post_constraint_block(self, posted_cts):
         if posted_cts:
             ct_indices = self._engine.create_block_linear_constraints(posted_cts)
             self._model._register_block_cts(self._model._linct_scope, posted_cts, ct_indices)
 
-
     # --- range block
 
     def new_range_block(self, lbs, exprs, ubs, names):
         try:
             n_exprs = len(exprs)
             if n_exprs != len(lbs):
                 self.fatal('incorrect number of expressions: expecting {0}, got: {1}'.format(len(lbs), n_exprs))
```

### Comparing `docplex-2.8.125/docplex/mp/model.py` & `docplex-2.9.141/docplex/mp/model.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 import sys
 import warnings
 import six
 from six import iteritems
 
 from docplex.mp.aggregator import ModelAggregator
 from docplex.mp.compat23 import StringIO, izip
-from docplex.mp.constants import SOSType, CplexScope, ObjectiveSense
+from docplex.mp.constants import SOSType, CplexScope, ObjectiveSense, BasisStatus
 from docplex.mp.constr import AbstractConstraint, LinearConstraint, RangeConstraint, \
     IndicatorConstraint, QuadraticConstraint, PwlConstraint, EquivalenceConstraint
 from docplex.mp.context import Context, \
     is_auto_publishing_solve_details, auto_publishing_result_output_names, \
     has_credentials, auto_publising_kpis_table_names
 from docplex.mp.cloudutils import is_url_valid, make_new_kpis_dict
 
@@ -81,21 +81,14 @@
     ``Context`` is created and initialized as described in :func:`docplex.mp.context.Context.read_settings`.
 
     Example::
 
         # Creates a model named 'my model' with default context
         model = Model('my model')
 
-    In the following example, credentials for the solve service are looked up as
-    described in :func:`docplex.mp.context.Context.read_settings`::
-
-        # Creates a model with default ``context``, and override the ``agent``
-        # to solve on Decision Optimization on Cloud.
-        model = Model(agent='docloud')
-
     In this example, we create a model to solve with just 2 threads::
 
         context = Context.make_default_context()
         context.cplex_parameters.threads = 2
         model = Model(context=context)
 
     Alternatively, this can be coded as::
@@ -103,21 +96,26 @@
         model = Model()
         model.context.cplex_parameters.threads = 2
 
     Args:
         name (optional): The name of the model.
         context (optional): The solve context to be used. If no ``context`` is
             passed, a default context is created.
-        agent (optional): The ``context.solver.agent`` is initialized with
-            this string.
         log_output (optional): If ``True``, solver logs are output to
             stdout. If this is a stream, solver logs are output to that
             stream object.
-        checker (optional): If ``None``, then checking is disabled everywhere. Turning off checking
+        checker (optional): If ``off``, then checking is disabled everywhere. Turning off checking
             may improve performance but should be done only with extreme caution.
+            Possible values for the `checker` keyword argument are:
+                - `default` (or `std`, or `on`): detects modeling errors, but doe snot check
+                    numerical values for infinities or NaNs. This is the default value
+                - `numerical`: checks modeling errors and also checks all number values for  infinities
+                    or NaNs. This option should be used when data are not trusted.
+                - `off`: no typechecking is performed. This options must be used when the model has been
+                    thorougly tested and numerical data are trusted.
     """
 
     _name_generator = _AutomaticSymbolGenerator(pattern="docplex_model", offset=1)
 
     @property
     def binary_vartype(self):
         """ This property returns an instance of :class:`docplex.mp.vartype.BinaryVarType`.
@@ -339,16 +337,14 @@
     def __init__(self, name=None, context=None, **kwargs):
         """Init a new Model.
 
         Args:
             name (optional): The name of the model
             context (optional): The solve context to be used. If no ``context`` is
                 passed, a default context is created.
-            agent (optional): The ``context.solver.agent`` is initialized with
-                this string.
             log_output (optional): if ``True``, solver logs are output to
                 stdout. If this is a stream, solver logs are output to that
                 stream object.
         """
         if name is None:
             name = Model._name_generator.new_symbol()
         self._name = name
@@ -371,14 +367,16 @@
         self.__allpwlfuncs = []
         self._benders_annotations = None
         self.__all_implicit_equiv_cts = []
         self._constraint_priority_dict = {}
 
         self._allsos = []
 
+        self._lazy_constraints = []
+
         self._pwl_counter = {}
 
         # -- kpis --
         self._allkpis = []
 
         self._progress_listeners = []
         self._solve_hooks = []  # debugSolveHook()
@@ -450,16 +448,14 @@
         self._quadct_scope = _IndexScope(self.iter_quadratic_constraints, self._default_quadct_pattern,
                                          cplex_scope=CplexScope.QUAD_CT_SCOPE, offset=name_offset)
         self._pwl_scope = _IndexScope(self.iter_pwl_constraints, self._default_pwl_pattern,
                                       cplex_scope=CplexScope.PWL_CT_SCOPE, offset=name_offset)
 
         self._scopes = [self._var_scope, self._linct_scope, self._indicator_scope, self._quadct_scope, self._pwl_scope]
         self._ctscopes = [self._linct_scope, self._indicator_scope, self._quadct_scope, self._pwl_scope]
-        # a counter to generate unique numbers, incremented at each new request
-        self._unique_counter = -1
 
         # init engine
         engine = self._make_new_engine_from_agent(self.solver_agent, self.context)
         self.__engine = engine
 
         self_keep_ordering = self.keep_ordering
         self_term_dict_type = self._term_dict_type
@@ -476,14 +472,15 @@
         self._linexpr_instance_counter = 0
         self._linexpr_clone_counter = 0
         self._quadexpr_instance_counter = 0
         self._quadexpr_clone_counter = 0
 
         # all the following must be placed after an engine has been set.
         self._objective_expr = None
+        self._multi_objective_exprs = None
         engineLogLevel = get_environment().get_parameter("oaas.engineLogLevel")
         if engineLogLevel is not None and engineLogLevel in {"FINE", "FINER", "FINEST"}:
             self.parameters.read.datacheck.set(2)
 
         self.set_objective(sense=self._lfactory.default_objective_sense(),
                            expr=self._new_default_objective_expr())
 
@@ -492,14 +489,15 @@
             self._term_dict_type = dict
         else:
             self._term_dict_type = FastOrderedDict
 
     def _sync_params(self, params):
         # INTERNAL: execute only once
         if self.has_cplex():
+            params.connect_model(self)
             self_env = self._environment
             self_cplex_parameters_version = self.context.cplex_parameters.cplex_version
             self_engine = self.__engine
             installed_cplex_version = self_env.cplex_version
             # installed version is different from parameters: reset all defaults
             if installed_cplex_version != self_cplex_parameters_version:  # pragma: no cover
                 # cplex is more recent than parameters. must update defaults.
@@ -527,17 +525,17 @@
         return self.__engine.get_infinity()
 
 
     def get_cplex(self, do_raise=True):
         """ Returns the instance of Cplex used by the model, if any.
 
         In case no local installation of CPLEX can be found, this method either raises an exception,
-        if parameter `do_raise` is TYrue, or returns None if the parameter is False.
+        if parameter `do_raise` is True, or else returns None.
 
-        :param do_raise: Optional flag: if True, raise an exception when no Cplex instance
+        :param do_raise: An optional flag: if True, raise an exception when no Cplex instance
             is available, otherwise return None.
 
         :return: an instance of Cplex, or None.
         """
         try:
             cpx = self.__engine.get_cplex()
             if cpx:
@@ -655,21 +653,14 @@
     def clean_before_solve(self):
         return self._clean_before_solve
 
     @clean_before_solve.setter
     def clean_before_solve(self, must_clean):
         self._clean_before_solve = bool(must_clean)
 
-
-    # generate a new , unique counter, in the scope of this model
-    def _new_unique_counter(self):
-        # INTERNAL
-        self._unique_counter += 1
-        return self._unique_counter
-
     @property
     def time_limit_parameter(self):
         # INTERNAL
         return self.parameters.timelimit
 
     def get_time_limit(self):
         """
@@ -1127,14 +1118,18 @@
 
     def _solves_as_mip(self):
         # INTERNAL: will the model solve as a MIP?
         # returns TRue if the model contains a discrete variable or if it has SOS or
         #  if it has Piecewise Linear constraints
         return self._has_discrete_var() or self._allsos or self._pwl_counter or self.number_of_semicontinuous_variables
 
+    def solves_as_qxp(self):
+        # INTERNAL
+        return self.has_quadratic_constraint() or self._objective_expr.is_quad_expr()
+
     def get_statistics(self):
         """ Returns statistics on the model.
 
         :returns: A new instance of :class:`docplex.mp.model_stats.ModelStatistics`.
         """
         return ModelStatistics._make_new_stats(self)
 
@@ -1228,28 +1223,83 @@
         # INTERNAL
         varname_map = self.__vars_by_name
         if varname_map is not None and base_name in varname_map:
             return '{0}#{1}'.format(base_name, len(self.__allvars))
         else:
             return base_name
 
+    def generate_user_variables(self):
+        # internal
+        for dv in self.iter_variables():
+            if not dv.is_generated():
+                yield dv
+
+    def generate_user_linear_constraints(self):
+        # internal
+        for lct in self.iter_linear_constraints():
+            if not lct.is_generated():
+                yield lct
+
     def find_matching_vars(self, pattern, match_case=False):
-        key_pattern = pattern if match_case else pattern.lower()
+        """ Finds all variables whose name contain a given string
+
+        This method searches for all variables whose name
+        is not null and contains the passed ``pattern`` string. Anonymous variables
+        are not considered.
+
+        :param pattern: a non-empty string.
+
+        :return: A list of decision variables.
+        """
+        return self._find_matching_objs(self.generate_user_variables, pattern, match_case)
+
+    def find_re_matching_vars(self, regexpr):
+        """ Finds all variables whose name match a regular expression.
+
+        This method searches for all variables with a name that
+        matches the given regular expression. Anonymous variables
+        are not counted as matching.
+
+        :param regexpr: a regular expression, as define din module ``re``
+
+        :return: A list of decision variables.
+        """
         matches = []
-        for dv in self.iter_variables():
+        for dv in self.generate_user_variables():
             dvname = dv.name
-            if dvname:
-                if match_case:
-                    if key_pattern in dvname:
-                        matches.append(dv)
-                else:
-                    if key_pattern in dvname.lower():
-                        matches.append(dv)
+            if dvname and regexpr.match(dvname):
+                matches.append(dv)
         return matches
 
+    def _find_matching_objs(self, obj_iter, pattern, match_case=False):
+        # internal
+        self._checker.typecheck_string(pattern, accept_empty=False, accept_none=False, header="Model.find_matching_vars")
+        key_pattern = pattern if match_case else pattern.lower()
+        matches = []
+        for obj in obj_iter():
+            obj_name = obj.name
+            if obj_name:
+                matched = obj_name if match_case else obj_name.lower()
+                if key_pattern in matched:
+                    matches.append(obj)
+        return matches
+
+    def find_matching_linear_constraints(self, pattern, match_case=False):
+        """ Finds all linear constraints whose name contain a given string
+
+        This method searches for all linear constraints whose name
+        is not empty and contains the passed ``pattern`` string. Anonymous linear constraints
+        are not considered.
+
+        :param pattern: a non-empty string.
+
+        :return: A list of linear constraints.
+        """
+        return self._find_matching_objs(self.generate_user_linear_constraints, pattern, match_case)
+
     # index management
     def _build_index_dict(self, mobj_it, raise_on_invalid_index=False):
         #  INTERNAL
         idx_dict = {}
         for mobj in mobj_it:
             if mobj.has_valid_index():
                 idx_dict[mobj.index] = mobj
@@ -1276,14 +1326,20 @@
 
     def set_var_name(self, dvar, new_name):
         # INTERNAL: use var.name to set variable names
         if new_name != dvar.name:
             self.__engine.rename_var(dvar, new_name)
             dvar._set_name(new_name)
 
+    def set_linear_constraint_name(self, linct, new_name):
+        # INTERNAL: use lct.name to set a linear constraint's name
+        if new_name != linct.get_name():
+            self.__engine.rename_linear_constraint(linct, new_name)
+            linct._set_name(new_name)
+
     def set_var_lb(self, var, candidate_lb):
         # INTERNAL: use var.lb to set lb
         new_lb = var.vartype.resolve_lb(candidate_lb, self)
         self.__engine.set_var_lb(var, new_lb)
         var._internal_set_lb(new_lb)
 
     def set_var_ub(self, var, candidate_ub):
@@ -1363,17 +1419,30 @@
         See Also:
             :func:`number_of_range_constraints`
 
         """
         return self._count_constraints_filtered(lambda c: c.is_linear())
 
     def iter_range_constraints(self):
+        """
+        Returns an iterator on the range constraints of the model.
+
+        Returns:
+            An iterator object.
+        """
         return self.gen_constraints_with_type(RangeConstraint)
 
     def iter_binary_constraints(self):
+        """
+        Returns an iterator on the binary constraints (expr1 <op> expr2) of the model.
+        This does not include range constraints.
+
+        Returns:
+            An iterator object.
+        """
         return self.gen_constraints_with_type(LinearConstraint)
 
     def iter_linear_constraints(self):
         """
         Returns an iterator on the linear constraints of the model.
         This includes binary linear constraints and ranges but not indicators.
 
@@ -1931,14 +2000,27 @@
                    objects in `keys`.
 
         See Also:
             :attr:`infinity`
         """
         return self._var_dict(keys, self.semiinteger_vartype, lb, ub, name, key_format)
 
+    def semiinteger_var_matrix(self, keys1, keys2, lb, ub=None, name=None, key_format=None):
+        """ Creates a dictionary of semiinteger decision variables, indexed by pairs of key objects.
+
+        Creates a dictionary that allows the retrieval of variables from  a tuple
+        of two keys, the first one from `keys1`, the second one from `keys2`.
+        In short, variables are indexed by the Cartesian product of the two key sets.
+
+        A key can be any Python object, with the exception of None.
+
+        Arguments `lb`, `ub`, `name`, and `key_format` are interpreted as in :func:`semiinteger_var_dict`.
+        """
+        return self.var_multidict(self.semiinteger_vartype, [keys1, keys2], lb, ub, name, key_format)
+
     def semicontinuous_var_dict(self, keys, lb, ub=None, name=str, key_format=None):
         """  Creates a dictionary of semi-continuous decision variables, indexed by key objects.
 
         Creates a dictionary that allows retrieval of variables from business
         model objects. Keys can be either a Python collection, an iterator, or a generator.
 
         A key can be any Python object, with the exception of None.
@@ -1982,14 +2064,27 @@
                    objects in `keys`.
 
         See Also:
             :attr:`infinity`
         """
         return self._var_dict(keys, self.semicontinuous_vartype, lb, ub, name, key_format)
 
+    def semicontinuous_var_matrix(self, keys1, keys2, lb, ub=None, name=None, key_format=None):
+        """ Creates a dictionary of semivpntinuous decision variables, indexed by pairs of key objects.
+
+        Creates a dictionary that allows the retrieval of variables from  a tuple
+        of two keys, the first one from `keys1`, the second one from `keys2`.
+        In short, variables are indexed by the Cartesian product of the two key sets.
+
+        A key can be any Python object, with the exception of None.
+
+        Arguments `lb`, `ub`, `name`, and `key_format` are interpreted as in :func:`semiinteger_var_dict`.
+        """
+        return self.var_multidict(self.semicontinuous_vartype, [keys1, keys2], lb, ub, name, key_format)
+
     def var_multidict(self, vartype, seq_of_key_seqs, lb=None, ub=None, name=None, key_format=None):
         # INTERNAL
         self._checker.typecheck_vartype(vartype)
         self._checker.typecheck_iterable(seq_of_key_seqs)
         return self._lfactory.new_var_multidict(seq_of_key_seqs, vartype, lb, ub, name, key_format, ordered=self._keep_ordering)
 
     def var_matrix(self, vartype, keys1, keys2, lb=None, ub=None, name=None, key_format=None):
@@ -2412,14 +2507,18 @@
 
             name (string): An optional string to name the constraint.
 
         :returns: An instance of :class:`docplex.mp.linear.LinearConstraint`.
         """
         return self._lfactory.new_binary_constraint(lhs, ctsense, rhs, name)
 
+
+    def not_equal_constraint(self, lhs, rhs, name=None):
+        return self._lfactory.new_neq_constraint(lhs, rhs, name)
+
     def _create_engine_constraint(self, ct):
         # INTERNAL
         eng = self.__engine
         if isinstance(ct, LinearConstraint):
             return eng.create_linear_constraint(ct)
         elif isinstance(ct, RangeConstraint):
             return eng.create_range_constraint(ct)
@@ -2512,15 +2611,15 @@
 
         # --- name management ---
         if ctname:
             ct_name_map = self._cts_by_name
             if ct_name_map is not None:
                 checker.check_duplicate_name(ctname, ct_name_map, "constraint")
                 ct_name_map[ctname] = ct
-            ct.set_name(ctname)
+            ct._set_name(ctname)
         # ---
 
         # check for already posted cts.
         if ct._index >= 0:
             self.warning("constraint has already been posted: {0!s}, index is: {1}", ct, ct.index)  # pragma: no cover
             return False  # pragma: no cover
         return True
@@ -3097,20 +3196,21 @@
 
     # ----------------------------------------------------
     # objective
     # ----------------------------------------------------
 
     def round_objective_if_discrete(self, raw_obj):
         # INTERNAL
-        if self._objective_expr.is_discrete():
-            return self.round_nearest(raw_obj)
+        if is_iterable(raw_obj):
+            return [self.round_objective_if_discrete(raw_obj_item) for raw_obj_item in raw_obj]
         else:
-            return raw_obj
-
-
+            if self._objective_expr.is_discrete():
+                return self.round_nearest(raw_obj)
+            else:
+                return raw_obj
 
     def minimize(self, expr):
         """ Sets an expression as the expression to be minimized.
 
         The argument is converted to a linear expression. Accepted types are variables (instances of
         :class:`docplex.mp.linear.Var` class), linear expressions (instances of
         :class:`docplex.mp.linear.LinearExpr`), or numbers.
@@ -3127,14 +3227,58 @@
         :class:`docplex.mp.linear.Var` class), linear expressions (instances of
         :class:`docplex.mp.linear.LinearExpr`), or numbers.
 
         :param expr: A linear expression or a variable.
         """
         self.set_objective(ObjectiveSense.Maximize, expr)
 
+    def minimize_static_lex(self, exprs):
+        """ Sets a list of expressions to be minimized in a lexicographic solve.
+        exprs defines an ordered sequence of objective functions that are minimized.
+
+        The argument is converted to a list of linear expressions. Accepted types for the list elements are variables
+        (instances of :class:`docplex.mp.linear.Var` class), linear expressions (instances of
+        :class:`docplex.mp.linear.LinearExpr`), or numbers.
+
+        :warning: This method requires CPLEX 12.9
+
+        :param exprs: a list of linear expressions or variables
+        :return:
+        """
+        if not exprs:
+            self.error("Model.minimize_static_lex() requires a non-empty list of linear expressions, got: {0!r}".format(exprs))
+            return None
+
+        if not is_indexable(exprs):
+            self.fatal("Model.minimize_static_lex() requires an indexable collection of linear expressions or variables")
+        priorities = [len(exprs) - i - 1 for i in range(len(exprs))]
+        self.set_multi_objective(ObjectiveSense.Minimize, exprs, priorities=priorities)
+
+    def maximize_static_lex(self, exprs):
+        """ Sets a list of expressions to be maximized in a lexicographic solve.
+        exprs defines an ordered sequence of objective functions that are maximized.
+
+        The argument is converted to a list of linear expressions. Accepted types for the list elements are variables
+        (instances of :class:`docplex.mp.linear.Var` class), linear expressions (instances of
+        :class:`docplex.mp.linear.LinearExpr`), or numbers.
+
+        :warning: This method requires CPLEX 12.9
+
+        :param exprs: a list of linear expressions or variables
+        :return:
+        """
+        if not exprs:
+            self.error("Model.maximize_static_lex() requires a non-empty list of linear expressions, got: {0!r}".format(exprs))
+            return None
+
+        if not is_indexable(exprs):
+            self.fatal("Model.maximize_static_lex() requires an indexable collection of linear expressions or variables")
+        priorities = [len(exprs) - i - 1 for i in range(len(exprs))]
+        self.set_multi_objective(ObjectiveSense.Maximize, exprs, priorities=priorities)
+
     def is_minimize(self):
         warnings.warn("deprecated", DeprecationWarning)
         return self.is_minimized()
 
     def is_minimized(self):
         """ Checks whether the model is a minimization model.
 
@@ -3200,19 +3344,103 @@
 
         Returns:
             Boolean: True, if the model has a non-constant objective expression.
 
         """
         return not self._objective_expr.is_constant()
 
+    def set_multi_objective(self, sense, exprs, priorities=None, weights=None,
+                                abstols=None, reltols=None, names=None):
+        """ Sets a list of objectives.
+
+        :warning: This method requires CPLEX 12.9
+
+        Args:
+            :param sense: Either an instance of :class:`docplex.mp.basic.ObjectiveSense` (Minimize or Maximize),
+                    or a string: "min" or "max".
+            :param exprs: Is converted to a list of expressions. Accepted types for this list items are variables,
+                    linear expressions or numbers.
+            :param priorities: if defined, a list of priorities having the same size as the `exprs` argument. Priorities
+                    define how objectives are grouped together into sub-problems, and in which order these sub-problems
+                    are solved (in decreasing order of priorities).
+            :param weights: if defined, a list of weights having the same size as the `exprs` argument. Weights define
+                    how objectives with same priority are blended together to define the associated sub-problem's
+                    objective that is optimized.
+            :param abstols: if defined, a list of absolute tolerances having the same size as the `exprs` argument.
+            :param reltols: if defined, a list of relative tolerances having the same size as the `exprs` argument.
+            :param names:  if defined, a list of names for objectives having the same size as the `exprs` argument.
+        :return:
+
+        Note:
+            When using a number for an objective, the search will not optimize but only look for a feasible solution.
+        """
+        self.set_objective_sense(sense)
+        self.set_multi_objective_exprs(exprs, priorities=priorities, weights=weights,
+                                       abstols=abstols, reltols=reltols, names=names)
+
+    def set_multi_objective_exprs(self, new_multiobjexprs, priorities=None, weights=None,
+                                abstols=None, reltols=None, names=None, clear_objective=True):
+        """ Sets a list of objectives.
+
+        :param new_multiobjexprs: Is converted to a list of expressions. Accepted types for this list items are variables,
+                    linear expressions or numbers.
+            :param priorities: if defined, a list of priorities having the same size as the `exprs` argument. Priorities
+                    define how objectives are grouped together into sub-problems, and in which order these sub-problems
+                    are solved (in decreasing order of priorities).
+            :param weights: if defined, a list of weights having the same size as the `exprs` argument. Weights define
+                    how objectives with same priority are blended together to define the associated sub-problem's
+                    objective that is optimized.
+            :param abstols: if defined, a list of absolute tolerances having the same size as the `exprs` argument.
+            :param reltols: if defined, a list of relative tolerances having the same size as the `exprs` argument.
+            :param names:  if defined, a list of names for objectives having the same size as the `exprs` argument.
+            :param clear_objective: internal flag. Default value should be left unchanged
+        :return:
+
+        Note:
+            When using a number for an objective, the search will not optimize but only look for a feasible solution.
+        """
+        # Check case of a single objective
+        if new_multiobjexprs is not None and is_indexable(new_multiobjexprs) and len(new_multiobjexprs) == 1:
+            self.set_objective_expr(new_multiobjexprs[0])
+            return
+
+        if self.has_objective() and clear_objective:
+            self.set_objective_expr(None, clear_multiobj=False)
+
+        if new_multiobjexprs is None:
+            exprs = [self._new_default_objective_expr()]
+        else:
+            exprs = [self._lfactory._to_expr(new_objexpr) for new_objexpr in new_multiobjexprs]
+            for expr in exprs:
+                expr.notify_used(self)
+
+        eng = self.__engine
+        current_multi_objective_exprs = self._multi_objective_exprs
+        if eng:
+            # when ending the model, the engine is None here
+            eng.set_multi_objective_exprs(new_multiobjexprs=exprs, old_multiobjexprs=current_multi_objective_exprs,
+                                          priorities=priorities, weights=weights, abstols=abstols, reltols=reltols,
+                                          objnames=names)
+            if current_multi_objective_exprs is not None:
+                for expr in current_multi_objective_exprs:
+                    expr.notify_unsubscribed(subscriber=self)
+        self._multi_objective_exprs = exprs
 
     def has_objective(self):
         # INTERNAL
         return not self._objective_expr.is_zero()
 
+    def has_multi_objective(self):
+        # INTERNAL
+        if self._multi_objective_exprs is None:
+            return False
+        if len(self._multi_objective_exprs) == 1 and self._multi_objective_exprs[0].is_zero():
+            return False
+        return True
+
     def set_objective(self, sense, expr):
         """ Sets a new objective.
 
         Args:
             sense: Either an instance of :class:`docplex.mp.basic.ObjectiveSense` (Minimize or Maximize),
                 or a string: "min" or "max".
             expr: Is converted to an expression. Accepted types are variables,
@@ -3246,28 +3474,33 @@
         """
         return self._objective_sense
 
     @objective_sense.setter
     def objective_sense(self, new_sense):
         self.set_objective_sense(new_sense)
 
+    def set_objective_expr(self, new_objexpr, clear_multiobj=True):
+        if self.has_multi_objective() and clear_multiobj:
+            # Need also to set all attributes to default values so that the model won't be treated as multi-objective
+            self.set_multi_objective_exprs(None, priorities=[0], weights=[1],
+                                abstols=[0], reltols=[0], names=[None], clear_objective=False)
 
-    def set_objective_expr(self, new_objexpr):
         if new_objexpr is None:
             expr = self._new_default_objective_expr()
         else:
             expr = self._lfactory._to_expr(new_objexpr)
             #expr.keep()
             expr.notify_used(self)
 
         eng = self.__engine
         current_objective_expr = self._objective_expr
         if eng:
             # when ending the model, the engine is None here
             eng.set_objective_expr(new_objexpr=expr, old_objexpr=current_objective_expr)
+
             if current_objective_expr is not None:
                 current_objective_expr.notify_unsubscribed(subscriber=self)
         self._objective_expr = expr
 
     def get_objective_expr(self):
         """ This method returns the expression used as the model objective.
 
@@ -3340,90 +3573,60 @@
                 context.update_key_value(argname, argval)
 
         return context
 
     def solve(self, **kwargs):
         """ Starts a solve operation on the model.
 
-        If CPLEX is available, the solve operation will be performed using the native CPLEX.
-        If CPLEX is not available, the solve operation will be started on DOcplexcloud.
-        The DOcplexcloud connection parameters are looked up in the following order:
-
-            - if ``kwargs`` contains valid ``url`` and ``key`` values, they are used.
-            - if ``kwargs`` contains a ``context`` and that context contains
-                valid ``solver.docloud.url`` and ``solver.docloud.key`` values,
-                those values are used. Other attributes of ``solver.docloud``
-                can also be used. See :class:`docplex.mp.context.Context`
-            - finally, the model's attribute ``context`` is used. This ``context``
-                is set at model creation time.
-
-        If CPLEX is not available and the model has no valid credentials, an error is raised, as there is
-        no way to perform the solve.
-
-        Note that if ``url`` and ``key`` parameters are present and the
-        values of the parameters are not in the ignored url or key list,
-        the solve operation will be started on DOcplexcloud even if CPLEX is
-        available.
-
-        Example::
-
-            # forces the solve on DOcplexcloud with the specified url and keys
-            model.solve(url='https://foo.com', key='bar')
-
-        Example::
-
-            # set some DOcplexcloud credentials, but depend on another
-            # method to decide if solve is local or not
-            ctx.solver.docloud.url = 'https://foo.com'
-            ctx.solver.docloud.key = 'bar'
-            agent = 'local' if method_that_decides_if_solve_is_local() or 'docloud'
-            model.solve(context=ctx, agent=agent)
-
         Args:
             context (optional): An instance of context to be used in instead of
                 the context this model was built with.
             cplex_parameters (optional): A set of CPLEX parameters to use
                 instead of the parameters defined as
                 ``context.cplex_parameters``.
                 Accepts either a RootParameterGroup object (obtained by cloning the model's
                 parameters), or a dict of path-like names and values.
-
-            agent (optional): Changes the ``context.solver.agent`` parameter.
-                Supported agents include:
-
-                - ``docloud``: forces the solve operation to use DOcplexcloud
-                - ``local``: forces the solve operation to use native CPLEX
-
             checker (optional): a string which control all argument checks in Docplex.
                 Expects 'on' (the default) to enable all checks, or 'off' to disable all.
                 Disabling all checks might improve performance, but only when
                 it is safe to do so.
-
-            url (optional): Overwrites the URL of the
-                DOcplexcloud service defined by ``context.solver.docloud.url``.
-            key (optional): Overwrites the
-                authentication key of the DOcplexcloud service defined by
-                ``context.solver.docloud.key``.
             log_output (optional): if ``True``, solver logs are output to
                 stdout. If this is a stream, solver logs are output to that
                 stream object. Overwrites the ``context.solver.log_output``
                 parameter.
-            proxies (optional): a dict with the proxies mapping.
 
         Returns:
-            A :class:`docplex.mp.solution.SolveSolution` object if the solve operation succeeded.
-            None if the solve operation failed.
+            A :class:`docplex.mp.solution.SolveSolution` object if the solve operation managed to create
+            a feasible solution, else None.
+            The reason why solve returned None includes not only errors, but also proper cases of infeasibilties
+            or unboundedness. When solve returns None, use Model.solve_details to check the status
+            of the latest solve operation: Model.solve_details always returns
+            a :class:`docplex.mp.sdetails.SolveDetails` object, whether or not
+            a solution has been found. This object contains detailed information about the latest solve operation.
+
+        See Also:
+            :func:`solve_details`
+            :class:`docplex.mp.sdetails.SolveDetails`
         """
         if not self.is_optimized():
             self.info("No objective to optimize - searching for a feasible solution")
 
-
         lex_mipstart = kwargs.pop('_lex_mipstart', None)
+        lex_timelimits = kwargs.pop('lex_timelimits', None)
+        lex_mipgaps = kwargs.pop('lex_mipgaps', None)
         context = self.prepare_actual_context(**kwargs)
 
+        if lex_timelimits is not None and len(lex_timelimits) == 1:
+            # This will be handled as a single-objective ==> set timelimit parameter
+            context.cplex_parameters.timelimit = lex_timelimits[0]
+        if lex_mipgaps is not None and len(lex_mipgaps) == 1:
+            # This will be handled as a single-objective ==> set mipgap parameter
+            context.cplex_parameters.mip.tolerances.mipgap = lex_mipgaps[0]
+
+
         # log stuff
         saved_context_log_output = self.context.solver.log_output
         saved_log_output_stream = self.log_output
 
         try:
             self.log_output = context.solver.log_output
 
@@ -3437,15 +3640,15 @@
                     self.fatal("DOcplexcloud context has no valid credentials: {0!s}",
                                context.solver.docloud)
 
             # from now on docloud_context is None
             elif self.environment.has_cplex:
                 # if CPLEX is installed go for it
                 force_clean_before_solve = kwargs.get('clean_before_solve')
-                return self._solve_local(context, force_clean_before_solve)
+                return self._solve_local(context, force_clean_before_solve, lex_timelimits, lex_mipgaps)
             elif have_credentials:
                 # no context passed as argument, no Cplex installed, try model's own context
                 return self._solve_cloud(context, lex_mipstart)
             else:
                 # no way to solve.. really
                 return self.fatal("CPLEX runtime not found: please install CPLEX or solve this model on DOcplexcloud")
         finally:
@@ -3469,15 +3672,15 @@
             pl.disconnect()
 
     def _notify_solve_hit_limit(self, solve_details):
         # INTERNAL
         if solve_details and solve_details.has_hit_limit():
             self.info("solve: {0}".format(solve_details.status))
 
-    def _solve_local(self, context, force_clean_before_solve=None):
+    def _solve_local(self, context, force_clean_before_solve=None, lex_timelimits=None, lex_mipgaps=None):
         """ Starts a solve operation on the local machine.
 
         Note:
         This method will never try to solve on DOcplexcloud, regardless of whether the model
         has an attached DOcplexcloud context.
         If CPLEX is not available, an error is raised.
 
@@ -3550,18 +3753,19 @@
         saved_clean_before_solve = self.clean_before_solve if force_clean_before_solve is not None else None
 
         new_solution = None
         try:
             if force_clean_before_solve is not None:
                 self.clean_before_solve = force_clean_before_solve
             used_parameters = parameters or self.context._get_raw_cplex_parameters()
-            #assert used_parameters is not None
+            # assert used_parameters is not None
             self._apply_parameters_to_engine(used_parameters)
 
-            new_solution = self_engine.solve(self, parameters=parameters)
+            new_solution = self_engine.solve(self, parameters=parameters, lex_timelimits=lex_timelimits,
+                                             lex_mipgaps=lex_mipgaps)
             has_solution = new_solution is not None
             self._set_solution(new_solution)
             reported_obj = self._reported_objective_value()
 
             # store solve status as returned by the engine.
             engine_status = self_engine.get_solve_status()
             self._last_solve_status = engine_status
@@ -3704,18 +3908,26 @@
         pass
 
     def notify_solve_failed(self):
         pass
 
     def get_solve_details(self):
         """
-        This property returns detailed information about the last solve,  an instance of :class:`docplex.mp.solution.SolveDetails`.
+        This property returns detailed information about the latest solve,
+        an instance of :class:`docplex.mp.solution.SolveDetails`.
+
+        When the latest solve did return a Solution instance, this property returns the solve details
+        corresponding to the solution; when no solution has been found (in other terms, the latest
+        solve operation returned None), it still returns a SolveDetails object,
+        containing a CPLEX code identifying the reason why no solution could be found
+         (for example, infeasibility or unboundedness).
+
+        See Also:
+            :class:`docplex.mp.sdetails.SolveDetails`
 
-        Note:
-            Detailed information is returned whether or not the solve succeeded.
         """
         from copy import copy as shallow_copy
 
         return shallow_copy(self._solve_details)
 
     solve_details = property(get_solve_details)
 
@@ -3738,15 +3950,17 @@
 
     def solve_lexicographic(self, goals,
                             senses=ObjectiveSense.Minimize,
                             tolerances=None,
                             **kwargs):
         """ Performs a lexicographic solve from an ordered collection of goals.
 
-        WILL BE DEPRECATED: Starting with CPLEX engines 12.9, a new api will be available to support multi-objectives.
+        Deprecated: From CPLEX 12.9,
+        :meth:`~docplex.mp.model.Model.set_multi_objective` should be used
+        instead.
 
         :param goals: An ordered collection of linear expressions.
 
         :param senses: Either an ordered collection of senses, one sense, or
            None. The default is None, in which case the solve uses a Minimize
            sense. Each sense can be either a sense object, that is either
            `ObjectiveSense.Minimize` or `Maximize`, or a string "min" or "max".
@@ -3764,15 +3978,15 @@
             goal to be no greater than 102 if minimizing, or
             no less than 98, if maximizing.
 
         Return:
             If successful, returns a tuple with all pass solutions, reversed else None.
             The current solution of the model is the first solution in the tuple.
         """
-        warnings.warn("Will be deprecated with CPLEX 12.9 multi-objective support", PendingDeprecationWarning)
+        warnings.warn("Will be deprecated with CPLEX 12.9 multi-objective support", DeprecationWarning)
         if tolerances is None:
             schemes = generate_constant(_ToleranceScheme(), count_max=None)
         elif is_number(tolerances):
             if 0 <= tolerances <= 1:
                 schemes = generate_constant(_ToleranceScheme(relative=tolerances), count_max=None)
             else:
                 self.fatal('lexicographic tolerances expects number in [0,1], got: {0}', tolerances)
@@ -3828,15 +4042,15 @@
         ctx_params = kwargs.get(cplex_param_key)
         iter_pass_params = generate_constant(None, nb_goals)
         baseline_params = None  # parameters to restore at each iteration, default is to do nothing
         if ctx_params and is_iterable(ctx_params):
             # must pop out the list as normal solve won't have it.
             pass_params = list(kwargs.pop(cplex_param_key))
             if len(pass_params) != nb_goals:
-                self.fatal("List of parameters should have same length as goals, expecting: {0} bu a list of size {1} was passed",
+                self.fatal("List of parameters should have same length as goals, expecting: {0} but a list of size {1} was passed",
                            nb_goals, pass_params)
             else:
                 iter_pass_params = iter(pass_params)
                 baseline_params = m.context.parameters  # need to clear/reset parameters at each pass
                 # print("received a list of pass-specific parameters")
                 # for p, param in enumerate(pass_params, start=1):
                 #     print("pass #{0}".format(p), end="")
@@ -3932,15 +4146,18 @@
         :return:
         """
         self._solution = new_solution
 
     def check_has_solution(self):
         # see if we can refine messages here...
         if self._solution is None:
-            self.fatal("Model<{0}> did not solve successfully", self.name)
+            if self._solve_details is None:
+                self.fatal("Model<{0}> has not been solved yet", self.name)
+            else:
+                self.fatal("Model<{0}> did not solve successfully", self.name)
 
     def add_mip_start(self, mip_start_sol):
         """  Adds a (possibly partial) solution to use as a starting point for a MIP.
 
         This is valid only for models with binary or integer decision variables.
         The given solution must contain the value for at least one binary or integer variable.
 
@@ -3959,25 +4176,53 @@
                 self._mipstarts.append(mip_start_sol)
             except AttributeError:
                 self.fatal("add_mip_starts expects solution, got: {0!r}", mip_start_sol)
 
     @property
     def objective_value(self):
         """ This property returns the value of the objective expression in the solution of the last solve.
-
+        In case of a multi-objective, only the value for the first objective is returned
 
         Raises an exception if the model has not been solved successfully.
 
         """
         self.check_has_solution()
         return self._objective_value()
 
     def _objective_value(self):
         return self.solution.objective_value
 
+    @property
+    def multi_objective_values(self):
+        """ This property returns the list of values of the objective expressions in the solution of the last solve.
+
+        Raises an exception if the model has not been solved successfully.
+
+        """
+        self.check_has_solution()
+        return self._multi_objective_values()
+
+    def _multi_objective_values(self):
+        return self.solution.multi_objective_values
+
+    @property
+    def blended_objective_values(self):
+        """ This property returns the list of values of the blended objective expressions based on the decreasing
+        order of priorities in the solution of the last solve.
+
+        Raises an exception if the model has not been solved successfully.
+
+        """
+        self.check_has_solution()
+        blended_obj_values = self._blended_objective_values()
+        return blended_obj_values
+
+    def _blended_objective_values(self):
+        return self.solution.get_blended_objective_value_by_priority()
+
     def _reported_objective_value(self, failure_obj=0):
         return self.solution.objective_value if self.solution else failure_obj
 
     def _resolve_path(self, path_arg, basename_arg, extension):
         # INTERNAL
         if is_string(path_arg):
             if os.path.isdir(path_arg):
@@ -4209,44 +4454,42 @@
         # combination of path/directory and basename resolution are done in resolve_path
         anno_path = self._resolve_path(path, basename, extension='.ann')
         ap = ModelAnnotationPrinter()
         ap.print_to_stream(self, anno_path)
 
         return anno_path
 
-    def check_solved_as_lp(self, arg):
-        # first check a solution exists
-        self.check_has_solution()
-        return self.__engine.solved_as_lp() or self._solves_as_lp1(arg)
-
-    def solves_as_lp(self):
-        return not self._solves_as_mip()
-
-    def _solves_as_lp1(self, arg):
-        # INTERNAL
-        if self._solves_as_mip():
-            self.fatal('{0} are only available for LP problems'.format(arg))
+    def check_problem_type(self, feature, requires_solution=True, accept_qxp=True):
+        # internal
+        if self._solve_details is None:
+            self.fatal('{0} require a solution, but model is not solved yet'.format(feature))
+        elif requires_solution and self._solution is None:
+            self.fatal('{0} require a solution, but model is not solved with a solution'.format(feature))
+        elif self._solves_as_mip() or self.__engine.solved_as_mip():
+            self.fatal('{0} are not available for integer problems'.format(feature))
+        elif not accept_qxp and self.solves_as_qxp():
+            self.fatal('{0} are not available for QP/QCP problems'.format(feature))
 
     def _dual_value1(self, linear_ct):
         # PRIVATE
-        self.check_solved_as_lp(arg='dual values')
+        self.check_problem_type(feature='dual values')
         dvs = self.dual_values([linear_ct])
         return dvs[0]
 
     def dual_values(self, cts):
         """ Returns the dual values of a sequence of linear constraints.
 
         Note: the model must a pure LP: no integer or binary variable, no piecewise, no SOS.
         The model must also be solved successfully before calling this method.
 
         :param cts: a sequence of linear constraints.
 
         :return: a sequence of float numbers
         """
-        self.check_solved_as_lp(arg='dual values')
+        self.check_problem_type(feature='dual values')
         checked_lcts = self._checker.typecheck_constraint_seq(cts, check_linear=True)
         return self._dual_values(checked_lcts)
 
     def _dual_values(self, lcts):
         # PRIVATE
         for ct in lcts:
             StaticTypeChecker.typecheck_added_constraint(self, ct)
@@ -4278,39 +4521,75 @@
         # ---
         sol = self.solution
         sol.ensure_slack_values(self, self.get_engine())
         return sol.get_slacks(cts)
 
     def _reduced_cost1(self, dvar):
         # PRIVATE
-        self.check_solved_as_lp(arg='reduced costs')
+        self.check_problem_type(feature='reduced costs')
         #self._checker.typecheck_var(dvar)
         rcs = self._reduced_costs([dvar])
         return rcs[0]
 
     def reduced_costs(self, dvars):
         """ Returns the reduced costs for a sequence of variables.
 
          Note: the model must a pure LP: no integer or binary variable, no piecewise, no SOS.
          The model must also be solved successfully before calling this method.
 
         :param dvars: a sequence of decision variables.
         :return: a sequence of float numbers, in the same order as the variable sequence.
         """
-        self.check_solved_as_lp(arg='reduced costs')
+        self.check_problem_type(feature='reduced costs')
         checked_vars = self._checker.typecheck_var_seq(dvars)
         return self._reduced_costs(checked_vars)
 
     def _reduced_costs(self, dvars):
         #return self._get_engine_attribute(dvars, SolveAttribute.reduced_costs)
         sol = self.solution
         assert sol is not None
         sol.ensure_reduced_costs(model=self, engine= self.get_engine())
         return sol.get_reduced_costs(dvars)
 
+    def _var_basis_status1(self, dvar):
+        # internal
+        return self.var_basis_status([dvar])[0]
+
+    def var_basis_status(self, dvars):
+        self.check_problem_type(feature='basis status', requires_solution=False, accept_qxp=False)
+        checked_vars = self._checker.typecheck_var_seq(dvars)
+        return self._var_basis_status(checked_vars)
+
+    def _var_basis_status(self, dvars):
+        sol = self.solution
+        if sol:
+            sol.ensure_basis_statuses(model=self, engine= self.get_engine())
+            return sol.get_var_basis_statuses(dvars)
+        else:
+            var_basis, linct_basis = self.__engine.get_basis(self)
+            if not len(var_basis):
+                self.error("No basis is available")
+                return [BasisStatus.unknown]
+            else:
+                return [ BasisStatus.parse(var_basis.get(dv, -1)) for dv in dvars]
+
+    def has_basis(self):
+        """ returns True if the model contains basis information.
+
+
+
+        """
+        sol = self.solution
+        if sol:
+            sol.ensure_basis_statuses(model=self, engine= self.get_engine())
+            return sol.has_basis()
+        else:
+            var_basis, linct_basis = self.__engine.get_basis(self)
+            return len(var_basis) > 0
+
 
     DEFAULT_VAR_VALUE_QUOTED_SOLUTION_FMT = '  \"{varname}\"={value:.{prec}f}'
     DEFAULT_VAR_VALUE_UNQUOTED_SOLUTION_FMT = '  {varname}={value:.{prec}f}'
     DEFAULT_OBJECTIVE_FMT = "{0}: {1:.{prec}f}"
 
     @classmethod
     def supports_logical_constraints(cls):
@@ -4548,16 +4827,18 @@
             kpi_arg:  Accepted arguments are either an expression,
                         a lambda function with two arguments (model + solution)
                         or an instance of a subclass of abstract class KPI.
 
             publish_name (string, optional): The published name of the KPI.
 
         Note:
-            If no publish_name is provided, DOcplex will use the name of the argument. If none,
-            it will use the string representation of the argument.
+            - If no publish_name is provided, DOcplex will try to access a 'name' attribute of the argument;
+            if none exists, it will use the tring representation of the argument , as returned by str().
+            - expression KPIs are not added to the model. In other terms, adding KPIs does not change the model
+            being solved.
 
         Example:
             `model.add_kpi(x+y+z, "Total Profit")` adds the expression `(x+y+z)` as a KPI with the name "Total Profit".
 
             `model.add_kpi(x+y+z)` adds the expression `(x+y+z)` as a KPI with
             the name "x+y+z", assuming variables x,y,z have names 'x', 'y', 'z' (resp.)
 
@@ -4767,15 +5048,15 @@
                 self.warning("LP relaxation translates SOS as a constraint: {0}", sos)
                 sos_lhs = copy_model.sum_vars(var_mapping[v] for v in sos.iter_variables())
                 sos_rhs = sos.sos_type.value
                 copy_model.add(sos_lhs == sos_rhs)
         else:
             for sos in self.iter_sos():
                 if not sos.is_generated():
-                    copy_model._register_sos(sos.copy(copy_model, var_mapping))
+                    copy_model._create_engine_sos(sos.copy(copy_model, var_mapping))
 
         # parameters
         for p in self.parameters.iter_params():
             if p.is_nondefault():
                 # copy value to new parames
                 newp = copy_model.get_parameter_from_id (p.cpx_id)
                 if newp:
@@ -4871,18 +5152,26 @@
         assert parameter_cpx_id >= 0
         for p in self.parameters.generate_params():
             if p.cpx_id == parameter_cpx_id:
                 return p
         else:
             return None
 
+    def get_engine_parameter_value(self, param):
+        return self.__engine.get_parameter(param)
+
     def apply_parameters(self):
         self._apply_parameters_to_engine(self.parameters)
 
+    def apply_one_parameter(self, param):
+        # internal
+        self.__engine.set_parameter(param, param.value)
+
     def _apply_parameters_to_engine(self, parameters_to_use):
+        # internal
         if parameters_to_use is not None:
             self_engine = self.__engine
             for param in parameters_to_use:
                 self_engine.set_parameter(param, param.value)
 
     # with protocol
     def __enter__(self):
@@ -4980,17 +5269,25 @@
                        sos_type.name, sos_type.min_size(), len(var_list))
         # creates a new sos object
         return self._add_sos(dvars, sos_type, name)
 
     def _add_sos(self, dvars, sos_type, name=None):
         # INTERNAL
         new_sos = self._lfactory.new_sos(dvars, sos_type=sos_type, name=name)
+        sos_index = self.__engine.create_sos(new_sos)
         self._register_sos(new_sos)
+        new_sos.set_index(sos_index)
         return new_sos
 
+    def _create_engine_sos(self, new_sos):
+        # internal
+        sos_index = self.__engine.create_sos(new_sos)
+        self._register_sos(new_sos)
+        new_sos.set_index(sos_index)
+
     def _register_sos(self, new_sos):
         self._allsos.append(new_sos)
 
     def iter_sos(self):
         ''' Iterates over all SOS sets in the model.
 
         Returns:
@@ -5005,14 +5302,15 @@
         '''
         return len(self._allsos)
 
     def clear_sos(self):
         ''' Clears all SOS sets in the model.
         '''
         self._allsos = []
+        self.__engine.clear_all_sos()
 
     def _generate_sos(self, sos_type):
         # INTERNAL
         for sos_set in self.iter_sos():
             if sos_set.sos_type == sos_type:
                 yield sos_set
 
@@ -5072,16 +5370,16 @@
         """
         if preslope is None:
             self._checker.fatal("argument 'preslope' must be defined")
         if breaksxy is None:
             self._checker.fatal("argument 'breaksxy' must be defined")
         if postslope is None:
             self._checker.fatal("argument 'postslope' must be defined")
-        PwlFunction.check_number(self._checker, preslope)
-        PwlFunction.check_number(self._checker, postslope)
+        PwlFunction.check_number(self, preslope)
+        PwlFunction.check_number(self, postslope)
         PwlFunction.check_list_pair_breaksxy(self._checker, breaksxy)
         return self._piecewise(PwlFunction._PwlAsBreaks(preslope, breaksxy, postslope), name)
 
     def piecewise_as_slopes(self, slopebreaksx, lastslope, anchor=(0, 0), name=None):
         """  Adds a piecewise linear function (PWL) to the model, using a list of slopes and x-coordinates.
 
         Args:
@@ -5103,17 +5401,17 @@
 
             # Here is the definition of a step function to illustrate the case of a discontinuous PWL function:
             model.piecewise_as_slopes([(0, 0), (0, 1)], 0, (0, 0))
 
         Returns:
             The newly added piecewise linear function.
         """
-        PwlFunction.check_number(self._checker, lastslope)
-        PwlFunction.check_number_pair(self._checker, anchor)
-        PwlFunction.check_list_pair_slope_breakx(self._checker, slopebreaksx, anchor)
+        PwlFunction.check_number(self, lastslope)
+        PwlFunction.check_number_pair(self, anchor)
+        PwlFunction.check_list_pair_slope_breakx(self, slopebreaksx, anchor)
         return self._piecewise(PwlFunction._PwlAsSlopes(slopebreaksx, lastslope, anchor), name)
 
     def add_piecewise_constraint(self, y, pwlf, x, name=None):
         checker = self._checker
         checker.typecheck_continuous_var(x)
         checker.typecheck_continuous_var(y)
         checker.typecheck_pwl_function(pwlf)
@@ -5125,15 +5423,15 @@
         return self._add_pwl_constraint_internal(pwl_ct)
 
     def _piecewise(self, pwl_def, name=None):
         pwl_func = self._lfactory.new_piecewise(pwl_def, name)
         self.__allpwlfuncs.append(pwl_func)
         return pwl_func
 
-    def _add_pwl_expr(self, pwl_func, arg, yvar=None, name=None, resolve=True):
+    def _add_pwl_expr(self, pwl_func, arg, yvar=None, resolve=True):
         pwl_func_usage_counter = self._pwl_counter.get(pwl_func, 0) + 1
         pwl_expr = self._lfactory.new_pwl_expr(pwl_func, arg, pwl_func_usage_counter, y_var=yvar, resolve=resolve)
         return pwl_expr
 
     def _add_pwl_constraint_internal(self, ct):
         """
         INTERNAL
@@ -5232,7 +5530,24 @@
         # INTERNAL
         return self._constraint_priority_dict.get(ct)  # return None if not found
 
     def set_constraint_priority(self, ct, prio):
         # INTERNAL
         self._constraint_priority_dict[ct] = prio
 
+    def add_lazy_constraints(self, lazy_cts):
+        lazy_cts_ = self._checker.typecheck_constraint_seq(lazy_cts, check_linear=True, accept_range=False)
+        self._lazy_constraints.extend(lazy_cts_)
+        self.__engine.add_lazy_constraints(lazy_cts_)
+
+    def add_lazy_constraint(self, lazy_ct):
+        self._checker.typecheck_linear_constraint(lazy_ct, accept_range=False)
+        self._lazy_constraints.append(lazy_ct)
+        self.__engine.add_lazy_constraints([lazy_ct])
+
+    def clear_lazy_constraints(self):
+        self._lazy_constraints = []
+        self.__engine.clear_lazy_constraints()
+
+    def iter_lazy_constraints(self):
+        return iter(self._lazy_constraints)
+
```

### Comparing `docplex-2.8.125/docplex/mp/model_reader.py` & `docplex-2.9.141/docplex/mp/model_reader.py`

 * *Files 10% similar despite different names*

```diff
@@ -8,27 +8,27 @@
 
 # docplex
 from docplex.mp.model import Model
 from docplex.mp.utils import DOcplexException
 
 from docplex.mp.params.cplex_params import get_params_from_cplex_version
 from docplex.mp.constants import ComparisonType
+
 # cplex
 try:
     from cplex import Cplex
     from cplex._internal._subinterfaces import ObjSense
     from cplex.exceptions import CplexError, CplexSolverError
     from docplex.mp.cplex_engine import _safe_cplex
 
 except ImportError:  # pragma: no cover
     Cplex = None
 
 from docplex.mp.compat23 import izip
 from docplex.mp.quad import VarPair
-from docplex.mp.xcounter import FastOrderedDict
 
 
 class ModelReaderError(DOcplexException):
     pass
 
 
 class _CplexReaderFileContext(object):
@@ -54,24 +54,22 @@
             return cpx
 
         except CplexError as cpx_e:  # pragma: no cover
             # delete cplex instance
             del cpx
             raise ModelReaderError("*CPLEX error {0!s} reading file {1} - exiting".format(cpx_e, self._filename))
 
-
     # noinspection PyUnusedLocal
     def __exit__(self, exc_type, exc_val, exc_tb):
         cpx = self._cplex
         if cpx is not None:
             del cpx
             self._cplex = None
 
 
-
 class ModelReader(object):
     """ This class is used to read models from CPLEX files.
 
     All keyword arguments understood by the `Model` class can be passed to the `ModelReader` constructor
     in which case, these arguments will be used to create the initial empty model.
 
     Args:
@@ -108,18 +106,43 @@
         expr = lfactory.linear_expr(arg=0, safe=True)
         for ix, k in izip(cpx_sparsepair.ind, cpx_sparsepair.val):
             dv = var_map[ix]
             expr._add_term(dv, k)
         return expr
 
     def __init__(self, **kwargs):
-        self.model_class = kwargs.get('model_class', Model)
-        self.debug = kwargs.get('debug', False)
+        pass
+
+    @classmethod
+    def read(cls, pathname, model_name=None, verbose=False, model_class=None, **kwargs):
+        """
+        A class method to read a model from a file.
+
+        :param pathname: a path to the file to read
+        :param model_name: An optional string to use as name for the returned model.
+            If None, the basename of the path is used.
+        :param verbose: An optional flag to print informative messages, default is False.
+        :param model_class: An optional class type; must be a subclass of Model.
+            The returned model is built using this model_class and the keyword arguments kwargs, if any.
+            By default, the model is class is `Model`.
+
+        kwargs: A dict of keyword-based arguments that are used when creating the model
+            instance.
+
+        :return: a model instance, or None, if an error occurred.
+
+        Note:
+            This class method calls `ModelReader.read_model()`, without requesting to create an explicit instance
+            of `ModelReader`.
+        """
+        mri = ModelReader()
+        return mri.read_model(pathname, model_name, verbose, model_class, **kwargs)
 
-    def read_prm(self, filename):
+    @classmethod
+    def read_prm(cls, filename):
         """ Reads a CPLEX PRM file.
 
         Reads a CPLEX parameters file and returns a DOcplex parameter group
         instance. This parameter object can be used in a solve().
 
         Args:
             filename: a path string
@@ -142,14 +165,32 @@
                     except CplexError:  # pragma: no cover
                         pass
                 return params
             else:
                 return None
 
     @staticmethod
+    def _safe_call_get_names(interface, fallback_names=None):
+        # cplex crashes when calling get_names on some files (e.g. SAV)
+        # in this case filter out error 1219
+        # and return a fallback list with None or ""
+        try:
+            names = interface.get_names()
+            return names
+        except CplexSolverError as cpxse:  # pragma: no cover
+            errcode = cpxse.args[2]
+            # when all indicators have no names, cplex raises this error
+            # CPLEX Error  1219: No names exist.
+            if errcode == 1219:
+                return fallback_names or []
+            else:
+                # this is something else
+                raise
+
+    @staticmethod
     def _cplex_read(filename, verbose=False):
         # print("-> start reading file: {0}".format(filename))
         cpx = _safe_cplex()
         # no warnings
         if not verbose:
             cpx.set_results_stream(None)
             cpx.set_log_stream(None)
@@ -157,90 +198,99 @@
             cpx.set_error_stream(None)  # remove messages about names
         try:
             cpx.read(filename)
             return cpx
         except CplexError as cpx_e:
             raise ModelReaderError("*CPLEX error {0!s} reading file {1} - exiting".format(cpx_e, filename))
 
-    def read_model(self, filename, model_name=None, verbose=True, **kwargs):
+    def read_model(self, filename, model_name=None, verbose=False, model_class=None, **kwargs):
         """ Reads a model from a CPLEX export file.
 
         Accepts all formats exported by CPLEX: LP, SAV, MPS.
 
         If an error occurs while reading the file, the message of the exception
         is printed and the function returns None.
 
         Args:
             filename: The file to read.
             model_name: An optional name for the newly created model. If None,
                 the model name will be the path basename.
-            verbose: Flag.
+            verbose: An optional flag to print informative messages, default is False.
+            model_class: An optional class type; must be a subclass of Model.
+                The returned model is built using this model_class and the keyword arguments kwargs, if any.
+                By default, the model is class is `Model` (see
             kwargs: A dict of keyword-based arguments that are used when creating the model
                 instance.
 
         Example:
             `m = read_model("c:/temp/foo.mps", model_name="docplex_foo", solver_agent="docloud", output_level=100)`
 
         Returns:
             An instance of Model, or None if an exception is raised.
 
+        See Also:
+            :class:`docplex.mp.model.Model`
+
         """
         if not Cplex:  # pragma: no cover
             raise RuntimeError("read_prm() requires CPLEX to run")
 
         if not os.path.exists(filename):
             raise IOError("* file not found: {0}".format(filename))
 
-
-        # extract pure basename
+        # extract basename
         if model_name:
             name_to_use = model_name
         else:
             basename = os.path.basename(filename)
             dotpos = basename.find(".")
             if dotpos > 0:
                 name_to_use = basename[:dotpos]
             else:
                 name_to_use = basename
 
+        model_class = model_class or Model
+
         if 0 == os.stat(filename).st_size:
             print("* file is empty: {0} - exiting".format(filename))
-            return Model(name=name_to_use, **kwargs)
-
+            return model_class(name=name_to_use, **kwargs)
 
         # print("-> start reading file: {0}".format(filename))
         cpx = self._cplex_read(filename, verbose=verbose)
+
         if not cpx:  # pragma: no cover
             return None
 
         range_map = {}
         final_output_level = kwargs.get("output_level", "info")
+        debug_read = kwargs.get("debug", False)
 
         try:
             # force no tck
             if 'checker' in kwargs:
                 final_checker = kwargs['checker']
             else:
                 final_checker = 'default'
             # build the model with no checker, then restore final_checker in the end.
             kwargs['checker'] = 'off'
             # -------------
 
-            mdl = self.model_class(name=name_to_use, **kwargs)
+            mdl = model_class(name=name_to_use, **kwargs)
             lfactory = mdl._lfactory
             qfactory = mdl._qfactory
             mdl.set_quiet()  # output level set to ERROR
             vartype_cont = mdl.continuous_vartype
             vartype_map = {'B': mdl.binary_vartype,
                            'I': mdl.integer_vartype,
                            'C': mdl.continuous_vartype,
                            'S': mdl.semicontinuous_vartype}
             # 1 upload variables
             cpx_nb_vars = cpx.variables.get_num()
-            cpx_var_names = cpx.variables.get_names()
+            cpx_var_names = self._safe_call_get_names(cpx.variables)
+
             if cpx._is_MIP():
                 cpx_vartypes = [vartype_map.get(cpxt, vartype_cont) for cpxt in cpx.variables.get_types()]
             else:
                 cpx_vartypes = [vartype_cont] * cpx_nb_vars
             cpx_var_lbs = cpx.variables.get_lower_bounds()
             cpx_var_ubs = cpx.variables.get_upper_bounds()
             # map from cplex variable indices to docplex's
@@ -250,17 +300,17 @@
 
             d = 0
             model_varnames = []
             model_lbs = []
             model_ubs = []
             model_types = []
             for v in range(cpx_nb_vars):
-                varname = cpx_var_names[v]
+                varname = cpx_var_names[v] if cpx_var_names else None
 
-                if varname.startswith("Rg"):
+                if varname and varname.startswith("Rg"):
                     # generated var for ranges
                     range_map[v] = self._RangeData(var_index=v, var_name=varname, ub=cpx_var_ubs[v])
                 else:
                     # docplex_var = lfactory.new_var(vartype, lb, ub, varname)
                     var_index_map[v] = d
                     model_varnames.append(varname)
                     model_types.append(cpx_vartypes[v])
@@ -280,15 +330,15 @@
             # 2. upload linear constraints and ranges (mixed in cplex)
             cpx_linearcts = cpx.linear_constraints
             nb_linear_cts = cpx_linearcts.get_num()
             all_rows = cpx_linearcts.get_rows()
             all_rhs = cpx_linearcts.get_rhs()
             all_senses = cpx_linearcts.get_senses()
             all_range_values = cpx_linearcts.get_range_values()
-            cpx_ctnames = cpx_linearcts.get_names()
+            cpx_ctnames = self._safe_call_get_names(cpx_linearcts)
 
             has_range = range_map or any(s == "R" for s in all_senses)
             deferred_cts = []
 
             for c in range(nb_linear_cts):
                 row = all_rows[c]
                 sense = all_senses[c]
@@ -305,40 +355,43 @@
                     op = ComparisonType.parse(sense)
                     ct = lfactory._new_binary_constraint(lhs=expr, rhs=rhs, sense=op)
                     ct.name = ctname
                     deferred_cts.append(ct)
 
                 else:
                     expr = lfactory.linear_expr()
+                    rcoef = 1
                     for idx, koef in izip(indices, coefs):
                         var = cpx_var_index_to_docplex.get(idx, None)
                         if var:
                             expr._add_term(var, koef)
                         elif idx in range_map:
                             # this is a range: coeff must be 1 or -1
                             abscoef = koef if koef >= 0 else -koef
+                            rcoef = koef
                             assert abscoef == 1, "range var has coef different from 1: {}".format(koef)
-                            assert range_data is None, "range_data is not None: {0!s}".format(range_data)  # cannot use two range vars
+                            assert range_data is None, "range_data is not None: {0!s}".format(
+                                range_data)  # cannot use two range vars
                             range_data = range_map[idx]
                         else:  # pragma: no cover
                             # this is an internal error.
                             raise ModelReaderError("ERROR: index not in var map or range map: {0}".format(idx))
 
                     if range_data:
                         label = ctname or 'c#%d' % (c + 1)
                         if sense not in "EL":  # pragma: no cover
                             raise ModelReaderError("{0} range sense is not E: {1!s}".format(label, sense))
-                        if koef < 0:  # -1 actually
+                        if rcoef < 0:  # -1 actually
                             rng_lb = rhs
                             rng_ub = rhs + range_data.ub
-                        elif koef > 0:  # koef is 1 here
+                        elif rcoef > 0:  # koef is 1 here
                             rng_lb = rhs - range_data.ub
                             rng_ub = rhs
                         else:  # pragma: no cover
-                            raise ModelReaderError("unexpected range coef: {}".format(koef))
+                            raise ModelReaderError("unexpected range coef: {}".format(rcoef))
 
                         mdl.add_range(lb=rng_lb, expr=expr, ub=rng_ub, rng_name=ctname)
                     else:
                         if sense == 'R':
                             # range min is rangeval
                             range_lb = rhs
                             range_ub = rhs + range_val
@@ -356,15 +409,15 @@
             nb_quadratic_cts = cpx_quadraticcts.get_num()
             all_rhs = cpx_quadraticcts.get_rhs()
             all_linear_nb_non_zeros = cpx_quadraticcts.get_linear_num_nonzeros()
             all_linear_components = cpx_quadraticcts.get_linear_components()
             all_quadratic_nb_non_zeros = cpx_quadraticcts.get_quad_num_nonzeros()
             all_quadratic_components = cpx_quadraticcts.get_quadratic_components()
             all_senses = cpx_quadraticcts.get_senses()
-            cpx_ctnames = cpx_quadraticcts.get_names()
+            cpx_ctnames = self._safe_call_get_names(cpx_quadraticcts)
 
             for c in range(nb_quadratic_cts):
                 rhs = all_rhs[c]
                 linear_nb_non_zeros = all_linear_nb_non_zeros[c]
                 linear_component = all_linear_components[c]
                 quadratic_nb_non_zeros = all_quadratic_nb_non_zeros[c]
                 quadratic_component = all_quadratic_components[c]
@@ -392,30 +445,15 @@
                 op = ComparisonType.cplex_ctsense_to_python_op(sense)
                 ct = op(quad_expr, rhs)
                 mdl.add_constraint(ct, ctname)
 
             # 4. upload indicators
             cpx_indicators = cpx.indicator_constraints
             nb_indicators = cpx_indicators.get_num()
-            try:
-                all_ind_names = cpx_indicators.get_names()
-
-            except CplexSolverError as cpxse:  # pragma: no cover
-                errcode = cpxse.args[2]
-                # when all indicators have no names, cplex raises this error
-                # CPLEX Error  1219: No names exist.
-                if errcode == 1219:
-                    # seems cplex raises this error when no indicator has name
-                    all_ind_names = []
-                else:
-                    raise cpxse  # this is something else.
-
-            except Exception as e:  # pragma: no cover
-                # any other Pythonlayer error is abnormal
-                raise ModelReaderError("Error when reading file: {0}, raised: {1!s}".format(filename, str(e)))
+            all_ind_names = self._safe_call_get_names(cpx_indicators)
 
             all_ind_bvars = cpx_indicators.get_indicator_variables()
             all_ind_rhs = cpx_indicators.get_rhs()
             all_ind_linearcts = cpx_indicators.get_linear_components()
             all_ind_senses = cpx_indicators.get_senses()
             all_ind_complemented = cpx_indicators.get_complemented()
             lfactory = mdl._lfactory
@@ -436,27 +474,28 @@
                                                           active_value=1 - ind_complemented, name=ind_name)
                 mdl.add(indct)
 
             # 5. upload Piecewise linear constraints
             try:
                 cpx_pwl = cpx.pwl_constraints
                 cpx_pwl_defs = cpx_pwl.get_definitions()
-                cpx_pwl_names = cpx_pwl.get_names()
+                pwl_fallback_names = [""] * cpx_pwl.get_num()
+                cpx_pwl_names = self._safe_call_get_names(cpx_pwl, pwl_fallback_names)
                 for (vary_idx, varx_idx, preslope, postslope, breakx, breaky), pwl_name in izip(cpx_pwl_defs,
                                                                                                 cpx_pwl_names):
                     varx = cpx_var_index_to_docplex.get(varx_idx, None)
                     vary = cpx_var_index_to_docplex.get(vary_idx, None)
                     breakxy = [(brkx, brky) for brkx, brky in zip(breakx, breaky)]
                     pwl_func = mdl.piecewise(preslope, breakxy, postslope, name=pwl_name)
                     pwl_expr = mdl._lfactory.new_pwl_expr(pwl_func, varx, 0, add_counter_suffix=False, resolve=False)
                     pwl_expr._f_var = vary
                     pwl_expr._ensure_resolved()
 
             except AttributeError:  # pragma: no cover
-                pass    # Do not check for PWLs if Cplex version does not support them
+                pass  # Do not check for PWLs if Cplex version does not support them
 
             # 6. upload objective
             cpx_obj = cpx.objective
             cpx_sense = cpx_obj.get_sense()
 
             cpx_all_lin_obj_coeffs = cpx_obj.get_linear()
             # noinspection PyPep8
@@ -502,44 +541,41 @@
                     cpx_sos_names = [None] * cpx_sos_num
                 for sostype, sos_sparse, sos_name in izip(cpx_sos_types, cpx_sos_indices, cpx_sos_names):
                     sos_var_indices = sos_sparse.ind
                     isostype = int(sostype)
                     sos_vars = [cpx_var_index_to_docplex[var_ix] for var_ix in sos_var_indices]
                     mdl.add_sos(dvars=sos_vars, sos_arg=isostype, name=sos_name)
 
-
             mdl.output_level = final_output_level
             if final_checker:
                 # need to restore checker
                 mdl.set_checker(final_checker)
 
         except CplexError as cpx_e:  # pragma: no cover
             print("* CPLEX error: {0!s} reading file {1}".format(cpx_e, filename))
             mdl = None
-            if self.debug:
+            if debug_read:
                 raise
 
         except ModelReaderError as mre:  # pragma: no cover
             print("! Model reader error: {0!s} while reading file {1}".format(mre, filename))
             mdl = None
-            if self.debug:
+            if debug_read:
                 raise
 
-        except DOcplexException as doe:   # pragma: no cover
+        except DOcplexException as doe:  # pragma: no cover
             print("! Internal DOcplex error: {0!s} while reading file {1}".format(doe, filename))
             mdl = None
-            if self.debug:
+            if debug_read:
                 raise
 
         except Exception as any_e:  # pragma: no cover
             print("Internal exception raised: {0!s} while reading file {1}".format(any_e, filename))
             mdl = None
-            if self.debug:
+            if debug_read:
                 raise
 
         finally:
             # clean up CPLEX instance...
             del cpx
 
-
         return mdl
-
```

### Comparing `docplex-2.8.125/docplex/mp/model_stats.py` & `docplex-2.9.141/docplex/mp/model_stats.py`

 * *Files identical despite different names*

### Comparing `docplex-2.8.125/docplex/mp/mprinter.py` & `docplex-2.9.141/docplex/mp/mprinter.py`

 * *Files 1% similar despite different names*

```diff
@@ -301,34 +301,30 @@
     def _make_prefix_name(mobj, prefix, local_index, offset=1):
         prefixed_name = "{0:s}{1:d}".format(prefix, local_index + offset)
         return prefixed_name
 
     from docplex.mp.compat23 import mktrans
 
     __raw = " -+/\\<>"
-    __cooked = "_mpd___"
+    __cooked = "_mp____"
 
     _str_translate_table = mktrans(__raw, __cooked)
     _unicode_translate_table = {}
     for c in range(len(__raw)):
         _unicode_translate_table[ord(__raw[c])] = ord(__cooked[c])
 
     @staticmethod
     def _translate_chars2(raw_name):
         # noinspection PyUnresolvedReferences
         if isinstance(raw_name, unicode):
             char_mapping = TextModelPrinter._unicode_translate_table
         else:
             char_mapping = TextModelPrinter._str_translate_table
         return raw_name.translate(char_mapping)
-        # INTERNAL
-        # return raw_name
-        # from docplex.mp.utils import mktrans
-        # table = mktrans(" -+/\\<>", "_mpd___")
-        # return raw_name.translate(table)
+
 
     @staticmethod
     def _translate_chars3(raw_name):
         return raw_name.translate(TextModelPrinter._unicode_translate_table)
 
     def fix_name(self, mobj, prefix, local_index, hide_names):
         # INTERNAL
```

### Comparing `docplex-2.8.125/docplex/mp/numutils.py` & `docplex-2.9.141/docplex/mp/numutils.py`

 * *Files identical despite different names*

### Comparing `docplex-2.8.125/docplex/mp/operand.py` & `docplex-2.9.141/docplex/mp/operand.py`

 * *Files 6% similar despite different names*

```diff
@@ -22,14 +22,15 @@
     # --- basic subscription api
     def notify_used(self, user):
         pass
 
     def notify_unsubscribed(self, subscriber):
         pass
 
+    # noinspection PyMethodMayBeStatic
     def is_in_use(self):
         return False
 
     def notify_modified(self, event):
         pass
 
     def keep(self):
@@ -48,14 +49,15 @@
 
     def __eq__(self, rhs):
         return self._model._qfactory.new_xconstraint(lhs=self, rhs=rhs, comparaison_type=ComparisonType.EQ)
 
     def __ge__(self, rhs):
         return self._model._qfactory.new_xconstraint(lhs=self, rhs=rhs, comparaison_type=ComparisonType.GE)
 
+
     le = __le__
     eq = __eq__
     ge = __ge__
 
 
 class LinearOperand(Operand):
     # no ctor as used in multiple inheritance
@@ -81,14 +83,15 @@
 
     def number_of_terms(self):
         return sum(1 for _ in self.iter_terms())
 
     def size(self):
         return self.number_of_terms()
 
+    # noinspection PyMethodMayBeStatic
     def iter_quads(self):
         return iter_emptyset()
 
     def is_constant(self):
         # redefine this for subclasses.
         return False  # pragma: no cover
 
@@ -112,14 +115,17 @@
         :param: dvar (:class:`docplex.mp.linear.Var`): A decision variable.
 
         Returns:
             Boolean: True if the variable is present in the expression, else False.
         """
         return self.contains_var(dvar)
 
+    def __ne__(self, rhs):
+        return self._model._lfactory.new_neq_constraint(lhs=self, rhs=rhs)
+
     def contains_var(self, dvar):
         raise NotImplementedError  # pragma: no cover
 
     def lock_discrete(self):
         pass
 
     def is_discrete_locked(self):
```

### Comparing `docplex-2.8.125/docplex/mp/ppretty.py` & `docplex-2.9.141/docplex/mp/ppretty.py`

 * *Files identical despite different names*

### Comparing `docplex-2.8.125/docplex/mp/printer_factory.py` & `docplex-2.9.141/docplex/mp/printer_factory.py`

 * *Files identical despite different names*

### Comparing `docplex-2.8.125/docplex/mp/progress.py` & `docplex-2.9.141/docplex/mp/progress.py`

 * *Files identical despite different names*

### Comparing `docplex-2.8.125/docplex/mp/pwl.py` & `docplex-2.9.141/docplex/mp/pwl.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 # (c) Copyright IBM Corp. 2015, 2016
 # --------------------------------------------------------------------------
 
 from docplex.mp.utils import is_iterable
 from docplex.mp.basic import ModelingObjectBase
 from docplex.mp.utils import DOcplexException, is_number
 from docplex.mp.compat23 import izip
+from docplex.mp.sttck import StaticTypeChecker
 
-import math
 import copy
 
 
 class PwlFunction(ModelingObjectBase):
     """
     This class models piecewise linear (PWL) functions. This class is not intended to be instantiated:
     piecewise linear functions are defined by invoking :func:`docplex.mp.model.Model.piecewise`,
@@ -27,96 +27,95 @@
     * by giving an ordered list of (x,y) points that are linearly connected, along with the slope before the first
       point and the slope after the last point.
 
     Note that a piecewise-linear function may be discontinuous.
     """
 
     @staticmethod
-    def check_number(checker, arg):
-        checker.typecheck_num(arg)
-        if math.isinf(arg):
-            checker.fatal("infinite value detected")
+    def check_number(logger, arg):
+        StaticTypeChecker.typecheck_num_nan_inf(logger, arg)
+
 
     @staticmethod
-    def check_list_pair_breaksxy(checker, arg):
+    def check_list_pair_breaksxy(logger, arg):
         if not is_iterable(arg):
-            checker.fatal("not an iterable: {0!s}".format(arg))
+            logger.fatal("not an iterable: {0!s}".format(arg))
         if isinstance(arg, tuple):
             # Encapsulate tuple argument into a list: this allows defining a PWL with a tuple if there is only
             #  one element in its definition
             arg = [arg]
         if len(arg) == 0:
-            checker.fatal("argument 'breaksxy' must be a non-empty list of (x, y) tuples.")
+            logger.fatal("argument 'breaksxy' must be a non-empty list of (x, y) tuples.")
         prev_pair = None
         pprev_pair = None
         for pair in arg:
             if isinstance(pair, tuple):
                 if len(pair) != 2:
-                    checker.fatal("invalid tuple in 'breaksxy': {0!s}. Each tuple must have 2 items.".format(pair))
-                PwlFunction.check_number(checker, pair[0])
-                PwlFunction.check_number(checker, pair[1])
+                    logger.fatal("invalid tuple in 'breaksxy': {0!s}. Each tuple must have 2 items.".format(pair))
+                PwlFunction.check_number(logger, pair[0])
+                PwlFunction.check_number(logger, pair[1])
             else:
-                checker.fatal("invalid item in 'breaksxy': {0!s}. Each item must be a (x, y) tuple.".format(pair))
+                logger.fatal("invalid item in 'breaksxy': {0!s}. Each item must be a (x, y) tuple.".format(pair))
             if prev_pair is not None:
                 if pair[0] < prev_pair[0]:
-                    checker.fatal("X coordinate in: {0!s} cannot be smaller than previous break abscisse: {1!s}.".
-                                  format(pair, prev_pair))
+                    logger.fatal("X coordinate in: {0!s} cannot be smaller than previous break abscisse: {1!s}.".
+                                 format(pair, prev_pair))
                 if pprev_pair is not None and pair[0] == prev_pair[0] and prev_pair[0] == pprev_pair[0]:
-                    checker.fatal(
+                    logger.fatal(
                         "invalid break: {0!s}. There cannot be more than 2 consecutive breaks with same abscisse.".
                             format(pair))
             pprev_pair = prev_pair
             prev_pair = pair
 
     @staticmethod
-    def check_number_pair(checker, arg):
+    def check_number_pair(logger, arg):
         if arg is None:
-            checker.fatal("argument 'anchor' must be defined")
+            logger.fatal("argument 'anchor' must be defined")
         if isinstance(arg, tuple):
             if len(arg) != 2:
-                checker.fatal("invalid tuple for 'anchor': {0!s}. Anchor argument must have 2 items.".format(arg))
-            PwlFunction.check_number(checker, arg[0])
-            PwlFunction.check_number(checker, arg[1])
+                logger.fatal("invalid tuple for 'anchor': {0!s}. Anchor argument must have 2 items.".format(arg))
+            PwlFunction.check_number(logger, arg[0])
+            PwlFunction.check_number(logger, arg[1])
         else:
-            checker.fatal("invalid value for 'anchor': {0!s}. Anchor argument must be a (x, y) tuple.".format(arg))
+            logger.fatal("invalid value for 'anchor': {0!s}. Anchor argument must be a (x, y) tuple.".format(arg))
 
     @staticmethod
-    def check_list_pair_slope_breakx(checker, arg, anchor):
+    def check_list_pair_slope_breakx(logger, arg, anchor):
         if arg is None:
-            checker.fatal("argument 'slopebreaksx' must be defined")
+            logger.fatal("argument 'slopebreaksx' must be defined")
         if not is_iterable(arg):
-            checker.fatal("not an iterable: {0!s}".format(arg))
+            logger.fatal("not an iterable: {0!s}".format(arg))
         if len(arg) == 0:
             return
         if isinstance(arg, tuple):
             # Encapsulate tuple argument into a list: this allows defining a PWL with a tuple if there is only
             #  one element in its definition
             arg = [arg]
         prev_pair = None
         pprev_pair = None
         for pair in arg:
             if isinstance(pair, tuple):
                 if len(pair) != 2:
-                    checker.fatal("invalid tuple in 'slopebreaksx': {0!s}. Each tuple must have 2 items.".
-                                  format(pair))
-                PwlFunction.check_number(checker, pair[0])
-                PwlFunction.check_number(checker, pair[1])
+                    logger.fatal("invalid tuple in 'slopebreaksx': {0!s}. Each tuple must have 2 items.".
+                                 format(pair))
+                PwlFunction.check_number(logger, pair[0])
+                PwlFunction.check_number(logger, pair[1])
             else:
-                checker.fatal("invalid item in 'slopebreaksx': {0!s}. Each item must be a (x, y) tuple.".format(pair))
+                logger.fatal("invalid item in 'slopebreaksx': {0!s}. Each item must be a (x, y) tuple.".format(pair))
             if prev_pair is not None:
                 if pair[1] < prev_pair[1]:
-                    checker.fatal("X coordinate in: {0!s} cannot be smaller than previous break abscisse: {1!s}.".
-                                  format(pair, prev_pair))
+                    logger.fatal("X coordinate in: {0!s} cannot be smaller than previous break abscisse: {1!s}.".
+                                 format(pair, prev_pair))
                 if pprev_pair is not None and pair[1] == prev_pair[1] and prev_pair[1] == pprev_pair[1]:
-                    checker.fatal(
+                    logger.fatal(
                         "invalid break: {0!s}. There cannot be more than 2 consecutive breaks with same abscisse.".
                             format(pair))
                 if pair[1] == prev_pair[1] and anchor[0] == pair[1]:
-                    checker.fatal("anchor {0!s} cannot be defined at discontinuity point: {1!s}".
-                                  format(anchor, pair))
+                    logger.fatal("anchor {0!s} cannot be defined at discontinuity point: {1!s}".
+                                 format(anchor, pair))
             pprev_pair = prev_pair
             prev_pair = pair
 
     class _PwlAsBreaks:
         """
         When using this class, the piecewise linear function is specified by:
          - Breakpoints defined as a list of coordinate pairs `(x[i], y[i])` defining the segments of the PWL function.
@@ -193,15 +192,15 @@
                     # Discontinuity
                     return break_1, break_2, index + 1
             return break_1, None, index
 
         def _get_y_value(self, x_coord, prev_break_index=-1):
             """
             :param x_coord:
-            :param prev_break: this parameter is mandatory if a breakxy tuple does exist before x_coord. Otherwise
+            :param prev_break_index: this parameter is mandatory if a breakxy tuple does exist before x_coord. Otherwise
                 an exception is raised.
             :return:
             """
             if prev_break_index < 0:
                 break_1, break_2, last_ind = self._get_break_at_index(0)
                 if break_1[0] < x_coord:
                     raise DOcplexException("Invalid arguments passed to PwlAsBreaks._get_y_value()")
```

### Comparing `docplex-2.8.125/docplex/mp/quad.py` & `docplex-2.9.141/docplex/mp/quad.py`

 * *Files 0% similar despite different names*

```diff
@@ -729,16 +729,18 @@
         # subtract quad
         quadterms = self._quadterms
         for oqv, oqk in other_quad.iter_quads():
             update_dict_from_item_value(quadterms, oqv, -oqk)
         # subtract linear part
         self._linexpr.subtract(other_quad._linexpr)
 
-    def to_linear_expr(self):  # pragma: no cover
-        self.fatal("Quadratic expression [{0!s}] cannot be converted to a linear expression", self)
+    def to_linear_expr(self, msg=None):  # pragma: no cover
+        # used_msg = msg or "Quadratic expression [{0!s}] cannot be converted to a linear expression"
+        # self.fatal(used_msg, self)
+        raise DocplexQuadToLinearException(self)
 
     def is_normalized(self):  # pragma: no cover
         # INTERNAL
         for _, qk in self.iter_quads():
             if not qk:
                 return False  # pragma: no cover
         else:
@@ -750,11 +752,14 @@
 
     def __le__(self, other):
         return self._model._qfactory.new_le_constraint(self, other)
 
     def __ge__(self, other):
         return self._model._qfactory.new_ge_constraint(self, other)
 
+    def __ne__(self, other):
+        self.model.fatal("Operator `!=` is not supported for quadratic expressions, {0!s} was passed", self)
+
     def notify_expr_modified(self, expr, event):
         if expr is self._linexpr:
             # something to do..
             self.notify_modified(event, )
```

### Comparing `docplex-2.8.125/docplex/mp/quadfact.py` & `docplex-2.9.141/docplex/mp/quadfact.py`

 * *Files identical despite different names*

### Comparing `docplex-2.8.125/docplex/mp/relaxer.py` & `docplex-2.9.141/docplex/mp/relaxer.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,14 +11,37 @@
 from docplex.mp.utils import is_function, apply_thread_limitations
 from docplex.mp.basic import Priority
 from docplex.mp.constr import AbstractConstraint
 from docplex.mp.error_handler import docplex_fatal
 from docplex.mp.sdetails import SolveDetails
 
 from docplex.mp.cloudutils import context_must_use_docloud, context_has_docloud_credentials
+from docplex.util import as_df
+from docplex.mp.utils import PublishResultAsDf
+
+
+try:
+    import pandas as pd
+except ImportError:
+    pd = None
+
+
+def to_output_table(relaxer, use_pd=True):
+    columns = ['Constraint', 'Priority', 'Amount']
+    if pd and use_pd:
+        return as_df(relaxer)
+    else:
+        TOutputTables = namedtuple('TOutputTables', columns)
+        result = []
+        prioritizer = relaxer.prioritizer
+        for ct, relaxed in relaxer.iter_relaxations():
+            result.append(TOutputTables(ct.name,
+                                        prioritizer.get_priority(ct).name,
+                                        relaxed))
+        return result
 
 
 def _match_priority_name(prio, s, sep='_'):
     if not s:
         return False  # pragma: no cover
 
     s_lower = s.lower()
@@ -241,15 +264,15 @@
 
 
 # internal named tuples
 _TRelaxableGroup = namedtuple("_TRelaxableGroup", ["preference", "relaxables"])
 _TParamData = namedtuple('_TParamInfo', ['short_name', 'default_value', 'accessor'])
 
 
-class Relaxer(object):
+class Relaxer(PublishResultAsDf, object):
     ''' This class is an abstract algorithm, in the sense that it operates on interfaces.
 
         It takes a prioritizer, which an implementation of ``IConstraintPrioritizer``.
         For convenience, predefined prioritizer types are accessible  through names:
 
             - `all` relaxes all constraints using a MEDIUM priority; this is the default.
             - `named` relaxes all constraints with a user name but not the others.
@@ -268,15 +291,19 @@
 
     '''
     default_precision = 1e-5
 
     _default_mode = RelaxationMode.OptSum
 
     def __init__(self, prioritizer='all', verbose=False, precision=default_precision,
-                 override=False):
+                 override=False, output_processing=None):
+        self.output_table_customizer = output_processing
+        self.output_table_property_name = 'relaxations_output'
+        self.default_output_table_name = 'relaxations.csv'
+        self.output_table_using_df = True  # if pandas is available of course
 
         self._precision = precision
         # ---
         if isinstance(prioritizer, IConstraintPrioritizer):
             self._prioritizer = prioritizer
         elif prioritizer == 'match':
             self._prioritizer = MatchNamePrioritizer(override=override)
@@ -303,20 +330,29 @@
         self._relaxations = {}
         self._verbose = verbose
         self._verbose_listener = VerboseRelaxationListener()
 
         if self._verbose:
             self.add_listener(self._verbose_listener)
 
+
+    @property
+    def prioritizer(self):
+        return self._prioritizer
+
     def set_verbose(self, is_verbose):
         if is_verbose != self._verbose:
-            if is_verbose:
-                self.add_listener(self._verbose_listener)
-            else:
-                self.remove_listener(self._verbose_listener)
+            self._verbose = is_verbose
+            self.set_verbose_listener_from_flag(is_verbose)
+
+    def set_verbose_listener_from_flag(self, is_verbose):
+        if is_verbose:
+            self.add_listener(self._verbose_listener)
+        else:
+            self.remove_listener(self._verbose_listener)
 
     def get_verbose(self):
         return self._verbose
 
     verbose = property(get_verbose, set_verbose)
 
     def _check_successful_relaxation(self):
@@ -351,15 +387,15 @@
     def remove_listener(self, listener):
         # INTERNAL
         # """ Removes a relaxation listener.
         #
         # Args:
         #     listener: The listener to remove.
         # """
-        if isinstance(listener, IRelaxationListener) and listener in self._listeners:
+        if listener in self._listeners:
             self._listeners.remove(listener)
 
     def clear_listeners(self):
         # INTERNAL
         # """ Removes all relaxation listeners.
         # """
         self._listeners = []
@@ -409,18 +445,18 @@
         if 0 == nb_prioritized_cts:
             mdl.error("Relaxation algorithm found no relaxable constraints - exiting")
             return None
         if nb_mandatories:
             assert mandatory_justifier is not None
             mdl.warning('{0} constraint(s) will not be relaxed (e.g.: {1!s})', nb_mandatories, mandatory_justifier)
 
-        relax_verbose = kwargs.pop('verbose', False)
-        temp_listener = VerboseRelaxationListener() if relax_verbose and not self._verbose else None
-        if temp_listener:
-            self.add_listener(temp_listener)
+        temp_relax_verbose = kwargs.pop('verbose', False)
+        if temp_relax_verbose != self._verbose:
+            # install/deinstall listener for this relaxation only
+            self.set_verbose_listener_from_flag(temp_relax_verbose)
 
         # relaxation loop
         all_groups = []
         all_relaxable_cts = []
         is_cumulative = self._cumulative
         # -- relaxation mode
         if relax_mode is None:
@@ -448,15 +484,15 @@
                 # create new docloud engine on the fly
                 relax_engine = mdl._new_docloud_engine(relax_context)
                 transient_engine = True
             else:
                 mdl.fatal("DOcplexcloud context has no valid credentials: {0!s}",
                           relax_context.solver.docloud)
 
-        if self.verbose:
+        if temp_relax_verbose:
             print("-- starting relaxation. mode: {0!s}, precision={1}".format(used_relax_mode.name, self._precision))
 
         try:
             # mdl.context has been saved in saved_context above
             mdl.context = relax_context
             mdl.set_log_output(mdl.context.solver.log_output)
 
@@ -510,37 +546,46 @@
                         self._last_relaxation_objective = relaxed_sol.objective_value
 
                         # filter irrelevant relaxations below some threshold
                         for ct in all_relaxable_cts:
                             raw_infeas = relaxed_sol.get_infeasibility(ct)
                             if self._accept_violation(raw_infeas):
                                 self._relaxations[ct] = raw_infeas
+                        if not self._relaxations:
+                            mdl.warning("Relaxation of model `{0}` found one relaxed solution, but no relaxed constraints - check".format(mdl.name))
 
                         for l in self._listeners:
                             l.notify_successful_relaxation(prio, all_relaxable_cts, relax_obj, self._relaxations)
                         # now get out
                         break
                     else:
+                        # TODO: maybe issue a warning that relaxation has failed?
                         # relaxation has failed, notify the listeners
                         for l in self._listeners:
                             l.notify_failed_relaxation(prio, all_relaxable_cts)
 
             mdl.notify_solve_relaxed(relaxed_sol, relax_engine.get_solve_details())
 
+            # write relaxation table.write_output_table() handles everything related to
+            # whether the table should be published etc...
+            if self.is_publishing_output_table(mdl.context):
+                output_table = to_output_table(self, self.output_table_using_df)
+                self.write_output_table(output_table, mdl.context)
         finally:
             # --- restore context, log_output if set.
             if saved_log_output_stream != mdl.log_output:
                 mdl.set_log_output_as_stream(saved_log_output_stream)
             if saved_context_log_output != mdl.context.solver.log_output:
                 mdl.context.solver.log_output = saved_context_log_output
             mdl.context = saved_context
             if transient_engine:
                 del relax_engine
-            if temp_listener:
-                self.remove_listener(temp_listener)
+            if temp_relax_verbose != self._verbose:
+                # realign listener with flag
+                self.set_verbose_listener_from_flag(self._verbose)
 
         return relaxed_sol
 
     def iter_relaxations(self):
         """ Iterates on relaxations.
 
         Relaxations are built as a dictionary with constraints as keys and numeric violations as values,
@@ -555,14 +600,36 @@
         Returns:
            A dictionary where the keys are the relaxed constraints,
           and the values are the numerical slacks.
 
         """
         return self._relaxations.copy()
 
+    def __as_df__(self):
+        ''' Returns a pandas.DataFrame with all relaxed constraint.
+
+        Returns:
+           A pandas.DataFrame which columns are:
+
+              - Constraint: the constraint name
+              - Priority: The priority of the constraint
+              - Amount: The amount of relaxation
+        '''
+        if not pd:
+            raise NotImplementedError('Cannot convert results to DataFrame, pandas is not available')
+        columns = ['Constraint', 'Priority', 'Amount']
+        results_list = []
+        prioritizer = self.prioritizer
+        for ct, relaxed in self.iter_relaxations():
+            results_list.append({'Constraint': ct.name,
+                                 'Priority': prioritizer.get_priority(ct).name,
+                                 'Amount': relaxed})
+        df = pd.DataFrame(results_list, columns=columns)
+        return df
+
     def get_total_relaxation(self):
         self._check_successful_relaxation()
         return sum(abs(v) for v in self._relaxations.values())
 
     @property
     def total_relaxation(self):
         return self.get_total_relaxation()
```

### Comparing `docplex-2.8.125/docplex/mp/sdetails.py` & `docplex-2.9.141/docplex/mp/sdetails.py`

 * *Files 6% similar despite different names*

```diff
@@ -91,18 +91,18 @@
                         8: "fixed_MIQP",
                         9: "node_QP",
                         10: "QCP",
                         11: "MIQCP",
                         12: "node_QCP"}
 
     @staticmethod
-    def _convert_problemtype(probtype, probtype_map=_problemtype_map, unknown_probtype="unknown"):
+    def _convert_problemtype(probtype, unknown_probtype="unknown"):
         try:
             iprobe_type = int(probtype)
-            return probtype_map.get(iprobe_type, unknown_probtype)
+            return SolveDetails._problemtype_map.get(iprobe_type, unknown_probtype)
         except ValueError:
             return unknown_probtype
 
     @staticmethod
     def to_plain_str(arg_s):
         if SIX_PY2:  # we are in py2: docloud returns unicode.
             try:
@@ -170,14 +170,23 @@
         """ This property returns the solve time in seconds.
 
         """
         return self._time
 
     @property
     def status_code(self):
+        """
+        This property returns the CPLEX status code as a number.
+        Possible values for the status code are described in the CPLEX documentation
+        at:
+        https://www.ibm.com/support/knowledgecenter/SSSA5P_12.8.0/ilog.odms.cplex.help/refcallablelibrary/macros/Solution_status_codes.html
+
+        :return: an integer number (a CPLEX status code)
+
+        """
         return self._solve_status_code
 
     # status string
     # CPX_STAT_ABORT_DETTIME_LIM =  25
     # CPX_STAT_ABORT_DUAL_OBJ_LIM =  22
     # CPX_STAT_ABORT_IT_LIM =  10
     # CPX_STAT_ABORT_OBJ_LIM =  12
@@ -210,19 +219,31 @@
     # CPX_STAT_OPTIMAL_RELAXED_SUM =  15
     # CPX_STAT_UNBOUNDED =  2
 
     @property
     def status(self):
         """ This property returns the solve status as a string.
 
+        This string is normally the value returned by the CPLEX callable library method
+        CPXXgetstatstring,
+        see https://www.ibm.com/support/knowledgecenter/SSSA5P_12.8.0/ilog.odms.cplex.help/refcallablelibrary/cpxapi/getstatstring.html
+
         Example:
             * Returns "optimal" when the solution has been proven optimal.
             * Returns "feasible" for a feasible, but not optimal, solution.
             * Returns "MIP_time_limit_feasible" for a MIP solution obtained before a time limit.
 
+        Note:
+            In certain cases, status may return a string that is not directly passed from CPLEX
+
+                * If an exception occurs during the CPLEX solve phase, status contains the text of the exception.
+                * If solve fails because of a promotional version limitation, the following message is returned
+                    "Promotional version. Problem size limits exceeded., CPLEX code=1016."
+                    The corresponding status  code is 1016.
+
         """
         return self._solve_status
 
     @property
     def problem_type(self):
         """  This property returns the problem type as a string.
```

### Comparing `docplex-2.8.125/docplex/mp/solution.py` & `docplex-2.9.141/docplex/mp/solution.py`

 * *Files 6% similar despite different names*

```diff
@@ -12,25 +12,28 @@
 import copy
 
 import six
 
 try:  # pragma: no cover
     from itertools import zip_longest as izip_longest
 except ImportError:  # pragma: no cover
+    # noinspection PyUnresolvedReferences
     from itertools import izip_longest
 
 from six import iteritems, iterkeys
 
-from docplex.mp.compat23 import StringIO, izip
-from docplex.mp.constants import CplexScope
-from docplex.mp.utils import is_iterable, is_number, is_string, str_holo, OutputStreamAdapter
+from docplex.mp.compat23 import StringIO
+from docplex.mp.constants import CplexScope, BasisStatus
+from docplex.mp.utils import is_iterable, is_number, is_string, is_indexable, str_holo, OutputStreamAdapter
 from docplex.mp.utils import make_output_path2, DOcplexException
 from docplex.mp.linear import Var
 from docplex.mp.error_handler import docplex_fatal
 
+from docplex.mp.solmst import SolutionMSTPrinter
+
 from collections import defaultdict
 
 
 # noinspection PyAttributeOutsideInit
 class SolveSolution(object):
     """
     The :class:`SolveSolution` class holds the result of a solve.
@@ -39,65 +42,77 @@
     # a symbolic value for no objective ?
     NO_OBJECTIVE_VALUE = -1e+75
 
     @staticmethod
     def _is_discrete_value(v):
         return v == int(v)
 
-    def __init__(self, model, var_value_map=None, obj=None, name=None, solved_by=None, keep_zeros=True,
-                 rounding=False):
+    def __init__(self, model, var_value_map=None, obj=None, blended_obj_by_priority=None, name=None, solved_by=None,
+                 keep_zeros=True, rounding=False):
         """ SolveSolution(model, var_value_map, obj, name)
 
         Creates a new solution object, associated to a a model.
 
         Args:
             model: The model to which the solution is associated. This model cannot be changed.
 
             obj: The value of the objective in the solution. A value of None means the objective is not defined at the
                 time the solution is created, and will be set later.
 
+            blended_obj_by_priority: For multi-objective models: the value of sub-problems' objectives (each sub-problem
+                groups objectives having same priority).
+
             var_value_map: a Python dictionary containing associations of variables to values.
 
             name: a name for the solution. The default is None, in which case the solution is named after the
                 model name.
 
         :return: A solution object.
         """
         assert model is not None
         assert solved_by is None or is_string(solved_by)
-        assert obj is None or is_number(obj)
+        assert obj is None or is_number(obj) or is_indexable(obj)
+        assert blended_obj_by_priority is None or is_indexable(blended_obj_by_priority)
 
         self.__model = model
         self._checker = model._checker
         self._name = name
         self._problem_name = model.name
         self._problem_objective_expr = model.objective_expr if model.has_objective() else None
         self._objective = self.NO_OBJECTIVE_VALUE if obj is None else obj
+        self._blended_objective_by_priority = [self.NO_OBJECTIVE_VALUE] if blended_obj_by_priority is None else \
+            blended_obj_by_priority
         self._solved_by = solved_by
         self.__var_value_map = {}
+
+        # attributes
         self._reduced_costs = None
         self._dual_values = None
         self._slack_values = None
         self._infeasibilities = {}
+        self._basis_statuses = None
+
         self.__round_discrete = rounding
         self._solve_status = None
         self._keep_zeros = keep_zeros
         self._solve_details = None
         # the round function
         self._roundfn = self.__model.round_nearest
 
         if var_value_map is not None:
             self._store_var_value_map(var_value_map, keep_zeros=keep_zeros, rounding=rounding)
 
     @staticmethod
-    def make_engine_solution(model, var_value_map, obj, solved_by, solve_details, job_solve_status=None):
+    def make_engine_solution(model, var_value_map, obj, blended_obj_by_priority, solved_by, solve_details,
+                             job_solve_status=None):
         # INTERNAL
         sol = SolveSolution(model,
                             var_value_map=None,
                             obj=obj,
+                            blended_obj_by_priority=blended_obj_by_priority,
                             solved_by=solved_by,
                             rounding=True,
                             keep_zeros=False)
         sol._solve_details = copy.copy(solve_details)
         # trust engines
         for var, value in iteritems(var_value_map):
             if value:
@@ -179,15 +194,15 @@
             # var is None hereafter
             elif do_raise:
                 self.model.fatal("No variable with named {0}", var_key)
             else:
                 self.model.warning("No variable with named {0}", var_key)
                 return None
 
-        else:  #  pragma: no cover
+        else:  # pragma: no cover
             self.model.fatal("Expecting variable or name, got: {0!r}", var_key)
 
     def _typecheck_var_key_value(self, var_key, value, caller):
         # INTERNAL
         self._checker.typecheck_num(value, caller=caller)
         if not is_string(var_key) and not isinstance(var_key, Var):
             self.model.fatal("{0} expects either Var or string, got: {1!r}", caller, var_key)
@@ -196,41 +211,59 @@
         """ Adds a new (variable, value) pair to this solution.
 
         Args:
             var_key: A decision variable (:class:`docplex.mp.linear.Var`) or a variable name (string).
             value (number): The value of the variable in the solution.
         """
         self._typecheck_var_key_value(var_key, value, caller="Solution.add_var_value")
-        self._set_var_key_value(var_key, value, keep_zero=True, rounding=False)
+        self._set_var_key_value(var_key, value, keep_zero=self._keep_zeros, rounding=False)
 
     def __setitem__(self, var_key, value):
         # always keep zero, no warnings, no checks
         self._set_var_key_value(var_key, value, keep_zero=self._keep_zeros, rounding=False)
 
     def set_var_key_value(self, var_key, value, keep_zero, rounding):
         # INTERNAL
         self._typecheck_var_key_value(var_key, value, caller="Solution.add_var_value")
         self._set_var_key_value(var_key, value, keep_zero, rounding)
 
     def _set_var_key_value(self, var_key, value, keep_zero, rounding):
         # INTERNAL: no checks done.
-        if value or keep_zero:
-            var = self._resolve_var(var_key, do_raise=False)
-            if var is not None:
-                self._set_var_value_internal(var, value, rounding)
+        dvar = self._resolve_var(var_key, do_raise=False)
+        if dvar is not None:
+            if value or keep_zero:
+                # either value is nonzero or we keep all, store.
+                self._set_var_value_internal(dvar, value, rounding)
+            elif self.contains(dvar):
+                # value is 0 and we dont keep zeros: zap the variable, if
+                del self.__var_value_map[dvar]
 
     def _set_var_value_internal(self, var, value, rounding):
         # INTERNAL, no check
-        if var.is_discrete() and rounding and not self._is_discrete_value(value):
+        if rounding and var.is_discrete() and not self._is_discrete_value(value):
             stored_value = self._roundfn(value)
         else:
             stored_value = value
 
         self.__var_value_map[var] = stored_value
 
+    def update(self, var_values_iterable):
+        """
+        Updates the solution from a dictionary. Keys can be either strings, interpreted as variable names,
+        or variables; values are the new values for the variable.
+
+        This method returns nothing, only performs a side effect on the solution object.
+
+        :param var_values_iterable: a dictionary of keys, values.
+
+        """
+        keep_zeros = self._keep_zeros
+        for k, v in iteritems(var_values_iterable):
+            self._set_var_key_value(k, v, keep_zeros, rounding=False)
+
     @property
     def model(self):
         """
         This property returns the model associated with the solution.
         """
         return self.__model
 
@@ -253,56 +286,87 @@
 
     # @property
     # def error_handler(self):
     #     return self.__model.error_handler
 
     def get_objective_value(self):
         """
-        Gets the objective value as defined in the solution.
+        Gets the objective value (or list of objectives value) as defined in the solution.
         When the objective value has not been defined, a special value `NO_SOLUTION` is returned.
         To check whether the objective has been set, use :func:`has_objective`.
 
         Returns:
-            float: The value of the objective as defined by the solution.
+            float or list(float): The value of the objective (or list of values for multi-objective) as defined by
+            the solution.
         """
         return self._objective
 
     def set_objective_value(self, obj):
         """
-        Sets the objective value of the solution.
+        Sets the objective value (or list of values for multi-objective) of the solution.
         
         Args:
-            obj (float): The value of the objective in the solution.
+            obj (float or list(float)): The value of the objective (or list of values for multi-objective) in
+            the solution.
         """
         self._objective = obj
 
+    def get_blended_objective_value_by_priority(self):
+        """
+        Gets the blended objective value (or list of blended objectives value) by priority level as defined in
+        the solution.
+        When the objective value has not been defined, a special value `NO_SOLUTION` is returned.
+        To check whether the objective has been set, use :func:`has_objective`.
+
+        Returns:
+            float or list(float): The value of the objective (or list of values for multi-objective) as defined by
+            the solution.
+        """
+        return self._blended_objective_by_priority
+
     def has_objective(self):
         """
         Checks whether or not the objective has been set.
 
         Returns:
             Boolean: True if the solution defines an objective value.
         """
         return self._objective != self.NO_OBJECTIVE_VALUE
 
     @property
     def objective_value(self):
-        """ This property is used to get or set the objective valueof the solution.
+        """ This property is used to get the objective value of the solution.
+        In case of multi-objective this property returns the value for the first objective
 
         When the objective value has not been defined, a special value `NO_SOLUTION` is returned.
         To check whether the objective has been set, use :func:`has_objective`.
 
         """
+        if is_indexable(self._objective):
+            return self._objective[0]
         return self._objective
 
     @objective_value.setter
     def objective_value(self, new_objvalue):
         self.set_objective_value(new_objvalue)
 
     @property
+    def multi_objective_values(self):
+        """ This property is used to get the list of objective values of the solution.
+        In case of single objective this property returns the value for the objective as a singleton list
+
+        When the objective value has not been defined, a special value `NO_SOLUTION` is returned.
+        To check whether the objective has been set, use :func:`has_objective`.
+
+        """
+        if is_indexable(self._objective):
+            return self._objective
+        return [self._objective]
+
+    @property
     def solve_status(self):
         return self._solve_status
 
     def _set_solve_status(self, new_status):
         # INTERNAL
         self._solve_status = new_status
 
@@ -373,16 +437,16 @@
         Gets the value of a variable or an expression in a solution.
         If the variable is not mentioned in the solution,
         the method returns 0 and does not raise an exception.
         Note that this method can also be used as :func:`solution[arg]`
         because the :func:`__getitem__` method has been overloaded.
 
         Args:
-            arg: A decision variable (:class:`docplex.mp.linear.Var`) or a variable name (string),
-                 or an expression.
+            arg: A decision variable (:class:`docplex.mp.linear.Var`),
+                 a variable name (a string), or an expression.
 
         Returns:
             float: The value of the variable in the solution.
         """
         if is_string(arg):
             var = self._get_var_by_name(arg)
             if var is None:
@@ -505,15 +569,25 @@
     def check(self, tolerance=1e-6):
         return not (self.find_unsatisfied_constraints(tolerance))
 
     def equals_solution(self, other, check_models=False, check_explicit=False, obj_precision=1e-3, var_precision=1e-6):
         if check_models and (self.model != other.model):
             return False
 
-        if math.fabs(self.objective_value - other.objective_value) >= obj_precision:
+        if is_iterable(self.objective_value) and is_iterable(other.objective_value):
+            if len(self.objective_value) == len(other.objective_value):
+                for self_obj_val, other_obj_val in zip(self.objective_value, other.objective_value):
+                    if math.fabs(self_obj_val - other_obj_val) >= obj_precision:
+                        return False
+            else:  # Different number of objectives
+                return False
+        elif not is_iterable(self.objective_value) and not is_iterable(other.objective_value):
+            if math.fabs(self.objective_value - other.objective_value) >= obj_precision:
+                return False
+        else:  # One solution is for multi-objective, and not the other
             return False
 
         for dvar, val in self.iter_var_values():
             if check_explicit and not other.contains(dvar):
                 return False
             this_val = self._get_var_value(dvar)
             other_val = other._get_var_value(dvar)
@@ -538,14 +612,22 @@
         if self._dual_values is None:
             self._dual_values = engine.get_all_dual_values(model)
 
     def ensure_slack_values(self, model, engine):
         if self._slack_values is None:
             self._slack_values = engine.get_all_slack_values(model)
 
+    def ensure_basis_statuses(self, model, engine):
+        if self._basis_statuses is None:
+            #  returns a tuple of two lists
+            self._basis_statuses = engine.get_basis(model)
+
+    def has_basis(self):
+        return self._basis_statuses is not None
+
     def get_reduced_costs(self, dvars):
         rcs = self._reduced_costs
         assert rcs is not None
         return [rcs.get(dv, 0) for dv in dvars]
 
     def get_dual_values(self, lcts):
         duals = self._dual_values
@@ -554,14 +636,23 @@
 
     def get_slacks(self, cts):
         all_slacks = self._slack_values
         assert all_slacks is not None
         # first get cplex_scope, then fetch the slack: two indirections
         return [all_slacks[ct.cplex_scope()].get(ct, 0) for ct in cts]
 
+    def get_var_basis_statuses(self, dvars):
+        assert self._basis_statuses is not None
+        all_var_basis_statuses = self._basis_statuses[0]
+        return [BasisStatus.parse(all_var_basis_statuses.get(dv, -1)) for dv in dvars]
+
+    def get_linearct_basis_statuses(self, linear_cts):
+        assert self._basis_statuses is not None
+        all_linearct_basis_statuses = self._basis_statuses[1]
+        return [all_linearct_basis_statuses.get(lct, -1) for lct in linear_cts]
 
     def get_infeasibility(self, ct):
         return self._infeasibilities.get(ct, 0)
 
     def display_attributes(self):
         pass
 
@@ -654,14 +745,27 @@
         return str_holo(r, maxlen=72)
 
     def __iter__(self):
         # INTERNAL: this is necessary to prevent solution from being an iterable.
         # as it follows getitem protocol, it can mistakenly be interpreted as an iterable
         raise TypeError
 
+    def __as_df__(self):
+        try:
+            import pandas
+        except ImportError:
+            raise NotImplementedError('Cannot convert solution to pandas.DataFrame if pandas is not available')
+        solution_df = pandas.DataFrame(columns=['name', 'value'])
+
+        for index, dvar in enumerate(self.iter_variables()):
+            solution_df.loc[index, 'name'] = dvar.to_string()
+            solution_df.loc[index, 'value'] = dvar.solution_value
+
+        return solution_df
+
     def print_mst(self):
         """
         Writes the solution in an output stream "out" (assumed to satisfy the file interface)
         in CPLEX MST format.
         """
         SolutionMSTPrinter.print_one_solution(sol=self, out=sys.stdout)
 
@@ -686,14 +790,17 @@
                 Can be a directory, in which case the basename
                 that was computed with the basename argument is appended to the directory to produce
                 the file.
                 If given a full path, the path is directly used to write the file, and
                 the basename argument is not used.
                 If passed None, the output directory will be ``tempfile.gettempdir()``.
 
+        returns:
+            The full path of the file, when successful, else None
+
         Example:
             Assuming the solution has the name "prob":
 
             ``sol.export_as_mst()`` will write file prob.mst in a temporary directory.
 
             ``sol.export_as_mst(path="c:/temp/myprob1.mst")`` will write file "c:/temp/myprob1.mst".
 
@@ -702,14 +809,15 @@
         """
         mst_path = make_output_path2(actual_name=self._problem_name,
                                      extension=SolutionMSTPrinter.mst_extension,
                                      path=path,
                                      basename_arg=basename)
         if mst_path:
             self.print_mst_to_stream(mst_path)
+            return mst_path
 
     def get_printer(self, key):
         # INTERNAL
         printers = {'json': SolutionJSONPrinter,
                     'xml': SolutionMSTPrinter
                     }
 
@@ -806,147 +914,14 @@
         See:
             :func: `docplex.mp.model.kpi_by_name`
         '''
         kpi = self.model.kpi_by_name(name, try_match=True, match_case=match_case)
         return kpi._get_solution_value(self)
 
 
-class SolutionMSTPrinter(object):
-    # header contains the final newline
-    mst_header = """<?xml version = "1.0" standalone="yes"?>
-<?xml-stylesheet href="https://www.ilog.com/products/cplex/xmlv1.0/solution.xsl" type="text/xsl"?>
-
-"""
-    mst_extension = ".mst"
-
-    one_solution_start_tag = "<CPLEXSolution version=\"1.0\">"
-    one_solution_end_tag = "</CPLEXSolution>"
-
-    # used when several solutions are present
-    many_solution_start_tag = "<CPLEXSolutions version=\"1.0\">"
-    many_solution_end_tag = "</CPLEXSolutions>"
-
-    @staticmethod
-    def print_signature(out):
-        from docplex.version import docplex_version_string
-        osa = OutputStreamAdapter(out)
-        osa.write("<!-- This file has been generated by DOcplex version {}  -->\n".format(docplex_version_string))
-
-    @classmethod
-    def print(cls, out, solutions):
-        # solutions can be either a plain solution or a sequence or an iterator
-        if not is_iterable(solutions):
-            cls.print_one_solution(solutions, out)
-        else:
-            sol_seq = list(solutions)
-            nb_solutions = len(sol_seq)
-            assert nb_solutions > 0
-            if 1 == nb_solutions:
-                cls.print_one_solution(sol_seq[0], out)
-            else:
-                cls.print_many_solutions(sol_seq, out)
-
-    @classmethod
-    def print_one_solution(cls, sol, out, print_header=True):
-        osa = OutputStreamAdapter(out)
-        if print_header:
-            osa.write(cls.mst_header)
-            cls.print_signature(out)
-        # <CPLEXSolution version="1.0">
-        osa.write(cls.one_solution_start_tag)
-        osa.write("\n")
-
-        # <header
-        # problemName="foo"
-        # objectiveValue="42"
-        # />
-        osa.write(" <header\n   problemName=\"{0}\"\n".format(sol.problem_name))
-        if sol.has_objective():
-            osa.write("   objectiveValue=\"{0:g}\"\n".format(sol.objective_value))
-        osa.write("  />\n")
-
-        # prepare reduced costs 
-        """ For mst, we don't want this !
-        model = sol.model
-        if not model._solves_as_mip():
-            reduced_costs = model.reduced_costs(model.iter_variables())
-        else:
-            reduced_costs = []
-        """
-        #  <variables>
-        #    <variable name="x1" index ="1" value="3.14"/>
-        #  </variables>
-        osa.write(" <variables>\n")
-        """ For mst, we don't want this !
-        for (dvar, rc) in zip_longest(model.iter_variables(), reduced_costs,
-                                      fillvalue=None):
-            var_name = dvar.name
-            var_value = sol[dvar]
-            var_index = dvar.index
-            rc_string = ""
-            if rc is not None:
-                rc_string = "reducedCost=\"{}\"".format(rc)
-            osa.write("  <variable name=\"{0}\" index=\"{1}\" value=\"{2:g}\" {3}/>\n"
-              .format(var_name, var_index, var_value, rc_string))
-        """
-        for dvar, val in sol.iter_var_values():
-            var_name = dvar.print_name()
-            var_value = sol[dvar]
-            var_index = dvar.index
-            osa.write("  <variable name=\"{0}\" index=\"{1}\" value=\"{2:g}\"/>\n"
-                      .format(var_name, var_index, var_value))
-        osa.write(" </variables>\n")
-
-        #  </CPLEXSolution version="1.0">
-        osa.write(cls.one_solution_end_tag)
-        osa.write("\n")
-
-    @classmethod
-    def print_many_solutions(cls, sol_seq, out):
-        osa = OutputStreamAdapter(out)
-        osa.write(cls.mst_header)
-        cls.print_signature(out)
-        # <CPLEXSolutions version="1.0">
-        osa.write(cls.many_solution_start_tag)
-        osa.write("\n")
-
-        for sol in sol_seq:
-            cls.print_one_solution(sol, out, print_header=False)
-
-        # <CPLEXSolutions version="1.0">
-        osa.write(cls.many_solution_end_tag)
-        osa.write("\n")
-
-    @classmethod
-    def print_to_stream(cls, solutions, out, extension=mst_extension, **kwargs):
-        if out is None:
-            # prints on standard output
-            cls.print(sys.stdout, solutions)
-        elif isinstance(out, str):
-            # a string is interpreted as a path name
-            path = out if out.endswith(extension) else out + extension
-            with open(path, "w") as of:
-                cls.print_to_stream(solutions, of)
-                # print("* file: %s overwritten" % path)
-        else:
-            try:
-                cls.print(out, solutions)
-
-            except AttributeError:  # pragma: no cover
-                pass  # pragma: no cover
-                # stringio will raise an attribute error here, due to with
-                # print("Cannot use this an output: %s" % str(out))
-
-    @classmethod
-    def print_to_string(cls, solutions):
-        oss = StringIO()
-        cls.print_to_stream(solutions, out=oss)
-        return oss.getvalue()
-
-
 from json import JSONEncoder
 
 
 class SolutionJSONEncoder(JSONEncoder):
     def __init__(self, **kwargs):
         # extract kwargs I know
         self.keep_zeros = None
@@ -1046,18 +1021,18 @@
         keep_zeros = sol._keep_zeros
         if self.keep_zeros is not None:
             keep_zeros = keep_zeros or self.keep_zeros
 
         for (dvar, rc) in izip_longest(model.iter_variables(), reduced_costs,
                                        fillvalue=None):
             value = sol[dvar]
-            if not keep_zeros and value == 0:
+            if not keep_zeros and not value:
                 continue
             v = {"index": "{}".format(dvar.index),
-                 "name": dvar.print_name(),
+                 "name": dvar.lp_name,
                  "value": "{}".format(value)}
             if rc is not None:
                 v["reducedCost"] = rc
             n.append(v)
         return n
```

### Comparing `docplex-2.8.125/docplex/mp/sosvarset.py` & `docplex-2.9.141/docplex/mp/sosvarset.py`

 * *Files identical despite different names*

### Comparing `docplex-2.8.125/docplex/mp/sumfn.py` & `docplex-2.9.141/docplex/mp/sumfn.py`

 * *Files identical despite different names*

### Comparing `docplex-2.8.125/docplex/mp/tck.py` & `docplex-2.9.141/docplex/mp/tck.py`

 * *Files 5% similar despite different names*

```diff
@@ -64,15 +64,15 @@
 
     def typecheck_ct_to_add(self, ct, mdl, header):
         raise NotImplementedError  # pragma: no cover
 
     def typecheck_linear_constraint(self, obj, accept_ranges=True):
         raise NotImplementedError  # pragma: no cover
 
-    def typecheck_constraint_seq(self, cts, check_linear=False):
+    def typecheck_constraint_seq(self, cts, check_linear=False, accept_range=True):
         # must return sequence unchanged
         return cts  # pragma: no cover
 
     def typecheck_zero_or_one(self, arg):
         raise NotImplementedError  # pragma: no cover
 
     def typecheck_num(self, arg, caller=None):
@@ -203,50 +203,49 @@
             self.fatal("Expecting constraint, got: {0!s} with type: {1!s}", obj, type(obj))
 
     def typecheck_ct_to_add(self, ct, mdl, header):
         if not isinstance(ct, AbstractConstraint):
             self.fatal("Expecting constraint, got: {0!r} with type: {1!s}", ct, type(ct))
         self.typecheck_in_model(mdl, ct, header)
 
-    def typecheck_linear_constraint(self, obj, accept_ranges=True):
-        if accept_ranges:
+    def typecheck_linear_constraint(self, obj, accept_range=True):
+        if accept_range:
             if not isinstance(obj, AbstractConstraint):
                 self.fatal("Expecting linear constraint, got: {0!r}", obj)
             if not obj.is_linear():
                 self.fatal("Expecting linear constraint, got: {0!s} with type: {1!s}", obj, type(obj))
         else:
             if not isinstance(obj, LinearConstraint):
                 self.fatal("Expecting linear constraint, got: {0!s} with type: {1!s}", obj, type(obj))
 
-    def typecheck_constraint_seq(self, cts, check_linear=False):
+    def typecheck_constraint_seq(self, cts, check_linear=False, accept_range=True):
         checked_cts_list = list(cts)
         for i, ct in enumerate(checked_cts_list):
             if not isinstance(ct, AbstractConstraint):
                 self.fatal("Expecting sequence of constraints, got: {0!r} at position {1}", ct, i)
-            if check_linear and not ct.is_linear():
-                self.fatal("Expecting sequence of linear constraints, got: {0!r} at position {1}", ct, i)
+            if check_linear:
+                if not ct.is_linear():
+                    self.fatal("Expecting sequence of linear constraints, got: {0!r} at position {1}", ct, i)
+                elif not accept_range and not isinstance(ct, LinearConstraint):
+                    self.fatal("Expecting sequence of linear constraints (not ranges), got: {0!r} at position {1}", ct, i)
         return checked_cts_list
 
     def typecheck_zero_or_one(self, arg):
         if arg != 0 and arg != 1:
             self.fatal("expecting 0 or 1, got: {0!s}", arg)
 
     def typecheck_num(self, arg, caller=None):
         caller_string = "{0}: ".format(caller) if caller is not None else ""
         if not is_number(arg):
             self.fatal("{0}Expecting number, got: {1!r}", caller_string, arg)
-        elif math.isnan(arg):
-            self.fatal("{0}NaN value detected", caller_string)
 
     def typecheck_int(self, arg, accept_negative=True, caller=None):
         caller_string = "{0}: ".format(caller) if caller is not None else ""
         if not is_number(arg):
             self.fatal("{0}Expecting number, got: {1!r}", caller_string, arg)
-        elif math.isnan(arg):
-            self.fatal("{0}NaN value detected", caller_string)
         elif not is_int(arg):
             self.fatal("{0}Expecting integer, got: {1!r}", caller_string, arg)
         elif not accept_negative and arg < 0:
             self.fatal("{0}Expecting positive integer, got: {1!r}", caller_string, arg)
 
     def check_vars_domain(self, lbs, ubs, names):
         l_ubs = len(ubs)
@@ -332,30 +331,29 @@
             try:
                 from inspect import signature
                 hook_signature = signature(sol_hook_fn)
                 nb_params = len(hook_signature.parameters)
                 if nb_params != 1:
                     self.fatal('Solution hook requires a function taking a solution as argument, wrong number of arguments: {0}'
                                .format(nb_params))
-            except (ImportError,TypeError):  # not a callable object or no signature
+            except (ImportError, TypeError):  # not a callable object or no signature
                 pass
 
-
     def typecheck_pwl_function(self, pwl):
         if not isinstance(pwl, PwlFunction):
             self.fatal('Expecting piecewise-linear function, {0!r} was passed', pwl)
 
-
     def check_duplicate_name(self, name, name_table, qualifier):
         if name_table is not None:
             if name in name_table:
                 self.warning("Duplicate {2} name: {0!s}, used for: {1}", name, name_table[name], qualifier)
 
 
 class NumericTypeChecker(StandardTypeChecker):
+
     def __init__(self, logger):
         StandardTypeChecker.__init__(self, logger)
 
     @staticmethod
     def static_validate_num(e, infinity=1e+20, context_msg=None):
         if not is_number(e):
             docplex_fatal("Not a number: {}".format(e))
@@ -381,14 +379,36 @@
             return infinity
         else:
             return -infinity
 
     def get_number_validation_fn(self):
         return self.static_validate_num
 
+    def typecheck_num(self, arg, caller=None):
+        caller_string = "{0}: ".format(caller) if caller is not None else ""
+        if not is_number(arg):
+            self.fatal("{0}Expecting number, got: {1!r}", caller_string, arg)
+        elif math.isnan(arg):
+            self.fatal("{0}NaN value detected", caller_string)
+        elif math.isinf(arg):
+            self.fatal("{0}Infinite value detected", caller_string)
+
+    def typecheck_int(self, arg, accept_negative=True, caller=None):
+        caller_string = "{0}: ".format(caller) if caller is not None else ""
+        if not is_number(arg):
+            self.fatal("{0}Expecting number, got: {1!r}", caller_string, arg)
+        elif math.isnan(arg):
+            self.fatal("{0}NaN value detected", caller_string)
+        elif math.isinf(arg):
+            self.fatal("{0}Infinite value detected", caller_string)
+        elif not is_int(arg):
+            self.fatal("{0}Expecting integer, got: {1!r}", caller_string, arg)
+        elif not accept_negative and arg < 0:
+            self.fatal("{0}Expecting positive integer, got: {1!r}", caller_string, arg)
+
 
 class DummyTypeChecker(IDocplexTypeChecker):
     # noinspection PyUnusedLocal
     def __init__(self, logger):
         pass
 
     def typecheck_iterable(self, arg):
@@ -417,18 +437,18 @@
 
     def typecheck_constraint(self, obj):
         pass  # pragma: no cover
 
     def typecheck_ct_to_add(self, ct, mdl, header):
         pass  # pragma: no cover
 
-    def typecheck_linear_constraint(self, obj, accept_ranges=True):
+    def typecheck_linear_constraint(self, obj, accept_range=True):
         pass  # pragma: no cover
 
-    def typecheck_constraint_seq(self, cts, check_linear=False):
+    def typecheck_constraint_seq(self, cts, check_linear=False, accept_range=True):
         # must return sequence unchanged
         return cts  # pragma: no cover
 
     def typecheck_zero_or_one(self, arg):
         pass  # pragma: no cover
 
     def typecheck_num(self, arg, caller=None):
```

### Comparing `docplex-2.8.125/docplex/mp/utils.py` & `docplex-2.9.141/docplex/mp/utils.py`

 * *Files 11% similar despite different names*

```diff
@@ -13,31 +13,37 @@
 import tempfile
 import threading
 import time
 import sys
 
 from six import PY2 as SIX_PY2
 from six import itervalues
+import six
 
+try:
+    import pandas
+except ImportError:
+    pandas = False
 
 from docplex.mp.compat23 import Queue
 from docplex.mp.compat23 import izip
+from docplex.util.environment import get_environment
 
 __int_types = {int}
 __float_types = {float}
 __numpy_ndslot_type = None
 __numpy_matrix_type = None
 __pandas_series_type = None
 __pandas_dataframe_type = None
 __spark_dataframe_type = None
 
 try:
-    type(long)
+    type(long)  # @UndefinedVariable
     # long is indeed a type we are in Python2,
-    __int_types.add(long)
+    __int_types.add(long)  # @UndefinedVariable
 except NameError:  # pragma: no cover
     # long is not a type, do nothing
     pass  # pragma: no cover
 
 try:
     import numpy
 
@@ -81,17 +87,17 @@
     __pandas_dataframe_type = DataFrame
 except ImportError:
     __pandas_series_type = None
     __pandas_dataframe_type = None
 
 # 'findspark' must be executed if running in Windows environment, before importing Spark
 try:
-    import findspark
+    import findspark  # @UnresolvedImport
     findspark.init()
-except (ImportError, IndexError):
+except (ImportError, IndexError, ValueError):
     pass
 
 try:
     import pyspark
 
     __spark_dataframe_type = pyspark.sql.dataframe.DataFrame
 except ImportError:
@@ -201,15 +207,15 @@
 
 def is_spark_dataframe(s):
     return __spark_dataframe_type and isinstance(s, __spark_dataframe_type)
 
 
 string_types = {str}
 if SIX_PY2:
-    string_types.add(unicode)
+    string_types.add(unicode)  # @UndefinedVariable
 string_types = frozenset(string_types)
 
 
 def is_string(e):
     return type(e) in string_types
 
 def has_len(e):
@@ -310,14 +316,21 @@
 class DOcplexLimitsExceeded(DOcplexException):
     cplexce_limits_exceeded_msg = "**** Promotional version. Problem size limits exceeded, CPLEX code=1016"
 
     def __init__(self):
         DOcplexException.__init__(self, self.cplexce_limits_exceeded_msg)
 
 
+class DocplexQuadToLinearException(DOcplexException):
+
+    def __init__(self, q):
+        msg = "Quadratic expression [{0!s}] cannot be converted to a linear expression".format(q)
+        DOcplexException.__init__(self, msg)
+
+
 def normalize_basename(s, force_lowercase=True, maxlen=255):
     """Replaces some characters from s with a translation table:
     
      trans_table = {" ": "_",
                    "/": "_slash_",
                    "\\": "_backslash_",
                    "?": "_question_",
@@ -516,14 +529,22 @@
 
 
 def write_csv_line(output, line, encoding):
     l = ','.join([encode_csv_string('%s' % c) for c in line])
     output.write(l.encode(encoding))
     output.write('\n'.encode(encoding))
 
+def write_csv(env, table, fields, name):
+    # table must be a named tuple
+    encoding = 'utf-8'
+    with env.get_output_stream(name) as ostr:
+        write_csv_line(ostr, fields, encoding)
+        for line in table:
+            write_csv_line(ostr, line, encoding)
+
 
 def write_kpis(env, kpis_table, name):
     '''Writes a kpis dataframe as file which name is specified.
     The data type depends of extension of name.
 
     This uses the specfied env to write data as attachments
     '''
@@ -832,31 +853,39 @@
         self._obj_iter = obj_iter
         self._index_map = None
         self.cplex_scope = cplex_scope
 
     def _make_index_map(self):
         return {m.get_index(): m for m in self._obj_iter()}
 
+    def number_of_objects(self):
+        idxmap = self._index_map
+        return 0 if idxmap is None else len(idxmap)
+
     @property
     def iter(self):
         return self._obj_iter()
 
     def __call__(self, idx):
         return self._object_by_index(idx)
 
     def get_object_by_index(self, idx, checker=None):
         if checker:
             checker.typecheck_valid_index(idx)
         return self._object_by_index(idx)
 
-    def _object_by_index(self, idx):
+    def _object_by_index(self, idx, do_raise=False):
         if self._index_map is None:
             self._index_map = self._make_index_map()
         # do not raise when not found, return None.
-        return self._index_map.get(idx)
+        if do_raise:
+            return self._index_map[idx]
+        else:
+            # returns None if idx not in map
+            return self._index_map.get(idx)
 
     def reset(self):
         _AutomaticSymbolGenerator.reset(self)
         self._index_map = None
 
     def notify_obj_index(self, obj, index):
         _AutomaticSymbolGenerator.notify_new_index(self, index)
@@ -955,7 +984,114 @@
         # s is supposed to be a string
         output_s = s
         if self.stream_is_binary:
             output_s = s.encode(self.encoding)
         self.stream.write(output_s)
 
 
+def get_auto_publish_names(context, prop_name, default_name):
+    # comparing auto_publish to boolean values because it can be a non-boolean
+    if context.solver.auto_publish is True:
+        return [default_name]
+    elif context.solver.auto_publish is False:
+        return None
+    if prop_name in context.solver.auto_publish:
+        name = context.solver.auto_publish[prop_name]
+    else:
+        name = None
+    if isinstance(name, six.string_types):
+        # only one string value: make this the name of the table
+        # in a list with one object
+        name = [name]
+    elif name is True:
+        # if true, then use default name:
+        name = [default_name]
+    elif name is False:
+        # Need to compare explicitely to False
+        name = None
+    else:
+        # otherwise the kpi_table_name can be a collection-like of names,
+        # just return it
+        pass
+    return name
+
+
+def identity_func(x):
+    return x
+
+
+def value_if_defined(obj, property, default=None):
+    value = getattr(obj, property) if hasattr(obj, property) else None
+    return value if value is not None else default
+
+
+class PublishResultAsDf(object):
+    '''Mixin for classes publishing a result as data frame
+    '''
+    def write_output_table(self, df, context,
+                           output_property_name=None,
+                           output_name=None):
+        '''Publishes the output `df`.
+
+        The `context` is used to control the output name:
+
+            - If context.solver.auto_publish is true, the `df` is written using
+            output_name.
+            - If context.solver.auto_publish is false, This method does nothing.
+            - If context.solver.auto_publish.output_property_name is true,
+               then `df` is written using output_name.
+            - If context.solver.auto_publish.output_propert_name is None or
+            False, this method does nothing.
+            - If context.solver.auto_publish.output_propert_name is a string,
+            it is used as a name to publish the df
+
+        Example:
+
+            A solver can be defined as publishing a result as data frame::
+
+                class SomeSolver(PublishResultAsDf)
+                   def __init__(self, output_customizer):
+                      # output something if context.solver.autopublish.somesolver_output is set
+                      self.output_table_property_name = 'somesolver_output'
+                      # output filename unless specified by somesolver_output:
+                      self.default_output_table_name = 'somesolver.csv'
+                      # customizer if users wants one
+                      self.output_table_customizer = output_customizer
+                      # uses pandas.DataFrame if possible, otherwise will use namedtuples
+                      self.output_table_using_df = True
+
+                    def solve(self):
+                        # do something here and return a result as a df
+                        result = pandas.DataFrame(columns=['A','B','C'])
+                        return result
+
+            Example usage::
+
+               solver = SomeSolver()
+               results = solver.solve()
+               solver.write_output_table(results)
+
+        '''
+        prop = value_if_defined(self, 'output_table_property_name')
+        prop = output_property_name if output_property_name else prop
+        default_name = value_if_defined(self, 'default_output_table_name')
+        default_name = output_name if output_name else default_name
+        names = get_auto_publish_names(context, prop, default_name)
+        use_df = value_if_defined(self, 'output_table_using_df', True)
+        if names:
+            env = get_environment()
+            customizer = value_if_defined(self, 'output_table_customizer', identity_func)
+            for name in names:
+                r = customizer(df)
+                if pandas and use_df:
+                    env.write_df(r, name)
+                else:
+                    # assume r is a namedtuple
+                    write_csv(env, r, r[0]._fields, name)
+
+
+    def is_publishing_output_table(self, context):
+        prop = value_if_defined(self, 'output_table_property_name')
+        default_name = value_if_defined(self, 'default_output_table_name')
+        names = get_auto_publish_names(context, prop, default_name)
+        return names
+
```

### Comparing `docplex-2.8.125/docplex/mp/vartype.py` & `docplex-2.9.141/docplex/mp/vartype.py`

 * *Files identical despite different names*

### Comparing `docplex-2.8.125/docplex/mp/xcounter.py` & `docplex-2.9.141/docplex/mp/xcounter.py`

 * *Files identical despite different names*

### Comparing `docplex-2.8.125/docplex/util/dods/executor.py` & `docplex-2.9.141/docplex/util/dods/executor.py`

 * *Files identical despite different names*

### Comparing `docplex-2.8.125/docplex/util/dods/project_handler.py` & `docplex-2.9.141/docplex/util/dods/project_handler.py`

 * *Files identical despite different names*

### Comparing `docplex-2.8.125/docplex/util/__init__.py` & `docplex-2.9.141/docplex/util/__init__.py`

 * *Files identical despite different names*

### Comparing `docplex-2.8.125/docplex/util/environment.py` & `docplex-2.9.141/docplex/util/environment.py`

 * *Files 2% similar despite different names*

```diff
@@ -356,41 +356,40 @@
         ''' Write a ``pandas.DataFrame`` as an output of the program.
 
         ``pandas`` must be installed.
 
         ``name`` is the name of the input object, as a filename. If a writer
         is not user provided, the writer used depends on the filename extension.
 
-        The default writer used depending on extension are:
-
-            * ``.csv``: ``DataFrame.to_csv()``
-            * ``.msg``: ``DataFrame.to_msgpack()``
+        This currently only supports csv output.
 
         Args:
             name: The name of the input object
             writer: an optional writer function
             **kwargs: additional parameters passed to the writer
         Raises:
             NotAvailableError: raises this error when ``pandas`` is not
                 available.
         '''
         if pandas is None:
             raise NotAvailableError('write_df() is only available if pandas is installed')
         _, ext = os.path.splitext(name)
         if writer is None:
             try:
-                default_writers = {'.csv': df.to_csv,
-                                   '.msg': df.to_msgpack}
+                default_writers = {'.csv': df.to_csv}
                 writer = default_writers.get(ext.lower(), None)
             except AttributeError:
                 raise NotAvailableError('Could not write writer function for extension: %s' % ext)
         if writer is None:
             raise ValueError('no default writer defined for files with extension: \'%s\'' % ext)
         with self.get_output_stream(name) as ost:
-            writer(ost, **kwargs)
+            if sys.version_info[0] < 3:
+                ost.write(writer(index=False, encoding='utf8'))
+            else:
+                ost.write(writer(index=False).encode(encoding='utf8'))
 
     def set_output_attachment(self, name, filename):
         '''Attach the file which filename is specified as an output of the
         program.
 
         The file is recorded as being part of the program output.
         This method can be called multiple times if the program contains
@@ -645,14 +644,30 @@
 
 class LocalEnvironment(Environment):
     # The environment solving environment using all local input and outputs.
     def __init__(self):
         super(LocalEnvironment, self).__init__()
         self.logger = None
 
+        # init number of cores. Default is no limits (engines will use
+        # number of cores reported by system).
+        # On Watson studio runtimes, the system reports the total number
+        # of physical cores but not the number of cores available to the
+        # runtime. The number of cores available to the runtime are
+        # specified in an environment variable instead.
+        self._available_cores = None
+        RUNTIME_HARDWARE_SPEC = os.environ.get('RUNTIME_HARDWARE_SPEC', None)
+        if RUNTIME_HARDWARE_SPEC:
+            try:
+                spec = json.loads(RUNTIME_HARDWARE_SPEC)
+                num = int(spec.get('num_cpu')) if ('num_cpu' in spec) else None
+                self._available_cores = num
+            except:
+                pass
+
     def get_input_stream(self, name):
         return open(name, "rb")
 
     def get_output_stream(self, name):
         return open(name, "wb")
 
     def get_parameter(self, name):
@@ -671,14 +686,16 @@
             shutil.copyfile(filename, name)  # copy to current
 
     def get_logger(self):
         if not self.logger:  # lazy init
             self.logger = LoggerToFile(sys.stdout)
         return self.logger
 
+    def get_available_core_count(self):
+        return self._available_cores
 
 class OutputFileWrapper(object):
     # Wraps a file object so that on __exit__() and on close(), the wrapped file is closed and
     # the output attachments are actually set in the worker
     def __init__(self, file, solve_hook, attachment_name):
         self.file = file
         self.solve_hook = solve_hook
```

### Comparing `docplex-2.8.125/docplex/util/logging_utils.py` & `docplex-2.9.141/docplex/util/logging_utils.py`

 * *Files identical despite different names*

### Comparing `docplex-2.8.125/docplex/util/status.py` & `docplex-2.9.141/docplex/util/status.py`

 * *Files identical despite different names*

### Comparing `docplex-2.8.125/docplex/__init__.py` & `docplex-2.9.141/docplex/__init__.py`

 * *Files identical despite different names*

### Comparing `docplex-2.8.125/docplex/cli.py` & `docplex-2.9.141/docplex/cli.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,12 +1,13 @@
-'''
-A command line interface / client for DOcplexcloud.
+# --------------------------------------------------------------------------
+# Source file provided under Apache License, Version 2.0, January 2004,
+# http://www.apache.org/licenses/
+# (c) Copyright IBM Corp. 2015, 2018
+# --------------------------------------------------------------------------
 
-@author: kong
-'''
 from __future__ import print_function
 
 import argparse
 import datetime
 import json
 import os.path
 from os.path import basename
@@ -100,16 +101,16 @@
         st = "<ul>"
         for item in self:
             st += "<li>%s</lu" % item
         st += "</ul>"
         return st
 
 
-def ls_jobs(client, program_result, quiet=False):
-    jobs = client.get_all_jobs()
+def ls_jobs(client, program_result, quiet=False, selected_jobs=None):
+    jobs = selected_jobs if selected_jobs else client.get_all_jobs()
     if ip:
         result = []
     for i, j in enumerate(jobs):
         jobid = j["_id"]
         date = datetime.datetime.fromtimestamp(j['createdAt'] / 1e3)
         if ip:
             in_att = list_with_html_repr()
@@ -198,15 +199,15 @@
                     del xkwargs['continuous_logs']
                     response = client.execute(**xkwargs)
                 else:
                     raise
         except TypeError as te:
             if 'execute() got an unexpected keyword argument \'info_cb\'' in te:
                 print('Your version of docplexcloud client does not support details polling (--details option). Please update')
-                sys.exit(-1)
+                return(-1)
             else:
                 raise
         if response.execution_status != JobExecutionStatus.PROCESSED:
             print("Execution failed.\nDetails:\n%s" % json.dumps(response.job_info, sort_keys=True, indent=4))
         log_items = client.get_log_items(response.jobid)
         if not continuous_logs_available:
             # download and print logs if the continuous log feature was not available
@@ -241,17 +242,30 @@
     epilog_cli = '''
   execute        Submit a job and wait for end of execution. Each ARG that
                  is a file is uploaded as the job input. Example:
                     Example: python run.py execute model.py model.data -v
                       executes a job which input files are model.py and
                       model.dada, in verbose mode.
 '''
+    filter_help = '''
 
+   Within filters, the following variables are defined:
+      now: current date and time as timestamp in millisec
+      minute: 60 sec in millisec
+      hour: 60 minutes in millisec
+      day: 24 hour in millisec
+      job: The current job being filtered
+
+    Example filter usage:
+        Delete all jobs older than 3 hour
+        python -m docplex.cli --filter "now-job['startedAt'] > 3*hour " rm
+'''
     if ip is None:
         epilog += epilog_cli
+    epilog += filter_help
     parser = argparse.ArgumentParser(prog=prog, description=description, epilog=epilog,
                                      formatter_class=argparse.RawDescriptionHelpFormatter)
     parser.add_argument('command',
                         metavar='COMMAND',
                         help='DOcplexcloud command')
     parser.add_argument('arguments', metavar='ARG', nargs='*',
                         help='Arguments for the command')
@@ -262,19 +276,21 @@
                         help='Verbose mode')
     parser.add_argument('--as', nargs=1, metavar='HOST',
                         dest="host_config", default=None,
                         help="'as host' - use the cplex_config_<HOST>.py configuration file found in PYTHONPATH")
     parser.add_argument('--url', nargs=1, metavar='URL',
                         dest="url", default=None,
                         help="The DOcplexcloud connection URL. If not specified, will use those found in docplex config files")
-    parser.add_argument('--key', nargs=1, metavar='API_KEY',
+    parser.add_argument('--key', metavar='API_KEY',
                         dest="key", default=None,
                         help="The DOcplexcloud connection key. If not specified, will use those found in docplex config files")
     parser.add_argument('--details', action='store_true', default=False,
                         help='Display solve details as they are available')
+    parser.add_argument('--filter', metavar='FILTER',  default=None,
+                        help='filter on job. Example: --filter "True if (now-job.createdAt) > 3600"')
     parser.add_argument('--quiet', '-q', action='store_true', default=False,
                         help='Only show numeric IDs as output')
     args = parser.parse_args(argv)
 
     program_result = ProgramResults()
 
     # Get the context here so that we have some credentials at hand
@@ -305,47 +321,97 @@
         print('Arguments:')
         for i in args.arguments:
             print('  -> %s' % i)
         print('verbose = %s' % args.verbose)
 
     client = JobClient(client_url, client_key)
 
+    target_jobs = []
+    if args.filter:
+        jobs = client.get_all_jobs()
+        now = (datetime.datetime.now() - datetime.datetime(1970,1,1)).total_seconds() * 1000.0
+        minute = 60 * 1000
+        hour = 60 * minute
+        day = 24 * hour
+        context = {'now': now,
+                   'minute': minute,
+                   'hour': hour,
+                   'day': day,
+                  }
+        for j in jobs:
+            context['job'] = j
+            keep = False
+            try:
+                keep = eval(args.filter, globals(), context)
+            except KeyError:  # if a key was not foud, just assume expression is false
+                keep = False
+            if keep:
+                target_jobs.append(j)
+
+    if target_jobs:
+        for i in target_jobs:
+            print('applying to %s' % i['_id'])
+
     if args.command == 'ls':
-        ls_jobs(client, program_result, quiet=args.quiet)
+        ls_jobs(client, program_result, quiet=args.quiet, selected_jobs=target_jobs)
     elif args.command == 'info':
-        if len(args.arguments) == 1 and args.arguments[0] == 'all':
+        if target_jobs:
+            args.arguments = [x["_id"] for x in target_jobs]
+        elif len(args.arguments) == 1 and args.arguments[0] == 'all':
             args.arguments = [x["_id"] for x in client.get_all_jobs()]
         for id in args.arguments:
             info_text = "NOT FOUND"
             try:
                 job = client.get_job(id)
                 info_text = json.dumps(job, indent=3)
             except:
                 pass
             print("%s:\n%s" % (id, info_text))
     elif args.command == 'rm':
-        if args.arguments:
+        if target_jobs:
+            joblist = [x["_id"] for x in target_jobs]
+        elif args.arguments:
             joblist = args.arguments
         else:
             joblist = shlex.split(sys.stdin.read())
         rm_job(client, joblist, verbose=args.verbose)
     elif args.command == 'logs':
+        if target_jobs:
+            if len(target_jobs) != 1:
+                print('Logs can only be retrieved when filter select one job (actual selection count = %s)' % len(target_jobs))
+                program_result.return_code = -1
+                return(program_result)
+            args.arguments = [x["_id"] for x in target_jobs]
+        if not args.arguments:
+            print('Please specify job list in arguments or using filter.')
+            program_result.return_code = -1
+            return(program_result)
         for jid in args.arguments:
             log_items = client.get_log_items(jid)
             for log in log_items:
                 for record in log["records"]:
                     print(record["message"])
     elif args.command == 'download':
+        if target_jobs:
+            if len(target_jobs) != 1:
+                print('Jobs can only be downloaded when filter select one job (actual selection count = %s)' % len(target_jobs))
+                program_result.return_code = -1
+                return(program_result)
+            args.arguments = [x["_id"] for x in target_jobs]
         for jid in args.arguments:
             job = client.get_job(jid)
             for attachment in job['attachments']:
                 print('downloading %s' % attachment['name'])
                 with open(attachment['name'], 'wb') as f:
                     f.write(client.download_job_attachment(id, attachment['name']))
     elif args.command == 'execute':
+        if target_jobs:
+            print('Execute command does not support job filtering')
+            program_result.return_code = -1
+            return(program_result)
         inputs = [{'name': basename(a), 'filename': a} for a in args.arguments]
         if args.verbose:
             for i in inputs:
                 print("Uploading %s as attachment name %s" % (i['filename'], i['name']))
         execute_job(client, inputs, args.verbose, args.details, args.nodelete)
     else:
         print("Unknown command: %s" % args.command)
```

### Comparing `docplex-2.8.125/CHANGELOG.rst` & `docplex-2.9.141/CHANGELOG.rst`

 * *Files 3% similar despite different names*

```diff
@@ -1,23 +1,37 @@
 Changelog
 ---------
 
+Changed in 2.9.141:
+```````````````````
+* In ``docplex.mp``:
+   * Removed links to rawgit.com as this service is going end of life.
+   * Model.solve_lexicographic() is deprecated. This method should be used
+     to perform lexicographic solve with COS 12.8, but with COS 12.9,
+     Model.set_multi_objective() should be used for solving problems
+     with multiple objectives.
+
+* In ``docplex.cp``:
+   * Add KPIs supported by CPO Solver 12.9
+   * Update CPO parser to read KPIs section for format 12.9
+   * Add new examples with KPIs.
+
+
 Changed in 2.8.125:
 ```````````````````
-* Solving with solver agent 'docloud' is deprecated. Models are now preferably
-  solved with local solver or the python source can be submitted to DOcplexcloud
-  solve service. See https://ibm.biz/BdYhhK
+* Solving with solver agent 'docloud' is deprecated. 
+  Models are now preferably solved with local solver, or the python source can be submitted to DOcplexcloud solve service. 
+  See https://ibm.biz/BdYhhK.
 
 * In ``docplex.mp``:
    * solve_lexicographic is being deprecated. In a future version, a new api will be available to support multi-objectives.
 
 * In ``docplex.cp``:
    * Fix problem with boolean indicators in no_overlap(), always_constant() and always_equal().
    * Allow model solution to be used directly as a starting point (ignores what is not integer or interval var).
-   * Add new examples with KPIs.
    * Add methods domain_min(), domain_max(), domain_iterator() and domain_contains() on both CpoIntVar and CpoIntVarSolution.
    * Default solver agent is now 'local' instead of 'docloud'. All examples modified consequently.
 
 
 Changed in 2.7.113:
 ```````````````````
```

### Comparing `docplex-2.8.125/LICENSE.txt` & `docplex-2.9.141/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `docplex-2.8.125/README.rst` & `docplex-2.9.141/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 your computer with IBM® ILOG CPLEX Optimization Studio.
 
 This library is composed of 2 modules:
 
     * IBM® Decision Optimization CPLEX Optimizer Modeling for Python - with namespace docplex.mp
     * IBM® Decision Optimization CP Optimizer Modeling for Python - with namespace docplex.cp
 
-Solving with CPLEX locally requires that IBM® ILOG CPLEX Optimization Studio V12.7.1 or V12.8
+Solving with CPLEX locally requires that IBM® ILOG CPLEX Optimization Studio V12.8 or V12.9
 is installed on your machine.
 
 Solving with the IBM® Decision Optimization on Cloud service requires that you
 register for an account and get the API key.
 
 This library is `numpy` friendly.
```

### Comparing `docplex-2.8.125/setup.py` & `docplex-2.9.141/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -18,15 +18,15 @@
         with open(os.path.join(HERE, *parts)) as f:
             return f.read()
     except:
         return None
 
 readme = read('README.rst')
 if readme is None:
-    readme = 'DOcplex 2.8'
+    readme = 'DOcplex 2.9'
 
 changelog = str(read('CHANGELOG.rst'))
 if changelog is None:
     changelog = ''
 
 ss = str(readme) + str(changelog)
 
@@ -41,15 +41,15 @@
                'docplex.mp.internal',
                'docplex.mp.params',
                'docplex.mp.sktrans',
                'docplex.mp.sparktrans',
                'docplex.mp.worker',
                'docplex.util',
                'docplex.util.dods'],
-    version = '2.8.125',  # replaced at build time
+    version = '2.9.141',  # replaced at build time
     description = 'The IBM Decision Optimization CPLEX Modeling for Python',
     author = 'The IBM Decision Optimization on Cloud team',
     author_email = 'dofeedback@wwpdl.vnet.ibm.com',
     long_description='%s\n' % ss,
     url = 'https://onboarding-oaas.docloud.ibmcloud.com/software/analytics/docloud/',
     keywords = ['docloud', 'optimization', 'cplex', 'cpo'],
     license = read('LICENSE.txt'),
```

### Comparing `docplex-2.8.125/PKG-INFO` & `docplex-2.9.141/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: docplex
-Version: 2.8.125
+Version: 2.9.141
 Summary: The IBM Decision Optimization CPLEX Modeling for Python
 Home-page: https://onboarding-oaas.docloud.ibmcloud.com/software/analytics/docloud/
 Author: The IBM Decision Optimization on Cloud team
 Author-email: dofeedback@wwpdl.vnet.ibm.com
 License: 
                                  Apache License
                            Version 2.0, January 2004
@@ -220,15 +220,15 @@
         your computer with IBM® ILOG CPLEX Optimization Studio.
         
         This library is composed of 2 modules:
         
             * IBM® Decision Optimization CPLEX Optimizer Modeling for Python - with namespace docplex.mp
             * IBM® Decision Optimization CP Optimizer Modeling for Python - with namespace docplex.cp
         
-        Solving with CPLEX locally requires that IBM® ILOG CPLEX Optimization Studio V12.7.1 or V12.8
+        Solving with CPLEX locally requires that IBM® ILOG CPLEX Optimization Studio V12.8 or V12.9
         is installed on your machine.
         
         Solving with the IBM® Decision Optimization on Cloud service requires that you
         register for an account and get the API key.
         
         This library is `numpy` friendly.
         
@@ -240,27 +240,41 @@
         ------------
         
         *  ``pip install docplex``
         
         Changelog
         ---------
         
+        Changed in 2.9.141:
+        ```````````````````
+        * In ``docplex.mp``:
+           * Removed links to rawgit.com as this service is going end of life.
+           * Model.solve_lexicographic() is deprecated. This method should be used
+             to perform lexicographic solve with COS 12.8, but with COS 12.9,
+             Model.set_multi_objective() should be used for solving problems
+             with multiple objectives.
+        
+        * In ``docplex.cp``:
+           * Add KPIs supported by CPO Solver 12.9
+           * Update CPO parser to read KPIs section for format 12.9
+           * Add new examples with KPIs.
+        
+        
         Changed in 2.8.125:
         ```````````````````
-        * Solving with solver agent 'docloud' is deprecated. Models are now preferably
-          solved with local solver or the python source can be submitted to DOcplexcloud
-          solve service. See https://ibm.biz/BdYhhK
+        * Solving with solver agent 'docloud' is deprecated. 
+          Models are now preferably solved with local solver, or the python source can be submitted to DOcplexcloud solve service. 
+          See https://ibm.biz/BdYhhK.
         
         * In ``docplex.mp``:
            * solve_lexicographic is being deprecated. In a future version, a new api will be available to support multi-objectives.
         
         * In ``docplex.cp``:
            * Fix problem with boolean indicators in no_overlap(), always_constant() and always_equal().
            * Allow model solution to be used directly as a starting point (ignores what is not integer or interval var).
-           * Add new examples with KPIs.
            * Add methods domain_min(), domain_max(), domain_iterator() and domain_contains() on both CpoIntVar and CpoIntVarSolution.
            * Default solver agent is now 'local' instead of 'docloud'. All examples modified consequently.
         
         
         Changed in 2.7.113:
         ```````````````````
```

