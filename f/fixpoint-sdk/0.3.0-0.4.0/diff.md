# Comparing `tmp/fixpoint_sdk-0.3.0.tar.gz` & `tmp/fixpoint_sdk-0.4.0.tar.gz`

## Comparing `fixpoint_sdk-0.3.0.tar` & `fixpoint_sdk-0.4.0.tar`

### file list

```diff
@@ -1,39 +1,176 @@
--rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 fixpoint_sdk-0.3.0/.editorconfig
--rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 fixpoint_sdk-0.3.0/.lintstagedrc.json
--rw-r--r--   0        0        0    21667 2020-02-02 00:00:00.000000 fixpoint_sdk-0.3.0/.pylintrc
--rw-r--r--   0        0        0      982 2020-02-02 00:00:00.000000 fixpoint_sdk-0.3.0/mypy.ini
--rw-r--r--   0        0        0      186 2020-02-02 00:00:00.000000 fixpoint_sdk-0.3.0/pytest.ini
--rw-r--r--   0        0        0     1356 2020-02-02 00:00:00.000000 fixpoint_sdk-0.3.0/requirements.txt
--rw-r--r--   0        0        0     1427 2020-02-02 00:00:00.000000 fixpoint_sdk-0.3.0/.github/workflows/ci.yml
--rw-r--r--   0        0        0      872 2020-02-02 00:00:00.000000 fixpoint_sdk-0.3.0/.github/workflows/pypi-release-prod.yml
--rw-r--r--   0        0        0      876 2020-02-02 00:00:00.000000 fixpoint_sdk-0.3.0/.github/workflows/pypi-release-test.yml
--rwxr-xr-x   0        0        0      646 2020-02-02 00:00:00.000000 fixpoint_sdk-0.3.0/bin/pip-freeze
--rwxr-xr-x   0        0        0      359 2020-02-02 00:00:00.000000 fixpoint_sdk-0.3.0/bin/pip-install
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fixpoint_sdk-0.3.0/examples/__init__.py
--rw-r--r--   0        0        0     3390 2020-02-02 00:00:00.000000 fixpoint_sdk-0.3.0/examples/main.py
--rw-r--r--   0        0        0     1772 2020-02-02 00:00:00.000000 fixpoint_sdk-0.3.0/examples/streaming.py
--rwxr-xr-x   0        0        0       78 2020-02-02 00:00:00.000000 fixpoint_sdk-0.3.0/githooks/pre-commit
--rw-r--r--   0        0        0      515 2020-02-02 00:00:00.000000 fixpoint_sdk-0.3.0/src/fixpoint_sdk/__init__.py
--rw-r--r--   0        0        0     2065 2020-02-02 00:00:00.000000 fixpoint_sdk-0.3.0/src/fixpoint_sdk/client.py
--rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 fixpoint_sdk-0.3.0/src/fixpoint_sdk/compat.py
--rw-r--r--   0        0        0     9226 2020-02-02 00:00:00.000000 fixpoint_sdk-0.3.0/src/fixpoint_sdk/completions.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fixpoint_sdk-0.3.0/src/fixpoint_sdk/py.typed
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fixpoint_sdk-0.3.0/src/fixpoint_sdk/lib/__init__.py
--rw-r--r--   0        0        0     2298 2020-02-02 00:00:00.000000 fixpoint_sdk-0.3.0/src/fixpoint_sdk/lib/debugging.py
--rw-r--r--   0        0        0     1620 2020-02-02 00:00:00.000000 fixpoint_sdk-0.3.0/src/fixpoint_sdk/lib/env.py
--rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 fixpoint_sdk-0.3.0/src/fixpoint_sdk/lib/exc.py
--rw-r--r--   0        0        0     1037 2020-02-02 00:00:00.000000 fixpoint_sdk-0.3.0/src/fixpoint_sdk/lib/iterwrapper.py
--rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 fixpoint_sdk-0.3.0/src/fixpoint_sdk/lib/logging.py
--rw-r--r--   0        0        0     6441 2020-02-02 00:00:00.000000 fixpoint_sdk-0.3.0/src/fixpoint_sdk/lib/requests.py
--rw-r--r--   0        0        0     4401 2020-02-02 00:00:00.000000 fixpoint_sdk-0.3.0/src/fixpoint_sdk/types/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fixpoint_sdk-0.3.0/tests/__init__.py
--rw-r--r--   0        0        0    15061 2020-02-02 00:00:00.000000 fixpoint_sdk-0.3.0/tests/mock_completions.py
--rw-r--r--   0        0        0     2978 2020-02-02 00:00:00.000000 fixpoint_sdk-0.3.0/tests/test_completions.py
--rw-r--r--   0        0        0      961 2020-02-02 00:00:00.000000 fixpoint_sdk-0.3.0/tests/test_types.py
--rw-r--r--   0        0        0     1977 2020-02-02 00:00:00.000000 fixpoint_sdk-0.3.0/tests/lib/test_iterwrapper.py
--rw-r--r--   0        0        0    10018 2020-02-02 00:00:00.000000 fixpoint_sdk-0.3.0/tests/lib/test_requests.py
--rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 fixpoint_sdk-0.3.0/.gitignore
--rw-r--r--   0        0        0    11338 2020-02-02 00:00:00.000000 fixpoint_sdk-0.3.0/LICENSE
--rw-r--r--   0        0        0     1601 2020-02-02 00:00:00.000000 fixpoint_sdk-0.3.0/README.md
--rw-r--r--   0        0        0      900 2020-02-02 00:00:00.000000 fixpoint_sdk-0.3.0/pyproject.toml
--rw-r--r--   0        0        0     2638 2020-02-02 00:00:00.000000 fixpoint_sdk-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 fixpoint_sdk-0.4.0/.editorconfig
+-rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 fixpoint_sdk-0.4.0/.lintstagedrc.json
+-rw-r--r--   0        0        0    21691 2020-02-02 00:00:00.000000 fixpoint_sdk-0.4.0/.pylintrc
+-rw-r--r--   0        0        0     1007 2020-02-02 00:00:00.000000 fixpoint_sdk-0.4.0/mypy.ini
+-rw-r--r--   0        0        0      186 2020-02-02 00:00:00.000000 fixpoint_sdk-0.4.0/pytest.ini
+-rw-r--r--   0        0        0     1356 2020-02-02 00:00:00.000000 fixpoint_sdk-0.4.0/requirements.txt
+-rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 fixpoint_sdk-0.4.0/test-requirements.txt
+-rw-r--r--   0        0        0     1469 2020-02-02 00:00:00.000000 fixpoint_sdk-0.4.0/.github/workflows/ci.yml
+-rw-r--r--   0        0        0      872 2020-02-02 00:00:00.000000 fixpoint_sdk-0.4.0/.github/workflows/pypi-release-prod.yml
+-rw-r--r--   0        0        0      876 2020-02-02 00:00:00.000000 fixpoint_sdk-0.4.0/.github/workflows/pypi-release-test.yml
+-rwxr-xr-x   0        0        0      646 2020-02-02 00:00:00.000000 fixpoint_sdk-0.4.0/bin/pip-freeze
+-rwxr-xr-x   0        0        0      359 2020-02-02 00:00:00.000000 fixpoint_sdk-0.4.0/bin/pip-install
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fixpoint_sdk-0.4.0/examples/__init__.py
+-rw-r--r--   0        0        0     5445 2020-02-02 00:00:00.000000 fixpoint_sdk-0.4.0/examples/main.py
+-rw-r--r--   0        0        0     1772 2020-02-02 00:00:00.000000 fixpoint_sdk-0.4.0/examples/streaming.py
+-rwxr-xr-x   0        0        0       78 2020-02-02 00:00:00.000000 fixpoint_sdk-0.4.0/githooks/pre-commit
+-rw-r--r--   0        0        0      515 2020-02-02 00:00:00.000000 fixpoint_sdk-0.4.0/src/fixpoint_sdk/__init__.py
+-rw-r--r--   0        0        0     3491 2020-02-02 00:00:00.000000 fixpoint_sdk-0.4.0/src/fixpoint_sdk/client.py
+-rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 fixpoint_sdk-0.4.0/src/fixpoint_sdk/compat.py
+-rw-r--r--   0        0        0    10547 2020-02-02 00:00:00.000000 fixpoint_sdk-0.4.0/src/fixpoint_sdk/completions.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fixpoint_sdk-0.4.0/src/fixpoint_sdk/py.typed
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fixpoint_sdk-0.4.0/src/fixpoint_sdk/lib/__init__.py
+-rw-r--r--   0        0        0     2298 2020-02-02 00:00:00.000000 fixpoint_sdk-0.4.0/src/fixpoint_sdk/lib/debugging.py
+-rw-r--r--   0        0        0     1620 2020-02-02 00:00:00.000000 fixpoint_sdk-0.4.0/src/fixpoint_sdk/lib/env.py
+-rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 fixpoint_sdk-0.4.0/src/fixpoint_sdk/lib/exc.py
+-rw-r--r--   0        0        0     1037 2020-02-02 00:00:00.000000 fixpoint_sdk-0.4.0/src/fixpoint_sdk/lib/iterwrapper.py
+-rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 fixpoint_sdk-0.4.0/src/fixpoint_sdk/lib/logging.py
+-rw-r--r--   0        0        0     7186 2020-02-02 00:00:00.000000 fixpoint_sdk-0.4.0/src/fixpoint_sdk/lib/requests.py
+-rw-r--r--   0        0        0      807 2020-02-02 00:00:00.000000 fixpoint_sdk-0.4.0/src/fixpoint_sdk/openapi/gen/.gitignore
+-rw-r--r--   0        0        0      709 2020-02-02 00:00:00.000000 fixpoint_sdk-0.4.0/src/fixpoint_sdk/openapi/gen/.gitlab-ci.yml
+-rw-r--r--   0        0        0     1040 2020-02-02 00:00:00.000000 fixpoint_sdk-0.4.0/src/fixpoint_sdk/openapi/gen/.openapi-generator-ignore
+-rw-r--r--   0        0        0      429 2020-02-02 00:00:00.000000 fixpoint_sdk-0.4.0/src/fixpoint_sdk/openapi/gen/.travis.yml
+-rw-r--r--   0        0        0     8526 2020-02-02 00:00:00.000000 fixpoint_sdk-0.4.0/src/fixpoint_sdk/openapi/gen/README.md
+-rw-r--r--   0        0        0     1830 2020-02-02 00:00:00.000000 fixpoint_sdk-0.4.0/src/fixpoint_sdk/openapi/gen/git_push.sh
+-rw-r--r--   0        0        0     1988 2020-02-02 00:00:00.000000 fixpoint_sdk-0.4.0/src/fixpoint_sdk/openapi/gen/pyproject.toml
+-rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 fixpoint_sdk-0.4.0/src/fixpoint_sdk/openapi/gen/requirements.txt
+-rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 fixpoint_sdk-0.4.0/src/fixpoint_sdk/openapi/gen/setup.cfg
+-rw-r--r--   0        0        0     1411 2020-02-02 00:00:00.000000 fixpoint_sdk-0.4.0/src/fixpoint_sdk/openapi/gen/setup.py
+-rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 fixpoint_sdk-0.4.0/src/fixpoint_sdk/openapi/gen/test-requirements.txt
+-rw-r--r--   0        0        0      150 2020-02-02 00:00:00.000000 fixpoint_sdk-0.4.0/src/fixpoint_sdk/openapi/gen/tox.ini
+-rw-r--r--   0        0        0     1352 2020-02-02 00:00:00.000000 fixpoint_sdk-0.4.0/src/fixpoint_sdk/openapi/gen/.github/workflows/python.yml
+-rw-r--r--   0        0        0     4744 2020-02-02 00:00:00.000000 fixpoint_sdk-0.4.0/src/fixpoint_sdk/openapi/gen/.openapi-generator/FILES
+-rw-r--r--   0        0        0        6 2020-02-02 00:00:00.000000 fixpoint_sdk-0.4.0/src/fixpoint_sdk/openapi/gen/.openapi-generator/VERSION
+-rw-r--r--   0        0        0      295 2020-02-02 00:00:00.000000 fixpoint_sdk-0.4.0/src/fixpoint_sdk/openapi/gen/docs/AppLogLevelType.md
+-rw-r--r--   0        0        0    44192 2020-02-02 00:00:00.000000 fixpoint_sdk-0.4.0/src/fixpoint_sdk/openapi/gen/docs/LLMProxyApi.md
+-rw-r--r--   0        0        0     1516 2020-02-02 00:00:00.000000 fixpoint_sdk-0.4.0/src/fixpoint_sdk/openapi/gen/docs/LLMProxyCreateOpenAIChatInputLogRequest.md
+-rw-r--r--   0        0        0     1648 2020-02-02 00:00:00.000000 fixpoint_sdk-0.4.0/src/fixpoint_sdk/openapi/gen/docs/LLMProxyCreateOpenAIChatOutputLogRequest.md
+-rw-r--r--   0        0        0     1137 2020-02-02 00:00:00.000000 fixpoint_sdk-0.4.0/src/fixpoint_sdk/openapi/gen/docs/LLMProxyPostDatasetLogsRequest.md
+-rw-r--r--   0        0        0     1217 2020-02-02 00:00:00.000000 fixpoint_sdk-0.4.0/src/fixpoint_sdk/openapi/gen/docs/LLMProxyUpdateSpendingTotalsRequest.md
+-rw-r--r--   0        0        0     1168 2020-02-02 00:00:00.000000 fixpoint_sdk-0.4.0/src/fixpoint_sdk/openapi/gen/docs/OpenAIChatOutputLogChoice.md
+-rw-r--r--   0        0        0     1150 2020-02-02 00:00:00.000000 fixpoint_sdk-0.4.0/src/fixpoint_sdk/openapi/gen/docs/OpenAIChatOutputLogUsage.md
+-rw-r--r--   0        0        0      851 2020-02-02 00:00:00.000000 fixpoint_sdk-0.4.0/src/fixpoint_sdk/openapi/gen/docs/ProtobufAny.md
+-rw-r--r--   0        0        0      477 2020-02-02 00:00:00.000000 fixpoint_sdk-0.4.0/src/fixpoint_sdk/openapi/gen/docs/ProtobufNullValue.md
+-rw-r--r--   0        0        0      935 2020-02-02 00:00:00.000000 fixpoint_sdk-0.4.0/src/fixpoint_sdk/openapi/gen/docs/RpcStatus.md
+-rw-r--r--   0        0        0     1116 2020-02-02 00:00:00.000000 fixpoint_sdk-0.4.0/src/fixpoint_sdk/openapi/gen/docs/V1ApiSecret.md
+-rw-r--r--   0        0        0      299 2020-02-02 00:00:00.000000 fixpoint_sdk-0.4.0/src/fixpoint_sdk/openapi/gen/docs/V1ApiSecretProvider.md
+-rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 fixpoint_sdk-0.4.0/src/fixpoint_sdk/openapi/gen/docs/V1AppLog.md
+-rw-r--r--   0        0        0      999 2020-02-02 00:00:00.000000 fixpoint_sdk-0.4.0/src/fixpoint_sdk/openapi/gen/docs/V1AttributeFilters.md
+-rw-r--r--   0        0        0     1205 2020-02-02 00:00:00.000000 fixpoint_sdk-0.4.0/src/fixpoint_sdk/openapi/gen/docs/V1CreateApiSecretRequest.md
+-rw-r--r--   0        0        0     1045 2020-02-02 00:00:00.000000 fixpoint_sdk-0.4.0/src/fixpoint_sdk/openapi/gen/docs/V1CreateAppLogsRequest.md
+-rw-r--r--   0        0        0     1032 2020-02-02 00:00:00.000000 fixpoint_sdk-0.4.0/src/fixpoint_sdk/openapi/gen/docs/V1CreateAppLogsResponse.md
+-rw-r--r--   0        0        0     1156 2020-02-02 00:00:00.000000 fixpoint_sdk-0.4.0/src/fixpoint_sdk/openapi/gen/docs/V1CreateDatasetRequest.md
+-rw-r--r--   0        0        0     1046 2020-02-02 00:00:00.000000 fixpoint_sdk-0.4.0/src/fixpoint_sdk/openapi/gen/docs/V1CreateDatasetResponse.md
+-rw-r--r--   0        0        0     1017 2020-02-02 00:00:00.000000 fixpoint_sdk-0.4.0/src/fixpoint_sdk/openapi/gen/docs/V1CreateLikesRequest.md
+-rw-r--r--   0        0        0      999 2020-02-02 00:00:00.000000 fixpoint_sdk-0.4.0/src/fixpoint_sdk/openapi/gen/docs/V1CreateLikesResponse.md
+-rw-r--r--   0        0        0     1121 2020-02-02 00:00:00.000000 fixpoint_sdk-0.4.0/src/fixpoint_sdk/openapi/gen/docs/V1CreateLogAttributeRequest.md
+-rw-r--r--   0        0        0     1134 2020-02-02 00:00:00.000000 fixpoint_sdk-0.4.0/src/fixpoint_sdk/openapi/gen/docs/V1CreateLogAttributeResponse.md
+-rw-r--r--   0        0        0     1331 2020-02-02 00:00:00.000000 fixpoint_sdk-0.4.0/src/fixpoint_sdk/openapi/gen/docs/V1CreateRoutingConfigRequest.md
+-rw-r--r--   0        0        0     1006 2020-02-02 00:00:00.000000 fixpoint_sdk-0.4.0/src/fixpoint_sdk/openapi/gen/docs/V1Dataset.md
+-rw-r--r--   0        0        0      938 2020-02-02 00:00:00.000000 fixpoint_sdk-0.4.0/src/fixpoint_sdk/openapi/gen/docs/V1DatasetFilters.md
+-rw-r--r--   0        0        0     1097 2020-02-02 00:00:00.000000 fixpoint_sdk-0.4.0/src/fixpoint_sdk/openapi/gen/docs/V1DeleteLogAttributeResponse.md
+-rw-r--r--   0        0        0      298 2020-02-02 00:00:00.000000 fixpoint_sdk-0.4.0/src/fixpoint_sdk/openapi/gen/docs/V1FallbackStrategy.md
+-rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 fixpoint_sdk-0.4.0/src/fixpoint_sdk/openapi/gen/docs/V1Like.md
+-rw-r--r--   0        0        0      918 2020-02-02 00:00:00.000000 fixpoint_sdk-0.4.0/src/fixpoint_sdk/openapi/gen/docs/V1LikeFilter.md
+-rw-r--r--   0        0        0     1063 2020-02-02 00:00:00.000000 fixpoint_sdk-0.4.0/src/fixpoint_sdk/openapi/gen/docs/V1LikeIngest.md
+-rw-r--r--   0        0        0     1080 2020-02-02 00:00:00.000000 fixpoint_sdk-0.4.0/src/fixpoint_sdk/openapi/gen/docs/V1ListApiSecretsResponse.md
+-rw-r--r--   0        0        0     1032 2020-02-02 00:00:00.000000 fixpoint_sdk-0.4.0/src/fixpoint_sdk/openapi/gen/docs/V1ListAppLogsResponse.md
+-rw-r--r--   0        0        0     1040 2020-02-02 00:00:00.000000 fixpoint_sdk-0.4.0/src/fixpoint_sdk/openapi/gen/docs/V1ListDatasetsResponse.md
+-rw-r--r--   0        0        0      992 2020-02-02 00:00:00.000000 fixpoint_sdk-0.4.0/src/fixpoint_sdk/openapi/gen/docs/V1ListLikesResponse.md
+-rw-r--r--   0        0        0     1128 2020-02-02 00:00:00.000000 fixpoint_sdk-0.4.0/src/fixpoint_sdk/openapi/gen/docs/V1ListLogAttributesResponse.md
+-rw-r--r--   0        0        0     1239 2020-02-02 00:00:00.000000 fixpoint_sdk-0.4.0/src/fixpoint_sdk/openapi/gen/docs/V1ListOpenAIChatLogsResponse.md
+-rw-r--r--   0        0        0     1191 2020-02-02 00:00:00.000000 fixpoint_sdk-0.4.0/src/fixpoint_sdk/openapi/gen/docs/V1ListRoutingConfigsResponse.md
+-rw-r--r--   0        0        0     1047 2020-02-02 00:00:00.000000 fixpoint_sdk-0.4.0/src/fixpoint_sdk/openapi/gen/docs/V1LogAttribute.md
+-rw-r--r--   0        0        0      864 2020-02-02 00:00:00.000000 fixpoint_sdk-0.4.0/src/fixpoint_sdk/openapi/gen/docs/V1Message.md
+-rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 fixpoint_sdk-0.4.0/src/fixpoint_sdk/openapi/gen/docs/V1Mode.md
+-rw-r--r--   0        0        0      978 2020-02-02 00:00:00.000000 fixpoint_sdk-0.4.0/src/fixpoint_sdk/openapi/gen/docs/V1Model.md
+-rw-r--r--   0        0        0     1282 2020-02-02 00:00:00.000000 fixpoint_sdk-0.4.0/src/fixpoint_sdk/openapi/gen/docs/V1OpenAIChatInputLog.md
+-rw-r--r--   0        0        0     1465 2020-02-02 00:00:00.000000 fixpoint_sdk-0.4.0/src/fixpoint_sdk/openapi/gen/docs/V1OpenAIChatLog.md
+-rw-r--r--   0        0        0     1361 2020-02-02 00:00:00.000000 fixpoint_sdk-0.4.0/src/fixpoint_sdk/openapi/gen/docs/V1OpenAIChatLogsFilters.md
+-rw-r--r--   0        0        0     1409 2020-02-02 00:00:00.000000 fixpoint_sdk-0.4.0/src/fixpoint_sdk/openapi/gen/docs/V1OpenAIChatOutputLog.md
+-rw-r--r--   0        0        0      292 2020-02-02 00:00:00.000000 fixpoint_sdk-0.4.0/src/fixpoint_sdk/openapi/gen/docs/V1OriginType.md
+-rw-r--r--   0        0        0     1058 2020-02-02 00:00:00.000000 fixpoint_sdk-0.4.0/src/fixpoint_sdk/openapi/gen/docs/V1PostDatasetLogsResponse.md
+-rw-r--r--   0        0        0     1056 2020-02-02 00:00:00.000000 fixpoint_sdk-0.4.0/src/fixpoint_sdk/openapi/gen/docs/V1RelativeDateTimeFilters.md
+-rw-r--r--   0        0        0      295 2020-02-02 00:00:00.000000 fixpoint_sdk-0.4.0/src/fixpoint_sdk/openapi/gen/docs/V1ResetInterval.md
+-rw-r--r--   0        0        0     1276 2020-02-02 00:00:00.000000 fixpoint_sdk-0.4.0/src/fixpoint_sdk/openapi/gen/docs/V1RoutingConfig.md
+-rw-r--r--   0        0        0      967 2020-02-02 00:00:00.000000 fixpoint_sdk-0.4.0/src/fixpoint_sdk/openapi/gen/docs/V1SpendCap.md
+-rw-r--r--   0        0        0      471 2020-02-02 00:00:00.000000 fixpoint_sdk-0.4.0/src/fixpoint_sdk/openapi/gen/docs/V1TerminalState.md
+-rw-r--r--   0        0        0      296 2020-02-02 00:00:00.000000 fixpoint_sdk-0.4.0/src/fixpoint_sdk/openapi/gen/docs/V1ThumbsReaction.md
+-rw-r--r--   0        0        0     1020 2020-02-02 00:00:00.000000 fixpoint_sdk-0.4.0/src/fixpoint_sdk/openapi/gen/docs/V1UsageTotals.md
+-rw-r--r--   0        0        0     4392 2020-02-02 00:00:00.000000 fixpoint_sdk-0.4.0/src/fixpoint_sdk/openapi/gen/openapi_client/__init__.py
+-rw-r--r--   0        0        0    25750 2020-02-02 00:00:00.000000 fixpoint_sdk-0.4.0/src/fixpoint_sdk/openapi/gen/openapi_client/api_client.py
+-rw-r--r--   0        0        0      652 2020-02-02 00:00:00.000000 fixpoint_sdk-0.4.0/src/fixpoint_sdk/openapi/gen/openapi_client/api_response.py
+-rw-r--r--   0        0        0    14511 2020-02-02 00:00:00.000000 fixpoint_sdk-0.4.0/src/fixpoint_sdk/openapi/gen/openapi_client/configuration.py
+-rw-r--r--   0        0        0     6009 2020-02-02 00:00:00.000000 fixpoint_sdk-0.4.0/src/fixpoint_sdk/openapi/gen/openapi_client/exceptions.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fixpoint_sdk-0.4.0/src/fixpoint_sdk/openapi/gen/openapi_client/py.typed
+-rw-r--r--   0        0        0     9255 2020-02-02 00:00:00.000000 fixpoint_sdk-0.4.0/src/fixpoint_sdk/openapi/gen/openapi_client/rest.py
+-rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 fixpoint_sdk-0.4.0/src/fixpoint_sdk/openapi/gen/openapi_client/api/__init__.py
+-rw-r--r--   0        0        0   198013 2020-02-02 00:00:00.000000 fixpoint_sdk-0.4.0/src/fixpoint_sdk/openapi/gen/openapi_client/api/llm_proxy_api.py
+-rw-r--r--   0        0        0     3546 2020-02-02 00:00:00.000000 fixpoint_sdk-0.4.0/src/fixpoint_sdk/openapi/gen/openapi_client/models/__init__.py
+-rw-r--r--   0        0        0      867 2020-02-02 00:00:00.000000 fixpoint_sdk-0.4.0/src/fixpoint_sdk/openapi/gen/openapi_client/models/app_log_level_type.py
+-rw-r--r--   0        0        0     3755 2020-02-02 00:00:00.000000 fixpoint_sdk-0.4.0/src/fixpoint_sdk/openapi/gen/openapi_client/models/llm_proxy_create_open_ai_chat_input_log_request.py
+-rw-r--r--   0        0        0     4204 2020-02-02 00:00:00.000000 fixpoint_sdk-0.4.0/src/fixpoint_sdk/openapi/gen/openapi_client/models/llm_proxy_create_open_ai_chat_output_log_request.py
+-rw-r--r--   0        0        0     2663 2020-02-02 00:00:00.000000 fixpoint_sdk-0.4.0/src/fixpoint_sdk/openapi/gen/openapi_client/models/llm_proxy_post_dataset_logs_request.py
+-rw-r--r--   0        0        0     3031 2020-02-02 00:00:00.000000 fixpoint_sdk-0.4.0/src/fixpoint_sdk/openapi/gen/openapi_client/models/llm_proxy_update_spending_totals_request.py
+-rw-r--r--   0        0        0     3097 2020-02-02 00:00:00.000000 fixpoint_sdk-0.4.0/src/fixpoint_sdk/openapi/gen/openapi_client/models/open_ai_chat_output_log_choice.py
+-rw-r--r--   0        0        0     2972 2020-02-02 00:00:00.000000 fixpoint_sdk-0.4.0/src/fixpoint_sdk/openapi/gen/openapi_client/models/open_ai_chat_output_log_usage.py
+-rw-r--r--   0        0        0     3159 2020-02-02 00:00:00.000000 fixpoint_sdk-0.4.0/src/fixpoint_sdk/openapi/gen/openapi_client/models/protobuf_any.py
+-rw-r--r--   0        0        0      949 2020-02-02 00:00:00.000000 fixpoint_sdk-0.4.0/src/fixpoint_sdk/openapi/gen/openapi_client/models/protobuf_null_value.py
+-rw-r--r--   0        0        0     3150 2020-02-02 00:00:00.000000 fixpoint_sdk-0.4.0/src/fixpoint_sdk/openapi/gen/openapi_client/models/rpc_status.py
+-rw-r--r--   0        0        0     3201 2020-02-02 00:00:00.000000 fixpoint_sdk-0.4.0/src/fixpoint_sdk/openapi/gen/openapi_client/models/v1_api_secret.py
+-rw-r--r--   0        0        0      897 2020-02-02 00:00:00.000000 fixpoint_sdk-0.4.0/src/fixpoint_sdk/openapi/gen/openapi_client/models/v1_api_secret_provider.py
+-rw-r--r--   0        0        0     3238 2020-02-02 00:00:00.000000 fixpoint_sdk-0.4.0/src/fixpoint_sdk/openapi/gen/openapi_client/models/v1_app_log.py
+-rw-r--r--   0        0        0     2654 2020-02-02 00:00:00.000000 fixpoint_sdk-0.4.0/src/fixpoint_sdk/openapi/gen/openapi_client/models/v1_attribute_filters.py
+-rw-r--r--   0        0        0     2944 2020-02-02 00:00:00.000000 fixpoint_sdk-0.4.0/src/fixpoint_sdk/openapi/gen/openapi_client/models/v1_create_api_secret_request.py
+-rw-r--r--   0        0        0     3036 2020-02-02 00:00:00.000000 fixpoint_sdk-0.4.0/src/fixpoint_sdk/openapi/gen/openapi_client/models/v1_create_app_logs_request.py
+-rw-r--r--   0        0        0     2586 2020-02-02 00:00:00.000000 fixpoint_sdk-0.4.0/src/fixpoint_sdk/openapi/gen/openapi_client/models/v1_create_app_logs_response.py
+-rw-r--r--   0        0        0     2985 2020-02-02 00:00:00.000000 fixpoint_sdk-0.4.0/src/fixpoint_sdk/openapi/gen/openapi_client/models/v1_create_dataset_request.py
+-rw-r--r--   0        0        0     2833 2020-02-02 00:00:00.000000 fixpoint_sdk-0.4.0/src/fixpoint_sdk/openapi/gen/openapi_client/models/v1_create_dataset_response.py
+-rw-r--r--   0        0        0     2983 2020-02-02 00:00:00.000000 fixpoint_sdk-0.4.0/src/fixpoint_sdk/openapi/gen/openapi_client/models/v1_create_likes_request.py
+-rw-r--r--   0        0        0     2578 2020-02-02 00:00:00.000000 fixpoint_sdk-0.4.0/src/fixpoint_sdk/openapi/gen/openapi_client/models/v1_create_likes_response.py
+-rw-r--r--   0        0        0     2963 2020-02-02 00:00:00.000000 fixpoint_sdk-0.4.0/src/fixpoint_sdk/openapi/gen/openapi_client/models/v1_create_log_attribute_request.py
+-rw-r--r--   0        0        0     2967 2020-02-02 00:00:00.000000 fixpoint_sdk-0.4.0/src/fixpoint_sdk/openapi/gen/openapi_client/models/v1_create_log_attribute_response.py
+-rw-r--r--   0        0        0     3575 2020-02-02 00:00:00.000000 fixpoint_sdk-0.4.0/src/fixpoint_sdk/openapi/gen/openapi_client/models/v1_create_routing_config_request.py
+-rw-r--r--   0        0        0     3082 2020-02-02 00:00:00.000000 fixpoint_sdk-0.4.0/src/fixpoint_sdk/openapi/gen/openapi_client/models/v1_dataset.py
+-rw-r--r--   0        0        0     2627 2020-02-02 00:00:00.000000 fixpoint_sdk-0.4.0/src/fixpoint_sdk/openapi/gen/openapi_client/models/v1_dataset_filters.py
+-rw-r--r--   0        0        0     2606 2020-02-02 00:00:00.000000 fixpoint_sdk-0.4.0/src/fixpoint_sdk/openapi/gen/openapi_client/models/v1_delete_log_attribute_response.py
+-rw-r--r--   0        0        0      882 2020-02-02 00:00:00.000000 fixpoint_sdk-0.4.0/src/fixpoint_sdk/openapi/gen/openapi_client/models/v1_fallback_strategy.py
+-rw-r--r--   0        0        0     3332 2020-02-02 00:00:00.000000 fixpoint_sdk-0.4.0/src/fixpoint_sdk/openapi/gen/openapi_client/models/v1_like.py
+-rw-r--r--   0        0        0     2660 2020-02-02 00:00:00.000000 fixpoint_sdk-0.4.0/src/fixpoint_sdk/openapi/gen/openapi_client/models/v1_like_filter.py
+-rw-r--r--   0        0        0     3054 2020-02-02 00:00:00.000000 fixpoint_sdk-0.4.0/src/fixpoint_sdk/openapi/gen/openapi_client/models/v1_like_ingest.py
+-rw-r--r--   0        0        0     3086 2020-02-02 00:00:00.000000 fixpoint_sdk-0.4.0/src/fixpoint_sdk/openapi/gen/openapi_client/models/v1_list_api_secrets_response.py
+-rw-r--r--   0        0        0     3032 2020-02-02 00:00:00.000000 fixpoint_sdk-0.4.0/src/fixpoint_sdk/openapi/gen/openapi_client/models/v1_list_app_logs_response.py
+-rw-r--r--   0        0        0     3005 2020-02-02 00:00:00.000000 fixpoint_sdk-0.4.0/src/fixpoint_sdk/openapi/gen/openapi_client/models/v1_list_datasets_response.py
+-rw-r--r--   0        0        0     2954 2020-02-02 00:00:00.000000 fixpoint_sdk-0.4.0/src/fixpoint_sdk/openapi/gen/openapi_client/models/v1_list_likes_response.py
+-rw-r--r--   0        0        0     3140 2020-02-02 00:00:00.000000 fixpoint_sdk-0.4.0/src/fixpoint_sdk/openapi/gen/openapi_client/models/v1_list_log_attributes_response.py
+-rw-r--r--   0        0        0     3582 2020-02-02 00:00:00.000000 fixpoint_sdk-0.4.0/src/fixpoint_sdk/openapi/gen/openapi_client/models/v1_list_open_ai_chat_logs_response.py
+-rw-r--r--   0        0        0     3327 2020-02-02 00:00:00.000000 fixpoint_sdk-0.4.0/src/fixpoint_sdk/openapi/gen/openapi_client/models/v1_list_routing_configs_response.py
+-rw-r--r--   0        0        0     2951 2020-02-02 00:00:00.000000 fixpoint_sdk-0.4.0/src/fixpoint_sdk/openapi/gen/openapi_client/models/v1_log_attribute.py
+-rw-r--r--   0        0        0     2610 2020-02-02 00:00:00.000000 fixpoint_sdk-0.4.0/src/fixpoint_sdk/openapi/gen/openapi_client/models/v1_message.py
+-rw-r--r--   0        0        0      856 2020-02-02 00:00:00.000000 fixpoint_sdk-0.4.0/src/fixpoint_sdk/openapi/gen/openapi_client/models/v1_mode.py
+-rw-r--r--   0        0        0     3465 2020-02-02 00:00:00.000000 fixpoint_sdk-0.4.0/src/fixpoint_sdk/openapi/gen/openapi_client/models/v1_model.py
+-rw-r--r--   0        0        0     3835 2020-02-02 00:00:00.000000 fixpoint_sdk-0.4.0/src/fixpoint_sdk/openapi/gen/openapi_client/models/v1_open_ai_chat_input_log.py
+-rw-r--r--   0        0        0     4407 2020-02-02 00:00:00.000000 fixpoint_sdk-0.4.0/src/fixpoint_sdk/openapi/gen/openapi_client/models/v1_open_ai_chat_log.py
+-rw-r--r--   0        0        0     4626 2020-02-02 00:00:00.000000 fixpoint_sdk-0.4.0/src/fixpoint_sdk/openapi/gen/openapi_client/models/v1_open_ai_chat_logs_filters.py
+-rw-r--r--   0        0        0     4259 2020-02-02 00:00:00.000000 fixpoint_sdk-0.4.0/src/fixpoint_sdk/openapi/gen/openapi_client/models/v1_open_ai_chat_output_log.py
+-rw-r--r--   0        0        0      872 2020-02-02 00:00:00.000000 fixpoint_sdk-0.4.0/src/fixpoint_sdk/openapi/gen/openapi_client/models/v1_origin_type.py
+-rw-r--r--   0        0        0     2594 2020-02-02 00:00:00.000000 fixpoint_sdk-0.4.0/src/fixpoint_sdk/openapi/gen/openapi_client/models/v1_post_dataset_logs_response.py
+-rw-r--r--   0        0        0     2622 2020-02-02 00:00:00.000000 fixpoint_sdk-0.4.0/src/fixpoint_sdk/openapi/gen/openapi_client/models/v1_relative_date_time_filters.py
+-rw-r--r--   0        0        0      969 2020-02-02 00:00:00.000000 fixpoint_sdk-0.4.0/src/fixpoint_sdk/openapi/gen/openapi_client/models/v1_reset_interval.py
+-rw-r--r--   0        0        0     3899 2020-02-02 00:00:00.000000 fixpoint_sdk-0.4.0/src/fixpoint_sdk/openapi/gen/openapi_client/models/v1_routing_config.py
+-rw-r--r--   0        0        0     2843 2020-02-02 00:00:00.000000 fixpoint_sdk-0.4.0/src/fixpoint_sdk/openapi/gen/openapi_client/models/v1_spend_cap.py
+-rw-r--r--   0        0        0     1083 2020-02-02 00:00:00.000000 fixpoint_sdk-0.4.0/src/fixpoint_sdk/openapi/gen/openapi_client/models/v1_terminal_state.py
+-rw-r--r--   0        0        0      860 2020-02-02 00:00:00.000000 fixpoint_sdk-0.4.0/src/fixpoint_sdk/openapi/gen/openapi_client/models/v1_thumbs_reaction.py
+-rw-r--r--   0        0        0     2980 2020-02-02 00:00:00.000000 fixpoint_sdk-0.4.0/src/fixpoint_sdk/openapi/gen/openapi_client/models/v1_usage_totals.py
+-rw-r--r--   0        0        0     5138 2020-02-02 00:00:00.000000 fixpoint_sdk-0.4.0/src/fixpoint_sdk/types/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fixpoint_sdk-0.4.0/tests/__init__.py
+-rw-r--r--   0        0        0    15061 2020-02-02 00:00:00.000000 fixpoint_sdk-0.4.0/tests/mock_completions.py
+-rw-r--r--   0        0        0     2978 2020-02-02 00:00:00.000000 fixpoint_sdk-0.4.0/tests/test_completions.py
+-rw-r--r--   0        0        0      961 2020-02-02 00:00:00.000000 fixpoint_sdk-0.4.0/tests/test_types.py
+-rw-r--r--   0        0        0     1977 2020-02-02 00:00:00.000000 fixpoint_sdk-0.4.0/tests/lib/test_iterwrapper.py
+-rw-r--r--   0        0        0    10018 2020-02-02 00:00:00.000000 fixpoint_sdk-0.4.0/tests/lib/test_requests.py
+-rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 fixpoint_sdk-0.4.0/.gitignore
+-rw-r--r--   0        0        0    11338 2020-02-02 00:00:00.000000 fixpoint_sdk-0.4.0/LICENSE
+-rw-r--r--   0        0        0     1601 2020-02-02 00:00:00.000000 fixpoint_sdk-0.4.0/README.md
+-rw-r--r--   0        0        0      995 2020-02-02 00:00:00.000000 fixpoint_sdk-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0     2838 2020-02-02 00:00:00.000000 fixpoint_sdk-0.4.0/PKG-INFO
```

### Comparing `fixpoint_sdk-0.3.0/.pylintrc` & `fixpoint_sdk-0.4.0/.pylintrc`

 * *Files 0% similar despite different names*

```diff
@@ -48,15 +48,15 @@
 # Files or directories to be skipped. They should be base names, not paths.
 ignore=CVS
 
 # Add files or directories matching the regular expressions patterns to the
 # ignore-list. The regex matches against paths and can be in Posix or Windows
 # format. Because '\\' represents the directory delimiter on Windows systems,
 # it can't be used as an escape character.
-ignore-paths=
+ignore-paths=src/fixpoint_sdk/openapi
 
 # Files or directories matching the regular expression patterns are skipped.
 # The regex matches against base names, not paths. The default value ignores
 # Emacs file locks
 ignore-patterns=^\.#
 
 # List of module names for which member attributes should not be checked
```

### Comparing `fixpoint_sdk-0.3.0/mypy.ini` & `fixpoint_sdk-0.4.0/mypy.ini`

 * *Files 16% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [mypy]
-exclude = (examples/|venv/)
+exclude = (examples/|venv/|src/fixpoint_sdk/openapi)
 # Start off with these
 warn_unused_configs = True
 warn_redundant_casts = True
 warn_unused_ignores = True
 
 # Getting these passing should be easy
 strict_equality = True
```

### Comparing `fixpoint_sdk-0.3.0/requirements.txt` & `fixpoint_sdk-0.4.0/requirements.txt`

 * *Files identical despite different names*

### Comparing `fixpoint_sdk-0.3.0/.github/workflows/ci.yml` & `fixpoint_sdk-0.4.0/.github/workflows/ci.yml`

 * *Files 3% similar despite different names*

```diff
@@ -38,15 +38,15 @@
         working-directory: ${{ github.workspace }}
 
       - name: Typecheck Python
         run: mypy .
         working-directory: ${{ github.workspace }}
 
       - name: Format Python
-        run: black --check .
+        run: black --check . --extend-exclude src/fixpoint_sdk/openapi
         working-directory: ${{ github.workspace }}
 
       - name: Lint Python
         run: pylint src/ examples/ tests/
         working-directory: ${{ github.workspace }}
 
       - name: Test Python
```

### Comparing `fixpoint_sdk-0.3.0/.github/workflows/pypi-release-prod.yml` & `fixpoint_sdk-0.4.0/.github/workflows/pypi-release-prod.yml`

 * *Files identical despite different names*

### Comparing `fixpoint_sdk-0.3.0/.github/workflows/pypi-release-test.yml` & `fixpoint_sdk-0.4.0/.github/workflows/pypi-release-test.yml`

 * *Files identical despite different names*

### Comparing `fixpoint_sdk-0.3.0/bin/pip-freeze` & `fixpoint_sdk-0.4.0/bin/pip-freeze`

 * *Files identical despite different names*

### Comparing `fixpoint_sdk-0.3.0/examples/streaming.py` & `fixpoint_sdk-0.4.0/examples/streaming.py`

 * *Files identical despite different names*

### Comparing `fixpoint_sdk-0.3.0/src/fixpoint_sdk/__init__.py` & `fixpoint_sdk-0.4.0/src/fixpoint_sdk/__init__.py`

 * *Files identical despite different names*

### Comparing `fixpoint_sdk-0.3.0/src/fixpoint_sdk/compat.py` & `fixpoint_sdk-0.4.0/src/fixpoint_sdk/compat.py`

 * *Files identical despite different names*

### Comparing `fixpoint_sdk-0.3.0/src/fixpoint_sdk/completions.py` & `fixpoint_sdk-0.4.0/src/fixpoint_sdk/completions.py`

 * *Files 6% similar despite different names*

```diff
@@ -14,14 +14,21 @@
 from .lib.debugging import dprint
 from .lib.iterwrapper import IterWrapper
 from .lib.logging import logger
 from . import types
 
 
 @dataclass
+class FixpointChatRoutedCompletion:
+    """Wraps the OpenAI chat completion with logging data."""
+
+    completion: types.ChatCompletion
+
+
+@dataclass
 class FixpointChatCompletion:
     """Wraps the OpenAI chat completion with logging data."""
 
     completion: ChatCompletion
     input_log: types.InputLog
     output_log: types.OutputLog
 
@@ -260,12 +267,48 @@
             mode_type=mode_type,
             requester=self._requester,
             trace_id=trace_id,
             model_name=req_copy["model_name"],
         )
 
 
+class RoutedCompletions:
+    """Create chat completion inferences and log them."""
+
+    def __init__(self, requester: Requester, client: OpenAI):
+        self._requester = requester
+        self._client = client
+
+    def create(
+        self,
+        mode: Optional[types.ModeArg] = "unspecified",
+        **kwargs: typing.Any,
+    ) -> typing.Union[FixpointChatRoutedCompletion]:
+        """Create an OpenAI completion and log the LLM input and output."""
+        # Prepare the request
+        req_copy = kwargs.copy()
+        trace_id = kwargs.pop("trace_id", None)
+
+        routed_log_resp = self._requester.create_openai_routed_log(
+            typing.cast(types.OpenAILLMInputLog, req_copy),
+            mode=types.parse_mode_type(mode),
+            trace_id=trace_id,
+        )
+        dprint(f"Created a routed log: {routed_log_resp['id']}")
+
+        return FixpointChatRoutedCompletion(
+            completion=routed_log_resp,
+        )
+
+
+class ChatWithRouter:
+    """The Chat class lets you interact with the underlying chat APIs."""
+
+    def __init__(self, requester: Requester, client: OpenAI):
+        self.completions = RoutedCompletions(requester, client)
+
+
 class Chat:
     """The Chat class lets you interact with the underlying chat APIs."""
 
     def __init__(self, requester: Requester, client: OpenAI):
         self.completions = Completions(requester, client)
```

### Comparing `fixpoint_sdk-0.3.0/src/fixpoint_sdk/lib/debugging.py` & `fixpoint_sdk-0.4.0/src/fixpoint_sdk/lib/debugging.py`

 * *Files identical despite different names*

### Comparing `fixpoint_sdk-0.3.0/src/fixpoint_sdk/lib/env.py` & `fixpoint_sdk-0.4.0/src/fixpoint_sdk/lib/env.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -2,14 +2,18 @@
 
 import os
 import typing
 
 from .exc import InitException
 from .logging import logger
 
+BASE_URL = "https://api.fixpoint.co"
+
+_FIXPOINT_BASE_URL_ENV_KEY = "FIXPOINT_API_BASE_URL"
+
 
 def get_fixpoint_api_key(api_key: typing.Optional[str]) -> str:
     """Returns the Fixpoint API key from the environment or the argument.
 
     Returns the Fixpoint API key from the environment or the argument,
     preferring the argument. If no key is defined, we raise an exception.
     """
@@ -23,18 +27,14 @@
     key = os.environ["FIXPOINT_API_KEY"]
     if not key:
         logger.error("FIXPOINT_API_KEY env variable is empty.")
         raise InitException("Fixpoint API key is empty")
     return key
 
 
-BASE_URL = "https://api.fixpoint.co"
-_FIXPOINT_BASE_URL_ENV_KEY = "FIXPOINT_API_BASE_URL"
-
-
 def get_api_base_url(base_url: typing.Optional[str]) -> str:
     """Returns the API base URL for Fixpoint. If not set, returns the default."""
     burl = _get_api_base_url(base_url)
     if burl[-1] == "/":
         return burl[:-1]
     return burl
```

### Comparing `fixpoint_sdk-0.3.0/src/fixpoint_sdk/lib/iterwrapper.py` & `fixpoint_sdk-0.4.0/src/fixpoint_sdk/lib/iterwrapper.py`

 * *Files identical despite different names*

### Comparing `fixpoint_sdk-0.3.0/src/fixpoint_sdk/lib/requests.py` & `fixpoint_sdk-0.4.0/src/fixpoint_sdk/lib/requests.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,16 +4,14 @@
 
 import requests
 from openai.types.chat import ChatCompletion
 
 from .debugging import debug_log_function_io
 from .. import types
 
-
-BASE_URL = "https://api.fixpoint.co"
 DEFAULT_TIMEOUT_S = 60
 
 ApiCallback = typing.Callable[[str, typing.Any, typing.Any], None]
 
 
 class Requester:
     """Makes requests to the Fixpoint API."""
@@ -36,14 +34,36 @@
 
         if self.base_url[-1] == "/":
             self.base_url = self.base_url[:-1]
 
         self._on_api_call = _on_api_call
 
     @debug_log_function_io
+    def create_openai_routed_log(
+        self,
+        request: types.OpenAILLMInputLog,
+        trace_id: typing.Optional[str] = None,
+        mode: types.ModeType = types.ModeType.MODE_UNSPECIFIED,
+    ) -> types.ChatCompletion:
+        """Create routed input log for an LLM inference request."""
+        url = f"{self.base_url}/v1/router"
+        input_log_req = types.CreateLLMRoutingRequest(
+            messages=request["messages"],
+            user_id=request.get("user", None),
+            temperature=request.get("temperature", None),
+            trace_id=trace_id,
+            mode=mode,
+        )
+
+        return typing.cast(
+            types.ChatCompletion,
+            self._post_to_fixpoint(url, input_log_req.to_dict()).json(),
+        )
+
+    @debug_log_function_io
     def create_openai_input_log(
         self,
         model_name: str,
         request: types.OpenAILLMInputLog,
         trace_id: typing.Optional[str] = None,
         mode: types.ModeType = types.ModeType.MODE_UNSPECIFIED,
     ) -> types.InputLog:
```

### Comparing `fixpoint_sdk-0.3.0/src/fixpoint_sdk/types/__init__.py` & `fixpoint_sdk-0.4.0/src/fixpoint_sdk/types/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -69,19 +69,37 @@
             return ModeType.MODE_STAGING
         if mode == "prod":
             return ModeType.MODE_PROD
     raise ValueError(f"Unknown mode: {mode}")
 
 
 @dataclass
+class CreateLLMRoutingRequest:
+    """Request to create a routing for an LLM."""
+
+    messages: List[ChatCompletionMessageParam]
+    temperature: Optional[float] = None
+    user_id: Optional[str] = None
+    trace_id: Optional[str] = None
+    mode: Optional[ModeType] = ModeType.MODE_UNSPECIFIED
+
+    def to_dict(self) -> Dict[str, Any]:
+        """Convert this request to a dictionary."""
+        d = asdict(self)
+        if self.mode is not None:
+            d["mode"] = self.mode.value
+        return d
+
+
+@dataclass
 class CreateLLMInputLogRequest:
     """Request to create a log of a chat completion input."""
 
-    model_name: str
     messages: List[ChatCompletionMessageParam]
+    model_name: str
     user_id: Optional[str] = None
     temperature: Optional[float] = None
     trace_id: Optional[str] = None
     mode: Optional[ModeType] = ModeType.MODE_UNSPECIFIED
 
     def to_dict(self) -> Dict[str, Any]:
         """Convert this request to a dictionary."""
@@ -103,14 +121,25 @@
     model: str
     messages: List[ChatCompletionMessageParam]
     user: Optional[str]
     temperature: Optional[float]
     trace_id: Optional[str]
 
 
+# TODO(jakub) this is an incomplete definition.
+class ChatCompletion(TypedDict):
+    """A chat completion."""
+
+    id: str
+    choices: List[Any]
+    created: int
+    model: str
+    object: Literal["chat.completion"]
+
+
 # TODO(dbmikus) this is an incomplete definition.
 class InputLog(TypedDict):
     """An LLM input log."""
 
     name: str
     modelName: Optional[str]
     sessionName: Optional[str]
```

### Comparing `fixpoint_sdk-0.3.0/tests/mock_completions.py` & `fixpoint_sdk-0.4.0/tests/mock_completions.py`

 * *Files identical despite different names*

### Comparing `fixpoint_sdk-0.3.0/tests/test_completions.py` & `fixpoint_sdk-0.4.0/tests/test_completions.py`

 * *Files identical despite different names*

### Comparing `fixpoint_sdk-0.3.0/tests/test_types.py` & `fixpoint_sdk-0.4.0/tests/test_types.py`

 * *Files identical despite different names*

### Comparing `fixpoint_sdk-0.3.0/tests/lib/test_iterwrapper.py` & `fixpoint_sdk-0.4.0/tests/lib/test_iterwrapper.py`

 * *Files identical despite different names*

### Comparing `fixpoint_sdk-0.3.0/tests/lib/test_requests.py` & `fixpoint_sdk-0.4.0/tests/lib/test_requests.py`

 * *Files identical despite different names*

### Comparing `fixpoint_sdk-0.3.0/LICENSE` & `fixpoint_sdk-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `fixpoint_sdk-0.3.0/README.md` & `fixpoint_sdk-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `fixpoint_sdk-0.3.0/pyproject.toml` & `fixpoint_sdk-0.4.0/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "fixpoint_sdk"
-version = "0.3.0"
+version = "0.4.0"
 
 authors = [
 { name="Jakub Cichon", email="jakub@fixpoint.co" },
 { name="Dylan Mikus", email="dylan@fixpoint.co" },
 ]
 description = "Python SDK for Fixpoint - Auto-improvement to make your LLM apps smarter"
 readme = "README.md"
@@ -31,12 +31,16 @@
   "ipdb>=0.13.13",
   "mypy>=1.8",
   "pylint>=3",
   "pytest>=8.0.2",
   "requests-mock>=1.11.0",
   "twine>=5.0.0",
   "types-requests>=2.31.0",
+  "urllib3>=1.25.3",
+  "python-dateutil>=2.8.2",
+  "pydantic>=2",
+  "typing-extensions>=4.7.1"
 ]
 
 [project.urls]
 Homepage = "https://github.com/gofixpoint/python-sdk"
 Issues = "https://github.com/gofixpoint/python-sdk/issues"
```

### Comparing `fixpoint_sdk-0.3.0/PKG-INFO` & `fixpoint_sdk-0.4.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: fixpoint_sdk
-Version: 0.3.0
+Version: 0.4.0
 Summary: Python SDK for Fixpoint - Auto-improvement to make your LLM apps smarter
 Project-URL: Homepage, https://github.com/gofixpoint/python-sdk
 Project-URL: Issues, https://github.com/gofixpoint/python-sdk/issues
 Author-email: Jakub Cichon <jakub@fixpoint.co>, Dylan Mikus <dylan@fixpoint.co>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
@@ -12,19 +12,23 @@
 Requires-Dist: openai>=1.6.1
 Requires-Dist: requests==2.31.0
 Provides-Extra: dev
 Requires-Dist: black>=24; extra == 'dev'
 Requires-Dist: build>=1.1.1; extra == 'dev'
 Requires-Dist: ipdb>=0.13.13; extra == 'dev'
 Requires-Dist: mypy>=1.8; extra == 'dev'
+Requires-Dist: pydantic>=2; extra == 'dev'
 Requires-Dist: pylint>=3; extra == 'dev'
 Requires-Dist: pytest>=8.0.2; extra == 'dev'
+Requires-Dist: python-dateutil>=2.8.2; extra == 'dev'
 Requires-Dist: requests-mock>=1.11.0; extra == 'dev'
 Requires-Dist: twine>=5.0.0; extra == 'dev'
 Requires-Dist: types-requests>=2.31.0; extra == 'dev'
+Requires-Dist: typing-extensions>=4.7.1; extra == 'dev'
+Requires-Dist: urllib3>=1.25.3; extra == 'dev'
 Description-Content-Type: text/markdown
 
 # Fixpoint Python SDK
 
 The `FixpointClient` wraps the OpenAI API Client. You can call it just like OpenAI API Client. The sdk will intercept calls to certain OpenAI APIs, record input / outputs and forward that information to Fixpoint's api server.
 
 ## Installation
```

