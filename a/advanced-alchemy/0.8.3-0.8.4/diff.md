# Comparing `tmp/advanced_alchemy-0.8.3.tar.gz` & `tmp/advanced_alchemy-0.8.4.tar.gz`

## Comparing `advanced_alchemy-0.8.3.tar` & `advanced_alchemy-0.8.4.tar`

### file list

```diff
@@ -1,181 +1,181 @@
--rw-r--r--   0        0        0     2020 2020-02-02 00:00:00.000000 advanced_alchemy-0.8.3/.pre-commit-config.yaml
--rw-r--r--   0        0        0      622 2020-02-02 00:00:00.000000 advanced_alchemy-0.8.3/.sourcery.yaml
--rw-r--r--   0        0        0      489 2020-02-02 00:00:00.000000 advanced_alchemy-0.8.3/CODEOWNERS
--rw-r--r--   0        0        0     4095 2020-02-02 00:00:00.000000 advanced_alchemy-0.8.3/CONTRIBUTING.rst
--rw-r--r--   0        0        0     6469 2020-02-02 00:00:00.000000 advanced_alchemy-0.8.3/Makefile
--rw-r--r--   0        0        0   350451 2020-02-02 00:00:00.000000 advanced_alchemy-0.8.3/pdm.lock
--rw-r--r--   0        0        0     1135 2020-02-02 00:00:00.000000 advanced_alchemy-0.8.3/sonar-project.properties
--rw-r--r--   0        0        0      489 2020-02-02 00:00:00.000000 advanced_alchemy-0.8.3/.github/CODEOWNERS
--rw-r--r--   0        0        0      572 2020-02-02 00:00:00.000000 advanced_alchemy-0.8.3/.github/workflows/cd.yaml
--rw-r--r--   0        0        0     3388 2020-02-02 00:00:00.000000 advanced_alchemy-0.8.3/.github/workflows/ci.yaml
--rw-r--r--   0        0        0     2342 2020-02-02 00:00:00.000000 advanced_alchemy-0.8.3/.github/workflows/docs-preview.yaml
--rw-r--r--   0        0        0     1022 2020-02-02 00:00:00.000000 advanced_alchemy-0.8.3/.github/workflows/docs.yaml
--rw-r--r--   0        0        0      346 2020-02-02 00:00:00.000000 advanced_alchemy-0.8.3/.github/workflows/pr-title.yaml
--rw-r--r--   0        0        0      697 2020-02-02 00:00:00.000000 advanced_alchemy-0.8.3/.github/workflows/publish.yaml
--rw-r--r--   0        0        0     2520 2020-02-02 00:00:00.000000 advanced_alchemy-0.8.3/.github/workflows/test.yaml
--rw-r--r--   0        0        0     1672 2020-02-02 00:00:00.000000 advanced_alchemy-0.8.3/advanced_alchemy/__init__.py
--rw-r--r--   0        0        0      326 2020-02-02 00:00:00.000000 advanced_alchemy-0.8.3/advanced_alchemy/__metadata__.py
--rw-r--r--   0        0        0      756 2020-02-02 00:00:00.000000 advanced_alchemy-0.8.3/advanced_alchemy/_listeners.py
--rw-r--r--   0        0        0      742 2020-02-02 00:00:00.000000 advanced_alchemy-0.8.3/advanced_alchemy/_serialization.py
--rw-r--r--   0        0        0     7680 2020-02-02 00:00:00.000000 advanced_alchemy-0.8.3/advanced_alchemy/base.py
--rw-r--r--   0        0        0     3985 2020-02-02 00:00:00.000000 advanced_alchemy-0.8.3/advanced_alchemy/exceptions.py
--rw-r--r--   0        0        0     3412 2020-02-02 00:00:00.000000 advanced_alchemy-0.8.3/advanced_alchemy/filters.py
--rw-r--r--   0        0        0     3111 2020-02-02 00:00:00.000000 advanced_alchemy-0.8.3/advanced_alchemy/operations.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 advanced_alchemy-0.8.3/advanced_alchemy/py.typed
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 advanced_alchemy-0.8.3/advanced_alchemy/alembic/__init__.py
--rw-r--r--   0        0        0     8596 2020-02-02 00:00:00.000000 advanced_alchemy-0.8.3/advanced_alchemy/alembic/commands.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 advanced_alchemy-0.8.3/advanced_alchemy/alembic/templates/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 advanced_alchemy-0.8.3/advanced_alchemy/alembic/templates/asyncio/__init__.py
--rw-r--r--   0        0        0     2559 2020-02-02 00:00:00.000000 advanced_alchemy-0.8.3/advanced_alchemy/alembic/templates/asyncio/alembic.ini.mako
--rw-r--r--   0        0        0     4497 2020-02-02 00:00:00.000000 advanced_alchemy-0.8.3/advanced_alchemy/alembic/templates/asyncio/env.py
--rw-r--r--   0        0        0     1815 2020-02-02 00:00:00.000000 advanced_alchemy-0.8.3/advanced_alchemy/alembic/templates/asyncio/script.py.mako
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 advanced_alchemy-0.8.3/advanced_alchemy/alembic/templates/sync/__init__.py
--rw-r--r--   0        0        0     2560 2020-02-02 00:00:00.000000 advanced_alchemy-0.8.3/advanced_alchemy/alembic/templates/sync/alembic.ini.mako
--rw-r--r--   0        0        0     4389 2020-02-02 00:00:00.000000 advanced_alchemy-0.8.3/advanced_alchemy/alembic/templates/sync/env.py
--rw-r--r--   0        0        0     1890 2020-02-02 00:00:00.000000 advanced_alchemy-0.8.3/advanced_alchemy/alembic/templates/sync/script.py.mako
--rw-r--r--   0        0        0      709 2020-02-02 00:00:00.000000 advanced_alchemy-0.8.3/advanced_alchemy/config/__init__.py
--rw-r--r--   0        0        0     2899 2020-02-02 00:00:00.000000 advanced_alchemy-0.8.3/advanced_alchemy/config/asyncio.py
--rw-r--r--   0        0        0    10651 2020-02-02 00:00:00.000000 advanced_alchemy-0.8.3/advanced_alchemy/config/common.py
--rw-r--r--   0        0        0    11108 2020-02-02 00:00:00.000000 advanced_alchemy-0.8.3/advanced_alchemy/config/engine.py
--rw-r--r--   0        0        0     2068 2020-02-02 00:00:00.000000 advanced_alchemy-0.8.3/advanced_alchemy/config/sync.py
--rw-r--r--   0        0        0      604 2020-02-02 00:00:00.000000 advanced_alchemy-0.8.3/advanced_alchemy/config/types.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 advanced_alchemy-0.8.3/advanced_alchemy/extensions/__init__.py
--rw-r--r--   0        0        0     8873 2020-02-02 00:00:00.000000 advanced_alchemy-0.8.3/advanced_alchemy/extensions/sanic.py
--rw-r--r--   0        0        0     6202 2020-02-02 00:00:00.000000 advanced_alchemy-0.8.3/advanced_alchemy/extensions/starlette.py
--rw-r--r--   0        0        0     1474 2020-02-02 00:00:00.000000 advanced_alchemy-0.8.3/advanced_alchemy/extensions/litestar/__init__.py
--rw-r--r--   0        0        0     1911 2020-02-02 00:00:00.000000 advanced_alchemy-0.8.3/advanced_alchemy/extensions/litestar/_utils.py
--rw-r--r--   0        0        0     1356 2020-02-02 00:00:00.000000 advanced_alchemy-0.8.3/advanced_alchemy/extensions/litestar/alembic.py
--rw-r--r--   0        0        0    11152 2020-02-02 00:00:00.000000 advanced_alchemy-0.8.3/advanced_alchemy/extensions/litestar/cli.py
--rw-r--r--   0        0        0    14665 2020-02-02 00:00:00.000000 advanced_alchemy-0.8.3/advanced_alchemy/extensions/litestar/dto.py
--rw-r--r--   0        0        0     1461 2020-02-02 00:00:00.000000 advanced_alchemy-0.8.3/advanced_alchemy/extensions/litestar/plugins/__init__.py
--rw-r--r--   0        0        0      320 2020-02-02 00:00:00.000000 advanced_alchemy-0.8.3/advanced_alchemy/extensions/litestar/plugins/_slots_base.py
--rw-r--r--   0        0        0     1536 2020-02-02 00:00:00.000000 advanced_alchemy-0.8.3/advanced_alchemy/extensions/litestar/plugins/serialization.py
--rw-r--r--   0        0        0      292 2020-02-02 00:00:00.000000 advanced_alchemy-0.8.3/advanced_alchemy/extensions/litestar/plugins/init/__init__.py
--rw-r--r--   0        0        0     3812 2020-02-02 00:00:00.000000 advanced_alchemy-0.8.3/advanced_alchemy/extensions/litestar/plugins/init/plugin.py
--rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 advanced_alchemy-0.8.3/advanced_alchemy/extensions/litestar/plugins/init/config/__init__.py
--rw-r--r--   0        0        0     8169 2020-02-02 00:00:00.000000 advanced_alchemy-0.8.3/advanced_alchemy/extensions/litestar/plugins/init/config/asyncio.py
--rw-r--r--   0        0        0      337 2020-02-02 00:00:00.000000 advanced_alchemy-0.8.3/advanced_alchemy/extensions/litestar/plugins/init/config/common.py
--rw-r--r--   0        0        0     1342 2020-02-02 00:00:00.000000 advanced_alchemy-0.8.3/advanced_alchemy/extensions/litestar/plugins/init/config/engine.py
--rw-r--r--   0        0        0     8159 2020-02-02 00:00:00.000000 advanced_alchemy-0.8.3/advanced_alchemy/extensions/litestar/plugins/init/config/sync.py
--rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 advanced_alchemy-0.8.3/advanced_alchemy/mixins/__init__.py
--rw-r--r--   0        0        0     5661 2020-02-02 00:00:00.000000 advanced_alchemy-0.8.3/advanced_alchemy/mixins/unique.py
--rw-r--r--   0        0        0      433 2020-02-02 00:00:00.000000 advanced_alchemy-0.8.3/advanced_alchemy/repository/__init__.py
--rw-r--r--   0        0        0    63602 2020-02-02 00:00:00.000000 advanced_alchemy-0.8.3/advanced_alchemy/repository/_async.py
--rw-r--r--   0        0        0    63121 2020-02-02 00:00:00.000000 advanced_alchemy-0.8.3/advanced_alchemy/repository/_sync.py
--rw-r--r--   0        0        0     1130 2020-02-02 00:00:00.000000 advanced_alchemy-0.8.3/advanced_alchemy/repository/_util.py
--rw-r--r--   0        0        0      807 2020-02-02 00:00:00.000000 advanced_alchemy-0.8.3/advanced_alchemy/repository/typing.py
--rw-r--r--   0        0        0      175 2020-02-02 00:00:00.000000 advanced_alchemy-0.8.3/advanced_alchemy/repository/memory/__init__.py
--rw-r--r--   0        0        0    18404 2020-02-02 00:00:00.000000 advanced_alchemy-0.8.3/advanced_alchemy/repository/memory/_async.py
--rw-r--r--   0        0        0    18258 2020-02-02 00:00:00.000000 advanced_alchemy-0.8.3/advanced_alchemy/repository/memory/_sync.py
--rw-r--r--   0        0        0    11955 2020-02-02 00:00:00.000000 advanced_alchemy-0.8.3/advanced_alchemy/repository/memory/base.py
--rw-r--r--   0        0        0      360 2020-02-02 00:00:00.000000 advanced_alchemy-0.8.3/advanced_alchemy/service/__init__.py
--rw-r--r--   0        0        0    26861 2020-02-02 00:00:00.000000 advanced_alchemy-0.8.3/advanced_alchemy/service/_async.py
--rw-r--r--   0        0        0    26650 2020-02-02 00:00:00.000000 advanced_alchemy-0.8.3/advanced_alchemy/service/_sync.py
--rw-r--r--   0        0        0      541 2020-02-02 00:00:00.000000 advanced_alchemy-0.8.3/advanced_alchemy/service/typing.py
--rw-r--r--   0        0        0      637 2020-02-02 00:00:00.000000 advanced_alchemy-0.8.3/advanced_alchemy/types/__init__.py
--rw-r--r--   0        0        0     1177 2020-02-02 00:00:00.000000 advanced_alchemy-0.8.3/advanced_alchemy/types/datetime.py
--rw-r--r--   0        0        0     4383 2020-02-02 00:00:00.000000 advanced_alchemy-0.8.3/advanced_alchemy/types/encrypted_string.py
--rw-r--r--   0        0        0     3300 2020-02-02 00:00:00.000000 advanced_alchemy-0.8.3/advanced_alchemy/types/guid.py
--rw-r--r--   0        0        0      236 2020-02-02 00:00:00.000000 advanced_alchemy-0.8.3/advanced_alchemy/types/identity.py
--rw-r--r--   0        0        0     3175 2020-02-02 00:00:00.000000 advanced_alchemy-0.8.3/advanced_alchemy/types/json.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 advanced_alchemy-0.8.3/advanced_alchemy/utils/__init__.py
--rw-r--r--   0        0        0     4788 2020-02-02 00:00:00.000000 advanced_alchemy-0.8.3/advanced_alchemy/utils/dataclass.py
--rw-r--r--   0        0        0     3578 2020-02-02 00:00:00.000000 advanced_alchemy-0.8.3/advanced_alchemy/utils/deprecation.py
--rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 advanced_alchemy-0.8.3/docs/Makefile
--rw-r--r--   0        0        0    61468 2020-02-02 00:00:00.000000 advanced_alchemy-0.8.3/docs/changelog.rst
--rw-r--r--   0        0        0     6457 2020-02-02 00:00:00.000000 advanced_alchemy-0.8.3/docs/conf.py
--rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 advanced_alchemy-0.8.3/docs/contribution-guide.rst
--rw-r--r--   0        0        0     1291 2020-02-02 00:00:00.000000 advanced_alchemy-0.8.3/docs/fix_missing_references.py
--rw-r--r--   0        0        0     1572 2020-02-02 00:00:00.000000 advanced_alchemy-0.8.3/docs/index.rst
--rw-r--r--   0        0        0   296255 2020-02-02 00:00:00.000000 advanced_alchemy-0.8.3/docs/_static/logo.png
--rw-r--r--   0        0        0     1941 2020-02-02 00:00:00.000000 advanced_alchemy-0.8.3/docs/_static/css/custom.css
--rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 advanced_alchemy-0.8.3/docs/reference/base.rst
--rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 advanced_alchemy-0.8.3/docs/reference/exceptions.rst
--rw-r--r--   0        0        0      112 2020-02-02 00:00:00.000000 advanced_alchemy-0.8.3/docs/reference/filters.rst
--rw-r--r--   0        0        0      621 2020-02-02 00:00:00.000000 advanced_alchemy-0.8.3/docs/reference/index.rst
--rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 advanced_alchemy-0.8.3/docs/reference/operations.rst
--rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 advanced_alchemy-0.8.3/docs/reference/repository.rst
--rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 advanced_alchemy-0.8.3/docs/reference/service.rst
--rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 advanced_alchemy-0.8.3/docs/reference/types.rst
--rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 advanced_alchemy-0.8.3/docs/reference/alembic/commands.rst
--rw-r--r--   0        0        0      296 2020-02-02 00:00:00.000000 advanced_alchemy-0.8.3/docs/reference/alembic/index.rst
--rw-r--r--   0        0        0      165 2020-02-02 00:00:00.000000 advanced_alchemy-0.8.3/docs/reference/alembic/templates/asyncio/alembic-ini.rst
--rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 advanced_alchemy-0.8.3/docs/reference/alembic/templates/asyncio/env.rst
--rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 advanced_alchemy-0.8.3/docs/reference/alembic/templates/asyncio/index.rst
--rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 advanced_alchemy-0.8.3/docs/reference/alembic/templates/asyncio/script-py.rst
--rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 advanced_alchemy-0.8.3/docs/reference/alembic/templates/sync/alembic-ini.rst
--rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 advanced_alchemy-0.8.3/docs/reference/alembic/templates/sync/env.rst
--rw-r--r--   0        0        0      274 2020-02-02 00:00:00.000000 advanced_alchemy-0.8.3/docs/reference/alembic/templates/sync/index.rst
--rw-r--r--   0        0        0      157 2020-02-02 00:00:00.000000 advanced_alchemy-0.8.3/docs/reference/alembic/templates/sync/script-py.rst
--rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 advanced_alchemy-0.8.3/docs/reference/config/asyncio.rst
--rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 advanced_alchemy-0.8.3/docs/reference/config/common.rst
--rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 advanced_alchemy-0.8.3/docs/reference/config/engine.rst
--rw-r--r--   0        0        0      279 2020-02-02 00:00:00.000000 advanced_alchemy-0.8.3/docs/reference/config/index.rst
--rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 advanced_alchemy-0.8.3/docs/reference/config/sync.rst
--rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 advanced_alchemy-0.8.3/docs/reference/config/types.rst
--rw-r--r--   0        0        0      285 2020-02-02 00:00:00.000000 advanced_alchemy-0.8.3/docs/reference/extensions/index.rst
--rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 advanced_alchemy-0.8.3/docs/reference/extensions/sanic.rst
--rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 advanced_alchemy-0.8.3/docs/reference/extensions/starlette.rst
--rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 advanced_alchemy-0.8.3/docs/reference/extensions/litestar/alembic.rst
--rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 advanced_alchemy-0.8.3/docs/reference/extensions/litestar/cli.rst
--rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 advanced_alchemy-0.8.3/docs/reference/extensions/litestar/dto.rst
--rw-r--r--   0        0        0      291 2020-02-02 00:00:00.000000 advanced_alchemy-0.8.3/docs/reference/extensions/litestar/index.rst
--rw-r--r--   0        0        0      386 2020-02-02 00:00:00.000000 advanced_alchemy-0.8.3/docs/reference/extensions/litestar/plugins/index.rst
--rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 advanced_alchemy-0.8.3/docs/reference/extensions/litestar/plugins/serialization.rst
--rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 advanced_alchemy-0.8.3/docs/reference/extensions/litestar/plugins/init/plugin.rst
--rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 advanced_alchemy-0.8.3/docs/reference/extensions/litestar/plugins/init/config/asyncio.rst
--rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 advanced_alchemy-0.8.3/docs/reference/extensions/litestar/plugins/init/config/common.rst
--rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 advanced_alchemy-0.8.3/docs/reference/extensions/litestar/plugins/init/config/engine.rst
--rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 advanced_alchemy-0.8.3/docs/reference/extensions/litestar/plugins/init/config/sync.rst
--rw-r--r--   0        0        0      112 2020-02-02 00:00:00.000000 advanced_alchemy-0.8.3/docs/reference/extensions/litestar/plugins/init/config/types.rst
--rw-r--r--   0        0        0      237 2020-02-02 00:00:00.000000 advanced_alchemy-0.8.3/docs/reference/mixins/index.rst
--rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 advanced_alchemy-0.8.3/docs/reference/mixins/unique.rst
--rw-r--r--   0        0        0      214 2020-02-02 00:00:00.000000 advanced_alchemy-0.8.3/docs/usage/index.rst
--rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 advanced_alchemy-0.8.3/docs/usage/placeholder.rst
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 advanced_alchemy-0.8.3/examples/__init__.py
--rw-r--r--   0        0        0     7175 2020-02-02 00:00:00.000000 advanced_alchemy-0.8.3/examples/fastapi.py
--rw-r--r--   0        0        0     1156 2020-02-02 00:00:00.000000 advanced_alchemy-0.8.3/examples/flask.py
--rw-r--r--   0        0        0     7352 2020-02-02 00:00:00.000000 advanced_alchemy-0.8.3/examples/litestar.py
--rw-r--r--   0        0        0     3810 2020-02-02 00:00:00.000000 advanced_alchemy-0.8.3/examples/sanic.py
--rw-r--r--   0        0        0     2860 2020-02-02 00:00:00.000000 advanced_alchemy-0.8.3/examples/standalone.py
--rw-r--r--   0        0        0     3165 2020-02-02 00:00:00.000000 advanced_alchemy-0.8.3/examples/us_state_lookup.json
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 advanced_alchemy-0.8.3/tests/__init__.py
--rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 advanced_alchemy-0.8.3/tests/conftest.py
--rw-r--r--   0        0        0     2455 2020-02-02 00:00:00.000000 advanced_alchemy-0.8.3/tests/docker-compose.yml
--rw-r--r--   0        0        0     9202 2020-02-02 00:00:00.000000 advanced_alchemy-0.8.3/tests/docker_service_fixtures.py
--rw-r--r--   0        0        0     1578 2020-02-02 00:00:00.000000 advanced_alchemy-0.8.3/tests/helpers.py
--rw-r--r--   0        0        0    10992 2020-02-02 00:00:00.000000 advanced_alchemy-0.8.3/tests/models_bigint.py
--rw-r--r--   0        0        0    10742 2020-02-02 00:00:00.000000 advanced_alchemy-0.8.3/tests/models_uuid.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 advanced_alchemy-0.8.3/tests/integration/__init__.py
--rw-r--r--   0        0        0    16714 2020-02-02 00:00:00.000000 advanced_alchemy-0.8.3/tests/integration/conftest.py
--rw-r--r--   0        0        0      889 2020-02-02 00:00:00.000000 advanced_alchemy-0.8.3/tests/integration/helpers.py
--rw-r--r--   0        0        0     7791 2020-02-02 00:00:00.000000 advanced_alchemy-0.8.3/tests/integration/test_alembic_commands.py
--rw-r--r--   0        0        0     3236 2020-02-02 00:00:00.000000 advanced_alchemy-0.8.3/tests/integration/test_lambda_stmt.py
--rw-r--r--   0        0        0     1284 2020-02-02 00:00:00.000000 advanced_alchemy-0.8.3/tests/integration/test_oracledb_json.py
--rw-r--r--   0        0        0    84897 2020-02-02 00:00:00.000000 advanced_alchemy-0.8.3/tests/integration/test_repository.py
--rw-r--r--   0        0        0     4479 2020-02-02 00:00:00.000000 advanced_alchemy-0.8.3/tests/integration/test_unique_mixin.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 advanced_alchemy-0.8.3/tests/unit/__init__.py
--rw-r--r--   0        0        0      275 2020-02-02 00:00:00.000000 advanced_alchemy-0.8.3/tests/unit/test_exceptions.py
--rw-r--r--   0        0        0    32016 2020-02-02 00:00:00.000000 advanced_alchemy-0.8.3/tests/unit/test_repository.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 advanced_alchemy-0.8.3/tests/unit/test_extensions/__init__.py
--rw-r--r--   0        0        0     8694 2020-02-02 00:00:00.000000 advanced_alchemy-0.8.3/tests/unit/test_extensions/test_sanic.py
--rw-r--r--   0        0        0     8968 2020-02-02 00:00:00.000000 advanced_alchemy-0.8.3/tests/unit/test_extensions/test_starlette.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 advanced_alchemy-0.8.3/tests/unit/test_extensions/test_litestar/__init__.py
--rw-r--r--   0        0        0     9763 2020-02-02 00:00:00.000000 advanced_alchemy-0.8.3/tests/unit/test_extensions/test_litestar/conftest.py
--rw-r--r--   0        0        0      918 2020-02-02 00:00:00.000000 advanced_alchemy-0.8.3/tests/unit/test_extensions/test_litestar/test_context.py
--rw-r--r--   0        0        0    21775 2020-02-02 00:00:00.000000 advanced_alchemy-0.8.3/tests/unit/test_extensions/test_litestar/test_dto.py
--rw-r--r--   0        0        0    21538 2020-02-02 00:00:00.000000 advanced_alchemy-0.8.3/tests/unit/test_extensions/test_litestar/test_dto_integration.py
--rw-r--r--   0        0        0      280 2020-02-02 00:00:00.000000 advanced_alchemy-0.8.3/tests/unit/test_extensions/test_litestar/test_litestar_re_exports.py
--rw-r--r--   0        0        0     2518 2020-02-02 00:00:00.000000 advanced_alchemy-0.8.3/tests/unit/test_extensions/test_litestar/test_serialization_plugin.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 advanced_alchemy-0.8.3/tests/unit/test_extensions/test_litestar/test_init_plugin/__init__.py
--rw-r--r--   0        0        0     7215 2020-02-02 00:00:00.000000 advanced_alchemy-0.8.3/tests/unit/test_extensions/test_litestar/test_init_plugin/test_asyncio.py
--rw-r--r--   0        0        0     5604 2020-02-02 00:00:00.000000 advanced_alchemy-0.8.3/tests/unit/test_extensions/test_litestar/test_init_plugin/test_common.py
--rw-r--r--   0        0        0      271 2020-02-02 00:00:00.000000 advanced_alchemy-0.8.3/tests/unit/test_extensions/test_litestar/test_init_plugin/test_engine.py
--rw-r--r--   0        0        0     7005 2020-02-02 00:00:00.000000 advanced_alchemy-0.8.3/tests/unit/test_extensions/test_litestar/test_init_plugin/test_sync.py
--rw-r--r--   0        0        0     1426 2020-02-02 00:00:00.000000 advanced_alchemy-0.8.3/tools/build_docs.py
--rwxr-xr-x   0        0        0      186 2020-02-02 00:00:00.000000 advanced_alchemy-0.8.3/tools/convert_docs.sh
--rw-r--r--   0        0        0     3182 2020-02-02 00:00:00.000000 advanced_alchemy-0.8.3/.gitignore
--rw-r--r--   0        0        0     1061 2020-02-02 00:00:00.000000 advanced_alchemy-0.8.3/LICENSE
--rw-r--r--   0        0        0    17356 2020-02-02 00:00:00.000000 advanced_alchemy-0.8.3/README.md
--rw-r--r--   0        0        0    14428 2020-02-02 00:00:00.000000 advanced_alchemy-0.8.3/pyproject.toml
--rw-r--r--   0        0        0    19259 2020-02-02 00:00:00.000000 advanced_alchemy-0.8.3/PKG-INFO
+-rw-r--r--   0        0        0     2020 2020-02-02 00:00:00.000000 advanced_alchemy-0.8.4/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      622 2020-02-02 00:00:00.000000 advanced_alchemy-0.8.4/.sourcery.yaml
+-rw-r--r--   0        0        0      489 2020-02-02 00:00:00.000000 advanced_alchemy-0.8.4/CODEOWNERS
+-rw-r--r--   0        0        0     4095 2020-02-02 00:00:00.000000 advanced_alchemy-0.8.4/CONTRIBUTING.rst
+-rw-r--r--   0        0        0     6469 2020-02-02 00:00:00.000000 advanced_alchemy-0.8.4/Makefile
+-rw-r--r--   0        0        0   350451 2020-02-02 00:00:00.000000 advanced_alchemy-0.8.4/pdm.lock
+-rw-r--r--   0        0        0     1135 2020-02-02 00:00:00.000000 advanced_alchemy-0.8.4/sonar-project.properties
+-rw-r--r--   0        0        0      489 2020-02-02 00:00:00.000000 advanced_alchemy-0.8.4/.github/CODEOWNERS
+-rw-r--r--   0        0        0      572 2020-02-02 00:00:00.000000 advanced_alchemy-0.8.4/.github/workflows/cd.yaml
+-rw-r--r--   0        0        0     3388 2020-02-02 00:00:00.000000 advanced_alchemy-0.8.4/.github/workflows/ci.yaml
+-rw-r--r--   0        0        0     2342 2020-02-02 00:00:00.000000 advanced_alchemy-0.8.4/.github/workflows/docs-preview.yaml
+-rw-r--r--   0        0        0     1022 2020-02-02 00:00:00.000000 advanced_alchemy-0.8.4/.github/workflows/docs.yaml
+-rw-r--r--   0        0        0      346 2020-02-02 00:00:00.000000 advanced_alchemy-0.8.4/.github/workflows/pr-title.yaml
+-rw-r--r--   0        0        0      697 2020-02-02 00:00:00.000000 advanced_alchemy-0.8.4/.github/workflows/publish.yaml
+-rw-r--r--   0        0        0     2520 2020-02-02 00:00:00.000000 advanced_alchemy-0.8.4/.github/workflows/test.yaml
+-rw-r--r--   0        0        0     1672 2020-02-02 00:00:00.000000 advanced_alchemy-0.8.4/advanced_alchemy/__init__.py
+-rw-r--r--   0        0        0      326 2020-02-02 00:00:00.000000 advanced_alchemy-0.8.4/advanced_alchemy/__metadata__.py
+-rw-r--r--   0        0        0      756 2020-02-02 00:00:00.000000 advanced_alchemy-0.8.4/advanced_alchemy/_listeners.py
+-rw-r--r--   0        0        0      742 2020-02-02 00:00:00.000000 advanced_alchemy-0.8.4/advanced_alchemy/_serialization.py
+-rw-r--r--   0        0        0     7680 2020-02-02 00:00:00.000000 advanced_alchemy-0.8.4/advanced_alchemy/base.py
+-rw-r--r--   0        0        0     3985 2020-02-02 00:00:00.000000 advanced_alchemy-0.8.4/advanced_alchemy/exceptions.py
+-rw-r--r--   0        0        0     3412 2020-02-02 00:00:00.000000 advanced_alchemy-0.8.4/advanced_alchemy/filters.py
+-rw-r--r--   0        0        0     3111 2020-02-02 00:00:00.000000 advanced_alchemy-0.8.4/advanced_alchemy/operations.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 advanced_alchemy-0.8.4/advanced_alchemy/py.typed
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 advanced_alchemy-0.8.4/advanced_alchemy/alembic/__init__.py
+-rw-r--r--   0        0        0     8596 2020-02-02 00:00:00.000000 advanced_alchemy-0.8.4/advanced_alchemy/alembic/commands.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 advanced_alchemy-0.8.4/advanced_alchemy/alembic/templates/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 advanced_alchemy-0.8.4/advanced_alchemy/alembic/templates/asyncio/__init__.py
+-rw-r--r--   0        0        0     2559 2020-02-02 00:00:00.000000 advanced_alchemy-0.8.4/advanced_alchemy/alembic/templates/asyncio/alembic.ini.mako
+-rw-r--r--   0        0        0     4497 2020-02-02 00:00:00.000000 advanced_alchemy-0.8.4/advanced_alchemy/alembic/templates/asyncio/env.py
+-rw-r--r--   0        0        0     1815 2020-02-02 00:00:00.000000 advanced_alchemy-0.8.4/advanced_alchemy/alembic/templates/asyncio/script.py.mako
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 advanced_alchemy-0.8.4/advanced_alchemy/alembic/templates/sync/__init__.py
+-rw-r--r--   0        0        0     2560 2020-02-02 00:00:00.000000 advanced_alchemy-0.8.4/advanced_alchemy/alembic/templates/sync/alembic.ini.mako
+-rw-r--r--   0        0        0     4389 2020-02-02 00:00:00.000000 advanced_alchemy-0.8.4/advanced_alchemy/alembic/templates/sync/env.py
+-rw-r--r--   0        0        0     1890 2020-02-02 00:00:00.000000 advanced_alchemy-0.8.4/advanced_alchemy/alembic/templates/sync/script.py.mako
+-rw-r--r--   0        0        0      709 2020-02-02 00:00:00.000000 advanced_alchemy-0.8.4/advanced_alchemy/config/__init__.py
+-rw-r--r--   0        0        0     2899 2020-02-02 00:00:00.000000 advanced_alchemy-0.8.4/advanced_alchemy/config/asyncio.py
+-rw-r--r--   0        0        0    10651 2020-02-02 00:00:00.000000 advanced_alchemy-0.8.4/advanced_alchemy/config/common.py
+-rw-r--r--   0        0        0    11108 2020-02-02 00:00:00.000000 advanced_alchemy-0.8.4/advanced_alchemy/config/engine.py
+-rw-r--r--   0        0        0     2068 2020-02-02 00:00:00.000000 advanced_alchemy-0.8.4/advanced_alchemy/config/sync.py
+-rw-r--r--   0        0        0      604 2020-02-02 00:00:00.000000 advanced_alchemy-0.8.4/advanced_alchemy/config/types.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 advanced_alchemy-0.8.4/advanced_alchemy/extensions/__init__.py
+-rw-r--r--   0        0        0     8873 2020-02-02 00:00:00.000000 advanced_alchemy-0.8.4/advanced_alchemy/extensions/sanic.py
+-rw-r--r--   0        0        0     6202 2020-02-02 00:00:00.000000 advanced_alchemy-0.8.4/advanced_alchemy/extensions/starlette.py
+-rw-r--r--   0        0        0     1474 2020-02-02 00:00:00.000000 advanced_alchemy-0.8.4/advanced_alchemy/extensions/litestar/__init__.py
+-rw-r--r--   0        0        0     1911 2020-02-02 00:00:00.000000 advanced_alchemy-0.8.4/advanced_alchemy/extensions/litestar/_utils.py
+-rw-r--r--   0        0        0     1356 2020-02-02 00:00:00.000000 advanced_alchemy-0.8.4/advanced_alchemy/extensions/litestar/alembic.py
+-rw-r--r--   0        0        0    11152 2020-02-02 00:00:00.000000 advanced_alchemy-0.8.4/advanced_alchemy/extensions/litestar/cli.py
+-rw-r--r--   0        0        0    14665 2020-02-02 00:00:00.000000 advanced_alchemy-0.8.4/advanced_alchemy/extensions/litestar/dto.py
+-rw-r--r--   0        0        0     1461 2020-02-02 00:00:00.000000 advanced_alchemy-0.8.4/advanced_alchemy/extensions/litestar/plugins/__init__.py
+-rw-r--r--   0        0        0      320 2020-02-02 00:00:00.000000 advanced_alchemy-0.8.4/advanced_alchemy/extensions/litestar/plugins/_slots_base.py
+-rw-r--r--   0        0        0     1536 2020-02-02 00:00:00.000000 advanced_alchemy-0.8.4/advanced_alchemy/extensions/litestar/plugins/serialization.py
+-rw-r--r--   0        0        0      292 2020-02-02 00:00:00.000000 advanced_alchemy-0.8.4/advanced_alchemy/extensions/litestar/plugins/init/__init__.py
+-rw-r--r--   0        0        0     3812 2020-02-02 00:00:00.000000 advanced_alchemy-0.8.4/advanced_alchemy/extensions/litestar/plugins/init/plugin.py
+-rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 advanced_alchemy-0.8.4/advanced_alchemy/extensions/litestar/plugins/init/config/__init__.py
+-rw-r--r--   0        0        0     8169 2020-02-02 00:00:00.000000 advanced_alchemy-0.8.4/advanced_alchemy/extensions/litestar/plugins/init/config/asyncio.py
+-rw-r--r--   0        0        0      337 2020-02-02 00:00:00.000000 advanced_alchemy-0.8.4/advanced_alchemy/extensions/litestar/plugins/init/config/common.py
+-rw-r--r--   0        0        0     1342 2020-02-02 00:00:00.000000 advanced_alchemy-0.8.4/advanced_alchemy/extensions/litestar/plugins/init/config/engine.py
+-rw-r--r--   0        0        0     8159 2020-02-02 00:00:00.000000 advanced_alchemy-0.8.4/advanced_alchemy/extensions/litestar/plugins/init/config/sync.py
+-rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 advanced_alchemy-0.8.4/advanced_alchemy/mixins/__init__.py
+-rw-r--r--   0        0        0     5661 2020-02-02 00:00:00.000000 advanced_alchemy-0.8.4/advanced_alchemy/mixins/unique.py
+-rw-r--r--   0        0        0      433 2020-02-02 00:00:00.000000 advanced_alchemy-0.8.4/advanced_alchemy/repository/__init__.py
+-rw-r--r--   0        0        0    63602 2020-02-02 00:00:00.000000 advanced_alchemy-0.8.4/advanced_alchemy/repository/_async.py
+-rw-r--r--   0        0        0    63121 2020-02-02 00:00:00.000000 advanced_alchemy-0.8.4/advanced_alchemy/repository/_sync.py
+-rw-r--r--   0        0        0     1083 2020-02-02 00:00:00.000000 advanced_alchemy-0.8.4/advanced_alchemy/repository/_util.py
+-rw-r--r--   0        0        0      807 2020-02-02 00:00:00.000000 advanced_alchemy-0.8.4/advanced_alchemy/repository/typing.py
+-rw-r--r--   0        0        0      175 2020-02-02 00:00:00.000000 advanced_alchemy-0.8.4/advanced_alchemy/repository/memory/__init__.py
+-rw-r--r--   0        0        0    18350 2020-02-02 00:00:00.000000 advanced_alchemy-0.8.4/advanced_alchemy/repository/memory/_async.py
+-rw-r--r--   0        0        0    18204 2020-02-02 00:00:00.000000 advanced_alchemy-0.8.4/advanced_alchemy/repository/memory/_sync.py
+-rw-r--r--   0        0        0    11955 2020-02-02 00:00:00.000000 advanced_alchemy-0.8.4/advanced_alchemy/repository/memory/base.py
+-rw-r--r--   0        0        0      360 2020-02-02 00:00:00.000000 advanced_alchemy-0.8.4/advanced_alchemy/service/__init__.py
+-rw-r--r--   0        0        0    26861 2020-02-02 00:00:00.000000 advanced_alchemy-0.8.4/advanced_alchemy/service/_async.py
+-rw-r--r--   0        0        0    26650 2020-02-02 00:00:00.000000 advanced_alchemy-0.8.4/advanced_alchemy/service/_sync.py
+-rw-r--r--   0        0        0      541 2020-02-02 00:00:00.000000 advanced_alchemy-0.8.4/advanced_alchemy/service/typing.py
+-rw-r--r--   0        0        0      637 2020-02-02 00:00:00.000000 advanced_alchemy-0.8.4/advanced_alchemy/types/__init__.py
+-rw-r--r--   0        0        0     1177 2020-02-02 00:00:00.000000 advanced_alchemy-0.8.4/advanced_alchemy/types/datetime.py
+-rw-r--r--   0        0        0     4383 2020-02-02 00:00:00.000000 advanced_alchemy-0.8.4/advanced_alchemy/types/encrypted_string.py
+-rw-r--r--   0        0        0     3300 2020-02-02 00:00:00.000000 advanced_alchemy-0.8.4/advanced_alchemy/types/guid.py
+-rw-r--r--   0        0        0      236 2020-02-02 00:00:00.000000 advanced_alchemy-0.8.4/advanced_alchemy/types/identity.py
+-rw-r--r--   0        0        0     3175 2020-02-02 00:00:00.000000 advanced_alchemy-0.8.4/advanced_alchemy/types/json.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 advanced_alchemy-0.8.4/advanced_alchemy/utils/__init__.py
+-rw-r--r--   0        0        0     4788 2020-02-02 00:00:00.000000 advanced_alchemy-0.8.4/advanced_alchemy/utils/dataclass.py
+-rw-r--r--   0        0        0     3578 2020-02-02 00:00:00.000000 advanced_alchemy-0.8.4/advanced_alchemy/utils/deprecation.py
+-rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 advanced_alchemy-0.8.4/docs/Makefile
+-rw-r--r--   0        0        0    61468 2020-02-02 00:00:00.000000 advanced_alchemy-0.8.4/docs/changelog.rst
+-rw-r--r--   0        0        0     6457 2020-02-02 00:00:00.000000 advanced_alchemy-0.8.4/docs/conf.py
+-rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 advanced_alchemy-0.8.4/docs/contribution-guide.rst
+-rw-r--r--   0        0        0     1291 2020-02-02 00:00:00.000000 advanced_alchemy-0.8.4/docs/fix_missing_references.py
+-rw-r--r--   0        0        0     1572 2020-02-02 00:00:00.000000 advanced_alchemy-0.8.4/docs/index.rst
+-rw-r--r--   0        0        0   296255 2020-02-02 00:00:00.000000 advanced_alchemy-0.8.4/docs/_static/logo.png
+-rw-r--r--   0        0        0     1941 2020-02-02 00:00:00.000000 advanced_alchemy-0.8.4/docs/_static/css/custom.css
+-rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 advanced_alchemy-0.8.4/docs/reference/base.rst
+-rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 advanced_alchemy-0.8.4/docs/reference/exceptions.rst
+-rw-r--r--   0        0        0      112 2020-02-02 00:00:00.000000 advanced_alchemy-0.8.4/docs/reference/filters.rst
+-rw-r--r--   0        0        0      621 2020-02-02 00:00:00.000000 advanced_alchemy-0.8.4/docs/reference/index.rst
+-rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 advanced_alchemy-0.8.4/docs/reference/operations.rst
+-rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 advanced_alchemy-0.8.4/docs/reference/repository.rst
+-rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 advanced_alchemy-0.8.4/docs/reference/service.rst
+-rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 advanced_alchemy-0.8.4/docs/reference/types.rst
+-rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 advanced_alchemy-0.8.4/docs/reference/alembic/commands.rst
+-rw-r--r--   0        0        0      296 2020-02-02 00:00:00.000000 advanced_alchemy-0.8.4/docs/reference/alembic/index.rst
+-rw-r--r--   0        0        0      165 2020-02-02 00:00:00.000000 advanced_alchemy-0.8.4/docs/reference/alembic/templates/asyncio/alembic-ini.rst
+-rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 advanced_alchemy-0.8.4/docs/reference/alembic/templates/asyncio/env.rst
+-rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 advanced_alchemy-0.8.4/docs/reference/alembic/templates/asyncio/index.rst
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 advanced_alchemy-0.8.4/docs/reference/alembic/templates/asyncio/script-py.rst
+-rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 advanced_alchemy-0.8.4/docs/reference/alembic/templates/sync/alembic-ini.rst
+-rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 advanced_alchemy-0.8.4/docs/reference/alembic/templates/sync/env.rst
+-rw-r--r--   0        0        0      274 2020-02-02 00:00:00.000000 advanced_alchemy-0.8.4/docs/reference/alembic/templates/sync/index.rst
+-rw-r--r--   0        0        0      157 2020-02-02 00:00:00.000000 advanced_alchemy-0.8.4/docs/reference/alembic/templates/sync/script-py.rst
+-rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 advanced_alchemy-0.8.4/docs/reference/config/asyncio.rst
+-rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 advanced_alchemy-0.8.4/docs/reference/config/common.rst
+-rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 advanced_alchemy-0.8.4/docs/reference/config/engine.rst
+-rw-r--r--   0        0        0      279 2020-02-02 00:00:00.000000 advanced_alchemy-0.8.4/docs/reference/config/index.rst
+-rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 advanced_alchemy-0.8.4/docs/reference/config/sync.rst
+-rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 advanced_alchemy-0.8.4/docs/reference/config/types.rst
+-rw-r--r--   0        0        0      285 2020-02-02 00:00:00.000000 advanced_alchemy-0.8.4/docs/reference/extensions/index.rst
+-rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 advanced_alchemy-0.8.4/docs/reference/extensions/sanic.rst
+-rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 advanced_alchemy-0.8.4/docs/reference/extensions/starlette.rst
+-rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 advanced_alchemy-0.8.4/docs/reference/extensions/litestar/alembic.rst
+-rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 advanced_alchemy-0.8.4/docs/reference/extensions/litestar/cli.rst
+-rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 advanced_alchemy-0.8.4/docs/reference/extensions/litestar/dto.rst
+-rw-r--r--   0        0        0      291 2020-02-02 00:00:00.000000 advanced_alchemy-0.8.4/docs/reference/extensions/litestar/index.rst
+-rw-r--r--   0        0        0      386 2020-02-02 00:00:00.000000 advanced_alchemy-0.8.4/docs/reference/extensions/litestar/plugins/index.rst
+-rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 advanced_alchemy-0.8.4/docs/reference/extensions/litestar/plugins/serialization.rst
+-rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 advanced_alchemy-0.8.4/docs/reference/extensions/litestar/plugins/init/plugin.rst
+-rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 advanced_alchemy-0.8.4/docs/reference/extensions/litestar/plugins/init/config/asyncio.rst
+-rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 advanced_alchemy-0.8.4/docs/reference/extensions/litestar/plugins/init/config/common.rst
+-rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 advanced_alchemy-0.8.4/docs/reference/extensions/litestar/plugins/init/config/engine.rst
+-rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 advanced_alchemy-0.8.4/docs/reference/extensions/litestar/plugins/init/config/sync.rst
+-rw-r--r--   0        0        0      112 2020-02-02 00:00:00.000000 advanced_alchemy-0.8.4/docs/reference/extensions/litestar/plugins/init/config/types.rst
+-rw-r--r--   0        0        0      237 2020-02-02 00:00:00.000000 advanced_alchemy-0.8.4/docs/reference/mixins/index.rst
+-rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 advanced_alchemy-0.8.4/docs/reference/mixins/unique.rst
+-rw-r--r--   0        0        0      214 2020-02-02 00:00:00.000000 advanced_alchemy-0.8.4/docs/usage/index.rst
+-rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 advanced_alchemy-0.8.4/docs/usage/placeholder.rst
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 advanced_alchemy-0.8.4/examples/__init__.py
+-rw-r--r--   0        0        0     7175 2020-02-02 00:00:00.000000 advanced_alchemy-0.8.4/examples/fastapi.py
+-rw-r--r--   0        0        0     1156 2020-02-02 00:00:00.000000 advanced_alchemy-0.8.4/examples/flask.py
+-rw-r--r--   0        0        0     7352 2020-02-02 00:00:00.000000 advanced_alchemy-0.8.4/examples/litestar.py
+-rw-r--r--   0        0        0     3810 2020-02-02 00:00:00.000000 advanced_alchemy-0.8.4/examples/sanic.py
+-rw-r--r--   0        0        0     2860 2020-02-02 00:00:00.000000 advanced_alchemy-0.8.4/examples/standalone.py
+-rw-r--r--   0        0        0     3165 2020-02-02 00:00:00.000000 advanced_alchemy-0.8.4/examples/us_state_lookup.json
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 advanced_alchemy-0.8.4/tests/__init__.py
+-rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 advanced_alchemy-0.8.4/tests/conftest.py
+-rw-r--r--   0        0        0     2455 2020-02-02 00:00:00.000000 advanced_alchemy-0.8.4/tests/docker-compose.yml
+-rw-r--r--   0        0        0     9202 2020-02-02 00:00:00.000000 advanced_alchemy-0.8.4/tests/docker_service_fixtures.py
+-rw-r--r--   0        0        0     1578 2020-02-02 00:00:00.000000 advanced_alchemy-0.8.4/tests/helpers.py
+-rw-r--r--   0        0        0    10992 2020-02-02 00:00:00.000000 advanced_alchemy-0.8.4/tests/models_bigint.py
+-rw-r--r--   0        0        0    10742 2020-02-02 00:00:00.000000 advanced_alchemy-0.8.4/tests/models_uuid.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 advanced_alchemy-0.8.4/tests/integration/__init__.py
+-rw-r--r--   0        0        0    16714 2020-02-02 00:00:00.000000 advanced_alchemy-0.8.4/tests/integration/conftest.py
+-rw-r--r--   0        0        0      889 2020-02-02 00:00:00.000000 advanced_alchemy-0.8.4/tests/integration/helpers.py
+-rw-r--r--   0        0        0     7791 2020-02-02 00:00:00.000000 advanced_alchemy-0.8.4/tests/integration/test_alembic_commands.py
+-rw-r--r--   0        0        0     3236 2020-02-02 00:00:00.000000 advanced_alchemy-0.8.4/tests/integration/test_lambda_stmt.py
+-rw-r--r--   0        0        0     1284 2020-02-02 00:00:00.000000 advanced_alchemy-0.8.4/tests/integration/test_oracledb_json.py
+-rw-r--r--   0        0        0    85855 2020-02-02 00:00:00.000000 advanced_alchemy-0.8.4/tests/integration/test_repository.py
+-rw-r--r--   0        0        0     4479 2020-02-02 00:00:00.000000 advanced_alchemy-0.8.4/tests/integration/test_unique_mixin.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 advanced_alchemy-0.8.4/tests/unit/__init__.py
+-rw-r--r--   0        0        0      275 2020-02-02 00:00:00.000000 advanced_alchemy-0.8.4/tests/unit/test_exceptions.py
+-rw-r--r--   0        0        0    32016 2020-02-02 00:00:00.000000 advanced_alchemy-0.8.4/tests/unit/test_repository.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 advanced_alchemy-0.8.4/tests/unit/test_extensions/__init__.py
+-rw-r--r--   0        0        0     8694 2020-02-02 00:00:00.000000 advanced_alchemy-0.8.4/tests/unit/test_extensions/test_sanic.py
+-rw-r--r--   0        0        0     8968 2020-02-02 00:00:00.000000 advanced_alchemy-0.8.4/tests/unit/test_extensions/test_starlette.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 advanced_alchemy-0.8.4/tests/unit/test_extensions/test_litestar/__init__.py
+-rw-r--r--   0        0        0     9763 2020-02-02 00:00:00.000000 advanced_alchemy-0.8.4/tests/unit/test_extensions/test_litestar/conftest.py
+-rw-r--r--   0        0        0      918 2020-02-02 00:00:00.000000 advanced_alchemy-0.8.4/tests/unit/test_extensions/test_litestar/test_context.py
+-rw-r--r--   0        0        0    21775 2020-02-02 00:00:00.000000 advanced_alchemy-0.8.4/tests/unit/test_extensions/test_litestar/test_dto.py
+-rw-r--r--   0        0        0    21538 2020-02-02 00:00:00.000000 advanced_alchemy-0.8.4/tests/unit/test_extensions/test_litestar/test_dto_integration.py
+-rw-r--r--   0        0        0      280 2020-02-02 00:00:00.000000 advanced_alchemy-0.8.4/tests/unit/test_extensions/test_litestar/test_litestar_re_exports.py
+-rw-r--r--   0        0        0     2518 2020-02-02 00:00:00.000000 advanced_alchemy-0.8.4/tests/unit/test_extensions/test_litestar/test_serialization_plugin.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 advanced_alchemy-0.8.4/tests/unit/test_extensions/test_litestar/test_init_plugin/__init__.py
+-rw-r--r--   0        0        0     7215 2020-02-02 00:00:00.000000 advanced_alchemy-0.8.4/tests/unit/test_extensions/test_litestar/test_init_plugin/test_asyncio.py
+-rw-r--r--   0        0        0     5604 2020-02-02 00:00:00.000000 advanced_alchemy-0.8.4/tests/unit/test_extensions/test_litestar/test_init_plugin/test_common.py
+-rw-r--r--   0        0        0      271 2020-02-02 00:00:00.000000 advanced_alchemy-0.8.4/tests/unit/test_extensions/test_litestar/test_init_plugin/test_engine.py
+-rw-r--r--   0        0        0     7005 2020-02-02 00:00:00.000000 advanced_alchemy-0.8.4/tests/unit/test_extensions/test_litestar/test_init_plugin/test_sync.py
+-rw-r--r--   0        0        0     1426 2020-02-02 00:00:00.000000 advanced_alchemy-0.8.4/tools/build_docs.py
+-rwxr-xr-x   0        0        0      186 2020-02-02 00:00:00.000000 advanced_alchemy-0.8.4/tools/convert_docs.sh
+-rw-r--r--   0        0        0     3182 2020-02-02 00:00:00.000000 advanced_alchemy-0.8.4/.gitignore
+-rw-r--r--   0        0        0     1061 2020-02-02 00:00:00.000000 advanced_alchemy-0.8.4/LICENSE
+-rw-r--r--   0        0        0    17356 2020-02-02 00:00:00.000000 advanced_alchemy-0.8.4/README.md
+-rw-r--r--   0        0        0    14481 2020-02-02 00:00:00.000000 advanced_alchemy-0.8.4/pyproject.toml
+-rw-r--r--   0        0        0    19259 2020-02-02 00:00:00.000000 advanced_alchemy-0.8.4/PKG-INFO
```

### Comparing `advanced_alchemy-0.8.3/.pre-commit-config.yaml` & `advanced_alchemy-0.8.4/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `advanced_alchemy-0.8.3/.sourcery.yaml` & `advanced_alchemy-0.8.4/.sourcery.yaml`

 * *Files identical despite different names*

### Comparing `advanced_alchemy-0.8.3/CONTRIBUTING.rst` & `advanced_alchemy-0.8.4/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `advanced_alchemy-0.8.3/Makefile` & `advanced_alchemy-0.8.4/Makefile`

 * *Files identical despite different names*

### Comparing `advanced_alchemy-0.8.3/pdm.lock` & `advanced_alchemy-0.8.4/pdm.lock`

 * *Files identical despite different names*

### Comparing `advanced_alchemy-0.8.3/sonar-project.properties` & `advanced_alchemy-0.8.4/sonar-project.properties`

 * *Files identical despite different names*

### Comparing `advanced_alchemy-0.8.3/.github/workflows/cd.yaml` & `advanced_alchemy-0.8.4/.github/workflows/cd.yaml`

 * *Files identical despite different names*

### Comparing `advanced_alchemy-0.8.3/.github/workflows/ci.yaml` & `advanced_alchemy-0.8.4/.github/workflows/ci.yaml`

 * *Files identical despite different names*

### Comparing `advanced_alchemy-0.8.3/.github/workflows/docs-preview.yaml` & `advanced_alchemy-0.8.4/.github/workflows/docs-preview.yaml`

 * *Files identical despite different names*

### Comparing `advanced_alchemy-0.8.3/.github/workflows/docs.yaml` & `advanced_alchemy-0.8.4/.github/workflows/docs.yaml`

 * *Files identical despite different names*

### Comparing `advanced_alchemy-0.8.3/.github/workflows/publish.yaml` & `advanced_alchemy-0.8.4/.github/workflows/publish.yaml`

 * *Files identical despite different names*

### Comparing `advanced_alchemy-0.8.3/.github/workflows/test.yaml` & `advanced_alchemy-0.8.4/.github/workflows/test.yaml`

 * *Files identical despite different names*

### Comparing `advanced_alchemy-0.8.3/advanced_alchemy/__init__.py` & `advanced_alchemy-0.8.4/advanced_alchemy/__init__.py`

 * *Files identical despite different names*

### Comparing `advanced_alchemy-0.8.3/advanced_alchemy/_listeners.py` & `advanced_alchemy-0.8.4/advanced_alchemy/_listeners.py`

 * *Files identical despite different names*

### Comparing `advanced_alchemy-0.8.3/advanced_alchemy/_serialization.py` & `advanced_alchemy-0.8.4/advanced_alchemy/_serialization.py`

 * *Files identical despite different names*

### Comparing `advanced_alchemy-0.8.3/advanced_alchemy/base.py` & `advanced_alchemy-0.8.4/advanced_alchemy/base.py`

 * *Files identical despite different names*

### Comparing `advanced_alchemy-0.8.3/advanced_alchemy/exceptions.py` & `advanced_alchemy-0.8.4/advanced_alchemy/exceptions.py`

 * *Files identical despite different names*

### Comparing `advanced_alchemy-0.8.3/advanced_alchemy/filters.py` & `advanced_alchemy-0.8.4/advanced_alchemy/filters.py`

 * *Files identical despite different names*

### Comparing `advanced_alchemy-0.8.3/advanced_alchemy/operations.py` & `advanced_alchemy-0.8.4/advanced_alchemy/operations.py`

 * *Files identical despite different names*

### Comparing `advanced_alchemy-0.8.3/advanced_alchemy/alembic/commands.py` & `advanced_alchemy-0.8.4/advanced_alchemy/alembic/commands.py`

 * *Files identical despite different names*

### Comparing `advanced_alchemy-0.8.3/advanced_alchemy/alembic/templates/asyncio/alembic.ini.mako` & `advanced_alchemy-0.8.4/advanced_alchemy/alembic/templates/asyncio/alembic.ini.mako`

 * *Files identical despite different names*

### Comparing `advanced_alchemy-0.8.3/advanced_alchemy/alembic/templates/asyncio/env.py` & `advanced_alchemy-0.8.4/advanced_alchemy/alembic/templates/asyncio/env.py`

 * *Files identical despite different names*

### Comparing `advanced_alchemy-0.8.3/advanced_alchemy/alembic/templates/asyncio/script.py.mako` & `advanced_alchemy-0.8.4/advanced_alchemy/alembic/templates/asyncio/script.py.mako`

 * *Files identical despite different names*

### Comparing `advanced_alchemy-0.8.3/advanced_alchemy/alembic/templates/sync/alembic.ini.mako` & `advanced_alchemy-0.8.4/advanced_alchemy/alembic/templates/sync/alembic.ini.mako`

 * *Files identical despite different names*

### Comparing `advanced_alchemy-0.8.3/advanced_alchemy/alembic/templates/sync/env.py` & `advanced_alchemy-0.8.4/advanced_alchemy/alembic/templates/sync/env.py`

 * *Files identical despite different names*

### Comparing `advanced_alchemy-0.8.3/advanced_alchemy/alembic/templates/sync/script.py.mako` & `advanced_alchemy-0.8.4/advanced_alchemy/alembic/templates/sync/script.py.mako`

 * *Files identical despite different names*

### Comparing `advanced_alchemy-0.8.3/advanced_alchemy/config/__init__.py` & `advanced_alchemy-0.8.4/advanced_alchemy/config/__init__.py`

 * *Files identical despite different names*

### Comparing `advanced_alchemy-0.8.3/advanced_alchemy/config/asyncio.py` & `advanced_alchemy-0.8.4/advanced_alchemy/config/asyncio.py`

 * *Files identical despite different names*

### Comparing `advanced_alchemy-0.8.3/advanced_alchemy/config/common.py` & `advanced_alchemy-0.8.4/advanced_alchemy/config/common.py`

 * *Files identical despite different names*

### Comparing `advanced_alchemy-0.8.3/advanced_alchemy/config/engine.py` & `advanced_alchemy-0.8.4/advanced_alchemy/config/engine.py`

 * *Files identical despite different names*

### Comparing `advanced_alchemy-0.8.3/advanced_alchemy/config/sync.py` & `advanced_alchemy-0.8.4/advanced_alchemy/config/sync.py`

 * *Files identical despite different names*

### Comparing `advanced_alchemy-0.8.3/advanced_alchemy/config/types.py` & `advanced_alchemy-0.8.4/advanced_alchemy/config/types.py`

 * *Files identical despite different names*

### Comparing `advanced_alchemy-0.8.3/advanced_alchemy/extensions/sanic.py` & `advanced_alchemy-0.8.4/advanced_alchemy/extensions/sanic.py`

 * *Files identical despite different names*

### Comparing `advanced_alchemy-0.8.3/advanced_alchemy/extensions/starlette.py` & `advanced_alchemy-0.8.4/advanced_alchemy/extensions/starlette.py`

 * *Files identical despite different names*

### Comparing `advanced_alchemy-0.8.3/advanced_alchemy/extensions/litestar/__init__.py` & `advanced_alchemy-0.8.4/advanced_alchemy/extensions/litestar/__init__.py`

 * *Files identical despite different names*

### Comparing `advanced_alchemy-0.8.3/advanced_alchemy/extensions/litestar/_utils.py` & `advanced_alchemy-0.8.4/advanced_alchemy/extensions/litestar/_utils.py`

 * *Files identical despite different names*

### Comparing `advanced_alchemy-0.8.3/advanced_alchemy/extensions/litestar/alembic.py` & `advanced_alchemy-0.8.4/advanced_alchemy/extensions/litestar/alembic.py`

 * *Files identical despite different names*

### Comparing `advanced_alchemy-0.8.3/advanced_alchemy/extensions/litestar/cli.py` & `advanced_alchemy-0.8.4/advanced_alchemy/extensions/litestar/cli.py`

 * *Files identical despite different names*

### Comparing `advanced_alchemy-0.8.3/advanced_alchemy/extensions/litestar/dto.py` & `advanced_alchemy-0.8.4/advanced_alchemy/extensions/litestar/dto.py`

 * *Files identical despite different names*

### Comparing `advanced_alchemy-0.8.3/advanced_alchemy/extensions/litestar/plugins/__init__.py` & `advanced_alchemy-0.8.4/advanced_alchemy/extensions/litestar/plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `advanced_alchemy-0.8.3/advanced_alchemy/extensions/litestar/plugins/serialization.py` & `advanced_alchemy-0.8.4/advanced_alchemy/extensions/litestar/plugins/serialization.py`

 * *Files identical despite different names*

### Comparing `advanced_alchemy-0.8.3/advanced_alchemy/extensions/litestar/plugins/init/plugin.py` & `advanced_alchemy-0.8.4/advanced_alchemy/extensions/litestar/plugins/init/plugin.py`

 * *Files identical despite different names*

### Comparing `advanced_alchemy-0.8.3/advanced_alchemy/extensions/litestar/plugins/init/config/asyncio.py` & `advanced_alchemy-0.8.4/advanced_alchemy/extensions/litestar/plugins/init/config/asyncio.py`

 * *Files identical despite different names*

### Comparing `advanced_alchemy-0.8.3/advanced_alchemy/extensions/litestar/plugins/init/config/engine.py` & `advanced_alchemy-0.8.4/advanced_alchemy/extensions/litestar/plugins/init/config/engine.py`

 * *Files identical despite different names*

### Comparing `advanced_alchemy-0.8.3/advanced_alchemy/extensions/litestar/plugins/init/config/sync.py` & `advanced_alchemy-0.8.4/advanced_alchemy/extensions/litestar/plugins/init/config/sync.py`

 * *Files identical despite different names*

### Comparing `advanced_alchemy-0.8.3/advanced_alchemy/mixins/unique.py` & `advanced_alchemy-0.8.4/advanced_alchemy/mixins/unique.py`

 * *Files identical despite different names*

### Comparing `advanced_alchemy-0.8.3/advanced_alchemy/repository/_async.py` & `advanced_alchemy-0.8.4/advanced_alchemy/repository/_async.py`

 * *Files identical despite different names*

### Comparing `advanced_alchemy-0.8.3/advanced_alchemy/repository/_sync.py` & `advanced_alchemy-0.8.4/advanced_alchemy/repository/_sync.py`

 * *Files identical despite different names*

### Comparing `advanced_alchemy-0.8.3/advanced_alchemy/repository/_util.py` & `advanced_alchemy-0.8.4/advanced_alchemy/repository/_util.py`

 * *Files 9% similar despite different names*

```diff
@@ -18,13 +18,13 @@
     if isinstance(key, str):
         return cast("InstrumentedAttribute", getattr(model, key))
     return key
 
 
 def model_from_dict(model: ModelT, **kwargs: Any) -> ModelT:
     """Return ORM Object from Dictionary."""
-    data = {}
-    for column_name in model.__mapper__.columns.keys():  # noqa: SIM118
-        column_val = kwargs.get(column_name, None)
-        if column_val is not None:
-            data[column_name] = column_val
+    data = {
+        column_name: kwargs[column_name]
+        for column_name in model.__mapper__.columns.keys()  # noqa: SIM118
+        if column_name in kwargs
+    }
     return model(**data)  # type: ignore  # noqa: PGH003
```

### Comparing `advanced_alchemy-0.8.3/advanced_alchemy/repository/typing.py` & `advanced_alchemy-0.8.4/advanced_alchemy/repository/typing.py`

 * *Files identical despite different names*

### Comparing `advanced_alchemy-0.8.3/advanced_alchemy/repository/memory/_async.py` & `advanced_alchemy-0.8.4/advanced_alchemy/repository/memory/_async.py`

 * *Files 0% similar despite different names*

```diff
@@ -396,22 +396,18 @@
     async def add_many(self, data: list[ModelT], **_: Any) -> list[ModelT]:
         for obj in data:
             await self.add(obj)
         return data
 
     async def update(self, data: ModelT, **_: Any) -> ModelT:
         self._find_or_raise_not_found(self.__collection__().key(data))
-        self.__collection__().update(data)
-        return data
+        return self.__collection__().update(data)
 
     async def update_many(self, data: list[ModelT], **_: Any) -> list[ModelT]:
-        for obj in data:
-            if obj in self.__collection__():
-                self.__collection__().update(obj)
-        return data
+        return [self.__collection__().update(obj) for obj in data if obj in self.__collection__()]
 
     async def delete(self, item_id: Any, **_: Any) -> ModelT:
         try:
             return self._find_or_raise_not_found(item_id)
         finally:
             self.__collection__().remove(item_id)
```

### Comparing `advanced_alchemy-0.8.3/advanced_alchemy/repository/memory/_sync.py` & `advanced_alchemy-0.8.4/advanced_alchemy/repository/memory/_sync.py`

 * *Files 1% similar despite different names*

```diff
@@ -398,22 +398,18 @@
     def add_many(self, data: list[ModelT], **_: Any) -> list[ModelT]:
         for obj in data:
             self.add(obj)
         return data
 
     def update(self, data: ModelT, **_: Any) -> ModelT:
         self._find_or_raise_not_found(self.__collection__().key(data))
-        self.__collection__().update(data)
-        return data
+        return self.__collection__().update(data)
 
     def update_many(self, data: list[ModelT], **_: Any) -> list[ModelT]:
-        for obj in data:
-            if obj in self.__collection__():
-                self.__collection__().update(obj)
-        return data
+        return [self.__collection__().update(obj) for obj in data if obj in self.__collection__()]
 
     def delete(self, item_id: Any, **_: Any) -> ModelT:
         try:
             return self._find_or_raise_not_found(item_id)
         finally:
             self.__collection__().remove(item_id)
```

### Comparing `advanced_alchemy-0.8.3/advanced_alchemy/repository/memory/base.py` & `advanced_alchemy-0.8.4/advanced_alchemy/repository/memory/base.py`

 * *Files identical despite different names*

### Comparing `advanced_alchemy-0.8.3/advanced_alchemy/service/_async.py` & `advanced_alchemy-0.8.4/advanced_alchemy/service/_async.py`

 * *Files identical despite different names*

### Comparing `advanced_alchemy-0.8.3/advanced_alchemy/service/_sync.py` & `advanced_alchemy-0.8.4/advanced_alchemy/service/_sync.py`

 * *Files identical despite different names*

### Comparing `advanced_alchemy-0.8.3/advanced_alchemy/service/typing.py` & `advanced_alchemy-0.8.4/advanced_alchemy/service/typing.py`

 * *Files identical despite different names*

### Comparing `advanced_alchemy-0.8.3/advanced_alchemy/types/__init__.py` & `advanced_alchemy-0.8.4/advanced_alchemy/types/__init__.py`

 * *Files identical despite different names*

### Comparing `advanced_alchemy-0.8.3/advanced_alchemy/types/datetime.py` & `advanced_alchemy-0.8.4/advanced_alchemy/types/datetime.py`

 * *Files identical despite different names*

### Comparing `advanced_alchemy-0.8.3/advanced_alchemy/types/encrypted_string.py` & `advanced_alchemy-0.8.4/advanced_alchemy/types/encrypted_string.py`

 * *Files identical despite different names*

### Comparing `advanced_alchemy-0.8.3/advanced_alchemy/types/guid.py` & `advanced_alchemy-0.8.4/advanced_alchemy/types/guid.py`

 * *Files identical despite different names*

### Comparing `advanced_alchemy-0.8.3/advanced_alchemy/types/json.py` & `advanced_alchemy-0.8.4/advanced_alchemy/types/json.py`

 * *Files identical despite different names*

### Comparing `advanced_alchemy-0.8.3/advanced_alchemy/utils/dataclass.py` & `advanced_alchemy-0.8.4/advanced_alchemy/utils/dataclass.py`

 * *Files identical despite different names*

### Comparing `advanced_alchemy-0.8.3/advanced_alchemy/utils/deprecation.py` & `advanced_alchemy-0.8.4/advanced_alchemy/utils/deprecation.py`

 * *Files identical despite different names*

### Comparing `advanced_alchemy-0.8.3/docs/Makefile` & `advanced_alchemy-0.8.4/docs/Makefile`

 * *Files identical despite different names*

### Comparing `advanced_alchemy-0.8.3/docs/changelog.rst` & `advanced_alchemy-0.8.4/docs/changelog.rst`

 * *Files identical despite different names*

### Comparing `advanced_alchemy-0.8.3/docs/conf.py` & `advanced_alchemy-0.8.4/docs/conf.py`

 * *Files identical despite different names*

### Comparing `advanced_alchemy-0.8.3/docs/fix_missing_references.py` & `advanced_alchemy-0.8.4/docs/fix_missing_references.py`

 * *Files identical despite different names*

### Comparing `advanced_alchemy-0.8.3/docs/index.rst` & `advanced_alchemy-0.8.4/docs/index.rst`

 * *Files identical despite different names*

### Comparing `advanced_alchemy-0.8.3/docs/_static/logo.png` & `advanced_alchemy-0.8.4/docs/_static/logo.png`

 * *Files identical despite different names*

### Comparing `advanced_alchemy-0.8.3/docs/_static/css/custom.css` & `advanced_alchemy-0.8.4/docs/_static/css/custom.css`

 * *Files identical despite different names*

### Comparing `advanced_alchemy-0.8.3/docs/reference/index.rst` & `advanced_alchemy-0.8.4/docs/reference/index.rst`

 * *Files identical despite different names*

### Comparing `advanced_alchemy-0.8.3/examples/fastapi.py` & `advanced_alchemy-0.8.4/examples/fastapi.py`

 * *Files identical despite different names*

### Comparing `advanced_alchemy-0.8.3/examples/flask.py` & `advanced_alchemy-0.8.4/examples/flask.py`

 * *Files identical despite different names*

### Comparing `advanced_alchemy-0.8.3/examples/litestar.py` & `advanced_alchemy-0.8.4/examples/litestar.py`

 * *Files identical despite different names*

### Comparing `advanced_alchemy-0.8.3/examples/sanic.py` & `advanced_alchemy-0.8.4/examples/sanic.py`

 * *Files identical despite different names*

### Comparing `advanced_alchemy-0.8.3/examples/standalone.py` & `advanced_alchemy-0.8.4/examples/standalone.py`

 * *Files identical despite different names*

### Comparing `advanced_alchemy-0.8.3/examples/us_state_lookup.json` & `advanced_alchemy-0.8.4/examples/us_state_lookup.json`

 * *Files identical despite different names*

### Comparing `advanced_alchemy-0.8.3/tests/docker-compose.yml` & `advanced_alchemy-0.8.4/tests/docker-compose.yml`

 * *Files identical despite different names*

### Comparing `advanced_alchemy-0.8.3/tests/docker_service_fixtures.py` & `advanced_alchemy-0.8.4/tests/docker_service_fixtures.py`

 * *Files identical despite different names*

### Comparing `advanced_alchemy-0.8.3/tests/helpers.py` & `advanced_alchemy-0.8.4/tests/helpers.py`

 * *Files identical despite different names*

### Comparing `advanced_alchemy-0.8.3/tests/models_bigint.py` & `advanced_alchemy-0.8.4/tests/models_bigint.py`

 * *Files identical despite different names*

### Comparing `advanced_alchemy-0.8.3/tests/models_uuid.py` & `advanced_alchemy-0.8.4/tests/models_uuid.py`

 * *Files identical despite different names*

### Comparing `advanced_alchemy-0.8.3/tests/integration/conftest.py` & `advanced_alchemy-0.8.4/tests/integration/conftest.py`

 * *Files identical despite different names*

### Comparing `advanced_alchemy-0.8.3/tests/integration/helpers.py` & `advanced_alchemy-0.8.4/tests/integration/helpers.py`

 * *Files identical despite different names*

### Comparing `advanced_alchemy-0.8.3/tests/integration/test_alembic_commands.py` & `advanced_alchemy-0.8.4/tests/integration/test_alembic_commands.py`

 * *Files identical despite different names*

### Comparing `advanced_alchemy-0.8.3/tests/integration/test_lambda_stmt.py` & `advanced_alchemy-0.8.4/tests/integration/test_lambda_stmt.py`

 * *Files identical despite different names*

### Comparing `advanced_alchemy-0.8.3/tests/integration/test_oracledb_json.py` & `advanced_alchemy-0.8.4/tests/integration/test_oracledb_json.py`

 * *Files identical despite different names*

### Comparing `advanced_alchemy-0.8.3/tests/integration/test_repository.py` & `advanced_alchemy-0.8.4/tests/integration/test_repository.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """Unit tests for the SQLAlchemy Repository implementation."""
 
 from __future__ import annotations
 
 import asyncio
 import contextlib
 import os
-from datetime import datetime, timedelta, timezone
+from datetime import date, datetime, timedelta, timezone
 from typing import TYPE_CHECKING, Any, Dict, Generator, Iterator, List, Literal, Type, Union, cast
 from unittest.mock import NonCallableMagicMock, create_autospec
 from uuid import UUID
 
 import pytest
 from pytest_lazyfixture import lazy_fixture
 from sqlalchemy import Engine, Table, and_, insert, select
@@ -1662,14 +1662,16 @@
 
 async def test_lazy_load(
     item_repo: ItemRepository,
     tag_repo: TagRepository,
     item_model: ItemModel,
     tag_model: TagModel,
 ) -> None:
+    if getattr(tag_repo, "__collection__", None) is not None:
+        pytest.skip("Skipping lazy load testing on Mock repositories.")
     tag_obj = await maybe_async(tag_repo.add(tag_model(name="A new tag")))
     assert tag_obj
     new_items = await maybe_async(
         item_repo.add_many([item_model(name="The first item"), item_model(name="The second item")]),
     )
     await maybe_async(item_repo.session.commit())
     await maybe_async(tag_repo.session.commit())
@@ -1917,14 +1919,34 @@
     obj = await maybe_async(author_service.get(first_author_id))
     obj.name = "Updated Name2"
     updated_obj = await maybe_async(author_service.update(data=obj))
     assert str(updated_obj.id) == str(first_author_id)
     assert updated_obj.name == obj.name
 
 
+async def test_service_update_method_data_is_dict(author_service: AuthorService, first_author_id: Any) -> None:
+    new_date = datetime.date(datetime.now())
+    updated_obj = await maybe_async(
+        author_service.update(item_id=first_author_id, data={"dob": new_date}),
+    )
+    assert updated_obj.dob == new_date
+    # ensure the other fields are not affected
+    assert updated_obj.name == "Agatha Christie"
+
+
+async def test_service_update_method_data_is_dict_with_none_value(
+    author_service: AuthorService,
+    first_author_id: Any,
+) -> None:
+    updated_obj = await maybe_async(author_service.update(item_id=first_author_id, data={"dob": None}))
+    assert cast(Union[date, None], updated_obj.dob) is None
+    # ensure the other fields are not affected
+    assert updated_obj.name == "Agatha Christie"
+
+
 async def test_service_update_method_instrumented_attribute(
     author_service: AuthorService,
     first_author_id: Any,
 ) -> None:
     obj = await maybe_async(author_service.get(first_author_id))
     id_attribute = get_instrumented_attr(author_service.repository.model_type, "id")
     obj.name = "Updated Name2"
```

### Comparing `advanced_alchemy-0.8.3/tests/integration/test_unique_mixin.py` & `advanced_alchemy-0.8.4/tests/integration/test_unique_mixin.py`

 * *Files identical despite different names*

### Comparing `advanced_alchemy-0.8.3/tests/unit/test_repository.py` & `advanced_alchemy-0.8.4/tests/unit/test_repository.py`

 * *Files identical despite different names*

### Comparing `advanced_alchemy-0.8.3/tests/unit/test_extensions/test_sanic.py` & `advanced_alchemy-0.8.4/tests/unit/test_extensions/test_sanic.py`

 * *Files identical despite different names*

### Comparing `advanced_alchemy-0.8.3/tests/unit/test_extensions/test_starlette.py` & `advanced_alchemy-0.8.4/tests/unit/test_extensions/test_starlette.py`

 * *Files identical despite different names*

### Comparing `advanced_alchemy-0.8.3/tests/unit/test_extensions/test_litestar/conftest.py` & `advanced_alchemy-0.8.4/tests/unit/test_extensions/test_litestar/conftest.py`

 * *Files identical despite different names*

### Comparing `advanced_alchemy-0.8.3/tests/unit/test_extensions/test_litestar/test_context.py` & `advanced_alchemy-0.8.4/tests/unit/test_extensions/test_litestar/test_context.py`

 * *Files identical despite different names*

### Comparing `advanced_alchemy-0.8.3/tests/unit/test_extensions/test_litestar/test_dto.py` & `advanced_alchemy-0.8.4/tests/unit/test_extensions/test_litestar/test_dto.py`

 * *Files identical despite different names*

### Comparing `advanced_alchemy-0.8.3/tests/unit/test_extensions/test_litestar/test_dto_integration.py` & `advanced_alchemy-0.8.4/tests/unit/test_extensions/test_litestar/test_dto_integration.py`

 * *Files identical despite different names*

### Comparing `advanced_alchemy-0.8.3/tests/unit/test_extensions/test_litestar/test_serialization_plugin.py` & `advanced_alchemy-0.8.4/tests/unit/test_extensions/test_litestar/test_serialization_plugin.py`

 * *Files identical despite different names*

### Comparing `advanced_alchemy-0.8.3/tests/unit/test_extensions/test_litestar/test_init_plugin/test_asyncio.py` & `advanced_alchemy-0.8.4/tests/unit/test_extensions/test_litestar/test_init_plugin/test_asyncio.py`

 * *Files identical despite different names*

### Comparing `advanced_alchemy-0.8.3/tests/unit/test_extensions/test_litestar/test_init_plugin/test_common.py` & `advanced_alchemy-0.8.4/tests/unit/test_extensions/test_litestar/test_init_plugin/test_common.py`

 * *Files identical despite different names*

### Comparing `advanced_alchemy-0.8.3/tests/unit/test_extensions/test_litestar/test_init_plugin/test_sync.py` & `advanced_alchemy-0.8.4/tests/unit/test_extensions/test_litestar/test_init_plugin/test_sync.py`

 * *Files identical despite different names*

### Comparing `advanced_alchemy-0.8.3/tools/build_docs.py` & `advanced_alchemy-0.8.4/tools/build_docs.py`

 * *Files identical despite different names*

### Comparing `advanced_alchemy-0.8.3/.gitignore` & `advanced_alchemy-0.8.4/.gitignore`

 * *Files identical despite different names*

### Comparing `advanced_alchemy-0.8.3/LICENSE` & `advanced_alchemy-0.8.4/LICENSE`

 * *Files identical despite different names*

### Comparing `advanced_alchemy-0.8.3/README.md` & `advanced_alchemy-0.8.4/README.md`

 * *Files identical despite different names*

### Comparing `advanced_alchemy-0.8.3/pyproject.toml` & `advanced_alchemy-0.8.4/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [project]
 authors = [
-  {name = "Cody Fincher", email = "cody.fincher@gmail.com"},
-  {name = "Peter Schutt", email = "peter.github@proton.me"},
-  {name = "Janek Nouvertné", email = "j.a.nouvertne@posteo.de"},
-  {name = "Jacob Coffee", email = "jacob@z7x.org"},
+  { name = "Cody Fincher", email = "cody.fincher@gmail.com" },
+  { name = "Peter Schutt", email = "peter.github@proton.me" },
+  { name = "Janek Nouvertné", email = "j.a.nouvertne@posteo.de" },
+  { name = "Jacob Coffee", email = "jacob@z7x.org" },
 ]
 classifiers = [
   "Development Status :: 3 - Alpha",
   "Environment :: Web Environment",
   "License :: OSI Approved :: MIT License",
   "Natural Language :: English",
   "Operating System :: OS Independent",
@@ -28,33 +28,31 @@
   "sqlalchemy>=2.0.20",
   "alembic>=1.12.0",
   "typing-extensions>=4.0.0",
   "greenlet; sys_platform == \"darwin\"",
 ]
 description = "Ready-to-go SQLAlchemy concoctions."
 keywords = ["sqlalchemy", "alembic", "litestar", "sanic", "fastapi", "flask"]
-license = {text = "MIT"}
+license = { text = "MIT" }
 name = "advanced_alchemy"
 readme = "README.md"
 requires-python = ">=3.8"
-version = "0.8.3"
+version = "0.8.4"
 
 [project.urls]
 Changelog = "https://docs.advanced-alchemy.jolt.rs/latest/changelog"
 Discord = "https://discord.gg/XpFNTjjtTK"
 Documentation = "https://docs.advanced-alchemy.jolt.rs/latest/"
 Funding = "https://github.com/sponsors/jolt-org"
 Homepage = "https://docs.advanced-alchemy.jolt.rs/latest/"
 Issue = "https://github.com/jolt-org/advanced-alchemy/issues/"
 Source = "https://github.com/jolt-org/advanced-alchemy"
 
 [project.optional-dependencies]
-uuid = [
-  "uuid-utils>=0.6.1",
-]
+uuid = ["uuid-utils>=0.6.1"]
 [build-system]
 build-backend = "hatchling.build"
 requires = ["hatchling"]
 
 [tool.pdm.dev-dependencies]
 dev = [
   "asyncmy>=0.2.8",
@@ -93,23 +91,23 @@
   "sanic[ext]>=23.6.0",
   "sanic-testing>=23.6.0",
   "msgspec>=0.18.2",
   "flask>=3.0.0",
   "flask-sqlalchemy>=3.1.1",
 ]
 linting = [
-    "pre-commit>=3.4.0",
-    "black>=23.7.0",
-    "mypy>=1.5.1",
-    "ruff>=0.0.287",
-    "asyncpg-stubs",
-    "types-pytest-lazy-fixture",
-    "types-click",
-    "types-pyyaml",
-    "pyright>=1.1.350",
+  "pre-commit>=3.4.0",
+  "black>=23.7.0",
+  "mypy>=1.5.1",
+  "ruff>=0.0.287",
+  "asyncpg-stubs",
+  "types-pytest-lazy-fixture",
+  "types-click",
+  "types-pyyaml",
+  "pyright>=1.1.350",
 ]
 test = [
   "pytest>=7.4.1,<8.0.0",
   "pytest-xdist>=3.3.1",
   "pytest-lazy-fixture>=0.6.3",
   "pytest-asyncio>=0.21.1",
   "pytest-mock>=3.11.1",
@@ -187,40 +185,40 @@
 src = ["advanced_alchemy", "tests"]
 target-version = "py38"
 
 [tool.ruff.lint]
 dummy-variable-rgx = "^(_+|(_+[a-zA-Z0-9_]*[a-zA-Z0-9]+?))$"
 fixable = ["ALL"]
 ignore = [
-  "A003", # flake8-builtins - class attribute {name} is shadowing a python builtin
-  "B010", # flake8-bugbear - do not call setattr with a constant attribute value
-  "D100", # pydocstyle - missing docstring in public module
-  "D101", # pydocstyle - missing docstring in public class
-  "D102", # pydocstyle - missing docstring in public method
-  "D103", # pydocstyle - missing docstring in public function
-  "D104", # pydocstyle - missing docstring in public package
-  "D105", # pydocstyle - missing docstring in magic method
-  "D106", # pydocstyle - missing docstring in public nested class
-  "D107", # pydocstyle - missing docstring in __init__
-  "D202", # pydocstyle - no blank lines allowed after function docstring
-  "D205", # pydocstyle - 1 blank line required between summary line and description
-  "D415", # pydocstyle - first line should end with a period, question mark, or exclamation point
-  "E501", # pycodestyle line too long, handled by black
+  "A003",    # flake8-builtins - class attribute {name} is shadowing a python builtin
+  "B010",    # flake8-bugbear - do not call setattr with a constant attribute value
+  "D100",    # pydocstyle - missing docstring in public module
+  "D101",    # pydocstyle - missing docstring in public class
+  "D102",    # pydocstyle - missing docstring in public method
+  "D103",    # pydocstyle - missing docstring in public function
+  "D104",    # pydocstyle - missing docstring in public package
+  "D105",    # pydocstyle - missing docstring in magic method
+  "D106",    # pydocstyle - missing docstring in public nested class
+  "D107",    # pydocstyle - missing docstring in __init__
+  "D202",    # pydocstyle - no blank lines allowed after function docstring
+  "D205",    # pydocstyle - 1 blank line required between summary line and description
+  "D415",    # pydocstyle - first line should end with a period, question mark, or exclamation point
+  "E501",    # pycodestyle line too long, handled by black
   "PLW2901", # pylint - for loop variable overwritten by assignment target
-  "RUF012", # Ruff-specific rule - annotated with classvar
+  "RUF012",  # Ruff-specific rule - annotated with classvar
   "ANN401",
   "ANN102",
   "ANN101",
   "FBT",
   "PLR0913", # too many arguments
   "PT",
   "TD",
-  "ARG002", # ignore for now; investigate
+  "ARG002",  # ignore for now; investigate
   "PERF203", # ignore for now; investigate
-  "PD011", # pandas
+  "PD011",   # pandas
 ]
 select = ["ALL"]
 
 [tool.ruff.lint.pydocstyle]
 convention = "google"
 
 [tool.ruff.lint.mccabe]
@@ -411,24 +409,24 @@
 =========\n
 All commits to this project will be documented in this file.\n
 """
 trim = true
 
 [tool.git-cliff.git]
 commit_parsers = [
-  {message = "^feat", group = "Features"},
-  {message = "^fix", group = "Bug Fixes"},
-  {message = "^doc", group = "Documentation"},
-  {message = "^perf", group = "Performance"},
-  {message = "^refactor", group = "Refactor"},
-  {message = "^style", group = "Styling"},
-  {message = "^test", group = "Testing"},
-  {message = "^chore\\(release\\): prepare for", skip = true},
-  {message = "^chore", group = "Miscellaneous Tasks"},
-  {body = ".*security", group = "Security"},
+  { message = "^feat", group = "Features" },
+  { message = "^fix", group = "Bug Fixes" },
+  { message = "^doc", group = "Documentation" },
+  { message = "^perf", group = "Performance" },
+  { message = "^refactor", group = "Refactor" },
+  { message = "^style", group = "Styling" },
+  { message = "^test", group = "Testing" },
+  { message = "^chore\\(release\\): prepare for", skip = true },
+  { message = "^chore", group = "Miscellaneous Tasks" },
+  { body = ".*security", group = "Security" },
 ]
 conventional_commits = true
 filter_commits = false
 filter_unconventional = true
 ignore_tags = ""
 protect_breaking_commits = false
 skip_tags = "v0.1.0-beta.1"
```

### Comparing `advanced_alchemy-0.8.3/PKG-INFO` & `advanced_alchemy-0.8.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: advanced_alchemy
-Version: 0.8.3
+Version: 0.8.4
 Summary: Ready-to-go SQLAlchemy concoctions.
 Project-URL: Changelog, https://docs.advanced-alchemy.jolt.rs/latest/changelog
 Project-URL: Discord, https://discord.gg/XpFNTjjtTK
 Project-URL: Documentation, https://docs.advanced-alchemy.jolt.rs/latest/
 Project-URL: Funding, https://github.com/sponsors/jolt-org
 Project-URL: Homepage, https://docs.advanced-alchemy.jolt.rs/latest/
 Project-URL: Issue, https://github.com/jolt-org/advanced-alchemy/issues/
```

