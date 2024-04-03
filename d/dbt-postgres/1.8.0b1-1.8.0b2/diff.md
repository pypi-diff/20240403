# Comparing `tmp/dbt_postgres-1.8.0b1.tar.gz` & `tmp/dbt_postgres-1.8.0b2.tar.gz`

## Comparing `dbt_postgres-1.8.0b1.tar` & `dbt_postgres-1.8.0b2.tar`

### file list

```diff
@@ -1,45 +1,46 @@
--rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 dbt_postgres-1.8.0b1/dbt/__init__.py
--rw-r--r--   0        0        0      492 2020-02-02 00:00:00.000000 dbt_postgres-1.8.0b1/dbt/adapters/postgres/__init__.py
--rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 dbt_postgres-1.8.0b1/dbt/adapters/postgres/__version__.py
--rw-r--r--   0        0        0      381 2020-02-02 00:00:00.000000 dbt_postgres-1.8.0b1/dbt/adapters/postgres/column.py
--rw-r--r--   0        0        0     7221 2020-02-02 00:00:00.000000 dbt_postgres-1.8.0b1/dbt/adapters/postgres/connections.py
--rw-r--r--   0        0        0     5688 2020-02-02 00:00:00.000000 dbt_postgres-1.8.0b1/dbt/adapters/postgres/impl.py
--rw-r--r--   0        0        0     3857 2020-02-02 00:00:00.000000 dbt_postgres-1.8.0b1/dbt/adapters/postgres/relation.py
--rw-r--r--   0        0        0      377 2020-02-02 00:00:00.000000 dbt_postgres-1.8.0b1/dbt/adapters/postgres/relation_configs/__init__.py
--rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 dbt_postgres-1.8.0b1/dbt/adapters/postgres/relation_configs/constants.py
--rw-r--r--   0        0        0     5720 2020-02-02 00:00:00.000000 dbt_postgres-1.8.0b1/dbt/adapters/postgres/relation_configs/index.py
--rw-r--r--   0        0        0     4158 2020-02-02 00:00:00.000000 dbt_postgres-1.8.0b1/dbt/adapters/postgres/relation_configs/materialized_view.py
--rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 dbt_postgres-1.8.0b1/dbt/include/postgres/__init__.py
--rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 dbt_postgres-1.8.0b1/dbt/include/postgres/dbt_project.yml
--rw-r--r--   0        0        0      410 2020-02-02 00:00:00.000000 dbt_postgres-1.8.0b1/dbt/include/postgres/profile_template.yml
--rw-r--r--   0        0        0      439 2020-02-02 00:00:00.000000 dbt_postgres-1.8.0b1/dbt/include/postgres/sample_profiles.yml
--rw-r--r--   0        0        0     9374 2020-02-02 00:00:00.000000 dbt_postgres-1.8.0b1/dbt/include/postgres/macros/adapters.sql
--rw-r--r--   0        0        0     2852 2020-02-02 00:00:00.000000 dbt_postgres-1.8.0b1/dbt/include/postgres/macros/catalog.sql
--rw-r--r--   0        0        0     2706 2020-02-02 00:00:00.000000 dbt_postgres-1.8.0b1/dbt/include/postgres/macros/relations.sql
--rw-r--r--   0        0        0      620 2020-02-02 00:00:00.000000 dbt_postgres-1.8.0b1/dbt/include/postgres/macros/timestamps.sql
--rw-r--r--   0        0        0      261 2020-02-02 00:00:00.000000 dbt_postgres-1.8.0b1/dbt/include/postgres/macros/materializations/incremental_strategies.sql
--rw-r--r--   0        0        0      794 2020-02-02 00:00:00.000000 dbt_postgres-1.8.0b1/dbt/include/postgres/macros/materializations/snapshot_merge.sql
--rw-r--r--   0        0        0     1534 2020-02-02 00:00:00.000000 dbt_postgres-1.8.0b1/dbt/include/postgres/macros/relations/materialized_view/alter.sql
--rw-r--r--   0        0        0      297 2020-02-02 00:00:00.000000 dbt_postgres-1.8.0b1/dbt/include/postgres/macros/relations/materialized_view/create.sql
--rw-r--r--   0        0        0      261 2020-02-02 00:00:00.000000 dbt_postgres-1.8.0b1/dbt/include/postgres/macros/relations/materialized_view/describe.sql
--rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 dbt_postgres-1.8.0b1/dbt/include/postgres/macros/relations/materialized_view/drop.sql
--rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 dbt_postgres-1.8.0b1/dbt/include/postgres/macros/relations/materialized_view/refresh.sql
--rw-r--r--   0        0        0      158 2020-02-02 00:00:00.000000 dbt_postgres-1.8.0b1/dbt/include/postgres/macros/relations/materialized_view/rename.sql
--rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 dbt_postgres-1.8.0b1/dbt/include/postgres/macros/relations/table/drop.sql
--rw-r--r--   0        0        0      134 2020-02-02 00:00:00.000000 dbt_postgres-1.8.0b1/dbt/include/postgres/macros/relations/table/rename.sql
--rw-r--r--   0        0        0      545 2020-02-02 00:00:00.000000 dbt_postgres-1.8.0b1/dbt/include/postgres/macros/relations/table/replace.sql
--rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 dbt_postgres-1.8.0b1/dbt/include/postgres/macros/relations/view/drop.sql
--rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 dbt_postgres-1.8.0b1/dbt/include/postgres/macros/relations/view/rename.sql
--rw-r--r--   0        0        0      436 2020-02-02 00:00:00.000000 dbt_postgres-1.8.0b1/dbt/include/postgres/macros/relations/view/replace.sql
--rw-r--r--   0        0        0      182 2020-02-02 00:00:00.000000 dbt_postgres-1.8.0b1/dbt/include/postgres/macros/utils/any_value.sql
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dbt_postgres-1.8.0b1/dbt/include/postgres/macros/utils/columns_spec_ddl.sql
--rw-r--r--   0        0        0      177 2020-02-02 00:00:00.000000 dbt_postgres-1.8.0b1/dbt/include/postgres/macros/utils/dateadd.sql
--rw-r--r--   0        0        0     2340 2020-02-02 00:00:00.000000 dbt_postgres-1.8.0b1/dbt/include/postgres/macros/utils/datediff.sql
--rw-r--r--   0        0        0      382 2020-02-02 00:00:00.000000 dbt_postgres-1.8.0b1/dbt/include/postgres/macros/utils/last_day.sql
--rw-r--r--   0        0        0      556 2020-02-02 00:00:00.000000 dbt_postgres-1.8.0b1/dbt/include/postgres/macros/utils/listagg.sql
--rw-r--r--   0        0        0      300 2020-02-02 00:00:00.000000 dbt_postgres-1.8.0b1/dbt/include/postgres/macros/utils/split_part.sql
--rw-r--r--   0        0        0     3105 2020-02-02 00:00:00.000000 dbt_postgres-1.8.0b1/.gitignore
--rw-r--r--   0        0        0    11344 2020-02-02 00:00:00.000000 dbt_postgres-1.8.0b1/LICENSE
--rw-r--r--   0        0        0     1923 2020-02-02 00:00:00.000000 dbt_postgres-1.8.0b1/README.md
--rw-r--r--   0        0        0     4734 2020-02-02 00:00:00.000000 dbt_postgres-1.8.0b1/pyproject.toml
--rw-r--r--   0        0        0     3308 2020-02-02 00:00:00.000000 dbt_postgres-1.8.0b1/PKG-INFO
+-rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 dbt_postgres-1.8.0b2/dbt/__init__.py
+-rw-r--r--   0        0        0      492 2020-02-02 00:00:00.000000 dbt_postgres-1.8.0b2/dbt/adapters/postgres/__init__.py
+-rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 dbt_postgres-1.8.0b2/dbt/adapters/postgres/__version__.py
+-rw-r--r--   0        0        0      381 2020-02-02 00:00:00.000000 dbt_postgres-1.8.0b2/dbt/adapters/postgres/column.py
+-rw-r--r--   0        0        0     7221 2020-02-02 00:00:00.000000 dbt_postgres-1.8.0b2/dbt/adapters/postgres/connections.py
+-rw-r--r--   0        0        0     5688 2020-02-02 00:00:00.000000 dbt_postgres-1.8.0b2/dbt/adapters/postgres/impl.py
+-rw-r--r--   0        0        0     3976 2020-02-02 00:00:00.000000 dbt_postgres-1.8.0b2/dbt/adapters/postgres/relation.py
+-rw-r--r--   0        0        0      377 2020-02-02 00:00:00.000000 dbt_postgres-1.8.0b2/dbt/adapters/postgres/relation_configs/__init__.py
+-rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 dbt_postgres-1.8.0b2/dbt/adapters/postgres/relation_configs/constants.py
+-rw-r--r--   0        0        0     5720 2020-02-02 00:00:00.000000 dbt_postgres-1.8.0b2/dbt/adapters/postgres/relation_configs/index.py
+-rw-r--r--   0        0        0     4158 2020-02-02 00:00:00.000000 dbt_postgres-1.8.0b2/dbt/adapters/postgres/relation_configs/materialized_view.py
+-rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 dbt_postgres-1.8.0b2/dbt/include/postgres/__init__.py
+-rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 dbt_postgres-1.8.0b2/dbt/include/postgres/dbt_project.yml
+-rw-r--r--   0        0        0      410 2020-02-02 00:00:00.000000 dbt_postgres-1.8.0b2/dbt/include/postgres/profile_template.yml
+-rw-r--r--   0        0        0      439 2020-02-02 00:00:00.000000 dbt_postgres-1.8.0b2/dbt/include/postgres/sample_profiles.yml
+-rw-r--r--   0        0        0     9374 2020-02-02 00:00:00.000000 dbt_postgres-1.8.0b2/dbt/include/postgres/macros/adapters.sql
+-rw-r--r--   0        0        0     2852 2020-02-02 00:00:00.000000 dbt_postgres-1.8.0b2/dbt/include/postgres/macros/catalog.sql
+-rw-r--r--   0        0        0     2706 2020-02-02 00:00:00.000000 dbt_postgres-1.8.0b2/dbt/include/postgres/macros/relations.sql
+-rw-r--r--   0        0        0      620 2020-02-02 00:00:00.000000 dbt_postgres-1.8.0b2/dbt/include/postgres/macros/timestamps.sql
+-rw-r--r--   0        0        0      261 2020-02-02 00:00:00.000000 dbt_postgres-1.8.0b2/dbt/include/postgres/macros/materializations/incremental_strategies.sql
+-rw-r--r--   0        0        0      794 2020-02-02 00:00:00.000000 dbt_postgres-1.8.0b2/dbt/include/postgres/macros/materializations/snapshot_merge.sql
+-rw-r--r--   0        0        0     1534 2020-02-02 00:00:00.000000 dbt_postgres-1.8.0b2/dbt/include/postgres/macros/relations/materialized_view/alter.sql
+-rw-r--r--   0        0        0      297 2020-02-02 00:00:00.000000 dbt_postgres-1.8.0b2/dbt/include/postgres/macros/relations/materialized_view/create.sql
+-rw-r--r--   0        0        0      261 2020-02-02 00:00:00.000000 dbt_postgres-1.8.0b2/dbt/include/postgres/macros/relations/materialized_view/describe.sql
+-rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 dbt_postgres-1.8.0b2/dbt/include/postgres/macros/relations/materialized_view/drop.sql
+-rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 dbt_postgres-1.8.0b2/dbt/include/postgres/macros/relations/materialized_view/refresh.sql
+-rw-r--r--   0        0        0      158 2020-02-02 00:00:00.000000 dbt_postgres-1.8.0b2/dbt/include/postgres/macros/relations/materialized_view/rename.sql
+-rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 dbt_postgres-1.8.0b2/dbt/include/postgres/macros/relations/table/drop.sql
+-rw-r--r--   0        0        0      134 2020-02-02 00:00:00.000000 dbt_postgres-1.8.0b2/dbt/include/postgres/macros/relations/table/rename.sql
+-rw-r--r--   0        0        0      545 2020-02-02 00:00:00.000000 dbt_postgres-1.8.0b2/dbt/include/postgres/macros/relations/table/replace.sql
+-rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 dbt_postgres-1.8.0b2/dbt/include/postgres/macros/relations/view/drop.sql
+-rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 dbt_postgres-1.8.0b2/dbt/include/postgres/macros/relations/view/rename.sql
+-rw-r--r--   0        0        0      436 2020-02-02 00:00:00.000000 dbt_postgres-1.8.0b2/dbt/include/postgres/macros/relations/view/replace.sql
+-rw-r--r--   0        0        0      182 2020-02-02 00:00:00.000000 dbt_postgres-1.8.0b2/dbt/include/postgres/macros/utils/any_value.sql
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dbt_postgres-1.8.0b2/dbt/include/postgres/macros/utils/columns_spec_ddl.sql
+-rw-r--r--   0        0        0      177 2020-02-02 00:00:00.000000 dbt_postgres-1.8.0b2/dbt/include/postgres/macros/utils/dateadd.sql
+-rw-r--r--   0        0        0     2340 2020-02-02 00:00:00.000000 dbt_postgres-1.8.0b2/dbt/include/postgres/macros/utils/datediff.sql
+-rw-r--r--   0        0        0      382 2020-02-02 00:00:00.000000 dbt_postgres-1.8.0b2/dbt/include/postgres/macros/utils/last_day.sql
+-rw-r--r--   0        0        0      556 2020-02-02 00:00:00.000000 dbt_postgres-1.8.0b2/dbt/include/postgres/macros/utils/listagg.sql
+-rw-r--r--   0        0        0      300 2020-02-02 00:00:00.000000 dbt_postgres-1.8.0b2/dbt/include/postgres/macros/utils/split_part.sql
+-rw-r--r--   0        0        0     3105 2020-02-02 00:00:00.000000 dbt_postgres-1.8.0b2/.gitignore
+-rw-r--r--   0        0        0    11344 2020-02-02 00:00:00.000000 dbt_postgres-1.8.0b2/LICENSE
+-rw-r--r--   0        0        0     1923 2020-02-02 00:00:00.000000 dbt_postgres-1.8.0b2/README.md
+-rw-r--r--   0        0        0     1919 2020-02-02 00:00:00.000000 dbt_postgres-1.8.0b2/hatch_build.py
+-rw-r--r--   0        0        0     4632 2020-02-02 00:00:00.000000 dbt_postgres-1.8.0b2/pyproject.toml
+-rw-r--r--   0        0        0     3371 2020-02-02 00:00:00.000000 dbt_postgres-1.8.0b2/PKG-INFO
```

### Comparing `dbt_postgres-1.8.0b1/dbt/adapters/postgres/connections.py` & `dbt_postgres-1.8.0b2/dbt/adapters/postgres/connections.py`

 * *Files identical despite different names*

### Comparing `dbt_postgres-1.8.0b1/dbt/adapters/postgres/impl.py` & `dbt_postgres-1.8.0b2/dbt/adapters/postgres/impl.py`

 * *Files identical despite different names*

### Comparing `dbt_postgres-1.8.0b1/dbt/adapters/postgres/relation.py` & `dbt_postgres-1.8.0b2/dbt/adapters/postgres/relation.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from dataclasses import dataclass
+from dataclasses import dataclass, field
 from typing import FrozenSet, Optional, Set
 
 from dbt.adapters.base.relation import BaseRelation
 from dbt.adapters.contracts.relation import RelationConfig, RelationType
 from dbt.adapters.relation_configs import (
     RelationConfigChangeAction,
     RelationResults,
@@ -16,27 +16,27 @@
     PostgresMaterializedViewConfig,
     PostgresMaterializedViewConfigChangeCollection,
 )
 
 
 @dataclass(frozen=True, eq=False, repr=False)
 class PostgresRelation(BaseRelation):
-    renameable_relations = frozenset(
+    renameable_relations: FrozenSet[RelationType] = field(default_factory=lambda: frozenset(
         {
             RelationType.View,
             RelationType.Table,
             RelationType.MaterializedView,
         }
-    )
-    replaceable_relations = frozenset(
+    ))
+    replaceable_relations: FrozenSet[RelationType] = field(default_factory=lambda: frozenset(
         {
             RelationType.View,
             RelationType.Table,
         }
-    )
+    ))
 
     def __post_init__(self):
         # Check for length of Postgres table/view names.
         # Check self.type to exclude test relation identifiers
         if (
             self.identifier is not None
             and self.type is not None
```

### Comparing `dbt_postgres-1.8.0b1/dbt/adapters/postgres/relation_configs/index.py` & `dbt_postgres-1.8.0b2/dbt/adapters/postgres/relation_configs/index.py`

 * *Files identical despite different names*

### Comparing `dbt_postgres-1.8.0b1/dbt/adapters/postgres/relation_configs/materialized_view.py` & `dbt_postgres-1.8.0b2/dbt/adapters/postgres/relation_configs/materialized_view.py`

 * *Files identical despite different names*

### Comparing `dbt_postgres-1.8.0b1/dbt/include/postgres/macros/adapters.sql` & `dbt_postgres-1.8.0b2/dbt/include/postgres/macros/adapters.sql`

 * *Files identical despite different names*

### Comparing `dbt_postgres-1.8.0b1/dbt/include/postgres/macros/catalog.sql` & `dbt_postgres-1.8.0b2/dbt/include/postgres/macros/catalog.sql`

 * *Files identical despite different names*

### Comparing `dbt_postgres-1.8.0b1/dbt/include/postgres/macros/relations.sql` & `dbt_postgres-1.8.0b2/dbt/include/postgres/macros/relations.sql`

 * *Files identical despite different names*

### Comparing `dbt_postgres-1.8.0b1/dbt/include/postgres/macros/timestamps.sql` & `dbt_postgres-1.8.0b2/dbt/include/postgres/macros/timestamps.sql`

 * *Files identical despite different names*

### Comparing `dbt_postgres-1.8.0b1/dbt/include/postgres/macros/materializations/snapshot_merge.sql` & `dbt_postgres-1.8.0b2/dbt/include/postgres/macros/materializations/snapshot_merge.sql`

 * *Files identical despite different names*

### Comparing `dbt_postgres-1.8.0b1/dbt/include/postgres/macros/relations/materialized_view/alter.sql` & `dbt_postgres-1.8.0b2/dbt/include/postgres/macros/relations/materialized_view/alter.sql`

 * *Files identical despite different names*

### Comparing `dbt_postgres-1.8.0b1/dbt/include/postgres/macros/relations/table/replace.sql` & `dbt_postgres-1.8.0b2/dbt/include/postgres/macros/relations/table/replace.sql`

 * *Files identical despite different names*

### Comparing `dbt_postgres-1.8.0b1/dbt/include/postgres/macros/utils/datediff.sql` & `dbt_postgres-1.8.0b2/dbt/include/postgres/macros/utils/datediff.sql`

 * *Files identical despite different names*

### Comparing `dbt_postgres-1.8.0b1/dbt/include/postgres/macros/utils/listagg.sql` & `dbt_postgres-1.8.0b2/dbt/include/postgres/macros/utils/listagg.sql`

 * *Files identical despite different names*

### Comparing `dbt_postgres-1.8.0b1/.gitignore` & `dbt_postgres-1.8.0b2/.gitignore`

 * *Files identical despite different names*

### Comparing `dbt_postgres-1.8.0b1/LICENSE` & `dbt_postgres-1.8.0b2/LICENSE`

 * *Files identical despite different names*

### Comparing `dbt_postgres-1.8.0b1/README.md` & `dbt_postgres-1.8.0b2/README.md`

 * *Files identical despite different names*

### Comparing `dbt_postgres-1.8.0b1/pyproject.toml` & `dbt_postgres-1.8.0b2/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [project]
-dynamic = ["version"]
+dynamic = ["version", "dependencies"]
 name = "dbt-postgres"
 description = "The set of adapter protocols and base functionality that supports integration with dbt-core"
 readme = "README.md"
 keywords = ["dbt", "adapter", "adapters", "database", "elt", "dbt-core", "dbt Core", "dbt Cloud", "dbt Labs", "postgres"]
 requires-python = ">=3.8.0"
 authors = [
     { name = "dbt Labs", email = "info@dbtlabs.com" },
@@ -18,21 +18,15 @@
     "Operating System :: Microsoft :: Windows",
     "Operating System :: POSIX :: Linux",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
 ]
-dependencies = [
-    "dbt-adapters>=0.1.0a1,<2.0",
-    "psycopg2>=2.9,<3.0",
-    # installed via dbt-adapters but used directly
-    "dbt-common>=0.1.0a1,<2.0",
-    "agate>=1.0,<2.0",
-]
+
 [project.urls]
 Homepage = "https://github.com/dbt-labs/dbt-postgres"
 Documentation = "https://docs.getdbt.com"
 Repository = "https://github.com/dbt-labs/dbt-postgres.git"
 Issues = "https://github.com/dbt-labs/dbt-postgres/issues"
 Changelog = "https://github.com/dbt-labs/dbt-postgres/blob/main/CHANGELOG.md"
 
@@ -45,24 +39,27 @@
 
 [tool.hatch.build.targets.wheel]
 packages = ["dbt"]
 
 [tool.hatch.version]
 path = "dbt/adapters/postgres/__version__.py"
 
+[tool.hatch.build.hooks.custom]
+path = "./hatch_build.py"
+
 [tool.hatch.envs.default]
 dependencies = [
     "dbt-adapters @ git+https://github.com/dbt-labs/dbt-adapters.git",
     "dbt-common @ git+https://github.com/dbt-labs/dbt-common.git",
 ]
 
 [tool.hatch.envs.lint]
 detached = true
 dependencies = [
-    "black",
+    "black>=24.3",
     "flake8",
     "Flake8-pyproject",
 ]
 [tool.hatch.envs.lint.scripts]
 all = [
     "black",
     "flake8",
@@ -115,14 +112,16 @@
 [tool.hatch.envs.build]
 detached = true
 dependencies = [
     "wheel",
     "twine",
     "check-wheel-contents",
 ]
+
+
 [tool.hatch.envs.build.scripts]
 check-all = [
     "- check-wheel",
     "- check-sdist",
 ]
 check-wheel = [
     "twine check dist/*",
@@ -162,8 +161,8 @@
 ]
 
 [tool.pytest]
 env_files = ["test.env"]
 testpaths = [
     "tests/functional",
     "tests/unit",
-]
+]
```

### Comparing `dbt_postgres-1.8.0b1/PKG-INFO` & `dbt_postgres-1.8.0b2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,11 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: dbt-postgres
-Version: 1.8.0b1
+Version: 1.8.0b2
+Dynamic: Requires-Dist
 Summary: The set of adapter protocols and base functionality that supports integration with dbt-core
 Project-URL: Homepage, https://github.com/dbt-labs/dbt-postgres
 Project-URL: Documentation, https://docs.getdbt.com
 Project-URL: Repository, https://github.com/dbt-labs/dbt-postgres.git
 Project-URL: Issues, https://github.com/dbt-labs/dbt-postgres/issues
 Project-URL: Changelog, https://github.com/dbt-labs/dbt-postgres/blob/main/CHANGELOG.md
 Author-email: dbt Labs <info@dbtlabs.com>
@@ -17,18 +18,19 @@
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.8.0
-Requires-Dist: agate<2.0,>=1.0
-Requires-Dist: dbt-adapters<2.0,>=0.1.0a1
-Requires-Dist: dbt-common<2.0,>=0.1.0a1
-Requires-Dist: psycopg2<3.0,>=2.9
+Requires-Dist: dbt-adapters>=0.1.0a1,<2.0
+Requires-Dist: dbt-core>=1.8.0a1
+Requires-Dist: dbt-common>=0.1.0a1,<2.0
+Requires-Dist: agate>=1.0,<2.0
+Requires-Dist: psycopg2-binary>=2.9,<3.0
 Description-Content-Type: text/markdown
 
 <p align="center">
   <img src="https://raw.githubusercontent.com/dbt-labs/dbt/ec7dee39f793aa4f7dd3dae37282cc87664813e4/etc/dbt-logo-full.svg" alt="dbt logo" width="500"/>
 </p>
 <p align="center">
   <a href="https://github.com/dbt-labs/dbt-core/actions/workflows/main.yml">
```

#### html2text {}

```diff
@@ -1,26 +1,27 @@
-Metadata-Version: 2.1 Name: dbt-postgres Version: 1.8.0b1 Summary: The set of
-adapter protocols and base functionality that supports integration with dbt-
-core Project-URL: Homepage, https://github.com/dbt-labs/dbt-postgres Project-
-URL: Documentation, https://docs.getdbt.com Project-URL: Repository, https://
-github.com/dbt-labs/dbt-postgres.git Project-URL: Issues, https://github.com/
-dbt-labs/dbt-postgres/issues Project-URL: Changelog, https://github.com/dbt-
-labs/dbt-postgres/blob/main/CHANGELOG.md Author-email: dbt Labs
+Metadata-Version: 2.3 Name: dbt-postgres Version: 1.8.0b2 Dynamic: Requires-
+Dist Summary: The set of adapter protocols and base functionality that supports
+integration with dbt-core Project-URL: Homepage, https://github.com/dbt-labs/
+dbt-postgres Project-URL: Documentation, https://docs.getdbt.com Project-URL:
+Repository, https://github.com/dbt-labs/dbt-postgres.git Project-URL: Issues,
+https://github.com/dbt-labs/dbt-postgres/issues Project-URL: Changelog, https:/
+/github.com/dbt-labs/dbt-postgres/blob/main/CHANGELOG.md Author-email: dbt Labs
 dbtlabs.com> Maintainer-email: dbt Labs
 dbtlabs.com> License-File: LICENSE Keywords: adapter,adapters,database,dbt,dbt
 Cloud,dbt Core,dbt Labs,dbt-core,elt,postgres Classifier: Development Status ::
 5 - Production/Stable Classifier: License :: OSI Approved :: Apache Software
 License Classifier: Operating System :: MacOS :: MacOS X Classifier: Operating
 System :: Microsoft :: Windows Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
 Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11 Requires-Python: >=3.8.0
-Requires-Dist: agate<2.0,>=1.0 Requires-Dist: dbt-adapters<2.0,>=0.1.0a1
-Requires-Dist: dbt-common<2.0,>=0.1.0a1 Requires-Dist: psycopg2<3.0,>=2.9
-Description-Content-Type: text/markdown
+Requires-Dist: dbt-adapters>=0.1.0a1,<2.0 Requires-Dist: dbt-core>=1.8.0a1
+Requires-Dist: dbt-common>=0.1.0a1,<2.0 Requires-Dist: agate>=1.0,<2.0
+Requires-Dist: psycopg2-binary>=2.9,<3.0 Description-Content-Type: text/
+markdown
                                   [dbt logo]
                                   _[_C_I_ _B_a_d_g_e_]
 **[dbt](https://www.getdbt.com/)** enables data analysts and engineers to
 transform their data using the same practices that software engineers use to
 build applications. dbt is the T in ELT. Organize, cleanse, denormalize,
 filter, rename, and pre-aggregate the raw data in your warehouse so that it's
 ready for analysis. ## dbt-postgres The `dbt-postgres` package contains all of
```

