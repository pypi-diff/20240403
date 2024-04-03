# Comparing `tmp/pynchon-2024.4.3.17.11.tar.gz` & `tmp/pynchon-2024.4.3.17.15.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pynchon-2024.4.3.17.11.tar", last modified: Wed Apr  3 17:11:27 2024, max compression
+gzip compressed data, was "pynchon-2024.4.3.17.15.tar", last modified: Wed Apr  3 17:15:50 2024, max compression
```

## Comparing `pynchon-2024.4.3.17.11.tar` & `pynchon-2024.4.3.17.15.tar`

### file list

```diff
@@ -1,297 +1,297 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:11:27.716485 pynchon-2024.4.3.17.11/
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-04-03 17:06:30.000000 pynchon-2024.4.3.17.11/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1714 2024-04-03 17:11:27.716485 pynchon-2024.4.3.17.11/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2144 2024-04-03 17:06:30.000000 pynchon-2024.4.3.17.11/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      979 2024-04-03 17:06:30.000000 pynchon-2024.4.3.17.11/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1728 2024-04-03 17:11:27.716485 pynchon-2024.4.3.17.11/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      770 2024-04-03 17:06:30.000000 pynchon-2024.4.3.17.11/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:11:27.664485 pynchon-2024.4.3.17.11/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:11:27.676485 pynchon-2024.4.3.17.11/src/pynchon/
--rw-r--r--   0 runner    (1001) docker     (127)      259 2024-04-03 17:06:30.000000 pynchon-2024.4.3.17.11/src/pynchon/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       96 2024-04-03 17:06:30.000000 pynchon-2024.4.3.17.11/src/pynchon/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)       77 2024-04-03 17:11:25.000000 pynchon-2024.4.3.17.11/src/pynchon/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:11:27.680485 pynchon-2024.4.3.17.11/src/pynchon/abcs/
--rw-r--r--   0 runner    (1001) docker     (127)      319 2024-04-03 17:06:30.000000 pynchon-2024.4.3.17.11/src/pynchon/abcs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1503 2024-04-03 17:06:30.000000 pynchon-2024.4.3.17.11/src/pynchon/abcs/attrdict.py
--rw-r--r--   0 runner    (1001) docker     (127)      115 2024-04-03 17:06:30.000000 pynchon-2024.4.3.17.11/src/pynchon/abcs/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     2011 2024-04-03 17:06:30.000000 pynchon-2024.4.3.17.11/src/pynchon/abcs/path.py
--rw-r--r--   0 runner    (1001) docker     (127)     5484 2024-04-03 17:06:30.000000 pynchon-2024.4.3.17.11/src/pynchon/abcs/visitor.py
--rw-r--r--   0 runner    (1001) docker     (127)     5088 2024-04-03 17:07:37.000000 pynchon-2024.4.3.17.11/src/pynchon/annotate.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:11:27.680485 pynchon-2024.4.3.17.11/src/pynchon/api/
--rw-r--r--   0 runner    (1001) docker     (127)       68 2024-04-03 17:06:30.000000 pynchon-2024.4.3.17.11/src/pynchon/api/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:11:27.680485 pynchon-2024.4.3.17.11/src/pynchon/api/git/
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-03 17:06:30.000000 pynchon-2024.4.3.17.11/src/pynchon/api/git/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:11:27.680485 pynchon-2024.4.3.17.11/src/pynchon/api/parsers/
--rw-r--r--   0 runner    (1001) docker     (127)       61 2024-04-03 17:06:30.000000 pynchon-2024.4.3.17.11/src/pynchon/api/parsers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:11:27.680485 pynchon-2024.4.3.17.11/src/pynchon/api/project/
--rw-r--r--   0 runner    (1001) docker     (127)     1203 2024-04-03 17:06:30.000000 pynchon-2024.4.3.17.11/src/pynchon/api/project/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-03 17:06:30.000000 pynchon-2024.4.3.17.11/src/pynchon/api/pynchon.py
--rw-r--r--   0 runner    (1001) docker     (127)     7246 2024-04-03 17:07:37.000000 pynchon-2024.4.3.17.11/src/pynchon/api/render.py
--rw-r--r--   0 runner    (1001) docker     (127)     5262 2024-04-03 17:07:37.000000 pynchon-2024.4.3.17.11/src/pynchon/app.py
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-03 17:06:30.000000 pynchon-2024.4.3.17.11/src/pynchon/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     2606 2024-04-03 17:07:37.000000 pynchon-2024.4.3.17.11/src/pynchon/bin.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:11:27.680485 pynchon-2024.4.3.17.11/src/pynchon/cli/
--rw-r--r--   0 runner    (1001) docker     (127)      128 2024-04-03 17:06:30.000000 pynchon-2024.4.3.17.11/src/pynchon/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5029 2024-04-03 17:07:37.000000 pynchon-2024.4.3.17.11/src/pynchon/cli/common.py
--rw-r--r--   0 runner    (1001) docker     (127)      357 2024-04-03 17:06:30.000000 pynchon-2024.4.3.17.11/src/pynchon/cli/options.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:11:27.680485 pynchon-2024.4.3.17.11/src/pynchon/codemod/
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-03 17:06:30.000000 pynchon-2024.4.3.17.11/src/pynchon/codemod/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:11:27.680485 pynchon-2024.4.3.17.11/src/pynchon/codemod/commands/
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-03 17:06:30.000000 pynchon-2024.4.3.17.11/src/pynchon/codemod/commands/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:11:27.684485 pynchon-2024.4.3.17.11/src/pynchon/codemod/commands/docstrings/
--rw-r--r--   0 runner    (1001) docker     (127)      329 2024-04-03 17:06:30.000000 pynchon-2024.4.3.17.11/src/pynchon/codemod/commands/docstrings/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2564 2024-04-03 17:06:30.000000 pynchon-2024.4.3.17.11/src/pynchon/codemod/commands/docstrings/base.py
--rw-r--r--   0 runner    (1001) docker     (127)      557 2024-04-03 17:06:30.000000 pynchon-2024.4.3.17.11/src/pynchon/codemod/commands/docstrings/javadoc.py
--rw-r--r--   0 runner    (1001) docker     (127)     9607 2024-04-03 17:07:37.000000 pynchon-2024.4.3.17.11/src/pynchon/codemod/commands/docstrings/simple.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:11:27.684485 pynchon-2024.4.3.17.11/src/pynchon/config/
--rw-r--r--   0 runner    (1001) docker     (127)     1865 2024-04-03 17:07:37.000000 pynchon-2024.4.3.17.11/src/pynchon/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5049 2024-04-03 17:07:37.000000 pynchon-2024.4.3.17.11/src/pynchon/config/util.py
--rw-r--r--   0 runner    (1001) docker     (127)     1470 2024-04-03 17:06:30.000000 pynchon-2024.4.3.17.11/src/pynchon/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     3677 2024-04-03 17:06:30.000000 pynchon-2024.4.3.17.11/src/pynchon/core.py
--rw-r--r--   0 runner    (1001) docker     (127)     2376 2024-04-03 17:06:30.000000 pynchon-2024.4.3.17.11/src/pynchon/events.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:11:27.684485 pynchon-2024.4.3.17.11/src/pynchon/models/
--rw-r--r--   0 runner    (1001) docker     (127)      135 2024-04-03 17:06:30.000000 pynchon-2024.4.3.17.11/src/pynchon/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9072 2024-04-03 17:07:37.000000 pynchon-2024.4.3.17.11/src/pynchon/models/planner.py
--rw-r--r--   0 runner    (1001) docker     (127)    12987 2024-04-03 17:07:37.000000 pynchon-2024.4.3.17.11/src/pynchon/models/planning.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:11:27.684485 pynchon-2024.4.3.17.11/src/pynchon/models/plugins/
--rw-r--r--   0 runner    (1001) docker     (127)     1420 2024-04-03 17:06:30.000000 pynchon-2024.4.3.17.11/src/pynchon/models/plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10507 2024-04-03 17:06:30.000000 pynchon-2024.4.3.17.11/src/pynchon/models/plugins/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     2690 2024-04-03 17:07:37.000000 pynchon-2024.4.3.17.11/src/pynchon/models/plugins/docker.py
--rw-r--r--   0 runner    (1001) docker     (127)      606 2024-04-03 17:07:37.000000 pynchon-2024.4.3.17.11/src/pynchon/models/plugins/provider.py
--rw-r--r--   0 runner    (1001) docker     (127)     5752 2024-04-03 17:07:37.000000 pynchon-2024.4.3.17.11/src/pynchon/models/plugins/pynchon.py
--rw-r--r--   0 runner    (1001) docker     (127)      568 2024-04-03 17:06:30.000000 pynchon-2024.4.3.17.11/src/pynchon/models/plugins/tool.py
--rw-r--r--   0 runner    (1001) docker     (127)      959 2024-04-03 17:06:30.000000 pynchon-2024.4.3.17.11/src/pynchon/models/plugins/validators.py
--rw-r--r--   0 runner    (1001) docker     (127)     3027 2024-04-03 17:06:30.000000 pynchon-2024.4.3.17.11/src/pynchon/models/python.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:11:27.692485 pynchon-2024.4.3.17.11/src/pynchon/plugins/
--rw-r--r--   0 runner    (1001) docker     (127)     1025 2024-04-03 17:06:30.000000 pynchon-2024.4.3.17.11/src/pynchon/plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      402 2024-04-03 17:06:30.000000 pynchon-2024.4.3.17.11/src/pynchon/plugins/__template__.py
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-03 17:06:30.000000 pynchon-2024.4.3.17.11/src/pynchon/plugins/api.py
--rw-r--r--   0 runner    (1001) docker     (127)     1520 2024-04-03 17:07:37.000000 pynchon-2024.4.3.17.11/src/pynchon/plugins/cicd.py
--rw-r--r--   0 runner    (1001) docker     (127)     8821 2024-04-03 17:07:37.000000 pynchon-2024.4.3.17.11/src/pynchon/plugins/core.py
--rw-r--r--   0 runner    (1001) docker     (127)     2035 2024-04-03 17:06:30.000000 pynchon-2024.4.3.17.11/src/pynchon/plugins/deck.py
--rw-r--r--   0 runner    (1001) docker     (127)     1036 2024-04-03 17:06:30.000000 pynchon-2024.4.3.17.11/src/pynchon/plugins/dockerhub.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:11:27.692485 pynchon-2024.4.3.17.11/src/pynchon/plugins/docs/
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-03 17:06:30.000000 pynchon-2024.4.3.17.11/src/pynchon/plugins/docs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5152 2024-04-03 17:07:37.000000 pynchon-2024.4.3.17.11/src/pynchon/plugins/docs/main.py
--rw-r--r--   0 runner    (1001) docker     (127)     2072 2024-04-03 17:06:30.000000 pynchon-2024.4.3.17.11/src/pynchon/plugins/docs/opener.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:11:27.692485 pynchon-2024.4.3.17.11/src/pynchon/plugins/doctor/
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-04-03 17:06:30.000000 pynchon-2024.4.3.17.11/src/pynchon/plugins/doctor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2489 2024-04-03 17:07:37.000000 pynchon-2024.4.3.17.11/src/pynchon/plugins/dot.py
--rw-r--r--   0 runner    (1001) docker     (127)     3301 2024-04-03 17:06:30.000000 pynchon-2024.4.3.17.11/src/pynchon/plugins/drawio.py
--rw-r--r--   0 runner    (1001) docker     (127)     3549 2024-04-03 17:07:37.000000 pynchon-2024.4.3.17.11/src/pynchon/plugins/fixme.py
--rw-r--r--   0 runner    (1001) docker     (127)     2902 2024-04-03 17:06:30.000000 pynchon-2024.4.3.17.11/src/pynchon/plugins/gen.py
--rw-r--r--   0 runner    (1001) docker     (127)     4747 2024-04-03 17:06:30.000000 pynchon-2024.4.3.17.11/src/pynchon/plugins/git.py
--rw-r--r--   0 runner    (1001) docker     (127)     4277 2024-04-03 17:06:30.000000 pynchon-2024.4.3.17.11/src/pynchon/plugins/github.py
--rw-r--r--   0 runner    (1001) docker     (127)      401 2024-04-03 17:07:37.000000 pynchon-2024.4.3.17.11/src/pynchon/plugins/globals.py
--rw-r--r--   0 runner    (1001) docker     (127)     1597 2024-04-03 17:06:30.000000 pynchon-2024.4.3.17.11/src/pynchon/plugins/griffe.py
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-03 17:06:30.000000 pynchon-2024.4.3.17.11/src/pynchon/plugins/hooks.py
--rw-r--r--   0 runner    (1001) docker     (127)     4232 2024-04-03 17:07:37.000000 pynchon-2024.4.3.17.11/src/pynchon/plugins/jinja.py
--rw-r--r--   0 runner    (1001) docker     (127)     1507 2024-04-03 17:06:30.000000 pynchon-2024.4.3.17.11/src/pynchon/plugins/json.py
--rw-r--r--   0 runner    (1001) docker     (127)     3954 2024-04-03 17:07:37.000000 pynchon-2024.4.3.17.11/src/pynchon/plugins/makefile.py
--rw-r--r--   0 runner    (1001) docker     (127)     6750 2024-04-03 17:06:30.000000 pynchon-2024.4.3.17.11/src/pynchon/plugins/markdown.py
--rw-r--r--   0 runner    (1001) docker     (127)     2745 2024-04-03 17:06:30.000000 pynchon-2024.4.3.17.11/src/pynchon/plugins/mermaid.py
--rw-r--r--   0 runner    (1001) docker     (127)     8009 2024-04-03 17:07:37.000000 pynchon-2024.4.3.17.11/src/pynchon/plugins/mkdocs.py
--rw-r--r--   0 runner    (1001) docker     (127)     3218 2024-04-03 17:07:37.000000 pynchon-2024.4.3.17.11/src/pynchon/plugins/pandoc.py
--rw-r--r--   0 runner    (1001) docker     (127)      456 2024-04-03 17:06:30.000000 pynchon-2024.4.3.17.11/src/pynchon/plugins/parse.py
--rw-r--r--   0 runner    (1001) docker     (127)    14638 2024-04-03 17:07:37.000000 pynchon-2024.4.3.17.11/src/pynchon/plugins/pattern.py
--rw-r--r--   0 runner    (1001) docker     (127)     1636 2024-04-03 17:07:37.000000 pynchon-2024.4.3.17.11/src/pynchon/plugins/plugins.py
--rw-r--r--   0 runner    (1001) docker     (127)     4044 2024-04-03 17:07:37.000000 pynchon-2024.4.3.17.11/src/pynchon/plugins/project.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:11:27.692485 pynchon-2024.4.3.17.11/src/pynchon/plugins/python/
--rw-r--r--   0 runner    (1001) docker     (127)      145 2024-04-03 17:06:30.000000 pynchon-2024.4.3.17.11/src/pynchon/plugins/python/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3374 2024-04-03 17:06:30.000000 pynchon-2024.4.3.17.11/src/pynchon/plugins/python/api.py
--rw-r--r--   0 runner    (1001) docker     (127)    17560 2024-04-03 17:07:37.000000 pynchon-2024.4.3.17.11/src/pynchon/plugins/python/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-03 17:06:30.000000 pynchon-2024.4.3.17.11/src/pynchon/plugins/python/config.py
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-04-03 17:06:30.000000 pynchon-2024.4.3.17.11/src/pynchon/plugins/python/cst.py
--rw-r--r--   0 runner    (1001) docker     (127)     3509 2024-04-03 17:07:37.000000 pynchon-2024.4.3.17.11/src/pynchon/plugins/python/libcst.py
--rw-r--r--   0 runner    (1001) docker     (127)      236 2024-04-03 17:06:30.000000 pynchon-2024.4.3.17.11/src/pynchon/plugins/python/models.py
--rw-r--r--   0 runner    (1001) docker     (127)     3207 2024-04-03 17:06:30.000000 pynchon-2024.4.3.17.11/src/pynchon/plugins/python/platform.py
--rw-r--r--   0 runner    (1001) docker     (127)      720 2024-04-03 17:06:30.000000 pynchon-2024.4.3.17.11/src/pynchon/plugins/python/pypi.py
--rw-r--r--   0 runner    (1001) docker     (127)      700 2024-04-03 17:06:30.000000 pynchon-2024.4.3.17.11/src/pynchon/plugins/release.py
--rw-r--r--   0 runner    (1001) docker     (127)     1153 2024-04-03 17:07:37.000000 pynchon-2024.4.3.17.11/src/pynchon/plugins/render.py
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-04-03 17:06:30.000000 pynchon-2024.4.3.17.11/src/pynchon/plugins/rtd.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:11:27.692485 pynchon-2024.4.3.17.11/src/pynchon/plugins/scaffolding/
--rw-r--r--   0 runner    (1001) docker     (127)     3784 2024-04-03 17:06:30.000000 pynchon-2024.4.3.17.11/src/pynchon/plugins/scaffolding/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1158 2024-04-03 17:06:30.000000 pynchon-2024.4.3.17.11/src/pynchon/plugins/scaffolding/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     7559 2024-04-03 17:06:30.000000 pynchon-2024.4.3.17.11/src/pynchon/plugins/src.py
--rw-r--r--   0 runner    (1001) docker     (127)     3893 2024-04-03 17:07:37.000000 pynchon-2024.4.3.17.11/src/pynchon/plugins/tests.py
--rw-r--r--   0 runner    (1001) docker     (127)      402 2024-04-03 17:06:30.000000 pynchon-2024.4.3.17.11/src/pynchon/plugins/tox.py
--rw-r--r--   0 runner    (1001) docker     (127)     1445 2024-04-03 17:06:30.000000 pynchon-2024.4.3.17.11/src/pynchon/plugins/util.py
--rw-r--r--   0 runner    (1001) docker     (127)       86 2024-04-03 17:06:30.000000 pynchon-2024.4.3.17.11/src/pynchon/tagging.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:11:27.672485 pynchon-2024.4.3.17.11/src/pynchon/templates/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:11:27.692485 pynchon-2024.4.3.17.11/src/pynchon/templates/docker/
--rw-r--r--   0 runner    (1001) docker     (127)      605 2024-04-03 17:06:30.000000 pynchon-2024.4.3.17.11/src/pynchon/templates/docker/Dockerfile.pandoc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:11:27.692485 pynchon-2024.4.3.17.11/src/pynchon/templates/docs/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 17:06:30.000000 pynchon-2024.4.3.17.11/src/pynchon/templates/docs/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:11:27.668485 pynchon-2024.4.3.17.11/src/pynchon/templates/includes/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:11:27.668485 pynchon-2024.4.3.17.11/src/pynchon/templates/includes/pynchon/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:11:27.692485 pynchon-2024.4.3.17.11/src/pynchon/templates/includes/pynchon/github/
--rw-r--r--   0 runner    (1001) docker     (127)      297 2024-04-03 17:06:30.000000 pynchon-2024.4.3.17.11/src/pynchon/templates/includes/pynchon/github/header.md.j2
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:11:27.672485 pynchon-2024.4.3.17.11/src/pynchon/templates/includes/pynchon/plugins/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:11:27.696485 pynchon-2024.4.3.17.11/src/pynchon/templates/includes/pynchon/plugins/core/
--rw-r--r--   0 runner    (1001) docker     (127)      401 2024-04-03 17:06:30.000000 pynchon-2024.4.3.17.11/src/pynchon/templates/includes/pynchon/plugins/core/VERSIONS.md.j2
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:11:27.696485 pynchon-2024.4.3.17.11/src/pynchon/templates/includes/pynchon/plugins/core/bootstrap/
--rw-r--r--   0 runner    (1001) docker     (127)      118 2024-04-03 17:06:30.000000 pynchon-2024.4.3.17.11/src/pynchon/templates/includes/pynchon/plugins/core/bootstrap/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)     1150 2024-04-03 17:06:30.000000 pynchon-2024.4.3.17.11/src/pynchon/templates/includes/pynchon/plugins/core/bootstrap/bash.sh
--rw-r--r--   0 runner    (1001) docker     (127)      799 2024-04-03 17:06:30.000000 pynchon-2024.4.3.17.11/src/pynchon/templates/includes/pynchon/plugins/core/bootstrap/bashrc.sh
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-03 17:06:30.000000 pynchon-2024.4.3.17.11/src/pynchon/templates/includes/pynchon/plugins/core/bootstrap/makefile.j2
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-03 17:06:30.000000 pynchon-2024.4.3.17.11/src/pynchon/templates/includes/pynchon/plugins/core/bootstrap/python.j2
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-03 17:06:30.000000 pynchon-2024.4.3.17.11/src/pynchon/templates/includes/pynchon/plugins/core/bootstrap/sh.j2
--rw-r--r--   0 runner    (1001) docker     (127)      912 2024-04-03 17:06:30.000000 pynchon-2024.4.3.17.11/src/pynchon/templates/includes/pynchon/plugins/core/bootstrap/tox.ini
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:11:27.696485 pynchon-2024.4.3.17.11/src/pynchon/templates/includes/pynchon/plugins/fixme/
--rw-r--r--   0 runner    (1001) docker     (127)      164 2024-04-03 17:06:30.000000 pynchon-2024.4.3.17.11/src/pynchon/templates/includes/pynchon/plugins/fixme/FIXME.md.j2
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:11:27.696485 pynchon-2024.4.3.17.11/src/pynchon/templates/includes/pynchon/plugins/makefile/
--rw-r--r--   0 runner    (1001) docker     (127)     1202 2024-04-03 17:06:30.000000 pynchon-2024.4.3.17.11/src/pynchon/templates/includes/pynchon/plugins/makefile/mermaid-graph.mmd.j2
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:11:27.668485 pynchon-2024.4.3.17.11/src/pynchon/templates/includes/pynchon/plugins/python/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:11:27.696485 pynchon-2024.4.3.17.11/src/pynchon/templates/includes/pynchon/plugins/python/api/
--rw-r--r--   0 runner    (1001) docker     (127)      105 2024-04-03 17:06:30.000000 pynchon-2024.4.3.17.11/src/pynchon/templates/includes/pynchon/plugins/python/api/TOC.md.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1218 2024-04-03 17:06:30.000000 pynchon-2024.4.3.17.11/src/pynchon/templates/includes/pynchon/plugins/python/api/classes.md.j2
--rw-r--r--   0 runner    (1001) docker     (127)      953 2024-04-03 17:06:30.000000 pynchon-2024.4.3.17.11/src/pynchon/templates/includes/pynchon/plugins/python/api/functions.md.j2
--rw-r--r--   0 runner    (1001) docker     (127)      324 2024-04-03 17:06:30.000000 pynchon-2024.4.3.17.11/src/pynchon/templates/includes/pynchon/plugins/python/api/modules.md.j2
--rw-r--r--   0 runner    (1001) docker     (127)      126 2024-04-03 17:06:30.000000 pynchon-2024.4.3.17.11/src/pynchon/templates/includes/pynchon/plugins/python/api/names.md.j2
--rw-r--r--   0 runner    (1001) docker     (127)      778 2024-04-03 17:06:30.000000 pynchon-2024.4.3.17.11/src/pynchon/templates/includes/pynchon/plugins/python/api/package.md.j2
--rw-r--r--   0 runner    (1001) docker     (127)     2987 2024-04-03 17:06:30.000000 pynchon-2024.4.3.17.11/src/pynchon/templates/includes/pynchon/plugins/python/api/toc2.md.j2
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:11:27.668485 pynchon-2024.4.3.17.11/src/pynchon/templates/includes/pynchon/plugins/python/gen/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:11:27.696485 pynchon-2024.4.3.17.11/src/pynchon/templates/includes/pynchon/plugins/python/gen/docstrings/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 17:06:30.000000 pynchon-2024.4.3.17.11/src/pynchon/templates/includes/pynchon/plugins/python/gen/docstrings/function.txt.j2
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 17:06:30.000000 pynchon-2024.4.3.17.11/src/pynchon/templates/includes/pynchon/plugins/python/gen/docstrings/module.txt.j2
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:11:27.700485 pynchon-2024.4.3.17.11/src/pynchon/templates/includes/pynchon/plugins/python_cli/
--rw-r--r--   0 runner    (1001) docker     (127)     1449 2024-04-03 17:06:30.000000 pynchon-2024.4.3.17.11/src/pynchon/templates/includes/pynchon/plugins/python_cli/TOC.md.j2
--rw-r--r--   0 runner    (1001) docker     (127)      200 2024-04-03 17:06:30.000000 pynchon-2024.4.3.17.11/src/pynchon/templates/includes/pynchon/plugins/python_cli/detail.md.j2
--rw-r--r--   0 runner    (1001) docker     (127)      696 2024-04-03 17:06:30.000000 pynchon-2024.4.3.17.11/src/pynchon/templates/includes/pynchon/plugins/python_cli/main.module.md.j2
--rw-r--r--   0 runner    (1001) docker     (127)      910 2024-04-03 17:06:30.000000 pynchon-2024.4.3.17.11/src/pynchon/templates/includes/pynchon/plugins/python_cli/script.console.md.j2
--rw-r--r--   0 runner    (1001) docker     (127)      284 2024-04-03 17:06:30.000000 pynchon-2024.4.3.17.11/src/pynchon/templates/includes/pynchon/plugins/python_cli/subcommand.md.j2
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:11:27.672485 pynchon-2024.4.3.17.11/src/pynchon/templates/includes/pynchon/plugins/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:11:27.700485 pynchon-2024.4.3.17.11/src/pynchon/templates/includes/pynchon/plugins/src/header/
--rw-r--r--   0 runner    (1001) docker     (127)      134 2024-04-03 17:06:30.000000 pynchon-2024.4.3.17.11/src/pynchon/templates/includes/pynchon/plugins/src/header/jinja-md.md.j2
--rw-r--r--   0 runner    (1001) docker     (127)      134 2024-04-03 17:06:30.000000 pynchon-2024.4.3.17.11/src/pynchon/templates/includes/pynchon/plugins/src/header/jinja.j2
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-04-03 17:06:30.000000 pynchon-2024.4.3.17.11/src/pynchon/templates/includes/pynchon/plugins/src/header/python.j2
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:11:27.700485 pynchon-2024.4.3.17.11/src/pynchon/templates/scaffolds/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 17:06:30.000000 pynchon-2024.4.3.17.11/src/pynchon/templates/scaffolds/.gitkeep
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:11:27.672485 pynchon-2024.4.3.17.11/src/pynchon/templates/scaffolds/ansible/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:11:27.700485 pynchon-2024.4.3.17.11/src/pynchon/templates/scaffolds/ansible/role/
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-03 17:06:30.000000 pynchon-2024.4.3.17.11/src/pynchon/templates/scaffolds/ansible/role/.ansible-lint
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:11:27.672485 pynchon-2024.4.3.17.11/src/pynchon/templates/scaffolds/ansible/role/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:11:27.700485 pynchon-2024.4.3.17.11/src/pynchon/templates/scaffolds/ansible/role/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 17:06:30.000000 pynchon-2024.4.3.17.11/src/pynchon/templates/scaffolds/ansible/role/.github/workflows/ansible-lint.yml
--rw-r--r--   0 runner    (1001) docker     (127)      505 2024-04-03 17:06:30.000000 pynchon-2024.4.3.17.11/src/pynchon/templates/scaffolds/ansible/role/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:11:27.700485 pynchon-2024.4.3.17.11/src/pynchon/templates/scaffolds/docker/
--rw-r--r--   0 runner    (1001) docker     (127)     1079 2024-04-03 17:06:30.000000 pynchon-2024.4.3.17.11/src/pynchon/templates/scaffolds/docker/.dockerignore
--rw-r--r--   0 runner    (1001) docker     (127)       90 2024-04-03 17:06:30.000000 pynchon-2024.4.3.17.11/src/pynchon/templates/scaffolds/docker/.scaffold.advice.json5
--rw-r--r--   0 runner    (1001) docker     (127)      162 2024-04-03 17:06:30.000000 pynchon-2024.4.3.17.11/src/pynchon/templates/scaffolds/docker/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (127)     1374 2024-04-03 17:06:30.000000 pynchon-2024.4.3.17.11/src/pynchon/templates/scaffolds/docker/README.md.j2
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:11:27.672485 pynchon-2024.4.3.17.11/src/pynchon/templates/scaffolds/docs/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:11:27.700485 pynchon-2024.4.3.17.11/src/pynchon/templates/scaffolds/docs/includes/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 17:06:30.000000 pynchon-2024.4.3.17.11/src/pynchon/templates/scaffolds/docs/includes/.gitkeep
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:11:27.700485 pynchon-2024.4.3.17.11/src/pynchon/templates/scaffolds/github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:11:27.672485 pynchon-2024.4.3.17.11/src/pynchon/templates/scaffolds/github/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:11:27.700485 pynchon-2024.4.3.17.11/src/pynchon/templates/scaffolds/github/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 17:06:30.000000 pynchon-2024.4.3.17.11/src/pynchon/templates/scaffolds/github/.github/workflows/.gitkeep
--rw-r--r--   0 runner    (1001) docker     (127)      153 2024-04-03 17:06:30.000000 pynchon-2024.4.3.17.11/src/pynchon/templates/scaffolds/github/.github/workflows/hello-world.yml
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-03 17:06:30.000000 pynchon-2024.4.3.17.11/src/pynchon/templates/scaffolds/github/.scaffold.advice.json5
--rw-r--r--   0 runner    (1001) docker     (127)      458 2024-04-03 17:06:30.000000 pynchon-2024.4.3.17.11/src/pynchon/templates/scaffolds/github/README.md.j2
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:11:27.672485 pynchon-2024.4.3.17.11/src/pynchon/templates/scaffolds/py/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:11:27.704485 pynchon-2024.4.3.17.11/src/pynchon/templates/scaffolds/py/pkg/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 17:06:30.000000 pynchon-2024.4.3.17.11/src/pynchon/templates/scaffolds/py/pkg/.ackrc
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 17:06:30.000000 pynchon-2024.4.3.17.11/src/pynchon/templates/scaffolds/py/pkg/.flake8
--rw-r--r--   0 runner    (1001) docker     (127)      776 2024-04-03 17:06:30.000000 pynchon-2024.4.3.17.11/src/pynchon/templates/scaffolds/py/pkg/.libcst.codemod.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       64 2024-04-03 17:06:30.000000 pynchon-2024.4.3.17.11/src/pynchon/templates/scaffolds/py/pkg/.scaffold.advice.json5
--rw-r--r--   0 runner    (1001) docker     (127)     1928 2024-04-03 17:06:30.000000 pynchon-2024.4.3.17.11/src/pynchon/templates/scaffolds/py/pkg/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)     2233 2024-04-03 17:06:30.000000 pynchon-2024.4.3.17.11/src/pynchon/templates/scaffolds/py/pkg/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1549 2024-04-03 17:06:30.000000 pynchon-2024.4.3.17.11/src/pynchon/templates/scaffolds/py/pkg/README.md.j2
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:11:27.704485 pynchon-2024.4.3.17.11/src/pynchon/templates/scaffolds/py/pkg/docs/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 17:06:30.000000 pynchon-2024.4.3.17.11/src/pynchon/templates/scaffolds/py/pkg/docs/.gitkeep
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:11:27.704485 pynchon-2024.4.3.17.11/src/pynchon/templates/scaffolds/py/pkg/docs/html/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 17:06:30.000000 pynchon-2024.4.3.17.11/src/pynchon/templates/scaffolds/py/pkg/docs/html/.gitkeep
--rw-r--r--   0 runner    (1001) docker     (127)     2396 2024-04-03 17:06:30.000000 pynchon-2024.4.3.17.11/src/pynchon/templates/scaffolds/py/pkg/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      771 2024-04-03 17:06:30.000000 pynchon-2024.4.3.17.11/src/pynchon/templates/scaffolds/py/pkg/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:11:27.672485 pynchon-2024.4.3.17.11/src/pynchon/templates/scaffolds/py/pkg/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:11:27.704485 pynchon-2024.4.3.17.11/src/pynchon/templates/scaffolds/py/pkg/src/{{name}}/
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-03 17:06:30.000000 pynchon-2024.4.3.17.11/src/pynchon/templates/scaffolds/py/pkg/src/{{name}}/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-03 17:06:30.000000 pynchon-2024.4.3.17.11/src/pynchon/templates/scaffolds/py/pkg/src/{{name}}/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-03 17:06:30.000000 pynchon-2024.4.3.17.11/src/pynchon/templates/scaffolds/py/pkg/src/{{name}}/app.py
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-03 17:06:30.000000 pynchon-2024.4.3.17.11/src/pynchon/templates/scaffolds/py/pkg/src/{{name}}/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-04-03 17:06:30.000000 pynchon-2024.4.3.17.11/src/pynchon/templates/scaffolds/py/pkg/src/{{name}}/lme.py
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-03 17:06:30.000000 pynchon-2024.4.3.17.11/src/pynchon/templates/scaffolds/py/pkg/src/{{name}}/models.py
--rw-r--r--   0 runner    (1001) docker     (127)       87 2024-04-03 17:06:30.000000 pynchon-2024.4.3.17.11/src/pynchon/templates/scaffolds/py/pkg/src/{{name}}/tagging.py
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-03 17:06:30.000000 pynchon-2024.4.3.17.11/src/pynchon/templates/scaffolds/py/pkg/src/{{name}}/typing.py
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-03 17:06:30.000000 pynchon-2024.4.3.17.11/src/pynchon/templates/scaffolds/py/pkg/src/{{name}}/util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:11:27.704485 pynchon-2024.4.3.17.11/src/pynchon/templates/scaffolds/py/pkg/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 17:06:30.000000 pynchon-2024.4.3.17.11/src/pynchon/templates/scaffolds/py/pkg/tests/.gitkeep
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 17:06:30.000000 pynchon-2024.4.3.17.11/src/pynchon/templates/scaffolds/py/pkg/tests/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:11:27.708485 pynchon-2024.4.3.17.11/src/pynchon/templates/scaffolds/py/pkg/tests/integration/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 17:06:30.000000 pynchon-2024.4.3.17.11/src/pynchon/templates/scaffolds/py/pkg/tests/integration/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-03 17:06:30.000000 pynchon-2024.4.3.17.11/src/pynchon/templates/scaffolds/py/pkg/tests/integration/test_all.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:11:27.708485 pynchon-2024.4.3.17.11/src/pynchon/templates/scaffolds/py/pkg/tests/smoke/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 17:06:30.000000 pynchon-2024.4.3.17.11/src/pynchon/templates/scaffolds/py/pkg/tests/smoke/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-03 17:06:30.000000 pynchon-2024.4.3.17.11/src/pynchon/templates/scaffolds/py/pkg/tests/smoke/test_all.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:11:27.708485 pynchon-2024.4.3.17.11/src/pynchon/templates/scaffolds/py/pkg/tests/units/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 17:06:30.000000 pynchon-2024.4.3.17.11/src/pynchon/templates/scaffolds/py/pkg/tests/units/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-03 17:06:30.000000 pynchon-2024.4.3.17.11/src/pynchon/templates/scaffolds/py/pkg/tests/units/test_all.py
--rw-r--r--   0 runner    (1001) docker     (127)     3097 2024-04-03 17:06:30.000000 pynchon-2024.4.3.17.11/src/pynchon/templates/scaffolds/py/pkg/tox.ini
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:11:27.708485 pynchon-2024.4.3.17.11/src/pynchon/templates/scaffolds/py/workspace/
--rw-r--r--   0 runner    (1001) docker     (127)       64 2024-04-03 17:06:30.000000 pynchon-2024.4.3.17.11/src/pynchon/templates/scaffolds/py/workspace/.scaffold.advice.json5
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:11:27.672485 pynchon-2024.4.3.17.11/src/pynchon/templates/scaffolds/software/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:11:27.708485 pynchon-2024.4.3.17.11/src/pynchon/templates/scaffolds/software/automation/
--rw-r--r--   0 runner    (1001) docker     (127)      348 2024-04-03 17:06:30.000000 pynchon-2024.4.3.17.11/src/pynchon/templates/scaffolds/software/automation/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:11:27.708485 pynchon-2024.4.3.17.11/src/pynchon/templates/scaffolds/software/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      348 2024-04-03 17:06:30.000000 pynchon-2024.4.3.17.11/src/pynchon/templates/scaffolds/software/tests/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:11:27.672485 pynchon-2024.4.3.17.11/src/pynchon/templates/scaffolds/software/tests/tests/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:11:27.708485 pynchon-2024.4.3.17.11/src/pynchon/templates/scaffolds/software/tests/tests/integration/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 17:06:30.000000 pynchon-2024.4.3.17.11/src/pynchon/templates/scaffolds/software/tests/tests/integration/.gitkeep
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:11:27.708485 pynchon-2024.4.3.17.11/src/pynchon/templates/scaffolds/software/tests/tests/smoke/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 17:06:30.000000 pynchon-2024.4.3.17.11/src/pynchon/templates/scaffolds/software/tests/tests/smoke/.gitkeep
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:11:27.708485 pynchon-2024.4.3.17.11/src/pynchon/templates/scaffolds/software/tests/tests/units/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 17:06:30.000000 pynchon-2024.4.3.17.11/src/pynchon/templates/scaffolds/software/tests/tests/units/.gitkeep
--rw-r--r--   0 runner    (1001) docker     (127)      284 2024-04-03 17:06:30.000000 pynchon-2024.4.3.17.11/src/pynchon/testing.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:11:27.708485 pynchon-2024.4.3.17.11/src/pynchon/util/
--rw-r--r--   0 runner    (1001) docker     (127)     1055 2024-04-03 17:06:30.000000 pynchon-2024.4.3.17.11/src/pynchon/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-03 17:06:30.000000 pynchon-2024.4.3.17.11/src/pynchon/util/click.py
--rw-r--r--   0 runner    (1001) docker     (127)     6160 2024-04-03 17:07:37.000000 pynchon-2024.4.3.17.11/src/pynchon/util/complexity.py
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-03 17:06:30.000000 pynchon-2024.4.3.17.11/src/pynchon/util/config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:11:27.712485 pynchon-2024.4.3.17.11/src/pynchon/util/console/
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-03 17:06:30.000000 pynchon-2024.4.3.17.11/src/pynchon/util/console/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-03 17:06:30.000000 pynchon-2024.4.3.17.11/src/pynchon/util/console/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4662 2024-04-03 17:06:30.000000 pynchon-2024.4.3.17.11/src/pynchon/util/docker.py
--rw-r--r--   0 runner    (1001) docker     (127)      711 2024-04-03 17:07:37.000000 pynchon-2024.4.3.17.11/src/pynchon/util/events.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:11:27.712485 pynchon-2024.4.3.17.11/src/pynchon/util/files/
--rw-r--r--   0 runner    (1001) docker     (127)     3902 2024-04-03 17:07:37.000000 pynchon-2024.4.3.17.11/src/pynchon/util/files/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      948 2024-04-03 17:07:37.000000 pynchon-2024.4.3.17.11/src/pynchon/util/files/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2089 2024-04-03 17:07:37.000000 pynchon-2024.4.3.17.11/src/pynchon/util/files/diff.py
--rw-r--r--   0 runner    (1001) docker     (127)     2608 2024-04-03 17:07:37.000000 pynchon-2024.4.3.17.11/src/pynchon/util/lme.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:11:27.712485 pynchon-2024.4.3.17.11/src/pynchon/util/makefile/
--rw-r--r--   0 runner    (1001) docker     (127)     5276 2024-04-03 17:07:37.000000 pynchon-2024.4.3.17.11/src/pynchon/util/makefile/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      484 2024-04-03 17:07:37.000000 pynchon-2024.4.3.17.11/src/pynchon/util/makefile/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1139 2024-04-03 17:06:30.000000 pynchon-2024.4.3.17.11/src/pynchon/util/oop.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:11:27.712485 pynchon-2024.4.3.17.11/src/pynchon/util/os/
--rw-r--r--   0 runner    (1001) docker     (127)      578 2024-04-03 17:06:30.000000 pynchon-2024.4.3.17.11/src/pynchon/util/os/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5760 2024-04-03 17:06:30.000000 pynchon-2024.4.3.17.11/src/pynchon/util/os/models.py
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-04-03 17:06:30.000000 pynchon-2024.4.3.17.11/src/pynchon/util/os/pidfile.py
--rw-r--r--   0 runner    (1001) docker     (127)     1081 2024-04-03 17:06:30.000000 pynchon-2024.4.3.17.11/src/pynchon/util/os/pids.py
--rw-r--r--   0 runner    (1001) docker     (127)     2054 2024-04-03 17:06:30.000000 pynchon-2024.4.3.17.11/src/pynchon/util/python.py
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-04-03 17:06:30.000000 pynchon-2024.4.3.17.11/src/pynchon/util/splitvt.py
--rw-r--r--   0 runner    (1001) docker     (127)      463 2024-04-03 17:06:30.000000 pynchon-2024.4.3.17.11/src/pynchon/util/testing.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:11:27.712485 pynchon-2024.4.3.17.11/src/pynchon/util/text/
--rw-r--r--   0 runner    (1001) docker     (127)      551 2024-04-03 17:06:30.000000 pynchon-2024.4.3.17.11/src/pynchon/util/text/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      367 2024-04-03 17:07:37.000000 pynchon-2024.4.3.17.11/src/pynchon/util/text/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:11:27.712485 pynchon-2024.4.3.17.11/src/pynchon/util/text/dumpf/
--rw-r--r--   0 runner    (1001) docker     (127)      790 2024-04-03 17:07:37.000000 pynchon-2024.4.3.17.11/src/pynchon/util/text/dumpf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1047 2024-04-03 17:07:37.000000 pynchon-2024.4.3.17.11/src/pynchon/util/text/dumpf/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)      598 2024-04-03 17:06:30.000000 pynchon-2024.4.3.17.11/src/pynchon/util/text/dumps.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:11:27.712485 pynchon-2024.4.3.17.11/src/pynchon/util/text/loadf/
--rw-r--r--   0 runner    (1001) docker     (127)     7414 2024-04-03 17:07:37.000000 pynchon-2024.4.3.17.11/src/pynchon/util/text/loadf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1042 2024-04-03 17:07:37.000000 pynchon-2024.4.3.17.11/src/pynchon/util/text/loadf/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1950 2024-04-03 17:07:37.000000 pynchon-2024.4.3.17.11/src/pynchon/util/text/loads.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:11:27.712485 pynchon-2024.4.3.17.11/src/pynchon/util/text/normalize/
--rw-r--r--   0 runner    (1001) docker     (127)     1285 2024-04-03 17:06:30.000000 pynchon-2024.4.3.17.11/src/pynchon/util/text/normalize/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:11:27.712485 pynchon-2024.4.3.17.11/src/pynchon/util/text/render/
--rw-r--r--   0 runner    (1001) docker     (127)     5825 2024-04-03 17:07:37.000000 pynchon-2024.4.3.17.11/src/pynchon/util/text/render/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      972 2024-04-03 17:07:37.000000 pynchon-2024.4.3.17.11/src/pynchon/util/text/render/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1395 2024-04-03 17:06:30.000000 pynchon-2024.4.3.17.11/src/pynchon/util/typing.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:11:27.712485 pynchon-2024.4.3.17.11/src/pynchon.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1714 2024-04-03 17:11:27.000000 pynchon-2024.4.3.17.11/src/pynchon.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     9272 2024-04-03 17:11:27.000000 pynchon-2024.4.3.17.11/src/pynchon.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 17:11:27.000000 pynchon-2024.4.3.17.11/src/pynchon.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-04-03 17:11:27.000000 pynchon-2024.4.3.17.11/src/pynchon.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 17:11:27.000000 pynchon-2024.4.3.17.11/src/pynchon.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      438 2024-04-03 17:11:27.000000 pynchon-2024.4.3.17.11/src/pynchon.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-03 17:11:27.000000 pynchon-2024.4.3.17.11/src/pynchon.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:15:50.255286 pynchon-2024.4.3.17.15/
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-04-03 17:10:52.000000 pynchon-2024.4.3.17.15/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1714 2024-04-03 17:15:50.255286 pynchon-2024.4.3.17.15/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2144 2024-04-03 17:10:52.000000 pynchon-2024.4.3.17.15/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      979 2024-04-03 17:10:52.000000 pynchon-2024.4.3.17.15/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1728 2024-04-03 17:15:50.255286 pynchon-2024.4.3.17.15/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      770 2024-04-03 17:10:52.000000 pynchon-2024.4.3.17.15/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:15:50.191285 pynchon-2024.4.3.17.15/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:15:50.207285 pynchon-2024.4.3.17.15/src/pynchon/
+-rw-r--r--   0 runner    (1001) docker     (127)      259 2024-04-03 17:10:52.000000 pynchon-2024.4.3.17.15/src/pynchon/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-04-03 17:10:52.000000 pynchon-2024.4.3.17.15/src/pynchon/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-04-03 17:15:47.000000 pynchon-2024.4.3.17.15/src/pynchon/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:15:50.207285 pynchon-2024.4.3.17.15/src/pynchon/abcs/
+-rw-r--r--   0 runner    (1001) docker     (127)      319 2024-04-03 17:10:52.000000 pynchon-2024.4.3.17.15/src/pynchon/abcs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1503 2024-04-03 17:10:52.000000 pynchon-2024.4.3.17.15/src/pynchon/abcs/attrdict.py
+-rw-r--r--   0 runner    (1001) docker     (127)      115 2024-04-03 17:10:52.000000 pynchon-2024.4.3.17.15/src/pynchon/abcs/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2011 2024-04-03 17:10:52.000000 pynchon-2024.4.3.17.15/src/pynchon/abcs/path.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5484 2024-04-03 17:10:52.000000 pynchon-2024.4.3.17.15/src/pynchon/abcs/visitor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5088 2024-04-03 17:11:58.000000 pynchon-2024.4.3.17.15/src/pynchon/annotate.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:15:50.211285 pynchon-2024.4.3.17.15/src/pynchon/api/
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-04-03 17:10:52.000000 pynchon-2024.4.3.17.15/src/pynchon/api/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:15:50.211285 pynchon-2024.4.3.17.15/src/pynchon/api/git/
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-03 17:10:52.000000 pynchon-2024.4.3.17.15/src/pynchon/api/git/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:15:50.211285 pynchon-2024.4.3.17.15/src/pynchon/api/parsers/
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-04-03 17:10:52.000000 pynchon-2024.4.3.17.15/src/pynchon/api/parsers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:15:50.211285 pynchon-2024.4.3.17.15/src/pynchon/api/project/
+-rw-r--r--   0 runner    (1001) docker     (127)     1203 2024-04-03 17:10:52.000000 pynchon-2024.4.3.17.15/src/pynchon/api/project/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-03 17:10:52.000000 pynchon-2024.4.3.17.15/src/pynchon/api/pynchon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7246 2024-04-03 17:11:58.000000 pynchon-2024.4.3.17.15/src/pynchon/api/render.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5262 2024-04-03 17:11:58.000000 pynchon-2024.4.3.17.15/src/pynchon/app.py
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-03 17:10:52.000000 pynchon-2024.4.3.17.15/src/pynchon/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2606 2024-04-03 17:11:58.000000 pynchon-2024.4.3.17.15/src/pynchon/bin.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:15:50.211285 pynchon-2024.4.3.17.15/src/pynchon/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)      128 2024-04-03 17:10:52.000000 pynchon-2024.4.3.17.15/src/pynchon/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5029 2024-04-03 17:11:58.000000 pynchon-2024.4.3.17.15/src/pynchon/cli/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)      357 2024-04-03 17:10:52.000000 pynchon-2024.4.3.17.15/src/pynchon/cli/options.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:15:50.211285 pynchon-2024.4.3.17.15/src/pynchon/codemod/
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-03 17:10:52.000000 pynchon-2024.4.3.17.15/src/pynchon/codemod/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:15:50.211285 pynchon-2024.4.3.17.15/src/pynchon/codemod/commands/
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-03 17:10:52.000000 pynchon-2024.4.3.17.15/src/pynchon/codemod/commands/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:15:50.211285 pynchon-2024.4.3.17.15/src/pynchon/codemod/commands/docstrings/
+-rw-r--r--   0 runner    (1001) docker     (127)      329 2024-04-03 17:10:52.000000 pynchon-2024.4.3.17.15/src/pynchon/codemod/commands/docstrings/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2564 2024-04-03 17:10:52.000000 pynchon-2024.4.3.17.15/src/pynchon/codemod/commands/docstrings/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      557 2024-04-03 17:10:52.000000 pynchon-2024.4.3.17.15/src/pynchon/codemod/commands/docstrings/javadoc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9607 2024-04-03 17:11:58.000000 pynchon-2024.4.3.17.15/src/pynchon/codemod/commands/docstrings/simple.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:15:50.211285 pynchon-2024.4.3.17.15/src/pynchon/config/
+-rw-r--r--   0 runner    (1001) docker     (127)     1865 2024-04-03 17:11:58.000000 pynchon-2024.4.3.17.15/src/pynchon/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5049 2024-04-03 17:11:58.000000 pynchon-2024.4.3.17.15/src/pynchon/config/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1470 2024-04-03 17:10:52.000000 pynchon-2024.4.3.17.15/src/pynchon/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3677 2024-04-03 17:10:52.000000 pynchon-2024.4.3.17.15/src/pynchon/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2376 2024-04-03 17:10:52.000000 pynchon-2024.4.3.17.15/src/pynchon/events.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:15:50.215285 pynchon-2024.4.3.17.15/src/pynchon/models/
+-rw-r--r--   0 runner    (1001) docker     (127)      135 2024-04-03 17:10:52.000000 pynchon-2024.4.3.17.15/src/pynchon/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9072 2024-04-03 17:11:58.000000 pynchon-2024.4.3.17.15/src/pynchon/models/planner.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12987 2024-04-03 17:11:58.000000 pynchon-2024.4.3.17.15/src/pynchon/models/planning.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:15:50.215285 pynchon-2024.4.3.17.15/src/pynchon/models/plugins/
+-rw-r--r--   0 runner    (1001) docker     (127)     1420 2024-04-03 17:10:52.000000 pynchon-2024.4.3.17.15/src/pynchon/models/plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10507 2024-04-03 17:10:52.000000 pynchon-2024.4.3.17.15/src/pynchon/models/plugins/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2690 2024-04-03 17:11:58.000000 pynchon-2024.4.3.17.15/src/pynchon/models/plugins/docker.py
+-rw-r--r--   0 runner    (1001) docker     (127)      606 2024-04-03 17:11:58.000000 pynchon-2024.4.3.17.15/src/pynchon/models/plugins/provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5752 2024-04-03 17:11:58.000000 pynchon-2024.4.3.17.15/src/pynchon/models/plugins/pynchon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      568 2024-04-03 17:10:52.000000 pynchon-2024.4.3.17.15/src/pynchon/models/plugins/tool.py
+-rw-r--r--   0 runner    (1001) docker     (127)      959 2024-04-03 17:10:52.000000 pynchon-2024.4.3.17.15/src/pynchon/models/plugins/validators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3027 2024-04-03 17:10:52.000000 pynchon-2024.4.3.17.15/src/pynchon/models/python.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:15:50.219285 pynchon-2024.4.3.17.15/src/pynchon/plugins/
+-rw-r--r--   0 runner    (1001) docker     (127)     1025 2024-04-03 17:10:52.000000 pynchon-2024.4.3.17.15/src/pynchon/plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      402 2024-04-03 17:10:52.000000 pynchon-2024.4.3.17.15/src/pynchon/plugins/__template__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-03 17:10:52.000000 pynchon-2024.4.3.17.15/src/pynchon/plugins/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1520 2024-04-03 17:11:58.000000 pynchon-2024.4.3.17.15/src/pynchon/plugins/cicd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8821 2024-04-03 17:11:58.000000 pynchon-2024.4.3.17.15/src/pynchon/plugins/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2035 2024-04-03 17:10:52.000000 pynchon-2024.4.3.17.15/src/pynchon/plugins/deck.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1036 2024-04-03 17:10:52.000000 pynchon-2024.4.3.17.15/src/pynchon/plugins/dockerhub.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:15:50.223285 pynchon-2024.4.3.17.15/src/pynchon/plugins/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-03 17:10:52.000000 pynchon-2024.4.3.17.15/src/pynchon/plugins/docs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5152 2024-04-03 17:11:58.000000 pynchon-2024.4.3.17.15/src/pynchon/plugins/docs/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2072 2024-04-03 17:10:52.000000 pynchon-2024.4.3.17.15/src/pynchon/plugins/docs/opener.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:15:50.223285 pynchon-2024.4.3.17.15/src/pynchon/plugins/doctor/
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-04-03 17:10:52.000000 pynchon-2024.4.3.17.15/src/pynchon/plugins/doctor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2489 2024-04-03 17:11:58.000000 pynchon-2024.4.3.17.15/src/pynchon/plugins/dot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3301 2024-04-03 17:10:52.000000 pynchon-2024.4.3.17.15/src/pynchon/plugins/drawio.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3549 2024-04-03 17:11:58.000000 pynchon-2024.4.3.17.15/src/pynchon/plugins/fixme.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2902 2024-04-03 17:10:52.000000 pynchon-2024.4.3.17.15/src/pynchon/plugins/gen.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4747 2024-04-03 17:10:52.000000 pynchon-2024.4.3.17.15/src/pynchon/plugins/git.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4277 2024-04-03 17:10:52.000000 pynchon-2024.4.3.17.15/src/pynchon/plugins/github.py
+-rw-r--r--   0 runner    (1001) docker     (127)      401 2024-04-03 17:11:58.000000 pynchon-2024.4.3.17.15/src/pynchon/plugins/globals.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1597 2024-04-03 17:10:52.000000 pynchon-2024.4.3.17.15/src/pynchon/plugins/griffe.py
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-03 17:10:52.000000 pynchon-2024.4.3.17.15/src/pynchon/plugins/hooks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4232 2024-04-03 17:11:58.000000 pynchon-2024.4.3.17.15/src/pynchon/plugins/jinja.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1507 2024-04-03 17:10:52.000000 pynchon-2024.4.3.17.15/src/pynchon/plugins/json.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3954 2024-04-03 17:11:58.000000 pynchon-2024.4.3.17.15/src/pynchon/plugins/makefile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6750 2024-04-03 17:10:52.000000 pynchon-2024.4.3.17.15/src/pynchon/plugins/markdown.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2745 2024-04-03 17:10:52.000000 pynchon-2024.4.3.17.15/src/pynchon/plugins/mermaid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8009 2024-04-03 17:11:58.000000 pynchon-2024.4.3.17.15/src/pynchon/plugins/mkdocs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3218 2024-04-03 17:11:58.000000 pynchon-2024.4.3.17.15/src/pynchon/plugins/pandoc.py
+-rw-r--r--   0 runner    (1001) docker     (127)      456 2024-04-03 17:10:52.000000 pynchon-2024.4.3.17.15/src/pynchon/plugins/parse.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14638 2024-04-03 17:11:58.000000 pynchon-2024.4.3.17.15/src/pynchon/plugins/pattern.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1636 2024-04-03 17:11:58.000000 pynchon-2024.4.3.17.15/src/pynchon/plugins/plugins.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4044 2024-04-03 17:11:58.000000 pynchon-2024.4.3.17.15/src/pynchon/plugins/project.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:15:50.223285 pynchon-2024.4.3.17.15/src/pynchon/plugins/python/
+-rw-r--r--   0 runner    (1001) docker     (127)      145 2024-04-03 17:10:52.000000 pynchon-2024.4.3.17.15/src/pynchon/plugins/python/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3374 2024-04-03 17:10:52.000000 pynchon-2024.4.3.17.15/src/pynchon/plugins/python/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17560 2024-04-03 17:11:58.000000 pynchon-2024.4.3.17.15/src/pynchon/plugins/python/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-03 17:10:52.000000 pynchon-2024.4.3.17.15/src/pynchon/plugins/python/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-04-03 17:10:52.000000 pynchon-2024.4.3.17.15/src/pynchon/plugins/python/cst.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3509 2024-04-03 17:11:58.000000 pynchon-2024.4.3.17.15/src/pynchon/plugins/python/libcst.py
+-rw-r--r--   0 runner    (1001) docker     (127)      236 2024-04-03 17:10:52.000000 pynchon-2024.4.3.17.15/src/pynchon/plugins/python/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3207 2024-04-03 17:10:52.000000 pynchon-2024.4.3.17.15/src/pynchon/plugins/python/platform.py
+-rw-r--r--   0 runner    (1001) docker     (127)      720 2024-04-03 17:10:52.000000 pynchon-2024.4.3.17.15/src/pynchon/plugins/python/pypi.py
+-rw-r--r--   0 runner    (1001) docker     (127)      700 2024-04-03 17:10:52.000000 pynchon-2024.4.3.17.15/src/pynchon/plugins/release.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1153 2024-04-03 17:11:58.000000 pynchon-2024.4.3.17.15/src/pynchon/plugins/render.py
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-04-03 17:10:52.000000 pynchon-2024.4.3.17.15/src/pynchon/plugins/rtd.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:15:50.223285 pynchon-2024.4.3.17.15/src/pynchon/plugins/scaffolding/
+-rw-r--r--   0 runner    (1001) docker     (127)     3784 2024-04-03 17:10:52.000000 pynchon-2024.4.3.17.15/src/pynchon/plugins/scaffolding/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1158 2024-04-03 17:10:52.000000 pynchon-2024.4.3.17.15/src/pynchon/plugins/scaffolding/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7559 2024-04-03 17:10:52.000000 pynchon-2024.4.3.17.15/src/pynchon/plugins/src.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3893 2024-04-03 17:11:58.000000 pynchon-2024.4.3.17.15/src/pynchon/plugins/tests.py
+-rw-r--r--   0 runner    (1001) docker     (127)      402 2024-04-03 17:10:52.000000 pynchon-2024.4.3.17.15/src/pynchon/plugins/tox.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1445 2024-04-03 17:10:52.000000 pynchon-2024.4.3.17.15/src/pynchon/plugins/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-04-03 17:10:52.000000 pynchon-2024.4.3.17.15/src/pynchon/tagging.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:15:50.195285 pynchon-2024.4.3.17.15/src/pynchon/templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:15:50.223285 pynchon-2024.4.3.17.15/src/pynchon/templates/docker/
+-rw-r--r--   0 runner    (1001) docker     (127)      605 2024-04-03 17:10:52.000000 pynchon-2024.4.3.17.15/src/pynchon/templates/docker/Dockerfile.pandoc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:15:50.223285 pynchon-2024.4.3.17.15/src/pynchon/templates/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 17:10:52.000000 pynchon-2024.4.3.17.15/src/pynchon/templates/docs/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:15:50.191285 pynchon-2024.4.3.17.15/src/pynchon/templates/includes/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:15:50.195285 pynchon-2024.4.3.17.15/src/pynchon/templates/includes/pynchon/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:15:50.223285 pynchon-2024.4.3.17.15/src/pynchon/templates/includes/pynchon/github/
+-rw-r--r--   0 runner    (1001) docker     (127)      297 2024-04-03 17:10:52.000000 pynchon-2024.4.3.17.15/src/pynchon/templates/includes/pynchon/github/header.md.j2
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:15:50.195285 pynchon-2024.4.3.17.15/src/pynchon/templates/includes/pynchon/plugins/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:15:50.227285 pynchon-2024.4.3.17.15/src/pynchon/templates/includes/pynchon/plugins/core/
+-rw-r--r--   0 runner    (1001) docker     (127)      401 2024-04-03 17:10:52.000000 pynchon-2024.4.3.17.15/src/pynchon/templates/includes/pynchon/plugins/core/VERSIONS.md.j2
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:15:50.227285 pynchon-2024.4.3.17.15/src/pynchon/templates/includes/pynchon/plugins/core/bootstrap/
+-rw-r--r--   0 runner    (1001) docker     (127)      118 2024-04-03 17:10:52.000000 pynchon-2024.4.3.17.15/src/pynchon/templates/includes/pynchon/plugins/core/bootstrap/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)     1150 2024-04-03 17:10:52.000000 pynchon-2024.4.3.17.15/src/pynchon/templates/includes/pynchon/plugins/core/bootstrap/bash.sh
+-rw-r--r--   0 runner    (1001) docker     (127)      799 2024-04-03 17:10:52.000000 pynchon-2024.4.3.17.15/src/pynchon/templates/includes/pynchon/plugins/core/bootstrap/bashrc.sh
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-03 17:10:52.000000 pynchon-2024.4.3.17.15/src/pynchon/templates/includes/pynchon/plugins/core/bootstrap/makefile.j2
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-03 17:10:52.000000 pynchon-2024.4.3.17.15/src/pynchon/templates/includes/pynchon/plugins/core/bootstrap/python.j2
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-03 17:10:52.000000 pynchon-2024.4.3.17.15/src/pynchon/templates/includes/pynchon/plugins/core/bootstrap/sh.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      912 2024-04-03 17:10:52.000000 pynchon-2024.4.3.17.15/src/pynchon/templates/includes/pynchon/plugins/core/bootstrap/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:15:50.227285 pynchon-2024.4.3.17.15/src/pynchon/templates/includes/pynchon/plugins/fixme/
+-rw-r--r--   0 runner    (1001) docker     (127)      164 2024-04-03 17:10:52.000000 pynchon-2024.4.3.17.15/src/pynchon/templates/includes/pynchon/plugins/fixme/FIXME.md.j2
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:15:50.227285 pynchon-2024.4.3.17.15/src/pynchon/templates/includes/pynchon/plugins/makefile/
+-rw-r--r--   0 runner    (1001) docker     (127)     1202 2024-04-03 17:10:52.000000 pynchon-2024.4.3.17.15/src/pynchon/templates/includes/pynchon/plugins/makefile/mermaid-graph.mmd.j2
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:15:50.195285 pynchon-2024.4.3.17.15/src/pynchon/templates/includes/pynchon/plugins/python/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:15:50.227285 pynchon-2024.4.3.17.15/src/pynchon/templates/includes/pynchon/plugins/python/api/
+-rw-r--r--   0 runner    (1001) docker     (127)      105 2024-04-03 17:10:52.000000 pynchon-2024.4.3.17.15/src/pynchon/templates/includes/pynchon/plugins/python/api/TOC.md.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1218 2024-04-03 17:10:52.000000 pynchon-2024.4.3.17.15/src/pynchon/templates/includes/pynchon/plugins/python/api/classes.md.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      953 2024-04-03 17:10:52.000000 pynchon-2024.4.3.17.15/src/pynchon/templates/includes/pynchon/plugins/python/api/functions.md.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      324 2024-04-03 17:10:52.000000 pynchon-2024.4.3.17.15/src/pynchon/templates/includes/pynchon/plugins/python/api/modules.md.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      126 2024-04-03 17:10:52.000000 pynchon-2024.4.3.17.15/src/pynchon/templates/includes/pynchon/plugins/python/api/names.md.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      778 2024-04-03 17:10:52.000000 pynchon-2024.4.3.17.15/src/pynchon/templates/includes/pynchon/plugins/python/api/package.md.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     2987 2024-04-03 17:10:52.000000 pynchon-2024.4.3.17.15/src/pynchon/templates/includes/pynchon/plugins/python/api/toc2.md.j2
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:15:50.195285 pynchon-2024.4.3.17.15/src/pynchon/templates/includes/pynchon/plugins/python/gen/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:15:50.227285 pynchon-2024.4.3.17.15/src/pynchon/templates/includes/pynchon/plugins/python/gen/docstrings/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 17:10:52.000000 pynchon-2024.4.3.17.15/src/pynchon/templates/includes/pynchon/plugins/python/gen/docstrings/function.txt.j2
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 17:10:52.000000 pynchon-2024.4.3.17.15/src/pynchon/templates/includes/pynchon/plugins/python/gen/docstrings/module.txt.j2
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:15:50.231285 pynchon-2024.4.3.17.15/src/pynchon/templates/includes/pynchon/plugins/python_cli/
+-rw-r--r--   0 runner    (1001) docker     (127)     1449 2024-04-03 17:10:52.000000 pynchon-2024.4.3.17.15/src/pynchon/templates/includes/pynchon/plugins/python_cli/TOC.md.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      200 2024-04-03 17:10:52.000000 pynchon-2024.4.3.17.15/src/pynchon/templates/includes/pynchon/plugins/python_cli/detail.md.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      696 2024-04-03 17:10:52.000000 pynchon-2024.4.3.17.15/src/pynchon/templates/includes/pynchon/plugins/python_cli/main.module.md.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      910 2024-04-03 17:10:52.000000 pynchon-2024.4.3.17.15/src/pynchon/templates/includes/pynchon/plugins/python_cli/script.console.md.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      284 2024-04-03 17:10:52.000000 pynchon-2024.4.3.17.15/src/pynchon/templates/includes/pynchon/plugins/python_cli/subcommand.md.j2
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:15:50.195285 pynchon-2024.4.3.17.15/src/pynchon/templates/includes/pynchon/plugins/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:15:50.231285 pynchon-2024.4.3.17.15/src/pynchon/templates/includes/pynchon/plugins/src/header/
+-rw-r--r--   0 runner    (1001) docker     (127)      134 2024-04-03 17:10:52.000000 pynchon-2024.4.3.17.15/src/pynchon/templates/includes/pynchon/plugins/src/header/jinja-md.md.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      134 2024-04-03 17:10:52.000000 pynchon-2024.4.3.17.15/src/pynchon/templates/includes/pynchon/plugins/src/header/jinja.j2
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-04-03 17:10:52.000000 pynchon-2024.4.3.17.15/src/pynchon/templates/includes/pynchon/plugins/src/header/python.j2
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:15:50.231285 pynchon-2024.4.3.17.15/src/pynchon/templates/scaffolds/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 17:10:52.000000 pynchon-2024.4.3.17.15/src/pynchon/templates/scaffolds/.gitkeep
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:15:50.195285 pynchon-2024.4.3.17.15/src/pynchon/templates/scaffolds/ansible/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:15:50.231285 pynchon-2024.4.3.17.15/src/pynchon/templates/scaffolds/ansible/role/
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-03 17:10:52.000000 pynchon-2024.4.3.17.15/src/pynchon/templates/scaffolds/ansible/role/.ansible-lint
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:15:50.195285 pynchon-2024.4.3.17.15/src/pynchon/templates/scaffolds/ansible/role/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:15:50.231285 pynchon-2024.4.3.17.15/src/pynchon/templates/scaffolds/ansible/role/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 17:10:52.000000 pynchon-2024.4.3.17.15/src/pynchon/templates/scaffolds/ansible/role/.github/workflows/ansible-lint.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      505 2024-04-03 17:10:52.000000 pynchon-2024.4.3.17.15/src/pynchon/templates/scaffolds/ansible/role/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:15:50.231285 pynchon-2024.4.3.17.15/src/pynchon/templates/scaffolds/docker/
+-rw-r--r--   0 runner    (1001) docker     (127)     1079 2024-04-03 17:10:52.000000 pynchon-2024.4.3.17.15/src/pynchon/templates/scaffolds/docker/.dockerignore
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-04-03 17:10:52.000000 pynchon-2024.4.3.17.15/src/pynchon/templates/scaffolds/docker/.scaffold.advice.json5
+-rw-r--r--   0 runner    (1001) docker     (127)      162 2024-04-03 17:10:52.000000 pynchon-2024.4.3.17.15/src/pynchon/templates/scaffolds/docker/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (127)     1374 2024-04-03 17:10:52.000000 pynchon-2024.4.3.17.15/src/pynchon/templates/scaffolds/docker/README.md.j2
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:15:50.199285 pynchon-2024.4.3.17.15/src/pynchon/templates/scaffolds/docs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:15:50.231285 pynchon-2024.4.3.17.15/src/pynchon/templates/scaffolds/docs/includes/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 17:10:52.000000 pynchon-2024.4.3.17.15/src/pynchon/templates/scaffolds/docs/includes/.gitkeep
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:15:50.231285 pynchon-2024.4.3.17.15/src/pynchon/templates/scaffolds/github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:15:50.199285 pynchon-2024.4.3.17.15/src/pynchon/templates/scaffolds/github/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:15:50.231285 pynchon-2024.4.3.17.15/src/pynchon/templates/scaffolds/github/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 17:10:52.000000 pynchon-2024.4.3.17.15/src/pynchon/templates/scaffolds/github/.github/workflows/.gitkeep
+-rw-r--r--   0 runner    (1001) docker     (127)      153 2024-04-03 17:10:52.000000 pynchon-2024.4.3.17.15/src/pynchon/templates/scaffolds/github/.github/workflows/hello-world.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-03 17:10:52.000000 pynchon-2024.4.3.17.15/src/pynchon/templates/scaffolds/github/.scaffold.advice.json5
+-rw-r--r--   0 runner    (1001) docker     (127)      458 2024-04-03 17:10:52.000000 pynchon-2024.4.3.17.15/src/pynchon/templates/scaffolds/github/README.md.j2
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:15:50.199285 pynchon-2024.4.3.17.15/src/pynchon/templates/scaffolds/py/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:15:50.235285 pynchon-2024.4.3.17.15/src/pynchon/templates/scaffolds/py/pkg/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 17:10:52.000000 pynchon-2024.4.3.17.15/src/pynchon/templates/scaffolds/py/pkg/.ackrc
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 17:10:52.000000 pynchon-2024.4.3.17.15/src/pynchon/templates/scaffolds/py/pkg/.flake8
+-rw-r--r--   0 runner    (1001) docker     (127)      776 2024-04-03 17:10:52.000000 pynchon-2024.4.3.17.15/src/pynchon/templates/scaffolds/py/pkg/.libcst.codemod.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       64 2024-04-03 17:10:52.000000 pynchon-2024.4.3.17.15/src/pynchon/templates/scaffolds/py/pkg/.scaffold.advice.json5
+-rw-r--r--   0 runner    (1001) docker     (127)     1928 2024-04-03 17:10:52.000000 pynchon-2024.4.3.17.15/src/pynchon/templates/scaffolds/py/pkg/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)     2233 2024-04-03 17:10:52.000000 pynchon-2024.4.3.17.15/src/pynchon/templates/scaffolds/py/pkg/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1549 2024-04-03 17:10:52.000000 pynchon-2024.4.3.17.15/src/pynchon/templates/scaffolds/py/pkg/README.md.j2
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:15:50.235285 pynchon-2024.4.3.17.15/src/pynchon/templates/scaffolds/py/pkg/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 17:10:52.000000 pynchon-2024.4.3.17.15/src/pynchon/templates/scaffolds/py/pkg/docs/.gitkeep
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:15:50.235285 pynchon-2024.4.3.17.15/src/pynchon/templates/scaffolds/py/pkg/docs/html/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 17:10:52.000000 pynchon-2024.4.3.17.15/src/pynchon/templates/scaffolds/py/pkg/docs/html/.gitkeep
+-rw-r--r--   0 runner    (1001) docker     (127)     2396 2024-04-03 17:10:52.000000 pynchon-2024.4.3.17.15/src/pynchon/templates/scaffolds/py/pkg/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      771 2024-04-03 17:10:52.000000 pynchon-2024.4.3.17.15/src/pynchon/templates/scaffolds/py/pkg/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:15:50.199285 pynchon-2024.4.3.17.15/src/pynchon/templates/scaffolds/py/pkg/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:15:50.235285 pynchon-2024.4.3.17.15/src/pynchon/templates/scaffolds/py/pkg/src/{{name}}/
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-03 17:10:52.000000 pynchon-2024.4.3.17.15/src/pynchon/templates/scaffolds/py/pkg/src/{{name}}/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-03 17:10:52.000000 pynchon-2024.4.3.17.15/src/pynchon/templates/scaffolds/py/pkg/src/{{name}}/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-03 17:10:52.000000 pynchon-2024.4.3.17.15/src/pynchon/templates/scaffolds/py/pkg/src/{{name}}/app.py
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-03 17:10:52.000000 pynchon-2024.4.3.17.15/src/pynchon/templates/scaffolds/py/pkg/src/{{name}}/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-04-03 17:10:52.000000 pynchon-2024.4.3.17.15/src/pynchon/templates/scaffolds/py/pkg/src/{{name}}/lme.py
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-03 17:10:52.000000 pynchon-2024.4.3.17.15/src/pynchon/templates/scaffolds/py/pkg/src/{{name}}/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-04-03 17:10:52.000000 pynchon-2024.4.3.17.15/src/pynchon/templates/scaffolds/py/pkg/src/{{name}}/tagging.py
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-03 17:10:52.000000 pynchon-2024.4.3.17.15/src/pynchon/templates/scaffolds/py/pkg/src/{{name}}/typing.py
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-03 17:10:52.000000 pynchon-2024.4.3.17.15/src/pynchon/templates/scaffolds/py/pkg/src/{{name}}/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:15:50.239285 pynchon-2024.4.3.17.15/src/pynchon/templates/scaffolds/py/pkg/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 17:10:52.000000 pynchon-2024.4.3.17.15/src/pynchon/templates/scaffolds/py/pkg/tests/.gitkeep
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 17:10:52.000000 pynchon-2024.4.3.17.15/src/pynchon/templates/scaffolds/py/pkg/tests/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:15:50.239285 pynchon-2024.4.3.17.15/src/pynchon/templates/scaffolds/py/pkg/tests/integration/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 17:10:52.000000 pynchon-2024.4.3.17.15/src/pynchon/templates/scaffolds/py/pkg/tests/integration/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-03 17:10:52.000000 pynchon-2024.4.3.17.15/src/pynchon/templates/scaffolds/py/pkg/tests/integration/test_all.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:15:50.239285 pynchon-2024.4.3.17.15/src/pynchon/templates/scaffolds/py/pkg/tests/smoke/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 17:10:52.000000 pynchon-2024.4.3.17.15/src/pynchon/templates/scaffolds/py/pkg/tests/smoke/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-03 17:10:52.000000 pynchon-2024.4.3.17.15/src/pynchon/templates/scaffolds/py/pkg/tests/smoke/test_all.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:15:50.239285 pynchon-2024.4.3.17.15/src/pynchon/templates/scaffolds/py/pkg/tests/units/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 17:10:52.000000 pynchon-2024.4.3.17.15/src/pynchon/templates/scaffolds/py/pkg/tests/units/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-03 17:10:52.000000 pynchon-2024.4.3.17.15/src/pynchon/templates/scaffolds/py/pkg/tests/units/test_all.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3097 2024-04-03 17:10:52.000000 pynchon-2024.4.3.17.15/src/pynchon/templates/scaffolds/py/pkg/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:15:50.239285 pynchon-2024.4.3.17.15/src/pynchon/templates/scaffolds/py/workspace/
+-rw-r--r--   0 runner    (1001) docker     (127)       64 2024-04-03 17:10:52.000000 pynchon-2024.4.3.17.15/src/pynchon/templates/scaffolds/py/workspace/.scaffold.advice.json5
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:15:50.199285 pynchon-2024.4.3.17.15/src/pynchon/templates/scaffolds/software/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:15:50.239285 pynchon-2024.4.3.17.15/src/pynchon/templates/scaffolds/software/automation/
+-rw-r--r--   0 runner    (1001) docker     (127)      348 2024-04-03 17:10:52.000000 pynchon-2024.4.3.17.15/src/pynchon/templates/scaffolds/software/automation/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:15:50.239285 pynchon-2024.4.3.17.15/src/pynchon/templates/scaffolds/software/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      348 2024-04-03 17:10:52.000000 pynchon-2024.4.3.17.15/src/pynchon/templates/scaffolds/software/tests/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:15:50.203285 pynchon-2024.4.3.17.15/src/pynchon/templates/scaffolds/software/tests/tests/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:15:50.239285 pynchon-2024.4.3.17.15/src/pynchon/templates/scaffolds/software/tests/tests/integration/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 17:10:52.000000 pynchon-2024.4.3.17.15/src/pynchon/templates/scaffolds/software/tests/tests/integration/.gitkeep
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:15:50.239285 pynchon-2024.4.3.17.15/src/pynchon/templates/scaffolds/software/tests/tests/smoke/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 17:10:52.000000 pynchon-2024.4.3.17.15/src/pynchon/templates/scaffolds/software/tests/tests/smoke/.gitkeep
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:15:50.239285 pynchon-2024.4.3.17.15/src/pynchon/templates/scaffolds/software/tests/tests/units/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 17:10:52.000000 pynchon-2024.4.3.17.15/src/pynchon/templates/scaffolds/software/tests/tests/units/.gitkeep
+-rw-r--r--   0 runner    (1001) docker     (127)      284 2024-04-03 17:10:52.000000 pynchon-2024.4.3.17.15/src/pynchon/testing.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:15:50.243285 pynchon-2024.4.3.17.15/src/pynchon/util/
+-rw-r--r--   0 runner    (1001) docker     (127)     1055 2024-04-03 17:10:52.000000 pynchon-2024.4.3.17.15/src/pynchon/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-03 17:10:52.000000 pynchon-2024.4.3.17.15/src/pynchon/util/click.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6160 2024-04-03 17:11:58.000000 pynchon-2024.4.3.17.15/src/pynchon/util/complexity.py
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-03 17:10:52.000000 pynchon-2024.4.3.17.15/src/pynchon/util/config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:15:50.243285 pynchon-2024.4.3.17.15/src/pynchon/util/console/
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-03 17:10:52.000000 pynchon-2024.4.3.17.15/src/pynchon/util/console/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-03 17:10:52.000000 pynchon-2024.4.3.17.15/src/pynchon/util/console/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4662 2024-04-03 17:10:52.000000 pynchon-2024.4.3.17.15/src/pynchon/util/docker.py
+-rw-r--r--   0 runner    (1001) docker     (127)      711 2024-04-03 17:11:58.000000 pynchon-2024.4.3.17.15/src/pynchon/util/events.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:15:50.243285 pynchon-2024.4.3.17.15/src/pynchon/util/files/
+-rw-r--r--   0 runner    (1001) docker     (127)     3902 2024-04-03 17:11:58.000000 pynchon-2024.4.3.17.15/src/pynchon/util/files/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      948 2024-04-03 17:11:58.000000 pynchon-2024.4.3.17.15/src/pynchon/util/files/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2089 2024-04-03 17:11:58.000000 pynchon-2024.4.3.17.15/src/pynchon/util/files/diff.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2608 2024-04-03 17:11:58.000000 pynchon-2024.4.3.17.15/src/pynchon/util/lme.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:15:50.243285 pynchon-2024.4.3.17.15/src/pynchon/util/makefile/
+-rw-r--r--   0 runner    (1001) docker     (127)     5276 2024-04-03 17:11:58.000000 pynchon-2024.4.3.17.15/src/pynchon/util/makefile/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      484 2024-04-03 17:11:58.000000 pynchon-2024.4.3.17.15/src/pynchon/util/makefile/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1139 2024-04-03 17:10:52.000000 pynchon-2024.4.3.17.15/src/pynchon/util/oop.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:15:50.243285 pynchon-2024.4.3.17.15/src/pynchon/util/os/
+-rw-r--r--   0 runner    (1001) docker     (127)      578 2024-04-03 17:10:52.000000 pynchon-2024.4.3.17.15/src/pynchon/util/os/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5760 2024-04-03 17:10:52.000000 pynchon-2024.4.3.17.15/src/pynchon/util/os/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-04-03 17:10:52.000000 pynchon-2024.4.3.17.15/src/pynchon/util/os/pidfile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1081 2024-04-03 17:10:52.000000 pynchon-2024.4.3.17.15/src/pynchon/util/os/pids.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2054 2024-04-03 17:10:52.000000 pynchon-2024.4.3.17.15/src/pynchon/util/python.py
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-04-03 17:10:52.000000 pynchon-2024.4.3.17.15/src/pynchon/util/splitvt.py
+-rw-r--r--   0 runner    (1001) docker     (127)      463 2024-04-03 17:10:52.000000 pynchon-2024.4.3.17.15/src/pynchon/util/testing.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:15:50.251285 pynchon-2024.4.3.17.15/src/pynchon/util/text/
+-rw-r--r--   0 runner    (1001) docker     (127)      551 2024-04-03 17:10:52.000000 pynchon-2024.4.3.17.15/src/pynchon/util/text/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      367 2024-04-03 17:11:58.000000 pynchon-2024.4.3.17.15/src/pynchon/util/text/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:15:50.251285 pynchon-2024.4.3.17.15/src/pynchon/util/text/dumpf/
+-rw-r--r--   0 runner    (1001) docker     (127)      790 2024-04-03 17:11:58.000000 pynchon-2024.4.3.17.15/src/pynchon/util/text/dumpf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1047 2024-04-03 17:11:58.000000 pynchon-2024.4.3.17.15/src/pynchon/util/text/dumpf/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      598 2024-04-03 17:10:52.000000 pynchon-2024.4.3.17.15/src/pynchon/util/text/dumps.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:15:50.251285 pynchon-2024.4.3.17.15/src/pynchon/util/text/loadf/
+-rw-r--r--   0 runner    (1001) docker     (127)     7414 2024-04-03 17:11:58.000000 pynchon-2024.4.3.17.15/src/pynchon/util/text/loadf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1042 2024-04-03 17:11:58.000000 pynchon-2024.4.3.17.15/src/pynchon/util/text/loadf/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1950 2024-04-03 17:11:58.000000 pynchon-2024.4.3.17.15/src/pynchon/util/text/loads.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:15:50.251285 pynchon-2024.4.3.17.15/src/pynchon/util/text/normalize/
+-rw-r--r--   0 runner    (1001) docker     (127)     1285 2024-04-03 17:10:52.000000 pynchon-2024.4.3.17.15/src/pynchon/util/text/normalize/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:15:50.251285 pynchon-2024.4.3.17.15/src/pynchon/util/text/render/
+-rw-r--r--   0 runner    (1001) docker     (127)     5825 2024-04-03 17:11:58.000000 pynchon-2024.4.3.17.15/src/pynchon/util/text/render/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      972 2024-04-03 17:11:58.000000 pynchon-2024.4.3.17.15/src/pynchon/util/text/render/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1395 2024-04-03 17:10:52.000000 pynchon-2024.4.3.17.15/src/pynchon/util/typing.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:15:50.251285 pynchon-2024.4.3.17.15/src/pynchon.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1714 2024-04-03 17:15:50.000000 pynchon-2024.4.3.17.15/src/pynchon.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     9272 2024-04-03 17:15:50.000000 pynchon-2024.4.3.17.15/src/pynchon.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 17:15:50.000000 pynchon-2024.4.3.17.15/src/pynchon.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-04-03 17:15:50.000000 pynchon-2024.4.3.17.15/src/pynchon.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 17:15:50.000000 pynchon-2024.4.3.17.15/src/pynchon.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      438 2024-04-03 17:15:50.000000 pynchon-2024.4.3.17.15/src/pynchon.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-03 17:15:50.000000 pynchon-2024.4.3.17.15/src/pynchon.egg-info/top_level.txt
```

### Comparing `pynchon-2024.4.3.17.11/PKG-INFO` & `pynchon-2024.4.3.17.15/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pynchon
-Version: 2024.4.3.17.11
+Version: 2024.4.3.17.15
 Summary: Autodocs for python projects
 Home-page: https://github.com/elo-enterprises/pynchon/
 Author: elo
 Author-email: engineering@elo.enterprises
 License: MIT
 Project-URL: Documentation, https://github.com/elo-enterprises/pynchon/
 Project-URL: Source, https://github.com/elo-enterprises/pynchon/
```

### Comparing `pynchon-2024.4.3.17.11/README.md` & `pynchon-2024.4.3.17.15/README.md`

 * *Files identical despite different names*

### Comparing `pynchon-2024.4.3.17.11/pyproject.toml` & `pynchon-2024.4.3.17.15/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pynchon-2024.4.3.17.11/setup.cfg` & `pynchon-2024.4.3.17.15/setup.cfg`

 * *Files identical despite different names*

### Comparing `pynchon-2024.4.3.17.11/setup.py` & `pynchon-2024.4.3.17.15/setup.py`

 * *Files identical despite different names*

### Comparing `pynchon-2024.4.3.17.11/src/pynchon/abcs/attrdict.py` & `pynchon-2024.4.3.17.15/src/pynchon/abcs/attrdict.py`

 * *Files identical despite different names*

### Comparing `pynchon-2024.4.3.17.11/src/pynchon/abcs/path.py` & `pynchon-2024.4.3.17.15/src/pynchon/abcs/path.py`

 * *Files identical despite different names*

### Comparing `pynchon-2024.4.3.17.11/src/pynchon/abcs/visitor.py` & `pynchon-2024.4.3.17.15/src/pynchon/abcs/visitor.py`

 * *Files identical despite different names*

### Comparing `pynchon-2024.4.3.17.11/src/pynchon/annotate.py` & `pynchon-2024.4.3.17.15/src/pynchon/annotate.py`

 * *Files identical despite different names*

### Comparing `pynchon-2024.4.3.17.11/src/pynchon/api/project/__init__.py` & `pynchon-2024.4.3.17.15/src/pynchon/api/project/__init__.py`

 * *Files identical despite different names*

### Comparing `pynchon-2024.4.3.17.11/src/pynchon/api/render.py` & `pynchon-2024.4.3.17.15/src/pynchon/api/render.py`

 * *Files identical despite different names*

### Comparing `pynchon-2024.4.3.17.11/src/pynchon/app.py` & `pynchon-2024.4.3.17.15/src/pynchon/app.py`

 * *Files identical despite different names*

### Comparing `pynchon-2024.4.3.17.11/src/pynchon/bin.py` & `pynchon-2024.4.3.17.15/src/pynchon/bin.py`

 * *Files identical despite different names*

### Comparing `pynchon-2024.4.3.17.11/src/pynchon/cli/common.py` & `pynchon-2024.4.3.17.15/src/pynchon/cli/common.py`

 * *Files identical despite different names*

### Comparing `pynchon-2024.4.3.17.11/src/pynchon/codemod/commands/docstrings/base.py` & `pynchon-2024.4.3.17.15/src/pynchon/codemod/commands/docstrings/base.py`

 * *Files identical despite different names*

### Comparing `pynchon-2024.4.3.17.11/src/pynchon/codemod/commands/docstrings/javadoc.py` & `pynchon-2024.4.3.17.15/src/pynchon/codemod/commands/docstrings/javadoc.py`

 * *Files identical despite different names*

### Comparing `pynchon-2024.4.3.17.11/src/pynchon/codemod/commands/docstrings/simple.py` & `pynchon-2024.4.3.17.15/src/pynchon/codemod/commands/docstrings/simple.py`

 * *Files identical despite different names*

### Comparing `pynchon-2024.4.3.17.11/src/pynchon/config/__init__.py` & `pynchon-2024.4.3.17.15/src/pynchon/config/__init__.py`

 * *Files identical despite different names*

### Comparing `pynchon-2024.4.3.17.11/src/pynchon/config/util.py` & `pynchon-2024.4.3.17.15/src/pynchon/config/util.py`

 * *Files identical despite different names*

### Comparing `pynchon-2024.4.3.17.11/src/pynchon/constants.py` & `pynchon-2024.4.3.17.15/src/pynchon/constants.py`

 * *Files identical despite different names*

### Comparing `pynchon-2024.4.3.17.11/src/pynchon/core.py` & `pynchon-2024.4.3.17.15/src/pynchon/core.py`

 * *Files identical despite different names*

### Comparing `pynchon-2024.4.3.17.11/src/pynchon/events.py` & `pynchon-2024.4.3.17.15/src/pynchon/events.py`

 * *Files identical despite different names*

### Comparing `pynchon-2024.4.3.17.11/src/pynchon/models/planner.py` & `pynchon-2024.4.3.17.15/src/pynchon/models/planner.py`

 * *Files identical despite different names*

### Comparing `pynchon-2024.4.3.17.11/src/pynchon/models/planning.py` & `pynchon-2024.4.3.17.15/src/pynchon/models/planning.py`

 * *Files identical despite different names*

### Comparing `pynchon-2024.4.3.17.11/src/pynchon/models/plugins/__init__.py` & `pynchon-2024.4.3.17.15/src/pynchon/models/plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `pynchon-2024.4.3.17.11/src/pynchon/models/plugins/cli.py` & `pynchon-2024.4.3.17.15/src/pynchon/models/plugins/cli.py`

 * *Files identical despite different names*

### Comparing `pynchon-2024.4.3.17.11/src/pynchon/models/plugins/docker.py` & `pynchon-2024.4.3.17.15/src/pynchon/models/plugins/docker.py`

 * *Files identical despite different names*

### Comparing `pynchon-2024.4.3.17.11/src/pynchon/models/plugins/provider.py` & `pynchon-2024.4.3.17.15/src/pynchon/models/plugins/provider.py`

 * *Files identical despite different names*

### Comparing `pynchon-2024.4.3.17.11/src/pynchon/models/plugins/pynchon.py` & `pynchon-2024.4.3.17.15/src/pynchon/models/plugins/pynchon.py`

 * *Files identical despite different names*

### Comparing `pynchon-2024.4.3.17.11/src/pynchon/models/plugins/tool.py` & `pynchon-2024.4.3.17.15/src/pynchon/models/plugins/tool.py`

 * *Files identical despite different names*

### Comparing `pynchon-2024.4.3.17.11/src/pynchon/models/plugins/validators.py` & `pynchon-2024.4.3.17.15/src/pynchon/models/plugins/validators.py`

 * *Files identical despite different names*

### Comparing `pynchon-2024.4.3.17.11/src/pynchon/models/python.py` & `pynchon-2024.4.3.17.15/src/pynchon/models/python.py`

 * *Files identical despite different names*

### Comparing `pynchon-2024.4.3.17.11/src/pynchon/plugins/__init__.py` & `pynchon-2024.4.3.17.15/src/pynchon/plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `pynchon-2024.4.3.17.11/src/pynchon/plugins/cicd.py` & `pynchon-2024.4.3.17.15/src/pynchon/plugins/cicd.py`

 * *Files identical despite different names*

### Comparing `pynchon-2024.4.3.17.11/src/pynchon/plugins/core.py` & `pynchon-2024.4.3.17.15/src/pynchon/plugins/core.py`

 * *Files identical despite different names*

### Comparing `pynchon-2024.4.3.17.11/src/pynchon/plugins/deck.py` & `pynchon-2024.4.3.17.15/src/pynchon/plugins/deck.py`

 * *Files identical despite different names*

### Comparing `pynchon-2024.4.3.17.11/src/pynchon/plugins/dockerhub.py` & `pynchon-2024.4.3.17.15/src/pynchon/plugins/dockerhub.py`

 * *Files identical despite different names*

### Comparing `pynchon-2024.4.3.17.11/src/pynchon/plugins/docs/main.py` & `pynchon-2024.4.3.17.15/src/pynchon/plugins/docs/main.py`

 * *Files identical despite different names*

### Comparing `pynchon-2024.4.3.17.11/src/pynchon/plugins/docs/opener.py` & `pynchon-2024.4.3.17.15/src/pynchon/plugins/docs/opener.py`

 * *Files identical despite different names*

### Comparing `pynchon-2024.4.3.17.11/src/pynchon/plugins/dot.py` & `pynchon-2024.4.3.17.15/src/pynchon/plugins/dot.py`

 * *Files identical despite different names*

### Comparing `pynchon-2024.4.3.17.11/src/pynchon/plugins/drawio.py` & `pynchon-2024.4.3.17.15/src/pynchon/plugins/drawio.py`

 * *Files identical despite different names*

### Comparing `pynchon-2024.4.3.17.11/src/pynchon/plugins/fixme.py` & `pynchon-2024.4.3.17.15/src/pynchon/plugins/fixme.py`

 * *Files identical despite different names*

### Comparing `pynchon-2024.4.3.17.11/src/pynchon/plugins/gen.py` & `pynchon-2024.4.3.17.15/src/pynchon/plugins/gen.py`

 * *Files identical despite different names*

### Comparing `pynchon-2024.4.3.17.11/src/pynchon/plugins/git.py` & `pynchon-2024.4.3.17.15/src/pynchon/plugins/git.py`

 * *Files identical despite different names*

### Comparing `pynchon-2024.4.3.17.11/src/pynchon/plugins/github.py` & `pynchon-2024.4.3.17.15/src/pynchon/plugins/github.py`

 * *Files identical despite different names*

### Comparing `pynchon-2024.4.3.17.11/src/pynchon/plugins/griffe.py` & `pynchon-2024.4.3.17.15/src/pynchon/plugins/griffe.py`

 * *Files identical despite different names*

### Comparing `pynchon-2024.4.3.17.11/src/pynchon/plugins/jinja.py` & `pynchon-2024.4.3.17.15/src/pynchon/plugins/jinja.py`

 * *Files identical despite different names*

### Comparing `pynchon-2024.4.3.17.11/src/pynchon/plugins/json.py` & `pynchon-2024.4.3.17.15/src/pynchon/plugins/json.py`

 * *Files identical despite different names*

### Comparing `pynchon-2024.4.3.17.11/src/pynchon/plugins/makefile.py` & `pynchon-2024.4.3.17.15/src/pynchon/plugins/makefile.py`

 * *Files identical despite different names*

### Comparing `pynchon-2024.4.3.17.11/src/pynchon/plugins/markdown.py` & `pynchon-2024.4.3.17.15/src/pynchon/plugins/markdown.py`

 * *Files identical despite different names*

### Comparing `pynchon-2024.4.3.17.11/src/pynchon/plugins/mermaid.py` & `pynchon-2024.4.3.17.15/src/pynchon/plugins/mermaid.py`

 * *Files identical despite different names*

### Comparing `pynchon-2024.4.3.17.11/src/pynchon/plugins/mkdocs.py` & `pynchon-2024.4.3.17.15/src/pynchon/plugins/mkdocs.py`

 * *Files identical despite different names*

### Comparing `pynchon-2024.4.3.17.11/src/pynchon/plugins/pandoc.py` & `pynchon-2024.4.3.17.15/src/pynchon/plugins/pandoc.py`

 * *Files identical despite different names*

### Comparing `pynchon-2024.4.3.17.11/src/pynchon/plugins/pattern.py` & `pynchon-2024.4.3.17.15/src/pynchon/plugins/pattern.py`

 * *Files identical despite different names*

### Comparing `pynchon-2024.4.3.17.11/src/pynchon/plugins/plugins.py` & `pynchon-2024.4.3.17.15/src/pynchon/plugins/plugins.py`

 * *Files identical despite different names*

### Comparing `pynchon-2024.4.3.17.11/src/pynchon/plugins/project.py` & `pynchon-2024.4.3.17.15/src/pynchon/plugins/project.py`

 * *Files identical despite different names*

### Comparing `pynchon-2024.4.3.17.11/src/pynchon/plugins/python/api.py` & `pynchon-2024.4.3.17.15/src/pynchon/plugins/python/api.py`

 * *Files identical despite different names*

### Comparing `pynchon-2024.4.3.17.11/src/pynchon/plugins/python/cli.py` & `pynchon-2024.4.3.17.15/src/pynchon/plugins/python/cli.py`

 * *Files identical despite different names*

### Comparing `pynchon-2024.4.3.17.11/src/pynchon/plugins/python/libcst.py` & `pynchon-2024.4.3.17.15/src/pynchon/plugins/python/libcst.py`

 * *Files identical despite different names*

### Comparing `pynchon-2024.4.3.17.11/src/pynchon/plugins/python/platform.py` & `pynchon-2024.4.3.17.15/src/pynchon/plugins/python/platform.py`

 * *Files identical despite different names*

### Comparing `pynchon-2024.4.3.17.11/src/pynchon/plugins/python/pypi.py` & `pynchon-2024.4.3.17.15/src/pynchon/plugins/python/pypi.py`

 * *Files identical despite different names*

### Comparing `pynchon-2024.4.3.17.11/src/pynchon/plugins/release.py` & `pynchon-2024.4.3.17.15/src/pynchon/plugins/release.py`

 * *Files identical despite different names*

### Comparing `pynchon-2024.4.3.17.11/src/pynchon/plugins/render.py` & `pynchon-2024.4.3.17.15/src/pynchon/plugins/render.py`

 * *Files identical despite different names*

### Comparing `pynchon-2024.4.3.17.11/src/pynchon/plugins/scaffolding/__init__.py` & `pynchon-2024.4.3.17.15/src/pynchon/plugins/scaffolding/__init__.py`

 * *Files identical despite different names*

### Comparing `pynchon-2024.4.3.17.11/src/pynchon/plugins/scaffolding/config.py` & `pynchon-2024.4.3.17.15/src/pynchon/plugins/scaffolding/config.py`

 * *Files identical despite different names*

### Comparing `pynchon-2024.4.3.17.11/src/pynchon/plugins/src.py` & `pynchon-2024.4.3.17.15/src/pynchon/plugins/src.py`

 * *Files identical despite different names*

### Comparing `pynchon-2024.4.3.17.11/src/pynchon/plugins/tests.py` & `pynchon-2024.4.3.17.15/src/pynchon/plugins/tests.py`

 * *Files identical despite different names*

### Comparing `pynchon-2024.4.3.17.11/src/pynchon/plugins/util.py` & `pynchon-2024.4.3.17.15/src/pynchon/plugins/util.py`

 * *Files identical despite different names*

### Comparing `pynchon-2024.4.3.17.11/src/pynchon/templates/docker/Dockerfile.pandoc` & `pynchon-2024.4.3.17.15/src/pynchon/templates/docker/Dockerfile.pandoc`

 * *Files identical despite different names*

### Comparing `pynchon-2024.4.3.17.11/src/pynchon/templates/includes/pynchon/plugins/core/bootstrap/bash.sh` & `pynchon-2024.4.3.17.15/src/pynchon/templates/includes/pynchon/plugins/core/bootstrap/bash.sh`

 * *Files identical despite different names*

### Comparing `pynchon-2024.4.3.17.11/src/pynchon/templates/includes/pynchon/plugins/core/bootstrap/bashrc.sh` & `pynchon-2024.4.3.17.15/src/pynchon/templates/includes/pynchon/plugins/core/bootstrap/bashrc.sh`

 * *Files identical despite different names*

### Comparing `pynchon-2024.4.3.17.11/src/pynchon/templates/includes/pynchon/plugins/core/bootstrap/tox.ini` & `pynchon-2024.4.3.17.15/src/pynchon/templates/includes/pynchon/plugins/core/bootstrap/tox.ini`

 * *Files identical despite different names*

### Comparing `pynchon-2024.4.3.17.11/src/pynchon/templates/includes/pynchon/plugins/makefile/mermaid-graph.mmd.j2` & `pynchon-2024.4.3.17.15/src/pynchon/templates/includes/pynchon/plugins/makefile/mermaid-graph.mmd.j2`

 * *Files identical despite different names*

### Comparing `pynchon-2024.4.3.17.11/src/pynchon/templates/includes/pynchon/plugins/python/api/classes.md.j2` & `pynchon-2024.4.3.17.15/src/pynchon/templates/includes/pynchon/plugins/python/api/classes.md.j2`

 * *Files identical despite different names*

### Comparing `pynchon-2024.4.3.17.11/src/pynchon/templates/includes/pynchon/plugins/python/api/functions.md.j2` & `pynchon-2024.4.3.17.15/src/pynchon/templates/includes/pynchon/plugins/python/api/functions.md.j2`

 * *Files identical despite different names*

### Comparing `pynchon-2024.4.3.17.11/src/pynchon/templates/includes/pynchon/plugins/python/api/package.md.j2` & `pynchon-2024.4.3.17.15/src/pynchon/templates/includes/pynchon/plugins/python/api/package.md.j2`

 * *Files identical despite different names*

### Comparing `pynchon-2024.4.3.17.11/src/pynchon/templates/includes/pynchon/plugins/python/api/toc2.md.j2` & `pynchon-2024.4.3.17.15/src/pynchon/templates/includes/pynchon/plugins/python/api/toc2.md.j2`

 * *Files identical despite different names*

### Comparing `pynchon-2024.4.3.17.11/src/pynchon/templates/includes/pynchon/plugins/python_cli/TOC.md.j2` & `pynchon-2024.4.3.17.15/src/pynchon/templates/includes/pynchon/plugins/python_cli/TOC.md.j2`

 * *Files identical despite different names*

### Comparing `pynchon-2024.4.3.17.11/src/pynchon/templates/includes/pynchon/plugins/python_cli/main.module.md.j2` & `pynchon-2024.4.3.17.15/src/pynchon/templates/includes/pynchon/plugins/python_cli/main.module.md.j2`

 * *Files identical despite different names*

### Comparing `pynchon-2024.4.3.17.11/src/pynchon/templates/includes/pynchon/plugins/python_cli/script.console.md.j2` & `pynchon-2024.4.3.17.15/src/pynchon/templates/includes/pynchon/plugins/python_cli/script.console.md.j2`

 * *Files identical despite different names*

### Comparing `pynchon-2024.4.3.17.11/src/pynchon/templates/scaffolds/docker/.dockerignore` & `pynchon-2024.4.3.17.15/src/pynchon/templates/scaffolds/docker/.dockerignore`

 * *Files identical despite different names*

### Comparing `pynchon-2024.4.3.17.11/src/pynchon/templates/scaffolds/docker/README.md.j2` & `pynchon-2024.4.3.17.15/src/pynchon/templates/scaffolds/docker/README.md.j2`

 * *Files identical despite different names*

### Comparing `pynchon-2024.4.3.17.11/src/pynchon/templates/scaffolds/py/pkg/.libcst.codemod.yaml` & `pynchon-2024.4.3.17.15/src/pynchon/templates/scaffolds/py/pkg/.libcst.codemod.yaml`

 * *Files identical despite different names*

### Comparing `pynchon-2024.4.3.17.11/src/pynchon/templates/scaffolds/py/pkg/Makefile` & `pynchon-2024.4.3.17.15/src/pynchon/templates/scaffolds/py/pkg/Makefile`

 * *Files identical despite different names*

### Comparing `pynchon-2024.4.3.17.11/src/pynchon/templates/scaffolds/py/pkg/README.md` & `pynchon-2024.4.3.17.15/src/pynchon/templates/scaffolds/py/pkg/README.md`

 * *Files identical despite different names*

### Comparing `pynchon-2024.4.3.17.11/src/pynchon/templates/scaffolds/py/pkg/README.md.j2` & `pynchon-2024.4.3.17.15/src/pynchon/templates/scaffolds/py/pkg/README.md.j2`

 * *Files identical despite different names*

### Comparing `pynchon-2024.4.3.17.11/src/pynchon/templates/scaffolds/py/pkg/setup.cfg` & `pynchon-2024.4.3.17.15/src/pynchon/templates/scaffolds/py/pkg/setup.cfg`

 * *Files identical despite different names*

### Comparing `pynchon-2024.4.3.17.11/src/pynchon/templates/scaffolds/py/pkg/setup.py` & `pynchon-2024.4.3.17.15/src/pynchon/templates/scaffolds/py/pkg/setup.py`

 * *Files identical despite different names*

### Comparing `pynchon-2024.4.3.17.11/src/pynchon/templates/scaffolds/py/pkg/tox.ini` & `pynchon-2024.4.3.17.15/src/pynchon/templates/scaffolds/py/pkg/tox.ini`

 * *Files identical despite different names*

### Comparing `pynchon-2024.4.3.17.11/src/pynchon/util/__init__.py` & `pynchon-2024.4.3.17.15/src/pynchon/util/__init__.py`

 * *Files identical despite different names*

### Comparing `pynchon-2024.4.3.17.11/src/pynchon/util/complexity.py` & `pynchon-2024.4.3.17.15/src/pynchon/util/complexity.py`

 * *Files identical despite different names*

### Comparing `pynchon-2024.4.3.17.11/src/pynchon/util/docker.py` & `pynchon-2024.4.3.17.15/src/pynchon/util/docker.py`

 * *Files identical despite different names*

### Comparing `pynchon-2024.4.3.17.11/src/pynchon/util/events.py` & `pynchon-2024.4.3.17.15/src/pynchon/util/events.py`

 * *Files identical despite different names*

### Comparing `pynchon-2024.4.3.17.11/src/pynchon/util/files/__init__.py` & `pynchon-2024.4.3.17.15/src/pynchon/util/files/__init__.py`

 * *Files identical despite different names*

### Comparing `pynchon-2024.4.3.17.11/src/pynchon/util/files/__main__.py` & `pynchon-2024.4.3.17.15/src/pynchon/util/files/__main__.py`

 * *Files identical despite different names*

### Comparing `pynchon-2024.4.3.17.11/src/pynchon/util/files/diff.py` & `pynchon-2024.4.3.17.15/src/pynchon/util/files/diff.py`

 * *Files identical despite different names*

### Comparing `pynchon-2024.4.3.17.11/src/pynchon/util/lme.py` & `pynchon-2024.4.3.17.15/src/pynchon/util/lme.py`

 * *Files identical despite different names*

### Comparing `pynchon-2024.4.3.17.11/src/pynchon/util/makefile/__init__.py` & `pynchon-2024.4.3.17.15/src/pynchon/util/makefile/__init__.py`

 * *Files identical despite different names*

### Comparing `pynchon-2024.4.3.17.11/src/pynchon/util/oop.py` & `pynchon-2024.4.3.17.15/src/pynchon/util/oop.py`

 * *Files identical despite different names*

### Comparing `pynchon-2024.4.3.17.11/src/pynchon/util/os/__init__.py` & `pynchon-2024.4.3.17.15/src/pynchon/util/os/__init__.py`

 * *Files identical despite different names*

### Comparing `pynchon-2024.4.3.17.11/src/pynchon/util/os/models.py` & `pynchon-2024.4.3.17.15/src/pynchon/util/os/models.py`

 * *Files identical despite different names*

### Comparing `pynchon-2024.4.3.17.11/src/pynchon/util/os/pids.py` & `pynchon-2024.4.3.17.15/src/pynchon/util/os/pids.py`

 * *Files identical despite different names*

### Comparing `pynchon-2024.4.3.17.11/src/pynchon/util/python.py` & `pynchon-2024.4.3.17.15/src/pynchon/util/python.py`

 * *Files identical despite different names*

### Comparing `pynchon-2024.4.3.17.11/src/pynchon/util/text/__init__.py` & `pynchon-2024.4.3.17.15/src/pynchon/util/text/__init__.py`

 * *Files identical despite different names*

### Comparing `pynchon-2024.4.3.17.11/src/pynchon/util/text/dumpf/__init__.py` & `pynchon-2024.4.3.17.15/src/pynchon/util/text/dumpf/__init__.py`

 * *Files identical despite different names*

### Comparing `pynchon-2024.4.3.17.11/src/pynchon/util/text/dumpf/__main__.py` & `pynchon-2024.4.3.17.15/src/pynchon/util/text/dumpf/__main__.py`

 * *Files identical despite different names*

### Comparing `pynchon-2024.4.3.17.11/src/pynchon/util/text/dumps.py` & `pynchon-2024.4.3.17.15/src/pynchon/util/text/dumps.py`

 * *Files identical despite different names*

### Comparing `pynchon-2024.4.3.17.11/src/pynchon/util/text/loadf/__init__.py` & `pynchon-2024.4.3.17.15/src/pynchon/util/text/loadf/__init__.py`

 * *Files identical despite different names*

### Comparing `pynchon-2024.4.3.17.11/src/pynchon/util/text/loadf/__main__.py` & `pynchon-2024.4.3.17.15/src/pynchon/util/text/loadf/__main__.py`

 * *Files identical despite different names*

### Comparing `pynchon-2024.4.3.17.11/src/pynchon/util/text/loads.py` & `pynchon-2024.4.3.17.15/src/pynchon/util/text/loads.py`

 * *Files identical despite different names*

### Comparing `pynchon-2024.4.3.17.11/src/pynchon/util/text/normalize/__init__.py` & `pynchon-2024.4.3.17.15/src/pynchon/util/text/normalize/__init__.py`

 * *Files identical despite different names*

### Comparing `pynchon-2024.4.3.17.11/src/pynchon/util/text/render/__init__.py` & `pynchon-2024.4.3.17.15/src/pynchon/util/text/render/__init__.py`

 * *Files identical despite different names*

### Comparing `pynchon-2024.4.3.17.11/src/pynchon/util/text/render/__main__.py` & `pynchon-2024.4.3.17.15/src/pynchon/util/text/render/__main__.py`

 * *Files identical despite different names*

### Comparing `pynchon-2024.4.3.17.11/src/pynchon/util/typing.py` & `pynchon-2024.4.3.17.15/src/pynchon/util/typing.py`

 * *Files identical despite different names*

### Comparing `pynchon-2024.4.3.17.11/src/pynchon.egg-info/PKG-INFO` & `pynchon-2024.4.3.17.15/src/pynchon.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pynchon
-Version: 2024.4.3.17.11
+Version: 2024.4.3.17.15
 Summary: Autodocs for python projects
 Home-page: https://github.com/elo-enterprises/pynchon/
 Author: elo
 Author-email: engineering@elo.enterprises
 License: MIT
 Project-URL: Documentation, https://github.com/elo-enterprises/pynchon/
 Project-URL: Source, https://github.com/elo-enterprises/pynchon/
```

### Comparing `pynchon-2024.4.3.17.11/src/pynchon.egg-info/SOURCES.txt` & `pynchon-2024.4.3.17.15/src/pynchon.egg-info/SOURCES.txt`

 * *Files identical despite different names*

