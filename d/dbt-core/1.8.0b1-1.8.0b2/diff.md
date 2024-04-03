# Comparing `tmp/dbt-core-1.8.0b1.tar.gz` & `tmp/dbt-core-1.8.0b2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dbt-core-1.8.0b1.tar", last modified: Wed Feb 28 23:34:21 2024, max compression
+gzip compressed data, was "dbt-core-1.8.0b2.tar", last modified: Wed Apr  3 15:20:18 2024, max compression
```

## Comparing `dbt-core-1.8.0b1.tar` & `dbt-core-1.8.0b2.tar`

### file list

```diff
@@ -1,262 +1,262 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 23:34:21.019235 dbt-core-1.8.0b1/
--rw-r--r--   0 runner    (1001) docker     (127)      139 2024-02-28 23:34:09.000000 dbt-core-1.8.0b1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     3916 2024-02-28 23:34:21.019235 dbt-core-1.8.0b1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2365 2024-02-28 23:34:09.000000 dbt-core-1.8.0b1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 23:34:20.979235 dbt-core-1.8.0b1/dbt/
--rw-r--r--   0 runner    (1001) docker     (127)      341 2024-02-28 23:34:09.000000 dbt-core-1.8.0b1/dbt/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 23:34:20.979235 dbt-core-1.8.0b1/dbt/artifacts/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-28 23:34:09.000000 dbt-core-1.8.0b1/dbt/artifacts/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 23:34:20.979235 dbt-core-1.8.0b1/dbt/artifacts/resources/
--rw-r--r--   0 runner    (1001) docker     (127)     2669 2024-02-28 23:34:09.000000 dbt-core-1.8.0b1/dbt/artifacts/resources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1779 2024-02-28 23:34:09.000000 dbt-core-1.8.0b1/dbt/artifacts/resources/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     1498 2024-02-28 23:34:09.000000 dbt-core-1.8.0b1/dbt/artifacts/resources/types.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 23:34:20.983235 dbt-core-1.8.0b1/dbt/artifacts/resources/v1/
--rw-r--r--   0 runner    (1001) docker     (127)      272 2024-02-28 23:34:09.000000 dbt-core-1.8.0b1/dbt/artifacts/resources/v1/analysis.py
--rw-r--r--   0 runner    (1001) docker     (127)     6870 2024-02-28 23:34:09.000000 dbt-core-1.8.0b1/dbt/artifacts/resources/v1/components.py
--rw-r--r--   0 runner    (1001) docker     (127)     9586 2024-02-28 23:34:09.000000 dbt-core-1.8.0b1/dbt/artifacts/resources/v1/config.py
--rw-r--r--   0 runner    (1001) docker     (127)      290 2024-02-28 23:34:09.000000 dbt-core-1.8.0b1/dbt/artifacts/resources/v1/documentation.py
--rw-r--r--   0 runner    (1001) docker     (127)     1555 2024-02-28 23:34:09.000000 dbt-core-1.8.0b1/dbt/artifacts/resources/v1/exposure.py
--rw-r--r--   0 runner    (1001) docker     (127)     1209 2024-02-28 23:34:09.000000 dbt-core-1.8.0b1/dbt/artifacts/resources/v1/generic_test.py
--rw-r--r--   0 runner    (1001) docker     (127)      332 2024-02-28 23:34:09.000000 dbt-core-1.8.0b1/dbt/artifacts/resources/v1/group.py
--rw-r--r--   0 runner    (1001) docker     (127)      315 2024-02-28 23:34:09.000000 dbt-core-1.8.0b1/dbt/artifacts/resources/v1/hook.py
--rw-r--r--   0 runner    (1001) docker     (127)     1003 2024-02-28 23:34:09.000000 dbt-core-1.8.0b1/dbt/artifacts/resources/v1/macro.py
--rw-r--r--   0 runner    (1001) docker     (127)     4728 2024-02-28 23:34:09.000000 dbt-core-1.8.0b1/dbt/artifacts/resources/v1/metric.py
--rw-r--r--   0 runner    (1001) docker     (127)     1079 2024-02-28 23:34:09.000000 dbt-core-1.8.0b1/dbt/artifacts/resources/v1/model.py
--rw-r--r--   0 runner    (1001) docker     (127)      260 2024-02-28 23:34:09.000000 dbt-core-1.8.0b1/dbt/artifacts/resources/v1/owner.py
--rw-r--r--   0 runner    (1001) docker     (127)     2827 2024-02-28 23:34:09.000000 dbt-core-1.8.0b1/dbt/artifacts/resources/v1/saved_query.py
--rw-r--r--   0 runner    (1001) docker     (127)     1168 2024-02-28 23:34:09.000000 dbt-core-1.8.0b1/dbt/artifacts/resources/v1/seed.py
--rw-r--r--   0 runner    (1001) docker     (127)     1327 2024-02-28 23:34:09.000000 dbt-core-1.8.0b1/dbt/artifacts/resources/v1/semantic_layer_components.py
--rw-r--r--   0 runner    (1001) docker     (127)     8913 2024-02-28 23:34:09.000000 dbt-core-1.8.0b1/dbt/artifacts/resources/v1/semantic_model.py
--rw-r--r--   0 runner    (1001) docker     (127)      523 2024-02-28 23:34:09.000000 dbt-core-1.8.0b1/dbt/artifacts/resources/v1/singular_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2909 2024-02-28 23:34:09.000000 dbt-core-1.8.0b1/dbt/artifacts/resources/v1/snapshot.py
--rw-r--r--   0 runner    (1001) docker     (127)     2385 2024-02-28 23:34:09.000000 dbt-core-1.8.0b1/dbt/artifacts/resources/v1/source_definition.py
--rw-r--r--   0 runner    (1001) docker     (127)      280 2024-02-28 23:34:09.000000 dbt-core-1.8.0b1/dbt/artifacts/resources/v1/sql_operation.py
--rw-r--r--   0 runner    (1001) docker     (127)     2369 2024-02-28 23:34:09.000000 dbt-core-1.8.0b1/dbt/artifacts/resources/v1/unit_test_definition.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 23:34:20.983235 dbt-core-1.8.0b1/dbt/artifacts/schemas/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-28 23:34:09.000000 dbt-core-1.8.0b1/dbt/artifacts/schemas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6404 2024-02-28 23:34:09.000000 dbt-core-1.8.0b1/dbt/artifacts/schemas/base.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 23:34:20.983235 dbt-core-1.8.0b1/dbt/artifacts/schemas/catalog/
--rw-r--r--   0 runner    (1001) docker     (127)       81 2024-02-28 23:34:09.000000 dbt-core-1.8.0b1/dbt/artifacts/schemas/catalog/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 23:34:20.983235 dbt-core-1.8.0b1/dbt/artifacts/schemas/catalog/v1/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-28 23:34:09.000000 dbt-core-1.8.0b1/dbt/artifacts/schemas/catalog/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2692 2024-02-28 23:34:09.000000 dbt-core-1.8.0b1/dbt/artifacts/schemas/catalog/v1/catalog.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 23:34:20.983235 dbt-core-1.8.0b1/dbt/artifacts/schemas/freshness/
--rw-r--r--   0 runner    (1001) docker     (127)       67 2024-02-28 23:34:09.000000 dbt-core-1.8.0b1/dbt/artifacts/schemas/freshness/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 23:34:20.987235 dbt-core-1.8.0b1/dbt/artifacts/schemas/freshness/v3/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-28 23:34:09.000000 dbt-core-1.8.0b1/dbt/artifacts/schemas/freshness/v3/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4270 2024-02-28 23:34:09.000000 dbt-core-1.8.0b1/dbt/artifacts/schemas/freshness/v3/freshness.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 23:34:20.987235 dbt-core-1.8.0b1/dbt/artifacts/schemas/manifest/
--rw-r--r--   0 runner    (1001) docker     (127)       84 2024-02-28 23:34:09.000000 dbt-core-1.8.0b1/dbt/artifacts/schemas/manifest/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 23:34:20.987235 dbt-core-1.8.0b1/dbt/artifacts/schemas/manifest/v12/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-28 23:34:09.000000 dbt-core-1.8.0b1/dbt/artifacts/schemas/manifest/v12/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5898 2024-02-28 23:34:09.000000 dbt-core-1.8.0b1/dbt/artifacts/schemas/manifest/v12/manifest.py
--rw-r--r--   0 runner    (1001) docker     (127)     4064 2024-02-28 23:34:09.000000 dbt-core-1.8.0b1/dbt/artifacts/schemas/results.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 23:34:20.987235 dbt-core-1.8.0b1/dbt/artifacts/schemas/run/
--rw-r--r--   0 runner    (1001) docker     (127)       73 2024-02-28 23:34:09.000000 dbt-core-1.8.0b1/dbt/artifacts/schemas/run/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 23:34:20.987235 dbt-core-1.8.0b1/dbt/artifacts/schemas/run/v5/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-28 23:34:09.000000 dbt-core-1.8.0b1/dbt/artifacts/schemas/run/v5/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4619 2024-02-28 23:34:09.000000 dbt-core-1.8.0b1/dbt/artifacts/schemas/run/v5/run.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 23:34:20.987235 dbt-core-1.8.0b1/dbt/artifacts/schemas/upgrades/
--rw-r--r--   0 runner    (1001) docker     (127)       82 2024-02-28 23:34:09.000000 dbt-core-1.8.0b1/dbt/artifacts/schemas/upgrades/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6898 2024-02-28 23:34:09.000000 dbt-core-1.8.0b1/dbt/artifacts/schemas/upgrades/upgrade_manifest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 23:34:20.987235 dbt-core-1.8.0b1/dbt/cli/
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-02-28 23:34:09.000000 dbt-core-1.8.0b1/dbt/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      379 2024-02-28 23:34:09.000000 dbt-core-1.8.0b1/dbt/cli/context.py
--rw-r--r--   0 runner    (1001) docker     (127)     1357 2024-02-28 23:34:09.000000 dbt-core-1.8.0b1/dbt/cli/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)    19904 2024-02-28 23:34:09.000000 dbt-core-1.8.0b1/dbt/cli/flags.py
--rw-r--r--   0 runner    (1001) docker     (127)    19041 2024-02-28 23:34:09.000000 dbt-core-1.8.0b1/dbt/cli/main.py
--rw-r--r--   0 runner    (1001) docker     (127)     2792 2024-02-28 23:34:09.000000 dbt-core-1.8.0b1/dbt/cli/option_types.py
--rw-r--r--   0 runner    (1001) docker     (127)     3520 2024-02-28 23:34:09.000000 dbt-core-1.8.0b1/dbt/cli/options.py
--rw-r--r--   0 runner    (1001) docker     (127)    21062 2024-02-28 23:34:09.000000 dbt-core-1.8.0b1/dbt/cli/params.py
--rw-r--r--   0 runner    (1001) docker     (127)    10642 2024-02-28 23:34:09.000000 dbt-core-1.8.0b1/dbt/cli/requires.py
--rw-r--r--   0 runner    (1001) docker     (127)     1247 2024-02-28 23:34:09.000000 dbt-core-1.8.0b1/dbt/cli/resolvers.py
--rw-r--r--   0 runner    (1001) docker     (127)     1006 2024-02-28 23:34:09.000000 dbt-core-1.8.0b1/dbt/cli/types.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 23:34:20.991235 dbt-core-1.8.0b1/dbt/clients/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-28 23:34:09.000000 dbt-core-1.8.0b1/dbt/clients/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5262 2024-02-28 23:34:09.000000 dbt-core-1.8.0b1/dbt/clients/git.py
--rw-r--r--   0 runner    (1001) docker     (127)     6525 2024-02-28 23:34:09.000000 dbt-core-1.8.0b1/dbt/clients/jinja.py
--rw-r--r--   0 runner    (1001) docker     (127)     5395 2024-02-28 23:34:09.000000 dbt-core-1.8.0b1/dbt/clients/jinja_static.py
--rw-r--r--   0 runner    (1001) docker     (127)     7961 2024-02-28 23:34:09.000000 dbt-core-1.8.0b1/dbt/clients/registry.py
--rw-r--r--   0 runner    (1001) docker     (127)     1729 2024-02-28 23:34:09.000000 dbt-core-1.8.0b1/dbt/clients/yaml_helper.py
--rw-r--r--   0 runner    (1001) docker     (127)    23871 2024-02-28 23:34:09.000000 dbt-core-1.8.0b1/dbt/compilation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 23:34:20.991235 dbt-core-1.8.0b1/dbt/config/
--rw-r--r--   0 runner    (1001) docker     (127)      224 2024-02-28 23:34:09.000000 dbt-core-1.8.0b1/dbt/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15551 2024-02-28 23:34:09.000000 dbt-core-1.8.0b1/dbt/config/profile.py
--rw-r--r--   0 runner    (1001) docker     (127)    31410 2024-02-28 23:34:09.000000 dbt-core-1.8.0b1/dbt/config/project.py
--rw-r--r--   0 runner    (1001) docker     (127)     8103 2024-02-28 23:34:09.000000 dbt-core-1.8.0b1/dbt/config/renderer.py
--rw-r--r--   0 runner    (1001) docker     (127)    17206 2024-02-28 23:34:09.000000 dbt-core-1.8.0b1/dbt/config/runtime.py
--rw-r--r--   0 runner    (1001) docker     (127)     7925 2024-02-28 23:34:09.000000 dbt-core-1.8.0b1/dbt/config/selectors.py
--rw-r--r--   0 runner    (1001) docker     (127)      842 2024-02-28 23:34:09.000000 dbt-core-1.8.0b1/dbt/config/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      676 2024-02-28 23:34:09.000000 dbt-core-1.8.0b1/dbt/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 23:34:20.991235 dbt-core-1.8.0b1/dbt/context/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-28 23:34:09.000000 dbt-core-1.8.0b1/dbt/context/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    23769 2024-02-28 23:34:09.000000 dbt-core-1.8.0b1/dbt/context/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     4467 2024-02-28 23:34:09.000000 dbt-core-1.8.0b1/dbt/context/configured.py
--rw-r--r--   0 runner    (1001) docker     (127)    14230 2024-02-28 23:34:09.000000 dbt-core-1.8.0b1/dbt/context/context_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     2538 2024-02-28 23:34:09.000000 dbt-core-1.8.0b1/dbt/context/docs.py
--rw-r--r--   0 runner    (1001) docker     (127)     4424 2024-02-28 23:34:09.000000 dbt-core-1.8.0b1/dbt/context/exceptions_jinja.py
--rw-r--r--   0 runner    (1001) docker     (127)     8681 2024-02-28 23:34:09.000000 dbt-core-1.8.0b1/dbt/context/macro_resolver.py
--rw-r--r--   0 runner    (1001) docker     (127)     7426 2024-02-28 23:34:09.000000 dbt-core-1.8.0b1/dbt/context/macros.py
--rw-r--r--   0 runner    (1001) docker     (127)     3044 2024-02-28 23:34:09.000000 dbt-core-1.8.0b1/dbt/context/manifest.py
--rw-r--r--   0 runner    (1001) docker     (127)    65637 2024-02-28 23:34:09.000000 dbt-core-1.8.0b1/dbt/context/providers.py
--rw-r--r--   0 runner    (1001) docker     (127)     2654 2024-02-28 23:34:09.000000 dbt-core-1.8.0b1/dbt/context/secret.py
--rw-r--r--   0 runner    (1001) docker     (127)     4165 2024-02-28 23:34:09.000000 dbt-core-1.8.0b1/dbt/context/target.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 23:34:20.995235 dbt-core-1.8.0b1/dbt/contracts/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-28 23:34:09.000000 dbt-core-1.8.0b1/dbt/contracts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10059 2024-02-28 23:34:09.000000 dbt-core-1.8.0b1/dbt/contracts/files.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 23:34:20.995235 dbt-core-1.8.0b1/dbt/contracts/graph/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-28 23:34:09.000000 dbt-core-1.8.0b1/dbt/contracts/graph/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    64188 2024-02-28 23:34:09.000000 dbt-core-1.8.0b1/dbt/contracts/graph/manifest.py
--rw-r--r--   0 runner    (1001) docker     (127)     3869 2024-02-28 23:34:09.000000 dbt-core-1.8.0b1/dbt/contracts/graph/metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)     2056 2024-02-28 23:34:09.000000 dbt-core-1.8.0b1/dbt/contracts/graph/model_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     1209 2024-02-28 23:34:09.000000 dbt-core-1.8.0b1/dbt/contracts/graph/node_args.py
--rw-r--r--   0 runner    (1001) docker     (127)    54957 2024-02-28 23:34:09.000000 dbt-core-1.8.0b1/dbt/contracts/graph/nodes.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-28 23:34:09.000000 dbt-core-1.8.0b1/dbt/contracts/graph/searcher.py
--rw-r--r--   0 runner    (1001) docker     (127)     4459 2024-02-28 23:34:09.000000 dbt-core-1.8.0b1/dbt/contracts/graph/semantic_manifest.py
--rw-r--r--   0 runner    (1001) docker     (127)    22110 2024-02-28 23:34:09.000000 dbt-core-1.8.0b1/dbt/contracts/graph/unparsed.py
--rw-r--r--   0 runner    (1001) docker     (127)     2677 2024-02-28 23:34:09.000000 dbt-core-1.8.0b1/dbt/contracts/graph/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    11569 2024-02-28 23:34:09.000000 dbt-core-1.8.0b1/dbt/contracts/project.py
--rw-r--r--   0 runner    (1001) docker     (127)     1228 2024-02-28 23:34:09.000000 dbt-core-1.8.0b1/dbt/contracts/results.py
--rw-r--r--   0 runner    (1001) docker     (127)      522 2024-02-28 23:34:09.000000 dbt-core-1.8.0b1/dbt/contracts/selection.py
--rw-r--r--   0 runner    (1001) docker     (127)     2243 2024-02-28 23:34:09.000000 dbt-core-1.8.0b1/dbt/contracts/sql.py
--rw-r--r--   0 runner    (1001) docker     (127)     3007 2024-02-28 23:34:09.000000 dbt-core-1.8.0b1/dbt/contracts/state.py
--rw-r--r--   0 runner    (1001) docker     (127)     1130 2024-02-28 23:34:09.000000 dbt-core-1.8.0b1/dbt/contracts/util.py
--rw-r--r--   0 runner    (1001) docker     (127)     4994 2024-02-28 23:34:09.000000 dbt-core-1.8.0b1/dbt/deprecations.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 23:34:20.999235 dbt-core-1.8.0b1/dbt/deps/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-28 23:34:09.000000 dbt-core-1.8.0b1/dbt/deps/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4778 2024-02-28 23:34:09.000000 dbt-core-1.8.0b1/dbt/deps/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     6438 2024-02-28 23:34:09.000000 dbt-core-1.8.0b1/dbt/deps/git.py
--rw-r--r--   0 runner    (1001) docker     (127)     2520 2024-02-28 23:34:09.000000 dbt-core-1.8.0b1/dbt/deps/local.py
--rw-r--r--   0 runner    (1001) docker     (127)     4553 2024-02-28 23:34:09.000000 dbt-core-1.8.0b1/dbt/deps/registry.py
--rw-r--r--   0 runner    (1001) docker     (127)     4889 2024-02-28 23:34:09.000000 dbt-core-1.8.0b1/dbt/deps/resolver.py
--rw-r--r--   0 runner    (1001) docker     (127)     4544 2024-02-28 23:34:09.000000 dbt-core-1.8.0b1/dbt/deps/tarball.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 23:34:20.971235 dbt-core-1.8.0b1/dbt/docs/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 23:34:20.999235 dbt-core-1.8.0b1/dbt/docs/source/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 23:34:20.999235 dbt-core-1.8.0b1/dbt/docs/source/_ext/
--rw-r--r--   0 runner    (1001) docker     (127)     3544 2024-02-28 23:34:09.000000 dbt-core-1.8.0b1/dbt/docs/source/_ext/dbt_click.py
--rw-r--r--   0 runner    (1001) docker     (127)     1060 2024-02-28 23:34:09.000000 dbt-core-1.8.0b1/dbt/docs/source/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 23:34:20.999235 dbt-core-1.8.0b1/dbt/events/
--rw-r--r--   0 runner    (1001) docker     (127)      454 2024-02-28 23:34:09.000000 dbt-core-1.8.0b1/dbt/events/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      924 2024-02-28 23:34:09.000000 dbt-core-1.8.0b1/dbt/events/base_types.py
--rw-r--r--   0 runner    (1001) docker     (127)    98081 2024-02-28 23:34:09.000000 dbt-core-1.8.0b1/dbt/events/core_types_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     3648 2024-02-28 23:34:09.000000 dbt-core-1.8.0b1/dbt/events/logging.py
--rw-r--r--   0 runner    (1001) docker     (127)    53528 2024-02-28 23:34:09.000000 dbt-core-1.8.0b1/dbt/events/types.py
--rw-r--r--   0 runner    (1001) docker     (127)    49691 2024-02-28 23:34:09.000000 dbt-core-1.8.0b1/dbt/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     3602 2024-02-28 23:34:09.000000 dbt-core-1.8.0b1/dbt/flags.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 23:34:20.999235 dbt-core-1.8.0b1/dbt/graph/
--rw-r--r--   0 runner    (1001) docker     (127)      430 2024-02-28 23:34:09.000000 dbt-core-1.8.0b1/dbt/graph/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9620 2024-02-28 23:34:09.000000 dbt-core-1.8.0b1/dbt/graph/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     5368 2024-02-28 23:34:09.000000 dbt-core-1.8.0b1/dbt/graph/graph.py
--rw-r--r--   0 runner    (1001) docker     (127)     7340 2024-02-28 23:34:09.000000 dbt-core-1.8.0b1/dbt/graph/queue.py
--rw-r--r--   0 runner    (1001) docker     (127)    14905 2024-02-28 23:34:09.000000 dbt-core-1.8.0b1/dbt/graph/selector.py
--rw-r--r--   0 runner    (1001) docker     (127)    35076 2024-02-28 23:34:09.000000 dbt-core-1.8.0b1/dbt/graph/selector_methods.py
--rw-r--r--   0 runner    (1001) docker     (127)     7229 2024-02-28 23:34:09.000000 dbt-core-1.8.0b1/dbt/graph/selector_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)      511 2024-02-28 23:34:09.000000 dbt-core-1.8.0b1/dbt/hooks.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 23:34:20.999235 dbt-core-1.8.0b1/dbt/include/
--rw-r--r--   0 runner    (1001) docker     (127)     4794 2024-02-28 23:34:09.000000 dbt-core-1.8.0b1/dbt/include/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-02-28 23:34:09.000000 dbt-core-1.8.0b1/dbt/include/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 23:34:20.999235 dbt-core-1.8.0b1/dbt/include/starter_project/
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-02-28 23:34:09.000000 dbt-core-1.8.0b1/dbt/include/starter_project/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      571 2024-02-28 23:34:09.000000 dbt-core-1.8.0b1/dbt/include/starter_project/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-02-28 23:34:09.000000 dbt-core-1.8.0b1/dbt/include/starter_project/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 23:34:20.999235 dbt-core-1.8.0b1/dbt/include/starter_project/analyses/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-28 23:34:09.000000 dbt-core-1.8.0b1/dbt/include/starter_project/analyses/.gitkeep
--rw-r--r--   0 runner    (1001) docker     (127)     1260 2024-02-28 23:34:09.000000 dbt-core-1.8.0b1/dbt/include/starter_project/dbt_project.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 23:34:21.003235 dbt-core-1.8.0b1/dbt/include/starter_project/macros/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-28 23:34:09.000000 dbt-core-1.8.0b1/dbt/include/starter_project/macros/.gitkeep
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 23:34:20.975235 dbt-core-1.8.0b1/dbt/include/starter_project/models/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 23:34:21.003235 dbt-core-1.8.0b1/dbt/include/starter_project/models/example/
--rw-r--r--   0 runner    (1001) docker     (127)      475 2024-02-28 23:34:09.000000 dbt-core-1.8.0b1/dbt/include/starter_project/models/example/my_first_dbt_model.sql
--rw-r--r--   0 runner    (1001) docker     (127)      115 2024-02-28 23:34:09.000000 dbt-core-1.8.0b1/dbt/include/starter_project/models/example/my_second_dbt_model.sql
--rw-r--r--   0 runner    (1001) docker     (127)      447 2024-02-28 23:34:09.000000 dbt-core-1.8.0b1/dbt/include/starter_project/models/example/schema.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 23:34:21.003235 dbt-core-1.8.0b1/dbt/include/starter_project/seeds/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-28 23:34:09.000000 dbt-core-1.8.0b1/dbt/include/starter_project/seeds/.gitkeep
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 23:34:21.003235 dbt-core-1.8.0b1/dbt/include/starter_project/snapshots/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-28 23:34:09.000000 dbt-core-1.8.0b1/dbt/include/starter_project/snapshots/.gitkeep
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 23:34:21.003235 dbt-core-1.8.0b1/dbt/include/starter_project/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-28 23:34:09.000000 dbt-core-1.8.0b1/dbt/include/starter_project/tests/.gitkeep
--rw-r--r--   0 runner    (1001) docker     (127)      712 2024-02-28 23:34:09.000000 dbt-core-1.8.0b1/dbt/internal_deprecations.py
--rw-r--r--   0 runner    (1001) docker     (127)      310 2024-02-28 23:34:09.000000 dbt-core-1.8.0b1/dbt/links.py
--rw-r--r--   0 runner    (1001) docker     (127)    16025 2024-02-28 23:34:09.000000 dbt-core-1.8.0b1/dbt/logger.py
--rw-r--r--   0 runner    (1001) docker     (127)      189 2024-02-28 23:34:09.000000 dbt-core-1.8.0b1/dbt/mp_context.py
--rw-r--r--   0 runner    (1001) docker     (127)      603 2024-02-28 23:34:09.000000 dbt-core-1.8.0b1/dbt/node_types.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 23:34:21.007235 dbt-core-1.8.0b1/dbt/parser/
--rw-r--r--   0 runner    (1001) docker     (127)      653 2024-02-28 23:34:09.000000 dbt-core-1.8.0b1/dbt/parser/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      630 2024-02-28 23:34:09.000000 dbt-core-1.8.0b1/dbt/parser/analysis.py
--rw-r--r--   0 runner    (1001) docker     (127)    19106 2024-02-28 23:34:09.000000 dbt-core-1.8.0b1/dbt/parser/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     5938 2024-02-28 23:34:09.000000 dbt-core-1.8.0b1/dbt/parser/common.py
--rw-r--r--   0 runner    (1001) docker     (127)     1842 2024-02-28 23:34:09.000000 dbt-core-1.8.0b1/dbt/parser/docs.py
--rw-r--r--   0 runner    (1001) docker     (127)     1594 2024-02-28 23:34:09.000000 dbt-core-1.8.0b1/dbt/parser/fixtures.py
--rw-r--r--   0 runner    (1001) docker     (127)     3497 2024-02-28 23:34:09.000000 dbt-core-1.8.0b1/dbt/parser/generic_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    13602 2024-02-28 23:34:09.000000 dbt-core-1.8.0b1/dbt/parser/generic_test_builders.py
--rw-r--r--   0 runner    (1001) docker     (127)     3646 2024-02-28 23:34:09.000000 dbt-core-1.8.0b1/dbt/parser/hooks.py
--rw-r--r--   0 runner    (1001) docker     (127)     4415 2024-02-28 23:34:09.000000 dbt-core-1.8.0b1/dbt/parser/macros.py
--rw-r--r--   0 runner    (1001) docker     (127)    77818 2024-02-28 23:34:09.000000 dbt-core-1.8.0b1/dbt/parser/manifest.py
--rw-r--r--   0 runner    (1001) docker     (127)    23806 2024-02-28 23:34:09.000000 dbt-core-1.8.0b1/dbt/parser/models.py
--rw-r--r--   0 runner    (1001) docker     (127)    53418 2024-02-28 23:34:09.000000 dbt-core-1.8.0b1/dbt/parser/partial.py
--rw-r--r--   0 runner    (1001) docker     (127)    17607 2024-02-28 23:34:09.000000 dbt-core-1.8.0b1/dbt/parser/read_files.py
--rw-r--r--   0 runner    (1001) docker     (127)    16987 2024-02-28 23:34:09.000000 dbt-core-1.8.0b1/dbt/parser/schema_generic_tests.py
--rw-r--r--   0 runner    (1001) docker     (127)     3389 2024-02-28 23:34:09.000000 dbt-core-1.8.0b1/dbt/parser/schema_renderer.py
--rw-r--r--   0 runner    (1001) docker     (127)    28895 2024-02-28 23:34:09.000000 dbt-core-1.8.0b1/dbt/parser/schema_yaml_readers.py
--rw-r--r--   0 runner    (1001) docker     (127)    41561 2024-02-28 23:34:09.000000 dbt-core-1.8.0b1/dbt/parser/schemas.py
--rw-r--r--   0 runner    (1001) docker     (127)     3723 2024-02-28 23:34:09.000000 dbt-core-1.8.0b1/dbt/parser/search.py
--rw-r--r--   0 runner    (1001) docker     (127)     1018 2024-02-28 23:34:09.000000 dbt-core-1.8.0b1/dbt/parser/seeds.py
--rw-r--r--   0 runner    (1001) docker     (127)      690 2024-02-28 23:34:09.000000 dbt-core-1.8.0b1/dbt/parser/singular_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     3101 2024-02-28 23:34:09.000000 dbt-core-1.8.0b1/dbt/parser/snapshots.py
--rw-r--r--   0 runner    (1001) docker     (127)    14913 2024-02-28 23:34:09.000000 dbt-core-1.8.0b1/dbt/parser/sources.py
--rw-r--r--   0 runner    (1001) docker     (127)     1956 2024-02-28 23:34:09.000000 dbt-core-1.8.0b1/dbt/parser/sql.py
--rw-r--r--   0 runner    (1001) docker     (127)    23041 2024-02-28 23:34:09.000000 dbt-core-1.8.0b1/dbt/parser/unit_tests.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 23:34:21.007235 dbt-core-1.8.0b1/dbt/plugins/
--rw-r--r--   0 runner    (1001) docker     (127)      583 2024-02-28 23:34:09.000000 dbt-core-1.8.0b1/dbt/plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      383 2024-02-28 23:34:09.000000 dbt-core-1.8.0b1/dbt/plugins/contracts.py
--rw-r--r--   0 runner    (1001) docker     (127)      112 2024-02-28 23:34:09.000000 dbt-core-1.8.0b1/dbt/plugins/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     5959 2024-02-28 23:34:09.000000 dbt-core-1.8.0b1/dbt/plugins/manager.py
--rw-r--r--   0 runner    (1001) docker     (127)      715 2024-02-28 23:34:09.000000 dbt-core-1.8.0b1/dbt/plugins/manifest.py
--rw-r--r--   0 runner    (1001) docker     (127)      504 2024-02-28 23:34:09.000000 dbt-core-1.8.0b1/dbt/profiler.py
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-02-28 23:34:09.000000 dbt-core-1.8.0b1/dbt/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)      201 2024-02-28 23:34:09.000000 dbt-core-1.8.0b1/dbt/selected_resources.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 23:34:21.011235 dbt-core-1.8.0b1/dbt/task/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-28 23:34:09.000000 dbt-core-1.8.0b1/dbt/task/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16496 2024-02-28 23:34:09.000000 dbt-core-1.8.0b1/dbt/task/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     9071 2024-02-28 23:34:09.000000 dbt-core-1.8.0b1/dbt/task/build.py
--rw-r--r--   0 runner    (1001) docker     (127)     1978 2024-02-28 23:34:09.000000 dbt-core-1.8.0b1/dbt/task/clean.py
--rw-r--r--   0 runner    (1001) docker     (127)     6168 2024-02-28 23:34:09.000000 dbt-core-1.8.0b1/dbt/task/clone.py
--rw-r--r--   0 runner    (1001) docker     (127)     5035 2024-02-28 23:34:09.000000 dbt-core-1.8.0b1/dbt/task/compile.py
--rw-r--r--   0 runner    (1001) docker     (127)    19071 2024-02-28 23:34:09.000000 dbt-core-1.8.0b1/dbt/task/debug.py
--rw-r--r--   0 runner    (1001) docker     (127)    10364 2024-02-28 23:34:09.000000 dbt-core-1.8.0b1/dbt/task/deps.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 23:34:21.015235 dbt-core-1.8.0b1/dbt/task/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      106 2024-02-28 23:34:09.000000 dbt-core-1.8.0b1/dbt/task/docs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14933 2024-02-28 23:34:09.000000 dbt-core-1.8.0b1/dbt/task/docs/generate.py
--rw-r--r--   0 runner    (1001) docker     (127)  1704729 2024-02-28 23:34:09.000000 dbt-core-1.8.0b1/dbt/task/docs/index.html
--rw-r--r--   0 runner    (1001) docker     (127)      845 2024-02-28 23:34:09.000000 dbt-core-1.8.0b1/dbt/task/docs/serve.py
--rw-r--r--   0 runner    (1001) docker     (127)     7516 2024-02-28 23:34:09.000000 dbt-core-1.8.0b1/dbt/task/freshness.py
--rw-r--r--   0 runner    (1001) docker     (127)    15380 2024-02-28 23:34:09.000000 dbt-core-1.8.0b1/dbt/task/init.py
--rw-r--r--   0 runner    (1001) docker     (127)     8398 2024-02-28 23:34:09.000000 dbt-core-1.8.0b1/dbt/task/list.py
--rw-r--r--   0 runner    (1001) docker     (127)     4575 2024-02-28 23:34:09.000000 dbt-core-1.8.0b1/dbt/task/printer.py
--rw-r--r--   0 runner    (1001) docker     (127)     4932 2024-02-28 23:34:09.000000 dbt-core-1.8.0b1/dbt/task/retry.py
--rw-r--r--   0 runner    (1001) docker     (127)    18532 2024-02-28 23:34:09.000000 dbt-core-1.8.0b1/dbt/task/run.py
--rw-r--r--   0 runner    (1001) docker     (127)     4219 2024-02-28 23:34:09.000000 dbt-core-1.8.0b1/dbt/task/run_operation.py
--rw-r--r--   0 runner    (1001) docker     (127)    25746 2024-02-28 23:34:09.000000 dbt-core-1.8.0b1/dbt/task/runnable.py
--rw-r--r--   0 runner    (1001) docker     (127)     3290 2024-02-28 23:34:09.000000 dbt-core-1.8.0b1/dbt/task/seed.py
--rw-r--r--   0 runner    (1001) docker     (127)     4204 2024-02-28 23:34:09.000000 dbt-core-1.8.0b1/dbt/task/show.py
--rw-r--r--   0 runner    (1001) docker     (127)     1802 2024-02-28 23:34:09.000000 dbt-core-1.8.0b1/dbt/task/snapshot.py
--rw-r--r--   0 runner    (1001) docker     (127)     3620 2024-02-28 23:34:09.000000 dbt-core-1.8.0b1/dbt/task/sql.py
--rw-r--r--   0 runner    (1001) docker     (127)    14563 2024-02-28 23:34:09.000000 dbt-core-1.8.0b1/dbt/task/test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 23:34:21.015235 dbt-core-1.8.0b1/dbt/tests/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 23:34:21.015235 dbt-core-1.8.0b1/dbt/tests/fixtures/
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-02-28 23:34:09.000000 dbt-core-1.8.0b1/dbt/tests/fixtures/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    20263 2024-02-28 23:34:09.000000 dbt-core-1.8.0b1/dbt/tests/fixtures/project.py
--rw-r--r--   0 runner    (1001) docker     (127)    20813 2024-02-28 23:34:09.000000 dbt-core-1.8.0b1/dbt/tests/util.py
--rw-r--r--   0 runner    (1001) docker     (127)    14893 2024-02-28 23:34:09.000000 dbt-core-1.8.0b1/dbt/tracking.py
--rw-r--r--   0 runner    (1001) docker     (127)    11981 2024-02-28 23:34:09.000000 dbt-core-1.8.0b1/dbt/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     7369 2024-02-28 23:34:09.000000 dbt-core-1.8.0b1/dbt/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 23:34:21.019235 dbt-core-1.8.0b1/dbt_core.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3916 2024-02-28 23:34:20.000000 dbt-core-1.8.0b1/dbt_core.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5972 2024-02-28 23:34:20.000000 dbt-core-1.8.0b1/dbt_core.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-28 23:34:20.000000 dbt-core-1.8.0b1/dbt_core.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-02-28 23:34:20.000000 dbt-core-1.8.0b1/dbt_core.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-28 23:34:20.000000 dbt-core-1.8.0b1/dbt_core.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-02-28 23:34:20.000000 dbt-core-1.8.0b1/dbt_core.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        4 2024-02-28 23:34:20.000000 dbt-core-1.8.0b1/dbt_core.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-28 23:34:21.019235 dbt-core-1.8.0b1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     3963 2024-02-28 23:34:09.000000 dbt-core-1.8.0b1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 15:20:18.708722 dbt-core-1.8.0b2/
+-rw-r--r--   0 runner    (1001) docker     (127)      139 2024-04-03 15:20:02.000000 dbt-core-1.8.0b2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3917 2024-04-03 15:20:18.708722 dbt-core-1.8.0b2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2365 2024-04-03 15:20:02.000000 dbt-core-1.8.0b2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 15:20:18.672722 dbt-core-1.8.0b2/dbt/
+-rw-r--r--   0 runner    (1001) docker     (127)      341 2024-04-03 15:20:02.000000 dbt-core-1.8.0b2/dbt/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 15:20:18.672722 dbt-core-1.8.0b2/dbt/artifacts/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 15:20:02.000000 dbt-core-1.8.0b2/dbt/artifacts/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 15:20:18.676722 dbt-core-1.8.0b2/dbt/artifacts/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)     2669 2024-04-03 15:20:02.000000 dbt-core-1.8.0b2/dbt/artifacts/resources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1779 2024-04-03 15:20:02.000000 dbt-core-1.8.0b2/dbt/artifacts/resources/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1498 2024-04-03 15:20:02.000000 dbt-core-1.8.0b2/dbt/artifacts/resources/types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 15:20:18.676722 dbt-core-1.8.0b2/dbt/artifacts/resources/v1/
+-rw-r--r--   0 runner    (1001) docker     (127)      272 2024-04-03 15:20:02.000000 dbt-core-1.8.0b2/dbt/artifacts/resources/v1/analysis.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6870 2024-04-03 15:20:02.000000 dbt-core-1.8.0b2/dbt/artifacts/resources/v1/components.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9586 2024-04-03 15:20:02.000000 dbt-core-1.8.0b2/dbt/artifacts/resources/v1/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      290 2024-04-03 15:20:02.000000 dbt-core-1.8.0b2/dbt/artifacts/resources/v1/documentation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1555 2024-04-03 15:20:02.000000 dbt-core-1.8.0b2/dbt/artifacts/resources/v1/exposure.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1209 2024-04-03 15:20:02.000000 dbt-core-1.8.0b2/dbt/artifacts/resources/v1/generic_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)      332 2024-04-03 15:20:02.000000 dbt-core-1.8.0b2/dbt/artifacts/resources/v1/group.py
+-rw-r--r--   0 runner    (1001) docker     (127)      315 2024-04-03 15:20:02.000000 dbt-core-1.8.0b2/dbt/artifacts/resources/v1/hook.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1003 2024-04-03 15:20:02.000000 dbt-core-1.8.0b2/dbt/artifacts/resources/v1/macro.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4728 2024-04-03 15:20:02.000000 dbt-core-1.8.0b2/dbt/artifacts/resources/v1/metric.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1079 2024-04-03 15:20:02.000000 dbt-core-1.8.0b2/dbt/artifacts/resources/v1/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)      260 2024-04-03 15:20:02.000000 dbt-core-1.8.0b2/dbt/artifacts/resources/v1/owner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2827 2024-04-03 15:20:02.000000 dbt-core-1.8.0b2/dbt/artifacts/resources/v1/saved_query.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1168 2024-04-03 15:20:02.000000 dbt-core-1.8.0b2/dbt/artifacts/resources/v1/seed.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1327 2024-04-03 15:20:02.000000 dbt-core-1.8.0b2/dbt/artifacts/resources/v1/semantic_layer_components.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8913 2024-04-03 15:20:02.000000 dbt-core-1.8.0b2/dbt/artifacts/resources/v1/semantic_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)      523 2024-04-03 15:20:02.000000 dbt-core-1.8.0b2/dbt/artifacts/resources/v1/singular_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2909 2024-04-03 15:20:02.000000 dbt-core-1.8.0b2/dbt/artifacts/resources/v1/snapshot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2385 2024-04-03 15:20:02.000000 dbt-core-1.8.0b2/dbt/artifacts/resources/v1/source_definition.py
+-rw-r--r--   0 runner    (1001) docker     (127)      280 2024-04-03 15:20:02.000000 dbt-core-1.8.0b2/dbt/artifacts/resources/v1/sql_operation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2369 2024-04-03 15:20:02.000000 dbt-core-1.8.0b2/dbt/artifacts/resources/v1/unit_test_definition.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 15:20:18.680722 dbt-core-1.8.0b2/dbt/artifacts/schemas/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 15:20:02.000000 dbt-core-1.8.0b2/dbt/artifacts/schemas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6404 2024-04-03 15:20:02.000000 dbt-core-1.8.0b2/dbt/artifacts/schemas/base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 15:20:18.680722 dbt-core-1.8.0b2/dbt/artifacts/schemas/catalog/
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-04-03 15:20:02.000000 dbt-core-1.8.0b2/dbt/artifacts/schemas/catalog/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 15:20:18.680722 dbt-core-1.8.0b2/dbt/artifacts/schemas/catalog/v1/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 15:20:02.000000 dbt-core-1.8.0b2/dbt/artifacts/schemas/catalog/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2692 2024-04-03 15:20:02.000000 dbt-core-1.8.0b2/dbt/artifacts/schemas/catalog/v1/catalog.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 15:20:18.680722 dbt-core-1.8.0b2/dbt/artifacts/schemas/freshness/
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-04-03 15:20:02.000000 dbt-core-1.8.0b2/dbt/artifacts/schemas/freshness/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 15:20:18.680722 dbt-core-1.8.0b2/dbt/artifacts/schemas/freshness/v3/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 15:20:02.000000 dbt-core-1.8.0b2/dbt/artifacts/schemas/freshness/v3/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4356 2024-04-03 15:20:02.000000 dbt-core-1.8.0b2/dbt/artifacts/schemas/freshness/v3/freshness.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 15:20:18.680722 dbt-core-1.8.0b2/dbt/artifacts/schemas/manifest/
+-rw-r--r--   0 runner    (1001) docker     (127)       84 2024-04-03 15:20:02.000000 dbt-core-1.8.0b2/dbt/artifacts/schemas/manifest/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 15:20:18.680722 dbt-core-1.8.0b2/dbt/artifacts/schemas/manifest/v12/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 15:20:02.000000 dbt-core-1.8.0b2/dbt/artifacts/schemas/manifest/v12/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5898 2024-04-03 15:20:02.000000 dbt-core-1.8.0b2/dbt/artifacts/schemas/manifest/v12/manifest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4064 2024-04-03 15:20:02.000000 dbt-core-1.8.0b2/dbt/artifacts/schemas/results.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 15:20:18.680722 dbt-core-1.8.0b2/dbt/artifacts/schemas/run/
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-04-03 15:20:02.000000 dbt-core-1.8.0b2/dbt/artifacts/schemas/run/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 15:20:18.680722 dbt-core-1.8.0b2/dbt/artifacts/schemas/run/v5/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 15:20:02.000000 dbt-core-1.8.0b2/dbt/artifacts/schemas/run/v5/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4660 2024-04-03 15:20:02.000000 dbt-core-1.8.0b2/dbt/artifacts/schemas/run/v5/run.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 15:20:18.680722 dbt-core-1.8.0b2/dbt/artifacts/schemas/upgrades/
+-rw-r--r--   0 runner    (1001) docker     (127)       82 2024-04-03 15:20:02.000000 dbt-core-1.8.0b2/dbt/artifacts/schemas/upgrades/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6898 2024-04-03 15:20:02.000000 dbt-core-1.8.0b2/dbt/artifacts/schemas/upgrades/upgrade_manifest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 15:20:18.684722 dbt-core-1.8.0b2/dbt/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-03 15:20:02.000000 dbt-core-1.8.0b2/dbt/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      379 2024-04-03 15:20:02.000000 dbt-core-1.8.0b2/dbt/cli/context.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1357 2024-04-03 15:20:02.000000 dbt-core-1.8.0b2/dbt/cli/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20055 2024-04-03 15:20:02.000000 dbt-core-1.8.0b2/dbt/cli/flags.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18842 2024-04-03 15:20:02.000000 dbt-core-1.8.0b2/dbt/cli/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2900 2024-04-03 15:20:02.000000 dbt-core-1.8.0b2/dbt/cli/option_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3520 2024-04-03 15:20:02.000000 dbt-core-1.8.0b2/dbt/cli/options.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21775 2024-04-03 15:20:02.000000 dbt-core-1.8.0b2/dbt/cli/params.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10642 2024-04-03 15:20:02.000000 dbt-core-1.8.0b2/dbt/cli/requires.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1247 2024-04-03 15:20:02.000000 dbt-core-1.8.0b2/dbt/cli/resolvers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1006 2024-04-03 15:20:02.000000 dbt-core-1.8.0b2/dbt/cli/types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 15:20:18.684722 dbt-core-1.8.0b2/dbt/clients/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 15:20:02.000000 dbt-core-1.8.0b2/dbt/clients/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5262 2024-04-03 15:20:02.000000 dbt-core-1.8.0b2/dbt/clients/git.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6525 2024-04-03 15:20:02.000000 dbt-core-1.8.0b2/dbt/clients/jinja.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5395 2024-04-03 15:20:02.000000 dbt-core-1.8.0b2/dbt/clients/jinja_static.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7961 2024-04-03 15:20:02.000000 dbt-core-1.8.0b2/dbt/clients/registry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1729 2024-04-03 15:20:02.000000 dbt-core-1.8.0b2/dbt/clients/yaml_helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23871 2024-04-03 15:20:02.000000 dbt-core-1.8.0b2/dbt/compilation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 15:20:18.684722 dbt-core-1.8.0b2/dbt/config/
+-rw-r--r--   0 runner    (1001) docker     (127)      224 2024-04-03 15:20:02.000000 dbt-core-1.8.0b2/dbt/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15551 2024-04-03 15:20:02.000000 dbt-core-1.8.0b2/dbt/config/profile.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31410 2024-04-03 15:20:02.000000 dbt-core-1.8.0b2/dbt/config/project.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8103 2024-04-03 15:20:02.000000 dbt-core-1.8.0b2/dbt/config/renderer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17206 2024-04-03 15:20:02.000000 dbt-core-1.8.0b2/dbt/config/runtime.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7925 2024-04-03 15:20:02.000000 dbt-core-1.8.0b2/dbt/config/selectors.py
+-rw-r--r--   0 runner    (1001) docker     (127)      842 2024-04-03 15:20:02.000000 dbt-core-1.8.0b2/dbt/config/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      676 2024-04-03 15:20:02.000000 dbt-core-1.8.0b2/dbt/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 15:20:18.688722 dbt-core-1.8.0b2/dbt/context/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 15:20:02.000000 dbt-core-1.8.0b2/dbt/context/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23769 2024-04-03 15:20:02.000000 dbt-core-1.8.0b2/dbt/context/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4467 2024-04-03 15:20:02.000000 dbt-core-1.8.0b2/dbt/context/configured.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14230 2024-04-03 15:20:02.000000 dbt-core-1.8.0b2/dbt/context/context_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2538 2024-04-03 15:20:02.000000 dbt-core-1.8.0b2/dbt/context/docs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4424 2024-04-03 15:20:02.000000 dbt-core-1.8.0b2/dbt/context/exceptions_jinja.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8681 2024-04-03 15:20:02.000000 dbt-core-1.8.0b2/dbt/context/macro_resolver.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7426 2024-04-03 15:20:02.000000 dbt-core-1.8.0b2/dbt/context/macros.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3044 2024-04-03 15:20:02.000000 dbt-core-1.8.0b2/dbt/context/manifest.py
+-rw-r--r--   0 runner    (1001) docker     (127)    67660 2024-04-03 15:20:02.000000 dbt-core-1.8.0b2/dbt/context/providers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2654 2024-04-03 15:20:02.000000 dbt-core-1.8.0b2/dbt/context/secret.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4165 2024-04-03 15:20:02.000000 dbt-core-1.8.0b2/dbt/context/target.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 15:20:18.688722 dbt-core-1.8.0b2/dbt/contracts/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 15:20:02.000000 dbt-core-1.8.0b2/dbt/contracts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10059 2024-04-03 15:20:02.000000 dbt-core-1.8.0b2/dbt/contracts/files.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 15:20:18.688722 dbt-core-1.8.0b2/dbt/contracts/graph/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 15:20:02.000000 dbt-core-1.8.0b2/dbt/contracts/graph/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    64188 2024-04-03 15:20:02.000000 dbt-core-1.8.0b2/dbt/contracts/graph/manifest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3869 2024-04-03 15:20:02.000000 dbt-core-1.8.0b2/dbt/contracts/graph/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2056 2024-04-03 15:20:02.000000 dbt-core-1.8.0b2/dbt/contracts/graph/model_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1209 2024-04-03 15:20:02.000000 dbt-core-1.8.0b2/dbt/contracts/graph/node_args.py
+-rw-r--r--   0 runner    (1001) docker     (127)    55019 2024-04-03 15:20:02.000000 dbt-core-1.8.0b2/dbt/contracts/graph/nodes.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 15:20:02.000000 dbt-core-1.8.0b2/dbt/contracts/graph/searcher.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4459 2024-04-03 15:20:02.000000 dbt-core-1.8.0b2/dbt/contracts/graph/semantic_manifest.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22110 2024-04-03 15:20:02.000000 dbt-core-1.8.0b2/dbt/contracts/graph/unparsed.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2677 2024-04-03 15:20:02.000000 dbt-core-1.8.0b2/dbt/contracts/graph/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11569 2024-04-03 15:20:02.000000 dbt-core-1.8.0b2/dbt/contracts/project.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1228 2024-04-03 15:20:02.000000 dbt-core-1.8.0b2/dbt/contracts/results.py
+-rw-r--r--   0 runner    (1001) docker     (127)      522 2024-04-03 15:20:02.000000 dbt-core-1.8.0b2/dbt/contracts/selection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2243 2024-04-03 15:20:02.000000 dbt-core-1.8.0b2/dbt/contracts/sql.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3007 2024-04-03 15:20:02.000000 dbt-core-1.8.0b2/dbt/contracts/state.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1130 2024-04-03 15:20:02.000000 dbt-core-1.8.0b2/dbt/contracts/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4994 2024-04-03 15:20:02.000000 dbt-core-1.8.0b2/dbt/deprecations.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 15:20:18.692722 dbt-core-1.8.0b2/dbt/deps/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 15:20:02.000000 dbt-core-1.8.0b2/dbt/deps/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4778 2024-04-03 15:20:02.000000 dbt-core-1.8.0b2/dbt/deps/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6438 2024-04-03 15:20:02.000000 dbt-core-1.8.0b2/dbt/deps/git.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2520 2024-04-03 15:20:02.000000 dbt-core-1.8.0b2/dbt/deps/local.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4553 2024-04-03 15:20:02.000000 dbt-core-1.8.0b2/dbt/deps/registry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4889 2024-04-03 15:20:02.000000 dbt-core-1.8.0b2/dbt/deps/resolver.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4544 2024-04-03 15:20:02.000000 dbt-core-1.8.0b2/dbt/deps/tarball.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 15:20:18.668722 dbt-core-1.8.0b2/dbt/docs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 15:20:18.692722 dbt-core-1.8.0b2/dbt/docs/source/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 15:20:18.692722 dbt-core-1.8.0b2/dbt/docs/source/_ext/
+-rw-r--r--   0 runner    (1001) docker     (127)     3544 2024-04-03 15:20:02.000000 dbt-core-1.8.0b2/dbt/docs/source/_ext/dbt_click.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1060 2024-04-03 15:20:02.000000 dbt-core-1.8.0b2/dbt/docs/source/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 15:20:18.692722 dbt-core-1.8.0b2/dbt/events/
+-rw-r--r--   0 runner    (1001) docker     (127)      454 2024-04-03 15:20:02.000000 dbt-core-1.8.0b2/dbt/events/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      924 2024-04-03 15:20:02.000000 dbt-core-1.8.0b2/dbt/events/base_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)    98530 2024-04-03 15:20:02.000000 dbt-core-1.8.0b2/dbt/events/core_types_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3648 2024-04-03 15:20:02.000000 dbt-core-1.8.0b2/dbt/events/logging.py
+-rw-r--r--   0 runner    (1001) docker     (127)    53554 2024-04-03 15:20:02.000000 dbt-core-1.8.0b2/dbt/events/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)    49734 2024-04-03 15:20:02.000000 dbt-core-1.8.0b2/dbt/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3602 2024-04-03 15:20:02.000000 dbt-core-1.8.0b2/dbt/flags.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 15:20:18.692722 dbt-core-1.8.0b2/dbt/graph/
+-rw-r--r--   0 runner    (1001) docker     (127)      430 2024-04-03 15:20:02.000000 dbt-core-1.8.0b2/dbt/graph/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9620 2024-04-03 15:20:02.000000 dbt-core-1.8.0b2/dbt/graph/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5368 2024-04-03 15:20:02.000000 dbt-core-1.8.0b2/dbt/graph/graph.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7340 2024-04-03 15:20:02.000000 dbt-core-1.8.0b2/dbt/graph/queue.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14905 2024-04-03 15:20:02.000000 dbt-core-1.8.0b2/dbt/graph/selector.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34960 2024-04-03 15:20:02.000000 dbt-core-1.8.0b2/dbt/graph/selector_methods.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7229 2024-04-03 15:20:02.000000 dbt-core-1.8.0b2/dbt/graph/selector_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)      511 2024-04-03 15:20:02.000000 dbt-core-1.8.0b2/dbt/hooks.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 15:20:18.692722 dbt-core-1.8.0b2/dbt/include/
+-rw-r--r--   0 runner    (1001) docker     (127)     4794 2024-04-03 15:20:02.000000 dbt-core-1.8.0b2/dbt/include/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-04-03 15:20:02.000000 dbt-core-1.8.0b2/dbt/include/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 15:20:18.696722 dbt-core-1.8.0b2/dbt/include/starter_project/
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-04-03 15:20:02.000000 dbt-core-1.8.0b2/dbt/include/starter_project/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      571 2024-04-03 15:20:02.000000 dbt-core-1.8.0b2/dbt/include/starter_project/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-03 15:20:02.000000 dbt-core-1.8.0b2/dbt/include/starter_project/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 15:20:18.696722 dbt-core-1.8.0b2/dbt/include/starter_project/analyses/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 15:20:02.000000 dbt-core-1.8.0b2/dbt/include/starter_project/analyses/.gitkeep
+-rw-r--r--   0 runner    (1001) docker     (127)     1260 2024-04-03 15:20:02.000000 dbt-core-1.8.0b2/dbt/include/starter_project/dbt_project.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 15:20:18.696722 dbt-core-1.8.0b2/dbt/include/starter_project/macros/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 15:20:02.000000 dbt-core-1.8.0b2/dbt/include/starter_project/macros/.gitkeep
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 15:20:18.668722 dbt-core-1.8.0b2/dbt/include/starter_project/models/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 15:20:18.696722 dbt-core-1.8.0b2/dbt/include/starter_project/models/example/
+-rw-r--r--   0 runner    (1001) docker     (127)      475 2024-04-03 15:20:02.000000 dbt-core-1.8.0b2/dbt/include/starter_project/models/example/my_first_dbt_model.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      115 2024-04-03 15:20:02.000000 dbt-core-1.8.0b2/dbt/include/starter_project/models/example/my_second_dbt_model.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      447 2024-04-03 15:20:02.000000 dbt-core-1.8.0b2/dbt/include/starter_project/models/example/schema.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 15:20:18.696722 dbt-core-1.8.0b2/dbt/include/starter_project/seeds/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 15:20:02.000000 dbt-core-1.8.0b2/dbt/include/starter_project/seeds/.gitkeep
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 15:20:18.696722 dbt-core-1.8.0b2/dbt/include/starter_project/snapshots/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 15:20:02.000000 dbt-core-1.8.0b2/dbt/include/starter_project/snapshots/.gitkeep
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 15:20:18.696722 dbt-core-1.8.0b2/dbt/include/starter_project/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 15:20:02.000000 dbt-core-1.8.0b2/dbt/include/starter_project/tests/.gitkeep
+-rw-r--r--   0 runner    (1001) docker     (127)      712 2024-04-03 15:20:02.000000 dbt-core-1.8.0b2/dbt/internal_deprecations.py
+-rw-r--r--   0 runner    (1001) docker     (127)      310 2024-04-03 15:20:02.000000 dbt-core-1.8.0b2/dbt/links.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16025 2024-04-03 15:20:02.000000 dbt-core-1.8.0b2/dbt/logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)      189 2024-04-03 15:20:02.000000 dbt-core-1.8.0b2/dbt/mp_context.py
+-rw-r--r--   0 runner    (1001) docker     (127)      603 2024-04-03 15:20:02.000000 dbt-core-1.8.0b2/dbt/node_types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 15:20:18.700722 dbt-core-1.8.0b2/dbt/parser/
+-rw-r--r--   0 runner    (1001) docker     (127)      653 2024-04-03 15:20:02.000000 dbt-core-1.8.0b2/dbt/parser/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      630 2024-04-03 15:20:02.000000 dbt-core-1.8.0b2/dbt/parser/analysis.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19106 2024-04-03 15:20:02.000000 dbt-core-1.8.0b2/dbt/parser/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5938 2024-04-03 15:20:02.000000 dbt-core-1.8.0b2/dbt/parser/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1842 2024-04-03 15:20:02.000000 dbt-core-1.8.0b2/dbt/parser/docs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1594 2024-04-03 15:20:02.000000 dbt-core-1.8.0b2/dbt/parser/fixtures.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3497 2024-04-03 15:20:02.000000 dbt-core-1.8.0b2/dbt/parser/generic_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13602 2024-04-03 15:20:02.000000 dbt-core-1.8.0b2/dbt/parser/generic_test_builders.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3646 2024-04-03 15:20:02.000000 dbt-core-1.8.0b2/dbt/parser/hooks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4415 2024-04-03 15:20:02.000000 dbt-core-1.8.0b2/dbt/parser/macros.py
+-rw-r--r--   0 runner    (1001) docker     (127)    78171 2024-04-03 15:20:02.000000 dbt-core-1.8.0b2/dbt/parser/manifest.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23806 2024-04-03 15:20:02.000000 dbt-core-1.8.0b2/dbt/parser/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)    53594 2024-04-03 15:20:02.000000 dbt-core-1.8.0b2/dbt/parser/partial.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17600 2024-04-03 15:20:02.000000 dbt-core-1.8.0b2/dbt/parser/read_files.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16987 2024-04-03 15:20:02.000000 dbt-core-1.8.0b2/dbt/parser/schema_generic_tests.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3473 2024-04-03 15:20:02.000000 dbt-core-1.8.0b2/dbt/parser/schema_renderer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28895 2024-04-03 15:20:02.000000 dbt-core-1.8.0b2/dbt/parser/schema_yaml_readers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    43015 2024-04-03 15:20:02.000000 dbt-core-1.8.0b2/dbt/parser/schemas.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3723 2024-04-03 15:20:02.000000 dbt-core-1.8.0b2/dbt/parser/search.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1018 2024-04-03 15:20:02.000000 dbt-core-1.8.0b2/dbt/parser/seeds.py
+-rw-r--r--   0 runner    (1001) docker     (127)      690 2024-04-03 15:20:02.000000 dbt-core-1.8.0b2/dbt/parser/singular_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3101 2024-04-03 15:20:02.000000 dbt-core-1.8.0b2/dbt/parser/snapshots.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14964 2024-04-03 15:20:02.000000 dbt-core-1.8.0b2/dbt/parser/sources.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1956 2024-04-03 15:20:02.000000 dbt-core-1.8.0b2/dbt/parser/sql.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23685 2024-04-03 15:20:02.000000 dbt-core-1.8.0b2/dbt/parser/unit_tests.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 15:20:18.700722 dbt-core-1.8.0b2/dbt/plugins/
+-rw-r--r--   0 runner    (1001) docker     (127)      583 2024-04-03 15:20:02.000000 dbt-core-1.8.0b2/dbt/plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      383 2024-04-03 15:20:02.000000 dbt-core-1.8.0b2/dbt/plugins/contracts.py
+-rw-r--r--   0 runner    (1001) docker     (127)      112 2024-04-03 15:20:02.000000 dbt-core-1.8.0b2/dbt/plugins/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5959 2024-04-03 15:20:02.000000 dbt-core-1.8.0b2/dbt/plugins/manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)      715 2024-04-03 15:20:02.000000 dbt-core-1.8.0b2/dbt/plugins/manifest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      504 2024-04-03 15:20:02.000000 dbt-core-1.8.0b2/dbt/profiler.py
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-04-03 15:20:02.000000 dbt-core-1.8.0b2/dbt/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)      201 2024-04-03 15:20:02.000000 dbt-core-1.8.0b2/dbt/selected_resources.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 15:20:18.704722 dbt-core-1.8.0b2/dbt/task/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 15:20:02.000000 dbt-core-1.8.0b2/dbt/task/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17771 2024-04-03 15:20:02.000000 dbt-core-1.8.0b2/dbt/task/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8918 2024-04-03 15:20:02.000000 dbt-core-1.8.0b2/dbt/task/build.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1978 2024-04-03 15:20:02.000000 dbt-core-1.8.0b2/dbt/task/clean.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6140 2024-04-03 15:20:02.000000 dbt-core-1.8.0b2/dbt/task/clone.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5035 2024-04-03 15:20:02.000000 dbt-core-1.8.0b2/dbt/task/compile.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19071 2024-04-03 15:20:02.000000 dbt-core-1.8.0b2/dbt/task/debug.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10384 2024-04-03 15:20:02.000000 dbt-core-1.8.0b2/dbt/task/deps.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 15:20:18.708722 dbt-core-1.8.0b2/dbt/task/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      106 2024-04-03 15:20:02.000000 dbt-core-1.8.0b2/dbt/task/docs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14986 2024-04-03 15:20:02.000000 dbt-core-1.8.0b2/dbt/task/docs/generate.py
+-rw-r--r--   0 runner    (1001) docker     (127)  1509632 2024-04-03 15:20:02.000000 dbt-core-1.8.0b2/dbt/task/docs/index.html
+-rw-r--r--   0 runner    (1001) docker     (127)      845 2024-04-03 15:20:02.000000 dbt-core-1.8.0b2/dbt/task/docs/serve.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7597 2024-04-03 15:20:02.000000 dbt-core-1.8.0b2/dbt/task/freshness.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15380 2024-04-03 15:20:02.000000 dbt-core-1.8.0b2/dbt/task/init.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8663 2024-04-03 15:20:02.000000 dbt-core-1.8.0b2/dbt/task/list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4966 2024-04-03 15:20:02.000000 dbt-core-1.8.0b2/dbt/task/printer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4932 2024-04-03 15:20:02.000000 dbt-core-1.8.0b2/dbt/task/retry.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18532 2024-04-03 15:20:02.000000 dbt-core-1.8.0b2/dbt/task/run.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4277 2024-04-03 15:20:02.000000 dbt-core-1.8.0b2/dbt/task/run_operation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26636 2024-04-03 15:20:02.000000 dbt-core-1.8.0b2/dbt/task/runnable.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3290 2024-04-03 15:20:02.000000 dbt-core-1.8.0b2/dbt/task/seed.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4204 2024-04-03 15:20:02.000000 dbt-core-1.8.0b2/dbt/task/show.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1802 2024-04-03 15:20:02.000000 dbt-core-1.8.0b2/dbt/task/snapshot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3620 2024-04-03 15:20:02.000000 dbt-core-1.8.0b2/dbt/task/sql.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14896 2024-04-03 15:20:02.000000 dbt-core-1.8.0b2/dbt/task/test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 15:20:18.708722 dbt-core-1.8.0b2/dbt/tests/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 15:20:18.708722 dbt-core-1.8.0b2/dbt/tests/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-04-03 15:20:02.000000 dbt-core-1.8.0b2/dbt/tests/fixtures/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20263 2024-04-03 15:20:02.000000 dbt-core-1.8.0b2/dbt/tests/fixtures/project.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20813 2024-04-03 15:20:02.000000 dbt-core-1.8.0b2/dbt/tests/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14893 2024-04-03 15:20:02.000000 dbt-core-1.8.0b2/dbt/tracking.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11981 2024-04-03 15:20:02.000000 dbt-core-1.8.0b2/dbt/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7369 2024-04-03 15:20:02.000000 dbt-core-1.8.0b2/dbt/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 15:20:18.708722 dbt-core-1.8.0b2/dbt_core.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3917 2024-04-03 15:20:18.000000 dbt-core-1.8.0b2/dbt_core.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5972 2024-04-03 15:20:18.000000 dbt-core-1.8.0b2/dbt_core.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 15:20:18.000000 dbt-core-1.8.0b2/dbt_core.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-03 15:20:18.000000 dbt-core-1.8.0b2/dbt_core.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 15:20:18.000000 dbt-core-1.8.0b2/dbt_core.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      412 2024-04-03 15:20:18.000000 dbt-core-1.8.0b2/dbt_core.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-04-03 15:20:18.000000 dbt-core-1.8.0b2/dbt_core.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-03 15:20:18.708722 dbt-core-1.8.0b2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3964 2024-04-03 15:20:02.000000 dbt-core-1.8.0b2/setup.py
```

### Comparing `dbt-core-1.8.0b1/PKG-INFO` & `dbt-core-1.8.0b2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbt-core
-Version: 1.8.0b1
+Version: 1.8.0b2
 Summary: With dbt, data analysts and engineers can build analytics the way engineers build applications.
 Home-page: https://github.com/dbt-labs/dbt-core
 Author: dbt Labs
 Author-email: info@dbtlabs.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: Microsoft :: Windows
@@ -19,24 +19,24 @@
 Description-Content-Type: text/markdown
 Requires-Dist: agate<1.8,>=1.7.0
 Requires-Dist: Jinja2<4,>=3.1.3
 Requires-Dist: mashumaro[msgpack]<4.0,>=3.9
 Requires-Dist: logbook<1.6,>=1.5
 Requires-Dist: click<9.0,>=8.0.2
 Requires-Dist: networkx<4.0,>=2.3
+Requires-Dist: protobuf<5,>=4.0.0
 Requires-Dist: requests<3.0.0
 Requires-Dist: pathspec<0.12,>=0.9
 Requires-Dist: sqlparse<0.5,>=0.2.3
 Requires-Dist: dbt-extractor<=0.6,>=0.5.0
 Requires-Dist: minimal-snowplow-tracker<0.1,>=0.0.2
-Requires-Dist: dbt-semantic-interfaces<0.6,>=0.5.0a2
+Requires-Dist: dbt-semantic-interfaces<0.6,>=0.5.1
 Requires-Dist: dbt-common<2.0
 Requires-Dist: dbt-adapters<2.0,>=0.1.0a2
 Requires-Dist: packaging>20.9
-Requires-Dist: protobuf>=4.0.0
 Requires-Dist: pytz>=2015.7
 Requires-Dist: pyyaml>=6.0
 Requires-Dist: daff>=1.3.46
 Requires-Dist: typing-extensions>=4.4
 
 <p align="center">
   <img src="https://raw.githubusercontent.com/dbt-labs/dbt-core/fa1ea14ddfb1d5ae319d5141844910dd53ab2834/etc/dbt-core.svg" alt="dbt logo" width="750"/>
```

#### html2text {}

```diff
@@ -1,28 +1,28 @@
-Metadata-Version: 2.1 Name: dbt-core Version: 1.8.0b1 Summary: With dbt, data
+Metadata-Version: 2.1 Name: dbt-core Version: 1.8.0b2 Summary: With dbt, data
 analysts and engineers can build analytics the way engineers build
 applications. Home-page: https://github.com/dbt-labs/dbt-core Author: dbt Labs
 Author-email: info@dbtlabs.com Classifier: Development Status :: 5 -
 Production/Stable Classifier: License :: OSI Approved :: Apache Software
 License Classifier: Operating System :: Microsoft :: Windows Classifier:
 Operating System :: MacOS :: MacOS X Classifier: Operating System :: POSIX ::
 Linux Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
 Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11 Classifier: Programming
 Language :: Python :: 3.12 Requires-Python: >=3.8 Description-Content-Type:
 text/markdown Requires-Dist: agate<1.8,>=1.7.0 Requires-Dist: Jinja2<4,>=3.1.3
 Requires-Dist: mashumaro[msgpack]<4.0,>=3.9 Requires-Dist: logbook<1.6,>=1.5
 Requires-Dist: click<9.0,>=8.0.2 Requires-Dist: networkx<4.0,>=2.3 Requires-
-Dist: requests<3.0.0 Requires-Dist: pathspec<0.12,>=0.9 Requires-Dist:
-sqlparse<0.5,>=0.2.3 Requires-Dist: dbt-extractor<=0.6,>=0.5.0 Requires-Dist:
-minimal-snowplow-tracker<0.1,>=0.0.2 Requires-Dist: dbt-semantic-
-interfaces<0.6,>=0.5.0a2 Requires-Dist: dbt-common<2.0 Requires-Dist: dbt-
-adapters<2.0,>=0.1.0a2 Requires-Dist: packaging>20.9 Requires-Dist:
-protobuf>=4.0.0 Requires-Dist: pytz>=2015.7 Requires-Dist: pyyaml>=6.0
-Requires-Dist: daff>=1.3.46 Requires-Dist: typing-extensions>=4.4
+Dist: protobuf<5,>=4.0.0 Requires-Dist: requests<3.0.0 Requires-Dist:
+pathspec<0.12,>=0.9 Requires-Dist: sqlparse<0.5,>=0.2.3 Requires-Dist: dbt-
+extractor<=0.6,>=0.5.0 Requires-Dist: minimal-snowplow-tracker<0.1,>=0.0.2
+Requires-Dist: dbt-semantic-interfaces<0.6,>=0.5.1 Requires-Dist: dbt-
+common<2.0 Requires-Dist: dbt-adapters<2.0,>=0.1.0a2 Requires-Dist:
+packaging>20.9 Requires-Dist: pytz>=2015.7 Requires-Dist: pyyaml>=6.0 Requires-
+Dist: daff>=1.3.46 Requires-Dist: typing-extensions>=4.4
                                   [dbt logo]
                                   _[_C_I_ _B_a_d_g_e_]
 **[dbt](https://www.getdbt.com/)** enables data analysts and engineers to
 transform their data using the same practices that software engineers use to
 build applications. ![architecture](https://raw.githubusercontent.com/dbt-labs/
 dbt-core/6c6649f9129d5d108aa3b0526f634cd8f3a9d1ed/etc/dbt-arch.png) ##
 Understanding dbt Analysts using dbt can transform their data by simply writing
```

### Comparing `dbt-core-1.8.0b1/README.md` & `dbt-core-1.8.0b2/README.md`

 * *Files identical despite different names*

### Comparing `dbt-core-1.8.0b1/dbt/artifacts/resources/__init__.py` & `dbt-core-1.8.0b2/dbt/artifacts/resources/__init__.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.8.0b1/dbt/artifacts/resources/base.py` & `dbt-core-1.8.0b2/dbt/artifacts/resources/base.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.8.0b1/dbt/artifacts/resources/types.py` & `dbt-core-1.8.0b2/dbt/artifacts/resources/types.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.8.0b1/dbt/artifacts/resources/v1/components.py` & `dbt-core-1.8.0b2/dbt/artifacts/resources/v1/components.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.8.0b1/dbt/artifacts/resources/v1/config.py` & `dbt-core-1.8.0b2/dbt/artifacts/resources/v1/config.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.8.0b1/dbt/artifacts/resources/v1/exposure.py` & `dbt-core-1.8.0b2/dbt/artifacts/resources/v1/exposure.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.8.0b1/dbt/artifacts/resources/v1/generic_test.py` & `dbt-core-1.8.0b2/dbt/artifacts/resources/v1/generic_test.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.8.0b1/dbt/artifacts/resources/v1/macro.py` & `dbt-core-1.8.0b2/dbt/artifacts/resources/v1/macro.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.8.0b1/dbt/artifacts/resources/v1/metric.py` & `dbt-core-1.8.0b2/dbt/artifacts/resources/v1/metric.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.8.0b1/dbt/artifacts/resources/v1/model.py` & `dbt-core-1.8.0b2/dbt/artifacts/resources/v1/model.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.8.0b1/dbt/artifacts/resources/v1/saved_query.py` & `dbt-core-1.8.0b2/dbt/artifacts/resources/v1/saved_query.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.8.0b1/dbt/artifacts/resources/v1/seed.py` & `dbt-core-1.8.0b2/dbt/artifacts/resources/v1/seed.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.8.0b1/dbt/artifacts/resources/v1/semantic_layer_components.py` & `dbt-core-1.8.0b2/dbt/artifacts/resources/v1/semantic_layer_components.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.8.0b1/dbt/artifacts/resources/v1/semantic_model.py` & `dbt-core-1.8.0b2/dbt/artifacts/resources/v1/semantic_model.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.8.0b1/dbt/artifacts/resources/v1/singular_test.py` & `dbt-core-1.8.0b2/dbt/artifacts/resources/v1/singular_test.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.8.0b1/dbt/artifacts/resources/v1/snapshot.py` & `dbt-core-1.8.0b2/dbt/artifacts/resources/v1/snapshot.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.8.0b1/dbt/artifacts/resources/v1/source_definition.py` & `dbt-core-1.8.0b2/dbt/artifacts/resources/v1/source_definition.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.8.0b1/dbt/artifacts/resources/v1/unit_test_definition.py` & `dbt-core-1.8.0b2/dbt/artifacts/resources/v1/unit_test_definition.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.8.0b1/dbt/artifacts/schemas/base.py` & `dbt-core-1.8.0b2/dbt/artifacts/schemas/base.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.8.0b1/dbt/artifacts/schemas/catalog/v1/catalog.py` & `dbt-core-1.8.0b2/dbt/artifacts/schemas/catalog/v1/catalog.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.8.0b1/dbt/artifacts/schemas/freshness/v3/freshness.py` & `dbt-core-1.8.0b2/dbt/artifacts/schemas/freshness/v3/freshness.py`

 * *Files 1% similar despite different names*

```diff
@@ -103,15 +103,19 @@
 ):
     metadata: FreshnessMetadata
     results: Sequence[FreshnessNodeOutput]
     elapsed_time: float
 
     @classmethod
     def from_result(cls, base: FreshnessResult):
-        processed = [process_freshness_result(r) for r in base.results]
+        processed = [
+            process_freshness_result(r)
+            for r in base.results
+            if isinstance(r, SourceFreshnessResult)
+        ]
         return cls(
             metadata=base.metadata,
             results=processed,
             elapsed_time=base.elapsed_time,
         )
```

### Comparing `dbt-core-1.8.0b1/dbt/artifacts/schemas/manifest/v12/manifest.py` & `dbt-core-1.8.0b2/dbt/artifacts/schemas/manifest/v12/manifest.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.8.0b1/dbt/artifacts/schemas/results.py` & `dbt-core-1.8.0b2/dbt/artifacts/schemas/results.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.8.0b1/dbt/artifacts/schemas/run/v5/run.py` & `dbt-core-1.8.0b2/dbt/artifacts/schemas/run/v5/run.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 import threading
-from typing import Any, Optional, Iterable, Tuple, Sequence, Dict
-import agate
+from typing import Any, Optional, Iterable, Tuple, Sequence, Dict, TYPE_CHECKING
 from dataclasses import dataclass, field
 from datetime import datetime
 
 
 from dbt.contracts.graph.nodes import CompiledNode
 from dbt.artifacts.schemas.base import (
     BaseArtifactMetadata,
@@ -18,17 +17,21 @@
     RunStatus,
     ResultNode,
     ExecutionResult,
 )
 from dbt_common.clients.system import write_json
 
 
+if TYPE_CHECKING:
+    import agate
+
+
 @dataclass
 class RunResult(NodeResult):
-    agate_table: Optional[agate.Table] = field(
+    agate_table: Optional["agate.Table"] = field(
         default=None, metadata={"serialize": lambda x: None, "deserialize": lambda x: None}
     )
 
     @property
     def skipped(self):
         return self.status == RunStatus.Skipped
```

### Comparing `dbt-core-1.8.0b1/dbt/artifacts/schemas/upgrades/upgrade_manifest.py` & `dbt-core-1.8.0b2/dbt/artifacts/schemas/upgrades/upgrade_manifest.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.8.0b1/dbt/cli/exceptions.py` & `dbt-core-1.8.0b2/dbt/cli/exceptions.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.8.0b1/dbt/cli/flags.py` & `dbt-core-1.8.0b2/dbt/cli/flags.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,14 +24,15 @@
 if os.name != "nt":
     # https://bugs.python.org/issue41567
     import multiprocessing.popen_spawn_posix  # type: ignore  # noqa: F401
 
 FLAGS_DEFAULTS = {
     "INDIRECT_SELECTION": "eager",
     "TARGET_PATH": None,
+    "DEFER_STATE": None,  # necessary because of retry construction of flags
     "WARN_ERROR": None,
     # Cli args without project_flags or env var option.
     "FULL_REFRESH": False,
     "STRICT_MODE": False,
     "STORE_FAILURES": False,
     "INTROSPECT": True,
 }
@@ -395,15 +396,18 @@
             def add_fn(x):
                 res.insert(0, x)
 
         spinal_cased = k.replace("_", "-")
 
         # MultiOption flags come back as lists, but we want to pass them as space separated strings
         if isinstance(v, list):
-            v = " ".join(v)
+            if len(v) > 0:
+                v = " ".join(v)
+            else:
+                continue
 
         if k == "macro" and command == CliCommand.RUN_OPERATION:
             add_fn(v)
         # None is a Singleton, False is a Flyweight, only one instance of each.
         elif (v is None or v is False) and k not in (
             # These are None by default but they do not support --no-{flag}
             "defer_state",
```

### Comparing `dbt-core-1.8.0b1/dbt/cli/main.py` & `dbt-core-1.8.0b2/dbt/cli/main.py`

 * *Files 7% similar despite different names*

```diff
@@ -16,32 +16,14 @@
     DbtInternalException,
     DbtUsageException,
 )
 from dbt.contracts.graph.manifest import Manifest
 from dbt.artifacts.schemas.catalog import CatalogArtifact
 from dbt.artifacts.schemas.run import RunExecutionResult
 from dbt_common.events.base_types import EventMsg
-from dbt.task.build import BuildTask
-from dbt.task.clean import CleanTask
-from dbt.task.clone import CloneTask
-from dbt.task.compile import CompileTask
-from dbt.task.debug import DebugTask
-from dbt.task.deps import DepsTask
-from dbt.task.docs.generate import GenerateTask
-from dbt.task.docs.serve import ServeTask
-from dbt.task.freshness import FreshnessTask
-from dbt.task.init import InitTask
-from dbt.task.list import ListTask
-from dbt.task.retry import RetryTask
-from dbt.task.run import RunTask
-from dbt.task.run_operation import RunOperationTask
-from dbt.task.seed import SeedTask
-from dbt.task.show import ShowTask
-from dbt.task.snapshot import SnapshotTask
-from dbt.task.test import TestTask
 
 
 @dataclass
 class dbtRunnerResult:
     """Contains the result of an invocation of the dbtRunner"""
 
     success: bool
@@ -68,15 +50,15 @@
 
         if callbacks is None:
             callbacks = []
         self.callbacks = callbacks
 
     def invoke(self, args: List[str], **kwargs) -> dbtRunnerResult:
         try:
-            dbt_ctx = cli.make_context(cli.name, args)
+            dbt_ctx = cli.make_context(cli.name, args.copy())
             dbt_ctx.obj = {
                 "manifest": self.manifest,
                 "callbacks": self.callbacks,
             }
 
             for key, value in kwargs.items():
                 dbt_ctx.params[key] = value
@@ -141,20 +123,22 @@
     @p.macro_debugging
     @p.partial_parse
     @p.partial_parse_file_path
     @p.partial_parse_file_diff
     @p.populate_cache
     @p.print
     @p.printer_width
+    @p.profile
     @p.quiet
     @p.record_timing_info
     @p.send_anonymous_usage_stats
     @p.single_threaded
     @p.state
     @p.static_parser
+    @p.target
     @p.use_colors
     @p.use_colors_file
     @p.use_experimental_parser
     @p.version
     @p.version_check
     @p.warn_error
     @p.warn_error_options
@@ -186,34 +170,35 @@
 @cli.command("build")
 @click.pass_context
 @global_flags
 @p.exclude
 @p.export_saved_queries
 @p.full_refresh
 @p.deprecated_include_saved_query
-@p.profile
 @p.profiles_dir
 @p.project_dir
 @p.resource_type
+@p.exclude_resource_type
 @p.select
 @p.selector
 @p.show
 @p.store_failures
-@p.target
 @p.target_path
 @p.threads
 @p.vars
 @requires.postflight
 @requires.preflight
 @requires.profile
 @requires.project
 @requires.runtime_config
 @requires.manifest
 def build(ctx, **kwargs):
     """Run all seeds, models, snapshots, and tests in DAG order"""
+    from dbt.task.build import BuildTask
+
     task = BuildTask(
         ctx.obj["flags"],
         ctx.obj["runtime_config"],
         ctx.obj["manifest"],
     )
 
     results = task.run()
@@ -222,26 +207,26 @@
 
 
 # dbt clean
 @cli.command("clean")
 @click.pass_context
 @global_flags
 @p.clean_project_files_only
-@p.profile
 @p.profiles_dir
 @p.project_dir
-@p.target
 @p.target_path
 @p.vars
 @requires.postflight
 @requires.preflight
 @requires.unset_profile
 @requires.project
 def clean(ctx, **kwargs):
     """Delete all folders in the clean-targets list (usually the dbt_packages and target directories.)"""
+    from dbt.task.clean import CleanTask
+
     task = CleanTask(ctx.obj["flags"], ctx.obj["project"])
 
     results = task.run()
     success = task.interpret_results(results)
     return results, success
 
 
@@ -255,33 +240,33 @@
 
 # dbt docs generate
 @docs.command("generate")
 @click.pass_context
 @global_flags
 @p.compile_docs
 @p.exclude
-@p.profile
 @p.profiles_dir
 @p.project_dir
 @p.select
 @p.selector
 @p.empty_catalog
 @p.static
-@p.target
 @p.target_path
 @p.threads
 @p.vars
 @requires.postflight
 @requires.preflight
 @requires.profile
 @requires.project
 @requires.runtime_config
 @requires.manifest(write=False)
 def docs_generate(ctx, **kwargs):
     """Generate the documentation website for your project"""
+    from dbt.task.docs.generate import GenerateTask
+
     task = GenerateTask(
         ctx.obj["flags"],
         ctx.obj["runtime_config"],
         ctx.obj["manifest"],
     )
 
     results = task.run()
@@ -291,27 +276,27 @@
 
 # dbt docs serve
 @docs.command("serve")
 @click.pass_context
 @global_flags
 @p.browser
 @p.port
-@p.profile
 @p.profiles_dir
 @p.project_dir
-@p.target
 @p.target_path
 @p.vars
 @requires.postflight
 @requires.preflight
 @requires.profile
 @requires.project
 @requires.runtime_config
 def docs_serve(ctx, **kwargs):
     """Serve the documentation website for your project"""
+    from dbt.task.docs.serve import ServeTask
+
     task = ServeTask(
         ctx.obj["flags"],
         ctx.obj["runtime_config"],
     )
 
     results = task.run()
     success = task.interpret_results(results)
@@ -322,35 +307,35 @@
 @cli.command("compile")
 @click.pass_context
 @global_flags
 @p.exclude
 @p.full_refresh
 @p.show_output_format
 @p.introspect
-@p.profile
 @p.profiles_dir
 @p.project_dir
 @p.empty
 @p.select
 @p.selector
 @p.inline
 @p.compile_inject_ephemeral_ctes
-@p.target
 @p.target_path
 @p.threads
 @p.vars
 @requires.postflight
 @requires.preflight
 @requires.profile
 @requires.project
 @requires.runtime_config
 @requires.manifest
 def compile(ctx, **kwargs):
     """Generates executable SQL from source, model, test, and analysis files. Compiled SQL files are written to the
     target/ directory."""
+    from dbt.task.compile import CompileTask
+
     task = CompileTask(
         ctx.obj["flags"],
         ctx.obj["runtime_config"],
         ctx.obj["manifest"],
     )
 
     results = task.run()
@@ -363,33 +348,33 @@
 @click.pass_context
 @global_flags
 @p.exclude
 @p.full_refresh
 @p.show_output_format
 @p.show_limit
 @p.introspect
-@p.profile
 @p.profiles_dir
 @p.project_dir
 @p.select
 @p.selector
 @p.inline
-@p.target
 @p.target_path
 @p.threads
 @p.vars
 @requires.postflight
 @requires.preflight
 @requires.profile
 @requires.project
 @requires.runtime_config
 @requires.manifest
 def show(ctx, **kwargs):
     """Generates executable SQL for a named resource or inline query, runs that SQL, and returns a preview of the
     results. Does not materialize anything to the warehouse."""
+    from dbt.task.show import ShowTask
+
     task = ShowTask(
         ctx.obj["flags"],
         ctx.obj["runtime_config"],
         ctx.obj["manifest"],
     )
 
     results = task.run()
@@ -399,23 +384,22 @@
 
 # dbt debug
 @cli.command("debug")
 @click.pass_context
 @global_flags
 @p.debug_connection
 @p.config_dir
-@p.profile
 @p.profiles_dir_exists_false
 @p.project_dir
-@p.target
 @p.vars
 @requires.postflight
 @requires.preflight
 def debug(ctx, **kwargs):
     """Show information on the current dbt environment and check dependencies, then test the database connection. Not to be confused with the --debug option which increases verbosity."""
+    from dbt.task.debug import DebugTask
 
     task = DebugTask(
         ctx.obj["flags"],
         None,
     )
 
     results = task.run()
@@ -423,18 +407,16 @@
     return results, success
 
 
 # dbt deps
 @cli.command("deps")
 @click.pass_context
 @global_flags
-@p.profile
 @p.profiles_dir_exists_false
 @p.project_dir
-@p.target
 @p.vars
 @p.source
 @p.lock
 @p.upgrade
 @p.add_package
 @requires.postflight
 @requires.preflight
@@ -447,14 +429,16 @@
     - user specify the flag --update, which means for packages that are specified as a
       range, dbt-core will try to install the newer version
     Otherwise, deps will use `package-lock.yml` as source of truth to install packages.
 
     There is a way to add new packages by providing an `--add-package` flag to deps command
     which will allow user to specify a package they want to add in the format of packagename@version.
     """
+    from dbt.task.deps import DepsTask
+
     flags = ctx.obj["flags"]
     if flags.ADD_PACKAGE:
         if not flags.ADD_PACKAGE["version"] and flags.SOURCE != "local":
             raise BadOptionUsage(
                 message=f"Version is required in --add-package when a package when source is {flags.SOURCE}",
                 option_name="--add-package",
             )
@@ -466,24 +450,24 @@
 
 # dbt init
 @cli.command("init")
 @click.pass_context
 @global_flags
 # for backwards compatibility, accept 'project_name' as an optional positional argument
 @click.argument("project_name", required=False)
-@p.profile
 @p.profiles_dir_exists_false
 @p.project_dir
 @p.skip_profile_setup
-@p.target
 @p.vars
 @requires.postflight
 @requires.preflight
 def init(ctx, **kwargs):
     """Initialize a new dbt project."""
+    from dbt.task.init import InitTask
+
     task = InitTask(ctx.obj["flags"], None)
 
     results = task.run()
     success = task.interpret_results(results)
     return results, success
 
 
@@ -491,31 +475,32 @@
 @cli.command("list")
 @click.pass_context
 @global_flags
 @p.exclude
 @p.models
 @p.output
 @p.output_keys
-@p.profile
 @p.profiles_dir
 @p.project_dir
 @p.resource_type
+@p.exclude_resource_type
 @p.raw_select
 @p.selector
-@p.target
 @p.target_path
 @p.vars
 @requires.postflight
 @requires.preflight
 @requires.profile
 @requires.project
 @requires.runtime_config
 @requires.manifest
 def list(ctx, **kwargs):
     """List the resources in your project"""
+    from dbt.task.list import ListTask
+
     task = ListTask(
         ctx.obj["flags"],
         ctx.obj["runtime_config"],
         ctx.obj["manifest"],
     )
 
     results = task.run()
@@ -529,18 +514,16 @@
 cli.add_command(ls, "ls")
 
 
 # dbt parse
 @cli.command("parse")
 @click.pass_context
 @global_flags
-@p.profile
 @p.profiles_dir
 @p.project_dir
-@p.target
 @p.target_path
 @p.threads
 @p.vars
 @requires.postflight
 @requires.preflight
 @requires.profile
 @requires.project
@@ -554,32 +537,32 @@
 
 # dbt run
 @cli.command("run")
 @click.pass_context
 @global_flags
 @p.exclude
 @p.full_refresh
-@p.profile
 @p.profiles_dir
 @p.project_dir
 @p.empty
 @p.select
 @p.selector
-@p.target
 @p.target_path
 @p.threads
 @p.vars
 @requires.postflight
 @requires.preflight
 @requires.profile
 @requires.project
 @requires.runtime_config
 @requires.manifest
 def run(ctx, **kwargs):
     """Compile SQL and execute against the current target database."""
+    from dbt.task.run import RunTask
+
     task = RunTask(
         ctx.obj["flags"],
         ctx.obj["runtime_config"],
         ctx.obj["manifest"],
     )
 
     results = task.run()
@@ -590,26 +573,26 @@
 # dbt retry
 @cli.command("retry")
 @click.pass_context
 @global_flags
 @p.project_dir
 @p.profiles_dir
 @p.vars
-@p.profile
-@p.target
 @p.target_path
 @p.threads
 @p.full_refresh
 @requires.postflight
 @requires.preflight
 @requires.profile
 @requires.project
 @requires.runtime_config
 def retry(ctx, **kwargs):
     """Retry the nodes that failed in the previous run."""
+    from dbt.task.retry import RetryTask
+
     # Retry will parse manifest inside the task after we consolidate the flags
     task = RetryTask(
         ctx.obj["flags"],
         ctx.obj["runtime_config"],
     )
 
     results = task.run()
@@ -619,32 +602,33 @@
 
 # dbt clone
 @cli.command("clone")
 @click.pass_context
 @global_flags
 @p.exclude
 @p.full_refresh
-@p.profile
 @p.profiles_dir
 @p.project_dir
 @p.resource_type
+@p.exclude_resource_type
 @p.select
 @p.selector
-@p.target
 @p.target_path
 @p.threads
 @p.vars
 @requires.preflight
 @requires.profile
 @requires.project
 @requires.runtime_config
 @requires.manifest
 @requires.postflight
 def clone(ctx, **kwargs):
     """Create clones of selected nodes based on their location in the manifest provided to --state."""
+    from dbt.task.clone import CloneTask
+
     task = CloneTask(
         ctx.obj["flags"],
         ctx.obj["runtime_config"],
         ctx.obj["manifest"],
     )
 
     results = task.run()
@@ -654,29 +638,29 @@
 
 # dbt run operation
 @cli.command("run-operation")
 @click.pass_context
 @global_flags
 @click.argument("macro")
 @p.args
-@p.profile
 @p.profiles_dir
 @p.project_dir
-@p.target
 @p.target_path
 @p.threads
 @p.vars
 @requires.postflight
 @requires.preflight
 @requires.profile
 @requires.project
 @requires.runtime_config
 @requires.manifest
 def run_operation(ctx, **kwargs):
     """Run the named macro with any supplied arguments."""
+    from dbt.task.run_operation import RunOperationTask
+
     task = RunOperationTask(
         ctx.obj["flags"],
         ctx.obj["runtime_config"],
         ctx.obj["manifest"],
     )
 
     results = task.run()
@@ -686,32 +670,32 @@
 
 # dbt seed
 @cli.command("seed")
 @click.pass_context
 @global_flags
 @p.exclude
 @p.full_refresh
-@p.profile
 @p.profiles_dir
 @p.project_dir
 @p.select
 @p.selector
 @p.show
-@p.target
 @p.target_path
 @p.threads
 @p.vars
 @requires.postflight
 @requires.preflight
 @requires.profile
 @requires.project
 @requires.runtime_config
 @requires.manifest
 def seed(ctx, **kwargs):
     """Load data from csv files into your data warehouse."""
+    from dbt.task.seed import SeedTask
+
     task = SeedTask(
         ctx.obj["flags"],
         ctx.obj["runtime_config"],
         ctx.obj["manifest"],
     )
     results = task.run()
     success = task.interpret_results(results)
@@ -719,31 +703,31 @@
 
 
 # dbt snapshot
 @cli.command("snapshot")
 @click.pass_context
 @global_flags
 @p.exclude
-@p.profile
 @p.profiles_dir
 @p.project_dir
 @p.select
 @p.selector
-@p.target
 @p.target_path
 @p.threads
 @p.vars
 @requires.postflight
 @requires.preflight
 @requires.profile
 @requires.project
 @requires.runtime_config
 @requires.manifest
 def snapshot(ctx, **kwargs):
     """Execute snapshots defined in your project"""
+    from dbt.task.snapshot import SnapshotTask
+
     task = SnapshotTask(
         ctx.obj["flags"],
         ctx.obj["runtime_config"],
         ctx.obj["manifest"],
     )
 
     results = task.run()
@@ -761,31 +745,31 @@
 
 # dbt source freshness
 @source.command("freshness")
 @click.pass_context
 @global_flags
 @p.exclude
 @p.output_path  # TODO: Is this ok to re-use?  We have three different output params, how much can we consolidate?
-@p.profile
 @p.profiles_dir
 @p.project_dir
 @p.select
 @p.selector
-@p.target
 @p.target_path
 @p.threads
 @p.vars
 @requires.postflight
 @requires.preflight
 @requires.profile
 @requires.project
 @requires.runtime_config
 @requires.manifest
 def freshness(ctx, **kwargs):
     """check the current freshness of the project's sources"""
+    from dbt.task.freshness import FreshnessTask
+
     task = FreshnessTask(
         ctx.obj["flags"],
         ctx.obj["runtime_config"],
         ctx.obj["manifest"],
     )
 
     results = task.run()
@@ -800,32 +784,32 @@
 
 
 # dbt test
 @cli.command("test")
 @click.pass_context
 @global_flags
 @p.exclude
-@p.profile
 @p.profiles_dir
 @p.project_dir
 @p.select
 @p.selector
 @p.store_failures
-@p.target
 @p.target_path
 @p.threads
 @p.vars
 @requires.postflight
 @requires.preflight
 @requires.profile
 @requires.project
 @requires.runtime_config
 @requires.manifest
 def test(ctx, **kwargs):
     """Runs tests on data in deployed models. Run this after `dbt run`"""
+    from dbt.task.test import TestTask
+
     task = TestTask(
         ctx.obj["flags"],
         ctx.obj["runtime_config"],
         ctx.obj["manifest"],
     )
 
     results = task.run()
```

### Comparing `dbt-core-1.8.0b1/dbt/cli/option_types.py` & `dbt-core-1.8.0b2/dbt/cli/option_types.py`

 * *Files 2% similar despite different names*

```diff
@@ -76,11 +76,14 @@
             return value
 
 
 class ChoiceTuple(Choice):
     name = "CHOICE_TUPLE"
 
     def convert(self, value, param, ctx):
-        for value_item in value:
-            super().convert(value_item, param, ctx)
+        if not isinstance(value, str):
+            for value_item in value:
+                super().convert(value_item, param, ctx)
+        else:
+            super().convert(value, param, ctx)
 
         return value
```

### Comparing `dbt-core-1.8.0b1/dbt/cli/options.py` & `dbt-core-1.8.0b2/dbt/cli/options.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.8.0b1/dbt/cli/params.py` & `dbt-core-1.8.0b2/dbt/cli/params.py`

 * *Files 2% similar despite different names*

```diff
@@ -338,15 +338,15 @@
     help="Sets the width of terminal output",
     type=click.INT,
     default=80,
 )
 
 profile = click.option(
     "--profile",
-    envvar=None,
+    envvar="DBT_PROFILE",
     help="Which existing profile to load. Overrides setting in dbt_project.yml.",
 )
 
 profiles_dir = click.option(
     "--profiles-dir",
     envvar="DBT_PROFILES_DIR",
     help="Which directory to look in for the profiles.yml file. If not set, dbt will look in the current working directory first, then HOME/.dbt/",
@@ -387,37 +387,66 @@
     help="When this option is passed, dbt will output low-level timing stats to the specified file. Example: `--record-timing-info output.profile`",
     type=click.Path(exists=False),
 )
 
 resource_type = click.option(
     "--resource-types",
     "--resource-type",
-    envvar=None,
+    envvar="DBT_RESOURCE_TYPES",
     help="Restricts the types of resources that dbt will include",
     type=ChoiceTuple(
         [
             "metric",
             "semantic_model",
+            "saved_query",
             "source",
             "analysis",
             "model",
             "test",
+            "unit_test",
             "exposure",
             "snapshot",
             "seed",
             "default",
             "all",
         ],
         case_sensitive=False,
     ),
     cls=MultiOption,
     multiple=True,
     default=(),
 )
 
+exclude_resource_type = click.option(
+    "--exclude-resource-types",
+    "--exclude-resource-type",
+    envvar="DBT_EXCLUDE_RESOURCE_TYPES",
+    help="Specify the types of resources that dbt will exclude",
+    type=ChoiceTuple(
+        [
+            "metric",
+            "semantic_model",
+            "saved_query",
+            "source",
+            "analysis",
+            "model",
+            "test",
+            "unit_test",
+            "exposure",
+            "snapshot",
+            "seed",
+            "default",
+        ],
+        case_sensitive=False,
+    ),
+    cls=MultiOption,
+    multiple=True,
+    default=(),
+)
+
 # Renamed to --export-saved-queries
 deprecated_include_saved_query = click.option(
     "--include-saved-query/--no-include-saved-query",
     envvar="DBT_INCLUDE_SAVED_QUERY",
     help="Include saved queries in the list of resources to be selected for build command",
     is_flag=True,
     hidden=True,
@@ -570,15 +599,15 @@
     help="Store test results (failing rows) in the database",
     is_flag=True,
 )
 
 target = click.option(
     "--target",
     "-t",
-    envvar=None,
+    envvar="DBT_TARGET",
     help="Which target to load for the given profile",
 )
 
 target_path = click.option(
     "--target-path",
     envvar="DBT_TARGET_PATH",
     help="Configure the 'target-path'. Only applies this setting for the current run. Overrides the 'DBT_TARGET_PATH' if it is set.",
```

### Comparing `dbt-core-1.8.0b1/dbt/cli/requires.py` & `dbt-core-1.8.0b2/dbt/cli/requires.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.8.0b1/dbt/cli/resolvers.py` & `dbt-core-1.8.0b2/dbt/cli/resolvers.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.8.0b1/dbt/cli/types.py` & `dbt-core-1.8.0b2/dbt/cli/types.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.8.0b1/dbt/clients/git.py` & `dbt-core-1.8.0b2/dbt/clients/git.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.8.0b1/dbt/clients/jinja.py` & `dbt-core-1.8.0b2/dbt/clients/jinja.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.8.0b1/dbt/clients/jinja_static.py` & `dbt-core-1.8.0b2/dbt/clients/jinja_static.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.8.0b1/dbt/clients/registry.py` & `dbt-core-1.8.0b2/dbt/clients/registry.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.8.0b1/dbt/clients/yaml_helper.py` & `dbt-core-1.8.0b2/dbt/clients/yaml_helper.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.8.0b1/dbt/compilation.py` & `dbt-core-1.8.0b2/dbt/compilation.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.8.0b1/dbt/config/profile.py` & `dbt-core-1.8.0b2/dbt/config/profile.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.8.0b1/dbt/config/project.py` & `dbt-core-1.8.0b2/dbt/config/project.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.8.0b1/dbt/config/renderer.py` & `dbt-core-1.8.0b2/dbt/config/renderer.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.8.0b1/dbt/config/runtime.py` & `dbt-core-1.8.0b2/dbt/config/runtime.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.8.0b1/dbt/config/selectors.py` & `dbt-core-1.8.0b2/dbt/config/selectors.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.8.0b1/dbt/config/utils.py` & `dbt-core-1.8.0b2/dbt/config/utils.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.8.0b1/dbt/constants.py` & `dbt-core-1.8.0b2/dbt/constants.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.8.0b1/dbt/context/base.py` & `dbt-core-1.8.0b2/dbt/context/base.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.8.0b1/dbt/context/configured.py` & `dbt-core-1.8.0b2/dbt/context/configured.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.8.0b1/dbt/context/context_config.py` & `dbt-core-1.8.0b2/dbt/context/context_config.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.8.0b1/dbt/context/docs.py` & `dbt-core-1.8.0b2/dbt/context/docs.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.8.0b1/dbt/context/exceptions_jinja.py` & `dbt-core-1.8.0b2/dbt/context/exceptions_jinja.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.8.0b1/dbt/context/macro_resolver.py` & `dbt-core-1.8.0b2/dbt/context/macro_resolver.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.8.0b1/dbt/context/macros.py` & `dbt-core-1.8.0b2/dbt/context/macros.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.8.0b1/dbt/context/manifest.py` & `dbt-core-1.8.0b2/dbt/context/manifest.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.8.0b1/dbt/context/providers.py` & `dbt-core-1.8.0b2/dbt/context/providers.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,24 +8,25 @@
     Optional,
     Union,
     List,
     TypeVar,
     Type,
     Iterable,
     Mapping,
+    Tuple,
+    TYPE_CHECKING,
 )
 
 from typing_extensions import Protocol
 
 from dbt.adapters.base.column import Column
 from dbt.artifacts.resources import NodeVersion, RefArgs
 from dbt_common.clients.jinja import MacroProtocol
 from dbt_common.context import get_invocation_context
 from dbt.adapters.factory import get_adapter, get_adapter_package_names, get_adapter_type_names
-from dbt_common.clients import agate_helper
 from dbt.clients.jinja import get_rendered, MacroGenerator, MacroStack, UnitTestMacroGenerator
 from dbt.config import RuntimeConfig, Project
 from dbt.constants import SECRET_ENV_PREFIX, DEFAULT_ENV_PLACEHOLDER
 from dbt.context.base import contextmember, contextproperty, Var
 from dbt.context.configured import FQNLookup
 from dbt.context.context_config import ContextConfig
 from dbt.context.exceptions_jinja import wrapped_exports
@@ -77,15 +78,16 @@
 from dbt.config import IsFQNResource
 from dbt.node_types import NodeType, ModelLanguage
 
 from dbt.utils import MultiDict, args_to_dict
 from dbt_common.utils import merge, AttrDict, cast_to_str
 from dbt import selected_resources
 
-import agate
+if TYPE_CHECKING:
+    import agate
 
 
 _MISSING = object()
 
 
 # base classes
 class RelationProxy:
@@ -846,16 +848,18 @@
                 return ret_val
         else:
             # Handle trying to load a result that was never stored
             return None
 
     @contextmember()
     def store_result(
-        self, name: str, response: Any, agate_table: Optional[agate.Table] = None
+        self, name: str, response: Any, agate_table: Optional["agate.Table"] = None
     ) -> str:
+        from dbt_common.clients import agate_helper
+
         if agate_table is None:
             agate_table = agate_helper.empty_table()
 
         self.sql_results[name] = AttrDict(
             {
                 "response": response,
                 "data": agate_helper.as_matrix(agate_table),
@@ -867,15 +871,15 @@
     @contextmember()
     def store_raw_result(
         self,
         name: str,
         message=Optional[str],
         code=Optional[str],
         rows_affected=Optional[str],
-        agate_table: Optional[agate.Table] = None,
+        agate_table: Optional["agate.Table"] = None,
     ) -> str:
         response = AdapterResponse(_message=message, code=code, rows_affected=rows_affected)
         return self.store_result(name, response, agate_table)
 
     @contextproperty()
     def validation(self):
         def validate_any(*args) -> Callable[[T], None]:
@@ -916,15 +920,17 @@
     ) -> Any:
         try:
             return func(*args, **kwargs)
         except Exception:
             raise CompilationError(message_if_exception, self.model)
 
     @contextmember()
-    def load_agate_table(self) -> agate.Table:
+    def load_agate_table(self) -> "agate.Table":
+        from dbt_common.clients import agate_helper
+
         if not isinstance(self.model, SeedNode):
             raise LoadAgateTableNotSeedError(self.model.resource_type, node=self.model)
 
         # include package_path for seeds defined in packages
         package_path = (
             os.path.join(self.config.packages_install_path, self.model.package_name)
             if self.model.package_name != self.config.project_name
@@ -1616,20 +1622,55 @@
     config: RuntimeConfig,
     manifest: Manifest,
 ) -> Dict[str, Any]:
     ctx = UnitTestContext(unit_test, config, manifest, RuntimeUnitTestProvider(), None)
     ctx_dict = ctx.to_dict()
 
     if unit_test.overrides and unit_test.overrides.macros:
+        global_macro_overrides: Dict[str, Any] = {}
+        package_macro_overrides: Dict[Tuple[str, str], Any] = {}
+
+        # split macro overrides into global and package-namespaced collections
         for macro_name, macro_value in unit_test.overrides.macros.items():
-            context_value = ctx_dict.get(macro_name)
-            if isinstance(context_value, MacroGenerator):
-                ctx_dict[macro_name] = UnitTestMacroGenerator(context_value, macro_value)
-            else:
+            macro_name_split = macro_name.split(".")
+            macro_package = macro_name_split[0] if len(macro_name_split) == 2 else None
+            macro_name = macro_name_split[-1]
+
+            # macro overrides of global macros
+            if macro_package is None and macro_name in ctx_dict:
+                original_context_value = ctx_dict[macro_name]
+                if isinstance(original_context_value, MacroGenerator):
+                    macro_value = UnitTestMacroGenerator(original_context_value, macro_value)
+                global_macro_overrides[macro_name] = macro_value
+
+            # macro overrides of package-namespaced macros
+            elif (
+                macro_package
+                and macro_package in ctx_dict
+                and macro_name in ctx_dict[macro_package]
+            ):
+                original_context_value = ctx_dict[macro_package][macro_name]
+                if isinstance(original_context_value, MacroGenerator):
+                    macro_value = UnitTestMacroGenerator(original_context_value, macro_value)
+                package_macro_overrides[(macro_package, macro_name)] = macro_value
+
+        # macro overrides of package-namespaced macros
+        for (macro_package, macro_name), macro_override_value in package_macro_overrides.items():
+            ctx_dict[macro_package][macro_name] = macro_override_value
+            # propgate override of namespaced dbt macro to global namespace
+            if macro_package == "dbt":
                 ctx_dict[macro_name] = macro_value
+
+        # macro overrides of global macros, which should take precedence over equivalent package-namespaced overrides
+        for macro_name, macro_override_value in global_macro_overrides.items():
+            ctx_dict[macro_name] = macro_override_value
+            # propgate override of global dbt macro to dbt namespace
+            if ctx_dict["dbt"].get(macro_name):
+                ctx_dict["dbt"][macro_name] = macro_override_value
+
     return ctx_dict
 
 
 class ExposureRefResolver(BaseResolver):
     def __call__(self, *args, **kwargs) -> str:
         package = None
         if len(args) == 1:
```

### Comparing `dbt-core-1.8.0b1/dbt/context/secret.py` & `dbt-core-1.8.0b2/dbt/context/secret.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.8.0b1/dbt/context/target.py` & `dbt-core-1.8.0b2/dbt/context/target.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.8.0b1/dbt/contracts/files.py` & `dbt-core-1.8.0b2/dbt/contracts/files.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.8.0b1/dbt/contracts/graph/manifest.py` & `dbt-core-1.8.0b2/dbt/contracts/graph/manifest.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.8.0b1/dbt/contracts/graph/metrics.py` & `dbt-core-1.8.0b2/dbt/contracts/graph/metrics.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.8.0b1/dbt/contracts/graph/model_config.py` & `dbt-core-1.8.0b2/dbt/contracts/graph/model_config.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.8.0b1/dbt/contracts/graph/node_args.py` & `dbt-core-1.8.0b2/dbt/contracts/graph/node_args.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.8.0b1/dbt/contracts/graph/nodes.py` & `dbt-core-1.8.0b2/dbt/contracts/graph/nodes.py`

 * *Files 1% similar despite different names*

```diff
@@ -83,14 +83,15 @@
     SqlOperation as SqlOperationResource,
     Seed as SeedResource,
     SingularTest as SingularTestResource,
     GenericTest as GenericTestResource,
     Snapshot as SnapshotResource,
     Quoting as QuotingResource,
     SourceDefinition as SourceDefinitionResource,
+    MetricInputMeasure,
     UnitTestDefinition as UnitTestDefinitionResource,
 )
 
 # =====================================================================
 # This contains the classes for all of the nodes and node-like objects
 # in the manifest. In the "nodes" dictionary of the manifest we find
 # all of the objects in the ManifestNode union below. In addition the
@@ -950,24 +951,14 @@
 @dataclass
 class UnitTestDefinition(NodeInfoMixin, GraphNode, UnitTestDefinitionResource):
     @classmethod
     def resource_class(cls) -> Type[UnitTestDefinitionResource]:
         return UnitTestDefinitionResource
 
     @property
-    def build_path(self):
-        # TODO: is this actually necessary?
-        return self.original_file_path
-
-    @property
-    def compiled_path(self):
-        # TODO: is this actually necessary?
-        return self.original_file_path
-
-    @property
     def depends_on_nodes(self):
         return self.depends_on.nodes
 
     @property
     def tags(self) -> List[str]:
         tags = self.config.tags
         return [tags] if isinstance(tags, str) else tags
@@ -1407,14 +1398,20 @@
             and self.same_type_params(old)
             and self.same_description(old)
             and self.same_label(old)
             and self.same_config(old)
             and True
         )
 
+    def add_input_measure(self, input_measure: MetricInputMeasure) -> None:
+        for existing_input_measure in self.type_params.input_measures:
+            if input_measure == existing_input_measure:
+                return
+        self.type_params.input_measures.append(input_measure)
+
 
 # ====================================
 # Group node
 # ====================================
 
 
 @dataclass
```

### Comparing `dbt-core-1.8.0b1/dbt/contracts/graph/semantic_manifest.py` & `dbt-core-1.8.0b2/dbt/contracts/graph/semantic_manifest.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.8.0b1/dbt/contracts/graph/unparsed.py` & `dbt-core-1.8.0b2/dbt/contracts/graph/unparsed.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.8.0b1/dbt/contracts/graph/utils.py` & `dbt-core-1.8.0b2/dbt/contracts/graph/utils.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.8.0b1/dbt/contracts/project.py` & `dbt-core-1.8.0b2/dbt/contracts/project.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.8.0b1/dbt/contracts/results.py` & `dbt-core-1.8.0b2/dbt/contracts/results.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.8.0b1/dbt/contracts/selection.py` & `dbt-core-1.8.0b2/dbt/contracts/selection.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.8.0b1/dbt/contracts/sql.py` & `dbt-core-1.8.0b2/dbt/contracts/sql.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.8.0b1/dbt/contracts/state.py` & `dbt-core-1.8.0b2/dbt/contracts/state.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.8.0b1/dbt/contracts/util.py` & `dbt-core-1.8.0b2/dbt/contracts/util.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.8.0b1/dbt/deprecations.py` & `dbt-core-1.8.0b2/dbt/deprecations.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.8.0b1/dbt/deps/base.py` & `dbt-core-1.8.0b2/dbt/deps/base.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.8.0b1/dbt/deps/git.py` & `dbt-core-1.8.0b2/dbt/deps/git.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.8.0b1/dbt/deps/local.py` & `dbt-core-1.8.0b2/dbt/deps/local.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.8.0b1/dbt/deps/registry.py` & `dbt-core-1.8.0b2/dbt/deps/registry.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.8.0b1/dbt/deps/resolver.py` & `dbt-core-1.8.0b2/dbt/deps/resolver.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.8.0b1/dbt/deps/tarball.py` & `dbt-core-1.8.0b2/dbt/deps/tarball.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.8.0b1/dbt/docs/source/_ext/dbt_click.py` & `dbt-core-1.8.0b2/dbt/docs/source/_ext/dbt_click.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.8.0b1/dbt/docs/source/conf.py` & `dbt-core-1.8.0b2/dbt/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.8.0b1/dbt/events/base_types.py` & `dbt-core-1.8.0b2/dbt/events/base_types.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.8.0b1/dbt/events/core_types_pb2.py` & `dbt-core-1.8.0b2/dbt/events/core_types_pb2.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 _sym_db = _symbol_database.Default()
 
 
 from google.protobuf import timestamp_pb2 as google_dot_protobuf_dot_timestamp__pb2
 from google.protobuf import struct_pb2 as google_dot_protobuf_dot_struct__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x10\x63ore_types.proto\x12\x0bproto_types\x1a\x1fgoogle/protobuf/timestamp.proto\x1a\x1cgoogle/protobuf/struct.proto\"\x99\x02\n\rCoreEventInfo\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x0c\n\x04\x63ode\x18\x02 \x01(\t\x12\x0b\n\x03msg\x18\x03 \x01(\t\x12\r\n\x05level\x18\x04 \x01(\t\x12\x15\n\rinvocation_id\x18\x05 \x01(\t\x12\x0b\n\x03pid\x18\x06 \x01(\x05\x12\x0e\n\x06thread\x18\x07 \x01(\t\x12&\n\x02ts\x18\x08 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x34\n\x05\x65xtra\x18\t \x03(\x0b\x32%.proto_types.CoreEventInfo.ExtraEntry\x12\x10\n\x08\x63\x61tegory\x18\n \x01(\t\x1a,\n\nExtraEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"V\n\x0cNodeRelation\x12\x10\n\x08\x64\x61tabase\x18\n \x01(\t\x12\x0e\n\x06schema\x18\x0b \x01(\t\x12\r\n\x05\x61lias\x18\x0c \x01(\t\x12\x15\n\rrelation_name\x18\r \x01(\t\"\x91\x02\n\x08NodeInfo\x12\x11\n\tnode_path\x18\x01 \x01(\t\x12\x11\n\tnode_name\x18\x02 \x01(\t\x12\x11\n\tunique_id\x18\x03 \x01(\t\x12\x15\n\rresource_type\x18\x04 \x01(\t\x12\x14\n\x0cmaterialized\x18\x05 \x01(\t\x12\x13\n\x0bnode_status\x18\x06 \x01(\t\x12\x17\n\x0fnode_started_at\x18\x07 \x01(\t\x12\x18\n\x10node_finished_at\x18\x08 \x01(\t\x12%\n\x04meta\x18\t \x01(\x0b\x32\x17.google.protobuf.Struct\x12\x30\n\rnode_relation\x18\n \x01(\x0b\x32\x19.proto_types.NodeRelation\"\x7f\n\rTimingInfoMsg\x12\x0c\n\x04name\x18\x01 \x01(\t\x12.\n\nstarted_at\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x30\n\x0c\x63ompleted_at\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\"\xd1\x01\n\x0cRunResultMsg\x12\x0e\n\x06status\x18\x01 \x01(\t\x12\x0f\n\x07message\x18\x02 \x01(\t\x12/\n\x0btiming_info\x18\x03 \x03(\x0b\x32\x1a.proto_types.TimingInfoMsg\x12\x0e\n\x06thread\x18\x04 \x01(\t\x12\x16\n\x0e\x65xecution_time\x18\x05 \x01(\x02\x12\x31\n\x10\x61\x64\x61pter_response\x18\x06 \x01(\x0b\x32\x17.google.protobuf.Struct\x12\x14\n\x0cnum_failures\x18\x07 \x01(\x05\"\\\n\nColumnType\x12\x13\n\x0b\x63olumn_name\x18\x01 \x01(\t\x12\x1c\n\x14previous_column_type\x18\x02 \x01(\t\x12\x1b\n\x13\x63urrent_column_type\x18\x03 \x01(\t\"Y\n\x10\x43olumnConstraint\x12\x13\n\x0b\x63olumn_name\x18\x01 \x01(\t\x12\x17\n\x0f\x63onstraint_name\x18\x02 \x01(\t\x12\x17\n\x0f\x63onstraint_type\x18\x03 \x01(\t\"T\n\x0fModelConstraint\x12\x17\n\x0f\x63onstraint_name\x18\x01 \x01(\t\x12\x17\n\x0f\x63onstraint_type\x18\x02 \x01(\t\x12\x0f\n\x07\x63olumns\x18\x03 \x03(\t\"9\n\x11MainReportVersion\x12\x0f\n\x07version\x18\x01 \x01(\t\x12\x13\n\x0blog_version\x18\x02 \x01(\x05\"n\n\x14MainReportVersionMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12,\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1e.proto_types.MainReportVersion\"r\n\x0eMainReportArgs\x12\x33\n\x04\x61rgs\x18\x01 \x03(\x0b\x32%.proto_types.MainReportArgs.ArgsEntry\x1a+\n\tArgsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"h\n\x11MainReportArgsMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12)\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1b.proto_types.MainReportArgs\"+\n\x15MainTrackingUserState\x12\x12\n\nuser_state\x18\x01 \x01(\t\"v\n\x18MainTrackingUserStateMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12\x30\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\".proto_types.MainTrackingUserState\"5\n\x0fMergedFromState\x12\x12\n\nnum_merged\x18\x01 \x01(\x05\x12\x0e\n\x06sample\x18\x02 \x03(\t\"j\n\x12MergedFromStateMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12*\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1c.proto_types.MergedFromState\"A\n\x14MissingProfileTarget\x12\x14\n\x0cprofile_name\x18\x01 \x01(\t\x12\x13\n\x0btarget_name\x18\x02 \x01(\t\"t\n\x17MissingProfileTargetMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12/\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32!.proto_types.MissingProfileTarget\"(\n\x11InvalidOptionYAML\x12\x13\n\x0boption_name\x18\x01 \x01(\t\"n\n\x14InvalidOptionYAMLMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12,\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1e.proto_types.InvalidOptionYAML\"!\n\x12LogDbtProjectError\x12\x0b\n\x03\x65xc\x18\x01 \x01(\t\"p\n\x15LogDbtProjectErrorMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12-\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1f.proto_types.LogDbtProjectError\"3\n\x12LogDbtProfileError\x12\x0b\n\x03\x65xc\x18\x01 \x01(\t\x12\x10\n\x08profiles\x18\x02 \x03(\t\"p\n\x15LogDbtProfileErrorMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12-\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1f.proto_types.LogDbtProfileError\"!\n\x12StarterProjectPath\x12\x0b\n\x03\x64ir\x18\x01 \x01(\t\"p\n\x15StarterProjectPathMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12-\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1f.proto_types.StarterProjectPath\"$\n\x15\x43onfigFolderDirectory\x12\x0b\n\x03\x64ir\x18\x01 \x01(\t\"v\n\x18\x43onfigFolderDirectoryMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12\x30\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\".proto_types.ConfigFolderDirectory\"\'\n\x14NoSampleProfileFound\x12\x0f\n\x07\x61\x64\x61pter\x18\x01 \x01(\t\"t\n\x17NoSampleProfileFoundMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12/\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32!.proto_types.NoSampleProfileFound\"6\n\x18ProfileWrittenWithSample\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x0c\n\x04path\x18\x02 \x01(\t\"|\n\x1bProfileWrittenWithSampleMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12\x33\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32%.proto_types.ProfileWrittenWithSample\"B\n$ProfileWrittenWithTargetTemplateYAML\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x0c\n\x04path\x18\x02 \x01(\t\"\x94\x01\n\'ProfileWrittenWithTargetTemplateYAMLMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12?\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x31.proto_types.ProfileWrittenWithTargetTemplateYAML\"C\n%ProfileWrittenWithProjectTemplateYAML\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x0c\n\x04path\x18\x02 \x01(\t\"\x96\x01\n(ProfileWrittenWithProjectTemplateYAMLMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12@\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x32.proto_types.ProfileWrittenWithProjectTemplateYAML\"\x12\n\x10SettingUpProfile\"l\n\x13SettingUpProfileMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12+\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1d.proto_types.SettingUpProfile\"\x1c\n\x1aInvalidProfileTemplateYAML\"\x80\x01\n\x1dInvalidProfileTemplateYAMLMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12\x35\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\'.proto_types.InvalidProfileTemplateYAML\"(\n\x18ProjectNameAlreadyExists\x12\x0c\n\x04name\x18\x01 \x01(\t\"|\n\x1bProjectNameAlreadyExistsMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12\x33\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32%.proto_types.ProjectNameAlreadyExists\"K\n\x0eProjectCreated\x12\x14\n\x0cproject_name\x18\x01 \x01(\t\x12\x10\n\x08\x64ocs_url\x18\x02 \x01(\t\x12\x11\n\tslack_url\x18\x03 \x01(\t\"h\n\x11ProjectCreatedMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12)\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1b.proto_types.ProjectCreated\"@\n\x1aPackageRedirectDeprecation\x12\x10\n\x08old_name\x18\x01 \x01(\t\x12\x10\n\x08new_name\x18\x02 \x01(\t\"\x80\x01\n\x1dPackageRedirectDeprecationMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12\x35\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\'.proto_types.PackageRedirectDeprecation\"\x1f\n\x1dPackageInstallPathDeprecation\"\x86\x01\n PackageInstallPathDeprecationMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12\x38\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32*.proto_types.PackageInstallPathDeprecation\"H\n\x1b\x43onfigSourcePathDeprecation\x12\x17\n\x0f\x64\x65precated_path\x18\x01 \x01(\t\x12\x10\n\x08\x65xp_path\x18\x02 \x01(\t\"\x82\x01\n\x1e\x43onfigSourcePathDeprecationMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12\x36\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32(.proto_types.ConfigSourcePathDeprecation\"F\n\x19\x43onfigDataPathDeprecation\x12\x17\n\x0f\x64\x65precated_path\x18\x01 \x01(\t\x12\x10\n\x08\x65xp_path\x18\x02 \x01(\t\"~\n\x1c\x43onfigDataPathDeprecationMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12\x34\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32&.proto_types.ConfigDataPathDeprecation\".\n\x17MetricAttributesRenamed\x12\x13\n\x0bmetric_name\x18\x01 \x01(\t\"z\n\x1aMetricAttributesRenamedMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12\x32\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32$.proto_types.MetricAttributesRenamed\"+\n\x17\x45xposureNameDeprecation\x12\x10\n\x08\x65xposure\x18\x01 \x01(\t\"z\n\x1a\x45xposureNameDeprecationMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12\x32\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32$.proto_types.ExposureNameDeprecation\"^\n\x13InternalDeprecation\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x0e\n\x06reason\x18\x02 \x01(\t\x12\x18\n\x10suggested_action\x18\x03 \x01(\t\x12\x0f\n\x07version\x18\x04 \x01(\t\"r\n\x16InternalDeprecationMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12.\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32 .proto_types.InternalDeprecation\"@\n\x1a\x45nvironmentVariableRenamed\x12\x10\n\x08old_name\x18\x01 \x01(\t\x12\x10\n\x08new_name\x18\x02 \x01(\t\"\x80\x01\n\x1d\x45nvironmentVariableRenamedMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12\x35\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\'.proto_types.EnvironmentVariableRenamed\"3\n\x18\x43onfigLogPathDeprecation\x12\x17\n\x0f\x64\x65precated_path\x18\x01 \x01(\t\"|\n\x1b\x43onfigLogPathDeprecationMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12\x33\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32%.proto_types.ConfigLogPathDeprecation\"6\n\x1b\x43onfigTargetPathDeprecation\x12\x17\n\x0f\x64\x65precated_path\x18\x01 \x01(\t\"\x82\x01\n\x1e\x43onfigTargetPathDeprecationMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12\x36\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32(.proto_types.ConfigTargetPathDeprecation\"C\n\x16TestsConfigDeprecation\x12\x17\n\x0f\x64\x65precated_path\x18\x01 \x01(\t\x12\x10\n\x08\x65xp_path\x18\x02 \x01(\t\"x\n\x19TestsConfigDeprecationMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12\x31\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32#.proto_types.TestsConfigDeprecation\"\x1e\n\x1cProjectFlagsMovedDeprecation\"\x84\x01\n\x1fProjectFlagsMovedDeprecationMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12\x37\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32).proto_types.ProjectFlagsMovedDeprecation\"V\n\x0f\x44\x65precatedModel\x12\x12\n\nmodel_name\x18\x01 \x01(\t\x12\x15\n\rmodel_version\x18\x02 \x01(\t\x12\x18\n\x10\x64\x65precation_date\x18\x03 \x01(\t\"j\n\x12\x44\x65precatedModelMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12*\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1c.proto_types.DeprecatedModel\"7\n\x12InputFileDiffError\x12\x10\n\x08\x63\x61tegory\x18\x01 \x01(\t\x12\x0f\n\x07\x66ile_id\x18\x02 \x01(\t\"p\n\x15InputFileDiffErrorMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12-\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1f.proto_types.InputFileDiffError\"?\n\x14InvalidValueForField\x12\x12\n\nfield_name\x18\x01 \x01(\t\x12\x13\n\x0b\x66ield_value\x18\x02 \x01(\t\"t\n\x17InvalidValueForFieldMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12/\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32!.proto_types.InvalidValueForField\"Q\n\x11ValidationWarning\x12\x15\n\rresource_type\x18\x01 \x01(\t\x12\x12\n\nfield_name\x18\x02 \x01(\t\x12\x11\n\tnode_name\x18\x03 \x01(\t\"n\n\x14ValidationWarningMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12,\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1e.proto_types.ValidationWarning\"!\n\x11ParsePerfInfoPath\x12\x0c\n\x04path\x18\x01 \x01(\t\"n\n\x14ParsePerfInfoPathMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12,\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1e.proto_types.ParsePerfInfoPath\"1\n!PartialParsingErrorProcessingFile\x12\x0c\n\x04\x66ile\x18\x01 \x01(\t\"\x8e\x01\n$PartialParsingErrorProcessingFileMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12<\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32..proto_types.PartialParsingErrorProcessingFile\"\x86\x01\n\x13PartialParsingError\x12?\n\x08\x65xc_info\x18\x01 \x03(\x0b\x32-.proto_types.PartialParsingError.ExcInfoEntry\x1a.\n\x0c\x45xcInfoEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"r\n\x16PartialParsingErrorMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12.\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32 .proto_types.PartialParsingError\"\x1b\n\x19PartialParsingSkipParsing\"~\n\x1cPartialParsingSkipParsingMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12\x34\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32&.proto_types.PartialParsingSkipParsing\"&\n\x14UnableToPartialParse\x12\x0e\n\x06reason\x18\x01 \x01(\t\"t\n\x17UnableToPartialParseMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12/\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32!.proto_types.UnableToPartialParse\"f\n\x12StateCheckVarsHash\x12\x10\n\x08\x63hecksum\x18\x01 \x01(\t\x12\x0c\n\x04vars\x18\x02 \x01(\t\x12\x0f\n\x07profile\x18\x03 \x01(\t\x12\x0e\n\x06target\x18\x04 \x01(\t\x12\x0f\n\x07version\x18\x05 \x01(\t\"p\n\x15StateCheckVarsHashMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12-\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1f.proto_types.StateCheckVarsHash\"\x1a\n\x18PartialParsingNotEnabled\"|\n\x1bPartialParsingNotEnabledMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12\x33\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32%.proto_types.PartialParsingNotEnabled\"C\n\x14ParsedFileLoadFailed\x12\x0c\n\x04path\x18\x01 \x01(\t\x12\x0b\n\x03\x65xc\x18\x02 \x01(\t\x12\x10\n\x08\x65xc_info\x18\x03 \x01(\t\"t\n\x17ParsedFileLoadFailedMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12/\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32!.proto_types.ParsedFileLoadFailed\"H\n\x15PartialParsingEnabled\x12\x0f\n\x07\x64\x65leted\x18\x01 \x01(\x05\x12\r\n\x05\x61\x64\x64\x65\x64\x18\x02 \x01(\x05\x12\x0f\n\x07\x63hanged\x18\x03 \x01(\x05\"v\n\x18PartialParsingEnabledMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12\x30\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\".proto_types.PartialParsingEnabled\"8\n\x12PartialParsingFile\x12\x0f\n\x07\x66ile_id\x18\x01 \x01(\t\x12\x11\n\toperation\x18\x02 \x01(\t\"p\n\x15PartialParsingFileMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12-\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1f.proto_types.PartialParsingFile\"\xaf\x01\n\x1fInvalidDisabledTargetInTestNode\x12\x1b\n\x13resource_type_title\x18\x01 \x01(\t\x12\x11\n\tunique_id\x18\x02 \x01(\t\x12\x1a\n\x12original_file_path\x18\x03 \x01(\t\x12\x13\n\x0btarget_kind\x18\x04 \x01(\t\x12\x13\n\x0btarget_name\x18\x05 \x01(\t\x12\x16\n\x0etarget_package\x18\x06 \x01(\t\"\x8a\x01\n\"InvalidDisabledTargetInTestNodeMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12:\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32,.proto_types.InvalidDisabledTargetInTestNode\"7\n\x18UnusedResourceConfigPath\x12\x1b\n\x13unused_config_paths\x18\x01 \x03(\t\"|\n\x1bUnusedResourceConfigPathMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12\x33\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32%.proto_types.UnusedResourceConfigPath\"3\n\rSeedIncreased\x12\x14\n\x0cpackage_name\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\"f\n\x10SeedIncreasedMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12(\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1a.proto_types.SeedIncreased\">\n\x18SeedExceedsLimitSamePath\x12\x14\n\x0cpackage_name\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\"|\n\x1bSeedExceedsLimitSamePathMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12\x33\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32%.proto_types.SeedExceedsLimitSamePath\"D\n\x1eSeedExceedsLimitAndPathChanged\x12\x14\n\x0cpackage_name\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\"\x88\x01\n!SeedExceedsLimitAndPathChangedMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12\x39\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32+.proto_types.SeedExceedsLimitAndPathChanged\"\\\n\x1fSeedExceedsLimitChecksumChanged\x12\x14\n\x0cpackage_name\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\x12\x15\n\rchecksum_name\x18\x03 \x01(\t\"\x8a\x01\n\"SeedExceedsLimitChecksumChangedMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12:\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32,.proto_types.SeedExceedsLimitChecksumChanged\"%\n\x0cUnusedTables\x12\x15\n\runused_tables\x18\x01 \x03(\t\"d\n\x0fUnusedTablesMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12\'\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x19.proto_types.UnusedTables\"\x87\x01\n\x17WrongResourceSchemaFile\x12\x12\n\npatch_name\x18\x01 \x01(\t\x12\x15\n\rresource_type\x18\x02 \x01(\t\x12\x1c\n\x14plural_resource_type\x18\x03 \x01(\t\x12\x10\n\x08yaml_key\x18\x04 \x01(\t\x12\x11\n\tfile_path\x18\x05 \x01(\t\"z\n\x1aWrongResourceSchemaFileMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12\x32\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32$.proto_types.WrongResourceSchemaFile\"K\n\x10NoNodeForYamlKey\x12\x12\n\npatch_name\x18\x01 \x01(\t\x12\x10\n\x08yaml_key\x18\x02 \x01(\t\x12\x11\n\tfile_path\x18\x03 \x01(\t\"l\n\x13NoNodeForYamlKeyMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12+\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1d.proto_types.NoNodeForYamlKey\"+\n\x15MacroNotFoundForPatch\x12\x12\n\npatch_name\x18\x01 \x01(\t\"v\n\x18MacroNotFoundForPatchMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12\x30\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\".proto_types.MacroNotFoundForPatch\"\xb8\x01\n\x16NodeNotFoundOrDisabled\x12\x1a\n\x12original_file_path\x18\x01 \x01(\t\x12\x11\n\tunique_id\x18\x02 \x01(\t\x12\x1b\n\x13resource_type_title\x18\x03 \x01(\t\x12\x13\n\x0btarget_name\x18\x04 \x01(\t\x12\x13\n\x0btarget_kind\x18\x05 \x01(\t\x12\x16\n\x0etarget_package\x18\x06 \x01(\t\x12\x10\n\x08\x64isabled\x18\x07 \x01(\t\"x\n\x19NodeNotFoundOrDisabledMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12\x31\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32#.proto_types.NodeNotFoundOrDisabled\"H\n\x0fJinjaLogWarning\x12(\n\tnode_info\x18\x01 \x01(\x0b\x32\x15.proto_types.NodeInfo\x12\x0b\n\x03msg\x18\x02 \x01(\t\"j\n\x12JinjaLogWarningMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12*\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1c.proto_types.JinjaLogWarning\"E\n\x0cJinjaLogInfo\x12(\n\tnode_info\x18\x01 \x01(\x0b\x32\x15.proto_types.NodeInfo\x12\x0b\n\x03msg\x18\x02 \x01(\t\"d\n\x0fJinjaLogInfoMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12\'\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x19.proto_types.JinjaLogInfo\"F\n\rJinjaLogDebug\x12(\n\tnode_info\x18\x01 \x01(\x0b\x32\x15.proto_types.NodeInfo\x12\x0b\n\x03msg\x18\x02 \x01(\t\"f\n\x10JinjaLogDebugMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12(\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1a.proto_types.JinjaLogDebug\"\xae\x01\n\x1eUnpinnedRefNewVersionAvailable\x12(\n\tnode_info\x18\x01 \x01(\x0b\x32\x15.proto_types.NodeInfo\x12\x15\n\rref_node_name\x18\x02 \x01(\t\x12\x18\n\x10ref_node_package\x18\x03 \x01(\t\x12\x18\n\x10ref_node_version\x18\x04 \x01(\t\x12\x17\n\x0fref_max_version\x18\x05 \x01(\t\"\x88\x01\n!UnpinnedRefNewVersionAvailableMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12\x39\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32+.proto_types.UnpinnedRefNewVersionAvailable\"\xc6\x01\n\x1cUpcomingReferenceDeprecation\x12\x12\n\nmodel_name\x18\x01 \x01(\t\x12\x19\n\x11ref_model_package\x18\x02 \x01(\t\x12\x16\n\x0eref_model_name\x18\x03 \x01(\t\x12\x19\n\x11ref_model_version\x18\x04 \x01(\t\x12 \n\x18ref_model_latest_version\x18\x05 \x01(\t\x12\"\n\x1aref_model_deprecation_date\x18\x06 \x01(\t\"\x84\x01\n\x1fUpcomingReferenceDeprecationMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12\x37\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32).proto_types.UpcomingReferenceDeprecation\"\xbd\x01\n\x13\x44\x65precatedReference\x12\x12\n\nmodel_name\x18\x01 \x01(\t\x12\x19\n\x11ref_model_package\x18\x02 \x01(\t\x12\x16\n\x0eref_model_name\x18\x03 \x01(\t\x12\x19\n\x11ref_model_version\x18\x04 \x01(\t\x12 \n\x18ref_model_latest_version\x18\x05 \x01(\t\x12\"\n\x1aref_model_deprecation_date\x18\x06 \x01(\t\"r\n\x16\x44\x65precatedReferenceMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12.\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32 .proto_types.DeprecatedReference\"<\n$UnsupportedConstraintMaterialization\x12\x14\n\x0cmaterialized\x18\x01 \x01(\t\"\x94\x01\n\'UnsupportedConstraintMaterializationMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12?\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x31.proto_types.UnsupportedConstraintMaterialization\"M\n\x14ParseInlineNodeError\x12(\n\tnode_info\x18\x01 \x01(\x0b\x32\x15.proto_types.NodeInfo\x12\x0b\n\x03\x65xc\x18\x02 \x01(\t\"t\n\x17ParseInlineNodeErrorMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12/\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32!.proto_types.ParseInlineNodeError\"(\n\x19SemanticValidationFailure\x12\x0b\n\x03msg\x18\x02 \x01(\t\"~\n\x1cSemanticValidationFailureMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12\x34\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32&.proto_types.SemanticValidationFailure\"\x8a\x03\n\x19UnversionedBreakingChange\x12\x18\n\x10\x62reaking_changes\x18\x01 \x03(\t\x12\x12\n\nmodel_name\x18\x02 \x01(\t\x12\x17\n\x0fmodel_file_path\x18\x03 \x01(\t\x12\"\n\x1a\x63ontract_enforced_disabled\x18\x04 \x01(\x08\x12\x17\n\x0f\x63olumns_removed\x18\x05 \x03(\t\x12\x34\n\x13\x63olumn_type_changes\x18\x06 \x03(\x0b\x32\x17.proto_types.ColumnType\x12I\n\"enforced_column_constraint_removed\x18\x07 \x03(\x0b\x32\x1d.proto_types.ColumnConstraint\x12G\n!enforced_model_constraint_removed\x18\x08 \x03(\x0b\x32\x1c.proto_types.ModelConstraint\x12\x1f\n\x17materialization_changed\x18\t \x03(\t\"~\n\x1cUnversionedBreakingChangeMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12\x34\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32&.proto_types.UnversionedBreakingChange\"*\n\x14WarnStateTargetEqual\x12\x12\n\nstate_path\x18\x01 \x01(\t\"t\n\x17WarnStateTargetEqualMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12/\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32!.proto_types.WarnStateTargetEqual\"%\n\x16\x46reshnessConfigProblem\x12\x0b\n\x03msg\x18\x01 \x01(\t\"x\n\x19\x46reshnessConfigProblemMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12\x31\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32#.proto_types.FreshnessConfigProblem\"/\n\x1dGitSparseCheckoutSubdirectory\x12\x0e\n\x06subdir\x18\x01 \x01(\t\"\x86\x01\n GitSparseCheckoutSubdirectoryMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12\x38\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32*.proto_types.GitSparseCheckoutSubdirectory\"/\n\x1bGitProgressCheckoutRevision\x12\x10\n\x08revision\x18\x01 \x01(\t\"\x82\x01\n\x1eGitProgressCheckoutRevisionMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12\x36\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32(.proto_types.GitProgressCheckoutRevision\"4\n%GitProgressUpdatingExistingDependency\x12\x0b\n\x03\x64ir\x18\x01 \x01(\t\"\x96\x01\n(GitProgressUpdatingExistingDependencyMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12@\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x32.proto_types.GitProgressUpdatingExistingDependency\".\n\x1fGitProgressPullingNewDependency\x12\x0b\n\x03\x64ir\x18\x01 \x01(\t\"\x8a\x01\n\"GitProgressPullingNewDependencyMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12:\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32,.proto_types.GitProgressPullingNewDependency\"\x1d\n\x0eGitNothingToDo\x12\x0b\n\x03sha\x18\x01 \x01(\t\"h\n\x11GitNothingToDoMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12)\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1b.proto_types.GitNothingToDo\"E\n\x1fGitProgressUpdatedCheckoutRange\x12\x11\n\tstart_sha\x18\x01 \x01(\t\x12\x0f\n\x07\x65nd_sha\x18\x02 \x01(\t\"\x8a\x01\n\"GitProgressUpdatedCheckoutRangeMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12:\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32,.proto_types.GitProgressUpdatedCheckoutRange\"*\n\x17GitProgressCheckedOutAt\x12\x0f\n\x07\x65nd_sha\x18\x01 \x01(\t\"z\n\x1aGitProgressCheckedOutAtMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12\x32\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32$.proto_types.GitProgressCheckedOutAt\")\n\x1aRegistryProgressGETRequest\x12\x0b\n\x03url\x18\x01 \x01(\t\"\x80\x01\n\x1dRegistryProgressGETRequestMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12\x35\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\'.proto_types.RegistryProgressGETRequest\"=\n\x1bRegistryProgressGETResponse\x12\x0b\n\x03url\x18\x01 \x01(\t\x12\x11\n\tresp_code\x18\x02 \x01(\x05\"\x82\x01\n\x1eRegistryProgressGETResponseMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12\x36\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32(.proto_types.RegistryProgressGETResponse\"_\n\x1dSelectorReportInvalidSelector\x12\x17\n\x0fvalid_selectors\x18\x01 \x01(\t\x12\x13\n\x0bspec_method\x18\x02 \x01(\t\x12\x10\n\x08raw_spec\x18\x03 \x01(\t\"\x86\x01\n SelectorReportInvalidSelectorMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12\x38\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32*.proto_types.SelectorReportInvalidSelector\"\x15\n\x13\x44\x65psNoPackagesFound\"r\n\x16\x44\x65psNoPackagesFoundMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12.\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32 .proto_types.DepsNoPackagesFound\"/\n\x17\x44\x65psStartPackageInstall\x12\x14\n\x0cpackage_name\x18\x01 \x01(\t\"z\n\x1a\x44\x65psStartPackageInstallMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12\x32\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32$.proto_types.DepsStartPackageInstall\"\'\n\x0f\x44\x65psInstallInfo\x12\x14\n\x0cversion_name\x18\x01 \x01(\t\"j\n\x12\x44\x65psInstallInfoMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12*\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1c.proto_types.DepsInstallInfo\"-\n\x13\x44\x65psUpdateAvailable\x12\x16\n\x0eversion_latest\x18\x01 \x01(\t\"r\n\x16\x44\x65psUpdateAvailableMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12.\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32 .proto_types.DepsUpdateAvailable\"\x0e\n\x0c\x44\x65psUpToDate\"d\n\x0f\x44\x65psUpToDateMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12\'\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x19.proto_types.DepsUpToDate\",\n\x14\x44\x65psListSubdirectory\x12\x14\n\x0csubdirectory\x18\x01 \x01(\t\"t\n\x17\x44\x65psListSubdirectoryMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12/\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32!.proto_types.DepsListSubdirectory\".\n\x1a\x44\x65psNotifyUpdatesAvailable\x12\x10\n\x08packages\x18\x01 \x03(\t\"\x80\x01\n\x1d\x44\x65psNotifyUpdatesAvailableMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12\x35\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\'.proto_types.DepsNotifyUpdatesAvailable\".\n\x1fRegistryIndexProgressGETRequest\x12\x0b\n\x03url\x18\x01 \x01(\t\"\x8a\x01\n\"RegistryIndexProgressGETRequestMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12:\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32,.proto_types.RegistryIndexProgressGETRequest\"B\n RegistryIndexProgressGETResponse\x12\x0b\n\x03url\x18\x01 \x01(\t\x12\x11\n\tresp_code\x18\x02 \x01(\x05\"\x8c\x01\n#RegistryIndexProgressGETResponseMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12;\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32-.proto_types.RegistryIndexProgressGETResponse\"2\n\x1eRegistryResponseUnexpectedType\x12\x10\n\x08response\x18\x01 \x01(\t\"\x88\x01\n!RegistryResponseUnexpectedTypeMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12\x39\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32+.proto_types.RegistryResponseUnexpectedType\"2\n\x1eRegistryResponseMissingTopKeys\x12\x10\n\x08response\x18\x01 \x01(\t\"\x88\x01\n!RegistryResponseMissingTopKeysMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12\x39\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32+.proto_types.RegistryResponseMissingTopKeys\"5\n!RegistryResponseMissingNestedKeys\x12\x10\n\x08response\x18\x01 \x01(\t\"\x8e\x01\n$RegistryResponseMissingNestedKeysMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12<\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32..proto_types.RegistryResponseMissingNestedKeys\"3\n\x1fRegistryResponseExtraNestedKeys\x12\x10\n\x08response\x18\x01 \x01(\t\"\x8a\x01\n\"RegistryResponseExtraNestedKeysMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12:\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32,.proto_types.RegistryResponseExtraNestedKeys\"(\n\x18\x44\x65psSetDownloadDirectory\x12\x0c\n\x04path\x18\x01 \x01(\t\"|\n\x1b\x44\x65psSetDownloadDirectoryMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12\x33\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32%.proto_types.DepsSetDownloadDirectory\"-\n\x0c\x44\x65psUnpinned\x12\x10\n\x08revision\x18\x01 \x01(\t\x12\x0b\n\x03git\x18\x02 \x01(\t\"d\n\x0f\x44\x65psUnpinnedMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12\'\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x19.proto_types.DepsUnpinned\"/\n\x1bNoNodesForSelectionCriteria\x12\x10\n\x08spec_raw\x18\x01 \x01(\t\"\x82\x01\n\x1eNoNodesForSelectionCriteriaMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12\x36\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32(.proto_types.NoNodesForSelectionCriteria\")\n\x10\x44\x65psLockUpdating\x12\x15\n\rlock_filepath\x18\x01 \x01(\t\"l\n\x13\x44\x65psLockUpdatingMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12+\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1d.proto_types.DepsLockUpdating\"R\n\x0e\x44\x65psAddPackage\x12\x14\n\x0cpackage_name\x18\x01 \x01(\t\x12\x0f\n\x07version\x18\x02 \x01(\t\x12\x19\n\x11packages_filepath\x18\x03 \x01(\t\"h\n\x11\x44\x65psAddPackageMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12)\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1b.proto_types.DepsAddPackage\"\xa7\x01\n\x19\x44\x65psFoundDuplicatePackage\x12S\n\x0fremoved_package\x18\x01 \x03(\x0b\x32:.proto_types.DepsFoundDuplicatePackage.RemovedPackageEntry\x1a\x35\n\x13RemovedPackageEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"~\n\x1c\x44\x65psFoundDuplicatePackageMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12\x34\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32&.proto_types.DepsFoundDuplicatePackage\"$\n\x12\x44\x65psVersionMissing\x12\x0e\n\x06source\x18\x01 \x01(\t\"p\n\x15\x44\x65psVersionMissingMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12-\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1f.proto_types.DepsVersionMissing\"/\n\x17\x44\x65psScrubbedPackageName\x12\x14\n\x0cpackage_name\x18\x01 \x01(\t\"z\n\x1a\x44\x65psScrubbedPackageNameMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12\x32\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32$.proto_types.DepsScrubbedPackageName\"*\n\x1bRunningOperationCaughtError\x12\x0b\n\x03\x65xc\x18\x01 \x01(\t\"\x82\x01\n\x1eRunningOperationCaughtErrorMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12\x36\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32(.proto_types.RunningOperationCaughtError\"\x11\n\x0f\x43ompileComplete\"j\n\x12\x43ompileCompleteMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12*\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1c.proto_types.CompileComplete\"\x18\n\x16\x46reshnessCheckComplete\"x\n\x19\x46reshnessCheckCompleteMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12\x31\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32#.proto_types.FreshnessCheckComplete\"\x1c\n\nSeedHeader\x12\x0e\n\x06header\x18\x01 \x01(\t\"`\n\rSeedHeaderMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12%\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x17.proto_types.SeedHeader\"]\n\x12SQLRunnerException\x12\x0b\n\x03\x65xc\x18\x01 \x01(\t\x12\x10\n\x08\x65xc_info\x18\x02 \x01(\t\x12(\n\tnode_info\x18\x03 \x01(\x0b\x32\x15.proto_types.NodeInfo\"p\n\x15SQLRunnerExceptionMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12-\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1f.proto_types.SQLRunnerException\"\xa8\x01\n\rLogTestResult\x12(\n\tnode_info\x18\x01 \x01(\x0b\x32\x15.proto_types.NodeInfo\x12\x0c\n\x04name\x18\x02 \x01(\t\x12\x0e\n\x06status\x18\x03 \x01(\t\x12\r\n\x05index\x18\x04 \x01(\x05\x12\x12\n\nnum_models\x18\x05 \x01(\x05\x12\x16\n\x0e\x65xecution_time\x18\x06 \x01(\x02\x12\x14\n\x0cnum_failures\x18\x07 \x01(\x05\"f\n\x10LogTestResultMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12(\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1a.proto_types.LogTestResult\"k\n\x0cLogStartLine\x12(\n\tnode_info\x18\x01 \x01(\x0b\x32\x15.proto_types.NodeInfo\x12\x13\n\x0b\x64\x65scription\x18\x02 \x01(\t\x12\r\n\x05index\x18\x03 \x01(\x05\x12\r\n\x05total\x18\x04 \x01(\x05\"d\n\x0fLogStartLineMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12\'\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x19.proto_types.LogStartLine\"\x95\x01\n\x0eLogModelResult\x12(\n\tnode_info\x18\x01 \x01(\x0b\x32\x15.proto_types.NodeInfo\x12\x13\n\x0b\x64\x65scription\x18\x02 \x01(\t\x12\x0e\n\x06status\x18\x03 \x01(\t\x12\r\n\x05index\x18\x04 \x01(\x05\x12\r\n\x05total\x18\x05 \x01(\x05\x12\x16\n\x0e\x65xecution_time\x18\x06 \x01(\x02\"h\n\x11LogModelResultMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12)\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1b.proto_types.LogModelResult\"\x92\x02\n\x11LogSnapshotResult\x12(\n\tnode_info\x18\x01 \x01(\x0b\x32\x15.proto_types.NodeInfo\x12\x13\n\x0b\x64\x65scription\x18\x02 \x01(\t\x12\x0e\n\x06status\x18\x03 \x01(\t\x12\r\n\x05index\x18\x04 \x01(\x05\x12\r\n\x05total\x18\x05 \x01(\x05\x12\x16\n\x0e\x65xecution_time\x18\x06 \x01(\x02\x12\x34\n\x03\x63\x66g\x18\x07 \x03(\x0b\x32\'.proto_types.LogSnapshotResult.CfgEntry\x12\x16\n\x0eresult_message\x18\x08 \x01(\t\x1a*\n\x08\x43\x66gEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"n\n\x14LogSnapshotResultMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12,\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1e.proto_types.LogSnapshotResult\"\xb9\x01\n\rLogSeedResult\x12(\n\tnode_info\x18\x01 \x01(\x0b\x32\x15.proto_types.NodeInfo\x12\x0e\n\x06status\x18\x02 \x01(\t\x12\x16\n\x0eresult_message\x18\x03 \x01(\t\x12\r\n\x05index\x18\x04 \x01(\x05\x12\r\n\x05total\x18\x05 \x01(\x05\x12\x16\n\x0e\x65xecution_time\x18\x06 \x01(\x02\x12\x0e\n\x06schema\x18\x07 \x01(\t\x12\x10\n\x08relation\x18\x08 \x01(\t\"f\n\x10LogSeedResultMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12(\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1a.proto_types.LogSeedResult\"\xad\x01\n\x12LogFreshnessResult\x12\x0e\n\x06status\x18\x01 \x01(\t\x12(\n\tnode_info\x18\x02 \x01(\x0b\x32\x15.proto_types.NodeInfo\x12\r\n\x05index\x18\x03 \x01(\x05\x12\r\n\x05total\x18\x04 \x01(\x05\x12\x16\n\x0e\x65xecution_time\x18\x05 \x01(\x02\x12\x13\n\x0bsource_name\x18\x06 \x01(\t\x12\x12\n\ntable_name\x18\x07 \x01(\t\"p\n\x15LogFreshnessResultMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12-\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1f.proto_types.LogFreshnessResult\"\x98\x01\n\x11LogNodeNoOpResult\x12(\n\tnode_info\x18\x01 \x01(\x0b\x32\x15.proto_types.NodeInfo\x12\x13\n\x0b\x64\x65scription\x18\x02 \x01(\t\x12\x0e\n\x06status\x18\x03 \x01(\t\x12\r\n\x05index\x18\x04 \x01(\x05\x12\r\n\x05total\x18\x05 \x01(\x05\x12\x16\n\x0e\x65xecution_time\x18\x06 \x01(\x02\"n\n\x14LogNodeNoOpResultMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12,\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1e.proto_types.LogNodeNoOpResult\"\"\n\rLogCancelLine\x12\x11\n\tconn_name\x18\x01 \x01(\t\"f\n\x10LogCancelLineMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12(\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1a.proto_types.LogCancelLine\"\x1f\n\x0f\x44\x65\x66\x61ultSelector\x12\x0c\n\x04name\x18\x01 \x01(\t\"j\n\x12\x44\x65\x66\x61ultSelectorMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12*\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1c.proto_types.DefaultSelector\"5\n\tNodeStart\x12(\n\tnode_info\x18\x01 \x01(\x0b\x32\x15.proto_types.NodeInfo\"^\n\x0cNodeStartMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12$\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x16.proto_types.NodeStart\"g\n\x0cNodeFinished\x12(\n\tnode_info\x18\x01 \x01(\x0b\x32\x15.proto_types.NodeInfo\x12-\n\nrun_result\x18\x02 \x01(\x0b\x32\x19.proto_types.RunResultMsg\"d\n\x0fNodeFinishedMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12\'\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x19.proto_types.NodeFinished\"+\n\x1bQueryCancelationUnsupported\x12\x0c\n\x04type\x18\x01 \x01(\t\"\x82\x01\n\x1eQueryCancelationUnsupportedMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12\x36\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32(.proto_types.QueryCancelationUnsupported\"O\n\x0f\x43oncurrencyLine\x12\x13\n\x0bnum_threads\x18\x01 \x01(\x05\x12\x13\n\x0btarget_name\x18\x02 \x01(\t\x12\x12\n\nnode_count\x18\x03 \x01(\x05\"j\n\x12\x43oncurrencyLineMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12*\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1c.proto_types.ConcurrencyLine\"E\n\x19WritingInjectedSQLForNode\x12(\n\tnode_info\x18\x01 \x01(\x0b\x32\x15.proto_types.NodeInfo\"~\n\x1cWritingInjectedSQLForNodeMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12\x34\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32&.proto_types.WritingInjectedSQLForNode\"9\n\rNodeCompiling\x12(\n\tnode_info\x18\x01 \x01(\x0b\x32\x15.proto_types.NodeInfo\"f\n\x10NodeCompilingMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12(\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1a.proto_types.NodeCompiling\"9\n\rNodeExecuting\x12(\n\tnode_info\x18\x01 \x01(\x0b\x32\x15.proto_types.NodeInfo\"f\n\x10NodeExecutingMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12(\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1a.proto_types.NodeExecuting\"m\n\x10LogHookStartLine\x12(\n\tnode_info\x18\x01 \x01(\x0b\x32\x15.proto_types.NodeInfo\x12\x11\n\tstatement\x18\x02 \x01(\t\x12\r\n\x05index\x18\x03 \x01(\x05\x12\r\n\x05total\x18\x04 \x01(\x05\"l\n\x13LogHookStartLineMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12+\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1d.proto_types.LogHookStartLine\"\x93\x01\n\x0eLogHookEndLine\x12(\n\tnode_info\x18\x01 \x01(\x0b\x32\x15.proto_types.NodeInfo\x12\x11\n\tstatement\x18\x02 \x01(\t\x12\x0e\n\x06status\x18\x03 \x01(\t\x12\r\n\x05index\x18\x04 \x01(\x05\x12\r\n\x05total\x18\x05 \x01(\x05\x12\x16\n\x0e\x65xecution_time\x18\x06 \x01(\x02\"h\n\x11LogHookEndLineMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12)\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1b.proto_types.LogHookEndLine\"\x93\x01\n\x0fSkippingDetails\x12(\n\tnode_info\x18\x01 \x01(\x0b\x32\x15.proto_types.NodeInfo\x12\x15\n\rresource_type\x18\x02 \x01(\t\x12\x0e\n\x06schema\x18\x03 \x01(\t\x12\x11\n\tnode_name\x18\x04 \x01(\t\x12\r\n\x05index\x18\x05 \x01(\x05\x12\r\n\x05total\x18\x06 \x01(\x05\"j\n\x12SkippingDetailsMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12*\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1c.proto_types.SkippingDetails\"\r\n\x0bNothingToDo\"b\n\x0eNothingToDoMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12&\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x18.proto_types.NothingToDo\",\n\x1dRunningOperationUncaughtError\x12\x0b\n\x03\x65xc\x18\x01 \x01(\t\"\x86\x01\n RunningOperationUncaughtErrorMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12\x38\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32*.proto_types.RunningOperationUncaughtError\"\x93\x01\n\x0c\x45ndRunResult\x12*\n\x07results\x18\x01 \x03(\x0b\x32\x19.proto_types.RunResultMsg\x12\x14\n\x0c\x65lapsed_time\x18\x02 \x01(\x02\x12\x30\n\x0cgenerated_at\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x0f\n\x07success\x18\x04 \x01(\x08\"d\n\x0f\x45ndRunResultMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12\'\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x19.proto_types.EndRunResult\"\x11\n\x0fNoNodesSelected\"j\n\x12NoNodesSelectedMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12*\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1c.proto_types.NoNodesSelected\"w\n\x10\x43ommandCompleted\x12\x0f\n\x07\x63ommand\x18\x01 \x01(\t\x12\x0f\n\x07success\x18\x02 \x01(\x08\x12\x30\n\x0c\x63ompleted_at\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x0f\n\x07\x65lapsed\x18\x04 \x01(\x02\"l\n\x13\x43ommandCompletedMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12+\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1d.proto_types.CommandCompleted\"k\n\x08ShowNode\x12\x11\n\tnode_name\x18\x01 \x01(\t\x12\x0f\n\x07preview\x18\x02 \x01(\t\x12\x11\n\tis_inline\x18\x03 \x01(\x08\x12\x15\n\routput_format\x18\x04 \x01(\t\x12\x11\n\tunique_id\x18\x05 \x01(\t\"\\\n\x0bShowNodeMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12#\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x15.proto_types.ShowNode\"p\n\x0c\x43ompiledNode\x12\x11\n\tnode_name\x18\x01 \x01(\t\x12\x10\n\x08\x63ompiled\x18\x02 \x01(\t\x12\x11\n\tis_inline\x18\x03 \x01(\x08\x12\x15\n\routput_format\x18\x04 \x01(\t\x12\x11\n\tunique_id\x18\x05 \x01(\t\"d\n\x0f\x43ompiledNodeMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12\'\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x19.proto_types.CompiledNode\"b\n\x17\x43\x61tchableExceptionOnRun\x12(\n\tnode_info\x18\x01 \x01(\x0b\x32\x15.proto_types.NodeInfo\x12\x0b\n\x03\x65xc\x18\x02 \x01(\t\x12\x10\n\x08\x65xc_info\x18\x03 \x01(\t\"z\n\x1a\x43\x61tchableExceptionOnRunMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12\x32\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32$.proto_types.CatchableExceptionOnRun\"_\n\x12InternalErrorOnRun\x12\x12\n\nbuild_path\x18\x01 \x01(\t\x12\x0b\n\x03\x65xc\x18\x02 \x01(\t\x12(\n\tnode_info\x18\x03 \x01(\x0b\x32\x15.proto_types.NodeInfo\"p\n\x15InternalErrorOnRunMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12-\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1f.proto_types.InternalErrorOnRun\"u\n\x15GenericExceptionOnRun\x12\x12\n\nbuild_path\x18\x01 \x01(\t\x12\x11\n\tunique_id\x18\x02 \x01(\t\x12\x0b\n\x03\x65xc\x18\x03 \x01(\t\x12(\n\tnode_info\x18\x04 \x01(\x0b\x32\x15.proto_types.NodeInfo\"v\n\x18GenericExceptionOnRunMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12\x30\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\".proto_types.GenericExceptionOnRun\"N\n\x1aNodeConnectionReleaseError\x12\x11\n\tnode_name\x18\x01 \x01(\t\x12\x0b\n\x03\x65xc\x18\x02 \x01(\t\x12\x10\n\x08\x65xc_info\x18\x03 \x01(\t\"\x80\x01\n\x1dNodeConnectionReleaseErrorMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12\x35\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\'.proto_types.NodeConnectionReleaseError\"\x1f\n\nFoundStats\x12\x11\n\tstat_line\x18\x01 \x01(\t\"`\n\rFoundStatsMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12%\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x17.proto_types.FoundStats\"\x17\n\x15MainKeyboardInterrupt\"v\n\x18MainKeyboardInterruptMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12\x30\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\".proto_types.MainKeyboardInterrupt\"#\n\x14MainEncounteredError\x12\x0b\n\x03\x65xc\x18\x01 \x01(\t\"t\n\x17MainEncounteredErrorMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12/\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32!.proto_types.MainEncounteredError\"%\n\x0eMainStackTrace\x12\x13\n\x0bstack_trace\x18\x01 \x01(\t\"h\n\x11MainStackTraceMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12)\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1b.proto_types.MainStackTrace\"p\n\x13TimingInfoCollected\x12(\n\tnode_info\x18\x01 \x01(\x0b\x32\x15.proto_types.NodeInfo\x12/\n\x0btiming_info\x18\x02 \x01(\x0b\x32\x1a.proto_types.TimingInfoMsg\"r\n\x16TimingInfoCollectedMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12.\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32 .proto_types.TimingInfoCollected\"&\n\x12LogDebugStackTrace\x12\x10\n\x08\x65xc_info\x18\x01 \x01(\t\"p\n\x15LogDebugStackTraceMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12-\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1f.proto_types.LogDebugStackTrace\"\x1e\n\x0e\x43heckCleanPath\x12\x0c\n\x04path\x18\x01 \x01(\t\"h\n\x11\x43heckCleanPathMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12)\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1b.proto_types.CheckCleanPath\" \n\x10\x43onfirmCleanPath\x12\x0c\n\x04path\x18\x01 \x01(\t\"l\n\x13\x43onfirmCleanPathMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12+\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1d.proto_types.ConfirmCleanPath\"\"\n\x12ProtectedCleanPath\x12\x0c\n\x04path\x18\x01 \x01(\t\"p\n\x15ProtectedCleanPathMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12-\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1f.proto_types.ProtectedCleanPath\"\x14\n\x12\x46inishedCleanPaths\"p\n\x15\x46inishedCleanPathsMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12-\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1f.proto_types.FinishedCleanPaths\"5\n\x0bOpenCommand\x12\x10\n\x08open_cmd\x18\x01 \x01(\t\x12\x14\n\x0cprofiles_dir\x18\x02 \x01(\t\"b\n\x0eOpenCommandMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12&\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x18.proto_types.OpenCommand\"0\n\x0fServingDocsPort\x12\x0f\n\x07\x61\x64\x64ress\x18\x01 \x01(\t\x12\x0c\n\x04port\x18\x02 \x01(\x05\"j\n\x12ServingDocsPortMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12*\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1c.proto_types.ServingDocsPort\"%\n\x15ServingDocsAccessInfo\x12\x0c\n\x04port\x18\x01 \x01(\t\"v\n\x18ServingDocsAccessInfoMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12\x30\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\".proto_types.ServingDocsAccessInfo\"\x15\n\x13ServingDocsExitInfo\"r\n\x16ServingDocsExitInfoMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12.\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32 .proto_types.ServingDocsExitInfo\"J\n\x10RunResultWarning\x12\x15\n\rresource_type\x18\x01 \x01(\t\x12\x11\n\tnode_name\x18\x02 \x01(\t\x12\x0c\n\x04path\x18\x03 \x01(\t\"l\n\x13RunResultWarningMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12+\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1d.proto_types.RunResultWarning\"J\n\x10RunResultFailure\x12\x15\n\rresource_type\x18\x01 \x01(\t\x12\x11\n\tnode_name\x18\x02 \x01(\t\x12\x0c\n\x04path\x18\x03 \x01(\t\"l\n\x13RunResultFailureMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12+\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1d.proto_types.RunResultFailure\"k\n\tStatsLine\x12\x30\n\x05stats\x18\x01 \x03(\x0b\x32!.proto_types.StatsLine.StatsEntry\x1a,\n\nStatsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\x05:\x02\x38\x01\"^\n\x0cStatsLineMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12$\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x16.proto_types.StatsLine\"\x1d\n\x0eRunResultError\x12\x0b\n\x03msg\x18\x01 \x01(\t\"h\n\x11RunResultErrorMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12)\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1b.proto_types.RunResultError\")\n\x17RunResultErrorNoMessage\x12\x0e\n\x06status\x18\x01 \x01(\t\"z\n\x1aRunResultErrorNoMessageMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12\x32\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32$.proto_types.RunResultErrorNoMessage\"\x1f\n\x0fSQLCompiledPath\x12\x0c\n\x04path\x18\x01 \x01(\t\"j\n\x12SQLCompiledPathMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12*\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1c.proto_types.SQLCompiledPath\"-\n\x14\x43heckNodeTestFailure\x12\x15\n\rrelation_name\x18\x01 \x01(\t\"t\n\x17\x43heckNodeTestFailureMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12/\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32!.proto_types.CheckNodeTestFailure\"W\n\x0f\x45ndOfRunSummary\x12\x12\n\nnum_errors\x18\x01 \x01(\x05\x12\x14\n\x0cnum_warnings\x18\x02 \x01(\x05\x12\x1a\n\x12keyboard_interrupt\x18\x03 \x01(\x08\"j\n\x12\x45ndOfRunSummaryMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12*\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1c.proto_types.EndOfRunSummary\"U\n\x13LogSkipBecauseError\x12\x0e\n\x06schema\x18\x01 \x01(\t\x12\x10\n\x08relation\x18\x02 \x01(\t\x12\r\n\x05index\x18\x03 \x01(\x05\x12\r\n\x05total\x18\x04 \x01(\x05\"r\n\x16LogSkipBecauseErrorMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12.\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32 .proto_types.LogSkipBecauseError\"\x14\n\x12\x45nsureGitInstalled\"p\n\x15\x45nsureGitInstalledMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12-\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1f.proto_types.EnsureGitInstalled\"\x1a\n\x18\x44\x65psCreatingLocalSymlink\"|\n\x1b\x44\x65psCreatingLocalSymlinkMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12\x33\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32%.proto_types.DepsCreatingLocalSymlink\"\x19\n\x17\x44\x65psSymlinkNotAvailable\"z\n\x1a\x44\x65psSymlinkNotAvailableMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12\x32\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32$.proto_types.DepsSymlinkNotAvailable\"\x11\n\x0f\x44isableTracking\"j\n\x12\x44isableTrackingMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12*\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1c.proto_types.DisableTracking\"\x1e\n\x0cSendingEvent\x12\x0e\n\x06kwargs\x18\x01 \x01(\t\"d\n\x0fSendingEventMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12\'\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x19.proto_types.SendingEvent\"\x12\n\x10SendEventFailure\"l\n\x13SendEventFailureMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12+\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1d.proto_types.SendEventFailure\"\r\n\x0b\x46lushEvents\"b\n\x0e\x46lushEventsMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12&\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x18.proto_types.FlushEvents\"\x14\n\x12\x46lushEventsFailure\"p\n\x15\x46lushEventsFailureMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12-\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1f.proto_types.FlushEventsFailure\"-\n\x19TrackingInitializeFailure\x12\x10\n\x08\x65xc_info\x18\x01 \x01(\t\"~\n\x1cTrackingInitializeFailureMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12\x34\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32&.proto_types.TrackingInitializeFailure\"&\n\x17RunResultWarningMessage\x12\x0b\n\x03msg\x18\x01 \x01(\t\"z\n\x1aRunResultWarningMessageMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12\x32\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32$.proto_types.RunResultWarningMessage\"\x1a\n\x0b\x44\x65\x62ugCmdOut\x12\x0b\n\x03msg\x18\x01 \x01(\t\"b\n\x0e\x44\x65\x62ugCmdOutMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12&\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x18.proto_types.DebugCmdOut\"\x1d\n\x0e\x44\x65\x62ugCmdResult\x12\x0b\n\x03msg\x18\x01 \x01(\t\"h\n\x11\x44\x65\x62ugCmdResultMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12)\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1b.proto_types.DebugCmdResult\"\x19\n\nListCmdOut\x12\x0b\n\x03msg\x18\x01 \x01(\t\"`\n\rListCmdOutMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12%\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x17.proto_types.ListCmdOut\"\xec\x01\n\x0eResourceReport\x12\x14\n\x0c\x63ommand_name\x18\x02 \x01(\t\x12\x17\n\x0f\x63ommand_success\x18\x03 \x01(\x08\x12\x1f\n\x17\x63ommand_wall_clock_time\x18\x04 \x01(\x02\x12\x19\n\x11process_user_time\x18\x05 \x01(\x02\x12\x1b\n\x13process_kernel_time\x18\x06 \x01(\x02\x12\x1b\n\x13process_mem_max_rss\x18\x07 \x01(\x03\x12\x19\n\x11process_in_blocks\x18\x08 \x01(\x03\x12\x1a\n\x12process_out_blocks\x18\t \x01(\x03\"h\n\x11ResourceReportMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12)\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1b.proto_types.ResourceReportb\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x10\x63ore_types.proto\x12\x0bproto_types\x1a\x1fgoogle/protobuf/timestamp.proto\x1a\x1cgoogle/protobuf/struct.proto\"\x99\x02\n\rCoreEventInfo\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x0c\n\x04\x63ode\x18\x02 \x01(\t\x12\x0b\n\x03msg\x18\x03 \x01(\t\x12\r\n\x05level\x18\x04 \x01(\t\x12\x15\n\rinvocation_id\x18\x05 \x01(\t\x12\x0b\n\x03pid\x18\x06 \x01(\x05\x12\x0e\n\x06thread\x18\x07 \x01(\t\x12&\n\x02ts\x18\x08 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x34\n\x05\x65xtra\x18\t \x03(\x0b\x32%.proto_types.CoreEventInfo.ExtraEntry\x12\x10\n\x08\x63\x61tegory\x18\n \x01(\t\x1a,\n\nExtraEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"V\n\x0cNodeRelation\x12\x10\n\x08\x64\x61tabase\x18\n \x01(\t\x12\x0e\n\x06schema\x18\x0b \x01(\t\x12\r\n\x05\x61lias\x18\x0c \x01(\t\x12\x15\n\rrelation_name\x18\r \x01(\t\"\x91\x02\n\x08NodeInfo\x12\x11\n\tnode_path\x18\x01 \x01(\t\x12\x11\n\tnode_name\x18\x02 \x01(\t\x12\x11\n\tunique_id\x18\x03 \x01(\t\x12\x15\n\rresource_type\x18\x04 \x01(\t\x12\x14\n\x0cmaterialized\x18\x05 \x01(\t\x12\x13\n\x0bnode_status\x18\x06 \x01(\t\x12\x17\n\x0fnode_started_at\x18\x07 \x01(\t\x12\x18\n\x10node_finished_at\x18\x08 \x01(\t\x12%\n\x04meta\x18\t \x01(\x0b\x32\x17.google.protobuf.Struct\x12\x30\n\rnode_relation\x18\n \x01(\x0b\x32\x19.proto_types.NodeRelation\"\x7f\n\rTimingInfoMsg\x12\x0c\n\x04name\x18\x01 \x01(\t\x12.\n\nstarted_at\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x30\n\x0c\x63ompleted_at\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\"\xd1\x01\n\x0cRunResultMsg\x12\x0e\n\x06status\x18\x01 \x01(\t\x12\x0f\n\x07message\x18\x02 \x01(\t\x12/\n\x0btiming_info\x18\x03 \x03(\x0b\x32\x1a.proto_types.TimingInfoMsg\x12\x0e\n\x06thread\x18\x04 \x01(\t\x12\x16\n\x0e\x65xecution_time\x18\x05 \x01(\x02\x12\x31\n\x10\x61\x64\x61pter_response\x18\x06 \x01(\x0b\x32\x17.google.protobuf.Struct\x12\x14\n\x0cnum_failures\x18\x07 \x01(\x05\"\\\n\nColumnType\x12\x13\n\x0b\x63olumn_name\x18\x01 \x01(\t\x12\x1c\n\x14previous_column_type\x18\x02 \x01(\t\x12\x1b\n\x13\x63urrent_column_type\x18\x03 \x01(\t\"Y\n\x10\x43olumnConstraint\x12\x13\n\x0b\x63olumn_name\x18\x01 \x01(\t\x12\x17\n\x0f\x63onstraint_name\x18\x02 \x01(\t\x12\x17\n\x0f\x63onstraint_type\x18\x03 \x01(\t\"T\n\x0fModelConstraint\x12\x17\n\x0f\x63onstraint_name\x18\x01 \x01(\t\x12\x17\n\x0f\x63onstraint_type\x18\x02 \x01(\t\x12\x0f\n\x07\x63olumns\x18\x03 \x03(\t\"9\n\x11MainReportVersion\x12\x0f\n\x07version\x18\x01 \x01(\t\x12\x13\n\x0blog_version\x18\x02 \x01(\x05\"n\n\x14MainReportVersionMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12,\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1e.proto_types.MainReportVersion\"r\n\x0eMainReportArgs\x12\x33\n\x04\x61rgs\x18\x01 \x03(\x0b\x32%.proto_types.MainReportArgs.ArgsEntry\x1a+\n\tArgsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"h\n\x11MainReportArgsMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12)\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1b.proto_types.MainReportArgs\"+\n\x15MainTrackingUserState\x12\x12\n\nuser_state\x18\x01 \x01(\t\"v\n\x18MainTrackingUserStateMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12\x30\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\".proto_types.MainTrackingUserState\"5\n\x0fMergedFromState\x12\x12\n\nnum_merged\x18\x01 \x01(\x05\x12\x0e\n\x06sample\x18\x02 \x03(\t\"j\n\x12MergedFromStateMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12*\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1c.proto_types.MergedFromState\"A\n\x14MissingProfileTarget\x12\x14\n\x0cprofile_name\x18\x01 \x01(\t\x12\x13\n\x0btarget_name\x18\x02 \x01(\t\"t\n\x17MissingProfileTargetMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12/\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32!.proto_types.MissingProfileTarget\"(\n\x11InvalidOptionYAML\x12\x13\n\x0boption_name\x18\x01 \x01(\t\"n\n\x14InvalidOptionYAMLMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12,\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1e.proto_types.InvalidOptionYAML\"!\n\x12LogDbtProjectError\x12\x0b\n\x03\x65xc\x18\x01 \x01(\t\"p\n\x15LogDbtProjectErrorMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12-\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1f.proto_types.LogDbtProjectError\"3\n\x12LogDbtProfileError\x12\x0b\n\x03\x65xc\x18\x01 \x01(\t\x12\x10\n\x08profiles\x18\x02 \x03(\t\"p\n\x15LogDbtProfileErrorMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12-\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1f.proto_types.LogDbtProfileError\"!\n\x12StarterProjectPath\x12\x0b\n\x03\x64ir\x18\x01 \x01(\t\"p\n\x15StarterProjectPathMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12-\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1f.proto_types.StarterProjectPath\"$\n\x15\x43onfigFolderDirectory\x12\x0b\n\x03\x64ir\x18\x01 \x01(\t\"v\n\x18\x43onfigFolderDirectoryMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12\x30\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\".proto_types.ConfigFolderDirectory\"\'\n\x14NoSampleProfileFound\x12\x0f\n\x07\x61\x64\x61pter\x18\x01 \x01(\t\"t\n\x17NoSampleProfileFoundMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12/\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32!.proto_types.NoSampleProfileFound\"6\n\x18ProfileWrittenWithSample\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x0c\n\x04path\x18\x02 \x01(\t\"|\n\x1bProfileWrittenWithSampleMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12\x33\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32%.proto_types.ProfileWrittenWithSample\"B\n$ProfileWrittenWithTargetTemplateYAML\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x0c\n\x04path\x18\x02 \x01(\t\"\x94\x01\n\'ProfileWrittenWithTargetTemplateYAMLMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12?\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x31.proto_types.ProfileWrittenWithTargetTemplateYAML\"C\n%ProfileWrittenWithProjectTemplateYAML\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x0c\n\x04path\x18\x02 \x01(\t\"\x96\x01\n(ProfileWrittenWithProjectTemplateYAMLMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12@\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x32.proto_types.ProfileWrittenWithProjectTemplateYAML\"\x12\n\x10SettingUpProfile\"l\n\x13SettingUpProfileMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12+\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1d.proto_types.SettingUpProfile\"\x1c\n\x1aInvalidProfileTemplateYAML\"\x80\x01\n\x1dInvalidProfileTemplateYAMLMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12\x35\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\'.proto_types.InvalidProfileTemplateYAML\"(\n\x18ProjectNameAlreadyExists\x12\x0c\n\x04name\x18\x01 \x01(\t\"|\n\x1bProjectNameAlreadyExistsMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12\x33\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32%.proto_types.ProjectNameAlreadyExists\"K\n\x0eProjectCreated\x12\x14\n\x0cproject_name\x18\x01 \x01(\t\x12\x10\n\x08\x64ocs_url\x18\x02 \x01(\t\x12\x11\n\tslack_url\x18\x03 \x01(\t\"h\n\x11ProjectCreatedMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12)\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1b.proto_types.ProjectCreated\"@\n\x1aPackageRedirectDeprecation\x12\x10\n\x08old_name\x18\x01 \x01(\t\x12\x10\n\x08new_name\x18\x02 \x01(\t\"\x80\x01\n\x1dPackageRedirectDeprecationMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12\x35\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\'.proto_types.PackageRedirectDeprecation\"\x1f\n\x1dPackageInstallPathDeprecation\"\x86\x01\n PackageInstallPathDeprecationMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12\x38\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32*.proto_types.PackageInstallPathDeprecation\"H\n\x1b\x43onfigSourcePathDeprecation\x12\x17\n\x0f\x64\x65precated_path\x18\x01 \x01(\t\x12\x10\n\x08\x65xp_path\x18\x02 \x01(\t\"\x82\x01\n\x1e\x43onfigSourcePathDeprecationMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12\x36\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32(.proto_types.ConfigSourcePathDeprecation\"F\n\x19\x43onfigDataPathDeprecation\x12\x17\n\x0f\x64\x65precated_path\x18\x01 \x01(\t\x12\x10\n\x08\x65xp_path\x18\x02 \x01(\t\"~\n\x1c\x43onfigDataPathDeprecationMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12\x34\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32&.proto_types.ConfigDataPathDeprecation\".\n\x17MetricAttributesRenamed\x12\x13\n\x0bmetric_name\x18\x01 \x01(\t\"z\n\x1aMetricAttributesRenamedMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12\x32\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32$.proto_types.MetricAttributesRenamed\"+\n\x17\x45xposureNameDeprecation\x12\x10\n\x08\x65xposure\x18\x01 \x01(\t\"z\n\x1a\x45xposureNameDeprecationMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12\x32\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32$.proto_types.ExposureNameDeprecation\"^\n\x13InternalDeprecation\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x0e\n\x06reason\x18\x02 \x01(\t\x12\x18\n\x10suggested_action\x18\x03 \x01(\t\x12\x0f\n\x07version\x18\x04 \x01(\t\"r\n\x16InternalDeprecationMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12.\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32 .proto_types.InternalDeprecation\"@\n\x1a\x45nvironmentVariableRenamed\x12\x10\n\x08old_name\x18\x01 \x01(\t\x12\x10\n\x08new_name\x18\x02 \x01(\t\"\x80\x01\n\x1d\x45nvironmentVariableRenamedMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12\x35\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\'.proto_types.EnvironmentVariableRenamed\"3\n\x18\x43onfigLogPathDeprecation\x12\x17\n\x0f\x64\x65precated_path\x18\x01 \x01(\t\"|\n\x1b\x43onfigLogPathDeprecationMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12\x33\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32%.proto_types.ConfigLogPathDeprecation\"6\n\x1b\x43onfigTargetPathDeprecation\x12\x17\n\x0f\x64\x65precated_path\x18\x01 \x01(\t\"\x82\x01\n\x1e\x43onfigTargetPathDeprecationMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12\x36\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32(.proto_types.ConfigTargetPathDeprecation\"C\n\x16TestsConfigDeprecation\x12\x17\n\x0f\x64\x65precated_path\x18\x01 \x01(\t\x12\x10\n\x08\x65xp_path\x18\x02 \x01(\t\"x\n\x19TestsConfigDeprecationMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12\x31\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32#.proto_types.TestsConfigDeprecation\"\x1e\n\x1cProjectFlagsMovedDeprecation\"\x84\x01\n\x1fProjectFlagsMovedDeprecationMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12\x37\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32).proto_types.ProjectFlagsMovedDeprecation\"V\n\x0f\x44\x65precatedModel\x12\x12\n\nmodel_name\x18\x01 \x01(\t\x12\x15\n\rmodel_version\x18\x02 \x01(\t\x12\x18\n\x10\x64\x65precation_date\x18\x03 \x01(\t\"j\n\x12\x44\x65precatedModelMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12*\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1c.proto_types.DeprecatedModel\"7\n\x12InputFileDiffError\x12\x10\n\x08\x63\x61tegory\x18\x01 \x01(\t\x12\x0f\n\x07\x66ile_id\x18\x02 \x01(\t\"p\n\x15InputFileDiffErrorMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12-\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1f.proto_types.InputFileDiffError\"?\n\x14InvalidValueForField\x12\x12\n\nfield_name\x18\x01 \x01(\t\x12\x13\n\x0b\x66ield_value\x18\x02 \x01(\t\"t\n\x17InvalidValueForFieldMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12/\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32!.proto_types.InvalidValueForField\"Q\n\x11ValidationWarning\x12\x15\n\rresource_type\x18\x01 \x01(\t\x12\x12\n\nfield_name\x18\x02 \x01(\t\x12\x11\n\tnode_name\x18\x03 \x01(\t\"n\n\x14ValidationWarningMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12,\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1e.proto_types.ValidationWarning\"!\n\x11ParsePerfInfoPath\x12\x0c\n\x04path\x18\x01 \x01(\t\"n\n\x14ParsePerfInfoPathMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12,\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1e.proto_types.ParsePerfInfoPath\"1\n!PartialParsingErrorProcessingFile\x12\x0c\n\x04\x66ile\x18\x01 \x01(\t\"\x8e\x01\n$PartialParsingErrorProcessingFileMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12<\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32..proto_types.PartialParsingErrorProcessingFile\"\x86\x01\n\x13PartialParsingError\x12?\n\x08\x65xc_info\x18\x01 \x03(\x0b\x32-.proto_types.PartialParsingError.ExcInfoEntry\x1a.\n\x0c\x45xcInfoEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"r\n\x16PartialParsingErrorMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12.\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32 .proto_types.PartialParsingError\"\x1b\n\x19PartialParsingSkipParsing\"~\n\x1cPartialParsingSkipParsingMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12\x34\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32&.proto_types.PartialParsingSkipParsing\"&\n\x14UnableToPartialParse\x12\x0e\n\x06reason\x18\x01 \x01(\t\"t\n\x17UnableToPartialParseMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12/\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32!.proto_types.UnableToPartialParse\"f\n\x12StateCheckVarsHash\x12\x10\n\x08\x63hecksum\x18\x01 \x01(\t\x12\x0c\n\x04vars\x18\x02 \x01(\t\x12\x0f\n\x07profile\x18\x03 \x01(\t\x12\x0e\n\x06target\x18\x04 \x01(\t\x12\x0f\n\x07version\x18\x05 \x01(\t\"p\n\x15StateCheckVarsHashMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12-\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1f.proto_types.StateCheckVarsHash\"\x1a\n\x18PartialParsingNotEnabled\"|\n\x1bPartialParsingNotEnabledMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12\x33\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32%.proto_types.PartialParsingNotEnabled\"C\n\x14ParsedFileLoadFailed\x12\x0c\n\x04path\x18\x01 \x01(\t\x12\x0b\n\x03\x65xc\x18\x02 \x01(\t\x12\x10\n\x08\x65xc_info\x18\x03 \x01(\t\"t\n\x17ParsedFileLoadFailedMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12/\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32!.proto_types.ParsedFileLoadFailed\"H\n\x15PartialParsingEnabled\x12\x0f\n\x07\x64\x65leted\x18\x01 \x01(\x05\x12\r\n\x05\x61\x64\x64\x65\x64\x18\x02 \x01(\x05\x12\x0f\n\x07\x63hanged\x18\x03 \x01(\x05\"v\n\x18PartialParsingEnabledMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12\x30\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\".proto_types.PartialParsingEnabled\"8\n\x12PartialParsingFile\x12\x0f\n\x07\x66ile_id\x18\x01 \x01(\t\x12\x11\n\toperation\x18\x02 \x01(\t\"p\n\x15PartialParsingFileMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12-\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1f.proto_types.PartialParsingFile\"\xaf\x01\n\x1fInvalidDisabledTargetInTestNode\x12\x1b\n\x13resource_type_title\x18\x01 \x01(\t\x12\x11\n\tunique_id\x18\x02 \x01(\t\x12\x1a\n\x12original_file_path\x18\x03 \x01(\t\x12\x13\n\x0btarget_kind\x18\x04 \x01(\t\x12\x13\n\x0btarget_name\x18\x05 \x01(\t\x12\x16\n\x0etarget_package\x18\x06 \x01(\t\"\x8a\x01\n\"InvalidDisabledTargetInTestNodeMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12:\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32,.proto_types.InvalidDisabledTargetInTestNode\"7\n\x18UnusedResourceConfigPath\x12\x1b\n\x13unused_config_paths\x18\x01 \x03(\t\"|\n\x1bUnusedResourceConfigPathMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12\x33\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32%.proto_types.UnusedResourceConfigPath\"3\n\rSeedIncreased\x12\x14\n\x0cpackage_name\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\"f\n\x10SeedIncreasedMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12(\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1a.proto_types.SeedIncreased\">\n\x18SeedExceedsLimitSamePath\x12\x14\n\x0cpackage_name\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\"|\n\x1bSeedExceedsLimitSamePathMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12\x33\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32%.proto_types.SeedExceedsLimitSamePath\"D\n\x1eSeedExceedsLimitAndPathChanged\x12\x14\n\x0cpackage_name\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\"\x88\x01\n!SeedExceedsLimitAndPathChangedMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12\x39\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32+.proto_types.SeedExceedsLimitAndPathChanged\"\\\n\x1fSeedExceedsLimitChecksumChanged\x12\x14\n\x0cpackage_name\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\x12\x15\n\rchecksum_name\x18\x03 \x01(\t\"\x8a\x01\n\"SeedExceedsLimitChecksumChangedMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12:\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32,.proto_types.SeedExceedsLimitChecksumChanged\"%\n\x0cUnusedTables\x12\x15\n\runused_tables\x18\x01 \x03(\t\"d\n\x0fUnusedTablesMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12\'\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x19.proto_types.UnusedTables\"\x87\x01\n\x17WrongResourceSchemaFile\x12\x12\n\npatch_name\x18\x01 \x01(\t\x12\x15\n\rresource_type\x18\x02 \x01(\t\x12\x1c\n\x14plural_resource_type\x18\x03 \x01(\t\x12\x10\n\x08yaml_key\x18\x04 \x01(\t\x12\x11\n\tfile_path\x18\x05 \x01(\t\"z\n\x1aWrongResourceSchemaFileMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12\x32\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32$.proto_types.WrongResourceSchemaFile\"K\n\x10NoNodeForYamlKey\x12\x12\n\npatch_name\x18\x01 \x01(\t\x12\x10\n\x08yaml_key\x18\x02 \x01(\t\x12\x11\n\tfile_path\x18\x03 \x01(\t\"l\n\x13NoNodeForYamlKeyMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12+\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1d.proto_types.NoNodeForYamlKey\"+\n\x15MacroNotFoundForPatch\x12\x12\n\npatch_name\x18\x01 \x01(\t\"v\n\x18MacroNotFoundForPatchMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12\x30\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\".proto_types.MacroNotFoundForPatch\"\xb8\x01\n\x16NodeNotFoundOrDisabled\x12\x1a\n\x12original_file_path\x18\x01 \x01(\t\x12\x11\n\tunique_id\x18\x02 \x01(\t\x12\x1b\n\x13resource_type_title\x18\x03 \x01(\t\x12\x13\n\x0btarget_name\x18\x04 \x01(\t\x12\x13\n\x0btarget_kind\x18\x05 \x01(\t\x12\x16\n\x0etarget_package\x18\x06 \x01(\t\x12\x10\n\x08\x64isabled\x18\x07 \x01(\t\"x\n\x19NodeNotFoundOrDisabledMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12\x31\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32#.proto_types.NodeNotFoundOrDisabled\"H\n\x0fJinjaLogWarning\x12(\n\tnode_info\x18\x01 \x01(\x0b\x32\x15.proto_types.NodeInfo\x12\x0b\n\x03msg\x18\x02 \x01(\t\"j\n\x12JinjaLogWarningMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12*\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1c.proto_types.JinjaLogWarning\"E\n\x0cJinjaLogInfo\x12(\n\tnode_info\x18\x01 \x01(\x0b\x32\x15.proto_types.NodeInfo\x12\x0b\n\x03msg\x18\x02 \x01(\t\"d\n\x0fJinjaLogInfoMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12\'\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x19.proto_types.JinjaLogInfo\"F\n\rJinjaLogDebug\x12(\n\tnode_info\x18\x01 \x01(\x0b\x32\x15.proto_types.NodeInfo\x12\x0b\n\x03msg\x18\x02 \x01(\t\"f\n\x10JinjaLogDebugMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12(\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1a.proto_types.JinjaLogDebug\"\xae\x01\n\x1eUnpinnedRefNewVersionAvailable\x12(\n\tnode_info\x18\x01 \x01(\x0b\x32\x15.proto_types.NodeInfo\x12\x15\n\rref_node_name\x18\x02 \x01(\t\x12\x18\n\x10ref_node_package\x18\x03 \x01(\t\x12\x18\n\x10ref_node_version\x18\x04 \x01(\t\x12\x17\n\x0fref_max_version\x18\x05 \x01(\t\"\x88\x01\n!UnpinnedRefNewVersionAvailableMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12\x39\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32+.proto_types.UnpinnedRefNewVersionAvailable\"\xc6\x01\n\x1cUpcomingReferenceDeprecation\x12\x12\n\nmodel_name\x18\x01 \x01(\t\x12\x19\n\x11ref_model_package\x18\x02 \x01(\t\x12\x16\n\x0eref_model_name\x18\x03 \x01(\t\x12\x19\n\x11ref_model_version\x18\x04 \x01(\t\x12 \n\x18ref_model_latest_version\x18\x05 \x01(\t\x12\"\n\x1aref_model_deprecation_date\x18\x06 \x01(\t\"\x84\x01\n\x1fUpcomingReferenceDeprecationMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12\x37\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32).proto_types.UpcomingReferenceDeprecation\"\xbd\x01\n\x13\x44\x65precatedReference\x12\x12\n\nmodel_name\x18\x01 \x01(\t\x12\x19\n\x11ref_model_package\x18\x02 \x01(\t\x12\x16\n\x0eref_model_name\x18\x03 \x01(\t\x12\x19\n\x11ref_model_version\x18\x04 \x01(\t\x12 \n\x18ref_model_latest_version\x18\x05 \x01(\t\x12\"\n\x1aref_model_deprecation_date\x18\x06 \x01(\t\"r\n\x16\x44\x65precatedReferenceMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12.\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32 .proto_types.DeprecatedReference\"<\n$UnsupportedConstraintMaterialization\x12\x14\n\x0cmaterialized\x18\x01 \x01(\t\"\x94\x01\n\'UnsupportedConstraintMaterializationMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12?\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x31.proto_types.UnsupportedConstraintMaterialization\"M\n\x14ParseInlineNodeError\x12(\n\tnode_info\x18\x01 \x01(\x0b\x32\x15.proto_types.NodeInfo\x12\x0b\n\x03\x65xc\x18\x02 \x01(\t\"t\n\x17ParseInlineNodeErrorMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12/\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32!.proto_types.ParseInlineNodeError\"(\n\x19SemanticValidationFailure\x12\x0b\n\x03msg\x18\x02 \x01(\t\"~\n\x1cSemanticValidationFailureMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12\x34\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32&.proto_types.SemanticValidationFailure\"\x8a\x03\n\x19UnversionedBreakingChange\x12\x18\n\x10\x62reaking_changes\x18\x01 \x03(\t\x12\x12\n\nmodel_name\x18\x02 \x01(\t\x12\x17\n\x0fmodel_file_path\x18\x03 \x01(\t\x12\"\n\x1a\x63ontract_enforced_disabled\x18\x04 \x01(\x08\x12\x17\n\x0f\x63olumns_removed\x18\x05 \x03(\t\x12\x34\n\x13\x63olumn_type_changes\x18\x06 \x03(\x0b\x32\x17.proto_types.ColumnType\x12I\n\"enforced_column_constraint_removed\x18\x07 \x03(\x0b\x32\x1d.proto_types.ColumnConstraint\x12G\n!enforced_model_constraint_removed\x18\x08 \x03(\x0b\x32\x1c.proto_types.ModelConstraint\x12\x1f\n\x17materialization_changed\x18\t \x03(\t\"~\n\x1cUnversionedBreakingChangeMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12\x34\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32&.proto_types.UnversionedBreakingChange\"*\n\x14WarnStateTargetEqual\x12\x12\n\nstate_path\x18\x01 \x01(\t\"t\n\x17WarnStateTargetEqualMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12/\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32!.proto_types.WarnStateTargetEqual\"%\n\x16\x46reshnessConfigProblem\x12\x0b\n\x03msg\x18\x01 \x01(\t\"x\n\x19\x46reshnessConfigProblemMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12\x31\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32#.proto_types.FreshnessConfigProblem\"/\n\x1dGitSparseCheckoutSubdirectory\x12\x0e\n\x06subdir\x18\x01 \x01(\t\"\x86\x01\n GitSparseCheckoutSubdirectoryMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12\x38\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32*.proto_types.GitSparseCheckoutSubdirectory\"/\n\x1bGitProgressCheckoutRevision\x12\x10\n\x08revision\x18\x01 \x01(\t\"\x82\x01\n\x1eGitProgressCheckoutRevisionMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12\x36\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32(.proto_types.GitProgressCheckoutRevision\"4\n%GitProgressUpdatingExistingDependency\x12\x0b\n\x03\x64ir\x18\x01 \x01(\t\"\x96\x01\n(GitProgressUpdatingExistingDependencyMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12@\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x32.proto_types.GitProgressUpdatingExistingDependency\".\n\x1fGitProgressPullingNewDependency\x12\x0b\n\x03\x64ir\x18\x01 \x01(\t\"\x8a\x01\n\"GitProgressPullingNewDependencyMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12:\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32,.proto_types.GitProgressPullingNewDependency\"\x1d\n\x0eGitNothingToDo\x12\x0b\n\x03sha\x18\x01 \x01(\t\"h\n\x11GitNothingToDoMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12)\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1b.proto_types.GitNothingToDo\"E\n\x1fGitProgressUpdatedCheckoutRange\x12\x11\n\tstart_sha\x18\x01 \x01(\t\x12\x0f\n\x07\x65nd_sha\x18\x02 \x01(\t\"\x8a\x01\n\"GitProgressUpdatedCheckoutRangeMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12:\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32,.proto_types.GitProgressUpdatedCheckoutRange\"*\n\x17GitProgressCheckedOutAt\x12\x0f\n\x07\x65nd_sha\x18\x01 \x01(\t\"z\n\x1aGitProgressCheckedOutAtMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12\x32\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32$.proto_types.GitProgressCheckedOutAt\")\n\x1aRegistryProgressGETRequest\x12\x0b\n\x03url\x18\x01 \x01(\t\"\x80\x01\n\x1dRegistryProgressGETRequestMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12\x35\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\'.proto_types.RegistryProgressGETRequest\"=\n\x1bRegistryProgressGETResponse\x12\x0b\n\x03url\x18\x01 \x01(\t\x12\x11\n\tresp_code\x18\x02 \x01(\x05\"\x82\x01\n\x1eRegistryProgressGETResponseMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12\x36\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32(.proto_types.RegistryProgressGETResponse\"_\n\x1dSelectorReportInvalidSelector\x12\x17\n\x0fvalid_selectors\x18\x01 \x01(\t\x12\x13\n\x0bspec_method\x18\x02 \x01(\t\x12\x10\n\x08raw_spec\x18\x03 \x01(\t\"\x86\x01\n SelectorReportInvalidSelectorMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12\x38\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32*.proto_types.SelectorReportInvalidSelector\"\x15\n\x13\x44\x65psNoPackagesFound\"r\n\x16\x44\x65psNoPackagesFoundMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12.\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32 .proto_types.DepsNoPackagesFound\"/\n\x17\x44\x65psStartPackageInstall\x12\x14\n\x0cpackage_name\x18\x01 \x01(\t\"z\n\x1a\x44\x65psStartPackageInstallMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12\x32\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32$.proto_types.DepsStartPackageInstall\"\'\n\x0f\x44\x65psInstallInfo\x12\x14\n\x0cversion_name\x18\x01 \x01(\t\"j\n\x12\x44\x65psInstallInfoMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12*\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1c.proto_types.DepsInstallInfo\"-\n\x13\x44\x65psUpdateAvailable\x12\x16\n\x0eversion_latest\x18\x01 \x01(\t\"r\n\x16\x44\x65psUpdateAvailableMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12.\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32 .proto_types.DepsUpdateAvailable\"\x0e\n\x0c\x44\x65psUpToDate\"d\n\x0f\x44\x65psUpToDateMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12\'\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x19.proto_types.DepsUpToDate\",\n\x14\x44\x65psListSubdirectory\x12\x14\n\x0csubdirectory\x18\x01 \x01(\t\"t\n\x17\x44\x65psListSubdirectoryMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12/\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32!.proto_types.DepsListSubdirectory\".\n\x1a\x44\x65psNotifyUpdatesAvailable\x12\x10\n\x08packages\x18\x01 \x03(\t\"\x80\x01\n\x1d\x44\x65psNotifyUpdatesAvailableMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12\x35\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\'.proto_types.DepsNotifyUpdatesAvailable\".\n\x1fRegistryIndexProgressGETRequest\x12\x0b\n\x03url\x18\x01 \x01(\t\"\x8a\x01\n\"RegistryIndexProgressGETRequestMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12:\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32,.proto_types.RegistryIndexProgressGETRequest\"B\n RegistryIndexProgressGETResponse\x12\x0b\n\x03url\x18\x01 \x01(\t\x12\x11\n\tresp_code\x18\x02 \x01(\x05\"\x8c\x01\n#RegistryIndexProgressGETResponseMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12;\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32-.proto_types.RegistryIndexProgressGETResponse\"2\n\x1eRegistryResponseUnexpectedType\x12\x10\n\x08response\x18\x01 \x01(\t\"\x88\x01\n!RegistryResponseUnexpectedTypeMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12\x39\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32+.proto_types.RegistryResponseUnexpectedType\"2\n\x1eRegistryResponseMissingTopKeys\x12\x10\n\x08response\x18\x01 \x01(\t\"\x88\x01\n!RegistryResponseMissingTopKeysMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12\x39\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32+.proto_types.RegistryResponseMissingTopKeys\"5\n!RegistryResponseMissingNestedKeys\x12\x10\n\x08response\x18\x01 \x01(\t\"\x8e\x01\n$RegistryResponseMissingNestedKeysMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12<\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32..proto_types.RegistryResponseMissingNestedKeys\"3\n\x1fRegistryResponseExtraNestedKeys\x12\x10\n\x08response\x18\x01 \x01(\t\"\x8a\x01\n\"RegistryResponseExtraNestedKeysMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12:\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32,.proto_types.RegistryResponseExtraNestedKeys\"(\n\x18\x44\x65psSetDownloadDirectory\x12\x0c\n\x04path\x18\x01 \x01(\t\"|\n\x1b\x44\x65psSetDownloadDirectoryMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12\x33\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32%.proto_types.DepsSetDownloadDirectory\"-\n\x0c\x44\x65psUnpinned\x12\x10\n\x08revision\x18\x01 \x01(\t\x12\x0b\n\x03git\x18\x02 \x01(\t\"d\n\x0f\x44\x65psUnpinnedMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12\'\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x19.proto_types.DepsUnpinned\"/\n\x1bNoNodesForSelectionCriteria\x12\x10\n\x08spec_raw\x18\x01 \x01(\t\"\x82\x01\n\x1eNoNodesForSelectionCriteriaMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12\x36\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32(.proto_types.NoNodesForSelectionCriteria\")\n\x10\x44\x65psLockUpdating\x12\x15\n\rlock_filepath\x18\x01 \x01(\t\"l\n\x13\x44\x65psLockUpdatingMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12+\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1d.proto_types.DepsLockUpdating\"R\n\x0e\x44\x65psAddPackage\x12\x14\n\x0cpackage_name\x18\x01 \x01(\t\x12\x0f\n\x07version\x18\x02 \x01(\t\x12\x19\n\x11packages_filepath\x18\x03 \x01(\t\"h\n\x11\x44\x65psAddPackageMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12)\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1b.proto_types.DepsAddPackage\"\xa7\x01\n\x19\x44\x65psFoundDuplicatePackage\x12S\n\x0fremoved_package\x18\x01 \x03(\x0b\x32:.proto_types.DepsFoundDuplicatePackage.RemovedPackageEntry\x1a\x35\n\x13RemovedPackageEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"~\n\x1c\x44\x65psFoundDuplicatePackageMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12\x34\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32&.proto_types.DepsFoundDuplicatePackage\"$\n\x12\x44\x65psVersionMissing\x12\x0e\n\x06source\x18\x01 \x01(\t\"p\n\x15\x44\x65psVersionMissingMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12-\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1f.proto_types.DepsVersionMissing\"/\n\x17\x44\x65psScrubbedPackageName\x12\x14\n\x0cpackage_name\x18\x01 \x01(\t\"z\n\x1a\x44\x65psScrubbedPackageNameMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12\x32\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32$.proto_types.DepsScrubbedPackageName\"*\n\x1bRunningOperationCaughtError\x12\x0b\n\x03\x65xc\x18\x01 \x01(\t\"\x82\x01\n\x1eRunningOperationCaughtErrorMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12\x36\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32(.proto_types.RunningOperationCaughtError\"\x11\n\x0f\x43ompileComplete\"j\n\x12\x43ompileCompleteMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12*\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1c.proto_types.CompileComplete\"\x18\n\x16\x46reshnessCheckComplete\"x\n\x19\x46reshnessCheckCompleteMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12\x31\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32#.proto_types.FreshnessCheckComplete\"\x1c\n\nSeedHeader\x12\x0e\n\x06header\x18\x01 \x01(\t\"`\n\rSeedHeaderMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12%\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x17.proto_types.SeedHeader\"]\n\x12SQLRunnerException\x12\x0b\n\x03\x65xc\x18\x01 \x01(\t\x12\x10\n\x08\x65xc_info\x18\x02 \x01(\t\x12(\n\tnode_info\x18\x03 \x01(\x0b\x32\x15.proto_types.NodeInfo\"p\n\x15SQLRunnerExceptionMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12-\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1f.proto_types.SQLRunnerException\"\xa8\x01\n\rLogTestResult\x12(\n\tnode_info\x18\x01 \x01(\x0b\x32\x15.proto_types.NodeInfo\x12\x0c\n\x04name\x18\x02 \x01(\t\x12\x0e\n\x06status\x18\x03 \x01(\t\x12\r\n\x05index\x18\x04 \x01(\x05\x12\x12\n\nnum_models\x18\x05 \x01(\x05\x12\x16\n\x0e\x65xecution_time\x18\x06 \x01(\x02\x12\x14\n\x0cnum_failures\x18\x07 \x01(\x05\"f\n\x10LogTestResultMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12(\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1a.proto_types.LogTestResult\"k\n\x0cLogStartLine\x12(\n\tnode_info\x18\x01 \x01(\x0b\x32\x15.proto_types.NodeInfo\x12\x13\n\x0b\x64\x65scription\x18\x02 \x01(\t\x12\r\n\x05index\x18\x03 \x01(\x05\x12\r\n\x05total\x18\x04 \x01(\x05\"d\n\x0fLogStartLineMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12\'\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x19.proto_types.LogStartLine\"\x95\x01\n\x0eLogModelResult\x12(\n\tnode_info\x18\x01 \x01(\x0b\x32\x15.proto_types.NodeInfo\x12\x13\n\x0b\x64\x65scription\x18\x02 \x01(\t\x12\x0e\n\x06status\x18\x03 \x01(\t\x12\r\n\x05index\x18\x04 \x01(\x05\x12\r\n\x05total\x18\x05 \x01(\x05\x12\x16\n\x0e\x65xecution_time\x18\x06 \x01(\x02\"h\n\x11LogModelResultMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12)\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1b.proto_types.LogModelResult\"\x92\x02\n\x11LogSnapshotResult\x12(\n\tnode_info\x18\x01 \x01(\x0b\x32\x15.proto_types.NodeInfo\x12\x13\n\x0b\x64\x65scription\x18\x02 \x01(\t\x12\x0e\n\x06status\x18\x03 \x01(\t\x12\r\n\x05index\x18\x04 \x01(\x05\x12\r\n\x05total\x18\x05 \x01(\x05\x12\x16\n\x0e\x65xecution_time\x18\x06 \x01(\x02\x12\x34\n\x03\x63\x66g\x18\x07 \x03(\x0b\x32\'.proto_types.LogSnapshotResult.CfgEntry\x12\x16\n\x0eresult_message\x18\x08 \x01(\t\x1a*\n\x08\x43\x66gEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"n\n\x14LogSnapshotResultMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12,\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1e.proto_types.LogSnapshotResult\"\xb9\x01\n\rLogSeedResult\x12(\n\tnode_info\x18\x01 \x01(\x0b\x32\x15.proto_types.NodeInfo\x12\x0e\n\x06status\x18\x02 \x01(\t\x12\x16\n\x0eresult_message\x18\x03 \x01(\t\x12\r\n\x05index\x18\x04 \x01(\x05\x12\r\n\x05total\x18\x05 \x01(\x05\x12\x16\n\x0e\x65xecution_time\x18\x06 \x01(\x02\x12\x0e\n\x06schema\x18\x07 \x01(\t\x12\x10\n\x08relation\x18\x08 \x01(\t\"f\n\x10LogSeedResultMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12(\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1a.proto_types.LogSeedResult\"\xad\x01\n\x12LogFreshnessResult\x12\x0e\n\x06status\x18\x01 \x01(\t\x12(\n\tnode_info\x18\x02 \x01(\x0b\x32\x15.proto_types.NodeInfo\x12\r\n\x05index\x18\x03 \x01(\x05\x12\r\n\x05total\x18\x04 \x01(\x05\x12\x16\n\x0e\x65xecution_time\x18\x05 \x01(\x02\x12\x13\n\x0bsource_name\x18\x06 \x01(\t\x12\x12\n\ntable_name\x18\x07 \x01(\t\"p\n\x15LogFreshnessResultMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12-\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1f.proto_types.LogFreshnessResult\"\x98\x01\n\x11LogNodeNoOpResult\x12(\n\tnode_info\x18\x01 \x01(\x0b\x32\x15.proto_types.NodeInfo\x12\x13\n\x0b\x64\x65scription\x18\x02 \x01(\t\x12\x0e\n\x06status\x18\x03 \x01(\t\x12\r\n\x05index\x18\x04 \x01(\x05\x12\r\n\x05total\x18\x05 \x01(\x05\x12\x16\n\x0e\x65xecution_time\x18\x06 \x01(\x02\"n\n\x14LogNodeNoOpResultMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12,\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1e.proto_types.LogNodeNoOpResult\"\"\n\rLogCancelLine\x12\x11\n\tconn_name\x18\x01 \x01(\t\"f\n\x10LogCancelLineMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12(\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1a.proto_types.LogCancelLine\"\x1f\n\x0f\x44\x65\x66\x61ultSelector\x12\x0c\n\x04name\x18\x01 \x01(\t\"j\n\x12\x44\x65\x66\x61ultSelectorMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12*\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1c.proto_types.DefaultSelector\"5\n\tNodeStart\x12(\n\tnode_info\x18\x01 \x01(\x0b\x32\x15.proto_types.NodeInfo\"^\n\x0cNodeStartMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12$\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x16.proto_types.NodeStart\"g\n\x0cNodeFinished\x12(\n\tnode_info\x18\x01 \x01(\x0b\x32\x15.proto_types.NodeInfo\x12-\n\nrun_result\x18\x02 \x01(\x0b\x32\x19.proto_types.RunResultMsg\"d\n\x0fNodeFinishedMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12\'\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x19.proto_types.NodeFinished\"+\n\x1bQueryCancelationUnsupported\x12\x0c\n\x04type\x18\x01 \x01(\t\"\x82\x01\n\x1eQueryCancelationUnsupportedMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12\x36\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32(.proto_types.QueryCancelationUnsupported\"O\n\x0f\x43oncurrencyLine\x12\x13\n\x0bnum_threads\x18\x01 \x01(\x05\x12\x13\n\x0btarget_name\x18\x02 \x01(\t\x12\x12\n\nnode_count\x18\x03 \x01(\x05\"j\n\x12\x43oncurrencyLineMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12*\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1c.proto_types.ConcurrencyLine\"E\n\x19WritingInjectedSQLForNode\x12(\n\tnode_info\x18\x01 \x01(\x0b\x32\x15.proto_types.NodeInfo\"~\n\x1cWritingInjectedSQLForNodeMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12\x34\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32&.proto_types.WritingInjectedSQLForNode\"9\n\rNodeCompiling\x12(\n\tnode_info\x18\x01 \x01(\x0b\x32\x15.proto_types.NodeInfo\"f\n\x10NodeCompilingMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12(\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1a.proto_types.NodeCompiling\"9\n\rNodeExecuting\x12(\n\tnode_info\x18\x01 \x01(\x0b\x32\x15.proto_types.NodeInfo\"f\n\x10NodeExecutingMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12(\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1a.proto_types.NodeExecuting\"m\n\x10LogHookStartLine\x12(\n\tnode_info\x18\x01 \x01(\x0b\x32\x15.proto_types.NodeInfo\x12\x11\n\tstatement\x18\x02 \x01(\t\x12\r\n\x05index\x18\x03 \x01(\x05\x12\r\n\x05total\x18\x04 \x01(\x05\"l\n\x13LogHookStartLineMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12+\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1d.proto_types.LogHookStartLine\"\x93\x01\n\x0eLogHookEndLine\x12(\n\tnode_info\x18\x01 \x01(\x0b\x32\x15.proto_types.NodeInfo\x12\x11\n\tstatement\x18\x02 \x01(\t\x12\x0e\n\x06status\x18\x03 \x01(\t\x12\r\n\x05index\x18\x04 \x01(\x05\x12\r\n\x05total\x18\x05 \x01(\x05\x12\x16\n\x0e\x65xecution_time\x18\x06 \x01(\x02\"h\n\x11LogHookEndLineMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12)\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1b.proto_types.LogHookEndLine\"\x93\x01\n\x0fSkippingDetails\x12(\n\tnode_info\x18\x01 \x01(\x0b\x32\x15.proto_types.NodeInfo\x12\x15\n\rresource_type\x18\x02 \x01(\t\x12\x0e\n\x06schema\x18\x03 \x01(\t\x12\x11\n\tnode_name\x18\x04 \x01(\t\x12\r\n\x05index\x18\x05 \x01(\x05\x12\r\n\x05total\x18\x06 \x01(\x05\"j\n\x12SkippingDetailsMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12*\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1c.proto_types.SkippingDetails\"\r\n\x0bNothingToDo\"b\n\x0eNothingToDoMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12&\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x18.proto_types.NothingToDo\",\n\x1dRunningOperationUncaughtError\x12\x0b\n\x03\x65xc\x18\x01 \x01(\t\"\x86\x01\n RunningOperationUncaughtErrorMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12\x38\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32*.proto_types.RunningOperationUncaughtError\"\x93\x01\n\x0c\x45ndRunResult\x12*\n\x07results\x18\x01 \x03(\x0b\x32\x19.proto_types.RunResultMsg\x12\x14\n\x0c\x65lapsed_time\x18\x02 \x01(\x02\x12\x30\n\x0cgenerated_at\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x0f\n\x07success\x18\x04 \x01(\x08\"d\n\x0f\x45ndRunResultMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12\'\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x19.proto_types.EndRunResult\"\x11\n\x0fNoNodesSelected\"j\n\x12NoNodesSelectedMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12*\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1c.proto_types.NoNodesSelected\"w\n\x10\x43ommandCompleted\x12\x0f\n\x07\x63ommand\x18\x01 \x01(\t\x12\x0f\n\x07success\x18\x02 \x01(\x08\x12\x30\n\x0c\x63ompleted_at\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x0f\n\x07\x65lapsed\x18\x04 \x01(\x02\"l\n\x13\x43ommandCompletedMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12+\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1d.proto_types.CommandCompleted\"k\n\x08ShowNode\x12\x11\n\tnode_name\x18\x01 \x01(\t\x12\x0f\n\x07preview\x18\x02 \x01(\t\x12\x11\n\tis_inline\x18\x03 \x01(\x08\x12\x15\n\routput_format\x18\x04 \x01(\t\x12\x11\n\tunique_id\x18\x05 \x01(\t\"\\\n\x0bShowNodeMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12#\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x15.proto_types.ShowNode\"p\n\x0c\x43ompiledNode\x12\x11\n\tnode_name\x18\x01 \x01(\t\x12\x10\n\x08\x63ompiled\x18\x02 \x01(\t\x12\x11\n\tis_inline\x18\x03 \x01(\x08\x12\x15\n\routput_format\x18\x04 \x01(\t\x12\x11\n\tunique_id\x18\x05 \x01(\t\"d\n\x0f\x43ompiledNodeMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12\'\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x19.proto_types.CompiledNode\"b\n\x17\x43\x61tchableExceptionOnRun\x12(\n\tnode_info\x18\x01 \x01(\x0b\x32\x15.proto_types.NodeInfo\x12\x0b\n\x03\x65xc\x18\x02 \x01(\t\x12\x10\n\x08\x65xc_info\x18\x03 \x01(\t\"z\n\x1a\x43\x61tchableExceptionOnRunMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12\x32\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32$.proto_types.CatchableExceptionOnRun\"_\n\x12InternalErrorOnRun\x12\x12\n\nbuild_path\x18\x01 \x01(\t\x12\x0b\n\x03\x65xc\x18\x02 \x01(\t\x12(\n\tnode_info\x18\x03 \x01(\x0b\x32\x15.proto_types.NodeInfo\"p\n\x15InternalErrorOnRunMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12-\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1f.proto_types.InternalErrorOnRun\"u\n\x15GenericExceptionOnRun\x12\x12\n\nbuild_path\x18\x01 \x01(\t\x12\x11\n\tunique_id\x18\x02 \x01(\t\x12\x0b\n\x03\x65xc\x18\x03 \x01(\t\x12(\n\tnode_info\x18\x04 \x01(\x0b\x32\x15.proto_types.NodeInfo\"v\n\x18GenericExceptionOnRunMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12\x30\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\".proto_types.GenericExceptionOnRun\"N\n\x1aNodeConnectionReleaseError\x12\x11\n\tnode_name\x18\x01 \x01(\t\x12\x0b\n\x03\x65xc\x18\x02 \x01(\t\x12\x10\n\x08\x65xc_info\x18\x03 \x01(\t\"\x80\x01\n\x1dNodeConnectionReleaseErrorMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12\x35\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\'.proto_types.NodeConnectionReleaseError\"\x1f\n\nFoundStats\x12\x11\n\tstat_line\x18\x01 \x01(\t\"`\n\rFoundStatsMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12%\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x17.proto_types.FoundStats\"\x17\n\x15MainKeyboardInterrupt\"v\n\x18MainKeyboardInterruptMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12\x30\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\".proto_types.MainKeyboardInterrupt\"#\n\x14MainEncounteredError\x12\x0b\n\x03\x65xc\x18\x01 \x01(\t\"t\n\x17MainEncounteredErrorMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12/\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32!.proto_types.MainEncounteredError\"%\n\x0eMainStackTrace\x12\x13\n\x0bstack_trace\x18\x01 \x01(\t\"h\n\x11MainStackTraceMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12)\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1b.proto_types.MainStackTrace\"p\n\x13TimingInfoCollected\x12(\n\tnode_info\x18\x01 \x01(\x0b\x32\x15.proto_types.NodeInfo\x12/\n\x0btiming_info\x18\x02 \x01(\x0b\x32\x1a.proto_types.TimingInfoMsg\"r\n\x16TimingInfoCollectedMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12.\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32 .proto_types.TimingInfoCollected\"&\n\x12LogDebugStackTrace\x12\x10\n\x08\x65xc_info\x18\x01 \x01(\t\"p\n\x15LogDebugStackTraceMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12-\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1f.proto_types.LogDebugStackTrace\"\x1e\n\x0e\x43heckCleanPath\x12\x0c\n\x04path\x18\x01 \x01(\t\"h\n\x11\x43heckCleanPathMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12)\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1b.proto_types.CheckCleanPath\" \n\x10\x43onfirmCleanPath\x12\x0c\n\x04path\x18\x01 \x01(\t\"l\n\x13\x43onfirmCleanPathMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12+\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1d.proto_types.ConfirmCleanPath\"\"\n\x12ProtectedCleanPath\x12\x0c\n\x04path\x18\x01 \x01(\t\"p\n\x15ProtectedCleanPathMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12-\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1f.proto_types.ProtectedCleanPath\"\x14\n\x12\x46inishedCleanPaths\"p\n\x15\x46inishedCleanPathsMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12-\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1f.proto_types.FinishedCleanPaths\"5\n\x0bOpenCommand\x12\x10\n\x08open_cmd\x18\x01 \x01(\t\x12\x14\n\x0cprofiles_dir\x18\x02 \x01(\t\"b\n\x0eOpenCommandMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12&\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x18.proto_types.OpenCommand\"0\n\x0fServingDocsPort\x12\x0f\n\x07\x61\x64\x64ress\x18\x01 \x01(\t\x12\x0c\n\x04port\x18\x02 \x01(\x05\"j\n\x12ServingDocsPortMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12*\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1c.proto_types.ServingDocsPort\"%\n\x15ServingDocsAccessInfo\x12\x0c\n\x04port\x18\x01 \x01(\t\"v\n\x18ServingDocsAccessInfoMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12\x30\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\".proto_types.ServingDocsAccessInfo\"\x15\n\x13ServingDocsExitInfo\"r\n\x16ServingDocsExitInfoMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12.\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32 .proto_types.ServingDocsExitInfo\"t\n\x10RunResultWarning\x12\x15\n\rresource_type\x18\x01 \x01(\t\x12\x11\n\tnode_name\x18\x02 \x01(\t\x12\x0c\n\x04path\x18\x03 \x01(\t\x12(\n\tnode_info\x18\x04 \x01(\x0b\x32\x15.proto_types.NodeInfo\"l\n\x13RunResultWarningMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12+\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1d.proto_types.RunResultWarning\"t\n\x10RunResultFailure\x12\x15\n\rresource_type\x18\x01 \x01(\t\x12\x11\n\tnode_name\x18\x02 \x01(\t\x12\x0c\n\x04path\x18\x03 \x01(\t\x12(\n\tnode_info\x18\x04 \x01(\x0b\x32\x15.proto_types.NodeInfo\"l\n\x13RunResultFailureMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12+\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1d.proto_types.RunResultFailure\"k\n\tStatsLine\x12\x30\n\x05stats\x18\x01 \x03(\x0b\x32!.proto_types.StatsLine.StatsEntry\x1a,\n\nStatsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\x05:\x02\x38\x01\"^\n\x0cStatsLineMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12$\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x16.proto_types.StatsLine\"G\n\x0eRunResultError\x12\x0b\n\x03msg\x18\x01 \x01(\t\x12(\n\tnode_info\x18\x02 \x01(\x0b\x32\x15.proto_types.NodeInfo\"h\n\x11RunResultErrorMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12)\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1b.proto_types.RunResultError\"S\n\x17RunResultErrorNoMessage\x12\x0e\n\x06status\x18\x01 \x01(\t\x12(\n\tnode_info\x18\x02 \x01(\x0b\x32\x15.proto_types.NodeInfo\"z\n\x1aRunResultErrorNoMessageMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12\x32\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32$.proto_types.RunResultErrorNoMessage\"I\n\x0fSQLCompiledPath\x12\x0c\n\x04path\x18\x01 \x01(\t\x12(\n\tnode_info\x18\x02 \x01(\x0b\x32\x15.proto_types.NodeInfo\"j\n\x12SQLCompiledPathMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12*\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1c.proto_types.SQLCompiledPath\"W\n\x14\x43heckNodeTestFailure\x12\x15\n\rrelation_name\x18\x01 \x01(\t\x12(\n\tnode_info\x18\x02 \x01(\x0b\x32\x15.proto_types.NodeInfo\"t\n\x17\x43heckNodeTestFailureMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12/\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32!.proto_types.CheckNodeTestFailure\"W\n\x0f\x45ndOfRunSummary\x12\x12\n\nnum_errors\x18\x01 \x01(\x05\x12\x14\n\x0cnum_warnings\x18\x02 \x01(\x05\x12\x1a\n\x12keyboard_interrupt\x18\x03 \x01(\x08\"j\n\x12\x45ndOfRunSummaryMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12*\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1c.proto_types.EndOfRunSummary\"U\n\x13LogSkipBecauseError\x12\x0e\n\x06schema\x18\x01 \x01(\t\x12\x10\n\x08relation\x18\x02 \x01(\t\x12\r\n\x05index\x18\x03 \x01(\x05\x12\r\n\x05total\x18\x04 \x01(\x05\"r\n\x16LogSkipBecauseErrorMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12.\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32 .proto_types.LogSkipBecauseError\"\x14\n\x12\x45nsureGitInstalled\"p\n\x15\x45nsureGitInstalledMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12-\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1f.proto_types.EnsureGitInstalled\"\x1a\n\x18\x44\x65psCreatingLocalSymlink\"|\n\x1b\x44\x65psCreatingLocalSymlinkMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12\x33\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32%.proto_types.DepsCreatingLocalSymlink\"\x19\n\x17\x44\x65psSymlinkNotAvailable\"z\n\x1a\x44\x65psSymlinkNotAvailableMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12\x32\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32$.proto_types.DepsSymlinkNotAvailable\"\x11\n\x0f\x44isableTracking\"j\n\x12\x44isableTrackingMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12*\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1c.proto_types.DisableTracking\"\x1e\n\x0cSendingEvent\x12\x0e\n\x06kwargs\x18\x01 \x01(\t\"d\n\x0fSendingEventMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12\'\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x19.proto_types.SendingEvent\"\x12\n\x10SendEventFailure\"l\n\x13SendEventFailureMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12+\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1d.proto_types.SendEventFailure\"\r\n\x0b\x46lushEvents\"b\n\x0e\x46lushEventsMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12&\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x18.proto_types.FlushEvents\"\x14\n\x12\x46lushEventsFailure\"p\n\x15\x46lushEventsFailureMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12-\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1f.proto_types.FlushEventsFailure\"-\n\x19TrackingInitializeFailure\x12\x10\n\x08\x65xc_info\x18\x01 \x01(\t\"~\n\x1cTrackingInitializeFailureMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12\x34\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32&.proto_types.TrackingInitializeFailure\"P\n\x17RunResultWarningMessage\x12\x0b\n\x03msg\x18\x01 \x01(\t\x12(\n\tnode_info\x18\x02 \x01(\x0b\x32\x15.proto_types.NodeInfo\"z\n\x1aRunResultWarningMessageMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12\x32\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32$.proto_types.RunResultWarningMessage\"\x1a\n\x0b\x44\x65\x62ugCmdOut\x12\x0b\n\x03msg\x18\x01 \x01(\t\"b\n\x0e\x44\x65\x62ugCmdOutMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12&\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x18.proto_types.DebugCmdOut\"\x1d\n\x0e\x44\x65\x62ugCmdResult\x12\x0b\n\x03msg\x18\x01 \x01(\t\"h\n\x11\x44\x65\x62ugCmdResultMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12)\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1b.proto_types.DebugCmdResult\"\x19\n\nListCmdOut\x12\x0b\n\x03msg\x18\x01 \x01(\t\"`\n\rListCmdOutMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12%\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x17.proto_types.ListCmdOut\"\xec\x01\n\x0eResourceReport\x12\x14\n\x0c\x63ommand_name\x18\x02 \x01(\t\x12\x17\n\x0f\x63ommand_success\x18\x03 \x01(\x08\x12\x1f\n\x17\x63ommand_wall_clock_time\x18\x04 \x01(\x02\x12\x19\n\x11process_user_time\x18\x05 \x01(\x02\x12\x1b\n\x13process_kernel_time\x18\x06 \x01(\x02\x12\x1b\n\x13process_mem_max_rss\x18\x07 \x01(\x03\x12\x19\n\x11process_in_blocks\x18\x08 \x01(\x03\x12\x1a\n\x12process_out_blocks\x18\t \x01(\x03\"h\n\x11ResourceReportMsg\x12(\n\x04info\x18\x01 \x01(\x0b\x32\x1a.proto_types.CoreEventInfo\x12)\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1b.proto_types.ResourceReportb\x06proto3')
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'core_types_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
   DESCRIPTOR._options = None
   _globals['_COREEVENTINFO_EXTRAENTRY']._options = None
@@ -646,101 +646,101 @@
   _globals['_SERVINGDOCSACCESSINFOMSG']._serialized_start=29310
   _globals['_SERVINGDOCSACCESSINFOMSG']._serialized_end=29428
   _globals['_SERVINGDOCSEXITINFO']._serialized_start=29430
   _globals['_SERVINGDOCSEXITINFO']._serialized_end=29451
   _globals['_SERVINGDOCSEXITINFOMSG']._serialized_start=29453
   _globals['_SERVINGDOCSEXITINFOMSG']._serialized_end=29567
   _globals['_RUNRESULTWARNING']._serialized_start=29569
-  _globals['_RUNRESULTWARNING']._serialized_end=29643
-  _globals['_RUNRESULTWARNINGMSG']._serialized_start=29645
-  _globals['_RUNRESULTWARNINGMSG']._serialized_end=29753
-  _globals['_RUNRESULTFAILURE']._serialized_start=29755
-  _globals['_RUNRESULTFAILURE']._serialized_end=29829
-  _globals['_RUNRESULTFAILUREMSG']._serialized_start=29831
-  _globals['_RUNRESULTFAILUREMSG']._serialized_end=29939
-  _globals['_STATSLINE']._serialized_start=29941
-  _globals['_STATSLINE']._serialized_end=30048
-  _globals['_STATSLINE_STATSENTRY']._serialized_start=30004
-  _globals['_STATSLINE_STATSENTRY']._serialized_end=30048
-  _globals['_STATSLINEMSG']._serialized_start=30050
-  _globals['_STATSLINEMSG']._serialized_end=30144
-  _globals['_RUNRESULTERROR']._serialized_start=30146
-  _globals['_RUNRESULTERROR']._serialized_end=30175
-  _globals['_RUNRESULTERRORMSG']._serialized_start=30177
-  _globals['_RUNRESULTERRORMSG']._serialized_end=30281
-  _globals['_RUNRESULTERRORNOMESSAGE']._serialized_start=30283
-  _globals['_RUNRESULTERRORNOMESSAGE']._serialized_end=30324
-  _globals['_RUNRESULTERRORNOMESSAGEMSG']._serialized_start=30326
-  _globals['_RUNRESULTERRORNOMESSAGEMSG']._serialized_end=30448
-  _globals['_SQLCOMPILEDPATH']._serialized_start=30450
-  _globals['_SQLCOMPILEDPATH']._serialized_end=30481
-  _globals['_SQLCOMPILEDPATHMSG']._serialized_start=30483
-  _globals['_SQLCOMPILEDPATHMSG']._serialized_end=30589
-  _globals['_CHECKNODETESTFAILURE']._serialized_start=30591
-  _globals['_CHECKNODETESTFAILURE']._serialized_end=30636
-  _globals['_CHECKNODETESTFAILUREMSG']._serialized_start=30638
-  _globals['_CHECKNODETESTFAILUREMSG']._serialized_end=30754
-  _globals['_ENDOFRUNSUMMARY']._serialized_start=30756
-  _globals['_ENDOFRUNSUMMARY']._serialized_end=30843
-  _globals['_ENDOFRUNSUMMARYMSG']._serialized_start=30845
-  _globals['_ENDOFRUNSUMMARYMSG']._serialized_end=30951
-  _globals['_LOGSKIPBECAUSEERROR']._serialized_start=30953
-  _globals['_LOGSKIPBECAUSEERROR']._serialized_end=31038
-  _globals['_LOGSKIPBECAUSEERRORMSG']._serialized_start=31040
-  _globals['_LOGSKIPBECAUSEERRORMSG']._serialized_end=31154
-  _globals['_ENSUREGITINSTALLED']._serialized_start=31156
-  _globals['_ENSUREGITINSTALLED']._serialized_end=31176
-  _globals['_ENSUREGITINSTALLEDMSG']._serialized_start=31178
-  _globals['_ENSUREGITINSTALLEDMSG']._serialized_end=31290
-  _globals['_DEPSCREATINGLOCALSYMLINK']._serialized_start=31292
-  _globals['_DEPSCREATINGLOCALSYMLINK']._serialized_end=31318
-  _globals['_DEPSCREATINGLOCALSYMLINKMSG']._serialized_start=31320
-  _globals['_DEPSCREATINGLOCALSYMLINKMSG']._serialized_end=31444
-  _globals['_DEPSSYMLINKNOTAVAILABLE']._serialized_start=31446
-  _globals['_DEPSSYMLINKNOTAVAILABLE']._serialized_end=31471
-  _globals['_DEPSSYMLINKNOTAVAILABLEMSG']._serialized_start=31473
-  _globals['_DEPSSYMLINKNOTAVAILABLEMSG']._serialized_end=31595
-  _globals['_DISABLETRACKING']._serialized_start=31597
-  _globals['_DISABLETRACKING']._serialized_end=31614
-  _globals['_DISABLETRACKINGMSG']._serialized_start=31616
-  _globals['_DISABLETRACKINGMSG']._serialized_end=31722
-  _globals['_SENDINGEVENT']._serialized_start=31724
-  _globals['_SENDINGEVENT']._serialized_end=31754
-  _globals['_SENDINGEVENTMSG']._serialized_start=31756
-  _globals['_SENDINGEVENTMSG']._serialized_end=31856
-  _globals['_SENDEVENTFAILURE']._serialized_start=31858
-  _globals['_SENDEVENTFAILURE']._serialized_end=31876
-  _globals['_SENDEVENTFAILUREMSG']._serialized_start=31878
-  _globals['_SENDEVENTFAILUREMSG']._serialized_end=31986
-  _globals['_FLUSHEVENTS']._serialized_start=31988
-  _globals['_FLUSHEVENTS']._serialized_end=32001
-  _globals['_FLUSHEVENTSMSG']._serialized_start=32003
-  _globals['_FLUSHEVENTSMSG']._serialized_end=32101
-  _globals['_FLUSHEVENTSFAILURE']._serialized_start=32103
-  _globals['_FLUSHEVENTSFAILURE']._serialized_end=32123
-  _globals['_FLUSHEVENTSFAILUREMSG']._serialized_start=32125
-  _globals['_FLUSHEVENTSFAILUREMSG']._serialized_end=32237
-  _globals['_TRACKINGINITIALIZEFAILURE']._serialized_start=32239
-  _globals['_TRACKINGINITIALIZEFAILURE']._serialized_end=32284
-  _globals['_TRACKINGINITIALIZEFAILUREMSG']._serialized_start=32286
-  _globals['_TRACKINGINITIALIZEFAILUREMSG']._serialized_end=32412
-  _globals['_RUNRESULTWARNINGMESSAGE']._serialized_start=32414
-  _globals['_RUNRESULTWARNINGMESSAGE']._serialized_end=32452
-  _globals['_RUNRESULTWARNINGMESSAGEMSG']._serialized_start=32454
-  _globals['_RUNRESULTWARNINGMESSAGEMSG']._serialized_end=32576
-  _globals['_DEBUGCMDOUT']._serialized_start=32578
-  _globals['_DEBUGCMDOUT']._serialized_end=32604
-  _globals['_DEBUGCMDOUTMSG']._serialized_start=32606
-  _globals['_DEBUGCMDOUTMSG']._serialized_end=32704
-  _globals['_DEBUGCMDRESULT']._serialized_start=32706
-  _globals['_DEBUGCMDRESULT']._serialized_end=32735
-  _globals['_DEBUGCMDRESULTMSG']._serialized_start=32737
-  _globals['_DEBUGCMDRESULTMSG']._serialized_end=32841
-  _globals['_LISTCMDOUT']._serialized_start=32843
-  _globals['_LISTCMDOUT']._serialized_end=32868
-  _globals['_LISTCMDOUTMSG']._serialized_start=32870
-  _globals['_LISTCMDOUTMSG']._serialized_end=32966
-  _globals['_RESOURCEREPORT']._serialized_start=32969
-  _globals['_RESOURCEREPORT']._serialized_end=33205
-  _globals['_RESOURCEREPORTMSG']._serialized_start=33207
-  _globals['_RESOURCEREPORTMSG']._serialized_end=33311
+  _globals['_RUNRESULTWARNING']._serialized_end=29685
+  _globals['_RUNRESULTWARNINGMSG']._serialized_start=29687
+  _globals['_RUNRESULTWARNINGMSG']._serialized_end=29795
+  _globals['_RUNRESULTFAILURE']._serialized_start=29797
+  _globals['_RUNRESULTFAILURE']._serialized_end=29913
+  _globals['_RUNRESULTFAILUREMSG']._serialized_start=29915
+  _globals['_RUNRESULTFAILUREMSG']._serialized_end=30023
+  _globals['_STATSLINE']._serialized_start=30025
+  _globals['_STATSLINE']._serialized_end=30132
+  _globals['_STATSLINE_STATSENTRY']._serialized_start=30088
+  _globals['_STATSLINE_STATSENTRY']._serialized_end=30132
+  _globals['_STATSLINEMSG']._serialized_start=30134
+  _globals['_STATSLINEMSG']._serialized_end=30228
+  _globals['_RUNRESULTERROR']._serialized_start=30230
+  _globals['_RUNRESULTERROR']._serialized_end=30301
+  _globals['_RUNRESULTERRORMSG']._serialized_start=30303
+  _globals['_RUNRESULTERRORMSG']._serialized_end=30407
+  _globals['_RUNRESULTERRORNOMESSAGE']._serialized_start=30409
+  _globals['_RUNRESULTERRORNOMESSAGE']._serialized_end=30492
+  _globals['_RUNRESULTERRORNOMESSAGEMSG']._serialized_start=30494
+  _globals['_RUNRESULTERRORNOMESSAGEMSG']._serialized_end=30616
+  _globals['_SQLCOMPILEDPATH']._serialized_start=30618
+  _globals['_SQLCOMPILEDPATH']._serialized_end=30691
+  _globals['_SQLCOMPILEDPATHMSG']._serialized_start=30693
+  _globals['_SQLCOMPILEDPATHMSG']._serialized_end=30799
+  _globals['_CHECKNODETESTFAILURE']._serialized_start=30801
+  _globals['_CHECKNODETESTFAILURE']._serialized_end=30888
+  _globals['_CHECKNODETESTFAILUREMSG']._serialized_start=30890
+  _globals['_CHECKNODETESTFAILUREMSG']._serialized_end=31006
+  _globals['_ENDOFRUNSUMMARY']._serialized_start=31008
+  _globals['_ENDOFRUNSUMMARY']._serialized_end=31095
+  _globals['_ENDOFRUNSUMMARYMSG']._serialized_start=31097
+  _globals['_ENDOFRUNSUMMARYMSG']._serialized_end=31203
+  _globals['_LOGSKIPBECAUSEERROR']._serialized_start=31205
+  _globals['_LOGSKIPBECAUSEERROR']._serialized_end=31290
+  _globals['_LOGSKIPBECAUSEERRORMSG']._serialized_start=31292
+  _globals['_LOGSKIPBECAUSEERRORMSG']._serialized_end=31406
+  _globals['_ENSUREGITINSTALLED']._serialized_start=31408
+  _globals['_ENSUREGITINSTALLED']._serialized_end=31428
+  _globals['_ENSUREGITINSTALLEDMSG']._serialized_start=31430
+  _globals['_ENSUREGITINSTALLEDMSG']._serialized_end=31542
+  _globals['_DEPSCREATINGLOCALSYMLINK']._serialized_start=31544
+  _globals['_DEPSCREATINGLOCALSYMLINK']._serialized_end=31570
+  _globals['_DEPSCREATINGLOCALSYMLINKMSG']._serialized_start=31572
+  _globals['_DEPSCREATINGLOCALSYMLINKMSG']._serialized_end=31696
+  _globals['_DEPSSYMLINKNOTAVAILABLE']._serialized_start=31698
+  _globals['_DEPSSYMLINKNOTAVAILABLE']._serialized_end=31723
+  _globals['_DEPSSYMLINKNOTAVAILABLEMSG']._serialized_start=31725
+  _globals['_DEPSSYMLINKNOTAVAILABLEMSG']._serialized_end=31847
+  _globals['_DISABLETRACKING']._serialized_start=31849
+  _globals['_DISABLETRACKING']._serialized_end=31866
+  _globals['_DISABLETRACKINGMSG']._serialized_start=31868
+  _globals['_DISABLETRACKINGMSG']._serialized_end=31974
+  _globals['_SENDINGEVENT']._serialized_start=31976
+  _globals['_SENDINGEVENT']._serialized_end=32006
+  _globals['_SENDINGEVENTMSG']._serialized_start=32008
+  _globals['_SENDINGEVENTMSG']._serialized_end=32108
+  _globals['_SENDEVENTFAILURE']._serialized_start=32110
+  _globals['_SENDEVENTFAILURE']._serialized_end=32128
+  _globals['_SENDEVENTFAILUREMSG']._serialized_start=32130
+  _globals['_SENDEVENTFAILUREMSG']._serialized_end=32238
+  _globals['_FLUSHEVENTS']._serialized_start=32240
+  _globals['_FLUSHEVENTS']._serialized_end=32253
+  _globals['_FLUSHEVENTSMSG']._serialized_start=32255
+  _globals['_FLUSHEVENTSMSG']._serialized_end=32353
+  _globals['_FLUSHEVENTSFAILURE']._serialized_start=32355
+  _globals['_FLUSHEVENTSFAILURE']._serialized_end=32375
+  _globals['_FLUSHEVENTSFAILUREMSG']._serialized_start=32377
+  _globals['_FLUSHEVENTSFAILUREMSG']._serialized_end=32489
+  _globals['_TRACKINGINITIALIZEFAILURE']._serialized_start=32491
+  _globals['_TRACKINGINITIALIZEFAILURE']._serialized_end=32536
+  _globals['_TRACKINGINITIALIZEFAILUREMSG']._serialized_start=32538
+  _globals['_TRACKINGINITIALIZEFAILUREMSG']._serialized_end=32664
+  _globals['_RUNRESULTWARNINGMESSAGE']._serialized_start=32666
+  _globals['_RUNRESULTWARNINGMESSAGE']._serialized_end=32746
+  _globals['_RUNRESULTWARNINGMESSAGEMSG']._serialized_start=32748
+  _globals['_RUNRESULTWARNINGMESSAGEMSG']._serialized_end=32870
+  _globals['_DEBUGCMDOUT']._serialized_start=32872
+  _globals['_DEBUGCMDOUT']._serialized_end=32898
+  _globals['_DEBUGCMDOUTMSG']._serialized_start=32900
+  _globals['_DEBUGCMDOUTMSG']._serialized_end=32998
+  _globals['_DEBUGCMDRESULT']._serialized_start=33000
+  _globals['_DEBUGCMDRESULT']._serialized_end=33029
+  _globals['_DEBUGCMDRESULTMSG']._serialized_start=33031
+  _globals['_DEBUGCMDRESULTMSG']._serialized_end=33135
+  _globals['_LISTCMDOUT']._serialized_start=33137
+  _globals['_LISTCMDOUT']._serialized_end=33162
+  _globals['_LISTCMDOUTMSG']._serialized_start=33164
+  _globals['_LISTCMDOUTMSG']._serialized_end=33260
+  _globals['_RESOURCEREPORT']._serialized_start=33263
+  _globals['_RESOURCEREPORT']._serialized_end=33499
+  _globals['_RESOURCEREPORTMSG']._serialized_start=33501
+  _globals['_RESOURCEREPORTMSG']._serialized_end=33605
 # @@protoc_insertion_point(module_scope)
```

### Comparing `dbt-core-1.8.0b1/dbt/events/logging.py` & `dbt-core-1.8.0b2/dbt/events/logging.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.8.0b1/dbt/events/types.py` & `dbt-core-1.8.0b2/dbt/events/types.py`

 * *Files 0% similar despite different names*

```diff
@@ -391,15 +391,15 @@
 class TestsConfigDeprecation(WarnLevel):
     def code(self) -> str:
         return "D012"
 
     def message(self) -> str:
         description = (
             f"The `{self.deprecated_path}` config has been renamed to `{self.exp_path}`. "
-            "Please update your `dbt_project.yml` configuration to reflect this change."
+            "Please see https://docs.getdbt.com/docs/build/data-tests#new-data_tests-syntax for more information."
         )
         return line_wrap_message(warning_tag(f"Deprecated functionality\n\n{description}"))
 
 
 class ProjectFlagsMovedDeprecation(WarnLevel):
     def code(self) -> str:
         return "D013"
```

### Comparing `dbt-core-1.8.0b1/dbt/exceptions.py` & `dbt-core-1.8.0b2/dbt/exceptions.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 import json
 import re
 import io
-import agate
-from typing import Any, Dict, List, Mapping, Optional, Union
+from typing import Any, Dict, List, Mapping, Optional, Union, TYPE_CHECKING
 
 from dbt_common.exceptions import (
     DbtRuntimeError,
     CompilationError,
     DbtInternalError,
     DbtConfigError,
     env_secrets,
@@ -15,14 +14,18 @@
     CommandResultError,
 )
 from dbt.node_types import NodeType, AccessType, REFABLE_NODE_TYPES
 
 from dbt_common.dataclass_schema import ValidationError
 
 
+if TYPE_CHECKING:
+    import agate
+
+
 class ContractBreakingChangeError(DbtRuntimeError):
     CODE = 10016
     MESSAGE = "Breaking Change to Contract"
 
     def __init__(
         self,
         breaking_changes: List[str],
@@ -1345,15 +1348,15 @@
 
 class ContractError(CompilationError):
     def __init__(self, yaml_columns, sql_columns):
         self.yaml_columns = yaml_columns
         self.sql_columns = sql_columns
         super().__init__(msg=self.get_message())
 
-    def get_mismatches(self) -> agate.Table:
+    def get_mismatches(self) -> "agate.Table":
         # avoid a circular import
         from dbt_common.clients.agate_helper import table_from_data_flat
 
         column_names = ["column_name", "definition_type", "contract_type", "mismatch_reason"]
         # list of mismatches
         mismatches: List[Dict[str, str]] = []
         # track sql cols so we don't need another for loop later
@@ -1396,15 +1399,15 @@
 
     def get_message(self) -> str:
         if not self.yaml_columns:
             return (
                 "This model has an enforced contract, and its 'columns' specification is missing"
             )
 
-        table: agate.Table = self.get_mismatches()
+        table: "agate.Table" = self.get_mismatches()
         # Hack to get Agate table output as string
         output = io.StringIO()
         table.print_table(output=output, max_rows=None, max_column_width=50)  # type: ignore
         mismatches = output.getvalue()
 
         msg = (
             "This model has an enforced contract that failed.\n"
```

### Comparing `dbt-core-1.8.0b1/dbt/flags.py` & `dbt-core-1.8.0b2/dbt/flags.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.8.0b1/dbt/graph/cli.py` & `dbt-core-1.8.0b2/dbt/graph/cli.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.8.0b1/dbt/graph/graph.py` & `dbt-core-1.8.0b2/dbt/graph/graph.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.8.0b1/dbt/graph/queue.py` & `dbt-core-1.8.0b2/dbt/graph/queue.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.8.0b1/dbt/graph/selector.py` & `dbt-core-1.8.0b2/dbt/graph/selector.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.8.0b1/dbt/graph/selector_methods.py` & `dbt-core-1.8.0b2/dbt/graph/selector_methods.py`

 * *Files 4% similar despite different names*

```diff
@@ -50,15 +50,14 @@
     TestType = "test_type"
     ResourceType = "resource_type"
     State = "state"
     Exposure = "exposure"
     Metric = "metric"
     Result = "result"
     SourceStatus = "source_status"
-    Wildcard = "wildcard"
     Version = "version"
     SemanticModel = "semantic_model"
     SavedQuery = "saved_query"
 
 
 def is_selected_node(fqn: List[str], node_selector: str, is_versioned: bool) -> bool:
     # If qualified_name exactly matches model name (fqn's leaf), return True
@@ -254,45 +253,43 @@
 
     def search(self, included_nodes: Set[UniqueId], selector: str) -> Iterator[UniqueId]:
         """Yield all nodes in the graph that match the selector.
 
         :param str selector: The selector or node name
         """
         non_source_nodes = list(self.non_source_nodes(included_nodes))
-        for node, real_node in non_source_nodes:
-            if self.node_is_match(selector, real_node.fqn, real_node.is_versioned):
-                yield node
+        for unique_id, node in non_source_nodes:
+            if self.node_is_match(selector, node.fqn, node.is_versioned):
+                yield unique_id
 
 
 class TagSelectorMethod(SelectorMethod):
     def search(self, included_nodes: Set[UniqueId], selector: str) -> Iterator[UniqueId]:
         """yields nodes from included that have the specified tag"""
-        for node, real_node in self.all_nodes(included_nodes):
-            if hasattr(real_node, "tags") and any(
-                fnmatch(tag, selector) for tag in real_node.tags
-            ):
-                yield node
+        for unique_id, node in self.all_nodes(included_nodes):
+            if hasattr(node, "tags") and any(fnmatch(tag, selector) for tag in node.tags):
+                yield unique_id
 
 
 class GroupSelectorMethod(SelectorMethod):
     def search(self, included_nodes: Set[UniqueId], selector: str) -> Iterator[UniqueId]:
         """yields nodes from included in the specified group"""
-        for node, real_node in self.groupable_nodes(included_nodes):
-            if selector == real_node.config.get("group"):
-                yield node
+        for unique_id, node in self.groupable_nodes(included_nodes):
+            if selector == node.config.get("group"):
+                yield unique_id
 
 
 class AccessSelectorMethod(SelectorMethod):
     def search(self, included_nodes: Set[UniqueId], selector: str) -> Iterator[UniqueId]:
         """yields model nodes matching the specified access level"""
-        for node, real_node in self.parsed_nodes(included_nodes):
-            if not isinstance(real_node, ModelNode):
+        for unique_id, node in self.parsed_nodes(included_nodes):
+            if not isinstance(node, ModelNode):
                 continue
-            if selector == real_node.access:
-                yield node
+            if selector == node.access:
+                yield unique_id
 
 
 class SourceSelectorMethod(SelectorMethod):
     def search(self, included_nodes: Set[UniqueId], selector: str) -> Iterator[UniqueId]:
         """yields nodes from included are the specified source."""
         parts = selector.split(".")
         target_package = SELECTOR_GLOB
@@ -307,22 +304,22 @@
                 'Invalid source selector value "{}". Sources must be of the '
                 "form `${{source_name}}`, "
                 "`${{source_name}}.${{target_name}}`, or "
                 "`${{package_name}}.${{source_name}}.${{target_name}}"
             ).format(selector)
             raise DbtRuntimeError(msg)
 
-        for node, real_node in self.source_nodes(included_nodes):
-            if not fnmatch(real_node.package_name, target_package):
+        for unique_id, node in self.source_nodes(included_nodes):
+            if not fnmatch(node.package_name, target_package):
                 continue
-            if not fnmatch(real_node.source_name, target_source):
+            if not fnmatch(node.source_name, target_source):
                 continue
-            if not fnmatch(real_node.name, target_table):
+            if not fnmatch(node.name, target_table):
                 continue
-            yield node
+            yield unique_id
 
 
 class ExposureSelectorMethod(SelectorMethod):
     def search(self, included_nodes: Set[UniqueId], selector: str) -> Iterator[UniqueId]:
         parts = selector.split(".")
         target_package = SELECTOR_GLOB
         if len(parts) == 1:
@@ -333,21 +330,21 @@
             msg = (
                 'Invalid exposure selector value "{}". Exposures must be of '
                 "the form ${{exposure_name}} or "
                 "${{exposure_package.exposure_name}}"
             ).format(selector)
             raise DbtRuntimeError(msg)
 
-        for node, real_node in self.exposure_nodes(included_nodes):
-            if not fnmatch(real_node.package_name, target_package):
+        for unique_id, node in self.exposure_nodes(included_nodes):
+            if not fnmatch(node.package_name, target_package):
                 continue
-            if not fnmatch(real_node.name, target_name):
+            if not fnmatch(node.name, target_name):
                 continue
 
-            yield node
+            yield unique_id
 
 
 class MetricSelectorMethod(SelectorMethod):
     def search(self, included_nodes: Set[UniqueId], selector: str) -> Iterator[UniqueId]:
         parts = selector.split(".")
         target_package = SELECTOR_GLOB
         if len(parts) == 1:
@@ -358,21 +355,21 @@
             msg = (
                 'Invalid metric selector value "{}". Metrics must be of '
                 "the form ${{metric_name}} or "
                 "${{metric_package.metric_name}}"
             ).format(selector)
             raise DbtRuntimeError(msg)
 
-        for node, real_node in self.metric_nodes(included_nodes):
-            if not fnmatch(real_node.package_name, target_package):
+        for unique_id, node in self.metric_nodes(included_nodes):
+            if not fnmatch(node.package_name, target_package):
                 continue
-            if not fnmatch(real_node.name, target_name):
+            if not fnmatch(node.name, target_name):
                 continue
 
-            yield node
+            yield unique_id
 
 
 class SemanticModelSelectorMethod(SelectorMethod):
     def search(self, included_nodes: Set[UniqueId], selector: str) -> Iterator[UniqueId]:
         parts = selector.split(".")
         target_package = SELECTOR_GLOB
         if len(parts) == 1:
@@ -383,21 +380,21 @@
             msg = (
                 'Invalid semantic model selector value "{}". Semantic models must be of '
                 "the form ${{semantic_model_name}} or "
                 "${{semantic_model_package.semantic_model_name}}"
             ).format(selector)
             raise DbtRuntimeError(msg)
 
-        for node, real_node in self.semantic_model_nodes(included_nodes):
-            if not fnmatch(real_node.package_name, target_package):
+        for unique_id, node in self.semantic_model_nodes(included_nodes):
+            if not fnmatch(node.package_name, target_package):
                 continue
-            if not fnmatch(real_node.name, target_name):
+            if not fnmatch(node.name, target_name):
                 continue
 
-            yield node
+            yield unique_id
 
 
 class SavedQuerySelectorMethod(SelectorMethod):
     def search(self, included_nodes: Set[UniqueId], selector: str) -> Iterator[UniqueId]:
         parts = selector.split(".")
         target_package = SELECTOR_GLOB
         if len(parts) == 1:
@@ -408,62 +405,62 @@
             msg = (
                 'Invalid saved query selector value "{}". Saved queries must be of '
                 "the form ${{saved_query_name}} or "
                 "${{saved_query_package.saved_query_name}}"
             ).format(selector)
             raise DbtRuntimeError(msg)
 
-        for node, real_node in self.saved_query_nodes(included_nodes):
-            if not fnmatch(real_node.package_name, target_package):
+        for unique_id, node in self.saved_query_nodes(included_nodes):
+            if not fnmatch(node.package_name, target_package):
                 continue
-            if not fnmatch(real_node.name, target_name):
+            if not fnmatch(node.name, target_name):
                 continue
 
-            yield node
+            yield unique_id
 
 
 class PathSelectorMethod(SelectorMethod):
     def search(self, included_nodes: Set[UniqueId], selector: str) -> Iterator[UniqueId]:
         """Yields nodes from included that match the given path."""
         # get project root from contextvar
         project_root = get_project_root()
         if project_root:
             root = Path(project_root)
         else:
             root = Path.cwd()
         paths = set(p.relative_to(root) for p in root.glob(selector))
-        for node, real_node in self.all_nodes(included_nodes):
-            ofp = Path(real_node.original_file_path)
+        for unique_id, node in self.all_nodes(included_nodes):
+            ofp = Path(node.original_file_path)
             if ofp in paths:
-                yield node
-            if hasattr(real_node, "patch_path") and real_node.patch_path:  # type: ignore
-                pfp = real_node.patch_path.split("://")[1]  # type: ignore
+                yield unique_id
+            if hasattr(node, "patch_path") and node.patch_path:  # type: ignore
+                pfp = node.patch_path.split("://")[1]  # type: ignore
                 ymlfp = Path(pfp)
                 if ymlfp in paths:
-                    yield node
+                    yield unique_id
             if any(parent in paths for parent in ofp.parents):
-                yield node
+                yield unique_id
 
 
 class FileSelectorMethod(SelectorMethod):
     def search(self, included_nodes: Set[UniqueId], selector: str) -> Iterator[UniqueId]:
         """Yields nodes from included that match the given file name."""
-        for node, real_node in self.all_nodes(included_nodes):
-            if fnmatch(Path(real_node.original_file_path).name, selector):
-                yield node
-            elif fnmatch(Path(real_node.original_file_path).stem, selector):
-                yield node
+        for unique_id, node in self.all_nodes(included_nodes):
+            if fnmatch(Path(node.original_file_path).name, selector):
+                yield unique_id
+            elif fnmatch(Path(node.original_file_path).stem, selector):
+                yield unique_id
 
 
 class PackageSelectorMethod(SelectorMethod):
     def search(self, included_nodes: Set[UniqueId], selector: str) -> Iterator[UniqueId]:
         """Yields nodes from included that have the specified package"""
-        for node, real_node in self.all_nodes(included_nodes):
-            if fnmatch(real_node.package_name, selector):
-                yield node
+        for unique_id, node in self.all_nodes(included_nodes):
+            if fnmatch(node.package_name, selector):
+                yield unique_id
 
 
 def _getattr_descend(obj: Any, attrs: List[str]) -> Any:
     value = obj
     for attr in attrs:
         try:
             value = getattr(value, attr)
@@ -497,46 +494,46 @@
         # make the comparison case-insensitive
         if parts == ["severity"]:
             selector = CaseInsensitive(selector)
 
         # search sources is kind of useless now source configs only have
         # 'enabled', which you can't really filter on anyway, but maybe we'll
         # add more someday, so search them anyway.
-        for node, real_node in self.configurable_nodes(included_nodes):
+        for unique_id, node in self.configurable_nodes(included_nodes):
             try:
-                value = _getattr_descend(real_node.config, parts)
+                value = _getattr_descend(node.config, parts)
             except AttributeError:
                 continue
             else:
                 if isinstance(value, list):
                     if (
                         (selector in value)
                         or (CaseInsensitive(selector) == "true" and True in value)
                         or (CaseInsensitive(selector) == "false" and False in value)
                     ):
-                        yield node
+                        yield unique_id
                 else:
                     if (
                         (selector == value)
                         or (CaseInsensitive(selector) == "true" and value is True)
                         or (CaseInsensitive(selector) == "false")
                         and value is False
                     ):
-                        yield node
+                        yield unique_id
 
 
 class ResourceTypeSelectorMethod(SelectorMethod):
     def search(self, included_nodes: Set[UniqueId], selector: str) -> Iterator[UniqueId]:
         try:
             resource_type = NodeType(selector)
         except ValueError as exc:
             raise DbtRuntimeError(f'Invalid resource_type selector "{selector}"') from exc
-        for node, real_node in self.all_nodes(included_nodes):
-            if real_node.resource_type == resource_type:
-                yield node
+        for unique_id, node in self.all_nodes(included_nodes):
+            if node.resource_type == resource_type:
+                yield unique_id
 
 
 class TestNameSelectorMethod(SelectorMethod):
     __test__ = False
 
     def search(self, included_nodes: Set[UniqueId], selector: str) -> Iterator[UniqueId]:
         for unique_id, node in self.parsed_and_unit_nodes(included_nodes):
@@ -758,17 +755,17 @@
 class ResultSelectorMethod(SelectorMethod):
     def search(self, included_nodes: Set[UniqueId], selector: str) -> Iterator[UniqueId]:
         if self.previous_state is None or self.previous_state.results is None:
             raise DbtInternalError("No comparison run_results")
         matches = set(
             result.unique_id for result in self.previous_state.results if result.status == selector
         )
-        for node, real_node in self.all_nodes(included_nodes):
-            if node in matches:
-                yield node
+        for unique_id, node in self.all_nodes(included_nodes):
+            if unique_id in matches:
+                yield unique_id
 
 
 class SourceStatusSelectorMethod(SelectorMethod):
     def search(self, included_nodes: Set[UniqueId], selector: str) -> Iterator[UniqueId]:
 
         if self.previous_state is None or self.previous_state.sources is None:
             raise DbtInternalError(
@@ -812,45 +809,45 @@
             for unique_id in matches:
                 if (
                     unique_id in previous_state_sources_runtime_error
                     or unique_id in current_state_sources_runtime_error
                 ):
                     matches.remove(unique_id)
 
-        for node, real_node in self.all_nodes(included_nodes):
-            if node in matches:
-                yield node
+        for unique_id, node in self.all_nodes(included_nodes):
+            if unique_id in matches:
+                yield unique_id
 
 
 class VersionSelectorMethod(SelectorMethod):
     def search(self, included_nodes: Set[UniqueId], selector: str) -> Iterator[UniqueId]:
-        for node, real_node in self.parsed_nodes(included_nodes):
-            if isinstance(real_node, ModelNode):
+        for unique_id, node in self.parsed_nodes(included_nodes):
+            if isinstance(node, ModelNode):
                 if selector == "latest":
-                    if real_node.is_latest_version:
-                        yield node
+                    if node.is_latest_version:
+                        yield unique_id
                 elif selector == "prerelease":
                     if (
-                        real_node.version
-                        and real_node.latest_version
-                        and UnparsedVersion(v=real_node.version)
-                        > UnparsedVersion(v=real_node.latest_version)
+                        node.version
+                        and node.latest_version
+                        and UnparsedVersion(v=node.version)
+                        > UnparsedVersion(v=node.latest_version)
                     ):
-                        yield node
+                        yield unique_id
                 elif selector == "old":
                     if (
-                        real_node.version
-                        and real_node.latest_version
-                        and UnparsedVersion(v=real_node.version)
-                        < UnparsedVersion(v=real_node.latest_version)
+                        node.version
+                        and node.latest_version
+                        and UnparsedVersion(v=node.version)
+                        < UnparsedVersion(v=node.latest_version)
                     ):
-                        yield node
+                        yield unique_id
                 elif selector == "none":
-                    if real_node.version is None:
-                        yield node
+                    if node.version is None:
+                        yield unique_id
                 else:
                     raise DbtRuntimeError(
                         f'Invalid version type selector {selector}: expected one of: "latest", "prerelease", "old", or "none"'
                     )
 
 
 class MethodManager:
```

### Comparing `dbt-core-1.8.0b1/dbt/graph/selector_spec.py` & `dbt-core-1.8.0b2/dbt/graph/selector_spec.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.8.0b1/dbt/include/README.md` & `dbt-core-1.8.0b2/dbt/include/README.md`

 * *Files identical despite different names*

### Comparing `dbt-core-1.8.0b1/dbt/include/starter_project/README.md` & `dbt-core-1.8.0b2/dbt/include/starter_project/README.md`

 * *Files identical despite different names*

### Comparing `dbt-core-1.8.0b1/dbt/include/starter_project/dbt_project.yml` & `dbt-core-1.8.0b2/dbt/include/starter_project/dbt_project.yml`

 * *Files identical despite different names*

### Comparing `dbt-core-1.8.0b1/dbt/internal_deprecations.py` & `dbt-core-1.8.0b2/dbt/internal_deprecations.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.8.0b1/dbt/logger.py` & `dbt-core-1.8.0b2/dbt/logger.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.8.0b1/dbt/node_types.py` & `dbt-core-1.8.0b2/dbt/node_types.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.8.0b1/dbt/parser/__init__.py` & `dbt-core-1.8.0b2/dbt/parser/__init__.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.8.0b1/dbt/parser/analysis.py` & `dbt-core-1.8.0b2/dbt/parser/analysis.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.8.0b1/dbt/parser/base.py` & `dbt-core-1.8.0b2/dbt/parser/base.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.8.0b1/dbt/parser/common.py` & `dbt-core-1.8.0b2/dbt/parser/common.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.8.0b1/dbt/parser/docs.py` & `dbt-core-1.8.0b2/dbt/parser/docs.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.8.0b1/dbt/parser/fixtures.py` & `dbt-core-1.8.0b2/dbt/parser/fixtures.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.8.0b1/dbt/parser/generic_test.py` & `dbt-core-1.8.0b2/dbt/parser/generic_test.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.8.0b1/dbt/parser/generic_test_builders.py` & `dbt-core-1.8.0b2/dbt/parser/generic_test_builders.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.8.0b1/dbt/parser/hooks.py` & `dbt-core-1.8.0b2/dbt/parser/hooks.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.8.0b1/dbt/parser/macros.py` & `dbt-core-1.8.0b2/dbt/parser/macros.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.8.0b1/dbt/parser/manifest.py` & `dbt-core-1.8.0b2/dbt/parser/manifest.py`

 * *Files 2% similar despite different names*

```diff
@@ -266,14 +266,15 @@
         # State check determines whether the saved_manifest and the current
         # manifest match well enough to do partial parsing
         self.manifest.state_check = self.build_manifest_state_check()
         # We need to know if we're actually partially parsing. It could
         # have been enabled, but not happening because of some issue.
         self.partially_parsing = False
         self.partial_parser: Optional[PartialParsing] = None
+        self.skip_parsing = False
 
         # This is a saved manifest from a previous run that's used for partial parsing
         self.saved_manifest: Optional[Manifest] = self.read_manifest_for_partial_parse()
 
     # This is the method that builds a complete manifest. We sometimes
     # use an abbreviated process in tests.
     @classmethod
@@ -370,79 +371,23 @@
         # Set the files in the manifest and save the project_parser_files
         file_reader.read_files()
         self.manifest.files = file_reader.files
         project_parser_files = orig_project_parser_files = file_reader.project_parser_files
         self._perf_info.path_count = len(self.manifest.files)
         self._perf_info.read_files_elapsed = time.perf_counter() - start_read_files
 
-        skip_parsing = False
-        if self.saved_manifest is not None:
-            self.partial_parser = PartialParsing(self.saved_manifest, self.manifest.files)
-            skip_parsing = self.partial_parser.skip_parsing()
-            if skip_parsing:
-                # nothing changed, so we don't need to generate project_parser_files
-                self.manifest = self.saved_manifest
-            else:
-                # create child_map and parent_map
-                self.saved_manifest.build_parent_and_child_maps()
-                # create group_map
-                self.saved_manifest.build_group_map()
-                # files are different, we need to create a new set of
-                # project_parser_files.
-                try:
-                    project_parser_files = self.partial_parser.get_parsing_files()
-                    self.partially_parsing = True
-                    self.manifest = self.saved_manifest
-                except Exception as exc:
-                    # pp_files should still be the full set and manifest is new manifest,
-                    # since get_parsing_files failed
-                    fire_event(
-                        UnableToPartialParse(
-                            reason="an error occurred. Switching to full reparse."
-                        )
-                    )
-
-                    # Get traceback info
-                    tb_info = traceback.format_exc()
-                    formatted_lines = tb_info.splitlines()
-                    (_, line, method) = formatted_lines[-3].split(", ")
-                    exc_info = {
-                        "traceback": tb_info,
-                        "exception": formatted_lines[-1],
-                        "code": formatted_lines[-2],
-                        "location": f"{line} {method}",
-                    }
-
-                    # get file info for local logs
-                    parse_file_type: str = ""
-                    file_id = self.partial_parser.processing_file
-                    if file_id:
-                        source_file = None
-                        if file_id in self.saved_manifest.files:
-                            source_file = self.saved_manifest.files[file_id]
-                        elif file_id in self.manifest.files:
-                            source_file = self.manifest.files[file_id]
-                        if source_file:
-                            parse_file_type = source_file.parse_file_type
-                            fire_event(PartialParsingErrorProcessingFile(file=file_id))
-                    exc_info["parse_file_type"] = parse_file_type
-                    fire_event(PartialParsingError(exc_info=exc_info))
-
-                    # Send event
-                    if dbt.tracking.active_user is not None:
-                        exc_info["full_reparse_reason"] = ReparseReason.exception
-                        dbt.tracking.track_partial_parser(exc_info)
-
-                    if os.environ.get("DBT_PP_TEST"):
-                        raise exc
+        self.skip_parsing = False
+        project_parser_files = self.safe_update_project_parser_files_partially(
+            project_parser_files
+        )
 
         if self.manifest._parsing_info is None:
             self.manifest._parsing_info = ParsingInfo()
 
-        if skip_parsing:
+        if self.skip_parsing:
             fire_event(PartialParsingSkipParsing())
         else:
             # Load Macros and tests
             # We need to parse the macros first, so they're resolvable when
             # the other files are loaded.  Also need to parse tests, specifically
             # generic tests
             start_load_macros = time.perf_counter()
@@ -552,36 +497,98 @@
             )
             self._perf_info.static_analysis_path_count = (
                 self.manifest._parsing_info.static_analysis_path_count
             )
 
         # Inject any available external nodes, reprocess refs if changes to the manifest were made.
         external_nodes_modified = False
-        if skip_parsing:
+        if self.skip_parsing:
             # If we didn't skip parsing, this will have already run because it must run
             # before process_refs. If we did skip parsing, then it's possible that only
             # external nodes have changed and we need to run this to capture that.
             self.manifest.build_parent_and_child_maps()
             external_nodes_modified = self.inject_external_nodes()
             if external_nodes_modified:
                 self.manifest.rebuild_ref_lookup()
                 self.process_refs(
                     self.root_project.project_name,
                     self.root_project.dependencies,
                 )
                 # parent and child maps will be rebuilt by write_manifest
 
-        if not skip_parsing or external_nodes_modified:
+        if not self.skip_parsing or external_nodes_modified:
             # write out the fully parsed manifest
             self.write_manifest_for_partial_parse()
 
         self.check_for_model_deprecations()
 
         return self.manifest
 
+    def safe_update_project_parser_files_partially(self, project_parser_files: Dict) -> Dict:
+        if self.saved_manifest is None:
+            return project_parser_files
+
+        self.partial_parser = PartialParsing(self.saved_manifest, self.manifest.files)  # type: ignore[arg-type]
+        self.skip_parsing = self.partial_parser.skip_parsing()
+        if self.skip_parsing:
+            # nothing changed, so we don't need to generate project_parser_files
+            self.manifest = self.saved_manifest  # type: ignore[assignment]
+        else:
+            # create child_map and parent_map
+            self.saved_manifest.build_parent_and_child_maps()  # type: ignore[union-attr]
+            # create group_map
+            self.saved_manifest.build_group_map()  # type: ignore[union-attr]
+            # files are different, we need to create a new set of
+            # project_parser_files.
+            try:
+                project_parser_files = self.partial_parser.get_parsing_files()
+                self.partially_parsing = True
+                self.manifest = self.saved_manifest  # type: ignore[assignment]
+            except Exception as exc:
+                # pp_files should still be the full set and manifest is new manifest,
+                # since get_parsing_files failed
+                fire_event(
+                    UnableToPartialParse(reason="an error occurred. Switching to full reparse.")
+                )
+
+                # Get traceback info
+                tb_info = traceback.format_exc()
+                # index last stack frame in traceback (i.e. lastest exception and its context)
+                tb_last_frame = traceback.extract_tb(exc.__traceback__)[-1]
+                exc_info = {
+                    "traceback": tb_info,
+                    "exception": tb_info.splitlines()[-1],
+                    "code": tb_last_frame.line,  # if the source is not available, it is None
+                    "location": f"line {tb_last_frame.lineno} in {tb_last_frame.name}",
+                }
+
+                # get file info for local logs
+                parse_file_type: str = ""
+                file_id = self.partial_parser.processing_file
+                if file_id:
+                    source_file = None
+                    if file_id in self.saved_manifest.files:
+                        source_file = self.saved_manifest.files[file_id]
+                    elif file_id in self.manifest.files:
+                        source_file = self.manifest.files[file_id]
+                    if source_file:
+                        parse_file_type = source_file.parse_file_type
+                        fire_event(PartialParsingErrorProcessingFile(file=file_id))
+                exc_info["parse_file_type"] = parse_file_type
+                fire_event(PartialParsingError(exc_info=exc_info))
+                # Send event
+                if dbt.tracking.active_user is not None:
+                    exc_info["full_reparse_reason"] = ReparseReason.exception
+                    dbt.tracking.track_partial_parser(exc_info)
+
+                if os.environ.get("DBT_PP_TEST"):
+                    raise exc
+
+        return project_parser_files
+
     def check_for_model_deprecations(self):
         for node in self.manifest.nodes.values():
             if isinstance(node, ModelNode):
                 if (
                     node.deprecation_date
                     and node.deprecation_date < datetime.datetime.now().astimezone()
                 ):
@@ -1614,25 +1621,25 @@
     if len(metric.type_params.input_measures) > 0:
         return
 
     if metric.type is MetricType.SIMPLE or metric.type is MetricType.CUMULATIVE:
         assert (
             metric.type_params.measure is not None
         ), f"{metric} should have a measure defined, but it does not."
-        metric.type_params.input_measures.append(metric.type_params.measure)
+        metric.add_input_measure(metric.type_params.measure)
         _process_metric_depends_on(
             manifest=manifest, current_project=current_project, metric=metric
         )
     elif metric.type is MetricType.CONVERSION:
         conversion_type_params = metric.type_params.conversion_type_params
         assert (
             conversion_type_params
         ), f"{metric.name} is a conversion metric and must have conversion_type_params defined."
-        metric.type_params.input_measures.append(conversion_type_params.base_measure)
-        metric.type_params.input_measures.append(conversion_type_params.conversion_measure)
+        metric.add_input_measure(conversion_type_params.base_measure)
+        metric.add_input_measure(conversion_type_params.conversion_measure)
         _process_metric_depends_on(
             manifest=manifest, current_project=current_project, metric=metric
         )
     elif metric.type is MetricType.DERIVED or metric.type is MetricType.RATIO:
         input_metrics = metric.input_metrics
         if metric.type is MetricType.RATIO:
             if metric.type_params.numerator is None or metric.type_params.denominator is None:
@@ -1660,15 +1667,16 @@
                     f"The metric `{input_metric.name}` is disabled and thus cannot be referenced.",
                     node=metric,
                 )
 
             _process_metric_node(
                 manifest=manifest, current_project=current_project, metric=target_metric
             )
-            metric.type_params.input_measures.extend(target_metric.type_params.input_measures)
+            for input_measure in target_metric.type_params.input_measures:
+                metric.add_input_measure(input_measure)
             metric.depends_on.add_node(target_metric.unique_id)
     else:
         assert_values_exhausted(metric.type)
 
 
 def _process_metrics_for_node(
     manifest: Manifest,
```

### Comparing `dbt-core-1.8.0b1/dbt/parser/models.py` & `dbt-core-1.8.0b2/dbt/parser/models.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.8.0b1/dbt/parser/partial.py` & `dbt-core-1.8.0b2/dbt/parser/partial.py`

 * *Files 0% similar despite different names*

```diff
@@ -207,14 +207,15 @@
         if project_name not in self.project_parser_files:
             self.project_parser_files[project_name] = {}
         if parser_name not in self.project_parser_files[project_name]:
             self.project_parser_files[project_name][parser_name] = []
         if (
             file_id not in self.project_parser_files[project_name][parser_name]
             and file_id not in self.file_diff["deleted"]
+            and file_id not in self.file_diff["deleted_schema_files"]
         ):
             self.project_parser_files[project_name][parser_name].append(file_id)
 
     def already_scheduled_for_parsing(self, source_file):
         file_id = source_file.file_id
         project_name = source_file.project_name
         if project_name not in self.project_parser_files:
@@ -463,15 +464,19 @@
                 unit_test = self.saved_manifest.unit_tests[unique_id]
                 self._schedule_for_parsing(
                     "unit_tests", unit_test, unit_test.name, self.delete_schema_unit_test
                 )
 
     def _schedule_for_parsing(self, dict_key: str, element, name, delete: Callable) -> None:
         file_id = element.file_id
-        if file_id in self.saved_files and file_id not in self.file_diff["deleted"]:
+        if (
+            file_id in self.saved_files
+            and file_id not in self.file_diff["deleted"]
+            and file_id not in self.file_diff["deleted_schema_files"]
+        ):
             schema_file = self.saved_files[file_id]
             elements = []
             assert isinstance(schema_file, SchemaSourceFile)
             if dict_key in schema_file.dict_from_yaml:
                 elements = schema_file.dict_from_yaml[dict_key]
             schema_element = self.get_schema_element(elements, name)
             if schema_element:
```

### Comparing `dbt-core-1.8.0b1/dbt/parser/read_files.py` & `dbt-core-1.8.0b2/dbt/parser/read_files.py`

 * *Files 0% similar despite different names*

```diff
@@ -77,15 +77,15 @@
             skip_loading_schema_file = True
 
     if not skip_loading_schema_file:
         # We strip the file_contents before generating the checksum because we want
         # the checksum to match the stored file contents
         file_contents = load_file_contents(path.absolute_path, strip=True)
         source_file.contents = file_contents
-        source_file.checksum = FileHash.from_contents(source_file.contents)
+        source_file.checksum = FileHash.from_contents(file_contents)
 
     if parse_file_type == ParseFileType.Schema and source_file.contents:
         dfy = yaml_from_file(source_file)
         if dfy:
             validate_yaml(source_file.path.original_file_path, dfy)
             source_file.dfy = dfy
     return source_file
```

### Comparing `dbt-core-1.8.0b1/dbt/parser/schema_generic_tests.py` & `dbt-core-1.8.0b2/dbt/parser/schema_generic_tests.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.8.0b1/dbt/parser/schema_renderer.py` & `dbt-core-1.8.0b2/dbt/parser/schema_renderer.py`

 * *Files 4% similar despite different names*

```diff
@@ -70,20 +70,21 @@
         elif self.key == "macros":
             if keypath[0] == "arguments":
                 if self._is_norender_key(keypath[1:]):
                     return False
             elif self._is_norender_key(keypath[0:]):
                 return False
         elif self.key == "metrics":
-            # This ensures all key paths that end in 'filter' for a metric are skipped
-            if keypath[-1] == "filter":
+            # This ensures that metric filters are skipped
+            if keypath[-1] == "filter" or len(keypath) > 1 and keypath[-2] == "filter":
                 return False
             elif self._is_norender_key(keypath[0:]):
                 return False
         elif self.key == "saved_queries":
+            # This ensures that saved query filters are skipped
             if keypath[0] == "query_params" and len(keypath) > 1 and keypath[1] == "where":
                 return False
             elif self._is_norender_key(keypath[0:]):
                 return False
         else:  # models, seeds, snapshots, analyses
             if self._is_norender_key(keypath[0:]):
                 return False
```

### Comparing `dbt-core-1.8.0b1/dbt/parser/schema_yaml_readers.py` & `dbt-core-1.8.0b2/dbt/parser/schema_yaml_readers.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.8.0b1/dbt/parser/schemas.py` & `dbt-core-1.8.0b2/dbt/parser/schemas.py`

 * *Files 2% similar despite different names*

```diff
@@ -893,18 +893,51 @@
                 c for c in constraints if "type" not in c or not ConstraintType.is_valid(c["type"])
             ):
                 raise ParsingError(
                     f"Invalid constraint type on model {node.name}: "
                     f"Type must be one of {[ct.value for ct in ConstraintType]}"
                 )
 
-            node.constraints = [ModelLevelConstraint.from_dict(c) for c in constraints]
+        self._validate_pk_constraints(node, constraints)
+        node.constraints = [ModelLevelConstraint.from_dict(c) for c in constraints]
 
-    def _validate_constraint_prerequisites(self, model_node: ModelNode):
+    def _validate_pk_constraints(self, model_node: ModelNode, constraints: List[Dict[str, Any]]):
+        errors = []
+        # check for primary key constraints defined at the column level
+        pk_col: List[str] = []
+        for col in model_node.columns.values():
+            for constraint in col.constraints:
+                if constraint.type == ConstraintType.primary_key:
+                    pk_col.append(col.name)
+
+        if len(pk_col) > 1:
+            errors.append(
+                f"Found {len(pk_col)} columns ({pk_col}) with primary key constraints defined. "
+                "Primary keys for multiple columns must be defined as a model level constraint."
+            )
+
+        if len(pk_col) > 0 and (
+            any(
+                constraint.type == ConstraintType.primary_key
+                for constraint in model_node.constraints
+            )
+            or any(constraint["type"] == ConstraintType.primary_key for constraint in constraints)
+        ):
+            errors.append(
+                "Primary key constraints defined at the model level and the columns level. "
+                "Primary keys can be defined at the model level or the column level, not both."
+            )
 
+        if errors:
+            raise ParsingError(
+                f"Primary key constraint error: ({model_node.original_file_path})\n"
+                + "\n".join(errors)
+            )
+
+    def _validate_constraint_prerequisites(self, model_node: ModelNode):
         column_warn_unsupported = [
             constraint.warn_unsupported
             for column in model_node.columns.values()
             for constraint in column.constraints
         ]
         model_warn_unsupported = [
             constraint.warn_unsupported for constraint in model_node.constraints
```

### Comparing `dbt-core-1.8.0b1/dbt/parser/search.py` & `dbt-core-1.8.0b2/dbt/parser/search.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.8.0b1/dbt/parser/seeds.py` & `dbt-core-1.8.0b2/dbt/parser/seeds.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.8.0b1/dbt/parser/singular_test.py` & `dbt-core-1.8.0b2/dbt/parser/singular_test.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.8.0b1/dbt/parser/snapshots.py` & `dbt-core-1.8.0b2/dbt/parser/snapshots.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.8.0b1/dbt/parser/sources.py` & `dbt-core-1.8.0b2/dbt/parser/sources.py`

 * *Files 2% similar despite different names*

```diff
@@ -128,22 +128,23 @@
     # This converts an UnpatchedSourceDefinition to a SourceDefinition
     def parse_source(self, target: UnpatchedSourceDefinition) -> SourceDefinition:
         source = target.source
         table = target.table
         refs = ParserRef.from_target(table)
         unique_id = target.unique_id
         description = table.description or ""
-        meta = table.meta or {}
         source_description = source.description or ""
         loaded_at_field = table.loaded_at_field or source.loaded_at_field
 
         freshness = merge_freshness(source.freshness, table.freshness)
         quoting = source.quoting.merged(table.quoting)
         # path = block.path.original_file_path
+        table_meta = table.meta or {}
         source_meta = source.meta or {}
+        meta = {**source_meta, **table_meta}
 
         # make sure we don't do duplicate tags from source + table
         tags = sorted(set(itertools.chain(source.tags, table.tags)))
 
         config = self._generate_source_config(
             target=target,
             rendered=True,
```

### Comparing `dbt-core-1.8.0b1/dbt/parser/sql.py` & `dbt-core-1.8.0b2/dbt/parser/sql.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.8.0b1/dbt/parser/unit_tests.py` & `dbt-core-1.8.0b2/dbt/parser/unit_tests.py`

 * *Files 4% similar despite different names*

```diff
@@ -116,57 +116,51 @@
         # always "ephemeral" they just wrap the tested_node SQL in additional CTEs. No actual table
         # or view is created.
         for given in test_case.given:
             # extract the original_input_node from the ref in the "input" key of the given list
             original_input_node = self._get_original_input_node(
                 given.input, tested_node, test_case.name
             )
+            input_name = original_input_node.name
 
             common_fields = {
                 "resource_type": NodeType.Model,
-                "original_file_path": original_input_node.original_file_path,
+                # root directory for input and output fixtures
+                "original_file_path": unit_test_node.original_file_path,
                 "config": ModelConfig(materialized="ephemeral"),
                 "database": original_input_node.database,
                 "alias": original_input_node.identifier,
                 "schema": original_input_node.schema,
                 "fqn": original_input_node.fqn,
                 "checksum": FileHash.empty(),
                 "raw_code": self._build_fixture_raw_code(given.rows, None),
+                "package_name": original_input_node.package_name,
+                "unique_id": f"model.{original_input_node.package_name}.{input_name}",
+                "name": input_name,
+                "path": f"{input_name}.sql",
             }
 
             if original_input_node.resource_type in (
                 NodeType.Model,
                 NodeType.Seed,
                 NodeType.Snapshot,
             ):
-                input_name = original_input_node.name
-                input_node = ModelNode(
-                    **common_fields,
-                    package_name=original_input_node.package_name,
-                    unique_id=f"model.{original_input_node.package_name}.{input_name}",
-                    name=input_name,
-                    path=original_input_node.path or f"{input_name}.sql",
-                )
+                input_node = ModelNode(**common_fields)
                 if (
                     original_input_node.resource_type == NodeType.Model
                     and original_input_node.version
                 ):
                     input_node.version = original_input_node.version
 
             elif original_input_node.resource_type == NodeType.Source:
                 # We are reusing the database/schema/identifier from the original source,
                 # but that shouldn't matter since this acts as an ephemeral model which just
                 # wraps a CTE around the unit test node.
-                input_name = original_input_node.name
                 input_node = UnitTestSourceDefinition(
                     **common_fields,
-                    package_name=original_input_node.package_name,
-                    unique_id=f"model.{original_input_node.package_name}.{input_name}",
-                    name=original_input_node.name,  # must be the same name for source lookup to work
-                    path=input_name + ".sql",  # for writing out compiled_code
                     source_name=original_input_node.source_name,  # needed for source lookup
                 )
                 # Sources need to go in the sources dictionary in order to create the right lookup
                 self.unit_test_manifest.sources[input_node.unique_id] = input_node  # type: ignore
 
             # Both ModelNode and UnitTestSourceDefinition need to go in nodes dictionary
             self.unit_test_manifest.nodes[input_node.unique_id] = input_node
@@ -416,15 +410,14 @@
 
 
 # This is called by the ManifestLoader after other processing has been done,
 # so that model versions are available.
 def process_models_for_unit_test(
     manifest: Manifest, current_project: str, unit_test_def: UnitTestDefinition, models_to_versions
 ):
-
     # If the unit tests doesn't have a depends_on.nodes[0] then we weren't able to resolve
     # the model, either because versions hadn't been processed yet, or it's not a valid model name
     if not unit_test_def.depends_on.nodes:
         tested_node = find_tested_model_node(manifest, current_project, unit_test_def.model)
         if not tested_node:
             raise ParsingError(
                 f"Unable to find model '{current_project}.{unit_test_def.model}' for "
@@ -434,14 +427,39 @@
         unit_test_def.schema = tested_node.schema
 
     # The UnitTestDefinition should only have one "depends_on" at this point,
     # the one that's found by the "model" field.
     target_model_id = unit_test_def.depends_on.nodes[0]
     target_model = manifest.nodes[target_model_id]
     assert isinstance(target_model, ModelNode)
+
+    target_model_is_incremental = "macro.dbt.is_incremental" in target_model.depends_on.macros
+    unit_test_def_has_incremental_override = unit_test_def.overrides and isinstance(
+        unit_test_def.overrides.macros.get("is_incremental"), bool
+    )
+
+    if target_model_is_incremental and (not unit_test_def_has_incremental_override):
+        raise ParsingError(
+            f"Boolean override for 'is_incremental' must be provided for unit test '{unit_test_def.name}' in model '{target_model.name}'"
+        )
+
+    unit_test_def_incremental_override_true = (
+        unit_test_def.overrides and unit_test_def.overrides.macros.get("is_incremental")
+    )
+    unit_test_def_has_this_input = "this" in [i.input for i in unit_test_def.given]
+
+    if (
+        target_model_is_incremental
+        and unit_test_def_incremental_override_true
+        and (not unit_test_def_has_this_input)
+    ):
+        raise ParsingError(
+            f"Unit test '{unit_test_def.name}' for incremental model '{target_model.name}' must have a 'this' input"
+        )
+
     # unit_test_versions = unit_test_def.versions
     # We're setting up unit tests for versioned models, so if
     # the model isn't versioned, we don't need to do anything
     if not target_model.is_versioned:
         if unit_test_def.versions and (
             unit_test_def.versions.include or unit_test_def.versions.exclude
         ):
```

### Comparing `dbt-core-1.8.0b1/dbt/plugins/__init__.py` & `dbt-core-1.8.0b2/dbt/plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.8.0b1/dbt/plugins/manager.py` & `dbt-core-1.8.0b2/dbt/plugins/manager.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.8.0b1/dbt/plugins/manifest.py` & `dbt-core-1.8.0b2/dbt/plugins/manifest.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.8.0b1/dbt/task/base.py` & `dbt-core-1.8.0b2/dbt/task/base.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,24 +2,25 @@
 import threading
 import time
 import traceback
 from abc import ABCMeta, abstractmethod
 from contextlib import nullcontext
 from datetime import datetime
 from pathlib import Path
-from typing import Any, Dict, List, Optional, Type, Union
+from typing import Any, Dict, List, Optional, Type, Union, Set
 
 from dbt.compilation import Compiler
 import dbt_common.exceptions.base
 import dbt.exceptions
 from dbt import tracking
 from dbt.config import RuntimeConfig, Project
 from dbt.config.profile import read_profile
 from dbt.constants import DBT_PROJECT_FILE_NAME
 from dbt.contracts.graph.manifest import Manifest
+from dbt.artifacts.resources.types import NodeType
 from dbt.artifacts.schemas.results import TimingInfo, collect_timing_info
 from dbt.artifacts.schemas.results import NodeStatus, RunningStatus, RunStatus
 from dbt.artifacts.schemas.run import RunResult
 from dbt_common.events.contextvars import get_node_info
 from dbt_common.events.functions import fire_event
 from dbt.events.types import (
     SkippingDetails,
@@ -202,14 +203,17 @@
 
         self.run_ephemeral_models = False
 
     @abstractmethod
     def compile(self, manifest: Manifest) -> Any:
         pass
 
+    def _node_build_path(self) -> Optional[str]:
+        return self.node.build_path if hasattr(self.node, "build_path") else None
+
     def get_result_status(self, result) -> Dict[str, str]:
         if result.status == NodeStatus.Error:
             return {"node_status": "error", "node_error": str(result.message)}
         elif result.status == NodeStatus.Skipped:
             return {"node_status": "skipped"}
         elif result.status == NodeStatus.Fail:
             return {"node_status": "failed"}
@@ -334,23 +338,23 @@
             )
         )
         return str(e)
 
     def _handle_internal_exception(self, e, ctx):
         fire_event(
             InternalErrorOnRun(
-                build_path=self.node.build_path, exc=str(e), node_info=get_node_info()
+                build_path=self._node_build_path(), exc=str(e), node_info=get_node_info()
             )
         )
         return str(e)
 
     def _handle_generic_exception(self, e, ctx):
         fire_event(
             GenericExceptionOnRun(
-                build_path=self.node.build_path,
+                build_path=self._node_build_path(),
                 unique_id=self.node.unique_id,
                 exc=str(e),
                 node_info=get_node_info(),
             )
         )
         fire_event(LogDebugStackTrace(exc_info=traceback.format_exc()))
 
@@ -476,7 +480,34 @@
 
         node_result = RunResult.from_node(self.node, RunStatus.Skipped, error_message)
         return node_result
 
     def do_skip(self, cause=None):
         self.skip = True
         self.skip_cause = cause
+
+
+def resource_types_from_args(
+    args, all_resource_values: Set[NodeType], default_resource_values: Set[NodeType]
+) -> Set[NodeType]:
+
+    if not args.resource_types:
+        resource_types = default_resource_values
+    else:
+        # This is a list of strings, not NodeTypes
+        arg_resource_types = set(args.resource_types)
+
+        if "all" in arg_resource_types:
+            arg_resource_types.remove("all")
+            arg_resource_types.update(all_resource_values)
+        if "default" in arg_resource_types:
+            arg_resource_types.remove("default")
+            arg_resource_types.update(default_resource_values)
+        # Convert to a set of NodeTypes now that the non-NodeType strings are gone
+        resource_types = set([NodeType(rt) for rt in list(arg_resource_types)])
+
+    if args.exclude_resource_types:
+        # Convert from a list of strings to a set of NodeTypes
+        exclude_resource_types = set([NodeType(rt) for rt in args.exclude_resource_types])
+        resource_types = resource_types - exclude_resource_types
+
+    return resource_types
```

### Comparing `dbt-core-1.8.0b1/dbt/task/build.py` & `dbt-core-1.8.0b2/dbt/task/build.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from .test import TestRunner as test_runner
 
 from dbt.artifacts.schemas.results import NodeStatus, RunStatus
 from dbt.artifacts.schemas.run import RunResult
 from dbt.graph import ResourceTypeSelector, GraphQueue, Graph
 from dbt.node_types import NodeType
 from dbt.task.test import TestSelector
-from dbt.task.base import BaseRunner
+from dbt.task.base import BaseRunner, resource_types_from_args
 from dbt_common.events.functions import fire_event
 from dbt.events.types import LogNodeNoOpResult
 from dbt.exceptions import DbtInternalError
 
 
 class SavedQueryRunner(BaseRunner):
     # Stub. No-op Runner for Saved Queries, which require MetricFlow for execution.
@@ -76,22 +76,17 @@
 
     def __init__(self, args, config, manifest) -> None:
         super().__init__(args, config, manifest)
         self.selected_unit_tests: Set = set()
         self.model_to_unit_test_map: Dict[str, List] = {}
 
     def resource_types(self, no_unit_tests=False):
-        if not self.args.resource_types:
-            resource_types = list(self.ALL_RESOURCE_VALUES)
-        else:
-            resource_types = set(self.args.resource_types)
-
-            if "all" in resource_types:
-                resource_types.remove("all")
-                resource_types.update(self.ALL_RESOURCE_VALUES)
+        resource_types = resource_types_from_args(
+            self.args, set(self.ALL_RESOURCE_VALUES), set(self.ALL_RESOURCE_VALUES)
+        )
 
         # First we get selected_nodes including unit tests, then without,
         # and do a set difference.
         if no_unit_tests is True and NodeType.Unit in resource_types:
             resource_types.remove(NodeType.Unit)
         return list(resource_types)
```

### Comparing `dbt-core-1.8.0b1/dbt/task/clean.py` & `dbt-core-1.8.0b2/dbt/task/clean.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.8.0b1/dbt/task/clone.py` & `dbt-core-1.8.0b2/dbt/task/clone.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,16 +5,16 @@
 from dbt.clients.jinja import MacroGenerator
 from dbt.context.providers import generate_runtime_model_context
 from dbt.contracts.graph.manifest import Manifest
 from dbt.artifacts.schemas.run import RunStatus, RunResult
 from dbt_common.dataclass_schema import dbtClassMixin
 from dbt_common.exceptions import DbtInternalError, CompilationError
 from dbt.graph import ResourceTypeSelector
-from dbt.node_types import NodeType, REFABLE_NODE_TYPES
-from dbt.task.base import BaseRunner
+from dbt.node_types import REFABLE_NODE_TYPES
+from dbt.task.base import BaseRunner, resource_types_from_args
 from dbt.task.run import _validate_materialization_relations_dict
 from dbt.task.runnable import GraphRunnableTask
 
 
 class CloneRunner(BaseRunner):
     def before_execute(self):
         pass
@@ -128,26 +128,21 @@
             schemas_to_create = super().get_model_schemas(adapter, selected_uids)
             self.create_schemas(adapter, schemas_to_create)
             schemas_to_cache = self.get_model_schemas(adapter, selected_uids)
             self.populate_adapter_cache(adapter, schemas_to_cache)
 
     @property
     def resource_types(self):
-        if not self.args.resource_types:
-            return REFABLE_NODE_TYPES
-
-        values = set(self.args.resource_types)
-
-        if "all" in values:
-            values.remove("all")
-            values.update(REFABLE_NODE_TYPES)
-
-        values = [NodeType(val) for val in values if val in REFABLE_NODE_TYPES]
+        resource_types = resource_types_from_args(
+            self.args, set(REFABLE_NODE_TYPES), set(REFABLE_NODE_TYPES)
+        )
 
-        return list(values)
+        # filter out any non-refable node types
+        resource_types = [rt for rt in resource_types if rt in REFABLE_NODE_TYPES]
+        return list(resource_types)
 
     def get_node_selector(self) -> ResourceTypeSelector:
         resource_types = self.resource_types
 
         if self.manifest is None or self.graph is None:
             raise DbtInternalError("manifest and graph must be set to get perform node selection")
         return ResourceTypeSelector(
```

### Comparing `dbt-core-1.8.0b1/dbt/task/compile.py` & `dbt-core-1.8.0b2/dbt/task/compile.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.8.0b1/dbt/task/debug.py` & `dbt-core-1.8.0b2/dbt/task/debug.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.8.0b1/dbt/task/deps.py` & `dbt-core-1.8.0b2/dbt/task/deps.py`

 * *Files 0% similar despite different names*

```diff
@@ -197,15 +197,15 @@
         for package in resolved_deps:
             packages_installed["packages"].append(package.to_dict())
         packages_installed[PACKAGE_LOCK_HASH_KEY] = _create_sha1_hash(
             self.project.packages.packages
         )
 
         with open(lock_filepath, "w") as lock_obj:
-            yaml.safe_dump(packages_installed, lock_obj)
+            yaml.dump(packages_installed, lock_obj, Dumper=dbtPackageDumper)
 
         fire_event(DepsLockUpdating(lock_filepath=lock_filepath))
 
     def run(self) -> None:
         if self.args.add_package:
             self.add()
```

### Comparing `dbt-core-1.8.0b1/dbt/task/docs/generate.py` & `dbt-core-1.8.0b2/dbt/task/docs/generate.py`

 * *Files 0% similar despite different names*

```diff
@@ -279,15 +279,16 @@
 
                 # This generates the catalog as an agate.Table
                 catalogable_nodes = chain(
                     [
                         node
                         for node in self.manifest.nodes.values()
                         if (node.is_relational and not node.is_ephemeral_model)
-                    ]
+                    ],
+                    self.manifest.sources.values(),
                 )
                 used_schemas = self.manifest.get_used_schemas()
                 catalog_table, exceptions = adapter.get_filtered_catalog(
                     catalogable_nodes, used_schemas, relations
                 )
 
         catalog_data: List[PrimitiveDict] = [
```

### Comparing `dbt-core-1.8.0b1/dbt/task/docs/serve.py` & `dbt-core-1.8.0b2/dbt/task/docs/serve.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.8.0b1/dbt/task/freshness.py` & `dbt-core-1.8.0b2/dbt/task/freshness.py`

 * *Files 2% similar despite different names*

```diff
@@ -116,29 +116,28 @@
                 )
 
                 status = compiled_node.freshness.status(freshness["age"])
             elif self.adapter.supports(Capability.TableLastModifiedMetadata):
                 if compiled_node.freshness.filter is not None:
                     fire_event(
                         Note(
-                            f"A filter cannot be applied to a metadata freshness check on source '{compiled_node.name}'.",
-                            EventLevel.WARN,
-                        )
+                            msg=f"A filter cannot be applied to a metadata freshness check on source '{compiled_node.name}'."
+                        ),
+                        EventLevel.WARN,
                     )
 
                 adapter_response, freshness = self.adapter.calculate_freshness_from_metadata(
                     relation,
                     macro_resolver=manifest,
                 )
 
                 status = compiled_node.freshness.status(freshness["age"])
             else:
-                status = FreshnessStatus.Warn
-                fire_event(
-                    Note(f"Skipping freshness for source {compiled_node.name}."),
+                raise DbtRuntimeError(
+                    f"Could not compute freshness for source {compiled_node.name}: no 'loaded_at_field' provided and {self.adapter.type()} adapter does not support metadata-based freshness checks."
                 )
 
         # adapter_response was not returned in previous versions, so this will be None
         # we cannot call to_dict() on NoneType
         if adapter_response:
             adapter_response = adapter_response.to_dict(omit_none=True)
```

### Comparing `dbt-core-1.8.0b1/dbt/task/init.py` & `dbt-core-1.8.0b2/dbt/task/init.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.8.0b1/dbt/task/list.py` & `dbt-core-1.8.0b2/dbt/task/list.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 import json
 
 from dbt.contracts.graph.nodes import (
     Exposure,
     SourceDefinition,
     Metric,
+    SavedQuery,
     SemanticModel,
     UnitTestDefinition,
 )
 from dbt.flags import get_flags
 from dbt.graph import ResourceTypeSelector
+from dbt.task.base import resource_types_from_args
 from dbt.task.runnable import GraphRunnableTask
 from dbt.task.test import TestSelector
 from dbt.node_types import NodeType
 from dbt_common.events.functions import (
     fire_event,
     warn_or_error,
 )
@@ -27,14 +29,15 @@
             NodeType.Model,
             NodeType.Snapshot,
             NodeType.Seed,
             NodeType.Test,
             NodeType.Source,
             NodeType.Exposure,
             NodeType.Metric,
+            NodeType.SavedQuery,
             NodeType.SemanticModel,
             NodeType.Unit,
         )
     )
     ALL_RESOURCE_VALUES = DEFAULT_RESOURCE_VALUES | frozenset((NodeType.Analysis,))
     ALLOWED_KEYS = frozenset(
         (
@@ -79,18 +82,20 @@
                 yield self.manifest.exposures[unique_id]
             elif unique_id in self.manifest.metrics:
                 yield self.manifest.metrics[unique_id]
             elif unique_id in self.manifest.semantic_models:
                 yield self.manifest.semantic_models[unique_id]
             elif unique_id in self.manifest.unit_tests:
                 yield self.manifest.unit_tests[unique_id]
+            elif unique_id in self.manifest.saved_queries:
+                yield self.manifest.saved_queries[unique_id]
             else:
                 raise DbtRuntimeError(
                     f'Got an unexpected result from node selection: "{unique_id}"'
-                    f"Expected a source or a node!"
+                    f"Listing this node type is not yet supported!"
                 )
 
     def generate_selectors(self):
         for node in self._iterate_selected_nodes():
             if node.resource_type == NodeType.Source:
                 assert isinstance(node, SourceDefinition)
                 # sources are searched for by pkg.source_name.table_name
@@ -102,14 +107,18 @@
                 exposure_selector = ".".join([node.package_name, node.name])
                 yield f"exposure:{exposure_selector}"
             elif node.resource_type == NodeType.Metric:
                 assert isinstance(node, Metric)
                 # metrics are searched for by pkg.metric_name
                 metric_selector = ".".join([node.package_name, node.name])
                 yield f"metric:{metric_selector}"
+            elif node.resource_type == NodeType.SavedQuery:
+                assert isinstance(node, SavedQuery)
+                saved_query_selector = ".".join([node.package_name, node.name])
+                yield f"saved_query:{saved_query_selector}"
             elif node.resource_type == NodeType.SemanticModel:
                 assert isinstance(node, SemanticModel)
                 semantic_model_selector = ".".join([node.package_name, node.name])
                 yield f"semantic_model:{semantic_model_selector}"
             elif node.resource_type == NodeType.Unit:
                 assert isinstance(node, UnitTestDefinition)
                 unit_test_selector = ".".join([node.package_name, node.versioned_name])
@@ -171,25 +180,19 @@
         return self.node_results
 
     @property
     def resource_types(self):
         if self.args.models:
             return [NodeType.Model]
 
-        if not self.args.resource_types:
-            return list(self.DEFAULT_RESOURCE_VALUES)
+        resource_types = resource_types_from_args(
+            self.args, set(self.ALL_RESOURCE_VALUES), set(self.DEFAULT_RESOURCE_VALUES)
+        )
 
-        values = set(self.args.resource_types)
-        if "default" in values:
-            values.remove("default")
-            values.update(self.DEFAULT_RESOURCE_VALUES)
-        if "all" in values:
-            values.remove("all")
-            values.update(self.ALL_RESOURCE_VALUES)
-        return list(values)
+        return list(resource_types)
 
     @property
     def selection_arg(self):
         # for backwards compatibility, list accepts both --models and --select,
         # with slightly different behavior: --models implies --resource-type model
         if self.args.models:
             return self.args.models
```

### Comparing `dbt-core-1.8.0b1/dbt/task/printer.py` & `dbt-core-1.8.0b2/dbt/task/printer.py`

 * *Files 18% similar despite different names*

```diff
@@ -75,52 +75,60 @@
 
 
 def print_run_result_error(result, newline: bool = True, is_warning: bool = False) -> None:
     if newline:
         with TextOnly():
             fire_event(Formatting(""))
 
+    # set node_info for logging events
+    node_info = None
+    if hasattr(result, "node") and result.node:
+        node_info = result.node.node_info
     if result.status == NodeStatus.Fail or (is_warning and result.status == NodeStatus.Warn):
         if is_warning:
             fire_event(
                 RunResultWarning(
                     resource_type=result.node.resource_type,
                     node_name=result.node.name,
                     path=result.node.original_file_path,
+                    node_info=node_info,
                 )
             )
         else:
             fire_event(
                 RunResultFailure(
                     resource_type=result.node.resource_type,
                     node_name=result.node.name,
                     path=result.node.original_file_path,
+                    node_info=node_info,
                 )
             )
 
         if result.message:
             if is_warning:
-                fire_event(RunResultWarningMessage(msg=result.message))
+                fire_event(RunResultWarningMessage(msg=result.message, node_info=node_info))
             else:
-                fire_event(RunResultError(msg=result.message))
+                fire_event(RunResultError(msg=result.message, node_info=node_info))
         else:
-            fire_event(RunResultErrorNoMessage(status=result.status))
+            fire_event(RunResultErrorNoMessage(status=result.status, node_info=node_info))
 
-        if result.node.build_path is not None:
+        if result.node.compiled_path is not None:
             with TextOnly():
                 fire_event(Formatting(""))
-            fire_event(SQLCompiledPath(path=result.node.compiled_path))
+            fire_event(SQLCompiledPath(path=result.node.compiled_path, node_info=node_info))
 
         if result.node.should_store_failures:
             with TextOnly():
                 fire_event(Formatting(""))
-            fire_event(CheckNodeTestFailure(relation_name=result.node.relation_name))
+            fire_event(
+                CheckNodeTestFailure(relation_name=result.node.relation_name, node_info=node_info)
+            )
 
     elif result.message is not None:
-        fire_event(RunResultError(msg=result.message))
+        fire_event(RunResultError(msg=result.message, node_info=node_info))
 
 
 def print_run_end_messages(results, keyboard_interrupt: bool = False) -> None:
     errors, warnings = [], []
     for r in results:
         if r.status in (NodeStatus.RuntimeErr, NodeStatus.Error, NodeStatus.Fail):
             errors.append(r)
```

### Comparing `dbt-core-1.8.0b1/dbt/task/retry.py` & `dbt-core-1.8.0b2/dbt/task/retry.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.8.0b1/dbt/task/run.py` & `dbt-core-1.8.0b2/dbt/task/run.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.8.0b1/dbt/task/run_operation.py` & `dbt-core-1.8.0b2/dbt/task/run_operation.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 import os
 import threading
 import traceback
 from datetime import datetime
-
-import agate
+from typing import TYPE_CHECKING
 
 import dbt_common.exceptions
 from dbt.adapters.factory import get_adapter
 from dbt.contracts.files import FileHash
 from dbt.contracts.graph.nodes import HookNode
 from dbt.artifacts.schemas.results import RunStatus, TimingInfo
 from dbt.artifacts.schemas.run import RunResultsArtifact, RunResult
@@ -20,25 +19,29 @@
 from dbt_common.exceptions import DbtInternalError
 from dbt.node_types import NodeType
 from dbt.task.base import ConfiguredTask
 
 RESULT_FILE_NAME = "run_results.json"
 
 
+if TYPE_CHECKING:
+    import agate
+
+
 class RunOperationTask(ConfiguredTask):
     def _get_macro_parts(self):
         macro_name = self.args.macro
         if "." in macro_name:
             package_name, macro_name = macro_name.split(".", 1)
         else:
             package_name = None
 
         return package_name, macro_name
 
-    def _run_unsafe(self, package_name, macro_name) -> agate.Table:
+    def _run_unsafe(self, package_name, macro_name) -> "agate.Table":
         adapter = get_adapter(self.config)
 
         macro_kwargs = self.args.args
 
         with adapter.connection_named("macro_{}".format(macro_name)):
             adapter.clear_transaction()
             res = adapter.execute_macro(
```

### Comparing `dbt-core-1.8.0b1/dbt/task/runnable.py` & `dbt-core-1.8.0b2/dbt/task/runnable.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,14 +28,15 @@
     DefaultSelector,
     NodeStart,
     NodeFinished,
     QueryCancelationUnsupported,
     ConcurrencyLine,
     EndRunResult,
     NothingToDo,
+    GenericExceptionOnRun,
 )
 from dbt.exceptions import (
     DbtInternalError,
     DbtRuntimeError,
     FailFastError,
 )
 from dbt_common.exceptions import NotImplementedError
@@ -46,15 +47,14 @@
     TextOnly,
     UniqueID,
     TimestampNamed,
     DbtModelState,
     ModelMetadata,
     NodeCount,
 )
-from dbt.node_types import NodeType
 from dbt.parser.manifest import write_manifest
 from dbt.task.base import ConfiguredTask, BaseRunner
 from .printer import (
     print_run_result_error,
     print_run_end_messages,
 )
 
@@ -217,31 +217,55 @@
             with startctx, extended_metadata:
                 fire_event(
                     NodeStart(
                         node_info=runner.node.node_info,
                     )
                 )
             status: Dict[str, str] = {}
+            result = None
+            thread_exception = None
             try:
                 result = runner.run_with_hooks(self.manifest)
-            except Exception as exc:
-                raise DbtInternalError(f"Unable to execute node: {exc}")
+            except Exception as e:
+                thread_exception = e
             finally:
                 finishctx = TimestampNamed("finished_at")
                 with finishctx, DbtModelState(status):
-                    fire_event(
-                        NodeFinished(
-                            node_info=runner.node.node_info,
-                            run_result=result.to_msg_dict(),
+                    if result is not None:
+                        fire_event(
+                            NodeFinished(
+                                node_info=runner.node.node_info,
+                                run_result=result.to_msg_dict(),
+                            )
                         )
-                    )
+                    else:
+                        msg = f"Exception on worker thread. {thread_exception}"
+
+                        fire_event(
+                            GenericExceptionOnRun(
+                                unique_id=runner.node.unique_id,
+                                exc=str(thread_exception),
+                                node_info=runner.node.node_info,
+                            )
+                        )
+
+                        result = RunResult(
+                            status=RunStatus.Error,  # type: ignore
+                            timing=[],
+                            thread_id="",
+                            execution_time=0.0,
+                            adapter_response={},
+                            message=msg,
+                            failures=None,
+                            node=runner.node,
+                        )
+
             # `_event_status` dict is only used for logging.  Make sure
-            # it gets deleted when we're done with it, except for unit tests
-            if not runner.node.resource_type == NodeType.Unit:
-                runner.node.clear_event_status()
+            # it gets deleted when we're done with it
+            runner.node.clear_event_status()
 
         fail_fast = get_flags().FAIL_FAST
 
         if result.status in (NodeStatus.Error, NodeStatus.Fail) and fail_fast:
             self._raise_next_tick = FailFastError(
                 msg="Failing early due to test failure or runtime error",
                 result=result,
@@ -647,12 +671,12 @@
         state = self.previous_defer_state or self.previous_state
         if not state:
             raise DbtRuntimeError(
                 "--state or --defer-state are required for deferral, but neither was provided"
             )
 
         if not state.manifest:
-            raise DbtRuntimeError(f'Could not find manifest in --state path: "{state}"')
+            raise DbtRuntimeError(f'Could not find manifest in --state path: "{state.state_path}"')
         return state.manifest
 
     def _get_deferred_manifest(self) -> Optional[Manifest]:
         return self._get_previous_state() if self.args.defer else None
```

### Comparing `dbt-core-1.8.0b1/dbt/task/seed.py` & `dbt-core-1.8.0b2/dbt/task/seed.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.8.0b1/dbt/task/show.py` & `dbt-core-1.8.0b2/dbt/task/show.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.8.0b1/dbt/task/snapshot.py` & `dbt-core-1.8.0b2/dbt/task/snapshot.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.8.0b1/dbt/task/sql.py` & `dbt-core-1.8.0b2/dbt/task/sql.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.8.0b1/dbt/task/test.py` & `dbt-core-1.8.0b2/dbt/task/test.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,28 @@
-import agate
 import daff
 import io
 import json
 import re
 from dataclasses import dataclass
 from dbt.utils import _coerce_decimal, strtobool
 from dbt_common.events.format import pluralize
 from dbt_common.dataclass_schema import dbtClassMixin
 import threading
-from typing import Dict, Any, Optional, Union, List
+from typing import Dict, Any, Optional, Union, List, TYPE_CHECKING, Tuple
 
 from .compile import CompileRunner
 from .run import RunTask
 
-from dbt.contracts.graph.nodes import TestNode, UnitTestDefinition, UnitTestNode
+from dbt.contracts.graph.nodes import (
+    TestNode,
+    UnitTestDefinition,
+    UnitTestNode,
+    GenericTestNode,
+    SingularTestNode,
+)
 from dbt.contracts.graph.manifest import Manifest
 from dbt.artifacts.schemas.results import TestStatus
 from dbt.artifacts.schemas.run import RunResult
 from dbt.artifacts.schemas.catalog import PrimitiveDict
 from dbt.context.providers import generate_runtime_model_context
 from dbt.clients.jinja import MacroGenerator
 from dbt_common.events.functions import fire_event
@@ -33,14 +38,18 @@
 )
 from dbt.node_types import NodeType
 from dbt.parser.unit_tests import UnitTestManifestLoader
 from dbt.flags import get_flags
 from dbt_common.ui import green, red
 
 
+if TYPE_CHECKING:
+    import agate
+
+
 @dataclass
 class UnitTestDiff(dbtClassMixin):
     actual: List[Dict[str, Any]]
     expected: List[Dict[str, Any]]
     rendered: str
 
 
@@ -173,24 +182,25 @@
     ) -> Manifest:
         # build a unit test manifest with only the test from this UnitTestDefinition
         loader = UnitTestManifestLoader(manifest, self.config, {unit_test_def.unique_id})
         return loader.load()
 
     def execute_unit_test(
         self, unit_test_def: UnitTestDefinition, manifest: Manifest
-    ) -> UnitTestResultData:
+    ) -> Tuple[UnitTestNode, UnitTestResultData]:
 
         unit_test_manifest = self.build_unit_test_manifest_from_test(unit_test_def, manifest)
 
         # The unit test node and definition have the same unique_id
         unit_test_node = unit_test_manifest.nodes[unit_test_def.unique_id]
         assert isinstance(unit_test_node, UnitTestNode)
 
         # Compile the node
         unit_test_node = self.compiler.compile_node(unit_test_node, unit_test_manifest, {})
+        assert isinstance(unit_test_node, UnitTestNode)
 
         # generate_runtime_unit_test_context not strictly needed - this is to run the 'unit'
         # materialization, not compile the node.compiled_code
         context = generate_runtime_model_context(unit_test_node, self.config, unit_test_manifest)
 
         materialization_macro = unit_test_manifest.find_materialization_macro_by_name(
             self.config.project_name, unit_test_node.get_materialization(), self.adapter.type()
@@ -236,26 +246,29 @@
 
             diff = UnitTestDiff(
                 actual=json_rows_from_table(actual),
                 expected=json_rows_from_table(expected),
                 rendered=rendered,
             )
 
-        return UnitTestResultData(
+        unit_test_result_data = UnitTestResultData(
             diff=diff,
             should_error=should_error,
             adapter_response=adapter_response,
         )
 
-    def execute(self, test: Union[TestNode, UnitTestDefinition], manifest: Manifest):
+        return unit_test_node, unit_test_result_data
+
+    def execute(self, test: Union[TestNode, UnitTestNode], manifest: Manifest):
         if isinstance(test, UnitTestDefinition):
-            unit_test_result = self.execute_unit_test(test, manifest)
-            return self.build_unit_test_run_result(test, unit_test_result)
+            unit_test_node, unit_test_result = self.execute_unit_test(test, manifest)
+            return self.build_unit_test_run_result(unit_test_node, unit_test_result)
         else:
             # Note: manifest here is a normal manifest
+            assert isinstance(test, (SingularTestNode, GenericTestNode))
             test_result = self.execute_data_test(test, manifest)
             return self.build_test_run_result(test, test_result)
 
     def build_test_run_result(self, test: TestNode, result: TestResultData) -> RunResult:
         severity = test.config.severity.upper()
         thread_id = threading.current_thread().name
         num_errors = pluralize(result.failures, "result")
@@ -286,28 +299,28 @@
             message=message,
             adapter_response=result.adapter_response,
             failures=failures,
         )
         return run_result
 
     def build_unit_test_run_result(
-        self, test: UnitTestDefinition, result: UnitTestResultData
+        self, test: UnitTestNode, result: UnitTestResultData
     ) -> RunResult:
         thread_id = threading.current_thread().name
 
         status = TestStatus.Pass
         message = None
         failures = 0
         if result.should_error:
             status = TestStatus.Fail
             message = result.diff.rendered if result.diff else None
             failures = 1
 
         return RunResult(
-            node=test,  # type: ignore
+            node=test,
             status=status,
             timing=[],
             thread_id=thread_id,
             execution_time=0,
             message=message,
             adapter_response=result.adapter_response,
             failures=failures,
@@ -321,15 +334,15 @@
             lambda row: row["actual_or_expected"] == actual_or_expected
         )
         columns = list(unit_test_table.columns.keys())
         columns.remove("actual_or_expected")
         return unit_test_table.select(columns)
 
     def _get_daff_diff(
-        self, expected: agate.Table, actual: agate.Table, ordered: bool = False
+        self, expected: "agate.Table", actual: "agate.Table", ordered: bool = False
     ) -> daff.TableDiff:
 
         expected_daff_table = daff.PythonTableView(list_rows_from_table(expected))
         actual_daff_table = daff.PythonTableView(list_rows_from_table(actual))
 
         alignment = daff.Coopy.compareTables(expected_daff_table, actual_daff_table).align()
         result = daff.PythonTableView([])
@@ -384,23 +397,23 @@
         )
 
     def get_runner_type(self, _):
         return TestRunner
 
 
 # This was originally in agate_helper, but that was moved out into dbt_common
-def json_rows_from_table(table: agate.Table) -> List[Dict[str, Any]]:
+def json_rows_from_table(table: "agate.Table") -> List[Dict[str, Any]]:
     "Convert a table to a list of row dict objects"
     output = io.StringIO()
     table.to_json(path=output)  # type: ignore
 
     return json.loads(output.getvalue())
 
 
 # This was originally in agate_helper, but that was moved out into dbt_common
-def list_rows_from_table(table: agate.Table) -> List[Any]:
+def list_rows_from_table(table: "agate.Table") -> List[Any]:
     "Convert a table to a list of lists, where the first element represents the header"
     rows = [[col.name for col in table.columns]]
     for row in table.rows:
         rows.append(list(row.values()))
 
     return rows
```

### Comparing `dbt-core-1.8.0b1/dbt/tests/fixtures/project.py` & `dbt-core-1.8.0b2/dbt/tests/fixtures/project.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.8.0b1/dbt/tests/util.py` & `dbt-core-1.8.0b2/dbt/tests/util.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.8.0b1/dbt/tracking.py` & `dbt-core-1.8.0b2/dbt/tracking.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.8.0b1/dbt/utils.py` & `dbt-core-1.8.0b2/dbt/utils.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.8.0b1/dbt/version.py` & `dbt-core-1.8.0b2/dbt/version.py`

 * *Files 0% similar despite different names*

```diff
@@ -225,9 +225,9 @@
             # the path is like .../dbt/adapters/{plugin_name}/__version__.py
             # except it could be \\ on windows!
             plugin_root, _ = os.path.split(version_path)
             _, plugin_name = os.path.split(plugin_root)
             yield plugin_name
 
 
-__version__ = "1.8.0b1"
+__version__ = "1.8.0b2"
 installed = get_installed_version()
```

### Comparing `dbt-core-1.8.0b1/dbt_core.egg-info/PKG-INFO` & `dbt-core-1.8.0b2/dbt_core.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbt-core
-Version: 1.8.0b1
+Version: 1.8.0b2
 Summary: With dbt, data analysts and engineers can build analytics the way engineers build applications.
 Home-page: https://github.com/dbt-labs/dbt-core
 Author: dbt Labs
 Author-email: info@dbtlabs.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: Microsoft :: Windows
@@ -19,24 +19,24 @@
 Description-Content-Type: text/markdown
 Requires-Dist: agate<1.8,>=1.7.0
 Requires-Dist: Jinja2<4,>=3.1.3
 Requires-Dist: mashumaro[msgpack]<4.0,>=3.9
 Requires-Dist: logbook<1.6,>=1.5
 Requires-Dist: click<9.0,>=8.0.2
 Requires-Dist: networkx<4.0,>=2.3
+Requires-Dist: protobuf<5,>=4.0.0
 Requires-Dist: requests<3.0.0
 Requires-Dist: pathspec<0.12,>=0.9
 Requires-Dist: sqlparse<0.5,>=0.2.3
 Requires-Dist: dbt-extractor<=0.6,>=0.5.0
 Requires-Dist: minimal-snowplow-tracker<0.1,>=0.0.2
-Requires-Dist: dbt-semantic-interfaces<0.6,>=0.5.0a2
+Requires-Dist: dbt-semantic-interfaces<0.6,>=0.5.1
 Requires-Dist: dbt-common<2.0
 Requires-Dist: dbt-adapters<2.0,>=0.1.0a2
 Requires-Dist: packaging>20.9
-Requires-Dist: protobuf>=4.0.0
 Requires-Dist: pytz>=2015.7
 Requires-Dist: pyyaml>=6.0
 Requires-Dist: daff>=1.3.46
 Requires-Dist: typing-extensions>=4.4
 
 <p align="center">
   <img src="https://raw.githubusercontent.com/dbt-labs/dbt-core/fa1ea14ddfb1d5ae319d5141844910dd53ab2834/etc/dbt-core.svg" alt="dbt logo" width="750"/>
```

#### html2text {}

```diff
@@ -1,28 +1,28 @@
-Metadata-Version: 2.1 Name: dbt-core Version: 1.8.0b1 Summary: With dbt, data
+Metadata-Version: 2.1 Name: dbt-core Version: 1.8.0b2 Summary: With dbt, data
 analysts and engineers can build analytics the way engineers build
 applications. Home-page: https://github.com/dbt-labs/dbt-core Author: dbt Labs
 Author-email: info@dbtlabs.com Classifier: Development Status :: 5 -
 Production/Stable Classifier: License :: OSI Approved :: Apache Software
 License Classifier: Operating System :: Microsoft :: Windows Classifier:
 Operating System :: MacOS :: MacOS X Classifier: Operating System :: POSIX ::
 Linux Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
 Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11 Classifier: Programming
 Language :: Python :: 3.12 Requires-Python: >=3.8 Description-Content-Type:
 text/markdown Requires-Dist: agate<1.8,>=1.7.0 Requires-Dist: Jinja2<4,>=3.1.3
 Requires-Dist: mashumaro[msgpack]<4.0,>=3.9 Requires-Dist: logbook<1.6,>=1.5
 Requires-Dist: click<9.0,>=8.0.2 Requires-Dist: networkx<4.0,>=2.3 Requires-
-Dist: requests<3.0.0 Requires-Dist: pathspec<0.12,>=0.9 Requires-Dist:
-sqlparse<0.5,>=0.2.3 Requires-Dist: dbt-extractor<=0.6,>=0.5.0 Requires-Dist:
-minimal-snowplow-tracker<0.1,>=0.0.2 Requires-Dist: dbt-semantic-
-interfaces<0.6,>=0.5.0a2 Requires-Dist: dbt-common<2.0 Requires-Dist: dbt-
-adapters<2.0,>=0.1.0a2 Requires-Dist: packaging>20.9 Requires-Dist:
-protobuf>=4.0.0 Requires-Dist: pytz>=2015.7 Requires-Dist: pyyaml>=6.0
-Requires-Dist: daff>=1.3.46 Requires-Dist: typing-extensions>=4.4
+Dist: protobuf<5,>=4.0.0 Requires-Dist: requests<3.0.0 Requires-Dist:
+pathspec<0.12,>=0.9 Requires-Dist: sqlparse<0.5,>=0.2.3 Requires-Dist: dbt-
+extractor<=0.6,>=0.5.0 Requires-Dist: minimal-snowplow-tracker<0.1,>=0.0.2
+Requires-Dist: dbt-semantic-interfaces<0.6,>=0.5.1 Requires-Dist: dbt-
+common<2.0 Requires-Dist: dbt-adapters<2.0,>=0.1.0a2 Requires-Dist:
+packaging>20.9 Requires-Dist: pytz>=2015.7 Requires-Dist: pyyaml>=6.0 Requires-
+Dist: daff>=1.3.46 Requires-Dist: typing-extensions>=4.4
                                   [dbt logo]
                                   _[_C_I_ _B_a_d_g_e_]
 **[dbt](https://www.getdbt.com/)** enables data analysts and engineers to
 transform their data using the same practices that software engineers use to
 build applications. ![architecture](https://raw.githubusercontent.com/dbt-labs/
 dbt-core/6c6649f9129d5d108aa3b0526f634cd8f3a9d1ed/etc/dbt-arch.png) ##
 Understanding dbt Analysts using dbt can transform their data by simply writing
```

### Comparing `dbt-core-1.8.0b1/dbt_core.egg-info/SOURCES.txt` & `dbt-core-1.8.0b2/dbt_core.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dbt-core-1.8.0b1/setup.py` & `dbt-core-1.8.0b2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 
 this_directory = os.path.abspath(os.path.dirname(__file__))
 with open(os.path.join(this_directory, "README.md")) as f:
     long_description = f.read()
 
 
 package_name = "dbt-core"
-package_version = "1.8.0b1"
+package_version = "1.8.0b2"
 description = """With dbt, data analysts and engineers can build analytics \
 the way engineers build applications."""
 
 
 setup(
     name=package_name,
     version=package_version,
@@ -57,33 +57,33 @@
         # The dependency here will be removed along with the removal of 'legacy logging', in a future release of dbt-core
         "logbook>=1.5,<1.6",
         # ----
         # dbt-core uses these packages in standard ways. Pin to the major version, and check compatibility
         # with major versions in each new minor version of dbt-core.
         "click>=8.0.2,<9.0",
         "networkx>=2.3,<4.0",
+        "protobuf>=4.0.0,<5",
         "requests<3.0.0",  # should match dbt-common
         # ----
         # These packages are major-version-0. Keep upper bounds on upcoming minor versions (which could have breaking changes)
         # and check compatibility / bump in each new minor version of dbt-core.
         "pathspec>=0.9,<0.12",
         "sqlparse>=0.2.3,<0.5",
         # ----
         # These are major-version-0 packages also maintained by dbt-labs.
         # Accept patches but avoid automatically updating past a set minor version range.
         "dbt-extractor>=0.5.0,<=0.6",
         "minimal-snowplow-tracker>=0.0.2,<0.1",
-        "dbt-semantic-interfaces>=0.5.0a2,<0.6",
+        "dbt-semantic-interfaces>=0.5.1,<0.6",
         # Minor versions for these are expected to be backwards-compatible
         "dbt-common<2.0",
         "dbt-adapters>=0.1.0a2,<2.0",
         # ----
         # Expect compatibility with all new versions of these packages, so lower bounds only.
         "packaging>20.9",
-        "protobuf>=4.0.0",
         "pytz>=2015.7",
         "pyyaml>=6.0",
         "daff>=1.3.46",
         "typing-extensions>=4.4",
         # ----
     ],
     zip_safe=False,
```

