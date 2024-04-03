# Comparing `tmp/pynchon-2024.3.5.19.3.tar.gz` & `tmp/pynchon-2024.4.3.17.11.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pynchon-2024.3.5.19.3.tar", last modified: Tue Mar  5 19:03:52 2024, max compression
+gzip compressed data, was "pynchon-2024.4.3.17.11.tar", last modified: Wed Apr  3 17:11:27 2024, max compression
```

## Comparing `pynchon-2024.3.5.19.3.tar` & `pynchon-2024.4.3.17.11.tar`

### file list

```diff
@@ -1,293 +1,297 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 19:03:52.481036 pynchon-2024.3.5.19.3/
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-03-05 18:58:59.000000 pynchon-2024.3.5.19.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1736 2024-03-05 19:03:52.481036 pynchon-2024.3.5.19.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    13478 2024-03-05 18:58:59.000000 pynchon-2024.3.5.19.3/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      979 2024-03-05 18:58:59.000000 pynchon-2024.3.5.19.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1714 2024-03-05 19:03:52.485036 pynchon-2024.3.5.19.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      770 2024-03-05 18:58:59.000000 pynchon-2024.3.5.19.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 19:03:52.449036 pynchon-2024.3.5.19.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 19:03:52.457036 pynchon-2024.3.5.19.3/src/pynchon/
--rw-r--r--   0 runner    (1001) docker     (127)      259 2024-03-05 18:58:59.000000 pynchon-2024.3.5.19.3/src/pynchon/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       96 2024-03-05 18:58:59.000000 pynchon-2024.3.5.19.3/src/pynchon/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-03-05 19:03:48.000000 pynchon-2024.3.5.19.3/src/pynchon/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 19:03:52.457036 pynchon-2024.3.5.19.3/src/pynchon/abcs/
--rw-r--r--   0 runner    (1001) docker     (127)      319 2024-03-05 18:58:59.000000 pynchon-2024.3.5.19.3/src/pynchon/abcs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1503 2024-03-05 18:58:59.000000 pynchon-2024.3.5.19.3/src/pynchon/abcs/attrdict.py
--rw-r--r--   0 runner    (1001) docker     (127)      115 2024-03-05 18:58:59.000000 pynchon-2024.3.5.19.3/src/pynchon/abcs/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     2011 2024-03-05 18:58:59.000000 pynchon-2024.3.5.19.3/src/pynchon/abcs/path.py
--rw-r--r--   0 runner    (1001) docker     (127)     5484 2024-03-05 18:58:59.000000 pynchon-2024.3.5.19.3/src/pynchon/abcs/visitor.py
--rw-r--r--   0 runner    (1001) docker     (127)     5088 2024-03-05 19:00:00.000000 pynchon-2024.3.5.19.3/src/pynchon/annotate.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 19:03:52.457036 pynchon-2024.3.5.19.3/src/pynchon/api/
--rw-r--r--   0 runner    (1001) docker     (127)       68 2024-03-05 18:58:59.000000 pynchon-2024.3.5.19.3/src/pynchon/api/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 19:03:52.457036 pynchon-2024.3.5.19.3/src/pynchon/api/git/
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-03-05 18:58:59.000000 pynchon-2024.3.5.19.3/src/pynchon/api/git/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 19:03:52.457036 pynchon-2024.3.5.19.3/src/pynchon/api/parsers/
--rw-r--r--   0 runner    (1001) docker     (127)       61 2024-03-05 18:58:59.000000 pynchon-2024.3.5.19.3/src/pynchon/api/parsers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 19:03:52.457036 pynchon-2024.3.5.19.3/src/pynchon/api/project/
--rw-r--r--   0 runner    (1001) docker     (127)     1203 2024-03-05 18:58:59.000000 pynchon-2024.3.5.19.3/src/pynchon/api/project/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-03-05 18:58:59.000000 pynchon-2024.3.5.19.3/src/pynchon/api/pynchon.py
--rw-r--r--   0 runner    (1001) docker     (127)     4540 2024-03-05 19:00:00.000000 pynchon-2024.3.5.19.3/src/pynchon/api/render.py
--rw-r--r--   0 runner    (1001) docker     (127)     5262 2024-03-05 19:00:00.000000 pynchon-2024.3.5.19.3/src/pynchon/app.py
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-03-05 18:58:59.000000 pynchon-2024.3.5.19.3/src/pynchon/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     2606 2024-03-05 19:00:00.000000 pynchon-2024.3.5.19.3/src/pynchon/bin.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 19:03:52.457036 pynchon-2024.3.5.19.3/src/pynchon/cli/
--rw-r--r--   0 runner    (1001) docker     (127)      128 2024-03-05 18:58:59.000000 pynchon-2024.3.5.19.3/src/pynchon/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5029 2024-03-05 19:00:00.000000 pynchon-2024.3.5.19.3/src/pynchon/cli/common.py
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-03-05 18:58:59.000000 pynchon-2024.3.5.19.3/src/pynchon/cli/options.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 19:03:52.457036 pynchon-2024.3.5.19.3/src/pynchon/codemod/
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-03-05 18:58:59.000000 pynchon-2024.3.5.19.3/src/pynchon/codemod/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 19:03:52.461036 pynchon-2024.3.5.19.3/src/pynchon/codemod/commands/
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-03-05 18:58:59.000000 pynchon-2024.3.5.19.3/src/pynchon/codemod/commands/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 19:03:52.461036 pynchon-2024.3.5.19.3/src/pynchon/codemod/commands/docstrings/
--rw-r--r--   0 runner    (1001) docker     (127)      329 2024-03-05 18:58:59.000000 pynchon-2024.3.5.19.3/src/pynchon/codemod/commands/docstrings/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2564 2024-03-05 18:58:59.000000 pynchon-2024.3.5.19.3/src/pynchon/codemod/commands/docstrings/base.py
--rw-r--r--   0 runner    (1001) docker     (127)      557 2024-03-05 18:58:59.000000 pynchon-2024.3.5.19.3/src/pynchon/codemod/commands/docstrings/javadoc.py
--rw-r--r--   0 runner    (1001) docker     (127)     9607 2024-03-05 19:00:00.000000 pynchon-2024.3.5.19.3/src/pynchon/codemod/commands/docstrings/simple.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 19:03:52.461036 pynchon-2024.3.5.19.3/src/pynchon/config/
--rw-r--r--   0 runner    (1001) docker     (127)     1865 2024-03-05 19:00:00.000000 pynchon-2024.3.5.19.3/src/pynchon/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5049 2024-03-05 19:00:00.000000 pynchon-2024.3.5.19.3/src/pynchon/config/util.py
--rw-r--r--   0 runner    (1001) docker     (127)     1470 2024-03-05 18:58:59.000000 pynchon-2024.3.5.19.3/src/pynchon/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     3677 2024-03-05 18:58:59.000000 pynchon-2024.3.5.19.3/src/pynchon/core.py
--rw-r--r--   0 runner    (1001) docker     (127)     2376 2024-03-05 18:58:59.000000 pynchon-2024.3.5.19.3/src/pynchon/events.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 19:03:52.461036 pynchon-2024.3.5.19.3/src/pynchon/models/
--rw-r--r--   0 runner    (1001) docker     (127)      135 2024-03-05 18:58:59.000000 pynchon-2024.3.5.19.3/src/pynchon/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7846 2024-03-05 19:00:00.000000 pynchon-2024.3.5.19.3/src/pynchon/models/planner.py
--rw-r--r--   0 runner    (1001) docker     (127)    12003 2024-03-05 19:00:00.000000 pynchon-2024.3.5.19.3/src/pynchon/models/planning.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 19:03:52.461036 pynchon-2024.3.5.19.3/src/pynchon/models/plugins/
--rw-r--r--   0 runner    (1001) docker     (127)     1378 2024-03-05 18:58:59.000000 pynchon-2024.3.5.19.3/src/pynchon/models/plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10507 2024-03-05 18:58:59.000000 pynchon-2024.3.5.19.3/src/pynchon/models/plugins/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)      606 2024-03-05 19:00:00.000000 pynchon-2024.3.5.19.3/src/pynchon/models/plugins/provider.py
--rw-r--r--   0 runner    (1001) docker     (127)     5752 2024-03-05 19:00:00.000000 pynchon-2024.3.5.19.3/src/pynchon/models/plugins/pynchon.py
--rw-r--r--   0 runner    (1001) docker     (127)      568 2024-03-05 18:58:59.000000 pynchon-2024.3.5.19.3/src/pynchon/models/plugins/tool.py
--rw-r--r--   0 runner    (1001) docker     (127)      959 2024-03-05 18:58:59.000000 pynchon-2024.3.5.19.3/src/pynchon/models/plugins/validators.py
--rw-r--r--   0 runner    (1001) docker     (127)     2851 2024-03-05 18:58:59.000000 pynchon-2024.3.5.19.3/src/pynchon/models/python.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 19:03:52.465036 pynchon-2024.3.5.19.3/src/pynchon/plugins/
--rw-r--r--   0 runner    (1001) docker     (127)     1025 2024-03-05 18:58:59.000000 pynchon-2024.3.5.19.3/src/pynchon/plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      402 2024-03-05 18:58:59.000000 pynchon-2024.3.5.19.3/src/pynchon/plugins/__template__.py
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-03-05 18:58:59.000000 pynchon-2024.3.5.19.3/src/pynchon/plugins/api.py
--rw-r--r--   0 runner    (1001) docker     (127)     1520 2024-03-05 19:00:00.000000 pynchon-2024.3.5.19.3/src/pynchon/plugins/cicd.py
--rw-r--r--   0 runner    (1001) docker     (127)     7905 2024-03-05 19:00:00.000000 pynchon-2024.3.5.19.3/src/pynchon/plugins/core.py
--rw-r--r--   0 runner    (1001) docker     (127)     2035 2024-03-05 18:58:59.000000 pynchon-2024.3.5.19.3/src/pynchon/plugins/deck.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 19:03:52.465036 pynchon-2024.3.5.19.3/src/pynchon/plugins/docs/
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-03-05 18:58:59.000000 pynchon-2024.3.5.19.3/src/pynchon/plugins/docs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5152 2024-03-05 19:00:00.000000 pynchon-2024.3.5.19.3/src/pynchon/plugins/docs/main.py
--rw-r--r--   0 runner    (1001) docker     (127)     1991 2024-03-05 18:58:59.000000 pynchon-2024.3.5.19.3/src/pynchon/plugins/docs/opener.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 19:03:52.465036 pynchon-2024.3.5.19.3/src/pynchon/plugins/doctor/
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-03-05 18:58:59.000000 pynchon-2024.3.5.19.3/src/pynchon/plugins/doctor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2481 2024-03-05 19:00:00.000000 pynchon-2024.3.5.19.3/src/pynchon/plugins/dot.py
--rw-r--r--   0 runner    (1001) docker     (127)     3549 2024-03-05 19:00:00.000000 pynchon-2024.3.5.19.3/src/pynchon/plugins/fixme.py
--rw-r--r--   0 runner    (1001) docker     (127)     2902 2024-03-05 18:58:59.000000 pynchon-2024.3.5.19.3/src/pynchon/plugins/gen.py
--rw-r--r--   0 runner    (1001) docker     (127)     4747 2024-03-05 18:58:59.000000 pynchon-2024.3.5.19.3/src/pynchon/plugins/git.py
--rw-r--r--   0 runner    (1001) docker     (127)     3943 2024-03-05 18:58:59.000000 pynchon-2024.3.5.19.3/src/pynchon/plugins/github.py
--rw-r--r--   0 runner    (1001) docker     (127)      401 2024-03-05 19:00:00.000000 pynchon-2024.3.5.19.3/src/pynchon/plugins/globals.py
--rw-r--r--   0 runner    (1001) docker     (127)     1597 2024-03-05 18:58:59.000000 pynchon-2024.3.5.19.3/src/pynchon/plugins/griffe.py
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-03-05 18:58:59.000000 pynchon-2024.3.5.19.3/src/pynchon/plugins/hooks.py
--rw-r--r--   0 runner    (1001) docker     (127)     5116 2024-03-05 19:00:00.000000 pynchon-2024.3.5.19.3/src/pynchon/plugins/jinja.py
--rw-r--r--   0 runner    (1001) docker     (127)     1507 2024-03-05 18:58:59.000000 pynchon-2024.3.5.19.3/src/pynchon/plugins/json.py
--rw-r--r--   0 runner    (1001) docker     (127)     3954 2024-03-05 19:00:00.000000 pynchon-2024.3.5.19.3/src/pynchon/plugins/makefile.py
--rw-r--r--   0 runner    (1001) docker     (127)     6669 2024-03-05 18:58:59.000000 pynchon-2024.3.5.19.3/src/pynchon/plugins/markdown.py
--rw-r--r--   0 runner    (1001) docker     (127)     2784 2024-03-05 19:00:00.000000 pynchon-2024.3.5.19.3/src/pynchon/plugins/mermaid.py
--rw-r--r--   0 runner    (1001) docker     (127)     7761 2024-03-05 19:00:00.000000 pynchon-2024.3.5.19.3/src/pynchon/plugins/mkdocs.py
--rw-r--r--   0 runner    (1001) docker     (127)     1664 2024-03-05 19:00:00.000000 pynchon-2024.3.5.19.3/src/pynchon/plugins/pandoc.py
--rw-r--r--   0 runner    (1001) docker     (127)      456 2024-03-05 18:58:59.000000 pynchon-2024.3.5.19.3/src/pynchon/plugins/parse.py
--rw-r--r--   0 runner    (1001) docker     (127)    14638 2024-03-05 19:00:00.000000 pynchon-2024.3.5.19.3/src/pynchon/plugins/pattern.py
--rw-r--r--   0 runner    (1001) docker     (127)     1635 2024-03-05 19:00:00.000000 pynchon-2024.3.5.19.3/src/pynchon/plugins/plugins.py
--rw-r--r--   0 runner    (1001) docker     (127)     3914 2024-03-05 19:00:00.000000 pynchon-2024.3.5.19.3/src/pynchon/plugins/project.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 19:03:52.465036 pynchon-2024.3.5.19.3/src/pynchon/plugins/python/
--rw-r--r--   0 runner    (1001) docker     (127)      145 2024-03-05 18:58:59.000000 pynchon-2024.3.5.19.3/src/pynchon/plugins/python/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3371 2024-03-05 18:58:59.000000 pynchon-2024.3.5.19.3/src/pynchon/plugins/python/api.py
--rw-r--r--   0 runner    (1001) docker     (127)    16435 2024-03-05 19:00:00.000000 pynchon-2024.3.5.19.3/src/pynchon/plugins/python/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-05 18:58:59.000000 pynchon-2024.3.5.19.3/src/pynchon/plugins/python/config.py
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-03-05 18:58:59.000000 pynchon-2024.3.5.19.3/src/pynchon/plugins/python/cst.py
--rw-r--r--   0 runner    (1001) docker     (127)     3509 2024-03-05 19:00:00.000000 pynchon-2024.3.5.19.3/src/pynchon/plugins/python/libcst.py
--rw-r--r--   0 runner    (1001) docker     (127)      236 2024-03-05 18:58:59.000000 pynchon-2024.3.5.19.3/src/pynchon/plugins/python/models.py
--rw-r--r--   0 runner    (1001) docker     (127)     3207 2024-03-05 18:58:59.000000 pynchon-2024.3.5.19.3/src/pynchon/plugins/python/platform.py
--rw-r--r--   0 runner    (1001) docker     (127)      720 2024-03-05 18:58:59.000000 pynchon-2024.3.5.19.3/src/pynchon/plugins/python/pypi.py
--rw-r--r--   0 runner    (1001) docker     (127)      700 2024-03-05 18:58:59.000000 pynchon-2024.3.5.19.3/src/pynchon/plugins/release.py
--rw-r--r--   0 runner    (1001) docker     (127)     1153 2024-03-05 19:00:00.000000 pynchon-2024.3.5.19.3/src/pynchon/plugins/render.py
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-03-05 18:58:59.000000 pynchon-2024.3.5.19.3/src/pynchon/plugins/rtd.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 19:03:52.465036 pynchon-2024.3.5.19.3/src/pynchon/plugins/scaffolding/
--rw-r--r--   0 runner    (1001) docker     (127)     3784 2024-03-05 18:58:59.000000 pynchon-2024.3.5.19.3/src/pynchon/plugins/scaffolding/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1158 2024-03-05 18:58:59.000000 pynchon-2024.3.5.19.3/src/pynchon/plugins/scaffolding/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     7559 2024-03-05 18:58:59.000000 pynchon-2024.3.5.19.3/src/pynchon/plugins/src.py
--rw-r--r--   0 runner    (1001) docker     (127)     3893 2024-03-05 19:00:00.000000 pynchon-2024.3.5.19.3/src/pynchon/plugins/tests.py
--rw-r--r--   0 runner    (1001) docker     (127)      402 2024-03-05 18:58:59.000000 pynchon-2024.3.5.19.3/src/pynchon/plugins/tox.py
--rw-r--r--   0 runner    (1001) docker     (127)     1445 2024-03-05 18:58:59.000000 pynchon-2024.3.5.19.3/src/pynchon/plugins/util.py
--rw-r--r--   0 runner    (1001) docker     (127)       86 2024-03-05 18:58:59.000000 pynchon-2024.3.5.19.3/src/pynchon/tagging.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 19:03:52.453036 pynchon-2024.3.5.19.3/src/pynchon/templates/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 19:03:52.469036 pynchon-2024.3.5.19.3/src/pynchon/templates/docker/
--rw-r--r--   0 runner    (1001) docker     (127)      605 2024-03-05 18:58:59.000000 pynchon-2024.3.5.19.3/src/pynchon/templates/docker/Dockerfile.pandoc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 19:03:52.469036 pynchon-2024.3.5.19.3/src/pynchon/templates/docs/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-05 18:58:59.000000 pynchon-2024.3.5.19.3/src/pynchon/templates/docs/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 19:03:52.449036 pynchon-2024.3.5.19.3/src/pynchon/templates/includes/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 19:03:52.449036 pynchon-2024.3.5.19.3/src/pynchon/templates/includes/pynchon/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 19:03:52.469036 pynchon-2024.3.5.19.3/src/pynchon/templates/includes/pynchon/github/
--rw-r--r--   0 runner    (1001) docker     (127)      297 2024-03-05 18:58:59.000000 pynchon-2024.3.5.19.3/src/pynchon/templates/includes/pynchon/github/header.md.j2
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 19:03:52.449036 pynchon-2024.3.5.19.3/src/pynchon/templates/includes/pynchon/plugins/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 19:03:52.469036 pynchon-2024.3.5.19.3/src/pynchon/templates/includes/pynchon/plugins/core/
--rw-r--r--   0 runner    (1001) docker     (127)      401 2024-03-05 18:58:59.000000 pynchon-2024.3.5.19.3/src/pynchon/templates/includes/pynchon/plugins/core/VERSIONS.md.j2
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 19:03:52.469036 pynchon-2024.3.5.19.3/src/pynchon/templates/includes/pynchon/plugins/core/bootstrap/
--rw-r--r--   0 runner    (1001) docker     (127)      118 2024-03-05 18:58:59.000000 pynchon-2024.3.5.19.3/src/pynchon/templates/includes/pynchon/plugins/core/bootstrap/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)     1150 2024-03-05 18:58:59.000000 pynchon-2024.3.5.19.3/src/pynchon/templates/includes/pynchon/plugins/core/bootstrap/bash.sh
--rw-r--r--   0 runner    (1001) docker     (127)      799 2024-03-05 18:58:59.000000 pynchon-2024.3.5.19.3/src/pynchon/templates/includes/pynchon/plugins/core/bootstrap/bashrc.sh
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-03-05 18:58:59.000000 pynchon-2024.3.5.19.3/src/pynchon/templates/includes/pynchon/plugins/core/bootstrap/makefile.j2
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-03-05 18:58:59.000000 pynchon-2024.3.5.19.3/src/pynchon/templates/includes/pynchon/plugins/core/bootstrap/python.j2
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-03-05 18:58:59.000000 pynchon-2024.3.5.19.3/src/pynchon/templates/includes/pynchon/plugins/core/bootstrap/sh.j2
--rw-r--r--   0 runner    (1001) docker     (127)      912 2024-03-05 18:58:59.000000 pynchon-2024.3.5.19.3/src/pynchon/templates/includes/pynchon/plugins/core/bootstrap/tox.ini
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 19:03:52.469036 pynchon-2024.3.5.19.3/src/pynchon/templates/includes/pynchon/plugins/fixme/
--rw-r--r--   0 runner    (1001) docker     (127)      164 2024-03-05 18:58:59.000000 pynchon-2024.3.5.19.3/src/pynchon/templates/includes/pynchon/plugins/fixme/FIXME.md.j2
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 19:03:52.469036 pynchon-2024.3.5.19.3/src/pynchon/templates/includes/pynchon/plugins/makefile/
--rw-r--r--   0 runner    (1001) docker     (127)     1202 2024-03-05 18:58:59.000000 pynchon-2024.3.5.19.3/src/pynchon/templates/includes/pynchon/plugins/makefile/mermaid-graph.mmd.j2
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 19:03:52.449036 pynchon-2024.3.5.19.3/src/pynchon/templates/includes/pynchon/plugins/python/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 19:03:52.469036 pynchon-2024.3.5.19.3/src/pynchon/templates/includes/pynchon/plugins/python/api/
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-03-05 18:58:59.000000 pynchon-2024.3.5.19.3/src/pynchon/templates/includes/pynchon/plugins/python/api/TOC.md.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1209 2024-03-05 18:58:59.000000 pynchon-2024.3.5.19.3/src/pynchon/templates/includes/pynchon/plugins/python/api/classes.md.j2
--rw-r--r--   0 runner    (1001) docker     (127)      949 2024-03-05 18:58:59.000000 pynchon-2024.3.5.19.3/src/pynchon/templates/includes/pynchon/plugins/python/api/functions.md.j2
--rw-r--r--   0 runner    (1001) docker     (127)      324 2024-03-05 18:58:59.000000 pynchon-2024.3.5.19.3/src/pynchon/templates/includes/pynchon/plugins/python/api/modules.md.j2
--rw-r--r--   0 runner    (1001) docker     (127)      757 2024-03-05 18:58:59.000000 pynchon-2024.3.5.19.3/src/pynchon/templates/includes/pynchon/plugins/python/api/package.md.j2
--rw-r--r--   0 runner    (1001) docker     (127)     2987 2024-03-05 18:58:59.000000 pynchon-2024.3.5.19.3/src/pynchon/templates/includes/pynchon/plugins/python/api/toc2.md.j2
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 19:03:52.449036 pynchon-2024.3.5.19.3/src/pynchon/templates/includes/pynchon/plugins/python/gen/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 19:03:52.469036 pynchon-2024.3.5.19.3/src/pynchon/templates/includes/pynchon/plugins/python/gen/docstrings/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-05 18:58:59.000000 pynchon-2024.3.5.19.3/src/pynchon/templates/includes/pynchon/plugins/python/gen/docstrings/function.txt.j2
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-05 18:58:59.000000 pynchon-2024.3.5.19.3/src/pynchon/templates/includes/pynchon/plugins/python/gen/docstrings/module.txt.j2
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 19:03:52.469036 pynchon-2024.3.5.19.3/src/pynchon/templates/includes/pynchon/plugins/python_cli/
--rw-r--r--   0 runner    (1001) docker     (127)     1446 2024-03-05 18:58:59.000000 pynchon-2024.3.5.19.3/src/pynchon/templates/includes/pynchon/plugins/python_cli/TOC.md.j2
--rw-r--r--   0 runner    (1001) docker     (127)      200 2024-03-05 18:58:59.000000 pynchon-2024.3.5.19.3/src/pynchon/templates/includes/pynchon/plugins/python_cli/detail.md.j2
--rw-r--r--   0 runner    (1001) docker     (127)      696 2024-03-05 18:58:59.000000 pynchon-2024.3.5.19.3/src/pynchon/templates/includes/pynchon/plugins/python_cli/main.module.md.j2
--rw-r--r--   0 runner    (1001) docker     (127)      910 2024-03-05 18:58:59.000000 pynchon-2024.3.5.19.3/src/pynchon/templates/includes/pynchon/plugins/python_cli/script.console.md.j2
--rw-r--r--   0 runner    (1001) docker     (127)      284 2024-03-05 18:58:59.000000 pynchon-2024.3.5.19.3/src/pynchon/templates/includes/pynchon/plugins/python_cli/subcommand.md.j2
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 19:03:52.453036 pynchon-2024.3.5.19.3/src/pynchon/templates/includes/pynchon/plugins/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 19:03:52.469036 pynchon-2024.3.5.19.3/src/pynchon/templates/includes/pynchon/plugins/src/header/
--rw-r--r--   0 runner    (1001) docker     (127)      134 2024-03-05 18:58:59.000000 pynchon-2024.3.5.19.3/src/pynchon/templates/includes/pynchon/plugins/src/header/jinja-md.md.j2
--rw-r--r--   0 runner    (1001) docker     (127)      134 2024-03-05 18:58:59.000000 pynchon-2024.3.5.19.3/src/pynchon/templates/includes/pynchon/plugins/src/header/jinja.j2
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-03-05 18:58:59.000000 pynchon-2024.3.5.19.3/src/pynchon/templates/includes/pynchon/plugins/src/header/python.j2
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 19:03:52.469036 pynchon-2024.3.5.19.3/src/pynchon/templates/scaffolds/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-05 18:58:59.000000 pynchon-2024.3.5.19.3/src/pynchon/templates/scaffolds/.gitkeep
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 19:03:52.453036 pynchon-2024.3.5.19.3/src/pynchon/templates/scaffolds/ansible/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 19:03:52.469036 pynchon-2024.3.5.19.3/src/pynchon/templates/scaffolds/ansible/role/
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-03-05 18:58:59.000000 pynchon-2024.3.5.19.3/src/pynchon/templates/scaffolds/ansible/role/.ansible-lint
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 19:03:52.453036 pynchon-2024.3.5.19.3/src/pynchon/templates/scaffolds/ansible/role/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 19:03:52.473036 pynchon-2024.3.5.19.3/src/pynchon/templates/scaffolds/ansible/role/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-05 18:58:59.000000 pynchon-2024.3.5.19.3/src/pynchon/templates/scaffolds/ansible/role/.github/workflows/ansible-lint.yml
--rw-r--r--   0 runner    (1001) docker     (127)      505 2024-03-05 18:58:59.000000 pynchon-2024.3.5.19.3/src/pynchon/templates/scaffolds/ansible/role/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 19:03:52.473036 pynchon-2024.3.5.19.3/src/pynchon/templates/scaffolds/docker/
--rw-r--r--   0 runner    (1001) docker     (127)     1079 2024-03-05 18:58:59.000000 pynchon-2024.3.5.19.3/src/pynchon/templates/scaffolds/docker/.dockerignore
--rw-r--r--   0 runner    (1001) docker     (127)       90 2024-03-05 18:58:59.000000 pynchon-2024.3.5.19.3/src/pynchon/templates/scaffolds/docker/.scaffold.advice.json5
--rw-r--r--   0 runner    (1001) docker     (127)      162 2024-03-05 18:58:59.000000 pynchon-2024.3.5.19.3/src/pynchon/templates/scaffolds/docker/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (127)     1374 2024-03-05 18:58:59.000000 pynchon-2024.3.5.19.3/src/pynchon/templates/scaffolds/docker/README.md.j2
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 19:03:52.453036 pynchon-2024.3.5.19.3/src/pynchon/templates/scaffolds/docs/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 19:03:52.473036 pynchon-2024.3.5.19.3/src/pynchon/templates/scaffolds/docs/includes/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-05 18:58:59.000000 pynchon-2024.3.5.19.3/src/pynchon/templates/scaffolds/docs/includes/.gitkeep
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 19:03:52.473036 pynchon-2024.3.5.19.3/src/pynchon/templates/scaffolds/github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 19:03:52.453036 pynchon-2024.3.5.19.3/src/pynchon/templates/scaffolds/github/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 19:03:52.473036 pynchon-2024.3.5.19.3/src/pynchon/templates/scaffolds/github/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-05 18:58:59.000000 pynchon-2024.3.5.19.3/src/pynchon/templates/scaffolds/github/.github/workflows/.gitkeep
--rw-r--r--   0 runner    (1001) docker     (127)      153 2024-03-05 18:58:59.000000 pynchon-2024.3.5.19.3/src/pynchon/templates/scaffolds/github/.github/workflows/hello-world.yml
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-03-05 18:58:59.000000 pynchon-2024.3.5.19.3/src/pynchon/templates/scaffolds/github/.scaffold.advice.json5
--rw-r--r--   0 runner    (1001) docker     (127)      458 2024-03-05 18:58:59.000000 pynchon-2024.3.5.19.3/src/pynchon/templates/scaffolds/github/README.md.j2
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 19:03:52.453036 pynchon-2024.3.5.19.3/src/pynchon/templates/scaffolds/py/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 19:03:52.473036 pynchon-2024.3.5.19.3/src/pynchon/templates/scaffolds/py/pkg/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-05 18:58:59.000000 pynchon-2024.3.5.19.3/src/pynchon/templates/scaffolds/py/pkg/.ackrc
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-05 18:58:59.000000 pynchon-2024.3.5.19.3/src/pynchon/templates/scaffolds/py/pkg/.flake8
--rw-r--r--   0 runner    (1001) docker     (127)      776 2024-03-05 18:58:59.000000 pynchon-2024.3.5.19.3/src/pynchon/templates/scaffolds/py/pkg/.libcst.codemod.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       64 2024-03-05 18:58:59.000000 pynchon-2024.3.5.19.3/src/pynchon/templates/scaffolds/py/pkg/.scaffold.advice.json5
--rw-r--r--   0 runner    (1001) docker     (127)     1928 2024-03-05 18:58:59.000000 pynchon-2024.3.5.19.3/src/pynchon/templates/scaffolds/py/pkg/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)     2033 2024-03-05 18:58:59.000000 pynchon-2024.3.5.19.3/src/pynchon/templates/scaffolds/py/pkg/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1549 2024-03-05 18:58:59.000000 pynchon-2024.3.5.19.3/src/pynchon/templates/scaffolds/py/pkg/README.md.j2
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 19:03:52.473036 pynchon-2024.3.5.19.3/src/pynchon/templates/scaffolds/py/pkg/docs/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-05 18:58:59.000000 pynchon-2024.3.5.19.3/src/pynchon/templates/scaffolds/py/pkg/docs/.gitkeep
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 19:03:52.473036 pynchon-2024.3.5.19.3/src/pynchon/templates/scaffolds/py/pkg/docs/html/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-05 18:58:59.000000 pynchon-2024.3.5.19.3/src/pynchon/templates/scaffolds/py/pkg/docs/html/.gitkeep
--rw-r--r--   0 runner    (1001) docker     (127)     2396 2024-03-05 18:58:59.000000 pynchon-2024.3.5.19.3/src/pynchon/templates/scaffolds/py/pkg/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      771 2024-03-05 18:58:59.000000 pynchon-2024.3.5.19.3/src/pynchon/templates/scaffolds/py/pkg/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 19:03:52.453036 pynchon-2024.3.5.19.3/src/pynchon/templates/scaffolds/py/pkg/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 19:03:52.473036 pynchon-2024.3.5.19.3/src/pynchon/templates/scaffolds/py/pkg/src/{{name}}/
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-03-05 18:58:59.000000 pynchon-2024.3.5.19.3/src/pynchon/templates/scaffolds/py/pkg/src/{{name}}/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-03-05 18:58:59.000000 pynchon-2024.3.5.19.3/src/pynchon/templates/scaffolds/py/pkg/src/{{name}}/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-03-05 18:58:59.000000 pynchon-2024.3.5.19.3/src/pynchon/templates/scaffolds/py/pkg/src/{{name}}/app.py
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-03-05 18:58:59.000000 pynchon-2024.3.5.19.3/src/pynchon/templates/scaffolds/py/pkg/src/{{name}}/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-03-05 18:58:59.000000 pynchon-2024.3.5.19.3/src/pynchon/templates/scaffolds/py/pkg/src/{{name}}/lme.py
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-03-05 18:58:59.000000 pynchon-2024.3.5.19.3/src/pynchon/templates/scaffolds/py/pkg/src/{{name}}/models.py
--rw-r--r--   0 runner    (1001) docker     (127)       87 2024-03-05 18:58:59.000000 pynchon-2024.3.5.19.3/src/pynchon/templates/scaffolds/py/pkg/src/{{name}}/tagging.py
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-03-05 18:58:59.000000 pynchon-2024.3.5.19.3/src/pynchon/templates/scaffolds/py/pkg/src/{{name}}/typing.py
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-03-05 18:58:59.000000 pynchon-2024.3.5.19.3/src/pynchon/templates/scaffolds/py/pkg/src/{{name}}/util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 19:03:52.473036 pynchon-2024.3.5.19.3/src/pynchon/templates/scaffolds/py/pkg/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-05 18:58:59.000000 pynchon-2024.3.5.19.3/src/pynchon/templates/scaffolds/py/pkg/tests/.gitkeep
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-05 18:58:59.000000 pynchon-2024.3.5.19.3/src/pynchon/templates/scaffolds/py/pkg/tests/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 19:03:52.477036 pynchon-2024.3.5.19.3/src/pynchon/templates/scaffolds/py/pkg/tests/integration/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-05 18:58:59.000000 pynchon-2024.3.5.19.3/src/pynchon/templates/scaffolds/py/pkg/tests/integration/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-03-05 18:58:59.000000 pynchon-2024.3.5.19.3/src/pynchon/templates/scaffolds/py/pkg/tests/integration/test_all.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 19:03:52.477036 pynchon-2024.3.5.19.3/src/pynchon/templates/scaffolds/py/pkg/tests/smoke/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-05 18:58:59.000000 pynchon-2024.3.5.19.3/src/pynchon/templates/scaffolds/py/pkg/tests/smoke/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-03-05 18:58:59.000000 pynchon-2024.3.5.19.3/src/pynchon/templates/scaffolds/py/pkg/tests/smoke/test_all.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 19:03:52.477036 pynchon-2024.3.5.19.3/src/pynchon/templates/scaffolds/py/pkg/tests/units/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-05 18:58:59.000000 pynchon-2024.3.5.19.3/src/pynchon/templates/scaffolds/py/pkg/tests/units/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-03-05 18:58:59.000000 pynchon-2024.3.5.19.3/src/pynchon/templates/scaffolds/py/pkg/tests/units/test_all.py
--rw-r--r--   0 runner    (1001) docker     (127)     3097 2024-03-05 18:58:59.000000 pynchon-2024.3.5.19.3/src/pynchon/templates/scaffolds/py/pkg/tox.ini
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 19:03:52.477036 pynchon-2024.3.5.19.3/src/pynchon/templates/scaffolds/py/workspace/
--rw-r--r--   0 runner    (1001) docker     (127)       64 2024-03-05 18:58:59.000000 pynchon-2024.3.5.19.3/src/pynchon/templates/scaffolds/py/workspace/.scaffold.advice.json5
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 19:03:52.453036 pynchon-2024.3.5.19.3/src/pynchon/templates/scaffolds/software/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 19:03:52.477036 pynchon-2024.3.5.19.3/src/pynchon/templates/scaffolds/software/automation/
--rw-r--r--   0 runner    (1001) docker     (127)      348 2024-03-05 18:58:59.000000 pynchon-2024.3.5.19.3/src/pynchon/templates/scaffolds/software/automation/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 19:03:52.477036 pynchon-2024.3.5.19.3/src/pynchon/templates/scaffolds/software/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      348 2024-03-05 18:58:59.000000 pynchon-2024.3.5.19.3/src/pynchon/templates/scaffolds/software/tests/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 19:03:52.453036 pynchon-2024.3.5.19.3/src/pynchon/templates/scaffolds/software/tests/tests/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 19:03:52.477036 pynchon-2024.3.5.19.3/src/pynchon/templates/scaffolds/software/tests/tests/integration/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-05 18:58:59.000000 pynchon-2024.3.5.19.3/src/pynchon/templates/scaffolds/software/tests/tests/integration/.gitkeep
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 19:03:52.477036 pynchon-2024.3.5.19.3/src/pynchon/templates/scaffolds/software/tests/tests/smoke/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-05 18:58:59.000000 pynchon-2024.3.5.19.3/src/pynchon/templates/scaffolds/software/tests/tests/smoke/.gitkeep
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 19:03:52.477036 pynchon-2024.3.5.19.3/src/pynchon/templates/scaffolds/software/tests/tests/units/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-05 18:58:59.000000 pynchon-2024.3.5.19.3/src/pynchon/templates/scaffolds/software/tests/tests/units/.gitkeep
--rw-r--r--   0 runner    (1001) docker     (127)      284 2024-03-05 18:58:59.000000 pynchon-2024.3.5.19.3/src/pynchon/testing.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 19:03:52.477036 pynchon-2024.3.5.19.3/src/pynchon/util/
--rw-r--r--   0 runner    (1001) docker     (127)     1055 2024-03-05 18:58:59.000000 pynchon-2024.3.5.19.3/src/pynchon/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-03-05 18:58:59.000000 pynchon-2024.3.5.19.3/src/pynchon/util/click.py
--rw-r--r--   0 runner    (1001) docker     (127)     5654 2024-03-05 19:00:00.000000 pynchon-2024.3.5.19.3/src/pynchon/util/complexity.py
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-03-05 18:58:59.000000 pynchon-2024.3.5.19.3/src/pynchon/util/config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 19:03:52.477036 pynchon-2024.3.5.19.3/src/pynchon/util/console/
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-05 18:58:59.000000 pynchon-2024.3.5.19.3/src/pynchon/util/console/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-05 18:58:59.000000 pynchon-2024.3.5.19.3/src/pynchon/util/console/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4662 2024-03-05 18:58:59.000000 pynchon-2024.3.5.19.3/src/pynchon/util/docker.py
--rw-r--r--   0 runner    (1001) docker     (127)      711 2024-03-05 19:00:00.000000 pynchon-2024.3.5.19.3/src/pynchon/util/events.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 19:03:52.477036 pynchon-2024.3.5.19.3/src/pynchon/util/files/
--rw-r--r--   0 runner    (1001) docker     (127)     3902 2024-03-05 19:00:00.000000 pynchon-2024.3.5.19.3/src/pynchon/util/files/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      948 2024-03-05 19:00:00.000000 pynchon-2024.3.5.19.3/src/pynchon/util/files/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2089 2024-03-05 19:00:00.000000 pynchon-2024.3.5.19.3/src/pynchon/util/files/diff.py
--rw-r--r--   0 runner    (1001) docker     (127)     2608 2024-03-05 19:00:00.000000 pynchon-2024.3.5.19.3/src/pynchon/util/lme.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 19:03:52.477036 pynchon-2024.3.5.19.3/src/pynchon/util/makefile/
--rw-r--r--   0 runner    (1001) docker     (127)     5276 2024-03-05 19:00:00.000000 pynchon-2024.3.5.19.3/src/pynchon/util/makefile/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      484 2024-03-05 19:00:00.000000 pynchon-2024.3.5.19.3/src/pynchon/util/makefile/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1139 2024-03-05 18:58:59.000000 pynchon-2024.3.5.19.3/src/pynchon/util/oop.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 19:03:52.481036 pynchon-2024.3.5.19.3/src/pynchon/util/os/
--rw-r--r--   0 runner    (1001) docker     (127)      578 2024-03-05 18:58:59.000000 pynchon-2024.3.5.19.3/src/pynchon/util/os/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5760 2024-03-05 18:58:59.000000 pynchon-2024.3.5.19.3/src/pynchon/util/os/models.py
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-03-05 18:58:59.000000 pynchon-2024.3.5.19.3/src/pynchon/util/os/pidfile.py
--rw-r--r--   0 runner    (1001) docker     (127)     1081 2024-03-05 18:58:59.000000 pynchon-2024.3.5.19.3/src/pynchon/util/os/pids.py
--rw-r--r--   0 runner    (1001) docker     (127)     2054 2024-03-05 18:58:59.000000 pynchon-2024.3.5.19.3/src/pynchon/util/python.py
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-03-05 18:58:59.000000 pynchon-2024.3.5.19.3/src/pynchon/util/splitvt.py
--rw-r--r--   0 runner    (1001) docker     (127)      463 2024-03-05 18:58:59.000000 pynchon-2024.3.5.19.3/src/pynchon/util/testing.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 19:03:52.481036 pynchon-2024.3.5.19.3/src/pynchon/util/text/
--rw-r--r--   0 runner    (1001) docker     (127)      551 2024-03-05 18:58:59.000000 pynchon-2024.3.5.19.3/src/pynchon/util/text/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      367 2024-03-05 19:00:00.000000 pynchon-2024.3.5.19.3/src/pynchon/util/text/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 19:03:52.481036 pynchon-2024.3.5.19.3/src/pynchon/util/text/dumpf/
--rw-r--r--   0 runner    (1001) docker     (127)      790 2024-03-05 19:00:00.000000 pynchon-2024.3.5.19.3/src/pynchon/util/text/dumpf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1047 2024-03-05 19:00:00.000000 pynchon-2024.3.5.19.3/src/pynchon/util/text/dumpf/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)      598 2024-03-05 18:58:59.000000 pynchon-2024.3.5.19.3/src/pynchon/util/text/dumps.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 19:03:52.481036 pynchon-2024.3.5.19.3/src/pynchon/util/text/loadf/
--rw-r--r--   0 runner    (1001) docker     (127)     7414 2024-03-05 19:00:00.000000 pynchon-2024.3.5.19.3/src/pynchon/util/text/loadf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1042 2024-03-05 19:00:00.000000 pynchon-2024.3.5.19.3/src/pynchon/util/text/loadf/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1950 2024-03-05 19:00:00.000000 pynchon-2024.3.5.19.3/src/pynchon/util/text/loads.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 19:03:52.481036 pynchon-2024.3.5.19.3/src/pynchon/util/text/normalize/
--rw-r--r--   0 runner    (1001) docker     (127)     1285 2024-03-05 18:58:59.000000 pynchon-2024.3.5.19.3/src/pynchon/util/text/normalize/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 19:03:52.481036 pynchon-2024.3.5.19.3/src/pynchon/util/text/render/
--rw-r--r--   0 runner    (1001) docker     (127)     6431 2024-03-05 19:00:00.000000 pynchon-2024.3.5.19.3/src/pynchon/util/text/render/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      972 2024-03-05 19:00:00.000000 pynchon-2024.3.5.19.3/src/pynchon/util/text/render/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1395 2024-03-05 18:58:59.000000 pynchon-2024.3.5.19.3/src/pynchon/util/typing.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 19:03:52.481036 pynchon-2024.3.5.19.3/src/pynchon.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1736 2024-03-05 19:03:52.000000 pynchon-2024.3.5.19.3/src/pynchon.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     9102 2024-03-05 19:03:52.000000 pynchon-2024.3.5.19.3/src/pynchon.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-05 19:03:52.000000 pynchon-2024.3.5.19.3/src/pynchon.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-03-05 19:03:52.000000 pynchon-2024.3.5.19.3/src/pynchon.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-05 19:03:52.000000 pynchon-2024.3.5.19.3/src/pynchon.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      425 2024-03-05 19:03:52.000000 pynchon-2024.3.5.19.3/src/pynchon.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-03-05 19:03:52.000000 pynchon-2024.3.5.19.3/src/pynchon.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:11:27.716485 pynchon-2024.4.3.17.11/
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-04-03 17:06:30.000000 pynchon-2024.4.3.17.11/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1714 2024-04-03 17:11:27.716485 pynchon-2024.4.3.17.11/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2144 2024-04-03 17:06:30.000000 pynchon-2024.4.3.17.11/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      979 2024-04-03 17:06:30.000000 pynchon-2024.4.3.17.11/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1728 2024-04-03 17:11:27.716485 pynchon-2024.4.3.17.11/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      770 2024-04-03 17:06:30.000000 pynchon-2024.4.3.17.11/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:11:27.664485 pynchon-2024.4.3.17.11/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:11:27.676485 pynchon-2024.4.3.17.11/src/pynchon/
+-rw-r--r--   0 runner    (1001) docker     (127)      259 2024-04-03 17:06:30.000000 pynchon-2024.4.3.17.11/src/pynchon/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-04-03 17:06:30.000000 pynchon-2024.4.3.17.11/src/pynchon/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-04-03 17:11:25.000000 pynchon-2024.4.3.17.11/src/pynchon/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:11:27.680485 pynchon-2024.4.3.17.11/src/pynchon/abcs/
+-rw-r--r--   0 runner    (1001) docker     (127)      319 2024-04-03 17:06:30.000000 pynchon-2024.4.3.17.11/src/pynchon/abcs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1503 2024-04-03 17:06:30.000000 pynchon-2024.4.3.17.11/src/pynchon/abcs/attrdict.py
+-rw-r--r--   0 runner    (1001) docker     (127)      115 2024-04-03 17:06:30.000000 pynchon-2024.4.3.17.11/src/pynchon/abcs/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2011 2024-04-03 17:06:30.000000 pynchon-2024.4.3.17.11/src/pynchon/abcs/path.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5484 2024-04-03 17:06:30.000000 pynchon-2024.4.3.17.11/src/pynchon/abcs/visitor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5088 2024-04-03 17:07:37.000000 pynchon-2024.4.3.17.11/src/pynchon/annotate.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:11:27.680485 pynchon-2024.4.3.17.11/src/pynchon/api/
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-04-03 17:06:30.000000 pynchon-2024.4.3.17.11/src/pynchon/api/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:11:27.680485 pynchon-2024.4.3.17.11/src/pynchon/api/git/
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-03 17:06:30.000000 pynchon-2024.4.3.17.11/src/pynchon/api/git/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:11:27.680485 pynchon-2024.4.3.17.11/src/pynchon/api/parsers/
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-04-03 17:06:30.000000 pynchon-2024.4.3.17.11/src/pynchon/api/parsers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:11:27.680485 pynchon-2024.4.3.17.11/src/pynchon/api/project/
+-rw-r--r--   0 runner    (1001) docker     (127)     1203 2024-04-03 17:06:30.000000 pynchon-2024.4.3.17.11/src/pynchon/api/project/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-03 17:06:30.000000 pynchon-2024.4.3.17.11/src/pynchon/api/pynchon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7246 2024-04-03 17:07:37.000000 pynchon-2024.4.3.17.11/src/pynchon/api/render.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5262 2024-04-03 17:07:37.000000 pynchon-2024.4.3.17.11/src/pynchon/app.py
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-03 17:06:30.000000 pynchon-2024.4.3.17.11/src/pynchon/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2606 2024-04-03 17:07:37.000000 pynchon-2024.4.3.17.11/src/pynchon/bin.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:11:27.680485 pynchon-2024.4.3.17.11/src/pynchon/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)      128 2024-04-03 17:06:30.000000 pynchon-2024.4.3.17.11/src/pynchon/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5029 2024-04-03 17:07:37.000000 pynchon-2024.4.3.17.11/src/pynchon/cli/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)      357 2024-04-03 17:06:30.000000 pynchon-2024.4.3.17.11/src/pynchon/cli/options.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:11:27.680485 pynchon-2024.4.3.17.11/src/pynchon/codemod/
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-03 17:06:30.000000 pynchon-2024.4.3.17.11/src/pynchon/codemod/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:11:27.680485 pynchon-2024.4.3.17.11/src/pynchon/codemod/commands/
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-03 17:06:30.000000 pynchon-2024.4.3.17.11/src/pynchon/codemod/commands/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:11:27.684485 pynchon-2024.4.3.17.11/src/pynchon/codemod/commands/docstrings/
+-rw-r--r--   0 runner    (1001) docker     (127)      329 2024-04-03 17:06:30.000000 pynchon-2024.4.3.17.11/src/pynchon/codemod/commands/docstrings/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2564 2024-04-03 17:06:30.000000 pynchon-2024.4.3.17.11/src/pynchon/codemod/commands/docstrings/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      557 2024-04-03 17:06:30.000000 pynchon-2024.4.3.17.11/src/pynchon/codemod/commands/docstrings/javadoc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9607 2024-04-03 17:07:37.000000 pynchon-2024.4.3.17.11/src/pynchon/codemod/commands/docstrings/simple.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:11:27.684485 pynchon-2024.4.3.17.11/src/pynchon/config/
+-rw-r--r--   0 runner    (1001) docker     (127)     1865 2024-04-03 17:07:37.000000 pynchon-2024.4.3.17.11/src/pynchon/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5049 2024-04-03 17:07:37.000000 pynchon-2024.4.3.17.11/src/pynchon/config/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1470 2024-04-03 17:06:30.000000 pynchon-2024.4.3.17.11/src/pynchon/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3677 2024-04-03 17:06:30.000000 pynchon-2024.4.3.17.11/src/pynchon/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2376 2024-04-03 17:06:30.000000 pynchon-2024.4.3.17.11/src/pynchon/events.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:11:27.684485 pynchon-2024.4.3.17.11/src/pynchon/models/
+-rw-r--r--   0 runner    (1001) docker     (127)      135 2024-04-03 17:06:30.000000 pynchon-2024.4.3.17.11/src/pynchon/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9072 2024-04-03 17:07:37.000000 pynchon-2024.4.3.17.11/src/pynchon/models/planner.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12987 2024-04-03 17:07:37.000000 pynchon-2024.4.3.17.11/src/pynchon/models/planning.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:11:27.684485 pynchon-2024.4.3.17.11/src/pynchon/models/plugins/
+-rw-r--r--   0 runner    (1001) docker     (127)     1420 2024-04-03 17:06:30.000000 pynchon-2024.4.3.17.11/src/pynchon/models/plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10507 2024-04-03 17:06:30.000000 pynchon-2024.4.3.17.11/src/pynchon/models/plugins/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2690 2024-04-03 17:07:37.000000 pynchon-2024.4.3.17.11/src/pynchon/models/plugins/docker.py
+-rw-r--r--   0 runner    (1001) docker     (127)      606 2024-04-03 17:07:37.000000 pynchon-2024.4.3.17.11/src/pynchon/models/plugins/provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5752 2024-04-03 17:07:37.000000 pynchon-2024.4.3.17.11/src/pynchon/models/plugins/pynchon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      568 2024-04-03 17:06:30.000000 pynchon-2024.4.3.17.11/src/pynchon/models/plugins/tool.py
+-rw-r--r--   0 runner    (1001) docker     (127)      959 2024-04-03 17:06:30.000000 pynchon-2024.4.3.17.11/src/pynchon/models/plugins/validators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3027 2024-04-03 17:06:30.000000 pynchon-2024.4.3.17.11/src/pynchon/models/python.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:11:27.692485 pynchon-2024.4.3.17.11/src/pynchon/plugins/
+-rw-r--r--   0 runner    (1001) docker     (127)     1025 2024-04-03 17:06:30.000000 pynchon-2024.4.3.17.11/src/pynchon/plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      402 2024-04-03 17:06:30.000000 pynchon-2024.4.3.17.11/src/pynchon/plugins/__template__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-03 17:06:30.000000 pynchon-2024.4.3.17.11/src/pynchon/plugins/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1520 2024-04-03 17:07:37.000000 pynchon-2024.4.3.17.11/src/pynchon/plugins/cicd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8821 2024-04-03 17:07:37.000000 pynchon-2024.4.3.17.11/src/pynchon/plugins/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2035 2024-04-03 17:06:30.000000 pynchon-2024.4.3.17.11/src/pynchon/plugins/deck.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1036 2024-04-03 17:06:30.000000 pynchon-2024.4.3.17.11/src/pynchon/plugins/dockerhub.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:11:27.692485 pynchon-2024.4.3.17.11/src/pynchon/plugins/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-03 17:06:30.000000 pynchon-2024.4.3.17.11/src/pynchon/plugins/docs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5152 2024-04-03 17:07:37.000000 pynchon-2024.4.3.17.11/src/pynchon/plugins/docs/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2072 2024-04-03 17:06:30.000000 pynchon-2024.4.3.17.11/src/pynchon/plugins/docs/opener.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:11:27.692485 pynchon-2024.4.3.17.11/src/pynchon/plugins/doctor/
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-04-03 17:06:30.000000 pynchon-2024.4.3.17.11/src/pynchon/plugins/doctor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2489 2024-04-03 17:07:37.000000 pynchon-2024.4.3.17.11/src/pynchon/plugins/dot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3301 2024-04-03 17:06:30.000000 pynchon-2024.4.3.17.11/src/pynchon/plugins/drawio.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3549 2024-04-03 17:07:37.000000 pynchon-2024.4.3.17.11/src/pynchon/plugins/fixme.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2902 2024-04-03 17:06:30.000000 pynchon-2024.4.3.17.11/src/pynchon/plugins/gen.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4747 2024-04-03 17:06:30.000000 pynchon-2024.4.3.17.11/src/pynchon/plugins/git.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4277 2024-04-03 17:06:30.000000 pynchon-2024.4.3.17.11/src/pynchon/plugins/github.py
+-rw-r--r--   0 runner    (1001) docker     (127)      401 2024-04-03 17:07:37.000000 pynchon-2024.4.3.17.11/src/pynchon/plugins/globals.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1597 2024-04-03 17:06:30.000000 pynchon-2024.4.3.17.11/src/pynchon/plugins/griffe.py
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-03 17:06:30.000000 pynchon-2024.4.3.17.11/src/pynchon/plugins/hooks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4232 2024-04-03 17:07:37.000000 pynchon-2024.4.3.17.11/src/pynchon/plugins/jinja.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1507 2024-04-03 17:06:30.000000 pynchon-2024.4.3.17.11/src/pynchon/plugins/json.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3954 2024-04-03 17:07:37.000000 pynchon-2024.4.3.17.11/src/pynchon/plugins/makefile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6750 2024-04-03 17:06:30.000000 pynchon-2024.4.3.17.11/src/pynchon/plugins/markdown.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2745 2024-04-03 17:06:30.000000 pynchon-2024.4.3.17.11/src/pynchon/plugins/mermaid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8009 2024-04-03 17:07:37.000000 pynchon-2024.4.3.17.11/src/pynchon/plugins/mkdocs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3218 2024-04-03 17:07:37.000000 pynchon-2024.4.3.17.11/src/pynchon/plugins/pandoc.py
+-rw-r--r--   0 runner    (1001) docker     (127)      456 2024-04-03 17:06:30.000000 pynchon-2024.4.3.17.11/src/pynchon/plugins/parse.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14638 2024-04-03 17:07:37.000000 pynchon-2024.4.3.17.11/src/pynchon/plugins/pattern.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1636 2024-04-03 17:07:37.000000 pynchon-2024.4.3.17.11/src/pynchon/plugins/plugins.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4044 2024-04-03 17:07:37.000000 pynchon-2024.4.3.17.11/src/pynchon/plugins/project.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:11:27.692485 pynchon-2024.4.3.17.11/src/pynchon/plugins/python/
+-rw-r--r--   0 runner    (1001) docker     (127)      145 2024-04-03 17:06:30.000000 pynchon-2024.4.3.17.11/src/pynchon/plugins/python/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3374 2024-04-03 17:06:30.000000 pynchon-2024.4.3.17.11/src/pynchon/plugins/python/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17560 2024-04-03 17:07:37.000000 pynchon-2024.4.3.17.11/src/pynchon/plugins/python/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-03 17:06:30.000000 pynchon-2024.4.3.17.11/src/pynchon/plugins/python/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-04-03 17:06:30.000000 pynchon-2024.4.3.17.11/src/pynchon/plugins/python/cst.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3509 2024-04-03 17:07:37.000000 pynchon-2024.4.3.17.11/src/pynchon/plugins/python/libcst.py
+-rw-r--r--   0 runner    (1001) docker     (127)      236 2024-04-03 17:06:30.000000 pynchon-2024.4.3.17.11/src/pynchon/plugins/python/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3207 2024-04-03 17:06:30.000000 pynchon-2024.4.3.17.11/src/pynchon/plugins/python/platform.py
+-rw-r--r--   0 runner    (1001) docker     (127)      720 2024-04-03 17:06:30.000000 pynchon-2024.4.3.17.11/src/pynchon/plugins/python/pypi.py
+-rw-r--r--   0 runner    (1001) docker     (127)      700 2024-04-03 17:06:30.000000 pynchon-2024.4.3.17.11/src/pynchon/plugins/release.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1153 2024-04-03 17:07:37.000000 pynchon-2024.4.3.17.11/src/pynchon/plugins/render.py
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-04-03 17:06:30.000000 pynchon-2024.4.3.17.11/src/pynchon/plugins/rtd.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:11:27.692485 pynchon-2024.4.3.17.11/src/pynchon/plugins/scaffolding/
+-rw-r--r--   0 runner    (1001) docker     (127)     3784 2024-04-03 17:06:30.000000 pynchon-2024.4.3.17.11/src/pynchon/plugins/scaffolding/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1158 2024-04-03 17:06:30.000000 pynchon-2024.4.3.17.11/src/pynchon/plugins/scaffolding/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7559 2024-04-03 17:06:30.000000 pynchon-2024.4.3.17.11/src/pynchon/plugins/src.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3893 2024-04-03 17:07:37.000000 pynchon-2024.4.3.17.11/src/pynchon/plugins/tests.py
+-rw-r--r--   0 runner    (1001) docker     (127)      402 2024-04-03 17:06:30.000000 pynchon-2024.4.3.17.11/src/pynchon/plugins/tox.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1445 2024-04-03 17:06:30.000000 pynchon-2024.4.3.17.11/src/pynchon/plugins/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-04-03 17:06:30.000000 pynchon-2024.4.3.17.11/src/pynchon/tagging.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:11:27.672485 pynchon-2024.4.3.17.11/src/pynchon/templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:11:27.692485 pynchon-2024.4.3.17.11/src/pynchon/templates/docker/
+-rw-r--r--   0 runner    (1001) docker     (127)      605 2024-04-03 17:06:30.000000 pynchon-2024.4.3.17.11/src/pynchon/templates/docker/Dockerfile.pandoc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:11:27.692485 pynchon-2024.4.3.17.11/src/pynchon/templates/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 17:06:30.000000 pynchon-2024.4.3.17.11/src/pynchon/templates/docs/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:11:27.668485 pynchon-2024.4.3.17.11/src/pynchon/templates/includes/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:11:27.668485 pynchon-2024.4.3.17.11/src/pynchon/templates/includes/pynchon/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:11:27.692485 pynchon-2024.4.3.17.11/src/pynchon/templates/includes/pynchon/github/
+-rw-r--r--   0 runner    (1001) docker     (127)      297 2024-04-03 17:06:30.000000 pynchon-2024.4.3.17.11/src/pynchon/templates/includes/pynchon/github/header.md.j2
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:11:27.672485 pynchon-2024.4.3.17.11/src/pynchon/templates/includes/pynchon/plugins/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:11:27.696485 pynchon-2024.4.3.17.11/src/pynchon/templates/includes/pynchon/plugins/core/
+-rw-r--r--   0 runner    (1001) docker     (127)      401 2024-04-03 17:06:30.000000 pynchon-2024.4.3.17.11/src/pynchon/templates/includes/pynchon/plugins/core/VERSIONS.md.j2
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:11:27.696485 pynchon-2024.4.3.17.11/src/pynchon/templates/includes/pynchon/plugins/core/bootstrap/
+-rw-r--r--   0 runner    (1001) docker     (127)      118 2024-04-03 17:06:30.000000 pynchon-2024.4.3.17.11/src/pynchon/templates/includes/pynchon/plugins/core/bootstrap/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)     1150 2024-04-03 17:06:30.000000 pynchon-2024.4.3.17.11/src/pynchon/templates/includes/pynchon/plugins/core/bootstrap/bash.sh
+-rw-r--r--   0 runner    (1001) docker     (127)      799 2024-04-03 17:06:30.000000 pynchon-2024.4.3.17.11/src/pynchon/templates/includes/pynchon/plugins/core/bootstrap/bashrc.sh
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-03 17:06:30.000000 pynchon-2024.4.3.17.11/src/pynchon/templates/includes/pynchon/plugins/core/bootstrap/makefile.j2
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-03 17:06:30.000000 pynchon-2024.4.3.17.11/src/pynchon/templates/includes/pynchon/plugins/core/bootstrap/python.j2
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-03 17:06:30.000000 pynchon-2024.4.3.17.11/src/pynchon/templates/includes/pynchon/plugins/core/bootstrap/sh.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      912 2024-04-03 17:06:30.000000 pynchon-2024.4.3.17.11/src/pynchon/templates/includes/pynchon/plugins/core/bootstrap/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:11:27.696485 pynchon-2024.4.3.17.11/src/pynchon/templates/includes/pynchon/plugins/fixme/
+-rw-r--r--   0 runner    (1001) docker     (127)      164 2024-04-03 17:06:30.000000 pynchon-2024.4.3.17.11/src/pynchon/templates/includes/pynchon/plugins/fixme/FIXME.md.j2
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:11:27.696485 pynchon-2024.4.3.17.11/src/pynchon/templates/includes/pynchon/plugins/makefile/
+-rw-r--r--   0 runner    (1001) docker     (127)     1202 2024-04-03 17:06:30.000000 pynchon-2024.4.3.17.11/src/pynchon/templates/includes/pynchon/plugins/makefile/mermaid-graph.mmd.j2
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:11:27.668485 pynchon-2024.4.3.17.11/src/pynchon/templates/includes/pynchon/plugins/python/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:11:27.696485 pynchon-2024.4.3.17.11/src/pynchon/templates/includes/pynchon/plugins/python/api/
+-rw-r--r--   0 runner    (1001) docker     (127)      105 2024-04-03 17:06:30.000000 pynchon-2024.4.3.17.11/src/pynchon/templates/includes/pynchon/plugins/python/api/TOC.md.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1218 2024-04-03 17:06:30.000000 pynchon-2024.4.3.17.11/src/pynchon/templates/includes/pynchon/plugins/python/api/classes.md.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      953 2024-04-03 17:06:30.000000 pynchon-2024.4.3.17.11/src/pynchon/templates/includes/pynchon/plugins/python/api/functions.md.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      324 2024-04-03 17:06:30.000000 pynchon-2024.4.3.17.11/src/pynchon/templates/includes/pynchon/plugins/python/api/modules.md.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      126 2024-04-03 17:06:30.000000 pynchon-2024.4.3.17.11/src/pynchon/templates/includes/pynchon/plugins/python/api/names.md.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      778 2024-04-03 17:06:30.000000 pynchon-2024.4.3.17.11/src/pynchon/templates/includes/pynchon/plugins/python/api/package.md.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     2987 2024-04-03 17:06:30.000000 pynchon-2024.4.3.17.11/src/pynchon/templates/includes/pynchon/plugins/python/api/toc2.md.j2
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:11:27.668485 pynchon-2024.4.3.17.11/src/pynchon/templates/includes/pynchon/plugins/python/gen/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:11:27.696485 pynchon-2024.4.3.17.11/src/pynchon/templates/includes/pynchon/plugins/python/gen/docstrings/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 17:06:30.000000 pynchon-2024.4.3.17.11/src/pynchon/templates/includes/pynchon/plugins/python/gen/docstrings/function.txt.j2
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 17:06:30.000000 pynchon-2024.4.3.17.11/src/pynchon/templates/includes/pynchon/plugins/python/gen/docstrings/module.txt.j2
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:11:27.700485 pynchon-2024.4.3.17.11/src/pynchon/templates/includes/pynchon/plugins/python_cli/
+-rw-r--r--   0 runner    (1001) docker     (127)     1449 2024-04-03 17:06:30.000000 pynchon-2024.4.3.17.11/src/pynchon/templates/includes/pynchon/plugins/python_cli/TOC.md.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      200 2024-04-03 17:06:30.000000 pynchon-2024.4.3.17.11/src/pynchon/templates/includes/pynchon/plugins/python_cli/detail.md.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      696 2024-04-03 17:06:30.000000 pynchon-2024.4.3.17.11/src/pynchon/templates/includes/pynchon/plugins/python_cli/main.module.md.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      910 2024-04-03 17:06:30.000000 pynchon-2024.4.3.17.11/src/pynchon/templates/includes/pynchon/plugins/python_cli/script.console.md.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      284 2024-04-03 17:06:30.000000 pynchon-2024.4.3.17.11/src/pynchon/templates/includes/pynchon/plugins/python_cli/subcommand.md.j2
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:11:27.672485 pynchon-2024.4.3.17.11/src/pynchon/templates/includes/pynchon/plugins/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:11:27.700485 pynchon-2024.4.3.17.11/src/pynchon/templates/includes/pynchon/plugins/src/header/
+-rw-r--r--   0 runner    (1001) docker     (127)      134 2024-04-03 17:06:30.000000 pynchon-2024.4.3.17.11/src/pynchon/templates/includes/pynchon/plugins/src/header/jinja-md.md.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      134 2024-04-03 17:06:30.000000 pynchon-2024.4.3.17.11/src/pynchon/templates/includes/pynchon/plugins/src/header/jinja.j2
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-04-03 17:06:30.000000 pynchon-2024.4.3.17.11/src/pynchon/templates/includes/pynchon/plugins/src/header/python.j2
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:11:27.700485 pynchon-2024.4.3.17.11/src/pynchon/templates/scaffolds/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 17:06:30.000000 pynchon-2024.4.3.17.11/src/pynchon/templates/scaffolds/.gitkeep
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:11:27.672485 pynchon-2024.4.3.17.11/src/pynchon/templates/scaffolds/ansible/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:11:27.700485 pynchon-2024.4.3.17.11/src/pynchon/templates/scaffolds/ansible/role/
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-03 17:06:30.000000 pynchon-2024.4.3.17.11/src/pynchon/templates/scaffolds/ansible/role/.ansible-lint
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:11:27.672485 pynchon-2024.4.3.17.11/src/pynchon/templates/scaffolds/ansible/role/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:11:27.700485 pynchon-2024.4.3.17.11/src/pynchon/templates/scaffolds/ansible/role/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 17:06:30.000000 pynchon-2024.4.3.17.11/src/pynchon/templates/scaffolds/ansible/role/.github/workflows/ansible-lint.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      505 2024-04-03 17:06:30.000000 pynchon-2024.4.3.17.11/src/pynchon/templates/scaffolds/ansible/role/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:11:27.700485 pynchon-2024.4.3.17.11/src/pynchon/templates/scaffolds/docker/
+-rw-r--r--   0 runner    (1001) docker     (127)     1079 2024-04-03 17:06:30.000000 pynchon-2024.4.3.17.11/src/pynchon/templates/scaffolds/docker/.dockerignore
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-04-03 17:06:30.000000 pynchon-2024.4.3.17.11/src/pynchon/templates/scaffolds/docker/.scaffold.advice.json5
+-rw-r--r--   0 runner    (1001) docker     (127)      162 2024-04-03 17:06:30.000000 pynchon-2024.4.3.17.11/src/pynchon/templates/scaffolds/docker/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (127)     1374 2024-04-03 17:06:30.000000 pynchon-2024.4.3.17.11/src/pynchon/templates/scaffolds/docker/README.md.j2
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:11:27.672485 pynchon-2024.4.3.17.11/src/pynchon/templates/scaffolds/docs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:11:27.700485 pynchon-2024.4.3.17.11/src/pynchon/templates/scaffolds/docs/includes/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 17:06:30.000000 pynchon-2024.4.3.17.11/src/pynchon/templates/scaffolds/docs/includes/.gitkeep
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:11:27.700485 pynchon-2024.4.3.17.11/src/pynchon/templates/scaffolds/github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:11:27.672485 pynchon-2024.4.3.17.11/src/pynchon/templates/scaffolds/github/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:11:27.700485 pynchon-2024.4.3.17.11/src/pynchon/templates/scaffolds/github/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 17:06:30.000000 pynchon-2024.4.3.17.11/src/pynchon/templates/scaffolds/github/.github/workflows/.gitkeep
+-rw-r--r--   0 runner    (1001) docker     (127)      153 2024-04-03 17:06:30.000000 pynchon-2024.4.3.17.11/src/pynchon/templates/scaffolds/github/.github/workflows/hello-world.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-03 17:06:30.000000 pynchon-2024.4.3.17.11/src/pynchon/templates/scaffolds/github/.scaffold.advice.json5
+-rw-r--r--   0 runner    (1001) docker     (127)      458 2024-04-03 17:06:30.000000 pynchon-2024.4.3.17.11/src/pynchon/templates/scaffolds/github/README.md.j2
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:11:27.672485 pynchon-2024.4.3.17.11/src/pynchon/templates/scaffolds/py/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:11:27.704485 pynchon-2024.4.3.17.11/src/pynchon/templates/scaffolds/py/pkg/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 17:06:30.000000 pynchon-2024.4.3.17.11/src/pynchon/templates/scaffolds/py/pkg/.ackrc
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 17:06:30.000000 pynchon-2024.4.3.17.11/src/pynchon/templates/scaffolds/py/pkg/.flake8
+-rw-r--r--   0 runner    (1001) docker     (127)      776 2024-04-03 17:06:30.000000 pynchon-2024.4.3.17.11/src/pynchon/templates/scaffolds/py/pkg/.libcst.codemod.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       64 2024-04-03 17:06:30.000000 pynchon-2024.4.3.17.11/src/pynchon/templates/scaffolds/py/pkg/.scaffold.advice.json5
+-rw-r--r--   0 runner    (1001) docker     (127)     1928 2024-04-03 17:06:30.000000 pynchon-2024.4.3.17.11/src/pynchon/templates/scaffolds/py/pkg/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)     2233 2024-04-03 17:06:30.000000 pynchon-2024.4.3.17.11/src/pynchon/templates/scaffolds/py/pkg/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1549 2024-04-03 17:06:30.000000 pynchon-2024.4.3.17.11/src/pynchon/templates/scaffolds/py/pkg/README.md.j2
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:11:27.704485 pynchon-2024.4.3.17.11/src/pynchon/templates/scaffolds/py/pkg/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 17:06:30.000000 pynchon-2024.4.3.17.11/src/pynchon/templates/scaffolds/py/pkg/docs/.gitkeep
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:11:27.704485 pynchon-2024.4.3.17.11/src/pynchon/templates/scaffolds/py/pkg/docs/html/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 17:06:30.000000 pynchon-2024.4.3.17.11/src/pynchon/templates/scaffolds/py/pkg/docs/html/.gitkeep
+-rw-r--r--   0 runner    (1001) docker     (127)     2396 2024-04-03 17:06:30.000000 pynchon-2024.4.3.17.11/src/pynchon/templates/scaffolds/py/pkg/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      771 2024-04-03 17:06:30.000000 pynchon-2024.4.3.17.11/src/pynchon/templates/scaffolds/py/pkg/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:11:27.672485 pynchon-2024.4.3.17.11/src/pynchon/templates/scaffolds/py/pkg/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:11:27.704485 pynchon-2024.4.3.17.11/src/pynchon/templates/scaffolds/py/pkg/src/{{name}}/
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-03 17:06:30.000000 pynchon-2024.4.3.17.11/src/pynchon/templates/scaffolds/py/pkg/src/{{name}}/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-03 17:06:30.000000 pynchon-2024.4.3.17.11/src/pynchon/templates/scaffolds/py/pkg/src/{{name}}/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-03 17:06:30.000000 pynchon-2024.4.3.17.11/src/pynchon/templates/scaffolds/py/pkg/src/{{name}}/app.py
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-03 17:06:30.000000 pynchon-2024.4.3.17.11/src/pynchon/templates/scaffolds/py/pkg/src/{{name}}/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-04-03 17:06:30.000000 pynchon-2024.4.3.17.11/src/pynchon/templates/scaffolds/py/pkg/src/{{name}}/lme.py
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-03 17:06:30.000000 pynchon-2024.4.3.17.11/src/pynchon/templates/scaffolds/py/pkg/src/{{name}}/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-04-03 17:06:30.000000 pynchon-2024.4.3.17.11/src/pynchon/templates/scaffolds/py/pkg/src/{{name}}/tagging.py
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-03 17:06:30.000000 pynchon-2024.4.3.17.11/src/pynchon/templates/scaffolds/py/pkg/src/{{name}}/typing.py
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-03 17:06:30.000000 pynchon-2024.4.3.17.11/src/pynchon/templates/scaffolds/py/pkg/src/{{name}}/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:11:27.704485 pynchon-2024.4.3.17.11/src/pynchon/templates/scaffolds/py/pkg/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 17:06:30.000000 pynchon-2024.4.3.17.11/src/pynchon/templates/scaffolds/py/pkg/tests/.gitkeep
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 17:06:30.000000 pynchon-2024.4.3.17.11/src/pynchon/templates/scaffolds/py/pkg/tests/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:11:27.708485 pynchon-2024.4.3.17.11/src/pynchon/templates/scaffolds/py/pkg/tests/integration/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 17:06:30.000000 pynchon-2024.4.3.17.11/src/pynchon/templates/scaffolds/py/pkg/tests/integration/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-03 17:06:30.000000 pynchon-2024.4.3.17.11/src/pynchon/templates/scaffolds/py/pkg/tests/integration/test_all.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:11:27.708485 pynchon-2024.4.3.17.11/src/pynchon/templates/scaffolds/py/pkg/tests/smoke/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 17:06:30.000000 pynchon-2024.4.3.17.11/src/pynchon/templates/scaffolds/py/pkg/tests/smoke/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-03 17:06:30.000000 pynchon-2024.4.3.17.11/src/pynchon/templates/scaffolds/py/pkg/tests/smoke/test_all.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:11:27.708485 pynchon-2024.4.3.17.11/src/pynchon/templates/scaffolds/py/pkg/tests/units/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 17:06:30.000000 pynchon-2024.4.3.17.11/src/pynchon/templates/scaffolds/py/pkg/tests/units/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-03 17:06:30.000000 pynchon-2024.4.3.17.11/src/pynchon/templates/scaffolds/py/pkg/tests/units/test_all.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3097 2024-04-03 17:06:30.000000 pynchon-2024.4.3.17.11/src/pynchon/templates/scaffolds/py/pkg/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:11:27.708485 pynchon-2024.4.3.17.11/src/pynchon/templates/scaffolds/py/workspace/
+-rw-r--r--   0 runner    (1001) docker     (127)       64 2024-04-03 17:06:30.000000 pynchon-2024.4.3.17.11/src/pynchon/templates/scaffolds/py/workspace/.scaffold.advice.json5
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:11:27.672485 pynchon-2024.4.3.17.11/src/pynchon/templates/scaffolds/software/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:11:27.708485 pynchon-2024.4.3.17.11/src/pynchon/templates/scaffolds/software/automation/
+-rw-r--r--   0 runner    (1001) docker     (127)      348 2024-04-03 17:06:30.000000 pynchon-2024.4.3.17.11/src/pynchon/templates/scaffolds/software/automation/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:11:27.708485 pynchon-2024.4.3.17.11/src/pynchon/templates/scaffolds/software/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      348 2024-04-03 17:06:30.000000 pynchon-2024.4.3.17.11/src/pynchon/templates/scaffolds/software/tests/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:11:27.672485 pynchon-2024.4.3.17.11/src/pynchon/templates/scaffolds/software/tests/tests/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:11:27.708485 pynchon-2024.4.3.17.11/src/pynchon/templates/scaffolds/software/tests/tests/integration/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 17:06:30.000000 pynchon-2024.4.3.17.11/src/pynchon/templates/scaffolds/software/tests/tests/integration/.gitkeep
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:11:27.708485 pynchon-2024.4.3.17.11/src/pynchon/templates/scaffolds/software/tests/tests/smoke/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 17:06:30.000000 pynchon-2024.4.3.17.11/src/pynchon/templates/scaffolds/software/tests/tests/smoke/.gitkeep
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:11:27.708485 pynchon-2024.4.3.17.11/src/pynchon/templates/scaffolds/software/tests/tests/units/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 17:06:30.000000 pynchon-2024.4.3.17.11/src/pynchon/templates/scaffolds/software/tests/tests/units/.gitkeep
+-rw-r--r--   0 runner    (1001) docker     (127)      284 2024-04-03 17:06:30.000000 pynchon-2024.4.3.17.11/src/pynchon/testing.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:11:27.708485 pynchon-2024.4.3.17.11/src/pynchon/util/
+-rw-r--r--   0 runner    (1001) docker     (127)     1055 2024-04-03 17:06:30.000000 pynchon-2024.4.3.17.11/src/pynchon/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-03 17:06:30.000000 pynchon-2024.4.3.17.11/src/pynchon/util/click.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6160 2024-04-03 17:07:37.000000 pynchon-2024.4.3.17.11/src/pynchon/util/complexity.py
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-03 17:06:30.000000 pynchon-2024.4.3.17.11/src/pynchon/util/config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:11:27.712485 pynchon-2024.4.3.17.11/src/pynchon/util/console/
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-03 17:06:30.000000 pynchon-2024.4.3.17.11/src/pynchon/util/console/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-03 17:06:30.000000 pynchon-2024.4.3.17.11/src/pynchon/util/console/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4662 2024-04-03 17:06:30.000000 pynchon-2024.4.3.17.11/src/pynchon/util/docker.py
+-rw-r--r--   0 runner    (1001) docker     (127)      711 2024-04-03 17:07:37.000000 pynchon-2024.4.3.17.11/src/pynchon/util/events.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:11:27.712485 pynchon-2024.4.3.17.11/src/pynchon/util/files/
+-rw-r--r--   0 runner    (1001) docker     (127)     3902 2024-04-03 17:07:37.000000 pynchon-2024.4.3.17.11/src/pynchon/util/files/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      948 2024-04-03 17:07:37.000000 pynchon-2024.4.3.17.11/src/pynchon/util/files/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2089 2024-04-03 17:07:37.000000 pynchon-2024.4.3.17.11/src/pynchon/util/files/diff.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2608 2024-04-03 17:07:37.000000 pynchon-2024.4.3.17.11/src/pynchon/util/lme.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:11:27.712485 pynchon-2024.4.3.17.11/src/pynchon/util/makefile/
+-rw-r--r--   0 runner    (1001) docker     (127)     5276 2024-04-03 17:07:37.000000 pynchon-2024.4.3.17.11/src/pynchon/util/makefile/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      484 2024-04-03 17:07:37.000000 pynchon-2024.4.3.17.11/src/pynchon/util/makefile/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1139 2024-04-03 17:06:30.000000 pynchon-2024.4.3.17.11/src/pynchon/util/oop.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:11:27.712485 pynchon-2024.4.3.17.11/src/pynchon/util/os/
+-rw-r--r--   0 runner    (1001) docker     (127)      578 2024-04-03 17:06:30.000000 pynchon-2024.4.3.17.11/src/pynchon/util/os/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5760 2024-04-03 17:06:30.000000 pynchon-2024.4.3.17.11/src/pynchon/util/os/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-04-03 17:06:30.000000 pynchon-2024.4.3.17.11/src/pynchon/util/os/pidfile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1081 2024-04-03 17:06:30.000000 pynchon-2024.4.3.17.11/src/pynchon/util/os/pids.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2054 2024-04-03 17:06:30.000000 pynchon-2024.4.3.17.11/src/pynchon/util/python.py
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-04-03 17:06:30.000000 pynchon-2024.4.3.17.11/src/pynchon/util/splitvt.py
+-rw-r--r--   0 runner    (1001) docker     (127)      463 2024-04-03 17:06:30.000000 pynchon-2024.4.3.17.11/src/pynchon/util/testing.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:11:27.712485 pynchon-2024.4.3.17.11/src/pynchon/util/text/
+-rw-r--r--   0 runner    (1001) docker     (127)      551 2024-04-03 17:06:30.000000 pynchon-2024.4.3.17.11/src/pynchon/util/text/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      367 2024-04-03 17:07:37.000000 pynchon-2024.4.3.17.11/src/pynchon/util/text/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:11:27.712485 pynchon-2024.4.3.17.11/src/pynchon/util/text/dumpf/
+-rw-r--r--   0 runner    (1001) docker     (127)      790 2024-04-03 17:07:37.000000 pynchon-2024.4.3.17.11/src/pynchon/util/text/dumpf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1047 2024-04-03 17:07:37.000000 pynchon-2024.4.3.17.11/src/pynchon/util/text/dumpf/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      598 2024-04-03 17:06:30.000000 pynchon-2024.4.3.17.11/src/pynchon/util/text/dumps.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:11:27.712485 pynchon-2024.4.3.17.11/src/pynchon/util/text/loadf/
+-rw-r--r--   0 runner    (1001) docker     (127)     7414 2024-04-03 17:07:37.000000 pynchon-2024.4.3.17.11/src/pynchon/util/text/loadf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1042 2024-04-03 17:07:37.000000 pynchon-2024.4.3.17.11/src/pynchon/util/text/loadf/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1950 2024-04-03 17:07:37.000000 pynchon-2024.4.3.17.11/src/pynchon/util/text/loads.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:11:27.712485 pynchon-2024.4.3.17.11/src/pynchon/util/text/normalize/
+-rw-r--r--   0 runner    (1001) docker     (127)     1285 2024-04-03 17:06:30.000000 pynchon-2024.4.3.17.11/src/pynchon/util/text/normalize/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:11:27.712485 pynchon-2024.4.3.17.11/src/pynchon/util/text/render/
+-rw-r--r--   0 runner    (1001) docker     (127)     5825 2024-04-03 17:07:37.000000 pynchon-2024.4.3.17.11/src/pynchon/util/text/render/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      972 2024-04-03 17:07:37.000000 pynchon-2024.4.3.17.11/src/pynchon/util/text/render/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1395 2024-04-03 17:06:30.000000 pynchon-2024.4.3.17.11/src/pynchon/util/typing.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 17:11:27.712485 pynchon-2024.4.3.17.11/src/pynchon.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1714 2024-04-03 17:11:27.000000 pynchon-2024.4.3.17.11/src/pynchon.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     9272 2024-04-03 17:11:27.000000 pynchon-2024.4.3.17.11/src/pynchon.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 17:11:27.000000 pynchon-2024.4.3.17.11/src/pynchon.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-04-03 17:11:27.000000 pynchon-2024.4.3.17.11/src/pynchon.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 17:11:27.000000 pynchon-2024.4.3.17.11/src/pynchon.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      438 2024-04-03 17:11:27.000000 pynchon-2024.4.3.17.11/src/pynchon.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-03 17:11:27.000000 pynchon-2024.4.3.17.11/src/pynchon.egg-info/top_level.txt
```

### Comparing `pynchon-2024.3.5.19.3/PKG-INFO` & `pynchon-2024.4.3.17.11/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pynchon
-Version: 2024.3.5.19.3
+Version: 2024.4.3.17.11
 Summary: Autodocs for python projects
 Home-page: https://github.com/elo-enterprises/pynchon/
 Author: elo
 Author-email: engineering@elo.enterprises
 License: MIT
 Project-URL: Documentation, https://github.com/elo-enterprises/pynchon/
 Project-URL: Source, https://github.com/elo-enterprises/pynchon/
@@ -27,17 +27,17 @@
 Requires-Dist: tomli_w==1.0.0
 Requires-Dist: tomli
 Requires-Dist: griffe==0.23.0
 Requires-Dist: mccabe==0.7.0
 Requires-Dist: Jinja2==3.1.2
 Requires-Dist: grip==4.6.1
 Requires-Dist: psutil==5.9.5
-Provides-Extra: mkdocs
-Requires-Dist: mkdocs>=1.5.3; extra == "mkdocs"
-Requires-Dist: mkdocs-material==9.5.3; extra == "mkdocs"
+Requires-Dist: mkdocs>=1.5.3
+Requires-Dist: mkdocs-material==9.5.3
+Requires-Dist: beautifulsoup4==4.12.3
 Provides-Extra: dev
 Requires-Dist: IPython; extra == "dev"
 Provides-Extra: testing
 Requires-Dist: IPython; extra == "testing"
 Requires-Dist: tox; extra == "testing"
 Requires-Dist: pytest; extra == "testing"
 Requires-Dist: pytest-cov; extra == "testing"
```

### Comparing `pynchon-2024.3.5.19.3/pyproject.toml` & `pynchon-2024.4.3.17.11/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pynchon-2024.3.5.19.3/setup.cfg` & `pynchon-2024.4.3.17.11/setup.cfg`

 * *Files 7% similar despite different names*

```diff
@@ -40,24 +40,24 @@
 	tomli_w==1.0.0   # parsing toml
 	tomli            # as tomllib; tomllib only available in py3.11
 	griffe==0.23.0
 	mccabe==0.7.0
 	Jinja2==3.1.2
 	grip==4.6.1
 	psutil==5.9.5
+	mkdocs>=1.5.3
+	mkdocs-material==9.5.3
+	beautifulsoup4==4.12.3
 
 [options.packages.find]
 where = src
 exclude = 
 	tests
 
 [options.extras_require]
-mkdocs = 
-	mkdocs>=1.5.3
-	mkdocs-material==9.5.3
 dev = 
 	IPython
 testing = 
 	IPython
 	tox
 	pytest
 	pytest-cov
```

### Comparing `pynchon-2024.3.5.19.3/setup.py` & `pynchon-2024.4.3.17.11/setup.py`

 * *Files identical despite different names*

### Comparing `pynchon-2024.3.5.19.3/src/pynchon/abcs/attrdict.py` & `pynchon-2024.4.3.17.11/src/pynchon/abcs/attrdict.py`

 * *Files identical despite different names*

### Comparing `pynchon-2024.3.5.19.3/src/pynchon/abcs/path.py` & `pynchon-2024.4.3.17.11/src/pynchon/abcs/path.py`

 * *Files identical despite different names*

### Comparing `pynchon-2024.3.5.19.3/src/pynchon/abcs/visitor.py` & `pynchon-2024.4.3.17.11/src/pynchon/abcs/visitor.py`

 * *Files identical despite different names*

### Comparing `pynchon-2024.3.5.19.3/src/pynchon/annotate.py` & `pynchon-2024.4.3.17.11/src/pynchon/annotate.py`

 * *Files identical despite different names*

### Comparing `pynchon-2024.3.5.19.3/src/pynchon/api/project/__init__.py` & `pynchon-2024.4.3.17.11/src/pynchon/api/project/__init__.py`

 * *Files identical despite different names*

### Comparing `pynchon-2024.3.5.19.3/src/pynchon/app.py` & `pynchon-2024.4.3.17.11/src/pynchon/app.py`

 * *Files identical despite different names*

### Comparing `pynchon-2024.3.5.19.3/src/pynchon/bin.py` & `pynchon-2024.4.3.17.11/src/pynchon/bin.py`

 * *Files identical despite different names*

### Comparing `pynchon-2024.3.5.19.3/src/pynchon/cli/common.py` & `pynchon-2024.4.3.17.11/src/pynchon/cli/common.py`

 * *Files identical despite different names*

### Comparing `pynchon-2024.3.5.19.3/src/pynchon/codemod/commands/docstrings/base.py` & `pynchon-2024.4.3.17.11/src/pynchon/codemod/commands/docstrings/base.py`

 * *Files identical despite different names*

### Comparing `pynchon-2024.3.5.19.3/src/pynchon/codemod/commands/docstrings/javadoc.py` & `pynchon-2024.4.3.17.11/src/pynchon/codemod/commands/docstrings/javadoc.py`

 * *Files identical despite different names*

### Comparing `pynchon-2024.3.5.19.3/src/pynchon/codemod/commands/docstrings/simple.py` & `pynchon-2024.4.3.17.11/src/pynchon/codemod/commands/docstrings/simple.py`

 * *Files identical despite different names*

### Comparing `pynchon-2024.3.5.19.3/src/pynchon/config/__init__.py` & `pynchon-2024.4.3.17.11/src/pynchon/config/__init__.py`

 * *Files identical despite different names*

### Comparing `pynchon-2024.3.5.19.3/src/pynchon/config/util.py` & `pynchon-2024.4.3.17.11/src/pynchon/config/util.py`

 * *Files identical despite different names*

### Comparing `pynchon-2024.3.5.19.3/src/pynchon/constants.py` & `pynchon-2024.4.3.17.11/src/pynchon/constants.py`

 * *Files identical despite different names*

### Comparing `pynchon-2024.3.5.19.3/src/pynchon/core.py` & `pynchon-2024.4.3.17.11/src/pynchon/core.py`

 * *Files identical despite different names*

### Comparing `pynchon-2024.3.5.19.3/src/pynchon/events.py` & `pynchon-2024.4.3.17.11/src/pynchon/events.py`

 * *Files identical despite different names*

### Comparing `pynchon-2024.3.5.19.3/src/pynchon/models/planner.py` & `pynchon-2024.4.3.17.11/src/pynchon/models/planner.py`

 * *Files 15% similar despite different names*

```diff
@@ -8,25 +8,49 @@
 
 from pynchon import abcs, cli
 from pynchon.app import app
 
 from . import planning
 from .plugins import BasePlugin
 
-from pynchon.util import lme, typing  # noqa
+from pynchon.util import files, lme, typing  # noqa
 
 
 LOGGER = lme.get_logger(" ")
 
 
 @tags(cli_label="Planner")
 class AbstractPlanner(BasePlugin):
     """A plugin-type that provides plan/apply basics"""
 
-    cli_label = "Planner"
+    def _list(self, use_glob=None, changes=False):
+        """
+        Lists affected resources for this project
+        """
+        use_glob = use_glob or getattr(self.__class__, "file_glob", None)
+        assert use_glob
+        default = self[:"project"]
+        proj_conf = self[:"project.subproject":default]
+        project_root = proj_conf.get("root", None) or self[:"git.root":"."]
+        globs = [
+            abcs.Path(project_root).joinpath(f"**/{use_glob}"),
+        ]
+        self.logger.debug(f"search patterns are {globs}")
+        result = files.find_globs(globs)
+        self.logger.debug(f"found {len(result)} {use_glob} files (pre-filter)")
+        excludes = self["exclude_patterns"::[]]
+        # NB: always honor the global-excludes
+        excludes += self.siblings["globals"]["exclude_patterns"::[]]
+        self.logger.debug(f"filtering search with {len(excludes)} excludes")
+        result = [p for p in result if not p.match_any_glob(excludes)]
+        self.logger.debug(f"found {len(result)} {use_glob} files (post-filter)")
+        if not result:
+            err = f"active, but found no {use_glob} files!"
+            self.logger.critical(err)
+        return result
 
     @tags(publish_to_cli=False)
     def goal(self, **kwargs):
         """ """
         return planning.Goal(
             owner=f"{self.__class__.__module__}.{self.__class__.__name__}", **kwargs
         )
@@ -52,27 +76,27 @@
             for g in goals:
                 _type = g.pop("type", "from-config")
                 cmd = g.pop("command", None)
                 cmd = cmd and cmd.format(**g)
                 g.update(command=cmd, type=_type)
                 plan.append(self.goal(**g))
         else:
+            self.logger.critical(f"packing  {len(goals)} goals")
             for g in goals:
-                LOGGER.critical(f"packaging {g}")
                 plan.append(g)
         app.status_bar.update(app="Pynchon", stage=f"{len(plan)}")
         return plan
 
-    @cli.click.flag("--quiet", "-q", default=False, help="Disable JSON output")
-    @cli.click.option("--parallelism", "-p", default="1", help="Paralellism")
-    @cli.click.flag("--fail-fast", default=False, help="fail fast")
+    @cli.options.quiet
+    @cli.options.parallelism
+    @cli.options.fail_fast
     def apply(
         self,
         plan: planning.Plan = None,
-        parallelism: str = "1",
+        parallelism: str = "0",
         fail_fast: bool = False,
         quiet: bool = False,
     ) -> planning.ApplyResults:
         """
         Executes the plan for this plugin
         """
         parallelism = int(parallelism)
@@ -85,19 +109,20 @@
             f"{self.name}.apply ( {len(plan)} goals with {parallelism} workers)"
         )
         results = plan.apply(parallelism=parallelism, git=self.siblings["git"])
 
         LOGGER.critical(
             f"{self.name}.apply finished ( {len(results.actions)}/{len(results.goals)} goals )"
         )
-        self.dispatch_apply_hooks(results)
+        self._dispatch_apply_hooks(results)
         if not quiet:
             return results
 
-    def dispatch_apply_hooks(self, results: planning.ApplyResults):
+    def _dispatch_apply_hooks(self, results: planning.ApplyResults):
+        """ """
         # write status event (used by the app-console)
         app.status_bar.update(
             app="Pynchon::HOOKS",
             stage=f"{self.__class__.name}",
         )
         if results.finished:
             hooks = self.apply_hooks
@@ -139,14 +164,18 @@
     @memoized_property
     def hooks(self):
         """ """
         hooks = self["hooks"::[]]
         self._validate_hooks(hooks)
         return hooks
 
+    def _hook_diff_after_apply(self, result: planning.ApplyResults) -> bool:
+        """ """
+        self.logger.warning("diff-after-apply not implemented yet")
+
     def _hook_open_after_apply(self, result: planning.ApplyResults) -> bool:
         """ """
         changes = list({r.resource for r in result})
         changes = [abcs.Path(rsrc) for rsrc in changes]
         changes = [rsrc for rsrc in changes if not rsrc.is_dir()]
         self.logger.warning(f"Opening {len(changes)} changed resources.")
         docs_plugin = self if self.name == "docs" else self.siblings["docs"]
```

### Comparing `pynchon-2024.3.5.19.3/src/pynchon/models/planning.py` & `pynchon-2024.4.3.17.11/src/pynchon/models/planning.py`

 * *Files 6% similar despite different names*

```diff
@@ -39,15 +39,15 @@
 
 
 class Action(BaseModel):
     """ """
 
     type: str = typing.Field(default="unknown_action_type")
     ok: bool = typing.Field(default=None)
-    error: str = typing.Field(default="")
+    error: typing.StringMaybe = typing.Field(default="")
     changed: bool = typing.Field(default=False)
     resource: abcs.ResourceType = typing.Field(default="??")
     command: str = typing.Field(default="echo")
     callable: typing.CallableMaybe = typing.Field(help="", default=None)
     owner: typing.StringMaybe = typing.Field(
         help="Name of the plugin that owns this Action", default=None
     )
@@ -157,15 +157,15 @@
 
     def act(goal, git=None, plugin_name="?", ordering="?"):
         """ """
         pynchon_app.status_bar.update(
             app="Pynchon::APPLY",
             stage=f"{plugin_name} plugin {ordering}",
         )
-        invocation = invoke(goal.command)
+        invocation = invoke(goal.command, interactive=goal.type == "interactive")
         success = invocation.succeeded
         action = dict(
             ok=success,
             ordering=goal.ordering,
             error="" if success else invocation.stderr,
             # log=invocation.succeeded and invocation.stderr else None,
             owner=goal.owner,
@@ -223,42 +223,61 @@
     """ """
 
     goals: typing.List[Goal] = typing.Field(default=[])
     owner: typing.StringMaybe = typing.Field(
         help="Name of the plugin that owns this Plan", default=None
     )
 
-    def apply(self, parallelism: int = 1, fail_fast: bool = True, git=None):
+    def apply(self, parallelism: int = 0, fail_fast: bool = True, git=None):
         """ """
         goals = self.goals
         total = len(goals)
 
         jobs = []
-        with concurrent.futures.ThreadPoolExecutor(max_workers=parallelism) as executor:
+        results = []
+        if parallelism:
+            LOGGER.warning(f"parallel execution enabled (workers={parallelism})")
+            with concurrent.futures.ThreadPoolExecutor(
+                max_workers=parallelism
+            ) as executor:
+                for i, goal in enumerate(goals):
+                    ordering = f"  {i+1}/{total}"
+                    jobs.append(
+                        executor.submit(
+                            goal.act,
+                            git=git,
+                            plugin_name=self.__class__.__name__,
+                            ordering=ordering,
+                        )
+                    )
+            for i, future in enumerate(concurrent.futures.as_completed(jobs)):
+                # LOGGER.debug(f' waiting for {i+1} / {total}')
+                action = future.result()
+                results.append(action)
+                lme.CONSOLE.print(action)
+                if fail_fast and not action.ok:
+                    msg = f"fail-fast is set, so exiting early.  exception follows\n\n{action.error}"
+                    LOGGER.critical(msg)
+                    break
+        else:
+            LOGGER.warning(f"parallel execution disabled (workers={parallelism})")
             for i, goal in enumerate(goals):
                 ordering = f"  {i+1}/{total}"
-                jobs.append(
-                    executor.submit(
-                        goal.act,
-                        git=git,
-                        plugin_name=self.__class__.__name__,
-                        ordering=ordering,
-                    )
+                lme.CONSOLE.print(goal)
+                action = goal.act(
+                    git=git,
+                    plugin_name=self.__class__.__name__,
+                    ordering=ordering,
                 )
-        results = []
-        for i, future in enumerate(concurrent.futures.as_completed(jobs)):
-            # LOGGER.debug(f' waiting for {i+1} / {total}')
-            action = future.result()
-            results.append(action)
-            lme.CONSOLE.print(action)
-            if fail_fast and not action.ok:
-                msg = f"fail-fast is set, so exiting early.  exception follows\n\n{action.error}"
-                LOGGER.critical(msg)
-                break
-
+                # lme.CONSOLE.print(action)
+                results.append(action)
+                if fail_fast and not action.ok:
+                    msg = f"fail-fast is set, so exiting early.  exception follows\n\n{action.error}"
+                    LOGGER.critical(msg)
+                    break
         results = ApplyResults(actions=results, goals=goals)
         return results
 
     def finalize(self):
         """
         When a plan is finished being appended to,
         it can be "finalized" to set the `ordering` value
@@ -372,15 +391,15 @@
     def __len__(self):
         return len(self.actions)
 
     def __iter__(self):
         return iter(self.actions)
 
     @property
-    def ok(self):
+    def ok(self) -> bool:
         return self.finished and all([a.ok for a in self])
 
     @property
     def action_types(self):
         tmp = list({g.type for g in self})
         return {k: [] for k in tmp}
```

### Comparing `pynchon-2024.3.5.19.3/src/pynchon/models/plugins/__init__.py` & `pynchon-2024.4.3.17.11/src/pynchon/models/plugins/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 from fleks import tagging
 
 from pynchon import abcs, api, cli, events  # noqa
 from pynchon.util import lme, typing  # noqa
 
 from . import validators  # noqa
 from .cli import CliPlugin  # noqa
+from .docker import DockerWrapper  # noqa
 from .provider import Provider  # noqa
 from .pynchon import PynchonPlugin  # noqa
 from .tool import ToolPlugin  # noqa
 
 LOGGER = lme.get_logger(__name__)
 classproperty = fleks.util.typing.classproperty
```

### Comparing `pynchon-2024.3.5.19.3/src/pynchon/models/plugins/cli.py` & `pynchon-2024.4.3.17.11/src/pynchon/models/plugins/cli.py`

 * *Files identical despite different names*

### Comparing `pynchon-2024.3.5.19.3/src/pynchon/models/plugins/provider.py` & `pynchon-2024.4.3.17.11/src/pynchon/models/plugins/provider.py`

 * *Files identical despite different names*

### Comparing `pynchon-2024.3.5.19.3/src/pynchon/models/plugins/pynchon.py` & `pynchon-2024.4.3.17.11/src/pynchon/models/plugins/pynchon.py`

 * *Files identical despite different names*

### Comparing `pynchon-2024.3.5.19.3/src/pynchon/models/plugins/tool.py` & `pynchon-2024.4.3.17.11/src/pynchon/models/plugins/tool.py`

 * *Files identical despite different names*

### Comparing `pynchon-2024.3.5.19.3/src/pynchon/models/plugins/validators.py` & `pynchon-2024.4.3.17.11/src/pynchon/models/plugins/validators.py`

 * *Files identical despite different names*

### Comparing `pynchon-2024.3.5.19.3/src/pynchon/models/python.py` & `pynchon-2024.4.3.17.11/src/pynchon/models/python.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from pynchon.util import lme, typing
 
 LOGGER = lme.get_logger(__name__)
 
 
 class EntrypointMetadata(BaseModel):
     is_click: bool = typing.Field(help="", required=False, default=False)
-    is_package: bool = typing.Field(help="", required=False, default=False)
+    is_package_entrypoint: bool = typing.Field(help="", required=False, default=False)
     is_module: bool = typing.Field(help="", required=False, default=True)
     bin_name: typing.StringMaybe = typing.Field(
         help="Name for this console script. (Nil if module-entrypoint)",
         required=False,
         default=None,
     )
     help_command: typing.StringMaybe = typing.Field(
@@ -31,27 +31,32 @@
         help="",
         required=True,
     )
     resource: abcs.Path = typing.Field(help="", required=True)
     path: abcs.Path = typing.Field(help="", required=True)
     entrypoints: typing.List = typing.Field(help="", required=False, default=[])
     src_root: abcs.Path = typing.Field(required=True)
+    inside_src_root: bool = typing.Field(default=True)
 
     @property
     def src_url(self) -> str:
-        return "/" + str(self.path.relative_to(self.src_root.parent))
+        if not self.inside_src_root:
+            return ""
+        else:
+            tmp = self.path.relative_to(self.src_root.parent)
+            return "/" + str(tmp)
         # return abcs.Path(path).absolute().relative_to(abcs.Path(git_root).absolute())
 
     @property
     def help_invocation(self):
         if self.help_command is not None:
             return self.help_command
         elif self.is_module:
             return f"python -m{self.dotpath} --help"
-        # if self.is_package:
+        # if self.is_package_entrypoint:
         #     return f""
         raise ValueError(f"Cannot determine help_invocation for {self}")
 
     @property
     def help_output(self):
         """
         Computes help-output given help-invocation.
```

### Comparing `pynchon-2024.3.5.19.3/src/pynchon/plugins/__init__.py` & `pynchon-2024.4.3.17.11/src/pynchon/plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `pynchon-2024.3.5.19.3/src/pynchon/plugins/cicd.py` & `pynchon-2024.4.3.17.11/src/pynchon/plugins/cicd.py`

 * *Files identical despite different names*

### Comparing `pynchon-2024.3.5.19.3/src/pynchon/plugins/core.py` & `pynchon-2024.4.3.17.11/src/pynchon/plugins/core.py`

 * *Files 6% similar despite different names*

```diff
@@ -31,24 +31,56 @@
         """ """
         kls._finalized_click_groups[kls] = entry
         return kls._finalized_click_groups[kls]
 
     @classmethod
     def get_current_config(kls):
         """ """
-        from pynchon import config as config_mod
+        from pynchon import config as config_mod  # noqa
 
         result = getattr(config_mod, kls.get_config_key())
         return result
 
     def cfg(self):
         """Show current project config (with templating/interpolation)"""
         tmp = self.project_config
         return tmp
 
+    def init(self, strict=True):
+        """Write .pynchon.json5 if it's not present"""
+        default_config = abcs.Path(".") / ".pynchon.json5"
+        if default_config.exists():
+            LOGGER.critical(f"{default_config} exists, nothing to do.")
+            err = f"Refusing to create {default_config} (file already exists)"
+            LOGGER.critical(err)
+            if strict:
+                raise SystemExit(1)
+        else:
+            self._init_config(default_config)
+            return True
+
+    def _init_config(self, config_path):
+        """ """
+        cfg = self.cfg().dict()
+        pop_list = ["apply_hooks"]
+        for plugin_name in cfg:
+            try:
+                sib = self.siblings[plugin_name]
+            except (KeyError,):
+                sib = None
+            else:
+                if isinstance(sib, (models.Provider,)):
+                    pop_list.append(plugin_name)
+        for p in pop_list:
+            cfg.pop(p)
+        LOGGER.critical(f"Writing {config_path.absolute()}")
+        from pynchon.util.text import dumpf
+
+        dumpf.json(cfg, file=config_path)
+
     @cli.click.flag("--bash", help="bootstrap bash")
     @cli.click.flag("--bashrc", help="bootstrap bashrc")
     @cli.click.flag("--bash-completions", help="bootstrap completions")
     @cli.click.flag("--pynchon", help="bootstrap .pynchon.json5")
     @cli.click.flag("--makefile", help="bootstrap Makefile")
     @cli.click.flag("--tox", help="bootstrap tox")
     def bootstrap(
@@ -115,21 +147,15 @@
         #     content = tmpl.render(pynchon_completions_script=pynchon_completions_script)
         #     files.dumps(content=content, file=bashrc_snippet, logger=LOGGER.info)
         #     return files.block_in_file(
         #         target_file=abcs.Path("~/.bashrc").expanduser(),
         #         block_file=bashrc_snippet,
         #     )
         elif pynchon:
-            tmp = abcs.Path(".") / ".pynchon.json5"
-            if tmp.exists():
-                err = f"Cowardly refusing to recreate {tmp}"
-                LOGGER.critical(err)
-                raise SystemExit(1)
-            else:
-                print("pynchon pattern sync . docs --plan")
+            return self.init()
         elif bash:
             this_cmd = "pynchon bootstrap --bash"  # FIXME: get from click-ctx
             LOGGER.debug("collecting `shell_aliases` from all plugins")
             out = self.siblings.collect_config_dict("shell_aliases")
             out = "\n".join([f"alias {k}='{v}';" for k, v in out.items()])
             print(out)
             LOGGER.warning(f'for this session, use "source <({this_cmd})"')
@@ -155,18 +181,20 @@
             p
             for p in plugins
             if isinstance(p, models.AbstractPlanner) and p.contribute_plan_apply
         ]
         plugins = sorted(plugins, key=lambda p: p.priority)
         return plugins
 
+    @cli.options.quiet
     def plan(
         self,
         config=None,
-        flattened=True,
+        quiet: bool = False,
+        flattened: bool = True,
     ) -> models.Plan:
         """Runs plan for all plugins"""
 
         config = config or self.project_config
         plan = super(self.__class__, self).plan(config)
         plans = [] if not flattened else None
         plugins = self.sorted_plugins
@@ -180,19 +208,20 @@
             else:
                 if flattened:
                     for g in subplan.goals:
                         self.logger.info(f"{plugin_obj} contributes {g}")
                         plan.append(g)
                 else:
                     plans.append(subplan)
-        return plan.finalize() if flattened else plans
+        result = plan.finalize() if flattened else plans
+        return result if not quiet else None
 
     @cli.click.option("--parallelism", "-p", default="1", help="Paralellism")
-    @cli.click.flag("--fail-fast", default=False, help="fail fast")
-    @cli.click.flag("--quiet", "-q", default=False, help="Disable JSON output")
+    @cli.click.flag("--fail-fast", "-f", default=False, help="fail fast")
+    @cli.options.quiet
     def apply(
         self,
         plan: planning.Plan = None,
         parallelism: str = "1",
         quiet: bool = False,
         fail_fast: bool = False,
     ) -> planning.ApplyResults:
```

### Comparing `pynchon-2024.3.5.19.3/src/pynchon/plugins/deck.py` & `pynchon-2024.4.3.17.11/src/pynchon/plugins/deck.py`

 * *Files identical despite different names*

### Comparing `pynchon-2024.3.5.19.3/src/pynchon/plugins/docs/main.py` & `pynchon-2024.4.3.17.11/src/pynchon/plugins/docs/main.py`

 * *Files identical despite different names*

### Comparing `pynchon-2024.3.5.19.3/src/pynchon/plugins/docs/opener.py` & `pynchon-2024.4.3.17.11/src/pynchon/plugins/docs/opener.py`

 * *Files 12% similar despite different names*

```diff
@@ -25,18 +25,15 @@
     (In the future other file-types like `.dot` for raw
     graphviz might be supported, but for now you'll still
     have to render those to png to see a picture.)
     """
 
     def _open_grip(self, file: str = None):
         """
-
-        :param file: str:  (Default value = None)
         :param file: str:  (Default value = None)
-
         """
         pfile = abcs.Path(file).absolute()
         relf = pfile.relative_to(abcs.Path(self.git_root))
         port = self.server.port
         if port is None:
             LOGGER.critical("no server yet..")
             self.serve()
@@ -52,17 +49,22 @@
     _open__mmd = _open_grip
 
     def _open_raw(self, file: str = None, server=None):
         """
         :param file: str:  (Default value = None)
         :param server: Default value = None)
         """
-        relf = file.absolute().relative_to(abcs.Path(self.git_root))
-        return self._open_grip(abcs.Path("__raw__") / relf)
+        # relf = file.absolute().relative_to(abcs.Path(self.git_root))
+        import webbrowser
+
+        return webbrowser.open(
+            f"file://{file.absolute()}"
+        )  # return self._open_grip(abcs.Path("__raw__") / relf)
 
     _open__html = _open_raw
     _open__png = _open_raw
     _open__jpg = _open_raw
     _open__jpeg = _open_raw
     _open__gif = _open_raw
     _open__svg = _open_raw
     _open__htm = _open__html
+    _open__pdf = _open_raw
```

### Comparing `pynchon-2024.3.5.19.3/src/pynchon/plugins/dot.py` & `pynchon-2024.4.3.17.11/src/pynchon/plugins/dot.py`

 * *Files 5% similar despite different names*

```diff
@@ -30,15 +30,15 @@
         result = files.find_globs(search)
         self.logger.debug(f"found {len(result)} files (pre-filter)")
         excludes = self["exclude_patterns" :: self[:"globals.exclude_patterns":]]
         self.logger.debug(f"filtering search with {len(excludes)} excludes")
         result = [p for p in result if not p.match_any_glob(excludes)]
         self.logger.debug(f"found {len(result)} files (post-filter)")
         if not result:
-            err = "jinja-plugin is included in this config, but found no .j2 files!"
+            err = f"{self.name} plugin is included in this config, but found no .dot files!"
             self.logger.critical(err)
         return result
 
     @cli.options.output
     @cli.click.option("--img", default="nshine/dot")
     @cli.click.option("--output-mode")
     @cli.click.argument("file", nargs=1)
```

### Comparing `pynchon-2024.3.5.19.3/src/pynchon/plugins/fixme.py` & `pynchon-2024.4.3.17.11/src/pynchon/plugins/fixme.py`

 * *Files identical despite different names*

### Comparing `pynchon-2024.3.5.19.3/src/pynchon/plugins/gen.py` & `pynchon-2024.4.3.17.11/src/pynchon/plugins/gen.py`

 * *Files identical despite different names*

### Comparing `pynchon-2024.3.5.19.3/src/pynchon/plugins/git.py` & `pynchon-2024.4.3.17.11/src/pynchon/plugins/git.py`

 * *Files identical despite different names*

### Comparing `pynchon-2024.3.5.19.3/src/pynchon/plugins/github.py` & `pynchon-2024.4.3.17.11/src/pynchon/plugins/github.py`

 * *Files 4% similar despite different names*

```diff
@@ -24,40 +24,49 @@
         config_key: typing.ClassVar[str] = "github"
         enterprise: bool = typing.Field(default=False)
         org_name: str = typing.Field(default=None)
         org_url: str = typing.Field(default=None)
         repo_url: str = typing.Field(default=None)
         actions: typing.List[abcs.Path] = typing.Field(default=[None])
         raw_url: str = typing.Field(default=None)
+        repo_ssh_url: str = typing.Field(default=None)
 
         @property
         def raw_url(self):
             return f"https://raw.githubusercontent.com/{self.org_name}/{config.git.repo_name}"
 
         @property
         def actions(self) -> typing.List[typing.Dict]:
             """ """
-            wflows = abcs.Path(config.git.root) / ".github" / "workflows"
-            if wflows.exists():
-                return [
-                    dict(
-                        name=fname,
-                        file=wflows / fname,
-                        url=f"{self.repo_url}/actions/workflows/{fname}",
-                    )
-                    for fname in wflows.list()
-                ]
-            else:
-                return []
+            groot = config.git.root
+            if groot:
+                wflows = abcs.Path(groot) / ".github" / "workflows"
+                if wflows.exists():
+                    return [
+                        dict(
+                            name=fname,
+                            file=wflows / fname,
+                            url=f"{self.repo_url}/actions/workflows/{fname}",
+                        )
+                        for fname in wflows.list()
+                    ]
+            return []
 
         @property
         def repo_url(self):
             return config.git.repo_url
 
         @property
+        def repo_ssh_url(self):
+            if self.repo_url:
+                return (
+                    f"git@github.com:{self.org_name}/{self.repo_url.split('/')[-1]}.git"
+                )
+
+        @property
         def org_url(self):
             return f"https://github.com/{self.org_name}"
 
         @property
         def org_name(self):
             return config.git.github_org
```

### Comparing `pynchon-2024.3.5.19.3/src/pynchon/plugins/griffe.py` & `pynchon-2024.4.3.17.11/src/pynchon/plugins/griffe.py`

 * *Files identical despite different names*

### Comparing `pynchon-2024.3.5.19.3/src/pynchon/plugins/jinja.py` & `pynchon-2024.4.3.17.11/src/pynchon/plugins/jinja.py`

 * *Files 22% similar despite different names*

```diff
@@ -10,20 +10,22 @@
 LOGGER = lme.get_logger(__name__)
 
 
 @tagging.tags(click_aliases=["j"])
 class Jinja(models.Planner):
     """Renders files with {jinja.template_includes}"""
 
+    file_glob = "*.j2"
     # diff --color --minimal -w --side-by-side /etc/bash.bashrc <(bash --pretty-print /etc/bash.bashrc )
 
     class config_class(abcs.Config):
         config_key: typing.ClassVar[str] = "jinja"
         template_includes: typing.List[str] = typing.Field(default=[])
         exclude_patterns: typing.List[str] = typing.Field()
+        vars: typing.Dict[str, str] = typing.Field(default={}, help="")
 
         # @tagging.tagged_property(conflict_strategy="override")
         @property
         def exclude_patterns(self):
             from pynchon.config import globals
 
             # globals = plugin_util.get_plugin("globals").get_current_config()
@@ -35,19 +37,14 @@
     priority = 7
     COMMAND_TEMPLATE = (
         "python -mpynchon.util.text render jinja "
         "{src} --context-file {context_file} "
         "--output {output} {template_args}"
     )
 
-    # cli_subsumes: typing.List[typing.Callable] = [
-    #     # render_main.j2cli,
-    #     # render_main.jinja_file,
-    # ]
-
     def _get_jinja_context(self):
         """ """
         fname = ".tmp.jinja.ctx.json"
         with open(fname, "w") as fhandle:
             fhandle.write(text.to_json(self.project_config))
         return f"{fname}"
 
@@ -94,36 +91,19 @@
                     out.append(fname)
                 break
             else:
                 pass
         return out
 
     @tagging.tags(click_aliases=["ls"])
-    def list(self, changes=False):
+    def list(self, changes=False, **kwargs):
         """
         Lists affected resources for this project
         """
-        default = self[:"project"]
-        proj_conf = self[:"project.subproject":default]
-        project_root = proj_conf.get("root", None) or self[:"git.root":"."]
-        # project_root = proj_conf.get("root", None) or '.'
-        globs = [
-            abcs.Path(project_root).joinpath("**/*.j2"),
-        ]
-        self.logger.debug(f"search patterns are {globs}")
-        result = files.find_globs(globs)
-        self.logger.debug(f"found {len(result)} j2 files (pre-filter)")
-        excludes = self["exclude_patterns"]
-        self.logger.debug(f"filtering search with {len(excludes)} excludes")
-        result = [p for p in result if not p.match_any_glob(excludes)]
-        self.logger.debug(f"found {len(result)} j2 files (post-filter)")
-        if not result:
-            err = f"{self.__class__.__name__} is active, but found no .j2 files!"
-            self.logger.critical(err)
-        return result
+        return self._list(changes=changes, **kwargs)
 
     def plan(
         self,
         config=None,
     ) -> typing.List:
         """Creates a plan for this plugin"""
```

### Comparing `pynchon-2024.3.5.19.3/src/pynchon/plugins/json.py` & `pynchon-2024.4.3.17.11/src/pynchon/plugins/json.py`

 * *Files identical despite different names*

### Comparing `pynchon-2024.3.5.19.3/src/pynchon/plugins/makefile.py` & `pynchon-2024.4.3.17.11/src/pynchon/plugins/makefile.py`

 * *Files identical despite different names*

### Comparing `pynchon-2024.3.5.19.3/src/pynchon/plugins/markdown.py` & `pynchon-2024.4.3.17.11/src/pynchon/plugins/markdown.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,58 +1,95 @@
 """ pynchon.plugins.markdown
 """
 
 import marko
+from bs4 import BeautifulSoup
 from fleks import tagging
-from marko.ast_renderer import ASTRenderer
 
 from pynchon import abcs, api, cli, events, models  # noqa
-from pynchon.util import lme, typing  # noqa
+from pynchon.util import files, lme, text, typing  # noqa
 
 LOGGER = lme.get_logger(__name__)
 
 ElementList = typing.List[typing.Dict]
-# from pynchon.plugins.tests import DocTestSuite
-# markdown_suite = DocTestSuite(
-#     suite_name="markdown",
-# )
 
 
 class Markdown(models.Planner):
-    """Markdown"""
+    """
+    Example usage:
+        # normalize markdown syntax (in-place)
+        $ pynchon markdown normalize file1 file2
+    """
 
     class config_class(abcs.Config):
         config_key: typing.ClassVar[str] = "markdown"
         goals: typing.List[str] = typing.Field(default=[])
         include_patterns: typing.List[str] = typing.Field(default=[])
         exclude_patterns: typing.List[str] = typing.Field(default=[])
         root: typing.Union[str, abcs.Path, None] = typing.Field(default=None)
         linter_docker_image: str = typing.Field(
             default="peterdavehello/markdownlint", help=""
         )
-        linter_args: str = typing.Field(default="--fix", help="")
+        linter_args: typing.List[str] = typing.Field(
+            help="arguments to pass to `linter_docker_image`",
+            default=[
+                "--disable MD013",  # line-length
+                "--disable MD045",  # Images should have alternate text
+                "--disable MD033",  # Allow HTML
+                "--disable MD041",  # first-line-h1
+                "--disable MD042",  # No empty links
+                "--fix",
+            ],
+        )
         goals: typing.List[typing.Dict] = typing.Field(default=[], help="")
 
     name = "markdown"
-    # @cli.click.flag("-p", "--python", help="only python codeblocks")
     cli_name = "markdown"
     priority = 0
 
+    @tagging.tags(click_aliases=["ls"])
+    def list(self, changes=False):
+        """
+        Lists affected resources for this project
+        """
+        default = self[:"project"]
+        proj_conf = self[:"project.subproject":default]
+        project_root = proj_conf.get("root", None) or self[:"git.root":"."]
+        # project_root = proj_conf.get("root", None) or '.'
+        globs = [
+            abcs.Path(project_root).joinpath("**/*.md"),
+        ]
+        self.logger.debug(f"search patterns are {globs}")
+        result = files.find_globs(globs)
+        self.logger.debug(f"found {len(result)} j2 files (pre-filter)")
+        excludes = self["exclude_patterns"]
+        self.logger.debug(f"filtering search with {len(excludes)} excludes")
+        result = [p for p in result if not p.match_any_glob(excludes)]
+        self.logger.debug(f"found {len(result)} j2 files (post-filter)")
+        if not result:
+            err = f"{self.__class__.__name__} is active, but found no .j2 files!"
+            self.logger.critical(err)
+        return result
+
     @cli.click.argument("paths", nargs=-1)
     def normalize(self, paths):
         """Use `markdownlint` to normalize input paths"""
         docker_image = self["linter_docker_image"]
-        linter_args = self["linter_args"]
+        linter_args = " ".join(self["linter_args"])
         goals = []
         for path in paths:
             goals.append(
                 self.goal(
                     resource=path,
                     type="normalize",
-                    command=f"docker run -v `pwd`:/workspace -w /workspace {docker_image} markdownlint {linter_args} {path}",
+                    command=(
+                        f"docker run -v `pwd`:/workspace "
+                        f"-w /workspace {docker_image} "
+                        f"markdownlint {linter_args} {path}"
+                    ),
                 )
             )
         return self.apply(plan=self.plan(goals=goals))
 
     @cli.click.flag("-p", "--python", help="only python codeblocks")
     @cli.click.flag("-b", "--bash", help="only bash codeblocks")
     @cli.click.argument("file")
@@ -80,104 +117,61 @@
             el.update(_doctest(el))
         return element_lst
 
     @tagging.tags(click_aliases=["parse.markdown"])
     @cli.click.flag("-c", "--codeblocks", help="only codeblocks")
     @cli.click.flag("-p", "--python", help="only python codeblocks")
     @cli.click.flag("-b", "--bash", help="only bash codeblocks")
-    @cli.click.argument("file")
+    @cli.click.flag("-l", "--links", help="only links")
+    @cli.click.flag("--all", "-a", help="run for each file found by `list`")
+    @cli.click.argument("files", nargs=-1)
     def parse(
         self,
-        file: str = None,
+        files: typing.Tuple = tuple(),
+        all: bool = False,
         codeblocks: bool = False,
         python: bool = False,
+        links: bool = False,
         bash: bool = False,
     ) -> ElementList:
         """Parses given markdown file into JSON"""
+
         codeblocks = codeblocks or python or bash
-        assert file
-        with open(file) as fhandle:
-            content = fhandle.read()
-
-        parsed = marko.Markdown(renderer=ASTRenderer)(content)
-        # def walk(thing):
-        #     LOGGER.critical(thing)
-        #     if isinstance(thing, (dict,)):
-        #         children = thing.pop('children', [])
-        #         if isinstance(children,(str,)):
-        #             return children
-        #         if not children:
-        #             return thing
-        #         else:
-        #             return [walk(ch) for ch in children]
-        #     if isinstance(thing, (list,)):
-        #         return [walk(x) for x in thing]
-        #     else:
-        #         return thing
-        #
-        children = parsed["children"]
-        out = []
-        for child in children:
-            if child.get("element") == "fenced_code":
-                lang = child.get("lang")
-                if lang is not None:
-                    out.append(child)
-        LOGGER.critical(child)
-        if python:
-            out = [ch for ch in out if child.get("lang") == "python"]
-        if bash:
-            out = [ch for ch in out if child.get("lang") == "bash"]
-        # out=[]
-        # for child in children:
-        #     if bash and lang=='bash':
-        #         child['code'] = ''.join([
-        #             x['children'] for x in tmp ])
-        #         out.append(child)
-        #     elif python and lang=='python':
-        #         child['code'] = ''.join([
-        #             x['children'] for x in tmp ])
-        #         out.append(child)
-
-        return out
-        # for child in children:
-        #     result import pydash
-        # flat = pydash.flatten_deep(children)
-        # flat = [pydash.flatten_deep(x) for x in flat]
-        # if codeblocks:
-        #     result = [x for x in flat if x.get("element") == "fenced_code"]
-        # if python:
-        #     assert not bash
-        #     result = [x for x in result if x.get("lang") == "python"]
-        # if bash:
-        #     assert not python
-        #     result = [x for x in result if x.get("lang") == "bash"]
-        # import IPython; IPython.embed()
-        # return result
-
-    # plan=None
-    # def plan(self, config=None):
-    #     """Describe plan for this plugin"""
-    #     plan = super().plan(config=config)
-    #     return plan
-    # resources = [abcs.Path(fsrc) for fsrc in self.list()]
-    # self.logger.warning("Adding user-provided goals")
-    # for g in self["goals"]:
-    #     plan.append(self.goal(command=g, resource="?", type="user-config"))
-    #
-    # self.logger.warning("Adding file-header related goals")
-    # cmd_t = "python -mpynchon.util.files prepend --clean "
-    # loop = self._get_missing_headers(resources)
-    # for rsrc in loop["files"]:
-    #     if rsrc.match_any_glob(self["exclude_patterns"::[]]):
-    #         continue
-    #     ext = rsrc.full_extension()
-    #     ext = ext[1:] if ext.startswith(".") else ext
-    #     # fhdr = header_files[ext]
-    #     fhdr = self._render_header_file(rsrc)
-    #     plan.append(
-    #         self.goal(
-    #             resource=rsrc,
-    #             type="change",
-    #             label=f"Adding file header for '{ext}'",
-    #             command=f"{cmd_t} {fhdr} {rsrc}",
-    #         )
-    #     )
+        assert files or all and not (files and all)
+        if files:
+            files = list(files)
+        else:
+            files = self.list()
+            LOGGER.warning(f"parsing all markdown from: {files} ")
+        out = {}
+        for file in files:
+            LOGGER.warning(f"parsing: {file}")
+            file = str(file)
+            with open(file) as fhandle:
+                content = fhandle.read()
+            if links:
+                parsed = marko.Markdown()(content)
+                soup = BeautifulSoup(parsed, features="html.parser")
+                out[file] = []
+                for a in soup.find_all("a", href=True):
+                    this_link = a["href"]
+                    if this_link.strip() == "#":
+                        LOGGER.warning(f"{file}: has placeholder link '#' ")
+                    else:
+                        out[file] += [this_link]
+            else:
+                from marko.ast_renderer import ASTRenderer
+
+                parsed = marko.Markdown(renderer=ASTRenderer)(content)
+                children = parsed["children"]
+                out[file] = []
+                for child in children:
+                    if child.get("element") == "fenced_code":
+                        lang = child.get("lang")
+                        if lang is not None:
+                            out[file] += [child]
+                LOGGER.critical(child)
+                if python:
+                    out[file] += [ch for ch in out if child.get("lang") == "python"]
+                if bash:
+                    out[file] += [ch for ch in out if child.get("lang") == "bash"]
+        return {k: v for k, v in out.items() if v}
```

### Comparing `pynchon-2024.3.5.19.3/src/pynchon/plugins/mermaid.py` & `pynchon-2024.4.3.17.11/src/pynchon/plugins/mermaid.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,32 +1,37 @@
 """ pynchon.plugins.mermaid
+
+    See also:
+        * https://github.com/mermaid-js/mermaid-cli
+        * https://mermaid.live/
 """
 
 import os
 
 from fleks import cli, tagging
 
-from pynchon.util.os import invoke
-
 from pynchon import abcs, events, models  # noqa
 from pynchon.util import files, lme, typing  # noqa
 
 LOGGER = lme.get_logger(__name__)
-IMG = "ghcr.io/mermaid-js/mermaid-cli/mermaid-cli"
 
 
-class Mermaid(models.Planner):
+class Mermaid(models.DockerWrapper):
     """Mermaid Plugin"""
 
     class config_class(abcs.Config):
         config_key: typing.ClassVar[str] = "mermaid"
         apply_hooks: typing.List[str] = typing.Field(default=["open-after"])
+        docker_image: str = typing.Field(
+            default="ghcr.io/mermaid-js/mermaid-cli/mermaid-cli:10.8.1-beta.15"
+        )
 
     name = "mermaid"
     cli_name = "mermaid"
+    contribute_plan_apply = True
 
     @tagging.tags(click_aliases=["ls"])
     def list(self):
         """
         Find mermaid diagrams under `{{project_root}}/**/*.mmd`
         """
         includes = "**/*.mmd"
@@ -35,39 +40,36 @@
         ]
         self.logger.debug(f"search pattern is {search}")
         result = files.find_globs(search)
         return result
 
     @cli.options.output
     @cli.click.option("--img", default="nshine/dot")
-    # @cli.click.option("--output-mode")
     @cli.click.argument("file", nargs=1)
     def render(
         self,
         img: str = "??",
         file: str = "",
-        # output_mode: str = "",
         output: str = "",
     ):
         """
         Renders mermaid diagram to image
         """
         assert output
         wd = self.working_dir
         file = abcs.Path(file).absolute().relative_to(wd)
         output = abcs.Path(output)
         output = output.absolute().relative_to(wd)
         uid = os.getuid()
         cmd = (
             f"docker run -v {wd}:/workspace "
-            f"-w /workspace -u {uid} {IMG} -i {file} "
+            f"-w /workspace -u {uid} {self.config.docker_image} -i {file} "
             f"-o {output} --backgroundColor efefef"
         )
-        LOGGER.critical(cmd)
-        result = invoke(cmd, strict=True)
+        result = self._run_docker(cmd, strict=True)
         return True
 
     @property
     def output_root(self):
         return abcs.Path(self[:"git.root":]) / "img"
 
     def plan(
@@ -87,14 +89,7 @@
                     command=(
                         f"pynchon {self.cli_name} " f"render {inp} --output {rsrc} "
                     ),
                     type="render",
                 )
             )
         return plan
-
-    # cli_label = "Tool"
-    # def run(self):
-
-
-# mmdc -i input.mmd -o output.png -t dark -b transparent
-# https://github.com/mermaid-js/mermaid-cli
```

### Comparing `pynchon-2024.3.5.19.3/src/pynchon/plugins/mkdocs.py` & `pynchon-2024.4.3.17.11/src/pynchon/plugins/mkdocs.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """ pynchon.plugins.mkdocs
 """
 
 import urllib
 from pathlib import Path
 
 import yaml
+import fleks
 from fleks import tagging
 
 from pynchon.plugins import util as plugin_util
 from pynchon.util.text import loadf
 
 from pynchon import abcs, api, events, models  # noqa
 from pynchon.util import lme, typing  # noqa
@@ -187,25 +188,31 @@
         return result
 
     @tagging.tags(click_aliases=["ls"])
     def list(self):
         """Lists site-pages based on mkdocs.yml"""
         return self.config.pages
 
-    def open(self):
+    @fleks.cli.click.argument("files", nargs=-1)
+    def open(
+        self,
+        files: tuple = tuple(),
+    ):
         """
         Opens `dev_addr` in a webbrowser
         """
         import webbrowser
 
+        file = files[0] if files else "."
         # index_f = Path(self.site_dir).absolute() / "index.html"
         # url = f"file://{index_f}"
         mconfig = self.config.config
         url = mconfig["dev_addr"]
-        assert url
+        url = f"{url}/{file}" if file else url
+        url = f"http://{url}" if not url.startswith("http") else url
         self.logger.warning(f"opening {url}")
         return webbrowser.open(url)
 
     @property
     def site_dir(self) -> str:
         """
         Returns mkdocs `site_dir` if present in config, or guesses what it should be
```

### Comparing `pynchon-2024.3.5.19.3/src/pynchon/plugins/pattern.py` & `pynchon-2024.4.3.17.11/src/pynchon/plugins/pattern.py`

 * *Files identical despite different names*

### Comparing `pynchon-2024.3.5.19.3/src/pynchon/plugins/plugins.py` & `pynchon-2024.4.3.17.11/src/pynchon/plugins/plugins.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from pynchon.util.os import invoke
 
 from pynchon.util import lme, typing  # noqa
 
 LOGGER = lme.get_logger(__name__)
 
 
-class PluginsMan(models.Manager):
+class PluginsMan(models.Provider):
     """Meta-plugin for managing plugins"""
 
     name = "plugins"
     cli_name = "plugins"
 
     @cli.click.option("--name")
     @cli.click.option("--template-skeleton", "-t", is_flag=True, default=False)
```

### Comparing `pynchon-2024.3.5.19.3/src/pynchon/plugins/project.py` & `pynchon-2024.4.3.17.11/src/pynchon/plugins/project.py`

 * *Files 4% similar despite different names*

```diff
@@ -68,32 +68,36 @@
 
     name = "project"
     priority = 2
     config_class = ProjectConfig
 
     @tagging.tags(click_aliases=["ls"])
     def list(self):
-        """ """
+        """List subprojects associated with this project"""
         default = self[:"project"]
         proj_conf = self[:"project.subproject":default]
         project_root = proj_conf.get("root", None) or self[:"git.root":"."]
         # project_root = proj_conf.get("root", None) or '.'
         globs = [
             abcs.Path(project_root).joinpath("**/.pynchon.json5"),
         ]
         self.logger.warning(f"search patterns are {globs}")
         result = files.find_globs(globs)
         self.logger.debug(f"found {len(result)} subprojects (pre-filter)")
         excludes = self["exclude_patterns"]
         self.logger.debug(f"filtering search with {len(excludes)} excludes")
         result = [p for p in result if not p.match_any_glob(excludes)]
+        result = [
+            dict(
+                name=str(p.relative_to(abcs.Path(".").absolute()).parent), config_file=p
+            )
+            for p in result
+        ]
+        result = [r for r in result if r["name"] != "."]
         self.logger.debug(f"found {len(result)} subprojects (post-filter)")
-        # if not result:
-        #     err = f"{self.__class__.__name__} is active, but found no .j2 files!"
-        #     self.logger.critical(err)
         return result
 
     # @common.kommand(
     #     name="version",
     #     parent=parent,
     #     formatters=dict(markdown=constants.T_VERSION_METADATA),
     #     options=[
```

### Comparing `pynchon-2024.3.5.19.3/src/pynchon/plugins/python/api.py` & `pynchon-2024.4.3.17.11/src/pynchon/plugins/python/api.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 class PythonAPI(models.Planner):
     """Generators for Python API docs"""
 
     class config_class(abcs.Config):
         config_key: typing.ClassVar[str] = "python-api"
         skip_private_methods: bool = typing.Field(default=True)
         skip_patterns: typing.List[str] = typing.Field(default=[])
-        apply_hooks: typing.List[str] = typing.Field(default=["open-after"])
+        apply_hooks: typing.List[str] = typing.Field(default=["diff-after"])
 
     name = "python-api"
 
     @cli.click.group("gen")
     def gen(self):
         """Generates API docs from python modules, packages, etc"""
 
@@ -50,20 +50,19 @@
         file=None,
         exclude=None,
         output=None,
         stdout=None,
         header=None,
     ):
         """Generate table-of-contents"""
-
         T_TOC_API = render.get_template("pynchon/plugins/python/api/TOC.md.j2")
         module = complexity.get_module(package=package, file=file)
         result = complexity.visit_module(
             module=module,
-            module_name=package,
+            module_name=module.name,
             template=T_TOC_API,
             exclude=exclude.split(","),
         )
         header = f"{header}\n\n" if header else ""
         result = dict(
             header=f"## API for '{package}' package\n\n{header}" + "-" * 80,
             blocks=result,
```

### Comparing `pynchon-2024.3.5.19.3/src/pynchon/plugins/python/cli.py` & `pynchon-2024.4.3.17.11/src/pynchon/plugins/python/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -63,14 +63,57 @@
         # # src_root = abcs.Path(
         # # config_mod.project.get(
         # #     "src_root", config_mod.pynchon.get("src_root")
         # # )).absolute()
         return abcs.Path(src_root)
 
     @property
+    def console_script_entrypoints(self) -> typing.List[EntrypointMetadata]:
+        """ """
+        from pynchon.config import python  # noqa
+
+        package_entrypoints = python.package.console_scripts
+        out = []
+        for dct in package_entrypoints:
+            bin_name = dct["bin_name"]
+            module_name, fxn_name = dct["setuptools_entrypoint"].split(":")
+            dotpath = ".".join([module_name, fxn_name])
+            module = shimport.import_module(module_name)
+            fxn = getattr(module, fxn_name, None)
+            file = module.__file__
+            try:
+                abcs.Path(file).relative_to(self.src_root)
+                inside_src_root = True
+            except (ValueError,) as exc:
+                # ValueError: ... is not in the subpath of .. OR one path is relative and the other is absolute.
+                LOGGER.critical(
+                    f"script-entrypoint file @ `{file}` is not relative to source root at `{self.src_root}`!"
+                )
+                LOGGER.critical(
+                    "make sure you've installed this package in development mode with `pip install -e ..`"
+                )
+                inside_src_root = False
+            emd = EntrypointMetadata(
+                is_click=_check_click(fxn=fxn),
+                is_package_entrypoint=True,
+                file=file,
+                bin_name=bin_name,
+                inside_src_root=inside_src_root,
+                help_command=f"{bin_name} --help",
+                path=abcs.Path(file),
+                resource=self.root / f"script-{bin_name}.md",
+                src_root=self.src_root,
+                is_module=False,
+                dotpath=dotpath,
+            )
+            assert bin_name
+            out.append(emd)
+        return out
+
+    @property
     def module_entrypoints(self) -> typing.List[typing.Dict]:
         """ """
         src_root = self.src_root
         pat = src_root / "**" / "__main__.py"
         excludes = config_mod.src["exclude_patterns"]
         matches = glob.glob(str(pat), recursive=True)
         LOGGER.info(f"{len(matches)} matches for `entrypoints` filter")
@@ -135,38 +178,15 @@
                 abcs.Path(emeta["path"]).absolute()
                 for emeta in self.config.module_entrypoints
             ]
 
     @memoized_property
     def console_script_entrypoints(self) -> typing.List[EntrypointMetadata]:
         """ """
-        python_platform_config = self.siblings["python"].config
-        package_entrypoints = python_platform_config["package"]["console_scripts"]
-        out = []
-        for dct in package_entrypoints:
-            bin_name = dct["bin_name"]
-            module_name, fxn_name = dct["setuptools_entrypoint"].split(":")
-            dotpath = ".".join([module_name, fxn_name])
-            module = shimport.import_module(module_name)
-            fxn = getattr(module, fxn_name, None)
-            file = module.__file__
-            emd = EntrypointMetadata(
-                is_click=_check_click(fxn=fxn),
-                is_package=True,
-                file=file,
-                bin_name=bin_name,
-                help_command=f"{bin_name} --help",
-                path=abcs.Path(file),
-                resource=self.root / f"script-{dotpath}.md",
-                src_root=self.src_root,
-                is_module=False,
-                dotpath=dotpath,
-            )
-            out.append(emd)
-        return out
+        return self.config.console_script_entrypoints
 
     @gen.command("toc")
     @cli.options.header
     @cli.options.output
     def toc(
         self,
         # format, file, stdout,
@@ -174,22 +194,27 @@
         header,
     ) -> None:
         """
         Generate table-of-contents for all project entrypoints
         """
         output = output or self.root / "README.md"
         LOGGER.warning(f"writing toc to file: {output}")
-        entrypoints = self.console_script_entrypoints + self.config.module_entrypoints
+        cse = self.console_script_entrypoints
+        cme = self.config.module_entrypoints
+        LOGGER.warning(f"found {len(cse)} console-script-entrypoints")
+        LOGGER.warning(f"found {len(cme)} module-entrypoints")
+        entrypoints = cse + cme
+        # import IPython; IPython.embed()
         cfg = {**self.config.dict(), **dict(entrypoints=entrypoints)}
         cfg = {**api.project.get_config().dict(), **{self.config_class.config_key: cfg}}
         templatef = self.plugin_templates_root / "TOC.md.j2"
         tmpl = api.render.get_template(templatef)
         result = tmpl.render(
             # package_entrypoints=python_cli.entrypoints,
-            package_entrypoints=[e for e in entrypoints if e.is_package],
+            package_entrypoints=[e for e in entrypoints if e.is_package_entrypoint],
             main_entrypoints=[e for e in entrypoints if e.is_module],
             **cfg,
         )
         with open(str(output), "w") as fhandle:
             fhandle.write(result)
 
     def _click_recursive_help(
@@ -275,16 +300,17 @@
             LOGGER.warning(f"looking up module-entrypoint metadata for '{file}'")
             filtered = self.config["module_entrypoints"]
         found = False
         file = abcs.Path(file)
         for emd in filtered:
             if str(emd.path) == str(file):
                 if console_script:
-                    raise Exception(emd.dict())
+                    pass  # raise Exception(emd.dict())
                 else:
+                    # raise Exception(emd.module)
                     module = shimport.import_module(emd.module)
                     wrapped = shimport.wrapper(module)
                     click_entries = wrapped.filter(
                         only_functions=True, filter_vals=[_check_click]
                     )
                     click_entry = (
                         list(click_entries.items())[0] if click_entries else None
```

### Comparing `pynchon-2024.3.5.19.3/src/pynchon/plugins/python/libcst.py` & `pynchon-2024.4.3.17.11/src/pynchon/plugins/python/libcst.py`

 * *Files identical despite different names*

### Comparing `pynchon-2024.3.5.19.3/src/pynchon/plugins/python/platform.py` & `pynchon-2024.4.3.17.11/src/pynchon/plugins/python/platform.py`

 * *Files identical despite different names*

### Comparing `pynchon-2024.3.5.19.3/src/pynchon/plugins/python/pypi.py` & `pynchon-2024.4.3.17.11/src/pynchon/plugins/python/pypi.py`

 * *Files identical despite different names*

### Comparing `pynchon-2024.3.5.19.3/src/pynchon/plugins/release.py` & `pynchon-2024.4.3.17.11/src/pynchon/plugins/release.py`

 * *Files identical despite different names*

### Comparing `pynchon-2024.3.5.19.3/src/pynchon/plugins/render.py` & `pynchon-2024.4.3.17.11/src/pynchon/plugins/render.py`

 * *Files identical despite different names*

### Comparing `pynchon-2024.3.5.19.3/src/pynchon/plugins/scaffolding/__init__.py` & `pynchon-2024.4.3.17.11/src/pynchon/plugins/scaffolding/__init__.py`

 * *Files identical despite different names*

### Comparing `pynchon-2024.3.5.19.3/src/pynchon/plugins/scaffolding/config.py` & `pynchon-2024.4.3.17.11/src/pynchon/plugins/scaffolding/config.py`

 * *Files identical despite different names*

### Comparing `pynchon-2024.3.5.19.3/src/pynchon/plugins/src.py` & `pynchon-2024.4.3.17.11/src/pynchon/plugins/src.py`

 * *Files identical despite different names*

### Comparing `pynchon-2024.3.5.19.3/src/pynchon/plugins/tests.py` & `pynchon-2024.4.3.17.11/src/pynchon/plugins/tests.py`

 * *Files identical despite different names*

### Comparing `pynchon-2024.3.5.19.3/src/pynchon/plugins/util.py` & `pynchon-2024.4.3.17.11/src/pynchon/plugins/util.py`

 * *Files identical despite different names*

### Comparing `pynchon-2024.3.5.19.3/src/pynchon/templates/docker/Dockerfile.pandoc` & `pynchon-2024.4.3.17.11/src/pynchon/templates/docker/Dockerfile.pandoc`

 * *Files identical despite different names*

### Comparing `pynchon-2024.3.5.19.3/src/pynchon/templates/includes/pynchon/plugins/core/bootstrap/bash.sh` & `pynchon-2024.4.3.17.11/src/pynchon/templates/includes/pynchon/plugins/core/bootstrap/bash.sh`

 * *Files identical despite different names*

### Comparing `pynchon-2024.3.5.19.3/src/pynchon/templates/includes/pynchon/plugins/core/bootstrap/bashrc.sh` & `pynchon-2024.4.3.17.11/src/pynchon/templates/includes/pynchon/plugins/core/bootstrap/bashrc.sh`

 * *Files identical despite different names*

### Comparing `pynchon-2024.3.5.19.3/src/pynchon/templates/includes/pynchon/plugins/core/bootstrap/tox.ini` & `pynchon-2024.4.3.17.11/src/pynchon/templates/includes/pynchon/plugins/core/bootstrap/tox.ini`

 * *Files identical despite different names*

### Comparing `pynchon-2024.3.5.19.3/src/pynchon/templates/includes/pynchon/plugins/makefile/mermaid-graph.mmd.j2` & `pynchon-2024.4.3.17.11/src/pynchon/templates/includes/pynchon/plugins/makefile/mermaid-graph.mmd.j2`

 * *Files identical despite different names*

### Comparing `pynchon-2024.3.5.19.3/src/pynchon/templates/includes/pynchon/plugins/python/api/classes.md.j2` & `pynchon-2024.4.3.17.11/src/pynchon/templates/includes/pynchon/plugins/python/api/classes.md.j2`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
+{# #}
 
-
-* Classes: ({{classes|length}} total)
+* **Classes:** ({{classes|length}} total)
   {% for name,obj in classes.items() %}
   {% set qname = module_name+'.'+name %}
   {% set start, end = obj._metadata.start, obj._metadata.end %}
   {% set rel_url = '/' + base_url + '#L' + start %}
   {% set rel_url = rel_url+'-L' + end if end else rel_url %}
   {% set extras = obj._metadata.bases | default([]) %}
   {% set admonitions=[]%}
```

### Comparing `pynchon-2024.3.5.19.3/src/pynchon/templates/includes/pynchon/plugins/python/api/functions.md.j2` & `pynchon-2024.4.3.17.11/src/pynchon/templates/includes/pynchon/plugins/python/api/functions.md.j2`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 
 
-* Functions: ({{functions|length}} total)
+* **Functions:** ({{functions|length}} total)
   {% for name,obj in functions.items() %}
   {% set qname = module_name+'.'+name %}
   {% set start, end = obj.lineno | string, obj.endlineno | string %}
   {% set rel_url = '/' + base_url + '#L' + start + '-L' + end %}
   {% set extras = obj._metadata.signature|default('')|string %}
   {% set admonitions=[]%}
   {% set mccabe=obj._metadata.mccabe|default([])%}
```

### Comparing `pynchon-2024.3.5.19.3/src/pynchon/templates/includes/pynchon/plugins/python/api/package.md.j2` & `pynchon-2024.4.3.17.11/src/pynchon/templates/includes/pynchon/plugins/python/api/package.md.j2`

 * *Files 20% similar despite different names*

```diff
@@ -5,17 +5,17 @@
 {% set base_url = module._metadata.base_url|default('?') %}
 {% set entrypoint='(entrypoint) |' if module_name.endswith('__main__') else '' %}
 {% set utest_root = utest_root|default('/tests/units')%}
 {% set itest_root = itest_root|default('/tests/integrations')%}
 
 ### {{module_name}}
 
-* Overview: {{entrypoint}} [source code](/{{base_url}}), [unit tests]({{utest_root}}/), [integration tests]({{itest_root}}/)
-{% if modules %}
-{% include "pynchon/plugins/python/api/classes.md.j2" %}
+* **Overview:** {{entrypoint}} [source code](/{{base_url}}), [unit tests]({{utest_root}}/), [integration tests]({{itest_root}}/)
+{% if not (classes or functions) %}
+{% include "pynchon/plugins/python/api/names.md.j2" %}
 {% endif %}
 
 {% if classes %}
 {% include "pynchon/plugins/python/api/classes.md.j2" %}
 {% endif %}
 
 {% if functions %}
```

### Comparing `pynchon-2024.3.5.19.3/src/pynchon/templates/includes/pynchon/plugins/python/api/toc2.md.j2` & `pynchon-2024.4.3.17.11/src/pynchon/templates/includes/pynchon/plugins/python/api/toc2.md.j2`

 * *Files identical despite different names*

### Comparing `pynchon-2024.3.5.19.3/src/pynchon/templates/includes/pynchon/plugins/python_cli/TOC.md.j2` & `pynchon-2024.4.3.17.11/src/pynchon/templates/includes/pynchon/plugins/python_cli/TOC.md.j2`

 * *Files 9% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 {# 
-  TOC for python-cli docs-gen 
+  TOC for `python-cli docs-gen` 
 #}
 [tooltip-package-entrypoints]: ## "Console Script Entrypoints"
 [tooltip-module-entrypoints]: ## "Module Entrypoints"
 
 [Docs](../) *↔* [CLI](README.md) *↔* Console Scripts *↔* [Module Entrypoints](README.md#module-entrypoints)
 
 ---------------------------------------------------
@@ -17,15 +17,15 @@
 
 ### Package Entrypoints
 
 [Console scripts](https://python-packaging.readthedocs.io/en/latest/command-line-scripts.html#the-console-scripts-entry-point) published by package `{{python.package.name}}`:
 
 {% if package_entrypoints %}
 {% for metadata in package_entrypoints %}
-* [{{metadata.bin_name}}](/docs/cli/script-{{metadata.dotpath}}.md) via `{{metadata.dotpath}}` *[source]({{metadata.src_url}})*
+* [{{metadata.bin_name}}](/docs/cli/script-{{metadata.bin_name}}.md) via `{{metadata.dotpath}}` *[source]({{metadata.src_url}})*
 {%-endfor%}
 {%else%}
 No console scripts found
 {%endif%}
 
 -------------------------------------------------------------------------------
```

### Comparing `pynchon-2024.3.5.19.3/src/pynchon/templates/includes/pynchon/plugins/python_cli/main.module.md.j2` & `pynchon-2024.4.3.17.11/src/pynchon/templates/includes/pynchon/plugins/python_cli/main.module.md.j2`

 * *Files identical despite different names*

### Comparing `pynchon-2024.3.5.19.3/src/pynchon/templates/includes/pynchon/plugins/python_cli/script.console.md.j2` & `pynchon-2024.4.3.17.11/src/pynchon/templates/includes/pynchon/plugins/python_cli/script.console.md.j2`

 * *Files identical despite different names*

### Comparing `pynchon-2024.3.5.19.3/src/pynchon/templates/scaffolds/docker/.dockerignore` & `pynchon-2024.4.3.17.11/src/pynchon/templates/scaffolds/docker/.dockerignore`

 * *Files identical despite different names*

### Comparing `pynchon-2024.3.5.19.3/src/pynchon/templates/scaffolds/docker/README.md.j2` & `pynchon-2024.4.3.17.11/src/pynchon/templates/scaffolds/docker/README.md.j2`

 * *Files identical despite different names*

### Comparing `pynchon-2024.3.5.19.3/src/pynchon/templates/scaffolds/py/pkg/.libcst.codemod.yaml` & `pynchon-2024.4.3.17.11/src/pynchon/templates/scaffolds/py/pkg/.libcst.codemod.yaml`

 * *Files identical despite different names*

### Comparing `pynchon-2024.3.5.19.3/src/pynchon/templates/scaffolds/py/pkg/Makefile` & `pynchon-2024.4.3.17.11/src/pynchon/templates/scaffolds/py/pkg/Makefile`

 * *Files identical despite different names*

### Comparing `pynchon-2024.3.5.19.3/src/pynchon/templates/scaffolds/py/pkg/README.md.j2` & `pynchon-2024.4.3.17.11/src/pynchon/templates/scaffolds/py/pkg/README.md.j2`

 * *Files identical despite different names*

### Comparing `pynchon-2024.3.5.19.3/src/pynchon/templates/scaffolds/py/pkg/setup.cfg` & `pynchon-2024.4.3.17.11/src/pynchon/templates/scaffolds/py/pkg/setup.cfg`

 * *Files identical despite different names*

### Comparing `pynchon-2024.3.5.19.3/src/pynchon/templates/scaffolds/py/pkg/setup.py` & `pynchon-2024.4.3.17.11/src/pynchon/templates/scaffolds/py/pkg/setup.py`

 * *Files identical despite different names*

### Comparing `pynchon-2024.3.5.19.3/src/pynchon/templates/scaffolds/py/pkg/tox.ini` & `pynchon-2024.4.3.17.11/src/pynchon/templates/scaffolds/py/pkg/tox.ini`

 * *Files identical despite different names*

### Comparing `pynchon-2024.3.5.19.3/src/pynchon/util/__init__.py` & `pynchon-2024.4.3.17.11/src/pynchon/util/__init__.py`

 * *Files identical despite different names*

### Comparing `pynchon-2024.3.5.19.3/src/pynchon/util/complexity.py` & `pynchon-2024.4.3.17.11/src/pynchon/util/complexity.py`

 * *Files 24% similar despite different names*

```diff
@@ -16,31 +16,33 @@
 WORKING_DIR = Path(".")
 LOGGER = lme.get_logger(__name__)
 
 GLYPH_COMPLEXITY = constants.GLYPH_COMPLEXITY
 
 
 def clean_text(txt: str) -> str:
-    """
+    """ """
+    return "\n".join([line for line in txt.split("\n") if line.strip()])
 
-    :param txt: str:
-    :param txt: str:
 
-    """
-    return "\n".join([line for line in txt.split("\n") if line.strip()])
+def get_module_name_from_package(pkg_name):
+    """ """
+    import pkg_resources as pkg  # included in setuptools package
+
+    metadata_dir = pkg.get_distribution(pkg_name).egg_info
+    metadata_dir = Path(metadata_dir)
+    with open(str(metadata_dir / "top_level.txt")) as fhandle:
+        names = fhandle.read().rstrip().split("\n")
+    return names[0]
 
 
 def get_module(package: str = "", file: str = ""):
     """
-
     :param package: str:  (Default value = "")
     :param file: str:  (Default value = "")
-    :param package: str:  (Default value = "")
-    :param file: str:  (Default value = "")
-
     """
     if not bool(package) ^ bool(file):
         err = "Expected --file or --package, but not both"
         raise RuntimeError(err)
     if file:
         file = os.path.abspath(file)
         new_path = os.path.dirname(file)
@@ -48,15 +50,16 @@
         LOGGER.warning(f"modifying sys.path to include {new_path}")
         sys.path.append(new_path)
         package = os.path.splitext(os.path.basename(file))[0]
         working_dir = os.path.dirname(file)
     else:
         working_dir = WORKING_DIR
     loader = griffe.loader.GriffeLoader()
-    module = loader.load_module(package)
+    mod_name = get_module_name_from_package(package)
+    module = loader.load_module(mod_name)
     annotate.module(package, module, working_dir=working_dir)
     return module
 
 
 def get_refs(working_dir=None, module=None) -> dict:
     """
 
@@ -94,40 +97,47 @@
     module=None,
     template=None,
     visited=[],
     exclude: list = [],
     module_name=None,
     working_dir=WORKING_DIR,
 ):
-    """recursive visitor for this package, submodules, classes, functions, etc
+    """
+    Recursive visitor for this package, submodules, classes, functions, etc
 
     :param output: Default value = [])
     :param stats: Default value = {})
     :param module: Default value = None)
     :param template: Default value = None)
     :param visited: Default value = [])
     :param exclude: list:  (Default value = [])
     :param module_name: Default value = None)
     :param working_dir: Default value = WORKING_DIR)
     :param exclude: list:  (Default value = [])
 
     """
-    if module_name in exclude:
+    if any([module_name.split(".")[-1].startswith("_"), module_name in exclude]):
         LOGGER.debug(f"skipping module: {module_name}")
         return output
     annotate.module(module_name, module, working_dir=working_dir)
     refs = get_refs(working_dir=working_dir, module=module)
     # LOGGER.debug(f"exclude: {exclude}")
     LOGGER.debug(f"rendering module: {module_name}")
+    # import IPython; IPython.embed()
     rendered = template.render(
         griffe=griffe,
         stats=stats,
         working_dir=working_dir,
         module_name=module_name,
         module=module,
+        names=[
+            x
+            for x in module.members.keys()
+            if not any([x in exclude, x.startswith("_")])
+        ],
         **refs,
     )
     output.append(clean_text(rendered))
     for name, sub in refs["modules"].items():
         if sub in visited:
             continue
         visit_module(
```

### Comparing `pynchon-2024.3.5.19.3/src/pynchon/util/docker.py` & `pynchon-2024.4.3.17.11/src/pynchon/util/docker.py`

 * *Files identical despite different names*

### Comparing `pynchon-2024.3.5.19.3/src/pynchon/util/events.py` & `pynchon-2024.4.3.17.11/src/pynchon/util/events.py`

 * *Files identical despite different names*

### Comparing `pynchon-2024.3.5.19.3/src/pynchon/util/files/__init__.py` & `pynchon-2024.4.3.17.11/src/pynchon/util/files/__init__.py`

 * *Files identical despite different names*

### Comparing `pynchon-2024.3.5.19.3/src/pynchon/util/files/__main__.py` & `pynchon-2024.4.3.17.11/src/pynchon/util/files/__main__.py`

 * *Files identical despite different names*

### Comparing `pynchon-2024.3.5.19.3/src/pynchon/util/files/diff.py` & `pynchon-2024.4.3.17.11/src/pynchon/util/files/diff.py`

 * *Files identical despite different names*

### Comparing `pynchon-2024.3.5.19.3/src/pynchon/util/lme.py` & `pynchon-2024.4.3.17.11/src/pynchon/util/lme.py`

 * *Files identical despite different names*

### Comparing `pynchon-2024.3.5.19.3/src/pynchon/util/makefile/__init__.py` & `pynchon-2024.4.3.17.11/src/pynchon/util/makefile/__init__.py`

 * *Files identical despite different names*

### Comparing `pynchon-2024.3.5.19.3/src/pynchon/util/oop.py` & `pynchon-2024.4.3.17.11/src/pynchon/util/oop.py`

 * *Files identical despite different names*

### Comparing `pynchon-2024.3.5.19.3/src/pynchon/util/os/__init__.py` & `pynchon-2024.4.3.17.11/src/pynchon/util/os/__init__.py`

 * *Files identical despite different names*

### Comparing `pynchon-2024.3.5.19.3/src/pynchon/util/os/models.py` & `pynchon-2024.4.3.17.11/src/pynchon/util/os/models.py`

 * *Files identical despite different names*

### Comparing `pynchon-2024.3.5.19.3/src/pynchon/util/os/pids.py` & `pynchon-2024.4.3.17.11/src/pynchon/util/os/pids.py`

 * *Files identical despite different names*

### Comparing `pynchon-2024.3.5.19.3/src/pynchon/util/python.py` & `pynchon-2024.4.3.17.11/src/pynchon/util/python.py`

 * *Files identical despite different names*

### Comparing `pynchon-2024.3.5.19.3/src/pynchon/util/text/__init__.py` & `pynchon-2024.4.3.17.11/src/pynchon/util/text/__init__.py`

 * *Files identical despite different names*

### Comparing `pynchon-2024.3.5.19.3/src/pynchon/util/text/dumpf/__init__.py` & `pynchon-2024.4.3.17.11/src/pynchon/util/text/dumpf/__init__.py`

 * *Files identical despite different names*

### Comparing `pynchon-2024.3.5.19.3/src/pynchon/util/text/dumpf/__main__.py` & `pynchon-2024.4.3.17.11/src/pynchon/util/text/dumpf/__main__.py`

 * *Files identical despite different names*

### Comparing `pynchon-2024.3.5.19.3/src/pynchon/util/text/dumps.py` & `pynchon-2024.4.3.17.11/src/pynchon/util/text/dumps.py`

 * *Files identical despite different names*

### Comparing `pynchon-2024.3.5.19.3/src/pynchon/util/text/loadf/__init__.py` & `pynchon-2024.4.3.17.11/src/pynchon/util/text/loadf/__init__.py`

 * *Files identical despite different names*

### Comparing `pynchon-2024.3.5.19.3/src/pynchon/util/text/loadf/__main__.py` & `pynchon-2024.4.3.17.11/src/pynchon/util/text/loadf/__main__.py`

 * *Files identical despite different names*

### Comparing `pynchon-2024.3.5.19.3/src/pynchon/util/text/loads.py` & `pynchon-2024.4.3.17.11/src/pynchon/util/text/loads.py`

 * *Files identical despite different names*

### Comparing `pynchon-2024.3.5.19.3/src/pynchon/util/text/normalize/__init__.py` & `pynchon-2024.4.3.17.11/src/pynchon/util/text/normalize/__init__.py`

 * *Files identical despite different names*

### Comparing `pynchon-2024.3.5.19.3/src/pynchon/util/text/render/__init__.py` & `pynchon-2024.4.3.17.11/src/pynchon/util/text/render/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -28,26 +28,25 @@
     strict: bool = True,
 ):
     """Renders jinja-templates (with support for includes)
 
     :param text: str:  (Default value = "")
     :param file: str:  (Default value = "?")
     :param context: dict:  (Default value = {})
-    :param includes: typing.List[str]:  (Default value = [])
     :param strict: bool:  (Default value = True)
-    :param text: str:  (Default value = "")
-    :param file: str:  (Default value = "?")
-    :param context: dict:  (Default value = {})
     :param includes: typing.List[str]:  (Default value = [])
-    :param strict: bool:  (Default value = True)
 
     """
     import jinja2
 
-    template = api.get_template_from_string(text, env=api.get_jinja_env(*includes))
+    template = api.get_template_from_string(
+        text,
+        env=api.get_jinja_env(*includes),
+        template_name=file,
+    )
     context = {
         # FIXME: try to santize this
         **dict(os.environ.items()),
         **dict(__template__=file),
         **context,
     }
     try:
@@ -70,26 +69,19 @@
     file: str,
     context: typing.Dict = {},
     includes: typing.List[str] = [],
     strict: bool = True,
     quiet: bool = False,
 ) -> str:
     """
-
-    :param file: str:
-    :param context: typing.Dict:  (Default value = {})
-    :param includes: typing.List[str]:  (Default value = [])
-    :param strict: bool:  (Default value = True)
-    :param quiet: bool:  (Default value = False)
     :param file: str:
     :param context: typing.Dict:  (Default value = {})
     :param includes: typing.List[str]:  (Default value = [])
     :param strict: bool:  (Default value = True)
     :param quiet: bool:  (Default value = False)
-
     """
     context = {} if context is None else context
     LOGGER.debug(f"Running with one file: {file} (strict={strict})")
     with open(file) as fhandle:
         content = fhandle.read()
     quiet and LOGGER.debug(f"render context: \n{text.to_json(context)}")
     tmp = list(context.keys())
@@ -100,16 +92,14 @@
     #     env=api.get_jinja_env(*includes))
     return content
 
 
 @options.output
 @options.should_print
 @options.includes
-# @options.context
-# @options.context_file
 @click.option("--context", help="context literal.  must be JSON")
 @click.option("--context-file", help="context file.  must be JSON")
 @click.argument("file", nargs=1)
 @tags(
     click_aliases=["jinja"],
 )
 def jinja_file(
@@ -132,15 +122,14 @@
 
     content = jinja_loadf(
         file=file,
         context=context,
         includes=includes,
         strict=strict,
     )
-
     assert output
     output = os.path.splitext(output)
     if output[-1] == ".j2":
         output = output[0]
     else:
         output = "".join(output)
     LOGGER.warning(f"writing output to {output or sys.stdout.name}")
@@ -167,30 +156,25 @@
 @click.argument("file", nargs=1)
 @tags(
     click_aliases=["j2"],
 )
 def j2cli(
     output: str, should_print: bool, file: str, context: str, format: str = "json"
 ) -> None:
-    """A wrapper on the `j2` command (j2cli must be installed)
+    """
+    A wrapper on the `j2` command (j2cli must be installed)
     Renders the named file, using the given context-file.
 
     NB: No support for jinja-includes or custom filters.
 
-    :param output: str:
-    :param should_print: bool:
-    :param file: str:
-    :param context: str:
-    :param format: str:  (Default value = 'json')
-    :param output: str:
-    :param should_print: bool:
-    :param file: str:
-    :param context: str:
-    :param format: str:  (Default value = 'json')
-
+        :param output: str:
+        :param should_print: bool:
+        :param file: str:
+        :param context: str:
+        :param format: str:  (Default value = 'json')
     """
     cmd = f"j2 --format {format} {file} {context}"
     result = invoke(cmd)
     if not result.succeeded:
         LOGGER.critical(f"failed to execute: {cmd}")
         raise SystemExit(1)
     result = result.stdout
```

### Comparing `pynchon-2024.3.5.19.3/src/pynchon/util/text/render/__main__.py` & `pynchon-2024.4.3.17.11/src/pynchon/util/text/render/__main__.py`

 * *Files identical despite different names*

### Comparing `pynchon-2024.3.5.19.3/src/pynchon/util/typing.py` & `pynchon-2024.4.3.17.11/src/pynchon/util/typing.py`

 * *Files identical despite different names*

### Comparing `pynchon-2024.3.5.19.3/src/pynchon.egg-info/PKG-INFO` & `pynchon-2024.4.3.17.11/src/pynchon.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pynchon
-Version: 2024.3.5.19.3
+Version: 2024.4.3.17.11
 Summary: Autodocs for python projects
 Home-page: https://github.com/elo-enterprises/pynchon/
 Author: elo
 Author-email: engineering@elo.enterprises
 License: MIT
 Project-URL: Documentation, https://github.com/elo-enterprises/pynchon/
 Project-URL: Source, https://github.com/elo-enterprises/pynchon/
@@ -27,17 +27,17 @@
 Requires-Dist: tomli_w==1.0.0
 Requires-Dist: tomli
 Requires-Dist: griffe==0.23.0
 Requires-Dist: mccabe==0.7.0
 Requires-Dist: Jinja2==3.1.2
 Requires-Dist: grip==4.6.1
 Requires-Dist: psutil==5.9.5
-Provides-Extra: mkdocs
-Requires-Dist: mkdocs>=1.5.3; extra == "mkdocs"
-Requires-Dist: mkdocs-material==9.5.3; extra == "mkdocs"
+Requires-Dist: mkdocs>=1.5.3
+Requires-Dist: mkdocs-material==9.5.3
+Requires-Dist: beautifulsoup4==4.12.3
 Provides-Extra: dev
 Requires-Dist: IPython; extra == "dev"
 Provides-Extra: testing
 Requires-Dist: IPython; extra == "testing"
 Requires-Dist: tox; extra == "testing"
 Requires-Dist: pytest; extra == "testing"
 Requires-Dist: pytest-cov; extra == "testing"
```

### Comparing `pynchon-2024.3.5.19.3/src/pynchon.egg-info/SOURCES.txt` & `pynchon-2024.4.3.17.11/src/pynchon.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -46,25 +46,28 @@
 src/pynchon/config/util.py
 src/pynchon/models/__init__.py
 src/pynchon/models/planner.py
 src/pynchon/models/planning.py
 src/pynchon/models/python.py
 src/pynchon/models/plugins/__init__.py
 src/pynchon/models/plugins/cli.py
+src/pynchon/models/plugins/docker.py
 src/pynchon/models/plugins/provider.py
 src/pynchon/models/plugins/pynchon.py
 src/pynchon/models/plugins/tool.py
 src/pynchon/models/plugins/validators.py
 src/pynchon/plugins/__init__.py
 src/pynchon/plugins/__template__.py
 src/pynchon/plugins/api.py
 src/pynchon/plugins/cicd.py
 src/pynchon/plugins/core.py
 src/pynchon/plugins/deck.py
+src/pynchon/plugins/dockerhub.py
 src/pynchon/plugins/dot.py
+src/pynchon/plugins/drawio.py
 src/pynchon/plugins/fixme.py
 src/pynchon/plugins/gen.py
 src/pynchon/plugins/git.py
 src/pynchon/plugins/github.py
 src/pynchon/plugins/globals.py
 src/pynchon/plugins/griffe.py
 src/pynchon/plugins/hooks.py
@@ -114,14 +117,15 @@
 src/pynchon/templates/includes/pynchon/plugins/core/bootstrap/tox.ini
 src/pynchon/templates/includes/pynchon/plugins/fixme/FIXME.md.j2
 src/pynchon/templates/includes/pynchon/plugins/makefile/mermaid-graph.mmd.j2
 src/pynchon/templates/includes/pynchon/plugins/python/api/TOC.md.j2
 src/pynchon/templates/includes/pynchon/plugins/python/api/classes.md.j2
 src/pynchon/templates/includes/pynchon/plugins/python/api/functions.md.j2
 src/pynchon/templates/includes/pynchon/plugins/python/api/modules.md.j2
+src/pynchon/templates/includes/pynchon/plugins/python/api/names.md.j2
 src/pynchon/templates/includes/pynchon/plugins/python/api/package.md.j2
 src/pynchon/templates/includes/pynchon/plugins/python/api/toc2.md.j2
 src/pynchon/templates/includes/pynchon/plugins/python/gen/docstrings/function.txt.j2
 src/pynchon/templates/includes/pynchon/plugins/python/gen/docstrings/module.txt.j2
 src/pynchon/templates/includes/pynchon/plugins/python_cli/TOC.md.j2
 src/pynchon/templates/includes/pynchon/plugins/python_cli/detail.md.j2
 src/pynchon/templates/includes/pynchon/plugins/python_cli/main.module.md.j2
```

