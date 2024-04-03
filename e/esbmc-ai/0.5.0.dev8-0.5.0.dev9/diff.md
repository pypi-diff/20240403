# Comparing `tmp/esbmc_ai-0.5.0.dev8.tar.gz` & `tmp/esbmc_ai-0.5.0.dev9.tar.gz`

## Comparing `esbmc_ai-0.5.0.dev8.tar` & `esbmc_ai-0.5.0.dev9.tar`

### file list

```diff
@@ -1,77 +1,139 @@
--rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev8/.env.example
--rw-r--r--   0        0        0    21341 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev8/.pylintrc
--rw-r--r--   0        0        0      731 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev8/Pipfile
--rwxr-xr-x   0        0        0       62 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev8/build.sh
--rwxr-xr-x   0        0        0       81 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev8/clean.sh
--rw-r--r--   0        0        0     5106 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev8/config.json
--rwxr-xr-x   0        0        0       41 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev8/esbmc-ai
--rw-r--r--   0        0        0     6657 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev8/requirements.txt
--rwxr-xr-x   0        0        0      412 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev8/upload.sh
--rw-r--r--   0        0        0     1495 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev8/.github/workflows/workflow.yml
--rw-r--r--   0        0        0      371 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev8/.vscode/c_cpp_properties.json
--rw-r--r--   0        0        0     1696 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev8/.vscode/launch.json
--rw-r--r--   0        0        0      105 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev8/.vscode/settings.json
--rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev8/esbmc_ai/__about__.py
--rw-r--r--   0        0        0      238 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev8/esbmc_ai/__init__.py
--rwxr-xr-x   0        0        0    14539 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev8/esbmc_ai/__main__.py
--rw-r--r--   0        0        0    12079 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev8/esbmc_ai/ai_models.py
--rw-r--r--   0        0        0      241 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev8/esbmc_ai/api_key_collection.py
--rw-r--r--   0        0        0     4612 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev8/esbmc_ai/base_chat_interface.py
--rw-r--r--   0        0        0     1547 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev8/esbmc_ai/chat_response.py
--rw-r--r--   0        0        0    15371 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev8/esbmc_ai/config.py
--rw-r--r--   0        0        0     4511 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev8/esbmc_ai/esbmc_util.py
--rw-r--r--   0        0        0     2487 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev8/esbmc_ai/loading_widget.py
--rw-r--r--   0        0        0      790 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev8/esbmc_ai/logging.py
--rw-r--r--   0        0        0      414 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev8/esbmc_ai/msg_bus.py
--rw-r--r--   0        0        0     1226 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev8/esbmc_ai/optimize_code.py
--rw-r--r--   0        0        0     5627 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev8/esbmc_ai/solution_generator.py
--rw-r--r--   0        0        0     2271 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev8/esbmc_ai/user_chat.py
--rw-r--r--   0        0        0      253 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev8/esbmc_ai/commands/__init__.py
--rw-r--r--   0        0        0      565 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev8/esbmc_ai/commands/chat_command.py
--rw-r--r--   0        0        0      458 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev8/esbmc_ai/commands/exit_command.py
--rw-r--r--   0        0        0     6270 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev8/esbmc_ai/commands/fix_code_command.py
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev8/esbmc_ai/commands/help_command.py
--rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev8/esbmc_ai/frontend/__init__.py
--rw-r--r--   0        0        0     1667 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev8/esbmc_ai/frontend/solution.py
--rw-r--r--   0        0        0    18626 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev8/notebooks/ast.ipynb
--rw-r--r--   0        0        0      557 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev8/notebooks/samples/typedefs.c
--rw-r--r--   0        0        0      565 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev8/samples/add_last_unsafe.c
--rw-r--r--   0        0        0      378 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev8/samples/automatic_arrays.c
--rw-r--r--   0        0        0      448 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev8/samples/dynamic_mem_alloc.c
--rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev8/samples/hello_world.c
--rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev8/samples/mem_leak.c
--rw-r--r--   0        0        0      272 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev8/samples/optimize_code_test_01.c
--rw-r--r--   0        0        0      363 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev8/samples/threading.c
--rw-r--r--   0        0        0      364 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev8/samples/threading_broken.c
--rw-r--r--   0        0        0      204 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev8/samples/unsafe_access.c
--rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev8/samples/ast/function_test_1.c
--rw-r--r--   0        0        0      347 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev8/samples/ast/function_test_2.c
--rw-r--r--   0        0        0      351 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev8/samples/optimize-code/fact_01.c
--rw-r--r--   0        0        0      275 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev8/samples/optimize-code/mult.c
--rw-r--r--   0        0        0      570 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev8/samples/optimize-code/sign_check.c
--rw-r--r--   0        0        0      588 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev8/samples/optimize-code/sign_check_hard.c
--rw-r--r--   0        0        0      791 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev8/scripts/function_equivalence.c
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev8/tests/__init__.py
--rw-r--r--   0        0        0     4229 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev8/tests/test_ai_models.py
--rw-r--r--   0        0        0     3835 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev8/tests/test_base_chat_interface.py
--rw-r--r--   0        0        0      588 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev8/tests/test_command_parser.py
--rw-r--r--   0        0        0     3499 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev8/tests/test_config.py
--rw-r--r--   0        0        0     4655 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev8/tests/test_esbmc_util.py
--rw-r--r--   0        0        0      459 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev8/tests/test_solution.py
--rw-r--r--   0        0        0      576 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev8/tests/test_solution_generator.py
--rw-r--r--   0        0        0     2238 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev8/tests/test_user_chat.py
--rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev8/tests/regtest/__init__.py
--rw-r--r--   0        0        0     1831 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev8/tests/regtest/test_base_chat_interface.py
--rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev8/tests/regtest/_regtest_outputs/test_base_chat_interface.test_push_message_stack.out
--rw-r--r--   0        0        0      558 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev8/tests/regtest/_regtest_outputs/test_base_chat_interface.test_send_message.out
--rw-r--r--   0        0        0  5597855 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev8/tests/samples/esbmc_output/line_test/cartpole_26_safe.c-amalgamation-74.c
--rw-r--r--   0        0        0  1700020 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev8/tests/samples/esbmc_output/line_test/cartpole_48_safe.c-amalgamation-6.c
--rw-r--r--   0        0        0     2115 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev8/tests/samples/esbmc_output/line_test/cartpole_92_safe.c-amalgamation-14.c
--rw-r--r--   0        0        0  1226238 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev8/tests/samples/esbmc_output/line_test/cartpole_95_safe.c-amalgamation-80.c
--rw-r--r--   0        0        0  2808039 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev8/tests/samples/esbmc_output/line_test/robot_5_safe.c-amalgamation-13.c
--rw-r--r--   0        0        0   373267 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev8/tests/samples/esbmc_output/line_test/vdp_1_safe.c-amalgamation-28.c
--rw-r--r--   0        0        0     3173 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev8/.gitignore
--rw-r--r--   0        0        0    34523 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev8/LICENSE
--rw-r--r--   0        0        0     2147 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev8/README.md
--rw-r--r--   0        0        0     1784 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev8/pyproject.toml
--rw-r--r--   0        0        0     3335 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev8/PKG-INFO
+-rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev9/.env.example
+-rw-r--r--   0        0        0    21341 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev9/.pylintrc
+-rw-r--r--   0        0        0      731 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev9/Pipfile
+-rwxr-xr-x   0        0        0       62 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev9/build.sh
+-rw-r--r--   0        0        0   126731 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev9/cartpole_60_safe.c-amalgamation-89.c
+-rwxr-xr-x   0        0        0       81 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev9/clean.sh
+-rw-r--r--   0        0        0     5106 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev9/config.json
+-rwxr-xr-x   0        0        0       41 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev9/esbmc-ai
+-rw-r--r--   0        0        0     6657 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev9/requirements.txt
+-rwxr-xr-x   0        0        0      412 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev9/upload.sh
+-rw-r--r--   0        0        0     1495 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev9/.github/workflows/workflow.yml
+-rw-r--r--   0        0        0      371 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev9/.vscode/c_cpp_properties.json
+-rw-r--r--   0        0        0     1696 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev9/.vscode/launch.json
+-rw-r--r--   0        0        0      105 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev9/.vscode/settings.json
+-rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev9/esbmc_ai/__about__.py
+-rw-r--r--   0        0        0      238 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev9/esbmc_ai/__init__.py
+-rwxr-xr-x   0        0        0    14539 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev9/esbmc_ai/__main__.py
+-rw-r--r--   0        0        0    12079 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev9/esbmc_ai/ai_models.py
+-rw-r--r--   0        0        0      241 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev9/esbmc_ai/api_key_collection.py
+-rw-r--r--   0        0        0     4612 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev9/esbmc_ai/base_chat_interface.py
+-rw-r--r--   0        0        0     1547 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev9/esbmc_ai/chat_response.py
+-rw-r--r--   0        0        0    15371 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev9/esbmc_ai/config.py
+-rw-r--r--   0        0        0     4511 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev9/esbmc_ai/esbmc_util.py
+-rw-r--r--   0        0        0     2487 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev9/esbmc_ai/loading_widget.py
+-rw-r--r--   0        0        0      790 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev9/esbmc_ai/logging.py
+-rw-r--r--   0        0        0      414 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev9/esbmc_ai/msg_bus.py
+-rw-r--r--   0        0        0     1226 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev9/esbmc_ai/optimize_code.py
+-rw-r--r--   0        0        0     5951 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev9/esbmc_ai/solution_generator.py
+-rw-r--r--   0        0        0     2271 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev9/esbmc_ai/user_chat.py
+-rw-r--r--   0        0        0      253 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev9/esbmc_ai/commands/__init__.py
+-rw-r--r--   0        0        0      565 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev9/esbmc_ai/commands/chat_command.py
+-rw-r--r--   0        0        0      458 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev9/esbmc_ai/commands/exit_command.py
+-rw-r--r--   0        0        0     6586 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev9/esbmc_ai/commands/fix_code_command.py
+-rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev9/esbmc_ai/commands/help_command.py
+-rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev9/esbmc_ai/frontend/__init__.py
+-rw-r--r--   0        0        0     1667 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev9/esbmc_ai/frontend/solution.py
+-rw-r--r--   0        0        0      672 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev9/includes/CMakeLists.txt
+-rw-r--r--   0        0        0      372 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev9/includes/verifier_functions.h
+-rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev9/includes/verifier_stubs.c
+-rw-r--r--   0        0        0     6789 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev9/includes/keras2c/k2c_activations.c
+-rw-r--r--   0        0        0    16892 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev9/includes/keras2c/k2c_convolution_layers.c
+-rw-r--r--   0        0        0     4200 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev9/includes/keras2c/k2c_core_layers.c
+-rw-r--r--   0        0        0      846 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev9/includes/keras2c/k2c_embedding_layers.c
+-rw-r--r--   0        0        0     8930 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev9/includes/keras2c/k2c_helper_functions.c
+-rw-r--r--   0        0        0     8151 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev9/includes/keras2c/k2c_include.h
+-rw-r--r--   0        0        0     5400 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev9/includes/keras2c/k2c_merge_layers.c
+-rw-r--r--   0        0        0     1395 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev9/includes/keras2c/k2c_normalization_layers.c
+-rw-r--r--   0        0        0     6006 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev9/includes/keras2c/k2c_pooling_layers.c
+-rw-r--r--   0        0        0    15198 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev9/includes/keras2c/k2c_recurrent_layers.c
+-rw-r--r--   0        0        0      739 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev9/includes/keras2c/k2c_tensor_include.h
+-rw-r--r--   0        0        0     1234 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev9/includes/math_op_models/__cosdf.c
+-rw-r--r--   0        0        0      580 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev9/includes/math_op_models/__expo2f.c
+-rw-r--r--   0        0        0      254 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev9/includes/math_op_models/__fpclassifyf.c
+-rw-r--r--   0        0        0     2397 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev9/includes/math_op_models/__invtrigl.c
+-rw-r--r--   0        0        0      202 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev9/includes/math_op_models/__invtrigl.h
+-rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev9/includes/math_op_models/__math_divzerof.c
+-rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev9/includes/math_op_models/__math_invalidf.c
+-rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev9/includes/math_op_models/__math_oflowf.c
+-rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev9/includes/math_op_models/__math_uflowf.c
+-rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev9/includes/math_op_models/__math_xflowf.c
+-rw-r--r--   0        0        0    16408 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev9/includes/math_op_models/__rem_pio2_large.c
+-rw-r--r--   0        0        0     2242 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev9/includes/math_op_models/__rem_pio2f.c
+-rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev9/includes/math_op_models/__signbitf.c
+-rw-r--r--   0        0        0     1233 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev9/includes/math_op_models/__sindf.c
+-rw-r--r--   0        0        0     2001 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev9/includes/math_op_models/__tandf.c
+-rw-r--r--   0        0        0     1567 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev9/includes/math_op_models/acosf.c
+-rw-r--r--   0        0        0      348 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev9/includes/math_op_models/alltypes.h
+-rw-r--r--   0        0        0     1462 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev9/includes/math_op_models/asinf.c
+-rw-r--r--   0        0        0      578 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev9/includes/math_op_models/atanhf.c
+-rw-r--r--   0        0        0     2091 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev9/includes/math_op_models/atomic.h
+-rw-r--r--   0        0        0     1943 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev9/includes/math_op_models/cosf.c
+-rw-r--r--   0        0        0     2070 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev9/includes/math_op_models/endian.h
+-rw-r--r--   0        0        0     5350 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev9/includes/math_op_models/erff.c
+-rw-r--r--   0        0        0     1323 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev9/includes/math_op_models/exp2f_data.c
+-rw-r--r--   0        0        0      494 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev9/includes/math_op_models/exp2f_data.h
+-rw-r--r--   0        0        0      535 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev9/includes/math_op_models/exp_data.h
+-rw-r--r--   0        0        0     1895 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev9/includes/math_op_models/expf.c
+-rw-r--r--   0        0        0     2731 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev9/includes/math_op_models/expm1f.c
+-rw-r--r--   0        0        0      136 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev9/includes/math_op_models/fabsf.c
+-rw-r--r--   0        0        0      241 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev9/includes/math_op_models/fmaxf.c
+-rw-r--r--   0        0        0     8880 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev9/includes/math_op_models/libm.h
+-rw-r--r--   0        0        0     1989 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev9/includes/math_op_models/log1pf.c
+-rw-r--r--   0        0        0      533 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev9/includes/math_op_models/log2_data.h
+-rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev9/includes/math_op_models/log2f_data.c
+-rw-r--r--   0        0        0      355 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev9/includes/math_op_models/log2f_data.h
+-rw-r--r--   0        0        0      547 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev9/includes/math_op_models/log_data.h
+-rw-r--r--   0        0        0     1732 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev9/includes/math_op_models/logf.c
+-rw-r--r--   0        0        0     1087 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev9/includes/math_op_models/logf_data.c
+-rw-r--r--   0        0        0      401 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev9/includes/math_op_models/logf_data.h
+-rw-r--r--   0        0        0      514 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev9/includes/math_op_models/pow_data.h
+-rw-r--r--   0        0        0     1388 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev9/includes/math_op_models/powf_data.c
+-rw-r--r--   0        0        0      548 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev9/includes/math_op_models/powf_data.h
+-rw-r--r--   0        0        0     1992 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev9/includes/math_op_models/sinf.c
+-rw-r--r--   0        0        0      974 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev9/includes/math_op_models/sqrt_data.c
+-rw-r--r--   0        0        0      347 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev9/includes/math_op_models/sqrt_data.h
+-rw-r--r--   0        0        0     1897 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev9/includes/math_op_models/sqrtf.c
+-rw-r--r--   0        0        0      653 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev9/includes/math_op_models/tanhf.c
+-rw-r--r--   0        0        0    18626 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev9/notebooks/ast.ipynb
+-rw-r--r--   0        0        0      557 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev9/notebooks/samples/typedefs.c
+-rw-r--r--   0        0        0      565 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev9/samples/add_last_unsafe.c
+-rw-r--r--   0        0        0      378 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev9/samples/automatic_arrays.c
+-rw-r--r--   0        0        0      448 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev9/samples/dynamic_mem_alloc.c
+-rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev9/samples/hello_world.c
+-rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev9/samples/mem_leak.c
+-rw-r--r--   0        0        0      272 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev9/samples/optimize_code_test_01.c
+-rw-r--r--   0        0        0      363 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev9/samples/threading.c
+-rw-r--r--   0        0        0      364 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev9/samples/threading_broken.c
+-rw-r--r--   0        0        0      204 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev9/samples/unsafe_access.c
+-rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev9/samples/ast/function_test_1.c
+-rw-r--r--   0        0        0      347 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev9/samples/ast/function_test_2.c
+-rw-r--r--   0        0        0      351 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev9/samples/optimize-code/fact_01.c
+-rw-r--r--   0        0        0      275 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev9/samples/optimize-code/mult.c
+-rw-r--r--   0        0        0      570 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev9/samples/optimize-code/sign_check.c
+-rw-r--r--   0        0        0      588 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev9/samples/optimize-code/sign_check_hard.c
+-rw-r--r--   0        0        0      791 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev9/scripts/function_equivalence.c
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev9/tests/__init__.py
+-rw-r--r--   0        0        0     4229 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev9/tests/test_ai_models.py
+-rw-r--r--   0        0        0     3835 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev9/tests/test_base_chat_interface.py
+-rw-r--r--   0        0        0      588 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev9/tests/test_command_parser.py
+-rw-r--r--   0        0        0     3499 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev9/tests/test_config.py
+-rw-r--r--   0        0        0     4655 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev9/tests/test_esbmc_util.py
+-rw-r--r--   0        0        0      459 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev9/tests/test_solution.py
+-rw-r--r--   0        0        0      576 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev9/tests/test_solution_generator.py
+-rw-r--r--   0        0        0     2238 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev9/tests/test_user_chat.py
+-rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev9/tests/regtest/__init__.py
+-rw-r--r--   0        0        0     1831 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev9/tests/regtest/test_base_chat_interface.py
+-rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev9/tests/regtest/_regtest_outputs/test_base_chat_interface.test_push_message_stack.out
+-rw-r--r--   0        0        0      558 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev9/tests/regtest/_regtest_outputs/test_base_chat_interface.test_send_message.out
+-rw-r--r--   0        0        0  5597855 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev9/tests/samples/esbmc_output/line_test/cartpole_26_safe.c-amalgamation-74.c
+-rw-r--r--   0        0        0  1700020 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev9/tests/samples/esbmc_output/line_test/cartpole_48_safe.c-amalgamation-6.c
+-rw-r--r--   0        0        0     2115 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev9/tests/samples/esbmc_output/line_test/cartpole_92_safe.c-amalgamation-14.c
+-rw-r--r--   0        0        0  1226238 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev9/tests/samples/esbmc_output/line_test/cartpole_95_safe.c-amalgamation-80.c
+-rw-r--r--   0        0        0  2808039 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev9/tests/samples/esbmc_output/line_test/robot_5_safe.c-amalgamation-13.c
+-rw-r--r--   0        0        0   373267 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev9/tests/samples/esbmc_output/line_test/vdp_1_safe.c-amalgamation-28.c
+-rw-r--r--   0        0        0     3173 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev9/.gitignore
+-rw-r--r--   0        0        0    34523 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev9/LICENSE
+-rw-r--r--   0        0        0     2147 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev9/README.md
+-rw-r--r--   0        0        0     1784 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev9/pyproject.toml
+-rw-r--r--   0        0        0     3335 2020-02-02 00:00:00.000000 esbmc_ai-0.5.0.dev9/PKG-INFO
```

### Comparing `esbmc_ai-0.5.0.dev8/.pylintrc` & `esbmc_ai-0.5.0.dev9/.pylintrc`

 * *Files identical despite different names*

### Comparing `esbmc_ai-0.5.0.dev8/Pipfile` & `esbmc_ai-0.5.0.dev9/Pipfile`

 * *Files identical despite different names*

### Comparing `esbmc_ai-0.5.0.dev8/config.json` & `esbmc_ai-0.5.0.dev9/config.json`

 * *Files identical despite different names*

### Comparing `esbmc_ai-0.5.0.dev8/requirements.txt` & `esbmc_ai-0.5.0.dev9/requirements.txt`

 * *Files identical despite different names*

### Comparing `esbmc_ai-0.5.0.dev8/.github/workflows/workflow.yml` & `esbmc_ai-0.5.0.dev9/.github/workflows/workflow.yml`

 * *Files identical despite different names*

### Comparing `esbmc_ai-0.5.0.dev8/.vscode/launch.json` & `esbmc_ai-0.5.0.dev9/.vscode/launch.json`

 * *Files identical despite different names*

### Comparing `esbmc_ai-0.5.0.dev8/esbmc_ai/__main__.py` & `esbmc_ai-0.5.0.dev9/esbmc_ai/__main__.py`

 * *Files identical despite different names*

### Comparing `esbmc_ai-0.5.0.dev8/esbmc_ai/ai_models.py` & `esbmc_ai-0.5.0.dev9/esbmc_ai/ai_models.py`

 * *Files identical despite different names*

### Comparing `esbmc_ai-0.5.0.dev8/esbmc_ai/base_chat_interface.py` & `esbmc_ai-0.5.0.dev9/esbmc_ai/base_chat_interface.py`

 * *Files identical despite different names*

### Comparing `esbmc_ai-0.5.0.dev8/esbmc_ai/chat_response.py` & `esbmc_ai-0.5.0.dev9/esbmc_ai/chat_response.py`

 * *Files identical despite different names*

### Comparing `esbmc_ai-0.5.0.dev8/esbmc_ai/config.py` & `esbmc_ai-0.5.0.dev9/esbmc_ai/config.py`

 * *Files identical despite different names*

### Comparing `esbmc_ai-0.5.0.dev8/esbmc_ai/esbmc_util.py` & `esbmc_ai-0.5.0.dev9/esbmc_ai/esbmc_util.py`

 * *Files identical despite different names*

### Comparing `esbmc_ai-0.5.0.dev8/esbmc_ai/loading_widget.py` & `esbmc_ai-0.5.0.dev9/esbmc_ai/loading_widget.py`

 * *Files identical despite different names*

### Comparing `esbmc_ai-0.5.0.dev8/esbmc_ai/logging.py` & `esbmc_ai-0.5.0.dev9/esbmc_ai/logging.py`

 * *Files identical despite different names*

### Comparing `esbmc_ai-0.5.0.dev8/esbmc_ai/optimize_code.py` & `esbmc_ai-0.5.0.dev9/esbmc_ai/optimize_code.py`

 * *Files identical despite different names*

### Comparing `esbmc_ai-0.5.0.dev8/esbmc_ai/solution_generator.py` & `esbmc_ai-0.5.0.dev9/esbmc_ai/solution_generator.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,35 +1,43 @@
 # Author: Yiannis Charalambous 2023
 
 from re import S
 from typing import Optional
 from typing_extensions import override
 from langchain.base_language import BaseLanguageModel
-from langchain.schema import BaseMessage, HumanMessage
+from langchain.schema import BaseMessage
 
 from esbmc_ai.chat_response import ChatResponse, FinishReason
 from esbmc_ai.config import ChatPromptSettings, DynamicAIModelAgent
 from esbmc_ai.frontend.solution import apply_line_patch
 
 from .ai_models import AIModel
 from .base_chat_interface import BaseChatInterface
 from esbmc_ai.esbmc_util import (
     esbmc_get_counter_example,
     esbmc_get_violated_property,
     get_source_code_err_line_idx,
 )
 
 
+class ESBMCTimedOutException(Exception):
+    pass
+
+
+class SourceCodeParseError(Exception):
+    pass
+
+
 def get_source_code_formatted(
     source_code_format: str, source_code: str, esbmc_output: str
 ) -> str:
     match source_code_format:
         case "single":
             line: Optional[int] = get_source_code_err_line_idx(esbmc_output)
-            assert line, "error line not found in esbmc output"
+            assert line, f"error line not found in esbmc output:\n{esbmc_output}"
             # ESBMC reports errors starting from 1. To get the correct line, we need to use 0 based
             # indexing.
             return source_code.splitlines(True)[line]
         case "full":
             return source_code
         case _:
             raise ValueError(
@@ -37,21 +45,23 @@
             )
 
 
 def get_esbmc_output_formatted(esbmc_output_type: str, esbmc_output: str) -> str:
     # Check for parsing error
     if "ERROR: PARSING ERROR" in esbmc_output:
         # Parsing errors are usually small in nature.
-        return esbmc_output
+        raise SourceCodeParseError()
+    elif "ERROR: Timed out" in esbmc_output:
+        raise ESBMCTimedOutException()
 
     match esbmc_output_type:
         case "vp":
             value: Optional[str] = esbmc_get_violated_property(esbmc_output)
             if not value:
-                raise ValueError("Not found violated property.")
+                raise ValueError("Not found violated property." + esbmc_output)
             return value
         case "ce":
             value: Optional[str] = esbmc_get_counter_example(esbmc_output)
             if not value:
                 raise ValueError("Not found counterexample.")
             return value
         case "full":
@@ -81,28 +91,30 @@
             ai_model_agent=chat_prompt,
             ai_model=ai_model,
             llm=llm,
         )
         self.initial_prompt = ai_model_agent.initial_prompt
 
         self.esbmc_output_type: str = esbmc_output_type
-        self.esbmc_output = get_esbmc_output_formatted(
-            esbmc_output_type=self.esbmc_output_type,
-            esbmc_output=esbmc_output,
-        )
-
         self.source_code_format: str = source_code_format
         self.source_code_raw: str = source_code
 
+        try:
+            self.esbmc_output = get_esbmc_output_formatted(
+                esbmc_output_type=self.esbmc_output_type,
+                esbmc_output=esbmc_output,
+            )
+        except SourceCodeParseError:
+            self.esbmc_output = esbmc_output
+
         source_code_formatted: str = get_source_code_formatted(
             source_code_format=self.source_code_format,
             source_code=self.source_code_raw,
             esbmc_output=self.esbmc_output,
         )
-
         self.apply_template_value(
             source_code=source_code_formatted,
             esbmc_output=self.esbmc_output,
         )
 
     @override
     def compress_message_stack(self) -> None:
```

### Comparing `esbmc_ai-0.5.0.dev8/esbmc_ai/user_chat.py` & `esbmc_ai-0.5.0.dev9/esbmc_ai/user_chat.py`

 * *Files identical despite different names*

### Comparing `esbmc_ai-0.5.0.dev8/esbmc_ai/commands/chat_command.py` & `esbmc_ai-0.5.0.dev9/esbmc_ai/commands/chat_command.py`

 * *Files identical despite different names*

### Comparing `esbmc_ai-0.5.0.dev8/esbmc_ai/commands/fix_code_command.py` & `esbmc_ai-0.5.0.dev9/esbmc_ai/commands/fix_code_command.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,25 +1,31 @@
 # Author: Yiannis Charalambous
 
 from os import get_terminal_size
+import sys
 from typing import Any, Tuple
 from typing_extensions import override
 from langchain.schema import AIMessage, HumanMessage
 
 from esbmc_ai.chat_response import FinishReason
 
 from .chat_command import ChatCommand
 from .. import config
 from ..msg_bus import Signal
 from ..loading_widget import create_loading_widget
 from ..esbmc_util import (
     esbmc_get_error_type,
     esbmc_load_source_code,
 )
-from ..solution_generator import SolutionGenerator, get_esbmc_output_formatted
+from ..solution_generator import (
+    ESBMCTimedOutException,
+    SolutionGenerator,
+    SourceCodeParseError,
+    get_esbmc_output_formatted,
+)
 from ..logging import print_horizontal_line, printv, printvv
 
 # TODO Remove built in messages and move them to config.
 
 
 class FixCodeCommand(ChatCommand):
     on_solution_signal: Signal = Signal()
@@ -51,29 +57,33 @@
         printv(f"Scenario: {scenario}")
         printv(
             f"Using dynamic prompt..."
             if scenario in config.chat_prompt_generator_mode.scenarios
             else "Using generic prompt..."
         )
 
-        solution_generator = SolutionGenerator(
-            ai_model_agent=config.chat_prompt_generator_mode,
-            source_code=source_code,
-            esbmc_output=esbmc_output,
-            ai_model=config.ai_model,
-            llm=config.ai_model.create_llm(
-                api_keys=config.api_keys,
-                temperature=config.chat_prompt_generator_mode.temperature,
-                requests_max_tries=config.requests_max_tries,
-                requests_timeout=config.requests_timeout,
-            ),
-            scenario=scenario,
-            source_code_format=config.source_code_format,
-            esbmc_output_type=config.esbmc_output_type,
-        )
+        try:
+            solution_generator = SolutionGenerator(
+                ai_model_agent=config.chat_prompt_generator_mode,
+                source_code=source_code,
+                esbmc_output=esbmc_output,
+                ai_model=config.ai_model,
+                llm=config.ai_model.create_llm(
+                    api_keys=config.api_keys,
+                    temperature=config.chat_prompt_generator_mode.temperature,
+                    requests_max_tries=config.requests_max_tries,
+                    requests_timeout=config.requests_timeout,
+                ),
+                scenario=scenario,
+                source_code_format=config.source_code_format,
+                esbmc_output_type=config.esbmc_output_type,
+            )
+        except ESBMCTimedOutException:
+            print("error: ESBMC has timed out...")
+            sys.exit(1)
 
         print()
 
         max_retries: int = config.fix_code_max_attempts
         for idx in range(max_retries):
             # Get a response. Use while loop to account for if the message stack
             # gets full, then need to compress and retry.
@@ -112,17 +122,19 @@
             # TODO Move this process into Solution Generator since have (beginning) is done
             # inside, and the other half is done here.
             try:
                 esbmc_output = get_esbmc_output_formatted(
                     esbmc_output_type=config.esbmc_output_type,
                     esbmc_output=esbmc_output,
                 )
-            except ValueError:
-                # Probably did not compile and so ESBMC source code is clang output.
+            except SourceCodeParseError:
                 pass
+            except ESBMCTimedOutException:
+                print("error: ESBMC has timed out...")
+                sys.exit(1)
 
             # Print verbose lvl 2
             print_horizontal_line(2)
             printvv(esbmc_output)
             print_horizontal_line(2)
 
             if exit_code == 0:
```

### Comparing `esbmc_ai-0.5.0.dev8/esbmc_ai/commands/help_command.py` & `esbmc_ai-0.5.0.dev9/esbmc_ai/commands/help_command.py`

 * *Files identical despite different names*

### Comparing `esbmc_ai-0.5.0.dev8/esbmc_ai/frontend/solution.py` & `esbmc_ai-0.5.0.dev9/esbmc_ai/frontend/solution.py`

 * *Files identical despite different names*

### Comparing `esbmc_ai-0.5.0.dev8/notebooks/ast.ipynb` & `esbmc_ai-0.5.0.dev9/notebooks/ast.ipynb`

 * *Files identical despite different names*

### Comparing `esbmc_ai-0.5.0.dev8/notebooks/samples/typedefs.c` & `esbmc_ai-0.5.0.dev9/notebooks/samples/typedefs.c`

 * *Files identical despite different names*

### Comparing `esbmc_ai-0.5.0.dev8/samples/add_last_unsafe.c` & `esbmc_ai-0.5.0.dev9/samples/add_last_unsafe.c`

 * *Files identical despite different names*

### Comparing `esbmc_ai-0.5.0.dev8/samples/optimize-code/sign_check.c` & `esbmc_ai-0.5.0.dev9/samples/optimize-code/sign_check.c`

 * *Files identical despite different names*

### Comparing `esbmc_ai-0.5.0.dev8/samples/optimize-code/sign_check_hard.c` & `esbmc_ai-0.5.0.dev9/samples/optimize-code/sign_check_hard.c`

 * *Files identical despite different names*

### Comparing `esbmc_ai-0.5.0.dev8/scripts/function_equivalence.c` & `esbmc_ai-0.5.0.dev9/scripts/function_equivalence.c`

 * *Files identical despite different names*

### Comparing `esbmc_ai-0.5.0.dev8/tests/test_ai_models.py` & `esbmc_ai-0.5.0.dev9/tests/test_ai_models.py`

 * *Files identical despite different names*

### Comparing `esbmc_ai-0.5.0.dev8/tests/test_base_chat_interface.py` & `esbmc_ai-0.5.0.dev9/tests/test_base_chat_interface.py`

 * *Files identical despite different names*

### Comparing `esbmc_ai-0.5.0.dev8/tests/test_command_parser.py` & `esbmc_ai-0.5.0.dev9/tests/test_command_parser.py`

 * *Files identical despite different names*

### Comparing `esbmc_ai-0.5.0.dev8/tests/test_config.py` & `esbmc_ai-0.5.0.dev9/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `esbmc_ai-0.5.0.dev8/tests/test_esbmc_util.py` & `esbmc_ai-0.5.0.dev9/tests/test_esbmc_util.py`

 * *Files identical despite different names*

### Comparing `esbmc_ai-0.5.0.dev8/tests/test_solution_generator.py` & `esbmc_ai-0.5.0.dev9/tests/test_solution_generator.py`

 * *Files identical despite different names*

### Comparing `esbmc_ai-0.5.0.dev8/tests/test_user_chat.py` & `esbmc_ai-0.5.0.dev9/tests/test_user_chat.py`

 * *Files identical despite different names*

### Comparing `esbmc_ai-0.5.0.dev8/tests/regtest/test_base_chat_interface.py` & `esbmc_ai-0.5.0.dev9/tests/regtest/test_base_chat_interface.py`

 * *Files identical despite different names*

### Comparing `esbmc_ai-0.5.0.dev8/tests/regtest/_regtest_outputs/test_base_chat_interface.test_send_message.out` & `esbmc_ai-0.5.0.dev9/tests/regtest/_regtest_outputs/test_base_chat_interface.test_send_message.out`

 * *Files identical despite different names*

### Comparing `esbmc_ai-0.5.0.dev8/tests/samples/esbmc_output/line_test/cartpole_26_safe.c-amalgamation-74.c` & `esbmc_ai-0.5.0.dev9/tests/samples/esbmc_output/line_test/cartpole_26_safe.c-amalgamation-74.c`

 * *Files identical despite different names*

### Comparing `esbmc_ai-0.5.0.dev8/tests/samples/esbmc_output/line_test/cartpole_48_safe.c-amalgamation-6.c` & `esbmc_ai-0.5.0.dev9/tests/samples/esbmc_output/line_test/cartpole_48_safe.c-amalgamation-6.c`

 * *Files identical despite different names*

### Comparing `esbmc_ai-0.5.0.dev8/tests/samples/esbmc_output/line_test/cartpole_92_safe.c-amalgamation-14.c` & `esbmc_ai-0.5.0.dev9/tests/samples/esbmc_output/line_test/cartpole_92_safe.c-amalgamation-14.c`

 * *Files identical despite different names*

### Comparing `esbmc_ai-0.5.0.dev8/tests/samples/esbmc_output/line_test/cartpole_95_safe.c-amalgamation-80.c` & `esbmc_ai-0.5.0.dev9/tests/samples/esbmc_output/line_test/cartpole_95_safe.c-amalgamation-80.c`

 * *Files identical despite different names*

### Comparing `esbmc_ai-0.5.0.dev8/tests/samples/esbmc_output/line_test/robot_5_safe.c-amalgamation-13.c` & `esbmc_ai-0.5.0.dev9/tests/samples/esbmc_output/line_test/robot_5_safe.c-amalgamation-13.c`

 * *Files identical despite different names*

### Comparing `esbmc_ai-0.5.0.dev8/tests/samples/esbmc_output/line_test/vdp_1_safe.c-amalgamation-28.c` & `esbmc_ai-0.5.0.dev9/tests/samples/esbmc_output/line_test/vdp_1_safe.c-amalgamation-28.c`

 * *Files identical despite different names*

### Comparing `esbmc_ai-0.5.0.dev8/.gitignore` & `esbmc_ai-0.5.0.dev9/.gitignore`

 * *Files identical despite different names*

### Comparing `esbmc_ai-0.5.0.dev8/LICENSE` & `esbmc_ai-0.5.0.dev9/LICENSE`

 * *Files identical despite different names*

### Comparing `esbmc_ai-0.5.0.dev8/README.md` & `esbmc_ai-0.5.0.dev9/README.md`

 * *Files identical despite different names*

### Comparing `esbmc_ai-0.5.0.dev8/pyproject.toml` & `esbmc_ai-0.5.0.dev9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `esbmc_ai-0.5.0.dev8/PKG-INFO` & `esbmc_ai-0.5.0.dev9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: esbmc_ai
-Version: 0.5.0.dev8
+Version: 0.5.0.dev9
 Summary: LLM driven development and automatic repair kit.
 Project-URL: Homepage, https://github.com/Yiannis128/esbmc-ai
 Project-URL: Source Code, https://github.com/Yiannis128/esbmc-ai
 Project-URL: Documentation, https://github.com/Yiannis128/esbmc-ai/wiki
 Project-URL: Issues, https://github.com/Yiannis128/esbmc-ai/issues
 Author-email: Yiannis Charalambous <yiannis128@hotmail.com>
 License-File: LICENSE
```

