# Comparing `tmp/esbmc_ai-0.5.0.dev5.tar.gz` & `tmp/esbmc_ai-0.5.0.dev6.tar.gz`

## Comparing `esbmc_ai-0.5.0.dev5.tar` & `esbmc_ai-0.5.0.dev6.tar`

### file list

```diff
@@ -1,76 +1,76 @@
--rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev5/.env.example
--rw-r--r--   0        0        0    21341 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev5/.pylintrc
--rw-r--r--   0        0        0      731 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev5/Pipfile
--rwxr-xr-x   0        0        0       62 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev5/build.sh
--rwxr-xr-x   0        0        0       81 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev5/clean.sh
--rw-r--r--   0        0        0     5106 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev5/config.json
--rwxr-xr-x   0        0        0       41 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev5/esbmc-ai
--rw-r--r--   0        0        0     6657 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev5/requirements.txt
--rwxr-xr-x   0        0        0      412 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev5/upload.sh
--rw-r--r--   0        0        0     1495 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev5/.github/workflows/workflow.yml
--rw-r--r--   0        0        0      371 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev5/.vscode/c_cpp_properties.json
--rw-r--r--   0        0        0     1696 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev5/.vscode/launch.json
--rw-r--r--   0        0        0      105 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev5/.vscode/settings.json
--rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev5/esbmc_ai/__about__.py
--rw-r--r--   0        0        0      238 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev5/esbmc_ai/__init__.py
--rwxr-xr-x   0        0        0    14539 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev5/esbmc_ai/__main__.py
--rw-r--r--   0        0        0    12079 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev5/esbmc_ai/ai_models.py
--rw-r--r--   0        0        0      241 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev5/esbmc_ai/api_key_collection.py
--rw-r--r--   0        0        0     3347 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev5/esbmc_ai/base_chat_interface.py
--rw-r--r--   0        0        0     1547 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev5/esbmc_ai/chat_response.py
--rw-r--r--   0        0        0    15345 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev5/esbmc_ai/config.py
--rw-r--r--   0        0        0     4510 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev5/esbmc_ai/esbmc_util.py
--rw-r--r--   0        0        0     2487 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev5/esbmc_ai/loading_widget.py
--rw-r--r--   0        0        0      769 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev5/esbmc_ai/logging.py
--rw-r--r--   0        0        0      414 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev5/esbmc_ai/msg_bus.py
--rw-r--r--   0        0        0     1226 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev5/esbmc_ai/optimize_code.py
--rw-r--r--   0        0        0     5421 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev5/esbmc_ai/solution_generator.py
--rw-r--r--   0        0        0     2899 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev5/esbmc_ai/user_chat.py
--rw-r--r--   0        0        0      253 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev5/esbmc_ai/commands/__init__.py
--rw-r--r--   0        0        0      565 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev5/esbmc_ai/commands/chat_command.py
--rw-r--r--   0        0        0      458 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev5/esbmc_ai/commands/exit_command.py
--rw-r--r--   0        0        0     6147 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev5/esbmc_ai/commands/fix_code_command.py
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev5/esbmc_ai/commands/help_command.py
--rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev5/esbmc_ai/frontend/__init__.py
--rw-r--r--   0        0        0     1667 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev5/esbmc_ai/frontend/solution.py
--rw-r--r--   0        0        0    18626 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev5/notebooks/ast.ipynb
--rw-r--r--   0        0        0      557 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev5/notebooks/samples/typedefs.c
--rw-r--r--   0        0        0      565 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev5/samples/add_last_unsafe.c
--rw-r--r--   0        0        0      378 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev5/samples/automatic_arrays.c
--rw-r--r--   0        0        0      448 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev5/samples/dynamic_mem_alloc.c
--rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev5/samples/hello_world.c
--rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev5/samples/mem_leak.c
--rw-r--r--   0        0        0      272 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev5/samples/optimize_code_test_01.c
--rw-r--r--   0        0        0      363 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev5/samples/threading.c
--rw-r--r--   0        0        0      204 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev5/samples/unsafe_access.c
--rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev5/samples/ast/function_test_1.c
--rw-r--r--   0        0        0      347 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev5/samples/ast/function_test_2.c
--rw-r--r--   0        0        0      351 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev5/samples/optimize-code/fact_01.c
--rw-r--r--   0        0        0      275 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev5/samples/optimize-code/mult.c
--rw-r--r--   0        0        0      570 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev5/samples/optimize-code/sign_check.c
--rw-r--r--   0        0        0      588 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev5/samples/optimize-code/sign_check_hard.c
--rw-r--r--   0        0        0      791 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev5/scripts/function_equivalence.c
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev5/tests/__init__.py
--rw-r--r--   0        0        0     4229 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev5/tests/test_ai_models.py
--rw-r--r--   0        0        0     2398 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev5/tests/test_base_chat_interface.py
--rw-r--r--   0        0        0      588 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev5/tests/test_command_parser.py
--rw-r--r--   0        0        0     3499 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev5/tests/test_config.py
--rw-r--r--   0        0        0     4655 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev5/tests/test_esbmc_util.py
--rw-r--r--   0        0        0      459 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev5/tests/test_solution.py
--rw-r--r--   0        0        0      576 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev5/tests/test_solution_generator.py
--rw-r--r--   0        0        0     2238 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev5/tests/test_user_chat.py
--rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev5/tests/regtest/__init__.py
--rw-r--r--   0        0        0     1831 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev5/tests/regtest/test_base_chat_interface.py
--rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev5/tests/regtest/_regtest_outputs/test_base_chat_interface.test_push_message_stack.out
--rw-r--r--   0        0        0      558 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev5/tests/regtest/_regtest_outputs/test_base_chat_interface.test_send_message.out
--rw-r--r--   0        0        0  5597855 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev5/tests/samples/esbmc_output/line_test/cartpole_26_safe.c-amalgamation-74.c
--rw-r--r--   0        0        0  1700020 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev5/tests/samples/esbmc_output/line_test/cartpole_48_safe.c-amalgamation-6.c
--rw-r--r--   0        0        0     2115 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev5/tests/samples/esbmc_output/line_test/cartpole_92_safe.c-amalgamation-14.c
--rw-r--r--   0        0        0  1226238 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev5/tests/samples/esbmc_output/line_test/cartpole_95_safe.c-amalgamation-80.c
--rw-r--r--   0        0        0  2808039 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev5/tests/samples/esbmc_output/line_test/robot_5_safe.c-amalgamation-13.c
--rw-r--r--   0        0        0   373267 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev5/tests/samples/esbmc_output/line_test/vdp_1_safe.c-amalgamation-28.c
--rw-r--r--   0        0        0     3173 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev5/.gitignore
--rw-r--r--   0        0        0    34523 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev5/LICENSE
--rw-r--r--   0        0        0     2147 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev5/README.md
--rw-r--r--   0        0        0     1784 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev5/pyproject.toml
--rw-r--r--   0        0        0     3335 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev5/PKG-INFO
+-rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev6/.env.example
+-rw-r--r--   0        0        0    21341 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev6/.pylintrc
+-rw-r--r--   0        0        0      731 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev6/Pipfile
+-rwxr-xr-x   0        0        0       62 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev6/build.sh
+-rwxr-xr-x   0        0        0       81 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev6/clean.sh
+-rw-r--r--   0        0        0     5106 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev6/config.json
+-rwxr-xr-x   0        0        0       41 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev6/esbmc-ai
+-rw-r--r--   0        0        0     6657 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev6/requirements.txt
+-rwxr-xr-x   0        0        0      412 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev6/upload.sh
+-rw-r--r--   0        0        0     1495 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev6/.github/workflows/workflow.yml
+-rw-r--r--   0        0        0      371 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev6/.vscode/c_cpp_properties.json
+-rw-r--r--   0        0        0     1696 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev6/.vscode/launch.json
+-rw-r--r--   0        0        0      105 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev6/.vscode/settings.json
+-rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev6/esbmc_ai/__about__.py
+-rw-r--r--   0        0        0      238 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev6/esbmc_ai/__init__.py
+-rwxr-xr-x   0        0        0    14539 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev6/esbmc_ai/__main__.py
+-rw-r--r--   0        0        0    12079 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev6/esbmc_ai/ai_models.py
+-rw-r--r--   0        0        0      241 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev6/esbmc_ai/api_key_collection.py
+-rw-r--r--   0        0        0     4612 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev6/esbmc_ai/base_chat_interface.py
+-rw-r--r--   0        0        0     1547 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev6/esbmc_ai/chat_response.py
+-rw-r--r--   0        0        0    15371 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev6/esbmc_ai/config.py
+-rw-r--r--   0        0        0     4510 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev6/esbmc_ai/esbmc_util.py
+-rw-r--r--   0        0        0     2487 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev6/esbmc_ai/loading_widget.py
+-rw-r--r--   0        0        0      790 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev6/esbmc_ai/logging.py
+-rw-r--r--   0        0        0      414 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev6/esbmc_ai/msg_bus.py
+-rw-r--r--   0        0        0     1226 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev6/esbmc_ai/optimize_code.py
+-rw-r--r--   0        0        0     5467 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev6/esbmc_ai/solution_generator.py
+-rw-r--r--   0        0        0     2271 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev6/esbmc_ai/user_chat.py
+-rw-r--r--   0        0        0      253 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev6/esbmc_ai/commands/__init__.py
+-rw-r--r--   0        0        0      565 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev6/esbmc_ai/commands/chat_command.py
+-rw-r--r--   0        0        0      458 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev6/esbmc_ai/commands/exit_command.py
+-rw-r--r--   0        0        0     6270 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev6/esbmc_ai/commands/fix_code_command.py
+-rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev6/esbmc_ai/commands/help_command.py
+-rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev6/esbmc_ai/frontend/__init__.py
+-rw-r--r--   0        0        0     1667 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev6/esbmc_ai/frontend/solution.py
+-rw-r--r--   0        0        0    18626 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev6/notebooks/ast.ipynb
+-rw-r--r--   0        0        0      557 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev6/notebooks/samples/typedefs.c
+-rw-r--r--   0        0        0      565 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev6/samples/add_last_unsafe.c
+-rw-r--r--   0        0        0      378 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev6/samples/automatic_arrays.c
+-rw-r--r--   0        0        0      448 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev6/samples/dynamic_mem_alloc.c
+-rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev6/samples/hello_world.c
+-rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev6/samples/mem_leak.c
+-rw-r--r--   0        0        0      272 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev6/samples/optimize_code_test_01.c
+-rw-r--r--   0        0        0      363 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev6/samples/threading.c
+-rw-r--r--   0        0        0      204 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev6/samples/unsafe_access.c
+-rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev6/samples/ast/function_test_1.c
+-rw-r--r--   0        0        0      347 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev6/samples/ast/function_test_2.c
+-rw-r--r--   0        0        0      351 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev6/samples/optimize-code/fact_01.c
+-rw-r--r--   0        0        0      275 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev6/samples/optimize-code/mult.c
+-rw-r--r--   0        0        0      570 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev6/samples/optimize-code/sign_check.c
+-rw-r--r--   0        0        0      588 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev6/samples/optimize-code/sign_check_hard.c
+-rw-r--r--   0        0        0      791 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev6/scripts/function_equivalence.c
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev6/tests/__init__.py
+-rw-r--r--   0        0        0     4229 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev6/tests/test_ai_models.py
+-rw-r--r--   0        0        0     3835 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev6/tests/test_base_chat_interface.py
+-rw-r--r--   0        0        0      588 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev6/tests/test_command_parser.py
+-rw-r--r--   0        0        0     3499 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev6/tests/test_config.py
+-rw-r--r--   0        0        0     4655 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev6/tests/test_esbmc_util.py
+-rw-r--r--   0        0        0      459 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev6/tests/test_solution.py
+-rw-r--r--   0        0        0      576 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev6/tests/test_solution_generator.py
+-rw-r--r--   0        0        0     2238 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev6/tests/test_user_chat.py
+-rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev6/tests/regtest/__init__.py
+-rw-r--r--   0        0        0     1831 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev6/tests/regtest/test_base_chat_interface.py
+-rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev6/tests/regtest/_regtest_outputs/test_base_chat_interface.test_push_message_stack.out
+-rw-r--r--   0        0        0      558 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev6/tests/regtest/_regtest_outputs/test_base_chat_interface.test_send_message.out
+-rw-r--r--   0        0        0  5597855 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev6/tests/samples/esbmc_output/line_test/cartpole_26_safe.c-amalgamation-74.c
+-rw-r--r--   0        0        0  1700020 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev6/tests/samples/esbmc_output/line_test/cartpole_48_safe.c-amalgamation-6.c
+-rw-r--r--   0        0        0     2115 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev6/tests/samples/esbmc_output/line_test/cartpole_92_safe.c-amalgamation-14.c
+-rw-r--r--   0        0        0  1226238 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev6/tests/samples/esbmc_output/line_test/cartpole_95_safe.c-amalgamation-80.c
+-rw-r--r--   0        0        0  2808039 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev6/tests/samples/esbmc_output/line_test/robot_5_safe.c-amalgamation-13.c
+-rw-r--r--   0        0        0   373267 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev6/tests/samples/esbmc_output/line_test/vdp_1_safe.c-amalgamation-28.c
+-rw-r--r--   0        0        0     3173 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev6/.gitignore
+-rw-r--r--   0        0        0    34523 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev6/LICENSE
+-rw-r--r--   0        0        0     2147 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev6/README.md
+-rw-r--r--   0        0        0     1784 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev6/pyproject.toml
+-rw-r--r--   0        0        0     3335 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev6/PKG-INFO
```

### Comparing `esbmc_ai-0.5.0.dev5/.pylintrc` & `esbmc_ai-0.5.0.dev6/.pylintrc`

 * *Files identical despite different names*

### Comparing `esbmc_ai-0.5.0.dev5/Pipfile` & `esbmc_ai-0.5.0.dev6/Pipfile`

 * *Files identical despite different names*

### Comparing `esbmc_ai-0.5.0.dev5/config.json` & `esbmc_ai-0.5.0.dev6/config.json`

 * *Files identical despite different names*

### Comparing `esbmc_ai-0.5.0.dev5/requirements.txt` & `esbmc_ai-0.5.0.dev6/requirements.txt`

 * *Files identical despite different names*

### Comparing `esbmc_ai-0.5.0.dev5/.github/workflows/workflow.yml` & `esbmc_ai-0.5.0.dev6/.github/workflows/workflow.yml`

 * *Files identical despite different names*

### Comparing `esbmc_ai-0.5.0.dev5/.vscode/launch.json` & `esbmc_ai-0.5.0.dev6/.vscode/launch.json`

 * *Files identical despite different names*

### Comparing `esbmc_ai-0.5.0.dev5/esbmc_ai/__main__.py` & `esbmc_ai-0.5.0.dev6/esbmc_ai/__main__.py`

 * *Files identical despite different names*

### Comparing `esbmc_ai-0.5.0.dev5/esbmc_ai/ai_models.py` & `esbmc_ai-0.5.0.dev6/esbmc_ai/ai_models.py`

 * *Files identical despite different names*

### Comparing `esbmc_ai-0.5.0.dev5/esbmc_ai/chat_response.py` & `esbmc_ai-0.5.0.dev6/esbmc_ai/chat_response.py`

 * *Files identical despite different names*

### Comparing `esbmc_ai-0.5.0.dev5/esbmc_ai/config.py` & `esbmc_ai-0.5.0.dev6/esbmc_ai/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from pathlib import Path
 from dotenv import load_dotenv, find_dotenv
 
 from typing import Any, NamedTuple, Optional, Union, Sequence
 from dataclasses import dataclass
 from langchain.schema import BaseMessage
 
-from .logging import *
+from esbmc_ai.logging import printv, set_verbose
 from .ai_models import *
 from .api_key_collection import APIKeyCollection
 from .chat_response import json_to_base_messages
 
 
 api_keys: APIKeyCollection
```

### Comparing `esbmc_ai-0.5.0.dev5/esbmc_ai/esbmc_util.py` & `esbmc_ai-0.5.0.dev6/esbmc_ai/esbmc_util.py`

 * *Files identical despite different names*

### Comparing `esbmc_ai-0.5.0.dev5/esbmc_ai/loading_widget.py` & `esbmc_ai-0.5.0.dev6/esbmc_ai/loading_widget.py`

 * *Files identical despite different names*

### Comparing `esbmc_ai-0.5.0.dev5/esbmc_ai/logging.py` & `esbmc_ai-0.5.0.dev6/esbmc_ai/logging.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,40 +1,43 @@
 # Author: Yiannis Charalambous
 
 """Logging module for verbose printing."""
 
 from os import get_terminal_size
-import esbmc_ai.config as config
 
-verbose: int = 0
+_verbose: int = 0
+
+
+def get_verbose_level() -> int:
+    return _verbose
 
 
 def set_verbose(level: int) -> None:
     """Sets the verbosity level."""
-    global verbose
-    verbose = level
+    global _verbose
+    _verbose = level
 
 
 def printv(m) -> None:
     """Level 1 verbose printing."""
-    if verbose > 0:
+    if _verbose > 0:
         print(m)
 
 
 def printvv(m) -> None:
     """Level 2 verbose printing."""
-    if verbose > 1:
+    if _verbose > 1:
         print(m)
 
 
 def printvvv(m) -> None:
     """Level 3 verbose printing."""
-    if verbose > 2:
+    if _verbose > 2:
         print(m)
 
 
 def print_horizontal_line(verbosity: int) -> None:
-    if verbosity >= config.verbose:
+    if verbosity >= _verbose:
         try:
             printvv("-" * get_terminal_size().columns)
         except OSError:
             pass
```

### Comparing `esbmc_ai-0.5.0.dev5/esbmc_ai/optimize_code.py` & `esbmc_ai-0.5.0.dev6/esbmc_ai/optimize_code.py`

 * *Files identical despite different names*

### Comparing `esbmc_ai-0.5.0.dev5/esbmc_ai/solution_generator.py` & `esbmc_ai-0.5.0.dev6/esbmc_ai/solution_generator.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 # Author: Yiannis Charalambous 2023
 
+from re import S
 from typing import Optional
 from typing_extensions import override
 from langchain.base_language import BaseLanguageModel
-from langchain.schema import BaseMessage
+from langchain.schema import BaseMessage, HumanMessage
 
 from esbmc_ai.chat_response import ChatResponse, FinishReason
 from esbmc_ai.config import ChatPromptSettings, DynamicAIModelAgent
 from esbmc_ai.frontend.solution import apply_line_patch
 
 from .ai_models import AIModel
 from .base_chat_interface import BaseChatInterface
@@ -82,22 +83,25 @@
         self.esbmc_output = get_esbmc_output_formatted(
             esbmc_output_type=self.esbmc_output_type,
             esbmc_output=esbmc_output,
         )
 
         self.source_code_format: str = source_code_format
         self.source_code_raw: str = source_code
-        self.source_code = get_source_code_formatted(
+
+        source_code_formatted: str = get_source_code_formatted(
             source_code_format=self.source_code_format,
             source_code=self.source_code_raw,
             esbmc_output=self.esbmc_output,
         )
 
-        self.set_template_value("source_code", self.source_code)
-        self.set_template_value("esbmc_output", self.esbmc_output)
+        self.apply_template_value(
+            source_code=source_code_formatted,
+            esbmc_output=self.esbmc_output,
+        )
 
     @override
     def compress_message_stack(self) -> None:
         # Resets the conversation - cannot summarize code
         self.messages: list[BaseMessage] = []
 
     @classmethod
```

### Comparing `esbmc_ai-0.5.0.dev5/esbmc_ai/user_chat.py` & `esbmc_ai-0.5.0.dev6/esbmc_ai/user_chat.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 # Author: Yiannis Charalambous 2023
 
 from typing_extensions import override
 
 from langchain.base_language import BaseLanguageModel
-from langchain.memory import ConversationSummaryMemory, ChatMessageHistory
-from langchain.schema import BaseMessage, PromptValue, SystemMessage
+from langchain.memory import ConversationSummaryMemory
+from langchain_community.chat_message_histories import ChatMessageHistory
+
+from langchain.schema import BaseMessage, SystemMessage
 
 from esbmc_ai.config import AIAgentConversation, ChatPromptSettings
 
 from .ai_models import AIModel
 from .base_chat_interface import BaseChatInterface
 
 
@@ -32,41 +34,24 @@
 
         # Store source code and esbmc output in order to substitute it into the message stack.
         self.source_code: str = source_code
         self.esbmc_output: str = esbmc_output
         # The messsages for setting a new solution to the source code.
         self.set_solution_messages = set_solution_messages
 
-        self.set_template_value("source_code", self.source_code)
-        self.set_template_value("esbmc_output", self.esbmc_output)
+        self.apply_template_value(source_code=self.source_code)
+        self.apply_template_value(esbmc_output=self.esbmc_output)
 
     def set_solution(self, source_code: str) -> None:
         """Sets the solution to the problem ESBMC reported, this will inform the AI."""
 
-        self.set_template_value("source_code_solution", source_code)
-
-        message_prompts: PromptValue = self.ai_model.apply_chat_template(
-            messages=self.set_solution_messages.messages,
-            **self.template_values,
-        )
-
-        for message in message_prompts.to_messages():
-            self.push_to_message_stack(message)
-
-    def set_optimized_solution(self, source_code: str) -> None:
-        # NOTE Here we use the same system message as `set_solution`.
-        self.set_template_value("source_code_solution", source_code)
-
-        message_prompts: PromptValue = self.ai_model.apply_chat_template(
-            messages=self.set_solution_messages.messages,
-            **self.template_values,
-        )
+        for msg in self.set_solution_messages.messages:
+            self.push_to_message_stack(msg)
 
-        for message in message_prompts.to_messages():
-            self.push_to_message_stack(message)
+        self.apply_template_value(source_code_solution=source_code)
 
     @override
     def compress_message_stack(self) -> None:
         """Uses ConversationSummaryMemory from Langchain to summarize the conversation of all the non-protected
         messages into one summary message which is added into the conversation as a SystemMessage.
         """
```

### Comparing `esbmc_ai-0.5.0.dev5/esbmc_ai/commands/chat_command.py` & `esbmc_ai-0.5.0.dev6/esbmc_ai/commands/chat_command.py`

 * *Files identical despite different names*

### Comparing `esbmc_ai-0.5.0.dev5/esbmc_ai/commands/fix_code_command.py` & `esbmc_ai-0.5.0.dev6/esbmc_ai/commands/fix_code_command.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,19 +30,20 @@
             help_message="Generates a solution for this code, and reevaluates it with ESBMC.",
         )
         self.anim = create_loading_widget()
 
     @override
     def execute(self, **kwargs: Any) -> Tuple[bool, str]:
         def print_raw_conversation() -> None:
-            print("Note: F-String substitution is not available with -r...")
-            messages: list[str] = [
-                f"{msg.type}: {msg.content}" for msg in solution_generator.messages
-            ]
+            print("Notice: Printing raw conversation...")
+            all_messages = solution_generator._system_messages.copy()
+            all_messages.extend(solution_generator.messages.copy())
+            messages: list[str] = [f"{msg.type}: {msg.content}" for msg in all_messages]
             print("\n" + "\n\n".join(messages))
+            print("Notice: End of conversation")
 
         file_name: str = kwargs["file_name"]
         source_code: str = kwargs["source_code"]
         esbmc_output: str = kwargs["esbmc_output"]
 
         # Parse the esbmc output here and determine what "Scenario" to use.
         scenario: str = esbmc_get_error_type(esbmc_output)
```

### Comparing `esbmc_ai-0.5.0.dev5/esbmc_ai/commands/help_command.py` & `esbmc_ai-0.5.0.dev6/esbmc_ai/commands/help_command.py`

 * *Files identical despite different names*

### Comparing `esbmc_ai-0.5.0.dev5/esbmc_ai/frontend/solution.py` & `esbmc_ai-0.5.0.dev6/esbmc_ai/frontend/solution.py`

 * *Files identical despite different names*

### Comparing `esbmc_ai-0.5.0.dev5/notebooks/ast.ipynb` & `esbmc_ai-0.5.0.dev6/notebooks/ast.ipynb`

 * *Files identical despite different names*

### Comparing `esbmc_ai-0.5.0.dev5/notebooks/samples/typedefs.c` & `esbmc_ai-0.5.0.dev6/notebooks/samples/typedefs.c`

 * *Files identical despite different names*

### Comparing `esbmc_ai-0.5.0.dev5/samples/add_last_unsafe.c` & `esbmc_ai-0.5.0.dev6/samples/add_last_unsafe.c`

 * *Files identical despite different names*

### Comparing `esbmc_ai-0.5.0.dev5/samples/optimize-code/sign_check.c` & `esbmc_ai-0.5.0.dev6/samples/optimize-code/sign_check.c`

 * *Files identical despite different names*

### Comparing `esbmc_ai-0.5.0.dev5/samples/optimize-code/sign_check_hard.c` & `esbmc_ai-0.5.0.dev6/samples/optimize-code/sign_check_hard.c`

 * *Files identical despite different names*

### Comparing `esbmc_ai-0.5.0.dev5/scripts/function_equivalence.c` & `esbmc_ai-0.5.0.dev6/scripts/function_equivalence.c`

 * *Files identical despite different names*

### Comparing `esbmc_ai-0.5.0.dev5/tests/test_ai_models.py` & `esbmc_ai-0.5.0.dev6/tests/test_ai_models.py`

 * *Files identical despite different names*

### Comparing `esbmc_ai-0.5.0.dev5/tests/test_base_chat_interface.py` & `esbmc_ai-0.5.0.dev6/tests/regtest/test_base_chat_interface.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,81 +1,69 @@
 # Author: Yiannis Charalambous
 
 import pytest
 
 from langchain.llms.fake import FakeListLLM
-from langchain.schema import AIMessage, BaseMessage, HumanMessage, SystemMessage
+from langchain.schema import BaseMessage, HumanMessage, AIMessage, SystemMessage
+
 from esbmc_ai.ai_models import AIModel
-from esbmc_ai.base_chat_interface import BaseChatInterface
 from esbmc_ai.chat_response import ChatResponse
+from esbmc_ai.base_chat_interface import BaseChatInterface
 from esbmc_ai.config import AIAgentConversation, ChatPromptSettings
 
 
-@pytest.fixture(scope="module")
+@pytest.fixture
 def setup():
+    responses: list[str] = ["OK 1", "OK 2", "OK 3"]
+    llm: FakeListLLM = FakeListLLM(responses=responses)
+
     ai_model: AIModel = AIModel("test", 1024)
 
-    system_messages: list[BaseMessage] = [
-        SystemMessage(content="First system message"),
+    system_messages = [
+        SystemMessage(content="System message"),
         AIMessage(content="OK"),
     ]
 
-    return ai_model, system_messages
-
-
-def test_push_message_stack(setup) -> None:
-    llm: FakeListLLM = FakeListLLM(responses=[])
-
-    ai_model, system_messages = setup
-
     chat: BaseChatInterface = BaseChatInterface(
         ai_model_agent=ChatPromptSettings(
-            AIAgentConversation.from_seq(system_messages),
             initial_prompt="",
+            system_messages=AIAgentConversation.from_seq(system_messages),
             temperature=1.0,
         ),
         ai_model=ai_model,
         llm=llm,
     )
 
-    assert chat.ai_model_agent.system_messages.messages == tuple(system_messages)
+    return chat
+
+
+def test_push_message_stack(regtest, setup) -> None:
+    chat = setup
 
     messages: list[BaseMessage] = [
         AIMessage(content="Test 1"),
         HumanMessage(content="Test 2"),
         SystemMessage(content="Test 3"),
     ]
 
-    chat.push_to_message_stack(message=messages[0])
-    chat.push_to_message_stack(message=messages[1])
-    chat.push_to_message_stack(message=messages[2])
+    chat.push_to_message_stack(messages[0])
+    chat.push_to_message_stack(messages[1])
+    chat.push_to_message_stack(messages[2])
 
-    assert chat.messages[0] == messages[0]
-    assert chat.messages[1] == messages[1]
-    assert chat.messages[2] == messages[2]
+    with regtest:
+        print(chat.ai_model_agent.system_messages.messages)
+        print(chat.messages)
 
 
-def test_send_message(setup) -> None:
-    responses: list[str] = ["OK 1", "OK 2", "OK 3"]
-    llm: FakeListLLM = FakeListLLM(responses=responses)
-
-    ai_model, system_messages = setup
-
-    chat: BaseChatInterface = BaseChatInterface(
-        ai_model_agent=ChatPromptSettings(
-            AIAgentConversation.from_seq(system_messages),
-            initial_prompt="",
-            temperature=1.0,
-        ),
-        ai_model=ai_model,
-        llm=llm,
-    )
+def test_send_message(regtest, setup) -> None:
+    chat = setup
 
     chat_responses: list[ChatResponse] = [
         chat.send_message("Test 1"),
         chat.send_message("Test 2"),
         chat.send_message("Test 3"),
     ]
 
-    assert chat_responses[0].message.content == responses[0]
-    assert chat_responses[1].message.content == responses[1]
-    assert chat_responses[2].message.content == responses[2]
+    with regtest:
+        print(chat.ai_model_agent.system_messages.messages)
+        print(chat.messages)
+        print(chat_responses)
```

### Comparing `esbmc_ai-0.5.0.dev5/tests/test_command_parser.py` & `esbmc_ai-0.5.0.dev6/tests/test_command_parser.py`

 * *Files identical despite different names*

### Comparing `esbmc_ai-0.5.0.dev5/tests/test_config.py` & `esbmc_ai-0.5.0.dev6/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `esbmc_ai-0.5.0.dev5/tests/test_esbmc_util.py` & `esbmc_ai-0.5.0.dev6/tests/test_esbmc_util.py`

 * *Files identical despite different names*

### Comparing `esbmc_ai-0.5.0.dev5/tests/test_solution_generator.py` & `esbmc_ai-0.5.0.dev6/tests/test_solution_generator.py`

 * *Files identical despite different names*

### Comparing `esbmc_ai-0.5.0.dev5/tests/test_user_chat.py` & `esbmc_ai-0.5.0.dev6/tests/test_user_chat.py`

 * *Files identical despite different names*

### Comparing `esbmc_ai-0.5.0.dev5/tests/regtest/_regtest_outputs/test_base_chat_interface.test_send_message.out` & `esbmc_ai-0.5.0.dev6/tests/regtest/_regtest_outputs/test_base_chat_interface.test_send_message.out`

 * *Files identical despite different names*

### Comparing `esbmc_ai-0.5.0.dev5/tests/samples/esbmc_output/line_test/cartpole_26_safe.c-amalgamation-74.c` & `esbmc_ai-0.5.0.dev6/tests/samples/esbmc_output/line_test/cartpole_26_safe.c-amalgamation-74.c`

 * *Files identical despite different names*

### Comparing `esbmc_ai-0.5.0.dev5/tests/samples/esbmc_output/line_test/cartpole_48_safe.c-amalgamation-6.c` & `esbmc_ai-0.5.0.dev6/tests/samples/esbmc_output/line_test/cartpole_48_safe.c-amalgamation-6.c`

 * *Files identical despite different names*

### Comparing `esbmc_ai-0.5.0.dev5/tests/samples/esbmc_output/line_test/cartpole_92_safe.c-amalgamation-14.c` & `esbmc_ai-0.5.0.dev6/tests/samples/esbmc_output/line_test/cartpole_92_safe.c-amalgamation-14.c`

 * *Files identical despite different names*

### Comparing `esbmc_ai-0.5.0.dev5/tests/samples/esbmc_output/line_test/cartpole_95_safe.c-amalgamation-80.c` & `esbmc_ai-0.5.0.dev6/tests/samples/esbmc_output/line_test/cartpole_95_safe.c-amalgamation-80.c`

 * *Files identical despite different names*

### Comparing `esbmc_ai-0.5.0.dev5/tests/samples/esbmc_output/line_test/robot_5_safe.c-amalgamation-13.c` & `esbmc_ai-0.5.0.dev6/tests/samples/esbmc_output/line_test/robot_5_safe.c-amalgamation-13.c`

 * *Files identical despite different names*

### Comparing `esbmc_ai-0.5.0.dev5/tests/samples/esbmc_output/line_test/vdp_1_safe.c-amalgamation-28.c` & `esbmc_ai-0.5.0.dev6/tests/samples/esbmc_output/line_test/vdp_1_safe.c-amalgamation-28.c`

 * *Files identical despite different names*

### Comparing `esbmc_ai-0.5.0.dev5/.gitignore` & `esbmc_ai-0.5.0.dev6/.gitignore`

 * *Files identical despite different names*

### Comparing `esbmc_ai-0.5.0.dev5/LICENSE` & `esbmc_ai-0.5.0.dev6/LICENSE`

 * *Files identical despite different names*

### Comparing `esbmc_ai-0.5.0.dev5/README.md` & `esbmc_ai-0.5.0.dev6/README.md`

 * *Files identical despite different names*

### Comparing `esbmc_ai-0.5.0.dev5/pyproject.toml` & `esbmc_ai-0.5.0.dev6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `esbmc_ai-0.5.0.dev5/PKG-INFO` & `esbmc_ai-0.5.0.dev6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: esbmc_ai
-Version: 0.5.0.dev5
+Version: 0.5.0.dev6
 Summary: LLM driven development and automatic repair kit.
 Project-URL: Homepage, https://github.com/Yiannis128/esbmc-ai
 Project-URL: Source Code, https://github.com/Yiannis128/esbmc-ai
 Project-URL: Documentation, https://github.com/Yiannis128/esbmc-ai/wiki
 Project-URL: Issues, https://github.com/Yiannis128/esbmc-ai/issues
 Author-email: Yiannis Charalambous <yiannis128@hotmail.com>
 License-File: LICENSE
```

