# Comparing `tmp/neon-skill-spelling-1.0.1a1.tar.gz` & `tmp/neon-skill-spelling-1.0.1a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neon-skill-spelling-1.0.1a1.tar", last modified: Mon Feb  5 22:31:17 2024, max compression
+gzip compressed data, was "neon-skill-spelling-1.0.1a2.tar", last modified: Tue Apr  2 22:04:31 2024, max compression
```

## Comparing `neon-skill-spelling-1.0.1a1.tar` & `neon-skill-spelling-1.0.1a2.tar`

### file list

```diff
@@ -1,91 +1,91 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-05 22:31:17.623748 neon-skill-spelling-1.0.1a1/
--rw-r--r--   0 runner    (1001) docker     (127)    11558 2024-02-05 22:31:11.000000 neon-skill-spelling-1.0.1a1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1635 2024-02-05 22:31:11.000000 neon-skill-spelling-1.0.1a1/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)      846 2024-02-05 22:31:17.623748 neon-skill-spelling-1.0.1a1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      562 2024-02-05 22:31:11.000000 neon-skill-spelling-1.0.1a1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     3580 2024-02-05 22:31:11.000000 neon-skill-spelling-1.0.1a1/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-05 22:31:17.615748 neon-skill-spelling-1.0.1a1/neon_skill_spelling.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      846 2024-02-05 22:31:17.000000 neon-skill-spelling-1.0.1a1/neon_skill_spelling.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1087 2024-02-05 22:31:17.000000 neon-skill-spelling-1.0.1a1/neon_skill_spelling.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-05 22:31:17.000000 neon-skill-spelling-1.0.1a1/neon_skill_spelling.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       79 2024-02-05 22:31:17.000000 neon-skill-spelling-1.0.1a1/neon_skill_spelling.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-02-05 22:31:17.000000 neon-skill-spelling-1.0.1a1/neon_skill_spelling.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-02-05 22:31:17.000000 neon-skill-spelling-1.0.1a1/neon_skill_spelling.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-05 22:31:17.615748 neon-skill-spelling-1.0.1a1/regex/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-05 22:31:17.619748 neon-skill-spelling-1.0.1a1/regex/ca-es/
--rw-r--r--   0 runner    (1001) docker     (127)       99 2024-02-05 22:31:11.000000 neon-skill-spelling-1.0.1a1/regex/ca-es/word.rx
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-05 22:31:17.619748 neon-skill-spelling-1.0.1a1/regex/da-dk/
--rw-r--r--   0 runner    (1001) docker     (127)       88 2024-02-05 22:31:11.000000 neon-skill-spelling-1.0.1a1/regex/da-dk/word.rx
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-05 22:31:17.619748 neon-skill-spelling-1.0.1a1/regex/de-de/
--rw-r--r--   0 runner    (1001) docker     (127)      110 2024-02-05 22:31:11.000000 neon-skill-spelling-1.0.1a1/regex/de-de/word.rx
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-05 22:31:17.619748 neon-skill-spelling-1.0.1a1/regex/el-gr/
--rw-r--r--   0 runner    (1001) docker     (127)      117 2024-02-05 22:31:11.000000 neon-skill-spelling-1.0.1a1/regex/el-gr/word.rx
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-05 22:31:17.619748 neon-skill-spelling-1.0.1a1/regex/en-us/
--rw-r--r--   0 runner    (1001) docker     (127)       97 2024-02-05 22:31:11.000000 neon-skill-spelling-1.0.1a1/regex/en-us/word.rx
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-05 22:31:17.619748 neon-skill-spelling-1.0.1a1/regex/es-es/
--rw-r--r--   0 runner    (1001) docker     (127)      101 2024-02-05 22:31:11.000000 neon-skill-spelling-1.0.1a1/regex/es-es/word.rx
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-05 22:31:17.619748 neon-skill-spelling-1.0.1a1/regex/fa-ir/
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-02-05 22:31:11.000000 neon-skill-spelling-1.0.1a1/regex/fa-ir/word.rx
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-05 22:31:17.619748 neon-skill-spelling-1.0.1a1/regex/fr-fr/
--rw-r--r--   0 runner    (1001) docker     (127)       86 2024-02-05 22:31:11.000000 neon-skill-spelling-1.0.1a1/regex/fr-fr/word.rx
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-05 22:31:17.619748 neon-skill-spelling-1.0.1a1/regex/gl-es/
--rw-r--r--   0 runner    (1001) docker     (127)       95 2024-02-05 22:31:11.000000 neon-skill-spelling-1.0.1a1/regex/gl-es/word.rx
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-05 22:31:17.619748 neon-skill-spelling-1.0.1a1/regex/hu-hu/
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-02-05 22:31:11.000000 neon-skill-spelling-1.0.1a1/regex/hu-hu/word.rx
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-05 22:31:17.619748 neon-skill-spelling-1.0.1a1/regex/it-it/
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-02-05 22:31:11.000000 neon-skill-spelling-1.0.1a1/regex/it-it/word.rx
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-05 22:31:17.619748 neon-skill-spelling-1.0.1a1/regex/nl-nl/
--rw-r--r--   0 runner    (1001) docker     (127)       97 2024-02-05 22:31:11.000000 neon-skill-spelling-1.0.1a1/regex/nl-nl/word.rx
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-05 22:31:17.619748 neon-skill-spelling-1.0.1a1/regex/pl-pl/
--rw-r--r--   0 runner    (1001) docker     (127)       67 2024-02-05 22:31:11.000000 neon-skill-spelling-1.0.1a1/regex/pl-pl/word.rx
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-05 22:31:17.619748 neon-skill-spelling-1.0.1a1/regex/pt-br/
--rw-r--r--   0 runner    (1001) docker     (127)       84 2024-02-05 22:31:11.000000 neon-skill-spelling-1.0.1a1/regex/pt-br/word.rx
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-05 22:31:17.619748 neon-skill-spelling-1.0.1a1/regex/ro-ro/
--rw-r--r--   0 runner    (1001) docker     (127)      109 2024-02-05 22:31:11.000000 neon-skill-spelling-1.0.1a1/regex/ro-ro/word.rx
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-05 22:31:17.619748 neon-skill-spelling-1.0.1a1/regex/ru-ru/
--rw-r--r--   0 runner    (1001) docker     (127)      263 2024-02-05 22:31:11.000000 neon-skill-spelling-1.0.1a1/regex/ru-ru/word.rx
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-05 22:31:17.619748 neon-skill-spelling-1.0.1a1/regex/sv-se/
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-02-05 22:31:11.000000 neon-skill-spelling-1.0.1a1/regex/sv-se/word.rx
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-05 22:31:17.619748 neon-skill-spelling-1.0.1a1/regex/tr-tr/
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-02-05 22:31:11.000000 neon-skill-spelling-1.0.1a1/regex/tr-tr/word.rx
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-05 22:31:17.623748 neon-skill-spelling-1.0.1a1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     4438 2024-02-05 22:31:11.000000 neon-skill-spelling-1.0.1a1/setup.py
--rw-r--r--   0 runner    (1001) docker     (127)     1270 2024-02-05 22:31:11.000000 neon-skill-spelling-1.0.1a1/skill.json
--rw-r--r--   0 runner    (1001) docker     (127)     1856 2024-02-05 22:31:11.000000 neon-skill-spelling-1.0.1a1/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-05 22:31:17.615748 neon-skill-spelling-1.0.1a1/vocab/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-05 22:31:17.619748 neon-skill-spelling-1.0.1a1/vocab/ca-es/
--rw-r--r--   0 runner    (1001) docker     (127)      159 2024-02-05 22:31:11.000000 neon-skill-spelling-1.0.1a1/vocab/ca-es/Spell.voc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-05 22:31:17.619748 neon-skill-spelling-1.0.1a1/vocab/da-dk/
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-02-05 22:31:11.000000 neon-skill-spelling-1.0.1a1/vocab/da-dk/Spell.voc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-05 22:31:17.619748 neon-skill-spelling-1.0.1a1/vocab/de-de/
--rw-r--r--   0 runner    (1001) docker     (127)       74 2024-02-05 22:31:11.000000 neon-skill-spelling-1.0.1a1/vocab/de-de/Spell.voc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-05 22:31:17.619748 neon-skill-spelling-1.0.1a1/vocab/el-gr/
--rw-r--r--   0 runner    (1001) docker     (127)      118 2024-02-05 22:31:11.000000 neon-skill-spelling-1.0.1a1/vocab/el-gr/Spell.voc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-05 22:31:17.619748 neon-skill-spelling-1.0.1a1/vocab/en-us/
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-02-05 22:31:11.000000 neon-skill-spelling-1.0.1a1/vocab/en-us/Spell.voc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-05 22:31:17.619748 neon-skill-spelling-1.0.1a1/vocab/es-es/
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-02-05 22:31:11.000000 neon-skill-spelling-1.0.1a1/vocab/es-es/Spell.voc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-05 22:31:17.619748 neon-skill-spelling-1.0.1a1/vocab/fa-ir/
--rw-r--r--   0 runner    (1001) docker     (127)       56 2024-02-05 22:31:11.000000 neon-skill-spelling-1.0.1a1/vocab/fa-ir/Spell.voc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-05 22:31:17.619748 neon-skill-spelling-1.0.1a1/vocab/fr-fr/
--rw-r--r--   0 runner    (1001) docker     (127)       57 2024-02-05 22:31:11.000000 neon-skill-spelling-1.0.1a1/vocab/fr-fr/Spell.voc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-05 22:31:17.619748 neon-skill-spelling-1.0.1a1/vocab/gl-es/
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-02-05 22:31:11.000000 neon-skill-spelling-1.0.1a1/vocab/gl-es/Spell.voc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-05 22:31:17.623748 neon-skill-spelling-1.0.1a1/vocab/hu-hu/
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-02-05 22:31:11.000000 neon-skill-spelling-1.0.1a1/vocab/hu-hu/Spell.voc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-05 22:31:17.623748 neon-skill-spelling-1.0.1a1/vocab/it-it/
--rw-r--r--   0 runner    (1001) docker     (127)       67 2024-02-05 22:31:11.000000 neon-skill-spelling-1.0.1a1/vocab/it-it/Spell.voc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-05 22:31:17.623748 neon-skill-spelling-1.0.1a1/vocab/nl-nl/
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-02-05 22:31:11.000000 neon-skill-spelling-1.0.1a1/vocab/nl-nl/Spell.voc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-05 22:31:17.623748 neon-skill-spelling-1.0.1a1/vocab/pl-pl/
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-02-05 22:31:11.000000 neon-skill-spelling-1.0.1a1/vocab/pl-pl/Spell.voc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-05 22:31:17.623748 neon-skill-spelling-1.0.1a1/vocab/pt-br/
--rw-r--r--   0 runner    (1001) docker     (127)       64 2024-02-05 22:31:11.000000 neon-skill-spelling-1.0.1a1/vocab/pt-br/Spell.voc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-05 22:31:17.623748 neon-skill-spelling-1.0.1a1/vocab/ro-ro/
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-02-05 22:31:11.000000 neon-skill-spelling-1.0.1a1/vocab/ro-ro/Spell.voc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-05 22:31:17.623748 neon-skill-spelling-1.0.1a1/vocab/ru-ru/
--rw-r--r--   0 runner    (1001) docker     (127)      125 2024-02-05 22:31:11.000000 neon-skill-spelling-1.0.1a1/vocab/ru-ru/Spell.voc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-05 22:31:17.623748 neon-skill-spelling-1.0.1a1/vocab/sv-se/
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-02-05 22:31:11.000000 neon-skill-spelling-1.0.1a1/vocab/sv-se/Spell.voc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-05 22:31:17.623748 neon-skill-spelling-1.0.1a1/vocab/tr-tr/
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-02-05 22:31:11.000000 neon-skill-spelling-1.0.1a1/vocab/tr-tr/Spell.voc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 22:04:31.788978 neon-skill-spelling-1.0.1a2/
+-rw-r--r--   0 runner    (1001) docker     (127)    11558 2024-04-02 22:04:21.000000 neon-skill-spelling-1.0.1a2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1635 2024-04-02 22:04:21.000000 neon-skill-spelling-1.0.1a2/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)      867 2024-04-02 22:04:31.788978 neon-skill-spelling-1.0.1a2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      562 2024-04-02 22:04:21.000000 neon-skill-spelling-1.0.1a2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3603 2024-04-02 22:04:21.000000 neon-skill-spelling-1.0.1a2/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 22:04:31.784978 neon-skill-spelling-1.0.1a2/neon_skill_spelling.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      867 2024-04-02 22:04:31.000000 neon-skill-spelling-1.0.1a2/neon_skill_spelling.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1087 2024-04-02 22:04:31.000000 neon-skill-spelling-1.0.1a2/neon_skill_spelling.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-02 22:04:31.000000 neon-skill-spelling-1.0.1a2/neon_skill_spelling.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-04-02 22:04:31.000000 neon-skill-spelling-1.0.1a2/neon_skill_spelling.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      123 2024-04-02 22:04:31.000000 neon-skill-spelling-1.0.1a2/neon_skill_spelling.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-02 22:04:31.000000 neon-skill-spelling-1.0.1a2/neon_skill_spelling.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 22:04:31.780978 neon-skill-spelling-1.0.1a2/regex/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 22:04:31.784978 neon-skill-spelling-1.0.1a2/regex/ca-es/
+-rw-r--r--   0 runner    (1001) docker     (127)       99 2024-04-02 22:04:21.000000 neon-skill-spelling-1.0.1a2/regex/ca-es/word.rx
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 22:04:31.784978 neon-skill-spelling-1.0.1a2/regex/da-dk/
+-rw-r--r--   0 runner    (1001) docker     (127)       88 2024-04-02 22:04:21.000000 neon-skill-spelling-1.0.1a2/regex/da-dk/word.rx
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 22:04:31.784978 neon-skill-spelling-1.0.1a2/regex/de-de/
+-rw-r--r--   0 runner    (1001) docker     (127)      110 2024-04-02 22:04:21.000000 neon-skill-spelling-1.0.1a2/regex/de-de/word.rx
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 22:04:31.784978 neon-skill-spelling-1.0.1a2/regex/el-gr/
+-rw-r--r--   0 runner    (1001) docker     (127)      117 2024-04-02 22:04:21.000000 neon-skill-spelling-1.0.1a2/regex/el-gr/word.rx
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 22:04:31.784978 neon-skill-spelling-1.0.1a2/regex/en-us/
+-rw-r--r--   0 runner    (1001) docker     (127)       97 2024-04-02 22:04:21.000000 neon-skill-spelling-1.0.1a2/regex/en-us/word.rx
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 22:04:31.784978 neon-skill-spelling-1.0.1a2/regex/es-es/
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-04-02 22:04:21.000000 neon-skill-spelling-1.0.1a2/regex/es-es/word.rx
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 22:04:31.784978 neon-skill-spelling-1.0.1a2/regex/fa-ir/
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-04-02 22:04:21.000000 neon-skill-spelling-1.0.1a2/regex/fa-ir/word.rx
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 22:04:31.784978 neon-skill-spelling-1.0.1a2/regex/fr-fr/
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-04-02 22:04:21.000000 neon-skill-spelling-1.0.1a2/regex/fr-fr/word.rx
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 22:04:31.784978 neon-skill-spelling-1.0.1a2/regex/gl-es/
+-rw-r--r--   0 runner    (1001) docker     (127)       95 2024-04-02 22:04:21.000000 neon-skill-spelling-1.0.1a2/regex/gl-es/word.rx
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 22:04:31.788978 neon-skill-spelling-1.0.1a2/regex/hu-hu/
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-02 22:04:21.000000 neon-skill-spelling-1.0.1a2/regex/hu-hu/word.rx
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 22:04:31.788978 neon-skill-spelling-1.0.1a2/regex/it-it/
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-02 22:04:21.000000 neon-skill-spelling-1.0.1a2/regex/it-it/word.rx
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 22:04:31.788978 neon-skill-spelling-1.0.1a2/regex/nl-nl/
+-rw-r--r--   0 runner    (1001) docker     (127)       97 2024-04-02 22:04:21.000000 neon-skill-spelling-1.0.1a2/regex/nl-nl/word.rx
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 22:04:31.788978 neon-skill-spelling-1.0.1a2/regex/pl-pl/
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-04-02 22:04:21.000000 neon-skill-spelling-1.0.1a2/regex/pl-pl/word.rx
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 22:04:31.788978 neon-skill-spelling-1.0.1a2/regex/pt-br/
+-rw-r--r--   0 runner    (1001) docker     (127)       84 2024-04-02 22:04:21.000000 neon-skill-spelling-1.0.1a2/regex/pt-br/word.rx
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 22:04:31.788978 neon-skill-spelling-1.0.1a2/regex/ro-ro/
+-rw-r--r--   0 runner    (1001) docker     (127)      109 2024-04-02 22:04:21.000000 neon-skill-spelling-1.0.1a2/regex/ro-ro/word.rx
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 22:04:31.788978 neon-skill-spelling-1.0.1a2/regex/ru-ru/
+-rw-r--r--   0 runner    (1001) docker     (127)      263 2024-04-02 22:04:21.000000 neon-skill-spelling-1.0.1a2/regex/ru-ru/word.rx
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 22:04:31.788978 neon-skill-spelling-1.0.1a2/regex/sv-se/
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-04-02 22:04:21.000000 neon-skill-spelling-1.0.1a2/regex/sv-se/word.rx
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 22:04:31.788978 neon-skill-spelling-1.0.1a2/regex/tr-tr/
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-04-02 22:04:21.000000 neon-skill-spelling-1.0.1a2/regex/tr-tr/word.rx
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-02 22:04:31.788978 neon-skill-spelling-1.0.1a2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     4510 2024-04-02 22:04:21.000000 neon-skill-spelling-1.0.1a2/setup.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1345 2024-04-02 22:04:21.000000 neon-skill-spelling-1.0.1a2/skill.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1856 2024-04-02 22:04:21.000000 neon-skill-spelling-1.0.1a2/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 22:04:31.784978 neon-skill-spelling-1.0.1a2/vocab/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 22:04:31.788978 neon-skill-spelling-1.0.1a2/vocab/ca-es/
+-rw-r--r--   0 runner    (1001) docker     (127)      159 2024-04-02 22:04:21.000000 neon-skill-spelling-1.0.1a2/vocab/ca-es/Spell.voc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 22:04:31.788978 neon-skill-spelling-1.0.1a2/vocab/da-dk/
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-02 22:04:21.000000 neon-skill-spelling-1.0.1a2/vocab/da-dk/Spell.voc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 22:04:31.788978 neon-skill-spelling-1.0.1a2/vocab/de-de/
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2024-04-02 22:04:21.000000 neon-skill-spelling-1.0.1a2/vocab/de-de/Spell.voc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 22:04:31.788978 neon-skill-spelling-1.0.1a2/vocab/el-gr/
+-rw-r--r--   0 runner    (1001) docker     (127)      118 2024-04-02 22:04:21.000000 neon-skill-spelling-1.0.1a2/vocab/el-gr/Spell.voc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 22:04:31.788978 neon-skill-spelling-1.0.1a2/vocab/en-us/
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-02 22:04:21.000000 neon-skill-spelling-1.0.1a2/vocab/en-us/Spell.voc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 22:04:31.788978 neon-skill-spelling-1.0.1a2/vocab/es-es/
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-04-02 22:04:21.000000 neon-skill-spelling-1.0.1a2/vocab/es-es/Spell.voc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 22:04:31.788978 neon-skill-spelling-1.0.1a2/vocab/fa-ir/
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-04-02 22:04:21.000000 neon-skill-spelling-1.0.1a2/vocab/fa-ir/Spell.voc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 22:04:31.788978 neon-skill-spelling-1.0.1a2/vocab/fr-fr/
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-02 22:04:21.000000 neon-skill-spelling-1.0.1a2/vocab/fr-fr/Spell.voc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 22:04:31.788978 neon-skill-spelling-1.0.1a2/vocab/gl-es/
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-04-02 22:04:21.000000 neon-skill-spelling-1.0.1a2/vocab/gl-es/Spell.voc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 22:04:31.788978 neon-skill-spelling-1.0.1a2/vocab/hu-hu/
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-04-02 22:04:21.000000 neon-skill-spelling-1.0.1a2/vocab/hu-hu/Spell.voc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 22:04:31.788978 neon-skill-spelling-1.0.1a2/vocab/it-it/
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-04-02 22:04:21.000000 neon-skill-spelling-1.0.1a2/vocab/it-it/Spell.voc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 22:04:31.788978 neon-skill-spelling-1.0.1a2/vocab/nl-nl/
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-02 22:04:21.000000 neon-skill-spelling-1.0.1a2/vocab/nl-nl/Spell.voc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 22:04:31.788978 neon-skill-spelling-1.0.1a2/vocab/pl-pl/
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-02 22:04:21.000000 neon-skill-spelling-1.0.1a2/vocab/pl-pl/Spell.voc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 22:04:31.788978 neon-skill-spelling-1.0.1a2/vocab/pt-br/
+-rw-r--r--   0 runner    (1001) docker     (127)       64 2024-04-02 22:04:21.000000 neon-skill-spelling-1.0.1a2/vocab/pt-br/Spell.voc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 22:04:31.788978 neon-skill-spelling-1.0.1a2/vocab/ro-ro/
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-02 22:04:21.000000 neon-skill-spelling-1.0.1a2/vocab/ro-ro/Spell.voc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 22:04:31.788978 neon-skill-spelling-1.0.1a2/vocab/ru-ru/
+-rw-r--r--   0 runner    (1001) docker     (127)      125 2024-04-02 22:04:21.000000 neon-skill-spelling-1.0.1a2/vocab/ru-ru/Spell.voc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 22:04:31.788978 neon-skill-spelling-1.0.1a2/vocab/sv-se/
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-02 22:04:21.000000 neon-skill-spelling-1.0.1a2/vocab/sv-se/Spell.voc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 22:04:31.788978 neon-skill-spelling-1.0.1a2/vocab/tr-tr/
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-04-02 22:04:21.000000 neon-skill-spelling-1.0.1a2/vocab/tr-tr/Spell.voc
```

### Comparing `neon-skill-spelling-1.0.1a1/LICENSE` & `neon-skill-spelling-1.0.1a2/LICENSE`

 * *Files identical despite different names*

### Comparing `neon-skill-spelling-1.0.1a1/LICENSE.md` & `neon-skill-spelling-1.0.1a2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `neon-skill-spelling-1.0.1a1/PKG-INFO` & `neon-skill-spelling-1.0.1a2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 Metadata-Version: 2.1
 Name: neon-skill-spelling
-Version: 1.0.1a1
+Version: 1.0.1a2
 Home-page: https://github.com/NeonGeckoCom/skill-spelling
 Author: Neongecko
 Author-email: developers@neon.ai
 License: BSD-3-Clause
 Description-Content-Type: text/markdown
+Provides-Extra: test
 License-File: LICENSE
 License-File: LICENSE.md
 
 # <img src='https://raw.githack.com/FortAwesome/Font-Awesome/master/svgs/solid/book-reader.svg' card_color='#22a7f0' width='50' height='50' style='vertical-align:bottom'/> Spelling
 Let Neon help you spell words
 
 ## About
```

### Comparing `neon-skill-spelling-1.0.1a1/README.md` & `neon-skill-spelling-1.0.1a2/README.md`

 * *Files identical despite different names*

### Comparing `neon-skill-spelling-1.0.1a1/__init__.py` & `neon-skill-spelling-1.0.1a2/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -41,15 +41,15 @@
 # limitations under the License.
 
 from neon_utils.skills import NeonSkill
 from adapt.intent import IntentBuilder
 from ovos_utils import classproperty
 from ovos_utils.process_utils import RuntimeRequirements
 
-from mycroft import intent_handler
+from ovos_workshop.decorators import intent_handler
 
 
 class SpellingSkill(NeonSkill):
     @classproperty
     def runtime_requirements(self):
         return RuntimeRequirements(network_before_load=False,
                                    internet_before_load=False,
@@ -57,15 +57,15 @@
                                    requires_internet=False,
                                    requires_network=False,
                                    requires_gui=False,
                                    no_internet_fallback=True,
                                    no_network_fallback=True,
                                    no_gui_fallback=True)
 
-    @intent_handler(IntentBuilder("Spell").require("Spell").require("Word"))
+    @intent_handler(IntentBuilder("SpellIntent").require("Spell").require("Word"))
     def handle_spell(self, message):
         if not self.neon_in_request(message):
             return
         word = message.data.get("Word")
         spelled_word = '; '.join(word).upper()
         self.gui.show_text(word)
         self.speak(spelled_word)
```

### Comparing `neon-skill-spelling-1.0.1a1/neon_skill_spelling.egg-info/PKG-INFO` & `neon-skill-spelling-1.0.1a2/neon_skill_spelling.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 Metadata-Version: 2.1
 Name: neon-skill-spelling
-Version: 1.0.1a1
+Version: 1.0.1a2
 Home-page: https://github.com/NeonGeckoCom/skill-spelling
 Author: Neongecko
 Author-email: developers@neon.ai
 License: BSD-3-Clause
 Description-Content-Type: text/markdown
+Provides-Extra: test
 License-File: LICENSE
 License-File: LICENSE.md
 
 # <img src='https://raw.githack.com/FortAwesome/Font-Awesome/master/svgs/solid/book-reader.svg' card_color='#22a7f0' width='50' height='50' style='vertical-align:bottom'/> Spelling
 Let Neon help you spell words
 
 ## About
```

### Comparing `neon-skill-spelling-1.0.1a1/neon_skill_spelling.egg-info/SOURCES.txt` & `neon-skill-spelling-1.0.1a2/neon_skill_spelling.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `neon-skill-spelling-1.0.1a1/setup.py` & `neon-skill-spelling-1.0.1a2/setup.py`

 * *Files 12% similar despite different names*

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

### Comparing `neon-skill-spelling-1.0.1a1/skill.json` & `neon-skill-spelling-1.0.1a2/skill.json`

 * *Files 16% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.996969696969697%*

 * *Differences: {"'requirements'": "{'python': {insert: [(0, 'adapt-parser<2.0,>=0.5'), (2, 'ovos-utils~=0.0, "*

 * *                   ">=0.0.28'), (3, 'ovos-workshop~=0.0.15')], delete: [1]}}"}*

```diff
@@ -26,16 +26,18 @@
         "x86_64",
         "ia64",
         "arm64",
         "arm"
     ],
     "requirements": {
         "python": [
+            "adapt-parser<2.0,>=0.5",
             "neon-utils~=1.0",
-            "ovos_utils~=0.0, >=0.0.28"
+            "ovos-utils~=0.0, >=0.0.28",
+            "ovos-workshop~=0.0.15"
         ],
         "skill": [],
         "system": {}
     },
     "short_description": "Let Neon help you spell words",
     "skillname": "skill-spelling",
     "summary": "Let Neon help you spell words",
```

### Comparing `neon-skill-spelling-1.0.1a1/version.py` & `neon-skill-spelling-1.0.1a2/version.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,8 +22,8 @@
 # EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO,
 # PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA,
 # OR PROFITS;  OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF
 # LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING
 # NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS
 # SOFTWARE,  EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
-__version__ = "1.0.1a1"
+__version__ = "1.0.1a2"
```

