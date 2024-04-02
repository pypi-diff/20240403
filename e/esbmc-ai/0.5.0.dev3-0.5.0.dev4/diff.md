# Comparing `tmp/esbmc_ai-0.5.0.dev3.tar.gz` & `tmp/esbmc_ai-0.5.0.dev4.tar.gz`

## Comparing `esbmc_ai-0.5.0.dev3.tar` & `esbmc_ai-0.5.0.dev4.tar`

### file list

```diff
@@ -1,76 +1,76 @@
--rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev3/.env.example
--rw-r--r--   0        0        0    21341 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev3/.pylintrc
--rw-r--r--   0        0        0      731 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev3/Pipfile
--rwxr-xr-x   0        0        0       62 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev3/build.sh
--rwxr-xr-x   0        0        0       81 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev3/clean.sh
--rw-r--r--   0        0        0     5106 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev3/config.json
--rwxr-xr-x   0        0        0       41 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev3/esbmc-ai
--rw-r--r--   0        0        0     6657 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev3/requirements.txt
--rwxr-xr-x   0        0        0      412 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev3/upload.sh
--rw-r--r--   0        0        0     1495 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev3/.github/workflows/workflow.yml
--rw-r--r--   0        0        0      371 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev3/.vscode/c_cpp_properties.json
--rw-r--r--   0        0        0     1696 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev3/.vscode/launch.json
--rw-r--r--   0        0        0      105 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev3/.vscode/settings.json
--rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev3/esbmc_ai/__about__.py
--rw-r--r--   0        0        0      238 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev3/esbmc_ai/__init__.py
--rwxr-xr-x   0        0        0    14558 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev3/esbmc_ai/__main__.py
--rw-r--r--   0        0        0    12079 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev3/esbmc_ai/ai_models.py
--rw-r--r--   0        0        0      241 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev3/esbmc_ai/api_key_collection.py
--rw-r--r--   0        0        0     3347 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev3/esbmc_ai/base_chat_interface.py
--rw-r--r--   0        0        0     1547 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev3/esbmc_ai/chat_response.py
--rw-r--r--   0        0        0    15345 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev3/esbmc_ai/config.py
--rw-r--r--   0        0        0     4510 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev3/esbmc_ai/esbmc_util.py
--rw-r--r--   0        0        0     2487 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev3/esbmc_ai/loading_widget.py
--rw-r--r--   0        0        0      504 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev3/esbmc_ai/logging.py
--rw-r--r--   0        0        0      414 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev3/esbmc_ai/msg_bus.py
--rw-r--r--   0        0        0     1226 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev3/esbmc_ai/optimize_code.py
--rw-r--r--   0        0        0     5421 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev3/esbmc_ai/solution_generator.py
--rw-r--r--   0        0        0     2899 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev3/esbmc_ai/user_chat.py
--rw-r--r--   0        0        0      253 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev3/esbmc_ai/commands/__init__.py
--rw-r--r--   0        0        0      565 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev3/esbmc_ai/commands/chat_command.py
--rw-r--r--   0        0        0      458 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev3/esbmc_ai/commands/exit_command.py
--rw-r--r--   0        0        0     6228 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev3/esbmc_ai/commands/fix_code_command.py
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev3/esbmc_ai/commands/help_command.py
--rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev3/esbmc_ai/frontend/__init__.py
--rw-r--r--   0        0        0     1667 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev3/esbmc_ai/frontend/solution.py
--rw-r--r--   0        0        0    18626 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev3/notebooks/ast.ipynb
--rw-r--r--   0        0        0      557 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev3/notebooks/samples/typedefs.c
--rw-r--r--   0        0        0      565 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev3/samples/add_last_unsafe.c
--rw-r--r--   0        0        0      378 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev3/samples/automatic_arrays.c
--rw-r--r--   0        0        0      448 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev3/samples/dynamic_mem_alloc.c
--rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev3/samples/hello_world.c
--rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev3/samples/mem_leak.c
--rw-r--r--   0        0        0      272 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev3/samples/optimize_code_test_01.c
--rw-r--r--   0        0        0      363 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev3/samples/threading.c
--rw-r--r--   0        0        0      204 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev3/samples/unsafe_access.c
--rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev3/samples/ast/function_test_1.c
--rw-r--r--   0        0        0      347 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev3/samples/ast/function_test_2.c
--rw-r--r--   0        0        0      351 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev3/samples/optimize-code/fact_01.c
--rw-r--r--   0        0        0      275 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev3/samples/optimize-code/mult.c
--rw-r--r--   0        0        0      570 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev3/samples/optimize-code/sign_check.c
--rw-r--r--   0        0        0      588 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev3/samples/optimize-code/sign_check_hard.c
--rw-r--r--   0        0        0      791 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev3/scripts/function_equivalence.c
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev3/tests/__init__.py
--rw-r--r--   0        0        0     4229 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev3/tests/test_ai_models.py
--rw-r--r--   0        0        0     2398 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev3/tests/test_base_chat_interface.py
--rw-r--r--   0        0        0      588 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev3/tests/test_command_parser.py
--rw-r--r--   0        0        0     3499 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev3/tests/test_config.py
--rw-r--r--   0        0        0     4655 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev3/tests/test_esbmc_util.py
--rw-r--r--   0        0        0      459 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev3/tests/test_solution.py
--rw-r--r--   0        0        0      576 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev3/tests/test_solution_generator.py
--rw-r--r--   0        0        0     2238 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev3/tests/test_user_chat.py
--rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev3/tests/regtest/__init__.py
--rw-r--r--   0        0        0     1831 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev3/tests/regtest/test_base_chat_interface.py
--rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev3/tests/regtest/_regtest_outputs/test_base_chat_interface.test_push_message_stack.out
--rw-r--r--   0        0        0      558 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev3/tests/regtest/_regtest_outputs/test_base_chat_interface.test_send_message.out
--rw-r--r--   0        0        0  5597855 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev3/tests/samples/esbmc_output/line_test/cartpole_26_safe.c-amalgamation-74.c
--rw-r--r--   0        0        0  1700020 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev3/tests/samples/esbmc_output/line_test/cartpole_48_safe.c-amalgamation-6.c
--rw-r--r--   0        0        0     2115 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev3/tests/samples/esbmc_output/line_test/cartpole_92_safe.c-amalgamation-14.c
--rw-r--r--   0        0        0  1226238 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev3/tests/samples/esbmc_output/line_test/cartpole_95_safe.c-amalgamation-80.c
--rw-r--r--   0        0        0  2808039 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev3/tests/samples/esbmc_output/line_test/robot_5_safe.c-amalgamation-13.c
--rw-r--r--   0        0        0   373267 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev3/tests/samples/esbmc_output/line_test/vdp_1_safe.c-amalgamation-28.c
--rw-r--r--   0        0        0     3173 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev3/.gitignore
--rw-r--r--   0        0        0    34523 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev3/LICENSE
--rw-r--r--   0        0        0     2147 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev3/README.md
--rw-r--r--   0        0        0     1784 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev3/pyproject.toml
--rw-r--r--   0        0        0     3335 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev3/PKG-INFO
+-rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev4/.env.example
+-rw-r--r--   0        0        0    21341 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev4/.pylintrc
+-rw-r--r--   0        0        0      731 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev4/Pipfile
+-rwxr-xr-x   0        0        0       62 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev4/build.sh
+-rwxr-xr-x   0        0        0       81 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev4/clean.sh
+-rw-r--r--   0        0        0     5106 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev4/config.json
+-rwxr-xr-x   0        0        0       41 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev4/esbmc-ai
+-rw-r--r--   0        0        0     6657 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev4/requirements.txt
+-rwxr-xr-x   0        0        0      412 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev4/upload.sh
+-rw-r--r--   0        0        0     1495 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev4/.github/workflows/workflow.yml
+-rw-r--r--   0        0        0      371 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev4/.vscode/c_cpp_properties.json
+-rw-r--r--   0        0        0     1696 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev4/.vscode/launch.json
+-rw-r--r--   0        0        0      105 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev4/.vscode/settings.json
+-rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev4/esbmc_ai/__about__.py
+-rw-r--r--   0        0        0      238 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev4/esbmc_ai/__init__.py
+-rwxr-xr-x   0        0        0    14539 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev4/esbmc_ai/__main__.py
+-rw-r--r--   0        0        0    12079 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev4/esbmc_ai/ai_models.py
+-rw-r--r--   0        0        0      241 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev4/esbmc_ai/api_key_collection.py
+-rw-r--r--   0        0        0     3347 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev4/esbmc_ai/base_chat_interface.py
+-rw-r--r--   0        0        0     1547 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev4/esbmc_ai/chat_response.py
+-rw-r--r--   0        0        0    15345 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev4/esbmc_ai/config.py
+-rw-r--r--   0        0        0     4510 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev4/esbmc_ai/esbmc_util.py
+-rw-r--r--   0        0        0     2487 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev4/esbmc_ai/loading_widget.py
+-rw-r--r--   0        0        0      769 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev4/esbmc_ai/logging.py
+-rw-r--r--   0        0        0      414 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev4/esbmc_ai/msg_bus.py
+-rw-r--r--   0        0        0     1226 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev4/esbmc_ai/optimize_code.py
+-rw-r--r--   0        0        0     5421 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev4/esbmc_ai/solution_generator.py
+-rw-r--r--   0        0        0     2899 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev4/esbmc_ai/user_chat.py
+-rw-r--r--   0        0        0      253 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev4/esbmc_ai/commands/__init__.py
+-rw-r--r--   0        0        0      565 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev4/esbmc_ai/commands/chat_command.py
+-rw-r--r--   0        0        0      458 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev4/esbmc_ai/commands/exit_command.py
+-rw-r--r--   0        0        0     6179 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev4/esbmc_ai/commands/fix_code_command.py
+-rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev4/esbmc_ai/commands/help_command.py
+-rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev4/esbmc_ai/frontend/__init__.py
+-rw-r--r--   0        0        0     1667 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev4/esbmc_ai/frontend/solution.py
+-rw-r--r--   0        0        0    18626 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev4/notebooks/ast.ipynb
+-rw-r--r--   0        0        0      557 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev4/notebooks/samples/typedefs.c
+-rw-r--r--   0        0        0      565 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev4/samples/add_last_unsafe.c
+-rw-r--r--   0        0        0      378 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev4/samples/automatic_arrays.c
+-rw-r--r--   0        0        0      448 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev4/samples/dynamic_mem_alloc.c
+-rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev4/samples/hello_world.c
+-rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev4/samples/mem_leak.c
+-rw-r--r--   0        0        0      272 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev4/samples/optimize_code_test_01.c
+-rw-r--r--   0        0        0      363 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev4/samples/threading.c
+-rw-r--r--   0        0        0      204 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev4/samples/unsafe_access.c
+-rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev4/samples/ast/function_test_1.c
+-rw-r--r--   0        0        0      347 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev4/samples/ast/function_test_2.c
+-rw-r--r--   0        0        0      351 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev4/samples/optimize-code/fact_01.c
+-rw-r--r--   0        0        0      275 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev4/samples/optimize-code/mult.c
+-rw-r--r--   0        0        0      570 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev4/samples/optimize-code/sign_check.c
+-rw-r--r--   0        0        0      588 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev4/samples/optimize-code/sign_check_hard.c
+-rw-r--r--   0        0        0      791 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev4/scripts/function_equivalence.c
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev4/tests/__init__.py
+-rw-r--r--   0        0        0     4229 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev4/tests/test_ai_models.py
+-rw-r--r--   0        0        0     2398 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev4/tests/test_base_chat_interface.py
+-rw-r--r--   0        0        0      588 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev4/tests/test_command_parser.py
+-rw-r--r--   0        0        0     3499 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev4/tests/test_config.py
+-rw-r--r--   0        0        0     4655 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev4/tests/test_esbmc_util.py
+-rw-r--r--   0        0        0      459 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev4/tests/test_solution.py
+-rw-r--r--   0        0        0      576 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev4/tests/test_solution_generator.py
+-rw-r--r--   0        0        0     2238 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev4/tests/test_user_chat.py
+-rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev4/tests/regtest/__init__.py
+-rw-r--r--   0        0        0     1831 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev4/tests/regtest/test_base_chat_interface.py
+-rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev4/tests/regtest/_regtest_outputs/test_base_chat_interface.test_push_message_stack.out
+-rw-r--r--   0        0        0      558 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev4/tests/regtest/_regtest_outputs/test_base_chat_interface.test_send_message.out
+-rw-r--r--   0        0        0  5597855 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev4/tests/samples/esbmc_output/line_test/cartpole_26_safe.c-amalgamation-74.c
+-rw-r--r--   0        0        0  1700020 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev4/tests/samples/esbmc_output/line_test/cartpole_48_safe.c-amalgamation-6.c
+-rw-r--r--   0        0        0     2115 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev4/tests/samples/esbmc_output/line_test/cartpole_92_safe.c-amalgamation-14.c
+-rw-r--r--   0        0        0  1226238 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev4/tests/samples/esbmc_output/line_test/cartpole_95_safe.c-amalgamation-80.c
+-rw-r--r--   0        0        0  2808039 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev4/tests/samples/esbmc_output/line_test/robot_5_safe.c-amalgamation-13.c
+-rw-r--r--   0        0        0   373267 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev4/tests/samples/esbmc_output/line_test/vdp_1_safe.c-amalgamation-28.c
+-rw-r--r--   0        0        0     3173 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev4/.gitignore
+-rw-r--r--   0        0        0    34523 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev4/LICENSE
+-rw-r--r--   0        0        0     2147 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev4/README.md
+-rw-r--r--   0        0        0     1784 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev4/pyproject.toml
+-rw-r--r--   0        0        0     3335 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev4/PKG-INFO
```

### Comparing `esbmc_ai-0.5.0.dev3/.pylintrc` & `esbmc_ai-0.5.0.dev4/.pylintrc`

 * *Files identical despite different names*

### Comparing `esbmc_ai-0.5.0.dev3/Pipfile` & `esbmc_ai-0.5.0.dev4/Pipfile`

 * *Files identical despite different names*

### Comparing `esbmc_ai-0.5.0.dev3/config.json` & `esbmc_ai-0.5.0.dev4/config.json`

 * *Files identical despite different names*

### Comparing `esbmc_ai-0.5.0.dev3/requirements.txt` & `esbmc_ai-0.5.0.dev4/requirements.txt`

 * *Files identical despite different names*

### Comparing `esbmc_ai-0.5.0.dev3/.github/workflows/workflow.yml` & `esbmc_ai-0.5.0.dev4/.github/workflows/workflow.yml`

 * *Files identical despite different names*

### Comparing `esbmc_ai-0.5.0.dev3/.vscode/launch.json` & `esbmc_ai-0.5.0.dev4/.vscode/launch.json`

 * *Files identical despite different names*

### Comparing `esbmc_ai-0.5.0.dev3/esbmc_ai/__main__.py` & `esbmc_ai-0.5.0.dev4/esbmc_ai/__main__.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,15 +27,15 @@
     FixCodeCommand,
     HelpCommand,
     ExitCommand,
 )
 
 from esbmc_ai.loading_widget import LoadingWidget, create_loading_widget
 from esbmc_ai.user_chat import UserChat
-from esbmc_ai.logging import printv, printvv
+from esbmc_ai.logging import print_horizontal_line, printv, printvv
 from esbmc_ai.esbmc_util import esbmc
 from esbmc_ai.chat_response import FinishReason, ChatResponse
 from esbmc_ai.ai_models import _ai_model_names
 
 
 commands: list[ChatCommand] = []
 command_names: list[str]
@@ -283,17 +283,17 @@
         path=get_main_source_file_path(),
         esbmc_params=config.esbmc_params,
         timeout=config.verifier_timeout,
     )
     anim.stop()
 
     # Print verbose lvl 2
-    printvv("-" * os.get_terminal_size().columns)
+    print_horizontal_line(2)
     printvv(esbmc_output)
-    printvv("-" * os.get_terminal_size().columns)
+    print_horizontal_line(2)
 
     # ESBMC will output 0 for verification success and 1 for verification
     # failed, if anything else gets thrown, it's an ESBMC error.
     if not config.allow_successful and exit_code == 0:
         print("Success!")
         print(esbmc_output)
         sys.exit(0)
```

### Comparing `esbmc_ai-0.5.0.dev3/esbmc_ai/ai_models.py` & `esbmc_ai-0.5.0.dev4/esbmc_ai/ai_models.py`

 * *Files identical despite different names*

### Comparing `esbmc_ai-0.5.0.dev3/esbmc_ai/base_chat_interface.py` & `esbmc_ai-0.5.0.dev4/esbmc_ai/base_chat_interface.py`

 * *Files identical despite different names*

### Comparing `esbmc_ai-0.5.0.dev3/esbmc_ai/chat_response.py` & `esbmc_ai-0.5.0.dev4/esbmc_ai/chat_response.py`

 * *Files identical despite different names*

### Comparing `esbmc_ai-0.5.0.dev3/esbmc_ai/config.py` & `esbmc_ai-0.5.0.dev4/esbmc_ai/config.py`

 * *Files identical despite different names*

### Comparing `esbmc_ai-0.5.0.dev3/esbmc_ai/esbmc_util.py` & `esbmc_ai-0.5.0.dev4/esbmc_ai/esbmc_util.py`

 * *Files identical despite different names*

### Comparing `esbmc_ai-0.5.0.dev3/esbmc_ai/loading_widget.py` & `esbmc_ai-0.5.0.dev4/esbmc_ai/loading_widget.py`

 * *Files identical despite different names*

### Comparing `esbmc_ai-0.5.0.dev3/esbmc_ai/optimize_code.py` & `esbmc_ai-0.5.0.dev4/esbmc_ai/optimize_code.py`

 * *Files identical despite different names*

### Comparing `esbmc_ai-0.5.0.dev3/esbmc_ai/solution_generator.py` & `esbmc_ai-0.5.0.dev4/esbmc_ai/solution_generator.py`

 * *Files identical despite different names*

### Comparing `esbmc_ai-0.5.0.dev3/esbmc_ai/user_chat.py` & `esbmc_ai-0.5.0.dev4/esbmc_ai/user_chat.py`

 * *Files identical despite different names*

### Comparing `esbmc_ai-0.5.0.dev3/esbmc_ai/commands/chat_command.py` & `esbmc_ai-0.5.0.dev4/esbmc_ai/commands/chat_command.py`

 * *Files identical despite different names*

### Comparing `esbmc_ai-0.5.0.dev3/esbmc_ai/commands/fix_code_command.py` & `esbmc_ai-0.5.0.dev4/esbmc_ai/commands/fix_code_command.py`

 * *Files 14% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 from ..msg_bus import Signal
 from ..loading_widget import create_loading_widget
 from ..esbmc_util import (
     esbmc_get_error_type,
     esbmc_load_source_code,
 )
 from ..solution_generator import SolutionGenerator, get_esbmc_output_formatted
-from ..logging import printv, printvv
+from ..logging import print_horizontal_line, printv, printvv
 
 # TODO Remove built in messages and move them to config.
 
 
 class FixCodeCommand(ChatCommand):
     on_solution_signal: Signal = Signal()
 
@@ -80,17 +80,17 @@
                     solution_generator.compress_message_stack()
                     self.anim.stop()
                 else:
                     break
 
             # Print verbose lvl 2
             printvv("\nGeneration:")
-            printvv("-" * get_terminal_size().columns)
+            print_horizontal_line(2)
             printvv(llm_solution)
-            printvv("-" * get_terminal_size().columns)
+            print_horizontal_line(2)
             printvv("")
 
             # Pass to ESBMC, a workaround is used where the file is saved
             # to a temporary location since ESBMC needs it in file format.
             self.anim.start("Verifying with ESBMC... Please Wait")
             exit_code, esbmc_output = esbmc_load_source_code(
                 file_path=file_name,
@@ -109,17 +109,17 @@
                     esbmc_output=esbmc_output,
                 )
             except ValueError:
                 # Probably did not compile and so ESBMC source code is clang output.
                 pass
 
             # Print verbose lvl 2
-            printvv("-" * get_terminal_size().columns)
+            print_horizontal_line(2)
             printvv(esbmc_output)
-            printvv("-" * get_terminal_size().columns)
+            print_horizontal_line(2)
 
             if exit_code == 0:
                 self.on_solution_signal.emit(llm_solution)
 
                 if config.raw_conversation:
                     messages: list[str] = [
                         f"{msg.type}: {msg.content}"
```

### Comparing `esbmc_ai-0.5.0.dev3/esbmc_ai/commands/help_command.py` & `esbmc_ai-0.5.0.dev4/esbmc_ai/commands/help_command.py`

 * *Files identical despite different names*

### Comparing `esbmc_ai-0.5.0.dev3/esbmc_ai/frontend/solution.py` & `esbmc_ai-0.5.0.dev4/esbmc_ai/frontend/solution.py`

 * *Files identical despite different names*

### Comparing `esbmc_ai-0.5.0.dev3/notebooks/ast.ipynb` & `esbmc_ai-0.5.0.dev4/notebooks/ast.ipynb`

 * *Files identical despite different names*

### Comparing `esbmc_ai-0.5.0.dev3/notebooks/samples/typedefs.c` & `esbmc_ai-0.5.0.dev4/notebooks/samples/typedefs.c`

 * *Files identical despite different names*

### Comparing `esbmc_ai-0.5.0.dev3/samples/add_last_unsafe.c` & `esbmc_ai-0.5.0.dev4/samples/add_last_unsafe.c`

 * *Files identical despite different names*

### Comparing `esbmc_ai-0.5.0.dev3/samples/optimize-code/sign_check.c` & `esbmc_ai-0.5.0.dev4/samples/optimize-code/sign_check.c`

 * *Files identical despite different names*

### Comparing `esbmc_ai-0.5.0.dev3/samples/optimize-code/sign_check_hard.c` & `esbmc_ai-0.5.0.dev4/samples/optimize-code/sign_check_hard.c`

 * *Files identical despite different names*

### Comparing `esbmc_ai-0.5.0.dev3/scripts/function_equivalence.c` & `esbmc_ai-0.5.0.dev4/scripts/function_equivalence.c`

 * *Files identical despite different names*

### Comparing `esbmc_ai-0.5.0.dev3/tests/test_ai_models.py` & `esbmc_ai-0.5.0.dev4/tests/test_ai_models.py`

 * *Files identical despite different names*

### Comparing `esbmc_ai-0.5.0.dev3/tests/test_base_chat_interface.py` & `esbmc_ai-0.5.0.dev4/tests/test_base_chat_interface.py`

 * *Files identical despite different names*

### Comparing `esbmc_ai-0.5.0.dev3/tests/test_command_parser.py` & `esbmc_ai-0.5.0.dev4/tests/test_command_parser.py`

 * *Files identical despite different names*

### Comparing `esbmc_ai-0.5.0.dev3/tests/test_config.py` & `esbmc_ai-0.5.0.dev4/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `esbmc_ai-0.5.0.dev3/tests/test_esbmc_util.py` & `esbmc_ai-0.5.0.dev4/tests/test_esbmc_util.py`

 * *Files identical despite different names*

### Comparing `esbmc_ai-0.5.0.dev3/tests/test_solution_generator.py` & `esbmc_ai-0.5.0.dev4/tests/test_solution_generator.py`

 * *Files identical despite different names*

### Comparing `esbmc_ai-0.5.0.dev3/tests/test_user_chat.py` & `esbmc_ai-0.5.0.dev4/tests/test_user_chat.py`

 * *Files identical despite different names*

### Comparing `esbmc_ai-0.5.0.dev3/tests/regtest/test_base_chat_interface.py` & `esbmc_ai-0.5.0.dev4/tests/regtest/test_base_chat_interface.py`

 * *Files identical despite different names*

### Comparing `esbmc_ai-0.5.0.dev3/tests/regtest/_regtest_outputs/test_base_chat_interface.test_send_message.out` & `esbmc_ai-0.5.0.dev4/tests/regtest/_regtest_outputs/test_base_chat_interface.test_send_message.out`

 * *Files identical despite different names*

### Comparing `esbmc_ai-0.5.0.dev3/tests/samples/esbmc_output/line_test/cartpole_26_safe.c-amalgamation-74.c` & `esbmc_ai-0.5.0.dev4/tests/samples/esbmc_output/line_test/cartpole_26_safe.c-amalgamation-74.c`

 * *Files identical despite different names*

### Comparing `esbmc_ai-0.5.0.dev3/tests/samples/esbmc_output/line_test/cartpole_48_safe.c-amalgamation-6.c` & `esbmc_ai-0.5.0.dev4/tests/samples/esbmc_output/line_test/cartpole_48_safe.c-amalgamation-6.c`

 * *Files identical despite different names*

### Comparing `esbmc_ai-0.5.0.dev3/tests/samples/esbmc_output/line_test/cartpole_92_safe.c-amalgamation-14.c` & `esbmc_ai-0.5.0.dev4/tests/samples/esbmc_output/line_test/cartpole_92_safe.c-amalgamation-14.c`

 * *Files identical despite different names*

### Comparing `esbmc_ai-0.5.0.dev3/tests/samples/esbmc_output/line_test/cartpole_95_safe.c-amalgamation-80.c` & `esbmc_ai-0.5.0.dev4/tests/samples/esbmc_output/line_test/cartpole_95_safe.c-amalgamation-80.c`

 * *Files identical despite different names*

### Comparing `esbmc_ai-0.5.0.dev3/tests/samples/esbmc_output/line_test/robot_5_safe.c-amalgamation-13.c` & `esbmc_ai-0.5.0.dev4/tests/samples/esbmc_output/line_test/robot_5_safe.c-amalgamation-13.c`

 * *Files identical despite different names*

### Comparing `esbmc_ai-0.5.0.dev3/tests/samples/esbmc_output/line_test/vdp_1_safe.c-amalgamation-28.c` & `esbmc_ai-0.5.0.dev4/tests/samples/esbmc_output/line_test/vdp_1_safe.c-amalgamation-28.c`

 * *Files identical despite different names*

### Comparing `esbmc_ai-0.5.0.dev3/.gitignore` & `esbmc_ai-0.5.0.dev4/.gitignore`

 * *Files identical despite different names*

### Comparing `esbmc_ai-0.5.0.dev3/LICENSE` & `esbmc_ai-0.5.0.dev4/LICENSE`

 * *Files identical despite different names*

### Comparing `esbmc_ai-0.5.0.dev3/README.md` & `esbmc_ai-0.5.0.dev4/README.md`

 * *Files identical despite different names*

### Comparing `esbmc_ai-0.5.0.dev3/pyproject.toml` & `esbmc_ai-0.5.0.dev4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `esbmc_ai-0.5.0.dev3/PKG-INFO` & `esbmc_ai-0.5.0.dev4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: esbmc_ai
-Version: 0.5.0.dev3
+Version: 0.5.0.dev4
 Summary: LLM driven development and automatic repair kit.
 Project-URL: Homepage, https://github.com/Yiannis128/esbmc-ai
 Project-URL: Source Code, https://github.com/Yiannis128/esbmc-ai
 Project-URL: Documentation, https://github.com/Yiannis128/esbmc-ai/wiki
 Project-URL: Issues, https://github.com/Yiannis128/esbmc-ai/issues
 Author-email: Yiannis Charalambous <yiannis128@hotmail.com>
 License-File: LICENSE
```

