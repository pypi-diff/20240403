# Comparing `tmp/neon-skill-instructions-0.1.1a3.tar.gz` & `tmp/neon-skill-instructions-0.1.1a4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neon-skill-instructions-0.1.1a3.tar", last modified: Tue Feb  6 01:04:27 2024, max compression
+gzip compressed data, was "neon-skill-instructions-0.1.1a4.tar", last modified: Wed Apr  3 18:48:16 2024, max compression
```

## Comparing `neon-skill-instructions-0.1.1a3.tar` & `neon-skill-instructions-0.1.1a4.tar`

### file list

```diff
@@ -1,61 +1,61 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 01:04:27.559495 neon-skill-instructions-0.1.1a3/
--rw-r--r--   0 runner    (1001) docker     (127)     1635 2024-02-06 01:04:23.000000 neon-skill-instructions-0.1.1a3/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)      967 2024-02-06 01:04:27.559495 neon-skill-instructions-0.1.1a3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      696 2024-02-06 01:04:23.000000 neon-skill-instructions-0.1.1a3/README.md
--rw-r--r--   0 runner    (1001) docker     (127)    11495 2024-02-06 01:04:23.000000 neon-skill-instructions-0.1.1a3/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7057 2024-02-06 01:04:23.000000 neon-skill-instructions-0.1.1a3/instruction_checks.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 01:04:27.551495 neon-skill-instructions-0.1.1a3/locale/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 01:04:27.555495 neon-skill-instructions-0.1.1a3/locale/en-us/
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-02-06 01:04:23.000000 neon-skill-instructions-0.1.1a3/locale/en-us/cancel.voc
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-02-06 01:04:23.000000 neon-skill-instructions-0.1.1a3/locale/en-us/choose.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-02-06 01:04:23.000000 neon-skill-instructions-0.1.1a3/locale/en-us/file_exists.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-02-06 01:04:23.000000 neon-skill-instructions-0.1.1a3/locale/en-us/finished.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-02-06 01:04:23.000000 neon-skill-instructions-0.1.1a3/locale/en-us/instruction_names.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-02-06 01:04:23.000000 neon-skill-instructions-0.1.1a3/locale/en-us/instructions_keyword.voc
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-02-06 01:04:23.000000 neon-skill-instructions-0.1.1a3/locale/en-us/neon.voc
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-02-06 01:04:23.000000 neon-skill-instructions-0.1.1a3/locale/en-us/no.voc
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-02-06 01:04:23.000000 neon-skill-instructions-0.1.1a3/locale/en-us/no_file.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-02-06 01:04:23.000000 neon-skill-instructions-0.1.1a3/locale/en-us/no_instruction.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-02-06 01:04:23.000000 neon-skill-instructions-0.1.1a3/locale/en-us/repeat.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      106 2024-02-06 01:04:23.000000 neon-skill-instructions-0.1.1a3/locale/en-us/run_instructions.intent
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-02-06 01:04:23.000000 neon-skill-instructions-0.1.1a3/locale/en-us/start.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-02-06 01:04:23.000000 neon-skill-instructions-0.1.1a3/locale/en-us/yes.voc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 01:04:27.555495 neon-skill-instructions-0.1.1a3/locale/pl-pl/
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-02-06 01:04:23.000000 neon-skill-instructions-0.1.1a3/locale/pl-pl/choose.dialog
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-06 01:04:23.000000 neon-skill-instructions-0.1.1a3/locale/pl-pl/file_exists.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-02-06 01:04:23.000000 neon-skill-instructions-0.1.1a3/locale/pl-pl/finished.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-02-06 01:04:23.000000 neon-skill-instructions-0.1.1a3/locale/pl-pl/instruction_names.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-02-06 01:04:23.000000 neon-skill-instructions-0.1.1a3/locale/pl-pl/instructions_keyword.voc
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-02-06 01:04:23.000000 neon-skill-instructions-0.1.1a3/locale/pl-pl/neon.voc
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-02-06 01:04:23.000000 neon-skill-instructions-0.1.1a3/locale/pl-pl/no_file.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-02-06 01:04:23.000000 neon-skill-instructions-0.1.1a3/locale/pl-pl/no_instruction.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-02-06 01:04:23.000000 neon-skill-instructions-0.1.1a3/locale/pl-pl/repeat.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-02-06 01:04:23.000000 neon-skill-instructions-0.1.1a3/locale/pl-pl/run_instructions.intent
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-02-06 01:04:23.000000 neon-skill-instructions-0.1.1a3/locale/pl-pl/start.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-02-06 01:04:23.000000 neon-skill-instructions-0.1.1a3/locale/pl-pl/yes.voc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 01:04:27.555495 neon-skill-instructions-0.1.1a3/locale/uk-uk/
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-02-06 01:04:23.000000 neon-skill-instructions-0.1.1a3/locale/uk-uk/choose.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       74 2024-02-06 01:04:23.000000 neon-skill-instructions-0.1.1a3/locale/uk-uk/file_exists.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-02-06 01:04:23.000000 neon-skill-instructions-0.1.1a3/locale/uk-uk/finished.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-02-06 01:04:23.000000 neon-skill-instructions-0.1.1a3/locale/uk-uk/instruction_names.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       98 2024-02-06 01:04:23.000000 neon-skill-instructions-0.1.1a3/locale/uk-uk/instructions_keyword.voc
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-02-06 01:04:23.000000 neon-skill-instructions-0.1.1a3/locale/uk-uk/neon.voc
--rw-r--r--   0 runner    (1001) docker     (127)       86 2024-02-06 01:04:23.000000 neon-skill-instructions-0.1.1a3/locale/uk-uk/no_file.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-02-06 01:04:23.000000 neon-skill-instructions-0.1.1a3/locale/uk-uk/no_instruction.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-02-06 01:04:23.000000 neon-skill-instructions-0.1.1a3/locale/uk-uk/repeat.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      245 2024-02-06 01:04:23.000000 neon-skill-instructions-0.1.1a3/locale/uk-uk/run_instructions.intent
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-02-06 01:04:23.000000 neon-skill-instructions-0.1.1a3/locale/uk-uk/start.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-02-06 01:04:23.000000 neon-skill-instructions-0.1.1a3/locale/uk-uk/yes.voc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 01:04:27.559495 neon-skill-instructions-0.1.1a3/neon_skill_instructions.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      967 2024-02-06 01:04:27.000000 neon-skill-instructions-0.1.1a3/neon_skill_instructions.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1512 2024-02-06 01:04:27.000000 neon-skill-instructions-0.1.1a3/neon_skill_instructions.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-06 01:04:27.000000 neon-skill-instructions-0.1.1a3/neon_skill_instructions.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-02-06 01:04:27.000000 neon-skill-instructions-0.1.1a3/neon_skill_instructions.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       67 2024-02-06 01:04:27.000000 neon-skill-instructions-0.1.1a3/neon_skill_instructions.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-02-06 01:04:27.000000 neon-skill-instructions-0.1.1a3/neon_skill_instructions.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-06 01:04:27.559495 neon-skill-instructions-0.1.1a3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     4445 2024-02-06 01:04:23.000000 neon-skill-instructions-0.1.1a3/setup.py
--rw-r--r--   0 runner    (1001) docker     (127)     1373 2024-02-06 01:04:23.000000 neon-skill-instructions-0.1.1a3/skill.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-06 01:04:27.559495 neon-skill-instructions-0.1.1a3/test/
--rw-r--r--   0 runner    (1001) docker     (127)     5777 2024-02-06 01:04:23.000000 neon-skill-instructions-0.1.1a3/test/test_skill.py
--rw-r--r--   0 runner    (1001) docker     (127)     1856 2024-02-06 01:04:23.000000 neon-skill-instructions-0.1.1a3/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 18:48:16.045857 neon-skill-instructions-0.1.1a4/
+-rw-r--r--   0 runner    (1001) docker     (127)     1635 2024-04-03 18:48:13.000000 neon-skill-instructions-0.1.1a4/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)      988 2024-04-03 18:48:16.045857 neon-skill-instructions-0.1.1a4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      696 2024-04-03 18:48:13.000000 neon-skill-instructions-0.1.1a4/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)    11508 2024-04-03 18:48:13.000000 neon-skill-instructions-0.1.1a4/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7057 2024-04-03 18:48:13.000000 neon-skill-instructions-0.1.1a4/instruction_checks.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 18:48:16.041857 neon-skill-instructions-0.1.1a4/locale/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 18:48:16.041857 neon-skill-instructions-0.1.1a4/locale/en-us/
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-04-03 18:48:13.000000 neon-skill-instructions-0.1.1a4/locale/en-us/cancel.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-04-03 18:48:13.000000 neon-skill-instructions-0.1.1a4/locale/en-us/choose.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-04-03 18:48:13.000000 neon-skill-instructions-0.1.1a4/locale/en-us/file_exists.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-03 18:48:13.000000 neon-skill-instructions-0.1.1a4/locale/en-us/finished.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-03 18:48:13.000000 neon-skill-instructions-0.1.1a4/locale/en-us/instruction_names.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-03 18:48:13.000000 neon-skill-instructions-0.1.1a4/locale/en-us/instructions_keyword.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-04-03 18:48:13.000000 neon-skill-instructions-0.1.1a4/locale/en-us/neon.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-04-03 18:48:13.000000 neon-skill-instructions-0.1.1a4/locale/en-us/no.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-04-03 18:48:13.000000 neon-skill-instructions-0.1.1a4/locale/en-us/no_file.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-04-03 18:48:13.000000 neon-skill-instructions-0.1.1a4/locale/en-us/no_instruction.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-03 18:48:13.000000 neon-skill-instructions-0.1.1a4/locale/en-us/repeat.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      106 2024-04-03 18:48:13.000000 neon-skill-instructions-0.1.1a4/locale/en-us/run_instructions.intent
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-03 18:48:13.000000 neon-skill-instructions-0.1.1a4/locale/en-us/start.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-03 18:48:13.000000 neon-skill-instructions-0.1.1a4/locale/en-us/yes.voc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 18:48:16.045857 neon-skill-instructions-0.1.1a4/locale/pl-pl/
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-04-03 18:48:13.000000 neon-skill-instructions-0.1.1a4/locale/pl-pl/choose.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 18:48:13.000000 neon-skill-instructions-0.1.1a4/locale/pl-pl/file_exists.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-03 18:48:13.000000 neon-skill-instructions-0.1.1a4/locale/pl-pl/finished.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-03 18:48:13.000000 neon-skill-instructions-0.1.1a4/locale/pl-pl/instruction_names.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-03 18:48:13.000000 neon-skill-instructions-0.1.1a4/locale/pl-pl/instructions_keyword.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-04-03 18:48:13.000000 neon-skill-instructions-0.1.1a4/locale/pl-pl/neon.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-04-03 18:48:13.000000 neon-skill-instructions-0.1.1a4/locale/pl-pl/no_file.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-03 18:48:13.000000 neon-skill-instructions-0.1.1a4/locale/pl-pl/no_instruction.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-03 18:48:13.000000 neon-skill-instructions-0.1.1a4/locale/pl-pl/repeat.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-03 18:48:13.000000 neon-skill-instructions-0.1.1a4/locale/pl-pl/run_instructions.intent
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-04-03 18:48:13.000000 neon-skill-instructions-0.1.1a4/locale/pl-pl/start.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-03 18:48:13.000000 neon-skill-instructions-0.1.1a4/locale/pl-pl/yes.voc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 18:48:16.045857 neon-skill-instructions-0.1.1a4/locale/uk-uk/
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-03 18:48:13.000000 neon-skill-instructions-0.1.1a4/locale/uk-uk/choose.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2024-04-03 18:48:13.000000 neon-skill-instructions-0.1.1a4/locale/uk-uk/file_exists.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-03 18:48:13.000000 neon-skill-instructions-0.1.1a4/locale/uk-uk/finished.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-03 18:48:13.000000 neon-skill-instructions-0.1.1a4/locale/uk-uk/instruction_names.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       98 2024-04-03 18:48:13.000000 neon-skill-instructions-0.1.1a4/locale/uk-uk/instructions_keyword.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-04-03 18:48:13.000000 neon-skill-instructions-0.1.1a4/locale/uk-uk/neon.voc
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-04-03 18:48:13.000000 neon-skill-instructions-0.1.1a4/locale/uk-uk/no_file.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-03 18:48:13.000000 neon-skill-instructions-0.1.1a4/locale/uk-uk/no_instruction.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-04-03 18:48:13.000000 neon-skill-instructions-0.1.1a4/locale/uk-uk/repeat.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      245 2024-04-03 18:48:13.000000 neon-skill-instructions-0.1.1a4/locale/uk-uk/run_instructions.intent
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-03 18:48:13.000000 neon-skill-instructions-0.1.1a4/locale/uk-uk/start.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-04-03 18:48:13.000000 neon-skill-instructions-0.1.1a4/locale/uk-uk/yes.voc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 18:48:16.045857 neon-skill-instructions-0.1.1a4/neon_skill_instructions.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      988 2024-04-03 18:48:16.000000 neon-skill-instructions-0.1.1a4/neon_skill_instructions.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1512 2024-04-03 18:48:16.000000 neon-skill-instructions-0.1.1a4/neon_skill_instructions.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 18:48:16.000000 neon-skill-instructions-0.1.1a4/neon_skill_instructions.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-04-03 18:48:16.000000 neon-skill-instructions-0.1.1a4/neon_skill_instructions.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      136 2024-04-03 18:48:16.000000 neon-skill-instructions-0.1.1a4/neon_skill_instructions.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-03 18:48:16.000000 neon-skill-instructions-0.1.1a4/neon_skill_instructions.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-03 18:48:16.045857 neon-skill-instructions-0.1.1a4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     4517 2024-04-03 18:48:13.000000 neon-skill-instructions-0.1.1a4/setup.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1410 2024-04-03 18:48:13.000000 neon-skill-instructions-0.1.1a4/skill.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 18:48:16.045857 neon-skill-instructions-0.1.1a4/test/
+-rw-r--r--   0 runner    (1001) docker     (127)     4575 2024-04-03 18:48:13.000000 neon-skill-instructions-0.1.1a4/test/test_skill.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1856 2024-04-03 18:48:13.000000 neon-skill-instructions-0.1.1a4/version.py
```

### Comparing `neon-skill-instructions-0.1.1a3/LICENSE.md` & `neon-skill-instructions-0.1.1a4/LICENSE.md`

 * *Files identical despite different names*

### Comparing `neon-skill-instructions-0.1.1a3/PKG-INFO` & `neon-skill-instructions-0.1.1a4/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 Metadata-Version: 2.1
 Name: neon-skill-instructions
-Version: 0.1.1a3
+Version: 0.1.1a4
 Home-page: https://github.com/NeonGeckoCom/skill-instructions
 Author: Neongecko
 Author-email: developers@neon.ai
 License: BSD-3-Clause
 Description-Content-Type: text/markdown
+Provides-Extra: test
 License-File: LICENSE.md
 
 # <img src='https://0000.us/klatchat/app/files/neon_images/icons/neon_skill.png' card_color="#FF8600" width="50" style="vertical-align:bottom">Instructions
 ## Summary
 Neon skill for instructions reading and implementation
 
 ## Description
```

### Comparing `neon-skill-instructions-0.1.1a3/README.md` & `neon-skill-instructions-0.1.1a4/README.md`

 * *Files identical despite different names*

### Comparing `neon-skill-instructions-0.1.1a3/__init__.py` & `neon-skill-instructions-0.1.1a4/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,16 +29,16 @@
 
 import os
 import json
 from neon_utils.skills.neon_skill import NeonSkill
 from ovos_utils import classproperty
 from ovos_utils.log import LOG
 from ovos_utils.process_utils import RuntimeRequirements
-from mycroft.skills.core import intent_file_handler
-from .instruction_checks import Check
+from ovos_workshop.decorators import intent_handler
+from skill_instructions.instruction_checks import Check
 
 
 class InstructionsSkill(NeonSkill):
     def __init__(self, **kwargs):
         NeonSkill.__init__(self, **kwargs)
         self.script_path = os.path.join(os.path.dirname(__file__),
                                         'instructions')
@@ -60,15 +60,15 @@
                                    no_gui_fallback=True)
 
     def initialize(self):
         # When first run or prompt not dismissed, wait for load and prompt user
         if self.settings.get('prompt_on_start'):
             self.bus.once('mycroft.ready', self._start_instructions_prompt)
 
-    @intent_file_handler("run_instructions.intent")
+    @intent_handler("run_instructions.intent")
     def start_instructions_intent(self, message):
         LOG.info(message.data)
 
         self._start_instructions_prompt(message)
         return
 
     def json_reading(self, json_path):
```

### Comparing `neon-skill-instructions-0.1.1a3/instruction_checks.py` & `neon-skill-instructions-0.1.1a4/instruction_checks.py`

 * *Files identical despite different names*

### Comparing `neon-skill-instructions-0.1.1a3/neon_skill_instructions.egg-info/PKG-INFO` & `neon-skill-instructions-0.1.1a4/neon_skill_instructions.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 Metadata-Version: 2.1
 Name: neon-skill-instructions
-Version: 0.1.1a3
+Version: 0.1.1a4
 Home-page: https://github.com/NeonGeckoCom/skill-instructions
 Author: Neongecko
 Author-email: developers@neon.ai
 License: BSD-3-Clause
 Description-Content-Type: text/markdown
+Provides-Extra: test
 License-File: LICENSE.md
 
 # <img src='https://0000.us/klatchat/app/files/neon_images/icons/neon_skill.png' card_color="#FF8600" width="50" style="vertical-align:bottom">Instructions
 ## Summary
 Neon skill for instructions reading and implementation
 
 ## Description
```

### Comparing `neon-skill-instructions-0.1.1a3/neon_skill_instructions.egg-info/SOURCES.txt` & `neon-skill-instructions-0.1.1a4/neon_skill_instructions.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `neon-skill-instructions-0.1.1a3/setup.py` & `neon-skill-instructions-0.1.1a4/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -85,14 +85,15 @@
 
 setup(
     name=f"neon-{SKILL_NAME}",
     version=version,
     url=f'https://github.com/NeonGeckoCom/{SKILL_NAME}',
     license='BSD-3-Clause',
     install_requires=get_requirements("requirements.txt"),
+    extras_require={"test": get_requirements("requirements/test.txt")},
     author='Neongecko',
     author_email='developers@neon.ai',
     long_description=long_description,
     long_description_content_type="text/markdown",
     package_dir={SKILL_PKG: ""},
     packages=[SKILL_PKG],
     package_data={SKILL_PKG: find_resource_files()},
```

### Comparing `neon-skill-instructions-0.1.1a3/test/test_skill.py` & `neon-skill-instructions-0.1.1a4/test/test_skill.py`

 * *Files 16% similar despite different names*

```diff
@@ -22,65 +22,24 @@
 # EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO,
 # PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA,
 # OR PROFITS;  OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF
 # LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING
 # NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS
 # SOFTWARE,  EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
-import shutil
-import unittest
 import pytest
 
-from os import mkdir
-from os.path import dirname, join, exists
+from os.path import dirname, join
 from mock import Mock
-from ovos_utils.messagebus import FakeBus
+from ovos_bus_client.message import Message
 
-from mycroft.skills.skill_loader import SkillLoader
+from neon_minerva.tests.skill_unit_test_base import SkillTestCase
 
-from mycroft_bus_client import Message
-
-
-class TestSkill(unittest.TestCase):
-
-    @classmethod
-    def setUpClass(cls) -> None:
-        bus = FakeBus()
-        bus.run_in_thread()
-        skill_loader = SkillLoader(bus, dirname(dirname(__file__)))
-        skill_loader.load()
-        cls.skill = skill_loader.instance
-
-        # Define a directory to use for testing
-        cls.test_fs = join(dirname(__file__), "skill")
-        if not exists(cls.test_fs):
-            mkdir(cls.test_fs)
-
-        # Override the configuration and fs paths to use the test directory
-        cls.skill.settings_write_path = cls.test_fs
-        cls.skill.file_system.path = cls.test_fs
-        cls.skill._init_settings()
-        cls.skill.initialize()
-
-        # Override speak and speak_dialog to test passed arguments
-        cls.skill.speak = Mock()
-        cls.skill.speak_dialog = Mock()
-
-        # TODO: Put any skill method overrides here
-
-    def setUp(self):
-        self.skill.speak.reset_mock()
-        self.skill.speak_dialog.reset_mock()
-
-        # TODO: Put any cleanup here that runs before each test case
-
-    @classmethod
-    def tearDownClass(cls) -> None:
-        shutil.rmtree(cls.test_fs)
 
+class TestSkill(SkillTestCase):
     def test_en_skill_init(self):
         real_askyesno = self.skill.ask_yesno
         real_execute = self.skill.execute
         real_instruction_selection = self.skill.instruction_selection
         self.skill.ask_yesno = Mock(return_value="yes")
         self.skill.execute = Mock()
         self.skill.instruction_selection = Mock()
```

### Comparing `neon-skill-instructions-0.1.1a3/version.py` & `neon-skill-instructions-0.1.1a4/version.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,8 +22,8 @@
 # EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO,
 # PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA,
 # OR PROFITS;  OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF
 # LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING
 # NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS
 # SOFTWARE,  EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
-__version__ = "0.1.1a3"
+__version__ = "0.1.1a4"
```

