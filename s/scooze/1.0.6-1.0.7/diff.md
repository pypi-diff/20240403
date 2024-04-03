# Comparing `tmp/scooze-1.0.6.tar.gz` & `tmp/scooze-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scooze-1.0.6.tar", max compression
+gzip compressed data, was "scooze-1.0.7.tar", max compression
```

## Comparing `scooze-1.0.6.tar` & `scooze-1.0.7.tar`

### file list

```diff
@@ -1,43 +1,47 @@
--rw-r--r--   0        0        0     1065 2024-03-03 03:38:00.075866 scooze-1.0.6/LICENSE
--rw-r--r--   0        0        0     3832 2024-03-03 03:38:00.075866 scooze-1.0.6/README.md
--rw-r--r--   0        0        0     2295 2024-03-03 03:38:00.079866 scooze-1.0.6/pyproject.toml
--rw-r--r--   0        0        0        0 2024-03-03 03:38:00.079866 scooze-1.0.6/src/scooze/__init__.py
--rw-r--r--   0        0        0       46 2024-03-03 03:38:00.079866 scooze-1.0.6/src/scooze/api/README.md
--rw-r--r--   0        0        0    18269 2024-03-03 03:38:00.079866 scooze-1.0.6/src/scooze/api/__init__.py
--rw-r--r--   0        0        0     3020 2024-03-03 03:38:00.079866 scooze-1.0.6/src/scooze/api/bulkdata.py
--rw-r--r--   0        0        0     5301 2024-03-03 03:38:00.079866 scooze-1.0.6/src/scooze/api/card.py
--rw-r--r--   0        0        0      388 2024-03-03 03:38:00.079866 scooze-1.0.6/src/scooze/api/deck.py
--rw-r--r--   0        0        0      993 2024-03-03 03:38:00.079866 scooze-1.0.6/src/scooze/api/utils.py
--rw-r--r--   0        0        0     3016 2024-03-03 03:38:00.079866 scooze-1.0.6/src/scooze/bulkdata.py
--rw-r--r--   0        0        0    27141 2024-03-03 03:38:00.079866 scooze-1.0.6/src/scooze/card.py
--rw-r--r--   0        0        0    12799 2024-03-03 03:38:00.079866 scooze-1.0.6/src/scooze/cardparts.py
--rw-r--r--   0        0        0    16121 2024-03-03 03:38:00.079866 scooze-1.0.6/src/scooze/catalogs.py
--rw-r--r--   0        0        0      482 2024-03-03 03:38:00.079866 scooze-1.0.6/src/scooze/config.py
--rw-r--r--   0        0        0     1502 2024-03-03 03:38:00.079866 scooze-1.0.6/src/scooze/console/cli.py
--rw-r--r--   0        0        0     1733 2024-03-03 03:38:00.079866 scooze-1.0.6/src/scooze/console/commands/delete.py
--rw-r--r--   0        0        0     1910 2024-03-03 03:38:00.079866 scooze-1.0.6/src/scooze/console/commands/load/cards.py
--rw-r--r--   0        0        0     2420 2024-03-03 03:38:00.079866 scooze-1.0.6/src/scooze/console/commands/load/decks.py
--rw-r--r--   0        0        0      319 2024-03-03 03:38:00.079866 scooze-1.0.6/src/scooze/console/commands/run.py
--rw-r--r--   0        0        0     1243 2024-03-03 03:38:00.079866 scooze-1.0.6/src/scooze/console/commands/setup/docker.py
--rw-r--r--   0        0        0      371 2024-03-03 03:38:00.079866 scooze-1.0.6/src/scooze/console/commands/setup/local.py
--rw-r--r--   0        0        0      545 2024-03-03 03:38:00.079866 scooze-1.0.6/src/scooze/console/commands/teardown/docker.py
--rw-r--r--   0        0        0      410 2024-03-03 03:38:00.079866 scooze-1.0.6/src/scooze/console/commands/teardown/local.py
--rw-r--r--   0        0        0     6134 2024-03-03 03:38:00.079866 scooze-1.0.6/src/scooze/database/core.py
--rw-r--r--   0        0        0     4517 2024-03-03 03:38:00.079866 scooze-1.0.6/src/scooze/database/deck.py
--rw-r--r--   0        0        0      593 2024-03-03 03:38:00.079866 scooze-1.0.6/src/scooze/database/mongo.py
--rw-r--r--   0        0        0    14001 2024-03-03 03:38:00.079866 scooze-1.0.6/src/scooze/deck.py
--rw-r--r--   0        0        0     4529 2024-03-03 03:38:00.079866 scooze-1.0.6/src/scooze/deckpart.py
--rw-r--r--   0        0        0       44 2024-03-03 03:38:00.079866 scooze-1.0.6/src/scooze/errors.py
--rw-r--r--   0        0        0     1302 2024-03-03 03:38:00.079866 scooze-1.0.6/src/scooze/main.py
--rw-r--r--   0        0        0    22904 2024-03-03 03:38:00.079866 scooze-1.0.6/src/scooze/models/card.py
--rw-r--r--   0        0        0    10886 2024-03-03 03:38:00.083866 scooze-1.0.6/src/scooze/models/cardparts.py
--rw-r--r--   0        0        0     4111 2024-03-03 03:38:00.083866 scooze-1.0.6/src/scooze/models/deck.py
--rw-r--r--   0        0        0     2666 2024-03-03 03:38:00.083866 scooze-1.0.6/src/scooze/models/utils.py
--rw-r--r--   0        0        0      592 2024-03-03 03:38:00.083866 scooze-1.0.6/src/scooze/mongo.py
--rw-r--r--   0        0        0     5552 2024-03-03 03:38:00.083866 scooze-1.0.6/src/scooze/routers/card.py
--rw-r--r--   0        0        0     3656 2024-03-03 03:38:00.083866 scooze-1.0.6/src/scooze/routers/cards.py
--rw-r--r--   0        0        0     2612 2024-03-03 03:38:00.083866 scooze-1.0.6/src/scooze/routers/deck.py
--rw-r--r--   0        0        0     2480 2024-03-03 03:38:00.083866 scooze-1.0.6/src/scooze/routers/decks.py
--rw-r--r--   0        0        0      281 2024-03-03 03:38:00.083866 scooze-1.0.6/src/scooze/static/index.html
--rw-r--r--   0        0        0    15897 2024-03-03 03:38:00.083866 scooze-1.0.6/src/scooze/utils.py
--rw-r--r--   0        0        0     4822 1970-01-01 00:00:00.000000 scooze-1.0.6/PKG-INFO
+-rw-r--r--   0        0        0     1191 2024-04-03 21:52:55.892997 scooze-1.0.7/LICENSE
+-rw-r--r--   0        0        0     2990 2024-04-03 21:52:55.892997 scooze-1.0.7/README.md
+-rw-r--r--   0        0        0     2565 2024-04-03 21:52:55.892997 scooze-1.0.7/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-03 21:52:55.892997 scooze-1.0.7/src/scooze/__init__.py
+-rw-r--r--   0        0        0       46 2024-04-03 21:52:55.896997 scooze-1.0.7/src/scooze/api/README.md
+-rw-r--r--   0        0        0    18295 2024-04-03 21:52:55.896997 scooze-1.0.7/src/scooze/api/__init__.py
+-rw-r--r--   0        0        0     3020 2024-04-03 21:52:55.896997 scooze-1.0.7/src/scooze/api/bulkdata.py
+-rw-r--r--   0        0        0     5375 2024-04-03 21:52:55.896997 scooze-1.0.7/src/scooze/api/card.py
+-rw-r--r--   0        0        0      354 2024-04-03 21:52:55.896997 scooze-1.0.7/src/scooze/api/deck.py
+-rw-r--r--   0        0        0      993 2024-04-03 21:52:55.896997 scooze-1.0.7/src/scooze/api/utils.py
+-rw-r--r--   0        0        0     3166 2024-04-03 21:52:55.896997 scooze-1.0.7/src/scooze/bulkdata.py
+-rw-r--r--   0        0        0    29964 2024-04-03 21:52:55.896997 scooze-1.0.7/src/scooze/card.py
+-rw-r--r--   0        0        0    14218 2024-04-03 21:52:55.896997 scooze-1.0.7/src/scooze/cardparts.py
+-rw-r--r--   0        0        0    16435 2024-04-03 21:52:55.896997 scooze-1.0.7/src/scooze/catalogs.py
+-rw-r--r--   0        0        0      482 2024-04-03 21:52:55.896997 scooze-1.0.7/src/scooze/config.py
+-rw-r--r--   0        0        0        0 2024-04-03 21:52:55.896997 scooze-1.0.7/src/scooze/console/__init__.py
+-rw-r--r--   0        0        0     1502 2024-04-03 21:52:55.896997 scooze-1.0.7/src/scooze/console/cli.py
+-rw-r--r--   0        0        0     1738 2024-04-03 21:52:55.896997 scooze-1.0.7/src/scooze/console/commands/delete.py
+-rw-r--r--   0        0        0     1910 2024-04-03 21:52:55.896997 scooze-1.0.7/src/scooze/console/commands/load/cards.py
+-rw-r--r--   0        0        0     2420 2024-04-03 21:52:55.896997 scooze-1.0.7/src/scooze/console/commands/load/decks.py
+-rw-r--r--   0        0        0      319 2024-04-03 21:52:55.896997 scooze-1.0.7/src/scooze/console/commands/run.py
+-rw-r--r--   0        0        0     1446 2024-04-03 21:52:55.896997 scooze-1.0.7/src/scooze/console/commands/setup/docker.py
+-rw-r--r--   0        0        0      371 2024-04-03 21:52:55.896997 scooze-1.0.7/src/scooze/console/commands/setup/local.py
+-rw-r--r--   0        0        0      545 2024-04-03 21:52:55.896997 scooze-1.0.7/src/scooze/console/commands/teardown/docker.py
+-rw-r--r--   0        0        0      410 2024-04-03 21:52:55.896997 scooze-1.0.7/src/scooze/console/commands/teardown/local.py
+-rw-r--r--   0        0        0     6337 2024-04-03 21:52:55.896997 scooze-1.0.7/src/scooze/database/core.py
+-rw-r--r--   0        0        0     4522 2024-04-03 21:52:55.896997 scooze-1.0.7/src/scooze/database/deck.py
+-rw-r--r--   0        0        0      593 2024-04-03 21:52:55.896997 scooze-1.0.7/src/scooze/database/mongo.py
+-rw-r--r--   0        0        0    15016 2024-04-03 21:52:55.896997 scooze-1.0.7/src/scooze/deck.py
+-rw-r--r--   0        0        0     4601 2024-04-03 21:52:55.896997 scooze-1.0.7/src/scooze/deckpart.py
+-rw-r--r--   0        0        0      681 2024-04-03 21:52:55.896997 scooze-1.0.7/src/scooze/enum.py
+-rw-r--r--   0        0        0       44 2024-04-03 21:52:55.896997 scooze-1.0.7/src/scooze/errors.py
+-rw-r--r--   0        0        0     1302 2024-04-03 21:52:55.896997 scooze-1.0.7/src/scooze/main.py
+-rw-r--r--   0        0        0        0 2024-04-03 21:52:55.896997 scooze-1.0.7/src/scooze/models/__init__.py
+-rw-r--r--   0        0        0    22935 2024-04-03 21:52:55.896997 scooze-1.0.7/src/scooze/models/card.py
+-rw-r--r--   0        0        0    10971 2024-04-03 21:52:55.896997 scooze-1.0.7/src/scooze/models/cardparts.py
+-rw-r--r--   0        0        0     4311 2024-04-03 21:52:55.896997 scooze-1.0.7/src/scooze/models/deck.py
+-rw-r--r--   0        0        0     2737 2024-04-03 21:52:55.896997 scooze-1.0.7/src/scooze/models/utils.py
+-rw-r--r--   0        0        0      592 2024-04-03 21:52:55.896997 scooze-1.0.7/src/scooze/mongo.py
+-rw-r--r--   0        0        0        0 2024-04-03 21:52:55.896997 scooze-1.0.7/src/scooze/routers/__init__.py
+-rw-r--r--   0        0        0     5527 2024-04-03 21:52:55.896997 scooze-1.0.7/src/scooze/routers/card.py
+-rw-r--r--   0        0        0     3656 2024-04-03 21:52:55.896997 scooze-1.0.7/src/scooze/routers/cards.py
+-rw-r--r--   0        0        0     3134 2024-04-03 21:52:55.896997 scooze-1.0.7/src/scooze/routers/deck.py
+-rw-r--r--   0        0        0     2847 2024-04-03 21:52:55.896997 scooze-1.0.7/src/scooze/routers/decks.py
+-rw-r--r--   0        0        0      281 2024-04-03 21:52:55.896997 scooze-1.0.7/src/scooze/static/index.html
+-rw-r--r--   0        0        0    14609 2024-04-03 21:52:55.896997 scooze-1.0.7/src/scooze/utils.py
+-rw-r--r--   0        0        0     4071 1970-01-01 00:00:00.000000 scooze-1.0.7/PKG-INFO
```

### Comparing `scooze-1.0.6/LICENSE` & `scooze-1.0.7/LICENSE`

 * *Files 26% similar despite different names*

```diff
@@ -1,18 +1,21 @@
 MIT License
 
-Copyright (c) 2023 Arcavios
+Copyright (c) 2023 to present Arcavios and individual contributors
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
 
+This software is in no way endorsed or promoted by Scryfall, or Wizards of the
+Coast.
+
 The above copyright notice and this permission notice shall be included in all
 copies or substantial portions of the Software.
 
 THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
 IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
```

### Comparing `scooze-1.0.6/pyproject.toml` & `scooze-1.0.7/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,59 +1,71 @@
 [tool.poetry]
 name = "scooze"
-version = "1.0.6"
+version = "1.0.7"
 description = "A flexible data layer for applications working with Magic: the Gathering cards, decks, and tournaments."
 authors = [
     "Alexander Gimmi <iambroadband@gmail.com>",
     "Ben Horkley <ben.horkley@gmail.com>",
     "Jacob Ginsparg <jacobginsparg@gmail.com>",
 ]
 readme = "README.md"
 packages = [{ include = "scooze", from = "src" }]
 
+[tool.poetry.urls]
+homepage = "https://github.com/arcavios/scooze"
+repository = "https://github.com/arcavios/scooze"
+documentation = "https://scooze.readthedocs.io"
+
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.black]
 line-length = 120
 
 [tool.isort]
 profile = "black"
 src_paths = ["scooze", "tests"]
 
-[tool.poetry.urls]
-"Homepage" = "https://github.com/arcavios/scooze"
-"Bug Tracker" = "https://github.com/arcavios/scooze/issues"
-
 [tool.poetry.dependencies]
-python = ">=3.11, <4"
+beanie = "^1.23.0"
+cleo = "^2.0.1"
+docker = "^6.1.3"
 fastapi = ">=0.100.0, <1.0.0"
-uvicorn = { extras = ["standard"], version = "^0.23.1" }
-motor = "^3.2.0"
-requests = "^2.31.0"
 frozendict = "^2.3.8"
 ijson = "^3.2.3"
-docker = "^6.1.3"
-cleo = "^2.0.1"
-beanie = "^1.23.0"
-pydantic-settings = "^2.0.3"
+motor = "^3.2.0"
+pydantic = "^2.0.0"
+pydantic-settings = "^2.0.0"
+python = ">=3.11, <4"
+requests = "^2.31.0"
+uvicorn = { extras = ["standard"], version = "^0.23.1" }
 
 [tool.poetry.group.dev.dependencies]
-pytest = "^7.4.0"
-pytest-cov = "^4.1.0"
+asgi-lifespan = "^2.1.0"
+black = "^24.3.0"
 coverage = "^7.3.2"
 httpx = "^0.24.1"
-black = "^24.2.0"
 isort = "^5.12.0"
 mongomock = "^4.1.2"
-asgi-lifespan = "^2.1.0"
+mongomock-motor = "^0.0.25"
+pytest = "^7.4.0"
 pytest-asyncio = "^0.21.1"
+pytest-cov = "^4.1.0"
 setuptools = "^68.2.2"
-mongomock-motor = "^0.0.25"
+
+[tool.poetry.group.docs]
+optional = true
+
+[tool.poetry.group.docs.dependencies]
+mkdocs = "^1.5.3"
+mkdocs-material = "^9.5.15"
+mkdocs-simple-hooks = "^0.1.5"
+mkdocstrings = "^0.24.1"
+mkdocstrings-python = "^1.9.0"
 
 [tool.poetry.scripts]
 scooze = "scooze.console.cli:run_cli"
 
 [tool.pytest.ini_options]
 # addopts = "-m 'not slow'"
 addopts = "-W ignore::DeprecationWarning -m 'not context'"
```

### Comparing `scooze-1.0.6/src/scooze/api/__init__.py` & `scooze-1.0.7/src/scooze/api/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,22 +12,24 @@
 from scooze.config import CONFIG
 from scooze.models.card import CardModel
 from scooze.mongo import db, mongo_close, mongo_connect
 
 
 class ScoozeApi(AbstractContextManager):
     """
-    Context manager object for doing I/O from a Mongo database.
+    Context manager object for doing I/O from a local database.
 
-    Sample usage:
-        >>> with ScoozeApi() as s:
-                green_cards = s.get_cards_by("colors", [Color.GREEN])
-                woe_cards = s.get_cards_by_set("woe")
-                black_lotus = s.get_card_by_scryfall_id("b0faa7f2-b547-42c4-a810-839da50dadfe")
-                print(black_lotus.total_words())
+    Example:
+        ``` python
+        with ScoozeApi() as s:
+            green_cards = s.get_cards_by("colors", [Color.GREEN])
+            woe_cards = s.get_cards_by_set("woe")
+            black_lotus = s.get_card_by_scryfall_id("b0faa7f2-b547-42c4-a810-839da50dadfe")
+            print(black_lotus.total_words())
+        ```
     """
 
     def __init__(self, card_class: type[CardT] = FullCard):
         self.card_class = card_class
         self.safe_context = False
 
     def __enter__(self):
@@ -42,15 +44,15 @@
     def __exit__(self, exc_type, exc_val, exc_tb):
         asyncio.get_event_loop().run_until_complete(mongo_close())
 
     # region Card endpoints
 
     @_safe_cache
     @_check_for_safe_context
-    def get_card_by(self, property_name: str, value) -> CardT:
+    def get_card_by(self, property_name: str, value: Any) -> CardT:
         """
         Search the database for the first card that matches the given criteria.
 
         Args:
             property_name: The property to check.
             value: The value to match on.
 
@@ -83,15 +85,15 @@
             values: A list of values to match on.
             paginated: Whether to paginate the results.
             page: The page to look at, if paginated.
             page_size: The size of each page, if paginated.
 
         Returns:
             A list of cards matching the search criteria, or empty list if none
-            were found.
+                were found.
 
         Raises:
             RuntimeError: If used outside a `with` context.
         """
 
         return asyncio.get_event_loop().run_until_complete(
             card_api.get_cards_by(
@@ -299,20 +301,20 @@
     # endregion
 
     # region Bulk data I/O
 
     @_check_for_safe_context
     def load_card_file(self, file_type: ScryfallBulkFile, bulk_file_dir: str):
         """
-        Loads the desired file from the given directory into a local Mongo
-        database. Attempts to download it from Scryfall if it isn't found.
+        Loads the desired file from the given directory into a local database.
+        Attempts to download it from Scryfall if it isn't found.
 
         Args:
             file_type: The type of [ScryfallBulkFile](https://scryfall.com/docs/api/bulk-data)
-            to insert into the database.
+                to insert into the database.
             bulk_file_dir: The path to the folder containing the ScryfallBulkFile.
 
         Raises:
             RuntimeError: If used outside a `with` context.
         """
 
         return asyncio.get_event_loop().run_until_complete(
@@ -323,24 +325,26 @@
         )
 
     # endregion
 
 
 class AsyncScoozeApi(AbstractAsyncContextManager):
     """
-    Async context manager object for doing I/O from a Mongo database.
+    Async context manager object for doing I/O from a local database.
     Most commonly used in asynchronous contexts like Jupyter Notebooks or other
     web applications.
 
-    Sample usage:
-        >>> async with AsyncScoozeApi() as s:
-                green_cards = await s.get_cards_by("colors", [Color.GREEN])
-                woe_cards = await s.get_cards_by_set("woe")
-                black_lotus = await s.get_card_by_scryfall_id("b0faa7f2-b547-42c4-a810-839da50dadfe")
-                print(black_lotus.total_words())
+    Example:
+        ``` python
+        async with AsyncScoozeApi() as s:
+            green_cards = await s.get_cards_by("colors", [Color.GREEN])
+            woe_cards = await s.get_cards_by_set("woe")
+            black_lotus = await s.get_card_by_scryfall_id("b0faa7f2-b547-42c4-a810-839da50dadfe")
+            print(black_lotus.total_words())
+        ```
     """
 
     def __init__(self, card_class: type[CardT] = FullCard):
         self.card_class = card_class
         self.safe_context = False
 
     async def __aenter__(self):
@@ -353,15 +357,15 @@
     async def __aexit__(self, exc_type, exc_val, exc_tb):
         await mongo_close()
 
     # region Card endpoints
 
     @_safe_cache
     @_check_for_safe_context
-    async def get_card_by(self, property_name: str, value) -> CardT:
+    async def get_card_by(self, property_name: str, value: Any) -> CardT:
         """
         Search the database for the first card that matches the given criteria.
 
         Args:
             property_name: The property to check.
             value: The value to match on.
 
@@ -392,15 +396,15 @@
             values: A list of values to match on.
             paginated: Whether to paginate the results.
             page: The page to look at, if paginated.
             page_size: The size of each page, if paginated.
 
         Returns:
             A list of cards matching the search criteria, or empty list if none
-            were found.
+                were found.
 
         Raises:
             RuntimeError: If used outside an `async with` context.
         """
 
         return await card_api.get_cards_by(
             property_name=property_name,
@@ -598,20 +602,20 @@
     # endregion
 
     # region Bulk data I/O
 
     @_check_for_safe_context
     async def load_card_file(self, file_type: ScryfallBulkFile, bulk_file_dir: str):
         """
-        Loads the desired file from the given directory into a local Mongo
-        database. Attempts to download it from Scryfall if it isn't found.
+        Loads the desired file from the given directory into a local database.
+        Attempts to download it from Scryfall if it isn't found.
 
         Args:
             file_type: The type of [ScryfallBulkFile](https://scryfall.com/docs/api/bulk-data)
-            to insert into the database.
+                to insert into the database.
             bulk_file_dir: The path to the folder containing the ScryfallBulkFile.
 
         Raises:
             RuntimeError: If used outside an `async with` context.
         """
 
         return await bulkdata_api.load_card_file(
```

### Comparing `scooze-1.0.6/src/scooze/api/bulkdata.py` & `scooze-1.0.7/src/scooze/api/bulkdata.py`

 * *Files identical despite different names*

### Comparing `scooze-1.0.6/src/scooze/api/card.py` & `scooze-1.0.7/src/scooze/api/card.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 from typing import Any
 
 from beanie import PydanticObjectId
 from scooze.card import CardT, FullCard
 from scooze.errors import BulkAddError
 from scooze.models.card import CardModel, CardModelData
-from scooze.utils import to_lower_camel
+from scooze.utils import scooze_logger, to_lower_camel
+
+logger = scooze_logger()
 
 
 def _normalize_for_ids(property_name: str, value, is_many: bool = False) -> tuple[str, Any | list[Any]]:
     match property_name:
         case "_id" | "id" | "scooze_id":
             prop_name = "_id"
             val = [PydanticObjectId(v) for v in value] if is_many else PydanticObjectId(value)
@@ -99,16 +101,15 @@
     try:
         card_data = CardModelData.model_validate(card.__dict__)
         card_model = CardModel.model_validate(card_data.model_dump(mode="json", by_alias=True))
         await card_model.create()
         card.scooze_id = card_model.id
         return card_model.id
     except Exception as e:
-        # TODO(#75): log error here
-        pass
+        logger.exception("Failed to add card.", extra={"card": card}, exc_info=e)
 
 
 async def add_cards(cards: list[CardT]) -> list[PydanticObjectId]:
     """
     Add a list of cards to the database.
 
     Assign the resulting database IDs to the given Cards.
```

### Comparing `scooze-1.0.6/src/scooze/api/utils.py` & `scooze-1.0.7/src/scooze/api/utils.py`

 * *Files identical despite different names*

### Comparing `scooze-1.0.6/src/scooze/bulkdata.py` & `scooze-1.0.7/src/scooze/bulkdata.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,11 @@
 import os
+from urllib.error import (  # TODO(#153): This allows for autolinking to the HTTPError documentation, but it's bloat, right?
+    HTTPError,
+)
 
 import requests
 from scooze.catalogs import ScryfallBulkFile
 from scooze.utils import DEFAULT_BULK_FILE_DIR
 
 SCRYFALL_BULK_INFO_ENDPOINT = "https://api.scryfall.com/bulk-data"
 
@@ -13,18 +16,18 @@
     bulk_file_dir: str = DEFAULT_BULK_FILE_DIR,
 ) -> None:
     """
     Download a single bulk data file from Scryfall.
 
     Args:
         uri: Location of bulk data file (generally found from bulk info
-          endpoint).
+            endpoint).
         bulk_file_type: Type of bulk file, used to set filename.
         bulk_file_dir: Directory to save bulk files. Defaults to `./data/bulk` if
-          not specified.
+            not specified.
 
     Raises:
         HTTPError: If request for bulk file not successful.
     """
 
     # TODO(#74): flag for check vs existing file; don't overwrite with same file or older version
     with requests.get(uri, stream=True) as r:
@@ -42,15 +45,15 @@
 ) -> None:
     """
     Get a bulk data file from Scryfall, specified by file type (from among ScryfallBulkFile).
 
     Args:
         bulk_file_type: Type of bulk file, used to set filename.
         bulk_file_dir: Directory to save bulk files. Defaults to `./data/bulk` if
-          not specified.
+            not specified.
 
     Raises:
         HTTPError: If request for bulk file not successful.
     """
 
     # get URI from Scryfall bulk endpoint
 
@@ -67,15 +70,15 @@
     bulk_file_dir: str = DEFAULT_BULK_FILE_DIR,
 ) -> None:
     """
     Download all supported Scryfall bulk data files to local filesystem.
 
     Args:
         bulk_file_dir: Directory to save bulk files. Defaults to `./data/bulk` if
-          not specified.
+            not specified.
 
     Raises:
         HTTPError: If request for bulk file not successful.
     """
 
     with requests.get(SCRYFALL_BULK_INFO_ENDPOINT) as bulk_metadata_request:
         bulk_metadata_request.raise_for_status()
```

### Comparing `scooze-1.0.6/src/scooze/card.py` & `scooze-1.0.7/src/scooze/card.py`

 * *Files 16% similar despite different names*

```diff
@@ -28,157 +28,185 @@
     Layout,
     Legality,
     Rarity,
     SecurityStamp,
     SetType,
 )
 from scooze.models.card import CardModel
-from scooze.utils import FloatableT, HashableObject
+from scooze.utils import FloatableT, HashableObject, scooze_logger
+
+logger = scooze_logger()
 
 ## Generic Types
 CardFaceT = TypeVar("CardFaceT", bound=CardFace)  # generic CardFace type
 
 
 class Card(HashableObject):
     """
     A basic Card object with minimal fields. Contains all information you might
     use to sort a decklist.
 
     Attributes:
-        scooze_id: A unique identifier for a document in a scooze database.
-        cmc: This card's mana value/converted mana cost.
-        color_identity: This card's color identity, for Commander variant
-          deckbuilding.
-        colors: This card's colors.
-        legalities: Formats and the legality status of this card in them.
-        mana_cost: Mana cost, as string of mana symbols.
-          (e.g. "{1}{W}{U}{B}{R}{G}")
-        name: This card's name.
-        power: Power of this card, if applicable.
-        toughness: Toughness of this card, if applicable.
-        type_line: This card's type line. (e.g. "Creature — Ooze")
+        name (str | None): This card's name.
+        scooze_id (PydanticObjectId | None): A unique identifier for a document
+            in a scooze database.
+        cmc (float | None): This card's mana value/converted mana cost.
+        color_identity (frozenset[Color] | None): This card's color identity,
+            for Commander variant deckbuilding.
+        colors (frozenset[Color] | None): This card's colors.
+        legalities (frozendict[Format, Legality] | None): Formats and the
+            legality status of this card in them.
+        mana_cost (str | None): Mana cost, as string of mana symbols.
+            (e.g. "{1}{W}{U}{B}{R}{G}")
+        power (str | None): Power of this card, if applicable.
+        toughness (str | None): Toughness of this card, if applicable.
+        type_line (str | None): This card's type line. (e.g. "Creature — Ooze")
     """
 
     def __init__(
         self,
+        name: str | None = None,
         cmc: FloatableT | None = None,
         color_identity: Iterable[Color] | None = None,
         colors: Iterable[Color] | None = None,
         legalities: Mapping[Format, Legality] | None = None,
         mana_cost: str | None = None,
-        name: str | None = None,
         power: str | None = None,
         toughness: str | None = None,
         type_line: str | None = None,
         # kwargs
-        **kwargs,  # TODO(77): log information about kwargs
+        **kwargs,
     ):
         self.scooze_id = CardNormalizer.to_id(id_like=kwargs.get("id"))
 
+        self.name = name
         self.cmc = CardNormalizer.to_float(cmc)
         self.color_identity = CardNormalizer.to_frozenset(color_identity, convert_to_enum=Color)
         self.colors = CardNormalizer.to_frozenset(colors, convert_to_enum=Color)
         self.legalities = CardNormalizer.to_frozendict(
             legalities, convert_key_to_enum=Format, convert_value_to_enum=Legality
         )
         self.mana_cost = mana_cost
-        self.name = name
         self.power = power
         self.toughness = toughness
         self.type_line = type_line
 
+        if kwargs:
+            logger.debug("kwargs found", extra=kwargs)
+
     def __str__(self):
         return self.name
 
     @classmethod
     def from_json(cls, data: dict | str) -> Self:
+        """
+        Create a new Card with the given JSON.
+
+        Args:
+            data: Some JSON to create a scooze Card from.
+        """
         if isinstance(data, dict):
             return cls(**data)
         elif isinstance(data, str):
             return cls(**json.loads(data))
 
     @classmethod
     def from_model(cls, model: CardModel) -> Self:
+        """
+        Create a new Card with the given `CardModel`.
+
+        Args:
+            model: A CardModel to create a scooze Card from.
+        """
         return cls(**model.model_dump())
 
 
 class OracleCard(Card):
     """
-    Card subclass containing all information about a unique card in Magic.
+    A Card object containing all information about a unique card in Magic.
     All information in this class is print-agnostic.
 
     Attributes:
-        scooze_id: A unique identifier for a document in a scooze database.
-        card_faces: All component CardFace objects of this card, for multifaced
-          cards.
-        cmc: This card's mana value/converted mana cost.
-        color_identity: This card's color identity, for Commander variant
-          deckbuilding.
-        color_indicator: The colors in this card's color indicator, if it has
-          one.
-        colors: This card's colors.
-        edhrec_rank: This card's rank/popularity on EDHREC, if applicable.
-        hand_modifier: This card's Vanguard hand size modifier, if applicable.
-        keywords: Keywords and keyword actions this card uses.
-        legalities: Formats and the legality status of this card in them.
-        life_modifier: This card's Vanguard life modifier value, if applicable.
-        loyalty: This card's starting planeswalker loyalty, if applicable.
-        mana_cost: Mana cost, as string of mana symbols.
-          (e.g. "{1}{W}{U}{B}{R}{G}")
-        name: This card's name.
-        oracle_id: A UUID for this card's oracle identity; shared across prints
-          of the same card but not same-named objects with different gameplay
-          properties.
-        oracle_text: This card's oracle text, if any.
-        penny_rank: This card's rank/popularity on Penny Dreadful.
-        power: Power of this card, if applicable.
-        prints_search_uri: A link to begin paginating through all prints of
-          this card in Scryfall's API.
-        produced_mana: Which colors of mana this card can produce.
-        reserved: Whether this card is on the Reserved List.
-        rulings_uri: A link to rulings for this card in Scryfall's API.
-        toughness: Toughness of this card, if applicable.
-        type_line: This card's type line. (e.g. "Creature — Ooze")
+        name (str | None): This card's name.
+        scooze_id (PydanticObjectId | None): A unique identifier for a document
+            in a scooze database.
+        card_faces (tuple[CardFaceT] | None): All component CardFaces of this
+            card, for multifaced cards.
+        cmc (float | None): This card's mana value/converted mana cost.
+        color_identity (frozenset[Color] | None): This card's color identity,
+            for Commander variant deckbuilding.
+        color_indicator (frozenset[Color] | None): The colors in this card's
+            color indicator, if it has one.
+        colors (frozenset[Color] | None): This card's colors.
+        edhrec_rank (int | None): This card's rank/popularity on EDHREC, if
+            applicable.
+        hand_modifier (str | None): This card's Vanguard hand size modifier, if
+            applicable.
+        keywords (frozenset[str] | None): Keywords and keyword actions this
+            card uses.
+        legalities (frozendict[Format, Legality] | None): Formats and the
+            legality status of this card in them.
+        life_modifier (str | None): This card's Vanguard life modifier value,
+            if applicable.
+        loyalty (str | None): This card's starting planeswalker loyalty, if
+            applicable.
+        mana_cost (str | None): Mana cost, as string of mana symbols.
+            (e.g. "{1}{W}{U}{B}{R}{G}")
+        oracle_id (str | None): A UUID for this card's oracle identity; shared
+            across prints of the same card but not same-named objects with
+            different gameplay properties.
+        oracle_text (str | None): This card's oracle text, if any.
+        penny_rank (int | None): This card's rank/popularity on Penny Dreadful.
+        power (str | None): Power of this card, if applicable.
+        prints_search_uri (str | None): A link to begin paginating through all
+            prints of this card in Scryfall's API.
+        produced_mana (frozenset[Color] | None): Which colors of mana this card
+            can produce.
+        reserved (bool | None): Whether this card is on the Reserved List.
+        rulings_uri (str | None): A link to rulings for this card in Scryfall's
+            API.
+        toughness (str | None): Toughness of this card, if applicable.
+        type_line (str | None): This card's type line. (e.g. "Creature — Ooze")
     """
 
     def __init__(
         self,
+        name: str | None = None,
         card_faces: Iterable[CardFace] | None = None,
         cmc: FloatableT | None = None,
         color_identity: Iterable[Color] | None = None,
         color_indicator: Iterable[Color] | None = None,
         colors: Iterable[Color] | None = None,
         edhrec_rank: int | None = None,
         hand_modifier: str | None = None,
         keywords: Iterable[str] = None,
         legalities: Mapping[Format, Legality] = None,
         life_modifier: str | None = None,
         loyalty: str | None = None,
         mana_cost: str | None = None,
-        name: str | None = None,
         oracle_id: str | None = None,
         oracle_text: str | None = None,
         penny_rank: int | None = None,
         power: str | None = None,
         prints_search_uri: str | None = None,
         produced_mana: Iterable[Color] | None = None,
         reserved: bool | None = None,
         rulings_uri: str | None = None,
         toughness: str | None = None,
         type_line: str | None = None,
         # kwargs
-        **kwargs,  # TODO(77): log information about kwargs
+        **kwargs,
     ):
         super().__init__(
+            name=name,
             cmc=cmc,
             color_identity=color_identity,
             colors=colors,
             legalities=legalities,
             mana_cost=mana_cost,
-            name=name,
             power=power,
             toughness=toughness,
             type_line=type_line,
             **kwargs,
         )
         self.scooze_id = CardNormalizer.to_id(id_like=kwargs.get("id"))
 
@@ -196,17 +224,20 @@
         self.produced_mana = CardNormalizer.to_frozenset(produced_mana, convert_to_enum=Color)
         self.reserved = reserved
         self.rulings_uri = rulings_uri
 
     @classmethod
     def oracle_text_without_reminder(cls, oracle_text: str) -> str:
         """
-        Provide the given oracle text with reminder text removed. This is a class method
-        because cards with different faces won't know which face you'd want. Instead you
-        simply pass the text you want to trim reminder text from here.
+        Provide the given oracle text with reminder text removed.
+
+        Note:
+            This is a class method because cards with two unique faces won't
+            know which face you'd want. Instead you simply pass the text from
+            which you want to trim reminder text.
 
         Args:
             oracle_text: The oracle text of a card.
         """
 
         pattern_reminder = r" ?\([^()]+\) ?"  # text between parens ()
         return re.sub(pattern_reminder, "", oracle_text)
@@ -236,139 +267,166 @@
         # Non-MDFC
         else:
             return len(re.findall(pattern_words, OracleCard.oracle_text_without_reminder(self.oracle_text)))
 
 
 class FullCard(OracleCard):
     """
-    Card object that supports all fields available from Scryfall's JSON data.
-    Scryfall documentation: https://scryfall.com/docs/api/cards
+    A Card object that supports all fields available from Scryfall's JSON data.
+    Represents a specific printing of a card.
 
     Attributes:
-        scooze_id: A unique identifier for a document in a scooze database.
-
-    Core fields
-        arena_id: This card's Arena ID, if applicable.
-        scryfall_id: Scryfall's unique ID for this card.
-        lang: The language code for this print;
-          see https://scryfall.com/docs/api/languages
-        mtgo_id: This card's MTGO Catalog ID, if applicable.
-        mtgo_foil_id: This card's foil MTGO Catalog ID, if applicable.
-        multiverse_ids: This card's multiverse IDs on Gatherer, if any.
-        tcgplayer_id: This card's ID on TCGplayer, or `productId` in their
-          system.
-        tcgplayer_etched_id: This card's ID on TCGplayer, for the etched
-          version if that is a separate product.
-        cardmarket_id: This card's ID on Cardmarket, or `idProduct` in their
-          system.
-        oracle_id: A UUID for this card's oracle identity; shared across prints
-          of the same card but not same-named objects with different gameplay
-          properties.
-        prints_search_uri: A link to begin paginating through all prints of
-          this card in Scryfall's API.
-        rulings_uri: A link to rulings for this card in Scryfall's API.
-        scryfall_uri: A link to the Scryfall page for this card.
-        uri: A link to this card object in Scryfall's API.
-
-    Gameplay fields
-        all_parts: RelatedCard objects for tokens/meld pairs/other associated
-          parts to this card, if applicable.
-        card_faces: All component CardFace objects of this card, for multifaced
-          cards.
-        cmc: This card's mana value/converted mana cost.
-        color_identity: This card's color identity, for Commander variant
-          deckbuilding.
-        color_indicator: color_indicator: The colors in this card's color
-          indicator, if it has one.
-        colors: This card's colors.
-        edhrec_rank: This card's rank/popularity on EDHREC, if applicable.
-        hand_modifier: This card's Vanguard hand size modifier, if applicable.
-        keywords: Keywords and keyword actions this card uses.
-        legalities: Formats and the legality status of this card in them.
-        life_modifier: This card's Vanguard life modifier value, if applicable.
-        loyalty: This card's starting planeswalker loyalty, if applicable.
+        name (str | None): This card's name.
+        scooze_id (PydanticObjectId | None): A unique identifier for a document
+            in a scooze database.
+
+        arena_id (int | None): This card's Arena ID, if applicable.
+        scryfall_id (str | None): Scryfall's unique ID for this card.
+        lang (Language | None): The language code for this print;
+            see [here](https://scryfall.com/docs/api/languages)
+        mtgo_id (int | None): This card's MTGO Catalog ID, if applicable.
+        mtgo_foil_id (int | None): This card's foil MTGO Catalog ID, if
+            applicable.
+        multiverse_ids (tuple[int] | None): This card's multiverse IDs on
+            Gatherer, if any.
+        tcgplayer_id (int | None): This card's ID on TCGplayer, or `productId`
+            in their system.
+        tcgplayer_etched_id (int | None): This card's ID on TCGplayer, for the
+            etched version if that is a separate product.
+        cardmarket_id (int | None): This card's ID on Cardmarket, or
+            `idProduct` in their system.
+        oracle_id (str | None): A UUID for this card's oracle identity; shared
+            across prints of the same card but not same-named objects with
+            different gameplay properties.
+        prints_search_uri (str | None): A link to begin paginating through all
+            prints of this card in Scryfall's API.
+        rulings_uri (str | None): A link to rulings for this card in Scryfall's
+            API.
+        scryfall_uri (str | None): A link to the Scryfall page for this card.
+        uri (str | None): A link to this card in Scryfall's API.
+
+        all_parts (tuple[RelatedCard] | None): RelatedCards for tokens/meld
+            pairs/other associated parts to this card, if applicable.
+        card_faces (tuple[CardFaceT] | None): All component CardFaces of this
+            card, for multifaced cards.
+        cmc (float | None): This card's mana value/converted mana cost.
+        color_identity (frozenset[Color] | None): This card's color identity,
+            for Commander variant deckbuilding.
+        color_indicator (frozenset[Color] | None): The colors in this card's
+            color indicator, if it has one.
+        colors (frozenset[Color] | None): This card's colors.
+        edhrec_rank (int | None): This card's rank/popularity on EDHREC, if
+            applicable.
+        hand_modifier (str | None): This card's Vanguard hand size modifier, if
+            applicable.
+        keywords (frozenset[str] | None): Keywords and keyword actions this
+            card uses.
+        legalities (frozendict[Format, Legality] | None): Formats and the
+            legality status of this card in them.
+        life_modifier (str | None): This card's Vanguard life modifier value,
+            if applicable.
+        loyalty (str | None): This card's starting planeswalker loyalty, if
+            applicable.
         mana_cost: Mana cost, as string of mana symbols.
-          (e.g. "{1}{W}{U}{B}{R}{G}")
-        name: This card's name.
-        oracle_text: This card's oracle text, if any.
-        penny_rank: This card's rank/popularity on Penny Dreadful.
-        power: Power of this card, if applicable.
-        produced_mana: Which colors of mana this card can produce.
-        reserved: Whether this card is on the Reserved List.
-        toughness: Toughness of this card, if applicable.
-        type_line: This card's type line. (e.g. "Creature — Ooze")
-
-    Print fields
-        artist: Artist for this card.
-        artist_ids: List of Scryfall IDs for artists of this card.
-        attraction_lights: Attraction lights lit on this card, if applicable.
-        booster: Whether this card can be opened in booster packs.
-        border_color: Border color of this card, from among
-          black, white, borderless, silver, and gold.
-        card_back_id: Scryfall UUID of the card back design for this card.
-        collector_number: This card's collector number; can contain non-numeric
-          characters.
-        content_warning: True if use of this print should be avoided;
-          see https://scryfall.com/blog/regarding-wotc-s-recent-statement-on-depictions-of-racism-220
-        digital: True if this card was only released in a video game.
-        finishes: Finishes this card is available in, from among foil, nonfoil, and etched.
-        flavor_name: Alternate name for this card, such as on Godzilla series.
-        flavor_text: Flavor text on this card, if any.
-        frame_effects: Special frame effects on this card;
-          see https://scryfall.com/docs/api/frames
-        frame: This card's frame layout;
-          see https://scryfall.com/docs/api/frames
-        full_art: Whether this print is full-art.
-        games: Which games this print is available on, from among
-          paper, mtgo, and arena.
-        highres_image: Whether this card has a high-res image available.
-        illustration_id: A UUID for the particular artwork on this print,
-          consistent across art reprints.
-        image_status: The quality/status of images available for this card.
-          Either missing, placeholder, lowres, or highres_scan.
-        image_uris: Links to images of this card in various qualities.
-        layout: This card's printed layout;
-          see https://scryfall.com/docs/api/layouts
-        oversized: Whether this card is oversized.
-        preview: Information about where, when, and how this print was
-          previewed.
-        prices: Prices for this card on various marketplaces.
-        printed_name: Printed name of this card, for localized non-English
-          cards.
-        printed_text: Printed text of this card, for localized non-English
-          cards.
-        printed_type_line: Printed type line of this card, for localized
-          non-English cards.
-        promo: Whether this print is a promo.
-        promo_types: Which promo categories this print falls into, if any.
-        purchase_uris: Links to purchase this print from marketplaces.
-        rarity: The rarity of this print.
-        related_uris: Links to this print's listing on other online resources.
-        released_at: The date this card was first released.
-        reprint: Whether this print is a reprint from an earlier set.
-        scryfall_set_uri: Link to the Scryfall set page for the set of this
-          print.
-        security_stamp: Security stamp on this card, if any.
-        set_name: Full name of the set this print belongs to.
-        set_search_uri: Link to Scryfall API to start paginating through this
-          print's full set.
-        set_type: An overall categorization for each set, provided by Scryfall.
-        set_uri: Link to the set object for this print in Scryfall's API.
-        set_code: Set code of the set this print belongs to.
-        set_id: UUID of the set this print belongs to.
-        story_spotlight: Whether this print is a Story Spotlight.
-        textless: Whether this print is textless.
-        variation: Whether this card print is a variation of another card
-          object.
-        variation_of: Which card object this object is a variant of, if any.
-        watermark: Watermark printed on this card, if any.
+            (e.g. "{1}{W}{U}{B}{R}{G}")
+        oracle_text (str | None): This card's oracle text, if any.
+        oversized (bool | None): Whether this card is oversized.
+        penny_rank (int | None): This card's rank/popularity on Penny Dreadful.
+
+        power (str | None): Power of this card, if applicable.
+        produced_mana (frozenset[Color] | None): Which colors of mana this card
+            can produce.
+        reserved (bool | None): Whether this card is on the Reserved List.
+        toughness (str | None): Toughness of this card, if applicable.
+        type_line (str | None): This card's type line. (e.g. "Creature — Ooze")
+
+        artist (str | None): Artist for this card.
+        artist_ids (tuple[str] | None): List of Scryfall IDs for artists of
+            this card.
+        attraction_lights (frozenset[int] | None): Attraction lights lit on
+            this card, if applicable.
+        booster (bool | None): Whether this card can be opened in booster
+            packs.
+        border_color (BorderColor | None): Border color of this card, from
+            among black, white, borderless, silver, and gold.
+        card_back_id (str | None): Scryfall UUID of the card back design for
+            this card.
+        collector_number (str | None): This card's collector number; can
+            contain non-numeric characters.
+        content_warning (bool): True if use of this print should be avoided;
+            see [here](https://scryfall.com/blog/regarding-wotc-s-recent-statement-on-depictions-of-racism-220)
+        digital (bool | None): True if this card was only released in a video
+            game.
+        finishes (frozenset[Finish] | None): Finishes this card is available
+            in, from among foil, nonfoil, and etched.
+        flavor_name (str | None): Alternate name for this card, such as on
+            Godzilla series.
+        flavor_text (str | None): Flavor text on this card, if any.
+        frame_effects (frozenset[FrameEffect] | None): Special frame effects on
+            this card; see [here](https://scryfall.com/docs/api/frames)
+        frame (frozenset[Frame] | None): This card's frame layout;
+            see [here](https://scryfall.com/docs/api/frames)
+        full_art (bool | None): Whether this print is full-art.
+        games (frozenset[Game] | None): Which games this print is available on,
+            from among paper, mtgo, and arena.
+        highres_image (bool | None): Whether this card has a high-res image
+            available.
+        illustration_id (str | None): A UUID for the particular artwork on this
+            print, consistent across art reprints.
+        image_status (ImageStatus | None): The quality/status of images
+            available for this card. Either missing, placeholder, lowres, or
+            highres_scan.
+        image_uris (ImageUris | None): Links to images of this card in various
+            qualities.
+        layout (Layout | None): This card's printed layout;
+            see [here](https://scryfall.com/docs/api/layouts)
+        preview (Preview | None): Information about where, when, and how this
+            print was previewed.
+        prices (Prices | None): Prices for this card on various marketplaces.
+        printed_name (str | None): Printed name of this card, for localized
+            non-English cards.
+        printed_text (str | None): Printed text of this card, for localized
+            non-English cards.
+        printed_type_line (str | None): Printed type line of this card, for
+            localized non-English cards.
+        promo (bool | None): Whether this print is a promo.
+        promo_types (frozenset[str] | None): Which promo categories this print
+            falls into, if any.
+        purchase_uris (PurchaseUris): Links to purchase this print from
+            marketplaces.
+        rarity (Rarity | None): The rarity of this print.
+        related_uris (RelatedUris): Links to this print's listing on other
+            online resources.
+        released_at (date | None): The date this card was first released.
+        reprint (bool | None): Whether this print is a reprint from an earlier
+            set.
+        scryfall_set_uri (str | None): Link to the Scryfall set page for the
+            set of this print.
+        security_stamp (SecurityStamp | None): Security stamp on this card, if
+            any.
+        set_name (str | None): Full name of the set this print belongs to.
+        set_search_uri (str | None): Link to Scryfall API to start paginating
+            through this print's full set.
+        set_type (SetType | None): An overall categorization for each set,
+            provided by Scryfall.
+        set_uri (str | None): Link to the set for this print in Scryfall's API.
+        set_code (str | None): Set code of the set this print belongs to.
+        set_id (str | None): UUID of the set this print belongs to.
+        story_spotlight (bool | None): Whether this print is a Story Spotlight.
+        textless (bool | None): Whether this print is textless.
+        variation (bool | None): Whether this card print is a variation of
+            another card.
+        variation_of (str | None): Which card this object is a variant of, if
+            any.
+        watermark (str | None): Watermark printed on this card, if any.
     """
 
     def __init__(
         self,
+        name: str | None = None,
         # Core Fields
         arena_id: int | None = None,
         scryfall_id: str | None = None,
         lang: Language | None = None,
         mtgo_id: int | None = None,
         mtgo_foil_id: int | None = None,
         multiverse_ids: Iterable[int] | None = None,
@@ -390,15 +448,14 @@
         edhrec_rank: int | None = None,
         hand_modifier: str | None = None,
         keywords: Iterable[str] | None = None,
         legalities: Mapping[Format, Legality] | None = None,
         life_modifier: str | None = None,
         loyalty: str | None = None,
         mana_cost: str | None = None,
-        name: str | None = None,
         oracle_text: str | None = None,
         oversized: bool | None = None,
         penny_rank: int | None = None,
         power: str | None = None,
         produced_mana: Iterable[Color] | None = None,
         reserved: bool | None = None,
         toughness: str | None = None,
@@ -447,30 +504,30 @@
         set_id: str | None = None,
         story_spotlight: bool | None = None,
         textless: bool | None = None,
         variation: bool | None = None,
         variation_of: str | None = None,
         watermark: str | None = None,
         # kwargs
-        **kwargs,  # TODO(77): log information about kwargs
+        **kwargs,
     ):
         super().__init__(
-            card_faces=None,  # will be overridden with FullCardFace objects
+            name=name,
+            card_faces=None,  # will be overridden with FullCardFaces
             cmc=0,  # will be overridden with reversible card logic
             color_identity=color_identity,
             color_indicator=color_indicator,
             colors=colors,
             edhrec_rank=edhrec_rank,
             hand_modifier=hand_modifier,
             keywords=keywords,
             legalities=legalities,
             life_modifier=life_modifier,
             loyalty=loyalty,
             mana_cost=mana_cost,
-            name=name,
             oracle_id=oracle_id,
             oracle_text=oracle_text,
             penny_rank=penny_rank,
             power=power,
             prints_search_uri=prints_search_uri,
             produced_mana=produced_mana,
             reserved=reserved,
@@ -559,15 +616,16 @@
         self.variation_of = variation_of
         self.watermark = watermark
 
         # endregion
 
     def total_words(self) -> int:
         """
-        The number of words in this card's oracle text (excludes reminder text).
+        The number of words in this card's oracle text (excludes reminder
+        text).
         """
 
         # Don't double count reversible card text
         return int(super().total_words() / (2 if self.layout is Layout.REVERSIBLE_CARD else 1))
 
 
 class CardNormalizer(CardPartsNormalizer):
@@ -596,52 +654,52 @@
             return tuple(RelatedCard(**part) for part in all_parts)
 
     @classmethod
     def to_card_faces(
         cls,
         card_faces: Iterable[CardFaceT] | Iterable[dict] | None,
         card_face_class: type[CardFaceT] = CardFace,
-    ) -> tuple[CardFaceT]:
+    ) -> tuple[CardFaceT] | None:
         """
         Normalize card_faces from JSON.
 
         Args:
-            card_faces: A Iterable[F] or Iterable[JSON] to normalize. F is of type
-              CardFace or FullCardFace.
+            card_faces: A Iterable[F] or Iterable[JSON] to normalize. F is of
+                type CardFace or FullCardFace.
             card_face_class: A CardFace class to create an instance of.
-              (one of CardFace or FullCardFace)
+                (one of CardFace or FullCardFace)
 
         Returns:
             A tuple[F] where F is of type CardFace or FullCardFace.
         """
 
         if card_faces is None or all(isinstance(card_face, card_face_class) for card_face in card_faces):
             return card_faces
         elif all(isinstance(card_face, dict) for card_face in card_faces):
             return tuple(card_face_class.from_json(card_face) for card_face in card_faces)
 
     @classmethod
-    def to_id(cls, id_like: PydanticObjectId | str | None) -> PydanticObjectId:
+    def to_id(cls, id_like: PydanticObjectId | str | None) -> PydanticObjectId | None:
         """
         Normalize ID from JSON.
 
         Args:
-          id_like: A PydanticObjectId or an ID string.
+            id_like: A PydanticObjectId or an ID string.
 
         Returns:
-          A PydanticObjectId.
+            A PydanticObjectId.
         """
 
         if id_like is None or isinstance(id_like, PydanticObjectId):
             return id_like
         elif PydanticObjectId.is_valid(id_like):
             return PydanticObjectId(id_like)
 
     @classmethod
-    def to_preview(cls, preview: Preview | dict | None) -> Preview:
+    def to_preview(cls, preview: Preview | dict | None) -> Preview | None:
         """
         Normalize preview from JSON.
 
         Args:
             preview: An instance of Preview or some JSON to normalize.
 
         Returns:
@@ -650,15 +708,15 @@
 
         if preview is None or isinstance(preview, Preview):
             return preview
         elif isinstance(preview, dict):
             return Preview(**preview)
 
     @classmethod
-    def to_prices(cls, prices: Prices | dict | None) -> Prices:
+    def to_prices(cls, prices: Prices | dict | None) -> Prices | None:
         """
         Normalize prices from JSON.
 
         Args:
             prices: An instance of Prices or some JSON to normalize.
 
         Returns:
@@ -667,8 +725,11 @@
 
         if prices is None or isinstance(prices, Prices):
             return prices
         elif isinstance(prices, dict):
             return Prices(**prices)
 
 
-CardT = TypeVar("CardT", bound=Card)  # generic Card type
+CardT = TypeVar("CardT", bound=Card)
+"""
+A TypeVar for representing Generic Card types.
+"""
```

### Comparing `scooze-1.0.6/src/scooze/cardparts.py` & `scooze-1.0.7/src/scooze/models/cardparts.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,375 +1,332 @@
-import json
 from datetime import date
-from typing import Iterable, Mapping, Self
 
+from pydantic import Field, field_serializer, field_validator
+from scooze.cardparts import ImageUris
 from scooze.catalogs import Color, Component, Layout
-from scooze.utils import FloatableT, HashableObject, JsonNormalizer
+from scooze.models.utils import ScoozeBaseModel
 
 
-class ImageUris(HashableObject):
+class ImageUrisModel(ScoozeBaseModel):
     """
-    URIs of images associated with this object on Scryfall.
-    Scryfall documentation: https://scryfall.com/docs/api/images
+    URIs of images associated with this model on [Scryfall](https://scryfall.com/docs/api/images).
 
     Attributes:
         png: Full card, high quality image with transparent background and
-          rounded corners.
+            rounded corners.
         border_crop: Full card image with corners and majority of border
-          cropped out.
+            cropped out.
         art_crop: Rectangular crop to just art box; may not be perfect for
-          cards with strange layouts.
+            cards with strange layouts.
         large: Large JPG image (672x936)
         normal: Medium JPG image (488x860)
         small: Small JPG image (146x204)
     """
 
-    def __init__(
-        self,
-        png: str | None = None,
-        border_crop: str | None = None,
-        art_crop: str | None = None,
-        large: str | None = None,
-        normal: str | None = None,
-        small: str | None = None,
-        # kwargs
-        **kwargs,  # TODO(77): log information about kwargs
-    ):
-        self.png = png
-        self.border_crop = border_crop
-        self.art_crop = art_crop
-        self.large = large
-        self.normal = normal
-        self.small = small
-
-
-class CardFace(HashableObject):
-    """
-    Object for a single face of a multi-faced OracleCard. Contains only fields that are consistent between card prints.
-    Multi-faced cards include MDFCs, split cards, aftermath, etc.
-
-    Scryfall documentation: https://scryfall.com/docs/api/cards#card-face-objects
+    png: str | None = Field(
+        default=None,
+        description="Full card, high quality image with transparent background and rounded corners.",
+    )
+    border_crop: str | None = Field(
+        default=None,
+        description="Full card image with corners and majority of border cropped out.",
+    )
+    art_crop: str | None = Field(
+        default=None,
+        description="Rectangular crop to just art box; may not be perfect for cards with strange layouts.",
+    )
+    large: str | None = Field(
+        default=None,
+        description="Large JPG image (672x936)",
+    )
+    normal: str | None = Field(
+        default=None,
+        description="Medium JPG image (488x860)",
+    )
+    small: str | None = Field(
+        default=None,
+        description="Small JPG image (146x204)",
+    )
+
+
+class CardFaceModel(ScoozeBaseModel):
+    """
+    A model for a single face of a multi-faced `CardModel`.
+    Multi-faced cards include MDFCs, split cards, aftermath, etc;
+    see [here](https://scryfall.com/docs/api/cards#card-face-objects)
 
     Attributes:
-        cmc: Mana value of this face.
-        color_indicator: Color indicator on this face, if any.
-        colors: Colors of this face.
-        loyalty: Starting planeswalker loyalty of this face, if any.
-        mana_cost: Mana cost of this face.
         name: Name of this face.
-        oracle_id: Oracle ID of this face, for reversible cards.
-        oracle_text: Oracle text of this face, if any.
-        power: Power of this face, if any.
-        toughness: Toughness of this face, if any.
-        type_line: Type line of this face, if any.
-    """
-
-    def __init__(
-        self,
-        cmc: FloatableT | None = None,
-        color_indicator: Iterable[Color] | None = None,
-        colors: Iterable[Color] | None = None,
-        loyalty: str | None = None,
-        mana_cost: str | None = None,
-        name: str | None = None,
-        oracle_id: str | None = None,
-        oracle_text: str | None = None,
-        power: str | None = None,
-        toughness: str | None = None,
-        type_line: str | None = None,
-        # kwargs
-        **kwargs,  # TODO(77): log information about kwargs
-    ):
-        self.cmc = CardPartsNormalizer.to_float(cmc)
-        self.color_indicator = CardPartsNormalizer.to_frozenset(color_indicator)
-        self.colors = CardPartsNormalizer.to_frozenset(colors)
-        self.loyalty = loyalty
-        self.mana_cost = mana_cost
-        self.name = name
-        self.oracle_id = oracle_id
-        self.oracle_text = oracle_text
-        self.power = power
-        self.toughness = toughness
-        self.type_line = type_line
-
-    @classmethod
-    def from_json(cls, data: dict | str) -> Self:
-        if isinstance(data, dict):
-            return cls(**data)
-        elif isinstance(data, str):
-            return cls(**json.loads(data))
-
-
-class FullCardFace(CardFace):
-    """
-    Object for a single face of a multi-faced FullCard.
-    Multi-faced cards include MDFCs, split cards, aftermath, etc.
-
-    Scryfall documentation: https://scryfall.com/docs/api/cards#card-face-objects
-
-    Attributes:
         artist: Illustrator for art on this face.
         artist_id: Scryfall ID for the artist of this face.
         cmc: Mana value of this face.
         color_indicator: Color indicator on this face, if any.
         colors: Colors of this face.
         flavor_text: Flavor text of this face, if any.
         illustration_id: Scryfall illustration ID of this face, if any.
-        image_uris: Scryfall illustration ID of this face, if any.
+        image_uris: URIs for images of this face on Scryfall.
         layout: Layout of this face, if any.
         loyalty: Starting planeswalker loyalty of this face, if any.
         mana_cost: Mana cost of this face.
-        name: Name of this face.
         oracle_id: Oracle ID of this face, for reversible cards.
         oracle_text: Oracle text of this face, if any.
         power: Power of this face, if any.
         printed_name: Printed name of this face, for localized non-English
-          cards.
+            cards.
         printed_text: Printed text of this face, for localized non-English
-          cards.
+            cards.
         printed_type_line: Printed type line of this face, for localized
-          non-English cards.
+            non-English cards.
         toughness: Toughness of this face, if any.
         type_line: Type line of this face, if any.
         watermark: Watermark printed on this face, if any.
     """
 
-    def __init__(
-        self,
-        artist: str | None = None,
-        artist_id: str | None = None,
-        cmc: FloatableT | None = None,
-        color_indicator: Iterable[Color] | None = None,
-        colors: Iterable[Color] | None = None,
-        flavor_text: str | None = None,
-        illustration_id: str | None = None,
-        image_uris: ImageUris | None = None,
-        layout: Layout | None = None,
-        loyalty: str | None = None,
-        mana_cost: str | None = None,
-        name: str | None = None,
-        oracle_id: str | None = None,
-        oracle_text: str | None = None,
-        power: str | None = None,
-        printed_name: str | None = None,
-        printed_text: str | None = None,
-        printed_type_line: str | None = None,
-        toughness: str | None = None,
-        type_line: str | None = None,
-        watermark: str | None = None,
-        # kwargs
-        **kwargs,  # TODO(77): log information about kwargs
-    ):
-        self.artist = artist
-        self.artist_id = artist_id
-        self.cmc = CardPartsNormalizer.to_float(cmc)
-        self.color_indicator = CardPartsNormalizer.to_frozenset(color_indicator, convert_to_enum=Color)
-        self.colors = CardPartsNormalizer.to_frozenset(colors, convert_to_enum=Color)
-        self.flavor_text = flavor_text
-        self.illustration_id = illustration_id
-        self.image_uris = CardPartsNormalizer.to_image_uris(image_uris)
-        self.layout = CardPartsNormalizer.to_enum(Layout, layout)
-        self.loyalty = loyalty
-        self.mana_cost = mana_cost
-        self.name = name
-        self.oracle_id = oracle_id
-        self.oracle_text = oracle_text
-        self.power = power
-        self.printed_name = printed_name
-        self.printed_text = printed_text
-        self.printed_type_line = printed_type_line
-        self.toughness = toughness
-        self.type_line = type_line
-        self.watermark = watermark
+    artist: str | None = Field(
+        default=None,
+        description="Illustrator for art on this face.",
+    )
+    artist_id: str | None = Field(
+        default=None,
+        description="Scryfall ID for the artist of this face.",
+    )
+    cmc: float | None = Field(
+        default=None,
+        description="Mana value of this face.",
+    )
+    color_indicator: set[Color] | None = Field(
+        default=None,
+        description="Color indicator on this face, if any.",
+    )
+    colors: set[Color] | None = Field(
+        default=None,
+        description="Colors of this face.",
+    )
+    flavor_text: str | None = Field(
+        default=None,
+        description="Flavor text of this face, if any.",
+    )
+    illustration_id: str | None = Field(
+        default=None,
+        description="Scryfall illustration ID of this face, if any.",
+    )
+    image_uris: ImageUrisModel | None = Field(
+        default=None,
+        description="URIs for images of this face on Scryfall.",
+    )
+    layout: Layout | None = Field(
+        default=None,
+        description="Layout of this face, if any.",
+    )
+    loyalty: str | None = Field(
+        default=None,
+        description="Starting planeswalker loyalty of this face, if any.",
+    )
+    mana_cost: str = Field(
+        default="",
+        description="Mana cost of this face.",
+    )
+    name: str = Field(
+        description="Name of this face.",
+    )
+    oracle_id: str | None = Field(
+        default=None,
+        description="Oracle ID of this face, for reversible cards.",
+    )
+    oracle_text: str | None = Field(
+        default=None,
+        description="Oracle text of this face, if any.",
+    )
+    power: str | None = Field(
+        default=None,
+        description="Power of this face, if any.",
+    )
+    printed_name: str | None = Field(
+        default=None,
+        description="Printed name of this face, for localized non-English cards.",
+    )
+    printed_text: str | None = Field(
+        default=None,
+        description="Printed text of this face, for localized non-English cards.",
+    )
+    printed_type_line: str | None = Field(
+        default=None,
+        description="Printed type line of this face, for localized non-English cards.",
+    )
+    toughness: str | None = Field(
+        default=None,
+        description="Toughness of this face, if any.",
+    )
+    type_line: str | None = Field(
+        default=None,
+        description="Type line of this face, if any.",
+    )
+    watermark: str | None = Field(
+        default=None,
+        description="Watermark printed on this face, if any.",
+    )
+
+    # region Validators
+
+    @field_validator("image_uris", mode="before")
+    @classmethod
+    def image_uris_validator(cls, v):
+        if isinstance(v, ImageUris):
+            v = ImageUrisModel.model_validate(v.__dict__)
+        return v
+
+    # endregion
 
 
-class Prices(HashableObject):
+class PricesModel(ScoozeBaseModel):
     """
-    Object for all price data associated with a Card object.
+    A model for all price data associated with a `CardModel`.
 
     Attributes:
         usd: Price in US dollars, from TCGplayer.
         usd_foil: Foil price in US dollars, from TCGplayer.
         usd_etched: Etched foil price in US dollars, from TCGplayer.
         eur: Price in Euros, from Cardmarket.
         eur_foil: Foil price in Euros, from Cardmarket.
         tix: Price in MTGO tix, from Cardhoarder.
     """
 
-    def __init__(
-        self,
-        usd: FloatableT | None = None,
-        usd_foil: FloatableT | None = None,
-        usd_etched: FloatableT | None = None,
-        eur: FloatableT | None = None,
-        eur_foil: FloatableT | None = None,
-        tix: FloatableT | None = None,
-        # kwargs
-        **kwargs,  # TODO(77): log information about kwargs
-    ):
-        self.usd = CardPartsNormalizer.to_float(usd)
-        self.usd_foil = CardPartsNormalizer.to_float(usd_foil)
-        self.usd_etched = CardPartsNormalizer.to_float(usd_etched)
-        self.eur = CardPartsNormalizer.to_float(eur)
-        self.eur_foil = CardPartsNormalizer.to_float(eur_foil)
-        self.tix = CardPartsNormalizer.to_float(tix)
+    usd: float | None = Field(
+        default=None,
+        description="Price in US dollars, from TCGplayer.",
+    )
+    usd_foil: float | None = Field(
+        default=None,
+        description="Foil price in US dollars, from TCGplayer.",
+    )
+    usd_etched: float | None = Field(
+        default=None,
+        description="Etched foil price in US dollars, from TCGplayer.",
+    )
+    eur: float | None = Field(
+        default=None,
+        description="Price in Euros, from Cardmarket.",
+    )
+    eur_foil: float | None = Field(
+        default=None,
+        description="Foil price in Euros, from Cardmarket.",
+    )
+    tix: float | None = Field(
+        default=None,
+        description="Price in MTGO tix, from Cardhoarder.",
+    )
 
 
-class Preview(HashableObject):
+class PreviewModel(ScoozeBaseModel):
     """
-    Object for information about where and when a card was previewed.
+    A model for information about where and when a card was previewed.
 
     Attributes:
         previewed_at: Date/time of preview being shown or added to Scryfall.
         source: Name of preview source.
         source_uri: Location of preview source.
     """
 
-    def __init__(
-        self,
-        previewed_at: date | None = None,
-        source: str | None = None,
-        source_uri: str | None = None,
-        # kwargs
-        **kwargs,  # TODO(77): log information about kwargs
-    ):
-        self.previewed_at = CardPartsNormalizer.to_date(previewed_at)
-        self.source = source
-        self.source_uri = source_uri
+    previewed_at: date | None = Field(
+        default=None,
+        description="Date/time of preview being shown or added to Scryfall.",
+    )
+    source: str | None = Field(
+        default=None,
+        description="Name of preview source.",
+    )
+    source_uri: str | None = Field(
+        default=None,
+        description="Location of preview source.",
+    )
+
+    @field_serializer("previewed_at")
+    def serialize_date(self, dt_field: date):
+        return super().serialize_date(dt_field=dt_field)
 
 
-class PurchaseUris(HashableObject):
+class PurchaseUrisModel(ScoozeBaseModel):
     """
-    URIs to this card’s listing on major marketplaces.
+    URIs to this card's listings on major marketplaces.
 
     Attributes:
         tcgplayer: Link to buy this card on the TCGplayer marketplace.
         cardmarket: Link to buy this card on the Cardmarket marketplace.
         cardhoarder: Link to buy this card digitally for MTGO on Cardhoarder.
     """
 
-    def __init__(
-        self,
-        tcgplayer: str | None = None,
-        cardmarket: str | None = None,
-        cardhoarder: str | None = None,
-    ):
-        self.tcgplayer = tcgplayer
-        self.cardmarket = cardmarket
-        self.cardhoarder = cardhoarder
+    tcgplayer: str | None = Field(
+        default=None,
+        description="Link to buy this card on the TCGplayer marketplace.",
+    )
+    cardmarket: str | None = Field(
+        default=None,
+        description="Link to buy this card on the Cardmarket marketplace.",
+    )
+    cardhoarder: str | None = Field(
+        default=None,
+        description="Link to buy this card digitally for MTGO on Cardhoarder.",
+    )
 
 
-class RelatedCard(HashableObject):
+class RelatedCardModel(ScoozeBaseModel):
     """
-    Data about Scryfall objects related to this card
+    Data about [Scryfall](https://scryfall.com/docs/api/cards#related-card-objects) objects related to this card
     (tokens, cards referenced by name, meld pairs, etc.)
 
-    Scryfall documentation: https://scryfall.com/docs/api/cards#related-card-objects
 
     Attributes:
+        name: Name of linked component.
         scryfall_id: ID of linked component.
         component: One of `token`, `meld_part`, `meld_result`, or
-          `combo_piece`.
-        name: Name of linked component.
+            `combo_piece`.
         type_line: Type line of linked component.
         uri: URI of linked component.
     """
 
-    def __init__(
-        self,
-        id: str = "",  # Alias for scryfall_id
-        scryfall_id: str = "",
-        component: Component | None = None,
-        name: str | None = None,
-        type_line: str | None = None,
-        uri: str | None = None,
-        # kwargs
-        **kwargs,  # TODO(77): log information about kwargs
-    ):
-        self.scryfall_id = scryfall_id if scryfall_id else id
-        self.component = CardPartsNormalizer.to_enum(Component, component)
-        self.name = name
-        self.type_line = type_line
-        self.uri = uri
+    scryfall_id: str = Field(
+        description="ID of linked component.",
+        alias="id",
+    )  # Scryfall ID
+    component: Component = Field(
+        description="One of `token`, `meld_part`, `meld_result`, or `combo_piece`.",
+    )
+    name: str = Field(
+        description="Name of linked component.",
+    )
+    type_line: str = Field(
+        description="Type line of linked component.",
+    )
+    uri: str = Field(
+        description="URI of linked component.",
+    )
 
 
-class RelatedUris(HashableObject):
+class RelatedUrisModel(ScoozeBaseModel):
     """
     Links to information about a Scryfall-based card object on other non-Scryfall resources.
 
     Attributes:
-        edhrec
-        gatherer
-        tcgplayer_infinite_articles
-        tcgplayer_infinite_decks
-    """
-
-    def __init__(
-        self,
-        edhrec: str | None = None,
-        gatherer: str | None = None,
-        tcgplayer_infinite_articles: str | None = None,
-        tcgplayer_infinite_decks: str | None = None,
-    ):
-        self.edhrec = edhrec
-        self.gatherer = gatherer
-        self.tcgplayer_infinite_articles = tcgplayer_infinite_articles
-        self.tcgplayer_infinite_decks = tcgplayer_infinite_decks
-
-
-class CardPartsNormalizer(JsonNormalizer):
-    """
-    A simple class to be used when normalizing non-serializable data from JSON.
-    """
-
-    @classmethod
-    def to_image_uris(cls, image_uris: ImageUris | Mapping[str, str] | None) -> ImageUris:
-        """
-        Normalize image_uris from JSON.
-
-        Args:
-            image_uris: An instance of ImageUris or some JSON to normalize.
-
-        Returns:
-            An instance of ImageUris.
-        """
-
-        if image_uris is None or isinstance(image_uris, ImageUris):
-            return image_uris
-
-        return ImageUris(**image_uris)
-
-    @classmethod
-    def to_purchase_uris(cls, purchase_uris: PurchaseUris | Mapping[str, str] | None) -> PurchaseUris:
-        """
-        Normalize purchase_uris from JSON.
-
-        Args:
-            purchase_uris: An instance of PurchaseUris or some JSON to normalize.
-        Returns:
-             An instance of PurchaseUris.
-        """
-
-        if purchase_uris is None:
-            return PurchaseUris()
-        elif isinstance(purchase_uris, PurchaseUris):
-            return purchase_uris
-
-        return PurchaseUris(**purchase_uris)
-
-    @classmethod
-    def to_related_uris(cls, related_uris: RelatedUris | Mapping[str, str] | None) -> RelatedUris:
-        """
-        Normalize related_uris from JSON.
-
-        Args:
-            related_uris: An instance of RelatedUris or some JSON to normalize.
-        Returns:
-             An instance of RelatedUris.
-        """
-
-        if related_uris is None:
-            return RelatedUris()
-        elif isinstance(related_uris, RelatedUris):
-            return related_uris
-
-        return RelatedUris(**related_uris)
+        edhrec: Link to EDHREC
+        gatherer: Link to gatherer.wizards.com
+        tcgplayer_infinite_articles: Link to
+            [infinite.tcgplayer.com/magic-the-gathering/articles](https://infinite.tcgplayer.com/magic-the-gathering/articles)
+        tcgplayer_infinite_decks: Link to
+            [infinite.tcgplayer.com/magic-the-gathering/decks](https://infinite.tcgplayer.com/magic-the-gathering/decks)
+    """
+
+    edhrec: str | None = Field(
+        default=None,
+        description="Information about this card on edhrec.",
+    )
+    gatherer: str | None = Field(
+        default=None,
+        description="Information about this card on Gatherer.",
+    )
+    tcgplayer_infinite_articles: str | None = Field(
+        default=None,
+        description="Articles about this card on TCGplayer Infinite.",
+    )
+    tcgplayer_infinite_decks: str | None = Field(
+        default=None,
+        description="Decks including this card on TCGplayer Infinite.",
+    )
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `scooze-1.0.6/src/scooze/catalogs.py` & `scooze-1.0.7/src/scooze/catalogs.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,38 +1,12 @@
-from enum import Enum, EnumMeta, StrEnum, auto
+from enum import StrEnum, auto
 from functools import cache
 from typing import FrozenSet
 
-# region Enum Extensions
-
-
-class CaseInsensitiveEnumMeta(EnumMeta):
-    """
-    An extension of the classic Python EnumMeta to support case-insensitive
-    fields.
-    """
-
-    def __getitem__(self, item):
-        if isinstance(item, str):
-            item = item.upper()
-        return super().__getitem__(item)
-
-
-class ExtendedEnum(Enum, metaclass=CaseInsensitiveEnumMeta):
-    """
-    An extension of the classic Python Enum to support additional
-    functionality.
-    """
-
-    @classmethod
-    def list(cls):
-        return list(map(lambda c: c.value, cls))
-
-
-# endregion
+from scooze.enum import ExtendedEnum
 
 # region Card Enums
 
 
 class BorderColor(ExtendedEnum, StrEnum):
     """
     A color that borders of Magic cards can be.
@@ -59,16 +33,16 @@
     # Not a color, but Scryfall uses this in `produced_mana` as a type that can be produced.
     COLORLESS = "C"
 
 
 class Component(ExtendedEnum, StrEnum):
     """
     A type of related object, used in Scryfall to link a card
-    to other cards or tokens referenced by it.
-    See https://scryfall.com/docs/api/cards for documentation.
+    to other cards or tokens referenced by it; see
+    [here](https://scryfall.com/docs/api/cards)
     """
 
     MELD_PART = auto()
     MELD_RESULT = auto()
     TOKEN = auto()
     COMBO_PIECE = auto()  # Generally a card referenced directly in rules text, in either direction.
 
@@ -92,15 +66,14 @@
     BRAWL = auto()
     COMMANDER = auto()
     DUEL = auto()
     EXPLORER = auto()
     FUTURE = auto()
     GLADIATOR = auto()
     HISTORIC = auto()
-    HISTORICBRAWL = auto()
     LEGACY = auto()
     MODERN = auto()
     OATHBREAKER = auto()
     OLDSCHOOL = auto()
     PAUPER = auto()
     PAUPERCOMMANDER = auto()
     PENNY = auto()
@@ -173,28 +146,28 @@
     ASTRAL = auto()
     SEGA = auto()
 
 
 class ImageStatus(ExtendedEnum, StrEnum):
     """
     An indicator for whether a card's image exists on Scryfall,
-    and how high quality the sourced image is.
-    See https://scryfall.com/docs/api/images for documentation.
+    and how high quality the sourced image is; see
+    [here](https://scryfall.com/docs/api/images)
     """
 
     MISSING = auto()
     PLACEHOLDER = auto()
     LOWRES = auto()
     HIGHRES_SCAN = auto()
 
 
 class Language(ExtendedEnum, StrEnum):
     """
-    A language that Magic cards have been printed in, using Scryfall's language codes.
-    See https://scryfall.com/docs/api/languages for documentation.
+    A language that Magic cards have been printed in, using Scryfall's language
+    codes; see [here](https://scryfall.com/docs/api/languages)
     """
 
     ENGLISH = "en"
     SPANISH = "es"
     FRENCH = "fr"
     GERMAN = "de"
     ITALIAN = "it"
@@ -220,14 +193,15 @@
     """
 
     NORMAL = auto()
     ADVENTURE = auto()
     ART_SERIES = auto()
     AUGMENT = auto()
     BATTLE = auto()
+    CASE = auto()
     CLASS = auto()
     DOUBLE_FACED_TOKEN = auto()
     EMBLEM = auto()
     FLIP = auto()
     HOST = auto()
     LEVELER = auto()
     MELD = auto()
@@ -297,16 +271,16 @@
     CIRCLE = auto()  # Signature Spellbook style
     HEART = auto()  # My Little Pony
     TRIANGLE = auto()  # Universes Beyond
 
 
 class SetType(ExtendedEnum, StrEnum):
     """
-    A Scryfall-provided categorization for a set.
-    See https://scryfall.com/docs/api/sets for documentation.
+    A Scryfall-provided categorization for a set; see
+    [here](https://scryfall.com/docs/api/sets)
     """
 
     ALCHEMY = auto()
     ARCHENEMY = auto()
     ARSENAL = auto()
     BOX = auto()
     COMMANDER = auto()
@@ -584,102 +558,136 @@
 
     # endregion
 
     # region Properties for types of symbol
 
     @property
     def is_generic(self) -> bool:
+        """
+        Determine if this mana symbol is generic.
+
+        Example:
+            ``` python
+            CostSymbol.GENERIC_1.is_generic()
+            ```
+        """
+
         return self in CostSymbol._generic_symbols()
 
     @property
     def is_half(self) -> bool:
+        """
+        Determine if this mana symbol is half.
+
+        Example:
+            ``` python
+            CostSymbol.GENERIC_HALF.is_half()
+            ```
+        """
+
         return self in CostSymbol._half_symbols()
 
     @property
     def is_hybrid(self) -> bool:
+        """
+        Determine if this mana symbol is hybrid.
+
+        Example:
+            ``` python
+            CostSymbol.HYBRID_RG.is_hybrid()
+            ```
+        """
+
         return self in CostSymbol._hybrid_symbols()
 
     @property
     def is_phyrexian(self) -> bool:
+        """
+        Determine if this mana symbol is Phyrexian.
+
+        Example:
+            ``` python
+            CostSymbol.PHYREXIAN_BLUE.is_phyrexian()
+            ```
+        """
+
         return self in CostSymbol._phyrexian_symbols()
 
     @property
     def is_twobrid(self) -> bool:
+        """
+        Determine if this mana symbol is a twobrid.
+
+        Example:
+            ``` python
+            CostSymbol.TWOBRID_WHITE.is_twobrid()
+            ```
+        """
+
         return self in CostSymbol._twobrid_symbols()
 
     @property
     def is_variable(self) -> bool:
+        """
+        Determine if this mana symbol is variable.
+
+        Example:
+            ``` python
+            CostSymbol.GENERIC_X.is_variable()
+            ```
+        """
+
         return self in CostSymbol._variable_symbols()
 
     @property
     def is_un(self) -> bool:
+        """
+        Determine if this mana symbol is from an "Un"-set.
+
+        Example:
+            ``` python
+            CostSymbol.GENERIC_100.is_un()
+            ```
+        """
+
         return self in CostSymbol._un_symbols()
 
     @property
     def is_nonmana(self) -> bool:
+        """
+        Determine if this mana symbol is non-mana.
+
+        Example:
+            ``` python
+            CostSymbol.TAP.is_nonmana()
+            ```
+        """
+
         return self in CostSymbol._nonmana_symbols()
 
     # endregion
 
     @property
     def mana_value_contribution(self) -> float:
         """
-        The contribution to mana value for this mana symbol.
+        The numerical mana value for this symbol; will be integer valued except
+        for 1/2 mana symbols from "Un"-sets.
 
-        Returns:
-            Numerical mana value for this symbol; will be integer valued except for 1/2 mana symbols from unsets.
+        Example:
+            ``` python
+            CostSymbol.GREEN.mana_value_contribution()
+            >>> 1
+            ```
         """
 
         if self.is_nonmana or self.is_variable:
             return 0
         if self.is_twobrid:
             return 2
         if self.is_half:
             return 0.5
         if self.is_generic:
             return float(self)
         return 1
 
 
 # endregion
-
-
-# region Deck Enums
-
-
-class InThe(ExtendedEnum, StrEnum):
-    """
-    The location of a Card in a Deck.
-    """
-
-    MAIN = auto()
-    SIDE = auto()
-    CMDR = auto()
-    ATTRACTIONS = auto()
-    STICKERS = auto()
-
-
-class DecklistFormatter(ExtendedEnum, StrEnum):
-    """
-    A method of formatting a decklist for external systems.
-    """
-
-    ARENA = auto()
-    MTGO = auto()
-
-
-# endregion
-
-
-# region Database Enums
-
-
-class DbCollection(ExtendedEnum, StrEnum):
-    """
-    Collections in the Scooze database.
-    """
-
-    CARDS = "cards"
-    DECKS = "decks"
-
-
-# endregion
```

### Comparing `scooze-1.0.6/src/scooze/console/cli.py` & `scooze-1.0.7/src/scooze/console/cli.py`

 * *Files identical despite different names*

### Comparing `scooze-1.0.6/src/scooze/console/commands/delete.py` & `scooze-1.0.7/src/scooze/console/commands/delete.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import scooze.database.deck as deck_db
 from cleo.commands.command import Command
 from cleo.helpers import argument
 from scooze.api import ScoozeApi
-from scooze.catalogs import DbCollection
+from scooze.database.core import DbCollection
 
 ACCEPTED_DELETE_ARGS = {
     "all",
     "cards",
     "decks",
 }
```

### Comparing `scooze-1.0.6/src/scooze/console/commands/load/cards.py` & `scooze-1.0.7/src/scooze/console/commands/load/cards.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
         option("all", description="Every print of all cards and game objects in all languages."),
         option("artwork", description="Includes each unique illustration once."),
         option("oracle", description="One version of each card ever printed."),
         option("prints", description="Every print of each card ever printed, in English where available."),
         option("test", description="The Power 9, for testing purposes."),
         option(
             "bulk-data-dir",
-            description="Directory to store bulk files, used with load-cards.",
+            description="Directory to store bulk files, used with load cards.",
             default=DEFAULT_BULK_FILE_DIR,
             value_required=True,
             flag=False,
         ),
     ]
 
     def handle(self):
```

### Comparing `scooze-1.0.6/src/scooze/console/commands/load/decks.py` & `scooze-1.0.7/src/scooze/console/commands/load/decks.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,15 +15,15 @@
     description = "Load sets of decks into the database."
 
     options = [
         option("all", description="All decks in the decks directory."),
         option("test", description="A set of Pioneer decks for testing purposes."),
         option(
             "decks-dir",
-            description="Directory to store deck files, used with load-decks.",
+            description="Directory to store deck files, used with load decks.",
             default=DEFAULT_DECKS_DIR,
             value_required=True,
             flag=False,
         ),
     ]
 
     def handle(self):
```

### Comparing `scooze-1.0.6/src/scooze/console/commands/setup/docker.py` & `scooze-1.0.7/src/scooze/console/commands/setup/docker.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,31 +1,37 @@
 import subprocess
 
 import docker
 from cleo.commands.command import Command
+from docker.errors import APIError, ImageNotFound
 
 
 class SetupDockerCommand(Command):
     name = "setup docker"
     description = "Setup MongoDB in a Docker container."
 
     def handle(self):
         # Check if Docker is installed and running
         p = subprocess.run(
             "docker stats --no-stream",
             stdout=subprocess.DEVNULL,
             stderr=subprocess.STDOUT,
             shell=True,
         )
-        if not p.returncode:
-            client = docker.from_env()
-            # Check if Docker container is already running
-            containers = client.containers.list(all=True)
-            if "scooze-mongodb" in [container.name for container in containers]:
-                self.line("Scooze mongodb container already exists! Exiting.")
-            else:
-                self.line("Setting up latest MongoDB Docker container as scooze-mongodb...")
-                # Start Docker container
-                client.containers.run("mongo:latest", detach=True, ports=({"27017/tcp": 27017}), name="scooze-mongodb")
-                self.line("Done. MongoDB running on localhost:27017.")
-        else:
+        if p.returncode:
             self.line("Cannot connect to Docker daemon -- Is docker installed and running?")
+            return
+        client = docker.from_env()
+        try:
+            scooze_container = client.containers.get("scooze-mongodb")
+        except (APIError, ImageNotFound):
+            # image doesn't yet exist; create and start it
+            self.line("Setting up latest MongoDB Docker container as scooze-mongodb...")
+            # Start Docker container
+            client.containers.run("mongo:latest", detach=True, ports=({"27017/tcp": 27017}), name="scooze-mongodb")
+            self.line("Done. MongoDB running on localhost:27017.")
+            return
+        if scooze_container.status == "running":
+            self.line("scooze mongodb container already running! Exiting.")
+        else:
+            self.line("scooze mongodb container exists, but not running; starting...")
+            scooze_container.start()
```

### Comparing `scooze-1.0.6/src/scooze/console/commands/teardown/docker.py` & `scooze-1.0.7/src/scooze/console/commands/teardown/docker.py`

 * *Files identical despite different names*

### Comparing `scooze-1.0.6/src/scooze/database/core.py` & `scooze-1.0.7/src/scooze/database/core.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,32 @@
+from enum import StrEnum
 from typing import Any
 
 from bson import ObjectId
 from pymongo import ReturnDocument
 from pymongo.results import DeleteResult
-from scooze.catalogs import DbCollection
 from scooze.database.mongo import db
+from scooze.enum import ExtendedEnum
 from scooze.utils import to_lower_camel
 
+# region Database Enums
+
+
+class DbCollection(ExtendedEnum, StrEnum):
+    """
+    Collections in the scooze database.
+    """
+
+    CARDS = "cards"
+    DECKS = "decks"
+
+
+# endregion
+
+
 # region Single document
 
 
 async def insert_document(coll_type: DbCollection, document: dict[str, Any]):
     """
     Insert a document into a collection in the database.
```

### Comparing `scooze-1.0.6/src/scooze/database/deck.py` & `scooze-1.0.7/src/scooze/database/deck.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from typing import Any
 
 import scooze.database.core as db_core
 from bson import ObjectId
-from scooze.catalogs import DbCollection
+from scooze.database.core import DbCollection
 from scooze.models.deck import DeckModelIn, DeckModelOut
 
 # region Deck
 
 
 async def add_deck(deck: DeckModelIn) -> DeckModelOut:
     """
```

### Comparing `scooze-1.0.6/src/scooze/database/mongo.py` & `scooze-1.0.7/src/scooze/database/mongo.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 
 class Database:
     """
     A simple database object to house the Motor client.
 
     Attributes:
-        client: An AsyncIOMotorClient for managing Scooze's MongoDB connection.
+        client: An AsyncIOMotorClient for managing scooze's MongoDB connection.
     """
 
     client: AsyncIOMotorClient = None
 
 
 db = Database()
```

### Comparing `scooze-1.0.6/src/scooze/deck.py` & `scooze-1.0.7/src/scooze/deck.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,83 +1,116 @@
 from collections import Counter
+from enum import StrEnum, auto
 from sys import maxsize
 from typing import Generic, Self
 
 import scooze.utils as utils
 from scooze.card import CardT
-from scooze.catalogs import DecklistFormatter, Format, InThe, Legality
+from scooze.catalogs import Format, Legality
 from scooze.deckpart import DeckDiff, DeckPart
+from scooze.enum import ExtendedEnum
+from scooze.utils import ComparableObject
 
+logger = utils.scooze_logger()
 
-class Deck(utils.ComparableObject, Generic[CardT]):
+# region Deck Enums
+
+
+class InThe(ExtendedEnum, StrEnum):
+    """
+    The location of a Card in a Deck.
+    """
+
+    MAIN = auto()
+    SIDE = auto()
+    CMDR = auto()
+    ATTRACTIONS = auto()
+    STICKERS = auto()
+
+
+class DecklistFormatter(ExtendedEnum, StrEnum):
+    """
+    A method of formatting a decklist for external systems.
+    """
+
+    ARENA = auto()
+    MTGO = auto()
+
+
+# endregion
+
+
+class Deck(ComparableObject, Generic[CardT]):
     """
     A class to represent a deck of Magic: the Gathering cards.
 
     Attributes:
-        archetype: The archetype of this Deck.
-        format: The format legality of the cards in this Deck.
-        main: The main deck. Typically 60 cards minimum.
-        side: The sideboard. Typically 15 cards maximum.
-        cmdr: The command zone. Typically 1 or 2 cards in Commander formats.
-        attractions: The attraction deck.
-        stickers: The sticker deck.
+        archetype (str | None): The archetype of this Deck.
+        format (Format): The format legality of the cards in this Deck.
+        main (DeckPart[CardT]): The main deck. Typically 60 cards minimum.
+        side (DeckPart[CardT]): The sideboard. Typically 15 cards maximum.
+        cmdr (DeckPart[CardT]): The command zone. Typically 1 or 2 cards in Commander formats.
+        attractions (DeckPart[CardT]): The attraction deck.
+        stickers (DeckPart[CardT]): The sticker deck.
+        companion (CardT | None): This deck's companion (if applicable).
     """
 
     def __init__(
         self,
         archetype: str | None = None,
         format: Format = Format.NONE,
-        main: DeckPart[CardT] = None,
-        side: DeckPart[CardT] = None,
-        cmdr: DeckPart[CardT] = None,
-        attractions: DeckPart[CardT] = None,
-        stickers: DeckPart[CardT] = None,
-        companion: CardT = None,
+        main: DeckPart[CardT] | None = None,
+        side: DeckPart[CardT] | None = None,
+        cmdr: DeckPart[CardT] | None = None,
+        attractions: DeckPart[CardT] | None = None,
+        stickers: DeckPart[CardT] | None = None,
+        companion: CardT | None = None,
     ):
         self.archetype = archetype
         self.format = format
 
         self.main = main if main is not None else DeckPart()
         self.side = side if side is not None else DeckPart()
         self.cmdr = cmdr if cmdr is not None else DeckPart()
         self.attractions = attractions if attractions is not None else DeckPart()
         self.stickers = stickers if stickers is not None else DeckPart()
 
         self.companion = companion
 
     @property
     def cards(self) -> Counter[CardT]:
+        """
+        Get this Deck as a collection of cards.
+        """
         return self.main.cards + self.side.cards + self.cmdr.cards + self.attractions.cards + self.stickers.cards
 
     def __str__(self):
         decklist = self.export()
         return f"""Archetype: {self.archetype}\n""" f"""Format: {self.format}\n""" f"""Decklist:\n{decklist}\n"""
 
+    # TODO(#112): Add type filters.
+    # TODO(#113): Reversible cards do not have a top-level cmc. Assign one?
     def average_cmc(self) -> float:
         """
         The average mana value of cards in this Deck.
         """
 
-        # TODO(#112): Add type filters.
-        # TODO(#113): Reversible cards do not have a top-level cmc. Assign one?
-
         total_cards = self.total_cards()
 
         if total_cards > 0:
             return self.total_cmc() / self.total_cards()
         return 0
 
+    # TODO(#112): Add type filters.
     def average_words(self) -> float:
         """
         The average number of words across all oracle text on all cards in this
         Deck (excludes reminder text).
         """
 
-        # TODO(#112): Add type filters.
-
         total_cards = self.total_cards()
 
         if total_cards > 0:
             return self.total_words() / self.total_cards()
         return 0
 
     def diff(self, other: Self) -> DeckDiff:
@@ -85,15 +118,15 @@
         Generate a diff between this Deck and another.
 
         Args:
             other: The other Deck.
 
         Returns:
             A DeckDiff with keys for each deck part. Each contains a dict of
-            each card in both decks and their counts.
+                each card in both decks and their counts.
         """
 
         return DeckDiff(
             main=self.main.diff(other.main),
             side=self.side.diff(other.side),
             cmdr=self.cmdr.diff(other.cmdr),
             attractions=self.attractions.diff(other.attractions),
@@ -105,15 +138,15 @@
         Determine if this Deck contains exactly the same cards as another.
 
         Args:
             other: The other Deck.
 
         Returns:
             True if this Deck contains exactly the same cards as another, else
-            False.
+                False.
         """
 
         if self.total_cards() != other.total_cards():
             return False
 
         diff = self.diff(other)
         same_main = not bool(diff.main)
@@ -129,15 +162,15 @@
         Export this Deck as a string with the given DecklistFormatter.
 
         Args:
             export_format: The format of the exported Deck.
 
         Returns:
             A string containing the names and quantities of the cards in this
-            Deck.
+                Deck.
         """
 
         match export_format:
             case DecklistFormatter.ARENA:
                 cmdr_prefix = "Commander\n"
                 companion_prefix = "Companion\n"
                 main_prefix = "Deck\n"
@@ -291,15 +324,16 @@
             case InThe.CMDR:
                 self.cmdr.add_card(card=card, quantity=quantity)
             case InThe.ATTRACTIONS:
                 self.attractions.add_card(card=card, quantity=quantity)
             case InThe.STICKERS:
                 self.stickers.add_card(card=card, quantity=quantity)
             case _:
-                pass  # TODO(#75): 'in' must be one of InThe.list()
+                logger.info("Failed to add card.", extra={"card": card})
+                logger.warning(f'in_the "{in_the}" not found. Must be one of {InThe.list()}')
 
     def add_cards(self, cards: Counter[CardT], in_the: InThe = InThe.MAIN) -> None:
         """
         Add the given cards to this Deck.
 
         Args:
             cards: The cards to add.
@@ -338,34 +372,35 @@
             case InThe.CMDR:
                 self.cmdr.remove_card(card=card, quantity=quantity)
             case InThe.ATTRACTIONS:
                 self.attractions.remove_card(card=card, quantity=quantity)
             case InThe.STICKERS:
                 self.stickers.remove_card(card=card, quantity=quantity)
             case _:
-                pass  # TODO(#75): failed to remove card
+                logger.info("Failed to remove card.", extra={"card": card})
+                logger.warning(f'in_the "{in_the}" not found. Must be one of {InThe.list()}')
 
     def remove_cards(self, cards: Counter[CardT], in_the: InThe = InThe.MAIN) -> None:
         """
         Remove the given cards from this Deck.
 
         Args:
             cards: The cards to remove.
             in_the: Where to remove the cards from (main, side, etc.)
         """
 
-        # using counterA - counterB results in a new Counter with only positive results
         match in_the:
             case InThe.MAIN:
                 self.main.remove_cards(cards=cards)
             case InThe.SIDE:
                 self.side.remove_cards(cards=cards)
             case InThe.CMDR:
                 self.cmdr.remove_cards(cards=cards)
             case InThe.ATTRACTIONS:
                 self.attractions.remove_cards(cards=cards)
             case InThe.STICKERS:
                 self.stickers.remove_cards(cards=cards)
             case _:
-                pass  # TODO(#75): failed to remove cards
+                logger.info("Failed to remove cards.")
+                logger.warning(f'in_the "{in_the}" not found. Must be one of {InThe.list()}')
 
     # endregion
```

### Comparing `scooze-1.0.6/src/scooze/deckpart.py` & `scooze-1.0.7/src/scooze/deckpart.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,19 +7,19 @@
 
 
 class DeckDiff(ComparableObject):
     """
     A class to represent a diff between two decks.
 
     Attributes:
-        main: The diff between the main decks of two Decks.
-        side: The diff between the sideboards of two Decks.
-        cmdr: The diff between the command zones of two Decks.
-        attractions: The diff between the attractions of the two Decks.
-        stickers: The diff between the stickers fo the two Decks.
+        main (DictDiff): The diff between the main decks of two Decks.
+        side (DictDiff): The diff between the sideboards of two Decks.
+        cmdr (DictDiff): The diff between the command zones of two Decks.
+        attractions (DictDiff): The diff between the attractions of the two Decks.
+        stickers (DictDiff): The diff between the stickers of the two Decks.
     """
 
     def __init__(
         self,
         main: DictDiff,
         side: DictDiff = None,
         cmdr: DictDiff = None,
@@ -52,26 +52,26 @@
 
             return diff
 
         return ""
 
     def total(self) -> int:
         """
-        The number of Cards in this DeckDiff.
+        The number of cards in this DeckDiff.
         """
 
         return sum(map(len, (self.main, self.side, self.cmdr, self.attractions, self.stickers)))
 
 
 class DeckPart(ComparableObject, Generic[CardT]):
     """
     A class to represent a part of a deck.
 
     Attributes:
-        cards: The cards in this DeckPart.
+        cards (Counter[CardT]): The cards in this DeckPart.
     """
 
     def __init__(self, cards: Counter[CardT] = None):
         self.cards = cards if cards is not None else Counter()
 
     def __getitem__(self, key: CardT):
         return self.cards[key]
```

### Comparing `scooze-1.0.6/src/scooze/main.py` & `scooze-1.0.7/src/scooze/main.py`

 * *Files identical despite different names*

### Comparing `scooze-1.0.6/src/scooze/models/card.py` & `scooze-1.0.7/src/scooze/models/card.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,38 +1,38 @@
 from datetime import date
 from typing import Any
 
-from pydantic import ConfigDict, Field, field_serializer, field_validator
+from pydantic import AliasChoices, ConfigDict, Field, field_serializer, field_validator
 from scooze.cardparts import (
     CardFace,
     FullCardFace,
     ImageUris,
     Preview,
     Prices,
     PurchaseUris,
     RelatedCard,
     RelatedUris,
 )
 from scooze.catalogs import (
     BorderColor,
     Color,
-    DbCollection,
     Finish,
     Format,
     Frame,
     FrameEffect,
     Game,
     ImageStatus,
     Language,
     Layout,
     Legality,
     Rarity,
     SecurityStamp,
     SetType,
 )
+from scooze.database.core import DbCollection
 from scooze.models.cardparts import (
     CardFaceModel,
     ImageUrisModel,
     PreviewModel,
     PricesModel,
     PurchaseUrisModel,
     RelatedCardModel,
@@ -40,150 +40,145 @@
 )
 from scooze.models.utils import ScoozeBaseModel, ScoozeDocument
 from scooze.utils import DATE_FORMAT
 
 
 class CardModelData(ScoozeBaseModel):
     """
-    Card object that supports all fields available from Scryfall's JSON data.
-    Scryfall documentation: https://scryfall.com/docs/api/cards
+    A Card object that supports all fields available from Scryfall's JSON data.
+    Represents a specific printing of a card.
 
     Attributes:
-    Core fields
         arena_id: This card's Arena ID, if applicable.
         scryfall_id: Scryfall's unique ID for this card.
         lang: The language code for this print;
-          see https://scryfall.com/docs/api/languages
+            see [here](https://scryfall.com/docs/api/languages)
         mtgo_id: This card's MTGO Catalog ID, if applicable.
         mtgo_foil_id: This card's foil MTGO Catalog ID, if applicable.
         multiverse_ids: This card's multiverse IDs on Gatherer, if any.
         tcgplayer_id: This card's ID on TCGplayer, or `productId` in their
-          system.
+            system.
         tcgplayer_etched_id: This card's ID on TCGplayer, for the etched
-          version if that is a separate product.
+            version if that is a separate product.
         cardmarket_id: This card's ID on Cardmarket, or `idProduct` in their
-          system.
+            system.
         oracle_id: A UUID for this card's oracle identity; shared across prints
-          of the same card but not same-named objects with different gameplay
-          properties.
+            of the same card but not same-named objects with different gameplay
+            properties.
         prints_search_uri: A link to begin paginating through all prints of
-          this card in Scryfall's API.
+            this card in Scryfall's API.
         rulings_uri: A link to rulings for this card in Scryfall's API.
         scryfall_uri: A link to the Scryfall page for this card.
-        uri: A link to this card object in Scryfall's API.
+        uri: A link to this card in Scryfall's API.
 
-    Gameplay fields
-        all_parts: RelatedCard objects for tokens/meld pairs/other associated
-          parts to this card, if applicable.
-        card_faces: All component CardFace objects of this card, for multifaced
-          cards.
+        all_parts: RelatedCards for tokens/meld pairs/other associated
+            parts to this card, if applicable.
+        card_faces: All component CardFaces of this card, for multifaced
+            cards.
         cmc: This card's mana value/converted mana cost.
         color_identity: This card's color identity, for Commander variant
-          deckbuilding.
+            deckbuilding.
         color_indicator: color_indicator: The colors in this card's color
-          indicator, if it has one.
+            indicator, if it has one.
         colors: This card's colors.
         edhrec_rank: This card's rank/popularity on EDHREC, if applicable.
         hand_modifier: This card's Vanguard hand size modifier, if applicable.
         keywords: Keywords and keyword actions this card uses.
         legalities: Formats and the legality status of this card in them.
         life_modifier: This card's Vanguard life modifier value, if applicable.
         loyalty: This card's starting planeswalker loyalty, if applicable.
         mana_cost: Mana cost, as string of mana symbols.
-          (e.g. "{1}{W}{U}{B}{R}{G}")
+            (e.g. "{1}{W}{U}{B}{R}{G}")
         name: This card's name.
         oracle_text: This card's oracle text, if any.
         penny_rank: This card's rank/popularity on Penny Dreadful.
         power: Power of this card, if applicable.
         produced_mana: Which colors of mana this card can produce.
         reserved: Whether this card is on the Reserved List.
         toughness: Toughness of this card, if applicable.
         type_line: This card's type line. (e.g. "Creature — Ooze")
 
-    Print fields
         artist: Artist for this card.
         artist_ids: List of Scryfall IDs for artists of this card.
         attraction_lights: Attraction lights lit on this card, if applicable.
         booster: Whether this card can be opened in booster packs.
         border_color: Border color of this card, from among
-          black, white, borderless, silver, and gold.
+            black, white, borderless, silver, and gold.
         card_back_id: Scryfall UUID of the card back design for this card.
         collector_number: This card's collector number; can contain non-numeric
-          characters.
+            characters.
         content_warning: True if use of this print should be avoided;
-          see https://scryfall.com/blog/regarding-wotc-s-recent-statement-on-depictions-of-racism-220
+            see [here](https://scryfall.com/blog/regarding-wotc-s-recent-statement-on-depictions-of-racism-220)
         digital: True if this card was only released in a video game.
         finishes: Finishes this card is available in, from among foil, nonfoil, and etched.
         flavor_name: Alternate name for this card, such as on Godzilla series.
         flavor_text: Flavor text on this card, if any.
         frame_effects: Special frame effects on this card;
-          see https://scryfall.com/docs/api/frames
+            see [here](https://scryfall.com/docs/api/frames)
         frame: This card's frame layout;
-          see https://scryfall.com/docs/api/frames
+            see [here](https://scryfall.com/docs/api/frames)
         full_art: Whether this print is full-art.
         games: Which games this print is available on, from among
-          paper, mtgo, and arena.
+            paper, mtgo, and arena.
         highres_image: Whether this card has a high-res image available.
         illustration_id: A UUID for the particular artwork on this print,
-          consistent across art reprints.
+            consistent across art reprints.
         image_status: The quality/status of images available for this card.
-          Either missing, placeholder, lowres, or highres_scan.
+            Either missing, placeholder, lowres, or highres_scan.
         image_uris: Links to images of this card in various qualities.
         layout: This card's printed layout;
-          see https://scryfall.com/docs/api/layouts
+            see [here](https://scryfall.com/docs/api/layouts)
         oversized: Whether this card is oversized.
         preview: Information about where, when, and how this print was
-          previewed.
+            previewed.
         prices: Prices for this card on various marketplaces.
         printed_name: Printed name of this card, for localized non-English
-          cards.
+            cards.
         printed_text: Printed text of this card, for localized non-English
-          cards.
+            cards.
         printed_type_line: Printed type line of this card, for localized
-          non-English cards.
+            non-English cards.
         promo: Whether this print is a promo.
         promo_types: Which promo categories this print falls into, if any.
         purchase_uris: Links to purchase this print from marketplaces.
         rarity: The rarity of this print.
         related_uris: Links to this print's listing on other online resources.
         released_at: The date this card was first released.
         reprint: Whether this print is a reprint from an earlier set.
         scryfall_set_uri: Link to the Scryfall set page for the set of this
-          print.
+            print.
         security_stamp: Security stamp on this card, if any.
         set_name: Full name of the set this print belongs to.
         set_search_uri: Link to Scryfall API to start paginating through this
-          print's full set.
+            print's full set.
         set_type: An overall categorization for each set, provided by Scryfall.
-        set_uri: Link to the set object for this print in Scryfall's API.
+        set_uri: Link to the set for this print in Scryfall's API.
         set_code: Set code of the set this print belongs to.
         set_id: UUID of the set this print belongs to.
         story_spotlight: Whether this print is a Story Spotlight.
         textless: Whether this print is textless.
-        variation: Whether this card print is a variation of another card
-          object.
-        variation_of: Which card object this object is a variant of, if any.
+        variation: Whether this card print is a variation of another card.
+        variation_of: Which card this object is a variant of, if any.
         watermark: Watermark printed on this card, if any.
     """
 
     # region Core fields
 
     arena_id: int | None = Field(
         default=None,
         description="This card's Arena ID, if applicable.",
     )
     scryfall_id: str | None = Field(
         default=None,
         description="Scryfall's unique ID for this card.",
-        validation_alias="id",
-        alias_priority=1,
+        validation_alias=AliasChoices("scryfall_id", "scryfallId", "id"),
     )
     lang: Language | None = Field(
         default=None,
-        description="The language code for this print; see https://scryfall.com/docs/api/languages",
+        description="The language code for this print; see [here](https://scryfall.com/docs/api/languages)",
     )
     mtgo_id: int | None = Field(
         default=None,
         description="This card's MTGO Catalog ID, if applicable.",
     )
     mtgo_foil_id: int | None = Field(
         default=None,
@@ -219,28 +214,28 @@
     )
     scryfall_uri: str | None = Field(
         default=None,
         description="A link to the Scryfall page for this card.",
     )
     uri: str | None = Field(
         default=None,
-        description="A link to this card object in Scryfall's API.",
+        description="A link to this card in Scryfall's API.",
     )
 
     # endregion
 
     # region Gameplay fields
 
     all_parts: list[RelatedCardModel] | None = Field(
         default=None,
-        description="RelatedCard objects for tokens/meld pairs/other associated parts to this card, if applicable.",
+        description="RelatedCards for tokens/meld pairs/other associated parts to this card, if applicable.",
     )
     card_faces: list[CardFaceModel] | None = Field(
         default=None,
-        description="All component CardFace objects of this card, for multifaced cards.",
+        description="All component CardFaces of this card, for multifaced cards.",
     )
     cmc: float | None = Field(
         default=None,
         description="This card's mana value/converted mana cost.",
     )
     color_identity: set[Color] | None = Field(
         default=None,
@@ -345,15 +340,15 @@
     )
     collector_number: str | None = Field(
         default=None,
         description="This card's collector number; can contain non-numeric characters.",
     )
     content_warning: bool = Field(
         default=False,
-        description="True if use of this print should be avoided; see https://scryfall.com/blog/regarding-wotc-s-recent-statement-on-depictions-of-racism-220",
+        description="True if use of this print should be avoided; see [here](https://scryfall.com/blog/regarding-wotc-s-recent-statement-on-depictions-of-racism-220)",
     )
     digital: bool | None = Field(
         default=None,
         description="True if this card was only released in a video game.",
     )
     finishes: set[Finish] | None = Field(
         default=None,
@@ -365,19 +360,19 @@
     )
     flavor_text: str | None = Field(
         default=None,
         description="Flavor text on this card, if any.",
     )
     frame_effects: set[FrameEffect] | None = Field(
         default=None,
-        description="Special frame effects on this card; see https://scryfall.com/docs/api/frames",
+        description="Special frame effects on this card; see [here](https://scryfall.com/docs/api/frames)",
     )
     frame: Frame | None = Field(
         default=None,
-        description="This card's frame layout; see https://scryfall.com/docs/api/frames",
+        description="This card's frame layout; see [here](https://scryfall.com/docs/api/frames)",
     )
     full_art: bool | None = Field(
         default=None,
         description="Whether this print is full-art.",
     )
     games: set[Game] | None = Field(
         default=None,
@@ -397,15 +392,15 @@
     )
     image_uris: ImageUrisModel | None = Field(
         default=None,
         description="Links to images of this card in various qualities.",
     )
     layout: Layout | None = Field(
         default=None,
-        description="This card's printed layout; see https://scryfall.com/docs/api/layouts",
+        description="This card's printed layout; see [here](https://scryfall.com/docs/api/layouts)",
     )
     oversized: bool | None = Field(
         default=None,
         description="Whether this card is oversized.",
     )
     preview: PreviewModel | None = Field(
         default=None,
@@ -473,40 +468,40 @@
     )
     set_type: SetType | None = Field(
         default=None,
         description="An overall categorization for each set, provided by Scryfall.",
     )
     set_uri: str | None = Field(
         default=None,
-        description="Link to the set object for this print in Scryfall's API.",
+        description="Link to the set for this print in Scryfall's API.",
     )
     set_code: str | None = Field(
         default=None,
         description="Set code of the set this print belongs to.",
         alias="set",
     )
     set_id: str | None = Field(
         default=None,
-        description="UUID of the set this print belongs to.",
+        description="UUID of the set this print belongs to",
     )
     story_spotlight: bool | None = Field(
         default=None,
-        description="Whether this print is a Story Spotlight.",
+        description="Whether this print is a Story Spotlight",
     )
     textless: bool | None = Field(
         default=None,
         description="Whether this print is textless.",
     )
     variation: bool | None = Field(
         default=None,
-        description="Whether this card print is a variation of another card object.",
+        description="Whether this card print is a variation of another card.",
     )
     variation_of: str | None = Field(
         default=None,
-        description="Which card object this object is a variant of, if any.",
+        description="Which card this object is a variant of, if any.",
     )
     watermark: str | None = Field(
         default=None,
         description="Watermark printed on this card, if any.",
     )
 
     # endregion
@@ -592,15 +587,15 @@
 
 def encode_date(dt: date):
     return dt.strftime(format=DATE_FORMAT)
 
 
 class CardModel(ScoozeDocument, CardModelData):
     """
-    Database representation of a Scooze Card
+    A database representation of a scooze Card.
     """
 
     model_config = ConfigDict(
         json_schema_extra={
             "examples": [
                 {
                     "cmc": 2.0,
```

### Comparing `scooze-1.0.6/src/scooze/models/deck.py` & `scooze-1.0.7/src/scooze/models/deck.py`

 * *Files 13% similar despite different names*

```diff
@@ -20,15 +20,15 @@
         cmdr: The command zone. Typically 1 or 2 cards in Commander formats.
     """
 
     model_config = ScoozeBaseModel.model_config.copy()
     model_config["json_schema_extra"] = {
         "examples": [
             {
-                "archetype": "Scooze Deck Example",
+                "archetype": "scooze Deck Example",
                 "format": "Limited",
                 "main": {
                     "6502bf99532dd43b31e6055a": 4,  # TODO(#6): replace with Python scooze id
                     "6502bf77bffae3b433093dcb": 4,  # TODO(#6): replace with Scavenging Ooze scooze id
                 },
                 "side": {
                     "6502bfe2e0e370d002c87ceb": 1,  # TODO(#6): replace with Keruga scooze id
@@ -107,15 +107,26 @@
             )
         return self
 
     # endregion
 
 
 class DeckModelIn(DeckModel):
+    """
+    A Deck model to be passed to the database.
+    """
+
     pass
 
 
 class DeckModelOut(DeckModel):
+    """
+    A Deck model to be retrieved from the database.
+
+    Attributes:
+        id: A UUID for this deck in the database.
+    """
+
     id: ObjectIdT = Field(
         default=None,
         alias="_id",
     )
```

### Comparing `scooze-1.0.6/src/scooze/models/utils.py` & `scooze-1.0.7/src/scooze/models/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -16,14 +16,17 @@
 
 # region Public Utility Classes
 
 
 class ScoozeDocument(Document):
     """
     A simple base Beanie Document class to support models in scooze.
+
+    Attributes:
+        id: A UUID for this Document in the database.
     """
 
     # Need to explicitly alias here to work around receiving scryfall_id as id when getting data directly from Scryfall
     id: PydanticObjectId | None = Field(
         default=None,
         description="MongoDB _id field",
         alias="_id",
```

### Comparing `scooze-1.0.6/src/scooze/mongo.py` & `scooze-1.0.7/src/scooze/mongo.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 
 class Database:
     """
     A simple database object to house the Motor client.
 
     Attributes:
-        client: An AsyncIOMotorClient for managing Scooze's MongoDB connection.
+        client: An AsyncIOMotorClient for managing scooze's MongoDB connection.
     """
 
     client: AsyncIOMotorClient = None
 
 
 db = Database()
```

### Comparing `scooze-1.0.6/src/scooze/routers/card.py` & `scooze-1.0.7/src/scooze/routers/card.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     tags=["card"],
     responses={404: {"description": "Card Not Found"}},
 )
 
 
 def _validate_card_id(card_id: str) -> PydanticObjectId:
     """
-    Helper to validate incoming strings as Card IDs
+    Helper to validate incoming strings as card IDs
 
     Args:
         card_id: Incoming string to test.
 
     Returns:
         Valid PydanticObjectId.
 
@@ -68,15 +68,16 @@
 
     Raises:
         HTTPException: 400 - Create failed, passes along the error message.
     """
 
     try:
         # NOTE: would like to add the dupe protection back in
-        card = CardModel.model_validate(card_data.model_dump(mode="json", by_alias=True))
+        card = CardModel.model_validate(card_data.model_dump())
+
         return await card.create()
     except Exception as e:
         raise HTTPException(status_code=400, detail=f"Failed to create a new card. Error: {e}")
 
 
 # Read
```

### Comparing `scooze-1.0.6/src/scooze/routers/cards.py` & `scooze-1.0.7/src/scooze/routers/cards.py`

 * *Files identical despite different names*

### Comparing `scooze-1.0.6/src/scooze/routers/deck.py` & `scooze-1.0.7/src/scooze/routers/deck.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,88 +1,114 @@
 import scooze.database.deck as db
 from fastapi import APIRouter
 from fastapi.responses import JSONResponse
-from scooze.models.deck import DeckModelIn
+from scooze.models.deck import DeckModelIn, DeckModelOut
 
 router = APIRouter(
     prefix="/deck",
     tags=["deck"],
     responses={404: {"description": "Deck Not Found"}},
 )
 
 
 @router.get("/", summary="Get a deck at random")
-async def deck_root():
+async def deck_root() -> DeckModelOut:
+    """
+    Get a random deck from the database.
+
+    Returns:
+        A random deck from the database.
+
+    Raises:
+        HTTPException: 404 - No decks found in the database.
+    """
+
     decks = await db.get_decks_random(limit=1)
     if decks is not None:
         deck = decks[0]
         return JSONResponse(deck.model_dump(mode="json"), status_code=200)
 
 
 # Create
 
 
 @router.post("/add", summary="Create a new deck")
-async def add_deck(deck: DeckModelIn):
+async def add_deck(deck: DeckModelIn) -> DeckModelOut:
+    """
+    Add a deck to the database.
+
+    Args:
+        deck: The deck to add.
+
+    Returns:
+        The created deck.
+
+    Raises:
+        HTTPException: 400 - Create failed, passes along the error message.
+    """
+
     new_deck = await db.add_deck(deck=deck)
     if new_deck is not None:
         return JSONResponse(new_deck.model_dump(mode="json"), status_code=200)
     else:
         return JSONResponse({"message": f"Failed to create a new deck."}, status_code=400)
 
 
 # Read
 
 
 @router.get("/id/{deck_id}", summary="Get a deck by ID")
-async def get_deck_by_id(deck_id: str):
+async def get_deck_by_id(deck_id: str) -> DeckModelOut:
     """
     Get the deck with the given scooze ID.
 
-    - **deck_id** - the scooze ID of the deck to get
+    Args:
+        deck_id: the scooze ID of the deck to get
     """
 
     deck = await db.get_deck_by_property(property_name="_id", value=deck_id)
     if deck is not None:
         return JSONResponse(deck.model_dump(mode="json"), status_code=200)
     else:
         return JSONResponse({"message": f"Deck with id {deck_id} not found."}, status_code=404)
 
 
 # Update
 
 
 @router.patch("/update/{deck_id}", summary="Update an existing deck")
-async def update_deck(deck_id: str, deck: DeckModelIn):
+async def update_deck(deck_id: str, deck: DeckModelIn) -> DeckModelOut:
     """
     Update an existing deck with the given scooze ID and payload.
 
     Fields will be updated according to the given payload. If a field is not
     present in the payload, it will not be updated.
 
-    - **deck_id** - the scooze ID of the deck to update
+    Args:
+        deck_id: the scooze ID of the deck to update
     """
 
     updated_deck = await db.update_deck(id=deck_id, deck=deck)
 
     if updated_deck is not None:
         return JSONResponse(updated_deck.model_dump(mode="json"), status_code=200)
     else:
         return JSONResponse({"message": f"Deck with id {deck_id} not found."}, status_code=404)
 
 
 # Delete
 
 
 @router.delete("/delete/{deck_id}", summary="Delete an existing deck")
-async def delete_deck_by_id(deck_id: str):
+async def delete_deck_by_id(deck_id: str) -> DeckModelOut:
     """
     Delete an existing deck with the given scooze ID.
 
-    - **deck_id** - the scooze ID of the deck to delete
+    Args:
+        deck_id: the scooze ID of the deck to delete
     """
 
     deleted_deck = await db.delete_deck(id=deck_id)
 
     if deleted_deck is not None:
         return JSONResponse({"message": f"Deck with id {deck_id} deleted."}, status_code=200)
     else:
```

### Comparing `scooze-1.0.6/src/scooze/routers/decks.py` & `scooze-1.0.7/src/scooze/routers/decks.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,61 +1,76 @@
 from typing import Any
 
 import scooze.database.deck as db
 from fastapi import APIRouter
 from fastapi.responses import JSONResponse
-from scooze.models.deck import DeckModelIn
+from scooze.models.deck import DeckModelIn, DeckModelOut
 
 router = APIRouter(
     prefix="/decks",
     tags=["decks"],
     responses={404: {"description": "Decks Not Found"}},
 )
 
 
 @router.get("/", summary="Get decks at random")
-async def decks_root(limit: int = 3):
+async def decks_root(limit: int = 3) -> DeckModelOut:
     """
     Get random decks up to the given limit.
 
-    - **limit** - the maximum number of decks to get
+    Args:
+        limit: the maximum number of decks to get
     """
 
     decks = await db.get_decks_random(limit=limit)
     if decks is not None:
         return JSONResponse([deck.model_dump(mode="json") for deck in decks], status_code=200)
     else:
         return JSONResponse({"message": "No decks found in the database."}, status_code=404)
 
 
 # Create
 
 
 @router.post("/add", summary="Create new decks")
-async def add_decks(decks: list[DeckModelIn]):
+async def add_decks(decks: list[DeckModelIn]) -> DeckModelOut:
+    """
+    Add decks to the database.
+
+    Args:
+        decks: The decks to add.
+
+    Returns:
+        The scooze IDs of the created decks.
+
+    Raises:
+        HTTPException: 400 - Create failed, passes along the error message.
+    """
+
     inserted_ids = await db.add_decks(decks=decks)
     if inserted_ids is not None:
         return JSONResponse({"message": f"Created {len(inserted_ids)} deck(s)."}, status_code=200)
     else:
         return JSONResponse({"message": "Failed to create any new decks."}, status_code=400)
 
 
 @router.post("/by", summary="Get decks by property")
 async def get_decks_by(
     property_name: str, values: list[Any], paginated: bool = False, page: int = 1, page_size: int = 10
-):
+) -> DeckModelOut:
     """
     Get decks where the given property matches any of the given values.
 
-    - **property_name** - the property to check against
-    - **values** - matching values of the given property
-    - **paginated** - return paginated results if True, return all matches if
-    False
-    - **page** - return matches from the given page
-    - **page_size** - the number of results per page
+    Args:
+        property_name: the property to check against
+        values: matching values of the given property
+        paginated: return paginated results if True, return all matches if
+            False
+        page: return matches from the given page
+        page_size: the number of results per page
     """
 
     decks = await db.get_decks_by_property(
         property_name=property_name, values=values, paginated=paginated, page=page, page_size=page_size
     )
     if decks is not None:
         return JSONResponse([deck.model_dump(mode="json") for deck in decks], status_code=200)
@@ -63,14 +78,18 @@
         return JSONResponse({"message": "Decks not found."}, status_code=404)
 
 
 # Delete
 
 
 @router.delete("/delete/all", summary="Delete all decks")
-async def delete_decks_all():
+async def delete_decks_all() -> DeckModelOut:
+    """
+    Delete all decks.
+    """
+
     deleted_count = await db.delete_decks_all()
 
     if deleted_count is not None:
         return JSONResponse({"message": f"Deleted {deleted_count} deck(s)."}, status_code=200)
     else:
         return JSONResponse({"message": "No decks deleted."}, status_code=404)
```

### Comparing `scooze-1.0.6/src/scooze/utils.py` & `scooze-1.0.7/src/scooze/utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,19 +1,19 @@
-import argparse
 import logging
-import os.path
 import re
 from collections import Counter
 from datetime import date, datetime
-from sys import maxsize, stdout
-from typing import Any, Dict, Hashable, Iterable, Mapping, Self, Type, TypeVar
+from enum import Enum, EnumMeta
+from sys import maxsize
+from typing import Any, Hashable, Iterable, Mapping, Self, Type, TypeVar
 
 from frozendict import frozendict
 from pydantic.alias_generators import to_camel
-from scooze.catalogs import CostSymbol, ExtendedEnum, Format
+from scooze.catalogs import CostSymbol, Format
+from scooze.enum import ExtendedEnum
 
 DEFAULT_BULK_FILE_DIR = "./data/bulk"
 DEFAULT_DECKS_DIR = "./data/decks"
 
 ## Generic Types
 T = TypeVar("T")  # generic type
 V = TypeVar("V")  # generic value type
@@ -29,65 +29,23 @@
 def to_lower_camel(string: str) -> str:
     if len(string.split("_")) == 1:
         return string
 
     return to_camel(string)
 
 
-def get_logger(
-    filename: str,
-    logger_name: str,
-    file_logging_level: int = logging.DEBUG,
-    console_logging_level: int = logging.WARNING,
-    formatter: logging.Formatter = logging.Formatter("%(asctime)s - %(name)s:%(levelname)s - %(message)s"),
-) -> logging.Logger:
+def scooze_logger() -> logging.Logger:
     """
-    Helper function to get a new logger.
+    Helper function to get the scooze logger.
 
-    Args:
-        filename: Filename of the log file.
-        logger_name: The logger's name.
-        file_logging_level: Logging level for the log file.
-        console_logging_level: Logging level for stdout.
-        formatter: The Formatter to be used in messages generated by this
-        logger.
-
-    Returns:
-        A new logger.
+    Use the default logging functionality here without any filters, formatters,
+    or handlers, so users can make informed decisions about their own logging.
     """
 
-    # Create directory if not exists
-    filepath = os.path.join("logs", filename)
-    os.makedirs(os.path.dirname(filepath), exist_ok=True)
-
-    # Handlers
-    fh = logging.FileHandler(filepath, mode="a", encoding="UTF-8", delay=False)
-    fh.setLevel(file_logging_level)
-    ch = logging.StreamHandler(stdout)
-    ch.setLevel(console_logging_level)
-
-    # Formatting
-    fh.setFormatter(formatter)
-    ch.setFormatter(formatter)
-
-    # Create the logger
-    logger = logging.getLogger(logger_name)
-    logger.setLevel(logging.DEBUG)
-    logger.addHandler(fh)
-    logger.addHandler(ch)
-
-    return logger
-
-
-class SmartFormatter(argparse.RawDescriptionHelpFormatter, argparse.HelpFormatter):
-    def _split_lines(self, text, width):
-        if text.startswith("R|"):
-            return text[2:].splitlines()
-        # this is the RawTextHelpFormatter._split_lines
-        return argparse.HelpFormatter._split_lines(self, text, width)
+    return logging.getLogger("scooze")
 
 
 # region Deck Format Helpers
 
 
 def max_relentless_quantity(name: str) -> int:
     """
@@ -425,15 +383,15 @@
 
 class JsonNormalizer:
     """
     A simple class to be used when normalizing non-serializable data from JSON.
     """
 
     @classmethod
-    def to_date(cls, d: date | str | None) -> date:
+    def to_date(cls, d: date | str | None) -> date | None:
         """
         Normalize a date.
 
         Args:
             d: A date to normalize.
 
         Returns:
@@ -442,15 +400,15 @@
 
         if d is None or isinstance(d, date):
             return d
 
         return datetime.strptime(d, DATE_FORMAT).date()
 
     @classmethod
-    def to_enum(cls, e: Type[E], v) -> E | None:
+    def to_enum(cls, e: Type[E], v: Any) -> E | None:
         """
         Normalize an Enum.
 
         Args:
             e: A type of Enum to normalize to.
             v: A value to normalize.
 
@@ -575,15 +533,15 @@
         """
         Generate a diff between two dicts.
 
         Args:
             d1: The first dict.
             d2: The second dict.
             NO_KEY: Default value to use when a key is in one dict, but not the
-              other.
+                other.
 
         Returns:
             A dict with all keys from both dicts. The values are tuple(v, v)
             for the values in each dict.
         """
 
         both = d1.keys() & d2.keys()
@@ -604,15 +562,15 @@
 
 
 # endregion
 
 # region Symbology utils
 
 
-def parse_symbols(cost: str) -> Dict[CostSymbol, int]:
+def parse_symbols(cost: str) -> Counter[CostSymbol]:
     """
     Parse a string containing one or more cost symbols, in standard oracle text form (e.g. "{4}{G}").
 
     Args:
         cost: String representing a mana cost, or rules text that may have one or more symbols.
 
     Returns:
```

