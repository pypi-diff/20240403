# Comparing `tmp/yes-chef-0.7.0.tar.gz` & `tmp/yes-chef-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yes-chef-0.7.0.tar", last modified: Sat Mar  9 20:46:14 2024, max compression
+gzip compressed data, was "yes-chef-0.8.0.tar", last modified: Wed Apr  3 18:09:44 2024, max compression
```

## Comparing `yes-chef-0.7.0.tar` & `yes-chef-0.8.0.tar`

### file list

```diff
@@ -1,37 +1,38 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-09 20:46:14.855475 yes-chef-0.7.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1704 2024-03-09 20:46:14.855475 yes-chef-0.7.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      660 2024-03-09 20:45:59.000000 yes-chef-0.7.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1727 2024-03-09 20:46:00.000000 yes-chef-0.7.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-09 20:46:14.855475 yes-chef-0.7.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-09 20:46:14.851475 yes-chef-0.7.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-09 20:46:14.851475 yes-chef-0.7.0/src/api/
--rw-r--r--   0 runner    (1001) docker     (127)      185 2024-03-09 20:46:00.000000 yes-chef-0.7.0/src/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3274 2024-03-09 20:45:59.000000 yes-chef-0.7.0/src/api/ingredient.py
--rw-r--r--   0 runner    (1001) docker     (127)      231 2024-03-09 20:45:59.000000 yes-chef-0.7.0/src/api/initialise.py
--rw-r--r--   0 runner    (1001) docker     (127)     1698 2024-03-09 20:45:59.000000 yes-chef-0.7.0/src/api/plan.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-09 20:46:14.851475 yes-chef-0.7.0/src/api/recipe/
--rw-r--r--   0 runner    (1001) docker     (127)       68 2024-03-09 20:45:59.000000 yes-chef-0.7.0/src/api/recipe/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1824 2024-03-09 20:45:59.000000 yes-chef-0.7.0/src/api/recipe/formats.py
--rw-r--r--   0 runner    (1001) docker     (127)     2510 2024-03-09 20:45:59.000000 yes-chef-0.7.0/src/api/recipe/recipe.py
--rw-r--r--   0 runner    (1001) docker     (127)      928 2024-03-09 20:45:59.000000 yes-chef-0.7.0/src/api/recipe/serializer.py
--rw-r--r--   0 runner    (1001) docker     (127)      671 2024-03-09 20:45:59.000000 yes-chef-0.7.0/src/api/recipe/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      823 2024-03-09 20:45:59.000000 yes-chef-0.7.0/src/api/settings.py
--rw-r--r--   0 runner    (1001) docker     (127)     1375 2024-03-09 20:45:59.000000 yes-chef-0.7.0/src/api/shopping_list.py
--rw-r--r--   0 runner    (1001) docker     (127)     2112 2024-03-09 20:45:59.000000 yes-chef-0.7.0/src/api/unit.py
--rw-r--r--   0 runner    (1001) docker     (127)      765 2024-03-09 20:45:59.000000 yes-chef-0.7.0/src/api/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-09 20:46:14.855475 yes-chef-0.7.0/src/cli/
--rw-r--r--   0 runner    (1001) docker     (127)     2174 2024-03-09 20:45:59.000000 yes-chef-0.7.0/src/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      812 2024-03-09 20:45:59.000000 yes-chef-0.7.0/src/cli/new.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-09 20:46:14.855475 yes-chef-0.7.0/src/cli/routines/
--rw-r--r--   0 runner    (1001) docker     (127)       80 2024-03-09 20:45:59.000000 yes-chef-0.7.0/src/cli/routines/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1993 2024-03-09 20:45:59.000000 yes-chef-0.7.0/src/cli/routines/export_recipes.py
--rw-r--r--   0 runner    (1001) docker     (127)     1226 2024-03-09 20:45:59.000000 yes-chef-0.7.0/src/cli/routines/plan_recipe.py
--rw-r--r--   0 runner    (1001) docker     (127)     2130 2024-03-09 20:45:59.000000 yes-chef-0.7.0/src/cli/routines/recipe_wizard.py
--rw-r--r--   0 runner    (1001) docker     (127)      905 2024-03-09 20:45:59.000000 yes-chef-0.7.0/src/cli/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3007 2024-03-09 20:45:59.000000 yes-chef-0.7.0/src/cli/view.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-09 20:46:14.855475 yes-chef-0.7.0/yes_chef.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1704 2024-03-09 20:46:14.000000 yes-chef-0.7.0/yes_chef.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      670 2024-03-09 20:46:14.000000 yes-chef-0.7.0/yes_chef.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-09 20:46:14.000000 yes-chef-0.7.0/yes_chef.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      230 2024-03-09 20:46:14.000000 yes-chef-0.7.0/yes_chef.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        4 2024-03-09 20:46:14.000000 yes-chef-0.7.0/yes_chef.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 18:09:44.462233 yes-chef-0.8.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1704 2024-04-03 18:09:44.458233 yes-chef-0.8.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      660 2024-04-03 18:09:26.000000 yes-chef-0.8.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1834 2024-04-03 18:09:26.000000 yes-chef-0.8.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-03 18:09:44.462233 yes-chef-0.8.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 18:09:44.454233 yes-chef-0.8.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 18:09:44.454233 yes-chef-0.8.0/src/api/
+-rw-r--r--   0 runner    (1001) docker     (127)      185 2024-04-03 18:09:26.000000 yes-chef-0.8.0/src/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-03 18:09:26.000000 yes-chef-0.8.0/src/api/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3887 2024-04-03 18:09:26.000000 yes-chef-0.8.0/src/api/ingredient.py
+-rw-r--r--   0 runner    (1001) docker     (127)      574 2024-04-03 18:09:26.000000 yes-chef-0.8.0/src/api/initialise.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1794 2024-04-03 18:09:26.000000 yes-chef-0.8.0/src/api/plan.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 18:09:44.458233 yes-chef-0.8.0/src/api/recipe/
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-04-03 18:09:26.000000 yes-chef-0.8.0/src/api/recipe/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1824 2024-04-03 18:09:26.000000 yes-chef-0.8.0/src/api/recipe/formats.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2534 2024-04-03 18:09:26.000000 yes-chef-0.8.0/src/api/recipe/recipe.py
+-rw-r--r--   0 runner    (1001) docker     (127)      928 2024-04-03 18:09:26.000000 yes-chef-0.8.0/src/api/recipe/serializer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      671 2024-04-03 18:09:26.000000 yes-chef-0.8.0/src/api/recipe/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3895 2024-04-03 18:09:26.000000 yes-chef-0.8.0/src/api/settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2307 2024-04-03 18:09:26.000000 yes-chef-0.8.0/src/api/shopping_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2180 2024-04-03 18:09:26.000000 yes-chef-0.8.0/src/api/unit.py
+-rw-r--r--   0 runner    (1001) docker     (127)      765 2024-04-03 18:09:26.000000 yes-chef-0.8.0/src/api/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 18:09:44.458233 yes-chef-0.8.0/src/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)     2214 2024-04-03 18:09:26.000000 yes-chef-0.8.0/src/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      901 2024-04-03 18:09:26.000000 yes-chef-0.8.0/src/cli/new.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 18:09:44.458233 yes-chef-0.8.0/src/cli/routines/
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2024-04-03 18:09:26.000000 yes-chef-0.8.0/src/cli/routines/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1983 2024-04-03 18:09:26.000000 yes-chef-0.8.0/src/cli/routines/export_recipes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1226 2024-04-03 18:09:26.000000 yes-chef-0.8.0/src/cli/routines/plan_recipe.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2130 2024-04-03 18:09:26.000000 yes-chef-0.8.0/src/cli/routines/recipe_wizard.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1514 2024-04-03 18:09:26.000000 yes-chef-0.8.0/src/cli/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3128 2024-04-03 18:09:26.000000 yes-chef-0.8.0/src/cli/view.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 18:09:44.458233 yes-chef-0.8.0/yes_chef.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1704 2024-04-03 18:09:44.000000 yes-chef-0.8.0/yes_chef.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      691 2024-04-03 18:09:44.000000 yes-chef-0.8.0/yes_chef.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 18:09:44.000000 yes-chef-0.8.0/yes_chef.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      230 2024-04-03 18:09:44.000000 yes-chef-0.8.0/yes_chef.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-04-03 18:09:44.000000 yes-chef-0.8.0/yes_chef.egg-info/top_level.txt
```

### Comparing `yes-chef-0.7.0/PKG-INFO` & `yes-chef-0.8.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yes-chef
-Version: 0.7.0
+Version: 0.8.0
 Summary: A command-line tool for managing recipes and making shopping lists.
 Author-email: Robin Neville <robin.m.neville@gmail.com>
 Maintainer-email: Robin Neville <robin.m.neville@gmail.com>
 Project-URL: Repository, https://github.com/binnev/yes-chef
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Requires-Dist: typer>=0.9
```

### Comparing `yes-chef-0.7.0/README.md` & `yes-chef-0.8.0/README.md`

 * *Files identical despite different names*

### Comparing `yes-chef-0.7.0/pyproject.toml` & `yes-chef-0.8.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [project]
 name = "yes-chef"
 description = "A command-line tool for managing recipes and making shopping lists."
-version = "0.7.0"
+version = "0.8.0"
 readme = "README.md"
 requires-python = ">=3.10"
 authors = [
     { name = "Robin Neville", email = "robin.m.neville@gmail.com" },
 ]
 maintainers = [
     { name = "Robin Neville", email = "robin.m.neville@gmail.com" },
@@ -45,14 +45,19 @@
 include = ["src*"]
 
 [tool.pytest.ini_options]
 #addopts = "-p no:cacheprovider --cov --cov-fail-under=70 --cov-report term-missing:skip-covered"
 testpaths = ["tests"]
 markers = [
     "allow_settings_save: by default, Settings.save is mocked, so we don't create real files when running tests.",
+    "allow_settings_load: ditto",
+    "allow_path_mkdir",
+    "allow_path_touch",
+    "allow_path_glob",
+
 ]
 
 [tool.coverage.run]
 omit = ["*/__init__.py"]
 
 
 [tool.ruff]
@@ -67,9 +72,9 @@
 tag_format = "$version"
 version_scheme = "semver"
 version_provider = "pep621"
 update_changelog_on_bump = true
 major_version_zero = true
 version_files = [
     "pyproject.toml:version",
-    "src/api/__init__.py:__version__",
+    "src/api/constants.py:__version__",
 ]
```

### Comparing `yes-chef-0.7.0/src/api/plan.py` & `yes-chef-0.8.0/src/api/plan.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,59 +1,66 @@
 import json
 from datetime import datetime
+from pathlib import Path
 
 from pydantic import BaseModel, Field
 
 from . import utils
 from .recipe import Recipe
-from .settings import Settings
+from .settings import PLANS_DIR
 from .shopping_list import merge_recipes, ShoppingList
 
 
 class Plan(BaseModel):
     created: datetime = Field(default_factory=lambda: datetime.utcnow())
     recipes: list[Recipe] = Field(default_factory=list)
 
     def __str__(self):
         return f"Plan (created at {self.created})"
 
     def shopping_list(self) -> ShoppingList:
         """
         Merge the ingredients from self.recipes into one list of ingredients.
+
+        Returns:
+            shopping list
         """
         return merge_recipes(self.recipes)
 
     def add(self, recipe: Recipe):
         self.recipes.append(recipe)
 
     @classmethod
     def new(cls) -> "Plan":
         """
         Create a new plan in the filesystem
-        :return: new plan
+
+        Returns:
+            new plan
         """
         plan = cls()
         filename = plan.filename
         utils.touch(filename)
         with open(filename, "w") as file:
             file.write(plan.model_dump_json())
         return plan
 
     @classmethod
     def current(cls) -> "Plan":
-        settings = Settings.from_file()
-        json_files = settings.plans_dir.glob("*.json")
+        json_files = list(PLANS_DIR.glob("*.json"))
+        if not json_files:
+            return cls.new()
         latest = max(json_files)  # relying on string comparison here
         with open(latest) as file:
             try:
                 return Plan(**json.load(file))
             except json.JSONDecodeError:
-                return cls.new_plan()
+                return cls.new()
 
     def save(self):
         with open(self.filename, "w") as file:
             file.write(self.model_dump_json())
 
     @property
-    def filename(self):
-        settings = Settings.from_file()
-        return settings.plans_dir / f"{self.created.isoformat()}.json"
+    def filename(self) -> Path:
+        time_str = self.created.isoformat(timespec="seconds")
+        return PLANS_DIR / f"{time_str}.json"
```

### Comparing `yes-chef-0.7.0/src/api/recipe/formats.py` & `yes-chef-0.8.0/src/api/recipe/formats.py`

 * *Files identical despite different names*

### Comparing `yes-chef-0.7.0/src/api/recipe/recipe.py` & `yes-chef-0.8.0/src/api/recipe/recipe.py`

 * *Files 11% similar despite different names*

```diff
@@ -61,17 +61,19 @@
         ]
 
     @classmethod
     async def load_all(cls) -> list["Recipe"]:
         """
         Load all the recipes from yaml
         """
-        settings = Settings.from_file()
+        settings = Settings.load()
         # todo: de-dupe these paths
-        filenames = settings.recipe_library.joinpath("yaml").glob("*.yaml")
+        filenames = settings.system.recipe_library.joinpath("yaml").glob(
+            "*.yaml"
+        )
         return list(await asyncio.gather(*(cls.load(f) for f in filenames)))
 
     @classmethod
     async def load(cls, filename: Path) -> "Recipe":
         """
         Load from yaml
         """
```

### Comparing `yes-chef-0.7.0/src/api/recipe/serializer.py` & `yes-chef-0.8.0/src/api/recipe/serializer.py`

 * *Files identical despite different names*

### Comparing `yes-chef-0.7.0/src/api/recipe/utils.py` & `yes-chef-0.8.0/src/api/recipe/utils.py`

 * *Files identical despite different names*

### Comparing `yes-chef-0.7.0/src/api/unit.py` & `yes-chef-0.8.0/src/api/unit.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,23 @@
+"""
+Handles normalising and converting between units.
+"""
+
 Number = int | float
 
 
 def normalise(amount: Number, unit: str) -> tuple[Number, str]:
     """
     Converts an amount + unit into the preferred internal format (grams or
     millilitres) if possible
 
     Handles:
-        alias (pounds -> lb)
-        system (imperial -> metric) (lb -> kg)
-        denomination (5kg -> 5000g)
+        - alias: (pounds -> lb)
+        - system (imperial -> metric): (lb -> kg)
+        - denomination: (5kg -> 5000g)
 
     Args:
         amount: the input amount e.g. 2.5
         unit: the input unit e.g. "kilos"
 
     Returns:
         The converted amount and unit
```

### Comparing `yes-chef-0.7.0/src/api/utils.py` & `yes-chef-0.8.0/src/api/utils.py`

 * *Files identical despite different names*

### Comparing `yes-chef-0.7.0/src/cli/__init__.py` & `yes-chef-0.8.0/src/cli/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 import asyncio
+import typing as t
 from pathlib import Path
 from typing import Optional
 
 import typer
 
 from . import new, routines
 from . import view
+from .utils import requires_library_init
 from .. import api
 from ..api.settings import Settings
 
 app = typer.Typer()
 app.add_typer(new.app, name="new", help="Create new plan, recipe, etc")
 app.add_typer(view.app, name="view", help="View plan, shopping list, etc")
 
@@ -25,52 +27,57 @@
     """
     path = path.absolute()
     print(f"you passed {path=}")
     api.init_library(path)
 
 
 @app.command()
+@requires_library_init
 def config(
-    recipe_library: str = typer.Option(
-        "",
-        "--recipe-library",
-        help="The folder in which the YAML recipes are stored",
-    ),
+    merge_ingredients: t.Annotated[
+        t.Optional[bool],
+        typer.Option(
+            ...,
+            "--merge-ingredients",
+            help=(
+                "Whether to merge similar ingredients when creating a "
+                "shopping list"
+            ),
+            is_flag=False,
+        ),
+    ] = None,
 ):
     """
     Update and/or view configuration
     """
-    settings = Settings.from_file()
-    if recipe_library:
-        print(f"{recipe_library=}")
-        if (recipe_library := Path(recipe_library)).exists():
-            absolute_path = recipe_library.absolute()
-            settings.recipe_library = absolute_path
-            print(f"Saving recipe library: {absolute_path}")
-            settings.save()
-        else:
-            typer.echo(f"{recipe_library} does not exist")
+    settings = Settings.load()
+    if merge_ingredients is not None:
+        settings.project.merge_ingredients = merge_ingredients
+
+    settings.save()
 
     print("config: ")
-    for key, val in settings.model_dump().items():
+    for key, val in settings.project.model_dump().items():
         print(f"\t{key}: {val}".expandtabs(4))
 
 
 @app.command()
+@requires_library_init
 def plan(
     query: list[str] = typer.Argument(help="Search term to find recipes"),
 ):
     """
     Add a recipe to a plan
     """
     query = " ".join(query)
     asyncio.run(routines.plan_recipe(query))
 
 
 @app.command()
+@requires_library_init
 def export():
     """
     Convert YAML recipes to markdown
     """
     asyncio.run(routines.export_recipes())
```

### Comparing `yes-chef-0.7.0/src/cli/new.py` & `yes-chef-0.8.0/src/cli/new.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,39 +1,42 @@
 """
 new.py
 """
 
 import typer
 
+from .utils import requires_library_init
 from .routines.recipe_wizard import recipe_wizard
 from .. import api
 from ..api import RecipeSerializer, Settings
 from ..api.recipe.serializer import Format
 from ..api.utils import clean_filename
 
 app = typer.Typer()
 
 
 @app.command(name="plan")
+@requires_library_init
 def new_plan():
     """
     Create a new plan
     """
     api.Plan.new()
     typer.secho("created new plan\n")
 
 
 @app.command(name="recipe")
+@requires_library_init
 def new_recipe():
     """
     New recipe wizard
     """
     recipe = recipe_wizard()
     yaml_str = RecipeSerializer().serialize(recipe, Format.YAML)
-    settings = Settings.from_file()
+    settings = Settings.load()
     filename = clean_filename(
-        settings.recipe_library / "yaml" / f"{recipe.name}.yaml"
+        settings.system.recipe_library / "yaml" / f"{recipe.name}.yaml"
     )
     with open(filename, "w") as file:
         file.write(yaml_str)
 
     print(f"Created recipe {filename}")
```

### Comparing `yes-chef-0.7.0/src/cli/routines/export_recipes.py` & `yes-chef-0.8.0/src/cli/routines/export_recipes.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from ...api import Settings
 from ...api.recipe.serializer import Format
 from ...api.recipe.utils import capitalise
 from ...api.utils import clean_filename
 
 
 async def export_recipes():
-    settings = Settings.from_file()
+    settings = Settings.load()
     markdown_folder = settings.recipe_library / "md"  # todo: dedupe this
     recipes = await Recipe.load_all()
     print(f"loaded {len(recipes)} recipes")
     await asyncio.gather(
         *(_serialize(recipe, markdown_folder) for recipe in recipes)
     )
     await create_readme(
@@ -27,15 +27,15 @@
     )
 
 
 async def create_readme(recipes: dict[Path, Recipe]):
     """
     :param recipes: dict of markdown filenames : recipe objects
     """
-    settings = Settings.from_file()
+    settings = Settings.load()
 
     readme = ["# Recipes"]
 
     recipes_list = []
     for md_filename in sorted(recipes):
         recipe = recipes[md_filename]
         recipes_list.append(
```

### Comparing `yes-chef-0.7.0/src/cli/routines/plan_recipe.py` & `yes-chef-0.8.0/src/cli/routines/plan_recipe.py`

 * *Files identical despite different names*

### Comparing `yes-chef-0.7.0/src/cli/routines/recipe_wizard.py` & `yes-chef-0.8.0/src/cli/routines/recipe_wizard.py`

 * *Files identical despite different names*

### Comparing `yes-chef-0.7.0/src/cli/view.py` & `yes-chef-0.8.0/src/cli/view.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,90 +1,93 @@
 """
 view.py
 """
 
 import typer
 
+from .utils import echo, requires_library_init
 from .. import api
-from ..api.shopping_list import Amounts
-from .utils import echo
+from ..api.shopping_list import MergedIngredient
 
 app = typer.Typer()
 
 
 @app.command(name="plan")
+@requires_library_init
 def view_plan():
     """
     view_plan
     """
     plan = api.Plan.current()
     echo("Current plan:")
     echo(f"\tcreated: {plan.created.isoformat()}")
     if plan.recipes:
         echo("\trecipes:")
         for recipe in plan.recipes:
             echo(f"\t\t{recipe}")
 
 
 @app.command(name="list")
+@requires_library_init
 def view_list():
     """
     view_list
     """
     plan = api.Plan.current()
     ingredients = plan.shopping_list()
     echo("Current shopping list:")
-    width = max(map(len, ingredients))
+    width = max(map(len, ingredients), default=0)
     for ing_name in sorted(ingredients):
         amounts = ingredients[ing_name]
         echo(_format_ingredient_for_list(ing_name, amounts, width))
 
 
 @app.command(name="recipe")
+@requires_library_init
 def view_recipe():
     """
     view recipe
     """
     # todo: serialize recipe nicely for terminal
 
 
 def _format_ingredient_for_list(
     ing_name: str,
-    amounts: Amounts,
+    amounts: MergedIngredient,
     width: int = 0,
 ) -> str:
     result = f"{ing_name}:".ljust(width)
-    unique_recipes = len(set(amounts.enough_for))
+    unique_recipes = len(set(amounts.amountless))
     match [unique_recipes, amounts.unitless, len(amounts.units)]:
         case [0, 0, 0]:
             raise ValueError("empty Amounts!")
 
         # ========================= single line cases =========================
         # only 1 unique recipe (could be repeated)
         case [1, 0, 0]:
             recipe_strings = (
-                amounts.enough_for[0]
-                if (count := len(amounts.enough_for)) == 1
-                else f"{amounts.enough_for[0]} (x{count})"
+                amounts.amountless[0]
+                if (count := len(amounts.amountless)) == 1
+                else f"{amounts.amountless[0]} (x{count})"
             )
             result += f" enough for {recipe_strings}"
 
         # just the unitless amount
         case [0, unitless, 0]:
             result += f" {unitless}"
 
         # only 1 unit e.g. {"kg": 2.5}
         case [0, 0, 1]:
             unit, amount = next(iter(amounts.units.items()))
             result += f" {amount} {unit}"
 
         # ========================== multi line cases ==========================
         case _:
-            if amounts.enough_for:
-                result += f"\n\t{_format_amountless(amounts.enough_for)}"
+            if amounts.amountless:
+                result += f"\n\t{_format_amountless(amounts.amountless)}"
             if amounts.unitless:
                 result += f"\n\t{amounts.unitless}"
             for unit, amount in amounts.units.items():
                 result += f"\n\t{amount} {unit}"
 
     return result
```

### Comparing `yes-chef-0.7.0/yes_chef.egg-info/PKG-INFO` & `yes-chef-0.8.0/yes_chef.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yes-chef
-Version: 0.7.0
+Version: 0.8.0
 Summary: A command-line tool for managing recipes and making shopping lists.
 Author-email: Robin Neville <robin.m.neville@gmail.com>
 Maintainer-email: Robin Neville <robin.m.neville@gmail.com>
 Project-URL: Repository, https://github.com/binnev/yes-chef
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Requires-Dist: typer>=0.9
```

### Comparing `yes-chef-0.7.0/yes_chef.egg-info/SOURCES.txt` & `yes-chef-0.8.0/yes_chef.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 README.md
 pyproject.toml
 src/api/__init__.py
+src/api/constants.py
 src/api/ingredient.py
 src/api/initialise.py
 src/api/plan.py
 src/api/settings.py
 src/api/shopping_list.py
 src/api/unit.py
 src/api/utils.py
```

