# Comparing `tmp/sirji-messages-0.0.2.tar.gz` & `tmp/sirji-messages-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sirji-messages-0.0.2.tar", last modified: Tue Apr  2 13:14:05 2024, max compression
+gzip compressed data, was "sirji-messages-0.0.3.tar", last modified: Wed Apr  3 15:11:57 2024, max compression
```

## Comparing `sirji-messages-0.0.2.tar` & `sirji-messages-0.0.3.tar`

### file list

```diff
@@ -1,70 +1,70 @@
-drwxr-xr-x   0 kedarchandrayan   (501) staff       (20)        0 2024-04-02 13:14:05.778352 sirji-messages-0.0.2/
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)     1069 2024-04-02 13:13:47.000000 sirji-messages-0.0.2/LICENSE
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)        0 2024-04-02 13:13:47.000000 sirji-messages-0.0.2/MANIFEST.in
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)     3753 2024-04-02 13:14:05.777891 sirji-messages-0.0.2/PKG-INFO
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)     3522 2024-04-02 13:13:47.000000 sirji-messages-0.0.2/README.md
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)       38 2024-04-02 13:14:05.778451 sirji-messages-0.0.2/setup.cfg
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)      633 2024-04-02 13:13:47.000000 sirji-messages-0.0.2/setup.py
-drwxr-xr-x   0 kedarchandrayan   (501) staff       (20)        0 2024-04-02 13:14:05.751480 sirji-messages-0.0.2/sirji_messages/
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)      591 2024-04-02 13:13:47.000000 sirji-messages-0.0.2/sirji_messages/__init__.py
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)      565 2024-04-02 13:13:47.000000 sirji-messages-0.0.2/sirji_messages/action_enum.py
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)      377 2024-04-02 13:13:47.000000 sirji-messages-0.0.2/sirji_messages/agent_enum.py
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)      476 2024-04-02 13:13:47.000000 sirji-messages-0.0.2/sirji_messages/custom_exceptions.py
-drwxr-xr-x   0 kedarchandrayan   (501) staff       (20)        0 2024-04-02 13:14:05.754078 sirji-messages-0.0.2/sirji_messages/messages/
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)        0 2024-04-02 13:13:47.000000 sirji-messages-0.0.2/sirji_messages/messages/__init__.py
-drwxr-xr-x   0 kedarchandrayan   (501) staff       (20)        0 2024-04-02 13:14:05.766441 sirji-messages-0.0.2/sirji_messages/messages/actions/
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)        0 2024-04-02 13:13:47.000000 sirji-messages-0.0.2/sirji_messages/messages/actions/__init__.py
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)      654 2024-04-02 13:13:47.000000 sirji-messages-0.0.2/sirji_messages/messages/actions/acknowledge.py
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)      723 2024-04-02 13:13:47.000000 sirji-messages-0.0.2/sirji_messages/messages/actions/answer.py
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)     1152 2024-04-02 13:13:47.000000 sirji-messages-0.0.2/sirji_messages/messages/actions/base.py
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)      866 2024-04-02 13:13:47.000000 sirji-messages-0.0.2/sirji_messages/messages/actions/create_file.py
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)      713 2024-04-02 13:13:47.000000 sirji-messages-0.0.2/sirji_messages/messages/actions/execute_command.py
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)      724 2024-04-02 13:13:47.000000 sirji-messages-0.0.2/sirji_messages/messages/actions/feedback.py
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)      744 2024-04-02 13:13:47.000000 sirji-messages-0.0.2/sirji_messages/messages/actions/generate_steps.py
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)      798 2024-04-02 13:13:47.000000 sirji-messages-0.0.2/sirji_messages/messages/actions/infer.py
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)      731 2024-04-02 13:13:47.000000 sirji-messages-0.0.2/sirji_messages/messages/actions/inform.py
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)      747 2024-04-02 13:13:47.000000 sirji-messages-0.0.2/sirji_messages/messages/actions/install_package.py
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)      706 2024-04-02 13:13:47.000000 sirji-messages-0.0.2/sirji_messages/messages/actions/output.py
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)      809 2024-04-02 13:13:47.000000 sirji-messages-0.0.2/sirji_messages/messages/actions/problem_statement.py
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)      775 2024-04-02 13:13:47.000000 sirji-messages-0.0.2/sirji_messages/messages/actions/question.py
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)      712 2024-04-02 13:13:47.000000 sirji-messages-0.0.2/sirji_messages/messages/actions/response.py
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)      786 2024-04-02 13:13:47.000000 sirji-messages-0.0.2/sirji_messages/messages/actions/solution_complete.py
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)      765 2024-04-02 13:13:47.000000 sirji-messages-0.0.2/sirji_messages/messages/actions/step_completed.py
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)      738 2024-04-02 13:13:47.000000 sirji-messages-0.0.2/sirji_messages/messages/actions/step_started.py
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)      784 2024-04-02 13:13:47.000000 sirji-messages-0.0.2/sirji_messages/messages/actions/steps.py
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)      759 2024-04-02 13:13:47.000000 sirji-messages-0.0.2/sirji_messages/messages/actions/train_using_search_term.py
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)      750 2024-04-02 13:13:47.000000 sirji-messages-0.0.2/sirji_messages/messages/actions/train_using_url.py
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)      732 2024-04-02 13:13:47.000000 sirji-messages-0.0.2/sirji_messages/messages/actions/training_output.py
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)     2668 2024-04-02 13:13:47.000000 sirji-messages-0.0.2/sirji_messages/messages/factory.py
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)     3351 2024-04-02 13:13:47.000000 sirji-messages-0.0.2/sirji_messages/parser.py
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)     2335 2024-04-02 13:13:47.000000 sirji-messages-0.0.2/sirji_messages/permissions.py
-drwxr-xr-x   0 kedarchandrayan   (501) staff       (20)        0 2024-04-02 13:14:05.767258 sirji-messages-0.0.2/sirji_messages/system_prompts/
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)        0 2024-04-02 13:13:47.000000 sirji-messages-0.0.2/sirji_messages/system_prompts/__init__.py
-drwxr-xr-x   0 kedarchandrayan   (501) staff       (20)        0 2024-04-02 13:14:05.771062 sirji-messages-0.0.2/sirji_messages/system_prompts/agents/
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)        0 2024-04-02 13:13:47.000000 sirji-messages-0.0.2/sirji_messages/system_prompts/agents/__init__.py
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)     4447 2024-04-02 13:13:47.000000 sirji-messages-0.0.2/sirji_messages/system_prompts/agents/base.py
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)     2469 2024-04-02 13:13:47.000000 sirji-messages-0.0.2/sirji_messages/system_prompts/agents/coder.py
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)      822 2024-04-02 13:13:47.000000 sirji-messages-0.0.2/sirji_messages/system_prompts/agents/executor.py
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)     1568 2024-04-02 13:13:47.000000 sirji-messages-0.0.2/sirji_messages/system_prompts/agents/planner.py
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)      755 2024-04-02 13:13:47.000000 sirji-messages-0.0.2/sirji_messages/system_prompts/agents/researcher.py
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)      883 2024-04-02 13:13:47.000000 sirji-messages-0.0.2/sirji_messages/system_prompts/agents/user.py
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)     1111 2024-04-02 13:13:47.000000 sirji-messages-0.0.2/sirji_messages/system_prompts/factory.py
-drwxr-xr-x   0 kedarchandrayan   (501) staff       (20)        0 2024-04-02 13:14:05.777394 sirji-messages-0.0.2/sirji_messages.egg-info/
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)     3753 2024-04-02 13:14:05.000000 sirji-messages-0.0.2/sirji_messages.egg-info/PKG-INFO
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)     2240 2024-04-02 13:14:05.000000 sirji-messages-0.0.2/sirji_messages.egg-info/SOURCES.txt
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)        1 2024-04-02 13:14:05.000000 sirji-messages-0.0.2/sirji_messages.egg-info/dependency_links.txt
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)       21 2024-04-02 13:14:05.000000 sirji-messages-0.0.2/sirji_messages.egg-info/top_level.txt
-drwxr-xr-x   0 kedarchandrayan   (501) staff       (20)        0 2024-04-02 13:14:05.771638 sirji-messages-0.0.2/tests/
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)        0 2024-04-02 13:13:47.000000 sirji-messages-0.0.2/tests/__init__.py
-drwxr-xr-x   0 kedarchandrayan   (501) staff       (20)        0 2024-04-02 13:14:05.773225 sirji-messages-0.0.2/tests/integration/
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)        0 2024-04-02 13:13:47.000000 sirji-messages-0.0.2/tests/integration/__init__.py
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)     1454 2024-04-02 13:13:47.000000 sirji-messages-0.0.2/tests/integration/test_message_factory.py
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)     1806 2024-04-02 13:13:47.000000 sirji-messages-0.0.2/tests/integration/test_system_prompts.py
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)      814 2024-04-02 13:13:47.000000 sirji-messages-0.0.2/tests/integration/test_system_prompts_base.py
-drwxr-xr-x   0 kedarchandrayan   (501) staff       (20)        0 2024-04-02 13:14:05.776698 sirji-messages-0.0.2/tests/unit/
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)        0 2024-04-02 13:13:47.000000 sirji-messages-0.0.2/tests/unit/__init__.py
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)      900 2024-04-02 13:13:47.000000 sirji-messages-0.0.2/tests/unit/test_actions_base.py
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)      633 2024-04-02 13:13:47.000000 sirji-messages-0.0.2/tests/unit/test_custom_exceptions.py
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)     1266 2024-04-02 13:13:47.000000 sirji-messages-0.0.2/tests/unit/test_enums.py
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)     2479 2024-04-02 13:13:47.000000 sirji-messages-0.0.2/tests/unit/test_parser.py
--rw-r--r--   0 kedarchandrayan   (501) staff       (20)     1609 2024-04-02 13:13:47.000000 sirji-messages-0.0.2/tests/unit/test_permissions.py
+drwxr-xr-x   0 kedarchandrayan   (501) staff       (20)        0 2024-04-03 15:11:57.580144 sirji-messages-0.0.3/
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)     1069 2024-04-03 15:11:16.000000 sirji-messages-0.0.3/LICENSE
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)        0 2024-04-03 15:11:16.000000 sirji-messages-0.0.3/MANIFEST.in
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)     3854 2024-04-03 15:11:57.578682 sirji-messages-0.0.3/PKG-INFO
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)     3561 2024-04-03 15:11:16.000000 sirji-messages-0.0.3/README.md
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)       38 2024-04-03 15:11:57.580371 sirji-messages-0.0.3/setup.cfg
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)      695 2024-04-03 15:11:16.000000 sirji-messages-0.0.3/setup.py
+drwxr-xr-x   0 kedarchandrayan   (501) staff       (20)        0 2024-04-03 15:11:57.542204 sirji-messages-0.0.3/sirji_messages/
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)      591 2024-04-03 15:11:16.000000 sirji-messages-0.0.3/sirji_messages/__init__.py
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)      565 2024-04-03 15:11:16.000000 sirji-messages-0.0.3/sirji_messages/action_enum.py
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)      377 2024-04-03 15:11:16.000000 sirji-messages-0.0.3/sirji_messages/agent_enum.py
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)      476 2024-04-03 15:11:16.000000 sirji-messages-0.0.3/sirji_messages/custom_exceptions.py
+drwxr-xr-x   0 kedarchandrayan   (501) staff       (20)        0 2024-04-03 15:11:57.544950 sirji-messages-0.0.3/sirji_messages/messages/
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)        0 2024-04-03 15:11:16.000000 sirji-messages-0.0.3/sirji_messages/messages/__init__.py
+drwxr-xr-x   0 kedarchandrayan   (501) staff       (20)        0 2024-04-03 15:11:57.558123 sirji-messages-0.0.3/sirji_messages/messages/actions/
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)        0 2024-04-03 15:11:16.000000 sirji-messages-0.0.3/sirji_messages/messages/actions/__init__.py
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)      654 2024-04-03 15:11:16.000000 sirji-messages-0.0.3/sirji_messages/messages/actions/acknowledge.py
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)      723 2024-04-03 15:11:16.000000 sirji-messages-0.0.3/sirji_messages/messages/actions/answer.py
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)     1152 2024-04-03 15:11:16.000000 sirji-messages-0.0.3/sirji_messages/messages/actions/base.py
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)      866 2024-04-03 15:11:16.000000 sirji-messages-0.0.3/sirji_messages/messages/actions/create_file.py
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)      713 2024-04-03 15:11:16.000000 sirji-messages-0.0.3/sirji_messages/messages/actions/execute_command.py
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)      724 2024-04-03 15:11:16.000000 sirji-messages-0.0.3/sirji_messages/messages/actions/feedback.py
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)      744 2024-04-03 15:11:16.000000 sirji-messages-0.0.3/sirji_messages/messages/actions/generate_steps.py
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)      798 2024-04-03 15:11:16.000000 sirji-messages-0.0.3/sirji_messages/messages/actions/infer.py
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)      731 2024-04-03 15:11:16.000000 sirji-messages-0.0.3/sirji_messages/messages/actions/inform.py
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)      747 2024-04-03 15:11:16.000000 sirji-messages-0.0.3/sirji_messages/messages/actions/install_package.py
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)      706 2024-04-03 15:11:16.000000 sirji-messages-0.0.3/sirji_messages/messages/actions/output.py
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)      809 2024-04-03 15:11:16.000000 sirji-messages-0.0.3/sirji_messages/messages/actions/problem_statement.py
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)      775 2024-04-03 15:11:16.000000 sirji-messages-0.0.3/sirji_messages/messages/actions/question.py
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)      712 2024-04-03 15:11:16.000000 sirji-messages-0.0.3/sirji_messages/messages/actions/response.py
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)      786 2024-04-03 15:11:16.000000 sirji-messages-0.0.3/sirji_messages/messages/actions/solution_complete.py
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)      765 2024-04-03 15:11:16.000000 sirji-messages-0.0.3/sirji_messages/messages/actions/step_completed.py
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)      738 2024-04-03 15:11:16.000000 sirji-messages-0.0.3/sirji_messages/messages/actions/step_started.py
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)      784 2024-04-03 15:11:16.000000 sirji-messages-0.0.3/sirji_messages/messages/actions/steps.py
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)      759 2024-04-03 15:11:16.000000 sirji-messages-0.0.3/sirji_messages/messages/actions/train_using_search_term.py
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)      750 2024-04-03 15:11:16.000000 sirji-messages-0.0.3/sirji_messages/messages/actions/train_using_url.py
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)      732 2024-04-03 15:11:16.000000 sirji-messages-0.0.3/sirji_messages/messages/actions/training_output.py
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)     2668 2024-04-03 15:11:16.000000 sirji-messages-0.0.3/sirji_messages/messages/factory.py
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)     3351 2024-04-03 15:11:16.000000 sirji-messages-0.0.3/sirji_messages/parser.py
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)     2335 2024-04-03 15:11:16.000000 sirji-messages-0.0.3/sirji_messages/permissions.py
+drwxr-xr-x   0 kedarchandrayan   (501) staff       (20)        0 2024-04-03 15:11:57.558972 sirji-messages-0.0.3/sirji_messages/system_prompts/
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)        0 2024-04-03 15:11:16.000000 sirji-messages-0.0.3/sirji_messages/system_prompts/__init__.py
+drwxr-xr-x   0 kedarchandrayan   (501) staff       (20)        0 2024-04-03 15:11:57.564154 sirji-messages-0.0.3/sirji_messages/system_prompts/agents/
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)        0 2024-04-03 15:11:16.000000 sirji-messages-0.0.3/sirji_messages/system_prompts/agents/__init__.py
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)     4447 2024-04-03 15:11:16.000000 sirji-messages-0.0.3/sirji_messages/system_prompts/agents/base.py
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)     2469 2024-04-03 15:11:16.000000 sirji-messages-0.0.3/sirji_messages/system_prompts/agents/coder.py
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)      822 2024-04-03 15:11:16.000000 sirji-messages-0.0.3/sirji_messages/system_prompts/agents/executor.py
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)     1568 2024-04-03 15:11:16.000000 sirji-messages-0.0.3/sirji_messages/system_prompts/agents/planner.py
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)      755 2024-04-03 15:11:16.000000 sirji-messages-0.0.3/sirji_messages/system_prompts/agents/researcher.py
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)      883 2024-04-03 15:11:16.000000 sirji-messages-0.0.3/sirji_messages/system_prompts/agents/user.py
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)     1111 2024-04-03 15:11:16.000000 sirji-messages-0.0.3/sirji_messages/system_prompts/factory.py
+drwxr-xr-x   0 kedarchandrayan   (501) staff       (20)        0 2024-04-03 15:11:57.577353 sirji-messages-0.0.3/sirji_messages.egg-info/
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)     3854 2024-04-03 15:11:57.000000 sirji-messages-0.0.3/sirji_messages.egg-info/PKG-INFO
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)     2240 2024-04-03 15:11:57.000000 sirji-messages-0.0.3/sirji_messages.egg-info/SOURCES.txt
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)        1 2024-04-03 15:11:57.000000 sirji-messages-0.0.3/sirji_messages.egg-info/dependency_links.txt
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)       21 2024-04-03 15:11:57.000000 sirji-messages-0.0.3/sirji_messages.egg-info/top_level.txt
+drwxr-xr-x   0 kedarchandrayan   (501) staff       (20)        0 2024-04-03 15:11:57.565100 sirji-messages-0.0.3/tests/
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)        0 2024-04-03 15:11:16.000000 sirji-messages-0.0.3/tests/__init__.py
+drwxr-xr-x   0 kedarchandrayan   (501) staff       (20)        0 2024-04-03 15:11:57.567975 sirji-messages-0.0.3/tests/integration/
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)        0 2024-04-03 15:11:16.000000 sirji-messages-0.0.3/tests/integration/__init__.py
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)     1454 2024-04-03 15:11:16.000000 sirji-messages-0.0.3/tests/integration/test_message_factory.py
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)     1806 2024-04-03 15:11:16.000000 sirji-messages-0.0.3/tests/integration/test_system_prompts.py
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)      814 2024-04-03 15:11:16.000000 sirji-messages-0.0.3/tests/integration/test_system_prompts_base.py
+drwxr-xr-x   0 kedarchandrayan   (501) staff       (20)        0 2024-04-03 15:11:57.574284 sirji-messages-0.0.3/tests/unit/
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)        0 2024-04-03 15:11:16.000000 sirji-messages-0.0.3/tests/unit/__init__.py
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)      900 2024-04-03 15:11:16.000000 sirji-messages-0.0.3/tests/unit/test_actions_base.py
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)      633 2024-04-03 15:11:16.000000 sirji-messages-0.0.3/tests/unit/test_custom_exceptions.py
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)     1266 2024-04-03 15:11:16.000000 sirji-messages-0.0.3/tests/unit/test_enums.py
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)     2479 2024-04-03 15:11:16.000000 sirji-messages-0.0.3/tests/unit/test_parser.py
+-rw-r--r--   0 kedarchandrayan   (501) staff       (20)     1609 2024-04-03 15:11:16.000000 sirji-messages-0.0.3/tests/unit/test_permissions.py
```

### Comparing `sirji-messages-0.0.2/LICENSE` & `sirji-messages-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `sirji-messages-0.0.2/PKG-INFO` & `sirji-messages-0.0.3/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,7 @@
-Metadata-Version: 2.1
-Name: sirji-messages
-Version: 0.0.2
-Summary: Message Mediator.
-Home-page: https://github.com/sirji-ai/sirji
-Author: Sirji
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # sirji-messages
 
 `sirji-messages` is a comprehensive Python package for creating, parsing, validating, and managing message interactions based on permissions in multi-agent systems or applications.
 
 ## Installation
 
 ```bash
@@ -98,15 +88,16 @@
 from sirji_messages import MessageFactory, ActionEnum, AgentSystemPromptFactory, AgentEnum
 
 # Message class instantiation from an action enum
 message_class = MessageFactory[ActionEnum.INFORM.name]
 print(f"Sample INFORM message:\n{message_class().sample()}")
 
 # Generate message using passed template variables
-print(f"Generated INFORM message:\n"{message_class().generate({"details": "Some sample information."})}")
+generated_messages = message_class().generate({"details": "Some sample information."})
+print(f"Generated INFORM message:\n{generated_messages}")
 
 # System prompt class instantiation from an agent enum
 prompt_class = AgentSystemPromptFactory[AgentEnum.CODER.name]
 print(f"CODER system prompt: {prompt_class().system_prompt()}")
 ```
 
 ## Running Tests and Coverage Analysis
@@ -123,8 +114,8 @@
 # Measure coverage, excluding test files
 coverage run --omit="tests/*" -m pytest
 coverage report
 ```
 
 ## License
 
-Distributed under the MIT License. See `LICENSE` for more information.
+Distributed under the MIT License. See `LICENSE` for more information.
```

### Comparing `sirji-messages-0.0.2/README.md` & `sirji-messages-0.0.3/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,7 +1,17 @@
+Metadata-Version: 2.1
+Name: sirji-messages
+Version: 0.0.3
+Summary: Sirji messaging protocol implementation to create, validate and parse messages.
+Home-page: https://github.com/sirji-ai/sirji
+Author: Sirji
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # sirji-messages
 
 `sirji-messages` is a comprehensive Python package for creating, parsing, validating, and managing message interactions based on permissions in multi-agent systems or applications.
 
 ## Installation
 
 ```bash
@@ -88,15 +98,16 @@
 from sirji_messages import MessageFactory, ActionEnum, AgentSystemPromptFactory, AgentEnum
 
 # Message class instantiation from an action enum
 message_class = MessageFactory[ActionEnum.INFORM.name]
 print(f"Sample INFORM message:\n{message_class().sample()}")
 
 # Generate message using passed template variables
-print(f"Generated INFORM message:\n"{message_class().generate({"details": "Some sample information."})}")
+generated_messages = message_class().generate({"details": "Some sample information."})
+print(f"Generated INFORM message:\n{generated_messages}")
 
 # System prompt class instantiation from an agent enum
 prompt_class = AgentSystemPromptFactory[AgentEnum.CODER.name]
 print(f"CODER system prompt: {prompt_class().system_prompt()}")
 ```
 
 ## Running Tests and Coverage Analysis
@@ -113,8 +124,8 @@
 # Measure coverage, excluding test files
 coverage run --omit="tests/*" -m pytest
 coverage report
 ```
 
 ## License
 
-Distributed under the MIT License. See `LICENSE` for more information.
+Distributed under the MIT License. See `LICENSE` for more information.
```

### Comparing `sirji-messages-0.0.2/setup.py` & `sirji-messages-0.0.3/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup, find_packages
 
 setup(
     name='sirji-messages',
-    version='0.0.2',
+    version='0.0.3',
     author='Sirji',
-    description='Message Mediator.',
+    description='Sirji messaging protocol implementation to create, validate and parse messages.',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/sirji-ai/sirji',
     packages=find_packages(),
     include_package_data=True,  # This includes non-code files specified in MANIFEST.in
     install_requires=[
         x for x in open("./requirements.txt", "r+").readlines() if x.strip()
```

### Comparing `sirji-messages-0.0.2/sirji_messages/__init__.py` & `sirji-messages-0.0.3/sirji_messages/__init__.py`

 * *Files identical despite different names*

### Comparing `sirji-messages-0.0.2/sirji_messages/action_enum.py` & `sirji-messages-0.0.3/sirji_messages/action_enum.py`

 * *Files identical despite different names*

### Comparing `sirji-messages-0.0.2/sirji_messages/messages/actions/acknowledge.py` & `sirji-messages-0.0.3/sirji_messages/messages/actions/acknowledge.py`

 * *Files identical despite different names*

### Comparing `sirji-messages-0.0.2/sirji_messages/messages/actions/answer.py` & `sirji-messages-0.0.3/sirji_messages/messages/actions/answer.py`

 * *Files identical despite different names*

### Comparing `sirji-messages-0.0.2/sirji_messages/messages/actions/base.py` & `sirji-messages-0.0.3/sirji_messages/messages/actions/base.py`

 * *Files identical despite different names*

### Comparing `sirji-messages-0.0.2/sirji_messages/messages/actions/create_file.py` & `sirji-messages-0.0.3/sirji_messages/messages/actions/create_file.py`

 * *Files identical despite different names*

### Comparing `sirji-messages-0.0.2/sirji_messages/messages/actions/execute_command.py` & `sirji-messages-0.0.3/sirji_messages/messages/actions/execute_command.py`

 * *Files identical despite different names*

### Comparing `sirji-messages-0.0.2/sirji_messages/messages/actions/feedback.py` & `sirji-messages-0.0.3/sirji_messages/messages/actions/feedback.py`

 * *Files identical despite different names*

### Comparing `sirji-messages-0.0.2/sirji_messages/messages/actions/generate_steps.py` & `sirji-messages-0.0.3/sirji_messages/messages/actions/generate_steps.py`

 * *Files identical despite different names*

### Comparing `sirji-messages-0.0.2/sirji_messages/messages/actions/infer.py` & `sirji-messages-0.0.3/sirji_messages/messages/actions/infer.py`

 * *Files identical despite different names*

### Comparing `sirji-messages-0.0.2/sirji_messages/messages/actions/inform.py` & `sirji-messages-0.0.3/sirji_messages/messages/actions/inform.py`

 * *Files identical despite different names*

### Comparing `sirji-messages-0.0.2/sirji_messages/messages/actions/install_package.py` & `sirji-messages-0.0.3/sirji_messages/messages/actions/install_package.py`

 * *Files identical despite different names*

### Comparing `sirji-messages-0.0.2/sirji_messages/messages/actions/output.py` & `sirji-messages-0.0.3/sirji_messages/messages/actions/output.py`

 * *Files identical despite different names*

### Comparing `sirji-messages-0.0.2/sirji_messages/messages/actions/problem_statement.py` & `sirji-messages-0.0.3/sirji_messages/messages/actions/problem_statement.py`

 * *Files identical despite different names*

### Comparing `sirji-messages-0.0.2/sirji_messages/messages/actions/question.py` & `sirji-messages-0.0.3/sirji_messages/messages/actions/question.py`

 * *Files identical despite different names*

### Comparing `sirji-messages-0.0.2/sirji_messages/messages/actions/response.py` & `sirji-messages-0.0.3/sirji_messages/messages/actions/response.py`

 * *Files identical despite different names*

### Comparing `sirji-messages-0.0.2/sirji_messages/messages/actions/solution_complete.py` & `sirji-messages-0.0.3/sirji_messages/messages/actions/solution_complete.py`

 * *Files identical despite different names*

### Comparing `sirji-messages-0.0.2/sirji_messages/messages/actions/step_completed.py` & `sirji-messages-0.0.3/sirji_messages/messages/actions/step_completed.py`

 * *Files identical despite different names*

### Comparing `sirji-messages-0.0.2/sirji_messages/messages/actions/step_started.py` & `sirji-messages-0.0.3/sirji_messages/messages/actions/step_started.py`

 * *Files identical despite different names*

### Comparing `sirji-messages-0.0.2/sirji_messages/messages/actions/steps.py` & `sirji-messages-0.0.3/sirji_messages/messages/actions/steps.py`

 * *Files identical despite different names*

### Comparing `sirji-messages-0.0.2/sirji_messages/messages/actions/train_using_search_term.py` & `sirji-messages-0.0.3/sirji_messages/messages/actions/train_using_search_term.py`

 * *Files identical despite different names*

### Comparing `sirji-messages-0.0.2/sirji_messages/messages/actions/train_using_url.py` & `sirji-messages-0.0.3/sirji_messages/messages/actions/train_using_url.py`

 * *Files identical despite different names*

### Comparing `sirji-messages-0.0.2/sirji_messages/messages/actions/training_output.py` & `sirji-messages-0.0.3/sirji_messages/messages/actions/training_output.py`

 * *Files identical despite different names*

### Comparing `sirji-messages-0.0.2/sirji_messages/messages/factory.py` & `sirji-messages-0.0.3/sirji_messages/messages/factory.py`

 * *Files identical despite different names*

### Comparing `sirji-messages-0.0.2/sirji_messages/parser.py` & `sirji-messages-0.0.3/sirji_messages/parser.py`

 * *Files identical despite different names*

### Comparing `sirji-messages-0.0.2/sirji_messages/permissions.py` & `sirji-messages-0.0.3/sirji_messages/permissions.py`

 * *Files identical despite different names*

### Comparing `sirji-messages-0.0.2/sirji_messages/system_prompts/agents/base.py` & `sirji-messages-0.0.3/sirji_messages/system_prompts/agents/base.py`

 * *Files identical despite different names*

### Comparing `sirji-messages-0.0.2/sirji_messages/system_prompts/agents/coder.py` & `sirji-messages-0.0.3/sirji_messages/system_prompts/agents/coder.py`

 * *Files identical despite different names*

### Comparing `sirji-messages-0.0.2/sirji_messages/system_prompts/agents/executor.py` & `sirji-messages-0.0.3/sirji_messages/system_prompts/agents/executor.py`

 * *Files identical despite different names*

### Comparing `sirji-messages-0.0.2/sirji_messages/system_prompts/agents/planner.py` & `sirji-messages-0.0.3/sirji_messages/system_prompts/agents/planner.py`

 * *Files identical despite different names*

### Comparing `sirji-messages-0.0.2/sirji_messages/system_prompts/agents/researcher.py` & `sirji-messages-0.0.3/sirji_messages/system_prompts/agents/researcher.py`

 * *Files identical despite different names*

### Comparing `sirji-messages-0.0.2/sirji_messages/system_prompts/agents/user.py` & `sirji-messages-0.0.3/sirji_messages/system_prompts/agents/user.py`

 * *Files identical despite different names*

### Comparing `sirji-messages-0.0.2/sirji_messages/system_prompts/factory.py` & `sirji-messages-0.0.3/sirji_messages/system_prompts/factory.py`

 * *Files identical despite different names*

### Comparing `sirji-messages-0.0.2/sirji_messages.egg-info/PKG-INFO` & `sirji-messages-0.0.3/sirji_messages.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: sirji-messages
-Version: 0.0.2
-Summary: Message Mediator.
+Version: 0.0.3
+Summary: Sirji messaging protocol implementation to create, validate and parse messages.
 Home-page: https://github.com/sirji-ai/sirji
 Author: Sirji
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # sirji-messages
@@ -98,15 +98,16 @@
 from sirji_messages import MessageFactory, ActionEnum, AgentSystemPromptFactory, AgentEnum
 
 # Message class instantiation from an action enum
 message_class = MessageFactory[ActionEnum.INFORM.name]
 print(f"Sample INFORM message:\n{message_class().sample()}")
 
 # Generate message using passed template variables
-print(f"Generated INFORM message:\n"{message_class().generate({"details": "Some sample information."})}")
+generated_messages = message_class().generate({"details": "Some sample information."})
+print(f"Generated INFORM message:\n{generated_messages}")
 
 # System prompt class instantiation from an agent enum
 prompt_class = AgentSystemPromptFactory[AgentEnum.CODER.name]
 print(f"CODER system prompt: {prompt_class().system_prompt()}")
 ```
 
 ## Running Tests and Coverage Analysis
```

### Comparing `sirji-messages-0.0.2/sirji_messages.egg-info/SOURCES.txt` & `sirji-messages-0.0.3/sirji_messages.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `sirji-messages-0.0.2/tests/integration/test_message_factory.py` & `sirji-messages-0.0.3/tests/integration/test_message_factory.py`

 * *Files identical despite different names*

### Comparing `sirji-messages-0.0.2/tests/integration/test_system_prompts.py` & `sirji-messages-0.0.3/tests/integration/test_system_prompts.py`

 * *Files identical despite different names*

### Comparing `sirji-messages-0.0.2/tests/integration/test_system_prompts_base.py` & `sirji-messages-0.0.3/tests/integration/test_system_prompts_base.py`

 * *Files identical despite different names*

### Comparing `sirji-messages-0.0.2/tests/unit/test_actions_base.py` & `sirji-messages-0.0.3/tests/unit/test_actions_base.py`

 * *Files identical despite different names*

### Comparing `sirji-messages-0.0.2/tests/unit/test_custom_exceptions.py` & `sirji-messages-0.0.3/tests/unit/test_custom_exceptions.py`

 * *Files identical despite different names*

### Comparing `sirji-messages-0.0.2/tests/unit/test_enums.py` & `sirji-messages-0.0.3/tests/unit/test_enums.py`

 * *Files identical despite different names*

### Comparing `sirji-messages-0.0.2/tests/unit/test_parser.py` & `sirji-messages-0.0.3/tests/unit/test_parser.py`

 * *Files identical despite different names*

### Comparing `sirji-messages-0.0.2/tests/unit/test_permissions.py` & `sirji-messages-0.0.3/tests/unit/test_permissions.py`

 * *Files identical despite different names*

