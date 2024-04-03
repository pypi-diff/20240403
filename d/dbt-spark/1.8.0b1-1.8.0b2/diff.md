# Comparing `tmp/dbt-spark-1.8.0b1.tar.gz` & `tmp/dbt-spark-1.8.0b2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dbt-spark-1.8.0b1.tar", last modified: Sat Mar  2 03:14:19 2024, max compression
+gzip compressed data, was "dbt-spark-1.8.0b2.tar", last modified: Wed Apr  3 21:47:45 2024, max compression
```

## Comparing `dbt-spark-1.8.0b1.tar` & `dbt-spark-1.8.0b2.tar`

### file list

```diff
@@ -1,58 +1,58 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-02 03:14:19.728776 dbt-spark-1.8.0b1/
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-03-02 03:14:06.000000 dbt-spark-1.8.0b1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     5108 2024-03-02 03:14:19.728776 dbt-spark-1.8.0b1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3732 2024-03-02 03:14:06.000000 dbt-spark-1.8.0b1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-02 03:14:19.716776 dbt-spark-1.8.0b1/dbt/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-02 03:14:19.716776 dbt-spark-1.8.0b1/dbt/adapters/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-02 03:14:19.720776 dbt-spark-1.8.0b1/dbt/adapters/spark/
--rw-r--r--   0 runner    (1001) docker     (127)      509 2024-03-02 03:14:06.000000 dbt-spark-1.8.0b1/dbt/adapters/spark/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-03-02 03:14:06.000000 dbt-spark-1.8.0b1/dbt/adapters/spark/__version__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2592 2024-03-02 03:14:06.000000 dbt-spark-1.8.0b1/dbt/adapters/spark/column.py
--rw-r--r--   0 runner    (1001) docker     (127)    23885 2024-03-02 03:14:06.000000 dbt-spark-1.8.0b1/dbt/adapters/spark/connections.py
--rw-r--r--   0 runner    (1001) docker     (127)    20528 2024-03-02 03:14:06.000000 dbt-spark-1.8.0b1/dbt/adapters/spark/impl.py
--rw-r--r--   0 runner    (1001) docker     (127)    12031 2024-03-02 03:14:06.000000 dbt-spark-1.8.0b1/dbt/adapters/spark/python_submissions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1504 2024-03-02 03:14:06.000000 dbt-spark-1.8.0b1/dbt/adapters/spark/relation.py
--rw-r--r--   0 runner    (1001) docker     (127)     6712 2024-03-02 03:14:06.000000 dbt-spark-1.8.0b1/dbt/adapters/spark/session.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-02 03:14:19.716776 dbt-spark-1.8.0b1/dbt/include/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-02 03:14:19.720776 dbt-spark-1.8.0b1/dbt/include/spark/
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-03-02 03:14:06.000000 dbt-spark-1.8.0b1/dbt/include/spark/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       72 2024-03-02 03:14:06.000000 dbt-spark-1.8.0b1/dbt/include/spark/dbt_project.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-02 03:14:19.720776 dbt-spark-1.8.0b1/dbt/include/spark/macros/
--rw-r--r--   0 runner    (1001) docker     (127)    15838 2024-03-02 03:14:06.000000 dbt-spark-1.8.0b1/dbt/include/spark/macros/adapters.sql
--rw-r--r--   0 runner    (1001) docker     (127)     1212 2024-03-02 03:14:06.000000 dbt-spark-1.8.0b1/dbt/include/spark/macros/apply_grants.sql
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-02 03:14:19.720776 dbt-spark-1.8.0b1/dbt/include/spark/macros/materializations/
--rw-r--r--   0 runner    (1001) docker     (127)     3039 2024-03-02 03:14:06.000000 dbt-spark-1.8.0b1/dbt/include/spark/macros/materializations/clone.sql
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-02 03:14:19.724776 dbt-spark-1.8.0b1/dbt/include/spark/macros/materializations/incremental/
--rw-r--r--   0 runner    (1001) docker     (127)      876 2024-03-02 03:14:06.000000 dbt-spark-1.8.0b1/dbt/include/spark/macros/materializations/incremental/column_helpers.sql
--rw-r--r--   0 runner    (1001) docker     (127)     3747 2024-03-02 03:14:06.000000 dbt-spark-1.8.0b1/dbt/include/spark/macros/materializations/incremental/incremental.sql
--rw-r--r--   0 runner    (1001) docker     (127)     3812 2024-03-02 03:14:06.000000 dbt-spark-1.8.0b1/dbt/include/spark/macros/materializations/incremental/strategies.sql
--rw-r--r--   0 runner    (1001) docker     (127)     1884 2024-03-02 03:14:06.000000 dbt-spark-1.8.0b1/dbt/include/spark/macros/materializations/incremental/validate.sql
--rw-r--r--   0 runner    (1001) docker     (127)     2631 2024-03-02 03:14:06.000000 dbt-spark-1.8.0b1/dbt/include/spark/macros/materializations/seed.sql
--rw-r--r--   0 runner    (1001) docker     (127)     7333 2024-03-02 03:14:06.000000 dbt-spark-1.8.0b1/dbt/include/spark/macros/materializations/snapshot.sql
--rw-r--r--   0 runner    (1001) docker     (127)     4228 2024-03-02 03:14:06.000000 dbt-spark-1.8.0b1/dbt/include/spark/macros/materializations/table.sql
--rw-r--r--   0 runner    (1001) docker     (127)      114 2024-03-02 03:14:06.000000 dbt-spark-1.8.0b1/dbt/include/spark/macros/materializations/view.sql
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-02 03:14:19.724776 dbt-spark-1.8.0b1/dbt/include/spark/macros/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      139 2024-03-02 03:14:06.000000 dbt-spark-1.8.0b1/dbt/include/spark/macros/utils/any_value.sql
--rw-r--r--   0 runner    (1001) docker     (127)      131 2024-03-02 03:14:06.000000 dbt-spark-1.8.0b1/dbt/include/spark/macros/utils/array_append.sql
--rw-r--r--   0 runner    (1001) docker     (127)      108 2024-03-02 03:14:06.000000 dbt-spark-1.8.0b1/dbt/include/spark/macros/utils/array_concat.sql
--rw-r--r--   0 runner    (1001) docker     (127)      109 2024-03-02 03:14:06.000000 dbt-spark-1.8.0b1/dbt/include/spark/macros/utils/array_construct.sql
--rw-r--r--   0 runner    (1001) docker     (127)      321 2024-03-02 03:14:06.000000 dbt-spark-1.8.0b1/dbt/include/spark/macros/utils/assert_not_null.sql
--rw-r--r--   0 runner    (1001) docker     (127)      372 2024-03-02 03:14:06.000000 dbt-spark-1.8.0b1/dbt/include/spark/macros/utils/bool_or.sql
--rw-r--r--   0 runner    (1001) docker     (127)       87 2024-03-02 03:14:06.000000 dbt-spark-1.8.0b1/dbt/include/spark/macros/utils/concat.sql
--rw-r--r--   0 runner    (1001) docker     (127)     2125 2024-03-02 03:14:06.000000 dbt-spark-1.8.0b1/dbt/include/spark/macros/utils/dateadd.sql
--rw-r--r--   0 runner    (1001) docker     (127)     4604 2024-03-02 03:14:06.000000 dbt-spark-1.8.0b1/dbt/include/spark/macros/utils/datediff.sql
--rw-r--r--   0 runner    (1001) docker     (127)      230 2024-03-02 03:14:06.000000 dbt-spark-1.8.0b1/dbt/include/spark/macros/utils/escape_single_quotes.sql
--rw-r--r--   0 runner    (1001) docker     (127)      553 2024-03-02 03:14:06.000000 dbt-spark-1.8.0b1/dbt/include/spark/macros/utils/listagg.sql
--rw-r--r--   0 runner    (1001) docker     (127)      409 2024-03-02 03:14:06.000000 dbt-spark-1.8.0b1/dbt/include/spark/macros/utils/safe_cast.sql
--rw-r--r--   0 runner    (1001) docker     (127)     1034 2024-03-02 03:14:06.000000 dbt-spark-1.8.0b1/dbt/include/spark/macros/utils/split_part.sql
--rw-r--r--   0 runner    (1001) docker     (127)       80 2024-03-02 03:14:06.000000 dbt-spark-1.8.0b1/dbt/include/spark/macros/utils/timestamps.sql
--rw-r--r--   0 runner    (1001) docker     (127)      852 2024-03-02 03:14:06.000000 dbt-spark-1.8.0b1/dbt/include/spark/profile_template.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-02 03:14:19.728776 dbt-spark-1.8.0b1/dbt_spark.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5108 2024-03-02 03:14:19.000000 dbt-spark-1.8.0b1/dbt_spark.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1857 2024-03-02 03:14:19.000000 dbt-spark-1.8.0b1/dbt_spark.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-02 03:14:19.000000 dbt-spark-1.8.0b1/dbt_spark.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-02 03:14:19.000000 dbt-spark-1.8.0b1/dbt_spark.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      285 2024-03-02 03:14:19.000000 dbt-spark-1.8.0b1/dbt_spark.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        4 2024-03-02 03:14:19.000000 dbt-spark-1.8.0b1/dbt_spark.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-02 03:14:19.728776 dbt-spark-1.8.0b1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     3019 2024-03-02 03:14:06.000000 dbt-spark-1.8.0b1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 21:47:45.289870 dbt-spark-1.8.0b2/
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-03 21:47:33.000000 dbt-spark-1.8.0b2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     5141 2024-04-03 21:47:45.285870 dbt-spark-1.8.0b2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3732 2024-04-03 21:47:33.000000 dbt-spark-1.8.0b2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 21:47:45.277870 dbt-spark-1.8.0b2/dbt/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 21:47:45.273870 dbt-spark-1.8.0b2/dbt/adapters/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 21:47:45.277870 dbt-spark-1.8.0b2/dbt/adapters/spark/
+-rw-r--r--   0 runner    (1001) docker     (127)      509 2024-04-03 21:47:33.000000 dbt-spark-1.8.0b2/dbt/adapters/spark/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-03 21:47:33.000000 dbt-spark-1.8.0b2/dbt/adapters/spark/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2592 2024-04-03 21:47:33.000000 dbt-spark-1.8.0b2/dbt/adapters/spark/column.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23885 2024-04-03 21:47:33.000000 dbt-spark-1.8.0b2/dbt/adapters/spark/connections.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20528 2024-04-03 21:47:33.000000 dbt-spark-1.8.0b2/dbt/adapters/spark/impl.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12031 2024-04-03 21:47:33.000000 dbt-spark-1.8.0b2/dbt/adapters/spark/python_submissions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1504 2024-04-03 21:47:33.000000 dbt-spark-1.8.0b2/dbt/adapters/spark/relation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6712 2024-04-03 21:47:33.000000 dbt-spark-1.8.0b2/dbt/adapters/spark/session.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 21:47:45.277870 dbt-spark-1.8.0b2/dbt/include/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 21:47:45.277870 dbt-spark-1.8.0b2/dbt/include/spark/
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-03 21:47:33.000000 dbt-spark-1.8.0b2/dbt/include/spark/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-04-03 21:47:33.000000 dbt-spark-1.8.0b2/dbt/include/spark/dbt_project.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 21:47:45.281870 dbt-spark-1.8.0b2/dbt/include/spark/macros/
+-rw-r--r--   0 runner    (1001) docker     (127)    15838 2024-04-03 21:47:33.000000 dbt-spark-1.8.0b2/dbt/include/spark/macros/adapters.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     1212 2024-04-03 21:47:33.000000 dbt-spark-1.8.0b2/dbt/include/spark/macros/apply_grants.sql
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 21:47:45.281870 dbt-spark-1.8.0b2/dbt/include/spark/macros/materializations/
+-rw-r--r--   0 runner    (1001) docker     (127)     3039 2024-04-03 21:47:33.000000 dbt-spark-1.8.0b2/dbt/include/spark/macros/materializations/clone.sql
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 21:47:45.281870 dbt-spark-1.8.0b2/dbt/include/spark/macros/materializations/incremental/
+-rw-r--r--   0 runner    (1001) docker     (127)      876 2024-04-03 21:47:33.000000 dbt-spark-1.8.0b2/dbt/include/spark/macros/materializations/incremental/column_helpers.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     3747 2024-04-03 21:47:33.000000 dbt-spark-1.8.0b2/dbt/include/spark/macros/materializations/incremental/incremental.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     3812 2024-04-03 21:47:33.000000 dbt-spark-1.8.0b2/dbt/include/spark/macros/materializations/incremental/strategies.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     1884 2024-04-03 21:47:33.000000 dbt-spark-1.8.0b2/dbt/include/spark/macros/materializations/incremental/validate.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     2631 2024-04-03 21:47:33.000000 dbt-spark-1.8.0b2/dbt/include/spark/macros/materializations/seed.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     7333 2024-04-03 21:47:33.000000 dbt-spark-1.8.0b2/dbt/include/spark/macros/materializations/snapshot.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     4228 2024-04-03 21:47:33.000000 dbt-spark-1.8.0b2/dbt/include/spark/macros/materializations/table.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      114 2024-04-03 21:47:33.000000 dbt-spark-1.8.0b2/dbt/include/spark/macros/materializations/view.sql
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 21:47:45.285870 dbt-spark-1.8.0b2/dbt/include/spark/macros/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      139 2024-04-03 21:47:33.000000 dbt-spark-1.8.0b2/dbt/include/spark/macros/utils/any_value.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      131 2024-04-03 21:47:33.000000 dbt-spark-1.8.0b2/dbt/include/spark/macros/utils/array_append.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      108 2024-04-03 21:47:33.000000 dbt-spark-1.8.0b2/dbt/include/spark/macros/utils/array_concat.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      109 2024-04-03 21:47:33.000000 dbt-spark-1.8.0b2/dbt/include/spark/macros/utils/array_construct.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      321 2024-04-03 21:47:33.000000 dbt-spark-1.8.0b2/dbt/include/spark/macros/utils/assert_not_null.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      372 2024-04-03 21:47:33.000000 dbt-spark-1.8.0b2/dbt/include/spark/macros/utils/bool_or.sql
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-04-03 21:47:33.000000 dbt-spark-1.8.0b2/dbt/include/spark/macros/utils/concat.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     2125 2024-04-03 21:47:33.000000 dbt-spark-1.8.0b2/dbt/include/spark/macros/utils/dateadd.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     4604 2024-04-03 21:47:33.000000 dbt-spark-1.8.0b2/dbt/include/spark/macros/utils/datediff.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      230 2024-04-03 21:47:33.000000 dbt-spark-1.8.0b2/dbt/include/spark/macros/utils/escape_single_quotes.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      553 2024-04-03 21:47:33.000000 dbt-spark-1.8.0b2/dbt/include/spark/macros/utils/listagg.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      409 2024-04-03 21:47:33.000000 dbt-spark-1.8.0b2/dbt/include/spark/macros/utils/safe_cast.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     1034 2024-04-03 21:47:33.000000 dbt-spark-1.8.0b2/dbt/include/spark/macros/utils/split_part.sql
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2024-04-03 21:47:33.000000 dbt-spark-1.8.0b2/dbt/include/spark/macros/utils/timestamps.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      852 2024-04-03 21:47:33.000000 dbt-spark-1.8.0b2/dbt/include/spark/profile_template.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 21:47:45.285870 dbt-spark-1.8.0b2/dbt_spark.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5141 2024-04-03 21:47:45.000000 dbt-spark-1.8.0b2/dbt_spark.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1857 2024-04-03 21:47:45.000000 dbt-spark-1.8.0b2/dbt_spark.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 21:47:45.000000 dbt-spark-1.8.0b2/dbt_spark.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 21:47:45.000000 dbt-spark-1.8.0b2/dbt_spark.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      303 2024-04-03 21:47:45.000000 dbt-spark-1.8.0b2/dbt_spark.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-04-03 21:47:45.000000 dbt-spark-1.8.0b2/dbt_spark.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-03 21:47:45.289870 dbt-spark-1.8.0b2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3203 2024-04-03 21:47:33.000000 dbt-spark-1.8.0b2/setup.py
```

### Comparing `dbt-spark-1.8.0b1/PKG-INFO` & `dbt-spark-1.8.0b2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbt-spark
-Version: 1.8.0b1
+Version: 1.8.0b2
 Summary: The Apache Spark adapter plugin for dbt
 Home-page: https://github.com/dbt-labs/dbt-spark
 Author: dbt Labs
 Author-email: info@dbtlabs.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: Microsoft :: Windows
@@ -15,14 +15,15 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Requires-Dist: sqlparams>=3.0.0
 Requires-Dist: dbt-common<2.0,>=0.1.0a1
 Requires-Dist: dbt-adapters<2.0,>=0.1.0a1
+Requires-Dist: dbt-core>=1.8.0a1
 Provides-Extra: odbc
 Requires-Dist: pyodbc~=4.0.39; extra == "odbc"
 Provides-Extra: pyhive
 Requires-Dist: PyHive[hive_pure_sasl]~=0.7.0; extra == "pyhive"
 Requires-Dist: thrift<0.17.0,>=0.11.0; extra == "pyhive"
 Provides-Extra: session
 Requires-Dist: pyspark<4.0.0,>=3.0.0; extra == "session"
```

#### html2text {}

```diff
@@ -1,21 +1,21 @@
-Metadata-Version: 2.1 Name: dbt-spark Version: 1.8.0b1 Summary: The Apache
+Metadata-Version: 2.1 Name: dbt-spark Version: 1.8.0b2 Summary: The Apache
 Spark adapter plugin for dbt Home-page: https://github.com/dbt-labs/dbt-spark
 Author: dbt Labs Author-email: info@dbtlabs.com Classifier: Development Status
 :: 5 - Production/Stable Classifier: License :: OSI Approved :: Apache Software
 License Classifier: Operating System :: Microsoft :: Windows Classifier:
 Operating System :: MacOS :: MacOS X Classifier: Operating System :: POSIX ::
 Linux Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
 Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11 Requires-Python: >=3.8
 Description-Content-Type: text/markdown Requires-Dist: sqlparams>=3.0.0
 Requires-Dist: dbt-common<2.0,>=0.1.0a1 Requires-Dist: dbt-
-adapters<2.0,>=0.1.0a1 Provides-Extra: odbc Requires-Dist: pyodbc~=4.0.39;
-extra == "odbc" Provides-Extra: pyhive Requires-Dist: PyHive
-[hive_pure_sasl]~=0.7.0; extra == "pyhive" Requires-Dist:
+adapters<2.0,>=0.1.0a1 Requires-Dist: dbt-core>=1.8.0a1 Provides-Extra: odbc
+Requires-Dist: pyodbc~=4.0.39; extra == "odbc" Provides-Extra: pyhive Requires-
+Dist: PyHive[hive_pure_sasl]~=0.7.0; extra == "pyhive" Requires-Dist:
 thrift<0.17.0,>=0.11.0; extra == "pyhive" Provides-Extra: session Requires-
 Dist: pyspark<4.0.0,>=3.0.0; extra == "session" Provides-Extra: all Requires-
 Dist: pyodbc~=4.0.39; extra == "all" Requires-Dist: PyHive
 [hive_pure_sasl]~=0.7.0; extra == "all" Requires-Dist: thrift<0.17.0,>=0.11.0;
 extra == "all" Requires-Dist: pyspark<4.0.0,>=3.0.0; extra == "all"
                                   [dbt logo]
                               _[_U_n_i_t_ _T_e_s_t_s_ _B_a_d_g_e_]
```

### Comparing `dbt-spark-1.8.0b1/README.md` & `dbt-spark-1.8.0b2/README.md`

 * *Files identical despite different names*

### Comparing `dbt-spark-1.8.0b1/dbt/adapters/spark/column.py` & `dbt-spark-1.8.0b2/dbt/adapters/spark/column.py`

 * *Files identical despite different names*

### Comparing `dbt-spark-1.8.0b1/dbt/adapters/spark/connections.py` & `dbt-spark-1.8.0b2/dbt/adapters/spark/connections.py`

 * *Files identical despite different names*

### Comparing `dbt-spark-1.8.0b1/dbt/adapters/spark/impl.py` & `dbt-spark-1.8.0b2/dbt/adapters/spark/impl.py`

 * *Files identical despite different names*

### Comparing `dbt-spark-1.8.0b1/dbt/adapters/spark/python_submissions.py` & `dbt-spark-1.8.0b2/dbt/adapters/spark/python_submissions.py`

 * *Files identical despite different names*

### Comparing `dbt-spark-1.8.0b1/dbt/adapters/spark/relation.py` & `dbt-spark-1.8.0b2/dbt/adapters/spark/relation.py`

 * *Files identical despite different names*

### Comparing `dbt-spark-1.8.0b1/dbt/adapters/spark/session.py` & `dbt-spark-1.8.0b2/dbt/adapters/spark/session.py`

 * *Files identical despite different names*

### Comparing `dbt-spark-1.8.0b1/dbt/include/spark/macros/adapters.sql` & `dbt-spark-1.8.0b2/dbt/include/spark/macros/adapters.sql`

 * *Files identical despite different names*

### Comparing `dbt-spark-1.8.0b1/dbt/include/spark/macros/apply_grants.sql` & `dbt-spark-1.8.0b2/dbt/include/spark/macros/apply_grants.sql`

 * *Files identical despite different names*

### Comparing `dbt-spark-1.8.0b1/dbt/include/spark/macros/materializations/clone.sql` & `dbt-spark-1.8.0b2/dbt/include/spark/macros/materializations/clone.sql`

 * *Files identical despite different names*

### Comparing `dbt-spark-1.8.0b1/dbt/include/spark/macros/materializations/incremental/column_helpers.sql` & `dbt-spark-1.8.0b2/dbt/include/spark/macros/materializations/incremental/column_helpers.sql`

 * *Files identical despite different names*

### Comparing `dbt-spark-1.8.0b1/dbt/include/spark/macros/materializations/incremental/incremental.sql` & `dbt-spark-1.8.0b2/dbt/include/spark/macros/materializations/incremental/incremental.sql`

 * *Files identical despite different names*

### Comparing `dbt-spark-1.8.0b1/dbt/include/spark/macros/materializations/incremental/strategies.sql` & `dbt-spark-1.8.0b2/dbt/include/spark/macros/materializations/incremental/strategies.sql`

 * *Files identical despite different names*

### Comparing `dbt-spark-1.8.0b1/dbt/include/spark/macros/materializations/incremental/validate.sql` & `dbt-spark-1.8.0b2/dbt/include/spark/macros/materializations/incremental/validate.sql`

 * *Files identical despite different names*

### Comparing `dbt-spark-1.8.0b1/dbt/include/spark/macros/materializations/seed.sql` & `dbt-spark-1.8.0b2/dbt/include/spark/macros/materializations/seed.sql`

 * *Files identical despite different names*

### Comparing `dbt-spark-1.8.0b1/dbt/include/spark/macros/materializations/snapshot.sql` & `dbt-spark-1.8.0b2/dbt/include/spark/macros/materializations/snapshot.sql`

 * *Files identical despite different names*

### Comparing `dbt-spark-1.8.0b1/dbt/include/spark/macros/materializations/table.sql` & `dbt-spark-1.8.0b2/dbt/include/spark/macros/materializations/table.sql`

 * *Files identical despite different names*

### Comparing `dbt-spark-1.8.0b1/dbt/include/spark/macros/utils/dateadd.sql` & `dbt-spark-1.8.0b2/dbt/include/spark/macros/utils/dateadd.sql`

 * *Files identical despite different names*

### Comparing `dbt-spark-1.8.0b1/dbt/include/spark/macros/utils/datediff.sql` & `dbt-spark-1.8.0b2/dbt/include/spark/macros/utils/datediff.sql`

 * *Files identical despite different names*

### Comparing `dbt-spark-1.8.0b1/dbt/include/spark/macros/utils/listagg.sql` & `dbt-spark-1.8.0b2/dbt/include/spark/macros/utils/listagg.sql`

 * *Files identical despite different names*

### Comparing `dbt-spark-1.8.0b1/dbt/include/spark/macros/utils/split_part.sql` & `dbt-spark-1.8.0b2/dbt/include/spark/macros/utils/split_part.sql`

 * *Files identical despite different names*

### Comparing `dbt-spark-1.8.0b1/dbt/include/spark/profile_template.yml` & `dbt-spark-1.8.0b2/dbt/include/spark/profile_template.yml`

 * *Files identical despite different names*

### Comparing `dbt-spark-1.8.0b1/dbt_spark.egg-info/PKG-INFO` & `dbt-spark-1.8.0b2/dbt_spark.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbt-spark
-Version: 1.8.0b1
+Version: 1.8.0b2
 Summary: The Apache Spark adapter plugin for dbt
 Home-page: https://github.com/dbt-labs/dbt-spark
 Author: dbt Labs
 Author-email: info@dbtlabs.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: Microsoft :: Windows
@@ -15,14 +15,15 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Requires-Dist: sqlparams>=3.0.0
 Requires-Dist: dbt-common<2.0,>=0.1.0a1
 Requires-Dist: dbt-adapters<2.0,>=0.1.0a1
+Requires-Dist: dbt-core>=1.8.0a1
 Provides-Extra: odbc
 Requires-Dist: pyodbc~=4.0.39; extra == "odbc"
 Provides-Extra: pyhive
 Requires-Dist: PyHive[hive_pure_sasl]~=0.7.0; extra == "pyhive"
 Requires-Dist: thrift<0.17.0,>=0.11.0; extra == "pyhive"
 Provides-Extra: session
 Requires-Dist: pyspark<4.0.0,>=3.0.0; extra == "session"
```

#### html2text {}

```diff
@@ -1,21 +1,21 @@
-Metadata-Version: 2.1 Name: dbt-spark Version: 1.8.0b1 Summary: The Apache
+Metadata-Version: 2.1 Name: dbt-spark Version: 1.8.0b2 Summary: The Apache
 Spark adapter plugin for dbt Home-page: https://github.com/dbt-labs/dbt-spark
 Author: dbt Labs Author-email: info@dbtlabs.com Classifier: Development Status
 :: 5 - Production/Stable Classifier: License :: OSI Approved :: Apache Software
 License Classifier: Operating System :: Microsoft :: Windows Classifier:
 Operating System :: MacOS :: MacOS X Classifier: Operating System :: POSIX ::
 Linux Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
 Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11 Requires-Python: >=3.8
 Description-Content-Type: text/markdown Requires-Dist: sqlparams>=3.0.0
 Requires-Dist: dbt-common<2.0,>=0.1.0a1 Requires-Dist: dbt-
-adapters<2.0,>=0.1.0a1 Provides-Extra: odbc Requires-Dist: pyodbc~=4.0.39;
-extra == "odbc" Provides-Extra: pyhive Requires-Dist: PyHive
-[hive_pure_sasl]~=0.7.0; extra == "pyhive" Requires-Dist:
+adapters<2.0,>=0.1.0a1 Requires-Dist: dbt-core>=1.8.0a1 Provides-Extra: odbc
+Requires-Dist: pyodbc~=4.0.39; extra == "odbc" Provides-Extra: pyhive Requires-
+Dist: PyHive[hive_pure_sasl]~=0.7.0; extra == "pyhive" Requires-Dist:
 thrift<0.17.0,>=0.11.0; extra == "pyhive" Provides-Extra: session Requires-
 Dist: pyspark<4.0.0,>=3.0.0; extra == "session" Provides-Extra: all Requires-
 Dist: pyodbc~=4.0.39; extra == "all" Requires-Dist: PyHive
 [hive_pure_sasl]~=0.7.0; extra == "all" Requires-Dist: thrift<0.17.0,>=0.11.0;
 extra == "all" Requires-Dist: pyspark<4.0.0,>=3.0.0; extra == "all"
                                   [dbt logo]
                               _[_U_n_i_t_ _T_e_s_t_s_ _B_a_d_g_e_]
```

### Comparing `dbt-spark-1.8.0b1/dbt_spark.egg-info/SOURCES.txt` & `dbt-spark-1.8.0b2/dbt_spark.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dbt-spark-1.8.0b1/setup.py` & `dbt-spark-1.8.0b2/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -27,24 +27,25 @@
 
 
 # get this package's version from dbt/adapters/<name>/__version__.py
 def _get_plugin_version_dict():
     _version_path = os.path.join(this_directory, "dbt", "adapters", "spark", "__version__.py")
     _semver = r"""(?P<major>\d+)\.(?P<minor>\d+)\.(?P<patch>\d+)"""
     _pre = r"""((?P<prekind>a|b|rc)(?P<pre>\d+))?"""
-    _version_pattern = rf"""version\s*=\s*["']{_semver}{_pre}["']"""
+    _build = r"""(\+build[0-9]+)?"""
+    _version_pattern = rf"""version\s*=\s*["']{_semver}{_pre}{_build}["']"""
     with open(_version_path) as f:
         match = re.search(_version_pattern, f.read().strip())
         if match is None:
             raise ValueError(f"invalid version at {_version_path}")
         return match.groupdict()
 
 
 package_name = "dbt-spark"
-package_version = "1.8.0b1"
+package_version = "1.8.0b2"
 description = """The Apache Spark adapter plugin for dbt"""
 
 odbc_extras = ["pyodbc~=4.0.39"]
 pyhive_extras = [
     "PyHive[hive_pure_sasl]~=0.7.0",
     "thrift>=0.11.0,<0.17.0",
 ]
@@ -62,14 +63,16 @@
     url="https://github.com/dbt-labs/dbt-spark",
     packages=find_namespace_packages(include=["dbt", "dbt.*"]),
     include_package_data=True,
     install_requires=[
         "sqlparams>=3.0.0",
         "dbt-common>=0.1.0a1,<2.0",
         "dbt-adapters>=0.1.0a1,<2.0",
+        # add dbt-core to ensure backwards compatibility of installation, this is not a functional dependency
+        "dbt-core>=1.8.0a1",
     ],
     extras_require={
         "ODBC": odbc_extras,
         "PyHive": pyhive_extras,
         "session": session_extras,
         "all": all_extras,
     },
```

