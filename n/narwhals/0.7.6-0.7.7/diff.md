# Comparing `tmp/narwhals-0.7.6.tar.gz` & `tmp/narwhals-0.7.7.tar.gz`

## Comparing `narwhals-0.7.6.tar` & `narwhals-0.7.7.tar`

### file list

```diff
@@ -1,93 +1,93 @@
--rw-r--r--   0        0        0      559 2020-02-02 00:00:00.000000 narwhals-0.7.6/.pre-commit-config.yaml
--rw-r--r--   0        0        0     1047 2020-02-02 00:00:00.000000 narwhals-0.7.6/CONTRIBUTING.md
--rw-r--r--   0        0        0     1143 2020-02-02 00:00:00.000000 narwhals-0.7.6/mkdocs.yml
--rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 narwhals-0.7.6/requirements-dev.txt
--rw-r--r--   0        0        0     5243 2020-02-02 00:00:00.000000 narwhals-0.7.6/.github/CODE_OF_CONDUCT.md
--rw-r--r--   0        0        0     2580 2020-02-02 00:00:00.000000 narwhals-0.7.6/.github/workflows/extremes.yml
--rw-r--r--   0        0        0      799 2020-02-02 00:00:00.000000 narwhals-0.7.6/.github/workflows/mkdocs.yml
--rw-r--r--   0        0        0     2638 2020-02-02 00:00:00.000000 narwhals-0.7.6/.github/workflows/publish_to_pypi.yml
--rw-r--r--   0        0        0     2000 2020-02-02 00:00:00.000000 narwhals-0.7.6/.github/workflows/pytest.yml
--rw-r--r--   0        0        0     1274 2020-02-02 00:00:00.000000 narwhals-0.7.6/docs/extending.md
--rw-r--r--   0        0        0     1323 2020-02-02 00:00:00.000000 narwhals-0.7.6/docs/generate_members.py
--rw-r--r--   0        0        0      635 2020-02-02 00:00:00.000000 narwhals-0.7.6/docs/index.md
--rw-r--r--   0        0        0      352 2020-02-02 00:00:00.000000 narwhals-0.7.6/docs/installation.md
--rw-r--r--   0        0        0     1114 2020-02-02 00:00:00.000000 narwhals-0.7.6/docs/quick_start.md
--rw-r--r--   0        0        0     1520 2020-02-02 00:00:00.000000 narwhals-0.7.6/docs/related.md
--rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 narwhals-0.7.6/docs/requirements-docs.txt
--rw-r--r--   0        0        0      558 2020-02-02 00:00:00.000000 narwhals-0.7.6/docs/roadmap.md
--rw-r--r--   0        0        0     1137 2020-02-02 00:00:00.000000 narwhals-0.7.6/docs/why.md
--rw-r--r--   0        0        0      485 2020-02-02 00:00:00.000000 narwhals-0.7.6/docs/api-reference/dataframe.md
--rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 narwhals-0.7.6/docs/api-reference/expressions.md
--rw-r--r--   0        0        0      408 2020-02-02 00:00:00.000000 narwhals-0.7.6/docs/api-reference/lazyframe.md
--rw-r--r--   0        0        0      341 2020-02-02 00:00:00.000000 narwhals-0.7.6/docs/api-reference/narwhals.md
--rw-r--r--   0        0        0      502 2020-02-02 00:00:00.000000 narwhals-0.7.6/docs/api-reference/series.md
--rwxr-xr-x   0        0        0   132699 2020-02-02 00:00:00.000000 narwhals-0.7.6/docs/assets/image.png
--rw-r--r--   0        0        0     4393 2020-02-02 00:00:00.000000 narwhals-0.7.6/docs/basics/column.md
--rw-r--r--   0        0        0     3625 2020-02-02 00:00:00.000000 narwhals-0.7.6/docs/basics/complete_example.md
--rw-r--r--   0        0        0     1601 2020-02-02 00:00:00.000000 narwhals-0.7.6/docs/basics/dataframe.md
--rw-r--r--   0        0        0      868 2020-02-02 00:00:00.000000 narwhals-0.7.6/narwhals/__init__.py
--rw-r--r--   0        0        0    46236 2020-02-02 00:00:00.000000 narwhals-0.7.6/narwhals/dataframe.py
--rw-r--r--   0        0        0      891 2020-02-02 00:00:00.000000 narwhals-0.7.6/narwhals/dependencies.py
--rw-r--r--   0        0        0     2791 2020-02-02 00:00:00.000000 narwhals-0.7.6/narwhals/dtypes.py
--rw-r--r--   0        0        0     9016 2020-02-02 00:00:00.000000 narwhals-0.7.6/narwhals/expression.py
--rw-r--r--   0        0        0      854 2020-02-02 00:00:00.000000 narwhals-0.7.6/narwhals/functions.py
--rw-r--r--   0        0        0     1155 2020-02-02 00:00:00.000000 narwhals-0.7.6/narwhals/group_by.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 narwhals-0.7.6/narwhals/py.typed
--rw-r--r--   0        0        0     2943 2020-02-02 00:00:00.000000 narwhals-0.7.6/narwhals/series.py
--rw-r--r--   0        0        0     3136 2020-02-02 00:00:00.000000 narwhals-0.7.6/narwhals/translate.py
--rw-r--r--   0        0        0      387 2020-02-02 00:00:00.000000 narwhals-0.7.6/narwhals/typing.py
--rw-r--r--   0        0        0     1124 2020-02-02 00:00:00.000000 narwhals-0.7.6/narwhals/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 narwhals-0.7.6/narwhals/_pandas_like/__init__.py
--rw-r--r--   0        0        0     7912 2020-02-02 00:00:00.000000 narwhals-0.7.6/narwhals/_pandas_like/dataframe.py
--rw-r--r--   0        0        0     8655 2020-02-02 00:00:00.000000 narwhals-0.7.6/narwhals/_pandas_like/expr.py
--rw-r--r--   0        0        0     5640 2020-02-02 00:00:00.000000 narwhals-0.7.6/narwhals/_pandas_like/group_by.py
--rw-r--r--   0        0        0     6324 2020-02-02 00:00:00.000000 narwhals-0.7.6/narwhals/_pandas_like/namespace.py
--rw-r--r--   0        0        0    11069 2020-02-02 00:00:00.000000 narwhals-0.7.6/narwhals/_pandas_like/series.py
--rw-r--r--   0        0        0      353 2020-02-02 00:00:00.000000 narwhals-0.7.6/narwhals/_pandas_like/typing.py
--rw-r--r--   0        0        0    12231 2020-02-02 00:00:00.000000 narwhals-0.7.6/narwhals/_pandas_like/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 narwhals-0.7.6/tests/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 narwhals-0.7.6/tests/group_by_test.py
--rw-r--r--   0        0        0    18342 2020-02-02 00:00:00.000000 narwhals-0.7.6/tests/test_common.py
--rw-r--r--   0        0        0      982 2020-02-02 00:00:00.000000 narwhals-0.7.6/tests/test_dt.py
--rw-r--r--   0        0        0     1232 2020-02-02 00:00:00.000000 narwhals-0.7.6/tests/test_group_by.py
--rw-r--r--   0        0        0      297 2020-02-02 00:00:00.000000 narwhals-0.7.6/tests/test_pandas.py
--rw-r--r--   0        0        0     6372 2020-02-02 00:00:00.000000 narwhals-0.7.6/tests/test_series.py
--rw-r--r--   0        0        0      924 2020-02-02 00:00:00.000000 narwhals-0.7.6/tests/test_str.py
--rw-r--r--   0        0        0     7354 2020-02-02 00:00:00.000000 narwhals-0.7.6/tests/tpch_q1_test.py
--rw-r--r--   0        0        0      888 2020-02-02 00:00:00.000000 narwhals-0.7.6/tests/utils.py
--rw-r--r--   0        0        0    21551 2020-02-02 00:00:00.000000 narwhals-0.7.6/tests/data/customer.parquet
--rw-r--r--   0        0        0    34095 2020-02-02 00:00:00.000000 narwhals-0.7.6/tests/data/lineitem.parquet
--rw-r--r--   0        0        0     2139 2020-02-02 00:00:00.000000 narwhals-0.7.6/tests/data/nation.parquet
--rw-r--r--   0        0        0    24714 2020-02-02 00:00:00.000000 narwhals-0.7.6/tests/data/orders.parquet
--rw-r--r--   0        0        0    13276 2020-02-02 00:00:00.000000 narwhals-0.7.6/tests/data/part.parquet
--rw-r--r--   0        0        0    14921 2020-02-02 00:00:00.000000 narwhals-0.7.6/tests/data/partsupp.parquet
--rw-r--r--   0        0        0     1131 2020-02-02 00:00:00.000000 narwhals-0.7.6/tests/data/region.parquet
--rw-r--r--   0        0        0    19817 2020-02-02 00:00:00.000000 narwhals-0.7.6/tests/data/supplier.parquet
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 narwhals-0.7.6/tpch/__init__.py
--rw-r--r--   0        0        0     1544 2020-02-02 00:00:00.000000 narwhals-0.7.6/tpch/q1.py
--rw-r--r--   0        0        0     2443 2020-02-02 00:00:00.000000 narwhals-0.7.6/tpch/q2.py
--rw-r--r--   0        0        0     1840 2020-02-02 00:00:00.000000 narwhals-0.7.6/tpch/q3.py
--rw-r--r--   0        0        0     1181 2020-02-02 00:00:00.000000 narwhals-0.7.6/tpch/q4.py
--rw-r--r--   0        0        0     2900 2020-02-02 00:00:00.000000 narwhals-0.7.6/tpch/q5.py
--rwxr-xr-x   0        0        0    47336 2020-02-02 00:00:00.000000 narwhals-0.7.6/tpch/notebooks/gpu/execute.ipynb
--rw-r--r--   0        0        0      408 2020-02-02 00:00:00.000000 narwhals-0.7.6/tpch/notebooks/gpu/kernel-metadata.json
--rwxr-xr-x   0        0        0    15160 2020-02-02 00:00:00.000000 narwhals-0.7.6/tpch/notebooks/q1/execute.ipynb
--rw-r--r--   0        0        0      407 2020-02-02 00:00:00.000000 narwhals-0.7.6/tpch/notebooks/q1/kernel-metadata.json
--rwxr-xr-x   0        0        0    16114 2020-02-02 00:00:00.000000 narwhals-0.7.6/tpch/notebooks/q2/execute.ipynb
--rw-r--r--   0        0        0      407 2020-02-02 00:00:00.000000 narwhals-0.7.6/tpch/notebooks/q2/kernel-metadata.json
--rwxr-xr-x   0        0        0    15420 2020-02-02 00:00:00.000000 narwhals-0.7.6/tpch/notebooks/q3/execute.ipynb
--rw-r--r--   0        0        0      407 2020-02-02 00:00:00.000000 narwhals-0.7.6/tpch/notebooks/q3/kernel-metadata.json
--rwxr-xr-x   0        0        0    14794 2020-02-02 00:00:00.000000 narwhals-0.7.6/tpch/notebooks/q4/execute.ipynb
--rw-r--r--   0        0        0      407 2020-02-02 00:00:00.000000 narwhals-0.7.6/tpch/notebooks/q4/kernel-metadata.json
--rwxr-xr-x   0        0        0    15844 2020-02-02 00:00:00.000000 narwhals-0.7.6/tpch/notebooks/q5/execute.ipynb
--rw-r--r--   0        0        0      407 2020-02-02 00:00:00.000000 narwhals-0.7.6/tpch/notebooks/q5/kernel-metadata.json
--rwxr-xr-x   0        0        0    14502 2020-02-02 00:00:00.000000 narwhals-0.7.6/tpch/notebooks/q6/execute.ipynb
--rw-r--r--   0        0        0      407 2020-02-02 00:00:00.000000 narwhals-0.7.6/tpch/notebooks/q6/kernel-metadata.json
--rwxr-xr-x   0        0        0    24376 2020-02-02 00:00:00.000000 narwhals-0.7.6/tpch/notebooks/q7/execute.ipynb
--rw-r--r--   0        0        0      407 2020-02-02 00:00:00.000000 narwhals-0.7.6/tpch/notebooks/q7/kernel-metadata.json
--rw-r--r--   0        0        0     1372 2020-02-02 00:00:00.000000 narwhals-0.7.6/utils/bump_version.py
--rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 narwhals-0.7.6/.gitignore
--rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 narwhals-0.7.6/LICENSE.md
--rw-r--r--   0        0        0     4550 2020-02-02 00:00:00.000000 narwhals-0.7.6/README.md
--rw-r--r--   0        0        0     1836 2020-02-02 00:00:00.000000 narwhals-0.7.6/pyproject.toml
--rw-r--r--   0        0        0     5136 2020-02-02 00:00:00.000000 narwhals-0.7.6/PKG-INFO
+-rw-r--r--   0        0        0      559 2020-02-02 00:00:00.000000 narwhals-0.7.7/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     1047 2020-02-02 00:00:00.000000 narwhals-0.7.7/CONTRIBUTING.md
+-rw-r--r--   0        0        0     1197 2020-02-02 00:00:00.000000 narwhals-0.7.7/mkdocs.yml
+-rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 narwhals-0.7.7/requirements-dev.txt
+-rw-r--r--   0        0        0     5243 2020-02-02 00:00:00.000000 narwhals-0.7.7/.github/CODE_OF_CONDUCT.md
+-rw-r--r--   0        0        0     2580 2020-02-02 00:00:00.000000 narwhals-0.7.7/.github/workflows/extremes.yml
+-rw-r--r--   0        0        0      799 2020-02-02 00:00:00.000000 narwhals-0.7.7/.github/workflows/mkdocs.yml
+-rw-r--r--   0        0        0     2638 2020-02-02 00:00:00.000000 narwhals-0.7.7/.github/workflows/publish_to_pypi.yml
+-rw-r--r--   0        0        0     2000 2020-02-02 00:00:00.000000 narwhals-0.7.7/.github/workflows/pytest.yml
+-rw-r--r--   0        0        0     1274 2020-02-02 00:00:00.000000 narwhals-0.7.7/docs/extending.md
+-rw-r--r--   0        0        0     1323 2020-02-02 00:00:00.000000 narwhals-0.7.7/docs/generate_members.py
+-rw-r--r--   0        0        0      635 2020-02-02 00:00:00.000000 narwhals-0.7.7/docs/index.md
+-rw-r--r--   0        0        0      352 2020-02-02 00:00:00.000000 narwhals-0.7.7/docs/installation.md
+-rw-r--r--   0        0        0     1114 2020-02-02 00:00:00.000000 narwhals-0.7.7/docs/quick_start.md
+-rw-r--r--   0        0        0     1520 2020-02-02 00:00:00.000000 narwhals-0.7.7/docs/related.md
+-rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 narwhals-0.7.7/docs/requirements-docs.txt
+-rw-r--r--   0        0        0      558 2020-02-02 00:00:00.000000 narwhals-0.7.7/docs/roadmap.md
+-rw-r--r--   0        0        0     1137 2020-02-02 00:00:00.000000 narwhals-0.7.7/docs/why.md
+-rw-r--r--   0        0        0      485 2020-02-02 00:00:00.000000 narwhals-0.7.7/docs/api-reference/dataframe.md
+-rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 narwhals-0.7.7/docs/api-reference/expressions.md
+-rw-r--r--   0        0        0      408 2020-02-02 00:00:00.000000 narwhals-0.7.7/docs/api-reference/lazyframe.md
+-rw-r--r--   0        0        0      341 2020-02-02 00:00:00.000000 narwhals-0.7.7/docs/api-reference/narwhals.md
+-rw-r--r--   0        0        0      502 2020-02-02 00:00:00.000000 narwhals-0.7.7/docs/api-reference/series.md
+-rwxr-xr-x   0        0        0   132699 2020-02-02 00:00:00.000000 narwhals-0.7.7/docs/assets/image.png
+-rw-r--r--   0        0        0     4393 2020-02-02 00:00:00.000000 narwhals-0.7.7/docs/basics/column.md
+-rw-r--r--   0        0        0     3625 2020-02-02 00:00:00.000000 narwhals-0.7.7/docs/basics/complete_example.md
+-rw-r--r--   0        0        0     1601 2020-02-02 00:00:00.000000 narwhals-0.7.7/docs/basics/dataframe.md
+-rw-r--r--   0        0        0      868 2020-02-02 00:00:00.000000 narwhals-0.7.7/narwhals/__init__.py
+-rw-r--r--   0        0        0    46236 2020-02-02 00:00:00.000000 narwhals-0.7.7/narwhals/dataframe.py
+-rw-r--r--   0        0        0      891 2020-02-02 00:00:00.000000 narwhals-0.7.7/narwhals/dependencies.py
+-rw-r--r--   0        0        0     2791 2020-02-02 00:00:00.000000 narwhals-0.7.7/narwhals/dtypes.py
+-rw-r--r--   0        0        0     9016 2020-02-02 00:00:00.000000 narwhals-0.7.7/narwhals/expression.py
+-rw-r--r--   0        0        0      854 2020-02-02 00:00:00.000000 narwhals-0.7.7/narwhals/functions.py
+-rw-r--r--   0        0        0     1155 2020-02-02 00:00:00.000000 narwhals-0.7.7/narwhals/group_by.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 narwhals-0.7.7/narwhals/py.typed
+-rw-r--r--   0        0        0     3067 2020-02-02 00:00:00.000000 narwhals-0.7.7/narwhals/series.py
+-rw-r--r--   0        0        0     3136 2020-02-02 00:00:00.000000 narwhals-0.7.7/narwhals/translate.py
+-rw-r--r--   0        0        0      387 2020-02-02 00:00:00.000000 narwhals-0.7.7/narwhals/typing.py
+-rw-r--r--   0        0        0     1124 2020-02-02 00:00:00.000000 narwhals-0.7.7/narwhals/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 narwhals-0.7.7/narwhals/_pandas_like/__init__.py
+-rw-r--r--   0        0        0     7912 2020-02-02 00:00:00.000000 narwhals-0.7.7/narwhals/_pandas_like/dataframe.py
+-rw-r--r--   0        0        0     8655 2020-02-02 00:00:00.000000 narwhals-0.7.7/narwhals/_pandas_like/expr.py
+-rw-r--r--   0        0        0     5640 2020-02-02 00:00:00.000000 narwhals-0.7.7/narwhals/_pandas_like/group_by.py
+-rw-r--r--   0        0        0     6324 2020-02-02 00:00:00.000000 narwhals-0.7.7/narwhals/_pandas_like/namespace.py
+-rw-r--r--   0        0        0    11222 2020-02-02 00:00:00.000000 narwhals-0.7.7/narwhals/_pandas_like/series.py
+-rw-r--r--   0        0        0      353 2020-02-02 00:00:00.000000 narwhals-0.7.7/narwhals/_pandas_like/typing.py
+-rw-r--r--   0        0        0    12231 2020-02-02 00:00:00.000000 narwhals-0.7.7/narwhals/_pandas_like/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 narwhals-0.7.7/tests/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 narwhals-0.7.7/tests/group_by_test.py
+-rw-r--r--   0        0        0    18342 2020-02-02 00:00:00.000000 narwhals-0.7.7/tests/test_common.py
+-rw-r--r--   0        0        0      982 2020-02-02 00:00:00.000000 narwhals-0.7.7/tests/test_dt.py
+-rw-r--r--   0        0        0     1232 2020-02-02 00:00:00.000000 narwhals-0.7.7/tests/test_group_by.py
+-rw-r--r--   0        0        0      297 2020-02-02 00:00:00.000000 narwhals-0.7.7/tests/test_pandas.py
+-rw-r--r--   0        0        0     6594 2020-02-02 00:00:00.000000 narwhals-0.7.7/tests/test_series.py
+-rw-r--r--   0        0        0      924 2020-02-02 00:00:00.000000 narwhals-0.7.7/tests/test_str.py
+-rw-r--r--   0        0        0     7354 2020-02-02 00:00:00.000000 narwhals-0.7.7/tests/tpch_q1_test.py
+-rw-r--r--   0        0        0      888 2020-02-02 00:00:00.000000 narwhals-0.7.7/tests/utils.py
+-rw-r--r--   0        0        0    21551 2020-02-02 00:00:00.000000 narwhals-0.7.7/tests/data/customer.parquet
+-rw-r--r--   0        0        0    34095 2020-02-02 00:00:00.000000 narwhals-0.7.7/tests/data/lineitem.parquet
+-rw-r--r--   0        0        0     2139 2020-02-02 00:00:00.000000 narwhals-0.7.7/tests/data/nation.parquet
+-rw-r--r--   0        0        0    24714 2020-02-02 00:00:00.000000 narwhals-0.7.7/tests/data/orders.parquet
+-rw-r--r--   0        0        0    13276 2020-02-02 00:00:00.000000 narwhals-0.7.7/tests/data/part.parquet
+-rw-r--r--   0        0        0    14921 2020-02-02 00:00:00.000000 narwhals-0.7.7/tests/data/partsupp.parquet
+-rw-r--r--   0        0        0     1131 2020-02-02 00:00:00.000000 narwhals-0.7.7/tests/data/region.parquet
+-rw-r--r--   0        0        0    19817 2020-02-02 00:00:00.000000 narwhals-0.7.7/tests/data/supplier.parquet
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 narwhals-0.7.7/tpch/__init__.py
+-rw-r--r--   0        0        0     1544 2020-02-02 00:00:00.000000 narwhals-0.7.7/tpch/q1.py
+-rw-r--r--   0        0        0     2443 2020-02-02 00:00:00.000000 narwhals-0.7.7/tpch/q2.py
+-rw-r--r--   0        0        0     1840 2020-02-02 00:00:00.000000 narwhals-0.7.7/tpch/q3.py
+-rw-r--r--   0        0        0     1181 2020-02-02 00:00:00.000000 narwhals-0.7.7/tpch/q4.py
+-rw-r--r--   0        0        0     2900 2020-02-02 00:00:00.000000 narwhals-0.7.7/tpch/q5.py
+-rwxr-xr-x   0        0        0    47336 2020-02-02 00:00:00.000000 narwhals-0.7.7/tpch/notebooks/gpu/execute.ipynb
+-rw-r--r--   0        0        0      408 2020-02-02 00:00:00.000000 narwhals-0.7.7/tpch/notebooks/gpu/kernel-metadata.json
+-rwxr-xr-x   0        0        0    15160 2020-02-02 00:00:00.000000 narwhals-0.7.7/tpch/notebooks/q1/execute.ipynb
+-rw-r--r--   0        0        0      407 2020-02-02 00:00:00.000000 narwhals-0.7.7/tpch/notebooks/q1/kernel-metadata.json
+-rwxr-xr-x   0        0        0    16114 2020-02-02 00:00:00.000000 narwhals-0.7.7/tpch/notebooks/q2/execute.ipynb
+-rw-r--r--   0        0        0      407 2020-02-02 00:00:00.000000 narwhals-0.7.7/tpch/notebooks/q2/kernel-metadata.json
+-rwxr-xr-x   0        0        0    15420 2020-02-02 00:00:00.000000 narwhals-0.7.7/tpch/notebooks/q3/execute.ipynb
+-rw-r--r--   0        0        0      407 2020-02-02 00:00:00.000000 narwhals-0.7.7/tpch/notebooks/q3/kernel-metadata.json
+-rwxr-xr-x   0        0        0    14794 2020-02-02 00:00:00.000000 narwhals-0.7.7/tpch/notebooks/q4/execute.ipynb
+-rw-r--r--   0        0        0      407 2020-02-02 00:00:00.000000 narwhals-0.7.7/tpch/notebooks/q4/kernel-metadata.json
+-rwxr-xr-x   0        0        0    15844 2020-02-02 00:00:00.000000 narwhals-0.7.7/tpch/notebooks/q5/execute.ipynb
+-rw-r--r--   0        0        0      407 2020-02-02 00:00:00.000000 narwhals-0.7.7/tpch/notebooks/q5/kernel-metadata.json
+-rwxr-xr-x   0        0        0    14502 2020-02-02 00:00:00.000000 narwhals-0.7.7/tpch/notebooks/q6/execute.ipynb
+-rw-r--r--   0        0        0      407 2020-02-02 00:00:00.000000 narwhals-0.7.7/tpch/notebooks/q6/kernel-metadata.json
+-rwxr-xr-x   0        0        0    24376 2020-02-02 00:00:00.000000 narwhals-0.7.7/tpch/notebooks/q7/execute.ipynb
+-rw-r--r--   0        0        0      407 2020-02-02 00:00:00.000000 narwhals-0.7.7/tpch/notebooks/q7/kernel-metadata.json
+-rw-r--r--   0        0        0     1372 2020-02-02 00:00:00.000000 narwhals-0.7.7/utils/bump_version.py
+-rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 narwhals-0.7.7/.gitignore
+-rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 narwhals-0.7.7/LICENSE.md
+-rw-r--r--   0        0        0     4550 2020-02-02 00:00:00.000000 narwhals-0.7.7/README.md
+-rw-r--r--   0        0        0     1836 2020-02-02 00:00:00.000000 narwhals-0.7.7/pyproject.toml
+-rw-r--r--   0        0        0     5136 2020-02-02 00:00:00.000000 narwhals-0.7.7/PKG-INFO
```

### Comparing `narwhals-0.7.6/.pre-commit-config.yaml` & `narwhals-0.7.7/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `narwhals-0.7.6/CONTRIBUTING.md` & `narwhals-0.7.7/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `narwhals-0.7.6/mkdocs.yml` & `narwhals-0.7.7/mkdocs.yml`

 * *Files 7% similar despite different names*

```diff
@@ -9,26 +9,28 @@
     - basics/dataframe.md
     - basics/column.md
     - basics/complete_example.md
   - Extending: extending.md
   - Roadmap: roadmap.md
   - Related projects: related.md
   - API Reference:
+    - api-reference/index.md
     - api-reference/narwhals.md
     - api-reference/dataframe.md
     - api-reference/lazyframe.md
     - api-reference/series.md
     - api-reference/expressions.md
 theme:
   name: material
   font: false
   features:
     - content.code.copy
     - content.code.annotate
     - navigation.footer
+    - navigation.indexes
 plugins:
 - search
 - mkdocstrings:
     handlers:
       python:
         import:
         - https://installer.readthedocs.io/en/stable/objects.inv
```

### Comparing `narwhals-0.7.6/.github/CODE_OF_CONDUCT.md` & `narwhals-0.7.7/.github/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `narwhals-0.7.6/.github/workflows/extremes.yml` & `narwhals-0.7.7/.github/workflows/extremes.yml`

 * *Files identical despite different names*

### Comparing `narwhals-0.7.6/.github/workflows/mkdocs.yml` & `narwhals-0.7.7/.github/workflows/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `narwhals-0.7.6/.github/workflows/publish_to_pypi.yml` & `narwhals-0.7.7/.github/workflows/publish_to_pypi.yml`

 * *Files identical despite different names*

### Comparing `narwhals-0.7.6/.github/workflows/pytest.yml` & `narwhals-0.7.7/.github/workflows/pytest.yml`

 * *Files identical despite different names*

### Comparing `narwhals-0.7.6/docs/extending.md` & `narwhals-0.7.7/docs/extending.md`

 * *Files identical despite different names*

### Comparing `narwhals-0.7.6/docs/generate_members.py` & `narwhals-0.7.7/docs/generate_members.py`

 * *Files identical despite different names*

### Comparing `narwhals-0.7.6/docs/index.md` & `narwhals-0.7.7/docs/index.md`

 * *Files identical despite different names*

### Comparing `narwhals-0.7.6/docs/quick_start.md` & `narwhals-0.7.7/docs/quick_start.md`

 * *Files identical despite different names*

### Comparing `narwhals-0.7.6/docs/related.md` & `narwhals-0.7.7/docs/related.md`

 * *Files identical despite different names*

### Comparing `narwhals-0.7.6/docs/roadmap.md` & `narwhals-0.7.7/docs/roadmap.md`

 * *Files identical despite different names*

### Comparing `narwhals-0.7.6/docs/why.md` & `narwhals-0.7.7/docs/why.md`

 * *Files identical despite different names*

### Comparing `narwhals-0.7.6/docs/assets/image.png` & `narwhals-0.7.7/docs/assets/image.png`

 * *Files identical despite different names*

### Comparing `narwhals-0.7.6/docs/basics/column.md` & `narwhals-0.7.7/docs/basics/column.md`

 * *Files identical despite different names*

### Comparing `narwhals-0.7.6/docs/basics/complete_example.md` & `narwhals-0.7.7/docs/basics/complete_example.md`

 * *Files identical despite different names*

### Comparing `narwhals-0.7.6/docs/basics/dataframe.md` & `narwhals-0.7.7/docs/basics/dataframe.md`

 * *Files identical despite different names*

### Comparing `narwhals-0.7.6/narwhals/__init__.py` & `narwhals-0.7.7/narwhals/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 from narwhals.expression import sum
 from narwhals.expression import sum_horizontal
 from narwhals.functions import concat
 from narwhals.series import Series
 from narwhals.translate import from_native
 from narwhals.translate import to_native
 
-__version__ = "0.7.6"
+__version__ = "0.7.7"
 
 __all__ = [
     "concat",
     "to_native",
     "from_native",
     "all",
     "col",
```

### Comparing `narwhals-0.7.6/narwhals/dataframe.py` & `narwhals-0.7.7/narwhals/dataframe.py`

 * *Files identical despite different names*

### Comparing `narwhals-0.7.6/narwhals/dependencies.py` & `narwhals-0.7.7/narwhals/dependencies.py`

 * *Files identical despite different names*

### Comparing `narwhals-0.7.6/narwhals/dtypes.py` & `narwhals-0.7.7/narwhals/dtypes.py`

 * *Files identical despite different names*

### Comparing `narwhals-0.7.6/narwhals/expression.py` & `narwhals-0.7.7/narwhals/expression.py`

 * *Files identical despite different names*

### Comparing `narwhals-0.7.6/narwhals/functions.py` & `narwhals-0.7.7/narwhals/functions.py`

 * *Files identical despite different names*

### Comparing `narwhals-0.7.6/narwhals/group_by.py` & `narwhals-0.7.7/narwhals/group_by.py`

 * *Files identical despite different names*

### Comparing `narwhals-0.7.6/narwhals/series.py` & `narwhals-0.7.7/narwhals/series.py`

 * *Files 12% similar despite different names*

```diff
@@ -79,14 +79,20 @@
         self,
         dtype: Any,
     ) -> Self:
         return self._from_series(
             self._series.cast(translate_dtype(self.__narwhals_namespace__(), dtype))
         )
 
+    def mean(self) -> Any:
+        return self._series.mean()
+
+    def std(self) -> Any:
+        return self._series.std()
+
     def is_in(self, other: Any) -> Self:
         return self._from_series(self._series.is_in(self._extract_native(other)))
 
     def sort(self) -> Self:
         return self._from_series(self._series.sort())
 
     def to_numpy(self) -> Any:
```

### Comparing `narwhals-0.7.6/narwhals/translate.py` & `narwhals-0.7.7/narwhals/translate.py`

 * *Files identical despite different names*

### Comparing `narwhals-0.7.6/narwhals/utils.py` & `narwhals-0.7.7/narwhals/utils.py`

 * *Files identical despite different names*

### Comparing `narwhals-0.7.6/narwhals/_pandas_like/dataframe.py` & `narwhals-0.7.7/narwhals/_pandas_like/dataframe.py`

 * *Files identical despite different names*

### Comparing `narwhals-0.7.6/narwhals/_pandas_like/expr.py` & `narwhals-0.7.7/narwhals/_pandas_like/expr.py`

 * *Files identical despite different names*

### Comparing `narwhals-0.7.6/narwhals/_pandas_like/group_by.py` & `narwhals-0.7.7/narwhals/_pandas_like/group_by.py`

 * *Files identical despite different names*

### Comparing `narwhals-0.7.6/narwhals/_pandas_like/namespace.py` & `narwhals-0.7.7/narwhals/_pandas_like/namespace.py`

 * *Files identical despite different names*

### Comparing `narwhals-0.7.6/narwhals/_pandas_like/series.py` & `narwhals-0.7.7/narwhals/_pandas_like/series.py`

 * *Files 3% similar despite different names*

```diff
@@ -253,14 +253,22 @@
         ser = self._series
         return ser.sum()
 
     def mean(self) -> Any:
         ser = self._series
         return ser.mean()
 
+    def std(
+        self,
+        *,
+        correction: float = 1.0,
+    ) -> Any:
+        ser = self._series
+        return ser.std(ddof=correction)
+
     def len(self) -> Any:
         return len(self._series)
 
     # Transformations
 
     def is_null(self) -> PandasSeries:
         ser = self._series
```

### Comparing `narwhals-0.7.6/narwhals/_pandas_like/utils.py` & `narwhals-0.7.7/narwhals/_pandas_like/utils.py`

 * *Files identical despite different names*

### Comparing `narwhals-0.7.6/tests/test_common.py` & `narwhals-0.7.7/tests/test_common.py`

 * *Files identical despite different names*

### Comparing `narwhals-0.7.6/tests/test_dt.py` & `narwhals-0.7.7/tests/test_dt.py`

 * *Files identical despite different names*

### Comparing `narwhals-0.7.6/tests/test_group_by.py` & `narwhals-0.7.7/tests/test_group_by.py`

 * *Files identical despite different names*

### Comparing `narwhals-0.7.6/tests/test_series.py` & `narwhals-0.7.7/tests/test_series.py`

 * *Files 9% similar despite different names*

```diff
@@ -49,14 +49,20 @@
 def test_dtype(df_raw: Any) -> None:
     result = nw.LazyFrame(df_raw).collect()["a"].dtype
     assert result == nw.Int64
     assert result.is_numeric()
 
 
 @pytest.mark.parametrize("df_raw", [df_pandas, df_lazy])
+def test_reductions(df_raw: Any) -> None:
+    assert nw.LazyFrame(df_raw).collect()["a"].mean() == 2.0
+    assert nw.LazyFrame(df_raw).collect()["a"].std() == 1.0
+
+
+@pytest.mark.parametrize("df_raw", [df_pandas, df_lazy])
 def test_convert(df_raw: Any) -> None:
     result = nw.LazyFrame(df_raw).collect()["a"].to_numpy()
     assert_array_equal(result, np.array([1, 3, 2]))
     result = nw.LazyFrame(df_raw).collect()["a"].to_pandas()
     assert_series_equal(result, pd.Series([1, 3, 2], name="a"))
```

### Comparing `narwhals-0.7.6/tests/test_str.py` & `narwhals-0.7.7/tests/test_str.py`

 * *Files identical despite different names*

### Comparing `narwhals-0.7.6/tests/tpch_q1_test.py` & `narwhals-0.7.7/tests/tpch_q1_test.py`

 * *Files identical despite different names*

### Comparing `narwhals-0.7.6/tests/utils.py` & `narwhals-0.7.7/tests/utils.py`

 * *Files identical despite different names*

### Comparing `narwhals-0.7.6/tests/data/customer.parquet` & `narwhals-0.7.7/tests/data/customer.parquet`

 * *Files identical despite different names*

### Comparing `narwhals-0.7.6/tests/data/lineitem.parquet` & `narwhals-0.7.7/tests/data/lineitem.parquet`

 * *Files identical despite different names*

### Comparing `narwhals-0.7.6/tests/data/nation.parquet` & `narwhals-0.7.7/tests/data/nation.parquet`

 * *Files identical despite different names*

### Comparing `narwhals-0.7.6/tests/data/orders.parquet` & `narwhals-0.7.7/tests/data/orders.parquet`

 * *Files identical despite different names*

### Comparing `narwhals-0.7.6/tests/data/part.parquet` & `narwhals-0.7.7/tests/data/part.parquet`

 * *Files identical despite different names*

### Comparing `narwhals-0.7.6/tests/data/partsupp.parquet` & `narwhals-0.7.7/tests/data/partsupp.parquet`

 * *Files identical despite different names*

### Comparing `narwhals-0.7.6/tests/data/region.parquet` & `narwhals-0.7.7/tests/data/region.parquet`

 * *Files identical despite different names*

### Comparing `narwhals-0.7.6/tests/data/supplier.parquet` & `narwhals-0.7.7/tests/data/supplier.parquet`

 * *Files identical despite different names*

### Comparing `narwhals-0.7.6/tpch/q1.py` & `narwhals-0.7.7/tpch/q1.py`

 * *Files identical despite different names*

### Comparing `narwhals-0.7.6/tpch/q2.py` & `narwhals-0.7.7/tpch/q2.py`

 * *Files identical despite different names*

### Comparing `narwhals-0.7.6/tpch/q3.py` & `narwhals-0.7.7/tpch/q3.py`

 * *Files identical despite different names*

### Comparing `narwhals-0.7.6/tpch/q4.py` & `narwhals-0.7.7/tpch/q4.py`

 * *Files identical despite different names*

### Comparing `narwhals-0.7.6/tpch/q5.py` & `narwhals-0.7.7/tpch/q5.py`

 * *Files identical despite different names*

### Comparing `narwhals-0.7.6/tpch/notebooks/gpu/execute.ipynb` & `narwhals-0.7.7/tpch/notebooks/gpu/execute.ipynb`

 * *Files identical despite different names*

### Comparing `narwhals-0.7.6/tpch/notebooks/q1/execute.ipynb` & `narwhals-0.7.7/tpch/notebooks/q1/execute.ipynb`

 * *Files identical despite different names*

### Comparing `narwhals-0.7.6/tpch/notebooks/q2/execute.ipynb` & `narwhals-0.7.7/tpch/notebooks/q2/execute.ipynb`

 * *Files identical despite different names*

### Comparing `narwhals-0.7.6/tpch/notebooks/q3/execute.ipynb` & `narwhals-0.7.7/tpch/notebooks/q3/execute.ipynb`

 * *Files identical despite different names*

### Comparing `narwhals-0.7.6/tpch/notebooks/q4/execute.ipynb` & `narwhals-0.7.7/tpch/notebooks/q4/execute.ipynb`

 * *Files identical despite different names*

### Comparing `narwhals-0.7.6/tpch/notebooks/q5/execute.ipynb` & `narwhals-0.7.7/tpch/notebooks/q5/execute.ipynb`

 * *Files identical despite different names*

### Comparing `narwhals-0.7.6/tpch/notebooks/q6/execute.ipynb` & `narwhals-0.7.7/tpch/notebooks/q6/execute.ipynb`

 * *Files identical despite different names*

### Comparing `narwhals-0.7.6/tpch/notebooks/q7/execute.ipynb` & `narwhals-0.7.7/tpch/notebooks/q7/execute.ipynb`

 * *Files identical despite different names*

### Comparing `narwhals-0.7.6/utils/bump_version.py` & `narwhals-0.7.7/utils/bump_version.py`

 * *Files identical despite different names*

### Comparing `narwhals-0.7.6/LICENSE.md` & `narwhals-0.7.7/LICENSE.md`

 * *Files identical despite different names*

### Comparing `narwhals-0.7.6/README.md` & `narwhals-0.7.7/README.md`

 * *Files identical despite different names*

### Comparing `narwhals-0.7.6/pyproject.toml` & `narwhals-0.7.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "narwhals"
-version = "0.7.6"
+version = "0.7.7"
 authors = [
   { name="Marco Gorelli", email="33491632+MarcoGorelli@users.noreply.github.com" },
 ]
 description = "Extremely lightweight compatibility layer between pandas, Polars, cuDF, and Modin"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `narwhals-0.7.6/PKG-INFO` & `narwhals-0.7.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: narwhals
-Version: 0.7.6
+Version: 0.7.7
 Summary: Extremely lightweight compatibility layer between pandas, Polars, cuDF, and Modin
 Project-URL: Homepage, https://github.com/MarcoGorelli/narwhals
 Project-URL: Bug Tracker, https://github.com/MarcoGorelli/narwhals
 Author-email: Marco Gorelli <33491632+MarcoGorelli@users.noreply.github.com>
 License-File: LICENSE.md
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

