# Comparing `tmp/dbt-snowflake-1.8.0b1.tar.gz` & `tmp/dbt-snowflake-1.8.0b2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dbt-snowflake-1.8.0b1.tar", last modified: Sat Mar  2 01:58:48 2024, max compression
+gzip compressed data, was "dbt-snowflake-1.8.0b2.tar", last modified: Wed Apr  3 19:59:22 2024, max compression
```

## Comparing `dbt-snowflake-1.8.0b1.tar` & `dbt-snowflake-1.8.0b2.tar`

### file list

```diff
@@ -1,79 +1,79 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-02 01:58:48.209085 dbt-snowflake-1.8.0b1/
--rw-r--r--   0 runner    (1001) docker     (127)    11344 2024-03-02 01:58:36.000000 dbt-snowflake-1.8.0b1/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-03-02 01:58:36.000000 dbt-snowflake-1.8.0b1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     3154 2024-03-02 01:58:48.209085 dbt-snowflake-1.8.0b1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2167 2024-03-02 01:58:36.000000 dbt-snowflake-1.8.0b1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-02 01:58:48.197085 dbt-snowflake-1.8.0b1/dbt/
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-03-02 01:58:36.000000 dbt-snowflake-1.8.0b1/dbt/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-02 01:58:48.197085 dbt-snowflake-1.8.0b1/dbt/adapters/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-02 01:58:48.201085 dbt-snowflake-1.8.0b1/dbt/adapters/snowflake/
--rw-r--r--   0 runner    (1001) docker     (127)      597 2024-03-02 01:58:36.000000 dbt-snowflake-1.8.0b1/dbt/adapters/snowflake/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-03-02 01:58:36.000000 dbt-snowflake-1.8.0b1/dbt/adapters/snowflake/__version__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1088 2024-03-02 01:58:36.000000 dbt-snowflake-1.8.0b1/dbt/adapters/snowflake/column.py
--rw-r--r--   0 runner    (1001) docker     (127)    21949 2024-03-02 01:58:36.000000 dbt-snowflake-1.8.0b1/dbt/adapters/snowflake/connections.py
--rw-r--r--   0 runner    (1001) docker     (127)    10197 2024-03-02 01:58:36.000000 dbt-snowflake-1.8.0b1/dbt/adapters/snowflake/impl.py
--rw-r--r--   0 runner    (1001) docker     (127)     2760 2024-03-02 01:58:36.000000 dbt-snowflake-1.8.0b1/dbt/adapters/snowflake/relation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-02 01:58:48.201085 dbt-snowflake-1.8.0b1/dbt/adapters/snowflake/relation_configs/
--rw-r--r--   0 runner    (1001) docker     (127)      387 2024-03-02 01:58:36.000000 dbt-snowflake-1.8.0b1/dbt/adapters/snowflake/relation_configs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2348 2024-03-02 01:58:36.000000 dbt-snowflake-1.8.0b1/dbt/adapters/snowflake/relation_configs/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     4259 2024-03-02 01:58:36.000000 dbt-snowflake-1.8.0b1/dbt/adapters/snowflake/relation_configs/dynamic_table.py
--rw-r--r--   0 runner    (1001) docker     (127)      532 2024-03-02 01:58:36.000000 dbt-snowflake-1.8.0b1/dbt/adapters/snowflake/relation_configs/policies.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-02 01:58:48.197085 dbt-snowflake-1.8.0b1/dbt/include/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-02 01:58:48.201085 dbt-snowflake-1.8.0b1/dbt/include/snowflake/
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-03-02 01:58:36.000000 dbt-snowflake-1.8.0b1/dbt/include/snowflake/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-03-02 01:58:36.000000 dbt-snowflake-1.8.0b1/dbt/include/snowflake/dbt_project.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-02 01:58:48.201085 dbt-snowflake-1.8.0b1/dbt/include/snowflake/macros/
--rw-r--r--   0 runner    (1001) docker     (127)     9813 2024-03-02 01:58:36.000000 dbt-snowflake-1.8.0b1/dbt/include/snowflake/macros/adapters.sql
--rw-r--r--   0 runner    (1001) docker     (127)      256 2024-03-02 01:58:36.000000 dbt-snowflake-1.8.0b1/dbt/include/snowflake/macros/apply_grants.sql
--rw-r--r--   0 runner    (1001) docker     (127)     4426 2024-03-02 01:58:36.000000 dbt-snowflake-1.8.0b1/dbt/include/snowflake/macros/catalog.sql
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-02 01:58:48.201085 dbt-snowflake-1.8.0b1/dbt/include/snowflake/macros/materializations/
--rw-r--r--   0 runner    (1001) docker     (127)      379 2024-03-02 01:58:36.000000 dbt-snowflake-1.8.0b1/dbt/include/snowflake/macros/materializations/clone.sql
--rw-r--r--   0 runner    (1001) docker     (127)     3717 2024-03-02 01:58:36.000000 dbt-snowflake-1.8.0b1/dbt/include/snowflake/macros/materializations/dynamic_table.sql
--rw-r--r--   0 runner    (1001) docker     (127)     6474 2024-03-02 01:58:36.000000 dbt-snowflake-1.8.0b1/dbt/include/snowflake/macros/materializations/incremental.sql
--rw-r--r--   0 runner    (1001) docker     (127)     1803 2024-03-02 01:58:36.000000 dbt-snowflake-1.8.0b1/dbt/include/snowflake/macros/materializations/merge.sql
--rw-r--r--   0 runner    (1001) docker     (127)     1536 2024-03-02 01:58:36.000000 dbt-snowflake-1.8.0b1/dbt/include/snowflake/macros/materializations/seed.sql
--rw-r--r--   0 runner    (1001) docker     (127)      268 2024-03-02 01:58:36.000000 dbt-snowflake-1.8.0b1/dbt/include/snowflake/macros/materializations/snapshot.sql
--rw-r--r--   0 runner    (1001) docker     (127)     3591 2024-03-02 01:58:36.000000 dbt-snowflake-1.8.0b1/dbt/include/snowflake/macros/materializations/table.sql
--rw-r--r--   0 runner    (1001) docker     (127)      264 2024-03-02 01:58:36.000000 dbt-snowflake-1.8.0b1/dbt/include/snowflake/macros/materializations/test.sql
--rw-r--r--   0 runner    (1001) docker     (127)      405 2024-03-02 01:58:36.000000 dbt-snowflake-1.8.0b1/dbt/include/snowflake/macros/materializations/view.sql
--rw-r--r--   0 runner    (1001) docker     (127)      727 2024-03-02 01:58:36.000000 dbt-snowflake-1.8.0b1/dbt/include/snowflake/macros/metadata.sql
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-02 01:58:48.205085 dbt-snowflake-1.8.0b1/dbt/include/snowflake/macros/relations/
--rw-r--r--   0 runner    (1001) docker     (127)      267 2024-03-02 01:58:36.000000 dbt-snowflake-1.8.0b1/dbt/include/snowflake/macros/relations/create.sql
--rw-r--r--   0 runner    (1001) docker     (127)      243 2024-03-02 01:58:36.000000 dbt-snowflake-1.8.0b1/dbt/include/snowflake/macros/relations/drop.sql
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-02 01:58:48.205085 dbt-snowflake-1.8.0b1/dbt/include/snowflake/macros/relations/dynamic_table/
--rw-r--r--   0 runner    (1001) docker     (127)      992 2024-03-02 01:58:36.000000 dbt-snowflake-1.8.0b1/dbt/include/snowflake/macros/relations/dynamic_table/alter.sql
--rw-r--r--   0 runner    (1001) docker     (127)      294 2024-03-02 01:58:36.000000 dbt-snowflake-1.8.0b1/dbt/include/snowflake/macros/relations/dynamic_table/create.sql
--rw-r--r--   0 runner    (1001) docker     (127)      602 2024-03-02 01:58:36.000000 dbt-snowflake-1.8.0b1/dbt/include/snowflake/macros/relations/dynamic_table/describe.sql
--rw-r--r--   0 runner    (1001) docker     (127)      123 2024-03-02 01:58:36.000000 dbt-snowflake-1.8.0b1/dbt/include/snowflake/macros/relations/dynamic_table/drop.sql
--rw-r--r--   0 runner    (1001) docker     (127)      172 2024-03-02 01:58:36.000000 dbt-snowflake-1.8.0b1/dbt/include/snowflake/macros/relations/dynamic_table/refresh.sql
--rw-r--r--   0 runner    (1001) docker     (127)      354 2024-03-02 01:58:36.000000 dbt-snowflake-1.8.0b1/dbt/include/snowflake/macros/relations/dynamic_table/replace.sql
--rw-r--r--   0 runner    (1001) docker     (127)      207 2024-03-02 01:58:36.000000 dbt-snowflake-1.8.0b1/dbt/include/snowflake/macros/relations/rename.sql
--rw-r--r--   0 runner    (1001) docker     (127)      372 2024-03-02 01:58:36.000000 dbt-snowflake-1.8.0b1/dbt/include/snowflake/macros/relations/replace.sql
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-02 01:58:48.205085 dbt-snowflake-1.8.0b1/dbt/include/snowflake/macros/relations/table/
--rw-r--r--   0 runner    (1001) docker     (127)     2403 2024-03-02 01:58:36.000000 dbt-snowflake-1.8.0b1/dbt/include/snowflake/macros/relations/table/create.sql
--rw-r--r--   0 runner    (1001) docker     (127)      115 2024-03-02 01:58:36.000000 dbt-snowflake-1.8.0b1/dbt/include/snowflake/macros/relations/table/drop.sql
--rw-r--r--   0 runner    (1001) docker     (127)      139 2024-03-02 01:58:36.000000 dbt-snowflake-1.8.0b1/dbt/include/snowflake/macros/relations/table/rename.sql
--rw-r--r--   0 runner    (1001) docker     (127)      134 2024-03-02 01:58:36.000000 dbt-snowflake-1.8.0b1/dbt/include/snowflake/macros/relations/table/replace.sql
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-02 01:58:48.205085 dbt-snowflake-1.8.0b1/dbt/include/snowflake/macros/relations/view/
--rw-r--r--   0 runner    (1001) docker     (127)     2648 2024-03-02 01:58:36.000000 dbt-snowflake-1.8.0b1/dbt/include/snowflake/macros/relations/view/create.sql
--rw-r--r--   0 runner    (1001) docker     (127)      113 2024-03-02 01:58:36.000000 dbt-snowflake-1.8.0b1/dbt/include/snowflake/macros/relations/view/drop.sql
--rw-r--r--   0 runner    (1001) docker     (127)      137 2024-03-02 01:58:36.000000 dbt-snowflake-1.8.0b1/dbt/include/snowflake/macros/relations/view/rename.sql
--rw-r--r--   0 runner    (1001) docker     (127)      125 2024-03-02 01:58:36.000000 dbt-snowflake-1.8.0b1/dbt/include/snowflake/macros/relations/view/replace.sql
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-02 01:58:48.209085 dbt-snowflake-1.8.0b1/dbt/include/snowflake/macros/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      123 2024-03-02 01:58:36.000000 dbt-snowflake-1.8.0b1/dbt/include/snowflake/macros/utils/array_construct.sql
--rw-r--r--   0 runner    (1001) docker     (127)       95 2024-03-02 01:58:36.000000 dbt-snowflake-1.8.0b1/dbt/include/snowflake/macros/utils/bool_or.sql
--rw-r--r--   0 runner    (1001) docker     (127)      273 2024-03-02 01:58:36.000000 dbt-snowflake-1.8.0b1/dbt/include/snowflake/macros/utils/cast.sql
--rw-r--r--   0 runner    (1001) docker     (127)      227 2024-03-02 01:58:36.000000 dbt-snowflake-1.8.0b1/dbt/include/snowflake/macros/utils/escape_single_quotes.sql
--rw-r--r--   0 runner    (1001) docker     (127)      247 2024-03-02 01:58:36.000000 dbt-snowflake-1.8.0b1/dbt/include/snowflake/macros/utils/right.sql
--rw-r--r--   0 runner    (1001) docker     (127)      596 2024-03-02 01:58:36.000000 dbt-snowflake-1.8.0b1/dbt/include/snowflake/macros/utils/safe_cast.sql
--rw-r--r--   0 runner    (1001) docker     (127)      666 2024-03-02 01:58:36.000000 dbt-snowflake-1.8.0b1/dbt/include/snowflake/macros/utils/timestamps.sql
--rw-r--r--   0 runner    (1001) docker     (127)      837 2024-03-02 01:58:36.000000 dbt-snowflake-1.8.0b1/dbt/include/snowflake/profile_template.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-02 01:58:48.209085 dbt-snowflake-1.8.0b1/dbt_snowflake.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3154 2024-03-02 01:58:48.000000 dbt-snowflake-1.8.0b1/dbt_snowflake.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2876 2024-03-02 01:58:48.000000 dbt-snowflake-1.8.0b1/dbt_snowflake.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-02 01:58:48.000000 dbt-snowflake-1.8.0b1/dbt_snowflake.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-02 01:58:48.000000 dbt-snowflake-1.8.0b1/dbt_snowflake.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      112 2024-03-02 01:58:48.000000 dbt-snowflake-1.8.0b1/dbt_snowflake.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        4 2024-03-02 01:58:48.000000 dbt-snowflake-1.8.0b1/dbt_snowflake.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-02 01:58:48.209085 dbt-snowflake-1.8.0b1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2907 2024-03-02 01:58:36.000000 dbt-snowflake-1.8.0b1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 19:59:22.723668 dbt-snowflake-1.8.0b2/
+-rw-r--r--   0 runner    (1001) docker     (127)    11344 2024-04-03 19:59:06.000000 dbt-snowflake-1.8.0b2/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-03 19:59:06.000000 dbt-snowflake-1.8.0b2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3187 2024-04-03 19:59:22.723668 dbt-snowflake-1.8.0b2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2167 2024-04-03 19:59:06.000000 dbt-snowflake-1.8.0b2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 19:59:22.711668 dbt-snowflake-1.8.0b2/dbt/
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-04-03 19:59:06.000000 dbt-snowflake-1.8.0b2/dbt/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 19:59:22.711668 dbt-snowflake-1.8.0b2/dbt/adapters/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 19:59:22.715669 dbt-snowflake-1.8.0b2/dbt/adapters/snowflake/
+-rw-r--r--   0 runner    (1001) docker     (127)      597 2024-04-03 19:59:06.000000 dbt-snowflake-1.8.0b2/dbt/adapters/snowflake/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-03 19:59:06.000000 dbt-snowflake-1.8.0b2/dbt/adapters/snowflake/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1088 2024-04-03 19:59:06.000000 dbt-snowflake-1.8.0b2/dbt/adapters/snowflake/column.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21917 2024-04-03 19:59:06.000000 dbt-snowflake-1.8.0b2/dbt/adapters/snowflake/connections.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10319 2024-04-03 19:59:06.000000 dbt-snowflake-1.8.0b2/dbt/adapters/snowflake/impl.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3024 2024-04-03 19:59:06.000000 dbt-snowflake-1.8.0b2/dbt/adapters/snowflake/relation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 19:59:22.715669 dbt-snowflake-1.8.0b2/dbt/adapters/snowflake/relation_configs/
+-rw-r--r--   0 runner    (1001) docker     (127)      387 2024-04-03 19:59:06.000000 dbt-snowflake-1.8.0b2/dbt/adapters/snowflake/relation_configs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2348 2024-04-03 19:59:06.000000 dbt-snowflake-1.8.0b2/dbt/adapters/snowflake/relation_configs/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4259 2024-04-03 19:59:06.000000 dbt-snowflake-1.8.0b2/dbt/adapters/snowflake/relation_configs/dynamic_table.py
+-rw-r--r--   0 runner    (1001) docker     (127)      532 2024-04-03 19:59:06.000000 dbt-snowflake-1.8.0b2/dbt/adapters/snowflake/relation_configs/policies.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 19:59:22.711668 dbt-snowflake-1.8.0b2/dbt/include/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 19:59:22.715669 dbt-snowflake-1.8.0b2/dbt/include/snowflake/
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-03 19:59:06.000000 dbt-snowflake-1.8.0b2/dbt/include/snowflake/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-04-03 19:59:06.000000 dbt-snowflake-1.8.0b2/dbt/include/snowflake/dbt_project.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 19:59:22.715669 dbt-snowflake-1.8.0b2/dbt/include/snowflake/macros/
+-rw-r--r--   0 runner    (1001) docker     (127)     9813 2024-04-03 19:59:06.000000 dbt-snowflake-1.8.0b2/dbt/include/snowflake/macros/adapters.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      256 2024-04-03 19:59:06.000000 dbt-snowflake-1.8.0b2/dbt/include/snowflake/macros/apply_grants.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     4520 2024-04-03 19:59:06.000000 dbt-snowflake-1.8.0b2/dbt/include/snowflake/macros/catalog.sql
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 19:59:22.715669 dbt-snowflake-1.8.0b2/dbt/include/snowflake/macros/materializations/
+-rw-r--r--   0 runner    (1001) docker     (127)      379 2024-04-03 19:59:06.000000 dbt-snowflake-1.8.0b2/dbt/include/snowflake/macros/materializations/clone.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     3717 2024-04-03 19:59:06.000000 dbt-snowflake-1.8.0b2/dbt/include/snowflake/macros/materializations/dynamic_table.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     6474 2024-04-03 19:59:06.000000 dbt-snowflake-1.8.0b2/dbt/include/snowflake/macros/materializations/incremental.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     1803 2024-04-03 19:59:06.000000 dbt-snowflake-1.8.0b2/dbt/include/snowflake/macros/materializations/merge.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     1536 2024-04-03 19:59:06.000000 dbt-snowflake-1.8.0b2/dbt/include/snowflake/macros/materializations/seed.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      268 2024-04-03 19:59:06.000000 dbt-snowflake-1.8.0b2/dbt/include/snowflake/macros/materializations/snapshot.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     3591 2024-04-03 19:59:06.000000 dbt-snowflake-1.8.0b2/dbt/include/snowflake/macros/materializations/table.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      264 2024-04-03 19:59:06.000000 dbt-snowflake-1.8.0b2/dbt/include/snowflake/macros/materializations/test.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      405 2024-04-03 19:59:06.000000 dbt-snowflake-1.8.0b2/dbt/include/snowflake/macros/materializations/view.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      727 2024-04-03 19:59:06.000000 dbt-snowflake-1.8.0b2/dbt/include/snowflake/macros/metadata.sql
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 19:59:22.719668 dbt-snowflake-1.8.0b2/dbt/include/snowflake/macros/relations/
+-rw-r--r--   0 runner    (1001) docker     (127)      267 2024-04-03 19:59:06.000000 dbt-snowflake-1.8.0b2/dbt/include/snowflake/macros/relations/create.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      243 2024-04-03 19:59:06.000000 dbt-snowflake-1.8.0b2/dbt/include/snowflake/macros/relations/drop.sql
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 19:59:22.719668 dbt-snowflake-1.8.0b2/dbt/include/snowflake/macros/relations/dynamic_table/
+-rw-r--r--   0 runner    (1001) docker     (127)      992 2024-04-03 19:59:06.000000 dbt-snowflake-1.8.0b2/dbt/include/snowflake/macros/relations/dynamic_table/alter.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      288 2024-04-03 19:59:06.000000 dbt-snowflake-1.8.0b2/dbt/include/snowflake/macros/relations/dynamic_table/create.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      602 2024-04-03 19:59:06.000000 dbt-snowflake-1.8.0b2/dbt/include/snowflake/macros/relations/dynamic_table/describe.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      123 2024-04-03 19:59:06.000000 dbt-snowflake-1.8.0b2/dbt/include/snowflake/macros/relations/dynamic_table/drop.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      172 2024-04-03 19:59:06.000000 dbt-snowflake-1.8.0b2/dbt/include/snowflake/macros/relations/dynamic_table/refresh.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      354 2024-04-03 19:59:06.000000 dbt-snowflake-1.8.0b2/dbt/include/snowflake/macros/relations/dynamic_table/replace.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      207 2024-04-03 19:59:06.000000 dbt-snowflake-1.8.0b2/dbt/include/snowflake/macros/relations/rename.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      372 2024-04-03 19:59:06.000000 dbt-snowflake-1.8.0b2/dbt/include/snowflake/macros/relations/replace.sql
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 19:59:22.719668 dbt-snowflake-1.8.0b2/dbt/include/snowflake/macros/relations/table/
+-rw-r--r--   0 runner    (1001) docker     (127)     2403 2024-04-03 19:59:06.000000 dbt-snowflake-1.8.0b2/dbt/include/snowflake/macros/relations/table/create.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      115 2024-04-03 19:59:06.000000 dbt-snowflake-1.8.0b2/dbt/include/snowflake/macros/relations/table/drop.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      139 2024-04-03 19:59:06.000000 dbt-snowflake-1.8.0b2/dbt/include/snowflake/macros/relations/table/rename.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      134 2024-04-03 19:59:06.000000 dbt-snowflake-1.8.0b2/dbt/include/snowflake/macros/relations/table/replace.sql
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 19:59:22.719668 dbt-snowflake-1.8.0b2/dbt/include/snowflake/macros/relations/view/
+-rw-r--r--   0 runner    (1001) docker     (127)     2648 2024-04-03 19:59:06.000000 dbt-snowflake-1.8.0b2/dbt/include/snowflake/macros/relations/view/create.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      113 2024-04-03 19:59:06.000000 dbt-snowflake-1.8.0b2/dbt/include/snowflake/macros/relations/view/drop.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      137 2024-04-03 19:59:06.000000 dbt-snowflake-1.8.0b2/dbt/include/snowflake/macros/relations/view/rename.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      125 2024-04-03 19:59:06.000000 dbt-snowflake-1.8.0b2/dbt/include/snowflake/macros/relations/view/replace.sql
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 19:59:22.723668 dbt-snowflake-1.8.0b2/dbt/include/snowflake/macros/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      123 2024-04-03 19:59:06.000000 dbt-snowflake-1.8.0b2/dbt/include/snowflake/macros/utils/array_construct.sql
+-rw-r--r--   0 runner    (1001) docker     (127)       95 2024-04-03 19:59:06.000000 dbt-snowflake-1.8.0b2/dbt/include/snowflake/macros/utils/bool_or.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      273 2024-04-03 19:59:06.000000 dbt-snowflake-1.8.0b2/dbt/include/snowflake/macros/utils/cast.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      227 2024-04-03 19:59:06.000000 dbt-snowflake-1.8.0b2/dbt/include/snowflake/macros/utils/escape_single_quotes.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      247 2024-04-03 19:59:06.000000 dbt-snowflake-1.8.0b2/dbt/include/snowflake/macros/utils/right.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      596 2024-04-03 19:59:06.000000 dbt-snowflake-1.8.0b2/dbt/include/snowflake/macros/utils/safe_cast.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      666 2024-04-03 19:59:06.000000 dbt-snowflake-1.8.0b2/dbt/include/snowflake/macros/utils/timestamps.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      837 2024-04-03 19:59:06.000000 dbt-snowflake-1.8.0b2/dbt/include/snowflake/profile_template.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 19:59:22.723668 dbt-snowflake-1.8.0b2/dbt_snowflake.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3187 2024-04-03 19:59:22.000000 dbt-snowflake-1.8.0b2/dbt_snowflake.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2876 2024-04-03 19:59:22.000000 dbt-snowflake-1.8.0b2/dbt_snowflake.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 19:59:22.000000 dbt-snowflake-1.8.0b2/dbt_snowflake.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 19:59:22.000000 dbt-snowflake-1.8.0b2/dbt_snowflake.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      130 2024-04-03 19:59:22.000000 dbt-snowflake-1.8.0b2/dbt_snowflake.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-04-03 19:59:22.000000 dbt-snowflake-1.8.0b2/dbt_snowflake.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-03 19:59:22.723668 dbt-snowflake-1.8.0b2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3091 2024-04-03 19:59:06.000000 dbt-snowflake-1.8.0b2/setup.py
```

### Comparing `dbt-snowflake-1.8.0b1/LICENSE.md` & `dbt-snowflake-1.8.0b2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `dbt-snowflake-1.8.0b1/PKG-INFO` & `dbt-snowflake-1.8.0b2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbt-snowflake
-Version: 1.8.0b1
+Version: 1.8.0b2
 Summary: The Snowflake adapter plugin for dbt
 Home-page: https://github.com/dbt-labs/dbt-snowflake
 Author: dbt Labs
 Author-email: info@dbtlabs.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: Microsoft :: Windows
@@ -17,14 +17,15 @@
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 Requires-Dist: dbt-common<2.0,>=0.1.0a1
 Requires-Dist: dbt-adapters<2.0,>=0.1.0a1
 Requires-Dist: snowflake-connector-python[secure-local-storage]~=3.0
+Requires-Dist: dbt-core>=1.8.0a1
 Requires-Dist: agate
 
 <p align="center">
   <img src="https://raw.githubusercontent.com/dbt-labs/dbt/ec7dee39f793aa4f7dd3dae37282cc87664813e4/etc/dbt-logo-full.svg" alt="dbt logo" width="500"/>
 </p>
 <p align="center">
   <a href="https://github.com/dbt-labs/dbt-snowflake/actions/workflows/main.yml">
```

#### html2text {}

```diff
@@ -1,20 +1,21 @@
-Metadata-Version: 2.1 Name: dbt-snowflake Version: 1.8.0b1 Summary: The
+Metadata-Version: 2.1 Name: dbt-snowflake Version: 1.8.0b2 Summary: The
 Snowflake adapter plugin for dbt Home-page: https://github.com/dbt-labs/dbt-
 snowflake Author: dbt Labs Author-email: info@dbtlabs.com Classifier:
 Development Status :: 5 - Production/Stable Classifier: License :: OSI Approved
 :: Apache Software License Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS :: MacOS X Classifier: Operating System
 :: POSIX :: Linux Classifier: Programming Language :: Python :: 3.8 Classifier:
 Programming Language :: Python :: 3.8 Classifier: Programming Language ::
 Python :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
 Programming Language :: Python :: 3.11 Requires-Python: >=3.8 Description-
 Content-Type: text/markdown License-File: LICENSE.md Requires-Dist: dbt-
 common<2.0,>=0.1.0a1 Requires-Dist: dbt-adapters<2.0,>=0.1.0a1 Requires-Dist:
-snowflake-connector-python[secure-local-storage]~=3.0 Requires-Dist: agate
+snowflake-connector-python[secure-local-storage]~=3.0 Requires-Dist: dbt-
+core>=1.8.0a1 Requires-Dist: agate
                                   [dbt logo]
                   _[_U_n_i_t_ _T_e_s_t_s_ _B_a_d_g_e_]_[_I_n_t_e_g_r_a_t_i_o_n_ _T_e_s_t_s_ _B_a_d_g_e_]
 **[dbt](https://www.getdbt.com/)** enables data analysts and engineers to
 transform their data using the same practices that software engineers use to
 build applications. dbt is the T in ELT. Organize, cleanse, denormalize,
 filter, rename, and pre-aggregate the raw data in your warehouse so that it's
 ready for analysis. ## dbt-snowflake The `dbt-snowflake` package contains all
```

### Comparing `dbt-snowflake-1.8.0b1/README.md` & `dbt-snowflake-1.8.0b2/README.md`

 * *Files identical despite different names*

### Comparing `dbt-snowflake-1.8.0b1/dbt/adapters/snowflake/__init__.py` & `dbt-snowflake-1.8.0b2/dbt/adapters/snowflake/__init__.py`

 * *Files identical despite different names*

### Comparing `dbt-snowflake-1.8.0b1/dbt/adapters/snowflake/column.py` & `dbt-snowflake-1.8.0b2/dbt/adapters/snowflake/column.py`

 * *Files identical despite different names*

### Comparing `dbt-snowflake-1.8.0b1/dbt/adapters/snowflake/connections.py` & `dbt-snowflake-1.8.0b2/dbt/adapters/snowflake/connections.py`

 * *Files 0% similar despite different names*

```diff
@@ -121,15 +121,14 @@
             "account",
             "user",
             "database",
             "warehouse",
             "role",
             "schema",
             "authenticator",
-            "private_key_path",
             "oauth_client_id",
             "query_tag",
             "client_session_keep_alive",
             "host",
             "port",
             "proxy_host",
             "proxy_port",
```

### Comparing `dbt-snowflake-1.8.0b1/dbt/adapters/snowflake/impl.py` & `dbt-snowflake-1.8.0b2/dbt/adapters/snowflake/impl.py`

 * *Files 2% similar despite different names*

```diff
@@ -213,18 +213,21 @@
                 packages.append(default_package)
         packages = "', '".join(packages)
         imports = "', '".join(imports)
         # we can't pass empty imports clause to snowflake
         if imports:
             imports = f"IMPORTS = ('{imports}')"
 
-        snowpark_telemetry_string = "dbtLabs_dbtPython"
-        snowpark_telemetry_snippet = f"""
+        if self.config.args.SEND_ANONYMOUS_USAGE_STATS:
+            snowpark_telemetry_string = "dbtLabs_dbtPython"
+            snowpark_telemetry_snippet = f"""
 import sys
 sys._xoptions['snowflake_partner_attribution'].append("{snowpark_telemetry_string}")"""
+        else:
+            snowpark_telemetry_snippet = ""
 
         common_procedure_code = f"""
 RETURNS STRING
 LANGUAGE PYTHON
 RUNTIME_VERSION = '{python_version}'
 PACKAGES = ('{packages}')
 {imports}
```

### Comparing `dbt-snowflake-1.8.0b1/dbt/adapters/snowflake/relation.py` & `dbt-snowflake-1.8.0b2/dbt/adapters/snowflake/relation.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from dataclasses import dataclass, field
-from typing import Optional, Type
+from typing import FrozenSet, Optional, Type
 
 from dbt.adapters.base.relation import BaseRelation
 from dbt.adapters.relation_configs import RelationConfigChangeAction, RelationResults
 from dbt.adapters.contracts.relation import RelationConfig
 from dbt.adapters.utils import classproperty
 
 from dbt.adapters.snowflake.relation_configs import (
@@ -16,21 +16,32 @@
 )
 
 
 @dataclass(frozen=True, eq=False, repr=False)
 class SnowflakeRelation(BaseRelation):
     type: Optional[SnowflakeRelationType] = None  # type: ignore
     quote_policy: SnowflakeQuotePolicy = field(default_factory=lambda: SnowflakeQuotePolicy())
-    renameable_relations = frozenset({SnowflakeRelationType.Table, SnowflakeRelationType.View})
-    replaceable_relations = frozenset(
-        {
-            SnowflakeRelationType.DynamicTable,
-            SnowflakeRelationType.Table,
-            SnowflakeRelationType.View,
-        }
+
+    renameable_relations: FrozenSet[SnowflakeRelationType] = field(
+        default_factory=lambda: frozenset(
+            {
+                SnowflakeRelationType.Table,
+                SnowflakeRelationType.View,
+            }
+        )
+    )
+
+    replaceable_relations: FrozenSet[SnowflakeRelationType] = field(
+        default_factory=lambda: frozenset(
+            {
+                SnowflakeRelationType.DynamicTable,
+                SnowflakeRelationType.Table,
+                SnowflakeRelationType.View,
+            }
+        )
     )
 
     @property
     def is_dynamic_table(self) -> bool:
         return self.type == SnowflakeRelationType.DynamicTable
 
     @classproperty
```

### Comparing `dbt-snowflake-1.8.0b1/dbt/adapters/snowflake/relation_configs/base.py` & `dbt-snowflake-1.8.0b2/dbt/adapters/snowflake/relation_configs/base.py`

 * *Files identical despite different names*

### Comparing `dbt-snowflake-1.8.0b1/dbt/adapters/snowflake/relation_configs/dynamic_table.py` & `dbt-snowflake-1.8.0b2/dbt/adapters/snowflake/relation_configs/dynamic_table.py`

 * *Files identical despite different names*

### Comparing `dbt-snowflake-1.8.0b1/dbt/adapters/snowflake/relation_configs/policies.py` & `dbt-snowflake-1.8.0b2/dbt/adapters/snowflake/relation_configs/policies.py`

 * *Files identical despite different names*

### Comparing `dbt-snowflake-1.8.0b1/dbt/include/snowflake/macros/adapters.sql` & `dbt-snowflake-1.8.0b2/dbt/include/snowflake/macros/adapters.sql`

 * *Files identical despite different names*

### Comparing `dbt-snowflake-1.8.0b1/dbt/include/snowflake/macros/catalog.sql` & `dbt-snowflake-1.8.0b2/dbt/include/snowflake/macros/catalog.sql`

 * *Files 2% similar despite different names*

```diff
@@ -37,15 +37,18 @@
 
 
 {% macro snowflake__get_catalog_tables_sql(information_schema) -%}
     select
         table_catalog as "table_database",
         table_schema as "table_schema",
         table_name as "table_name",
-        coalesce(table_type, 'DYNAMIC TABLE') as "table_type",
+        case
+            when is_dynamic = 'YES' and table_type = 'BASE TABLE' THEN 'DYNAMIC TABLE'
+            else table_type
+        end as "table_type",
         comment as "table_comment",
 
         -- note: this is the _role_ that owns the table
         table_owner as "table_owner",
 
         'Clustering Key' as "stats:clustering_key:label",
         clustering_key as "stats:clustering_key:value",
```

### Comparing `dbt-snowflake-1.8.0b1/dbt/include/snowflake/macros/materializations/dynamic_table.sql` & `dbt-snowflake-1.8.0b2/dbt/include/snowflake/macros/materializations/dynamic_table.sql`

 * *Files identical despite different names*

### Comparing `dbt-snowflake-1.8.0b1/dbt/include/snowflake/macros/materializations/incremental.sql` & `dbt-snowflake-1.8.0b2/dbt/include/snowflake/macros/materializations/incremental.sql`

 * *Files identical despite different names*

### Comparing `dbt-snowflake-1.8.0b1/dbt/include/snowflake/macros/materializations/merge.sql` & `dbt-snowflake-1.8.0b2/dbt/include/snowflake/macros/materializations/merge.sql`

 * *Files identical despite different names*

### Comparing `dbt-snowflake-1.8.0b1/dbt/include/snowflake/macros/materializations/seed.sql` & `dbt-snowflake-1.8.0b2/dbt/include/snowflake/macros/materializations/seed.sql`

 * *Files identical despite different names*

### Comparing `dbt-snowflake-1.8.0b1/dbt/include/snowflake/macros/materializations/table.sql` & `dbt-snowflake-1.8.0b2/dbt/include/snowflake/macros/materializations/table.sql`

 * *Files identical despite different names*

### Comparing `dbt-snowflake-1.8.0b1/dbt/include/snowflake/macros/metadata.sql` & `dbt-snowflake-1.8.0b2/dbt/include/snowflake/macros/metadata.sql`

 * *Files identical despite different names*

### Comparing `dbt-snowflake-1.8.0b1/dbt/include/snowflake/macros/relations/dynamic_table/alter.sql` & `dbt-snowflake-1.8.0b2/dbt/include/snowflake/macros/relations/dynamic_table/alter.sql`

 * *Files identical despite different names*

### Comparing `dbt-snowflake-1.8.0b1/dbt/include/snowflake/macros/relations/dynamic_table/describe.sql` & `dbt-snowflake-1.8.0b2/dbt/include/snowflake/macros/relations/dynamic_table/describe.sql`

 * *Files identical despite different names*

### Comparing `dbt-snowflake-1.8.0b1/dbt/include/snowflake/macros/relations/table/create.sql` & `dbt-snowflake-1.8.0b2/dbt/include/snowflake/macros/relations/table/create.sql`

 * *Files identical despite different names*

### Comparing `dbt-snowflake-1.8.0b1/dbt/include/snowflake/macros/relations/view/create.sql` & `dbt-snowflake-1.8.0b2/dbt/include/snowflake/macros/relations/view/create.sql`

 * *Files identical despite different names*

### Comparing `dbt-snowflake-1.8.0b1/dbt/include/snowflake/macros/utils/safe_cast.sql` & `dbt-snowflake-1.8.0b2/dbt/include/snowflake/macros/utils/safe_cast.sql`

 * *Files identical despite different names*

### Comparing `dbt-snowflake-1.8.0b1/dbt/include/snowflake/macros/utils/timestamps.sql` & `dbt-snowflake-1.8.0b2/dbt/include/snowflake/macros/utils/timestamps.sql`

 * *Files identical despite different names*

### Comparing `dbt-snowflake-1.8.0b1/dbt/include/snowflake/profile_template.yml` & `dbt-snowflake-1.8.0b2/dbt/include/snowflake/profile_template.yml`

 * *Files identical despite different names*

### Comparing `dbt-snowflake-1.8.0b1/dbt_snowflake.egg-info/PKG-INFO` & `dbt-snowflake-1.8.0b2/dbt_snowflake.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbt-snowflake
-Version: 1.8.0b1
+Version: 1.8.0b2
 Summary: The Snowflake adapter plugin for dbt
 Home-page: https://github.com/dbt-labs/dbt-snowflake
 Author: dbt Labs
 Author-email: info@dbtlabs.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: Microsoft :: Windows
@@ -17,14 +17,15 @@
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 Requires-Dist: dbt-common<2.0,>=0.1.0a1
 Requires-Dist: dbt-adapters<2.0,>=0.1.0a1
 Requires-Dist: snowflake-connector-python[secure-local-storage]~=3.0
+Requires-Dist: dbt-core>=1.8.0a1
 Requires-Dist: agate
 
 <p align="center">
   <img src="https://raw.githubusercontent.com/dbt-labs/dbt/ec7dee39f793aa4f7dd3dae37282cc87664813e4/etc/dbt-logo-full.svg" alt="dbt logo" width="500"/>
 </p>
 <p align="center">
   <a href="https://github.com/dbt-labs/dbt-snowflake/actions/workflows/main.yml">
```

#### html2text {}

```diff
@@ -1,20 +1,21 @@
-Metadata-Version: 2.1 Name: dbt-snowflake Version: 1.8.0b1 Summary: The
+Metadata-Version: 2.1 Name: dbt-snowflake Version: 1.8.0b2 Summary: The
 Snowflake adapter plugin for dbt Home-page: https://github.com/dbt-labs/dbt-
 snowflake Author: dbt Labs Author-email: info@dbtlabs.com Classifier:
 Development Status :: 5 - Production/Stable Classifier: License :: OSI Approved
 :: Apache Software License Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS :: MacOS X Classifier: Operating System
 :: POSIX :: Linux Classifier: Programming Language :: Python :: 3.8 Classifier:
 Programming Language :: Python :: 3.8 Classifier: Programming Language ::
 Python :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
 Programming Language :: Python :: 3.11 Requires-Python: >=3.8 Description-
 Content-Type: text/markdown License-File: LICENSE.md Requires-Dist: dbt-
 common<2.0,>=0.1.0a1 Requires-Dist: dbt-adapters<2.0,>=0.1.0a1 Requires-Dist:
-snowflake-connector-python[secure-local-storage]~=3.0 Requires-Dist: agate
+snowflake-connector-python[secure-local-storage]~=3.0 Requires-Dist: dbt-
+core>=1.8.0a1 Requires-Dist: agate
                                   [dbt logo]
                   _[_U_n_i_t_ _T_e_s_t_s_ _B_a_d_g_e_]_[_I_n_t_e_g_r_a_t_i_o_n_ _T_e_s_t_s_ _B_a_d_g_e_]
 **[dbt](https://www.getdbt.com/)** enables data analysts and engineers to
 transform their data using the same practices that software engineers use to
 build applications. dbt is the T in ELT. Organize, cleanse, denormalize,
 filter, rename, and pre-aggregate the raw data in your warehouse so that it's
 ready for analysis. ## dbt-snowflake The `dbt-snowflake` package contains all
```

### Comparing `dbt-snowflake-1.8.0b1/dbt_snowflake.egg-info/SOURCES.txt` & `dbt-snowflake-1.8.0b2/dbt_snowflake.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dbt-snowflake-1.8.0b1/setup.py` & `dbt-snowflake-1.8.0b2/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -30,24 +30,25 @@
 
 # get this package's version from dbt/adapters/<name>/__version__.py
 def _get_plugin_version_dict():
     _version_path = os.path.join(this_directory, "dbt", "adapters", "snowflake", "__version__.py")
     _semver = r"""(?P<major>\d+)\.(?P<minor>\d+)\.(?P<patch>\d+)"""
     _pre = r"""((?P<prekind>a|b|rc)(?P<pre>\d+))?"""
     _nightly = r"""(\.(?P<nightly>[a-z0-9]+)?)?"""
-    _version_pattern = rf"""version\s*=\s*["']{_semver}{_pre}{_nightly}["']"""
+    _build = r"""(\+build[0-9]+)?"""
+    _version_pattern = rf"""version\s*=\s*["']{_semver}{_pre}{_nightly}{_build}["']"""
     with open(_version_path) as f:
         match = re.search(_version_pattern, f.read().strip())
         if match is None:
             raise ValueError(f"invalid version at {_version_path}")
         return match.groupdict()
 
 
 package_name = "dbt-snowflake"
-package_version = "1.8.0b1"
+package_version = "1.8.0b2"
 description = """The Snowflake adapter plugin for dbt"""
 
 setup(
     name=package_name,
     version=package_version,
     description=description,
     long_description=long_description,
@@ -57,14 +58,16 @@
     url="https://github.com/dbt-labs/dbt-snowflake",
     packages=find_namespace_packages(include=["dbt", "dbt.*"]),
     include_package_data=True,
     install_requires=[
         "dbt-common>=0.1.0a1,<2.0",
         "dbt-adapters>=0.1.0a1,<2.0",
         "snowflake-connector-python[secure-local-storage]~=3.0",
+        # add dbt-core to ensure backwards compatibility of installation, this is not a functional dependency
+        "dbt-core>=1.8.0a1",
         # installed via dbt-core but referenced directly; don't pin to avoid version conflicts with dbt-core
         "agate",
     ],
     zip_safe=False,
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "License :: OSI Approved :: Apache Software License",
```

